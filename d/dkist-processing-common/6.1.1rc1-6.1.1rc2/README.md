# Comparing `tmp/dkist-processing-common-6.1.1rc1.tar.gz` & `tmp/dkist-processing-common-6.1.1rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dkist-processing-common-6.1.1rc1.tar", last modified: Fri Apr  5 20:20:59 2024, max compression
+gzip compressed data, was "dkist-processing-common-6.1.1rc2.tar", last modified: Wed Apr 10 21:52:20 2024, max compression
```

## Comparing `dkist-processing-common-6.1.1rc1.tar` & `dkist-processing-common-6.1.1rc2.tar`

### file list

```diff
@@ -1,136 +1,137 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-05 20:20:59.080866 dkist-processing-common-6.1.1rc1/
--rw-rw-rw-   0 root         (0) root         (0)     2481 2024-04-05 20:20:52.000000 dkist-processing-common-6.1.1rc1/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)      844 2024-04-05 20:20:52.000000 dkist-processing-common-6.1.1rc1/.pre-commit-config.yaml
--rw-rw-rw-   0 root         (0) root         (0)      429 2024-04-05 20:20:52.000000 dkist-processing-common-6.1.1rc1/.readthedocs.yml
--rw-rw-rw-   0 root         (0) root         (0)    23402 2024-04-05 20:20:52.000000 dkist-processing-common-6.1.1rc1/CHANGELOG.rst
--rw-rw-rw-   0 root         (0) root         (0)     4370 2024-04-05 20:20:59.080866 dkist-processing-common-6.1.1rc1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     3730 2024-04-05 20:20:52.000000 dkist-processing-common-6.1.1rc1/README.rst
--rw-rw-rw-   0 root         (0) root         (0)     2610 2024-04-05 20:20:52.000000 dkist-processing-common-6.1.1rc1/bitbucket-pipelines.yml
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-05 20:20:59.064866 dkist-processing-common-6.1.1rc1/changelog/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-05 20:20:52.000000 dkist-processing-common-6.1.1rc1/changelog/.gitempty
--rw-rw-rw-   0 root         (0) root         (0)       81 2024-04-05 20:20:52.000000 dkist-processing-common-6.1.1rc1/changelog/180.misc.rst
--rw-rw-rw-   0 root         (0) root         (0)      140 2024-04-05 20:20:52.000000 dkist-processing-common-6.1.1rc1/changelog/181.misc.rst
--rwxrwxrwx   0 root         (0) root         (0)      642 2024-04-05 20:20:52.000000 dkist-processing-common-6.1.1rc1/check_changelog_updated.sh
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-05 20:20:59.064866 dkist-processing-common-6.1.1rc1/dkist_processing_common/
--rw-rw-rw-   0 root         (0) root         (0)      317 2024-04-05 20:20:52.000000 dkist-processing-common-6.1.1rc1/dkist_processing_common/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-05 20:20:59.064866 dkist-processing-common-6.1.1rc1/dkist_processing_common/_util/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-05 20:20:52.000000 dkist-processing-common-6.1.1rc1/dkist_processing_common/_util/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2931 2024-04-05 20:20:52.000000 dkist-processing-common-6.1.1rc1/dkist_processing_common/_util/config.py
--rw-rw-rw-   0 root         (0) root         (0)     3244 2024-04-05 20:20:52.000000 dkist-processing-common-6.1.1rc1/dkist_processing_common/_util/constants.py
--rw-rw-rw-   0 root         (0) root         (0)     1178 2024-04-05 20:20:52.000000 dkist-processing-common-6.1.1rc1/dkist_processing_common/_util/dkist_location.py
--rw-rw-rw-   0 root         (0) root         (0)     3426 2024-04-05 20:20:52.000000 dkist-processing-common-6.1.1rc1/dkist_processing_common/_util/graphql.py
--rw-rw-rw-   0 root         (0) root         (0)    10111 2024-04-05 20:20:52.000000 dkist-processing-common-6.1.1rc1/dkist_processing_common/_util/scratch.py
--rw-rw-rw-   0 root         (0) root         (0)     5868 2024-04-05 20:20:52.000000 dkist-processing-common-6.1.1rc1/dkist_processing_common/_util/tags.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-05 20:20:59.068866 dkist-processing-common-6.1.1rc1/dkist_processing_common/codecs/
--rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-05 20:20:52.000000 dkist-processing-common-6.1.1rc1/dkist_processing_common/codecs/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      823 2024-04-05 20:20:52.000000 dkist-processing-common-6.1.1rc1/dkist_processing_common/codecs/asdf.py
--rw-rw-rw-   0 root         (0) root         (0)      495 2024-04-05 20:20:52.000000 dkist-processing-common-6.1.1rc1/dkist_processing_common/codecs/bytes.py
--rw-rw-rw-   0 root         (0) root         (0)     2331 2024-04-05 20:20:52.000000 dkist-processing-common-6.1.1rc1/dkist_processing_common/codecs/fits.py
--rw-rw-rw-   0 root         (0) root         (0)      977 2024-04-05 20:20:52.000000 dkist-processing-common-6.1.1rc1/dkist_processing_common/codecs/iobase.py
--rw-rw-rw-   0 root         (0) root         (0)      939 2024-04-05 20:20:52.000000 dkist-processing-common-6.1.1rc1/dkist_processing_common/codecs/json.py
--rw-rw-rw-   0 root         (0) root         (0)      197 2024-04-05 20:20:52.000000 dkist-processing-common-6.1.1rc1/dkist_processing_common/codecs/path.py
--rw-rw-rw-   0 root         (0) root         (0)      679 2024-04-05 20:20:52.000000 dkist-processing-common-6.1.1rc1/dkist_processing_common/codecs/str.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-05 20:20:59.068866 dkist-processing-common-6.1.1rc1/dkist_processing_common/fonts/
--rw-rw-rw-   0 root         (0) root         (0)   656568 2024-04-05 20:20:52.000000 dkist-processing-common-6.1.1rc1/dkist_processing_common/fonts/Lato-Regular.ttf
--rw-rw-rw-   0 root         (0) root         (0)      101 2024-04-05 20:20:52.000000 dkist-processing-common-6.1.1rc1/dkist_processing_common/fonts/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7037 2024-04-05 20:20:52.000000 dkist-processing-common-6.1.1rc1/dkist_processing_common/manual.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-05 20:20:59.072866 dkist-processing-common-6.1.1rc1/dkist_processing_common/models/
--rw-rw-rw-   0 root         (0) root         (0)       74 2024-04-05 20:20:52.000000 dkist-processing-common-6.1.1rc1/dkist_processing_common/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5409 2024-04-05 20:20:52.000000 dkist-processing-common-6.1.1rc1/dkist_processing_common/models/constants.py
--rw-rw-rw-   0 root         (0) root         (0)     4113 2024-04-05 20:20:52.000000 dkist-processing-common-6.1.1rc1/dkist_processing_common/models/fits_access.py
--rw-rw-rw-   0 root         (0) root         (0)     5176 2024-04-05 20:20:52.000000 dkist-processing-common-6.1.1rc1/dkist_processing_common/models/flower_pot.py
--rw-rw-rw-   0 root         (0) root         (0)     3681 2024-04-05 20:20:52.000000 dkist-processing-common-6.1.1rc1/dkist_processing_common/models/graphql.py
--rw-rw-rw-   0 root         (0) root         (0)     1109 2024-04-05 20:20:52.000000 dkist-processing-common-6.1.1rc1/dkist_processing_common/models/message.py
--rw-rw-rw-   0 root         (0) root         (0)     6532 2024-04-05 20:20:52.000000 dkist-processing-common-6.1.1rc1/dkist_processing_common/models/parameters.py
--rw-rw-rw-   0 root         (0) root         (0)     2225 2024-04-05 20:20:52.000000 dkist-processing-common-6.1.1rc1/dkist_processing_common/models/quality.py
--rw-rw-rw-   0 root         (0) root         (0)     1096 2024-04-05 20:20:52.000000 dkist-processing-common-6.1.1rc1/dkist_processing_common/models/quality_json_encoders.py
--rw-rw-rw-   0 root         (0) root         (0)    11331 2024-04-05 20:20:52.000000 dkist-processing-common-6.1.1rc1/dkist_processing_common/models/tags.py
--rw-rw-rw-   0 root         (0) root         (0)      565 2024-04-05 20:20:52.000000 dkist-processing-common-6.1.1rc1/dkist_processing_common/models/task_name.py
--rw-rw-rw-   0 root         (0) root         (0)      870 2024-04-05 20:20:52.000000 dkist-processing-common-6.1.1rc1/dkist_processing_common/models/wavelength.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-05 20:20:59.072866 dkist-processing-common-6.1.1rc1/dkist_processing_common/parsers/
--rw-rw-rw-   0 root         (0) root         (0)       67 2024-04-05 20:20:52.000000 dkist-processing-common-6.1.1rc1/dkist_processing_common/parsers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6461 2024-04-05 20:20:52.000000 dkist-processing-common-6.1.1rc1/dkist_processing_common/parsers/cs_step.py
--rw-rw-rw-   0 root         (0) root         (0)     1571 2024-04-05 20:20:52.000000 dkist-processing-common-6.1.1rc1/dkist_processing_common/parsers/dsps_repeat.py
--rw-rw-rw-   0 root         (0) root         (0)      706 2024-04-05 20:20:52.000000 dkist-processing-common-6.1.1rc1/dkist_processing_common/parsers/experiment_id_bud.py
--rw-rw-rw-   0 root         (0) root         (0)     1536 2024-04-05 20:20:52.000000 dkist-processing-common-6.1.1rc1/dkist_processing_common/parsers/id_bud.py
--rw-rw-rw-   0 root         (0) root         (0)      921 2024-04-05 20:20:52.000000 dkist-processing-common-6.1.1rc1/dkist_processing_common/parsers/l0_fits_access.py
--rw-rw-rw-   0 root         (0) root         (0)     2595 2024-04-05 20:20:52.000000 dkist-processing-common-6.1.1rc1/dkist_processing_common/parsers/l1_fits_access.py
--rw-rw-rw-   0 root         (0) root         (0)      677 2024-04-05 20:20:52.000000 dkist-processing-common-6.1.1rc1/dkist_processing_common/parsers/proposal_id_bud.py
--rw-rw-rw-   0 root         (0) root         (0)     1058 2024-04-05 20:20:52.000000 dkist-processing-common-6.1.1rc1/dkist_processing_common/parsers/quality.py
--rw-rw-rw-   0 root         (0) root         (0)     1230 2024-04-05 20:20:52.000000 dkist-processing-common-6.1.1rc1/dkist_processing_common/parsers/single_value_single_key_flower.py
--rw-rw-rw-   0 root         (0) root         (0)     3938 2024-04-05 20:20:52.000000 dkist-processing-common-6.1.1rc1/dkist_processing_common/parsers/task.py
--rw-rw-rw-   0 root         (0) root         (0)     7839 2024-04-05 20:20:52.000000 dkist-processing-common-6.1.1rc1/dkist_processing_common/parsers/time.py
--rw-rw-rw-   0 root         (0) root         (0)     3041 2024-04-05 20:20:52.000000 dkist-processing-common-6.1.1rc1/dkist_processing_common/parsers/unique_bud.py
--rw-rw-rw-   0 root         (0) root         (0)      545 2024-04-05 20:20:52.000000 dkist-processing-common-6.1.1rc1/dkist_processing_common/parsers/wavelength.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-05 20:20:59.076866 dkist-processing-common-6.1.1rc1/dkist_processing_common/tasks/
--rw-rw-rw-   0 root         (0) root         (0)      562 2024-04-05 20:20:52.000000 dkist-processing-common-6.1.1rc1/dkist_processing_common/tasks/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    12488 2024-04-05 20:20:52.000000 dkist-processing-common-6.1.1rc1/dkist_processing_common/tasks/assemble_movie.py
--rw-rw-rw-   0 root         (0) root         (0)    12875 2024-04-05 20:20:52.000000 dkist-processing-common-6.1.1rc1/dkist_processing_common/tasks/base.py
--rw-rw-rw-   0 root         (0) root         (0)     8867 2024-04-05 20:20:52.000000 dkist-processing-common-6.1.1rc1/dkist_processing_common/tasks/l1_output_data.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-05 20:20:59.076866 dkist-processing-common-6.1.1rc1/dkist_processing_common/tasks/mixin/
--rw-rw-rw-   0 root         (0) root         (0)       68 2024-04-05 20:20:52.000000 dkist-processing-common-6.1.1rc1/dkist_processing_common/tasks/mixin/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6598 2024-04-05 20:20:52.000000 dkist-processing-common-6.1.1rc1/dkist_processing_common/tasks/mixin/globus.py
--rw-rw-rw-   0 root         (0) root         (0)     6813 2024-04-05 20:20:52.000000 dkist-processing-common-6.1.1rc1/dkist_processing_common/tasks/mixin/input_dataset.py
--rw-rw-rw-   0 root         (0) root         (0)     2077 2024-04-05 20:20:52.000000 dkist-processing-common-6.1.1rc1/dkist_processing_common/tasks/mixin/interservice_bus.py
--rw-rw-rw-   0 root         (0) root         (0)    14513 2024-04-05 20:20:52.000000 dkist-processing-common-6.1.1rc1/dkist_processing_common/tasks/mixin/metadata_store.py
--rw-rw-rw-   0 root         (0) root         (0)     3242 2024-04-05 20:20:52.000000 dkist-processing-common-6.1.1rc1/dkist_processing_common/tasks/mixin/object_store.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-05 20:20:59.076866 dkist-processing-common-6.1.1rc1/dkist_processing_common/tasks/mixin/quality/
--rw-rw-rw-   0 root         (0) root         (0)      383 2024-04-05 20:20:52.000000 dkist-processing-common-6.1.1rc1/dkist_processing_common/tasks/mixin/quality/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8287 2024-04-05 20:20:52.000000 dkist-processing-common-6.1.1rc1/dkist_processing_common/tasks/mixin/quality/_base.py
--rw-rw-rw-   0 root         (0) root         (0)    47891 2024-04-05 20:20:52.000000 dkist-processing-common-6.1.1rc1/dkist_processing_common/tasks/mixin/quality/_metrics.py
--rw-rw-rw-   0 root         (0) root         (0)     3699 2024-04-05 20:20:52.000000 dkist-processing-common-6.1.1rc1/dkist_processing_common/tasks/output_data_base.py
--rw-rw-rw-   0 root         (0) root         (0)     7986 2024-04-05 20:20:52.000000 dkist-processing-common-6.1.1rc1/dkist_processing_common/tasks/parse_l0_input_data.py
--rw-rw-rw-   0 root         (0) root         (0)     8852 2024-04-05 20:20:52.000000 dkist-processing-common-6.1.1rc1/dkist_processing_common/tasks/quality_metrics.py
--rw-rw-rw-   0 root         (0) root         (0)     2270 2024-04-05 20:20:52.000000 dkist-processing-common-6.1.1rc1/dkist_processing_common/tasks/teardown.py
--rw-rw-rw-   0 root         (0) root         (0)     5215 2024-04-05 20:20:52.000000 dkist-processing-common-6.1.1rc1/dkist_processing_common/tasks/transfer_input_data.py
--rw-rw-rw-   0 root         (0) root         (0)     5833 2024-04-05 20:20:52.000000 dkist-processing-common-6.1.1rc1/dkist_processing_common/tasks/trial_catalog.py
--rw-rw-rw-   0 root         (0) root         (0)     8200 2024-04-05 20:20:52.000000 dkist-processing-common-6.1.1rc1/dkist_processing_common/tasks/trial_output_data.py
--rw-rw-rw-   0 root         (0) root         (0)    19478 2024-04-05 20:20:52.000000 dkist-processing-common-6.1.1rc1/dkist_processing_common/tasks/write_l1.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-05 20:20:59.080866 dkist-processing-common-6.1.1rc1/dkist_processing_common/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-05 20:20:52.000000 dkist-processing-common-6.1.1rc1/dkist_processing_common/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    27099 2024-04-05 20:20:52.000000 dkist-processing-common-6.1.1rc1/dkist_processing_common/tests/conftest.py
--rw-rw-rw-   0 root         (0) root         (0)     4165 2024-04-05 20:20:52.000000 dkist-processing-common-6.1.1rc1/dkist_processing_common/tests/test_assemble_movie.py
--rw-rw-rw-   0 root         (0) root         (0)     7048 2024-04-05 20:20:52.000000 dkist-processing-common-6.1.1rc1/dkist_processing_common/tests/test_base.py
--rw-rw-rw-   0 root         (0) root         (0)    11068 2024-04-05 20:20:52.000000 dkist-processing-common-6.1.1rc1/dkist_processing_common/tests/test_codecs.py
--rw-rw-rw-   0 root         (0) root         (0)     5903 2024-04-05 20:20:52.000000 dkist-processing-common-6.1.1rc1/dkist_processing_common/tests/test_constants.py
--rw-rw-rw-   0 root         (0) root         (0)     2408 2024-04-05 20:20:52.000000 dkist-processing-common-6.1.1rc1/dkist_processing_common/tests/test_cs_step.py
--rw-rw-rw-   0 root         (0) root         (0)      513 2024-04-05 20:20:52.000000 dkist-processing-common-6.1.1rc1/dkist_processing_common/tests/test_dkist_location.py
--rw-rw-rw-   0 root         (0) root         (0)    10946 2024-04-05 20:20:52.000000 dkist-processing-common-6.1.1rc1/dkist_processing_common/tests/test_fits_access.py
--rw-rw-rw-   0 root         (0) root         (0)     3151 2024-04-05 20:20:52.000000 dkist-processing-common-6.1.1rc1/dkist_processing_common/tests/test_flower_pot.py
--rw-rw-rw-   0 root         (0) root         (0)    19450 2024-04-05 20:20:52.000000 dkist-processing-common-6.1.1rc1/dkist_processing_common/tests/test_input_dataset.py
--rw-rw-rw-   0 root         (0) root         (0)     3120 2024-04-05 20:20:52.000000 dkist-processing-common-6.1.1rc1/dkist_processing_common/tests/test_output_data_base.py
--rw-rw-rw-   0 root         (0) root         (0)     8346 2024-04-05 20:20:52.000000 dkist-processing-common-6.1.1rc1/dkist_processing_common/tests/test_parameters.py
--rw-rw-rw-   0 root         (0) root         (0)    10629 2024-04-05 20:20:52.000000 dkist-processing-common-6.1.1rc1/dkist_processing_common/tests/test_parse_l0_input_data.py
--rw-rw-rw-   0 root         (0) root         (0)     3198 2024-04-05 20:20:52.000000 dkist-processing-common-6.1.1rc1/dkist_processing_common/tests/test_publish_catalog_messages.py
--rw-rw-rw-   0 root         (0) root         (0)     9356 2024-04-05 20:20:52.000000 dkist-processing-common-6.1.1rc1/dkist_processing_common/tests/test_quality.py
--rw-rw-rw-   0 root         (0) root         (0)    36297 2024-04-05 20:20:52.000000 dkist-processing-common-6.1.1rc1/dkist_processing_common/tests/test_quality_mixin.py
--rw-rw-rw-   0 root         (0) root         (0)    16481 2024-04-05 20:20:52.000000 dkist-processing-common-6.1.1rc1/dkist_processing_common/tests/test_scratch.py
--rw-rw-rw-   0 root         (0) root         (0)    24306 2024-04-05 20:20:52.000000 dkist-processing-common-6.1.1rc1/dkist_processing_common/tests/test_stems.py
--rw-rw-rw-   0 root         (0) root         (0)     5023 2024-04-05 20:20:52.000000 dkist-processing-common-6.1.1rc1/dkist_processing_common/tests/test_tags.py
--rw-rw-rw-   0 root         (0) root         (0)     1234 2024-04-05 20:20:52.000000 dkist-processing-common-6.1.1rc1/dkist_processing_common/tests/test_task_name.py
--rw-rw-rw-   0 root         (0) root         (0)     4027 2024-04-05 20:20:52.000000 dkist-processing-common-6.1.1rc1/dkist_processing_common/tests/test_task_parsing.py
--rw-rw-rw-   0 root         (0) root         (0)     5494 2024-04-05 20:20:52.000000 dkist-processing-common-6.1.1rc1/dkist_processing_common/tests/test_teardown.py
--rw-rw-rw-   0 root         (0) root         (0)     6658 2024-04-05 20:20:52.000000 dkist-processing-common-6.1.1rc1/dkist_processing_common/tests/test_transfer_input_data.py
--rw-rw-rw-   0 root         (0) root         (0)     2109 2024-04-05 20:20:52.000000 dkist-processing-common-6.1.1rc1/dkist_processing_common/tests/test_transfer_l1_output_data.py
--rw-rw-rw-   0 root         (0) root         (0)     4253 2024-04-05 20:20:52.000000 dkist-processing-common-6.1.1rc1/dkist_processing_common/tests/test_trial_catalog.py
--rw-rw-rw-   0 root         (0) root         (0)    15740 2024-04-05 20:20:52.000000 dkist-processing-common-6.1.1rc1/dkist_processing_common/tests/test_trial_output_data.py
--rw-rw-rw-   0 root         (0) root         (0)    10488 2024-04-05 20:20:52.000000 dkist-processing-common-6.1.1rc1/dkist_processing_common/tests/test_workflow_task_base.py
--rw-rw-rw-   0 root         (0) root         (0)    17356 2024-04-05 20:20:52.000000 dkist-processing-common-6.1.1rc1/dkist_processing_common/tests/test_write_l1.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-05 20:20:59.064866 dkist-processing-common-6.1.1rc1/dkist_processing_common.egg-info/
--rw-rw-rw-   0 root         (0) root         (0)     4370 2024-04-05 20:20:59.000000 dkist-processing-common-6.1.1rc1/dkist_processing_common.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     5037 2024-04-05 20:20:59.000000 dkist-processing-common-6.1.1rc1/dkist_processing_common.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2024-04-05 20:20:59.000000 dkist-processing-common-6.1.1rc1/dkist_processing_common.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)      770 2024-04-05 20:20:59.000000 dkist-processing-common-6.1.1rc1/dkist_processing_common.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)       24 2024-04-05 20:20:59.000000 dkist-processing-common-6.1.1rc1/dkist_processing_common.egg-info/top_level.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-05 20:20:59.080866 dkist-processing-common-6.1.1rc1/docs/
--rw-rw-rw-   0 root         (0) root         (0)     4598 2024-04-05 20:20:52.000000 dkist-processing-common-6.1.1rc1/docs/Makefile
--rw-rw-rw-   0 root         (0) root         (0)      120 2024-04-05 20:20:52.000000 dkist-processing-common-6.1.1rc1/docs/changelog.rst
--rw-rw-rw-   0 root         (0) root         (0)     1890 2024-04-05 20:20:52.000000 dkist-processing-common-6.1.1rc1/docs/conf.py
--rw-rw-rw-   0 root         (0) root         (0)      113 2024-04-05 20:20:52.000000 dkist-processing-common-6.1.1rc1/docs/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     4513 2024-04-05 20:20:52.000000 dkist-processing-common-6.1.1rc1/docs/make.bat
--rw-rw-rw-   0 root         (0) root         (0)       29 2024-04-05 20:20:52.000000 dkist-processing-common-6.1.1rc1/docs/requirements.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-05 20:20:59.080866 dkist-processing-common-6.1.1rc1/licenses/
--rw-rw-rw-   0 root         (0) root         (0)     1462 2024-04-05 20:20:52.000000 dkist-processing-common-6.1.1rc1/licenses/LICENSE.rst
--rw-rw-rw-   0 root         (0) root         (0)      780 2024-04-05 20:20:52.000000 dkist-processing-common-6.1.1rc1/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)     1839 2024-04-05 20:20:59.084866 dkist-processing-common-6.1.1rc1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      102 2024-04-05 20:20:52.000000 dkist-processing-common-6.1.1rc1/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-10 21:52:20.777304 dkist-processing-common-6.1.1rc2/
+-rw-rw-rw-   0 root         (0) root         (0)     2481 2024-04-10 21:52:14.000000 dkist-processing-common-6.1.1rc2/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      844 2024-04-10 21:52:14.000000 dkist-processing-common-6.1.1rc2/.pre-commit-config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      429 2024-04-10 21:52:14.000000 dkist-processing-common-6.1.1rc2/.readthedocs.yml
+-rw-rw-rw-   0 root         (0) root         (0)    23402 2024-04-10 21:52:14.000000 dkist-processing-common-6.1.1rc2/CHANGELOG.rst
+-rw-rw-rw-   0 root         (0) root         (0)     4370 2024-04-10 21:52:20.777304 dkist-processing-common-6.1.1rc2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3730 2024-04-10 21:52:14.000000 dkist-processing-common-6.1.1rc2/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2610 2024-04-10 21:52:14.000000 dkist-processing-common-6.1.1rc2/bitbucket-pipelines.yml
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-10 21:52:20.765303 dkist-processing-common-6.1.1rc2/changelog/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-10 21:52:14.000000 dkist-processing-common-6.1.1rc2/changelog/.gitempty
+-rw-rw-rw-   0 root         (0) root         (0)      162 2024-04-10 21:52:14.000000 dkist-processing-common-6.1.1rc2/changelog/182.misc.rst
+-rw-rw-rw-   0 root         (0) root         (0)       96 2024-04-10 21:52:14.000000 dkist-processing-common-6.1.1rc2/changelog/183.misc.rst
+-rw-rw-rw-   0 root         (0) root         (0)       69 2024-04-10 21:52:14.000000 dkist-processing-common-6.1.1rc2/changelog/184.misc.rst
+-rwxrwxrwx   0 root         (0) root         (0)      642 2024-04-10 21:52:14.000000 dkist-processing-common-6.1.1rc2/check_changelog_updated.sh
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-10 21:52:20.765303 dkist-processing-common-6.1.1rc2/dkist_processing_common/
+-rw-rw-rw-   0 root         (0) root         (0)      317 2024-04-10 21:52:14.000000 dkist-processing-common-6.1.1rc2/dkist_processing_common/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-10 21:52:20.765303 dkist-processing-common-6.1.1rc2/dkist_processing_common/_util/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-10 21:52:14.000000 dkist-processing-common-6.1.1rc2/dkist_processing_common/_util/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2931 2024-04-10 21:52:14.000000 dkist-processing-common-6.1.1rc2/dkist_processing_common/_util/config.py
+-rw-rw-rw-   0 root         (0) root         (0)     3244 2024-04-10 21:52:14.000000 dkist-processing-common-6.1.1rc2/dkist_processing_common/_util/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)     1178 2024-04-10 21:52:14.000000 dkist-processing-common-6.1.1rc2/dkist_processing_common/_util/dkist_location.py
+-rw-rw-rw-   0 root         (0) root         (0)     3426 2024-04-10 21:52:14.000000 dkist-processing-common-6.1.1rc2/dkist_processing_common/_util/graphql.py
+-rw-rw-rw-   0 root         (0) root         (0)    10378 2024-04-10 21:52:14.000000 dkist-processing-common-6.1.1rc2/dkist_processing_common/_util/scratch.py
+-rw-rw-rw-   0 root         (0) root         (0)     6226 2024-04-10 21:52:14.000000 dkist-processing-common-6.1.1rc2/dkist_processing_common/_util/tags.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-10 21:52:20.769303 dkist-processing-common-6.1.1rc2/dkist_processing_common/codecs/
+-rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-10 21:52:14.000000 dkist-processing-common-6.1.1rc2/dkist_processing_common/codecs/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      823 2024-04-10 21:52:14.000000 dkist-processing-common-6.1.1rc2/dkist_processing_common/codecs/asdf.py
+-rw-rw-rw-   0 root         (0) root         (0)      495 2024-04-10 21:52:14.000000 dkist-processing-common-6.1.1rc2/dkist_processing_common/codecs/bytes.py
+-rw-rw-rw-   0 root         (0) root         (0)     2331 2024-04-10 21:52:14.000000 dkist-processing-common-6.1.1rc2/dkist_processing_common/codecs/fits.py
+-rw-rw-rw-   0 root         (0) root         (0)      977 2024-04-10 21:52:14.000000 dkist-processing-common-6.1.1rc2/dkist_processing_common/codecs/iobase.py
+-rw-rw-rw-   0 root         (0) root         (0)      939 2024-04-10 21:52:14.000000 dkist-processing-common-6.1.1rc2/dkist_processing_common/codecs/json.py
+-rw-rw-rw-   0 root         (0) root         (0)      197 2024-04-10 21:52:14.000000 dkist-processing-common-6.1.1rc2/dkist_processing_common/codecs/path.py
+-rw-rw-rw-   0 root         (0) root         (0)      679 2024-04-10 21:52:14.000000 dkist-processing-common-6.1.1rc2/dkist_processing_common/codecs/str.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-10 21:52:20.769303 dkist-processing-common-6.1.1rc2/dkist_processing_common/fonts/
+-rw-rw-rw-   0 root         (0) root         (0)   656568 2024-04-10 21:52:14.000000 dkist-processing-common-6.1.1rc2/dkist_processing_common/fonts/Lato-Regular.ttf
+-rw-rw-rw-   0 root         (0) root         (0)      101 2024-04-10 21:52:14.000000 dkist-processing-common-6.1.1rc2/dkist_processing_common/fonts/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7037 2024-04-10 21:52:14.000000 dkist-processing-common-6.1.1rc2/dkist_processing_common/manual.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-10 21:52:20.769303 dkist-processing-common-6.1.1rc2/dkist_processing_common/models/
+-rw-rw-rw-   0 root         (0) root         (0)       74 2024-04-10 21:52:14.000000 dkist-processing-common-6.1.1rc2/dkist_processing_common/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5409 2024-04-10 21:52:14.000000 dkist-processing-common-6.1.1rc2/dkist_processing_common/models/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)     4113 2024-04-10 21:52:14.000000 dkist-processing-common-6.1.1rc2/dkist_processing_common/models/fits_access.py
+-rw-rw-rw-   0 root         (0) root         (0)     5176 2024-04-10 21:52:14.000000 dkist-processing-common-6.1.1rc2/dkist_processing_common/models/flower_pot.py
+-rw-rw-rw-   0 root         (0) root         (0)     3333 2024-04-10 21:52:14.000000 dkist-processing-common-6.1.1rc2/dkist_processing_common/models/graphql.py
+-rw-rw-rw-   0 root         (0) root         (0)     1109 2024-04-10 21:52:14.000000 dkist-processing-common-6.1.1rc2/dkist_processing_common/models/message.py
+-rw-rw-rw-   0 root         (0) root         (0)     6532 2024-04-10 21:52:14.000000 dkist-processing-common-6.1.1rc2/dkist_processing_common/models/parameters.py
+-rw-rw-rw-   0 root         (0) root         (0)     2225 2024-04-10 21:52:14.000000 dkist-processing-common-6.1.1rc2/dkist_processing_common/models/quality.py
+-rw-rw-rw-   0 root         (0) root         (0)     1096 2024-04-10 21:52:14.000000 dkist-processing-common-6.1.1rc2/dkist_processing_common/models/quality_json_encoders.py
+-rw-rw-rw-   0 root         (0) root         (0)    11331 2024-04-10 21:52:14.000000 dkist-processing-common-6.1.1rc2/dkist_processing_common/models/tags.py
+-rw-rw-rw-   0 root         (0) root         (0)      565 2024-04-10 21:52:14.000000 dkist-processing-common-6.1.1rc2/dkist_processing_common/models/task_name.py
+-rw-rw-rw-   0 root         (0) root         (0)      870 2024-04-10 21:52:14.000000 dkist-processing-common-6.1.1rc2/dkist_processing_common/models/wavelength.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-10 21:52:20.773303 dkist-processing-common-6.1.1rc2/dkist_processing_common/parsers/
+-rw-rw-rw-   0 root         (0) root         (0)       67 2024-04-10 21:52:14.000000 dkist-processing-common-6.1.1rc2/dkist_processing_common/parsers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6461 2024-04-10 21:52:14.000000 dkist-processing-common-6.1.1rc2/dkist_processing_common/parsers/cs_step.py
+-rw-rw-rw-   0 root         (0) root         (0)     1571 2024-04-10 21:52:14.000000 dkist-processing-common-6.1.1rc2/dkist_processing_common/parsers/dsps_repeat.py
+-rw-rw-rw-   0 root         (0) root         (0)      706 2024-04-10 21:52:14.000000 dkist-processing-common-6.1.1rc2/dkist_processing_common/parsers/experiment_id_bud.py
+-rw-rw-rw-   0 root         (0) root         (0)     1536 2024-04-10 21:52:14.000000 dkist-processing-common-6.1.1rc2/dkist_processing_common/parsers/id_bud.py
+-rw-rw-rw-   0 root         (0) root         (0)      921 2024-04-10 21:52:14.000000 dkist-processing-common-6.1.1rc2/dkist_processing_common/parsers/l0_fits_access.py
+-rw-rw-rw-   0 root         (0) root         (0)     2595 2024-04-10 21:52:14.000000 dkist-processing-common-6.1.1rc2/dkist_processing_common/parsers/l1_fits_access.py
+-rw-rw-rw-   0 root         (0) root         (0)      677 2024-04-10 21:52:14.000000 dkist-processing-common-6.1.1rc2/dkist_processing_common/parsers/proposal_id_bud.py
+-rw-rw-rw-   0 root         (0) root         (0)     1058 2024-04-10 21:52:14.000000 dkist-processing-common-6.1.1rc2/dkist_processing_common/parsers/quality.py
+-rw-rw-rw-   0 root         (0) root         (0)     1230 2024-04-10 21:52:14.000000 dkist-processing-common-6.1.1rc2/dkist_processing_common/parsers/single_value_single_key_flower.py
+-rw-rw-rw-   0 root         (0) root         (0)     3938 2024-04-10 21:52:14.000000 dkist-processing-common-6.1.1rc2/dkist_processing_common/parsers/task.py
+-rw-rw-rw-   0 root         (0) root         (0)     7839 2024-04-10 21:52:14.000000 dkist-processing-common-6.1.1rc2/dkist_processing_common/parsers/time.py
+-rw-rw-rw-   0 root         (0) root         (0)     3041 2024-04-10 21:52:14.000000 dkist-processing-common-6.1.1rc2/dkist_processing_common/parsers/unique_bud.py
+-rw-rw-rw-   0 root         (0) root         (0)      545 2024-04-10 21:52:14.000000 dkist-processing-common-6.1.1rc2/dkist_processing_common/parsers/wavelength.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-10 21:52:20.773303 dkist-processing-common-6.1.1rc2/dkist_processing_common/tasks/
+-rw-rw-rw-   0 root         (0) root         (0)      562 2024-04-10 21:52:14.000000 dkist-processing-common-6.1.1rc2/dkist_processing_common/tasks/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    12488 2024-04-10 21:52:14.000000 dkist-processing-common-6.1.1rc2/dkist_processing_common/tasks/assemble_movie.py
+-rw-rw-rw-   0 root         (0) root         (0)    12852 2024-04-10 21:52:14.000000 dkist-processing-common-6.1.1rc2/dkist_processing_common/tasks/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     8867 2024-04-10 21:52:14.000000 dkist-processing-common-6.1.1rc2/dkist_processing_common/tasks/l1_output_data.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-10 21:52:20.773303 dkist-processing-common-6.1.1rc2/dkist_processing_common/tasks/mixin/
+-rw-rw-rw-   0 root         (0) root         (0)       68 2024-04-10 21:52:14.000000 dkist-processing-common-6.1.1rc2/dkist_processing_common/tasks/mixin/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6598 2024-04-10 21:52:14.000000 dkist-processing-common-6.1.1rc2/dkist_processing_common/tasks/mixin/globus.py
+-rw-rw-rw-   0 root         (0) root         (0)     6813 2024-04-10 21:52:14.000000 dkist-processing-common-6.1.1rc2/dkist_processing_common/tasks/mixin/input_dataset.py
+-rw-rw-rw-   0 root         (0) root         (0)     2077 2024-04-10 21:52:14.000000 dkist-processing-common-6.1.1rc2/dkist_processing_common/tasks/mixin/interservice_bus.py
+-rw-rw-rw-   0 root         (0) root         (0)    13806 2024-04-10 21:52:14.000000 dkist-processing-common-6.1.1rc2/dkist_processing_common/tasks/mixin/metadata_store.py
+-rw-rw-rw-   0 root         (0) root         (0)     3242 2024-04-10 21:52:14.000000 dkist-processing-common-6.1.1rc2/dkist_processing_common/tasks/mixin/object_store.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-10 21:52:20.773303 dkist-processing-common-6.1.1rc2/dkist_processing_common/tasks/mixin/quality/
+-rw-rw-rw-   0 root         (0) root         (0)      383 2024-04-10 21:52:14.000000 dkist-processing-common-6.1.1rc2/dkist_processing_common/tasks/mixin/quality/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8287 2024-04-10 21:52:14.000000 dkist-processing-common-6.1.1rc2/dkist_processing_common/tasks/mixin/quality/_base.py
+-rw-rw-rw-   0 root         (0) root         (0)    47891 2024-04-10 21:52:14.000000 dkist-processing-common-6.1.1rc2/dkist_processing_common/tasks/mixin/quality/_metrics.py
+-rw-rw-rw-   0 root         (0) root         (0)     3699 2024-04-10 21:52:14.000000 dkist-processing-common-6.1.1rc2/dkist_processing_common/tasks/output_data_base.py
+-rw-rw-rw-   0 root         (0) root         (0)     7986 2024-04-10 21:52:14.000000 dkist-processing-common-6.1.1rc2/dkist_processing_common/tasks/parse_l0_input_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     8852 2024-04-10 21:52:14.000000 dkist-processing-common-6.1.1rc2/dkist_processing_common/tasks/quality_metrics.py
+-rw-rw-rw-   0 root         (0) root         (0)     2270 2024-04-10 21:52:14.000000 dkist-processing-common-6.1.1rc2/dkist_processing_common/tasks/teardown.py
+-rw-rw-rw-   0 root         (0) root         (0)     5215 2024-04-10 21:52:14.000000 dkist-processing-common-6.1.1rc2/dkist_processing_common/tasks/transfer_input_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     5833 2024-04-10 21:52:14.000000 dkist-processing-common-6.1.1rc2/dkist_processing_common/tasks/trial_catalog.py
+-rw-rw-rw-   0 root         (0) root         (0)     8200 2024-04-10 21:52:14.000000 dkist-processing-common-6.1.1rc2/dkist_processing_common/tasks/trial_output_data.py
+-rw-rw-rw-   0 root         (0) root         (0)    19073 2024-04-10 21:52:14.000000 dkist-processing-common-6.1.1rc2/dkist_processing_common/tasks/write_l1.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-10 21:52:20.777304 dkist-processing-common-6.1.1rc2/dkist_processing_common/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-10 21:52:14.000000 dkist-processing-common-6.1.1rc2/dkist_processing_common/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    26212 2024-04-10 21:52:14.000000 dkist-processing-common-6.1.1rc2/dkist_processing_common/tests/conftest.py
+-rw-rw-rw-   0 root         (0) root         (0)     4165 2024-04-10 21:52:14.000000 dkist-processing-common-6.1.1rc2/dkist_processing_common/tests/test_assemble_movie.py
+-rw-rw-rw-   0 root         (0) root         (0)     7048 2024-04-10 21:52:14.000000 dkist-processing-common-6.1.1rc2/dkist_processing_common/tests/test_base.py
+-rw-rw-rw-   0 root         (0) root         (0)    11068 2024-04-10 21:52:14.000000 dkist-processing-common-6.1.1rc2/dkist_processing_common/tests/test_codecs.py
+-rw-rw-rw-   0 root         (0) root         (0)     5903 2024-04-10 21:52:14.000000 dkist-processing-common-6.1.1rc2/dkist_processing_common/tests/test_constants.py
+-rw-rw-rw-   0 root         (0) root         (0)     2408 2024-04-10 21:52:14.000000 dkist-processing-common-6.1.1rc2/dkist_processing_common/tests/test_cs_step.py
+-rw-rw-rw-   0 root         (0) root         (0)      513 2024-04-10 21:52:14.000000 dkist-processing-common-6.1.1rc2/dkist_processing_common/tests/test_dkist_location.py
+-rw-rw-rw-   0 root         (0) root         (0)    10946 2024-04-10 21:52:14.000000 dkist-processing-common-6.1.1rc2/dkist_processing_common/tests/test_fits_access.py
+-rw-rw-rw-   0 root         (0) root         (0)     3151 2024-04-10 21:52:14.000000 dkist-processing-common-6.1.1rc2/dkist_processing_common/tests/test_flower_pot.py
+-rw-rw-rw-   0 root         (0) root         (0)    19450 2024-04-10 21:52:14.000000 dkist-processing-common-6.1.1rc2/dkist_processing_common/tests/test_input_dataset.py
+-rw-rw-rw-   0 root         (0) root         (0)     3120 2024-04-10 21:52:14.000000 dkist-processing-common-6.1.1rc2/dkist_processing_common/tests/test_output_data_base.py
+-rw-rw-rw-   0 root         (0) root         (0)     8346 2024-04-10 21:52:14.000000 dkist-processing-common-6.1.1rc2/dkist_processing_common/tests/test_parameters.py
+-rw-rw-rw-   0 root         (0) root         (0)    10629 2024-04-10 21:52:14.000000 dkist-processing-common-6.1.1rc2/dkist_processing_common/tests/test_parse_l0_input_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     3198 2024-04-10 21:52:14.000000 dkist-processing-common-6.1.1rc2/dkist_processing_common/tests/test_publish_catalog_messages.py
+-rw-rw-rw-   0 root         (0) root         (0)     9356 2024-04-10 21:52:14.000000 dkist-processing-common-6.1.1rc2/dkist_processing_common/tests/test_quality.py
+-rw-rw-rw-   0 root         (0) root         (0)    36297 2024-04-10 21:52:14.000000 dkist-processing-common-6.1.1rc2/dkist_processing_common/tests/test_quality_mixin.py
+-rw-rw-rw-   0 root         (0) root         (0)    16481 2024-04-10 21:52:14.000000 dkist-processing-common-6.1.1rc2/dkist_processing_common/tests/test_scratch.py
+-rw-rw-rw-   0 root         (0) root         (0)    24306 2024-04-10 21:52:14.000000 dkist-processing-common-6.1.1rc2/dkist_processing_common/tests/test_stems.py
+-rw-rw-rw-   0 root         (0) root         (0)     5023 2024-04-10 21:52:14.000000 dkist-processing-common-6.1.1rc2/dkist_processing_common/tests/test_tags.py
+-rw-rw-rw-   0 root         (0) root         (0)     1234 2024-04-10 21:52:14.000000 dkist-processing-common-6.1.1rc2/dkist_processing_common/tests/test_task_name.py
+-rw-rw-rw-   0 root         (0) root         (0)     4027 2024-04-10 21:52:14.000000 dkist-processing-common-6.1.1rc2/dkist_processing_common/tests/test_task_parsing.py
+-rw-rw-rw-   0 root         (0) root         (0)     6052 2024-04-10 21:52:14.000000 dkist-processing-common-6.1.1rc2/dkist_processing_common/tests/test_teardown.py
+-rw-rw-rw-   0 root         (0) root         (0)     6658 2024-04-10 21:52:14.000000 dkist-processing-common-6.1.1rc2/dkist_processing_common/tests/test_transfer_input_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     2109 2024-04-10 21:52:14.000000 dkist-processing-common-6.1.1rc2/dkist_processing_common/tests/test_transfer_l1_output_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     4253 2024-04-10 21:52:14.000000 dkist-processing-common-6.1.1rc2/dkist_processing_common/tests/test_trial_catalog.py
+-rw-rw-rw-   0 root         (0) root         (0)    15911 2024-04-10 21:52:14.000000 dkist-processing-common-6.1.1rc2/dkist_processing_common/tests/test_trial_output_data.py
+-rw-rw-rw-   0 root         (0) root         (0)    10488 2024-04-10 21:52:14.000000 dkist-processing-common-6.1.1rc2/dkist_processing_common/tests/test_workflow_task_base.py
+-rw-rw-rw-   0 root         (0) root         (0)    15170 2024-04-10 21:52:14.000000 dkist-processing-common-6.1.1rc2/dkist_processing_common/tests/test_write_l1.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-10 21:52:20.765303 dkist-processing-common-6.1.1rc2/dkist_processing_common.egg-info/
+-rw-rw-rw-   0 root         (0) root         (0)     4370 2024-04-10 21:52:20.000000 dkist-processing-common-6.1.1rc2/dkist_processing_common.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     5060 2024-04-10 21:52:20.000000 dkist-processing-common-6.1.1rc2/dkist_processing_common.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2024-04-10 21:52:20.000000 dkist-processing-common-6.1.1rc2/dkist_processing_common.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)      770 2024-04-10 21:52:20.000000 dkist-processing-common-6.1.1rc2/dkist_processing_common.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)       24 2024-04-10 21:52:20.000000 dkist-processing-common-6.1.1rc2/dkist_processing_common.egg-info/top_level.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-10 21:52:20.777304 dkist-processing-common-6.1.1rc2/docs/
+-rw-rw-rw-   0 root         (0) root         (0)     4598 2024-04-10 21:52:14.000000 dkist-processing-common-6.1.1rc2/docs/Makefile
+-rw-rw-rw-   0 root         (0) root         (0)      120 2024-04-10 21:52:14.000000 dkist-processing-common-6.1.1rc2/docs/changelog.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1890 2024-04-10 21:52:14.000000 dkist-processing-common-6.1.1rc2/docs/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)      113 2024-04-10 21:52:14.000000 dkist-processing-common-6.1.1rc2/docs/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     4513 2024-04-10 21:52:14.000000 dkist-processing-common-6.1.1rc2/docs/make.bat
+-rw-rw-rw-   0 root         (0) root         (0)       29 2024-04-10 21:52:14.000000 dkist-processing-common-6.1.1rc2/docs/requirements.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-10 21:52:20.777304 dkist-processing-common-6.1.1rc2/licenses/
+-rw-rw-rw-   0 root         (0) root         (0)     1462 2024-04-10 21:52:14.000000 dkist-processing-common-6.1.1rc2/licenses/LICENSE.rst
+-rw-rw-rw-   0 root         (0) root         (0)      780 2024-04-10 21:52:14.000000 dkist-processing-common-6.1.1rc2/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)     1839 2024-04-10 21:52:20.777304 dkist-processing-common-6.1.1rc2/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      102 2024-04-10 21:52:14.000000 dkist-processing-common-6.1.1rc2/setup.py
```

### Comparing `dkist-processing-common-6.1.1rc1/.gitignore` & `dkist-processing-common-6.1.1rc2/.gitignore`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.1.1rc1/.pre-commit-config.yaml` & `dkist-processing-common-6.1.1rc2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.1.1rc1/CHANGELOG.rst` & `dkist-processing-common-6.1.1rc2/CHANGELOG.rst`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.1.1rc1/PKG-INFO` & `dkist-processing-common-6.1.1rc2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dkist-processing-common
-Version: 6.1.1rc1
+Version: 6.1.1rc2
 Summary: Common task classes used by the DKIST Science Data Processing pipelines to process DKIST data.
 Home-page: https://bitbucket.org/dkistdc/dkist-processing-common/src/main/
 Author: NSO / AURA
 Author-email: "dkistdc@nso.edu"
 License: MIT
 Project-URL: Documentation, https://docs.dkist.nso.edu/projects/common
 Classifier: Programming Language :: Python
