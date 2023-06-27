# Comparing `tmp/hera_sim-4.0.0.tar.gz` & `tmp/hera_sim-4.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hera_sim-4.0.0.tar", last modified: Mon May 22 20:28:31 2023, max compression
+gzip compressed data, was "hera_sim-4.1.0.tar", last modified: Tue Jun 27 19:28:49 2023, max compression
```

## Comparing `hera_sim-4.0.0.tar` & `hera_sim-4.1.0.tar`

### file list

```diff
@@ -1,137 +1,151 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:28:31.396020 hera_sim-4.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-05-22 20:28:19.000000 hera_sim-4.0.0/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-05-22 20:28:19.000000 hera_sim-4.0.0/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:28:31.360020 hera_sim-4.0.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:28:31.364020 hera_sim-4.0.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-05-22 20:28:19.000000 hera_sim-4.0.0/.github/workflows/publish.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-05-22 20:28:19.000000 hera_sim-4.0.0/.github/workflows/test_suite.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-05-22 20:28:19.000000 hera_sim-4.0.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-05-22 20:28:19.000000 hera_sim-4.0.0/.isort.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-05-22 20:28:19.000000 hera_sim-4.0.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-05-22 20:28:19.000000 hera_sim-4.0.0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-22 20:28:19.000000 hera_sim-4.0.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)    18215 2023-05-22 20:28:19.000000 hera_sim-4.0.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2427 2023-05-22 20:28:19.000000 hera_sim-4.0.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-22 20:28:19.000000 hera_sim-4.0.0/LICENSE.rst
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-22 20:28:19.000000 hera_sim-4.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4639 2023-05-22 20:28:31.396020 hera_sim-4.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3631 2023-05-22 20:28:19.000000 hera_sim-4.0.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:28:31.364020 hera_sim-4.0.0/config_examples/
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-22 20:28:19.000000 hera_sim-4.0.0/config_examples/simulator.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4973 2023-05-22 20:28:19.000000 hera_sim-4.0.0/config_examples/template_config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:28:31.368020 hera_sim-4.0.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     5586 2023-05-22 20:28:19.000000 hera_sim-4.0.0/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:28:31.368020 hera_sim-4.0.0/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-05-22 20:28:19.000000 hera_sim-4.0.0/docs/_templates/class.rst
--rw-r--r--   0 runner    (1001) docker     (123)      727 2023-05-22 20:28:19.000000 hera_sim-4.0.0/docs/_templates/module.rst
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-22 20:28:19.000000 hera_sim-4.0.0/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-22 20:28:19.000000 hera_sim-4.0.0/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6244 2023-05-22 20:28:19.000000 hera_sim-4.0.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-22 20:28:19.000000 hera_sim-4.0.0/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-22 20:28:19.000000 hera_sim-4.0.0/docs/environment.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-05-22 20:28:19.000000 hera_sim-4.0.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-22 20:28:19.000000 hera_sim-4.0.0/docs/notes_for_developers.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:28:31.368020 hera_sim-4.0.0/docs/reference/
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-05-22 20:28:19.000000 hera_sim-4.0.0/docs/reference/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-05-22 20:28:19.000000 hera_sim-4.0.0/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:28:31.376020 hera_sim-4.0.0/docs/tutorials/
--rw-r--r--   0 runner    (1001) docker     (123)   344696 2023-05-22 20:28:19.000000 hera_sim-4.0.0/docs/tutorials/end_to_end_example.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     9038 2023-05-22 20:28:19.000000 hera_sim-4.0.0/docs/tutorials/hera_sim_cli.rst
--rw-r--r--   0 runner    (1001) docker     (123)   145439 2023-05-22 20:28:19.000000 hera_sim-4.0.0/docs/tutorials/hera_sim_defaults.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)  2406697 2023-05-22 20:28:19.000000 hera_sim-4.0.0/docs/tutorials/hera_sim_simulator.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)  2634846 2023-05-22 20:28:19.000000 hera_sim-4.0.0/docs/tutorials/hera_sim_tour.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     2629 2023-05-22 20:28:19.000000 hera_sim-4.0.0/docs/tutorials/hera_sim_vis_cli.rst
--rw-r--r--   0 runner    (1001) docker     (123)   462848 2023-05-22 20:28:19.000000 hera_sim-4.0.0/docs/tutorials/mutual_coupling_example.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    95849 2023-05-22 20:28:19.000000 hera_sim-4.0.0/docs/tutorials/polybeam_simulation.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)   165797 2023-05-22 20:28:19.000000 hera_sim-4.0.0/docs/tutorials/visibility_simulator.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-05-22 20:28:19.000000 hera_sim-4.0.0/docs/tutorials.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:28:31.380020 hera_sim-4.0.0/hera_sim/
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-05-22 20:28:19.000000 hera_sim-4.0.0/hera_sim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-05-22 20:28:19.000000 hera_sim-4.0.0/hera_sim/__yaml_constructors.py
--rw-r--r--   0 runner    (1001) docker     (123)    41518 2023-05-22 20:28:19.000000 hera_sim-4.0.0/hera_sim/adjustment.py
--rw-r--r--   0 runner    (1001) docker     (123)     6374 2023-05-22 20:28:19.000000 hera_sim-4.0.0/hera_sim/antpos.py
--rw-r--r--   0 runner    (1001) docker     (123)    48424 2023-05-22 20:28:19.000000 hera_sim-4.0.0/hera_sim/beams.py
--rw-r--r--   0 runner    (1001) docker     (123)     9076 2023-05-22 20:28:19.000000 hera_sim-4.0.0/hera_sim/cli_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    11975 2023-05-22 20:28:19.000000 hera_sim-4.0.0/hera_sim/components.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:28:31.384020 hera_sim-4.0.0/hera_sim/config/
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-05-22 20:28:19.000000 hera_sim-4.0.0/hera_sim/config/H1C.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-05-22 20:28:19.000000 hera_sim-4.0.0/hera_sim/config/H2C.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-22 20:28:19.000000 hera_sim-4.0.0/hera_sim/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-05-22 20:28:19.000000 hera_sim-4.0.0/hera_sim/config/debug.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:28:31.388020 hera_sim-4.0.0/hera_sim/data/
--rw-r--r--   0 runner    (1001) docker     (123)   815652 2023-05-22 20:28:19.000000 hera_sim-4.0.0/hera_sim/data/H37_FR_Filters_small.npz
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-05-22 20:28:19.000000 hera_sim-4.0.0/hera_sim/data/HERA_H1C_BANDPASS.npy
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-22 20:28:19.000000 hera_sim-4.0.0/hera_sim/data/HERA_H1C_BEAM_POLY.npy
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-05-22 20:28:19.000000 hera_sim-4.0.0/hera_sim/data/HERA_H1C_RFI_STATIONS.npy
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-22 20:28:19.000000 hera_sim-4.0.0/hera_sim/data/HERA_H2C_BANDPASS.npy
--rw-r--r--   0 runner    (1001) docker     (123)     3680 2023-05-22 20:28:19.000000 hera_sim-4.0.0/hera_sim/data/HERA_H2C_BEAM_MODEL.npz
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-22 20:28:19.000000 hera_sim-4.0.0/hera_sim/data/HERA_H2C_BEAM_POLY.npy
--rw-r--r--   0 runner    (1001) docker     (123)     4488 2023-05-22 20:28:19.000000 hera_sim-4.0.0/hera_sim/data/HERA_H2C_RFI_STATIONS.npy
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-22 20:28:19.000000 hera_sim-4.0.0/hera_sim/data/HERA_LAT_LON_ALT.npy
--rw-r--r--   0 runner    (1001) docker     (123)    51246 2023-05-22 20:28:19.000000 hera_sim-4.0.0/hera_sim/data/HERA_Tsky_Reformatted.npz
--rw-r--r--   0 runner    (1001) docker     (123)    50598 2023-05-22 20:28:19.000000 hera_sim-4.0.0/hera_sim/data/HERA_Tsky_vs_LST.npz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:28:31.360020 hera_sim-4.0.0/hera_sim/data/tutorials_data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:28:31.388020 hera_sim-4.0.0/hera_sim/data/tutorials_data/end_to_end/
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-05-22 20:28:19.000000 hera_sim-4.0.0/hera_sim/data/tutorials_data/end_to_end/array_layout.csv
--rw-r--r--   0 runner    (1001) docker     (123)     3200 2023-05-22 20:28:19.000000 hera_sim-4.0.0/hera_sim/data/tutorials_data/end_to_end/make_mock_catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-05-22 20:28:19.000000 hera_sim-4.0.0/hera_sim/data/tutorials_data/end_to_end/obsparams.yaml
--rw-r--r--   0 runner    (1001) docker     (123)   229229 2023-05-22 20:28:19.000000 hera_sim-4.0.0/hera_sim/data/tutorials_data/end_to_end/sample_catalog.txt
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-22 20:28:19.000000 hera_sim-4.0.0/hera_sim/data/tutorials_data/end_to_end/telescope.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:28:31.388020 hera_sim-4.0.0/hera_sim/data/tutorials_data/visibility_simulator/
--rw-r--r--   0 runner    (1001) docker     (123)     2773 2023-05-22 20:28:19.000000 hera_sim-4.0.0/hera_sim/data/tutorials_data/visibility_simulator/antenna_layout_hera_phase1.csv
--rw-r--r--   0 runner    (1001) docker     (123)    20400 2023-05-22 20:28:19.000000 hera_sim-4.0.0/hera_sim/data/tutorials_data/visibility_simulator/gleam_top50.skyh5
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-05-22 20:28:19.000000 hera_sim-4.0.0/hera_sim/data/tutorials_data/visibility_simulator/obsparam_hera_phase1_gleam_top50.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-05-22 20:28:19.000000 hera_sim-4.0.0/hera_sim/data/tutorials_data/visibility_simulator/telescope_config_hera_airy.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13419 2023-05-22 20:28:19.000000 hera_sim-4.0.0/hera_sim/defaults.py
--rw-r--r--   0 runner    (1001) docker     (123)     3810 2023-05-22 20:28:19.000000 hera_sim-4.0.0/hera_sim/eor.py
--rw-r--r--   0 runner    (1001) docker     (123)    11305 2023-05-22 20:28:19.000000 hera_sim-4.0.0/hera_sim/foregrounds.py
--rw-r--r--   0 runner    (1001) docker     (123)    13243 2023-05-22 20:28:19.000000 hera_sim-4.0.0/hera_sim/interpolators.py
--rw-r--r--   0 runner    (1001) docker     (123)     8030 2023-05-22 20:28:19.000000 hera_sim-4.0.0/hera_sim/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     8403 2023-05-22 20:28:19.000000 hera_sim-4.0.0/hera_sim/noise.py
--rw-r--r--   0 runner    (1001) docker     (123)    16249 2023-05-22 20:28:19.000000 hera_sim-4.0.0/hera_sim/rfi.py
--rw-r--r--   0 runner    (1001) docker     (123)    60721 2023-05-22 20:28:19.000000 hera_sim-4.0.0/hera_sim/sigchain.py
--rw-r--r--   0 runner    (1001) docker     (123)    63166 2023-05-22 20:28:19.000000 hera_sim-4.0.0/hera_sim/simulate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:28:31.392020 hera_sim-4.0.0/hera_sim/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-05-22 20:28:19.000000 hera_sim-4.0.0/hera_sim/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    39798 2023-05-22 20:28:19.000000 hera_sim-4.0.0/hera_sim/tests/test_adjustment.py
--rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-05-22 20:28:19.000000 hera_sim-4.0.0/hera_sim/tests/test_antpos.py
--rw-r--r--   0 runner    (1001) docker     (123)    16610 2023-05-22 20:28:19.000000 hera_sim-4.0.0/hera_sim/tests/test_beams.py
--rw-r--r--   0 runner    (1001) docker     (123)     6333 2023-05-22 20:28:19.000000 hera_sim-4.0.0/hera_sim/tests/test_cli_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6996 2023-05-22 20:28:19.000000 hera_sim-4.0.0/hera_sim/tests/test_compare_pyuvsim.py
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-05-22 20:28:19.000000 hera_sim-4.0.0/hera_sim/tests/test_components.py
--rw-r--r--   0 runner    (1001) docker     (123)     3119 2023-05-22 20:28:19.000000 hera_sim-4.0.0/hera_sim/tests/test_defaults.py
--rw-r--r--   0 runner    (1001) docker     (123)     2441 2023-05-22 20:28:19.000000 hera_sim-4.0.0/hera_sim/tests/test_eor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5377 2023-05-22 20:28:19.000000 hera_sim-4.0.0/hera_sim/tests/test_foregrounds.py
--rw-r--r--   0 runner    (1001) docker     (123)     7663 2023-05-22 20:28:19.000000 hera_sim-4.0.0/hera_sim/tests/test_interpolators.py
--rw-r--r--   0 runner    (1001) docker     (123)     3555 2023-05-22 20:28:19.000000 hera_sim-4.0.0/hera_sim/tests/test_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     4228 2023-05-22 20:28:19.000000 hera_sim-4.0.0/hera_sim/tests/test_noise.py
--rw-r--r--   0 runner    (1001) docker     (123)     5505 2023-05-22 20:28:19.000000 hera_sim-4.0.0/hera_sim/tests/test_rfi.py
--rw-r--r--   0 runner    (1001) docker     (123)    34096 2023-05-22 20:28:19.000000 hera_sim-4.0.0/hera_sim/tests/test_sigchain.py
--rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-05-22 20:28:19.000000 hera_sim-4.0.0/hera_sim/tests/test_sim_red_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2291 2023-05-22 20:28:19.000000 hera_sim-4.0.0/hera_sim/tests/test_simulate_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    22073 2023-05-22 20:28:19.000000 hera_sim-4.0.0/hera_sim/tests/test_simulator.py
--rw-r--r--   0 runner    (1001) docker     (123)    15813 2023-05-22 20:28:19.000000 hera_sim-4.0.0/hera_sim/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    17137 2023-05-22 20:28:19.000000 hera_sim-4.0.0/hera_sim/tests/test_vis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-05-22 20:28:19.000000 hera_sim-4.0.0/hera_sim/tests/test_yaml_constructors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:28:31.392020 hera_sim-4.0.0/hera_sim/tests/testdata/
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-22 20:28:19.000000 hera_sim-4.0.0/hera_sim/tests/testdata/healvis_catalog.txt
--rw-r--r--   0 runner    (1001) docker     (123)    26497 2023-05-22 20:28:19.000000 hera_sim-4.0.0/hera_sim/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-05-22 20:28:19.000000 hera_sim-4.0.0/hera_sim/vis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:28:31.396020 hera_sim-4.0.0/hera_sim/visibilities/
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-05-22 20:28:19.000000 hera_sim-4.0.0/hera_sim/visibilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-05-22 20:28:19.000000 hera_sim-4.0.0/hera_sim/visibilities/pyuvsim_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    16828 2023-05-22 20:28:19.000000 hera_sim-4.0.0/hera_sim/visibilities/simulators.py
--rw-r--r--   0 runner    (1001) docker     (123)    16850 2023-05-22 20:28:19.000000 hera_sim-4.0.0/hera_sim/visibilities/vis_cpu.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:28:31.384020 hera_sim-4.0.0/hera_sim.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4639 2023-05-22 20:28:31.000000 hera_sim-4.0.0/hera_sim.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3546 2023-05-22 20:28:31.000000 hera_sim-4.0.0/hera_sim.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 20:28:31.000000 hera_sim-4.0.0/hera_sim.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 20:28:30.000000 hera_sim-4.0.0/hera_sim.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-05-22 20:28:31.000000 hera_sim-4.0.0/hera_sim.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-22 20:28:31.000000 hera_sim-4.0.0/hera_sim.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-05-22 20:28:19.000000 hera_sim-4.0.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:28:31.396020 hera_sim-4.0.0/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     7038 2023-05-22 20:28:19.000000 hera_sim-4.0.0/scripts/hera-sim-simulate.py
--rw-r--r--   0 runner    (1001) docker     (123)     7707 2023-05-22 20:28:19.000000 hera_sim-4.0.0/scripts/hera-sim-vis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-05-22 20:28:31.396020 hera_sim-4.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 20:28:19.000000 hera_sim-4.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 19:28:49.612172 hera_sim-4.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-06-27 19:28:40.000000 hera_sim-4.1.0/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-06-27 19:28:40.000000 hera_sim-4.1.0/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 19:28:49.556171 hera_sim-4.1.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 19:28:49.568171 hera_sim-4.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-06-27 19:28:40.000000 hera_sim-4.1.0/.github/workflows/publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-06-27 19:28:40.000000 hera_sim-4.1.0/.github/workflows/test_suite.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-06-27 19:28:40.000000 hera_sim-4.1.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-06-27 19:28:40.000000 hera_sim-4.1.0/.isort.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-06-27 19:28:40.000000 hera_sim-4.1.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-06-27 19:28:40.000000 hera_sim-4.1.0/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-27 19:28:40.000000 hera_sim-4.1.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    20362 2023-06-27 19:28:40.000000 hera_sim-4.1.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2427 2023-06-27 19:28:40.000000 hera_sim-4.1.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-27 19:28:40.000000 hera_sim-4.1.0/LICENSE.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-27 19:28:40.000000 hera_sim-4.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4639 2023-06-27 19:28:49.612172 hera_sim-4.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3631 2023-06-27 19:28:40.000000 hera_sim-4.1.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 19:28:49.568171 hera_sim-4.1.0/config_examples/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-27 19:28:40.000000 hera_sim-4.1.0/config_examples/simulator.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4973 2023-06-27 19:28:40.000000 hera_sim-4.1.0/config_examples/template_config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 19:28:49.568171 hera_sim-4.1.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     5586 2023-06-27 19:28:40.000000 hera_sim-4.1.0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 19:28:49.568171 hera_sim-4.1.0/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-06-27 19:28:40.000000 hera_sim-4.1.0/docs/_templates/class.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-06-27 19:28:40.000000 hera_sim-4.1.0/docs/_templates/module.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-27 19:28:40.000000 hera_sim-4.1.0/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-27 19:28:40.000000 hera_sim-4.1.0/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6393 2023-06-27 19:28:40.000000 hera_sim-4.1.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-27 19:28:40.000000 hera_sim-4.1.0/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-06-27 19:28:40.000000 hera_sim-4.1.0/docs/environment.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-06-27 19:28:40.000000 hera_sim-4.1.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-06-27 19:28:40.000000 hera_sim-4.1.0/docs/notes_for_developers.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 19:28:49.568171 hera_sim-4.1.0/docs/reference/
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-06-27 19:28:40.000000 hera_sim-4.1.0/docs/reference/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-06-27 19:28:40.000000 hera_sim-4.1.0/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 19:28:49.580171 hera_sim-4.1.0/docs/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (123)   344696 2023-06-27 19:28:40.000000 hera_sim-4.1.0/docs/tutorials/end_to_end_example.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     9038 2023-06-27 19:28:40.000000 hera_sim-4.1.0/docs/tutorials/hera_sim_cli.rst
+-rw-r--r--   0 runner    (1001) docker     (123)   145439 2023-06-27 19:28:40.000000 hera_sim-4.1.0/docs/tutorials/hera_sim_defaults.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)  2406697 2023-06-27 19:28:40.000000 hera_sim-4.1.0/docs/tutorials/hera_sim_simulator.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)  2634846 2023-06-27 19:28:40.000000 hera_sim-4.1.0/docs/tutorials/hera_sim_tour.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     2629 2023-06-27 19:28:40.000000 hera_sim-4.1.0/docs/tutorials/hera_sim_vis_cli.rst
+-rw-r--r--   0 runner    (1001) docker     (123)   462848 2023-06-27 19:28:40.000000 hera_sim-4.1.0/docs/tutorials/mutual_coupling_example.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    95849 2023-06-27 19:28:40.000000 hera_sim-4.1.0/docs/tutorials/polybeam_simulation.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   165797 2023-06-27 19:28:40.000000 hera_sim-4.1.0/docs/tutorials/visibility_simulator.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-06-27 19:28:40.000000 hera_sim-4.1.0/docs/tutorials.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 19:28:49.584171 hera_sim-4.1.0/hera_sim/
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-06-27 19:28:40.000000 hera_sim-4.1.0/hera_sim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-06-27 19:28:40.000000 hera_sim-4.1.0/hera_sim/__yaml_constructors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41449 2023-06-27 19:28:40.000000 hera_sim-4.1.0/hera_sim/adjustment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6374 2023-06-27 19:28:40.000000 hera_sim-4.1.0/hera_sim/antpos.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48320 2023-06-27 19:28:40.000000 hera_sim-4.1.0/hera_sim/beams.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9112 2023-06-27 19:28:40.000000 hera_sim-4.1.0/hera_sim/cli_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11975 2023-06-27 19:28:40.000000 hera_sim-4.1.0/hera_sim/components.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 19:28:49.588172 hera_sim-4.1.0/hera_sim/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-06-27 19:28:40.000000 hera_sim-4.1.0/hera_sim/config/H1C.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-06-27 19:28:40.000000 hera_sim-4.1.0/hera_sim/config/H2C.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-27 19:28:40.000000 hera_sim-4.1.0/hera_sim/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-06-27 19:28:40.000000 hera_sim-4.1.0/hera_sim/config/debug.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 19:28:49.592172 hera_sim-4.1.0/hera_sim/data/
+-rw-r--r--   0 runner    (1001) docker     (123)   815652 2023-06-27 19:28:40.000000 hera_sim-4.1.0/hera_sim/data/H37_FR_Filters_small.npz
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-06-27 19:28:40.000000 hera_sim-4.1.0/hera_sim/data/HERA_H1C_BANDPASS.npy
+-rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-06-27 19:28:40.000000 hera_sim-4.1.0/hera_sim/data/HERA_H1C_BEAM_INTEGRALS.npz
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-06-27 19:28:40.000000 hera_sim-4.1.0/hera_sim/data/HERA_H1C_BEAM_POLY.npy
+-rw-r--r--   0 runner    (1001) docker     (123)    25092 2023-06-27 19:28:40.000000 hera_sim-4.1.0/hera_sim/data/HERA_H1C_REFLECTIONS.npz
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-06-27 19:28:40.000000 hera_sim-4.1.0/hera_sim/data/HERA_H1C_RFI_STATIONS.npy
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-06-27 19:28:40.000000 hera_sim-4.1.0/hera_sim/data/HERA_H2C_BANDPASS.npy
+-rw-r--r--   0 runner    (1001) docker     (123)     3680 2023-06-27 19:28:40.000000 hera_sim-4.1.0/hera_sim/data/HERA_H2C_BEAM_MODEL.npz
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-06-27 19:28:40.000000 hera_sim-4.1.0/hera_sim/data/HERA_H2C_BEAM_POLY.npy
+-rw-r--r--   0 runner    (1001) docker     (123)     4488 2023-06-27 19:28:40.000000 hera_sim-4.1.0/hera_sim/data/HERA_H2C_RFI_STATIONS.npy
+-rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-06-27 19:28:40.000000 hera_sim-4.1.0/hera_sim/data/HERA_H4C_BANDPASS.npz
+-rw-r--r--   0 runner    (1001) docker     (123)     3800 2023-06-27 19:28:40.000000 hera_sim-4.1.0/hera_sim/data/HERA_H4C_BEAM_INTEGRALS.npz
+-rw-r--r--   0 runner    (1001) docker     (123)    49740 2023-06-27 19:28:40.000000 hera_sim-4.1.0/hera_sim/data/HERA_H4C_REFLECTIONS.npz
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-27 19:28:40.000000 hera_sim-4.1.0/hera_sim/data/HERA_LAT_LON_ALT.npy
+-rw-r--r--   0 runner    (1001) docker     (123)    51246 2023-06-27 19:28:40.000000 hera_sim-4.1.0/hera_sim/data/HERA_Tsky_Reformatted.npz
+-rw-r--r--   0 runner    (1001) docker     (123)    50598 2023-06-27 19:28:40.000000 hera_sim-4.1.0/hera_sim/data/HERA_Tsky_vs_LST.npz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 19:28:49.560171 hera_sim-4.1.0/hera_sim/data/tutorials_data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 19:28:49.596171 hera_sim-4.1.0/hera_sim/data/tutorials_data/end_to_end/
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-06-27 19:28:40.000000 hera_sim-4.1.0/hera_sim/data/tutorials_data/end_to_end/array_layout.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     3200 2023-06-27 19:28:40.000000 hera_sim-4.1.0/hera_sim/data/tutorials_data/end_to_end/make_mock_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-06-27 19:28:40.000000 hera_sim-4.1.0/hera_sim/data/tutorials_data/end_to_end/obsparams.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)   229229 2023-06-27 19:28:40.000000 hera_sim-4.1.0/hera_sim/data/tutorials_data/end_to_end/sample_catalog.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-06-27 19:28:40.000000 hera_sim-4.1.0/hera_sim/data/tutorials_data/end_to_end/telescope.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 19:28:49.596171 hera_sim-4.1.0/hera_sim/data/tutorials_data/visibility_simulator/
+-rw-r--r--   0 runner    (1001) docker     (123)     2773 2023-06-27 19:28:40.000000 hera_sim-4.1.0/hera_sim/data/tutorials_data/visibility_simulator/antenna_layout_hera_phase1.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    20400 2023-06-27 19:28:40.000000 hera_sim-4.1.0/hera_sim/data/tutorials_data/visibility_simulator/gleam_top50.skyh5
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-06-27 19:28:40.000000 hera_sim-4.1.0/hera_sim/data/tutorials_data/visibility_simulator/obsparam_hera_phase1_gleam_top50.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-06-27 19:28:40.000000 hera_sim-4.1.0/hera_sim/data/tutorials_data/visibility_simulator/telescope_config_hera_airy.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13419 2023-06-27 19:28:40.000000 hera_sim-4.1.0/hera_sim/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3810 2023-06-27 19:28:40.000000 hera_sim-4.1.0/hera_sim/eor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11305 2023-06-27 19:28:40.000000 hera_sim-4.1.0/hera_sim/foregrounds.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14162 2023-06-27 19:28:40.000000 hera_sim-4.1.0/hera_sim/interpolators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8030 2023-06-27 19:28:40.000000 hera_sim-4.1.0/hera_sim/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8403 2023-06-27 19:28:40.000000 hera_sim-4.1.0/hera_sim/noise.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16249 2023-06-27 19:28:40.000000 hera_sim-4.1.0/hera_sim/rfi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61987 2023-06-27 19:28:40.000000 hera_sim-4.1.0/hera_sim/sigchain.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63166 2023-06-27 19:28:40.000000 hera_sim-4.1.0/hera_sim/simulate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 19:28:49.604172 hera_sim-4.1.0/hera_sim/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-06-27 19:28:40.000000 hera_sim-4.1.0/hera_sim/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39798 2023-06-27 19:28:40.000000 hera_sim-4.1.0/hera_sim/tests/test_adjustment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-06-27 19:28:40.000000 hera_sim-4.1.0/hera_sim/tests/test_antpos.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16631 2023-06-27 19:28:40.000000 hera_sim-4.1.0/hera_sim/tests/test_beams.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6333 2023-06-27 19:28:40.000000 hera_sim-4.1.0/hera_sim/tests/test_cli_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6996 2023-06-27 19:28:40.000000 hera_sim-4.1.0/hera_sim/tests/test_compare_pyuvsim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-06-27 19:28:40.000000 hera_sim-4.1.0/hera_sim/tests/test_components.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3119 2023-06-27 19:28:40.000000 hera_sim-4.1.0/hera_sim/tests/test_defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2441 2023-06-27 19:28:40.000000 hera_sim-4.1.0/hera_sim/tests/test_eor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5377 2023-06-27 19:28:40.000000 hera_sim-4.1.0/hera_sim/tests/test_foregrounds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8145 2023-06-27 19:28:40.000000 hera_sim-4.1.0/hera_sim/tests/test_interpolators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3555 2023-06-27 19:28:40.000000 hera_sim-4.1.0/hera_sim/tests/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4228 2023-06-27 19:28:40.000000 hera_sim-4.1.0/hera_sim/tests/test_noise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5505 2023-06-27 19:28:40.000000 hera_sim-4.1.0/hera_sim/tests/test_rfi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34979 2023-06-27 19:28:40.000000 hera_sim-4.1.0/hera_sim/tests/test_sigchain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-06-27 19:28:40.000000 hera_sim-4.1.0/hera_sim/tests/test_sim_red_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2291 2023-06-27 19:28:40.000000 hera_sim-4.1.0/hera_sim/tests/test_simulate_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22073 2023-06-27 19:28:40.000000 hera_sim-4.1.0/hera_sim/tests/test_simulator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16007 2023-06-27 19:28:40.000000 hera_sim-4.1.0/hera_sim/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17767 2023-06-27 19:28:40.000000 hera_sim-4.1.0/hera_sim/tests/test_vis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2363 2023-06-27 19:28:40.000000 hera_sim-4.1.0/hera_sim/tests/test_vis_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-06-27 19:28:40.000000 hera_sim-4.1.0/hera_sim/tests/test_yaml_constructors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 19:28:49.604172 hera_sim-4.1.0/hera_sim/tests/testdata/
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-06-27 19:28:40.000000 hera_sim-4.1.0/hera_sim/tests/testdata/healvis_catalog.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 19:28:49.608172 hera_sim-4.1.0/hera_sim/tests/testdata/hera-sim-vis-config/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      929 2023-06-27 19:28:40.000000 hera_sim-4.1.0/hera_sim/tests/testdata/hera-sim-vis-config/H4C-antennas-slim.csv
+-rw-r--r--   0 runner    (1001) docker     (123)  2635200 2023-06-27 19:28:40.000000 hera_sim-4.1.0/hera_sim/tests/testdata/hera-sim-vis-config/NF_HERA_Dipole_small.fits
+-rw-r--r--   0 runner    (1001) docker     (123)    59077 2023-06-27 19:28:40.000000 hera_sim-4.1.0/hera_sim/tests/testdata/hera-sim-vis-config/gleam_50srcs.vot
+-rwxr-xr-x   0 runner    (1001) docker     (123)      130 2023-06-27 19:28:40.000000 hera_sim-4.1.0/hera_sim/tests/testdata/hera-sim-vis-config/h4c_idr2.1_teleconfig.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      110 2023-06-27 19:28:40.000000 hera_sim-4.1.0/hera_sim/tests/testdata/hera-sim-vis-config/viscpu.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      124 2023-06-27 19:28:40.000000 hera_sim-4.1.0/hera_sim/tests/testdata/hera-sim-vis-config/visgpu.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    27060 2023-06-27 19:28:40.000000 hera_sim-4.1.0/hera_sim/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-06-27 19:28:40.000000 hera_sim-4.1.0/hera_sim/vis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 19:28:49.608172 hera_sim-4.1.0/hera_sim/visibilities/
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-06-27 19:28:40.000000 hera_sim-4.1.0/hera_sim/visibilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9659 2023-06-27 19:28:40.000000 hera_sim-4.1.0/hera_sim/visibilities/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-06-27 19:28:40.000000 hera_sim-4.1.0/hera_sim/visibilities/pyuvsim_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18643 2023-06-27 19:28:40.000000 hera_sim-4.1.0/hera_sim/visibilities/simulators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20480 2023-06-27 19:28:40.000000 hera_sim-4.1.0/hera_sim/visibilities/vis_cpu.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 19:28:49.584171 hera_sim-4.1.0/hera_sim.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4639 2023-06-27 19:28:49.000000 hera_sim-4.1.0/hera_sim.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4184 2023-06-27 19:28:49.000000 hera_sim-4.1.0/hera_sim.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 19:28:49.000000 hera_sim-4.1.0/hera_sim.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 19:28:49.000000 hera_sim-4.1.0/hera_sim.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-06-27 19:28:49.000000 hera_sim-4.1.0/hera_sim.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-27 19:28:49.000000 hera_sim-4.1.0/hera_sim.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-06-27 19:28:40.000000 hera_sim-4.1.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 19:28:49.608172 hera_sim-4.1.0/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     7038 2023-06-27 19:28:40.000000 hera_sim-4.1.0/scripts/hera-sim-simulate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-06-27 19:28:40.000000 hera_sim-4.1.0/scripts/hera-sim-vis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-06-27 19:28:49.612172 hera_sim-4.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 19:28:40.000000 hera_sim-4.1.0/setup.py
```

### Comparing `hera_sim-4.0.0/.coveragerc` & `hera_sim-4.1.0/.coveragerc`

 * *Files 26% similar despite different names*

```diff
@@ -1,12 +1,31 @@
 [run]
