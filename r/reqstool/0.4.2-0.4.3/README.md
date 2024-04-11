# Comparing `tmp/reqstool-0.4.2.tar.gz` & `tmp/reqstool-0.4.3.tar.gz`

## Comparing `reqstool-0.4.2.tar` & `reqstool-0.4.3.tar`

### file list

```diff
@@ -1,204 +1,204 @@
--rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 reqstool-0.4.2/.github/dependabot.yml
--rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 reqstool-0.4.2/.github/workflows/build.yml
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 reqstool-0.4.2/.github/workflows/check_release.yml
--rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 reqstool-0.4.2/.github/workflows/lint.yml
--rw-r--r--   0        0        0     1257 2020-02-02 00:00:00.000000 reqstool-0.4.2/.github/workflows/publish_gh_pages.yml
--rw-r--r--   0        0        0      859 2020-02-02 00:00:00.000000 reqstool-0.4.2/.github/workflows/publish_pypi_prod.yml
--rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 reqstool-0.4.2/.github/workflows/publish_pypi_test.yml
--rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 reqstool-0.4.2/docs/antora-playbook.yml
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 reqstool-0.4.2/docs/antora.yml
--rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 reqstool-0.4.2/docs/examples/requirements/manual_verification_results.yml
--rw-r--r--   0        0        0      921 2020-02-02 00:00:00.000000 reqstool-0.4.2/docs/examples/requirements/requirements_external.yml
--rw-r--r--   0        0        0     1598 2020-02-02 00:00:00.000000 reqstool-0.4.2/docs/examples/requirements/requirements_microservice.yml
--rw-r--r--   0        0        0     1715 2020-02-02 00:00:00.000000 reqstool-0.4.2/docs/examples/requirements/requirements_system.yml
--rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 reqstool-0.4.2/docs/examples/requirements/software_verification_cases.yml
--rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 reqstool-0.4.2/docs/modules/ROOT/nav.adoc
--rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 reqstool-0.4.2/docs/modules/ROOT/pages/background.adoc
--rw-r--r--   0        0        0    10790 2020-02-02 00:00:00.000000 reqstool-0.4.2/docs/modules/ROOT/pages/data.adoc
--rw-r--r--   0        0        0     3822 2020-02-02 00:00:00.000000 reqstool-0.4.2/docs/modules/ROOT/pages/file_and_directory_set.adoc
--rw-r--r--   0        0        0     6723 2020-02-02 00:00:00.000000 reqstool-0.4.2/docs/modules/ROOT/pages/how_it_works.adoc
--rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 reqstool-0.4.2/docs/modules/ROOT/pages/index.adoc
--rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 reqstool-0.4.2/docs/modules/ROOT/pages/installation.adoc
--rw-r--r--   0        0        0     1126 2020-02-02 00:00:00.000000 reqstool-0.4.2/docs/modules/ROOT/pages/overview.adoc
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 reqstool-0.4.2/docs/modules/ROOT/pages/quickstart.adoc
--rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 reqstool-0.4.2/docs/modules/ROOT/pages/terminology.adoc
--rw-r--r--   0        0        0     3433 2020-02-02 00:00:00.000000 reqstool-0.4.2/docs/modules/ROOT/pages/usage.adoc
--rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 reqstool-0.4.2/docs/modules/ROOT/pages/yml/annotations.adoc
--rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 reqstool-0.4.2/docs/modules/ROOT/pages/yml/manual_verification_results.adoc
--rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 reqstool-0.4.2/docs/modules/ROOT/pages/yml/reqstool_config.adoc
--rw-r--r--   0        0        0     2222 2020-02-02 00:00:00.000000 reqstool-0.4.2/docs/modules/ROOT/pages/yml/requirements.adoc
--rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 reqstool-0.4.2/docs/modules/ROOT/pages/yml/requirements_annotations.adoc
--rw-r--r--   0        0        0     1028 2020-02-02 00:00:00.000000 reqstool-0.4.2/docs/modules/ROOT/pages/yml/requirements_external.adoc
--rw-r--r--   0        0        0     2222 2020-02-02 00:00:00.000000 reqstool-0.4.2/docs/modules/ROOT/pages/yml/requirements_microservice.adoc
--rw-r--r--   0        0        0     1858 2020-02-02 00:00:00.000000 reqstool-0.4.2/docs/modules/ROOT/pages/yml/requirements_system.adoc
--rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 reqstool-0.4.2/docs/modules/ROOT/pages/yml/software_verification_cases.adoc
--rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 reqstool-0.4.2/docs/modules/ROOT/pages/yml/svcs_annotations.adoc
--rw-r--r--   0        0        0     3879 2020-02-02 00:00:00.000000 reqstool-0.4.2/docs/modules/ROOT/partials/C4_Component.puml
--rw-r--r--   0        0        0    14863 2020-02-02 00:00:00.000000 reqstool-0.4.2/docs/modules/ROOT/partials/C4_Sequence.puml
--rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 reqstool-0.4.2/docs/modules/examples/partials/requirements/manual_verification_results.yml
--rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 reqstool-0.4.2/docs/modules/examples/partials/requirements/reqstool_config.yml
--rw-r--r--   0        0        0      875 2020-02-02 00:00:00.000000 reqstool-0.4.2/docs/modules/examples/partials/requirements/requirements_external.yml
--rw-r--r--   0        0        0     1725 2020-02-02 00:00:00.000000 reqstool-0.4.2/docs/modules/examples/partials/requirements/requirements_microservice.yml
--rw-r--r--   0        0        0     1402 2020-02-02 00:00:00.000000 reqstool-0.4.2/docs/modules/examples/partials/requirements/requirements_system.yml
--rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 reqstool-0.4.2/docs/modules/examples/partials/requirements/software_verification_cases.yml
--rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 reqstool-0.4.2/docs/reqstool/manual_verification_results.yml
--rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 reqstool-0.4.2/docs/reqstool/reqstool_config.yml
--rw-r--r--   0        0        0    10690 2020-02-02 00:00:00.000000 reqstool-0.4.2/docs/reqstool/requirements.yml
--rw-r--r--   0        0        0     6822 2020-02-02 00:00:00.000000 reqstool-0.4.2/docs/reqstool/software_verification_cases.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 reqstool-0.4.2/src/reqstool/__init__.py
--rwxr-xr-x   0        0        0    10652 2020-02-02 00:00:00.000000 reqstool-0.4.2/src/reqstool/command.py
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 reqstool-0.4.2/src/reqstool/commands/exit_codes.py
--rw-r--r--   0        0        0     2942 2020-02-02 00:00:00.000000 reqstool-0.4.2/src/reqstool/commands/generate_json/generate_json.py
--rw-r--r--   0        0        0    10524 2020-02-02 00:00:00.000000 reqstool-0.4.2/src/reqstool/commands/report/report.py
--rw-r--r--   0        0        0     2735 2020-02-02 00:00:00.000000 reqstool-0.4.2/src/reqstool/commands/report/criterias/group_by.py
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 reqstool-0.4.2/src/reqstool/commands/report/criterias/sort_by.py
--rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 reqstool-0.4.2/src/reqstool/commands/report/templates/annotation_impls.j2
--rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 reqstool-0.4.2/src/reqstool/commands/report/templates/annotation_tests.j2
--rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 reqstool-0.4.2/src/reqstool/commands/report/templates/mvrs.j2
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 reqstool-0.4.2/src/reqstool/commands/report/templates/report.j2
--rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 reqstool-0.4.2/src/reqstool/commands/report/templates/req_references.j2
--rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 reqstool-0.4.2/src/reqstool/commands/report/templates/requirements.j2
--rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 reqstool-0.4.2/src/reqstool/commands/report/templates/svcs.j2
--rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 reqstool-0.4.2/src/reqstool/commands/report/templates/total_statistics.j2
--rw-r--r--   0        0        0     3055 2020-02-02 00:00:00.000000 reqstool-0.4.2/src/reqstool/commands/status/statistics_container.py
--rw-r--r--   0        0        0    13286 2020-02-02 00:00:00.000000 reqstool-0.4.2/src/reqstool/commands/status/statistics_generator.py
--rw-r--r--   0        0        0     9220 2020-02-02 00:00:00.000000 reqstool-0.4.2/src/reqstool/commands/status/status.py
--rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 reqstool-0.4.2/src/reqstool/common/jinja2.py
--rw-r--r--   0        0        0     9339 2020-02-02 00:00:00.000000 reqstool-0.4.2/src/reqstool/common/utils.py
--rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 reqstool-0.4.2/src/reqstool/common/validator_error_holder.py
--rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 reqstool-0.4.2/src/reqstool/common/dataclasses/urn_id.py
--rw-r--r--   0        0        0    12026 2020-02-02 00:00:00.000000 reqstool-0.4.2/src/reqstool/common/validators/semantic_validator.py
--rw-r--r--   0        0        0     2259 2020-02-02 00:00:00.000000 reqstool-0.4.2/src/reqstool/common/validators/syntax_validator.py
--rwxr-xr-x   0        0        0     2575 2020-02-02 00:00:00.000000 reqstool-0.4.2/src/reqstool/expression_languages/generic_el.py
--rwxr-xr-x   0        0        0      235 2020-02-02 00:00:00.000000 reqstool-0.4.2/src/reqstool/expression_languages/requirements_el.py
--rwxr-xr-x   0        0        0      203 2020-02-02 00:00:00.000000 reqstool-0.4.2/src/reqstool/expression_languages/svcs_el.py
--rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 reqstool-0.4.2/src/reqstool/filters/id_filters.py
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 reqstool-0.4.2/src/reqstool/filters/requirements_filters.py
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 reqstool-0.4.2/src/reqstool/filters/svcs_filters.py
--rw-r--r--   0        0        0     1698 2020-02-02 00:00:00.000000 reqstool-0.4.2/src/reqstool/location_resolver/location_resolver.py
--rw-r--r--   0        0        0     1272 2020-02-02 00:00:00.000000 reqstool-0.4.2/src/reqstool/locations/git_location.py
--rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 reqstool-0.4.2/src/reqstool/locations/local_location.py
--rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 reqstool-0.4.2/src/reqstool/locations/location.py
--rw-r--r--   0        0        0     1935 2020-02-02 00:00:00.000000 reqstool-0.4.2/src/reqstool/locations/maven_location.py
--rw-r--r--   0        0        0     1894 2020-02-02 00:00:00.000000 reqstool-0.4.2/src/reqstool/model_generators/annotations_model_generator.py
--rw-r--r--   0        0        0    29195 2020-02-02 00:00:00.000000 reqstool-0.4.2/src/reqstool/model_generators/combined_indexed_dataset_generator.py
--rw-r--r--   0        0        0    10755 2020-02-02 00:00:00.000000 reqstool-0.4.2/src/reqstool/model_generators/combined_raw_datasets_generator.py
--rw-r--r--   0        0        0     1559 2020-02-02 00:00:00.000000 reqstool-0.4.2/src/reqstool/model_generators/mvrs_model_generator.py
--rw-r--r--   0        0        0    12615 2020-02-02 00:00:00.000000 reqstool-0.4.2/src/reqstool/model_generators/requirements_model_generator.py
--rw-r--r--   0        0        0     4515 2020-02-02 00:00:00.000000 reqstool-0.4.2/src/reqstool/model_generators/svcs_model_generator.py
--rw-r--r--   0        0        0     2461 2020-02-02 00:00:00.000000 reqstool-0.4.2/src/reqstool/model_generators/testdata_model_generator.py
--rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 reqstool-0.4.2/src/reqstool/models/annotations.py
--rw-r--r--   0        0        0     1341 2020-02-02 00:00:00.000000 reqstool-0.4.2/src/reqstool/models/combined_indexed_dataset.py
--rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 reqstool-0.4.2/src/reqstool/models/implementations.py
--rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 reqstool-0.4.2/src/reqstool/models/imports.py
--rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 reqstool-0.4.2/src/reqstool/models/mvrs.py
--rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 reqstool-0.4.2/src/reqstool/models/raw_datasets.py
--rw-r--r--   0        0        0     2222 2020-02-02 00:00:00.000000 reqstool-0.4.2/src/reqstool/models/requirements.py
--rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 reqstool-0.4.2/src/reqstool/models/svcs.py
--rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 reqstool-0.4.2/src/reqstool/models/test_data.py
--rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 reqstool-0.4.2/src/reqstool/reqstool_config/reqstool_config.py
--rw-r--r--   0        0        0     5508 2020-02-02 00:00:00.000000 reqstool-0.4.2/src/reqstool/requirements_indata/requirements_indata.py
--rw-r--r--   0        0        0     2027 2020-02-02 00:00:00.000000 reqstool-0.4.2/src/reqstool/requirements_indata/requirements_indata_paths.py
--rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 reqstool-0.4.2/src/reqstool/requirements_indata/java/java_maven_requirements_indata_paths.py
--rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 reqstool-0.4.2/src/reqstool/requirements_indata/python/python_requirements_indata_paths.py
--rw-r--r--   0        0        0     2471 2020-02-02 00:00:00.000000 reqstool-0.4.2/src/reqstool/resources/schemas/v1/annotations.schema.json
--rw-r--r--   0        0        0    11023 2020-02-02 00:00:00.000000 reqstool-0.4.2/src/reqstool/resources/schemas/v1/common.schema.json
--rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 reqstool-0.4.2/src/reqstool/resources/schemas/v1/manual_verification_results.schema.json
--rw-r--r--   0        0        0     1315 2020-02-02 00:00:00.000000 reqstool-0.4.2/src/reqstool/resources/schemas/v1/reqstool_config.schema.json
--rw-r--r--   0        0        0    10841 2020-02-02 00:00:00.000000 reqstool-0.4.2/src/reqstool/resources/schemas/v1/requirements.schema.json
--rw-r--r--   0        0        0     2646 2020-02-02 00:00:00.000000 reqstool-0.4.2/src/reqstool/resources/schemas/v1/software_verification_cases.schema.json
--rw-r--r--   0        0        0     2120 2020-02-02 00:00:00.000000 reqstool-0.4.2/tests/integration/reqstool/model_generators/test_included_models_generator.py
--rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 reqstool-0.4.2/tests/resources/test_data/data/local/test_basic/baseline/ms-101/annotations.yml
--rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 reqstool-0.4.2/tests/resources/test_data/data/local/test_basic/baseline/ms-101/manual_verification_results.yml
--rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 reqstool-0.4.2/tests/resources/test_data/data/local/test_basic/baseline/ms-101/requirements.yml
--rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 reqstool-0.4.2/tests/resources/test_data/data/local/test_basic/baseline/ms-101/software_verification_cases.yml
--rw-r--r--   0        0        0     6367 2020-02-02 00:00:00.000000 reqstool-0.4.2/tests/resources/test_data/data/local/test_basic/baseline/ms-101/test_results/failsafe/TEST-com.example.RequirementsExampleTestsIT.xml
--rw-r--r--   0        0        0     5744 2020-02-02 00:00:00.000000 reqstool-0.4.2/tests/resources/test_data/data/local/test_basic/baseline/ms-101/test_results/surefire/TEST-com.example.RequirementsExampleTests.xml
--rw-r--r--   0        0        0     2724 2020-02-02 00:00:00.000000 reqstool-0.4.2/tests/resources/test_data/data/local/test_basic/layout_maven/ms-101/pom.xml
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 reqstool-0.4.2/tests/resources/test_data/data/local/test_basic/layout_maven/ms-101/src/resources/docs/requirements/manual_verification_results.yml -> ../../../../../../baseline/ms-101/manual_verification_results.yml
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 reqstool-0.4.2/tests/resources/test_data/data/local/test_basic/layout_maven/ms-101/src/resources/docs/requirements/requirements.yml -> ../../../../../../baseline/ms-101/requirements.yml
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 reqstool-0.4.2/tests/resources/test_data/data/local/test_basic/layout_maven/ms-101/src/resources/docs/requirements/software_verification_cases.yml -> ../../../../../../baseline/ms-101/software_verification_cases.yml
--rw-r--r--   0        0        0     3264 2020-02-02 00:00:00.000000 reqstool-0.4.2/tests/resources/test_data/data/local/test_basic/with_requirements_config/README.md
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 reqstool-0.4.2/tests/resources/test_data/data/local/test_basic/with_requirements_config/ms-101/manual_verification_results.yml -> ../../baseline/ms-101/manual_verification_results.yml
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 reqstool-0.4.2/tests/resources/test_data/data/local/test_basic/with_requirements_config/ms-101/reqstool_config.yml
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 reqstool-0.4.2/tests/resources/test_data/data/local/test_basic/with_requirements_config/ms-101/requirements.yml -> ../../baseline/ms-101/requirements.yml
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 reqstool-0.4.2/tests/resources/test_data/data/local/test_basic/with_requirements_config/ms-101/software_verification_cases.yml -> ../../baseline/ms-101/software_verification_cases.yml
--rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 reqstool-0.4.2/tests/resources/test_data/data/local/test_errors/ms-101/annotations.yml
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 reqstool-0.4.2/tests/resources/test_data/data/local/test_errors/ms-101/errors.adoc
--rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 reqstool-0.4.2/tests/resources/test_data/data/local/test_errors/ms-101/manual_verification_results.yml
--rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 reqstool-0.4.2/tests/resources/test_data/data/local/test_errors/ms-101/requirements.yml
--rw-r--r--   0        0        0      892 2020-02-02 00:00:00.000000 reqstool-0.4.2/tests/resources/test_data/data/local/test_errors/ms-101/software_verification_cases.yml
--rw-r--r--   0        0        0     6367 2020-02-02 00:00:00.000000 reqstool-0.4.2/tests/resources/test_data/data/local/test_errors/ms-101/test_results/failsafe/TEST-com.example.RequirementsExampleTestsIT.xml
--rw-r--r--   0        0        0     5744 2020-02-02 00:00:00.000000 reqstool-0.4.2/tests/resources/test_data/data/local/test_errors/ms-101/test_results/surefire/TEST-com.example.RequirementsExampleTests.xml
--rw-r--r--   0        0        0      944 2020-02-02 00:00:00.000000 reqstool-0.4.2/tests/resources/test_data/data/local/test_standard/baseline/visualization.adoc
--rw-r--r--   0        0        0     2059 2020-02-02 00:00:00.000000 reqstool-0.4.2/tests/resources/test_data/data/local/test_standard/baseline/ms-001/annotations.yml
--rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 reqstool-0.4.2/tests/resources/test_data/data/local/test_standard/baseline/ms-001/manual_verification_results.yml
--rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 reqstool-0.4.2/tests/resources/test_data/data/local/test_standard/baseline/ms-001/requirements.yml
--rw-r--r--   0        0        0     1375 2020-02-02 00:00:00.000000 reqstool-0.4.2/tests/resources/test_data/data/local/test_standard/baseline/ms-001/software_verification_cases.yml
--rw-r--r--   0        0        0     7126 2020-02-02 00:00:00.000000 reqstool-0.4.2/tests/resources/test_data/data/local/test_standard/baseline/ms-001/test_results/failsafe/TEST-com.reqstool.example.demo.DemoApplicationTestsIT.xml
--rw-r--r--   0        0        0     8258 2020-02-02 00:00:00.000000 reqstool-0.4.2/tests/resources/test_data/data/local/test_standard/baseline/ms-001/test_results/surefire/TEST-com.reqstool.example.demo.SVCsTest.xml
--rw-r--r--   0        0        0      817 2020-02-02 00:00:00.000000 reqstool-0.4.2/tests/resources/test_data/data/local/test_standard/baseline/sys-001/requirements.yml
--rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 reqstool-0.4.2/tests/resources/test_data/data/local/test_standard/baseline/sys-001/software_verification_cases.yml
--rw-r--r--   0        0        0      838 2020-02-02 00:00:00.000000 reqstool-0.4.2/tests/resources/test_data/data/local/test_standard/baseline/sys-001/ext-001/requirements.yml
--rw-r--r--   0        0        0     1199 2020-02-02 00:00:00.000000 reqstool-0.4.2/tests/resources/test_data/data/local/test_standard/baseline/sys-001/ext-002/requirements.yml
--rw-r--r--   0        0        0     2119 2020-02-02 00:00:00.000000 reqstool-0.4.2/tests/resources/test_data/data/local/test_standard/empty_ms/ms-001/annotations.yml
--rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 reqstool-0.4.2/tests/resources/test_data/data/local/test_standard/empty_ms/ms-001/requirements.yml
--rw-r--r--   0        0        0     7125 2020-02-02 00:00:00.000000 reqstool-0.4.2/tests/resources/test_data/data/local/test_standard/empty_ms/ms-001/test_results/failsafe/TEST-com.reqstool.example.demo.DemoApplicationTestsIT.xml
--rw-r--r--   0        0        0     8258 2020-02-02 00:00:00.000000 reqstool-0.4.2/tests/resources/test_data/data/local/test_standard/empty_ms/ms-001/test_results/surefire/TEST-com.reqstool.example.demo.SVCsTest.xml
--rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 reqstool-0.4.2/tests/resources/test_data/data/local/test_standard/empty_ms/sys-001/manual_verification_results.yml
--rw-r--r--   0        0        0     1426 2020-02-02 00:00:00.000000 reqstool-0.4.2/tests/resources/test_data/data/local/test_standard/empty_ms/sys-001/requirements.yml
--rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 reqstool-0.4.2/tests/resources/test_data/data/local/test_standard/empty_ms/sys-001/software_verification_cases.yml
--rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 reqstool-0.4.2/tests/resources/test_data/data/local/test_standard/empty_ms/sys-001/ext-001/requirements.yml
--rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 reqstool-0.4.2/tests/resources/test_data/data/local/test_standard/empty_ms/sys-001/ext-002/requirements.yml
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 reqstool-0.4.2/tests/resources/test_data/data/remote/test_standard/test_standard_maven_git/ms-001/annotations.yml -> ../../../../local/test_standard/baseline/ms-001/annotations.yml
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 reqstool-0.4.2/tests/resources/test_data/data/remote/test_standard/test_standard_maven_git/ms-001/manual_verification_results.yml -> ../../../../local/test_standard/baseline/ms-001/manual_verification_results.yml
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 reqstool-0.4.2/tests/resources/test_data/data/remote/test_standard/test_standard_maven_git/ms-001/requirements.yml -> ../../../../local/test_standard/baseline/ms-001/requirements.yml
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 reqstool-0.4.2/tests/resources/test_data/data/remote/test_standard/test_standard_maven_git/ms-001/software_verification_cases.yml -> ../../../../local/test_standard/baseline/ms-001/software_verification_cases.yml
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 reqstool-0.4.2/tests/resources/test_data/data/remote/test_standard/test_standard_maven_git/sys-001/annotations.yml -> ../../../../local/test_standard/baseline/sys-001/annotations.yml
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 reqstool-0.4.2/tests/resources/test_data/data/remote/test_standard/test_standard_maven_git/sys-001/manual_verification_results.yml -> ../../../../local/test_standard/baseline/sys-001/manual_verification_results.yml
--rw-r--r--   0        0        0     1414 2020-02-02 00:00:00.000000 reqstool-0.4.2/tests/resources/test_data/data/remote/test_standard/test_standard_maven_git/sys-001/requirements.yml
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 reqstool-0.4.2/tests/resources/test_data/data/remote/test_standard/test_standard_maven_git/sys-001/software_verification_cases.yml -> ../../../../local/test_standard/baseline/sys-001/software_verification_cases.yml
--rw-r--r--   0        0        0     1573 2020-02-02 00:00:00.000000 reqstool-0.4.2/tests/resources/unit/reqstool/model_generators/test_annotations_model_generator/test_annotations_model_generator/annotations.yml
--rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 reqstool-0.4.2/tests/resources/unit/reqstool/model_generators/test_mvrs_model_generator/test_mvrs_model_generator/manual_verification_results.yml
--rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 reqstool-0.4.2/tests/resources/unit/reqstool/model_generators/test_requirements_model_generator/test_external_requirements_model_generator/requirements.yml
--rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 reqstool-0.4.2/tests/resources/unit/reqstool/model_generators/test_requirements_model_generator/test_microservice_requirements_model_generator/requirements.yml
--rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 reqstool-0.4.2/tests/resources/unit/reqstool/model_generators/test_requirements_model_generator/test_rational_optional_model_generator/requirements.yml
--rw-r--r--   0        0        0     2047 2020-02-02 00:00:00.000000 reqstool-0.4.2/tests/resources/unit/reqstool/model_generators/test_requirements_model_generator/test_system_requirements_model_generator/requirements.yml
--rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 reqstool-0.4.2/tests/resources/unit/reqstool/model_generators/test_svcs_model_generator/test_svcs_model_generator/software_verification_cases.yml
--rw-r--r--   0        0        0     2212 2020-02-02 00:00:00.000000 reqstool-0.4.2/tests/unit/conftest.py
--rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 reqstool-0.4.2/tests/unit/reqstool/commands/generate_json/test_generate_json.py
--rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 reqstool-0.4.2/tests/unit/reqstool/commands/report/test_report.py
--rw-r--r--   0        0        0     1569 2020-02-02 00:00:00.000000 reqstool-0.4.2/tests/unit/reqstool/commands/report/criterias/test_criterias.py
--rw-r--r--   0        0        0     2693 2020-02-02 00:00:00.000000 reqstool-0.4.2/tests/unit/reqstool/commands/status/test_statistics_container.py
--rw-r--r--   0        0        0    18426 2020-02-02 00:00:00.000000 reqstool-0.4.2/tests/unit/reqstool/commands/status/test_statistics_generator.py
--rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 reqstool-0.4.2/tests/unit/reqstool/commands/status/test_status.py
--rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 reqstool-0.4.2/tests/unit/reqstool/common/test_locations.py
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 reqstool-0.4.2/tests/unit/reqstool/common/test_utils.py
--rw-r--r--   0        0        0     8209 2020-02-02 00:00:00.000000 reqstool-0.4.2/tests/unit/reqstool/common/validators/test_semantic_validator.py
--rw-r--r--   0        0        0     5305 2020-02-02 00:00:00.000000 reqstool-0.4.2/tests/unit/reqstool/expression_languages/test_requirements_el.py
--rw-r--r--   0        0        0     4054 2020-02-02 00:00:00.000000 reqstool-0.4.2/tests/unit/reqstool/expression_languages/test_svcs_el.py
--rw-r--r--   0        0        0     1321 2020-02-02 00:00:00.000000 reqstool-0.4.2/tests/unit/reqstool/filters/test_requirements_filters.py
--rw-r--r--   0        0        0     1362 2020-02-02 00:00:00.000000 reqstool-0.4.2/tests/unit/reqstool/filters/test_software_verification_cases_filters.py
--rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 reqstool-0.4.2/tests/unit/reqstool/locations/test_git_location.py
--rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 reqstool-0.4.2/tests/unit/reqstool/locations/test_local_location.py
--rw-r--r--   0        0        0     2192 2020-02-02 00:00:00.000000 reqstool-0.4.2/tests/unit/reqstool/model_generators/test_annotations_model_generator.py
--rw-r--r--   0        0        0     3369 2020-02-02 00:00:00.000000 reqstool-0.4.2/tests/unit/reqstool/model_generators/test_combined_indexed_dataset_generator.py
--rw-r--r--   0        0        0     3887 2020-02-02 00:00:00.000000 reqstool-0.4.2/tests/unit/reqstool/model_generators/test_combined_raw_datasets_generator.py
--rw-r--r--   0        0        0     1402 2020-02-02 00:00:00.000000 reqstool-0.4.2/tests/unit/reqstool/model_generators/test_mvrs_model_generator.py
--rw-r--r--   0        0        0    11130 2020-02-02 00:00:00.000000 reqstool-0.4.2/tests/unit/reqstool/model_generators/test_requirements_model_generator.py
--rw-r--r--   0        0        0     2258 2020-02-02 00:00:00.000000 reqstool-0.4.2/tests/unit/reqstool/model_generators/test_svcs_model_generator.py
--rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 reqstool-0.4.2/tests/unit/reqstool/model_generators/test_testdata_model_generator.py
--rw-r--r--   0        0        0      960 2020-02-02 00:00:00.000000 reqstool-0.4.2/tests/unit/reqstool/models/test_annotations.py
--rw-r--r--   0        0        0     2435 2020-02-02 00:00:00.000000 reqstool-0.4.2/tests/unit/reqstool/models/test_implementations.py
--rw-r--r--   0        0        0     2246 2020-02-02 00:00:00.000000 reqstool-0.4.2/tests/unit/reqstool/models/test_imports.py
--rw-r--r--   0        0        0     1044 2020-02-02 00:00:00.000000 reqstool-0.4.2/tests/unit/reqstool/models/test_mvrs.py
--rw-r--r--   0        0        0     2368 2020-02-02 00:00:00.000000 reqstool-0.4.2/tests/unit/reqstool/models/test_requirements.py
--rw-r--r--   0        0        0     2922 2020-02-02 00:00:00.000000 reqstool-0.4.2/tests/unit/reqstool/models/test_svcs.py
--rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 reqstool-0.4.2/tests/unit/reqstool/reqstool_config/test_reqstool_config.py
--rw-r--r--   0        0        0     1934 2020-02-02 00:00:00.000000 reqstool-0.4.2/tests/unit/reqstool/requirements_indata/test_requirements_indata_paths.py
--rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 reqstool-0.4.2/tests/unit/reqstool/resources/schemas/v1/test_json_schemas.py
--rw-r--r--   0        0        0     4213 2020-02-02 00:00:00.000000 reqstool-0.4.2/.gitignore
--rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 reqstool-0.4.2/LICENSE
--rw-r--r--   0        0        0     3264 2020-02-02 00:00:00.000000 reqstool-0.4.2/README.md
--rw-r--r--   0        0        0     1942 2020-02-02 00:00:00.000000 reqstool-0.4.2/pyproject.toml
--rw-r--r--   0        0        0     4177 2020-02-02 00:00:00.000000 reqstool-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 reqstool-0.4.3/.github/dependabot.yml
+-rw-r--r--   0        0        0     1219 2020-02-02 00:00:00.000000 reqstool-0.4.3/.github/workflows/build.yml
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 reqstool-0.4.3/.github/workflows/check_release.yml
+-rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 reqstool-0.4.3/.github/workflows/lint.yml
+-rw-r--r--   0        0        0     1257 2020-02-02 00:00:00.000000 reqstool-0.4.3/.github/workflows/publish_gh_pages.yml
+-rw-r--r--   0        0        0      859 2020-02-02 00:00:00.000000 reqstool-0.4.3/.github/workflows/publish_pypi_prod.yml
+-rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 reqstool-0.4.3/.github/workflows/publish_pypi_test.yml
+-rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 reqstool-0.4.3/docs/antora-playbook.yml
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 reqstool-0.4.3/docs/antora.yml
+-rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 reqstool-0.4.3/docs/examples/requirements/manual_verification_results.yml
+-rw-r--r--   0        0        0      921 2020-02-02 00:00:00.000000 reqstool-0.4.3/docs/examples/requirements/requirements_external.yml
+-rw-r--r--   0        0        0     1598 2020-02-02 00:00:00.000000 reqstool-0.4.3/docs/examples/requirements/requirements_microservice.yml
+-rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 reqstool-0.4.3/docs/examples/requirements/requirements_system.yml
+-rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 reqstool-0.4.3/docs/examples/requirements/software_verification_cases.yml
+-rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 reqstool-0.4.3/docs/modules/ROOT/nav.adoc
+-rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 reqstool-0.4.3/docs/modules/ROOT/pages/background.adoc
+-rw-r--r--   0        0        0    10790 2020-02-02 00:00:00.000000 reqstool-0.4.3/docs/modules/ROOT/pages/data.adoc
+-rw-r--r--   0        0        0     3822 2020-02-02 00:00:00.000000 reqstool-0.4.3/docs/modules/ROOT/pages/file_and_directory_set.adoc
+-rw-r--r--   0        0        0     6723 2020-02-02 00:00:00.000000 reqstool-0.4.3/docs/modules/ROOT/pages/how_it_works.adoc
+-rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 reqstool-0.4.3/docs/modules/ROOT/pages/index.adoc
+-rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 reqstool-0.4.3/docs/modules/ROOT/pages/installation.adoc
+-rw-r--r--   0        0        0     1126 2020-02-02 00:00:00.000000 reqstool-0.4.3/docs/modules/ROOT/pages/overview.adoc
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 reqstool-0.4.3/docs/modules/ROOT/pages/quickstart.adoc
+-rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 reqstool-0.4.3/docs/modules/ROOT/pages/terminology.adoc
+-rw-r--r--   0        0        0     3433 2020-02-02 00:00:00.000000 reqstool-0.4.3/docs/modules/ROOT/pages/usage.adoc
+-rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 reqstool-0.4.3/docs/modules/ROOT/pages/yml/annotations.adoc
+-rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 reqstool-0.4.3/docs/modules/ROOT/pages/yml/manual_verification_results.adoc
+-rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 reqstool-0.4.3/docs/modules/ROOT/pages/yml/reqstool_config.adoc
+-rw-r--r--   0        0        0     2222 2020-02-02 00:00:00.000000 reqstool-0.4.3/docs/modules/ROOT/pages/yml/requirements.adoc
+-rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 reqstool-0.4.3/docs/modules/ROOT/pages/yml/requirements_annotations.adoc
+-rw-r--r--   0        0        0     1028 2020-02-02 00:00:00.000000 reqstool-0.4.3/docs/modules/ROOT/pages/yml/requirements_external.adoc
+-rw-r--r--   0        0        0     2222 2020-02-02 00:00:00.000000 reqstool-0.4.3/docs/modules/ROOT/pages/yml/requirements_microservice.adoc
+-rw-r--r--   0        0        0     1858 2020-02-02 00:00:00.000000 reqstool-0.4.3/docs/modules/ROOT/pages/yml/requirements_system.adoc
+-rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 reqstool-0.4.3/docs/modules/ROOT/pages/yml/software_verification_cases.adoc
+-rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 reqstool-0.4.3/docs/modules/ROOT/pages/yml/svcs_annotations.adoc
+-rw-r--r--   0        0        0     3879 2020-02-02 00:00:00.000000 reqstool-0.4.3/docs/modules/ROOT/partials/C4_Component.puml
+-rw-r--r--   0        0        0    14863 2020-02-02 00:00:00.000000 reqstool-0.4.3/docs/modules/ROOT/partials/C4_Sequence.puml
+-rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 reqstool-0.4.3/docs/modules/examples/partials/requirements/manual_verification_results.yml
+-rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 reqstool-0.4.3/docs/modules/examples/partials/requirements/reqstool_config.yml
+-rw-r--r--   0        0        0      875 2020-02-02 00:00:00.000000 reqstool-0.4.3/docs/modules/examples/partials/requirements/requirements_external.yml
+-rw-r--r--   0        0        0     1727 2020-02-02 00:00:00.000000 reqstool-0.4.3/docs/modules/examples/partials/requirements/requirements_microservice.yml
+-rw-r--r--   0        0        0     1402 2020-02-02 00:00:00.000000 reqstool-0.4.3/docs/modules/examples/partials/requirements/requirements_system.yml
+-rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 reqstool-0.4.3/docs/modules/examples/partials/requirements/software_verification_cases.yml
+-rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 reqstool-0.4.3/docs/reqstool/manual_verification_results.yml
+-rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 reqstool-0.4.3/docs/reqstool/reqstool_config.yml
+-rw-r--r--   0        0        0    10690 2020-02-02 00:00:00.000000 reqstool-0.4.3/docs/reqstool/requirements.yml
+-rw-r--r--   0        0        0     6822 2020-02-02 00:00:00.000000 reqstool-0.4.3/docs/reqstool/software_verification_cases.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 reqstool-0.4.3/src/reqstool/__init__.py
+-rwxr-xr-x   0        0        0    10652 2020-02-02 00:00:00.000000 reqstool-0.4.3/src/reqstool/command.py
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 reqstool-0.4.3/src/reqstool/commands/exit_codes.py
+-rw-r--r--   0        0        0     3353 2020-02-02 00:00:00.000000 reqstool-0.4.3/src/reqstool/commands/generate_json/generate_json.py
+-rw-r--r--   0        0        0    10532 2020-02-02 00:00:00.000000 reqstool-0.4.3/src/reqstool/commands/report/report.py
+-rw-r--r--   0        0        0     2735 2020-02-02 00:00:00.000000 reqstool-0.4.3/src/reqstool/commands/report/criterias/group_by.py
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 reqstool-0.4.3/src/reqstool/commands/report/criterias/sort_by.py
+-rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 reqstool-0.4.3/src/reqstool/commands/report/templates/annotation_impls.j2
+-rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 reqstool-0.4.3/src/reqstool/commands/report/templates/annotation_tests.j2
+-rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 reqstool-0.4.3/src/reqstool/commands/report/templates/mvrs.j2
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 reqstool-0.4.3/src/reqstool/commands/report/templates/report.j2
+-rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 reqstool-0.4.3/src/reqstool/commands/report/templates/req_references.j2
+-rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 reqstool-0.4.3/src/reqstool/commands/report/templates/requirements.j2
+-rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 reqstool-0.4.3/src/reqstool/commands/report/templates/svcs.j2
+-rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 reqstool-0.4.3/src/reqstool/commands/report/templates/total_statistics.j2
+-rw-r--r--   0        0        0     3055 2020-02-02 00:00:00.000000 reqstool-0.4.3/src/reqstool/commands/status/statistics_container.py
+-rw-r--r--   0        0        0    13322 2020-02-02 00:00:00.000000 reqstool-0.4.3/src/reqstool/commands/status/statistics_generator.py
+-rw-r--r--   0        0        0     9220 2020-02-02 00:00:00.000000 reqstool-0.4.3/src/reqstool/commands/status/status.py
+-rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 reqstool-0.4.3/src/reqstool/common/jinja2.py
+-rw-r--r--   0        0        0     9339 2020-02-02 00:00:00.000000 reqstool-0.4.3/src/reqstool/common/utils.py
+-rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 reqstool-0.4.3/src/reqstool/common/validator_error_holder.py
+-rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 reqstool-0.4.3/src/reqstool/common/dataclasses/urn_id.py
+-rw-r--r--   0        0        0    12034 2020-02-02 00:00:00.000000 reqstool-0.4.3/src/reqstool/common/validators/semantic_validator.py
+-rw-r--r--   0        0        0     2259 2020-02-02 00:00:00.000000 reqstool-0.4.3/src/reqstool/common/validators/syntax_validator.py
+-rwxr-xr-x   0        0        0     2575 2020-02-02 00:00:00.000000 reqstool-0.4.3/src/reqstool/expression_languages/generic_el.py
+-rwxr-xr-x   0        0        0      235 2020-02-02 00:00:00.000000 reqstool-0.4.3/src/reqstool/expression_languages/requirements_el.py
+-rwxr-xr-x   0        0        0      203 2020-02-02 00:00:00.000000 reqstool-0.4.3/src/reqstool/expression_languages/svcs_el.py
+-rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 reqstool-0.4.3/src/reqstool/filters/id_filters.py
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 reqstool-0.4.3/src/reqstool/filters/requirements_filters.py
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 reqstool-0.4.3/src/reqstool/filters/svcs_filters.py
+-rw-r--r--   0        0        0     1698 2020-02-02 00:00:00.000000 reqstool-0.4.3/src/reqstool/location_resolver/location_resolver.py
+-rw-r--r--   0        0        0     1272 2020-02-02 00:00:00.000000 reqstool-0.4.3/src/reqstool/locations/git_location.py
+-rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 reqstool-0.4.3/src/reqstool/locations/local_location.py
+-rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 reqstool-0.4.3/src/reqstool/locations/location.py
+-rw-r--r--   0        0        0     1935 2020-02-02 00:00:00.000000 reqstool-0.4.3/src/reqstool/locations/maven_location.py
+-rw-r--r--   0        0        0     1894 2020-02-02 00:00:00.000000 reqstool-0.4.3/src/reqstool/model_generators/annotations_model_generator.py
+-rw-r--r--   0        0        0    29242 2020-02-02 00:00:00.000000 reqstool-0.4.3/src/reqstool/model_generators/combined_indexed_dataset_generator.py
+-rw-r--r--   0        0        0    10755 2020-02-02 00:00:00.000000 reqstool-0.4.3/src/reqstool/model_generators/combined_raw_datasets_generator.py
+-rw-r--r--   0        0        0     1559 2020-02-02 00:00:00.000000 reqstool-0.4.3/src/reqstool/model_generators/mvrs_model_generator.py
+-rw-r--r--   0        0        0    12619 2020-02-02 00:00:00.000000 reqstool-0.4.3/src/reqstool/model_generators/requirements_model_generator.py
+-rw-r--r--   0        0        0     4519 2020-02-02 00:00:00.000000 reqstool-0.4.3/src/reqstool/model_generators/svcs_model_generator.py
+-rw-r--r--   0        0        0     2471 2020-02-02 00:00:00.000000 reqstool-0.4.3/src/reqstool/model_generators/testdata_model_generator.py
+-rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 reqstool-0.4.3/src/reqstool/models/annotations.py
+-rw-r--r--   0        0        0     1341 2020-02-02 00:00:00.000000 reqstool-0.4.3/src/reqstool/models/combined_indexed_dataset.py
+-rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 reqstool-0.4.3/src/reqstool/models/implementations.py
+-rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 reqstool-0.4.3/src/reqstool/models/imports.py
+-rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 reqstool-0.4.3/src/reqstool/models/mvrs.py
+-rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 reqstool-0.4.3/src/reqstool/models/raw_datasets.py
+-rw-r--r--   0        0        0     2222 2020-02-02 00:00:00.000000 reqstool-0.4.3/src/reqstool/models/requirements.py
+-rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 reqstool-0.4.3/src/reqstool/models/svcs.py
+-rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 reqstool-0.4.3/src/reqstool/models/test_data.py
+-rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 reqstool-0.4.3/src/reqstool/reqstool_config/reqstool_config.py
+-rw-r--r--   0        0        0     5508 2020-02-02 00:00:00.000000 reqstool-0.4.3/src/reqstool/requirements_indata/requirements_indata.py
+-rw-r--r--   0        0        0     2027 2020-02-02 00:00:00.000000 reqstool-0.4.3/src/reqstool/requirements_indata/requirements_indata_paths.py
+-rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 reqstool-0.4.3/src/reqstool/requirements_indata/java/java_maven_requirements_indata_paths.py
+-rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 reqstool-0.4.3/src/reqstool/requirements_indata/python/python_requirements_indata_paths.py
+-rw-r--r--   0        0        0     2471 2020-02-02 00:00:00.000000 reqstool-0.4.3/src/reqstool/resources/schemas/v1/annotations.schema.json
+-rw-r--r--   0        0        0    11026 2020-02-02 00:00:00.000000 reqstool-0.4.3/src/reqstool/resources/schemas/v1/common.schema.json
+-rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 reqstool-0.4.3/src/reqstool/resources/schemas/v1/manual_verification_results.schema.json
+-rw-r--r--   0        0        0     1315 2020-02-02 00:00:00.000000 reqstool-0.4.3/src/reqstool/resources/schemas/v1/reqstool_config.schema.json
+-rw-r--r--   0        0        0    10841 2020-02-02 00:00:00.000000 reqstool-0.4.3/src/reqstool/resources/schemas/v1/requirements.schema.json
+-rw-r--r--   0        0        0     2646 2020-02-02 00:00:00.000000 reqstool-0.4.3/src/reqstool/resources/schemas/v1/software_verification_cases.schema.json
+-rw-r--r--   0        0        0     2120 2020-02-02 00:00:00.000000 reqstool-0.4.3/tests/integration/reqstool/model_generators/test_included_models_generator.py
+-rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 reqstool-0.4.3/tests/resources/test_data/data/local/test_basic/baseline/ms-101/annotations.yml
+-rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 reqstool-0.4.3/tests/resources/test_data/data/local/test_basic/baseline/ms-101/manual_verification_results.yml
+-rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 reqstool-0.4.3/tests/resources/test_data/data/local/test_basic/baseline/ms-101/requirements.yml
+-rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 reqstool-0.4.3/tests/resources/test_data/data/local/test_basic/baseline/ms-101/software_verification_cases.yml
+-rw-r--r--   0        0        0     6367 2020-02-02 00:00:00.000000 reqstool-0.4.3/tests/resources/test_data/data/local/test_basic/baseline/ms-101/test_results/failsafe/TEST-com.example.RequirementsExampleTestsIT.xml
+-rw-r--r--   0        0        0     5744 2020-02-02 00:00:00.000000 reqstool-0.4.3/tests/resources/test_data/data/local/test_basic/baseline/ms-101/test_results/surefire/TEST-com.example.RequirementsExampleTests.xml
+-rw-r--r--   0        0        0     2724 2020-02-02 00:00:00.000000 reqstool-0.4.3/tests/resources/test_data/data/local/test_basic/layout_maven/ms-101/pom.xml
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 reqstool-0.4.3/tests/resources/test_data/data/local/test_basic/layout_maven/ms-101/src/resources/docs/requirements/manual_verification_results.yml -> ../../../../../../baseline/ms-101/manual_verification_results.yml
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 reqstool-0.4.3/tests/resources/test_data/data/local/test_basic/layout_maven/ms-101/src/resources/docs/requirements/requirements.yml -> ../../../../../../baseline/ms-101/requirements.yml
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 reqstool-0.4.3/tests/resources/test_data/data/local/test_basic/layout_maven/ms-101/src/resources/docs/requirements/software_verification_cases.yml -> ../../../../../../baseline/ms-101/software_verification_cases.yml
+-rw-r--r--   0        0        0     3264 2020-02-02 00:00:00.000000 reqstool-0.4.3/tests/resources/test_data/data/local/test_basic/with_requirements_config/README.md
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 reqstool-0.4.3/tests/resources/test_data/data/local/test_basic/with_requirements_config/ms-101/manual_verification_results.yml -> ../../baseline/ms-101/manual_verification_results.yml
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 reqstool-0.4.3/tests/resources/test_data/data/local/test_basic/with_requirements_config/ms-101/reqstool_config.yml
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 reqstool-0.4.3/tests/resources/test_data/data/local/test_basic/with_requirements_config/ms-101/requirements.yml -> ../../baseline/ms-101/requirements.yml
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 reqstool-0.4.3/tests/resources/test_data/data/local/test_basic/with_requirements_config/ms-101/software_verification_cases.yml -> ../../baseline/ms-101/software_verification_cases.yml
+-rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 reqstool-0.4.3/tests/resources/test_data/data/local/test_errors/ms-101/annotations.yml
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 reqstool-0.4.3/tests/resources/test_data/data/local/test_errors/ms-101/errors.adoc
+-rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 reqstool-0.4.3/tests/resources/test_data/data/local/test_errors/ms-101/manual_verification_results.yml
+-rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 reqstool-0.4.3/tests/resources/test_data/data/local/test_errors/ms-101/requirements.yml
+-rw-r--r--   0        0        0      892 2020-02-02 00:00:00.000000 reqstool-0.4.3/tests/resources/test_data/data/local/test_errors/ms-101/software_verification_cases.yml
+-rw-r--r--   0        0        0     6367 2020-02-02 00:00:00.000000 reqstool-0.4.3/tests/resources/test_data/data/local/test_errors/ms-101/test_results/failsafe/TEST-com.example.RequirementsExampleTestsIT.xml
+-rw-r--r--   0        0        0     5744 2020-02-02 00:00:00.000000 reqstool-0.4.3/tests/resources/test_data/data/local/test_errors/ms-101/test_results/surefire/TEST-com.example.RequirementsExampleTests.xml
+-rw-r--r--   0        0        0      944 2020-02-02 00:00:00.000000 reqstool-0.4.3/tests/resources/test_data/data/local/test_standard/baseline/visualization.adoc
+-rw-r--r--   0        0        0     2059 2020-02-02 00:00:00.000000 reqstool-0.4.3/tests/resources/test_data/data/local/test_standard/baseline/ms-001/annotations.yml
+-rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 reqstool-0.4.3/tests/resources/test_data/data/local/test_standard/baseline/ms-001/manual_verification_results.yml
+-rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 reqstool-0.4.3/tests/resources/test_data/data/local/test_standard/baseline/ms-001/requirements.yml
+-rw-r--r--   0        0        0     1375 2020-02-02 00:00:00.000000 reqstool-0.4.3/tests/resources/test_data/data/local/test_standard/baseline/ms-001/software_verification_cases.yml
+-rw-r--r--   0        0        0     7126 2020-02-02 00:00:00.000000 reqstool-0.4.3/tests/resources/test_data/data/local/test_standard/baseline/ms-001/test_results/failsafe/TEST-com.reqstool.example.demo.DemoApplicationTestsIT.xml
+-rw-r--r--   0        0        0     8258 2020-02-02 00:00:00.000000 reqstool-0.4.3/tests/resources/test_data/data/local/test_standard/baseline/ms-001/test_results/surefire/TEST-com.reqstool.example.demo.SVCsTest.xml
+-rw-r--r--   0        0        0      817 2020-02-02 00:00:00.000000 reqstool-0.4.3/tests/resources/test_data/data/local/test_standard/baseline/sys-001/requirements.yml
+-rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 reqstool-0.4.3/tests/resources/test_data/data/local/test_standard/baseline/sys-001/software_verification_cases.yml
+-rw-r--r--   0        0        0      838 2020-02-02 00:00:00.000000 reqstool-0.4.3/tests/resources/test_data/data/local/test_standard/baseline/sys-001/ext-001/requirements.yml
+-rw-r--r--   0        0        0     1199 2020-02-02 00:00:00.000000 reqstool-0.4.3/tests/resources/test_data/data/local/test_standard/baseline/sys-001/ext-002/requirements.yml
+-rw-r--r--   0        0        0     2119 2020-02-02 00:00:00.000000 reqstool-0.4.3/tests/resources/test_data/data/local/test_standard/empty_ms/ms-001/annotations.yml
+-rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 reqstool-0.4.3/tests/resources/test_data/data/local/test_standard/empty_ms/ms-001/requirements.yml
+-rw-r--r--   0        0        0     7125 2020-02-02 00:00:00.000000 reqstool-0.4.3/tests/resources/test_data/data/local/test_standard/empty_ms/ms-001/test_results/failsafe/TEST-com.reqstool.example.demo.DemoApplicationTestsIT.xml
+-rw-r--r--   0        0        0     8258 2020-02-02 00:00:00.000000 reqstool-0.4.3/tests/resources/test_data/data/local/test_standard/empty_ms/ms-001/test_results/surefire/TEST-com.reqstool.example.demo.SVCsTest.xml
+-rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 reqstool-0.4.3/tests/resources/test_data/data/local/test_standard/empty_ms/sys-001/manual_verification_results.yml
+-rw-r--r--   0        0        0     1426 2020-02-02 00:00:00.000000 reqstool-0.4.3/tests/resources/test_data/data/local/test_standard/empty_ms/sys-001/requirements.yml
+-rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 reqstool-0.4.3/tests/resources/test_data/data/local/test_standard/empty_ms/sys-001/software_verification_cases.yml
+-rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 reqstool-0.4.3/tests/resources/test_data/data/local/test_standard/empty_ms/sys-001/ext-001/requirements.yml
+-rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 reqstool-0.4.3/tests/resources/test_data/data/local/test_standard/empty_ms/sys-001/ext-002/requirements.yml
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 reqstool-0.4.3/tests/resources/test_data/data/remote/test_standard/test_standard_maven_git/ms-001/annotations.yml -> ../../../../local/test_standard/baseline/ms-001/annotations.yml
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 reqstool-0.4.3/tests/resources/test_data/data/remote/test_standard/test_standard_maven_git/ms-001/manual_verification_results.yml -> ../../../../local/test_standard/baseline/ms-001/manual_verification_results.yml
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 reqstool-0.4.3/tests/resources/test_data/data/remote/test_standard/test_standard_maven_git/ms-001/requirements.yml -> ../../../../local/test_standard/baseline/ms-001/requirements.yml
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 reqstool-0.4.3/tests/resources/test_data/data/remote/test_standard/test_standard_maven_git/ms-001/software_verification_cases.yml -> ../../../../local/test_standard/baseline/ms-001/software_verification_cases.yml
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 reqstool-0.4.3/tests/resources/test_data/data/remote/test_standard/test_standard_maven_git/sys-001/annotations.yml -> ../../../../local/test_standard/baseline/sys-001/annotations.yml
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 reqstool-0.4.3/tests/resources/test_data/data/remote/test_standard/test_standard_maven_git/sys-001/manual_verification_results.yml -> ../../../../local/test_standard/baseline/sys-001/manual_verification_results.yml
+-rw-r--r--   0        0        0     1414 2020-02-02 00:00:00.000000 reqstool-0.4.3/tests/resources/test_data/data/remote/test_standard/test_standard_maven_git/sys-001/requirements.yml
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 reqstool-0.4.3/tests/resources/test_data/data/remote/test_standard/test_standard_maven_git/sys-001/software_verification_cases.yml -> ../../../../local/test_standard/baseline/sys-001/software_verification_cases.yml
+-rw-r--r--   0        0        0     1573 2020-02-02 00:00:00.000000 reqstool-0.4.3/tests/resources/unit/reqstool/model_generators/test_annotations_model_generator/test_annotations_model_generator/annotations.yml
+-rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 reqstool-0.4.3/tests/resources/unit/reqstool/model_generators/test_mvrs_model_generator/test_mvrs_model_generator/manual_verification_results.yml
+-rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 reqstool-0.4.3/tests/resources/unit/reqstool/model_generators/test_requirements_model_generator/test_external_requirements_model_generator/requirements.yml
+-rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 reqstool-0.4.3/tests/resources/unit/reqstool/model_generators/test_requirements_model_generator/test_microservice_requirements_model_generator/requirements.yml
+-rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 reqstool-0.4.3/tests/resources/unit/reqstool/model_generators/test_requirements_model_generator/test_rational_optional_model_generator/requirements.yml
+-rw-r--r--   0        0        0     2047 2020-02-02 00:00:00.000000 reqstool-0.4.3/tests/resources/unit/reqstool/model_generators/test_requirements_model_generator/test_system_requirements_model_generator/requirements.yml
+-rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 reqstool-0.4.3/tests/resources/unit/reqstool/model_generators/test_svcs_model_generator/test_svcs_model_generator/software_verification_cases.yml
+-rw-r--r--   0        0        0     2212 2020-02-02 00:00:00.000000 reqstool-0.4.3/tests/unit/conftest.py
+-rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 reqstool-0.4.3/tests/unit/reqstool/commands/generate_json/test_generate_json.py
+-rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 reqstool-0.4.3/tests/unit/reqstool/commands/report/test_report.py
+-rw-r--r--   0        0        0     1569 2020-02-02 00:00:00.000000 reqstool-0.4.3/tests/unit/reqstool/commands/report/criterias/test_criterias.py
+-rw-r--r--   0        0        0     2693 2020-02-02 00:00:00.000000 reqstool-0.4.3/tests/unit/reqstool/commands/status/test_statistics_container.py
+-rw-r--r--   0        0        0    18426 2020-02-02 00:00:00.000000 reqstool-0.4.3/tests/unit/reqstool/commands/status/test_statistics_generator.py
+-rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 reqstool-0.4.3/tests/unit/reqstool/commands/status/test_status.py
+-rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 reqstool-0.4.3/tests/unit/reqstool/common/test_locations.py
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 reqstool-0.4.3/tests/unit/reqstool/common/test_utils.py
+-rw-r--r--   0        0        0     8217 2020-02-02 00:00:00.000000 reqstool-0.4.3/tests/unit/reqstool/common/validators/test_semantic_validator.py
+-rw-r--r--   0        0        0     5305 2020-02-02 00:00:00.000000 reqstool-0.4.3/tests/unit/reqstool/expression_languages/test_requirements_el.py
+-rw-r--r--   0        0        0     4054 2020-02-02 00:00:00.000000 reqstool-0.4.3/tests/unit/reqstool/expression_languages/test_svcs_el.py
+-rw-r--r--   0        0        0     1321 2020-02-02 00:00:00.000000 reqstool-0.4.3/tests/unit/reqstool/filters/test_requirements_filters.py
+-rw-r--r--   0        0        0     1362 2020-02-02 00:00:00.000000 reqstool-0.4.3/tests/unit/reqstool/filters/test_software_verification_cases_filters.py
+-rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 reqstool-0.4.3/tests/unit/reqstool/locations/test_git_location.py
+-rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 reqstool-0.4.3/tests/unit/reqstool/locations/test_local_location.py
+-rw-r--r--   0        0        0     2192 2020-02-02 00:00:00.000000 reqstool-0.4.3/tests/unit/reqstool/model_generators/test_annotations_model_generator.py
+-rw-r--r--   0        0        0     3369 2020-02-02 00:00:00.000000 reqstool-0.4.3/tests/unit/reqstool/model_generators/test_combined_indexed_dataset_generator.py
+-rw-r--r--   0        0        0     3904 2020-02-02 00:00:00.000000 reqstool-0.4.3/tests/unit/reqstool/model_generators/test_combined_raw_datasets_generator.py
+-rw-r--r--   0        0        0     1402 2020-02-02 00:00:00.000000 reqstool-0.4.3/tests/unit/reqstool/model_generators/test_mvrs_model_generator.py
+-rw-r--r--   0        0        0    11130 2020-02-02 00:00:00.000000 reqstool-0.4.3/tests/unit/reqstool/model_generators/test_requirements_model_generator.py
+-rw-r--r--   0        0        0     2258 2020-02-02 00:00:00.000000 reqstool-0.4.3/tests/unit/reqstool/model_generators/test_svcs_model_generator.py
+-rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 reqstool-0.4.3/tests/unit/reqstool/model_generators/test_testdata_model_generator.py
+-rw-r--r--   0        0        0      960 2020-02-02 00:00:00.000000 reqstool-0.4.3/tests/unit/reqstool/models/test_annotations.py
+-rw-r--r--   0        0        0     2435 2020-02-02 00:00:00.000000 reqstool-0.4.3/tests/unit/reqstool/models/test_implementations.py
+-rw-r--r--   0        0        0     2246 2020-02-02 00:00:00.000000 reqstool-0.4.3/tests/unit/reqstool/models/test_imports.py
+-rw-r--r--   0        0        0     1044 2020-02-02 00:00:00.000000 reqstool-0.4.3/tests/unit/reqstool/models/test_mvrs.py
+-rw-r--r--   0        0        0     2368 2020-02-02 00:00:00.000000 reqstool-0.4.3/tests/unit/reqstool/models/test_requirements.py
+-rw-r--r--   0        0        0     2922 2020-02-02 00:00:00.000000 reqstool-0.4.3/tests/unit/reqstool/models/test_svcs.py
+-rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 reqstool-0.4.3/tests/unit/reqstool/reqstool_config/test_reqstool_config.py
+-rw-r--r--   0        0        0     1934 2020-02-02 00:00:00.000000 reqstool-0.4.3/tests/unit/reqstool/requirements_indata/test_requirements_indata_paths.py
+-rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 reqstool-0.4.3/tests/unit/reqstool/resources/schemas/v1/test_json_schemas.py
+-rw-r--r--   0        0        0     4213 2020-02-02 00:00:00.000000 reqstool-0.4.3/.gitignore
+-rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 reqstool-0.4.3/LICENSE
+-rw-r--r--   0        0        0     3264 2020-02-02 00:00:00.000000 reqstool-0.4.3/README.md
+-rw-r--r--   0        0        0     1965 2020-02-02 00:00:00.000000 reqstool-0.4.3/pyproject.toml
+-rw-r--r--   0        0        0     4208 2020-02-02 00:00:00.000000 reqstool-0.4.3/PKG-INFO
```

