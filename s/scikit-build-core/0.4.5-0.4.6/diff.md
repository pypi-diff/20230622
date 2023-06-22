# Comparing `tmp/scikit_build_core-0.4.5.tar.gz` & `tmp/scikit_build_core-0.4.6.tar.gz`

## Comparing `scikit_build_core-0.4.5.tar` & `scikit_build_core-0.4.6.tar`

### file list

```diff
@@ -1,252 +1,267 @@
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/.git_archival.txt
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/.gitattributes
--rw-r--r--   0        0        0     2215 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/.packit.yaml
--rw-r--r--   0        0        0     3309 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/.pre-commit-config.yaml
--rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/.readthedocs.yml
--rw-r--r--   0        0        0     5990 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/noxfile.py
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/.distro/packit.toml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/.distro/python-scikit-build-core.rpmlintrc
--rw-r--r--   0        0        0     1249 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/.distro/python-scikit-build-core.spec
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/.distro/.fmf/version
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/.distro/plans/main.fmf.dist-git
--rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/.distro/plans/rpmlint.fmf
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/.distro/plans/smoke.fmf
--rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/.distro/tests/rpmlint.fmf
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/.distro/tests/smoke.fmf
--rw-r--r--   0        0        0     9969 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/.github/CONTRIBUTING.md
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/.github/codecov.yml
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/.github/dependabot.yml
--rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/.github/matchers/pylint.json
--rw-r--r--   0        0        0      783 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/.github/workflows/cd.yml
--rw-r--r--   0        0        0     6827 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/.github/workflows/ci.yml
--rw-r--r--   0        0        0    16489 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/docs/changelog.md
--rw-r--r--   0        0        0     3809 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/docs/cmakelists.md
--rw-r--r--   0        0        0     1740 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/docs/conf.py
--rw-r--r--   0        0        0    12730 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/docs/configuration.md
--rw-r--r--   0        0        0     9062 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/docs/getting_started.md
--rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/docs/index.md
--rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/docs/api/scikit_build_core.build.rst
--rw-r--r--   0        0        0     1375 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/docs/api/scikit_build_core.builder.rst
--rw-r--r--   0        0        0     1735 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/docs/api/scikit_build_core.file_api.model.rst
--rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/docs/api/scikit_build_core.file_api.rst
--rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/docs/api/scikit_build_core.metadata.rst
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/docs/api/scikit_build_core.resources.find_python.rst
--rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/docs/api/scikit_build_core.resources.rst
--rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/docs/api/scikit_build_core.rst
--rw-r--r--   0        0        0     1044 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/docs/api/scikit_build_core.settings.rst
--rw-r--r--   0        0        0      829 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/docs/api/scikit_build_core.setuptools.rst
--rw-r--r--   0        0        0     2389 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/docs/examples/downstream/nanobind_example/CMakeLists.txt
--rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/docs/examples/downstream/nanobind_example/LICENSE
--rw-r--r--   0        0        0     2208 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/docs/examples/downstream/nanobind_example/README.md
--rw-r--r--   0        0        0     1114 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/docs/examples/downstream/nanobind_example/pyproject.toml
--rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/docs/examples/downstream/nanobind_example/src/nanobind_example_ext.cpp
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/docs/examples/downstream/nanobind_example/src/nanobind_example/__init__.py
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/docs/examples/downstream/nanobind_example/tests/test_basic.py
--rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/docs/examples/downstream/pybind11_example/CMakeLists.txt
--rw-r--r--   0        0        0     2182 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/docs/examples/downstream/pybind11_example/LICENSE
--rw-r--r--   0        0        0     1993 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/docs/examples/downstream/pybind11_example/README.md
--rw-r--r--   0        0        0     1260 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/docs/examples/downstream/pybind11_example/pyproject.toml
--rw-r--r--   0        0        0      867 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/docs/examples/downstream/pybind11_example/src/main.cpp
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/docs/examples/downstream/pybind11_example/src/scikit_build_example/__init__.py
--rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/docs/examples/downstream/pybind11_example/tests/test_basic.py
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/docs/examples/getting_started/test.py
--rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/docs/examples/getting_started/abi3/CMakeLists.txt
--rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/docs/examples/getting_started/abi3/example.c
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/docs/examples/getting_started/abi3/pyproject.toml
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/docs/examples/getting_started/c/CMakeLists.txt
--rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/docs/examples/getting_started/c/example.c
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/docs/examples/getting_started/c/pyproject.toml
--rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/docs/examples/getting_started/cython/CMakeLists.txt
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/docs/examples/getting_started/cython/example.pyx
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/docs/examples/getting_started/cython/pyproject.toml
--rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/docs/examples/getting_started/fortran/CMakeLists.txt
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/docs/examples/getting_started/fortran/example.f
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/docs/examples/getting_started/fortran/pyproject.toml
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/docs/examples/getting_started/pybind11/CMakeLists.txt
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/docs/examples/getting_started/pybind11/example.cpp
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/docs/examples/getting_started/pybind11/pyproject.toml
--rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/docs/examples/getting_started/swig/CMakeLists.txt
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/docs/examples/getting_started/swig/example.c
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/docs/examples/getting_started/swig/example.i
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/docs/examples/getting_started/swig/pyproject.toml
--rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/src/scikit_build_core/__init__.py
--rw-r--r--   0        0        0     3830 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/src/scikit_build_core/_logging.py
--rw-r--r--   0        0        0     2279 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/src/scikit_build_core/_shutil.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/src/scikit_build_core/_version.py
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/src/scikit_build_core/_version.pyi
--rw-r--r--   0        0        0     8594 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/src/scikit_build_core/cmake.py
--rw-r--r--   0        0        0     2093 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/src/scikit_build_core/errors.py
--rw-r--r--   0        0        0     3989 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/src/scikit_build_core/program_search.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/src/scikit_build_core/py.typed
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/src/scikit_build_core/_compat/__init__.py
--rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/src/scikit_build_core/_compat/builtins.py
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/src/scikit_build_core/_compat/tomllib.py
--rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/src/scikit_build_core/_compat/typing.py
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/src/scikit_build_core/_compat/importlib/__init__.py
--rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/src/scikit_build_core/_compat/importlib/metadata.py
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/src/scikit_build_core/_compat/importlib/resources.py
--rw-r--r--   0        0        0     3972 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/src/scikit_build_core/build/__init__.py
--rw-r--r--   0        0        0     1293 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/src/scikit_build_core/build/_file_processor.py
--rw-r--r--   0        0        0      796 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/src/scikit_build_core/build/_init.py
--rw-r--r--   0        0        0     1396 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/src/scikit_build_core/build/_pathutil.py
--rw-r--r--   0        0        0      922 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/src/scikit_build_core/build/_scripts.py
--rw-r--r--   0        0        0     8169 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/src/scikit_build_core/build/_wheelfile.py
--rw-r--r--   0        0        0     4007 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/src/scikit_build_core/build/sdist.py
--rw-r--r--   0        0        0    10674 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/src/scikit_build_core/build/wheel.py
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/src/scikit_build_core/builder/__init__.py
--rw-r--r--   0        0        0     7054 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/src/scikit_build_core/builder/builder.py
--rw-r--r--   0        0        0     3337 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/src/scikit_build_core/builder/generator.py
--rw-r--r--   0        0        0     3547 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/src/scikit_build_core/builder/get_requires.py
--rw-r--r--   0        0        0     1800 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/src/scikit_build_core/builder/macos.py
--rw-r--r--   0        0        0     4990 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/src/scikit_build_core/builder/sysconfig.py
--rw-r--r--   0        0        0     4290 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/src/scikit_build_core/builder/wheel_tag.py
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/src/scikit_build_core/file_api/__init__.py
--rw-r--r--   0        0        0     2453 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/src/scikit_build_core/file_api/_cattrs_converter.py
--rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/src/scikit_build_core/file_api/query.py
--rw-r--r--   0        0        0     4033 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/src/scikit_build_core/file_api/reply.py
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/src/scikit_build_core/file_api/model/__init__.py
--rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/src/scikit_build_core/file_api/model/cache.py
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/src/scikit_build_core/file_api/model/cmakefiles.py
--rw-r--r--   0        0        0     3269 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/src/scikit_build_core/file_api/model/codemodel.py
--rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/src/scikit_build_core/file_api/model/common.py
--rw-r--r--   0        0        0     1699 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/src/scikit_build_core/file_api/model/directory.py
--rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/src/scikit_build_core/file_api/model/index.py
--rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/src/scikit_build_core/file_api/model/toolchains.py
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/src/scikit_build_core/metadata/__init__.py
--rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/src/scikit_build_core/metadata/fancy_pypi_readme.py
--rw-r--r--   0        0        0      921 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/src/scikit_build_core/metadata/setuptools_scm.py
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/src/scikit_build_core/resources/__init__.py
--rw-r--r--   0        0        0     4184 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/src/scikit_build_core/resources/_editable_redirect.py
--rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/src/scikit_build_core/resources/known_wheels.toml
--rw-r--r--   0        0        0     5477 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/src/scikit_build_core/resources/find_python/Copyright.txt
--rw-r--r--   0        0        0    23174 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/src/scikit_build_core/resources/find_python/FindPackageHandleStandardArgs.cmake
--rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/src/scikit_build_core/resources/find_python/FindPackageMessage.cmake
--rw-r--r--   0        0        0    22536 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/src/scikit_build_core/resources/find_python/FindPython.cmake
--rw-r--r--   0        0        0    19036 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/src/scikit_build_core/resources/find_python/FindPython3.cmake
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/src/scikit_build_core/resources/find_python/__init__.py
--rw-r--r--   0        0        0   198528 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/src/scikit_build_core/resources/find_python/FindPython/Support.cmake
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/src/scikit_build_core/settings/__init__.py
--rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/src/scikit_build_core/settings/_load_provider.py
--rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/src/scikit_build_core/settings/metadata.py
--rw-r--r--   0        0        0     5642 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/src/scikit_build_core/settings/skbuild_model.py
--rw-r--r--   0        0        0     4916 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/src/scikit_build_core/settings/skbuild_read_settings.py
--rw-r--r--   0        0        0    18214 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/src/scikit_build_core/settings/sources.py
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/src/scikit_build_core/setuptools/__init__.py
--rw-r--r--   0        0        0     7759 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/src/scikit_build_core/setuptools/build_cmake.py
--rw-r--r--   0        0        0     1894 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/src/scikit_build_core/setuptools/build_meta.py
--rw-r--r--   0        0        0     1302 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/src/scikit_build_core/setuptools/wrapper.py
--rw-r--r--   0        0        0     9442 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/conftest.py
--rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/constraints.txt
--rw-r--r--   0        0        0     6449 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/test_builder.py
--rw-r--r--   0        0        0     3524 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/test_cmake_config.py
--rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/test_custom_modules.py
--rw-r--r--   0        0        0     8426 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/test_dynamic_metadata.py
--rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/test_file_processor.py
--rw-r--r--   0        0        0     3107 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/test_fileapi.py
--rw-r--r--   0        0        0     2073 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/test_fortran.py
--rw-r--r--   0        0        0    15811 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/test_generator_default.py
--rw-r--r--   0        0        0     2856 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/test_get_requires.py
--rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/test_logging.py
--rw-r--r--   0        0        0     1789 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/test_module_dir.py
--rw-r--r--   0        0        0     1874 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/test_name_main.py
--rw-r--r--   0        0        0     1274 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/test_prepare_metadata.py
--rw-r--r--   0        0        0     1785 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/test_process_scripts.py
--rw-r--r--   0        0        0     4009 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/test_program_search.py
--rw-r--r--   0        0        0     1758 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/test_pyproject_abi3.py
--rw-r--r--   0        0        0     2397 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/test_pyproject_extra_dirs.py
--rw-r--r--   0        0        0     8248 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/test_pyproject_pep517.py
--rw-r--r--   0        0        0     4572 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/test_pyproject_pep518.py
--rw-r--r--   0        0        0     2099 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/test_pyproject_pep660.py
--rw-r--r--   0        0        0    14021 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/test_settings.py
--rw-r--r--   0        0        0     1780 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/test_setuptools_abi3.py
--rw-r--r--   0        0        0     3982 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/test_setuptools_pep517.py
--rw-r--r--   0        0        0     1985 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/test_setuptools_pep518.py
--rw-r--r--   0        0        0     3067 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/test_simple_pure.py
--rw-r--r--   0        0        0     4034 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/test_simplest_c.py
--rw-r--r--   0        0        0    12743 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/test_skbuild_settings.py
--rw-r--r--   0        0        0     2469 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/test_wheelfile_utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/api/simple_pure/.cmake/api/v1/query/cache-v2
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/api/simple_pure/.cmake/api/v1/query/cmakeFiles-v1
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/api/simple_pure/.cmake/api/v1/query/codemodel-v2
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/api/simple_pure/.cmake/api/v1/query/toolchains-v1
--rw-r--r--   0        0        0    20671 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/api/simple_pure/.cmake/api/v1/reply/cache-v2-2dececcab32f1eda138d.json
--rw-r--r--   0        0        0     3209 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/api/simple_pure/.cmake/api/v1/reply/cmakeFiles-v1-74870fd87af7f965b597.json
--rw-r--r--   0        0        0     1045 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/api/simple_pure/.cmake/api/v1/reply/codemodel-v2-ea39b5a28cb1a3e0a069.json
--rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/api/simple_pure/.cmake/api/v1/reply/directory-.-5e7a28751b0c9235cbe7.json
--rw-r--r--   0        0        0     1795 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/api/simple_pure/.cmake/api/v1/reply/index-2022-09-12T15-23-13-0135.json
--rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/api/simple_pure/.cmake/api/v1/reply/target-simple_pure-7eb73eb5c359b881e083.json
--rw-r--r--   0        0        0     1416 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/api/simple_pure/.cmake/api/v1/reply/toolchains-v1-06b92b86597808b5f980.json
--rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/packages/abi3_pyproject_ext/CMakeLists.txt
--rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/packages/abi3_pyproject_ext/abi3_example.c
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/packages/abi3_pyproject_ext/pyproject.toml
--rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/packages/abi3_setuptools_ext/CMakeLists.txt
--rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/packages/abi3_setuptools_ext/abi3_example.c
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/packages/abi3_setuptools_ext/pyproject.toml
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/packages/abi3_setuptools_ext/setup.cfg
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/packages/abi3_setuptools_ext/setup.py
--rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/packages/custom_cmake/CMakeLists.txt
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/packages/custom_cmake/pyproject.toml
--rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/packages/custom_cmake/extern/pyproject.toml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/packages/custom_cmake/extern/custom_cmake_testing_stuff/__init__.py
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/packages/custom_cmake/extern/custom_cmake_testing_stuff/cmake_modules/ExampleInclude.cmake
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/packages/custom_cmake/extern/custom_cmake_testing_stuff/cmake_modules/__init__.py
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/packages/custom_cmake/extern/custom_cmake_testing_stuff/cmake_prefix/ExamplePkgConfig.cmake
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/packages/custom_cmake/extern/custom_cmake_testing_stuff/cmake_prefix/__init__.py
--rwxr-xr-x   0        0        0       82 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/packages/custom_cmake/scripts/script1
--rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/packages/dynamic_metadata/CMakeLists.txt
--rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/packages/dynamic_metadata/dual_project.toml
--rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/packages/dynamic_metadata/faulty_dual_project.toml
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/packages/dynamic_metadata/faulty_project.toml
--rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/packages/dynamic_metadata/local_pyproject.toml
--rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/packages/dynamic_metadata/plugin_project.toml
--rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/packages/dynamic_metadata/pyproject.toml
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/packages/dynamic_metadata/warn_project.toml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/packages/dynamic_metadata/plugins/local/version/__init__.py
--rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/packages/dynamic_metadata/plugins/local/version/nested/__init__.py
--rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/packages/dynamic_metadata/src/module.c
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/packages/dynamic_metadata/src/dynamic/__init__.py
--rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/packages/filepath_pure/CMakeLists.txt
--rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/packages/filepath_pure/pyproject.toml
--rw-r--r--   0        0        0     1360 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/packages/fortran_example/CMakeLists.txt
--rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/packages/fortran_example/fib1.f
--rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/packages/fortran_example/pyproject.toml
--rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/packages/mixed_setuptools/CMakeLists.txt
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/packages/mixed_setuptools/pyproject.toml
--rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/packages/mixed_setuptools/setup.cfg
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/packages/mixed_setuptools/setup.py
--rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/packages/mixed_setuptools/src/main.cpp
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/packages/mixed_setuptools/src/mixed_setuptools/__init__.py
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/packages/mixed_setuptools/src/mixed_setuptools/_core.pyi
--rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/packages/simple_pure/CMakeLists.txt
--rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/packages/simple_pure/simple_pure.cpp
--rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/packages/simple_pyproject_ext/CMakeLists.txt
--rw-r--r--   0        0        0    11346 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/packages/simple_pyproject_ext/LICENSE
--rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/packages/simple_pyproject_ext/pyproject.toml
--rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/packages/simple_pyproject_ext/src/main.cpp
--rw-r--r--   0        0        0    11346 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/packages/simple_pyproject_source_dir/LICENSE
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/packages/simple_pyproject_source_dir/pyproject.toml
--rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/packages/simple_pyproject_source_dir/src/CMakeLists.txt
--rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/packages/simple_pyproject_source_dir/src/main.cpp
--rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/packages/simple_setuptools_ext/CMakeLists.txt
--rw-r--r--   0        0        0    11346 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/packages/simple_setuptools_ext/LICENSE
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/packages/simple_setuptools_ext/pyproject.toml
--rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/packages/simple_setuptools_ext/setup.py
--rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/packages/simple_setuptools_ext/src/main.cpp
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/packages/simplest_c/.gitignore
--rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/packages/simplest_c/CMakeLists.txt
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/packages/simplest_c/pyproject.toml
--rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/packages/simplest_c/src/module.c
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/packages/simplest_c/src/not_a_package/simple.txt
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/packages/simplest_c/src/simplest/__init__.py
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/packages/simplest_c/src/simplest/_module.pyi
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/packages/simplest_c/src/simplest/artifact_ignored.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/packages/simplest_c/src/simplest/data.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/packages/simplest_c/src/simplest/excluded.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/packages/simplest_c/src/simplest/ignored.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/packages/simplest_c/src/simplest/ignored_included.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/tests/packages/simplest_c/src/simplest/sdist_only.txt
--rw-r--r--   0        0        0     2510 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/.gitignore
--rw-r--r--   0        0        0    11346 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/LICENSE
--rw-r--r--   0        0        0    10816 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/README.md
--rw-r--r--   0        0        0     8587 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/pyproject.toml
--rw-r--r--   0        0        0    13815 2020-02-02 00:00:00.000000 scikit_build_core-0.4.5/PKG-INFO
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/.git_archival.txt
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/.gitattributes
+-rw-r--r--   0        0        0     2253 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/.packit.yaml
+-rw-r--r--   0        0        0     3380 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/.readthedocs.yml
+-rw-r--r--   0        0        0     6527 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/noxfile.py
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/.fmf/version
+-rw-r--r--   0        0        0     9969 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/.github/CONTRIBUTING.md
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/.github/codecov.yml
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/.github/dependabot.yml
+-rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/.github/matchers/pylint.json
+-rw-r--r--   0        0        0      783 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/.github/workflows/cd.yml
+-rw-r--r--   0        0        0     7074 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/.github/workflows/ci.yml
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/distro/packit.toml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/distro/python-scikit-build-core.rpmlintrc
+-rw-r--r--   0        0        0     1248 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/distro/python-scikit-build-core.spec
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/distro/plans/examples.fmf
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/distro/plans/main.fmf.dist-git
+-rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/distro/plans/rpmlint.fmf
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/distro/plans/smoke.fmf
+-rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/distro/tests/rpmlint.fmf
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/distro/tests/smoke.fmf
+-rw-r--r--   0        0        0    17544 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/docs/changelog.md
+-rw-r--r--   0        0        0     3809 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/docs/cmakelists.md
+-rw-r--r--   0        0        0     3399 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/docs/conf.py
+-rw-r--r--   0        0        0    12729 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/docs/configuration.md
+-rw-r--r--   0        0        0    10617 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/docs/getting_started.md
+-rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/docs/index.md
+-rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/docs/man.md
+-rw-r--r--   0        0        0     3315 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/docs/migration_guide.md
+-rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/docs/api/scikit_build_core.build.rst
+-rw-r--r--   0        0        0     1375 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/docs/api/scikit_build_core.builder.rst
+-rw-r--r--   0        0        0     1735 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/docs/api/scikit_build_core.file_api.model.rst
+-rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/docs/api/scikit_build_core.file_api.rst
+-rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/docs/api/scikit_build_core.metadata.rst
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/docs/api/scikit_build_core.resources.find_python.rst
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/docs/api/scikit_build_core.resources.rst
+-rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/docs/api/scikit_build_core.rst
+-rw-r--r--   0        0        0     1044 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/docs/api/scikit_build_core.settings.rst
+-rw-r--r--   0        0        0      829 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/docs/api/scikit_build_core.setuptools.rst
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/docs/examples/main.fmf
+-rwxr-xr-x   0        0        0      865 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/docs/examples/test.sh
+-rw-r--r--   0        0        0     2389 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/docs/examples/downstream/nanobind_example/CMakeLists.txt
+-rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/docs/examples/downstream/nanobind_example/LICENSE
+-rw-r--r--   0        0        0     2208 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/docs/examples/downstream/nanobind_example/README.md
+-rw-r--r--   0        0        0     1114 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/docs/examples/downstream/nanobind_example/pyproject.toml
+-rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/docs/examples/downstream/nanobind_example/src/nanobind_example_ext.cpp
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/docs/examples/downstream/nanobind_example/src/nanobind_example/__init__.py
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/docs/examples/downstream/nanobind_example/tests/test_basic.py
+-rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/docs/examples/downstream/pybind11_example/CMakeLists.txt
+-rw-r--r--   0        0        0     2182 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/docs/examples/downstream/pybind11_example/LICENSE
+-rw-r--r--   0        0        0     1993 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/docs/examples/downstream/pybind11_example/README.md
+-rw-r--r--   0        0        0     1260 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/docs/examples/downstream/pybind11_example/pyproject.toml
+-rw-r--r--   0        0        0      867 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/docs/examples/downstream/pybind11_example/src/main.cpp
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/docs/examples/downstream/pybind11_example/src/scikit_build_example/__init__.py
+-rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/docs/examples/downstream/pybind11_example/tests/test_basic.py
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/docs/examples/getting_started/test.py
+-rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/docs/examples/getting_started/abi3/CMakeLists.txt
+-rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/docs/examples/getting_started/abi3/example.c
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/docs/examples/getting_started/abi3/main.fmf
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/docs/examples/getting_started/abi3/pyproject.toml
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/docs/examples/getting_started/c/CMakeLists.txt
+-rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/docs/examples/getting_started/c/example.c
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/docs/examples/getting_started/c/main.fmf
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/docs/examples/getting_started/c/pyproject.toml
+-rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/docs/examples/getting_started/cython/CMakeLists.txt
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/docs/examples/getting_started/cython/example.pyx
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/docs/examples/getting_started/cython/main.fmf
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/docs/examples/getting_started/cython/pyproject.toml
+-rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/docs/examples/getting_started/fortran/CMakeLists.txt
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/docs/examples/getting_started/fortran/example.f
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/docs/examples/getting_started/fortran/main.fmf
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/docs/examples/getting_started/fortran/pyproject.toml
+-rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/docs/examples/getting_started/nanobind/CMakeLists.txt
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/docs/examples/getting_started/nanobind/example.cpp
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/docs/examples/getting_started/nanobind/pyproject.toml
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/docs/examples/getting_started/pybind11/CMakeLists.txt
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/docs/examples/getting_started/pybind11/example.cpp
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/docs/examples/getting_started/pybind11/main.fmf
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/docs/examples/getting_started/pybind11/pyproject.toml
+-rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/docs/examples/getting_started/swig/CMakeLists.txt
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/docs/examples/getting_started/swig/example.c
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/docs/examples/getting_started/swig/example.i
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/docs/examples/getting_started/swig/main.fmf
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/docs/examples/getting_started/swig/pyproject.toml
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/src/scikit_build_core/__init__.py
+-rw-r--r--   0        0        0     3830 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/src/scikit_build_core/_logging.py
+-rw-r--r--   0        0        0     3062 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/src/scikit_build_core/_shutil.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/src/scikit_build_core/_version.py
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/src/scikit_build_core/_version.pyi
+-rw-r--r--   0        0        0     8586 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/src/scikit_build_core/cmake.py
+-rw-r--r--   0        0        0     2093 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/src/scikit_build_core/errors.py
+-rw-r--r--   0        0        0     3989 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/src/scikit_build_core/program_search.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/src/scikit_build_core/py.typed
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/src/scikit_build_core/_compat/__init__.py
+-rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/src/scikit_build_core/_compat/builtins.py
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/src/scikit_build_core/_compat/tomllib.py
+-rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/src/scikit_build_core/_compat/typing.py
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/src/scikit_build_core/_compat/importlib/__init__.py
+-rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/src/scikit_build_core/_compat/importlib/metadata.py
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/src/scikit_build_core/_compat/importlib/resources.py
+-rw-r--r--   0        0        0     3972 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/src/scikit_build_core/build/__init__.py
+-rw-r--r--   0        0        0     1293 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/src/scikit_build_core/build/_file_processor.py
+-rw-r--r--   0        0        0      796 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/src/scikit_build_core/build/_init.py
+-rw-r--r--   0        0        0     1396 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/src/scikit_build_core/build/_pathutil.py
+-rw-r--r--   0        0        0      922 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/src/scikit_build_core/build/_scripts.py
+-rw-r--r--   0        0        0     8161 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/src/scikit_build_core/build/_wheelfile.py
+-rw-r--r--   0        0        0     4007 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/src/scikit_build_core/build/sdist.py
+-rw-r--r--   0        0        0    10814 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/src/scikit_build_core/build/wheel.py
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/src/scikit_build_core/builder/__init__.py
+-rw-r--r--   0        0        0     7054 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/src/scikit_build_core/builder/builder.py
+-rw-r--r--   0        0        0     3337 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/src/scikit_build_core/builder/generator.py
+-rw-r--r--   0        0        0     3547 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/src/scikit_build_core/builder/get_requires.py
+-rw-r--r--   0        0        0     1800 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/src/scikit_build_core/builder/macos.py
+-rw-r--r--   0        0        0     4990 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/src/scikit_build_core/builder/sysconfig.py
+-rw-r--r--   0        0        0     4290 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/src/scikit_build_core/builder/wheel_tag.py
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/src/scikit_build_core/file_api/__init__.py
+-rw-r--r--   0        0        0     2453 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/src/scikit_build_core/file_api/_cattrs_converter.py
+-rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/src/scikit_build_core/file_api/query.py
+-rw-r--r--   0        0        0     4033 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/src/scikit_build_core/file_api/reply.py
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/src/scikit_build_core/file_api/model/__init__.py
+-rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/src/scikit_build_core/file_api/model/cache.py
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/src/scikit_build_core/file_api/model/cmakefiles.py
+-rw-r--r--   0        0        0     3269 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/src/scikit_build_core/file_api/model/codemodel.py
+-rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/src/scikit_build_core/file_api/model/common.py
+-rw-r--r--   0        0        0     1699 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/src/scikit_build_core/file_api/model/directory.py
+-rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/src/scikit_build_core/file_api/model/index.py
+-rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/src/scikit_build_core/file_api/model/toolchains.py
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/src/scikit_build_core/metadata/__init__.py
+-rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/src/scikit_build_core/metadata/fancy_pypi_readme.py
+-rw-r--r--   0        0        0      921 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/src/scikit_build_core/metadata/setuptools_scm.py
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/src/scikit_build_core/resources/__init__.py
+-rw-r--r--   0        0        0     4184 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/src/scikit_build_core/resources/_editable_redirect.py
+-rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/src/scikit_build_core/resources/known_wheels.toml
+-rw-r--r--   0        0        0     5477 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/src/scikit_build_core/resources/find_python/Copyright.txt
+-rw-r--r--   0        0        0    23174 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/src/scikit_build_core/resources/find_python/FindPackageHandleStandardArgs.cmake
+-rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/src/scikit_build_core/resources/find_python/FindPackageMessage.cmake
+-rw-r--r--   0        0        0    22536 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/src/scikit_build_core/resources/find_python/FindPython.cmake
+-rw-r--r--   0        0        0    19036 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/src/scikit_build_core/resources/find_python/FindPython3.cmake
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/src/scikit_build_core/resources/find_python/__init__.py
+-rw-r--r--   0        0        0   198528 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/src/scikit_build_core/resources/find_python/FindPython/Support.cmake
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/src/scikit_build_core/settings/__init__.py
+-rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/src/scikit_build_core/settings/_load_provider.py
+-rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/src/scikit_build_core/settings/metadata.py
+-rw-r--r--   0        0        0     5690 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/src/scikit_build_core/settings/skbuild_model.py
+-rw-r--r--   0        0        0     4916 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/src/scikit_build_core/settings/skbuild_read_settings.py
+-rw-r--r--   0        0        0    18214 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/src/scikit_build_core/settings/sources.py
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/src/scikit_build_core/setuptools/__init__.py
+-rw-r--r--   0        0        0     7759 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/src/scikit_build_core/setuptools/build_cmake.py
+-rw-r--r--   0        0        0     1894 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/src/scikit_build_core/setuptools/build_meta.py
+-rw-r--r--   0        0        0     1302 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/src/scikit_build_core/setuptools/wrapper.py
+-rw-r--r--   0        0        0     9491 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/conftest.py
+-rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/constraints.txt
+-rw-r--r--   0        0        0     6449 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/test_builder.py
+-rw-r--r--   0        0        0     3524 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/test_cmake_config.py
+-rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/test_custom_modules.py
+-rw-r--r--   0        0        0     8426 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/test_dynamic_metadata.py
+-rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/test_file_processor.py
+-rw-r--r--   0        0        0     3107 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/test_fileapi.py
+-rw-r--r--   0        0        0     2096 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/test_fortran.py
+-rw-r--r--   0        0        0    15811 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/test_generator_default.py
+-rw-r--r--   0        0        0     2856 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/test_get_requires.py
+-rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/test_logging.py
+-rw-r--r--   0        0        0     1789 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/test_module_dir.py
+-rw-r--r--   0        0        0     1874 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/test_name_main.py
+-rw-r--r--   0        0        0     1274 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/test_prepare_metadata.py
+-rw-r--r--   0        0        0     1785 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/test_process_scripts.py
+-rw-r--r--   0        0        0     4009 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/test_program_search.py
+-rw-r--r--   0        0        0     1758 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/test_pyproject_abi3.py
+-rw-r--r--   0        0        0     2397 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/test_pyproject_extra_dirs.py
+-rw-r--r--   0        0        0     8248 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/test_pyproject_pep517.py
+-rw-r--r--   0        0        0     4571 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/test_pyproject_pep518.py
+-rw-r--r--   0        0        0     2099 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/test_pyproject_pep660.py
+-rw-r--r--   0        0        0    14021 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/test_settings.py
+-rw-r--r--   0        0        0     1780 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/test_setuptools_abi3.py
+-rw-r--r--   0        0        0     3982 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/test_setuptools_pep517.py
+-rw-r--r--   0        0        0     1985 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/test_setuptools_pep518.py
+-rw-r--r--   0        0        0     1307 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/test_shutil.py
+-rw-r--r--   0        0        0     3067 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/test_simple_pure.py
+-rw-r--r--   0        0        0     4034 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/test_simplest_c.py
+-rw-r--r--   0        0        0    12743 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/test_skbuild_settings.py
+-rw-r--r--   0        0        0     2469 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/test_wheelfile_utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/api/simple_pure/.cmake/api/v1/query/cache-v2
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/api/simple_pure/.cmake/api/v1/query/cmakeFiles-v1
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/api/simple_pure/.cmake/api/v1/query/codemodel-v2
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/api/simple_pure/.cmake/api/v1/query/toolchains-v1
+-rw-r--r--   0        0        0    20671 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/api/simple_pure/.cmake/api/v1/reply/cache-v2-2dececcab32f1eda138d.json
+-rw-r--r--   0        0        0     3209 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/api/simple_pure/.cmake/api/v1/reply/cmakeFiles-v1-74870fd87af7f965b597.json
+-rw-r--r--   0        0        0     1045 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/api/simple_pure/.cmake/api/v1/reply/codemodel-v2-ea39b5a28cb1a3e0a069.json
+-rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/api/simple_pure/.cmake/api/v1/reply/directory-.-5e7a28751b0c9235cbe7.json
+-rw-r--r--   0        0        0     1795 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/api/simple_pure/.cmake/api/v1/reply/index-2022-09-12T15-23-13-0135.json
+-rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/api/simple_pure/.cmake/api/v1/reply/target-simple_pure-7eb73eb5c359b881e083.json
+-rw-r--r--   0        0        0     1416 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/api/simple_pure/.cmake/api/v1/reply/toolchains-v1-06b92b86597808b5f980.json
+-rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/packages/abi3_pyproject_ext/CMakeLists.txt
+-rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/packages/abi3_pyproject_ext/abi3_example.c
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/packages/abi3_pyproject_ext/pyproject.toml
+-rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/packages/abi3_setuptools_ext/CMakeLists.txt
+-rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/packages/abi3_setuptools_ext/abi3_example.c
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/packages/abi3_setuptools_ext/pyproject.toml
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/packages/abi3_setuptools_ext/setup.cfg
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/packages/abi3_setuptools_ext/setup.py
+-rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/packages/custom_cmake/CMakeLists.txt
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/packages/custom_cmake/pyproject.toml
+-rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/packages/custom_cmake/extern/pyproject.toml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/packages/custom_cmake/extern/custom_cmake_testing_stuff/__init__.py
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/packages/custom_cmake/extern/custom_cmake_testing_stuff/cmake_modules/ExampleInclude.cmake
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/packages/custom_cmake/extern/custom_cmake_testing_stuff/cmake_modules/__init__.py
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/packages/custom_cmake/extern/custom_cmake_testing_stuff/cmake_prefix/ExamplePkgConfig.cmake
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/packages/custom_cmake/extern/custom_cmake_testing_stuff/cmake_prefix/__init__.py
+-rwxr-xr-x   0        0        0       82 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/packages/custom_cmake/scripts/script1
+-rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/packages/dynamic_metadata/CMakeLists.txt
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/packages/dynamic_metadata/dual_project.toml
+-rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/packages/dynamic_metadata/faulty_dual_project.toml
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/packages/dynamic_metadata/faulty_project.toml
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/packages/dynamic_metadata/local_pyproject.toml
+-rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/packages/dynamic_metadata/plugin_project.toml
+-rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/packages/dynamic_metadata/pyproject.toml
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/packages/dynamic_metadata/warn_project.toml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/packages/dynamic_metadata/plugins/local/version/__init__.py
+-rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/packages/dynamic_metadata/plugins/local/version/nested/__init__.py
+-rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/packages/dynamic_metadata/src/module.c
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/packages/dynamic_metadata/src/dynamic/__init__.py
+-rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/packages/filepath_pure/CMakeLists.txt
+-rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/packages/filepath_pure/pyproject.toml
+-rw-r--r--   0        0        0     1360 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/packages/fortran_example/CMakeLists.txt
+-rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/packages/fortran_example/fib1.f
+-rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/packages/fortran_example/pyproject.toml
+-rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/packages/mixed_setuptools/CMakeLists.txt
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/packages/mixed_setuptools/pyproject.toml
+-rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/packages/mixed_setuptools/setup.cfg
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/packages/mixed_setuptools/setup.py
+-rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/packages/mixed_setuptools/src/main.cpp
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/packages/mixed_setuptools/src/mixed_setuptools/__init__.py
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/packages/mixed_setuptools/src/mixed_setuptools/_core.pyi
+-rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/packages/simple_pure/CMakeLists.txt
+-rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/packages/simple_pure/simple_pure.cpp
+-rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/packages/simple_pyproject_ext/CMakeLists.txt
+-rw-r--r--   0        0        0    11346 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/packages/simple_pyproject_ext/LICENSE
+-rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/packages/simple_pyproject_ext/pyproject.toml
+-rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/packages/simple_pyproject_ext/src/main.cpp
+-rw-r--r--   0        0        0    11346 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/packages/simple_pyproject_source_dir/LICENSE
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/packages/simple_pyproject_source_dir/pyproject.toml
+-rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/packages/simple_pyproject_source_dir/src/CMakeLists.txt
+-rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/packages/simple_pyproject_source_dir/src/main.cpp
+-rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/packages/simple_setuptools_ext/CMakeLists.txt
+-rw-r--r--   0        0        0    11346 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/packages/simple_setuptools_ext/LICENSE
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/packages/simple_setuptools_ext/pyproject.toml
+-rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/packages/simple_setuptools_ext/setup.py
+-rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/packages/simple_setuptools_ext/src/main.cpp
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/packages/simplest_c/.gitignore
+-rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/packages/simplest_c/CMakeLists.txt
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/packages/simplest_c/pyproject.toml
+-rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/packages/simplest_c/src/module.c
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/packages/simplest_c/src/not_a_package/simple.txt
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/packages/simplest_c/src/simplest/__init__.py
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/packages/simplest_c/src/simplest/_module.pyi
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/packages/simplest_c/src/simplest/artifact_ignored.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/packages/simplest_c/src/simplest/data.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/packages/simplest_c/src/simplest/excluded.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/packages/simplest_c/src/simplest/ignored.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/packages/simplest_c/src/simplest/ignored_included.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/packages/simplest_c/src/simplest/sdist_only.txt
+-rw-r--r--   0        0        0     2505 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/.gitignore
+-rw-r--r--   0        0        0    11346 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/LICENSE
+-rw-r--r--   0        0        0    10816 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/README.md
+-rw-r--r--   0        0        0     9166 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/pyproject.toml
+-rw-r--r--   0        0        0    14562 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/PKG-INFO
```