```

### Comparing `dkist-processing-common-6.1.1rc1/README.rst` & `dkist-processing-common-6.1.1rc2/README.rst`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.1.1rc1/bitbucket-pipelines.yml` & `dkist-processing-common-6.1.1rc2/bitbucket-pipelines.yml`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.1.1rc1/check_changelog_updated.sh` & `dkist-processing-common-6.1.1rc2/check_changelog_updated.sh`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.1.1rc1/dkist_processing_common/_util/config.py` & `dkist-processing-common-6.1.1rc2/dkist_processing_common/_util/config.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.1.1rc1/dkist_processing_common/_util/constants.py` & `dkist-processing-common-6.1.1rc2/dkist_processing_common/_util/constants.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.1.1rc1/dkist_processing_common/_util/dkist_location.py` & `dkist-processing-common-6.1.1rc2/dkist_processing_common/_util/dkist_location.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.1.1rc1/dkist_processing_common/_util/graphql.py` & `dkist-processing-common-6.1.1rc2/dkist_processing_common/_util/graphql.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.1.1rc1/dkist_processing_common/_util/scratch.py` & `dkist-processing-common-6.1.1rc2/dkist_processing_common/_util/scratch.py`

 * *Files 8% similar despite different names*

```diff
@@ -46,14 +46,15 @@
             self.workflow_base_path.mkdir(parents=True, exist_ok=True)
         self._tag_db = TagDB(recipe_run_id=self.recipe_run_id, task_name=self.task_name)
         self._audit_db = TagDB(
             recipe_run_id=self.recipe_run_id, task_name=self.task_name, namespace="scratch_audit"
         )
         self._audit_write_tag = f"WRITE_{self.task_name}"
         self._audit_tag_tag = f"TAG_{self.task_name}"
+        self._audit_new_tag_cache = dict()
 
     @staticmethod
     @contextmanager
     def _mask():
         """Set a permissive umask to allow other users (e.g. globus) to modify resources created by the scratch library."""
         old_mask = umask(0)
         try:
@@ -112,25 +113,25 @@
 
         Returns
         -------
         None
         """
         tags = self._parse_tags(tags)
         path = self.absolute_path(relative_path)
+        # audit the path that was written to scratch
+        self._audit_db.add(tag=self._audit_write_tag, value=str(path))
         with self._mask():
             path.parent.mkdir(parents=True, exist_ok=True)
             if overwrite:
                 mode = "wb"
             else:
                 mode = "xb"
             with path.open(mode=mode) as f:
                 f.write(file_obj)
         self.tag(path, tags)
-        # audit the path that was written to scratch
-        self._audit_db.add(tag=self._audit_write_tag, value=str(path))
 
     def delete(self, path: Path | str):
         """
         Delete the file or path.
 
         Parameters
         ----------
@@ -168,19 +169,24 @@
             raise ValueError(
                 f"Cannot tag paths which are not children of the base path {self.workflow_base_path}"
             )
         if not path.exists():
             raise FileNotFoundError(f"Cannot tag paths which do not exist. {path=}")
 
         for tag in tags:
-            tag_is_new = not bool(self._tag_db.all(tags=tag))
-            self._tag_db.add(tag, str(path))
             # audit the tag that was newly added to the scratch tag db
-            if tag_is_new:
+            if self._tag_is_new(tag=tag):
                 self._audit_db.add(tag=self._audit_tag_tag, value=tag)
+            self._tag_db.add(tag, str(path))
+
+    def _tag_is_new(self, tag: str) -> bool:
+        if self._audit_new_tag_cache.get(tag, None) is None:
+            tag_is_new = not bool(self._tag_db.all(tags=tag))
+            self._audit_new_tag_cache[tag] = tag_is_new
+        return self._audit_new_tag_cache[tag]
 
     def tags(self, path: Path | str):
         """
         Return the tags associated with the given file object.
 
         Parameters
         ----------
```