### Comparing `reqstool-0.4.2/.github/dependabot.yml` & `reqstool-0.4.3/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.2/.github/workflows/build.yml` & `reqstool-0.4.3/.github/workflows/build.yml`

 * *Files 19% similar despite different names*

```diff
@@ -28,13 +28,18 @@
           python-version: "3.10"
       - name: Install dependencies
         run: pip install hatch
       - name: Run unit and integrations tests
         run: hatch run test:pytest --cov=reqstool-client --cov-report=xml --cov-report=html -o junit_family=xunit2 --junitxml=build/junit.xml
       - name: Build project
         run: hatch build
+      - name: Test reqstool-client from build by installing and running
+        run: |
+          WHL_FILE=$(ls dist/*.whl)
+          pip install $WHL_FILE
+          reqstool status local -p docs/reqstool
       # Upload artifacts for later use
       - name: Upload Artifacts
         uses: actions/upload-artifact@v4
         with:
           name: dist
           path: dist/
```

### Comparing `reqstool-0.4.2/.github/workflows/lint.yml` & `reqstool-0.4.3/.github/workflows/lint.yml`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.2/.github/workflows/publish_gh_pages.yml` & `reqstool-0.4.3/.github/workflows/publish_gh_pages.yml`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     environment:
       name: github-pages
       url: ${{ steps.deployment.outputs.page_url }}
     steps:
       - name: Checkout repository
         uses: actions/checkout@v4
       - name: Configure Pages
