# Comparing `tmp/dkist-processing-common-3.0.0rc5.tar.gz` & `tmp/dkist-processing-common-3.0.0rc6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dkist-processing-common-3.0.0rc5.tar", last modified: Wed Jun 21 17:01:02 2023, max compression
+gzip compressed data, was "dkist-processing-common-3.0.0rc6.tar", last modified: Thu Jun 22 20:47:57 2023, max compression
```

## Comparing `dkist-processing-common-3.0.0rc5.tar` & `dkist-processing-common-3.0.0rc6.tar`

### file list

```diff
@@ -1,133 +1,133 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-21 17:01:02.371241 dkist-processing-common-3.0.0rc5/
--rw-rw-rw-   0 root         (0) root         (0)     2481 2023-06-21 17:00:55.000000 dkist-processing-common-3.0.0rc5/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)      844 2023-06-21 17:00:55.000000 dkist-processing-common-3.0.0rc5/.pre-commit-config.yaml
--rw-rw-rw-   0 root         (0) root         (0)      429 2023-06-21 17:00:55.000000 dkist-processing-common-3.0.0rc5/.readthedocs.yml
--rw-rw-rw-   0 root         (0) root         (0)    13348 2023-06-21 17:00:55.000000 dkist-processing-common-3.0.0rc5/CHANGELOG.rst
--rw-rw-rw-   0 root         (0) root         (0)     4327 2023-06-21 17:01:02.371241 dkist-processing-common-3.0.0rc5/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     3732 2023-06-21 17:00:55.000000 dkist-processing-common-3.0.0rc5/README.rst
--rw-rw-rw-   0 root         (0) root         (0)     2433 2023-06-21 17:00:55.000000 dkist-processing-common-3.0.0rc5/bitbucket-pipelines.yml
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-21 17:01:02.359241 dkist-processing-common-3.0.0rc5/changelog/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-21 17:00:55.000000 dkist-processing-common-3.0.0rc5/changelog/.gitempty
--rw-rw-rw-   0 root         (0) root         (0)      149 2023-06-21 17:00:55.000000 dkist-processing-common-3.0.0rc5/changelog/139.feature.2.rst
--rw-rw-rw-   0 root         (0) root         (0)       85 2023-06-21 17:00:55.000000 dkist-processing-common-3.0.0rc5/changelog/139.feature.rst
--rw-rw-rw-   0 root         (0) root         (0)      342 2023-06-21 17:00:55.000000 dkist-processing-common-3.0.0rc5/changelog/140.feature.rst
--rwxrwxrwx   0 root         (0) root         (0)      642 2023-06-21 17:00:55.000000 dkist-processing-common-3.0.0rc5/check_changelog_updated.sh
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-21 17:01:02.359241 dkist-processing-common-3.0.0rc5/dkist_processing_common/
--rw-rw-rw-   0 root         (0) root         (0)      317 2023-06-21 17:00:55.000000 dkist-processing-common-3.0.0rc5/dkist_processing_common/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-21 17:01:02.359241 dkist-processing-common-3.0.0rc5/dkist_processing_common/_util/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-21 17:00:55.000000 dkist-processing-common-3.0.0rc5/dkist_processing_common/_util/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1572 2023-06-21 17:00:55.000000 dkist-processing-common-3.0.0rc5/dkist_processing_common/_util/config.py
--rw-rw-rw-   0 root         (0) root         (0)     2409 2023-06-21 17:00:55.000000 dkist-processing-common-3.0.0rc5/dkist_processing_common/_util/constants.py
--rw-rw-rw-   0 root         (0) root         (0)     1178 2023-06-21 17:00:55.000000 dkist-processing-common-3.0.0rc5/dkist_processing_common/_util/dkist_location.py
--rw-rw-rw-   0 root         (0) root         (0)     1580 2023-06-21 17:00:55.000000 dkist-processing-common-3.0.0rc5/dkist_processing_common/_util/graphql.py
--rw-rw-rw-   0 root         (0) root         (0)     8215 2023-06-21 17:00:55.000000 dkist-processing-common-3.0.0rc5/dkist_processing_common/_util/scratch.py
--rw-rw-rw-   0 root         (0) root         (0)     5641 2023-06-21 17:00:55.000000 dkist-processing-common-3.0.0rc5/dkist_processing_common/_util/tags.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-21 17:01:02.363241 dkist-processing-common-3.0.0rc5/dkist_processing_common/codecs/
--rw-rw-rw-   0 root         (0) root         (0)      159 2023-06-21 17:00:55.000000 dkist-processing-common-3.0.0rc5/dkist_processing_common/codecs/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      495 2023-06-21 17:00:55.000000 dkist-processing-common-3.0.0rc5/dkist_processing_common/codecs/bytes.py
--rw-rw-rw-   0 root         (0) root         (0)     2030 2023-06-21 17:00:55.000000 dkist-processing-common-3.0.0rc5/dkist_processing_common/codecs/fits.py
--rw-rw-rw-   0 root         (0) root         (0)      900 2023-06-21 17:00:55.000000 dkist-processing-common-3.0.0rc5/dkist_processing_common/codecs/iobase.py
--rw-rw-rw-   0 root         (0) root         (0)      939 2023-06-21 17:00:55.000000 dkist-processing-common-3.0.0rc5/dkist_processing_common/codecs/json.py
--rw-rw-rw-   0 root         (0) root         (0)      197 2023-06-21 17:00:55.000000 dkist-processing-common-3.0.0rc5/dkist_processing_common/codecs/path.py
--rw-rw-rw-   0 root         (0) root         (0)      679 2023-06-21 17:00:55.000000 dkist-processing-common-3.0.0rc5/dkist_processing_common/codecs/str.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-21 17:01:02.363241 dkist-processing-common-3.0.0rc5/dkist_processing_common/fonts/
--rw-rw-rw-   0 root         (0) root         (0)   656568 2023-06-21 17:00:55.000000 dkist-processing-common-3.0.0rc5/dkist_processing_common/fonts/Lato-Regular.ttf
--rw-rw-rw-   0 root         (0) root         (0)      101 2023-06-21 17:00:55.000000 dkist-processing-common-3.0.0rc5/dkist_processing_common/fonts/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7037 2023-06-21 17:00:55.000000 dkist-processing-common-3.0.0rc5/dkist_processing_common/manual.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-21 17:01:02.363241 dkist-processing-common-3.0.0rc5/dkist_processing_common/models/
--rw-rw-rw-   0 root         (0) root         (0)       74 2023-06-21 17:00:55.000000 dkist-processing-common-3.0.0rc5/dkist_processing_common/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4766 2023-06-21 17:00:55.000000 dkist-processing-common-3.0.0rc5/dkist_processing_common/models/constants.py
--rw-rw-rw-   0 root         (0) root         (0)     3453 2023-06-21 17:00:55.000000 dkist-processing-common-3.0.0rc5/dkist_processing_common/models/fits_access.py
--rw-rw-rw-   0 root         (0) root         (0)     4176 2023-06-21 17:00:55.000000 dkist-processing-common-3.0.0rc5/dkist_processing_common/models/flower_pot.py
--rw-rw-rw-   0 root         (0) root         (0)     3514 2023-06-21 17:00:55.000000 dkist-processing-common-3.0.0rc5/dkist_processing_common/models/graphql.py
--rw-rw-rw-   0 root         (0) root         (0)     1109 2023-06-21 17:00:55.000000 dkist-processing-common-3.0.0rc5/dkist_processing_common/models/message.py
--rw-rw-rw-   0 root         (0) root         (0)     3408 2023-06-21 17:00:55.000000 dkist-processing-common-3.0.0rc5/dkist_processing_common/models/parameters.py
--rw-rw-rw-   0 root         (0) root         (0)     2225 2023-06-21 17:00:55.000000 dkist-processing-common-3.0.0rc5/dkist_processing_common/models/quality.py
--rw-rw-rw-   0 root         (0) root         (0)     1096 2023-06-21 17:00:55.000000 dkist-processing-common-3.0.0rc5/dkist_processing_common/models/quality_json_encoders.py
--rw-rw-rw-   0 root         (0) root         (0)     7510 2023-06-21 17:00:55.000000 dkist-processing-common-3.0.0rc5/dkist_processing_common/models/tags.py
--rw-rw-rw-   0 root         (0) root         (0)      870 2023-06-21 17:00:55.000000 dkist-processing-common-3.0.0rc5/dkist_processing_common/models/wavelength.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-21 17:01:02.367241 dkist-processing-common-3.0.0rc5/dkist_processing_common/parsers/
--rw-rw-rw-   0 root         (0) root         (0)       67 2023-06-21 17:00:55.000000 dkist-processing-common-3.0.0rc5/dkist_processing_common/parsers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6381 2023-06-21 17:00:55.000000 dkist-processing-common-3.0.0rc5/dkist_processing_common/parsers/cs_step.py
--rw-rw-rw-   0 root         (0) root         (0)     1827 2023-06-21 17:00:55.000000 dkist-processing-common-3.0.0rc5/dkist_processing_common/parsers/dsps_repeat.py
--rw-rw-rw-   0 root         (0) root         (0)      706 2023-06-21 17:00:55.000000 dkist-processing-common-3.0.0rc5/dkist_processing_common/parsers/experiment_id_bud.py
--rw-rw-rw-   0 root         (0) root         (0)     1767 2023-06-21 17:00:55.000000 dkist-processing-common-3.0.0rc5/dkist_processing_common/parsers/id_bud.py
--rw-rw-rw-   0 root         (0) root         (0)      921 2023-06-21 17:00:55.000000 dkist-processing-common-3.0.0rc5/dkist_processing_common/parsers/l0_fits_access.py
--rw-rw-rw-   0 root         (0) root         (0)     2451 2023-06-21 17:00:55.000000 dkist-processing-common-3.0.0rc5/dkist_processing_common/parsers/l1_fits_access.py
--rw-rw-rw-   0 root         (0) root         (0)      677 2023-06-21 17:00:55.000000 dkist-processing-common-3.0.0rc5/dkist_processing_common/parsers/proposal_id_bud.py
--rw-rw-rw-   0 root         (0) root         (0)     1058 2023-06-21 17:00:55.000000 dkist-processing-common-3.0.0rc5/dkist_processing_common/parsers/quality.py
--rw-rw-rw-   0 root         (0) root         (0)     1230 2023-06-21 17:00:55.000000 dkist-processing-common-3.0.0rc5/dkist_processing_common/parsers/single_value_single_key_flower.py
--rw-rw-rw-   0 root         (0) root         (0)     5720 2023-06-21 17:00:55.000000 dkist-processing-common-3.0.0rc5/dkist_processing_common/parsers/time.py
--rw-rw-rw-   0 root         (0) root         (0)     1669 2023-06-21 17:00:55.000000 dkist-processing-common-3.0.0rc5/dkist_processing_common/parsers/unique_bud.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-21 17:01:02.367241 dkist-processing-common-3.0.0rc5/dkist_processing_common/tasks/
--rw-rw-rw-   0 root         (0) root         (0)      504 2023-06-21 17:00:55.000000 dkist-processing-common-3.0.0rc5/dkist_processing_common/tasks/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11470 2023-06-21 17:00:55.000000 dkist-processing-common-3.0.0rc5/dkist_processing_common/tasks/assemble_movie.py
--rw-rw-rw-   0 root         (0) root         (0)     9049 2023-06-21 17:00:55.000000 dkist-processing-common-3.0.0rc5/dkist_processing_common/tasks/base.py
--rw-rw-rw-   0 root         (0) root         (0)     8689 2023-06-21 17:00:55.000000 dkist-processing-common-3.0.0rc5/dkist_processing_common/tasks/l1_output_data.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-21 17:01:02.367241 dkist-processing-common-3.0.0rc5/dkist_processing_common/tasks/mixin/
--rw-rw-rw-   0 root         (0) root         (0)       68 2023-06-21 17:00:55.000000 dkist-processing-common-3.0.0rc5/dkist_processing_common/tasks/mixin/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3243 2023-06-21 17:00:55.000000 dkist-processing-common-3.0.0rc5/dkist_processing_common/tasks/mixin/debug_frame.py
--rw-rw-rw-   0 root         (0) root         (0)     2033 2023-06-21 17:00:55.000000 dkist-processing-common-3.0.0rc5/dkist_processing_common/tasks/mixin/fits.py
--rw-rw-rw-   0 root         (0) root         (0)     6887 2023-06-21 17:00:55.000000 dkist-processing-common-3.0.0rc5/dkist_processing_common/tasks/mixin/globus.py
--rw-rw-rw-   0 root         (0) root         (0)     6813 2023-06-21 17:00:55.000000 dkist-processing-common-3.0.0rc5/dkist_processing_common/tasks/mixin/input_dataset.py
--rw-rw-rw-   0 root         (0) root         (0)     2421 2023-06-21 17:00:55.000000 dkist-processing-common-3.0.0rc5/dkist_processing_common/tasks/mixin/interservice_bus.py
--rw-rw-rw-   0 root         (0) root         (0)    13376 2023-06-21 17:00:55.000000 dkist-processing-common-3.0.0rc5/dkist_processing_common/tasks/mixin/metadata_store.py
--rw-rw-rw-   0 root         (0) root         (0)     3612 2023-06-21 17:00:55.000000 dkist-processing-common-3.0.0rc5/dkist_processing_common/tasks/mixin/object_store.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-21 17:01:02.367241 dkist-processing-common-3.0.0rc5/dkist_processing_common/tasks/mixin/quality/
--rw-rw-rw-   0 root         (0) root         (0)      383 2023-06-21 17:00:55.000000 dkist-processing-common-3.0.0rc5/dkist_processing_common/tasks/mixin/quality/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8287 2023-06-21 17:00:55.000000 dkist-processing-common-3.0.0rc5/dkist_processing_common/tasks/mixin/quality/_base.py
--rw-rw-rw-   0 root         (0) root         (0)    47886 2023-06-21 17:00:55.000000 dkist-processing-common-3.0.0rc5/dkist_processing_common/tasks/mixin/quality/_metrics.py
--rw-rw-rw-   0 root         (0) root         (0)     3153 2023-06-21 17:00:55.000000 dkist-processing-common-3.0.0rc5/dkist_processing_common/tasks/output_data_base.py
--rw-rw-rw-   0 root         (0) root         (0)     8329 2023-06-21 17:00:55.000000 dkist-processing-common-3.0.0rc5/dkist_processing_common/tasks/parse_l0_input_data.py
--rw-rw-rw-   0 root         (0) root         (0)     8859 2023-06-21 17:00:55.000000 dkist-processing-common-3.0.0rc5/dkist_processing_common/tasks/quality_metrics.py
--rw-rw-rw-   0 root         (0) root         (0)     2368 2023-06-21 17:00:55.000000 dkist-processing-common-3.0.0rc5/dkist_processing_common/tasks/teardown.py
--rw-rw-rw-   0 root         (0) root         (0)     4863 2023-06-21 17:00:55.000000 dkist-processing-common-3.0.0rc5/dkist_processing_common/tasks/transfer_input_data.py
--rw-rw-rw-   0 root         (0) root         (0)     8475 2023-06-21 17:00:55.000000 dkist-processing-common-3.0.0rc5/dkist_processing_common/tasks/trial_output_data.py
--rw-rw-rw-   0 root         (0) root         (0)    18550 2023-06-21 17:00:55.000000 dkist-processing-common-3.0.0rc5/dkist_processing_common/tasks/write_l1.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-21 17:01:02.371241 dkist-processing-common-3.0.0rc5/dkist_processing_common/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-21 17:00:55.000000 dkist-processing-common-3.0.0rc5/dkist_processing_common/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    24490 2023-06-21 17:00:55.000000 dkist-processing-common-3.0.0rc5/dkist_processing_common/tests/conftest.py
--rw-rw-rw-   0 root         (0) root         (0)     3023 2023-06-21 17:00:55.000000 dkist-processing-common-3.0.0rc5/dkist_processing_common/tests/test_assemble_movie.py
--rw-rw-rw-   0 root         (0) root         (0)     1587 2023-06-21 17:00:55.000000 dkist-processing-common-3.0.0rc5/dkist_processing_common/tests/test_base.py
--rw-rw-rw-   0 root         (0) root         (0)     7501 2023-06-21 17:00:55.000000 dkist-processing-common-3.0.0rc5/dkist_processing_common/tests/test_codecs.py
--rw-rw-rw-   0 root         (0) root         (0)     4203 2023-06-21 17:00:55.000000 dkist-processing-common-3.0.0rc5/dkist_processing_common/tests/test_constants.py
--rw-rw-rw-   0 root         (0) root         (0)     2291 2023-06-21 17:00:55.000000 dkist-processing-common-3.0.0rc5/dkist_processing_common/tests/test_cs_step.py
--rw-rw-rw-   0 root         (0) root         (0)     4097 2023-06-21 17:00:55.000000 dkist-processing-common-3.0.0rc5/dkist_processing_common/tests/test_debug_frame.py
--rw-rw-rw-   0 root         (0) root         (0)      513 2023-06-21 17:00:55.000000 dkist-processing-common-3.0.0rc5/dkist_processing_common/tests/test_dkist_location.py
--rw-rw-rw-   0 root         (0) root         (0)     4682 2023-06-21 17:00:55.000000 dkist-processing-common-3.0.0rc5/dkist_processing_common/tests/test_fits.py
--rw-rw-rw-   0 root         (0) root         (0)     8808 2023-06-21 17:00:55.000000 dkist-processing-common-3.0.0rc5/dkist_processing_common/tests/test_fits_access.py
--rw-rw-rw-   0 root         (0) root         (0)    12959 2023-06-21 17:00:55.000000 dkist-processing-common-3.0.0rc5/dkist_processing_common/tests/test_fits_flowers.py
--rw-rw-rw-   0 root         (0) root         (0)     2258 2023-06-21 17:00:55.000000 dkist-processing-common-3.0.0rc5/dkist_processing_common/tests/test_flower_pot.py
--rw-rw-rw-   0 root         (0) root         (0)    19450 2023-06-21 17:00:55.000000 dkist-processing-common-3.0.0rc5/dkist_processing_common/tests/test_input_dataset.py
--rw-rw-rw-   0 root         (0) root         (0)     3159 2023-06-21 17:00:55.000000 dkist-processing-common-3.0.0rc5/dkist_processing_common/tests/test_output_data_base.py
--rw-rw-rw-   0 root         (0) root         (0)     6276 2023-06-21 17:00:55.000000 dkist-processing-common-3.0.0rc5/dkist_processing_common/tests/test_parameters.py
--rw-rw-rw-   0 root         (0) root         (0)    10476 2023-06-21 17:00:55.000000 dkist-processing-common-3.0.0rc5/dkist_processing_common/tests/test_parse_l0_input_data.py
--rw-rw-rw-   0 root         (0) root         (0)     3198 2023-06-21 17:00:55.000000 dkist-processing-common-3.0.0rc5/dkist_processing_common/tests/test_publish_catalog_messages.py
--rw-rw-rw-   0 root         (0) root         (0)     9168 2023-06-21 17:00:55.000000 dkist-processing-common-3.0.0rc5/dkist_processing_common/tests/test_quality.py
--rw-rw-rw-   0 root         (0) root         (0)    36336 2023-06-21 17:00:55.000000 dkist-processing-common-3.0.0rc5/dkist_processing_common/tests/test_quality_mixin.py
--rw-rw-rw-   0 root         (0) root         (0)    11282 2023-06-21 17:00:55.000000 dkist-processing-common-3.0.0rc5/dkist_processing_common/tests/test_scratch.py
--rw-rw-rw-   0 root         (0) root         (0)     4569 2023-06-21 17:00:55.000000 dkist-processing-common-3.0.0rc5/dkist_processing_common/tests/test_tags.py
--rw-rw-rw-   0 root         (0) root         (0)     5745 2023-06-21 17:00:55.000000 dkist-processing-common-3.0.0rc5/dkist_processing_common/tests/test_teardown.py
--rw-rw-rw-   0 root         (0) root         (0)     6666 2023-06-21 17:00:55.000000 dkist-processing-common-3.0.0rc5/dkist_processing_common/tests/test_transfer_input_data.py
--rw-rw-rw-   0 root         (0) root         (0)     2270 2023-06-21 17:00:55.000000 dkist-processing-common-3.0.0rc5/dkist_processing_common/tests/test_transfer_l1_output_data.py
--rw-rw-rw-   0 root         (0) root         (0)    13679 2023-06-21 17:00:55.000000 dkist-processing-common-3.0.0rc5/dkist_processing_common/tests/test_trial_output_data.py
--rw-rw-rw-   0 root         (0) root         (0)    10527 2023-06-21 17:00:55.000000 dkist-processing-common-3.0.0rc5/dkist_processing_common/tests/test_workflow_task_base.py
--rw-rw-rw-   0 root         (0) root         (0)    14952 2023-06-21 17:00:55.000000 dkist-processing-common-3.0.0rc5/dkist_processing_common/tests/test_write_l1.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-21 17:01:02.359241 dkist-processing-common-3.0.0rc5/dkist_processing_common.egg-info/
--rw-rw-rw-   0 root         (0) root         (0)     4327 2023-06-21 17:01:02.000000 dkist-processing-common-3.0.0rc5/dkist_processing_common.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     4899 2023-06-21 17:01:02.000000 dkist-processing-common-3.0.0rc5/dkist_processing_common.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2023-06-21 17:01:02.000000 dkist-processing-common-3.0.0rc5/dkist_processing_common.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)      603 2023-06-21 17:01:02.000000 dkist-processing-common-3.0.0rc5/dkist_processing_common.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)       24 2023-06-21 17:01:02.000000 dkist-processing-common-3.0.0rc5/dkist_processing_common.egg-info/top_level.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-21 17:01:02.371241 dkist-processing-common-3.0.0rc5/docs/
--rw-rw-rw-   0 root         (0) root         (0)     4598 2023-06-21 17:00:55.000000 dkist-processing-common-3.0.0rc5/docs/Makefile
--rw-rw-rw-   0 root         (0) root         (0)      120 2023-06-21 17:00:55.000000 dkist-processing-common-3.0.0rc5/docs/changelog.rst
--rw-rw-rw-   0 root         (0) root         (0)     1890 2023-06-21 17:00:55.000000 dkist-processing-common-3.0.0rc5/docs/conf.py
--rw-rw-rw-   0 root         (0) root         (0)      113 2023-06-21 17:00:55.000000 dkist-processing-common-3.0.0rc5/docs/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     4513 2023-06-21 17:00:55.000000 dkist-processing-common-3.0.0rc5/docs/make.bat
--rw-rw-rw-   0 root         (0) root         (0)       29 2023-06-21 17:00:55.000000 dkist-processing-common-3.0.0rc5/docs/requirements.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-21 17:01:02.371241 dkist-processing-common-3.0.0rc5/licenses/
--rw-rw-rw-   0 root         (0) root         (0)     1462 2023-06-21 17:00:55.000000 dkist-processing-common-3.0.0rc5/licenses/LICENSE.rst
--rw-rw-rw-   0 root         (0) root         (0)      780 2023-06-21 17:00:55.000000 dkist-processing-common-3.0.0rc5/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)     1690 2023-06-21 17:01:02.371241 dkist-processing-common-3.0.0rc5/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      102 2023-06-21 17:00:55.000000 dkist-processing-common-3.0.0rc5/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-22 20:47:57.832761 dkist-processing-common-3.0.0rc6/
+-rw-rw-rw-   0 root         (0) root         (0)     2481 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      844 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/.pre-commit-config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      429 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/.readthedocs.yml
+-rw-rw-rw-   0 root         (0) root         (0)    13348 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/CHANGELOG.rst
+-rw-rw-rw-   0 root         (0) root         (0)     4327 2023-06-22 20:47:57.832761 dkist-processing-common-3.0.0rc6/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3732 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2433 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/bitbucket-pipelines.yml
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-22 20:47:57.820761 dkist-processing-common-3.0.0rc6/changelog/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/changelog/.gitempty
+-rw-rw-rw-   0 root         (0) root         (0)      149 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/changelog/139.feature.2.rst
+-rw-rw-rw-   0 root         (0) root         (0)       85 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/changelog/139.feature.rst
+-rw-rw-rw-   0 root         (0) root         (0)      342 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/changelog/140.feature.rst
+-rwxrwxrwx   0 root         (0) root         (0)      642 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/check_changelog_updated.sh
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-22 20:47:57.820761 dkist-processing-common-3.0.0rc6/dkist_processing_common/
+-rw-rw-rw-   0 root         (0) root         (0)      317 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/dkist_processing_common/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-22 20:47:57.824761 dkist-processing-common-3.0.0rc6/dkist_processing_common/_util/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/dkist_processing_common/_util/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1572 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/dkist_processing_common/_util/config.py
+-rw-rw-rw-   0 root         (0) root         (0)     2409 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/dkist_processing_common/_util/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)     1178 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/dkist_processing_common/_util/dkist_location.py
+-rw-rw-rw-   0 root         (0) root         (0)     1580 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/dkist_processing_common/_util/graphql.py
+-rw-rw-rw-   0 root         (0) root         (0)     8215 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/dkist_processing_common/_util/scratch.py
+-rw-rw-rw-   0 root         (0) root         (0)     5641 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/dkist_processing_common/_util/tags.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-22 20:47:57.824761 dkist-processing-common-3.0.0rc6/dkist_processing_common/codecs/
+-rw-rw-rw-   0 root         (0) root         (0)      159 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/dkist_processing_common/codecs/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      495 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/dkist_processing_common/codecs/bytes.py
+-rw-rw-rw-   0 root         (0) root         (0)     2030 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/dkist_processing_common/codecs/fits.py
+-rw-rw-rw-   0 root         (0) root         (0)      900 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/dkist_processing_common/codecs/iobase.py
+-rw-rw-rw-   0 root         (0) root         (0)      939 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/dkist_processing_common/codecs/json.py
+-rw-rw-rw-   0 root         (0) root         (0)      197 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/dkist_processing_common/codecs/path.py
+-rw-rw-rw-   0 root         (0) root         (0)      679 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/dkist_processing_common/codecs/str.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-22 20:47:57.824761 dkist-processing-common-3.0.0rc6/dkist_processing_common/fonts/
+-rw-rw-rw-   0 root         (0) root         (0)   656568 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/dkist_processing_common/fonts/Lato-Regular.ttf
+-rw-rw-rw-   0 root         (0) root         (0)      101 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/dkist_processing_common/fonts/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7037 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/dkist_processing_common/manual.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-22 20:47:57.824761 dkist-processing-common-3.0.0rc6/dkist_processing_common/models/
+-rw-rw-rw-   0 root         (0) root         (0)       74 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/dkist_processing_common/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4766 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/dkist_processing_common/models/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)     3453 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/dkist_processing_common/models/fits_access.py
+-rw-rw-rw-   0 root         (0) root         (0)     4176 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/dkist_processing_common/models/flower_pot.py
+-rw-rw-rw-   0 root         (0) root         (0)     3514 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/dkist_processing_common/models/graphql.py
+-rw-rw-rw-   0 root         (0) root         (0)     1109 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/dkist_processing_common/models/message.py
+-rw-rw-rw-   0 root         (0) root         (0)     3408 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/dkist_processing_common/models/parameters.py
+-rw-rw-rw-   0 root         (0) root         (0)     2225 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/dkist_processing_common/models/quality.py
+-rw-rw-rw-   0 root         (0) root         (0)     1096 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/dkist_processing_common/models/quality_json_encoders.py
+-rw-rw-rw-   0 root         (0) root         (0)     7510 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/dkist_processing_common/models/tags.py
+-rw-rw-rw-   0 root         (0) root         (0)      870 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/dkist_processing_common/models/wavelength.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-22 20:47:57.828761 dkist-processing-common-3.0.0rc6/dkist_processing_common/parsers/
+-rw-rw-rw-   0 root         (0) root         (0)       67 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/dkist_processing_common/parsers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6381 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/dkist_processing_common/parsers/cs_step.py
+-rw-rw-rw-   0 root         (0) root         (0)     1827 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/dkist_processing_common/parsers/dsps_repeat.py
+-rw-rw-rw-   0 root         (0) root         (0)      706 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/dkist_processing_common/parsers/experiment_id_bud.py
+-rw-rw-rw-   0 root         (0) root         (0)     1767 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/dkist_processing_common/parsers/id_bud.py
+-rw-rw-rw-   0 root         (0) root         (0)      921 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/dkist_processing_common/parsers/l0_fits_access.py
+-rw-rw-rw-   0 root         (0) root         (0)     2451 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/dkist_processing_common/parsers/l1_fits_access.py
+-rw-rw-rw-   0 root         (0) root         (0)      677 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/dkist_processing_common/parsers/proposal_id_bud.py
+-rw-rw-rw-   0 root         (0) root         (0)     1058 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/dkist_processing_common/parsers/quality.py
+-rw-rw-rw-   0 root         (0) root         (0)     1230 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/dkist_processing_common/parsers/single_value_single_key_flower.py
+-rw-rw-rw-   0 root         (0) root         (0)     5720 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/dkist_processing_common/parsers/time.py
+-rw-rw-rw-   0 root         (0) root         (0)     1669 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/dkist_processing_common/parsers/unique_bud.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-22 20:47:57.828761 dkist-processing-common-3.0.0rc6/dkist_processing_common/tasks/
+-rw-rw-rw-   0 root         (0) root         (0)      504 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/dkist_processing_common/tasks/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11470 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/dkist_processing_common/tasks/assemble_movie.py
+-rw-rw-rw-   0 root         (0) root         (0)    11318 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/dkist_processing_common/tasks/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     8689 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/dkist_processing_common/tasks/l1_output_data.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-22 20:47:57.828761 dkist-processing-common-3.0.0rc6/dkist_processing_common/tasks/mixin/
+-rw-rw-rw-   0 root         (0) root         (0)       68 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/dkist_processing_common/tasks/mixin/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3243 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/dkist_processing_common/tasks/mixin/debug_frame.py
+-rw-rw-rw-   0 root         (0) root         (0)     2033 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/dkist_processing_common/tasks/mixin/fits.py
+-rw-rw-rw-   0 root         (0) root         (0)     6887 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/dkist_processing_common/tasks/mixin/globus.py
+-rw-rw-rw-   0 root         (0) root         (0)     6813 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/dkist_processing_common/tasks/mixin/input_dataset.py
+-rw-rw-rw-   0 root         (0) root         (0)     2421 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/dkist_processing_common/tasks/mixin/interservice_bus.py
+-rw-rw-rw-   0 root         (0) root         (0)    13374 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/dkist_processing_common/tasks/mixin/metadata_store.py
+-rw-rw-rw-   0 root         (0) root         (0)     3612 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/dkist_processing_common/tasks/mixin/object_store.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-22 20:47:57.828761 dkist-processing-common-3.0.0rc6/dkist_processing_common/tasks/mixin/quality/
+-rw-rw-rw-   0 root         (0) root         (0)      383 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/dkist_processing_common/tasks/mixin/quality/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8287 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/dkist_processing_common/tasks/mixin/quality/_base.py
+-rw-rw-rw-   0 root         (0) root         (0)    47886 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/dkist_processing_common/tasks/mixin/quality/_metrics.py
+-rw-rw-rw-   0 root         (0) root         (0)     3153 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/dkist_processing_common/tasks/output_data_base.py
+-rw-rw-rw-   0 root         (0) root         (0)     8329 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/dkist_processing_common/tasks/parse_l0_input_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     8859 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/dkist_processing_common/tasks/quality_metrics.py
+-rw-rw-rw-   0 root         (0) root         (0)     2368 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/dkist_processing_common/tasks/teardown.py
+-rw-rw-rw-   0 root         (0) root         (0)     4863 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/dkist_processing_common/tasks/transfer_input_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     7979 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/dkist_processing_common/tasks/trial_output_data.py
+-rw-rw-rw-   0 root         (0) root         (0)    18550 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/dkist_processing_common/tasks/write_l1.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-22 20:47:57.832761 dkist-processing-common-3.0.0rc6/dkist_processing_common/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/dkist_processing_common/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    24490 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/dkist_processing_common/tests/conftest.py
+-rw-rw-rw-   0 root         (0) root         (0)     3023 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/dkist_processing_common/tests/test_assemble_movie.py
+-rw-rw-rw-   0 root         (0) root         (0)     3060 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/dkist_processing_common/tests/test_base.py
+-rw-rw-rw-   0 root         (0) root         (0)     7501 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/dkist_processing_common/tests/test_codecs.py
+-rw-rw-rw-   0 root         (0) root         (0)     4203 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/dkist_processing_common/tests/test_constants.py
+-rw-rw-rw-   0 root         (0) root         (0)     2291 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/dkist_processing_common/tests/test_cs_step.py
+-rw-rw-rw-   0 root         (0) root         (0)     4097 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/dkist_processing_common/tests/test_debug_frame.py
+-rw-rw-rw-   0 root         (0) root         (0)      513 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/dkist_processing_common/tests/test_dkist_location.py
+-rw-rw-rw-   0 root         (0) root         (0)     4682 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/dkist_processing_common/tests/test_fits.py
+-rw-rw-rw-   0 root         (0) root         (0)     8808 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/dkist_processing_common/tests/test_fits_access.py
+-rw-rw-rw-   0 root         (0) root         (0)    12959 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/dkist_processing_common/tests/test_fits_flowers.py
+-rw-rw-rw-   0 root         (0) root         (0)     2258 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/dkist_processing_common/tests/test_flower_pot.py
+-rw-rw-rw-   0 root         (0) root         (0)    19450 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/dkist_processing_common/tests/test_input_dataset.py
+-rw-rw-rw-   0 root         (0) root         (0)     3159 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/dkist_processing_common/tests/test_output_data_base.py
+-rw-rw-rw-   0 root         (0) root         (0)     6276 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/dkist_processing_common/tests/test_parameters.py
+-rw-rw-rw-   0 root         (0) root         (0)    10476 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/dkist_processing_common/tests/test_parse_l0_input_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     3198 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/dkist_processing_common/tests/test_publish_catalog_messages.py
+-rw-rw-rw-   0 root         (0) root         (0)     9168 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/dkist_processing_common/tests/test_quality.py
+-rw-rw-rw-   0 root         (0) root         (0)    36336 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/dkist_processing_common/tests/test_quality_mixin.py
+-rw-rw-rw-   0 root         (0) root         (0)    11282 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/dkist_processing_common/tests/test_scratch.py
+-rw-rw-rw-   0 root         (0) root         (0)     4569 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/dkist_processing_common/tests/test_tags.py
+-rw-rw-rw-   0 root         (0) root         (0)     5745 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/dkist_processing_common/tests/test_teardown.py
+-rw-rw-rw-   0 root         (0) root         (0)     6666 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/dkist_processing_common/tests/test_transfer_input_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     2270 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/dkist_processing_common/tests/test_transfer_l1_output_data.py
+-rw-rw-rw-   0 root         (0) root         (0)    11883 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/dkist_processing_common/tests/test_trial_output_data.py
+-rw-rw-rw-   0 root         (0) root         (0)    10527 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/dkist_processing_common/tests/test_workflow_task_base.py
+-rw-rw-rw-   0 root         (0) root         (0)    14952 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/dkist_processing_common/tests/test_write_l1.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-22 20:47:57.820761 dkist-processing-common-3.0.0rc6/dkist_processing_common.egg-info/
+-rw-rw-rw-   0 root         (0) root         (0)     4327 2023-06-22 20:47:57.000000 dkist-processing-common-3.0.0rc6/dkist_processing_common.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     4899 2023-06-22 20:47:57.000000 dkist-processing-common-3.0.0rc6/dkist_processing_common.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2023-06-22 20:47:57.000000 dkist-processing-common-3.0.0rc6/dkist_processing_common.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)      603 2023-06-22 20:47:57.000000 dkist-processing-common-3.0.0rc6/dkist_processing_common.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)       24 2023-06-22 20:47:57.000000 dkist-processing-common-3.0.0rc6/dkist_processing_common.egg-info/top_level.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-22 20:47:57.832761 dkist-processing-common-3.0.0rc6/docs/
+-rw-rw-rw-   0 root         (0) root         (0)     4598 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/docs/Makefile
+-rw-rw-rw-   0 root         (0) root         (0)      120 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/docs/changelog.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1890 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/docs/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)      113 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/docs/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     4513 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/docs/make.bat
+-rw-rw-rw-   0 root         (0) root         (0)       29 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/docs/requirements.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-22 20:47:57.832761 dkist-processing-common-3.0.0rc6/licenses/
+-rw-rw-rw-   0 root         (0) root         (0)     1462 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/licenses/LICENSE.rst
+-rw-rw-rw-   0 root         (0) root         (0)      780 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)     1690 2023-06-22 20:47:57.832761 dkist-processing-common-3.0.0rc6/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      102 2023-06-22 20:47:41.000000 dkist-processing-common-3.0.0rc6/setup.py
```

### Comparing `dkist-processing-common-3.0.0rc5/.gitignore` & `dkist-processing-common-3.0.0rc6/.gitignore`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc5/.pre-commit-config.yaml` & `dkist-processing-common-3.0.0rc6/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc5/CHANGELOG.rst` & `dkist-processing-common-3.0.0rc6/CHANGELOG.rst`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc5/PKG-INFO` & `dkist-processing-common-3.0.0rc6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dkist-processing-common
-Version: 3.0.0rc5
+Version: 3.0.0rc6
 Summary: Common task classes used by the DKIST Science Data Processing pipelines to process DKIST data.
 Home-page: https://bitbucket.org/dkistdc/dkist-processing-common/src/master/
 Author: NSO / AURA
 Author-email: "dkistdc@nso.edu"
 License: MIT
 Project-URL: Documentation, https://docs.dkist.nso.edu/projects/common
 Classifier: Programming Language :: Python
