# Comparing `tmp/dbt_semantic_interfaces-0.1.0.dev7.tar.gz` & `tmp/dbt_semantic_interfaces-0.1.0.dev8.tar.gz`

## Comparing `dbt_semantic_interfaces-0.1.0.dev7.tar` & `dbt_semantic_interfaces-0.1.0.dev8.tar`

### file list

```diff
@@ -1,99 +1,85 @@
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev7/.tool-versions
--rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev7/CHANGELOG.md
--rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev7/Makefile
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev7/mypy.ini
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/__init__.py
--rw-r--r--   0        0        0    18186 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/dataclass_serialization.py
--rw-r--r--   0        0        0     2218 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/enum_extension.py
--rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/errors.py
--rw-r--r--   0        0        0     3459 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/pretty_print.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/py.typed
--rw-r--r--   0        0        0     3229 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/references.py
--rw-r--r--   0        0        0     6161 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/test_utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/implementations/__init__.py
--rw-r--r--   0        0        0     7622 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/implementations/base.py
--rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/implementations/metadata.py
--rw-r--r--   0        0        0     7699 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/implementations/metric.py
--rw-r--r--   0        0        0     1194 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/implementations/semantic_manifest.py
--rw-r--r--   0        0        0     6442 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/implementations/semantic_model.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/implementations/elements/__init__.py
--rw-r--r--   0        0        0     2492 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/implementations/elements/dimension.py
--rw-r--r--   0        0        0      933 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/implementations/elements/entity.py
--rw-r--r--   0        0        0     2113 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/implementations/elements/measure.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/implementations/filters/__init__.py
--rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/implementations/filters/call_parameter_sets.py
--rw-r--r--   0        0        0     5056 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/implementations/filters/where_filter.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/parsing/__init__.py
--rw-r--r--   0        0        0    14122 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/parsing/dir_to_model.py
--rw-r--r--   0        0        0     2783 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/parsing/explicit_schema.py
--rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/parsing/objects.py
--rw-r--r--   0        0        0     2967 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/parsing/schema_validator.py
--rw-r--r--   0        0        0     9504 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/parsing/schemas.py
--rw-r--r--   0        0        0     4483 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/parsing/yaml_loader.py
--rw-r--r--   0        0        0    14735 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/parsing/schemas/default_explicit_schema.json
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/protocols/__init__.py
--rw-r--r--   0        0        0     2836 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/protocols/dimension.py
--rw-r--r--   0        0        0     1516 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/protocols/entity.py
--rw-r--r--   0        0        0     2501 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/protocols/measure.py
--rw-r--r--   0        0        0      875 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/protocols/metadata.py
--rw-r--r--   0        0        0     5164 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/protocols/metric.py
--rw-r--r--   0        0        0     1221 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/protocols/protocol_hint.py
--rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/protocols/semantic_manifest.py
--rw-r--r--   0        0        0     3886 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/protocols/semantic_model.py
--rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/protocols/where_filter.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/transformations/__init__.py
--rw-r--r--   0        0        0     2797 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/transformations/add_input_metric_measures.py
--rw-r--r--   0        0        0     1304 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/transformations/agg_time_dimension.py
--rw-r--r--   0        0        0     1396 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/transformations/boolean_measure.py
--rw-r--r--   0        0        0     1678 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/transformations/convert_count.py
--rw-r--r--   0        0        0     2475 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/transformations/convert_median.py
--rw-r--r--   0        0        0     2081 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/transformations/names.py
--rw-r--r--   0        0        0     2762 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/transformations/proxy_measure.py
--rw-r--r--   0        0        0     2350 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/transformations/pydantic_rule_set.py
--rw-r--r--   0        0        0      994 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/transformations/rule_set.py
--rw-r--r--   0        0        0     2429 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/transformations/semantic_manifest_transformer.py
--rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/transformations/transform_rule.py
--rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/type_enums/__init__.py
--rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/type_enums/aggregation_type.py
--rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/type_enums/dimension_type.py
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/type_enums/entity_type.py
--rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/type_enums/metric_type.py
--rw-r--r--   0        0        0     1879 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/type_enums/time_granularity.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/validations/__init__.py
--rw-r--r--   0        0        0     2644 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/validations/agg_time_dimension.py
--rw-r--r--   0        0        0     3761 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/validations/common_entities.py
--rw-r--r--   0        0        0     7487 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/validations/dimension_const.py
--rw-r--r--   0        0        0     4149 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/validations/element_const.py
--rw-r--r--   0        0        0     5017 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/validations/entities.py
--rw-r--r--   0        0        0    28360 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/validations/measures.py
--rw-r--r--   0        0        0     7460 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/validations/metrics.py
--rw-r--r--   0        0        0     2420 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/validations/non_empty.py
--rw-r--r--   0        0        0     6753 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/validations/reserved_keywords.py
--rw-r--r--   0        0        0     5233 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/validations/semantic_manifest_validator.py
--rw-r--r--   0        0        0    10920 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/validations/semantic_models.py
--rw-r--r--   0        0        0     9960 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/validations/unique_valid_name.py
--rw-r--r--   0        0        0    15060 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/validations/validator_helpers.py
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev7/venv-3.9.16/pyvenv.cfg
--rw-r--r--   0        0        0     8834 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev7/venv-3.9.16/bin/Activate.ps1
--rw-r--r--   0        0        0     1958 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev7/venv-3.9.16/bin/activate
--rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev7/venv-3.9.16/bin/activate.csh
--rw-r--r--   0        0        0     2047 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev7/venv-3.9.16/bin/activate.fish
--rwxr-xr-x   0        0        0      279 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev7/venv-3.9.16/bin/hatch
--rwxr-xr-x   0        0        0      293 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev7/venv-3.9.16/bin/hatchling
--rwxr-xr-x   0        0        0      275 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev7/venv-3.9.16/bin/httpx
--rwxr-xr-x   0        0        0      281 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev7/venv-3.9.16/bin/keyring
--rwxr-xr-x   0        0        0      291 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev7/venv-3.9.16/bin/markdown-it
--rwxr-xr-x   0        0        0      292 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev7/venv-3.9.16/bin/pip
--rwxr-xr-x   0        0        0      292 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev7/venv-3.9.16/bin/pip3
--rwxr-xr-x   0        0        0      292 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev7/venv-3.9.16/bin/pip3.9
--rwxr-xr-x   0        0        0      286 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev7/venv-3.9.16/bin/pygmentize
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev7/venv-3.9.16/bin/python -> /Users/quigleymalcolm/.asdf/installs/python/3.9.16/bin/python
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev7/venv-3.9.16/bin/python3 -> python
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev7/venv-3.9.16/bin/python3.9 -> python
--rwxr-xr-x   0        0        0      290 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev7/venv-3.9.16/bin/userpath
--rwxr-xr-x   0        0        0      309 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev7/venv-3.9.16/bin/virtualenv
--rw-r--r--   0        0        0     1864 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev7/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev7/LICENSE
--rw-r--r--   0        0        0     1476 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev7/README.md
--rw-r--r--   0        0        0     2399 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev7/pyproject.toml
--rw-r--r--   0        0        0     2522 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev7/PKG-INFO
+-rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev8/CHANGELOG.md
+-rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev8/Makefile
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev8/mypy.ini
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/__init__.py
+-rw-r--r--   0        0        0    18186 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/dataclass_serialization.py
+-rw-r--r--   0        0        0     2218 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/enum_extension.py
+-rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/errors.py
+-rw-r--r--   0        0        0     3459 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/pretty_print.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/py.typed
+-rw-r--r--   0        0        0     3229 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/references.py
+-rw-r--r--   0        0        0     6161 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/test_utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/implementations/__init__.py
+-rw-r--r--   0        0        0     7622 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/implementations/base.py
+-rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/implementations/metadata.py
+-rw-r--r--   0        0        0     7699 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/implementations/metric.py
+-rw-r--r--   0        0        0     1737 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/implementations/project_configuration.py
+-rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/implementations/semantic_manifest.py
+-rw-r--r--   0        0        0     6442 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/implementations/semantic_model.py
+-rw-r--r--   0        0        0     1775 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/implementations/semantic_version.py
+-rw-r--r--   0        0        0      782 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/implementations/time_spine_table_configuration.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/implementations/elements/__init__.py
+-rw-r--r--   0        0        0     2492 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/implementations/elements/dimension.py
+-rw-r--r--   0        0        0      933 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/implementations/elements/entity.py
+-rw-r--r--   0        0        0     2113 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/implementations/elements/measure.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/implementations/filters/__init__.py
+-rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/implementations/filters/call_parameter_sets.py
+-rw-r--r--   0        0        0     5056 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/implementations/filters/where_filter.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/parsing/__init__.py
+-rw-r--r--   0        0        0    15561 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/parsing/dir_to_model.py
+-rw-r--r--   0        0        0     2812 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/parsing/generate_json_schema_file.py
+-rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/parsing/objects.py
+-rw-r--r--   0        0        0     2967 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/parsing/schema_validator.py
+-rw-r--r--   0        0        0     9860 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/parsing/schemas.py
+-rw-r--r--   0        0        0     4483 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/parsing/yaml_loader.py
+-rw-r--r--   0        0        0    15414 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/parsing/generated_json_schemas/default_explicit_schema.json
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/protocols/__init__.py
+-rw-r--r--   0        0        0     2836 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/protocols/dimension.py
+-rw-r--r--   0        0        0     1516 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/protocols/entity.py
+-rw-r--r--   0        0        0     2501 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/protocols/measure.py
+-rw-r--r--   0        0        0      875 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/protocols/metadata.py
+-rw-r--r--   0        0        0     5164 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/protocols/metric.py
+-rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/protocols/project_configuration.py
+-rw-r--r--   0        0        0     1221 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/protocols/protocol_hint.py
+-rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/protocols/semantic_manifest.py
+-rw-r--r--   0        0        0     3886 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/protocols/semantic_model.py
+-rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/protocols/semantic_version.py
+-rw-r--r--   0        0        0      989 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/protocols/time_spine_configuration.py
+-rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/protocols/where_filter.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/transformations/__init__.py
+-rw-r--r--   0        0        0     2797 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/transformations/add_input_metric_measures.py
+-rw-r--r--   0        0        0     1304 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/transformations/agg_time_dimension.py
+-rw-r--r--   0        0        0     1396 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/transformations/boolean_measure.py
+-rw-r--r--   0        0        0     1678 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/transformations/convert_count.py
+-rw-r--r--   0        0        0     2475 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/transformations/convert_median.py
+-rw-r--r--   0        0        0     2081 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/transformations/names.py
+-rw-r--r--   0        0        0     2762 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/transformations/proxy_measure.py
+-rw-r--r--   0        0        0     2350 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/transformations/pydantic_rule_set.py
+-rw-r--r--   0        0        0      994 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/transformations/rule_set.py
+-rw-r--r--   0        0        0     2429 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/transformations/semantic_manifest_transformer.py
+-rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/transformations/transform_rule.py
+-rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/type_enums/__init__.py
+-rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/type_enums/aggregation_type.py
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/type_enums/dimension_type.py
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/type_enums/entity_type.py
+-rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/type_enums/metric_type.py
+-rw-r--r--   0        0        0     1879 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/type_enums/time_granularity.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/validations/__init__.py
+-rw-r--r--   0        0        0     2644 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/validations/agg_time_dimension.py
+-rw-r--r--   0        0        0     3761 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/validations/common_entities.py
+-rw-r--r--   0        0        0     7487 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/validations/dimension_const.py
+-rw-r--r--   0        0        0     4149 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/validations/element_const.py
+-rw-r--r--   0        0        0     5017 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/validations/entities.py
+-rw-r--r--   0        0        0    28360 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/validations/measures.py
+-rw-r--r--   0        0        0     7460 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/validations/metrics.py
+-rw-r--r--   0        0        0     2420 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/validations/non_empty.py
+-rw-r--r--   0        0        0     6753 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/validations/reserved_keywords.py
+-rw-r--r--   0        0        0     5233 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/validations/semantic_manifest_validator.py
+-rw-r--r--   0        0        0    10920 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/validations/semantic_models.py
+-rw-r--r--   0        0        0     9960 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/validations/unique_valid_name.py
+-rw-r--r--   0        0        0    15060 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/validations/validator_helpers.py
+-rw-r--r--   0        0        0     1864 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev8/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev8/LICENSE
+-rw-r--r--   0        0        0     1476 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev8/README.md
+-rw-r--r--   0        0        0     2399 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev8/pyproject.toml
+-rw-r--r--   0        0        0     2522 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev8/PKG-INFO
```

