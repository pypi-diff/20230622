# Comparing `tmp/ase2sprkkr-2.1.0.tar.gz` & `tmp/ase2sprkkr-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ase2sprkkr-2.1.0.tar", last modified: Sun Jun 18 19:58:15 2023, max compression
+gzip compressed data, was "ase2sprkkr-2.1.1.tar", last modified: Thu Jun 22 18:02:23 2023, max compression
```

## Comparing `ase2sprkkr-2.1.0.tar` & `ase2sprkkr-2.1.1.tar`

### file list

```diff
@@ -1,178 +1,179 @@
-drwxrwxr-x   0 logik     (1000) logik     (1000)        0 2023-06-18 19:58:15.465288 ase2sprkkr-2.1.0/
--rw-rw-r--   0 logik     (1000) logik     (1000)     1074 2021-09-02 09:12:56.000000 ase2sprkkr-2.1.0/LICENCE
--rw-rw-r--   0 logik     (1000) logik     (1000)      110 2022-03-06 22:35:24.000000 ase2sprkkr-2.1.0/MANIFEST.in
--rw-rw-r--   0 logik     (1000) logik     (1000)     4830 2023-06-18 19:58:15.465288 ase2sprkkr-2.1.0/PKG-INFO
--rw-rw-r--   0 logik     (1000) logik     (1000)     4356 2023-03-30 16:14:13.000000 ase2sprkkr-2.1.0/README.md
--rw-rw-r--   0 logik     (1000) logik     (1000)      104 2021-09-02 09:12:56.000000 ase2sprkkr-2.1.0/pyproject.toml
--rw-rw-r--   0 logik     (1000) logik     (1000)      779 2023-06-18 19:58:15.465288 ase2sprkkr-2.1.0/setup.cfg
--rw-rw-r--   0 logik     (1000) logik     (1000)      256 2023-06-07 19:13:11.000000 ase2sprkkr-2.1.0/setup.py
-drwxrwxr-x   0 logik     (1000) logik     (1000)        0 2023-06-18 19:58:15.449288 ase2sprkkr-2.1.0/src/
--rw-rw-r--   0 logik     (1000) logik     (1000)        0 2021-02-10 09:12:38.000000 ase2sprkkr-2.1.0/src/MANIFEST.in
-drwxrwxr-x   0 logik     (1000) logik     (1000)        0 2023-06-18 19:58:15.449288 ase2sprkkr-2.1.0/src/ase2sprkkr/
--rw-rw-r--   0 logik     (1000) logik     (1000)      890 2023-06-18 15:04:21.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/__init__.py
-drwxrwxr-x   0 logik     (1000) logik     (1000)        0 2023-06-18 19:58:15.449288 ase2sprkkr-2.1.0/src/ase2sprkkr/ase/
--rw-rw-r--   0 logik     (1000) logik     (1000)        0 2023-02-11 17:57:59.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/ase/__init__.py
--rw-rw-r--   0 logik     (1000) logik     (1000)     8263 2023-03-28 14:31:52.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/ase/build.py
--rw-rw-r--   0 logik     (1000) logik     (1000)      286 2023-03-28 14:31:52.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/ase/pbc.py
--rw-rw-r--   0 logik     (1000) logik     (1000)     2370 2023-06-17 14:04:22.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/ase/symbols.py
--rw-rw-r--   0 logik     (1000) logik     (1000)     2373 2023-02-11 17:57:59.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/ase/visualise.py
-drwxrwxr-x   0 logik     (1000) logik     (1000)        0 2023-06-18 19:58:15.449288 ase2sprkkr-2.1.0/src/ase2sprkkr/asr/
--rw-rw-r--   0 logik     (1000) logik     (1000)      279 2023-06-08 07:39:18.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/asr/__init__.py
-drwxrwxr-x   0 logik     (1000) logik     (1000)        0 2023-06-18 19:58:15.449288 ase2sprkkr-2.1.0/src/ase2sprkkr/bindings/
--rw-rw-r--   0 logik     (1000) logik     (1000)       86 2023-01-27 00:17:47.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/bindings/__init__.py
--rw-rw-r--   0 logik     (1000) logik     (1000)     4892 2023-03-30 15:12:03.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/bindings/es_finder.py
--rw-rw-r--   0 logik     (1000) logik     (1000)     8391 2023-03-28 14:31:52.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/bindings/spglib.py
-drwxrwxr-x   0 logik     (1000) logik     (1000)        0 2023-06-18 19:58:15.453288 ase2sprkkr-2.1.0/src/ase2sprkkr/common/
--rw-rw-r--   0 logik     (1000) logik     (1000)       66 2022-03-06 17:00:17.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/common/__init__.py
--rw-rw-r--   0 logik     (1000) logik     (1000)     1097 2023-03-28 14:31:52.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/common/alternative_types.py
--rw-rw-r--   0 logik     (1000) logik     (1000)     5389 2023-03-28 14:31:52.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/common/configuration.py
--rw-rw-r--   0 logik     (1000) logik     (1000)    18435 2023-06-18 18:27:59.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/common/configuration_containers.py
--rw-rw-r--   0 logik     (1000) logik     (1000)    43224 2023-06-18 18:16:18.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/common/configuration_definitions.py
--rw-rw-r--   0 logik     (1000) logik     (1000)    10044 2023-06-18 12:13:29.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/common/decorators.py
--rw-rw-r--   0 logik     (1000) logik     (1000)     1348 2023-03-30 15:12:03.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/common/directory.py
--rw-rw-r--   0 logik     (1000) logik     (1000)      512 2023-03-28 14:31:52.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/common/doc.py
--rw-rw-r--   0 logik     (1000) logik     (1000)     1114 2023-01-27 00:17:47.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/common/formats.py
--rw-rw-r--   0 logik     (1000) logik     (1000)     2906 2023-06-18 18:17:15.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/common/generated_configuration_definitions.py
--rw-rw-r--   0 logik     (1000) logik     (1000)     2858 2022-12-05 17:02:51.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/common/grammar.py
-drwxrwxr-x   0 logik     (1000) logik     (1000)        0 2023-06-18 19:58:15.453288 ase2sprkkr-2.1.0/src/ase2sprkkr/common/grammar_types/
--rw-rw-r--   0 logik     (1000) logik     (1000)     1490 2023-06-16 20:05:37.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/common/grammar_types/__init__.py
--rw-rw-r--   0 logik     (1000) logik     (1000)    16245 2023-06-18 19:18:28.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/common/grammar_types/arrays.py
--rw-rw-r--   0 logik     (1000) logik     (1000)    10886 2023-06-18 11:03:15.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/common/grammar_types/basic.py
--rw-rw-r--   0 logik     (1000) logik     (1000)     1734 2023-06-18 19:18:28.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/common/grammar_types/data.py
--rw-rw-r--   0 logik     (1000) logik     (1000)        1 2023-06-15 07:45:04.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/common/grammar_types/functions.py
--rw-rw-r--   0 logik     (1000) logik     (1000)    16998 2023-06-18 19:18:28.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/common/grammar_types/grammar_type.py
--rw-rw-r--   0 logik     (1000) logik     (1000)     3624 2023-06-18 18:25:56.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/common/grammar_types/mixed.py
--rw-rw-r--   0 logik     (1000) logik     (1000)     2804 2023-03-28 14:31:52.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/common/init_tests.py
--rw-rw-r--   0 logik     (1000) logik     (1000)     1608 2023-03-28 14:31:52.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/common/misc.py
--rw-rw-r--   0 logik     (1000) logik     (1000)     2221 2023-03-28 14:31:52.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/common/no_output.py
--rw-rw-r--   0 logik     (1000) logik     (1000)    16385 2023-06-18 19:48:21.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/common/options.py
--rw-rw-r--   0 logik     (1000) logik     (1000)     6382 2022-09-04 15:14:59.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/common/process_output_reader.py
-drwxrwxr-x   0 logik     (1000) logik     (1000)        0 2023-06-18 19:58:15.453288 ase2sprkkr-2.1.0/src/ase2sprkkr/common/test/
--rw-rw-r--   0 logik     (1000) logik     (1000)        0 2022-03-06 22:35:24.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/common/test/__init__.py
--rw-rw-r--   0 logik     (1000) logik     (1000)     2804 2023-03-28 14:31:52.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/common/test/init_tests.py
--rw-rw-r--   0 logik     (1000) logik     (1000)     3395 2023-06-18 12:18:11.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/common/test/test_common.py
--rw-rw-r--   0 logik     (1000) logik     (1000)     8125 2023-03-28 14:31:52.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/common/test/test_grammar_types.py
--rw-rw-r--   0 logik     (1000) logik     (1000)      927 2023-06-17 12:20:25.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/common/tools.py
--rw-rw-r--   0 logik     (1000) logik     (1000)     6798 2023-03-28 14:31:52.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/common/unique_values.py
-drwxrwxr-x   0 logik     (1000) logik     (1000)        0 2023-06-18 19:58:15.453288 ase2sprkkr-2.1.0/src/ase2sprkkr/input_parameters/
--rw-rw-r--   0 logik     (1000) logik     (1000)       78 2022-03-06 22:35:24.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/input_parameters/__init__.py
-drwxrwxr-x   0 logik     (1000) logik     (1000)        0 2023-06-18 19:58:15.453288 ase2sprkkr-2.1.0/src/ase2sprkkr/input_parameters/definitions/
--rw-rw-r--   0 logik     (1000) logik     (1000)      369 2023-03-28 14:31:52.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/input_parameters/definitions/__init__.py
--rw-rw-r--   0 logik     (1000) logik     (1000)     5645 2023-06-18 19:34:47.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/input_parameters/definitions/arpes.py
--rw-rw-r--   0 logik     (1000) logik     (1000)      690 2023-03-28 14:31:52.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/input_parameters/definitions/dos.py
--rw-rw-r--   0 logik     (1000) logik     (1000)     2279 2023-06-18 11:00:14.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/input_parameters/definitions/gilbert.py
--rw-rw-r--   0 logik     (1000) logik     (1000)      659 2023-03-28 14:31:52.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/input_parameters/definitions/phagen.py
--rw-rw-r--   0 logik     (1000) logik     (1000)      746 2023-03-28 14:31:52.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/input_parameters/definitions/scf.py
--rw-rw-r--   0 logik     (1000) logik     (1000)    10536 2023-06-18 19:33:50.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/input_parameters/definitions/sections.py
-drwxrwxr-x   0 logik     (1000) logik     (1000)        0 2023-06-18 19:58:15.453288 ase2sprkkr-2.1.0/src/ase2sprkkr/input_parameters/examples/
--rw-rw-r--   0 logik     (1000) logik     (1000)      726 2022-03-06 17:00:17.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/input_parameters/examples/arpes.in
--rw-rw-r--   0 logik     (1000) logik     (1000)      210 2022-03-06 17:00:17.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/input_parameters/examples/dos.in
--rw-rw-r--   0 logik     (1000) logik     (1000)      266 2022-03-06 17:00:17.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/input_parameters/examples/phagen.in
--rw-rw-r--   0 logik     (1000) logik     (1000)      276 2022-03-06 17:00:17.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/input_parameters/examples/scf.in
--rw-rw-r--   0 logik     (1000) logik     (1000)    13384 2023-06-18 14:47:44.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/input_parameters/input_parameters.py
--rw-rw-r--   0 logik     (1000) logik     (1000)     4541 2023-06-18 11:35:58.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/input_parameters/input_parameters_definitions.py
-drwxrwxr-x   0 logik     (1000) logik     (1000)        0 2023-06-18 19:58:15.453288 ase2sprkkr-2.1.0/src/ase2sprkkr/input_parameters/test/
--rw-rw-r--   0 logik     (1000) logik     (1000)        0 2022-03-06 17:00:17.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/input_parameters/test/__init__.py
--rw-rw-r--   0 logik     (1000) logik     (1000)     2804 2023-03-28 14:31:52.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/input_parameters/test/init_tests.py
--rw-rw-r--   0 logik     (1000) logik     (1000)     2162 2023-06-18 19:55:56.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/input_parameters/test/test_definitions.py
--rw-rw-r--   0 logik     (1000) logik     (1000)    12772 2023-06-18 18:40:47.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/input_parameters/test/test_input_parameters.py
-drwxrwxr-x   0 logik     (1000) logik     (1000)        0 2023-06-18 19:58:15.453288 ase2sprkkr-2.1.0/src/ase2sprkkr/outputs/
--rw-rw-r--   0 logik     (1000) logik     (1000)       67 2022-03-14 23:27:47.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/outputs/__init__.py
--rw-rw-r--   0 logik     (1000) logik     (1000)     2128 2023-03-28 14:31:52.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/outputs/output_definitions.py
-drwxrwxr-x   0 logik     (1000) logik     (1000)        0 2023-06-18 19:58:15.457288 ase2sprkkr-2.1.0/src/ase2sprkkr/outputs/output_files/
--rw-rw-r--   0 logik     (1000) logik     (1000)     2036 2023-06-16 20:42:06.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/outputs/output_files/__init__.py
--rw-rw-r--   0 logik     (1000) logik     (1000)     3489 2023-06-18 19:18:42.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/outputs/output_files/spc.py
--rw-rw-r--   0 logik     (1000) logik     (1000)     3413 2023-06-16 19:09:52.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/outputs/output_files_definitions.py
-drwxrwxr-x   0 logik     (1000) logik     (1000)        0 2023-06-18 19:58:15.457288 ase2sprkkr-2.1.0/src/ase2sprkkr/outputs/readers/
--rw-rw-r--   0 logik     (1000) logik     (1000)       50 2022-03-14 23:27:47.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/outputs/readers/__init__.py
--rw-rw-r--   0 logik     (1000) logik     (1000)      968 2023-06-18 13:35:35.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/outputs/readers/arpes.py
--rw-rw-r--   0 logik     (1000) logik     (1000)      295 2023-03-28 14:31:52.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/outputs/readers/default.py
--rw-rw-r--   0 logik     (1000) logik     (1000)     8303 2023-06-18 07:50:22.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/outputs/readers/scf.py
--rw-rw-r--   0 logik     (1000) logik     (1000)     1649 2023-03-28 14:31:52.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/outputs/task_result.py
-drwxrwxr-x   0 logik     (1000) logik     (1000)        0 2023-06-18 19:58:15.457288 ase2sprkkr-2.1.0/src/ase2sprkkr/outputs/test/
--rw-rw-r--   0 logik     (1000) logik     (1000)        0 2022-03-11 17:30:24.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/outputs/test/__init__.py
--rw-rw-r--   0 logik     (1000) logik     (1000)     2804 2023-03-28 14:31:52.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/outputs/test/init_tests.py
--rw-rw-r--   0 logik     (1000) logik     (1000)     1034 2023-06-18 19:18:42.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/outputs/test/test_files.py
--rw-rw-r--   0 logik     (1000) logik     (1000)      985 2022-03-06 22:35:24.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/outputs/test/test_output.py
-drwxrwxr-x   0 logik     (1000) logik     (1000)        0 2023-06-18 19:58:15.457288 ase2sprkkr-2.1.0/src/ase2sprkkr/physics/
--rw-rw-r--   0 logik     (1000) logik     (1000)      101 2023-01-27 00:17:47.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/physics/__init__.py
--rw-rw-r--   0 logik     (1000) logik     (1000)     9561 2023-03-28 14:31:52.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/physics/lattice_data.py
--rw-rw-r--   0 logik     (1000) logik     (1000)     1865 2023-03-30 15:12:03.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/physics/winger_seitz_radii.py
-drwxrwxr-x   0 logik     (1000) logik     (1000)        0 2023-06-18 19:58:15.457288 ase2sprkkr-2.1.0/src/ase2sprkkr/potentials/
--rw-rw-r--   0 logik     (1000) logik     (1000)       84 2022-03-06 22:35:24.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/potentials/__init__.py
--rw-rw-r--   0 logik     (1000) logik     (1000)     2989 2023-03-28 14:31:52.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/potentials/custom_potential_section.py
-drwxrwxr-x   0 logik     (1000) logik     (1000)        0 2023-06-18 19:58:15.457288 ase2sprkkr-2.1.0/src/ase2sprkkr/potentials/definitions/
--rw-rw-r--   0 logik     (1000) logik     (1000)      334 2023-03-28 14:31:52.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/potentials/definitions/__init__.py
--rw-rw-r--   0 logik     (1000) logik     (1000)     3186 2023-03-28 14:31:52.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/potentials/definitions/potential.py
-drwxrwxr-x   0 logik     (1000) logik     (1000)        0 2023-06-18 19:58:15.457288 ase2sprkkr-2.1.0/src/ase2sprkkr/potentials/definitions/sections/
--rw-rw-r--   0 logik     (1000) logik     (1000)      531 2022-03-11 17:30:24.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/potentials/definitions/sections/__init__.py
--rw-rw-r--   0 logik     (1000) logik     (1000)      900 2022-09-04 19:42:44.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/potentials/definitions/sections/global_system_parameter.py
--rw-rw-r--   0 logik     (1000) logik     (1000)     7295 2023-03-28 14:31:52.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/potentials/definitions/sections/lattice.py
--rw-rw-r--   0 logik     (1000) logik     (1000)      998 2022-09-04 19:42:44.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/potentials/definitions/sections/mesh_information.py
--rw-rw-r--   0 logik     (1000) logik     (1000)     2748 2023-03-28 14:31:52.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/potentials/definitions/sections/occupation.py
--rw-rw-r--   0 logik     (1000) logik     (1000)     1326 2023-03-28 14:31:52.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/potentials/definitions/sections/reference_system.py
--rw-rw-r--   0 logik     (1000) logik     (1000)     2012 2023-03-28 14:31:52.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/potentials/definitions/sections/sites.py
--rw-rw-r--   0 logik     (1000) logik     (1000)      833 2022-09-04 19:42:44.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/potentials/definitions/sections/types.py
-drwxrwxr-x   0 logik     (1000) logik     (1000)        0 2023-06-18 19:58:15.461288 ase2sprkkr-2.1.0/src/ase2sprkkr/potentials/examples/
--rw-rw-r--   0 logik     (1000) logik     (1000)   265591 2022-03-06 22:35:24.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/potentials/examples/FePt.new.pot
--rw-rw-r--   0 logik     (1000) logik     (1000)     3894 2022-03-06 22:35:24.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/potentials/examples/FePt.pot
--rw-rw-r--   0 logik     (1000) logik     (1000)    22581 2023-03-28 14:31:52.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/potentials/examples/GeTe.pot
--rw-rw-r--   0 logik     (1000) logik     (1000)   263365 2022-03-06 22:35:24.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/potentials/examples/Li_scf.new.pot
--rw-rw-r--   0 logik     (1000) logik     (1000)     9591 2022-03-06 22:35:24.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/potentials/examples/fp_basscale0.pot
--rw-rw-r--   0 logik     (1000) logik     (1000)   395148 2022-03-06 22:35:24.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/potentials/examples/fp_new.pot
--rw-rw-r--   0 logik     (1000) logik     (1000)     5137 2023-03-28 14:31:52.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/potentials/potential_definitions.py
--rw-rw-r--   0 logik     (1000) logik     (1000)     5236 2023-03-28 14:31:52.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/potentials/potential_sections.py
--rw-rw-r--   0 logik     (1000) logik     (1000)     4062 2023-03-28 14:31:52.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/potentials/potentials.py
-drwxrwxr-x   0 logik     (1000) logik     (1000)        0 2023-06-18 19:58:15.461288 ase2sprkkr-2.1.0/src/ase2sprkkr/potentials/test/
--rw-rw-r--   0 logik     (1000) logik     (1000)        0 2022-03-06 22:35:24.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/potentials/test/__init__.py
--rw-rw-r--   0 logik     (1000) logik     (1000)     2804 2023-03-28 14:31:52.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/potentials/test/init_tests.py
--rw-rw-r--   0 logik     (1000) logik     (1000)     1156 2023-03-28 14:31:52.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/potentials/test/test_2D.py
--rw-rw-r--   0 logik     (1000) logik     (1000)     2135 2022-03-06 22:35:24.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/potentials/test/test_custom_section.py
--rw-rw-r--   0 logik     (1000) logik     (1000)     3880 2023-03-28 14:31:52.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/potentials/test/test_potential.py
--rw-rw-r--   0 logik     (1000) logik     (1000)     1334 2022-09-04 19:42:44.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/potentials/test/test_structure.py
-drwxrwxr-x   0 logik     (1000) logik     (1000)        0 2023-06-18 19:58:15.461288 ase2sprkkr-2.1.0/src/ase2sprkkr/sprkkr/
--rw-rw-r--   0 logik     (1000) logik     (1000)      112 2022-03-06 17:00:17.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/sprkkr/__init__.py
--rw-rw-r--   0 logik     (1000) logik     (1000)     6553 2023-03-28 14:31:52.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/sprkkr/atomic_types.py
--rw-rw-r--   0 logik     (1000) logik     (1000)     5136 2023-03-30 15:12:03.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/sprkkr/atoms_region.py
--rw-rw-r--   0 logik     (1000) logik     (1000)     3799 2023-03-28 14:31:52.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/sprkkr/build.py
--rw-rw-r--   0 logik     (1000) logik     (1000)    37563 2023-06-18 19:18:42.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/sprkkr/calculator.py
--rw-rw-r--   0 logik     (1000) logik     (1000)     4381 2023-03-28 14:31:52.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/sprkkr/configuration.py
--rw-rw-r--   0 logik     (1000) logik     (1000)     2210 2023-03-28 14:31:52.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/sprkkr/io_data.py
--rw-rw-r--   0 logik     (1000) logik     (1000)     7669 2023-03-28 14:31:52.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/sprkkr/occupations.py
--rw-rw-r--   0 logik     (1000) logik     (1000)      912 2022-03-14 23:27:47.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/sprkkr/radial_meshes.py
--rw-rw-r--   0 logik     (1000) logik     (1000)      328 2022-03-14 23:18:04.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/sprkkr/reference_systems.py
--rw-rw-r--   0 logik     (1000) logik     (1000)     5323 2023-03-28 14:31:52.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/sprkkr/sites.py
--rw-rw-r--   0 logik     (1000) logik     (1000)    13056 2023-03-28 14:31:52.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/sprkkr/sprkkr_atoms.py
--rw-rw-r--   0 logik     (1000) logik     (1000)      802 2023-03-28 14:31:52.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/sprkkr/sprkkr_grammar_types.py
--rw-rw-r--   0 logik     (1000) logik     (1000)     5647 2023-02-11 17:57:59.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/sprkkr/structure.py
--rw-rw-r--   0 logik     (1000) logik     (1000)     7511 2023-03-28 14:31:52.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/sprkkr/sysfile.py
-drwxrwxr-x   0 logik     (1000) logik     (1000)        0 2023-06-18 19:58:15.461288 ase2sprkkr-2.1.0/src/ase2sprkkr/sprkkr/test/
--rw-rw-r--   0 logik     (1000) logik     (1000)        0 2022-03-06 22:35:24.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/sprkkr/test/__init__.py
--rw-rw-r--   0 logik     (1000) logik     (1000)     2804 2023-03-28 14:31:52.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/sprkkr/test/init_tests.py
--rw-rw-r--   0 logik     (1000) logik     (1000)     1394 2023-06-18 13:46:33.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/sprkkr/test/test_arpes.py
--rw-rw-r--   0 logik     (1000) logik     (1000)      676 2023-03-28 14:31:52.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/sprkkr/test/test_build.py
--rw-rw-r--   0 logik     (1000) logik     (1000)     6989 2023-06-18 14:32:45.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/sprkkr/test/test_calculator.py
--rw-rw-r--   0 logik     (1000) logik     (1000)     1965 2023-03-28 14:31:52.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/sprkkr/test/test_sites.py
--rw-rw-r--   0 logik     (1000) logik     (1000)     3824 2023-03-28 14:31:52.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/sprkkr/test/test_sprkkr_atoms.py
--rw-rw-r--   0 logik     (1000) logik     (1000)     2537 2023-03-28 14:31:52.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/sprkkr/test/test_sysfile.py
-drwxrwxr-x   0 logik     (1000) logik     (1000)        0 2023-06-18 19:58:15.461288 ase2sprkkr-2.1.0/src/ase2sprkkr/tools/
--rw-rw-r--   0 logik     (1000) logik     (1000)       55 2022-03-14 23:27:47.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/tools/__init__.py
--rwxrwxr-x   0 logik     (1000) logik     (1000)     1997 2023-06-18 12:07:20.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/tools/a2s_plot_output.py
--rwxrwxr-x   0 logik     (1000) logik     (1000)     2632 2023-02-11 17:57:59.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/tools/a2s_visualise_in_struct.py
-drwxrwxr-x   0 logik     (1000) logik     (1000)        0 2023-06-18 19:58:15.465288 ase2sprkkr-2.1.0/src/ase2sprkkr/tools/test/
--rw-rw-r--   0 logik     (1000) logik     (1000)        0 2023-02-11 17:57:59.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/tools/test/__init__.py
--rw-rw-r--   0 logik     (1000) logik     (1000)     2804 2023-03-28 14:31:52.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/tools/test/init_tests.py
--rw-rw-r--   0 logik     (1000) logik     (1000)      750 2023-02-11 17:57:59.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/tools/test/test_tools.py
--rw-rw-r--   0 logik     (1000) logik     (1000)      150 2023-06-18 19:19:01.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/version.py
-drwxrwxr-x   0 logik     (1000) logik     (1000)        0 2023-06-18 19:58:15.465288 ase2sprkkr-2.1.0/src/ase2sprkkr/visualise/
--rw-rw-r--   0 logik     (1000) logik     (1000)        0 2023-06-18 14:02:55.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/visualise/__init__.py
--rw-rw-r--   0 logik     (1000) logik     (1000)     6607 2023-06-17 12:11:09.000000 ase2sprkkr-2.1.0/src/ase2sprkkr/visualise/plot.py
-drwxrwxr-x   0 logik     (1000) logik     (1000)        0 2023-06-18 19:58:15.449288 ase2sprkkr-2.1.0/src/ase2sprkkr.egg-info/
--rw-rw-r--   0 logik     (1000) logik     (1000)     4830 2023-06-18 19:58:15.000000 ase2sprkkr-2.1.0/src/ase2sprkkr.egg-info/PKG-INFO
--rw-rw-r--   0 logik     (1000) logik     (1000)     6096 2023-06-18 19:58:15.000000 ase2sprkkr-2.1.0/src/ase2sprkkr.egg-info/SOURCES.txt
--rw-rw-r--   0 logik     (1000) logik     (1000)        1 2023-06-18 19:58:15.000000 ase2sprkkr-2.1.0/src/ase2sprkkr.egg-info/dependency_links.txt
--rw-rw-r--   0 logik     (1000) logik     (1000)       35 2023-06-18 19:58:15.000000 ase2sprkkr-2.1.0/src/ase2sprkkr.egg-info/requires.txt
--rw-rw-r--   0 logik     (1000) logik     (1000)       11 2023-06-18 19:58:15.000000 ase2sprkkr-2.1.0/src/ase2sprkkr.egg-info/top_level.txt
-drwxrwxr-x   0 logik     (1000) logik     (1000)        0 2023-06-18 19:58:15.465288 ase2sprkkr-2.1.0/tests/
--rw-rw-r--   0 logik     (1000) logik     (1000)     2838 2021-09-02 09:12:56.000000 ase2sprkkr-2.1.0/tests/test.py
--rw-rw-r--   0 logik     (1000) logik     (1000)      468 2021-09-02 09:12:56.000000 ase2sprkkr-2.1.0/tests/test_inputfile.py
+drwxrwxr-x   0 logik     (1000) logik     (1000)        0 2023-06-22 18:02:23.806183 ase2sprkkr-2.1.1/
+-rw-rw-r--   0 logik     (1000) logik     (1000)     1074 2021-09-02 09:12:56.000000 ase2sprkkr-2.1.1/LICENCE
+-rw-rw-r--   0 logik     (1000) logik     (1000)      110 2022-03-06 22:35:24.000000 ase2sprkkr-2.1.1/MANIFEST.in
+-rw-rw-r--   0 logik     (1000) logik     (1000)     4830 2023-06-22 18:02:23.806183 ase2sprkkr-2.1.1/PKG-INFO
+-rw-rw-r--   0 logik     (1000) logik     (1000)     4356 2023-03-30 16:14:13.000000 ase2sprkkr-2.1.1/README.md
+-rw-rw-r--   0 logik     (1000) logik     (1000)      104 2021-09-02 09:12:56.000000 ase2sprkkr-2.1.1/pyproject.toml
+-rw-rw-r--   0 logik     (1000) logik     (1000)      779 2023-06-22 18:02:23.806183 ase2sprkkr-2.1.1/setup.cfg
+-rw-rw-r--   0 logik     (1000) logik     (1000)      256 2023-06-07 19:13:11.000000 ase2sprkkr-2.1.1/setup.py
+drwxrwxr-x   0 logik     (1000) logik     (1000)        0 2023-06-22 18:02:23.778183 ase2sprkkr-2.1.1/src/
+-rw-rw-r--   0 logik     (1000) logik     (1000)        0 2021-02-10 09:12:38.000000 ase2sprkkr-2.1.1/src/MANIFEST.in
+drwxrwxr-x   0 logik     (1000) logik     (1000)        0 2023-06-22 18:02:23.778183 ase2sprkkr-2.1.1/src/ase2sprkkr/
+-rw-rw-r--   0 logik     (1000) logik     (1000)      890 2023-06-18 15:04:21.000000 ase2sprkkr-2.1.1/src/ase2sprkkr/__init__.py
+drwxrwxr-x   0 logik     (1000) logik     (1000)        0 2023-06-22 18:02:23.782183 ase2sprkkr-2.1.1/src/ase2sprkkr/ase/
+-rw-rw-r--   0 logik     (1000) logik     (1000)        0 2023-02-11 17:57:59.000000 ase2sprkkr-2.1.1/src/ase2sprkkr/ase/__init__.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)     8263 2023-03-28 14:31:52.000000 ase2sprkkr-2.1.1/src/ase2sprkkr/ase/build.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)      286 2023-03-28 14:31:52.000000 ase2sprkkr-2.1.1/src/ase2sprkkr/ase/pbc.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)     2371 2023-06-18 20:03:12.000000 ase2sprkkr-2.1.1/src/ase2sprkkr/ase/symbols.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)     2373 2023-02-11 17:57:59.000000 ase2sprkkr-2.1.1/src/ase2sprkkr/ase/visualise.py
+drwxrwxr-x   0 logik     (1000) logik     (1000)        0 2023-06-22 18:02:23.782183 ase2sprkkr-2.1.1/src/ase2sprkkr/asr/
+-rw-rw-r--   0 logik     (1000) logik     (1000)      279 2023-06-08 07:39:18.000000 ase2sprkkr-2.1.1/src/ase2sprkkr/asr/__init__.py
+drwxrwxr-x   0 logik     (1000) logik     (1000)        0 2023-06-22 18:02:23.782183 ase2sprkkr-2.1.1/src/ase2sprkkr/bindings/
+-rw-rw-r--   0 logik     (1000) logik     (1000)       86 2023-01-27 00:17:47.000000 ase2sprkkr-2.1.1/src/ase2sprkkr/bindings/__init__.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)     4892 2023-03-30 15:12:03.000000 ase2sprkkr-2.1.1/src/ase2sprkkr/bindings/es_finder.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)     8391 2023-03-28 14:31:52.000000 ase2sprkkr-2.1.1/src/ase2sprkkr/bindings/spglib.py
+drwxrwxr-x   0 logik     (1000) logik     (1000)        0 2023-06-22 18:02:23.786183 ase2sprkkr-2.1.1/src/ase2sprkkr/common/
+-rw-rw-r--   0 logik     (1000) logik     (1000)       66 2022-03-06 17:00:17.000000 ase2sprkkr-2.1.1/src/ase2sprkkr/common/__init__.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)     1097 2023-03-28 14:31:52.000000 ase2sprkkr-2.1.1/src/ase2sprkkr/common/alternative_types.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)     5388 2023-06-21 19:18:48.000000 ase2sprkkr-2.1.1/src/ase2sprkkr/common/configuration.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)    18601 2023-06-21 19:18:48.000000 ase2sprkkr-2.1.1/src/ase2sprkkr/common/configuration_containers.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)    43600 2023-06-21 21:10:51.000000 ase2sprkkr-2.1.1/src/ase2sprkkr/common/configuration_definitions.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)    10523 2023-06-21 10:24:02.000000 ase2sprkkr-2.1.1/src/ase2sprkkr/common/decorators.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)     1348 2023-03-30 15:12:03.000000 ase2sprkkr-2.1.1/src/ase2sprkkr/common/directory.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)      512 2023-03-28 14:31:52.000000 ase2sprkkr-2.1.1/src/ase2sprkkr/common/doc.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)     1114 2023-01-27 00:17:47.000000 ase2sprkkr-2.1.1/src/ase2sprkkr/common/formats.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)     3384 2023-06-21 19:18:47.000000 ase2sprkkr-2.1.1/src/ase2sprkkr/common/generated_configuration_definitions.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)     3070 2023-06-21 19:18:47.000000 ase2sprkkr-2.1.1/src/ase2sprkkr/common/grammar.py
+drwxrwxr-x   0 logik     (1000) logik     (1000)        0 2023-06-22 18:02:23.786183 ase2sprkkr-2.1.1/src/ase2sprkkr/common/grammar_types/
+-rw-rw-r--   0 logik     (1000) logik     (1000)     1490 2023-06-16 20:05:37.000000 ase2sprkkr-2.1.1/src/ase2sprkkr/common/grammar_types/__init__.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)    16292 2023-06-21 21:21:14.000000 ase2sprkkr-2.1.1/src/ase2sprkkr/common/grammar_types/arrays.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)    11278 2023-06-21 21:18:19.000000 ase2sprkkr-2.1.1/src/ase2sprkkr/common/grammar_types/basic.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)     3523 2023-06-21 19:18:48.000000 ase2sprkkr-2.1.1/src/ase2sprkkr/common/grammar_types/data.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)    16998 2023-06-21 21:11:00.000000 ase2sprkkr-2.1.1/src/ase2sprkkr/common/grammar_types/grammar_type.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)     3624 2023-06-21 20:52:51.000000 ase2sprkkr-2.1.1/src/ase2sprkkr/common/grammar_types/mixed.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)      252 2023-06-21 19:18:48.000000 ase2sprkkr-2.1.1/src/ase2sprkkr/common/grammar_types/warnings.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)     2804 2023-03-28 14:31:52.000000 ase2sprkkr-2.1.1/src/ase2sprkkr/common/init_tests.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)     1608 2023-03-28 14:31:52.000000 ase2sprkkr-2.1.1/src/ase2sprkkr/common/misc.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)     2221 2023-03-28 14:31:52.000000 ase2sprkkr-2.1.1/src/ase2sprkkr/common/no_output.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)    16736 2023-06-21 19:18:48.000000 ase2sprkkr-2.1.1/src/ase2sprkkr/common/options.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)     6382 2022-09-04 15:14:59.000000 ase2sprkkr-2.1.1/src/ase2sprkkr/common/process_output_reader.py
+drwxrwxr-x   0 logik     (1000) logik     (1000)        0 2023-06-22 18:02:23.786183 ase2sprkkr-2.1.1/src/ase2sprkkr/common/test/
+-rw-rw-r--   0 logik     (1000) logik     (1000)        0 2022-03-06 22:35:24.000000 ase2sprkkr-2.1.1/src/ase2sprkkr/common/test/__init__.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)     2804 2023-03-28 14:31:52.000000 ase2sprkkr-2.1.1/src/ase2sprkkr/common/test/init_tests.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)     3400 2023-06-18 20:10:52.000000 ase2sprkkr-2.1.1/src/ase2sprkkr/common/test/test_common.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)     9054 2023-06-21 21:31:02.000000 ase2sprkkr-2.1.1/src/ase2sprkkr/common/test/test_grammar_types.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)      927 2023-06-17 12:20:25.000000 ase2sprkkr-2.1.1/src/ase2sprkkr/common/tools.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)     6798 2023-03-28 14:31:52.000000 ase2sprkkr-2.1.1/src/ase2sprkkr/common/unique_values.py
+drwxrwxr-x   0 logik     (1000) logik     (1000)        0 2023-06-22 18:02:23.790183 ase2sprkkr-2.1.1/src/ase2sprkkr/input_parameters/
+-rw-rw-r--   0 logik     (1000) logik     (1000)       78 2022-03-06 22:35:24.000000 ase2sprkkr-2.1.1/src/ase2sprkkr/input_parameters/__init__.py
+drwxrwxr-x   0 logik     (1000) logik     (1000)        0 2023-06-22 18:02:23.790183 ase2sprkkr-2.1.1/src/ase2sprkkr/input_parameters/definitions/
+-rw-rw-r--   0 logik     (1000) logik     (1000)      369 2023-03-28 14:31:52.000000 ase2sprkkr-2.1.1/src/ase2sprkkr/input_parameters/definitions/__init__.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)     5673 2023-06-21 09:06:40.000000 ase2sprkkr-2.1.1/src/ase2sprkkr/input_parameters/definitions/arpes.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)      690 2023-03-28 14:31:52.000000 ase2sprkkr-2.1.1/src/ase2sprkkr/input_parameters/definitions/dos.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)     2279 2023-06-18 11:00:14.000000 ase2sprkkr-2.1.1/src/ase2sprkkr/input_parameters/definitions/gilbert.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)      659 2023-03-28 14:31:52.000000 ase2sprkkr-2.1.1/src/ase2sprkkr/input_parameters/definitions/phagen.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)      829 2023-06-21 20:40:27.000000 ase2sprkkr-2.1.1/src/ase2sprkkr/input_parameters/definitions/scf.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)    11417 2023-06-21 20:39:26.000000 ase2sprkkr-2.1.1/src/ase2sprkkr/input_parameters/definitions/sections.py
+drwxrwxr-x   0 logik     (1000) logik     (1000)        0 2023-06-22 18:02:23.790183 ase2sprkkr-2.1.1/src/ase2sprkkr/input_parameters/examples/
+-rw-rw-r--   0 logik     (1000) logik     (1000)      726 2022-03-06 17:00:17.000000 ase2sprkkr-2.1.1/src/ase2sprkkr/input_parameters/examples/arpes.in
+-rw-rw-r--   0 logik     (1000) logik     (1000)      210 2022-03-06 17:00:17.000000 ase2sprkkr-2.1.1/src/ase2sprkkr/input_parameters/examples/dos.in
+-rw-rw-r--   0 logik     (1000) logik     (1000)      266 2022-03-06 17:00:17.000000 ase2sprkkr-2.1.1/src/ase2sprkkr/input_parameters/examples/phagen.in
+-rw-rw-r--   0 logik     (1000) logik     (1000)      276 2022-03-06 17:00:17.000000 ase2sprkkr-2.1.1/src/ase2sprkkr/input_parameters/examples/scf.in
+-rw-rw-r--   0 logik     (1000) logik     (1000)    13384 2023-06-18 14:47:44.000000 ase2sprkkr-2.1.1/src/ase2sprkkr/input_parameters/input_parameters.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)     4541 2023-06-18 11:35:58.000000 ase2sprkkr-2.1.1/src/ase2sprkkr/input_parameters/input_parameters_definitions.py
+drwxrwxr-x   0 logik     (1000) logik     (1000)        0 2023-06-22 18:02:23.790183 ase2sprkkr-2.1.1/src/ase2sprkkr/input_parameters/test/
+-rw-rw-r--   0 logik     (1000) logik     (1000)        0 2022-03-06 17:00:17.000000 ase2sprkkr-2.1.1/src/ase2sprkkr/input_parameters/test/__init__.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)     2804 2023-03-28 14:31:52.000000 ase2sprkkr-2.1.1/src/ase2sprkkr/input_parameters/test/init_tests.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)     2162 2023-06-18 19:55:56.000000 ase2sprkkr-2.1.1/src/ase2sprkkr/input_parameters/test/test_definitions.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)    13606 2023-06-21 19:18:48.000000 ase2sprkkr-2.1.1/src/ase2sprkkr/input_parameters/test/test_input_parameters.py
+drwxrwxr-x   0 logik     (1000) logik     (1000)        0 2023-06-22 18:02:23.790183 ase2sprkkr-2.1.1/src/ase2sprkkr/outputs/
+-rw-rw-r--   0 logik     (1000) logik     (1000)       67 2022-03-14 23:27:47.000000 ase2sprkkr-2.1.1/src/ase2sprkkr/outputs/__init__.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)     2128 2023-03-28 14:31:52.000000 ase2sprkkr-2.1.1/src/ase2sprkkr/outputs/output_definitions.py
+drwxrwxr-x   0 logik     (1000) logik     (1000)        0 2023-06-22 18:02:23.794183 ase2sprkkr-2.1.1/src/ase2sprkkr/outputs/output_files/
+-rw-rw-r--   0 logik     (1000) logik     (1000)     4582 2023-06-21 19:18:48.000000 ase2sprkkr-2.1.1/src/ase2sprkkr/outputs/output_files/__init__.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)     4232 2023-06-21 19:18:48.000000 ase2sprkkr-2.1.1/src/ase2sprkkr/outputs/output_files/dos.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)     2767 2023-06-21 19:18:48.000000 ase2sprkkr-2.1.1/src/ase2sprkkr/outputs/output_files/spc.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)     3366 2023-06-21 19:18:48.000000 ase2sprkkr-2.1.1/src/ase2sprkkr/outputs/output_files_definitions.py
+drwxrwxr-x   0 logik     (1000) logik     (1000)        0 2023-06-22 18:02:23.794183 ase2sprkkr-2.1.1/src/ase2sprkkr/outputs/readers/
+-rw-rw-r--   0 logik     (1000) logik     (1000)       50 2022-03-14 23:27:47.000000 ase2sprkkr-2.1.1/src/ase2sprkkr/outputs/readers/__init__.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)      968 2023-06-18 13:35:35.000000 ase2sprkkr-2.1.1/src/ase2sprkkr/outputs/readers/arpes.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)      295 2023-03-28 14:31:52.000000 ase2sprkkr-2.1.1/src/ase2sprkkr/outputs/readers/default.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)     8303 2023-06-18 07:50:22.000000 ase2sprkkr-2.1.1/src/ase2sprkkr/outputs/readers/scf.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)     1649 2023-03-28 14:31:52.000000 ase2sprkkr-2.1.1/src/ase2sprkkr/outputs/task_result.py
+drwxrwxr-x   0 logik     (1000) logik     (1000)        0 2023-06-22 18:02:23.794183 ase2sprkkr-2.1.1/src/ase2sprkkr/outputs/test/
+-rw-rw-r--   0 logik     (1000) logik     (1000)        0 2022-03-11 17:30:24.000000 ase2sprkkr-2.1.1/src/ase2sprkkr/outputs/test/__init__.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)     2804 2023-03-28 14:31:52.000000 ase2sprkkr-2.1.1/src/ase2sprkkr/outputs/test/init_tests.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)     1327 2023-06-21 20:38:24.000000 ase2sprkkr-2.1.1/src/ase2sprkkr/outputs/test/test_files.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)      985 2022-03-06 22:35:24.000000 ase2sprkkr-2.1.1/src/ase2sprkkr/outputs/test/test_output.py
+drwxrwxr-x   0 logik     (1000) logik     (1000)        0 2023-06-22 18:02:23.794183 ase2sprkkr-2.1.1/src/ase2sprkkr/physics/
+-rw-rw-r--   0 logik     (1000) logik     (1000)      101 2023-01-27 00:17:47.000000 ase2sprkkr-2.1.1/src/ase2sprkkr/physics/__init__.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)     9561 2023-03-28 14:31:52.000000 ase2sprkkr-2.1.1/src/ase2sprkkr/physics/lattice_data.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)     1865 2023-03-30 15:12:03.000000 ase2sprkkr-2.1.1/src/ase2sprkkr/physics/winger_seitz_radii.py
+drwxrwxr-x   0 logik     (1000) logik     (1000)        0 2023-06-22 18:02:23.794183 ase2sprkkr-2.1.1/src/ase2sprkkr/potentials/
+-rw-rw-r--   0 logik     (1000) logik     (1000)       84 2022-03-06 22:35:24.000000 ase2sprkkr-2.1.1/src/ase2sprkkr/potentials/__init__.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)     2989 2023-03-28 14:31:52.000000 ase2sprkkr-2.1.1/src/ase2sprkkr/potentials/custom_potential_section.py
+drwxrwxr-x   0 logik     (1000) logik     (1000)        0 2023-06-22 18:02:23.794183 ase2sprkkr-2.1.1/src/ase2sprkkr/potentials/definitions/
+-rw-rw-r--   0 logik     (1000) logik     (1000)      334 2023-03-28 14:31:52.000000 ase2sprkkr-2.1.1/src/ase2sprkkr/potentials/definitions/__init__.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)     3186 2023-03-28 14:31:52.000000 ase2sprkkr-2.1.1/src/ase2sprkkr/potentials/definitions/potential.py
+drwxrwxr-x   0 logik     (1000) logik     (1000)        0 2023-06-22 18:02:23.798183 ase2sprkkr-2.1.1/src/ase2sprkkr/potentials/definitions/sections/
+-rw-rw-r--   0 logik     (1000) logik     (1000)      531 2022-03-11 17:30:24.000000 ase2sprkkr-2.1.1/src/ase2sprkkr/potentials/definitions/sections/__init__.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)      900 2022-09-04 19:42:44.000000 ase2sprkkr-2.1.1/src/ase2sprkkr/potentials/definitions/sections/global_system_parameter.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)     7295 2023-03-28 14:31:52.000000 ase2sprkkr-2.1.1/src/ase2sprkkr/potentials/definitions/sections/lattice.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)      998 2022-09-04 19:42:44.000000 ase2sprkkr-2.1.1/src/ase2sprkkr/potentials/definitions/sections/mesh_information.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)     2748 2023-03-28 14:31:52.000000 ase2sprkkr-2.1.1/src/ase2sprkkr/potentials/definitions/sections/occupation.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)     1326 2023-03-28 14:31:52.000000 ase2sprkkr-2.1.1/src/ase2sprkkr/potentials/definitions/sections/reference_system.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)     2012 2023-03-28 14:31:52.000000 ase2sprkkr-2.1.1/src/ase2sprkkr/potentials/definitions/sections/sites.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)      833 2022-09-04 19:42:44.000000 ase2sprkkr-2.1.1/src/ase2sprkkr/potentials/definitions/sections/types.py
+drwxrwxr-x   0 logik     (1000) logik     (1000)        0 2023-06-22 18:02:23.802183 ase2sprkkr-2.1.1/src/ase2sprkkr/potentials/examples/
+-rw-rw-r--   0 logik     (1000) logik     (1000)   265591 2022-03-06 22:35:24.000000 ase2sprkkr-2.1.1/src/ase2sprkkr/potentials/examples/FePt.new.pot
+-rw-rw-r--   0 logik     (1000) logik     (1000)     3894 2022-03-06 22:35:24.000000 ase2sprkkr-2.1.1/src/ase2sprkkr/potentials/examples/FePt.pot
+-rw-rw-r--   0 logik     (1000) logik     (1000)    22581 2023-03-28 14:31:52.000000 ase2sprkkr-2.1.1/src/ase2sprkkr/potentials/examples/GeTe.pot
+-rw-rw-r--   0 logik     (1000) logik     (1000)   263365 2022-03-06 22:35:24.000000 ase2sprkkr-2.1.1/src/ase2sprkkr/potentials/examples/Li_scf.new.pot
+-rw-rw-r--   0 logik     (1000) logik     (1000)     9591 2022-03-06 22:35:24.000000 ase2sprkkr-2.1.1/src/ase2sprkkr/potentials/examples/fp_basscale0.pot
+-rw-rw-r--   0 logik     (1000) logik     (1000)   395148 2022-03-06 22:35:24.000000 ase2sprkkr-2.1.1/src/ase2sprkkr/potentials/examples/fp_new.pot
+-rw-rw-r--   0 logik     (1000) logik     (1000)     5137 2023-03-28 14:31:52.000000 ase2sprkkr-2.1.1/src/ase2sprkkr/potentials/potential_definitions.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)     5236 2023-03-28 14:31:52.000000 ase2sprkkr-2.1.1/src/ase2sprkkr/potentials/potential_sections.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)     4062 2023-03-28 14:31:52.000000 ase2sprkkr-2.1.1/src/ase2sprkkr/potentials/potentials.py
+drwxrwxr-x   0 logik     (1000) logik     (1000)        0 2023-06-22 18:02:23.802183 ase2sprkkr-2.1.1/src/ase2sprkkr/potentials/test/
+-rw-rw-r--   0 logik     (1000) logik     (1000)        0 2022-03-06 22:35:24.000000 ase2sprkkr-2.1.1/src/ase2sprkkr/potentials/test/__init__.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)     2804 2023-03-28 14:31:52.000000 ase2sprkkr-2.1.1/src/ase2sprkkr/potentials/test/init_tests.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)     1156 2023-03-28 14:31:52.000000 ase2sprkkr-2.1.1/src/ase2sprkkr/potentials/test/test_2D.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)     2135 2022-03-06 22:35:24.000000 ase2sprkkr-2.1.1/src/ase2sprkkr/potentials/test/test_custom_section.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)     3880 2023-03-28 14:31:52.000000 ase2sprkkr-2.1.1/src/ase2sprkkr/potentials/test/test_potential.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)     1334 2022-09-04 19:42:44.000000 ase2sprkkr-2.1.1/src/ase2sprkkr/potentials/test/test_structure.py
+drwxrwxr-x   0 logik     (1000) logik     (1000)        0 2023-06-22 18:02:23.806183 ase2sprkkr-2.1.1/src/ase2sprkkr/sprkkr/
+-rw-rw-r--   0 logik     (1000) logik     (1000)      112 2022-03-06 17:00:17.000000 ase2sprkkr-2.1.1/src/ase2sprkkr/sprkkr/__init__.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)     6553 2023-03-28 14:31:52.000000 ase2sprkkr-2.1.1/src/ase2sprkkr/sprkkr/atomic_types.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)     5136 2023-03-30 15:12:03.000000 ase2sprkkr-2.1.1/src/ase2sprkkr/sprkkr/atoms_region.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)     3799 2023-03-28 14:31:52.000000 ase2sprkkr-2.1.1/src/ase2sprkkr/sprkkr/build.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)    37563 2023-06-18 19:18:42.000000 ase2sprkkr-2.1.1/src/ase2sprkkr/sprkkr/calculator.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)     4381 2023-03-28 14:31:52.000000 ase2sprkkr-2.1.1/src/ase2sprkkr/sprkkr/configuration.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)     2210 2023-03-28 14:31:52.000000 ase2sprkkr-2.1.1/src/ase2sprkkr/sprkkr/io_data.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)     7669 2023-03-28 14:31:52.000000 ase2sprkkr-2.1.1/src/ase2sprkkr/sprkkr/occupations.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)      912 2022-03-14 23:27:47.000000 ase2sprkkr-2.1.1/src/ase2sprkkr/sprkkr/radial_meshes.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)      328 2022-03-14 23:18:04.000000 ase2sprkkr-2.1.1/src/ase2sprkkr/sprkkr/reference_systems.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)     5323 2023-03-28 14:31:52.000000 ase2sprkkr-2.1.1/src/ase2sprkkr/sprkkr/sites.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)    13056 2023-03-28 14:31:52.000000 ase2sprkkr-2.1.1/src/ase2sprkkr/sprkkr/sprkkr_atoms.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)      802 2023-03-28 14:31:52.000000 ase2sprkkr-2.1.1/src/ase2sprkkr/sprkkr/sprkkr_grammar_types.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)     5647 2023-02-11 17:57:59.000000 ase2sprkkr-2.1.1/src/ase2sprkkr/sprkkr/structure.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)     7511 2023-03-28 14:31:52.000000 ase2sprkkr-2.1.1/src/ase2sprkkr/sprkkr/sysfile.py
+drwxrwxr-x   0 logik     (1000) logik     (1000)        0 2023-06-22 18:02:23.806183 ase2sprkkr-2.1.1/src/ase2sprkkr/sprkkr/test/
+-rw-rw-r--   0 logik     (1000) logik     (1000)        0 2022-03-06 22:35:24.000000 ase2sprkkr-2.1.1/src/ase2sprkkr/sprkkr/test/__init__.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)     2804 2023-03-28 14:31:52.000000 ase2sprkkr-2.1.1/src/ase2sprkkr/sprkkr/test/init_tests.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)     1394 2023-06-18 13:46:33.000000 ase2sprkkr-2.1.1/src/ase2sprkkr/sprkkr/test/test_arpes.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)      676 2023-03-28 14:31:52.000000 ase2sprkkr-2.1.1/src/ase2sprkkr/sprkkr/test/test_build.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)     6989 2023-06-18 14:32:45.000000 ase2sprkkr-2.1.1/src/ase2sprkkr/sprkkr/test/test_calculator.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)     1965 2023-03-28 14:31:52.000000 ase2sprkkr-2.1.1/src/ase2sprkkr/sprkkr/test/test_sites.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)     3824 2023-03-28 14:31:52.000000 ase2sprkkr-2.1.1/src/ase2sprkkr/sprkkr/test/test_sprkkr_atoms.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)     2537 2023-03-28 14:31:52.000000 ase2sprkkr-2.1.1/src/ase2sprkkr/sprkkr/test/test_sysfile.py
+drwxrwxr-x   0 logik     (1000) logik     (1000)        0 2023-06-22 18:02:23.806183 ase2sprkkr-2.1.1/src/ase2sprkkr/tools/
+-rw-rw-r--   0 logik     (1000) logik     (1000)       55 2022-03-14 23:27:47.000000 ase2sprkkr-2.1.1/src/ase2sprkkr/tools/__init__.py
+-rwxrwxr-x   0 logik     (1000) logik     (1000)     2315 2023-06-21 19:18:48.000000 ase2sprkkr-2.1.1/src/ase2sprkkr/tools/a2s_plot_output.py
+-rwxrwxr-x   0 logik     (1000) logik     (1000)     2632 2023-02-11 17:57:59.000000 ase2sprkkr-2.1.1/src/ase2sprkkr/tools/a2s_visualise_in_struct.py
+drwxrwxr-x   0 logik     (1000) logik     (1000)        0 2023-06-22 18:02:23.806183 ase2sprkkr-2.1.1/src/ase2sprkkr/tools/test/
+-rw-rw-r--   0 logik     (1000) logik     (1000)        0 2023-02-11 17:57:59.000000 ase2sprkkr-2.1.1/src/ase2sprkkr/tools/test/__init__.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)     2804 2023-03-28 14:31:52.000000 ase2sprkkr-2.1.1/src/ase2sprkkr/tools/test/init_tests.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)      750 2023-02-11 17:57:59.000000 ase2sprkkr-2.1.1/src/ase2sprkkr/tools/test/test_tools.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)      150 2023-06-21 19:18:51.000000 ase2sprkkr-2.1.1/src/ase2sprkkr/version.py
+drwxrwxr-x   0 logik     (1000) logik     (1000)        0 2023-06-22 18:02:23.806183 ase2sprkkr-2.1.1/src/ase2sprkkr/visualise/
+-rw-rw-r--   0 logik     (1000) logik     (1000)        0 2023-06-18 14:02:55.000000 ase2sprkkr-2.1.1/src/ase2sprkkr/visualise/__init__.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)     8678 2023-06-21 21:24:18.000000 ase2sprkkr-2.1.1/src/ase2sprkkr/visualise/plot.py
+drwxrwxr-x   0 logik     (1000) logik     (1000)        0 2023-06-22 18:02:23.782183 ase2sprkkr-2.1.1/src/ase2sprkkr.egg-info/
+-rw-rw-r--   0 logik     (1000) logik     (1000)     4830 2023-06-22 18:02:23.000000 ase2sprkkr-2.1.1/src/ase2sprkkr.egg-info/PKG-INFO
+-rw-rw-r--   0 logik     (1000) logik     (1000)     6138 2023-06-22 18:02:23.000000 ase2sprkkr-2.1.1/src/ase2sprkkr.egg-info/SOURCES.txt
+-rw-rw-r--   0 logik     (1000) logik     (1000)        1 2023-06-22 18:02:23.000000 ase2sprkkr-2.1.1/src/ase2sprkkr.egg-info/dependency_links.txt
+-rw-rw-r--   0 logik     (1000) logik     (1000)       35 2023-06-22 18:02:23.000000 ase2sprkkr-2.1.1/src/ase2sprkkr.egg-info/requires.txt
+-rw-rw-r--   0 logik     (1000) logik     (1000)       11 2023-06-22 18:02:23.000000 ase2sprkkr-2.1.1/src/ase2sprkkr.egg-info/top_level.txt
+drwxrwxr-x   0 logik     (1000) logik     (1000)        0 2023-06-22 18:02:23.806183 ase2sprkkr-2.1.1/tests/
+-rw-rw-r--   0 logik     (1000) logik     (1000)     2838 2021-09-02 09:12:56.000000 ase2sprkkr-2.1.1/tests/test.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)      468 2021-09-02 09:12:56.000000 ase2sprkkr-2.1.1/tests/test_inputfile.py
```

### Comparing `ase2sprkkr-2.1.0/LICENCE` & `ase2sprkkr-2.1.1/LICENCE`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.1.0/PKG-INFO` & `ase2sprkkr-2.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ase2sprkkr
-Version: 2.1.0
+Version: 2.1.1
 Summary: ASE (atomic simulation environment) interface to SPRKKR
 Home-page: https://ase2sprkkr.github.io/ase2sprkkr/
 Author: Matyáš Novák & Jano Minár
 Author-email: ase2kkr@ntc.zcu.cz
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ase2sprkkr-2.1.0/README.md` & `ase2sprkkr-2.1.1/README.md`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.1.0/setup.cfg` & `ase2sprkkr-2.1.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.1.0/src/ase2sprkkr/__init__.py` & `ase2sprkkr-2.1.1/src/ase2sprkkr/__init__.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.1.0/src/ase2sprkkr/ase/build.py` & `ase2sprkkr-2.1.1/src/ase2sprkkr/ase/build.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.1.0/src/ase2sprkkr/ase/symbols.py` & `ase2sprkkr-2.1.1/src/ase2sprkkr/ase/symbols.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     """
     if not isinstance(symbols, Symbols):
         symbols = Symbols.fromsymbols(symbols)
     out = symbols.get_chemical_formula('reduce')
     if len(out) <= max_len:
        return out
     out = pretty_symbols(symbols)
-    out = re.sub("^\{([^}]*)\}[0-9]+$", r"\1", out)
+    out = re.sub(r"^\{([^}]*)\}[0-9]+$", r"\1", out)
     if len(out) <= max_len:
        return out
     out = symbols.get_chemical_formula()
     if len(out) <= max_len:
        return out
     return symbols.get_chemical_formula(empirical=True)
```

### Comparing `ase2sprkkr-2.1.0/src/ase2sprkkr/ase/visualise.py` & `ase2sprkkr-2.1.1/src/ase2sprkkr/ase/visualise.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.1.0/src/ase2sprkkr/bindings/es_finder.py` & `ase2sprkkr-2.1.1/src/ase2sprkkr/bindings/es_finder.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.1.0/src/ase2sprkkr/bindings/spglib.py` & `ase2sprkkr-2.1.1/src/ase2sprkkr/bindings/spglib.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.1.0/src/ase2sprkkr/common/alternative_types.py` & `ase2sprkkr-2.1.1/src/ase2sprkkr/common/alternative_types.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.1.0/src/ase2sprkkr/common/configuration.py` & `ase2sprkkr-2.1.1/src/ase2sprkkr/common/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -148,9 +148,8 @@
            out=self._save_to_file(file)
            file.flush()
       else:
          out=self._save_to_file(file)
          file.flush()
       return out
 
-
 _help_warning_printed=False
```

### Comparing `ase2sprkkr-2.1.0/src/ase2sprkkr/common/configuration_containers.py` & `ase2sprkkr-2.1.1/src/ase2sprkkr/common/configuration_containers.py`

 * *Files 2% similar despite different names*

```diff
@@ -448,14 +448,17 @@
 
       Returns
       -------
       something_have_been_written
         If any value have been written return True, otherwise return False.
       """
       d = self._definition
