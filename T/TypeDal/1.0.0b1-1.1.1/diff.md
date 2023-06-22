# Comparing `tmp/typedal-1.0.0b1.tar.gz` & `tmp/typedal-1.1.1.tar.gz`

## Comparing `typedal-1.0.0b1.tar` & `typedal-1.1.1.tar`

### file list

```diff
@@ -1,340 +1,349 @@
--rw-r--r--   0        0        0     2079 2020-02-02 00:00:00.000000 typedal-1.0.0b1/CHANGELOG.md
--rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 typedal-1.0.0b1/coverage.svg
--rw-r--r--   0        0        0     7896 2020-02-02 00:00:00.000000 typedal-1.0.0b1/example_new.py
--rw-r--r--   0        0        0     2872 2020-02-02 00:00:00.000000 typedal-1.0.0b1/example_old.py
--rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.github/workflows/su6.yml
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/.gitignore
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/@plugins_snapshot.json
--rw-r--r--   0        0        0   177667 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/_ast.data.json
--rw-r--r--   0        0        0     1567 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/_ast.meta.json
--rw-r--r--   0        0        0    52400 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/_codecs.data.json
--rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/_codecs.meta.json
--rw-r--r--   0        0        0    18227 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/_collections_abc.data.json
--rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/_collections_abc.meta.json
--rw-r--r--   0        0        0     2923 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/_ctypes.data.json
--rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/_ctypes.meta.json
--rw-r--r--   0        0        0   170960 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/_decimal.data.json
--rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/_decimal.meta.json
--rw-r--r--   0        0        0    23362 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/abc.data.json
--rw-r--r--   0        0        0     1574 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/abc.meta.json
--rw-r--r--   0        0        0    60687 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/array.data.json
--rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/array.meta.json
--rw-r--r--   0        0        0  1054992 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/builtins.data.json
--rw-r--r--   0        0        0     1721 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/builtins.meta.json
--rw-r--r--   0        0        0   123328 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/codecs.data.json
--rw-r--r--   0        0        0     1671 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/codecs.meta.json
--rw-r--r--   0        0        0   104160 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/contextlib.data.json
--rw-r--r--   0        0        0     1610 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/contextlib.meta.json
--rw-r--r--   0        0        0    57612 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/dataclasses.data.json
--rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/dataclasses.meta.json
--rw-r--r--   0        0        0   142044 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/datetime.data.json
--rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/datetime.meta.json
--rw-r--r--   0        0        0     4911 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/decimal.data.json
--rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/decimal.meta.json
--rw-r--r--   0        0        0    61020 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/enum.data.json
--rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/enum.meta.json
--rw-r--r--   0        0        0    22399 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/genericpath.data.json
--rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/genericpath.meta.json
--rw-r--r--   0        0        0    85348 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/io.data.json
--rw-r--r--   0        0        0     1673 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/io.meta.json
--rw-r--r--   0        0        0    28778 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/mmap.data.json
--rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/mmap.meta.json
--rw-r--r--   0        0        0    78982 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/numbers.data.json
--rw-r--r--   0        0        0     1519 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/numbers.meta.json
--rw-r--r--   0        0        0    88278 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/pathlib.data.json
--rw-r--r--   0        0        0     1682 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/pathlib.meta.json
--rw-r--r--   0        0        0    45131 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/pickle.data.json
--rw-r--r--   0        0        0     1630 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/pickle.meta.json
--rw-r--r--   0        0        0    75208 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/posixpath.data.json
--rw-r--r--   0        0        0     1627 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/posixpath.meta.json
--rw-r--r--   0        0        0   167175 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/re.data.json
--rw-r--r--   0        0        0     1701 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/re.meta.json
--rw-r--r--   0        0        0    14131 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/sre_compile.data.json
--rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/sre_compile.meta.json
--rw-r--r--   0        0        0    28013 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/sre_constants.data.json
--rw-r--r--   0        0        0     1584 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/sre_constants.meta.json
--rw-r--r--   0        0        0    49442 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/sre_parse.data.json
--rw-r--r--   0        0        0     1627 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/sre_parse.meta.json
--rw-r--r--   0        0        0   168498 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/subprocess.data.json
--rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/subprocess.meta.json
--rw-r--r--   0        0        0   146267 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/sys.data.json
--rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/sys.meta.json
--rw-r--r--   0        0        0    43605 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/time.data.json
--rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/time.meta.json
--rw-r--r--   0        0        0   228230 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/types.data.json
--rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/types.meta.json
--rw-r--r--   0        0        0   416965 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/typing.data.json
--rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/typing.meta.json
--rw-r--r--   0        0        0    73907 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/typing_extensions.data.json
--rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/typing_extensions.meta.json
--rw-r--r--   0        0        0    89065 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/_typeshed/__init__.data.json
--rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/_typeshed/__init__.meta.json
--rw-r--r--   0        0        0   407999 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/collections/__init__.data.json
--rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/collections/__init__.meta.json
--rw-r--r--   0        0        0     3731 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/collections/abc.data.json
--rw-r--r--   0        0        0     1558 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/collections/abc.meta.json
--rw-r--r--   0        0        0   128994 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/ctypes/__init__.data.json
--rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/ctypes/__init__.meta.json
--rw-r--r--   0        0        0     7438 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/email/__init__.data.json
--rw-r--r--   0        0        0     1610 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/email/__init__.meta.json
--rw-r--r--   0        0        0    12200 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/email/charset.data.json
--rw-r--r--   0        0        0     1555 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/email/charset.meta.json
--rw-r--r--   0        0        0     7249 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/email/contentmanager.data.json
--rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/email/contentmanager.meta.json
--rw-r--r--   0        0        0    25073 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/email/errors.data.json
--rw-r--r--   0        0        0     1559 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/email/errors.meta.json
--rw-r--r--   0        0        0     9154 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/email/header.data.json
--rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/email/header.meta.json
--rw-r--r--   0        0        0    79298 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/email/message.data.json
--rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/email/message.meta.json
--rw-r--r--   0        0        0    30857 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/email/policy.data.json
--rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/email/policy.meta.json
--rw-r--r--   0        0        0     6125 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/importlib/__init__.data.json
--rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/importlib/__init__.meta.json
--rw-r--r--   0        0        0    70175 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/importlib/abc.data.json
--rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/importlib/abc.meta.json
--rw-r--r--   0        0        0    64626 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/importlib/machinery.data.json
--rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/importlib/machinery.meta.json
--rw-r--r--   0        0        0    90277 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/importlib/metadata/__init__.data.json
--rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/importlib/metadata/__init__.meta.json
--rw-r--r--   0        0        0    11935 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/importlib/metadata/_meta.data.json
--rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/importlib/metadata/_meta.meta.json
--rw-r--r--   0        0        0   350178 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/os/__init__.data.json
--rw-r--r--   0        0        0     1725 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/os/__init__.meta.json
--rw-r--r--   0        0        0     4908 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/os/path.data.json
--rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/os/path.meta.json
--rw-r--r--   0        0        0     1385 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/src/__init__.data.json
--rw-r--r--   0        0        0     1433 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/src/__init__.meta.json
--rw-r--r--   0        0        0     1506 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/src/typedal/__about__.data.json
--rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/src/typedal/__about__.meta.json
--rw-r--r--   0        0        0     2114 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/src/typedal/__init__.data.json
--rw-r--r--   0        0        0     1499 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/src/typedal/__init__.meta.json
--rw-r--r--   0        0        0    33347 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/src/typedal/core.data.json
--rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/src/typedal/core.meta.json
--rw-r--r--   0        0        0    29038 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/src/typedal/fields.data.json
--rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/src/typedal/fields.meta.json
--rw-r--r--   0        0        0     2775 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/src/typedal/pydal_objects.data.json
--rw-r--r--   0        0        0     1503 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.10/src/typedal/pydal_objects.meta.json
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/@plugins_snapshot.json
--rw-r--r--   0        0        0   180368 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/_ast.data.json
--rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/_ast.meta.json
--rw-r--r--   0        0        0    52400 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/_codecs.data.json
--rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/_codecs.meta.json
--rw-r--r--   0        0        0    18227 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/_collections_abc.data.json
--rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/_collections_abc.meta.json
--rw-r--r--   0        0        0     3125 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/_ctypes.data.json
--rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/_ctypes.meta.json
--rw-r--r--   0        0        0   171931 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/_decimal.data.json
--rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/_decimal.meta.json
--rw-r--r--   0        0        0    23336 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/abc.data.json
--rw-r--r--   0        0        0     1574 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/abc.meta.json
--rw-r--r--   0        0        0    60676 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/array.data.json
--rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/array.meta.json
--rw-r--r--   0        0        0  1130454 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/builtins.data.json
--rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/builtins.meta.json
--rw-r--r--   0        0        0   123317 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/codecs.data.json
--rw-r--r--   0        0        0     1671 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/codecs.meta.json
--rw-r--r--   0        0        0   109204 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/contextlib.data.json
--rw-r--r--   0        0        0     1610 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/contextlib.meta.json
--rw-r--r--   0        0        0    57745 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/dataclasses.data.json
--rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/dataclasses.meta.json
--rw-r--r--   0        0        0   142208 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/datetime.data.json
--rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/datetime.meta.json
--rw-r--r--   0        0        0     4911 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/decimal.data.json
--rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/decimal.meta.json
--rw-r--r--   0        0        0    90123 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/enum.data.json
--rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/enum.meta.json
--rw-r--r--   0        0        0    22388 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/genericpath.data.json
--rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/genericpath.meta.json
--rw-r--r--   0        0        0    85337 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/io.data.json
--rw-r--r--   0        0        0     1673 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/io.meta.json
--rw-r--r--   0        0        0    28767 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/mmap.data.json
--rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/mmap.meta.json
--rw-r--r--   0        0        0    78982 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/numbers.data.json
--rw-r--r--   0        0        0     1519 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/numbers.meta.json
--rw-r--r--   0        0        0    87488 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/pathlib.data.json
--rw-r--r--   0        0        0     1682 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/pathlib.meta.json
--rw-r--r--   0        0        0    45131 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/pickle.data.json
--rw-r--r--   0        0        0     1630 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/pickle.meta.json
--rw-r--r--   0        0        0    75197 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/posixpath.data.json
--rw-r--r--   0        0        0     1627 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/posixpath.meta.json
--rw-r--r--   0        0        0   167545 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/re.data.json
--rw-r--r--   0        0        0     1701 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/re.meta.json
--rw-r--r--   0        0        0    14373 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/sre_compile.data.json
--rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/sre_compile.meta.json
--rw-r--r--   0        0        0    28480 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/sre_constants.data.json
--rw-r--r--   0        0        0     1584 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/sre_constants.meta.json
--rw-r--r--   0        0        0    49741 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/sre_parse.data.json
--rw-r--r--   0        0        0     1627 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/sre_parse.meta.json
--rw-r--r--   0        0        0   172768 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/subprocess.data.json
--rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/subprocess.meta.json
--rw-r--r--   0        0        0   148675 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/sys.data.json
--rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/sys.meta.json
--rw-r--r--   0        0        0    43605 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/time.data.json
--rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/time.meta.json
--rw-r--r--   0        0        0   239632 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/types.data.json
--rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/types.meta.json
--rw-r--r--   0        0        0   432234 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/typing.data.json
--rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/typing.meta.json
--rw-r--r--   0        0        0    57845 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/typing_extensions.data.json
--rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/typing_extensions.meta.json
--rw-r--r--   0        0        0    89054 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/_typeshed/__init__.data.json
--rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/_typeshed/__init__.meta.json
--rw-r--r--   0        0        0   407988 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/collections/__init__.data.json
--rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/collections/__init__.meta.json
--rw-r--r--   0        0        0     3731 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/collections/abc.data.json
--rw-r--r--   0        0        0     1558 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/collections/abc.meta.json
--rw-r--r--   0        0        0   128983 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/ctypes/__init__.data.json
--rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/ctypes/__init__.meta.json
--rw-r--r--   0        0        0     7438 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/email/__init__.data.json
--rw-r--r--   0        0        0     1610 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/email/__init__.meta.json
--rw-r--r--   0        0        0    12200 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/email/charset.data.json
--rw-r--r--   0        0        0     1555 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/email/charset.meta.json
--rw-r--r--   0        0        0     7249 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/email/contentmanager.data.json
--rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/email/contentmanager.meta.json
--rw-r--r--   0        0        0    25073 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/email/errors.data.json
--rw-r--r--   0        0        0     1559 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/email/errors.meta.json
--rw-r--r--   0        0        0     9154 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/email/header.data.json
--rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/email/header.meta.json
--rw-r--r--   0        0        0    79287 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/email/message.data.json
--rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/email/message.meta.json
--rw-r--r--   0        0        0    30857 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/email/policy.data.json
--rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/email/policy.meta.json
--rw-r--r--   0        0        0     6125 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/importlib/__init__.data.json
--rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/importlib/__init__.meta.json
--rw-r--r--   0        0        0    70579 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/importlib/abc.data.json
--rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/importlib/abc.meta.json
--rw-r--r--   0        0        0    64626 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/importlib/machinery.data.json
--rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/importlib/machinery.meta.json
--rw-r--r--   0        0        0    91119 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/importlib/metadata/__init__.data.json
--rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/importlib/metadata/__init__.meta.json
--rw-r--r--   0        0        0    11935 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/importlib/metadata/_meta.data.json
--rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/importlib/metadata/_meta.meta.json
--rw-r--r--   0        0        0   350743 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/os/__init__.data.json
--rw-r--r--   0        0        0     1725 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/os/__init__.meta.json
--rw-r--r--   0        0        0     4908 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/os/path.data.json
--rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/os/path.meta.json
--rw-r--r--   0        0        0     1385 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/src/__init__.data.json
--rw-r--r--   0        0        0     1433 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/src/__init__.meta.json
--rw-r--r--   0        0        0     1506 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/src/typedal/__about__.data.json
--rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/src/typedal/__about__.meta.json
--rw-r--r--   0        0        0     2114 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/src/typedal/__init__.data.json
--rw-r--r--   0        0        0     1499 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/src/typedal/__init__.meta.json
--rw-r--r--   0        0        0    33350 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/src/typedal/core.data.json
--rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/src/typedal/core.meta.json
--rw-r--r--   0        0        0    29038 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/src/typedal/fields.data.json
--rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/src/typedal/fields.meta.json
--rw-r--r--   0        0        0     1478 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/typedal/__about__.data.json
--rw-r--r--   0        0        0     1458 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/typedal/__about__.meta.json
--rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/typedal/__init__.data.json
--rw-r--r--   0        0        0     1487 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/typedal/__init__.meta.json
--rw-r--r--   0        0        0    33137 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/typedal/core.data.json
--rw-r--r--   0        0        0     1662 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/typedal/core.meta.json
--rw-r--r--   0        0        0    30390 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/typedal/fields.data.json
--rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.mypy_cache/3.11/typedal/fields.meta.json
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.pytest_cache/README.md
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.pytest_cache/v/cache/lastfailed
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.ruff_cache/.gitignore
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.ruff_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.ruff_cache/content/121ed75fe9fe5f8e
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.ruff_cache/content/19309938546e93ab
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.ruff_cache/content/197f3188bc94f91f
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.ruff_cache/content/1aa1390b5bde1004
--rw-r--r--   0        0        0     8089 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.ruff_cache/content/1b34455c399f0006
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.ruff_cache/content/1bd1a229a4f4ee7f
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.ruff_cache/content/1c46d1f378d28fbb
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.ruff_cache/content/1ca71ee291d82018
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.ruff_cache/content/1d6bb777df44b8ec
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.ruff_cache/content/1dc8423cfb79eaa4
--rw-r--r--   0        0        0      908 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.ruff_cache/content/20585cf790eae81e
--rw-r--r--   0        0        0    12122 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.ruff_cache/content/221af82ae72a7f27
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.ruff_cache/content/2282e801459c52a4
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.ruff_cache/content/248c4e1a32c704cb
--rw-r--r--   0        0        0    10858 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.ruff_cache/content/24e1b4aab386ebc8
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.ruff_cache/content/28b1d8ac7e2aab6b
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.ruff_cache/content/2b7f7d266c8efaad
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.ruff_cache/content/2dac345be8527adf
--rw-r--r--   0        0        0    11525 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.ruff_cache/content/2f3396c610fd7095
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.ruff_cache/content/31731f8e74291475
--rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.ruff_cache/content/3826106cf4494de8
--rw-r--r--   0        0        0    11210 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.ruff_cache/content/38d5fd55b14a9d6c
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.ruff_cache/content/3afc55a04b8f8bb2
--rw-r--r--   0        0        0    12129 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.ruff_cache/content/4022ee8774ccd98a
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.ruff_cache/content/42f9a2406e74c24f
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.ruff_cache/content/4696b157ff786f22
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.ruff_cache/content/46a88ce266f1ad94
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.ruff_cache/content/4a6edd5010cb9700
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.ruff_cache/content/4d0230e9a81a468
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.ruff_cache/content/52018ba3989fcaf7
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.ruff_cache/content/54e6ba8c25a22ffc
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.ruff_cache/content/566d94db91d23339
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.ruff_cache/content/5b076d769fa5cacd
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.ruff_cache/content/5ceb1580c62ee794
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.ruff_cache/content/6bc90dbb56504f96
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.ruff_cache/content/6f0c8f98e4da1d48
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.ruff_cache/content/74e52af774eebdbd
--rw-r--r--   0        0        0    11023 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.ruff_cache/content/75bd1769f6e29ed7
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.ruff_cache/content/815ba2cfea236769
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.ruff_cache/content/876d9a8d302e1c46
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.ruff_cache/content/88e2927df9448936
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.ruff_cache/content/8c4d3f5ef14b0167
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.ruff_cache/content/8f8ec552e76f3eab
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.ruff_cache/content/95c82d8566c6704c
--rw-r--r--   0        0        0     8349 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.ruff_cache/content/a0739889bf9412e8
--rw-r--r--   0        0        0     5692 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.ruff_cache/content/a225e4df39be9b29
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.ruff_cache/content/a2340fd4c9aa1141
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.ruff_cache/content/a513d558646cd439
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.ruff_cache/content/b121e2b70fd66eb8
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.ruff_cache/content/b218ff88bc22b626
--rw-r--r--   0        0        0    10964 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.ruff_cache/content/b419496fa9e72887
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.ruff_cache/content/b886c97e4d4117f0
--rw-r--r--   0        0        0     8238 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.ruff_cache/content/bdcdf5c7bbc1d738
--rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.ruff_cache/content/c06de16f3c7a64cc
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.ruff_cache/content/c635f255374598c5
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.ruff_cache/content/c671ae94ff3d3e2e
--rw-r--r--   0        0        0     8042 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.ruff_cache/content/cdfecbca581311ee
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.ruff_cache/content/ce44121ca4091b64
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.ruff_cache/content/ced49ec87d10bcb0
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.ruff_cache/content/cfc06a1f13c8ab47
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.ruff_cache/content/d16c5d29763a704e
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.ruff_cache/content/d225ad4c14b8ca60
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.ruff_cache/content/d3a95555c0919160
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.ruff_cache/content/d655bee8ff0a59f2
--rw-r--r--   0        0        0    11315 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.ruff_cache/content/da4811a7730a562a
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.ruff_cache/content/dca573767bc8be7e
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.ruff_cache/content/e3e29f9eacb7027f
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.ruff_cache/content/e46ab4b61bb5d446
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.ruff_cache/content/e5e0cc178d5c9df5
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.ruff_cache/content/eb564f7989641958
--rw-r--r--   0        0        0    11467 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.ruff_cache/content/eee2f3c667de6c7a
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.ruff_cache/content/f04d0d78a00adfd6
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.ruff_cache/content/f2ddc22a4b221f54
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.ruff_cache/content/f879e8c947a6b7a4
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.ruff_cache/content/faa51a5044a3c279
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 typedal-1.0.0b1/htmlcov/.gitignore
--rw-r--r--   0        0        0    21359 2020-02-02 00:00:00.000000 typedal-1.0.0b1/htmlcov/coverage_html.js
--rw-r--r--   0        0        0     5891 2020-02-02 00:00:00.000000 typedal-1.0.0b1/htmlcov/d_0ccc93afd6526b6c___about___py.html
--rw-r--r--   0        0        0     7178 2020-02-02 00:00:00.000000 typedal-1.0.0b1/htmlcov/d_0ccc93afd6526b6c___init___py.html
--rw-r--r--   0        0        0    96583 2020-02-02 00:00:00.000000 typedal-1.0.0b1/htmlcov/d_0ccc93afd6526b6c_core_py.html
--rw-r--r--   0        0        0    63148 2020-02-02 00:00:00.000000 typedal-1.0.0b1/htmlcov/d_0ccc93afd6526b6c_fields_py.html
--rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 typedal-1.0.0b1/htmlcov/favicon_32.png
--rw-r--r--   0        0        0     4823 2020-02-02 00:00:00.000000 typedal-1.0.0b1/htmlcov/index.html
--rw-r--r--   0        0        0     9004 2020-02-02 00:00:00.000000 typedal-1.0.0b1/htmlcov/keybd_closed.png
--rw-r--r--   0        0        0     9003 2020-02-02 00:00:00.000000 typedal-1.0.0b1/htmlcov/keybd_open.png
--rw-r--r--   0        0        0      921 2020-02-02 00:00:00.000000 typedal-1.0.0b1/htmlcov/status.json
--rw-r--r--   0        0        0    12387 2020-02-02 00:00:00.000000 typedal-1.0.0b1/htmlcov/style.css
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 typedal-1.0.0b1/src/typedal/__about__.py
--rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 typedal-1.0.0b1/src/typedal/__init__.py
--rw-r--r--   0        0        0    12033 2020-02-02 00:00:00.000000 typedal-1.0.0b1/src/typedal/core.py
--rw-r--r--   0        0        0     5207 2020-02-02 00:00:00.000000 typedal-1.0.0b1/src/typedal/fields.py
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 typedal-1.0.0b1/tests/__init__.py
--rw-r--r--   0        0        0     7847 2020-02-02 00:00:00.000000 typedal-1.0.0b1/tests/test_main.py
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 typedal-1.0.0b1/.gitignore
--rw-r--r--   0        0        0     9146 2020-02-02 00:00:00.000000 typedal-1.0.0b1/README.md
--rw-r--r--   0        0        0     4619 2020-02-02 00:00:00.000000 typedal-1.0.0b1/pyproject.toml
--rw-r--r--   0        0        0    10151 2020-02-02 00:00:00.000000 typedal-1.0.0b1/PKG-INFO
+-rw-r--r--   0        0        0     2982 2020-02-02 00:00:00.000000 typedal-1.1.1/CHANGELOG.md
+-rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 typedal-1.1.1/coverage.svg
+-rw-r--r--   0        0        0     6840 2020-02-02 00:00:00.000000 typedal-1.1.1/example_new.py
+-rw-r--r--   0        0        0     2872 2020-02-02 00:00:00.000000 typedal-1.1.1/example_old.py
+-rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 typedal-1.1.1/.github/workflows/su6.yml
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/.gitignore
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.10/@plugins_snapshot.json
+-rw-r--r--   0        0        0   177667 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.10/_ast.data.json
+-rw-r--r--   0        0        0     1567 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.10/_ast.meta.json
+-rw-r--r--   0        0        0    52400 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.10/_codecs.data.json
+-rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.10/_codecs.meta.json
+-rw-r--r--   0        0        0    18227 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.10/_collections_abc.data.json
+-rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.10/_collections_abc.meta.json
+-rw-r--r--   0        0        0     2923 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.10/_ctypes.data.json
+-rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.10/_ctypes.meta.json
+-rw-r--r--   0        0        0   170960 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.10/_decimal.data.json
+-rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.10/_decimal.meta.json
+-rw-r--r--   0        0        0    23362 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.10/abc.data.json
+-rw-r--r--   0        0        0     1574 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.10/abc.meta.json
+-rw-r--r--   0        0        0    60687 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.10/array.data.json
+-rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.10/array.meta.json
+-rw-r--r--   0        0        0  1054992 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.10/builtins.data.json
+-rw-r--r--   0        0        0     1721 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.10/builtins.meta.json
+-rw-r--r--   0        0        0   123328 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.10/codecs.data.json
+-rw-r--r--   0        0        0     1671 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.10/codecs.meta.json
+-rw-r--r--   0        0        0   104160 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.10/contextlib.data.json
+-rw-r--r--   0        0        0     1610 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.10/contextlib.meta.json
+-rw-r--r--   0        0        0    57612 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.10/dataclasses.data.json
+-rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.10/dataclasses.meta.json
+-rw-r--r--   0        0        0   142044 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.10/datetime.data.json
+-rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.10/datetime.meta.json
+-rw-r--r--   0        0        0     4911 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.10/decimal.data.json
+-rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.10/decimal.meta.json
+-rw-r--r--   0        0        0    61020 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.10/enum.data.json
+-rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.10/enum.meta.json
+-rw-r--r--   0        0        0    22399 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.10/genericpath.data.json
+-rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.10/genericpath.meta.json
+-rw-r--r--   0        0        0    85348 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.10/io.data.json
+-rw-r--r--   0        0        0     1673 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.10/io.meta.json
+-rw-r--r--   0        0        0    28778 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.10/mmap.data.json
+-rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.10/mmap.meta.json
+-rw-r--r--   0        0        0    78982 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.10/numbers.data.json
+-rw-r--r--   0        0        0     1519 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.10/numbers.meta.json
+-rw-r--r--   0        0        0    88278 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.10/pathlib.data.json
+-rw-r--r--   0        0        0     1682 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.10/pathlib.meta.json
+-rw-r--r--   0        0        0    45131 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.10/pickle.data.json
+-rw-r--r--   0        0        0     1630 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.10/pickle.meta.json
+-rw-r--r--   0        0        0    75208 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.10/posixpath.data.json
+-rw-r--r--   0        0        0     1627 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.10/posixpath.meta.json
+-rw-r--r--   0        0        0   167175 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.10/re.data.json
+-rw-r--r--   0        0        0     1701 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.10/re.meta.json
+-rw-r--r--   0        0        0    14131 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.10/sre_compile.data.json
+-rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.10/sre_compile.meta.json
+-rw-r--r--   0        0        0    28013 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.10/sre_constants.data.json
+-rw-r--r--   0        0        0     1584 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.10/sre_constants.meta.json
+-rw-r--r--   0        0        0    49442 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.10/sre_parse.data.json
+-rw-r--r--   0        0        0     1627 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.10/sre_parse.meta.json
+-rw-r--r--   0        0        0   168498 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.10/subprocess.data.json
+-rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.10/subprocess.meta.json
+-rw-r--r--   0        0        0   146267 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.10/sys.data.json
+-rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.10/sys.meta.json
+-rw-r--r--   0        0        0    43605 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.10/time.data.json
+-rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.10/time.meta.json
+-rw-r--r--   0        0        0   228230 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.10/types.data.json
+-rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.10/types.meta.json
+-rw-r--r--   0        0        0   416965 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.10/typing.data.json
+-rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.10/typing.meta.json
+-rw-r--r--   0        0        0    73907 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.10/typing_extensions.data.json
+-rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.10/typing_extensions.meta.json
+-rw-r--r--   0        0        0    89065 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.10/_typeshed/__init__.data.json
+-rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.10/_typeshed/__init__.meta.json
+-rw-r--r--   0        0        0   407999 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.10/collections/__init__.data.json
+-rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.10/collections/__init__.meta.json
+-rw-r--r--   0        0        0     3731 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.10/collections/abc.data.json
+-rw-r--r--   0        0        0     1558 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.10/collections/abc.meta.json
+-rw-r--r--   0        0        0   128994 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.10/ctypes/__init__.data.json
+-rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.10/ctypes/__init__.meta.json
+-rw-r--r--   0        0        0     7438 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.10/email/__init__.data.json
+-rw-r--r--   0        0        0     1610 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.10/email/__init__.meta.json
+-rw-r--r--   0        0        0    12200 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.10/email/charset.data.json
+-rw-r--r--   0        0        0     1555 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.10/email/charset.meta.json
+-rw-r--r--   0        0        0     7249 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.10/email/contentmanager.data.json
+-rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.10/email/contentmanager.meta.json
+-rw-r--r--   0        0        0    25073 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.10/email/errors.data.json
+-rw-r--r--   0        0        0     1559 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.10/email/errors.meta.json
+-rw-r--r--   0        0        0     9154 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.10/email/header.data.json
+-rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.10/email/header.meta.json
+-rw-r--r--   0        0        0    79298 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.10/email/message.data.json
+-rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.10/email/message.meta.json
+-rw-r--r--   0        0        0    30857 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.10/email/policy.data.json
+-rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.10/email/policy.meta.json
+-rw-r--r--   0        0        0     6125 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.10/importlib/__init__.data.json
+-rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.10/importlib/__init__.meta.json
+-rw-r--r--   0        0        0    70175 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.10/importlib/abc.data.json
+-rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.10/importlib/abc.meta.json
+-rw-r--r--   0        0        0    64626 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.10/importlib/machinery.data.json
+-rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.10/importlib/machinery.meta.json
+-rw-r--r--   0        0        0    90277 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.10/importlib/metadata/__init__.data.json
+-rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.10/importlib/metadata/__init__.meta.json
+-rw-r--r--   0        0        0    11935 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.10/importlib/metadata/_meta.data.json
+-rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.10/importlib/metadata/_meta.meta.json
+-rw-r--r--   0        0        0   350178 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.10/os/__init__.data.json
+-rw-r--r--   0        0        0     1725 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.10/os/__init__.meta.json
+-rw-r--r--   0        0        0     4908 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.10/os/path.data.json
+-rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.10/os/path.meta.json
+-rw-r--r--   0        0        0     1385 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.10/src/__init__.data.json
+-rw-r--r--   0        0        0     1433 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.10/src/__init__.meta.json
+-rw-r--r--   0        0        0     1506 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.10/src/typedal/__about__.data.json
+-rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.10/src/typedal/__about__.meta.json
+-rw-r--r--   0        0        0     2114 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.10/src/typedal/__init__.data.json
+-rw-r--r--   0        0        0     1499 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.10/src/typedal/__init__.meta.json
+-rw-r--r--   0        0        0    33347 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.10/src/typedal/core.data.json
+-rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.10/src/typedal/core.meta.json
+-rw-r--r--   0        0        0    29038 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.10/src/typedal/fields.data.json
+-rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.10/src/typedal/fields.meta.json
+-rw-r--r--   0        0        0     2775 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.10/src/typedal/pydal_objects.data.json
+-rw-r--r--   0        0        0     1503 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.10/src/typedal/pydal_objects.meta.json
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.11/@plugins_snapshot.json
+-rw-r--r--   0        0        0   180368 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.11/_ast.data.json
+-rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.11/_ast.meta.json
+-rw-r--r--   0        0        0    52400 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.11/_codecs.data.json
+-rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.11/_codecs.meta.json
+-rw-r--r--   0        0        0    18227 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.11/_collections_abc.data.json
+-rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.11/_collections_abc.meta.json
+-rw-r--r--   0        0        0     3125 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.11/_ctypes.data.json
+-rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.11/_ctypes.meta.json
+-rw-r--r--   0        0        0   171931 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.11/_decimal.data.json
+-rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.11/_decimal.meta.json
+-rw-r--r--   0        0        0    23336 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.11/abc.data.json
+-rw-r--r--   0        0        0     1574 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.11/abc.meta.json
+-rw-r--r--   0        0        0    60676 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.11/array.data.json
+-rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.11/array.meta.json
+-rw-r--r--   0        0        0  1130454 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.11/builtins.data.json
+-rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.11/builtins.meta.json
+-rw-r--r--   0        0        0   123317 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.11/codecs.data.json
+-rw-r--r--   0        0        0     1671 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.11/codecs.meta.json
+-rw-r--r--   0        0        0   109204 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.11/contextlib.data.json
+-rw-r--r--   0        0        0     1610 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.11/contextlib.meta.json
+-rw-r--r--   0        0        0    57745 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.11/dataclasses.data.json
+-rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.11/dataclasses.meta.json
+-rw-r--r--   0        0        0   142208 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.11/datetime.data.json
+-rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.11/datetime.meta.json
+-rw-r--r--   0        0        0     4911 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.11/decimal.data.json
+-rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.11/decimal.meta.json
+-rw-r--r--   0        0        0    90123 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.11/enum.data.json
+-rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.11/enum.meta.json
+-rw-r--r--   0        0        0    22388 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.11/genericpath.data.json
+-rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.11/genericpath.meta.json
+-rw-r--r--   0        0        0    85337 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.11/io.data.json
+-rw-r--r--   0        0        0     1673 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.11/io.meta.json
+-rw-r--r--   0        0        0    28767 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.11/mmap.data.json
+-rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.11/mmap.meta.json
+-rw-r--r--   0        0        0    78982 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.11/numbers.data.json
+-rw-r--r--   0        0        0     1519 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.11/numbers.meta.json
+-rw-r--r--   0        0        0    87488 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.11/pathlib.data.json
+-rw-r--r--   0        0        0     1682 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.11/pathlib.meta.json
+-rw-r--r--   0        0        0    45131 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.11/pickle.data.json
+-rw-r--r--   0        0        0     1630 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.11/pickle.meta.json
+-rw-r--r--   0        0        0    75197 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.11/posixpath.data.json
+-rw-r--r--   0        0        0     1627 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.11/posixpath.meta.json
+-rw-r--r--   0        0        0   167545 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.11/re.data.json
+-rw-r--r--   0        0        0     1701 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.11/re.meta.json
+-rw-r--r--   0        0        0    14373 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.11/sre_compile.data.json
+-rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.11/sre_compile.meta.json
+-rw-r--r--   0        0        0    28480 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.11/sre_constants.data.json
+-rw-r--r--   0        0        0     1584 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.11/sre_constants.meta.json
+-rw-r--r--   0        0        0    49741 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.11/sre_parse.data.json
+-rw-r--r--   0        0        0     1627 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.11/sre_parse.meta.json
+-rw-r--r--   0        0        0   172768 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.11/subprocess.data.json
+-rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.11/subprocess.meta.json
+-rw-r--r--   0        0        0   148675 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.11/sys.data.json
+-rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.11/sys.meta.json
+-rw-r--r--   0        0        0    43605 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.11/time.data.json
+-rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.11/time.meta.json
+-rw-r--r--   0        0        0   239632 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.11/types.data.json
+-rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.11/types.meta.json
+-rw-r--r--   0        0        0   432234 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.11/typing.data.json
+-rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.11/typing.meta.json
+-rw-r--r--   0        0        0    57845 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.11/typing_extensions.data.json
+-rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.11/typing_extensions.meta.json
+-rw-r--r--   0        0        0    89054 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.11/_typeshed/__init__.data.json
+-rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.11/_typeshed/__init__.meta.json
+-rw-r--r--   0        0        0   407988 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.11/collections/__init__.data.json
+-rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.11/collections/__init__.meta.json
+-rw-r--r--   0        0        0     3731 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.11/collections/abc.data.json
+-rw-r--r--   0        0        0     1558 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.11/collections/abc.meta.json
+-rw-r--r--   0        0        0   128983 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.11/ctypes/__init__.data.json
+-rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.11/ctypes/__init__.meta.json
+-rw-r--r--   0        0        0     7438 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.11/email/__init__.data.json
+-rw-r--r--   0        0        0     1610 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.11/email/__init__.meta.json
+-rw-r--r--   0        0        0    12200 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.11/email/charset.data.json
+-rw-r--r--   0        0        0     1555 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.11/email/charset.meta.json
+-rw-r--r--   0        0        0     7249 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.11/email/contentmanager.data.json
+-rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.11/email/contentmanager.meta.json
+-rw-r--r--   0        0        0    25073 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.11/email/errors.data.json
+-rw-r--r--   0        0        0     1559 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.11/email/errors.meta.json
+-rw-r--r--   0        0        0     9154 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.11/email/header.data.json
+-rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.11/email/header.meta.json
+-rw-r--r--   0        0        0    79287 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.11/email/message.data.json
+-rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.11/email/message.meta.json
+-rw-r--r--   0        0        0    30857 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.11/email/policy.data.json
+-rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.11/email/policy.meta.json
+-rw-r--r--   0        0        0     6125 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.11/importlib/__init__.data.json
+-rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.11/importlib/__init__.meta.json
+-rw-r--r--   0        0        0    70579 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.11/importlib/abc.data.json
+-rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.11/importlib/abc.meta.json
+-rw-r--r--   0        0        0    64626 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.11/importlib/machinery.data.json
+-rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.11/importlib/machinery.meta.json
+-rw-r--r--   0        0        0    91119 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.11/importlib/metadata/__init__.data.json
+-rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.11/importlib/metadata/__init__.meta.json
+-rw-r--r--   0        0        0    11935 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.11/importlib/metadata/_meta.data.json
+-rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.11/importlib/metadata/_meta.meta.json
+-rw-r--r--   0        0        0   350743 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.11/os/__init__.data.json
+-rw-r--r--   0        0        0     1725 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.11/os/__init__.meta.json
+-rw-r--r--   0        0        0     4908 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.11/os/path.data.json
+-rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.11/os/path.meta.json
+-rw-r--r--   0        0        0     1385 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.11/src/__init__.data.json
+-rw-r--r--   0        0        0     1433 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.11/src/__init__.meta.json
+-rw-r--r--   0        0        0     1506 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.11/src/typedal/__about__.data.json
+-rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.11/src/typedal/__about__.meta.json
+-rw-r--r--   0        0        0     2114 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.11/src/typedal/__init__.data.json
+-rw-r--r--   0        0        0     1499 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.11/src/typedal/__init__.meta.json
+-rw-r--r--   0        0        0    33350 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.11/src/typedal/core.data.json
+-rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.11/src/typedal/core.meta.json
+-rw-r--r--   0        0        0    29038 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.11/src/typedal/fields.data.json
+-rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.11/src/typedal/fields.meta.json
+-rw-r--r--   0        0        0     1478 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.11/typedal/__about__.data.json
+-rw-r--r--   0        0        0     1458 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.11/typedal/__about__.meta.json
+-rw-r--r--   0        0        0     2274 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.11/typedal/__init__.data.json
+-rw-r--r--   0        0        0     1487 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.11/typedal/__init__.meta.json
+-rw-r--r--   0        0        0    34871 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.11/typedal/core.data.json
+-rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.11/typedal/core.meta.json
+-rw-r--r--   0        0        0    28193 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.11/typedal/fields.data.json
+-rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 typedal-1.1.1/.mypy_cache/3.11/typedal/fields.meta.json
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 typedal-1.1.1/.pytest_cache/.gitignore
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 typedal-1.1.1/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 typedal-1.1.1/.pytest_cache/README.md
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 typedal-1.1.1/.pytest_cache/v/cache/lastfailed
+-rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 typedal-1.1.1/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 typedal-1.1.1/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 typedal-1.1.1/.ruff_cache/.gitignore
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 typedal-1.1.1/.ruff_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 typedal-1.1.1/.ruff_cache/content/1215429078721865123
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.1.1/.ruff_cache/content/121ed75fe9fe5f8e
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.1.1/.ruff_cache/content/19309938546e93ab
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.1.1/.ruff_cache/content/197f3188bc94f91f
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.1.1/.ruff_cache/content/1aa1390b5bde1004
+-rw-r--r--   0        0        0     8089 2020-02-02 00:00:00.000000 typedal-1.1.1/.ruff_cache/content/1b34455c399f0006
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.1.1/.ruff_cache/content/1bd1a229a4f4ee7f
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.1.1/.ruff_cache/content/1c46d1f378d28fbb
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.1.1/.ruff_cache/content/1ca71ee291d82018
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.1.1/.ruff_cache/content/1d6bb777df44b8ec
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.1.1/.ruff_cache/content/1dc8423cfb79eaa4
+-rw-r--r--   0        0        0      908 2020-02-02 00:00:00.000000 typedal-1.1.1/.ruff_cache/content/20585cf790eae81e
+-rw-r--r--   0        0        0    12122 2020-02-02 00:00:00.000000 typedal-1.1.1/.ruff_cache/content/221af82ae72a7f27
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.1.1/.ruff_cache/content/2282e801459c52a4
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.1.1/.ruff_cache/content/248c4e1a32c704cb
+-rw-r--r--   0        0        0    10858 2020-02-02 00:00:00.000000 typedal-1.1.1/.ruff_cache/content/24e1b4aab386ebc8
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.1.1/.ruff_cache/content/28b1d8ac7e2aab6b
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.1.1/.ruff_cache/content/2b7f7d266c8efaad
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.1.1/.ruff_cache/content/2bb6610cadf18e18
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.1.1/.ruff_cache/content/2dac345be8527adf
+-rw-r--r--   0        0        0    11525 2020-02-02 00:00:00.000000 typedal-1.1.1/.ruff_cache/content/2f3396c610fd7095
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.1.1/.ruff_cache/content/31731f8e74291475
+-rw-r--r--   0        0        0    13342 2020-02-02 00:00:00.000000 typedal-1.1.1/.ruff_cache/content/322af04e6d059ce5
+-rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 typedal-1.1.1/.ruff_cache/content/3826106cf4494de8
+-rw-r--r--   0        0        0    11210 2020-02-02 00:00:00.000000 typedal-1.1.1/.ruff_cache/content/38d5fd55b14a9d6c
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.1.1/.ruff_cache/content/3afc55a04b8f8bb2
+-rw-r--r--   0        0        0    12129 2020-02-02 00:00:00.000000 typedal-1.1.1/.ruff_cache/content/4022ee8774ccd98a
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.1.1/.ruff_cache/content/42f9a2406e74c24f
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.1.1/.ruff_cache/content/4696b157ff786f22
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.1.1/.ruff_cache/content/46a88ce266f1ad94
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.1.1/.ruff_cache/content/4a6edd5010cb9700
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.1.1/.ruff_cache/content/4d0230e9a81a468
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.1.1/.ruff_cache/content/52018ba3989fcaf7
+-rw-r--r--   0        0        0    13679 2020-02-02 00:00:00.000000 typedal-1.1.1/.ruff_cache/content/5491563776466765346
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.1.1/.ruff_cache/content/54e6ba8c25a22ffc
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.1.1/.ruff_cache/content/566d94db91d23339
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.1.1/.ruff_cache/content/5a67aed8f6b70cd5
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.1.1/.ruff_cache/content/5b076d769fa5cacd
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.1.1/.ruff_cache/content/5ceb1580c62ee794
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.1.1/.ruff_cache/content/6bc90dbb56504f96
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.1.1/.ruff_cache/content/6c52d14716eee431
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.1.1/.ruff_cache/content/6f0c8f98e4da1d48
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.1.1/.ruff_cache/content/74e52af774eebdbd
+-rw-r--r--   0        0        0    11023 2020-02-02 00:00:00.000000 typedal-1.1.1/.ruff_cache/content/75bd1769f6e29ed7
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.1.1/.ruff_cache/content/815ba2cfea236769
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.1.1/.ruff_cache/content/876d9a8d302e1c46
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.1.1/.ruff_cache/content/88e2927df9448936
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.1.1/.ruff_cache/content/8c4d3f5ef14b0167
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.1.1/.ruff_cache/content/8f8ec552e76f3eab
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.1.1/.ruff_cache/content/95c82d8566c6704c
+-rw-r--r--   0        0        0     8349 2020-02-02 00:00:00.000000 typedal-1.1.1/.ruff_cache/content/a0739889bf9412e8
+-rw-r--r--   0        0        0     5692 2020-02-02 00:00:00.000000 typedal-1.1.1/.ruff_cache/content/a225e4df39be9b29
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.1.1/.ruff_cache/content/a2340fd4c9aa1141
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.1.1/.ruff_cache/content/a513d558646cd439
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.1.1/.ruff_cache/content/b121e2b70fd66eb8
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.1.1/.ruff_cache/content/b218ff88bc22b626
+-rw-r--r--   0        0        0    10964 2020-02-02 00:00:00.000000 typedal-1.1.1/.ruff_cache/content/b419496fa9e72887
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.1.1/.ruff_cache/content/b886c97e4d4117f0
+-rw-r--r--   0        0        0     8238 2020-02-02 00:00:00.000000 typedal-1.1.1/.ruff_cache/content/bdcdf5c7bbc1d738
+-rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 typedal-1.1.1/.ruff_cache/content/c06de16f3c7a64cc
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.1.1/.ruff_cache/content/c635f255374598c5
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.1.1/.ruff_cache/content/c671ae94ff3d3e2e
+-rw-r--r--   0        0        0     8042 2020-02-02 00:00:00.000000 typedal-1.1.1/.ruff_cache/content/cdfecbca581311ee
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.1.1/.ruff_cache/content/ce44121ca4091b64
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.1.1/.ruff_cache/content/ced49ec87d10bcb0
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.1.1/.ruff_cache/content/cfc06a1f13c8ab47
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.1.1/.ruff_cache/content/d16c5d29763a704e
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.1.1/.ruff_cache/content/d225ad4c14b8ca60
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.1.1/.ruff_cache/content/d379b35d5e80b789
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.1.1/.ruff_cache/content/d3a95555c0919160
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.1.1/.ruff_cache/content/d655bee8ff0a59f2
+-rw-r--r--   0        0        0    11315 2020-02-02 00:00:00.000000 typedal-1.1.1/.ruff_cache/content/da4811a7730a562a
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.1.1/.ruff_cache/content/dca573767bc8be7e
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.1.1/.ruff_cache/content/e3e29f9eacb7027f
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.1.1/.ruff_cache/content/e46ab4b61bb5d446
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.1.1/.ruff_cache/content/e5e0cc178d5c9df5
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.1.1/.ruff_cache/content/eb564f7989641958
+-rw-r--r--   0        0        0    11467 2020-02-02 00:00:00.000000 typedal-1.1.1/.ruff_cache/content/eee2f3c667de6c7a
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.1.1/.ruff_cache/content/f04d0d78a00adfd6
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.1.1/.ruff_cache/content/f2ddc22a4b221f54
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.1.1/.ruff_cache/content/f879e8c947a6b7a4
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.1.1/.ruff_cache/content/fa45ef3c3166e02d
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.1.1/.ruff_cache/content/faa51a5044a3c279
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 typedal-1.1.1/htmlcov/.gitignore
+-rw-r--r--   0        0        0    21359 2020-02-02 00:00:00.000000 typedal-1.1.1/htmlcov/coverage_html.js
+-rw-r--r--   0        0        0     5891 2020-02-02 00:00:00.000000 typedal-1.1.1/htmlcov/d_0ccc93afd6526b6c___about___py.html
+-rw-r--r--   0        0        0     7178 2020-02-02 00:00:00.000000 typedal-1.1.1/htmlcov/d_0ccc93afd6526b6c___init___py.html
+-rw-r--r--   0        0        0   104085 2020-02-02 00:00:00.000000 typedal-1.1.1/htmlcov/d_0ccc93afd6526b6c_core_py.html
+-rw-r--r--   0        0        0    63516 2020-02-02 00:00:00.000000 typedal-1.1.1/htmlcov/d_0ccc93afd6526b6c_fields_py.html
+-rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 typedal-1.1.1/htmlcov/favicon_32.png
+-rw-r--r--   0        0        0     4821 2020-02-02 00:00:00.000000 typedal-1.1.1/htmlcov/index.html
+-rw-r--r--   0        0        0     9004 2020-02-02 00:00:00.000000 typedal-1.1.1/htmlcov/keybd_closed.png
+-rw-r--r--   0        0        0     9003 2020-02-02 00:00:00.000000 typedal-1.1.1/htmlcov/keybd_open.png
+-rw-r--r--   0        0        0      923 2020-02-02 00:00:00.000000 typedal-1.1.1/htmlcov/status.json
+-rw-r--r--   0        0        0    12387 2020-02-02 00:00:00.000000 typedal-1.1.1/htmlcov/style.css
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 typedal-1.1.1/src/typedal/__about__.py
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 typedal-1.1.1/src/typedal/__init__.py
+-rw-r--r--   0        0        0    13165 2020-02-02 00:00:00.000000 typedal-1.1.1/src/typedal/core.py
+-rw-r--r--   0        0        0     4949 2020-02-02 00:00:00.000000 typedal-1.1.1/src/typedal/fields.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 typedal-1.1.1/src/typedal/py.typed
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 typedal-1.1.1/tests/__init__.py
+-rw-r--r--   0        0        0     7918 2020-02-02 00:00:00.000000 typedal-1.1.1/tests/test_main.py
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 typedal-1.1.1/.gitignore
+-rw-r--r--   0        0        0     9220 2020-02-02 00:00:00.000000 typedal-1.1.1/README.md
+-rw-r--r--   0        0        0     4782 2020-02-02 00:00:00.000000 typedal-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0    10274 2020-02-02 00:00:00.000000 typedal-1.1.1/PKG-INFO
```

### Comparing `typedal-1.0.0b1/CHANGELOG.md` & `typedal-1.1.1/CHANGELOG.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,33 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
-## v1.0.0-beta.1 (2023-06-05)
+## v1.1.1 (2023-06-22)
+### Fix
+
+* **mypy:** Made the package properly typed ([`a242895`](https://github.com/trialandsuccess/TypeDAL/commit/a242895d9d8a2d04add9c863105c2b1c756a3b6a))
+
+## v1.1.0 (2023-06-22)
+### Feature
+
+* **types:** You should use `param = TypedField()` instead of `param: TypedField()` from now on for better mypy support ([`ed50273`](https://github.com/trialandsuccess/TypeDAL/commit/ed50273ded4a178a30ec8c9d6f492b871853a568))
+
+### Fix
+
+* **version:** We were already on 1.0.0 ([`d6a8d0d`](https://github.com/trialandsuccess/TypeDAL/commit/d6a8d0d17274a5a89e7c0260ba00bb916533866c))
+
+### Documentation
+
+* More info about new release ([`ddfffe2`](https://github.com/trialandsuccess/TypeDAL/commit/ddfffe2c5e6a8f7799449d059e5a2b8dd9c95dab))
+
+## v1.0.0 (2023-06-05)
+Refactored pre-1.0 code and added [su6](https://github.com/robinvandernoord/su6-checker) checker tool.  
+Moved to `pyproject.toml` based build system.
+
 ### Feature
 * **su6:** Add github workflow with checkers ([`d462387`](https://github.com/trialandsuccess/TypeDAL/commit/d46238705b27137ed60806eca5c53d8c2940052f))
 * **tests:** Moved tests.py to pytest ([`de33d20`](https://github.com/trialandsuccess/TypeDAL/commit/de33d2053e6499c4a8628cfc4b8813b5a649c584))
 * **define:** Pass extra kwargs (e.g. format) to define_table ([`bb692dc`](https://github.com/trialandsuccess/TypeDAL/commit/bb692dc1b2a9c18e45bcb70771b7435df8a39c8e))
 * **TypedRows:** Subscriptable return type for .select() ([`7b674b0`](https://github.com/trialandsuccess/TypeDAL/commit/7b674b07d4e61f4ead5d3f006e018b1aa66c10e7))
 * Add specific Fields, experimented with __future__.annotations (does not work right now) and general improvements ([`9af27c2`](https://github.com/trialandsuccess/TypeDAL/commit/9af27c254bf2ad7bd3bfa80e66b6e08e82f8f13a))
```

### Comparing `typedal-1.0.0b1/coverage.svg` & `typedal-1.1.1/coverage.svg`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/example_new.py` & `typedal-1.1.1/example_new.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,22 +11,23 @@
 
 ### basic examples
 
 @db.define
 class Person(TypedTable):
     name: str
 
-    # todo: let pycharm know age is actually int
-    age: TypedField(int, default=18)
+    age = TypedField(int, default=18)
     nicknames: list[str]
 
     format = "%(name)s"
 
+
 assert db.person._format == "%(name)s"
 
+
 @db.define
 class Pet(TypedTable):
     name: str
     owners: list[Person]
 
 
 # delayed define (without decorator):
@@ -62,118 +63,93 @@
 ### example with all possible field types;
 
 @db.define
 class OtherTable(TypedTable):
     ...
 
 
-# class AllFields(TypedTable):
-#     # http://www.web2py.com/books/default/chapter/29/06/the-database-abstraction-layer#Field-types
-#     string: str | TypedField(str)
-#     text: TypedField(str, type="text")
-#     blob: bytes | TypedField(bytes)
-#     boolean: bool | TypedField(bool)
-#     integer: int | TypedField(int)
-#     double: float | TypedField(float)
-#     decimal: Decimal | TypedField(Decimal, n=2, m=3)
-#     date: dt.date | TypedField(dt.date)
-#     time: dt.time | TypedField(dt.time)
-#     datetime: dt.datetime | TypedField(dt.datetime)
-#     password: TypedField(str, type="password")
-#     upload: TypedField(str, uploadfield="upload_data")
-#     upload_data: bytes | TypedField(bytes)
-#     reference: OtherTable | TypedField(OtherTable)
-#     list_string: list[str] | TypedField(list[str])
-#     list_integer: list[int] | TypedField(list[int])
-#     list_reference: list[OtherTable] | TypedField(list[OtherTable])
-#     json: object | TypedField(object)
-#     bigint: TypedField(int, type="bigint")
-
-
 @db.define
 class AllFieldsBasic(TypedTable):
     # http://www.web2py.com/books/default/chapter/29/06/the-database-abstraction-layer#Field-types
     string: typing.Optional[str]
     # string: str | None
-    text: TypedField(str, type="text")
+    text = TypedField(str, type="text")
     blob: bytes
     boolean: bool
     integer: int
     double: float
     decimal: Decimal
     date: dt.date
     time: dt.time
     datetime: dt.datetime
-    password: TypedField(str, type="password")
-    upload: TypedField(str, type="upload", uploadfield="upload_data")
+    password = TypedField(str, type="password")
+    upload = TypedField(str, type="upload", uploadfield="upload_data")
     upload_data: bytes
     reference: OtherTable
     reference_two: typing.Optional[db.other_table]
     list_string: list[str]
     list_integer: list[int]
     list_reference: list[OtherTable]
     json: object
-    bigint: TypedField(int, type="bigint")
+    bigint = TypedField(int, type="bigint")
 
 
 @db.define
 class AllFieldsAdvanced(TypedTable):
     # http://www.web2py.com/books/default/chapter/29/06/the-database-abstraction-layer#Field-types
 
     # typing.Optional won't work on a TypedField! todo: document caveat
-    string: TypedField(str, length=1000, notnull=False)
-    text: TextField()
-    blob: TypedField(bytes)
-    boolean: TypedField(bool)
-    integer: TypedField(int)
-    double: TypedField(float)
-    decimal: TypedField(Decimal, n=2, m=3)
-    date: TypedField(dt.date)
-    time: TypedField(dt.time)
-    datetime: TypedField(dt.datetime)
-    password: TypedField(str, type="password")
-    upload: TypedField(str, type="upload", uploadfield="upload_data")
-    upload_data: TypedField(bytes)
-    reference: TypedField(OtherTable)
-    reference_two: TypedField(db.other_table, notnull=False)
-    list_string: TypedField(list[str])
-    list_integer: TypedField(list[int])
-    list_reference: TypedField(list[OtherTable])
-    json: TypedField(object)
-    bigint: TypedField(int, type="bigint")
+    string = TypedField(str, length=1000, notnull=False)
+    text = TextField()
+    blob = TypedField(bytes)
+    boolean = TypedField(bool)
+    integer = TypedField(int)
+    double = TypedField(float)
+    decimal = TypedField(Decimal, n=2, m=3)
+    date = TypedField(dt.date)
+    time = TypedField(dt.time)
+    datetime = TypedField(dt.datetime)
+    password = TypedField(str, type="password")
+    upload = TypedField(str, type="upload", uploadfield="upload_data")
+    upload_data = TypedField(bytes)
+    reference = TypedField(OtherTable)
+    reference_two = TypedField(db.other_table, notnull=False)
+    list_string = TypedField(list[str])
+    list_integer = TypedField(list[int])
+    list_reference = TypedField(list[OtherTable])
+    json = TypedField(object)
+    bigint = TypedField(int, type="bigint")
 
 
 @db.define
 class AllFieldsExplicit(TypedTable):
     # http://www.web2py.com/books/default/chapter/29/06/the-database-abstraction-layer#Field-types
 
     # typing.Optional won't work on a TypedField! todo: document caveat
-    string: fields.StringField(length=1000, notnull=False)
-    text: fields.TextField()
-    blob: fields.BlobField()
-    boolean: fields.BooleanField()
-    integer: fields.IntegerField()
-    double: fields.DoubleField()
-    decimal: fields.DecimalField(n=2, m=3)
-    date: fields.DateField()
-    time: fields.TimeField()
-    datetime: fields.DatetimeField()
-    password: fields.PasswordField()
-    upload: fields.UploadField(uploadfield="upload_data")
-    upload_data: fields.BlobField()
-    reference: fields.ReferenceField("other_table")
-    reference_two: fields.ReferenceField("other_table", notnull=False)
-    list_string: fields.ListStringField()
-    list_integer: fields.ListIntegerField()
-    list_reference: fields.ListReferenceField('other_table')
-    json: fields.JSONField()
-    bigint: fields.BigintField()
-
+    string = fields.StringField(length=1000, notnull=False)
+    text = fields.TextField()
+    blob = fields.BlobField()
+    boolean = fields.BooleanField()
+    integer = fields.IntegerField()
+    double = fields.DoubleField()
+    decimal = fields.DecimalField(n=2, m=3)
+    date = fields.DateField()
+    time = fields.TimeField()
+    datetime = fields.DatetimeField()
+    password = fields.PasswordField()
+    upload = fields.UploadField(uploadfield="upload_data")
+    upload_data = fields.BlobField()
+    reference = fields.ReferenceField("other_table")
+    reference_two = fields.ReferenceField("other_table", notnull=False)
+    list_string = fields.ListStringField()
+    list_integer = fields.ListIntegerField()
+    list_reference = fields.ListReferenceField('other_table')
+    json = fields.JSONField()
+    bigint = fields.BigintField()
 
-xyz = AllFieldsExplicit.text
 
 # todo: fix:
 # for fname, ftype in AllFieldsBasic.__annotations__.items():
 #     print(fname, repr(ftype))
 #
 # for fname, ftype in AllFieldsAdvanced.__annotations__.items():
 #     print(fname, repr(ftype))
```

### Comparing `typedal-1.0.0b1/example_old.py` & `typedal-1.1.1/example_old.py`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.10/_ast.data.json` & `typedal-1.1.1/.mypy_cache/3.10/_ast.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.10/_ast.meta.json` & `typedal-1.1.1/.mypy_cache/3.10/_ast.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.10/_codecs.data.json` & `typedal-1.1.1/.mypy_cache/3.10/_codecs.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.10/_codecs.meta.json` & `typedal-1.1.1/.mypy_cache/3.10/_codecs.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.10/_collections_abc.data.json` & `typedal-1.1.1/.mypy_cache/3.10/_collections_abc.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.10/_collections_abc.meta.json` & `typedal-1.1.1/.mypy_cache/3.10/_collections_abc.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.10/_ctypes.data.json` & `typedal-1.1.1/.mypy_cache/3.10/_ctypes.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.10/_ctypes.meta.json` & `typedal-1.1.1/.mypy_cache/3.10/_ctypes.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.10/_decimal.data.json` & `typedal-1.1.1/.mypy_cache/3.10/_decimal.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.10/_decimal.meta.json` & `typedal-1.1.1/.mypy_cache/3.10/_decimal.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.10/abc.data.json` & `typedal-1.1.1/.mypy_cache/3.10/abc.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.10/abc.meta.json` & `typedal-1.1.1/.mypy_cache/3.10/abc.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.10/array.data.json` & `typedal-1.1.1/.mypy_cache/3.10/array.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.10/array.meta.json` & `typedal-1.1.1/.mypy_cache/3.10/array.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.10/builtins.data.json` & `typedal-1.1.1/.mypy_cache/3.10/builtins.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.10/builtins.meta.json` & `typedal-1.1.1/.mypy_cache/3.10/builtins.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.10/codecs.data.json` & `typedal-1.1.1/.mypy_cache/3.10/codecs.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.10/codecs.meta.json` & `typedal-1.1.1/.mypy_cache/3.10/codecs.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.10/contextlib.data.json` & `typedal-1.1.1/.mypy_cache/3.10/contextlib.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.10/contextlib.meta.json` & `typedal-1.1.1/.mypy_cache/3.10/contextlib.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.10/dataclasses.data.json` & `typedal-1.1.1/.mypy_cache/3.10/dataclasses.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.10/dataclasses.meta.json` & `typedal-1.1.1/.mypy_cache/3.10/dataclasses.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.10/datetime.data.json` & `typedal-1.1.1/.mypy_cache/3.10/datetime.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.10/datetime.meta.json` & `typedal-1.1.1/.mypy_cache/3.10/datetime.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.10/decimal.data.json` & `typedal-1.1.1/.mypy_cache/3.10/decimal.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.10/decimal.meta.json` & `typedal-1.1.1/.mypy_cache/3.10/decimal.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.10/enum.data.json` & `typedal-1.1.1/.mypy_cache/3.10/enum.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.10/enum.meta.json` & `typedal-1.1.1/.mypy_cache/3.10/enum.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.10/genericpath.data.json` & `typedal-1.1.1/.mypy_cache/3.10/genericpath.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.10/genericpath.meta.json` & `typedal-1.1.1/.mypy_cache/3.10/genericpath.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.10/io.data.json` & `typedal-1.1.1/.mypy_cache/3.10/io.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.10/io.meta.json` & `typedal-1.1.1/.mypy_cache/3.10/io.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.10/mmap.data.json` & `typedal-1.1.1/.mypy_cache/3.10/mmap.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.10/mmap.meta.json` & `typedal-1.1.1/.mypy_cache/3.10/mmap.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.10/numbers.data.json` & `typedal-1.1.1/.mypy_cache/3.10/numbers.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.10/numbers.meta.json` & `typedal-1.1.1/.mypy_cache/3.10/numbers.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.10/pathlib.data.json` & `typedal-1.1.1/.mypy_cache/3.10/pathlib.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.10/pathlib.meta.json` & `typedal-1.1.1/.mypy_cache/3.10/pathlib.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.10/pickle.data.json` & `typedal-1.1.1/.mypy_cache/3.10/pickle.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.10/pickle.meta.json` & `typedal-1.1.1/.mypy_cache/3.10/pickle.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.10/posixpath.data.json` & `typedal-1.1.1/.mypy_cache/3.10/posixpath.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.10/posixpath.meta.json` & `typedal-1.1.1/.mypy_cache/3.10/posixpath.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.10/re.data.json` & `typedal-1.1.1/.mypy_cache/3.10/re.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.10/re.meta.json` & `typedal-1.1.1/.mypy_cache/3.10/re.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.10/sre_compile.data.json` & `typedal-1.1.1/.mypy_cache/3.10/sre_compile.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.10/sre_compile.meta.json` & `typedal-1.1.1/.mypy_cache/3.10/sre_compile.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.10/sre_constants.data.json` & `typedal-1.1.1/.mypy_cache/3.10/sre_constants.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.10/sre_constants.meta.json` & `typedal-1.1.1/.mypy_cache/3.10/sre_constants.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.10/sre_parse.data.json` & `typedal-1.1.1/.mypy_cache/3.10/sre_parse.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.10/sre_parse.meta.json` & `typedal-1.1.1/.mypy_cache/3.10/sre_parse.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.10/subprocess.data.json` & `typedal-1.1.1/.mypy_cache/3.10/subprocess.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.10/subprocess.meta.json` & `typedal-1.1.1/.mypy_cache/3.10/subprocess.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.10/sys.data.json` & `typedal-1.1.1/.mypy_cache/3.10/sys.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.10/sys.meta.json` & `typedal-1.1.1/.mypy_cache/3.10/sys.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.10/time.data.json` & `typedal-1.1.1/.mypy_cache/3.10/time.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.10/time.meta.json` & `typedal-1.1.1/.mypy_cache/3.10/time.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.10/types.data.json` & `typedal-1.1.1/.mypy_cache/3.10/types.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.10/types.meta.json` & `typedal-1.1.1/.mypy_cache/3.10/types.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.10/typing.data.json` & `typedal-1.1.1/.mypy_cache/3.10/typing.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.10/typing.meta.json` & `typedal-1.1.1/.mypy_cache/3.10/typing.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.10/typing_extensions.data.json` & `typedal-1.1.1/.mypy_cache/3.10/typing_extensions.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.10/typing_extensions.meta.json` & `typedal-1.1.1/.mypy_cache/3.10/typing_extensions.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.10/_typeshed/__init__.data.json` & `typedal-1.1.1/.mypy_cache/3.10/_typeshed/__init__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.10/_typeshed/__init__.meta.json` & `typedal-1.1.1/.mypy_cache/3.10/_typeshed/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.10/collections/__init__.data.json` & `typedal-1.1.1/.mypy_cache/3.10/collections/__init__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.10/collections/__init__.meta.json` & `typedal-1.1.1/.mypy_cache/3.10/collections/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.10/collections/abc.data.json` & `typedal-1.1.1/.mypy_cache/3.10/collections/abc.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.10/collections/abc.meta.json` & `typedal-1.1.1/.mypy_cache/3.10/collections/abc.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.10/ctypes/__init__.data.json` & `typedal-1.1.1/.mypy_cache/3.10/ctypes/__init__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.10/ctypes/__init__.meta.json` & `typedal-1.1.1/.mypy_cache/3.10/ctypes/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.10/email/__init__.data.json` & `typedal-1.1.1/.mypy_cache/3.10/email/__init__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.10/email/__init__.meta.json` & `typedal-1.1.1/.mypy_cache/3.10/email/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.10/email/charset.data.json` & `typedal-1.1.1/.mypy_cache/3.10/email/charset.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.10/email/charset.meta.json` & `typedal-1.1.1/.mypy_cache/3.10/email/charset.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.10/email/contentmanager.data.json` & `typedal-1.1.1/.mypy_cache/3.10/email/contentmanager.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.10/email/contentmanager.meta.json` & `typedal-1.1.1/.mypy_cache/3.10/email/contentmanager.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.10/email/errors.data.json` & `typedal-1.1.1/.mypy_cache/3.10/email/errors.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.10/email/errors.meta.json` & `typedal-1.1.1/.mypy_cache/3.10/email/errors.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.10/email/header.data.json` & `typedal-1.1.1/.mypy_cache/3.10/email/header.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.10/email/header.meta.json` & `typedal-1.1.1/.mypy_cache/3.10/email/header.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.10/email/message.data.json` & `typedal-1.1.1/.mypy_cache/3.10/email/message.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.10/email/message.meta.json` & `typedal-1.1.1/.mypy_cache/3.10/email/message.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.10/email/policy.data.json` & `typedal-1.1.1/.mypy_cache/3.10/email/policy.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.10/email/policy.meta.json` & `typedal-1.1.1/.mypy_cache/3.10/email/policy.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.10/importlib/__init__.data.json` & `typedal-1.1.1/.mypy_cache/3.10/importlib/__init__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.10/importlib/__init__.meta.json` & `typedal-1.1.1/.mypy_cache/3.10/importlib/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.10/importlib/abc.data.json` & `typedal-1.1.1/.mypy_cache/3.10/importlib/abc.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.10/importlib/abc.meta.json` & `typedal-1.1.1/.mypy_cache/3.10/importlib/abc.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.10/importlib/machinery.data.json` & `typedal-1.1.1/.mypy_cache/3.10/importlib/machinery.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.10/importlib/machinery.meta.json` & `typedal-1.1.1/.mypy_cache/3.10/importlib/machinery.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.10/importlib/metadata/__init__.data.json` & `typedal-1.1.1/.mypy_cache/3.10/importlib/metadata/__init__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.10/importlib/metadata/__init__.meta.json` & `typedal-1.1.1/.mypy_cache/3.10/importlib/metadata/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.10/importlib/metadata/_meta.data.json` & `typedal-1.1.1/.mypy_cache/3.10/importlib/metadata/_meta.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.10/importlib/metadata/_meta.meta.json` & `typedal-1.1.1/.mypy_cache/3.10/importlib/metadata/_meta.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.10/os/__init__.data.json` & `typedal-1.1.1/.mypy_cache/3.10/os/__init__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.10/os/__init__.meta.json` & `typedal-1.1.1/.mypy_cache/3.10/os/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.10/os/path.data.json` & `typedal-1.1.1/.mypy_cache/3.10/os/path.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.10/os/path.meta.json` & `typedal-1.1.1/.mypy_cache/3.10/os/path.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.10/src/__init__.data.json` & `typedal-1.1.1/.mypy_cache/3.10/src/__init__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.10/src/__init__.meta.json` & `typedal-1.1.1/.mypy_cache/3.10/src/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.10/src/typedal/__about__.data.json` & `typedal-1.1.1/.mypy_cache/3.10/src/typedal/__about__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.10/src/typedal/__about__.meta.json` & `typedal-1.1.1/.mypy_cache/3.10/src/typedal/__about__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.10/src/typedal/__init__.data.json` & `typedal-1.1.1/.mypy_cache/3.10/src/typedal/__init__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.10/src/typedal/__init__.meta.json` & `typedal-1.1.1/.mypy_cache/3.10/src/typedal/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.10/src/typedal/core.data.json` & `typedal-1.1.1/.mypy_cache/3.10/src/typedal/core.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.10/src/typedal/core.meta.json` & `typedal-1.1.1/.mypy_cache/3.10/src/typedal/core.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.10/src/typedal/fields.data.json` & `typedal-1.1.1/.mypy_cache/3.10/src/typedal/fields.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.10/src/typedal/fields.meta.json` & `typedal-1.1.1/.mypy_cache/3.10/src/typedal/fields.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.10/src/typedal/pydal_objects.data.json` & `typedal-1.1.1/.mypy_cache/3.10/src/typedal/pydal_objects.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.10/src/typedal/pydal_objects.meta.json` & `typedal-1.1.1/.mypy_cache/3.10/src/typedal/pydal_objects.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.11/_ast.data.json` & `typedal-1.1.1/.mypy_cache/3.11/_ast.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.11/_ast.meta.json` & `typedal-1.1.1/.mypy_cache/3.11/_ast.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.11/_codecs.data.json` & `typedal-1.1.1/.mypy_cache/3.11/_codecs.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.11/_codecs.meta.json` & `typedal-1.1.1/.mypy_cache/3.11/_codecs.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.11/_collections_abc.data.json` & `typedal-1.1.1/.mypy_cache/3.11/_collections_abc.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.11/_collections_abc.meta.json` & `typedal-1.1.1/.mypy_cache/3.11/_collections_abc.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.11/_ctypes.data.json` & `typedal-1.1.1/.mypy_cache/3.11/_ctypes.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.11/_ctypes.meta.json` & `typedal-1.1.1/.mypy_cache/3.11/_ctypes.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.11/_decimal.data.json` & `typedal-1.1.1/.mypy_cache/3.11/_decimal.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.11/_decimal.meta.json` & `typedal-1.1.1/.mypy_cache/3.11/_decimal.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.11/abc.data.json` & `typedal-1.1.1/.mypy_cache/3.11/abc.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.11/abc.meta.json` & `typedal-1.1.1/.mypy_cache/3.11/abc.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.11/array.data.json` & `typedal-1.1.1/.mypy_cache/3.11/array.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.11/array.meta.json` & `typedal-1.1.1/.mypy_cache/3.11/array.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.11/builtins.data.json` & `typedal-1.1.1/.mypy_cache/3.11/builtins.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.11/builtins.meta.json` & `typedal-1.1.1/.mypy_cache/3.11/builtins.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.11/codecs.data.json` & `typedal-1.1.1/.mypy_cache/3.11/codecs.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.11/codecs.meta.json` & `typedal-1.1.1/.mypy_cache/3.11/codecs.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.11/contextlib.data.json` & `typedal-1.1.1/.mypy_cache/3.11/contextlib.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.11/contextlib.meta.json` & `typedal-1.1.1/.mypy_cache/3.11/contextlib.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.11/dataclasses.data.json` & `typedal-1.1.1/.mypy_cache/3.11/dataclasses.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.11/dataclasses.meta.json` & `typedal-1.1.1/.mypy_cache/3.11/dataclasses.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.11/datetime.data.json` & `typedal-1.1.1/.mypy_cache/3.11/datetime.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.11/datetime.meta.json` & `typedal-1.1.1/.mypy_cache/3.11/datetime.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.11/decimal.data.json` & `typedal-1.1.1/.mypy_cache/3.11/decimal.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.11/decimal.meta.json` & `typedal-1.1.1/.mypy_cache/3.11/decimal.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.11/enum.data.json` & `typedal-1.1.1/.mypy_cache/3.11/enum.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.11/enum.meta.json` & `typedal-1.1.1/.mypy_cache/3.11/enum.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.11/genericpath.data.json` & `typedal-1.1.1/.mypy_cache/3.11/genericpath.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.11/genericpath.meta.json` & `typedal-1.1.1/.mypy_cache/3.11/genericpath.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.11/io.data.json` & `typedal-1.1.1/.mypy_cache/3.11/io.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.11/io.meta.json` & `typedal-1.1.1/.mypy_cache/3.11/io.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.11/mmap.data.json` & `typedal-1.1.1/.mypy_cache/3.11/mmap.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.11/mmap.meta.json` & `typedal-1.1.1/.mypy_cache/3.11/mmap.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.11/numbers.data.json` & `typedal-1.1.1/.mypy_cache/3.11/numbers.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.11/numbers.meta.json` & `typedal-1.1.1/.mypy_cache/3.11/numbers.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.11/pathlib.data.json` & `typedal-1.1.1/.mypy_cache/3.11/pathlib.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.11/pathlib.meta.json` & `typedal-1.1.1/.mypy_cache/3.11/pathlib.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.11/pickle.data.json` & `typedal-1.1.1/.mypy_cache/3.11/pickle.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.11/pickle.meta.json` & `typedal-1.1.1/.mypy_cache/3.11/pickle.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.11/posixpath.data.json` & `typedal-1.1.1/.mypy_cache/3.11/posixpath.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.11/posixpath.meta.json` & `typedal-1.1.1/.mypy_cache/3.11/posixpath.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.11/re.data.json` & `typedal-1.1.1/.mypy_cache/3.11/re.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.11/re.meta.json` & `typedal-1.1.1/.mypy_cache/3.11/re.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.11/sre_compile.data.json` & `typedal-1.1.1/.mypy_cache/3.11/sre_compile.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.11/sre_compile.meta.json` & `typedal-1.1.1/.mypy_cache/3.11/sre_compile.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.11/sre_constants.data.json` & `typedal-1.1.1/.mypy_cache/3.11/sre_constants.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.11/sre_constants.meta.json` & `typedal-1.1.1/.mypy_cache/3.11/sre_constants.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.11/sre_parse.data.json` & `typedal-1.1.1/.mypy_cache/3.11/sre_parse.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.11/sre_parse.meta.json` & `typedal-1.1.1/.mypy_cache/3.11/sre_parse.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.11/subprocess.data.json` & `typedal-1.1.1/.mypy_cache/3.11/subprocess.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.11/subprocess.meta.json` & `typedal-1.1.1/.mypy_cache/3.11/subprocess.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.11/sys.data.json` & `typedal-1.1.1/.mypy_cache/3.11/sys.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.11/sys.meta.json` & `typedal-1.1.1/.mypy_cache/3.11/sys.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.11/time.data.json` & `typedal-1.1.1/.mypy_cache/3.11/time.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.11/time.meta.json` & `typedal-1.1.1/.mypy_cache/3.11/time.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.11/types.data.json` & `typedal-1.1.1/.mypy_cache/3.11/types.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.11/types.meta.json` & `typedal-1.1.1/.mypy_cache/3.11/types.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.11/typing.data.json` & `typedal-1.1.1/.mypy_cache/3.11/typing.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.11/typing.meta.json` & `typedal-1.1.1/.mypy_cache/3.11/typing.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.11/typing_extensions.data.json` & `typedal-1.1.1/.mypy_cache/3.11/typing_extensions.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.11/typing_extensions.meta.json` & `typedal-1.1.1/.mypy_cache/3.11/typing_extensions.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.11/_typeshed/__init__.data.json` & `typedal-1.1.1/.mypy_cache/3.11/_typeshed/__init__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.11/_typeshed/__init__.meta.json` & `typedal-1.1.1/.mypy_cache/3.11/_typeshed/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.11/collections/__init__.data.json` & `typedal-1.1.1/.mypy_cache/3.11/collections/__init__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.11/collections/__init__.meta.json` & `typedal-1.1.1/.mypy_cache/3.11/collections/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.11/collections/abc.data.json` & `typedal-1.1.1/.mypy_cache/3.11/collections/abc.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.11/collections/abc.meta.json` & `typedal-1.1.1/.mypy_cache/3.11/collections/abc.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.11/ctypes/__init__.data.json` & `typedal-1.1.1/.mypy_cache/3.11/ctypes/__init__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.11/ctypes/__init__.meta.json` & `typedal-1.1.1/.mypy_cache/3.11/ctypes/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.11/email/__init__.data.json` & `typedal-1.1.1/.mypy_cache/3.11/email/__init__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.11/email/__init__.meta.json` & `typedal-1.1.1/.mypy_cache/3.11/email/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.11/email/charset.data.json` & `typedal-1.1.1/.mypy_cache/3.11/email/charset.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.11/email/charset.meta.json` & `typedal-1.1.1/.mypy_cache/3.11/email/charset.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.11/email/contentmanager.data.json` & `typedal-1.1.1/.mypy_cache/3.11/email/contentmanager.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.11/email/contentmanager.meta.json` & `typedal-1.1.1/.mypy_cache/3.11/email/contentmanager.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.11/email/errors.data.json` & `typedal-1.1.1/.mypy_cache/3.11/email/errors.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.11/email/errors.meta.json` & `typedal-1.1.1/.mypy_cache/3.11/email/errors.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.11/email/header.data.json` & `typedal-1.1.1/.mypy_cache/3.11/email/header.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.11/email/header.meta.json` & `typedal-1.1.1/.mypy_cache/3.11/email/header.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.11/email/message.data.json` & `typedal-1.1.1/.mypy_cache/3.11/email/message.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.11/email/message.meta.json` & `typedal-1.1.1/.mypy_cache/3.11/email/message.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.11/email/policy.data.json` & `typedal-1.1.1/.mypy_cache/3.11/email/policy.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.11/email/policy.meta.json` & `typedal-1.1.1/.mypy_cache/3.11/email/policy.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.11/importlib/__init__.data.json` & `typedal-1.1.1/.mypy_cache/3.11/importlib/__init__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.11/importlib/__init__.meta.json` & `typedal-1.1.1/.mypy_cache/3.11/importlib/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.11/importlib/abc.data.json` & `typedal-1.1.1/.mypy_cache/3.11/importlib/abc.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.11/importlib/abc.meta.json` & `typedal-1.1.1/.mypy_cache/3.11/importlib/abc.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.11/importlib/machinery.data.json` & `typedal-1.1.1/.mypy_cache/3.11/importlib/machinery.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.11/importlib/machinery.meta.json` & `typedal-1.1.1/.mypy_cache/3.11/importlib/machinery.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.11/importlib/metadata/__init__.data.json` & `typedal-1.1.1/.mypy_cache/3.11/importlib/metadata/__init__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.11/importlib/metadata/__init__.meta.json` & `typedal-1.1.1/.mypy_cache/3.11/importlib/metadata/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.11/importlib/metadata/_meta.data.json` & `typedal-1.1.1/.mypy_cache/3.11/importlib/metadata/_meta.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.11/importlib/metadata/_meta.meta.json` & `typedal-1.1.1/.mypy_cache/3.11/importlib/metadata/_meta.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.11/os/__init__.data.json` & `typedal-1.1.1/.mypy_cache/3.11/os/__init__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.11/os/__init__.meta.json` & `typedal-1.1.1/.mypy_cache/3.11/os/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.11/os/path.data.json` & `typedal-1.1.1/.mypy_cache/3.11/os/path.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.11/os/path.meta.json` & `typedal-1.1.1/.mypy_cache/3.11/os/path.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.11/src/__init__.data.json` & `typedal-1.1.1/.mypy_cache/3.11/src/__init__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.11/src/__init__.meta.json` & `typedal-1.1.1/.mypy_cache/3.11/src/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.11/src/typedal/__about__.data.json` & `typedal-1.1.1/.mypy_cache/3.11/src/typedal/__about__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.11/src/typedal/__about__.meta.json` & `typedal-1.1.1/.mypy_cache/3.11/src/typedal/__about__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.11/src/typedal/__init__.data.json` & `typedal-1.1.1/.mypy_cache/3.11/src/typedal/__init__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.11/src/typedal/__init__.meta.json` & `typedal-1.1.1/.mypy_cache/3.11/src/typedal/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.11/src/typedal/core.data.json` & `typedal-1.1.1/.mypy_cache/3.11/src/typedal/core.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.11/src/typedal/core.meta.json` & `typedal-1.1.1/.mypy_cache/3.11/src/typedal/core.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.11/src/typedal/fields.data.json` & `typedal-1.1.1/.mypy_cache/3.11/src/typedal/fields.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.11/src/typedal/fields.meta.json` & `typedal-1.1.1/.mypy_cache/3.11/src/typedal/fields.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.11/typedal/__about__.data.json` & `typedal-1.1.1/.mypy_cache/3.11/typedal/__about__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.mypy_cache/3.11/typedal/__about__.meta.json` & `typedal-1.1.1/.mypy_cache/3.11/typedal/__init__.meta.json`

 * *Files 11% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7266666666666667%*

 * *Differences: {"'data_mtime'": '1687423582',*

 * * "'dep_lines'": '{insert: [(0, 5), (1, 6)]}',*

 * * "'dep_prios'": '{insert: [(0, 5), (1, 5)]}',*

 * * "'dependencies'": "{insert: [(0, 'typedal.fields'), (1, 'typedal.core')]}",*

 * * "'hash'": "'86d37918830825d489c752ba036279764d920eb61960613df7edd1ea97ababeb'",*

 * * "'id'": "'typedal'",*

 * * "'interface_hash'": "'02445b61c73d58f2edb445e4d531ec93da432ca9e7dd8ca09bbc5336f30bdf07'",*

 * * "'mtime'": '1687423586',*

 * * "'path'": "'src/typedal/__init__.py'",*

 * * "'size'": '201'}*

```diff
@@ -1,29 +1,35 @@
 {
-    "data_mtime": 1685969397,
+    "data_mtime": 1687423582,
     "dep_lines": [
+        5,
+        6,
         1,
         1,
         1
     ],
     "dep_prios": [
         5,
+        5,
+        5,
         30,
         30
     ],
     "dependencies": [
+        "typedal.fields",
+        "typedal.core",
         "builtins",
         "abc",
         "typing"
     ],
-    "hash": "2af4074b9a9486e6b48127009cb4285ac1f424fe7169502c1572b6168127714f",
-    "id": "typedal.__about__",
+    "hash": "86d37918830825d489c752ba036279764d920eb61960613df7edd1ea97ababeb",
+    "id": "typedal",
     "ignore_all": false,
-    "interface_hash": "78ab11aa8e8cfd1f5fac091f83a1f2c46aac46f2e8973053a728baf5854e8af9",
-    "mtime": 1685520605,
+    "interface_hash": "02445b61c73d58f2edb445e4d531ec93da432ca9e7dd8ca09bbc5336f30bdf07",
+    "mtime": 1687423586,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
@@ -57,13 +63,13 @@
         "strict_equality": true,
         "strict_optional": true,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "src/typedal/__about__.py",
+    "path": "src/typedal/__init__.py",
     "plugin_data": null,
-    "size": 206,
+    "size": 201,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `typedal-1.0.0b1/.mypy_cache/3.11/typedal/__init__.data.json` & `typedal-1.1.1/.mypy_cache/3.11/typedal/__init__.data.json`

 * *Files 20% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9853021978021977%*

 * *Differences: {"'names'": "{'TypeDAL': {delete: ['module_hidden', 'module_public']}, 'TypedField': {delete: "*

 * *            "['module_hidden', 'module_public']}, 'TypedRows': {delete: ['module_hidden', "*

 * *            "'module_public']}, 'TypedTable': {delete: ['module_hidden', 'module_public']}, "*

 * *            "'__annotations__': {'module_public': False}, '__doc__': {'module_public': False}, "*

 * *            "'__file__': {'module_public': False}, '__name__': {'module_public': False}, "*

 * *            "'__package__': {'module_publi […]*

```diff
@@ -5,42 +5,56 @@
     "is_partial_stub_package": false,
     "is_stub": false,
     "names": {
         ".class": "SymbolTable",
         "TypeDAL": {
             ".class": "SymbolTableNode",
             "cross_ref": "typedal.core.TypeDAL",
-            "kind": "Gdef",
-            "module_hidden": true,
-            "module_public": false
+            "kind": "Gdef"
         },
         "TypedField": {
             ".class": "SymbolTableNode",
             "cross_ref": "typedal.fields.TypedField",
-            "kind": "Gdef",
-            "module_hidden": true,
-            "module_public": false
+            "kind": "Gdef"
         },
         "TypedRows": {
             ".class": "SymbolTableNode",
             "cross_ref": "typedal.core.TypedRows",
-            "kind": "Gdef",
-            "module_hidden": true,
-            "module_public": false
+            "kind": "Gdef"
         },
         "TypedTable": {
             ".class": "SymbolTableNode",
             "cross_ref": "typedal.core.TypedTable",
+            "kind": "Gdef"
+        },
+        "__all__": {
+            ".class": "SymbolTableNode",
             "kind": "Gdef",
-            "module_hidden": true,
-            "module_public": false
+            "module_public": false,
+            "node": {
+                ".class": "Var",
+                "flags": [
+                    "is_inferred",
+                    "has_explicit_value"
+                ],
+                "fullname": "typedal.__all__",
+                "name": "__all__",
+                "type": {
+                    ".class": "Instance",
+                    "args": [
+                        "builtins.str"
+                    ],
+                    "type_ref": "builtins.list"
+                }
+            }
         },
         "__annotations__": {
             ".class": "SymbolTableNode",
             "kind": "Gdef",
+            "module_public": false,
             "node": {
                 ".class": "Var",
                 "flags": [
                     "is_ready"
                 ],
                 "fullname": "typedal.__annotations__",
                 "name": "__annotations__",
@@ -58,66 +72,71 @@
                     "type_ref": "builtins.dict"
                 }
             }
         },
         "__doc__": {
             ".class": "SymbolTableNode",
             "kind": "Gdef",
+            "module_public": false,
             "node": {
                 ".class": "Var",
                 "flags": [
                     "is_ready"
                 ],
                 "fullname": "typedal.__doc__",
                 "name": "__doc__",
                 "type": "builtins.str"
             }
         },
         "__file__": {
             ".class": "SymbolTableNode",
             "kind": "Gdef",
+            "module_public": false,
             "node": {
                 ".class": "Var",
                 "flags": [
                     "is_ready"
                 ],
                 "fullname": "typedal.__file__",
                 "name": "__file__",
                 "type": "builtins.str"
             }
         },
         "__name__": {
             ".class": "SymbolTableNode",
             "kind": "Gdef",
+            "module_public": false,
             "node": {
                 ".class": "Var",
                 "flags": [
                     "is_ready"
                 ],
                 "fullname": "typedal.__name__",
                 "name": "__name__",
                 "type": "builtins.str"
             }
         },
         "__package__": {
             ".class": "SymbolTableNode",
             "kind": "Gdef",
+            "module_public": false,
             "node": {
                 ".class": "Var",
                 "flags": [
                     "is_ready"
                 ],
                 "fullname": "typedal.__package__",
                 "name": "__package__",
                 "type": "builtins.str"
             }
         },
         "__path__": {
             ".class": "SymbolTableNode",
             "kind": "Gdef",
+            "module_public": false,
             "node": {
                 ".class": "Var",
                 "flags": [
                     "is_ready"
                 ],
                 "fullname": "typedal.__path__",
                 "name": "__path__",
@@ -129,13 +148,12 @@
                     "type_ref": "builtins.list"
                 }
             }
         },
         "fields": {
             ".class": "SymbolTableNode",
             "cross_ref": "typedal.fields",
-            "kind": "Gdef",
-            "module_public": false
+            "kind": "Gdef"
         }
     },
     "path": "src/typedal/__init__.py"
 }
```

### Comparing `typedal-1.0.0b1/.mypy_cache/3.11/typedal/__init__.meta.json` & `typedal-1.1.1/.mypy_cache/3.11/typedal/__about__.meta.json`

 * *Files 13% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7266666666666667%*

 * *Differences: {"'data_mtime'": '1685969397',*

 * * "'dep_lines'": '{delete: [1, 0]}',*

 * * "'dep_prios'": '{delete: [1, 0]}',*

 * * "'dependencies'": '{delete: [1, 0]}',*

 * * "'hash'": "'e0acd1b21f59a6b1680357b204242b74a82e167f6fd415247029e7d3df241873'",*

 * * "'id'": "'typedal.__about__'",*

 * * "'interface_hash'": "'78ab11aa8e8cfd1f5fac091f83a1f2c46aac46f2e8973053a728baf5854e8af9'",*

 * * "'mtime'": '1687423439',*

 * * "'path'": "'src/typedal/__about__.py'",*

 * * "'size'": '206'}*

```diff
@@ -1,35 +1,29 @@
 {
-    "data_mtime": 1685974094,
+    "data_mtime": 1685969397,
     "dep_lines": [
-        5,
-        6,
         1,
         1,
         1
     ],
     "dep_prios": [
         5,
-        5,
-        5,
         30,
         30
     ],
     "dependencies": [
-        "typedal.fields",
-        "typedal.core",
         "builtins",
         "abc",
         "typing"
     ],
-    "hash": "335b93fb2ee3e31d3b0aa68072850cc80c542a1c3b27d992b8d6eab75415c695",
-    "id": "typedal",
+    "hash": "e0acd1b21f59a6b1680357b204242b74a82e167f6fd415247029e7d3df241873",
+    "id": "typedal.__about__",
     "ignore_all": false,
-    "interface_hash": "04a5d5560ecfe285738056027ab0a861a766011f0c3a6dba66f5b6f9df7be866",
-    "mtime": 1685968488,
+    "interface_hash": "78ab11aa8e8cfd1f5fac091f83a1f2c46aac46f2e8973053a728baf5854e8af9",
+    "mtime": 1687423439,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
@@ -63,13 +57,13 @@
         "strict_equality": true,
         "strict_optional": true,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "src/typedal/__init__.py",
+    "path": "src/typedal/__about__.py",
     "plugin_data": null,
-    "size": 349,
+    "size": 206,
     "suppressed": [],
     "version_id": "1.3.0"
 }
```

### Comparing `typedal-1.0.0b1/.mypy_cache/3.11/typedal/core.data.json` & `typedal-1.1.1/.mypy_cache/3.11/typedal/core.data.json`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.993495217358503%*

 * *Differences: {"'names'": "{'TypeDAL': {'node': {'names': {'default_kwargs': {'node': {'flags': {insert: [(1, "*

 * *            "'is_classvar'), (2, 'is_ready')], delete: [1]}, 'type': {'args': {insert: [(1, "*

 * *            "OrderedDict([('.class', 'AnyType'), ('missing_import_name', None), ('source_any', "*

 * *            "None), ('type_of_any', 2)]))], delete: [1]}}}}}}}, 'TypedRow': {'node': {'line': "*

 * *            "325}}, 'ChainMap': OrderedDict([('.class', 'SymbolTableNode'), ('cross_ref', "*

 * *            "'collections.ChainMap' […]*

```diff
@@ -117,14 +117,21 @@
                         },
                         "builtins.str"
                     ],
                     "type_ref": "builtins.dict"
                 }
             }
         },
+        "ChainMap": {
+            ".class": "SymbolTableNode",
+            "cross_ref": "collections.ChainMap",
+            "kind": "Gdef",
+            "module_hidden": true,
+            "module_public": false
+        },
         "Decimal": {
             ".class": "SymbolTableNode",
             "cross_ref": "_decimal.Decimal",
             "kind": "Gdef",
             "module_hidden": true,
             "module_public": false
         },
@@ -942,24 +949,30 @@
                     "default_kwargs": {
                         ".class": "SymbolTableNode",
                         "kind": "Mdef",
                         "node": {
                             ".class": "Var",
                             "flags": [
                                 "is_initialized_in_class",
-                                "is_inferred",
+                                "is_classvar",
+                                "is_ready",
                                 "has_explicit_value"
                             ],
                             "fullname": "typedal.core.TypeDAL.default_kwargs",
                             "name": "default_kwargs",
                             "type": {
                                 ".class": "Instance",
                                 "args": [
                                     "builtins.str",
-                                    "builtins.bool"
+                                    {
+                                        ".class": "AnyType",
+                                        "missing_import_name": null,
+                                        "source_any": null,
+                                        "type_of_any": 2
+                                    }
                                 ],
                                 "type_ref": "builtins.dict"
                             }
                         }
                     },
                     "define": {
                         ".class": "SymbolTableNode",
@@ -1387,15 +1400,15 @@
             ".class": "SymbolTableNode",
             "kind": "Gdef",
             "node": {
                 ".class": "TypeAlias",
                 "alias_tvars": [],
                 "column": 0,
                 "fullname": "typedal.core.TypedRow",
-                "line": 298,
+                "line": 325,
                 "no_args": true,
                 "normalized": false,
                 "target": "typedal.core.TypedTable"
             }
         },
         "TypedRows": {
             ".class": "SymbolTableNode",
@@ -2237,14 +2250,133 @@
                     "is_ready"
                 ],
                 "fullname": "typedal.core.__package__",
                 "name": "__package__",
                 "type": "builtins.str"
             }
         },
+        "_all_annotations": {
+            ".class": "SymbolTableNode",
+            "kind": "Gdef",
+            "node": {
+                ".class": "FuncDef",
+                "abstract_status": 0,
+                "arg_kinds": [
+                    0
+                ],
+                "arg_names": [
+                    "cls"
+                ],
+                "dataclass_transform_spec": null,
+                "flags": [],
+                "fullname": "typedal.core._all_annotations",
+                "name": "_all_annotations",
+                "type": {
+                    ".class": "CallableType",
+                    "arg_kinds": [
+                        0
+                    ],
+                    "arg_names": [
+                        "cls"
+                    ],
+                    "arg_types": [
+                        "builtins.type"
+                    ],
+                    "bound_args": [],
+                    "def_extras": {
+                        "first_arg": null
+                    },
+                    "fallback": "builtins.function",
+                    "from_concatenate": false,
+                    "implicit": false,
+                    "is_ellipsis_args": false,
+                    "name": "_all_annotations",
+                    "ret_type": {
+                        ".class": "Instance",
+                        "args": [
+                            "builtins.str",
+                            "builtins.type"
+                        ],
+                        "type_ref": "collections.ChainMap"
+                    },
+                    "type_guard": null,
+                    "unpack_kwargs": false,
+                    "variables": []
+                }
+            }
+        },
+        "all_annotations": {
+            ".class": "SymbolTableNode",
+            "kind": "Gdef",
+            "node": {
+                ".class": "FuncDef",
+                "abstract_status": 0,
+                "arg_kinds": [
+                    0,
+                    1
+                ],
+                "arg_names": [
+                    "cls",
+                    "_except"
+                ],
+                "dataclass_transform_spec": null,
+                "flags": [],
+                "fullname": "typedal.core.all_annotations",
+                "name": "all_annotations",
+                "type": {
+                    ".class": "CallableType",
+                    "arg_kinds": [
+                        0,
+                        1
+                    ],
+                    "arg_names": [
+                        "cls",
+                        "_except"
+                    ],
+                    "arg_types": [
+                        "builtins.type",
+                        {
+                            ".class": "UnionType",
+                            "items": [
+                                {
+                                    ".class": "Instance",
+                                    "args": [
+                                        "builtins.str"
+                                    ],
+                                    "type_ref": "typing.Iterable"
+                                },
+                                {
+                                    ".class": "NoneType"
+                                }
+                            ]
+                        }
+                    ],
+                    "bound_args": [],
+                    "def_extras": {
+                        "first_arg": null
+                    },
+                    "fallback": "builtins.function",
+                    "from_concatenate": false,
+                    "implicit": false,
+                    "is_ellipsis_args": false,
+                    "name": "all_annotations",
+                    "ret_type": {
+                        ".class": "Instance",
+                        "args": [
+                            "builtins.str",
+                            "builtins.type"
+                        ],
+                        "type_ref": "builtins.dict"
+                    },
+                    "type_guard": null,
+                    "unpack_kwargs": false,
+                    "variables": []
+                }
+            }
+        },
         "dt": {
             ".class": "SymbolTableNode",
             "cross_ref": "datetime",
             "kind": "Gdef",
             "module_hidden": true,
             "module_public": false
         },
```

### Comparing `typedal-1.0.0b1/.mypy_cache/3.11/typedal/core.meta.json` & `typedal-1.1.1/.mypy_cache/3.11/typedal/fields.meta.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.726525054466231%*

 * *Differences: {"'data_mtime'": '1687422111',*

 * * "'dep_lines'": '{insert: [(0, 12)], delete: [14, 4]}',*

 * * "'dep_prios'": '{insert: [(0, 5), (4, 10)], delete: [15, 5, 3]}',*

 * * "'dependencies'": "{insert: [(0, 'typedal.core'), (2, 'decimal')], delete: [5, 3]}",*

 * * "'hash'": "'2da5da10836f40ec000f32c64446f28df3e5081a9e14d5473684770659627369'",*

 * * "'id'": "'typedal.fields'",*

 * * "'interface_hash'": "'7f52734fa267868275c2d07b23b14504cf86d84ca8ba75738eacb85b5ff41a00'",*

 * * "'mtime'": '1687423422',*

 * * "'path'": "'src/typedal/fields.py'",*

 * * "'size […]*

```diff
@@ -1,66 +1,64 @@
 {
-    "data_mtime": 1685974138,
+    "data_mtime": 1687422111,
     "dep_lines": [
+        12,
         5,
         6,
         7,
         8,
         1,
         1,
         1,
         1,
         1,
         1,
         1,
         1,
         1,
-        1,
-        11,
         10
     ],
     "dep_prios": [
+        5,
+        10,
         10,
         10,
         10,
         5,
-        5,
-        30,
         30,
         30,
         30,
         30,
         30,
         30,
         30,
         30,
-        5,
-        10
+        5
     ],
     "dependencies": [
+        "typedal.core",
         "datetime",
+        "decimal",
         "types",
         "typing",
-        "decimal",
         "builtins",
-        "_collections_abc",
         "_decimal",
         "_typeshed",
         "abc",
         "array",
         "ctypes",
         "mmap",
         "pickle",
         "typing_extensions"
     ],
-    "hash": "2bd5facb89d34de87665254d3124e5a9d82c4f0723b66ce2d084ecc835d98a5a",
-    "id": "typedal.core",
+    "hash": "2da5da10836f40ec000f32c64446f28df3e5081a9e14d5473684770659627369",
+    "id": "typedal.fields",
     "ignore_all": false,
-    "interface_hash": "3dbffd2d74a964acee246524a1244638abf60e50848c38a1ed84835a24a46009",
-    "mtime": 1685974225,
+    "interface_hash": "7f52734fa267868275c2d07b23b14504cf86d84ca8ba75738eacb85b5ff41a00",
+    "mtime": 1687423422,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
@@ -94,16 +92,15 @@
         "strict_equality": true,
         "strict_optional": true,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "src/typedal/core.py",
+    "path": "src/typedal/fields.py",
     "plugin_data": null,
-    "size": 12033,
+    "size": 4949,
     "suppressed": [
-        "pydal.objects",
-        "pydal"
+        "pydal.objects"
     ],
     "version_id": "1.3.0"
 }
```

### Comparing `typedal-1.0.0b1/.mypy_cache/3.11/typedal/fields.data.json` & `typedal-1.1.1/.mypy_cache/3.11/typedal/fields.data.json`

 * *Files 16% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9960866358971104%*

 * *Differences: {"'names'": "{'Bigint': {'node': {'type': {'ret_type': 'builtins.int'}}}, 'BigintField': {'node': "*

 * *            "{'type': {'ret_type': 'builtins.int'}}}, 'Blob': {'node': {'type': {'ret_type': "*

 * *            "'builtins.bytes'}}}, 'BlobField': {'node': {'type': {'ret_type': 'builtins.bytes'}}}, "*

 * *            "'Boolean': {'node': {'type': {'ret_type': 'builtins.bool'}}}, 'BooleanField': "*

 * *            "{'node': {'type': {'ret_type': 'builtins.bool'}}}, 'Date': {'node': {'type': "*

 * *            "{'ret_type': 'date […]*

```diff
@@ -38,19 +38,15 @@
                         "first_arg": null
                     },
                     "fallback": "builtins.function",
                     "from_concatenate": false,
                     "implicit": false,
                     "is_ellipsis_args": false,
                     "name": null,
-                    "ret_type": {
-                        ".class": "TypeAliasType",
-                        "args": [],
-                        "type_ref": "typedal.fields.TYPE_INT"
-                    },
+                    "ret_type": "builtins.int",
                     "type_guard": null,
                     "unpack_kwargs": false,
                     "variables": []
                 }
             }
         },
         "BigintField": {
@@ -90,19 +86,15 @@
                         "first_arg": null
                     },
                     "fallback": "builtins.function",
                     "from_concatenate": false,
                     "implicit": false,
                     "is_ellipsis_args": false,
                     "name": "BigintField",
-                    "ret_type": {
-                        ".class": "TypeAliasType",
-                        "args": [],
-                        "type_ref": "typedal.fields.TYPE_INT"
-                    },
+                    "ret_type": "builtins.int",
                     "type_guard": null,
                     "unpack_kwargs": false,
                     "variables": []
                 }
             }
         },
         "Blob": {
@@ -137,18 +129,15 @@
                         "first_arg": null
                     },
                     "fallback": "builtins.function",
                     "from_concatenate": false,
                     "implicit": false,
                     "is_ellipsis_args": false,
                     "name": null,
-                    "ret_type": {
-                        ".class": "TypeType",
-                        "item": "builtins.bytes"
-                    },
+                    "ret_type": "builtins.bytes",
                     "type_guard": null,
                     "unpack_kwargs": false,
                     "variables": []
                 }
             }
         },
         "BlobField": {
@@ -188,18 +177,15 @@
                         "first_arg": null
                     },
                     "fallback": "builtins.function",
                     "from_concatenate": false,
                     "implicit": false,
                     "is_ellipsis_args": false,
                     "name": "BlobField",
-                    "ret_type": {
-                        ".class": "TypeType",
-                        "item": "builtins.bytes"
-                    },
+                    "ret_type": "builtins.bytes",
                     "type_guard": null,
                     "unpack_kwargs": false,
                     "variables": []
                 }
             }
         },
         "Boolean": {
@@ -234,18 +220,15 @@
                         "first_arg": null
                     },
                     "fallback": "builtins.function",
                     "from_concatenate": false,
                     "implicit": false,
                     "is_ellipsis_args": false,
                     "name": null,
-                    "ret_type": {
-                        ".class": "TypeType",
-                        "item": "builtins.bool"
-                    },
+                    "ret_type": "builtins.bool",
                     "type_guard": null,
                     "unpack_kwargs": false,
                     "variables": []
                 }
             }
         },
         "BooleanField": {
@@ -285,18 +268,15 @@
                         "first_arg": null
                     },
                     "fallback": "builtins.function",
                     "from_concatenate": false,
                     "implicit": false,
                     "is_ellipsis_args": false,
                     "name": "BooleanField",
-                    "ret_type": {
-                        ".class": "TypeType",
-                        "item": "builtins.bool"
-                    },
+                    "ret_type": "builtins.bool",
                     "type_guard": null,
                     "unpack_kwargs": false,
                     "variables": []
                 }
             }
         },
         "Date": {
@@ -331,18 +311,15 @@
                         "first_arg": null
                     },
                     "fallback": "builtins.function",
                     "from_concatenate": false,
                     "implicit": false,
                     "is_ellipsis_args": false,
                     "name": null,
-                    "ret_type": {
-                        ".class": "TypeType",
-                        "item": "datetime.date"
-                    },
+                    "ret_type": "datetime.date",
                     "type_guard": null,
                     "unpack_kwargs": false,
                     "variables": []
                 }
             }
         },
         "DateField": {
@@ -382,18 +359,15 @@
                         "first_arg": null
                     },
                     "fallback": "builtins.function",
                     "from_concatenate": false,
                     "implicit": false,
                     "is_ellipsis_args": false,
                     "name": "DateField",
-                    "ret_type": {
-                        ".class": "TypeType",
-                        "item": "datetime.date"
-                    },
+                    "ret_type": "datetime.date",
                     "type_guard": null,
                     "unpack_kwargs": false,
                     "variables": []
                 }
             }
         },
         "Datetime": {
@@ -428,18 +402,15 @@
                         "first_arg": null
                     },
                     "fallback": "builtins.function",
                     "from_concatenate": false,
                     "implicit": false,
                     "is_ellipsis_args": false,
                     "name": null,
-                    "ret_type": {
-                        ".class": "TypeType",
-                        "item": "datetime.datetime"
-                    },
+                    "ret_type": "datetime.datetime",
                     "type_guard": null,
                     "unpack_kwargs": false,
                     "variables": []
                 }
             }
         },
         "DatetimeField": {
@@ -479,18 +450,15 @@
                         "first_arg": null
                     },
                     "fallback": "builtins.function",
                     "from_concatenate": false,
                     "implicit": false,
                     "is_ellipsis_args": false,
                     "name": "DatetimeField",
-                    "ret_type": {
-                        ".class": "TypeType",
-                        "item": "datetime.datetime"
-                    },
+                    "ret_type": "datetime.datetime",
                     "type_guard": null,
                     "unpack_kwargs": false,
                     "variables": []
                 }
             }
         },
         "Decimal": {
@@ -531,18 +499,15 @@
                         "first_arg": null
                     },
                     "fallback": "builtins.function",
                     "from_concatenate": false,
                     "implicit": false,
                     "is_ellipsis_args": false,
                     "name": null,
-                    "ret_type": {
-                        ".class": "TypeType",
-                        "item": "_decimal.Decimal"
-                    },
+                    "ret_type": "_decimal.Decimal",
                     "type_guard": null,
                     "unpack_kwargs": false,
                     "variables": []
                 }
             }
         },
         "DecimalField": {
@@ -592,18 +557,15 @@
                         "first_arg": null
                     },
                     "fallback": "builtins.function",
                     "from_concatenate": false,
                     "implicit": false,
                     "is_ellipsis_args": false,
                     "name": "DecimalField",
-                    "ret_type": {
-                        ".class": "TypeType",
-                        "item": "_decimal.Decimal"
-                    },
+                    "ret_type": "_decimal.Decimal",
                     "type_guard": null,
                     "unpack_kwargs": false,
                     "variables": []
                 }
             }
         },
         "Double": {
@@ -638,18 +600,15 @@
                         "first_arg": null
                     },
                     "fallback": "builtins.function",
                     "from_concatenate": false,
                     "implicit": false,
                     "is_ellipsis_args": false,
                     "name": null,
-                    "ret_type": {
-                        ".class": "TypeType",
-                        "item": "builtins.float"
-                    },
+                    "ret_type": "builtins.float",
                     "type_guard": null,
                     "unpack_kwargs": false,
                     "variables": []
                 }
             }
         },
         "DoubleField": {
@@ -689,18 +648,15 @@
                         "first_arg": null
                     },
                     "fallback": "builtins.function",
                     "from_concatenate": false,
                     "implicit": false,
                     "is_ellipsis_args": false,
                     "name": "DoubleField",
-                    "ret_type": {
-                        ".class": "TypeType",
-                        "item": "builtins.float"
-                    },
+                    "ret_type": "builtins.float",
                     "type_guard": null,
                     "unpack_kwargs": false,
                     "variables": []
                 }
             }
         },
         "Integer": {
@@ -735,18 +691,15 @@
                         "first_arg": null
                     },
                     "fallback": "builtins.function",
                     "from_concatenate": false,
                     "implicit": false,
                     "is_ellipsis_args": false,
                     "name": null,
-                    "ret_type": {
-                        ".class": "TypeType",
-                        "item": "builtins.int"
-                    },
+                    "ret_type": "builtins.int",
                     "type_guard": null,
                     "unpack_kwargs": false,
                     "variables": []
                 }
             }
         },
         "IntegerField": {
@@ -786,18 +739,15 @@
                         "first_arg": null
                     },
                     "fallback": "builtins.function",
                     "from_concatenate": false,
                     "implicit": false,
                     "is_ellipsis_args": false,
                     "name": "IntegerField",
-                    "ret_type": {
-                        ".class": "TypeType",
-                        "item": "builtins.int"
-                    },
+                    "ret_type": "builtins.int",
                     "type_guard": null,
                     "unpack_kwargs": false,
                     "variables": []
                 }
             }
         },
         "JSONField": {
@@ -837,18 +787,15 @@
                         "first_arg": null
                     },
                     "fallback": "builtins.function",
                     "from_concatenate": false,
                     "implicit": false,
                     "is_ellipsis_args": false,
                     "name": "JSONField",
-                    "ret_type": {
-                        ".class": "TypeType",
-                        "item": "builtins.object"
-                    },
+                    "ret_type": "builtins.object",
                     "type_guard": null,
                     "unpack_kwargs": false,
                     "variables": []
                 }
             }
         },
         "ListInteger": {
@@ -884,17 +831,19 @@
                     },
                     "fallback": "builtins.function",
                     "from_concatenate": false,
                     "implicit": false,
                     "is_ellipsis_args": false,
                     "name": null,
                     "ret_type": {
-                        ".class": "TypeAliasType",
-                        "args": [],
-                        "type_ref": "typedal.fields.TYPE_LIST_OF_INT"
+                        ".class": "Instance",
+                        "args": [
+                            "builtins.int"
+                        ],
+                        "type_ref": "builtins.list"
                     },
                     "type_guard": null,
                     "unpack_kwargs": false,
                     "variables": []
                 }
             }
         },
@@ -936,17 +885,19 @@
                     },
                     "fallback": "builtins.function",
                     "from_concatenate": false,
                     "implicit": false,
                     "is_ellipsis_args": false,
                     "name": "ListIntegerField",
                     "ret_type": {
-                        ".class": "TypeAliasType",
-                        "args": [],
-                        "type_ref": "typedal.fields.TYPE_LIST_OF_INT"
+                        ".class": "Instance",
+                        "args": [
+                            "builtins.int"
+                        ],
+                        "type_ref": "builtins.list"
                     },
                     "type_guard": null,
                     "unpack_kwargs": false,
                     "variables": []
                 }
             }
         },
@@ -986,17 +937,19 @@
                     },
                     "fallback": "builtins.function",
                     "from_concatenate": false,
                     "implicit": false,
                     "is_ellipsis_args": false,
                     "name": null,
                     "ret_type": {
-                        ".class": "TypeAliasType",
-                        "args": [],
-                        "type_ref": "typedal.fields.TYPE_LIST_OF_INT"
+                        ".class": "Instance",
+                        "args": [
+                            "builtins.int"
+                        ],
+                        "type_ref": "builtins.list"
                     },
                     "type_guard": null,
                     "unpack_kwargs": false,
                     "variables": []
                 }
             }
         },
@@ -1043,17 +996,19 @@
                     },
                     "fallback": "builtins.function",
                     "from_concatenate": false,
                     "implicit": false,
                     "is_ellipsis_args": false,
                     "name": "ListReferenceField",
                     "ret_type": {
-                        ".class": "TypeAliasType",
-                        "args": [],
-                        "type_ref": "typedal.fields.TYPE_LIST_OF_INT"
+                        ".class": "Instance",
+                        "args": [
+                            "builtins.int"
+                        ],
+                        "type_ref": "builtins.list"
                     },
                     "type_guard": null,
                     "unpack_kwargs": false,
                     "variables": []
                 }
             }
         },
@@ -1090,22 +1045,19 @@
                     },
                     "fallback": "builtins.function",
                     "from_concatenate": false,
                     "implicit": false,
                     "is_ellipsis_args": false,
                     "name": null,
                     "ret_type": {
-                        ".class": "TypeType",
-                        "item": {
-                            ".class": "Instance",
-                            "args": [
-                                "builtins.str"
-                            ],
-                            "type_ref": "builtins.list"
-                        }
+                        ".class": "Instance",
+                        "args": [
+                            "builtins.str"
+                        ],
+                        "type_ref": "builtins.list"
                     },
                     "type_guard": null,
                     "unpack_kwargs": false,
                     "variables": []
                 }
             }
         },
@@ -1147,22 +1099,19 @@
                     },
                     "fallback": "builtins.function",
                     "from_concatenate": false,
                     "implicit": false,
                     "is_ellipsis_args": false,
                     "name": "ListStringField",
                     "ret_type": {
-                        ".class": "TypeType",
-                        "item": {
-                            ".class": "Instance",
-                            "args": [
-                                "builtins.str"
-                            ],
-                            "type_ref": "builtins.list"
-                        }
+                        ".class": "Instance",
+                        "args": [
+                            "builtins.str"
+                        ],
+                        "type_ref": "builtins.list"
                     },
                     "type_guard": null,
                     "unpack_kwargs": false,
                     "variables": []
                 }
             }
         },
@@ -1198,19 +1147,15 @@
                         "first_arg": null
                     },
                     "fallback": "builtins.function",
                     "from_concatenate": false,
                     "implicit": false,
                     "is_ellipsis_args": false,
                     "name": null,
-                    "ret_type": {
-                        ".class": "TypeAliasType",
-                        "args": [],
-                        "type_ref": "typedal.fields.TYPE_STR"
-                    },
+                    "ret_type": "builtins.str",
                     "type_guard": null,
                     "unpack_kwargs": false,
                     "variables": []
                 }
             }
         },
         "PasswordField": {
@@ -1250,19 +1195,15 @@
                         "first_arg": null
                     },
                     "fallback": "builtins.function",
                     "from_concatenate": false,
                     "implicit": false,
                     "is_ellipsis_args": false,
                     "name": "PasswordField",
-                    "ret_type": {
-                        ".class": "TypeAliasType",
-                        "args": [],
-                        "type_ref": "typedal.fields.TYPE_STR"
-                    },
+                    "ret_type": "builtins.str",
                     "type_guard": null,
                     "unpack_kwargs": false,
                     "variables": []
                 }
             }
         },
         "Reference": {
@@ -1330,19 +1271,15 @@
                         "first_arg": null
                     },
                     "fallback": "builtins.function",
                     "from_concatenate": false,
                     "implicit": false,
                     "is_ellipsis_args": false,
                     "name": null,
-                    "ret_type": {
-                        ".class": "TypeAliasType",
-                        "args": [],
-                        "type_ref": "typedal.fields.TYPE_INT"
-                    },
+                    "ret_type": "builtins.int",
                     "type_guard": null,
                     "unpack_kwargs": false,
                     "variables": [
                         {
                             ".class": "TypeVarType",
                             "fullname": "typedal.fields.T_subclass",
                             "id": -1,
@@ -1436,19 +1373,15 @@
                         "first_arg": null
                     },
                     "fallback": "builtins.function",
                     "from_concatenate": false,
                     "implicit": false,
                     "is_ellipsis_args": false,
                     "name": "ReferenceField",
-                    "ret_type": {
-                        ".class": "TypeAliasType",
-                        "args": [],
-                        "type_ref": "typedal.fields.TYPE_INT"
-                    },
+                    "ret_type": "builtins.int",
                     "type_guard": null,
                     "unpack_kwargs": false,
                     "variables": [
                         {
                             ".class": "TypeVarType",
                             "fullname": "typedal.fields.T_subclass",
                             "id": -1,
@@ -1502,19 +1435,15 @@
                         "first_arg": null
                     },
                     "fallback": "builtins.function",
                     "from_concatenate": false,
                     "implicit": false,
                     "is_ellipsis_args": false,
                     "name": null,
-                    "ret_type": {
-                        ".class": "TypeAliasType",
-                        "args": [],
-                        "type_ref": "typedal.fields.TYPE_STR"
-                    },
+                    "ret_type": "builtins.str",
                     "type_guard": null,
                     "unpack_kwargs": false,
                     "variables": []
                 }
             }
         },
         "StringField": {
@@ -1554,102 +1483,38 @@
                         "first_arg": null
                     },
                     "fallback": "builtins.function",
                     "from_concatenate": false,
                     "implicit": false,
                     "is_ellipsis_args": false,
                     "name": "StringField",
-                    "ret_type": {
-                        ".class": "TypeAliasType",
-                        "args": [],
-                        "type_ref": "typedal.fields.TYPE_STR"
-                    },
+                    "ret_type": "builtins.str",
                     "type_guard": null,
                     "unpack_kwargs": false,
                     "variables": []
                 }
             }
         },
         "T": {
             ".class": "SymbolTableNode",
             "kind": "Gdef",
             "node": {
                 ".class": "TypeVarExpr",
                 "fullname": "typedal.fields.T",
                 "name": "T",
                 "upper_bound": {
-                    ".class": "TypeType",
-                    "item": {
-                        ".class": "AnyType",
-                        "missing_import_name": null,
-                        "source_any": null,
-                        "type_of_any": 2
-                    }
+                    ".class": "AnyType",
+                    "missing_import_name": null,
+                    "source_any": null,
+                    "type_of_any": 2
                 },
                 "values": [],
                 "variance": 0
             }
         },
-        "TYPE_INT": {
-            ".class": "SymbolTableNode",
-            "kind": "Gdef",
-            "node": {
-                ".class": "TypeAlias",
-                "alias_tvars": [],
-                "column": 0,
-                "fullname": "typedal.fields.TYPE_INT",
-                "line": 36,
-                "no_args": false,
-                "normalized": false,
-                "target": {
-                    ".class": "TypeType",
-                    "item": "builtins.int"
-                }
-            }
-        },
-        "TYPE_LIST_OF_INT": {
-            ".class": "SymbolTableNode",
-            "kind": "Gdef",
-            "node": {
-                ".class": "TypeAlias",
-                "alias_tvars": [],
-                "column": 0,
-                "fullname": "typedal.fields.TYPE_LIST_OF_INT",
-                "line": 37,
-                "no_args": false,
-                "normalized": false,
-                "target": {
-                    ".class": "TypeType",
-                    "item": {
-                        ".class": "Instance",
-                        "args": [
-                            "builtins.int"
-                        ],
-                        "type_ref": "builtins.list"
-                    }
-                }
-            }
-        },
-        "TYPE_STR": {
-            ".class": "SymbolTableNode",
-            "kind": "Gdef",
-            "node": {
-                ".class": "TypeAlias",
-                "alias_tvars": [],
-                "column": 0,
-                "fullname": "typedal.fields.TYPE_STR",
-                "line": 35,
-                "no_args": false,
-                "normalized": false,
-                "target": {
-                    ".class": "TypeType",
-                    "item": "builtins.str"
-                }
-            }
-        },
         "T_subclass": {
             ".class": "SymbolTableNode",
             "kind": "Gdef",
             "node": {
                 ".class": "TypeVarExpr",
                 "fullname": "typedal.fields.T_subclass",
                 "name": "T_subclass",
@@ -1720,19 +1585,15 @@
                         "first_arg": null
                     },
                     "fallback": "builtins.function",
                     "from_concatenate": false,
                     "implicit": false,
                     "is_ellipsis_args": false,
                     "name": null,
-                    "ret_type": {
-                        ".class": "TypeAliasType",
-                        "args": [],
-                        "type_ref": "typedal.fields.TYPE_STR"
-                    },
+                    "ret_type": "builtins.str",
                     "type_guard": null,
                     "unpack_kwargs": false,
                     "variables": []
                 }
             }
         },
         "TextField": {
@@ -1772,19 +1633,15 @@
                         "first_arg": null
                     },
                     "fallback": "builtins.function",
                     "from_concatenate": false,
                     "implicit": false,
                     "is_ellipsis_args": false,
                     "name": "TextField",
-                    "ret_type": {
-                        ".class": "TypeAliasType",
-                        "args": [],
-                        "type_ref": "typedal.fields.TYPE_STR"
-                    },
+                    "ret_type": "builtins.str",
                     "type_guard": null,
                     "unpack_kwargs": false,
                     "variables": []
                 }
             }
         },
         "Time": {
@@ -1819,18 +1676,15 @@
                         "first_arg": null
                     },
                     "fallback": "builtins.function",
                     "from_concatenate": false,
                     "implicit": false,
                     "is_ellipsis_args": false,
                     "name": null,
-                    "ret_type": {
-                        ".class": "TypeType",
-                        "item": "datetime.time"
-                    },
+                    "ret_type": "datetime.time",
                     "type_guard": null,
                     "unpack_kwargs": false,
                     "variables": []
                 }
             }
         },
         "TimeField": {
@@ -1870,18 +1724,15 @@
                         "first_arg": null
                     },
                     "fallback": "builtins.function",
                     "from_concatenate": false,
                     "implicit": false,
                     "is_ellipsis_args": false,
                     "name": "TimeField",
-                    "ret_type": {
-                        ".class": "TypeType",
-                        "item": "datetime.time"
-                    },
+                    "ret_type": "datetime.time",
                     "type_guard": null,
                     "unpack_kwargs": false,
                     "variables": []
                 }
             }
         },
         "TypeDAL": {
@@ -1920,30 +1771,30 @@
                         "kwargs"
                     ],
                     "arg_types": [
                         {
                             ".class": "UnionType",
                             "items": [
                                 {
-                                    ".class": "TypeVarType",
-                                    "fullname": "typedal.fields.T",
-                                    "id": -1,
-                                    "name": "T",
-                                    "namespace": "",
-                                    "upper_bound": {
-                                        ".class": "TypeType",
-                                        "item": {
+                                    ".class": "TypeType",
+                                    "item": {
+                                        ".class": "TypeVarType",
+                                        "fullname": "typedal.fields.T",
+                                        "id": -1,
+                                        "name": "T",
+                                        "namespace": "",
+                                        "upper_bound": {
                                             ".class": "AnyType",
                                             "missing_import_name": null,
                                             "source_any": null,
                                             "type_of_any": 2
-                                        }
-                                    },
-                                    "values": [],
-                                    "variance": 0
+                                        },
+                                        "values": [],
+                                        "variance": 0
+                                    }
                                 },
                                 "types.UnionType"
                             ]
                         },
                         {
                             ".class": "AnyType",
                             "missing_import_name": null,
@@ -1963,42 +1814,36 @@
                     "ret_type": {
                         ".class": "TypeVarType",
                         "fullname": "typedal.fields.T",
                         "id": -1,
                         "name": "T",
                         "namespace": "",
                         "upper_bound": {
-                            ".class": "TypeType",
-                            "item": {
-                                ".class": "AnyType",
-                                "missing_import_name": null,
-                                "source_any": null,
-                                "type_of_any": 2
-                            }
+                            ".class": "AnyType",
+                            "missing_import_name": null,
+                            "source_any": null,
+                            "type_of_any": 2
                         },
                         "values": [],
                         "variance": 0
                     },
                     "type_guard": null,
                     "unpack_kwargs": false,
                     "variables": [
                         {
                             ".class": "TypeVarType",
                             "fullname": "typedal.fields.T",
                             "id": -1,
                             "name": "T",
                             "namespace": "",
                             "upper_bound": {
-                                ".class": "TypeType",
-                                "item": {
-                                    ".class": "AnyType",
-                                    "missing_import_name": null,
-                                    "source_any": null,
-                                    "type_of_any": 2
-                                }
+                                ".class": "AnyType",
+                                "missing_import_name": null,
+                                "source_any": null,
+                                "type_of_any": 2
                             },
                             "values": [],
                             "variance": 0
                         }
                     ]
                 }
             }
@@ -2049,19 +1894,15 @@
                         "first_arg": null
                     },
                     "fallback": "builtins.function",
                     "from_concatenate": false,
                     "implicit": false,
                     "is_ellipsis_args": false,
                     "name": null,
-                    "ret_type": {
-                        ".class": "TypeAliasType",
-                        "args": [],
-                        "type_ref": "typedal.fields.TYPE_STR"
-                    },
+                    "ret_type": "builtins.str",
                     "type_guard": null,
                     "unpack_kwargs": false,
                     "variables": []
                 }
             }
         },
         "UploadField": {
@@ -2101,19 +1942,15 @@
                         "first_arg": null
                     },
                     "fallback": "builtins.function",
                     "from_concatenate": false,
                     "implicit": false,
                     "is_ellipsis_args": false,
                     "name": "UploadField",
-                    "ret_type": {
-                        ".class": "TypeAliasType",
-                        "args": [],
-                        "type_ref": "typedal.fields.TYPE_STR"
-                    },
+                    "ret_type": "builtins.str",
                     "type_guard": null,
                     "unpack_kwargs": false,
                     "variables": []
                 }
             }
         },
         "__annotations__": {
```

### Comparing `typedal-1.0.0b1/.mypy_cache/3.11/typedal/fields.meta.json` & `typedal-1.1.1/.mypy_cache/3.11/typedal/core.meta.json`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7222623552344914%*

 * *Differences: {"'data_mtime'": '1687423394',*

 * * "'dep_lines'": '{insert: [(0, 4), (5, 1), (15, 11)], delete: [0]}',*

 * * "'dep_prios'": '{insert: [(3, 5), (4, 5), (6, 30), (16, 10)], delete: [1, 0]}',*

 * * "'dependencies'": "{insert: [(3, 'collections'), (4, 'decimal'), (6, '_collections_abc')], "*

 * *                   'delete: [2, 0]}',*

 * * "'hash'": "'f0b936192e73975a7f0b3a773944bc8023a2d010b2a7442ef5a409c70c64c9aa'",*

 * * "'id'": "'typedal.core'",*

 * * "'interface_hash'": "'076cc41a8a473e325374327fae7f7a67e34867a85651a5f79a450aa3c7dcdfa9'",*

 * * […]*

```diff
@@ -1,64 +1,69 @@
 {
-    "data_mtime": 1685974094,
+    "data_mtime": 1687423394,
     "dep_lines": [
-        12,
+        4,
         5,
         6,
         7,
         8,
         1,
         1,
         1,
         1,
         1,
         1,
         1,
         1,
         1,
+        1,
+        11,
         10
     ],
     "dep_prios": [
-        5,
-        10,
         10,
         10,
         10,
         5,
+        5,
+        5,
         30,
         30,
         30,
         30,
         30,
         30,
         30,
         30,
-        5
+        30,
+        5,
+        10
     ],
     "dependencies": [
-        "typedal.core",
         "datetime",
-        "decimal",
         "types",
         "typing",
+        "collections",
+        "decimal",
         "builtins",
+        "_collections_abc",
         "_decimal",
         "_typeshed",
         "abc",
         "array",
         "ctypes",
         "mmap",
         "pickle",
         "typing_extensions"
     ],
-    "hash": "c6ff107fa932b5526fc076f424574906267069c87fb6672f7eca05289614fdd1",
-    "id": "typedal.fields",
+    "hash": "f0b936192e73975a7f0b3a773944bc8023a2d010b2a7442ef5a409c70c64c9aa",
+    "id": "typedal.core",
     "ignore_all": false,
-    "interface_hash": "cc03aa226b2fd8b523b3eaf6a1618dad596fc43404c0e7b387a504583109c5f0",
-    "mtime": 1685973224,
+    "interface_hash": "076cc41a8a473e325374327fae7f7a67e34867a85651a5f79a450aa3c7dcdfa9",
+    "mtime": 1687423422,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
@@ -92,15 +97,16 @@
         "strict_equality": true,
         "strict_optional": true,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "src/typedal/fields.py",
+    "path": "src/typedal/core.py",
     "plugin_data": null,
-    "size": 5207,
+    "size": 13165,
     "suppressed": [
-        "pydal.objects"
+        "pydal.objects",
+        "pydal"
     ],
     "version_id": "1.3.0"
 }
```

### Comparing `typedal-1.0.0b1/.ruff_cache/content/1b34455c399f0006` & `typedal-1.1.1/.ruff_cache/content/1b34455c399f0006`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.ruff_cache/content/20585cf790eae81e` & `typedal-1.1.1/.ruff_cache/content/20585cf790eae81e`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.ruff_cache/content/221af82ae72a7f27` & `typedal-1.1.1/.ruff_cache/content/221af82ae72a7f27`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.ruff_cache/content/24e1b4aab386ebc8` & `typedal-1.1.1/.ruff_cache/content/24e1b4aab386ebc8`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.ruff_cache/content/2f3396c610fd7095` & `typedal-1.1.1/.ruff_cache/content/2f3396c610fd7095`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.ruff_cache/content/3826106cf4494de8` & `typedal-1.1.1/.ruff_cache/content/3826106cf4494de8`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.ruff_cache/content/38d5fd55b14a9d6c` & `typedal-1.1.1/.ruff_cache/content/38d5fd55b14a9d6c`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.ruff_cache/content/4022ee8774ccd98a` & `typedal-1.1.1/.ruff_cache/content/4022ee8774ccd98a`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.ruff_cache/content/75bd1769f6e29ed7` & `typedal-1.1.1/.ruff_cache/content/75bd1769f6e29ed7`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.ruff_cache/content/a0739889bf9412e8` & `typedal-1.1.1/.ruff_cache/content/a0739889bf9412e8`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.ruff_cache/content/a225e4df39be9b29` & `typedal-1.1.1/.ruff_cache/content/a225e4df39be9b29`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.ruff_cache/content/b419496fa9e72887` & `typedal-1.1.1/.ruff_cache/content/b419496fa9e72887`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.ruff_cache/content/bdcdf5c7bbc1d738` & `typedal-1.1.1/.ruff_cache/content/bdcdf5c7bbc1d738`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.ruff_cache/content/c06de16f3c7a64cc` & `typedal-1.1.1/.ruff_cache/content/c06de16f3c7a64cc`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.ruff_cache/content/cdfecbca581311ee` & `typedal-1.1.1/.ruff_cache/content/cdfecbca581311ee`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.ruff_cache/content/da4811a7730a562a` & `typedal-1.1.1/.ruff_cache/content/da4811a7730a562a`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/.ruff_cache/content/eee2f3c667de6c7a` & `typedal-1.1.1/.ruff_cache/content/eee2f3c667de6c7a`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/htmlcov/coverage_html.js` & `typedal-1.1.1/htmlcov/coverage_html.js`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/htmlcov/d_0ccc93afd6526b6c___about___py.html` & `typedal-1.1.1/htmlcov/d_0ccc93afd6526b6c___about___py.html`

 * *Files 2% similar despite different names*

```diff
@@ -61,15 +61,15 @@
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="index.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_0ccc93afd6526b6c___init___py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-06-05 15:15 +0200
+            created at 2023-06-22 10:05 +0200
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -83,23 +83,23 @@
     <p class="pln"><span class="n"><a id="t1" href="#t1">1</a></span><span class="t"><span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t2" href="#t2">2</a></span><span class="t"><span class="str">This file contains the Version info for this package.</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t3" href="#t3">3</a></span><span class="t"><span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t4" href="#t4">4</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t5" href="#t5">5</a></span><span class="t"><span class="com"># SPDX-FileCopyrightText: 2023-present Robin van der Noord &lt;robinvandernoord@gmail.com></span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t6" href="#t6">6</a></span><span class="t"><span class="com">#</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t7" href="#t7">7</a></span><span class="t"><span class="com"># SPDX-License-Identifier: MIT</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t8" href="#t8">8</a></span><span class="t"><span class="nam">__version__</span> <span class="op">=</span> <span class="str">"0.6.2"</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t8" href="#t8">8</a></span><span class="t"><span class="nam">__version__</span> <span class="op">=</span> <span class="str">"1.0.0"</span>&nbsp;</span><span class="r"></span></p>
 </main>
 <footer>
     <div class="content">
         <p>
             <a id="prevFileLink" class="nav" href="index.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_0ccc93afd6526b6c___init___py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-06-05 15:15 +0200
+            created at 2023-06-22 10:05 +0200
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -7,22 +7,22 @@
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
 ***** 1 statements   1 run 0 missing 0 excluded *****
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.7, created
-at 2023-06-05 15:15 +0200
+at 2023-06-22 10:05 +0200
 
 
 1""" 
 2This file contains the Version info for this package. 
 3""" 
 4 
 5# SPDX-FileCopyrightText: 2023-present Robin van der Noord
 <robinvandernoord@gmail.com> 
 6# 
 7# SPDX-License-Identifier: MIT 
-8__version__ = "0.6.2" 
+8__version__ = "1.0.0" 
 
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.7, created
-at 2023-06-05 15:15 +0200
+at 2023-06-22 10:05 +0200
```

### Comparing `typedal-1.0.0b1/htmlcov/d_0ccc93afd6526b6c___init___py.html` & `typedal-1.1.1/htmlcov/d_0ccc93afd6526b6c___init___py.html`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/htmlcov/d_0ccc93afd6526b6c_core_py.html` & `typedal-1.1.1/htmlcov/d_0ccc93afd6526b6c_core_py.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 <!DOCTYPE html>
 <html>
 <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8">
-    <title>Coverage for src/typedal/core.py: 100%</title>
+    <title>Coverage for src/typedal/core.py: 67%</title>
     <link rel="icon" sizes="32x32" href="favicon_32.png">
     <link rel="stylesheet" href="style.css" type="text/css">
     <script type="text/javascript" src="coverage_html.js" defer></script>
 </head>
 <body class="pyfile">
 <header>
     <div class="content">
         <h1>
             <span class="text">Coverage for </span><b>src/typedal/core.py</b>:
-            <span class="pc_cov">100%</span>
+            <span class="pc_cov">67%</span>
         </h1>
         <aside id="help_panel_wrapper">
             <input id="help_panel_state" type="checkbox">
             <label for="help_panel_state">
                 <img id="keyboard_icon" src="keybd_closed.png" alt="Show/hide keyboard shortcuts" />
             </label>
             <div id="help_panel">
@@ -50,26 +50,26 @@
                     <p>
                         <kbd>?</kbd> &nbsp; show/hide this help
                     </p>
                 </div>
             </div>
         </aside>
         <h2>
-            <span class="text">119 statements &nbsp;</span>
-            <button type="button" class="run button_toggle_run" value="run" data-shortcut="r" title="Toggle lines run">119<span class="text"> run</span></button>
-            <button type="button" class="mis show_mis button_toggle_mis" value="mis" data-shortcut="m" title="Toggle lines missing">0<span class="text"> missing</span></button>
+            <span class="text">124 statements &nbsp;</span>
+            <button type="button" class="run button_toggle_run" value="run" data-shortcut="r" title="Toggle lines run">83<span class="text"> run</span></button>
+            <button type="button" class="mis show_mis button_toggle_mis" value="mis" data-shortcut="m" title="Toggle lines missing">41<span class="text"> missing</span></button>
             <button type="button" class="exc show_exc button_toggle_exc" value="exc" data-shortcut="x" title="Toggle lines excluded">2<span class="text"> excluded</span></button>
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="d_0ccc93afd6526b6c___init___py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_0ccc93afd6526b6c_fields_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-06-05 16:10 +0200
+            created at 2023-06-22 10:11 +0200
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -83,382 +83,406 @@
     <p class="pln"><span class="n"><a id="t1" href="#t1">1</a></span><span class="t"><span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t2" href="#t2">2</a></span><span class="t"><span class="str">Core functionality of TypeDAL.</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t3" href="#t3">3</a></span><span class="t"><span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t4" href="#t4">4</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t5" href="#t5">5</a></span><span class="t"><span class="key">import</span> <span class="nam">datetime</span> <span class="key">as</span> <span class="nam">dt</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t6" href="#t6">6</a></span><span class="t"><span class="key">import</span> <span class="nam">types</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t7" href="#t7">7</a></span><span class="t"><span class="key">import</span> <span class="nam">typing</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t8" href="#t8">8</a></span><span class="t"><span class="key">from</span> <span class="nam">decimal</span> <span class="key">import</span> <span class="nam">Decimal</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t9" href="#t9">9</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t10" href="#t10">10</a></span><span class="t"><span class="key">import</span> <span class="nam">pydal</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t11" href="#t11">11</a></span><span class="t"><span class="key">from</span> <span class="nam">pydal</span><span class="op">.</span><span class="nam">objects</span> <span class="key">import</span> <span class="nam">Field</span><span class="op">,</span> <span class="nam">Query</span><span class="op">,</span> <span class="nam">Row</span><span class="op">,</span> <span class="nam">Rows</span><span class="op">,</span> <span class="nam">Table</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t12" href="#t12">12</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t13" href="#t13">13</a></span><span class="t"><span class="com"># use typing.cast(type, ...) to make mypy happy with unions</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t14" href="#t14">14</a></span><span class="t"><span class="nam">T_annotation</span> <span class="op">=</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Type</span><span class="op">[</span><span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">]</span> <span class="op">|</span> <span class="nam">types</span><span class="op">.</span><span class="nam">UnionType</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t15" href="#t15">15</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t16" href="#t16">16</a></span><span class="t"><span class="nam">BASIC_MAPPINGS</span><span class="op">:</span> <span class="nam">dict</span><span class="op">[</span><span class="nam">T_annotation</span><span class="op">,</span> <span class="nam">str</span><span class="op">]</span> <span class="op">=</span> <span class="op">{</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t17" href="#t17">17</a></span><span class="t">    <span class="nam">str</span><span class="op">:</span> <span class="str">"string"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t18" href="#t18">18</a></span><span class="t">    <span class="nam">int</span><span class="op">:</span> <span class="str">"integer"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t19" href="#t19">19</a></span><span class="t">    <span class="nam">bool</span><span class="op">:</span> <span class="str">"boolean"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t20" href="#t20">20</a></span><span class="t">    <span class="nam">bytes</span><span class="op">:</span> <span class="str">"blob"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t21" href="#t21">21</a></span><span class="t">    <span class="nam">float</span><span class="op">:</span> <span class="str">"double"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t22" href="#t22">22</a></span><span class="t">    <span class="nam">object</span><span class="op">:</span> <span class="str">"json"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t23" href="#t23">23</a></span><span class="t">    <span class="nam">Decimal</span><span class="op">:</span> <span class="str">"decimal(10,2)"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t24" href="#t24">24</a></span><span class="t">    <span class="nam">dt</span><span class="op">.</span><span class="nam">date</span><span class="op">:</span> <span class="str">"date"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t25" href="#t25">25</a></span><span class="t">    <span class="nam">dt</span><span class="op">.</span><span class="nam">time</span><span class="op">:</span> <span class="str">"time"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t26" href="#t26">26</a></span><span class="t">    <span class="nam">dt</span><span class="op">.</span><span class="nam">datetime</span><span class="op">:</span> <span class="str">"datetime"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t27" href="#t27">27</a></span><span class="t"><span class="op">}</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t28" href="#t28">28</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t8" href="#t8">8</a></span><span class="t"><span class="key">from</span> <span class="nam">collections</span> <span class="key">import</span> <span class="nam">ChainMap</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t9" href="#t9">9</a></span><span class="t"><span class="key">from</span> <span class="nam">decimal</span> <span class="key">import</span> <span class="nam">Decimal</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t10" href="#t10">10</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t11" href="#t11">11</a></span><span class="t"><span class="key">import</span> <span class="nam">pydal</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t12" href="#t12">12</a></span><span class="t"><span class="key">from</span> <span class="nam">pydal</span><span class="op">.</span><span class="nam">objects</span> <span class="key">import</span> <span class="nam">Field</span><span class="op">,</span> <span class="nam">Query</span><span class="op">,</span> <span class="nam">Row</span><span class="op">,</span> <span class="nam">Rows</span><span class="op">,</span> <span class="nam">Table</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t13" href="#t13">13</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t14" href="#t14">14</a></span><span class="t"><span class="com"># use typing.cast(type, ...) to make mypy happy with unions</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t15" href="#t15">15</a></span><span class="t"><span class="nam">T_annotation</span> <span class="op">=</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Type</span><span class="op">[</span><span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">]</span> <span class="op">|</span> <span class="nam">types</span><span class="op">.</span><span class="nam">UnionType</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t16" href="#t16">16</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t17" href="#t17">17</a></span><span class="t"><span class="nam">BASIC_MAPPINGS</span><span class="op">:</span> <span class="nam">dict</span><span class="op">[</span><span class="nam">T_annotation</span><span class="op">,</span> <span class="nam">str</span><span class="op">]</span> <span class="op">=</span> <span class="op">{</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t18" href="#t18">18</a></span><span class="t">    <span class="nam">str</span><span class="op">:</span> <span class="str">"string"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t19" href="#t19">19</a></span><span class="t">    <span class="nam">int</span><span class="op">:</span> <span class="str">"integer"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t20" href="#t20">20</a></span><span class="t">    <span class="nam">bool</span><span class="op">:</span> <span class="str">"boolean"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t21" href="#t21">21</a></span><span class="t">    <span class="nam">bytes</span><span class="op">:</span> <span class="str">"blob"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t22" href="#t22">22</a></span><span class="t">    <span class="nam">float</span><span class="op">:</span> <span class="str">"double"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t23" href="#t23">23</a></span><span class="t">    <span class="nam">object</span><span class="op">:</span> <span class="str">"json"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t24" href="#t24">24</a></span><span class="t">    <span class="nam">Decimal</span><span class="op">:</span> <span class="str">"decimal(10,2)"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t25" href="#t25">25</a></span><span class="t">    <span class="nam">dt</span><span class="op">.</span><span class="nam">date</span><span class="op">:</span> <span class="str">"date"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t26" href="#t26">26</a></span><span class="t">    <span class="nam">dt</span><span class="op">.</span><span class="nam">time</span><span class="op">:</span> <span class="str">"time"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t27" href="#t27">27</a></span><span class="t">    <span class="nam">dt</span><span class="op">.</span><span class="nam">datetime</span><span class="op">:</span> <span class="str">"datetime"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t28" href="#t28">28</a></span><span class="t"><span class="op">}</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t29" href="#t29">29</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t30" href="#t30">30</a></span><span class="t"><span class="key">class</span> <span class="nam">_Types</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t31" href="#t31">31</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t32" href="#t32">32</a></span><span class="t"><span class="str">    Internal type storage for stuff that mypy otherwise won't understand.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t33" href="#t33">33</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t34" href="#t34">34</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t35" href="#t35">35</a></span><span class="t">    <span class="nam">NONETYPE</span> <span class="op">=</span> <span class="nam">type</span><span class="op">(</span><span class="key">None</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t36" href="#t36">36</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t30" href="#t30">30</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t31" href="#t31">31</a></span><span class="t"><span class="key">class</span> <span class="nam">_Types</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t32" href="#t32">32</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t33" href="#t33">33</a></span><span class="t"><span class="str">    Internal type storage for stuff that mypy otherwise won't understand.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t34" href="#t34">34</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t35" href="#t35">35</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t36" href="#t36">36</a></span><span class="t">    <span class="nam">NONETYPE</span> <span class="op">=</span> <span class="nam">type</span><span class="op">(</span><span class="key">None</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t37" href="#t37">37</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t38" href="#t38">38</a></span><span class="t"><span class="com"># the input and output of TypeDAL.define</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t39" href="#t39">39</a></span><span class="t"><span class="nam">T</span> <span class="op">=</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">TypeVar</span><span class="op">(</span><span class="str">"T"</span><span class="op">,</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Type</span><span class="op">[</span><span class="str">"TypedTable"</span><span class="op">]</span><span class="op">,</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Type</span><span class="op">[</span><span class="str">"Table"</span><span class="op">]</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t40" href="#t40">40</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t38" href="#t38">38</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t39" href="#t39">39</a></span><span class="t"><span class="com"># the input and output of TypeDAL.define</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t40" href="#t40">40</a></span><span class="t"><span class="nam">T</span> <span class="op">=</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">TypeVar</span><span class="op">(</span><span class="str">"T"</span><span class="op">,</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Type</span><span class="op">[</span><span class="str">"TypedTable"</span><span class="op">]</span><span class="op">,</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Type</span><span class="op">[</span><span class="str">"Table"</span><span class="op">]</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t41" href="#t41">41</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t42" href="#t42">42</a></span><span class="t"><span class="key">def</span> <span class="nam">is_union</span><span class="op">(</span><span class="nam">some_type</span><span class="op">:</span> <span class="nam">type</span><span class="op">)</span> <span class="op">-></span> <span class="nam">bool</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t43" href="#t43">43</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t44" href="#t44">44</a></span><span class="t"><span class="str">    Check if a type is some type of Union.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t45" href="#t45">45</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t46" href="#t46">46</a></span><span class="t"><span class="str">    Args:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t47" href="#t47">47</a></span><span class="t"><span class="str">        some_type: types.UnionType = type(int | str); typing.Union = typing.Union[int, str]</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t48" href="#t48">48</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t49" href="#t49">49</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t50" href="#t50">50</a></span><span class="t">    <span class="key">return</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">get_origin</span><span class="op">(</span><span class="nam">some_type</span><span class="op">)</span> <span class="key">in</span> <span class="op">(</span><span class="nam">types</span><span class="op">.</span><span class="nam">UnionType</span><span class="op">,</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Union</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t51" href="#t51">51</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t42" href="#t42">42</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t43" href="#t43">43</a></span><span class="t"><span class="key">def</span> <span class="nam">is_union</span><span class="op">(</span><span class="nam">some_type</span><span class="op">:</span> <span class="nam">type</span><span class="op">)</span> <span class="op">-></span> <span class="nam">bool</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t44" href="#t44">44</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t45" href="#t45">45</a></span><span class="t"><span class="str">    Check if a type is some type of Union.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t46" href="#t46">46</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t47" href="#t47">47</a></span><span class="t"><span class="str">    Args:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t48" href="#t48">48</a></span><span class="t"><span class="str">        some_type: types.UnionType = type(int | str); typing.Union = typing.Union[int, str]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t49" href="#t49">49</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t50" href="#t50">50</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t51" href="#t51">51</a></span><span class="t">    <span class="key">return</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">get_origin</span><span class="op">(</span><span class="nam">some_type</span><span class="op">)</span> <span class="key">in</span> <span class="op">(</span><span class="nam">types</span><span class="op">.</span><span class="nam">UnionType</span><span class="op">,</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Union</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t52" href="#t52">52</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t53" href="#t53">53</a></span><span class="t"><span class="key">class</span> <span class="nam">TypeDAL</span><span class="op">(</span><span class="nam">pydal</span><span class="op">.</span><span class="nam">DAL</span><span class="op">)</span><span class="op">:</span>  <span class="com"># type: ignore</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t53" href="#t53">53</a></span><span class="t"><span class="key">def</span> <span class="nam">_all_annotations</span><span class="op">(</span><span class="nam">cls</span><span class="op">:</span> <span class="nam">type</span><span class="op">)</span> <span class="op">-></span> <span class="nam">ChainMap</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">type</span><span class="op">]</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t54" href="#t54">54</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t55" href="#t55">55</a></span><span class="t"><span class="str">    Drop-in replacement for pyDAL with layer to convert class-based table definitions to classical pydal define_tables.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t56" href="#t56">56</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t57" href="#t57">57</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t58" href="#t58">58</a></span><span class="t">    <span class="nam">dal</span><span class="op">:</span> <span class="nam">Table</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t55" href="#t55">55</a></span><span class="t"><span class="str">    Returns a dictionary-like ChainMap that includes annotations for all \</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t56" href="#t56">56</a></span><span class="t"><span class="str">    attributes defined in cls or inherited from superclasses.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t57" href="#t57">57</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t58" href="#t58">58</a></span><span class="t">    <span class="key">return</span> <span class="nam">ChainMap</span><span class="op">(</span><span class="op">*</span><span class="op">(</span><span class="nam">c</span><span class="op">.</span><span class="nam">__annotations__</span> <span class="key">for</span> <span class="nam">c</span> <span class="key">in</span> <span class="nam">getattr</span><span class="op">(</span><span class="nam">cls</span><span class="op">,</span> <span class="str">"__mro__"</span><span class="op">,</span> <span class="op">[</span><span class="op">]</span><span class="op">)</span> <span class="key">if</span> <span class="str">"__annotations__"</span> <span class="key">in</span> <span class="nam">c</span><span class="op">.</span><span class="nam">__dict__</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t59" href="#t59">59</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t60" href="#t60">60</a></span><span class="t">    <span class="nam">default_kwargs</span> <span class="op">=</span> <span class="op">{</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t61" href="#t61">61</a></span><span class="t">        <span class="com"># fields are 'required' (notnull) by default:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t62" href="#t62">62</a></span><span class="t">        <span class="str">"notnull"</span><span class="op">:</span> <span class="key">True</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t63" href="#t63">63</a></span><span class="t">    <span class="op">}</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t60" href="#t60">60</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t61" href="#t61">61</a></span><span class="t"><span class="key">def</span> <span class="nam">all_annotations</span><span class="op">(</span><span class="nam">cls</span><span class="op">:</span> <span class="nam">type</span><span class="op">,</span> <span class="nam">_except</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Iterable</span><span class="op">[</span><span class="nam">str</span><span class="op">]</span> <span class="op">=</span> <span class="key">None</span><span class="op">)</span> <span class="op">-></span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">type</span><span class="op">]</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t62" href="#t62">62</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t63" href="#t63">63</a></span><span class="t"><span class="str">    Wrapper around `_all_annotations` that filters away any keys in _except.</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t64" href="#t64">64</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t65" href="#t65">65</a></span><span class="t">    <span class="key">def</span> <span class="nam">define</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">cls</span><span class="op">:</span> <span class="nam">T</span><span class="op">)</span> <span class="op">-></span> <span class="nam">Table</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t66" href="#t66">66</a></span><span class="t">        <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t67" href="#t67">67</a></span><span class="t"><span class="str">        Can be used as a decorator on a class that inherits `TypedTable`, \</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t68" href="#t68">68</a></span><span class="t"><span class="str">          or as a regular method if you need to define your classes before you have access to a 'db' instance.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t65" href="#t65">65</a></span><span class="t"><span class="str">    It also flattens the ChainMap to a regular dict.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t66" href="#t66">66</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t67" href="#t67">67</a></span><span class="t">    <span class="key">if</span> <span class="nam">_except</span> <span class="key">is</span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t68" href="#t68">68</a></span><span class="t">        <span class="nam">_except</span> <span class="op">=</span> <span class="nam">set</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t69" href="#t69">69</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t70" href="#t70">70</a></span><span class="t"><span class="str">        Args:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t71" href="#t71">71</a></span><span class="t"><span class="str">            cls:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t70" href="#t70">70</a></span><span class="t">    <span class="nam">_all</span> <span class="op">=</span> <span class="nam">_all_annotations</span><span class="op">(</span><span class="nam">cls</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t71" href="#t71">71</a></span><span class="t">    <span class="key">return</span> <span class="op">{</span><span class="nam">k</span><span class="op">:</span> <span class="nam">v</span> <span class="key">for</span> <span class="nam">k</span><span class="op">,</span> <span class="nam">v</span> <span class="key">in</span> <span class="nam">_all</span><span class="op">.</span><span class="nam">items</span><span class="op">(</span><span class="op">)</span> <span class="key">if</span> <span class="nam">k</span> <span class="key">not</span> <span class="key">in</span> <span class="nam">_except</span><span class="op">}</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t72" href="#t72">72</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t73" href="#t73">73</a></span><span class="t"><span class="str">        Example:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t74" href="#t74">74</a></span><span class="t"><span class="str">            @db.define</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t75" href="#t75">75</a></span><span class="t"><span class="str">            class Person(TypedTable):</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t76" href="#t76">76</a></span><span class="t"><span class="str">                ...</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t73" href="#t73">73</a></span><span class="t"><span class="key">class</span> <span class="nam">TypeDAL</span><span class="op">(</span><span class="nam">pydal</span><span class="op">.</span><span class="nam">DAL</span><span class="op">)</span><span class="op">:</span>  <span class="com"># type: ignore</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t74" href="#t74">74</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t75" href="#t75">75</a></span><span class="t"><span class="str">    Drop-in replacement for pyDAL with layer to convert class-based table definitions to classical pydal define_tables.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t76" href="#t76">76</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t77" href="#t77">77</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t78" href="#t78">78</a></span><span class="t"><span class="str">            class Article(TypedTable):</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t79" href="#t79">79</a></span><span class="t"><span class="str">                ...</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t80" href="#t80">80</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t81" href="#t81">81</a></span><span class="t"><span class="str">            # at a later time:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t82" href="#t82">82</a></span><span class="t"><span class="str">            db.define(Article)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t83" href="#t83">83</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t84" href="#t84">84</a></span><span class="t"><span class="str">        Returns:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t85" href="#t85">85</a></span><span class="t"><span class="str">            the result of pydal.define_table</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t86" href="#t86">86</a></span><span class="t"><span class="str">        """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t87" href="#t87">87</a></span><span class="t">        <span class="com"># when __future__.annotations is implemented, cls.__annotations__ will not work anymore as below.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t88" href="#t88">88</a></span><span class="t">        <span class="com"># proper way to handle this would be (but gives error right now due to Table implementing magic methods):</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t89" href="#t89">89</a></span><span class="t">        <span class="com"># typing.get_type_hints(cls, globalns=None, localns=None)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t90" href="#t90">90</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t91" href="#t91">91</a></span><span class="t">        <span class="com"># dirty way (with evil eval):</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t92" href="#t92">92</a></span><span class="t">        <span class="com"># [eval(v) for k, v in cls.__annotations__.items()]</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t93" href="#t93">93</a></span><span class="t">        <span class="com"># this however also stops working when variables outside this scope or even references to other</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t94" href="#t94">94</a></span><span class="t">        <span class="com"># objects are used. So for now, this package will NOT work when from __future__ import annotations is used,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t95" href="#t95">95</a></span><span class="t">        <span class="com"># and might break in the future, when this annotations behavior is enabled by default.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t96" href="#t96">96</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t97" href="#t97">97</a></span><span class="t">        <span class="com"># non-annotated variables have to be passed to define_table as kwargs</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t98" href="#t98">98</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t99" href="#t99">99</a></span><span class="t">        <span class="nam">tablename</span> <span class="op">=</span> <span class="nam">self</span><span class="op">.</span><span class="nam">_to_snake</span><span class="op">(</span><span class="nam">cls</span><span class="op">.</span><span class="nam">__name__</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t100" href="#t100">100</a></span><span class="t">        <span class="nam">fields</span> <span class="op">=</span> <span class="op">[</span><span class="nam">self</span><span class="op">.</span><span class="nam">_to_field</span><span class="op">(</span><span class="nam">fname</span><span class="op">,</span> <span class="nam">ftype</span><span class="op">)</span> <span class="key">for</span> <span class="nam">fname</span><span class="op">,</span> <span class="nam">ftype</span> <span class="key">in</span> <span class="nam">cls</span><span class="op">.</span><span class="nam">__annotations__</span><span class="op">.</span><span class="nam">items</span><span class="op">(</span><span class="op">)</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t101" href="#t101">101</a></span><span class="t">        <span class="nam">other_kwargs</span> <span class="op">=</span> <span class="op">{</span><span class="nam">k</span><span class="op">:</span> <span class="nam">v</span> <span class="key">for</span> <span class="nam">k</span><span class="op">,</span> <span class="nam">v</span> <span class="key">in</span> <span class="nam">cls</span><span class="op">.</span><span class="nam">__dict__</span><span class="op">.</span><span class="nam">items</span><span class="op">(</span><span class="op">)</span> <span class="key">if</span> <span class="nam">k</span> <span class="key">not</span> <span class="key">in</span> <span class="nam">cls</span><span class="op">.</span><span class="nam">__annotations__</span> <span class="key">and</span> <span class="key">not</span> <span class="nam">k</span><span class="op">.</span><span class="nam">startswith</span><span class="op">(</span><span class="str">"_"</span><span class="op">)</span><span class="op">}</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t102" href="#t102">102</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t103" href="#t103">103</a></span><span class="t">        <span class="nam">table</span><span class="op">:</span> <span class="nam">Table</span> <span class="op">=</span> <span class="nam">self</span><span class="op">.</span><span class="nam">define_table</span><span class="op">(</span><span class="nam">tablename</span><span class="op">,</span> <span class="op">*</span><span class="nam">fields</span><span class="op">,</span> <span class="op">**</span><span class="nam">other_kwargs</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t104" href="#t104">104</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t105" href="#t105">105</a></span><span class="t">        <span class="nam">cls</span><span class="op">.</span><span class="nam">__set_internals__</span><span class="op">(</span><span class="nam">db</span><span class="op">=</span><span class="nam">self</span><span class="op">,</span> <span class="nam">table</span><span class="op">=</span><span class="nam">table</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t106" href="#t106">106</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t107" href="#t107">107</a></span><span class="t">        <span class="com"># the ACTUAL output is not TypedTable but rather pydal.Table</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t108" href="#t108">108</a></span><span class="t">        <span class="com"># but telling the editor it is T helps with hinting.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t109" href="#t109">109</a></span><span class="t">        <span class="key">return</span> <span class="nam">table</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t78" href="#t78">78</a></span><span class="t">    <span class="nam">dal</span><span class="op">:</span> <span class="nam">Table</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t79" href="#t79">79</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t80" href="#t80">80</a></span><span class="t">    <span class="nam">default_kwargs</span> <span class="op">=</span> <span class="op">{</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t81" href="#t81">81</a></span><span class="t">        <span class="com"># fields are 'required' (notnull) by default:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t82" href="#t82">82</a></span><span class="t">        <span class="str">"notnull"</span><span class="op">:</span> <span class="key">True</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t83" href="#t83">83</a></span><span class="t">    <span class="op">}</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t84" href="#t84">84</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t85" href="#t85">85</a></span><span class="t">    <span class="key">def</span> <span class="nam">define</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">cls</span><span class="op">:</span> <span class="nam">T</span><span class="op">)</span> <span class="op">-></span> <span class="nam">Table</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t86" href="#t86">86</a></span><span class="t">        <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t87" href="#t87">87</a></span><span class="t"><span class="str">        Can be used as a decorator on a class that inherits `TypedTable`, \</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t88" href="#t88">88</a></span><span class="t"><span class="str">          or as a regular method if you need to define your classes before you have access to a 'db' instance.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t89" href="#t89">89</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t90" href="#t90">90</a></span><span class="t"><span class="str">        Args:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t91" href="#t91">91</a></span><span class="t"><span class="str">            cls:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t92" href="#t92">92</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t93" href="#t93">93</a></span><span class="t"><span class="str">        Example:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t94" href="#t94">94</a></span><span class="t"><span class="str">            @db.define</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t95" href="#t95">95</a></span><span class="t"><span class="str">            class Person(TypedTable):</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t96" href="#t96">96</a></span><span class="t"><span class="str">                ...</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t97" href="#t97">97</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t98" href="#t98">98</a></span><span class="t"><span class="str">            class Article(TypedTable):</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t99" href="#t99">99</a></span><span class="t"><span class="str">                ...</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t100" href="#t100">100</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t101" href="#t101">101</a></span><span class="t"><span class="str">            # at a later time:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t102" href="#t102">102</a></span><span class="t"><span class="str">            db.define(Article)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t103" href="#t103">103</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t104" href="#t104">104</a></span><span class="t"><span class="str">        Returns:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t105" href="#t105">105</a></span><span class="t"><span class="str">            the result of pydal.define_table</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t106" href="#t106">106</a></span><span class="t"><span class="str">        """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t107" href="#t107">107</a></span><span class="t">        <span class="com"># when __future__.annotations is implemented, cls.__annotations__ will not work anymore as below.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t108" href="#t108">108</a></span><span class="t">        <span class="com"># proper way to handle this would be (but gives error right now due to Table implementing magic methods):</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t109" href="#t109">109</a></span><span class="t">        <span class="com"># typing.get_type_hints(cls, globalns=None, localns=None)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t110" href="#t110">110</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t111" href="#t111">111</a></span><span class="t">    <span class="key">def</span> <span class="nam">__call__</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="op">*</span><span class="nam">_args</span><span class="op">:</span> <span class="nam">Query</span><span class="op">,</span> <span class="op">**</span><span class="nam">kwargs</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">)</span> <span class="op">-></span> <span class="nam">pydal</span><span class="op">.</span><span class="nam">objects</span><span class="op">.</span><span class="nam">Set</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t112" href="#t112">112</a></span><span class="t">        <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t113" href="#t113">113</a></span><span class="t"><span class="str">        A db instance can be called directly to perform a query.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t114" href="#t114">114</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t115" href="#t115">115</a></span><span class="t"><span class="str">        Usually, only a query is passed</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t111" href="#t111">111</a></span><span class="t">        <span class="com"># dirty way (with evil eval):</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t112" href="#t112">112</a></span><span class="t">        <span class="com"># [eval(v) for k, v in cls.__annotations__.items()]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t113" href="#t113">113</a></span><span class="t">        <span class="com"># this however also stops working when variables outside this scope or even references to other</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t114" href="#t114">114</a></span><span class="t">        <span class="com"># objects are used. So for now, this package will NOT work when from __future__ import annotations is used,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t115" href="#t115">115</a></span><span class="t">        <span class="com"># and might break in the future, when this annotations behavior is enabled by default.</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t116" href="#t116">116</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t117" href="#t117">117</a></span><span class="t"><span class="str">        Example:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t118" href="#t118">118</a></span><span class="t"><span class="str">            db(query).select()</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t119" href="#t119">119</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t120" href="#t120">120</a></span><span class="t"><span class="str">        """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t121" href="#t121">121</a></span><span class="t">        <span class="nam">args</span> <span class="op">=</span> <span class="nam">list</span><span class="op">(</span><span class="nam">_args</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t122" href="#t122">122</a></span><span class="t">        <span class="key">if</span> <span class="nam">args</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t123" href="#t123">123</a></span><span class="t">            <span class="nam">cls</span> <span class="op">=</span> <span class="nam">args</span><span class="op">[</span><span class="num">0</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t124" href="#t124">124</a></span><span class="t">            <span class="key">if</span> <span class="nam">issubclass</span><span class="op">(</span><span class="nam">type</span><span class="op">(</span><span class="nam">cls</span><span class="op">)</span><span class="op">,</span> <span class="nam">type</span><span class="op">)</span> <span class="key">and</span> <span class="nam">issubclass</span><span class="op">(</span><span class="nam">cls</span><span class="op">,</span> <span class="nam">TypedTable</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t125" href="#t125">125</a></span><span class="t">                <span class="com"># table defined without @db.define decorator!</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t126" href="#t126">126</a></span><span class="t">                <span class="nam">args</span><span class="op">[</span><span class="num">0</span><span class="op">]</span> <span class="op">=</span> <span class="nam">cls</span><span class="op">.</span><span class="nam">id</span> <span class="op">!=</span> <span class="key">None</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t127" href="#t127">127</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t128" href="#t128">128</a></span><span class="t">        <span class="key">return</span> <span class="nam">super</span><span class="op">(</span><span class="op">)</span><span class="op">.</span><span class="nam">__call__</span><span class="op">(</span><span class="op">*</span><span class="nam">args</span><span class="op">,</span> <span class="op">**</span><span class="nam">kwargs</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t129" href="#t129">129</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t130" href="#t130">130</a></span><span class="t">    <span class="com"># todo: insert etc shadowen?</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t131" href="#t131">131</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t132" href="#t132">132</a></span><span class="t">    <span class="op">@</span><span class="nam">classmethod</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t133" href="#t133">133</a></span><span class="t">    <span class="key">def</span> <span class="nam">_build_field</span><span class="op">(</span><span class="nam">cls</span><span class="op">,</span> <span class="nam">name</span><span class="op">:</span> <span class="nam">str</span><span class="op">,</span> <span class="nam">_type</span><span class="op">:</span> <span class="nam">str</span><span class="op">,</span> <span class="op">**</span><span class="nam">kw</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">)</span> <span class="op">-></span> <span class="nam">Field</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t134" href="#t134">134</a></span><span class="t">        <span class="key">return</span> <span class="nam">Field</span><span class="op">(</span><span class="nam">name</span><span class="op">,</span> <span class="nam">_type</span><span class="op">,</span> <span class="op">**</span><span class="op">{</span><span class="op">**</span><span class="nam">cls</span><span class="op">.</span><span class="nam">default_kwargs</span><span class="op">,</span> <span class="op">**</span><span class="nam">kw</span><span class="op">}</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t135" href="#t135">135</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t136" href="#t136">136</a></span><span class="t">    <span class="op">@</span><span class="nam">classmethod</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t137" href="#t137">137</a></span><span class="t">    <span class="key">def</span> <span class="nam">_annotation_to_pydal_fieldtype</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t138" href="#t138">138</a></span><span class="t">        <span class="nam">cls</span><span class="op">,</span> <span class="nam">_ftype</span><span class="op">:</span> <span class="nam">T_annotation</span><span class="op">,</span> <span class="nam">mut_kw</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">MutableMapping</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t139" href="#t139">139</a></span><span class="t">    <span class="op">)</span> <span class="op">-></span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Optional</span><span class="op">[</span><span class="nam">str</span><span class="op">]</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t140" href="#t140">140</a></span><span class="t">        <span class="com"># ftype can be a union or type. typing.cast is sometimes used to tell mypy when it's not a union.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t141" href="#t141">141</a></span><span class="t">        <span class="nam">ftype</span> <span class="op">=</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">cast</span><span class="op">(</span><span class="nam">type</span><span class="op">,</span> <span class="nam">_ftype</span><span class="op">)</span>  <span class="com"># cast from typing.Type to type to make mypy happy)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t142" href="#t142">142</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t143" href="#t143">143</a></span><span class="t">        <span class="key">if</span> <span class="nam">mapping</span> <span class="op">:=</span> <span class="nam">BASIC_MAPPINGS</span><span class="op">.</span><span class="nam">get</span><span class="op">(</span><span class="nam">ftype</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t144" href="#t144">144</a></span><span class="t">            <span class="com"># basi types</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t145" href="#t145">145</a></span><span class="t">            <span class="key">return</span> <span class="nam">mapping</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t146" href="#t146">146</a></span><span class="t">        <span class="key">elif</span> <span class="nam">isinstance</span><span class="op">(</span><span class="nam">ftype</span><span class="op">,</span> <span class="nam">Table</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t147" href="#t147">147</a></span><span class="t">            <span class="com"># db.table</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t148" href="#t148">148</a></span><span class="t">            <span class="key">return</span> <span class="str">f"reference {ftype._tablename}"</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t149" href="#t149">149</a></span><span class="t">        <span class="key">elif</span> <span class="nam">issubclass</span><span class="op">(</span><span class="nam">type</span><span class="op">(</span><span class="nam">ftype</span><span class="op">)</span><span class="op">,</span> <span class="nam">type</span><span class="op">)</span> <span class="key">and</span> <span class="nam">issubclass</span><span class="op">(</span><span class="nam">ftype</span><span class="op">,</span> <span class="nam">TypedTable</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t150" href="#t150">150</a></span><span class="t">            <span class="com"># SomeTable</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t151" href="#t151">151</a></span><span class="t">            <span class="nam">snakename</span> <span class="op">=</span> <span class="nam">cls</span><span class="op">.</span><span class="nam">_to_snake</span><span class="op">(</span><span class="nam">ftype</span><span class="op">.</span><span class="nam">__name__</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t152" href="#t152">152</a></span><span class="t">            <span class="key">return</span> <span class="str">f"reference {snakename}"</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t153" href="#t153">153</a></span><span class="t">        <span class="key">elif</span> <span class="nam">isinstance</span><span class="op">(</span><span class="nam">ftype</span><span class="op">,</span> <span class="nam">TypedFieldType</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t154" href="#t154">154</a></span><span class="t">            <span class="com"># FieldType(type, ...)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t155" href="#t155">155</a></span><span class="t">            <span class="key">return</span> <span class="nam">ftype</span><span class="op">.</span><span class="nam">_to_field</span><span class="op">(</span><span class="nam">mut_kw</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t156" href="#t156">156</a></span><span class="t">        <span class="key">elif</span> <span class="nam">isinstance</span><span class="op">(</span><span class="nam">ftype</span><span class="op">,</span> <span class="nam">types</span><span class="op">.</span><span class="nam">GenericAlias</span><span class="op">)</span> <span class="key">and</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">get_origin</span><span class="op">(</span><span class="nam">ftype</span><span class="op">)</span> <span class="key">is</span> <span class="nam">list</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t157" href="#t157">157</a></span><span class="t">            <span class="com"># list[str] -> str -> string -> list:string</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t158" href="#t158">158</a></span><span class="t">            <span class="nam">_child_type</span> <span class="op">=</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">get_args</span><span class="op">(</span><span class="nam">ftype</span><span class="op">)</span><span class="op">[</span><span class="num">0</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t159" href="#t159">159</a></span><span class="t">            <span class="nam">_child_type</span> <span class="op">=</span> <span class="nam">cls</span><span class="op">.</span><span class="nam">_annotation_to_pydal_fieldtype</span><span class="op">(</span><span class="nam">_child_type</span><span class="op">,</span> <span class="nam">mut_kw</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t160" href="#t160">160</a></span><span class="t">            <span class="key">return</span> <span class="str">f"list:{_child_type}"</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t161" href="#t161">161</a></span><span class="t">        <span class="key">elif</span> <span class="nam">is_union</span><span class="op">(</span><span class="nam">ftype</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t162" href="#t162">162</a></span><span class="t">            <span class="com"># str | int -> UnionType</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t163" href="#t163">163</a></span><span class="t">            <span class="com"># typing.Union[str | int] -> typing._UnionGenericAlias</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t164" href="#t164">164</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t165" href="#t165">165</a></span><span class="t">            <span class="com"># typing.Optional[type] == type | None</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t117" href="#t117">117</a></span><span class="t">        <span class="com"># non-annotated variables have to be passed to define_table as kwargs</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t118" href="#t118">118</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t119" href="#t119">119</a></span><span class="t">        <span class="nam">tablename</span> <span class="op">=</span> <span class="nam">self</span><span class="op">.</span><span class="nam">_to_snake</span><span class="op">(</span><span class="nam">cls</span><span class="op">.</span><span class="nam">__name__</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t120" href="#t120">120</a></span><span class="t">        <span class="nam">annotations</span> <span class="op">=</span> <span class="nam">all_annotations</span><span class="op">(</span><span class="nam">cls</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t121" href="#t121">121</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t122" href="#t122">122</a></span><span class="t">        <span class="key">raise</span> <span class="nam">ValueError</span><span class="op">(</span><span class="nam">annotations</span><span class="op">,</span> <span class="nam">cls</span><span class="op">.</span><span class="nam">__dict__</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t123" href="#t123">123</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t124" href="#t124">124</a></span><span class="t">        <span class="nam">fields</span> <span class="op">=</span> <span class="op">[</span><span class="nam">self</span><span class="op">.</span><span class="nam">_to_field</span><span class="op">(</span><span class="nam">fname</span><span class="op">,</span> <span class="nam">ftype</span><span class="op">)</span> <span class="key">for</span> <span class="nam">fname</span><span class="op">,</span> <span class="nam">ftype</span> <span class="key">in</span> <span class="nam">annotations</span><span class="op">.</span><span class="nam">items</span><span class="op">(</span><span class="op">)</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t125" href="#t125">125</a></span><span class="t">        <span class="nam">other_kwargs</span> <span class="op">=</span> <span class="op">{</span><span class="nam">k</span><span class="op">:</span> <span class="nam">v</span> <span class="key">for</span> <span class="nam">k</span><span class="op">,</span> <span class="nam">v</span> <span class="key">in</span> <span class="nam">cls</span><span class="op">.</span><span class="nam">__dict__</span><span class="op">.</span><span class="nam">items</span><span class="op">(</span><span class="op">)</span> <span class="key">if</span> <span class="nam">k</span> <span class="key">not</span> <span class="key">in</span> <span class="nam">annotations</span> <span class="key">and</span> <span class="key">not</span> <span class="nam">k</span><span class="op">.</span><span class="nam">startswith</span><span class="op">(</span><span class="str">"_"</span><span class="op">)</span><span class="op">}</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t126" href="#t126">126</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t127" href="#t127">127</a></span><span class="t">        <span class="nam">table</span><span class="op">:</span> <span class="nam">Table</span> <span class="op">=</span> <span class="nam">self</span><span class="op">.</span><span class="nam">define_table</span><span class="op">(</span><span class="nam">tablename</span><span class="op">,</span> <span class="op">*</span><span class="nam">fields</span><span class="op">,</span> <span class="op">**</span><span class="nam">other_kwargs</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t128" href="#t128">128</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t129" href="#t129">129</a></span><span class="t">        <span class="nam">cls</span><span class="op">.</span><span class="nam">__set_internals__</span><span class="op">(</span><span class="nam">db</span><span class="op">=</span><span class="nam">self</span><span class="op">,</span> <span class="nam">table</span><span class="op">=</span><span class="nam">table</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t130" href="#t130">130</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t131" href="#t131">131</a></span><span class="t">        <span class="com"># the ACTUAL output is not TypedTable but rather pydal.Table</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t132" href="#t132">132</a></span><span class="t">        <span class="com"># but telling the editor it is T helps with hinting.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t133" href="#t133">133</a></span><span class="t">        <span class="key">return</span> <span class="nam">table</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t134" href="#t134">134</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t135" href="#t135">135</a></span><span class="t">    <span class="key">def</span> <span class="nam">__call__</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="op">*</span><span class="nam">_args</span><span class="op">:</span> <span class="nam">Query</span><span class="op">,</span> <span class="op">**</span><span class="nam">kwargs</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">)</span> <span class="op">-></span> <span class="nam">pydal</span><span class="op">.</span><span class="nam">objects</span><span class="op">.</span><span class="nam">Set</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t136" href="#t136">136</a></span><span class="t">        <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t137" href="#t137">137</a></span><span class="t"><span class="str">        A db instance can be called directly to perform a query.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t138" href="#t138">138</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t139" href="#t139">139</a></span><span class="t"><span class="str">        Usually, only a query is passed</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t140" href="#t140">140</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t141" href="#t141">141</a></span><span class="t"><span class="str">        Example:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t142" href="#t142">142</a></span><span class="t"><span class="str">            db(query).select()</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t143" href="#t143">143</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t144" href="#t144">144</a></span><span class="t"><span class="str">        """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t145" href="#t145">145</a></span><span class="t">        <span class="nam">args</span> <span class="op">=</span> <span class="nam">list</span><span class="op">(</span><span class="nam">_args</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t146" href="#t146">146</a></span><span class="t">        <span class="key">if</span> <span class="nam">args</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t147" href="#t147">147</a></span><span class="t">            <span class="nam">cls</span> <span class="op">=</span> <span class="nam">args</span><span class="op">[</span><span class="num">0</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t148" href="#t148">148</a></span><span class="t">            <span class="key">if</span> <span class="nam">issubclass</span><span class="op">(</span><span class="nam">type</span><span class="op">(</span><span class="nam">cls</span><span class="op">)</span><span class="op">,</span> <span class="nam">type</span><span class="op">)</span> <span class="key">and</span> <span class="nam">issubclass</span><span class="op">(</span><span class="nam">cls</span><span class="op">,</span> <span class="nam">TypedTable</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t149" href="#t149">149</a></span><span class="t">                <span class="com"># table defined without @db.define decorator!</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t150" href="#t150">150</a></span><span class="t">                <span class="nam">args</span><span class="op">[</span><span class="num">0</span><span class="op">]</span> <span class="op">=</span> <span class="nam">cls</span><span class="op">.</span><span class="nam">id</span> <span class="op">!=</span> <span class="key">None</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t151" href="#t151">151</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t152" href="#t152">152</a></span><span class="t">        <span class="key">return</span> <span class="nam">super</span><span class="op">(</span><span class="op">)</span><span class="op">.</span><span class="nam">__call__</span><span class="op">(</span><span class="op">*</span><span class="nam">args</span><span class="op">,</span> <span class="op">**</span><span class="nam">kwargs</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t153" href="#t153">153</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t154" href="#t154">154</a></span><span class="t">    <span class="com"># todo: insert etc shadowen?</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t155" href="#t155">155</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t156" href="#t156">156</a></span><span class="t">    <span class="op">@</span><span class="nam">classmethod</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t157" href="#t157">157</a></span><span class="t">    <span class="key">def</span> <span class="nam">_build_field</span><span class="op">(</span><span class="nam">cls</span><span class="op">,</span> <span class="nam">name</span><span class="op">:</span> <span class="nam">str</span><span class="op">,</span> <span class="nam">_type</span><span class="op">:</span> <span class="nam">str</span><span class="op">,</span> <span class="op">**</span><span class="nam">kw</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">)</span> <span class="op">-></span> <span class="nam">Field</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t158" href="#t158">158</a></span><span class="t">        <span class="key">return</span> <span class="nam">Field</span><span class="op">(</span><span class="nam">name</span><span class="op">,</span> <span class="nam">_type</span><span class="op">,</span> <span class="op">**</span><span class="op">{</span><span class="op">**</span><span class="nam">cls</span><span class="op">.</span><span class="nam">default_kwargs</span><span class="op">,</span> <span class="op">**</span><span class="nam">kw</span><span class="op">}</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t159" href="#t159">159</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t160" href="#t160">160</a></span><span class="t">    <span class="op">@</span><span class="nam">classmethod</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t161" href="#t161">161</a></span><span class="t">    <span class="key">def</span> <span class="nam">_annotation_to_pydal_fieldtype</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t162" href="#t162">162</a></span><span class="t">        <span class="nam">cls</span><span class="op">,</span> <span class="nam">_ftype</span><span class="op">:</span> <span class="nam">T_annotation</span><span class="op">,</span> <span class="nam">mut_kw</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">MutableMapping</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t163" href="#t163">163</a></span><span class="t">    <span class="op">)</span> <span class="op">-></span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Optional</span><span class="op">[</span><span class="nam">str</span><span class="op">]</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t164" href="#t164">164</a></span><span class="t">        <span class="com"># ftype can be a union or type. typing.cast is sometimes used to tell mypy when it's not a union.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t165" href="#t165">165</a></span><span class="t">        <span class="nam">ftype</span> <span class="op">=</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">cast</span><span class="op">(</span><span class="nam">type</span><span class="op">,</span> <span class="nam">_ftype</span><span class="op">)</span>  <span class="com"># cast from typing.Type to type to make mypy happy)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t166" href="#t166">166</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t167" href="#t167">167</a></span><span class="t">            <span class="key">match</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">get_args</span><span class="op">(</span><span class="nam">ftype</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t168" href="#t168">168</a></span><span class="t">                <span class="key">case</span> <span class="op">(</span><span class="nam">_child_type</span><span class="op">,</span> <span class="nam">_Types</span><span class="op">.</span><span class="nam">NONETYPE</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t169" href="#t169">169</a></span><span class="t">                    <span class="com"># good union of Nullable</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t170" href="#t170">170</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t171" href="#t171">171</a></span><span class="t">                    <span class="com"># if a field is optional, it is nullable:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t172" href="#t172">172</a></span><span class="t">                    <span class="nam">mut_kw</span><span class="op">[</span><span class="str">"notnull"</span><span class="op">]</span> <span class="op">=</span> <span class="key">False</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t173" href="#t173">173</a></span><span class="t">                    <span class="key">return</span> <span class="nam">cls</span><span class="op">.</span><span class="nam">_annotation_to_pydal_fieldtype</span><span class="op">(</span><span class="nam">_child_type</span><span class="op">,</span> <span class="nam">mut_kw</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t174" href="#t174">174</a></span><span class="t">                <span class="key">case</span> <span class="nam">_</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t175" href="#t175">175</a></span><span class="t">                    <span class="com"># two types is not supported by the db!</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t176" href="#t176">176</a></span><span class="t">                    <span class="key">return</span> <span class="key">None</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t177" href="#t177">177</a></span><span class="t">        <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t178" href="#t178">178</a></span><span class="t">            <span class="key">return</span> <span class="key">None</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t179" href="#t179">179</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t180" href="#t180">180</a></span><span class="t">    <span class="op">@</span><span class="nam">classmethod</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t181" href="#t181">181</a></span><span class="t">    <span class="key">def</span> <span class="nam">_to_field</span><span class="op">(</span><span class="nam">cls</span><span class="op">,</span> <span class="nam">fname</span><span class="op">:</span> <span class="nam">str</span><span class="op">,</span> <span class="nam">ftype</span><span class="op">:</span> <span class="nam">type</span><span class="op">,</span> <span class="op">**</span><span class="nam">kw</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">)</span> <span class="op">-></span> <span class="nam">Field</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t182" href="#t182">182</a></span><span class="t">        <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t183" href="#t183">183</a></span><span class="t"><span class="str">        Convert a annotation into a pydal Field.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t184" href="#t184">184</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t185" href="#t185">185</a></span><span class="t"><span class="str">        Args:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t186" href="#t186">186</a></span><span class="t"><span class="str">            fname: name of the property</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t187" href="#t187">187</a></span><span class="t"><span class="str">            ftype: annotation of the property</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t188" href="#t188">188</a></span><span class="t"><span class="str">            kw: when using TypedField or a function returning it (e.g. StringField),</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t189" href="#t189">189</a></span><span class="t"><span class="str">                keyword args can be used to pass any other settings you would normally to a pydal Field</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t167" href="#t167">167</a></span><span class="t">        <span class="key">if</span> <span class="nam">mapping</span> <span class="op">:=</span> <span class="nam">BASIC_MAPPINGS</span><span class="op">.</span><span class="nam">get</span><span class="op">(</span><span class="nam">ftype</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t168" href="#t168">168</a></span><span class="t">            <span class="com"># basi types</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t169" href="#t169">169</a></span><span class="t">            <span class="key">return</span> <span class="nam">mapping</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t170" href="#t170">170</a></span><span class="t">        <span class="key">elif</span> <span class="nam">isinstance</span><span class="op">(</span><span class="nam">ftype</span><span class="op">,</span> <span class="nam">Table</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t171" href="#t171">171</a></span><span class="t">            <span class="com"># db.table</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t172" href="#t172">172</a></span><span class="t">            <span class="key">return</span> <span class="str">f"reference {ftype._tablename}"</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t173" href="#t173">173</a></span><span class="t">        <span class="key">elif</span> <span class="nam">issubclass</span><span class="op">(</span><span class="nam">type</span><span class="op">(</span><span class="nam">ftype</span><span class="op">)</span><span class="op">,</span> <span class="nam">type</span><span class="op">)</span> <span class="key">and</span> <span class="nam">issubclass</span><span class="op">(</span><span class="nam">ftype</span><span class="op">,</span> <span class="nam">TypedTable</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t174" href="#t174">174</a></span><span class="t">            <span class="com"># SomeTable</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t175" href="#t175">175</a></span><span class="t">            <span class="nam">snakename</span> <span class="op">=</span> <span class="nam">cls</span><span class="op">.</span><span class="nam">_to_snake</span><span class="op">(</span><span class="nam">ftype</span><span class="op">.</span><span class="nam">__name__</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t176" href="#t176">176</a></span><span class="t">            <span class="key">return</span> <span class="str">f"reference {snakename}"</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t177" href="#t177">177</a></span><span class="t">        <span class="key">elif</span> <span class="nam">isinstance</span><span class="op">(</span><span class="nam">ftype</span><span class="op">,</span> <span class="nam">TypedFieldType</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t178" href="#t178">178</a></span><span class="t">            <span class="com"># FieldType(type, ...)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t179" href="#t179">179</a></span><span class="t">            <span class="key">return</span> <span class="nam">ftype</span><span class="op">.</span><span class="nam">_to_field</span><span class="op">(</span><span class="nam">mut_kw</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t180" href="#t180">180</a></span><span class="t">        <span class="key">elif</span> <span class="nam">isinstance</span><span class="op">(</span><span class="nam">ftype</span><span class="op">,</span> <span class="nam">types</span><span class="op">.</span><span class="nam">GenericAlias</span><span class="op">)</span> <span class="key">and</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">get_origin</span><span class="op">(</span><span class="nam">ftype</span><span class="op">)</span> <span class="key">is</span> <span class="nam">list</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t181" href="#t181">181</a></span><span class="t">            <span class="com"># list[str] -> str -> string -> list:string</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t182" href="#t182">182</a></span><span class="t">            <span class="nam">_child_type</span> <span class="op">=</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">get_args</span><span class="op">(</span><span class="nam">ftype</span><span class="op">)</span><span class="op">[</span><span class="num">0</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t183" href="#t183">183</a></span><span class="t">            <span class="nam">_child_type</span> <span class="op">=</span> <span class="nam">cls</span><span class="op">.</span><span class="nam">_annotation_to_pydal_fieldtype</span><span class="op">(</span><span class="nam">_child_type</span><span class="op">,</span> <span class="nam">mut_kw</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t184" href="#t184">184</a></span><span class="t">            <span class="key">return</span> <span class="str">f"list:{_child_type}"</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t185" href="#t185">185</a></span><span class="t">        <span class="key">elif</span> <span class="nam">is_union</span><span class="op">(</span><span class="nam">ftype</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t186" href="#t186">186</a></span><span class="t">            <span class="com"># str | int -> UnionType</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t187" href="#t187">187</a></span><span class="t">            <span class="com"># typing.Union[str | int] -> typing._UnionGenericAlias</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t188" href="#t188">188</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t189" href="#t189">189</a></span><span class="t">            <span class="com"># typing.Optional[type] == type | None</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t190" href="#t190">190</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t191" href="#t191">191</a></span><span class="t"><span class="str">        -> pydal.Field(fname, ftype, **kw)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t192" href="#t192">192</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t193" href="#t193">193</a></span><span class="t"><span class="str">        Example:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t194" href="#t194">194</a></span><span class="t"><span class="str">            class MyTable:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t195" href="#t195">195</a></span><span class="t"><span class="str">                fname: ftype</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t196" href="#t196">196</a></span><span class="t"><span class="str">                id: int</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t197" href="#t197">197</a></span><span class="t"><span class="str">                name: str</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t198" href="#t198">198</a></span><span class="t"><span class="str">                reference: Table</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t199" href="#t199">199</a></span><span class="t"><span class="str">                other: TypedField(str, default="John Doe")  # default will be in kwargs</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t200" href="#t200">200</a></span><span class="t"><span class="str">        """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t201" href="#t201">201</a></span><span class="t">        <span class="nam">fname</span> <span class="op">=</span> <span class="nam">cls</span><span class="op">.</span><span class="nam">_to_snake</span><span class="op">(</span><span class="nam">fname</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t202" href="#t202">202</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t203" href="#t203">203</a></span><span class="t">        <span class="nam">converted_type</span> <span class="op">=</span> <span class="nam">cls</span><span class="op">.</span><span class="nam">_annotation_to_pydal_fieldtype</span><span class="op">(</span><span class="nam">ftype</span><span class="op">,</span> <span class="nam">kw</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t204" href="#t204">204</a></span><span class="t">        <span class="key">if</span> <span class="key">not</span> <span class="nam">converted_type</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t205" href="#t205">205</a></span><span class="t">            <span class="key">raise</span> <span class="nam">NotImplementedError</span><span class="op">(</span><span class="str">f"Unsupported type {ftype}/{type(ftype)}"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t206" href="#t206">206</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t207" href="#t207">207</a></span><span class="t">        <span class="key">return</span> <span class="nam">cls</span><span class="op">.</span><span class="nam">_build_field</span><span class="op">(</span><span class="nam">fname</span><span class="op">,</span> <span class="nam">converted_type</span><span class="op">,</span> <span class="op">**</span><span class="nam">kw</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t191" href="#t191">191</a></span><span class="t">            <span class="key">match</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">get_args</span><span class="op">(</span><span class="nam">ftype</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t192" href="#t192">192</a></span><span class="t">                <span class="key">case</span> <span class="op">(</span><span class="nam">_child_type</span><span class="op">,</span> <span class="nam">_Types</span><span class="op">.</span><span class="nam">NONETYPE</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t193" href="#t193">193</a></span><span class="t">                    <span class="com"># good union of Nullable</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t194" href="#t194">194</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t195" href="#t195">195</a></span><span class="t">                    <span class="com"># if a field is optional, it is nullable:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t196" href="#t196">196</a></span><span class="t">                    <span class="nam">mut_kw</span><span class="op">[</span><span class="str">"notnull"</span><span class="op">]</span> <span class="op">=</span> <span class="key">False</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t197" href="#t197">197</a></span><span class="t">                    <span class="key">return</span> <span class="nam">cls</span><span class="op">.</span><span class="nam">_annotation_to_pydal_fieldtype</span><span class="op">(</span><span class="nam">_child_type</span><span class="op">,</span> <span class="nam">mut_kw</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t198" href="#t198">198</a></span><span class="t">                <span class="key">case</span> <span class="nam">_</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t199" href="#t199">199</a></span><span class="t">                    <span class="com"># two types is not supported by the db!</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t200" href="#t200">200</a></span><span class="t">                    <span class="key">return</span> <span class="key">None</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t201" href="#t201">201</a></span><span class="t">        <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t202" href="#t202">202</a></span><span class="t">            <span class="key">return</span> <span class="key">None</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t203" href="#t203">203</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t204" href="#t204">204</a></span><span class="t">    <span class="op">@</span><span class="nam">classmethod</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t205" href="#t205">205</a></span><span class="t">    <span class="key">def</span> <span class="nam">_to_field</span><span class="op">(</span><span class="nam">cls</span><span class="op">,</span> <span class="nam">fname</span><span class="op">:</span> <span class="nam">str</span><span class="op">,</span> <span class="nam">ftype</span><span class="op">:</span> <span class="nam">type</span><span class="op">,</span> <span class="op">**</span><span class="nam">kw</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">)</span> <span class="op">-></span> <span class="nam">Field</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t206" href="#t206">206</a></span><span class="t">        <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t207" href="#t207">207</a></span><span class="t"><span class="str">        Convert a annotation into a pydal Field.</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t208" href="#t208">208</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t209" href="#t209">209</a></span><span class="t">    <span class="op">@</span><span class="nam">staticmethod</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t210" href="#t210">210</a></span><span class="t">    <span class="key">def</span> <span class="nam">_to_snake</span><span class="op">(</span><span class="nam">camel</span><span class="op">:</span> <span class="nam">str</span><span class="op">)</span> <span class="op">-></span> <span class="nam">str</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t211" href="#t211">211</a></span><span class="t">        <span class="com"># https://stackoverflow.com/a/44969381</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t212" href="#t212">212</a></span><span class="t">        <span class="key">return</span> <span class="str">""</span><span class="op">.</span><span class="nam">join</span><span class="op">(</span><span class="op">[</span><span class="str">f"_{c.lower()}"</span> <span class="key">if</span> <span class="nam">c</span><span class="op">.</span><span class="nam">isupper</span><span class="op">(</span><span class="op">)</span> <span class="key">else</span> <span class="nam">c</span> <span class="key">for</span> <span class="nam">c</span> <span class="key">in</span> <span class="nam">camel</span><span class="op">]</span><span class="op">)</span><span class="op">.</span><span class="nam">lstrip</span><span class="op">(</span><span class="str">"_"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t213" href="#t213">213</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t209" href="#t209">209</a></span><span class="t"><span class="str">        Args:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t210" href="#t210">210</a></span><span class="t"><span class="str">            fname: name of the property</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t211" href="#t211">211</a></span><span class="t"><span class="str">            ftype: annotation of the property</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t212" href="#t212">212</a></span><span class="t"><span class="str">            kw: when using TypedField or a function returning it (e.g. StringField),</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t213" href="#t213">213</a></span><span class="t"><span class="str">                keyword args can be used to pass any other settings you would normally to a pydal Field</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t214" href="#t214">214</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t215" href="#t215">215</a></span><span class="t"><span class="key">class</span> <span class="nam">TypedTableMeta</span><span class="op">(</span><span class="nam">type</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t216" href="#t216">216</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t217" href="#t217">217</a></span><span class="t"><span class="str">    Meta class allows getattribute on class variables instead instance variables.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t218" href="#t218">218</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t219" href="#t219">219</a></span><span class="t"><span class="str">    Used in `class TypedTable(Table, metaclass=TypedTableMeta)`</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t220" href="#t220">220</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t221" href="#t221">221</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t222" href="#t222">222</a></span><span class="t">    <span class="key">def</span> <span class="nam">__getattr__</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">key</span><span class="op">:</span> <span class="nam">str</span><span class="op">)</span> <span class="op">-></span> <span class="nam">Field</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t223" href="#t223">223</a></span><span class="t">        <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t224" href="#t224">224</a></span><span class="t"><span class="str">        The getattr method is only called when getattribute can't find something.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t225" href="#t225">225</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t226" href="#t226">226</a></span><span class="t"><span class="str">        `__get_table_column__` is defined in `TypedTable`</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t227" href="#t227">227</a></span><span class="t"><span class="str">        """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t228" href="#t228">228</a></span><span class="t">        <span class="key">return</span> <span class="nam">self</span><span class="op">.</span><span class="nam">__get_table_column__</span><span class="op">(</span><span class="nam">key</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t229" href="#t229">229</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t215" href="#t215">215</a></span><span class="t"><span class="str">        -> pydal.Field(fname, ftype, **kw)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t216" href="#t216">216</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t217" href="#t217">217</a></span><span class="t"><span class="str">        Example:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t218" href="#t218">218</a></span><span class="t"><span class="str">            class MyTable:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t219" href="#t219">219</a></span><span class="t"><span class="str">                fname: ftype</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t220" href="#t220">220</a></span><span class="t"><span class="str">                id: int</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t221" href="#t221">221</a></span><span class="t"><span class="str">                name: str</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t222" href="#t222">222</a></span><span class="t"><span class="str">                reference: Table</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t223" href="#t223">223</a></span><span class="t"><span class="str">                other: TypedField(str, default="John Doe")  # default will be in kwargs</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t224" href="#t224">224</a></span><span class="t"><span class="str">        """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t225" href="#t225">225</a></span><span class="t">        <span class="nam">fname</span> <span class="op">=</span> <span class="nam">cls</span><span class="op">.</span><span class="nam">_to_snake</span><span class="op">(</span><span class="nam">fname</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t226" href="#t226">226</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t227" href="#t227">227</a></span><span class="t">        <span class="nam">converted_type</span> <span class="op">=</span> <span class="nam">cls</span><span class="op">.</span><span class="nam">_annotation_to_pydal_fieldtype</span><span class="op">(</span><span class="nam">ftype</span><span class="op">,</span> <span class="nam">kw</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t228" href="#t228">228</a></span><span class="t">        <span class="key">if</span> <span class="key">not</span> <span class="nam">converted_type</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t229" href="#t229">229</a></span><span class="t">            <span class="key">raise</span> <span class="nam">NotImplementedError</span><span class="op">(</span><span class="str">f"Unsupported type {ftype}/{type(ftype)}"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t230" href="#t230">230</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t231" href="#t231">231</a></span><span class="t"><span class="key">class</span> <span class="nam">TypedTable</span><span class="op">(</span><span class="nam">Table</span><span class="op">,</span> <span class="nam">metaclass</span><span class="op">=</span><span class="nam">TypedTableMeta</span><span class="op">)</span><span class="op">:</span>  <span class="com"># type: ignore</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t232" href="#t232">232</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t233" href="#t233">233</a></span><span class="t"><span class="str">    Typed version of pydal.Table, does not really do anything itself but forwards logic to pydal.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t234" href="#t234">234</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t235" href="#t235">235</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t236" href="#t236">236</a></span><span class="t">    <span class="nam">id</span><span class="op">:</span> <span class="nam">int</span>  <span class="com"># noqa: 'id' has to be id since that's the db column</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t231" href="#t231">231</a></span><span class="t">        <span class="key">return</span> <span class="nam">cls</span><span class="op">.</span><span class="nam">_build_field</span><span class="op">(</span><span class="nam">fname</span><span class="op">,</span> <span class="nam">converted_type</span><span class="op">,</span> <span class="op">**</span><span class="nam">kw</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t232" href="#t232">232</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t233" href="#t233">233</a></span><span class="t">    <span class="op">@</span><span class="nam">staticmethod</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t234" href="#t234">234</a></span><span class="t">    <span class="key">def</span> <span class="nam">_to_snake</span><span class="op">(</span><span class="nam">camel</span><span class="op">:</span> <span class="nam">str</span><span class="op">)</span> <span class="op">-></span> <span class="nam">str</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t235" href="#t235">235</a></span><span class="t">        <span class="com"># https://stackoverflow.com/a/44969381</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t236" href="#t236">236</a></span><span class="t">        <span class="key">return</span> <span class="str">""</span><span class="op">.</span><span class="nam">join</span><span class="op">(</span><span class="op">[</span><span class="str">f"_{c.lower()}"</span> <span class="key">if</span> <span class="nam">c</span><span class="op">.</span><span class="nam">isupper</span><span class="op">(</span><span class="op">)</span> <span class="key">else</span> <span class="nam">c</span> <span class="key">for</span> <span class="nam">c</span> <span class="key">in</span> <span class="nam">camel</span><span class="op">]</span><span class="op">)</span><span class="op">.</span><span class="nam">lstrip</span><span class="op">(</span><span class="str">"_"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t237" href="#t237">237</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t238" href="#t238">238</a></span><span class="t">    <span class="com"># set up by db.define:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t239" href="#t239">239</a></span><span class="t">    <span class="nam">__db</span><span class="op">:</span> <span class="nam">TypeDAL</span> <span class="op">|</span> <span class="key">None</span> <span class="op">=</span> <span class="key">None</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t240" href="#t240">240</a></span><span class="t">    <span class="nam">__table</span><span class="op">:</span> <span class="nam">Table</span> <span class="op">|</span> <span class="key">None</span> <span class="op">=</span> <span class="key">None</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t241" href="#t241">241</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t242" href="#t242">242</a></span><span class="t">    <span class="op">@</span><span class="nam">classmethod</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t243" href="#t243">243</a></span><span class="t">    <span class="key">def</span> <span class="nam">__set_internals__</span><span class="op">(</span><span class="nam">cls</span><span class="op">,</span> <span class="nam">db</span><span class="op">:</span> <span class="nam">pydal</span><span class="op">.</span><span class="nam">DAL</span><span class="op">,</span> <span class="nam">table</span><span class="op">:</span> <span class="nam">Table</span><span class="op">)</span> <span class="op">-></span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t244" href="#t244">244</a></span><span class="t">        <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t245" href="#t245">245</a></span><span class="t"><span class="str">        Store the related database and pydal table for later usage.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t246" href="#t246">246</a></span><span class="t"><span class="str">        """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t247" href="#t247">247</a></span><span class="t">        <span class="nam">cls</span><span class="op">.</span><span class="nam">__db</span> <span class="op">=</span> <span class="nam">db</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t248" href="#t248">248</a></span><span class="t">        <span class="nam">cls</span><span class="op">.</span><span class="nam">__table</span> <span class="op">=</span> <span class="nam">table</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t238" href="#t238">238</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t239" href="#t239">239</a></span><span class="t"><span class="key">class</span> <span class="nam">TypedTableMeta</span><span class="op">(</span><span class="nam">type</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t240" href="#t240">240</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t241" href="#t241">241</a></span><span class="t"><span class="str">    Meta class allows getattribute on class variables instead instance variables.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t242" href="#t242">242</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t243" href="#t243">243</a></span><span class="t"><span class="str">    Used in `class TypedTable(Table, metaclass=TypedTableMeta)`</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t244" href="#t244">244</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t245" href="#t245">245</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t246" href="#t246">246</a></span><span class="t">    <span class="key">def</span> <span class="nam">__getattr__</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">key</span><span class="op">:</span> <span class="nam">str</span><span class="op">)</span> <span class="op">-></span> <span class="nam">Field</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t247" href="#t247">247</a></span><span class="t">        <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t248" href="#t248">248</a></span><span class="t"><span class="str">        The getattr method is only called when getattribute can't find something.</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t249" href="#t249">249</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t250" href="#t250">250</a></span><span class="t">    <span class="op">@</span><span class="nam">classmethod</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t251" href="#t251">251</a></span><span class="t">    <span class="key">def</span> <span class="nam">__get_table_column__</span><span class="op">(</span><span class="nam">cls</span><span class="op">,</span> <span class="nam">col</span><span class="op">:</span> <span class="nam">str</span><span class="op">)</span> <span class="op">-></span> <span class="nam">Field</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t252" href="#t252">252</a></span><span class="t">        <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t253" href="#t253">253</a></span><span class="t"><span class="str">        Magic method used by TypedTableMeta to get a database field with dot notation on a class.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t250" href="#t250">250</a></span><span class="t"><span class="str">        `__get_table_column__` is defined in `TypedTable`</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t251" href="#t251">251</a></span><span class="t"><span class="str">        """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t252" href="#t252">252</a></span><span class="t">        <span class="key">return</span> <span class="nam">self</span><span class="op">.</span><span class="nam">__get_table_column__</span><span class="op">(</span><span class="nam">key</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t253" href="#t253">253</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t254" href="#t254">254</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t255" href="#t255">255</a></span><span class="t"><span class="str">        Example:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t256" href="#t256">256</a></span><span class="t"><span class="str">            SomeTypedTable.col -> db.table.col (via TypedTableMeta.__getattr__)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t257" href="#t257">257</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t258" href="#t258">258</a></span><span class="t"><span class="str">        """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t259" href="#t259">259</a></span><span class="t">        <span class="com">#</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t260" href="#t260">260</a></span><span class="t">        <span class="key">if</span> <span class="nam">cls</span><span class="op">.</span><span class="nam">__table</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t261" href="#t261">261</a></span><span class="t">            <span class="key">return</span> <span class="nam">cls</span><span class="op">.</span><span class="nam">__table</span><span class="op">[</span><span class="nam">col</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t262" href="#t262">262</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t263" href="#t263">263</a></span><span class="t">    <span class="key">def</span> <span class="nam">__new__</span><span class="op">(</span><span class="nam">cls</span><span class="op">,</span> <span class="op">*</span><span class="nam">a</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">,</span> <span class="op">**</span><span class="nam">kw</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">)</span> <span class="op">-></span> <span class="nam">Row</span><span class="op">:</span>  <span class="com"># or none!</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t264" href="#t264">264</a></span><span class="t">        <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t265" href="#t265">265</a></span><span class="t"><span class="str">        When e.g. Table(id=0) is called without db.define, \</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t266" href="#t266">266</a></span><span class="t"><span class="str">        this catches it and forwards for proper behavior.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t267" href="#t267">267</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t268" href="#t268">268</a></span><span class="t"><span class="str">        Args:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t269" href="#t269">269</a></span><span class="t"><span class="str">            *a: can be for example Table(&lt;id>)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t270" href="#t270">270</a></span><span class="t"><span class="str">            **kw: can be for example Table(slug=&lt;slug>)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t271" href="#t271">271</a></span><span class="t"><span class="str">        """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t272" href="#t272">272</a></span><span class="t">        <span class="key">if</span> <span class="key">not</span> <span class="nam">cls</span><span class="op">.</span><span class="nam">__table</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t273" href="#t273">273</a></span><span class="t">            <span class="key">raise</span> <span class="nam">EnvironmentError</span><span class="op">(</span><span class="str">"@define or db.define is not called on this class yet!"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t274" href="#t274">274</a></span><span class="t">        <span class="key">return</span> <span class="nam">cls</span><span class="op">.</span><span class="nam">__table</span><span class="op">(</span><span class="op">*</span><span class="nam">a</span><span class="op">,</span> <span class="op">**</span><span class="nam">kw</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t275" href="#t275">275</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t276" href="#t276">276</a></span><span class="t">    <span class="op">@</span><span class="nam">classmethod</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t277" href="#t277">277</a></span><span class="t">    <span class="key">def</span> <span class="nam">insert</span><span class="op">(</span><span class="nam">cls</span><span class="op">,</span> <span class="op">**</span><span class="nam">fields</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">)</span> <span class="op">-></span> <span class="nam">int</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t278" href="#t278">278</a></span><span class="t">        <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t279" href="#t279">279</a></span><span class="t"><span class="str">        This is only called when db.define is not used as a decorator.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t280" href="#t280">280</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t281" href="#t281">281</a></span><span class="t"><span class="str">        cls.__table functions as 'self'</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t282" href="#t282">282</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t283" href="#t283">283</a></span><span class="t"><span class="str">        Args:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t284" href="#t284">284</a></span><span class="t"><span class="str">            **fields: anything you want to insert in the database</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t285" href="#t285">285</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t286" href="#t286">286</a></span><span class="t"><span class="str">        Returns: the ID of the new row.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t287" href="#t287">287</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t288" href="#t288">288</a></span><span class="t"><span class="str">        """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t289" href="#t289">289</a></span><span class="t">        <span class="key">if</span> <span class="key">not</span> <span class="nam">cls</span><span class="op">.</span><span class="nam">__table</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t290" href="#t290">290</a></span><span class="t">            <span class="key">raise</span> <span class="nam">EnvironmentError</span><span class="op">(</span><span class="str">"@define or db.define is not called on this class yet!"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t255" href="#t255">255</a></span><span class="t"><span class="key">class</span> <span class="nam">TypedTable</span><span class="op">(</span><span class="nam">Table</span><span class="op">,</span> <span class="nam">metaclass</span><span class="op">=</span><span class="nam">TypedTableMeta</span><span class="op">)</span><span class="op">:</span>  <span class="com"># type: ignore</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t256" href="#t256">256</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t257" href="#t257">257</a></span><span class="t"><span class="str">    Typed version of pydal.Table, does not really do anything itself but forwards logic to pydal.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t258" href="#t258">258</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t259" href="#t259">259</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t260" href="#t260">260</a></span><span class="t">    <span class="nam">id</span><span class="op">:</span> <span class="nam">int</span>  <span class="com"># noqa: 'id' has to be id since that's the db column</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t261" href="#t261">261</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t262" href="#t262">262</a></span><span class="t">    <span class="com"># set up by db.define:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t263" href="#t263">263</a></span><span class="t">    <span class="nam">__db</span><span class="op">:</span> <span class="nam">TypeDAL</span> <span class="op">|</span> <span class="key">None</span> <span class="op">=</span> <span class="key">None</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t264" href="#t264">264</a></span><span class="t">    <span class="nam">__table</span><span class="op">:</span> <span class="nam">Table</span> <span class="op">|</span> <span class="key">None</span> <span class="op">=</span> <span class="key">None</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t265" href="#t265">265</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t266" href="#t266">266</a></span><span class="t">    <span class="op">@</span><span class="nam">classmethod</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t267" href="#t267">267</a></span><span class="t">    <span class="key">def</span> <span class="nam">__set_internals__</span><span class="op">(</span><span class="nam">cls</span><span class="op">,</span> <span class="nam">db</span><span class="op">:</span> <span class="nam">pydal</span><span class="op">.</span><span class="nam">DAL</span><span class="op">,</span> <span class="nam">table</span><span class="op">:</span> <span class="nam">Table</span><span class="op">)</span> <span class="op">-></span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t268" href="#t268">268</a></span><span class="t">        <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t269" href="#t269">269</a></span><span class="t"><span class="str">        Store the related database and pydal table for later usage.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t270" href="#t270">270</a></span><span class="t"><span class="str">        """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t271" href="#t271">271</a></span><span class="t">        <span class="nam">cls</span><span class="op">.</span><span class="nam">__db</span> <span class="op">=</span> <span class="nam">db</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t272" href="#t272">272</a></span><span class="t">        <span class="nam">cls</span><span class="op">.</span><span class="nam">__table</span> <span class="op">=</span> <span class="nam">table</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t273" href="#t273">273</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t274" href="#t274">274</a></span><span class="t">    <span class="op">@</span><span class="nam">classmethod</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t275" href="#t275">275</a></span><span class="t">    <span class="key">def</span> <span class="nam">__get_table_column__</span><span class="op">(</span><span class="nam">cls</span><span class="op">,</span> <span class="nam">col</span><span class="op">:</span> <span class="nam">str</span><span class="op">)</span> <span class="op">-></span> <span class="nam">Field</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t276" href="#t276">276</a></span><span class="t">        <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t277" href="#t277">277</a></span><span class="t"><span class="str">        Magic method used by TypedTableMeta to get a database field with dot notation on a class.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t278" href="#t278">278</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t279" href="#t279">279</a></span><span class="t"><span class="str">        Example:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t280" href="#t280">280</a></span><span class="t"><span class="str">            SomeTypedTable.col -> db.table.col (via TypedTableMeta.__getattr__)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t281" href="#t281">281</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t282" href="#t282">282</a></span><span class="t"><span class="str">        """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t283" href="#t283">283</a></span><span class="t">        <span class="com">#</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t284" href="#t284">284</a></span><span class="t">        <span class="key">if</span> <span class="nam">cls</span><span class="op">.</span><span class="nam">__table</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t285" href="#t285">285</a></span><span class="t">            <span class="key">return</span> <span class="nam">cls</span><span class="op">.</span><span class="nam">__table</span><span class="op">[</span><span class="nam">col</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t286" href="#t286">286</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t287" href="#t287">287</a></span><span class="t">    <span class="key">def</span> <span class="nam">__new__</span><span class="op">(</span><span class="nam">cls</span><span class="op">,</span> <span class="op">*</span><span class="nam">a</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">,</span> <span class="op">**</span><span class="nam">kw</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">)</span> <span class="op">-></span> <span class="nam">Row</span><span class="op">:</span>  <span class="com"># or none!</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t288" href="#t288">288</a></span><span class="t">        <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t289" href="#t289">289</a></span><span class="t"><span class="str">        When e.g. Table(id=0) is called without db.define, \</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t290" href="#t290">290</a></span><span class="t"><span class="str">        this catches it and forwards for proper behavior.</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t291" href="#t291">291</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t292" href="#t292">292</a></span><span class="t">        <span class="nam">result</span> <span class="op">=</span> <span class="nam">super</span><span class="op">(</span><span class="op">)</span><span class="op">.</span><span class="nam">insert</span><span class="op">(</span><span class="nam">cls</span><span class="op">.</span><span class="nam">__table</span><span class="op">,</span> <span class="op">**</span><span class="nam">fields</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t293" href="#t293">293</a></span><span class="t">        <span class="com"># it already is an int but mypy doesn't understand that</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t294" href="#t294">294</a></span><span class="t">        <span class="key">return</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">cast</span><span class="op">(</span><span class="nam">int</span><span class="op">,</span> <span class="nam">result</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t295" href="#t295">295</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t296" href="#t296">296</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t297" href="#t297">297</a></span><span class="t"><span class="com"># backwards compat:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t298" href="#t298">298</a></span><span class="t"><span class="nam">TypedRow</span> <span class="op">=</span> <span class="nam">TypedTable</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t292" href="#t292">292</a></span><span class="t"><span class="str">        Args:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t293" href="#t293">293</a></span><span class="t"><span class="str">            *a: can be for example Table(&lt;id>)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t294" href="#t294">294</a></span><span class="t"><span class="str">            **kw: can be for example Table(slug=&lt;slug>)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t295" href="#t295">295</a></span><span class="t"><span class="str">        """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t296" href="#t296">296</a></span><span class="t">        <span class="key">if</span> <span class="key">not</span> <span class="nam">cls</span><span class="op">.</span><span class="nam">__table</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t297" href="#t297">297</a></span><span class="t">            <span class="key">raise</span> <span class="nam">EnvironmentError</span><span class="op">(</span><span class="str">"@define or db.define is not called on this class yet!"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t298" href="#t298">298</a></span><span class="t">        <span class="key">return</span> <span class="nam">cls</span><span class="op">.</span><span class="nam">__table</span><span class="op">(</span><span class="op">*</span><span class="nam">a</span><span class="op">,</span> <span class="op">**</span><span class="nam">kw</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t299" href="#t299">299</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t300" href="#t300">300</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t301" href="#t301">301</a></span><span class="t"><span class="key">class</span> <span class="nam">TypedFieldType</span><span class="op">(</span><span class="nam">Field</span><span class="op">)</span><span class="op">:</span>  <span class="com"># type: ignore</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t302" href="#t302">302</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t303" href="#t303">303</a></span><span class="t"><span class="str">    Typed version of pydal.Field, which will be converted to a normal Field in the background.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t304" href="#t304">304</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t305" href="#t305">305</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t306" href="#t306">306</a></span><span class="t">    <span class="nam">_table</span> <span class="op">=</span> <span class="str">"&lt;any table>"</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t307" href="#t307">307</a></span><span class="t">    <span class="nam">_type</span><span class="op">:</span> <span class="nam">T_annotation</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t308" href="#t308">308</a></span><span class="t">    <span class="nam">kwargs</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t300" href="#t300">300</a></span><span class="t">    <span class="op">@</span><span class="nam">classmethod</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t301" href="#t301">301</a></span><span class="t">    <span class="key">def</span> <span class="nam">insert</span><span class="op">(</span><span class="nam">cls</span><span class="op">,</span> <span class="op">**</span><span class="nam">fields</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">)</span> <span class="op">-></span> <span class="nam">int</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t302" href="#t302">302</a></span><span class="t">        <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t303" href="#t303">303</a></span><span class="t"><span class="str">        This is only called when db.define is not used as a decorator.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t304" href="#t304">304</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t305" href="#t305">305</a></span><span class="t"><span class="str">        cls.__table functions as 'self'</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t306" href="#t306">306</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t307" href="#t307">307</a></span><span class="t"><span class="str">        Args:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t308" href="#t308">308</a></span><span class="t"><span class="str">            **fields: anything you want to insert in the database</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t309" href="#t309">309</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t310" href="#t310">310</a></span><span class="t">    <span class="key">def</span> <span class="nam">__init__</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">_type</span><span class="op">:</span> <span class="nam">T_annotation</span><span class="op">,</span> <span class="op">**</span><span class="nam">kwargs</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">)</span> <span class="op">-></span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t311" href="#t311">311</a></span><span class="t">        <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t312" href="#t312">312</a></span><span class="t"><span class="str">        A TypedFieldType should not be inited manually, but TypedField (from `fields.py`) should be used!</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t313" href="#t313">313</a></span><span class="t"><span class="str">        """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t314" href="#t314">314</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">_type</span> <span class="op">=</span> <span class="nam">_type</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t315" href="#t315">315</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">kwargs</span> <span class="op">=</span> <span class="nam">kwargs</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t316" href="#t316">316</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t317" href="#t317">317</a></span><span class="t">    <span class="key">def</span> <span class="nam">__str__</span><span class="op">(</span><span class="nam">self</span><span class="op">)</span> <span class="op">-></span> <span class="nam">str</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t318" href="#t318">318</a></span><span class="t">        <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t319" href="#t319">319</a></span><span class="t"><span class="str">        String representation of a Typed Field.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t310" href="#t310">310</a></span><span class="t"><span class="str">        Returns: the ID of the new row.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t311" href="#t311">311</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t312" href="#t312">312</a></span><span class="t"><span class="str">        """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t313" href="#t313">313</a></span><span class="t">        <span class="key">if</span> <span class="key">not</span> <span class="nam">cls</span><span class="op">.</span><span class="nam">__table</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t314" href="#t314">314</a></span><span class="t">            <span class="key">raise</span> <span class="nam">EnvironmentError</span><span class="op">(</span><span class="str">"@define or db.define is not called on this class yet!"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t315" href="#t315">315</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t316" href="#t316">316</a></span><span class="t">        <span class="nam">result</span> <span class="op">=</span> <span class="nam">super</span><span class="op">(</span><span class="op">)</span><span class="op">.</span><span class="nam">insert</span><span class="op">(</span><span class="nam">cls</span><span class="op">.</span><span class="nam">__table</span><span class="op">,</span> <span class="op">**</span><span class="nam">fields</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t317" href="#t317">317</a></span><span class="t">        <span class="com"># it already is an int but mypy doesn't understand that</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t318" href="#t318">318</a></span><span class="t">        <span class="key">return</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">cast</span><span class="op">(</span><span class="nam">int</span><span class="op">,</span> <span class="nam">result</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t319" href="#t319">319</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t320" href="#t320">320</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t321" href="#t321">321</a></span><span class="t"><span class="str">        If `type` is set explicitly (e.g. TypedField(str, type="text")), that type is used: `TypedField.text`,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t322" href="#t322">322</a></span><span class="t"><span class="str">        otherwise the type annotation is used (e.g. TypedField(str) -> TypedField.str)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t323" href="#t323">323</a></span><span class="t"><span class="str">        """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t324" href="#t324">324</a></span><span class="t">        <span class="key">if</span> <span class="str">"type"</span> <span class="key">in</span> <span class="nam">self</span><span class="op">.</span><span class="nam">kwargs</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t325" href="#t325">325</a></span><span class="t">            <span class="com"># manual type in kwargs supplied</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t326" href="#t326">326</a></span><span class="t">            <span class="nam">t</span> <span class="op">=</span> <span class="nam">self</span><span class="op">.</span><span class="nam">kwargs</span><span class="op">[</span><span class="str">"type"</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t327" href="#t327">327</a></span><span class="t">        <span class="key">elif</span> <span class="nam">issubclass</span><span class="op">(</span><span class="nam">type</span><span class="op">,</span> <span class="nam">type</span><span class="op">(</span><span class="nam">self</span><span class="op">.</span><span class="nam">_type</span><span class="op">)</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t328" href="#t328">328</a></span><span class="t">            <span class="com"># normal type, str.__name__ = 'str'</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t329" href="#t329">329</a></span><span class="t">            <span class="nam">t</span> <span class="op">=</span> <span class="nam">getattr</span><span class="op">(</span><span class="nam">self</span><span class="op">.</span><span class="nam">_type</span><span class="op">,</span> <span class="str">"__name__"</span><span class="op">,</span> <span class="nam">str</span><span class="op">(</span><span class="nam">self</span><span class="op">.</span><span class="nam">_type</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t330" href="#t330">330</a></span><span class="t">        <span class="key">elif</span> <span class="nam">t_args</span> <span class="op">:=</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">get_args</span><span class="op">(</span><span class="nam">self</span><span class="op">.</span><span class="nam">_type</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t331" href="#t331">331</a></span><span class="t">            <span class="com"># list[str] -> 'str'</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t332" href="#t332">332</a></span><span class="t">            <span class="nam">t</span> <span class="op">=</span> <span class="nam">t_args</span><span class="op">[</span><span class="num">0</span><span class="op">]</span><span class="op">.</span><span class="nam">__name__</span>&nbsp;</span><span class="r"></span></p>
-    <p class="exc show_exc"><span class="n"><a id="t333" href="#t333">333</a></span><span class="t">        <span class="key">else</span><span class="op">:</span>  <span class="com"># pragma: no cover</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t334" href="#t334">334</a></span><span class="t">            <span class="com"># fallback - something else, may not even happen, I'm not sure</span>&nbsp;</span><span class="r"></span></p>
-    <p class="exc show_exc"><span class="n"><a id="t335" href="#t335">335</a></span><span class="t">            <span class="nam">t</span> <span class="op">=</span> <span class="nam">self</span><span class="op">.</span><span class="nam">_type</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t336" href="#t336">336</a></span><span class="t">        <span class="key">return</span> <span class="str">f"TypedField.{t}"</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t337" href="#t337">337</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t338" href="#t338">338</a></span><span class="t">    <span class="key">def</span> <span class="nam">__repr__</span><span class="op">(</span><span class="nam">self</span><span class="op">)</span> <span class="op">-></span> <span class="nam">str</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t339" href="#t339">339</a></span><span class="t">        <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t340" href="#t340">340</a></span><span class="t"><span class="str">        More detailed string representation of a Typed Field.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t341" href="#t341">341</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t342" href="#t342">342</a></span><span class="t"><span class="str">        Uses __str__ and adds the provided extra options (kwargs) in the representation.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t343" href="#t343">343</a></span><span class="t"><span class="str">        """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t344" href="#t344">344</a></span><span class="t">        <span class="nam">s</span> <span class="op">=</span> <span class="nam">self</span><span class="op">.</span><span class="nam">__str__</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t345" href="#t345">345</a></span><span class="t">        <span class="nam">kw</span> <span class="op">=</span> <span class="nam">self</span><span class="op">.</span><span class="nam">kwargs</span><span class="op">.</span><span class="nam">copy</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t346" href="#t346">346</a></span><span class="t">        <span class="nam">kw</span><span class="op">.</span><span class="nam">pop</span><span class="op">(</span><span class="str">"type"</span><span class="op">,</span> <span class="key">None</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t347" href="#t347">347</a></span><span class="t">        <span class="key">return</span> <span class="str">f"&lt;{s} with options {kw}>"</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t348" href="#t348">348</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t349" href="#t349">349</a></span><span class="t">    <span class="key">def</span> <span class="nam">_to_field</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">extra_kwargs</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">MutableMapping</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">]</span><span class="op">)</span> <span class="op">-></span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Optional</span><span class="op">[</span><span class="nam">str</span><span class="op">]</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t350" href="#t350">350</a></span><span class="t">        <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t351" href="#t351">351</a></span><span class="t"><span class="str">        Convert a Typed Field instance to a pydal.Field.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t352" href="#t352">352</a></span><span class="t"><span class="str">        """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t353" href="#t353">353</a></span><span class="t">        <span class="nam">other_kwargs</span> <span class="op">=</span> <span class="nam">self</span><span class="op">.</span><span class="nam">kwargs</span><span class="op">.</span><span class="nam">copy</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t354" href="#t354">354</a></span><span class="t">        <span class="nam">extra_kwargs</span><span class="op">.</span><span class="nam">update</span><span class="op">(</span><span class="nam">other_kwargs</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t355" href="#t355">355</a></span><span class="t">        <span class="key">return</span> <span class="nam">extra_kwargs</span><span class="op">.</span><span class="nam">pop</span><span class="op">(</span><span class="str">"type"</span><span class="op">,</span> <span class="key">False</span><span class="op">)</span> <span class="key">or</span> <span class="nam">TypeDAL</span><span class="op">.</span><span class="nam">_annotation_to_pydal_fieldtype</span><span class="op">(</span><span class="nam">self</span><span class="op">.</span><span class="nam">_type</span><span class="op">,</span> <span class="nam">extra_kwargs</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t356" href="#t356">356</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t357" href="#t357">357</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t358" href="#t358">358</a></span><span class="t"><span class="nam">S</span> <span class="op">=</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">TypeVar</span><span class="op">(</span><span class="str">"S"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t359" href="#t359">359</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t360" href="#t360">360</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t361" href="#t361">361</a></span><span class="t"><span class="key">class</span> <span class="nam">TypedRows</span><span class="op">(</span><span class="nam">typing</span><span class="op">.</span><span class="nam">Collection</span><span class="op">[</span><span class="nam">S</span><span class="op">]</span><span class="op">,</span> <span class="nam">Rows</span><span class="op">)</span><span class="op">:</span>  <span class="com"># type: ignore</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t362" href="#t362">362</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t363" href="#t363">363</a></span><span class="t"><span class="str">    Can be used as the return type of a .select().</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t364" href="#t364">364</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t365" href="#t365">365</a></span><span class="t"><span class="str">    Example:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t366" href="#t366">366</a></span><span class="t"><span class="str">        people: TypedRows[Person] = db(Person).select()</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t367" href="#t367">367</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t321" href="#t321">321</a></span><span class="t"><span class="com"># backwards compat:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t322" href="#t322">322</a></span><span class="t"><span class="nam">TypedRow</span> <span class="op">=</span> <span class="nam">TypedTable</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t323" href="#t323">323</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t324" href="#t324">324</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t325" href="#t325">325</a></span><span class="t"><span class="key">class</span> <span class="nam">TypedFieldType</span><span class="op">(</span><span class="nam">Field</span><span class="op">)</span><span class="op">:</span>  <span class="com"># type: ignore</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t326" href="#t326">326</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t327" href="#t327">327</a></span><span class="t"><span class="str">    Typed version of pydal.Field, which will be converted to a normal Field in the background.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t328" href="#t328">328</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t329" href="#t329">329</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t330" href="#t330">330</a></span><span class="t">    <span class="nam">_table</span> <span class="op">=</span> <span class="str">"&lt;any table>"</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t331" href="#t331">331</a></span><span class="t">    <span class="nam">_type</span><span class="op">:</span> <span class="nam">T_annotation</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t332" href="#t332">332</a></span><span class="t">    <span class="nam">kwargs</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t333" href="#t333">333</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t334" href="#t334">334</a></span><span class="t">    <span class="key">def</span> <span class="nam">__init__</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">_type</span><span class="op">:</span> <span class="nam">T_annotation</span><span class="op">,</span> <span class="op">**</span><span class="nam">kwargs</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">)</span> <span class="op">-></span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t335" href="#t335">335</a></span><span class="t">        <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t336" href="#t336">336</a></span><span class="t"><span class="str">        A TypedFieldType should not be inited manually, but TypedField (from `fields.py`) should be used!</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t337" href="#t337">337</a></span><span class="t"><span class="str">        """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t338" href="#t338">338</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">_type</span> <span class="op">=</span> <span class="nam">_type</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t339" href="#t339">339</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">kwargs</span> <span class="op">=</span> <span class="nam">kwargs</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t340" href="#t340">340</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t341" href="#t341">341</a></span><span class="t">    <span class="key">def</span> <span class="nam">__str__</span><span class="op">(</span><span class="nam">self</span><span class="op">)</span> <span class="op">-></span> <span class="nam">str</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t342" href="#t342">342</a></span><span class="t">        <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t343" href="#t343">343</a></span><span class="t"><span class="str">        String representation of a Typed Field.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t344" href="#t344">344</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t345" href="#t345">345</a></span><span class="t"><span class="str">        If `type` is set explicitly (e.g. TypedField(str, type="text")), that type is used: `TypedField.text`,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t346" href="#t346">346</a></span><span class="t"><span class="str">        otherwise the type annotation is used (e.g. TypedField(str) -> TypedField.str)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t347" href="#t347">347</a></span><span class="t"><span class="str">        """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t348" href="#t348">348</a></span><span class="t">        <span class="key">if</span> <span class="str">"type"</span> <span class="key">in</span> <span class="nam">self</span><span class="op">.</span><span class="nam">kwargs</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t349" href="#t349">349</a></span><span class="t">            <span class="com"># manual type in kwargs supplied</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t350" href="#t350">350</a></span><span class="t">            <span class="nam">t</span> <span class="op">=</span> <span class="nam">self</span><span class="op">.</span><span class="nam">kwargs</span><span class="op">[</span><span class="str">"type"</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t351" href="#t351">351</a></span><span class="t">        <span class="key">elif</span> <span class="nam">issubclass</span><span class="op">(</span><span class="nam">type</span><span class="op">,</span> <span class="nam">type</span><span class="op">(</span><span class="nam">self</span><span class="op">.</span><span class="nam">_type</span><span class="op">)</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t352" href="#t352">352</a></span><span class="t">            <span class="com"># normal type, str.__name__ = 'str'</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t353" href="#t353">353</a></span><span class="t">            <span class="nam">t</span> <span class="op">=</span> <span class="nam">getattr</span><span class="op">(</span><span class="nam">self</span><span class="op">.</span><span class="nam">_type</span><span class="op">,</span> <span class="str">"__name__"</span><span class="op">,</span> <span class="nam">str</span><span class="op">(</span><span class="nam">self</span><span class="op">.</span><span class="nam">_type</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t354" href="#t354">354</a></span><span class="t">        <span class="key">elif</span> <span class="nam">t_args</span> <span class="op">:=</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">get_args</span><span class="op">(</span><span class="nam">self</span><span class="op">.</span><span class="nam">_type</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t355" href="#t355">355</a></span><span class="t">            <span class="com"># list[str] -> 'str'</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t356" href="#t356">356</a></span><span class="t">            <span class="nam">t</span> <span class="op">=</span> <span class="nam">t_args</span><span class="op">[</span><span class="num">0</span><span class="op">]</span><span class="op">.</span><span class="nam">__name__</span>&nbsp;</span><span class="r"></span></p>
+    <p class="exc show_exc"><span class="n"><a id="t357" href="#t357">357</a></span><span class="t">        <span class="key">else</span><span class="op">:</span>  <span class="com"># pragma: no cover</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t358" href="#t358">358</a></span><span class="t">            <span class="com"># fallback - something else, may not even happen, I'm not sure</span>&nbsp;</span><span class="r"></span></p>
+    <p class="exc show_exc"><span class="n"><a id="t359" href="#t359">359</a></span><span class="t">            <span class="nam">t</span> <span class="op">=</span> <span class="nam">self</span><span class="op">.</span><span class="nam">_type</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t360" href="#t360">360</a></span><span class="t">        <span class="key">return</span> <span class="str">f"TypedField.{t}"</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t361" href="#t361">361</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t362" href="#t362">362</a></span><span class="t">    <span class="key">def</span> <span class="nam">__repr__</span><span class="op">(</span><span class="nam">self</span><span class="op">)</span> <span class="op">-></span> <span class="nam">str</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t363" href="#t363">363</a></span><span class="t">        <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t364" href="#t364">364</a></span><span class="t"><span class="str">        More detailed string representation of a Typed Field.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t365" href="#t365">365</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t366" href="#t366">366</a></span><span class="t"><span class="str">        Uses __str__ and adds the provided extra options (kwargs) in the representation.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t367" href="#t367">367</a></span><span class="t"><span class="str">        """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t368" href="#t368">368</a></span><span class="t">        <span class="nam">s</span> <span class="op">=</span> <span class="nam">self</span><span class="op">.</span><span class="nam">__str__</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t369" href="#t369">369</a></span><span class="t">        <span class="nam">kw</span> <span class="op">=</span> <span class="nam">self</span><span class="op">.</span><span class="nam">kwargs</span><span class="op">.</span><span class="nam">copy</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t370" href="#t370">370</a></span><span class="t">        <span class="nam">kw</span><span class="op">.</span><span class="nam">pop</span><span class="op">(</span><span class="str">"type"</span><span class="op">,</span> <span class="key">None</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t371" href="#t371">371</a></span><span class="t">        <span class="key">return</span> <span class="str">f"&lt;{s} with options {kw}>"</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t372" href="#t372">372</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t373" href="#t373">373</a></span><span class="t">    <span class="key">def</span> <span class="nam">_to_field</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">extra_kwargs</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">MutableMapping</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">]</span><span class="op">)</span> <span class="op">-></span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Optional</span><span class="op">[</span><span class="nam">str</span><span class="op">]</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t374" href="#t374">374</a></span><span class="t">        <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t375" href="#t375">375</a></span><span class="t"><span class="str">        Convert a Typed Field instance to a pydal.Field.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t376" href="#t376">376</a></span><span class="t"><span class="str">        """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t377" href="#t377">377</a></span><span class="t">        <span class="nam">other_kwargs</span> <span class="op">=</span> <span class="nam">self</span><span class="op">.</span><span class="nam">kwargs</span><span class="op">.</span><span class="nam">copy</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t378" href="#t378">378</a></span><span class="t">        <span class="nam">extra_kwargs</span><span class="op">.</span><span class="nam">update</span><span class="op">(</span><span class="nam">other_kwargs</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t379" href="#t379">379</a></span><span class="t">        <span class="key">return</span> <span class="nam">extra_kwargs</span><span class="op">.</span><span class="nam">pop</span><span class="op">(</span><span class="str">"type"</span><span class="op">,</span> <span class="key">False</span><span class="op">)</span> <span class="key">or</span> <span class="nam">TypeDAL</span><span class="op">.</span><span class="nam">_annotation_to_pydal_fieldtype</span><span class="op">(</span><span class="nam">self</span><span class="op">.</span><span class="nam">_type</span><span class="op">,</span> <span class="nam">extra_kwargs</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t380" href="#t380">380</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t381" href="#t381">381</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t382" href="#t382">382</a></span><span class="t"><span class="nam">S</span> <span class="op">=</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">TypeVar</span><span class="op">(</span><span class="str">"S"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t383" href="#t383">383</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t384" href="#t384">384</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t385" href="#t385">385</a></span><span class="t"><span class="key">class</span> <span class="nam">TypedRows</span><span class="op">(</span><span class="nam">typing</span><span class="op">.</span><span class="nam">Collection</span><span class="op">[</span><span class="nam">S</span><span class="op">]</span><span class="op">,</span> <span class="nam">Rows</span><span class="op">)</span><span class="op">:</span>  <span class="com"># type: ignore</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t386" href="#t386">386</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t387" href="#t387">387</a></span><span class="t"><span class="str">    Can be used as the return type of a .select().</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t388" href="#t388">388</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t389" href="#t389">389</a></span><span class="t"><span class="str">    Example:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t390" href="#t390">390</a></span><span class="t"><span class="str">        people: TypedRows[Person] = db(Person).select()</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t391" href="#t391">391</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
 </main>
 <footer>
     <div class="content">
         <p>
             <a id="prevFileLink" class="nav" href="d_0ccc93afd6526b6c___init___py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_0ccc93afd6526b6c_fields_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-06-05 16:10 +0200
+            created at 2023-06-22 10:11 +0200
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -1,414 +1,440 @@
 
-****** Coverage for src/typedal/core.py: 100% ******
+****** Coverage for src/typedal/core.py: 67% ******
  ⁰  [Show/hide keyboard shortcuts]
 Shortcuts on this page
 r m x   toggle line displays
 j k   next/prev highlighted chunk
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
-***** 119 statements   119 run 0 missing 2 excluded *****
+***** 124 statements   83 run 41 missing 2 excluded *****
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.7, created
-at 2023-06-05 16:10 +0200
+at 2023-06-22 10:11 +0200
 
 
 1""" 
 2Core functionality of TypeDAL. 
 3""" 
 4 
 5import datetime as dt 
 6import types 
 7import typing 
-8from decimal import Decimal 
-9 
-10import pydal 
-11from pydal.objects import Field, Query, Row, Rows, Table 
-12 
-13# use typing.cast(type, ...) to make mypy happy with unions 
-14T_annotation = typing.Type[typing.Any] | types.UnionType 
-15 
-16BASIC_MAPPINGS: dict[T_annotation, str] = { 
-17 str: "string", 
-18 int: "integer", 
-19 bool: "boolean", 
-20 bytes: "blob", 
-21 float: "double", 
-22 object: "json", 
-23 Decimal: "decimal(10,2)", 
-24 dt.date: "date", 
-25 dt.time: "time", 
-26 dt.datetime: "datetime", 
-27} 
-28 
+8from collections import ChainMap 
+9from decimal import Decimal 
+10 
+11import pydal 
+12from pydal.objects import Field, Query, Row, Rows, Table 
+13 
+14# use typing.cast(type, ...) to make mypy happy with unions 
+15T_annotation = typing.Type[typing.Any] | types.UnionType 
+16 
+17BASIC_MAPPINGS: dict[T_annotation, str] = { 
+18 str: "string", 
+19 int: "integer", 
+20 bool: "boolean", 
+21 bytes: "blob", 
+22 float: "double", 
+23 object: "json", 
+24 Decimal: "decimal(10,2)", 
+25 dt.date: "date", 
+26 dt.time: "time", 
+27 dt.datetime: "datetime", 
+28} 
 29 
-30class _Types: 
-31 """ 
-32 Internal type storage for stuff that mypy otherwise won't understand. 
-33 """ 
-34 
-35 NONETYPE = type(None) 
-36 
+30 
+31class _Types: 
+32 """ 
+33 Internal type storage for stuff that mypy otherwise won't understand. 
+34 """ 
+35 
+36 NONETYPE = type(None) 
 37 
-38# the input and output of TypeDAL.define 
-39T = typing.TypeVar("T", typing.Type["TypedTable"], typing.Type["Table"]) 
-40 
+38 
+39# the input and output of TypeDAL.define 
+40T = typing.TypeVar("T", typing.Type["TypedTable"], typing.Type["Table"]) 
 41 
-42def is_union(some_type: type) -> bool: 
-43 """ 
-44 Check if a type is some type of Union. 
-45 
-46 Args: 
-47 some_type: types.UnionType = type(int | str); typing.Union = typing.Union
+42 
+43def is_union(some_type: type) -> bool: 
+44 """ 
+45 Check if a type is some type of Union. 
+46 
+47 Args: 
+48 some_type: types.UnionType = type(int | str); typing.Union = typing.Union
 [int, str] 
-48 
-49 """ 
-50 return typing.get_origin(some_type) in (types.UnionType, typing.Union) 
-51 
+49 
+50 """ 
+51 return typing.get_origin(some_type) in (types.UnionType, typing.Union) 
 52 
-53class TypeDAL(pydal.DAL): # type: ignore 
+53def _all_annotations(cls: type) -> ChainMap[str, type]: 
 54 """ 
-55 Drop-in replacement for pyDAL with layer to convert class-based table
-definitions to classical pydal define_tables. 
-56 """ 
-57 
-58 dal: Table 
+55 Returns a dictionary-like ChainMap that includes annotations for all \ 
+56 attributes defined in cls or inherited from superclasses. 
+57 """ 
+58 return ChainMap(*(c.__annotations__ for c in getattr(cls, "__mro__", []) if
+"__annotations__" in c.__dict__)) 
 59 
-60 default_kwargs = { 
-61 # fields are 'required' (notnull) by default: 
-62 "notnull": True, 
-63 } 
+60 
+61def all_annotations(cls: type, _except: typing.Iterable[str] = None) -> dict
+[str, type]: 
+62 """ 
+63 Wrapper around `_all_annotations` that filters away any keys in _except. 
 64 
-65 def define(self, cls: T) -> Table: 
+65 It also flattens the ChainMap to a regular dict. 
 66 """ 
-67 Can be used as a decorator on a class that inherits `TypedTable`, \ 
-68 or as a regular method if you need to define your classes before you have
-access to a 'db' instance. 
+67 if _except is None: 
+68 _except = set() 
 69 
-70 Args: 
-71 cls: 
+70 _all = _all_annotations(cls) 
+71 return {k: v for k, v in _all.items() if k not in _except} 
 72 
-73 Example: 
-74 @db.define 
-75 class Person(TypedTable): 
-76 ... 
+73class TypeDAL(pydal.DAL): # type: ignore 
+74 """ 
+75 Drop-in replacement for pyDAL with layer to convert class-based table
+definitions to classical pydal define_tables. 
+76 """ 
 77 
-78 class Article(TypedTable): 
-79 ... 
-80 
-81 # at a later time: 
-82 db.define(Article) 
-83 
-84 Returns: 
-85 the result of pydal.define_table 
+78 dal: Table 
+79 
+80 default_kwargs = { 
+81 # fields are 'required' (notnull) by default: 
+82 "notnull": True, 
+83 } 
+84 
+85 def define(self, cls: T) -> Table: 
 86 """ 
-87 # when __future__.annotations is implemented, cls.__annotations__ will not
+87 Can be used as a decorator on a class that inherits `TypedTable`, \ 
+88 or as a regular method if you need to define your classes before you have
+access to a 'db' instance. 
+89 
+90 Args: 
+91 cls: 
+92 
+93 Example: 
+94 @db.define 
+95 class Person(TypedTable): 
+96 ... 
+97 
+98 class Article(TypedTable): 
+99 ... 
+100 
+101 # at a later time: 
+102 db.define(Article) 
+103 
+104 Returns: 
+105 the result of pydal.define_table 
+106 """ 
+107 # when __future__.annotations is implemented, cls.__annotations__ will not
 work anymore as below. 
-88 # proper way to handle this would be (but gives error right now due to Table
-implementing magic methods): 
-89 # typing.get_type_hints(cls, globalns=None, localns=None) 
-90 
-91 # dirty way (with evil eval): 
-92 # [eval(v) for k, v in cls.__annotations__.items()] 
-93 # this however also stops working when variables outside this scope or even
+108 # proper way to handle this would be (but gives error right now due to
+Table implementing magic methods): 
+109 # typing.get_type_hints(cls, globalns=None, localns=None) 
+110 
+111 # dirty way (with evil eval): 
+112 # [eval(v) for k, v in cls.__annotations__.items()] 
+113 # this however also stops working when variables outside this scope or even
 references to other 
-94 # objects are used. So for now, this package will NOT work when from
+114 # objects are used. So for now, this package will NOT work when from
 __future__ import annotations is used, 
-95 # and might break in the future, when this annotations behavior is enabled
+115 # and might break in the future, when this annotations behavior is enabled
 by default. 
-96 
-97 # non-annotated variables have to be passed to define_table as kwargs 
-98 
-99 tablename = self._to_snake(cls.__name__) 
-100 fields = [self._to_field(fname, ftype) for fname, ftype in
-cls.__annotations__.items()] 
-101 other_kwargs = {k: v for k, v in cls.__dict__.items() if k not in
-cls.__annotations__ and not k.startswith("_")} 
-102 
-103 table: Table = self.define_table(tablename, *fields, **other_kwargs) 
-104 
-105 cls.__set_internals__(db=self, table=table) 
-106 
-107 # the ACTUAL output is not TypedTable but rather pydal.Table 
-108 # but telling the editor it is T helps with hinting. 
-109 return table 
-110 
-111 def __call__(self, *_args: Query, **kwargs: typing.Any) -
-> pydal.objects.Set: 
-112 """ 
-113 A db instance can be called directly to perform a query. 
-114 
-115 Usually, only a query is passed 
 116 
-117 Example: 
-118 db(query).select() 
-119 
-120 """ 
-121 args = list(_args) 
-122 if args: 
-123 cls = args[0] 
-124 if issubclass(type(cls), type) and issubclass(cls, TypedTable): 
-125 # table defined without @db.define decorator! 
-126 args[0] = cls.id != None 
-127 
-128 return super().__call__(*args, **kwargs) 
-129 
-130 # todo: insert etc shadowen? 
-131 
-132 @classmethod 
-133 def _build_field(cls, name: str, _type: str, **kw: typing.Any) -> Field: 
-134 return Field(name, _type, **{**cls.default_kwargs, **kw}) 
-135 
-136 @classmethod 
-137 def _annotation_to_pydal_fieldtype( 
-138 cls, _ftype: T_annotation, mut_kw: typing.MutableMapping[str, typing.Any] 
-139 ) -> typing.Optional[str]: 
-140 # ftype can be a union or type. typing.cast is sometimes used to tell mypy
+117 # non-annotated variables have to be passed to define_table as kwargs 
+118 
+119 tablename = self._to_snake(cls.__name__) 
+120 annotations = all_annotations(cls) 
+121 
+122 raise ValueError(annotations, cls.__dict__) 
+123 
+124 fields = [self._to_field(fname, ftype) for fname, ftype in
+annotations.items()] 
+125 other_kwargs = {k: v for k, v in cls.__dict__.items() if k not in
+annotations and not k.startswith("_")} 
+126 
+127 table: Table = self.define_table(tablename, *fields, **other_kwargs) 
+128 
+129 cls.__set_internals__(db=self, table=table) 
+130 
+131 # the ACTUAL output is not TypedTable but rather pydal.Table 
+132 # but telling the editor it is T helps with hinting. 
+133 return table 
+134 
+135 def __call__(self, *_args: Query, **kwargs: typing.Any) -
+> pydal.objects.Set: 
+136 """ 
+137 A db instance can be called directly to perform a query. 
+138 
+139 Usually, only a query is passed 
+140 
+141 Example: 
+142 db(query).select() 
+143 
+144 """ 
+145 args = list(_args) 
+146 if args: 
+147 cls = args[0] 
+148 if issubclass(type(cls), type) and issubclass(cls, TypedTable): 
+149 # table defined without @db.define decorator! 
+150 args[0] = cls.id != None 
+151 
+152 return super().__call__(*args, **kwargs) 
+153 
+154 # todo: insert etc shadowen? 
+155 
+156 @classmethod 
+157 def _build_field(cls, name: str, _type: str, **kw: typing.Any) -> Field: 
+158 return Field(name, _type, **{**cls.default_kwargs, **kw}) 
+159 
+160 @classmethod 
+161 def _annotation_to_pydal_fieldtype( 
+162 cls, _ftype: T_annotation, mut_kw: typing.MutableMapping[str, typing.Any] 
+163 ) -> typing.Optional[str]: 
+164 # ftype can be a union or type. typing.cast is sometimes used to tell mypy
 when it's not a union. 
-141 ftype = typing.cast(type, _ftype) # cast from typing.Type to type to make
+165 ftype = typing.cast(type, _ftype) # cast from typing.Type to type to make
 mypy happy) 
-142 
-143 if mapping := BASIC_MAPPINGS.get(ftype): 
-144 # basi types 
-145 return mapping 
-146 elif isinstance(ftype, Table): 
-147 # db.table 
-148 return f"reference {ftype._tablename}" 
-149 elif issubclass(type(ftype), type) and issubclass(ftype, TypedTable): 
-150 # SomeTable 
-151 snakename = cls._to_snake(ftype.__name__) 
-152 return f"reference {snakename}" 
-153 elif isinstance(ftype, TypedFieldType): 
-154 # FieldType(type, ...) 
-155 return ftype._to_field(mut_kw) 
-156 elif isinstance(ftype, types.GenericAlias) and typing.get_origin(ftype) is
-list: 
-157 # list[str] -> str -> string -> list:string 
-158 _child_type = typing.get_args(ftype)[0] 
-159 _child_type = cls._annotation_to_pydal_fieldtype(_child_type, mut_kw) 
-160 return f"list:{_child_type}" 
-161 elif is_union(ftype): 
-162 # str | int -> UnionType 
-163 # typing.Union[str | int] -> typing._UnionGenericAlias 
-164 
-165 # typing.Optional[type] == type | None 
 166 
-167 match typing.get_args(ftype): 
-168 case (_child_type, _Types.NONETYPE): 
-169 # good union of Nullable 
-170 
-171 # if a field is optional, it is nullable: 
-172 mut_kw["notnull"] = False 
-173 return cls._annotation_to_pydal_fieldtype(_child_type, mut_kw) 
-174 case _: 
-175 # two types is not supported by the db! 
-176 return None 
-177 else: 
-178 return None 
-179 
-180 @classmethod 
-181 def _to_field(cls, fname: str, ftype: type, **kw: typing.Any) -> Field: 
-182 """ 
-183 Convert a annotation into a pydal Field. 
-184 
-185 Args: 
-186 fname: name of the property 
-187 ftype: annotation of the property 
-188 kw: when using TypedField or a function returning it (e.g. StringField), 
-189 keyword args can be used to pass any other settings you would normally to a
-pydal Field 
+167 if mapping := BASIC_MAPPINGS.get(ftype): 
+168 # basi types 
+169 return mapping 
+170 elif isinstance(ftype, Table): 
+171 # db.table 
+172 return f"reference {ftype._tablename}" 
+173 elif issubclass(type(ftype), type) and issubclass(ftype, TypedTable): 
+174 # SomeTable 
+175 snakename = cls._to_snake(ftype.__name__) 
+176 return f"reference {snakename}" 
+177 elif isinstance(ftype, TypedFieldType): 
+178 # FieldType(type, ...) 
+179 return ftype._to_field(mut_kw) 
+180 elif isinstance(ftype, types.GenericAlias) and typing.get_origin(ftype) is
+list: 
+181 # list[str] -> str -> string -> list:string 
+182 _child_type = typing.get_args(ftype)[0] 
+183 _child_type = cls._annotation_to_pydal_fieldtype(_child_type, mut_kw) 
+184 return f"list:{_child_type}" 
+185 elif is_union(ftype): 
+186 # str | int -> UnionType 
+187 # typing.Union[str | int] -> typing._UnionGenericAlias 
+188 
+189 # typing.Optional[type] == type | None 
 190 
-191 -> pydal.Field(fname, ftype, **kw) 
-192 
-193 Example: 
-194 class MyTable: 
-195 fname: ftype 
-196 id: int 
-197 name: str 
-198 reference: Table 
-199 other: TypedField(str, default="John Doe") # default will be in kwargs 
-200 """ 
-201 fname = cls._to_snake(fname) 
-202 
-203 converted_type = cls._annotation_to_pydal_fieldtype(ftype, kw) 
-204 if not converted_type: 
-205 raise NotImplementedError(f"Unsupported type {ftype}/{type(ftype)}") 
-206 
-207 return cls._build_field(fname, converted_type, **kw) 
+191 match typing.get_args(ftype): 
+192 case (_child_type, _Types.NONETYPE): 
+193 # good union of Nullable 
+194 
+195 # if a field is optional, it is nullable: 
+196 mut_kw["notnull"] = False 
+197 return cls._annotation_to_pydal_fieldtype(_child_type, mut_kw) 
+198 case _: 
+199 # two types is not supported by the db! 
+200 return None 
+201 else: 
+202 return None 
+203 
+204 @classmethod 
+205 def _to_field(cls, fname: str, ftype: type, **kw: typing.Any) -> Field: 
+206 """ 
+207 Convert a annotation into a pydal Field. 
 208 
-209 @staticmethod 
-210 def _to_snake(camel: str) -> str: 
-211 # https://stackoverflow.com/a/44969381 
-212 return "".join([f"_{c.lower()}" if c.isupper() else c for c in
-camel]).lstrip("_") 
-213 
+209 Args: 
+210 fname: name of the property 
+211 ftype: annotation of the property 
+212 kw: when using TypedField or a function returning it (e.g. StringField), 
+213 keyword args can be used to pass any other settings you would normally to a
+pydal Field 
 214 
-215class TypedTableMeta(type): 
-216 """ 
-217 Meta class allows getattribute on class variables instead instance
-variables. 
-218 
-219 Used in `class TypedTable(Table, metaclass=TypedTableMeta)` 
-220 """ 
-221 
-222 def __getattr__(self, key: str) -> Field: 
-223 """ 
-224 The getattr method is only called when getattribute can't find something. 
-225 
-226 `__get_table_column__` is defined in `TypedTable` 
-227 """ 
-228 return self.__get_table_column__(key) 
-229 
+215 -> pydal.Field(fname, ftype, **kw) 
+216 
+217 Example: 
+218 class MyTable: 
+219 fname: ftype 
+220 id: int 
+221 name: str 
+222 reference: Table 
+223 other: TypedField(str, default="John Doe") # default will be in kwargs 
+224 """ 
+225 fname = cls._to_snake(fname) 
+226 
+227 converted_type = cls._annotation_to_pydal_fieldtype(ftype, kw) 
+228 if not converted_type: 
+229 raise NotImplementedError(f"Unsupported type {ftype}/{type(ftype)}") 
 230 
-231class TypedTable(Table, metaclass=TypedTableMeta): # type: ignore 
-232 """ 
-233 Typed version of pydal.Table, does not really do anything itself but
-forwards logic to pydal. 
-234 """ 
-235 
-236 id: int # noqa: 'id' has to be id since that's the db column 
+231 return cls._build_field(fname, converted_type, **kw) 
+232 
+233 @staticmethod 
+234 def _to_snake(camel: str) -> str: 
+235 # https://stackoverflow.com/a/44969381 
+236 return "".join([f"_{c.lower()}" if c.isupper() else c for c in
+camel]).lstrip("_") 
 237 
-238 # set up by db.define: 
-239 __db: TypeDAL | None = None 
-240 __table: Table | None = None 
-241 
-242 @classmethod 
-243 def __set_internals__(cls, db: pydal.DAL, table: Table) -> None: 
+238 
+239class TypedTableMeta(type): 
+240 """ 
+241 Meta class allows getattribute on class variables instead instance
+variables. 
+242 
+243 Used in `class TypedTable(Table, metaclass=TypedTableMeta)` 
 244 """ 
-245 Store the related database and pydal table for later usage. 
-246 """ 
-247 cls.__db = db 
-248 cls.__table = table 
+245 
+246 def __getattr__(self, key: str) -> Field: 
+247 """ 
+248 The getattr method is only called when getattribute can't find something. 
 249 
-250 @classmethod 
-251 def __get_table_column__(cls, col: str) -> Field: 
-252 """ 
-253 Magic method used by TypedTableMeta to get a database field with dot
-notation on a class. 
+250 `__get_table_column__` is defined in `TypedTable` 
+251 """ 
+252 return self.__get_table_column__(key) 
+253 
 254 
-255 Example: 
-256 SomeTypedTable.col -> db.table.col (via TypedTableMeta.__getattr__) 
-257 
+255class TypedTable(Table, metaclass=TypedTableMeta): # type: ignore 
+256 """ 
+257 Typed version of pydal.Table, does not really do anything itself but
+forwards logic to pydal. 
 258 """ 
-259 # 
-260 if cls.__table: 
-261 return cls.__table[col] 
-262 
-263 def __new__(cls, *a: typing.Any, **kw: typing.Any) -> Row: # or none! 
-264 """ 
-265 When e.g. Table(id=0) is called without db.define, \ 
-266 this catches it and forwards for proper behavior. 
-267 
-268 Args: 
-269 *a: can be for example Table(<id>) 
-270 **kw: can be for example Table(slug=<slug>) 
-271 """ 
-272 if not cls.__table: 
-273 raise EnvironmentError("@define or db.define is not called on this class
-yet!") 
-274 return cls.__table(*a, **kw) 
-275 
-276 @classmethod 
-277 def insert(cls, **fields: typing.Any) -> int: 
-278 """ 
-279 This is only called when db.define is not used as a decorator. 
-280 
-281 cls.__table functions as 'self' 
-282 
-283 Args: 
-284 **fields: anything you want to insert in the database 
-285 
-286 Returns: the ID of the new row. 
-287 
+259 
+260 id: int # noqa: 'id' has to be id since that's the db column 
+261 
+262 # set up by db.define: 
+263 __db: TypeDAL | None = None 
+264 __table: Table | None = None 
+265 
+266 @classmethod 
+267 def __set_internals__(cls, db: pydal.DAL, table: Table) -> None: 
+268 """ 
+269 Store the related database and pydal table for later usage. 
+270 """ 
+271 cls.__db = db 
+272 cls.__table = table 
+273 
+274 @classmethod 
+275 def __get_table_column__(cls, col: str) -> Field: 
+276 """ 
+277 Magic method used by TypedTableMeta to get a database field with dot
+notation on a class. 
+278 
+279 Example: 
+280 SomeTypedTable.col -> db.table.col (via TypedTableMeta.__getattr__) 
+281 
+282 """ 
+283 # 
+284 if cls.__table: 
+285 return cls.__table[col] 
+286 
+287 def __new__(cls, *a: typing.Any, **kw: typing.Any) -> Row: # or none! 
 288 """ 
-289 if not cls.__table: 
-290 raise EnvironmentError("@define or db.define is not called on this class
-yet!") 
+289 When e.g. Table(id=0) is called without db.define, \ 
+290 this catches it and forwards for proper behavior. 
 291 
-292 result = super().insert(cls.__table, **fields) 
-293 # it already is an int but mypy doesn't understand that 
-294 return typing.cast(int, result) 
-295 
-296 
-297# backwards compat: 
-298TypedRow = TypedTable 
+292 Args: 
+293 *a: can be for example Table(<id>) 
+294 **kw: can be for example Table(slug=<slug>) 
+295 """ 
+296 if not cls.__table: 
+297 raise EnvironmentError("@define or db.define is not called on this class
+yet!") 
+298 return cls.__table(*a, **kw) 
 299 
-300 
-301class TypedFieldType(Field): # type: ignore 
+300 @classmethod 
+301 def insert(cls, **fields: typing.Any) -> int: 
 302 """ 
-303 Typed version of pydal.Field, which will be converted to a normal Field in
-the background. 
-304 """ 
-305 
-306 _table = "<any table>" 
-307 _type: T_annotation 
-308 kwargs: typing.Any 
+303 This is only called when db.define is not used as a decorator. 
+304 
+305 cls.__table functions as 'self' 
+306 
+307 Args: 
+308 **fields: anything you want to insert in the database 
 309 
-310 def __init__(self, _type: T_annotation, **kwargs: typing.Any) -> None: 
-311 """ 
-312 A TypedFieldType should not be inited manually, but TypedField (from
-`fields.py`) should be used! 
-313 """ 
-314 self._type = _type 
-315 self.kwargs = kwargs 
-316 
-317 def __str__(self) -> str: 
-318 """ 
-319 String representation of a Typed Field. 
+310 Returns: the ID of the new row. 
+311 
+312 """ 
+313 if not cls.__table: 
+314 raise EnvironmentError("@define or db.define is not called on this class
+yet!") 
+315 
+316 result = super().insert(cls.__table, **fields) 
+317 # it already is an int but mypy doesn't understand that 
+318 return typing.cast(int, result) 
+319 
 320 
-321 If `type` is set explicitly (e.g. TypedField(str, type="text")), that type
+321# backwards compat: 
+322TypedRow = TypedTable 
+323 
+324 
+325class TypedFieldType(Field): # type: ignore 
+326 """ 
+327 Typed version of pydal.Field, which will be converted to a normal Field in
+the background. 
+328 """ 
+329 
+330 _table = "<any table>" 
+331 _type: T_annotation 
+332 kwargs: typing.Any 
+333 
+334 def __init__(self, _type: T_annotation, **kwargs: typing.Any) -> None: 
+335 """ 
+336 A TypedFieldType should not be inited manually, but TypedField (from
+`fields.py`) should be used! 
+337 """ 
+338 self._type = _type 
+339 self.kwargs = kwargs 
+340 
+341 def __str__(self) -> str: 
+342 """ 
+343 String representation of a Typed Field. 
+344 
+345 If `type` is set explicitly (e.g. TypedField(str, type="text")), that type
 is used: `TypedField.text`, 
-322 otherwise the type annotation is used (e.g. TypedField(str) -
+346 otherwise the type annotation is used (e.g. TypedField(str) -
 > TypedField.str) 
-323 """ 
-324 if "type" in self.kwargs: 
-325 # manual type in kwargs supplied 
-326 t = self.kwargs["type"] 
-327 elif issubclass(type, type(self._type)): 
-328 # normal type, str.__name__ = 'str' 
-329 t = getattr(self._type, "__name__", str(self._type)) 
-330 elif t_args := typing.get_args(self._type): 
-331 # list[str] -> 'str' 
-332 t = t_args[0].__name__ 
-333 else: # pragma: no cover 
-334 # fallback - something else, may not even happen, I'm not sure 
-335 t = self._type 
-336 return f"TypedField.{t}" 
-337 
-338 def __repr__(self) -> str: 
-339 """ 
-340 More detailed string representation of a Typed Field. 
-341 
-342 Uses __str__ and adds the provided extra options (kwargs) in the
+347 """ 
+348 if "type" in self.kwargs: 
+349 # manual type in kwargs supplied 
+350 t = self.kwargs["type"] 
+351 elif issubclass(type, type(self._type)): 
+352 # normal type, str.__name__ = 'str' 
+353 t = getattr(self._type, "__name__", str(self._type)) 
+354 elif t_args := typing.get_args(self._type): 
+355 # list[str] -> 'str' 
+356 t = t_args[0].__name__ 
+357 else: # pragma: no cover 
+358 # fallback - something else, may not even happen, I'm not sure 
+359 t = self._type 
+360 return f"TypedField.{t}" 
+361 
+362 def __repr__(self) -> str: 
+363 """ 
+364 More detailed string representation of a Typed Field. 
+365 
+366 Uses __str__ and adds the provided extra options (kwargs) in the
 representation. 
-343 """ 
-344 s = self.__str__() 
-345 kw = self.kwargs.copy() 
-346 kw.pop("type", None) 
-347 return f"<{s} with options {kw}>" 
-348 
-349 def _to_field(self, extra_kwargs: typing.MutableMapping[str, typing.Any]) -
+367 """ 
+368 s = self.__str__() 
+369 kw = self.kwargs.copy() 
+370 kw.pop("type", None) 
+371 return f"<{s} with options {kw}>" 
+372 
+373 def _to_field(self, extra_kwargs: typing.MutableMapping[str, typing.Any]) -
 > typing.Optional[str]: 
-350 """ 
-351 Convert a Typed Field instance to a pydal.Field. 
-352 """ 
-353 other_kwargs = self.kwargs.copy() 
-354 extra_kwargs.update(other_kwargs) 
-355 return extra_kwargs.pop("type", False) or
+374 """ 
+375 Convert a Typed Field instance to a pydal.Field. 
+376 """ 
+377 other_kwargs = self.kwargs.copy() 
+378 extra_kwargs.update(other_kwargs) 
+379 return extra_kwargs.pop("type", False) or
 TypeDAL._annotation_to_pydal_fieldtype(self._type, extra_kwargs) 
-356 
-357 
-358S = typing.TypeVar("S") 
-359 
-360 
-361class TypedRows(typing.Collection[S], Rows): # type: ignore 
-362 """ 
-363 Can be used as the return type of a .select(). 
-364 
-365 Example: 
-366 people: TypedRows[Person] = db(Person).select() 
-367 """ 
+380 
+381 
+382S = typing.TypeVar("S") 
+383 
+384 
+385class TypedRows(typing.Collection[S], Rows): # type: ignore 
+386 """ 
+387 Can be used as the return type of a .select(). 
+388 
+389 Example: 
+390 people: TypedRows[Person] = db(Person).select() 
+391 """ 
 
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.7, created
-at 2023-06-05 16:10 +0200
+at 2023-06-22 10:11 +0200
```

### Comparing `typedal-1.0.0b1/htmlcov/d_0ccc93afd6526b6c_fields_py.html` & `typedal-1.1.1/htmlcov/d_0ccc93afd6526b6c_fields_py.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 <!DOCTYPE html>
 <html>
 <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8">
-    <title>Coverage for src/typedal/fields.py: 100%</title>
+    <title>Coverage for src/typedal/fields.py: 55%</title>
     <link rel="icon" sizes="32x32" href="favicon_32.png">
     <link rel="stylesheet" href="style.css" type="text/css">
     <script type="text/javascript" src="coverage_html.js" defer></script>
 </head>
 <body class="pyfile">
 <header>
     <div class="content">
         <h1>
             <span class="text">Coverage for </span><b>src/typedal/fields.py</b>:
-            <span class="pc_cov">100%</span>
+            <span class="pc_cov">55%</span>
         </h1>
         <aside id="help_panel_wrapper">
             <input id="help_panel_state" type="checkbox">
             <label for="help_panel_state">
                 <img id="keyboard_icon" src="keybd_closed.png" alt="Show/hide keyboard shortcuts" />
             </label>
             <div id="help_panel">
@@ -51,25 +51,25 @@
                         <kbd>?</kbd> &nbsp; show/hide this help
                     </p>
                 </div>
             </div>
         </aside>
         <h2>
             <span class="text">91 statements &nbsp;</span>
-            <button type="button" class="run button_toggle_run" value="run" data-shortcut="r" title="Toggle lines run">91<span class="text"> run</span></button>
-            <button type="button" class="mis show_mis button_toggle_mis" value="mis" data-shortcut="m" title="Toggle lines missing">0<span class="text"> missing</span></button>
+            <button type="button" class="run button_toggle_run" value="run" data-shortcut="r" title="Toggle lines run">50<span class="text"> run</span></button>
+            <button type="button" class="mis show_mis button_toggle_mis" value="mis" data-shortcut="m" title="Toggle lines missing">41<span class="text"> missing</span></button>
             <button type="button" class="exc show_exc button_toggle_exc" value="exc" data-shortcut="x" title="Toggle lines excluded">0<span class="text"> excluded</span></button>
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="d_0ccc93afd6526b6c_core_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="index.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-06-05 16:09 +0200
+            created at 2023-06-22 10:11 +0200
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -120,16 +120,16 @@
     <p class="pln"><span class="n"><a id="t38" href="#t38">38</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t39" href="#t39">39</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t40" href="#t40">40</a></span><span class="t"><span class="com">## specific</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t41" href="#t41">41</a></span><span class="t"><span class="key">def</span> <span class="nam">StringField</span><span class="op">(</span><span class="op">**</span><span class="nam">kw</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">)</span> <span class="op">-></span> <span class="nam">TYPE_STR</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t42" href="#t42">42</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t43" href="#t43">43</a></span><span class="t"><span class="str">    Pydal type is string, Python type is str.</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t44" href="#t44">44</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t45" href="#t45">45</a></span><span class="t">    <span class="nam">kw</span><span class="op">[</span><span class="str">"type"</span><span class="op">]</span> <span class="op">=</span> <span class="str">"string"</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t46" href="#t46">46</a></span><span class="t">    <span class="key">return</span> <span class="nam">TypedField</span><span class="op">(</span><span class="nam">str</span><span class="op">,</span> <span class="op">**</span><span class="nam">kw</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t45" href="#t45">45</a></span><span class="t">    <span class="nam">kw</span><span class="op">[</span><span class="str">"type"</span><span class="op">]</span> <span class="op">=</span> <span class="str">"string"</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t46" href="#t46">46</a></span><span class="t">    <span class="key">return</span> <span class="nam">TypedField</span><span class="op">(</span><span class="nam">str</span><span class="op">,</span> <span class="op">**</span><span class="nam">kw</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t47" href="#t47">47</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t48" href="#t48">48</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t49" href="#t49">49</a></span><span class="t"><span class="nam">String</span> <span class="op">=</span> <span class="nam">StringField</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t50" href="#t50">50</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t51" href="#t51">51</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t52" href="#t52">52</a></span><span class="t"><span class="key">def</span> <span class="nam">TextField</span><span class="op">(</span><span class="op">**</span><span class="nam">kw</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">)</span> <span class="op">-></span> <span class="nam">TYPE_STR</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t53" href="#t53">53</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
@@ -142,202 +142,202 @@
     <p class="run"><span class="n"><a id="t60" href="#t60">60</a></span><span class="t"><span class="nam">Text</span> <span class="op">=</span> <span class="nam">TextField</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t61" href="#t61">61</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t62" href="#t62">62</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t63" href="#t63">63</a></span><span class="t"><span class="key">def</span> <span class="nam">BlobField</span><span class="op">(</span><span class="op">**</span><span class="nam">kw</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">)</span> <span class="op">-></span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Type</span><span class="op">[</span><span class="nam">bytes</span><span class="op">]</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t64" href="#t64">64</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t65" href="#t65">65</a></span><span class="t"><span class="str">    Pydal type is blob, Python type is bytes.</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t66" href="#t66">66</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t67" href="#t67">67</a></span><span class="t">    <span class="nam">kw</span><span class="op">[</span><span class="str">"type"</span><span class="op">]</span> <span class="op">=</span> <span class="str">"blob"</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t68" href="#t68">68</a></span><span class="t">    <span class="key">return</span> <span class="nam">TypedField</span><span class="op">(</span><span class="nam">bytes</span><span class="op">,</span> <span class="op">**</span><span class="nam">kw</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t67" href="#t67">67</a></span><span class="t">    <span class="nam">kw</span><span class="op">[</span><span class="str">"type"</span><span class="op">]</span> <span class="op">=</span> <span class="str">"blob"</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t68" href="#t68">68</a></span><span class="t">    <span class="key">return</span> <span class="nam">TypedField</span><span class="op">(</span><span class="nam">bytes</span><span class="op">,</span> <span class="op">**</span><span class="nam">kw</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t69" href="#t69">69</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t70" href="#t70">70</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t71" href="#t71">71</a></span><span class="t"><span class="nam">Blob</span> <span class="op">=</span> <span class="nam">BlobField</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t72" href="#t72">72</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t73" href="#t73">73</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t74" href="#t74">74</a></span><span class="t"><span class="key">def</span> <span class="nam">BooleanField</span><span class="op">(</span><span class="op">**</span><span class="nam">kw</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">)</span> <span class="op">-></span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Type</span><span class="op">[</span><span class="nam">bool</span><span class="op">]</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t75" href="#t75">75</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t76" href="#t76">76</a></span><span class="t"><span class="str">    Pydal type is boolean, Python type is bool.</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t77" href="#t77">77</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t78" href="#t78">78</a></span><span class="t">    <span class="nam">kw</span><span class="op">[</span><span class="str">"type"</span><span class="op">]</span> <span class="op">=</span> <span class="str">"boolean"</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t79" href="#t79">79</a></span><span class="t">    <span class="key">return</span> <span class="nam">TypedField</span><span class="op">(</span><span class="nam">bool</span><span class="op">,</span> <span class="op">**</span><span class="nam">kw</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t78" href="#t78">78</a></span><span class="t">    <span class="nam">kw</span><span class="op">[</span><span class="str">"type"</span><span class="op">]</span> <span class="op">=</span> <span class="str">"boolean"</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t79" href="#t79">79</a></span><span class="t">    <span class="key">return</span> <span class="nam">TypedField</span><span class="op">(</span><span class="nam">bool</span><span class="op">,</span> <span class="op">**</span><span class="nam">kw</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t80" href="#t80">80</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t81" href="#t81">81</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t82" href="#t82">82</a></span><span class="t"><span class="nam">Boolean</span> <span class="op">=</span> <span class="nam">BooleanField</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t83" href="#t83">83</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t84" href="#t84">84</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t85" href="#t85">85</a></span><span class="t"><span class="key">def</span> <span class="nam">IntegerField</span><span class="op">(</span><span class="op">**</span><span class="nam">kw</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">)</span> <span class="op">-></span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Type</span><span class="op">[</span><span class="nam">int</span><span class="op">]</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t86" href="#t86">86</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t87" href="#t87">87</a></span><span class="t"><span class="str">    Pydal type is integer, Python type is int.</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t88" href="#t88">88</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t89" href="#t89">89</a></span><span class="t">    <span class="nam">kw</span><span class="op">[</span><span class="str">"type"</span><span class="op">]</span> <span class="op">=</span> <span class="str">"integer"</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t90" href="#t90">90</a></span><span class="t">    <span class="key">return</span> <span class="nam">TypedField</span><span class="op">(</span><span class="nam">int</span><span class="op">,</span> <span class="op">**</span><span class="nam">kw</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t89" href="#t89">89</a></span><span class="t">    <span class="nam">kw</span><span class="op">[</span><span class="str">"type"</span><span class="op">]</span> <span class="op">=</span> <span class="str">"integer"</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t90" href="#t90">90</a></span><span class="t">    <span class="key">return</span> <span class="nam">TypedField</span><span class="op">(</span><span class="nam">int</span><span class="op">,</span> <span class="op">**</span><span class="nam">kw</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t91" href="#t91">91</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t92" href="#t92">92</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t93" href="#t93">93</a></span><span class="t"><span class="nam">Integer</span> <span class="op">=</span> <span class="nam">IntegerField</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t94" href="#t94">94</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t95" href="#t95">95</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t96" href="#t96">96</a></span><span class="t"><span class="key">def</span> <span class="nam">DoubleField</span><span class="op">(</span><span class="op">**</span><span class="nam">kw</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">)</span> <span class="op">-></span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Type</span><span class="op">[</span><span class="nam">float</span><span class="op">]</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t97" href="#t97">97</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t98" href="#t98">98</a></span><span class="t"><span class="str">    Pydal type is double, Python type is float.</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t99" href="#t99">99</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t100" href="#t100">100</a></span><span class="t">    <span class="nam">kw</span><span class="op">[</span><span class="str">"type"</span><span class="op">]</span> <span class="op">=</span> <span class="str">"double"</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t101" href="#t101">101</a></span><span class="t">    <span class="key">return</span> <span class="nam">TypedField</span><span class="op">(</span><span class="nam">float</span><span class="op">,</span> <span class="op">**</span><span class="nam">kw</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t100" href="#t100">100</a></span><span class="t">    <span class="nam">kw</span><span class="op">[</span><span class="str">"type"</span><span class="op">]</span> <span class="op">=</span> <span class="str">"double"</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t101" href="#t101">101</a></span><span class="t">    <span class="key">return</span> <span class="nam">TypedField</span><span class="op">(</span><span class="nam">float</span><span class="op">,</span> <span class="op">**</span><span class="nam">kw</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t102" href="#t102">102</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t103" href="#t103">103</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t104" href="#t104">104</a></span><span class="t"><span class="nam">Double</span> <span class="op">=</span> <span class="nam">DoubleField</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t105" href="#t105">105</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t106" href="#t106">106</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t107" href="#t107">107</a></span><span class="t"><span class="key">def</span> <span class="nam">DecimalField</span><span class="op">(</span><span class="nam">n</span><span class="op">:</span> <span class="nam">int</span><span class="op">,</span> <span class="nam">m</span><span class="op">:</span> <span class="nam">int</span><span class="op">,</span> <span class="op">**</span><span class="nam">kw</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">)</span> <span class="op">-></span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Type</span><span class="op">[</span><span class="nam">decimal</span><span class="op">.</span><span class="nam">Decimal</span><span class="op">]</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t108" href="#t108">108</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t109" href="#t109">109</a></span><span class="t"><span class="str">    Pydal type is decimal, Python type is Decimal.</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t110" href="#t110">110</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t111" href="#t111">111</a></span><span class="t">    <span class="nam">kw</span><span class="op">[</span><span class="str">"type"</span><span class="op">]</span> <span class="op">=</span> <span class="str">f"decimal({n}, {m})"</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t112" href="#t112">112</a></span><span class="t">    <span class="key">return</span> <span class="nam">TypedField</span><span class="op">(</span><span class="nam">decimal</span><span class="op">.</span><span class="nam">Decimal</span><span class="op">,</span> <span class="op">**</span><span class="nam">kw</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t111" href="#t111">111</a></span><span class="t">    <span class="nam">kw</span><span class="op">[</span><span class="str">"type"</span><span class="op">]</span> <span class="op">=</span> <span class="str">f"decimal({n}, {m})"</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t112" href="#t112">112</a></span><span class="t">    <span class="key">return</span> <span class="nam">TypedField</span><span class="op">(</span><span class="nam">decimal</span><span class="op">.</span><span class="nam">Decimal</span><span class="op">,</span> <span class="op">**</span><span class="nam">kw</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t113" href="#t113">113</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t114" href="#t114">114</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t115" href="#t115">115</a></span><span class="t"><span class="nam">Decimal</span> <span class="op">=</span> <span class="nam">DecimalField</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t116" href="#t116">116</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t117" href="#t117">117</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t118" href="#t118">118</a></span><span class="t"><span class="key">def</span> <span class="nam">DateField</span><span class="op">(</span><span class="op">**</span><span class="nam">kw</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">)</span> <span class="op">-></span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Type</span><span class="op">[</span><span class="nam">dt</span><span class="op">.</span><span class="nam">date</span><span class="op">]</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t119" href="#t119">119</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t120" href="#t120">120</a></span><span class="t"><span class="str">    Pydal type is date, Python type is datetime.date.</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t121" href="#t121">121</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t122" href="#t122">122</a></span><span class="t">    <span class="nam">kw</span><span class="op">[</span><span class="str">"type"</span><span class="op">]</span> <span class="op">=</span> <span class="str">"date"</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t123" href="#t123">123</a></span><span class="t">    <span class="key">return</span> <span class="nam">TypedField</span><span class="op">(</span><span class="nam">dt</span><span class="op">.</span><span class="nam">date</span><span class="op">,</span> <span class="op">**</span><span class="nam">kw</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t122" href="#t122">122</a></span><span class="t">    <span class="nam">kw</span><span class="op">[</span><span class="str">"type"</span><span class="op">]</span> <span class="op">=</span> <span class="str">"date"</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t123" href="#t123">123</a></span><span class="t">    <span class="key">return</span> <span class="nam">TypedField</span><span class="op">(</span><span class="nam">dt</span><span class="op">.</span><span class="nam">date</span><span class="op">,</span> <span class="op">**</span><span class="nam">kw</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t124" href="#t124">124</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t125" href="#t125">125</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t126" href="#t126">126</a></span><span class="t"><span class="nam">Date</span> <span class="op">=</span> <span class="nam">DateField</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t127" href="#t127">127</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t128" href="#t128">128</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t129" href="#t129">129</a></span><span class="t"><span class="key">def</span> <span class="nam">TimeField</span><span class="op">(</span><span class="op">**</span><span class="nam">kw</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">)</span> <span class="op">-></span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Type</span><span class="op">[</span><span class="nam">dt</span><span class="op">.</span><span class="nam">time</span><span class="op">]</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t130" href="#t130">130</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t131" href="#t131">131</a></span><span class="t"><span class="str">    Pydal type is time, Python type is datetime.time.</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t132" href="#t132">132</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t133" href="#t133">133</a></span><span class="t">    <span class="nam">kw</span><span class="op">[</span><span class="str">"type"</span><span class="op">]</span> <span class="op">=</span> <span class="str">"time"</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t134" href="#t134">134</a></span><span class="t">    <span class="key">return</span> <span class="nam">TypedField</span><span class="op">(</span><span class="nam">dt</span><span class="op">.</span><span class="nam">time</span><span class="op">,</span> <span class="op">**</span><span class="nam">kw</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t133" href="#t133">133</a></span><span class="t">    <span class="nam">kw</span><span class="op">[</span><span class="str">"type"</span><span class="op">]</span> <span class="op">=</span> <span class="str">"time"</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t134" href="#t134">134</a></span><span class="t">    <span class="key">return</span> <span class="nam">TypedField</span><span class="op">(</span><span class="nam">dt</span><span class="op">.</span><span class="nam">time</span><span class="op">,</span> <span class="op">**</span><span class="nam">kw</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t135" href="#t135">135</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t136" href="#t136">136</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t137" href="#t137">137</a></span><span class="t"><span class="nam">Time</span> <span class="op">=</span> <span class="nam">TimeField</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t138" href="#t138">138</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t139" href="#t139">139</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t140" href="#t140">140</a></span><span class="t"><span class="key">def</span> <span class="nam">DatetimeField</span><span class="op">(</span><span class="op">**</span><span class="nam">kw</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">)</span> <span class="op">-></span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Type</span><span class="op">[</span><span class="nam">dt</span><span class="op">.</span><span class="nam">datetime</span><span class="op">]</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t141" href="#t141">141</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t142" href="#t142">142</a></span><span class="t"><span class="str">    Pydal type is datetime, Python type is datetime.datetime.</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t143" href="#t143">143</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t144" href="#t144">144</a></span><span class="t">    <span class="nam">kw</span><span class="op">[</span><span class="str">"type"</span><span class="op">]</span> <span class="op">=</span> <span class="str">"datetime"</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t145" href="#t145">145</a></span><span class="t">    <span class="key">return</span> <span class="nam">TypedField</span><span class="op">(</span><span class="nam">dt</span><span class="op">.</span><span class="nam">datetime</span><span class="op">,</span> <span class="op">**</span><span class="nam">kw</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t144" href="#t144">144</a></span><span class="t">    <span class="nam">kw</span><span class="op">[</span><span class="str">"type"</span><span class="op">]</span> <span class="op">=</span> <span class="str">"datetime"</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t145" href="#t145">145</a></span><span class="t">    <span class="key">return</span> <span class="nam">TypedField</span><span class="op">(</span><span class="nam">dt</span><span class="op">.</span><span class="nam">datetime</span><span class="op">,</span> <span class="op">**</span><span class="nam">kw</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t146" href="#t146">146</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t147" href="#t147">147</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t148" href="#t148">148</a></span><span class="t"><span class="nam">Datetime</span> <span class="op">=</span> <span class="nam">DatetimeField</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t149" href="#t149">149</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t150" href="#t150">150</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t151" href="#t151">151</a></span><span class="t"><span class="key">def</span> <span class="nam">PasswordField</span><span class="op">(</span><span class="op">**</span><span class="nam">kw</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">)</span> <span class="op">-></span> <span class="nam">TYPE_STR</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t152" href="#t152">152</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t153" href="#t153">153</a></span><span class="t"><span class="str">    Pydal type is password, Python type is str.</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t154" href="#t154">154</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t155" href="#t155">155</a></span><span class="t">    <span class="nam">kw</span><span class="op">[</span><span class="str">"type"</span><span class="op">]</span> <span class="op">=</span> <span class="str">"password"</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t156" href="#t156">156</a></span><span class="t">    <span class="key">return</span> <span class="nam">TypedField</span><span class="op">(</span><span class="nam">str</span><span class="op">,</span> <span class="op">**</span><span class="nam">kw</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t155" href="#t155">155</a></span><span class="t">    <span class="nam">kw</span><span class="op">[</span><span class="str">"type"</span><span class="op">]</span> <span class="op">=</span> <span class="str">"password"</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t156" href="#t156">156</a></span><span class="t">    <span class="key">return</span> <span class="nam">TypedField</span><span class="op">(</span><span class="nam">str</span><span class="op">,</span> <span class="op">**</span><span class="nam">kw</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t157" href="#t157">157</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t158" href="#t158">158</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t159" href="#t159">159</a></span><span class="t"><span class="nam">Password</span> <span class="op">=</span> <span class="nam">PasswordField</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t160" href="#t160">160</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t161" href="#t161">161</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t162" href="#t162">162</a></span><span class="t"><span class="key">def</span> <span class="nam">UploadField</span><span class="op">(</span><span class="op">**</span><span class="nam">kw</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">)</span> <span class="op">-></span> <span class="nam">TYPE_STR</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t163" href="#t163">163</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t164" href="#t164">164</a></span><span class="t"><span class="str">    Pydal type is upload, Python type is str.</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t165" href="#t165">165</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t166" href="#t166">166</a></span><span class="t">    <span class="nam">kw</span><span class="op">[</span><span class="str">"type"</span><span class="op">]</span> <span class="op">=</span> <span class="str">"upload"</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t167" href="#t167">167</a></span><span class="t">    <span class="key">return</span> <span class="nam">TypedField</span><span class="op">(</span><span class="nam">str</span><span class="op">,</span> <span class="op">**</span><span class="nam">kw</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t166" href="#t166">166</a></span><span class="t">    <span class="nam">kw</span><span class="op">[</span><span class="str">"type"</span><span class="op">]</span> <span class="op">=</span> <span class="str">"upload"</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t167" href="#t167">167</a></span><span class="t">    <span class="key">return</span> <span class="nam">TypedField</span><span class="op">(</span><span class="nam">str</span><span class="op">,</span> <span class="op">**</span><span class="nam">kw</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t168" href="#t168">168</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t169" href="#t169">169</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t170" href="#t170">170</a></span><span class="t"><span class="nam">Upload</span> <span class="op">=</span> <span class="nam">UploadField</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t171" href="#t171">171</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t172" href="#t172">172</a></span><span class="t"><span class="nam">T_subclass</span> <span class="op">=</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">TypeVar</span><span class="op">(</span><span class="str">"T_subclass"</span><span class="op">,</span> <span class="nam">TypedTable</span><span class="op">,</span> <span class="nam">Table</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t173" href="#t173">173</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t174" href="#t174">174</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t175" href="#t175">175</a></span><span class="t"><span class="key">def</span> <span class="nam">ReferenceField</span><span class="op">(</span><span class="nam">other_table</span><span class="op">:</span> <span class="nam">str</span> <span class="op">|</span> <span class="nam">TypedTable</span> <span class="op">|</span> <span class="nam">Table</span> <span class="op">|</span> <span class="nam">T_subclass</span><span class="op">,</span> <span class="op">**</span><span class="nam">kw</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">)</span> <span class="op">-></span> <span class="nam">TYPE_INT</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t176" href="#t176">176</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t177" href="#t177">177</a></span><span class="t"><span class="str">    Pydal type is reference, Python type is int (id).</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t178" href="#t178">178</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t179" href="#t179">179</a></span><span class="t">    <span class="key">if</span> <span class="nam">isinstance</span><span class="op">(</span><span class="nam">other_table</span><span class="op">,</span> <span class="nam">str</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t180" href="#t180">180</a></span><span class="t">        <span class="nam">kw</span><span class="op">[</span><span class="str">"type"</span><span class="op">]</span> <span class="op">=</span> <span class="str">f"reference {other_table}"</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t181" href="#t181">181</a></span><span class="t">    <span class="key">elif</span> <span class="nam">isinstance</span><span class="op">(</span><span class="nam">other_table</span><span class="op">,</span> <span class="nam">Table</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t179" href="#t179">179</a></span><span class="t">    <span class="key">if</span> <span class="nam">isinstance</span><span class="op">(</span><span class="nam">other_table</span><span class="op">,</span> <span class="nam">str</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t180" href="#t180">180</a></span><span class="t">        <span class="nam">kw</span><span class="op">[</span><span class="str">"type"</span><span class="op">]</span> <span class="op">=</span> <span class="str">f"reference {other_table}"</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t181" href="#t181">181</a></span><span class="t">    <span class="key">elif</span> <span class="nam">isinstance</span><span class="op">(</span><span class="nam">other_table</span><span class="op">,</span> <span class="nam">Table</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t182" href="#t182">182</a></span><span class="t">        <span class="com"># db.table</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t183" href="#t183">183</a></span><span class="t">        <span class="nam">kw</span><span class="op">[</span><span class="str">"type"</span><span class="op">]</span> <span class="op">=</span> <span class="str">f"reference {other_table._tablename}"</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t184" href="#t184">184</a></span><span class="t">    <span class="key">elif</span> <span class="nam">issubclass</span><span class="op">(</span><span class="nam">type</span><span class="op">(</span><span class="nam">other_table</span><span class="op">)</span><span class="op">,</span> <span class="nam">type</span><span class="op">)</span> <span class="key">and</span> <span class="nam">issubclass</span><span class="op">(</span><span class="nam">other_table</span><span class="op">,</span> <span class="nam">TypedTable</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t183" href="#t183">183</a></span><span class="t">        <span class="nam">kw</span><span class="op">[</span><span class="str">"type"</span><span class="op">]</span> <span class="op">=</span> <span class="str">f"reference {other_table._tablename}"</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t184" href="#t184">184</a></span><span class="t">    <span class="key">elif</span> <span class="nam">issubclass</span><span class="op">(</span><span class="nam">type</span><span class="op">(</span><span class="nam">other_table</span><span class="op">)</span><span class="op">,</span> <span class="nam">type</span><span class="op">)</span> <span class="key">and</span> <span class="nam">issubclass</span><span class="op">(</span><span class="nam">other_table</span><span class="op">,</span> <span class="nam">TypedTable</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t185" href="#t185">185</a></span><span class="t">        <span class="com"># SomeTable</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t186" href="#t186">186</a></span><span class="t">        <span class="nam">snakename</span> <span class="op">=</span> <span class="nam">TypeDAL</span><span class="op">.</span><span class="nam">_to_snake</span><span class="op">(</span><span class="nam">other_table</span><span class="op">.</span><span class="nam">__name__</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t187" href="#t187">187</a></span><span class="t">        <span class="nam">kw</span><span class="op">[</span><span class="str">"type"</span><span class="op">]</span> <span class="op">=</span> <span class="str">f"reference {snakename}"</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t186" href="#t186">186</a></span><span class="t">        <span class="nam">snakename</span> <span class="op">=</span> <span class="nam">TypeDAL</span><span class="op">.</span><span class="nam">_to_snake</span><span class="op">(</span><span class="nam">other_table</span><span class="op">.</span><span class="nam">__name__</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t187" href="#t187">187</a></span><span class="t">        <span class="nam">kw</span><span class="op">[</span><span class="str">"type"</span><span class="op">]</span> <span class="op">=</span> <span class="str">f"reference {snakename}"</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t188" href="#t188">188</a></span><span class="t">    <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t189" href="#t189">189</a></span><span class="t">        <span class="key">raise</span> <span class="nam">ValueError</span><span class="op">(</span><span class="str">f"Don't know what to do with {type(other_table)}"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t189" href="#t189">189</a></span><span class="t">        <span class="key">raise</span> <span class="nam">ValueError</span><span class="op">(</span><span class="str">f"Don't know what to do with {type(other_table)}"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t190" href="#t190">190</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t191" href="#t191">191</a></span><span class="t">    <span class="key">return</span> <span class="nam">TypedField</span><span class="op">(</span><span class="nam">int</span><span class="op">,</span> <span class="op">**</span><span class="nam">kw</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t191" href="#t191">191</a></span><span class="t">    <span class="key">return</span> <span class="nam">TypedField</span><span class="op">(</span><span class="nam">int</span><span class="op">,</span> <span class="op">**</span><span class="nam">kw</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t192" href="#t192">192</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t193" href="#t193">193</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t194" href="#t194">194</a></span><span class="t"><span class="nam">Reference</span> <span class="op">=</span> <span class="nam">ReferenceField</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t195" href="#t195">195</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t196" href="#t196">196</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t197" href="#t197">197</a></span><span class="t"><span class="key">def</span> <span class="nam">ListStringField</span><span class="op">(</span><span class="op">**</span><span class="nam">kw</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">)</span> <span class="op">-></span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Type</span><span class="op">[</span><span class="nam">list</span><span class="op">[</span><span class="nam">str</span><span class="op">]</span><span class="op">]</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t198" href="#t198">198</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t199" href="#t199">199</a></span><span class="t"><span class="str">    Pydal type is list:string, Python type is list of str.</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t200" href="#t200">200</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t201" href="#t201">201</a></span><span class="t">    <span class="nam">kw</span><span class="op">[</span><span class="str">"type"</span><span class="op">]</span> <span class="op">=</span> <span class="str">"list:string"</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t202" href="#t202">202</a></span><span class="t">    <span class="key">return</span> <span class="nam">TypedField</span><span class="op">(</span><span class="nam">list</span><span class="op">[</span><span class="nam">str</span><span class="op">]</span><span class="op">,</span> <span class="op">**</span><span class="nam">kw</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t201" href="#t201">201</a></span><span class="t">    <span class="nam">kw</span><span class="op">[</span><span class="str">"type"</span><span class="op">]</span> <span class="op">=</span> <span class="str">"list:string"</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t202" href="#t202">202</a></span><span class="t">    <span class="key">return</span> <span class="nam">TypedField</span><span class="op">(</span><span class="nam">list</span><span class="op">[</span><span class="nam">str</span><span class="op">]</span><span class="op">,</span> <span class="op">**</span><span class="nam">kw</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t203" href="#t203">203</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t204" href="#t204">204</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t205" href="#t205">205</a></span><span class="t"><span class="nam">ListString</span> <span class="op">=</span> <span class="nam">ListStringField</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t206" href="#t206">206</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t207" href="#t207">207</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t208" href="#t208">208</a></span><span class="t"><span class="key">def</span> <span class="nam">ListIntegerField</span><span class="op">(</span><span class="op">**</span><span class="nam">kw</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">)</span> <span class="op">-></span> <span class="nam">TYPE_LIST_OF_INT</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t209" href="#t209">209</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t210" href="#t210">210</a></span><span class="t"><span class="str">    Pydal type is list:integer, Python type is list of int.</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t211" href="#t211">211</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t212" href="#t212">212</a></span><span class="t">    <span class="nam">kw</span><span class="op">[</span><span class="str">"type"</span><span class="op">]</span> <span class="op">=</span> <span class="str">"list:integer"</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t213" href="#t213">213</a></span><span class="t">    <span class="key">return</span> <span class="nam">TypedField</span><span class="op">(</span><span class="nam">list</span><span class="op">[</span><span class="nam">int</span><span class="op">]</span><span class="op">,</span> <span class="op">**</span><span class="nam">kw</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t212" href="#t212">212</a></span><span class="t">    <span class="nam">kw</span><span class="op">[</span><span class="str">"type"</span><span class="op">]</span> <span class="op">=</span> <span class="str">"list:integer"</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t213" href="#t213">213</a></span><span class="t">    <span class="key">return</span> <span class="nam">TypedField</span><span class="op">(</span><span class="nam">list</span><span class="op">[</span><span class="nam">int</span><span class="op">]</span><span class="op">,</span> <span class="op">**</span><span class="nam">kw</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t214" href="#t214">214</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t215" href="#t215">215</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t216" href="#t216">216</a></span><span class="t"><span class="nam">ListInteger</span> <span class="op">=</span> <span class="nam">ListIntegerField</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t217" href="#t217">217</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t218" href="#t218">218</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t219" href="#t219">219</a></span><span class="t"><span class="key">def</span> <span class="nam">ListReferenceField</span><span class="op">(</span><span class="nam">other_table</span><span class="op">:</span> <span class="nam">str</span><span class="op">,</span> <span class="op">**</span><span class="nam">kw</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">)</span> <span class="op">-></span> <span class="nam">TYPE_LIST_OF_INT</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t220" href="#t220">220</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t221" href="#t221">221</a></span><span class="t"><span class="str">    Pydal type is list:reference, Python type is list of int (id).</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t222" href="#t222">222</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t223" href="#t223">223</a></span><span class="t">    <span class="nam">kw</span><span class="op">[</span><span class="str">"type"</span><span class="op">]</span> <span class="op">=</span> <span class="str">f"list:reference {other_table}"</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t224" href="#t224">224</a></span><span class="t">    <span class="key">return</span> <span class="nam">TypedField</span><span class="op">(</span><span class="nam">list</span><span class="op">[</span><span class="nam">int</span><span class="op">]</span><span class="op">,</span> <span class="op">**</span><span class="nam">kw</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t223" href="#t223">223</a></span><span class="t">    <span class="nam">kw</span><span class="op">[</span><span class="str">"type"</span><span class="op">]</span> <span class="op">=</span> <span class="str">f"list:reference {other_table}"</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t224" href="#t224">224</a></span><span class="t">    <span class="key">return</span> <span class="nam">TypedField</span><span class="op">(</span><span class="nam">list</span><span class="op">[</span><span class="nam">int</span><span class="op">]</span><span class="op">,</span> <span class="op">**</span><span class="nam">kw</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t225" href="#t225">225</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t226" href="#t226">226</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t227" href="#t227">227</a></span><span class="t"><span class="nam">ListReference</span> <span class="op">=</span> <span class="nam">ListReferenceField</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t228" href="#t228">228</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t229" href="#t229">229</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t230" href="#t230">230</a></span><span class="t"><span class="key">def</span> <span class="nam">JSONField</span><span class="op">(</span><span class="op">**</span><span class="nam">kw</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">)</span> <span class="op">-></span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Type</span><span class="op">[</span><span class="nam">object</span><span class="op">]</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t231" href="#t231">231</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t232" href="#t232">232</a></span><span class="t"><span class="str">    Pydal type is json, Python type is object (can be anything JSON-encodable).</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t233" href="#t233">233</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t234" href="#t234">234</a></span><span class="t">    <span class="nam">kw</span><span class="op">[</span><span class="str">"type"</span><span class="op">]</span> <span class="op">=</span> <span class="str">"json"</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t235" href="#t235">235</a></span><span class="t">    <span class="key">return</span> <span class="nam">TypedField</span><span class="op">(</span><span class="nam">object</span><span class="op">,</span> <span class="op">**</span><span class="nam">kw</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t234" href="#t234">234</a></span><span class="t">    <span class="nam">kw</span><span class="op">[</span><span class="str">"type"</span><span class="op">]</span> <span class="op">=</span> <span class="str">"json"</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t235" href="#t235">235</a></span><span class="t">    <span class="key">return</span> <span class="nam">TypedField</span><span class="op">(</span><span class="nam">object</span><span class="op">,</span> <span class="op">**</span><span class="nam">kw</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t236" href="#t236">236</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t237" href="#t237">237</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t238" href="#t238">238</a></span><span class="t"><span class="key">def</span> <span class="nam">BigintField</span><span class="op">(</span><span class="op">**</span><span class="nam">kw</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">)</span> <span class="op">-></span> <span class="nam">TYPE_INT</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t239" href="#t239">239</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t240" href="#t240">240</a></span><span class="t"><span class="str">    Pydal type is bigint, Python type is int.</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t241" href="#t241">241</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t242" href="#t242">242</a></span><span class="t">    <span class="nam">kw</span><span class="op">[</span><span class="str">"type"</span><span class="op">]</span> <span class="op">=</span> <span class="str">"bigint"</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t243" href="#t243">243</a></span><span class="t">    <span class="key">return</span> <span class="nam">TypedField</span><span class="op">(</span><span class="nam">int</span><span class="op">,</span> <span class="op">**</span><span class="nam">kw</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t242" href="#t242">242</a></span><span class="t">    <span class="nam">kw</span><span class="op">[</span><span class="str">"type"</span><span class="op">]</span> <span class="op">=</span> <span class="str">"bigint"</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t243" href="#t243">243</a></span><span class="t">    <span class="key">return</span> <span class="nam">TypedField</span><span class="op">(</span><span class="nam">int</span><span class="op">,</span> <span class="op">**</span><span class="nam">kw</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t244" href="#t244">244</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t245" href="#t245">245</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t246" href="#t246">246</a></span><span class="t"><span class="nam">Bigint</span> <span class="op">=</span> <span class="nam">BigintField</span>&nbsp;</span><span class="r"></span></p>
 </main>
 <footer>
     <div class="content">
         <p>
             <a id="prevFileLink" class="nav" href="d_0ccc93afd6526b6c_core_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="index.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-06-05 16:09 +0200
+            created at 2023-06-22 10:11 +0200
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -1,21 +1,21 @@
 
-****** Coverage for src/typedal/fields.py: 100% ******
+****** Coverage for src/typedal/fields.py: 55% ******
  ⁰  [Show/hide keyboard shortcuts]
 Shortcuts on this page
 r m x   toggle line displays
 j k   next/prev highlighted chunk
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
-***** 91 statements   91 run 0 missing 0 excluded *****
+***** 91 statements   50 run 41 missing 0 excluded *****
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.7, created
-at 2023-06-05 16:09 +0200
+at 2023-06-22 10:11 +0200
 
 
 1""" 
 2This file contains available Field types. 
 3""" 
 4 
 5import datetime as dt 
@@ -263,8 +263,8 @@
 242 kw["type"] = "bigint" 
 243 return TypedField(int, **kw) 
 244 
 245 
 246Bigint = BigintField 
 
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.7, created
-at 2023-06-05 16:09 +0200
+at 2023-06-22 10:11 +0200
```

### Comparing `typedal-1.0.0b1/htmlcov/favicon_32.png` & `typedal-1.1.1/htmlcov/favicon_32.png`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/htmlcov/index.html` & `typedal-1.1.1/htmlcov/index.html`

 * *Files 6% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     <link rel="stylesheet" href="style.css" type="text/css">
     <script type="text/javascript" src="coverage_html.js" defer></script>
 </head>
 <body class="indexfile">
 <header>
     <div class="content">
         <h1>Coverage report:
-            <span class="pc_cov">100%</span>
+            <span class="pc_cov">63%</span>
         </h1>
         <aside id="help_panel_wrapper">
             <input id="help_panel_state" type="checkbox">
             <label for="help_panel_state">
                 <img id="keyboard_icon" src="keybd_closed.png" alt="Show/hide keyboard shortcuts" />
             </label>
             <div id="help_panel">
@@ -41,15 +41,15 @@
             </div>
         </aside>
         <form id="filter_container">
             <input id="filter" type="text" value="" placeholder="filter..." />
         </form>
         <p class="text">
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-06-05 16:10 +0200
+            created at 2023-06-22 10:11 +0200
         </p>
     </div>
 </header>
 <main id="index">
     <table class="index" data-sortable>
         <thead>
             <tr class="tablehead" title="Click to sort">
@@ -73,46 +73,46 @@
                 <td>3</td>
                 <td>0</td>
                 <td>0</td>
                 <td class="right" data-ratio="3 3">100%</td>
             </tr>
             <tr class="file">
                 <td class="name left"><a href="d_0ccc93afd6526b6c_core_py.html">src/typedal/core.py</a></td>
-                <td>119</td>
-                <td>0</td>
+                <td>124</td>
+                <td>41</td>
                 <td>2</td>
-                <td class="right" data-ratio="119 119">100%</td>
+                <td class="right" data-ratio="83 124">67%</td>
             </tr>
             <tr class="file">
                 <td class="name left"><a href="d_0ccc93afd6526b6c_fields_py.html">src/typedal/fields.py</a></td>
                 <td>91</td>
+                <td>41</td>
                 <td>0</td>
-                <td>0</td>
-                <td class="right" data-ratio="91 91">100%</td>
+                <td class="right" data-ratio="50 91">55%</td>
             </tr>
         </tbody>
         <tfoot>
             <tr class="total">
                 <td class="name left">Total</td>
-                <td>214</td>
-                <td>0</td>
+                <td>219</td>
+                <td>82</td>
                 <td>2</td>
-                <td class="right" data-ratio="214 214">100%</td>
+                <td class="right" data-ratio="137 219">63%</td>
             </tr>
         </tfoot>
     </table>
     <p id="no_rows">
         No items found using the specified filter.
     </p>
 </main>
 <footer>
     <div class="content">
         <p>
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-06-05 16:10 +0200
+            created at 2023-06-22 10:11 +0200
         </p>
     </div>
     <aside class="hidden">
         <a id="prevFileLink" class="nav" href="d_0ccc93afd6526b6c_fields_py.html"/>
         <a id="nextFileLink" class="nav" href="d_0ccc93afd6526b6c___about___py.html"/>
         <button type="button" class="button_prev_file" data-shortcut="["/>
         <button type="button" class="button_next_file" data-shortcut="]"/>
```

#### html2text {}

```diff
@@ -1,20 +1,20 @@
 
-****** Coverage report: 100% ******
+****** Coverage report: 63% ******
  ⁰  [Show/hide keyboard shortcuts]
 Shortcuts on this page
 n s m x c   change column sorting
 [ ]   prev/next file
 ?   show/hide this help
 [                    ]
-coverage.py_v7.2.7, created at 2023-06-05 16:10 +0200
+coverage.py_v7.2.7, created at 2023-06-22 10:11 +0200
 
 Module                   statements missing excluded coverage
 src/typedal/__about__.py 1          0       0        100%
 src/typedal/__init__.py  3          0       0        100%
-src/typedal/core.py      119        0       2        100%
-src/typedal/fields.py    91         0       0        100%
-Total                    214        0       2        100%
+src/typedal/core.py      124        41      2        67%
+src/typedal/fields.py    91         41      0        55%
+Total                    219        82      2        63%
 No items found using the specified filter.
 
-coverage.py_v7.2.7, created at 2023-06-05 16:10 +0200
+coverage.py_v7.2.7, created at 2023-06-22 10:11 +0200
  ____
```

### Comparing `typedal-1.0.0b1/htmlcov/keybd_closed.png` & `typedal-1.1.1/htmlcov/keybd_closed.png`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/htmlcov/keybd_open.png` & `typedal-1.1.1/htmlcov/keybd_open.png`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/htmlcov/style.css` & `typedal-1.1.1/htmlcov/style.css`

 * *Files identical despite different names*

### Comparing `typedal-1.0.0b1/src/typedal/core.py` & `typedal-1.1.1/src/typedal/core.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 Core functionality of TypeDAL.
 """
-
 import datetime as dt
 import types
 import typing
+from collections import ChainMap
 from decimal import Decimal
 
 import pydal
 from pydal.objects import Field, Query, Row, Rows, Table
 
 # use typing.cast(type, ...) to make mypy happy with unions
 T_annotation = typing.Type[typing.Any] | types.UnionType
@@ -46,22 +46,43 @@
     Args:
         some_type: types.UnionType = type(int | str); typing.Union = typing.Union[int, str]
 
     """
     return typing.get_origin(some_type) in (types.UnionType, typing.Union)
 
 
+def _all_annotations(cls: type) -> ChainMap[str, type]:
+    """
+    Returns a dictionary-like ChainMap that includes annotations for all \
+    attributes defined in cls or inherited from superclasses.
+    """
+    return ChainMap(*(c.__annotations__ for c in getattr(cls, "__mro__", []) if "__annotations__" in c.__dict__))
+
+
+def all_annotations(cls: type, _except: typing.Iterable[str] = None) -> dict[str, type]:
+    """
+    Wrapper around `_all_annotations` that filters away any keys in _except.
+
+    It also flattens the ChainMap to a regular dict.
+    """
+    if _except is None:
+        _except = set()
+
+    _all = _all_annotations(cls)
+    return {k: v for k, v in _all.items() if k not in _except}
+
+
 class TypeDAL(pydal.DAL):  # type: ignore
     """
     Drop-in replacement for pyDAL with layer to convert class-based table definitions to classical pydal define_tables.
     """
 
     dal: Table
 
-    default_kwargs = {
+    default_kwargs: typing.ClassVar[typing.Dict[str, typing.Any]] = {
         # fields are 'required' (notnull) by default:
         "notnull": True,
     }
 
     def define(self, cls: T) -> Table:
         """
         Can be used as a decorator on a class that inherits `TypedTable`, \
@@ -93,16 +114,23 @@
         # this however also stops working when variables outside this scope or even references to other
         # objects are used. So for now, this package will NOT work when from __future__ import annotations is used,
         # and might break in the future, when this annotations behavior is enabled by default.
 
         # non-annotated variables have to be passed to define_table as kwargs
 
         tablename = self._to_snake(cls.__name__)
-        fields = [self._to_field(fname, ftype) for fname, ftype in cls.__annotations__.items()]
-        other_kwargs = {k: v for k, v in cls.__dict__.items() if k not in cls.__annotations__ and not k.startswith("_")}
+        # grab annotations of cls and it's parents:
+        annotations = all_annotations(cls)
+        # extend with `prop = TypedField()` 'annotations':
+        annotations |= {k: v for k, v in cls.__dict__.items() if isinstance(v, TypedFieldType)}
+        # remove internal stuff:
+        annotations = {k: v for k, v in annotations.items() if not k.startswith("_")}
+
+        fields = [self._to_field(fname, ftype) for fname, ftype in annotations.items()]
+        other_kwargs = {k: v for k, v in cls.__dict__.items() if k not in annotations and not k.startswith("_")}
 
         table: Table = self.define_table(tablename, *fields, **other_kwargs)
 
         cls.__set_internals__(db=self, table=table)
 
         # the ACTUAL output is not TypedTable but rather pydal.Table
         # but telling the editor it is T helps with hinting.
@@ -196,20 +224,19 @@
                 id: int
                 name: str
                 reference: Table
                 other: TypedField(str, default="John Doe")  # default will be in kwargs
         """
         fname = cls._to_snake(fname)
 
-        converted_type = cls._annotation_to_pydal_fieldtype(ftype, kw)
-        if not converted_type:
+        if converted_type := cls._annotation_to_pydal_fieldtype(ftype, kw):
+            return cls._build_field(fname, converted_type, **kw)
+        else:
             raise NotImplementedError(f"Unsupported type {ftype}/{type(ftype)}")
 
-        return cls._build_field(fname, converted_type, **kw)
-
     @staticmethod
     def _to_snake(camel: str) -> str:
         # https://stackoverflow.com/a/44969381
         return "".join([f"_{c.lower()}" if c.isupper() else c for c in camel]).lstrip("_")
 
 
 class TypedTableMeta(type):
```

### Comparing `typedal-1.0.0b1/src/typedal/fields.py` & `typedal-1.1.1/src/typedal/fields.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,176 +7,171 @@
 import types
 import typing
 
 from pydal.objects import Table
 
 from .core import TypeDAL, TypedFieldType, TypedTable
 
-T = typing.TypeVar("T", bound=typing.Type[typing.Any])
+T = typing.TypeVar("T", bound=typing.Any)
 
 
 ## general
 
 
 def TypedField(
-    _type: T | types.UnionType,
+    _type: typing.Type[T] | types.UnionType,
     **kwargs: typing.Any,
 ) -> T:
     """
     sneaky: its a function and not a class, because there's a return type.
 
     and the return type (T) is the input type in _type
 
     Example:
         age: TypedField(int, default=18)
     """
-    return TypedFieldType(_type, **kwargs)
-
-
-TYPE_STR = typing.Type[str]
-TYPE_INT = typing.Type[int]
-TYPE_LIST_OF_INT = typing.Type[list[int]]
+    return typing.cast(T, TypedFieldType(_type, **kwargs))
 
 
 ## specific
-def StringField(**kw: typing.Any) -> TYPE_STR:
+def StringField(**kw: typing.Any) -> str:
     """
     Pydal type is string, Python type is str.
     """
     kw["type"] = "string"
     return TypedField(str, **kw)
 
 
 String = StringField
 
 
-def TextField(**kw: typing.Any) -> TYPE_STR:
+def TextField(**kw: typing.Any) -> str:
     """
     Pydal type is text, Python type is str.
     """
     kw["type"] = "text"
     return TypedField(str, **kw)
 
 
 Text = TextField
 
 
-def BlobField(**kw: typing.Any) -> typing.Type[bytes]:
+def BlobField(**kw: typing.Any) -> bytes:
     """
     Pydal type is blob, Python type is bytes.
     """
     kw["type"] = "blob"
     return TypedField(bytes, **kw)
 
 
 Blob = BlobField
 
 
-def BooleanField(**kw: typing.Any) -> typing.Type[bool]:
+def BooleanField(**kw: typing.Any) -> bool:
     """
     Pydal type is boolean, Python type is bool.
     """
     kw["type"] = "boolean"
     return TypedField(bool, **kw)
 
 
 Boolean = BooleanField
 
 
-def IntegerField(**kw: typing.Any) -> typing.Type[int]:
+def IntegerField(**kw: typing.Any) -> int:
     """
     Pydal type is integer, Python type is int.
     """
     kw["type"] = "integer"
     return TypedField(int, **kw)
 
 
 Integer = IntegerField
 
 
-def DoubleField(**kw: typing.Any) -> typing.Type[float]:
+def DoubleField(**kw: typing.Any) -> float:
     """
     Pydal type is double, Python type is float.
     """
     kw["type"] = "double"
     return TypedField(float, **kw)
 
 
 Double = DoubleField
 
 
-def DecimalField(n: int, m: int, **kw: typing.Any) -> typing.Type[decimal.Decimal]:
+def DecimalField(n: int, m: int, **kw: typing.Any) -> decimal.Decimal:
     """
     Pydal type is decimal, Python type is Decimal.
     """
     kw["type"] = f"decimal({n}, {m})"
     return TypedField(decimal.Decimal, **kw)
 
 
 Decimal = DecimalField
 
 
-def DateField(**kw: typing.Any) -> typing.Type[dt.date]:
+def DateField(**kw: typing.Any) -> dt.date:
     """
     Pydal type is date, Python type is datetime.date.
     """
     kw["type"] = "date"
     return TypedField(dt.date, **kw)
 
 
 Date = DateField
 
 
-def TimeField(**kw: typing.Any) -> typing.Type[dt.time]:
+def TimeField(**kw: typing.Any) -> dt.time:
     """
     Pydal type is time, Python type is datetime.time.
     """
     kw["type"] = "time"
     return TypedField(dt.time, **kw)
 
 
 Time = TimeField
 
 
-def DatetimeField(**kw: typing.Any) -> typing.Type[dt.datetime]:
+def DatetimeField(**kw: typing.Any) -> dt.datetime:
     """
     Pydal type is datetime, Python type is datetime.datetime.
     """
     kw["type"] = "datetime"
     return TypedField(dt.datetime, **kw)
 
 
 Datetime = DatetimeField
 
 
-def PasswordField(**kw: typing.Any) -> TYPE_STR:
+def PasswordField(**kw: typing.Any) -> str:
     """
     Pydal type is password, Python type is str.
     """
     kw["type"] = "password"
     return TypedField(str, **kw)
 
 
 Password = PasswordField
 
 
-def UploadField(**kw: typing.Any) -> TYPE_STR:
+def UploadField(**kw: typing.Any) -> str:
     """
     Pydal type is upload, Python type is str.
     """
     kw["type"] = "upload"
     return TypedField(str, **kw)
 
 
 Upload = UploadField
 
 T_subclass = typing.TypeVar("T_subclass", TypedTable, Table)
 
 
-def ReferenceField(other_table: str | TypedTable | Table | T_subclass, **kw: typing.Any) -> TYPE_INT:
+def ReferenceField(other_table: str | TypedTable | Table | T_subclass, **kw: typing.Any) -> int:
     """
     Pydal type is reference, Python type is int (id).
     """
     if isinstance(other_table, str):
         kw["type"] = f"reference {other_table}"
     elif isinstance(other_table, Table):
         # db.table
@@ -190,56 +185,56 @@
 
     return TypedField(int, **kw)
 
 
 Reference = ReferenceField
 
 
-def ListStringField(**kw: typing.Any) -> typing.Type[list[str]]:
+def ListStringField(**kw: typing.Any) -> list[str]:
     """
     Pydal type is list:string, Python type is list of str.
     """
     kw["type"] = "list:string"
     return TypedField(list[str], **kw)
 
 
 ListString = ListStringField
 
 
-def ListIntegerField(**kw: typing.Any) -> TYPE_LIST_OF_INT:
+def ListIntegerField(**kw: typing.Any) -> list[int]:
     """
     Pydal type is list:integer, Python type is list of int.
     """
     kw["type"] = "list:integer"
     return TypedField(list[int], **kw)
 
 
 ListInteger = ListIntegerField
 
 
-def ListReferenceField(other_table: str, **kw: typing.Any) -> TYPE_LIST_OF_INT:
+def ListReferenceField(other_table: str, **kw: typing.Any) -> list[int]:
     """
     Pydal type is list:reference, Python type is list of int (id).
     """
     kw["type"] = f"list:reference {other_table}"
     return TypedField(list[int], **kw)
 
 
 ListReference = ListReferenceField
 
 
-def JSONField(**kw: typing.Any) -> typing.Type[object]:
+def JSONField(**kw: typing.Any) -> object:
     """
     Pydal type is json, Python type is object (can be anything JSON-encodable).
     """
     kw["type"] = "json"
     return TypedField(object, **kw)
 
 
-def BigintField(**kw: typing.Any) -> TYPE_INT:
+def BigintField(**kw: typing.Any) -> int:
     """
     Pydal type is bigint, Python type is int.
     """
     kw["type"] = "bigint"
     return TypedField(int, **kw)
```

### Comparing `typedal-1.0.0b1/tests/test_main.py` & `typedal-1.1.1/tests/test_main.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,39 +50,39 @@
     @db.define
     class FirstNewSyntax(TypedTable):
         # simple:
         name: str
         # optional: (sets required=False and notnull=False)
         age: float | None
         # with extra options (and non-native type 'text'):
-        location: TypedField(str, type="text", default="Amsterdam")
+        location = TypedField(str, type="text", default="Amsterdam")
         # references:
         # can only be made optional with typing.Optional, not '| None'
         first_new_relation: typing.Optional[NewRelation]
         second_new_relation: typing.Optional[SecondNewRelation]
         # backwards compatible:
         old_relation: typing.Optional[db.relation]
         # generics:
         tags: list[str]
 
     # instead of using just a native type, TypedField can also always be used:
     class SecondNewSyntax(TypedTable):
         # simple:
-        name: TypedField(str)
+        name = TypedField(str)
         # optional: (sets required=False and notnull=False)
         # note: TypedField can NOT be used with typing.Optional or '| None' !!
-        age: TypedField(float, notnull=False)
+        age = TypedField(float, notnull=False)
         # with extra options (and non-native type 'text'):
-        location: TextField(default="Rotterdam")
-        first_new_relation: ReferenceField(NewRelation)
-        second_new_relation: ReferenceField(db.second_new_relation)
+        location = TextField(default="Rotterdam")
+        first_new_relation = ReferenceField(NewRelation)
+        second_new_relation = ReferenceField(db.second_new_relation)
         # backwards compatible:
-        old_relation: TypedField(db.relation, notnull=False)
+        old_relation = TypedField(db.relation, notnull=False)
         # generics:
-        tags: TypedField(list[str])
+        tags = TypedField(list[str])
 
     db.define(SecondNewSyntax)
 
     ### INSERTS
     db.relation.insert()
 
     db.new_relation.insert()
@@ -144,14 +144,16 @@
     assert SecondNewSyntax(id=1) is not None
     assert SecondNewSyntax(1) is not None
     assert SecondNewSyntax(id=2) is None
     assert SecondNewSyntax(2) is None
     _print_and_assert_len(db(SecondNewSyntax).select().as_list(), 1)
     _print_and_assert_len(db(SecondNewSyntax.id > 0).select().as_list(), 1)
 
+    assert SecondNewSyntax(1).location == "Rotterdam"
+
 
 def test_invalid_union():
     with pytest.raises(NotImplementedError):
         @db.define
         class Invalid(TypedTable):
             valid: int | None
             invalid: int | str
@@ -187,28 +189,28 @@
     assert str(TextField()) == "TypedField.text"
     assert repr(TextField()) == "<TypedField.text with options {}>"
 
 
 def test_typedfield_to_field_type():
     @db.define
     class SomeTable(TypedTable):
-        name: TypedField(str)  # basic mapping
+        name = TypedField(str)  # basic mapping
 
     @db.define
     class OtherTable(TypedTable):
-        second: ReferenceField(SomeTable)  # reference to TypedTable
-        third: ReferenceField(db.some_table)  # reference to pydal table
-        third: TypedField(list[str])  # generic alias
-        optional_one: TypedField(typing.Optional[str])
-        optional_two: TypedField(str | None)
+        second = ReferenceField(SomeTable)  # reference to TypedTable
+        third = ReferenceField(db.some_table)  # reference to pydal table
+        fourth = TypedField(list[str])  # generic alias
+        optional_one = TypedField(typing.Optional[str])
+        optional_two = TypedField(str | None)
 
     with pytest.raises(NotImplementedError):
         @db.define
         class Invalid(TypedTable):
-            third: TypedField(dict[str, int])  # not supported
+            third = TypedField(dict[str, int])  # not supported
 
 
 def test_fields():
     @db.define
     class SomeNewTable(TypedTable):
         name: str
```

### Comparing `typedal-1.0.0b1/README.md` & `typedal-1.1.1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # TypeDAL
 
-[![PyPI - Version](https://img.shields.io/pypi/v/TypeDal.svg)](https://pypi.org/project/typedal)
-[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/TypeDal.svg)](https://pypi.org/project/typedal)  
+[![PyPI - Version](https://img.shields.io/pypi/v/TypeDAL.svg)](https://pypi.org/project/TypeDAL)
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/TypeDAL.svg)](https://pypi.org/project/TypeDAL)  
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)  
-[![su6 checks](https://github.com/trialandsuccess/typedal/actions/workflows/su6.yml/badge.svg)](https://github.com/trialandsuccess/typedal/actions)
+[![su6 checks](https://github.com/trialandsuccess/TypeDAL/actions/workflows/su6.yml/badge.svg?branch=development)](https://github.com/trialandsuccess/TypeDAL/actions)
 ![coverage.svg](coverage.svg)
 
 Typing support for [PyDAL](http://web2py.com/books/default/chapter/29/6).
 This package aims to improve the typing support for PyDAL. By using classes instead of the define_table method,
 type hinting the result of queries can improve the experience while developing. In the background, the queries are still
 generated and executed by pydal itself, this package only proves some logic to properly pass calls from class methods to
 the underlying `db.define_table` pydal Tables.
 
 - `TypeDAL` is the replacement class for DAL that manages the code on top of DAL.
 - `TypedTable` must be the parent class of any custom Tables you define (e.g. `class SomeTable(TypedTable)`)
 - `TypedField` can be used instead of Python native types when extra settings (such as default) are required (
-  e.g. `name: TypedField(str, default="John Doe")`)
+  e.g. `name = TypedField(str, default="John Doe")`)
 - `TypedRows`: can be used as the return type of .select() and subscribed with the actual table class, so
   e.g. `rows: TypedRows[SomeTable]`. If you're lazy, `list[SomeTable]` works fine too but that misses hinting
   possibilities such as `.first()`.
 
 ### Translations from pydal to typedal
 
 <table>
@@ -74,29 +74,29 @@
 <td>
 
 ```python
 @db.define
 class TableName(TypedTable):
     fieldname: str
     otherfield: float | None
-    yet_another: TypedField(str, type="text", default="something", required=False)
+    yet_another = TypedField(str, type="text", default="something", required=False)
 ```
 
 </td>
 
 <td>
 
 ```python
 import typing
 
 
 class TableName(TypedTable):
     fieldname: str
     otherfield: typing.Optional[float]
-    yet_another: TextField(default="something", required=False)
+    yet_another = TextField(default="something", required=False)
 
 
 db.define(TableName)
 ```
 
 </td>
 </tr>
@@ -187,43 +187,43 @@
 
 </td>
 </tr>
 -->
 
 ### All Types
 
-| pydal                                     | typedal (native python type) | typedal (using TypedField)               | typedal (using specific Field)      |
-|-------------------------------------------|------------------------------|------------------------------------------|-------------------------------------|
-| `Field('name', 'string')`                 | `name: str`                  | `name: TypedField(str)`                  | `name: StringField()`               |
-| `Field('name', 'text')`                   | ×                            | `name: TypedField(str, type="text")`     | `name: TextField()`                 |
-| `Field('name', 'blob')`                   | `name: bytes`                | `name: TypedField(bytes)`                | `name: BlobField()`                 |
-| `Field('name', 'boolean')`                | `name: bool`                 | `name: TypedField(bool)`                 | `name: BooleanField()`              |
-| `Field('name', 'integer')`                | `name: int`                  | `name: TypedField(int)`                  | `name: IntegerField()`              |
-| `Field('name', 'double')`                 | `name: float`                | `name: TypedField(float)`                | `name: DoubleField()`               |
-| `Field('name', 'decimal(n,m)')`           | `name: decimal.Decimal`      | `name: TypedField(decimal.Decimal)`      | `name: DecimalField(n=n, m=m)`      |
-| `Field('name', 'date')`                   | `name: datetime.date`        | `name: TypedField(datetime.date)`        | `name: DateField()`                 |
-| `Field('name', 'time')`                   | `name: datetime.time`        | `name: TypedField(datetime.time)`        | `name: TimeField()`                 |
-| `Field('name', 'datetime')`               | `name: datetime.datetime`    | `name: TypedField(datetime.datetime)`    | `name: DatetimeField()`             |
-| `Field('name', 'password')`               | ×                            | `name: TypedField(str, type="password")` | `name: PasswordField()`             |
-| `Field('name', 'upload')`                 | ×                            | `name: TypedField(str, type="upload)`    | `name: UploadField()`               |
-| `Field('name', 'reference <table>')`      | `name: Table`                | `name: TypedField(Table)`                | `name: ReferenceField('table')`     |
-| `Field('name', 'list:string')`            | `name: list[str]`            | `name: TypedField(list[str])`            | `name: ListStringField()`           |
-| `Field('name', 'list:integer')`           | `name: list[int]`            | `name: TypedField()`                     | `name: ListIntegerField()`          |
-| `Field('name', 'list:reference <table>')` | `name: list[Table]`          | `name: TypedField()`                     | `name: ListReferenceField('table')` |
-| `Field('name', 'json')`                   | ×                            | `name: TypedField()`                     | `name: JSONField()`                 |
-| `Field('name', 'bigint')`                 | ×                            | `name: TypedField()`                     | `name: BigintField()`               |
-| `Field('name', 'big-id')`                 | ×                            | ×                                        | ×                                   |
-| `Field('name', 'big-reference')`          | ×                            | ×                                        | ×                                   |
+| pydal                                     | typedal (native python type) | typedal (using TypedField)                | typedal (using specific Field)       |
+|-------------------------------------------|------------------------------|-------------------------------------------|--------------------------------------|
+| `Field('name', 'string')`                 | `name: str`                  | `name = TypedField(str)`                  | `name = StringField()`               |
+| `Field('name', 'text')`                   | ×                            | `name = TypedField(str, type="text")`     | `name = TextField()`                 |
+| `Field('name', 'blob')`                   | `name: bytes`                | `name = TypedField(bytes)`                | `name = BlobField()`                 |
+| `Field('name', 'boolean')`                | `name: bool`                 | `name = TypedField(bool)`                 | `name = BooleanField()`              |
+| `Field('name', 'integer')`                | `name: int`                  | `name = TypedField(int)`                  | `name = IntegerField()`              |
+| `Field('name', 'double')`                 | `name: float`                | `name = TypedField(float)`                | `name = DoubleField()`               |
+| `Field('name', 'decimal(n,m)')`           | `name: decimal.Decimal`      | `name = TypedField(decimal.Decimal)`      | `name = DecimalField(n=n, m=m)`      |
+| `Field('name', 'date')`                   | `name: datetime.date`        | `name = TypedField(datetime.date)`        | `name = DateField()`                 |
+| `Field('name', 'time')`                   | `name: datetime.time`        | `name = TypedField(datetime.time)`        | `name = TimeField()`                 |
+| `Field('name', 'datetime')`               | `name: datetime.datetime`    | `name = TypedField(datetime.datetime)`    | `name = DatetimeField()`             |
+| `Field('name', 'password')`               | ×                            | `name = TypedField(str, type="password")` | `name = PasswordField()`             |
+| `Field('name', 'upload')`                 | ×                            | `name = TypedField(str, type="upload)`    | `name = UploadField()`               |
+| `Field('name', 'reference <table>')`      | `name: Table`                | `name = TypedField(Table)`                | `name = ReferenceField('table')`     |
+| `Field('name', 'list:string')`            | `name: list[str]`            | `name = TypedField(list[str])`            | `name = ListStringField()`           |
+| `Field('name', 'list:integer')`           | `name: list[int]`            | `name = TypedField()`                     | `name = ListIntegerField()`          |
+| `Field('name', 'list:reference <table>')` | `name: list[Table]`          | `name = TypedField()`                     | `name = ListReferenceField('table')` |
+| `Field('name', 'json')`                   | ×                            | `name = TypedField()`                     | `name = JSONField()`                 |
+| `Field('name', 'bigint')`                 | ×                            | `name = TypedField()`                     | `name = BigintField()`               |
+| `Field('name', 'big-id')`                 | ×                            | ×                                         | ×                                    |
+| `Field('name', 'big-reference')`          | ×                            | ×                                         | ×                                    |
 
 ### Making a field required/optional
 
-| pydal                                    | typedal (native python type)                                              | typedal (using TypedField)                           | typedal (using specific Field)      |
-|------------------------------------------|---------------------------------------------------------------------------|------------------------------------------------------|-------------------------------------|
-| `Field('name', 'string', required=True)` | `name: str`                                                               | `name: TypedField(str, required=True)`               | `name: StringField(required=True)`  |
-| `Field('name', 'text', required=False)`  | `name: typing.Optional[str]` or  <br/> <code>name: str &#124; None</code> | `name: TypedField(str, type="text", required=False)` | `name: StringField(required=False)` |
+| pydal                                    | typedal (native python type)                                              | typedal (using TypedField)                            | typedal (using specific Field)       |
+|------------------------------------------|---------------------------------------------------------------------------|-------------------------------------------------------|--------------------------------------|
+| `Field('name', 'string', required=True)` | `name: str`                                                               | `name = TypedField(str, required=True)`               | `name = StringField(required=True)`  |
+| `Field('name', 'text', required=False)`  | `name: typing.Optional[str]` or  <br/> <code>name: str &#124; None</code> | `name = TypedField(str, type="text", required=False)` | `name = StringField(required=False)` |
 
 ## Caveats
 
 - This package depends heavily on the current implementation of annotations (which are computed when the class is
   defined). PEP 563 (Postponed Evaluation of Annotations, accepted) aims to change this behavior (
   and `from __future__ import annotations` already does) in a way that this module currently can not handle: all
   annotations are converted to string representations. This makes it very hard to re-evaluate the annotation into the
```

### Comparing `typedal-1.0.0b1/pyproject.toml` & `typedal-1.1.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -25,19 +25,23 @@
 dependencies = [
     "pydal",
 ]
 
 [template.plugins.default]
 src-layout = true
 
+[tool.setuptools.package-data]
+"typedal" = ["py.typed"]
+
 [project.optional-dependencies]
 dev = [
     "hatch",
     "su6[all]",
     "python-semantic-release",
+    "pytest-mypy-testing",
 ]
 
 [project.urls]
 Documentation = "https://github.com/trialandsuccess/TypeDAL#readme"
 Issues = "https://github.com/trialandsuccess/TypeDAL/issues"
 Source = "https://github.com/trialandsuccess/TypeDAL"
 
@@ -51,14 +55,15 @@
 upload_to_repository = false
 upload_to_release = false
 build_command = "hatch build"
 
 ### required in every su6 pyproject: ###
 [tool.su6]
 directory = "src"
+stop-after-first-failure = true
 include = []
 exclude = []
 coverage = 100
 badge = true
 
 [tool.black]
 target-version = ["py310"]
@@ -118,14 +123,18 @@
 extend-ignore = [
     # db.field == None should NOT be fixed to db.field is None
     "E711",
 ]
 
 extend-exclude = ["*.bak/", "venv*/"]
 
+ignore = [
+    "RUF013" # implicit optional
+]
+
 [tool.bandit]
 # bandit -c pyproject.toml -r .
 exclude_dirs = [".bak", "venv"]
 skips = [
     "B108"  # hard coded /tmp/... files are fine for me tbh
 ]
```

### Comparing `typedal-1.0.0b1/PKG-INFO` & `typedal-1.1.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TypeDal
-Version: 1.0.0b1
+Version: 1.1.1
 Summary: Typing support for PyDAL
 Project-URL: Documentation, https://github.com/trialandsuccess/TypeDAL#readme
 Project-URL: Issues, https://github.com/trialandsuccess/TypeDAL/issues
 Project-URL: Source, https://github.com/trialandsuccess/TypeDAL
 Author-email: Robin van der Noord <contact@trialandsuccess.nl>
 License-Expression: MIT
 Classifier: Development Status :: 4 - Beta
@@ -14,37 +14,38 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.10
 Requires-Dist: pydal
 Provides-Extra: dev
 Requires-Dist: hatch; extra == 'dev'
+Requires-Dist: pytest-mypy-testing; extra == 'dev'
 Requires-Dist: python-semantic-release; extra == 'dev'
 Requires-Dist: su6[all]; extra == 'dev'
 Description-Content-Type: text/markdown
 
 # TypeDAL
 
-[![PyPI - Version](https://img.shields.io/pypi/v/TypeDal.svg)](https://pypi.org/project/typedal)
-[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/TypeDal.svg)](https://pypi.org/project/typedal)  
+[![PyPI - Version](https://img.shields.io/pypi/v/TypeDAL.svg)](https://pypi.org/project/TypeDAL)
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/TypeDAL.svg)](https://pypi.org/project/TypeDAL)  
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)  
-[![su6 checks](https://github.com/trialandsuccess/typedal/actions/workflows/su6.yml/badge.svg)](https://github.com/trialandsuccess/typedal/actions)
+[![su6 checks](https://github.com/trialandsuccess/TypeDAL/actions/workflows/su6.yml/badge.svg?branch=development)](https://github.com/trialandsuccess/TypeDAL/actions)
 ![coverage.svg](coverage.svg)
 
 Typing support for [PyDAL](http://web2py.com/books/default/chapter/29/6).
 This package aims to improve the typing support for PyDAL. By using classes instead of the define_table method,
 type hinting the result of queries can improve the experience while developing. In the background, the queries are still
 generated and executed by pydal itself, this package only proves some logic to properly pass calls from class methods to
 the underlying `db.define_table` pydal Tables.
 
 - `TypeDAL` is the replacement class for DAL that manages the code on top of DAL.
 - `TypedTable` must be the parent class of any custom Tables you define (e.g. `class SomeTable(TypedTable)`)
 - `TypedField` can be used instead of Python native types when extra settings (such as default) are required (
-  e.g. `name: TypedField(str, default="John Doe")`)
+  e.g. `name = TypedField(str, default="John Doe")`)
 - `TypedRows`: can be used as the return type of .select() and subscribed with the actual table class, so
   e.g. `rows: TypedRows[SomeTable]`. If you're lazy, `list[SomeTable]` works fine too but that misses hinting
   possibilities such as `.first()`.
 
 ### Translations from pydal to typedal
 
 <table>
@@ -98,29 +99,29 @@
 <td>
 
 ```python
 @db.define
 class TableName(TypedTable):
     fieldname: str
     otherfield: float | None
-    yet_another: TypedField(str, type="text", default="something", required=False)
+    yet_another = TypedField(str, type="text", default="something", required=False)
 ```
 
 </td>
 
 <td>
 
 ```python
 import typing
 
 
 class TableName(TypedTable):
     fieldname: str
     otherfield: typing.Optional[float]
-    yet_another: TextField(default="something", required=False)
+    yet_another = TextField(default="something", required=False)
 
 
 db.define(TableName)
 ```
 
 </td>
 </tr>
@@ -211,43 +212,43 @@
 
 </td>
 </tr>
 -->
 
 ### All Types
 
-| pydal                                     | typedal (native python type) | typedal (using TypedField)               | typedal (using specific Field)      |
-|-------------------------------------------|------------------------------|------------------------------------------|-------------------------------------|
-| `Field('name', 'string')`                 | `name: str`                  | `name: TypedField(str)`                  | `name: StringField()`               |
-| `Field('name', 'text')`                   | ×                            | `name: TypedField(str, type="text")`     | `name: TextField()`                 |
-| `Field('name', 'blob')`                   | `name: bytes`                | `name: TypedField(bytes)`                | `name: BlobField()`                 |
-| `Field('name', 'boolean')`                | `name: bool`                 | `name: TypedField(bool)`                 | `name: BooleanField()`              |
-| `Field('name', 'integer')`                | `name: int`                  | `name: TypedField(int)`                  | `name: IntegerField()`              |
-| `Field('name', 'double')`                 | `name: float`                | `name: TypedField(float)`                | `name: DoubleField()`               |
-| `Field('name', 'decimal(n,m)')`           | `name: decimal.Decimal`      | `name: TypedField(decimal.Decimal)`      | `name: DecimalField(n=n, m=m)`      |
-| `Field('name', 'date')`                   | `name: datetime.date`        | `name: TypedField(datetime.date)`        | `name: DateField()`                 |
-| `Field('name', 'time')`                   | `name: datetime.time`        | `name: TypedField(datetime.time)`        | `name: TimeField()`                 |
-| `Field('name', 'datetime')`               | `name: datetime.datetime`    | `name: TypedField(datetime.datetime)`    | `name: DatetimeField()`             |
-| `Field('name', 'password')`               | ×                            | `name: TypedField(str, type="password")` | `name: PasswordField()`             |
-| `Field('name', 'upload')`                 | ×                            | `name: TypedField(str, type="upload)`    | `name: UploadField()`               |
-| `Field('name', 'reference <table>')`      | `name: Table`                | `name: TypedField(Table)`                | `name: ReferenceField('table')`     |
-| `Field('name', 'list:string')`            | `name: list[str]`            | `name: TypedField(list[str])`            | `name: ListStringField()`           |
-| `Field('name', 'list:integer')`           | `name: list[int]`            | `name: TypedField()`                     | `name: ListIntegerField()`          |
-| `Field('name', 'list:reference <table>')` | `name: list[Table]`          | `name: TypedField()`                     | `name: ListReferenceField('table')` |
-| `Field('name', 'json')`                   | ×                            | `name: TypedField()`                     | `name: JSONField()`                 |
-| `Field('name', 'bigint')`                 | ×                            | `name: TypedField()`                     | `name: BigintField()`               |
-| `Field('name', 'big-id')`                 | ×                            | ×                                        | ×                                   |
-| `Field('name', 'big-reference')`          | ×                            | ×                                        | ×                                   |
+| pydal                                     | typedal (native python type) | typedal (using TypedField)                | typedal (using specific Field)       |
+|-------------------------------------------|------------------------------|-------------------------------------------|--------------------------------------|
+| `Field('name', 'string')`                 | `name: str`                  | `name = TypedField(str)`                  | `name = StringField()`               |
+| `Field('name', 'text')`                   | ×                            | `name = TypedField(str, type="text")`     | `name = TextField()`                 |
+| `Field('name', 'blob')`                   | `name: bytes`                | `name = TypedField(bytes)`                | `name = BlobField()`                 |
+| `Field('name', 'boolean')`                | `name: bool`                 | `name = TypedField(bool)`                 | `name = BooleanField()`              |
+| `Field('name', 'integer')`                | `name: int`                  | `name = TypedField(int)`                  | `name = IntegerField()`              |
+| `Field('name', 'double')`                 | `name: float`                | `name = TypedField(float)`                | `name = DoubleField()`               |
+| `Field('name', 'decimal(n,m)')`           | `name: decimal.Decimal`      | `name = TypedField(decimal.Decimal)`      | `name = DecimalField(n=n, m=m)`      |
+| `Field('name', 'date')`                   | `name: datetime.date`        | `name = TypedField(datetime.date)`        | `name = DateField()`                 |
+| `Field('name', 'time')`                   | `name: datetime.time`        | `name = TypedField(datetime.time)`        | `name = TimeField()`                 |
+| `Field('name', 'datetime')`               | `name: datetime.datetime`    | `name = TypedField(datetime.datetime)`    | `name = DatetimeField()`             |
+| `Field('name', 'password')`               | ×                            | `name = TypedField(str, type="password")` | `name = PasswordField()`             |
+| `Field('name', 'upload')`                 | ×                            | `name = TypedField(str, type="upload)`    | `name = UploadField()`               |
+| `Field('name', 'reference <table>')`      | `name: Table`                | `name = TypedField(Table)`                | `name = ReferenceField('table')`     |
+| `Field('name', 'list:string')`            | `name: list[str]`            | `name = TypedField(list[str])`            | `name = ListStringField()`           |
+| `Field('name', 'list:integer')`           | `name: list[int]`            | `name = TypedField()`                     | `name = ListIntegerField()`          |
+| `Field('name', 'list:reference <table>')` | `name: list[Table]`          | `name = TypedField()`                     | `name = ListReferenceField('table')` |
+| `Field('name', 'json')`                   | ×                            | `name = TypedField()`                     | `name = JSONField()`                 |
+| `Field('name', 'bigint')`                 | ×                            | `name = TypedField()`                     | `name = BigintField()`               |
+| `Field('name', 'big-id')`                 | ×                            | ×                                         | ×                                    |
+| `Field('name', 'big-reference')`          | ×                            | ×                                         | ×                                    |
 
 ### Making a field required/optional
 
-| pydal                                    | typedal (native python type)                                              | typedal (using TypedField)                           | typedal (using specific Field)      |
-|------------------------------------------|---------------------------------------------------------------------------|------------------------------------------------------|-------------------------------------|
-| `Field('name', 'string', required=True)` | `name: str`                                                               | `name: TypedField(str, required=True)`               | `name: StringField(required=True)`  |
-| `Field('name', 'text', required=False)`  | `name: typing.Optional[str]` or  <br/> <code>name: str &#124; None</code> | `name: TypedField(str, type="text", required=False)` | `name: StringField(required=False)` |
+| pydal                                    | typedal (native python type)                                              | typedal (using TypedField)                            | typedal (using specific Field)       |
+|------------------------------------------|---------------------------------------------------------------------------|-------------------------------------------------------|--------------------------------------|
+| `Field('name', 'string', required=True)` | `name: str`                                                               | `name = TypedField(str, required=True)`               | `name = StringField(required=True)`  |
+| `Field('name', 'text', required=False)`  | `name: typing.Optional[str]` or  <br/> <code>name: str &#124; None</code> | `name = TypedField(str, type="text", required=False)` | `name = StringField(required=False)` |
 
 ## Caveats
 
 - This package depends heavily on the current implementation of annotations (which are computed when the class is
   defined). PEP 563 (Postponed Evaluation of Annotations, accepted) aims to change this behavior (
   and `from __future__ import annotations` already does) in a way that this module currently can not handle: all
   annotations are converted to string representations. This makes it very hard to re-evaluate the annotation into the
```

