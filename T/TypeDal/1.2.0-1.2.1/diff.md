# Comparing `tmp/typedal-1.2.0.tar.gz` & `tmp/typedal-1.2.1.tar.gz`

## Comparing `typedal-1.2.0.tar` & `typedal-1.2.1.tar`

### file list

```diff
@@ -1,352 +1,354 @@
--rw-r--r--   0        0        0     3393 2020-02-02 00:00:00.000000 typedal-1.2.0/CHANGELOG.md
--rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 typedal-1.2.0/coverage.svg
--rw-r--r--   0        0        0     7007 2020-02-02 00:00:00.000000 typedal-1.2.0/example_new.py
--rw-r--r--   0        0        0     2872 2020-02-02 00:00:00.000000 typedal-1.2.0/example_old.py
--rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 typedal-1.2.0/.github/workflows/su6.yml
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/.gitignore
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.10/@plugins_snapshot.json
--rw-r--r--   0        0        0   177667 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.10/_ast.data.json
--rw-r--r--   0        0        0     1567 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.10/_ast.meta.json
--rw-r--r--   0        0        0    52400 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.10/_codecs.data.json
--rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.10/_codecs.meta.json
--rw-r--r--   0        0        0    18227 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.10/_collections_abc.data.json
--rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.10/_collections_abc.meta.json
--rw-r--r--   0        0        0     2923 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.10/_ctypes.data.json
--rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.10/_ctypes.meta.json
--rw-r--r--   0        0        0   170960 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.10/_decimal.data.json
--rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.10/_decimal.meta.json
--rw-r--r--   0        0        0    23362 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.10/abc.data.json
--rw-r--r--   0        0        0     1574 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.10/abc.meta.json
--rw-r--r--   0        0        0    60687 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.10/array.data.json
--rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.10/array.meta.json
--rw-r--r--   0        0        0  1054992 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.10/builtins.data.json
--rw-r--r--   0        0        0     1721 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.10/builtins.meta.json
--rw-r--r--   0        0        0   123328 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.10/codecs.data.json
--rw-r--r--   0        0        0     1671 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.10/codecs.meta.json
--rw-r--r--   0        0        0   104160 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.10/contextlib.data.json
--rw-r--r--   0        0        0     1610 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.10/contextlib.meta.json
--rw-r--r--   0        0        0    57612 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.10/dataclasses.data.json
--rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.10/dataclasses.meta.json
--rw-r--r--   0        0        0   142044 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.10/datetime.data.json
--rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.10/datetime.meta.json
--rw-r--r--   0        0        0     4911 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.10/decimal.data.json
--rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.10/decimal.meta.json
--rw-r--r--   0        0        0    61020 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.10/enum.data.json
--rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.10/enum.meta.json
--rw-r--r--   0        0        0    22399 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.10/genericpath.data.json
--rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.10/genericpath.meta.json
--rw-r--r--   0        0        0    85348 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.10/io.data.json
--rw-r--r--   0        0        0     1673 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.10/io.meta.json
--rw-r--r--   0        0        0    28778 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.10/mmap.data.json
--rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.10/mmap.meta.json
--rw-r--r--   0        0        0    78982 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.10/numbers.data.json
--rw-r--r--   0        0        0     1519 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.10/numbers.meta.json
--rw-r--r--   0        0        0    88278 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.10/pathlib.data.json
--rw-r--r--   0        0        0     1682 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.10/pathlib.meta.json
--rw-r--r--   0        0        0    45131 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.10/pickle.data.json
--rw-r--r--   0        0        0     1630 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.10/pickle.meta.json
--rw-r--r--   0        0        0    75208 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.10/posixpath.data.json
--rw-r--r--   0        0        0     1627 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.10/posixpath.meta.json
--rw-r--r--   0        0        0   167175 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.10/re.data.json
--rw-r--r--   0        0        0     1701 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.10/re.meta.json
--rw-r--r--   0        0        0    14131 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.10/sre_compile.data.json
--rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.10/sre_compile.meta.json
--rw-r--r--   0        0        0    28013 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.10/sre_constants.data.json
--rw-r--r--   0        0        0     1584 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.10/sre_constants.meta.json
--rw-r--r--   0        0        0    49442 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.10/sre_parse.data.json
--rw-r--r--   0        0        0     1627 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.10/sre_parse.meta.json
--rw-r--r--   0        0        0   168498 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.10/subprocess.data.json
--rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.10/subprocess.meta.json
--rw-r--r--   0        0        0   146267 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.10/sys.data.json
--rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.10/sys.meta.json
--rw-r--r--   0        0        0    43605 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.10/time.data.json
--rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.10/time.meta.json
--rw-r--r--   0        0        0   228230 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.10/types.data.json
--rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.10/types.meta.json
--rw-r--r--   0        0        0   416965 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.10/typing.data.json
--rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.10/typing.meta.json
--rw-r--r--   0        0        0    73907 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.10/typing_extensions.data.json
--rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.10/typing_extensions.meta.json
--rw-r--r--   0        0        0    89065 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.10/_typeshed/__init__.data.json
--rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.10/_typeshed/__init__.meta.json
--rw-r--r--   0        0        0   407999 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.10/collections/__init__.data.json
--rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.10/collections/__init__.meta.json
--rw-r--r--   0        0        0     3731 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.10/collections/abc.data.json
--rw-r--r--   0        0        0     1558 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.10/collections/abc.meta.json
--rw-r--r--   0        0        0   128994 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.10/ctypes/__init__.data.json
--rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.10/ctypes/__init__.meta.json
--rw-r--r--   0        0        0     7438 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.10/email/__init__.data.json
--rw-r--r--   0        0        0     1610 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.10/email/__init__.meta.json
--rw-r--r--   0        0        0    12200 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.10/email/charset.data.json
--rw-r--r--   0        0        0     1555 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.10/email/charset.meta.json
--rw-r--r--   0        0        0     7249 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.10/email/contentmanager.data.json
--rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.10/email/contentmanager.meta.json
--rw-r--r--   0        0        0    25073 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.10/email/errors.data.json
--rw-r--r--   0        0        0     1559 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.10/email/errors.meta.json
--rw-r--r--   0        0        0     9154 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.10/email/header.data.json
--rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.10/email/header.meta.json
--rw-r--r--   0        0        0    79298 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.10/email/message.data.json
--rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.10/email/message.meta.json
--rw-r--r--   0        0        0    30857 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.10/email/policy.data.json
--rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.10/email/policy.meta.json
--rw-r--r--   0        0        0     6125 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.10/importlib/__init__.data.json
--rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.10/importlib/__init__.meta.json
--rw-r--r--   0        0        0    70175 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.10/importlib/abc.data.json
--rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.10/importlib/abc.meta.json
--rw-r--r--   0        0        0    64626 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.10/importlib/machinery.data.json
--rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.10/importlib/machinery.meta.json
--rw-r--r--   0        0        0    90277 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.10/importlib/metadata/__init__.data.json
--rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.10/importlib/metadata/__init__.meta.json
--rw-r--r--   0        0        0    11935 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.10/importlib/metadata/_meta.data.json
--rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.10/importlib/metadata/_meta.meta.json
--rw-r--r--   0        0        0   350178 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.10/os/__init__.data.json
--rw-r--r--   0        0        0     1725 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.10/os/__init__.meta.json
--rw-r--r--   0        0        0     4908 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.10/os/path.data.json
--rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.10/os/path.meta.json
--rw-r--r--   0        0        0     1385 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.10/src/__init__.data.json
--rw-r--r--   0        0        0     1433 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.10/src/__init__.meta.json
--rw-r--r--   0        0        0     1506 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.10/src/typedal/__about__.data.json
--rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.10/src/typedal/__about__.meta.json
--rw-r--r--   0        0        0     2114 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.10/src/typedal/__init__.data.json
--rw-r--r--   0        0        0     1499 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.10/src/typedal/__init__.meta.json
--rw-r--r--   0        0        0    33347 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.10/src/typedal/core.data.json
--rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.10/src/typedal/core.meta.json
--rw-r--r--   0        0        0    29038 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.10/src/typedal/fields.data.json
--rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.10/src/typedal/fields.meta.json
--rw-r--r--   0        0        0     2775 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.10/src/typedal/pydal_objects.data.json
--rw-r--r--   0        0        0     1503 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.10/src/typedal/pydal_objects.meta.json
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.11/@plugins_snapshot.json
--rw-r--r--   0        0        0   180368 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.11/_ast.data.json
--rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.11/_ast.meta.json
--rw-r--r--   0        0        0    52400 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.11/_codecs.data.json
--rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.11/_codecs.meta.json
--rw-r--r--   0        0        0    18227 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.11/_collections_abc.data.json
--rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.11/_collections_abc.meta.json
--rw-r--r--   0        0        0     3125 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.11/_ctypes.data.json
--rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.11/_ctypes.meta.json
--rw-r--r--   0        0        0   171931 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.11/_decimal.data.json
--rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.11/_decimal.meta.json
--rw-r--r--   0        0        0    23336 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.11/abc.data.json
--rw-r--r--   0        0        0     1574 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.11/abc.meta.json
--rw-r--r--   0        0        0    60676 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.11/array.data.json
--rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.11/array.meta.json
--rw-r--r--   0        0        0  1130454 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.11/builtins.data.json
--rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.11/builtins.meta.json
--rw-r--r--   0        0        0   123317 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.11/codecs.data.json
--rw-r--r--   0        0        0     1671 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.11/codecs.meta.json
--rw-r--r--   0        0        0   109204 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.11/contextlib.data.json
--rw-r--r--   0        0        0     1610 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.11/contextlib.meta.json
--rw-r--r--   0        0        0    57745 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.11/dataclasses.data.json
--rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.11/dataclasses.meta.json
--rw-r--r--   0        0        0   142208 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.11/datetime.data.json
--rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.11/datetime.meta.json
--rw-r--r--   0        0        0     4911 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.11/decimal.data.json
--rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.11/decimal.meta.json
--rw-r--r--   0        0        0    90123 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.11/enum.data.json
--rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.11/enum.meta.json
--rw-r--r--   0        0        0    22388 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.11/genericpath.data.json
--rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.11/genericpath.meta.json
--rw-r--r--   0        0        0    85337 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.11/io.data.json
--rw-r--r--   0        0        0     1673 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.11/io.meta.json
--rw-r--r--   0        0        0    28767 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.11/mmap.data.json
--rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.11/mmap.meta.json
--rw-r--r--   0        0        0    78982 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.11/numbers.data.json
--rw-r--r--   0        0        0     1519 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.11/numbers.meta.json
--rw-r--r--   0        0        0    87488 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.11/pathlib.data.json
--rw-r--r--   0        0        0     1682 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.11/pathlib.meta.json
--rw-r--r--   0        0        0    45131 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.11/pickle.data.json
--rw-r--r--   0        0        0     1630 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.11/pickle.meta.json
--rw-r--r--   0        0        0    75197 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.11/posixpath.data.json
--rw-r--r--   0        0        0     1627 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.11/posixpath.meta.json
--rw-r--r--   0        0        0   167545 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.11/re.data.json
--rw-r--r--   0        0        0     1701 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.11/re.meta.json
--rw-r--r--   0        0        0     1181 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.11/src.data.json
--rw-r--r--   0        0        0     1391 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.11/src.meta.json
--rw-r--r--   0        0        0    14373 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.11/sre_compile.data.json
--rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.11/sre_compile.meta.json
--rw-r--r--   0        0        0    28480 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.11/sre_constants.data.json
--rw-r--r--   0        0        0     1584 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.11/sre_constants.meta.json
--rw-r--r--   0        0        0    49741 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.11/sre_parse.data.json
--rw-r--r--   0        0        0     1627 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.11/sre_parse.meta.json
--rw-r--r--   0        0        0   172768 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.11/subprocess.data.json
--rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.11/subprocess.meta.json
--rw-r--r--   0        0        0   148675 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.11/sys.data.json
--rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.11/sys.meta.json
--rw-r--r--   0        0        0    43605 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.11/time.data.json
--rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.11/time.meta.json
--rw-r--r--   0        0        0   239632 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.11/types.data.json
--rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.11/types.meta.json
--rw-r--r--   0        0        0   432234 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.11/typing.data.json
--rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.11/typing.meta.json
--rw-r--r--   0        0        0    57845 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.11/typing_extensions.data.json
--rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.11/typing_extensions.meta.json
--rw-r--r--   0        0        0    89054 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.11/_typeshed/__init__.data.json
--rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.11/_typeshed/__init__.meta.json
--rw-r--r--   0        0        0   407988 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.11/collections/__init__.data.json
--rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.11/collections/__init__.meta.json
--rw-r--r--   0        0        0     3731 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.11/collections/abc.data.json
--rw-r--r--   0        0        0     1558 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.11/collections/abc.meta.json
--rw-r--r--   0        0        0   128983 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.11/ctypes/__init__.data.json
--rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.11/ctypes/__init__.meta.json
--rw-r--r--   0        0        0     7438 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.11/email/__init__.data.json
--rw-r--r--   0        0        0     1610 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.11/email/__init__.meta.json
--rw-r--r--   0        0        0    12200 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.11/email/charset.data.json
--rw-r--r--   0        0        0     1555 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.11/email/charset.meta.json
--rw-r--r--   0        0        0     7249 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.11/email/contentmanager.data.json
--rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.11/email/contentmanager.meta.json
--rw-r--r--   0        0        0    25073 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.11/email/errors.data.json
--rw-r--r--   0        0        0     1559 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.11/email/errors.meta.json
--rw-r--r--   0        0        0     9154 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.11/email/header.data.json
--rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.11/email/header.meta.json
--rw-r--r--   0        0        0    79287 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.11/email/message.data.json
--rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.11/email/message.meta.json
--rw-r--r--   0        0        0    30857 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.11/email/policy.data.json
--rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.11/email/policy.meta.json
--rw-r--r--   0        0        0     6125 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.11/importlib/__init__.data.json
--rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.11/importlib/__init__.meta.json
--rw-r--r--   0        0        0    70579 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.11/importlib/abc.data.json
--rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.11/importlib/abc.meta.json
--rw-r--r--   0        0        0    64626 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.11/importlib/machinery.data.json
--rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.11/importlib/machinery.meta.json
--rw-r--r--   0        0        0    91119 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.11/importlib/metadata/__init__.data.json
--rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.11/importlib/metadata/__init__.meta.json
--rw-r--r--   0        0        0    11935 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.11/importlib/metadata/_meta.data.json
--rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.11/importlib/metadata/_meta.meta.json
--rw-r--r--   0        0        0   350743 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.11/os/__init__.data.json
--rw-r--r--   0        0        0     1725 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.11/os/__init__.meta.json
--rw-r--r--   0        0        0     4908 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.11/os/path.data.json
--rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.11/os/path.meta.json
--rw-r--r--   0        0        0     1385 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.11/src/__init__.data.json
--rw-r--r--   0        0        0     1433 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.11/src/__init__.meta.json
--rw-r--r--   0        0        0     1506 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.11/src/typedal/__about__.data.json
--rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.11/src/typedal/__about__.meta.json
--rw-r--r--   0        0        0     2357 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.11/src/typedal/__init__.data.json
--rw-r--r--   0        0        0     1530 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.11/src/typedal/__init__.meta.json
--rw-r--r--   0        0        0    40879 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.11/src/typedal/core.data.json
--rw-r--r--   0        0        0     1715 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.11/src/typedal/core.meta.json
--rw-r--r--   0        0        0    28504 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.11/src/typedal/fields.data.json
--rw-r--r--   0        0        0     1687 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.11/src/typedal/fields.meta.json
--rw-r--r--   0        0        0     1478 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.11/typedal/__about__.data.json
--rw-r--r--   0        0        0     1458 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.11/typedal/__about__.meta.json
--rw-r--r--   0        0        0     2274 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.11/typedal/__init__.data.json
--rw-r--r--   0        0        0     1487 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.11/typedal/__init__.meta.json
--rw-r--r--   0        0        0    39828 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.11/typedal/core.data.json
--rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.11/typedal/core.meta.json
--rw-r--r--   0        0        0    28193 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.11/typedal/fields.data.json
--rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 typedal-1.2.0/.mypy_cache/3.11/typedal/fields.meta.json
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 typedal-1.2.0/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 typedal-1.2.0/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 typedal-1.2.0/.pytest_cache/README.md
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 typedal-1.2.0/.pytest_cache/v/cache/lastfailed
--rw-r--r--   0        0        0      989 2020-02-02 00:00:00.000000 typedal-1.2.0/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 typedal-1.2.0/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 typedal-1.2.0/.ruff_cache/.gitignore
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 typedal-1.2.0/.ruff_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 typedal-1.2.0/.ruff_cache/content/1215429078721865123
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.0/.ruff_cache/content/121ed75fe9fe5f8e
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.0/.ruff_cache/content/19309938546e93ab
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.0/.ruff_cache/content/197f3188bc94f91f
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.0/.ruff_cache/content/1aa1390b5bde1004
--rw-r--r--   0        0        0     8089 2020-02-02 00:00:00.000000 typedal-1.2.0/.ruff_cache/content/1b34455c399f0006
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.0/.ruff_cache/content/1bd1a229a4f4ee7f
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.0/.ruff_cache/content/1c46d1f378d28fbb
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.0/.ruff_cache/content/1ca71ee291d82018
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.0/.ruff_cache/content/1d6bb777df44b8ec
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.0/.ruff_cache/content/1dc8423cfb79eaa4
--rw-r--r--   0        0        0      908 2020-02-02 00:00:00.000000 typedal-1.2.0/.ruff_cache/content/20585cf790eae81e
--rw-r--r--   0        0        0    12122 2020-02-02 00:00:00.000000 typedal-1.2.0/.ruff_cache/content/221af82ae72a7f27
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.0/.ruff_cache/content/2282e801459c52a4
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.0/.ruff_cache/content/248c4e1a32c704cb
--rw-r--r--   0        0        0    10858 2020-02-02 00:00:00.000000 typedal-1.2.0/.ruff_cache/content/24e1b4aab386ebc8
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.0/.ruff_cache/content/28b1d8ac7e2aab6b
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.0/.ruff_cache/content/2b7f7d266c8efaad
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.0/.ruff_cache/content/2bb6610cadf18e18
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.0/.ruff_cache/content/2dac345be8527adf
--rw-r--r--   0        0        0    11525 2020-02-02 00:00:00.000000 typedal-1.2.0/.ruff_cache/content/2f3396c610fd7095
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.0/.ruff_cache/content/31731f8e74291475
--rw-r--r--   0        0        0    13342 2020-02-02 00:00:00.000000 typedal-1.2.0/.ruff_cache/content/322af04e6d059ce5
--rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 typedal-1.2.0/.ruff_cache/content/3826106cf4494de8
--rw-r--r--   0        0        0    11210 2020-02-02 00:00:00.000000 typedal-1.2.0/.ruff_cache/content/38d5fd55b14a9d6c
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.0/.ruff_cache/content/3afc55a04b8f8bb2
--rw-r--r--   0        0        0    12129 2020-02-02 00:00:00.000000 typedal-1.2.0/.ruff_cache/content/4022ee8774ccd98a
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.0/.ruff_cache/content/42f9a2406e74c24f
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.0/.ruff_cache/content/4696b157ff786f22
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.0/.ruff_cache/content/46a88ce266f1ad94
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.0/.ruff_cache/content/4a6edd5010cb9700
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.0/.ruff_cache/content/4d0230e9a81a468
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.0/.ruff_cache/content/52018ba3989fcaf7
--rw-r--r--   0        0        0    13679 2020-02-02 00:00:00.000000 typedal-1.2.0/.ruff_cache/content/5491563776466765346
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.0/.ruff_cache/content/54e6ba8c25a22ffc
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.0/.ruff_cache/content/566d94db91d23339
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.0/.ruff_cache/content/5a67aed8f6b70cd5
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.0/.ruff_cache/content/5b076d769fa5cacd
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.0/.ruff_cache/content/5ceb1580c62ee794
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.0/.ruff_cache/content/6bc90dbb56504f96
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.0/.ruff_cache/content/6c52d14716eee431
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.0/.ruff_cache/content/6f0c8f98e4da1d48
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.0/.ruff_cache/content/74e52af774eebdbd
--rw-r--r--   0        0        0    11023 2020-02-02 00:00:00.000000 typedal-1.2.0/.ruff_cache/content/75bd1769f6e29ed7
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.0/.ruff_cache/content/815ba2cfea236769
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.0/.ruff_cache/content/876d9a8d302e1c46
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.0/.ruff_cache/content/88e2927df9448936
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.0/.ruff_cache/content/8c4d3f5ef14b0167
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.0/.ruff_cache/content/8f8ec552e76f3eab
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.0/.ruff_cache/content/95c82d8566c6704c
--rw-r--r--   0        0        0     8349 2020-02-02 00:00:00.000000 typedal-1.2.0/.ruff_cache/content/a0739889bf9412e8
--rw-r--r--   0        0        0     5692 2020-02-02 00:00:00.000000 typedal-1.2.0/.ruff_cache/content/a225e4df39be9b29
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.0/.ruff_cache/content/a2340fd4c9aa1141
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.0/.ruff_cache/content/a513d558646cd439
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.0/.ruff_cache/content/b121e2b70fd66eb8
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.0/.ruff_cache/content/b218ff88bc22b626
--rw-r--r--   0        0        0    10964 2020-02-02 00:00:00.000000 typedal-1.2.0/.ruff_cache/content/b419496fa9e72887
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.0/.ruff_cache/content/b886c97e4d4117f0
--rw-r--r--   0        0        0     8238 2020-02-02 00:00:00.000000 typedal-1.2.0/.ruff_cache/content/bdcdf5c7bbc1d738
--rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 typedal-1.2.0/.ruff_cache/content/c06de16f3c7a64cc
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.0/.ruff_cache/content/c635f255374598c5
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.0/.ruff_cache/content/c671ae94ff3d3e2e
--rw-r--r--   0        0        0     8042 2020-02-02 00:00:00.000000 typedal-1.2.0/.ruff_cache/content/cdfecbca581311ee
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.0/.ruff_cache/content/ce44121ca4091b64
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.0/.ruff_cache/content/ced49ec87d10bcb0
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.0/.ruff_cache/content/cfc06a1f13c8ab47
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.0/.ruff_cache/content/d16c5d29763a704e
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.0/.ruff_cache/content/d225ad4c14b8ca60
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.0/.ruff_cache/content/d379b35d5e80b789
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.0/.ruff_cache/content/d3a95555c0919160
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.0/.ruff_cache/content/d655bee8ff0a59f2
--rw-r--r--   0        0        0    11315 2020-02-02 00:00:00.000000 typedal-1.2.0/.ruff_cache/content/da4811a7730a562a
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.0/.ruff_cache/content/dca573767bc8be7e
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.0/.ruff_cache/content/e3e29f9eacb7027f
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.0/.ruff_cache/content/e46ab4b61bb5d446
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.0/.ruff_cache/content/e5e0cc178d5c9df5
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.0/.ruff_cache/content/eb564f7989641958
--rw-r--r--   0        0        0    11467 2020-02-02 00:00:00.000000 typedal-1.2.0/.ruff_cache/content/eee2f3c667de6c7a
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.0/.ruff_cache/content/f04d0d78a00adfd6
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.0/.ruff_cache/content/f2ddc22a4b221f54
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.0/.ruff_cache/content/f879e8c947a6b7a4
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.0/.ruff_cache/content/fa45ef3c3166e02d
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.0/.ruff_cache/content/faa51a5044a3c279
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 typedal-1.2.0/htmlcov/.gitignore
--rw-r--r--   0        0        0    21359 2020-02-02 00:00:00.000000 typedal-1.2.0/htmlcov/coverage_html.js
--rw-r--r--   0        0        0     5891 2020-02-02 00:00:00.000000 typedal-1.2.0/htmlcov/d_0ccc93afd6526b6c___about___py.html
--rw-r--r--   0        0        0     6664 2020-02-02 00:00:00.000000 typedal-1.2.0/htmlcov/d_0ccc93afd6526b6c___init___py.html
--rw-r--r--   0        0        0   122020 2020-02-02 00:00:00.000000 typedal-1.2.0/htmlcov/d_0ccc93afd6526b6c_core_py.html
--rw-r--r--   0        0        0    60671 2020-02-02 00:00:00.000000 typedal-1.2.0/htmlcov/d_0ccc93afd6526b6c_fields_py.html
--rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 typedal-1.2.0/htmlcov/favicon_32.png
--rw-r--r--   0        0        0     4825 2020-02-02 00:00:00.000000 typedal-1.2.0/htmlcov/index.html
--rw-r--r--   0        0        0     9004 2020-02-02 00:00:00.000000 typedal-1.2.0/htmlcov/keybd_closed.png
--rw-r--r--   0        0        0     9003 2020-02-02 00:00:00.000000 typedal-1.2.0/htmlcov/keybd_open.png
--rw-r--r--   0        0        0      922 2020-02-02 00:00:00.000000 typedal-1.2.0/htmlcov/status.json
--rw-r--r--   0        0        0    12387 2020-02-02 00:00:00.000000 typedal-1.2.0/htmlcov/style.css
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 typedal-1.2.0/src/typedal/__about__.py
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 typedal-1.2.0/src/typedal/__init__.py
--rw-r--r--   0        0        0    14972 2020-02-02 00:00:00.000000 typedal-1.2.0/src/typedal/core.py
--rw-r--r--   0        0        0     4949 2020-02-02 00:00:00.000000 typedal-1.2.0/src/typedal/fields.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 typedal-1.2.0/src/typedal/py.typed
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 typedal-1.2.0/tests/__init__.py
--rw-r--r--   0        0        0     8827 2020-02-02 00:00:00.000000 typedal-1.2.0/tests/test_main.py
--rw-r--r--   0        0        0      917 2020-02-02 00:00:00.000000 typedal-1.2.0/tests/test_mypy.py
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 typedal-1.2.0/.gitignore
--rw-r--r--   0        0        0     9220 2020-02-02 00:00:00.000000 typedal-1.2.0/README.md
--rw-r--r--   0        0        0     4782 2020-02-02 00:00:00.000000 typedal-1.2.0/pyproject.toml
--rw-r--r--   0        0        0    10274 2020-02-02 00:00:00.000000 typedal-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0     3589 2020-02-02 00:00:00.000000 typedal-1.2.1/CHANGELOG.md
+-rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 typedal-1.2.1/coverage.svg
+-rw-r--r--   0        0        0     7120 2020-02-02 00:00:00.000000 typedal-1.2.1/example_new.py
+-rw-r--r--   0        0        0     2872 2020-02-02 00:00:00.000000 typedal-1.2.1/example_old.py
+-rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 typedal-1.2.1/.github/workflows/su6.yml
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/.gitignore
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/@plugins_snapshot.json
+-rw-r--r--   0        0        0   177667 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/_ast.data.json
+-rw-r--r--   0        0        0     1567 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/_ast.meta.json
+-rw-r--r--   0        0        0    52400 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/_codecs.data.json
+-rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/_codecs.meta.json
+-rw-r--r--   0        0        0    18227 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/_collections_abc.data.json
+-rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/_collections_abc.meta.json
+-rw-r--r--   0        0        0     2923 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/_ctypes.data.json
+-rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/_ctypes.meta.json
+-rw-r--r--   0        0        0   170960 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/_decimal.data.json
+-rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/_decimal.meta.json
+-rw-r--r--   0        0        0    23362 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/abc.data.json
+-rw-r--r--   0        0        0     1574 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/abc.meta.json
+-rw-r--r--   0        0        0    60687 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/array.data.json
+-rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/array.meta.json
+-rw-r--r--   0        0        0  1054992 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/builtins.data.json
+-rw-r--r--   0        0        0     1721 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/builtins.meta.json
+-rw-r--r--   0        0        0   123328 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/codecs.data.json
+-rw-r--r--   0        0        0     1671 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/codecs.meta.json
+-rw-r--r--   0        0        0   104160 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/contextlib.data.json
+-rw-r--r--   0        0        0     1610 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/contextlib.meta.json
+-rw-r--r--   0        0        0    57612 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/dataclasses.data.json
+-rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/dataclasses.meta.json
+-rw-r--r--   0        0        0   142044 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/datetime.data.json
+-rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/datetime.meta.json
+-rw-r--r--   0        0        0     4911 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/decimal.data.json
+-rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/decimal.meta.json
+-rw-r--r--   0        0        0    61020 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/enum.data.json
+-rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/enum.meta.json
+-rw-r--r--   0        0        0    22399 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/genericpath.data.json
+-rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/genericpath.meta.json
+-rw-r--r--   0        0        0    85348 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/io.data.json
+-rw-r--r--   0        0        0     1673 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/io.meta.json
+-rw-r--r--   0        0        0    28778 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/mmap.data.json
+-rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/mmap.meta.json
+-rw-r--r--   0        0        0    78982 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/numbers.data.json
+-rw-r--r--   0        0        0     1519 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/numbers.meta.json
+-rw-r--r--   0        0        0    88278 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/pathlib.data.json
+-rw-r--r--   0        0        0     1682 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/pathlib.meta.json
+-rw-r--r--   0        0        0    45131 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/pickle.data.json
+-rw-r--r--   0        0        0     1630 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/pickle.meta.json
+-rw-r--r--   0        0        0    75208 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/posixpath.data.json
+-rw-r--r--   0        0        0     1627 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/posixpath.meta.json
+-rw-r--r--   0        0        0   167175 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/re.data.json
+-rw-r--r--   0        0        0     1701 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/re.meta.json
+-rw-r--r--   0        0        0    14131 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/sre_compile.data.json
+-rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/sre_compile.meta.json
+-rw-r--r--   0        0        0    28013 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/sre_constants.data.json
+-rw-r--r--   0        0        0     1584 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/sre_constants.meta.json
+-rw-r--r--   0        0        0    49442 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/sre_parse.data.json
+-rw-r--r--   0        0        0     1627 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/sre_parse.meta.json
+-rw-r--r--   0        0        0   168498 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/subprocess.data.json
+-rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/subprocess.meta.json
+-rw-r--r--   0        0        0   146267 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/sys.data.json
+-rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/sys.meta.json
+-rw-r--r--   0        0        0    43605 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/time.data.json
+-rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/time.meta.json
+-rw-r--r--   0        0        0   228230 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/types.data.json
+-rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/types.meta.json
+-rw-r--r--   0        0        0   416965 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/typing.data.json
+-rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/typing.meta.json
+-rw-r--r--   0        0        0    73907 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/typing_extensions.data.json
+-rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/typing_extensions.meta.json
+-rw-r--r--   0        0        0    89065 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/_typeshed/__init__.data.json
+-rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/_typeshed/__init__.meta.json
+-rw-r--r--   0        0        0   407999 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/collections/__init__.data.json
+-rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/collections/__init__.meta.json
+-rw-r--r--   0        0        0     3731 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/collections/abc.data.json
+-rw-r--r--   0        0        0     1558 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/collections/abc.meta.json
+-rw-r--r--   0        0        0   128994 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/ctypes/__init__.data.json
+-rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/ctypes/__init__.meta.json
+-rw-r--r--   0        0        0     7438 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/email/__init__.data.json
+-rw-r--r--   0        0        0     1610 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/email/__init__.meta.json
+-rw-r--r--   0        0        0    12200 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/email/charset.data.json
+-rw-r--r--   0        0        0     1555 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/email/charset.meta.json
+-rw-r--r--   0        0        0     7249 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/email/contentmanager.data.json
+-rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/email/contentmanager.meta.json
+-rw-r--r--   0        0        0    25073 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/email/errors.data.json
+-rw-r--r--   0        0        0     1559 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/email/errors.meta.json
+-rw-r--r--   0        0        0     9154 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/email/header.data.json
+-rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/email/header.meta.json
+-rw-r--r--   0        0        0    79298 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/email/message.data.json
+-rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/email/message.meta.json
+-rw-r--r--   0        0        0    30857 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/email/policy.data.json
+-rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/email/policy.meta.json
+-rw-r--r--   0        0        0     6125 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/importlib/__init__.data.json
+-rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/importlib/__init__.meta.json
+-rw-r--r--   0        0        0    70175 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/importlib/abc.data.json
+-rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/importlib/abc.meta.json
+-rw-r--r--   0        0        0    64626 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/importlib/machinery.data.json
+-rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/importlib/machinery.meta.json
+-rw-r--r--   0        0        0    90277 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/importlib/metadata/__init__.data.json
+-rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/importlib/metadata/__init__.meta.json
+-rw-r--r--   0        0        0    11935 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/importlib/metadata/_meta.data.json
+-rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/importlib/metadata/_meta.meta.json
+-rw-r--r--   0        0        0   350178 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/os/__init__.data.json
+-rw-r--r--   0        0        0     1725 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/os/__init__.meta.json
+-rw-r--r--   0        0        0     4908 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/os/path.data.json
+-rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/os/path.meta.json
+-rw-r--r--   0        0        0     1385 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/src/__init__.data.json
+-rw-r--r--   0        0        0     1433 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/src/__init__.meta.json
+-rw-r--r--   0        0        0     1506 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/src/typedal/__about__.data.json
+-rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/src/typedal/__about__.meta.json
+-rw-r--r--   0        0        0     2114 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/src/typedal/__init__.data.json
+-rw-r--r--   0        0        0     1499 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/src/typedal/__init__.meta.json
+-rw-r--r--   0        0        0    33347 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/src/typedal/core.data.json
+-rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/src/typedal/core.meta.json
+-rw-r--r--   0        0        0    29038 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/src/typedal/fields.data.json
+-rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/src/typedal/fields.meta.json
+-rw-r--r--   0        0        0     2775 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/src/typedal/pydal_objects.data.json
+-rw-r--r--   0        0        0     1503 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.10/src/typedal/pydal_objects.meta.json
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/@plugins_snapshot.json
+-rw-r--r--   0        0        0   180368 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/_ast.data.json
+-rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/_ast.meta.json
+-rw-r--r--   0        0        0    52400 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/_codecs.data.json
+-rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/_codecs.meta.json
+-rw-r--r--   0        0        0    18227 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/_collections_abc.data.json
+-rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/_collections_abc.meta.json
+-rw-r--r--   0        0        0     3125 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/_ctypes.data.json
+-rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/_ctypes.meta.json
+-rw-r--r--   0        0        0   171931 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/_decimal.data.json
+-rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/_decimal.meta.json
+-rw-r--r--   0        0        0    23336 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/abc.data.json
+-rw-r--r--   0        0        0     1574 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/abc.meta.json
+-rw-r--r--   0        0        0    60676 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/array.data.json
+-rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/array.meta.json
+-rw-r--r--   0        0        0  1130454 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/builtins.data.json
+-rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/builtins.meta.json
+-rw-r--r--   0        0        0   123317 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/codecs.data.json
+-rw-r--r--   0        0        0     1671 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/codecs.meta.json
+-rw-r--r--   0        0        0   109204 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/contextlib.data.json
+-rw-r--r--   0        0        0     1610 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/contextlib.meta.json
+-rw-r--r--   0        0        0    57745 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/dataclasses.data.json
+-rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/dataclasses.meta.json
+-rw-r--r--   0        0        0   142208 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/datetime.data.json
+-rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/datetime.meta.json
+-rw-r--r--   0        0        0     4911 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/decimal.data.json
+-rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/decimal.meta.json
+-rw-r--r--   0        0        0    90123 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/enum.data.json
+-rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/enum.meta.json
+-rw-r--r--   0        0        0    27481 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/example_new.data.json
+-rw-r--r--   0        0        0     1695 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/example_new.meta.json
+-rw-r--r--   0        0        0    22388 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/genericpath.data.json
+-rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/genericpath.meta.json
+-rw-r--r--   0        0        0    85337 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/io.data.json
+-rw-r--r--   0        0        0     1673 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/io.meta.json
+-rw-r--r--   0        0        0    28767 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/mmap.data.json
+-rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/mmap.meta.json
+-rw-r--r--   0        0        0    78982 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/numbers.data.json
+-rw-r--r--   0        0        0     1519 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/numbers.meta.json
+-rw-r--r--   0        0        0    87488 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/pathlib.data.json
+-rw-r--r--   0        0        0     1682 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/pathlib.meta.json
+-rw-r--r--   0        0        0    45131 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/pickle.data.json
+-rw-r--r--   0        0        0     1630 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/pickle.meta.json
+-rw-r--r--   0        0        0    75197 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/posixpath.data.json
+-rw-r--r--   0        0        0     1627 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/posixpath.meta.json
+-rw-r--r--   0        0        0   167545 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/re.data.json
+-rw-r--r--   0        0        0     1701 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/re.meta.json
+-rw-r--r--   0        0        0     1181 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/src.data.json
+-rw-r--r--   0        0        0     1391 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/src.meta.json
+-rw-r--r--   0        0        0    14373 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/sre_compile.data.json
+-rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/sre_compile.meta.json
+-rw-r--r--   0        0        0    28480 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/sre_constants.data.json
+-rw-r--r--   0        0        0     1584 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/sre_constants.meta.json
+-rw-r--r--   0        0        0    49741 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/sre_parse.data.json
+-rw-r--r--   0        0        0     1627 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/sre_parse.meta.json
+-rw-r--r--   0        0        0   172768 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/subprocess.data.json
+-rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/subprocess.meta.json
+-rw-r--r--   0        0        0   148675 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/sys.data.json
+-rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/sys.meta.json
+-rw-r--r--   0        0        0    43605 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/time.data.json
+-rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/time.meta.json
+-rw-r--r--   0        0        0   239632 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/types.data.json
+-rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/types.meta.json
+-rw-r--r--   0        0        0   432234 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/typing.data.json
+-rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/typing.meta.json
+-rw-r--r--   0        0        0    57845 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/typing_extensions.data.json
+-rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/typing_extensions.meta.json
+-rw-r--r--   0        0        0    89054 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/_typeshed/__init__.data.json
+-rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/_typeshed/__init__.meta.json
+-rw-r--r--   0        0        0   407988 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/collections/__init__.data.json
+-rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/collections/__init__.meta.json
+-rw-r--r--   0        0        0     3731 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/collections/abc.data.json
+-rw-r--r--   0        0        0     1558 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/collections/abc.meta.json
+-rw-r--r--   0        0        0   128983 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/ctypes/__init__.data.json
+-rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/ctypes/__init__.meta.json
+-rw-r--r--   0        0        0     7438 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/email/__init__.data.json
+-rw-r--r--   0        0        0     1610 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/email/__init__.meta.json
+-rw-r--r--   0        0        0    12200 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/email/charset.data.json
+-rw-r--r--   0        0        0     1555 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/email/charset.meta.json
+-rw-r--r--   0        0        0     7249 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/email/contentmanager.data.json
+-rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/email/contentmanager.meta.json
+-rw-r--r--   0        0        0    25073 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/email/errors.data.json
+-rw-r--r--   0        0        0     1559 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/email/errors.meta.json
+-rw-r--r--   0        0        0     9154 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/email/header.data.json
+-rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/email/header.meta.json
+-rw-r--r--   0        0        0    79287 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/email/message.data.json
+-rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/email/message.meta.json
+-rw-r--r--   0        0        0    30857 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/email/policy.data.json
+-rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/email/policy.meta.json
+-rw-r--r--   0        0        0     6125 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/importlib/__init__.data.json
+-rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/importlib/__init__.meta.json
+-rw-r--r--   0        0        0    70579 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/importlib/abc.data.json
+-rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/importlib/abc.meta.json
+-rw-r--r--   0        0        0    64626 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/importlib/machinery.data.json
+-rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/importlib/machinery.meta.json
+-rw-r--r--   0        0        0    91119 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/importlib/metadata/__init__.data.json
+-rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/importlib/metadata/__init__.meta.json
+-rw-r--r--   0        0        0    11935 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/importlib/metadata/_meta.data.json
+-rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/importlib/metadata/_meta.meta.json
+-rw-r--r--   0        0        0   350743 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/os/__init__.data.json
+-rw-r--r--   0        0        0     1725 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/os/__init__.meta.json
+-rw-r--r--   0        0        0     4908 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/os/path.data.json
+-rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/os/path.meta.json
+-rw-r--r--   0        0        0     1385 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/src/__init__.data.json
+-rw-r--r--   0        0        0     1433 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/src/__init__.meta.json
+-rw-r--r--   0        0        0     1506 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/src/typedal/__about__.data.json
+-rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/src/typedal/__about__.meta.json
+-rw-r--r--   0        0        0     2357 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/src/typedal/__init__.data.json
+-rw-r--r--   0        0        0     1530 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/src/typedal/__init__.meta.json
+-rw-r--r--   0        0        0    43623 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/src/typedal/core.data.json
+-rw-r--r--   0        0        0     1737 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/src/typedal/core.meta.json
+-rw-r--r--   0        0        0    28504 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/src/typedal/fields.data.json
+-rw-r--r--   0        0        0     1687 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/src/typedal/fields.meta.json
+-rw-r--r--   0        0        0     1478 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/typedal/__about__.data.json
+-rw-r--r--   0        0        0     1458 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/typedal/__about__.meta.json
+-rw-r--r--   0        0        0     2274 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/typedal/__init__.data.json
+-rw-r--r--   0        0        0     1487 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/typedal/__init__.meta.json
+-rw-r--r--   0        0        0    42844 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/typedal/core.data.json
+-rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/typedal/core.meta.json
+-rw-r--r--   0        0        0    28193 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/typedal/fields.data.json
+-rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 typedal-1.2.1/.mypy_cache/3.11/typedal/fields.meta.json
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 typedal-1.2.1/.pytest_cache/.gitignore
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 typedal-1.2.1/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 typedal-1.2.1/.pytest_cache/README.md
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 typedal-1.2.1/.pytest_cache/v/cache/lastfailed
+-rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 typedal-1.2.1/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 typedal-1.2.1/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 typedal-1.2.1/.ruff_cache/.gitignore
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 typedal-1.2.1/.ruff_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 typedal-1.2.1/.ruff_cache/content/1215429078721865123
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.1/.ruff_cache/content/121ed75fe9fe5f8e
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.1/.ruff_cache/content/19309938546e93ab
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.1/.ruff_cache/content/197f3188bc94f91f
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.1/.ruff_cache/content/1aa1390b5bde1004
+-rw-r--r--   0        0        0     8089 2020-02-02 00:00:00.000000 typedal-1.2.1/.ruff_cache/content/1b34455c399f0006
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.1/.ruff_cache/content/1bd1a229a4f4ee7f
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.1/.ruff_cache/content/1c46d1f378d28fbb
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.1/.ruff_cache/content/1ca71ee291d82018
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.1/.ruff_cache/content/1d6bb777df44b8ec
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.1/.ruff_cache/content/1dc8423cfb79eaa4
+-rw-r--r--   0        0        0      908 2020-02-02 00:00:00.000000 typedal-1.2.1/.ruff_cache/content/20585cf790eae81e
+-rw-r--r--   0        0        0    12122 2020-02-02 00:00:00.000000 typedal-1.2.1/.ruff_cache/content/221af82ae72a7f27
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.1/.ruff_cache/content/2282e801459c52a4
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.1/.ruff_cache/content/248c4e1a32c704cb
+-rw-r--r--   0        0        0    10858 2020-02-02 00:00:00.000000 typedal-1.2.1/.ruff_cache/content/24e1b4aab386ebc8
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.1/.ruff_cache/content/28b1d8ac7e2aab6b
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.1/.ruff_cache/content/2b7f7d266c8efaad
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.1/.ruff_cache/content/2bb6610cadf18e18
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.1/.ruff_cache/content/2dac345be8527adf
+-rw-r--r--   0        0        0    11525 2020-02-02 00:00:00.000000 typedal-1.2.1/.ruff_cache/content/2f3396c610fd7095
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.1/.ruff_cache/content/31731f8e74291475
+-rw-r--r--   0        0        0    13342 2020-02-02 00:00:00.000000 typedal-1.2.1/.ruff_cache/content/322af04e6d059ce5
+-rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 typedal-1.2.1/.ruff_cache/content/3826106cf4494de8
+-rw-r--r--   0        0        0    11210 2020-02-02 00:00:00.000000 typedal-1.2.1/.ruff_cache/content/38d5fd55b14a9d6c
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.1/.ruff_cache/content/3afc55a04b8f8bb2
+-rw-r--r--   0        0        0    12129 2020-02-02 00:00:00.000000 typedal-1.2.1/.ruff_cache/content/4022ee8774ccd98a
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.1/.ruff_cache/content/42f9a2406e74c24f
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.1/.ruff_cache/content/4696b157ff786f22
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.1/.ruff_cache/content/46a88ce266f1ad94
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.1/.ruff_cache/content/4a6edd5010cb9700
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.1/.ruff_cache/content/4d0230e9a81a468
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.1/.ruff_cache/content/52018ba3989fcaf7
+-rw-r--r--   0        0        0    13679 2020-02-02 00:00:00.000000 typedal-1.2.1/.ruff_cache/content/5491563776466765346
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.1/.ruff_cache/content/54e6ba8c25a22ffc
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.1/.ruff_cache/content/566d94db91d23339
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.1/.ruff_cache/content/5a67aed8f6b70cd5
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.1/.ruff_cache/content/5b076d769fa5cacd
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.1/.ruff_cache/content/5ceb1580c62ee794
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.1/.ruff_cache/content/6bc90dbb56504f96
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.1/.ruff_cache/content/6c52d14716eee431
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.1/.ruff_cache/content/6f0c8f98e4da1d48
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.1/.ruff_cache/content/74e52af774eebdbd
+-rw-r--r--   0        0        0    11023 2020-02-02 00:00:00.000000 typedal-1.2.1/.ruff_cache/content/75bd1769f6e29ed7
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.1/.ruff_cache/content/815ba2cfea236769
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.1/.ruff_cache/content/876d9a8d302e1c46
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.1/.ruff_cache/content/88e2927df9448936
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.1/.ruff_cache/content/8c4d3f5ef14b0167
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.1/.ruff_cache/content/8f8ec552e76f3eab
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.1/.ruff_cache/content/95c82d8566c6704c
+-rw-r--r--   0        0        0     8349 2020-02-02 00:00:00.000000 typedal-1.2.1/.ruff_cache/content/a0739889bf9412e8
+-rw-r--r--   0        0        0     5692 2020-02-02 00:00:00.000000 typedal-1.2.1/.ruff_cache/content/a225e4df39be9b29
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.1/.ruff_cache/content/a2340fd4c9aa1141
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.1/.ruff_cache/content/a513d558646cd439
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.1/.ruff_cache/content/b121e2b70fd66eb8
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.1/.ruff_cache/content/b218ff88bc22b626
+-rw-r--r--   0        0        0    10964 2020-02-02 00:00:00.000000 typedal-1.2.1/.ruff_cache/content/b419496fa9e72887
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.1/.ruff_cache/content/b886c97e4d4117f0
+-rw-r--r--   0        0        0     8238 2020-02-02 00:00:00.000000 typedal-1.2.1/.ruff_cache/content/bdcdf5c7bbc1d738
+-rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 typedal-1.2.1/.ruff_cache/content/c06de16f3c7a64cc
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.1/.ruff_cache/content/c635f255374598c5
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.1/.ruff_cache/content/c671ae94ff3d3e2e
+-rw-r--r--   0        0        0     8042 2020-02-02 00:00:00.000000 typedal-1.2.1/.ruff_cache/content/cdfecbca581311ee
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.1/.ruff_cache/content/ce44121ca4091b64
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.1/.ruff_cache/content/ced49ec87d10bcb0
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.1/.ruff_cache/content/cfc06a1f13c8ab47
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.1/.ruff_cache/content/d16c5d29763a704e
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.1/.ruff_cache/content/d225ad4c14b8ca60
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.1/.ruff_cache/content/d379b35d5e80b789
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.1/.ruff_cache/content/d3a95555c0919160
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.1/.ruff_cache/content/d655bee8ff0a59f2
+-rw-r--r--   0        0        0    11315 2020-02-02 00:00:00.000000 typedal-1.2.1/.ruff_cache/content/da4811a7730a562a
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.1/.ruff_cache/content/dca573767bc8be7e
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.1/.ruff_cache/content/e3e29f9eacb7027f
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.1/.ruff_cache/content/e46ab4b61bb5d446
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.1/.ruff_cache/content/e5e0cc178d5c9df5
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.1/.ruff_cache/content/eb564f7989641958
+-rw-r--r--   0        0        0    11467 2020-02-02 00:00:00.000000 typedal-1.2.1/.ruff_cache/content/eee2f3c667de6c7a
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.1/.ruff_cache/content/f04d0d78a00adfd6
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.1/.ruff_cache/content/f2ddc22a4b221f54
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.1/.ruff_cache/content/f879e8c947a6b7a4
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.1/.ruff_cache/content/fa45ef3c3166e02d
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 typedal-1.2.1/.ruff_cache/content/faa51a5044a3c279
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 typedal-1.2.1/htmlcov/.gitignore
+-rw-r--r--   0        0        0    21359 2020-02-02 00:00:00.000000 typedal-1.2.1/htmlcov/coverage_html.js
+-rw-r--r--   0        0        0     5891 2020-02-02 00:00:00.000000 typedal-1.2.1/htmlcov/d_0ccc93afd6526b6c___about___py.html
+-rw-r--r--   0        0        0     6664 2020-02-02 00:00:00.000000 typedal-1.2.1/htmlcov/d_0ccc93afd6526b6c___init___py.html
+-rw-r--r--   0        0        0   127189 2020-02-02 00:00:00.000000 typedal-1.2.1/htmlcov/d_0ccc93afd6526b6c_core_py.html
+-rw-r--r--   0        0        0    60671 2020-02-02 00:00:00.000000 typedal-1.2.1/htmlcov/d_0ccc93afd6526b6c_fields_py.html
+-rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 typedal-1.2.1/htmlcov/favicon_32.png
+-rw-r--r--   0        0        0     4825 2020-02-02 00:00:00.000000 typedal-1.2.1/htmlcov/index.html
+-rw-r--r--   0        0        0     9004 2020-02-02 00:00:00.000000 typedal-1.2.1/htmlcov/keybd_closed.png
+-rw-r--r--   0        0        0     9003 2020-02-02 00:00:00.000000 typedal-1.2.1/htmlcov/keybd_open.png
+-rw-r--r--   0        0        0      922 2020-02-02 00:00:00.000000 typedal-1.2.1/htmlcov/status.json
+-rw-r--r--   0        0        0    12387 2020-02-02 00:00:00.000000 typedal-1.2.1/htmlcov/style.css
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 typedal-1.2.1/src/typedal/__about__.py
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 typedal-1.2.1/src/typedal/__init__.py
+-rw-r--r--   0        0        0    15559 2020-02-02 00:00:00.000000 typedal-1.2.1/src/typedal/core.py
+-rw-r--r--   0        0        0     4949 2020-02-02 00:00:00.000000 typedal-1.2.1/src/typedal/fields.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 typedal-1.2.1/src/typedal/py.typed
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 typedal-1.2.1/tests/__init__.py
+-rw-r--r--   0        0        0     9736 2020-02-02 00:00:00.000000 typedal-1.2.1/tests/test_main.py
+-rw-r--r--   0        0        0     1228 2020-02-02 00:00:00.000000 typedal-1.2.1/tests/test_mypy.py
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 typedal-1.2.1/.gitignore
+-rw-r--r--   0        0        0     9220 2020-02-02 00:00:00.000000 typedal-1.2.1/README.md
+-rw-r--r--   0        0        0     4782 2020-02-02 00:00:00.000000 typedal-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0    10274 2020-02-02 00:00:00.000000 typedal-1.2.1/PKG-INFO
```