+      if d.write_condition and not d.write_condition(self):
+         return
+
       if d.is_expert:
           if not self.is_changed():
               return False
       else:
           if not self.has_any_value():
               return False
       if self._definition.name_in_grammar:
@@ -517,20 +520,24 @@
   """ Base class for data of configuration/problem-definition files
 
   In addition to container capabilities, it can read/write its data from/to file.
   """
 
   def _save_to_file(self, file):
       """ Implementation of the saving the configuration """
+      d = self._definition
+      if d.write_condition and not d.write_condition(self):
+         return
+
       it = iter(self)
       i = next(it)
       if i:
         i._save_to_file(file)
         for i in it:
-          file.write(self._definition.delimiter)
+          file.write(d.delimiter)
           i._save_to_file(file)
 
   def read_from_file(self, file, clear_first:bool=True, allow_dangerous:bool=False):
       """ Read data from a file
 
       Parameters
       ----------
```

### Comparing `ase2sprkkr-2.1.0/src/ase2sprkkr/common/configuration_definitions.py` & `ase2sprkkr-2.1.1/src/ase2sprkkr/common/configuration_definitions.py`

 * *Files 0% similar despite different names*

```diff
@@ -85,15 +85,16 @@
    the behavior.
    """
 
    def __init__(self, name, alternative_names=None,
                 is_optional=False, is_hidden=False, is_expert=False,
                 name_in_grammar=None, info=None, description=None,
                 write_alternative_name:bool=False,
-                result_class=None,
+                write_condition=None,
+                result_class=None
                 ):
        """
        Parameters
        ----------
         name: str
           Name of the value/section
 
@@ -122,16 +123,19 @@
 
         description: str
            The additional informations for the users.
 
         write_alternative_name
            Wheter use the name or the (first) alternative name in the output.
 
+        write_condition
+           If defined, write the value, only if write_condition(the option) is True.
+
         result_class
-           Redefine the class that holds data for this option/section
+           Redefine the class that holds data for this option/section.
        """
        self.name = name
        """ The name of the option/section """
        if isinstance(alternative_names, str):
           alternative_names = [ alternative_names ]
        self.alternative_names = alternative_names
        """ Alternative names of the option/section. The option/section can
@@ -139,14 +143,15 @@
        of the alternative names.
        """
        self.is_optional = is_optional
        self.is_expert = is_expert
        self.is_hidden = is_hidden
        """ Is it required part of configuration (or can it be ommited)? """
        self.write_alternative_name = write_alternative_name