### Comparing `dkist-processing-common-6.1.1rc1/dkist_processing_common/_util/tags.py` & `dkist-processing-common-6.1.1rc2/dkist_processing_common/_util/tags.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 """Tag cloud manager."""
 from pathlib import Path
 from typing import Iterable
 
 from redis import Redis
+from redis.backoff import FullJitterBackoff
+from redis.exceptions import ConnectionError
+from redis.retry import Retry
 
 from dkist_processing_common._util.config import service_configuration
 
 
 class TagDB:
     """
     Class for managing the tags database used to process and manage input data.
@@ -26,19 +29,26 @@
     def __init__(self, recipe_run_id: int, task_name: str, namespace: str = "path"):
         self.recipe_run_id = recipe_run_id
         self.task_name = task_name
         self._db = self.recipe_run_id % service_configuration.scratch_inventory_max_db_index
         self.namespace = f"{self.recipe_run_id}:{namespace}:"
         connection_name = f"{self.namespace}{self.task_name}"
         scratch_inventory = service_configuration.scratch_inventory_mesh_service
+        self.db_retry = Retry(
+            backoff=FullJitterBackoff(), retries=3, supported_errors=(ConnectionError,)
+        )
         self.db = Redis(
             db=self._db,
             host=scratch_inventory.host,
             port=scratch_inventory.port,
             client_name=connection_name,
+            retry_on_error=[
+                ConnectionError,
+            ],
+            retry=self.db_retry,
         )
 
     @staticmethod
     def _format_query_result(result: list[bytes]) -> set[str]:
         return {r.decode("utf8") for r in result}
 
     def _add_name_space(self, tags: Iterable[str] | str) -> Iterable[str] | str:
```

### Comparing `dkist-processing-common-6.1.1rc1/dkist_processing_common/codecs/asdf.py` & `dkist-processing-common-6.1.1rc2/dkist_processing_common/codecs/asdf.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.1.1rc1/dkist_processing_common/codecs/fits.py` & `dkist-processing-common-6.1.1rc2/dkist_processing_common/codecs/fits.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.1.1rc1/dkist_processing_common/codecs/iobase.py` & `dkist-processing-common-6.1.1rc2/dkist_processing_common/codecs/iobase.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.1.1rc1/dkist_processing_common/codecs/json.py` & `dkist-processing-common-6.1.1rc2/dkist_processing_common/codecs/json.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.1.1rc1/dkist_processing_common/codecs/str.py` & `dkist-processing-common-6.1.1rc2/dkist_processing_common/codecs/str.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.1.1rc1/dkist_processing_common/fonts/Lato-Regular.ttf` & `dkist-processing-common-6.1.1rc2/dkist_processing_common/fonts/Lato-Regular.ttf`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.1.1rc1/dkist_processing_common/manual.py` & `dkist-processing-common-6.1.1rc2/dkist_processing_common/manual.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.1.1rc1/dkist_processing_common/models/constants.py` & `dkist-processing-common-6.1.1rc2/dkist_processing_common/models/constants.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.1.1rc1/dkist_processing_common/models/fits_access.py` & `dkist-processing-common-6.1.1rc2/dkist_processing_common/models/fits_access.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.1.1rc1/dkist_processing_common/models/flower_pot.py` & `dkist-processing-common-6.1.1rc2/dkist_processing_common/models/flower_pot.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.1.1rc1/dkist_processing_common/models/graphql.py` & `dkist-processing-common-6.1.1rc2/dkist_processing_common/models/graphql.py`

 * *Files 10% similar despite different names*

```diff
@@ -62,50 +62,27 @@
 
     inputDatasetId: int
     isActive: bool
     inputDatasetInputDatasetParts: list[InputDatasetInputDatasetPartResponse]
 
 
 @dataclass
-class InputDatasetRecipeInstanceResponse:
-    """Recipe instance query response."""
-
-    inputDataset: InputDatasetResponse
-
-
-@dataclass
-class InputDatasetRecipeRunResponse:
-    """Recipe run query response."""
-
-    recipeInstance: InputDatasetRecipeInstanceResponse
-
-
-@dataclass
 class RecipeInstanceResponse:
     """Recipe instance query response."""
 
+    inputDataset: InputDatasetResponse
     recipeId: int
-    inputDatasetId: int
-
-
-@dataclass
-class RecipeRunProvenanceResponse:
-    """Response for the metadata store recipeRunProvenances and mutations endpoints."""
-
-    recipeRunProvenanceId: int
-    isTaskManual: bool
 
 
 @dataclass
 class RecipeRunResponse:
     """Recipe run query response."""
 
     recipeInstance: RecipeInstanceResponse
     recipeInstanceId: int
-    recipeRunProvenances: list[RecipeRunProvenanceResponse]
     configuration: str = None
 
 
 @dataclass
 class RecipeRunMutationResponse:
     """Recipe run mutation response."""
 
@@ -149,14 +126,21 @@
     taskName: str
     libraryVersions: str
     workflowVersion: str
     codeVersion: str = None
 
 
 @dataclass
+class RecipeRunProvenanceResponse:
+    """Response for the metadata store recipeRunProvenances and mutations endpoints."""
+
+    recipeRunProvenanceId: int
+
+
+@dataclass
 class QualityReportMutation:
     """Quality report mutation record."""
 
     datasetId: str
     qualityReport: str  # JSON
```

### Comparing `dkist-processing-common-6.1.1rc1/dkist_processing_common/models/message.py` & `dkist-processing-common-6.1.1rc2/dkist_processing_common/models/message.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.1.1rc1/dkist_processing_common/models/parameters.py` & `dkist-processing-common-6.1.1rc2/dkist_processing_common/models/parameters.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.1.1rc1/dkist_processing_common/models/quality.py` & `dkist-processing-common-6.1.1rc2/dkist_processing_common/models/quality.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.1.1rc1/dkist_processing_common/models/quality_json_encoders.py` & `dkist-processing-common-6.1.1rc2/dkist_processing_common/models/quality_json_encoders.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.1.1rc1/dkist_processing_common/models/tags.py` & `dkist-processing-common-6.1.1rc2/dkist_processing_common/models/tags.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.1.1rc1/dkist_processing_common/models/task_name.py` & `dkist-processing-common-6.1.1rc2/dkist_processing_common/models/task_name.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.1.1rc1/dkist_processing_common/models/wavelength.py` & `dkist-processing-common-6.1.1rc2/dkist_processing_common/models/wavelength.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.1.1rc1/dkist_processing_common/parsers/cs_step.py` & `dkist-processing-common-6.1.1rc2/dkist_processing_common/parsers/cs_step.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.1.1rc1/dkist_processing_common/parsers/dsps_repeat.py` & `dkist-processing-common-6.1.1rc2/dkist_processing_common/parsers/dsps_repeat.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.1.1rc1/dkist_processing_common/parsers/experiment_id_bud.py` & `dkist-processing-common-6.1.1rc2/dkist_processing_common/parsers/experiment_id_bud.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.1.1rc1/dkist_processing_common/parsers/id_bud.py` & `dkist-processing-common-6.1.1rc2/dkist_processing_common/parsers/id_bud.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.1.1rc1/dkist_processing_common/parsers/l0_fits_access.py` & `dkist-processing-common-6.1.1rc2/dkist_processing_common/parsers/l0_fits_access.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.1.1rc1/dkist_processing_common/parsers/l1_fits_access.py` & `dkist-processing-common-6.1.1rc2/dkist_processing_common/parsers/l1_fits_access.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.1.1rc1/dkist_processing_common/parsers/proposal_id_bud.py` & `dkist-processing-common-6.1.1rc2/dkist_processing_common/parsers/proposal_id_bud.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.1.1rc1/dkist_processing_common/parsers/quality.py` & `dkist-processing-common-6.1.1rc2/dkist_processing_common/parsers/quality.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.1.1rc1/dkist_processing_common/parsers/single_value_single_key_flower.py` & `dkist-processing-common-6.1.1rc2/dkist_processing_common/parsers/single_value_single_key_flower.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.1.1rc1/dkist_processing_common/parsers/task.py` & `dkist-processing-common-6.1.1rc2/dkist_processing_common/parsers/task.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.1.1rc1/dkist_processing_common/parsers/time.py` & `dkist-processing-common-6.1.1rc2/dkist_processing_common/parsers/time.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.1.1rc1/dkist_processing_common/parsers/unique_bud.py` & `dkist-processing-common-6.1.1rc2/dkist_processing_common/parsers/unique_bud.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.1.1rc1/dkist_processing_common/parsers/wavelength.py` & `dkist-processing-common-6.1.1rc2/dkist_processing_common/parsers/wavelength.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.1.1rc1/dkist_processing_common/tasks/__init__.py` & `dkist-processing-common-6.1.1rc2/dkist_processing_common/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.1.1rc1/dkist_processing_common/tasks/assemble_movie.py` & `dkist-processing-common-6.1.1rc2/dkist_processing_common/tasks/assemble_movie.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.1.1rc1/dkist_processing_common/tasks/base.py` & `dkist-processing-common-6.1.1rc2/dkist_processing_common/tasks/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -147,15 +147,15 @@
         self.metadata_store_record_provenance(
             is_task_manual=self.is_task_manual, library_versions=self.library_versions
         )
 
     def pre_run(self) -> None:
         """Execute any pre-task setup required."""
         super().pre_run()
-        if self.record_provenance or self.is_task_manual:
+        if self.record_provenance:
             with self.apm_task_step("Record Provenance"):
                 self._record_provenance()
 
     def read(
         self, tags: tag_type_hint, decoder: callable = path_decoder, **decoder_kwargs
     ) -> Generator[Any, None, None]:
         """