-        uses: actions/configure-pages@v4
+        uses: actions/configure-pages@v5
       - name: Install Node.js
         uses: actions/setup-node@v4
         with:
           node-version: "18"
       - name: Install Antora
         run: npm i antora
       - name: Install Asciidoctor Kroki extension
```

### Comparing `reqstool-0.4.2/.github/workflows/publish_pypi_prod.yml` & `reqstool-0.4.3/.github/workflows/publish_pypi_prod.yml`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.2/.github/workflows/publish_pypi_test.yml` & `reqstool-0.4.3/.github/workflows/publish_pypi_test.yml`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.2/docs/antora-playbook.yml` & `reqstool-0.4.3/docs/antora-playbook.yml`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.2/docs/examples/requirements/requirements_external.yml` & `reqstool-0.4.3/docs/examples/requirements/requirements_external.yml`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.2/docs/examples/requirements/requirements_microservice.yml` & `reqstool-0.4.3/docs/examples/requirements/requirements_microservice.yml`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.2/docs/examples/requirements/requirements_system.yml` & `reqstool-0.4.3/docs/examples/requirements/requirements_system.yml`

 * *Files 10% similar despite different names*

```diff
@@ -21,21 +21,21 @@
       version: 1.0.0
   local:
     - path: ../..
 
 filters:
   ext-001:
     requirement_ids:
-      imports: [REQ_001]
+      includes: [REQ_001]
   ext-002:
     requirement_ids:
-      imports: [REQ_001]
+      includes: [REQ_001]
   ext-003:
     requirement_ids:
-      imports: [REQ_001]
+      includes: [REQ_001]
 
 implementations: # only used with type = system
   git:
     - env_token: e.g. GITLAB_TOKEN or empty
       branch: main
       url: url
       path: ../..
@@ -53,12 +53,10 @@
   - id: id # alphanumerical
     title: title # text
     significance: shall # was level # shall, should, may # https://www.rfc-editor.org/rfc/rfc2119
     description: description # text
     rationale: test # text
     categories: [functional-suitability]
     references: # links, source
-      - requirement_ids: [REQ123] # links to another requirement in this document
-      - sources: [FSB] # FSB, SAF, SWAL
-      - requirement_ids: [REQ123] # links to another requirement in this document
-        sources: [FSB] # FSB, SAF, SWAL
+      requirement_ids:
+        - REQ123 # links to another requirement in this document
     revision: 0.0.0 # requirement added from revision number, e.g. 1.0.2
```