+       self.write_condition = write_condition
        self.name_in_grammar = self.__class__.name_in_grammar \
                                if name_in_grammar is None else name_in_grammar
        self._info = info
        """ A short help text describing the content for the users. """
        self._description = description
        """ A longer help text describing the content for the users. """
        if result_class:
@@ -294,15 +299,16 @@
   name_in_grammar = None
 
   def __init__(self, name, type=None, default_value=None, alternative_names=None,
                fixed_value=None, required=None, info=None, description=None,
                is_hidden=False, is_optional=None, is_expert=False, is_numbered_array:bool=False,
                is_always_added:bool=None,
                name_in_grammar=None, name_format=None, expert=None,
-               write_alternative_name:bool=False, result_class=None,
+               write_alternative_name:bool=False, write_condition=None,
+               result_class=None,
                ):
     """
     Definition of a configuration value.
 
     Parameters
     ----------
     name: str
@@ -368,14 +374,17 @@
       If not None, set ``is_expert`` to True, ``default_value`` to the given value and
       ``required`` to False. Note, that also ``type`` can be determined from such given
       ``default_value``.
 
     write_alternative_name
        Wheter use the name or the (first) alternative name in the output.
 
+    write_condition
+       If defined, write the value, only if write_condition(the option) is True.
+
     result_class
        Redefine the class that holds data for this option/section
     """
     if expert is not None:
        if type is None:
           type = expert
        else:
@@ -421,14 +430,15 @@
          is_optional = is_optional,
          is_hidden = is_hidden,
          is_expert = is_expert,
          name_in_grammar = name_in_grammar,
          info=info,
          description = description,
          write_alternative_name = write_alternative_name,
+         write_condition = write_condition,
          result_class = result_class
     )
 
     if self.name_in_grammar is None:
         self.name_in_grammar = self.type.name_in_grammar
 
     self.is_numbered_array = is_numbered_array
@@ -617,15 +627,14 @@
      file
       The file to write to.
 
      value
       The value to write. It can be instance of DangerousValue, in such case
       It's own type is used to write the value.
      """
-
      if self.type.has_value:
         missing, df, np = self.type.missing_value()
 
      def write(name, value):
          if isinstance(value, DangerousValue):
             type = value.value_type
             value = value()
```

### Comparing `ase2sprkkr-2.1.0/src/ase2sprkkr/common/decorators.py` & `ase2sprkkr-2.1.1/src/ase2sprkkr/common/decorators.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """ Various decorators, mainly for class methods """
 import functools
 import itertools
 import inspect
 import heapq
 import asyncio
+import warnings
 
 if hasattr(functools,'cache'):
    cache = functools.cache
    """ Functools.cache. Python 3.8 and earlier does not have this method, so it is mocked for this version of python. """
 else:
    cache = functools.lru_cache(maxsize=None)
    """ Functools.cache. Python 3.8 and earlier does not have this method, so it is mocked for this version of python. """
@@ -307,7 +308,24 @@
 
     #@functools.wraps(function)
     def wrapper(function):
         function = decorator(function)
         return AddCalledClassAsArgument(function)
 
     return wrapper
+
+def warnings_from_here(stacklevel=1):
+    stacklevel+=1
+
+    def wrapper(func):
+
+       @functools.wraps(func)
+       def wrapped(*args, **kwargs):
+           with warnings.catch_warnings(record = True) as warning_list:
+               result = func(*args, **kwargs)
+           for warning in warning_list:
+               warnings.warn(warning.message, warning.category, stacklevel =stacklevel)
+           return result
+
+       return wrapped
+
+    return wrapper
```

### Comparing `ase2sprkkr-2.1.0/src/ase2sprkkr/common/directory.py` & `ase2sprkkr-2.1.1/src/ase2sprkkr/common/directory.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.1.0/src/ase2sprkkr/common/doc.py` & `ase2sprkkr-2.1.1/src/ase2sprkkr/common/doc.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.1.0/src/ase2sprkkr/common/formats.py` & `ase2sprkkr-2.1.1/src/ase2sprkkr/common/formats.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.1.0/src/ase2sprkkr/common/generated_configuration_definitions.py` & `ase2sprkkr-2.1.1/src/ase2sprkkr/common/generated_configuration_definitions.py`

 * *Files 23% similar despite different names*

```diff
@@ -22,18 +22,22 @@
       pass
 
 class GeneratedValueDefinition(BaseGeneratedValueDefinition):
 
    @add_to_signature(BaseDefinition.__init__, prepend=True)
    def __init__(self, name, getter, setter=None, **kwargs):
        super().__init__(name, **kwargs)
-       if getter is not None:
-           self.getter = getter
-       if setter is not None:
-           self.setter = setter
+       self.getter = getter
+       self._setter = setter
+
+   @property
+   def setter(self):
+       if not self._setter:
+           raise ValueError("Setting the value(s) of {self.name} is not allowed")
+       return self._setter
 
 class NumpyViewDefinition(BaseGeneratedValueDefinition):
    """
    Values described by this description are possibly reshaped views into a large
    "raw data array"
 
    Parameters