### Comparing `dbt_semantic_interfaces-0.1.0.dev7/Makefile` & `dbt_semantic_interfaces-0.1.0.dev8/Makefile`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/dataclass_serialization.py` & `dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/dataclass_serialization.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/enum_extension.py` & `dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/enum_extension.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/errors.py` & `dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/errors.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/pretty_print.py` & `dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/pretty_print.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/references.py` & `dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/references.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/test_utils.py` & `dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/test_utils.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/implementations/base.py` & `dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/implementations/base.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/implementations/metric.py` & `dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/implementations/metric.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/implementations/semantic_model.py` & `dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/implementations/semantic_model.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/implementations/elements/dimension.py` & `dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/implementations/elements/dimension.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/implementations/elements/entity.py` & `dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/implementations/elements/entity.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/implementations/elements/measure.py` & `dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/implementations/elements/measure.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/implementations/filters/call_parameter_sets.py` & `dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/implementations/filters/call_parameter_sets.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/implementations/filters/where_filter.py` & `dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/implementations/filters/where_filter.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/parsing/dir_to_model.py` & `dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/parsing/dir_to_model.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,28 +5,33 @@
 from string import Template
 from typing import Dict, List, Optional, Type, Union
 
 from jsonschema import exceptions
 
 from dbt_semantic_interfaces.errors import ParsingException
 from dbt_semantic_interfaces.implementations.metric import PydanticMetric