### Comparing `reqstool-0.4.2/docs/examples/requirements/software_verification_cases.yml` & `reqstool-0.4.3/docs/modules/examples/partials/requirements/software_verification_cases.yml`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # yaml-language-server: $schema=https://raw.githubusercontent.com/Luftfartsverket/reqstool-client/main/src/reqstool/resources/schemas/v1/software_verification_cases.schema.json
 
 filters:
   sys001:
-    svcs_ids:
-      imports: ["SVC_123", "SVC_124"]
+    svc_ids:
+      includes: ["SVC_123", "SVC_124"]
     custom:
-      imports: 'ids == "SVC_123", "SVC_124"'
+      includes: 'ids == "SVC_123", "SVC_124"'
   sys002:
-    svcs_ids:
+    svc_ids:
       excludes: ["SVC_123", "SVC_124"]
     custom:
       exclude: 'ids == "SVC_123", "SVC_124"'
 
 cases:
   - id: # alphanumerical
     requirement_ids: # array of alphanumerical
```

### Comparing `reqstool-0.4.2/docs/modules/ROOT/pages/background.adoc` & `reqstool-0.4.3/docs/modules/ROOT/pages/background.adoc`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.2/docs/modules/ROOT/pages/data.adoc` & `reqstool-0.4.3/docs/modules/ROOT/pages/data.adoc`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.2/docs/modules/ROOT/pages/file_and_directory_set.adoc` & `reqstool-0.4.3/docs/modules/ROOT/pages/file_and_directory_set.adoc`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.2/docs/modules/ROOT/pages/how_it_works.adoc` & `reqstool-0.4.3/docs/modules/ROOT/pages/how_it_works.adoc`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.2/docs/modules/ROOT/pages/index.adoc` & `reqstool-0.4.3/docs/modules/ROOT/pages/index.adoc`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.2/docs/modules/ROOT/pages/overview.adoc` & `reqstool-0.4.3/docs/modules/ROOT/pages/overview.adoc`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.2/docs/modules/ROOT/pages/terminology.adoc` & `reqstool-0.4.3/docs/modules/ROOT/pages/terminology.adoc`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.2/docs/modules/ROOT/pages/usage.adoc` & `reqstool-0.4.3/docs/modules/ROOT/pages/usage.adoc`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.2/docs/modules/ROOT/pages/yml/annotations.adoc` & `reqstool-0.4.3/docs/modules/ROOT/pages/yml/annotations.adoc`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.2/docs/modules/ROOT/pages/yml/requirements.adoc` & `reqstool-0.4.3/docs/modules/ROOT/pages/yml/requirements.adoc`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.2/docs/modules/ROOT/pages/yml/requirements_annotations.adoc` & `reqstool-0.4.3/docs/modules/ROOT/pages/yml/requirements_annotations.adoc`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.2/docs/modules/ROOT/pages/yml/requirements_external.adoc` & `reqstool-0.4.3/docs/modules/ROOT/pages/yml/requirements_external.adoc`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.2/docs/modules/ROOT/pages/yml/requirements_microservice.adoc` & `reqstool-0.4.3/docs/modules/ROOT/pages/yml/requirements_microservice.adoc`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.2/docs/modules/ROOT/pages/yml/requirements_system.adoc` & `reqstool-0.4.3/docs/modules/ROOT/pages/yml/requirements_system.adoc`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.2/docs/modules/ROOT/pages/yml/software_verification_cases.adoc` & `reqstool-0.4.3/docs/modules/ROOT/pages/yml/software_verification_cases.adoc`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.2/docs/modules/ROOT/pages/yml/svcs_annotations.adoc` & `reqstool-0.4.3/docs/modules/ROOT/pages/yml/svcs_annotations.adoc`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.2/docs/modules/ROOT/partials/C4_Component.puml` & `reqstool-0.4.3/docs/modules/ROOT/partials/C4_Component.puml`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.2/docs/modules/ROOT/partials/C4_Sequence.puml` & `reqstool-0.4.3/docs/modules/ROOT/partials/C4_Sequence.puml`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.2/docs/modules/examples/partials/requirements/requirements_external.yml` & `reqstool-0.4.3/docs/modules/examples/partials/requirements/requirements_external.yml`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.2/docs/modules/examples/partials/requirements/requirements_microservice.yml` & `reqstool-0.4.3/docs/modules/examples/partials/requirements/requirements_microservice.yml`

 * *Files 4% similar despite different names*