@@ -51,44 +55,55 @@
    shape
      The data will be reshaped to given shape. The dimension can be given
      either by number, or by names of other container variables. E.g.
      ``('NE', 5)``
    """
 
    @add_to_signature(BaseDefinition.__init__, prepend=True)
-   def __init__(self, name, data, selector=slice(None), shape=None, plot=None, *args, **kwargs):
+   def __init__(self, name, data, selector=slice(None),
+                shape=None, transpose=False, transform_key=None,
+                plot=None,
+                *args, **kwargs):
        super().__init__(name, *args, **kwargs)
        self.selector = selector
        self.shape = shape
        self.data = data
        self.plot = plot
+       self.transform_key=transform_key
+       self.transpose = transpose
 
-   def determine_shape(self, option):
+   def determine_shape(self, container):
        """ Return the shape of the resulting array, possibly computed using
        properties of the other values in the container"""
        def get(i):
            if isinstance(i, str):
-              return option._container[i]()
+              return container[i]()
            return i
        return tuple([get(i) for i in self.shape])
 
-   def source(self, option):
-       out=option._container[self.data]()[self.selector]
+   def source(self, container):
+       out=container[self.data]()[self.selector]
        if self.shape:
-          out.shape = self.determine_shape(option)
+          out.shape = self.determine_shape(container)
+       if self.transpose:
+          out = out.T
        return out
 
-   def getter(self, option, key=None):
-       out=self.source(option)
+   def getter(self, container, key=None):
+       out=self.source(container)
        if key is not None:
-          return out[key]
+          if self.transform_key:
+             key=self.transform_key(key, container)
+          out=out[key]
        return out
 
-   def setter(self, option, value, key=slice(None)):
-       self.source(option)[key]=value
+   def setter(self, container, value, key=slice(None)):
+       if self.transform_key:
+          key=self.transform_key(key, container)
+       self.source(container)[key]=value
 
    def enrich(self, option):
        if self.plot:
          option.plot = lambda **kwargs: self.plot(option, **kwargs)
          option.plot.__doc__ = " Plot the data."
 
    def copy_value(self, value, all_values=False):
```

### Comparing `ase2sprkkr-2.1.0/src/ase2sprkkr/common/grammar.py` & `ase2sprkkr-2.1.1/src/ase2sprkkr/common/grammar.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,22 +7,27 @@
 
 @contextmanager
 def generate_grammar():
     """ Set the pyparsing newline handling
         and then restore to the original state """
     try:
       old = None
+      kchars = None
       pe = pp.ParserElement
       if hasattr(pe, "DEFAULT_WHITE_CHARS"):
           old = pe.DEFAULT_WHITE_CHARS
+      if hasattr(pp.Keyword, "DEFAULT_KEYWORD_CHARS"):
+          kchars = pp.Keyword.DEFAULT_KEYWORD_CHARS + '-'
       pe.setDefaultWhitespaceChars(' \t\r')
       yield
     finally:
       if old is not None:
         pe.setDefaultWhitespaceChars(old)
+      if kchars is not None:
+        pp.Keyword.DEFAULT_KEYWORD_CHARS = kchars
 
 def replace_whitechars(expr):
     expr = expr.copy()
     expr.setWhitespaceChars(' \t\r')
     return expr
```

### Comparing `ase2sprkkr-2.1.0/src/ase2sprkkr/common/grammar_types/__init__.py` & `ase2sprkkr-2.1.1/src/ase2sprkkr/common/grammar_types/__init__.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.1.0/src/ase2sprkkr/common/grammar_types/arrays.py` & `ase2sprkkr-2.1.1/src/ase2sprkkr/common/grammar_types/arrays.py`

 * *Files 2% similar despite different names*

```diff
@@ -129,21 +129,23 @@
   def convert(self, value):
     if self.as_list:
        if callable(self.as_list):
           return value if isinstance(value, self.as_list) else self.as_list(value)
        else:
           return list(value) if isinstance(value, tuple) else value
     if not isinstance(value, np.ndarray):
-       if self.type.numpy_type == object:
-          #https://stackoverflow.com/questions/60939396/forcing-a-creation-of-1d-numpy-array-from-a-list-array-of-possibly-iterable-obje
-          out = np.empty(len(value), object)
-          out[:] = value
-          return out
+       if not hasattr(value, '__iter__'):
+           value = [ value ]
+           ln=1
        else:
-          return np.atleast_1d(value)
+           ln=len(value)
+       value = [ self.type.convert(i) for i in value ]
+       out = np.asarray(value)
+       return out
+
     return value
 
   is_the_same_value = staticmethod(compare_numpy_values)
 
 class SetOf(Array):
   """ Set of values of the same type. E.g. {1,2,3} """
 
@@ -287,29 +289,30 @@
   name_in_grammar = False
 
   def __init__(self, columns=None,
                      header=None, free_header=False,
                      format = {float: '>21.17', None: '>16'}, format_all=True,
                      numbering=None, numbering_label=None, numbering_format=True,
                      prefix=None, postfix=None, length=None,
-                     row_condition=None,
+                     row_condition=None, flatten=False,
                      default_values=False,
                      named_result = False, **kwargs):
       super().__init__(prefix=None, postfix=None)
       if columns is None:
          columns = kwargs
       if isinstance(columns, dict):
          self.names = list(columns.keys())
          columns = columns.values()
       else:
          self.names = None
       if header is None:
          header = self.names
       self.sequence = Sequence( *columns, format=format, format_all=format_all, condition = row_condition, default_values=default_values )
       self.header = header
+      self.flatten = flatten
       self.free_header = free_header
       if numbering.__class__ is str:
          numbering_label=numbering
          numbering=True
       self.numbering = Unsigned.I if numbering is True else numbering
       if self.numbering and numbering_format and not (numbering_format is True and self.numbering.format):
          if numbering_format is True:
@@ -353,14 +356,16 @@
              raise pp.ParseException(s, loc, 'First column should contain row numbering')
           return datas
 
       if self.numbering is not None:
          grammar.addParseAction(ensure_numbering)
 
       grammar.addParseActionEx( lambda x: np.array(x.asList(), self.numpy_type), "Cannot retype to numpy array")
+      if self.flatten:
+          grammar.addParseAction(lambda x: x[0].ravel())
       return grammar
 
   def _string(self, data):
       out = []
       if self.header:
          def gen():
              names = ((i[1] if isinstance(i, tuple) else i) for i in self.names)
@@ -390,15 +395,15 @@
          out.append(self.sequence.string(i))
       return ''.join(out)
 
   def _validate(self, value, why='set'):
       if not isinstance(value, np.ndarray):
          return f"Numpy array as a value required {value.__class__} given"
       dtype = self.numpy_type
-      dim = 1 if isinstance(dtype, list) else 2
+      dim = 1 if isinstance(dtype, list) or self.flatten else 2
       if len(value.shape) != dim:
          return f"The array should have dimension={dim}, it has dimension {len(value.shape)}"
       if value.dtype != self.numpy_type:
          return f"The data type of the value should be {dtype}, it is {value.dtype}"
       if dim==2 and value.shape[1] != len(self.sequence.types):
          return f"The array is required to have {len(self.sequence.types)} columns, it has {value.shape[1]}"
       if self.length is not None and self.length != value.shape[0]:
@@ -419,26 +424,26 @@
                  nr = True
                  break
          else:
              return dtype
       names = self.names or itertools.repeat('')
       return list(zip(names, (i.numpy_type for i in types)))
 
-  def number_of_collumns(self):
+  def number_of_columns(self):
       return len(self.sequence.types)
 
   def zero_data(self, length):
       """ Return array of zeros with the given number of rows and
           with the dtype of the table
       """
       dtype = self.numpy_type
       if isinstance(dtype, list):
          return np.zeros(length, dtype)
       else:
-         return np.zeros((length, self.number_of_collumns()), dtype)
+         return np.zeros((length, self.number_of_columns()), dtype)
 
   def grammar_name(self):
       if self.names:
         data = " ".join( (f'{i}:{j.grammar_name()}' for i,j in zip(self.names, self.sequence.types) ) )
       else:
         data = self.sequence.grammar_name()
       return f"<TABLE of {data}>"
```

### Comparing `ase2sprkkr-2.1.0/src/ase2sprkkr/common/grammar_types/basic.py` & `ase2sprkkr-2.1.1/src/ase2sprkkr/common/grammar_types/basic.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """ Common GrammarTypes as numbers, strings etc. """
 
 from ase.units import Rydberg
 import datetime
 import pyparsing as pp
 ppc = pp.pyparsing_common
 from typing import  Optional
+import numpy as np
 
 from ..decorators import add_to_signature
 from ..grammar import generate_grammar, separator as separator_grammar, \
                      replace_whitechars, optional_quote
 
 from .grammar_type import TypedGrammarType, GrammarType, add_to_parent_validation
 
@@ -33,14 +34,15 @@
   @add_to_parent_validation
   def _validate(self, value, why='set'):
       if self.min is not None and self.min > value:
          return f"A value greater that or equal to {self.min} is required, {value} have been given."
       if self.max is not None and self.max < value:
          return f"A value less than or equal to {self.max} is required, {value} have been given."
       return True
+
 class Unsigned(Number):
   """ Unsigned integer (zero is possible) """
 
   _grammar = replace_whitechars(ppc.integer).setParseAction(lambda x:int(x[0]))
 
   @add_to_parent_validation
   def _validate(self, value, why='set'):
@@ -119,14 +121,23 @@
   _grammar = replace_whitechars(ppc.fnumber).setParseAction(lambda x: float(x[0]))
 
   def grammar_name(self):
     return '<float>'
 
   numpy_type = float
 
+  def convert(self, value):
+      if isinstance(value, (int, np.integer)):
+          from .warnings import SuspiciousValueWarning
+          SuspiciousValueWarning(value, 'An attemtp to set <float> value using an <integer>. I will do a conversion for you.').warn(
+              stacklevel=6
+              )
+          value=float(value)
+
+      return super().convert(value)
 
 class Date(Number):
   """ A date value of the form 'DD.MM.YYYY' """
 
   _grammar = pp.Regex(r'(?P<d>\d{2}).(?P<m>\d{2}).(?P<y>\d{4})').setParseAction(lambda x: datetime.date(int(x['y']), int(x['m']), int(x['d'])))
 
   def grammar_name(self):
```

### Comparing `ase2sprkkr-2.1.0/src/ase2sprkkr/common/grammar_types/grammar_type.py` & `ase2sprkkr-2.1.1/src/ase2sprkkr/common/grammar_types/grammar_type.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.1.0/src/ase2sprkkr/common/grammar_types/mixed.py` & `ase2sprkkr-2.1.1/src/ase2sprkkr/common/grammar_types/mixed.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.1.0/src/ase2sprkkr/common/init_tests.py` & `ase2sprkkr-2.1.1/src/ase2sprkkr/common/init_tests.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.1.0/src/ase2sprkkr/common/misc.py` & `ase2sprkkr-2.1.1/src/ase2sprkkr/common/misc.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.1.0/src/ase2sprkkr/common/no_output.py` & `ase2sprkkr-2.1.1/src/ase2sprkkr/common/no_output.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.1.0/src/ase2sprkkr/common/options.py` & `ase2sprkkr-2.1.1/src/ase2sprkkr/common/options.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 from __future__ import annotations
 
 from typing import Union
 from ..common.grammar_types import mixed
 from .configuration import Configuration
 from ..common.misc import as_integer
+from .decorators import warnings_from_here
 
 class DangerousValue:
   """ This class is used to store (encapsulate) a value, which should not be validated
   - to  overcame sometimes too strict enforment of the options values.
 
   """
 
@@ -96,15 +97,15 @@
       ----------
       all_values: For numbered_array (see :class:`ConfigurationDefinition.is_numbered_array <ConfigurationDefinition>`,
       pass True as this argument to obtain array of all values. If False (the default) is given,
       only the 'wildcard' value (i.e. the one without array index, which is used for the all values
       not explicitly specified) is returned.
       """
       if self._definition.is_generated:
-         return self._definition.getter(self)
+         return self._definition.getter(self._container)
 
       value = self._unpack_value(self._value)
       if value is not None:
           if self._definition.is_numbered_array and not all_values:
               return value.get('def', self.default_value)
           return value
       if hasattr(self, '_result'):
