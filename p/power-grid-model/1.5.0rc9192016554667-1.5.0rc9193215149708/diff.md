# Comparing `tmp/power-grid-model-1.5.0rc9192016554667.tar.gz` & `tmp/power-grid-model-1.5.0rc9193215149708.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "power-grid-model-1.5.0rc9192016554667.tar", last modified: Tue Jun 27 09:08:40 2023, max compression
+gzip compressed data, was "power-grid-model-1.5.0rc9193215149708.tar", last modified: Tue Jun 27 12:07:47 2023, max compression
```

## Comparing `power-grid-model-1.5.0rc9192016554667.tar` & `power-grid-model-1.5.0rc9193215149708.tar`

### file list

```diff
@@ -1,620 +1,620 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:08:40.683107 power-grid-model-1.5.0rc9192016554667/
--rw-r--r--   0 runner    (1001) docker     (123)    14907 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8142 2023-06-27 09:08:40.683107 power-grid-model-1.5.0rc9192016554667/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-27 09:07:51.000000 power-grid-model-1.5.0rc9192016554667/PYPI_VERSION
--rw-r--r--   0 runner    (1001) docker     (123)     6818 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:08:40.535108 power-grid-model-1.5.0rc9192016554667/power_grid_model_c/
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/power_grid_model_c/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:08:40.535108 power-grid-model-1.5.0rc9192016554667/power_grid_model_c/power_grid_model/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/power_grid_model_c/power_grid_model/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:08:40.527108 power-grid-model-1.5.0rc9192016554667/power_grid_model_c/power_grid_model/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:08:40.539108 power-grid-model-1.5.0rc9192016554667/power_grid_model_c/power_grid_model/include/power_grid_model/
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/power_grid_model_c/power_grid_model/include/power_grid_model/all_components.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:08:40.539108 power-grid-model-1.5.0rc9192016554667/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/
--rw-r--r--   0 runner    (1001) docker     (123)     4220 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/dataset.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    28563 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/input.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     9937 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_data.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_data_gen.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    17078 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/output.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     9396 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/update.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     9108 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/power_grid_model_c/power_grid_model/include/power_grid_model/calculation_parameters.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:08:40.543108 power-grid-model-1.5.0rc9192016554667/power_grid_model_c/power_grid_model/include/power_grid_model/component/
--rw-r--r--   0 runner    (1001) docker     (123)     4215 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/power_grid_model_c/power_grid_model/include/power_grid_model/component/appliance.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/power_grid_model_c/power_grid_model/include/power_grid_model/component/base.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     8932 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/power_grid_model_c/power_grid_model/include/power_grid_model/component/branch.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     6781 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/power_grid_model_c/power_grid_model/include/power_grid_model/component/branch3.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4446 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/power_grid_model_c/power_grid_model/include/power_grid_model/component/fault.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/power_grid_model_c/power_grid_model/include/power_grid_model/component/line.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/power_grid_model_c/power_grid_model/include/power_grid_model/component/link.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     5344 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/power_grid_model_c/power_grid_model/include/power_grid_model/component/load_gen.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2694 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/power_grid_model_c/power_grid_model/include/power_grid_model/component/node.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4775 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/power_grid_model_c/power_grid_model/include/power_grid_model/component/power_sensor.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/power_grid_model_c/power_grid_model/include/power_grid_model/component/sensor.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2874 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/power_grid_model_c/power_grid_model/include/power_grid_model/component/shunt.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4397 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/power_grid_model_c/power_grid_model/include/power_grid_model/component/source.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    20049 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/power_grid_model_c/power_grid_model/include/power_grid_model/component/three_winding_transformer.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    10955 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/power_grid_model_c/power_grid_model/include/power_grid_model/component/transformer.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/power_grid_model_c/power_grid_model/include/power_grid_model/component/transformer_utils.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     5581 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/power_grid_model_c/power_grid_model/include/power_grid_model/component/voltage_sensor.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    15119 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/power_grid_model_c/power_grid_model/include/power_grid_model/container.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/power_grid_model_c/power_grid_model/include/power_grid_model/enum.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     5302 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/power_grid_model_c/power_grid_model/include/power_grid_model/exception.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    67927 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/power_grid_model_c/power_grid_model/include/power_grid_model/main_model.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:08:40.547108 power-grid-model-1.5.0rc9192016554667/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/
--rw-r--r--   0 runner    (1001) docker     (123)     2436 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/block_matrix.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     8954 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/iterative_current_pf_solver.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    41694 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/iterative_linear_se_solver.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     7164 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/iterative_pf_solver.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     6446 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/linear_pf_solver.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     6192 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/math_solver.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    16064 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/newton_raphson_pf_solver.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    16203 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/sparse_lu_solver.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    20148 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/y_bus.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3055 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/power_grid_model_c/power_grid_model/include/power_grid_model/power_grid_model.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2753 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/power_grid_model_c/power_grid_model/include/power_grid_model/sparse_mapping.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    11399 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/power_grid_model_c/power_grid_model/include/power_grid_model/three_phase_tensor.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/power_grid_model_c/power_grid_model/include/power_grid_model/timer.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    30797 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/power_grid_model_c/power_grid_model/include/power_grid_model/topology.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:08:40.547108 power-grid-model-1.5.0rc9192016554667/power_grid_model_c/power_grid_model_c/
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/power_grid_model_c/power_grid_model_c/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:08:40.547108 power-grid-model-1.5.0rc9192016554667/power_grid_model_c/power_grid_model_c/include/
--rw-r--r--   0 runner    (1001) docker     (123)    26085 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/power_grid_model_c/power_grid_model_c/include/power_grid_model_c.h
--rw-r--r--   0 runner    (1001) docker     (123)    15382 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/power_grid_model_c/power_grid_model_c/power_grid_model_c.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3634 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 09:08:40.683107 power-grid-model-1.5.0rc9192016554667/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     7078 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:08:40.527108 power-grid-model-1.5.0rc9192016554667/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:08:40.547108 power-grid-model-1.5.0rc9192016554667/src/power_grid_model/
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/src/power_grid_model/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:08:40.551108 power-grid-model-1.5.0rc9192016554667/src/power_grid_model/core/
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/src/power_grid_model/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/src/power_grid_model/core/error_handling.py
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/src/power_grid_model/core/index_integer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/src/power_grid_model/core/options.py
--rw-r--r--   0 runner    (1001) docker     (123)     9994 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/src/power_grid_model/core/power_grid_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     9240 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/src/power_grid_model/core/power_grid_meta.py
--rw-r--r--   0 runner    (1001) docker     (123)    17761 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/src/power_grid_model/core/power_grid_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5239 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/src/power_grid_model/data_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/src/power_grid_model/enum.py
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/src/power_grid_model/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    21645 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/src/power_grid_model/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:08:40.551108 power-grid-model-1.5.0rc9192016554667/src/power_grid_model/validation/
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/src/power_grid_model/validation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4166 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/src/power_grid_model/validation/assertions.py
--rw-r--r--   0 runner    (1001) docker     (123)    14686 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/src/power_grid_model/validation/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    30704 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/src/power_grid_model/validation/rules.py
--rw-r--r--   0 runner    (1001) docker     (123)     8601 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/src/power_grid_model/validation/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    28618 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/src/power_grid_model/validation/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:08:40.551108 power-grid-model-1.5.0rc9192016554667/src/power_grid_model.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8142 2023-06-27 09:08:40.000000 power-grid-model-1.5.0rc9192016554667/src/power_grid_model.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    37053 2023-06-27 09:08:40.000000 power-grid-model-1.5.0rc9192016554667/src/power_grid_model.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 09:08:40.000000 power-grid-model-1.5.0rc9192016554667/src/power_grid_model.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-06-27 09:08:40.000000 power-grid-model-1.5.0rc9192016554667/src/power_grid_model.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-27 09:08:40.000000 power-grid-model-1.5.0rc9192016554667/src/power_grid_model.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:08:40.535108 power-grid-model-1.5.0rc9192016554667/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:08:40.535108 power-grid-model-1.5.0rc9192016554667/tests/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:08:40.531108 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:08:40.555107 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/1os2msr/
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/1os2msr/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/1os2msr/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/1os2msr/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/1os2msr/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/1os2msr/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/1os2msr/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:08:40.555107 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/dummy-test/
--rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/dummy-test/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/dummy-test/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/dummy-test/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/dummy-test/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/dummy-test/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/dummy-test/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:08:40.559107 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/dummy-test-batch/
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/dummy-test-batch/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/dummy-test-batch/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/dummy-test-batch/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/dummy-test-batch/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/dummy-test-batch/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/dummy-test-batch/sym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/dummy-test-batch/sym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/dummy-test-batch/sym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/dummy-test-batch/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/dummy-test-batch/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:08:40.563107 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/dummy-test-batch-dependent-cacheable/
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/dummy-test-batch-dependent-cacheable/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/dummy-test-batch-dependent-cacheable/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/dummy-test-batch-dependent-cacheable/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/dummy-test-batch-dependent-cacheable/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/dummy-test-batch-dependent-cacheable/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/dummy-test-batch-dependent-cacheable/sym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/dummy-test-batch-dependent-cacheable/sym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/dummy-test-batch-dependent-cacheable/sym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/dummy-test-batch-dependent-cacheable/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/dummy-test-batch-dependent-cacheable/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:08:40.567108 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/sym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/sym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/sym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:08:40.567108 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/dummy-test-batch-incomplete-input/
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/dummy-test-batch-incomplete-input/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/dummy-test-batch-incomplete-input/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/dummy-test-batch-incomplete-input/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/dummy-test-batch-incomplete-input/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/dummy-test-batch-incomplete-input/sym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/dummy-test-batch-incomplete-input/sym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/dummy-test-batch-incomplete-input/sym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/dummy-test-batch-incomplete-input/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/dummy-test-batch-incomplete-input/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:08:40.571107 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/dummy-test-batch-independent-cacheable/
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/dummy-test-batch-independent-cacheable/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/dummy-test-batch-independent-cacheable/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/dummy-test-batch-independent-cacheable/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/dummy-test-batch-independent-cacheable/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/dummy-test-batch-independent-cacheable/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/dummy-test-batch-independent-cacheable/sym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/dummy-test-batch-independent-cacheable/sym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/dummy-test-batch-independent-cacheable/sym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/dummy-test-batch-independent-cacheable/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/dummy-test-batch-independent-cacheable/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:08:40.575107 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/sym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/sym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/sym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:08:40.575107 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/dummy-test-batch-newton/
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/dummy-test-batch-newton/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/dummy-test-batch-newton/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/dummy-test-batch-newton/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/dummy-test-batch-newton/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/dummy-test-batch-newton/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/dummy-test-batch-newton/sym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/dummy-test-batch-newton/sym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/dummy-test-batch-newton/sym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/dummy-test-batch-newton/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/dummy-test-batch-newton/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:08:40.579107 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/dummy-test-i-n-optional/
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/dummy-test-i-n-optional/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/dummy-test-i-n-optional/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/dummy-test-i-n-optional/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/dummy-test-i-n-optional/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/dummy-test-i-n-optional/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/dummy-test-i-n-optional/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:08:40.583107 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/gaia-example/
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/gaia-example/asym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/gaia-example/asym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/gaia-example/gaia_grid.gnf
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/gaia-example/gaia_grid.gnf.license
--rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/gaia-example/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/gaia-example/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/gaia-example/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/gaia-example/params.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:08:40.583107 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/multi-source-with-angle/
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/multi-source-with-angle/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/multi-source-with-angle/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/multi-source-with-angle/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/multi-source-with-angle/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/multi-source-with-angle/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/multi-source-with-angle/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:08:40.531108 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:08:40.531108 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/components/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:08:40.531108 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/components/asymmetric/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:08:40.583107 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/asym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/asym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/params.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:08:40.587107 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/components/asymmetric/asym_load/
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/components/asymmetric/asym_load/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/components/asymmetric/asym_load/asym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/components/asymmetric/asym_load/asym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/components/asymmetric/asym_load/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/components/asymmetric/asym_load/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/components/asymmetric/asym_load/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/components/asymmetric/asym_load/params.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:08:40.587107 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/components/asymmetric/line/
--rw-r--r--   0 runner    (1001) docker     (123)      910 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/components/asymmetric/line/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/components/asymmetric/line/asym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/components/asymmetric/line/asym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/components/asymmetric/line/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/components/asymmetric/line/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/components/asymmetric/line/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/components/asymmetric/line/params.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:08:40.587107 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/components/asymmetric/node/
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/components/asymmetric/node/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/components/asymmetric/node/asym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/components/asymmetric/node/asym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/components/asymmetric/node/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/components/asymmetric/node/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/components/asymmetric/node/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/components/asymmetric/node/params.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:08:40.591107 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/components/asymmetric/shunt/
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/components/asymmetric/shunt/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/components/asymmetric/shunt/asym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/components/asymmetric/shunt/asym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/components/asymmetric/shunt/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/components/asymmetric/shunt/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/components/asymmetric/shunt/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/components/asymmetric/shunt/params.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:08:40.591107 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/components/asymmetric/source/
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/components/asymmetric/source/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/components/asymmetric/source/asym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/components/asymmetric/source/asym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/components/asymmetric/source/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/components/asymmetric/source/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/components/asymmetric/source/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/components/asymmetric/source/params.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:08:40.591107 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/asym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/asym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/params.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:08:40.595107 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/components/asymmetric/sym_load/
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/components/asymmetric/sym_load/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/components/asymmetric/sym_load/asym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/components/asymmetric/sym_load/asym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/components/asymmetric/sym_load/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/components/asymmetric/sym_load/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/components/asymmetric/sym_load/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/components/asymmetric/sym_load/params.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:08:40.595107 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/components/asymmetric/transformer/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/components/asymmetric/transformer/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    17633 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/components/asymmetric/transformer/asym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/components/asymmetric/transformer/asym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/components/asymmetric/transformer/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/components/asymmetric/transformer/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/components/asymmetric/transformer/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/components/asymmetric/transformer/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/components/asymmetric/transformer/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/components/asymmetric/transformer/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:08:40.531108 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/components/symmetric/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:08:40.595107 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/components/symmetric/basic-node/
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/components/symmetric/basic-node/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/components/symmetric/basic-node/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/components/symmetric/basic-node/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/components/symmetric/basic-node/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/components/symmetric/basic-node/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/components/symmetric/basic-node/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/components/symmetric/basic-node/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:08:40.599107 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/components/symmetric/line/
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/components/symmetric/line/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/components/symmetric/line/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/components/symmetric/line/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/components/symmetric/line/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/components/symmetric/line/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/components/symmetric/line/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/components/symmetric/line/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:08:40.599107 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/components/symmetric/node/
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/components/symmetric/node/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/components/symmetric/node/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/components/symmetric/node/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/components/symmetric/node/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/components/symmetric/node/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/components/symmetric/node/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/components/symmetric/node/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:08:40.603107 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/components/symmetric/shunt/
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/components/symmetric/shunt/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      892 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/components/symmetric/shunt/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/components/symmetric/shunt/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/components/symmetric/shunt/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/components/symmetric/shunt/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/components/symmetric/shunt/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/components/symmetric/shunt/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:08:40.603107 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/components/symmetric/source/
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/components/symmetric/source/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/components/symmetric/source/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/components/symmetric/source/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/components/symmetric/source/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/components/symmetric/source/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/components/symmetric/source/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/components/symmetric/source/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:08:40.607107 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/components/symmetric/sym_gen/
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/components/symmetric/sym_gen/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/components/symmetric/sym_gen/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/components/symmetric/sym_gen/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/components/symmetric/sym_gen/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/components/symmetric/sym_gen/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/components/symmetric/sym_gen/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/components/symmetric/sym_gen/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:08:40.611107 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/components/symmetric/sym_load/
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/components/symmetric/sym_load/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/components/symmetric/sym_load/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/components/symmetric/sym_load/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/components/symmetric/sym_load/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/components/symmetric/sym_load/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/components/symmetric/sym_load/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/components/symmetric/sym_load/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:08:40.619107 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/
--rw-r--r--   0 runner    (1001) docker     (123)      917 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     8883 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/sym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/sym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:08:40.623107 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/components/symmetric/transformer/
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/components/symmetric/transformer/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/components/symmetric/transformer/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/components/symmetric/transformer/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/components/symmetric/transformer/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/components/symmetric/transformer/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)    15639 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/components/symmetric/transformer/sym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/components/symmetric/transformer/sym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     2827 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/components/symmetric/transformer/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/components/symmetric/transformer/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:08:40.531108 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/networks/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:08:40.531108 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/networks/asymmetric/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:08:40.631107 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    15865 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/asym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/asym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     8935 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     6642 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:08:40.635107 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    10605 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/asym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/asym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     6208 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/params.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:08:40.531108 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/networks/symmetric/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:08:40.639107 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/
--rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     8939 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     8702 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/sym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/sym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     6642 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:08:40.643107 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     6216 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     5384 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:08:40.643107 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/r-state-estimation/
--rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/r-state-estimation/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/r-state-estimation/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/r-state-estimation/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/r-state-estimation/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/r-state-estimation/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/r-state-estimation/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:08:40.643107 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/three-winding-transformer/
--rw-r--r--   0 runner    (1001) docker     (123)    21196 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/three-winding-transformer/asym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/three-winding-transformer/asym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/three-winding-transformer/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/three-winding-transformer/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/three-winding-transformer/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/three-winding-transformer/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     7374 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/three-winding-transformer/sym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/three-winding-transformer/sym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/three-winding-transformer/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/three-winding-transformer/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:08:40.647107 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/vision-example/
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/vision-example/asym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/vision-example/asym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/vision-example/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/vision-example/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/vision-example/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/vision-example/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     2450 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/vision-example/vision_grid.vnf
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/vision-example/vision_grid.vnf.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:08:40.647107 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/vision-validation-network/
--rw-r--r--   0 runner    (1001) docker     (123)    20486 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/vision-validation-network/asym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/vision-validation-network/asym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)    30756 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/vision-validation-network/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/vision-validation-network/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/vision-validation-network/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/vision-validation-network/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)    11853 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/vision-validation-network/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/vision-validation-network/sym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)    35119 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/vision-validation-network/vision_validation_network.vnf
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/vision-validation-network/vision_validation_network.vnf.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:08:40.535108 power-grid-model-1.5.0rc9192016554667/tests/data/short_circuit/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:08:40.651107 power-grid-model-1.5.0rc9192016554667/tests/data/short_circuit/single_phase_to_ground_a/
--rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/short_circuit/single_phase_to_ground_a/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/short_circuit/single_phase_to_ground_a/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/short_circuit/single_phase_to_ground_a/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/short_circuit/single_phase_to_ground_a/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)    60794 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/short_circuit/single_phase_to_ground_a/sc_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/short_circuit/single_phase_to_ground_a/sc_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     5234 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/short_circuit/single_phase_to_ground_a/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/short_circuit/single_phase_to_ground_a/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:08:40.651107 power-grid-model-1.5.0rc9192016554667/tests/data/short_circuit/single_phase_to_ground_b/
--rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/short_circuit/single_phase_to_ground_b/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/short_circuit/single_phase_to_ground_b/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/short_circuit/single_phase_to_ground_b/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/short_circuit/single_phase_to_ground_b/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)    60980 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/short_circuit/single_phase_to_ground_b/sc_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/short_circuit/single_phase_to_ground_b/sc_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     5234 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/short_circuit/single_phase_to_ground_b/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/short_circuit/single_phase_to_ground_b/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:08:40.655107 power-grid-model-1.5.0rc9192016554667/tests/data/short_circuit/single_phase_to_ground_c/
--rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/short_circuit/single_phase_to_ground_c/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/short_circuit/single_phase_to_ground_c/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/short_circuit/single_phase_to_ground_c/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/short_circuit/single_phase_to_ground_c/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)    60938 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/short_circuit/single_phase_to_ground_c/sc_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/short_circuit/single_phase_to_ground_c/sc_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     5234 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/short_circuit/single_phase_to_ground_c/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/short_circuit/single_phase_to_ground_c/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:08:40.655107 power-grid-model-1.5.0rc9192016554667/tests/data/short_circuit/three_phase_abc/
--rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/short_circuit/three_phase_abc/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/short_circuit/three_phase_abc/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/short_circuit/three_phase_abc/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/short_circuit/three_phase_abc/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)    58916 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/short_circuit/three_phase_abc/sc_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/short_circuit/three_phase_abc/sc_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     5234 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/short_circuit/three_phase_abc/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/short_circuit/three_phase_abc/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:08:40.659107 power-grid-model-1.5.0rc9192016554667/tests/data/short_circuit/two_phase_ab/
--rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/short_circuit/two_phase_ab/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/short_circuit/two_phase_ab/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/short_circuit/two_phase_ab/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/short_circuit/two_phase_ab/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)    59750 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/short_circuit/two_phase_ab/sc_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/short_circuit/two_phase_ab/sc_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     5234 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/short_circuit/two_phase_ab/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/short_circuit/two_phase_ab/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:08:40.659107 power-grid-model-1.5.0rc9192016554667/tests/data/short_circuit/two_phase_ac/
--rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/short_circuit/two_phase_ac/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/short_circuit/two_phase_ac/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/short_circuit/two_phase_ac/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/short_circuit/two_phase_ac/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)    58820 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/short_circuit/two_phase_ac/sc_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/short_circuit/two_phase_ac/sc_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     5234 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/short_circuit/two_phase_ac/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/short_circuit/two_phase_ac/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:08:40.663107 power-grid-model-1.5.0rc9192016554667/tests/data/short_circuit/two_phase_bc/
--rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/short_circuit/two_phase_bc/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/short_circuit/two_phase_bc/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/short_circuit/two_phase_bc/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/short_circuit/two_phase_bc/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)    58892 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/short_circuit/two_phase_bc/sc_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/short_circuit/two_phase_bc/sc_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     5234 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/short_circuit/two_phase_bc/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/short_circuit/two_phase_bc/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:08:40.663107 power-grid-model-1.5.0rc9192016554667/tests/data/short_circuit/two_phase_to_ground_ab/
--rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/short_circuit/two_phase_to_ground_ab/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/short_circuit/two_phase_to_ground_ab/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/short_circuit/two_phase_to_ground_ab/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/short_circuit/two_phase_to_ground_ab/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)    60848 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/short_circuit/two_phase_to_ground_ab/sc_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/short_circuit/two_phase_to_ground_ab/sc_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     5234 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/short_circuit/two_phase_to_ground_ab/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/short_circuit/two_phase_to_ground_ab/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:08:40.667107 power-grid-model-1.5.0rc9192016554667/tests/data/short_circuit/two_phase_to_ground_ac/
--rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/short_circuit/two_phase_to_ground_ac/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/short_circuit/two_phase_to_ground_ac/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/short_circuit/two_phase_to_ground_ac/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/short_circuit/two_phase_to_ground_ac/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)    60752 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/short_circuit/two_phase_to_ground_ac/sc_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/short_circuit/two_phase_to_ground_ac/sc_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     5234 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/short_circuit/two_phase_to_ground_ac/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/short_circuit/two_phase_to_ground_ac/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:08:40.667107 power-grid-model-1.5.0rc9192016554667/tests/data/short_circuit/two_phase_to_ground_bc/
--rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/short_circuit/two_phase_to_ground_bc/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/short_circuit/two_phase_to_ground_bc/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/short_circuit/two_phase_to_ground_bc/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/short_circuit/two_phase_to_ground_bc/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)    60554 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/short_circuit/two_phase_to_ground_bc/sc_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/short_circuit/two_phase_to_ground_bc/sc_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     5234 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/short_circuit/two_phase_to_ground_bc/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/short_circuit/two_phase_to_ground_bc/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:08:40.535108 power-grid-model-1.5.0rc9192016554667/tests/data/state_estimation/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:08:40.667107 power-grid-model-1.5.0rc9192016554667/tests/data/state_estimation/1os2msr/
--rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/state_estimation/1os2msr/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/state_estimation/1os2msr/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/state_estimation/1os2msr/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/state_estimation/1os2msr/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/state_estimation/1os2msr/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/state_estimation/1os2msr/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:08:40.671107 power-grid-model-1.5.0rc9192016554667/tests/data/state_estimation/1os2msr-no-angle/
--rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/state_estimation/1os2msr-no-angle/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/state_estimation/1os2msr-no-angle/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/state_estimation/1os2msr-no-angle/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/state_estimation/1os2msr-no-angle/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/state_estimation/1os2msr-no-angle/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/state_estimation/1os2msr-no-angle/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:08:40.671107 power-grid-model-1.5.0rc9192016554667/tests/data/state_estimation/distribution-case/
--rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/state_estimation/distribution-case/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     8939 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/state_estimation/distribution-case/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/state_estimation/distribution-case/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/state_estimation/distribution-case/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/state_estimation/distribution-case/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)    19468 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/state_estimation/distribution-case/sym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/state_estimation/distribution-case/sym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     6642 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/state_estimation/distribution-case/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/state_estimation/distribution-case/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:08:40.671107 power-grid-model-1.5.0rc9192016554667/tests/data/state_estimation/dummy-test-sym/
--rw-r--r--   0 runner    (1001) docker     (123)     3196 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/state_estimation/dummy-test-sym/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/state_estimation/dummy-test-sym/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/state_estimation/dummy-test-sym/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/state_estimation/dummy-test-sym/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/state_estimation/dummy-test-sym/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/state_estimation/dummy-test-sym/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:08:40.675107 power-grid-model-1.5.0rc9192016554667/tests/data/state_estimation/node-injection-sensor-and-zero-injection/
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/state_estimation/node-injection-sensor-and-zero-injection/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/state_estimation/node-injection-sensor-and-zero-injection/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/state_estimation/node-injection-sensor-and-zero-injection/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/state_estimation/node-injection-sensor-and-zero-injection/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/state_estimation/node-injection-sensor-and-zero-injection/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/state_estimation/node-injection-sensor-and-zero-injection/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:08:40.675107 power-grid-model-1.5.0rc9192016554667/tests/data/state_estimation/residual-test/
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/state_estimation/residual-test/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/state_estimation/residual-test/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/state_estimation/residual-test/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/state_estimation/residual-test/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/state_estimation/residual-test/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/state_estimation/residual-test/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:08:40.675107 power-grid-model-1.5.0rc9192016554667/tests/data/state_estimation/single-line-load/
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/state_estimation/single-line-load/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/state_estimation/single-line-load/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/state_estimation/single-line-load/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/state_estimation/single-line-load/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/state_estimation/single-line-load/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/state_estimation/single-line-load/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:08:40.675107 power-grid-model-1.5.0rc9192016554667/tests/data/state_estimation/three_winding_transformer/
--rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/state_estimation/three_winding_transformer/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/state_estimation/three_winding_transformer/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/state_estimation/three_winding_transformer/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/state_estimation/three_winding_transformer/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/state_estimation/three_winding_transformer/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/state_estimation/three_winding_transformer/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:08:40.679107 power-grid-model-1.5.0rc9192016554667/tests/data/state_estimation/transmission-case/
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/state_estimation/transmission-case/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    29158 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/state_estimation/transmission-case/asym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/state_estimation/transmission-case/asym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)    11996 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/state_estimation/transmission-case/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/state_estimation/transmission-case/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/state_estimation/transmission-case/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/state_estimation/transmission-case/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     7827 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/state_estimation/transmission-case/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/data/state_estimation/transmission-case/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:08:40.679107 power-grid-model-1.5.0rc9192016554667/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/unit/test_0Z_model_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/unit/test_error_handling.py
--rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/unit/test_meta_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     6422 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/unit/test_power_grid_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    20807 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/unit/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7996 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/unit/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:08:40.679107 power-grid-model-1.5.0rc9192016554667/tests/unit/validation/
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/unit/validation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/unit/validation/test_assertions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/unit/validation/test_batch_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4855 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/unit/validation/test_errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    27362 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/unit/validation/test_input_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)    14325 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/unit/validation/test_rules.py
--rw-r--r--   0 runner    (1001) docker     (123)     6991 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/unit/validation/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    23023 2023-06-27 09:07:49.000000 power-grid-model-1.5.0rc9192016554667/tests/unit/validation/test_validation_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:07:47.055650 power-grid-model-1.5.0rc9193215149708/
+-rw-r--r--   0 runner    (1001) docker     (123)    14907 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8142 2023-06-27 12:07:47.055650 power-grid-model-1.5.0rc9193215149708/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-27 12:06:54.000000 power-grid-model-1.5.0rc9193215149708/PYPI_VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)     6818 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:07:46.903649 power-grid-model-1.5.0rc9193215149708/power_grid_model_c/
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/power_grid_model_c/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:07:46.903649 power-grid-model-1.5.0rc9193215149708/power_grid_model_c/power_grid_model/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/power_grid_model_c/power_grid_model/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:07:46.891649 power-grid-model-1.5.0rc9193215149708/power_grid_model_c/power_grid_model/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:07:46.903649 power-grid-model-1.5.0rc9193215149708/power_grid_model_c/power_grid_model/include/power_grid_model/
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/power_grid_model_c/power_grid_model/include/power_grid_model/all_components.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:07:46.907649 power-grid-model-1.5.0rc9193215149708/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/
+-rw-r--r--   0 runner    (1001) docker     (123)     4229 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/dataset.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    28563 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/input.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    10354 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_data.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_data_gen.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    17078 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/output.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     9396 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/update.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     9108 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/power_grid_model_c/power_grid_model/include/power_grid_model/calculation_parameters.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:07:46.911650 power-grid-model-1.5.0rc9193215149708/power_grid_model_c/power_grid_model/include/power_grid_model/component/
+-rw-r--r--   0 runner    (1001) docker     (123)     4215 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/power_grid_model_c/power_grid_model/include/power_grid_model/component/appliance.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/power_grid_model_c/power_grid_model/include/power_grid_model/component/base.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     8941 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/power_grid_model_c/power_grid_model/include/power_grid_model/component/branch.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6790 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/power_grid_model_c/power_grid_model/include/power_grid_model/component/branch3.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4455 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/power_grid_model_c/power_grid_model/include/power_grid_model/component/fault.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2329 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/power_grid_model_c/power_grid_model/include/power_grid_model/component/line.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/power_grid_model_c/power_grid_model/include/power_grid_model/component/link.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5353 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/power_grid_model_c/power_grid_model/include/power_grid_model/component/load_gen.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/power_grid_model_c/power_grid_model/include/power_grid_model/component/node.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4793 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/power_grid_model_c/power_grid_model/include/power_grid_model/component/power_sensor.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/power_grid_model_c/power_grid_model/include/power_grid_model/component/sensor.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2883 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/power_grid_model_c/power_grid_model/include/power_grid_model/component/shunt.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4406 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/power_grid_model_c/power_grid_model/include/power_grid_model/component/source.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    20067 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/power_grid_model_c/power_grid_model/include/power_grid_model/component/three_winding_transformer.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    10964 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/power_grid_model_c/power_grid_model/include/power_grid_model/component/transformer.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/power_grid_model_c/power_grid_model/include/power_grid_model/component/transformer_utils.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5599 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/power_grid_model_c/power_grid_model/include/power_grid_model/component/voltage_sensor.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    15128 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/power_grid_model_c/power_grid_model/include/power_grid_model/container.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/power_grid_model_c/power_grid_model/include/power_grid_model/enum.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5347 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/power_grid_model_c/power_grid_model/include/power_grid_model/exception.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    67948 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/power_grid_model_c/power_grid_model/include/power_grid_model/main_model.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:07:46.911650 power-grid-model-1.5.0rc9193215149708/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/
+-rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/block_matrix.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     8954 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/iterative_current_pf_solver.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    41694 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/iterative_linear_se_solver.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7164 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/iterative_pf_solver.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6446 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/linear_pf_solver.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6192 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/math_solver.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    16064 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/newton_raphson_pf_solver.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    16203 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/sparse_lu_solver.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    20157 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/y_bus.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3055 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/power_grid_model_c/power_grid_model/include/power_grid_model/power_grid_model.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2753 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/power_grid_model_c/power_grid_model/include/power_grid_model/sparse_mapping.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    11399 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/power_grid_model_c/power_grid_model/include/power_grid_model/three_phase_tensor.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/power_grid_model_c/power_grid_model/include/power_grid_model/timer.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    30818 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/power_grid_model_c/power_grid_model/include/power_grid_model/topology.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:07:46.911650 power-grid-model-1.5.0rc9193215149708/power_grid_model_c/power_grid_model_c/
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/power_grid_model_c/power_grid_model_c/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:07:46.911650 power-grid-model-1.5.0rc9193215149708/power_grid_model_c/power_grid_model_c/include/
+-rw-r--r--   0 runner    (1001) docker     (123)    26155 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/power_grid_model_c/power_grid_model_c/include/power_grid_model_c.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15811 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/power_grid_model_c/power_grid_model_c/power_grid_model_c.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3634 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 12:07:47.055650 power-grid-model-1.5.0rc9193215149708/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     7078 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:07:46.891649 power-grid-model-1.5.0rc9193215149708/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:07:46.915650 power-grid-model-1.5.0rc9193215149708/src/power_grid_model/
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/src/power_grid_model/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:07:46.915650 power-grid-model-1.5.0rc9193215149708/src/power_grid_model/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/src/power_grid_model/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/src/power_grid_model/core/error_handling.py
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/src/power_grid_model/core/index_integer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/src/power_grid_model/core/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9994 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/src/power_grid_model/core/power_grid_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9240 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/src/power_grid_model/core/power_grid_meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17761 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/src/power_grid_model/core/power_grid_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5239 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/src/power_grid_model/data_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/src/power_grid_model/enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/src/power_grid_model/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21645 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/src/power_grid_model/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:07:46.919649 power-grid-model-1.5.0rc9193215149708/src/power_grid_model/validation/
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/src/power_grid_model/validation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4166 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/src/power_grid_model/validation/assertions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14686 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/src/power_grid_model/validation/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30704 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/src/power_grid_model/validation/rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8601 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/src/power_grid_model/validation/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28618 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/src/power_grid_model/validation/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:07:46.915650 power-grid-model-1.5.0rc9193215149708/src/power_grid_model.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8142 2023-06-27 12:07:46.000000 power-grid-model-1.5.0rc9193215149708/src/power_grid_model.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    37053 2023-06-27 12:07:46.000000 power-grid-model-1.5.0rc9193215149708/src/power_grid_model.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 12:07:46.000000 power-grid-model-1.5.0rc9193215149708/src/power_grid_model.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-06-27 12:07:46.000000 power-grid-model-1.5.0rc9193215149708/src/power_grid_model.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-27 12:07:46.000000 power-grid-model-1.5.0rc9193215149708/src/power_grid_model.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:07:46.899649 power-grid-model-1.5.0rc9193215149708/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:07:46.899649 power-grid-model-1.5.0rc9193215149708/tests/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:07:46.895650 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:07:46.919649 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/1os2msr/
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/1os2msr/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/1os2msr/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/1os2msr/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/1os2msr/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/1os2msr/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/1os2msr/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:07:46.919649 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/dummy-test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/dummy-test/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/dummy-test/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/dummy-test/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/dummy-test/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/dummy-test/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/dummy-test/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:07:46.923650 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/dummy-test-batch/
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/dummy-test-batch/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/dummy-test-batch/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/dummy-test-batch/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/dummy-test-batch/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/dummy-test-batch/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/dummy-test-batch/sym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/dummy-test-batch/sym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/dummy-test-batch/sym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/dummy-test-batch/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/dummy-test-batch/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:07:46.927650 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/dummy-test-batch-dependent-cacheable/
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/dummy-test-batch-dependent-cacheable/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/dummy-test-batch-dependent-cacheable/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/dummy-test-batch-dependent-cacheable/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/dummy-test-batch-dependent-cacheable/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/dummy-test-batch-dependent-cacheable/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/dummy-test-batch-dependent-cacheable/sym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/dummy-test-batch-dependent-cacheable/sym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/dummy-test-batch-dependent-cacheable/sym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/dummy-test-batch-dependent-cacheable/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/dummy-test-batch-dependent-cacheable/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:07:46.927650 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/sym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/sym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/sym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:07:46.927650 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/dummy-test-batch-incomplete-input/
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/dummy-test-batch-incomplete-input/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/dummy-test-batch-incomplete-input/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/dummy-test-batch-incomplete-input/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/dummy-test-batch-incomplete-input/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/dummy-test-batch-incomplete-input/sym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/dummy-test-batch-incomplete-input/sym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/dummy-test-batch-incomplete-input/sym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/dummy-test-batch-incomplete-input/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/dummy-test-batch-incomplete-input/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:07:46.931650 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/dummy-test-batch-independent-cacheable/
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/dummy-test-batch-independent-cacheable/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/dummy-test-batch-independent-cacheable/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/dummy-test-batch-independent-cacheable/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/dummy-test-batch-independent-cacheable/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/dummy-test-batch-independent-cacheable/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/dummy-test-batch-independent-cacheable/sym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/dummy-test-batch-independent-cacheable/sym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/dummy-test-batch-independent-cacheable/sym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/dummy-test-batch-independent-cacheable/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/dummy-test-batch-independent-cacheable/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:07:46.935650 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/sym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/sym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/sym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:07:46.935650 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/dummy-test-batch-newton/
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/dummy-test-batch-newton/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/dummy-test-batch-newton/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/dummy-test-batch-newton/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/dummy-test-batch-newton/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/dummy-test-batch-newton/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/dummy-test-batch-newton/sym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/dummy-test-batch-newton/sym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/dummy-test-batch-newton/sym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/dummy-test-batch-newton/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/dummy-test-batch-newton/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:07:46.939650 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/dummy-test-i-n-optional/
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/dummy-test-i-n-optional/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/dummy-test-i-n-optional/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/dummy-test-i-n-optional/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/dummy-test-i-n-optional/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/dummy-test-i-n-optional/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/dummy-test-i-n-optional/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:07:46.943650 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/gaia-example/
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/gaia-example/asym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/gaia-example/asym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/gaia-example/gaia_grid.gnf
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/gaia-example/gaia_grid.gnf.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/gaia-example/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/gaia-example/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/gaia-example/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/gaia-example/params.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:07:46.943650 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/multi-source-with-angle/
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/multi-source-with-angle/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/multi-source-with-angle/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/multi-source-with-angle/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/multi-source-with-angle/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/multi-source-with-angle/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/multi-source-with-angle/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:07:46.895650 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:07:46.895650 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/components/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:07:46.895650 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/components/asymmetric/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:07:46.947650 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/asym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/asym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/params.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:07:46.947650 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/components/asymmetric/asym_load/
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/components/asymmetric/asym_load/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/components/asymmetric/asym_load/asym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/components/asymmetric/asym_load/asym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/components/asymmetric/asym_load/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/components/asymmetric/asym_load/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/components/asymmetric/asym_load/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/components/asymmetric/asym_load/params.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:07:46.951650 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/components/asymmetric/line/
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/components/asymmetric/line/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/components/asymmetric/line/asym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/components/asymmetric/line/asym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/components/asymmetric/line/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/components/asymmetric/line/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/components/asymmetric/line/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/components/asymmetric/line/params.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:07:46.951650 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/components/asymmetric/node/
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/components/asymmetric/node/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/components/asymmetric/node/asym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/components/asymmetric/node/asym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/components/asymmetric/node/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/components/asymmetric/node/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/components/asymmetric/node/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/components/asymmetric/node/params.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:07:46.951650 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/components/asymmetric/shunt/
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/components/asymmetric/shunt/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/components/asymmetric/shunt/asym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/components/asymmetric/shunt/asym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/components/asymmetric/shunt/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/components/asymmetric/shunt/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/components/asymmetric/shunt/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/components/asymmetric/shunt/params.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:07:46.955650 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/components/asymmetric/source/
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/components/asymmetric/source/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/components/asymmetric/source/asym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/components/asymmetric/source/asym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/components/asymmetric/source/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/components/asymmetric/source/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/components/asymmetric/source/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/components/asymmetric/source/params.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:07:46.955650 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/asym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/asym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/params.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:07:46.959650 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/components/asymmetric/sym_load/
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/components/asymmetric/sym_load/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/components/asymmetric/sym_load/asym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/components/asymmetric/sym_load/asym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/components/asymmetric/sym_load/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/components/asymmetric/sym_load/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/components/asymmetric/sym_load/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/components/asymmetric/sym_load/params.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:07:46.963650 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/components/asymmetric/transformer/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/components/asymmetric/transformer/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    17633 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/components/asymmetric/transformer/asym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/components/asymmetric/transformer/asym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/components/asymmetric/transformer/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/components/asymmetric/transformer/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/components/asymmetric/transformer/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/components/asymmetric/transformer/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/components/asymmetric/transformer/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/components/asymmetric/transformer/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:07:46.895650 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/components/symmetric/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:07:46.963650 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/components/symmetric/basic-node/
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/components/symmetric/basic-node/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/components/symmetric/basic-node/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/components/symmetric/basic-node/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/components/symmetric/basic-node/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/components/symmetric/basic-node/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/components/symmetric/basic-node/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/components/symmetric/basic-node/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:07:46.967650 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/components/symmetric/line/
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/components/symmetric/line/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/components/symmetric/line/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/components/symmetric/line/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/components/symmetric/line/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/components/symmetric/line/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/components/symmetric/line/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/components/symmetric/line/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:07:46.971650 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/components/symmetric/node/
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/components/symmetric/node/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/components/symmetric/node/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/components/symmetric/node/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/components/symmetric/node/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/components/symmetric/node/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/components/symmetric/node/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/components/symmetric/node/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:07:46.971650 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/components/symmetric/shunt/
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/components/symmetric/shunt/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      892 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/components/symmetric/shunt/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/components/symmetric/shunt/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/components/symmetric/shunt/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/components/symmetric/shunt/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/components/symmetric/shunt/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/components/symmetric/shunt/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:07:46.975650 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/components/symmetric/source/
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/components/symmetric/source/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/components/symmetric/source/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/components/symmetric/source/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/components/symmetric/source/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/components/symmetric/source/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/components/symmetric/source/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/components/symmetric/source/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:07:46.975650 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/components/symmetric/sym_gen/
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/components/symmetric/sym_gen/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/components/symmetric/sym_gen/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/components/symmetric/sym_gen/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/components/symmetric/sym_gen/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/components/symmetric/sym_gen/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/components/symmetric/sym_gen/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/components/symmetric/sym_gen/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:07:46.979650 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/components/symmetric/sym_load/
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/components/symmetric/sym_load/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/components/symmetric/sym_load/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/components/symmetric/sym_load/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/components/symmetric/sym_load/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/components/symmetric/sym_load/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/components/symmetric/sym_load/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/components/symmetric/sym_load/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:07:46.979650 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     8883 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/sym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/sym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:07:46.983650 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/components/symmetric/transformer/
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/components/symmetric/transformer/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/components/symmetric/transformer/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/components/symmetric/transformer/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/components/symmetric/transformer/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/components/symmetric/transformer/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)    15639 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/components/symmetric/transformer/sym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/components/symmetric/transformer/sym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     2827 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/components/symmetric/transformer/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/components/symmetric/transformer/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:07:46.895650 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/networks/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:07:46.895650 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/networks/asymmetric/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:07:46.983650 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    15865 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/asym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/asym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     8935 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     6642 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:07:46.987650 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10605 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/asym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/asym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     6208 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/params.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:07:46.895650 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/networks/symmetric/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:07:46.991650 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/
+-rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     8939 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     8702 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/sym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/sym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     6642 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:07:46.991650 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6216 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5384 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:07:46.995650 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/r-state-estimation/
+-rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/r-state-estimation/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/r-state-estimation/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/r-state-estimation/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/r-state-estimation/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/r-state-estimation/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/r-state-estimation/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:07:47.003650 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/three-winding-transformer/
+-rw-r--r--   0 runner    (1001) docker     (123)    21196 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/three-winding-transformer/asym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/three-winding-transformer/asym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/three-winding-transformer/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/three-winding-transformer/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/three-winding-transformer/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/three-winding-transformer/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     7374 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/three-winding-transformer/sym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/three-winding-transformer/sym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/three-winding-transformer/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/three-winding-transformer/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:07:47.003650 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/vision-example/
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/vision-example/asym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/vision-example/asym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/vision-example/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/vision-example/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/vision-example/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/vision-example/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     2450 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/vision-example/vision_grid.vnf
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/vision-example/vision_grid.vnf.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:07:47.007650 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/vision-validation-network/
+-rw-r--r--   0 runner    (1001) docker     (123)    20486 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/vision-validation-network/asym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/vision-validation-network/asym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)    30756 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/vision-validation-network/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/vision-validation-network/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/vision-validation-network/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/vision-validation-network/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)    11853 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/vision-validation-network/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/vision-validation-network/sym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)    35119 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/vision-validation-network/vision_validation_network.vnf
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/vision-validation-network/vision_validation_network.vnf.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:07:46.899649 power-grid-model-1.5.0rc9193215149708/tests/data/short_circuit/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:07:47.011650 power-grid-model-1.5.0rc9193215149708/tests/data/short_circuit/single_phase_to_ground_a/
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/short_circuit/single_phase_to_ground_a/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/short_circuit/single_phase_to_ground_a/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/short_circuit/single_phase_to_ground_a/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/short_circuit/single_phase_to_ground_a/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)    60794 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/short_circuit/single_phase_to_ground_a/sc_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/short_circuit/single_phase_to_ground_a/sc_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5234 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/short_circuit/single_phase_to_ground_a/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/short_circuit/single_phase_to_ground_a/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:07:47.015650 power-grid-model-1.5.0rc9193215149708/tests/data/short_circuit/single_phase_to_ground_b/
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/short_circuit/single_phase_to_ground_b/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/short_circuit/single_phase_to_ground_b/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/short_circuit/single_phase_to_ground_b/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/short_circuit/single_phase_to_ground_b/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)    60980 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/short_circuit/single_phase_to_ground_b/sc_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/short_circuit/single_phase_to_ground_b/sc_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5234 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/short_circuit/single_phase_to_ground_b/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/short_circuit/single_phase_to_ground_b/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:07:47.015650 power-grid-model-1.5.0rc9193215149708/tests/data/short_circuit/single_phase_to_ground_c/
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/short_circuit/single_phase_to_ground_c/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/short_circuit/single_phase_to_ground_c/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/short_circuit/single_phase_to_ground_c/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/short_circuit/single_phase_to_ground_c/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)    60938 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/short_circuit/single_phase_to_ground_c/sc_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/short_circuit/single_phase_to_ground_c/sc_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5234 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/short_circuit/single_phase_to_ground_c/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/short_circuit/single_phase_to_ground_c/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:07:47.019650 power-grid-model-1.5.0rc9193215149708/tests/data/short_circuit/three_phase_abc/
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/short_circuit/three_phase_abc/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/short_circuit/three_phase_abc/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/short_circuit/three_phase_abc/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/short_circuit/three_phase_abc/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)    58916 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/short_circuit/three_phase_abc/sc_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/short_circuit/three_phase_abc/sc_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5234 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/short_circuit/three_phase_abc/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/short_circuit/three_phase_abc/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:07:47.023650 power-grid-model-1.5.0rc9193215149708/tests/data/short_circuit/two_phase_ab/
+-rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/short_circuit/two_phase_ab/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/short_circuit/two_phase_ab/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/short_circuit/two_phase_ab/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/short_circuit/two_phase_ab/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)    59750 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/short_circuit/two_phase_ab/sc_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/short_circuit/two_phase_ab/sc_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5234 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/short_circuit/two_phase_ab/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/short_circuit/two_phase_ab/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:07:47.023650 power-grid-model-1.5.0rc9193215149708/tests/data/short_circuit/two_phase_ac/
+-rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/short_circuit/two_phase_ac/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/short_circuit/two_phase_ac/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/short_circuit/two_phase_ac/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/short_circuit/two_phase_ac/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)    58820 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/short_circuit/two_phase_ac/sc_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/short_circuit/two_phase_ac/sc_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5234 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/short_circuit/two_phase_ac/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/short_circuit/two_phase_ac/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:07:47.027650 power-grid-model-1.5.0rc9193215149708/tests/data/short_circuit/two_phase_bc/
+-rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/short_circuit/two_phase_bc/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/short_circuit/two_phase_bc/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/short_circuit/two_phase_bc/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/short_circuit/two_phase_bc/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)    58892 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/short_circuit/two_phase_bc/sc_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/short_circuit/two_phase_bc/sc_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5234 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/short_circuit/two_phase_bc/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/short_circuit/two_phase_bc/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:07:47.031650 power-grid-model-1.5.0rc9193215149708/tests/data/short_circuit/two_phase_to_ground_ab/
+-rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/short_circuit/two_phase_to_ground_ab/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/short_circuit/two_phase_to_ground_ab/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/short_circuit/two_phase_to_ground_ab/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/short_circuit/two_phase_to_ground_ab/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)    60848 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/short_circuit/two_phase_to_ground_ab/sc_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/short_circuit/two_phase_to_ground_ab/sc_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5234 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/short_circuit/two_phase_to_ground_ab/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/short_circuit/two_phase_to_ground_ab/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:07:47.031650 power-grid-model-1.5.0rc9193215149708/tests/data/short_circuit/two_phase_to_ground_ac/
+-rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/short_circuit/two_phase_to_ground_ac/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/short_circuit/two_phase_to_ground_ac/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/short_circuit/two_phase_to_ground_ac/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/short_circuit/two_phase_to_ground_ac/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)    60752 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/short_circuit/two_phase_to_ground_ac/sc_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/short_circuit/two_phase_to_ground_ac/sc_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5234 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/short_circuit/two_phase_to_ground_ac/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/short_circuit/two_phase_to_ground_ac/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:07:47.035650 power-grid-model-1.5.0rc9193215149708/tests/data/short_circuit/two_phase_to_ground_bc/
+-rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/short_circuit/two_phase_to_ground_bc/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/short_circuit/two_phase_to_ground_bc/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/short_circuit/two_phase_to_ground_bc/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/short_circuit/two_phase_to_ground_bc/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)    60554 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/short_circuit/two_phase_to_ground_bc/sc_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/short_circuit/two_phase_to_ground_bc/sc_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5234 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/short_circuit/two_phase_to_ground_bc/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/short_circuit/two_phase_to_ground_bc/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:07:46.899649 power-grid-model-1.5.0rc9193215149708/tests/data/state_estimation/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:07:47.035650 power-grid-model-1.5.0rc9193215149708/tests/data/state_estimation/1os2msr/
+-rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/state_estimation/1os2msr/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/state_estimation/1os2msr/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/state_estimation/1os2msr/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/state_estimation/1os2msr/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/state_estimation/1os2msr/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/state_estimation/1os2msr/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:07:47.039650 power-grid-model-1.5.0rc9193215149708/tests/data/state_estimation/1os2msr-no-angle/
+-rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/state_estimation/1os2msr-no-angle/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/state_estimation/1os2msr-no-angle/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/state_estimation/1os2msr-no-angle/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/state_estimation/1os2msr-no-angle/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/state_estimation/1os2msr-no-angle/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/state_estimation/1os2msr-no-angle/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:07:47.039650 power-grid-model-1.5.0rc9193215149708/tests/data/state_estimation/distribution-case/
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/state_estimation/distribution-case/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     8939 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/state_estimation/distribution-case/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/state_estimation/distribution-case/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/state_estimation/distribution-case/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/state_estimation/distribution-case/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)    19468 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/state_estimation/distribution-case/sym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/state_estimation/distribution-case/sym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     6642 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/state_estimation/distribution-case/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/state_estimation/distribution-case/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:07:47.043650 power-grid-model-1.5.0rc9193215149708/tests/data/state_estimation/dummy-test-sym/
+-rw-r--r--   0 runner    (1001) docker     (123)     3196 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/state_estimation/dummy-test-sym/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/state_estimation/dummy-test-sym/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/state_estimation/dummy-test-sym/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/state_estimation/dummy-test-sym/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/state_estimation/dummy-test-sym/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/state_estimation/dummy-test-sym/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:07:47.043650 power-grid-model-1.5.0rc9193215149708/tests/data/state_estimation/node-injection-sensor-and-zero-injection/
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/state_estimation/node-injection-sensor-and-zero-injection/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/state_estimation/node-injection-sensor-and-zero-injection/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/state_estimation/node-injection-sensor-and-zero-injection/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/state_estimation/node-injection-sensor-and-zero-injection/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/state_estimation/node-injection-sensor-and-zero-injection/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/state_estimation/node-injection-sensor-and-zero-injection/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:07:47.043650 power-grid-model-1.5.0rc9193215149708/tests/data/state_estimation/residual-test/
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/state_estimation/residual-test/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/state_estimation/residual-test/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/state_estimation/residual-test/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/state_estimation/residual-test/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/state_estimation/residual-test/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/state_estimation/residual-test/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:07:47.047650 power-grid-model-1.5.0rc9193215149708/tests/data/state_estimation/single-line-load/
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/state_estimation/single-line-load/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/state_estimation/single-line-load/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/state_estimation/single-line-load/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/state_estimation/single-line-load/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/state_estimation/single-line-load/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/state_estimation/single-line-load/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:07:47.047650 power-grid-model-1.5.0rc9193215149708/tests/data/state_estimation/three_winding_transformer/
+-rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/state_estimation/three_winding_transformer/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/state_estimation/three_winding_transformer/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/state_estimation/three_winding_transformer/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/state_estimation/three_winding_transformer/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/state_estimation/three_winding_transformer/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/state_estimation/three_winding_transformer/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:07:47.051650 power-grid-model-1.5.0rc9193215149708/tests/data/state_estimation/transmission-case/
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/state_estimation/transmission-case/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    29158 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/state_estimation/transmission-case/asym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/state_estimation/transmission-case/asym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)    11996 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/state_estimation/transmission-case/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/state_estimation/transmission-case/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/state_estimation/transmission-case/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/state_estimation/transmission-case/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     7827 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/state_estimation/transmission-case/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/data/state_estimation/transmission-case/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:07:47.051650 power-grid-model-1.5.0rc9193215149708/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/unit/test_0Z_model_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/unit/test_error_handling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/unit/test_meta_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6422 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/unit/test_power_grid_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20807 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/unit/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7996 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/unit/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:07:47.051650 power-grid-model-1.5.0rc9193215149708/tests/unit/validation/
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/unit/validation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/unit/validation/test_assertions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/unit/validation/test_batch_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4855 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/unit/validation/test_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27362 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/unit/validation/test_input_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14325 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/unit/validation/test_rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6991 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/unit/validation/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23023 2023-06-27 12:06:49.000000 power-grid-model-1.5.0rc9193215149708/tests/unit/validation/test_validation_functions.py
```

### Comparing `power-grid-model-1.5.0rc9192016554667/LICENSE` & `power-grid-model-1.5.0rc9193215149708/LICENSE`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9192016554667/PKG-INFO` & `power-grid-model-1.5.0rc9193215149708/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: power-grid-model
-Version: 1.5.0rc9192016554667
+Version: 1.5.0rc9193215149708
 Summary: Python/C++ library for distribution power system analysis
 Author-email: Alliander Dynamic Grid Calculation <dynamic.grid.calculation@alliander.com>
 License: MPL-2.0
 Project-URL: Home-page, https://lfenergy.org/projects/power-grid-model/
 Project-URL: GitHub, https://github.com/PowerGridModel/power-grid-model
 Project-URL: Documentation, https://power-grid-model.readthedocs.io/en/stable/
 Project-URL: Mailing-list, https://lists.lfenergy.org/g/powergridmodel
```