```

### Comparing `dkist-processing-common-3.0.0rc5/README.rst` & `dkist-processing-common-3.0.0rc6/README.rst`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc5/bitbucket-pipelines.yml` & `dkist-processing-common-3.0.0rc6/bitbucket-pipelines.yml`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc5/check_changelog_updated.sh` & `dkist-processing-common-3.0.0rc6/check_changelog_updated.sh`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc5/dkist_processing_common/_util/config.py` & `dkist-processing-common-3.0.0rc6/dkist_processing_common/_util/config.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc5/dkist_processing_common/_util/constants.py` & `dkist-processing-common-3.0.0rc6/dkist_processing_common/_util/constants.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc5/dkist_processing_common/_util/dkist_location.py` & `dkist-processing-common-3.0.0rc6/dkist_processing_common/_util/dkist_location.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc5/dkist_processing_common/_util/graphql.py` & `dkist-processing-common-3.0.0rc6/dkist_processing_common/_util/graphql.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc5/dkist_processing_common/_util/scratch.py` & `dkist-processing-common-3.0.0rc6/dkist_processing_common/_util/scratch.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc5/dkist_processing_common/_util/tags.py` & `dkist-processing-common-3.0.0rc6/dkist_processing_common/_util/tags.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc5/dkist_processing_common/codecs/fits.py` & `dkist-processing-common-3.0.0rc6/dkist_processing_common/codecs/fits.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc5/dkist_processing_common/codecs/iobase.py` & `dkist-processing-common-3.0.0rc6/dkist_processing_common/codecs/iobase.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc5/dkist_processing_common/codecs/json.py` & `dkist-processing-common-3.0.0rc6/dkist_processing_common/codecs/json.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc5/dkist_processing_common/codecs/str.py` & `dkist-processing-common-3.0.0rc6/dkist_processing_common/codecs/str.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc5/dkist_processing_common/fonts/Lato-Regular.ttf` & `dkist-processing-common-3.0.0rc6/dkist_processing_common/fonts/Lato-Regular.ttf`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc5/dkist_processing_common/manual.py` & `dkist-processing-common-3.0.0rc6/dkist_processing_common/manual.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc5/dkist_processing_common/models/constants.py` & `dkist-processing-common-3.0.0rc6/dkist_processing_common/models/constants.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc5/dkist_processing_common/models/fits_access.py` & `dkist-processing-common-3.0.0rc6/dkist_processing_common/models/fits_access.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc5/dkist_processing_common/models/flower_pot.py` & `dkist-processing-common-3.0.0rc6/dkist_processing_common/models/flower_pot.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc5/dkist_processing_common/models/graphql.py` & `dkist-processing-common-3.0.0rc6/dkist_processing_common/models/graphql.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc5/dkist_processing_common/models/message.py` & `dkist-processing-common-3.0.0rc6/dkist_processing_common/models/message.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc5/dkist_processing_common/models/parameters.py` & `dkist-processing-common-3.0.0rc6/dkist_processing_common/models/parameters.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc5/dkist_processing_common/models/quality.py` & `dkist-processing-common-3.0.0rc6/dkist_processing_common/models/quality.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc5/dkist_processing_common/models/quality_json_encoders.py` & `dkist-processing-common-3.0.0rc6/dkist_processing_common/models/quality_json_encoders.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc5/dkist_processing_common/models/tags.py` & `dkist-processing-common-3.0.0rc6/dkist_processing_common/models/tags.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc5/dkist_processing_common/models/wavelength.py` & `dkist-processing-common-3.0.0rc6/dkist_processing_common/models/wavelength.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc5/dkist_processing_common/parsers/cs_step.py` & `dkist-processing-common-3.0.0rc6/dkist_processing_common/parsers/cs_step.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc5/dkist_processing_common/parsers/dsps_repeat.py` & `dkist-processing-common-3.0.0rc6/dkist_processing_common/parsers/dsps_repeat.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc5/dkist_processing_common/parsers/experiment_id_bud.py` & `dkist-processing-common-3.0.0rc6/dkist_processing_common/parsers/experiment_id_bud.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc5/dkist_processing_common/parsers/id_bud.py` & `dkist-processing-common-3.0.0rc6/dkist_processing_common/parsers/id_bud.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc5/dkist_processing_common/parsers/l0_fits_access.py` & `dkist-processing-common-3.0.0rc6/dkist_processing_common/parsers/l0_fits_access.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc5/dkist_processing_common/parsers/l1_fits_access.py` & `dkist-processing-common-3.0.0rc6/dkist_processing_common/parsers/l1_fits_access.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc5/dkist_processing_common/parsers/proposal_id_bud.py` & `dkist-processing-common-3.0.0rc6/dkist_processing_common/parsers/proposal_id_bud.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc5/dkist_processing_common/parsers/quality.py` & `dkist-processing-common-3.0.0rc6/dkist_processing_common/parsers/quality.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc5/dkist_processing_common/parsers/single_value_single_key_flower.py` & `dkist-processing-common-3.0.0rc6/dkist_processing_common/parsers/single_value_single_key_flower.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc5/dkist_processing_common/parsers/time.py` & `dkist-processing-common-3.0.0rc6/dkist_processing_common/parsers/time.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc5/dkist_processing_common/parsers/unique_bud.py` & `dkist-processing-common-3.0.0rc6/dkist_processing_common/parsers/unique_bud.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc5/dkist_processing_common/tasks/assemble_movie.py` & `dkist-processing-common-3.0.0rc6/dkist_processing_common/tasks/assemble_movie.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc5/dkist_processing_common/tasks/base.py` & `dkist-processing-common-3.0.0rc6/dkist_processing_common/tasks/base.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 """Wrappers for all workflow tasks."""
 import json
 import logging
 from abc import ABC
