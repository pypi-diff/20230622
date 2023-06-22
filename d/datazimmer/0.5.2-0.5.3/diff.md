# Comparing `tmp/datazimmer-0.5.2.tar.gz` & `tmp/datazimmer-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datazimmer-0.5.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "datazimmer-0.5.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `datazimmer-0.5.2.tar` & `datazimmer-0.5.3.tar`

### file list

```diff
@@ -1,149 +1,150 @@
--rw-r--r--   0        0        0     1003 2023-06-19 14:24:46.688842 datazimmer-0.5.2/.github/workflows/compatibility_test.yml
--rw-r--r--   0        0        0     1299 2023-06-19 14:24:46.688842 datazimmer-0.5.2/.github/workflows/test.yml
--rw-r--r--   0        0        0      565 2023-06-19 14:24:46.688842 datazimmer-0.5.2/.github/workflows/twine_release.yml
--rw-r--r--   0        0        0     1795 2023-06-19 14:24:46.688842 datazimmer-0.5.2/.gitignore
--rw-r--r--   0        0        0      288 2023-06-19 14:24:46.688842 datazimmer-0.5.2/.readthedocs.yml
--rw-r--r--   0        0        0      491 2023-06-19 14:24:46.688842 datazimmer-0.5.2/CITATION.cff
--rw-r--r--   0        0        0     1077 2023-06-19 14:24:46.688842 datazimmer-0.5.2/LICENSE
--rw-r--r--   0        0        0     3122 2023-06-19 14:24:46.692842 datazimmer-0.5.2/README.md
--rw-r--r--   0        0        0     4074 2023-06-19 14:24:46.692842 datazimmer-0.5.2/conftest.py
--rw-r--r--   0        0        0      634 2023-06-19 14:24:46.692842 datazimmer-0.5.2/datazimmer/__init__.py
--rw-r--r--   0        0        0     2962 2023-06-19 14:24:46.692842 datazimmer-0.5.2/datazimmer/aswan_integration.py
--rw-r--r--   0        0        0     7923 2023-06-19 14:24:46.692842 datazimmer-0.5.2/datazimmer/config_loading.py
--rw-r--r--   0        0        0     2112 2023-06-19 14:24:46.692842 datazimmer-0.5.2/datazimmer/dvc_util.py
--rw-r--r--   0        0        0      144 2023-06-19 14:24:46.692842 datazimmer-0.5.2/datazimmer/exceptions.py
--rw-r--r--   0        0        0      624 2023-06-19 14:24:46.692842 datazimmer-0.5.2/datazimmer/get_runtime.py
--rw-r--r--   0        0        0     2434 2023-06-19 14:24:46.692842 datazimmer-0.5.2/datazimmer/gh_actions.py
--rw-r--r--   0        0        0        0 2023-06-19 14:24:46.692842 datazimmer-0.5.2/datazimmer/metadata/__init__.py
--rw-r--r--   0        0        0     6235 2023-06-19 14:24:46.692842 datazimmer-0.5.2/datazimmer/metadata/atoms.py
--rw-r--r--   0        0        0     1422 2023-06-19 14:24:46.692842 datazimmer-0.5.2/datazimmer/metadata/complete_id.py
--rw-r--r--   0        0        0     1744 2023-06-19 14:24:46.692842 datazimmer-0.5.2/datazimmer/metadata/datascript.py
--rw-r--r--   0        0        0     4537 2023-06-19 14:24:46.692842 datazimmer-0.5.2/datazimmer/metadata/high_level.py
--rw-r--r--   0        0        0     4798 2023-06-19 14:24:46.692842 datazimmer-0.5.2/datazimmer/metadata/scrutable.py
--rw-r--r--   0        0        0     3456 2023-06-19 14:24:46.692842 datazimmer-0.5.2/datazimmer/naming.py
--rw-r--r--   0        0        0      526 2023-06-19 14:24:46.692842 datazimmer-0.5.2/datazimmer/persistent_state.py
--rw-r--r--   0        0        0     8463 2023-06-19 14:24:46.692842 datazimmer-0.5.2/datazimmer/pipeline_element.py
--rw-r--r--   0        0        0     7648 2023-06-19 14:24:46.692842 datazimmer-0.5.2/datazimmer/project_runtime.py
--rw-r--r--   0        0        0      935 2023-06-19 14:24:46.692842 datazimmer-0.5.2/datazimmer/raw_data.py
--rw-r--r--   0        0        0     6235 2023-06-19 14:24:46.692842 datazimmer-0.5.2/datazimmer/registry.py
--rw-r--r--   0        0        0      863 2023-06-19 14:24:46.692842 datazimmer-0.5.2/datazimmer/reporting.py
--rw-r--r--   0        0        0        0 2023-06-19 14:24:46.692842 datazimmer-0.5.2/datazimmer/sql/__init__.py
--rw-r--r--   0        0        0       87 2023-06-19 14:24:46.692842 datazimmer-0.5.2/datazimmer/sql/draw.py
--rw-r--r--   0        0        0     7107 2023-06-19 14:24:46.692842 datazimmer-0.5.2/datazimmer/sql/loader.py
--rw-r--r--   0        0        0        0 2023-06-19 14:24:46.692842 datazimmer-0.5.2/datazimmer/tests/__init__.py
--rw-r--r--   0        0        0     4692 2023-06-19 14:24:46.692842 datazimmer-0.5.2/datazimmer/tests/create_dogshow.py
--rw-r--r--   0        0        0      845 2023-06-19 14:24:46.692842 datazimmer-0.5.2/datazimmer/tests/test_commands.py
--rw-r--r--   0        0        0      346 2023-06-19 14:24:46.692842 datazimmer-0.5.2/datazimmer/tests/test_config.py
--rw-r--r--   0        0        0     4366 2023-06-19 14:24:46.692842 datazimmer-0.5.2/datazimmer/tests/test_full_integration.py
--rw-r--r--   0        0        0      465 2023-06-19 14:24:46.692842 datazimmer-0.5.2/datazimmer/tests/test_registry.py
--rw-r--r--   0        0        0      294 2023-06-19 14:24:46.692842 datazimmer-0.5.2/datazimmer/tests/test_runtime.py
--rw-r--r--   0        0        0     1799 2023-06-19 14:24:46.692842 datazimmer-0.5.2/datazimmer/tests/test_scrutable.py
--rw-r--r--   0        0        0      152 2023-06-19 14:24:46.692842 datazimmer-0.5.2/datazimmer/tests/test_sql.py
--rw-r--r--   0        0        0      235 2023-06-19 14:24:46.692842 datazimmer-0.5.2/datazimmer/tests/test_util.py
--rw-r--r--   0        0        0      943 2023-06-19 14:24:46.692842 datazimmer-0.5.2/datazimmer/tests/test_validation.py
--rw-r--r--   0        0        0      939 2023-06-19 14:24:46.692842 datazimmer-0.5.2/datazimmer/tests/util.py
--rw-r--r--   0        0        0    10109 2023-06-19 14:24:46.692842 datazimmer-0.5.2/datazimmer/typer_commands.py
--rw-r--r--   0        0        0     3260 2023-06-19 14:24:46.692842 datazimmer-0.5.2/datazimmer/utils.py
--rw-r--r--   0        0        0     2957 2023-06-19 14:24:46.692842 datazimmer-0.5.2/datazimmer/validation_functions.py
--rw-r--r--   0        0        0    10327 2023-06-19 14:24:46.692842 datazimmer-0.5.2/datazimmer/zenodo.py
--rw-r--r--   0        0        0      114 2023-06-19 14:24:46.692842 datazimmer-0.5.2/docs/api/datazimmer.AbstractEntity.rst
--rw-r--r--   0        0        0      123 2023-06-19 14:24:46.692842 datazimmer-0.5.2/docs/api/datazimmer.CompositeTypeBase.rst
--rw-r--r--   0        0        0      746 2023-06-19 14:24:46.692842 datazimmer-0.5.2/docs/api/datazimmer.DzAswan.rst
--rw-r--r--   0        0        0      739 2023-06-19 14:24:46.692842 datazimmer-0.5.2/docs/api/datazimmer.EntityClass.rst
--rw-r--r--   0        0        0       87 2023-06-19 14:24:46.692842 datazimmer-0.5.2/docs/api/datazimmer.Index.rst
--rw-r--r--   0        0        0       96 2023-06-19 14:24:46.692842 datazimmer-0.5.2/docs/api/datazimmer.Nullable.rst
--rw-r--r--   0        0        0      444 2023-06-19 14:24:46.692842 datazimmer-0.5.2/docs/api/datazimmer.PersistentState.rst
--rw-r--r--   0        0        0      592 2023-06-19 14:24:46.692842 datazimmer-0.5.2/docs/api/datazimmer.ReportFile.rst
--rw-r--r--   0        0        0      565 2023-06-19 14:24:46.692842 datazimmer-0.5.2/docs/api/datazimmer.ScruTable.rst
--rw-r--r--   0        0        0       99 2023-06-19 14:24:46.692842 datazimmer-0.5.2/docs/api/datazimmer.SourceUrl.rst
--rw-r--r--   0        0        0      107 2023-06-19 14:24:46.692842 datazimmer-0.5.2/docs/api/datazimmer.dump_dfs_to_tables.rst
--rw-r--r--   0        0        0      104 2023-06-19 14:24:46.692842 datazimmer-0.5.2/docs/api/datazimmer.get_raw_data_path.rst
--rw-r--r--   0        0        0       77 2023-06-19 14:24:46.692842 datazimmer-0.5.2/docs/api/datazimmer.parse_df.rst
--rw-r--r--   0        0        0       77 2023-06-19 14:24:46.692842 datazimmer-0.5.2/docs/api/datazimmer.register.rst
--rw-r--r--   0        0        0      113 2023-06-19 14:24:46.692842 datazimmer-0.5.2/docs/api/datazimmer.register_data_loader.rst
--rw-r--r--   0        0        0      113 2023-06-19 14:24:46.692842 datazimmer-0.5.2/docs/api/datazimmer.register_env_creator.rst
--rw-r--r--   0        0        0       39 2023-06-19 14:24:46.692842 datazimmer-0.5.2/docs/autosumm.rst
--rw-r--r--   0        0        0     2402 2023-06-19 14:24:46.692842 datazimmer-0.5.2/docs/conf.py
--rw-r--r--   0        0        0      263 2023-06-19 14:24:46.692842 datazimmer-0.5.2/docs/index.rst
--rw-r--r--   0        0        0       77 2023-06-19 14:24:46.692842 datazimmer-0.5.2/docs/notebooks/doc-001-intro.rst
--rw-r--r--   0        0        0     4171 2023-06-19 14:24:46.692842 datazimmer-0.5.2/docs/notebooks/doc-002-glossary.rst
--rw-r--r--   0        0        0      616 2023-06-19 14:24:46.692842 datazimmer-0.5.2/docs/notebooks/doc-003-mock-projects.rst
--rw-r--r--   0        0        0     1269 2023-06-19 14:24:46.692842 datazimmer-0.5.2/docs/notebooks/doc-004-rules-conventions.rst
--rw-r--r--   0        0        0      284 2023-06-19 14:24:46.692842 datazimmer-0.5.2/docs/notebooks/doc-005-cli.rst
--rw-r--r--   0        0        0      102 2023-06-19 14:24:46.692842 datazimmer-0.5.2/docs/release_notes/main.rst
--rw-r--r--   0        0        0       45 2023-06-19 14:24:46.692842 datazimmer-0.5.2/docs/release_notes/v0.1.0.rst
--rw-r--r--   0        0        0       46 2023-06-19 14:24:46.692842 datazimmer-0.5.2/docs/release_notes/v0.1.1.rst
--rw-r--r--   0        0        0       27 2023-06-19 14:24:46.692842 datazimmer-0.5.2/docs/release_notes/v0.1.2.rst
--rw-r--r--   0        0        0       15 2023-06-19 14:24:46.692842 datazimmer-0.5.2/docs/release_notes/v0.1.3.rst
--rw-r--r--   0        0        0       15 2023-06-19 14:24:46.692842 datazimmer-0.5.2/docs/release_notes/v0.1.4.rst
--rw-r--r--   0        0        0       15 2023-06-19 14:24:46.692842 datazimmer-0.5.2/docs/release_notes/v0.1.5.rst
--rw-r--r--   0        0        0       34 2023-06-19 14:24:46.692842 datazimmer-0.5.2/docs/release_notes/v0.2.1.rst
--rw-r--r--   0        0        0       31 2023-06-19 14:24:46.692842 datazimmer-0.5.2/docs/release_notes/v0.2.2.rst
--rw-r--r--   0        0        0       31 2023-06-19 14:24:46.692842 datazimmer-0.5.2/docs/release_notes/v0.2.3.rst
--rw-r--r--   0        0        0       31 2023-06-19 14:24:46.692842 datazimmer-0.5.2/docs/release_notes/v0.2.4.rst
--rw-r--r--   0        0        0       29 2023-06-19 14:24:46.692842 datazimmer-0.5.2/docs/release_notes/v0.2.5.rst
--rw-r--r--   0        0        0       39 2023-06-19 14:24:46.692842 datazimmer-0.5.2/docs/release_notes/v0.2.6.rst
--rw-r--r--   0        0        0       34 2023-06-19 14:24:46.692842 datazimmer-0.5.2/docs/release_notes/v0.2.7.rst
--rw-r--r--   0        0        0       45 2023-06-19 14:24:46.692842 datazimmer-0.5.2/docs/release_notes/v0.3.0.rst
--rw-r--r--   0        0        0       32 2023-06-19 14:24:46.692842 datazimmer-0.5.2/docs/release_notes/v0.3.1.rst
--rw-r--r--   0        0        0       48 2023-06-19 14:24:46.692842 datazimmer-0.5.2/docs/release_notes/v0.3.10.rst
--rw-r--r--   0        0        0       47 2023-06-19 14:24:46.692842 datazimmer-0.5.2/docs/release_notes/v0.3.2.rst
--rw-r--r--   0        0        0       39 2023-06-19 14:24:46.692842 datazimmer-0.5.2/docs/release_notes/v0.3.3.rst
--rw-r--r--   0        0        0       33 2023-06-19 14:24:46.692842 datazimmer-0.5.2/docs/release_notes/v0.3.4.rst
--rw-r--r--   0        0        0       34 2023-06-19 14:24:46.692842 datazimmer-0.5.2/docs/release_notes/v0.3.5.rst
--rw-r--r--   0        0        0       32 2023-06-19 14:24:46.692842 datazimmer-0.5.2/docs/release_notes/v0.3.6.rst
--rw-r--r--   0        0        0       32 2023-06-19 14:24:46.692842 datazimmer-0.5.2/docs/release_notes/v0.3.7.rst
--rw-r--r--   0        0        0       31 2023-06-19 14:24:46.692842 datazimmer-0.5.2/docs/release_notes/v0.3.8.rst
--rw-r--r--   0        0        0       35 2023-06-19 14:24:46.692842 datazimmer-0.5.2/docs/release_notes/v0.3.9.rst
--rw-r--r--   0        0        0       37 2023-06-19 14:24:46.692842 datazimmer-0.5.2/docs/release_notes/v0.4.0.rst
--rw-r--r--   0        0        0       32 2023-06-19 14:24:46.692842 datazimmer-0.5.2/docs/release_notes/v0.4.1.rst
--rw-r--r--   0        0        0       70 2023-06-19 14:24:46.692842 datazimmer-0.5.2/docs/release_notes/v0.4.10.rst
--rw-r--r--   0        0        0       55 2023-06-19 14:24:46.692842 datazimmer-0.5.2/docs/release_notes/v0.4.11.rst
--rw-r--r--   0        0        0       45 2023-06-19 14:24:46.692842 datazimmer-0.5.2/docs/release_notes/v0.4.12.rst
--rw-r--r--   0        0        0       68 2023-06-19 14:24:46.692842 datazimmer-0.5.2/docs/release_notes/v0.4.13.rst
--rw-r--r--   0        0        0       68 2023-06-19 14:24:46.692842 datazimmer-0.5.2/docs/release_notes/v0.4.14.rst
--rw-r--r--   0        0        0       42 2023-06-19 14:24:46.692842 datazimmer-0.5.2/docs/release_notes/v0.4.15.rst
--rw-r--r--   0        0        0       52 2023-06-19 14:24:46.692842 datazimmer-0.5.2/docs/release_notes/v0.4.2.rst
--rw-r--r--   0        0        0       66 2023-06-19 14:24:46.692842 datazimmer-0.5.2/docs/release_notes/v0.4.3.rst
--rw-r--r--   0        0        0       53 2023-06-19 14:24:46.692842 datazimmer-0.5.2/docs/release_notes/v0.4.4.rst
--rw-r--r--   0        0        0       45 2023-06-19 14:24:46.692842 datazimmer-0.5.2/docs/release_notes/v0.4.5.rst
--rw-r--r--   0        0        0       41 2023-06-19 14:24:46.692842 datazimmer-0.5.2/docs/release_notes/v0.4.6.rst
--rw-r--r--   0        0        0       71 2023-06-19 14:24:46.692842 datazimmer-0.5.2/docs/release_notes/v0.4.7.rst
--rw-r--r--   0        0        0       47 2023-06-19 14:24:46.692842 datazimmer-0.5.2/docs/release_notes/v0.4.8.rst
--rw-r--r--   0        0        0       53 2023-06-19 14:24:46.692842 datazimmer-0.5.2/docs/release_notes/v0.4.9.rst
--rw-r--r--   0        0        0       64 2023-06-19 14:24:46.692842 datazimmer-0.5.2/docs/release_notes/v0.5.0.rst
--rw-r--r--   0        0        0       50 2023-06-19 14:24:46.692842 datazimmer-0.5.2/docs/release_notes/v0.5.1.rst
--rw-r--r--   0        0        0       51 2023-06-19 14:24:46.692842 datazimmer-0.5.2/docs/release_notes/v0.5.2.rst
--rw-r--r--   0        0        0      159 2023-06-19 14:24:46.692842 datazimmer-0.5.2/dogshow/confs.yaml
--rw-r--r--   0        0        0     1773 2023-06-19 14:24:46.692842 datazimmer-0.5.2/dogshow/data/photo.csv
--rw-r--r--   0        0        0      655 2023-06-19 14:24:46.692842 datazimmer-0.5.2/dogshow/minimal.py
--rw-r--r--   0        0        0     9861 2023-06-19 14:24:46.692842 datazimmer-0.5.2/dogshow/projects/cc-dog-raw/{{cookiecutter.project}}/notebooks/create-dogshow-test-data.ipynb
--rw-r--r--   0        0        0       57 2023-06-19 14:24:46.692842 datazimmer-0.5.2/dogshow/projects/cc-dog-raw/{{cookiecutter.project}}/zimmer.yaml
--rw-r--r--   0        0        0        0 2023-06-19 14:24:46.692842 datazimmer-0.5.2/dogshow/projects/cc-dog-show/{{cookiecutter.project}}/src/__init__.py
--rw-r--r--   0        0        0        0 2023-06-19 14:24:46.692842 datazimmer-0.5.2/dogshow/projects/cc-dog-show/{{cookiecutter.project}}/src/core/__init__.py
--rw-r--r--   0        0        0     2304 2023-06-19 14:24:46.692842 datazimmer-0.5.2/dogshow/projects/cc-dog-show/{{cookiecutter.project}}/src/core/create_envs.py
--rw-r--r--   0        0        0     1566 2023-06-19 14:24:46.692842 datazimmer-0.5.2/dogshow/projects/cc-dog-show/{{cookiecutter.project}}/src/core/ns_meta.py
--rw-r--r--   0        0        0     3192 2023-06-19 14:24:46.692842 datazimmer-0.5.2/dogshow/projects/cc-dog-show/{{cookiecutter.project}}/src/core/update_data.py
--rw-r--r--   0        0        0      307 2023-06-19 14:24:46.692842 datazimmer-0.5.2/dogshow/projects/cc-dog-show/{{cookiecutter.project}}/zimmer.yaml
--rw-r--r--   0        0        0        0 2023-06-19 14:24:46.696843 datazimmer-0.5.2/dogshow/projects/cc-dogcombine/{{cookiecutter.project}}/src/__init__.py
--rw-r--r--   0        0        0      674 2023-06-19 14:24:46.696843 datazimmer-0.5.2/dogshow/projects/cc-dogcombine/{{cookiecutter.project}}/src/joint_success.py
--rw-r--r--   0        0        0      261 2023-06-19 14:24:46.696843 datazimmer-0.5.2/dogshow/projects/cc-dogcombine/{{cookiecutter.project}}/zimmer.yaml
--rw-r--r--   0        0        0        0 2023-06-19 14:24:46.696843 datazimmer-0.5.2/dogshow/projects/cc-dograce/{{cookiecutter.project}}/src/__init__.py
--rw-r--r--   0        0        0     2533 2023-06-19 14:24:46.696843 datazimmer-0.5.2/dogshow/projects/cc-dograce/{{cookiecutter.project}}/src/core.py
--rw-r--r--   0        0        0      120 2023-06-19 14:24:46.696843 datazimmer-0.5.2/dogshow/projects/cc-dograce/{{cookiecutter.project}}/zimmer.yaml
--rw-r--r--   0        0        0        0 2023-06-19 14:24:46.696843 datazimmer-0.5.2/dogshow/projects/cc-dogsuccess/{{cookiecutter.project}}/src/__init__.py
--rw-r--r--   0        0        0       65 2023-06-19 14:24:46.696843 datazimmer-0.5.2/dogshow/projects/cc-dogsuccess/{{cookiecutter.project}}/src/counts/__init__.py
--rw-r--r--   0        0        0      421 2023-06-19 14:24:46.696843 datazimmer-0.5.2/dogshow/projects/cc-dogsuccess/{{cookiecutter.project}}/src/counts/meta.py
--rw-r--r--   0        0        0      945 2023-06-19 14:24:46.696843 datazimmer-0.5.2/dogshow/projects/cc-dogsuccess/{{cookiecutter.project}}/src/counts/proc.py
--rw-r--r--   0        0        0     1093 2023-06-19 14:24:46.696843 datazimmer-0.5.2/dogshow/projects/cc-dogsuccess/{{cookiecutter.project}}/src/sex_matches.py
--rw-r--r--   0        0        0     2415 2023-06-19 14:24:46.696843 datazimmer-0.5.2/dogshow/projects/cc-dogsuccess/{{cookiecutter.project}}/src/success.py
--rw-r--r--   0        0        0      810 2023-06-19 14:24:46.696843 datazimmer-0.5.2/dogshow/projects/cc-dogsuccess/{{cookiecutter.project}}/src/top_report.py
--rw-r--r--   0        0        0      575 2023-06-19 14:24:46.696843 datazimmer-0.5.2/dogshow/projects/cc-dogsuccess/{{cookiecutter.project}}/zimmer.yaml
--rw-r--r--   0        0        0     2940 2023-06-19 14:24:46.696843 datazimmer-0.5.2/dogshow/todo/complex_success.py
--rw-r--r--   0        0        0      612 2023-06-19 14:24:46.696843 datazimmer-0.5.2/notebooks/doc-001-intro.ipynb
--rw-r--r--   0        0        0     5328 2023-06-19 14:24:46.696843 datazimmer-0.5.2/notebooks/doc-002-glossary.ipynb
--rw-r--r--   0        0        0     1877 2023-06-19 14:24:46.696843 datazimmer-0.5.2/notebooks/doc-003-mock-projects.ipynb
--rw-r--r--   0        0        0     1928 2023-06-19 14:24:46.696843 datazimmer-0.5.2/notebooks/doc-004-rules-conventions.ipynb
--rw-r--r--   0        0        0     1235 2023-06-19 14:24:46.696843 datazimmer-0.5.2/notebooks/doc-005-cli.ipynb
--rw-r--r--   0        0        0     1109 2023-06-19 14:24:46.696843 datazimmer-0.5.2/pyproject.toml
--rw-r--r--   0        0        0     4493 1970-01-01 00:00:00.000000 datazimmer-0.5.2/PKG-INFO
+-rw-r--r--   0        0        0     1003 2023-06-22 12:16:49.810338 datazimmer-0.5.3/.github/workflows/compatibility_test.yml
+-rw-r--r--   0        0        0     1299 2023-06-22 12:16:49.810338 datazimmer-0.5.3/.github/workflows/test.yml
+-rw-r--r--   0        0        0      565 2023-06-22 12:16:49.810338 datazimmer-0.5.3/.github/workflows/twine_release.yml
+-rw-r--r--   0        0        0     1795 2023-06-22 12:16:49.810338 datazimmer-0.5.3/.gitignore
+-rw-r--r--   0        0        0      288 2023-06-22 12:16:49.810338 datazimmer-0.5.3/.readthedocs.yml
+-rw-r--r--   0        0        0      491 2023-06-22 12:16:49.810338 datazimmer-0.5.3/CITATION.cff
+-rw-r--r--   0        0        0     1077 2023-06-22 12:16:49.810338 datazimmer-0.5.3/LICENSE
+-rw-r--r--   0        0        0     3122 2023-06-22 12:16:49.810338 datazimmer-0.5.3/README.md
+-rw-r--r--   0        0        0     4090 2023-06-22 12:16:49.810338 datazimmer-0.5.3/conftest.py
+-rw-r--r--   0        0        0      634 2023-06-22 12:16:49.810338 datazimmer-0.5.3/datazimmer/__init__.py
+-rw-r--r--   0        0        0     2962 2023-06-22 12:16:49.810338 datazimmer-0.5.3/datazimmer/aswan_integration.py
+-rw-r--r--   0        0        0     7923 2023-06-22 12:16:49.810338 datazimmer-0.5.3/datazimmer/config_loading.py
+-rw-r--r--   0        0        0     2192 2023-06-22 12:16:49.810338 datazimmer-0.5.3/datazimmer/dvc_util.py
+-rw-r--r--   0        0        0      144 2023-06-22 12:16:49.810338 datazimmer-0.5.3/datazimmer/exceptions.py
+-rw-r--r--   0        0        0      624 2023-06-22 12:16:49.810338 datazimmer-0.5.3/datazimmer/get_runtime.py
+-rw-r--r--   0        0        0     2434 2023-06-22 12:16:49.810338 datazimmer-0.5.3/datazimmer/gh_actions.py
+-rw-r--r--   0        0        0        0 2023-06-22 12:16:49.810338 datazimmer-0.5.3/datazimmer/metadata/__init__.py
+-rw-r--r--   0        0        0     6235 2023-06-22 12:16:49.810338 datazimmer-0.5.3/datazimmer/metadata/atoms.py
+-rw-r--r--   0        0        0     1422 2023-06-22 12:16:49.810338 datazimmer-0.5.3/datazimmer/metadata/complete_id.py
+-rw-r--r--   0        0        0     1744 2023-06-22 12:16:49.810338 datazimmer-0.5.3/datazimmer/metadata/datascript.py
+-rw-r--r--   0        0        0     4537 2023-06-22 12:16:49.810338 datazimmer-0.5.3/datazimmer/metadata/high_level.py
+-rw-r--r--   0        0        0     4798 2023-06-22 12:16:49.810338 datazimmer-0.5.3/datazimmer/metadata/scrutable.py
+-rw-r--r--   0        0        0     3456 2023-06-22 12:16:49.810338 datazimmer-0.5.3/datazimmer/naming.py
+-rw-r--r--   0        0        0      526 2023-06-22 12:16:49.810338 datazimmer-0.5.3/datazimmer/persistent_state.py
+-rw-r--r--   0        0        0     8463 2023-06-22 12:16:49.810338 datazimmer-0.5.3/datazimmer/pipeline_element.py
+-rw-r--r--   0        0        0     7648 2023-06-22 12:16:49.810338 datazimmer-0.5.3/datazimmer/project_runtime.py
+-rw-r--r--   0        0        0      935 2023-06-22 12:16:49.810338 datazimmer-0.5.3/datazimmer/raw_data.py
+-rw-r--r--   0        0        0     6249 2023-06-22 12:16:49.810338 datazimmer-0.5.3/datazimmer/registry.py
+-rw-r--r--   0        0        0      863 2023-06-22 12:16:49.810338 datazimmer-0.5.3/datazimmer/reporting.py
+-rw-r--r--   0        0        0        0 2023-06-22 12:16:49.810338 datazimmer-0.5.3/datazimmer/sql/__init__.py
+-rw-r--r--   0        0        0       87 2023-06-22 12:16:49.810338 datazimmer-0.5.3/datazimmer/sql/draw.py
+-rw-r--r--   0        0        0     7107 2023-06-22 12:16:49.810338 datazimmer-0.5.3/datazimmer/sql/loader.py
+-rw-r--r--   0        0        0        0 2023-06-22 12:16:49.810338 datazimmer-0.5.3/datazimmer/tests/__init__.py
+-rw-r--r--   0        0        0     4708 2023-06-22 12:16:49.810338 datazimmer-0.5.3/datazimmer/tests/create_dogshow.py
+-rw-r--r--   0        0        0      845 2023-06-22 12:16:49.810338 datazimmer-0.5.3/datazimmer/tests/test_commands.py
+-rw-r--r--   0        0        0      346 2023-06-22 12:16:49.810338 datazimmer-0.5.3/datazimmer/tests/test_config.py
+-rw-r--r--   0        0        0     4366 2023-06-22 12:16:49.810338 datazimmer-0.5.3/datazimmer/tests/test_full_integration.py
+-rw-r--r--   0        0        0      465 2023-06-22 12:16:49.810338 datazimmer-0.5.3/datazimmer/tests/test_registry.py
+-rw-r--r--   0        0        0      294 2023-06-22 12:16:49.810338 datazimmer-0.5.3/datazimmer/tests/test_runtime.py
+-rw-r--r--   0        0        0     1799 2023-06-22 12:16:49.810338 datazimmer-0.5.3/datazimmer/tests/test_scrutable.py
+-rw-r--r--   0        0        0      152 2023-06-22 12:16:49.810338 datazimmer-0.5.3/datazimmer/tests/test_sql.py
+-rw-r--r--   0        0        0      235 2023-06-22 12:16:49.810338 datazimmer-0.5.3/datazimmer/tests/test_util.py
+-rw-r--r--   0        0        0      943 2023-06-22 12:16:49.810338 datazimmer-0.5.3/datazimmer/tests/test_validation.py
+-rw-r--r--   0        0        0      939 2023-06-22 12:16:49.810338 datazimmer-0.5.3/datazimmer/tests/util.py
+-rw-r--r--   0        0        0    10106 2023-06-22 12:16:49.810338 datazimmer-0.5.3/datazimmer/typer_commands.py
+-rw-r--r--   0        0        0     3260 2023-06-22 12:16:49.810338 datazimmer-0.5.3/datazimmer/utils.py
+-rw-r--r--   0        0        0     2957 2023-06-22 12:16:49.810338 datazimmer-0.5.3/datazimmer/validation_functions.py
+-rw-r--r--   0        0        0    10327 2023-06-22 12:16:49.810338 datazimmer-0.5.3/datazimmer/zenodo.py
+-rw-r--r--   0        0        0      114 2023-06-22 12:16:49.810338 datazimmer-0.5.3/docs/api/datazimmer.AbstractEntity.rst
+-rw-r--r--   0        0        0      123 2023-06-22 12:16:49.810338 datazimmer-0.5.3/docs/api/datazimmer.CompositeTypeBase.rst
+-rw-r--r--   0        0        0      746 2023-06-22 12:16:49.810338 datazimmer-0.5.3/docs/api/datazimmer.DzAswan.rst
+-rw-r--r--   0        0        0      739 2023-06-22 12:16:49.810338 datazimmer-0.5.3/docs/api/datazimmer.EntityClass.rst
+-rw-r--r--   0        0        0       87 2023-06-22 12:16:49.810338 datazimmer-0.5.3/docs/api/datazimmer.Index.rst
+-rw-r--r--   0        0        0       96 2023-06-22 12:16:49.810338 datazimmer-0.5.3/docs/api/datazimmer.Nullable.rst
+-rw-r--r--   0        0        0      444 2023-06-22 12:16:49.810338 datazimmer-0.5.3/docs/api/datazimmer.PersistentState.rst
+-rw-r--r--   0        0        0      592 2023-06-22 12:16:49.810338 datazimmer-0.5.3/docs/api/datazimmer.ReportFile.rst
+-rw-r--r--   0        0        0      565 2023-06-22 12:16:49.810338 datazimmer-0.5.3/docs/api/datazimmer.ScruTable.rst
+-rw-r--r--   0        0        0       99 2023-06-22 12:16:49.810338 datazimmer-0.5.3/docs/api/datazimmer.SourceUrl.rst
+-rw-r--r--   0        0        0      107 2023-06-22 12:16:49.810338 datazimmer-0.5.3/docs/api/datazimmer.dump_dfs_to_tables.rst
+-rw-r--r--   0        0        0      104 2023-06-22 12:16:49.810338 datazimmer-0.5.3/docs/api/datazimmer.get_raw_data_path.rst
+-rw-r--r--   0        0        0       77 2023-06-22 12:16:49.810338 datazimmer-0.5.3/docs/api/datazimmer.parse_df.rst
+-rw-r--r--   0        0        0       77 2023-06-22 12:16:49.810338 datazimmer-0.5.3/docs/api/datazimmer.register.rst
+-rw-r--r--   0        0        0      113 2023-06-22 12:16:49.810338 datazimmer-0.5.3/docs/api/datazimmer.register_data_loader.rst
+-rw-r--r--   0        0        0      113 2023-06-22 12:16:49.810338 datazimmer-0.5.3/docs/api/datazimmer.register_env_creator.rst
+-rw-r--r--   0        0        0       39 2023-06-22 12:16:49.810338 datazimmer-0.5.3/docs/autosumm.rst
+-rw-r--r--   0        0        0     2402 2023-06-22 12:16:49.810338 datazimmer-0.5.3/docs/conf.py
+-rw-r--r--   0        0        0      263 2023-06-22 12:16:49.810338 datazimmer-0.5.3/docs/index.rst
+-rw-r--r--   0        0        0       77 2023-06-22 12:16:49.810338 datazimmer-0.5.3/docs/notebooks/doc-001-intro.rst
+-rw-r--r--   0        0        0     4171 2023-06-22 12:16:49.810338 datazimmer-0.5.3/docs/notebooks/doc-002-glossary.rst
+-rw-r--r--   0        0        0      616 2023-06-22 12:16:49.814338 datazimmer-0.5.3/docs/notebooks/doc-003-mock-projects.rst
+-rw-r--r--   0        0        0     1269 2023-06-22 12:16:49.814338 datazimmer-0.5.3/docs/notebooks/doc-004-rules-conventions.rst
+-rw-r--r--   0        0        0      284 2023-06-22 12:16:49.814338 datazimmer-0.5.3/docs/notebooks/doc-005-cli.rst
+-rw-r--r--   0        0        0      102 2023-06-22 12:16:49.814338 datazimmer-0.5.3/docs/release_notes/main.rst
+-rw-r--r--   0        0        0       45 2023-06-22 12:16:49.814338 datazimmer-0.5.3/docs/release_notes/v0.1.0.rst
+-rw-r--r--   0        0        0       46 2023-06-22 12:16:49.814338 datazimmer-0.5.3/docs/release_notes/v0.1.1.rst
+-rw-r--r--   0        0        0       27 2023-06-22 12:16:49.814338 datazimmer-0.5.3/docs/release_notes/v0.1.2.rst
+-rw-r--r--   0        0        0       15 2023-06-22 12:16:49.814338 datazimmer-0.5.3/docs/release_notes/v0.1.3.rst
+-rw-r--r--   0        0        0       15 2023-06-22 12:16:49.814338 datazimmer-0.5.3/docs/release_notes/v0.1.4.rst
+-rw-r--r--   0        0        0       15 2023-06-22 12:16:49.814338 datazimmer-0.5.3/docs/release_notes/v0.1.5.rst
+-rw-r--r--   0        0        0       34 2023-06-22 12:16:49.814338 datazimmer-0.5.3/docs/release_notes/v0.2.1.rst
+-rw-r--r--   0        0        0       31 2023-06-22 12:16:49.814338 datazimmer-0.5.3/docs/release_notes/v0.2.2.rst
+-rw-r--r--   0        0        0       31 2023-06-22 12:16:49.814338 datazimmer-0.5.3/docs/release_notes/v0.2.3.rst
+-rw-r--r--   0        0        0       31 2023-06-22 12:16:49.814338 datazimmer-0.5.3/docs/release_notes/v0.2.4.rst
+-rw-r--r--   0        0        0       29 2023-06-22 12:16:49.814338 datazimmer-0.5.3/docs/release_notes/v0.2.5.rst
+-rw-r--r--   0        0        0       39 2023-06-22 12:16:49.814338 datazimmer-0.5.3/docs/release_notes/v0.2.6.rst
+-rw-r--r--   0        0        0       34 2023-06-22 12:16:49.814338 datazimmer-0.5.3/docs/release_notes/v0.2.7.rst
+-rw-r--r--   0        0        0       45 2023-06-22 12:16:49.814338 datazimmer-0.5.3/docs/release_notes/v0.3.0.rst
+-rw-r--r--   0        0        0       32 2023-06-22 12:16:49.814338 datazimmer-0.5.3/docs/release_notes/v0.3.1.rst
+-rw-r--r--   0        0        0       48 2023-06-22 12:16:49.814338 datazimmer-0.5.3/docs/release_notes/v0.3.10.rst
+-rw-r--r--   0        0        0       47 2023-06-22 12:16:49.814338 datazimmer-0.5.3/docs/release_notes/v0.3.2.rst
+-rw-r--r--   0        0        0       39 2023-06-22 12:16:49.814338 datazimmer-0.5.3/docs/release_notes/v0.3.3.rst
+-rw-r--r--   0        0        0       33 2023-06-22 12:16:49.814338 datazimmer-0.5.3/docs/release_notes/v0.3.4.rst
+-rw-r--r--   0        0        0       34 2023-06-22 12:16:49.814338 datazimmer-0.5.3/docs/release_notes/v0.3.5.rst
+-rw-r--r--   0        0        0       32 2023-06-22 12:16:49.814338 datazimmer-0.5.3/docs/release_notes/v0.3.6.rst
+-rw-r--r--   0        0        0       32 2023-06-22 12:16:49.814338 datazimmer-0.5.3/docs/release_notes/v0.3.7.rst
+-rw-r--r--   0        0        0       31 2023-06-22 12:16:49.814338 datazimmer-0.5.3/docs/release_notes/v0.3.8.rst
+-rw-r--r--   0        0        0       35 2023-06-22 12:16:49.814338 datazimmer-0.5.3/docs/release_notes/v0.3.9.rst
+-rw-r--r--   0        0        0       37 2023-06-22 12:16:49.814338 datazimmer-0.5.3/docs/release_notes/v0.4.0.rst
+-rw-r--r--   0        0        0       32 2023-06-22 12:16:49.814338 datazimmer-0.5.3/docs/release_notes/v0.4.1.rst
+-rw-r--r--   0        0        0       70 2023-06-22 12:16:49.814338 datazimmer-0.5.3/docs/release_notes/v0.4.10.rst
+-rw-r--r--   0        0        0       55 2023-06-22 12:16:49.814338 datazimmer-0.5.3/docs/release_notes/v0.4.11.rst
+-rw-r--r--   0        0        0       45 2023-06-22 12:16:49.814338 datazimmer-0.5.3/docs/release_notes/v0.4.12.rst
+-rw-r--r--   0        0        0       68 2023-06-22 12:16:49.814338 datazimmer-0.5.3/docs/release_notes/v0.4.13.rst
+-rw-r--r--   0        0        0       68 2023-06-22 12:16:49.814338 datazimmer-0.5.3/docs/release_notes/v0.4.14.rst
+-rw-r--r--   0        0        0       42 2023-06-22 12:16:49.814338 datazimmer-0.5.3/docs/release_notes/v0.4.15.rst
+-rw-r--r--   0        0        0       52 2023-06-22 12:16:49.814338 datazimmer-0.5.3/docs/release_notes/v0.4.2.rst
+-rw-r--r--   0        0        0       66 2023-06-22 12:16:49.814338 datazimmer-0.5.3/docs/release_notes/v0.4.3.rst
+-rw-r--r--   0        0        0       53 2023-06-22 12:16:49.814338 datazimmer-0.5.3/docs/release_notes/v0.4.4.rst
+-rw-r--r--   0        0        0       45 2023-06-22 12:16:49.814338 datazimmer-0.5.3/docs/release_notes/v0.4.5.rst
+-rw-r--r--   0        0        0       41 2023-06-22 12:16:49.814338 datazimmer-0.5.3/docs/release_notes/v0.4.6.rst
+-rw-r--r--   0        0        0       71 2023-06-22 12:16:49.814338 datazimmer-0.5.3/docs/release_notes/v0.4.7.rst
+-rw-r--r--   0        0        0       47 2023-06-22 12:16:49.814338 datazimmer-0.5.3/docs/release_notes/v0.4.8.rst
+-rw-r--r--   0        0        0       53 2023-06-22 12:16:49.814338 datazimmer-0.5.3/docs/release_notes/v0.4.9.rst
+-rw-r--r--   0        0        0       64 2023-06-22 12:16:49.814338 datazimmer-0.5.3/docs/release_notes/v0.5.0.rst
+-rw-r--r--   0        0        0       50 2023-06-22 12:16:49.814338 datazimmer-0.5.3/docs/release_notes/v0.5.1.rst
+-rw-r--r--   0        0        0       51 2023-06-22 12:16:49.814338 datazimmer-0.5.3/docs/release_notes/v0.5.2.rst
+-rw-r--r--   0        0        0       59 2023-06-22 12:16:49.814338 datazimmer-0.5.3/docs/release_notes/v0.5.3.rst
+-rw-r--r--   0        0        0      159 2023-06-22 12:16:49.814338 datazimmer-0.5.3/dogshow/confs.yaml
+-rw-r--r--   0        0        0     1773 2023-06-22 12:16:49.814338 datazimmer-0.5.3/dogshow/data/photo.csv
+-rw-r--r--   0        0        0      655 2023-06-22 12:16:49.814338 datazimmer-0.5.3/dogshow/minimal.py
+-rw-r--r--   0        0        0     9861 2023-06-22 12:16:49.814338 datazimmer-0.5.3/dogshow/projects/cc-dog-raw/{{cookiecutter.project}}/notebooks/create-dogshow-test-data.ipynb
+-rw-r--r--   0        0        0       57 2023-06-22 12:16:49.814338 datazimmer-0.5.3/dogshow/projects/cc-dog-raw/{{cookiecutter.project}}/zimmer.yaml
+-rw-r--r--   0        0        0        0 2023-06-22 12:16:49.814338 datazimmer-0.5.3/dogshow/projects/cc-dog-show/{{cookiecutter.project}}/src/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-22 12:16:49.814338 datazimmer-0.5.3/dogshow/projects/cc-dog-show/{{cookiecutter.project}}/src/core/__init__.py
+-rw-r--r--   0        0        0     2304 2023-06-22 12:16:49.814338 datazimmer-0.5.3/dogshow/projects/cc-dog-show/{{cookiecutter.project}}/src/core/create_envs.py
+-rw-r--r--   0        0        0     1566 2023-06-22 12:16:49.814338 datazimmer-0.5.3/dogshow/projects/cc-dog-show/{{cookiecutter.project}}/src/core/ns_meta.py
+-rw-r--r--   0        0        0     3324 2023-06-22 12:16:49.814338 datazimmer-0.5.3/dogshow/projects/cc-dog-show/{{cookiecutter.project}}/src/core/update_data.py
+-rw-r--r--   0        0        0      307 2023-06-22 12:16:49.814338 datazimmer-0.5.3/dogshow/projects/cc-dog-show/{{cookiecutter.project}}/zimmer.yaml
+-rw-r--r--   0        0        0        0 2023-06-22 12:16:49.814338 datazimmer-0.5.3/dogshow/projects/cc-dogcombine/{{cookiecutter.project}}/src/__init__.py
+-rw-r--r--   0        0        0      674 2023-06-22 12:16:49.814338 datazimmer-0.5.3/dogshow/projects/cc-dogcombine/{{cookiecutter.project}}/src/joint_success.py
+-rw-r--r--   0        0        0      261 2023-06-22 12:16:49.814338 datazimmer-0.5.3/dogshow/projects/cc-dogcombine/{{cookiecutter.project}}/zimmer.yaml
+-rw-r--r--   0        0        0        0 2023-06-22 12:16:49.814338 datazimmer-0.5.3/dogshow/projects/cc-dograce/{{cookiecutter.project}}/src/__init__.py
+-rw-r--r--   0        0        0     2533 2023-06-22 12:16:49.814338 datazimmer-0.5.3/dogshow/projects/cc-dograce/{{cookiecutter.project}}/src/core.py
+-rw-r--r--   0        0        0      120 2023-06-22 12:16:49.814338 datazimmer-0.5.3/dogshow/projects/cc-dograce/{{cookiecutter.project}}/zimmer.yaml
+-rw-r--r--   0        0        0        0 2023-06-22 12:16:49.814338 datazimmer-0.5.3/dogshow/projects/cc-dogsuccess/{{cookiecutter.project}}/src/__init__.py
+-rw-r--r--   0        0        0       65 2023-06-22 12:16:49.814338 datazimmer-0.5.3/dogshow/projects/cc-dogsuccess/{{cookiecutter.project}}/src/counts/__init__.py
+-rw-r--r--   0        0        0      421 2023-06-22 12:16:49.814338 datazimmer-0.5.3/dogshow/projects/cc-dogsuccess/{{cookiecutter.project}}/src/counts/meta.py
+-rw-r--r--   0        0        0      945 2023-06-22 12:16:49.814338 datazimmer-0.5.3/dogshow/projects/cc-dogsuccess/{{cookiecutter.project}}/src/counts/proc.py
+-rw-r--r--   0        0        0     1093 2023-06-22 12:16:49.814338 datazimmer-0.5.3/dogshow/projects/cc-dogsuccess/{{cookiecutter.project}}/src/sex_matches.py
+-rw-r--r--   0        0        0     2415 2023-06-22 12:16:49.814338 datazimmer-0.5.3/dogshow/projects/cc-dogsuccess/{{cookiecutter.project}}/src/success.py
+-rw-r--r--   0        0        0      810 2023-06-22 12:16:49.814338 datazimmer-0.5.3/dogshow/projects/cc-dogsuccess/{{cookiecutter.project}}/src/top_report.py
+-rw-r--r--   0        0        0      575 2023-06-22 12:16:49.814338 datazimmer-0.5.3/dogshow/projects/cc-dogsuccess/{{cookiecutter.project}}/zimmer.yaml
+-rw-r--r--   0        0        0     2940 2023-06-22 12:16:49.814338 datazimmer-0.5.3/dogshow/todo/complex_success.py
+-rw-r--r--   0        0        0      612 2023-06-22 12:16:49.814338 datazimmer-0.5.3/notebooks/doc-001-intro.ipynb
+-rw-r--r--   0        0        0     5328 2023-06-22 12:16:49.814338 datazimmer-0.5.3/notebooks/doc-002-glossary.ipynb
+-rw-r--r--   0        0        0     1877 2023-06-22 12:16:49.814338 datazimmer-0.5.3/notebooks/doc-003-mock-projects.ipynb
+-rw-r--r--   0        0        0     1928 2023-06-22 12:16:49.814338 datazimmer-0.5.3/notebooks/doc-004-rules-conventions.ipynb
+-rw-r--r--   0        0        0     1235 2023-06-22 12:16:49.814338 datazimmer-0.5.3/notebooks/doc-005-cli.ipynb
+-rw-r--r--   0        0        0     1120 2023-06-22 12:16:49.814338 datazimmer-0.5.3/pyproject.toml
+-rw-r--r--   0        0        0     4564 1970-01-01 00:00:00.000000 datazimmer-0.5.3/PKG-INFO
```