@@ -140,14 +141,15 @@
       """ Return default value for the option.
       The function is here, and not in the definition, since the default value can be given
       by callable, that accepts the Option as argument. This possibility is used in ase2sprkkr,
       when the default values of some options are generated from the underlined Atoms object
       """
       return self._definition.get_value(self)
 
+  @warnings_from_here(stacklevel=2)
   def set(self, value, *, unknown=None, error=None):
       """
       Set the value of the option.
 
       Parameters
       ----------
       value: mixed
@@ -156,15 +158,15 @@
       unknown: str or None
         A dummy argument to make the method compatibile with
         ase2sprkkr.sprkkr.common.configuration_containers.ConfigurationContainer.set()
 
       error:
       """
       if self._definition.is_generated:
-          return self._definition.setter(self, value)
+          return self._definition.setter(self._container, value)
 
       if value is None:
           try:
               return self.clear()
           except ValueError:
               if not error=='ignore': raise
               return
@@ -193,15 +195,15 @@
       """ Check, whether the option is numbered array and thus it can be accessed as array using [] """
       if not self._definition.is_numbered_array and not self._definition.type.array_access:
           raise TypeException('It is not allowed to access {self._get_path()} as array')
 
   def __setitem__(self, name, value):
       """ Set an item of a numbered array. If the Option is not a numbered array, throw an Exception. """
       if self._definition.is_generated:
-          self._definition.setter(self, value, name)
+          self._definition.setter(self._container, value, name)
           return
 
       self._check_array_access()
 
       if not self._definition.is_numbered_array:
           self()[name]=value
           self.validate(why='set')
@@ -237,16 +239,15 @@
             self._value[name] = self._pack_value(value)
          except ValueError:
             if error!='ignore': raise
 
   def __getitem__(self, name):
       """ Get an item of a numbered array. If the Option is not a numbered array, throw an Exception. """
       if self._definition.is_generated:
-          self._definition.getter(self, name)
-          return
+          return self._definition.getter(self._container, name)
       self._check_array_access()
       if not self._definition.is_numbered_array:
           return self()[name]
 
       if isinstance(name, (list, tuple)):
           return [ self._getitem(n) for n in name ]
       elif isinstance(name, slice):
@@ -321,15 +322,15 @@
           del self._result
 
   def clear(self, do_not_check_required=False, call_hooks=True, generated=True):
       """ Clear the value: set it to None """
       if self._definition.is_generated:
           if not generated:
              return
-          self._definition.setter(self, None)
+          self._definition.setter(self._container, None)
       else:
           if not self._definition.type.has_value:
              return
           if self._definition.default_value is None and not do_not_check_required and self._definition.required:
              raise ValueError(f'Option {self._get_path()} must have a value')
           self._value = None
           self.clear_result()
@@ -346,14 +347,16 @@
 
   def _save_to_file(self, file):
       """ Write the name-value pair to the given file, if the value
       is set. """
       d = self._definition
       if d.is_generated:
          return
+      if d.write_condition and not d.write_condition(self):
+         return
 
       if not d.type.has_value:
          return d.write(file, None)
       elif self.is_dangerous():
          value = self._value
       else:
          value = self.result
@@ -446,14 +449,23 @@
   def _find_value(self, name):
       if self._definition.name == name:
          return self
 
   def get_path(self):
       return self._get_path()
 
+  def __len__(self):
+      return len(self())
+
+  def __iter__(self):
+      return iter(self())
+
+  def __bool__(self):
+      return True
+
   def __repr__(self):
       if self._definition.is_generated:
          v = self()
          o = ' (generated)'
       else:
          v = self._value
          o = None
@@ -466,14 +478,15 @@
       if v is None:
         if o:
            o='out' + o
         else:
            o='out'
         v=''
       else:
+         o=''
          v=' = '+str(v)
 
       type = '(generated)' if self._definition.is_generated else f'of type {self._definition.type}'
       return f"<Option {self._get_path()} {type} with{o} value{v}>"
 
 class CustomOption(Option):
   """ An user-added option (configuration value). It can be removed from the section. """
```

### Comparing `ase2sprkkr-2.1.0/src/ase2sprkkr/common/process_output_reader.py` & `ase2sprkkr-2.1.1/src/ase2sprkkr/common/process_output_reader.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.1.0/src/ase2sprkkr/common/test/init_tests.py` & `ase2sprkkr-2.1.1/src/ase2sprkkr/common/test/init_tests.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.1.0/src/ase2sprkkr/common/test/test_common.py` & `ase2sprkkr-2.1.1/src/ase2sprkkr/common/test/test_common.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,18 +88,18 @@
 
 
     def f(a=1, b=2):
         return a,b
 
     @add_to_signature(f, excluding='b')
     def ff(c=1, *args, **kwargs):
-        return c,*f(b=5, *args, **kwargs)
-    self.assertEqual((7,3,5), ff(3,7))
-    self.assertEqual((7,3,5), ff(3,c=7))
-    self.assertEqual((7,3,5), ff(a=3,c=7))
+        return c,f(b=5, *args, **kwargs)
+    self.assertEqual((7,(3,5)), ff(3,7))
+    self.assertEqual((7,(3,5)), ff(3,c=7))
+    self.assertEqual((7,(3,5)), ff(a=3,c=7))
 
 
   def test_asyncio_file_reader(self):
     with tempfile.TemporaryFile(mode='w+b') as tfile:
       tfile.write(b"""First line\nSecond line\nHi, this is a very long file!! really!!! 12345123456789""")
       tfile.seek(0)
       ar = AsyncioFileReader(tfile, buffersize=5)
```

### Comparing `ase2sprkkr-2.1.0/src/ase2sprkkr/common/test/test_grammar_types.py` & `ase2sprkkr-2.1.1/src/ase2sprkkr/common/test/test_grammar_types.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 if __package__:
    from .init_tests import TestCase, patch_package
 else:
    from init_tests import TestCase, patch_package
 __package__, __name__ = patch_package(__package__, __name__)
 
+import warnings
 import pyparsing
 from .. import grammar_types as gt
 from ..grammar import generate_grammar
 import numpy as np
 import datetime
 from ase.units import Rydberg
 
@@ -62,21 +63,30 @@
       #except Exception as e:
       #  if isinstance(e, AssertionError):
       #    raise
       #  raise AssertionError(f"Error '{val}' should be validated to '{res}', {str(e)} occurs")
 
     def test_invalid(val):
       try:
-        val = type.convert(val)
-        self.assertTrue(type.validate(val) is not True)
+        with warnings.catch_warnings():
+          warnings.simplefilter("ignore")
+          val = type.convert(val)
+          self.assertTrue(type.validate(val) is not True)
       except ValueError:
         pass
       else:
         self.assertTrue(False)
 
+    def test_warning(val, res):
+        with warnings.catch_warnings(record = True) as warning_list:
+            val = type.convert(val)
+            self.assertEqual(val, res)
+            self.assertTrue(type.validate(val))
+        self.assertEqual(True, bool(warning_list))
+
     def test_valid(val):
       val = type.convert(val)
       self.assertTrue(type.validate(val) is True)
 
     type = gt.Integer()
     for val, res in [
         ('1', 1),
@@ -122,28 +132,29 @@
         ('1', 1.0),
         ('a', Error),
         ('-1.1', -1.1),
         ('1.1 a', Error),
         ('-1e-2', -1e-2)
         ]:
         test(val, res)
-    for v in [1, 'aaaa', (1,2,3)]: test_invalid(v)
+    for v in ['aaaa', (1,2,3)]: test_invalid(v)
 
     type = gt.Real(min=-5., max=10.)
     for val, res in [
         ('10', 10.0),
         ('10.0001', Error),
         ('a', Error),
         ('-5.1', Error),
         ('-5', -5.),
         ('1.1 a', Error),
         ('-1e-2', -1e-2)
         ]:
         test(val, res)
-    for v in [1, 15., 'aaaa', (1,2,3)]: test_invalid(v)
+    for v in [15., 'aaaa', (1,2,3)]: test_invalid(v)
+    for v,r in [(1, 1.0)]: test_warning(v,r)
 
     type = gt.String()
     for val, res in [
          ('a', 'a'),
          ('a a', Error),
          ('1','1')
          ]:
@@ -154,15 +165,16 @@
     for val, res in [
          ('1', 1.0),
          ('Ry', Error),
          ('1 Ry',1.0),
          ('1 eV', 1.0/Rydberg),
          ]:
          test(val, res)