### Comparing `power-grid-model-1.5.0rc9192016554667/README.md` & `power-grid-model-1.5.0rc9193215149708/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9192016554667/power_grid_model_c/power_grid_model/CMakeLists.txt` & `power-grid-model-1.5.0rc9193215149708/power_grid_model_c/power_grid_model/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9192016554667/power_grid_model_c/power_grid_model/include/power_grid_model/all_components.hpp` & `power-grid-model-1.5.0rc9193215149708/power_grid_model_c/power_grid_model/include/power_grid_model/all_components.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9192016554667/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/dataset.hpp` & `power-grid-model-1.5.0rc9193215149708/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/dataset.hpp`

 * *Files 0% similar despite different names*

```diff
@@ -103,15 +103,15 @@
         else {
             return batch_size_ == 0 || elements_per_scenario_ == 0;
         }
     }
 
     // conversion to const iterator
     template <class UX = DataPointer<true>>
-    requires(!is_const) operator UX() const {
+    requires(!is_const) explicit operator UX() const {
         return DataPointer<true>{ptr_, indptr_, batch_size_, elements_per_scenario_};
     }
 
    private:
     ptr_t<void> ptr_;
     Idx const* indptr_;
     Idx batch_size_;             // number of batches
```

### Comparing `power-grid-model-1.5.0rc9192016554667/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/input.hpp` & `power-grid-model-1.5.0rc9193215149708/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/input.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9192016554667/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_data.hpp` & `power-grid-model-1.5.0rc9193215149708/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_data.hpp`

 * *Files 22% similar despite different names*