### Comparing `datazimmer-0.5.2/.github/workflows/compatibility_test.yml` & `datazimmer-0.5.3/.github/workflows/compatibility_test.yml`

 * *Files identical despite different names*

### Comparing `datazimmer-0.5.2/.github/workflows/test.yml` & `datazimmer-0.5.3/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `datazimmer-0.5.2/.github/workflows/twine_release.yml` & `datazimmer-0.5.3/.github/workflows/twine_release.yml`

 * *Files identical despite different names*

### Comparing `datazimmer-0.5.2/.gitignore` & `datazimmer-0.5.3/.gitignore`

 * *Files identical despite different names*

### Comparing `datazimmer-0.5.2/LICENSE` & `datazimmer-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `datazimmer-0.5.2/README.md` & `datazimmer-0.5.3/README.md`

 * *Files identical despite different names*

### Comparing `datazimmer-0.5.2/conftest.py` & `datazimmer-0.5.3/conftest.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 import pytest
 from aswan.constants import DEFAULT_REMOTE_ENV_VAR, DEPOT_ROOT_ENV_VAR
 from aswan.depot.remote import HEX_ENV, PW_ENV
 from zimmauth import ZimmAuth
 from zimmauth.core import LOCAL_HOST_NAMES_ENV_VAR
 
 from datazimmer.config_loading import RunConfig