-omit = hera_sim/tests/*
+omit =
+    */tests/*
+    */docs/*
+    setup.py
+branch = true
+source =
+    hera_sim
 
 [report]
-omit = hera_sim/tests/*
+omit =
+    */tests/*
+    */docs/*
+    setup.py
+
+show_missing = true
+
+[paths]
+source =
+    hera_sim
+    */site-packages"
+tests =
+    hera_sim/tests
+    */tests
 
 # Regexes for lines to exclude from consideration
 exclude_lines =
     # Have to re-enable the standard pragma
     pragma: no cover
     pragma: nocover
```

### Comparing `hera_sim-4.0.0/.flake8` & `hera_sim-4.1.0/.flake8`

 * *Files 7% similar despite different names*

```diff
@@ -11,14 +11,16 @@
     D401,
     # allow method names to be the same as python builtins
     A003,
     # inline strong start-string without end-string. This is OK in the case of **kwargs in parameters.
     RST210,
     # Logging statement uses f-string.
     G004,
+    # Logging statement uses + (this makes no sense...)
+    G003,
 max-line-length = 88
 # Should be 18.
 max-complexity = 35
 exclude =
     development/*
 per-file-ignores =
     # print statements allowed in tests
```

### Comparing `hera_sim-4.0.0/.github/workflows/publish.yaml` & `hera_sim-4.1.0/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `hera_sim-4.0.0/.github/workflows/test_suite.yaml` & `hera_sim-4.1.0/.github/workflows/test_suite.yaml`

 * *Files 14% similar despite different names*

```diff
@@ -32,19 +32,20 @@
       - name: Setup Python
         uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python-version }}
 
       - name: Install
         run: |
+          pip install --upgrade pip
           pip install .[tests]
 
       - name: Run Tests
         run: |
-          python -m pytest
+          python -m pytest --log-cli-level INFO
 
       - name: Upload coverage report
         uses: codecov/codecov-action@v3.1.3
         with:
           token: ${{ secrets.CODECOV_TOKEN }}
           file: ./coverage.xml
           flags: unittests
```

### Comparing `hera_sim-4.0.0/.pre-commit-config.yaml` & `hera_sim-4.1.0/.pre-commit-config.yaml`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-exclude: 'config.yaml|config_examples/.*.yaml|hera_sim/config/H1C.yaml|hera_sim/config/H2C.yaml|setup.py'
+exclude: 'config.yaml|config_examples/.*.yaml|hera_sim/config/H1C.yaml|hera_sim/config/H2C.yaml|setup.py|hera_sim/tests/testdata/hera-sim-vis-config/NF_HERA_Dipole_small.fits'
 
 repos:
 - repo: https://github.com/pre-commit/pre-commit-hooks
   rev: v4.4.0
   hooks:
   - id: trailing-whitespace
   - id: check-added-large-files
@@ -29,30 +29,30 @@
           - flake8-rst-docstrings
           - flake8-rst
 #          - flake8-markdown    # not available for flake8>5 (check later...)
           - flake8-bugbear
           - flake8-comprehensions
           - flake8-print
 -   repo: https://github.com/psf/black
-    rev: 23.1.0
+    rev: 23.3.0
     hooks:
     - id: black
 -   repo: https://github.com/pre-commit/pygrep-hooks
     rev: v1.10.0
     hooks:
       - id: rst-backticks
 
 - repo: https://github.com/PyCQA/isort
   rev: 5.12.0
   hooks:
   - id: isort
 
 - repo: https://github.com/asottile/pyupgrade
-  rev: v3.3.1
+  rev: v3.7.0
   hooks:
   - id: pyupgrade
     args: [--py39-plus]
 
 - repo: https://github.com/asottile/setup-cfg-fmt
-  rev: v2.2.0
+  rev: v2.3.0
   hooks:
   - id: setup-cfg-fmt
```

### Comparing `hera_sim-4.0.0/CHANGELOG.rst` & `hera_sim-4.1.0/CHANGELOG.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,54 @@
 =========
 Changelog
 =========
 
+v4.1.0 [2023.06.26]
+===================
+This release heavily focuses on performance of the visibility simulators, and in
+particular the ``VisCPU`` simulator.
+
+Fixed
+-----
+- Passing ``spline_interp_opts`` now correctly pipes these options through to the
+  visibility simulators.
+
+Added
+-----
+- New ``_blt_order_kws`` class-attribute for ``VisibilitySimulator`` subclasses, that
+  can be used to create the mock metadata in an order corresponding to that required
+  by the simulator (instead of re-ordering after data creation, which can take some
+  time).
+- New optional ``compress_data_model()`` method on ``VisibilitySimulator`` subclasses
+  that allows unnecessary metadata in the ``UVData`` object to be dropped before
+  simulation (can be restored afterwards with the associated ``restore_data_model()``).
+  This can reduce peak memory usage.
+- New ``check_antenna_conjugation`` parameter for the ``VisCPU`` simulator, to allow
+  turning off checks for antenna conjugation, which takes time and is unnecessary for
+  mock datasets.
+- Dependency on ``hera-cli-utils`` which adds options like ``--log-level`` and ``--profile``
+  to ``hera-sim-vis.py``.
+- Option to use a taper in generating a bandpass.
+- ``utils.tanh_window`` function for generating a two-sided tanh window.
+- ``interpolators.Reflection`` class for building a complex reflection
+  coefficient interpolator from a ``npz`` archive.
+- Reflection coefficient and beam integral ``npz`` archives for the phase 1
+  and phase 4 systems (i.e., dipole feed and Vivaldi feed).
+
+Changed
+-------
+- ``run_check_acceptability`` is now ``False`` by default when constructing simulations
+  from obsparams configuration files, to improve performance.
+- For ``VisCPU`` simulator, we no longer copy the whole data array when simulating, but
+  instead just fill the existing one, to save on peak RAM.
+- Made ``VisCPU._reorder_vis()`` much faster (like 99% time reduction).
+- The ``--compress`` option to ``hera-sim-vis.py`` is no longer a boolean flag but
+  takes a file argument. This file will be written as a cache of the baseline-time indices
+  required to keep when compressing by redundancy.
+
 v4.0.0 [2023.05.22]
 ===================
 
 Breaking Changes
 ----------------
 - Removed the ``HealVis`` wrapper. Use ``pyuvsim`` instead.
```

### Comparing `hera_sim-4.0.0/CONTRIBUTING.rst` & `hera_sim-4.1.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `hera_sim-4.0.0/LICENSE.rst` & `hera_sim-4.1.0/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `hera_sim-4.0.0/PKG-INFO` & `hera_sim-4.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hera_sim
-Version: 4.0.0
+Version: 4.1.0
 Summary: A collection of simulation routines describing the HERA instrument.
 Home-page: https://github.com/HERA-Team/hera_sim
 Author: HERA Team
 Author-email: steven.g.murray@asu.edu
 License: MIT
 Project-URL: Documentation, https://hera_sim.readthedocs.org
 Platform: any
```

### Comparing `hera_sim-4.0.0/README.rst` & `hera_sim-4.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `hera_sim-4.0.0/config_examples/template_config.yaml` & `hera_sim-4.1.0/config_examples/template_config.yaml`

 * *Files identical despite different names*

### Comparing `hera_sim-4.0.0/docs/Makefile` & `hera_sim-4.1.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `hera_sim-4.0.0/docs/_templates/class.rst` & `hera_sim-4.1.0/docs/_templates/class.rst`

 * *Files identical despite different names*

### Comparing `hera_sim-4.0.0/docs/_templates/module.rst` & `hera_sim-4.1.0/docs/_templates/module.rst`

 * *Files identical despite different names*

### Comparing `hera_sim-4.0.0/docs/conf.py` & `hera_sim-4.1.0/docs/conf.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,14 +10,20 @@
 # If extensions (or modules to document with autodoc) are in another directory,
 # add these directories to sys.path here. If the directory is relative to the
 # documentation root, use os.path.abspath to make it absolute, like shown here.
 #
 from pkg_resources import get_distribution
 
 __version__ = get_distribution("hera_sim").version
+
+# Do the following to see if hera_sim can be imported properly, and throw a reasonable
+# error with traceback if not.
+import hera_sim
+
+del hera_sim
 # -- Project information -----------------------------------------------------
 
 project = "hera_sim"
 copyright = "2020, HERA-Team"
 author = "HERA-Team"
```

### Comparing `hera_sim-4.0.0/docs/reference/index.rst` & `hera_sim-4.1.0/docs/reference/index.rst`

 * *Files identical despite different names*

### Comparing `hera_sim-4.0.0/docs/tutorials/end_to_end_example.ipynb` & `hera_sim-4.1.0/docs/tutorials/end_to_end_example.ipynb`

 * *Files identical despite different names*

### Comparing `hera_sim-4.0.0/docs/tutorials/hera_sim_cli.rst` & `hera_sim-4.1.0/docs/tutorials/hera_sim_cli.rst`

 * *Files identical despite different names*

### Comparing `hera_sim-4.0.0/docs/tutorials/hera_sim_defaults.ipynb` & `hera_sim-4.1.0/docs/tutorials/hera_sim_defaults.ipynb`

 * *Files identical despite different names*

### Comparing `hera_sim-4.0.0/docs/tutorials/hera_sim_simulator.ipynb` & `hera_sim-4.1.0/docs/tutorials/hera_sim_simulator.ipynb`

 * *Files identical despite different names*

### Comparing `hera_sim-4.0.0/docs/tutorials/hera_sim_tour.ipynb` & `hera_sim-4.1.0/docs/tutorials/hera_sim_tour.ipynb`

 * *Files identical despite different names*

### Comparing `hera_sim-4.0.0/docs/tutorials/hera_sim_vis_cli.rst` & `hera_sim-4.1.0/docs/tutorials/hera_sim_vis_cli.rst`

 * *Files identical despite different names*

### Comparing `hera_sim-4.0.0/docs/tutorials/mutual_coupling_example.ipynb` & `hera_sim-4.1.0/docs/tutorials/mutual_coupling_example.ipynb`

 * *Files identical despite different names*

### Comparing `hera_sim-4.0.0/docs/tutorials/polybeam_simulation.ipynb` & `hera_sim-4.1.0/docs/tutorials/polybeam_simulation.ipynb`

 * *Files identical despite different names*

### Comparing `hera_sim-4.0.0/docs/tutorials/visibility_simulator.ipynb` & `hera_sim-4.1.0/docs/tutorials/visibility_simulator.ipynb`

 * *Files identical despite different names*

### Comparing `hera_sim-4.0.0/docs/tutorials.rst` & `hera_sim-4.1.0/docs/tutorials.rst`

 * *Files identical despite different names*

### Comparing `hera_sim-4.0.0/hera_sim/__init__.py` & `hera_sim-4.1.0/hera_sim/__init__.py`

 * *Files identical despite different names*

### Comparing `hera_sim-4.0.0/hera_sim/__yaml_constructors.py` & `hera_sim-4.1.0/hera_sim/__yaml_constructors.py`

 * *Files identical despite different names*

### Comparing `hera_sim-4.0.0/hera_sim/adjustment.py` & `hera_sim-4.1.0/hera_sim/adjustment.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,14 @@
 
     HERA_CAL = True
 except (ModuleNotFoundError, FileNotFoundError) as err:  # pragma: no cover
     if err is ModuleNotFoundError:
         missing = "hera-calibration"
     else:
         missing = "git"
-    warn(f"{missing} is not installed. Rephasing tool unavailable.")
     HERA_CAL = False
 
 
 logger = logging.getLogger(__name__)
 
 
 def adjust_to_reference(
```

### Comparing `hera_sim-4.0.0/hera_sim/antpos.py` & `hera_sim-4.1.0/hera_sim/antpos.py`

 * *Files identical despite different names*

### Comparing `hera_sim-4.0.0/hera_sim/beams.py` & `hera_sim-4.1.0/hera_sim/beams.py`

 * *Files 0% similar despite different names*

```diff
@@ -185,17 +185,17 @@
     pol_efield_beam = dipole_mod[:, ...] * beam_vals[np.newaxis, np.newaxis, ...]
 
     # Correct it for frequency dependency.
     # extract modulus and phase of the beams
     modulus = np.abs(pol_efield_beam)
     phase = np.angle(pol_efield_beam)
     # assume linear shift of phase along frequency
-    shift = -np.pi / 18e6 * (freqs[:, np.newaxis] - ref_freq)  # shape (Nfreq, 1)
+    shift = -np.pi / 18e6 * (freqs - ref_freq)  # shape (Nfreq, )
     # shift the phase
-    phase += shift[np.newaxis, np.newaxis, :, :]
+    phase += shift[np.newaxis, np.newaxis, :, np.newaxis]
     # upscale the modulus
     modulus = np.power(modulus, 0.6)  # ad-hoc
     # map the phase to [-pi; +pi]
     phase = utils.wrap2pipi(phase)
     # reconstruct
     pol_efield_beam = modulus * np.exp(1j * phase)
 
@@ -636,15 +636,14 @@
         # Call interp() method on parent class
         interp_data, interp_basis_vector = super().interp(
             az_array=az_array,
             za_array=za_array,
             freq_array=freq_array,
             reuse_spline=reuse_spline,
         )
-
         # Smooth step function
         step = 0.5 * (
             1.0 + np.tanh((za_array - self.mainlobe_width) / self.transition_width)
         )
 
         # Construct sidelobe perturbations (angle- and frequency-dependent)
         p_za = self._sidelobe_modulation_za(
@@ -653,17 +652,15 @@
         p_freq = self._sidelobe_modulation_freq(
             freq_array, scale=self._scale_pfreq, zeropoint=self._zeropoint_pfreq
         )
         p_za = np.atleast_1d(self.perturb_scale * p_za)
         p_freq = np.atleast_1d(self.freq_perturb_scale * p_freq)
 
         # Modulate primary beam by sidelobe perturbation function
-        interp_data *= 1.0 + (step * p_za)[np.newaxis, :] * (
-            1.0 + p_freq[:, np.newaxis]
-        )
+        interp_data *= 1.0 + np.outer(1.0 + p_freq, step * p_za)
 
         # Add mainlobe stretch factor
         if self.mainlobe_scale != 1.0:
             # Subtract and re-add Gaussian normalized to 1 at za = 0
             w = self.mainlobe_width / 2.0
             mainlobe0 = np.exp(-0.5 * (za_array / w) ** 2.0)
             mainlobe_pert = np.exp(-0.5 * (za_array / (w * self.mainlobe_scale)) ** 2.0)
@@ -732,16 +729,16 @@
             Npixels/(Naxis1, Naxis2) or az_array.size if az/za_arrays are passed)
         """
         # Empty data array
         interp_data = np.zeros((2, 2, freq_array.size, az_array.size), dtype=float)
 
         # Frequency scaling
         fscale = (freq_array / self.ref_freq) ** self.spectral_index
-        radial_coord = za_array[np.newaxis, ...] / fscale[:, np.newaxis]
-        axial_coord = az_array[np.newaxis, ...]
+        radial_coord = za_array / fscale
+        axial_coord = az_array
 
         # Primary beam values from Zernike polynomial
         values = self.zernike(
             coeffs=self.beam_coeffs,
             x=radial_coord * np.cos(axial_coord),
             y=radial_coord * np.sin(axial_coord),
         )
```

### Comparing `hera_sim-4.0.0/hera_sim/cli_utils.py` & `hera_sim-4.1.0/hera_sim/cli_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 """Useful helper functions and argparsers for running simulations via CLI."""
+from __future__ import annotations
+
 import itertools
 import numpy as np
 import os
 import warnings
 from pyuvdata import UVData
 
 from .defaults import SEASON_CONFIGS
```

### Comparing `hera_sim-4.0.0/hera_sim/components.py` & `hera_sim-4.1.0/hera_sim/components.py`

 * *Files identical despite different names*

### Comparing `hera_sim-4.0.0/hera_sim/config/H1C.yaml` & `hera_sim-4.1.0/hera_sim/config/H1C.yaml`

 * *Files identical despite different names*

### Comparing `hera_sim-4.0.0/hera_sim/config/H2C.yaml` & `hera_sim-4.1.0/hera_sim/config/H2C.yaml`

 * *Files identical despite different names*

### Comparing `hera_sim-4.0.0/hera_sim/config/debug.yaml` & `hera_sim-4.1.0/hera_sim/config/debug.yaml`

 * *Files identical despite different names*

### Comparing `hera_sim-4.0.0/hera_sim/data/H37_FR_Filters_small.npz` & `hera_sim-4.1.0/hera_sim/data/H37_FR_Filters_small.npz`

 * *Files identical despite different names*

### Comparing `hera_sim-4.0.0/hera_sim/data/HERA_H1C_RFI_STATIONS.npy` & `hera_sim-4.1.0/hera_sim/data/HERA_H1C_RFI_STATIONS.npy`

 * *Files identical despite different names*

### Comparing `hera_sim-4.0.0/hera_sim/data/HERA_H2C_BEAM_MODEL.npz` & `hera_sim-4.1.0/hera_sim/data/HERA_H2C_BEAM_MODEL.npz`

 * *Files identical despite different names*

### Comparing `hera_sim-4.0.0/hera_sim/data/HERA_H2C_RFI_STATIONS.npy` & `hera_sim-4.1.0/hera_sim/data/HERA_H2C_RFI_STATIONS.npy`

 * *Files identical despite different names*

### Comparing `hera_sim-4.0.0/hera_sim/data/HERA_Tsky_Reformatted.npz` & `hera_sim-4.1.0/hera_sim/data/HERA_Tsky_Reformatted.npz`

 * *Files identical despite different names*

### Comparing `hera_sim-4.0.0/hera_sim/data/HERA_Tsky_vs_LST.npz` & `hera_sim-4.1.0/hera_sim/data/HERA_Tsky_vs_LST.npz`

 * *Files identical despite different names*

### Comparing `hera_sim-4.0.0/hera_sim/data/tutorials_data/end_to_end/make_mock_catalog.py` & `hera_sim-4.1.0/hera_sim/data/tutorials_data/end_to_end/make_mock_catalog.py`

 * *Files identical despite different names*

### Comparing `hera_sim-4.0.0/hera_sim/data/tutorials_data/end_to_end/sample_catalog.txt` & `hera_sim-4.1.0/hera_sim/data/tutorials_data/end_to_end/sample_catalog.txt`

 * *Files identical despite different names*

### Comparing `hera_sim-4.0.0/hera_sim/data/tutorials_data/visibility_simulator/antenna_layout_hera_phase1.csv` & `hera_sim-4.1.0/hera_sim/data/tutorials_data/visibility_simulator/antenna_layout_hera_phase1.csv`

 * *Files identical despite different names*

### Comparing `hera_sim-4.0.0/hera_sim/data/tutorials_data/visibility_simulator/gleam_top50.skyh5` & `hera_sim-4.1.0/hera_sim/data/tutorials_data/visibility_simulator/gleam_top50.skyh5`

 * *Files identical despite different names*

### Comparing `hera_sim-4.0.0/hera_sim/defaults.py` & `hera_sim-4.1.0/hera_sim/defaults.py`

 * *Files identical despite different names*

### Comparing `hera_sim-4.0.0/hera_sim/eor.py` & `hera_sim-4.1.0/hera_sim/eor.py`

 * *Files identical despite different names*

### Comparing `hera_sim-4.0.0/hera_sim/foregrounds.py` & `hera_sim-4.1.0/hera_sim/foregrounds.py`

 * *Files identical despite different names*

### Comparing `hera_sim-4.0.0/hera_sim/interpolators.py` & `hera_sim-4.1.0/hera_sim/interpolators.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 
 from hera_sim import DATA_PATH
 
 INTERP_OBJECTS = {
     "1d": (
         "beam",
         "bandpass",
+        "reflection",
     ),
     "2d": ("Tsky_mdl",),
 }
 
 
 def _check_path(datafile):
     # if the datafile is not an absolute path, assume it's in the data folder
@@ -270,18 +271,19 @@
         This is raised if the choice of interpolator and the required type
         of the ref_file do not agree (i.e. trying to make a 'poly1d' object
         using a .npz file as a reference). An AssertionError is also raised
         if the .npz for generating an 'interp1d' object does not have the
         correct arrays in its archive.
     """
 
-    def __init__(self, datafile, **interp_kwargs):
+    def __init__(self, datafile, obj_type=None, **interp_kwargs):
         super().__init__(datafile, **interp_kwargs)
         self._interp_type = self._interp_kwargs.pop("interpolator", "poly1d")
-        self._obj = None
+        self._obj = obj_type
+        self._check_format()
 
     def __call__(self, freqs):
         """Evaluate the interpolation object at the given frequencies."""
         return self._interpolator(freqs)
 
     @cached_property
     def _interpolator(self):
@@ -336,27 +338,51 @@
     datafile : str
         Passed to the superclass constructor.
     interp_kwargs : unpacked dict, optional
         Passed to the superclass constructor.
     """
 
     def __init__(self, datafile, **interp_kwargs):
-        super().__init__(datafile, **interp_kwargs)
-        self._obj = "beam"
-        self._check_format()
+        super().__init__(datafile, obj_type="beam", **interp_kwargs)
 
 
 class Bandpass(FreqInterpolator):
     """Bandpass interpolation object.
 
     Parameters
     ----------
     datafile : str
         Passed to the superclass constructor.
     interp_kwargs : unpacked dict, optional
         Passed to the superclass constructor.
     """
 
     def __init__(self, datafile, **interp_kwargs):
-        super().__init__(datafile, **interp_kwargs)
-        self._obj = "bandpass"
-        self._check_format()
+        super().__init__(datafile, obj_type="bandpass", **interp_kwargs)
+
+
+class Reflection(FreqInterpolator):
+    """Complex reflection coefficient interpolator."""
+
+    def __init__(self, datafile, **interp_kwargs):
+        if "interpolator" not in interp_kwargs:
+            interp_kwargs["interpolator"] = "interp1d"
+        super().__init__(datafile, obj_type="reflection", **interp_kwargs)
+
+    @cached_property
+    def _re_interp(self):
+        interp_kwargs = {"kind": "cubic"}
+        interp_kwargs.update(self._interp_kwargs)
+        return interp1d(
+            self._data["freqs"], self._data[self._obj].real, **interp_kwargs
+        )
+
+    @cached_property
+    def _im_interp(self):
+        interp_kwargs = {"kind": "cubic"}
+        interp_kwargs.update(self._interp_kwargs)
+        return interp1d(
+            self._data["freqs"], self._data[self._obj].imag, **interp_kwargs
+        )
+
+    def __call__(self, freqs):
+        return self._re_interp(freqs) + 1j * self._im_interp(freqs)
```

### Comparing `hera_sim-4.0.0/hera_sim/io.py` & `hera_sim-4.1.0/hera_sim/io.py`

 * *Files identical despite different names*

### Comparing `hera_sim-4.0.0/hera_sim/noise.py` & `hera_sim-4.1.0/hera_sim/noise.py`

 * *Files identical despite different names*

### Comparing `hera_sim-4.0.0/hera_sim/rfi.py` & `hera_sim-4.1.0/hera_sim/rfi.py`

 * *Files identical despite different names*

### Comparing `hera_sim-4.0.0/hera_sim/sigchain.py` & `hera_sim-4.1.0/hera_sim/sigchain.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,46 +18,73 @@
 from scipy.signal import blackmanharris
 from typing import Callable
 
 from . import DATA_PATH, interpolators, utils
 from .components import component
 from .defaults import _defaults
 
+try:
+    from uvtools.dspec import gen_window
+
+    HAVE_UVTOOLS = True
+except ModuleNotFoundError:
+    HAVE_UVTOOLS = False
+
 
 @component
 class Gain:
     """Base class for systematic gains."""
 
     pass
 
 
 class Bandpass(Gain):
     """Generate bandpass gains.
 
     Parameters
     ----------
-    gain_spread : float, optional
-        Standard deviation of random gains.
-    dly_rng : tuple, optional
-        Lower and upper range of delays which are uniformly sampled.
-    bp_poly : callable or array_like, optional
-        If an array, polynomial coefficients to evaluate. Otherwise, a function
-        of frequency that can be evaluated to generate real numbers giving
-        the bandpass gain.
+    gain_spread
+        Standard deviation of random gains. Default is about 10% variation across
+        antennas.
+    dly_rng
+        Lower and upper range of delays which are uniformly sampled, in nanoseconds.
+        Default is -20 ns to +20 ns.
+    bp_poly
+        Either an array of polynomial coefficients, a callable object that provides
+        the bandpass amplitude as a function of frequency (in GHz), or a string
+        providing a path to a file that can be read into an interpolation object.
+        By default, the HERA Phase One bandpass is used.
+    taper
+        Taper to apply to the simulated gains. Default is to not apply a taper.
+    taper_kwds
+        Keyword arguments used in generating the taper.
     """
 
     _alias = ("gains", "bandpass_gain")
     is_multiplicative = True
     return_type = "per_antenna"
     attrs_to_pull = dict(
         ants="antpos",
     )
 
-    def __init__(self, gain_spread=0.1, dly_rng=(-20, 20), bp_poly=None):
-        super().__init__(gain_spread=gain_spread, dly_rng=dly_rng, bp_poly=bp_poly)
+    def __init__(
+        self,
+        gain_spread: float | np.ndarray = 0.1,
+        dly_rng: tuple = (-20, 20),
+        bp_poly: str | callable | np.ndarray | None = None,
+        taper: str | callable | np.ndarray | None = None,
+        taper_kwds: dict | None = None,
+    ):
+        super().__init__(
+            gain_spread=gain_spread,
+            dly_rng=dly_rng,
+            bp_poly=bp_poly,
+            taper=taper,
+            taper_kwds=taper_kwds,
+        )
 
     def __call__(self, freqs, ants, **kwargs):
         """Generate the bandpass.
 
         Parameters
         ----------
         freqs : array_like of float
@@ -71,23 +98,47 @@
             Keys are antenna numbers and values are arrays of bandpass
             gains as a function of frequency.
         """
         # validate kwargs
         self._check_kwargs(**kwargs)
 
         # unpack the kwargs
-        (gain_spread, dly_rng, bp_poly) = self._extract_kwarg_values(**kwargs)
+        (gain_spread, dly_rng, bp_poly, taper, taper_kwds) = self._extract_kwarg_values(
+            **kwargs
+        )
 
         # get the bandpass gains
         bandpass = self._gen_bandpass(freqs, ants, gain_spread, bp_poly)
 
         # get the delay phases
         phase = self._gen_delay_phase(freqs, ants, dly_rng)
 
-        return {ant: bandpass[ant] * phase[ant] for ant in ants}
+        if taper is None:
+            taper = np.ones(freqs.size)
+        elif isinstance(taper, str):
+            if taper_kwds is None:
+                taper_kwds = {}
+            if taper == "tanh":
+                taper = utils.tanh_window(freqs, **taper_kwds)
+            elif HAVE_UVTOOLS:
+                taper = gen_window(taper, freqs.size, **taper_kwds)
+            else:  # pragma: no cover
+                taper = np.ones(freqs.size)
+                warnings.warn(
+                    "uvtools is not installed, so you must provide the taper.",
+                    stacklevel=1,
+                )
+        elif callable(taper):
+            if taper_kwds is None:
+                taper_kwds = {}
+            taper = taper(freqs, **taper_kwds)
+        elif not isinstance(taper, np.ndarray):
+            raise ValueError("Unsupported choice of taper.")
+
+        return {ant: bandpass[ant] * phase[ant] * taper for ant in ants}
 
     @_defaults
     def _gen_bandpass(self, freqs, ants, gain_spread=0.1, bp_poly=None):
         if bp_poly is None:
             # default to the H1C bandpass
             bp_poly = np.load(DATA_PATH / "HERA_H1C_BANDPASS.npy")
         elif isinstance(bp_poly, str):
@@ -937,16 +988,14 @@
             invert=True,
             use_numba=use_numba,
         )
 
     @staticmethod
     def build_coupling_matrix(
         freqs: np.ndarray,
-        ant_1_array: np.ndarray,
-        ant_2_array: np.ndarray,
         array_layout: dict,
         uvbeam: UVBeam | str,
         reflection: np.ndarray | Callable | None = None,
         omega_p: np.ndarray | Callable | None = None,
         pixel_interp: str | None = "az_za_simple",
         freq_interp: str | None = "cubic",
         **beam_kwargs,
@@ -956,21 +1005,14 @@
         See the :class:`MutualCoupling` class docstring for a description of
         the coupling matrix.
 
         Parameters
         ----------
         freqs
             The observed frequencies, in GHz.
-        ant_1_array
-            Array of integers specifying the number of the first antenna in each
-            visibility. Required for calculating the coupling matrix and the
-            coupled visibilities.
-        ant_2_array
-            Array of integers specifying the number of the second antenna in each
-            visibility.
         array_layout
             Dictionary mapping antenna numbers to their positions in local East-
             North-Up coordinates, expressed in meters. Not required if providing
             a pre-calculated coupling matrix.
         uvbeam
             The beam (i.e. Jones matrix) to be used for calculating the coupling
             matrix. This may either be a :class:`pyuvdata.UVBeam` object, a path
```

### Comparing `hera_sim-4.0.0/hera_sim/simulate.py` & `hera_sim-4.1.0/hera_sim/simulate.py`

 * *Files identical despite different names*

### Comparing `hera_sim-4.0.0/hera_sim/tests/conftest.py` & `hera_sim-4.1.0/hera_sim/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `hera_sim-4.0.0/hera_sim/tests/test_adjustment.py` & `hera_sim-4.1.0/hera_sim/tests/test_adjustment.py`

 * *Files identical despite different names*

### Comparing `hera_sim-4.0.0/hera_sim/tests/test_antpos.py` & `hera_sim-4.1.0/hera_sim/tests/test_antpos.py`

 * *Files identical despite different names*

### Comparing `hera_sim-4.0.0/hera_sim/tests/test_beams.py` & `hera_sim-4.1.0/hera_sim/tests/test_beams.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,15 +57,15 @@
     n = np.where(lsqr < 1, np.sqrt(1 - lsqr), 0)
 
     # Generate azimuth and zenith angle.
     az = -np.arctan2(m, L)
     za = np.pi / 2 - np.arcsin(n)
 
     freqs = np.arange(1e8, 2.01e8, 0.04e8)
-
+    print(len(freqs))
     eval_beam = polybeam.interp(az, za, freqs)
 
     # Check that calling the interp() method with wrongly sized
     # coordinates results in an error
     with pytest.raises(ValueError):
         _ = polybeam.interp(az, za[:-1], freqs)
```

### Comparing `hera_sim-4.0.0/hera_sim/tests/test_cli_utils.py` & `hera_sim-4.1.0/hera_sim/tests/test_cli_utils.py`

 * *Files identical despite different names*

### Comparing `hera_sim-4.0.0/hera_sim/tests/test_compare_pyuvsim.py` & `hera_sim-4.1.0/hera_sim/tests/test_compare_pyuvsim.py`

 * *Files identical despite different names*

### Comparing `hera_sim-4.0.0/hera_sim/tests/test_components.py` & `hera_sim-4.1.0/hera_sim/tests/test_components.py`

 * *Files identical despite different names*

### Comparing `hera_sim-4.0.0/hera_sim/tests/test_defaults.py` & `hera_sim-4.1.0/hera_sim/tests/test_defaults.py`

 * *Files identical despite different names*

### Comparing `hera_sim-4.0.0/hera_sim/tests/test_eor.py` & `hera_sim-4.1.0/hera_sim/tests/test_eor.py`

 * *Files identical despite different names*

### Comparing `hera_sim-4.0.0/hera_sim/tests/test_foregrounds.py` & `hera_sim-4.1.0/hera_sim/tests/test_foregrounds.py`

 * *Files identical despite different names*

### Comparing `hera_sim-4.0.0/hera_sim/tests/test_interpolators.py` & `hera_sim-4.1.0/hera_sim/tests/test_interpolators.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import pytest
 
 import numpy as np
 from scipy.interpolate import RectBivariateSpline, interp1d
 
-from hera_sim.interpolators import Bandpass, Beam, Tsky, _check_path, _read
+from hera_sim.interpolators import Bandpass, Beam, Reflection, Tsky, _check_path, _read
 
 INTERPOLATORS = {"beam": Beam, "bandpass": Bandpass, "tsky": Tsky}
 
 
 @pytest.fixture(scope="function")
 def freqs():
     return np.linspace(0.1, 0.2, 100, endpoint=False)
@@ -85,14 +85,24 @@
     data_file = str(tmp_path / f"shape_test_{model}_{interpolator}")
     interpolator = construct_interpolator(freqs, model, interpolator, data_file)
     new_freqs = np.linspace(0.12, 0.18, 720)
     resampled_data = interpolator(new_freqs)
     assert resampled_data.size == new_freqs.size
 
 
+def test_reflection_interpolator(freqs, tmp_path):
+    data_file = str(tmp_path / "sample_reflections.npz")
+    mock_data = np.exp(2j * np.pi * (freqs - freqs.mean()) / freqs.max())
+    np.savez(data_file, freqs=freqs[::2], reflection=mock_data[::2])
+    interpolator = Reflection(data_file)
+    interp_data = interpolator(freqs[1:-2:2])
+    assert np.allclose(interp_data.real, mock_data[1:-2:2].real)
+    assert np.allclose(interp_data.imag, mock_data[1:-2:2].imag)
+
+
 def test_tsky_exception_no_freqs(lsts, Tsky_mdl, tmp_path):
     data_file = str(tmp_path / "test_tsky_no_freqs.npz")
     np.savez(data_file, lsts=lsts, tsky=Tsky_mdl[None, :, :], meta={"pols": ("xx",)})
     with pytest.raises(AssertionError) as err:
         Tsky(data_file)
     assert "frequencies corresponding to the sky temperature" in err.value.args[0]
```

### Comparing `hera_sim-4.0.0/hera_sim/tests/test_io.py` & `hera_sim-4.1.0/hera_sim/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `hera_sim-4.0.0/hera_sim/tests/test_noise.py` & `hera_sim-4.1.0/hera_sim/tests/test_noise.py`

 * *Files identical despite different names*

### Comparing `hera_sim-4.0.0/hera_sim/tests/test_rfi.py` & `hera_sim-4.1.0/hera_sim/tests/test_rfi.py`

 * *Files identical despite different names*

### Comparing `hera_sim-4.0.0/hera_sim/tests/test_sigchain.py` & `hera_sim-4.1.0/hera_sim/tests/test_sigchain.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,57 +10,14 @@
 from hera_sim import DATA_PATH, foregrounds, noise, sigchain
 from hera_sim.interpolators import Bandpass, Beam
 from hera_sim.io import empty_uvdata
 
 np.random.seed(0)
 
 
-def test_gen_bandpass():
-    fqs = np.linspace(0.1, 0.2, 1024, endpoint=False)
-    g = sigchain.gen_bandpass(fqs, [1, 2], gain_spread=0)
-    assert 1 in g
-    assert 2 in g
-    assert g[1].size == fqs.size
-    assert np.all(g[1] == g[2])
-    g = sigchain.gen_bandpass(fqs, list(range(10)), 0.2)
-    assert not np.all(g[1] == g[2])
-
-
-def test_gen_delay_phs():
-    fqs = np.linspace(0.12, 0.18, 1024, endpoint=False)
-    phs = sigchain.gen_delay_phs(fqs, [1, 2], dly_rng=(0, 20))
-    assert len(phs) == 2
-    assert 1 in phs
-    assert 2 in phs
-    assert np.allclose(np.abs(phs[1]), 1)
-    p = np.polyfit(fqs, np.unwrap(np.angle(phs[1])), deg=1)
-    assert np.any(np.isclose(p[-1] % (2 * np.pi), (0, 2 * np.pi), atol=1e-2))
-    assert p[0] <= 20 * 2 * np.pi
-    assert p[0] >= 0
-
-
-def test_gen_gains():
-    fqs = np.linspace(0.12, 0.18, 1024, endpoint=False)
-    g = sigchain.gen_gains(fqs, [1, 2], gain_spread=0, dly_rng=(10, 20))
-    assert np.allclose(np.abs(g[1]), np.abs(g[2]), rtol=1e-5)
-    for i in g:
-        p = np.polyfit(fqs, np.unwrap(np.angle(g[i])), deg=1)
-        assert np.any(np.isclose(p[-1] % (2 * np.pi), (0, 2 * np.pi), atol=1e-2))
-        assert p[0] <= 20 * 2 * np.pi
-        assert p[0] >= 10 * 2 * np.pi
-
-
-def test_apply_gains():
-    fqs = np.linspace(0.12, 0.18, 1024, endpoint=False)
-    vis = np.ones((100, fqs.size), dtype=complex)
-    g = sigchain.gen_gains(fqs, [1, 2], gain_spread=0, dly_rng=(10, 10))
-    gvis = sigchain.apply_gains(vis, g, (1, 2))
-    assert np.allclose(np.angle(gvis), 0, rtol=1e-5)
-
-
 @pytest.fixture(scope="function")
 def fqs():
     return np.linspace(0.1, 0.2, 100, endpoint=False)
 
 
 @pytest.fixture(scope="function")
 def lsts():
@@ -105,14 +62,87 @@
 
 
 @pytest.fixture(scope="function")
 def vfft(vis):
     return uvtools.utils.FFT(vis, axis=1)
 
 
+def test_gen_bandpass():
+    fqs = np.linspace(0.1, 0.2, 1024, endpoint=False)
+    g = sigchain.gen_bandpass(fqs, [1, 2], gain_spread=0)
+    assert 1 in g
+    assert 2 in g
+    assert g[1].size == fqs.size
+    assert np.all(g[1] == g[2])
+    g = sigchain.gen_bandpass(fqs, list(range(10)), 0.2)
+    assert not np.all(g[1] == g[2])
+
+
+def test_gen_delay_phs():
+    fqs = np.linspace(0.12, 0.18, 1024, endpoint=False)
+    phs = sigchain.gen_delay_phs(fqs, [1, 2], dly_rng=(0, 20))
+    assert len(phs) == 2
+    assert 1 in phs
+    assert 2 in phs
+    assert np.allclose(np.abs(phs[1]), 1)
+    p = np.polyfit(fqs, np.unwrap(np.angle(phs[1])), deg=1)
+    assert np.any(np.isclose(p[-1] % (2 * np.pi), (0, 2 * np.pi), atol=1e-2))
+    assert p[0] <= 20 * 2 * np.pi
+    assert p[0] >= 0
+
+
+def test_gen_gains():
+    fqs = np.linspace(0.12, 0.18, 1024, endpoint=False)
+    g = sigchain.gen_gains(fqs, [1, 2], gain_spread=0, dly_rng=(10, 20))
+    assert np.allclose(np.abs(g[1]), np.abs(g[2]), rtol=1e-5)
+    for i in g:
+        p = np.polyfit(fqs, np.unwrap(np.angle(g[i])), deg=1)
+        assert np.any(np.isclose(p[-1] % (2 * np.pi), (0, 2 * np.pi), atol=1e-2))
+        assert p[0] <= 20 * 2 * np.pi
+        assert p[0] >= 10 * 2 * np.pi
+
+
+def test_apply_gains():
+    fqs = np.linspace(0.12, 0.18, 1024, endpoint=False)
+    vis = np.ones((100, fqs.size), dtype=complex)
+    g = sigchain.gen_gains(fqs, [1, 2], gain_spread=0, dly_rng=(10, 10))
+    gvis = sigchain.apply_gains(vis, g, (1, 2))
+    assert np.allclose(np.angle(gvis), 0, rtol=1e-5)
+
+
+@pytest.mark.parametrize("taper", ["tanh", "bh", "custom", "callable"])
+def test_bandpass_with_taper(fqs, taper):
+    taper_kwds = None
+    if taper == "custom":
+        taper = np.linspace(0, 1, fqs.size)
+    elif taper == "callable":
+
+        def taper(freqs):
+            return np.sin(np.pi * (freqs - freqs.mean() / freqs.max()))
+
+    elif taper == "tanh":
+        taper_kwds = dict(x_min=fqs[10], x_max=fqs[-10])
+
+    base_bandpass = sigchain.gen_gains(fqs, [0], gain_spread=0, dly_rng=(0, 0))[0]
+    bandpass = sigchain.gen_gains(
+        fqs,
+        [0],
+        gain_spread=0,
+        dly_rng=(0, 0),
+        taper=taper,
+        taper_kwds=taper_kwds,
+    )[0]
+    assert not np.allclose(base_bandpass, bandpass)
+
+
+def test_bandpass_bad_taper(fqs):
+    with pytest.raises(ValueError, match="Unsupported choice of taper."):
+        sigchain.gen_gains(fqs, [0], taper=13)
+
+
 def test_reflection_gains_correct_delays(
     fqs,
     vis,
     dlys,
 ):
     # introduce a cable reflection into the autocorrelation
     gains = sigchain.gen_reflection_gains(fqs, [0], amp=[1e-1], dly=[300], phs=[1])
```

### Comparing `hera_sim-4.0.0/hera_sim/tests/test_sim_red_data.py` & `hera_sim-4.1.0/hera_sim/tests/test_sim_red_data.py`

 * *Files identical despite different names*

### Comparing `hera_sim-4.0.0/hera_sim/tests/test_simulate_cli.py` & `hera_sim-4.1.0/hera_sim/tests/test_simulate_cli.py`

 * *Files identical despite different names*

### Comparing `hera_sim-4.0.0/hera_sim/tests/test_simulator.py` & `hera_sim-4.1.0/hera_sim/tests/test_simulator.py`

 * *Files identical despite different names*

### Comparing `hera_sim-4.0.0/hera_sim/tests/test_utils.py` & `hera_sim-4.1.0/hera_sim/tests/test_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -437,7 +437,13 @@
     vis = utils.reshape_vis(
         utils.reshape_vis(*reshape_args, invert=False, use_numba=jit),
         *reshape_args[1:],
         invert=True,
         use_numba=jit,
     )
     assert np.all(sim.data_array == vis)
+
+
+def test_tanh_window_warning():
+    with pytest.warns(UserWarning, match="Insufficient information"):
+        window = utils.tanh_window(np.linspace(0, 1, 100))
+    assert np.all(window == 1)
```

### Comparing `hera_sim-4.0.0/hera_sim/tests/test_vis.py` & `hera_sim-4.1.0/hera_sim/tests/test_vis.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
 if HAVE_GPU:
 
     class VisGPU(VisCPU):
         """Simple mock class to make testing VisCPU with use_gpu=True easier"""
 
         def __init__(self, *args, **kwargs):
-            super().__init__(*args, use_gpu=True, **kwargs)
+            super().__init__(*args, use_gpu=True, ref_time="min", **kwargs)
 
     SIMULATORS = SIMULATORS + (VisGPU,)
 
 
 np.random.seed(0)
 NTIMES = 10
 NPIX = 12 * 16**2
@@ -258,14 +258,25 @@
 
 
 @pytest.mark.parametrize("precision, cdtype", [(1, np.complex64), (2, complex)])
 def test_dtypes(uvdata, precision, cdtype):
     sky = create_uniform_sky(np.unique(uvdata.freq_array))
     vis = VisCPU(precision=precision)
 
+    # If data_array is empty, then we never create new vis, and the returned value
+    # is literally the data array, so we should expect to get complex128 regardless.
+    sim = VisibilitySimulation(
+        data_model=ModelData(uvdata=uvdata, sky_model=sky), simulator=vis
+    )
+
+    v = sim.simulate()
+    assert v.dtype == complex
+
+    # Now, the uvdata array has stuff in it, so the returned v is a new array that
+    # would have been added to it.
     sim = VisibilitySimulation(
         data_model=ModelData(uvdata=uvdata, sky_model=sky), simulator=vis
     )
 
     v = sim.simulate()
     assert v.dtype == cdtype
 
@@ -352,30 +363,30 @@
         simulator=VisCPU(
             correct_source_positions=True, ref_time="2018-08-31T04:02:30.11"
         ),
     )
 
     # Apply correction
     # viscpu.correct_point_source_pos(obstime="2018-08-31T04:02:30.11", frame="icrs")
-    v = sim.simulate()
+    v = sim.simulate().copy()
     assert np.all(~np.isnan(v))
 
     sim2 = VisibilitySimulation(
         data_model=ModelData(
             uvdata=uvdata2,
             sky_model=zenith_sky_model(uvdata2),
         ),
         simulator=VisCPU(
             correct_source_positions=True,
             ref_time=apt.Time("2018-08-31T04:02:30.11", format="isot", scale="utc"),
         ),
     )
 
     v2 = sim2.simulate()
-    assert np.allclose(v, v2)
+    np.testing.assert_allclose(v, v2)
 
 
 def align_src_to_healpix(ra, dec, nside=2**4):
     """Where the point sources will be placed when converted to healpix model
 
     Parameters
     ----------
@@ -412,24 +423,32 @@
     ],
 )
 def test_comparison(simulator, uvdata2, sky_model, beam_model):
     model_data = ModelData(
         uvdata=uvdata2, sky_model=sky_model(uvdata2), beams=beam_model
     )
 
-    v0 = VisibilitySimulation(
-        data_model=model_data, simulator=SIMULATORS[0](), n_side=2**4
-    ).simulate()
+    v0 = (
+        VisibilitySimulation(
+            data_model=model_data,
+            simulator=SIMULATORS[0](),
+            n_side=2**4,
+        )
+        .simulate()
+        .copy()
+    )
+
+    print(v0[0, 0, 0, 0])
 
     v1 = VisibilitySimulation(
         data_model=model_data, simulator=simulator(), n_side=2**4
     ).simulate()
 
     assert v0.shape == v1.shape
-
+    print(v0[-9:, 0, 0, :], v1[-9:, 0, 0, :])
     np.testing.assert_allclose(v0, v1, rtol=0.05)
 
 
 @pytest.mark.parametrize("simulator", SIMULATORS)
 @pytest.mark.parametrize("order", ["time", "baseline", "ant1", "ant2"])
 @pytest.mark.parametrize("conj", ["ant1<ant2", "ant2<ant1"])
 def test_ordering(uvdata_linear, simulator, order, conj):
```

### Comparing `hera_sim-4.0.0/hera_sim/tests/test_yaml_constructors.py` & `hera_sim-4.1.0/hera_sim/tests/test_yaml_constructors.py`

 * *Files identical despite different names*

### Comparing `hera_sim-4.0.0/hera_sim/utils.py` & `hera_sim-4.1.0/hera_sim/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -677,14 +677,33 @@
         for blnum in group:
             ai, aj = uvutils.baseline_to_antnums(blnum, antenna_numbers.size)
             antpair2angle[(ai, aj)] = angle
             antpair2angle[(aj, ai)] = conj_angle
     return antpair2angle
 
 
+def tanh_window(x, x_min=None, x_max=None, scale_low=1, scale_high=1):
+    if x_min is None and x_max is None:
+        warnings.warn(
+            "Insufficient information provided; you must provide either x_min or "
+            "x_max. Returning uniform window.",
+            stacklevel=1,
+        )
+        return np.ones(x.size)
+
+    window = np.ones(x.size)
+    if x_min is not None:
+        window *= 0.5 * (1 + np.tanh((x - x_min) / scale_low))
+
+    if x_max is not None:
+        window *= 0.5 * (1 + np.tanh((x_max - x) / scale_high))
+
+    return window
+
+
 # Just some numba-fied helpful functions.
 # Note that coverage can't see that these are run without disabling JIT,
 # which kind of defeats the purpose of testing it.
 if HAVE_NUMBA:  # pragma: no cover
 
     @numba.njit
     def jit_reshape_vis(
```

### Comparing `hera_sim-4.0.0/hera_sim/vis.py` & `hera_sim-4.1.0/hera_sim/vis.py`

 * *Files identical despite different names*

### Comparing `hera_sim-4.0.0/hera_sim/visibilities/__init__.py` & `hera_sim-4.1.0/hera_sim/visibilities/__init__.py`

 * *Files identical despite different names*

### Comparing `hera_sim-4.0.0/hera_sim/visibilities/pyuvsim_wrapper.py` & `hera_sim-4.1.0/hera_sim/visibilities/pyuvsim_wrapper.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,24 +11,25 @@
 
     Parameters
     ----------
     quiet
         If True, don't print anything.
     """
 
+    _blt_order_kws = {"order": "time", "minor_order": "baseline"}
+
     _functions_to_profile = (pyuvsim.uvsim.run_uvdata_uvsim,)
 
     def __init__(self, quiet: bool = False):
         self.quiet = quiet
 
     def simulate(self, data_model: ModelData):
         """Simulate the visibilities."""
         beam_dict = {
-            ant: data_model.beam_ids[str(idx)]
-            for idx, ant in enumerate(data_model.uvdata.antenna_names)
+            ant: data_model.beam_ids[ant] for ant in data_model.uvdata.antenna_names
         }
 
         # TODO: this can be removed once
         # https://github.com/RadioAstronomySoftwareGroup/pyuvsim/pull/357
         # is mereged.
         if data_model.sky_model.name is not None:
             data_model.sky_model.name = np.array(data_model.sky_model.name)
```

### Comparing `hera_sim-4.0.0/hera_sim/visibilities/simulators.py` & `hera_sim-4.1.0/hera_sim/visibilities/simulators.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,37 +1,40 @@
 """Module defining a high-level visibility simulator wrapper."""
 from __future__ import annotations
 
 import astropy_healpix as aph
 import importlib
+import logging
 import numpy as np
 import yaml
 from abc import ABCMeta, abstractmethod
 from astropy import units
 from cached_property import cached_property
 from collections.abc import Sequence
 from dataclasses import dataclass
 from os import path
 from pathlib import Path
 from pyradiosky import SkyModel
 from pyuvdata import UVBeam, UVData
 from pyuvsim import BeamList
+from pyuvsim import __version__ as uvsimv
 from pyuvsim import analyticbeam as ab
 from pyuvsim.simsetup import (
     _complete_uvdata,
     initialize_catalog_from_params,
     initialize_uvdata_from_params,
     uvdata_to_telescope_config,
 )
 from typing import Union
 
 from .. import __version__
 from .. import visibilities as vis
 
 BeamListType = Union[BeamList, list[Union[ab.AnalyticBeam, UVBeam]]]
+logger = logging.getLogger(__name__)
 
 
 class ModelData:
     """
     An object containing all the information required to perform visibility simulation.
 
     Parameters
@@ -82,14 +85,15 @@
 
         self.beams = self._process_beams(beams, normalize_beams)
         self.beam_ids = self._process_beam_ids(beam_ids, self.beams)
         self._validate_beam_ids(self.beam_ids, self.beams)
 
         self.sky_model = sky_model
         self.sky_model.at_frequencies(self.freqs * units.Hz)
+
         if not isinstance(self.sky_model, SkyModel):
             raise TypeError("sky_model must be a SkyModel instance.")
 
         self._validate()
 
     def _process_uvdata(self, uvdata: UVData | str | Path):
         if isinstance(uvdata, (str, Path)):
@@ -176,18 +180,34 @@
             )
 
     @classmethod
     def from_config(
         cls, config_file: str | Path, normalize_beams: bool = False
     ) -> ModelData:
         """Initialize the :class:`ModelData` from a pyuvsim-compatible config."""
-        uvdata, beams, beam_ids = initialize_uvdata_from_params(config_file)
-        catalog = initialize_catalog_from_params(config_file, return_recarray=False)[0]
+        # Don't reorder the blt axis, because each simulator might do it differently.
+        logger.info("Initializing UVData object...")
+        uvdata, beams, beam_ids = initialize_uvdata_from_params(
+            config_file,
+            reorder_blt_kw={},
+            check_kw={"run_check_acceptability": False},
+        )
 
-        _complete_uvdata(uvdata, inplace=True)
+        logger.info("Initializing Sky Model...")
+        if uvsimv > "1.2.5":
+            catalog = initialize_catalog_from_params(config_file)[0]
+        else:
+            catalog = initialize_catalog_from_params(
+                config_file, return_recarray=False
+            )[0]
+
+        logger.info("Completing UVData object...")
+        _complete_uvdata(
+            uvdata, inplace=True, check_kw={"run_check_acceptability": False}
+        )
 
         return ModelData(
             uvdata=uvdata,
             beams=beams,
             beam_ids=beam_ids,
             sky_model=catalog,
             normalize_beams=normalize_beams,
@@ -266,15 +286,25 @@
 
     data_model: ModelData
     simulator: VisibilitySimulator
     n_side: int = 2**5
 
     def __post_init__(self):
         """Perform simple validation on combined attributes."""
+        logging.info("blt_order vissim: {data_model.uvdata.blt_order}")
+        if self.simulator._blt_order_kws is not None:
+            logger.info(
+                "Re-ordering baseline-time axis with params: "
+                f"{self.simulator._blt_order_kws}"
+            )
+            self.data_model.uvdata.reorder_blts(**self.simulator._blt_order_kws)
+
+        logger.info("Validating data model")
         self.simulator.validate(self.data_model)
+        logger.info("Done validation.")
 
         # Convert the sky model to either point source or healpix depending on the
         # simulator's capabilities.
         sky_model = self.data_model.sky_model
         if not self.simulator.diffuse_ability and sky_model.component_type == "healpix":
             sky_model.healpix_to_point()
         if (
@@ -325,21 +355,24 @@
         )
         self.uvdata.history += f"Class Repr: {repr(self.simulator)}\n"
         self.uvdata.history += f"hera_sim version: {__version__}"
         self.uvdata.history += f"Simulator Version: {self.simulator.__version__}"
 
     def simulate(self):
         """Perform the visibility simulation."""
-        # Order the baselines/times in the order expected by the simulator.
+        self.simulator.compress_data_model(self.data_model)
         vis = self.simulator.simulate(self.data_model)
-
         self.uvdata.data_array += vis
         self._write_history()
+        self.simulator.restore_data_model(self.data_model)
 
-        return vis
+        if isinstance(vis, np.ndarray):
+            return vis
+        else:
+            return self.uvdata.data_array
 
     @property
     def uvdata(self) -> UVData:
         """A simple view into the UVData object in the :attr:`data_model`."""
         return self.data_model.uvdata
 
 
@@ -375,14 +408,18 @@
     #: Whether this particular simulator has the ability to simulate diffuse
     #: maps directly.
     diffuse_ability = False
 
     #: Any underlying functions that are called and we may want to do profiling on.
     _functions_to_profile = ()
 
+    #: Keyword arguments to use in ordering the baseline-time axis of the incoming
+    #: UVData object, if necessasry. A dict, or None.
+    _blt_order_kws = None
+
     __version__ = "unknown"
 
     @abstractmethod
     def simulate(self, data_model: ModelData) -> np.ndarray:
         """Simulate the visibilities."""
         pass
 
@@ -420,14 +457,25 @@
 
         .. note:: the default method is very much a lower bound -- just the size of the
           output visibilities. Each individual simulator may or may not implement a
           more accurate estimate.
         """
         return data_model.uvdata.data_array.nbytes / 1024**3
 
+    def compress_data_model(self, data_model):  # noqa: B027
+        """Temporarily delete/remove data from the model to reduce memory usage.
+
+        Anything that is removed here should be restored after the simulation.
+        """
+        pass
+
+    def restore_data_model(self, data_model):  # noqa: B027
+        """Restore data from the model removed by :func:`compress_data_model`."""
+        pass
+
 
 def load_simulator_from_yaml(config: Path | str) -> VisibilitySimulator:
     """Construct a visibility simulator from a YAML file."""
     with open(config) as fl:
         cfg = yaml.safe_load(fl)
 
     simulator_cls = cfg.pop("simulator")
```

### Comparing `hera_sim-4.0.0/hera_sim/visibilities/vis_cpu.py` & `hera_sim-4.1.0/hera_sim/visibilities/vis_cpu.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 """Wrapper for vis_cpu visibility simulator."""
 from __future__ import annotations
 
 import astropy.units as u
 import itertools
+import logging
 import numpy as np
 from astropy.coordinates import EarthLocation
 from astropy.time import Time
 from pyuvdata import UVData
 from pyuvdata import utils as uvutils
 
 from vis_cpu import HAVE_GPU, __version__
 from vis_cpu import conversions as convs
 from vis_cpu import vis_cpu, vis_gpu
 from vis_cpu.cpu import _evaluate_beam_cpu, _wrangle_beams
 
 from .simulators import ModelData, VisibilitySimulator
 
+logger = logging.getLogger(__name__)
+
 
 class VisCPU(VisibilitySimulator):
     """
     vis_cpu visibility simulator.
 
     This is a fast, simple visibility simulator that is intended to be
     replaced by vis_gpu.
@@ -52,14 +55,18 @@
         astropy. For best fidelity, set this to a mid-point of your observation times.
         If specified as a string, this must either use the 'isot' format and 'utc'
         scale, or be one of "mean", "min" or "max". If any of the latter, the value
         ll be calculated from the input data directly.
     correct_source_positions
         Whether to correct the source positions using astropy and the reference time.
         Default is True if `ref_time` is given otherwise False.
+    check_antenna_conjugation
+        Whether to check the antenna conjugation. Default is True. This is a fairly
+        heavy operation if there are many antennas and/or many times, and can be
+        safely ignored if the data_model was created from a config file.
     **kwargs
         Passed through to :class:`~.simulators.VisibilitySimulator`.
 
     """
 
     conjugation_convention = "ant1<ant2"
     time_ordering = "time"
@@ -70,14 +77,16 @@
     def __init__(
         self,
         precision: int = 1,
         use_gpu: bool = False,
         mpi_comm=None,
         ref_time: str | Time | None = None,
         correct_source_positions: bool | None = None,
+        check_antenna_conjugation: bool = True,
+        **kwargs,
     ):
         assert precision in {1, 2}
         self._precision = precision
         if precision == 1:
             self._real_dtype = np.float32
             self._complex_dtype = np.complex64
         else:
@@ -98,41 +107,47 @@
         self.mpi_comm = mpi_comm
         self.ref_time = ref_time
         self.correct_source_positions = (
             (ref_time is not None)
             if correct_source_positions is None
             else correct_source_positions
         )
-
+        self.check_antenna_conjugation = check_antenna_conjugation
         self._functions_to_profile = (self._vis_cpu, _wrangle_beams, _evaluate_beam_cpu)
+        self.kwargs = kwargs
 
     def validate(self, data_model: ModelData):
         """Checks for correct input format."""
         # N(N-1)/2 unique cross-correlations + N autocorrelations.
         if data_model.uvdata.Nbls != data_model.n_ant * (data_model.n_ant + 1) / 2:
             raise ValueError(
                 "VisCPU requires using every pair of antennas, "
                 "but the UVData object does not comply."
             )
 
+        logger.info("Checking baseline-time axis shape")
         if len(data_model.uvdata.data_array) != len(
             data_model.uvdata.get_antpairs()
         ) * len(data_model.lsts):
             raise ValueError("VisCPU requires that every baseline uses the same LSTS.")
 
-        if any(
-            len(data_model.uvdata.antpair2ind(ai, aj)) > 0
-            and len(data_model.uvdata.antpair2ind(aj, ai)) > 0
-            for ai, aj in data_model.uvdata.get_antpairs()
-            if ai != aj
-        ):
-            raise ValueError(
-                "VisCPU requires that baselines be in a conjugation in which antenna "
-                "order doesn't change with time!"
-            )
+        if self.check_antenna_conjugation:
+            logger.info("Checking antenna conjugation")
+            # TODO: the following is extremely slow. If possible, it would be good to
+            # find a better way to do it.
+            if any(
+                len(data_model.uvdata.antpair2ind(ai, aj)) > 0
+                and len(data_model.uvdata.antpair2ind(aj, ai)) > 0
+                for ai, aj in data_model.uvdata.get_antpairs()
+                if ai != aj
+            ):
+                raise ValueError(
+                    "VisCPU requires that baselines be in a conjugation in which "
+                    "antenna order doesn't change with time!"
+                )
 
         uvbeam = data_model.beams[0]  # Representative beam
         uvdata = data_model.uvdata
 
         # Now check that we only have linear polarizations (don't allow pseudo-stokes)
         if any(pol not in [-5, -6, -7, -8] for pol in uvdata.polarization_array):
             raise ValueError(
@@ -144,15 +159,15 @@
                 """
             )
 
         do_pol = self._check_if_polarized(data_model)
         if do_pol:
             # Number of feeds must be two if doing polarized
             try:
-                nfeeds = uvbeam.data_array.shape[2]
+                nfeeds = uvbeam.data_array.shape[1 if uvbeam.future_array_shapes else 2]
             except AttributeError:
                 # TODO: the following assumes that analytic beams are 2 feeds unless
                 # otherwise specified. This should be fixed at the AnalyticBeam API
                 # level.
                 nfeeds = getattr(uvbeam, "Nfeeds", 2)
 
             assert nfeeds == 2
@@ -249,14 +264,15 @@
         # Get reference location
         # location = EarthLocation.from_geodetic(lat=lat, lon=lon, height=alt)
         location = EarthLocation.from_geocentric(
             *data_model.uvdata.telescope_location, unit=u.m
         )
 
         # Apply correction to point source positions
+        logger.info("Correcting Source Positions...")
         ra, dec = data_model.sky_model.ra, data_model.sky_model.dec
         return convs.equatorial_to_eci_coords(
             ra, dec, obstime, location, unit="rad", frame=frame
         )
 
     def _check_if_polarized(self, data_model: ModelData) -> bool:
         p = data_model.uvdata.polarization_array
@@ -302,32 +318,32 @@
 
         # Setup MPI info if enabled
         if self.mpi_comm is not None:
             myid = self.mpi_comm.Get_rank()
             nproc = self.mpi_comm.Get_size()
 
         if self.correct_source_positions:
-            # TODO: check if this is the right time to be using...
-            ra, dec = self.correct_point_source_pos(
-                data_model, obstime=Time(data_model.uvdata.time_array[0], format="jd")
-            )
+            ra, dec = self.correct_point_source_pos(data_model)
+            logger.info("Done correcting source positions.")
         else:
             ra, dec = data_model.sky_model.ra, data_model.sky_model.dec
 
+        logger.info("Getting Equatorial Coordinates")
         crd_eq = convs.point_source_crd_eq(ra, dec)
 
         # Convert equatorial to topocentric coords
+        logger.info("Getting Rotation Matrices")
         eq2tops = self.get_eq2tops(data_model.uvdata, data_model.lsts)
 
         # The following are antenna positions in the order that they are
         # in the uvdata.data_array
         active_antpos, ant_list = data_model.uvdata.get_ENU_antpos(pick_data_ants=True)
 
         # Get pixelized beams if required
-
+        logger.info("Preparing Beams...")
         beam_list = [
             convs.prepare_beam(
                 beam,
                 polarized=polarized,
                 use_feed=feed,
             )
             for beam in data_model.beams
@@ -344,64 +360,114 @@
 
         # Get all the polarizations required to be simulated.
         req_pols = self._get_req_pols(
             data_model.uvdata, data_model.beams[0], polarized=polarized
         )
 
         # Empty visibility array
-        visfull = np.zeros_like(data_model.uvdata.data_array, dtype=self._complex_dtype)
+        if np.all(data_model.uvdata.data_array == 0):
+            # Here, we don't make new memory, because that is just a whole extra copy
+            # of the largest array in the calculation. Instead we fill the data_array
+            # directly.
+            visfull = data_model.uvdata.data_array
+        else:
+            visfull = np.zeros_like(
+                data_model.uvdata.data_array, dtype=self._complex_dtype
+            )
 
         for i, freq in enumerate(data_model.freqs):
             # Divide tasks between MPI workers if needed
             if self.mpi_comm is not None and i % nproc != myid:
                 continue
 
+            logger.info(f"Simulating Frequency {i+1}/{len(data_model.freqs)}")
+
             # Call vis_cpu function to simulate visibilities
             vis = self._vis_cpu(
                 antpos=active_antpos,
                 freq=freq,
                 eq2tops=eq2tops,
                 crd_eq=crd_eq,
                 I_sky=data_model.sky_model.stokes[0, i].to("Jy").value,
                 beam_list=beam_list,
                 beam_idx=beam_ids,
+                beam_spline_opts=data_model.beams.spline_interp_opts,
                 precision=self._precision,
                 polarized=polarized,
+                **self.kwargs,
             )
 
+            logger.info("... re-ordering visibilities...")
             self._reorder_vis(
                 req_pols, data_model.uvdata, visfull[:, 0, i], vis, ant_list, polarized
             )
 
         # Reduce visfull array if in MPI mode
         if self.mpi_comm is not None:
             visfull = self._reduce_mpi(visfull, myid)
 
-        return visfull
+        if visfull is data_model.uvdata.data_array:
+            # In the case that we were just fulling up the data array the whole time,
+            # we return zero, because this will be added to the data_array in the
+            # wrapper simulate() function.
+            return 0
+        else:
+            return visfull
 
     def _reorder_vis(self, req_pols, uvdata, visfull, vis, ant_list, polarized):
-        indices = np.triu_indices(vis.shape[-1])
+        ant1idx, ant2idx = np.triu_indices(vis.shape[-1])
 
-        for p, (p1, p2) in enumerate(req_pols):
-            for ant1, ant2 in zip(*indices):  # go through indices in output
-                vis_here = (
-                    vis[:, p1, p2, ant1, ant2] if polarized else vis[:, ant1, ant2]
-                )
-                # get official "antenna numbers" corresponding to these indices
-                antnum1, antnum2 = ant_list[ant1], ant_list[ant2]
+        try:
+            if (
+                getattr(uvdata, "blt_order", None) == ("time", "ant1")
+                and sorted(req_pols) == req_pols
+            ):
+                logger.info("Using direct setting of data without reordering")
+                # This is the best case scenario -- no need to reorder anything.
+                # It is also MUCH MUCH faster!
+                start_shape = visfull.shape
+                visfull.shape = (np.prod(visfull.shape),)  # flatten without copying
+                n = (uvdata.Nblts // vis.shape[0]) * len(req_pols)
+                for i, vis_here in enumerate(vis):
+                    if polarized:
+                        vis_here = vis_here.transpose(2, 3, 0, 1)[
+                            ant1idx, ant2idx
+                        ].reshape((-1,))
+                    else:
+                        vis_here = vis_here[:, ant1idx, ant2idx].reshape((-1,))
+
+                    visfull[(i * n) : ((i + 1) * n)] = vis_here
+                visfull.shape = start_shape
+                return
+        except AttributeError:
+            pass
 
-                # get all blt indices corresponding to this antpair
-                indx = uvdata.antpair2ind(antnum1, antnum2)
-                if len(indx) == 0:
-                    # maybe we chose the wrong ordering according to the data. Then
-                    # we just conjugate.
-                    indx = uvdata.antpair2ind(antnum2, antnum1)
-                    vis_here = np.conj(vis_here)
+        logger.info(
+            f"Reordering baselines. Pols sorted: {sorted(req_pols) == req_pols}. "
+            f"Pols = {req_pols}. blt_order = {uvdata.blt_order}"
+        )
+        for ant1, ant2 in zip(ant1idx, ant2idx):  # go through indices in output
+            # get official "antenna numbers" corresponding to these indices
+            antnum1, antnum2 = ant_list[ant1], ant_list[ant2]
+
+            # get all blt indices corresponding to this antpair
+            indx = uvdata.antpair2ind(antnum1, antnum2)
+            if len(indx) == 0:
+                # maybe we chose the wrong ordering according to the data. Then
+                # we just conjugate.
+                indx = uvdata.antpair2ind(antnum2, antnum1)
+                vis_here = vis[..., ant2, ant1]
+            else:
+                vis_here = vis[..., ant1, ant2]
 
-                visfull[indx, p] = vis_here
+            if polarized:
+                for p, (p1, p2) in enumerate(req_pols):
+                    visfull[indx, p] = vis_here[:, p1, p2]
+            else:
+                visfull[indx, 0] = vis_here
 
     def _get_req_pols(self, uvdata, uvbeam, polarized: bool) -> list[tuple[int, int]]:
         if not polarized:
             return [(0, 0)]
 
         # TODO: this can be updated to just access uvbeam.feed_array once the
         # AnalyticBeam API has been improved.
@@ -435,7 +501,19 @@
 
         _visfull = np.zeros(visfull.shape, dtype=visfull.dtype)
         self.mpi_comm.Reduce(visfull, _visfull, op=SUM, root=0)
         if myid == 0:
             return _visfull
         else:
             return 0  # workers return 0
+
+    def compress_data_model(self, data_model: ModelData):
+        data_model.uvdata.uvw_array = 0
+        # data_model.uvdata.baseline_array = 0
+        data_model.uvdata.integration_time = data_model.uvdata.integration_time.item(0)
+
+    def restore_data_model(self, data_model: ModelData):
+        uv_obj = data_model.uvdata
+        uv_obj.integration_time = np.repeat(
+            uv_obj.integration_time, uv_obj.Nbls * uv_obj.Ntimes
+        )
+        uv_obj.set_uvws_from_antenna_positions()
```

### Comparing `hera_sim-4.0.0/hera_sim.egg-info/PKG-INFO` & `hera_sim-4.1.0/hera_sim.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hera-sim
-Version: 4.0.0
+Version: 4.1.0
 Summary: A collection of simulation routines describing the HERA instrument.
 Home-page: https://github.com/HERA-Team/hera_sim
 Author: HERA Team
 Author-email: steven.g.murray@asu.edu
 License: MIT
 Project-URL: Documentation, https://hera_sim.readthedocs.org
 Platform: any
```

### Comparing `hera_sim-4.0.0/hera_sim.egg-info/SOURCES.txt` & `hera_sim-4.1.0/hera_sim.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -65,20 +65,25 @@
 hera_sim.egg-info/top_level.txt
 hera_sim/config/H1C.yaml
 hera_sim/config/H2C.yaml
 hera_sim/config/__init__.py
 hera_sim/config/debug.yaml
 hera_sim/data/H37_FR_Filters_small.npz
 hera_sim/data/HERA_H1C_BANDPASS.npy
+hera_sim/data/HERA_H1C_BEAM_INTEGRALS.npz
 hera_sim/data/HERA_H1C_BEAM_POLY.npy
+hera_sim/data/HERA_H1C_REFLECTIONS.npz
 hera_sim/data/HERA_H1C_RFI_STATIONS.npy
 hera_sim/data/HERA_H2C_BANDPASS.npy
 hera_sim/data/HERA_H2C_BEAM_MODEL.npz
 hera_sim/data/HERA_H2C_BEAM_POLY.npy
 hera_sim/data/HERA_H2C_RFI_STATIONS.npy
+hera_sim/data/HERA_H4C_BANDPASS.npz
+hera_sim/data/HERA_H4C_BEAM_INTEGRALS.npz
+hera_sim/data/HERA_H4C_REFLECTIONS.npz
 hera_sim/data/HERA_LAT_LON_ALT.npy
 hera_sim/data/HERA_Tsky_Reformatted.npz
 hera_sim/data/HERA_Tsky_vs_LST.npz
 hera_sim/data/tutorials_data/end_to_end/array_layout.csv
 hera_sim/data/tutorials_data/end_to_end/make_mock_catalog.py
 hera_sim/data/tutorials_data/end_to_end/obsparams.yaml
 hera_sim/data/tutorials_data/end_to_end/sample_catalog.txt
@@ -103,15 +108,23 @@
 hera_sim/tests/test_rfi.py
 hera_sim/tests/test_sigchain.py
 hera_sim/tests/test_sim_red_data.py
 hera_sim/tests/test_simulate_cli.py
 hera_sim/tests/test_simulator.py
 hera_sim/tests/test_utils.py
 hera_sim/tests/test_vis.py
+hera_sim/tests/test_vis_cli.py
 hera_sim/tests/test_yaml_constructors.py
 hera_sim/tests/testdata/healvis_catalog.txt
+hera_sim/tests/testdata/hera-sim-vis-config/H4C-antennas-slim.csv
+hera_sim/tests/testdata/hera-sim-vis-config/NF_HERA_Dipole_small.fits
+hera_sim/tests/testdata/hera-sim-vis-config/gleam_50srcs.vot
+hera_sim/tests/testdata/hera-sim-vis-config/h4c_idr2.1_teleconfig.yaml
+hera_sim/tests/testdata/hera-sim-vis-config/viscpu.yaml
+hera_sim/tests/testdata/hera-sim-vis-config/visgpu.yaml
 hera_sim/visibilities/__init__.py
+hera_sim/visibilities/cli.py
 hera_sim/visibilities/pyuvsim_wrapper.py
 hera_sim/visibilities/simulators.py
 hera_sim/visibilities/vis_cpu.py
 scripts/hera-sim-simulate.py
 scripts/hera-sim-vis.py
```

### Comparing `hera_sim-4.0.0/scripts/hera-sim-simulate.py` & `hera_sim-4.1.0/scripts/hera-sim-simulate.py`

 * *Files identical despite different names*

### Comparing `hera_sim-4.0.0/setup.cfg` & `hera_sim-4.1.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 description = A collection of simulation routines describing the HERA instrument.
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 url = https://github.com/HERA-Team/hera_sim
 author = HERA Team
 author_email = steven.g.murray@asu.edu
 license = MIT
-license_file = LICENSE.rst
+license_files = LICENSE.rst
 platforms = any
 classifiers = 
 	Development Status :: 4 - Beta
 	Intended Audience :: Science/Research
 	License :: OSI Approved
 	License :: OSI Approved :: MIT License
 	Natural Language :: English
@@ -25,16 +25,17 @@
 [options]
 packages = find:
 install_requires = 
 	astropy
 	astropy-healpix
 	cached-property
 	deprecation
+	hera-cli-utils>=0.1.0
 	numpy>=1.18
-	pyuvdata
+	pyuvdata>=2.2.12
 	pyuvsim>=1.2.5
 	pyyaml>=5.1
 	rich
 	scipy
 python_requires = >=3.9
 include_package_data = True
 scripts = 
@@ -73,14 +74,15 @@
 	hera-sim[bda,cal,vis]
 	matplotlib>=3.4.2
 	pre-commit
 	pytest>=3.5.1
 	pytest-cov>=2.5.1
 	uvtools
 vis = 
+	line-profiler
 	mpi4py
 	pyradiosky>=0.1.2
 	vis-cpu>=1.1.0
 
 [tool:pytest]
 addopts = 
 	--cov hera_sim
```