```diff
@@ -22,100 +22,106 @@
 struct trait_pointer_to_member;
 template <class StructType, class ValueType>
 struct trait_pointer_to_member<ValueType StructType::*> {
     using struct_type = StructType;
     using value_type = ValueType;
 };
 
-using SetNaNFunc = std::add_pointer_t<void(void*)>;
-using CheckNaNFunc = std::add_pointer_t<bool(void const*)>;
-using SetValueFunc = std::add_pointer_t<void(void*, void const*)>;
-using CompareValueFunc = std::add_pointer_t<bool(void const* ptr_x, void const* ptr_y, double atol, double rtol)>;
+using RawDataPtr = void*;             // raw mutable data ptr
+using RawDataConstPtr = void const*;  // raw read-only data ptr
+
+using SetNaNFunc = std::add_pointer_t<void(RawDataPtr)>;
+using CheckNaNFunc = std::add_pointer_t<bool(RawDataConstPtr)>;
+using SetValueFunc = std::add_pointer_t<void(RawDataPtr, RawDataConstPtr)>;
+using CompareValueFunc =
+    std::add_pointer_t<bool(RawDataConstPtr ptr_x, RawDataConstPtr ptr_y, double atol, double rtol)>;
 
 template <class T>
-void set_value_template(void* dest, void const* src) {
+void set_value_template(RawDataPtr dest, RawDataConstPtr src) {
     *reinterpret_cast<T*>(dest) = *reinterpret_cast<T const*>(src);
 }
 
 constexpr std::array<size_t, 1> three_phase_dimension{3};
 
 template <class T, bool is_enum = std::is_enum_v<T>>
 struct data_type;
 
 template <>
 struct data_type<double, false> {
     static constexpr const char* numpy_type = "f8";
     static constexpr const char* ctype = "double";
     static constexpr size_t ndim = 0;
     static constexpr size_t const* dims = nullptr;
-    static constexpr SetNaNFunc set_nan = [](void* ptr) {
+    static constexpr SetNaNFunc set_nan = [](RawDataPtr ptr) {
         *reinterpret_cast<double*>(ptr) = nan;
     };
-    static constexpr CheckNaNFunc check_nan = [](void const* ptr) -> bool {
+    static constexpr CheckNaNFunc check_nan = [](RawDataConstPtr ptr) -> bool {
         return is_nan(*reinterpret_cast<double const*>(ptr));
     };
     static constexpr SetValueFunc set_value = set_value_template<double>;
-    static constexpr CompareValueFunc compare_value = [](void const* ptr_x, void const* ptr_y, double atol,
+    static constexpr CompareValueFunc compare_value = [](RawDataConstPtr ptr_x, RawDataConstPtr ptr_y, double atol,
                                                          double rtol) -> bool {
         double const x = *reinterpret_cast<double const*>(ptr_x);
         double const y = *reinterpret_cast<double const*>(ptr_y);
         return std::abs(y - x) < (std::abs(x) * rtol + atol);
     };
 };
 
 template <>
 struct data_type<int32_t, false> {
     static constexpr const char* numpy_type = "i4";
     static constexpr const char* ctype = "int32_t";
     static constexpr size_t ndim = 0;
     static constexpr size_t const* dims = nullptr;
-    static constexpr SetNaNFunc set_nan = [](void* ptr) {
+    static constexpr SetNaNFunc set_nan = [](RawDataPtr ptr) {
         *reinterpret_cast<int32_t*>(ptr) = na_IntID;
     };
-    static constexpr CheckNaNFunc check_nan = [](void const* ptr) -> bool {
+    static constexpr CheckNaNFunc check_nan = [](RawDataConstPtr ptr) -> bool {
         return *reinterpret_cast<int32_t const*>(ptr) == na_IntID;
     };
     static constexpr SetValueFunc set_value = set_value_template<int32_t>;
-    static constexpr CompareValueFunc compare_value = [](void const* ptr_x, void const* ptr_y, double, double) -> bool {
+    static constexpr CompareValueFunc compare_value = [](RawDataConstPtr ptr_x, RawDataConstPtr ptr_y, double,
+                                                         double) -> bool {
         return *reinterpret_cast<int32_t const*>(ptr_x) == *reinterpret_cast<int32_t const*>(ptr_y);
     };
 };
 
 template <>
 struct data_type<int8_t, false> {
     static constexpr const char* numpy_type = "i1";
     static constexpr const char* ctype = "int8_t";
     static constexpr size_t ndim = 0;
     static constexpr size_t const* dims = nullptr;
-    static constexpr SetNaNFunc set_nan = [](void* ptr) {
+    static constexpr SetNaNFunc set_nan = [](RawDataPtr ptr) {
         *reinterpret_cast<int8_t*>(ptr) = na_IntS;
     };
-    static constexpr CheckNaNFunc check_nan = [](void const* ptr) -> bool {
+    static constexpr CheckNaNFunc check_nan = [](RawDataConstPtr ptr) -> bool {
         return *reinterpret_cast<int8_t const*>(ptr) == na_IntS;
     };
     static constexpr SetValueFunc set_value = set_value_template<int8_t>;
-    static constexpr CompareValueFunc compare_value = [](void const* ptr_x, void const* ptr_y, double, double) -> bool {
+    static constexpr CompareValueFunc compare_value = [](RawDataConstPtr ptr_x, RawDataConstPtr ptr_y, double,
+                                                         double) -> bool {
         return *reinterpret_cast<int8_t const*>(ptr_x) == *reinterpret_cast<int8_t const*>(ptr_y);
     };
 };
 
 template <>
 struct data_type<RealValue<false>, false> {
     static constexpr const char* numpy_type = "f8";
     static constexpr const char* ctype = "double[3]";
     static constexpr size_t ndim = 1;
     static constexpr size_t const* dims = three_phase_dimension.data();
-    static constexpr SetNaNFunc set_nan = [](void* ptr) {
+    static constexpr SetNaNFunc set_nan = [](RawDataPtr ptr) {
         *reinterpret_cast<RealValue<false>*>(ptr) = RealValue<false>{nan, nan, nan};
     };
-    static constexpr CheckNaNFunc check_nan = [](void const* ptr) -> bool {
+    static constexpr CheckNaNFunc check_nan = [](RawDataConstPtr ptr) -> bool {
         return is_nan(*reinterpret_cast<RealValue<false> const*>(ptr));
     };
     static constexpr SetValueFunc set_value = set_value_template<RealValue<false>>;
-    static constexpr CompareValueFunc compare_value = [](void const* ptr_x, void const* ptr_y, double atol,
+    static constexpr CompareValueFunc compare_value = [](RawDataConstPtr ptr_x, RawDataConstPtr ptr_y, double atol,
                                                          double rtol) -> bool {
         RealValue<false> const x = *reinterpret_cast<RealValue<false> const*>(ptr_x);
         RealValue<false> const y = *reinterpret_cast<RealValue<false> const*>(ptr_y);
         return (abs(y - x) < (abs(x) * rtol + atol)).all();
     };
 };
 
@@ -192,54 +198,54 @@
         return -1;
     }
 
     bool has_attr(std::string const& attr_name) const {
         return find_attr(attr_name) >= 0;
     }
 
-    void* get_position(void* ptr, Idx position) const {
+    RawDataPtr get_position(RawDataPtr ptr, Idx position) const {
         return reinterpret_cast<char*>(ptr) + position * size;
     }
-    void const* get_position(void const* ptr, Idx position) const {
+    RawDataConstPtr get_position(RawDataConstPtr ptr, Idx position) const {
         return reinterpret_cast<char const*>(ptr) + position * size;
     }
 
     // set nan for all attributes
-    void set_nan(void* ptr, Idx position = 0) const {
+    void set_nan(RawDataPtr ptr, Idx position = 0) const {
         ptr = get_position(ptr, position);
         for (DataAttribute const& attr : attributes) {
             void* const offset_ptr = reinterpret_cast<char*>(ptr) + attr.offset;
             attr.set_nan(offset_ptr);
         }
     }
     // check nan for a attribute
-    bool check_nan(void const* ptr, DataAttribute const& attr, Idx position = 0) const {
+    bool check_nan(RawDataConstPtr ptr, DataAttribute const& attr, Idx position = 0) const {
         ptr = get_position(ptr, position);
-        void const* const offset_ptr = reinterpret_cast<char const*>(ptr) + attr.offset;
+        RawDataConstPtr const offset_ptr = reinterpret_cast<char const*>(ptr) + attr.offset;
         return attr.check_nan(offset_ptr);
     }
     // set value of one attribute
-    void set_attr(void* ptr, void const* value_ptr, DataAttribute const& attr, Idx position = 0) const {
+    void set_attr(RawDataPtr ptr, RawDataConstPtr value_ptr, DataAttribute const& attr, Idx position = 0) const {
         ptr = get_position(ptr, position);
         void* const offset_ptr = reinterpret_cast<char*>(ptr) + attr.offset;
         attr.set_value(offset_ptr, value_ptr);
     }
     // get value of one attribute
-    void get_attr(void const* ptr, void* value_ptr, DataAttribute const& attr, Idx position = 0) const {
+    void get_attr(RawDataConstPtr ptr, RawDataPtr value_ptr, DataAttribute const& attr, Idx position = 0) const {
         ptr = get_position(ptr, position);
-        void const* const offset_ptr = reinterpret_cast<char const*>(ptr) + attr.offset;
+        RawDataConstPtr const offset_ptr = reinterpret_cast<char const*>(ptr) + attr.offset;
         attr.set_value(value_ptr, offset_ptr);
     }
     // compare value of one attribute
-    bool compare_attr(void const* ptr_x, void const* ptr_y, double atol, double rtol, DataAttribute const& attr,
+    bool compare_attr(RawDataConstPtr ptr_x, RawDataConstPtr ptr_y, double atol, double rtol, DataAttribute const& attr,
                       Idx position = 0) const {
         ptr_x = get_position(ptr_x, position);
         ptr_y = get_position(ptr_y, position);
-        void const* const attr_ptr_x = reinterpret_cast<char const*>(ptr_x) + attr.offset;
-        void const* const attr_ptr_y = reinterpret_cast<char const*>(ptr_y) + attr.offset;
+        RawDataConstPtr const attr_ptr_x = reinterpret_cast<char const*>(ptr_x) + attr.offset;
+        RawDataConstPtr const attr_ptr_y = reinterpret_cast<char const*>(ptr_y) + attr.offset;
         return attr.compare_value(attr_ptr_x, attr_ptr_y, atol, rtol);
     }
 };
 
 using PowerGridMetaData = std::map<std::string, MetaData>;
 using AllPowerGridMetaData = std::map<std::string, PowerGridMetaData>;
```