+from datazimmer.dvc_util import run_dvc
 from datazimmer.naming import (
     AUTH_HEX_ENV_VAR,
     AUTH_PASS_ENV_VAR,
     DEFAULT_ENV_NAME,
     MAIN_MODULE_NAME,
     META_MODULE_NAME,
 )
@@ -48,16 +49,16 @@
     dvc_rem = tmp_dir / "dvc-rem"
     pname = "test-project"
     with cd_into(tmp_dir):
         check_call(["git", "init", "remote"])
         init(pname, git_remote=(tmp_dir / "remote").as_posix())
     pdir = tmp_dir / pname
     with cd_into(pdir):
-        check_call(["dvc", "remote", "add", "testrem", dvc_rem.as_posix()])
-        check_call(["dvc", "remote", "default", "testrem"])
+        run_dvc("remote", "add", "testrem", dvc_rem.as_posix())
+        run_dvc("remote", "default", "testrem")
         Path(MAIN_MODULE_NAME, "core.py").write_text(CORE_PY.read_text())
 
     with dz_ctx([pdir]):
         yield pdir
     gen_rmtree(tmp_dir)
```

### Comparing `datazimmer-0.5.2/datazimmer/__init__.py` & `datazimmer-0.5.3/datazimmer/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,8 +13,8 @@
 from .persistent_state import PersistentState
 from .pipeline_element import register, register_data_loader, register_env_creator
 from .project_runtime import dump_dfs_to_tables
 from .raw_data import get_raw_data_path
 from .reporting import ReportFile
 from .typer_commands import app
 
