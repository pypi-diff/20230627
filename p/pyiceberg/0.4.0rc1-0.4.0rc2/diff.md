# Comparing `tmp/pyiceberg-0.4.0rc1.tar.gz` & `tmp/pyiceberg-0.4.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyiceberg-0.4.0rc1.tar", max compression
+gzip compressed data, was "pyiceberg-0.4.0rc2.tar", max compression
```

## Comparing `pyiceberg-0.4.0rc1.tar` & `pyiceberg-0.4.0rc2.tar`

### file list

```diff
@@ -1,121 +1,121 @@
--rw-r--r--   0        0        0    12548 2022-12-02 14:33:08.931249 pyiceberg-0.4.0rc1/LICENSE
--rw-r--r--   0        0        0     2063 2023-06-26 08:00:39.798947 pyiceberg-0.4.0rc1/Makefile
--rw-r--r--   0        0        0      251 2022-12-02 14:33:08.931589 pyiceberg-0.4.0rc1/NOTICE
--rw-r--r--   0        0        0     1218 2023-06-22 07:56:06.334404 pyiceberg-0.4.0rc1/README.md
--rw-r--r--   0        0        0       20 2023-04-26 09:54:47.766320 pyiceberg-0.4.0rc1/dev/.rat-excludes
--rw-r--r--   0        0        0     2975 2023-06-26 08:00:39.799351 pyiceberg-0.4.0rc1/dev/Dockerfile
--rwxr-xr-x   0        0        0     2529 2023-04-26 09:54:47.766490 pyiceberg-0.4.0rc1/dev/check-license
--rw-r--r--   0        0        0     1018 2023-05-11 18:59:33.655015 pyiceberg-0.4.0rc1/dev/docker-compose-azurite.yml
--rw-r--r--   0        0        0     2569 2023-05-11 18:59:33.655087 pyiceberg-0.4.0rc1/dev/docker-compose-integration.yml
--rw-r--r--   0        0        0     1626 2023-05-11 18:59:33.655176 pyiceberg-0.4.0rc1/dev/docker-compose.yml
--rwxr-xr-x   0        0        0      912 2023-06-26 08:00:39.799561 pyiceberg-0.4.0rc1/dev/entrypoint.sh
--rw-r--r--   0        0        0     5267 2023-06-26 08:00:39.799891 pyiceberg-0.4.0rc1/dev/provision.py
--rwxr-xr-x   0        0        0     1198 2023-04-26 09:54:47.766904 pyiceberg-0.4.0rc1/dev/run-azurite.sh
--rwxr-xr-x   0        0        0     1194 2023-04-26 09:54:47.766997 pyiceberg-0.4.0rc1/dev/run-minio.sh
--rw-r--r--   0        0        0     1526 2023-05-22 23:14:10.622990 pyiceberg-0.4.0rc1/dev/spark-defaults.conf
--rw-r--r--   0        0        0      808 2023-06-26 08:45:12.059730 pyiceberg-0.4.0rc1/pyiceberg/__init__.py
--rw-r--r--   0        0        0      785 2023-05-01 21:38:02.315613 pyiceberg-0.4.0rc1/pyiceberg/avro/__init__.py
--rw-r--r--   0        0        0     1684 2022-12-22 10:04:24.888689 pyiceberg-0.4.0rc1/pyiceberg/avro/codecs/__init__.py
--rw-r--r--   0        0        0     1621 2022-11-24 08:06:13.045660 pyiceberg-0.4.0rc1/pyiceberg/avro/codecs/bzip2.py
--rw-r--r--   0        0        0     1131 2022-11-24 08:06:13.045739 pyiceberg-0.4.0rc1/pyiceberg/avro/codecs/codec.py
--rw-r--r--   0        0        0     1416 2022-11-24 08:06:13.045844 pyiceberg-0.4.0rc1/pyiceberg/avro/codecs/deflate.py
--rw-r--r--   0        0        0     2702 2023-06-26 08:15:00.501668 pyiceberg-0.4.0rc1/pyiceberg/avro/codecs/snappy_codec.py
--rw-r--r--   0        0        0     2075 2022-11-24 08:06:13.045960 pyiceberg-0.4.0rc1/pyiceberg/avro/codecs/zstandard_codec.py
--rw-r--r--   0        0        0     7038 2023-06-26 08:15:00.501810 pyiceberg-0.4.0rc1/pyiceberg/avro/decoder.py
--rw-r--r--   0        0        0     6853 2023-06-26 08:15:00.501957 pyiceberg-0.4.0rc1/pyiceberg/avro/file.py
--rw-r--r--   0        0        0    11784 2023-06-26 08:15:00.502120 pyiceberg-0.4.0rc1/pyiceberg/avro/reader.py
--rw-r--r--   0        0        0    11684 2023-06-26 08:15:00.502294 pyiceberg-0.4.0rc1/pyiceberg/avro/resolver.py
--rw-r--r--   0        0        0    20398 2023-06-26 08:15:00.502502 pyiceberg-0.4.0rc1/pyiceberg/catalog/__init__.py
--rw-r--r--   0        0        0    30334 2023-06-26 08:15:00.502710 pyiceberg-0.4.0rc1/pyiceberg/catalog/dynamodb.py
--rw-r--r--   0        0        0    20916 2023-06-26 08:15:00.502909 pyiceberg-0.4.0rc1/pyiceberg/catalog/glue.py
--rw-r--r--   0        0        0    20256 2023-06-26 08:15:00.503111 pyiceberg-0.4.0rc1/pyiceberg/catalog/hive.py
--rw-r--r--   0        0        0     2998 2023-06-26 08:15:00.503214 pyiceberg-0.4.0rc1/pyiceberg/catalog/noop.py
--rw-r--r--   0        0        0    23422 2023-06-26 08:15:00.503400 pyiceberg-0.4.0rc1/pyiceberg/catalog/rest.py
--rw-r--r--   0        0        0      785 2022-11-24 08:06:42.281296 pyiceberg-0.4.0rc1/pyiceberg/cli/__init__.py
--rw-r--r--   0        0        0    12027 2023-06-26 08:15:00.503571 pyiceberg-0.4.0rc1/pyiceberg/cli/console.py
--rw-r--r--   0        0        0     7378 2023-06-26 08:15:00.503705 pyiceberg-0.4.0rc1/pyiceberg/cli/output.py
--rw-r--r--   0        0        0     9829 2023-06-26 08:15:00.503849 pyiceberg-0.4.0rc1/pyiceberg/conversions.py
--rw-r--r--   0        0        0     3085 2023-06-26 08:15:00.503993 pyiceberg-0.4.0rc1/pyiceberg/exceptions.py
--rw-r--r--   0        0        0    30678 2023-06-26 08:15:00.504186 pyiceberg-0.4.0rc1/pyiceberg/expressions/__init__.py
--rw-r--r--   0        0        0    21961 2023-06-26 08:15:00.504392 pyiceberg-0.4.0rc1/pyiceberg/expressions/literals.py
--rw-r--r--   0        0        0     7149 2023-06-26 08:15:00.504557 pyiceberg-0.4.0rc1/pyiceberg/expressions/parser.py
--rw-r--r--   0        0        0    55299 2023-06-26 08:15:00.504819 pyiceberg-0.4.0rc1/pyiceberg/expressions/visitors.py
--rw-r--r--   0        0        0     1198 2023-06-26 08:15:00.504963 pyiceberg-0.4.0rc1/pyiceberg/files.py
--rw-r--r--   0        0        0    11090 2023-06-26 08:15:00.505113 pyiceberg-0.4.0rc1/pyiceberg/io/__init__.py
--rw-r--r--   0        0        0    10733 2023-06-26 08:15:00.505296 pyiceberg-0.4.0rc1/pyiceberg/io/fsspec.py
--rw-r--r--   0        0        0     2574 2023-06-26 08:15:00.505452 pyiceberg-0.4.0rc1/pyiceberg/io/memory.py
--rw-r--r--   0        0        0    40921 2023-06-26 08:15:00.505736 pyiceberg-0.4.0rc1/pyiceberg/io/pyarrow.py
--rw-r--r--   0        0        0    13521 2023-06-26 08:15:00.505921 pyiceberg-0.4.0rc1/pyiceberg/manifest.py
--rw-r--r--   0        0        0     7881 2023-06-26 08:15:00.506092 pyiceberg-0.4.0rc1/pyiceberg/partitioning.py
--rw-r--r--   0        0        0    52797 2023-06-26 08:15:00.506544 pyiceberg-0.4.0rc1/pyiceberg/schema.py
--rw-r--r--   0        0        0     2940 2023-06-26 08:15:00.506763 pyiceberg-0.4.0rc1/pyiceberg/serializers.py
--rw-r--r--   0        0        0    28940 2023-06-26 08:15:00.507030 pyiceberg-0.4.0rc1/pyiceberg/table/__init__.py
--rw-r--r--   0        0        0    16674 2023-06-26 08:15:00.507242 pyiceberg-0.4.0rc1/pyiceberg/table/metadata.py
--rw-r--r--   0        0        0     1577 2023-06-26 08:15:00.507408 pyiceberg-0.4.0rc1/pyiceberg/table/refs.py
--rw-r--r--   0        0        0     5347 2023-06-26 08:15:00.507583 pyiceberg-0.4.0rc1/pyiceberg/table/snapshots.py
--rw-r--r--   0        0        0     6531 2023-06-26 08:15:00.507767 pyiceberg-0.4.0rc1/pyiceberg/table/sorting.py
--rw-r--r--   0        0        0    28318 2023-06-26 08:15:00.507997 pyiceberg-0.4.0rc1/pyiceberg/transforms.py
--rw-r--r--   0        0        0     6151 2023-06-26 08:15:00.508184 pyiceberg-0.4.0rc1/pyiceberg/typedef.py
--rw-r--r--   0        0        0    20264 2023-06-26 08:15:00.508392 pyiceberg-0.4.0rc1/pyiceberg/types.py
--rw-r--r--   0        0        0      785 2022-11-24 08:06:13.053196 pyiceberg-0.4.0rc1/pyiceberg/utils/__init__.py
--rw-r--r--   0        0        0     3245 2023-06-26 08:15:00.508561 pyiceberg-0.4.0rc1/pyiceberg/utils/bin_packing.py
--rw-r--r--   0        0        0     6471 2023-06-26 08:15:00.508702 pyiceberg-0.4.0rc1/pyiceberg/utils/config.py
--rw-r--r--   0        0        0     6405 2023-06-26 08:15:00.509030 pyiceberg-0.4.0rc1/pyiceberg/utils/datetime.py
--rw-r--r--   0        0        0     3111 2023-06-26 08:15:00.509180 pyiceberg-0.4.0rc1/pyiceberg/utils/decimal.py
--rw-r--r--   0        0        0     1862 2023-06-26 08:15:00.509307 pyiceberg-0.4.0rc1/pyiceberg/utils/deprecated.py
--rw-r--r--   0        0        0     1350 2023-06-26 08:15:00.509440 pyiceberg-0.4.0rc1/pyiceberg/utils/parsing.py
--rw-r--r--   0        0        0    17618 2023-06-26 08:15:00.509619 pyiceberg-0.4.0rc1/pyiceberg/utils/schema_conversion.py
--rw-r--r--   0        0        0     2140 2023-06-26 08:15:00.509772 pyiceberg-0.4.0rc1/pyiceberg/utils/singleton.py
--rw-r--r--   0        0        0     6836 2023-06-26 08:48:05.170801 pyiceberg-0.4.0rc1/pyproject.toml
--rw-r--r--   0        0        0     6551 2023-04-26 09:54:47.775757 pyiceberg-0.4.0rc1/tests/avro/test_decoder.py
--rw-r--r--   0        0        0     2008 2023-04-26 09:54:47.775847 pyiceberg-0.4.0rc1/tests/avro/test_file.py
--rw-r--r--   0        0        0    15116 2023-04-26 09:54:47.775997 pyiceberg-0.4.0rc1/tests/avro/test_reader.py
--rw-r--r--   0        0        0     8616 2023-06-26 08:00:39.817203 pyiceberg-0.4.0rc1/tests/avro/test_resolver.py
--rw-r--r--   0        0        0    11592 2023-06-26 08:15:00.510095 pyiceberg-0.4.0rc1/tests/catalog/integration_test_dynamodb.py
--rw-r--r--   0        0        0    11780 2023-06-26 08:15:00.510242 pyiceberg-0.4.0rc1/tests/catalog/integration_test_glue.py
--rw-r--r--   0        0        0    18074 2023-06-26 08:15:00.510401 pyiceberg-0.4.0rc1/tests/catalog/test_base.py
--rw-r--r--   0        0        0    20923 2023-05-01 21:45:18.704369 pyiceberg-0.4.0rc1/tests/catalog/test_dynamodb.py
--rw-r--r--   0        0        0    20601 2023-06-26 08:15:00.510587 pyiceberg-0.4.0rc1/tests/catalog/test_glue.py
--rw-r--r--   0        0        0    25678 2023-06-04 13:37:00.195421 pyiceberg-0.4.0rc1/tests/catalog/test_hive.py
--rw-r--r--   0        0        0    31137 2023-06-26 08:15:00.510936 pyiceberg-0.4.0rc1/tests/catalog/test_rest.py
--rw-r--r--   0        0        0    42591 2023-06-26 08:15:00.511189 pyiceberg-0.4.0rc1/tests/cli/test_console.py
--rw-r--r--   0        0        0      799 2022-12-02 14:33:08.938744 pyiceberg-0.4.0rc1/tests/cli/test_output.py
--rw-r--r--   0        0        0    61479 2023-06-26 08:15:00.511486 pyiceberg-0.4.0rc1/tests/conftest.py
--rw-r--r--   0        0        0    45204 2023-05-01 21:45:18.705300 pyiceberg-0.4.0rc1/tests/expressions/test_evaluator.py
--rw-r--r--   0        0        0    43602 2023-06-26 08:15:00.511722 pyiceberg-0.4.0rc1/tests/expressions/test_expressions.py
--rw-r--r--   0        0        0    25456 2023-05-01 21:45:18.705504 pyiceberg-0.4.0rc1/tests/expressions/test_literals.py
--rw-r--r--   0        0        0     5188 2023-05-01 21:45:18.705651 pyiceberg-0.4.0rc1/tests/expressions/test_parser.py
--rw-r--r--   0        0        0    12446 2023-04-26 09:54:47.778813 pyiceberg-0.4.0rc1/tests/expressions/test_projection.py
--rw-r--r--   0        0        0    64029 2023-06-26 08:00:39.820219 pyiceberg-0.4.0rc1/tests/expressions/test_visitors.py
--rw-r--r--   0        0        0    19528 2023-04-26 09:54:47.779721 pyiceberg-0.4.0rc1/tests/io/test_fsspec.py
--rw-r--r--   0        0        0    11456 2023-05-01 21:45:18.706178 pyiceberg-0.4.0rc1/tests/io/test_io.py
--rw-r--r--   0        0        0    44659 2023-06-26 08:15:00.511993 pyiceberg-0.4.0rc1/tests/io/test_pyarrow.py
--rw-r--r--   0        0        0    10762 2023-06-26 08:00:39.820673 pyiceberg-0.4.0rc1/tests/io/test_pyarrow_visitor.py
--rw-r--r--   0        0        0    12694 2023-06-26 08:15:00.512192 pyiceberg-0.4.0rc1/tests/table/test_init.py
--rw-r--r--   0        0        0    31242 2023-04-26 09:54:47.780462 pyiceberg-0.4.0rc1/tests/table/test_metadata.py
--rw-r--r--   0        0        0     5243 2023-04-26 09:54:47.780608 pyiceberg-0.4.0rc1/tests/table/test_partitioning.py
--rw-r--r--   0        0        0     1434 2023-04-26 09:54:47.780721 pyiceberg-0.4.0rc1/tests/table/test_refs.py
--rw-r--r--   0        0        0     4951 2023-04-26 09:54:47.780871 pyiceberg-0.4.0rc1/tests/table/test_snapshots.py
--rw-r--r--   0        0        0     4085 2023-04-26 09:54:47.780991 pyiceberg-0.4.0rc1/tests/table/test_sorting.py
--rw-r--r--   0        0        0    21467 2023-04-26 09:54:47.781149 pyiceberg-0.4.0rc1/tests/test_conversions.py
--rw-r--r--   0        0        0    10446 2023-06-26 08:15:00.512351 pyiceberg-0.4.0rc1/tests/test_integration.py
--rw-r--r--   0        0        0    27064 2023-04-26 09:54:47.781399 pyiceberg-0.4.0rc1/tests/test_schema.py
--rw-r--r--   0        0        0    33953 2023-06-26 08:00:39.822555 pyiceberg-0.4.0rc1/tests/test_transforms.py
--rw-r--r--   0        0        0     2567 2023-04-26 09:54:47.781682 pyiceberg-0.4.0rc1/tests/test_typedef.py
--rw-r--r--   0        0        0    18554 2023-06-26 08:15:00.512534 pyiceberg-0.4.0rc1/tests/test_types.py
--rw-r--r--   0        0        0     1113 2023-04-26 09:54:47.781968 pyiceberg-0.4.0rc1/tests/test_version.py
--rw-r--r--   0        0        0     2725 2023-06-26 08:00:39.822930 pyiceberg-0.4.0rc1/tests/utils/test_bin_packing.py
--rw-r--r--   0        0        0     2250 2023-06-26 08:00:39.823033 pyiceberg-0.4.0rc1/tests/utils/test_config.py
--rw-r--r--   0        0        0     1354 2023-04-26 09:54:47.782246 pyiceberg-0.4.0rc1/tests/utils/test_deprecated.py
--rw-r--r--   0        0        0     9312 2023-06-26 08:00:39.824675 pyiceberg-0.4.0rc1/tests/utils/test_manifest.py
--rw-r--r--   0        0        0    12321 2023-06-26 08:00:39.824976 pyiceberg-0.4.0rc1/tests/utils/test_schema_conversion.py
--rw-r--r--   0        0        0     1334 2023-04-26 09:54:47.782780 pyiceberg-0.4.0rc1/tests/utils/test_singleton.py
--rw-r--r--   0        0        0    74745 2022-12-02 14:33:08.946465 pyiceberg-0.4.0rc1/vendor/fb303/FacebookService.py
--rw-r--r--   0        0        0      853 2022-12-02 14:33:08.946568 pyiceberg-0.4.0rc1/vendor/fb303/__init__.py
--rw-r--r--   0        0        0      943 2022-12-02 14:33:08.946641 pyiceberg-0.4.0rc1/vendor/fb303/constants.py
--rw-r--r--   0        0        0     1549 2022-12-02 14:33:08.946707 pyiceberg-0.4.0rc1/vendor/fb303/ttypes.py
--rw-r--r--   0        0        0  2241478 2023-06-06 21:21:16.752393 pyiceberg-0.4.0rc1/vendor/hive_metastore/ThriftHiveMetastore.py
--rw-r--r--   0        0        0      856 2022-12-02 14:33:08.949446 pyiceberg-0.4.0rc1/vendor/hive_metastore/__init__.py
--rw-r--r--   0        0        0     2401 2022-12-02 14:33:08.949506 pyiceberg-0.4.0rc1/vendor/hive_metastore/constants.py
--rw-r--r--   0        0        0  1354270 2022-12-22 09:59:35.298067 pyiceberg-0.4.0rc1/vendor/hive_metastore/ttypes.py
--rw-r--r--   0        0        0     3295 1970-01-01 00:00:00.000000 pyiceberg-0.4.0rc1/PKG-INFO
+-rw-r--r--   0        0        0    12548 2022-12-02 14:33:08.931249 pyiceberg-0.4.0rc2/LICENSE
+-rw-r--r--   0        0        0     2063 2023-06-27 20:30:03.370406 pyiceberg-0.4.0rc2/Makefile
+-rw-r--r--   0        0        0      251 2022-12-02 14:33:08.931589 pyiceberg-0.4.0rc2/NOTICE
+-rw-r--r--   0        0        0     1218 2023-06-27 19:47:54.157949 pyiceberg-0.4.0rc2/README.md
+-rw-r--r--   0        0        0       20 2023-04-26 09:54:47.766320 pyiceberg-0.4.0rc2/dev/.rat-excludes
+-rw-r--r--   0        0        0     2975 2023-06-26 08:00:39.799351 pyiceberg-0.4.0rc2/dev/Dockerfile
+-rwxr-xr-x   0        0        0     2529 2023-04-26 09:54:47.766490 pyiceberg-0.4.0rc2/dev/check-license
+-rw-r--r--   0        0        0     1018 2023-05-11 18:59:33.655015 pyiceberg-0.4.0rc2/dev/docker-compose-azurite.yml
+-rw-r--r--   0        0        0     2569 2023-06-27 20:30:03.370530 pyiceberg-0.4.0rc2/dev/docker-compose-integration.yml
+-rw-r--r--   0        0        0     1626 2023-05-11 18:59:33.655176 pyiceberg-0.4.0rc2/dev/docker-compose.yml
+-rwxr-xr-x   0        0        0      912 2023-06-26 08:00:39.799561 pyiceberg-0.4.0rc2/dev/entrypoint.sh
+-rw-r--r--   0        0        0     5267 2023-06-26 08:00:39.799891 pyiceberg-0.4.0rc2/dev/provision.py
+-rwxr-xr-x   0        0        0     1198 2023-04-26 09:54:47.766904 pyiceberg-0.4.0rc2/dev/run-azurite.sh
+-rwxr-xr-x   0        0        0     1194 2023-04-26 09:54:47.766997 pyiceberg-0.4.0rc2/dev/run-minio.sh
+-rw-r--r--   0        0        0     1526 2023-05-22 23:14:10.622990 pyiceberg-0.4.0rc2/dev/spark-defaults.conf
+-rw-r--r--   0        0        0      808 2023-06-27 20:30:03.372670 pyiceberg-0.4.0rc2/pyiceberg/__init__.py
+-rw-r--r--   0        0        0      785 2023-05-01 21:38:02.315613 pyiceberg-0.4.0rc2/pyiceberg/avro/__init__.py
+-rw-r--r--   0        0        0     1684 2022-12-22 10:04:24.888689 pyiceberg-0.4.0rc2/pyiceberg/avro/codecs/__init__.py
+-rw-r--r--   0        0        0     1621 2022-11-24 08:06:13.045660 pyiceberg-0.4.0rc2/pyiceberg/avro/codecs/bzip2.py
+-rw-r--r--   0        0        0     1131 2022-11-24 08:06:13.045739 pyiceberg-0.4.0rc2/pyiceberg/avro/codecs/codec.py
+-rw-r--r--   0        0        0     1416 2022-11-24 08:06:13.045844 pyiceberg-0.4.0rc2/pyiceberg/avro/codecs/deflate.py
+-rw-r--r--   0        0        0     2702 2023-06-26 08:15:00.501668 pyiceberg-0.4.0rc2/pyiceberg/avro/codecs/snappy_codec.py
+-rw-r--r--   0        0        0     2075 2022-11-24 08:06:13.045960 pyiceberg-0.4.0rc2/pyiceberg/avro/codecs/zstandard_codec.py
+-rw-r--r--   0        0        0     7038 2023-06-26 08:15:00.501810 pyiceberg-0.4.0rc2/pyiceberg/avro/decoder.py
+-rw-r--r--   0        0        0     6853 2023-06-27 20:30:03.373080 pyiceberg-0.4.0rc2/pyiceberg/avro/file.py
+-rw-r--r--   0        0        0    11784 2023-06-27 20:30:03.373385 pyiceberg-0.4.0rc2/pyiceberg/avro/reader.py
+-rw-r--r--   0        0        0    11684 2023-06-26 08:15:00.502294 pyiceberg-0.4.0rc2/pyiceberg/avro/resolver.py
+-rw-r--r--   0        0        0    20398 2023-06-27 20:30:03.374051 pyiceberg-0.4.0rc2/pyiceberg/catalog/__init__.py
+-rw-r--r--   0        0        0    30334 2023-06-27 20:30:03.374444 pyiceberg-0.4.0rc2/pyiceberg/catalog/dynamodb.py
+-rw-r--r--   0        0        0    20916 2023-06-27 20:30:03.374780 pyiceberg-0.4.0rc2/pyiceberg/catalog/glue.py
+-rw-r--r--   0        0        0    20256 2023-06-27 20:30:03.374998 pyiceberg-0.4.0rc2/pyiceberg/catalog/hive.py
+-rw-r--r--   0        0        0     2998 2023-06-27 20:30:03.377261 pyiceberg-0.4.0rc2/pyiceberg/catalog/noop.py
+-rw-r--r--   0        0        0    23422 2023-06-27 20:30:03.377489 pyiceberg-0.4.0rc2/pyiceberg/catalog/rest.py
+-rw-r--r--   0        0        0      785 2022-11-24 08:06:42.281296 pyiceberg-0.4.0rc2/pyiceberg/cli/__init__.py
+-rw-r--r--   0        0        0    12027 2023-06-26 08:15:00.503571 pyiceberg-0.4.0rc2/pyiceberg/cli/console.py
+-rw-r--r--   0        0        0     7378 2023-06-26 08:15:00.503705 pyiceberg-0.4.0rc2/pyiceberg/cli/output.py
+-rw-r--r--   0        0        0     9829 2023-06-26 08:15:00.503849 pyiceberg-0.4.0rc2/pyiceberg/conversions.py
+-rw-r--r--   0        0        0     3085 2023-06-27 20:30:03.377998 pyiceberg-0.4.0rc2/pyiceberg/exceptions.py
+-rw-r--r--   0        0        0    30678 2023-06-27 20:30:03.378344 pyiceberg-0.4.0rc2/pyiceberg/expressions/__init__.py
+-rw-r--r--   0        0        0    21961 2023-06-27 20:30:03.378574 pyiceberg-0.4.0rc2/pyiceberg/expressions/literals.py
+-rw-r--r--   0        0        0     7149 2023-06-26 08:15:00.504557 pyiceberg-0.4.0rc2/pyiceberg/expressions/parser.py
+-rw-r--r--   0        0        0    55299 2023-06-26 08:15:00.504819 pyiceberg-0.4.0rc2/pyiceberg/expressions/visitors.py
+-rw-r--r--   0        0        0     1198 2023-06-26 08:15:00.504963 pyiceberg-0.4.0rc2/pyiceberg/files.py
+-rw-r--r--   0        0        0    11090 2023-06-27 20:30:03.378724 pyiceberg-0.4.0rc2/pyiceberg/io/__init__.py
+-rw-r--r--   0        0        0    10733 2023-06-26 08:15:00.505296 pyiceberg-0.4.0rc2/pyiceberg/io/fsspec.py
+-rw-r--r--   0        0        0     2574 2023-06-27 20:30:03.378892 pyiceberg-0.4.0rc2/pyiceberg/io/memory.py
+-rw-r--r--   0        0        0    40921 2023-06-27 20:30:03.379150 pyiceberg-0.4.0rc2/pyiceberg/io/pyarrow.py
+-rw-r--r--   0        0        0    13521 2023-06-27 20:30:03.379655 pyiceberg-0.4.0rc2/pyiceberg/manifest.py
+-rw-r--r--   0        0        0     7881 2023-06-27 20:30:03.379843 pyiceberg-0.4.0rc2/pyiceberg/partitioning.py
+-rw-r--r--   0        0        0    52797 2023-06-27 20:30:03.380224 pyiceberg-0.4.0rc2/pyiceberg/schema.py
+-rw-r--r--   0        0        0     2940 2023-06-26 08:15:00.506763 pyiceberg-0.4.0rc2/pyiceberg/serializers.py
+-rw-r--r--   0        0        0    28940 2023-06-27 20:30:03.380621 pyiceberg-0.4.0rc2/pyiceberg/table/__init__.py
+-rw-r--r--   0        0        0    16674 2023-06-26 08:15:00.507242 pyiceberg-0.4.0rc2/pyiceberg/table/metadata.py
+-rw-r--r--   0        0        0     1577 2023-06-27 20:30:03.380778 pyiceberg-0.4.0rc2/pyiceberg/table/refs.py
+-rw-r--r--   0        0        0     5347 2023-06-27 20:30:03.380948 pyiceberg-0.4.0rc2/pyiceberg/table/snapshots.py
+-rw-r--r--   0        0        0     6531 2023-06-27 20:30:03.381116 pyiceberg-0.4.0rc2/pyiceberg/table/sorting.py
+-rw-r--r--   0        0        0    28318 2023-06-27 20:30:03.381394 pyiceberg-0.4.0rc2/pyiceberg/transforms.py
+-rw-r--r--   0        0        0     6151 2023-06-27 20:30:03.381578 pyiceberg-0.4.0rc2/pyiceberg/typedef.py
+-rw-r--r--   0        0        0    20264 2023-06-27 20:30:03.381874 pyiceberg-0.4.0rc2/pyiceberg/types.py
+-rw-r--r--   0        0        0      785 2022-11-24 08:06:13.053196 pyiceberg-0.4.0rc2/pyiceberg/utils/__init__.py
+-rw-r--r--   0        0        0     3245 2023-06-27 20:30:03.382083 pyiceberg-0.4.0rc2/pyiceberg/utils/bin_packing.py
+-rw-r--r--   0        0        0     6471 2023-06-26 08:15:00.508702 pyiceberg-0.4.0rc2/pyiceberg/utils/config.py
+-rw-r--r--   0        0        0     6405 2023-06-26 08:15:00.509030 pyiceberg-0.4.0rc2/pyiceberg/utils/datetime.py
+-rw-r--r--   0        0        0     3111 2023-06-26 08:15:00.509180 pyiceberg-0.4.0rc2/pyiceberg/utils/decimal.py
+-rw-r--r--   0        0        0     1862 2023-06-26 08:15:00.509307 pyiceberg-0.4.0rc2/pyiceberg/utils/deprecated.py
+-rw-r--r--   0        0        0     1350 2023-06-26 08:15:00.509440 pyiceberg-0.4.0rc2/pyiceberg/utils/parsing.py
+-rw-r--r--   0        0        0    17618 2023-06-27 20:30:03.382289 pyiceberg-0.4.0rc2/pyiceberg/utils/schema_conversion.py
+-rw-r--r--   0        0        0     2140 2023-06-26 08:15:00.509772 pyiceberg-0.4.0rc2/pyiceberg/utils/singleton.py
+-rw-r--r--   0        0        0     6836 2023-06-27 20:31:47.553392 pyiceberg-0.4.0rc2/pyproject.toml
+-rw-r--r--   0        0        0     6551 2023-04-26 09:54:47.775757 pyiceberg-0.4.0rc2/tests/avro/test_decoder.py
+-rw-r--r--   0        0        0     2008 2023-04-26 09:54:47.775847 pyiceberg-0.4.0rc2/tests/avro/test_file.py
+-rw-r--r--   0        0        0    15116 2023-04-26 09:54:47.775997 pyiceberg-0.4.0rc2/tests/avro/test_reader.py
+-rw-r--r--   0        0        0     8616 2023-06-26 08:00:39.817203 pyiceberg-0.4.0rc2/tests/avro/test_resolver.py
+-rw-r--r--   0        0        0    11592 2023-06-26 08:15:00.510095 pyiceberg-0.4.0rc2/tests/catalog/integration_test_dynamodb.py
+-rw-r--r--   0        0        0    11780 2023-06-26 08:15:00.510242 pyiceberg-0.4.0rc2/tests/catalog/integration_test_glue.py
+-rw-r--r--   0        0        0    18074 2023-06-27 20:30:03.382826 pyiceberg-0.4.0rc2/tests/catalog/test_base.py
+-rw-r--r--   0        0        0    20923 2023-05-01 21:45:18.704369 pyiceberg-0.4.0rc2/tests/catalog/test_dynamodb.py
+-rw-r--r--   0        0        0    20601 2023-06-26 08:15:00.510587 pyiceberg-0.4.0rc2/tests/catalog/test_glue.py
+-rw-r--r--   0        0        0    25678 2023-06-04 13:37:00.195421 pyiceberg-0.4.0rc2/tests/catalog/test_hive.py
+-rw-r--r--   0        0        0    31137 2023-06-27 20:30:03.383010 pyiceberg-0.4.0rc2/tests/catalog/test_rest.py
+-rw-r--r--   0        0        0    42591 2023-06-27 20:30:03.383273 pyiceberg-0.4.0rc2/tests/cli/test_console.py
+-rw-r--r--   0        0        0      799 2022-12-02 14:33:08.938744 pyiceberg-0.4.0rc2/tests/cli/test_output.py
+-rw-r--r--   0        0        0    61479 2023-06-27 20:30:03.383695 pyiceberg-0.4.0rc2/tests/conftest.py
+-rw-r--r--   0        0        0    45204 2023-05-01 21:45:18.705300 pyiceberg-0.4.0rc2/tests/expressions/test_evaluator.py
+-rw-r--r--   0        0        0    43602 2023-06-26 08:15:00.511722 pyiceberg-0.4.0rc2/tests/expressions/test_expressions.py
+-rw-r--r--   0        0        0    25456 2023-05-01 21:45:18.705504 pyiceberg-0.4.0rc2/tests/expressions/test_literals.py
+-rw-r--r--   0        0        0     5450 2023-06-27 20:30:08.169894 pyiceberg-0.4.0rc2/tests/expressions/test_parser.py
+-rw-r--r--   0        0        0    12446 2023-04-26 09:54:47.778813 pyiceberg-0.4.0rc2/tests/expressions/test_projection.py
+-rw-r--r--   0        0        0    64029 2023-06-26 08:00:39.820219 pyiceberg-0.4.0rc2/tests/expressions/test_visitors.py
+-rw-r--r--   0        0        0    19528 2023-04-26 09:54:47.779721 pyiceberg-0.4.0rc2/tests/io/test_fsspec.py
+-rw-r--r--   0        0        0    11456 2023-05-01 21:45:18.706178 pyiceberg-0.4.0rc2/tests/io/test_io.py
+-rw-r--r--   0        0        0    44659 2023-06-27 20:30:03.384460 pyiceberg-0.4.0rc2/tests/io/test_pyarrow.py
+-rw-r--r--   0        0        0    10762 2023-06-26 08:00:39.820673 pyiceberg-0.4.0rc2/tests/io/test_pyarrow_visitor.py
+-rw-r--r--   0        0        0    12694 2023-06-27 20:30:03.384868 pyiceberg-0.4.0rc2/tests/table/test_init.py
+-rw-r--r--   0        0        0    31242 2023-04-26 09:54:47.780462 pyiceberg-0.4.0rc2/tests/table/test_metadata.py
+-rw-r--r--   0        0        0     5243 2023-04-26 09:54:47.780608 pyiceberg-0.4.0rc2/tests/table/test_partitioning.py
+-rw-r--r--   0        0        0     1434 2023-04-26 09:54:47.780721 pyiceberg-0.4.0rc2/tests/table/test_refs.py
+-rw-r--r--   0        0        0     4951 2023-04-26 09:54:47.780871 pyiceberg-0.4.0rc2/tests/table/test_snapshots.py
+-rw-r--r--   0        0        0     4085 2023-04-26 09:54:47.780991 pyiceberg-0.4.0rc2/tests/table/test_sorting.py
+-rw-r--r--   0        0        0    21467 2023-04-26 09:54:47.781149 pyiceberg-0.4.0rc2/tests/test_conversions.py
+-rw-r--r--   0        0        0    10446 2023-06-27 20:30:03.385134 pyiceberg-0.4.0rc2/tests/test_integration.py
+-rw-r--r--   0        0        0    27064 2023-04-26 09:54:47.781399 pyiceberg-0.4.0rc2/tests/test_schema.py
+-rw-r--r--   0        0        0    33953 2023-06-26 08:00:39.822555 pyiceberg-0.4.0rc2/tests/test_transforms.py
+-rw-r--r--   0        0        0     2567 2023-04-26 09:54:47.781682 pyiceberg-0.4.0rc2/tests/test_typedef.py
+-rw-r--r--   0        0        0    18554 2023-06-26 08:15:00.512534 pyiceberg-0.4.0rc2/tests/test_types.py
+-rw-r--r--   0        0        0     1113 2023-04-26 09:54:47.781968 pyiceberg-0.4.0rc2/tests/test_version.py
+-rw-r--r--   0        0        0     2725 2023-06-26 08:00:39.822930 pyiceberg-0.4.0rc2/tests/utils/test_bin_packing.py
+-rw-r--r--   0        0        0     2250 2023-06-26 08:00:39.823033 pyiceberg-0.4.0rc2/tests/utils/test_config.py
+-rw-r--r--   0        0        0     1354 2023-04-26 09:54:47.782246 pyiceberg-0.4.0rc2/tests/utils/test_deprecated.py
+-rw-r--r--   0        0        0     9312 2023-06-26 08:00:39.824675 pyiceberg-0.4.0rc2/tests/utils/test_manifest.py
+-rw-r--r--   0        0        0    12321 2023-06-26 08:00:39.824976 pyiceberg-0.4.0rc2/tests/utils/test_schema_conversion.py
+-rw-r--r--   0        0        0     1334 2023-04-26 09:54:47.782780 pyiceberg-0.4.0rc2/tests/utils/test_singleton.py
+-rw-r--r--   0        0        0    74745 2022-12-02 14:33:08.946465 pyiceberg-0.4.0rc2/vendor/fb303/FacebookService.py
+-rw-r--r--   0        0        0      853 2022-12-02 14:33:08.946568 pyiceberg-0.4.0rc2/vendor/fb303/__init__.py
+-rw-r--r--   0        0        0      943 2022-12-02 14:33:08.946641 pyiceberg-0.4.0rc2/vendor/fb303/constants.py
+-rw-r--r--   0        0        0     1549 2022-12-02 14:33:08.946707 pyiceberg-0.4.0rc2/vendor/fb303/ttypes.py
+-rw-r--r--   0        0        0  2241478 2023-06-06 21:21:16.752393 pyiceberg-0.4.0rc2/vendor/hive_metastore/ThriftHiveMetastore.py
+-rw-r--r--   0        0        0      856 2022-12-02 14:33:08.949446 pyiceberg-0.4.0rc2/vendor/hive_metastore/__init__.py
+-rw-r--r--   0        0        0     2401 2022-12-02 14:33:08.949506 pyiceberg-0.4.0rc2/vendor/hive_metastore/constants.py
+-rw-r--r--   0        0        0  1354270 2022-12-22 09:59:35.298067 pyiceberg-0.4.0rc2/vendor/hive_metastore/ttypes.py
+-rw-r--r--   0        0        0     3295 1970-01-01 00:00:00.000000 pyiceberg-0.4.0rc2/PKG-INFO
```

### Comparing `pyiceberg-0.4.0rc1/LICENSE` & `pyiceberg-0.4.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.4.0rc1/Makefile` & `pyiceberg-0.4.0rc2/Makefile`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.4.0rc1/README.md` & `pyiceberg-0.4.0rc2/README.md`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.4.0rc1/dev/Dockerfile` & `pyiceberg-0.4.0rc2/dev/Dockerfile`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.4.0rc1/dev/check-license` & `pyiceberg-0.4.0rc2/dev/check-license`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.4.0rc1/dev/docker-compose-azurite.yml` & `pyiceberg-0.4.0rc2/dev/docker-compose-azurite.yml`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.4.0rc1/dev/docker-compose-integration.yml` & `pyiceberg-0.4.0rc2/dev/docker-compose-integration.yml`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.4.0rc1/dev/docker-compose.yml` & `pyiceberg-0.4.0rc2/dev/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.4.0rc1/dev/entrypoint.sh` & `pyiceberg-0.4.0rc2/dev/entrypoint.sh`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.4.0rc1/dev/provision.py` & `pyiceberg-0.4.0rc2/dev/provision.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.4.0rc1/dev/run-azurite.sh` & `pyiceberg-0.4.0rc2/dev/run-azurite.sh`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.4.0rc1/dev/run-minio.sh` & `pyiceberg-0.4.0rc2/dev/run-minio.sh`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.4.0rc1/dev/spark-defaults.conf` & `pyiceberg-0.4.0rc2/dev/spark-defaults.conf`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.4.0rc1/pyiceberg/__init__.py` & `pyiceberg-0.4.0rc2/pyiceberg/__init__.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.4.0rc1/pyiceberg/avro/__init__.py` & `pyiceberg-0.4.0rc2/pyiceberg/avro/__init__.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.4.0rc1/pyiceberg/avro/codecs/__init__.py` & `pyiceberg-0.4.0rc2/pyiceberg/avro/codecs/__init__.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.4.0rc1/pyiceberg/avro/codecs/bzip2.py` & `pyiceberg-0.4.0rc2/pyiceberg/avro/codecs/bzip2.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.4.0rc1/pyiceberg/avro/codecs/codec.py` & `pyiceberg-0.4.0rc2/pyiceberg/avro/codecs/codec.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.4.0rc1/pyiceberg/avro/codecs/deflate.py` & `pyiceberg-0.4.0rc2/pyiceberg/avro/codecs/deflate.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.4.0rc1/pyiceberg/avro/codecs/snappy_codec.py` & `pyiceberg-0.4.0rc2/pyiceberg/avro/codecs/snappy_codec.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.4.0rc1/pyiceberg/avro/codecs/zstandard_codec.py` & `pyiceberg-0.4.0rc2/pyiceberg/avro/codecs/zstandard_codec.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.4.0rc1/pyiceberg/avro/decoder.py` & `pyiceberg-0.4.0rc2/pyiceberg/avro/decoder.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.4.0rc1/pyiceberg/avro/file.py` & `pyiceberg-0.4.0rc2/pyiceberg/avro/file.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.4.0rc1/pyiceberg/avro/reader.py` & `pyiceberg-0.4.0rc2/pyiceberg/avro/reader.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.4.0rc1/pyiceberg/avro/resolver.py` & `pyiceberg-0.4.0rc2/pyiceberg/avro/resolver.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.4.0rc1/pyiceberg/catalog/__init__.py` & `pyiceberg-0.4.0rc2/pyiceberg/catalog/__init__.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.4.0rc1/pyiceberg/catalog/dynamodb.py` & `pyiceberg-0.4.0rc2/pyiceberg/catalog/dynamodb.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.4.0rc1/pyiceberg/catalog/glue.py` & `pyiceberg-0.4.0rc2/pyiceberg/catalog/glue.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.4.0rc1/pyiceberg/catalog/hive.py` & `pyiceberg-0.4.0rc2/pyiceberg/catalog/hive.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.4.0rc1/pyiceberg/catalog/noop.py` & `pyiceberg-0.4.0rc2/pyiceberg/catalog/noop.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.4.0rc1/pyiceberg/catalog/rest.py` & `pyiceberg-0.4.0rc2/pyiceberg/catalog/rest.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.4.0rc1/pyiceberg/cli/__init__.py` & `pyiceberg-0.4.0rc2/pyiceberg/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.4.0rc1/pyiceberg/cli/console.py` & `pyiceberg-0.4.0rc2/pyiceberg/cli/console.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.4.0rc1/pyiceberg/cli/output.py` & `pyiceberg-0.4.0rc2/pyiceberg/cli/output.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.4.0rc1/pyiceberg/conversions.py` & `pyiceberg-0.4.0rc2/pyiceberg/conversions.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.4.0rc1/pyiceberg/exceptions.py` & `pyiceberg-0.4.0rc2/pyiceberg/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.4.0rc1/pyiceberg/expressions/__init__.py` & `pyiceberg-0.4.0rc2/pyiceberg/expressions/__init__.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.4.0rc1/pyiceberg/expressions/literals.py` & `pyiceberg-0.4.0rc2/pyiceberg/expressions/literals.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.4.0rc1/pyiceberg/expressions/parser.py` & `pyiceberg-0.4.0rc2/pyiceberg/expressions/parser.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.4.0rc1/pyiceberg/expressions/visitors.py` & `pyiceberg-0.4.0rc2/pyiceberg/expressions/visitors.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.4.0rc1/pyiceberg/files.py` & `pyiceberg-0.4.0rc2/pyiceberg/files.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.4.0rc1/pyiceberg/io/__init__.py` & `pyiceberg-0.4.0rc2/pyiceberg/io/__init__.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.4.0rc1/pyiceberg/io/fsspec.py` & `pyiceberg-0.4.0rc2/pyiceberg/io/fsspec.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.4.0rc1/pyiceberg/io/memory.py` & `pyiceberg-0.4.0rc2/pyiceberg/io/memory.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.4.0rc1/pyiceberg/io/pyarrow.py` & `pyiceberg-0.4.0rc2/pyiceberg/io/pyarrow.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.4.0rc1/pyiceberg/manifest.py` & `pyiceberg-0.4.0rc2/pyiceberg/manifest.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.4.0rc1/pyiceberg/partitioning.py` & `pyiceberg-0.4.0rc2/pyiceberg/partitioning.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.4.0rc1/pyiceberg/schema.py` & `pyiceberg-0.4.0rc2/pyiceberg/schema.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.4.0rc1/pyiceberg/serializers.py` & `pyiceberg-0.4.0rc2/pyiceberg/serializers.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.4.0rc1/pyiceberg/table/__init__.py` & `pyiceberg-0.4.0rc2/pyiceberg/table/__init__.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.4.0rc1/pyiceberg/table/metadata.py` & `pyiceberg-0.4.0rc2/pyiceberg/table/metadata.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.4.0rc1/pyiceberg/table/refs.py` & `pyiceberg-0.4.0rc2/pyiceberg/table/refs.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.4.0rc1/pyiceberg/table/snapshots.py` & `pyiceberg-0.4.0rc2/pyiceberg/table/snapshots.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.4.0rc1/pyiceberg/table/sorting.py` & `pyiceberg-0.4.0rc2/pyiceberg/table/sorting.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.4.0rc1/pyiceberg/transforms.py` & `pyiceberg-0.4.0rc2/pyiceberg/transforms.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.4.0rc1/pyiceberg/typedef.py` & `pyiceberg-0.4.0rc2/pyiceberg/typedef.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.4.0rc1/pyiceberg/types.py` & `pyiceberg-0.4.0rc2/pyiceberg/types.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.4.0rc1/pyiceberg/utils/__init__.py` & `pyiceberg-0.4.0rc2/pyiceberg/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.4.0rc1/pyiceberg/utils/bin_packing.py` & `pyiceberg-0.4.0rc2/pyiceberg/utils/bin_packing.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.4.0rc1/pyiceberg/utils/config.py` & `pyiceberg-0.4.0rc2/pyiceberg/utils/config.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.4.0rc1/pyiceberg/utils/datetime.py` & `pyiceberg-0.4.0rc2/pyiceberg/utils/datetime.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.4.0rc1/pyiceberg/utils/decimal.py` & `pyiceberg-0.4.0rc2/pyiceberg/utils/decimal.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.4.0rc1/pyiceberg/utils/deprecated.py` & `pyiceberg-0.4.0rc2/pyiceberg/utils/deprecated.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.4.0rc1/pyiceberg/utils/parsing.py` & `pyiceberg-0.4.0rc2/pyiceberg/utils/parsing.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.4.0rc1/pyiceberg/utils/schema_conversion.py` & `pyiceberg-0.4.0rc2/pyiceberg/utils/schema_conversion.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.4.0rc1/pyiceberg/utils/singleton.py` & `pyiceberg-0.4.0rc2/pyiceberg/utils/singleton.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.4.0rc1/pyproject.toml` & `pyiceberg-0.4.0rc2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 [tool.poetry]
 name = "pyiceberg"