### Comparing `scikit_build_core-0.4.5/.packit.yaml` & `scikit_build_core-0.4.6/.packit.yaml`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 # See the documentation for more information:
 # https://packit.dev/docs/configuration/
 
-specfile_path: .distro/python-scikit-build-core.spec
+specfile_path: distro/python-scikit-build-core.spec
 
 files_to_sync:
-  - src: .distro/python-scikit-build-core.spec
+  - src: distro/python-scikit-build-core.spec
     dest: python-scikit-build-core.spec
   - .packit.yaml
-  - src: .distro/python-scikit-build-core.rpmlintrc
+  - src: distro/python-scikit-build-core.rpmlintrc
     dest: python-scikit-build-core.rpmlintrc
   # tmt setup
-  - src: .distro/.fmf/
+  - src: .fmf/
     dest: .fmf/
-  - src: .distro/plans/
+  - src: distro/plans/
     dest: plans/
     filters:
-      - "- .distro/plans/main.fmf.dist-git"
-      - "- .distro/plans/rpmlint.fmf"
-  - src: .distro/plans/main.fmf.dist-git
+      - "- main.fmf.dist-git"
+      - "- rpmlint.fmf"
+  - src: distro/plans/main.fmf.dist-git
     dest: plans/main.fmf
 upstream_package_name: scikit_build_core
 downstream_package_name: python-scikit-build-core
 update_release: false
 upstream_tag_template: v{version}
 
 jobs:
@@ -29,19 +29,22 @@
     trigger: pull_request
     owner: "@scikit-build"
     project: scikit-build-core
     update_release: true
     release_suffix: "{PACKIT_RPMSPEC_RELEASE}"
     targets:
       - fedora-development
+      - fedora-latest
   - job: tests
     trigger: pull_request
     targets:
-      - fedora-development
-    fmf_path: .distro
+      - fedora-development-x86_64
+      - fedora-latest-x86_64
+      - fedora-development-aarch64
+      - fedora-latest-aarch64
   - job: copr_build
     trigger: commit
     branch: main
     owner: "@scikit-build"
     project: nightly
     targets:
       - fedora-development-x86_64
@@ -50,15 +53,14 @@
       - fedora-latest-aarch64
   - job: tests
     trigger: commit
     branch: main
     targets:
       - fedora-development
       - fedora-latest
-    fmf_path: .distro
   - job: copr_build
     trigger: release
     owner: "@scikit-build"
     project: release
     targets:
       - fedora-development-x86_64
       - fedora-latest-x86_64
```

### Comparing `scikit_build_core-0.4.5/.pre-commit-config.yaml` & `scikit_build_core-0.4.6/.pre-commit-config.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 
   - repo: https://github.com/psf/black
     rev: 23.3.0
     hooks:
       - id: black-jupyter
 
   - repo: https://github.com/asottile/blacken-docs
