# Comparing `tmp/h3ronpy-0.17.0.tar.gz` & `tmp/h3ronpy-0.9.0.tar.gz`

## Comparing `h3ronpy-0.17.0.tar` & `h3ronpy-0.9.0.tar`

### file list

```diff
@@ -1,74 +1,99 @@
--rw-r--r--   0        0        0     1247 1970-01-01 00:00:00.000000 h3ronpy-0.17.0/Cargo.toml
--rw-r--r--   0        0        0       59 2023-06-27 17:59:52.000000 h3ronpy-0.17.0/.gitattributes
--rw-r--r--   0        0        0     5917 2023-06-27 17:59:52.000000 h3ronpy-0.17.0/.github/workflows/ci.yml
--rw-r--r--   0        0        0      231 2023-06-27 17:59:52.000000 h3ronpy-0.17.0/.gitignore
--rw-r--r--   0        0        0      219 2023-06-27 17:59:52.000000 h3ronpy-0.17.0/.readthedocs.yaml
--rw-r--r--   0        0        0     4797 2023-06-27 17:59:52.000000 h3ronpy-0.17.0/CHANGES.rst
--rw-r--r--   0        0        0     1479 2023-06-27 17:59:52.000000 h3ronpy-0.17.0/CONTRIBUTING.rst
--rw-r--r--   0        0        0     1046 2023-06-27 17:59:52.000000 h3ronpy-0.17.0/LICENSE.txt
--rw-r--r--   0        0        0       91 2023-06-27 17:59:52.000000 h3ronpy-0.17.0/MANIFEST.in
--rw-r--r--   0        0        0     1461 2023-06-27 17:59:52.000000 h3ronpy-0.17.0/README.rst
--rw-r--r--   0        0        0   279250 2023-06-27 17:59:52.000000 h3ronpy-0.17.0/data/europe-and-north-africa.tif
--rw-r--r--   0        0        0   489248 2023-06-27 17:59:52.000000 h3ronpy-0.17.0/data/naturalearth_110m_admin_0_countries.fgb
--rw-r--r--   0        0        0    90924 2023-06-27 17:59:52.000000 h3ronpy-0.17.0/data/r.tiff
--rw-r--r--   0        0        0      658 2023-06-27 17:59:52.000000 h3ronpy-0.17.0/docs/Makefile
--rw-r--r--   0        0        0      799 2023-06-27 17:59:52.000000 h3ronpy-0.17.0/docs/make.bat
--rw-r--r--   0        0        0      145 2023-06-27 17:59:52.000000 h3ronpy-0.17.0/docs/requirements.txt
--rw-r--r--   0        0        0      321 2023-06-27 17:59:52.000000 h3ronpy-0.17.0/docs/source/api/arrow.rst
--rw-r--r--   0        0        0       88 2023-06-27 17:59:52.000000 h3ronpy-0.17.0/docs/source/api/index.rst
--rw-r--r--   0        0        0      346 2023-06-27 17:59:52.000000 h3ronpy-0.17.0/docs/source/api/pandas.rst
--rw-r--r--   0        0        0      326 2023-06-27 17:59:52.000000 h3ronpy-0.17.0/docs/source/api/polars.rst
--rw-r--r--   0        0        0       32 2023-06-27 17:59:52.000000 h3ronpy-0.17.0/docs/source/changelog.rst
--rw-r--r--   0        0        0     1007 2023-06-27 17:59:52.000000 h3ronpy-0.17.0/docs/source/conf.py
--rw-r--r--   0        0        0       37 2023-06-27 17:59:52.000000 h3ronpy-0.17.0/docs/source/contributing.rst
--rw-r--r--   0        0        0      248 2023-06-27 17:59:52.000000 h3ronpy-0.17.0/docs/source/index.rst
--rw-r--r--   0        0        0     1118 2023-06-27 17:59:52.000000 h3ronpy-0.17.0/docs/source/installation.rst
--rw-r--r--   0        0        0       57 2023-06-27 17:59:52.000000 h3ronpy-0.17.0/docs/source/license.rst
--rw-r--r--   0        0        0     1632 2023-06-27 17:59:52.000000 h3ronpy-0.17.0/docs/source/usage/grid.rst
--rw-r--r--   0        0        0      412 2023-06-27 17:59:52.000000 h3ronpy-0.17.0/docs/source/usage/index.rst
--rw-r--r--   0        0        0     2656 2023-06-27 17:59:52.000000 h3ronpy-0.17.0/docs/source/usage/raster.rst
--rw-r--r--   0        0        0     2360 2023-06-27 17:59:52.000000 h3ronpy-0.17.0/docs/source/usage/vector.rst
--rw-r--r--   0        0        0      331 2023-06-27 17:59:52.000000 h3ronpy-0.17.0/h3ronpy/__init__.py
--rw-r--r--   0        0        0     5151 2023-06-27 17:59:52.000000 h3ronpy-0.17.0/h3ronpy/arrow/__init__.py
--rw-r--r--   0        0        0     3670 2023-06-27 17:59:52.000000 h3ronpy-0.17.0/h3ronpy/arrow/raster.py
--rw-r--r--   0        0        0      596 2023-06-27 17:59:52.000000 h3ronpy-0.17.0/h3ronpy/arrow/util.py
--rw-r--r--   0        0        0     3044 2023-06-27 17:59:52.000000 h3ronpy-0.17.0/h3ronpy/arrow/vector.py
--rw-r--r--   0        0        0     2711 2023-06-27 17:59:52.000000 h3ronpy-0.17.0/h3ronpy/pandas/__init__.py
--rw-r--r--   0        0        0     1909 2023-06-27 17:59:52.000000 h3ronpy-0.17.0/h3ronpy/pandas/raster.py
--rw-r--r--   0        0        0     4202 2023-06-27 17:59:52.000000 h3ronpy-0.17.0/h3ronpy/pandas/vector.py
--rw-r--r--   0        0        0     2512 2023-06-27 17:59:52.000000 h3ronpy-0.17.0/h3ronpy/polars/__init__.py
--rw-r--r--   0        0        0      344 2023-06-27 17:59:52.000000 h3ronpy-0.17.0/h3ronpy/polars/raster.py
--rw-r--r--   0        0        0     1196 2023-06-27 17:59:52.000000 h3ronpy-0.17.0/h3ronpy/polars/vector.py
--rw-r--r--   0        0        0     1621 2023-06-27 17:59:52.000000 h3ronpy-0.17.0/install-dev-dependencies.py
--rw-r--r--   0        0        0      175 2023-06-27 17:59:52.000000 h3ronpy-0.17.0/justfile
--rw-r--r--   0        0        0      703 2023-06-27 17:59:52.000000 h3ronpy-0.17.0/pyproject.toml
--rw-r--r--   0        0        0     3427 2023-06-27 17:59:52.000000 h3ronpy-0.17.0/src/arrow_interop.rs
--rw-r--r--   0        0        0     2717 2023-06-27 17:59:52.000000 h3ronpy-0.17.0/src/error.rs
--rw-r--r--   0        0        0     1607 2023-06-27 17:59:52.000000 h3ronpy-0.17.0/src/lib.rs
--rw-r--r--   0        0        0     1097 2023-06-27 17:59:52.000000 h3ronpy-0.17.0/src/op/compact.rs
--rw-r--r--   0        0        0      921 2023-06-27 17:59:52.000000 h3ronpy-0.17.0/src/op/measure.rs
--rw-r--r--   0        0        0     1310 2023-06-27 17:59:52.000000 h3ronpy-0.17.0/src/op/mod.rs
--rw-r--r--   0        0        0     4509 2023-06-27 17:59:52.000000 h3ronpy-0.17.0/src/op/neighbor.rs
--rw-r--r--   0        0        0      624 2023-06-27 17:59:52.000000 h3ronpy-0.17.0/src/op/parse.rs
--rw-r--r--   0        0        0     1905 2023-06-27 17:59:52.000000 h3ronpy-0.17.0/src/op/resolution.rs
--rw-r--r--   0        0        0     1815 2023-06-27 17:59:52.000000 h3ronpy-0.17.0/src/op/valid.rs
--rw-r--r--   0        0        0     7379 2023-06-27 17:59:52.000000 h3ronpy-0.17.0/src/raster.rs
--rw-r--r--   0        0        0     1560 2023-06-27 17:59:52.000000 h3ronpy-0.17.0/src/transform.rs
--rw-r--r--   0        0        0     9417 2023-06-27 17:59:52.000000 h3ronpy-0.17.0/src/vector.rs
--rw-r--r--   0        0        0      288 2023-06-27 17:59:52.000000 h3ronpy-0.17.0/tests/__init__.py
--rw-r--r--   0        0        0        0 2023-06-27 17:59:52.000000 h3ronpy-0.17.0/tests/arrow/__init__.py
--rw-r--r--   0        0        0      384 2023-06-27 17:59:52.000000 h3ronpy-0.17.0/tests/arrow/test_vector.py
--rw-r--r--   0        0        0        0 2023-06-27 17:59:52.000000 h3ronpy-0.17.0/tests/pandas/__init__.py
--rw-r--r--   0        0        0     1763 2023-06-27 17:59:52.000000 h3ronpy-0.17.0/tests/pandas/test_raster.py
--rw-r--r--   0        0        0     1597 2023-06-27 17:59:52.000000 h3ronpy-0.17.0/tests/pandas/test_resolution.py
--rw-r--r--   0        0        0     2956 2023-06-27 17:59:52.000000 h3ronpy-0.17.0/tests/pandas/test_vector.py
--rw-r--r--   0        0        0        0 2023-06-27 17:59:52.000000 h3ronpy-0.17.0/tests/polars/__init__.py
--rw-r--r--   0        0        0     1101 2023-06-27 17:59:52.000000 h3ronpy-0.17.0/tests/polars/test_compact.py
--rw-r--r--   0        0        0     1336 2023-06-27 17:59:52.000000 h3ronpy-0.17.0/tests/polars/test_coordinates.py
--rw-r--r--   0        0        0      562 2023-06-27 17:59:52.000000 h3ronpy-0.17.0/tests/polars/test_measure.py
--rw-r--r--   0        0        0     2499 2023-06-27 17:59:52.000000 h3ronpy-0.17.0/tests/polars/test_neighbor.py
--rw-r--r--   0        0        0     1363 2023-06-27 17:59:52.000000 h3ronpy-0.17.0/tests/polars/test_parse.py
--rw-r--r--   0        0        0     1150 2023-06-27 17:59:52.000000 h3ronpy-0.17.0/tests/polars/test_raster.py
--rw-r--r--   0        0        0      217 2023-06-27 17:59:52.000000 h3ronpy-0.17.0/tests/test_transform.py
--rw-r--r--   0        0        0    36512 2023-06-27 18:03:42.000000 h3ronpy-0.17.0/Cargo.lock
--rw-r--r--   0        0        0     2397 1970-01-01 00:00:00.000000 h3ronpy-0.17.0/PKG-INFO
+-rw-r--r--   0        0        0      734 1970-01-01 00:00:00.000000 h3ronpy-0.9.0/local_dependencies/h3ron/Cargo.toml
+-rw-rw-r--   0     1000     1000     3843 2021-04-08 12:23:38.000000 h3ronpy-0.9.0/local_dependencies/h3ron/src/algorithm.rs
+-rw-rw-r--   0     1000     1000    13471 2021-04-08 12:23:38.000000 h3ronpy-0.9.0/local_dependencies/h3ron/src/collections.rs
+-rw-rw-r--   0     1000     1000     1618 2021-04-05 19:34:20.000000 h3ronpy-0.9.0/local_dependencies/h3ron/src/error.rs
+-rw-rw-r--   0     1000     1000     2594 2021-04-11 12:23:33.000000 h3ronpy-0.9.0/local_dependencies/h3ron/src/experimental.rs
+-rw-rw-r--   0     1000     1000    16161 2021-04-08 12:24:15.000000 h3ronpy-0.9.0/local_dependencies/h3ron/src/index.rs
+-rw-rw-r--   0     1000     1000     6872 2021-04-08 12:23:38.000000 h3ronpy-0.9.0/local_dependencies/h3ron/src/lib.rs
+-rw-rw-r--   0     1000     1000     7546 2021-04-08 12:23:38.000000 h3ronpy-0.9.0/local_dependencies/h3ron/src/to_geo.rs
+-rw-rw-r--   0     1000     1000     4307 2021-04-08 12:23:38.000000 h3ronpy-0.9.0/local_dependencies/h3ron/src/to_h3.rs
+-rw-rw-r--   0     1000     1000      999 2021-04-05 19:34:20.000000 h3ronpy-0.9.0/local_dependencies/h3ron/src/util.rs
+-rw-r--r--   0        0        0      637 1970-01-01 00:00:00.000000 h3ronpy-0.9.0/local_dependencies/h3ron-h3-sys/Cargo.toml
+-rw-rw-r--   0     1000     1000      410 2021-03-05 18:52:26.000000 h3ronpy-0.9.0/local_dependencies/h3ron-h3-sys/README.md
+-rw-rw-r--   0     1000     1000     2058 2021-04-08 12:23:38.000000 h3ronpy-0.9.0/local_dependencies/h3ron-h3-sys/build.rs
+-rw-rw-r--   0     1000     1000       36 2021-03-05 18:52:30.000000 h3ronpy-0.9.0/local_dependencies/h3ron-h3-sys/libh3/.clang-format
+-rw-rw-r--   0     1000     1000     1135 2021-03-05 18:52:30.000000 h3ronpy-0.9.0/local_dependencies/h3ron-h3-sys/libh3/.clang-tidy
+-rw-rw-r--   0     1000     1000     1374 2021-03-05 18:52:30.000000 h3ronpy-0.9.0/local_dependencies/h3ron-h3-sys/libh3/.gitignore
+-rw-rw-r--   0     1000     1000     1799 2021-03-05 18:52:30.000000 h3ronpy-0.9.0/local_dependencies/h3ron-h3-sys/libh3/.travis.yml
+-rw-rw-r--   0     1000     1000     8707 2021-03-05 18:52:30.000000 h3ronpy-0.9.0/local_dependencies/h3ron-h3-sys/libh3/CHANGELOG.md
+-rw-rw-r--   0     1000     1000    29799 2021-03-05 18:52:30.000000 h3ronpy-0.9.0/local_dependencies/h3ron-h3-sys/libh3/CMakeLists.txt
+-rw-rw-r--   0     1000     1000     1483 2021-03-05 18:52:30.000000 h3ronpy-0.9.0/local_dependencies/h3ron-h3-sys/libh3/CONTRIBUTING.md
+-rw-rw-r--   0     1000     1000     7611 2021-03-05 18:52:30.000000 h3ronpy-0.9.0/local_dependencies/h3ron-h3-sys/libh3/KML/icosa.kml
+-rw-rw-r--   0     1000     1000    11354 2021-03-05 18:52:30.000000 h3ronpy-0.9.0/local_dependencies/h3ron-h3-sys/libh3/LICENSE
+-rw-rw-r--   0     1000     1000     7575 2021-03-05 18:52:30.000000 h3ronpy-0.9.0/local_dependencies/h3ron-h3-sys/libh3/README.md
+-rw-rw-r--   0     1000     1000      593 2021-03-05 18:52:30.000000 h3ronpy-0.9.0/local_dependencies/h3ron-h3-sys/libh3/RELEASE.md
+-rw-rw-r--   0     1000     1000        6 2021-03-05 18:52:30.000000 h3ronpy-0.9.0/local_dependencies/h3ron-h3-sys/libh3/VERSION
+-rw-rw-r--   0     1000     1000      125 2021-03-05 18:52:30.000000 h3ronpy-0.9.0/local_dependencies/h3ron-h3-sys/libh3/cmake/Config.cmake.in
+-rw-rw-r--   0     1000     1000     1403 2021-03-05 18:52:30.000000 h3ronpy-0.9.0/local_dependencies/h3ron-h3-sys/libh3/cmake/TestWrapValgrind.cmake
+-rw-rw-r--   0     1000     1000      643 2021-03-05 18:52:30.000000 h3ronpy-0.9.0/local_dependencies/h3ron-h3-sys/libh3/cmake/toolchain.cmake
+-rw-rw-r--   0     1000     1000      966 2021-03-05 18:52:30.000000 h3ronpy-0.9.0/local_dependencies/h3ron-h3-sys/libh3/scripts/binding_functions.ps1
+-rwxrwxr-x   0     1000     1000      945 2021-03-05 18:52:30.000000 h3ronpy-0.9.0/local_dependencies/h3ron-h3-sys/libh3/scripts/binding_functions.sh
+-rwxrwxr-x   0     1000     1000     2364 2021-03-05 18:52:30.000000 h3ronpy-0.9.0/local_dependencies/h3ron-h3-sys/libh3/scripts/coverage.sh.in
+-rwxrwxr-x   0     1000     1000      931 2021-03-05 18:52:30.000000 h3ronpy-0.9.0/local_dependencies/h3ron-h3-sys/libh3/scripts/publish_website.sh
+-rwxrwxr-x   0     1000     1000     1761 2021-03-05 18:52:30.000000 h3ronpy-0.9.0/local_dependencies/h3ron-h3-sys/libh3/scripts/update_version.sh
+-rw-rw-r--   0     1000     1000     1791 2021-03-05 18:52:30.000000 h3ronpy-0.9.0/local_dependencies/h3ron-h3-sys/libh3/src/h3lib/include/algos.h
+-rw-rw-r--   0     1000     1000     1286 2021-03-05 18:52:30.000000 h3ronpy-0.9.0/local_dependencies/h3ron-h3-sys/libh3/src/h3lib/include/alloc.h
+-rw-rw-r--   0     1000     1000     2114 2021-03-05 18:52:30.000000 h3ronpy-0.9.0/local_dependencies/h3ron-h3-sys/libh3/src/h3lib/include/baseCells.h
+-rw-rw-r--   0     1000     1000     1400 2021-03-05 18:52:30.000000 h3ronpy-0.9.0/local_dependencies/h3ron-h3-sys/libh3/src/h3lib/include/bbox.h
+-rw-rw-r--   0     1000     1000     2470 2021-03-05 18:52:30.000000 h3ronpy-0.9.0/local_dependencies/h3ron-h3-sys/libh3/src/h3lib/include/constants.h
+-rw-rw-r--   0     1000     1000     3744 2021-03-05 18:52:30.000000 h3ronpy-0.9.0/local_dependencies/h3ron-h3-sys/libh3/src/h3lib/include/coordijk.h
+-rw-rw-r--   0     1000     1000     3055 2021-03-05 18:52:30.000000 h3ronpy-0.9.0/local_dependencies/h3ron-h3-sys/libh3/src/h3lib/include/faceijk.h
+-rw-rw-r--   0     1000     1000     1588 2021-03-05 18:52:30.000000 h3ronpy-0.9.0/local_dependencies/h3ron-h3-sys/libh3/src/h3lib/include/geoCoord.h
+-rw-rw-r--   0     1000     1000     6091 2021-03-05 18:52:30.000000 h3ronpy-0.9.0/local_dependencies/h3ron-h3-sys/libh3/src/h3lib/include/h3Index.h
+-rw-rw-r--   0     1000     1000      841 2021-03-05 18:52:30.000000 h3ronpy-0.9.0/local_dependencies/h3ron-h3-sys/libh3/src/h3lib/include/h3UniEdge.h
+-rw-rw-r--   0     1000     1000    19625 2021-03-05 18:52:30.000000 h3ronpy-0.9.0/local_dependencies/h3ron-h3-sys/libh3/src/h3lib/include/h3api.h.in
+-rw-rw-r--   0     1000     1000     3343 2021-03-05 18:52:30.000000 h3ronpy-0.9.0/local_dependencies/h3ron-h3-sys/libh3/src/h3lib/include/linkedGeo.h
+-rw-rw-r--   0     1000     1000      902 2021-03-05 18:52:30.000000 h3ronpy-0.9.0/local_dependencies/h3ron-h3-sys/libh3/src/h3lib/include/localij.h
+-rw-rw-r--   0     1000     1000      955 2021-03-05 18:52:30.000000 h3ronpy-0.9.0/local_dependencies/h3ron-h3-sys/libh3/src/h3lib/include/mathExtensions.h
+-rw-rw-r--   0     1000     1000     2469 2021-03-05 18:52:30.000000 h3ronpy-0.9.0/local_dependencies/h3ron-h3-sys/libh3/src/h3lib/include/polygon.h
+-rw-rw-r--   0     1000     1000     7049 2021-03-05 18:52:30.000000 h3ronpy-0.9.0/local_dependencies/h3ron-h3-sys/libh3/src/h3lib/include/polygonAlgos.h
+-rw-rw-r--   0     1000     1000     1126 2021-03-05 18:52:30.000000 h3ronpy-0.9.0/local_dependencies/h3ron-h3-sys/libh3/src/h3lib/include/vec2d.h
+-rw-rw-r--   0     1000     1000     1042 2021-03-05 18:52:30.000000 h3ronpy-0.9.0/local_dependencies/h3ron-h3-sys/libh3/src/h3lib/include/vec3d.h
+-rw-rw-r--   0     1000     1000     1400 2021-03-05 18:52:30.000000 h3ronpy-0.9.0/local_dependencies/h3ron-h3-sys/libh3/src/h3lib/include/vertex.h
+-rw-rw-r--   0     1000     1000     2022 2021-03-05 18:52:30.000000 h3ronpy-0.9.0/local_dependencies/h3ron-h3-sys/libh3/src/h3lib/include/vertexGraph.h
+-rw-rw-r--   0     1000     1000    41264 2021-03-05 18:52:30.000000 h3ronpy-0.9.0/local_dependencies/h3ron-h3-sys/libh3/src/h3lib/lib/algos.c
+-rw-rw-r--   0     1000     1000    37442 2021-03-05 18:52:30.000000 h3ronpy-0.9.0/local_dependencies/h3ron-h3-sys/libh3/src/h3lib/lib/baseCells.c
+-rw-rw-r--   0     1000     1000     5538 2021-03-05 18:52:30.000000 h3ronpy-0.9.0/local_dependencies/h3ron-h3-sys/libh3/src/h3lib/lib/bbox.c
+-rw-rw-r--   0     1000     1000    13648 2021-03-05 18:52:30.000000 h3ronpy-0.9.0/local_dependencies/h3ron-h3-sys/libh3/src/h3lib/lib/coordijk.c
+-rw-rw-r--   0     1000     1000    33881 2021-03-05 18:52:30.000000 h3ronpy-0.9.0/local_dependencies/h3ron-h3-sys/libh3/src/h3lib/lib/faceijk.c
+-rw-rw-r--   0     1000     1000    12511 2021-03-05 18:52:30.000000 h3ronpy-0.9.0/local_dependencies/h3ron-h3-sys/libh3/src/h3lib/lib/geoCoord.c
+-rw-rw-r--   0     1000     1000    34041 2021-03-05 18:52:30.000000 h3ronpy-0.9.0/local_dependencies/h3ron-h3-sys/libh3/src/h3lib/lib/h3Index.c
+-rw-rw-r--   0     1000     1000     9668 2021-03-05 18:52:30.000000 h3ronpy-0.9.0/local_dependencies/h3ron-h3-sys/libh3/src/h3lib/lib/h3UniEdge.c
+-rw-rw-r--   0     1000     1000    12599 2021-03-05 18:52:30.000000 h3ronpy-0.9.0/local_dependencies/h3ron-h3-sys/libh3/src/h3lib/lib/linkedGeo.c
+-rw-rw-r--   0     1000     1000    23670 2021-03-05 18:52:30.000000 h3ronpy-0.9.0/local_dependencies/h3ron-h3-sys/libh3/src/h3lib/lib/localij.c
+-rw-rw-r--   0     1000     1000     1177 2021-03-05 18:52:30.000000 h3ronpy-0.9.0/local_dependencies/h3ron-h3-sys/libh3/src/h3lib/lib/mathExtensions.c
+-rw-rw-r--   0     1000     1000     2700 2021-03-05 18:52:30.000000 h3ronpy-0.9.0/local_dependencies/h3ron-h3-sys/libh3/src/h3lib/lib/polygon.c
+-rw-rw-r--   0     1000     1000     2127 2021-03-05 18:52:30.000000 h3ronpy-0.9.0/local_dependencies/h3ron-h3-sys/libh3/src/h3lib/lib/vec2d.c
+-rw-rw-r--   0     1000     1000     1608 2021-03-05 18:52:30.000000 h3ronpy-0.9.0/local_dependencies/h3ron-h3-sys/libh3/src/h3lib/lib/vec3d.c
+-rw-rw-r--   0     1000     1000     4930 2021-03-05 18:52:30.000000 h3ronpy-0.9.0/local_dependencies/h3ron-h3-sys/libh3/src/h3lib/lib/vertex.c
+-rw-rw-r--   0     1000     1000     7267 2021-03-05 18:52:30.000000 h3ronpy-0.9.0/local_dependencies/h3ron-h3-sys/libh3/src/h3lib/lib/vertexGraph.c
+-rw-rw-r--   0     1000     1000      298 2021-03-05 18:52:26.000000 h3ronpy-0.9.0/local_dependencies/h3ron-h3-sys/src/lib.rs
+-rw-r--r--   0        0        0      812 1970-01-01 00:00:00.000000 h3ronpy-0.9.0/local_dependencies/h3ron-ndarray/Cargo.toml
+-rw-rw-r--   0     1000     1000      434 2021-03-05 18:52:26.000000 h3ronpy-0.9.0/local_dependencies/h3ron-ndarray/README.md
+-rw-rw-r--   0     1000     1000     1546 2021-04-05 19:35:37.000000 h3ronpy-0.9.0/local_dependencies/h3ron-ndarray/benches/convert_dataset_r.rs
+-rw-rw-r--   0     1000     1000     2347 2021-04-05 19:35:42.000000 h3ronpy-0.9.0/local_dependencies/h3ron-ndarray/examples/h3ify_r_tiff.rs
+-rw-rw-r--   0     1000     1000    13670 2021-04-09 19:08:10.000000 h3ronpy-0.9.0/local_dependencies/h3ron-ndarray/src/array.rs
+-rw-rw-r--   0     1000     1000      517 2021-04-05 18:44:30.000000 h3ronpy-0.9.0/local_dependencies/h3ron-ndarray/src/error.rs
+-rw-rw-r--   0     1000     1000      788 2021-04-05 19:35:30.000000 h3ronpy-0.9.0/local_dependencies/h3ron-ndarray/src/lib.rs
+-rw-rw-r--   0     1000     1000     3840 2021-04-08 12:23:38.000000 h3ronpy-0.9.0/local_dependencies/h3ron-ndarray/src/resolution.rs
+-rw-rw-r--   0     1000     1000     1521 2021-04-05 19:35:30.000000 h3ronpy-0.9.0/local_dependencies/h3ron-ndarray/src/sphere.rs
+-rw-rw-r--   0     1000     1000     6369 2021-04-05 19:35:30.000000 h3ronpy-0.9.0/local_dependencies/h3ron-ndarray/src/transform.rs
+-rw-r--r--   0        0        0     1298 1970-01-01 00:00:00.000000 h3ronpy-0.9.0/Cargo.toml
+-rw-rw-r--   0     1000     1000     1023 2021-04-11 18:37:21.000000 h3ronpy-0.9.0/LICENSE.txt
+-rw-rw-r--   0     1000     1000     2581 2021-04-11 18:37:21.000000 h3ronpy-0.9.0/README.md
+-rw-rw-r--   0     1000     1000  2088546 2021-04-09 19:04:30.000000 h3ronpy-0.9.0/documentation.ipynb
+-rw-rw-r--   0     1000     1000      143 2021-04-09 19:04:30.000000 h3ronpy-0.9.0/h3ronpy/__init__.py
+-rw-rw-r--   0     1000     1000     3951 2021-04-09 19:04:30.000000 h3ronpy-0.9.0/h3ronpy/raster.py
+-rw-rw-r--   0     1000     1000     1245 2021-04-09 19:04:30.000000 h3ronpy-0.9.0/h3ronpy/util.py
+-rw-rw-r--   0     1000     1000     3208 2021-04-09 19:04:30.000000 h3ronpy-0.9.0/h3ronpy/vector.py
+-rw-rw-r--   0     1000     1000       78 2021-04-11 18:27:47.000000 h3ronpy-0.9.0/pyproject.toml
+-rw-rw-r--   0     1000     1000       16 2021-04-11 17:31:34.000000 h3ronpy-0.9.0/requirements.dev.txt
+-rw-rw-r--   0     1000     1000       62 2021-03-05 18:52:26.000000 h3ronpy-0.9.0/requirements.documentation.txt
+-rw-rw-r--   0     1000     1000     1780 2021-04-09 19:12:10.000000 h3ronpy-0.9.0/src/collections.rs
+-rw-rw-r--   0     1000     1000     1458 2021-04-05 19:36:14.000000 h3ronpy-0.9.0/src/error.rs
+-rw-rw-r--   0     1000     1000     1057 2021-04-09 19:07:16.000000 h3ronpy-0.9.0/src/lib.rs
+-rw-rw-r--   0     1000     1000     2197 2021-04-09 19:10:54.000000 h3ronpy-0.9.0/src/polygon.rs
+-rw-rw-r--   0     1000     1000     5446 2021-04-09 19:04:30.000000 h3ronpy-0.9.0/src/raster.rs
+-rw-rw-r--   0     1000     1000     1535 2021-04-05 19:36:15.000000 h3ronpy-0.9.0/src/transform.rs
+-rw-rw-r--   0     1000     1000     2658 2021-04-09 19:13:17.000000 h3ronpy-0.9.0/src/vector.rs
+-rw-r--r--   0        0        0     3176 1970-01-01 00:00:00.000000 h3ronpy-0.9.0/PKG-INFO
```