-from io import BytesIO
 from pathlib import Path
 from typing import Any
 from typing import Generator
 from typing import Iterable
 from typing import Type
 from uuid import uuid4
 
@@ -14,14 +13,15 @@
 from dkist_processing_core import TaskBase
 
 from dkist_processing_common._util.config import get_config
 from dkist_processing_common._util.scratch import WorkflowFileSystem
 from dkist_processing_common.codecs.bytes import bytes_encoder
 from dkist_processing_common.codecs.path import path_decoder
 from dkist_processing_common.models.constants import ConstantsBase
+from dkist_processing_common.models.tags import StemName
 from dkist_processing_common.tasks.mixin.metadata_store import MetadataStoreMixin
 
 __all__ = ["WorkflowTaskBase", "tag_type_hint"]
 
 logger = logging.getLogger(__name__)
 
 tag_type_hint = Iterable[str] | str
@@ -204,21 +204,81 @@
 
         Returns
         -------
         The path for the written file
         """
         file_obj = encoder(data, **encoder_kwargs)
         tags = self._parse_tags(tags)
-        relative_path = relative_path or f"{uuid4().hex}.dat"
+        relative_path = relative_path or self._build_generic_tag_filename(tags)
         relative_path = Path(relative_path)
         self.scratch.write(
             file_obj=file_obj, relative_path=relative_path, tags=tags, overwrite=overwrite
         )
         return relative_path
 
+    @property
+    def filename_tag_order(self) -> list[str]:
+        """
+        Order of tags to consider when constructing a filename.
+
+        This list does NOT need to contain *all* possible tags, just the ones for which we care about the order.
+        """
+        return [
+            StemName.debug.value,
+            StemName.input.value,
+            StemName.intermediate.value,
+            StemName.calibrated.value,
+            StemName.output.value,
+            StemName.task.value,
+            StemName.dsps_repeat.value,
+            StemName.cs_step.value,
+            StemName.modstate.value,
+        ]
+
+    def _build_generic_tag_filename(self, tags: Iterable[str]) -> str:
+        """
+        Build a filename from a set of tags.
+
+        The algorithm is:
+
+         1. Any tag Stems that appear in `self.filename_tag_order` will be joined, in order, along with their values
+            (if applicable).
+
+         2. Any remaining tags not in `self.filename_tag_order` are sorted alphabetically and joined to the end of the
+            filename.
+
+         3. A random set of 6 characters is appened to avoid any collisions on files that have the same set of tags.
+
+         4. You can have any extension you want so long as it's ".dat".
+        """
+        # This call to list not only copies the input object so it doesn't get modified in place, it also ensures
+        # any Iterable that got passed in is a list inside the function.
+        copied_tags = list(tags)
+        try:
+            copied_tags.remove(StemName.frame.value)
+        except ValueError:
+            # Not a frame. This is fine.
+            pass
+
+        filename_parts = []
+        for ordered_tag in self.filename_tag_order:
+            tags_with_stem = filter(lambda t: ordered_tag in t, copied_tags)
+            for tag in tags_with_stem:
+                filename_parts.append(tag)
+                copied_tags.remove(tag)
+
+        sorted_remaining_tags = sorted(copied_tags)
+        filename_parts += sorted_remaining_tags
+
+        dash_separated_parts = [t.replace("_", "-") for t in filename_parts]
+
+        base_filename = "_".join(dash_separated_parts)
+
+        return base_filename + "_" + uuid4().hex[:6] + ".dat"
+
     def count(self, tags: tag_type_hint) -> int:
         """
         Return the number of objects tagged with the given tags.
 
         Parameters
         ----------
         tags