```diff
@@ -30,20 +30,20 @@
     requirement_ids:
       excludes: ["REQ_sys002_002"] # list of requirement ids
   sys003:
     custom:
       includes: ids == "REQ_sys003_001"
   sys004:
     custom:
-      exclude: ids == "REQ_sys004_001", "REQ_sys004_002"" # list of requirement ids
+      excludes: ids == "REQ_sys004_001", "REQ_sys004_002"" # list of requirement ids
   sys005:
     requirement_ids:
       excludes: ["REQ_sys005_002"] # list of requirement ids
     custom:
-      exclude: ids == "REQ_sys005_003" # list of requirement ids
+      excludes: ids == "REQ_sys005_003" # list of requirement ids
   sys006:
     requirement_ids:
       includes: ["REQ_sys006_001"]
     custom:
       includes: ids == "REQ_sys006_003" # list of requirement ids
 
 requirements:
```

### Comparing `reqstool-0.4.2/docs/modules/examples/partials/requirements/requirements_system.yml` & `reqstool-0.4.3/docs/modules/examples/partials/requirements/requirements_system.yml`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.2/docs/modules/examples/partials/requirements/software_verification_cases.yml` & `reqstool-0.4.3/docs/examples/requirements/software_verification_cases.yml`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
       includes: ["SVC_123", "SVC_124"]
     custom:
       includes: 'ids == "SVC_123", "SVC_124"'
   sys002:
     svc_ids:
       excludes: ["SVC_123", "SVC_124"]
     custom:
-      exclude: 'ids == "SVC_123", "SVC_124"'
+      excludes: 'ids == "SVC_123", "SVC_124"'
 
 cases:
   - id: # alphanumerical
     requirement_ids: # array of alphanumerical
     title: # text
     description: # text
     verification: # automated (test), manual (test), review, platform, other
```

### Comparing `reqstool-0.4.2/docs/reqstool/manual_verification_results.yml` & `reqstool-0.4.3/docs/reqstool/manual_verification_results.yml`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.2/docs/reqstool/requirements.yml` & `reqstool-0.4.3/docs/reqstool/requirements.yml`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.2/docs/reqstool/software_verification_cases.yml` & `reqstool-0.4.3/docs/reqstool/software_verification_cases.yml`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.2/src/reqstool/command.py` & `reqstool-0.4.3/src/reqstool/command.py`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.2/src/reqstool/commands/generate_json/generate_json.py` & `reqstool-0.4.3/src/reqstool/commands/generate_json/generate_json.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,40 +1,41 @@
 # Copyright © LFV
 
 
 import re
 from enum import Enum
 
 import jsonpickle
+from packaging.version import Version
 from reqstool_python_decorators.decorators.decorators import Requirements
 
 from reqstool.common.dataclasses.urn_id import UrnId
 from reqstool.common.validator_error_holder import ValidationErrorHolder
 from reqstool.common.validators.semantic_validator import SemanticValidator
 from reqstool.locations.location import LOCATIONTYPES, LocationInterface
 from reqstool.model_generators.combined_indexed_dataset_generator import CombinedIndexedDatasetGenerator
 from reqstool.model_generators.combined_raw_datasets_generator import CombinedRawDatasetsGenerator
 from reqstool.models.raw_datasets import CombinedRawDataset
-from reqstool.models.requirements import SIGNIFANCETYPES, TYPES, VARIANTS
+from reqstool.models.requirements import CATEGORIES, SIGNIFANCETYPES, TYPES, VARIANTS
 from reqstool.models.svcs import VERIFICATIONTYPES
+from reqstool.models.test_data import TEST_RUN_STATUS
 
 
 class UrnIdHandler(jsonpickle.handlers.BaseHandler):
-    def flatten(self, obj, data):
+    def flatten(self, obj, data) -> str:
         return UrnId.assure_urn_id(obj.urn, obj.id)
 
-    def restore(self, obj):
-        urn_id_str = obj
-        return UrnId.instance(urn_id_str)
 
+class RevisionHandler(jsonpickle.handlers.BaseHandler):
+    def flatten(self, obj, data):
+        version: Version = obj
+        return {"major": version.major, "minor": version.minor, "patch": version.micro}
 
-class JsonEnumHandler(jsonpickle.handlers.BaseHandler):
-    def restore(self, obj):
-        pass
 
+class JsonEnumHandler(jsonpickle.handlers.BaseHandler):
     def flatten(self, obj: Enum, data):
         return obj.value
 
 
 @Requirements("REQ_030")
 class GenerateJsonCommand:
     def __init__(self, location: LocationInterface, filter_data: bool):
@@ -57,19 +58,22 @@
         cids = CombinedIndexedDatasetGenerator(
             _crd=combined_raw_datasets, _filtered=self.__filter_data
         ).combined_indexed_dataset
 
         # Register the custom handler for enumerations
 
         jsonpickle.handlers.registry.register(UrnId, UrnIdHandler)
-        jsonpickle.handlers.registry.register(SIGNIFANCETYPES, JsonEnumHandler)
-        jsonpickle.handlers.registry.register(VERIFICATIONTYPES, JsonEnumHandler)
-        jsonpickle.handlers.registry.register(VARIANTS, JsonEnumHandler)
+        jsonpickle.handlers.registry.register(Version, RevisionHandler)
+        jsonpickle.handlers.registry.register(CATEGORIES, JsonEnumHandler)
         jsonpickle.handlers.registry.register(LOCATIONTYPES, JsonEnumHandler)
+        jsonpickle.handlers.registry.register(SIGNIFANCETYPES, JsonEnumHandler)
         jsonpickle.handlers.registry.register(TYPES, JsonEnumHandler)
+        jsonpickle.handlers.registry.register(VARIANTS, JsonEnumHandler)
+        jsonpickle.handlers.registry.register(VERIFICATIONTYPES, JsonEnumHandler)
+        jsonpickle.handlers.registry.register(TEST_RUN_STATUS, JsonEnumHandler)
 
         json_data = jsonpickle.encode(cids, make_refs=False, keys=True, unpicklable=False)
 
         # Regular expression pattern to match the given format
         pattern = r'json://\\"(.*?)\\"'
 
         # Replacement using regex
```

### Comparing `reqstool-0.4.2/src/reqstool/commands/report/report.py` & `reqstool-0.4.3/src/reqstool/commands/report/report.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 from reqstool.locations.location import LocationInterface
 from reqstool.model_generators.combined_indexed_dataset_generator import CombinedIndexedDatasetGenerator
 from reqstool.model_generators.combined_raw_datasets_generator import CombinedRawDatasetsGenerator
 from reqstool.models.annotations import AnnotationData
 from reqstool.models.combined_indexed_dataset import CombinedIndexedDataset
 from reqstool.models.mvrs import MVRData
 from reqstool.models.svcs import SVCData
-from reqstool.models.test_data import TestRunStatus
+from reqstool.models.test_data import TEST_RUN_STATUS
 
 
 class Jinja2Templates(Enum):
     REQUIREMENTS = "requirements", "requirements.j2"
     SVCS = "svcs", "svcs.j2"
     ANNOTATION_IMPLS = "annotation_impls", "annotation_impls.j2"
     ANNOTATION_TESTS = "annotation_tests", "annotation_tests.j2"
@@ -221,23 +221,23 @@
                             "fqn": test.fully_qualified_name,
                             "test_result": results_as_string,
                         }
                         automated_test_results.append(annot_test)
 
         return automated_test_results
 
-    def __get_annotated_test_results(self, cid: CombinedIndexedDataset, urn_id: UrnId) -> List[TestRunStatus]:
-        test_results: List[TestRunStatus] = []
+    def __get_annotated_test_results(self, cid: CombinedIndexedDataset, urn_id: UrnId) -> List[TEST_RUN_STATUS]:
+        test_results: List[TEST_RUN_STATUS] = []
         # do lookup for each test from previous method, and if result is missing, add a Missing status
         if urn_id in cid.automated_test_result:
             tests = cid.automated_test_result[urn_id]
             for test in tests:
                 test_results.append(test)
         else:
-            test_results.append(TestRunStatus.MISSING)
+            test_results.append(TEST_RUN_STATUS.MISSING)
 
         return test_results
 
     def _get_annotation_impls(self, cid: CombinedIndexedDataset, urn_id: UrnId):
         impls_list = []
         impls_for_urn: List[AnnotationData] = cid.annotations_impls[urn_id] if urn_id in cid.annotations_impls else []
         if impls_for_urn:
```

### Comparing `reqstool-0.4.2/src/reqstool/commands/report/criterias/group_by.py` & `reqstool-0.4.3/src/reqstool/commands/report/criterias/group_by.py`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.2/src/reqstool/commands/report/templates/total_statistics.j2` & `reqstool-0.4.3/src/reqstool/commands/report/templates/total_statistics.j2`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.2/src/reqstool/commands/status/statistics_container.py` & `reqstool-0.4.3/src/reqstool/commands/status/statistics_container.py`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.2/src/reqstool/commands/status/statistics_generator.py` & `reqstool-0.4.3/src/reqstool/commands/status/statistics_generator.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from reqstool.common.validators.semantic_validator import SemanticValidator
 from reqstool.locations.location import LocationInterface
 from reqstool.model_generators.combined_indexed_dataset_generator import CombinedIndexedDatasetGenerator
 from reqstool.model_generators.combined_raw_datasets_generator import CombinedRawDatasetsGenerator
 from reqstool.models.combined_indexed_dataset import CombinedIndexedDataset
 from reqstool.models.mvrs import MVRData
 from reqstool.models.svcs import VERIFICATIONTYPES, SVCData
-from reqstool.models.test_data import TestData, TestRunStatus
+from reqstool.models.test_data import TEST_RUN_STATUS, TestData
 
 EXPECTS_MVRS = [
     VERIFICATIONTYPES.MANUAL_TEST,
     VERIFICATIONTYPES.REVIEW,
     VERIFICATIONTYPES.PLATFORM,
     VERIFICATIONTYPES.OTHER,
 ]
@@ -128,21 +128,21 @@
             return TestStatisticsItem(nr_of_missing_automated_tests=no_of_missing_automated_tests)
 
         stats_item = TestStatisticsItem(nr_of_total_tests=len(tests))
         # we need to do a check if the current automated test is already counted as passed or failed,
         # as each test could relate to several svc's
         for test in tests:
             match (test.status):
-                case TestRunStatus.PASSED:
+                case TEST_RUN_STATUS.PASSED:
                     stats_item.nr_of_passed_tests += 1
-                case TestRunStatus.FAILED:
+                case TEST_RUN_STATUS.FAILED:
                     stats_item.nr_of_failed_tests += 1
-                case TestRunStatus.SKIPPED:
+                case TEST_RUN_STATUS.SKIPPED:
                     stats_item.nr_of_skipped_tests += 1
-                case TestRunStatus.MISSING:
+                case TEST_RUN_STATUS.MISSING:
                     stats_item.nr_of_missing_automated_tests += 1
 
         return stats_item
 
     # Returns a string if all mvrs passes or fails
     def _get_mvr_stats(self, mvrs: List[MVRData], svcs: List[SVCData]) -> TestStatisticsItem:
         # svc specifies mvr, but no mvr exists
@@ -177,31 +177,31 @@
             if annotation_id == urn_id:
                 nr_of_implementations += 1
         return nr_of_implementations
 
     def _get_annotated_automated_test_results_for_req(
         self,
         svcs_urn_ids: List[UrnId],
-    ) -> List[TestRunStatus]:
+    ) -> List[TEST_RUN_STATUS]:
         automated_test_results: List[TestData] = []
         for urn_id in svcs_urn_ids:
             if urn_id in self.cid.annotations_tests:
                 annotations = self.cid.annotations_tests[urn_id]
                 for tests in annotations:
                     for test in tests:
                         test_urn_id = UrnId(urn=urn_id.urn, id=test.fully_qualified_name)
                         results = self.__get_annotated_test_results(urn_id=test_urn_id)
                         automated_test_results.extend(results)
 
         return automated_test_results
 
     def _get_automated_test_results_for_req(
         self, automated_test_fqn: List[str], automated_test_result: Dict[UrnId, List[TestData]]
-    ) -> List[TestRunStatus]:
-        test_results: List[TestRunStatus] = []
+    ) -> List[TEST_RUN_STATUS]:
+        test_results: List[TEST_RUN_STATUS] = []
         for fqn in automated_test_fqn:
             for test_id, test_result in automated_test_result:
                 if test_id.id == fqn:
                     for test in test_result:
                         test_results.append(test)
         return test_results
 
@@ -247,51 +247,51 @@
     def __count_mvr_status(self, mvrs: List[MVRData], stats_container: StatisticsContainer):
         for mvr in mvrs:
             if mvr.passed:
                 stats_container._total_statistics.nr_of_passed_tests += 1
             else:
                 stats_container._total_statistics.nr_of_failed_tests += 1
 
-    def __get_results_from_annotated_tests(self) -> List[TestRunStatus]:
-        test_results: List[TestRunStatus] = []
+    def __get_results_from_annotated_tests(self) -> List[TEST_RUN_STATUS]:
+        test_results: List[TEST_RUN_STATUS] = []
         parsed_test_annotation_urns: List[UrnId] = []
         for urn_id, annotation_data in self.cid.annotations_tests.items():
             for annotation_test in annotation_data:
                 for test in annotation_test:
                     urn_id = UrnId(urn=urn_id.urn, id=test.fully_qualified_name)
                     # we should save this urn_id in a list, and only do the result lookup
                     # below if the urn_id is not in list.
                     # This is to avoid duplicate counting of the total test results
                     if urn_id not in parsed_test_annotation_urns:
                         parsed_test_annotation_urns.append(urn_id)
                         results = self.__get_annotated_test_results(urn_id=urn_id)
                         test_results.extend(results)
         return test_results
 
-    def __get_annotated_test_results(self, urn_id: UrnId) -> List[TestRunStatus]:
-        test_results: List[TestRunStatus] = []
+    def __get_annotated_test_results(self, urn_id: UrnId) -> List[TEST_RUN_STATUS]:
+        test_results: List[TEST_RUN_STATUS] = []
         # do lookup for each test from previous method, and if result is missing, add a Missing status
         if urn_id in self.cid.automated_test_result:
             tests = self.cid.automated_test_result[urn_id]
             for test in tests:
                 # We shouldn't add the same test result several times.
                 if test not in test_results:
                     test_results.append(test)
         else:
-            test_results.append(TestRunStatus.MISSING)
+            test_results.append(TEST_RUN_STATUS.MISSING)
 
         return test_results
 
     def __calculate_total_automated_test_statistics(
-        self, test_results: List[TestRunStatus], stats_container: StatisticsContainer
+        self, test_results: List[TEST_RUN_STATUS], stats_container: StatisticsContainer
     ):
         for test in test_results:
             match test.status:
-                case TestRunStatus.PASSED:
+                case TEST_RUN_STATUS.PASSED:
                     stats_container._total_statistics.nr_of_passed_tests += 1
-                case TestRunStatus.FAILED:
+                case TEST_RUN_STATUS.FAILED:
                     stats_container._total_statistics.nr_of_failed_tests += 1
-                case TestRunStatus.SKIPPED:
+                case TEST_RUN_STATUS.SKIPPED:
                     stats_container._total_statistics.nr_of_skipped_tests += 1
-                case TestRunStatus.MISSING:
+                case TEST_RUN_STATUS.MISSING:
                     stats_container._total_statistics.nr_of_missing_automated_tests += 1
                     stats_container._total_statistics.nr_of_total_tests -= 1
```

### Comparing `reqstool-0.4.2/src/reqstool/commands/status/status.py` & `reqstool-0.4.3/src/reqstool/commands/status/status.py`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.2/src/reqstool/common/jinja2.py` & `reqstool-0.4.3/src/reqstool/common/jinja2.py`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.2/src/reqstool/common/utils.py` & `reqstool-0.4.3/src/reqstool/common/utils.py`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.2/src/reqstool/common/validator_error_holder.py` & `reqstool-0.4.3/src/reqstool/common/validator_error_holder.py`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.2/src/reqstool/common/dataclasses/urn_id.py` & `reqstool-0.4.3/src/reqstool/common/dataclasses/urn_id.py`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.2/src/reqstool/common/validators/semantic_validator.py` & `reqstool-0.4.3/src/reqstool/common/validators/semantic_validator.py`

 * *Files 1% similar despite different names*

```diff
@@ -204,52 +204,52 @@
                     if not self._svc_id_exists(svc_id=svc_id, combined_raw_dataset=combined_raw_dataset):
                         errors.append(
                             ValidationError(msg=f"MVR refers to non-existing svc id: {self.prettify_urn_id(svc_id)}")
                         )
 
         return errors
 
-    def _validate_svc_imports_filter_has_exclude_xor_imports(self, svc_data: SVCsData) -> List[ValidationError]:
+    def _validate_svc_imports_filter_has_excludes_xor_includes(self, svc_data: SVCsData) -> List[ValidationError]:
         if "filters" in svc_data:
             for urn in svc_data["filters"].keys():
                 urn_filter = svc_data["filters"][urn]
-                if "imports" in urn_filter["svc_ids"] and "excludes" in urn_filter["svc_ids"]:
+                if "includes" in urn_filter["svc_ids"] and "excludes" in urn_filter["svc_ids"]:
                     self._validation_error_holder.add_error(
                         ValidationError(
                             msg=f"""Both imports and exclude filters applied to svc! (urn: {urn})
                             Exclude filter will be used as default
                             """
                         )
                     )
                 if "custom" in urn_filter:
-                    if "imports" in urn_filter["custom"] and "excludes" in urn_filter["custom"]:
+                    if "includes" in urn_filter["custom"] and "excludes" in urn_filter["custom"]:
                         self._validation_error_holder.add_error(
                             ValidationError(
                                 msg=f"""Both custom imports and exclude filters applied to svc! (urn: {urn})
                                 Exclude filter will be used as default
                                 """
                             )
                         )
 
         return self._validation_error_holder.get_no_of_errors() > 0
 
-    def _validate_req_imports_filter_has_exclude_xor_imports(self, req_data: ImportDataInterface) -> bool:
+    def _validate_req_imports_filter_has_excludes_xor_includes(self, req_data: ImportDataInterface) -> bool:
         if "filters" in req_data:
             for urn in req_data["filters"].keys():
                 urn_filter = req_data["filters"][urn]
-                if "imports" in urn_filter["requirement_ids"] and "excludes" in urn_filter["requirement_ids"]:
+                if "includes" in urn_filter["requirement_ids"] and "excludes" in urn_filter["requirement_ids"]:
                     self._validation_error_holder.add_error(
                         ValidationError(
                             msg=f"""Both imports and exclude filters applied to req! (urn: {urn})
                             Exclude filter will be used as default
                             """
                         )
                     )
                 if "custom" in urn_filter:
-                    if "imports" in urn_filter["custom"] and "excludes" in urn_filter["custom"]:
+                    if "includes" in urn_filter["custom"] and "excludes" in urn_filter["custom"]:
                         self._validation_error_holder.add_error(
                             ValidationError(
                                 msg=f"""Both custom imports and exclude filters applied to req! (urn: {urn})
                                 Exclude filter will be used as default
                                 """
                             )
                         )
```

### Comparing `reqstool-0.4.2/src/reqstool/common/validators/syntax_validator.py` & `reqstool-0.4.3/src/reqstool/common/validators/syntax_validator.py`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.2/src/reqstool/expression_languages/generic_el.py` & `reqstool-0.4.3/src/reqstool/expression_languages/generic_el.py`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.2/src/reqstool/filters/id_filters.py` & `reqstool-0.4.3/src/reqstool/filters/id_filters.py`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.2/src/reqstool/location_resolver/location_resolver.py` & `reqstool-0.4.3/src/reqstool/location_resolver/location_resolver.py`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.2/src/reqstool/locations/git_location.py` & `reqstool-0.4.3/src/reqstool/locations/git_location.py`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.2/src/reqstool/locations/local_location.py` & `reqstool-0.4.3/src/reqstool/locations/local_location.py`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.2/src/reqstool/locations/maven_location.py` & `reqstool-0.4.3/src/reqstool/locations/maven_location.py`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.2/src/reqstool/model_generators/annotations_model_generator.py` & `reqstool-0.4.3/src/reqstool/model_generators/annotations_model_generator.py`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.2/src/reqstool/model_generators/combined_indexed_dataset_generator.py` & `reqstool-0.4.3/src/reqstool/model_generators/combined_indexed_dataset_generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from reqstool.filters.svcs_filters import SVCFilter
 from reqstool.models.annotations import AnnotationData
 from reqstool.models.combined_indexed_dataset import CombinedIndexedDataset
 from reqstool.models.mvrs import MVRData
 from reqstool.models.raw_datasets import CombinedRawDataset
 from reqstool.models.requirements import VARIANTS, RequirementData, RequirementsData
 from reqstool.models.svcs import SVCData, SVCsData
-from reqstool.models.test_data import TestData, TestRunStatus
+from reqstool.models.test_data import TEST_RUN_STATUS, TestData
 
 
 @dataclass(kw_only=True)
 class CombinedIndexedDatasetGenerator:
     combined_indexed_dataset: CombinedIndexedDataset = field(init=False, default=None)
 
     _crd: CombinedRawDataset
@@ -252,46 +252,47 @@
                             and automated_test_result_urn_id in self._crd.raw_datasets[urn].automated_tests.tests
                         ):
                             test_data = self._crd.raw_datasets[urn].automated_tests.tests[automated_test_result_urn_id]
 
                         # since there is an annotation we are missing automated test result
                         else:
                             test_data = TestData(
-                                fully_qualified_name=annotation_data.fully_qualified_name, status=TestRunStatus.MISSING
+                                fully_qualified_name=annotation_data.fully_qualified_name,
+                                status=TEST_RUN_STATUS.MISSING,
                             )
 
                         append_data_item_to_dict_list_entry(
                             dictionary=self._automated_test_result, key=svc_urn_id, data=test_data
                         )
 
     def __process_class_annotated_test_results(self, urn: str, fqn: str):
         # get all test results that includes the class fqn
-        get_all_test_res: [TestRunStatus] = [
+        get_all_test_res: [TEST_RUN_STATUS] = [
             self._crd.raw_datasets[urn].automated_tests.tests[urn_id].status
             for urn_id in self._crd.raw_datasets[urn].automated_tests.tests
             if fqn in urn_id.id
         ]
 
         test_data = None
         # if no entries in list, then the test result(s) are missing.
         if not get_all_test_res:
             test_data = TestData(
                 fully_qualified_name=fqn,
-                status=TestRunStatus.MISSING,
+                status=TEST_RUN_STATUS.MISSING,
             )
         # if any test in list is failed, then the test should be marked as failed
-        elif all(test_res == TestRunStatus.PASSED for test_res in get_all_test_res):
+        elif all(test_res == TEST_RUN_STATUS.PASSED for test_res in get_all_test_res):
             test_data = TestData(
                 fully_qualified_name=fqn,
-                status=TestRunStatus.PASSED,
+                status=TEST_RUN_STATUS.PASSED,
             )
         else:
             test_data = TestData(
                 fully_qualified_name=fqn,
-                status=TestRunStatus.FAILED,
+                status=TEST_RUN_STATUS.FAILED,
             )
 
         return test_data
 
     def __process_filters(self):
         self.__process_req_filters()
         self.__process_svc_filters()
```

### Comparing `reqstool-0.4.2/src/reqstool/model_generators/combined_raw_datasets_generator.py` & `reqstool-0.4.3/src/reqstool/model_generators/combined_raw_datasets_generator.py`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.2/src/reqstool/model_generators/mvrs_model_generator.py` & `reqstool-0.4.3/src/reqstool/model_generators/mvrs_model_generator.py`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.2/src/reqstool/model_generators/requirements_model_generator.py` & `reqstool-0.4.3/src/reqstool/model_generators/requirements_model_generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -223,15 +223,15 @@
                 )
 
                 r_systems.append(git_system)
 
     def __parse_requirement_filters(self, data) -> Dict[str, RequirementFilter]:  # NOSONAR
         r_filters = {}
 
-        self.semantic_validator._validate_req_imports_filter_has_exclude_xor_imports(data)
+        self.semantic_validator._validate_req_imports_filter_has_excludes_xor_includes(data)
 
         if "filters" in data:
             for urn in data["filters"].keys():
                 urn_filter = data["filters"][urn]
 
                 req_urn_ids_imports: Set[str] = None  # NOSONAR
                 req_urn_ids_excludes: Set[str] = None  # NOSONAR
@@ -257,16 +257,16 @@
                             utils.convert_ids_to_urn_id(urn=urn, ids=req_ids_excludes)
                         )
 
                 if "custom" in urn_filter:
                     if "includes" in urn_filter["custom"]:
                         custom_includes = urn_filter["custom"]["includes"]
 
-                    if "exclude" in urn_filter["custom"]:
-                        custom_exclude = urn_filter["custom"]["exclude"]
+                    if "excludes" in urn_filter["custom"]:
+                        custom_exclude = urn_filter["custom"]["excludes"]
 
                 req_filter = RequirementFilter(
                     urn_ids_imports=req_urn_ids_imports,
                     urn_ids_excludes=req_urn_ids_excludes,
                     custom_imports=custom_includes,
                     custom_exclude=custom_exclude,
                 )