### Comparing `power-grid-model-1.5.0rc9192016554667/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_data_gen.hpp` & `power-grid-model-1.5.0rc9193215149708/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_data_gen.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9192016554667/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/output.hpp` & `power-grid-model-1.5.0rc9193215149708/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/output.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9192016554667/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/update.hpp` & `power-grid-model-1.5.0rc9193215149708/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/update.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9192016554667/power_grid_model_c/power_grid_model/include/power_grid_model/calculation_parameters.hpp` & `power-grid-model-1.5.0rc9193215149708/power_grid_model_c/power_grid_model/include/power_grid_model/calculation_parameters.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9192016554667/power_grid_model_c/power_grid_model/include/power_grid_model/component/appliance.hpp` & `power-grid-model-1.5.0rc9193215149708/power_grid_model_c/power_grid_model/include/power_grid_model/component/appliance.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9192016554667/power_grid_model_c/power_grid_model/include/power_grid_model/component/base.hpp` & `power-grid-model-1.5.0rc9193215149708/power_grid_model_c/power_grid_model/include/power_grid_model/component/base.hpp`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     using InputType = BaseInput;
     using UpdateType = BaseUpdate;
     template <bool sym>
     using OutputType = BaseOutput;
     static constexpr char const* name = "base";
     virtual ComponentType math_model_type() const = 0;
 