-    rev: 1.13.0
+    rev: 1.14.0
     hooks:
       - id: blacken-docs
         additional_dependencies: [black==23.3.0]
 
   - repo: https://github.com/cheshirekow/cmake-format-precommit
     rev: v0.6.13
     hooks:
@@ -50,15 +50,15 @@
     hooks:
       - id: prettier
         types_or: [yaml, markdown, html, css, scss, javascript, json]
         args: [--prose-wrap=always]
         exclude: "^tests"
 
   - repo: https://github.com/charliermarsh/ruff-pre-commit
-    rev: v0.0.270
+    rev: v0.0.272
     hooks:
       - id: ruff
         args: ["--fix", "--show-fixes"]
 
   - repo: https://github.com/pre-commit/mirrors-mypy
     rev: v1.3.0
     hooks:
@@ -75,14 +75,15 @@
           - build
           - cattrs
           - cmake
           - exceptiongroup
           - hatch-fancy-pypi-readme
           - importlib-metadata>=6.6.0
           - importlib-resources
+          - markdown-it-py<3 # Python 3.7 compat needed for mypy check
           - ninja
           - packaging
           - pyproject_metadata
           - pytest
           - rich
           - setuptools-scm
           - tomli
@@ -94,15 +95,15 @@
       - id: check-sdist
         args: [--inject-junk]
         additional_dependencies:
           - hatchling
           - hatch-vcs
 
   - repo: https://github.com/codespell-project/codespell
-    rev: v2.2.4
+    rev: v2.2.5
     hooks:
       - id: codespell
         exclude: ^(LICENSE$|src/scikit_build_core/resources/find_python)
 
   - repo: https://github.com/shellcheck-py/shellcheck-py
     rev: v0.9.0.5
     hooks:
```

### Comparing `scikit_build_core-0.4.5/noxfile.py` & `scikit_build_core-0.4.6/noxfile.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,48 +25,51 @@
 @nox.session(reuse_venv=True)
 def pylint(session: nox.Session) -> None:
     """
     Run PyLint.
     """
     # This needs to be installed into the package environment, and is slower
     # than a pre-commit check
-    session.install(
-        "-e.[dev,test]", "pylint", "hatch-fancy-pypi-readme", "setuptools-scm"
-    )
+    session.install("-e.[dev,test,test-meta]", "pylint")
     session.run("pylint", "scikit_build_core", *session.posargs)
 
 
 def _run_tests(
-    session: nox.Session, *, install_args: Sequence[str], run_args: Sequence[str] = ()
+    session: nox.Session,
+    *,
+    install_args: Sequence[str],
+    run_args: Sequence[str] = (),
+    extras: Sequence[str] = (),
 ) -> None:
     posargs = list(session.posargs)
     env = {"PIP_DISABLE_PIP_VERSION_CHECK": "1"}
-    extra = []
+
+    _install_args = list(install_args)
     # This will not work if system CMake is too old (<3.15)
     if shutil.which("cmake") is None and shutil.which("cmake3") is None:
-        extra.append("cmake")
+        _install_args.append("cmake")
     if shutil.which("ninja") is None:
-        extra.append("ninja")
-    if (3, 8) <= sys.version_info < (3, 12):
-        extra.append("numpy")
+        _install_args.append("ninja")
 
-    install_arg = "-e.[test,cov]" if "--cov" in posargs else "-e.[test]"
+    _extras = ["test", *extras]
     if "--cov" in posargs:
+        _extras.append("cov")
         posargs.append("--cov-config=pyproject.toml")
 
-    session.install(install_arg, *extra, *install_args)
+    install_arg = f"-e.[{','.join(_extras)}]"
+    session.install(install_arg, *install_args)
     session.run("pytest", *run_args, *posargs, env=env)
 
 
 @nox.session
 def tests(session: nox.Session) -> None:
     """
     Run the unit and regular tests. Includes coverage if --cov passed.
     """
-    _run_tests(session, install_args=["hatch-fancy-pypi-readme", "setuptools-scm"])
+    _run_tests(session, extras=["test-meta,test-numpy"])
 
 
 @nox.session
 def minimums(session: nox.Session) -> None:
     """
     Test the minimum versions of dependencies.
     """
@@ -81,19 +84,41 @@
 def docs(session: nox.Session) -> None:
     """
     Build the docs. Pass "--serve" to serve.
     """
 
     parser = argparse.ArgumentParser()
     parser.add_argument("--serve", action="store_true", help="Serve after building")
-    args = parser.parse_args(session.posargs)
+    parser.add_argument(
+        "-b", dest="builder", default="html", help="Build target (default: html)"
+    )
+    args, posargs = parser.parse_known_args(session.posargs)
+
+    if args.builder != "html" and args.serve:
+        session.error("Must not specify non-HTML builder with --serve")
 
     session.install(".[docs,pyproject]")
     session.chdir("docs")
-    session.run("sphinx-build", "-M", "html", ".", "_build")
+
+    if args.builder == "linkcheck":
+        session.run(
+            "sphinx-build", "-b", "linkcheck", ".", "_build/linkcheck", *posargs
+        )
+        return
+
+    session.run(
+        "sphinx-build",
+        "-n",  # nitpicky mode
+        "-T",  # full tracebacks
+        "-b",
+        args.builder,
+        ".",
+        f"_build/{args.builder}",
+        *posargs,
+    )
 
     if args.serve:
         print("Launching docs at http://localhost:8000/ - use Ctrl-C to quit")
         session.run("python", "-m", "http.server", "8000", "-d", "_build/html")
 
 
 @nox.session