```

### Comparing `dkist-processing-common-6.1.1rc1/dkist_processing_common/tasks/l1_output_data.py` & `dkist-processing-common-6.1.1rc2/dkist_processing_common/tasks/l1_output_data.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.1.1rc1/dkist_processing_common/tasks/mixin/globus.py` & `dkist-processing-common-6.1.1rc2/dkist_processing_common/tasks/mixin/globus.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.1.1rc1/dkist_processing_common/tasks/mixin/input_dataset.py` & `dkist-processing-common-6.1.1rc2/dkist_processing_common/tasks/mixin/input_dataset.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.1.1rc1/dkist_processing_common/tasks/mixin/interservice_bus.py` & `dkist-processing-common-6.1.1rc2/dkist_processing_common/tasks/mixin/interservice_bus.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.1.1rc1/dkist_processing_common/tasks/mixin/metadata_store.py` & `dkist-processing-common-6.1.1rc2/dkist_processing_common/tasks/mixin/metadata_store.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 """Mixin for a WorkflowDataTaskBase subclass which implements Metadata Store data access functionality."""
 import json
 import logging
-from functools import cached_property
 
 from dkist_processing_common._util.config import service_configuration
 from dkist_processing_common._util.graphql import GraphQLClient
 from dkist_processing_common.models.graphql import DatasetCatalogReceiptAccountMutation
 from dkist_processing_common.models.graphql import DatasetCatalogReceiptAccountResponse
 from dkist_processing_common.models.graphql import InputDatasetPartResponse