```

### Comparing `reqstool-0.4.2/src/reqstool/model_generators/svcs_model_generator.py` & `reqstool-0.4.3/src/reqstool/model_generators/svcs_model_generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,15 +64,15 @@
                 r_result[svc.id] = svc
 
         return r_result
 
     def __parse_svc_filters(self, data) -> Dict[str, SVCFilter]:  # NOSONAR
         r_filters = {}
 
-        self.semantic_validator._validate_svc_imports_filter_has_exclude_xor_imports(data)
+        self.semantic_validator._validate_svc_imports_filter_has_excludes_xor_includes(data)
 
         if "filters" in data:
             for urn in data["filters"].keys():
                 urn_filter = data["filters"][urn]
 
                 svc_urn_ids_includes: Set[UrnId] = None  # NOSONAR
                 svc_urn_ids_excludes: Set[UrnId] = None  # NOSONAR
@@ -92,16 +92,16 @@
                         )
                         svc_urn_ids_excludes = set(utils.convert_ids_to_urn_id(urn=urn, ids=svc_ids_excludes))
 
                 if "custom" in urn_filter:
                     if "includes" in urn_filter["custom"]:
                         custom_includes = urn_filter["custom"]["includes"]
 
-                    if "exclude" in urn_filter["custom"]:
-                        custom_exclude = urn_filter["custom"]["exclude"]
+                    if "excludes" in urn_filter["custom"]:
+                        custom_exclude = urn_filter["custom"]["excludes"]
 
                 svc_filter = SVCFilter(
                     urn_ids_imports=svc_urn_ids_includes,
                     urn_ids_excludes=svc_urn_ids_excludes,
                     custom_imports=custom_includes,
                     custom_exclude=custom_exclude,
                 )
```

### Comparing `reqstool-0.4.2/src/reqstool/model_generators/testdata_model_generator.py` & `reqstool-0.4.3/src/reqstool/model_generators/testdata_model_generator.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import xml.etree.ElementTree as ET
 from pathlib import Path
 from typing import Dict
 
 from reqstool_python_decorators.decorators.decorators import Requirements
 
 from reqstool.common.dataclasses.urn_id import UrnId
-from reqstool.models.test_data import TestData, TestRunStatus, TestsData
+from reqstool.models.test_data import TEST_RUN_STATUS, TestData, TestsData
 
 
 class TestDataModelGenerator:
     UNIT_METHOD_IDENTIFIER_REGEX = r"^([a-zA-Z_$][a-zA-Z0-9_$]*).*$"
     KARATE_METHOD_IDENTIFIER_REGEX = r"\[\d+(?:\.\d+)?:\d+\]\s*(.+)"
 
     def __init__(self, path: str, urn: str):
@@ -46,22 +46,22 @@
                     methodname = match_unit.group(1)
                 elif match_karate:
                     methodname = match_karate.group(1)
                 else:
                     logging.error(f"{testcase.attrib['name']} is not a valid method name\n")
                     methodname = "invalid_method_name"
 
-                test_run_status: TestRunStatus
+                test_run_status: TEST_RUN_STATUS
 
                 if testcase.find("./failure") is not None:
-                    test_run_status = TestRunStatus.FAILED
+                    test_run_status = TEST_RUN_STATUS.FAILED
                 elif testcase.find("./skipped") is not None:
-                    test_run_status = TestRunStatus.SKIPPED
+                    test_run_status = TEST_RUN_STATUS.SKIPPED
                 else:
-                    test_run_status = TestRunStatus.PASSED
+                    test_run_status = TEST_RUN_STATUS.PASSED
 
                 fqn = f"{testcase.attrib['classname']}.{methodname}"
 
                 test_data = TestData(fully_qualified_name=fqn, status=test_run_status)
                 urn_id = UrnId(urn=urn, id=fqn)
                 r_testdata[urn_id] = test_data