@@ -121,15 +146,15 @@
     Build an SDist and wheel.
     """
 
     session.install("build")
     session.run("python", "-m", "build", **session.posargs)
 
 
-EXAMPLES = ["c", "abi3", "pybind11", "swig", "cython"]
+EXAMPLES = ["c", "abi3", "pybind11", "nanobind", "swig", "cython"]
 if not sys.platform.startswith("win") and shutil.which("gfortran"):
     EXAMPLES.append("fortran")
 EXAMPLES = [f"getting_started/{n}" for n in EXAMPLES]
 EXAMPLES += ["downstream/pybind11_example", "downstream/nanobind_example"]
 
 
 @nox.session
```

### Comparing `scikit_build_core-0.4.5/.distro/python-scikit-build-core.spec` & `scikit_build_core-0.4.6/distro/python-scikit-build-core.spec`

 * *Files 11% similar despite different names*

```diff
@@ -46,15 +46,15 @@
 %install
 %pyproject_install
 %pyproject_save_files scikit_build_core
 
 
 %check
 %pytest \
-    -m "not isolated"
+    -m "not network"
 
 
 %files -n python3-scikit-build-core -f %{pyproject_files}
 %license LICENSE
 %doc README.md
```

### Comparing `scikit_build_core-0.4.5/.github/CONTRIBUTING.md` & `scikit_build_core-0.4.6/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.5/.github/matchers/pylint.json` & `scikit_build_core-0.4.6/.github/matchers/pylint.json`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.5/.github/workflows/cd.yml` & `scikit_build_core-0.4.6/.github/workflows/cd.yml`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.5/.github/workflows/ci.yml` & `scikit_build_core-0.4.6/.github/workflows/ci.yml`

 * *Files 18% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     name: Format
     runs-on: ubuntu-latest
     timeout-minutes: 5
     steps:
       - uses: actions/checkout@v3
       - uses: actions/setup-python@v4
         with:
-          python-version: "3.10"
+          python-version: "3.11"
       - uses: pre-commit/action@v3.0.0
         with:
           extra_args: --hook-stage manual --all-files
       - name: Run PyLint
         run: |
           echo "::add-matcher::$GITHUB_WORKSPACE/.github/matchers/pylint.json"
           pipx run nox -s pylint
@@ -37,15 +37,15 @@
       Check 🐍 ${{ matrix.python-version }} • CMake ${{ matrix.cmake-version }}
       on ${{ matrix.runs-on }}
     runs-on: ${{ matrix.runs-on }}
     timeout-minutes: 30
     strategy:
       fail-fast: false
       matrix:
-        python-version: ["3.7", "pypy-3.8", "3.11"]
+        python-version: ["3.7", "pypy-3.9", "3.12"]
         runs-on: [ubuntu-latest, macos-latest]
         cmake-version: ["3.15.x"]
 
         include:
           - python-version: "3.7"
             runs-on: windows-2022
             cmake-version: "3.21.x"
@@ -54,48 +54,46 @@
             cmake-version: "3.21.x"
           - python-version: "3.11"
             runs-on: windows-2022
             cmake-version: "3.26.x"
           - python-version: "pypy-3.7"
             runs-on: ubuntu-latest
             cmake-version: "3.15.x"
+          - python-version: "pypy-3.10"
+            runs-on: ubuntu-latest
+            cmake-version: "3.15.x"
           - python-version: "3.8"
             runs-on: ubuntu-latest
             cmake-version: "3.21.x"
           - python-version: "3.9"
             runs-on: ubuntu-latest
             cmake-version: "3.20.x"
           - python-version: "3.10"
             runs-on: ubuntu-latest
             cmake-version: "3.22.x"
+          - python-version: "3.11"
+            runs-on: ubuntu-latest
+            cmake-version: "3.26.x"
           - python-version: "3.8"
             runs-on: windows-2019
             cmake-version: "3.24.x"
-          - python-version: "3.12-dev"
-            runs-on: ubuntu-latest
-            cmake-version: "3.15.x"
-    continue-on-error: ${{ endsWith(matrix.python-version, '-dev') }}
+          - python-version: "3.12"
+            runs-on: windows-latest
+            cmake-version: "3.26.x"
 
     steps:
       - uses: actions/checkout@v3
 
       - uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python-version }}
+          allow-prereleases: true
 
       - name: Install package
-        run: >-
-          pip install -e.[test,cov] cmake ninja rich hatch-fancy-pypi-readme
-          setuptools-scm
-
-      - name: Add NumPy
-        if: >-
-          (matrix.runs-on == 'ubuntu-latest' || matrix.python-version !=
-          'pypy-3.8') && matrix.python-version != '3.12-dev'
-        run: "pip install --only-binary=:all: numpy"
+        run: pip install -e.[test,test-meta,test-numpy,wheels,cov]
 
       - name: Test package
         run: >-
           pytest -ra --showlocals --cov --cov-report=xml --cov-report=term
           --durations=20
 
       - name: Upload coverage report
@@ -103,29 +101,40 @@
         with:
           name:
             ${{ runner.os }}-${{ matrix.python-version }}-${{
             matrix.cmake-version }}
           verbose: true
           token: 6d9cc0e0-158a-41ee-b8f4-0318d3595ac2
 
-      # the min requirements are not compatible with the metadata plugin
-      # packages so we remove those first (they then won't be tested)
+  min:
+    name: Min 🐍 ${{ matrix.python-version }} on ${{ matrix.runs-on }}
+    runs-on: ${{ matrix.runs-on }}
+    timeout-minutes: 30
+    strategy:
+      fail-fast: false
+      matrix:
+        python-version: ["3.7", "3.11"]
+        runs-on: [ubuntu-latest, macos-latest, windows-latest]
+
+    steps:
+      - uses: actions/checkout@v3
+
+      - uses: actions/setup-python@v4
+        with:
+          python-version: ${{ matrix.python-version }}
+
+      # The min requirements are not compatible with some of the extra test
+      # deps, so limit to just built-in deps.
       - name: Min requirements
-        run: |
-          pip uninstall -y cmake hatch-fancy-pypi-readme setuptools-scm
-          pip install --constraint tests/constraints.txt .[test]
+        run: pip install --constraint tests/constraints.txt .[test] ninja
 
       - name: Setup CMake ${{ matrix.cmake-version }}
         uses: jwlawson/actions-setup-cmake@v1.14
-        with:
-          cmake-version: "${{ matrix.cmake-version }}"
 
-      # Skipped on pypy to keep the tests fast
       - name: Test min package
-        if: matrix.python-version != 'pypy-3.8'
         run: pytest -ra --showlocals -Wdefault
 
   cygwin:
     name: Tests on 🐍 3.9 • cygwin
     runs-on: windows-latest
     timeout-minutes: 30
 
@@ -236,28 +245,34 @@
     steps:
       - uses: actions/checkout@v3
 
       - uses: wntrblm/nox@2023.04.22
         with:
           python-versions: "3.11"
 
-      - name: Build docs
-        run: nox -s docs
+      - name: Linkcheck
+        run: nox -s docs -- -b linkcheck
+
+      - name: Manpage
+        run: nox -s docs -- -b man -W
+
+      - name: Build docs with warnings as errors
+        run: nox -s docs -- -W
 
       - name: Check examples
         run: nox -s test_doc_examples
 
       - name: Verify no changes required to API docs
         run: |
           nox -s build_api_docs
           git diff --exit-code
 
   pass:
     if: always()
-    needs: [lint, checks, cygwin, dist, docs]
+    needs: [lint, checks, min, cygwin, dist, docs]
     runs-on: ubuntu-latest
     timeout-minutes: 1
     steps:
       - name: Decide whether the needed jobs succeeded or failed
         uses: re-actors/alls-green@release/v1
         with:
           jobs: ${{ toJSON(needs) }}
```

### Comparing `scikit_build_core-0.4.5/docs/changelog.md` & `scikit_build_core-0.4.6/docs/changelog.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,42 @@
 # Changelog
 
+## Version 0.4.6
+
+This release has one small new feature (access to `${SKBUILD_STATE}` from
+CMake), and fixes an issue when adding read-only files on Windows with Python
+3.7. Some testing and docs infrastructure updates should make it easier for
+downstream packagers to ship scikit-build-core.
+
+Fixes:
+
+- Provide access to current state in CMake by @henryiii in #394
+- Support building older versions of `setuptools_scm` by @henryiii in #390
+- Workaround for Windows Python 3.7 `TemporaryDirectory` bug by @henryiii in
+  #391
+
+Tests:
+
+- Rework testing extras by @henryiii in #395 and #393
+- Add `network` marker by @henryiii in #379
+
+CI:
+
+- Add example tests to Fedora packaging by @LecrisUT in #378
+- Fedora: Correct rsync rule by @LecrisUT in #389
+- Use `not network` for spec by @henryiii in #383
+
+Docs:
+
+- Add migration guide by @vyasr in #356
+- Support building the documentation as a man page by @henryiii in #372
+- Add nanobind example by @henryiii in #375
+- Use `UseSWIG` for swig by @henryiii in #377
+- Fix or hide nitpicks by @henryiii in #370
+
 ## Version 0.4.5
 
 This version fixes issues with output being incorrectly interleaved with logging
 messages. Symlinks are now followed when making SDists. And finally,
 `SKBUILD_SOABI` is now correctly set when cross-compiling on Windows (Warning!
 FindPython still does not report the correct SOABI when cross-compiling to ARM).
```

### Comparing `scikit_build_core-0.4.5/docs/cmakelists.md` & `scikit_build_core-0.4.6/docs/cmakelists.md`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.5/docs/configuration.md` & `scikit_build_core-0.4.6/docs/configuration.md`

 * *Files 0% similar despite different names*

```diff
@@ -53,15 +53,15 @@
 
 `````
 
 ````{tab} Environment
 
 
 ```yaml
-SKBUILD_CMAKE_VERSBOSE: true
+SKBUILD_CMAKE_VERBOSE: true
 SKBUILD_LOGGING_LEVEL: "INFO"
 ```
 
 
 ````
 
 :::{warning}
```

### Comparing `scikit_build_core-0.4.5/docs/getting_started.md` & `scikit_build_core-0.4.6/docs/getting_started.md`

 * *Files 19% similar despite different names*

```diff
@@ -38,14 +38,25 @@
 ├── example.cpp
 ├── pyproject.toml
 └── CMakeLists.txt
 ```
 
 ````
 
+````{tab} nanobind
+
+```
+example-project
+├── example.cpp
+├── pyproject.toml
+└── CMakeLists.txt
+```
+
+````
+
 ````{tab} SWIG
 
 ```
 example-project
 ├── example.c
 ├── example.i
 ├── pyproject.toml
@@ -101,14 +112,22 @@
 
 ```{literalinclude} examples/getting_started/pybind11/example.cpp
 :language: cpp
 ```
 
 ````
 
+````{tab} nanobind
+
+```{literalinclude} examples/getting_started/nanobind/example.cpp
+:language: cpp
+```
+
+````
+
 ````{tab} SWIG
 
 ```{literalinclude} examples/getting_started/swig/example.c
 :language: c
 ```
 
 ```{literalinclude} examples/getting_started/swig/example.i
@@ -157,14 +176,22 @@
 
 ```{literalinclude} examples/getting_started/pybind11/pyproject.toml
 :language: toml
 ```
 
 ````
 
+````{tab} nanobind
+
+```{literalinclude} examples/getting_started/nanobind/pyproject.toml
+:language: toml
+```
+
+````
+
 ````{tab} SWIG
 
 ```{literalinclude} examples/getting_started/swig/pyproject.toml
 :language: toml
 ```
 
 
@@ -276,22 +303,39 @@
 `SKBUILD_PROJECT_VERSION` variables to avoid repeating this information from
 your `pyproject.toml`. You should specify exactly what language you use to keep
 CMake from searching for both `C` and `CXX` compilers (the default).
 
 If you place find Python first, pybind11 will resepct it instead of the classic
 FindPythonInterp/FindPythonLibs mechanisms, which work, but are not as modern.
 Here we set `PYBIND11_NEWPYTHON` to `ON` instead of doing the find Python
-ourselves. Pybind11 places it's config file such that CMake can find it from
+ourselves. Pybind11 places its config file such that CMake can find it from
 site-packages.
 
 You can either use `pybind11_add_module` or `python_add_library` and then link
 to `pybind11::module`, your choice.
 
 ````
 
+````{tab} nanobind
+
+```{literalinclude} examples/getting_started/pybind11/CMakeLists.txt
+:language: cmake
+```
+
+Scikit-build and nanobind require CMake 3.15, so there's no need to set it
+lower than 3.15.
+
+The project line can optionally use `SKBUILD_PROJECT_NAME` and
+`SKBUILD_PROJECT_VERSION` variables to avoid repeating this information from
+your `pyproject.toml`. You should specify exactly what language you use to keep
+CMake from searching for both `C` and `CXX` compilers (the default).
+
+Nanobind places its config file such that CMake can find it from site-packages.
+````
+
 ````{tab} SWIG
 
 ```{literalinclude} examples/getting_started/swig/CMakeLists.txt
 :language: cmake
 ```
 
 Scikit-build requires CMake 3.15, so there's no need to set it lower than 3.15.
@@ -357,7 +401,20 @@
 Or installing it (in a virtualenv, ideally):
 
 ```console
 $ pip install .
 ```
 
 That's it for a basic package!
+
+## Other examples
+
+You can find other examples here:
+
+- [pybind11's scikit_build_core example](https://github.com/pybind/scikit_build_example):
+  An example project using pybind11.
+- [nanobind example](https://github.com/wjakob/nanobind_example): An example
+  project using nanobind and the Stable ABI on Python 3.12+!
+- [scikit-build-example-projects](https://github.com/scikit-build/scikit-build-sample-projects):
+  Some example projects for both scikit-build and scikit-build-core.
+- [Scientific-Python Cookie](https://github.com/scientific-python/cookie): A
+  cookiecutter with 12 backends, including scikit-build-core.
```

### Comparing `scikit_build_core-0.4.5/docs/index.md` & `scikit_build_core-0.4.6/docs/index.md`

 * *Files 27% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 :titlesonly:
 :caption: Guide
 :glob:
 
 getting_started
 configuration
 cmakelists
+migration_guide
 changelog
 ```
 
 ```{toctree}
 :maxdepth: 1
 :titlesonly:
 :caption: API docs
@@ -33,7 +34,9 @@
 ```
 
 ## Indices and tables
 
 - {ref}`genindex`
 - {ref}`modindex`
 - {ref}`search`
+
+Generated using scikit-build-core {{ version }}.
```

### Comparing `scikit_build_core-0.4.5/docs/api/scikit_build_core.build.rst` & `scikit_build_core-0.4.6/docs/api/scikit_build_core.build.rst`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.5/docs/api/scikit_build_core.builder.rst` & `scikit_build_core-0.4.6/docs/api/scikit_build_core.builder.rst`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.5/docs/api/scikit_build_core.file_api.model.rst` & `scikit_build_core-0.4.6/docs/api/scikit_build_core.file_api.model.rst`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.5/docs/api/scikit_build_core.file_api.rst` & `scikit_build_core-0.4.6/docs/api/scikit_build_core.file_api.rst`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.5/docs/api/scikit_build_core.metadata.rst` & `scikit_build_core-0.4.6/docs/api/scikit_build_core.metadata.rst`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.5/docs/api/scikit_build_core.rst` & `scikit_build_core-0.4.6/docs/api/scikit_build_core.rst`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.5/docs/api/scikit_build_core.settings.rst` & `scikit_build_core-0.4.6/docs/api/scikit_build_core.settings.rst`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.5/docs/api/scikit_build_core.setuptools.rst` & `scikit_build_core-0.4.6/docs/api/scikit_build_core.setuptools.rst`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.5/docs/examples/downstream/nanobind_example/CMakeLists.txt` & `scikit_build_core-0.4.6/docs/examples/downstream/nanobind_example/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.5/docs/examples/downstream/nanobind_example/LICENSE` & `scikit_build_core-0.4.6/docs/examples/downstream/nanobind_example/LICENSE`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.5/docs/examples/downstream/nanobind_example/README.md` & `scikit_build_core-0.4.6/docs/examples/downstream/nanobind_example/README.md`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.5/docs/examples/downstream/nanobind_example/pyproject.toml` & `scikit_build_core-0.4.6/docs/examples/downstream/nanobind_example/pyproject.toml`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.5/docs/examples/downstream/pybind11_example/LICENSE` & `scikit_build_core-0.4.6/docs/examples/downstream/pybind11_example/LICENSE`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.5/docs/examples/downstream/pybind11_example/README.md` & `scikit_build_core-0.4.6/docs/examples/downstream/pybind11_example/README.md`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.5/docs/examples/downstream/pybind11_example/pyproject.toml` & `scikit_build_core-0.4.6/docs/examples/downstream/pybind11_example/pyproject.toml`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.5/docs/examples/downstream/pybind11_example/src/main.cpp` & `scikit_build_core-0.4.6/docs/examples/downstream/pybind11_example/src/main.cpp`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.5/docs/examples/getting_started/abi3/example.c` & `scikit_build_core-0.4.6/docs/examples/getting_started/abi3/example.c`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.5/docs/examples/getting_started/c/example.c` & `scikit_build_core-0.4.6/docs/examples/getting_started/c/example.c`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.5/docs/examples/getting_started/cython/CMakeLists.txt` & `scikit_build_core-0.4.6/docs/examples/getting_started/cython/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.5/docs/examples/getting_started/fortran/CMakeLists.txt` & `scikit_build_core-0.4.6/docs/examples/getting_started/fortran/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.5/docs/examples/getting_started/swig/CMakeLists.txt` & `scikit_build_core-0.4.6/docs/examples/getting_started/swig/CMakeLists.txt`

 * *Files 25% similar despite different names*

```diff
@@ -7,18 +7,22 @@
   REQUIRED)
 
 find_package(
   SWIG
   COMPONENTS python
   REQUIRED)
 
-add_custom_command(
-  OUTPUT example.py example_wrap.c
-  COMMAND ${SWIG_EXECUTABLE} -python -outcurrentdir
-          "${CMAKE_CURRENT_SOURCE_DIR}/example.i"
-  DEPENDS example.i)
+include(UseSWIG)
 
-python_add_library(_example MODULE example.c
-                   "${CMAKE_CURRENT_BINARY_DIR}/example_wrap.c" WITH_SOABI)
+swig_add_library(
+  example
+  LANGUAGE python OUTPUT_DIR "${SKBUILD_PLATLIB_DIR}"
+  SOURCES example.i example.c)
+if(WIN32)
+  set_property(TARGET example PROPERTY SUFFIX ".${Python_SOABI}.pyd")
+else()
+  set_property(TARGET example
+               PROPERTY SUFFIX ".${Python_SOABI}${CMAKE_SHARED_MODULE_SUFFIX}")
+endif()
+target_link_libraries(example PRIVATE Python::Module)
 
-install(TARGETS _example DESTINATION .)
-install(FILES "${CMAKE_CURRENT_BINARY_DIR}/example.py" DESTINATION .)
+install(TARGETS example DESTINATION .)
```

### Comparing `scikit_build_core-0.4.5/src/scikit_build_core/_logging.py` & `scikit_build_core-0.4.6/src/scikit_build_core/_logging.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.5/src/scikit_build_core/_shutil.py` & `scikit_build_core-0.4.6/src/scikit_build_core/_shutil.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 from __future__ import annotations
 
+import contextlib
 import dataclasses
 import os
+import stat
 import subprocess
-from collections.abc import Iterable
+import sys
+from collections.abc import Generator, Iterable
 from typing import ClassVar
 
 from ._logging import logger
 
 __all__ = ["Run"]
 
 
@@ -74,7 +77,30 @@
     def _key_diff(self, k: str) -> str:
         assert self.env
         if k in self.env and k not in self._prev_env:
             return "+"
         if k in self._prev_env and k not in self.env:
             return "-"
         return " "
+
+
+def _fix_all_permissions(directory: str) -> None:
+    """
+    Makes sure the write permission is set. Only run this on Windows.
+    """
+    with os.scandir(directory) as it:
+        for entry in it:
+            if entry.is_dir():
+                _fix_all_permissions(entry.path)
+                continue
+            mode = stat.S_IMODE(entry.stat().st_mode)
+            if not mode & stat.S_IWRITE:
+                os.chmod(entry.path, mode | stat.S_IWRITE)  # noqa: PTH101
+
+
+@contextlib.contextmanager
+def fix_win_37_all_permissions(tmpdir: str) -> Generator[None, None, None]:
+    try:
+        yield
+    finally:
+        if sys.version_info < (3, 8) and sys.platform.startswith("win"):
+            _fix_all_permissions(tmpdir)
```

### Comparing `scikit_build_core-0.4.5/src/scikit_build_core/cmake.py` & `scikit_build_core-0.4.6/src/scikit_build_core/cmake.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,18 +11,18 @@
 import textwrap
 from collections.abc import Mapping, Sequence
 from pathlib import Path
 from typing import Generator
 
 from packaging.version import Version
 
+from . import __version__
 from ._compat.typing import Self
 from ._logging import logger
 from ._shutil import Run
-from ._version import __version__
 from .errors import CMakeConfigError, CMakeNotFoundError, FailedLiveProcessError
 from .program_search import best_program, get_cmake_programs
 
 __all__ = ["CMake", "CMaker"]
 
 
 def __dir__() -> list[str]:
```

### Comparing `scikit_build_core-0.4.5/src/scikit_build_core/errors.py` & `scikit_build_core-0.4.6/src/scikit_build_core/errors.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.5/src/scikit_build_core/program_search.py` & `scikit_build_core-0.4.6/src/scikit_build_core/program_search.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.5/src/scikit_build_core/_compat/typing.py` & `scikit_build_core-0.4.6/src/scikit_build_core/_compat/typing.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.5/src/scikit_build_core/_compat/importlib/metadata.py` & `scikit_build_core-0.4.6/src/scikit_build_core/_compat/importlib/metadata.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.5/src/scikit_build_core/build/__init__.py` & `scikit_build_core-0.4.6/src/scikit_build_core/build/__init__.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.5/src/scikit_build_core/build/_file_processor.py` & `scikit_build_core-0.4.6/src/scikit_build_core/build/_file_processor.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.5/src/scikit_build_core/build/_init.py` & `scikit_build_core-0.4.6/src/scikit_build_core/build/_init.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.5/src/scikit_build_core/build/_pathutil.py` & `scikit_build_core-0.4.6/src/scikit_build_core/build/_pathutil.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.5/src/scikit_build_core/build/_scripts.py` & `scikit_build_core-0.4.6/src/scikit_build_core/build/_scripts.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.5/src/scikit_build_core/build/_wheelfile.py` & `scikit_build_core-0.4.6/src/scikit_build_core/build/_wheelfile.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,16 +17,16 @@
 from zipfile import ZipInfo
 
 import packaging.utils
 from packaging.tags import Tag
 from packaging.utils import BuildTag
 from pyproject_metadata import StandardMetadata
 
+from .. import __version__
 from .._compat.typing import Self
-from .._version import __version__
 
 EMAIL_POLICY = EmailPolicy(max_line_length=0, mangle_from_=False, utf8=True)
 
 MIN_TIMESTAMP = 315532800  # 1980-01-01 00:00:00 UTC
 
 
 def _b64encode(data: bytes) -> bytes:
```

### Comparing `scikit_build_core-0.4.5/src/scikit_build_core/build/sdist.py` & `scikit_build_core-0.4.6/src/scikit_build_core/build/sdist.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.5/src/scikit_build_core/build/wheel.py` & `scikit_build_core-0.4.6/src/scikit_build_core/build/wheel.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from pathlib import Path
 
 from packaging.version import Version
 
 from .. import __version__
 from .._compat import tomllib
 from .._logging import logger, rich_print
+from .._shutil import fix_win_37_all_permissions
 from ..builder.builder import Builder, archs_to_tags, get_archs
 from ..builder.wheel_tag import WheelTag
 from ..cmake import CMake, CMaker
 from ..resources import resources
 from ..settings.metadata import get_standard_metadata
 from ..settings.skbuild_read_settings import SettingsReader
 from ._init import setup_logging
@@ -86,27 +87,29 @@
 
     if metadata.version is None:
         msg = "project.version is not statically specified, must be present currently"
         raise AssertionError(msg)
 
     normalized_name = metadata.name.replace("-", "_").replace(".", "_")
 
+    action = "editable" if editable else "wheel"
+    if wheel_directory is None:
+        action = f"metadata_{action}"
+
     cmake = CMake.default_search(
         minimum_version=Version(settings.cmake.minimum_version)
     )
-    action = (
-        "metadata" if wheel_directory is None else "editable" if editable else "wheel"
-    )
+
     rich_print(
         f"[green]***[/green] [bold][green]scikit-build-core {__version__}[/green]",
         f"using [blue]CMake {cmake.version}[/blue]",
         f"[red]({action})[/red]",
     )
 
-    with tempfile.TemporaryDirectory() as tmpdir:
+    with tempfile.TemporaryDirectory() as tmpdir, fix_win_37_all_permissions(tmpdir):
         build_tmp_folder = Path(tmpdir)
         wheel_dir = build_tmp_folder / "wheel"
 
         tags = WheelTag.compute_best(
             archs_to_tags(get_archs(os.environ)),
             settings.wheel.py_api,
             expand_macos=settings.wheel.expand_macos_universal_tags,
@@ -191,14 +194,15 @@
                     path.parent.mkdir(exist_ok=True, parents=True)
                 path.write_bytes(data)
             return WheelImplReturn(wheel_filename=dist_info.name)
 
         rich_print("[green]***[/green] [bold]Configuring CMake...")
         defines: dict[str, str] = {}
         cache_entries = {f"SKBUILD_{k.upper()}_DIR": v for k, v in wheel_dirs.items()}
+        defines["SKBUILD_STATE"] = action
         builder.configure(
             defines=defines,
             cache_entries=cache_entries,
             name=metadata.name,
             version=metadata.version,
         )
```

### Comparing `scikit_build_core-0.4.5/src/scikit_build_core/builder/builder.py` & `scikit_build_core-0.4.6/src/scikit_build_core/builder/builder.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.5/src/scikit_build_core/builder/generator.py` & `scikit_build_core-0.4.6/src/scikit_build_core/builder/generator.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.5/src/scikit_build_core/builder/get_requires.py` & `scikit_build_core-0.4.6/src/scikit_build_core/builder/get_requires.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.5/src/scikit_build_core/builder/macos.py` & `scikit_build_core-0.4.6/src/scikit_build_core/builder/macos.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.5/src/scikit_build_core/builder/sysconfig.py` & `scikit_build_core-0.4.6/src/scikit_build_core/builder/sysconfig.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.5/src/scikit_build_core/builder/wheel_tag.py` & `scikit_build_core-0.4.6/src/scikit_build_core/builder/wheel_tag.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.5/src/scikit_build_core/file_api/_cattrs_converter.py` & `scikit_build_core-0.4.6/src/scikit_build_core/file_api/_cattrs_converter.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.5/src/scikit_build_core/file_api/query.py` & `scikit_build_core-0.4.6/src/scikit_build_core/file_api/query.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.5/src/scikit_build_core/file_api/reply.py` & `scikit_build_core-0.4.6/src/scikit_build_core/file_api/reply.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.5/src/scikit_build_core/file_api/model/codemodel.py` & `scikit_build_core-0.4.6/src/scikit_build_core/file_api/model/codemodel.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.5/src/scikit_build_core/file_api/model/directory.py` & `scikit_build_core-0.4.6/src/scikit_build_core/file_api/model/directory.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.5/src/scikit_build_core/file_api/model/index.py` & `scikit_build_core-0.4.6/src/scikit_build_core/file_api/model/index.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.5/src/scikit_build_core/file_api/model/toolchains.py` & `scikit_build_core-0.4.6/src/scikit_build_core/file_api/model/toolchains.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.5/src/scikit_build_core/metadata/fancy_pypi_readme.py` & `scikit_build_core-0.4.6/src/scikit_build_core/metadata/fancy_pypi_readme.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.5/src/scikit_build_core/metadata/setuptools_scm.py` & `scikit_build_core-0.4.6/src/scikit_build_core/metadata/setuptools_scm.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.5/src/scikit_build_core/resources/_editable_redirect.py` & `scikit_build_core-0.4.6/src/scikit_build_core/resources/_editable_redirect.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.5/src/scikit_build_core/resources/known_wheels.toml` & `scikit_build_core-0.4.6/src/scikit_build_core/resources/known_wheels.toml`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.5/src/scikit_build_core/resources/find_python/Copyright.txt` & `scikit_build_core-0.4.6/src/scikit_build_core/resources/find_python/Copyright.txt`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.5/src/scikit_build_core/resources/find_python/FindPackageHandleStandardArgs.cmake` & `scikit_build_core-0.4.6/src/scikit_build_core/resources/find_python/FindPackageHandleStandardArgs.cmake`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.5/src/scikit_build_core/resources/find_python/FindPackageMessage.cmake` & `scikit_build_core-0.4.6/src/scikit_build_core/resources/find_python/FindPackageMessage.cmake`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.5/src/scikit_build_core/resources/find_python/FindPython.cmake` & `scikit_build_core-0.4.6/src/scikit_build_core/resources/find_python/FindPython.cmake`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.5/src/scikit_build_core/resources/find_python/FindPython3.cmake` & `scikit_build_core-0.4.6/src/scikit_build_core/resources/find_python/FindPython3.cmake`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.5/src/scikit_build_core/resources/find_python/FindPython/Support.cmake` & `scikit_build_core-0.4.6/src/scikit_build_core/resources/find_python/FindPython/Support.cmake`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.5/src/scikit_build_core/settings/_load_provider.py` & `scikit_build_core-0.4.6/src/scikit_build_core/settings/_load_provider.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.5/src/scikit_build_core/settings/metadata.py` & `scikit_build_core-0.4.6/src/scikit_build_core/settings/metadata.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.5/src/scikit_build_core/settings/skbuild_model.py` & `scikit_build_core-0.4.6/src/scikit_build_core/settings/skbuild_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import dataclasses
 from typing import Any, Dict, List, Optional
 
 __all__ = [
-    "ScikitBuildSettings",
-    "NinjaSettings",
+    "BackportSettings",
     "CMakeSettings",
+    "EditableSettings",
     "LoggingSettings",
+    "NinjaSettings",
     "SDistSettings",
-    "BackportSettings",
+    "ScikitBuildSettings",
     "WheelSettings",
 ]
 
 
 def __dir__() -> List[str]:
     return __all__
 
@@ -108,15 +109,15 @@
 class BackportSettings:
     #: If CMake is less than this value, backport a copy of FindPython. Set
     #: to 0 disable this, or the empty string.
     find_python: str = "3.26.1"
 
 
 @dataclasses.dataclass
-class Editable:
+class EditableSettings:
     #: Select the editable mode to use. Currently only "redirect" is supported.
     mode: str = "redirect"
 
     #: Turn on verbose output for the editable mode rebuilds.
     verbose: bool = True
 
     #: Rebuild the project when the package is imported.
@@ -129,15 +130,15 @@
     cmake: CMakeSettings = dataclasses.field(default_factory=CMakeSettings)
     ninja: NinjaSettings = dataclasses.field(default_factory=NinjaSettings)
     logging: LoggingSettings = dataclasses.field(default_factory=LoggingSettings)
     sdist: SDistSettings = dataclasses.field(default_factory=SDistSettings)
     wheel: WheelSettings = dataclasses.field(default_factory=WheelSettings)
     backport: BackportSettings = dataclasses.field(default_factory=BackportSettings)
     metadata: Dict[str, Dict[str, Any]] = dataclasses.field(default_factory=dict)
-    editable: Editable = dataclasses.field(default_factory=Editable)
+    editable: EditableSettings = dataclasses.field(default_factory=EditableSettings)
 
     #: Strictly check all config options. If False, warnings will be
     #: printed for unknown options. If True, an error will be raised.
     strict_config: bool = True
 
     #: Enable early previews of features not finalized yet.
     experimental: bool = False
```

### Comparing `scikit_build_core-0.4.5/src/scikit_build_core/settings/skbuild_read_settings.py` & `scikit_build_core-0.4.6/src/scikit_build_core/settings/skbuild_read_settings.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.5/src/scikit_build_core/settings/sources.py` & `scikit_build_core-0.4.6/src/scikit_build_core/settings/sources.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.5/src/scikit_build_core/setuptools/build_cmake.py` & `scikit_build_core-0.4.6/src/scikit_build_core/setuptools/build_cmake.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.5/src/scikit_build_core/setuptools/build_meta.py` & `scikit_build_core-0.4.6/src/scikit_build_core/setuptools/build_meta.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.5/src/scikit_build_core/setuptools/wrapper.py` & `scikit_build_core-0.4.6/src/scikit_build_core/setuptools/wrapper.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.5/tests/conftest.py` & `scikit_build_core-0.4.6/tests/conftest.py`

 * *Files 2% similar despite different names*

```diff
@@ -293,14 +293,15 @@
     for item in items:
         # Ensure all tests using virtualenv are marked as such
         if "virtualenv" in getattr(item, "fixturenames", ()):
             item.add_marker(pytest.mark.virtualenv)
         if "isolated" in getattr(item, "fixturenames", ()):
             item.add_marker(pytest.mark.virtualenv)
             item.add_marker(pytest.mark.isolated)
+            item.add_marker(pytest.mark.network)
 
 
 def pytest_report_header() -> str:
     interesting_packages = [
         "build",
         "packaging",
         "pathspec",
```

### Comparing `scikit_build_core-0.4.5/tests/test_builder.py` & `scikit_build_core-0.4.6/tests/test_builder.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.5/tests/test_cmake_config.py` & `scikit_build_core-0.4.6/tests/test_cmake_config.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.5/tests/test_custom_modules.py` & `scikit_build_core-0.4.6/tests/test_custom_modules.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.5/tests/test_dynamic_metadata.py` & `scikit_build_core-0.4.6/tests/test_dynamic_metadata.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.5/tests/test_file_processor.py` & `scikit_build_core-0.4.6/tests/test_file_processor.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.5/tests/test_fileapi.py` & `scikit_build_core-0.4.6/tests/test_fileapi.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.5/tests/test_fortran.py` & `scikit_build_core-0.4.6/tests/test_fortran.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 cmake_info = best_program(get_cmake_programs(), minimum_version=Version("3.17.2"))
 ninja_info = best_program(get_ninja_programs(), minimum_version=Version("1.10"))
 
 
 @pytest.mark.compile()
 @pytest.mark.configure()
 @pytest.mark.fortran()
+@pytest.mark.network()
 @pytest.mark.skipif(shutil.which("gfortran") is None, reason="gfortran not available")
 @pytest.mark.skipif(
     sysconfig.get_platform().startswith("win"),
     reason="No reasonable Fortran compiler for MSVC",
 )
 @pytest.mark.skipif(
     cmake_info is None, reason="CMake needs to be 3.17.2+ to support Fortran with Ninja"
```

### Comparing `scikit_build_core-0.4.5/tests/test_generator_default.py` & `scikit_build_core-0.4.6/tests/test_generator_default.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.5/tests/test_get_requires.py` & `scikit_build_core-0.4.6/tests/test_get_requires.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.5/tests/test_module_dir.py` & `scikit_build_core-0.4.6/tests/test_module_dir.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.5/tests/test_name_main.py` & `scikit_build_core-0.4.6/tests/test_name_main.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.5/tests/test_prepare_metadata.py` & `scikit_build_core-0.4.6/tests/test_prepare_metadata.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.5/tests/test_process_scripts.py` & `scikit_build_core-0.4.6/tests/test_process_scripts.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.5/tests/test_program_search.py` & `scikit_build_core-0.4.6/tests/test_program_search.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.5/tests/test_pyproject_abi3.py` & `scikit_build_core-0.4.6/tests/test_pyproject_abi3.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.5/tests/test_pyproject_extra_dirs.py` & `scikit_build_core-0.4.6/tests/test_pyproject_extra_dirs.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.5/tests/test_pyproject_pep517.py` & `scikit_build_core-0.4.6/tests/test_pyproject_pep517.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.5/tests/test_pyproject_pep518.py` & `scikit_build_core-0.4.6/tests/test_pyproject_pep518.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import textwrap
 import zipfile
 from pathlib import Path
 
 import pytest
 
 
-@pytest.mark.isolated()
+@pytest.mark.network()
 @pytest.mark.integration()
 def test_pep518_sdist(package_simple_pyproject_ext):
     correct_metadata = textwrap.dedent(
         """\
         Metadata-Version: 2.1
         Name: cmake-example
         Version: 0.0.1