-__version__ = "0.5.2"
+__version__ = "0.5.3"
```

### Comparing `datazimmer-0.5.2/datazimmer/aswan_integration.py` & `datazimmer-0.5.3/datazimmer/aswan_integration.py`

 * *Files identical despite different names*

### Comparing `datazimmer-0.5.2/datazimmer/config_loading.py` & `datazimmer-0.5.3/datazimmer/config_loading.py`

 * *Files identical despite different names*

### Comparing `datazimmer-0.5.2/datazimmer/dvc_util.py` & `datazimmer-0.5.3/datazimmer/dvc_util.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,20 +5,19 @@
 import yaml
 from structlog import get_logger
 
 from .naming import BASE_CONF_PATH
 
 logger = get_logger("dvc-util")
 
-DVC_ENV = Path.home() / ".dvc-env"
-DVC_ENV_EXC = DVC_ENV / "bin" / "python"
+DVC_ENV_DIR = Path.home() / ".dvc-env"
 
 
 def setup_dvc(update: bool = False):
-    venv.create(DVC_ENV, system_site_packages=True)
+    venv.create(DVC_ENV_DIR, system_site_packages=True, with_pip=True)
     uarg = ("-U",) if update else ()
     _erun("-m", "pip", "install", *uarg, "dvc[ssh,s3]")
 
 
 def import_dvc(uri, path, out, rev=None, no_exec=False):
     comm = ["import", "-o", out]
     if rev:
@@ -88,9 +87,13 @@
 
 
 def run_dvc(*comm):
     logger.info("running dvc command", comm=comm)
     return _erun("-m", "dvc", *comm)
 
 
+def get_dvc_venv_exec():
+    return venv.EnvBuilder().ensure_directories(DVC_ENV_DIR).env_exec_cmd
+
+
 def _erun(*comm):
-    return check_output([DVC_ENV_EXC.as_posix(), *comm]).decode()
+    return check_output([get_dvc_venv_exec(), *comm]).decode()
```

### Comparing `datazimmer-0.5.2/datazimmer/get_runtime.py` & `datazimmer-0.5.3/datazimmer/get_runtime.py`

 * *Files identical despite different names*

### Comparing `datazimmer-0.5.2/datazimmer/gh_actions.py` & `datazimmer-0.5.3/datazimmer/gh_actions.py`

 * *Files identical despite different names*

### Comparing `datazimmer-0.5.2/datazimmer/metadata/atoms.py` & `datazimmer-0.5.3/datazimmer/metadata/atoms.py`

 * *Files identical despite different names*

### Comparing `datazimmer-0.5.2/datazimmer/metadata/complete_id.py` & `datazimmer-0.5.3/datazimmer/metadata/complete_id.py`

 * *Files identical despite different names*

### Comparing `datazimmer-0.5.2/datazimmer/metadata/datascript.py` & `datazimmer-0.5.3/datazimmer/metadata/datascript.py`

 * *Files identical despite different names*

### Comparing `datazimmer-0.5.2/datazimmer/metadata/high_level.py` & `datazimmer-0.5.3/datazimmer/metadata/high_level.py`

 * *Files identical despite different names*

### Comparing `datazimmer-0.5.2/datazimmer/metadata/scrutable.py` & `datazimmer-0.5.3/datazimmer/metadata/scrutable.py`

 * *Files identical despite different names*

### Comparing `datazimmer-0.5.2/datazimmer/naming.py` & `datazimmer-0.5.3/datazimmer/naming.py`

 * *Files identical despite different names*

### Comparing `datazimmer-0.5.2/datazimmer/persistent_state.py` & `datazimmer-0.5.3/datazimmer/persistent_state.py`

 * *Files identical despite different names*

### Comparing `datazimmer-0.5.2/datazimmer/pipeline_element.py` & `datazimmer-0.5.3/datazimmer/pipeline_element.py`

 * *Files identical despite different names*

### Comparing `datazimmer-0.5.2/datazimmer/project_runtime.py` & `datazimmer-0.5.3/datazimmer/project_runtime.py`

 * *Files identical despite different names*

### Comparing `datazimmer-0.5.2/datazimmer/raw_data.py` & `datazimmer-0.5.3/datazimmer/raw_data.py`

 * *Files identical despite different names*

### Comparing `datazimmer-0.5.2/datazimmer/registry.py` & `datazimmer-0.5.3/datazimmer/registry.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 import toml
 import yaml
 from flit.build import main
 from structlog import get_logger
 
 from .config_loading import get_full_auth