### Comparing `h3ronpy-0.17.0/LICENSE.txt` & `h3ronpy-0.9.0/LICENSE.txt`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-Permission is hereby granted, free of charge, to any
-person obtaining a copy of this software and associated
-documentation files (the "Software"), to deal in the
-Software without restriction, including without
-limitation the rights to use, copy, modify, merge,
-publish, distribute, sublicense, and/or sell copies of
-the Software, and to permit persons to whom the Software
-is furnished to do so, subject to the following
-conditions:
-
-The above copyright notice and this permission notice
-shall be included in all copies or substantial portions
-of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF
-ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED
-TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A
-PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT
-SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY
-CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
-OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR
-IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
-DEALINGS IN THE SOFTWARE.
+Permission is hereby granted, free of charge, to any
+person obtaining a copy of this software and associated
+documentation files (the "Software"), to deal in the
+Software without restriction, including without
+limitation the rights to use, copy, modify, merge,
+publish, distribute, sublicense, and/or sell copies of
+the Software, and to permit persons to whom the Software
+is furnished to do so, subject to the following
+conditions:
+
+The above copyright notice and this permission notice
+shall be included in all copies or substantial portions
+of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF
+ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED
+TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A
+PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT
+SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY
+CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
+OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR
+IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
+DEALINGS IN THE SOFTWARE.
```

### Comparing `h3ronpy-0.17.0/h3ronpy/arrow/raster.py` & `h3ronpy-0.9.0/h3ronpy/raster.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,107 +1,117 @@
-"""
-Conversion of raster `numpy` arrays to H3 cells
-
-Resolution search modes
------------------------
-
-* "min_diff": chose the H3 resolution where the difference in the area of a pixel and the h3index is as small as possible.
-* "smaller_than_pixel":  chose the H3 resolution where the area of the h3index is smaller than the area of a pixel.
-
-"""
-
-from ..h3ronpy import raster
-from .. import DEFAULT_CELL_COLUMN_NAME
-import numpy as np
-import pyarrow as pa
-
-try:
-    # affine library is used by rasterio
-    import affine
-
-    __HAS_AFFINE_LIB = True
-except ImportError:
-    __HAS_AFFINE_LIB = False
-
-Transform = raster.Transform
-
-
-def _get_transform(t):
-    if isinstance(t, Transform):
-        return t
-    if __HAS_AFFINE_LIB:
-        if isinstance(t, affine.Affine):
-            return Transform.from_rasterio([t.a, t.b, t.c, t.d, t.e, t.f])
-    if type(t) in (list, tuple) and len(t) == 6:
-        # probably native gdal
-        return Transform.from_gdal(t)
-    raise ValueError("unsupported object for transform")
-
-
-def nearest_h3_resolution(shape, transform, axis_order="yx", search_mode="min_diff") -> int:
-    """
-    Find the H3 resolution closest to the size of a pixel in an array
-    of the given shape with the given transform
-
-    :param shape: dimensions of the 2d array
-    :param transform: the affine transformation
-    :param axis_order: axis order of the 2d array. Either "xy" or "yx"
-    :param search_mode: resolution search mode (see documentation of this module)
-    :return:
-    """
-    return raster.nearest_h3_resolution(shape, _get_transform(transform), axis_order, search_mode)
-
-
-def raster_to_dataframe(
-    in_raster: np.array,
-    transform,
-    h3_resolution: int,
-    nodata_value=None,
-    axis_order: str = "yx",
-    compact: bool = True,
-) -> pa.Table:
-    """
-    Convert a raster/array to a pandas `DataFrame` containing H3 cell indexes
-
-    This function is parallelized and uses the available CPUs by distributing tiles to a thread pool.
-
-    The input geometry must be in WGS84.
-
-    :param in_raster: Input 2D array
-    :param transform:  The affine transformation
-    :param nodata_value: The nodata value. For these cells of the array there will be no h3 indexes generated
-    :param axis_order: Axis order of the 2d array. Either "xy" or "yx"
-    :param h3_resolution: Target h3 resolution
-    :param compact: Return compacted h3 indexes (see H3 docs). This results in mixed H3 resolutions, but also can
-            reduce the amount of required memory.
-    :return: Tuple of arrow arrays
-    """
-
-    dtype = in_raster.dtype
-    func = None
-    if dtype == np.uint8:
-        func = raster.raster_to_h3_u8
-    elif dtype == np.int8:
-        func = raster.raster_to_h3_i8
-    elif dtype == np.uint16:
-        func = raster.raster_to_h3_u16
-    elif dtype == np.int16:
-        func = raster.raster_to_h3_i16
-    elif dtype == np.uint32:
-        func = raster.raster_to_h3_u32
-    elif dtype == np.int32:
-        func = raster.raster_to_h3_i32
-    elif dtype == np.uint64:
-        func = raster.raster_to_h3_u64
-    elif dtype == np.int64:
-        func = raster.raster_to_h3_i64
-    elif dtype == np.float32:
-        func = raster.raster_to_h3_f32
-    elif dtype == np.float64:
-        func = raster.raster_to_h3_f64
-    else:
-        raise NotImplementedError(f"no raster_to_h3 implementation for dtype {dtype.name}")
-
-    return pa.Table.from_arrays(
-        arrays=func(in_raster, _get_transform(transform), h3_resolution, axis_order, compact, nodata_value),
-        names=["value", DEFAULT_CELL_COLUMN_NAME],
-    )
+"""
+Conversion of raster numpy arrays to h3.
+
+Resolution search modes
+-----------------------
+
+* "min_diff": chose the h3 resolution where the difference in the area of a pixel and the h3index is as small as possible.
+* "smaller_than_pixel":  chose the h3 resolution where the area of the h3index is smaller than the area of a pixel.
+"""
+
+import geopandas as gp
+import h3.api.numpy_int as h3
+import numpy as np
+from shapely.geometry import Polygon
+
+import pandas as pd
+from .h3ronpy import raster
+from . import H3_CRS
+
+try:
+    # affine library is used by rasterio
+    import affine
+
+    __HAS_AFFINE_LIB = True
+except:
+    __HAS_AFFINE_LIB = False
+
+
+def _get_transform(t):
+    if isinstance(t, raster.Transform):
+        return t
+    if __HAS_AFFINE_LIB:
+        if isinstance(t, affine.Affine):
+            return raster.Transform.from_rasterio([t.a, t.b, t.c, t.d, t.e, t.f])
+    if type(t) in (list, tuple) and len(t) == 6:
+        # probably native gdal
+        return raster.Transform.from_gdal(t)
+    raise ValueError("unsupported object for transform")
+
+
+def nearest_h3_resolution(shape, transform, axis_order="yx", search_mode="min_diff"):
+    """
+    find the h3 resolution closed to the size of a pixel in an array
+    of the given shape with the given transform
+
+    :param shape: dimensions of the 2d array
+    :param transform: the affine transformation
+    :param axis_order: axis order of the 2d array. Either "xy" or "yx"
+    :param search_mode: resolution search mode (see documentation of this module)
+    :return:
+    """
+    return raster.nearest_h3_resolution(shape, _get_transform(transform), axis_order, search_mode)
+
+
+def raster_to_dataframe(in_raster: np.array, transform, h3_resolution: int, nodata_value=None, axis_order: str = "yx",
+                        compacted: bool = True, geo: bool = False):
+    """
+    convert a raster/array to a pandas dataframe containing H3 indexes
+
+    This function is parallelized and uses the available CPUs by distributing tiles to a thread pool.
+
+    The input geometry must be in WGS84.
+
+    :param in_raster: input 2-d array
+    :param transform:  the affine transformation
+    :param nodata_value: the nodata value. For these cells of the array there will be no h3 indexes generated
+    :param axis_order: axis order of the 2d array. Either "xy" or "yx"
+    :param h3_resolution: target h3 resolution
+    :param compacted: return compacted h3 indexes (see H3 docs)
+    :param geo: return a geopandas geodataframe with geometries. increases the memory usage.
+    :return: pandas dataframe or geodataframe
+    """
+
+    dtype = in_raster.dtype
+    func = None
+    if dtype == np.uint8:
+        func = raster.raster_to_h3_u8
+    elif dtype == np.int8:
+        func = raster.raster_to_h3_i8
+    elif dtype == np.uint16:
+        func = raster.raster_to_h3_u16
+    elif dtype == np.int16:
+        func = raster.raster_to_h3_i16
+    elif dtype == np.uint32:
+        func = raster.raster_to_h3_u32
+    elif dtype == np.int32:
+        func = raster.raster_to_h3_i32
+    elif dtype == np.uint64:
+        func = raster.raster_to_h3_u64
+    elif dtype == np.int64:
+        func = raster.raster_to_h3_i64
+    else:
+        raise NotImplementedError(f"no raster_to_h3 implementation for dtype {dtype.name}")
+
+    # print(func.__name__)
+    values, indexes = func(in_raster, _get_transform(transform), nodata_value, h3_resolution, axis_order, compacted)
+    if geo:
+        return gp.GeoDataFrame({
+            "h3index": indexes,
+            "value": values,
+            "geometry": [Polygon(h3.h3_to_geo_boundary(h, geo_json=True)) for h in np.nditer(indexes)],
+        }, crs=H3_CRS)
+    else:
+        return pd.DataFrame({
+            "h3index": indexes,
+            "value": values
+        })
+
+
+def raster_to_geodataframe(*a, **kw):
+    """
+    convert to a geodataframe
+
+    Uses the same parameters as array_to_dataframe
+    """
+    kw["geo"] = True
+    return raster_to_dataframe(*a, **kw)
```