-version = "0.4.0rc1"
+version = "0.4.0rc2"
 readme = "README.md"
 homepage = "https://iceberg.apache.org/"
 repository = "https://github.com/apache/iceberg/"
 description = "Apache Iceberg is an open table format for huge analytic datasets"
 authors = ["Apache Software Foundation <dev@iceberg.apache.org>"]
 license = "Apache License 2.0"
 classifiers = [
@@ -47,15 +47,15 @@
 requests = ">=2.20.0,<3.0.0"
 click = ">=7.1.1,<9.0.0"
 rich = ">=10.11.0,<14.0.0"
 strictyaml = ">=1.7.0,<2.0.0" # CVE-2020-14343 was fixed in 5.4.
 pydantic = ">=1.9.0,<2.0.0"
 sortedcontainers = "2.4.0"
 fsspec = ">=2021.09.0,<2024.1.0" # `lexists()` was implemented in 2021.09.0. Upper bound set arbitrarily, to be reassessed in early 2024.
-pyparsing = ">=3.0.7,<4.0.0" # The `min` keyword argument for `delimited_list()` was added in 3.0.7.
+pyparsing = ">=3.0.7,<3.1.0" # The `min` keyword argument for `delimited_list()` was added in 3.0.7.
 zstandard = ">=0.13.0,<1.0.0"
 pyarrow = { version = ">=9.0.0,<13.0.0", optional = true }
 pandas = { version = ">=1.0.0,<3.0.0", optional = true }
 duckdb = { version = ">=0.5.0,<1.0.0", optional = true }
 ray = { version = ">=2.0.0,<3.0.0", optional = true }
 python-snappy = { version = ">=0.6.0,<1.0.0", optional = true }
 thrift = { version = ">=0.13.0,<1.0.0", optional = true }
```

### Comparing `pyiceberg-0.4.0rc1/tests/avro/test_decoder.py` & `pyiceberg-0.4.0rc2/tests/avro/test_decoder.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.4.0rc1/tests/avro/test_file.py` & `pyiceberg-0.4.0rc2/tests/avro/test_file.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.4.0rc1/tests/avro/test_reader.py` & `pyiceberg-0.4.0rc2/tests/avro/test_reader.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.4.0rc1/tests/avro/test_resolver.py` & `pyiceberg-0.4.0rc2/tests/avro/test_resolver.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.4.0rc1/tests/catalog/integration_test_dynamodb.py` & `pyiceberg-0.4.0rc2/tests/catalog/integration_test_dynamodb.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.4.0rc1/tests/catalog/integration_test_glue.py` & `pyiceberg-0.4.0rc2/tests/catalog/integration_test_glue.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.4.0rc1/tests/catalog/test_base.py` & `pyiceberg-0.4.0rc2/tests/catalog/test_base.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.4.0rc1/tests/catalog/test_dynamodb.py` & `pyiceberg-0.4.0rc2/tests/catalog/test_dynamodb.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.4.0rc1/tests/catalog/test_glue.py` & `pyiceberg-0.4.0rc2/tests/catalog/test_glue.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.4.0rc1/tests/catalog/test_hive.py` & `pyiceberg-0.4.0rc2/tests/catalog/test_hive.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.4.0rc1/tests/catalog/test_rest.py` & `pyiceberg-0.4.0rc2/tests/catalog/test_rest.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.4.0rc1/tests/cli/test_console.py` & `pyiceberg-0.4.0rc2/tests/cli/test_console.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.4.0rc1/tests/cli/test_output.py` & `pyiceberg-0.4.0rc2/tests/cli/test_output.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.4.0rc1/tests/conftest.py` & `pyiceberg-0.4.0rc2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.4.0rc1/tests/expressions/test_evaluator.py` & `pyiceberg-0.4.0rc2/tests/expressions/test_evaluator.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.4.0rc1/tests/expressions/test_expressions.py` & `pyiceberg-0.4.0rc2/tests/expressions/test_expressions.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.4.0rc1/tests/expressions/test_literals.py` & `pyiceberg-0.4.0rc2/tests/expressions/test_literals.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.4.0rc1/tests/expressions/test_parser.py` & `pyiceberg-0.4.0rc2/tests/expressions/test_parser.py`

 * *Files 20% similar despite different names*

```diff
@@ -46,116 +46,122 @@
 
 
 def test_false() -> None:
     assert AlwaysFalse() == parser.parse("false")
 
 
 def test_is_null() -> None:
-    assert IsNull("x") == parser.parse("x is null")
-    assert IsNull("x") == parser.parse("x IS NULL")
+    assert IsNull("foo") == parser.parse("foo is null")
+    assert IsNull("foo") == parser.parse("foo IS NULL")
 
 
 def test_not_null() -> None:
-    assert NotNull("x") == parser.parse("x is not null")
-    assert NotNull("x") == parser.parse("x IS NOT NULL")
+    assert NotNull("foo") == parser.parse("foo is not null")
+    assert NotNull("foo") == parser.parse("foo IS NOT NULL")
 
 
 def test_is_nan() -> None:
-    assert IsNaN("x") == parser.parse("x is nan")
-    assert IsNaN("x") == parser.parse("x IS NAN")
+    assert IsNaN("foo") == parser.parse("foo is nan")
+    assert IsNaN("foo") == parser.parse("foo IS NAN")
 
 
 def test_not_nan() -> None:
-    assert NotNaN("x") == parser.parse("x is not nan")
-    assert NotNaN("x") == parser.parse("x IS NOT NaN")
+    assert NotNaN("foo") == parser.parse("foo is not nan")
+    assert NotNaN("foo") == parser.parse("foo IS NOT NaN")
 
 
 def test_less_than() -> None:
-    assert LessThan("x", 5) == parser.parse("x < 5")
-    assert LessThan("x", "a") == parser.parse("'a' > x")
+    assert LessThan("foo", 5) == parser.parse("foo < 5")
+    assert LessThan("foo", "a") == parser.parse("'a' > foo")
 
 
 def test_less_than_or_equal() -> None:
-    assert LessThanOrEqual("x", 5) == parser.parse("x <= 5")
-    assert LessThanOrEqual("x", "a") == parser.parse("'a' >= x")
+    assert LessThanOrEqual("foo", 5) == parser.parse("foo <= 5")
+    assert LessThanOrEqual("foo", "a") == parser.parse("'a' >= foo")
 
 
 def test_greater_than() -> None:
-    assert GreaterThan("x", 5) == parser.parse("x > 5")
-    assert GreaterThan("x", "a") == parser.parse("'a' < x")
+    assert GreaterThan("foo", 5) == parser.parse("foo > 5")
+    assert GreaterThan("foo", "a") == parser.parse("'a' < foo")
 
 
 def test_greater_than_or_equal() -> None:
-    assert GreaterThanOrEqual("x", 5) == parser.parse("x <= 5")
-    assert GreaterThanOrEqual("x", "a") == parser.parse("'a' >= x")
+    assert GreaterThanOrEqual("foo", 5) == parser.parse("foo <= 5")
+    assert GreaterThanOrEqual("foo", "a") == parser.parse("'a' >= foo")
 
 
 def test_equal_to() -> None:
-    assert EqualTo("x", 5) == parser.parse("x = 5")
-    assert EqualTo("x", "a") == parser.parse("'a' = x")
-    assert EqualTo("x", "a") == parser.parse("x == 'a'")
-    assert EqualTo("x", 5) == parser.parse("5 == x")
+    assert EqualTo("foo", 5) == parser.parse("foo = 5")
+    assert EqualTo("foo", "a") == parser.parse("'a' = foo")
+    assert EqualTo("foo", "a") == parser.parse("foo == 'a'")
+    assert EqualTo("foo", 5) == parser.parse("5 == foo")
 
 
 def test_not_equal_to() -> None:
-    assert NotEqualTo("x", 5) == parser.parse("x != 5")
-    assert NotEqualTo("x", "a") == parser.parse("'a' != x")
-    assert NotEqualTo("x", "a") == parser.parse("x <> 'a'")
-    assert NotEqualTo("x", 5) == parser.parse("5 <> x")
+    assert NotEqualTo("foo", 5) == parser.parse("foo != 5")
+    assert NotEqualTo("foo", "a") == parser.parse("'a' != foo")
+    assert NotEqualTo("foo", "a") == parser.parse("foo <> 'a'")
+    assert NotEqualTo("foo", 5) == parser.parse("5 <> foo")
 
 
 def test_in() -> None:
-    assert In("x", {5, 6, 7}) == parser.parse("x in (5, 6, 7)")
-    assert In("x", {"a", "b", "c"}) == parser.parse("x IN ('a', 'b', 'c')")
+    assert In("foo", {5, 6, 7}) == parser.parse("foo in (5, 6, 7)")
+    assert In("foo", {"a", "b", "c"}) == parser.parse("foo IN ('a', 'b', 'c')")
 
 
 def test_in_different_types() -> None:
     with pytest.raises(ParseException):
-        parser.parse("x in (5, 'a')")
+        parser.parse("foo in (5, 'a')")
 
 
 def test_not_in() -> None:
-    assert NotIn("x", {5, 6, 7}) == parser.parse("x not in (5, 6, 7)")
-    assert NotIn("x", {"a", "b", "c"}) == parser.parse("x NOT IN ('a', 'b', 'c')")
+    assert NotIn("foo", {5, 6, 7}) == parser.parse("foo not in (5, 6, 7)")
+    assert NotIn("foo", {"a", "b", "c"}) == parser.parse("foo NOT IN ('a', 'b', 'c')")
 
 
 def test_not_in_different_types() -> None:
     with pytest.raises(ParseException):
-        parser.parse("x not in (5, 'a')")
+        parser.parse("foo not in (5, 'a')")
 
 
 def test_simple_and() -> None:
-    assert And(GreaterThanOrEqual("x", 5), LessThan("x", 10)) == parser.parse("5 <= x and x < 10")
+    assert And(GreaterThanOrEqual("foo", 5), LessThan("foo", 10)) == parser.parse("5 <= foo and foo < 10")
 
 
 def test_and_with_not() -> None:
-    assert And(Not(GreaterThanOrEqual("x", 5)), LessThan("x", 10)) == parser.parse("not 5 <= x and x < 10")
-    assert And(GreaterThanOrEqual("x", 5), Not(LessThan("x", 10))) == parser.parse("5 <= x and not x < 10")
+    assert And(Not(GreaterThanOrEqual("foo", 5)), LessThan("foo", 10)) == parser.parse("not 5 <= foo and foo < 10")
+    assert And(GreaterThanOrEqual("foo", 5), Not(LessThan("foo", 10))) == parser.parse("5 <= foo and not foo < 10")
 
 
 def test_or_with_not() -> None:
-    assert Or(Not(LessThan("x", 5)), GreaterThan("x", 10)) == parser.parse("not x < 5 or 10 < x")
-    assert Or(LessThan("x", 5), Not(GreaterThan("x", 10))) == parser.parse("x < 5 or not 10 < x")
+    assert Or(Not(LessThan("foo", 5)), GreaterThan("foo", 10)) == parser.parse("not foo < 5 or 10 < foo")
+    assert Or(LessThan("foo", 5), Not(GreaterThan("foo", 10))) == parser.parse("foo < 5 or not 10 < foo")
 
 
 def test_simple_or() -> None:
-    assert Or(LessThan("x", 5), GreaterThan("x", 10)) == parser.parse("x < 5 or 10 < x")
+    assert Or(LessThan("foo", 5), GreaterThan("foo", 10)) == parser.parse("foo < 5 or 10 < foo")
 
 
 def test_and_or_without_parens() -> None:
-    assert Or(And(NotNull("x"), LessThan("x", 5)), GreaterThan("x", 10)) == parser.parse("x is not null and x < 5 or 10 < x")
-    assert Or(IsNull("x"), And(GreaterThanOrEqual("x", 5), LessThan("x", 10))) == parser.parse("x is null or 5 <= x and x < 10")
+    assert Or(And(NotNull("foo"), LessThan("foo", 5)), GreaterThan("foo", 10)) == parser.parse(
+        "foo is not null and foo < 5 or 10 < foo"
+    )
+    assert Or(IsNull("foo"), And(GreaterThanOrEqual("foo", 5), LessThan("foo", 10))) == parser.parse(
+        "foo is null or 5 <= foo and foo < 10"
+    )
 
 
 def test_and_or_with_parens() -> None:
-    assert And(NotNull("x"), Or(LessThan("x", 5), GreaterThan("x", 10))) == parser.parse("x is not null and (x < 5 or 10 < x)")
-    assert Or(IsNull("x"), And(GreaterThanOrEqual("x", 5), Not(LessThan("x", 10)))) == parser.parse(
-        "(x is null) or (5 <= x) and not(x < 10)"
+    assert And(NotNull("foo"), Or(LessThan("foo", 5), GreaterThan("foo", 10))) == parser.parse(
+        "foo is not null and (foo < 5 or 10 < foo)"
+    )
+    assert Or(IsNull("foo"), And(GreaterThanOrEqual("foo", 5), Not(LessThan("foo", 10)))) == parser.parse(
+        "(foo is null) or (5 <= foo) and not(foo < 10)"
     )
 
 
 def test_starts_with() -> None:
-    assert StartsWith("x", "data") == parser.parse("x LIKE 'data'")
+    assert StartsWith("foo", "data") == parser.parse("foo LIKE 'data'")
 
 
 def test_not_starts_with() -> None:
-    assert NotStartsWith("x", "data") == parser.parse("x NOT LIKE 'data'")
+    assert NotStartsWith("foo", "data") == parser.parse("foo NOT LIKE 'data'")
```

### Comparing `pyiceberg-0.4.0rc1/tests/expressions/test_projection.py` & `pyiceberg-0.4.0rc2/tests/expressions/test_projection.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.4.0rc1/tests/expressions/test_visitors.py` & `pyiceberg-0.4.0rc2/tests/expressions/test_visitors.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.4.0rc1/tests/io/test_fsspec.py` & `pyiceberg-0.4.0rc2/tests/io/test_fsspec.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.4.0rc1/tests/io/test_io.py` & `pyiceberg-0.4.0rc2/tests/io/test_io.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.4.0rc1/tests/io/test_pyarrow.py` & `pyiceberg-0.4.0rc2/tests/io/test_pyarrow.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.4.0rc1/tests/io/test_pyarrow_visitor.py` & `pyiceberg-0.4.0rc2/tests/io/test_pyarrow_visitor.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.4.0rc1/tests/table/test_init.py` & `pyiceberg-0.4.0rc2/tests/table/test_init.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.4.0rc1/tests/table/test_metadata.py` & `pyiceberg-0.4.0rc2/tests/table/test_metadata.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.4.0rc1/tests/table/test_partitioning.py` & `pyiceberg-0.4.0rc2/tests/table/test_partitioning.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.4.0rc1/tests/table/test_refs.py` & `pyiceberg-0.4.0rc2/tests/table/test_refs.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.4.0rc1/tests/table/test_snapshots.py` & `pyiceberg-0.4.0rc2/tests/table/test_snapshots.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.4.0rc1/tests/table/test_sorting.py` & `pyiceberg-0.4.0rc2/tests/table/test_sorting.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.4.0rc1/tests/test_conversions.py` & `pyiceberg-0.4.0rc2/tests/test_conversions.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.4.0rc1/tests/test_integration.py` & `pyiceberg-0.4.0rc2/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.4.0rc1/tests/test_schema.py` & `pyiceberg-0.4.0rc2/tests/test_schema.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.4.0rc1/tests/test_transforms.py` & `pyiceberg-0.4.0rc2/tests/test_transforms.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.4.0rc1/tests/test_typedef.py` & `pyiceberg-0.4.0rc2/tests/test_typedef.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.4.0rc1/tests/test_types.py` & `pyiceberg-0.4.0rc2/tests/test_types.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.4.0rc1/tests/test_version.py` & `pyiceberg-0.4.0rc2/tests/test_version.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.4.0rc1/tests/utils/test_bin_packing.py` & `pyiceberg-0.4.0rc2/tests/utils/test_bin_packing.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.4.0rc1/tests/utils/test_config.py` & `pyiceberg-0.4.0rc2/tests/utils/test_config.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.4.0rc1/tests/utils/test_deprecated.py` & `pyiceberg-0.4.0rc2/tests/utils/test_deprecated.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.4.0rc1/tests/utils/test_manifest.py` & `pyiceberg-0.4.0rc2/tests/utils/test_manifest.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.4.0rc1/tests/utils/test_schema_conversion.py` & `pyiceberg-0.4.0rc2/tests/utils/test_schema_conversion.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.4.0rc1/tests/utils/test_singleton.py` & `pyiceberg-0.4.0rc2/tests/utils/test_singleton.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.4.0rc1/vendor/fb303/FacebookService.py` & `pyiceberg-0.4.0rc2/vendor/fb303/FacebookService.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.4.0rc1/vendor/fb303/__init__.py` & `pyiceberg-0.4.0rc2/vendor/fb303/__init__.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.4.0rc1/vendor/fb303/constants.py` & `pyiceberg-0.4.0rc2/vendor/fb303/constants.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.4.0rc1/vendor/fb303/ttypes.py` & `pyiceberg-0.4.0rc2/vendor/fb303/ttypes.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.4.0rc1/vendor/hive_metastore/ThriftHiveMetastore.py` & `pyiceberg-0.4.0rc2/vendor/hive_metastore/ThriftHiveMetastore.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.4.0rc1/vendor/hive_metastore/__init__.py` & `pyiceberg-0.4.0rc2/vendor/hive_metastore/__init__.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.4.0rc1/vendor/hive_metastore/constants.py` & `pyiceberg-0.4.0rc2/vendor/hive_metastore/constants.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.4.0rc1/vendor/hive_metastore/ttypes.py` & `pyiceberg-0.4.0rc2/vendor/hive_metastore/ttypes.py`

 * *Files identical despite different names*

### Comparing `pyiceberg-0.4.0rc1/PKG-INFO` & `pyiceberg-0.4.0rc2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyiceberg
-Version: 0.4.0rc1
+Version: 0.4.0rc2
 Summary: Apache Iceberg is an open table format for huge analytic datasets
 Home-page: https://iceberg.apache.org/
 License: Apache-2.0
 Author: Apache Software Foundation
 Author-email: dev@iceberg.apache.org
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
@@ -30,15 +30,15 @@
 Requires-Dist: click (>=7.1.1,<9.0.0)
 Requires-Dist: duckdb (>=0.5.0,<1.0.0) ; extra == "duckdb"
 Requires-Dist: fsspec (>=2021.09.0,<2024.1.0)
 Requires-Dist: mmhash3 (>=3.0.0,<4.0.0)
 Requires-Dist: pandas (>=1.0.0,<3.0.0) ; extra == "pandas" or extra == "ray"
 Requires-Dist: pyarrow (>=9.0.0,<13.0.0) ; extra == "pyarrow" or extra == "pandas" or extra == "duckdb" or extra == "ray"
 Requires-Dist: pydantic (>=1.9.0,<2.0.0)
-Requires-Dist: pyparsing (>=3.0.7,<4.0.0)
+Requires-Dist: pyparsing (>=3.0.7,<3.1.0)
 Requires-Dist: python-snappy (>=0.6.0,<1.0.0) ; extra == "snappy"
 Requires-Dist: ray (>=2.0.0,<3.0.0) ; extra == "ray"
 Requires-Dist: requests (>=2.20.0,<3.0.0)
 Requires-Dist: rich (>=10.11.0,<14.0.0)
 Requires-Dist: s3fs (>=2021.08.0,<2024.1.0) ; extra == "s3fs"
 Requires-Dist: sortedcontainers (==2.4.0)
 Requires-Dist: strictyaml (>=1.7.0,<2.0.0)
```