```

### Comparing `scikit_build_core-0.4.5/tests/test_pyproject_pep660.py` & `scikit_build_core-0.4.6/tests/test_pyproject_pep660.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.5/tests/test_settings.py` & `scikit_build_core-0.4.6/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.5/tests/test_setuptools_abi3.py` & `scikit_build_core-0.4.6/tests/test_setuptools_abi3.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.5/tests/test_setuptools_pep517.py` & `scikit_build_core-0.4.6/tests/test_setuptools_pep517.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.5/tests/test_setuptools_pep518.py` & `scikit_build_core-0.4.6/tests/test_setuptools_pep518.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.5/tests/test_simple_pure.py` & `scikit_build_core-0.4.6/tests/test_simple_pure.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.5/tests/test_simplest_c.py` & `scikit_build_core-0.4.6/tests/test_simplest_c.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.5/tests/test_skbuild_settings.py` & `scikit_build_core-0.4.6/tests/test_skbuild_settings.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.5/tests/test_wheelfile_utils.py` & `scikit_build_core-0.4.6/tests/test_wheelfile_utils.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.5/tests/api/simple_pure/.cmake/api/v1/reply/cache-v2-2dececcab32f1eda138d.json` & `scikit_build_core-0.4.6/tests/api/simple_pure/.cmake/api/v1/reply/cache-v2-2dececcab32f1eda138d.json`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.5/tests/api/simple_pure/.cmake/api/v1/reply/cmakeFiles-v1-74870fd87af7f965b597.json` & `scikit_build_core-0.4.6/tests/api/simple_pure/.cmake/api/v1/reply/cmakeFiles-v1-74870fd87af7f965b597.json`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.5/tests/api/simple_pure/.cmake/api/v1/reply/codemodel-v2-ea39b5a28cb1a3e0a069.json` & `scikit_build_core-0.4.6/tests/api/simple_pure/.cmake/api/v1/reply/codemodel-v2-ea39b5a28cb1a3e0a069.json`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.5/tests/api/simple_pure/.cmake/api/v1/reply/directory-.-5e7a28751b0c9235cbe7.json` & `scikit_build_core-0.4.6/tests/api/simple_pure/.cmake/api/v1/reply/directory-.-5e7a28751b0c9235cbe7.json`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.5/tests/api/simple_pure/.cmake/api/v1/reply/index-2022-09-12T15-23-13-0135.json` & `scikit_build_core-0.4.6/tests/api/simple_pure/.cmake/api/v1/reply/index-2022-09-12T15-23-13-0135.json`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.5/tests/api/simple_pure/.cmake/api/v1/reply/target-simple_pure-7eb73eb5c359b881e083.json` & `scikit_build_core-0.4.6/tests/api/simple_pure/.cmake/api/v1/reply/target-simple_pure-7eb73eb5c359b881e083.json`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.5/tests/api/simple_pure/.cmake/api/v1/reply/toolchains-v1-06b92b86597808b5f980.json` & `scikit_build_core-0.4.6/tests/api/simple_pure/.cmake/api/v1/reply/toolchains-v1-06b92b86597808b5f980.json`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.5/tests/packages/abi3_pyproject_ext/abi3_example.c` & `scikit_build_core-0.4.6/tests/packages/abi3_pyproject_ext/abi3_example.c`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.5/tests/packages/abi3_setuptools_ext/abi3_example.c` & `scikit_build_core-0.4.6/tests/packages/abi3_setuptools_ext/abi3_example.c`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.5/tests/packages/dynamic_metadata/plugin_project.toml` & `scikit_build_core-0.4.6/tests/packages/dynamic_metadata/plugin_project.toml`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.5/tests/packages/dynamic_metadata/src/module.c` & `scikit_build_core-0.4.6/tests/packages/dynamic_metadata/src/module.c`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.5/tests/packages/filepath_pure/CMakeLists.txt` & `scikit_build_core-0.4.6/tests/packages/filepath_pure/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.5/tests/packages/fortran_example/CMakeLists.txt` & `scikit_build_core-0.4.6/tests/packages/fortran_example/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.5/tests/packages/mixed_setuptools/CMakeLists.txt` & `scikit_build_core-0.4.6/tests/packages/mixed_setuptools/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.5/tests/packages/simple_pyproject_ext/LICENSE` & `scikit_build_core-0.4.6/tests/packages/simple_pyproject_ext/LICENSE`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.5/tests/packages/simple_pyproject_ext/src/main.cpp` & `scikit_build_core-0.4.6/tests/packages/simple_pyproject_ext/src/main.cpp`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.5/tests/packages/simple_pyproject_source_dir/LICENSE` & `scikit_build_core-0.4.6/tests/packages/simple_pyproject_source_dir/LICENSE`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.5/tests/packages/simple_pyproject_source_dir/src/main.cpp` & `scikit_build_core-0.4.6/tests/packages/simple_pyproject_source_dir/src/main.cpp`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.5/tests/packages/simple_setuptools_ext/LICENSE` & `scikit_build_core-0.4.6/tests/packages/simple_setuptools_ext/LICENSE`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.5/tests/packages/simple_setuptools_ext/src/main.cpp` & `scikit_build_core-0.4.6/tests/packages/simple_setuptools_ext/src/main.cpp`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.5/tests/packages/simplest_c/CMakeLists.txt` & `scikit_build_core-0.4.6/tests/packages/simplest_c/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.5/tests/packages/simplest_c/src/module.c` & `scikit_build_core-0.4.6/tests/packages/simplest_c/src/module.c`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.5/.gitignore` & `scikit_build_core-0.4.6/.gitignore`

 * *Files 13% similar despite different names*

```diff
@@ -149,16 +149,16 @@
 /src/scikit_build_core/_version.py
 
 # Common editor files
 *~
 *.swp
 
 # RPM spec file