-    for v in [1, 15, 'aaaa', (1,2,3)]: test_invalid(v)
+    for v in ['aaaa', (1,2,3)]: test_invalid(v)
+    for v,r in [(1, 1.0),(15, 15.0)]: test_warning(v,r)
 
 
     type = gt.SetOf(int)
     for val, res in [
         ('a{}', Error),
         ('{a}', Error),
         ('{1,2}', np.array([1,2])),
@@ -214,14 +226,32 @@
     for val, res in [(
         """ X YY ZZZ
         1 1 dog 2.5
         2 3 cat 3e-2""", np.array([(1,'dog',2.5), (3,'cat', 3e-2)], dtype=[('X', int), ('YY', object), ('ZZZ', float)])
         )]:
         test(val, res)
 
+    type = gt.Table(X=int, numbering='Y')
+    for val, res in [(
+        """ Y X
+        1 1
+        2 3""", np.array([[1], [3]])
+        )]:
+        test(val, res)
+
+    type = gt.Table(X=int, numbering='Y', flatten=True)
+    for val, res in [(
+        """ Y X
+        1 1
+        2 3""", np.array([1, 3])
+        )]:
+        test(val, res)
+
+
+
     type = gt.PotMixed.I
     for val, res in [
         ('1', 1),
         ('-2',-2),
         ('-2.4',-2.4),
         ('AHOJ', 'AHOJ'),
         ('T', True),
@@ -259,15 +289,17 @@
     for val, res in [
          ('{40,50}', np.array([40.,50.])),
          ('40', 40.),
          ('{40,50,60}', Error),
          ('{40}', Error),
          ]:
          test(val, res)
-    for v in [[1.,2,3], 'asasd', 3 ]: test_invalid(v)
+    for v in [[1.,2,3], 'asasd' ]: test_invalid(v)
+    a = lambda *args: np.asarray(args)
+    for v,r in [ (3,3.), ((5,1.),a(5.,1.)), ((7.,3),a(7.,3.)) ]: test_warning(v,r)
     for v in [ [1.,3.], 8. ]: test_valid(v)
 
     type = gt.Date()
     for val, res in [
          ('{40,50}', Error),
          ('23.01.2020', datetime.date(2020,1,23) ),
          ('40', Error),
```

### Comparing `ase2sprkkr-2.1.0/src/ase2sprkkr/common/tools.py` & `ase2sprkkr-2.1.1/src/ase2sprkkr/common/tools.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.1.0/src/ase2sprkkr/common/unique_values.py` & `ase2sprkkr-2.1.1/src/ase2sprkkr/common/unique_values.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.1.0/src/ase2sprkkr/input_parameters/definitions/arpes.py` & `ase2sprkkr-2.1.1/src/ase2sprkkr/input_parameters/definitions/arpes.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,16 +36,16 @@
       V('CRYS_VEC', True, info='Miller indices with respect to crystalographic primitive vectors'),
 
       V('STRVER', 1, is_expert=True, is_always_added=True, info="Set to 0 to supply the ARPES input file 'struc.inp' manually (and do not generate it)."),
       V('INPVER', 1, is_expert=True, is_always_added=True, info='Set to 0 to use an old input.inp from old rslab'),
     ]),
 
     Section('SPEC_PH', [
-      V('THETA', 45.),
-      V('PHI', 0.),
+      V('THETA', Range(float), 45.),
+      V('PHI', Range(float), 0.),
       V('POL_P', DefKeyword('P', 'S', 'C+', 'C-'), info='Polarization of the light'),
       V('EPHOT', 6675., info='Photon energy in eV'),
       #Expert
       V('ALQ', expert=45., info='Alignment of polarization vector or pol.ellipsis'),
       V('DELQ', expert=0., info='Phase shift between real and imaginary part of e-vector, delq=90 for circular polarized light'),
       V('NPOL', Keyword({
         0: 'unpolarized and p-s dichroism for the calculation',
```

### Comparing `ase2sprkkr-2.1.0/src/ase2sprkkr/input_parameters/definitions/dos.py` & `ase2sprkkr-2.1.1/src/ase2sprkkr/input_parameters/definitions/dos.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.1.0/src/ase2sprkkr/input_parameters/definitions/gilbert.py` & `ase2sprkkr-2.1.1/src/ase2sprkkr/input_parameters/definitions/gilbert.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.1.0/src/ase2sprkkr/input_parameters/definitions/phagen.py` & `ase2sprkkr-2.1.1/src/ase2sprkkr/input_parameters/definitions/phagen.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.1.0/src/ase2sprkkr/input_parameters/definitions/scf.py` & `ase2sprkkr-2.1.1/src/ase2sprkkr/input_parameters/definitions/scf.py`

 * *Files 27% similar despite different names*

```diff
@@ -4,15 +4,16 @@
 from ..input_parameters_definitions import \
     InputParametersDefinition as InputParameters, \
     InputValueDefinition as V
 
 input_parameters = InputParameters(
       'scf', [
         CONTROL('SCF').copy([
-          V('KRWS', 1)
+          V('KRWS', Integer(min=0, max=1), 1),
+          V('KRMT', Integer(min=0, max=6), required=False)
         ]),
         TAU,
         ENERGY,
         SCF,
         SITES,
         STRCONST,
         CPA,
```

### Comparing `ase2sprkkr-2.1.0/src/ase2sprkkr/input_parameters/definitions/sections.py` & `ase2sprkkr-2.1.1/src/ase2sprkkr/input_parameters/definitions/sections.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """ Definitions of sections to be used in definitions of input parameters
 (input files for SPR-KKR tasks) """
 
-from ...common.grammar_types  import DefKeyword, SetOf, flag, energy, Integer, Array
+from ...common.grammar_types  import DefKeyword, SetOf, flag, energy, Integer, Array, Keyword
 from ..input_parameters_definitions import \
       InputSectionDefinition as Section, \
       InputValueDefinition as V
 from ...sprkkr.sprkkr_grammar_types import Site, AtomicType
 
 def CONTROL(ADSI):
   """ Create the definition of the CONTROL section of the task input file.
@@ -63,21 +63,21 @@
 points. It is the standard method and gives a good compromise concerning accuracy
 and efficiency. For BZINT=POINTS the parameter NKTAB will be adjusted to allow a
 regular mesh.
 """), required=True,
                              info='The mode of BZ-integration used for calculation of the scattering '
                                   ' path operator τ'),
       V('NKTAB', 250, info='Number of points for the special points method', is_optional=True,
-        description='For 2D problem, it severs only as default value for NKTABxD.'),
-      V('NKTAB2D', int, _nktab_value, info='Number of points for the special points method for 2D region of 2D problem', is_optional=True,
-        description='If it is not specified, NKTAB is used.'),
-      V('NKTAB3D', int, _nktab_value, info='Number of points for the special points method for 3D region of 2D problem', is_optional=True,
-        description='If it is not specified, NKTAB is used'),
-      V('NKMIN', 300, info='Minimal number of k-points used for Weyl integration'),
-      V('NKMAX', 500, info='Maximal number of k-points used for Weyl integration'),
+        description='For 2D problem, it serves only as default value for NKTABxD.'),
+      V('NKTAB2D', int, _nktab_value, info='Number of points for the special points method for 2D region of 2D problem',
+        is_optional=True, description='If it is not specified, NKTAB is used.'),
+      V('NKTAB3D', int, _nktab_value, info='Number of points for the special points method for 3D region of 2D problem',
+        is_optional=True, description='If it is not specified, NKTAB is used'),
+      V('NKMIN', 300, info='Minimal number of k-points used for Weyl integration', write_condition= lambda o: o._container.BZINT() == 'WEYL'),
+      V('NKMAX', 500, info='Maximal number of k-points used for Weyl integration', write_condition= lambda o: o._container.BZINT() == 'WEYL'),
       #expert
       V('CLUSTER', flag, expert=False, info="""Do cluster type calculation.""", description=
         "Cluster type calculation calculate τ by inverting the real space KKR matrix. "
         "Specify cluster center using IQCNTR or ITCNTR and its size using NSHLCLU or CLURAD."
       ),
       V('NSHLCLU', int, is_expert=True, is_optional=True, info="Number of atomic shells around the central atom of a cluster"),
       V('CLURAD', int, is_expert=True, is_optional=True, info="Radius of the cluster in multiples of ALAT."),
@@ -95,27 +95,34 @@
       V('EMIN', -0.2, info='The real part of the lowest E-value'),
   ])
 """The definition of the ENERGY section of the task input file """
 
 SCF = Section('SCF', [
       V('NITER', 200, info='Maximal number of iterations of the SCF cycle'),
       V('MIX', 0.2, info='Mixing parameter'),
+      V('MIXOP', float, required=False),
       V('VXC', DefKeyword({
         'VWN' : 'Vosko, Wilk, Nusair',
         'MJW' : 'Janak, Williams, Moruzzigit g',
         'VBH' : 'von Barth, Hedin',
-        'PBE' : 'Perdew, Burke, Ernzendorfer GGA'
+        'PBE' : 'Perdew, Burke, Ernzendorfer GGA',
+        'PW92' : 'Perdew Wang',
+        'EV-GGA' : 'Engel and Vosko GGA',
+        'BJ' : 'Becke-Johnson',
+        'MBJ' : 'modified Becke-Johnson'
+
         }), info='parametrisation of the exchange-correlation potential'),
       V('ALG', DefKeyword({
           'BROYDEN2': 'Broyden’s second method',
           'TCHEBY': 'Tchebychev'
         }), info='Mixing algorithm'),
-      V('EFGUESS', 0.7),
+      V('EFGUESS', float, required=False, info='Skip the Fermi energy search in the beginning.'),
       V('TOL', 0.00001, info='Tolerance threshold for the mixing algorithm'),
       V('ISTBRY', 1, info='Start Broyden after ISTBRY iterations'),
+      V('FULLPOT', False, info='Non-spherical callculation (full-potential) instead of ASA'),
       V('ITDEPT', 40, info='Iteration depth for Broyden algorithm (length of used history)'),
       V('QION', Array(float), required=False, info='Guess for the ionic charges Qt for atomic types'),
       V('MSPIN', Array(float), required=False, info='Guess for the magnetic moment μ_{spin,t} for atomic types'),
       V('USEVMATT', False, info='Set up the starting potential using the original Mattheiss'
                                  'construction for the potential V instead of the charge density')
   ])
 """The definition of the SCF section of the task input file """
@@ -157,15 +164,22 @@
   ], is_expert=True, is_optional=True,
   info="""For a system with substitutional disorder, the CPA is used. The listed variables control the CPA cycle """,
 )
 """CPA section definition"""
 
 
 MODE = Section('MODE', [
-  V('SP-SREL', False, info="work in the spin-polarized scalar-relativistic mode"),
+  V('MODE',
+    Keyword({
+    'NREL' : "work in the nonrelativistic mode",
+    'SREL' : "work in the spin-polarized scalar-relativistic mode",
+    'SP-SREL' : "work in the scalar-relativistic mode"}), None,
+            required=False, name_in_grammar=False,
+            info='Using this option you can switch on spin the polarization and relativistic mode'),
+  V('LLOYD', False, info='Use LLoyd formula for scattering operator. It can improve the accuracy of the Fermi energy.'),
   V('MDIR', [0,0,1], info="Common magnetisation direction vector with x, y and z in Cartesian coordinates. The normalisation is arbitrary.", is_numbered_array=True),
   V('C', 1.0, info='Scale the speed of light for a given atom type.', is_numbered_array=True),
   V('SOC', 1.0, info='Scale the strength of the spin-orbit coupling for atom type.', is_numbered_array=True),
   ], is_expert=True, is_optional=True, info=
       """If not specified otherwise the programs of the SPRKKR-package assume that a magnetic system should be treated in a fully relativistic way. By setting the parameter SP-SREL a slightly faster scalar relativistic calculation can be done instead for a magnetic system.""",
 )
 """MODE Section definition"""
```

### Comparing `ase2sprkkr-2.1.0/src/ase2sprkkr/input_parameters/examples/arpes.in` & `ase2sprkkr-2.1.1/src/ase2sprkkr/input_parameters/examples/arpes.in`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.1.0/src/ase2sprkkr/input_parameters/input_parameters.py` & `ase2sprkkr-2.1.1/src/ase2sprkkr/input_parameters/input_parameters.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.1.0/src/ase2sprkkr/input_parameters/input_parameters_definitions.py` & `ase2sprkkr-2.1.1/src/ase2sprkkr/input_parameters/input_parameters_definitions.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.1.0/src/ase2sprkkr/input_parameters/test/init_tests.py` & `ase2sprkkr-2.1.1/src/ase2sprkkr/input_parameters/test/init_tests.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.1.0/src/ase2sprkkr/input_parameters/test/test_definitions.py` & `ase2sprkkr-2.1.1/src/ase2sprkkr/input_parameters/test/test_definitions.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.1.0/src/ase2sprkkr/input_parameters/test/test_input_parameters.py` & `ase2sprkkr-2.1.1/src/ase2sprkkr/input_parameters/test/test_input_parameters.py`

 * *Files 3% similar despite different names*

```diff
@@ -68,14 +68,33 @@
        cv = cd.InputValueDefinition('aaa', int, required=True).grammar(allow_dangerous=True)
 
      assertParse("aaa=1", ('aaa', 1))
      assertParseDangerous("aaa=1.0", ('aaa', 1.0))
      assertParseDangerous("aaa=sss", ('aaa', 'sss'))
      assertParseDangerous("aaa={2,3}", ('aaa', np.array([2,3])))
 
+  def test_write_condition(self):
+    V = cd.InputValueDefinition
+
+    input_parameters_def = cd.InputParametersDefinition.from_dict({
+      'ENERGY' : [
+        V('E', 1)
+      ]})
+    del input_parameters_def._members['TASK']
+    id=input_parameters_def.read_from_file(io.StringIO('ENERGY E=1'))
+    self.assertEqual(id.to_string(), "ENERGY\n\tE=1\n")
+    input_parameters_def['ENERGY']['E'].write_condition = lambda o: True
+    self.assertEqual(id.to_string(), "ENERGY\n\tE=1\n")
+    input_parameters_def['ENERGY']['E'].write_condition = lambda o: False
+    self.assertEqual(id.to_string(), "ENERGY\n")
+    input_parameters_def['ENERGY'].write_condition = lambda o: True
+    self.assertEqual(id.to_string(), "ENERGY\n")
+    input_parameters_def['ENERGY'].write_condition = lambda o: False
+    self.assertEqual(id.to_string(), "")
+
   def test_input_parameters_definition(self):
     V = cd.InputValueDefinition
 
     input_parameters_def = cd.InputParametersDefinition.from_dict({
       'ENERGY' : [
         V('GRID', gt.SetOf(int, length=1), fixed_value=3),
         V('NE', gt.SetOf(int, min_length=1)),
```

### Comparing `ase2sprkkr-2.1.0/src/ase2sprkkr/outputs/output_definitions.py` & `ase2sprkkr-2.1.1/src/ase2sprkkr/outputs/output_definitions.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.1.0/src/ase2sprkkr/outputs/output_files_definitions.py` & `ase2sprkkr-2.1.1/src/ase2sprkkr/outputs/output_files_definitions.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 from ..sprkkr.configuration import ConfigurationValueDefinition, ConfigurationFileDefinition, \
                                    CustomConfigurationValue
 
-from ..common.decorators import cached_class_property
+from ..common.decorators import cached_class_property, cache
 from ..common.grammar_types  import unsigned, Array, Table, RestOfTheFile, Keyword, GrammarType, \
                                      pot_mixed, line_string, line_end, Separator as GTSeparator
 from ..common.grammar import generate_grammar
 import pyparsing as pp
 from ..common.decorators import cached_class_property
 import sys
 from .output_files import OutputFile
-from functools import cache
 
 class OutputFileValueDefinition(ConfigurationValueDefinition):
   """ This class describes the format of one value of
   a header of an output file """
   @cached_class_property
   def grammar_of_delimiter():
     return pp.Empty().setName(' ')
@@ -77,18 +76,16 @@
       V('NT_EFF', int),
       Separator(),
       V('NE', int),
       V('IREL', int),
       V('EFERMI', float),
       V('INFO', str),
       Separator(),
-      V('ORBITALS', Table({'NLQ' : unsigned}, numbering='IQ'), name_in_grammar = False),
+      V('ORBITALS', Table({'NLQ' : unsigned}, numbering='IQ', flatten=True), name_in_grammar = False),
       V('TYPES', Table({'TXT_T': str, 'CONC': float, 'NAT': int, 'IQAT': Array(int)}, numbering='IT'), name_in_grammar=False),
-      V('NT', int),
-      V('NP', int),
     ]
 
 def create_output_file_definition(keyword, add, name=None,
                                   cls=OutputFileDefinition,
                                   **kwargs):
     """ Create a definition of a output file. One should supply the additional values
     containing the actual data.
```

### Comparing `ase2sprkkr-2.1.0/src/ase2sprkkr/outputs/readers/arpes.py` & `ase2sprkkr-2.1.1/src/ase2sprkkr/outputs/readers/arpes.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.1.0/src/ase2sprkkr/outputs/readers/scf.py` & `ase2sprkkr-2.1.1/src/ase2sprkkr/outputs/readers/scf.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.1.0/src/ase2sprkkr/outputs/task_result.py` & `ase2sprkkr-2.1.1/src/ase2sprkkr/outputs/task_result.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.1.0/src/ase2sprkkr/outputs/test/init_tests.py` & `ase2sprkkr-2.1.1/src/ase2sprkkr/outputs/test/init_tests.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.1.0/src/ase2sprkkr/outputs/test/test_files.py` & `ase2sprkkr-2.1.1/src/ase2sprkkr/outputs/test/test_files.py`

 * *Files 14% similar despite different names*

```diff
@@ -22,7 +22,12 @@
                self.assertEqual('ARPES', out.KEYWORD())
                self.assertEqual((200,160), out.ENERGY().shape)
                o2 = out + out
                for i in 'ENERGY', 'THETA', 'K', 'DETERMINANT':
                    self.assertEqual(out[i](), o2[i]())
                for i in 'TOTAL', 'POLARIZATION', 'UP', 'DOWN':
                    self.assertEqual(2*out[i](), o2[i]())
+            if ext=='dos':
+               self.assertEqual(out.n_orbitals(1), 3)
+               self.assertEqual(out.n_spins(), 2)
+               self.assertEqual((3,2,1200), out.dos_for_site_type('Ta').shape)
+               self.assertEqual(out.DOS['Ta'][5], out.dos_for_site_type('Ta',1,2))
```

### Comparing `ase2sprkkr-2.1.0/src/ase2sprkkr/outputs/test/test_output.py` & `ase2sprkkr-2.1.1/src/ase2sprkkr/outputs/test/test_output.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.1.0/src/ase2sprkkr/physics/lattice_data.py` & `ase2sprkkr-2.1.1/src/ase2sprkkr/physics/lattice_data.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.1.0/src/ase2sprkkr/physics/winger_seitz_radii.py` & `ase2sprkkr-2.1.1/src/ase2sprkkr/physics/winger_seitz_radii.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.1.0/src/ase2sprkkr/potentials/custom_potential_section.py` & `ase2sprkkr-2.1.1/src/ase2sprkkr/potentials/custom_potential_section.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.1.0/src/ase2sprkkr/potentials/definitions/potential.py` & `ase2sprkkr-2.1.1/src/ase2sprkkr/potentials/definitions/potential.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.1.0/src/ase2sprkkr/potentials/definitions/sections/__init__.py` & `ase2sprkkr-2.1.1/src/ase2sprkkr/potentials/definitions/sections/__init__.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.1.0/src/ase2sprkkr/potentials/definitions/sections/global_system_parameter.py` & `ase2sprkkr-2.1.1/src/ase2sprkkr/potentials/definitions/sections/global_system_parameter.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.1.0/src/ase2sprkkr/potentials/definitions/sections/lattice.py` & `ase2sprkkr-2.1.1/src/ase2sprkkr/potentials/definitions/sections/lattice.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.1.0/src/ase2sprkkr/potentials/definitions/sections/mesh_information.py` & `ase2sprkkr-2.1.1/src/ase2sprkkr/potentials/definitions/sections/mesh_information.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.1.0/src/ase2sprkkr/potentials/definitions/sections/occupation.py` & `ase2sprkkr-2.1.1/src/ase2sprkkr/potentials/definitions/sections/occupation.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.1.0/src/ase2sprkkr/potentials/definitions/sections/reference_system.py` & `ase2sprkkr-2.1.1/src/ase2sprkkr/potentials/definitions/sections/reference_system.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.1.0/src/ase2sprkkr/potentials/definitions/sections/sites.py` & `ase2sprkkr-2.1.1/src/ase2sprkkr/potentials/definitions/sections/sites.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.1.0/src/ase2sprkkr/potentials/definitions/sections/types.py` & `ase2sprkkr-2.1.1/src/ase2sprkkr/potentials/definitions/sections/types.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.1.0/src/ase2sprkkr/potentials/examples/FePt.new.pot` & `ase2sprkkr-2.1.1/src/ase2sprkkr/potentials/examples/FePt.new.pot`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.1.0/src/ase2sprkkr/potentials/examples/FePt.pot` & `ase2sprkkr-2.1.1/src/ase2sprkkr/potentials/examples/FePt.pot`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.1.0/src/ase2sprkkr/potentials/examples/GeTe.pot` & `ase2sprkkr-2.1.1/src/ase2sprkkr/potentials/examples/GeTe.pot`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.1.0/src/ase2sprkkr/potentials/examples/Li_scf.new.pot` & `ase2sprkkr-2.1.1/src/ase2sprkkr/potentials/examples/Li_scf.new.pot`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.1.0/src/ase2sprkkr/potentials/examples/fp_basscale0.pot` & `ase2sprkkr-2.1.1/src/ase2sprkkr/potentials/examples/fp_basscale0.pot`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.1.0/src/ase2sprkkr/potentials/examples/fp_new.pot` & `ase2sprkkr-2.1.1/src/ase2sprkkr/potentials/examples/fp_new.pot`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.1.0/src/ase2sprkkr/potentials/potential_definitions.py` & `ase2sprkkr-2.1.1/src/ase2sprkkr/potentials/potential_definitions.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.1.0/src/ase2sprkkr/potentials/potential_sections.py` & `ase2sprkkr-2.1.1/src/ase2sprkkr/potentials/potential_sections.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.1.0/src/ase2sprkkr/potentials/potentials.py` & `ase2sprkkr-2.1.1/src/ase2sprkkr/potentials/potentials.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.1.0/src/ase2sprkkr/potentials/test/init_tests.py` & `ase2sprkkr-2.1.1/src/ase2sprkkr/potentials/test/init_tests.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.1.0/src/ase2sprkkr/potentials/test/test_2D.py` & `ase2sprkkr-2.1.1/src/ase2sprkkr/potentials/test/test_2D.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.1.0/src/ase2sprkkr/potentials/test/test_custom_section.py` & `ase2sprkkr-2.1.1/src/ase2sprkkr/potentials/test/test_custom_section.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.1.0/src/ase2sprkkr/potentials/test/test_potential.py` & `ase2sprkkr-2.1.1/src/ase2sprkkr/potentials/test/test_potential.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.1.0/src/ase2sprkkr/potentials/test/test_structure.py` & `ase2sprkkr-2.1.1/src/ase2sprkkr/potentials/test/test_structure.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.1.0/src/ase2sprkkr/sprkkr/atomic_types.py` & `ase2sprkkr-2.1.1/src/ase2sprkkr/sprkkr/atomic_types.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.1.0/src/ase2sprkkr/sprkkr/atoms_region.py` & `ase2sprkkr-2.1.1/src/ase2sprkkr/sprkkr/atoms_region.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.1.0/src/ase2sprkkr/sprkkr/build.py` & `ase2sprkkr-2.1.1/src/ase2sprkkr/sprkkr/build.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.1.0/src/ase2sprkkr/sprkkr/calculator.py` & `ase2sprkkr-2.1.1/src/ase2sprkkr/sprkkr/calculator.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.1.0/src/ase2sprkkr/sprkkr/configuration.py` & `ase2sprkkr-2.1.1/src/ase2sprkkr/sprkkr/configuration.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.1.0/src/ase2sprkkr/sprkkr/io_data.py` & `ase2sprkkr-2.1.1/src/ase2sprkkr/sprkkr/io_data.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.1.0/src/ase2sprkkr/sprkkr/occupations.py` & `ase2sprkkr-2.1.1/src/ase2sprkkr/sprkkr/occupations.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.1.0/src/ase2sprkkr/sprkkr/radial_meshes.py` & `ase2sprkkr-2.1.1/src/ase2sprkkr/sprkkr/radial_meshes.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.1.0/src/ase2sprkkr/sprkkr/sites.py` & `ase2sprkkr-2.1.1/src/ase2sprkkr/sprkkr/sites.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.1.0/src/ase2sprkkr/sprkkr/sprkkr_atoms.py` & `ase2sprkkr-2.1.1/src/ase2sprkkr/sprkkr/sprkkr_atoms.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.1.0/src/ase2sprkkr/sprkkr/sprkkr_grammar_types.py` & `ase2sprkkr-2.1.1/src/ase2sprkkr/sprkkr/sprkkr_grammar_types.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.1.0/src/ase2sprkkr/sprkkr/structure.py` & `ase2sprkkr-2.1.1/src/ase2sprkkr/sprkkr/structure.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.1.0/src/ase2sprkkr/sprkkr/sysfile.py` & `ase2sprkkr-2.1.1/src/ase2sprkkr/sprkkr/sysfile.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.1.0/src/ase2sprkkr/sprkkr/test/init_tests.py` & `ase2sprkkr-2.1.1/src/ase2sprkkr/sprkkr/test/init_tests.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.1.0/src/ase2sprkkr/sprkkr/test/test_arpes.py` & `ase2sprkkr-2.1.1/src/ase2sprkkr/sprkkr/test/test_arpes.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.1.0/src/ase2sprkkr/sprkkr/test/test_build.py` & `ase2sprkkr-2.1.1/src/ase2sprkkr/sprkkr/test/test_build.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.1.0/src/ase2sprkkr/sprkkr/test/test_calculator.py` & `ase2sprkkr-2.1.1/src/ase2sprkkr/sprkkr/test/test_calculator.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.1.0/src/ase2sprkkr/sprkkr/test/test_sites.py` & `ase2sprkkr-2.1.1/src/ase2sprkkr/sprkkr/test/test_sites.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.1.0/src/ase2sprkkr/sprkkr/test/test_sprkkr_atoms.py` & `ase2sprkkr-2.1.1/src/ase2sprkkr/sprkkr/test/test_sprkkr_atoms.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.1.0/src/ase2sprkkr/sprkkr/test/test_sysfile.py` & `ase2sprkkr-2.1.1/src/ase2sprkkr/sprkkr/test/test_sysfile.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.1.0/src/ase2sprkkr/tools/a2s_plot_output.py` & `ase2sprkkr-2.1.1/src/ase2sprkkr/tools/a2s_plot_output.py`

 * *Files 18% similar despite different names*

```diff
@@ -17,14 +17,16 @@
   description='This is a script for plotting SPR-KKR output files'
   parser = argparse.ArgumentParser(description=description)
   parser.add_argument('output', help='SPR-KKR output file, e.g. ARPES output (*.spc).')
   parser.add_argument('-v','--value', dest='value', type=str, help='Only the value of the given name will be plotted (can be repeated)', action='append', default=[], required=False)
   parser.add_argument('-o','--output_filename', dest='filename', type=str, help='The plot will be saved to a file with given name, instead of showing it on the screen', default=None, required=False)
   parser.add_argument('-L','--do_not_use_latex', dest='latex', action='store_false', default=True, help='Do not use LaTex for captions generating', required=False)
   parser.add_argument('-s','--plot_size', dest='figsize', default=(6,4), type=parse_tuple_function(float,2),   help='The plot size', required=False)
+  parser.add_argument('-c','--colormap', dest='colormap', type=str, help='Matplotlib colormap', required=False)
+  parser.add_argument('-n','--norm', dest='norm', choices=['lin', 'log'], help='Matplotlib colormap will use linear or logarithmic scale (the default behavior depends on the plotted data)', required=False)
 
   args = parser.parse_args()
   kwargs = vars(args)
 
   of = OutputFile.from_file(args.output)
   del kwargs['output']
```

### Comparing `ase2sprkkr-2.1.0/src/ase2sprkkr/tools/a2s_visualise_in_struct.py` & `ase2sprkkr-2.1.1/src/ase2sprkkr/tools/a2s_visualise_in_struct.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.1.0/src/ase2sprkkr/tools/test/init_tests.py` & `ase2sprkkr-2.1.1/src/ase2sprkkr/tools/test/init_tests.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.1.0/src/ase2sprkkr/tools/test/test_tools.py` & `ase2sprkkr-2.1.1/src/ase2sprkkr/tools/test/test_tools.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.1.0/src/ase2sprkkr/visualise/plot.py` & `ase2sprkkr-2.1.1/src/ase2sprkkr/visualise/plot.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 """ In this file the general plotting routines are present. """
+import copy
 
 from matplotlib import rc_context
 import matplotlib.pyplot as plt
+from matplotlib.colors import SymLogNorm, CenteredNorm, LogNorm, Normalize
 from typing import Optional, Callable
 import numpy as np
 import functools
+
 from ..common.decorators import add_to_signature
 
 def normalize_rc_params(params):
     out = {}
     for k,v in params.items():
         if isinstance(v, dict):
            v=normalize_rc_params(v)
@@ -42,14 +45,15 @@
 
     return combined_cmap
 
 def combined_colormap(range1=(0.5, 0), range2=(0.15, 1), n1=8000, n2=15000, cmap1=plt.cm.bwr, cmap2=plt.cm.jet):
     # Create the new colormap
     return combine_colormaps(cmap1, cmap2, n1, n2, range1, range2)
 
+
 def create_rc_context(latex:bool=True):
     """
     Create the context that sets defaults for plotting
     """
     params = rc_params
     if not latex:
        params['text.usetex'] = False
@@ -76,66 +80,105 @@
     with create_rc_context(latex):
       fig, ax = plt.subplots(figsize=figsize)
       plt.subplots_adjust(left=0.15,right=0.95,bottom=0.17,top=0.93)
       fn(*args, **kwargs, axis=ax)
       finish_plot(filename, show, dpi)
 
 def finish_plot(filename:Optional[str]=None, show:Optional[bool]=None, dpi=600):
+     """
+     Show the plot and/or save it to the given file
+     """
      if show is None:
         show=filename is None
      if show:
         plt.show()
      if filename:
         plt.savefig(filename, dpi=dpi)
 
 
 def auto_range(rng, data):
+    """
+    Fill the missing value in the given range by the data.
+
+    >>> auto_range( (None, None), [2,5,-3,7] )
+    (-3, 7)
+    >>> auto_range( (None, 4), [2,5,-3,7] )
+    (-3, 4)
+    >>> auto_range( (2, 4), [2,5,-3,7] )
+    (2, 4)
+    """
     if rng is None:
        return ( np.min(data), np.max(data) )
     return (
-        data[0] if data[0] is not None else np.min(data),
-        data[1] if data[1] is not None else np.max(data),
+        rng[0] if rng[0] is not None else np.min(data),
+        rng[1] if rng[1] is not None else np.max(data),
         )
 def plotting_function(func):
+    """ Decorator, that 'completes' the given function that just draw into a
+    matplolib axis.
+    The completed function will have a few more arguments. One of them is
+    ``axis``. If it is given, the plot is just drawn to the axis. If not,
+    a plot is created, the function is called to draw into the plot, and
+    then the plot is either showed or saved, according to the rest of the added
+    arguments
+    """
+
     @add_to_signature(func)
     @functools.wraps(func)
     def plot_function(*args, filename=None, show=None, dpi=600, latex=True, axis=None, **kwargs):
         if axis:
            func(*args, axis=axis, **kwargs)
         else:
            single_plot(func, filename=filename, show=show, dpi=dpi, latex=latex, *args, **kwargs)
     return plot_function
 
-def common_plot(title=None, xlabel=None, ylabel=None, xticklabels=None, yticklabels=None, axis=None):
+def set_up_common_plot(axis, title=None, xlabel=None, ylabel=None, xticklabels=None, yticklabels=None):
    l = locals()
+   """
+   This functions just set the properties of an matplotlib axis, that are common across various plots.
+   """
    args = { n: l[n]
             for n in ('xlabel', 'ylabel', 'xticklabels', 'yticklabels', 'title')
             if l[n] is not None }
    for name in args:
        if args[name] is not None:
            getattr(axis, 'set_'+name)(args[name])
 
 
 @plotting_function
-@add_to_signature(common_plot, prepend=True)
-def colormesh(x,y,c, xrange=None, yrange=None, colormap=None, show_zero_line=False, axis=None, **kwargs):
+@add_to_signature(set_up_common_plot, prepend=True)
+def colormesh(x,y,c, xrange=None, yrange=None, colormap=None, show_zero_line=False, axis=None, mode=False, norm=None, vmax=None, **kwargs):
    """
    Plot 3D data by assigning colors to 2D grid. See matplotlib.pyplot.pcolormesh
    """
-   common_plot(**kwargs, axis=axis)
-   colormap = colormap or 'Blues'
+   set_up_common_plot(axis, **kwargs)
+   autonorm = False
+   if mode == 'centered':
+       if norm == 'log':
+           colormap = colormap or 'RdBu_r'
+           norm = SymLogNorm(linthresh=1e-12,vmax=vmax) #, vmin=c.min(), vmax=c.max())
+       elif norm =='lin':
+           colormap = colormap or 'seismic'
+           norm = CenteredNorm(vmax=vmax)
+   else:
+       colormap = colormap or 'BuPu'
+       if norm == 'log':
+           norm=LogNorm(vmin=1e-8, vmax=vmax)
+       elif norm=='lin':
+           norm=Normalize(vmin=0. if mode == 'from_zero' else None, vmax=vmax)
+
    axis.set_xlim(auto_range(xrange, x))
    axis.set_ylim(auto_range(yrange, y))
-   axis.pcolormesh(x,y,c,cmap=colormap,shading='gouraud',
-                 vmin=c.min(), vmax=c.max())
+   axis.pcolormesh(x,y,c,cmap=colormap,shading='gouraud', norm=norm)
    if show_zero_line:
        axis.plot(axis.get_xlim(),[0,0],color='black',lw=1)
 
 
 class Multiplot:
+  """ This class can be used for plotting more plots into one resulting image/window. """
 
   def __init__(self, layout, figsize=(6,4), latex=True, updown_layout=False):
       self.fig, self.axes = plt.subplots(figsize=(6,4), nrows=layout[0], ncols=layout[1])
       plt.subplots_adjust(left=0.12,right=0.95,bottom=0.17,top=0.90, hspace=0.75, wspace=0.5)
       self.free_axes = self.axes.ravel(order='F' if not updown_layout else 'C')
       self.free_axes = [ i for i in self.free_axes[::-1] ]
 
@@ -171,22 +214,30 @@
   """
 
   def __init__(self, axes, method=None, **kwargs):
       self.kwargs = kwargs
       self.axes = axes
       self.method = method
 