```

### Comparing `reqstool-0.4.2/src/reqstool/models/combined_indexed_dataset.py` & `reqstool-0.4.3/src/reqstool/models/combined_indexed_dataset.py`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.2/src/reqstool/models/raw_datasets.py` & `reqstool-0.4.3/src/reqstool/models/raw_datasets.py`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.2/src/reqstool/models/requirements.py` & `reqstool-0.4.3/src/reqstool/models/requirements.py`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.2/src/reqstool/models/svcs.py` & `reqstool-0.4.3/src/reqstool/models/svcs.py`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.2/src/reqstool/reqstool_config/reqstool_config.py` & `reqstool-0.4.3/src/reqstool/reqstool_config/reqstool_config.py`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.2/src/reqstool/requirements_indata/requirements_indata.py` & `reqstool-0.4.3/src/reqstool/requirements_indata/requirements_indata.py`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.2/src/reqstool/requirements_indata/requirements_indata_paths.py` & `reqstool-0.4.3/src/reqstool/requirements_indata/requirements_indata_paths.py`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.2/src/reqstool/requirements_indata/java/java_maven_requirements_indata_paths.py` & `reqstool-0.4.3/src/reqstool/requirements_indata/java/java_maven_requirements_indata_paths.py`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.2/src/reqstool/resources/schemas/v1/annotations.schema.json` & `reqstool-0.4.3/src/reqstool/resources/schemas/v1/annotations.schema.json`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.2/src/reqstool/resources/schemas/v1/common.schema.json` & `reqstool-0.4.3/src/reqstool/resources/schemas/v1/common.schema.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999878118067612%*

 * *Differences: {"'$defs'": "{'filters': {'patternProperties': {'^.+$': {'properties': {'custom': {'properties': "*

 * *            "{replace: OrderedDict([('includes', OrderedDict([('$ref', "*

 * *            "'#/$defs/expressionLang')])), ('excludes', OrderedDict([('$ref', "*

 * *            "'#/$defs/expressionLang')]))])}, 'oneOf': {0: {'not': {'required': ['excludes']}}, 1: "*

 * *            "{'required': ['excludes']}}}}, 'allOf': {0: {'if': {'properties': {'custom': "*

 * *            "{'required': ['excludes']}}}}, 2: {'if': {'properties' […]*

```diff
@@ -54,15 +54,15 @@
                     "additionalProperties": false,
                     "allOf": [
                         {
                             "if": {
                                 "properties": {
                                     "custom": {
                                         "required": [
-                                            "exclude"
+                                            "excludes"
                                         ]
                                     }
                                 },
                                 "required": [
                                     "custom",
                                     "requirement_ids"
                                 ]
@@ -106,47 +106,47 @@
                             }
                         },
                         {
                             "if": {
                                 "properties": {
                                     "custom": {
                                         "required": [
-                                            "exclude"
+                                            "excludes"
                                         ]
                                     }
                                 },
                                 "required": [
                                     "custom",
-                                    "svcs_ids"
+                                    "svc_ids"
                                 ]
                             },
                             "then": {
                                 "properties": {
-                                    "svcs_ids": {
+                                    "svc_ids": {
                                         "not": {
                                             "required": [
                                                 "includes"
                                             ]
                                         }
                                     }
                                 }
                             }
                         },
                         {
                             "if": {
                                 "properties": {
-                                    "svcs_ids": {
+                                    "svc_ids": {
                                         "required": [
                                             "excludes"
                                         ]
                                     }
                                 },
                                 "required": [
                                     "custom",
-                                    "svcs_ids"
+                                    "svc_ids"
                                 ]
                             },
                             "then": {
                                 "properties": {
                                     "custom": {
                                         "not": {
                                             "required": [
@@ -158,15 +158,15 @@
                             }
                         },
                         {
                             "if": {
                                 "properties": {
                                     "custom": {
                                         "required": [
-                                            "exclude"
+                                            "excludes"
                                         ]
                                     }
                                 },
                                 "required": [
                                     "custom",
                                     "mvr_ids"
                                 ]
@@ -220,37 +220,37 @@
                         "custom": {
                             "additionalProperties": false,
                             "description": "Optionally includes or exclude requirements/verification cases using an expression language. Excludes have precedence and cannot be combined with includes",
                             "oneOf": [
                                 {
                                     "not": {
                                         "required": [
-                                            "exclude"
+                                            "excludes"
                                         ]
                                     },
                                     "required": [
                                         "includes"
                                     ]
                                 },
                                 {
                                     "not": {
                                         "required": [
                                             "includes"
                                         ]
                                     },
                                     "required": [
-                                        "exclude"
+                                        "excludes"
                                     ]
                                 }
                             ],
                             "properties": {
-                                "exclude": {
+                                "excludes": {
                                     "$ref": "#/$defs/expressionLang"
                                 },
-                                "imports": {
+                                "includes": {
                                     "$ref": "#/$defs/expressionLang"
                                 }
                             },
                             "type": "object"
                         }
                     },
                     "type": "object"
```

### Comparing `reqstool-0.4.2/src/reqstool/resources/schemas/v1/manual_verification_results.schema.json` & `reqstool-0.4.3/src/reqstool/resources/schemas/v1/manual_verification_results.schema.json`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.2/src/reqstool/resources/schemas/v1/reqstool_config.schema.json` & `reqstool-0.4.3/src/reqstool/resources/schemas/v1/reqstool_config.schema.json`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.2/src/reqstool/resources/schemas/v1/requirements.schema.json` & `reqstool-0.4.3/src/reqstool/resources/schemas/v1/requirements.schema.json`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.2/src/reqstool/resources/schemas/v1/software_verification_cases.schema.json` & `reqstool-0.4.3/src/reqstool/resources/schemas/v1/software_verification_cases.schema.json`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.2/tests/integration/reqstool/model_generators/test_included_models_generator.py` & `reqstool-0.4.3/tests/integration/reqstool/model_generators/test_included_models_generator.py`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.2/tests/resources/test_data/data/local/test_basic/baseline/ms-101/annotations.yml` & `reqstool-0.4.3/tests/resources/test_data/data/local/test_basic/baseline/ms-101/annotations.yml`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.2/tests/resources/test_data/data/local/test_basic/baseline/ms-101/requirements.yml` & `reqstool-0.4.3/tests/resources/test_data/data/local/test_basic/baseline/ms-101/requirements.yml`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.2/tests/resources/test_data/data/local/test_basic/baseline/ms-101/software_verification_cases.yml` & `reqstool-0.4.3/tests/resources/test_data/data/local/test_basic/baseline/ms-101/software_verification_cases.yml`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.2/tests/resources/test_data/data/local/test_basic/baseline/ms-101/test_results/failsafe/TEST-com.example.RequirementsExampleTestsIT.xml` & `reqstool-0.4.3/tests/resources/test_data/data/local/test_basic/baseline/ms-101/test_results/failsafe/TEST-com.example.RequirementsExampleTestsIT.xml`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.2/tests/resources/test_data/data/local/test_basic/baseline/ms-101/test_results/surefire/TEST-com.example.RequirementsExampleTests.xml` & `reqstool-0.4.3/tests/resources/test_data/data/local/test_basic/baseline/ms-101/test_results/surefire/TEST-com.example.RequirementsExampleTests.xml`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.2/tests/resources/test_data/data/local/test_basic/layout_maven/ms-101/pom.xml` & `reqstool-0.4.3/tests/resources/test_data/data/local/test_basic/layout_maven/ms-101/pom.xml`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.2/tests/resources/test_data/data/local/test_basic/with_requirements_config/README.md` & `reqstool-0.4.3/tests/resources/test_data/data/local/test_basic/with_requirements_config/README.md`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.2/tests/resources/test_data/data/local/test_errors/ms-101/annotations.yml` & `reqstool-0.4.3/tests/resources/test_data/data/local/test_errors/ms-101/annotations.yml`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.2/tests/resources/test_data/data/local/test_errors/ms-101/requirements.yml` & `reqstool-0.4.3/tests/resources/test_data/data/local/test_errors/ms-101/requirements.yml`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.2/tests/resources/test_data/data/local/test_errors/ms-101/software_verification_cases.yml` & `reqstool-0.4.3/tests/resources/test_data/data/local/test_errors/ms-101/software_verification_cases.yml`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.2/tests/resources/test_data/data/local/test_errors/ms-101/test_results/failsafe/TEST-com.example.RequirementsExampleTestsIT.xml` & `reqstool-0.4.3/tests/resources/test_data/data/local/test_errors/ms-101/test_results/failsafe/TEST-com.example.RequirementsExampleTestsIT.xml`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.2/tests/resources/test_data/data/local/test_errors/ms-101/test_results/surefire/TEST-com.example.RequirementsExampleTests.xml` & `reqstool-0.4.3/tests/resources/test_data/data/local/test_errors/ms-101/test_results/surefire/TEST-com.example.RequirementsExampleTests.xml`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.2/tests/resources/test_data/data/local/test_standard/baseline/visualization.adoc` & `reqstool-0.4.3/tests/resources/test_data/data/local/test_standard/baseline/visualization.adoc`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.2/tests/resources/test_data/data/local/test_standard/baseline/ms-001/annotations.yml` & `reqstool-0.4.3/tests/resources/test_data/data/local/test_standard/baseline/ms-001/annotations.yml`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.2/tests/resources/test_data/data/local/test_standard/baseline/ms-001/requirements.yml` & `reqstool-0.4.3/tests/resources/test_data/data/local/test_standard/baseline/ms-001/requirements.yml`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.2/tests/resources/test_data/data/local/test_standard/baseline/ms-001/software_verification_cases.yml` & `reqstool-0.4.3/tests/resources/test_data/data/local/test_standard/baseline/ms-001/software_verification_cases.yml`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.2/tests/resources/test_data/data/local/test_standard/baseline/ms-001/test_results/failsafe/TEST-com.reqstool.example.demo.DemoApplicationTestsIT.xml` & `reqstool-0.4.3/tests/resources/test_data/data/local/test_standard/baseline/ms-001/test_results/failsafe/TEST-com.reqstool.example.demo.DemoApplicationTestsIT.xml`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.2/tests/resources/test_data/data/local/test_standard/baseline/ms-001/test_results/surefire/TEST-com.reqstool.example.demo.SVCsTest.xml` & `reqstool-0.4.3/tests/resources/test_data/data/local/test_standard/baseline/ms-001/test_results/surefire/TEST-com.reqstool.example.demo.SVCsTest.xml`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.2/tests/resources/test_data/data/local/test_standard/baseline/sys-001/requirements.yml` & `reqstool-0.4.3/tests/resources/test_data/data/local/test_standard/baseline/sys-001/requirements.yml`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.2/tests/resources/test_data/data/local/test_standard/baseline/sys-001/software_verification_cases.yml` & `reqstool-0.4.3/tests/resources/test_data/data/local/test_standard/baseline/sys-001/software_verification_cases.yml`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.2/tests/resources/test_data/data/local/test_standard/baseline/sys-001/ext-001/requirements.yml` & `reqstool-0.4.3/tests/resources/test_data/data/local/test_standard/baseline/sys-001/ext-001/requirements.yml`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.2/tests/resources/test_data/data/local/test_standard/baseline/sys-001/ext-002/requirements.yml` & `reqstool-0.4.3/tests/resources/test_data/data/local/test_standard/baseline/sys-001/ext-002/requirements.yml`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.2/tests/resources/test_data/data/local/test_standard/empty_ms/ms-001/annotations.yml` & `reqstool-0.4.3/tests/resources/test_data/data/local/test_standard/empty_ms/ms-001/annotations.yml`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.2/tests/resources/test_data/data/local/test_standard/empty_ms/ms-001/test_results/failsafe/TEST-com.reqstool.example.demo.DemoApplicationTestsIT.xml` & `reqstool-0.4.3/tests/resources/test_data/data/local/test_standard/empty_ms/ms-001/test_results/failsafe/TEST-com.reqstool.example.demo.DemoApplicationTestsIT.xml`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.2/tests/resources/test_data/data/local/test_standard/empty_ms/ms-001/test_results/surefire/TEST-com.reqstool.example.demo.SVCsTest.xml` & `reqstool-0.4.3/tests/resources/test_data/data/local/test_standard/empty_ms/ms-001/test_results/surefire/TEST-com.reqstool.example.demo.SVCsTest.xml`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.2/tests/resources/test_data/data/local/test_standard/empty_ms/sys-001/requirements.yml` & `reqstool-0.4.3/tests/resources/test_data/data/local/test_standard/empty_ms/sys-001/requirements.yml`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.2/tests/resources/test_data/data/local/test_standard/empty_ms/sys-001/software_verification_cases.yml` & `reqstool-0.4.3/tests/resources/test_data/data/local/test_standard/empty_ms/sys-001/software_verification_cases.yml`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.2/tests/resources/test_data/data/local/test_standard/empty_ms/sys-001/ext-001/requirements.yml` & `reqstool-0.4.3/tests/resources/test_data/data/local/test_standard/empty_ms/sys-001/ext-001/requirements.yml`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.2/tests/resources/test_data/data/local/test_standard/empty_ms/sys-001/ext-002/requirements.yml` & `reqstool-0.4.3/tests/resources/test_data/data/local/test_standard/empty_ms/sys-001/ext-002/requirements.yml`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.2/tests/resources/test_data/data/remote/test_standard/test_standard_maven_git/sys-001/requirements.yml` & `reqstool-0.4.3/tests/resources/test_data/data/remote/test_standard/test_standard_maven_git/sys-001/requirements.yml`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.2/tests/resources/unit/reqstool/model_generators/test_annotations_model_generator/test_annotations_model_generator/annotations.yml` & `reqstool-0.4.3/tests/resources/unit/reqstool/model_generators/test_annotations_model_generator/test_annotations_model_generator/annotations.yml`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.2/tests/resources/unit/reqstool/model_generators/test_requirements_model_generator/test_external_requirements_model_generator/requirements.yml` & `reqstool-0.4.3/tests/resources/unit/reqstool/model_generators/test_requirements_model_generator/test_external_requirements_model_generator/requirements.yml`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.2/tests/resources/unit/reqstool/model_generators/test_requirements_model_generator/test_microservice_requirements_model_generator/requirements.yml` & `reqstool-0.4.3/tests/resources/unit/reqstool/model_generators/test_requirements_model_generator/test_microservice_requirements_model_generator/requirements.yml`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.2/tests/resources/unit/reqstool/model_generators/test_requirements_model_generator/test_rational_optional_model_generator/requirements.yml` & `reqstool-0.4.3/tests/resources/unit/reqstool/model_generators/test_requirements_model_generator/test_rational_optional_model_generator/requirements.yml`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.2/tests/resources/unit/reqstool/model_generators/test_requirements_model_generator/test_system_requirements_model_generator/requirements.yml` & `reqstool-0.4.3/tests/resources/unit/reqstool/model_generators/test_requirements_model_generator/test_system_requirements_model_generator/requirements.yml`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.2/tests/resources/unit/reqstool/model_generators/test_svcs_model_generator/test_svcs_model_generator/software_verification_cases.yml` & `reqstool-0.4.3/tests/resources/unit/reqstool/model_generators/test_svcs_model_generator/test_svcs_model_generator/software_verification_cases.yml`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.2/tests/unit/conftest.py` & `reqstool-0.4.3/tests/unit/conftest.py`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.2/tests/unit/reqstool/commands/report/test_report.py` & `reqstool-0.4.3/tests/unit/reqstool/commands/report/test_report.py`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.2/tests/unit/reqstool/commands/report/criterias/test_criterias.py` & `reqstool-0.4.3/tests/unit/reqstool/commands/report/criterias/test_criterias.py`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.2/tests/unit/reqstool/commands/status/test_statistics_container.py` & `reqstool-0.4.3/tests/unit/reqstool/commands/status/test_statistics_container.py`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.2/tests/unit/reqstool/commands/status/test_statistics_generator.py` & `reqstool-0.4.3/tests/unit/reqstool/commands/status/test_statistics_generator.py`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.2/tests/unit/reqstool/commands/status/test_status.py` & `reqstool-0.4.3/tests/unit/reqstool/commands/status/test_status.py`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.2/tests/unit/reqstool/common/test_locations.py` & `reqstool-0.4.3/tests/unit/reqstool/common/test_locations.py`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.2/tests/unit/reqstool/common/validators/test_semantic_validator.py` & `reqstool-0.4.3/tests/unit/reqstool/common/validators/test_semantic_validator.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,27 +21,27 @@
 
 
 @pytest.fixture
 def get_svcs_data_raw():
     # Data is raw since it's parsed directly from yaml data at runtime
     data = {
         "filters": {
-            "sys-001": {"svc_ids": {"imports": ["SVC_sys001_101", "SVC_sys001_109"], "excludes": ["SVC_sys001_101"]}}
+            "sys-001": {"svc_ids": {"includes": ["SVC_sys001_101", "SVC_sys001_109"], "excludes": ["SVC_sys001_101"]}}
         },
         "cases": {},
     }
     return data
 
 
 @pytest.fixture
 def get_systems_data_raw():
     # Data is raw since it's parsed directly from yaml data at runtime
     data = {
         "path": "../sys-001",
-        "filters": {"sys-001": {"requirement_ids": {"imports": ["REQ_sys001_101"], "excludes": ["REQ_sys001_102"]}}},
+        "filters": {"sys-001": {"requirement_ids": {"includes": ["REQ_sys001_101"], "excludes": ["REQ_sys001_102"]}}},
     }
 
     return data
 
 
 @pytest.fixture
 def get_requirements_data_raw():
@@ -54,15 +54,15 @@
             "url": "https://url.example.com",
         },
         "systems": {
             "local": [
                 {
                     "path": "../sys-001",
                     "filters": {
-                        "sys-001": {"requirement_ids": {"imports": ["REQ_sys001_103", "ext001:REQ_ext003_101"]}}
+                        "sys-001": {"requirement_ids": {"includes": ["REQ_sys001_103", "ext001:REQ_ext003_101"]}}
                     },
                 }
             ]
         },
         "requirements": [
             {
                 "id": "REQ_ms001_101",
@@ -89,15 +89,15 @@
     return data
 
 
 @pytest.fixture
 def get_svc_data():
     # Data is raw since it's parsed directly from yaml data at runtime
     data = {
-        "filters": {"sys-001": {"svc_ids": {"imports": ["SVC_sys001_101", "SVC_sys001_109"]}}},
+        "filters": {"sys-001": {"svc_ids": {"includes": ["SVC_sys001_101", "SVC_sys001_109"]}}},
         "cases": [
             {
                 "id": "SVC_ms001_101",
                 "requirement_ids": ["REQ_ms001_101"],
                 "title": "Some Title SVC_ms001_101",
                 "verification": "automated-test",
                 "revision": "0.0.1",
@@ -190,21 +190,21 @@
     errors = semantic_validator._validate_mvr_refers_to_existing_svc_ids(get_validation)
     expected_error = "MVR refers to non-existing svc id: <ms-101:SVC_20111>"
     assert expected_error in errors[0].msg
 
 
 def test_validate_svc_filter_exlude_xor_import(get_svcs_data_raw):
     semantic_validator = SemanticValidator(validation_error_holder=ValidationErrorHolder())
-    has_errors = semantic_validator._validate_svc_imports_filter_has_exclude_xor_imports(get_svcs_data_raw)
+    has_errors = semantic_validator._validate_svc_imports_filter_has_excludes_xor_includes(get_svcs_data_raw)
     expected_error = "Both imports and exclude filters applied to svc! (urn: sys-001)"
     errors = semantic_validator._validation_error_holder.get_errors()
     assert has_errors > 0
     assert expected_error in errors[0].msg
 
 
 def test_validate_req_filter_exlude_xor_import(get_systems_data_raw):
     semantic_validator = SemanticValidator(validation_error_holder=ValidationErrorHolder())
-    has_errors = semantic_validator._validate_req_imports_filter_has_exclude_xor_imports(get_systems_data_raw)
+    has_errors = semantic_validator._validate_req_imports_filter_has_excludes_xor_includes(get_systems_data_raw)
     expected_error = "Both imports and exclude filters applied to req! (urn: sys-001)"
     errors = semantic_validator._validation_error_holder.get_errors()
     assert has_errors > 0
     assert expected_error in errors[0].msg
```

### Comparing `reqstool-0.4.2/tests/unit/reqstool/expression_languages/test_requirements_el.py` & `reqstool-0.4.3/tests/unit/reqstool/expression_languages/test_requirements_el.py`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.2/tests/unit/reqstool/expression_languages/test_svcs_el.py` & `reqstool-0.4.3/tests/unit/reqstool/expression_languages/test_svcs_el.py`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.2/tests/unit/reqstool/filters/test_requirements_filters.py` & `reqstool-0.4.3/tests/unit/reqstool/filters/test_requirements_filters.py`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.2/tests/unit/reqstool/filters/test_software_verification_cases_filters.py` & `reqstool-0.4.3/tests/unit/reqstool/filters/test_software_verification_cases_filters.py`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.2/tests/unit/reqstool/locations/test_git_location.py` & `reqstool-0.4.3/tests/unit/reqstool/locations/test_git_location.py`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.2/tests/unit/reqstool/model_generators/test_annotations_model_generator.py` & `reqstool-0.4.3/tests/unit/reqstool/model_generators/test_annotations_model_generator.py`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.2/tests/unit/reqstool/model_generators/test_combined_indexed_dataset_generator.py` & `reqstool-0.4.3/tests/unit/reqstool/model_generators/test_combined_indexed_dataset_generator.py`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.2/tests/unit/reqstool/model_generators/test_combined_raw_datasets_generator.py` & `reqstool-0.4.3/tests/unit/reqstool/model_generators/test_combined_raw_datasets_generator.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,14 +68,15 @@
     semantic_validator = SemanticValidator(validation_error_holder=ValidationErrorHolder())
     combined_raw_datasets_generator.CombinedRawDatasetsGenerator(
         initial_location=LocalLocation(path=local_testdata_resources_rootdir_w_path("test_standard/baseline/sys-001")),
         semantic_validator=semantic_validator,
     )
 
 
+@SVCs("SVC_020")
 def test_missing_requirements_file(local_testdata_resources_rootdir_w_path):
     with pytest.raises(SystemExit) as excinfo:
         semantic_validator = SemanticValidator(validation_error_holder=ValidationErrorHolder())
         combined_raw_datasets_generator.CombinedRawDatasetsGenerator(
             initial_location=LocalLocation(
                 path=local_testdata_resources_rootdir_w_path("this/path/does/not/have/a/requirements/file")
             ),
```

### Comparing `reqstool-0.4.2/tests/unit/reqstool/model_generators/test_mvrs_model_generator.py` & `reqstool-0.4.3/tests/unit/reqstool/model_generators/test_mvrs_model_generator.py`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.2/tests/unit/reqstool/model_generators/test_requirements_model_generator.py` & `reqstool-0.4.3/tests/unit/reqstool/model_generators/test_requirements_model_generator.py`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.2/tests/unit/reqstool/model_generators/test_svcs_model_generator.py` & `reqstool-0.4.3/tests/unit/reqstool/model_generators/test_svcs_model_generator.py`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.2/tests/unit/reqstool/model_generators/test_testdata_model_generator.py` & `reqstool-0.4.3/tests/unit/reqstool/model_generators/test_testdata_model_generator.py`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.2/tests/unit/reqstool/models/test_annotations.py` & `reqstool-0.4.3/tests/unit/reqstool/models/test_annotations.py`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.2/tests/unit/reqstool/models/test_implementations.py` & `reqstool-0.4.3/tests/unit/reqstool/models/test_implementations.py`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.2/tests/unit/reqstool/models/test_imports.py` & `reqstool-0.4.3/tests/unit/reqstool/models/test_imports.py`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.2/tests/unit/reqstool/models/test_mvrs.py` & `reqstool-0.4.3/tests/unit/reqstool/models/test_mvrs.py`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.2/tests/unit/reqstool/models/test_requirements.py` & `reqstool-0.4.3/tests/unit/reqstool/models/test_requirements.py`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.2/tests/unit/reqstool/models/test_svcs.py` & `reqstool-0.4.3/tests/unit/reqstool/models/test_svcs.py`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.2/tests/unit/reqstool/reqstool_config/test_reqstool_config.py` & `reqstool-0.4.3/tests/unit/reqstool/reqstool_config/test_reqstool_config.py`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.2/tests/unit/reqstool/requirements_indata/test_requirements_indata_paths.py` & `reqstool-0.4.3/tests/unit/reqstool/requirements_indata/test_requirements_indata_paths.py`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.2/tests/unit/reqstool/resources/schemas/v1/test_json_schemas.py` & `reqstool-0.4.3/tests/unit/reqstool/resources/schemas/v1/test_json_schemas.py`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.2/.gitignore` & `reqstool-0.4.3/.gitignore`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.2/LICENSE` & `reqstool-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.2/README.md` & `reqstool-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `reqstool-0.4.2/pyproject.toml` & `reqstool-0.4.3/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -37,29 +37,30 @@
     "maven-artifact==0.3.4",
     "pygit2==1.14.1",
     "referencing==0.34.0",
     "requests-file==2.0.0",
     "ruamel.yaml==0.18.6",
     "tabulate==0.9.0",
     "xmldict==0.4.1",
-    "reqstool-python-decorators ==0.0.4",
+    "reqstool-python-decorators==0.0.4",
+    "packaging==24.0",
 ]
 
 [project.scripts]
 reqstool = "reqstool.command:main"
 
 [tool.hatch.version]
 source = "vcs"
 
 [tool.hatch.version.raw-options]
 local_scheme = "no-local-version"
 
 [tool.hatch.build.targets.wheel.hooks.decorators]
 dependencies = ["reqstool-python-hatch-plugin==0.0.3"]
-path = ["src","tests"]
+path = ["src", "tests"]
 
 [tool.hatch.envs.test]
 dependencies = ["pytest==8.0.0", "pytest-sugar==1.0.0", "pytest-cov==4.1.0"]
 
 [tool.hatch.envs.lint]
 detached = true
```

### Comparing `reqstool-0.4.2/PKG-INFO` & `reqstool-0.4.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.3
 Name: reqstool
-Version: 0.4.2
+Version: 0.4.3
 Summary: A tool for managing requirements with related tests and test results.
 Project-URL: Source, https://github.com/Luftfartsverket/reqstool-client
 Author-email: LFV <info@lfv.se>
 License-File: LICENSE
 Classifier: Development Status :: 3 - Alpha
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Requires-Dist: colorama==0.4.6
 Requires-Dist: jinja2==3.1.3
 Requires-Dist: jsonpickle==3.0.3
 Requires-Dist: jsonschema[format-nongpl]==4.21.1
 Requires-Dist: lark==1.1.9
 Requires-Dist: maven-artifact==0.3.4
+Requires-Dist: packaging==24.0
 Requires-Dist: pygit2==1.14.1
 Requires-Dist: referencing==0.34.0
 Requires-Dist: reqstool-python-decorators==0.0.4
 Requires-Dist: requests-file==2.0.0
 Requires-Dist: ruamel-yaml==0.18.6
 Requires-Dist: tabulate==0.9.0
 Requires-Dist: xmldict==0.4.1
```