-from .dvc_util import DVC_ENV_EXC
+from .dvc_util import get_dvc_venv_exec
 from .metadata.high_level import PROJ_KEYS
 from .naming import (
     GIT_TOKEN_ENV_VAR,
     MAIN_MODULE_NAME,
     META_MODULE_NAME,
     PYV,
     REQUIREMENTS_FILE,
@@ -79,15 +79,15 @@
         ypath = self.paths.info_yaml_of(project_name, version)
         if ypath.exists():
             return yaml.safe_load(ypath.read_text())
         logger.warning(f"info for {project_name} {version} requested but not found")
 
     def full_build(self, global_conf=False):
         self.dump_info()
-        get_full_auth().dump_dvc(local=not global_conf, executable=DVC_ENV_EXC)
+        get_full_auth().dump_dvc(local=not global_conf, executable=get_dvc_venv_exec())
         if not self._is_released():
             self._package()
         if self.requires:
             self._install_no_server(self.requires)
 
     def update(self):
         self._git_run(pull=True)
```

### Comparing `datazimmer-0.5.2/datazimmer/reporting.py` & `datazimmer-0.5.3/datazimmer/reporting.py`

 * *Files identical despite different names*

### Comparing `datazimmer-0.5.2/datazimmer/sql/loader.py` & `datazimmer-0.5.3/datazimmer/sql/loader.py`

 * *Files identical despite different names*

### Comparing `datazimmer-0.5.2/datazimmer/tests/create_dogshow.py` & `datazimmer-0.5.3/datazimmer/tests/create_dogshow.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from pathlib import Path
 from subprocess import check_call
 
 from cookiecutter.main import generate_files
 from structlog import get_logger
 from yaml import safe_load
 
+from datazimmer.dvc_util import run_dvc
 from datazimmer.naming import BASE_CONF_PATH, MAIN_MODULE_NAME
 from datazimmer.typer_commands import init
 from datazimmer.utils import cd_into, gen_rmtree, git_run, package_root
 
 logger = get_logger()
 
 dogshow_root = package_root / "dogshow"
@@ -51,16 +52,16 @@
             self.local_root,
             overwrite_if_exists=True,
         )
         self.ran_dirs.append(root_dir)
         with cd_into(root_dir):
             sys.path.insert(0, Path.cwd().as_posix())
             for remote_name, remote_id in self.dvc_remotes:
-                check_call(["dvc", "remote", "add", remote_name, remote_id])
-            check_call(["dvc", "remote", "default", self.dvc_remotes[0][0]])
+                run_dvc("remote", "add", remote_name, remote_id)
+            run_dvc("remote", "default", self.dvc_remotes[0][0])
             git_run(add=["*"], msg=f"setup {name} project", push=True)
             pzen = _PRIVATE_ZEN.get(name, "")
             yield name, _VERSIONS.get(name, []), _RAW_IMPORTS.get(name, []), pzen
             sys.path.pop(0)
 
     def check_sdists(self):
         pass  # TODO check builds
```

### Comparing `datazimmer-0.5.2/datazimmer/tests/test_commands.py` & `datazimmer-0.5.3/datazimmer/tests/test_commands.py`

 * *Files identical despite different names*

### Comparing `datazimmer-0.5.2/datazimmer/tests/test_full_integration.py` & `datazimmer-0.5.3/datazimmer/tests/test_full_integration.py`

 * *Files identical despite different names*

### Comparing `datazimmer-0.5.2/datazimmer/tests/test_scrutable.py` & `datazimmer-0.5.3/datazimmer/tests/test_scrutable.py`

 * *Files identical despite different names*

### Comparing `datazimmer-0.5.2/datazimmer/tests/test_validation.py` & `datazimmer-0.5.3/datazimmer/tests/test_validation.py`

 * *Files identical despite different names*

### Comparing `datazimmer-0.5.2/datazimmer/tests/util.py` & `datazimmer-0.5.3/datazimmer/tests/util.py`

 * *Files identical despite different names*

### Comparing `datazimmer-0.5.2/datazimmer/typer_commands.py` & `datazimmer-0.5.3/datazimmer/typer_commands.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from typing import TYPE_CHECKING
 
 import typer
 from structlog import get_logger
 
 from . import dvc_util as dvcu
 from .config_loading import CONF_KEYS, Config, RunConfig, UserConfig