-  def __call__(self, option, **kwargs):
+  def __add__(self, others):
+      if not isinstance(others, dict):
+          raise NotImplementedError("Only dict can be added to the PlotInfo")
+      out = copy.copy(self)
+      out.kwargs = copy.copy(out.kwargs)
+      out.kwargs.update(others)
+      return out
 
+  def __call__(self, option, **kwargs):
       values = option()
       tmp = self.kwargs.copy()
-      tmp.update(kwargs)
+      tmp.update( (k,v) for k,v in kwargs.items() if v is not None )
       kwargs = tmp
       if 'args' in kwargs and option.name in kwargs['args']:
          kwargs.update(kwargs['args'][option.name])
+      kwargs = { k: v(option) if isinstance(v, PlotValue) else v for k,v in kwargs.items() }
 
       axes = kwargs.get('axes', self.axes)
       method = kwargs.get('method', self.method)
       if method is None:
          if values.ndim == 2: method = colormesh
 
       kwargs = { i:j for i,j in kwargs.items() if i not in ('axes', 'method', 'args') }
@@ -206,7 +257,15 @@
 
       if 'title' in kwargs and kwargs['title'] == False:
          del kwargs['title']
       elif 'title' not in kwargs:
          kwargs['title'] = option.info if option.info else option.name
 
       method(*xdata, values, **kwargs)
+
+class PlotValue:
+
+  def __init__(self, func):
+      self.func = func
+
+  def __call__(self, option):
+      return self.func(option)
```

### Comparing `ase2sprkkr-2.1.0/src/ase2sprkkr.egg-info/PKG-INFO` & `ase2sprkkr-2.1.1/src/ase2sprkkr.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ase2sprkkr
-Version: 2.1.0
+Version: 2.1.1
 Summary: ASE (atomic simulation environment) interface to SPRKKR
 Home-page: https://ase2sprkkr.github.io/ase2sprkkr/
 Author: Matyáš Novák & Jano Minár
 Author-email: ase2kkr@ntc.zcu.cz
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ase2sprkkr-2.1.0/src/ase2sprkkr.egg-info/SOURCES.txt` & `ase2sprkkr-2.1.1/src/ase2sprkkr.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -39,17 +39,17 @@
 src/ase2sprkkr/common/process_output_reader.py
 src/ase2sprkkr/common/tools.py
 src/ase2sprkkr/common/unique_values.py
 src/ase2sprkkr/common/grammar_types/__init__.py
 src/ase2sprkkr/common/grammar_types/arrays.py
 src/ase2sprkkr/common/grammar_types/basic.py
 src/ase2sprkkr/common/grammar_types/data.py
-src/ase2sprkkr/common/grammar_types/functions.py
 src/ase2sprkkr/common/grammar_types/grammar_type.py
 src/ase2sprkkr/common/grammar_types/mixed.py
+src/ase2sprkkr/common/grammar_types/warnings.py
 src/ase2sprkkr/common/test/__init__.py
 src/ase2sprkkr/common/test/init_tests.py
 src/ase2sprkkr/common/test/test_common.py
 src/ase2sprkkr/common/test/test_grammar_types.py
 src/ase2sprkkr/input_parameters/__init__.py
 src/ase2sprkkr/input_parameters/input_parameters.py
 src/ase2sprkkr/input_parameters/input_parameters_definitions.py
@@ -69,14 +69,15 @@
 src/ase2sprkkr/input_parameters/test/test_definitions.py
 src/ase2sprkkr/input_parameters/test/test_input_parameters.py
 src/ase2sprkkr/outputs/__init__.py
 src/ase2sprkkr/outputs/output_definitions.py
 src/ase2sprkkr/outputs/output_files_definitions.py
 src/ase2sprkkr/outputs/task_result.py
 src/ase2sprkkr/outputs/output_files/__init__.py
+src/ase2sprkkr/outputs/output_files/dos.py
 src/ase2sprkkr/outputs/output_files/spc.py
 src/ase2sprkkr/outputs/readers/__init__.py
 src/ase2sprkkr/outputs/readers/arpes.py
 src/ase2sprkkr/outputs/readers/default.py
 src/ase2sprkkr/outputs/readers/scf.py
 src/ase2sprkkr/outputs/test/__init__.py
 src/ase2sprkkr/outputs/test/init_tests.py
```

### Comparing `ase2sprkkr-2.1.0/tests/test.py` & `ase2sprkkr-2.1.1/tests/test.py`

 * *Files identical despite different names*