### Comparing `typedal-1.2.0/CHANGELOG.md` & `typedal-1.2.1/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,16 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
+## v1.2.1 (2023-06-27)
+### Fix
+
+* Typehint query options for db() and update_or_insert() ([`2b65f58`](https://github.com/trialandsuccess/TypeDAL/commit/2b65f58ccf93f12713877fd420ec43454911efe9))
+
 ## v1.2.0 (2023-06-27)
 ### Feature
 
 * **set:** Type hints for .count() and .select() ([`1f23581`](https://github.com/trialandsuccess/TypeDAL/commit/1f2358169c6690e36153e99983c53a6c370f5e40))
 
 ## v1.1.2 (2023-06-27)
 ### Fix
```

### Comparing `typedal-1.2.0/coverage.svg` & `typedal-1.2.1/coverage.svg`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/example_new.py` & `typedal-1.2.1/example_new.py`

 * *Files 6% similar despite different names*

```diff
@@ -55,14 +55,20 @@
 people: TypedRows[Person] = db(Person).select()  # db(db.person.id > 0).select()
 
 print(people.first())
 
 for person in people:
     print(person.nicknames)
 
+# max ran away!
+Pet.update_or_insert(Pet.name == "Max", owners=[])
+max = Pet(name="Max")
+
+assert not max.owners
+
 
 ### example with all possible field types;
 
 @db.define
 class OtherTable(TypedTable):
     ...
```

### Comparing `typedal-1.2.0/example_old.py` & `typedal-1.2.1/example_old.py`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.10/_ast.data.json` & `typedal-1.2.1/.mypy_cache/3.10/_ast.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.10/_ast.meta.json` & `typedal-1.2.1/.mypy_cache/3.10/_ast.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.10/_codecs.data.json` & `typedal-1.2.1/.mypy_cache/3.10/_codecs.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.10/_codecs.meta.json` & `typedal-1.2.1/.mypy_cache/3.10/_codecs.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.10/_collections_abc.data.json` & `typedal-1.2.1/.mypy_cache/3.10/_collections_abc.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.10/_collections_abc.meta.json` & `typedal-1.2.1/.mypy_cache/3.10/_collections_abc.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.10/_ctypes.data.json` & `typedal-1.2.1/.mypy_cache/3.10/_ctypes.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.10/_ctypes.meta.json` & `typedal-1.2.1/.mypy_cache/3.10/_ctypes.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.10/_decimal.data.json` & `typedal-1.2.1/.mypy_cache/3.10/_decimal.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.10/_decimal.meta.json` & `typedal-1.2.1/.mypy_cache/3.10/_decimal.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.10/abc.data.json` & `typedal-1.2.1/.mypy_cache/3.10/abc.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.10/abc.meta.json` & `typedal-1.2.1/.mypy_cache/3.10/abc.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.10/array.data.json` & `typedal-1.2.1/.mypy_cache/3.10/array.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.10/array.meta.json` & `typedal-1.2.1/.mypy_cache/3.10/array.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.10/builtins.data.json` & `typedal-1.2.1/.mypy_cache/3.10/builtins.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.10/builtins.meta.json` & `typedal-1.2.1/.mypy_cache/3.10/builtins.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.10/codecs.data.json` & `typedal-1.2.1/.mypy_cache/3.10/codecs.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.10/codecs.meta.json` & `typedal-1.2.1/.mypy_cache/3.10/codecs.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.10/contextlib.data.json` & `typedal-1.2.1/.mypy_cache/3.10/contextlib.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.10/contextlib.meta.json` & `typedal-1.2.1/.mypy_cache/3.10/contextlib.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.10/dataclasses.data.json` & `typedal-1.2.1/.mypy_cache/3.10/dataclasses.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.10/dataclasses.meta.json` & `typedal-1.2.1/.mypy_cache/3.10/dataclasses.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.10/datetime.data.json` & `typedal-1.2.1/.mypy_cache/3.10/datetime.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.10/datetime.meta.json` & `typedal-1.2.1/.mypy_cache/3.10/datetime.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.10/decimal.data.json` & `typedal-1.2.1/.mypy_cache/3.10/decimal.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.10/decimal.meta.json` & `typedal-1.2.1/.mypy_cache/3.10/decimal.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.10/enum.data.json` & `typedal-1.2.1/.mypy_cache/3.10/enum.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.10/enum.meta.json` & `typedal-1.2.1/.mypy_cache/3.10/enum.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.10/genericpath.data.json` & `typedal-1.2.1/.mypy_cache/3.10/genericpath.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.10/genericpath.meta.json` & `typedal-1.2.1/.mypy_cache/3.10/genericpath.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.10/io.data.json` & `typedal-1.2.1/.mypy_cache/3.10/io.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.10/io.meta.json` & `typedal-1.2.1/.mypy_cache/3.10/io.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.10/mmap.data.json` & `typedal-1.2.1/.mypy_cache/3.10/mmap.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.10/mmap.meta.json` & `typedal-1.2.1/.mypy_cache/3.10/mmap.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.10/numbers.data.json` & `typedal-1.2.1/.mypy_cache/3.10/numbers.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.10/numbers.meta.json` & `typedal-1.2.1/.mypy_cache/3.10/numbers.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.10/pathlib.data.json` & `typedal-1.2.1/.mypy_cache/3.10/pathlib.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.10/pathlib.meta.json` & `typedal-1.2.1/.mypy_cache/3.10/pathlib.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.10/pickle.data.json` & `typedal-1.2.1/.mypy_cache/3.10/pickle.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.10/pickle.meta.json` & `typedal-1.2.1/.mypy_cache/3.10/pickle.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.10/posixpath.data.json` & `typedal-1.2.1/.mypy_cache/3.10/posixpath.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.10/posixpath.meta.json` & `typedal-1.2.1/.mypy_cache/3.10/posixpath.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.10/re.data.json` & `typedal-1.2.1/.mypy_cache/3.10/re.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.10/re.meta.json` & `typedal-1.2.1/.mypy_cache/3.10/re.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.10/sre_compile.data.json` & `typedal-1.2.1/.mypy_cache/3.10/sre_compile.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.10/sre_compile.meta.json` & `typedal-1.2.1/.mypy_cache/3.10/sre_compile.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.10/sre_constants.data.json` & `typedal-1.2.1/.mypy_cache/3.10/sre_constants.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.10/sre_constants.meta.json` & `typedal-1.2.1/.mypy_cache/3.10/sre_constants.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.10/sre_parse.data.json` & `typedal-1.2.1/.mypy_cache/3.10/sre_parse.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.10/sre_parse.meta.json` & `typedal-1.2.1/.mypy_cache/3.10/sre_parse.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.10/subprocess.data.json` & `typedal-1.2.1/.mypy_cache/3.10/subprocess.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.10/subprocess.meta.json` & `typedal-1.2.1/.mypy_cache/3.10/subprocess.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.10/sys.data.json` & `typedal-1.2.1/.mypy_cache/3.10/sys.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.10/sys.meta.json` & `typedal-1.2.1/.mypy_cache/3.10/sys.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.10/time.data.json` & `typedal-1.2.1/.mypy_cache/3.10/time.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.10/time.meta.json` & `typedal-1.2.1/.mypy_cache/3.10/time.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.10/types.data.json` & `typedal-1.2.1/.mypy_cache/3.10/types.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.10/types.meta.json` & `typedal-1.2.1/.mypy_cache/3.10/types.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.10/typing.data.json` & `typedal-1.2.1/.mypy_cache/3.10/typing.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.10/typing.meta.json` & `typedal-1.2.1/.mypy_cache/3.10/typing.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.10/typing_extensions.data.json` & `typedal-1.2.1/.mypy_cache/3.10/typing_extensions.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.10/typing_extensions.meta.json` & `typedal-1.2.1/.mypy_cache/3.10/typing_extensions.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.10/_typeshed/__init__.data.json` & `typedal-1.2.1/.mypy_cache/3.10/_typeshed/__init__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.10/_typeshed/__init__.meta.json` & `typedal-1.2.1/.mypy_cache/3.10/_typeshed/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.10/collections/__init__.data.json` & `typedal-1.2.1/.mypy_cache/3.10/collections/__init__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.10/collections/__init__.meta.json` & `typedal-1.2.1/.mypy_cache/3.10/collections/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.10/collections/abc.data.json` & `typedal-1.2.1/.mypy_cache/3.10/collections/abc.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.10/collections/abc.meta.json` & `typedal-1.2.1/.mypy_cache/3.10/collections/abc.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.10/ctypes/__init__.data.json` & `typedal-1.2.1/.mypy_cache/3.10/ctypes/__init__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.10/ctypes/__init__.meta.json` & `typedal-1.2.1/.mypy_cache/3.10/ctypes/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.10/email/__init__.data.json` & `typedal-1.2.1/.mypy_cache/3.10/email/__init__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.10/email/__init__.meta.json` & `typedal-1.2.1/.mypy_cache/3.10/email/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.10/email/charset.data.json` & `typedal-1.2.1/.mypy_cache/3.10/email/charset.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.10/email/charset.meta.json` & `typedal-1.2.1/.mypy_cache/3.10/email/charset.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.10/email/contentmanager.data.json` & `typedal-1.2.1/.mypy_cache/3.10/email/contentmanager.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.10/email/contentmanager.meta.json` & `typedal-1.2.1/.mypy_cache/3.10/email/contentmanager.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.10/email/errors.data.json` & `typedal-1.2.1/.mypy_cache/3.10/email/errors.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.10/email/errors.meta.json` & `typedal-1.2.1/.mypy_cache/3.10/email/errors.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.10/email/header.data.json` & `typedal-1.2.1/.mypy_cache/3.10/email/header.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.10/email/header.meta.json` & `typedal-1.2.1/.mypy_cache/3.10/email/header.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.10/email/message.data.json` & `typedal-1.2.1/.mypy_cache/3.10/email/message.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.10/email/message.meta.json` & `typedal-1.2.1/.mypy_cache/3.10/email/message.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.10/email/policy.data.json` & `typedal-1.2.1/.mypy_cache/3.10/email/policy.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.10/email/policy.meta.json` & `typedal-1.2.1/.mypy_cache/3.10/email/policy.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.10/importlib/__init__.data.json` & `typedal-1.2.1/.mypy_cache/3.10/importlib/__init__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.10/importlib/__init__.meta.json` & `typedal-1.2.1/.mypy_cache/3.10/importlib/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.10/importlib/abc.data.json` & `typedal-1.2.1/.mypy_cache/3.10/importlib/abc.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.10/importlib/abc.meta.json` & `typedal-1.2.1/.mypy_cache/3.10/importlib/abc.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.10/importlib/machinery.data.json` & `typedal-1.2.1/.mypy_cache/3.10/importlib/machinery.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.10/importlib/machinery.meta.json` & `typedal-1.2.1/.mypy_cache/3.10/importlib/machinery.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.10/importlib/metadata/__init__.data.json` & `typedal-1.2.1/.mypy_cache/3.10/importlib/metadata/__init__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.10/importlib/metadata/__init__.meta.json` & `typedal-1.2.1/.mypy_cache/3.10/importlib/metadata/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.10/importlib/metadata/_meta.data.json` & `typedal-1.2.1/.mypy_cache/3.10/importlib/metadata/_meta.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.10/importlib/metadata/_meta.meta.json` & `typedal-1.2.1/.mypy_cache/3.10/importlib/metadata/_meta.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.10/os/__init__.data.json` & `typedal-1.2.1/.mypy_cache/3.10/os/__init__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.10/os/__init__.meta.json` & `typedal-1.2.1/.mypy_cache/3.10/os/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.10/os/path.data.json` & `typedal-1.2.1/.mypy_cache/3.10/os/path.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.10/os/path.meta.json` & `typedal-1.2.1/.mypy_cache/3.10/os/path.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.10/src/__init__.data.json` & `typedal-1.2.1/.mypy_cache/3.10/src/__init__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.10/src/__init__.meta.json` & `typedal-1.2.1/.mypy_cache/3.10/src/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.10/src/typedal/__about__.data.json` & `typedal-1.2.1/.mypy_cache/3.10/src/typedal/__about__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.10/src/typedal/__about__.meta.json` & `typedal-1.2.1/.mypy_cache/3.10/src/typedal/__about__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.10/src/typedal/__init__.data.json` & `typedal-1.2.1/.mypy_cache/3.10/src/typedal/__init__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.10/src/typedal/__init__.meta.json` & `typedal-1.2.1/.mypy_cache/3.10/src/typedal/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.10/src/typedal/core.data.json` & `typedal-1.2.1/.mypy_cache/3.10/src/typedal/core.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.10/src/typedal/core.meta.json` & `typedal-1.2.1/.mypy_cache/3.10/src/typedal/core.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.10/src/typedal/fields.data.json` & `typedal-1.2.1/.mypy_cache/3.10/src/typedal/fields.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.10/src/typedal/fields.meta.json` & `typedal-1.2.1/.mypy_cache/3.10/src/typedal/fields.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.10/src/typedal/pydal_objects.data.json` & `typedal-1.2.1/.mypy_cache/3.10/src/typedal/pydal_objects.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.10/src/typedal/pydal_objects.meta.json` & `typedal-1.2.1/.mypy_cache/3.10/src/typedal/pydal_objects.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.11/_ast.data.json` & `typedal-1.2.1/.mypy_cache/3.11/_ast.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.11/_ast.meta.json` & `typedal-1.2.1/.mypy_cache/3.11/_ast.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.11/_codecs.data.json` & `typedal-1.2.1/.mypy_cache/3.11/_codecs.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.11/_codecs.meta.json` & `typedal-1.2.1/.mypy_cache/3.11/_codecs.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.11/_collections_abc.data.json` & `typedal-1.2.1/.mypy_cache/3.11/_collections_abc.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.11/_collections_abc.meta.json` & `typedal-1.2.1/.mypy_cache/3.11/_collections_abc.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.11/_ctypes.data.json` & `typedal-1.2.1/.mypy_cache/3.11/_ctypes.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.11/_ctypes.meta.json` & `typedal-1.2.1/.mypy_cache/3.11/_ctypes.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.11/_decimal.data.json` & `typedal-1.2.1/.mypy_cache/3.11/_decimal.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.11/_decimal.meta.json` & `typedal-1.2.1/.mypy_cache/3.11/_decimal.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.11/abc.data.json` & `typedal-1.2.1/.mypy_cache/3.11/abc.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.11/abc.meta.json` & `typedal-1.2.1/.mypy_cache/3.11/abc.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.11/array.data.json` & `typedal-1.2.1/.mypy_cache/3.11/array.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.11/array.meta.json` & `typedal-1.2.1/.mypy_cache/3.11/array.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.11/builtins.data.json` & `typedal-1.2.1/.mypy_cache/3.11/builtins.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.11/builtins.meta.json` & `typedal-1.2.1/.mypy_cache/3.11/builtins.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.11/codecs.data.json` & `typedal-1.2.1/.mypy_cache/3.11/codecs.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.11/codecs.meta.json` & `typedal-1.2.1/.mypy_cache/3.11/codecs.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.11/contextlib.data.json` & `typedal-1.2.1/.mypy_cache/3.11/contextlib.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.11/contextlib.meta.json` & `typedal-1.2.1/.mypy_cache/3.11/contextlib.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.11/dataclasses.data.json` & `typedal-1.2.1/.mypy_cache/3.11/dataclasses.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.11/dataclasses.meta.json` & `typedal-1.2.1/.mypy_cache/3.11/dataclasses.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.11/datetime.data.json` & `typedal-1.2.1/.mypy_cache/3.11/datetime.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.11/datetime.meta.json` & `typedal-1.2.1/.mypy_cache/3.11/datetime.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.11/decimal.data.json` & `typedal-1.2.1/.mypy_cache/3.11/decimal.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.11/decimal.meta.json` & `typedal-1.2.1/.mypy_cache/3.11/decimal.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.11/enum.data.json` & `typedal-1.2.1/.mypy_cache/3.11/enum.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.11/enum.meta.json` & `typedal-1.2.1/.mypy_cache/3.11/enum.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.11/genericpath.data.json` & `typedal-1.2.1/.mypy_cache/3.11/genericpath.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.11/genericpath.meta.json` & `typedal-1.2.1/.mypy_cache/3.11/genericpath.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.11/io.data.json` & `typedal-1.2.1/.mypy_cache/3.11/io.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.11/io.meta.json` & `typedal-1.2.1/.mypy_cache/3.11/io.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.11/mmap.data.json` & `typedal-1.2.1/.mypy_cache/3.11/mmap.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.11/mmap.meta.json` & `typedal-1.2.1/.mypy_cache/3.11/mmap.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.11/numbers.data.json` & `typedal-1.2.1/.mypy_cache/3.11/numbers.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.11/numbers.meta.json` & `typedal-1.2.1/.mypy_cache/3.11/numbers.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.11/pathlib.data.json` & `typedal-1.2.1/.mypy_cache/3.11/pathlib.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.11/pathlib.meta.json` & `typedal-1.2.1/.mypy_cache/3.11/pathlib.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.11/pickle.data.json` & `typedal-1.2.1/.mypy_cache/3.11/pickle.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.11/pickle.meta.json` & `typedal-1.2.1/.mypy_cache/3.11/pickle.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.11/posixpath.data.json` & `typedal-1.2.1/.mypy_cache/3.11/posixpath.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.11/posixpath.meta.json` & `typedal-1.2.1/.mypy_cache/3.11/posixpath.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.11/re.data.json` & `typedal-1.2.1/.mypy_cache/3.11/re.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.11/re.meta.json` & `typedal-1.2.1/.mypy_cache/3.11/re.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.11/src.data.json` & `typedal-1.2.1/.mypy_cache/3.11/src.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.11/src.meta.json` & `typedal-1.2.1/.mypy_cache/3.11/src.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.11/sre_compile.data.json` & `typedal-1.2.1/.mypy_cache/3.11/sre_compile.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.11/sre_compile.meta.json` & `typedal-1.2.1/.mypy_cache/3.11/sre_compile.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.11/sre_constants.data.json` & `typedal-1.2.1/.mypy_cache/3.11/sre_constants.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.11/sre_constants.meta.json` & `typedal-1.2.1/.mypy_cache/3.11/sre_constants.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.11/sre_parse.data.json` & `typedal-1.2.1/.mypy_cache/3.11/sre_parse.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.11/sre_parse.meta.json` & `typedal-1.2.1/.mypy_cache/3.11/sre_parse.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.11/subprocess.data.json` & `typedal-1.2.1/.mypy_cache/3.11/subprocess.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.11/subprocess.meta.json` & `typedal-1.2.1/.mypy_cache/3.11/subprocess.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.11/sys.data.json` & `typedal-1.2.1/.mypy_cache/3.11/sys.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.11/sys.meta.json` & `typedal-1.2.1/.mypy_cache/3.11/sys.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.11/time.data.json` & `typedal-1.2.1/.mypy_cache/3.11/time.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.11/time.meta.json` & `typedal-1.2.1/.mypy_cache/3.11/time.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.11/types.data.json` & `typedal-1.2.1/.mypy_cache/3.11/types.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.11/types.meta.json` & `typedal-1.2.1/.mypy_cache/3.11/types.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.11/typing.data.json` & `typedal-1.2.1/.mypy_cache/3.11/typing.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.11/typing.meta.json` & `typedal-1.2.1/.mypy_cache/3.11/typing.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.11/typing_extensions.data.json` & `typedal-1.2.1/.mypy_cache/3.11/typing_extensions.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.11/typing_extensions.meta.json` & `typedal-1.2.1/.mypy_cache/3.11/typing_extensions.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.11/_typeshed/__init__.data.json` & `typedal-1.2.1/.mypy_cache/3.11/_typeshed/__init__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.11/_typeshed/__init__.meta.json` & `typedal-1.2.1/.mypy_cache/3.11/_typeshed/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.11/collections/__init__.data.json` & `typedal-1.2.1/.mypy_cache/3.11/collections/__init__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.11/collections/__init__.meta.json` & `typedal-1.2.1/.mypy_cache/3.11/collections/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.11/collections/abc.data.json` & `typedal-1.2.1/.mypy_cache/3.11/collections/abc.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.11/collections/abc.meta.json` & `typedal-1.2.1/.mypy_cache/3.11/collections/abc.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.11/ctypes/__init__.data.json` & `typedal-1.2.1/.mypy_cache/3.11/ctypes/__init__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.11/ctypes/__init__.meta.json` & `typedal-1.2.1/.mypy_cache/3.11/ctypes/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.11/email/__init__.data.json` & `typedal-1.2.1/.mypy_cache/3.11/email/__init__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.11/email/__init__.meta.json` & `typedal-1.2.1/.mypy_cache/3.11/email/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.11/email/charset.data.json` & `typedal-1.2.1/.mypy_cache/3.11/email/charset.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.11/email/charset.meta.json` & `typedal-1.2.1/.mypy_cache/3.11/email/charset.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.11/email/contentmanager.data.json` & `typedal-1.2.1/.mypy_cache/3.11/email/contentmanager.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.11/email/contentmanager.meta.json` & `typedal-1.2.1/.mypy_cache/3.11/email/contentmanager.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.11/email/errors.data.json` & `typedal-1.2.1/.mypy_cache/3.11/email/errors.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.11/email/errors.meta.json` & `typedal-1.2.1/.mypy_cache/3.11/email/errors.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.11/email/header.data.json` & `typedal-1.2.1/.mypy_cache/3.11/email/header.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.11/email/header.meta.json` & `typedal-1.2.1/.mypy_cache/3.11/email/header.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.11/email/message.data.json` & `typedal-1.2.1/.mypy_cache/3.11/email/message.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.11/email/message.meta.json` & `typedal-1.2.1/.mypy_cache/3.11/email/message.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.11/email/policy.data.json` & `typedal-1.2.1/.mypy_cache/3.11/email/policy.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.11/email/policy.meta.json` & `typedal-1.2.1/.mypy_cache/3.11/email/policy.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.11/importlib/__init__.data.json` & `typedal-1.2.1/.mypy_cache/3.11/importlib/__init__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.11/importlib/__init__.meta.json` & `typedal-1.2.1/.mypy_cache/3.11/importlib/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.11/importlib/abc.data.json` & `typedal-1.2.1/.mypy_cache/3.11/importlib/abc.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.11/importlib/abc.meta.json` & `typedal-1.2.1/.mypy_cache/3.11/importlib/abc.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.11/importlib/machinery.data.json` & `typedal-1.2.1/.mypy_cache/3.11/importlib/machinery.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.11/importlib/machinery.meta.json` & `typedal-1.2.1/.mypy_cache/3.11/importlib/machinery.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.11/importlib/metadata/__init__.data.json` & `typedal-1.2.1/.mypy_cache/3.11/importlib/metadata/__init__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.11/importlib/metadata/__init__.meta.json` & `typedal-1.2.1/.mypy_cache/3.11/importlib/metadata/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.11/importlib/metadata/_meta.data.json` & `typedal-1.2.1/.mypy_cache/3.11/importlib/metadata/_meta.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.11/importlib/metadata/_meta.meta.json` & `typedal-1.2.1/.mypy_cache/3.11/importlib/metadata/_meta.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.11/os/__init__.data.json` & `typedal-1.2.1/.mypy_cache/3.11/os/__init__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.11/os/__init__.meta.json` & `typedal-1.2.1/.mypy_cache/3.11/os/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.11/os/path.data.json` & `typedal-1.2.1/.mypy_cache/3.11/os/path.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.11/os/path.meta.json` & `typedal-1.2.1/.mypy_cache/3.11/os/path.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.11/src/__init__.data.json` & `typedal-1.2.1/.mypy_cache/3.11/src/__init__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.11/src/__init__.meta.json` & `typedal-1.2.1/.mypy_cache/3.11/src/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.11/src/typedal/__about__.data.json` & `typedal-1.2.1/.mypy_cache/3.11/src/typedal/__about__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.11/src/typedal/__about__.meta.json` & `typedal-1.2.1/.mypy_cache/3.11/src/typedal/__about__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.11/src/typedal/__init__.data.json` & `typedal-1.2.1/.mypy_cache/3.11/src/typedal/__init__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.11/src/typedal/__init__.meta.json` & `typedal-1.2.1/.mypy_cache/3.11/src/typedal/__init__.meta.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9666666666666667%*

 * *Differences: {"'data_mtime'": '1687881806'}*

```diff
@@ -1,9 +1,9 @@
 {
-    "data_mtime": 1687879062,
+    "data_mtime": 1687881806,
     "dep_lines": [
         5,
         6,
         1,
         1,
         1
     ],
```

### Comparing `typedal-1.2.0/.mypy_cache/3.11/src/typedal/core.data.json` & `typedal-1.2.1/.mypy_cache/3.11/src/typedal/core.data.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9961184709528305%*

 * *Differences: {"'names'": "{'T_annotation': {'node': {'line': 15}}, 'TypeDAL': {'node': {'names': {'__call__': "*

 * *            "{'node': {'type': {'arg_types': {1: {'.class': 'TypeAliasType', 'args': [], "*

 * *            "'type_ref': 'src.typedal.core.T_Query', delete: ['missing_import_name', 'source_any', "*

 * *            "'type_of_any']}}}}}}}}, 'TypedRow': {'node': {'line': 346}}, 'TypedTable': {'node': "*

 * *            "{'names': {'update_or_insert': OrderedDict([('.class', 'SymbolTableNode'), ('kind', "*

 * *            "'Mdef'), ( […]*

```diff
@@ -124,14 +124,36 @@
         "ChainMap": {
             ".class": "SymbolTableNode",
             "cross_ref": "collections.ChainMap",
             "kind": "Gdef",
             "module_hidden": true,
             "module_public": false
         },
+        "DEFAULT": {
+            ".class": "SymbolTableNode",
+            "kind": "Gdef",
+            "module_hidden": true,
+            "module_public": false,
+            "node": {
+                ".class": "Var",
+                "flags": [
+                    "is_suppressed_import",
+                    "is_ready",
+                    "is_inferred"
+                ],
+                "fullname": "src.typedal.core.DEFAULT",
+                "name": "DEFAULT",
+                "type": {
+                    ".class": "AnyType",
+                    "missing_import_name": "src.typedal.core.DEFAULT",
+                    "source_any": null,
+                    "type_of_any": 3
+                }
+            }
+        },
         "Decimal": {
             ".class": "SymbolTableNode",
             "cross_ref": "_decimal.Decimal",
             "kind": "Gdef",
             "module_hidden": true,
             "module_public": false
         },
@@ -257,14 +279,53 @@
                             "type_of_any": 3
                         }
                     }
                 ],
                 "variance": 0
             }
         },
+        "T_Query": {
+            ".class": "SymbolTableNode",
+            "kind": "Gdef",
+            "node": {
+                ".class": "TypeAlias",
+                "alias_tvars": [],
+                "column": 0,
+                "fullname": "src.typedal.core.T_Query",
+                "line": 16,
+                "no_args": false,
+                "normalized": false,
+                "target": {
+                    ".class": "UnionType",
+                    "items": [
+                        {
+                            ".class": "AnyType",
+                            "missing_import_name": "src.typedal.core.Table",
+                            "source_any": null,
+                            "type_of_any": 3
+                        },
+                        {
+                            ".class": "AnyType",
+                            "missing_import_name": "src.typedal.core.Query",
+                            "source_any": null,
+                            "type_of_any": 3
+                        },
+                        "builtins.bool",
+                        {
+                            ".class": "NoneType"
+                        },
+                        "src.typedal.core.TypedTable",
+                        {
+                            ".class": "TypeType",
+                            "item": "src.typedal.core.TypedTable"
+                        }
+                    ]
+                }
+            }
+        },
         "T_Table": {
             ".class": "SymbolTableNode",
             "kind": "Gdef",
             "node": {
                 ".class": "TypeVarExpr",
                 "fullname": "src.typedal.core.T_Table",
                 "name": "T_Table",
@@ -282,15 +343,15 @@
             ".class": "SymbolTableNode",
             "kind": "Gdef",
             "node": {
                 ".class": "TypeAlias",
                 "alias_tvars": [],
                 "column": 0,
                 "fullname": "src.typedal.core.T_annotation",
-                "line": 14,
+                "line": 15,
                 "no_args": false,
                 "normalized": false,
                 "target": {
                     ".class": "UnionType",
                     "items": [
                         {
                             ".class": "TypeType",
@@ -393,18 +454,17 @@
                                     "self",
                                     "_args",
                                     "kwargs"
                                 ],
                                 "arg_types": [
                                     "src.typedal.core.TypeDAL",
                                     {
-                                        ".class": "AnyType",
-                                        "missing_import_name": null,
-                                        "source_any": null,
-                                        "type_of_any": 2
+                                        ".class": "TypeAliasType",
+                                        "args": [],
+                                        "type_ref": "src.typedal.core.T_Query"
                                     },
                                     {
                                         ".class": "AnyType",
                                         "missing_import_name": null,
                                         "source_any": null,
                                         "type_of_any": 2
                                     }
@@ -1570,15 +1630,15 @@
             ".class": "SymbolTableNode",
             "kind": "Gdef",
             "node": {
                 ".class": "TypeAlias",
                 "alias_tvars": [],
                 "column": 0,
                 "fullname": "src.typedal.core.TypedRow",
-                "line": 335,
+                "line": 346,
                 "no_args": true,
                 "normalized": false,
                 "target": "src.typedal.core.TypedTable"
             }
         },
         "TypedRows": {
             ".class": "SymbolTableNode",
@@ -2406,14 +2466,156 @@
                                     "ret_type": "builtins.int",
                                     "type_guard": null,
                                     "unpack_kwargs": false,
                                     "variables": []
                                 }
                             }
                         }
+                    },
+                    "update_or_insert": {
+                        ".class": "SymbolTableNode",
+                        "kind": "Mdef",
+                        "node": {
+                            ".class": "Decorator",
+                            "func": {
+                                ".class": "FuncDef",
+                                "abstract_status": 0,
+                                "arg_kinds": [
+                                    0,
+                                    1,
+                                    4
+                                ],
+                                "arg_names": [
+                                    "cls",
+                                    "query",
+                                    "values"
+                                ],
+                                "dataclass_transform_spec": null,
+                                "flags": [
+                                    "is_class",
+                                    "is_decorated"
+                                ],
+                                "fullname": "src.typedal.core.TypedTable.update_or_insert",
+                                "name": "update_or_insert",
+                                "type": {
+                                    ".class": "CallableType",
+                                    "arg_kinds": [
+                                        0,
+                                        1,
+                                        4
+                                    ],
+                                    "arg_names": [
+                                        "cls",
+                                        "query",
+                                        "values"
+                                    ],
+                                    "arg_types": [
+                                        {
+                                            ".class": "TypeType",
+                                            "item": "src.typedal.core.TypedTable"
+                                        },
+                                        {
+                                            ".class": "TypeAliasType",
+                                            "args": [],
+                                            "type_ref": "src.typedal.core.T_Query"
+                                        },
+                                        {
+                                            ".class": "AnyType",
+                                            "missing_import_name": null,
+                                            "source_any": null,
+                                            "type_of_any": 2
+                                        }
+                                    ],
+                                    "bound_args": [],
+                                    "def_extras": {
+                                        "first_arg": "cls"
+                                    },
+                                    "fallback": "builtins.function",
+                                    "from_concatenate": false,
+                                    "implicit": false,
+                                    "is_ellipsis_args": false,
+                                    "name": "update_or_insert of TypedTable",
+                                    "ret_type": {
+                                        ".class": "UnionType",
+                                        "items": [
+                                            "builtins.int",
+                                            {
+                                                ".class": "NoneType"
+                                            }
+                                        ]
+                                    },
+                                    "type_guard": null,
+                                    "unpack_kwargs": false,
+                                    "variables": []
+                                }
+                            },
+                            "is_overload": false,
+                            "var": {
+                                ".class": "Var",
+                                "flags": [
+                                    "is_initialized_in_class",
+                                    "is_classmethod",
+                                    "is_ready",
+                                    "is_inferred"
+                                ],
+                                "fullname": "src.typedal.core.TypedTable.update_or_insert",
+                                "name": "update_or_insert",
+                                "type": {
+                                    ".class": "CallableType",
+                                    "arg_kinds": [
+                                        0,
+                                        1,
+                                        4
+                                    ],
+                                    "arg_names": [
+                                        "cls",
+                                        "query",
+                                        "values"
+                                    ],
+                                    "arg_types": [
+                                        {
+                                            ".class": "TypeType",
+                                            "item": "src.typedal.core.TypedTable"
+                                        },
+                                        {
+                                            ".class": "TypeAliasType",
+                                            "args": [],
+                                            "type_ref": "src.typedal.core.T_Query"
+                                        },
+                                        {
+                                            ".class": "AnyType",
+                                            "missing_import_name": null,
+                                            "source_any": null,
+                                            "type_of_any": 2
+                                        }
+                                    ],
+                                    "bound_args": [],
+                                    "def_extras": {
+                                        "first_arg": "cls"
+                                    },
+                                    "fallback": "builtins.function",
+                                    "from_concatenate": false,
+                                    "implicit": false,
+                                    "is_ellipsis_args": false,
+                                    "name": "update_or_insert of TypedTable",
+                                    "ret_type": {
+                                        ".class": "UnionType",
+                                        "items": [
+                                            "builtins.int",
+                                            {
+                                                ".class": "NoneType"
+                                            }
+                                        ]
+                                    },
+                                    "type_guard": null,
+                                    "unpack_kwargs": false,
+                                    "variables": []
+                                }
+                            }
+                        }
                     }
                 },
                 "self_type": null,
                 "slots": null,
                 "tuple_type": null,
                 "type_vars": [],
                 "typeddict_type": null
@@ -2549,15 +2751,15 @@
                         ".class": "SymbolTableNode",
                         "kind": "Mdef",
                         "node": {
                             ".class": "TypeAlias",
                             "alias_tvars": [],
                             "column": 4,
                             "fullname": "src.typedal.core._Types.NONETYPE",
-                            "line": 35,
+                            "line": 37,
                             "no_args": false,
                             "normalized": false,
                             "target": {
                                 ".class": "NoneType"
                             }
                         }
                     }
```

### Comparing `typedal-1.2.0/.mypy_cache/3.11/src/typedal/core.meta.json` & `typedal-1.2.1/.mypy_cache/3.11/typedal/fields.meta.json`

 * *Files 14% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7222623552344914%*

 * *Differences: {"'data_mtime'": '1687879747',*

 * * "'dep_lines'": '{insert: [(0, 12)], delete: [15, 5, 0]}',*

 * * "'dep_prios'": '{insert: [(0, 5), (4, 10)], delete: [16, 6, 4, 3]}',*

 * * "'dependencies'": "{insert: [(0, 'typedal.core'), (2, 'decimal')], delete: [6, 4, 3]}",*

 * * "'hash'": "'2da5da10836f40ec000f32c64446f28df3e5081a9e14d5473684770659627369'",*

 * * "'id'": "'typedal.fields'",*

 * * "'interface_hash'": "'7f52734fa267868275c2d07b23b14504cf86d84ca8ba75738eacb85b5ff41a00'",*

 * * "'mtime'": '1687423422',*

 * * "'path'": "'src/typedal/fields.py'" […]*

```diff
@@ -1,69 +1,64 @@
 {
-    "data_mtime": 1687879973,
+    "data_mtime": 1687879747,
     "dep_lines": [
-        4,
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
-        5,
-        5,
         5,
         30,
         30,
         30,
         30,
         30,
         30,
         30,
         30,
-        30,
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
-        "collections",
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
-    "hash": "80d36592c6bce2b6337f637211ae19616779140573ccea38a08c76de0d2abb85",
-    "id": "src.typedal.core",
+    "hash": "2da5da10836f40ec000f32c64446f28df3e5081a9e14d5473684770659627369",
+    "id": "typedal.fields",
     "ignore_all": false,
-    "interface_hash": "e2a9f02ce4509e95ca99954260ca834c13d813025e3b8e70d2a736f0fda9376b",
-    "mtime": 1687879971,
+    "interface_hash": "7f52734fa267868275c2d07b23b14504cf86d84ca8ba75738eacb85b5ff41a00",
+    "mtime": 1687423422,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
@@ -97,16 +92,15 @@
         "strict_equality": true,
         "strict_optional": true,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "/home/robin/werk/Eigen/typedal/src/typedal/core.py",
+    "path": "src/typedal/fields.py",
     "plugin_data": null,
-    "size": 14524,
+    "size": 4949,
     "suppressed": [
-        "pydal.objects",
-        "pydal"
+        "pydal.objects"
     ],
     "version_id": "1.3.0"
 }
```

### Comparing `typedal-1.2.0/.mypy_cache/3.11/src/typedal/fields.data.json` & `typedal-1.2.1/.mypy_cache/3.11/src/typedal/fields.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.11/src/typedal/fields.meta.json` & `typedal-1.2.1/.mypy_cache/3.11/src/typedal/fields.meta.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9666666666666667%*

 * *Differences: {"'data_mtime'": '1687881806'}*

```diff
@@ -1,9 +1,9 @@
 {
-    "data_mtime": 1687879062,
+    "data_mtime": 1687881806,
     "dep_lines": [
         12,
         5,
         6,
         7,
         8,
         1,
```

### Comparing `typedal-1.2.0/.mypy_cache/3.11/typedal/__about__.data.json` & `typedal-1.2.1/.mypy_cache/3.11/typedal/__about__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.11/typedal/__about__.meta.json` & `typedal-1.2.1/.mypy_cache/3.11/typedal/__about__.meta.json`

 * *Files 16% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9333333333333333%*

 * *Differences: {"'hash'": "'715b564c762b0d7a05435d3d89098ff8e0731a48bf0ce68da91aeda6c4af1a60'",*

 * * "'mtime'": '1687881086'}*

```diff
@@ -11,19 +11,19 @@
         30
     ],
     "dependencies": [
         "builtins",
         "abc",
         "typing"
     ],
-    "hash": "d3fdb2a8e64ecc817b37ceda3cb568df16b663293ebedfad785f3e9a886973cd",
+    "hash": "715b564c762b0d7a05435d3d89098ff8e0731a48bf0ce68da91aeda6c4af1a60",
     "id": "typedal.__about__",
     "ignore_all": false,
     "interface_hash": "78ab11aa8e8cfd1f5fac091f83a1f2c46aac46f2e8973053a728baf5854e8af9",
-    "mtime": 1687876422,
+    "mtime": 1687881086,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
```

### Comparing `typedal-1.2.0/.mypy_cache/3.11/typedal/__init__.data.json` & `typedal-1.2.1/.mypy_cache/3.11/typedal/__init__.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.11/typedal/__init__.meta.json` & `typedal-1.2.1/.mypy_cache/3.11/typedal/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.11/typedal/core.data.json` & `typedal-1.2.1/.mypy_cache/3.11/typedal/core.data.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9941879690223284%*

 * *Differences: {"'names'": "{'T_annotation': {'node': {'line': 15}}, 'TypeDAL': {'node': {'names': {'__call__': "*

 * *            "{'node': {'type': {'arg_types': {1: {'.class': 'TypeAliasType', 'args': [], "*

 * *            "'type_ref': 'typedal.core.T_Query', delete: ['missing_import_name', 'source_any', "*

 * *            "'type_of_any']}}}}}}}}, 'TypedRow': {'node': {'line': 349}}, 'TypedTable': {'node': "*

 * *            "{'names': {'update_or_insert': OrderedDict([('.class', 'SymbolTableNode'), ('kind', "*

 * *            "'Mdef'), ('nod […]*

```diff
@@ -124,14 +124,36 @@
         "ChainMap": {
             ".class": "SymbolTableNode",
             "cross_ref": "collections.ChainMap",
             "kind": "Gdef",
             "module_hidden": true,
             "module_public": false
         },
+        "DEFAULT": {
+            ".class": "SymbolTableNode",
+            "kind": "Gdef",
+            "module_hidden": true,
+            "module_public": false,
+            "node": {
+                ".class": "Var",
+                "flags": [
+                    "is_suppressed_import",
+                    "is_ready",
+                    "is_inferred"
+                ],
+                "fullname": "typedal.core.DEFAULT",
+                "name": "DEFAULT",
+                "type": {
+                    ".class": "AnyType",
+                    "missing_import_name": "typedal.core.DEFAULT",
+                    "source_any": null,
+                    "type_of_any": 3
+                }
+            }
+        },
         "Decimal": {
             ".class": "SymbolTableNode",
             "cross_ref": "_decimal.Decimal",
             "kind": "Gdef",
             "module_hidden": true,
             "module_public": false
         },
@@ -153,14 +175,36 @@
                     ".class": "AnyType",
                     "missing_import_name": "typedal.core.Field",
                     "source_any": null,
                     "type_of_any": 3
                 }
             }
         },
+        "Query": {
+            ".class": "SymbolTableNode",
+            "kind": "Gdef",
+            "module_hidden": true,
+            "module_public": false,
+            "node": {
+                ".class": "Var",
+                "flags": [
+                    "is_suppressed_import",
+                    "is_ready",
+                    "is_inferred"
+                ],
+                "fullname": "typedal.core.Query",
+                "name": "Query",
+                "type": {
+                    ".class": "AnyType",
+                    "missing_import_name": "typedal.core.Query",
+                    "source_any": null,
+                    "type_of_any": 3
+                }
+            }
+        },
         "Row": {
             ".class": "SymbolTableNode",
             "kind": "Gdef",
             "module_hidden": true,
             "module_public": false,
             "node": {
                 ".class": "Var",
@@ -235,14 +279,53 @@
                             "type_of_any": 3
                         }
                     }
                 ],
                 "variance": 0
             }
         },
+        "T_Query": {
+            ".class": "SymbolTableNode",
+            "kind": "Gdef",
+            "node": {
+                ".class": "TypeAlias",
+                "alias_tvars": [],
+                "column": 0,
+                "fullname": "typedal.core.T_Query",
+                "line": 16,
+                "no_args": false,
+                "normalized": false,
+                "target": {
+                    ".class": "UnionType",
+                    "items": [
+                        {
+                            ".class": "AnyType",
+                            "missing_import_name": "typedal.core.Table",
+                            "source_any": null,
+                            "type_of_any": 3
+                        },
+                        {
+                            ".class": "AnyType",
+                            "missing_import_name": "typedal.core.Query",
+                            "source_any": null,
+                            "type_of_any": 3
+                        },
+                        "builtins.bool",
+                        {
+                            ".class": "NoneType"
+                        },
+                        "typedal.core.TypedTable",
+                        {
+                            ".class": "TypeType",
+                            "item": "typedal.core.TypedTable"
+                        }
+                    ]
+                }
+            }
+        },
         "T_Table": {
             ".class": "SymbolTableNode",
             "kind": "Gdef",
             "node": {
                 ".class": "TypeVarExpr",
                 "fullname": "typedal.core.T_Table",
                 "name": "T_Table",
@@ -260,15 +343,15 @@
             ".class": "SymbolTableNode",
             "kind": "Gdef",
             "node": {
                 ".class": "TypeAlias",
                 "alias_tvars": [],
                 "column": 0,
                 "fullname": "typedal.core.T_annotation",
-                "line": 14,
+                "line": 15,
                 "no_args": false,
                 "normalized": false,
                 "target": {
                     ".class": "UnionType",
                     "items": [
                         {
                             ".class": "TypeType",
@@ -371,18 +454,17 @@
                                     "self",
                                     "_args",
                                     "kwargs"
                                 ],
                                 "arg_types": [
                                     "typedal.core.TypeDAL",
                                     {
-                                        ".class": "AnyType",
-                                        "missing_import_name": null,
-                                        "source_any": null,
-                                        "type_of_any": 2
+                                        ".class": "TypeAliasType",
+                                        "args": [],
+                                        "type_ref": "typedal.core.T_Query"
                                     },
                                     {
                                         ".class": "AnyType",
                                         "missing_import_name": null,
                                         "source_any": null,
                                         "type_of_any": 2
                                     }
@@ -1548,15 +1630,15 @@
             ".class": "SymbolTableNode",
             "kind": "Gdef",
             "node": {
                 ".class": "TypeAlias",
                 "alias_tvars": [],
                 "column": 0,
                 "fullname": "typedal.core.TypedRow",
-                "line": 335,
+                "line": 349,
                 "no_args": true,
                 "normalized": false,
                 "target": "typedal.core.TypedTable"
             }
         },
         "TypedRows": {
             ".class": "SymbolTableNode",
@@ -2384,14 +2466,156 @@
                                     "ret_type": "builtins.int",
                                     "type_guard": null,
                                     "unpack_kwargs": false,
                                     "variables": []
                                 }
                             }
                         }
+                    },
+                    "update_or_insert": {
+                        ".class": "SymbolTableNode",
+                        "kind": "Mdef",
+                        "node": {
+                            ".class": "Decorator",
+                            "func": {
+                                ".class": "FuncDef",
+                                "abstract_status": 0,
+                                "arg_kinds": [
+                                    0,
+                                    1,
+                                    4
+                                ],
+                                "arg_names": [
+                                    "cls",
+                                    "query",
+                                    "values"
+                                ],
+                                "dataclass_transform_spec": null,
+                                "flags": [
+                                    "is_class",
+                                    "is_decorated"
+                                ],
+                                "fullname": "typedal.core.TypedTable.update_or_insert",
+                                "name": "update_or_insert",
+                                "type": {
+                                    ".class": "CallableType",
+                                    "arg_kinds": [
+                                        0,
+                                        1,
+                                        4
+                                    ],
+                                    "arg_names": [
+                                        "cls",
+                                        "query",
+                                        "values"
+                                    ],
+                                    "arg_types": [
+                                        {
+                                            ".class": "TypeType",
+                                            "item": "typedal.core.TypedTable"
+                                        },
+                                        {
+                                            ".class": "TypeAliasType",
+                                            "args": [],
+                                            "type_ref": "typedal.core.T_Query"
+                                        },
+                                        {
+                                            ".class": "AnyType",
+                                            "missing_import_name": null,
+                                            "source_any": null,
+                                            "type_of_any": 2
+                                        }
+                                    ],
+                                    "bound_args": [],
+                                    "def_extras": {
+                                        "first_arg": "cls"
+                                    },
+                                    "fallback": "builtins.function",
+                                    "from_concatenate": false,
+                                    "implicit": false,
+                                    "is_ellipsis_args": false,
+                                    "name": "update_or_insert of TypedTable",
+                                    "ret_type": {
+                                        ".class": "UnionType",
+                                        "items": [
+                                            "builtins.int",
+                                            {
+                                                ".class": "NoneType"
+                                            }
+                                        ]
+                                    },
+                                    "type_guard": null,
+                                    "unpack_kwargs": false,
+                                    "variables": []
+                                }
+                            },
+                            "is_overload": false,
+                            "var": {
+                                ".class": "Var",
+                                "flags": [
+                                    "is_initialized_in_class",
+                                    "is_classmethod",
+                                    "is_ready",
+                                    "is_inferred"
+                                ],
+                                "fullname": "typedal.core.TypedTable.update_or_insert",
+                                "name": "update_or_insert",
+                                "type": {
+                                    ".class": "CallableType",
+                                    "arg_kinds": [
+                                        0,
+                                        1,
+                                        4
+                                    ],
+                                    "arg_names": [
+                                        "cls",
+                                        "query",
+                                        "values"
+                                    ],
+                                    "arg_types": [
+                                        {
+                                            ".class": "TypeType",
+                                            "item": "typedal.core.TypedTable"
+                                        },
+                                        {
+                                            ".class": "TypeAliasType",
+                                            "args": [],
+                                            "type_ref": "typedal.core.T_Query"
+                                        },
+                                        {
+                                            ".class": "AnyType",
+                                            "missing_import_name": null,
+                                            "source_any": null,
+                                            "type_of_any": 2
+                                        }
+                                    ],
+                                    "bound_args": [],
+                                    "def_extras": {
+                                        "first_arg": "cls"
+                                    },
+                                    "fallback": "builtins.function",
+                                    "from_concatenate": false,
+                                    "implicit": false,
+                                    "is_ellipsis_args": false,
+                                    "name": "update_or_insert of TypedTable",
+                                    "ret_type": {
+                                        ".class": "UnionType",
+                                        "items": [
+                                            "builtins.int",
+                                            {
+                                                ".class": "NoneType"
+                                            }
+                                        ]
+                                    },
+                                    "type_guard": null,
+                                    "unpack_kwargs": false,
+                                    "variables": []
+                                }
+                            }
+                        }
                     }
                 },
                 "self_type": null,
                 "slots": null,
                 "tuple_type": null,
                 "type_vars": [],
                 "typeddict_type": null
@@ -2527,15 +2751,15 @@
                         ".class": "SymbolTableNode",
                         "kind": "Mdef",
                         "node": {
                             ".class": "TypeAlias",
                             "alias_tvars": [],
                             "column": 4,
                             "fullname": "typedal.core._Types.NONETYPE",
-                            "line": 35,
+                            "line": 37,
                             "no_args": false,
                             "normalized": false,
                             "target": {
                                 ".class": "NoneType"
                             }
                         }
                     }
```

### Comparing `typedal-1.2.0/.mypy_cache/3.11/typedal/core.meta.json` & `typedal-1.2.1/.mypy_cache/3.11/src/typedal/core.meta.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7518518518518519%*

 * *Differences: {"'data_mtime'": '1687882435',*

 * * "'dep_lines'": '{insert: [(16, 12)]}',*

 * * "'dep_prios'": '{insert: [(15, 5)]}',*

 * * "'hash'": "'386278e719ac9d6a24361f3043e0f739b3c59ca54f70136bb5e0f8bb3f839112'",*

 * * "'id'": "'src.typedal.core'",*

 * * "'interface_hash'": "'210f10c57be8628ed30ea78ff26b5d006227bca740293ee8005ffd1e37920d90'",*

 * * "'mtime'": '1687882362',*

 * * "'path'": "'/home/robin/werk/Eigen/typedal/src/typedal/core.py'",*

 * * "'size'": '15482',*

 * * "'suppressed'": "{insert: [(0, 'pydal._globals')]}"}*

```diff
@@ -1,9 +1,9 @@
 {
-    "data_mtime": 1687880020,
+    "data_mtime": 1687882435,
     "dep_lines": [
         4,
         5,
         6,
         7,
         8,
         1,
@@ -13,14 +13,15 @@
         1,
         1,
         1,
         1,
         1,
         1,
         11,
+        12,
         10
     ],
     "dep_prios": [
         10,
         10,
         10,
         5,
@@ -32,14 +33,15 @@
         30,
         30,
         30,
         30,
         30,
         30,
         5,
+        5,
         10
     ],
     "dependencies": [
         "datetime",
         "types",
         "typing",
         "collections",
@@ -51,19 +53,19 @@
         "abc",
         "array",
         "ctypes",
         "mmap",
         "pickle",
         "typing_extensions"
     ],
-    "hash": "cd26cc7f7d4990b2e02772442f5369932bdf298ab3f9035e0e7a8b53a5dab825",
-    "id": "typedal.core",
+    "hash": "386278e719ac9d6a24361f3043e0f739b3c59ca54f70136bb5e0f8bb3f839112",
+    "id": "src.typedal.core",
     "ignore_all": false,
-    "interface_hash": "74b2d4b5ecb63e92749321270f72a1fd1e64c49454226b0ce10c326c6f7dde6a",
-    "mtime": 1687881023,
+    "interface_hash": "210f10c57be8628ed30ea78ff26b5d006227bca740293ee8005ffd1e37920d90",
+    "mtime": 1687882362,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
@@ -97,16 +99,17 @@
         "strict_equality": true,
         "strict_optional": true,
         "warn_no_return": true,
         "warn_return_any": true,
         "warn_unreachable": false,
         "warn_unused_ignores": true
     },
-    "path": "src/typedal/core.py",
+    "path": "/home/robin/werk/Eigen/typedal/src/typedal/core.py",
     "plugin_data": null,
-    "size": 14972,
+    "size": 15482,
     "suppressed": [
+        "pydal._globals",
         "pydal.objects",
         "pydal"
     ],
     "version_id": "1.3.0"
 }
```

### Comparing `typedal-1.2.0/.mypy_cache/3.11/typedal/fields.data.json` & `typedal-1.2.1/.mypy_cache/3.11/typedal/fields.data.json`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.mypy_cache/3.11/typedal/fields.meta.json` & `typedal-1.2.1/.mypy_cache/3.11/typedal/core.meta.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7142019263845889%*

 * *Differences: {"'data_mtime'": '1687882472',*

 * * "'dep_lines'": '{insert: [(0, 4), (5, 1), (15, 11), (16, 12)], delete: [0]}',*

 * * "'dep_prios'": '{insert: [(3, 5), (4, 5), (6, 30), (15, 5), (17, 10)], delete: [1, 0]}',*

 * * "'dependencies'": "{insert: [(3, 'collections'), (4, 'decimal'), (6, '_collections_abc')], "*

 * *                   'delete: [2, 0]}',*

 * * "'hash'": "'14e567a449e281cd42f7beb83cf9625a9f4fa46929fd5aee437f19cc7fb7505c'",*

 * * "'id'": "'typedal.core'",*

 * * "'interface_hash'": "'2a8637fd7039de29c861d95cfdb6fdf32577902c31ebc2db1 […]*

```diff
@@ -1,64 +1,71 @@
 {
-    "data_mtime": 1687879747,
+    "data_mtime": 1687882472,
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
+        12,
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
-    "hash": "2da5da10836f40ec000f32c64446f28df3e5081a9e14d5473684770659627369",
-    "id": "typedal.fields",
+    "hash": "14e567a449e281cd42f7beb83cf9625a9f4fa46929fd5aee437f19cc7fb7505c",
+    "id": "typedal.core",
     "ignore_all": false,
-    "interface_hash": "7f52734fa267868275c2d07b23b14504cf86d84ca8ba75738eacb85b5ff41a00",
-    "mtime": 1687423422,
+    "interface_hash": "2a8637fd7039de29c861d95cfdb6fdf32577902c31ebc2db1a4c65341d866760",
+    "mtime": 1687882471,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": true,
@@ -92,15 +99,17 @@
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
-    "size": 4949,
+    "size": 15559,
     "suppressed": [
-        "pydal.objects"
+        "pydal._globals",
+        "pydal.objects",
+        "pydal"
     ],
     "version_id": "1.3.0"
 }
```

### Comparing `typedal-1.2.0/.pytest_cache/v/cache/nodeids` & `typedal-1.2.1/.pytest_cache/v/cache/nodeids`

 * *Files 11% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9565217391304348%*

 * *Differences: {'insert': "[(20, 'tests/test_mypy.py::[mypy]mypy_test_query')]"}*

```diff
@@ -15,10 +15,11 @@
     "tests/test_main.py::test_everything",
     "tests/test_main.py::test_fields",
     "tests/test_main.py::test_invalid_union",
     "tests/test_main.py::test_mixed_defines",
     "tests/test_main.py::test_typedfield_reprs",
     "tests/test_main.py::test_typedfield_to_field_type",
     "tests/test_main.py::test_using_model_without_define",
+    "tests/test_mypy.py::[mypy]mypy_test_query",
     "tests/test_mypy.py::[mypy]mypy_test_typedset",
     "tests/test_mypy.py::test_typedset"
 ]
```

### Comparing `typedal-1.2.0/.ruff_cache/content/1b34455c399f0006` & `typedal-1.2.1/.ruff_cache/content/1b34455c399f0006`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.ruff_cache/content/20585cf790eae81e` & `typedal-1.2.1/.ruff_cache/content/20585cf790eae81e`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.ruff_cache/content/221af82ae72a7f27` & `typedal-1.2.1/.ruff_cache/content/221af82ae72a7f27`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.ruff_cache/content/24e1b4aab386ebc8` & `typedal-1.2.1/.ruff_cache/content/24e1b4aab386ebc8`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.ruff_cache/content/2f3396c610fd7095` & `typedal-1.2.1/.ruff_cache/content/2f3396c610fd7095`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.ruff_cache/content/322af04e6d059ce5` & `typedal-1.2.1/.ruff_cache/content/322af04e6d059ce5`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.ruff_cache/content/3826106cf4494de8` & `typedal-1.2.1/.ruff_cache/content/3826106cf4494de8`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.ruff_cache/content/38d5fd55b14a9d6c` & `typedal-1.2.1/.ruff_cache/content/38d5fd55b14a9d6c`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.ruff_cache/content/4022ee8774ccd98a` & `typedal-1.2.1/.ruff_cache/content/4022ee8774ccd98a`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.ruff_cache/content/5491563776466765346` & `typedal-1.2.1/.ruff_cache/content/5491563776466765346`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.ruff_cache/content/75bd1769f6e29ed7` & `typedal-1.2.1/.ruff_cache/content/75bd1769f6e29ed7`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.ruff_cache/content/a0739889bf9412e8` & `typedal-1.2.1/.ruff_cache/content/a0739889bf9412e8`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.ruff_cache/content/a225e4df39be9b29` & `typedal-1.2.1/.ruff_cache/content/a225e4df39be9b29`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.ruff_cache/content/b419496fa9e72887` & `typedal-1.2.1/.ruff_cache/content/b419496fa9e72887`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.ruff_cache/content/bdcdf5c7bbc1d738` & `typedal-1.2.1/.ruff_cache/content/bdcdf5c7bbc1d738`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.ruff_cache/content/c06de16f3c7a64cc` & `typedal-1.2.1/.ruff_cache/content/c06de16f3c7a64cc`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.ruff_cache/content/cdfecbca581311ee` & `typedal-1.2.1/.ruff_cache/content/cdfecbca581311ee`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.ruff_cache/content/da4811a7730a562a` & `typedal-1.2.1/.ruff_cache/content/da4811a7730a562a`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/.ruff_cache/content/eee2f3c667de6c7a` & `typedal-1.2.1/.ruff_cache/content/eee2f3c667de6c7a`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/htmlcov/coverage_html.js` & `typedal-1.2.1/htmlcov/coverage_html.js`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/htmlcov/d_0ccc93afd6526b6c___about___py.html` & `typedal-1.2.1/htmlcov/d_0ccc93afd6526b6c___about___py.html`

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
-            created at 2023-06-27 17:35 +0200
+            created at 2023-06-27 18:07 +0200
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
-    <p class="run"><span class="n"><a id="t8" href="#t8">8</a></span><span class="t"><span class="nam">__version__</span> <span class="op">=</span> <span class="str">"1.1.2"</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t8" href="#t8">8</a></span><span class="t"><span class="nam">__version__</span> <span class="op">=</span> <span class="str">"1.2.0"</span>&nbsp;</span><span class="r"></span></p>
 </main>
 <footer>
     <div class="content">
         <p>
             <a id="prevFileLink" class="nav" href="index.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_0ccc93afd6526b6c___init___py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-06-27 17:35 +0200
+            created at 2023-06-27 18:07 +0200
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
-at 2023-06-27 17:35 +0200
+at 2023-06-27 18:07 +0200
 
 
 1""" 
 2This file contains the Version info for this package. 
 3""" 
 4 
 5# SPDX-FileCopyrightText: 2023-present Robin van der Noord
 <robinvandernoord@gmail.com> 
 6# 
 7# SPDX-License-Identifier: MIT 
-8__version__ = "1.1.2" 
+8__version__ = "1.2.0" 
 
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.7, created
-at 2023-06-27 17:35 +0200
+at 2023-06-27 18:07 +0200
```

### Comparing `typedal-1.2.0/htmlcov/d_0ccc93afd6526b6c___init___py.html` & `typedal-1.2.1/htmlcov/d_0ccc93afd6526b6c___init___py.html`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/htmlcov/d_0ccc93afd6526b6c_core_py.html` & `typedal-1.2.1/htmlcov/d_0ccc93afd6526b6c_core_py.html`

 * *Files 0% similar despite different names*

```diff
@@ -50,26 +50,26 @@
                     <p>
                         <kbd>?</kbd> &nbsp; show/hide this help
                     </p>
                 </div>
             </div>
         </aside>
         <h2>
-            <span class="text">144 statements &nbsp;</span>
-            <button type="button" class="run button_toggle_run" value="run" data-shortcut="r" title="Toggle lines run">144<span class="text"> run</span></button>
+            <span class="text">153 statements &nbsp;</span>
+            <button type="button" class="run button_toggle_run" value="run" data-shortcut="r" title="Toggle lines run">153<span class="text"> run</span></button>
             <button type="button" class="mis show_mis button_toggle_mis" value="mis" data-shortcut="m" title="Toggle lines missing">0<span class="text"> missing</span></button>
             <button type="button" class="exc show_exc button_toggle_exc" value="exc" data-shortcut="x" title="Toggle lines excluded">12<span class="text"> excluded</span></button>
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="d_0ccc93afd6526b6c___init___py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_0ccc93afd6526b6c_fields_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-06-27 17:50 +0200
+            created at 2023-06-27 18:15 +0200
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -86,465 +86,479 @@
     <p class="run"><span class="n"><a id="t4" href="#t4">4</a></span><span class="t"><span class="key">import</span> <span class="nam">datetime</span> <span class="key">as</span> <span class="nam">dt</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t5" href="#t5">5</a></span><span class="t"><span class="key">import</span> <span class="nam">types</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t6" href="#t6">6</a></span><span class="t"><span class="key">import</span> <span class="nam">typing</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t7" href="#t7">7</a></span><span class="t"><span class="key">from</span> <span class="nam">collections</span> <span class="key">import</span> <span class="nam">ChainMap</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t8" href="#t8">8</a></span><span class="t"><span class="key">from</span> <span class="nam">decimal</span> <span class="key">import</span> <span class="nam">Decimal</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t9" href="#t9">9</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t10" href="#t10">10</a></span><span class="t"><span class="key">import</span> <span class="nam">pydal</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t11" href="#t11">11</a></span><span class="t"><span class="key">from</span> <span class="nam">pydal</span><span class="op">.</span><span class="nam">objects</span> <span class="key">import</span> <span class="nam">Field</span><span class="op">,</span> <span class="nam">Row</span><span class="op">,</span> <span class="nam">Rows</span><span class="op">,</span> <span class="nam">Table</span>&nbsp;</span><span class="r"></span></p>
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
-    <p class="pln"><span class="n"><a id="t29" href="#t29">29</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t30" href="#t30">30</a></span><span class="t"><span class="key">class</span> <span class="nam">_Types</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t31" href="#t31">31</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t32" href="#t32">32</a></span><span class="t"><span class="str">    Internal type storage for stuff that mypy otherwise won't understand.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t33" href="#t33">33</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t34" href="#t34">34</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t35" href="#t35">35</a></span><span class="t">    <span class="nam">NONETYPE</span> <span class="op">=</span> <span class="nam">type</span><span class="op">(</span><span class="key">None</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t11" href="#t11">11</a></span><span class="t"><span class="key">from</span> <span class="nam">pydal</span><span class="op">.</span><span class="nam">_globals</span> <span class="key">import</span> <span class="nam">DEFAULT</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t12" href="#t12">12</a></span><span class="t"><span class="key">from</span> <span class="nam">pydal</span><span class="op">.</span><span class="nam">objects</span> <span class="key">import</span> <span class="nam">Field</span><span class="op">,</span> <span class="nam">Query</span><span class="op">,</span> <span class="nam">Row</span><span class="op">,</span> <span class="nam">Rows</span><span class="op">,</span> <span class="nam">Table</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t13" href="#t13">13</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t14" href="#t14">14</a></span><span class="t"><span class="com"># use typing.cast(type, ...) to make mypy happy with unions</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t15" href="#t15">15</a></span><span class="t"><span class="nam">T_annotation</span> <span class="op">=</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Type</span><span class="op">[</span><span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">]</span> <span class="op">|</span> <span class="nam">types</span><span class="op">.</span><span class="nam">UnionType</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t16" href="#t16">16</a></span><span class="t"><span class="nam">T_Query</span> <span class="op">=</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Union</span><span class="op">[</span><span class="str">"Table"</span><span class="op">,</span> <span class="str">"Query"</span><span class="op">,</span> <span class="str">"bool"</span><span class="op">,</span> <span class="str">"None"</span><span class="op">,</span> <span class="str">"TypedTable"</span><span class="op">,</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Type</span><span class="op">[</span><span class="str">"TypedTable"</span><span class="op">]</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t17" href="#t17">17</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t18" href="#t18">18</a></span><span class="t"><span class="nam">BASIC_MAPPINGS</span><span class="op">:</span> <span class="nam">dict</span><span class="op">[</span><span class="nam">T_annotation</span><span class="op">,</span> <span class="nam">str</span><span class="op">]</span> <span class="op">=</span> <span class="op">{</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t19" href="#t19">19</a></span><span class="t">    <span class="nam">str</span><span class="op">:</span> <span class="str">"string"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t20" href="#t20">20</a></span><span class="t">    <span class="nam">int</span><span class="op">:</span> <span class="str">"integer"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t21" href="#t21">21</a></span><span class="t">    <span class="nam">bool</span><span class="op">:</span> <span class="str">"boolean"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t22" href="#t22">22</a></span><span class="t">    <span class="nam">bytes</span><span class="op">:</span> <span class="str">"blob"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t23" href="#t23">23</a></span><span class="t">    <span class="nam">float</span><span class="op">:</span> <span class="str">"double"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t24" href="#t24">24</a></span><span class="t">    <span class="nam">object</span><span class="op">:</span> <span class="str">"json"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t25" href="#t25">25</a></span><span class="t">    <span class="nam">Decimal</span><span class="op">:</span> <span class="str">"decimal(10,2)"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t26" href="#t26">26</a></span><span class="t">    <span class="nam">dt</span><span class="op">.</span><span class="nam">date</span><span class="op">:</span> <span class="str">"date"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t27" href="#t27">27</a></span><span class="t">    <span class="nam">dt</span><span class="op">.</span><span class="nam">time</span><span class="op">:</span> <span class="str">"time"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t28" href="#t28">28</a></span><span class="t">    <span class="nam">dt</span><span class="op">.</span><span class="nam">datetime</span><span class="op">:</span> <span class="str">"datetime"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t29" href="#t29">29</a></span><span class="t"><span class="op">}</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t30" href="#t30">30</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t31" href="#t31">31</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t32" href="#t32">32</a></span><span class="t"><span class="key">class</span> <span class="nam">_Types</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t33" href="#t33">33</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t34" href="#t34">34</a></span><span class="t"><span class="str">    Internal type storage for stuff that mypy otherwise won't understand.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t35" href="#t35">35</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t36" href="#t36">36</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t37" href="#t37">37</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t38" href="#t38">38</a></span><span class="t"><span class="com"># the input and output of TypeDAL.define</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t39" href="#t39">39</a></span><span class="t"><span class="nam">T</span> <span class="op">=</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">TypeVar</span><span class="op">(</span><span class="str">"T"</span><span class="op">,</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Type</span><span class="op">[</span><span class="str">"TypedTable"</span><span class="op">]</span><span class="op">,</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Type</span><span class="op">[</span><span class="str">"Table"</span><span class="op">]</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t40" href="#t40">40</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t41" href="#t41">41</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
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
-    <p class="pln"><span class="n"><a id="t52" href="#t52">52</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t53" href="#t53">53</a></span><span class="t"><span class="key">def</span> <span class="nam">_all_annotations</span><span class="op">(</span><span class="nam">cls</span><span class="op">:</span> <span class="nam">type</span><span class="op">)</span> <span class="op">-></span> <span class="nam">ChainMap</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">type</span><span class="op">]</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t54" href="#t54">54</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t55" href="#t55">55</a></span><span class="t"><span class="str">    Returns a dictionary-like ChainMap that includes annotations for all \</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t56" href="#t56">56</a></span><span class="t"><span class="str">    attributes defined in cls or inherited from superclasses.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t57" href="#t57">57</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t58" href="#t58">58</a></span><span class="t">    <span class="key">return</span> <span class="nam">ChainMap</span><span class="op">(</span><span class="op">*</span><span class="op">(</span><span class="nam">c</span><span class="op">.</span><span class="nam">__annotations__</span> <span class="key">for</span> <span class="nam">c</span> <span class="key">in</span> <span class="nam">getattr</span><span class="op">(</span><span class="nam">cls</span><span class="op">,</span> <span class="str">"__mro__"</span><span class="op">,</span> <span class="op">[</span><span class="op">]</span><span class="op">)</span> <span class="key">if</span> <span class="str">"__annotations__"</span> <span class="key">in</span> <span class="nam">c</span><span class="op">.</span><span class="nam">__dict__</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t59" href="#t59">59</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t60" href="#t60">60</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t61" href="#t61">61</a></span><span class="t"><span class="key">def</span> <span class="nam">all_annotations</span><span class="op">(</span><span class="nam">cls</span><span class="op">:</span> <span class="nam">type</span><span class="op">,</span> <span class="nam">_except</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Iterable</span><span class="op">[</span><span class="nam">str</span><span class="op">]</span> <span class="op">=</span> <span class="key">None</span><span class="op">)</span> <span class="op">-></span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">type</span><span class="op">]</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t62" href="#t62">62</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t63" href="#t63">63</a></span><span class="t"><span class="str">    Wrapper around `_all_annotations` that filters away any keys in _except.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t64" href="#t64">64</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t65" href="#t65">65</a></span><span class="t"><span class="str">    It also flattens the ChainMap to a regular dict.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t66" href="#t66">66</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t67" href="#t67">67</a></span><span class="t">    <span class="key">if</span> <span class="nam">_except</span> <span class="key">is</span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t68" href="#t68">68</a></span><span class="t">        <span class="nam">_except</span> <span class="op">=</span> <span class="nam">set</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t69" href="#t69">69</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t70" href="#t70">70</a></span><span class="t">    <span class="nam">_all</span> <span class="op">=</span> <span class="nam">_all_annotations</span><span class="op">(</span><span class="nam">cls</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t71" href="#t71">71</a></span><span class="t">    <span class="key">return</span> <span class="op">{</span><span class="nam">k</span><span class="op">:</span> <span class="nam">v</span> <span class="key">for</span> <span class="nam">k</span><span class="op">,</span> <span class="nam">v</span> <span class="key">in</span> <span class="nam">_all</span><span class="op">.</span><span class="nam">items</span><span class="op">(</span><span class="op">)</span> <span class="key">if</span> <span class="nam">k</span> <span class="key">not</span> <span class="key">in</span> <span class="nam">_except</span><span class="op">}</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t72" href="#t72">72</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t73" href="#t73">73</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t74" href="#t74">74</a></span><span class="t"><span class="key">class</span> <span class="nam">TypeDAL</span><span class="op">(</span><span class="nam">pydal</span><span class="op">.</span><span class="nam">DAL</span><span class="op">)</span><span class="op">:</span>  <span class="com"># type: ignore</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t75" href="#t75">75</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t76" href="#t76">76</a></span><span class="t"><span class="str">    Drop-in replacement for pyDAL with layer to convert class-based table definitions to classical pydal define_tables.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t77" href="#t77">77</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t78" href="#t78">78</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t79" href="#t79">79</a></span><span class="t">    <span class="nam">dal</span><span class="op">:</span> <span class="nam">Table</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t37" href="#t37">37</a></span><span class="t">    <span class="nam">NONETYPE</span> <span class="op">=</span> <span class="nam">type</span><span class="op">(</span><span class="key">None</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t38" href="#t38">38</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t39" href="#t39">39</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t40" href="#t40">40</a></span><span class="t"><span class="com"># the input and output of TypeDAL.define</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t41" href="#t41">41</a></span><span class="t"><span class="nam">T</span> <span class="op">=</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">TypeVar</span><span class="op">(</span><span class="str">"T"</span><span class="op">,</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Type</span><span class="op">[</span><span class="str">"TypedTable"</span><span class="op">]</span><span class="op">,</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Type</span><span class="op">[</span><span class="str">"Table"</span><span class="op">]</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t42" href="#t42">42</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t43" href="#t43">43</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t44" href="#t44">44</a></span><span class="t"><span class="key">def</span> <span class="nam">is_union</span><span class="op">(</span><span class="nam">some_type</span><span class="op">:</span> <span class="nam">type</span><span class="op">)</span> <span class="op">-></span> <span class="nam">bool</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t45" href="#t45">45</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t46" href="#t46">46</a></span><span class="t"><span class="str">    Check if a type is some type of Union.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t47" href="#t47">47</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t48" href="#t48">48</a></span><span class="t"><span class="str">    Args:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t49" href="#t49">49</a></span><span class="t"><span class="str">        some_type: types.UnionType = type(int | str); typing.Union = typing.Union[int, str]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t50" href="#t50">50</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t51" href="#t51">51</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t52" href="#t52">52</a></span><span class="t">    <span class="key">return</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">get_origin</span><span class="op">(</span><span class="nam">some_type</span><span class="op">)</span> <span class="key">in</span> <span class="op">(</span><span class="nam">types</span><span class="op">.</span><span class="nam">UnionType</span><span class="op">,</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Union</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t53" href="#t53">53</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t54" href="#t54">54</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t55" href="#t55">55</a></span><span class="t"><span class="key">def</span> <span class="nam">_all_annotations</span><span class="op">(</span><span class="nam">cls</span><span class="op">:</span> <span class="nam">type</span><span class="op">)</span> <span class="op">-></span> <span class="nam">ChainMap</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">type</span><span class="op">]</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t56" href="#t56">56</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t57" href="#t57">57</a></span><span class="t"><span class="str">    Returns a dictionary-like ChainMap that includes annotations for all \</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t58" href="#t58">58</a></span><span class="t"><span class="str">    attributes defined in cls or inherited from superclasses.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t59" href="#t59">59</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t60" href="#t60">60</a></span><span class="t">    <span class="key">return</span> <span class="nam">ChainMap</span><span class="op">(</span><span class="op">*</span><span class="op">(</span><span class="nam">c</span><span class="op">.</span><span class="nam">__annotations__</span> <span class="key">for</span> <span class="nam">c</span> <span class="key">in</span> <span class="nam">getattr</span><span class="op">(</span><span class="nam">cls</span><span class="op">,</span> <span class="str">"__mro__"</span><span class="op">,</span> <span class="op">[</span><span class="op">]</span><span class="op">)</span> <span class="key">if</span> <span class="str">"__annotations__"</span> <span class="key">in</span> <span class="nam">c</span><span class="op">.</span><span class="nam">__dict__</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t61" href="#t61">61</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t62" href="#t62">62</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t63" href="#t63">63</a></span><span class="t"><span class="key">def</span> <span class="nam">all_annotations</span><span class="op">(</span><span class="nam">cls</span><span class="op">:</span> <span class="nam">type</span><span class="op">,</span> <span class="nam">_except</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Iterable</span><span class="op">[</span><span class="nam">str</span><span class="op">]</span> <span class="op">=</span> <span class="key">None</span><span class="op">)</span> <span class="op">-></span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">type</span><span class="op">]</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t64" href="#t64">64</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t65" href="#t65">65</a></span><span class="t"><span class="str">    Wrapper around `_all_annotations` that filters away any keys in _except.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t66" href="#t66">66</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t67" href="#t67">67</a></span><span class="t"><span class="str">    It also flattens the ChainMap to a regular dict.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t68" href="#t68">68</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t69" href="#t69">69</a></span><span class="t">    <span class="key">if</span> <span class="nam">_except</span> <span class="key">is</span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t70" href="#t70">70</a></span><span class="t">        <span class="nam">_except</span> <span class="op">=</span> <span class="nam">set</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t71" href="#t71">71</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t72" href="#t72">72</a></span><span class="t">    <span class="nam">_all</span> <span class="op">=</span> <span class="nam">_all_annotations</span><span class="op">(</span><span class="nam">cls</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t73" href="#t73">73</a></span><span class="t">    <span class="key">return</span> <span class="op">{</span><span class="nam">k</span><span class="op">:</span> <span class="nam">v</span> <span class="key">for</span> <span class="nam">k</span><span class="op">,</span> <span class="nam">v</span> <span class="key">in</span> <span class="nam">_all</span><span class="op">.</span><span class="nam">items</span><span class="op">(</span><span class="op">)</span> <span class="key">if</span> <span class="nam">k</span> <span class="key">not</span> <span class="key">in</span> <span class="nam">_except</span><span class="op">}</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t74" href="#t74">74</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t75" href="#t75">75</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t76" href="#t76">76</a></span><span class="t"><span class="key">class</span> <span class="nam">TypeDAL</span><span class="op">(</span><span class="nam">pydal</span><span class="op">.</span><span class="nam">DAL</span><span class="op">)</span><span class="op">:</span>  <span class="com"># type: ignore</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t77" href="#t77">77</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t78" href="#t78">78</a></span><span class="t"><span class="str">    Drop-in replacement for pyDAL with layer to convert class-based table definitions to classical pydal define_tables.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t79" href="#t79">79</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t80" href="#t80">80</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t81" href="#t81">81</a></span><span class="t">    <span class="nam">default_kwargs</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">ClassVar</span><span class="op">[</span><span class="nam">typing</span><span class="op">.</span><span class="nam">Dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">]</span><span class="op">]</span> <span class="op">=</span> <span class="op">{</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t82" href="#t82">82</a></span><span class="t">        <span class="com"># fields are 'required' (notnull) by default:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t83" href="#t83">83</a></span><span class="t">        <span class="str">"notnull"</span><span class="op">:</span> <span class="key">True</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t84" href="#t84">84</a></span><span class="t">    <span class="op">}</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t85" href="#t85">85</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t86" href="#t86">86</a></span><span class="t">    <span class="key">def</span> <span class="nam">define</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">cls</span><span class="op">:</span> <span class="nam">T</span><span class="op">)</span> <span class="op">-></span> <span class="nam">T</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t87" href="#t87">87</a></span><span class="t">        <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t88" href="#t88">88</a></span><span class="t"><span class="str">        Can be used as a decorator on a class that inherits `TypedTable`, \</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t89" href="#t89">89</a></span><span class="t"><span class="str">          or as a regular method if you need to define your classes before you have access to a 'db' instance.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t90" href="#t90">90</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t91" href="#t91">91</a></span><span class="t"><span class="str">        Args:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t92" href="#t92">92</a></span><span class="t"><span class="str">            cls:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t93" href="#t93">93</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t94" href="#t94">94</a></span><span class="t"><span class="str">        Example:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t95" href="#t95">95</a></span><span class="t"><span class="str">            @db.define</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t96" href="#t96">96</a></span><span class="t"><span class="str">            class Person(TypedTable):</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t97" href="#t97">97</a></span><span class="t"><span class="str">                ...</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t98" href="#t98">98</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t99" href="#t99">99</a></span><span class="t"><span class="str">            class Article(TypedTable):</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t100" href="#t100">100</a></span><span class="t"><span class="str">                ...</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t101" href="#t101">101</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t102" href="#t102">102</a></span><span class="t"><span class="str">            # at a later time:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t103" href="#t103">103</a></span><span class="t"><span class="str">            db.define(Article)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t104" href="#t104">104</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t105" href="#t105">105</a></span><span class="t"><span class="str">        Returns:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t106" href="#t106">106</a></span><span class="t"><span class="str">            the result of pydal.define_table</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t107" href="#t107">107</a></span><span class="t"><span class="str">        """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t108" href="#t108">108</a></span><span class="t">        <span class="com"># when __future__.annotations is implemented, cls.__annotations__ will not work anymore as below.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t109" href="#t109">109</a></span><span class="t">        <span class="com"># proper way to handle this would be (but gives error right now due to Table implementing magic methods):</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t110" href="#t110">110</a></span><span class="t">        <span class="com"># typing.get_type_hints(cls, globalns=None, localns=None)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t111" href="#t111">111</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t112" href="#t112">112</a></span><span class="t">        <span class="com"># dirty way (with evil eval):</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t113" href="#t113">113</a></span><span class="t">        <span class="com"># [eval(v) for k, v in cls.__annotations__.items()]</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t114" href="#t114">114</a></span><span class="t">        <span class="com"># this however also stops working when variables outside this scope or even references to other</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t115" href="#t115">115</a></span><span class="t">        <span class="com"># objects are used. So for now, this package will NOT work when from __future__ import annotations is used,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t116" href="#t116">116</a></span><span class="t">        <span class="com"># and might break in the future, when this annotations behavior is enabled by default.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t117" href="#t117">117</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t118" href="#t118">118</a></span><span class="t">        <span class="com"># non-annotated variables have to be passed to define_table as kwargs</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t81" href="#t81">81</a></span><span class="t">    <span class="nam">dal</span><span class="op">:</span> <span class="nam">Table</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t82" href="#t82">82</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t83" href="#t83">83</a></span><span class="t">    <span class="nam">default_kwargs</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">ClassVar</span><span class="op">[</span><span class="nam">typing</span><span class="op">.</span><span class="nam">Dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">]</span><span class="op">]</span> <span class="op">=</span> <span class="op">{</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t84" href="#t84">84</a></span><span class="t">        <span class="com"># fields are 'required' (notnull) by default:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t85" href="#t85">85</a></span><span class="t">        <span class="str">"notnull"</span><span class="op">:</span> <span class="key">True</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t86" href="#t86">86</a></span><span class="t">    <span class="op">}</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t87" href="#t87">87</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t88" href="#t88">88</a></span><span class="t">    <span class="key">def</span> <span class="nam">define</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">cls</span><span class="op">:</span> <span class="nam">T</span><span class="op">)</span> <span class="op">-></span> <span class="nam">T</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t89" href="#t89">89</a></span><span class="t">        <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t90" href="#t90">90</a></span><span class="t"><span class="str">        Can be used as a decorator on a class that inherits `TypedTable`, \</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t91" href="#t91">91</a></span><span class="t"><span class="str">          or as a regular method if you need to define your classes before you have access to a 'db' instance.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t92" href="#t92">92</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t93" href="#t93">93</a></span><span class="t"><span class="str">        Args:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t94" href="#t94">94</a></span><span class="t"><span class="str">            cls:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t95" href="#t95">95</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t96" href="#t96">96</a></span><span class="t"><span class="str">        Example:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t97" href="#t97">97</a></span><span class="t"><span class="str">            @db.define</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t98" href="#t98">98</a></span><span class="t"><span class="str">            class Person(TypedTable):</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t99" href="#t99">99</a></span><span class="t"><span class="str">                ...</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t100" href="#t100">100</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t101" href="#t101">101</a></span><span class="t"><span class="str">            class Article(TypedTable):</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t102" href="#t102">102</a></span><span class="t"><span class="str">                ...</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t103" href="#t103">103</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t104" href="#t104">104</a></span><span class="t"><span class="str">            # at a later time:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t105" href="#t105">105</a></span><span class="t"><span class="str">            db.define(Article)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t106" href="#t106">106</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t107" href="#t107">107</a></span><span class="t"><span class="str">        Returns:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t108" href="#t108">108</a></span><span class="t"><span class="str">            the result of pydal.define_table</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t109" href="#t109">109</a></span><span class="t"><span class="str">        """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t110" href="#t110">110</a></span><span class="t">        <span class="com"># when __future__.annotations is implemented, cls.__annotations__ will not work anymore as below.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t111" href="#t111">111</a></span><span class="t">        <span class="com"># proper way to handle this would be (but gives error right now due to Table implementing magic methods):</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t112" href="#t112">112</a></span><span class="t">        <span class="com"># typing.get_type_hints(cls, globalns=None, localns=None)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t113" href="#t113">113</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t114" href="#t114">114</a></span><span class="t">        <span class="com"># dirty way (with evil eval):</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t115" href="#t115">115</a></span><span class="t">        <span class="com"># [eval(v) for k, v in cls.__annotations__.items()]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t116" href="#t116">116</a></span><span class="t">        <span class="com"># this however also stops working when variables outside this scope or even references to other</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t117" href="#t117">117</a></span><span class="t">        <span class="com"># objects are used. So for now, this package will NOT work when from __future__ import annotations is used,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t118" href="#t118">118</a></span><span class="t">        <span class="com"># and might break in the future, when this annotations behavior is enabled by default.</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t119" href="#t119">119</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t120" href="#t120">120</a></span><span class="t">        <span class="nam">tablename</span> <span class="op">=</span> <span class="nam">self</span><span class="op">.</span><span class="nam">_to_snake</span><span class="op">(</span><span class="nam">cls</span><span class="op">.</span><span class="nam">__name__</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t121" href="#t121">121</a></span><span class="t">        <span class="com"># grab annotations of cls and it's parents:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t122" href="#t122">122</a></span><span class="t">        <span class="nam">annotations</span> <span class="op">=</span> <span class="nam">all_annotations</span><span class="op">(</span><span class="nam">cls</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t123" href="#t123">123</a></span><span class="t">        <span class="com"># extend with `prop = TypedField()` 'annotations':</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t124" href="#t124">124</a></span><span class="t">        <span class="nam">annotations</span> <span class="op">|=</span> <span class="op">{</span><span class="nam">k</span><span class="op">:</span> <span class="nam">v</span> <span class="key">for</span> <span class="nam">k</span><span class="op">,</span> <span class="nam">v</span> <span class="key">in</span> <span class="nam">cls</span><span class="op">.</span><span class="nam">__dict__</span><span class="op">.</span><span class="nam">items</span><span class="op">(</span><span class="op">)</span> <span class="key">if</span> <span class="nam">isinstance</span><span class="op">(</span><span class="nam">v</span><span class="op">,</span> <span class="nam">TypedFieldType</span><span class="op">)</span><span class="op">}</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t125" href="#t125">125</a></span><span class="t">        <span class="com"># remove internal stuff:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t126" href="#t126">126</a></span><span class="t">        <span class="nam">annotations</span> <span class="op">=</span> <span class="op">{</span><span class="nam">k</span><span class="op">:</span> <span class="nam">v</span> <span class="key">for</span> <span class="nam">k</span><span class="op">,</span> <span class="nam">v</span> <span class="key">in</span> <span class="nam">annotations</span><span class="op">.</span><span class="nam">items</span><span class="op">(</span><span class="op">)</span> <span class="key">if</span> <span class="key">not</span> <span class="nam">k</span><span class="op">.</span><span class="nam">startswith</span><span class="op">(</span><span class="str">"_"</span><span class="op">)</span><span class="op">}</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t127" href="#t127">127</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t128" href="#t128">128</a></span><span class="t">        <span class="nam">typedfields</span> <span class="op">=</span> <span class="op">{</span><span class="nam">k</span><span class="op">:</span> <span class="nam">v</span> <span class="key">for</span> <span class="nam">k</span><span class="op">,</span> <span class="nam">v</span> <span class="key">in</span> <span class="nam">annotations</span><span class="op">.</span><span class="nam">items</span><span class="op">(</span><span class="op">)</span> <span class="key">if</span> <span class="nam">isinstance</span><span class="op">(</span><span class="nam">v</span><span class="op">,</span> <span class="nam">TypedFieldType</span><span class="op">)</span><span class="op">}</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t120" href="#t120">120</a></span><span class="t">        <span class="com"># non-annotated variables have to be passed to define_table as kwargs</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t121" href="#t121">121</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t122" href="#t122">122</a></span><span class="t">        <span class="nam">tablename</span> <span class="op">=</span> <span class="nam">self</span><span class="op">.</span><span class="nam">_to_snake</span><span class="op">(</span><span class="nam">cls</span><span class="op">.</span><span class="nam">__name__</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t123" href="#t123">123</a></span><span class="t">        <span class="com"># grab annotations of cls and it's parents:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t124" href="#t124">124</a></span><span class="t">        <span class="nam">annotations</span> <span class="op">=</span> <span class="nam">all_annotations</span><span class="op">(</span><span class="nam">cls</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t125" href="#t125">125</a></span><span class="t">        <span class="com"># extend with `prop = TypedField()` 'annotations':</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t126" href="#t126">126</a></span><span class="t">        <span class="nam">annotations</span> <span class="op">|=</span> <span class="op">{</span><span class="nam">k</span><span class="op">:</span> <span class="nam">v</span> <span class="key">for</span> <span class="nam">k</span><span class="op">,</span> <span class="nam">v</span> <span class="key">in</span> <span class="nam">cls</span><span class="op">.</span><span class="nam">__dict__</span><span class="op">.</span><span class="nam">items</span><span class="op">(</span><span class="op">)</span> <span class="key">if</span> <span class="nam">isinstance</span><span class="op">(</span><span class="nam">v</span><span class="op">,</span> <span class="nam">TypedFieldType</span><span class="op">)</span><span class="op">}</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t127" href="#t127">127</a></span><span class="t">        <span class="com"># remove internal stuff:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t128" href="#t128">128</a></span><span class="t">        <span class="nam">annotations</span> <span class="op">=</span> <span class="op">{</span><span class="nam">k</span><span class="op">:</span> <span class="nam">v</span> <span class="key">for</span> <span class="nam">k</span><span class="op">,</span> <span class="nam">v</span> <span class="key">in</span> <span class="nam">annotations</span><span class="op">.</span><span class="nam">items</span><span class="op">(</span><span class="op">)</span> <span class="key">if</span> <span class="key">not</span> <span class="nam">k</span><span class="op">.</span><span class="nam">startswith</span><span class="op">(</span><span class="str">"_"</span><span class="op">)</span><span class="op">}</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t129" href="#t129">129</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t130" href="#t130">130</a></span><span class="t">        <span class="nam">fields</span> <span class="op">=</span> <span class="op">{</span><span class="nam">fname</span><span class="op">:</span> <span class="nam">self</span><span class="op">.</span><span class="nam">_to_field</span><span class="op">(</span><span class="nam">fname</span><span class="op">,</span> <span class="nam">ftype</span><span class="op">)</span> <span class="key">for</span> <span class="nam">fname</span><span class="op">,</span> <span class="nam">ftype</span> <span class="key">in</span> <span class="nam">annotations</span><span class="op">.</span><span class="nam">items</span><span class="op">(</span><span class="op">)</span><span class="op">}</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t131" href="#t131">131</a></span><span class="t">        <span class="nam">other_kwargs</span> <span class="op">=</span> <span class="op">{</span><span class="nam">k</span><span class="op">:</span> <span class="nam">v</span> <span class="key">for</span> <span class="nam">k</span><span class="op">,</span> <span class="nam">v</span> <span class="key">in</span> <span class="nam">cls</span><span class="op">.</span><span class="nam">__dict__</span><span class="op">.</span><span class="nam">items</span><span class="op">(</span><span class="op">)</span> <span class="key">if</span> <span class="nam">k</span> <span class="key">not</span> <span class="key">in</span> <span class="nam">annotations</span> <span class="key">and</span> <span class="key">not</span> <span class="nam">k</span><span class="op">.</span><span class="nam">startswith</span><span class="op">(</span><span class="str">"_"</span><span class="op">)</span><span class="op">}</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t132" href="#t132">132</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t133" href="#t133">133</a></span><span class="t">        <span class="nam">table</span><span class="op">:</span> <span class="nam">Table</span> <span class="op">=</span> <span class="nam">self</span><span class="op">.</span><span class="nam">define_table</span><span class="op">(</span><span class="nam">tablename</span><span class="op">,</span> <span class="op">*</span><span class="nam">fields</span><span class="op">.</span><span class="nam">values</span><span class="op">(</span><span class="op">)</span><span class="op">,</span> <span class="op">**</span><span class="nam">other_kwargs</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t130" href="#t130">130</a></span><span class="t">        <span class="nam">typedfields</span> <span class="op">=</span> <span class="op">{</span><span class="nam">k</span><span class="op">:</span> <span class="nam">v</span> <span class="key">for</span> <span class="nam">k</span><span class="op">,</span> <span class="nam">v</span> <span class="key">in</span> <span class="nam">annotations</span><span class="op">.</span><span class="nam">items</span><span class="op">(</span><span class="op">)</span> <span class="key">if</span> <span class="nam">isinstance</span><span class="op">(</span><span class="nam">v</span><span class="op">,</span> <span class="nam">TypedFieldType</span><span class="op">)</span><span class="op">}</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t131" href="#t131">131</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t132" href="#t132">132</a></span><span class="t">        <span class="nam">fields</span> <span class="op">=</span> <span class="op">{</span><span class="nam">fname</span><span class="op">:</span> <span class="nam">self</span><span class="op">.</span><span class="nam">_to_field</span><span class="op">(</span><span class="nam">fname</span><span class="op">,</span> <span class="nam">ftype</span><span class="op">)</span> <span class="key">for</span> <span class="nam">fname</span><span class="op">,</span> <span class="nam">ftype</span> <span class="key">in</span> <span class="nam">annotations</span><span class="op">.</span><span class="nam">items</span><span class="op">(</span><span class="op">)</span><span class="op">}</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t133" href="#t133">133</a></span><span class="t">        <span class="nam">other_kwargs</span> <span class="op">=</span> <span class="op">{</span><span class="nam">k</span><span class="op">:</span> <span class="nam">v</span> <span class="key">for</span> <span class="nam">k</span><span class="op">,</span> <span class="nam">v</span> <span class="key">in</span> <span class="nam">cls</span><span class="op">.</span><span class="nam">__dict__</span><span class="op">.</span><span class="nam">items</span><span class="op">(</span><span class="op">)</span> <span class="key">if</span> <span class="nam">k</span> <span class="key">not</span> <span class="key">in</span> <span class="nam">annotations</span> <span class="key">and</span> <span class="key">not</span> <span class="nam">k</span><span class="op">.</span><span class="nam">startswith</span><span class="op">(</span><span class="str">"_"</span><span class="op">)</span><span class="op">}</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t134" href="#t134">134</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t135" href="#t135">135</a></span><span class="t">        <span class="key">for</span> <span class="nam">name</span><span class="op">,</span> <span class="nam">typed_field</span> <span class="key">in</span> <span class="nam">typedfields</span><span class="op">.</span><span class="nam">items</span><span class="op">(</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t136" href="#t136">136</a></span><span class="t">            <span class="nam">field</span> <span class="op">=</span> <span class="nam">fields</span><span class="op">[</span><span class="nam">name</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t137" href="#t137">137</a></span><span class="t">            <span class="nam">typed_field</span><span class="op">.</span><span class="nam">bind</span><span class="op">(</span><span class="nam">field</span><span class="op">,</span> <span class="nam">table</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t138" href="#t138">138</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t139" href="#t139">139</a></span><span class="t">        <span class="nam">cls</span><span class="op">.</span><span class="nam">__set_internals__</span><span class="op">(</span><span class="nam">db</span><span class="op">=</span><span class="nam">self</span><span class="op">,</span> <span class="nam">table</span><span class="op">=</span><span class="nam">table</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t135" href="#t135">135</a></span><span class="t">        <span class="nam">table</span><span class="op">:</span> <span class="nam">Table</span> <span class="op">=</span> <span class="nam">self</span><span class="op">.</span><span class="nam">define_table</span><span class="op">(</span><span class="nam">tablename</span><span class="op">,</span> <span class="op">*</span><span class="nam">fields</span><span class="op">.</span><span class="nam">values</span><span class="op">(</span><span class="op">)</span><span class="op">,</span> <span class="op">**</span><span class="nam">other_kwargs</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t136" href="#t136">136</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t137" href="#t137">137</a></span><span class="t">        <span class="key">for</span> <span class="nam">name</span><span class="op">,</span> <span class="nam">typed_field</span> <span class="key">in</span> <span class="nam">typedfields</span><span class="op">.</span><span class="nam">items</span><span class="op">(</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t138" href="#t138">138</a></span><span class="t">            <span class="nam">field</span> <span class="op">=</span> <span class="nam">fields</span><span class="op">[</span><span class="nam">name</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t139" href="#t139">139</a></span><span class="t">            <span class="nam">typed_field</span><span class="op">.</span><span class="nam">bind</span><span class="op">(</span><span class="nam">field</span><span class="op">,</span> <span class="nam">table</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t140" href="#t140">140</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t141" href="#t141">141</a></span><span class="t">        <span class="com"># the ACTUAL output is not TypedTable but rather pydal.Table</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t142" href="#t142">142</a></span><span class="t">        <span class="com"># but telling the editor it is T helps with hinting.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t143" href="#t143">143</a></span><span class="t">        <span class="key">return</span> <span class="nam">cls</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t144" href="#t144">144</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t145" href="#t145">145</a></span><span class="t">    <span class="key">def</span> <span class="nam">__call__</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="op">*</span><span class="nam">_args</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">,</span> <span class="op">**</span><span class="nam">kwargs</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">)</span> <span class="op">-></span> <span class="str">"TypedSet"</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t146" href="#t146">146</a></span><span class="t">        <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t147" href="#t147">147</a></span><span class="t"><span class="str">        A db instance can be called directly to perform a query.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t148" href="#t148">148</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t149" href="#t149">149</a></span><span class="t"><span class="str">        Usually, only a query is passed.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t141" href="#t141">141</a></span><span class="t">        <span class="nam">cls</span><span class="op">.</span><span class="nam">__set_internals__</span><span class="op">(</span><span class="nam">db</span><span class="op">=</span><span class="nam">self</span><span class="op">,</span> <span class="nam">table</span><span class="op">=</span><span class="nam">table</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t142" href="#t142">142</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t143" href="#t143">143</a></span><span class="t">        <span class="com"># the ACTUAL output is not TypedTable but rather pydal.Table</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t144" href="#t144">144</a></span><span class="t">        <span class="com"># but telling the editor it is T helps with hinting.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t145" href="#t145">145</a></span><span class="t">        <span class="key">return</span> <span class="nam">cls</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t146" href="#t146">146</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t147" href="#t147">147</a></span><span class="t">    <span class="key">def</span> <span class="nam">__call__</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="op">*</span><span class="nam">_args</span><span class="op">:</span> <span class="nam">T_Query</span><span class="op">,</span> <span class="op">**</span><span class="nam">kwargs</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">)</span> <span class="op">-></span> <span class="str">"TypedSet"</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t148" href="#t148">148</a></span><span class="t">        <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t149" href="#t149">149</a></span><span class="t"><span class="str">        A db instance can be called directly to perform a query.</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t150" href="#t150">150</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t151" href="#t151">151</a></span><span class="t"><span class="str">        Example:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t152" href="#t152">152</a></span><span class="t"><span class="str">            db(query).select()</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t153" href="#t153">153</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t154" href="#t154">154</a></span><span class="t"><span class="str">        """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t155" href="#t155">155</a></span><span class="t">        <span class="nam">args</span> <span class="op">=</span> <span class="nam">list</span><span class="op">(</span><span class="nam">_args</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t156" href="#t156">156</a></span><span class="t">        <span class="key">if</span> <span class="nam">args</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t157" href="#t157">157</a></span><span class="t">            <span class="nam">cls</span> <span class="op">=</span> <span class="nam">args</span><span class="op">[</span><span class="num">0</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t158" href="#t158">158</a></span><span class="t">            <span class="key">if</span> <span class="nam">isinstance</span><span class="op">(</span><span class="nam">cls</span><span class="op">,</span> <span class="nam">bool</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t159" href="#t159">159</a></span><span class="t">                <span class="key">raise</span> <span class="nam">ValueError</span><span class="op">(</span><span class="str">"Don't actually pass a bool to db()! Use a query instead."</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t160" href="#t160">160</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t161" href="#t161">161</a></span><span class="t">            <span class="key">if</span> <span class="nam">issubclass</span><span class="op">(</span><span class="nam">type</span><span class="op">(</span><span class="nam">cls</span><span class="op">)</span><span class="op">,</span> <span class="nam">type</span><span class="op">)</span> <span class="key">and</span> <span class="nam">issubclass</span><span class="op">(</span><span class="nam">cls</span><span class="op">,</span> <span class="nam">TypedTable</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t162" href="#t162">162</a></span><span class="t">                <span class="com"># table defined without @db.define decorator!</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t163" href="#t163">163</a></span><span class="t">                <span class="nam">args</span><span class="op">[</span><span class="num">0</span><span class="op">]</span> <span class="op">=</span> <span class="nam">cls</span><span class="op">.</span><span class="nam">id</span> <span class="op">!=</span> <span class="key">None</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t164" href="#t164">164</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t165" href="#t165">165</a></span><span class="t">        <span class="nam">_set</span> <span class="op">=</span> <span class="nam">super</span><span class="op">(</span><span class="op">)</span><span class="op">.</span><span class="nam">__call__</span><span class="op">(</span><span class="op">*</span><span class="nam">args</span><span class="op">,</span> <span class="op">**</span><span class="nam">kwargs</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t166" href="#t166">166</a></span><span class="t">        <span class="key">return</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">cast</span><span class="op">(</span><span class="nam">TypedSet</span><span class="op">,</span> <span class="nam">_set</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t151" href="#t151">151</a></span><span class="t"><span class="str">        Usually, only a query is passed.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t152" href="#t152">152</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t153" href="#t153">153</a></span><span class="t"><span class="str">        Example:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t154" href="#t154">154</a></span><span class="t"><span class="str">            db(query).select()</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t155" href="#t155">155</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t156" href="#t156">156</a></span><span class="t"><span class="str">        """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t157" href="#t157">157</a></span><span class="t">        <span class="nam">args</span> <span class="op">=</span> <span class="nam">list</span><span class="op">(</span><span class="nam">_args</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t158" href="#t158">158</a></span><span class="t">        <span class="key">if</span> <span class="nam">args</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t159" href="#t159">159</a></span><span class="t">            <span class="nam">cls</span> <span class="op">=</span> <span class="nam">args</span><span class="op">[</span><span class="num">0</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t160" href="#t160">160</a></span><span class="t">            <span class="key">if</span> <span class="nam">isinstance</span><span class="op">(</span><span class="nam">cls</span><span class="op">,</span> <span class="nam">bool</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t161" href="#t161">161</a></span><span class="t">                <span class="key">raise</span> <span class="nam">ValueError</span><span class="op">(</span><span class="str">"Don't actually pass a bool to db()! Use a query instead."</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t162" href="#t162">162</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t163" href="#t163">163</a></span><span class="t">            <span class="key">if</span> <span class="nam">isinstance</span><span class="op">(</span><span class="nam">cls</span><span class="op">,</span> <span class="nam">type</span><span class="op">)</span> <span class="key">and</span> <span class="nam">issubclass</span><span class="op">(</span><span class="nam">type</span><span class="op">(</span><span class="nam">cls</span><span class="op">)</span><span class="op">,</span> <span class="nam">type</span><span class="op">)</span> <span class="key">and</span> <span class="nam">issubclass</span><span class="op">(</span><span class="nam">cls</span><span class="op">,</span> <span class="nam">TypedTable</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t164" href="#t164">164</a></span><span class="t">                <span class="com"># table defined without @db.define decorator!</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t165" href="#t165">165</a></span><span class="t">                <span class="nam">_cls</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Type</span><span class="op">[</span><span class="nam">TypedTable</span><span class="op">]</span> <span class="op">=</span> <span class="nam">cls</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t166" href="#t166">166</a></span><span class="t">                <span class="nam">args</span><span class="op">[</span><span class="num">0</span><span class="op">]</span> <span class="op">=</span> <span class="nam">_cls</span><span class="op">.</span><span class="nam">id</span> <span class="op">!=</span> <span class="key">None</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t167" href="#t167">167</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t168" href="#t168">168</a></span><span class="t">    <span class="com"># todo: insert etc shadowen?</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t169" href="#t169">169</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t170" href="#t170">170</a></span><span class="t">    <span class="op">@</span><span class="nam">classmethod</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t171" href="#t171">171</a></span><span class="t">    <span class="key">def</span> <span class="nam">_build_field</span><span class="op">(</span><span class="nam">cls</span><span class="op">,</span> <span class="nam">name</span><span class="op">:</span> <span class="nam">str</span><span class="op">,</span> <span class="nam">_type</span><span class="op">:</span> <span class="nam">str</span><span class="op">,</span> <span class="op">**</span><span class="nam">kw</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">)</span> <span class="op">-></span> <span class="nam">Field</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t172" href="#t172">172</a></span><span class="t">        <span class="key">return</span> <span class="nam">Field</span><span class="op">(</span><span class="nam">name</span><span class="op">,</span> <span class="nam">_type</span><span class="op">,</span> <span class="op">**</span><span class="op">{</span><span class="op">**</span><span class="nam">cls</span><span class="op">.</span><span class="nam">default_kwargs</span><span class="op">,</span> <span class="op">**</span><span class="nam">kw</span><span class="op">}</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t173" href="#t173">173</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t174" href="#t174">174</a></span><span class="t">    <span class="op">@</span><span class="nam">classmethod</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t175" href="#t175">175</a></span><span class="t">    <span class="key">def</span> <span class="nam">_annotation_to_pydal_fieldtype</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t176" href="#t176">176</a></span><span class="t">        <span class="nam">cls</span><span class="op">,</span> <span class="nam">_ftype</span><span class="op">:</span> <span class="nam">T_annotation</span><span class="op">,</span> <span class="nam">mut_kw</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">MutableMapping</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t177" href="#t177">177</a></span><span class="t">    <span class="op">)</span> <span class="op">-></span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Optional</span><span class="op">[</span><span class="nam">str</span><span class="op">]</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t178" href="#t178">178</a></span><span class="t">        <span class="com"># ftype can be a union or type. typing.cast is sometimes used to tell mypy when it's not a union.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t179" href="#t179">179</a></span><span class="t">        <span class="nam">ftype</span> <span class="op">=</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">cast</span><span class="op">(</span><span class="nam">type</span><span class="op">,</span> <span class="nam">_ftype</span><span class="op">)</span>  <span class="com"># cast from typing.Type to type to make mypy happy)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t180" href="#t180">180</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t181" href="#t181">181</a></span><span class="t">        <span class="key">if</span> <span class="nam">mapping</span> <span class="op">:=</span> <span class="nam">BASIC_MAPPINGS</span><span class="op">.</span><span class="nam">get</span><span class="op">(</span><span class="nam">ftype</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t182" href="#t182">182</a></span><span class="t">            <span class="com"># basi types</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t183" href="#t183">183</a></span><span class="t">            <span class="key">return</span> <span class="nam">mapping</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t184" href="#t184">184</a></span><span class="t">        <span class="key">elif</span> <span class="nam">isinstance</span><span class="op">(</span><span class="nam">ftype</span><span class="op">,</span> <span class="nam">Table</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t185" href="#t185">185</a></span><span class="t">            <span class="com"># db.table</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t186" href="#t186">186</a></span><span class="t">            <span class="key">return</span> <span class="str">f"reference {ftype._tablename}"</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t187" href="#t187">187</a></span><span class="t">        <span class="key">elif</span> <span class="nam">issubclass</span><span class="op">(</span><span class="nam">type</span><span class="op">(</span><span class="nam">ftype</span><span class="op">)</span><span class="op">,</span> <span class="nam">type</span><span class="op">)</span> <span class="key">and</span> <span class="nam">issubclass</span><span class="op">(</span><span class="nam">ftype</span><span class="op">,</span> <span class="nam">TypedTable</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t188" href="#t188">188</a></span><span class="t">            <span class="com"># SomeTable</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t189" href="#t189">189</a></span><span class="t">            <span class="nam">snakename</span> <span class="op">=</span> <span class="nam">cls</span><span class="op">.</span><span class="nam">_to_snake</span><span class="op">(</span><span class="nam">ftype</span><span class="op">.</span><span class="nam">__name__</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t190" href="#t190">190</a></span><span class="t">            <span class="key">return</span> <span class="str">f"reference {snakename}"</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t191" href="#t191">191</a></span><span class="t">        <span class="key">elif</span> <span class="nam">isinstance</span><span class="op">(</span><span class="nam">ftype</span><span class="op">,</span> <span class="nam">TypedFieldType</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t192" href="#t192">192</a></span><span class="t">            <span class="com"># FieldType(type, ...)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t193" href="#t193">193</a></span><span class="t">            <span class="key">return</span> <span class="nam">ftype</span><span class="op">.</span><span class="nam">_to_field</span><span class="op">(</span><span class="nam">mut_kw</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t194" href="#t194">194</a></span><span class="t">        <span class="key">elif</span> <span class="nam">isinstance</span><span class="op">(</span><span class="nam">ftype</span><span class="op">,</span> <span class="nam">types</span><span class="op">.</span><span class="nam">GenericAlias</span><span class="op">)</span> <span class="key">and</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">get_origin</span><span class="op">(</span><span class="nam">ftype</span><span class="op">)</span> <span class="key">is</span> <span class="nam">list</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t195" href="#t195">195</a></span><span class="t">            <span class="com"># list[str] -> str -> string -> list:string</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t196" href="#t196">196</a></span><span class="t">            <span class="nam">_child_type</span> <span class="op">=</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">get_args</span><span class="op">(</span><span class="nam">ftype</span><span class="op">)</span><span class="op">[</span><span class="num">0</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t197" href="#t197">197</a></span><span class="t">            <span class="nam">_child_type</span> <span class="op">=</span> <span class="nam">cls</span><span class="op">.</span><span class="nam">_annotation_to_pydal_fieldtype</span><span class="op">(</span><span class="nam">_child_type</span><span class="op">,</span> <span class="nam">mut_kw</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t198" href="#t198">198</a></span><span class="t">            <span class="key">return</span> <span class="str">f"list:{_child_type}"</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t199" href="#t199">199</a></span><span class="t">        <span class="key">elif</span> <span class="nam">is_union</span><span class="op">(</span><span class="nam">ftype</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t200" href="#t200">200</a></span><span class="t">            <span class="com"># str | int -> UnionType</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t201" href="#t201">201</a></span><span class="t">            <span class="com"># typing.Union[str | int] -> typing._UnionGenericAlias</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t202" href="#t202">202</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t203" href="#t203">203</a></span><span class="t">            <span class="com"># typing.Optional[type] == type | None</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t204" href="#t204">204</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t205" href="#t205">205</a></span><span class="t">            <span class="key">match</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">get_args</span><span class="op">(</span><span class="nam">ftype</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t206" href="#t206">206</a></span><span class="t">                <span class="key">case</span> <span class="op">(</span><span class="nam">_child_type</span><span class="op">,</span> <span class="nam">_Types</span><span class="op">.</span><span class="nam">NONETYPE</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t207" href="#t207">207</a></span><span class="t">                    <span class="com"># good union of Nullable</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t208" href="#t208">208</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t209" href="#t209">209</a></span><span class="t">                    <span class="com"># if a field is optional, it is nullable:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t210" href="#t210">210</a></span><span class="t">                    <span class="nam">mut_kw</span><span class="op">[</span><span class="str">"notnull"</span><span class="op">]</span> <span class="op">=</span> <span class="key">False</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t211" href="#t211">211</a></span><span class="t">                    <span class="key">return</span> <span class="nam">cls</span><span class="op">.</span><span class="nam">_annotation_to_pydal_fieldtype</span><span class="op">(</span><span class="nam">_child_type</span><span class="op">,</span> <span class="nam">mut_kw</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t212" href="#t212">212</a></span><span class="t">                <span class="key">case</span> <span class="nam">_</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t213" href="#t213">213</a></span><span class="t">                    <span class="com"># two types is not supported by the db!</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t214" href="#t214">214</a></span><span class="t">                    <span class="key">return</span> <span class="key">None</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t215" href="#t215">215</a></span><span class="t">        <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t216" href="#t216">216</a></span><span class="t">            <span class="key">return</span> <span class="key">None</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t217" href="#t217">217</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t218" href="#t218">218</a></span><span class="t">    <span class="op">@</span><span class="nam">classmethod</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t219" href="#t219">219</a></span><span class="t">    <span class="key">def</span> <span class="nam">_to_field</span><span class="op">(</span><span class="nam">cls</span><span class="op">,</span> <span class="nam">fname</span><span class="op">:</span> <span class="nam">str</span><span class="op">,</span> <span class="nam">ftype</span><span class="op">:</span> <span class="nam">type</span><span class="op">,</span> <span class="op">**</span><span class="nam">kw</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">)</span> <span class="op">-></span> <span class="nam">Field</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t220" href="#t220">220</a></span><span class="t">        <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t221" href="#t221">221</a></span><span class="t"><span class="str">        Convert a annotation into a pydal Field.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t222" href="#t222">222</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t223" href="#t223">223</a></span><span class="t"><span class="str">        Args:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t224" href="#t224">224</a></span><span class="t"><span class="str">            fname: name of the property</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t225" href="#t225">225</a></span><span class="t"><span class="str">            ftype: annotation of the property</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t226" href="#t226">226</a></span><span class="t"><span class="str">            kw: when using TypedField or a function returning it (e.g. StringField),</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t227" href="#t227">227</a></span><span class="t"><span class="str">                keyword args can be used to pass any other settings you would normally to a pydal Field</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t228" href="#t228">228</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t229" href="#t229">229</a></span><span class="t"><span class="str">        -> pydal.Field(fname, ftype, **kw)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t230" href="#t230">230</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t231" href="#t231">231</a></span><span class="t"><span class="str">        Example:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t232" href="#t232">232</a></span><span class="t"><span class="str">            class MyTable:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t233" href="#t233">233</a></span><span class="t"><span class="str">                fname: ftype</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t234" href="#t234">234</a></span><span class="t"><span class="str">                id: int</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t235" href="#t235">235</a></span><span class="t"><span class="str">                name: str</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t236" href="#t236">236</a></span><span class="t"><span class="str">                reference: Table</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t237" href="#t237">237</a></span><span class="t"><span class="str">                other: TypedField(str, default="John Doe")  # default will be in kwargs</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t238" href="#t238">238</a></span><span class="t"><span class="str">        """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t239" href="#t239">239</a></span><span class="t">        <span class="nam">fname</span> <span class="op">=</span> <span class="nam">cls</span><span class="op">.</span><span class="nam">_to_snake</span><span class="op">(</span><span class="nam">fname</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t240" href="#t240">240</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t241" href="#t241">241</a></span><span class="t">        <span class="key">if</span> <span class="nam">converted_type</span> <span class="op">:=</span> <span class="nam">cls</span><span class="op">.</span><span class="nam">_annotation_to_pydal_fieldtype</span><span class="op">(</span><span class="nam">ftype</span><span class="op">,</span> <span class="nam">kw</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t242" href="#t242">242</a></span><span class="t">            <span class="key">return</span> <span class="nam">cls</span><span class="op">.</span><span class="nam">_build_field</span><span class="op">(</span><span class="nam">fname</span><span class="op">,</span> <span class="nam">converted_type</span><span class="op">,</span> <span class="op">**</span><span class="nam">kw</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t243" href="#t243">243</a></span><span class="t">        <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t244" href="#t244">244</a></span><span class="t">            <span class="key">raise</span> <span class="nam">NotImplementedError</span><span class="op">(</span><span class="str">f"Unsupported type {ftype}/{type(ftype)}"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t245" href="#t245">245</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t246" href="#t246">246</a></span><span class="t">    <span class="op">@</span><span class="nam">staticmethod</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t247" href="#t247">247</a></span><span class="t">    <span class="key">def</span> <span class="nam">_to_snake</span><span class="op">(</span><span class="nam">camel</span><span class="op">:</span> <span class="nam">str</span><span class="op">)</span> <span class="op">-></span> <span class="nam">str</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t248" href="#t248">248</a></span><span class="t">        <span class="com"># https://stackoverflow.com/a/44969381</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t249" href="#t249">249</a></span><span class="t">        <span class="key">return</span> <span class="str">""</span><span class="op">.</span><span class="nam">join</span><span class="op">(</span><span class="op">[</span><span class="str">f"_{c.lower()}"</span> <span class="key">if</span> <span class="nam">c</span><span class="op">.</span><span class="nam">isupper</span><span class="op">(</span><span class="op">)</span> <span class="key">else</span> <span class="nam">c</span> <span class="key">for</span> <span class="nam">c</span> <span class="key">in</span> <span class="nam">camel</span><span class="op">]</span><span class="op">)</span><span class="op">.</span><span class="nam">lstrip</span><span class="op">(</span><span class="str">"_"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t250" href="#t250">250</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t251" href="#t251">251</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t252" href="#t252">252</a></span><span class="t"><span class="key">class</span> <span class="nam">TypedTableMeta</span><span class="op">(</span><span class="nam">type</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t253" href="#t253">253</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t254" href="#t254">254</a></span><span class="t"><span class="str">    Meta class allows getattribute on class variables instead instance variables.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t255" href="#t255">255</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t256" href="#t256">256</a></span><span class="t"><span class="str">    Used in `class TypedTable(Table, metaclass=TypedTableMeta)`</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t257" href="#t257">257</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t168" href="#t168">168</a></span><span class="t">        <span class="nam">_set</span> <span class="op">=</span> <span class="nam">super</span><span class="op">(</span><span class="op">)</span><span class="op">.</span><span class="nam">__call__</span><span class="op">(</span><span class="op">*</span><span class="nam">args</span><span class="op">,</span> <span class="op">**</span><span class="nam">kwargs</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t169" href="#t169">169</a></span><span class="t">        <span class="key">return</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">cast</span><span class="op">(</span><span class="nam">TypedSet</span><span class="op">,</span> <span class="nam">_set</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t170" href="#t170">170</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t171" href="#t171">171</a></span><span class="t">    <span class="com"># todo: insert etc shadowen?</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t172" href="#t172">172</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t173" href="#t173">173</a></span><span class="t">    <span class="op">@</span><span class="nam">classmethod</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t174" href="#t174">174</a></span><span class="t">    <span class="key">def</span> <span class="nam">_build_field</span><span class="op">(</span><span class="nam">cls</span><span class="op">,</span> <span class="nam">name</span><span class="op">:</span> <span class="nam">str</span><span class="op">,</span> <span class="nam">_type</span><span class="op">:</span> <span class="nam">str</span><span class="op">,</span> <span class="op">**</span><span class="nam">kw</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">)</span> <span class="op">-></span> <span class="nam">Field</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t175" href="#t175">175</a></span><span class="t">        <span class="key">return</span> <span class="nam">Field</span><span class="op">(</span><span class="nam">name</span><span class="op">,</span> <span class="nam">_type</span><span class="op">,</span> <span class="op">**</span><span class="op">{</span><span class="op">**</span><span class="nam">cls</span><span class="op">.</span><span class="nam">default_kwargs</span><span class="op">,</span> <span class="op">**</span><span class="nam">kw</span><span class="op">}</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t176" href="#t176">176</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t177" href="#t177">177</a></span><span class="t">    <span class="op">@</span><span class="nam">classmethod</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t178" href="#t178">178</a></span><span class="t">    <span class="key">def</span> <span class="nam">_annotation_to_pydal_fieldtype</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t179" href="#t179">179</a></span><span class="t">        <span class="nam">cls</span><span class="op">,</span> <span class="nam">_ftype</span><span class="op">:</span> <span class="nam">T_annotation</span><span class="op">,</span> <span class="nam">mut_kw</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">MutableMapping</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t180" href="#t180">180</a></span><span class="t">    <span class="op">)</span> <span class="op">-></span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Optional</span><span class="op">[</span><span class="nam">str</span><span class="op">]</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t181" href="#t181">181</a></span><span class="t">        <span class="com"># ftype can be a union or type. typing.cast is sometimes used to tell mypy when it's not a union.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t182" href="#t182">182</a></span><span class="t">        <span class="nam">ftype</span> <span class="op">=</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">cast</span><span class="op">(</span><span class="nam">type</span><span class="op">,</span> <span class="nam">_ftype</span><span class="op">)</span>  <span class="com"># cast from typing.Type to type to make mypy happy)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t183" href="#t183">183</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t184" href="#t184">184</a></span><span class="t">        <span class="key">if</span> <span class="nam">mapping</span> <span class="op">:=</span> <span class="nam">BASIC_MAPPINGS</span><span class="op">.</span><span class="nam">get</span><span class="op">(</span><span class="nam">ftype</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t185" href="#t185">185</a></span><span class="t">            <span class="com"># basi types</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t186" href="#t186">186</a></span><span class="t">            <span class="key">return</span> <span class="nam">mapping</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t187" href="#t187">187</a></span><span class="t">        <span class="key">elif</span> <span class="nam">isinstance</span><span class="op">(</span><span class="nam">ftype</span><span class="op">,</span> <span class="nam">Table</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t188" href="#t188">188</a></span><span class="t">            <span class="com"># db.table</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t189" href="#t189">189</a></span><span class="t">            <span class="key">return</span> <span class="str">f"reference {ftype._tablename}"</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t190" href="#t190">190</a></span><span class="t">        <span class="key">elif</span> <span class="nam">issubclass</span><span class="op">(</span><span class="nam">type</span><span class="op">(</span><span class="nam">ftype</span><span class="op">)</span><span class="op">,</span> <span class="nam">type</span><span class="op">)</span> <span class="key">and</span> <span class="nam">issubclass</span><span class="op">(</span><span class="nam">ftype</span><span class="op">,</span> <span class="nam">TypedTable</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t191" href="#t191">191</a></span><span class="t">            <span class="com"># SomeTable</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t192" href="#t192">192</a></span><span class="t">            <span class="nam">snakename</span> <span class="op">=</span> <span class="nam">cls</span><span class="op">.</span><span class="nam">_to_snake</span><span class="op">(</span><span class="nam">ftype</span><span class="op">.</span><span class="nam">__name__</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t193" href="#t193">193</a></span><span class="t">            <span class="key">return</span> <span class="str">f"reference {snakename}"</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t194" href="#t194">194</a></span><span class="t">        <span class="key">elif</span> <span class="nam">isinstance</span><span class="op">(</span><span class="nam">ftype</span><span class="op">,</span> <span class="nam">TypedFieldType</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t195" href="#t195">195</a></span><span class="t">            <span class="com"># FieldType(type, ...)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t196" href="#t196">196</a></span><span class="t">            <span class="key">return</span> <span class="nam">ftype</span><span class="op">.</span><span class="nam">_to_field</span><span class="op">(</span><span class="nam">mut_kw</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t197" href="#t197">197</a></span><span class="t">        <span class="key">elif</span> <span class="nam">isinstance</span><span class="op">(</span><span class="nam">ftype</span><span class="op">,</span> <span class="nam">types</span><span class="op">.</span><span class="nam">GenericAlias</span><span class="op">)</span> <span class="key">and</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">get_origin</span><span class="op">(</span><span class="nam">ftype</span><span class="op">)</span> <span class="key">is</span> <span class="nam">list</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t198" href="#t198">198</a></span><span class="t">            <span class="com"># list[str] -> str -> string -> list:string</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t199" href="#t199">199</a></span><span class="t">            <span class="nam">_child_type</span> <span class="op">=</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">get_args</span><span class="op">(</span><span class="nam">ftype</span><span class="op">)</span><span class="op">[</span><span class="num">0</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t200" href="#t200">200</a></span><span class="t">            <span class="nam">_child_type</span> <span class="op">=</span> <span class="nam">cls</span><span class="op">.</span><span class="nam">_annotation_to_pydal_fieldtype</span><span class="op">(</span><span class="nam">_child_type</span><span class="op">,</span> <span class="nam">mut_kw</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t201" href="#t201">201</a></span><span class="t">            <span class="key">return</span> <span class="str">f"list:{_child_type}"</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t202" href="#t202">202</a></span><span class="t">        <span class="key">elif</span> <span class="nam">is_union</span><span class="op">(</span><span class="nam">ftype</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t203" href="#t203">203</a></span><span class="t">            <span class="com"># str | int -> UnionType</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t204" href="#t204">204</a></span><span class="t">            <span class="com"># typing.Union[str | int] -> typing._UnionGenericAlias</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t205" href="#t205">205</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t206" href="#t206">206</a></span><span class="t">            <span class="com"># typing.Optional[type] == type | None</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t207" href="#t207">207</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t208" href="#t208">208</a></span><span class="t">            <span class="key">match</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">get_args</span><span class="op">(</span><span class="nam">ftype</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t209" href="#t209">209</a></span><span class="t">                <span class="key">case</span> <span class="op">(</span><span class="nam">_child_type</span><span class="op">,</span> <span class="nam">_Types</span><span class="op">.</span><span class="nam">NONETYPE</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t210" href="#t210">210</a></span><span class="t">                    <span class="com"># good union of Nullable</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t211" href="#t211">211</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t212" href="#t212">212</a></span><span class="t">                    <span class="com"># if a field is optional, it is nullable:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t213" href="#t213">213</a></span><span class="t">                    <span class="nam">mut_kw</span><span class="op">[</span><span class="str">"notnull"</span><span class="op">]</span> <span class="op">=</span> <span class="key">False</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t214" href="#t214">214</a></span><span class="t">                    <span class="key">return</span> <span class="nam">cls</span><span class="op">.</span><span class="nam">_annotation_to_pydal_fieldtype</span><span class="op">(</span><span class="nam">_child_type</span><span class="op">,</span> <span class="nam">mut_kw</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t215" href="#t215">215</a></span><span class="t">                <span class="key">case</span> <span class="nam">_</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t216" href="#t216">216</a></span><span class="t">                    <span class="com"># two types is not supported by the db!</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t217" href="#t217">217</a></span><span class="t">                    <span class="key">return</span> <span class="key">None</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t218" href="#t218">218</a></span><span class="t">        <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t219" href="#t219">219</a></span><span class="t">            <span class="key">return</span> <span class="key">None</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t220" href="#t220">220</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t221" href="#t221">221</a></span><span class="t">    <span class="op">@</span><span class="nam">classmethod</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t222" href="#t222">222</a></span><span class="t">    <span class="key">def</span> <span class="nam">_to_field</span><span class="op">(</span><span class="nam">cls</span><span class="op">,</span> <span class="nam">fname</span><span class="op">:</span> <span class="nam">str</span><span class="op">,</span> <span class="nam">ftype</span><span class="op">:</span> <span class="nam">type</span><span class="op">,</span> <span class="op">**</span><span class="nam">kw</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">)</span> <span class="op">-></span> <span class="nam">Field</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t223" href="#t223">223</a></span><span class="t">        <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t224" href="#t224">224</a></span><span class="t"><span class="str">        Convert a annotation into a pydal Field.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t225" href="#t225">225</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t226" href="#t226">226</a></span><span class="t"><span class="str">        Args:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t227" href="#t227">227</a></span><span class="t"><span class="str">            fname: name of the property</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t228" href="#t228">228</a></span><span class="t"><span class="str">            ftype: annotation of the property</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t229" href="#t229">229</a></span><span class="t"><span class="str">            kw: when using TypedField or a function returning it (e.g. StringField),</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t230" href="#t230">230</a></span><span class="t"><span class="str">                keyword args can be used to pass any other settings you would normally to a pydal Field</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t231" href="#t231">231</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t232" href="#t232">232</a></span><span class="t"><span class="str">        -> pydal.Field(fname, ftype, **kw)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t233" href="#t233">233</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t234" href="#t234">234</a></span><span class="t"><span class="str">        Example:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t235" href="#t235">235</a></span><span class="t"><span class="str">            class MyTable:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t236" href="#t236">236</a></span><span class="t"><span class="str">                fname: ftype</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t237" href="#t237">237</a></span><span class="t"><span class="str">                id: int</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t238" href="#t238">238</a></span><span class="t"><span class="str">                name: str</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t239" href="#t239">239</a></span><span class="t"><span class="str">                reference: Table</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t240" href="#t240">240</a></span><span class="t"><span class="str">                other: TypedField(str, default="John Doe")  # default will be in kwargs</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t241" href="#t241">241</a></span><span class="t"><span class="str">        """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t242" href="#t242">242</a></span><span class="t">        <span class="nam">fname</span> <span class="op">=</span> <span class="nam">cls</span><span class="op">.</span><span class="nam">_to_snake</span><span class="op">(</span><span class="nam">fname</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t243" href="#t243">243</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t244" href="#t244">244</a></span><span class="t">        <span class="key">if</span> <span class="nam">converted_type</span> <span class="op">:=</span> <span class="nam">cls</span><span class="op">.</span><span class="nam">_annotation_to_pydal_fieldtype</span><span class="op">(</span><span class="nam">ftype</span><span class="op">,</span> <span class="nam">kw</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t245" href="#t245">245</a></span><span class="t">            <span class="key">return</span> <span class="nam">cls</span><span class="op">.</span><span class="nam">_build_field</span><span class="op">(</span><span class="nam">fname</span><span class="op">,</span> <span class="nam">converted_type</span><span class="op">,</span> <span class="op">**</span><span class="nam">kw</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t246" href="#t246">246</a></span><span class="t">        <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t247" href="#t247">247</a></span><span class="t">            <span class="key">raise</span> <span class="nam">NotImplementedError</span><span class="op">(</span><span class="str">f"Unsupported type {ftype}/{type(ftype)}"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t248" href="#t248">248</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t249" href="#t249">249</a></span><span class="t">    <span class="op">@</span><span class="nam">staticmethod</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t250" href="#t250">250</a></span><span class="t">    <span class="key">def</span> <span class="nam">_to_snake</span><span class="op">(</span><span class="nam">camel</span><span class="op">:</span> <span class="nam">str</span><span class="op">)</span> <span class="op">-></span> <span class="nam">str</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t251" href="#t251">251</a></span><span class="t">        <span class="com"># https://stackoverflow.com/a/44969381</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t252" href="#t252">252</a></span><span class="t">        <span class="key">return</span> <span class="str">""</span><span class="op">.</span><span class="nam">join</span><span class="op">(</span><span class="op">[</span><span class="str">f"_{c.lower()}"</span> <span class="key">if</span> <span class="nam">c</span><span class="op">.</span><span class="nam">isupper</span><span class="op">(</span><span class="op">)</span> <span class="key">else</span> <span class="nam">c</span> <span class="key">for</span> <span class="nam">c</span> <span class="key">in</span> <span class="nam">camel</span><span class="op">]</span><span class="op">)</span><span class="op">.</span><span class="nam">lstrip</span><span class="op">(</span><span class="str">"_"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t253" href="#t253">253</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t254" href="#t254">254</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t255" href="#t255">255</a></span><span class="t"><span class="key">class</span> <span class="nam">TypedTableMeta</span><span class="op">(</span><span class="nam">type</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t256" href="#t256">256</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t257" href="#t257">257</a></span><span class="t"><span class="str">    Meta class allows getattribute on class variables instead instance variables.</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t258" href="#t258">258</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t259" href="#t259">259</a></span><span class="t">    <span class="key">def</span> <span class="nam">__getattr__</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">key</span><span class="op">:</span> <span class="nam">str</span><span class="op">)</span> <span class="op">-></span> <span class="nam">Field</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t260" href="#t260">260</a></span><span class="t">        <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t261" href="#t261">261</a></span><span class="t"><span class="str">        The getattr method is only called when getattribute can't find something.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t262" href="#t262">262</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t263" href="#t263">263</a></span><span class="t"><span class="str">        `__get_table_column__` is defined in `TypedTable`</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t264" href="#t264">264</a></span><span class="t"><span class="str">        """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t265" href="#t265">265</a></span><span class="t">        <span class="key">return</span> <span class="nam">self</span><span class="op">.</span><span class="nam">__get_table_column__</span><span class="op">(</span><span class="nam">key</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t266" href="#t266">266</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t267" href="#t267">267</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t268" href="#t268">268</a></span><span class="t"><span class="key">class</span> <span class="nam">TypedTable</span><span class="op">(</span><span class="nam">Table</span><span class="op">,</span> <span class="nam">metaclass</span><span class="op">=</span><span class="nam">TypedTableMeta</span><span class="op">)</span><span class="op">:</span>  <span class="com"># type: ignore</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t269" href="#t269">269</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t270" href="#t270">270</a></span><span class="t"><span class="str">    Typed version of pydal.Table, does not really do anything itself but forwards logic to pydal.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t271" href="#t271">271</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t272" href="#t272">272</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t273" href="#t273">273</a></span><span class="t">    <span class="nam">id</span><span class="op">:</span> <span class="nam">int</span>  <span class="com"># noqa: 'id' has to be id since that's the db column</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t274" href="#t274">274</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t275" href="#t275">275</a></span><span class="t">    <span class="com"># set up by db.define:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t276" href="#t276">276</a></span><span class="t">    <span class="nam">__db</span><span class="op">:</span> <span class="nam">TypeDAL</span> <span class="op">|</span> <span class="key">None</span> <span class="op">=</span> <span class="key">None</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t277" href="#t277">277</a></span><span class="t">    <span class="nam">__table</span><span class="op">:</span> <span class="nam">Table</span> <span class="op">|</span> <span class="key">None</span> <span class="op">=</span> <span class="key">None</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t278" href="#t278">278</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t279" href="#t279">279</a></span><span class="t">    <span class="op">@</span><span class="nam">classmethod</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t280" href="#t280">280</a></span><span class="t">    <span class="key">def</span> <span class="nam">__set_internals__</span><span class="op">(</span><span class="nam">cls</span><span class="op">,</span> <span class="nam">db</span><span class="op">:</span> <span class="nam">pydal</span><span class="op">.</span><span class="nam">DAL</span><span class="op">,</span> <span class="nam">table</span><span class="op">:</span> <span class="nam">Table</span><span class="op">)</span> <span class="op">-></span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t281" href="#t281">281</a></span><span class="t">        <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t282" href="#t282">282</a></span><span class="t"><span class="str">        Store the related database and pydal table for later usage.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t283" href="#t283">283</a></span><span class="t"><span class="str">        """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t284" href="#t284">284</a></span><span class="t">        <span class="nam">cls</span><span class="op">.</span><span class="nam">__db</span> <span class="op">=</span> <span class="nam">db</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t285" href="#t285">285</a></span><span class="t">        <span class="nam">cls</span><span class="op">.</span><span class="nam">__table</span> <span class="op">=</span> <span class="nam">table</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t286" href="#t286">286</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t287" href="#t287">287</a></span><span class="t">    <span class="op">@</span><span class="nam">classmethod</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t288" href="#t288">288</a></span><span class="t">    <span class="key">def</span> <span class="nam">__get_table_column__</span><span class="op">(</span><span class="nam">cls</span><span class="op">,</span> <span class="nam">col</span><span class="op">:</span> <span class="nam">str</span><span class="op">)</span> <span class="op">-></span> <span class="nam">Field</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t289" href="#t289">289</a></span><span class="t">        <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t290" href="#t290">290</a></span><span class="t"><span class="str">        Magic method used by TypedTableMeta to get a database field with dot notation on a class.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t291" href="#t291">291</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t292" href="#t292">292</a></span><span class="t"><span class="str">        Example:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t293" href="#t293">293</a></span><span class="t"><span class="str">            SomeTypedTable.col -> db.table.col (via TypedTableMeta.__getattr__)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t259" href="#t259">259</a></span><span class="t"><span class="str">    Used in `class TypedTable(Table, metaclass=TypedTableMeta)`</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t260" href="#t260">260</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t261" href="#t261">261</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t262" href="#t262">262</a></span><span class="t">    <span class="key">def</span> <span class="nam">__getattr__</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">key</span><span class="op">:</span> <span class="nam">str</span><span class="op">)</span> <span class="op">-></span> <span class="nam">Field</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t263" href="#t263">263</a></span><span class="t">        <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t264" href="#t264">264</a></span><span class="t"><span class="str">        The getattr method is only called when getattribute can't find something.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t265" href="#t265">265</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t266" href="#t266">266</a></span><span class="t"><span class="str">        `__get_table_column__` is defined in `TypedTable`</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t267" href="#t267">267</a></span><span class="t"><span class="str">        """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t268" href="#t268">268</a></span><span class="t">        <span class="key">return</span> <span class="nam">self</span><span class="op">.</span><span class="nam">__get_table_column__</span><span class="op">(</span><span class="nam">key</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t269" href="#t269">269</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t270" href="#t270">270</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t271" href="#t271">271</a></span><span class="t"><span class="key">class</span> <span class="nam">TypedTable</span><span class="op">(</span><span class="nam">Table</span><span class="op">,</span> <span class="nam">metaclass</span><span class="op">=</span><span class="nam">TypedTableMeta</span><span class="op">)</span><span class="op">:</span>  <span class="com"># type: ignore</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t272" href="#t272">272</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t273" href="#t273">273</a></span><span class="t"><span class="str">    Typed version of pydal.Table, does not really do anything itself but forwards logic to pydal.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t274" href="#t274">274</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t275" href="#t275">275</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t276" href="#t276">276</a></span><span class="t">    <span class="nam">id</span><span class="op">:</span> <span class="nam">int</span>  <span class="com"># noqa: 'id' has to be id since that's the db column</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t277" href="#t277">277</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t278" href="#t278">278</a></span><span class="t">    <span class="com"># set up by db.define:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t279" href="#t279">279</a></span><span class="t">    <span class="nam">__db</span><span class="op">:</span> <span class="nam">TypeDAL</span> <span class="op">|</span> <span class="key">None</span> <span class="op">=</span> <span class="key">None</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t280" href="#t280">280</a></span><span class="t">    <span class="nam">__table</span><span class="op">:</span> <span class="nam">Table</span> <span class="op">|</span> <span class="key">None</span> <span class="op">=</span> <span class="key">None</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t281" href="#t281">281</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t282" href="#t282">282</a></span><span class="t">    <span class="op">@</span><span class="nam">classmethod</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t283" href="#t283">283</a></span><span class="t">    <span class="key">def</span> <span class="nam">__set_internals__</span><span class="op">(</span><span class="nam">cls</span><span class="op">,</span> <span class="nam">db</span><span class="op">:</span> <span class="nam">pydal</span><span class="op">.</span><span class="nam">DAL</span><span class="op">,</span> <span class="nam">table</span><span class="op">:</span> <span class="nam">Table</span><span class="op">)</span> <span class="op">-></span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t284" href="#t284">284</a></span><span class="t">        <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t285" href="#t285">285</a></span><span class="t"><span class="str">        Store the related database and pydal table for later usage.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t286" href="#t286">286</a></span><span class="t"><span class="str">        """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t287" href="#t287">287</a></span><span class="t">        <span class="nam">cls</span><span class="op">.</span><span class="nam">__db</span> <span class="op">=</span> <span class="nam">db</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t288" href="#t288">288</a></span><span class="t">        <span class="nam">cls</span><span class="op">.</span><span class="nam">__table</span> <span class="op">=</span> <span class="nam">table</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t289" href="#t289">289</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t290" href="#t290">290</a></span><span class="t">    <span class="op">@</span><span class="nam">classmethod</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t291" href="#t291">291</a></span><span class="t">    <span class="key">def</span> <span class="nam">__get_table_column__</span><span class="op">(</span><span class="nam">cls</span><span class="op">,</span> <span class="nam">col</span><span class="op">:</span> <span class="nam">str</span><span class="op">)</span> <span class="op">-></span> <span class="nam">Field</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t292" href="#t292">292</a></span><span class="t">        <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t293" href="#t293">293</a></span><span class="t"><span class="str">        Magic method used by TypedTableMeta to get a database field with dot notation on a class.</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t294" href="#t294">294</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t295" href="#t295">295</a></span><span class="t"><span class="str">        """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t296" href="#t296">296</a></span><span class="t">        <span class="com">#</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t297" href="#t297">297</a></span><span class="t">        <span class="key">if</span> <span class="nam">cls</span><span class="op">.</span><span class="nam">__table</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t298" href="#t298">298</a></span><span class="t">            <span class="key">return</span> <span class="nam">cls</span><span class="op">.</span><span class="nam">__table</span><span class="op">[</span><span class="nam">col</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t299" href="#t299">299</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t300" href="#t300">300</a></span><span class="t">    <span class="key">def</span> <span class="nam">__new__</span><span class="op">(</span><span class="nam">cls</span><span class="op">,</span> <span class="op">*</span><span class="nam">a</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">,</span> <span class="op">**</span><span class="nam">kw</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">)</span> <span class="op">-></span> <span class="nam">Row</span><span class="op">:</span>  <span class="com"># or none!</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t301" href="#t301">301</a></span><span class="t">        <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t302" href="#t302">302</a></span><span class="t"><span class="str">        When e.g. Table(id=0) is called without db.define, \</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t303" href="#t303">303</a></span><span class="t"><span class="str">        this catches it and forwards for proper behavior.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t304" href="#t304">304</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t305" href="#t305">305</a></span><span class="t"><span class="str">        Args:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t306" href="#t306">306</a></span><span class="t"><span class="str">            *a: can be for example Table(&lt;id>)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t307" href="#t307">307</a></span><span class="t"><span class="str">            **kw: can be for example Table(slug=&lt;slug>)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t308" href="#t308">308</a></span><span class="t"><span class="str">        """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t309" href="#t309">309</a></span><span class="t">        <span class="key">if</span> <span class="key">not</span> <span class="nam">cls</span><span class="op">.</span><span class="nam">__table</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t310" href="#t310">310</a></span><span class="t">            <span class="key">raise</span> <span class="nam">EnvironmentError</span><span class="op">(</span><span class="str">"@define or db.define is not called on this class yet!"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t311" href="#t311">311</a></span><span class="t">        <span class="key">return</span> <span class="nam">cls</span><span class="op">.</span><span class="nam">__table</span><span class="op">(</span><span class="op">*</span><span class="nam">a</span><span class="op">,</span> <span class="op">**</span><span class="nam">kw</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t312" href="#t312">312</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t313" href="#t313">313</a></span><span class="t">    <span class="op">@</span><span class="nam">classmethod</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t314" href="#t314">314</a></span><span class="t">    <span class="key">def</span> <span class="nam">insert</span><span class="op">(</span><span class="nam">cls</span><span class="op">,</span> <span class="op">**</span><span class="nam">fields</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">)</span> <span class="op">-></span> <span class="nam">int</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t315" href="#t315">315</a></span><span class="t">        <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t316" href="#t316">316</a></span><span class="t"><span class="str">        This is only called when db.define is not used as a decorator.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t317" href="#t317">317</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t318" href="#t318">318</a></span><span class="t"><span class="str">        cls.__table functions as 'self'</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t319" href="#t319">319</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t320" href="#t320">320</a></span><span class="t"><span class="str">        Args:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t321" href="#t321">321</a></span><span class="t"><span class="str">            **fields: anything you want to insert in the database</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t295" href="#t295">295</a></span><span class="t"><span class="str">        Example:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t296" href="#t296">296</a></span><span class="t"><span class="str">            SomeTypedTable.col -> db.table.col (via TypedTableMeta.__getattr__)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t297" href="#t297">297</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t298" href="#t298">298</a></span><span class="t"><span class="str">        """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t299" href="#t299">299</a></span><span class="t">        <span class="com">#</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t300" href="#t300">300</a></span><span class="t">        <span class="key">if</span> <span class="nam">cls</span><span class="op">.</span><span class="nam">__table</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t301" href="#t301">301</a></span><span class="t">            <span class="key">return</span> <span class="nam">cls</span><span class="op">.</span><span class="nam">__table</span><span class="op">[</span><span class="nam">col</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t302" href="#t302">302</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t303" href="#t303">303</a></span><span class="t">    <span class="key">def</span> <span class="nam">__new__</span><span class="op">(</span><span class="nam">cls</span><span class="op">,</span> <span class="op">*</span><span class="nam">a</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">,</span> <span class="op">**</span><span class="nam">kw</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">)</span> <span class="op">-></span> <span class="nam">Row</span><span class="op">:</span>  <span class="com"># or none!</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t304" href="#t304">304</a></span><span class="t">        <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t305" href="#t305">305</a></span><span class="t"><span class="str">        When e.g. Table(id=0) is called without db.define, \</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t306" href="#t306">306</a></span><span class="t"><span class="str">        this catches it and forwards for proper behavior.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t307" href="#t307">307</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t308" href="#t308">308</a></span><span class="t"><span class="str">        Args:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t309" href="#t309">309</a></span><span class="t"><span class="str">            *a: can be for example Table(&lt;id>)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t310" href="#t310">310</a></span><span class="t"><span class="str">            **kw: can be for example Table(slug=&lt;slug>)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t311" href="#t311">311</a></span><span class="t"><span class="str">        """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t312" href="#t312">312</a></span><span class="t">        <span class="key">if</span> <span class="key">not</span> <span class="nam">cls</span><span class="op">.</span><span class="nam">__table</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t313" href="#t313">313</a></span><span class="t">            <span class="key">raise</span> <span class="nam">EnvironmentError</span><span class="op">(</span><span class="str">"@define or db.define is not called on this class yet!"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t314" href="#t314">314</a></span><span class="t">        <span class="key">return</span> <span class="nam">cls</span><span class="op">.</span><span class="nam">__table</span><span class="op">(</span><span class="op">*</span><span class="nam">a</span><span class="op">,</span> <span class="op">**</span><span class="nam">kw</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t315" href="#t315">315</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t316" href="#t316">316</a></span><span class="t">    <span class="op">@</span><span class="nam">classmethod</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t317" href="#t317">317</a></span><span class="t">    <span class="key">def</span> <span class="nam">insert</span><span class="op">(</span><span class="nam">cls</span><span class="op">,</span> <span class="op">**</span><span class="nam">fields</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">)</span> <span class="op">-></span> <span class="nam">int</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t318" href="#t318">318</a></span><span class="t">        <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t319" href="#t319">319</a></span><span class="t"><span class="str">        This is only called when db.define is not used as a decorator.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t320" href="#t320">320</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t321" href="#t321">321</a></span><span class="t"><span class="str">        cls.__table functions as 'self'</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t322" href="#t322">322</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t323" href="#t323">323</a></span><span class="t"><span class="str">        Returns: the ID of the new row.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t324" href="#t324">324</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t325" href="#t325">325</a></span><span class="t"><span class="str">        """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t326" href="#t326">326</a></span><span class="t">        <span class="key">if</span> <span class="key">not</span> <span class="nam">cls</span><span class="op">.</span><span class="nam">__table</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t327" href="#t327">327</a></span><span class="t">            <span class="key">raise</span> <span class="nam">EnvironmentError</span><span class="op">(</span><span class="str">"@define or db.define is not called on this class yet!"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t328" href="#t328">328</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t329" href="#t329">329</a></span><span class="t">        <span class="nam">result</span> <span class="op">=</span> <span class="nam">super</span><span class="op">(</span><span class="op">)</span><span class="op">.</span><span class="nam">insert</span><span class="op">(</span><span class="nam">cls</span><span class="op">.</span><span class="nam">__table</span><span class="op">,</span> <span class="op">**</span><span class="nam">fields</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t330" href="#t330">330</a></span><span class="t">        <span class="com"># it already is an int but mypy doesn't understand that</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t331" href="#t331">331</a></span><span class="t">        <span class="key">return</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">cast</span><span class="op">(</span><span class="nam">int</span><span class="op">,</span> <span class="nam">result</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t332" href="#t332">332</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t333" href="#t333">333</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t334" href="#t334">334</a></span><span class="t"><span class="com"># backwards compat:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t335" href="#t335">335</a></span><span class="t"><span class="nam">TypedRow</span> <span class="op">=</span> <span class="nam">TypedTable</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t336" href="#t336">336</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t337" href="#t337">337</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t338" href="#t338">338</a></span><span class="t"><span class="key">class</span> <span class="nam">TypedFieldType</span><span class="op">(</span><span class="nam">Field</span><span class="op">)</span><span class="op">:</span>  <span class="com"># type: ignore</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t339" href="#t339">339</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t340" href="#t340">340</a></span><span class="t"><span class="str">    Typed version of pydal.Field, which will be converted to a normal Field in the background.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t341" href="#t341">341</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t342" href="#t342">342</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t343" href="#t343">343</a></span><span class="t">    <span class="com"># todo: .bind</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t344" href="#t344">344</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t345" href="#t345">345</a></span><span class="t">    <span class="com"># will be set by .bind on db.define</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t346" href="#t346">346</a></span><span class="t">    <span class="nam">name</span> <span class="op">=</span> <span class="str">""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t347" href="#t347">347</a></span><span class="t">    <span class="nam">_db</span> <span class="op">=</span> <span class="key">None</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t348" href="#t348">348</a></span><span class="t">    <span class="nam">_rname</span> <span class="op">=</span> <span class="key">None</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t349" href="#t349">349</a></span><span class="t">    <span class="nam">_table</span> <span class="op">=</span> <span class="key">None</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t323" href="#t323">323</a></span><span class="t"><span class="str">        Args:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t324" href="#t324">324</a></span><span class="t"><span class="str">            **fields: anything you want to insert in the database</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t325" href="#t325">325</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t326" href="#t326">326</a></span><span class="t"><span class="str">        Returns: the ID of the new row.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t327" href="#t327">327</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t328" href="#t328">328</a></span><span class="t"><span class="str">        """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t329" href="#t329">329</a></span><span class="t">        <span class="key">if</span> <span class="key">not</span> <span class="nam">cls</span><span class="op">.</span><span class="nam">__table</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t330" href="#t330">330</a></span><span class="t">            <span class="key">raise</span> <span class="nam">EnvironmentError</span><span class="op">(</span><span class="str">"@define or db.define is not called on this class yet!"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t331" href="#t331">331</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t332" href="#t332">332</a></span><span class="t">        <span class="nam">result</span> <span class="op">=</span> <span class="nam">super</span><span class="op">(</span><span class="op">)</span><span class="op">.</span><span class="nam">insert</span><span class="op">(</span><span class="nam">cls</span><span class="op">.</span><span class="nam">__table</span><span class="op">,</span> <span class="op">**</span><span class="nam">fields</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t333" href="#t333">333</a></span><span class="t">        <span class="com"># it already is an int but mypy doesn't understand that</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t334" href="#t334">334</a></span><span class="t">        <span class="key">return</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">cast</span><span class="op">(</span><span class="nam">int</span><span class="op">,</span> <span class="nam">result</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t335" href="#t335">335</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t336" href="#t336">336</a></span><span class="t">    <span class="op">@</span><span class="nam">classmethod</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t337" href="#t337">337</a></span><span class="t">    <span class="key">def</span> <span class="nam">update_or_insert</span><span class="op">(</span><span class="nam">cls</span><span class="op">,</span> <span class="nam">query</span><span class="op">:</span> <span class="nam">T_Query</span> <span class="op">=</span> <span class="nam">DEFAULT</span><span class="op">,</span> <span class="op">**</span><span class="nam">values</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">)</span> <span class="op">-></span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Optional</span><span class="op">[</span><span class="nam">int</span><span class="op">]</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t338" href="#t338">338</a></span><span class="t">        <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t339" href="#t339">339</a></span><span class="t"><span class="str">        Add typing to pydal's update_or_insert.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t340" href="#t340">340</a></span><span class="t"><span class="str">        """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t341" href="#t341">341</a></span><span class="t">        <span class="nam">result</span> <span class="op">=</span> <span class="nam">super</span><span class="op">(</span><span class="op">)</span><span class="op">.</span><span class="nam">update_or_insert</span><span class="op">(</span><span class="nam">cls</span><span class="op">,</span> <span class="nam">_key</span><span class="op">=</span><span class="nam">query</span><span class="op">,</span> <span class="op">**</span><span class="nam">values</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t342" href="#t342">342</a></span><span class="t">        <span class="key">if</span> <span class="nam">result</span> <span class="key">is</span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t343" href="#t343">343</a></span><span class="t">            <span class="key">return</span> <span class="key">None</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t344" href="#t344">344</a></span><span class="t">        <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t345" href="#t345">345</a></span><span class="t">            <span class="key">return</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">cast</span><span class="op">(</span><span class="nam">int</span><span class="op">,</span> <span class="nam">result</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t346" href="#t346">346</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t347" href="#t347">347</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t348" href="#t348">348</a></span><span class="t"><span class="com"># backwards compat:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t349" href="#t349">349</a></span><span class="t"><span class="nam">TypedRow</span> <span class="op">=</span> <span class="nam">TypedTable</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t350" href="#t350">350</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t351" href="#t351">351</a></span><span class="t">    <span class="nam">_type</span><span class="op">:</span> <span class="nam">T_annotation</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t352" href="#t352">352</a></span><span class="t">    <span class="nam">kwargs</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t353" href="#t353">353</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t354" href="#t354">354</a></span><span class="t">    <span class="key">def</span> <span class="nam">__init__</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">_type</span><span class="op">:</span> <span class="nam">T_annotation</span><span class="op">,</span> <span class="op">**</span><span class="nam">kwargs</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">)</span> <span class="op">-></span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t355" href="#t355">355</a></span><span class="t">        <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t356" href="#t356">356</a></span><span class="t"><span class="str">        A TypedFieldType should not be inited manually, but TypedField (from `fields.py`) should be used!</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t357" href="#t357">357</a></span><span class="t"><span class="str">        """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t358" href="#t358">358</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">_type</span> <span class="op">=</span> <span class="nam">_type</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t359" href="#t359">359</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">kwargs</span> <span class="op">=</span> <span class="nam">kwargs</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t360" href="#t360">360</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t361" href="#t361">361</a></span><span class="t">    <span class="key">def</span> <span class="nam">__str__</span><span class="op">(</span><span class="nam">self</span><span class="op">)</span> <span class="op">-></span> <span class="nam">str</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t362" href="#t362">362</a></span><span class="t">        <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t363" href="#t363">363</a></span><span class="t"><span class="str">        String representation of a Typed Field.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t351" href="#t351">351</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t352" href="#t352">352</a></span><span class="t"><span class="key">class</span> <span class="nam">TypedFieldType</span><span class="op">(</span><span class="nam">Field</span><span class="op">)</span><span class="op">:</span>  <span class="com"># type: ignore</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t353" href="#t353">353</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t354" href="#t354">354</a></span><span class="t"><span class="str">    Typed version of pydal.Field, which will be converted to a normal Field in the background.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t355" href="#t355">355</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t356" href="#t356">356</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t357" href="#t357">357</a></span><span class="t">    <span class="com"># todo: .bind</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t358" href="#t358">358</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t359" href="#t359">359</a></span><span class="t">    <span class="com"># will be set by .bind on db.define</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t360" href="#t360">360</a></span><span class="t">    <span class="nam">name</span> <span class="op">=</span> <span class="str">""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t361" href="#t361">361</a></span><span class="t">    <span class="nam">_db</span> <span class="op">=</span> <span class="key">None</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t362" href="#t362">362</a></span><span class="t">    <span class="nam">_rname</span> <span class="op">=</span> <span class="key">None</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t363" href="#t363">363</a></span><span class="t">    <span class="nam">_table</span> <span class="op">=</span> <span class="key">None</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t364" href="#t364">364</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t365" href="#t365">365</a></span><span class="t"><span class="str">        If `type` is set explicitly (e.g. TypedField(str, type="text")), that type is used: `TypedField.text`,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t366" href="#t366">366</a></span><span class="t"><span class="str">        otherwise the type annotation is used (e.g. TypedField(str) -> TypedField.str)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t367" href="#t367">367</a></span><span class="t"><span class="str">        """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t368" href="#t368">368</a></span><span class="t">        <span class="key">if</span> <span class="str">"type"</span> <span class="key">in</span> <span class="nam">self</span><span class="op">.</span><span class="nam">kwargs</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t369" href="#t369">369</a></span><span class="t">            <span class="com"># manual type in kwargs supplied</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t370" href="#t370">370</a></span><span class="t">            <span class="nam">t</span> <span class="op">=</span> <span class="nam">self</span><span class="op">.</span><span class="nam">kwargs</span><span class="op">[</span><span class="str">"type"</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t371" href="#t371">371</a></span><span class="t">        <span class="key">elif</span> <span class="nam">issubclass</span><span class="op">(</span><span class="nam">type</span><span class="op">,</span> <span class="nam">type</span><span class="op">(</span><span class="nam">self</span><span class="op">.</span><span class="nam">_type</span><span class="op">)</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t372" href="#t372">372</a></span><span class="t">            <span class="com"># normal type, str.__name__ = 'str'</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t373" href="#t373">373</a></span><span class="t">            <span class="nam">t</span> <span class="op">=</span> <span class="nam">getattr</span><span class="op">(</span><span class="nam">self</span><span class="op">.</span><span class="nam">_type</span><span class="op">,</span> <span class="str">"__name__"</span><span class="op">,</span> <span class="nam">str</span><span class="op">(</span><span class="nam">self</span><span class="op">.</span><span class="nam">_type</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t374" href="#t374">374</a></span><span class="t">        <span class="key">elif</span> <span class="nam">t_args</span> <span class="op">:=</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">get_args</span><span class="op">(</span><span class="nam">self</span><span class="op">.</span><span class="nam">_type</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t375" href="#t375">375</a></span><span class="t">            <span class="com"># list[str] -> 'str'</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t376" href="#t376">376</a></span><span class="t">            <span class="nam">t</span> <span class="op">=</span> <span class="nam">t_args</span><span class="op">[</span><span class="num">0</span><span class="op">]</span><span class="op">.</span><span class="nam">__name__</span>&nbsp;</span><span class="r"></span></p>
-    <p class="exc show_exc"><span class="n"><a id="t377" href="#t377">377</a></span><span class="t">        <span class="key">else</span><span class="op">:</span>  <span class="com"># pragma: no cover</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t378" href="#t378">378</a></span><span class="t">            <span class="com"># fallback - something else, may not even happen, I'm not sure</span>&nbsp;</span><span class="r"></span></p>
-    <p class="exc show_exc"><span class="n"><a id="t379" href="#t379">379</a></span><span class="t">            <span class="nam">t</span> <span class="op">=</span> <span class="nam">self</span><span class="op">.</span><span class="nam">_type</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t380" href="#t380">380</a></span><span class="t">        <span class="key">return</span> <span class="str">f"TypedField.{t}"</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t381" href="#t381">381</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t382" href="#t382">382</a></span><span class="t">    <span class="key">def</span> <span class="nam">__repr__</span><span class="op">(</span><span class="nam">self</span><span class="op">)</span> <span class="op">-></span> <span class="nam">str</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t383" href="#t383">383</a></span><span class="t">        <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t384" href="#t384">384</a></span><span class="t"><span class="str">        More detailed string representation of a Typed Field.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t385" href="#t385">385</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t386" href="#t386">386</a></span><span class="t"><span class="str">        Uses __str__ and adds the provided extra options (kwargs) in the representation.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t387" href="#t387">387</a></span><span class="t"><span class="str">        """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t388" href="#t388">388</a></span><span class="t">        <span class="nam">s</span> <span class="op">=</span> <span class="nam">self</span><span class="op">.</span><span class="nam">__str__</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t389" href="#t389">389</a></span><span class="t">        <span class="nam">kw</span> <span class="op">=</span> <span class="nam">self</span><span class="op">.</span><span class="nam">kwargs</span><span class="op">.</span><span class="nam">copy</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t390" href="#t390">390</a></span><span class="t">        <span class="nam">kw</span><span class="op">.</span><span class="nam">pop</span><span class="op">(</span><span class="str">"type"</span><span class="op">,</span> <span class="key">None</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t391" href="#t391">391</a></span><span class="t">        <span class="key">return</span> <span class="str">f"&lt;{s} with options {kw}>"</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t392" href="#t392">392</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t393" href="#t393">393</a></span><span class="t">    <span class="key">def</span> <span class="nam">_to_field</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">extra_kwargs</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">MutableMapping</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">]</span><span class="op">)</span> <span class="op">-></span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Optional</span><span class="op">[</span><span class="nam">str</span><span class="op">]</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t394" href="#t394">394</a></span><span class="t">        <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t395" href="#t395">395</a></span><span class="t"><span class="str">        Convert a Typed Field instance to a pydal.Field.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t396" href="#t396">396</a></span><span class="t"><span class="str">        """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t397" href="#t397">397</a></span><span class="t">        <span class="nam">other_kwargs</span> <span class="op">=</span> <span class="nam">self</span><span class="op">.</span><span class="nam">kwargs</span><span class="op">.</span><span class="nam">copy</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t398" href="#t398">398</a></span><span class="t">        <span class="nam">extra_kwargs</span><span class="op">.</span><span class="nam">update</span><span class="op">(</span><span class="nam">other_kwargs</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t399" href="#t399">399</a></span><span class="t">        <span class="key">return</span> <span class="nam">extra_kwargs</span><span class="op">.</span><span class="nam">pop</span><span class="op">(</span><span class="str">"type"</span><span class="op">,</span> <span class="key">False</span><span class="op">)</span> <span class="key">or</span> <span class="nam">TypeDAL</span><span class="op">.</span><span class="nam">_annotation_to_pydal_fieldtype</span><span class="op">(</span><span class="nam">self</span><span class="op">.</span><span class="nam">_type</span><span class="op">,</span> <span class="nam">extra_kwargs</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t400" href="#t400">400</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t401" href="#t401">401</a></span><span class="t">    <span class="key">def</span> <span class="nam">bind</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">field</span><span class="op">:</span> <span class="nam">Field</span><span class="op">,</span> <span class="nam">table</span><span class="op">:</span> <span class="nam">Table</span><span class="op">)</span> <span class="op">-></span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t402" href="#t402">402</a></span><span class="t">        <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t403" href="#t403">403</a></span><span class="t"><span class="str">        Bind the right db/table/field info to this class, so queries can be made using `Class.field == ...`.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t404" href="#t404">404</a></span><span class="t"><span class="str">        """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t405" href="#t405">405</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">name</span> <span class="op">=</span> <span class="nam">field</span><span class="op">.</span><span class="nam">name</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t406" href="#t406">406</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">type</span> <span class="op">=</span> <span class="nam">field</span><span class="op">.</span><span class="nam">type</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t407" href="#t407">407</a></span><span class="t">        <span class="nam">super</span><span class="op">(</span><span class="op">)</span><span class="op">.</span><span class="nam">bind</span><span class="op">(</span><span class="nam">table</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t408" href="#t408">408</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t409" href="#t409">409</a></span><span class="t">    <span class="com"># def __eq__(self, value):</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t410" href="#t410">410</a></span><span class="t">    <span class="com">#     return Query(self.db, self._dialect.eq, self, value)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t411" href="#t411">411</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t412" href="#t412">412</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t413" href="#t413">413</a></span><span class="t"><span class="nam">S</span> <span class="op">=</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">TypeVar</span><span class="op">(</span><span class="str">"S"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t365" href="#t365">365</a></span><span class="t">    <span class="nam">_type</span><span class="op">:</span> <span class="nam">T_annotation</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t366" href="#t366">366</a></span><span class="t">    <span class="nam">kwargs</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t367" href="#t367">367</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t368" href="#t368">368</a></span><span class="t">    <span class="key">def</span> <span class="nam">__init__</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">_type</span><span class="op">:</span> <span class="nam">T_annotation</span><span class="op">,</span> <span class="op">**</span><span class="nam">kwargs</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">)</span> <span class="op">-></span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t369" href="#t369">369</a></span><span class="t">        <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t370" href="#t370">370</a></span><span class="t"><span class="str">        A TypedFieldType should not be inited manually, but TypedField (from `fields.py`) should be used!</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t371" href="#t371">371</a></span><span class="t"><span class="str">        """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t372" href="#t372">372</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">_type</span> <span class="op">=</span> <span class="nam">_type</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t373" href="#t373">373</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">kwargs</span> <span class="op">=</span> <span class="nam">kwargs</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t374" href="#t374">374</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t375" href="#t375">375</a></span><span class="t">    <span class="key">def</span> <span class="nam">__str__</span><span class="op">(</span><span class="nam">self</span><span class="op">)</span> <span class="op">-></span> <span class="nam">str</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t376" href="#t376">376</a></span><span class="t">        <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t377" href="#t377">377</a></span><span class="t"><span class="str">        String representation of a Typed Field.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t378" href="#t378">378</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t379" href="#t379">379</a></span><span class="t"><span class="str">        If `type` is set explicitly (e.g. TypedField(str, type="text")), that type is used: `TypedField.text`,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t380" href="#t380">380</a></span><span class="t"><span class="str">        otherwise the type annotation is used (e.g. TypedField(str) -> TypedField.str)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t381" href="#t381">381</a></span><span class="t"><span class="str">        """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t382" href="#t382">382</a></span><span class="t">        <span class="key">if</span> <span class="str">"type"</span> <span class="key">in</span> <span class="nam">self</span><span class="op">.</span><span class="nam">kwargs</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t383" href="#t383">383</a></span><span class="t">            <span class="com"># manual type in kwargs supplied</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t384" href="#t384">384</a></span><span class="t">            <span class="nam">t</span> <span class="op">=</span> <span class="nam">self</span><span class="op">.</span><span class="nam">kwargs</span><span class="op">[</span><span class="str">"type"</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t385" href="#t385">385</a></span><span class="t">        <span class="key">elif</span> <span class="nam">issubclass</span><span class="op">(</span><span class="nam">type</span><span class="op">,</span> <span class="nam">type</span><span class="op">(</span><span class="nam">self</span><span class="op">.</span><span class="nam">_type</span><span class="op">)</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t386" href="#t386">386</a></span><span class="t">            <span class="com"># normal type, str.__name__ = 'str'</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t387" href="#t387">387</a></span><span class="t">            <span class="nam">t</span> <span class="op">=</span> <span class="nam">getattr</span><span class="op">(</span><span class="nam">self</span><span class="op">.</span><span class="nam">_type</span><span class="op">,</span> <span class="str">"__name__"</span><span class="op">,</span> <span class="nam">str</span><span class="op">(</span><span class="nam">self</span><span class="op">.</span><span class="nam">_type</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t388" href="#t388">388</a></span><span class="t">        <span class="key">elif</span> <span class="nam">t_args</span> <span class="op">:=</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">get_args</span><span class="op">(</span><span class="nam">self</span><span class="op">.</span><span class="nam">_type</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t389" href="#t389">389</a></span><span class="t">            <span class="com"># list[str] -> 'str'</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t390" href="#t390">390</a></span><span class="t">            <span class="nam">t</span> <span class="op">=</span> <span class="nam">t_args</span><span class="op">[</span><span class="num">0</span><span class="op">]</span><span class="op">.</span><span class="nam">__name__</span>&nbsp;</span><span class="r"></span></p>
+    <p class="exc show_exc"><span class="n"><a id="t391" href="#t391">391</a></span><span class="t">        <span class="key">else</span><span class="op">:</span>  <span class="com"># pragma: no cover</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t392" href="#t392">392</a></span><span class="t">            <span class="com"># fallback - something else, may not even happen, I'm not sure</span>&nbsp;</span><span class="r"></span></p>
+    <p class="exc show_exc"><span class="n"><a id="t393" href="#t393">393</a></span><span class="t">            <span class="nam">t</span> <span class="op">=</span> <span class="nam">self</span><span class="op">.</span><span class="nam">_type</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t394" href="#t394">394</a></span><span class="t">        <span class="key">return</span> <span class="str">f"TypedField.{t}"</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t395" href="#t395">395</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t396" href="#t396">396</a></span><span class="t">    <span class="key">def</span> <span class="nam">__repr__</span><span class="op">(</span><span class="nam">self</span><span class="op">)</span> <span class="op">-></span> <span class="nam">str</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t397" href="#t397">397</a></span><span class="t">        <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t398" href="#t398">398</a></span><span class="t"><span class="str">        More detailed string representation of a Typed Field.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t399" href="#t399">399</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t400" href="#t400">400</a></span><span class="t"><span class="str">        Uses __str__ and adds the provided extra options (kwargs) in the representation.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t401" href="#t401">401</a></span><span class="t"><span class="str">        """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t402" href="#t402">402</a></span><span class="t">        <span class="nam">s</span> <span class="op">=</span> <span class="nam">self</span><span class="op">.</span><span class="nam">__str__</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t403" href="#t403">403</a></span><span class="t">        <span class="nam">kw</span> <span class="op">=</span> <span class="nam">self</span><span class="op">.</span><span class="nam">kwargs</span><span class="op">.</span><span class="nam">copy</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t404" href="#t404">404</a></span><span class="t">        <span class="nam">kw</span><span class="op">.</span><span class="nam">pop</span><span class="op">(</span><span class="str">"type"</span><span class="op">,</span> <span class="key">None</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t405" href="#t405">405</a></span><span class="t">        <span class="key">return</span> <span class="str">f"&lt;{s} with options {kw}>"</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t406" href="#t406">406</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t407" href="#t407">407</a></span><span class="t">    <span class="key">def</span> <span class="nam">_to_field</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">extra_kwargs</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">MutableMapping</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">]</span><span class="op">)</span> <span class="op">-></span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Optional</span><span class="op">[</span><span class="nam">str</span><span class="op">]</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t408" href="#t408">408</a></span><span class="t">        <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t409" href="#t409">409</a></span><span class="t"><span class="str">        Convert a Typed Field instance to a pydal.Field.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t410" href="#t410">410</a></span><span class="t"><span class="str">        """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t411" href="#t411">411</a></span><span class="t">        <span class="nam">other_kwargs</span> <span class="op">=</span> <span class="nam">self</span><span class="op">.</span><span class="nam">kwargs</span><span class="op">.</span><span class="nam">copy</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t412" href="#t412">412</a></span><span class="t">        <span class="nam">extra_kwargs</span><span class="op">.</span><span class="nam">update</span><span class="op">(</span><span class="nam">other_kwargs</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t413" href="#t413">413</a></span><span class="t">        <span class="key">return</span> <span class="nam">extra_kwargs</span><span class="op">.</span><span class="nam">pop</span><span class="op">(</span><span class="str">"type"</span><span class="op">,</span> <span class="key">False</span><span class="op">)</span> <span class="key">or</span> <span class="nam">TypeDAL</span><span class="op">.</span><span class="nam">_annotation_to_pydal_fieldtype</span><span class="op">(</span><span class="nam">self</span><span class="op">.</span><span class="nam">_type</span><span class="op">,</span> <span class="nam">extra_kwargs</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t414" href="#t414">414</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t415" href="#t415">415</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t416" href="#t416">416</a></span><span class="t"><span class="key">class</span> <span class="nam">TypedRows</span><span class="op">(</span><span class="nam">typing</span><span class="op">.</span><span class="nam">Collection</span><span class="op">[</span><span class="nam">S</span><span class="op">]</span><span class="op">,</span> <span class="nam">Rows</span><span class="op">)</span><span class="op">:</span>  <span class="com"># type: ignore</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t417" href="#t417">417</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t418" href="#t418">418</a></span><span class="t"><span class="str">    Can be used as the return type of a .select().</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t419" href="#t419">419</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t420" href="#t420">420</a></span><span class="t"><span class="str">    Example:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t421" href="#t421">421</a></span><span class="t"><span class="str">        people: TypedRows[Person] = db(Person).select()</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t422" href="#t422">422</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t423" href="#t423">423</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t424" href="#t424">424</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t425" href="#t425">425</a></span><span class="t"><span class="nam">T_Table</span> <span class="op">=</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">TypeVar</span><span class="op">(</span><span class="str">"T_Table"</span><span class="op">,</span> <span class="nam">bound</span><span class="op">=</span><span class="nam">Table</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t415" href="#t415">415</a></span><span class="t">    <span class="key">def</span> <span class="nam">bind</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">field</span><span class="op">:</span> <span class="nam">Field</span><span class="op">,</span> <span class="nam">table</span><span class="op">:</span> <span class="nam">Table</span><span class="op">)</span> <span class="op">-></span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t416" href="#t416">416</a></span><span class="t">        <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t417" href="#t417">417</a></span><span class="t"><span class="str">        Bind the right db/table/field info to this class, so queries can be made using `Class.field == ...`.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t418" href="#t418">418</a></span><span class="t"><span class="str">        """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t419" href="#t419">419</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">name</span> <span class="op">=</span> <span class="nam">field</span><span class="op">.</span><span class="nam">name</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t420" href="#t420">420</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">type</span> <span class="op">=</span> <span class="nam">field</span><span class="op">.</span><span class="nam">type</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t421" href="#t421">421</a></span><span class="t">        <span class="nam">super</span><span class="op">(</span><span class="op">)</span><span class="op">.</span><span class="nam">bind</span><span class="op">(</span><span class="nam">table</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t422" href="#t422">422</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t423" href="#t423">423</a></span><span class="t">    <span class="com"># def __eq__(self, value):</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t424" href="#t424">424</a></span><span class="t">    <span class="com">#     return Query(self.db, self._dialect.eq, self, value)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t425" href="#t425">425</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t426" href="#t426">426</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t427" href="#t427">427</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="exc show_exc"><span class="n"><a id="t428" href="#t428">428</a></span><span class="t"><span class="key">class</span> <span class="nam">TypedSet</span><span class="op">(</span><span class="nam">pydal</span><span class="op">.</span><span class="nam">objects</span><span class="op">.</span><span class="nam">Set</span><span class="op">)</span><span class="op">:</span>  <span class="com"># type: ignore # pragma: no cover</span>&nbsp;</span><span class="r"></span></p>
-    <p class="exc show_exc"><span class="n"><a id="t429" href="#t429">429</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t430" href="#t430">430</a></span><span class="t"><span class="str">    Used to make pydal Set more typed.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t431" href="#t431">431</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t432" href="#t432">432</a></span><span class="t"><span class="str">    This class is not actually used, only 'cast' by TypeDAL.__call__</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t433" href="#t433">433</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t434" href="#t434">434</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="exc show_exc"><span class="n"><a id="t435" href="#t435">435</a></span><span class="t">    <span class="key">def</span> <span class="nam">count</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">distinct</span><span class="op">:</span> <span class="nam">bool</span> <span class="op">=</span> <span class="key">None</span><span class="op">,</span> <span class="nam">cache</span><span class="op">:</span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">]</span> <span class="op">=</span> <span class="key">None</span><span class="op">)</span> <span class="op">-></span> <span class="nam">int</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="exc show_exc"><span class="n"><a id="t436" href="#t436">436</a></span><span class="t">        <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t437" href="#t437">437</a></span><span class="t"><span class="str">        Count returns an int.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t438" href="#t438">438</a></span><span class="t"><span class="str">        """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="exc show_exc"><span class="n"><a id="t439" href="#t439">439</a></span><span class="t">        <span class="nam">result</span> <span class="op">=</span> <span class="nam">super</span><span class="op">(</span><span class="op">)</span><span class="op">.</span><span class="nam">count</span><span class="op">(</span><span class="nam">distinct</span><span class="op">,</span> <span class="nam">cache</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="exc show_exc"><span class="n"><a id="t440" href="#t440">440</a></span><span class="t">        <span class="key">return</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">cast</span><span class="op">(</span><span class="nam">int</span><span class="op">,</span> <span class="nam">result</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t427" href="#t427">427</a></span><span class="t"><span class="nam">S</span> <span class="op">=</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">TypeVar</span><span class="op">(</span><span class="str">"S"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t428" href="#t428">428</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t429" href="#t429">429</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t430" href="#t430">430</a></span><span class="t"><span class="key">class</span> <span class="nam">TypedRows</span><span class="op">(</span><span class="nam">typing</span><span class="op">.</span><span class="nam">Collection</span><span class="op">[</span><span class="nam">S</span><span class="op">]</span><span class="op">,</span> <span class="nam">Rows</span><span class="op">)</span><span class="op">:</span>  <span class="com"># type: ignore</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t431" href="#t431">431</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t432" href="#t432">432</a></span><span class="t"><span class="str">    Can be used as the return type of a .select().</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t433" href="#t433">433</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t434" href="#t434">434</a></span><span class="t"><span class="str">    Example:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t435" href="#t435">435</a></span><span class="t"><span class="str">        people: TypedRows[Person] = db(Person).select()</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t436" href="#t436">436</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t437" href="#t437">437</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t438" href="#t438">438</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t439" href="#t439">439</a></span><span class="t"><span class="nam">T_Table</span> <span class="op">=</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">TypeVar</span><span class="op">(</span><span class="str">"T_Table"</span><span class="op">,</span> <span class="nam">bound</span><span class="op">=</span><span class="nam">Table</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t440" href="#t440">440</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t441" href="#t441">441</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="exc show_exc"><span class="n"><a id="t442" href="#t442">442</a></span><span class="t">    <span class="key">def</span> <span class="nam">select</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="op">*</span><span class="nam">fields</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">,</span> <span class="op">**</span><span class="nam">attributes</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">)</span> <span class="op">-></span> <span class="nam">TypedRows</span><span class="op">[</span><span class="nam">T_Table</span><span class="op">]</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="exc show_exc"><span class="n"><a id="t443" href="#t443">443</a></span><span class="t">        <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t444" href="#t444">444</a></span><span class="t"><span class="str">        Select returns a TypedRows of a user defined table.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="exc show_exc"><span class="n"><a id="t442" href="#t442">442</a></span><span class="t"><span class="key">class</span> <span class="nam">TypedSet</span><span class="op">(</span><span class="nam">pydal</span><span class="op">.</span><span class="nam">objects</span><span class="op">.</span><span class="nam">Set</span><span class="op">)</span><span class="op">:</span>  <span class="com"># type: ignore # pragma: no cover</span>&nbsp;</span><span class="r"></span></p>
+    <p class="exc show_exc"><span class="n"><a id="t443" href="#t443">443</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t444" href="#t444">444</a></span><span class="t"><span class="str">    Used to make pydal Set more typed.</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t445" href="#t445">445</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t446" href="#t446">446</a></span><span class="t"><span class="str">        Example:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t447" href="#t447">447</a></span><span class="t"><span class="str">            result: TypedRows[MyTable] = db(MyTable.id > 0).select()</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t446" href="#t446">446</a></span><span class="t"><span class="str">    This class is not actually used, only 'cast' by TypeDAL.__call__</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t447" href="#t447">447</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t448" href="#t448">448</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t449" href="#t449">449</a></span><span class="t"><span class="str">            for row in result:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t450" href="#t450">450</a></span><span class="t"><span class="str">                typing.reveal_type(row)  # MyTable</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t451" href="#t451">451</a></span><span class="t"><span class="str">        """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="exc show_exc"><span class="n"><a id="t452" href="#t452">452</a></span><span class="t">        <span class="nam">rows</span> <span class="op">=</span> <span class="nam">super</span><span class="op">(</span><span class="op">)</span><span class="op">.</span><span class="nam">select</span><span class="op">(</span><span class="op">*</span><span class="nam">fields</span><span class="op">,</span> <span class="op">**</span><span class="nam">attributes</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="exc show_exc"><span class="n"><a id="t453" href="#t453">453</a></span><span class="t">        <span class="key">return</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">cast</span><span class="op">(</span><span class="nam">TypedRows</span><span class="op">[</span><span class="nam">T_Table</span><span class="op">]</span><span class="op">,</span> <span class="nam">rows</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="exc show_exc"><span class="n"><a id="t449" href="#t449">449</a></span><span class="t">    <span class="key">def</span> <span class="nam">count</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">distinct</span><span class="op">:</span> <span class="nam">bool</span> <span class="op">=</span> <span class="key">None</span><span class="op">,</span> <span class="nam">cache</span><span class="op">:</span> <span class="nam">dict</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">]</span> <span class="op">=</span> <span class="key">None</span><span class="op">)</span> <span class="op">-></span> <span class="nam">int</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="exc show_exc"><span class="n"><a id="t450" href="#t450">450</a></span><span class="t">        <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t451" href="#t451">451</a></span><span class="t"><span class="str">        Count returns an int.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t452" href="#t452">452</a></span><span class="t"><span class="str">        """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="exc show_exc"><span class="n"><a id="t453" href="#t453">453</a></span><span class="t">        <span class="nam">result</span> <span class="op">=</span> <span class="nam">super</span><span class="op">(</span><span class="op">)</span><span class="op">.</span><span class="nam">count</span><span class="op">(</span><span class="nam">distinct</span><span class="op">,</span> <span class="nam">cache</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="exc show_exc"><span class="n"><a id="t454" href="#t454">454</a></span><span class="t">        <span class="key">return</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">cast</span><span class="op">(</span><span class="nam">int</span><span class="op">,</span> <span class="nam">result</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t455" href="#t455">455</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="exc show_exc"><span class="n"><a id="t456" href="#t456">456</a></span><span class="t">    <span class="key">def</span> <span class="nam">select</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="op">*</span><span class="nam">fields</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">,</span> <span class="op">**</span><span class="nam">attributes</span><span class="op">:</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">Any</span><span class="op">)</span> <span class="op">-></span> <span class="nam">TypedRows</span><span class="op">[</span><span class="nam">T_Table</span><span class="op">]</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="exc show_exc"><span class="n"><a id="t457" href="#t457">457</a></span><span class="t">        <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t458" href="#t458">458</a></span><span class="t"><span class="str">        Select returns a TypedRows of a user defined table.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t459" href="#t459">459</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t460" href="#t460">460</a></span><span class="t"><span class="str">        Example:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t461" href="#t461">461</a></span><span class="t"><span class="str">            result: TypedRows[MyTable] = db(MyTable.id > 0).select()</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t462" href="#t462">462</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t463" href="#t463">463</a></span><span class="t"><span class="str">            for row in result:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t464" href="#t464">464</a></span><span class="t"><span class="str">                typing.reveal_type(row)  # MyTable</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t465" href="#t465">465</a></span><span class="t"><span class="str">        """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="exc show_exc"><span class="n"><a id="t466" href="#t466">466</a></span><span class="t">        <span class="nam">rows</span> <span class="op">=</span> <span class="nam">super</span><span class="op">(</span><span class="op">)</span><span class="op">.</span><span class="nam">select</span><span class="op">(</span><span class="op">*</span><span class="nam">fields</span><span class="op">,</span> <span class="op">**</span><span class="nam">attributes</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="exc show_exc"><span class="n"><a id="t467" href="#t467">467</a></span><span class="t">        <span class="key">return</span> <span class="nam">typing</span><span class="op">.</span><span class="nam">cast</span><span class="op">(</span><span class="nam">TypedRows</span><span class="op">[</span><span class="nam">T_Table</span><span class="op">]</span><span class="op">,</span> <span class="nam">rows</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
 </main>
 <footer>
     <div class="content">
         <p>
             <a id="prevFileLink" class="nav" href="d_0ccc93afd6526b6c___init___py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_0ccc93afd6526b6c_fields_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-06-27 17:50 +0200
+            created at 2023-06-27 18:15 +0200
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -5,506 +5,522 @@
 r m x   toggle line displays
 j k   next/prev highlighted chunk
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
-***** 144 statements   144 run 0 missing 12 excluded *****
+***** 153 statements   153 run 0 missing 12 excluded *****
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.7, created
-at 2023-06-27 17:50 +0200
+at 2023-06-27 18:15 +0200
 
 
 1""" 
 2Core functionality of TypeDAL. 
 3""" 
 4import datetime as dt 
 5import types 
 6import typing 
 7from collections import ChainMap 
 8from decimal import Decimal 
 9 
 10import pydal 
-11from pydal.objects import Field, Row, Rows, Table 
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
-29 
-30class _Types: 
-31 """ 
-32 Internal type storage for stuff that mypy otherwise won't understand. 
+11from pydal._globals import DEFAULT 
+12from pydal.objects import Field, Query, Row, Rows, Table 
+13 
+14# use typing.cast(type, ...) to make mypy happy with unions 
+15T_annotation = typing.Type[typing.Any] | types.UnionType 
+16T_Query = typing.Union["Table", "Query", "bool", "None", "TypedTable",
+typing.Type["TypedTable"]] 
+17 
+18BASIC_MAPPINGS: dict[T_annotation, str] = { 
+19 str: "string", 
+20 int: "integer", 
+21 bool: "boolean", 
+22 bytes: "blob", 
+23 float: "double", 
+24 object: "json", 
+25 Decimal: "decimal(10,2)", 
+26 dt.date: "date", 
+27 dt.time: "time", 
+28 dt.datetime: "datetime", 
+29} 
+30 
+31 
+32class _Types: 
 33 """ 
-34 
-35 NONETYPE = type(None) 
+34 Internal type storage for stuff that mypy otherwise won't understand. 
+35 """ 
 36 
-37 
-38# the input and output of TypeDAL.define 
-39T = typing.TypeVar("T", typing.Type["TypedTable"], typing.Type["Table"]) 
-40 
-41 
-42def is_union(some_type: type) -> bool: 
-43 """ 
-44 Check if a type is some type of Union. 
-45 
-46 Args: 
-47 some_type: types.UnionType = type(int | str); typing.Union = typing.Union
+37 NONETYPE = type(None) 
+38 
+39 
+40# the input and output of TypeDAL.define 
+41T = typing.TypeVar("T", typing.Type["TypedTable"], typing.Type["Table"]) 
+42 
+43 
+44def is_union(some_type: type) -> bool: 
+45 """ 
+46 Check if a type is some type of Union. 
+47 
+48 Args: 
+49 some_type: types.UnionType = type(int | str); typing.Union = typing.Union
 [int, str] 
-48 
-49 """ 
-50 return typing.get_origin(some_type) in (types.UnionType, typing.Union) 
-51 
-52 
-53def _all_annotations(cls: type) -> ChainMap[str, type]: 
-54 """ 
-55 Returns a dictionary-like ChainMap that includes annotations for all \ 
-56 attributes defined in cls or inherited from superclasses. 
-57 """ 
-58 return ChainMap(*(c.__annotations__ for c in getattr(cls, "__mro__", []) if
+50 
+51 """ 
+52 return typing.get_origin(some_type) in (types.UnionType, typing.Union) 
+53 
+54 
+55def _all_annotations(cls: type) -> ChainMap[str, type]: 
+56 """ 
+57 Returns a dictionary-like ChainMap that includes annotations for all \ 
+58 attributes defined in cls or inherited from superclasses. 
+59 """ 
+60 return ChainMap(*(c.__annotations__ for c in getattr(cls, "__mro__", []) if
 "__annotations__" in c.__dict__)) 
-59 
-60 
-61def all_annotations(cls: type, _except: typing.Iterable[str] = None) -> dict
+61 
+62 
+63def all_annotations(cls: type, _except: typing.Iterable[str] = None) -> dict
 [str, type]: 
-62 """ 
-63 Wrapper around `_all_annotations` that filters away any keys in _except. 
-64 
-65 It also flattens the ChainMap to a regular dict. 
-66 """ 
-67 if _except is None: 
-68 _except = set() 
-69 
-70 _all = _all_annotations(cls) 
-71 return {k: v for k, v in _all.items() if k not in _except} 
-72 
-73 
-74class TypeDAL(pydal.DAL): # type: ignore 
-75 """ 
-76 Drop-in replacement for pyDAL with layer to convert class-based table
-definitions to classical pydal define_tables. 
+64 """ 
+65 Wrapper around `_all_annotations` that filters away any keys in _except. 
+66 
+67 It also flattens the ChainMap to a regular dict. 
+68 """ 
+69 if _except is None: 
+70 _except = set() 
+71 
+72 _all = _all_annotations(cls) 
+73 return {k: v for k, v in _all.items() if k not in _except} 
+74 
+75 
+76class TypeDAL(pydal.DAL): # type: ignore 
 77 """ 
-78 
-79 dal: Table 
+78 Drop-in replacement for pyDAL with layer to convert class-based table
+definitions to classical pydal define_tables. 
+79 """ 
 80 
-81 default_kwargs: typing.ClassVar[typing.Dict[str, typing.Any]] = { 
-82 # fields are 'required' (notnull) by default: 
-83 "notnull": True, 
-84 } 
-85 
-86 def define(self, cls: T) -> T: 
-87 """ 
-88 Can be used as a decorator on a class that inherits `TypedTable`, \ 
-89 or as a regular method if you need to define your classes before you have
+81 dal: Table 
+82 
+83 default_kwargs: typing.ClassVar[typing.Dict[str, typing.Any]] = { 
+84 # fields are 'required' (notnull) by default: 
+85 "notnull": True, 
+86 } 
+87 
+88 def define(self, cls: T) -> T: 
+89 """ 
+90 Can be used as a decorator on a class that inherits `TypedTable`, \ 
+91 or as a regular method if you need to define your classes before you have
 access to a 'db' instance. 
-90 
-91 Args: 
-92 cls: 
-93 
-94 Example: 
-95 @db.define 
-96 class Person(TypedTable): 
-97 ... 
-98 
-99 class Article(TypedTable): 
-100 ... 
-101 
-102 # at a later time: 
-103 db.define(Article) 
-104 
-105 Returns: 
-106 the result of pydal.define_table 
-107 """ 
-108 # when __future__.annotations is implemented, cls.__annotations__ will not
+92 
+93 Args: 
+94 cls: 
+95 
+96 Example: 
+97 @db.define 
+98 class Person(TypedTable): 
+99 ... 
+100 
+101 class Article(TypedTable): 
+102 ... 
+103 
+104 # at a later time: 
+105 db.define(Article) 
+106 
+107 Returns: 
+108 the result of pydal.define_table 
+109 """ 
+110 # when __future__.annotations is implemented, cls.__annotations__ will not
 work anymore as below. 
-109 # proper way to handle this would be (but gives error right now due to
+111 # proper way to handle this would be (but gives error right now due to
 Table implementing magic methods): 
-110 # typing.get_type_hints(cls, globalns=None, localns=None) 
-111 
-112 # dirty way (with evil eval): 
-113 # [eval(v) for k, v in cls.__annotations__.items()] 
-114 # this however also stops working when variables outside this scope or even
+112 # typing.get_type_hints(cls, globalns=None, localns=None) 
+113 
+114 # dirty way (with evil eval): 
+115 # [eval(v) for k, v in cls.__annotations__.items()] 
+116 # this however also stops working when variables outside this scope or even
 references to other 
-115 # objects are used. So for now, this package will NOT work when from
+117 # objects are used. So for now, this package will NOT work when from
 __future__ import annotations is used, 
-116 # and might break in the future, when this annotations behavior is enabled
+118 # and might break in the future, when this annotations behavior is enabled
 by default. 
-117 
-118 # non-annotated variables have to be passed to define_table as kwargs 
 119 
-120 tablename = self._to_snake(cls.__name__) 
-121 # grab annotations of cls and it's parents: 
-122 annotations = all_annotations(cls) 
-123 # extend with `prop = TypedField()` 'annotations': 
-124 annotations |= {k: v for k, v in cls.__dict__.items() if isinstance(v,
+120 # non-annotated variables have to be passed to define_table as kwargs 
+121 
+122 tablename = self._to_snake(cls.__name__) 
+123 # grab annotations of cls and it's parents: 
+124 annotations = all_annotations(cls) 
+125 # extend with `prop = TypedField()` 'annotations': 
+126 annotations |= {k: v for k, v in cls.__dict__.items() if isinstance(v,
 TypedFieldType)} 
-125 # remove internal stuff: 
-126 annotations = {k: v for k, v in annotations.items() if not k.startswith
+127 # remove internal stuff: 
+128 annotations = {k: v for k, v in annotations.items() if not k.startswith
 ("_")} 
-127 
-128 typedfields = {k: v for k, v in annotations.items() if isinstance(v,
-TypedFieldType)} 
 129 
-130 fields = {fname: self._to_field(fname, ftype) for fname, ftype in
+130 typedfields = {k: v for k, v in annotations.items() if isinstance(v,
+TypedFieldType)} 
+131 
+132 fields = {fname: self._to_field(fname, ftype) for fname, ftype in
 annotations.items()} 
-131 other_kwargs = {k: v for k, v in cls.__dict__.items() if k not in
+133 other_kwargs = {k: v for k, v in cls.__dict__.items() if k not in
 annotations and not k.startswith("_")} 
-132 
-133 table: Table = self.define_table(tablename, *fields.values(),
-**other_kwargs) 
 134 
-135 for name, typed_field in typedfields.items(): 
-136 field = fields[name] 
-137 typed_field.bind(field, table) 
-138 
-139 cls.__set_internals__(db=self, table=table) 
+135 table: Table = self.define_table(tablename, *fields.values(),
+**other_kwargs) 
+136 
+137 for name, typed_field in typedfields.items(): 
+138 field = fields[name] 
+139 typed_field.bind(field, table) 
 140 
-141 # the ACTUAL output is not TypedTable but rather pydal.Table 
-142 # but telling the editor it is T helps with hinting. 
-143 return cls 
-144 
-145 def __call__(self, *_args: typing.Any, **kwargs: typing.Any) -> "TypedSet":
- 
-146 """ 
-147 A db instance can be called directly to perform a query. 
-148 
-149 Usually, only a query is passed. 
+141 cls.__set_internals__(db=self, table=table) 
+142 
+143 # the ACTUAL output is not TypedTable but rather pydal.Table 
+144 # but telling the editor it is T helps with hinting. 
+145 return cls 
+146 
+147 def __call__(self, *_args: T_Query, **kwargs: typing.Any) -> "TypedSet": 
+148 """ 
+149 A db instance can be called directly to perform a query. 
 150 
-151 Example: 
-152 db(query).select() 
-153 
-154 """ 
-155 args = list(_args) 
-156 if args: 
-157 cls = args[0] 
-158 if isinstance(cls, bool): 
-159 raise ValueError("Don't actually pass a bool to db()! Use a query
+151 Usually, only a query is passed. 
+152 
+153 Example: 
+154 db(query).select() 
+155 
+156 """ 
+157 args = list(_args) 
+158 if args: 
+159 cls = args[0] 
+160 if isinstance(cls, bool): 
+161 raise ValueError("Don't actually pass a bool to db()! Use a query
 instead.") 
-160 
-161 if issubclass(type(cls), type) and issubclass(cls, TypedTable): 
-162 # table defined without @db.define decorator! 
-163 args[0] = cls.id != None 
-164 
-165 _set = super().__call__(*args, **kwargs) 
-166 return typing.cast(TypedSet, _set) 
+162 
+163 if isinstance(cls, type) and issubclass(type(cls), type) and issubclass
+(cls, TypedTable): 
+164 # table defined without @db.define decorator! 
+165 _cls: typing.Type[TypedTable] = cls 
+166 args[0] = _cls.id != None 
 167 
-168 # todo: insert etc shadowen? 
-169 
-170 @classmethod 
-171 def _build_field(cls, name: str, _type: str, **kw: typing.Any) -> Field: 
-172 return Field(name, _type, **{**cls.default_kwargs, **kw}) 
-173 
-174 @classmethod 
-175 def _annotation_to_pydal_fieldtype( 
-176 cls, _ftype: T_annotation, mut_kw: typing.MutableMapping[str, typing.Any] 
-177 ) -> typing.Optional[str]: 
-178 # ftype can be a union or type. typing.cast is sometimes used to tell mypy
+168 _set = super().__call__(*args, **kwargs) 
+169 return typing.cast(TypedSet, _set) 
+170 
+171 # todo: insert etc shadowen? 
+172 
+173 @classmethod 
+174 def _build_field(cls, name: str, _type: str, **kw: typing.Any) -> Field: 
+175 return Field(name, _type, **{**cls.default_kwargs, **kw}) 
+176 
+177 @classmethod 
+178 def _annotation_to_pydal_fieldtype( 
+179 cls, _ftype: T_annotation, mut_kw: typing.MutableMapping[str, typing.Any] 
+180 ) -> typing.Optional[str]: 
+181 # ftype can be a union or type. typing.cast is sometimes used to tell mypy
 when it's not a union. 
-179 ftype = typing.cast(type, _ftype) # cast from typing.Type to type to make
+182 ftype = typing.cast(type, _ftype) # cast from typing.Type to type to make
 mypy happy) 
-180 
-181 if mapping := BASIC_MAPPINGS.get(ftype): 
-182 # basi types 
-183 return mapping 
-184 elif isinstance(ftype, Table): 
-185 # db.table 
-186 return f"reference {ftype._tablename}" 
-187 elif issubclass(type(ftype), type) and issubclass(ftype, TypedTable): 
-188 # SomeTable 
-189 snakename = cls._to_snake(ftype.__name__) 
-190 return f"reference {snakename}" 
-191 elif isinstance(ftype, TypedFieldType): 
-192 # FieldType(type, ...) 
-193 return ftype._to_field(mut_kw) 
-194 elif isinstance(ftype, types.GenericAlias) and typing.get_origin(ftype) is
+183 
+184 if mapping := BASIC_MAPPINGS.get(ftype): 
+185 # basi types 
+186 return mapping 
+187 elif isinstance(ftype, Table): 
+188 # db.table 
+189 return f"reference {ftype._tablename}" 
+190 elif issubclass(type(ftype), type) and issubclass(ftype, TypedTable): 
+191 # SomeTable 
+192 snakename = cls._to_snake(ftype.__name__) 
+193 return f"reference {snakename}" 
+194 elif isinstance(ftype, TypedFieldType): 
+195 # FieldType(type, ...) 
+196 return ftype._to_field(mut_kw) 
+197 elif isinstance(ftype, types.GenericAlias) and typing.get_origin(ftype) is
 list: 
-195 # list[str] -> str -> string -> list:string 
-196 _child_type = typing.get_args(ftype)[0] 
-197 _child_type = cls._annotation_to_pydal_fieldtype(_child_type, mut_kw) 
-198 return f"list:{_child_type}" 
-199 elif is_union(ftype): 
-200 # str | int -> UnionType 
-201 # typing.Union[str | int] -> typing._UnionGenericAlias 
-202 
-203 # typing.Optional[type] == type | None 
-204 
-205 match typing.get_args(ftype): 
-206 case (_child_type, _Types.NONETYPE): 
-207 # good union of Nullable 
-208 
-209 # if a field is optional, it is nullable: 
-210 mut_kw["notnull"] = False 
-211 return cls._annotation_to_pydal_fieldtype(_child_type, mut_kw) 
-212 case _: 
-213 # two types is not supported by the db! 
-214 return None 
-215 else: 
-216 return None 
-217 
-218 @classmethod 
-219 def _to_field(cls, fname: str, ftype: type, **kw: typing.Any) -> Field: 
-220 """ 
-221 Convert a annotation into a pydal Field. 
-222 
-223 Args: 
-224 fname: name of the property 
-225 ftype: annotation of the property 
-226 kw: when using TypedField or a function returning it (e.g. StringField), 
-227 keyword args can be used to pass any other settings you would normally to a
+198 # list[str] -> str -> string -> list:string 
+199 _child_type = typing.get_args(ftype)[0] 
+200 _child_type = cls._annotation_to_pydal_fieldtype(_child_type, mut_kw) 
+201 return f"list:{_child_type}" 
+202 elif is_union(ftype): 
+203 # str | int -> UnionType 
+204 # typing.Union[str | int] -> typing._UnionGenericAlias 
+205 
+206 # typing.Optional[type] == type | None 
+207 
+208 match typing.get_args(ftype): 
+209 case (_child_type, _Types.NONETYPE): 
+210 # good union of Nullable 
+211 
+212 # if a field is optional, it is nullable: 
+213 mut_kw["notnull"] = False 
+214 return cls._annotation_to_pydal_fieldtype(_child_type, mut_kw) 
+215 case _: 
+216 # two types is not supported by the db! 
+217 return None 
+218 else: 
+219 return None 
+220 
+221 @classmethod 
+222 def _to_field(cls, fname: str, ftype: type, **kw: typing.Any) -> Field: 
+223 """ 
+224 Convert a annotation into a pydal Field. 
+225 
+226 Args: 
+227 fname: name of the property 
+228 ftype: annotation of the property 
+229 kw: when using TypedField or a function returning it (e.g. StringField), 
+230 keyword args can be used to pass any other settings you would normally to a
 pydal Field 
-228 
-229 -> pydal.Field(fname, ftype, **kw) 
-230 
-231 Example: 
-232 class MyTable: 
-233 fname: ftype 
-234 id: int 
-235 name: str 
-236 reference: Table 
-237 other: TypedField(str, default="John Doe") # default will be in kwargs 
-238 """ 
-239 fname = cls._to_snake(fname) 
-240 
-241 if converted_type := cls._annotation_to_pydal_fieldtype(ftype, kw): 
-242 return cls._build_field(fname, converted_type, **kw) 
-243 else: 
-244 raise NotImplementedError(f"Unsupported type {ftype}/{type(ftype)}") 
-245 
-246 @staticmethod 
-247 def _to_snake(camel: str) -> str: 
-248 # https://stackoverflow.com/a/44969381 
-249 return "".join([f"_{c.lower()}" if c.isupper() else c for c in
+231 
+232 -> pydal.Field(fname, ftype, **kw) 
+233 
+234 Example: 
+235 class MyTable: 
+236 fname: ftype 
+237 id: int 
+238 name: str 
+239 reference: Table 
+240 other: TypedField(str, default="John Doe") # default will be in kwargs 
+241 """ 
+242 fname = cls._to_snake(fname) 
+243 
+244 if converted_type := cls._annotation_to_pydal_fieldtype(ftype, kw): 
+245 return cls._build_field(fname, converted_type, **kw) 
+246 else: 
+247 raise NotImplementedError(f"Unsupported type {ftype}/{type(ftype)}") 
+248 
+249 @staticmethod 
+250 def _to_snake(camel: str) -> str: 
+251 # https://stackoverflow.com/a/44969381 
+252 return "".join([f"_{c.lower()}" if c.isupper() else c for c in
 camel]).lstrip("_") 
-250 
-251 
-252class TypedTableMeta(type): 
-253 """ 
-254 Meta class allows getattribute on class variables instead instance
+253 
+254 
+255class TypedTableMeta(type): 
+256 """ 
+257 Meta class allows getattribute on class variables instead instance
 variables. 
-255 
-256 Used in `class TypedTable(Table, metaclass=TypedTableMeta)` 
-257 """ 
 258 
-259 def __getattr__(self, key: str) -> Field: 
+259 Used in `class TypedTable(Table, metaclass=TypedTableMeta)` 
 260 """ 
-261 The getattr method is only called when getattribute can't find something. 
-262 
-263 `__get_table_column__` is defined in `TypedTable` 
-264 """ 
-265 return self.__get_table_column__(key) 
-266 
-267 
-268class TypedTable(Table, metaclass=TypedTableMeta): # type: ignore 
-269 """ 
-270 Typed version of pydal.Table, does not really do anything itself but
+261 
+262 def __getattr__(self, key: str) -> Field: 
+263 """ 
+264 The getattr method is only called when getattribute can't find something. 
+265 
+266 `__get_table_column__` is defined in `TypedTable` 
+267 """ 
+268 return self.__get_table_column__(key) 
+269 
+270 
+271class TypedTable(Table, metaclass=TypedTableMeta): # type: ignore 
+272 """ 
+273 Typed version of pydal.Table, does not really do anything itself but
 forwards logic to pydal. 
-271 """ 
-272 
-273 id: int # noqa: 'id' has to be id since that's the db column 
-274 
-275 # set up by db.define: 
-276 __db: TypeDAL | None = None 
-277 __table: Table | None = None 
-278 
-279 @classmethod 
-280 def __set_internals__(cls, db: pydal.DAL, table: Table) -> None: 
-281 """ 
-282 Store the related database and pydal table for later usage. 
-283 """ 
-284 cls.__db = db 
-285 cls.__table = table 
-286 
-287 @classmethod 
-288 def __get_table_column__(cls, col: str) -> Field: 
-289 """ 
-290 Magic method used by TypedTableMeta to get a database field with dot
+274 """ 
+275 
+276 id: int # noqa: 'id' has to be id since that's the db column 
+277 
+278 # set up by db.define: 
+279 __db: TypeDAL | None = None 
+280 __table: Table | None = None 
+281 
+282 @classmethod 
+283 def __set_internals__(cls, db: pydal.DAL, table: Table) -> None: 
+284 """ 
+285 Store the related database and pydal table for later usage. 
+286 """ 
+287 cls.__db = db 
+288 cls.__table = table 
+289 
+290 @classmethod 
+291 def __get_table_column__(cls, col: str) -> Field: 
+292 """ 
+293 Magic method used by TypedTableMeta to get a database field with dot
 notation on a class. 
-291 
-292 Example: 
-293 SomeTypedTable.col -> db.table.col (via TypedTableMeta.__getattr__) 
 294 
-295 """ 
-296 # 
-297 if cls.__table: 
-298 return cls.__table[col] 
-299 
-300 def __new__(cls, *a: typing.Any, **kw: typing.Any) -> Row: # or none! 
-301 """ 
-302 When e.g. Table(id=0) is called without db.define, \ 
-303 this catches it and forwards for proper behavior. 
-304 
-305 Args: 
-306 *a: can be for example Table(<id>) 
-307 **kw: can be for example Table(slug=<slug>) 
-308 """ 
-309 if not cls.__table: 
-310 raise EnvironmentError("@define or db.define is not called on this class
+295 Example: 
+296 SomeTypedTable.col -> db.table.col (via TypedTableMeta.__getattr__) 
+297 
+298 """ 
+299 # 
+300 if cls.__table: 
+301 return cls.__table[col] 
+302 
+303 def __new__(cls, *a: typing.Any, **kw: typing.Any) -> Row: # or none! 
+304 """ 
+305 When e.g. Table(id=0) is called without db.define, \ 
+306 this catches it and forwards for proper behavior. 
+307 
+308 Args: 
+309 *a: can be for example Table(<id>) 
+310 **kw: can be for example Table(slug=<slug>) 
+311 """ 
+312 if not cls.__table: 
+313 raise EnvironmentError("@define or db.define is not called on this class
 yet!") 
-311 return cls.__table(*a, **kw) 
-312 
-313 @classmethod 
-314 def insert(cls, **fields: typing.Any) -> int: 
-315 """ 
-316 This is only called when db.define is not used as a decorator. 
-317 
-318 cls.__table functions as 'self' 
-319 
-320 Args: 
-321 **fields: anything you want to insert in the database 
+314 return cls.__table(*a, **kw) 
+315 
+316 @classmethod 
+317 def insert(cls, **fields: typing.Any) -> int: 
+318 """ 
+319 This is only called when db.define is not used as a decorator. 
+320 
+321 cls.__table functions as 'self' 
 322 
-323 Returns: the ID of the new row. 
-324 
-325 """ 
-326 if not cls.__table: 
-327 raise EnvironmentError("@define or db.define is not called on this class
+323 Args: 
+324 **fields: anything you want to insert in the database 
+325 
+326 Returns: the ID of the new row. 
+327 
+328 """ 
+329 if not cls.__table: 
+330 raise EnvironmentError("@define or db.define is not called on this class
 yet!") 
-328 
-329 result = super().insert(cls.__table, **fields) 
-330 # it already is an int but mypy doesn't understand that 
-331 return typing.cast(int, result) 
-332 
-333 
-334# backwards compat: 
-335TypedRow = TypedTable 
-336 
-337 
-338class TypedFieldType(Field): # type: ignore 
-339 """ 
-340 Typed version of pydal.Field, which will be converted to a normal Field in
-the background. 
-341 """ 
-342 
-343 # todo: .bind 
-344 
-345 # will be set by .bind on db.define 
-346 name = "" 
-347 _db = None 
-348 _rname = None 
-349 _table = None 
+331 
+332 result = super().insert(cls.__table, **fields) 
+333 # it already is an int but mypy doesn't understand that 
+334 return typing.cast(int, result) 
+335 
+336 @classmethod 
+337 def update_or_insert(cls, query: T_Query = DEFAULT, **values: typing.Any) -
+> typing.Optional[int]: 
+338 """ 
+339 Add typing to pydal's update_or_insert. 
+340 """ 
+341 result = super().update_or_insert(cls, _key=query, **values) 
+342 if result is None: 
+343 return None 
+344 else: 
+345 return typing.cast(int, result) 
+346 
+347 
+348# backwards compat: 
+349TypedRow = TypedTable 
 350 
-351 _type: T_annotation 
-352 kwargs: typing.Any 
-353 
-354 def __init__(self, _type: T_annotation, **kwargs: typing.Any) -> None: 
+351 
+352class TypedFieldType(Field): # type: ignore 
+353 """ 
+354 Typed version of pydal.Field, which will be converted to a normal Field in
+the background. 
 355 """ 
-356 A TypedFieldType should not be inited manually, but TypedField (from
-`fields.py`) should be used! 
-357 """ 
-358 self._type = _type 
-359 self.kwargs = kwargs 
-360 
-361 def __str__(self) -> str: 
-362 """ 
-363 String representation of a Typed Field. 
+356 
+357 # todo: .bind 
+358 
+359 # will be set by .bind on db.define 
+360 name = "" 
+361 _db = None 
+362 _rname = None 
+363 _table = None 
 364 
-365 If `type` is set explicitly (e.g. TypedField(str, type="text")), that type
+365 _type: T_annotation 
+366 kwargs: typing.Any 
+367 
+368 def __init__(self, _type: T_annotation, **kwargs: typing.Any) -> None: 
+369 """ 
+370 A TypedFieldType should not be inited manually, but TypedField (from
+`fields.py`) should be used! 
+371 """ 
+372 self._type = _type 
+373 self.kwargs = kwargs 
+374 
+375 def __str__(self) -> str: 
+376 """ 
+377 String representation of a Typed Field. 
+378 
+379 If `type` is set explicitly (e.g. TypedField(str, type="text")), that type
 is used: `TypedField.text`, 
-366 otherwise the type annotation is used (e.g. TypedField(str) -
+380 otherwise the type annotation is used (e.g. TypedField(str) -
 > TypedField.str) 
-367 """ 
-368 if "type" in self.kwargs: 
-369 # manual type in kwargs supplied 
-370 t = self.kwargs["type"] 
-371 elif issubclass(type, type(self._type)): 
-372 # normal type, str.__name__ = 'str' 
-373 t = getattr(self._type, "__name__", str(self._type)) 
-374 elif t_args := typing.get_args(self._type): 
-375 # list[str] -> 'str' 
-376 t = t_args[0].__name__ 
-377 else: # pragma: no cover 
-378 # fallback - something else, may not even happen, I'm not sure 
-379 t = self._type 
-380 return f"TypedField.{t}" 
-381 
-382 def __repr__(self) -> str: 
-383 """ 
-384 More detailed string representation of a Typed Field. 
-385 
-386 Uses __str__ and adds the provided extra options (kwargs) in the
+381 """ 
+382 if "type" in self.kwargs: 
+383 # manual type in kwargs supplied 
+384 t = self.kwargs["type"] 
+385 elif issubclass(type, type(self._type)): 
+386 # normal type, str.__name__ = 'str' 
+387 t = getattr(self._type, "__name__", str(self._type)) 
+388 elif t_args := typing.get_args(self._type): 
+389 # list[str] -> 'str' 
+390 t = t_args[0].__name__ 
+391 else: # pragma: no cover 
+392 # fallback - something else, may not even happen, I'm not sure 
+393 t = self._type 
+394 return f"TypedField.{t}" 
+395 
+396 def __repr__(self) -> str: 
+397 """ 
+398 More detailed string representation of a Typed Field. 
+399 
+400 Uses __str__ and adds the provided extra options (kwargs) in the
 representation. 
-387 """ 
-388 s = self.__str__() 
-389 kw = self.kwargs.copy() 
-390 kw.pop("type", None) 
-391 return f"<{s} with options {kw}>" 
-392 
-393 def _to_field(self, extra_kwargs: typing.MutableMapping[str, typing.Any]) -
+401 """ 
+402 s = self.__str__() 
+403 kw = self.kwargs.copy() 
+404 kw.pop("type", None) 
+405 return f"<{s} with options {kw}>" 
+406 
+407 def _to_field(self, extra_kwargs: typing.MutableMapping[str, typing.Any]) -
 > typing.Optional[str]: 
-394 """ 
-395 Convert a Typed Field instance to a pydal.Field. 
-396 """ 
-397 other_kwargs = self.kwargs.copy() 
-398 extra_kwargs.update(other_kwargs) 
-399 return extra_kwargs.pop("type", False) or
+408 """ 
+409 Convert a Typed Field instance to a pydal.Field. 
+410 """ 
+411 other_kwargs = self.kwargs.copy() 
+412 extra_kwargs.update(other_kwargs) 
+413 return extra_kwargs.pop("type", False) or
 TypeDAL._annotation_to_pydal_fieldtype(self._type, extra_kwargs) 
-400 
-401 def bind(self, field: Field, table: Table) -> None: 
-402 """ 
-403 Bind the right db/table/field info to this class, so queries can be made
-using `Class.field == ...`. 
-404 """ 
-405 self.name = field.name 
-406 self.type = field.type 
-407 super().bind(table) 
-408 
-409 # def __eq__(self, value): 
-410 # return Query(self.db, self._dialect.eq, self, value) 
-411 
-412 
-413S = typing.TypeVar("S") 
 414 
-415 
-416class TypedRows(typing.Collection[S], Rows): # type: ignore 
-417 """ 
-418 Can be used as the return type of a .select(). 
-419 
-420 Example: 
-421 people: TypedRows[Person] = db(Person).select() 
-422 """ 
-423 
-424 
-425T_Table = typing.TypeVar("T_Table", bound=Table) 
+415 def bind(self, field: Field, table: Table) -> None: 
+416 """ 
+417 Bind the right db/table/field info to this class, so queries can be made
+using `Class.field == ...`. 
+418 """ 
+419 self.name = field.name 
+420 self.type = field.type 
+421 super().bind(table) 
+422 
+423 # def __eq__(self, value): 
+424 # return Query(self.db, self._dialect.eq, self, value) 
+425 
 426 
-427 
-428class TypedSet(pydal.objects.Set): # type: ignore # pragma: no cover 
-429 """ 
-430 Used to make pydal Set more typed. 
-431 
-432 This class is not actually used, only 'cast' by TypeDAL.__call__ 
-433 """ 
-434 
-435 def count(self, distinct: bool = None, cache: dict[str, typing.Any] = None)
--> int: 
+427S = typing.TypeVar("S") 
+428 
+429 
+430class TypedRows(typing.Collection[S], Rows): # type: ignore 
+431 """ 
+432 Can be used as the return type of a .select(). 
+433 
+434 Example: 
+435 people: TypedRows[Person] = db(Person).select() 
 436 """ 
-437 Count returns an int. 
-438 """ 
-439 result = super().count(distinct, cache) 
-440 return typing.cast(int, result) 
+437 
+438 
+439T_Table = typing.TypeVar("T_Table", bound=Table) 
+440 
 441 
-442 def select(self, *fields: typing.Any, **attributes: typing.Any) -
-> TypedRows[T_Table]: 
+442class TypedSet(pydal.objects.Set): # type: ignore # pragma: no cover 
 443 """ 
-444 Select returns a TypedRows of a user defined table. 
+444 Used to make pydal Set more typed. 
 445 
-446 Example: 
-447 result: TypedRows[MyTable] = db(MyTable.id > 0).select() 
+446 This class is not actually used, only 'cast' by TypeDAL.__call__ 
+447 """ 
 448 
-449 for row in result: 
-450 typing.reveal_type(row) # MyTable 
-451 """ 
-452 rows = super().select(*fields, **attributes) 
-453 return typing.cast(TypedRows[T_Table], rows) 
+449 def count(self, distinct: bool = None, cache: dict[str, typing.Any] = None)
+-> int: 
+450 """ 
+451 Count returns an int. 
+452 """ 
+453 result = super().count(distinct, cache) 
+454 return typing.cast(int, result) 
+455 
+456 def select(self, *fields: typing.Any, **attributes: typing.Any) -
+> TypedRows[T_Table]: 
+457 """ 
+458 Select returns a TypedRows of a user defined table. 
+459 
+460 Example: 
+461 result: TypedRows[MyTable] = db(MyTable.id > 0).select() 
+462 
+463 for row in result: 
+464 typing.reveal_type(row) # MyTable 
+465 """ 
+466 rows = super().select(*fields, **attributes) 
+467 return typing.cast(TypedRows[T_Table], rows) 
 
 &#xab;_prev     &Hat;_index     &#xbb;_next       coverage.py_v7.2.7, created
-at 2023-06-27 17:50 +0200
+at 2023-06-27 18:15 +0200
```

### Comparing `typedal-1.2.0/htmlcov/d_0ccc93afd6526b6c_fields_py.html` & `typedal-1.2.1/htmlcov/d_0ccc93afd6526b6c_fields_py.html`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/htmlcov/favicon_32.png` & `typedal-1.2.1/htmlcov/favicon_32.png`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/htmlcov/index.html` & `typedal-1.2.1/htmlcov/index.html`

 * *Files 2% similar despite different names*

```diff
@@ -41,15 +41,15 @@
             </div>
         </aside>
         <form id="filter_container">
             <input id="filter" type="text" value="" placeholder="filter..." />
         </form>
         <p class="text">
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.7">coverage.py v7.2.7</a>,
-            created at 2023-06-27 17:50 +0200
+            created at 2023-06-27 18:16 +0200
         </p>
     </div>
 </header>
 <main id="index">
     <table class="index" data-sortable>
         <thead>
             <tr class="tablehead" title="Click to sort">
@@ -73,46 +73,46 @@
                 <td>4</td>
                 <td>0</td>
                 <td>0</td>
                 <td class="right" data-ratio="4 4">100%</td>
             </tr>
             <tr class="file">
                 <td class="name left"><a href="d_0ccc93afd6526b6c_core_py.html">src/typedal/core.py</a></td>
-                <td>144</td>
+                <td>153</td>
                 <td>0</td>
                 <td>12</td>
-                <td class="right" data-ratio="144 144">100%</td>
+                <td class="right" data-ratio="153 153">100%</td>
             </tr>
             <tr class="file">
                 <td class="name left"><a href="d_0ccc93afd6526b6c_fields_py.html">src/typedal/fields.py</a></td>
                 <td>88</td>
                 <td>0</td>
                 <td>0</td>
                 <td class="right" data-ratio="88 88">100%</td>
             </tr>
         </tbody>
         <tfoot>
             <tr class="total">
                 <td class="name left">Total</td>
-                <td>237</td>
+                <td>246</td>
                 <td>0</td>
                 <td>12</td>
-                <td class="right" data-ratio="237 237">100%</td>
+                <td class="right" data-ratio="246 246">100%</td>
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
-            created at 2023-06-27 17:50 +0200
+            created at 2023-06-27 18:16 +0200
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
@@ -2,19 +2,19 @@
 ****** Coverage report: 100% ******
  ⁰  [Show/hide keyboard shortcuts]
 Shortcuts on this page
 n s m x c   change column sorting
 [ ]   prev/next file
 ?   show/hide this help
 [                    ]
-coverage.py_v7.2.7, created at 2023-06-27 17:50 +0200
+coverage.py_v7.2.7, created at 2023-06-27 18:16 +0200
 
 Module                   statements missing excluded coverage
 src/typedal/__about__.py 1          0       0        100%
 src/typedal/__init__.py  4          0       0        100%
-src/typedal/core.py      144        0       12       100%
+src/typedal/core.py      153        0       12       100%
 src/typedal/fields.py    88         0       0        100%
-Total                    237        0       12       100%
+Total                    246        0       12       100%
 No items found using the specified filter.
 
-coverage.py_v7.2.7, created at 2023-06-27 17:50 +0200
+coverage.py_v7.2.7, created at 2023-06-27 18:16 +0200
  ____
```

### Comparing `typedal-1.2.0/htmlcov/keybd_closed.png` & `typedal-1.2.1/htmlcov/keybd_closed.png`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/htmlcov/keybd_open.png` & `typedal-1.2.1/htmlcov/keybd_open.png`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/htmlcov/status.json` & `typedal-1.2.1/htmlcov/status.json`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9920428240740741%*

 * *Differences: {"'files'": "{'d_0ccc93afd6526b6c___about___py': {'hash': '444a462c64f0c3ae18642e64523ff791'}, "*

 * *            "'d_0ccc93afd6526b6c_core_py': {'hash': '7ed8a2335e7efe7b03754b7a90062de6', 'index': "*

 * *            "{'nums': {insert: [(2, 153)], delete: [2]}}}}"}*

```diff
@@ -1,11 +1,11 @@
 {
     "files": {
         "d_0ccc93afd6526b6c___about___py": {
-            "hash": "4c3eca8da28906a79fc17b13dbdd4d77",
+            "hash": "444a462c64f0c3ae18642e64523ff791",
             "index": {
                 "html_filename": "d_0ccc93afd6526b6c___about___py.html",
                 "nums": [
                     0,
                     1,
                     1,
                     0,
@@ -31,21 +31,21 @@
                     0,
                     0
                 ],
                 "relative_filename": "src/typedal/__init__.py"
             }
         },
         "d_0ccc93afd6526b6c_core_py": {
-            "hash": "2c473194e63e68eb985a8c1f999246dc",
+            "hash": "7ed8a2335e7efe7b03754b7a90062de6",
             "index": {
                 "html_filename": "d_0ccc93afd6526b6c_core_py.html",
                 "nums": [
                     0,
                     1,
-                    144,
+                    153,
                     12,
                     0,
                     0,
                     0,
                     0
                 ],
                 "relative_filename": "src/typedal/core.py"
```

### Comparing `typedal-1.2.0/htmlcov/style.css` & `typedal-1.2.1/htmlcov/style.css`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/src/typedal/core.py` & `typedal-1.2.1/src/typedal/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,18 +4,20 @@
 import datetime as dt
 import types
 import typing
 from collections import ChainMap
 from decimal import Decimal
 
 import pydal
-from pydal.objects import Field, Row, Rows, Table
+from pydal._globals import DEFAULT
+from pydal.objects import Field, Query, Row, Rows, Table
 
 # use typing.cast(type, ...) to make mypy happy with unions
 T_annotation = typing.Type[typing.Any] | types.UnionType
+T_Query = typing.Union["Table", "Query", "bool", "None", "TypedTable", typing.Type["TypedTable"]]
 
 BASIC_MAPPINGS: dict[T_annotation, str] = {
     str: "string",
     int: "integer",
     bool: "boolean",
     bytes: "blob",
     float: "double",
@@ -138,15 +140,15 @@
 
         cls.__set_internals__(db=self, table=table)
 
         # the ACTUAL output is not TypedTable but rather pydal.Table
         # but telling the editor it is T helps with hinting.
         return cls
 
-    def __call__(self, *_args: typing.Any, **kwargs: typing.Any) -> "TypedSet":
+    def __call__(self, *_args: T_Query, **kwargs: typing.Any) -> "TypedSet":
         """
         A db instance can be called directly to perform a query.
 
         Usually, only a query is passed.
 
         Example:
             db(query).select()
@@ -154,17 +156,18 @@
         """
         args = list(_args)
         if args:
             cls = args[0]
             if isinstance(cls, bool):
                 raise ValueError("Don't actually pass a bool to db()! Use a query instead.")
 
-            if issubclass(type(cls), type) and issubclass(cls, TypedTable):
+            if isinstance(cls, type) and issubclass(type(cls), type) and issubclass(cls, TypedTable):
                 # table defined without @db.define decorator!
-                args[0] = cls.id != None
+                _cls: typing.Type[TypedTable] = cls
+                args[0] = _cls.id != None
 
         _set = super().__call__(*args, **kwargs)
         return typing.cast(TypedSet, _set)
 
     # todo: insert etc shadowen?
 
     @classmethod
@@ -326,14 +329,25 @@
         if not cls.__table:
             raise EnvironmentError("@define or db.define is not called on this class yet!")
 
         result = super().insert(cls.__table, **fields)
         # it already is an int but mypy doesn't understand that
         return typing.cast(int, result)
 
+    @classmethod
+    def update_or_insert(cls, query: T_Query = DEFAULT, **values: typing.Any) -> typing.Optional[int]:
+        """
+        Add typing to pydal's update_or_insert.
+        """
+        result = super().update_or_insert(cls, _key=query, **values)
+        if result is None:
+            return None
+        else:
+            return typing.cast(int, result)
+
 
 # backwards compat:
 TypedRow = TypedTable
 
 
 class TypedFieldType(Field):  # type: ignore
     """
```

### Comparing `typedal-1.2.0/src/typedal/fields.py` & `typedal-1.2.1/src/typedal/fields.py`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/tests/test_main.py` & `typedal-1.2.1/tests/test_main.py`

 * *Files 8% similar despite different names*

```diff
@@ -264,8 +264,39 @@
     counted3 = db(db.some_new_table).count()
 
     assert counted1 == counted2 == counted3 == 0
 
     select2: TypedRows[SomeNewTable] = db(SomeNewTable).select()
 
     for row in select2:
-        raise ValueError("no rows should exist")
+        raise ValueError("no rows should exist")
+
+    SomeNewTable.update_or_insert(
+        SomeNewTable.name == "Hendrik",
+        name="Hendrik 2",
+    )
+
+    idx = OtherNewTable.update_or_insert(
+        OtherNewTable.name == "Hendrik",
+        name="Hendrik 2",
+    )
+    assert idx
+
+    OtherNewTable.update_or_insert(
+        OtherNewTable.name == "Hendrik",
+        name="Hendrik 2",
+    )
+
+    assert db(SomeNewTable.name == "Hendrik").count() == 0
+    assert db(SomeNewTable.name == "Hendrik 2").count() == 1
+
+    assert db(OtherNewTable.name == "Hendrik").count() == 0
+    assert db(OtherNewTable.name == "Hendrik 2").count() == 2
+
+    no_idx = OtherNewTable.update_or_insert(
+        OtherNewTable.name == "Hendrik 2",
+        name="Hendrik 3",
+    )  # should only update one and return None!
+
+    assert no_idx is None
+    assert db(OtherNewTable.name == "Hendrik 2").count() == 1
+    assert db(OtherNewTable.name == "Hendrik 3").count() == 1
```

### Comparing `typedal-1.2.0/tests/test_mypy.py` & `typedal-1.2.1/tests/test_mypy.py`

 * *Files 20% similar despite different names*

```diff
@@ -28,7 +28,26 @@
     select2: TypedRows[MyTable] = db(MyTable).select()
 
     typing.reveal_type(select1)  # R: src.typedal.core.TypedRows[Any]
     typing.reveal_type(select2)  # R: src.typedal.core.TypedRows[tests.test_mypy.MyTable]
 
     for row in select2:
         typing.reveal_type(row)  # R: tests.test_mypy.MyTable
+
+
+@pytest.mark.mypy_testing
+def mypy_test_query() -> None:
+    db(
+        MyTable.id > 0
+    )
+
+    db(
+        db.old_style.id > 3
+    )
+
+    db(MyTable)
+
+    db(db.old_style)
+
+    MyTable.update_or_insert(MyTable)
+    MyTable.update_or_insert(MyTable.id > 3)
+    MyTable.update_or_insert(db.my_table.id > 3)
```

### Comparing `typedal-1.2.0/README.md` & `typedal-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/pyproject.toml` & `typedal-1.2.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `typedal-1.2.0/PKG-INFO` & `typedal-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TypeDal
-Version: 1.2.0
+Version: 1.2.1
 Summary: Typing support for PyDAL
 Project-URL: Documentation, https://github.com/trialandsuccess/TypeDAL#readme
 Project-URL: Issues, https://github.com/trialandsuccess/TypeDAL/issues
 Project-URL: Source, https://github.com/trialandsuccess/TypeDAL
 Author-email: Robin van der Noord <contact@trialandsuccess.nl>
 License-Expression: MIT
 Classifier: Development Status :: 4 - Beta
```