+from dbt_semantic_interfaces.implementations.project_configuration import (
+    PydanticProjectConfiguration,
+)
 from dbt_semantic_interfaces.implementations.semantic_manifest import (
     PydanticSemanticManifest,
 )
 from dbt_semantic_interfaces.implementations.semantic_model import PydanticSemanticModel
 from dbt_semantic_interfaces.parsing.objects import Version, YamlConfigFile
 from dbt_semantic_interfaces.parsing.schemas import (
     metric_validator,
+    project_configuration_validator,
     semantic_model_validator,
 )
 from dbt_semantic_interfaces.parsing.yaml_loader import (
     PARSING_CONTEXT_KEY,
     ParsingContext,
     YamlConfigLoader,
 )
+from dbt_semantic_interfaces.pretty_print import pformat_big_objects
 from dbt_semantic_interfaces.transformations.semantic_manifest_transformer import (
     PydanticSemanticManifestTransformer,
 )
 from dbt_semantic_interfaces.validations.validator_helpers import (
     FileContext,
     SemanticManifestValidationException,
     SemanticManifestValidationResults,
@@ -35,15 +40,17 @@
 )
 
 logger = logging.getLogger(__name__)
 
 VERSION_KEY = "mf_config_schema"
 METRIC_TYPE = "metric"
 SEMANTIC_MODEL_TYPE = "semantic_model"