-from dkist_processing_common.models.graphql import InputDatasetRecipeRunResponse
 from dkist_processing_common.models.graphql import QualityReportMutation
 from dkist_processing_common.models.graphql import QualityReportQuery
 from dkist_processing_common.models.graphql import QualityReportResponse
 from dkist_processing_common.models.graphql import RecipeRunMutation
 from dkist_processing_common.models.graphql import RecipeRunMutationResponse
 from dkist_processing_common.models.graphql import RecipeRunProvenanceMutation
 from dkist_processing_common.models.graphql import RecipeRunProvenanceResponse
@@ -111,27 +109,20 @@
                     f"Expected json encoded dictionary, received json encoded {type(configuration)}"
                 )
             return configuration
         except (json.JSONDecodeError, ValueError, TypeError, UnicodeDecodeError) as e:
             logger.error(f"Invalid recipe run configuration")
             raise e
 
-    @cached_property
+    @property
     def metadata_store_input_dataset_parts(self) -> list[InputDatasetPartResponse]:
         """Get the input dataset parts from the metadata store."""
-        params = RecipeRunQuery(recipeRunId=self.recipe_run_id)
-        response = self.metadata_store_client.execute_gql_query(
-            query_base="recipeRuns",
-            query_response_cls=InputDatasetRecipeRunResponse,
-            query_parameters=params,
-        )  # queried independently of other recipe run metadata for performance
-        recipe_run = response[0]
         return [
             part_link.inputDatasetPart
-            for part_link in recipe_run.recipeInstance.inputDataset.inputDatasetInputDatasetParts
+            for part_link in self._metadata_store_recipe_run().recipeInstance.inputDataset.inputDatasetInputDatasetParts
         ]
 
     def _metadata_store_filter_input_dataset_parts(
         self, input_dataset_part_type_name: str
     ) -> InputDatasetPartResponse | list[InputDatasetPartResponse] | None:
         """Filter the input dataset parts based on the input dataset part type name."""
         target_parts = [
@@ -216,31 +207,26 @@
         """Get the input dataset part document for parameters."""
         if part := self._metadata_store_input_dataset_parameters_part:
             return part.inputDatasetPartDocument
 
     @property
     def metadata_store_input_dataset_id(self) -> int:
         """Get the input dataset id from the metadata store."""
-        return self._metadata_store_recipe_run().recipeInstance.inputDatasetId
+        return self._metadata_store_recipe_run().recipeInstance.inputDataset.inputDatasetId
 
     @property
     def metadata_store_recipe_instance_id(self) -> int:
         """Get the recipe instance id from the metadata store."""
         return self._metadata_store_recipe_run().recipeInstanceId
 
     @property
     def metadata_store_recipe_id(self) -> int:
         """Get the recipe id from the metadata store."""
         return self._metadata_store_recipe_run().recipeInstance.recipeId
 
-    @property
-    def metadata_store_recipe_run_provenance(self) -> list[RecipeRunProvenanceResponse]:
-        """Get all the provenance records for the recipe run."""
-        return self._metadata_store_recipe_run().recipeRunProvenances
-
     def _metadata_store_recipe_run(self, allow_cache: bool = True) -> RecipeRunResponse:
         is_cached = bool(getattr(self, "_recipe_run_cache", False))
         if is_cached and allow_cache:
             return self._recipe_run_cache
         params = RecipeRunQuery(recipeRunId=self.recipe_run_id)
         response = self.metadata_store_client.execute_gql_query(
             query_base="recipeRuns",
```

### Comparing `dkist-processing-common-6.1.1rc1/dkist_processing_common/tasks/mixin/object_store.py` & `dkist-processing-common-6.1.1rc2/dkist_processing_common/tasks/mixin/object_store.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.1.1rc1/dkist_processing_common/tasks/mixin/quality/_base.py` & `dkist-processing-common-6.1.1rc2/dkist_processing_common/tasks/mixin/quality/_base.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.1.1rc1/dkist_processing_common/tasks/mixin/quality/_metrics.py` & `dkist-processing-common-6.1.1rc2/dkist_processing_common/tasks/mixin/quality/_metrics.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.1.1rc1/dkist_processing_common/tasks/output_data_base.py` & `dkist-processing-common-6.1.1rc2/dkist_processing_common/tasks/output_data_base.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.1.1rc1/dkist_processing_common/tasks/parse_l0_input_data.py` & `dkist-processing-common-6.1.1rc2/dkist_processing_common/tasks/parse_l0_input_data.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.1.1rc1/dkist_processing_common/tasks/quality_metrics.py` & `dkist-processing-common-6.1.1rc2/dkist_processing_common/tasks/quality_metrics.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.1.1rc1/dkist_processing_common/tasks/teardown.py` & `dkist-processing-common-6.1.1rc2/dkist_processing_common/tasks/teardown.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.1.1rc1/dkist_processing_common/tasks/transfer_input_data.py` & `dkist-processing-common-6.1.1rc2/dkist_processing_common/tasks/transfer_input_data.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.1.1rc1/dkist_processing_common/tasks/trial_catalog.py` & `dkist-processing-common-6.1.1rc2/dkist_processing_common/tasks/trial_catalog.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.1.1rc1/dkist_processing_common/tasks/trial_output_data.py` & `dkist-processing-common-6.1.1rc2/dkist_processing_common/tasks/trial_output_data.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.1.1rc1/dkist_processing_common/tasks/write_l1.py` & `dkist-processing-common-6.1.1rc2/dkist_processing_common/tasks/write_l1.py`

 * *Files 3% similar despite different names*

```diff
@@ -100,22 +100,14 @@
         return self.metadata_store_recipe_run_configuration().get("tile_size", None)
 
     @cached_property
     def validate_l1_on_write(self) -> bool:
         """Check for validate on write."""
         return self.metadata_store_recipe_run_configuration().get("validate_l1_on_write", True)
 
-    @cached_property
-    def _workflow_had_manual_intervention(self):
-        """Indicate determining if any provenance capturing steps had manual intervention."""
-        for provenance_record in self.metadata_store_recipe_run_provenance:
-            if provenance_record.isTaskManual:
-                return True
-        return False
-
     def _get_tile_size(self, data: np.ndarray) -> list | None:
         if self._tile_size_param is None:
             return None
         tile_size = []
         for dim_size in data.shape:
             if dim_size < self._tile_size_param:
                 tile_size.append(dim_size)
@@ -191,15 +183,14 @@
         if ids_obs_id := self.metadata_store_input_dataset_observe_frames_part_id:
             header["IDSOBSID"] = ids_obs_id
         if ids_cal_id := self.metadata_store_input_dataset_calibration_frames_part_id:
             header["IDSCALID"] = ids_cal_id
         header["WKFLNAME"] = self.workflow_name
         header["WKFLVERS"] = self.workflow_version
         header = self._add_contributing_id_headers(header=header)
-        header["MANPROCD"] = self._workflow_had_manual_intervention
         # Spectral line keywords
         wavelength_range = self.get_wavelength_range(header=header)
         spectral_lines = get_spectral_lines(
             wavelength_min=wavelength_range.min,
             wavelength_max=wavelength_range.max,
         )
         if spectral_lines:
```

### Comparing `dkist-processing-common-6.1.1rc1/dkist_processing_common/tests/conftest.py` & `dkist-processing-common-6.1.1rc2/dkist_processing_common/tests/conftest.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,32 +29,29 @@
 
 from dkist_processing_common._util.constants import ConstantsDb
 from dkist_processing_common._util.scratch import WorkflowFileSystem
 from dkist_processing_common._util.tags import TagDB
 from dkist_processing_common.models.graphql import InputDatasetInputDatasetPartResponse
 from dkist_processing_common.models.graphql import InputDatasetPartResponse
 from dkist_processing_common.models.graphql import InputDatasetPartTypeResponse
-from dkist_processing_common.models.graphql import InputDatasetRecipeInstanceResponse
-from dkist_processing_common.models.graphql import InputDatasetRecipeRunResponse
 from dkist_processing_common.models.graphql import InputDatasetResponse
 from dkist_processing_common.models.graphql import RecipeInstanceResponse
-from dkist_processing_common.models.graphql import RecipeRunProvenanceResponse
 from dkist_processing_common.models.graphql import RecipeRunResponse
 from dkist_processing_common.models.graphql import RecipeRunStatusResponse
 from dkist_processing_common.models.tags import Tag
 from dkist_processing_common.parsers.l0_fits_access import L0FitsAccess
 from dkist_processing_common.tasks import WorkflowTaskBase
 from dkist_processing_common.tasks.mixin.input_dataset import InputDatasetMixin
 
 TILE_SIZE = 64
 
 
 @pytest.fixture()
 def recipe_run_id():
-    return randint(0, 999999)
+    return randint(0, 99999)
 
 
 @pytest.fixture()
 def tag_db(recipe_run_id) -> TagDB:
     t = TagDB(recipe_run_id=recipe_run_id, task_name="test_tags")
     yield t
     t.purge()
@@ -335,82 +332,70 @@
         pass
 
     def execute_gql_query(self, **kwargs):
         query_base = kwargs["query_base"]
         if query_base == "recipeRunStatuses":
             return [RecipeRunStatusResponse(recipeRunStatusId=1)]
         if query_base == "recipeRuns":
-            if kwargs.get("query_response_cls") == InputDatasetRecipeRunResponse:
-                return [
-                    InputDatasetRecipeRunResponse(
-                        recipeInstance=InputDatasetRecipeInstanceResponse(
-                            inputDataset=InputDatasetResponse(
-                                inputDatasetId=1,
-                                isActive=True,
-                                inputDatasetInputDatasetParts=[
-                                    InputDatasetInputDatasetPartResponse(
-                                        inputDatasetPart=InputDatasetPartResponse(
-                                            inputDatasetPartId=1,
-                                            inputDatasetPartDocument='[{"parameterName": "", "parameterValues": [{"parameterValueId": 1, "parameterValue": "[[1,2,3],[4,5,6],[7,8,9]]", "parameterValueStartDate": "1/1/2000"}]}]',
-                                            inputDatasetPartType=InputDatasetPartTypeResponse(
-                                                inputDatasetPartTypeName="parameters"
-                                            ),
-                                        )
-                                    ),
-                                    InputDatasetInputDatasetPartResponse(
-                                        inputDatasetPart=InputDatasetPartResponse(
-                                            inputDatasetPartId=2,
-                                            inputDatasetPartDocument="""[
+            return [
+                RecipeRunResponse(
+                    recipeInstanceId=1,
+                    recipeInstance=RecipeInstanceResponse(
+                        recipeId=1,
+                        inputDataset=InputDatasetResponse(
+                            inputDatasetId=1,
+                            isActive=True,
+                            inputDatasetInputDatasetParts=[
+                                InputDatasetInputDatasetPartResponse(
+                                    inputDatasetPart=InputDatasetPartResponse(
+                                        inputDatasetPartId=1,
+                                        inputDatasetPartDocument='[{"parameterName": "", "parameterValues": [{"parameterValueId": 1, "parameterValue": "[[1,2,3],[4,5,6],[7,8,9]]", "parameterValueStartDate": "1/1/2000"}]}]',
+                                        inputDatasetPartType=InputDatasetPartTypeResponse(
+                                            inputDatasetPartTypeName="parameters"
+                                        ),
+                                    )
+                                ),
+                                InputDatasetInputDatasetPartResponse(
+                                    inputDatasetPart=InputDatasetPartResponse(
+                                        inputDatasetPartId=2,
+                                        inputDatasetPartDocument="""[
                                             {
                                                 "bucket": "bucket_name",
                                                 "object_keys": [
                                                     "key1",
                                                     "key2"
                                                 ]
                                             },
                                         ]""",
-                                            inputDatasetPartType=InputDatasetPartTypeResponse(
-                                                inputDatasetPartTypeName="observe_frames"
-                                            ),
-                                        )
-                                    ),
-                                    InputDatasetInputDatasetPartResponse(
-                                        inputDatasetPart=InputDatasetPartResponse(
-                                            inputDatasetPartId=3,
-                                            inputDatasetPartDocument="""[
+                                        inputDatasetPartType=InputDatasetPartTypeResponse(
+                                            inputDatasetPartTypeName="observe_frames"
+                                        ),
+                                    )
+                                ),
+                                InputDatasetInputDatasetPartResponse(
+                                    inputDatasetPart=InputDatasetPartResponse(
+                                        inputDatasetPartId=3,
+                                        inputDatasetPartDocument="""[
                                             {
                                                 "bucket": "bucket_name",
                                                 "object_keys": [
                                                     "key3",
                                                     "key4"
                                                 ]
                                             },
                                         ]""",
-                                            inputDatasetPartType=InputDatasetPartTypeResponse(
-                                                inputDatasetPartTypeName="calibration_frames"
-                                            ),
-                                        )
-                                    ),
-                                ],
-                            ),
+                                        inputDatasetPartType=InputDatasetPartTypeResponse(
+                                            inputDatasetPartTypeName="calibration_frames"
+                                        ),
+                                    )
+                                ),
+                            ],
                         ),
                     ),
-                ]
-
-            return [
-                RecipeRunResponse(
-                    recipeInstanceId=1,
-                    recipeInstance=RecipeInstanceResponse(
-                        recipeId=1,
-                        inputDatasetId=1,
-                    ),
                     configuration=f'{{"tile_size": {TILE_SIZE}}}',
-                    recipeRunProvenances=[
-                        RecipeRunProvenanceResponse(recipeRunProvenanceId=1, isTaskManual=False),
-                    ],
                 ),
             ]
 
     @staticmethod
     def execute_gql_mutation(**kwargs):
         ...