-    Base(BaseInput const& base_input) : id_{base_input.id} {
+    explicit Base(BaseInput const& base_input) : id_{base_input.id} {
     }
     virtual ~Base() = default;
     ID id() const noexcept {
         return id_;
     }
     BaseOutput base_output(bool is_energized) const {
         return BaseOutput{id_, is_energized};
```

### Comparing `power-grid-model-1.5.0rc9192016554667/power_grid_model_c/power_grid_model/include/power_grid_model/component/branch.hpp` & `power-grid-model-1.5.0rc9193215149708/power_grid_model_c/power_grid_model/include/power_grid_model/component/branch.hpp`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     using OutputType = BranchOutput<sym>;
     using ShortCircuitOutputType = BranchShortCircuitOutput;
     static constexpr char const* name = "branch";
     ComponentType math_model_type() const final {
         return ComponentType::branch;
     }
 
-    Branch(BranchInput const& branch_input)
+    explicit Branch(BranchInput const& branch_input)
         : Base{branch_input},
           from_node_{branch_input.from_node},
           to_node_{branch_input.to_node},
           from_status_{static_cast<bool>(branch_input.from_status)},
           to_status_{static_cast<bool>(branch_input.to_status)} {
         if (from_node_ == to_node_) {
             throw InvalidBranch{id(), from_node_};
```

### Comparing `power-grid-model-1.5.0rc9192016554667/power_grid_model_c/power_grid_model/include/power_grid_model/component/branch3.hpp` & `power-grid-model-1.5.0rc9193215149708/power_grid_model_c/power_grid_model/include/power_grid_model/component/branch3.hpp`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     using OutputType = Branch3Output<sym>;
     using ShortCircuitOutputType = Branch3ShortCircuitOutput;
     static constexpr char const* name = "branch3";
     ComponentType math_model_type() const final {
         return ComponentType::branch3;
     }
 
-    Branch3(Branch3Input const& branch3_input)
+    explicit Branch3(Branch3Input const& branch3_input)
         : Base{branch3_input},
           node_1_{branch3_input.node_1},
           node_2_{branch3_input.node_2},
           node_3_{branch3_input.node_3},
           status_1_{static_cast<bool>(branch3_input.status_1)},
           status_2_{static_cast<bool>(branch3_input.status_2)},
           status_3_{static_cast<bool>(branch3_input.status_3)} {
```

### Comparing `power-grid-model-1.5.0rc9192016554667/power_grid_model_c/power_grid_model/include/power_grid_model/component/fault.hpp` & `power-grid-model-1.5.0rc9193215149708/power_grid_model_c/power_grid_model/include/power_grid_model/component/fault.hpp`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     using OutputType = FaultOutput;
     using ShortCircuitOutputType = FaultShortCircuitOutput;
     static constexpr char const* name = "fault";
     ComponentType math_model_type() const final {
         return ComponentType::fault;
     }
 
-    Fault(FaultInput const& fault_input)
+    explicit Fault(FaultInput const& fault_input)
         : Base{fault_input},
           status_{static_cast<bool>(fault_input.status)},
           fault_type_{fault_input.fault_type},
           fault_phase_{fault_input.fault_phase},
           fault_object_{fault_input.fault_object},
           r_f_{is_nan(fault_input.r_f) ? double{} : fault_input.r_f},
           x_f_{is_nan(fault_input.x_f) ? double{} : fault_input.x_f} {
```

### Comparing `power-grid-model-1.5.0rc9192016554667/power_grid_model_c/power_grid_model/include/power_grid_model/component/line.hpp` & `power-grid-model-1.5.0rc9193215149708/power_grid_model_c/power_grid_model/include/power_grid_model/component/line.hpp`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 class Line final : public Branch {
    public:
     using InputType = LineInput;
     using UpdateType = BranchUpdate;
     static constexpr char const* name = "line";
 
-    Line(LineInput const& line_input, double system_frequency, double u1, double u2)
+    explicit Line(LineInput const& line_input, double system_frequency, double u1, double u2)
         : Branch{line_input}, i_n_{line_input.i_n}, base_i_{base_power_3p / u1 / sqrt3} {
         if (cabs(u1 - u2) > numerical_tolerance) {
             throw ConflictVoltage{id(), from_node(), to_node(), u1, u2};
         }
         double const base_y = base_i_ / (u1 / sqrt3);
         y1_series_ = 1.0 / (line_input.r1 + 1.0i * line_input.x1) / base_y;
         y1_shunt_ = 2.0 * pi * system_frequency * line_input.c1 / base_y * (line_input.tan1 + 1.0i);
```

### Comparing `power-grid-model-1.5.0rc9192016554667/power_grid_model_c/power_grid_model/include/power_grid_model/component/link.hpp` & `power-grid-model-1.5.0rc9193215149708/power_grid_model_c/power_grid_model/include/power_grid_model/component/link.hpp`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 class Link final : public Branch {
    public:
     using InputType = LinkInput;
     using UpdateType = BranchUpdate;
     static constexpr char const* name = "link";
 
-    Link(LinkInput const& link_input, double u1, double u2)
+    explicit Link(LinkInput const& link_input, double u1, double u2)
         : Branch{link_input}, base_i_from_{base_power_3p / u1 / sqrt3}, base_i_to_{base_power_3p / u2 / sqrt3} {
     }
 
     // override getter
     double base_i_from() const final {
         return base_i_from_;
     }
```

### Comparing `power-grid-model-1.5.0rc9192016554667/power_grid_model_c/power_grid_model/include/power_grid_model/component/load_gen.hpp` & `power-grid-model-1.5.0rc9193215149708/power_grid_model_c/power_grid_model/include/power_grid_model/component/load_gen.hpp`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
    public:
     using InputType = GenericLoadGenInput;
     static constexpr char const* name = "generic_load_gen";
     ComponentType math_model_type() const final {
         return ComponentType::generic_load_gen;
     }
 
-    GenericLoadGen(GenericLoadGenInput const& generic_load_gen_input, double u)
+    explicit GenericLoadGen(GenericLoadGenInput const& generic_load_gen_input, double u)
         : Appliance{generic_load_gen_input, u}, type_{generic_load_gen_input.type} {
     }
 
     // getter for load type
     LoadGenType type() const {
         return type_;
     }
```

### Comparing `power-grid-model-1.5.0rc9192016554667/power_grid_model_c/power_grid_model/include/power_grid_model/component/node.hpp` & `power-grid-model-1.5.0rc9193215149708/power_grid_model_c/power_grid_model/include/power_grid_model/component/node.hpp`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     using OutputType = NodeOutput<sym>;
     using ShortCircuitOutputType = NodeShortCircuitOutput;
     static constexpr char const* name = "node";
     ComponentType math_model_type() const final {
         return ComponentType::node;
     }
 
-    Node(NodeInput const& node_input) : Base{node_input}, u_rated_{node_input.u_rated} {
+    explicit Node(NodeInput const& node_input) : Base{node_input}, u_rated_{node_input.u_rated} {
     }
 
     // update node, nothing happens here
     UpdateChange update(BaseUpdate const&) {
         return {false, false};
     }
```

### Comparing `power-grid-model-1.5.0rc9192016554667/power_grid_model_c/power_grid_model/include/power_grid_model/component/power_sensor.hpp` & `power-grid-model-1.5.0rc9193215149708/power_grid_model_c/power_grid_model/include/power_grid_model/component/power_sensor.hpp`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 namespace power_grid_model {
 
 class GenericPowerSensor : public Sensor {
    public:
     static constexpr char const* name = "generic_power_sensor";
 
-    GenericPowerSensor(GenericPowerSensorInput const& generic_power_sensor_input)
+    explicit GenericPowerSensor(GenericPowerSensorInput const& generic_power_sensor_input)
         : Sensor{generic_power_sensor_input}, terminal_type_{generic_power_sensor_input.measured_terminal_type} {
     }
 
     MeasuredTerminalType get_terminal_type() const {
         return terminal_type_;
     }
 
@@ -64,15 +64,15 @@
    public:
     static constexpr char const* name = sym ? "sym_power_sensor" : "asym_power_sensor";
     using InputType = PowerSensorInput<sym>;
     using UpdateType = PowerSensorUpdate<sym>;
     template <bool sym_calc>
     using OutputType = PowerSensorOutput<sym_calc>;
 
-    PowerSensor(PowerSensorInput<sym> const& power_sensor_input)
+    explicit PowerSensor(PowerSensorInput<sym> const& power_sensor_input)
         : GenericPowerSensor{power_sensor_input}, power_sigma_{power_sensor_input.power_sigma / base_power<sym>} {
         set_power(power_sensor_input.p_measured, power_sensor_input.q_measured);
     };
 
     UpdateChange update(PowerSensorUpdate<sym> const& power_sensor_update) {
         set_power(power_sensor_update.p_measured, power_sensor_update.q_measured);
```

### Comparing `power-grid-model-1.5.0rc9192016554667/power_grid_model_c/power_grid_model/include/power_grid_model/component/sensor.hpp` & `power-grid-model-1.5.0rc9193215149708/power_grid_model_c/power_grid_model/include/power_grid_model/component/sensor.hpp`

 * *Files 6% similar despite different names*

```diff
@@ -19,15 +19,16 @@
 class Sensor : public Base {
    public:
     static constexpr char const* name = "sensor";
     using InputType = SensorInput;
     using ShortCircuitOutputType = SensorShortCircuitOutput;
 
     // constructor
-    Sensor(SensorInput const& sensor_input) : Base{sensor_input}, measured_object_{sensor_input.measured_object} {
+    explicit Sensor(SensorInput const& sensor_input)
+        : Base{sensor_input}, measured_object_{sensor_input.measured_object} {
     }
 
     ID measured_object() const {
         return measured_object_;
     };
 
     // sensor always energized
```

### Comparing `power-grid-model-1.5.0rc9192016554667/power_grid_model_c/power_grid_model/include/power_grid_model/component/shunt.hpp` & `power-grid-model-1.5.0rc9193215149708/power_grid_model_c/power_grid_model/include/power_grid_model/component/shunt.hpp`

 * *Files 4% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     using InputType = ShuntInput;
     using UpdateType = ApplianceUpdate;
     static constexpr char const* name = "shunt";
     ComponentType math_model_type() const final {
         return ComponentType::shunt;
     }
 
-    Shunt(ShuntInput const& shunt_input, double u) : Appliance{shunt_input, u} {
+    explicit Shunt(ShuntInput const& shunt_input, double u) : Appliance{shunt_input, u} {
         double const base_y = base_i() / (u / sqrt3);
         y1_ = (shunt_input.g1 + 1.0i * shunt_input.b1) / base_y;
         y0_ = (shunt_input.g0 + 1.0i * shunt_input.b0) / base_y;
     }
 
     // getter for calculation param, shunt y
     template <bool sym>
```

### Comparing `power-grid-model-1.5.0rc9192016554667/power_grid_model_c/power_grid_model/include/power_grid_model/component/source.hpp` & `power-grid-model-1.5.0rc9193215149708/power_grid_model_c/power_grid_model/include/power_grid_model/component/source.hpp`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     using InputType = SourceInput;
     using UpdateType = SourceUpdate;
     static constexpr char const* name = "source";
     ComponentType math_model_type() const final {
         return ComponentType::source;
     }
 
-    Source(SourceInput const& source_input, double u)
+    explicit Source(SourceInput const& source_input, double u)
         : Appliance{source_input, u}, u_ref_{source_input.u_ref}, u_ref_angle_{}, y1_ref_{}, y0_ref_{} {
         u_ref_angle_ = is_nan(source_input.u_ref_angle) ? 0.0 : source_input.u_ref_angle;
         double const sk{is_nan(source_input.sk) ? default_source_sk : source_input.sk};
         double const rx_ratio{is_nan(source_input.rx_ratio) ? default_source_rx_ratio : source_input.rx_ratio};
         double const z01_ratio{is_nan(source_input.z01_ratio) ? default_source_z01_ratio : source_input.z01_ratio};
         calculate_y_ref(sk, rx_ratio, z01_ratio);
     }
```

### Comparing `power-grid-model-1.5.0rc9192016554667/power_grid_model_c/power_grid_model/include/power_grid_model/component/three_winding_transformer.hpp` & `power-grid-model-1.5.0rc9193215149708/power_grid_model_c/power_grid_model/include/power_grid_model/component/three_winding_transformer.hpp`

 * *Files 0% similar despite different names*

```diff
@@ -14,16 +14,16 @@
 
 class ThreeWindingTransformer : public Branch3 {
    public:
     using InputType = ThreeWindingTransformerInput;
     using UpdateType = ThreeWindingTransformerUpdate;
     static constexpr char const* name = "three_winding_transformer";
 
-    ThreeWindingTransformer(ThreeWindingTransformerInput const& three_winding_transformer_input, double u1_rated,
-                            double u2_rated, double u3_rated)
+    explicit ThreeWindingTransformer(ThreeWindingTransformerInput const& three_winding_transformer_input,
+                                     double u1_rated, double u2_rated, double u3_rated)
         : Branch3{three_winding_transformer_input},
           u1_{three_winding_transformer_input.u1},
           u2_{three_winding_transformer_input.u2},
           u3_{three_winding_transformer_input.u3},
           u1_rated_{u1_rated},
           u2_rated_{u2_rated},
           u3_rated_{u3_rated},
```

### Comparing `power-grid-model-1.5.0rc9192016554667/power_grid_model_c/power_grid_model/include/power_grid_model/component/transformer.hpp` & `power-grid-model-1.5.0rc9193215149708/power_grid_model_c/power_grid_model/include/power_grid_model/component/transformer.hpp`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 class Transformer : public Branch {
    public:
     using InputType = TransformerInput;
     using UpdateType = TransformerUpdate;
     static constexpr char const* name = "transformer";
 
-    Transformer(TransformerInput const& transformer_input, double u1_rated, double u2_rated)
+    explicit Transformer(TransformerInput const& transformer_input, double u1_rated, double u2_rated)
         : Branch{transformer_input},
           u1_{transformer_input.u1},
           u2_{transformer_input.u2},
           sn_{transformer_input.sn},
           tap_size_{transformer_input.tap_size},
           uk_{transformer_input.uk},
           pk_{transformer_input.pk},
```

### Comparing `power-grid-model-1.5.0rc9192016554667/power_grid_model_c/power_grid_model/include/power_grid_model/component/transformer_utils.hpp` & `power-grid-model-1.5.0rc9193215149708/power_grid_model_c/power_grid_model/include/power_grid_model/component/transformer_utils.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9192016554667/power_grid_model_c/power_grid_model/include/power_grid_model/component/voltage_sensor.hpp` & `power-grid-model-1.5.0rc9193215149708/power_grid_model_c/power_grid_model/include/power_grid_model/component/voltage_sensor.hpp`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 namespace power_grid_model {
 
 class GenericVoltageSensor : public Sensor {
    public:
     static constexpr char const* name = "generic_voltage_sensor";
 
-    GenericVoltageSensor(GenericVoltageSensorInput const& generic_voltage_sensor_input)
+    explicit GenericVoltageSensor(GenericVoltageSensorInput const& generic_voltage_sensor_input)
         : Sensor{generic_voltage_sensor_input} {};
 
     template <bool sym>
     VoltageSensorOutput<sym> get_output(ComplexValue<sym> const& u) const {
         if constexpr (sym) {
             assert(u != 0.0 + 0.0i);
             return get_sym_output(u);
@@ -58,15 +58,15 @@
    public:
     static constexpr char const* name = sym ? "sym_voltage_sensor" : "asym_voltage_sensor";
     using InputType = VoltageSensorInput<sym>;
     using UpdateType = VoltageSensorUpdate<sym>;
     template <bool sym_calc>
     using OutputType = VoltageSensorOutput<sym_calc>;
 
-    VoltageSensor(VoltageSensorInput<sym> const& voltage_sensor_input, double u_rated)
+    explicit VoltageSensor(VoltageSensorInput<sym> const& voltage_sensor_input, double u_rated)
         : GenericVoltageSensor{voltage_sensor_input},
           u_rated_{u_rated},
           u_sigma_{voltage_sensor_input.u_sigma / (u_rated_ * u_scale<sym>)},
           u_measured_{voltage_sensor_input.u_measured / (u_rated_ * u_scale<sym>)},
           u_angle_measured_{voltage_sensor_input.u_angle_measured} {};
 
     UpdateChange update(VoltageSensorUpdate<sym> const& voltage_sensor_update) {
```

### Comparing `power-grid-model-1.5.0rc9192016554667/power_grid_model_c/power_grid_model/include/power_grid_model/container.hpp` & `power-grid-model-1.5.0rc9193215149708/power_grid_model_c/power_grid_model/include/power_grid_model/container.hpp`

 * *Files 0% similar despite different names*

```diff
@@ -345,15 +345,15 @@
     class Proxy {
        private:
         static constexpr bool is_const = std::is_const_v<Gettable>;
         using base_type = std::remove_cv_t<Gettable>;
         using container_type = std::conditional_t<is_const, Container const, Container>;
 
        public:
-        Proxy(container_type& container)
+        explicit Proxy(container_type& container)
             : begin_{&container, 0}, end_{&container, container.template size<base_type>()} {
         }
         Iterator<Gettable> begin() {
             return begin_;
         }
         Iterator<Gettable> end() {
             return end_;
```

### Comparing `power-grid-model-1.5.0rc9192016554667/power_grid_model_c/power_grid_model/include/power_grid_model/enum.hpp` & `power-grid-model-1.5.0rc9193215149708/power_grid_model_c/power_grid_model/include/power_grid_model/enum.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9192016554667/power_grid_model_c/power_grid_model/include/power_grid_model/exception.hpp` & `power-grid-model-1.5.0rc9193215149708/power_grid_model_c/power_grid_model/include/power_grid_model/exception.hpp`

 * *Files 3% similar despite different names*

```diff
@@ -90,43 +90,43 @@
         append_msg("Iteration failed to converge after " + std::to_string(num_iter) + " iterations! Max deviation: " +
                    std::to_string(max_dev) + ", error tolerance: " + std::to_string(err_tol) + ".\n");
     }
 };
 
 class ConflictID : public PowerGridError {
    public:
-    ConflictID(ID id) {
+    explicit ConflictID(ID id) {
         append_msg("Conflicting id detected: " + std::to_string(id) + '\n');
     }
 };
 
 class IDNotFound : public PowerGridError {
    public:
-    IDNotFound(ID id) {
+    explicit IDNotFound(ID id) {
         append_msg("The id cannot be found: " + std::to_string(id) + '\n');
     }
 };
 
 class InvalidMeasuredObject : public PowerGridError {
    public:
     InvalidMeasuredObject(const std::string &object, const std::string &sensor) {
         append_msg(sensor + " is not supported for " + object);
     }
 };
 
 class IDWrongType : public PowerGridError {
    public:
-    IDWrongType(ID id) {
+    explicit IDWrongType(ID id) {
         append_msg("Wrong type for object with id " + std::to_string(id) + '\n');
     }
 };
 
 class CalculationError : public PowerGridError {
    public:
-    CalculationError(std::string const &msg) {
+    explicit CalculationError(std::string const &msg) {
         append_msg(msg);
     }
 };
 
 class BatchCalculationError : public CalculationError {
    public:
     BatchCalculationError(std::string const &msg, IdxVector const &failed_scenarios,
@@ -151,15 +151,15 @@
    public:
     InvalidCalculationMethod() : CalculationError("The calculation method is invalid for this calculation!") {
     }
 };
 
 class UnknownAttributeName : public PowerGridError {
    public:
-    UnknownAttributeName(std::string const &attr_name) {
+    explicit UnknownAttributeName(std::string const &attr_name) {
         append_msg("Unknown attribute name!" + attr_name + "\n");
     }
 };
 
 }  // namespace power_grid_model
 
 #endif
```

### Comparing `power-grid-model-1.5.0rc9192016554667/power_grid_model_c/power_grid_model/include/power_grid_model/main_model.hpp` & `power-grid-model-1.5.0rc9193215149708/power_grid_model_c/power_grid_model/include/power_grid_model/main_model.hpp`

 * *Files 0% similar despite different names*

```diff
@@ -1089,15 +1089,15 @@
      * model and all of them are filled within the same function call (i.e. Notice that calc_input is a vector).
      *
      *  1. For each component, check if it should be included.
      *     By default, all component are included, except for some cases, like power sensors. For power sensors, the
      *     list of component contains all power sensors, but the preparation should only be done for one type of power
      *     sensors at a time. Therefore, `included` will be a lambda function, such as:
      *
-     *       [&](Idx i) { return comp_topo_->power_sensor_terminal_type[i] == MeasuredTerminalType::source; }
+     *       [this](Idx i) { return comp_topo_->power_sensor_terminal_type[i] == MeasuredTerminalType::source; }
      *
      *  2. Find the original component in the topology and retrieve its calculation parameters.
      *
      *  3. Fill the calculation parameters of the right math model.
      *
      *
      *  @tparam sym
@@ -1206,45 +1206,45 @@
         prepare_input_status<sym, &StateEstimationInput<sym>::source_status, Source>(comp_coup_->source, se_input);
 
         prepare_input<sym, StateEstimationInput<sym>, SensorCalcParam<sym>,
                       &StateEstimationInput<sym>::measured_voltage, GenericVoltageSensor>(comp_coup_->voltage_sensor,
                                                                                           se_input);
         prepare_input<sym, StateEstimationInput<sym>, SensorCalcParam<sym>,
                       &StateEstimationInput<sym>::measured_source_power, GenericPowerSensor>(
-            comp_coup_->power_sensor, se_input, [&](Idx i) {
+            comp_coup_->power_sensor, se_input, [this](Idx i) {
                 return comp_topo_->power_sensor_terminal_type[i] == MeasuredTerminalType::source;
             });
         prepare_input<sym, StateEstimationInput<sym>, SensorCalcParam<sym>,
                       &StateEstimationInput<sym>::measured_load_gen_power, GenericPowerSensor>(
-            comp_coup_->power_sensor, se_input, [&](Idx i) {
+            comp_coup_->power_sensor, se_input, [this](Idx i) {
                 return comp_topo_->power_sensor_terminal_type[i] == MeasuredTerminalType::load ||
                        comp_topo_->power_sensor_terminal_type[i] == MeasuredTerminalType::generator;
             });
         prepare_input<sym, StateEstimationInput<sym>, SensorCalcParam<sym>,
                       &StateEstimationInput<sym>::measured_shunt_power, GenericPowerSensor>(
-            comp_coup_->power_sensor, se_input, [&](Idx i) {
+            comp_coup_->power_sensor, se_input, [this](Idx i) {
                 return comp_topo_->power_sensor_terminal_type[i] == MeasuredTerminalType::shunt;
             });
         prepare_input<sym, StateEstimationInput<sym>, SensorCalcParam<sym>,
                       &StateEstimationInput<sym>::measured_branch_from_power, GenericPowerSensor>(
-            comp_coup_->power_sensor, se_input, [&](Idx i) {
+            comp_coup_->power_sensor, se_input, [this](Idx i) {
                 return comp_topo_->power_sensor_terminal_type[i] == MeasuredTerminalType::branch_from ||
                        // all branch3 sensors are at from side in the mathematical model
                        comp_topo_->power_sensor_terminal_type[i] == MeasuredTerminalType::branch3_1 ||
                        comp_topo_->power_sensor_terminal_type[i] == MeasuredTerminalType::branch3_2 ||
                        comp_topo_->power_sensor_terminal_type[i] == MeasuredTerminalType::branch3_3;
             });
         prepare_input<sym, StateEstimationInput<sym>, SensorCalcParam<sym>,
                       &StateEstimationInput<sym>::measured_branch_to_power, GenericPowerSensor>(
-            comp_coup_->power_sensor, se_input, [&](Idx i) {
+            comp_coup_->power_sensor, se_input, [this](Idx i) {
                 return comp_topo_->power_sensor_terminal_type[i] == MeasuredTerminalType::branch_to;
             });
         prepare_input<sym, StateEstimationInput<sym>, SensorCalcParam<sym>,
                       &StateEstimationInput<sym>::measured_bus_injection, GenericPowerSensor>(
-            comp_coup_->power_sensor, se_input, [&](Idx i) {
+            comp_coup_->power_sensor, se_input, [this](Idx i) {
                 return comp_topo_->power_sensor_terminal_type[i] == MeasuredTerminalType::node;
             });
 
         return se_input;
     }
 
     template <bool sym>
```

### Comparing `power-grid-model-1.5.0rc9192016554667/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/block_matrix.hpp` & `power-grid-model-1.5.0rc9193215149708/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/block_matrix.hpp`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     using ArrayType = typename block_trait<T, sym, is_tensor, n_sub_block>::ArrayType;
     using ArrayType::operator();
 
     // default zero
     Block() : ArrayType{ArrayType::Zero()} {};
     // eigen expression
     template <typename OtherDerived>
-    Block(Eigen::ArrayBase<OtherDerived> const& other) : ArrayType{other} {
+    explicit Block(Eigen::ArrayBase<OtherDerived> const& other) : ArrayType{other} {
     }
     template <typename OtherDerived>
     Block& operator=(Eigen::ArrayBase<OtherDerived> const& other) {
         this->ArrayType::operator=(other);
         return *this;
     }
```

### Comparing `power-grid-model-1.5.0rc9192016554667/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/iterative_current_pf_solver.hpp` & `power-grid-model-1.5.0rc9193215149708/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/iterative_current_pf_solver.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9192016554667/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/iterative_linear_se_solver.hpp` & `power-grid-model-1.5.0rc9193215149708/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/iterative_linear_se_solver.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9192016554667/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/iterative_pf_solver.hpp` & `power-grid-model-1.5.0rc9193215149708/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/iterative_pf_solver.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9192016554667/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/linear_pf_solver.hpp` & `power-grid-model-1.5.0rc9193215149708/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/linear_pf_solver.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9192016554667/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/math_solver.hpp` & `power-grid-model-1.5.0rc9193215149708/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/math_solver.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9192016554667/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/newton_raphson_pf_solver.hpp` & `power-grid-model-1.5.0rc9193215149708/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/newton_raphson_pf_solver.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9192016554667/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/sparse_lu_solver.hpp` & `power-grid-model-1.5.0rc9193215149708/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/sparse_lu_solver.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9192016554667/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/y_bus.hpp` & `power-grid-model-1.5.0rc9193215149708/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/y_bus.hpp`

 * *Files 0% similar despite different names*

```diff
@@ -91,15 +91,15 @@
     // transpose entry of the sparse matrix
     // length of nnz_lu Idx array.
     // for lu_transpose_entry[i] indicates the position i-th element in transposed lu matrix in CSR form
     // for entry in the diagonal lu_transpose_entry[i] = i
     IdxVector lu_transpose_entry;
 
     // construct ybus structure
-    YBusStructure(MathModelTopology const& topo) {
+    explicit YBusStructure(MathModelTopology const& topo) {
         Idx const n_bus = topo.n_bus();
         Idx const n_branch = topo.n_branch();
         Idx const n_fill_in = (Idx)topo.fill_in.size();
         // allocate element vector
         std::vector<YBusElementMap> vec_map_element;
         Idx const total_number_entries = 4 * n_branch + n_bus + 2 * n_fill_in;
         vec_map_element.reserve(total_number_entries);
```

### Comparing `power-grid-model-1.5.0rc9192016554667/power_grid_model_c/power_grid_model/include/power_grid_model/power_grid_model.hpp` & `power-grid-model-1.5.0rc9193215149708/power_grid_model_c/power_grid_model/include/power_grid_model/power_grid_model.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9192016554667/power_grid_model_c/power_grid_model/include/power_grid_model/sparse_mapping.hpp` & `power-grid-model-1.5.0rc9193215149708/power_grid_model_c/power_grid_model/include/power_grid_model/sparse_mapping.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9192016554667/power_grid_model_c/power_grid_model/include/power_grid_model/three_phase_tensor.hpp` & `power-grid-model-1.5.0rc9193215149708/power_grid_model_c/power_grid_model/include/power_grid_model/three_phase_tensor.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9192016554667/power_grid_model_c/power_grid_model/include/power_grid_model/timer.hpp` & `power-grid-model-1.5.0rc9193215149708/power_grid_model_c/power_grid_model/include/power_grid_model/timer.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9192016554667/power_grid_model_c/power_grid_model/include/power_grid_model/topology.hpp` & `power-grid-model-1.5.0rc9193215149708/power_grid_model_c/power_grid_model/include/power_grid_model/topology.hpp`

 * *Files 0% similar despite different names*

```diff
@@ -603,46 +603,46 @@
                 continue;
             }
             math_topology_[idx_math.group].load_gen_type[idx_math.pos] = comp_topo_.load_gen_type[k];
         }
 
         // source
         couple_object_components<&MathModelTopology::source_bus_indptr, &MathModelTopology::n_bus>(
-            {comp_topo_.source_node_idx, comp_coup_.node}, comp_coup_.source, [&](Idx i) {
+            {comp_topo_.source_node_idx, comp_coup_.node}, comp_coup_.source, [this](Idx i) {
                 return comp_conn_.source_connected[i];
             });
     }
 
     void couple_sensors() {
         // voltage sensors
         couple_object_components<&MathModelTopology::voltage_sensor_indptr, &MathModelTopology::n_bus>(
             {comp_topo_.voltage_sensor_node_idx, comp_coup_.node}, comp_coup_.voltage_sensor);
 
         // source power sensors
         couple_object_components<&MathModelTopology::source_power_sensor_indptr, &MathModelTopology::n_source>(
-            {comp_topo_.power_sensor_object_idx, comp_coup_.source}, comp_coup_.power_sensor, [&](Idx i) {
+            {comp_topo_.power_sensor_object_idx, comp_coup_.source}, comp_coup_.power_sensor, [this](Idx i) {
                 return comp_topo_.power_sensor_terminal_type[i] == MeasuredTerminalType::source;
             });
 
         // shunt power sensors
         couple_object_components<&MathModelTopology::shunt_power_sensor_indptr, &MathModelTopology::n_shunt>(
-            {comp_topo_.power_sensor_object_idx, comp_coup_.shunt}, comp_coup_.power_sensor, [&](Idx i) {
+            {comp_topo_.power_sensor_object_idx, comp_coup_.shunt}, comp_coup_.power_sensor, [this](Idx i) {
                 return comp_topo_.power_sensor_terminal_type[i] == MeasuredTerminalType::shunt;
             });
 
         // load + generator power sensors
         couple_object_components<&MathModelTopology::load_gen_power_sensor_indptr, &MathModelTopology::n_load_gen>(
-            {comp_topo_.power_sensor_object_idx, comp_coup_.load_gen}, comp_coup_.power_sensor, [&](Idx i) {
+            {comp_topo_.power_sensor_object_idx, comp_coup_.load_gen}, comp_coup_.power_sensor, [this](Idx i) {
                 return comp_topo_.power_sensor_terminal_type[i] == MeasuredTerminalType::load ||
                        comp_topo_.power_sensor_terminal_type[i] == MeasuredTerminalType::generator;
             });
 
         // branch 'from' power sensors
         // include all branch3 sensors
-        auto const predicate_from_sensor = [&](Idx i) {
+        auto const predicate_from_sensor = [this](Idx i) {
             using enum MeasuredTerminalType;
 
             return comp_topo_.power_sensor_terminal_type[i] == branch_from ||
                    // all branch3 sensors are at from side in the mathemtical model
                    comp_topo_.power_sensor_terminal_type[i] == branch3_1 ||
                    comp_topo_.power_sensor_terminal_type[i] == branch3_2 ||
                    comp_topo_.power_sensor_terminal_type[i] == branch3_3;
@@ -651,21 +651,21 @@
                                                                  comp_topo_.power_sensor_terminal_type,
                                                                  comp_coup_.branch, comp_coup_.branch3};
         couple_object_components<&MathModelTopology::branch_from_power_sensor_indptr, &MathModelTopology::n_branch>(
             object_finder_from_sensor, comp_coup_.power_sensor, predicate_from_sensor);
 
         // branch 'to' power sensors
         couple_object_components<&MathModelTopology::branch_to_power_sensor_indptr, &MathModelTopology::n_branch>(
-            {comp_topo_.power_sensor_object_idx, comp_coup_.branch}, comp_coup_.power_sensor, [&](Idx i) {
+            {comp_topo_.power_sensor_object_idx, comp_coup_.branch}, comp_coup_.power_sensor, [this](Idx i) {
                 return comp_topo_.power_sensor_terminal_type[i] == MeasuredTerminalType::branch_to;
             });
 
         // node injection power sensors
         couple_object_components<&MathModelTopology::bus_power_sensor_indptr, &MathModelTopology::n_bus>(
-            {comp_topo_.power_sensor_object_idx, comp_coup_.node}, comp_coup_.power_sensor, [&](Idx i) {
+            {comp_topo_.power_sensor_object_idx, comp_coup_.node}, comp_coup_.power_sensor, [this](Idx i) {
                 return comp_topo_.power_sensor_terminal_type[i] == MeasuredTerminalType::node;
             });
     }
 };
 
 }  // namespace power_grid_model
```

### Comparing `power-grid-model-1.5.0rc9192016554667/power_grid_model_c/power_grid_model_c/CMakeLists.txt` & `power-grid-model-1.5.0rc9193215149708/power_grid_model_c/power_grid_model_c/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9192016554667/power_grid_model_c/power_grid_model_c/include/power_grid_model_c.h` & `power-grid-model-1.5.0rc9193215149708/power_grid_model_c/power_grid_model_c/include/power_grid_model_c.h`

 * *Files 1% similar despite different names*

```diff
@@ -35,16 +35,21 @@
 #else
 #define PGM_API PGM_HELPER_DLL_IMPORT
 #endif  // PGM_DLL_EXPORTS
 #define PGM_LOCAL PGM_HELPER_DLL_LOCAL
 // API_MACRO_BLOCK
 
 // integers
+#ifdef __cplusplus
+#include <cstddef>
+#include <cstdint>
+#else
 #include <stddef.h>
 #include <stdint.h>
+#endif
 
 // C linkage
 #ifdef __cplusplus
 extern "C" {
 #endif
 
 // index type
```

### Comparing `power-grid-model-1.5.0rc9192016554667/power_grid_model_c/power_grid_model_c/power_grid_model_c.cpp` & `power-grid-model-1.5.0rc9193215149708/power_grid_model_c/power_grid_model_c/power_grid_model_c.cpp`

 * *Files 4% similar despite different names*

```diff
@@ -12,14 +12,17 @@
 #include "power_grid_model/auxiliary/meta_data_gen.hpp"
 #include "power_grid_model/main_model.hpp"
 #include "power_grid_model/power_grid_model.hpp"
 
 using namespace power_grid_model;
 
 namespace {
+using meta_data::RawDataConstPtr;
+using meta_data::RawDataPtr;
+
 meta_data::AllPowerGridMetaData const& pgm_meta = meta_data::meta_data();
 }  // namespace
 
 // assert index type
 static_assert(std::is_same_v<PGM_Idx, Idx>);
 static_assert(std::is_same_v<PGM_ID, ID>);
 
@@ -97,15 +100,15 @@
 PGM_Idx PGM_error_code(PGM_Handle const* handle) {
     return handle->err_code;
 }
 char const* PGM_error_message(PGM_Handle const* handle) {
     return handle->err_msg.c_str();
 }
 PGM_Idx PGM_n_failed_scenarios(PGM_Handle const* handle) {
-    return (Idx)handle->failed_scenarios.size();
+    return static_cast<Idx>(handle->failed_scenarios.size());
 }
 PGM_Idx const* PGM_failed_scenarios(PGM_Handle const* handle) {
     return handle->failed_scenarios.data();
 }
 char const** PGM_batch_errors(PGM_Handle const* handle) {
     handle->batch_errs_c_str.clear();
     std::transform(handle->batch_errs.begin(), handle->batch_errs.end(), std::back_inserter(handle->batch_errs_c_str),
@@ -121,90 +124,90 @@
 // retrieve meta data
 // dataset
 PGM_Idx PGM_meta_n_datasets(PGM_Handle*) {
     return (Idx)pgm_meta.size();
 }
 char const* PGM_meta_dataset_name(PGM_Handle* handle, PGM_Idx idx) {
     static auto const dataset_list = list_of_datasets();
-    return call_with_bound(handle, [&]() -> decltype(auto) {
+    return call_with_bound(handle, [idx]() -> decltype(auto) {
         return dataset_list.at(idx).c_str();
     });
 }
 // class
 PGM_Idx PGM_meta_n_components(PGM_Handle* handle, char const* dataset) {
-    return call_with_bound(handle, [&]() -> decltype(auto) {
-        return (Idx)pgm_meta.at(dataset).size();
+    return call_with_bound(handle, [dataset]() -> decltype(auto) {
+        return static_cast<Idx>(pgm_meta.at(dataset).size());
     });
 }
 char const* PGM_meta_component_name(PGM_Handle* handle, char const* dataset, PGM_Idx idx) {
     static auto const class_list = list_of_classes();
-    return call_with_bound(handle, [&]() -> decltype(auto) {
+    return call_with_bound(handle, [dataset, idx]() -> decltype(auto) {
         return class_list.at(dataset).at(idx).c_str();
     });
 }
 size_t PGM_meta_component_size(PGM_Handle* handle, char const* dataset, char const* component) {
-    return call_with_bound(handle, [&]() -> decltype(auto) {
+    return call_with_bound(handle, [dataset, component]() -> decltype(auto) {
         return pgm_meta.at(dataset).at(component).size;
     });
 }
 size_t PGM_meta_component_alignment(PGM_Handle* handle, char const* dataset, char const* component) {
-    return call_with_bound(handle, [&]() -> decltype(auto) {
+    return call_with_bound(handle, [dataset, component]() -> decltype(auto) {
         return pgm_meta.at(dataset).at(component).alignment;
     });
 }
 // attributes
 PGM_Idx PGM_meta_n_attributes(PGM_Handle* handle, char const* dataset, char const* component) {
-    return call_with_bound(handle, [&]() -> decltype(auto) {
-        return (Idx)pgm_meta.at(dataset).at(component).attributes.size();
+    return call_with_bound(handle, [dataset, component]() -> decltype(auto) {
+        return static_cast<Idx>(pgm_meta.at(dataset).at(component).attributes.size());
     });
 }
 char const* PGM_meta_attribute_name(PGM_Handle* handle, char const* dataset, char const* component, PGM_Idx idx) {
-    return call_with_bound(handle, [&]() -> decltype(auto) {
+    return call_with_bound(handle, [dataset, component, idx]() -> decltype(auto) {
         return pgm_meta.at(dataset).at(component).attributes.at(idx).name.c_str();
     });
 }
 char const* PGM_meta_attribute_ctype(PGM_Handle* handle, char const* dataset, char const* component,
                                      char const* attribute) {
-    return call_with_bound(handle, [&]() -> decltype(auto) {
+    return call_with_bound(handle, [dataset, component, attribute]() -> decltype(auto) {
         return pgm_meta.at(dataset).at(component).get_attr(attribute).ctype.c_str();
     });
 }
 size_t PGM_meta_attribute_offset(PGM_Handle* handle, char const* dataset, char const* component,
                                  char const* attribute) {
-    return call_with_bound(handle, [&]() -> decltype(auto) {
+    return call_with_bound(handle, [dataset, component, attribute]() -> decltype(auto) {
         return pgm_meta.at(dataset).at(component).get_attr(attribute).offset;
     });
 }
 int PGM_is_little_endian(PGM_Handle*) {
     return meta_data::is_little_endian();
 }
 
 // buffer control
-void* PGM_create_buffer(PGM_Handle* handle, char const* dataset, char const* component, PGM_Idx size) {
-    auto const& data_class = call_with_bound(handle, [&]() -> decltype(auto) {
+RawDataPtr PGM_create_buffer(PGM_Handle* handle, char const* dataset, char const* component, PGM_Idx size) {
+    auto const& data_class = call_with_bound(handle, [dataset, component]() -> decltype(auto) {
         return pgm_meta.at(dataset).at(component);
     });
     if (data_class.name == "") {
         return nullptr;
     }
 #ifdef _WIN32
     return _aligned_malloc(data_class.size * size, data_class.alignment);
 #else
     return std::aligned_alloc(data_class.alignment, data_class.size * size);
 #endif
 }
-void PGM_destroy_buffer(void* ptr) {
+void PGM_destroy_buffer(RawDataPtr ptr) {
 #ifdef _WIN32
     _aligned_free(ptr);
 #else
     std::free(ptr);
 #endif
 }
-void PGM_buffer_set_nan(PGM_Handle* handle, char const* dataset, char const* component, void* ptr, PGM_Idx size) {
-    auto const& data_class = call_with_bound(handle, [&]() -> decltype(auto) {
+void PGM_buffer_set_nan(PGM_Handle* handle, char const* dataset, char const* component, RawDataPtr ptr, PGM_Idx size) {
+    auto const& data_class = call_with_bound(handle, [dataset, component]() -> decltype(auto) {
         return pgm_meta.at(dataset).at(component);
     });
     if (data_class.name == "") {
         return;
     }
     for (Idx i = 0; i != size; ++i) {
         data_class.set_nan(ptr, i);
@@ -212,18 +215,18 @@
 }
 
 namespace {
 // template for get and set attribute
 template <bool is_get, class BufferPtr, class ValuePtr>
 void buffer_get_set_value(PGM_Handle* handle, char const* dataset, char const* component, char const* attribute,
                           BufferPtr buffer_ptr, ValuePtr value_ptr, PGM_Idx size, PGM_Idx stride) {
-    auto const& data_class = call_with_bound(handle, [&]() -> decltype(auto) {
+    auto const& data_class = call_with_bound(handle, [dataset, component]() -> decltype(auto) {
         return pgm_meta.at(dataset).at(component);
     });
-    auto const& attr = call_with_bound(handle, [&]() -> decltype(auto) {
+    auto const& attr = call_with_bound(handle, [&data_class, attribute]() -> decltype(auto) {
         return data_class.get_attr(attribute);
     });
     if (attr.name == "") {
         return;
     }
     // if stride is negative, use the size of the attributes as stride
     if (stride < 0) {
@@ -238,19 +241,19 @@
         else {
             data_class.set_attr(buffer_ptr, shifted_value_ptr, attr, i);
         }
     }
 }
 }  // namespace
 void PGM_buffer_set_value(PGM_Handle* handle, char const* dataset, char const* component, char const* attribute,
-                          void* buffer_ptr, void const* src_ptr, PGM_Idx size, PGM_Idx src_stride) {
+                          RawDataPtr buffer_ptr, RawDataConstPtr src_ptr, PGM_Idx size, PGM_Idx src_stride) {
     buffer_get_set_value<false>(handle, dataset, component, attribute, buffer_ptr, src_ptr, size, src_stride);
 }
 void PGM_buffer_get_value(PGM_Handle* handle, char const* dataset, char const* component, char const* attribute,
-                          void const* buffer_ptr, void* dest_ptr, PGM_Idx size, PGM_Idx dest_stride) {
+                          RawDataConstPtr buffer_ptr, RawDataPtr dest_ptr, PGM_Idx size, PGM_Idx dest_stride) {
     buffer_get_set_value<true>(handle, dataset, component, attribute, buffer_ptr, dest_ptr, size, dest_stride);
 }
 
 // options
 PGM_Options* PGM_create_options(PGM_Handle*) {
     return new PGM_Options{};
 }
@@ -274,15 +277,16 @@
 }
 void PGM_set_threading(PGM_Handle*, PGM_Options* opt, PGM_Idx threading) {
     opt->threading = threading;
 }
 
 // create model
 PGM_PowerGridModel* PGM_create_model(PGM_Handle* handle, double system_frequency, PGM_Idx n_components,
-                                     char const** components, PGM_Idx const* component_sizes, void const** input_data) {
+                                     char const** components, PGM_Idx const* component_sizes,
+                                     RawDataConstPtr* input_data) {
     PGM_clear_error(handle);
     ConstDataset dataset{};
     for (Idx i = 0; i != n_components; ++i) {
         dataset[components[i]] = ConstDataPointer{input_data[i], component_sizes[i]};
     }
     try {
         return new PGM_PowerGridModel{system_frequency, dataset, 0};
@@ -292,15 +296,15 @@
         handle->err_msg = e.what();
         return nullptr;
     }
 }
 
 // update model
 void PGM_update_model(PGM_Handle* handle, PGM_PowerGridModel* model, PGM_Idx n_components, char const** components,
-                      PGM_Idx const* component_sizes, void const** update_data) {
+                      PGM_Idx const* component_sizes, RawDataConstPtr* update_data) {
     PGM_clear_error(handle);
     ConstDataset dataset{};
     for (Idx i = 0; i != n_components; ++i) {
         dataset[components[i]] = ConstDataPointer{update_data[i], component_sizes[i]};
     }
     try {
         model->update_component<MainModel::permanent_update_t>(dataset);
@@ -333,23 +337,24 @@
         handle->err_code = PGM_regular_error;
         handle->err_msg = e.what();
     }
 }
 
 // run calculation
 void PGM_calculate(PGM_Handle* handle, PGM_PowerGridModel* model, PGM_Options const* opt, PGM_Idx n_output_components,
-                   char const** output_components, void** output_data, PGM_Idx n_scenarios, PGM_Idx n_update_components,
-                   char const** update_components, PGM_Idx const* n_component_elements_per_scenario,
-                   PGM_Idx const** indptrs_per_component, void const** update_data) {
+                   char const** output_components, RawDataPtr* output_data, PGM_Idx n_scenarios,
+                   PGM_Idx n_update_components, char const** update_components,
+                   PGM_Idx const* n_component_elements_per_scenario, PGM_Idx const** indptrs_per_component,
+                   RawDataConstPtr* update_data) {
     PGM_clear_error(handle);
     std::map<std::string, Idx> const n_component = model->all_component_count();
     // prepare output dataset
     Dataset output_dataset{};
     // set n_output_batch to one for single calculation
-    Idx const n_output_scenarios = std::max((Idx)1, n_scenarios);
+    Idx const n_output_scenarios = std::max(Idx{1}, n_scenarios);
     for (Idx i = 0; i != n_output_components; ++i) {
         auto const found = n_component.find(output_components[i]);
         if (found != n_component.cend()) {
             output_dataset[output_components[i]] =
                 MutableDataPointer{output_data[i], n_output_scenarios, found->second};
         }
     }
```

### Comparing `power-grid-model-1.5.0rc9192016554667/pyproject.toml` & `power-grid-model-1.5.0rc9193215149708/pyproject.toml`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9192016554667/setup.py` & `power-grid-model-1.5.0rc9193215149708/setup.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9192016554667/src/power_grid_model/core/error_handling.py` & `power-grid-model-1.5.0rc9193215149708/src/power_grid_model/core/error_handling.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9192016554667/src/power_grid_model/core/options.py` & `power-grid-model-1.5.0rc9193215149708/src/power_grid_model/core/options.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9192016554667/src/power_grid_model/core/power_grid_core.py` & `power-grid-model-1.5.0rc9193215149708/src/power_grid_model/core/power_grid_core.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9192016554667/src/power_grid_model/core/power_grid_meta.py` & `power-grid-model-1.5.0rc9193215149708/src/power_grid_model/core/power_grid_meta.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9192016554667/src/power_grid_model/core/power_grid_model.py` & `power-grid-model-1.5.0rc9193215149708/src/power_grid_model/core/power_grid_model.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9192016554667/src/power_grid_model/data_types.py` & `power-grid-model-1.5.0rc9193215149708/src/power_grid_model/data_types.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9192016554667/src/power_grid_model/enum.py` & `power-grid-model-1.5.0rc9193215149708/src/power_grid_model/enum.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9192016554667/src/power_grid_model/utils.py` & `power-grid-model-1.5.0rc9193215149708/src/power_grid_model/utils.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9192016554667/src/power_grid_model/validation/__init__.py` & `power-grid-model-1.5.0rc9193215149708/src/power_grid_model/validation/__init__.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9192016554667/src/power_grid_model/validation/assertions.py` & `power-grid-model-1.5.0rc9193215149708/src/power_grid_model/validation/assertions.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9192016554667/src/power_grid_model/validation/errors.py` & `power-grid-model-1.5.0rc9193215149708/src/power_grid_model/validation/errors.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9192016554667/src/power_grid_model/validation/rules.py` & `power-grid-model-1.5.0rc9193215149708/src/power_grid_model/validation/rules.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9192016554667/src/power_grid_model/validation/utils.py` & `power-grid-model-1.5.0rc9193215149708/src/power_grid_model/validation/utils.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9192016554667/src/power_grid_model/validation/validation.py` & `power-grid-model-1.5.0rc9193215149708/src/power_grid_model/validation/validation.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9192016554667/src/power_grid_model.egg-info/PKG-INFO` & `power-grid-model-1.5.0rc9193215149708/src/power_grid_model.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: power-grid-model
-Version: 1.5.0rc9192016554667
+Version: 1.5.0rc9193215149708
 Summary: Python/C++ library for distribution power system analysis
 Author-email: Alliander Dynamic Grid Calculation <dynamic.grid.calculation@alliander.com>
 License: MPL-2.0
 Project-URL: Home-page, https://lfenergy.org/projects/power-grid-model/
 Project-URL: GitHub, https://github.com/PowerGridModel/power-grid-model
 Project-URL: Documentation, https://power-grid-model.readthedocs.io/en/stable/
 Project-URL: Mailing-list, https://lists.lfenergy.org/g/powergridmodel
```

### Comparing `power-grid-model-1.5.0rc9192016554667/src/power_grid_model.egg-info/SOURCES.txt` & `power-grid-model-1.5.0rc9193215149708/src/power_grid_model.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/1os2msr/input.json` & `power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/1os2msr/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/1os2msr/sym_output.json` & `power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/1os2msr/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/dummy-test/input.json` & `power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/dummy-test/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/dummy-test/sym_output.json` & `power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/dummy-test/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/dummy-test-batch/input.json` & `power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/dummy-test-batch/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/dummy-test-batch-dependent-cacheable/input.json` & `power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/dummy-test-batch-dependent-cacheable/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/input.json` & `power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/update_batch.json` & `power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/dummy-test-batch-incomplete-input/input.json` & `power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/dummy-test-batch-incomplete-input/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/dummy-test-batch-independent-cacheable/input.json` & `power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/dummy-test-batch-independent-cacheable/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/input.json` & `power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/update_batch.json` & `power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/dummy-test-batch-newton/input.json` & `power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/dummy-test-batch-newton/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/dummy-test-i-n-optional/input.json` & `power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/dummy-test-i-n-optional/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/dummy-test-i-n-optional/sym_output.json` & `power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/dummy-test-i-n-optional/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/gaia-example/asym_output.json` & `power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/gaia-example/asym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/gaia-example/gaia_grid.gnf` & `power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/gaia-example/gaia_grid.gnf`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/gaia-example/input.json` & `power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/gaia-example/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/multi-source-with-angle/input.json` & `power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/multi-source-with-angle/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/README.md` & `power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/asym_output.json` & `power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/asym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/input.json` & `power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/components/asymmetric/asym_load/README.md` & `power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/components/asymmetric/asym_load/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/components/asymmetric/asym_load/asym_output.json` & `power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/components/asymmetric/asym_load/asym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/components/asymmetric/asym_load/input.json` & `power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/components/asymmetric/asym_load/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/components/asymmetric/line/README.md` & `power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/components/asymmetric/line/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/components/asymmetric/line/asym_output.json` & `power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/components/asymmetric/line/asym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/components/asymmetric/line/input.json` & `power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/components/asymmetric/line/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/components/asymmetric/node/README.md` & `power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/components/asymmetric/node/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/components/asymmetric/node/asym_output.json` & `power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/components/asymmetric/node/asym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/components/asymmetric/node/input.json` & `power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/components/asymmetric/node/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/components/asymmetric/shunt/README.md` & `power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/components/asymmetric/shunt/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/components/asymmetric/shunt/asym_output.json` & `power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/components/asymmetric/shunt/asym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/components/asymmetric/shunt/input.json` & `power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/components/asymmetric/shunt/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/components/asymmetric/source/README.md` & `power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/components/asymmetric/source/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/components/asymmetric/source/asym_output.json` & `power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/components/asymmetric/source/asym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/components/asymmetric/source/input.json` & `power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/components/asymmetric/source/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/README.md` & `power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/asym_output.json` & `power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/asym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/input.json` & `power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/components/asymmetric/sym_load/README.md` & `power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/components/asymmetric/sym_load/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/components/asymmetric/sym_load/asym_output.json` & `power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/components/asymmetric/sym_load/asym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/components/asymmetric/sym_load/input.json` & `power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/components/asymmetric/sym_load/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/components/asymmetric/transformer/README.md` & `power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/components/asymmetric/transformer/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/components/asymmetric/transformer/asym_output_batch.json` & `power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/components/asymmetric/transformer/asym_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/components/asymmetric/transformer/input.json` & `power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/components/asymmetric/transformer/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/components/asymmetric/transformer/update_batch.json` & `power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/components/asymmetric/transformer/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/components/symmetric/line/README.md` & `power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/components/symmetric/line/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/components/symmetric/line/input.json` & `power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/components/symmetric/line/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/components/symmetric/line/sym_output.json` & `power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/components/symmetric/line/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/components/symmetric/node/input.json` & `power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/components/symmetric/node/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/components/symmetric/node/sym_output.json` & `power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/components/symmetric/node/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/components/symmetric/shunt/input.json` & `power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/components/symmetric/shunt/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/components/symmetric/shunt/sym_output.json` & `power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/components/symmetric/shunt/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/components/symmetric/source/input.json` & `power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/components/symmetric/source/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/components/symmetric/source/sym_output.json` & `power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/components/symmetric/source/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/components/symmetric/sym_gen/README.md` & `power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/components/symmetric/sym_gen/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/components/symmetric/sym_gen/input.json` & `power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/components/symmetric/sym_gen/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/components/symmetric/sym_gen/sym_output.json` & `power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/components/symmetric/sym_gen/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/components/symmetric/sym_load/README.md` & `power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/components/symmetric/sym_load/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/components/symmetric/sym_load/input.json` & `power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/components/symmetric/sym_load/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/components/symmetric/sym_load/sym_output.json` & `power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/components/symmetric/sym_load/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/README.md` & `power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/input.json` & `power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/sym_output_batch.json` & `power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/sym_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/update_batch.json` & `power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/components/symmetric/transformer/README.md` & `power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/components/symmetric/transformer/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/components/symmetric/transformer/input.json` & `power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/components/symmetric/transformer/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/components/symmetric/transformer/sym_output_batch.json` & `power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/components/symmetric/transformer/sym_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/components/symmetric/transformer/update_batch.json` & `power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/components/symmetric/transformer/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/README.md` & `power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/asym_output_batch.json` & `power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/asym_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/input.json` & `power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/update_batch.json` & `power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/README.md` & `power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/asym_output.json` & `power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/asym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/input.json` & `power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/README.md` & `power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/input.json` & `power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/sym_output_batch.json` & `power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/sym_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/update_batch.json` & `power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/README.md` & `power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/input.json` & `power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/sym_output.json` & `power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/r-state-estimation/input.json` & `power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/r-state-estimation/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/r-state-estimation/sym_output.json` & `power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/r-state-estimation/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/three-winding-transformer/asym_output_batch.json` & `power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/three-winding-transformer/asym_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/three-winding-transformer/input.json` & `power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/three-winding-transformer/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/three-winding-transformer/sym_output_batch.json` & `power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/three-winding-transformer/sym_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/three-winding-transformer/update_batch.json` & `power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/three-winding-transformer/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/vision-example/asym_output.json` & `power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/vision-example/asym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/vision-example/input.json` & `power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/vision-example/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/vision-example/vision_grid.vnf` & `power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/vision-example/vision_grid.vnf`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/vision-validation-network/asym_output.json` & `power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/vision-validation-network/asym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/vision-validation-network/input.json` & `power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/vision-validation-network/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/vision-validation-network/sym_output.json` & `power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/vision-validation-network/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9192016554667/tests/data/power_flow/vision-validation-network/vision_validation_network.vnf` & `power-grid-model-1.5.0rc9193215149708/tests/data/power_flow/vision-validation-network/vision_validation_network.vnf`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9192016554667/tests/data/short_circuit/single_phase_to_ground_a/input.json` & `power-grid-model-1.5.0rc9193215149708/tests/data/short_circuit/single_phase_to_ground_a/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9192016554667/tests/data/short_circuit/single_phase_to_ground_a/sc_output_batch.json` & `power-grid-model-1.5.0rc9193215149708/tests/data/short_circuit/single_phase_to_ground_a/sc_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9192016554667/tests/data/short_circuit/single_phase_to_ground_a/update_batch.json` & `power-grid-model-1.5.0rc9193215149708/tests/data/short_circuit/single_phase_to_ground_a/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9192016554667/tests/data/short_circuit/single_phase_to_ground_b/input.json` & `power-grid-model-1.5.0rc9193215149708/tests/data/short_circuit/single_phase_to_ground_b/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9192016554667/tests/data/short_circuit/single_phase_to_ground_b/sc_output_batch.json` & `power-grid-model-1.5.0rc9193215149708/tests/data/short_circuit/single_phase_to_ground_b/sc_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9192016554667/tests/data/short_circuit/single_phase_to_ground_b/update_batch.json` & `power-grid-model-1.5.0rc9193215149708/tests/data/short_circuit/single_phase_to_ground_b/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9192016554667/tests/data/short_circuit/single_phase_to_ground_c/input.json` & `power-grid-model-1.5.0rc9193215149708/tests/data/short_circuit/single_phase_to_ground_c/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9192016554667/tests/data/short_circuit/single_phase_to_ground_c/sc_output_batch.json` & `power-grid-model-1.5.0rc9193215149708/tests/data/short_circuit/single_phase_to_ground_c/sc_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9192016554667/tests/data/short_circuit/single_phase_to_ground_c/update_batch.json` & `power-grid-model-1.5.0rc9193215149708/tests/data/short_circuit/single_phase_to_ground_c/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9192016554667/tests/data/short_circuit/three_phase_abc/input.json` & `power-grid-model-1.5.0rc9193215149708/tests/data/short_circuit/three_phase_abc/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9192016554667/tests/data/short_circuit/three_phase_abc/sc_output_batch.json` & `power-grid-model-1.5.0rc9193215149708/tests/data/short_circuit/three_phase_abc/sc_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9192016554667/tests/data/short_circuit/three_phase_abc/update_batch.json` & `power-grid-model-1.5.0rc9193215149708/tests/data/short_circuit/three_phase_abc/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9192016554667/tests/data/short_circuit/two_phase_ab/input.json` & `power-grid-model-1.5.0rc9193215149708/tests/data/short_circuit/two_phase_ab/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9192016554667/tests/data/short_circuit/two_phase_ab/sc_output_batch.json` & `power-grid-model-1.5.0rc9193215149708/tests/data/short_circuit/two_phase_ab/sc_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9192016554667/tests/data/short_circuit/two_phase_ab/update_batch.json` & `power-grid-model-1.5.0rc9193215149708/tests/data/short_circuit/two_phase_ab/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9192016554667/tests/data/short_circuit/two_phase_ac/input.json` & `power-grid-model-1.5.0rc9193215149708/tests/data/short_circuit/two_phase_ac/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9192016554667/tests/data/short_circuit/two_phase_ac/sc_output_batch.json` & `power-grid-model-1.5.0rc9193215149708/tests/data/short_circuit/two_phase_ac/sc_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9192016554667/tests/data/short_circuit/two_phase_ac/update_batch.json` & `power-grid-model-1.5.0rc9193215149708/tests/data/short_circuit/two_phase_ac/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9192016554667/tests/data/short_circuit/two_phase_bc/input.json` & `power-grid-model-1.5.0rc9193215149708/tests/data/short_circuit/two_phase_bc/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9192016554667/tests/data/short_circuit/two_phase_bc/sc_output_batch.json` & `power-grid-model-1.5.0rc9193215149708/tests/data/short_circuit/two_phase_bc/sc_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9192016554667/tests/data/short_circuit/two_phase_bc/update_batch.json` & `power-grid-model-1.5.0rc9193215149708/tests/data/short_circuit/two_phase_bc/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9192016554667/tests/data/short_circuit/two_phase_to_ground_ab/input.json` & `power-grid-model-1.5.0rc9193215149708/tests/data/short_circuit/two_phase_to_ground_ab/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9192016554667/tests/data/short_circuit/two_phase_to_ground_ab/sc_output_batch.json` & `power-grid-model-1.5.0rc9193215149708/tests/data/short_circuit/two_phase_to_ground_ab/sc_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9192016554667/tests/data/short_circuit/two_phase_to_ground_ab/update_batch.json` & `power-grid-model-1.5.0rc9193215149708/tests/data/short_circuit/two_phase_to_ground_ab/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9192016554667/tests/data/short_circuit/two_phase_to_ground_ac/input.json` & `power-grid-model-1.5.0rc9193215149708/tests/data/short_circuit/two_phase_to_ground_ac/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9192016554667/tests/data/short_circuit/two_phase_to_ground_ac/sc_output_batch.json` & `power-grid-model-1.5.0rc9193215149708/tests/data/short_circuit/two_phase_to_ground_ac/sc_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9192016554667/tests/data/short_circuit/two_phase_to_ground_ac/update_batch.json` & `power-grid-model-1.5.0rc9193215149708/tests/data/short_circuit/two_phase_to_ground_ac/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9192016554667/tests/data/short_circuit/two_phase_to_ground_bc/input.json` & `power-grid-model-1.5.0rc9193215149708/tests/data/short_circuit/two_phase_to_ground_bc/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9192016554667/tests/data/short_circuit/two_phase_to_ground_bc/sc_output_batch.json` & `power-grid-model-1.5.0rc9193215149708/tests/data/short_circuit/two_phase_to_ground_bc/sc_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9192016554667/tests/data/short_circuit/two_phase_to_ground_bc/update_batch.json` & `power-grid-model-1.5.0rc9193215149708/tests/data/short_circuit/two_phase_to_ground_bc/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9192016554667/tests/data/state_estimation/1os2msr/input.json` & `power-grid-model-1.5.0rc9193215149708/tests/data/state_estimation/1os2msr/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9192016554667/tests/data/state_estimation/1os2msr/sym_output.json` & `power-grid-model-1.5.0rc9193215149708/tests/data/state_estimation/1os2msr/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9192016554667/tests/data/state_estimation/1os2msr-no-angle/input.json` & `power-grid-model-1.5.0rc9193215149708/tests/data/state_estimation/1os2msr-no-angle/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9192016554667/tests/data/state_estimation/1os2msr-no-angle/sym_output.json` & `power-grid-model-1.5.0rc9193215149708/tests/data/state_estimation/1os2msr-no-angle/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9192016554667/tests/data/state_estimation/distribution-case/README.md` & `power-grid-model-1.5.0rc9193215149708/tests/data/state_estimation/distribution-case/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9192016554667/tests/data/state_estimation/distribution-case/input.json` & `power-grid-model-1.5.0rc9193215149708/tests/data/state_estimation/distribution-case/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9192016554667/tests/data/state_estimation/distribution-case/sym_output_batch.json` & `power-grid-model-1.5.0rc9193215149708/tests/data/state_estimation/distribution-case/sym_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9192016554667/tests/data/state_estimation/distribution-case/update_batch.json` & `power-grid-model-1.5.0rc9193215149708/tests/data/state_estimation/distribution-case/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9192016554667/tests/data/state_estimation/dummy-test-sym/input.json` & `power-grid-model-1.5.0rc9193215149708/tests/data/state_estimation/dummy-test-sym/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9192016554667/tests/data/state_estimation/dummy-test-sym/sym_output.json` & `power-grid-model-1.5.0rc9193215149708/tests/data/state_estimation/dummy-test-sym/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9192016554667/tests/data/state_estimation/node-injection-sensor-and-zero-injection/input.json` & `power-grid-model-1.5.0rc9193215149708/tests/data/state_estimation/node-injection-sensor-and-zero-injection/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9192016554667/tests/data/state_estimation/node-injection-sensor-and-zero-injection/sym_output.json` & `power-grid-model-1.5.0rc9193215149708/tests/data/state_estimation/node-injection-sensor-and-zero-injection/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9192016554667/tests/data/state_estimation/single-line-load/input.json` & `power-grid-model-1.5.0rc9193215149708/tests/data/state_estimation/single-line-load/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9192016554667/tests/data/state_estimation/single-line-load/sym_output.json` & `power-grid-model-1.5.0rc9193215149708/tests/data/state_estimation/single-line-load/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9192016554667/tests/data/state_estimation/three_winding_transformer/input.json` & `power-grid-model-1.5.0rc9193215149708/tests/data/state_estimation/three_winding_transformer/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9192016554667/tests/data/state_estimation/three_winding_transformer/sym_output.json` & `power-grid-model-1.5.0rc9193215149708/tests/data/state_estimation/three_winding_transformer/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9192016554667/tests/data/state_estimation/transmission-case/README.md` & `power-grid-model-1.5.0rc9193215149708/tests/data/state_estimation/transmission-case/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9192016554667/tests/data/state_estimation/transmission-case/asym_output.json` & `power-grid-model-1.5.0rc9193215149708/tests/data/state_estimation/transmission-case/asym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9192016554667/tests/data/state_estimation/transmission-case/input.json` & `power-grid-model-1.5.0rc9193215149708/tests/data/state_estimation/transmission-case/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9192016554667/tests/data/state_estimation/transmission-case/sym_output.json` & `power-grid-model-1.5.0rc9193215149708/tests/data/state_estimation/transmission-case/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9192016554667/tests/unit/test_0Z_model_validation.py` & `power-grid-model-1.5.0rc9193215149708/tests/unit/test_0Z_model_validation.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9192016554667/tests/unit/test_error_handling.py` & `power-grid-model-1.5.0rc9193215149708/tests/unit/test_error_handling.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9192016554667/tests/unit/test_meta_data.py` & `power-grid-model-1.5.0rc9193215149708/tests/unit/test_meta_data.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9192016554667/tests/unit/test_power_grid_model.py` & `power-grid-model-1.5.0rc9193215149708/tests/unit/test_power_grid_model.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9192016554667/tests/unit/test_utils.py` & `power-grid-model-1.5.0rc9193215149708/tests/unit/test_utils.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9192016554667/tests/unit/utils.py` & `power-grid-model-1.5.0rc9193215149708/tests/unit/utils.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9192016554667/tests/unit/validation/test_assertions.py` & `power-grid-model-1.5.0rc9193215149708/tests/unit/validation/test_assertions.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9192016554667/tests/unit/validation/test_batch_validation.py` & `power-grid-model-1.5.0rc9193215149708/tests/unit/validation/test_batch_validation.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9192016554667/tests/unit/validation/test_errors.py` & `power-grid-model-1.5.0rc9193215149708/tests/unit/validation/test_errors.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9192016554667/tests/unit/validation/test_input_validation.py` & `power-grid-model-1.5.0rc9193215149708/tests/unit/validation/test_input_validation.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9192016554667/tests/unit/validation/test_rules.py` & `power-grid-model-1.5.0rc9193215149708/tests/unit/validation/test_rules.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9192016554667/tests/unit/validation/test_utils.py` & `power-grid-model-1.5.0rc9193215149708/tests/unit/validation/test_utils.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9192016554667/tests/unit/validation/test_validation_functions.py` & `power-grid-model-1.5.0rc9193215149708/tests/unit/validation/test_validation_functions.py`

 * *Files identical despite different names*