```

### Comparing `dkist-processing-common-3.0.0rc5/dkist_processing_common/tasks/l1_output_data.py` & `dkist-processing-common-3.0.0rc6/dkist_processing_common/tasks/l1_output_data.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc5/dkist_processing_common/tasks/mixin/debug_frame.py` & `dkist-processing-common-3.0.0rc6/dkist_processing_common/tasks/mixin/debug_frame.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc5/dkist_processing_common/tasks/mixin/fits.py` & `dkist-processing-common-3.0.0rc6/dkist_processing_common/tasks/mixin/fits.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc5/dkist_processing_common/tasks/mixin/globus.py` & `dkist-processing-common-3.0.0rc6/dkist_processing_common/tasks/mixin/globus.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc5/dkist_processing_common/tasks/mixin/input_dataset.py` & `dkist-processing-common-3.0.0rc6/dkist_processing_common/tasks/mixin/input_dataset.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc5/dkist_processing_common/tasks/mixin/interservice_bus.py` & `dkist-processing-common-3.0.0rc6/dkist_processing_common/tasks/mixin/interservice_bus.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc5/dkist_processing_common/tasks/mixin/metadata_store.py` & `dkist-processing-common-3.0.0rc6/dkist_processing_common/tasks/mixin/metadata_store.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,15 +41,15 @@
         self._metadata_store_change_status(status="INPROGRESS", is_complete=False)
 
     def metadata_store_change_recipe_run_to_completed_successfully(self):
         """Set the recipe run status to "COMPLETEDSUCCESSFULLY"."""
         self._metadata_store_change_status(status="COMPLETEDSUCCESSFULLY", is_complete=True)
 
     def metadata_store_change_recipe_run_to_trial_success(self):