```

### Comparing `dkist-processing-common-6.1.1rc1/dkist_processing_common/tests/test_assemble_movie.py` & `dkist-processing-common-6.1.1rc2/dkist_processing_common/tests/test_assemble_movie.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.1.1rc1/dkist_processing_common/tests/test_base.py` & `dkist-processing-common-6.1.1rc2/dkist_processing_common/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.1.1rc1/dkist_processing_common/tests/test_codecs.py` & `dkist-processing-common-6.1.1rc2/dkist_processing_common/tests/test_codecs.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.1.1rc1/dkist_processing_common/tests/test_constants.py` & `dkist-processing-common-6.1.1rc2/dkist_processing_common/tests/test_constants.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.1.1rc1/dkist_processing_common/tests/test_cs_step.py` & `dkist-processing-common-6.1.1rc2/dkist_processing_common/tests/test_cs_step.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.1.1rc1/dkist_processing_common/tests/test_dkist_location.py` & `dkist-processing-common-6.1.1rc2/dkist_processing_common/tests/test_dkist_location.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.1.1rc1/dkist_processing_common/tests/test_fits_access.py` & `dkist-processing-common-6.1.1rc2/dkist_processing_common/tests/test_fits_access.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.1.1rc1/dkist_processing_common/tests/test_flower_pot.py` & `dkist-processing-common-6.1.1rc2/dkist_processing_common/tests/test_flower_pot.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.1.1rc1/dkist_processing_common/tests/test_input_dataset.py` & `dkist-processing-common-6.1.1rc2/dkist_processing_common/tests/test_input_dataset.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.1.1rc1/dkist_processing_common/tests/test_output_data_base.py` & `dkist-processing-common-6.1.1rc2/dkist_processing_common/tests/test_output_data_base.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.1.1rc1/dkist_processing_common/tests/test_parameters.py` & `dkist-processing-common-6.1.1rc2/dkist_processing_common/tests/test_parameters.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.1.1rc1/dkist_processing_common/tests/test_parse_l0_input_data.py` & `dkist-processing-common-6.1.1rc2/dkist_processing_common/tests/test_parse_l0_input_data.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.1.1rc1/dkist_processing_common/tests/test_publish_catalog_messages.py` & `dkist-processing-common-6.1.1rc2/dkist_processing_common/tests/test_publish_catalog_messages.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.1.1rc1/dkist_processing_common/tests/test_quality.py` & `dkist-processing-common-6.1.1rc2/dkist_processing_common/tests/test_quality.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.1.1rc1/dkist_processing_common/tests/test_quality_mixin.py` & `dkist-processing-common-6.1.1rc2/dkist_processing_common/tests/test_quality_mixin.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.1.1rc1/dkist_processing_common/tests/test_scratch.py` & `dkist-processing-common-6.1.1rc2/dkist_processing_common/tests/test_scratch.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.1.1rc1/dkist_processing_common/tests/test_stems.py` & `dkist-processing-common-6.1.1rc2/dkist_processing_common/tests/test_stems.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.1.1rc1/dkist_processing_common/tests/test_tags.py` & `dkist-processing-common-6.1.1rc2/dkist_processing_common/tests/test_tags.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.1.1rc1/dkist_processing_common/tests/test_task_name.py` & `dkist-processing-common-6.1.1rc2/dkist_processing_common/tests/test_task_name.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.1.1rc1/dkist_processing_common/tests/test_task_parsing.py` & `dkist-processing-common-6.1.1rc2/dkist_processing_common/tests/test_task_parsing.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.1.1rc1/dkist_processing_common/tests/test_teardown.py` & `dkist-processing-common-6.1.1rc2/dkist_processing_common/tests/test_teardown.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,34 +5,53 @@
 
 from dkist_processing_common._util.scratch import WorkflowFileSystem
 from dkist_processing_common.models.graphql import InputDatasetResponse
 from dkist_processing_common.models.graphql import RecipeInstanceResponse
 from dkist_processing_common.models.graphql import RecipeRunResponse
 from dkist_processing_common.models.tags import Tag
 from dkist_processing_common.tasks.teardown import Teardown