-from .dvc_util import setup_dvc
+from .dvc_util import run_dvc, setup_dvc
 from .exceptions import ProjectSetupException
 from .get_runtime import get_runtime
 from .gh_actions import write_aswan_crons, write_project_cron
 from .metadata.high_level import ProjectMetadata
 from .naming import (
     BASE_CONF_PATH,
     MAIN_MODULE_NAME,
@@ -289,15 +289,15 @@
         tag_env = env_from_tag(tag)
         if (env == tag_env) or not env:
             return tag_env, tag
     return None, None
 
 
 def _commit_dvc_default(remote):
-    check_call(["dvc", "remote", "default", remote])
+    run_dvc("remote", "default", remote)
     git_run(add=[".dvc"], msg=f"update dvc default remote to {remote}", check=True)
 
 
 def _dvc_commit(paths, msg):
     git_run(add=["*.gitignore", *[f"{p}.dvc" for p in paths]], msg=msg, check=True)
```

### Comparing `datazimmer-0.5.2/datazimmer/utils.py` & `datazimmer-0.5.3/datazimmer/utils.py`

 * *Files identical despite different names*

### Comparing `datazimmer-0.5.2/datazimmer/validation_functions.py` & `datazimmer-0.5.3/datazimmer/validation_functions.py`

 * *Files identical despite different names*

### Comparing `datazimmer-0.5.2/datazimmer/zenodo.py` & `datazimmer-0.5.3/datazimmer/zenodo.py`

 * *Files identical despite different names*

### Comparing `datazimmer-0.5.2/docs/api/datazimmer.DzAswan.rst` & `datazimmer-0.5.3/docs/api/datazimmer.DzAswan.rst`

 * *Files identical despite different names*

### Comparing `datazimmer-0.5.2/docs/api/datazimmer.EntityClass.rst` & `datazimmer-0.5.3/docs/api/datazimmer.EntityClass.rst`

 * *Files identical despite different names*

### Comparing `datazimmer-0.5.2/docs/api/datazimmer.ReportFile.rst` & `datazimmer-0.5.3/docs/api/datazimmer.ReportFile.rst`

 * *Files identical despite different names*

### Comparing `datazimmer-0.5.2/docs/api/datazimmer.ScruTable.rst` & `datazimmer-0.5.3/docs/api/datazimmer.ScruTable.rst`

 * *Files identical despite different names*

### Comparing `datazimmer-0.5.2/docs/conf.py` & `datazimmer-0.5.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `datazimmer-0.5.2/docs/notebooks/doc-002-glossary.rst` & `datazimmer-0.5.3/docs/notebooks/doc-002-glossary.rst`

 * *Files identical despite different names*

### Comparing `datazimmer-0.5.2/docs/notebooks/doc-003-mock-projects.rst` & `datazimmer-0.5.3/docs/notebooks/doc-003-mock-projects.rst`

 * *Files identical despite different names*

### Comparing `datazimmer-0.5.2/docs/notebooks/doc-004-rules-conventions.rst` & `datazimmer-0.5.3/docs/notebooks/doc-004-rules-conventions.rst`

 * *Files identical despite different names*

### Comparing `datazimmer-0.5.2/dogshow/data/photo.csv` & `datazimmer-0.5.3/dogshow/data/photo.csv`

 * *Files identical despite different names*

### Comparing `datazimmer-0.5.2/dogshow/minimal.py` & `datazimmer-0.5.3/dogshow/minimal.py`

 * *Files identical despite different names*

### Comparing `datazimmer-0.5.2/dogshow/projects/cc-dog-raw/{{cookiecutter.project}}/notebooks/create-dogshow-test-data.ipynb` & `datazimmer-0.5.3/dogshow/projects/cc-dog-raw/{{cookiecutter.project}}/notebooks/create-dogshow-test-data.ipynb`

 * *Files identical despite different names*

### Comparing `datazimmer-0.5.2/dogshow/projects/cc-dog-show/{{cookiecutter.project}}/src/core/create_envs.py` & `datazimmer-0.5.3/dogshow/projects/cc-dog-show/{{cookiecutter.project}}/src/core/create_envs.py`

 * *Files identical despite different names*

### Comparing `datazimmer-0.5.2/dogshow/projects/cc-dog-show/{{cookiecutter.project}}/src/core/ns_meta.py` & `datazimmer-0.5.3/dogshow/projects/cc-dog-show/{{cookiecutter.project}}/src/core/ns_meta.py`

 * *Files identical despite different names*

### Comparing `datazimmer-0.5.2/dogshow/projects/cc-dog-show/{{cookiecutter.project}}/src/core/update_data.py` & `datazimmer-0.5.3/dogshow/projects/cc-dog-show/{{cookiecutter.project}}/src/core/update_data.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,25 +18,34 @@
 
 def read_ext_csv(name, **kwargs) -> pd.DataFrame:
     return pd.read_csv(dz.get_raw_data_path(f"{name}.csv", "dog-raw"), **kwargs)
 
 
 class PhotoCollector(aswan.RequestHandler):
     def load_cache(self, _):
-        ps = PhotoState.load()
-        rng = random.Random(7 + ps.photos_loaded)
-        rel_df = read_ext_csv("rel").set_index(list(rel_renamer.keys()))
-        rec_part = partial(_get_prec, rdf=rel_df, rng=rng, n=ps.photos_loaded)
-        photo_df = pd.DataFrame(map(rec_part, range(PHOTO_INC))).set_index("photo_id")
-        raw_dir = dz.get_raw_data_path(f"b-{ps.photos_loaded}")
-        raw_dir.mkdir()
-        photo_df.to_markdown(raw_dir / "p.md")
-        return photo_df.rename(
-            columns={f"rel__{k}": f"rel__{v}" for k, v in rel_renamer.items()}
-        )
+        from structlog import get_logger
+
+        try:
+            return get_photos()
+        except Exception as e:
+            get_logger().exception(e)
+
+
+def get_photos():
+    ps = PhotoState.load()
+    rng = random.Random(7 + ps.photos_loaded)
+    rel_df = read_ext_csv("rel").set_index(list(rel_renamer.keys()))
+    rec_part = partial(_get_prec, rdf=rel_df, rng=rng, n=ps.photos_loaded)
+    photo_df = pd.DataFrame(map(rec_part, range(PHOTO_INC))).set_index("photo_id")
+    raw_dir = dz.get_raw_data_path(f"b-{ps.photos_loaded}")
+    raw_dir.mkdir()
+    photo_df.to_markdown(raw_dir / "p.md")
+    return photo_df.rename(
+        columns={f"rel__{k}": f"rel__{v}" for k, v in rel_renamer.items()}
+    )
 
 
 def _get_prec(i, rng: random.Random, rdf: pd.DataFrame, n: int):
     rels = {
         f"rel__{ind_id}": val
         for ind_id, val in zip(rdf.index.names, rng.choice(rdf.index))
     }
```

### Comparing `datazimmer-0.5.2/dogshow/projects/cc-dogcombine/{{cookiecutter.project}}/src/joint_success.py` & `datazimmer-0.5.3/dogshow/projects/cc-dogcombine/{{cookiecutter.project}}/src/joint_success.py`

 * *Files identical despite different names*

### Comparing `datazimmer-0.5.2/dogshow/projects/cc-dograce/{{cookiecutter.project}}/src/core.py` & `datazimmer-0.5.3/dogshow/projects/cc-dograce/{{cookiecutter.project}}/src/core.py`

 * *Files identical despite different names*

### Comparing `datazimmer-0.5.2/dogshow/projects/cc-dogsuccess/{{cookiecutter.project}}/src/counts/proc.py` & `datazimmer-0.5.3/dogshow/projects/cc-dogsuccess/{{cookiecutter.project}}/src/counts/proc.py`

 * *Files identical despite different names*

### Comparing `datazimmer-0.5.2/dogshow/projects/cc-dogsuccess/{{cookiecutter.project}}/src/sex_matches.py` & `datazimmer-0.5.3/dogshow/projects/cc-dogsuccess/{{cookiecutter.project}}/src/sex_matches.py`

 * *Files identical despite different names*

### Comparing `datazimmer-0.5.2/dogshow/projects/cc-dogsuccess/{{cookiecutter.project}}/src/success.py` & `datazimmer-0.5.3/dogshow/projects/cc-dogsuccess/{{cookiecutter.project}}/src/success.py`

 * *Files identical despite different names*

### Comparing `datazimmer-0.5.2/dogshow/projects/cc-dogsuccess/{{cookiecutter.project}}/src/top_report.py` & `datazimmer-0.5.3/dogshow/projects/cc-dogsuccess/{{cookiecutter.project}}/src/top_report.py`

 * *Files identical despite different names*

### Comparing `datazimmer-0.5.2/dogshow/projects/cc-dogsuccess/{{cookiecutter.project}}/zimmer.yaml` & `datazimmer-0.5.3/dogshow/projects/cc-dogsuccess/{{cookiecutter.project}}/zimmer.yaml`

 * *Files identical despite different names*

### Comparing `datazimmer-0.5.2/dogshow/todo/complex_success.py` & `datazimmer-0.5.3/dogshow/todo/complex_success.py`

 * *Files identical despite different names*

### Comparing `datazimmer-0.5.2/notebooks/doc-001-intro.ipynb` & `datazimmer-0.5.3/notebooks/doc-001-intro.ipynb`

 * *Files identical despite different names*

### Comparing `datazimmer-0.5.2/notebooks/doc-002-glossary.ipynb` & `datazimmer-0.5.3/notebooks/doc-002-glossary.ipynb`

 * *Files identical despite different names*

### Comparing `datazimmer-0.5.2/notebooks/doc-003-mock-projects.ipynb` & `datazimmer-0.5.3/notebooks/doc-003-mock-projects.ipynb`

 * *Files identical despite different names*

### Comparing `datazimmer-0.5.2/notebooks/doc-004-rules-conventions.ipynb` & `datazimmer-0.5.3/notebooks/doc-004-rules-conventions.ipynb`

 * *Files identical despite different names*

### Comparing `datazimmer-0.5.2/notebooks/doc-005-cli.ipynb` & `datazimmer-0.5.3/notebooks/doc-005-cli.ipynb`

 * *Files identical despite different names*

### Comparing `datazimmer-0.5.2/pyproject.toml` & `datazimmer-0.5.3/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 ]
 
 [project.optional-dependencies]
 collect = ["aswan[remote]>=0.4.2"]
 postgres = ["psycopg2"]
 profile = ["pyinstrument"]
 zenodo = ["requests", "markdown2"]
-test = ["branthebuilder", "zimmauth[test]", "atqo", "faker"]
+test = ["branthebuilder", "atqo", "faker", "moto", "boto3", "tabulate"]
 doc = ["branthebuilder[doc]"]
 [project.urls]
 Homepage = "https://github.com/sscu-budapest/datazimmer"
 
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
```

### Comparing `datazimmer-0.5.2/PKG-INFO` & `datazimmer-0.5.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datazimmer
-Version: 0.5.2
+Version: 0.5.3
 Summary: sscu-budapest utilities for scientific data engineering
 Author-email: Social Science Computing Unit Budapest <borza.endre@krtk.hu>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: flit
 Requires-Dist: wheel>=0.37.0
 Requires-Dist: pip>=22.0.0
@@ -22,17 +22,19 @@
 Requires-Dist: metazimmer
 Requires-Dist: zimmauth>=0.1.0
 Requires-Dist: aswan[remote]>=0.4.2 ; extra == "collect"
 Requires-Dist: branthebuilder[doc] ; extra == "doc"
 Requires-Dist: psycopg2 ; extra == "postgres"
 Requires-Dist: pyinstrument ; extra == "profile"
 Requires-Dist: branthebuilder ; extra == "test"
-Requires-Dist: zimmauth[test] ; extra == "test"
 Requires-Dist: atqo ; extra == "test"
 Requires-Dist: faker ; extra == "test"
+Requires-Dist: moto ; extra == "test"
+Requires-Dist: boto3 ; extra == "test"
+Requires-Dist: tabulate ; extra == "test"
 Requires-Dist: requests ; extra == "zenodo"
 Requires-Dist: markdown2 ; extra == "zenodo"
 Project-URL: Homepage, https://github.com/sscu-budapest/datazimmer
 Provides-Extra: collect
 Provides-Extra: doc
 Provides-Extra: postgres
 Provides-Extra: profile
```