-!/.distro/*.spec
-/.distro/*.tar.gz
+!/distro/*.spec
+/distro/*.tar.gz
 *.rpm
 
 # ruff
 .ruff_cache/
 
 # OS specific stuff
 .DS_Store
@@ -167,12 +167,12 @@
 .Spotlight-V100
 .Trashes
 ehthumbs.db
 Thumbs.db
 
 .idea/
 # tmt setup
-/.distro/main.fmf
-/.distro/plans/main.fmf
-/.distro/tests/main.fmf
+/distro/main.fmf
+/distro/plans/main.fmf
+/distro/tests/main.fmf
 
 /docs/**/build
```

### Comparing `scikit_build_core-0.4.5/LICENSE` & `scikit_build_core-0.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.5/README.md` & `scikit_build_core-0.4.6/README.md`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.5/pyproject.toml` & `scikit_build_core-0.4.6/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -30,57 +30,69 @@
     "Typing :: Typed",
 ]
 
 dynamic = ["version"]
 
 dependencies = [
     "exceptiongroup; python_version<'3.11'",
-    "importlib_resources >=1.3; python_version<'3.9'",
-    "importlib_metadata; python_version<'3.8'",
+    "importlib-resources >=1.3; python_version<'3.9'",
+    "importlib-metadata; python_version<'3.8'",
     "packaging >=20.9",
     "tomli >=1.1; python_version<'3.11'",
-    "typing_extensions >=3.10.0; python_version<'3.8'",
+    "typing-extensions >=3.10.0; python_version<'3.8'",
 ]
 # Note: for building wheels and sdists, there are also additional dependencies
 # in the pyproject extra. And cmake and possibly ninja if those are not already
 # present (user controllable)
 
 [project.optional-dependencies]
 pyproject = [
     "pyproject-metadata >=0.5",
     "pathspec >=0.10.1",
 ]
 test = [
     "build[virtualenv]",
     "cattrs >=22.2.0",
-    "importlib_metadata; python_version<'3.8'",
+    "importlib-metadata; python_version<'3.8'",
     "pathspec >=0.10.1",
     "pybind11",
     "pyproject-metadata >=0.5",
     "pytest >=7.0",  # 7.2+ recommended for better tracebacks with ExceptionGroup
     "pytest-subprocess >=1.5",
     "setuptools",
     "wheel",
 ]
+test-meta = [
+    "hatch-fancy-pypi-readme",
+    "setuptools-scm",
+]
+test-numpy = [
+    "numpy; python_version<'3.12' and platform_python_implementation!='PyPy'",
+    "numpy~=1.21.0; python_version=='3.7' and platform_python_implementation=='PyPy' and sys_platform == 'linux'",
+    "numpy~=1.24.0; python_version=='3.8' and platform_python_implementation=='PyPy'",
+    "numpy~=1.25.0; python_version=='3.9' and platform_python_implementation=='PyPy'",
+]
 cov = [
     "pytest-cov[toml]",
 ]
+wheels = [
+    "cmake",
+    "ninja; sys_platform!='win32'",
+]
 dev = [
-    "build",
-    "cattrs >=22.2.0",
-    "pytest >=7.0",
-    "pytest-subprocess",
     "rich",
 ]
 docs = [
     "furo",
-    "myst_parser >=0.13",
+    "myst-parser >=0.13",
+    "pathspec >=0.10.1",
+    "pyproject-metadata >=0.5",
     "sphinx >=4.0",
-    "sphinx_copybutton",
-    "sphinx_inline_tabs",
+    "sphinx-copybutton",
+    "sphinx-inline-tabs",
 ]
 
 [project.urls]
 Homepage = "https://github.com/scikit-build/scikit-build-core"
 Documentation = "https://scikit-build-core.readthedocs.io"
 Discussions = "https://github.com/orgs/scikit-build/discussions"
 Issues = "https://github.com/scikit-build/scikit-build-core/issues"
@@ -113,14 +125,15 @@
 markers = [
     "broken_on_urct: Broken for now due to lib not found",
     "compile: Compiles code",
     "configure: Configures CMake code",
     "fortran: Fortran code",
     "integration: Full package build",
     "isolated: Needs an isolated virtualenv",
+    "network: Needs a network connection to setup or run",
     "setuptools: Tests setuptools integration",
     "virtualenv: Needs a virtualenv",
 ]
 
 
 [tool.mypy]
 files = ["src", "tests"]
@@ -177,15 +190,15 @@
 [tool.check-wheel-contents]
 ignore = ["W002"]  # Triggers on __init__.py's
 
 
 [tool.ruff]
 select = [
     "E", "F", "W", # flake8
-    "B",  "B904",  # flake8-bugbear
+    "B",           # flake8-bugbear
     "I",           # isort
     "ARG",         # flake8-unused-arguments
     "C4",          # flake8-comprehensions
     "EM",          # flake8-errmsg
     "ICN",         # flake8-import-conventions
     "ISC",         # flake8-implicit-str-concat
     "PGH",         # pygrep-hooks
@@ -240,11 +253,12 @@
 
 [tool.ruff.per-file-ignores]
 "tests/**" = ["T20"]
 "noxfile.py" = ["T20", "TID251"]
 "src/scikit_build_core/resources/*.py" = ["PTH", "ARG002"]
 "src/scikit_build_core/_compat/**.py" = ["TID251"]
 "tests/conftest.py" = ["TID251"]
+"docs/conf.py" = ["TID251"]
 
 
 [tool.check-sdist]
 sdist-only = ["src/scikit_build_core/_version.py"]
```