-from dkist_processing_common.tests.conftest import FakeGQLClient
 
 
 class TeardownTest(Teardown):
     def metadata_store_change_recipe_run_to_completed_successfully(self):
         pass
 
 
 @pytest.fixture()
 def make_mock_GQL_with_configuration():
     def class_generator(configuration: dict):
-        class TeardownFakeGQLClient(FakeGQLClient):
-            def execute_gql_query(self, **kwargs):
-                response = super().execute_gql_query(**kwargs)
-                if isinstance(response, list):
-                    if isinstance(response[0], RecipeRunResponse):
-                        response[0].configuration = json.dumps(configuration)
-                return response
+        class FakeGQLClient:
+            def __init__(self, *args, **kwargs):
+                pass
+
+            @staticmethod
+            def execute_gql_query(**kwargs):
+                query_base = kwargs["query_base"]
+
+                if query_base == "recipeRuns":
+                    return [
+                        RecipeRunResponse(
+                            recipeInstanceId=1,
+                            recipeInstance=RecipeInstanceResponse(
+                                recipeId=1,
+                                inputDataset=InputDatasetResponse(
+                                    inputDatasetId=1,
+                                    isActive=True,
+                                    inputDatasetInputDatasetParts=[],
+                                ),
+                            ),
+                            configuration=json.dumps(configuration),
+                        ),
+                    ]
+
+            @staticmethod
+            def execute_gql_mutation(**kwargs):
+                ...
 
