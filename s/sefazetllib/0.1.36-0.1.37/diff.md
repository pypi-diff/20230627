# Comparing `tmp/sefazetllib-0.1.36.tar.gz` & `tmp/sefazetllib-0.1.37.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sefazetllib-0.1.36.tar", max compression
+gzip compressed data, was "sefazetllib-0.1.37.tar", max compression
```

## Comparing `sefazetllib-0.1.36.tar` & `sefazetllib-0.1.37.tar`

### file list

```diff
@@ -1,78 +1,78 @@
--rw-r--r--   0        0        0    10173 2023-06-16 21:22:11.599220 sefazetllib-0.1.36/LICENSE
--rw-r--r--   0        0        0     3159 2023-06-16 21:22:11.599220 sefazetllib-0.1.36/README.md
--rw-r--r--   0        0        0     2445 2023-06-16 21:22:11.599220 sefazetllib-0.1.36/pyproject.toml
--rw-r--r--   0        0        0     1663 2023-06-16 21:22:11.599220 sefazetllib-0.1.36/sefazetllib/Builder.py
--rw-r--r--   0        0        0      135 2023-06-16 21:22:11.599220 sefazetllib-0.1.36/sefazetllib/__init__.py
--rw-r--r--   0        0        0     2338 2023-06-16 21:22:11.599220 sefazetllib-0.1.36/sefazetllib/config/CustomLogging.py
--rw-r--r--   0        0        0       52 2023-06-16 21:22:11.599220 sefazetllib-0.1.36/sefazetllib/config/__init__.py
--rw-r--r--   0        0        0     8218 2023-06-16 21:22:11.599220 sefazetllib-0.1.36/sefazetllib/etl/ETL.py
--rw-r--r--   0        0        0       36 2023-06-16 21:22:11.599220 sefazetllib-0.1.36/sefazetllib/etl/__init__.py
--rw-r--r--   0        0        0      701 2023-06-16 21:22:11.599220 sefazetllib-0.1.36/sefazetllib/extract/Extract.py
--rw-r--r--   0        0        0     1986 2023-06-16 21:22:11.599220 sefazetllib-0.1.36/sefazetllib/extract/ExtractLocal.py
--rw-r--r--   0        0        0     2479 2023-06-16 21:22:11.599220 sefazetllib-0.1.36/sefazetllib/extract/ExtractS3.py
--rw-r--r--   0        0        0     2521 2023-06-16 21:22:11.599220 sefazetllib-0.1.36/sefazetllib/extract/ExtractSQL.py
--rw-r--r--   0        0        0     2282 2023-06-16 21:22:11.599220 sefazetllib-0.1.36/sefazetllib/extract/ExtractStorage.py
--rw-r--r--   0        0        0      274 2023-06-16 21:22:11.599220 sefazetllib-0.1.36/sefazetllib/extract/__init__.py
--rw-r--r--   0        0        0      949 2023-06-16 21:22:11.599220 sefazetllib-0.1.36/sefazetllib/factory/Factory.py
--rw-r--r--   0        0        0       89 2023-06-16 21:22:11.599220 sefazetllib-0.1.36/sefazetllib/factory/__init__.py
--rw-r--r--   0        0        0      362 2023-06-16 21:22:11.599220 sefazetllib-0.1.36/sefazetllib/factory/platform/DatabasePlatform.py
--rw-r--r--   0        0        0      281 2023-06-16 21:22:11.599220 sefazetllib-0.1.36/sefazetllib/factory/platform/Platform.py
--rw-r--r--   0        0        0     1049 2023-06-16 21:22:11.609220 sefazetllib-0.1.36/sefazetllib/factory/platform/PlatformFactory.py
--rw-r--r--   0        0        0      268 2023-06-16 21:22:11.609220 sefazetllib-0.1.36/sefazetllib/factory/platform/__init__.py
--rw-r--r--   0        0        0      723 2023-06-16 21:22:11.609220 sefazetllib-0.1.36/sefazetllib/factory/platform/database/MySQL.py
--rw-r--r--   0        0        0     4069 2023-06-16 21:22:11.609220 sefazetllib-0.1.36/sefazetllib/factory/platform/database/PostgreSQL.py
--rw-r--r--   0        0        0      134 2023-06-16 21:22:11.609220 sefazetllib-0.1.36/sefazetllib/factory/platform/database/__init__.py
--rw-r--r--   0        0        0      259 2023-06-16 21:22:11.609220 sefazetllib-0.1.36/sefazetllib/factory/platform/dataframe/Default.py
--rw-r--r--   0        0        0     1793 2023-06-16 21:22:11.609220 sefazetllib-0.1.36/sefazetllib/factory/platform/dataframe/Pandas.py
--rw-r--r--   0        0        0     4679 2023-06-16 21:22:11.609220 sefazetllib-0.1.36/sefazetllib/factory/platform/dataframe/Spark.py
--rw-r--r--   0        0        0      195 2023-06-16 21:22:11.609220 sefazetllib-0.1.36/sefazetllib/factory/platform/dataframe/__init__.py
--rw-r--r--   0        0        0      683 2023-06-16 21:22:11.609220 sefazetllib-0.1.36/sefazetllib/load/Load.py
--rw-r--r--   0        0        0     2134 2023-06-16 21:22:11.609220 sefazetllib-0.1.36/sefazetllib/load/LoadLocal.py
--rw-r--r--   0        0        0     2386 2023-06-16 21:22:11.609220 sefazetllib-0.1.36/sefazetllib/load/LoadS3.py
--rw-r--r--   0        0        0     7601 2023-06-16 21:22:11.609220 sefazetllib-0.1.36/sefazetllib/load/LoadSQL.py
--rw-r--r--   0        0        0     2194 2023-06-16 21:22:11.609220 sefazetllib-0.1.36/sefazetllib/load/LoadStorage.py
--rw-r--r--   0        0        0      229 2023-06-16 21:22:11.609220 sefazetllib-0.1.36/sefazetllib/load/__init__.py
--rw-r--r--   0        0        0     1471 2023-06-16 21:22:11.609220 sefazetllib-0.1.36/sefazetllib/transform/MinMaxLineTransform.py
--rw-r--r--   0        0        0     4331 2023-06-16 21:22:11.609220 sefazetllib-0.1.36/sefazetllib/transform/QuartileTransform.py
--rw-r--r--   0        0        0      552 2023-06-16 21:22:11.609220 sefazetllib-0.1.36/sefazetllib/transform/Transform.py
--rw-r--r--   0        0        0      198 2023-06-16 21:22:11.609220 sefazetllib-0.1.36/sefazetllib/transform/__init__.py
--rw-r--r--   0        0        0       45 2023-06-16 21:22:11.609220 sefazetllib-0.1.36/sefazetllib/utils/__init__.py
--rw-r--r--   0        0        0      325 2023-06-16 21:22:11.609220 sefazetllib-0.1.36/sefazetllib/utils/key/DefaultKey.py
--rw-r--r--   0        0        0      400 2023-06-16 21:22:11.609220 sefazetllib-0.1.36/sefazetllib/utils/key/Key.py
--rw-r--r--   0        0        0      747 2023-06-16 21:22:11.609220 sefazetllib-0.1.36/sefazetllib/utils/key/SurrogateKey.py
--rw-r--r--   0        0        0      158 2023-06-16 21:22:11.609220 sefazetllib-0.1.36/sefazetllib/utils/key/__init__.py
--rw-r--r--   0        0        0     2097 2023-06-16 21:22:11.609220 sefazetllib-0.1.36/sefazetllib/utils/partition/DatePartition.py
--rw-r--r--   0        0        0      627 2023-06-16 21:22:11.609220 sefazetllib-0.1.36/sefazetllib/utils/partition/IncrementalRangePartition.py
--rw-r--r--   0        0        0      425 2023-06-16 21:22:11.609220 sefazetllib-0.1.36/sefazetllib/utils/partition/Partition.py
--rw-r--r--   0        0        0      229 2023-06-16 21:22:11.609220 sefazetllib-0.1.36/sefazetllib/utils/partition/__init__.py
--rw-r--r--   0        0        0     7729 2023-06-16 21:22:11.609220 sefazetllib-0.1.36/sefazetllib/validate/DataValidate.py
--rw-r--r--   0        0        0      383 2023-06-16 21:22:11.609220 sefazetllib-0.1.36/sefazetllib/validate/Validate.py
--rw-r--r--   0        0        0      110 2023-06-16 21:22:11.609220 sefazetllib-0.1.36/sefazetllib/validate/__init__.py
--rw-r--r--   0        0        0     3551 2023-06-16 21:22:11.609220 sefazetllib-0.1.36/sefazetllibcli/__init__.py
--rw-r--r--   0        0        0        0 2023-06-16 21:22:11.609220 sefazetllib-0.1.36/sefazetllibcli/config/__init__.py
--rw-r--r--   0        0        0     1117 2023-06-16 21:22:11.609220 sefazetllib-0.1.36/sefazetllibcli/config/logging.py
--rw-r--r--   0        0        0      185 2023-06-16 21:22:11.609220 sefazetllib-0.1.36/sefazetllibcli/errors/__init__.py
--rw-r--r--   0        0        0       76 2023-06-16 21:22:11.609220 sefazetllib-0.1.36/sefazetllibcli/errors/method_not_implemented.py
--rw-r--r--   0        0        0       52 2023-06-16 21:22:11.609220 sefazetllib-0.1.36/sefazetllibcli/errors/unsupported_file_extension.py
--rw-r--r--   0        0        0       88 2023-06-16 21:22:11.609220 sefazetllib-0.1.36/sefazetllibcli/errors/variable_processing_error.py
--rw-r--r--   0        0        0        0 2023-06-16 21:22:11.609220 sefazetllib-0.1.36/sefazetllibcli/generators/__init__.py
--rw-r--r--   0        0        0     5897 2023-06-16 21:22:11.609220 sefazetllib-0.1.36/sefazetllibcli/generators/etl_generator.py
--rw-r--r--   0        0        0      884 2023-06-16 21:22:11.609220 sefazetllib-0.1.36/sefazetllibcli/generators/generator.py
--rw-r--r--   0        0        0      374 2023-06-16 21:22:11.609220 sefazetllib-0.1.36/sefazetllibcli/templates/etl_template
--rw-r--r--   0        0        0        0 2023-06-16 21:22:11.609220 sefazetllib-0.1.36/sefazetllibcli/usecases/__init__.py
--rw-r--r--   0        0        0      524 2023-06-16 21:22:11.609220 sefazetllib-0.1.36/sefazetllibcli/usecases/process_variable/__init__.py
--rw-r--r--   0        0        0     3484 2023-06-16 21:22:11.609220 sefazetllib-0.1.36/sefazetllibcli/usecases/process_variable/process_etl_variable.py
--rw-r--r--   0        0        0     1128 2023-06-16 21:22:11.609220 sefazetllib-0.1.36/sefazetllibcli/usecases/process_variable/process_extract_variable.py
--rw-r--r--   0        0        0      986 2023-06-16 21:22:11.609220 sefazetllib-0.1.36/sefazetllibcli/usecases/process_variable/process_imports_variable.py
--rw-r--r--   0        0        0     1142 2023-06-16 21:22:11.609220 sefazetllib-0.1.36/sefazetllibcli/usecases/process_variable/process_key_variable.py
--rw-r--r--   0        0        0     1110 2023-06-16 21:22:11.609220 sefazetllib-0.1.36/sefazetllibcli/usecases/process_variable/process_load_variable.py
--rw-r--r--   0        0        0     1595 2023-06-16 21:22:11.609220 sefazetllib-0.1.36/sefazetllibcli/usecases/process_variable/process_partition_variable.py
--rw-r--r--   0        0        0     2086 2023-06-16 21:22:11.609220 sefazetllib-0.1.36/sefazetllibcli/usecases/process_variable/process_transforms_variable.py
--rw-r--r--   0        0        0     1074 2023-06-16 21:22:11.609220 sefazetllib-0.1.36/sefazetllibcli/usecases/process_variable/process_validate_variable.py
--rw-r--r--   0        0        0      935 2023-06-16 21:22:11.609220 sefazetllib-0.1.36/sefazetllibcli/usecases/process_variable/process_variable.py
--rw-r--r--   0        0        0       99 2023-06-16 21:22:11.609220 sefazetllib-0.1.36/sefazetllibcli/usecases/replace_template/__init__.py
--rw-r--r--   0        0        0      963 2023-06-16 21:22:11.609220 sefazetllib-0.1.36/sefazetllibcli/usecases/replace_template/replace_etl_template.py
--rw-r--r--   0        0        0     1678 2023-06-16 21:22:11.609220 sefazetllib-0.1.36/sefazetllibcli/usecases/replace_template/replace_template.py
--rw-r--r--   0        0        0       32 2023-06-16 21:22:11.609220 sefazetllib-0.1.36/sefazetllibcli/utils/__init__.py
--rw-r--r--   0        0        0     3631 2023-06-16 21:22:11.609220 sefazetllib-0.1.36/sefazetllibcli/utils/parse_etl.py
--rw-r--r--   0        0        0     4680 1970-01-01 00:00:00.000000 sefazetllib-0.1.36/PKG-INFO
+-rw-r--r--   0        0        0    10173 2023-06-27 14:11:06.678585 sefazetllib-0.1.37/LICENSE
+-rw-r--r--   0        0        0     3159 2023-06-27 14:11:06.678585 sefazetllib-0.1.37/README.md
+-rw-r--r--   0        0        0     2445 2023-06-27 14:11:06.688585 sefazetllib-0.1.37/pyproject.toml
+-rw-r--r--   0        0        0     1663 2023-06-27 14:11:06.688585 sefazetllib-0.1.37/sefazetllib/Builder.py
+-rw-r--r--   0        0        0      135 2023-06-27 14:11:06.688585 sefazetllib-0.1.37/sefazetllib/__init__.py
+-rw-r--r--   0        0        0     2338 2023-06-27 14:11:06.688585 sefazetllib-0.1.37/sefazetllib/config/CustomLogging.py
+-rw-r--r--   0        0        0       52 2023-06-27 14:11:06.688585 sefazetllib-0.1.37/sefazetllib/config/__init__.py
+-rw-r--r--   0        0        0     8218 2023-06-27 14:11:06.688585 sefazetllib-0.1.37/sefazetllib/etl/ETL.py
+-rw-r--r--   0        0        0       36 2023-06-27 14:11:06.688585 sefazetllib-0.1.37/sefazetllib/etl/__init__.py
+-rw-r--r--   0        0        0      701 2023-06-27 14:11:06.688585 sefazetllib-0.1.37/sefazetllib/extract/Extract.py
+-rw-r--r--   0        0        0     1986 2023-06-27 14:11:06.688585 sefazetllib-0.1.37/sefazetllib/extract/ExtractLocal.py
+-rw-r--r--   0        0        0     3366 2023-06-27 14:11:06.688585 sefazetllib-0.1.37/sefazetllib/extract/ExtractS3.py
+-rw-r--r--   0        0        0     2521 2023-06-27 14:11:06.688585 sefazetllib-0.1.37/sefazetllib/extract/ExtractSQL.py
+-rw-r--r--   0        0        0     2282 2023-06-27 14:11:06.688585 sefazetllib-0.1.37/sefazetllib/extract/ExtractStorage.py
+-rw-r--r--   0        0        0      274 2023-06-27 14:11:06.688585 sefazetllib-0.1.37/sefazetllib/extract/__init__.py
+-rw-r--r--   0        0        0      949 2023-06-27 14:11:06.688585 sefazetllib-0.1.37/sefazetllib/factory/Factory.py
+-rw-r--r--   0        0        0       89 2023-06-27 14:11:06.688585 sefazetllib-0.1.37/sefazetllib/factory/__init__.py
+-rw-r--r--   0        0        0      362 2023-06-27 14:11:06.688585 sefazetllib-0.1.37/sefazetllib/factory/platform/DatabasePlatform.py
+-rw-r--r--   0        0        0      281 2023-06-27 14:11:06.688585 sefazetllib-0.1.37/sefazetllib/factory/platform/Platform.py
+-rw-r--r--   0        0        0     1049 2023-06-27 14:11:06.688585 sefazetllib-0.1.37/sefazetllib/factory/platform/PlatformFactory.py
+-rw-r--r--   0        0        0      268 2023-06-27 14:11:06.688585 sefazetllib-0.1.37/sefazetllib/factory/platform/__init__.py
+-rw-r--r--   0        0        0      723 2023-06-27 14:11:06.688585 sefazetllib-0.1.37/sefazetllib/factory/platform/database/MySQL.py
+-rw-r--r--   0        0        0     4069 2023-06-27 14:11:06.688585 sefazetllib-0.1.37/sefazetllib/factory/platform/database/PostgreSQL.py
+-rw-r--r--   0        0        0      134 2023-06-27 14:11:06.688585 sefazetllib-0.1.37/sefazetllib/factory/platform/database/__init__.py
+-rw-r--r--   0        0        0      259 2023-06-27 14:11:06.688585 sefazetllib-0.1.37/sefazetllib/factory/platform/dataframe/Default.py
+-rw-r--r--   0        0        0     1793 2023-06-27 14:11:06.688585 sefazetllib-0.1.37/sefazetllib/factory/platform/dataframe/Pandas.py
+-rw-r--r--   0        0        0     4679 2023-06-27 14:11:06.688585 sefazetllib-0.1.37/sefazetllib/factory/platform/dataframe/Spark.py
+-rw-r--r--   0        0        0      195 2023-06-27 14:11:06.688585 sefazetllib-0.1.37/sefazetllib/factory/platform/dataframe/__init__.py
+-rw-r--r--   0        0        0      683 2023-06-27 14:11:06.688585 sefazetllib-0.1.37/sefazetllib/load/Load.py
+-rw-r--r--   0        0        0     2134 2023-06-27 14:11:06.688585 sefazetllib-0.1.37/sefazetllib/load/LoadLocal.py
+-rw-r--r--   0        0        0     2386 2023-06-27 14:11:06.688585 sefazetllib-0.1.37/sefazetllib/load/LoadS3.py
+-rw-r--r--   0        0        0     7601 2023-06-27 14:11:06.688585 sefazetllib-0.1.37/sefazetllib/load/LoadSQL.py
+-rw-r--r--   0        0        0     2194 2023-06-27 14:11:06.688585 sefazetllib-0.1.37/sefazetllib/load/LoadStorage.py
+-rw-r--r--   0        0        0      229 2023-06-27 14:11:06.688585 sefazetllib-0.1.37/sefazetllib/load/__init__.py
+-rw-r--r--   0        0        0     1471 2023-06-27 14:11:06.688585 sefazetllib-0.1.37/sefazetllib/transform/MinMaxLineTransform.py
+-rw-r--r--   0        0        0     4331 2023-06-27 14:11:06.688585 sefazetllib-0.1.37/sefazetllib/transform/QuartileTransform.py
+-rw-r--r--   0        0        0      552 2023-06-27 14:11:06.688585 sefazetllib-0.1.37/sefazetllib/transform/Transform.py
+-rw-r--r--   0        0        0      198 2023-06-27 14:11:06.688585 sefazetllib-0.1.37/sefazetllib/transform/__init__.py
+-rw-r--r--   0        0        0       45 2023-06-27 14:11:06.688585 sefazetllib-0.1.37/sefazetllib/utils/__init__.py
+-rw-r--r--   0        0        0      325 2023-06-27 14:11:06.688585 sefazetllib-0.1.37/sefazetllib/utils/key/DefaultKey.py
+-rw-r--r--   0        0        0      400 2023-06-27 14:11:06.688585 sefazetllib-0.1.37/sefazetllib/utils/key/Key.py
+-rw-r--r--   0        0        0      747 2023-06-27 14:11:06.688585 sefazetllib-0.1.37/sefazetllib/utils/key/SurrogateKey.py
+-rw-r--r--   0        0        0      158 2023-06-27 14:11:06.688585 sefazetllib-0.1.37/sefazetllib/utils/key/__init__.py
+-rw-r--r--   0        0        0     2097 2023-06-27 14:11:06.688585 sefazetllib-0.1.37/sefazetllib/utils/partition/DatePartition.py
+-rw-r--r--   0        0        0      627 2023-06-27 14:11:06.688585 sefazetllib-0.1.37/sefazetllib/utils/partition/IncrementalRangePartition.py
+-rw-r--r--   0        0        0      425 2023-06-27 14:11:06.688585 sefazetllib-0.1.37/sefazetllib/utils/partition/Partition.py
+-rw-r--r--   0        0        0      229 2023-06-27 14:11:06.688585 sefazetllib-0.1.37/sefazetllib/utils/partition/__init__.py
+-rw-r--r--   0        0        0     7729 2023-06-27 14:11:06.688585 sefazetllib-0.1.37/sefazetllib/validate/DataValidate.py
+-rw-r--r--   0        0        0      383 2023-06-27 14:11:06.688585 sefazetllib-0.1.37/sefazetllib/validate/Validate.py
+-rw-r--r--   0        0        0      110 2023-06-27 14:11:06.688585 sefazetllib-0.1.37/sefazetllib/validate/__init__.py
+-rw-r--r--   0        0        0     3551 2023-06-27 14:11:06.688585 sefazetllib-0.1.37/sefazetllibcli/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-27 14:11:06.688585 sefazetllib-0.1.37/sefazetllibcli/config/__init__.py
+-rw-r--r--   0        0        0     1117 2023-06-27 14:11:06.688585 sefazetllib-0.1.37/sefazetllibcli/config/logging.py
+-rw-r--r--   0        0        0      185 2023-06-27 14:11:06.688585 sefazetllib-0.1.37/sefazetllibcli/errors/__init__.py
+-rw-r--r--   0        0        0       76 2023-06-27 14:11:06.688585 sefazetllib-0.1.37/sefazetllibcli/errors/method_not_implemented.py
+-rw-r--r--   0        0        0       52 2023-06-27 14:11:06.688585 sefazetllib-0.1.37/sefazetllibcli/errors/unsupported_file_extension.py
+-rw-r--r--   0        0        0       88 2023-06-27 14:11:06.688585 sefazetllib-0.1.37/sefazetllibcli/errors/variable_processing_error.py
+-rw-r--r--   0        0        0        0 2023-06-27 14:11:06.688585 sefazetllib-0.1.37/sefazetllibcli/generators/__init__.py
+-rw-r--r--   0        0        0     5897 2023-06-27 14:11:06.688585 sefazetllib-0.1.37/sefazetllibcli/generators/etl_generator.py
+-rw-r--r--   0        0        0      884 2023-06-27 14:11:06.688585 sefazetllib-0.1.37/sefazetllibcli/generators/generator.py
+-rw-r--r--   0        0        0      374 2023-06-27 14:11:06.688585 sefazetllib-0.1.37/sefazetllibcli/templates/etl_template
+-rw-r--r--   0        0        0        0 2023-06-27 14:11:06.688585 sefazetllib-0.1.37/sefazetllibcli/usecases/__init__.py
+-rw-r--r--   0        0        0      524 2023-06-27 14:11:06.688585 sefazetllib-0.1.37/sefazetllibcli/usecases/process_variable/__init__.py
+-rw-r--r--   0        0        0     3484 2023-06-27 14:11:06.688585 sefazetllib-0.1.37/sefazetllibcli/usecases/process_variable/process_etl_variable.py
+-rw-r--r--   0        0        0     1128 2023-06-27 14:11:06.688585 sefazetllib-0.1.37/sefazetllibcli/usecases/process_variable/process_extract_variable.py
+-rw-r--r--   0        0        0      986 2023-06-27 14:11:06.688585 sefazetllib-0.1.37/sefazetllibcli/usecases/process_variable/process_imports_variable.py
+-rw-r--r--   0        0        0     1142 2023-06-27 14:11:06.688585 sefazetllib-0.1.37/sefazetllibcli/usecases/process_variable/process_key_variable.py
+-rw-r--r--   0        0        0     1110 2023-06-27 14:11:06.688585 sefazetllib-0.1.37/sefazetllibcli/usecases/process_variable/process_load_variable.py
+-rw-r--r--   0        0        0     1595 2023-06-27 14:11:06.688585 sefazetllib-0.1.37/sefazetllibcli/usecases/process_variable/process_partition_variable.py
+-rw-r--r--   0        0        0     2086 2023-06-27 14:11:06.688585 sefazetllib-0.1.37/sefazetllibcli/usecases/process_variable/process_transforms_variable.py
+-rw-r--r--   0        0        0     1074 2023-06-27 14:11:06.688585 sefazetllib-0.1.37/sefazetllibcli/usecases/process_variable/process_validate_variable.py
+-rw-r--r--   0        0        0      935 2023-06-27 14:11:06.688585 sefazetllib-0.1.37/sefazetllibcli/usecases/process_variable/process_variable.py
+-rw-r--r--   0        0        0       99 2023-06-27 14:11:06.688585 sefazetllib-0.1.37/sefazetllibcli/usecases/replace_template/__init__.py
+-rw-r--r--   0        0        0      963 2023-06-27 14:11:06.688585 sefazetllib-0.1.37/sefazetllibcli/usecases/replace_template/replace_etl_template.py
+-rw-r--r--   0        0        0     1678 2023-06-27 14:11:06.688585 sefazetllib-0.1.37/sefazetllibcli/usecases/replace_template/replace_template.py
+-rw-r--r--   0        0        0       32 2023-06-27 14:11:06.688585 sefazetllib-0.1.37/sefazetllibcli/utils/__init__.py
+-rw-r--r--   0        0        0     3631 2023-06-27 14:11:06.688585 sefazetllib-0.1.37/sefazetllibcli/utils/parse_etl.py
+-rw-r--r--   0        0        0     4680 1970-01-01 00:00:00.000000 sefazetllib-0.1.37/PKG-INFO
```

### Comparing `sefazetllib-0.1.36/LICENSE` & `sefazetllib-0.1.37/LICENSE`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.36/README.md` & `sefazetllib-0.1.37/README.md`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.36/pyproject.toml` & `sefazetllib-0.1.37/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sefazetllib"
-version = "0.1.36"
+version = "0.1.37"
 description = "sefazetllib is a library that provides a simplified and abstracted way to construct ETL/ELT pipelines."
 license = "Apache-2.0"
 authors = ["Felipe Gochi <felipe.gochi@elogroup.com.br>"]
 maintainers = [
     "Bruno Santos <bruno.santos@elogroup.com.br>",
     "Felipe Alcantara <felipe.alcantara@elogroup.com.br>",
     "Felipe Gochi <felipe.gochi@elogroup.com.br>",
```

### Comparing `sefazetllib-0.1.36/sefazetllib/Builder.py` & `sefazetllib-0.1.37/sefazetllib/Builder.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.36/sefazetllib/config/CustomLogging.py` & `sefazetllib-0.1.37/sefazetllib/config/CustomLogging.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.36/sefazetllib/etl/ETL.py` & `sefazetllib-0.1.37/sefazetllib/etl/ETL.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.36/sefazetllib/extract/Extract.py` & `sefazetllib-0.1.37/sefazetllib/extract/Extract.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.36/sefazetllib/extract/ExtractLocal.py` & `sefazetllib-0.1.37/sefazetllib/extract/ExtractLocal.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.36/sefazetllib/extract/ExtractS3.py` & `sefazetllib-0.1.37/sefazetllib/extract/ExtractS3.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import warnings
 from typing import Any, Dict, List
+from itertools import product
 
 from sefazetllib.Builder import Builder, field
 from sefazetllib.extract.Extract import Extract
 from sefazetllib.factory.platform.dataframe.Default import Default
 from sefazetllib.factory.platform.Platform import Platform
 
 
@@ -23,33 +24,54 @@
     partition: List[str] = field(default_factory=list)
     etl_partition: bool = field(default=False)
     reference: str = field(default="")
     duplicates: bool = field(default=False)
     columns: List[str] = field(default_factory=list)
     optional: bool = field(default=False)
 
+    # TODO (MX): Refatorar lógica do file_format do Hudi para que seja independente do Extract
     def build_connection_string(self):
         self.url = f"s3a://{self.repository}/{self.layer}/{self.schema}/{self.entity}"
 
         if self.partition != []:
-            for partition in self.partition:
-                self.setUrl(f"{self.url}/{partition}")
+            if self.file_format in ("hudi", "org.apache.hudi"):
+                self.partitions = list(
+                    product(
+                        *[
+                            partition.strip("{}").split(",")
+                            for partition in self.partition.get()
+                        ]
+                    )
+                )
+                self.format_properties.update(
+                    {
+                        "hoodie.datasource.read.paths": ",".join(
+                            [
+                                f"{self.url}/{'/'.join(partition)}"
+                                for partition in self.partitions
+                            ]
+                        )
+                    }
+                )
+            else:
+                for partition in self.partition.get():
+                    self.setUrl(f"{self.url}/{partition}")
 
         return self.url
 
     def execute(self, **kwargs):
         if isinstance(self.platform, Default):
             self.setPlatform(kwargs["platform"])
 
         local_repository = self.repository
         if local_repository == "":
             self.setRepository(kwargs["repository"])
-            
+
         if self.etl_partition:
-            self.setPartition(kwargs["partition"].get())
+            self.setPartition(kwargs["partition"])
 
         url = self.build_connection_string()
 
         if kwargs:
             args = kwargs["args"]
             if args.extractRepository and local_repository == "":
                 self.setRepository(args.extractRepository)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `sefazetllib-0.1.36/sefazetllib/extract/ExtractSQL.py` & `sefazetllib-0.1.37/sefazetllib/extract/ExtractSQL.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.36/sefazetllib/extract/ExtractStorage.py` & `sefazetllib-0.1.37/sefazetllib/extract/ExtractStorage.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.36/sefazetllib/factory/Factory.py` & `sefazetllib-0.1.37/sefazetllib/factory/Factory.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.36/sefazetllib/factory/platform/PlatformFactory.py` & `sefazetllib-0.1.37/sefazetllib/factory/platform/PlatformFactory.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.36/sefazetllib/factory/platform/database/MySQL.py` & `sefazetllib-0.1.37/sefazetllib/factory/platform/database/MySQL.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.36/sefazetllib/factory/platform/database/PostgreSQL.py` & `sefazetllib-0.1.37/sefazetllib/factory/platform/database/PostgreSQL.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.36/sefazetllib/factory/platform/dataframe/Pandas.py` & `sefazetllib-0.1.37/sefazetllib/factory/platform/dataframe/Pandas.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.36/sefazetllib/factory/platform/dataframe/Spark.py` & `sefazetllib-0.1.37/sefazetllib/factory/platform/dataframe/Spark.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.36/sefazetllib/load/Load.py` & `sefazetllib-0.1.37/sefazetllib/load/Load.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.36/sefazetllib/load/LoadLocal.py` & `sefazetllib-0.1.37/sefazetllib/load/LoadLocal.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.36/sefazetllib/load/LoadS3.py` & `sefazetllib-0.1.37/sefazetllib/load/LoadS3.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.36/sefazetllib/load/LoadSQL.py` & `sefazetllib-0.1.37/sefazetllib/load/LoadSQL.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.36/sefazetllib/load/LoadStorage.py` & `sefazetllib-0.1.37/sefazetllib/load/LoadStorage.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.36/sefazetllib/transform/MinMaxLineTransform.py` & `sefazetllib-0.1.37/sefazetllib/transform/MinMaxLineTransform.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.36/sefazetllib/transform/QuartileTransform.py` & `sefazetllib-0.1.37/sefazetllib/transform/QuartileTransform.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.36/sefazetllib/transform/Transform.py` & `sefazetllib-0.1.37/sefazetllib/transform/Transform.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.36/sefazetllib/utils/key/SurrogateKey.py` & `sefazetllib-0.1.37/sefazetllib/utils/key/SurrogateKey.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.36/sefazetllib/utils/partition/DatePartition.py` & `sefazetllib-0.1.37/sefazetllib/utils/partition/DatePartition.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.36/sefazetllib/utils/partition/IncrementalRangePartition.py` & `sefazetllib-0.1.37/sefazetllib/utils/partition/IncrementalRangePartition.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.36/sefazetllib/validate/DataValidate.py` & `sefazetllib-0.1.37/sefazetllib/validate/DataValidate.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.36/sefazetllibcli/__init__.py` & `sefazetllib-0.1.37/sefazetllibcli/__init__.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.36/sefazetllibcli/config/logging.py` & `sefazetllib-0.1.37/sefazetllibcli/config/logging.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.36/sefazetllibcli/generators/etl_generator.py` & `sefazetllib-0.1.37/sefazetllibcli/generators/etl_generator.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.36/sefazetllibcli/generators/generator.py` & `sefazetllib-0.1.37/sefazetllibcli/generators/generator.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.36/sefazetllibcli/usecases/process_variable/__init__.py` & `sefazetllib-0.1.37/sefazetllibcli/usecases/process_variable/__init__.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.36/sefazetllibcli/usecases/process_variable/process_etl_variable.py` & `sefazetllib-0.1.37/sefazetllibcli/usecases/process_variable/process_etl_variable.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.36/sefazetllibcli/usecases/process_variable/process_extract_variable.py` & `sefazetllib-0.1.37/sefazetllibcli/usecases/process_variable/process_extract_variable.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.36/sefazetllibcli/usecases/process_variable/process_imports_variable.py` & `sefazetllib-0.1.37/sefazetllibcli/usecases/process_variable/process_imports_variable.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.36/sefazetllibcli/usecases/process_variable/process_key_variable.py` & `sefazetllib-0.1.37/sefazetllibcli/usecases/process_variable/process_key_variable.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.36/sefazetllibcli/usecases/process_variable/process_load_variable.py` & `sefazetllib-0.1.37/sefazetllibcli/usecases/process_variable/process_load_variable.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.36/sefazetllibcli/usecases/process_variable/process_partition_variable.py` & `sefazetllib-0.1.37/sefazetllibcli/usecases/process_variable/process_partition_variable.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.36/sefazetllibcli/usecases/process_variable/process_transforms_variable.py` & `sefazetllib-0.1.37/sefazetllibcli/usecases/process_variable/process_transforms_variable.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.36/sefazetllibcli/usecases/process_variable/process_validate_variable.py` & `sefazetllib-0.1.37/sefazetllibcli/usecases/process_variable/process_validate_variable.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.36/sefazetllibcli/usecases/process_variable/process_variable.py` & `sefazetllib-0.1.37/sefazetllibcli/usecases/process_variable/process_variable.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.36/sefazetllibcli/usecases/replace_template/replace_etl_template.py` & `sefazetllib-0.1.37/sefazetllibcli/usecases/replace_template/replace_etl_template.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.36/sefazetllibcli/usecases/replace_template/replace_template.py` & `sefazetllib-0.1.37/sefazetllibcli/usecases/replace_template/replace_template.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.36/sefazetllibcli/utils/parse_etl.py` & `sefazetllib-0.1.37/sefazetllibcli/utils/parse_etl.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.36/PKG-INFO` & `sefazetllib-0.1.37/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sefazetllib
-Version: 0.1.36
+Version: 0.1.37
 Summary: sefazetllib is a library that provides a simplified and abstracted way to construct ETL/ELT pipelines.
 Home-page: https://sa-east-1.console.aws.amazon.com/codesuite/codecommit/repositories/jobs-lib-sefaz-ce/browse?region=sa-east-1
 License: Apache-2.0
 Author: Felipe Gochi
 Author-email: felipe.gochi@elogroup.com.br
 Maintainer: Bruno Santos
 Maintainer-email: bruno.santos@elogroup.com.br
```