-        """Set the recipe run status to "TRIALCOMPLETED"."""
+        """Set the recipe run status to "TRIALSUCCESS"."""
         self._metadata_store_change_status(status="TRIALSUCCESS", is_complete=False)
 
     def metadata_store_add_dataset_receipt_account(
         self, dataset_id: str, expected_object_count: int
     ):
         """Set the number of expected objects."""
         self.metadata_store_client.execute_gql_mutation(
```

### Comparing `dkist-processing-common-3.0.0rc5/dkist_processing_common/tasks/mixin/object_store.py` & `dkist-processing-common-3.0.0rc6/dkist_processing_common/tasks/mixin/object_store.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc5/dkist_processing_common/tasks/mixin/quality/_base.py` & `dkist-processing-common-3.0.0rc6/dkist_processing_common/tasks/mixin/quality/_base.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc5/dkist_processing_common/tasks/mixin/quality/_metrics.py` & `dkist-processing-common-3.0.0rc6/dkist_processing_common/tasks/mixin/quality/_metrics.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc5/dkist_processing_common/tasks/output_data_base.py` & `dkist-processing-common-3.0.0rc6/dkist_processing_common/tasks/output_data_base.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc5/dkist_processing_common/tasks/parse_l0_input_data.py` & `dkist-processing-common-3.0.0rc6/dkist_processing_common/tasks/parse_l0_input_data.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc5/dkist_processing_common/tasks/quality_metrics.py` & `dkist-processing-common-3.0.0rc6/dkist_processing_common/tasks/quality_metrics.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc5/dkist_processing_common/tasks/teardown.py` & `dkist-processing-common-3.0.0rc6/dkist_processing_common/tasks/teardown.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc5/dkist_processing_common/tasks/transfer_input_data.py` & `dkist-processing-common-3.0.0rc6/dkist_processing_common/tasks/transfer_input_data.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc5/dkist_processing_common/tasks/trial_output_data.py` & `dkist-processing-common-3.0.0rc6/dkist_processing_common/tasks/trial_output_data.py`

 * *Files 8% similar despite different names*

```diff
@@ -45,36 +45,60 @@
 
     @property
     def destination_root_folder(self) -> Path:
         """Format the destination root folder with a value that can be set in the recipe run configuration."""
         root_name_from_configuration = self.metadata_store_recipe_run_configuration().get(
             "trial_root_directory_name"
         )
-        root_name = root_name_from_configuration or super().destination_root_folder
-        if isinstance(root_name, str):
-            root_name = Path(root_name)
+        root_name = Path(root_name_from_configuration or super().destination_root_folder)
 
         return root_name
 
     @property
     def destination_folder(self) -> Path:
         """Format the destination folder with a parent that can be set by the recipe run configuration."""
         dir_name = self.metadata_store_recipe_run_configuration().get(
             "trial_directory_name"
         ) or Path(self.constants.dataset_id)
         return self.destination_root_folder / dir_name
 
+    @property
+    def debug_frame_switch(self) -> bool:
+        """Switch to turn on/off the transfer of DEBUG frames to the trial location."""
+        return self.metadata_store_recipe_run_configuration().get(
+            "trial_transfer_debug_frames", True
+        )
+
+    @property
+    def intermediate_frame_switch(self) -> bool:
+        """Switch to turn on/off the transfer of INTERMEDIATE frames to the trial location."""
+        return self.metadata_store_recipe_run_configuration().get(
+            "trial_transfer_intermediate_frames", True
+        )
+
+    @property
+    def output_frame_switch(self) -> bool:
+        """Switch to turn on/off the transfer of OUTPUT frames to the trial location."""
+        return self.metadata_store_recipe_run_configuration().get(
+            "trial_transfer_output_frames", True
+        )
+
+    @property
+    def specific_frame_tag_lists(self) -> list:
+        """Return list of tag lists that define specific files we want to transfer to the trial location."""
+        return self.metadata_store_recipe_run_configuration().get("trial_transfer_tag_lists", [])
+
     @abstractmethod
     def build_transfer_list(self) -> list[GlobusTransferItem]:
         """Build a list of all items on scratch to transfer to the trial location."""
         pass
 
     def build_debug_frame_transfer_list(self) -> list[GlobusTransferItem]:
         """Build a transfer list containing all frames tagged with DEBUG."""
-        debug_frame_paths: list[Path] = list(self.read(tags=[Tag.debug(), Tag.frame()]))
+        debug_frame_paths = self.read(tags=[Tag.debug(), Tag.frame()])
         transfer_items = []
         for p in debug_frame_paths:
             object_key = self.format_object_key(p)
             destination_path = Path(self.destination_bucket, object_key)
             item = GlobusTransferItem(
                 source_path=p,
                 destination_path=destination_path,
@@ -101,48 +125,27 @@
                 transfer_items.extend(self._build_single_task_intermediate_manifest(task=task))
 
         return transfer_items
 
     def _build_single_task_intermediate_manifest(self, task: str) -> list[GlobusTransferItem]:
         """Build a transfer list containing all frames tagged with INTERMEDIATE and the given TASK."""
         transfer_items = []
-        dark_frames = self.read(tags=[Tag.intermediate(), Tag.task(task)])
+        task_frames = self.read(tags=[Tag.intermediate(), Tag.task(task)])
 
-        for p in dark_frames:
-            tags = self.tags(p)
-            output_name = Path(self._construct_intermediate_name_from_tags(tags, task))
-            destination_object_key = self.format_object_key(output_name)
+        for p in task_frames:
+            destination_object_key = self.format_object_key(p)
             destination_path = Path(self.destination_bucket, destination_object_key)
             item = GlobusTransferItem(
                 source_path=p,
                 destination_path=destination_path,
             )
             transfer_items.append(item)
 
         return transfer_items
 
-    def _construct_intermediate_name_from_tags(self, tags: list, task: str) -> str:
-        """
-        Build a sensible filename from a list of tags on an INTERMEDIATE frame with a specific TASK.
-
-        The name will be `f"INTERMEDIATE_TASK-{task}_[{TAG_STEM}-{TAG_VALUE}, ...].dat"`
-        """
-        name_parts = []
-        for t in tags:
-            if t in [Tag.frame(), Tag.intermediate(), Tag.task(task)]:
-                continue
-
-            name_parts.append(t.replace("_", "-"))
-
-        name_parts.sort()
-
-        tag_name = "_".join(name_parts)
-
-        return f"INTERMEDIATE_TASK-{task}_" + tag_name + ".dat"
-
     def build_transfer_list_from_tag_lists(
         self, tag_lists: list[str] | list[list[str]]
     ) -> list[GlobusTransferItem]:
         """
         Build a transfer list containing all files that are tagged with any of the sets of input tags.
 
         For example, if `tag_lists` is [list1, list2,... listn] then the resulting transfer list will contain:
@@ -162,46 +165,24 @@
             tag_lists = [tag_lists]
 
         transfer_items = []
         for tag_set in tag_lists:
 
             paths = self.read(tags=tag_set)
             for p in paths:
-                tags = self.tags(p)
-                output_name = Path(self._construct_generic_name_from_tags(tags))
-                destination_object_key = self.format_object_key(output_name)
+                destination_object_key = self.format_object_key(p)
                 destination_path = Path(self.destination_bucket, destination_object_key)
                 item = GlobusTransferItem(
                     source_path=p,
                     destination_path=destination_path,
                 )
                 transfer_items.append(item)
 
         return list(set(transfer_items))
 
-    def _construct_generic_name_from_tags(self, tags: list[str]) -> str:
-        """
-        Build a sensible filename from an arbitrary set of tags.
-
-        Unlike `_construct_intermediate_name_from_tags` this method doesn't assign any weighting for readability to the
-        input tags. The result is simply `[{TAG_STEM}-{TAG_VALUE}, ...].dat"`.
-        """
-        name_parts = []
-        for t in tags:
-            if t in [Tag.frame()]:
-                continue
-
-            name_parts.append(t.replace("_", "-"))
-
-        name_parts.sort()
-
-        tag_name = "_".join(name_parts)
-
-        return tag_name + ".dat"
-
     def transfer_all_trial_frames(self, transfer_items: list[GlobusTransferItem]) -> None:
         """Send a list of transfer items to Globus for transfer."""
         logger.info(
             f"Preparing globus transfer {len(transfer_items)} items: "
             f"recipe_run_id={self.recipe_run_id}. "
             f"transfer_items={transfer_items[:3]}..."
         )
```

### Comparing `dkist-processing-common-3.0.0rc5/dkist_processing_common/tasks/write_l1.py` & `dkist-processing-common-3.0.0rc6/dkist_processing_common/tasks/write_l1.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc5/dkist_processing_common/tests/conftest.py` & `dkist-processing-common-3.0.0rc6/dkist_processing_common/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc5/dkist_processing_common/tests/test_assemble_movie.py` & `dkist-processing-common-3.0.0rc6/dkist_processing_common/tests/test_assemble_movie.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc5/dkist_processing_common/tests/test_codecs.py` & `dkist-processing-common-3.0.0rc6/dkist_processing_common/tests/test_codecs.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc5/dkist_processing_common/tests/test_constants.py` & `dkist-processing-common-3.0.0rc6/dkist_processing_common/tests/test_constants.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc5/dkist_processing_common/tests/test_cs_step.py` & `dkist-processing-common-3.0.0rc6/dkist_processing_common/tests/test_cs_step.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc5/dkist_processing_common/tests/test_debug_frame.py` & `dkist-processing-common-3.0.0rc6/dkist_processing_common/tests/test_debug_frame.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc5/dkist_processing_common/tests/test_dkist_location.py` & `dkist-processing-common-3.0.0rc6/dkist_processing_common/tests/test_dkist_location.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc5/dkist_processing_common/tests/test_fits.py` & `dkist-processing-common-3.0.0rc6/dkist_processing_common/tests/test_fits.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc5/dkist_processing_common/tests/test_fits_access.py` & `dkist-processing-common-3.0.0rc6/dkist_processing_common/tests/test_fits_access.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc5/dkist_processing_common/tests/test_fits_flowers.py` & `dkist-processing-common-3.0.0rc6/dkist_processing_common/tests/test_fits_flowers.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc5/dkist_processing_common/tests/test_flower_pot.py` & `dkist-processing-common-3.0.0rc6/dkist_processing_common/tests/test_flower_pot.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc5/dkist_processing_common/tests/test_input_dataset.py` & `dkist-processing-common-3.0.0rc6/dkist_processing_common/tests/test_input_dataset.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc5/dkist_processing_common/tests/test_output_data_base.py` & `dkist-processing-common-3.0.0rc6/dkist_processing_common/tests/test_output_data_base.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc5/dkist_processing_common/tests/test_parameters.py` & `dkist-processing-common-3.0.0rc6/dkist_processing_common/tests/test_parameters.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc5/dkist_processing_common/tests/test_parse_l0_input_data.py` & `dkist-processing-common-3.0.0rc6/dkist_processing_common/tests/test_parse_l0_input_data.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc5/dkist_processing_common/tests/test_publish_catalog_messages.py` & `dkist-processing-common-3.0.0rc6/dkist_processing_common/tests/test_publish_catalog_messages.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc5/dkist_processing_common/tests/test_quality.py` & `dkist-processing-common-3.0.0rc6/dkist_processing_common/tests/test_quality.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc5/dkist_processing_common/tests/test_quality_mixin.py` & `dkist-processing-common-3.0.0rc6/dkist_processing_common/tests/test_quality_mixin.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc5/dkist_processing_common/tests/test_scratch.py` & `dkist-processing-common-3.0.0rc6/dkist_processing_common/tests/test_scratch.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc5/dkist_processing_common/tests/test_tags.py` & `dkist-processing-common-3.0.0rc6/dkist_processing_common/tests/test_tags.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc5/dkist_processing_common/tests/test_teardown.py` & `dkist-processing-common-3.0.0rc6/dkist_processing_common/tests/test_teardown.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc5/dkist_processing_common/tests/test_transfer_input_data.py` & `dkist-processing-common-3.0.0rc6/dkist_processing_common/tests/test_transfer_input_data.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc5/dkist_processing_common/tests/test_transfer_l1_output_data.py` & `dkist-processing-common-3.0.0rc6/dkist_processing_common/tests/test_transfer_l1_output_data.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc5/dkist_processing_common/tests/test_trial_output_data.py` & `dkist-processing-common-3.0.0rc6/dkist_processing_common/tests/test_trial_output_data.py`

 * *Files 20% similar despite different names*

```diff
@@ -157,53 +157,14 @@
         Path(expected_root_name, expected_dir_name, filename)
     )
 
 
 @pytest.mark.parametrize(
     "custom_root_name, custom_dir_name", [pytest.param(None, None, id="Default trial dir name")]
 )
-def test_construct_intermediate_name_from_tags(basic_trial_output_task):
-    """
-    Given: A base task from TransferTrialDataBase
-    When: Formatting a sensible name for an INTERMEDIATE tag
-    Then: The correct name is returned
-    """
-    task, _ = basic_trial_output_task
-    tags = [Tag.frame(), Tag.intermediate(), Tag.movie(), Tag.modstate(4), Tag.task("FOO")]
-    expected_name = "INTERMEDIATE_TASK-FOO_MODSTATE-4_MOVIE.dat"
-
-    assert task._construct_intermediate_name_from_tags(tags, task="FOO") == expected_name
-
-
-@pytest.mark.parametrize(
-    "custom_root_name, custom_dir_name", [pytest.param(None, None, id="Default trial dir name")]
-)
-def test_construct_generic_name_from_tags(basic_trial_output_task):
-    """
-    Given: A base task from TransferTrialDataBase
-    When: Formatting a sensible name for an arbitrary file
-    Then: The correct name is returned
-    """
-    task, _ = basic_trial_output_task
-    tags = [
-        Tag.frame(),
-        Tag.debug(),
-        Tag.intermediate(),
-        Tag.movie(),
-        Tag.modstate(4),
-        Tag.task("FOO"),
-    ]
-    expected_name = "DEBUG_INTERMEDIATE_MODSTATE-4_MOVIE_TASK-FOO.dat"
-
-    assert task._construct_generic_name_from_tags(tags) == expected_name
-
-
-@pytest.mark.parametrize(
-    "custom_root_name, custom_dir_name", [pytest.param(None, None, id="Default trial dir name")]
-)
 def test_build_transfer_list(complete_trial_output_task, dummy_globus_transfer_item):
     """
     Given: A Task based on TransferTrialDataBase with a defined build_transfer_list
     When: Building the full transfer list
     Then: The expected transfer list is returned
     """
     task, *_ = complete_trial_output_task
@@ -247,17 +208,15 @@
     Given: A Task based on TransferTrialDataBase with tagged INTERMEDIATE frames
     When: Building the intermediate transfer list
     Then: The resulting transfer list has the correct source and destination paths and references the correct frames
     """
     task, proposal_id, _, intermediate_file_obj, _ = complete_trial_output_task
 
     transfer_list = task.build_intermediate_frame_transfer_list()
-    expected_destination_name = task._construct_intermediate_name_from_tags(
-        tags=[Tag.intermediate(), Tag.frame(), Tag.task("FOO")], task="FOO"
-    )
+    expected_destination_name = "intermediate.ext"
     expected_destination_path = Path(
         destination_bucket, task.format_object_key(Path(expected_destination_name))
     )
 
     assert len(transfer_list) == 1
     transfer_item = transfer_list[0]
     assert transfer_item.source_path == task.scratch.workflow_base_path / "intermediate.ext"
@@ -292,43 +251,37 @@
     assert len(transfer_list) == 3
     sorted_transfer_list = sorted(transfer_list, key=lambda x: x.source_path.name)
 
     # This whole structure is nasty. I'm sorry
 
     # Debug frame
     transfer_item = sorted_transfer_list[0]
-    expected_destination_name = task._construct_generic_name_from_tags(
-        tags=[Tag.debug(), Tag.frame()]
-    )
+    expected_destination_name = "debug.ext"
     expected_destination_path = Path(
         destination_bucket, task.format_object_key(Path(expected_destination_name))
     )
     assert transfer_item.source_path == task.scratch.workflow_base_path / "debug.ext"
     assert transfer_item.destination_path == expected_destination_path
     with transfer_item.source_path.open(mode="rb") as f:
         assert debug_file_obj == f.read()
 
     # Intermediate frame 1
     transfer_item = sorted_transfer_list[1]
-    expected_destination_name = task._construct_generic_name_from_tags(
-        tags=[Tag.intermediate(), Tag.frame(), Tag.task("FOO")]
-    )
+    expected_destination_name = "intermediate.ext"
     expected_destination_path = Path(
         destination_bucket, task.format_object_key(Path(expected_destination_name))
     )
     assert transfer_item.source_path == task.scratch.workflow_base_path / "intermediate.ext"
     assert transfer_item.destination_path == expected_destination_path
     with transfer_item.source_path.open(mode="rb") as f:
         assert intermediate_file_obj == f.read()
 
     # Intermediate frame 2
     transfer_item = sorted_transfer_list[2]
-    expected_destination_name = task._construct_generic_name_from_tags(
-        tags=[Tag.intermediate(), Tag.frame(), Tag.task("WHO_CARES")]
-    )
+    expected_destination_name = "something_else.ext"
     expected_destination_path = Path(
         destination_bucket, task.format_object_key(Path(expected_destination_name))
     )
     assert transfer_item.source_path == task.scratch.workflow_base_path / "something_else.ext"
     assert transfer_item.destination_path == expected_destination_path
     with transfer_item.source_path.open(mode="rb") as f:
         assert intermediate_file_obj_2 == f.read()
@@ -349,17 +302,15 @@
 
     tag_list = [Tag.debug()]
 
     transfer_list = task.build_transfer_list_from_tag_lists(tag_list)
 
     assert len(transfer_list) == 1
     transfer_item = transfer_list[0]
-    expected_destination_name = task._construct_generic_name_from_tags(
-        tags=[Tag.debug(), Tag.frame()]
-    )
+    expected_destination_name = "debug.ext"
     expected_destination_path = Path(
         destination_bucket, task.format_object_key(Path(expected_destination_name))
     )
     assert transfer_item.source_path == task.scratch.workflow_base_path / "debug.ext"
     assert transfer_item.destination_path == expected_destination_path
     with transfer_item.source_path.open(mode="rb") as f:
         assert debug_file_obj == f.read()
```

### Comparing `dkist-processing-common-3.0.0rc5/dkist_processing_common/tests/test_workflow_task_base.py` & `dkist-processing-common-3.0.0rc6/dkist_processing_common/tests/test_workflow_task_base.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc5/dkist_processing_common/tests/test_write_l1.py` & `dkist-processing-common-3.0.0rc6/dkist_processing_common/tests/test_write_l1.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc5/dkist_processing_common.egg-info/PKG-INFO` & `dkist-processing-common-3.0.0rc6/dkist_processing_common.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dkist-processing-common
-Version: 3.0.0rc5
+Version: 3.0.0rc6
 Summary: Common task classes used by the DKIST Science Data Processing pipelines to process DKIST data.
 Home-page: https://bitbucket.org/dkistdc/dkist-processing-common/src/master/
 Author: NSO / AURA
 Author-email: "dkistdc@nso.edu"
 License: MIT
 Project-URL: Documentation, https://docs.dkist.nso.edu/projects/common
 Classifier: Programming Language :: Python
```

### Comparing `dkist-processing-common-3.0.0rc5/dkist_processing_common.egg-info/SOURCES.txt` & `dkist-processing-common-3.0.0rc6/dkist_processing_common.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc5/dkist_processing_common.egg-info/requires.txt` & `dkist-processing-common-3.0.0rc6/dkist_processing_common.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc5/docs/Makefile` & `dkist-processing-common-3.0.0rc6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc5/docs/conf.py` & `dkist-processing-common-3.0.0rc6/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc5/docs/make.bat` & `dkist-processing-common-3.0.0rc6/docs/make.bat`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc5/licenses/LICENSE.rst` & `dkist-processing-common-3.0.0rc6/licenses/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc5/pyproject.toml` & `dkist-processing-common-3.0.0rc6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc5/setup.cfg` & `dkist-processing-common-3.0.0rc6/setup.cfg`

 * *Files identical despite different names*