-        return TeardownFakeGQLClient
+        return FakeGQLClient
 
     return class_generator
 
 
 @pytest.fixture(scope="session")
 def config_with_teardown_enabled() -> dict:
     return {"teardown_enabled": True}
```

### Comparing `dkist-processing-common-6.1.1rc1/dkist_processing_common/tests/test_transfer_input_data.py` & `dkist-processing-common-6.1.1rc2/dkist_processing_common/tests/test_transfer_input_data.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.1.1rc1/dkist_processing_common/tests/test_transfer_l1_output_data.py` & `dkist-processing-common-6.1.1rc2/dkist_processing_common/tests/test_transfer_l1_output_data.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.1.1rc1/dkist_processing_common/tests/test_trial_catalog.py` & `dkist-processing-common-6.1.1rc2/dkist_processing_common/tests/test_trial_catalog.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.1.1rc1/dkist_processing_common/tests/test_trial_output_data.py` & `dkist-processing-common-6.1.1rc2/dkist_processing_common/tests/test_trial_output_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,37 +5,47 @@
 import pytest
 
 from dkist_processing_common._util.scratch import WorkflowFileSystem
 from dkist_processing_common.models.graphql import RecipeRunResponse
 from dkist_processing_common.models.tags import Tag
 from dkist_processing_common.tasks.mixin.globus import GlobusTransferItem
 from dkist_processing_common.tasks.trial_output_data import TransferTrialDataBase
-from dkist_processing_common.tests.conftest import FakeGQLClient
 
 
 @pytest.fixture
 def destination_bucket() -> str:
     return "crazy"
 
 
 @pytest.fixture
 def recipe_run_configuration(custom_root_name, custom_dir_name, destination_bucket):
-    class GQLClientWithConfiguration(FakeGQLClient):
+    class GQLClientWithConfiguration:
+        def __init__(self, *args, **kwargs):
+            pass
+
         def execute_gql_query(self, **kwargs):
-            response = super().execute_gql_query(**kwargs)
-            if isinstance(response, list):
-                if isinstance(response[0], RecipeRunResponse):
-                    response[0].configuration = json.dumps(
-                        {
-                            "trial_root_directory_name": custom_root_name,
-                            "trial_directory_name": custom_dir_name,
-                            "destination_bucket": destination_bucket,
-                        }
-                    )
-            return response
+            query_base = kwargs["query_base"]
+            if query_base == "recipeRuns":
+                return [
+                    RecipeRunResponse(
+                        recipeInstanceId=1,
+                        recipeInstance=None,
+                        configuration=json.dumps(
+                            {
+                                "trial_root_directory_name": custom_root_name,
+                                "trial_directory_name": custom_dir_name,
+                                "destination_bucket": destination_bucket,
+                            }
+                        ),
+                    ),
+                ]
+
+        @staticmethod
+        def execute_gql_mutation(**kwargs):
+            ...
 
     return GQLClientWithConfiguration
 
 
 @pytest.fixture
 def dummy_globus_transfer_item() -> GlobusTransferItem:
     return GlobusTransferItem(source_path="foo", destination_path="bar", recursive=True)
```

### Comparing `dkist-processing-common-6.1.1rc1/dkist_processing_common/tests/test_workflow_task_base.py` & `dkist-processing-common-6.1.1rc2/dkist_processing_common/tests/test_workflow_task_base.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.1.1rc1/dkist_processing_common/tests/test_write_l1.py` & `dkist-processing-common-6.1.1rc2/dkist_processing_common/tests/test_write_l1.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,16 +10,14 @@
 from astropy.time import Time
 from astropy.time import TimeDelta
 from dkist_fits_specifications import __version__ as spec_version
 from dkist_header_validator import spec214_validator
 
 from dkist_processing_common import __version__ as common_version
 from dkist_processing_common.codecs.fits import fits_hdulist_encoder
-from dkist_processing_common.models.graphql import RecipeRunProvenanceResponse
-from dkist_processing_common.models.graphql import RecipeRunResponse
 from dkist_processing_common.models.tags import Tag
 from dkist_processing_common.models.wavelength import WavelengthRange
 from dkist_processing_common.tasks.write_l1 import WriteL1Frame
 from dkist_processing_common.tests.conftest import FakeGQLClient
 from dkist_processing_common.tests.conftest import FakeGQLClientNoRecipeConfiguration
 from dkist_processing_common.tests.conftest import TILE_SIZE
 
@@ -131,80 +129,22 @@
             )
             used_stokes_params.append(stokes_params[i])
         task.constants._update(asdict(FakeConstantDb()))
         yield task, used_stokes_params, header
         task._purge()
 
 
-@pytest.fixture()
-def make_mock_gql_client_with_provenance():
-    """Factory to create GraphQL client Mocks that will return customizable provenance records."""
-
-    def factory(provenances: list[RecipeRunProvenanceResponse]):
-        class WriteL1FakeGQLClient(FakeGQLClient):
-            def execute_gql_query(self, **kwargs):
-                response = super().execute_gql_query(**kwargs)
-                if isinstance(response, list):
-                    if isinstance(response[0], RecipeRunResponse):
-                        response: list[RecipeRunResponse]
-                        response[0].recipeRunProvenances = provenances
-                return response
-
-        return WriteL1FakeGQLClient
-
-    return factory
-
-
-@pytest.mark.parametrize(
-    "provenances, is_manual",
-    [
-        pytest.param(
-            [RecipeRunProvenanceResponse(recipeRunProvenanceId=1, isTaskManual=False)],
-            False,
-            id="auto_single",
-        ),
-        pytest.param(
-            [
-                RecipeRunProvenanceResponse(recipeRunProvenanceId=1, isTaskManual=False),
-                RecipeRunProvenanceResponse(recipeRunProvenanceId=2, isTaskManual=False),
-            ],
-            False,
-            id="auto_multiple",
-        ),
-        pytest.param(
-            [RecipeRunProvenanceResponse(recipeRunProvenanceId=1, isTaskManual=True)],
-            True,
-            id="manual_single",
-        ),
-        pytest.param(
-            [
-                RecipeRunProvenanceResponse(recipeRunProvenanceId=1, isTaskManual=False),
-                RecipeRunProvenanceResponse(recipeRunProvenanceId=2, isTaskManual=True),
-            ],
-            True,
-            id="manual_multiple",
-        ),
-    ],
-)
-def test_write_l1_frame(
-    write_l1_task,
-    mocker,
-    make_mock_gql_client_with_provenance,
-    provenances: list[RecipeRunProvenanceResponse],
-    is_manual,
-):
+def test_write_l1_frame(write_l1_task, mocker):
     """
     :Given: a write L1 task
     :When: running the task
     :Then: no errors are raised
     """
-    WriteL1GQLClient = make_mock_gql_client_with_provenance(provenances=provenances)
-
     mocker.patch(
-        "dkist_processing_common.tasks.mixin.metadata_store.GraphQLClient", new=WriteL1GQLClient
+        "dkist_processing_common.tasks.mixin.metadata_store.GraphQLClient", new=FakeGQLClient
     )
     mocker.patch(
         "dkist_processing_common.tasks.write_l1.WriteL1Frame._get_version_from_module_name",
         new_callable=Mock,
         return_value="fake_version_number",
     )
 
@@ -212,16 +152,14 @@
     task()
     for stokes_param in used_stokes_params:
         files = list(task.read(tags=[Tag.frame(), Tag.output(), Tag.stokes(stokes_param)]))
         assert len(files) == 1
         for file in files:
             assert file.exists
             spec214_validator.validate(file, extra=False)
-            with fits.open(file) as hdul:
-                assert hdul[-1].header["MANPROCD"] == is_manual
 
 
 def test_tags_preserved(write_l1_task, mocker):
     """
     :Given: an input header
     :When: converting that header to L1 and writing it to disk
     :Then: all tags that are not CALIBRATED are copied over to the new file
```

### Comparing `dkist-processing-common-6.1.1rc1/dkist_processing_common.egg-info/PKG-INFO` & `dkist-processing-common-6.1.1rc2/dkist_processing_common.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dkist-processing-common
-Version: 6.1.1rc1
+Version: 6.1.1rc2
 Summary: Common task classes used by the DKIST Science Data Processing pipelines to process DKIST data.
 Home-page: https://bitbucket.org/dkistdc/dkist-processing-common/src/main/
 Author: NSO / AURA
 Author-email: "dkistdc@nso.edu"
 License: MIT
 Project-URL: Documentation, https://docs.dkist.nso.edu/projects/common
 Classifier: Programming Language :: Python
```

### Comparing `dkist-processing-common-6.1.1rc1/dkist_processing_common.egg-info/SOURCES.txt` & `dkist-processing-common-6.1.1rc2/dkist_processing_common.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -5,16 +5,17 @@
 README.rst
 bitbucket-pipelines.yml
 check_changelog_updated.sh
 pyproject.toml
 setup.cfg
 setup.py
 changelog/.gitempty
-changelog/180.misc.rst
-changelog/181.misc.rst
+changelog/182.misc.rst
+changelog/183.misc.rst
+changelog/184.misc.rst
 dkist_processing_common/__init__.py
 dkist_processing_common/manual.py
 dkist_processing_common.egg-info/PKG-INFO
 dkist_processing_common.egg-info/SOURCES.txt
 dkist_processing_common.egg-info/dependency_links.txt
 dkist_processing_common.egg-info/requires.txt
 dkist_processing_common.egg-info/top_level.txt
```

### Comparing `dkist-processing-common-6.1.1rc1/dkist_processing_common.egg-info/requires.txt` & `dkist-processing-common-6.1.1rc2/dkist_processing_common.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.1.1rc1/docs/Makefile` & `dkist-processing-common-6.1.1rc2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.1.1rc1/docs/conf.py` & `dkist-processing-common-6.1.1rc2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.1.1rc1/docs/make.bat` & `dkist-processing-common-6.1.1rc2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.1.1rc1/licenses/LICENSE.rst` & `dkist-processing-common-6.1.1rc2/licenses/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.1.1rc1/pyproject.toml` & `dkist-processing-common-6.1.1rc2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.1.1rc1/setup.cfg` & `dkist-processing-common-6.1.1rc2/setup.cfg`

 * *Files identical despite different names*