-DOCUMENT_TYPES = [METRIC_TYPE, SEMANTIC_MODEL_TYPE]
+PROJECT_CONFIGURATION_TYPE = "project_configuration"
+
+DOCUMENT_TYPES = [METRIC_TYPE, SEMANTIC_MODEL_TYPE, PROJECT_CONFIGURATION_TYPE]
 
 
 @dataclass(frozen=True)
 class SemanticManifestBuildResult:  # noqa: D
     semantic_manifest: PydanticSemanticManifest
     # Issues found in the model.
     issues: SemanticManifestValidationResults = SemanticManifestValidationResults()
@@ -54,15 +61,15 @@
     """Results of parsing a config file.
 
     Attributes:
         elements: MetricFlow model elements parsed from the file
         issues: Issues found when trying to parse the file
     """
 
-    elements: List[Union[PydanticSemanticModel, PydanticMetric]]
+    elements: List[Union[PydanticSemanticModel, PydanticMetric, PydanticProjectConfiguration]]
     issues: List[ValidationIssue]
 
 
 def collect_yaml_config_file_paths(directory: str) -> List[str]:
     """Collects a list of file paths for model config files.
 
     Ignores files that are:
@@ -179,65 +186,79 @@
     return SemanticManifestBuildResult(semantic_manifest=model, issues=build_issues)
 
 
 def parse_yaml_files_to_semantic_manifest(
     files: List[YamlConfigFile],
     semantic_model_class: Type[PydanticSemanticModel] = PydanticSemanticModel,
     metric_class: Type[PydanticMetric] = PydanticMetric,
+    project_configuration_class: Type[PydanticProjectConfiguration] = PydanticProjectConfiguration,
 ) -> SemanticManifestBuildResult:
     """Builds SemanticManifest from list of config files (as strings).
 
     Persistent storage connection may be passed to write parsed objects=
     to storage and populate object metadata
 
     Note: this function does not finalize the model
     """
     semantic_models = []
     metrics = []
-    valid_object_classes = [semantic_model_class.__name__, metric_class.__name__]
+    project_configurations = []
+    valid_object_classes = [semantic_model_class.__name__, metric_class.__name__, project_configuration_class.__name__]
     issues: List[ValidationIssue] = []
 
     for config_file in files:
+        logger.error(f"Parsing: {config_file}")
         parsing_result = parse_config_yaml(  # parse config file
             config_file,
             semantic_model_class=semantic_model_class,
             metric_class=metric_class,
+            project_configuration_class=project_configuration_class,
         )
         file_issues = parsing_result.issues
         for obj in parsing_result.elements:
             if isinstance(obj, semantic_model_class):
                 semantic_models.append(obj)
             elif isinstance(obj, metric_class):
                 metrics.append(obj)
+            elif isinstance(obj, project_configuration_class):
+                project_configurations.append(obj)
             else:
                 file_issues.append(
                     ValidationError(
                         context=FileContext(file_name=config_file.filepath),
                         message=f"Unexpected model object {obj.__class__.__name__}. Expected {valid_object_classes}.",
                     )
                 )
 
         issues += file_issues
 
+    if len(project_configurations) != 1:
+        raise ParsingException(
+            f"Did not find exactly one project configuration. Debugging context is:\n\n"
+            f"{pformat_big_objects(project_configurations=project_configurations, issues=issues)}"
+        )
+
     return SemanticManifestBuildResult(
         semantic_manifest=PydanticSemanticManifest(
             semantic_models=semantic_models,
             metrics=metrics,
+            project_configuration=project_configurations[0],
         ),
         issues=SemanticManifestValidationResults.from_issues_sequence(issues),
     )
 
 
 def parse_config_yaml(
     config_yaml: YamlConfigFile,
     semantic_model_class: Type[PydanticSemanticModel] = PydanticSemanticModel,
     metric_class: Type[PydanticMetric] = PydanticMetric,
+    project_configuration_class: Type[PydanticProjectConfiguration] = PydanticProjectConfiguration,
 ) -> FileParsingResult:
     """Parses transform config file passed as string - Returns list of model objects."""
-    results: List[Union[PydanticSemanticModel, PydanticMetric]] = []
+    results: List[Union[PydanticSemanticModel, PydanticMetric, PydanticProjectConfiguration]] = []
     ctx: Optional[ParsingContext] = None
     issues: List[ValidationIssue] = []
     try:
         for config_document in YamlConfigLoader.load_all_with_context(
             name=config_yaml.filepath, contents=config_yaml.contents
         ):
             # The config document can be None if there is nothing but white space between two `---`
@@ -295,14 +316,17 @@
             try:
                 if document_type == METRIC_TYPE:
                     metric_validator.validate(config_document[document_type])
                     results.append(metric_class.parse_obj(object_cfg))
                 elif document_type == SEMANTIC_MODEL_TYPE:
                     semantic_model_validator.validate(config_document[document_type])
                     results.append(semantic_model_class.parse_obj(object_cfg))
+                elif document_type == PROJECT_CONFIGURATION_TYPE:
+                    project_configuration_validator.validate(config_document[document_type])
+                    results.append(project_configuration_class.parse_obj(object_cfg))
                 else:
                     issues.append(
                         ValidationError(
                             context=FileContext(file_name=ctx.filename, line_number=ctx.start_line),
                             message=f"Invalid document type: {document_type}. Expected {DOCUMENT_TYPES}.",
                         )
                     )
```

### Comparing `dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/parsing/explicit_schema.py` & `dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/parsing/generate_json_schema_file.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 from copy import deepcopy
 from pathlib import Path
 from typing import Dict, List, Union
 
 from dbt_semantic_interfaces.parsing import schemas
 
 TOP_LEVEL_SCHEMAS = {
-    "metric": "metric",
-    "semantic_model": "semantic_model",
-    "derived_group_by_element_schema": "derived_identifier",
+    "project_configuration_schema": "project_configuration",
+    "metric_schema": "metric",
+    "semantic_model_schema": "semantic_model",
 }
 
 BASE_SCHEMA = {
     "$schema": "http://json-schema.org/draft-07/schema#",
     "type": "object",
     "title": "MetricFlow file schema",
 }
@@ -73,10 +73,10 @@
         json.dump(json_schema, f, indent=4, sort_keys=True)
         f.write("\n")
 
 
 if __name__ == "__main__":
     write_json_schema(
         json_schema=generate_explict_json_schema(schemas.schema_store),
-        output_dir=str(Path(__file__).parent / "schemas"),
+        output_dir=str(Path(__file__).parent / "generated_json_schemas"),
         file_name="default_explicit_schema.json",
     )
```

### Comparing `dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/parsing/objects.py` & `dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/parsing/objects.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/parsing/schema_validator.py` & `dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/parsing/schema_validator.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/parsing/schemas.py` & `dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/parsing/schemas.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from dbt_semantic_interfaces.parsing.schema_validator import SchemaValidator
 
 TRANSFORM_OBJECT_NAME_PATTERN = "(?!.*__).*^[a-z][a-z0-9_]*[a-z0-9]$"
 
 
 # Enums
-metric_types_enum_values = ["SIMPLE", "RATIO", "EXPR", "CUMULATIVE", "DERIVED"]
+metric_types_enum_values = ["SIMPLE", "RATIO", "CUMULATIVE", "DERIVED"]
 metric_types_enum_values += [x.lower() for x in metric_types_enum_values]
 
 entity_type_enum_values = ["PRIMARY", "UNIQUE", "FOREIGN", "NATURAL"]
 entity_type_enum_values += [x.lower() for x in entity_type_enum_values]
 
 aggregation_type_values = [
     "SUM",
@@ -197,15 +197,15 @@
     },
     "additionalProperties": False,
     "required": ["name", "type"],
 }
 
 # Top level object schemas
 metric_schema = {
-    "$id": "metric",
+    "$id": "metric_schema",
     "type": "object",
     "properties": {
         "name": {
             "type": "string",
             "pattern": TRANSFORM_OBJECT_NAME_PATTERN,
         },
         "type": {"enum": metric_types_enum_values},
@@ -238,16 +238,43 @@
         "agg_time_dimension": {"type": "string"},
     },
     "additionalProperties": False,
     "required": [],
 }
 
 
+time_spine_table_configuration_schema = {
+    "$id": "time_spine_table_configuration_schema",
+    "type": "object",
+    "properties": {
+        "location": {"type": "string"},
+        "column_name": {"type": "string"},
+        "grain": {"enum": time_granularity_values},
+    },
+    "additionalProperties": False,
+    "required": ["location", "column_name", "grain"],
+}
+
+
+project_configuration_schema = {
+    "$id": "project_configuration_schema",
+    "type": "object",
+    "properties": {
+        "time_spine_table_configurations": {
+            "type": "array",
+            "items": {"$ref": "time_spine_table_configuration_schema"},
+        },
+    },
+    "additionalProperties": False,
+    "required": ["time_spine_table_configurations"],
+}
+
+
 semantic_model_schema = {
-    "$id": "semantic_model",
+    "$id": "semantic_model_schema",
     "type": "object",
     "properties": {
         "name": {
             "type": "string",
             "pattern": TRANSFORM_OBJECT_NAME_PATTERN,
         },
         "node_relation": {"$ref": "node_relation_schema"},
@@ -257,50 +284,34 @@
         "dimensions": {"type": "array", "items": {"$ref": "dimension_schema"}},
         "description": {"type": "string"},
     },
     "additionalProperties": False,
     "required": ["name"],
 }
 
-derived_group_by_element_schema = {
-    "$id": "derived_group_by_element_schema",
-    "type": "object",
-    "properties": {
-        "name": {
-            "type": "string",
-            "pattern": TRANSFORM_OBJECT_NAME_PATTERN,
-        },
-        "expr": {"type": ["string", "boolean"]},
-        "expr_elements": {
-            "type": "array",
-            "items": {"type": "string"},
-        },
-    },
-    "additionalProperties": False,
-    "required": ["name", "expr"],
-}
 
 schema_store = {
     # Top level schemas
     metric_schema["$id"]: metric_schema,
     semantic_model_schema["$id"]: semantic_model_schema,
-    derived_group_by_element_schema["$id"]: derived_group_by_element_schema,
+    project_configuration_schema["$id"]: project_configuration_schema,
     # Sub-object schemas
     metric_input_measure_schema["$id"]: metric_input_measure_schema,
     metric_type_params_schema["$id"]: metric_type_params_schema,
     entity_schema["$id"]: entity_schema,
     measure_schema["$id"]: measure_schema,
     dimension_schema["$id"]: dimension_schema,
     validity_params_schema["$id"]: validity_params_schema,
     dimension_type_params_schema["$id"]: dimension_type_params_schema,
     aggregation_type_params_schema["$id"]: aggregation_type_params_schema,
     non_additive_dimension_schema["$id"]: non_additive_dimension_schema,
     metric_input_schema["$id"]: metric_input_schema,
     node_relation_schema["$id"]: node_relation_schema,
     semantic_model_defaults_schema["$id"]: semantic_model_defaults_schema,
+    time_spine_table_configuration_schema["$id"]: time_spine_table_configuration_schema,
 }
 
 
 resolver = RefResolver.from_schema(schema=metric_schema, store=schema_store)
 semantic_model_validator = SchemaValidator(semantic_model_schema, resolver=resolver)
-derived_group_by_element_validator = SchemaValidator(derived_group_by_element_schema, resolver=resolver)
 metric_validator = SchemaValidator(metric_schema, resolver=resolver)
+project_configuration_validator = SchemaValidator(project_configuration_schema, resolver=resolver)
```

### Comparing `dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/parsing/yaml_loader.py` & `dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/parsing/yaml_loader.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/parsing/schemas/default_explicit_schema.json` & `dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/parsing/generated_json_schemas/default_explicit_schema.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9025000000000001%*

 * *Differences: {"'definitions'": "{'metric_schema': OrderedDict([('$id', 'metric_schema'), "*

 * *                  "('additionalProperties', False), ('properties', OrderedDict([('description', "*

 * *                  "OrderedDict([('type', 'string')])), ('filter', OrderedDict([('type', "*

 * *                  "'string')])), ('name', OrderedDict([('pattern', "*

 * *                  "'(?!.*__).*^[a-z][a-z0-9_]*[a-z0-9]$'), ('type', 'string')])), ('type', "*

 * *                  "OrderedDict([('enum', ['SIMPLE', 'RATIO', 'CUMULATIVE', 'DERIVED' […]*

```diff
@@ -13,41 +13,14 @@
                 },
                 "use_discrete_percentile": {
                     "type": "boolean"
                 }
             },
             "type": "object"
         },
-        "derived_group_by_element_schema": {
-            "$id": "derived_group_by_element_schema",
-            "additionalProperties": false,
-            "properties": {
-                "expr": {
-                    "type": [
-                        "string",
-                        "boolean"
-                    ]
-                },
-                "expr_elements": {
-                    "items": {
-                        "type": "string"
-                    },
-                    "type": "array"
-                },
-                "name": {
-                    "pattern": "(?!.*__).*^[a-z][a-z0-9_]*[a-z0-9]$",
-                    "type": "string"
-                }
-            },
-            "required": [
-                "name",
-                "expr"
-            ],
-            "type": "object"
-        },
         "dimension_schema": {
             "$id": "dimension_schema",
             "additionalProperties": false,
             "anyOf": [
                 {
                     "not": {
                         "$ref": "#/definitions/is-time-dimension"
@@ -232,53 +205,14 @@
             },
             "required": [
                 "name",
                 "agg"
             ],
             "type": "object"
         },
-        "metric": {
-            "$id": "metric",
-            "additionalProperties": false,
-            "properties": {
-                "description": {
-                    "type": "string"
-                },
-                "filter": {
-                    "type": "string"
-                },
-                "name": {
-                    "pattern": "(?!.*__).*^[a-z][a-z0-9_]*[a-z0-9]$",
-                    "type": "string"
-                },
-                "type": {
-                    "enum": [
-                        "SIMPLE",
-                        "RATIO",
-                        "EXPR",
-                        "CUMULATIVE",
-                        "DERIVED",
-                        "simple",
-                        "ratio",
-                        "expr",
-                        "cumulative",
-                        "derived"
-                    ]
-                },
-                "type_params": {
-                    "$ref": "#/definitions/metric_type_params"
-                }
-            },
-            "required": [
-                "name",
-                "type",
-                "type_params"
-            ],
-            "type": "object"
-        },
         "metric_input_measure_schema": {
             "$id": "metric_input_measure_schema",
             "oneOf": [
                 {
                     "type": "string"
                 },
                 {
@@ -316,14 +250,51 @@
                 },
                 "offset_window": {
                     "type": "string"
                 }
             },
             "type": "object"
         },
+        "metric_schema": {
+            "$id": "metric_schema",
+            "additionalProperties": false,
+            "properties": {
+                "description": {
+                    "type": "string"
+                },
+                "filter": {
+                    "type": "string"
+                },
+                "name": {
+                    "pattern": "(?!.*__).*^[a-z][a-z0-9_]*[a-z0-9]$",
+                    "type": "string"
+                },
+                "type": {
+                    "enum": [
+                        "SIMPLE",
+                        "RATIO",
+                        "CUMULATIVE",
+                        "DERIVED",
+                        "simple",
+                        "ratio",
+                        "cumulative",
+                        "derived"
+                    ]
+                },
+                "type_params": {
+                    "$ref": "#/definitions/metric_type_params"
+                }
+            },
+            "required": [
+                "name",
+                "type",
+                "type_params"
+            ],
+            "type": "object"
+        },
         "metric_type_params": {
             "$id": "metric_type_params",
             "additionalProperties": false,
             "properties": {
                 "denominator": {
                     "$ref": "#/definitions/metric_input_measure_schema"
                 },
@@ -400,16 +371,43 @@
                 }
             },
             "required": [
                 "name"
             ],
             "type": "object"
         },
-        "semantic_model": {
-            "$id": "semantic_model",
+        "project_configuration_schema": {
+            "$id": "project_configuration_schema",
+            "additionalProperties": false,
+            "properties": {
+                "time_spine_table_configurations": {
+                    "items": {
+                        "$ref": "#/definitions/time_spine_table_configuration_schema"
+                    },
+                    "type": "array"
+                }
+            },
+            "required": [
+                "time_spine_table_configurations"
+            ],
+            "type": "object"
+        },
+        "semantic_model_defaults_schema": {
+            "$id": "semantic_model_defaults_schema",
+            "additionalProperties": false,
+            "properties": {
+                "agg_time_dimension": {
+                    "type": "string"
+                }
+            },
+            "required": [],
+            "type": "object"
+        },
+        "semantic_model_schema": {
+            "$id": "semantic_model_schema",
             "additionalProperties": false,
             "properties": {
                 "defaults": {
                     "$ref": "#/definitions/semantic_model_defaults_schema"
                 },
                 "description": {
                     "type": "string"
@@ -441,23 +439,44 @@
                 }
             },
             "required": [
                 "name"
             ],
             "type": "object"
         },
-        "semantic_model_defaults_schema": {
-            "$id": "semantic_model_defaults_schema",
+        "time_spine_table_configuration_schema": {
+            "$id": "time_spine_table_configuration_schema",
             "additionalProperties": false,
             "properties": {
-                "agg_time_dimension": {
+                "column_name": {
+                    "type": "string"
+                },
+                "grain": {
+                    "enum": [
+                        "DAY",
+                        "WEEK",
+                        "MONTH",
+                        "QUARTER",
+                        "YEAR",
+                        "day",
+                        "week",
+                        "month",
+                        "quarter",
+                        "year"
+                    ]
+                },
+                "location": {
                     "type": "string"
                 }
             },
-            "required": [],
+            "required": [
+                "location",
+                "column_name",
+                "grain"
+            ],
             "type": "object"
         },
         "validity_params_schema": {
             "$id": "validity_params_schema",
             "additionalProperties": false,
             "properties": {
                 "is_end": {
@@ -467,20 +486,20 @@
                     "type": "boolean"
                 }
             },
             "type": "object"
         }
     },
     "properties": {
-        "derived_identifier": {
-            "$ref": "#/definitions/derived_group_by_element_schema"
-        },
         "metric": {
-            "$ref": "#/definitions/metric"
+            "$ref": "#/definitions/metric_schema"
+        },
+        "project_configuration": {
+            "$ref": "#/definitions/project_configuration_schema"
         },
         "semantic_model": {
-            "$ref": "#/definitions/semantic_model"
+            "$ref": "#/definitions/semantic_model_schema"
         }
     },
     "title": "MetricFlow file schema",
     "type": "object"
 }
```

### Comparing `dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/protocols/__init__.py` & `dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/protocols/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/protocols/dimension.py` & `dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/protocols/dimension.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/protocols/entity.py` & `dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/protocols/entity.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/protocols/measure.py` & `dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/protocols/measure.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/protocols/metadata.py` & `dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/protocols/metadata.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/protocols/metric.py` & `dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/protocols/metric.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/protocols/protocol_hint.py` & `dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/protocols/protocol_hint.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/protocols/semantic_model.py` & `dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/protocols/semantic_model.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/transformations/add_input_metric_measures.py` & `dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/transformations/add_input_metric_measures.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/transformations/agg_time_dimension.py` & `dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/transformations/agg_time_dimension.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/transformations/boolean_measure.py` & `dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/transformations/boolean_measure.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/transformations/convert_count.py` & `dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/transformations/convert_count.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/transformations/convert_median.py` & `dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/transformations/convert_median.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/transformations/names.py` & `dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/transformations/names.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/transformations/proxy_measure.py` & `dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/transformations/proxy_measure.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/transformations/pydantic_rule_set.py` & `dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/transformations/pydantic_rule_set.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/transformations/rule_set.py` & `dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/transformations/rule_set.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/transformations/semantic_manifest_transformer.py` & `dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/transformations/semantic_manifest_transformer.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/transformations/transform_rule.py` & `dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/transformations/transform_rule.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/type_enums/time_granularity.py` & `dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/type_enums/time_granularity.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/validations/agg_time_dimension.py` & `dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/validations/agg_time_dimension.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/validations/common_entities.py` & `dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/validations/common_entities.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/validations/dimension_const.py` & `dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/validations/dimension_const.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/validations/element_const.py` & `dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/validations/element_const.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/validations/entities.py` & `dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/validations/entities.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/validations/measures.py` & `dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/validations/measures.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/validations/metrics.py` & `dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/validations/metrics.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/validations/non_empty.py` & `dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/validations/non_empty.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/validations/reserved_keywords.py` & `dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/validations/reserved_keywords.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/validations/semantic_manifest_validator.py` & `dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/validations/semantic_manifest_validator.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/validations/semantic_models.py` & `dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/validations/semantic_models.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/validations/unique_valid_name.py` & `dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/validations/unique_valid_name.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev7/dbt_semantic_interfaces/validations/validator_helpers.py` & `dbt_semantic_interfaces-0.1.0.dev8/dbt_semantic_interfaces/validations/validator_helpers.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev7/.gitignore` & `dbt_semantic_interfaces-0.1.0.dev8/.gitignore`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev7/LICENSE` & `dbt_semantic_interfaces-0.1.0.dev8/LICENSE`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev7/README.md` & `dbt_semantic_interfaces-0.1.0.dev8/README.md`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev7/pyproject.toml` & `dbt_semantic_interfaces-0.1.0.dev8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "dbt-semantic-interfaces"
-version = "0.1.0.dev7"
+version = "0.1.0.dev8"
 description = 'The shared semantic layer definitions that dbt-core and MetricFlow use'
 readme = "README.md"
 requires-python = ">=3.8"
 license = "Apache-2.0"
 keywords = []
 authors = [
   { name = "dbt Labs", email = "info@dbtlabs.com" },
```

### Comparing `dbt_semantic_interfaces-0.1.0.dev7/PKG-INFO` & `dbt_semantic_interfaces-0.1.0.dev8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-semantic-interfaces
-Version: 0.1.0.dev7
+Version: 0.1.0.dev8
 Summary: The shared semantic layer definitions that dbt-core and MetricFlow use
 Author-email: dbt Labs <info@dbtlabs.com>
 License-Expression: Apache-2.0
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dbt-semantic-interfaces Version: 0.1.0.dev7
+Metadata-Version: 2.1 Name: dbt-semantic-interfaces Version: 0.1.0.dev8
 Summary: The shared semantic layer definitions that dbt-core and MetricFlow use
 Author-email: dbt Labs
 dbtlabs.com> License-Expression: Apache-2.0 License-File: LICENSE Classifier:
 Development Status :: 4 - Beta Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
```