### Comparing `scikit_build_core-0.4.5/PKG-INFO` & `scikit_build_core-0.4.6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scikit_build_core
-Version: 0.4.5
+Version: 0.4.6
 Summary: Build backend for CMake based projects
 Project-URL: Homepage, https://github.com/scikit-build/scikit-build-core
 Project-URL: Documentation, https://scikit-build-core.readthedocs.io
 Project-URL: Discussions, https://github.com/orgs/scikit-build/discussions
 Project-URL: Issues, https://github.com/scikit-build/scikit-build-core/issues
 Project-URL: Changelog, https://scikit-build-core.readthedocs.io/en/latest/changelog.html
 Author-email: Henry Schreiner <henryfs@princeton.edu>
@@ -32,22 +32,20 @@
 Requires-Dist: importlib-resources>=1.3; python_version < '3.9'
 Requires-Dist: packaging>=20.9
 Requires-Dist: tomli>=1.1; python_version < '3.11'
 Requires-Dist: typing-extensions>=3.10.0; python_version < '3.8'
 Provides-Extra: cov
 Requires-Dist: pytest-cov[toml]; extra == 'cov'
 Provides-Extra: dev
-Requires-Dist: build; extra == 'dev'
-Requires-Dist: cattrs>=22.2.0; extra == 'dev'
-Requires-Dist: pytest-subprocess; extra == 'dev'
-Requires-Dist: pytest>=7.0; extra == 'dev'
 Requires-Dist: rich; extra == 'dev'
 Provides-Extra: docs
 Requires-Dist: furo; extra == 'docs'
 Requires-Dist: myst-parser>=0.13; extra == 'docs'
+Requires-Dist: pathspec>=0.10.1; extra == 'docs'
+Requires-Dist: pyproject-metadata>=0.5; extra == 'docs'
 Requires-Dist: sphinx-copybutton; extra == 'docs'
 Requires-Dist: sphinx-inline-tabs; extra == 'docs'
 Requires-Dist: sphinx>=4.0; extra == 'docs'
 Provides-Extra: pyproject
 Requires-Dist: pathspec>=0.10.1; extra == 'pyproject'
 Requires-Dist: pyproject-metadata>=0.5; extra == 'pyproject'
 Provides-Extra: test
@@ -57,14 +55,25 @@
 Requires-Dist: pathspec>=0.10.1; extra == 'test'
 Requires-Dist: pybind11; extra == 'test'
 Requires-Dist: pyproject-metadata>=0.5; extra == 'test'
 Requires-Dist: pytest-subprocess>=1.5; extra == 'test'
 Requires-Dist: pytest>=7.0; extra == 'test'
 Requires-Dist: setuptools; extra == 'test'
 Requires-Dist: wheel; extra == 'test'
+Provides-Extra: test-meta
+Requires-Dist: hatch-fancy-pypi-readme; extra == 'test-meta'
+Requires-Dist: setuptools-scm; extra == 'test-meta'
+Provides-Extra: test-numpy
+Requires-Dist: numpy; python_version < '3.12' and platform_python_implementation != 'PyPy' and extra == 'test-numpy'
+Requires-Dist: numpy~=1.21.0; python_version == '3.7' and platform_python_implementation == 'PyPy' and sys_platform == 'linux' and extra == 'test-numpy'
+Requires-Dist: numpy~=1.24.0; python_version == '3.8' and platform_python_implementation == 'PyPy' and extra == 'test-numpy'
+Requires-Dist: numpy~=1.25.0; python_version == '3.9' and platform_python_implementation == 'PyPy' and extra == 'test-numpy'
+Provides-Extra: wheels
+Requires-Dist: cmake; extra == 'wheels'
+Requires-Dist: ninja; sys_platform != 'win32' and extra == 'wheels'
 Description-Content-Type: text/markdown
 
 # scikit-build-core
 
 [![Documentation Status][rtd-badge]][rtd-link]
 [![GitHub Discussion][github-discussions-badge]][github-discussions-link]
```

