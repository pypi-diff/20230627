# Comparing `tmp/snudda-1.4.4.tar.gz` & `tmp/snudda-1.4.71.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snudda-1.4.4.tar", last modified: Wed Apr 26 08:34:26 2023, max compression
+gzip compressed data, was "snudda-1.4.71.tar", last modified: Tue Jun 27 13:27:26 2023, max compression
```

## Comparing `snudda-1.4.4.tar` & `snudda-1.4.71.tar`

### file list

```diff
@@ -1,483 +1,492 @@
-drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-04-26 08:34:26.348803 snudda-1.4.4/
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    35149 2022-09-19 09:45:08.000000 snudda-1.4.4/LICENSE
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     4188 2023-04-26 08:34:26.348803 snudda-1.4.4/PKG-INFO
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3711 2022-09-19 09:45:08.000000 snudda-1.4.4/README.md
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)       38 2023-04-26 08:34:26.348803 snudda-1.4.4/setup.cfg
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2677 2023-04-26 08:33:58.000000 snudda-1.4.4/setup.py
-drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-04-26 08:34:26.252802 snudda-1.4.4/snudda/
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)      506 2023-04-26 08:33:58.000000 snudda-1.4.4/snudda/__init__.py
-drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-04-26 08:34:26.256802 snudda-1.4.4/snudda/analyse/
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)      199 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/analyse/__init__.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)   107778 2023-04-26 08:33:58.000000 snudda-1.4.4/snudda/analyse/analyse.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     7923 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/analyse/analyse_gap_junction_coupling.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3251 2023-02-15 16:15:38.000000 snudda-1.4.4/snudda/analyse/analyse_input.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     5575 2022-11-03 09:16:18.000000 snudda-1.4.4/snudda/analyse/analyse_neuroinformatics2020.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     8650 2023-04-26 08:33:58.000000 snudda-1.4.4/snudda/analyse/analyse_spike_trains.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    18255 2022-11-03 09:16:18.000000 snudda-1.4.4/snudda/analyse/analyse_striatum.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2996 2023-04-26 08:33:58.000000 snudda-1.4.4/snudda/analyse/analyse_synapse_location.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     7574 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/analyse/analyse_topology.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    12378 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/analyse/analyse_topology_activity.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     6277 2023-04-26 08:33:58.000000 snudda-1.4.4/snudda/analyse/spike_time_tiling_coefficient.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    11585 2023-04-26 08:33:58.000000 snudda-1.4.4/snudda/cli.py
--rwxr-xr-x   0 hjorth    (1001) hjorth    (1001)    29470 2023-04-26 08:33:58.000000 snudda-1.4.4/snudda/core.py
-drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-04-26 08:34:26.252802 snudda-1.4.4/snudda/data/
-drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-04-26 08:34:26.252802 snudda-1.4.4/snudda/data/InputAxons/
-drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-04-26 08:34:26.256802 snudda-1.4.4/snudda/data/InputAxons/Cortex/
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)   432939 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/InputAxons/Cortex/AA0059.swc
-drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-04-26 08:34:26.256802 snudda-1.4.4/snudda/data/InputAxons/Cortex/Reg10/
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)   900524 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/InputAxons/Cortex/Reg10/AA0059-reg10.swc
-drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-04-26 08:34:26.260803 snudda-1.4.4/snudda/data/InputAxons/Cortex/Reg15/
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)   597398 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/InputAxons/Cortex/Reg15/AA0059-reg15.swc
-drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-04-26 08:34:26.260803 snudda-1.4.4/snudda/data/InputAxons/Cortex/Reg5/
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)  1809577 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/InputAxons/Cortex/Reg5/AA0059-reg5.swc
-drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-04-26 08:34:26.264803 snudda-1.4.4/snudda/data/InputAxons/GPe2Striatum/
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1269 2023-04-26 08:33:58.000000 snudda-1.4.4/snudda/data/InputAxons/GPe2Striatum/example-projection-config.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)   444324 2023-02-15 16:15:38.000000 snudda-1.4.4/snudda/data/InputAxons/GPe2Striatum/prototypical-axon.swc
-drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-04-26 08:34:26.264803 snudda-1.4.4/snudda/data/InputAxons/Thalamus/
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)   464916 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/InputAxons/Thalamus/AA0054.swc
-drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-04-26 08:34:26.264803 snudda-1.4.4/snudda/data/InputAxons/Thalamus/Reg10/
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)   513478 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/InputAxons/Thalamus/Reg10/AA0054-reg10.swc
-drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-04-26 08:34:26.264803 snudda-1.4.4/snudda/data/InputAxons/Thalamus/Reg15/
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)   346069 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/InputAxons/Thalamus/Reg15/AA0054-reg15.swc
-drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-04-26 08:34:26.264803 snudda-1.4.4/snudda/data/InputAxons/Thalamus/Reg5/
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)  1022637 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/InputAxons/Thalamus/Reg5/AA0054-reg5.swc
-drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-04-26 08:34:26.272802 snudda-1.4.4/snudda/data/density/
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    87096 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/density/1001_STRd_Sst_dens.csv
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    89256 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/density/1001_STRd_Sst_dens_smooth.csv
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    74510 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/density/252_STRd_Chat_dens.csv
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    77158 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/density/252_STRd_Chat_dens_smooth.csv
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    94468 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/density/352_STRd_Drd1_dens.csv
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    95346 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/density/352_STRd_Drd1_dens_smooth.csv
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    95932 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/density/72109410_STRd_Adora2a_dens.csv
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    96454 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/density/72109410_STRd_Adora2a_dens_smooth.csv
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    77578 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/density/79556738_STRd_Pvalb_dens.csv
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    79756 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/density/79556738_STRd_Pvalb_dens_smooth.csv
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1132 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/density/combine_densities.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)  2256264 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/density/dorsal_striatum_density.json
-drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-04-26 08:34:26.252802 snudda-1.4.4/snudda/data/experiment_config/
-drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-04-26 08:34:26.276803 snudda-1.4.4/snudda/data/experiment_config/pair_recording/
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)      469 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/experiment_config/pair_recording/experiment-config-1.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)      583 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/experiment_config/pair_recording/experiment-config-2.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)      635 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/experiment_config/pair_recording/experiment-config-3.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)      636 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/experiment_config/pair_recording/experiment-config-4.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)      455 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/experiment_config/pair_recording/experiment-config-5.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)      595 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/experiment_config/pair_recording/experiment-config-6.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)      693 2022-11-11 14:42:41.000000 snudda-1.4.4/snudda/data/experiment_config/pair_recording/experiment-config-7.json
-drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-04-26 08:34:26.276803 snudda-1.4.4/snudda/data/images/
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    52659 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/images/snudda-video-qr-code.png
-drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-04-26 08:34:26.276803 snudda-1.4.4/snudda/data/input_config/
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     5834 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/input_config/external-input-dSTR-scaled-v2.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     5827 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/input_config/external-input-dSTR-scaled-v3.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     5827 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/input_config/external-input-dSTR-scaled-v3b.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     5834 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/input_config/external-input-dSTR-scaled-v4-cluster-test.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     5811 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/input_config/external-input-dSTR-scaled-v4.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     5843 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/input_config/external-input-dSTR-scaled.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)      768 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/input_config/input-tinytest-ChIN.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1831 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/input_config/input-tinytest-Channel-Activation.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1803 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/input_config/input-tinytest-channel-1.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1803 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/input_config/input-tinytest-channel-2.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     5395 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/input_config/input-tinytest-v7.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     5409 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/input_config/input-tinytest-v8.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     5547 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/input_config/input-tinytest-v9-freq-vectors.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     5639 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/input_config/input-v10-scaled.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)      506 2023-04-26 08:33:58.000000 snudda-1.4.4/snudda/data/input_config/input_output_dspn_template_IC.json
-drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-04-26 08:34:26.284803 snudda-1.4.4/snudda/data/mesh/
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)   192511 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/mesh/GPe.obj
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    60912 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/mesh/GPi.obj
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    68536 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/mesh/SNc.obj
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)   164445 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/mesh/SNr.obj
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    44005 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/mesh/STN.obj
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)  1069021 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/mesh/Striatum-d.obj
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)  1733004 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/mesh/Striatum-dorsal-left-hemisphere.obj
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)  1813629 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/mesh/Striatum-dorsal-right-hemisphere.obj
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)   763087 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/mesh/Striatum-v.obj
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2358 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/mesh/get_mesh.ipynb
-drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-04-26 08:34:26.252802 snudda-1.4.4/snudda/data/nest/
-drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-04-26 08:34:26.284803 snudda-1.4.4/snudda/data/nest/models/
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)      272 2023-04-26 08:33:58.000000 snudda-1.4.4/snudda/data/nest/models/FS.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)      278 2023-04-26 08:33:58.000000 snudda-1.4.4/snudda/data/nest/models/dSPN.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)      276 2023-04-26 08:33:58.000000 snudda-1.4.4/snudda/data/nest/models/iSPN.json
-drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-04-26 08:34:26.252802 snudda-1.4.4/snudda/data/neurons/
-drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-04-26 08:34:26.288802 snudda-1.4.4/snudda/data/neurons/mechanisms/
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2111 2023-04-26 08:33:58.000000 snudda-1.4.4/snudda/data/neurons/mechanisms/Im_ms.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1352 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/mechanisms/Kv3_ch.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1375 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/mechanisms/NO.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2598 2023-04-26 08:33:58.000000 snudda-1.4.4/snudda/data/neurons/mechanisms/bk_ch.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2511 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/mechanisms/bk_fs.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2744 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/mechanisms/bk_ms.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     4351 2023-04-26 08:33:58.000000 snudda-1.4.4/snudda/data/neurons/mechanisms/ca_ch.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1282 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/mechanisms/cadyn_fs.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1609 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/mechanisms/cadyn_ms.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     4561 2023-04-26 08:33:58.000000 snudda-1.4.4/snudda/data/neurons/mechanisms/cal12_ms.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     4723 2023-04-26 08:33:58.000000 snudda-1.4.4/snudda/data/neurons/mechanisms/cal13_ms.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2871 2023-04-26 08:33:58.000000 snudda-1.4.4/snudda/data/neurons/mechanisms/cal_ch.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1663 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/mechanisms/caldyn_ms.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3256 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/mechanisms/can_fs.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     4517 2023-04-26 08:33:58.000000 snudda-1.4.4/snudda/data/neurons/mechanisms/can_ms.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2986 2023-04-26 08:33:58.000000 snudda-1.4.4/snudda/data/neurons/mechanisms/cap_ch.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2424 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/mechanisms/caq_fs.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2485 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/mechanisms/caq_ms.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2814 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/mechanisms/car_fs.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3855 2023-04-26 08:33:58.000000 snudda-1.4.4/snudda/data/neurons/mechanisms/car_ms.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2413 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/mechanisms/cat32_ms.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2414 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/mechanisms/cat33_ms.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1074 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/mechanisms/concACh.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1084 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/mechanisms/concDA.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)      907 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/mechanisms/concDAfile.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3903 2023-04-26 08:33:58.000000 snudda-1.4.4/snudda/data/neurons/mechanisms/hcn12_ch.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2247 2023-04-26 08:33:58.000000 snudda-1.4.4/snudda/data/neurons/mechanisms/hd_lts.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3028 2023-04-26 08:33:58.000000 snudda-1.4.4/snudda/data/neurons/mechanisms/im_lts.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3099 2023-04-26 08:33:58.000000 snudda-1.4.4/snudda/data/neurons/mechanisms/it_lts.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3406 2023-04-26 08:33:58.000000 snudda-1.4.4/snudda/data/neurons/mechanisms/kaf_fs.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3407 2023-04-26 08:33:58.000000 snudda-1.4.4/snudda/data/neurons/mechanisms/kaf_lts.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     4335 2023-04-26 08:33:58.000000 snudda-1.4.4/snudda/data/neurons/mechanisms/kaf_ms.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3334 2023-04-26 08:33:58.000000 snudda-1.4.4/snudda/data/neurons/mechanisms/kas_fs.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3932 2023-04-26 08:33:58.000000 snudda-1.4.4/snudda/data/neurons/mechanisms/kas_ms.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1189 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/mechanisms/kcnq_ch.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1179 2023-04-26 08:33:58.000000 snudda-1.4.4/snudda/data/neurons/mechanisms/kdb_lts.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1781 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/mechanisms/kdr_fs.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2810 2023-04-26 08:33:58.000000 snudda-1.4.4/snudda/data/neurons/mechanisms/kdr_lts.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1725 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/mechanisms/kdr_ms.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1230 2023-04-26 08:33:58.000000 snudda-1.4.4/snudda/data/neurons/mechanisms/kdrb_lts.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3594 2023-04-26 08:33:58.000000 snudda-1.4.4/snudda/data/neurons/mechanisms/kir23_ch.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3595 2023-04-26 08:33:58.000000 snudda-1.4.4/snudda/data/neurons/mechanisms/kir23_lts.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1665 2023-04-26 08:33:58.000000 snudda-1.4.4/snudda/data/neurons/mechanisms/kir2_ch.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3586 2023-04-26 08:33:58.000000 snudda-1.4.4/snudda/data/neurons/mechanisms/kir_fs.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     4151 2023-04-26 08:33:58.000000 snudda-1.4.4/snudda/data/neurons/mechanisms/kir_ms.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1254 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/mechanisms/kv2_ch.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2679 2023-04-26 08:33:58.000000 snudda-1.4.4/snudda/data/neurons/mechanisms/kv4_ch.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3111 2023-04-26 08:33:58.000000 snudda-1.4.4/snudda/data/neurons/mechanisms/na2_ch.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3677 2023-04-26 08:33:58.000000 snudda-1.4.4/snudda/data/neurons/mechanisms/na3_lts.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3119 2023-04-26 08:33:58.000000 snudda-1.4.4/snudda/data/neurons/mechanisms/na_ch.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2833 2023-04-26 08:33:58.000000 snudda-1.4.4/snudda/data/neurons/mechanisms/naf_fs.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3043 2023-04-26 08:33:58.000000 snudda-1.4.4/snudda/data/neurons/mechanisms/naf_lts.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3245 2023-04-26 08:33:58.000000 snudda-1.4.4/snudda/data/neurons/mechanisms/naf_ms.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)      377 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/mechanisms/par_ggap.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1909 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/mechanisms/sk_ch.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1896 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/mechanisms/sk_fs.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1896 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/mechanisms/sk_ms.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2370 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/mechanisms/tmampa.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     4291 2023-04-26 08:33:58.000000 snudda-1.4.4/snudda/data/neurons/mechanisms/tmgabaa.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     7671 2023-04-26 08:33:58.000000 snudda-1.4.4/snudda/data/neurons/mechanisms/tmglut.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     7535 2023-04-26 08:33:58.000000 snudda-1.4.4/snudda/data/neurons/mechanisms/tmglut_M1RH_D1.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     8029 2023-04-26 08:33:58.000000 snudda-1.4.4/snudda/data/neurons/mechanisms/tmglut_double.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1336 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/mechanisms/tmnmda.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1026 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/mechanisms/vecevent.mod
-drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-04-26 08:34:26.296803 snudda-1.4.4/snudda/data/neurons/mechanisms.OLD/
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1352 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/mechanisms.OLD/Kv3_ch.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2225 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/mechanisms.OLD/bk_ch.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2511 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/mechanisms.OLD/bk_fs.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2744 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/mechanisms.OLD/bk_ms.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3998 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/mechanisms.OLD/ca_ch.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1282 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/mechanisms.OLD/cadyn_fs.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1609 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/mechanisms.OLD/cadyn_ms.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3249 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/mechanisms.OLD/cal12_ms.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3452 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/mechanisms.OLD/cal13_ms.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1800 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/mechanisms.OLD/cal_ch.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1663 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/mechanisms.OLD/caldyn_ms.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3256 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/mechanisms.OLD/can_fs.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3256 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/mechanisms.OLD/can_ms.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1686 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/mechanisms.OLD/cap_ch.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2424 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/mechanisms.OLD/caq_fs.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2485 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/mechanisms.OLD/caq_ms.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2814 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/mechanisms.OLD/car_fs.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2814 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/mechanisms.OLD/car_ms.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2413 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/mechanisms.OLD/cat32_ms.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2414 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/mechanisms.OLD/cat33_ms.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1164 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/mechanisms.OLD/h_lts.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2855 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/mechanisms.OLD/hcn12_ch.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1724 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/mechanisms.OLD/im_lts.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2061 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/mechanisms.OLD/it_lts.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2364 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/mechanisms.OLD/kaf_fs.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2993 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/mechanisms.OLD/kaf_ms.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2292 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/mechanisms.OLD/kas_fs.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2886 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/mechanisms.OLD/kas_ms.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1189 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/mechanisms.OLD/kcnq_ch.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1781 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/mechanisms.OLD/kdr_fs.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1725 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/mechanisms.OLD/kdr_ms.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1250 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/mechanisms.OLD/kdrbca1_lts.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)      605 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/mechanisms.OLD/kir2_ch.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2543 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/mechanisms.OLD/kir_fs.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2882 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/mechanisms.OLD/kir_ms.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1254 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/mechanisms.OLD/kv2_ch.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1642 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/mechanisms.OLD/kv4_ch.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2082 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/mechanisms.OLD/na2_ch.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2637 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/mechanisms.OLD/na3n_lts.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2076 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/mechanisms.OLD/na_ch.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1791 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/mechanisms.OLD/naf_fs.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1980 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/mechanisms.OLD/naf_ms.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)      377 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/mechanisms.OLD/par_ggap.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1909 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/mechanisms.OLD/sk_ch.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1896 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/mechanisms.OLD/sk_fs.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1896 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/mechanisms.OLD/sk_ms.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2370 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/mechanisms.OLD/tmampa.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2893 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/mechanisms.OLD/tmgabaa.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     5773 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/mechanisms.OLD/tmglut.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1336 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/mechanisms.OLD/tmnmda.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1026 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/mechanisms.OLD/vecevent.mod
-drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-04-26 08:34:26.252802 snudda-1.4.4/snudda/data/neurons/striatum/
-drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-04-26 08:34:26.252802 snudda-1.4.4/snudda/data/neurons/striatum/chin/
-drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-04-26 08:34:26.296803 snudda-1.4.4/snudda/data/neurons/striatum/chin/str-chin-e170614_cell6-m17JUL301751_170614_no6_MD_cell_1_x63-v20190710/
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)      215 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/striatum/chin/str-chin-e170614_cell6-m17JUL301751_170614_no6_MD_cell_1_x63-v20190710/mechanisms.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    89390 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/striatum/chin/str-chin-e170614_cell6-m17JUL301751_170614_no6_MD_cell_1_x63-v20190710/modulation.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    69404 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/striatum/chin/str-chin-e170614_cell6-m17JUL301751_170614_no6_MD_cell_1_x63-v20190710/optim_chin_morph_renamed2019-11-08.swc
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3194 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/striatum/chin/str-chin-e170614_cell6-m17JUL301751_170614_no6_MD_cell_1_x63-v20190710/parameters.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)      403 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/striatum/chin/str-chin-e170614_cell6-m17JUL301751_170614_no6_MD_cell_1_x63-v20190710/protocols.json
-drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-04-26 08:34:26.252802 snudda-1.4.4/snudda/data/neurons/striatum/dspn/
-drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-04-26 08:34:26.300803 snudda-1.4.4/snudda/data/neurons/striatum/dspn/str-dspn-e150602_c1_D1-mWT-0728MSN01-v20190508/
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)   673225 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/striatum/dspn/str-dspn-e150602_c1_D1-mWT-0728MSN01-v20190508/WT-0728MSN01-cor-rep-ax.swc
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)      936 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/striatum/dspn/str-dspn-e150602_c1_D1-mWT-0728MSN01-v20190508/fix_indexing.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)      643 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/striatum/dspn/str-dspn-e150602_c1_D1-mWT-0728MSN01-v20190508/mechanisms.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    92361 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/striatum/dspn/str-dspn-e150602_c1_D1-mWT-0728MSN01-v20190508/modulation.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    94239 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/striatum/dspn/str-dspn-e150602_c1_D1-mWT-0728MSN01-v20190508/modulationDAACh.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    80017 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/striatum/dspn/str-dspn-e150602_c1_D1-mWT-0728MSN01-v20190508/parameters.json
-drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-04-26 08:34:26.300803 snudda-1.4.4/snudda/data/neurons/striatum/dspn/str-dspn-e150917_c10_D1-mWT-P270-20-v20190521/
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)   600711 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/striatum/dspn/str-dspn-e150917_c10_D1-mWT-P270-20-v20190521/WT-P270-20-15ak-cor.swc
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)      643 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/striatum/dspn/str-dspn-e150917_c10_D1-mWT-P270-20-v20190521/mechanisms.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    92630 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/striatum/dspn/str-dspn-e150917_c10_D1-mWT-P270-20-v20190521/modulation.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    59991 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/striatum/dspn/str-dspn-e150917_c10_D1-mWT-P270-20-v20190521/parameters.json
-drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-04-26 08:34:26.300803 snudda-1.4.4/snudda/data/neurons/striatum/dspn/str-dspn-e150917_c6_D1-m21-6-DE-v20190503/
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)   183549 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/striatum/dspn/str-dspn-e150917_c6_D1-m21-6-DE-v20190503/21-6-DE-cor-rep-ax.swc
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)      643 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/striatum/dspn/str-dspn-e150917_c6_D1-m21-6-DE-v20190503/mechanisms.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    92630 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/striatum/dspn/str-dspn-e150917_c6_D1-m21-6-DE-v20190503/modulation.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    59972 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/striatum/dspn/str-dspn-e150917_c6_D1-m21-6-DE-v20190503/parameters.json
-drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-04-26 08:34:26.304803 snudda-1.4.4/snudda/data/neurons/striatum/dspn/str-dspn-e150917_c9_d1-mWT-1215MSN03-v20190521/
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)   660197 2023-02-15 16:15:38.000000 snudda-1.4.4/snudda/data/neurons/striatum/dspn/str-dspn-e150917_c9_d1-mWT-1215MSN03-v20190521/WT-1215MSN03-cor-rep-ax2.swc
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)      643 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/striatum/dspn/str-dspn-e150917_c9_d1-mWT-1215MSN03-v20190521/mechanisms.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    92630 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/striatum/dspn/str-dspn-e150917_c9_d1-mWT-1215MSN03-v20190521/modulation.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    99934 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/striatum/dspn/str-dspn-e150917_c9_d1-mWT-1215MSN03-v20190521/parameters.json
-drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-04-26 08:34:26.252802 snudda-1.4.4/snudda/data/neurons/striatum/fs/
-drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-04-26 08:34:26.304803 snudda-1.4.4/snudda/data/neurons/striatum/fs/str-fs-e160628_FS2-mMTC180800A-IDB-v20190226/
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)   620377 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/striatum/fs/str-fs-e160628_FS2-mMTC180800A-IDB-v20190226/MTC180800A-IDB-cor-rep.swc
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)      244 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/striatum/fs/str-fs-e160628_FS2-mMTC180800A-IDB-v20190226/mechanisms.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)  1226312 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/striatum/fs/str-fs-e160628_FS2-mMTC180800A-IDB-v20190226/modulation.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    21438 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/striatum/fs/str-fs-e160628_FS2-mMTC180800A-IDB-v20190226/parameters.json
-drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-04-26 08:34:26.312803 snudda-1.4.4/snudda/data/neurons/striatum/fs/str-fs-e161024_FS16-mDR-rat-Mar-13-08-1-536-R-v20190225/
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)  4918863 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/striatum/fs/str-fs-e161024_FS16-mDR-rat-Mar-13-08-1-536-R-v20190225/DR-rat-Mar-13-08-1-536-R-cor-rep.swc
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)      244 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/striatum/fs/str-fs-e161024_FS16-mDR-rat-Mar-13-08-1-536-R-v20190225/mechanisms.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)  1226312 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/striatum/fs/str-fs-e161024_FS16-mDR-rat-Mar-13-08-1-536-R-v20190225/modulation.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    19567 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/striatum/fs/str-fs-e161024_FS16-mDR-rat-Mar-13-08-1-536-R-v20190225/parameters.json
-drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-04-26 08:34:26.316803 snudda-1.4.4/snudda/data/neurons/striatum/fs/str-fs-e161205_FS1-mMTC180800A-IDB-v20190312/
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)   620377 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/striatum/fs/str-fs-e161205_FS1-mMTC180800A-IDB-v20190312/MTC180800A-IDB-cor-rep.swc
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)      244 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/striatum/fs/str-fs-e161205_FS1-mMTC180800A-IDB-v20190312/mechanisms.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)  1226312 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/striatum/fs/str-fs-e161205_FS1-mMTC180800A-IDB-v20190312/modulation.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     5366 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/striatum/fs/str-fs-e161205_FS1-mMTC180800A-IDB-v20190312/parameters.json
-drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-04-26 08:34:26.320803 snudda-1.4.4/snudda/data/neurons/striatum/fs/str-fs-e180418_FS5-mMTC251001A-IDB-v20190301/
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)   826139 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/striatum/fs/str-fs-e180418_FS5-mMTC251001A-IDB-v20190301/MTC251001A-IDB-cor-rep.swc
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)      244 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/striatum/fs/str-fs-e180418_FS5-mMTC251001A-IDB-v20190301/mechanisms.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)  1226312 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/striatum/fs/str-fs-e180418_FS5-mMTC251001A-IDB-v20190301/modulation.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     5354 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/striatum/fs/str-fs-e180418_FS5-mMTC251001A-IDB-v20190301/parameters.json
-drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-04-26 08:34:26.252802 snudda-1.4.4/snudda/data/neurons/striatum/ispn/
-drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-04-26 08:34:26.320803 snudda-1.4.4/snudda/data/neurons/striatum/ispn/str-ispn-e150908_c4_D2-m51-5-DE-v20190611/
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)  1013802 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/striatum/ispn/str-ispn-e150908_c4_D2-m51-5-DE-v20190611/51-5-DE-cor-rep-ax.swc
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)      643 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/striatum/ispn/str-ispn-e150908_c4_D2-m51-5-DE-v20190611/mechanisms.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    59125 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/striatum/ispn/str-ispn-e150908_c4_D2-m51-5-DE-v20190611/modulation.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    69979 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/striatum/ispn/str-ispn-e150908_c4_D2-m51-5-DE-v20190611/parameters.json
-drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-04-26 08:34:26.324803 snudda-1.4.4/snudda/data/neurons/striatum/ispn/str-ispn-e150917_c11_D2-mWT-MSN1-v20190603/
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)  1153456 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/striatum/ispn/str-ispn-e150917_c11_D2-mWT-MSN1-v20190603/WT-MSN1-cor-rep-ax.swc
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)      643 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/striatum/ispn/str-ispn-e150917_c11_D2-mWT-MSN1-v20190603/mechanisms.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    59125 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/striatum/ispn/str-ispn-e150917_c11_D2-mWT-MSN1-v20190603/modulation.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    59905 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/striatum/ispn/str-ispn-e150917_c11_D2-mWT-MSN1-v20190603/parameters.json
-drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-04-26 08:34:26.324803 snudda-1.4.4/snudda/data/neurons/striatum/ispn/str-ispn-e151123_c1_D2-mWT-P270-09-v20190527/
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)   587827 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/striatum/ispn/str-ispn-e151123_c1_D2-mWT-P270-09-v20190527/WT-P270-09-15ak-cor.swc
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)      643 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/striatum/ispn/str-ispn-e151123_c1_D2-mWT-P270-09-v20190527/mechanisms.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    59125 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/striatum/ispn/str-ispn-e151123_c1_D2-mWT-P270-09-v20190527/modulation.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    49989 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/striatum/ispn/str-ispn-e151123_c1_D2-mWT-P270-09-v20190527/parameters.json
-drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-04-26 08:34:26.324803 snudda-1.4.4/snudda/data/neurons/striatum/ispn/str-ispn-e160118_c10_D2-m46-3-DE-v20190529/
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)   254041 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/striatum/ispn/str-ispn-e160118_c10_D2-m46-3-DE-v20190529/46-3-DE-cor-rep-ax.swc
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)      643 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/striatum/ispn/str-ispn-e160118_c10_D2-m46-3-DE-v20190529/mechanisms.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    59125 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/striatum/ispn/str-ispn-e160118_c10_D2-m46-3-DE-v20190529/modulation.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    29994 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/striatum/ispn/str-ispn-e160118_c10_D2-m46-3-DE-v20190529/parameters.json
-drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-04-26 08:34:26.252802 snudda-1.4.4/snudda/data/neurons/striatum/lts/
-drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-04-26 08:34:26.328803 snudda-1.4.4/snudda/data/neurons/striatum/lts/LTS_Experiment-9862_20181211/
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)      582 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/striatum/lts/LTS_Experiment-9862_20181211/fix_indexing.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    19983 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/striatum/lts/LTS_Experiment-9862_20181211/lts_morp_2019-11-07_centered_no_axon.swc
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)      289 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/striatum/lts/LTS_Experiment-9862_20181211/mechanisms.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    32177 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/striatum/lts/LTS_Experiment-9862_20181211/modulation.json
-drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-04-26 08:34:26.328803 snudda-1.4.4/snudda/data/neurons/striatum/lts/LTS_Experiment-9862_20181211/morphologies/
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    19983 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/striatum/lts/LTS_Experiment-9862_20181211/morphologies/lts_morp_2019-11-07_centered_noAxon.swc
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3895 2023-04-26 08:33:58.000000 snudda-1.4.4/snudda/data/neurons/striatum/lts/LTS_Experiment-9862_20181211/parameters.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)      406 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/striatum/lts/LTS_Experiment-9862_20181211/protocols.json
-drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-04-26 08:34:26.328803 snudda-1.4.4/snudda/data/synapses/
-drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-04-26 08:34:26.328803 snudda-1.4.4/snudda/data/synapses/example_data/
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)   127486 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/synapses/example_data/10_MSN12_GBZ_CC_H20.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)      644 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/synapses/example_data/M1LH-contra_dSPN.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1623 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/synapses/formatinfo.txt
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)      238 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/synapses/pair_pulse_experiment_data.json
-drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-04-26 08:34:26.332803 snudda-1.4.4/snudda/data/synapses/striatum/
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    15242 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/synapses/striatum/M1LH_Analysis_191001.h5-parameters-FS.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3494 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/synapses/striatum/M1LH_Analysis_191001.h5-parameters-LTS.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    50601 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/synapses/striatum/M1LH_Analysis_191001.h5-parameters-MS.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     8102 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/synapses/striatum/M1RH_Analysis_190925.h5-parameters-CHAT.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    18630 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/synapses/striatum/M1RH_Analysis_190925.h5-parameters-FS.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    11632 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/synapses/striatum/M1RH_Analysis_190925.h5-parameters-LTS.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    97843 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/synapses/striatum/M1RH_Analysis_190925.h5-parameters-MS.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    39622 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/synapses/striatum/PlanertFitting-DD-tmgaba-fit.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    39725 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/synapses/striatum/PlanertFitting-DI-tmgaba-fit.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    39238 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/synapses/striatum/PlanertFitting-FD-tmgaba-fit.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    39455 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/synapses/striatum/PlanertFitting-FI-tmgaba-fit.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    39599 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/synapses/striatum/PlanertFitting-ID-tmgaba-fit.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    39624 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/synapses/striatum/PlanertFitting-II-tmgaba-fit.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3535 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/synapses/striatum/S1_Analysis_191001.h5-parameters-CHAT.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    28148 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/synapses/striatum/S1_Analysis_191001.h5-parameters-FS.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2277 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/synapses/striatum/S1_Analysis_191001.h5-parameters-LTS.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)   140662 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/synapses/striatum/S1_Analysis_191001.h5-parameters-MS.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    19848 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/synapses/striatum/TH_Analysis_191001.h5-parameters-CHAT.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    12939 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/synapses/striatum/TH_Analysis_191001.h5-parameters-FS.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)   109072 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/synapses/striatum/TH_Analysis_191001.h5-parameters-MS.json
-drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-04-26 08:34:26.332803 snudda-1.4.4/snudda/data/synapses/striatum/partial/
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1092 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/synapses/striatum/partial/trace_table.txt-parameters-DD.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1079 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/synapses/striatum/partial/trace_table.txt-parameters-DI.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3255 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/synapses/striatum/partial/trace_table.txt-parameters-FD.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     4345 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/synapses/striatum/partial/trace_table.txt-parameters-FI.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     8626 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/synapses/striatum/partial/trace_table.txt-parameters-ID.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     5339 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/synapses/striatum/partial/trace_table.txt-parameters-II.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1093 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/synapses/striatum/partial/trace_table.txt-parameters-LI.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)      413 2023-04-26 08:33:58.000000 snudda-1.4.4/snudda/data/synapses/striatum/readme.txt
-drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-04-26 08:34:26.336803 snudda-1.4.4/snudda/data/synapses/v1/
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     9657 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/synapses/v1/M1_Analysis_LH_extr_UP.pxp-traceList-FS-require-H20-model-parameters.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3482 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/synapses/v1/M1_Analysis_LH_extr_UP.pxp-traceList-LTS-require-H20-model-parameters.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     7077 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/synapses/v1/M1_Analysis_LH_extr_UP.pxp-traceList-MSND1-require-H20-model-parameters.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     8386 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/synapses/v1/M1_Analysis_LH_extr_UP.pxp-traceList-MSND2-require-H20-model-parameters.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    13748 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/synapses/v1/M1_Analysis_RH_extr_UP.pxp-traceList-FS-require-H20-model-parameters.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    12464 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/synapses/v1/M1_Analysis_RH_extr_UP.pxp-traceList-LTS-require-H20-model-parameters.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    13368 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/synapses/v1/M1_Analysis_RH_extr_UP.pxp-traceList-MSND1-require-H20-model-parameters.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     8270 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/synapses/v1/M1_Analysis_RH_extr_UP.pxp-traceList-MSND2-require-H20-model-parameters.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    19238 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/synapses/v1/S1_Analysis_extr_UP.pxp-traceList-FS-require-H20-model-parameters.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     8345 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/synapses/v1/S1_Analysis_extr_UP.pxp-traceList-LTS-require-H20-model-parameters.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    11827 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/synapses/v1/S1_Analysis_extr_UP.pxp-traceList-MSND1-require-H20-model-parameters.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    11864 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/synapses/v1/S1_Analysis_extr_UP.pxp-traceList-MSND2-require-H20-model-parameters.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    16683 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/synapses/v1/TH_Analysis_extr_UP.pxp-traceList-CH-require-H20-model-parameters.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     9737 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/synapses/v1/TH_Analysis_extr_UP.pxp-traceList-FS-require-H20-model-parameters.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    15282 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/synapses/v1/TH_Analysis_extr_UP.pxp-traceList-MSND1-require-H20-model-parameters.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    17464 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/synapses/v1/TH_Analysis_extr_UP.pxp-traceList-MSND2-require-H20-model-parameters.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)      751 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/synapses/v1/trace_table.txt-DD-model-parameters.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)      738 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/synapses/v1/trace_table.txt-DI-model-parameters.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2213 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/synapses/v1/trace_table.txt-FD-model-parameters.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2943 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/synapses/v1/trace_table.txt-FI-model-parameters.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     5839 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/synapses/v1/trace_table.txt-ID-model-parameters.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3600 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/synapses/v1/trace_table.txt-II-model-parameters.json
-drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-04-26 08:34:26.336803 snudda-1.4.4/snudda/detect/
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)      138 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/detect/__init__.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)   157811 2023-04-26 08:33:58.000000 snudda-1.4.4/snudda/detect/detect.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    16515 2023-02-15 16:15:38.000000 snudda-1.4.4/snudda/detect/project.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    15527 2023-02-15 16:15:38.000000 snudda-1.4.4/snudda/detect/projection_detection.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)   103112 2023-04-26 08:33:58.000000 snudda-1.4.4/snudda/detect/prune.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)      801 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/help.py
-drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-04-26 08:34:26.336803 snudda-1.4.4/snudda/init/
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)       40 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/init/__init__.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    77893 2023-04-26 08:33:58.000000 snudda-1.4.4/snudda/init/init.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3141 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/init/init_custom.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2308 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/init/init_wojtek.py
-drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-04-26 08:34:26.336803 snudda-1.4.4/snudda/input/
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)       95 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/input/__init__.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    98298 2023-04-26 08:33:58.000000 snudda-1.4.4/snudda/input/input.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    47318 2023-02-15 16:15:38.000000 snudda-1.4.4/snudda/input/input_tuning.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2809 2023-02-15 16:15:38.000000 snudda-1.4.4/snudda/input/inspectinput.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     5135 2022-11-03 09:16:18.000000 snudda-1.4.4/snudda/input/time_varying_input.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1088 2023-02-15 16:15:38.000000 snudda-1.4.4/snudda/input/virtual_input.py
-drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-04-26 08:34:26.336803 snudda-1.4.4/snudda/neuromodulation/
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)      177 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/neuromodulation/__init__.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2679 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/neuromodulation/modulation.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     7470 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/neuromodulation/modulation_network.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     4495 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/neuromodulation/modulation_synapse.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     7179 2023-02-15 16:15:38.000000 snudda-1.4.4/snudda/neuromodulation/neuromodulation.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    21645 2023-02-15 16:15:38.000000 snudda-1.4.4/snudda/neuromodulation/neuromodulation_synapse.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)      289 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/neuromodulation/translator.py
-drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-04-26 08:34:26.336803 snudda-1.4.4/snudda/neurons/
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)      203 2023-02-15 16:15:38.000000 snudda-1.4.4/snudda/neurons/__init__.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1617 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/neurons/index_tree.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    34255 2023-04-26 08:33:58.000000 snudda-1.4.4/snudda/neurons/morphology_data.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    18302 2023-02-15 16:15:38.000000 snudda-1.4.4/snudda/neurons/neuron_model_extended.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    54245 2023-02-15 16:15:38.000000 snudda-1.4.4/snudda/neurons/neuron_morphology.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    23275 2023-04-26 08:33:58.000000 snudda-1.4.4/snudda/neurons/neuron_morphology_extended.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    21962 2023-02-15 16:15:38.000000 snudda-1.4.4/snudda/neurons/neuron_prototype.py
-drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-04-26 08:34:26.340803 snudda-1.4.4/snudda/place/
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)      258 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/place/__init__.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2747 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/place/create_cube_mesh.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3196 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/place/create_slice_mesh.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    57441 2023-04-26 08:33:58.000000 snudda-1.4.4/snudda/place/place.py
--rwxr-xr-x   0 hjorth    (1001) hjorth    (1001)     4611 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/place/projection_map_finder.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    54892 2023-02-15 16:15:38.000000 snudda-1.4.4/snudda/place/region_mesh.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     7972 2023-02-15 16:15:38.000000 snudda-1.4.4/snudda/place/rotation.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     5670 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/place/volumetric_mapping.py
-drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-04-26 08:34:26.340803 snudda-1.4.4/snudda/plotting/
-drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-04-26 08:34:26.340803 snudda-1.4.4/snudda/plotting/Blender/
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)        0 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/plotting/Blender/__init__.py
-drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-04-26 08:34:26.340803 snudda-1.4.4/snudda/plotting/Blender/io_mesh_swc/
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)      661 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/plotting/Blender/io_mesh_swc/__init__.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     6031 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/plotting/Blender/io_mesh_swc/operator_swc_import.py
-drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-04-26 08:34:26.344803 snudda-1.4.4/snudda/plotting/Blender/visualisation/
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)        0 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/plotting/Blender/visualisation/__init__.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1980 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/plotting/Blender/visualisation/drawHyperCubeSomas.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1429 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/plotting/Blender/visualisation/drawHyperCubeSomasRender.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1217 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/plotting/Blender/visualisation/drawHyperCubeSomasWithLTS.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     4086 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/plotting/Blender/visualisation/makeNeuronCube.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     4371 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/plotting/Blender/visualisation/makeNeuronCubeSubset.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     5497 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/plotting/Blender/visualisation/visualiseCubeOfNeuronsWhiteBackground.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     5109 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/plotting/Blender/visualisation/visualiseStriatumNeurons.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     5250 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/plotting/Blender/visualisation/visualiseStriatumNeuronsWithSynapses.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    22786 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/plotting/Blender/visualisation/visualise_network.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    10089 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/plotting/Blender/visualisation/visualise_network_old.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     5344 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/plotting/Blender/visualisation/visualise_touch_detection.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)      381 2022-11-03 09:16:18.000000 snudda-1.4.4/snudda/plotting/__init__.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3414 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/plotting/plotLTSdensity.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2740 2023-04-26 08:33:58.000000 snudda-1.4.4/snudda/plotting/plot_connection_matrix.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     9403 2023-04-26 08:33:58.000000 snudda-1.4.4/snudda/plotting/plot_connectivity.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     8658 2022-11-03 09:16:18.000000 snudda-1.4.4/snudda/plotting/plot_cross_correlogram.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2869 2023-04-26 08:33:58.000000 snudda-1.4.4/snudda/plotting/plot_degeneration.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     6935 2022-10-07 09:01:39.000000 snudda-1.4.4/snudda/plotting/plot_degeneration_and_growth.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1279 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/plotting/plot_density.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2779 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/plotting/plot_density_slice.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3415 2022-11-03 09:16:18.000000 snudda-1.4.4/snudda/plotting/plot_distance_statistics.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     5309 2022-11-03 09:16:18.000000 snudda-1.4.4/snudda/plotting/plot_input.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    15738 2023-04-26 08:33:58.000000 snudda-1.4.4/snudda/plotting/plot_input_locations.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    11861 2023-02-15 16:15:38.000000 snudda-1.4.4/snudda/plotting/plot_network.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3081 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/plotting/plot_network_simulation.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3703 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/plotting/plot_node_benchmark.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     8024 2022-11-04 18:40:55.000000 snudda-1.4.4/snudda/plotting/plot_period_experiment.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3397 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/plotting/plot_size_benchmark.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    22560 2022-11-03 09:16:18.000000 snudda-1.4.4/snudda/plotting/plot_spike_raster_v2.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    18674 2023-02-15 16:15:38.000000 snudda-1.4.4/snudda/plotting/plot_traces.py
-drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-04-26 08:34:26.344803 snudda-1.4.4/snudda/prune/
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)      226 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/prune/__init__.py
-drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-04-26 08:34:26.344803 snudda-1.4.4/snudda/simulate/
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)       52 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/simulate/__init__.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    24795 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/simulate/model_current_injections.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    22316 2023-02-15 16:15:38.000000 snudda-1.4.4/snudda/simulate/network_pair_pulse_simulation.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3729 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/simulate/nrn_simulator_parallel.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    22967 2022-11-11 14:42:41.000000 snudda-1.4.4/snudda/simulate/pair_recording.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    13157 2023-02-15 16:15:38.000000 snudda-1.4.4/snudda/simulate/save_network_recording.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    81843 2023-02-15 16:15:38.000000 snudda-1.4.4/snudda/simulate/simulate.py
-drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-04-26 08:34:26.348803 snudda-1.4.4/snudda/utils/
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)      437 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/utils/__init__.py
--rwxr-xr-x   0 hjorth    (1001) hjorth    (1001)    22027 2023-04-26 08:33:58.000000 snudda-1.4.4/snudda/utils/ablate_network.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     5292 2023-04-26 08:33:58.000000 snudda-1.4.4/snudda/utils/benchmark_logging.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1237 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/utils/cleanup.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2533 2022-11-03 09:16:18.000000 snudda-1.4.4/snudda/utils/clone_neurons.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    18451 2023-04-26 08:33:58.000000 snudda-1.4.4/snudda/utils/conv_hurt.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1230 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/utils/create_parameter_morphology_input_map.py
--rwxr-xr-x   0 hjorth    (1001) hjorth    (1001)    17769 2023-04-26 08:33:58.000000 snudda-1.4.4/snudda/utils/cut.py
--rwxr-xr-x   0 hjorth    (1001) hjorth    (1001)     3728 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/utils/export_connection_matrix.py
--rwxr-xr-x   0 hjorth    (1001) hjorth    (1001)     4512 2023-04-26 08:33:58.000000 snudda-1.4.4/snudda/utils/export_eroded_connection_matrix.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    35149 2023-04-26 08:33:58.000000 snudda-1.4.4/snudda/utils/export_sonata.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2310 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/utils/fake_load.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)       80 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/utils/input_helper.py
--rwxr-xr-x   0 hjorth    (1001) hjorth    (1001)    49806 2023-04-26 08:33:58.000000 snudda-1.4.4/snudda/utils/load.py
--rwxr-xr-x   0 hjorth    (1001) hjorth    (1001)    15170 2023-02-15 16:15:38.000000 snudda-1.4.4/snudda/utils/load_network_simulation.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)      278 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/utils/memory.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     6298 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/utils/merge_synapse_files.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)      593 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/utils/numpy_encoder.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)      185 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/utils/pip_upgrade.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3919 2023-02-15 16:15:38.000000 snudda-1.4.4/snudda/utils/reposition_neurons.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     4840 2023-02-15 16:15:38.000000 snudda-1.4.4/snudda/utils/snudda_path.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    38508 2023-04-26 08:33:58.000000 snudda-1.4.4/snudda/utils/swap_to_degenerated_morphologies.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    19223 2023-04-26 08:33:58.000000 snudda-1.4.4/snudda/utils/swap_to_degenerated_morphologies_extended.py
--rwxr-xr-x   0 hjorth    (1001) hjorth    (1001)     1916 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/utils/upgrade_old_network_file.py
-drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-04-26 08:34:26.252802 snudda-1.4.4/snudda.egg-info/
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     4188 2023-04-26 08:34:26.000000 snudda-1.4.4/snudda.egg-info/PKG-INFO
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    22867 2023-04-26 08:34:26.000000 snudda-1.4.4/snudda.egg-info/SOURCES.txt
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)        1 2023-04-26 08:34:26.000000 snudda-1.4.4/snudda.egg-info/dependency_links.txt
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)      417 2023-04-26 08:34:26.000000 snudda-1.4.4/snudda.egg-info/entry_points.txt
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)      197 2023-04-26 08:34:26.000000 snudda-1.4.4/snudda.egg-info/requires.txt
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)        7 2023-04-26 08:34:26.000000 snudda-1.4.4/snudda.egg-info/top_level.txt
+drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-06-27 13:27:26.432946 snudda-1.4.71/
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    35149 2022-09-19 09:45:08.000000 snudda-1.4.71/LICENSE
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     4234 2023-06-27 13:27:26.432946 snudda-1.4.71/PKG-INFO
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3756 2023-06-27 13:26:59.000000 snudda-1.4.71/README.md
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)       38 2023-06-27 13:27:26.432946 snudda-1.4.71/setup.cfg
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2696 2023-06-27 13:26:59.000000 snudda-1.4.71/setup.py
+drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-06-27 13:27:26.340947 snudda-1.4.71/snudda/
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)      507 2023-06-27 13:26:59.000000 snudda-1.4.71/snudda/__init__.py
+drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-06-27 13:27:26.340947 snudda-1.4.71/snudda/analyse/
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)      199 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/analyse/__init__.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)   107771 2023-06-27 13:26:59.000000 snudda-1.4.71/snudda/analyse/analyse.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     7923 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/analyse/analyse_gap_junction_coupling.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3251 2023-02-15 16:15:38.000000 snudda-1.4.71/snudda/analyse/analyse_input.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     5575 2022-11-03 09:16:18.000000 snudda-1.4.71/snudda/analyse/analyse_neuroinformatics2020.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     8650 2023-06-27 13:26:59.000000 snudda-1.4.71/snudda/analyse/analyse_spike_trains.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    18255 2022-11-03 09:16:18.000000 snudda-1.4.71/snudda/analyse/analyse_striatum.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2996 2023-06-27 13:26:59.000000 snudda-1.4.71/snudda/analyse/analyse_synapse_location.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     7574 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/analyse/analyse_topology.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    12378 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/analyse/analyse_topology_activity.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     6277 2023-06-27 13:26:59.000000 snudda-1.4.71/snudda/analyse/spike_time_tiling_coefficient.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    11585 2023-06-27 13:26:59.000000 snudda-1.4.71/snudda/cli.py
+-rwxr-xr-x   0 hjorth    (1001) hjorth    (1001)    29470 2023-06-27 13:26:59.000000 snudda-1.4.71/snudda/core.py
+drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-06-27 13:27:26.340947 snudda-1.4.71/snudda/data/
+drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-06-27 13:27:26.336947 snudda-1.4.71/snudda/data/InputAxons/
+drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-06-27 13:27:26.340947 snudda-1.4.71/snudda/data/InputAxons/Cortex/
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)   432939 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/InputAxons/Cortex/AA0059.swc
+drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-06-27 13:27:26.344946 snudda-1.4.71/snudda/data/InputAxons/Cortex/Reg10/
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)   900524 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/InputAxons/Cortex/Reg10/AA0059-reg10.swc
+drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-06-27 13:27:26.344946 snudda-1.4.71/snudda/data/InputAxons/Cortex/Reg15/
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)   597398 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/InputAxons/Cortex/Reg15/AA0059-reg15.swc
+drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-06-27 13:27:26.344946 snudda-1.4.71/snudda/data/InputAxons/Cortex/Reg5/
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)  1809577 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/InputAxons/Cortex/Reg5/AA0059-reg5.swc
+drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-06-27 13:27:26.348947 snudda-1.4.71/snudda/data/InputAxons/GPe2Striatum/
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1269 2023-06-27 13:26:59.000000 snudda-1.4.71/snudda/data/InputAxons/GPe2Striatum/example-projection-config.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)   444324 2023-02-15 16:15:38.000000 snudda-1.4.71/snudda/data/InputAxons/GPe2Striatum/prototypical-axon.swc
+drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-06-27 13:27:26.348947 snudda-1.4.71/snudda/data/InputAxons/Thalamus/
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)   464916 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/InputAxons/Thalamus/AA0054.swc
+drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-06-27 13:27:26.348947 snudda-1.4.71/snudda/data/InputAxons/Thalamus/Reg10/
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)   513478 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/InputAxons/Thalamus/Reg10/AA0054-reg10.swc
+drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-06-27 13:27:26.352947 snudda-1.4.71/snudda/data/InputAxons/Thalamus/Reg15/
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)   346069 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/InputAxons/Thalamus/Reg15/AA0054-reg15.swc
+drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-06-27 13:27:26.352947 snudda-1.4.71/snudda/data/InputAxons/Thalamus/Reg5/
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)  1022637 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/InputAxons/Thalamus/Reg5/AA0054-reg5.swc
+drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-06-27 13:27:26.356947 snudda-1.4.71/snudda/data/density/
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    87096 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/density/1001_STRd_Sst_dens.csv
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    89256 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/density/1001_STRd_Sst_dens_smooth.csv
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    74510 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/density/252_STRd_Chat_dens.csv
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    77158 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/density/252_STRd_Chat_dens_smooth.csv
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    94468 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/density/352_STRd_Drd1_dens.csv
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    95346 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/density/352_STRd_Drd1_dens_smooth.csv
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    95932 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/density/72109410_STRd_Adora2a_dens.csv
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    96454 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/density/72109410_STRd_Adora2a_dens_smooth.csv
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    77578 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/density/79556738_STRd_Pvalb_dens.csv
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    79756 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/density/79556738_STRd_Pvalb_dens_smooth.csv
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1132 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/density/combine_densities.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)  2256264 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/density/dorsal_striatum_density.json
+drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-06-27 13:27:26.336947 snudda-1.4.71/snudda/data/experiment_config/
+drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-06-27 13:27:26.360947 snudda-1.4.71/snudda/data/experiment_config/pair_recording/
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)      469 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/experiment_config/pair_recording/experiment-config-1.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)      583 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/experiment_config/pair_recording/experiment-config-2.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)      635 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/experiment_config/pair_recording/experiment-config-3.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)      636 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/experiment_config/pair_recording/experiment-config-4.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)      455 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/experiment_config/pair_recording/experiment-config-5.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)      595 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/experiment_config/pair_recording/experiment-config-6.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)      693 2022-11-11 14:42:41.000000 snudda-1.4.71/snudda/data/experiment_config/pair_recording/experiment-config-7.json
+drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-06-27 13:27:26.360947 snudda-1.4.71/snudda/data/images/
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    52659 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/images/snudda-video-qr-code.png
+drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-06-27 13:27:26.364946 snudda-1.4.71/snudda/data/input_config/
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     5834 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/input_config/external-input-dSTR-scaled-v2.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     5827 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/input_config/external-input-dSTR-scaled-v3.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     5827 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/input_config/external-input-dSTR-scaled-v3b.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     5834 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/input_config/external-input-dSTR-scaled-v4-cluster-test.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     5811 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/input_config/external-input-dSTR-scaled-v4.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     5843 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/input_config/external-input-dSTR-scaled.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)      768 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/input_config/input-tinytest-ChIN.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1831 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/input_config/input-tinytest-Channel-Activation.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1803 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/input_config/input-tinytest-channel-1.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1803 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/input_config/input-tinytest-channel-2.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     5395 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/input_config/input-tinytest-v7.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     5409 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/input_config/input-tinytest-v8.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     5547 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/input_config/input-tinytest-v9-freq-vectors.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     5639 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/input_config/input-v10-scaled.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)      506 2023-06-27 13:26:59.000000 snudda-1.4.71/snudda/data/input_config/input_output_dspn_template_IC.json
+drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-06-27 13:27:26.372946 snudda-1.4.71/snudda/data/mesh/
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)   192511 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/mesh/GPe.obj
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    60912 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/mesh/GPi.obj
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    68536 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/mesh/SNc.obj
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)   164445 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/mesh/SNr.obj
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    44005 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/mesh/STN.obj
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)  1069021 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/mesh/Striatum-d.obj
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)  1733004 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/mesh/Striatum-dorsal-left-hemisphere.obj
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)  1813629 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/mesh/Striatum-dorsal-right-hemisphere.obj
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)   763087 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/mesh/Striatum-v.obj
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2358 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/mesh/get_mesh.ipynb
+drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-06-27 13:27:26.336947 snudda-1.4.71/snudda/data/nest/
+drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-06-27 13:27:26.372946 snudda-1.4.71/snudda/data/nest/models/
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)      272 2023-06-27 13:26:59.000000 snudda-1.4.71/snudda/data/nest/models/FS.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)      278 2023-06-27 13:26:59.000000 snudda-1.4.71/snudda/data/nest/models/dSPN.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)      276 2023-06-27 13:26:59.000000 snudda-1.4.71/snudda/data/nest/models/iSPN.json
+drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-06-27 13:27:26.372946 snudda-1.4.71/snudda/data/nest/synapses/
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)       25 2023-06-27 13:26:59.000000 snudda-1.4.71/snudda/data/nest/synapses/excitatory.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)       25 2023-06-27 13:26:59.000000 snudda-1.4.71/snudda/data/nest/synapses/excitatory_distal.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)       25 2023-06-27 13:26:59.000000 snudda-1.4.71/snudda/data/nest/synapses/excitatory_proximal.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)       25 2023-06-27 13:26:59.000000 snudda-1.4.71/snudda/data/nest/synapses/excitatory_soma.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)       25 2023-06-27 13:26:59.000000 snudda-1.4.71/snudda/data/nest/synapses/inhibitory.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)       25 2023-06-27 13:26:59.000000 snudda-1.4.71/snudda/data/nest/synapses/inhibitory_distal.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)       25 2023-06-27 13:26:59.000000 snudda-1.4.71/snudda/data/nest/synapses/inhibitory_proximal.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)       25 2023-06-27 13:26:59.000000 snudda-1.4.71/snudda/data/nest/synapses/inhibitory_soma.json
+drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-06-27 13:27:26.336947 snudda-1.4.71/snudda/data/neurons/
+drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-06-27 13:27:26.376947 snudda-1.4.71/snudda/data/neurons/mechanisms/
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2111 2023-06-27 13:26:59.000000 snudda-1.4.71/snudda/data/neurons/mechanisms/Im_ms.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1352 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/neurons/mechanisms/Kv3_ch.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1375 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/neurons/mechanisms/NO.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2598 2023-06-27 13:26:59.000000 snudda-1.4.71/snudda/data/neurons/mechanisms/bk_ch.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2511 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/neurons/mechanisms/bk_fs.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2744 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/neurons/mechanisms/bk_ms.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     4351 2023-06-27 13:26:59.000000 snudda-1.4.71/snudda/data/neurons/mechanisms/ca_ch.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1282 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/neurons/mechanisms/cadyn_fs.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1609 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/neurons/mechanisms/cadyn_ms.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     4561 2023-06-27 13:26:59.000000 snudda-1.4.71/snudda/data/neurons/mechanisms/cal12_ms.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     4723 2023-06-27 13:26:59.000000 snudda-1.4.71/snudda/data/neurons/mechanisms/cal13_ms.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2871 2023-06-27 13:26:59.000000 snudda-1.4.71/snudda/data/neurons/mechanisms/cal_ch.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1663 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/neurons/mechanisms/caldyn_ms.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3256 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/neurons/mechanisms/can_fs.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     4517 2023-06-27 13:26:59.000000 snudda-1.4.71/snudda/data/neurons/mechanisms/can_ms.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2986 2023-06-27 13:26:59.000000 snudda-1.4.71/snudda/data/neurons/mechanisms/cap_ch.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2424 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/neurons/mechanisms/caq_fs.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2485 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/neurons/mechanisms/caq_ms.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2814 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/neurons/mechanisms/car_fs.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3855 2023-06-27 13:26:59.000000 snudda-1.4.71/snudda/data/neurons/mechanisms/car_ms.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2413 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/neurons/mechanisms/cat32_ms.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2414 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/neurons/mechanisms/cat33_ms.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1074 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/neurons/mechanisms/concACh.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1084 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/neurons/mechanisms/concDA.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)      907 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/neurons/mechanisms/concDAfile.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3903 2023-06-27 13:26:59.000000 snudda-1.4.71/snudda/data/neurons/mechanisms/hcn12_ch.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2247 2023-06-27 13:26:59.000000 snudda-1.4.71/snudda/data/neurons/mechanisms/hd_lts.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3028 2023-06-27 13:26:59.000000 snudda-1.4.71/snudda/data/neurons/mechanisms/im_lts.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3099 2023-06-27 13:26:59.000000 snudda-1.4.71/snudda/data/neurons/mechanisms/it_lts.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3406 2023-06-27 13:26:59.000000 snudda-1.4.71/snudda/data/neurons/mechanisms/kaf_fs.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3407 2023-06-27 13:26:59.000000 snudda-1.4.71/snudda/data/neurons/mechanisms/kaf_lts.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     4335 2023-06-27 13:26:59.000000 snudda-1.4.71/snudda/data/neurons/mechanisms/kaf_ms.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3334 2023-06-27 13:26:59.000000 snudda-1.4.71/snudda/data/neurons/mechanisms/kas_fs.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3932 2023-06-27 13:26:59.000000 snudda-1.4.71/snudda/data/neurons/mechanisms/kas_ms.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1189 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/neurons/mechanisms/kcnq_ch.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1179 2023-06-27 13:26:59.000000 snudda-1.4.71/snudda/data/neurons/mechanisms/kdb_lts.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1781 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/neurons/mechanisms/kdr_fs.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2810 2023-06-27 13:26:59.000000 snudda-1.4.71/snudda/data/neurons/mechanisms/kdr_lts.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1725 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/neurons/mechanisms/kdr_ms.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1230 2023-06-27 13:26:59.000000 snudda-1.4.71/snudda/data/neurons/mechanisms/kdrb_lts.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3594 2023-06-27 13:26:59.000000 snudda-1.4.71/snudda/data/neurons/mechanisms/kir23_ch.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3595 2023-06-27 13:26:59.000000 snudda-1.4.71/snudda/data/neurons/mechanisms/kir23_lts.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1665 2023-06-27 13:26:59.000000 snudda-1.4.71/snudda/data/neurons/mechanisms/kir2_ch.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3586 2023-06-27 13:26:59.000000 snudda-1.4.71/snudda/data/neurons/mechanisms/kir_fs.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     4151 2023-06-27 13:26:59.000000 snudda-1.4.71/snudda/data/neurons/mechanisms/kir_ms.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1254 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/neurons/mechanisms/kv2_ch.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2679 2023-06-27 13:26:59.000000 snudda-1.4.71/snudda/data/neurons/mechanisms/kv4_ch.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3111 2023-06-27 13:26:59.000000 snudda-1.4.71/snudda/data/neurons/mechanisms/na2_ch.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3677 2023-06-27 13:26:59.000000 snudda-1.4.71/snudda/data/neurons/mechanisms/na3_lts.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3119 2023-06-27 13:26:59.000000 snudda-1.4.71/snudda/data/neurons/mechanisms/na_ch.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2833 2023-06-27 13:26:59.000000 snudda-1.4.71/snudda/data/neurons/mechanisms/naf_fs.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3043 2023-06-27 13:26:59.000000 snudda-1.4.71/snudda/data/neurons/mechanisms/naf_lts.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3245 2023-06-27 13:26:59.000000 snudda-1.4.71/snudda/data/neurons/mechanisms/naf_ms.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)      377 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/neurons/mechanisms/par_ggap.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1909 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/neurons/mechanisms/sk_ch.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1896 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/neurons/mechanisms/sk_fs.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1896 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/neurons/mechanisms/sk_ms.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2370 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/neurons/mechanisms/tmampa.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     4291 2023-06-27 13:26:59.000000 snudda-1.4.71/snudda/data/neurons/mechanisms/tmgabaa.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     7671 2023-06-27 13:26:59.000000 snudda-1.4.71/snudda/data/neurons/mechanisms/tmglut.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     7535 2023-06-27 13:26:59.000000 snudda-1.4.71/snudda/data/neurons/mechanisms/tmglut_M1RH_D1.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     8029 2023-06-27 13:26:59.000000 snudda-1.4.71/snudda/data/neurons/mechanisms/tmglut_double.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1336 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/neurons/mechanisms/tmnmda.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1026 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/neurons/mechanisms/vecevent.mod
+drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-06-27 13:27:26.380946 snudda-1.4.71/snudda/data/neurons/mechanisms.OLD/
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1352 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/neurons/mechanisms.OLD/Kv3_ch.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2225 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/neurons/mechanisms.OLD/bk_ch.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2511 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/neurons/mechanisms.OLD/bk_fs.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2744 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/neurons/mechanisms.OLD/bk_ms.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3998 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/neurons/mechanisms.OLD/ca_ch.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1282 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/neurons/mechanisms.OLD/cadyn_fs.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1609 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/neurons/mechanisms.OLD/cadyn_ms.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3249 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/neurons/mechanisms.OLD/cal12_ms.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3452 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/neurons/mechanisms.OLD/cal13_ms.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1800 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/neurons/mechanisms.OLD/cal_ch.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1663 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/neurons/mechanisms.OLD/caldyn_ms.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3256 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/neurons/mechanisms.OLD/can_fs.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3256 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/neurons/mechanisms.OLD/can_ms.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1686 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/neurons/mechanisms.OLD/cap_ch.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2424 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/neurons/mechanisms.OLD/caq_fs.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2485 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/neurons/mechanisms.OLD/caq_ms.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2814 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/neurons/mechanisms.OLD/car_fs.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2814 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/neurons/mechanisms.OLD/car_ms.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2413 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/neurons/mechanisms.OLD/cat32_ms.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2414 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/neurons/mechanisms.OLD/cat33_ms.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1164 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/neurons/mechanisms.OLD/h_lts.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2855 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/neurons/mechanisms.OLD/hcn12_ch.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1724 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/neurons/mechanisms.OLD/im_lts.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2061 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/neurons/mechanisms.OLD/it_lts.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2364 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/neurons/mechanisms.OLD/kaf_fs.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2993 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/neurons/mechanisms.OLD/kaf_ms.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2292 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/neurons/mechanisms.OLD/kas_fs.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2886 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/neurons/mechanisms.OLD/kas_ms.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1189 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/neurons/mechanisms.OLD/kcnq_ch.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1781 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/neurons/mechanisms.OLD/kdr_fs.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1725 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/neurons/mechanisms.OLD/kdr_ms.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1250 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/neurons/mechanisms.OLD/kdrbca1_lts.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)      605 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/neurons/mechanisms.OLD/kir2_ch.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2543 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/neurons/mechanisms.OLD/kir_fs.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2882 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/neurons/mechanisms.OLD/kir_ms.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1254 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/neurons/mechanisms.OLD/kv2_ch.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1642 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/neurons/mechanisms.OLD/kv4_ch.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2082 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/neurons/mechanisms.OLD/na2_ch.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2637 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/neurons/mechanisms.OLD/na3n_lts.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2076 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/neurons/mechanisms.OLD/na_ch.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1791 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/neurons/mechanisms.OLD/naf_fs.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1980 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/neurons/mechanisms.OLD/naf_ms.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)      377 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/neurons/mechanisms.OLD/par_ggap.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1909 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/neurons/mechanisms.OLD/sk_ch.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1896 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/neurons/mechanisms.OLD/sk_fs.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1896 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/neurons/mechanisms.OLD/sk_ms.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2370 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/neurons/mechanisms.OLD/tmampa.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2893 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/neurons/mechanisms.OLD/tmgabaa.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     5773 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/neurons/mechanisms.OLD/tmglut.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1336 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/neurons/mechanisms.OLD/tmnmda.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1026 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/neurons/mechanisms.OLD/vecevent.mod
+drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-06-27 13:27:26.340947 snudda-1.4.71/snudda/data/neurons/striatum/
+drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-06-27 13:27:26.336947 snudda-1.4.71/snudda/data/neurons/striatum/chin/
+drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-06-27 13:27:26.384946 snudda-1.4.71/snudda/data/neurons/striatum/chin/str-chin-e170614_cell6-m17JUL301751_170614_no6_MD_cell_1_x63-v20190710/
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)      215 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/neurons/striatum/chin/str-chin-e170614_cell6-m17JUL301751_170614_no6_MD_cell_1_x63-v20190710/mechanisms.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    89390 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/neurons/striatum/chin/str-chin-e170614_cell6-m17JUL301751_170614_no6_MD_cell_1_x63-v20190710/modulation.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    69404 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/neurons/striatum/chin/str-chin-e170614_cell6-m17JUL301751_170614_no6_MD_cell_1_x63-v20190710/optim_chin_morph_renamed2019-11-08.swc
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3194 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/neurons/striatum/chin/str-chin-e170614_cell6-m17JUL301751_170614_no6_MD_cell_1_x63-v20190710/parameters.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)      403 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/neurons/striatum/chin/str-chin-e170614_cell6-m17JUL301751_170614_no6_MD_cell_1_x63-v20190710/protocols.json
+drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-06-27 13:27:26.336947 snudda-1.4.71/snudda/data/neurons/striatum/dspn/
+drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-06-27 13:27:26.384946 snudda-1.4.71/snudda/data/neurons/striatum/dspn/str-dspn-e150602_c1_D1-mWT-0728MSN01-v20190508/
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)   673225 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/neurons/striatum/dspn/str-dspn-e150602_c1_D1-mWT-0728MSN01-v20190508/WT-0728MSN01-cor-rep-ax.swc
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)      936 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/neurons/striatum/dspn/str-dspn-e150602_c1_D1-mWT-0728MSN01-v20190508/fix_indexing.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)      643 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/neurons/striatum/dspn/str-dspn-e150602_c1_D1-mWT-0728MSN01-v20190508/mechanisms.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    92361 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/neurons/striatum/dspn/str-dspn-e150602_c1_D1-mWT-0728MSN01-v20190508/modulation.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    94239 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/neurons/striatum/dspn/str-dspn-e150602_c1_D1-mWT-0728MSN01-v20190508/modulationDAACh.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    80017 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/neurons/striatum/dspn/str-dspn-e150602_c1_D1-mWT-0728MSN01-v20190508/parameters.json
+drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-06-27 13:27:26.388946 snudda-1.4.71/snudda/data/neurons/striatum/dspn/str-dspn-e150917_c10_D1-mWT-P270-20-v20190521/
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)   600711 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/neurons/striatum/dspn/str-dspn-e150917_c10_D1-mWT-P270-20-v20190521/WT-P270-20-15ak-cor.swc
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)      643 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/neurons/striatum/dspn/str-dspn-e150917_c10_D1-mWT-P270-20-v20190521/mechanisms.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    92630 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/neurons/striatum/dspn/str-dspn-e150917_c10_D1-mWT-P270-20-v20190521/modulation.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    59991 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/neurons/striatum/dspn/str-dspn-e150917_c10_D1-mWT-P270-20-v20190521/parameters.json
+drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-06-27 13:27:26.388946 snudda-1.4.71/snudda/data/neurons/striatum/dspn/str-dspn-e150917_c6_D1-m21-6-DE-v20190503/
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)   183549 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/neurons/striatum/dspn/str-dspn-e150917_c6_D1-m21-6-DE-v20190503/21-6-DE-cor-rep-ax.swc
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)      643 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/neurons/striatum/dspn/str-dspn-e150917_c6_D1-m21-6-DE-v20190503/mechanisms.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    92630 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/neurons/striatum/dspn/str-dspn-e150917_c6_D1-m21-6-DE-v20190503/modulation.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    59972 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/neurons/striatum/dspn/str-dspn-e150917_c6_D1-m21-6-DE-v20190503/parameters.json
+drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-06-27 13:27:26.388946 snudda-1.4.71/snudda/data/neurons/striatum/dspn/str-dspn-e150917_c9_d1-mWT-1215MSN03-v20190521/
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)   660197 2023-02-15 16:15:38.000000 snudda-1.4.71/snudda/data/neurons/striatum/dspn/str-dspn-e150917_c9_d1-mWT-1215MSN03-v20190521/WT-1215MSN03-cor-rep-ax2.swc
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)      643 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/neurons/striatum/dspn/str-dspn-e150917_c9_d1-mWT-1215MSN03-v20190521/mechanisms.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    92630 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/neurons/striatum/dspn/str-dspn-e150917_c9_d1-mWT-1215MSN03-v20190521/modulation.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    99934 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/neurons/striatum/dspn/str-dspn-e150917_c9_d1-mWT-1215MSN03-v20190521/parameters.json
+drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-06-27 13:27:26.336947 snudda-1.4.71/snudda/data/neurons/striatum/fs/
+drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-06-27 13:27:26.392946 snudda-1.4.71/snudda/data/neurons/striatum/fs/str-fs-e160628_FS2-mMTC180800A-IDB-v20190226/
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)   620377 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/neurons/striatum/fs/str-fs-e160628_FS2-mMTC180800A-IDB-v20190226/MTC180800A-IDB-cor-rep.swc
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)      244 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/neurons/striatum/fs/str-fs-e160628_FS2-mMTC180800A-IDB-v20190226/mechanisms.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)  1226312 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/neurons/striatum/fs/str-fs-e160628_FS2-mMTC180800A-IDB-v20190226/modulation.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    21438 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/neurons/striatum/fs/str-fs-e160628_FS2-mMTC180800A-IDB-v20190226/parameters.json
+drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-06-27 13:27:26.400946 snudda-1.4.71/snudda/data/neurons/striatum/fs/str-fs-e161024_FS16-mDR-rat-Mar-13-08-1-536-R-v20190225/
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)  4918863 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/neurons/striatum/fs/str-fs-e161024_FS16-mDR-rat-Mar-13-08-1-536-R-v20190225/DR-rat-Mar-13-08-1-536-R-cor-rep.swc
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)      244 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/neurons/striatum/fs/str-fs-e161024_FS16-mDR-rat-Mar-13-08-1-536-R-v20190225/mechanisms.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)  1226312 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/neurons/striatum/fs/str-fs-e161024_FS16-mDR-rat-Mar-13-08-1-536-R-v20190225/modulation.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    19567 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/neurons/striatum/fs/str-fs-e161024_FS16-mDR-rat-Mar-13-08-1-536-R-v20190225/parameters.json
+drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-06-27 13:27:26.400946 snudda-1.4.71/snudda/data/neurons/striatum/fs/str-fs-e161205_FS1-mMTC180800A-IDB-v20190312/
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)   620377 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/neurons/striatum/fs/str-fs-e161205_FS1-mMTC180800A-IDB-v20190312/MTC180800A-IDB-cor-rep.swc
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)      244 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/neurons/striatum/fs/str-fs-e161205_FS1-mMTC180800A-IDB-v20190312/mechanisms.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)  1226312 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/neurons/striatum/fs/str-fs-e161205_FS1-mMTC180800A-IDB-v20190312/modulation.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     5366 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/neurons/striatum/fs/str-fs-e161205_FS1-mMTC180800A-IDB-v20190312/parameters.json
+drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-06-27 13:27:26.404946 snudda-1.4.71/snudda/data/neurons/striatum/fs/str-fs-e180418_FS5-mMTC251001A-IDB-v20190301/
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)   826139 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/neurons/striatum/fs/str-fs-e180418_FS5-mMTC251001A-IDB-v20190301/MTC251001A-IDB-cor-rep.swc
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)      244 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/neurons/striatum/fs/str-fs-e180418_FS5-mMTC251001A-IDB-v20190301/mechanisms.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)  1226312 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/neurons/striatum/fs/str-fs-e180418_FS5-mMTC251001A-IDB-v20190301/modulation.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     5354 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/neurons/striatum/fs/str-fs-e180418_FS5-mMTC251001A-IDB-v20190301/parameters.json
+drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-06-27 13:27:26.340947 snudda-1.4.71/snudda/data/neurons/striatum/ispn/
+drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-06-27 13:27:26.404946 snudda-1.4.71/snudda/data/neurons/striatum/ispn/str-ispn-e150908_c4_D2-m51-5-DE-v20190611/
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)  1013802 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/neurons/striatum/ispn/str-ispn-e150908_c4_D2-m51-5-DE-v20190611/51-5-DE-cor-rep-ax.swc
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)      643 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/neurons/striatum/ispn/str-ispn-e150908_c4_D2-m51-5-DE-v20190611/mechanisms.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    59125 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/neurons/striatum/ispn/str-ispn-e150908_c4_D2-m51-5-DE-v20190611/modulation.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    69979 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/neurons/striatum/ispn/str-ispn-e150908_c4_D2-m51-5-DE-v20190611/parameters.json
+drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-06-27 13:27:26.408946 snudda-1.4.71/snudda/data/neurons/striatum/ispn/str-ispn-e150917_c11_D2-mWT-MSN1-v20190603/
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)  1153456 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/neurons/striatum/ispn/str-ispn-e150917_c11_D2-mWT-MSN1-v20190603/WT-MSN1-cor-rep-ax.swc
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)      643 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/neurons/striatum/ispn/str-ispn-e150917_c11_D2-mWT-MSN1-v20190603/mechanisms.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    59125 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/neurons/striatum/ispn/str-ispn-e150917_c11_D2-mWT-MSN1-v20190603/modulation.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    59905 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/neurons/striatum/ispn/str-ispn-e150917_c11_D2-mWT-MSN1-v20190603/parameters.json
+drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-06-27 13:27:26.408946 snudda-1.4.71/snudda/data/neurons/striatum/ispn/str-ispn-e151123_c1_D2-mWT-P270-09-v20190527/
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)   587827 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/neurons/striatum/ispn/str-ispn-e151123_c1_D2-mWT-P270-09-v20190527/WT-P270-09-15ak-cor.swc
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)      643 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/neurons/striatum/ispn/str-ispn-e151123_c1_D2-mWT-P270-09-v20190527/mechanisms.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    59125 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/neurons/striatum/ispn/str-ispn-e151123_c1_D2-mWT-P270-09-v20190527/modulation.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    49989 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/neurons/striatum/ispn/str-ispn-e151123_c1_D2-mWT-P270-09-v20190527/parameters.json
+drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-06-27 13:27:26.408946 snudda-1.4.71/snudda/data/neurons/striatum/ispn/str-ispn-e160118_c10_D2-m46-3-DE-v20190529/
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)   254041 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/neurons/striatum/ispn/str-ispn-e160118_c10_D2-m46-3-DE-v20190529/46-3-DE-cor-rep-ax.swc
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)      643 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/neurons/striatum/ispn/str-ispn-e160118_c10_D2-m46-3-DE-v20190529/mechanisms.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    59125 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/neurons/striatum/ispn/str-ispn-e160118_c10_D2-m46-3-DE-v20190529/modulation.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    29994 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/neurons/striatum/ispn/str-ispn-e160118_c10_D2-m46-3-DE-v20190529/parameters.json
+drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-06-27 13:27:26.340947 snudda-1.4.71/snudda/data/neurons/striatum/lts/
+drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-06-27 13:27:26.412946 snudda-1.4.71/snudda/data/neurons/striatum/lts/LTS_Experiment-9862_20181211/
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)      582 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/neurons/striatum/lts/LTS_Experiment-9862_20181211/fix_indexing.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    19983 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/neurons/striatum/lts/LTS_Experiment-9862_20181211/lts_morp_2019-11-07_centered_no_axon.swc
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)      289 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/neurons/striatum/lts/LTS_Experiment-9862_20181211/mechanisms.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    32177 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/neurons/striatum/lts/LTS_Experiment-9862_20181211/modulation.json
+drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-06-27 13:27:26.412946 snudda-1.4.71/snudda/data/neurons/striatum/lts/LTS_Experiment-9862_20181211/morphologies/
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    19983 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/neurons/striatum/lts/LTS_Experiment-9862_20181211/morphologies/lts_morp_2019-11-07_centered_noAxon.swc
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3895 2023-06-27 13:26:59.000000 snudda-1.4.71/snudda/data/neurons/striatum/lts/LTS_Experiment-9862_20181211/parameters.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)      406 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/neurons/striatum/lts/LTS_Experiment-9862_20181211/protocols.json
+drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-06-27 13:27:26.412946 snudda-1.4.71/snudda/data/synapses/
+drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-06-27 13:27:26.412946 snudda-1.4.71/snudda/data/synapses/example_data/
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)   127486 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/synapses/example_data/10_MSN12_GBZ_CC_H20.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)      644 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/synapses/example_data/M1LH-contra_dSPN.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1623 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/synapses/formatinfo.txt
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)      238 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/synapses/pair_pulse_experiment_data.json
+drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-06-27 13:27:26.416946 snudda-1.4.71/snudda/data/synapses/striatum/
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    15242 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/synapses/striatum/M1LH_Analysis_191001.h5-parameters-FS.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3494 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/synapses/striatum/M1LH_Analysis_191001.h5-parameters-LTS.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    50601 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/synapses/striatum/M1LH_Analysis_191001.h5-parameters-MS.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     8102 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/synapses/striatum/M1RH_Analysis_190925.h5-parameters-CHAT.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    18630 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/synapses/striatum/M1RH_Analysis_190925.h5-parameters-FS.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    11632 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/synapses/striatum/M1RH_Analysis_190925.h5-parameters-LTS.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    97843 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/synapses/striatum/M1RH_Analysis_190925.h5-parameters-MS.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    39622 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/synapses/striatum/PlanertFitting-DD-tmgaba-fit.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    39725 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/synapses/striatum/PlanertFitting-DI-tmgaba-fit.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    39238 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/synapses/striatum/PlanertFitting-FD-tmgaba-fit.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    39455 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/synapses/striatum/PlanertFitting-FI-tmgaba-fit.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    39599 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/synapses/striatum/PlanertFitting-ID-tmgaba-fit.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    39624 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/synapses/striatum/PlanertFitting-II-tmgaba-fit.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3535 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/synapses/striatum/S1_Analysis_191001.h5-parameters-CHAT.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    28148 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/synapses/striatum/S1_Analysis_191001.h5-parameters-FS.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2277 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/synapses/striatum/S1_Analysis_191001.h5-parameters-LTS.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)   140662 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/synapses/striatum/S1_Analysis_191001.h5-parameters-MS.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    19848 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/synapses/striatum/TH_Analysis_191001.h5-parameters-CHAT.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    12939 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/synapses/striatum/TH_Analysis_191001.h5-parameters-FS.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)   109072 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/synapses/striatum/TH_Analysis_191001.h5-parameters-MS.json
+drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-06-27 13:27:26.416946 snudda-1.4.71/snudda/data/synapses/striatum/partial/
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1092 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/synapses/striatum/partial/trace_table.txt-parameters-DD.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1079 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/synapses/striatum/partial/trace_table.txt-parameters-DI.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3255 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/synapses/striatum/partial/trace_table.txt-parameters-FD.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     4345 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/synapses/striatum/partial/trace_table.txt-parameters-FI.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     8626 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/synapses/striatum/partial/trace_table.txt-parameters-ID.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     5339 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/synapses/striatum/partial/trace_table.txt-parameters-II.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1093 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/synapses/striatum/partial/trace_table.txt-parameters-LI.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)      413 2023-06-27 13:26:59.000000 snudda-1.4.71/snudda/data/synapses/striatum/readme.txt
+drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-06-27 13:27:26.420946 snudda-1.4.71/snudda/data/synapses/v1/
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     9657 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/synapses/v1/M1_Analysis_LH_extr_UP.pxp-traceList-FS-require-H20-model-parameters.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3482 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/synapses/v1/M1_Analysis_LH_extr_UP.pxp-traceList-LTS-require-H20-model-parameters.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     7077 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/synapses/v1/M1_Analysis_LH_extr_UP.pxp-traceList-MSND1-require-H20-model-parameters.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     8386 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/synapses/v1/M1_Analysis_LH_extr_UP.pxp-traceList-MSND2-require-H20-model-parameters.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    13748 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/synapses/v1/M1_Analysis_RH_extr_UP.pxp-traceList-FS-require-H20-model-parameters.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    12464 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/synapses/v1/M1_Analysis_RH_extr_UP.pxp-traceList-LTS-require-H20-model-parameters.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    13368 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/synapses/v1/M1_Analysis_RH_extr_UP.pxp-traceList-MSND1-require-H20-model-parameters.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     8270 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/synapses/v1/M1_Analysis_RH_extr_UP.pxp-traceList-MSND2-require-H20-model-parameters.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    19238 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/synapses/v1/S1_Analysis_extr_UP.pxp-traceList-FS-require-H20-model-parameters.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     8345 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/synapses/v1/S1_Analysis_extr_UP.pxp-traceList-LTS-require-H20-model-parameters.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    11827 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/synapses/v1/S1_Analysis_extr_UP.pxp-traceList-MSND1-require-H20-model-parameters.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    11864 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/synapses/v1/S1_Analysis_extr_UP.pxp-traceList-MSND2-require-H20-model-parameters.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    16683 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/synapses/v1/TH_Analysis_extr_UP.pxp-traceList-CH-require-H20-model-parameters.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     9737 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/synapses/v1/TH_Analysis_extr_UP.pxp-traceList-FS-require-H20-model-parameters.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    15282 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/synapses/v1/TH_Analysis_extr_UP.pxp-traceList-MSND1-require-H20-model-parameters.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    17464 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/synapses/v1/TH_Analysis_extr_UP.pxp-traceList-MSND2-require-H20-model-parameters.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)      751 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/synapses/v1/trace_table.txt-DD-model-parameters.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)      738 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/synapses/v1/trace_table.txt-DI-model-parameters.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2213 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/synapses/v1/trace_table.txt-FD-model-parameters.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2943 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/synapses/v1/trace_table.txt-FI-model-parameters.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     5839 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/synapses/v1/trace_table.txt-ID-model-parameters.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3600 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/data/synapses/v1/trace_table.txt-II-model-parameters.json
+drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-06-27 13:27:26.420946 snudda-1.4.71/snudda/detect/
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)      138 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/detect/__init__.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)   157811 2023-06-27 13:26:59.000000 snudda-1.4.71/snudda/detect/detect.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    16515 2023-02-15 16:15:38.000000 snudda-1.4.71/snudda/detect/project.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    15527 2023-02-15 16:15:38.000000 snudda-1.4.71/snudda/detect/projection_detection.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)   103112 2023-06-27 13:26:59.000000 snudda-1.4.71/snudda/detect/prune.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)      801 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/help.py
+drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-06-27 13:27:26.420946 snudda-1.4.71/snudda/init/
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)       40 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/init/__init__.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    77893 2023-06-27 13:26:59.000000 snudda-1.4.71/snudda/init/init.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3141 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/init/init_custom.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2308 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/init/init_wojtek.py
+drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-06-27 13:27:26.420946 snudda-1.4.71/snudda/input/
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)       95 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/input/__init__.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)   101303 2023-06-27 13:26:59.000000 snudda-1.4.71/snudda/input/input.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    47318 2023-02-15 16:15:38.000000 snudda-1.4.71/snudda/input/input_tuning.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2809 2023-02-15 16:15:38.000000 snudda-1.4.71/snudda/input/inspectinput.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     5135 2022-11-03 09:16:18.000000 snudda-1.4.71/snudda/input/time_varying_input.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1088 2023-02-15 16:15:38.000000 snudda-1.4.71/snudda/input/virtual_input.py
+drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-06-27 13:27:26.424946 snudda-1.4.71/snudda/neuromodulation/
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)      177 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/neuromodulation/__init__.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2679 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/neuromodulation/modulation.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     7470 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/neuromodulation/modulation_network.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     4495 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/neuromodulation/modulation_synapse.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     7179 2023-02-15 16:15:38.000000 snudda-1.4.71/snudda/neuromodulation/neuromodulation.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    21645 2023-02-15 16:15:38.000000 snudda-1.4.71/snudda/neuromodulation/neuromodulation_synapse.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)      289 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/neuromodulation/translator.py
+drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-06-27 13:27:26.424946 snudda-1.4.71/snudda/neurons/
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)      203 2023-02-15 16:15:38.000000 snudda-1.4.71/snudda/neurons/__init__.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1617 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/neurons/index_tree.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    34038 2023-06-27 13:26:59.000000 snudda-1.4.71/snudda/neurons/morphology_data.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    18302 2023-02-15 16:15:38.000000 snudda-1.4.71/snudda/neurons/neuron_model_extended.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    54245 2023-02-15 16:15:38.000000 snudda-1.4.71/snudda/neurons/neuron_morphology.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    23275 2023-06-27 13:26:59.000000 snudda-1.4.71/snudda/neurons/neuron_morphology_extended.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    21962 2023-02-15 16:15:38.000000 snudda-1.4.71/snudda/neurons/neuron_prototype.py
+drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-06-27 13:27:26.424946 snudda-1.4.71/snudda/place/
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)      258 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/place/__init__.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2747 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/place/create_cube_mesh.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3196 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/place/create_slice_mesh.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    57441 2023-06-27 13:26:59.000000 snudda-1.4.71/snudda/place/place.py
+-rwxr-xr-x   0 hjorth    (1001) hjorth    (1001)     4611 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/place/projection_map_finder.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    54892 2023-02-15 16:15:38.000000 snudda-1.4.71/snudda/place/region_mesh.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     7972 2023-02-15 16:15:38.000000 snudda-1.4.71/snudda/place/rotation.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     5670 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/place/volumetric_mapping.py
+drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-06-27 13:27:26.428946 snudda-1.4.71/snudda/plotting/
+drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-06-27 13:27:26.428946 snudda-1.4.71/snudda/plotting/Blender/
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)        0 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/plotting/Blender/__init__.py
+drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-06-27 13:27:26.428946 snudda-1.4.71/snudda/plotting/Blender/io_mesh_swc/
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)      661 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/plotting/Blender/io_mesh_swc/__init__.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     6031 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/plotting/Blender/io_mesh_swc/operator_swc_import.py
+drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-06-27 13:27:26.428946 snudda-1.4.71/snudda/plotting/Blender/visualisation/
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)        0 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/plotting/Blender/visualisation/__init__.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1980 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/plotting/Blender/visualisation/drawHyperCubeSomas.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1429 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/plotting/Blender/visualisation/drawHyperCubeSomasRender.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1217 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/plotting/Blender/visualisation/drawHyperCubeSomasWithLTS.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     4086 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/plotting/Blender/visualisation/makeNeuronCube.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     4371 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/plotting/Blender/visualisation/makeNeuronCubeSubset.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     5497 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/plotting/Blender/visualisation/visualiseCubeOfNeuronsWhiteBackground.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     5109 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/plotting/Blender/visualisation/visualiseStriatumNeurons.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     5250 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/plotting/Blender/visualisation/visualiseStriatumNeuronsWithSynapses.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    25826 2023-06-27 13:26:59.000000 snudda-1.4.71/snudda/plotting/Blender/visualisation/visualise_network.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    10089 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/plotting/Blender/visualisation/visualise_network_old.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     5344 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/plotting/Blender/visualisation/visualise_touch_detection.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)      381 2022-11-03 09:16:18.000000 snudda-1.4.71/snudda/plotting/__init__.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3414 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/plotting/plotLTSdensity.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2740 2023-06-27 13:26:59.000000 snudda-1.4.71/snudda/plotting/plot_connection_matrix.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     9403 2023-06-27 13:26:59.000000 snudda-1.4.71/snudda/plotting/plot_connectivity.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     8658 2022-11-03 09:16:18.000000 snudda-1.4.71/snudda/plotting/plot_cross_correlogram.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2869 2023-06-27 13:26:59.000000 snudda-1.4.71/snudda/plotting/plot_degeneration.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     6935 2022-10-07 09:01:39.000000 snudda-1.4.71/snudda/plotting/plot_degeneration_and_growth.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1279 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/plotting/plot_density.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2779 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/plotting/plot_density_slice.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3415 2022-11-03 09:16:18.000000 snudda-1.4.71/snudda/plotting/plot_distance_statistics.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     5309 2022-11-03 09:16:18.000000 snudda-1.4.71/snudda/plotting/plot_input.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    15738 2023-06-27 13:26:59.000000 snudda-1.4.71/snudda/plotting/plot_input_locations.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    11861 2023-02-15 16:15:38.000000 snudda-1.4.71/snudda/plotting/plot_network.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3081 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/plotting/plot_network_simulation.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3703 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/plotting/plot_node_benchmark.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     8024 2022-11-04 18:40:55.000000 snudda-1.4.71/snudda/plotting/plot_period_experiment.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3397 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/plotting/plot_size_benchmark.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    22560 2022-11-03 09:16:18.000000 snudda-1.4.71/snudda/plotting/plot_spike_raster_v2.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    18674 2023-02-15 16:15:38.000000 snudda-1.4.71/snudda/plotting/plot_traces.py
+drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-06-27 13:27:26.428946 snudda-1.4.71/snudda/prune/
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)      226 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/prune/__init__.py
+drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-06-27 13:27:26.428946 snudda-1.4.71/snudda/simulate/
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)       52 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/simulate/__init__.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    24795 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/simulate/model_current_injections.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    22316 2023-02-15 16:15:38.000000 snudda-1.4.71/snudda/simulate/network_pair_pulse_simulation.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3729 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/simulate/nrn_simulator_parallel.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    22967 2022-11-11 14:42:41.000000 snudda-1.4.71/snudda/simulate/pair_recording.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    13157 2023-02-15 16:15:38.000000 snudda-1.4.71/snudda/simulate/save_network_recording.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    81843 2023-02-15 16:15:38.000000 snudda-1.4.71/snudda/simulate/simulate.py
+drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-06-27 13:27:26.432946 snudda-1.4.71/snudda/utils/
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)      437 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/utils/__init__.py
+-rwxr-xr-x   0 hjorth    (1001) hjorth    (1001)    22245 2023-06-27 13:26:59.000000 snudda-1.4.71/snudda/utils/ablate_network.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     5292 2023-06-27 13:26:59.000000 snudda-1.4.71/snudda/utils/benchmark_logging.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1237 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/utils/cleanup.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2533 2022-11-03 09:16:18.000000 snudda-1.4.71/snudda/utils/clone_neurons.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    16656 2023-06-27 13:26:59.000000 snudda-1.4.71/snudda/utils/conv_hurt.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1230 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/utils/create_parameter_morphology_input_map.py
+-rwxr-xr-x   0 hjorth    (1001) hjorth    (1001)    17769 2023-06-27 13:26:59.000000 snudda-1.4.71/snudda/utils/cut.py
+-rwxr-xr-x   0 hjorth    (1001) hjorth    (1001)     3728 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/utils/export_connection_matrix.py
+-rwxr-xr-x   0 hjorth    (1001) hjorth    (1001)     4512 2023-06-27 13:26:59.000000 snudda-1.4.71/snudda/utils/export_eroded_connection_matrix.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    52218 2023-06-27 13:26:59.000000 snudda-1.4.71/snudda/utils/export_sonata.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2310 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/utils/fake_load.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)       80 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/utils/input_helper.py
+-rwxr-xr-x   0 hjorth    (1001) hjorth    (1001)    50326 2023-06-27 13:26:59.000000 snudda-1.4.71/snudda/utils/load.py
+-rwxr-xr-x   0 hjorth    (1001) hjorth    (1001)    15170 2023-02-15 16:15:38.000000 snudda-1.4.71/snudda/utils/load_network_simulation.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)      278 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/utils/memory.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     6298 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/utils/merge_synapse_files.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)      593 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/utils/numpy_encoder.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)      185 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/utils/pip_upgrade.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3919 2023-02-15 16:15:38.000000 snudda-1.4.71/snudda/utils/reposition_neurons.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     4840 2023-02-15 16:15:38.000000 snudda-1.4.71/snudda/utils/snudda_path.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    38508 2023-06-27 13:26:59.000000 snudda-1.4.71/snudda/utils/swap_to_degenerated_morphologies.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    19223 2023-06-27 13:26:59.000000 snudda-1.4.71/snudda/utils/swap_to_degenerated_morphologies_extended.py
+-rwxr-xr-x   0 hjorth    (1001) hjorth    (1001)     1916 2022-09-19 09:45:08.000000 snudda-1.4.71/snudda/utils/upgrade_old_network_file.py
+drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-06-27 13:27:26.340947 snudda-1.4.71/snudda.egg-info/
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     4234 2023-06-27 13:27:26.000000 snudda-1.4.71/snudda.egg-info/PKG-INFO
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    23245 2023-06-27 13:27:26.000000 snudda-1.4.71/snudda.egg-info/SOURCES.txt
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)        1 2023-06-27 13:27:26.000000 snudda-1.4.71/snudda.egg-info/dependency_links.txt
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)      417 2023-06-27 13:27:26.000000 snudda-1.4.71/snudda.egg-info/entry_points.txt
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)      189 2023-06-27 13:27:26.000000 snudda-1.4.71/snudda.egg-info/requires.txt
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)        7 2023-06-27 13:27:26.000000 snudda-1.4.71/snudda.egg-info/top_level.txt
```

### Comparing `snudda-1.4.4/LICENSE` & `snudda-1.4.71/LICENSE`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/PKG-INFO` & `snudda-1.4.71/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snudda
-Version: 1.4.4
+Version: 1.4.71
 Summary: Create realistic networks of neurons, synapses placed using touch detection between axons and dendrites.
 Home-page: https://github.com/Hjorthmedh/Snudda
 Author: Johannes Hjorth
 Author-email: hjorth@kth.se
 License: GPLv3
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -18,15 +18,15 @@
 
 ## Contact details
 Johannes Hjorth, Royal Institute of Technology (KTH)
 Human Brain Project
 hjorth@kth.se
 
 ## Funding
-Horizon 2020 Framework Programme (785907, HBP SGA2); Horizon 2020 Framework Programme (945539, HBP SGA3); Vetenskapsrådet (VR-M-2017-02806, VR-M-2020-01652); Swedish e-science Research Center (SeRC); KTH Digital Futures. The computations are enabled by resources provided by the Swedish National Infrastructure for Computing (SNIC) at PDC KTH partially funded by the Swedish Research Council through grant agreement no. 2018-05973. We acknowledge the use of Fenix Infrastructure resources, which are partially funded from the European Union's Horizon 2020 research and innovation programme through the ICEI project under the grant agreement No. 800858.
+Horizon 2020 Framework Programme (785907, HBP SGA2); Horizon 2020 Framework Programme (945539, HBP SGA3); Vetenskapsrådet (VR-M-2017-02806, VR-M-2020-01652); Swedish e-science Research Center (SeRC); KTH Digital Futures. The computations are enabled by resources provided by the Swedish National Infrastructure for Computing (SNIC) at PDC KTH partially funded by the Swedish Research Council through grant agreement no. 2018-05973. We acknowledge the use of Fenix Infrastructure resources, which are partially funded from the European Union's Horizon 2020 research and innovation programme through the ICEI project under the grant agreement No. 800858. Snudda is supported and featured on EBRAINS.
 
 ## Citation
 Please cite the first paper for the general Snudda network creation and simulation methods, and the second paper for the Striatal microcircutiry model.
 
 * *Predicting Synaptic Connectivity for Large-Scale Microcircuit Simulations Using Snudda.* J. J. Johannes Hjorth, Jeanette Hellgren Kotaleski, Alexander Kozlov. Neuroinform (2021). https://doi.org/10.1007/s12021-021-09531-w
 
 * *The microcircuits of striatum in silico.* J. J. Johannes Hjorth, Alexander Kozlov, Ilaria Carannante, Johanna Frost Nylén, Robert Lindroos, Yvonne Johansson, Anna Tokarska, Matthijs C. Dorst, Shreyas M. Suryanarayana, Gilad Silberberg, Jeanette Hellgren Kotaleski, Sten Grillner. Proceedings of the National Academy of Sciences (2020). https://doi.org/10.1073/pnas.2000671117
```

### Comparing `snudda-1.4.4/README.md` & `snudda-1.4.71/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 ## Contact details
 Johannes Hjorth, Royal Institute of Technology (KTH)
 Human Brain Project
 hjorth@kth.se
 
 ## Funding
-Horizon 2020 Framework Programme (785907, HBP SGA2); Horizon 2020 Framework Programme (945539, HBP SGA3); Vetenskapsrådet (VR-M-2017-02806, VR-M-2020-01652); Swedish e-science Research Center (SeRC); KTH Digital Futures. The computations are enabled by resources provided by the Swedish National Infrastructure for Computing (SNIC) at PDC KTH partially funded by the Swedish Research Council through grant agreement no. 2018-05973. We acknowledge the use of Fenix Infrastructure resources, which are partially funded from the European Union's Horizon 2020 research and innovation programme through the ICEI project under the grant agreement No. 800858.
+Horizon 2020 Framework Programme (785907, HBP SGA2); Horizon 2020 Framework Programme (945539, HBP SGA3); Vetenskapsrådet (VR-M-2017-02806, VR-M-2020-01652); Swedish e-science Research Center (SeRC); KTH Digital Futures. The computations are enabled by resources provided by the Swedish National Infrastructure for Computing (SNIC) at PDC KTH partially funded by the Swedish Research Council through grant agreement no. 2018-05973. We acknowledge the use of Fenix Infrastructure resources, which are partially funded from the European Union's Horizon 2020 research and innovation programme through the ICEI project under the grant agreement No. 800858. Snudda is supported and featured on EBRAINS.
 
 ## Citation
 Please cite the first paper for the general Snudda network creation and simulation methods, and the second paper for the Striatal microcircutiry model.
 
 * *Predicting Synaptic Connectivity for Large-Scale Microcircuit Simulations Using Snudda.* J. J. Johannes Hjorth, Jeanette Hellgren Kotaleski, Alexander Kozlov. Neuroinform (2021). https://doi.org/10.1007/s12021-021-09531-w
 
 * *The microcircuits of striatum in silico.* J. J. Johannes Hjorth, Alexander Kozlov, Ilaria Carannante, Johanna Frost Nylén, Robert Lindroos, Yvonne Johansson, Anna Tokarska, Matthijs C. Dorst, Shreyas M. Suryanarayana, Gilad Silberberg, Jeanette Hellgren Kotaleski, Sten Grillner. Proceedings of the National Academy of Sciences (2020). https://doi.org/10.1073/pnas.2000671117
```

### Comparing `snudda-1.4.4/setup.py` & `snudda-1.4.71/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,22 +21,23 @@
     print(f"READTHEDOCS = {os.environ.get('READTHEDOCS')}") 
     install_requires = [
         "bluepyopt>=1.11.7",
         "h5py>=3.2.1",
         "ipyparallel>=6.3.0",
         "matplotlib>=3.3.4",
         "mpi4py>=3.0.3",
-        "numpy==1.23.5",  # Numba depends on specific numpy version, so removing this line for now as numba will install its requirements
+         # "numpy==1.23.5",  # Numba depends on specific numpy version, so removing this line for now as numba will install its requirements
         "scipy>=1.6.3",
         "sonata>=0.0.2",
         "pyzmq>=22.0.3",
         "setuptools",
         "psutil",
         "numexpr>=2.7.3",
         "numba>=0.56.4",
+        "wheel"
         # "igraph"
     ]
     
 setuptools.setup(
     name="snudda",
     version=__version__,
     author="Johannes Hjorth",
```

### Comparing `snudda-1.4.4/snudda/analyse/analyse.py` & `snudda-1.4.71/snudda/analyse/analyse.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,16 @@
 import scipy.sparse as sps
 
 from snudda.utils.load import SnuddaLoad
 from snudda.utils.snudda_path import snudda_parse_path
 
 # !!! We need to parallelise the analysis script also!
 
-class SnuddaAnalyse(object):
+
+class SnuddaAnalyse:
 
     # saveCache = should we save a pickled file with connection matrix?
     # loadCache = should we load cache file if available
     # lowMemory = if false, uses dense matrix which is faster (assuming lots of memory)
 
     def __init__(self,
                  hdf5_file=None,
```

### Comparing `snudda-1.4.4/snudda/analyse/analyse_gap_junction_coupling.py` & `snudda-1.4.71/snudda/analyse/analyse_gap_junction_coupling.py`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/analyse/analyse_input.py` & `snudda-1.4.71/snudda/analyse/analyse_input.py`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/analyse/analyse_neuroinformatics2020.py` & `snudda-1.4.71/snudda/analyse/analyse_neuroinformatics2020.py`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/analyse/analyse_spike_trains.py` & `snudda-1.4.71/snudda/analyse/analyse_spike_trains.py`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/analyse/analyse_striatum.py` & `snudda-1.4.71/snudda/analyse/analyse_striatum.py`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/analyse/analyse_synapse_location.py` & `snudda-1.4.71/snudda/analyse/analyse_synapse_location.py`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/analyse/analyse_topology.py` & `snudda-1.4.71/snudda/analyse/analyse_topology.py`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/analyse/analyse_topology_activity.py` & `snudda-1.4.71/snudda/analyse/analyse_topology_activity.py`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/analyse/spike_time_tiling_coefficient.py` & `snudda-1.4.71/snudda/analyse/spike_time_tiling_coefficient.py`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/cli.py` & `snudda-1.4.71/snudda/cli.py`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/core.py` & `snudda-1.4.71/snudda/core.py`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/InputAxons/Cortex/AA0059.swc` & `snudda-1.4.71/snudda/data/InputAxons/Cortex/AA0059.swc`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/InputAxons/Cortex/Reg10/AA0059-reg10.swc` & `snudda-1.4.71/snudda/data/InputAxons/Cortex/Reg10/AA0059-reg10.swc`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/InputAxons/Cortex/Reg15/AA0059-reg15.swc` & `snudda-1.4.71/snudda/data/InputAxons/Cortex/Reg15/AA0059-reg15.swc`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/InputAxons/Cortex/Reg5/AA0059-reg5.swc` & `snudda-1.4.71/snudda/data/InputAxons/Cortex/Reg5/AA0059-reg5.swc`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/InputAxons/GPe2Striatum/example-projection-config.json` & `snudda-1.4.71/snudda/data/InputAxons/GPe2Striatum/example-projection-config.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/InputAxons/GPe2Striatum/prototypical-axon.swc` & `snudda-1.4.71/snudda/data/InputAxons/GPe2Striatum/prototypical-axon.swc`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/InputAxons/Thalamus/AA0054.swc` & `snudda-1.4.71/snudda/data/InputAxons/Thalamus/AA0054.swc`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/InputAxons/Thalamus/Reg10/AA0054-reg10.swc` & `snudda-1.4.71/snudda/data/InputAxons/Thalamus/Reg10/AA0054-reg10.swc`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/InputAxons/Thalamus/Reg15/AA0054-reg15.swc` & `snudda-1.4.71/snudda/data/InputAxons/Thalamus/Reg15/AA0054-reg15.swc`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/InputAxons/Thalamus/Reg5/AA0054-reg5.swc` & `snudda-1.4.71/snudda/data/InputAxons/Thalamus/Reg5/AA0054-reg5.swc`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/density/1001_STRd_Sst_dens.csv` & `snudda-1.4.71/snudda/data/density/1001_STRd_Sst_dens.csv`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/density/1001_STRd_Sst_dens_smooth.csv` & `snudda-1.4.71/snudda/data/density/1001_STRd_Sst_dens_smooth.csv`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/density/252_STRd_Chat_dens.csv` & `snudda-1.4.71/snudda/data/density/252_STRd_Chat_dens.csv`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/density/252_STRd_Chat_dens_smooth.csv` & `snudda-1.4.71/snudda/data/density/252_STRd_Chat_dens_smooth.csv`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/density/352_STRd_Drd1_dens.csv` & `snudda-1.4.71/snudda/data/density/352_STRd_Drd1_dens.csv`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/density/352_STRd_Drd1_dens_smooth.csv` & `snudda-1.4.71/snudda/data/density/352_STRd_Drd1_dens_smooth.csv`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/density/72109410_STRd_Adora2a_dens.csv` & `snudda-1.4.71/snudda/data/density/72109410_STRd_Adora2a_dens.csv`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/density/72109410_STRd_Adora2a_dens_smooth.csv` & `snudda-1.4.71/snudda/data/density/72109410_STRd_Adora2a_dens_smooth.csv`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/density/79556738_STRd_Pvalb_dens.csv` & `snudda-1.4.71/snudda/data/density/79556738_STRd_Pvalb_dens.csv`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/density/79556738_STRd_Pvalb_dens_smooth.csv` & `snudda-1.4.71/snudda/data/density/79556738_STRd_Pvalb_dens_smooth.csv`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/density/combine_densities.py` & `snudda-1.4.71/snudda/data/density/combine_densities.py`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/density/dorsal_striatum_density.json` & `snudda-1.4.71/snudda/data/density/dorsal_striatum_density.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/experiment_config/pair_recording/experiment-config-2.json` & `snudda-1.4.71/snudda/data/experiment_config/pair_recording/experiment-config-2.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/experiment_config/pair_recording/experiment-config-3.json` & `snudda-1.4.71/snudda/data/experiment_config/pair_recording/experiment-config-3.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/experiment_config/pair_recording/experiment-config-4.json` & `snudda-1.4.71/snudda/data/experiment_config/pair_recording/experiment-config-4.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/experiment_config/pair_recording/experiment-config-6.json` & `snudda-1.4.71/snudda/data/experiment_config/pair_recording/experiment-config-6.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/experiment_config/pair_recording/experiment-config-7.json` & `snudda-1.4.71/snudda/data/experiment_config/pair_recording/experiment-config-7.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/images/snudda-video-qr-code.png` & `snudda-1.4.71/snudda/data/images/snudda-video-qr-code.png`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/input_config/external-input-dSTR-scaled-v2.json` & `snudda-1.4.71/snudda/data/input_config/external-input-dSTR-scaled-v2.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/input_config/external-input-dSTR-scaled-v3.json` & `snudda-1.4.71/snudda/data/input_config/external-input-dSTR-scaled-v3.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/input_config/external-input-dSTR-scaled-v3b.json` & `snudda-1.4.71/snudda/data/input_config/external-input-dSTR-scaled-v3b.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/input_config/external-input-dSTR-scaled-v4-cluster-test.json` & `snudda-1.4.71/snudda/data/input_config/external-input-dSTR-scaled-v4-cluster-test.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/input_config/external-input-dSTR-scaled-v4.json` & `snudda-1.4.71/snudda/data/input_config/external-input-dSTR-scaled-v4.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/input_config/external-input-dSTR-scaled.json` & `snudda-1.4.71/snudda/data/input_config/external-input-dSTR-scaled.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/input_config/input-tinytest-ChIN.json` & `snudda-1.4.71/snudda/data/input_config/input-tinytest-ChIN.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/input_config/input-tinytest-Channel-Activation.json` & `snudda-1.4.71/snudda/data/input_config/input-tinytest-Channel-Activation.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/input_config/input-tinytest-channel-1.json` & `snudda-1.4.71/snudda/data/input_config/input-tinytest-channel-1.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/input_config/input-tinytest-channel-2.json` & `snudda-1.4.71/snudda/data/input_config/input-tinytest-channel-2.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/input_config/input-tinytest-v7.json` & `snudda-1.4.71/snudda/data/input_config/input-tinytest-v7.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/input_config/input-tinytest-v8.json` & `snudda-1.4.71/snudda/data/input_config/input-tinytest-v8.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/input_config/input-tinytest-v9-freq-vectors.json` & `snudda-1.4.71/snudda/data/input_config/input-tinytest-v9-freq-vectors.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/input_config/input-v10-scaled.json` & `snudda-1.4.71/snudda/data/input_config/input-v10-scaled.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/mesh/GPe.obj` & `snudda-1.4.71/snudda/data/mesh/GPe.obj`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/mesh/GPi.obj` & `snudda-1.4.71/snudda/data/mesh/GPi.obj`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/mesh/SNc.obj` & `snudda-1.4.71/snudda/data/mesh/SNc.obj`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/mesh/SNr.obj` & `snudda-1.4.71/snudda/data/mesh/SNr.obj`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/mesh/STN.obj` & `snudda-1.4.71/snudda/data/mesh/STN.obj`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/mesh/Striatum-d.obj` & `snudda-1.4.71/snudda/data/mesh/Striatum-d.obj`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/mesh/Striatum-dorsal-left-hemisphere.obj` & `snudda-1.4.71/snudda/data/mesh/Striatum-dorsal-left-hemisphere.obj`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/mesh/Striatum-dorsal-right-hemisphere.obj` & `snudda-1.4.71/snudda/data/mesh/Striatum-dorsal-right-hemisphere.obj`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/mesh/Striatum-v.obj` & `snudda-1.4.71/snudda/data/mesh/Striatum-v.obj`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/mesh/get_mesh.ipynb` & `snudda-1.4.71/snudda/data/mesh/get_mesh.ipynb`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/neurons/mechanisms/Im_ms.mod` & `snudda-1.4.71/snudda/data/neurons/mechanisms/Im_ms.mod`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/neurons/mechanisms/Kv3_ch.mod` & `snudda-1.4.71/snudda/data/neurons/mechanisms/Kv3_ch.mod`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/neurons/mechanisms/NO.mod` & `snudda-1.4.71/snudda/data/neurons/mechanisms/NO.mod`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/neurons/mechanisms/bk_ch.mod` & `snudda-1.4.71/snudda/data/neurons/mechanisms/bk_ch.mod`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/neurons/mechanisms/bk_fs.mod` & `snudda-1.4.71/snudda/data/neurons/mechanisms/bk_fs.mod`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/neurons/mechanisms/bk_ms.mod` & `snudda-1.4.71/snudda/data/neurons/mechanisms/bk_ms.mod`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/neurons/mechanisms/ca_ch.mod` & `snudda-1.4.71/snudda/data/neurons/mechanisms/ca_ch.mod`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/neurons/mechanisms/cadyn_fs.mod` & `snudda-1.4.71/snudda/data/neurons/mechanisms/cadyn_fs.mod`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/neurons/mechanisms/cadyn_ms.mod` & `snudda-1.4.71/snudda/data/neurons/mechanisms/cadyn_ms.mod`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/neurons/mechanisms/cal12_ms.mod` & `snudda-1.4.71/snudda/data/neurons/mechanisms/cal12_ms.mod`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/neurons/mechanisms/cal13_ms.mod` & `snudda-1.4.71/snudda/data/neurons/mechanisms/cal13_ms.mod`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/neurons/mechanisms/cal_ch.mod` & `snudda-1.4.71/snudda/data/neurons/mechanisms/cal_ch.mod`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/neurons/mechanisms/caldyn_ms.mod` & `snudda-1.4.71/snudda/data/neurons/mechanisms/caldyn_ms.mod`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/neurons/mechanisms/can_fs.mod` & `snudda-1.4.71/snudda/data/neurons/mechanisms/can_fs.mod`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/neurons/mechanisms/can_ms.mod` & `snudda-1.4.71/snudda/data/neurons/mechanisms/can_ms.mod`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/neurons/mechanisms/cap_ch.mod` & `snudda-1.4.71/snudda/data/neurons/mechanisms/cap_ch.mod`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/neurons/mechanisms/caq_fs.mod` & `snudda-1.4.71/snudda/data/neurons/mechanisms/caq_fs.mod`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/neurons/mechanisms/caq_ms.mod` & `snudda-1.4.71/snudda/data/neurons/mechanisms/caq_ms.mod`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/neurons/mechanisms/car_fs.mod` & `snudda-1.4.71/snudda/data/neurons/mechanisms/car_fs.mod`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/neurons/mechanisms/car_ms.mod` & `snudda-1.4.71/snudda/data/neurons/mechanisms/car_ms.mod`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/neurons/mechanisms/cat32_ms.mod` & `snudda-1.4.71/snudda/data/neurons/mechanisms/cat32_ms.mod`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/neurons/mechanisms/cat33_ms.mod` & `snudda-1.4.71/snudda/data/neurons/mechanisms/cat33_ms.mod`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/neurons/mechanisms/concACh.mod` & `snudda-1.4.71/snudda/data/neurons/mechanisms/concACh.mod`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/neurons/mechanisms/concDA.mod` & `snudda-1.4.71/snudda/data/neurons/mechanisms/concDA.mod`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/neurons/mechanisms/concDAfile.mod` & `snudda-1.4.71/snudda/data/neurons/mechanisms/concDAfile.mod`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/neurons/mechanisms/hcn12_ch.mod` & `snudda-1.4.71/snudda/data/neurons/mechanisms/hcn12_ch.mod`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/neurons/mechanisms/hd_lts.mod` & `snudda-1.4.71/snudda/data/neurons/mechanisms/hd_lts.mod`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/neurons/mechanisms/im_lts.mod` & `snudda-1.4.71/snudda/data/neurons/mechanisms/im_lts.mod`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/neurons/mechanisms/it_lts.mod` & `snudda-1.4.71/snudda/data/neurons/mechanisms/it_lts.mod`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/neurons/mechanisms/kaf_fs.mod` & `snudda-1.4.71/snudda/data/neurons/mechanisms/kaf_fs.mod`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/neurons/mechanisms/kaf_lts.mod` & `snudda-1.4.71/snudda/data/neurons/mechanisms/kaf_lts.mod`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/neurons/mechanisms/kaf_ms.mod` & `snudda-1.4.71/snudda/data/neurons/mechanisms/kaf_ms.mod`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/neurons/mechanisms/kas_fs.mod` & `snudda-1.4.71/snudda/data/neurons/mechanisms/kas_fs.mod`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/neurons/mechanisms/kas_ms.mod` & `snudda-1.4.71/snudda/data/neurons/mechanisms/kas_ms.mod`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/neurons/mechanisms/kcnq_ch.mod` & `snudda-1.4.71/snudda/data/neurons/mechanisms/kcnq_ch.mod`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/neurons/mechanisms/kdb_lts.mod` & `snudda-1.4.71/snudda/data/neurons/mechanisms/kdb_lts.mod`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/neurons/mechanisms/kdr_fs.mod` & `snudda-1.4.71/snudda/data/neurons/mechanisms/kdr_fs.mod`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/neurons/mechanisms/kdr_lts.mod` & `snudda-1.4.71/snudda/data/neurons/mechanisms/kdr_lts.mod`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/neurons/mechanisms/kdr_ms.mod` & `snudda-1.4.71/snudda/data/neurons/mechanisms/kdr_ms.mod`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/neurons/mechanisms/kdrb_lts.mod` & `snudda-1.4.71/snudda/data/neurons/mechanisms/kdrb_lts.mod`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/neurons/mechanisms/kir23_ch.mod` & `snudda-1.4.71/snudda/data/neurons/mechanisms/kir23_ch.mod`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/neurons/mechanisms/kir23_lts.mod` & `snudda-1.4.71/snudda/data/neurons/mechanisms/kir23_lts.mod`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/neurons/mechanisms/kir2_ch.mod` & `snudda-1.4.71/snudda/data/neurons/mechanisms/kir2_ch.mod`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/neurons/mechanisms/kir_fs.mod` & `snudda-1.4.71/snudda/data/neurons/mechanisms/kir_fs.mod`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/neurons/mechanisms/kir_ms.mod` & `snudda-1.4.71/snudda/data/neurons/mechanisms/kir_ms.mod`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/neurons/mechanisms/kv2_ch.mod` & `snudda-1.4.71/snudda/data/neurons/mechanisms/kv2_ch.mod`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/neurons/mechanisms/kv4_ch.mod` & `snudda-1.4.71/snudda/data/neurons/mechanisms/kv4_ch.mod`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/neurons/mechanisms/na2_ch.mod` & `snudda-1.4.71/snudda/data/neurons/mechanisms/na2_ch.mod`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/neurons/mechanisms/na3_lts.mod` & `snudda-1.4.71/snudda/data/neurons/mechanisms/na3_lts.mod`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/neurons/mechanisms/na_ch.mod` & `snudda-1.4.71/snudda/data/neurons/mechanisms/na_ch.mod`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/neurons/mechanisms/naf_fs.mod` & `snudda-1.4.71/snudda/data/neurons/mechanisms/naf_fs.mod`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/neurons/mechanisms/naf_lts.mod` & `snudda-1.4.71/snudda/data/neurons/mechanisms/naf_lts.mod`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/neurons/mechanisms/naf_ms.mod` & `snudda-1.4.71/snudda/data/neurons/mechanisms/naf_ms.mod`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/neurons/mechanisms/sk_ch.mod` & `snudda-1.4.71/snudda/data/neurons/mechanisms/sk_ch.mod`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/neurons/mechanisms/sk_fs.mod` & `snudda-1.4.71/snudda/data/neurons/mechanisms/sk_fs.mod`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/neurons/mechanisms/sk_ms.mod` & `snudda-1.4.71/snudda/data/neurons/mechanisms/sk_ms.mod`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/neurons/mechanisms/tmampa.mod` & `snudda-1.4.71/snudda/data/neurons/mechanisms/tmampa.mod`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/neurons/mechanisms/tmgabaa.mod` & `snudda-1.4.71/snudda/data/neurons/mechanisms/tmgabaa.mod`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/neurons/mechanisms/tmglut.mod` & `snudda-1.4.71/snudda/data/neurons/mechanisms/tmglut.mod`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/neurons/mechanisms/tmglut_M1RH_D1.mod` & `snudda-1.4.71/snudda/data/neurons/mechanisms/tmglut_M1RH_D1.mod`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/neurons/mechanisms/tmglut_double.mod` & `snudda-1.4.71/snudda/data/neurons/mechanisms/tmglut_double.mod`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/neurons/mechanisms/tmnmda.mod` & `snudda-1.4.71/snudda/data/neurons/mechanisms/tmnmda.mod`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/neurons/mechanisms/vecevent.mod` & `snudda-1.4.71/snudda/data/neurons/mechanisms/vecevent.mod`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/neurons/mechanisms.OLD/Kv3_ch.mod` & `snudda-1.4.71/snudda/data/neurons/mechanisms.OLD/Kv3_ch.mod`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/neurons/mechanisms.OLD/bk_ch.mod` & `snudda-1.4.71/snudda/data/neurons/mechanisms.OLD/bk_ch.mod`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/neurons/mechanisms.OLD/bk_fs.mod` & `snudda-1.4.71/snudda/data/neurons/mechanisms.OLD/bk_fs.mod`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/neurons/mechanisms.OLD/bk_ms.mod` & `snudda-1.4.71/snudda/data/neurons/mechanisms.OLD/bk_ms.mod`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/neurons/mechanisms.OLD/ca_ch.mod` & `snudda-1.4.71/snudda/data/neurons/mechanisms.OLD/ca_ch.mod`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/neurons/mechanisms.OLD/cadyn_fs.mod` & `snudda-1.4.71/snudda/data/neurons/mechanisms.OLD/cadyn_fs.mod`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/neurons/mechanisms.OLD/cadyn_ms.mod` & `snudda-1.4.71/snudda/data/neurons/mechanisms.OLD/cadyn_ms.mod`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/neurons/mechanisms.OLD/cal12_ms.mod` & `snudda-1.4.71/snudda/data/neurons/mechanisms.OLD/cal12_ms.mod`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/neurons/mechanisms.OLD/cal13_ms.mod` & `snudda-1.4.71/snudda/data/neurons/mechanisms.OLD/cal13_ms.mod`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/neurons/mechanisms.OLD/cal_ch.mod` & `snudda-1.4.71/snudda/data/neurons/mechanisms.OLD/cal_ch.mod`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/neurons/mechanisms.OLD/caldyn_ms.mod` & `snudda-1.4.71/snudda/data/neurons/mechanisms.OLD/caldyn_ms.mod`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/neurons/mechanisms.OLD/can_fs.mod` & `snudda-1.4.71/snudda/data/neurons/mechanisms.OLD/can_fs.mod`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/neurons/mechanisms.OLD/can_ms.mod` & `snudda-1.4.71/snudda/data/neurons/mechanisms.OLD/can_ms.mod`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/neurons/mechanisms.OLD/cap_ch.mod` & `snudda-1.4.71/snudda/data/neurons/mechanisms.OLD/cap_ch.mod`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/neurons/mechanisms.OLD/caq_fs.mod` & `snudda-1.4.71/snudda/data/neurons/mechanisms.OLD/caq_fs.mod`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/neurons/mechanisms.OLD/caq_ms.mod` & `snudda-1.4.71/snudda/data/neurons/mechanisms.OLD/caq_ms.mod`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/neurons/mechanisms.OLD/car_fs.mod` & `snudda-1.4.71/snudda/data/neurons/mechanisms.OLD/car_fs.mod`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/neurons/mechanisms.OLD/car_ms.mod` & `snudda-1.4.71/snudda/data/neurons/mechanisms.OLD/car_ms.mod`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/neurons/mechanisms.OLD/cat32_ms.mod` & `snudda-1.4.71/snudda/data/neurons/mechanisms.OLD/cat32_ms.mod`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/neurons/mechanisms.OLD/cat33_ms.mod` & `snudda-1.4.71/snudda/data/neurons/mechanisms.OLD/cat33_ms.mod`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/neurons/mechanisms.OLD/h_lts.mod` & `snudda-1.4.71/snudda/data/neurons/mechanisms.OLD/h_lts.mod`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/neurons/mechanisms.OLD/hcn12_ch.mod` & `snudda-1.4.71/snudda/data/neurons/mechanisms.OLD/hcn12_ch.mod`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/neurons/mechanisms.OLD/im_lts.mod` & `snudda-1.4.71/snudda/data/neurons/mechanisms.OLD/im_lts.mod`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/neurons/mechanisms.OLD/it_lts.mod` & `snudda-1.4.71/snudda/data/neurons/mechanisms.OLD/it_lts.mod`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/neurons/mechanisms.OLD/kaf_fs.mod` & `snudda-1.4.71/snudda/data/neurons/mechanisms.OLD/kaf_fs.mod`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/neurons/mechanisms.OLD/kaf_ms.mod` & `snudda-1.4.71/snudda/data/neurons/mechanisms.OLD/kaf_ms.mod`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/neurons/mechanisms.OLD/kas_fs.mod` & `snudda-1.4.71/snudda/data/neurons/mechanisms.OLD/kas_fs.mod`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/neurons/mechanisms.OLD/kas_ms.mod` & `snudda-1.4.71/snudda/data/neurons/mechanisms.OLD/kas_ms.mod`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/neurons/mechanisms.OLD/kcnq_ch.mod` & `snudda-1.4.71/snudda/data/neurons/mechanisms.OLD/kcnq_ch.mod`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/neurons/mechanisms.OLD/kdr_fs.mod` & `snudda-1.4.71/snudda/data/neurons/mechanisms.OLD/kdr_fs.mod`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/neurons/mechanisms.OLD/kdr_ms.mod` & `snudda-1.4.71/snudda/data/neurons/mechanisms.OLD/kdr_ms.mod`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/neurons/mechanisms.OLD/kdrbca1_lts.mod` & `snudda-1.4.71/snudda/data/neurons/mechanisms.OLD/kdrbca1_lts.mod`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/neurons/mechanisms.OLD/kir2_ch.mod` & `snudda-1.4.71/snudda/data/neurons/mechanisms.OLD/kir2_ch.mod`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/neurons/mechanisms.OLD/kir_fs.mod` & `snudda-1.4.71/snudda/data/neurons/mechanisms.OLD/kir_fs.mod`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/neurons/mechanisms.OLD/kir_ms.mod` & `snudda-1.4.71/snudda/data/neurons/mechanisms.OLD/kir_ms.mod`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/neurons/mechanisms.OLD/kv2_ch.mod` & `snudda-1.4.71/snudda/data/neurons/mechanisms.OLD/kv2_ch.mod`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/neurons/mechanisms.OLD/kv4_ch.mod` & `snudda-1.4.71/snudda/data/neurons/mechanisms.OLD/kv4_ch.mod`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/neurons/mechanisms.OLD/na2_ch.mod` & `snudda-1.4.71/snudda/data/neurons/mechanisms.OLD/na2_ch.mod`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/neurons/mechanisms.OLD/na3n_lts.mod` & `snudda-1.4.71/snudda/data/neurons/mechanisms.OLD/na3n_lts.mod`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/neurons/mechanisms.OLD/na_ch.mod` & `snudda-1.4.71/snudda/data/neurons/mechanisms.OLD/na_ch.mod`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/neurons/mechanisms.OLD/naf_fs.mod` & `snudda-1.4.71/snudda/data/neurons/mechanisms.OLD/naf_fs.mod`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/neurons/mechanisms.OLD/naf_ms.mod` & `snudda-1.4.71/snudda/data/neurons/mechanisms.OLD/naf_ms.mod`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/neurons/mechanisms.OLD/sk_ch.mod` & `snudda-1.4.71/snudda/data/neurons/mechanisms.OLD/sk_ch.mod`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/neurons/mechanisms.OLD/sk_fs.mod` & `snudda-1.4.71/snudda/data/neurons/mechanisms.OLD/sk_fs.mod`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/neurons/mechanisms.OLD/sk_ms.mod` & `snudda-1.4.71/snudda/data/neurons/mechanisms.OLD/sk_ms.mod`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/neurons/mechanisms.OLD/tmampa.mod` & `snudda-1.4.71/snudda/data/neurons/mechanisms.OLD/tmampa.mod`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/neurons/mechanisms.OLD/tmgabaa.mod` & `snudda-1.4.71/snudda/data/neurons/mechanisms.OLD/tmgabaa.mod`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/neurons/mechanisms.OLD/tmglut.mod` & `snudda-1.4.71/snudda/data/neurons/mechanisms.OLD/tmglut.mod`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/neurons/mechanisms.OLD/tmnmda.mod` & `snudda-1.4.71/snudda/data/neurons/mechanisms.OLD/tmnmda.mod`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/neurons/mechanisms.OLD/vecevent.mod` & `snudda-1.4.71/snudda/data/neurons/mechanisms.OLD/vecevent.mod`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/neurons/striatum/chin/str-chin-e170614_cell6-m17JUL301751_170614_no6_MD_cell_1_x63-v20190710/modulation.json` & `snudda-1.4.71/snudda/data/neurons/striatum/chin/str-chin-e170614_cell6-m17JUL301751_170614_no6_MD_cell_1_x63-v20190710/modulation.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/neurons/striatum/chin/str-chin-e170614_cell6-m17JUL301751_170614_no6_MD_cell_1_x63-v20190710/optim_chin_morph_renamed2019-11-08.swc` & `snudda-1.4.71/snudda/data/neurons/striatum/chin/str-chin-e170614_cell6-m17JUL301751_170614_no6_MD_cell_1_x63-v20190710/optim_chin_morph_renamed2019-11-08.swc`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/neurons/striatum/chin/str-chin-e170614_cell6-m17JUL301751_170614_no6_MD_cell_1_x63-v20190710/parameters.json` & `snudda-1.4.71/snudda/data/neurons/striatum/chin/str-chin-e170614_cell6-m17JUL301751_170614_no6_MD_cell_1_x63-v20190710/parameters.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/neurons/striatum/dspn/str-dspn-e150602_c1_D1-mWT-0728MSN01-v20190508/WT-0728MSN01-cor-rep-ax.swc` & `snudda-1.4.71/snudda/data/neurons/striatum/dspn/str-dspn-e150602_c1_D1-mWT-0728MSN01-v20190508/WT-0728MSN01-cor-rep-ax.swc`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/neurons/striatum/dspn/str-dspn-e150602_c1_D1-mWT-0728MSN01-v20190508/fix_indexing.py` & `snudda-1.4.71/snudda/data/neurons/striatum/dspn/str-dspn-e150602_c1_D1-mWT-0728MSN01-v20190508/fix_indexing.py`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/neurons/striatum/dspn/str-dspn-e150602_c1_D1-mWT-0728MSN01-v20190508/mechanisms.json` & `snudda-1.4.71/snudda/data/neurons/striatum/dspn/str-dspn-e150602_c1_D1-mWT-0728MSN01-v20190508/mechanisms.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/neurons/striatum/dspn/str-dspn-e150602_c1_D1-mWT-0728MSN01-v20190508/modulation.json` & `snudda-1.4.71/snudda/data/neurons/striatum/dspn/str-dspn-e150602_c1_D1-mWT-0728MSN01-v20190508/modulation.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/neurons/striatum/dspn/str-dspn-e150602_c1_D1-mWT-0728MSN01-v20190508/modulationDAACh.json` & `snudda-1.4.71/snudda/data/neurons/striatum/dspn/str-dspn-e150602_c1_D1-mWT-0728MSN01-v20190508/modulationDAACh.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/neurons/striatum/dspn/str-dspn-e150602_c1_D1-mWT-0728MSN01-v20190508/parameters.json` & `snudda-1.4.71/snudda/data/neurons/striatum/dspn/str-dspn-e150602_c1_D1-mWT-0728MSN01-v20190508/parameters.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/neurons/striatum/dspn/str-dspn-e150917_c10_D1-mWT-P270-20-v20190521/WT-P270-20-15ak-cor.swc` & `snudda-1.4.71/snudda/data/neurons/striatum/dspn/str-dspn-e150917_c10_D1-mWT-P270-20-v20190521/WT-P270-20-15ak-cor.swc`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/neurons/striatum/dspn/str-dspn-e150917_c10_D1-mWT-P270-20-v20190521/mechanisms.json` & `snudda-1.4.71/snudda/data/neurons/striatum/dspn/str-dspn-e150917_c10_D1-mWT-P270-20-v20190521/mechanisms.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/neurons/striatum/dspn/str-dspn-e150917_c10_D1-mWT-P270-20-v20190521/modulation.json` & `snudda-1.4.71/snudda/data/neurons/striatum/dspn/str-dspn-e150917_c10_D1-mWT-P270-20-v20190521/modulation.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/neurons/striatum/dspn/str-dspn-e150917_c10_D1-mWT-P270-20-v20190521/parameters.json` & `snudda-1.4.71/snudda/data/neurons/striatum/dspn/str-dspn-e150917_c10_D1-mWT-P270-20-v20190521/parameters.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/neurons/striatum/dspn/str-dspn-e150917_c6_D1-m21-6-DE-v20190503/21-6-DE-cor-rep-ax.swc` & `snudda-1.4.71/snudda/data/neurons/striatum/dspn/str-dspn-e150917_c6_D1-m21-6-DE-v20190503/21-6-DE-cor-rep-ax.swc`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/neurons/striatum/dspn/str-dspn-e150917_c6_D1-m21-6-DE-v20190503/mechanisms.json` & `snudda-1.4.71/snudda/data/neurons/striatum/dspn/str-dspn-e150917_c6_D1-m21-6-DE-v20190503/mechanisms.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/neurons/striatum/dspn/str-dspn-e150917_c6_D1-m21-6-DE-v20190503/modulation.json` & `snudda-1.4.71/snudda/data/neurons/striatum/dspn/str-dspn-e150917_c6_D1-m21-6-DE-v20190503/modulation.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/neurons/striatum/dspn/str-dspn-e150917_c6_D1-m21-6-DE-v20190503/parameters.json` & `snudda-1.4.71/snudda/data/neurons/striatum/dspn/str-dspn-e150917_c6_D1-m21-6-DE-v20190503/parameters.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/neurons/striatum/dspn/str-dspn-e150917_c9_d1-mWT-1215MSN03-v20190521/WT-1215MSN03-cor-rep-ax2.swc` & `snudda-1.4.71/snudda/data/neurons/striatum/dspn/str-dspn-e150917_c9_d1-mWT-1215MSN03-v20190521/WT-1215MSN03-cor-rep-ax2.swc`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/neurons/striatum/dspn/str-dspn-e150917_c9_d1-mWT-1215MSN03-v20190521/mechanisms.json` & `snudda-1.4.71/snudda/data/neurons/striatum/dspn/str-dspn-e150917_c9_d1-mWT-1215MSN03-v20190521/mechanisms.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/neurons/striatum/dspn/str-dspn-e150917_c9_d1-mWT-1215MSN03-v20190521/modulation.json` & `snudda-1.4.71/snudda/data/neurons/striatum/dspn/str-dspn-e150917_c9_d1-mWT-1215MSN03-v20190521/modulation.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/neurons/striatum/dspn/str-dspn-e150917_c9_d1-mWT-1215MSN03-v20190521/parameters.json` & `snudda-1.4.71/snudda/data/neurons/striatum/dspn/str-dspn-e150917_c9_d1-mWT-1215MSN03-v20190521/parameters.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/neurons/striatum/fs/str-fs-e160628_FS2-mMTC180800A-IDB-v20190226/MTC180800A-IDB-cor-rep.swc` & `snudda-1.4.71/snudda/data/neurons/striatum/fs/str-fs-e160628_FS2-mMTC180800A-IDB-v20190226/MTC180800A-IDB-cor-rep.swc`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/neurons/striatum/fs/str-fs-e160628_FS2-mMTC180800A-IDB-v20190226/modulation.json` & `snudda-1.4.71/snudda/data/neurons/striatum/fs/str-fs-e160628_FS2-mMTC180800A-IDB-v20190226/modulation.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/neurons/striatum/fs/str-fs-e160628_FS2-mMTC180800A-IDB-v20190226/parameters.json` & `snudda-1.4.71/snudda/data/neurons/striatum/fs/str-fs-e160628_FS2-mMTC180800A-IDB-v20190226/parameters.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/neurons/striatum/fs/str-fs-e161024_FS16-mDR-rat-Mar-13-08-1-536-R-v20190225/DR-rat-Mar-13-08-1-536-R-cor-rep.swc` & `snudda-1.4.71/snudda/data/neurons/striatum/fs/str-fs-e161024_FS16-mDR-rat-Mar-13-08-1-536-R-v20190225/DR-rat-Mar-13-08-1-536-R-cor-rep.swc`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/neurons/striatum/fs/str-fs-e161024_FS16-mDR-rat-Mar-13-08-1-536-R-v20190225/modulation.json` & `snudda-1.4.71/snudda/data/neurons/striatum/fs/str-fs-e161024_FS16-mDR-rat-Mar-13-08-1-536-R-v20190225/modulation.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/neurons/striatum/fs/str-fs-e161024_FS16-mDR-rat-Mar-13-08-1-536-R-v20190225/parameters.json` & `snudda-1.4.71/snudda/data/neurons/striatum/fs/str-fs-e161024_FS16-mDR-rat-Mar-13-08-1-536-R-v20190225/parameters.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/neurons/striatum/fs/str-fs-e161205_FS1-mMTC180800A-IDB-v20190312/MTC180800A-IDB-cor-rep.swc` & `snudda-1.4.71/snudda/data/neurons/striatum/fs/str-fs-e161205_FS1-mMTC180800A-IDB-v20190312/MTC180800A-IDB-cor-rep.swc`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/neurons/striatum/fs/str-fs-e161205_FS1-mMTC180800A-IDB-v20190312/modulation.json` & `snudda-1.4.71/snudda/data/neurons/striatum/fs/str-fs-e161205_FS1-mMTC180800A-IDB-v20190312/modulation.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/neurons/striatum/fs/str-fs-e161205_FS1-mMTC180800A-IDB-v20190312/parameters.json` & `snudda-1.4.71/snudda/data/neurons/striatum/fs/str-fs-e161205_FS1-mMTC180800A-IDB-v20190312/parameters.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/neurons/striatum/fs/str-fs-e180418_FS5-mMTC251001A-IDB-v20190301/MTC251001A-IDB-cor-rep.swc` & `snudda-1.4.71/snudda/data/neurons/striatum/fs/str-fs-e180418_FS5-mMTC251001A-IDB-v20190301/MTC251001A-IDB-cor-rep.swc`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/neurons/striatum/fs/str-fs-e180418_FS5-mMTC251001A-IDB-v20190301/modulation.json` & `snudda-1.4.71/snudda/data/neurons/striatum/fs/str-fs-e180418_FS5-mMTC251001A-IDB-v20190301/modulation.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/neurons/striatum/fs/str-fs-e180418_FS5-mMTC251001A-IDB-v20190301/parameters.json` & `snudda-1.4.71/snudda/data/neurons/striatum/fs/str-fs-e180418_FS5-mMTC251001A-IDB-v20190301/parameters.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/neurons/striatum/ispn/str-ispn-e150908_c4_D2-m51-5-DE-v20190611/51-5-DE-cor-rep-ax.swc` & `snudda-1.4.71/snudda/data/neurons/striatum/ispn/str-ispn-e150908_c4_D2-m51-5-DE-v20190611/51-5-DE-cor-rep-ax.swc`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/neurons/striatum/ispn/str-ispn-e150908_c4_D2-m51-5-DE-v20190611/mechanisms.json` & `snudda-1.4.71/snudda/data/neurons/striatum/ispn/str-ispn-e150908_c4_D2-m51-5-DE-v20190611/mechanisms.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/neurons/striatum/ispn/str-ispn-e150908_c4_D2-m51-5-DE-v20190611/modulation.json` & `snudda-1.4.71/snudda/data/neurons/striatum/ispn/str-ispn-e150908_c4_D2-m51-5-DE-v20190611/modulation.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/neurons/striatum/ispn/str-ispn-e150908_c4_D2-m51-5-DE-v20190611/parameters.json` & `snudda-1.4.71/snudda/data/neurons/striatum/ispn/str-ispn-e150908_c4_D2-m51-5-DE-v20190611/parameters.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/neurons/striatum/ispn/str-ispn-e150917_c11_D2-mWT-MSN1-v20190603/WT-MSN1-cor-rep-ax.swc` & `snudda-1.4.71/snudda/data/neurons/striatum/ispn/str-ispn-e150917_c11_D2-mWT-MSN1-v20190603/WT-MSN1-cor-rep-ax.swc`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/neurons/striatum/ispn/str-ispn-e150917_c11_D2-mWT-MSN1-v20190603/mechanisms.json` & `snudda-1.4.71/snudda/data/neurons/striatum/ispn/str-ispn-e150917_c11_D2-mWT-MSN1-v20190603/mechanisms.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/neurons/striatum/ispn/str-ispn-e150917_c11_D2-mWT-MSN1-v20190603/modulation.json` & `snudda-1.4.71/snudda/data/neurons/striatum/ispn/str-ispn-e150917_c11_D2-mWT-MSN1-v20190603/modulation.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/neurons/striatum/ispn/str-ispn-e150917_c11_D2-mWT-MSN1-v20190603/parameters.json` & `snudda-1.4.71/snudda/data/neurons/striatum/ispn/str-ispn-e150917_c11_D2-mWT-MSN1-v20190603/parameters.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/neurons/striatum/ispn/str-ispn-e151123_c1_D2-mWT-P270-09-v20190527/WT-P270-09-15ak-cor.swc` & `snudda-1.4.71/snudda/data/neurons/striatum/ispn/str-ispn-e151123_c1_D2-mWT-P270-09-v20190527/WT-P270-09-15ak-cor.swc`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/neurons/striatum/ispn/str-ispn-e151123_c1_D2-mWT-P270-09-v20190527/mechanisms.json` & `snudda-1.4.71/snudda/data/neurons/striatum/ispn/str-ispn-e151123_c1_D2-mWT-P270-09-v20190527/mechanisms.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/neurons/striatum/ispn/str-ispn-e151123_c1_D2-mWT-P270-09-v20190527/modulation.json` & `snudda-1.4.71/snudda/data/neurons/striatum/ispn/str-ispn-e151123_c1_D2-mWT-P270-09-v20190527/modulation.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/neurons/striatum/ispn/str-ispn-e151123_c1_D2-mWT-P270-09-v20190527/parameters.json` & `snudda-1.4.71/snudda/data/neurons/striatum/ispn/str-ispn-e151123_c1_D2-mWT-P270-09-v20190527/parameters.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/neurons/striatum/ispn/str-ispn-e160118_c10_D2-m46-3-DE-v20190529/46-3-DE-cor-rep-ax.swc` & `snudda-1.4.71/snudda/data/neurons/striatum/ispn/str-ispn-e160118_c10_D2-m46-3-DE-v20190529/46-3-DE-cor-rep-ax.swc`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/neurons/striatum/ispn/str-ispn-e160118_c10_D2-m46-3-DE-v20190529/mechanisms.json` & `snudda-1.4.71/snudda/data/neurons/striatum/ispn/str-ispn-e160118_c10_D2-m46-3-DE-v20190529/mechanisms.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/neurons/striatum/ispn/str-ispn-e160118_c10_D2-m46-3-DE-v20190529/modulation.json` & `snudda-1.4.71/snudda/data/neurons/striatum/ispn/str-ispn-e160118_c10_D2-m46-3-DE-v20190529/modulation.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/neurons/striatum/ispn/str-ispn-e160118_c10_D2-m46-3-DE-v20190529/parameters.json` & `snudda-1.4.71/snudda/data/neurons/striatum/ispn/str-ispn-e160118_c10_D2-m46-3-DE-v20190529/parameters.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/neurons/striatum/lts/LTS_Experiment-9862_20181211/fix_indexing.py` & `snudda-1.4.71/snudda/data/neurons/striatum/lts/LTS_Experiment-9862_20181211/fix_indexing.py`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/neurons/striatum/lts/LTS_Experiment-9862_20181211/lts_morp_2019-11-07_centered_no_axon.swc` & `snudda-1.4.71/snudda/data/neurons/striatum/lts/LTS_Experiment-9862_20181211/lts_morp_2019-11-07_centered_no_axon.swc`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/neurons/striatum/lts/LTS_Experiment-9862_20181211/modulation.json` & `snudda-1.4.71/snudda/data/neurons/striatum/lts/LTS_Experiment-9862_20181211/modulation.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/neurons/striatum/lts/LTS_Experiment-9862_20181211/morphologies/lts_morp_2019-11-07_centered_noAxon.swc` & `snudda-1.4.71/snudda/data/neurons/striatum/lts/LTS_Experiment-9862_20181211/morphologies/lts_morp_2019-11-07_centered_noAxon.swc`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/neurons/striatum/lts/LTS_Experiment-9862_20181211/parameters.json` & `snudda-1.4.71/snudda/data/neurons/striatum/lts/LTS_Experiment-9862_20181211/parameters.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/synapses/example_data/10_MSN12_GBZ_CC_H20.json` & `snudda-1.4.71/snudda/data/synapses/example_data/10_MSN12_GBZ_CC_H20.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/synapses/example_data/M1LH-contra_dSPN.json` & `snudda-1.4.71/snudda/data/synapses/example_data/M1LH-contra_dSPN.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/synapses/formatinfo.txt` & `snudda-1.4.71/snudda/data/synapses/formatinfo.txt`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/synapses/striatum/M1LH_Analysis_191001.h5-parameters-FS.json` & `snudda-1.4.71/snudda/data/synapses/striatum/M1LH_Analysis_191001.h5-parameters-FS.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/synapses/striatum/M1LH_Analysis_191001.h5-parameters-LTS.json` & `snudda-1.4.71/snudda/data/synapses/striatum/M1LH_Analysis_191001.h5-parameters-LTS.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/synapses/striatum/M1LH_Analysis_191001.h5-parameters-MS.json` & `snudda-1.4.71/snudda/data/synapses/striatum/M1LH_Analysis_191001.h5-parameters-MS.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/synapses/striatum/M1RH_Analysis_190925.h5-parameters-CHAT.json` & `snudda-1.4.71/snudda/data/synapses/striatum/M1RH_Analysis_190925.h5-parameters-CHAT.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/synapses/striatum/M1RH_Analysis_190925.h5-parameters-FS.json` & `snudda-1.4.71/snudda/data/synapses/striatum/M1RH_Analysis_190925.h5-parameters-FS.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/synapses/striatum/M1RH_Analysis_190925.h5-parameters-LTS.json` & `snudda-1.4.71/snudda/data/synapses/striatum/M1RH_Analysis_190925.h5-parameters-LTS.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/synapses/striatum/M1RH_Analysis_190925.h5-parameters-MS.json` & `snudda-1.4.71/snudda/data/synapses/striatum/M1RH_Analysis_190925.h5-parameters-MS.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/synapses/striatum/PlanertFitting-DD-tmgaba-fit.json` & `snudda-1.4.71/snudda/data/synapses/striatum/PlanertFitting-DD-tmgaba-fit.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/synapses/striatum/PlanertFitting-DI-tmgaba-fit.json` & `snudda-1.4.71/snudda/data/synapses/striatum/PlanertFitting-DI-tmgaba-fit.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/synapses/striatum/PlanertFitting-FD-tmgaba-fit.json` & `snudda-1.4.71/snudda/data/synapses/striatum/PlanertFitting-FD-tmgaba-fit.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/synapses/striatum/PlanertFitting-FI-tmgaba-fit.json` & `snudda-1.4.71/snudda/data/synapses/striatum/PlanertFitting-FI-tmgaba-fit.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/synapses/striatum/PlanertFitting-ID-tmgaba-fit.json` & `snudda-1.4.71/snudda/data/synapses/striatum/PlanertFitting-ID-tmgaba-fit.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/synapses/striatum/PlanertFitting-II-tmgaba-fit.json` & `snudda-1.4.71/snudda/data/synapses/striatum/PlanertFitting-II-tmgaba-fit.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/synapses/striatum/S1_Analysis_191001.h5-parameters-CHAT.json` & `snudda-1.4.71/snudda/data/synapses/striatum/S1_Analysis_191001.h5-parameters-CHAT.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/synapses/striatum/S1_Analysis_191001.h5-parameters-FS.json` & `snudda-1.4.71/snudda/data/synapses/striatum/S1_Analysis_191001.h5-parameters-FS.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/synapses/striatum/S1_Analysis_191001.h5-parameters-LTS.json` & `snudda-1.4.71/snudda/data/synapses/striatum/S1_Analysis_191001.h5-parameters-LTS.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/synapses/striatum/S1_Analysis_191001.h5-parameters-MS.json` & `snudda-1.4.71/snudda/data/synapses/striatum/S1_Analysis_191001.h5-parameters-MS.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/synapses/striatum/TH_Analysis_191001.h5-parameters-CHAT.json` & `snudda-1.4.71/snudda/data/synapses/striatum/TH_Analysis_191001.h5-parameters-CHAT.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/synapses/striatum/TH_Analysis_191001.h5-parameters-FS.json` & `snudda-1.4.71/snudda/data/synapses/striatum/TH_Analysis_191001.h5-parameters-FS.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/synapses/striatum/TH_Analysis_191001.h5-parameters-MS.json` & `snudda-1.4.71/snudda/data/synapses/striatum/TH_Analysis_191001.h5-parameters-MS.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/synapses/striatum/partial/trace_table.txt-parameters-DD.json` & `snudda-1.4.71/snudda/data/synapses/striatum/partial/trace_table.txt-parameters-DD.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/synapses/striatum/partial/trace_table.txt-parameters-DI.json` & `snudda-1.4.71/snudda/data/synapses/striatum/partial/trace_table.txt-parameters-DI.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/synapses/striatum/partial/trace_table.txt-parameters-FD.json` & `snudda-1.4.71/snudda/data/synapses/striatum/partial/trace_table.txt-parameters-FD.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/synapses/striatum/partial/trace_table.txt-parameters-FI.json` & `snudda-1.4.71/snudda/data/synapses/striatum/partial/trace_table.txt-parameters-FI.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/synapses/striatum/partial/trace_table.txt-parameters-ID.json` & `snudda-1.4.71/snudda/data/synapses/striatum/partial/trace_table.txt-parameters-ID.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/synapses/striatum/partial/trace_table.txt-parameters-II.json` & `snudda-1.4.71/snudda/data/synapses/striatum/partial/trace_table.txt-parameters-II.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/synapses/striatum/partial/trace_table.txt-parameters-LI.json` & `snudda-1.4.71/snudda/data/synapses/striatum/partial/trace_table.txt-parameters-LI.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/synapses/v1/M1_Analysis_LH_extr_UP.pxp-traceList-FS-require-H20-model-parameters.json` & `snudda-1.4.71/snudda/data/synapses/v1/M1_Analysis_LH_extr_UP.pxp-traceList-FS-require-H20-model-parameters.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/synapses/v1/M1_Analysis_LH_extr_UP.pxp-traceList-LTS-require-H20-model-parameters.json` & `snudda-1.4.71/snudda/data/synapses/v1/M1_Analysis_LH_extr_UP.pxp-traceList-LTS-require-H20-model-parameters.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/synapses/v1/M1_Analysis_LH_extr_UP.pxp-traceList-MSND1-require-H20-model-parameters.json` & `snudda-1.4.71/snudda/data/synapses/v1/M1_Analysis_LH_extr_UP.pxp-traceList-MSND1-require-H20-model-parameters.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/synapses/v1/M1_Analysis_LH_extr_UP.pxp-traceList-MSND2-require-H20-model-parameters.json` & `snudda-1.4.71/snudda/data/synapses/v1/M1_Analysis_LH_extr_UP.pxp-traceList-MSND2-require-H20-model-parameters.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/synapses/v1/M1_Analysis_RH_extr_UP.pxp-traceList-FS-require-H20-model-parameters.json` & `snudda-1.4.71/snudda/data/synapses/v1/M1_Analysis_RH_extr_UP.pxp-traceList-FS-require-H20-model-parameters.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/synapses/v1/M1_Analysis_RH_extr_UP.pxp-traceList-LTS-require-H20-model-parameters.json` & `snudda-1.4.71/snudda/data/synapses/v1/M1_Analysis_RH_extr_UP.pxp-traceList-LTS-require-H20-model-parameters.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/synapses/v1/M1_Analysis_RH_extr_UP.pxp-traceList-MSND1-require-H20-model-parameters.json` & `snudda-1.4.71/snudda/data/synapses/v1/M1_Analysis_RH_extr_UP.pxp-traceList-MSND1-require-H20-model-parameters.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/synapses/v1/M1_Analysis_RH_extr_UP.pxp-traceList-MSND2-require-H20-model-parameters.json` & `snudda-1.4.71/snudda/data/synapses/v1/M1_Analysis_RH_extr_UP.pxp-traceList-MSND2-require-H20-model-parameters.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/synapses/v1/S1_Analysis_extr_UP.pxp-traceList-FS-require-H20-model-parameters.json` & `snudda-1.4.71/snudda/data/synapses/v1/S1_Analysis_extr_UP.pxp-traceList-FS-require-H20-model-parameters.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/synapses/v1/S1_Analysis_extr_UP.pxp-traceList-LTS-require-H20-model-parameters.json` & `snudda-1.4.71/snudda/data/synapses/v1/S1_Analysis_extr_UP.pxp-traceList-LTS-require-H20-model-parameters.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/synapses/v1/S1_Analysis_extr_UP.pxp-traceList-MSND1-require-H20-model-parameters.json` & `snudda-1.4.71/snudda/data/synapses/v1/S1_Analysis_extr_UP.pxp-traceList-MSND1-require-H20-model-parameters.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/synapses/v1/S1_Analysis_extr_UP.pxp-traceList-MSND2-require-H20-model-parameters.json` & `snudda-1.4.71/snudda/data/synapses/v1/S1_Analysis_extr_UP.pxp-traceList-MSND2-require-H20-model-parameters.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/synapses/v1/TH_Analysis_extr_UP.pxp-traceList-CH-require-H20-model-parameters.json` & `snudda-1.4.71/snudda/data/synapses/v1/TH_Analysis_extr_UP.pxp-traceList-CH-require-H20-model-parameters.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/synapses/v1/TH_Analysis_extr_UP.pxp-traceList-FS-require-H20-model-parameters.json` & `snudda-1.4.71/snudda/data/synapses/v1/TH_Analysis_extr_UP.pxp-traceList-FS-require-H20-model-parameters.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/synapses/v1/TH_Analysis_extr_UP.pxp-traceList-MSND1-require-H20-model-parameters.json` & `snudda-1.4.71/snudda/data/synapses/v1/TH_Analysis_extr_UP.pxp-traceList-MSND1-require-H20-model-parameters.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/synapses/v1/TH_Analysis_extr_UP.pxp-traceList-MSND2-require-H20-model-parameters.json` & `snudda-1.4.71/snudda/data/synapses/v1/TH_Analysis_extr_UP.pxp-traceList-MSND2-require-H20-model-parameters.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/synapses/v1/trace_table.txt-DD-model-parameters.json` & `snudda-1.4.71/snudda/data/synapses/v1/trace_table.txt-DD-model-parameters.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/synapses/v1/trace_table.txt-DI-model-parameters.json` & `snudda-1.4.71/snudda/data/synapses/v1/trace_table.txt-DI-model-parameters.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/synapses/v1/trace_table.txt-FD-model-parameters.json` & `snudda-1.4.71/snudda/data/synapses/v1/trace_table.txt-FD-model-parameters.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/synapses/v1/trace_table.txt-FI-model-parameters.json` & `snudda-1.4.71/snudda/data/synapses/v1/trace_table.txt-FI-model-parameters.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/synapses/v1/trace_table.txt-ID-model-parameters.json` & `snudda-1.4.71/snudda/data/synapses/v1/trace_table.txt-ID-model-parameters.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/data/synapses/v1/trace_table.txt-II-model-parameters.json` & `snudda-1.4.71/snudda/data/synapses/v1/trace_table.txt-II-model-parameters.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/detect/detect.py` & `snudda-1.4.71/snudda/detect/detect.py`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/detect/project.py` & `snudda-1.4.71/snudda/detect/project.py`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/detect/projection_detection.py` & `snudda-1.4.71/snudda/detect/projection_detection.py`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/detect/prune.py` & `snudda-1.4.71/snudda/detect/prune.py`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/help.py` & `snudda-1.4.71/snudda/help.py`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/init/init.py` & `snudda-1.4.71/snudda/init/init.py`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/init/init_custom.py` & `snudda-1.4.71/snudda/init/init_custom.py`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/init/init_wojtek.py` & `snudda-1.4.71/snudda/init/init_wojtek.py`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/input/input.py` & `snudda-1.4.71/snudda/input/input.py`

 * *Files 2% similar despite different names*

```diff
@@ -534,18 +534,23 @@
 
     # Reads from self.inputConfigFile
 
     def read_input_config_file(self):
 
         """ Read input configuration from JSON file. """
 
-        self.write_log(f"Loading input configuration from {self.input_config_file}")
+        if isinstance(self.input_config_file, dict):
+            self.write_log(f"Input was specified directly by a dictionary")
+            self.input_info = self.input_config_file.copy()
 
-        with open(snudda_parse_path(self.input_config_file, self.snudda_data), 'rt') as f:
-            self.input_info = json.load(f, object_pairs_hook=OrderedDict)
+        else:
+            self.write_log(f"Loading input configuration from {self.input_config_file}")
+
+            with open(snudda_parse_path(self.input_config_file, self.snudda_data), 'rt') as f:
+                self.input_info = json.load(f, object_pairs_hook=OrderedDict)
 
         max_time = self.time
 
         for neuron_type in self.input_info:
             for input_type in self.input_info[neuron_type]:
 
                 if "end" in self.input_info[neuron_type][input_type]:
@@ -719,14 +724,15 @@
         parameter_file_list = []
         parameter_list_list = []
         cluster_size_list = []
         cluster_spread_list = []
 
         generator_list = []
         population_unit_fraction_list = []
+        num_soma_synapses_list = []
 
         dendrite_location_override_list = []
         if self.use_meta_input:
             self.write_log("Input from meta.json will be used")
         else:
             self.write_log("Input from meta.json will NOT be used")
 
@@ -873,22 +879,36 @@
                         x = y = z = dist_to_soma = np.zeros((len(sec_id),))
                         input_loc = [(x, y, z), np.array(sec_id), np.array(sec_x), dist_to_soma]
                     else:
                         # Automatically generate dendrite locations
                         cluster_size = None
                         cluster_spread = None
 
+                        if "nSomaSynapses" in input_inf:
+                            n_soma_synapses = input_inf["nSomaSynapses"]
+                        else:
+                            n_soma_synapses = 0
+
+                        if n_soma_synapses > num_spike_trains:
+                            raise ValueError(f"nSomaSynapses can not be greater than the number of input trains read from CSV file")
+
                         # We need a random seed generator for the dendrite_input_location on the master TODO: Cleanup
                         input_loc = self.dendrite_input_locations(neuron_id=neuron_id,
                                                                   synapse_density=synapse_density,
-                                                                  num_spike_trains=num_spike_trains,
+                                                                  num_spike_trains=num_spike_trains - n_soma_synapses,
                                                                   rng=rng_master,
                                                                   cluster_size=cluster_size,
                                                                   cluster_spread=cluster_spread)
 
+                        # If there are synapses on the soma then we need to add those also
+                        if n_soma_synapses > 0:
+                            input_loc = self.add_soma_synapses(input_loc,
+                                                               n_soma_synapses=n_soma_synapses,
+                                                               neuron_id=neuron_id)
+
                     self.neuron_input[neuron_id][input_type]["location"] = input_loc
                     self.neuron_input[neuron_id][input_type]["synapseDensity"] = synapse_density
 
                     parameter_id = rng_master.integers(1e6, size=num_spike_trains)
                     self.neuron_input[neuron_id][input_type]["parameterID"] = parameter_id
 
                     # Done for CSV input
@@ -1045,25 +1065,33 @@
                     freq_list.append(input_inf["frequency"])
                     generator_list.append("frequency_function")
 
                 else:
                     self.write_log(f"Unknown input generator: {input_inf['generator']} for {neuron_id}", is_error=True)
                     assert False, f"Unknown input generator {input_inf['generator']}"
 
+                if "nSomaSynapses" in input_inf:
+                    n_soma_synapses = input_inf["nSomaSynapses"]
+                else:
+                    n_soma_synapses = 0
+
+                num_soma_synapses_list.append(n_soma_synapses)
+
         seed_list = self.generate_seeds(num_states=len(neuron_id_list))
 
         amr = None
 
         assert len(neuron_id_list) == len(input_type_list) == len(freq_list)\
             == len(start_list) == len(end_list) == len(synapse_density_list) == len(num_inputs_list)\
             == len(num_inputs_list) == len(population_unit_spikes_list) == len(jitter_dt_list)\
             == len(population_unit_id_list) == len(conductance_list) == len(correlation_list)\
             == len(mod_file_list) == len(parameter_file_list) == len(parameter_list_list)\
             == len(seed_list) == len(cluster_size_list) == len(cluster_spread_list)\
-            == len(dendrite_location_override_list) == len(generator_list) == len(population_unit_fraction_list),\
+            == len(dendrite_location_override_list) == len(generator_list) == len(population_unit_fraction_list)\
+            == len(num_soma_synapses_list),\
             "Internal error, input lists length missmatch"
 
         # Lets try and swap self.lbView for self.dView
         if self.d_view is not None:
 
             # self.writeLog("Sending jobs to workers, using lbView")
             self.write_log("Sending jobs to workers, using dView")
@@ -1087,15 +1115,16 @@
                                   parameter_file_list,
                                   parameter_list_list,
                                   seed_list,
                                   cluster_size_list,
                                   cluster_spread_list,
                                   dendrite_location_override_list,
                                   generator_list,
-                                  population_unit_fraction_list))
+                                  population_unit_fraction_list,
+                                  num_soma_synapses_list))
 
             self.d_view.scatter("input_list", input_list, block=True)
             cmd_str = "inpt = list(map(nl.make_input_helper_parallel,input_list))"
 
             self.write_log("Calling workers to generate input in parallel")
             self.d_view.execute(cmd_str, block=True)
             self.d_view.execute("nl.write_log('Execution done on workers')")
@@ -1127,15 +1156,16 @@
                       parameter_file_list,
                       parameter_list_list,
                       seed_list,
                       cluster_size_list,
                       cluster_spread_list,
                       dendrite_location_override_list,
                       generator_list,
-                      population_unit_fraction_list)
+                      population_unit_fraction_list,
+                      num_soma_synapses_list)
 
         # Gather the spikes that were generated in parallel
         for neuron_id, input_type, spikes, loc, synapse_density, frq, \
             jdt, p_uid, cond, corr, timeRange, mod_file, param_file, param_list, param_id in amr:
 
             self.write_log(f"Gathering {neuron_id} - {input_type}")
             self.neuron_input[neuron_id][input_type]["spikes"] = spikes
@@ -1862,14 +1892,39 @@
                                                    num_locations=num_spike_trains,
                                                    rng=rng,
                                                    cluster_size=cluster_size,
                                                    cluster_spread=cluster_spread)
 
     ############################################################################
 
+    def add_soma_synapses(self, input_loc, n_soma_synapses, neuron_id):
+
+        if n_soma_synapses is None or n_soma_synapses == 0:
+            return input_loc
+
+        soma_pos = self.neuron_info[neuron_id]["position"]
+
+        xyz, sec_id, sec_x, dist_to_soma = input_loc
+
+        soma_xyz = np.atleast_2d(soma_pos).repeat(repeats=n_soma_synapses, axis=0)
+        soma_sec_id = np.full((n_soma_synapses, ), -1)
+        soma_sec_x = np.full((n_soma_synapses, ), 0.5)
+        soma_dist_to_soma = np.zeros((n_soma_synapses, ))
+
+        new_xyz = np.vstack((xyz, soma_xyz))
+        new_sec_id = np.concatenate((sec_id, soma_sec_id))
+        new_sec_x = np.concatenate((sec_x, soma_sec_x))
+        new_soma_dist = np.concatenate((dist_to_soma, soma_dist_to_soma))
+
+        new_input_loc = (new_xyz, new_sec_id, new_sec_x, new_soma_dist)
+
+        return new_input_loc
+
+    ############################################################################
+
     def setup_parallel(self):
 
         """ Setup worker nodes for parallel execution. """
 
         slurm_job_id = os.getenv("SLURM_JOBID")
 
         if slurm_job_id is None:
@@ -1993,15 +2048,15 @@
         """ Helper function for parallel input generation."""
 
         try:
 
             neuron_id, input_type, freq, start, end, synapse_density, num_spike_trains, \
             population_unit_spikes, jitter_dt, population_unit_id, conductance, correlation, mod_file, \
             parameter_file, parameter_list, random_seed, cluster_size, cluster_spread, \
-            dendrite_location_override, input_generator, population_unit_fraction = args
+            dendrite_location_override, input_generator, population_unit_fraction, num_soma_synapses = args
 
             return self.make_input_helper_serial(neuron_id=neuron_id,
                                                  input_type=input_type,
                                                  freq=freq,
                                                  t_start=start,
                                                  t_end=end,
                                                  synapse_density=synapse_density,
@@ -2015,15 +2070,16 @@
                                                  parameter_file=parameter_file,
                                                  parameter_list=parameter_list,
                                                  random_seed=random_seed,
                                                  cluster_size=cluster_size,
                                                  cluster_spread=cluster_spread,
                                                  dendrite_location=dendrite_location_override,
                                                  input_generator=input_generator,
-                                                 population_unit_fraction=population_unit_fraction)
+                                                 population_unit_fraction=population_unit_fraction,
+                                                 num_soma_synapses=num_soma_synapses)
 
         except:
             import traceback
             tstr = traceback.format_exc()
             self.write_log(tstr, is_error=True)
             import pdb
             pdb.set_trace()
@@ -2053,15 +2109,16 @@
                                  parameter_file,
                                  parameter_list,
                                  random_seed,
                                  cluster_size=None,
                                  cluster_spread=None,
                                  dendrite_location=None,
                                  input_generator=None,
-                                 population_unit_fraction=1):
+                                 population_unit_fraction=1,
+                                 num_soma_synapses=0):
 
         """
         Generate poisson input.
 
         Args:
             neuron_id (int): Neuron ID to generate input for
             input_type: Input type
@@ -2080,14 +2137,16 @@
             parameter_list: Parameter list (to inline parameters, instead of reading from file)
             random_seed: Random seed.
             cluster_size: Input synapse cluster size
             cluster_spread: Spread of cluster along dendrite (in meters)
             dendrite_location: Override location of dendrites, list of (sec_id, sec_x) tuples.
             input_generator: "poisson" or "frequency_function"
             population_unit_fraction: Fraction of population unit spikes used, 1.0=all correlation within population unit, 0.0 = only correlation within the particular neuron
+            num_soma_synapses: How many additional synapses are placed on the soma
+
         """
 
     # First, find out how many inputs and where, based on morphology and
         # synapse density
 
         time_range = (t_start, t_end)
 
@@ -2123,22 +2182,29 @@
                 sec_id, sec_x = zip(*dendrite_location)
 
                 # TODO: Calculate the correct x,y,z and distance to soma
                 x = y = z = dist_to_soma = np.zeros((len(sec_id),))
                 input_loc = [(x, y, z), np.array(sec_id), np.array(sec_x), dist_to_soma]
 
             else:
+
                 # (x,y,z), secID, secX, dist_to_soma
                 input_loc = self.dendrite_input_locations(neuron_id=neuron_id,
                                                           synapse_density=synapse_density,
                                                           num_spike_trains=num_spike_trains,
                                                           rng=rng,
                                                           cluster_size=cluster_size,
                                                           cluster_spread=cluster_spread)
 
+                # If there are any soma synapses, update input_info with them
+                if num_soma_synapses > 0:
+                    input_loc = self.add_soma_synapses(input_loc,
+                                                       n_soma_synapses=num_soma_synapses,
+                                                       neuron_id=neuron_id)
+
             num_inputs = input_loc[0].shape[0]
 
             if num_inputs > 0:
                 # Rudolph, Michael, and Alain Destexhe. Do neocortical pyramidal neurons display stochastic resonance?.
                 # Journal of computational neuroscience 11.1(2001): 19 - 42.
                 # doi: https://doi.org/10.1023/A:1011200713411
                 p_keep = np.sqrt(correlation)
```

### Comparing `snudda-1.4.4/snudda/input/input_tuning.py` & `snudda-1.4.71/snudda/input/input_tuning.py`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/input/inspectinput.py` & `snudda-1.4.71/snudda/input/inspectinput.py`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/input/time_varying_input.py` & `snudda-1.4.71/snudda/input/time_varying_input.py`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/input/virtual_input.py` & `snudda-1.4.71/snudda/input/virtual_input.py`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/neuromodulation/modulation.py` & `snudda-1.4.71/snudda/neuromodulation/modulation.py`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/neuromodulation/modulation_network.py` & `snudda-1.4.71/snudda/neuromodulation/modulation_network.py`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/neuromodulation/modulation_synapse.py` & `snudda-1.4.71/snudda/neuromodulation/modulation_synapse.py`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/neuromodulation/neuromodulation.py` & `snudda-1.4.71/snudda/neuromodulation/neuromodulation.py`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/neuromodulation/neuromodulation_synapse.py` & `snudda-1.4.71/snudda/neuromodulation/neuromodulation_synapse.py`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/neurons/index_tree.py` & `snudda-1.4.71/snudda/neurons/index_tree.py`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/neurons/morphology_data.py` & `snudda-1.4.71/snudda/neurons/morphology_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,18 +13,14 @@
 
     """ Holds parent_id, children_id, points_id"""
 
     __slots__ = ["section_id", "parent_section_id", "parent_point_idx", "parent_section_type",
                  "child_section_id", "point_idx", "section_type",
                  "morphology_data", "neuron_id"]
 
-    # Använd numpy structured arrays? https://numpy.org/doc/stable/user/basics.rec.html
-    # Ta bort slots??
-    # Dataclass: https://stackoverflow.com/questions/35988/c-like-structures-in-python/45426493#45426493
-
     section_id: int
     parent_section_idx: int
     parent_point_idx: int
     parent_section_type: int
     child_section_id: np.ndarray  # First row is child_section_id, second row is child_section_type
     point_idx: np.ndarray
     section_type: int
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `snudda-1.4.4/snudda/neurons/neuron_model_extended.py` & `snudda-1.4.71/snudda/neurons/neuron_model_extended.py`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/neurons/neuron_morphology.py` & `snudda-1.4.71/snudda/neurons/neuron_morphology.py`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/neurons/neuron_morphology_extended.py` & `snudda-1.4.71/snudda/neurons/neuron_morphology_extended.py`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/neurons/neuron_prototype.py` & `snudda-1.4.71/snudda/neurons/neuron_prototype.py`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/place/create_cube_mesh.py` & `snudda-1.4.71/snudda/place/create_cube_mesh.py`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/place/create_slice_mesh.py` & `snudda-1.4.71/snudda/place/create_slice_mesh.py`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/place/place.py` & `snudda-1.4.71/snudda/place/place.py`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/place/projection_map_finder.py` & `snudda-1.4.71/snudda/place/projection_map_finder.py`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/place/region_mesh.py` & `snudda-1.4.71/snudda/place/region_mesh.py`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/place/rotation.py` & `snudda-1.4.71/snudda/place/rotation.py`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/place/volumetric_mapping.py` & `snudda-1.4.71/snudda/place/volumetric_mapping.py`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/plotting/Blender/io_mesh_swc/__init__.py` & `snudda-1.4.71/snudda/plotting/Blender/io_mesh_swc/__init__.py`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/plotting/Blender/io_mesh_swc/operator_swc_import.py` & `snudda-1.4.71/snudda/plotting/Blender/io_mesh_swc/operator_swc_import.py`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/plotting/Blender/visualisation/drawHyperCubeSomas.py` & `snudda-1.4.71/snudda/plotting/Blender/visualisation/drawHyperCubeSomas.py`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/plotting/Blender/visualisation/drawHyperCubeSomasRender.py` & `snudda-1.4.71/snudda/plotting/Blender/visualisation/drawHyperCubeSomasRender.py`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/plotting/Blender/visualisation/drawHyperCubeSomasWithLTS.py` & `snudda-1.4.71/snudda/plotting/Blender/visualisation/drawHyperCubeSomasWithLTS.py`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/plotting/Blender/visualisation/makeNeuronCube.py` & `snudda-1.4.71/snudda/plotting/Blender/visualisation/makeNeuronCube.py`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/plotting/Blender/visualisation/makeNeuronCubeSubset.py` & `snudda-1.4.71/snudda/plotting/Blender/visualisation/makeNeuronCubeSubset.py`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/plotting/Blender/visualisation/visualiseCubeOfNeuronsWhiteBackground.py` & `snudda-1.4.71/snudda/plotting/Blender/visualisation/visualiseCubeOfNeuronsWhiteBackground.py`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/plotting/Blender/visualisation/visualiseStriatumNeurons.py` & `snudda-1.4.71/snudda/plotting/Blender/visualisation/visualiseStriatumNeurons.py`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/plotting/Blender/visualisation/visualiseStriatumNeuronsWithSynapses.py` & `snudda-1.4.71/snudda/plotting/Blender/visualisation/visualiseStriatumNeuronsWithSynapses.py`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/plotting/Blender/visualisation/visualise_network.py` & `snudda-1.4.71/snudda/plotting/Blender/visualisation/visualise_network.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,19 +12,21 @@
 from snudda.utils.load_network_simulation import SnuddaLoadNetworkSimulation
 
 
 class VisualiseNetwork(object):
 
     # You need to provide neuron
     def __init__(self, network_path, blender_save_file=None, blender_output_image=None,
-                 network_json=None, simulation_output_file_name=None):
+                 network_json=None, simulation_output_file_name=None, use_neuron_cache=True):
 
         self.network_path = network_path
         self.snudda_data = get_snudda_data(network_path=network_path)
         self.scale_f = 1000  # factor to downscale the data
+        self.neuron_colour_lookup = dict()  # Allow the user to override the neuron colours
+        self.use_neuron_cache = use_neuron_cache
 
         if network_json:
             self.network_json = network_json
             self.network_file = None
         else:
             self.network_json = None
             self.network_file = os.path.join(network_path, "network-synapses.hdf5")
@@ -50,19 +52,31 @@
             self.data = self.sl.data
         elif self.network_json:
             from snudda.utils.fake_load import FakeLoad
             self.sl = FakeLoad()
             self.sl.import_json(self.network_json)
             self.data = self.sl.data
 
+    def set_neuron_colour(self, neuron_id, colour):
+
+        if len(colour) != 4:
+            raise ValueError(f"Colour should be R,G,B,alpha (4 values)")
+        self.neuron_colour_lookup[neuron_id] = colour
+
+    def clear_neuron_colours(self):
+
+        self.neuron_colour_lookup = dict()
+
     def visualise(self,
                   neuron_id=None,
                   blender_output_image=None,
                   white_background=True,
                   show_synapses=True,
+                  synapse_colour=None,
+                  synapse_pair_filter=None,
                   draw_meshes=True,
                   full_meshes=None,
                   camera_location=None,
                   camera_rotation=None,
                   camera_scale=None,
                   detail_level=1):
 
@@ -70,39 +84,44 @@
             Visualise network in blender.
 
             Args:
                 neuron_id (list) : Neuron ID to visualise, default None means all
                 blender_output_image
                 white_background
                 show_synapses
+                synapse_colour: R,G,B,alpha (For values, range 0-1). Default None.
+                synapse_pair_filter (list): List of pairs of neurons (tuples) to show synapses for, default None = no filtering
                 camera_location
                 camera_rotation
                 camera_scale
                 detail_level (int) : 1 = full morphologies, 2 = reduced morphologies, 3 = soma only
 
         """
 
-        if neuron_id:
+        if neuron_id is not None:
             neurons = [self.data["neurons"][x] for x in neuron_id]
         else:
             neurons = self.data["neurons"]
             neuron_id = self.data["neuronID"]
 
         if blender_output_image:
             self.blender_output_image = blender_output_image
 
         if camera_location is None:
-            camera_location = (2.98, 2.68, 4.96)
+            camera_location = (3.228, 4.3433, 7.6695)  # (2.98, 2.68, 4.96)
 
         if camera_rotation is None:
-            camera_rotation = (1.59, 0, -0.26)
+            camera_rotation = (94.1*(np.pi/180), 0, -103*(np.pi/180))  # (1.59, 0, -0.26)
 
         if camera_scale is None:
             camera_scale = (1, 1, 1)
 
+        if synapse_pair_filter is not None:
+            synapse_pair_filter = set(synapse_pair_filter)
+
         origo = self.data["simulationOrigo"]
         voxel_size = self.data["voxelSize"]
 
         # Remove the start cube
         VisualiseNetwork.clean_scene()
 
         # Add a light source
@@ -131,14 +150,22 @@
             bg.inputs[1].default_value = 1.0
             bpy.context.scene.view_settings.view_transform = 'Standard'
 
         else:
             bg.inputs[0].default_value[:3] = (0.0, 0.0, 0.0)
             bg.inputs[1].default_value = 0.0
 
+        #Scott's magic
+        '''
+        mat_dspn = bpy.data.materials.new("DSPN")
+        mat_dspn.use_nodes = True
+        mat_dspn.node_tree.nodes["Principled BSDF"].inputs[0].default_value = (0, 1, 0, 1)
+        mat_dspn.node_tree.nodes["Principled BSDF"].inputs['Alpha'].default_value = 1
+        '''
+        
         # Define materials
         mat_dspn = bpy.data.materials.new("PKHG")
         mat_dspn.diffuse_color = (77. / 255, 151. / 255, 1.0, 0.5)
         mat_ispn = bpy.data.materials.new("PKHG")
         mat_ispn.diffuse_color = (67. / 255, 55. / 255, 181. / 255, 0.5)
         mat_fs = bpy.data.materials.new("PKHG")
         mat_fs.diffuse_color = (6. / 255, 31. / 255, 85. / 255, 1.0)
@@ -175,64 +202,94 @@
                            "lts": mat_lts,
                            "snrneurons": mat_snr,
                            "proto": mat_proto,
                            "arky": mat_arky,
                            "synapse": mat_synapse,
                            "other": mat_other}
 
-        if white_background:
+        # Add the user requested custom colours
+        for nid in self.neuron_colour_lookup.keys():
+            material_lookup[nid] = bpy.data.materials.new(str(nid))
+            material_lookup[nid].use_nodes = True
+            material_lookup[nid].node_tree.nodes["Principled BSDF"].inputs[0].default_value = self.neuron_colour_lookup[nid]
+            material_lookup[nid].node_tree.nodes["Principled BSDF"].inputs['Alpha'].default_value = self.neuron_colour_lookup[nid][-1]
+                
+            #material_lookup[nid] = bpy.data.materials.new("PKHG")
+            #material_lookup[nid].diffuse_color = self.neuron_colour_lookup[nid]
+        
+        if synapse_colour is not None:
+            mat_synapse.diffuse_color = synapse_colour
+        elif white_background:
             mat_synapse.diffuse_color = (0.8, 0.0, 0.0, 1.0)
         else:
             mat_synapse.diffuse_color = (1.0, 1.0, 0.9, 1.0)
 
         # matSynapse.use_transparency = True
+
+        """
+        # We comment out these lines, to get the synapse colour to be set correctly (otherwise they are white)
+        # Thanks Scott for finding this fix.
+        
         mat_synapse.use_nodes = True
 
         if not white_background:
             emission_strength = 5.0
 
             # Make synapses glow
             emission = mat_synapse.node_tree.nodes.new('ShaderNodeEmission')
             emission.inputs['Strength'].default_value = emission_strength
 
             material_output = mat_synapse.node_tree.nodes.get('Material Output')
             mat_synapse.node_tree.links.new(material_output.inputs[0], emission.outputs[0])
+        """
 
-        for neuron in neurons:
+        for idx, neuron in enumerate(neurons):
 
             e_rot = mathutils.Matrix(neuron["rotation"].reshape(3, 3)).to_euler()
 
-            if neuron["name"] in self.neuron_cache:
+            if self.use_neuron_cache and neuron["name"] in self.neuron_cache:
                 # If we already have the object in memory, copy it.
                 obj = self.neuron_cache[neuron["name"]].copy()
 
                 if self.neuron_cache[neuron["name"]].data:
                     obj.data = self.neuron_cache[neuron["name"]].data.copy()
 
                 VisualiseNetwork.copy_children(self.neuron_cache[neuron["name"]], obj)
                 obj.animation_data_clear()
 
                 # Will return None if there is no obj named CUBe
                 obj.name = f"{neuron['name']}-{neuron['neuronID']}"
                 VisualiseNetwork.link_object(obj)
             else:
-                self.read_swc_data(filepath=snudda_parse_path(neuron["morphology"], self.snudda_data), detail_level=detail_level)
+                if type(detail_level) == np.ndarray:
+                    if len(detail_level) != len(neurons):
+                        raise ValueError(f"detail_level is either 1,2 or 3, "
+                                         f"if given as a array must be same length as number of neurons (ie {len(idx)}).")
+                    dl = detail_level[idx]
+                else:
+                    dl = detail_level
+
+                self.read_swc_data(filepath=snudda_parse_path(neuron["morphology"], self.snudda_data), detail_level=dl)
                 obj = bpy.context.selected_objects[0]
                 obj.name = f"{neuron['name']}-{neuron['neuronID']}"
 
                 self.neuron_cache[neuron["name"]] = obj
 
             obj.rotation_euler = e_rot
 
             print(f"Setting neuron {neuron['neuronID']} ({neuron['name']}) position: {neuron['position']}")
             obj.location = neuron["position"] * self.scale_f
 
             n_type = neuron["type"].lower()
 
-            if n_type in material_lookup:
+            if neuron['neuronID'] in material_lookup:
+                # Custom colour for neuron (priority)
+                mat = material_lookup[neuron['neuronID']]
+            elif n_type in material_lookup:
+                # Each neuron type has its own colour
                 mat = material_lookup[n_type]
             else:
                 mat = material_lookup["other"]
 
             if self.spike_times:
                 rest_color = mat.diffuse_color[:]
                 # if animating spike times we need to make a fresh material per neuron
@@ -283,14 +340,18 @@
                         # No synapses between pair
                         continue
 
                     for syn in synapses:
                         pre_id = syn[0]
                         post_id = syn[1]
 
+                        if synapse_pair_filter is not None:
+                            if (pre_id, post_id) not in synapse_pair_filter:
+                                continue
+
                         assert pre_id == vis_pre_id and post_id == vis_post_id  # Just sanity check, should be true
 
                         # Draw this neuron (the SWC import scales from micrometers to mm), the
                         # positions in the simulation are in meters, need to scale it to mm for
                         # blender to have same units.
                         x = (origo[0] + voxel_size * syn[2]) * self.scale_f
                         y = (origo[1] + voxel_size * syn[3]) * self.scale_f
```

### Comparing `snudda-1.4.4/snudda/plotting/Blender/visualisation/visualise_network_old.py` & `snudda-1.4.71/snudda/plotting/Blender/visualisation/visualise_network_old.py`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/plotting/Blender/visualisation/visualise_touch_detection.py` & `snudda-1.4.71/snudda/plotting/Blender/visualisation/visualise_touch_detection.py`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/plotting/plotLTSdensity.py` & `snudda-1.4.71/snudda/plotting/plotLTSdensity.py`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/plotting/plot_connection_matrix.py` & `snudda-1.4.71/snudda/plotting/plot_connection_matrix.py`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/plotting/plot_connectivity.py` & `snudda-1.4.71/snudda/plotting/plot_connectivity.py`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/plotting/plot_cross_correlogram.py` & `snudda-1.4.71/snudda/plotting/plot_cross_correlogram.py`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/plotting/plot_degeneration.py` & `snudda-1.4.71/snudda/plotting/plot_degeneration.py`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/plotting/plot_degeneration_and_growth.py` & `snudda-1.4.71/snudda/plotting/plot_degeneration_and_growth.py`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/plotting/plot_density.py` & `snudda-1.4.71/snudda/plotting/plot_density.py`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/plotting/plot_density_slice.py` & `snudda-1.4.71/snudda/plotting/plot_density_slice.py`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/plotting/plot_distance_statistics.py` & `snudda-1.4.71/snudda/plotting/plot_distance_statistics.py`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/plotting/plot_input.py` & `snudda-1.4.71/snudda/plotting/plot_input.py`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/plotting/plot_input_locations.py` & `snudda-1.4.71/snudda/plotting/plot_input_locations.py`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/plotting/plot_network.py` & `snudda-1.4.71/snudda/plotting/plot_network.py`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/plotting/plot_network_simulation.py` & `snudda-1.4.71/snudda/plotting/plot_network_simulation.py`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/plotting/plot_node_benchmark.py` & `snudda-1.4.71/snudda/plotting/plot_node_benchmark.py`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/plotting/plot_period_experiment.py` & `snudda-1.4.71/snudda/plotting/plot_period_experiment.py`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/plotting/plot_size_benchmark.py` & `snudda-1.4.71/snudda/plotting/plot_size_benchmark.py`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/plotting/plot_spike_raster_v2.py` & `snudda-1.4.71/snudda/plotting/plot_spike_raster_v2.py`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/plotting/plot_traces.py` & `snudda-1.4.71/snudda/plotting/plot_traces.py`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/simulate/model_current_injections.py` & `snudda-1.4.71/snudda/simulate/model_current_injections.py`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/simulate/network_pair_pulse_simulation.py` & `snudda-1.4.71/snudda/simulate/network_pair_pulse_simulation.py`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/simulate/nrn_simulator_parallel.py` & `snudda-1.4.71/snudda/simulate/nrn_simulator_parallel.py`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/simulate/pair_recording.py` & `snudda-1.4.71/snudda/simulate/pair_recording.py`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/simulate/save_network_recording.py` & `snudda-1.4.71/snudda/simulate/save_network_recording.py`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/simulate/simulate.py` & `snudda-1.4.71/snudda/simulate/simulate.py`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/utils/ablate_network.py` & `snudda-1.4.71/snudda/utils/ablate_network.py`

 * *Files 2% similar despite different names*

```diff
@@ -132,14 +132,17 @@
 
     def filter_synapses(self, data_type):
 
         """ Filters synapses, data_type is either 'synapses' or 'gapJunctions' """
 
         synapse_data = self.in_file[f"network/{data_type}"][()].copy()
 
+        if synapse_data.size == 0:
+            return np.array([], dtype=int)
+
         keep_flag = np.zeros((synapse_data.shape[0],), dtype=bool)
 
         # Shortcut, if user wants to remove all, skip the processing part
         if data_type == "synapses" and self.remove_all_synapses:
             return keep_flag  # All zero
         elif data_type == "gapJunctions" and self.remove_all_gap_junctions:
             return keep_flag
@@ -350,18 +353,23 @@
 
                 # We need to remap the neuronID if some neurons have been removed!!
                 row = gj_mat[row_idx, :]
                 row[0] = remap_id[row[0]]
                 row[1] = remap_id[row[1]]
                 temp_gj_mat[idx, :] = row
 
+            if temp_gj_mat.size > 0:
+                gj_chunk_size = self.in_file["network/gapJunctions"].chunks
+            else:
+                gj_chunk_size = None
+
             network_group.create_dataset("gapJunctions",
                                          data=temp_gj_mat,
                                          dtype=np.int32, shape=(num_gj, self.in_file["network/gapJunctions"].shape[1]),
-                                         chunks=self.in_file["network/gapJunctions"].chunks,
+                                         chunks=gj_chunk_size,
                                          maxshape=(None, self.in_file["network/gapJunctions"].shape[1]),
                                          compression=self.in_file["network/gapJunctions"].compression)
 
             print(f"{num_gj} / {num_gj} gap junction rows parsed")
             print("Gap junction matrix written.")
             print(f"Keeping {num_gj}  gap junctions (out of {gj_mat.shape[0]})")
```

### Comparing `snudda-1.4.4/snudda/utils/benchmark_logging.py` & `snudda-1.4.71/snudda/utils/benchmark_logging.py`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/utils/cleanup.py` & `snudda-1.4.71/snudda/utils/cleanup.py`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/utils/clone_neurons.py` & `snudda-1.4.71/snudda/utils/clone_neurons.py`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/utils/conv_hurt.py` & `snudda-1.4.71/snudda/utils/conv_hurt.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,26 +9,27 @@
 import numpy as np
 
 
 # TODO: This needs to be updated to match the latest SONATA release.
 
 class ConvHurt(object):
 
-    def __init__(self, simulation_structures, base_dir="TEST/", target_simulator="NEST"):
+    def __init__(self, simulation_structures, base_dir="TEST/", target_simulator="NEST", has_input=False):
 
         self.base_dir = base_dir
         self.network_dir = os.path.join(base_dir, 'networks')
+
         self.target_simulator = target_simulator
 
         self.h5py_libver = "earliest"  # "latest"
 
         self.setup_directories(base_dir=base_dir)
 
         self.write_main_config(simulation_structures=simulation_structures,
-                               base_dir=base_dir, target_simulator=target_simulator)
+                               base_dir=base_dir, target_simulator=target_simulator, has_input=has_input)
 
     ############################################################################
 
     @staticmethod
     def create_dir(directory):
 
         if not os.path.exists(directory):
@@ -61,15 +62,16 @@
     #
     # Writing the main configuration file, linking everything together
 
     def write_main_config(self,
                           base_dir="TEST/",
                           out_file="circuit_config.json",
                           simulation_structures=[],
-                          target_simulator="NEURON"):
+                          target_simulator="NEURON",
+                          has_input=False):
 
         config = OrderedDict([])
 
         config["target_simulator"] = target_simulator
 
         manifest = OrderedDict([("$BASE_DIR", "."),
                                 ("$NETWORK_DIR", "$BASE_DIR/networks"),
@@ -97,14 +99,23 @@
                          "node_types_file": os.path.join("$NETWORK_DIR", f"{ss}_node_types.csv") }
             nodes.append(node_info)
 
             edge_info = {"edges_file": os.path.join("$NETWORK_DIR", f"{ss}_edges.hdf5"),
                          "edge_types_file": os.path.join("$NETWORK_DIR", f"{ss}_edge_types.csv") }
             edges.append(edge_info)
 
+            if has_input:
+                node_info = {"nodes_file": os.path.join("$NETWORK_DIR", f"{ss}-input_nodes.hdf5"),
+                             "node_types_file": os.path.join("$NETWORK_DIR", f"{ss}-input_node_types.csv")}
+                nodes.append(node_info)
+
+                edge_info = {"edges_file": os.path.join("$NETWORK_DIR", f"{ss}-input_edges.hdf5"),
+                             "edge_types_file": os.path.join("$NETWORK_DIR", f"{ss}-input_edge_types.csv")}
+                edges.append(edge_info)
+
         config["networks"] = OrderedDict([("nodes", nodes), ("edges", edges)])
 
         with open(os.path.join(base_dir, out_file), 'wt') as f:
             json.dump(config, f, indent=4)
 
     ############################################################################
 
@@ -121,63 +132,73 @@
                     population_name,
                     node_id,
                     node_type_id,
                     node_group_id,
                     node_group_index,
                     data,
                     model_type=None,
-                    model_template=None):
-
-        with h5py.File(os.path.join(self.network_dir, node_file), 'w', libver=self.h5py_libver) as f:
+                    model_template=None,
+                    close_file=True):
 
+        if isinstance(node_file, h5py._hl.files.File):
+            f = node_file
+            n_group = f["nodes"]
+        else:
+            f = h5py.File(os.path.join(self.network_dir, node_file), 'w', libver=self.h5py_libver)
             self.add_version(f)
-
             n_group = f.create_group("nodes")
 
-            nodes_group = n_group.create_group(population_name)
+        print(f"Creating nodes/{population_name}")
+        nodes_group = n_group.create_group(population_name)
 
-            nodes_group.create_dataset("node_id", data=node_id)
-            nodes_group.create_dataset("node_type_id", data=node_type_id)
-            nodes_group.create_dataset("node_group_id", data=node_group_id)
-            nodes_group.create_dataset("node_group_index", data=node_group_index)
+        nodes_group.create_dataset("node_id", data=node_id)
+        nodes_group.create_dataset("node_type_id", data=node_type_id)
+        nodes_group.create_dataset("node_group_id", data=node_group_id)
+        nodes_group.create_dataset("node_group_index", data=node_group_index)
+
+        groups = np.unique(node_group_id)
+
+        for g in groups:
+            idx = np.where(node_group_id == g)
+
+            group_group = nodes_group.create_group(str(g))
+            # dynGroup = groupGroup.create_group("dynamics_params")
+
+            for data_type in data.keys():
+                # This assumes all our data is matrices
+                # if there are string data, we need to handle that separately
+                if len(data[data_type].shape) == 1:
+                    group_group.create_dataset(data_type, data=data[data_type][idx])
+                elif len(data[data_type].shape) == 2:
+                    group_group.create_dataset(data_type, data=data[data_type][idx, :])
+                else:
+                    print("Data has too many columns, require 1 or 2 columns max.")
 
-            groups = np.unique(node_group_id)
+            # These are optional, would overwrite the defaults in the CSV file
+            if model_type is not None and model_type != [None]:
+                # If this line fails, try to use .encode() on each element in the list
+                str_type = f"S{max([len(x) if x is not None else 1 for x in model_type[idx]])}"
 
-            for g in groups:
-                idx = np.where(node_group_id == g)
+                nodes_group.create_dataset("model_type", (len(idx),), str_type,
+                                           data=model_type[idx],
+                                           compression="gzip")
 
-                group_group = nodes_group.create_group(str(g))
-                # dynGroup = groupGroup.create_group("dynamics_params")
+            if model_template is not None and model_template != [None]:
+                assert model_type is not None, "model_type must be set if model_template set"
 
-                for data_type in data.keys():
-                    # This assumes all our data is matrices
-                    # if there are string data, we need to handle that separately
-                    if len(data[data_type].shape) == 1:
-                        group_group.create_dataset(data_type, data=data[data_type][idx])
-                    elif len(data[data_type].shape) == 2:
-                        group_group.create_dataset(data_type, data=data[data_type][idx, :])
-                    else:
-                        print("Data has too many columns, require 1 or 2 columns max.")
-
-                # These are optional, would overwrite the defaults in the CSV file
-                if model_type is not None and model_type != [None]:
-                    # If this line fails, try to use .encode() on each element in the list
-                    str_type = f"S{max([len(x) if x is not None else 1 for x in model_type[idx]])}"
-
-                    nodes_group.create_dataset("model_type", (len(idx),), str_type,
-                                               data=model_type[idx],
-                                               compression="gzip")
+                str_type2 = f"S{max([len(x) for x in model_template[idx]])}"
+                nodes_group.create_dataset("model_template", (len(idx),), str_type2, data=model_template[idx])
 
-                if model_template is not None and model_template != [None]:
-                    assert model_type is not None, "model_type must be set if model_template set"
+            # model_type_id should be added here also
 
-                    str_type2 = f"S{max([len(x) for x in model_template[idx]])}"
-                    nodes_group.create_dataset("model_template", (len(idx),), str_type2, data=model_template[idx])
+        if close_file:
+            f.close()
+            f = None
 
-                # model_type_id should be added here also
+        return f
 
     ############################################################################
 
     # node_csv_file is the name of the file that will be stored in the networks dir
     # node_type_id is the node type ID for each row
     # data is a dictionary, where each key corresponds to a column, and it must
     # contain a list of len(nodeTypeID).
@@ -218,15 +239,16 @@
 
     def write_edges(self,
                     edge_file,
                     population_rows,
                     edge_type_id,
                     source_id,
                     target_id,
-                    data):
+                    data,
+                    include_index=False):
 
         # We need to have the targetID vector sorted
         # How should we handle cells that do not have any edges at all?
         sort_idx = np.argsort(target_id)
 
         # EVERYTHING we write needs to use sort_idx (idx) so it is in the right order
         with h5py.File(os.path.join(self.network_dir, edge_file), 'w', libver=self.h5py_libver) as f:
@@ -236,15 +258,16 @@
 
             for pop_name, pop_rows in population_rows.items():
                 source_population_name, target_population_name = pop_name.split("_")
                 n_rows = len(pop_rows)
 
                 e_group = edg_group.create_group(pop_name)
 
-                idx = sort_idx[pop_rows]
+                sort_idx = np.argsort(target_id[pop_rows])
+                idx = pop_rows[sort_idx]
 
                 e_group.create_dataset("edge_group_id", data=np.zeros((n_rows,), dtype=int))
                 e_group.create_dataset("edge_group_index", data=np.arange(n_rows), dtype=int)
                 e_group.create_dataset("edge_type_id", data=edge_type_id[idx])
                 e_group.create_dataset("source_node_id", data=source_id[idx])
                 e_group.create_dataset("target_node_id", data=target_id[idx])
 
@@ -257,24 +280,27 @@
                     if len(data[data_type].shape) == 1:
                         group_group.create_dataset(data_type, data=data[data_type][idx])
                     elif len(data[data_type].shape) == 2:
                         group_group.create_dataset(data_type, data=data[data_type][idx, :])
                     else:
                         print("Unsupported width of data column.")
 
-                # We need to create the indices needed by Allen Institute
-                self.create_index(e_group["source_node_id"], e_group, index_source=True)
-                self.create_index(e_group["target_node_id"], e_group, index_source=False)
+                if include_index:
+                    # We need to create the indices needed by Allen Institute
+                    self.create_index(e_group["source_node_id"], e_group, index_source=True)
+                    self.create_index(e_group["target_node_id"], e_group, index_source=False)
 
     ############################################################################
 
     # createIndex provided by Kael Dai from Allen Institute, 2018-11-27
 
     def create_index(self, node_ids_ds, output_grp, index_source=0):
 
+        # TODO: Verify that this is correct! -- I am not sure it is...
+
         if not index_source:
             edge_nodes = np.array(node_ids_ds, dtype=np.int64)
             output_grp = output_grp.create_group('indices/target_to_source')
         else:
             edge_nodes = np.array(node_ids_ds, dtype=np.int64)
             output_grp = output_grp.create_group('indices/source_to_target')
 
@@ -341,31 +367,31 @@
                     else:
                         row.append(v[i])
 
                 csv_writer.writerow(row)
 
     ############################################################################
 
-    def write_input(self, spike_file_name, spikes):
-
-        if spikes is None:
-            print(f"No spikes specified, not writing {spike_file_name}")
-            print("Use python3 Network_input.py yourinput.json yournetwork.hdf5 input-spikes.hdf5")
-            return
+    def write_input(self, spike_file_name, spike_times, gids):
 
         f_name = os.path.join(self.base_dir, spike_file_name)
 
+        print(f"Writing spikes to {f_name}")
+
         with h5py.File(f_name, 'w', libver=self.h5py_libver) as f:
             self.add_version(f)
 
             print(f"Writing file {f_name}")
 
             s_group = f.create_group("spikes")
-            s_group.create_dataset("gids", data=spikes[:, 1])
-            s_group.create_dataset("timestamps", data=spikes[:, 0])
+            s_group.attrs["sorting"] = "gid"
+            s_group.create_dataset("gids", data=gids)
+            s_group.create_dataset("timestamps", data=spike_times*1e3)  # Convert to ms
+
+        return f_name
 
     ############################################################################
 
     # OBS, check that the files go in right directory
 
     def write_input_neurodamus(self, spike_file_name, spikes):
 
@@ -385,69 +411,7 @@
 
     ############################################################################
 
     def add_version(self, hdf5_file):
 
         hdf5_file.attrs["version"] = [0, 1]
         hdf5_file.attrs["magic"] = 0x0A7A
-
-
-if __name__ == "__main__":
-    # ch = ConvHurt()
-    # ch = ConvHurt(simulationStructure="cerebellum",
-    #              inputStructures=["pons","cortex"])
-
-    ch = ConvHurt(simulation_structure="striatum",
-                  input_structures=["cortex", "thalamus"])
-
-    # Test example, we have 5 neurons, big network
-    # two groups
-
-    node_data = {"positions": np.array([[1., 2., 3.], [4., 5., 6.], [7., 8., 9.],
-                                        [1., 8., 9.], [2., 3., 2.]]),
-                 "rotation_angle_zaxis": np.array([0.1, 0.2, 0.3, 0.4, 0.5])}
-
-    ch.write_nodes(node_file='striatum_nodes.hdf5',
-                   data=node_data,
-                   node_id=np.array([0, 1, 2, 3, 4]),
-                   population_name="striatum_nodes",
-                   node_type_id=np.array([0, 1, 0, 1, 0]),
-                   node_group_id=np.array([0, 0, 1, 1, 1]),
-                   node_group_index=np.array([0, 1, 0, 1, 2]))
-
-    node_type_id = np.array([0, 1])
-    node_data_csv = OrderedDict([('name', ['A', 'B']),
-                                 ('location', ['structA', 'structB'])])
-
-    ch.write_node_csv(node_csv_file='striatum_node_types.csv',
-                      node_type_id=node_type_id,
-                      data=node_data_csv)
-
-    edge_group = np.array([5, 5, 11, 11, 11])
-    edge_group_index = np.array([0, 1, 0, 1, 2])
-    edge_type_id = np.array([0, 1, 0, 1, 0])
-    source_gid = np.array([1, 2, 3, 3, 4])
-    target_gid = np.array([2, 3, 4, 0, 1])  # THESE ARE SORTED ... HAHAHA
-
-    # Delay needs to be in ms (bad bad people, real scientists use SI units)
-    edge_data = OrderedDict([("sec_id", np.array([10, 22, 33, 24, 15])),
-                             ("sec_x", np.array([0.1, 0.3, 0.5, 0.2, 0])),
-                             ("syn_weight", np.array([0.1e-9, 2e-9, 3e-9,
-                                                      0.3e-9, 0.1e-9])),
-                             ("delay", 1e3 * np.array([1e-3, 4e-3, 2e-3, 5e-3, 1e-3]))])
-
-    ch.write_edges(edge_file="striatum_edges.hdf5",
-                   edge_group=edge_group,
-                   edge_group_index=edge_group_index,
-                   edge_type_id=edge_type_id,
-                   edge_population_name="striatum_edges",
-                   source_id=source_gid,
-                   target_id=target_gid,
-                   data=edge_data)
-
-    edge_type_id = np.array([0, 1])
-    edge_csv_data = OrderedDict([('template', ['Exp2Syn', 'NULL']),
-                                 ('dynamics_params', ["mysyn.json", 'yoursyn.json'])])
-
-    ch.write_edges_csv(edge_csv_file="striatum_edge_types.csv",
-                       edge_type_id=edge_type_id,
-                       data=edge_csv_data)
```

### Comparing `snudda-1.4.4/snudda/utils/create_parameter_morphology_input_map.py` & `snudda-1.4.71/snudda/utils/create_parameter_morphology_input_map.py`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/utils/cut.py` & `snudda-1.4.71/snudda/utils/cut.py`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/utils/export_connection_matrix.py` & `snudda-1.4.71/snudda/utils/export_connection_matrix.py`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/utils/export_eroded_connection_matrix.py` & `snudda-1.4.71/snudda/utils/export_eroded_connection_matrix.py`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/utils/export_sonata.py` & `snudda-1.4.71/snudda/utils/export_sonata.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # This uses ConvHurt to convert the network created by Network_connect.py
 
 #
 # TODO:
+# - Add support for gap junctions
 # - Check what axon and dendrite propagation speeds should be
 #
 
 import json
 import os
 import sys
 from collections import OrderedDict
@@ -18,53 +19,82 @@
 from snudda.utils import snudda_parse_path
 from snudda.utils.conv_hurt import ConvHurt
 from snudda import SnuddaLoad
 
 
 class ExportSonata:
 
-    def __init__(self, network_file, input_file, out_dir, debug_flag=True, target_simulator="NEST"):
+    def __init__(self, network_path=None, network_file=None, input_file=None, out_dir=None, debug_flag=True, target_simulator="NEST"):
 
         self.debug = debug_flag
 
-        self.out_dir = out_dir
+        if network_path is not None:
+            self.network_path = network_path
+        elif network_file is not None:
+            self.network_path = os.path.dirname(network_file)
+        else:
+            raise ValueError("You must specify network_path or network_file")
+
+        if network_file is None:
+            network_file = os.path.join(network_path, "network-synapses.hdf5")
+
+        if out_dir is not None:
+            self.out_dir = out_dir
+        else:
+            self.out_dir = os.path.join(network_path, "SONATA")
+
         self.target_simulator = target_simulator
 
         # Read the data
         self.snudda_load = SnuddaLoad(network_file)
         self.network_file = self.snudda_load.network_file
-        self.input_file = input_file
+
+        if input_file is not None:
+            self.input_file = input_file
+        else:
+            input_file_candidate = os.path.join(self.network_path, "input-spikes.hdf5")
+
+            if os.path.isfile(input_file_candidate):
+                self.input_file = input_file_candidate
+            else:
+                self.input_file = None
 
         self.network_config = json.loads(self.snudda_load.data["config"])
 
-        print(f"Using input file: {self.input_file}")
+        if self.input_file:
+            print(f"Using input file: {self.input_file}")
+            has_input = True
+        else:
+            print("No input file specified, and default file not found.")
+            has_input = False
 
         # This contains data for converting to Neurodamus secID and secX
         self.morph_cache = dict([])
 
         self.morph_location_lookup = dict([])
         self.hoc_location_lookup = dict([])
 
         # Write the data in new format using the ConvHurt module
         # TODO: We need to read structure names from the network-config.json
         structure_names = [x for x in self.network_config["Volume"]]
         ch = ConvHurt(simulation_structures=structure_names,
-                      base_dir=out_dir)
+                      base_dir=self.out_dir, has_input=has_input)
 
         self.copy_morphologies()
         self.copy_mechanisms()
         self.copy_hoc()
 
         # Convert our rotation matrices to vx,vy,vz rotation angles
         # Neurodamus rotation order is first Z then Y and X.
         (vx, vy, vz) = self.rot_angles_zyx(self.snudda_load)
 
         # We need to convert the named neuron types to numbers
-        (node_type_id, node_type_id_lookup) = self.allocate_node_type_id()
-        (node_group_id, group_idx, node_group_lookup) = self.allocate_node_groups()
+        node_type_id, node_type_id_lookup = self.allocate_node_type_id()
+        # node_group_id, group_idx, node_group_lookup = self.allocate_node_groups()
+        node_group_id, group_idx, node_group_lookup, neuron_id_remap = self.allocate_groups_and_remap_nodeid()
 
         volume_id_list = [x["volumeID"] for x in self.snudda_load.data["neurons"]]
         volume_list = set(volume_id_list)
 
         # node_name_list = [x["name"] for x in self.snudda_load.data["neurons"]]
         node_name_list = [f"{n['name']}_{n['morphologyKey']}_{n['parameterKey']}_{n['modulationKey']}"
                           for n in self.snudda_load.data["neurons"]]
@@ -78,45 +108,73 @@
                     continue
                 else:
                     edge_type_id = con_type_data["channelModelID"]
 
                     if self.target_simulator == "NEST":
                         if "nestModelTemplate" in con_type_data["channelParameters"]:
                             edge_model = con_type_data["channelParameters"]["nestModelTemplate"]
+                            if "nestDynamicParams" not in con_type_data["channelParameters"]:
+                                raise KeyError("If nestModelTemplate is specified, nestDynamicParams must be specified also")
+                            dynamic_params = con_type_data["channelParameters"]["nestDynamicParams"]
                         else:
                             edge_model = "static_synapse"
+                            if con_type == "GABA":
+                                dynamic_params = "inhibitory.json"
+                            else:
+                                dynamic_params = "excitatory.json"
                     else:
                         edge_model = con_type_data["channelParameters"]["modFile"]
 
-                edge_type_lookup[pre_type, post_type, con_type] = (edge_type_id, edge_model)
+                edge_type_lookup[pre_type, post_type, con_type] = (edge_type_id, edge_model, f"{pre_type}_{post_type}", dynamic_params)
+
+        node_id_remap = np.full(shape=(self.snudda_load.data["nNeurons"],), fill_value=-1, dtype=int)
+        input_list = []
 
         for volume_name in volume_list:
-            v_idx = np.where([v == volume_name for v in volume_id_list])[0]
 
-            # Node data is stored in a HDF5 file and a CSV file (CONVERT TO micrometers)
-            node_data = OrderedDict([("x", self.snudda_load.data["neuronPositions"][v_idx, 0] * 1e6),
-                                     ("y", self.snudda_load.data["neuronPositions"][v_idx, 1] * 1e6),
-                                     ("z", self.snudda_load.data["neuronPositions"][v_idx, 2] * 1e6),
-                                     ("rotation_angle_zaxis", vz[v_idx]),
-                                     ("rotation_angle_yaxis", vy[v_idx]),
-                                     ("rotation_angle_xaxis", vx[v_idx])])
-
-            node_id_list = np.array([x["neuronID"] for x in self.snudda_load.data["neurons"]
-                                     if x["volumeID"] == "Striatum"], dtype=int)
-
-            assert (v_idx == node_id_list).all()
-
-            ch.write_nodes(node_file=f"{volume_name}_nodes.hdf5",
-                           population_name=volume_name,
-                           data=node_data,
-                           node_id=node_id_list,
-                           node_type_id=node_type_id[node_id_list],
-                           node_group_id=node_group_id[node_id_list],
-                           node_group_index=group_idx[node_id_list])
+            node_file = f"{volume_name}_nodes.hdf5"
+
+            for nt in self.snudda_load.get_neuron_types(return_set=True):
+                nt_idx = np.where([x["volumeID"] == volume_name and x["type"] == nt
+                                   for x in self.snudda_load.data["neurons"]])
+
+                # Node data is stored in a HDF5 file and a CSV file (CONVERT TO micrometers)
+                node_data = OrderedDict([("x", self.snudda_load.data["neuronPositions"][nt_idx, 0].flatten() * 1e6),
+                                         ("y", self.snudda_load.data["neuronPositions"][nt_idx, 1].flatten() * 1e6),
+                                         ("z", self.snudda_load.data["neuronPositions"][nt_idx, 2].flatten() * 1e6),
+                                         ("rotation_angle_zaxis", vz[nt_idx].flatten()),
+                                         ("rotation_angle_yaxis", vy[nt_idx].flatten()),
+                                         ("rotation_angle_xaxis", vx[nt_idx].flatten())])
+
+                node_id_list = np.array([x["neuronID"] for x in self.snudda_load.data["neurons"]
+                                         if x["volumeID"] == volume_name and x["type"] == nt], dtype=int)
+
+                assert (nt_idx == node_id_list).all()
+
+                new_node_id = np.arange(0, len(node_id_list))
+
+                assert (node_id_remap[node_id_list] == -1).all(), f"Node id already remapped!"
+                node_id_remap[node_id_list] = new_node_id
+
+                # Population name should be name of neuron type
+                node_file = ch.write_nodes(node_file=node_file,
+                                           population_name=nt,
+                                           data=node_data,
+                                           node_id=node_id_remap[node_id_list],
+                                           node_type_id=node_type_id[nt_idx],
+                                           node_group_id=node_group_id[nt_idx],
+                                           node_group_index=group_idx[nt_idx],
+                                           close_file=False)
+
+            node_file.close()
+            # Done writing hdf5 file, time to create csv file
 
+            assert (node_id_remap >= 0).all(), f"Not all node id remapped."
+
+            v_idx = np.where([v == volume_name for v in volume_id_list])[0]
             csv_node_names = sorted(list(set([node_name_list[x] for x in v_idx])))
             csv_node_type_id = [node_type_id_lookup[n] for n in csv_node_names]
             csv_node_location = [volume_name for n in csv_node_names]
 
             (model_template_list, model_type_list, morphology_list, dynamic_params) \
                 = self.get_node_templates(csv_node_names)
 
@@ -135,44 +193,161 @@
             ch.write_node_csv(node_csv_file=f"{volume_name}_node_types.csv",
                               node_type_id=csv_node_type_id,
                               data=node_data_csv)
 
             edge_population_lookup, edge_population_id_lookup = self.setup_edge_population(node_group_lookup)
 
             population_rows, edge_type_id, source_gid, target_gid, edge_data = \
-                self.setup_edge_info(edge_population_lookup, node_group_id)
+                self.setup_edge_info(edge_population_lookup, node_group_id, group_idx)
 
             ch.write_edges(edge_file=f"{volume_name}_edges.hdf5",
                            population_rows=population_rows,
                            edge_type_id=edge_type_id,
                            source_id=source_gid,
                            target_id=target_gid,
                            data=edge_data)
 
             edge_type_id = [x[0] for x in edge_type_lookup.values()]
 
-            edge_data = {"model_template": [x[1] for x in edge_type_lookup.values()]}
+            edge_data_csv = {"model_template": [x[1] for x in edge_type_lookup.values()],
+                             "population": [x[2] for x in edge_type_lookup.values()],
+                             "dynamic_params": [x[3] for x in edge_type_lookup.values()]}
 
             ch.write_edges_csv(edge_csv_file=f"{volume_name}_edge_types.csv",
                                edge_type_id=edge_type_id,
-                               data=edge_data)
+                               data=edge_data_csv)
+
+            if self.input_file:
+
+                (sonata_input_hdf5,
+                 sonata_virtual_node_hdf5, sonata_virtual_node_csv,
+                 sonata_virtual_edges_hdf5, sonata_virtual_edges_csv) = \
+                    self.write_input(node_id_remap=node_id_remap,
+                                     input_hdf5=self.input_file,
+                                     conv_hurt=ch, volume_name=volume_name)
 
-        # !!! WE ALSO NEED TO ADD BACKGROUND INPUT TO THE NEURONS IN THE NETWORK
+                input_list.append((volume_name, sonata_input_hdf5,
+                                   sonata_virtual_node_hdf5, sonata_virtual_node_csv,
+                                   sonata_virtual_edges_hdf5, sonata_virtual_edges_csv))
 
-        self.write_simulation_config()
+        # !!! TODO: We need to pass the new input files, node and edge files to the config
+        self.write_simulation_config(input_list=input_list)
 
-        print(f"SONATA files exported to {out_dir}")
+        print(f"SONATA files exported to {self.out_dir}")
 
     ############################################################################
 
-    def get_edge_type_lookup(self):
+    def get_all_input_types(self, input_hdf5, neuron_type=None, volume_name=None):
 
-        # Read the config file, to find out all possible types of connections
+        input_types = set()
 
-        pass
+        if type(input_hdf5) != h5py._hl.files.File:
+            input_hdf5 = h5py.File(input_hdf5, "r")
+
+        neuron_id_list = self.snudda_load.get_neuron_id_of_type(neuron_type=neuron_type, volume=volume_name)
+
+        for neuron_id in neuron_id_list:
+            neuron_input_types = set(input_hdf5[f"input/{neuron_id}"].keys())
+
+            input_types += neuron_input_types
+
+        return input_types
+
+    def write_input(self,
+                    input_hdf5,
+                    conv_hurt,
+                    node_id_remap,
+                    volume_name=None):
+
+        """
+            Args:
+                input_hdf5 : File to read data from
+                sonata_input_hdf5 : File to write data to
+                conv_hurt :
+                node_id_remap : Numpy array mapping neuron_id to gid (which is population specific)
+                volume_name (str) : Name of volume (default: None, assumes neuron type only in one volume)
+        """
+
+        # If there are N neurons in the volume, and they receive cortical and thalamic input
+        #
+        # Then...
+        # Virtual neuron 0-(N-1) provide cortical input to neurons 0-(N-1)
+        # Virtual neuron N-(2*N-1) provide thalamic input to neurons 0-(N-1)
+        #
+
+        if type(input_hdf5) != h5py._hl.files.File:
+            input_hdf5 = h5py.File(input_hdf5, "r")
+
+        sonata_input_hdf5 = f"inputs/input_{volume_name}.hdf5"
+
+        neuron_id_list = self.snudda_load.get_neuron_id_of_type(volume=volume_name, neuron_type=None)
+        input_data = []  # [(neuron_type, neuron_node_id, input_type, spikes, weight, virtual_node_id), (np, nid, it, s, w, vid), ...]
+
+        virtual_node_ctr = 0
+
+        for neuron_id in neuron_id_list:
+
+            for input_type in input_hdf5[f"input/{neuron_id}"].keys():
+                neuron_spikes = []
+
+                spike_group = input_hdf5[f"input/{neuron_id}/{input_type}/spikes"]
+                n_spikes = spike_group.attrs["nSpikes"]
+
+                for idx, ns in enumerate(n_spikes):
+                    neuron_spikes.append(spike_group[idx, :ns])
+
+                input_spikes = np.array(sorted(np.concatenate(neuron_spikes)))
+
+                neuron_type = self.snudda_load.data["neurons"][neuron_id]["type"]
+
+                weight = input_hdf5[f"input/{neuron_id}/{input_type}"].attrs["conductance"] * 1e6  # microsiemens for NEST
+                if "GABA" in input_hdf5[f"input/{neuron_id}/{input_type}"].attrs["modFile"].upper():
+                    weight *= -1
+
+                # [(neuron_type, neuron_node_id, input_type, spikes, weight, virtual_node_id), (np, nid, it, s, w, vid), ...]
+                input_data.append((neuron_type, node_id_remap[neuron_id], input_type, input_spikes, weight, virtual_node_ctr))
+                virtual_node_ctr += 1
+
+        # Next we need to write the input spikes to file
+        all_spikes = []
+        all_gid = []
+
+        for _, _, _, spikes, _, gid in input_data:
+            all_spikes.append(spikes)
+            all_gid.append(np.full(shape=spikes.shape, fill_value=gid, dtype=int))
+
+        spikes = np.concatenate(all_spikes)
+        gids = np.concatenate(all_gid)
+
+        if len(spikes) == 0:
+            return None
+
+        # We need to make sure the spikes are sorted by gid, then by time
+        idx = np.lexsort((spikes, gids))
+
+        f_name = conv_hurt.write_input(spike_file_name=sonata_input_hdf5,
+                                       spike_times=spikes[idx],
+                                       gids=gids[idx])
+
+        input_hdf5.close()
+
+        # We also need to create the virtual nodes, and edges to connect them
+
+        virtual_node_id = np.array([x[5] for x in input_data], dtype=int)
+        neuron_type = [x[0] for x in input_data]
+        node_id = np.array([x[1] for x in input_data], dtype=int)
+        weight = np.array([x[4] for x in input_data])
+
+        sonata_virtual_node_hdf5, sonata_virtual_node_csv, sonata_virtual_edges_hdf5, sonata_virtual_edges_csv = \
+            self.add_virtual_input(volume_name=volume_name, virtual_node_id=virtual_node_id,
+                                   neuron_type=neuron_type, node_id=node_id, weight=weight, conv_hurt=conv_hurt)
+
+        return (sonata_input_hdf5,
+                sonata_virtual_node_hdf5, sonata_virtual_node_csv,
+                sonata_virtual_edges_hdf5, sonata_virtual_edges_csv)
 
     ############################################################################
 
     def rot_mat_to_angles_xyz(self, rot_mat):
         # http://nghiaho.com/?page_id=846
 
         # This is for Rz*Ry*Rx
@@ -241,17 +416,19 @@
         # Since each neuron directory can have multiple morphology/parameter sets
         # we need to use the name + morphology_key + parameter_key + modulation_key
 
         node_type_id_lookup = OrderedDict([])
         next_node_type_id = 0
 
         node_names = [f"{n['name']}_{n['morphologyKey']}_{n['parameterKey']}_{n['modulationKey']}"
-                      for n in self.snudda_load.data["neurons"]]
+                             for n in self.snudda_load.data["neurons"]]
+
+        node_names_sorted = sorted(node_names)
 
-        for n in node_names:
+        for n in node_names_sorted:
             if n not in node_type_id_lookup:
                 node_type_id_lookup[n] = next_node_type_id
                 next_node_type_id += 1
 
         node_type_id = np.array([node_type_id_lookup[x] for x in node_names], dtype=int)
 
         return node_type_id, node_type_id_lookup
@@ -260,15 +437,18 @@
 
     # Comment from 2018, hope they support all now (guess we will find out):
     #  --> RT neuron only supports one group, so put everything in the same group
 
     # Snudda neuron type corresponds to SONATA NodeGroup
     # SONATA NodeType is {Snudda neuron name}_{morphology_key}_{parameter_key}_{modulation_key}
 
-    def allocate_node_groups(self):
+    def allocate_node_groups_OLD(self):
+
+        # node_group_id -- tells which group_id each neuron belongs to
+        # group_idx -- tells the index with the group that the neuron has
 
         node_group_id = np.zeros(len(self.snudda_load.data["neurons"]), dtype=int)
         group_idx = np.zeros(len(self.snudda_load.data["neurons"]), dtype=int)
         group_lookup = dict([])
 
         neuron_types = [n["type"] for n in self.snudda_load.data["neurons"]]
 
@@ -284,14 +464,63 @@
         for idx, nt in enumerate(neuron_types):
             node_group_id[idx] = group_lookup[nt]
             group_idx[idx] = next_group_idx[nt]
             next_group_idx[nt] += 1
 
         return node_group_id, group_idx, group_lookup
 
+    def allocate_groups_and_remap_nodeid(self):
+
+        n_neurons = self.snudda_load.data["nNeurons"]
+        volume_list = set([x["volumeID"] for x in self.snudda_load.data["neurons"]])
+        neuron_types = self.snudda_load.get_neuron_types(return_set=True)
+
+        node_group_id = np.zeros(shape=(n_neurons, ), dtype=int)
+        group_idx = np.full(shape=(n_neurons, ), fill_value=-1, dtype=int)
+        neuron_id_remap = np.full(shape=(n_neurons, ), fill_value=-1, dtype=int)
+
+        next_group = 0
+        group_lookup = dict()
+
+        for vol in volume_list:
+            for nt in neuron_types:
+                idx = self.snudda_load.get_neuron_id_of_type(neuron_type=nt, volume=vol)
+
+                group_lookup[vol, nt] = next_group
+                node_group_id[idx] = next_group
+                next_group += 1
+
+                assert (neuron_id_remap[idx] == -1).all(), f"Neuron id already remapped!"
+                neuron_id_remap[idx] = np.arange(0, len(idx))
+                group_idx[idx] = np.arange(0, len(idx))
+
+                # Originally we did not remap neuron id, but it seems that SONATA and NEST requires
+                # renumbering of the neuron_id to be consequent and starting from 0 for each group
+
+        assert (neuron_id_remap >= 0).all(), f"Not all neuron_id remapped!"
+
+        return node_group_id, group_idx, group_lookup, neuron_id_remap
+
+    def remap_nodes(self):
+
+        n_neurons = self.snudda_load.data["nNeurons"]
+        neuron_id_remap = np.full(shape=(n_neurons,), fill_value=-1)
+
+        neuron_types = self.snudda_load.get_neuron_types()
+        for nt in neuron_types:
+            old_id = self.snudda_load.get_neuron_id_of_type(neuron_type=nt)
+            new_id = np.arange(0, len(old_id))
+
+            assert (neuron_id_remap[old_id] == -1).all(), f"old_id already allocated!"
+            neuron_id_remap[old_id] = new_id
+
+        assert (neuron_id_remap >= 0).all(), f"Not all neuron_id remapped"
+
+        return neuron_id_remap
+
     ############################################################################
 
     def get_node_templates(self, csv_node_name):
 
         template_dict = dict([])
         model_type_dict = dict([])
         morphology_dict = dict([])
@@ -303,15 +532,15 @@
         for n in self.snudda_load.data["neurons"]:
             hoc_file = n["hoc"]
             name = f"{n['name']}_{n['morphologyKey']}_{n['parameterKey']}_{n['modulationKey']}"
 
             # It seems that RT neuron requires the filename without .swc at the end
             # Also, they prepend morphology path, but only allows one directory for all morphologies
             # morph_file = os.path.splitext(os.path.basename(n["morphology"]))[0]
-            morph_file = os.path.basename(n["morphology"])
+            morph_file = os.path.basename(n["morphology"]).replace(".swc", "")
 
             if hoc_file in self.hoc_location_lookup:
                 # We need to change from old hoc location to the SONATA hoc location
                 hoc_str = f"hoc:{os.path.basename(self.hoc_location_lookup[hoc_file])}"
             elif n["virtualNeuron"]:
                 hoc_str = "virtual"
             else:
@@ -332,15 +561,15 @@
                     model_type_dict[name] = "point_neuron"
                     dynamics_params_list.append(self.get_dynamics_params(n))
                     template_dict[name] = "aeif_cond_exp"
                 else:
                     model_type_dict[name] = "biophysical"
                     template_dict[name] = hoc_str
 
-            elif self.target_simulator is not "NEST":
+            elif self.target_simulator != "NEST":
 
                 assert template_dict[name] == hoc_str, \
                     f"All files named {name} do not share same hoc file: {template_dict[name]} and {hoc_str}"
 
         # Need to put them in the order in csvNodeName
 
         template_list = [template_dict[x] for x in csv_node_name]
@@ -357,15 +586,15 @@
 
         new_dynamics_params_list = []
         copied_files = []
 
         for file_path in dynamics_params_list:
 
             if file_path is None:
-                new_dynamics_params_list.append(None)
+                new_dynamics_params_list.append("MISSING-FILE-HERE.json")
                 continue
 
             if os.path.basename(file_path) == "dynamics_params.json":
                 dir_name = os.path.basename(os.path.dirname(file_path))
                 new_file = os.path.join(dest_path, f"{dir_name}_dynamics_params.json")
             else:
                 new_file = os.path.join(dest_path, os.path.basename(file_path))
@@ -380,27 +609,71 @@
 
     def setup_edge_population(self, node_group_lookup):
 
         edge_population_lookup = dict()
         edge_population_id_lookup = dict()
         next_id = 1
 
-        for pre_node_type, pre_node_group in node_group_lookup.items():
-            for post_node_type, post_node_group in node_group_lookup.items():
+        for (pre_volume, pre_node_type), pre_node_group in node_group_lookup.items():
+            for (post_volume, post_node_type), post_node_group in node_group_lookup.items():
+
+                if (pre_node_group, post_node_group) in edge_population_lookup:
+                    raise KeyError(f"{pre_node_group} to {post_node_group} connections occur in multiple volumes, "
+                                   f"please rename so neuron with specific name only occur in one volume")
+
                 edge_population_lookup[pre_node_group, post_node_group] = f"{pre_node_type}_{post_node_type}"
                 edge_population_id_lookup[pre_node_group, post_node_group] = next_id
                 next_id += 1
 
         return edge_population_lookup, edge_population_id_lookup
 
     ############################################################################
 
+    def get_nest_synapse_models(self):
+
+        synapse_model_lookup = dict()
+
+        for synapse_models in self.snudda_load.data["connectivityDistributions"].values():
+            for synapse_type, synapse_model in synapse_models.items():
+                synapse_type_id = synapse_model["channelModelID"]
+
+                if synapse_type == "GABA":
+                    synapse_model_lookup[synapse_type_id] = dict()
+                    synapse_model_lookup[synapse_type_id]["soma"] = "inhibitory_soma.json"
+                    synapse_model_lookup[synapse_type_id]["proximal"] = "inhibitory_proximal.json"
+                    synapse_model_lookup[synapse_type_id]["distal"] = "inhibitory_distal.json"
+                else:
+                    # Assume excitatory
+                    synapse_model_lookup[synapse_type_id] = dict()
+                    synapse_model_lookup[synapse_type_id]["soma"] = "excitatory_soma.json"
+                    synapse_model_lookup[synapse_type_id]["proximal"] = "excitatory_proximal.json"
+                    synapse_model_lookup[synapse_type_id]["distal"] = "excitatory_distal.json"
+
+        return synapse_model_lookup
+
+    def get_nest_synapse_sign_lookup(self):
+
+        synapse_sign_lookup = dict()
+
+        for synapse_models in self.snudda_load.data["connectivityDistributions"].values():
+            for synapse_type, synapse_model in synapse_models.items():
+                synapse_type_id = synapse_model["channelModelID"]
+
+                if synapse_type.upper() == "GABA":
+                    synapse_sign_lookup[synapse_type_id] = -1.0
+                else:
+                    synapse_sign_lookup[synapse_type_id] = 1.0
+
+        return synapse_sign_lookup
+
+    ############################################################################
+
     # This code sets up the info about edges
 
-    def setup_edge_info(self, edge_population_lookup, node_group_id):
+    def setup_edge_info(self, edge_population_lookup, node_group_id, group_idx):
 
         n_synapses = self.snudda_load.data["synapses"].shape[0]
         edge_type_id = np.zeros(n_synapses, dtype=int)
         source_gid = np.zeros(n_synapses, dtype=int)
         target_gid = np.zeros(n_synapses, dtype=int)
 
         population_rows = dict()  # For each population name, list all the synapse rows
@@ -415,44 +688,50 @@
         dend_speed = 1.0
 
         # columns in nl.data["synapses"]
         # 0: sourceCellID, 1: sourceComp, 2: destCellID, 3: destComp,
         # 4: locType, 5: synapseType, 6: somaDistDend 7:somaDistAxon
         # somaDist is an int, representing micrometers
 
+        synapse_sign_lookup = self.get_nest_synapse_sign_lookup()
+
         for i_syn, syn_row in enumerate(self.snudda_load.data["synapses"]):
-            source_gid[i_syn] = syn_row[0]
-            target_gid[i_syn] = syn_row[1]
+            source_gid[i_syn] = group_idx[syn_row[0]]
+            target_gid[i_syn] = group_idx[syn_row[1]]
 
             source_node_group = node_group_id[syn_row[0]]
             target_node_group = node_group_id[syn_row[1]]
 
             population_group = edge_population_lookup[source_node_group, target_node_group]
 
             if population_group in population_rows:
                 population_rows[population_group].append(i_syn)
             else:
                 population_rows[population_group] = [i_syn]
 
             sec_id[i_syn] = syn_row[9]
             sec_x[i_syn] = syn_row[10] / 1000.0
             synapse_type = syn_row[6]
+            synapse_conductance = syn_row[11] * 1e-3  # pS --> micro simens
+
+            # We need to set the weight to negative for inhibitory synapses it seems
+            # hence the synapse_sign_lookup (returns +1 or -1)
+            syn_weight[i_syn] = synapse_conductance * synapse_sign_lookup[synapse_type]
 
             pre_type = self.snudda_load.data["neurons"][source_gid[i_syn]]["type"]
             post_type = self.snudda_load.data["neurons"][target_gid[i_syn]]["type"]
 
             edge_type_id[i_syn] = synapse_type
 
             dend_dist = syn_row[6] * 1e-6
             axon_dist = syn_row[7] * 1e-6
-            delay[i_syn] = axon_dist / axon_speed + dend_dist / dend_speed
-            syn_weight[i_syn] = 1.0  # !!! THIS NEEDS TO BE SET DEPENDING ON CONNECTION TYPE
+            delay[i_syn] = axon_dist / axon_speed * 1e3 + 1  # Delay in ms and not SI units :-(
 
-        edge_data = OrderedDict([("sec_id", sec_id),
-                                 ("sec_x", sec_x),
+        edge_data = OrderedDict([("afferent_section_id", sec_id),
+                                 ("afferent_section_pos", sec_x),
                                  ("syn_weight", syn_weight),
                                  ("delay", delay)])
 
         for pop_name in population_rows.keys():
             population_rows[pop_name] = np.array(population_rows[pop_name])
 
         return population_rows, edge_type_id, source_gid, target_gid, edge_data
@@ -721,15 +1000,15 @@
         plt.ion()
         plt.show()
         plt.draw()
         plt.pause(0.001)
 
     ############################################################################
 
-    def write_simulation_config(self):
+    def write_simulation_config(self, input_list):
 
         sim_conf = dict([])
 
         sim_conf["manifest"] = {
             "$BASE_DIR": ".",
             "$NETWORK_DIR": "$BASE_DIR/networks",
             "$COMPONENT_DIR": "$BASE_DIR/components",
@@ -750,23 +1029,28 @@
         sim_conf["overwrite_output_dir"] = True
 
         sim_conf["network"] = "$BASE_DIR/circuit_config.json"
 
         # node_sets_file contains the reports we want written from the simulation
         # simConf["node_sets_file"] = None # !!! THIS NEEDS TO BE WRITTEN
 
-        cortex_input = {"input_type": "spikes",
-                        "module": "h5",
-                        "input_file": "$INPUT_DIR/cortexInput.hdf5"}
-
-        thalamus_input = {"input_type": "spikes",
-                          "module": "h5",
-                          "input_file": "$INPUT_DIR/thalamusInput.hdf5"}
-        sim_conf["inputs"] = {"cortexInput": cortex_input,
-                              "thalamusInput": thalamus_input}
+        if input_list:
+            sim_conf["inputs"] = dict()
+
+            for volume_name, sonata_input_hdf5, \
+                sonata_virtual_node_hdf5, sonata_virtual_node_csv, \
+                    sonata_virtual_edges_hdf5, sonata_virtual_edges_csv in input_list:
+
+                input_info = dict()
+                input_info["input_type"] = "spikes"
+                input_info["module"] = "h5"
+                input_info["input_file"] = f"$INPUT_DIR/{os.path.basename(sonata_input_hdf5)}"
+                input_info["node_set"] = f"{volume_name}-input"
+
+                sim_conf["inputs"][f"{volume_name}_spikes"] = input_info
 
         out_conf_file = os.path.join(self.out_dir, "simulation_config.json")
         print(f"Writing {out_conf_file}")
 
         with open(out_conf_file, 'wt') as f:
             json.dump(sim_conf, f, indent=4)
 
@@ -834,18 +1118,33 @@
         for mech in glob(os.path.join(mech_path, "*.mod")):
             if self.debug:
                 print(f"Copying {mech}")
 
             mech_file = os.path.basename(mech)
             copyfile(mech, os.path.join(self.out_dir, "components", "mechanisms", mech_file))
 
+    def copy_nest_synapses(self):
+        print("Copying NEST synapses")
+
+        mech_path = snudda_parse_path(os.path.join("$SNUDDA_DATA", "nest", "synapses"),
+                                      snudda_data=self.snudda_load.data["SnuddaData"])
+
+        for mech in glob(os.path.join(mech_path, "*.json")):
+            if self.debug:
+                print(f"Copying {mech}")
+
+            mech_file = os.path.basename(mech)
+            copyfile(mech, os.path.join(self.out_dir, "components", "synapse_dynamics", mech_file))
+
     ############################################################################
 
     def sort_input(self, nl, node_type_id_lookup, input_name=None):
 
+        raise DeprecationWarning("Code is deprecated")
+
         if self.input_file is None or not os.path.isfile(self.input_file):
             print("No input file has been specified!")
             return None
 
         max_input = 1000000
 
         input_mat = np.zeros((max_input, 2))
@@ -891,14 +1190,86 @@
         sort_idx = np.argsort(input_mat[:input_ctr, 0])
         input_matrix = input_mat[sort_idx, :]
 
         return input_matrix
 
         ############################################################################
 
+    def add_virtual_input(self, volume_name, virtual_node_id, neuron_type, node_id, weight, conv_hurt):
+
+        """ Creates one virtual neurons, to provide external input to that the neuron population
+
+            To know the target neuron, we need to know both neuron population, and node id within that population
+
+            Args:
+                volume_name (str): Name of volume
+                virtual_node_id (np.array): ID of all virtual nodes
+                neuron_type (list of str): Which population does each input target
+                node_id (np.array): ID of nodes that are connected
+                conv_hurt : ConvHurt object
+        """
+
+        virtual_neuron_population = f"{volume_name}-input"
+        virtual_node_file = f"{virtual_neuron_population}_nodes.hdf5"
+
+        n_virtual_nodes = len(virtual_node_id)
+        node_data = dict()  # Let's see if we get away without specifying coordinates
+        virtual_node_type_id = np.zeros(shape=(n_virtual_nodes, ), dtype=int)
+        virtual_node_group_id = np.zeros(shape=(n_virtual_nodes, ), dtype=int)
+        virtual_node_group_index = np.arange(0, n_virtual_nodes, dtype=int)
+
+        conv_hurt.write_nodes(node_file=virtual_node_file,
+                              population_name=virtual_neuron_population,
+                              data=node_data,
+                              node_id=virtual_node_id,
+                              node_type_id=virtual_node_type_id,
+                              node_group_id=virtual_node_group_id,
+                              node_group_index=virtual_node_group_index,
+                              close_file=True)
+
+        csv_virtual_node_types_file = f"{virtual_neuron_population}_node_types.csv"
+
+        virtual_node_data_csv = OrderedDict([("model_type", ["virtual"])])
+        conv_hurt.write_node_csv(node_csv_file=csv_virtual_node_types_file,
+                                 node_type_id=[0],
+                                 data=virtual_node_data_csv)
+
+        edge_file = f"{virtual_neuron_population}_edges.hdf5"
+
+        population_rows = dict()
+
+        # We need to write separate sets of edges for each targeted population
+        for nrn_type in set(neuron_type):
+            population_rows[f"{volume_name}-input_{nrn_type}"] = \
+                np.array([i for (i, val) in enumerate(neuron_type) if val == nrn_type], dtype=int)
+            # population_rows[nrn_type] = np.where(np.array(neuron_type) == nrn_type)[0]
+
+        edge_data = {"syn_weight": weight}
+
+        conv_hurt.write_edges(edge_file=edge_file,
+                              population_rows=population_rows,
+                              edge_type_id=np.zeros(len(virtual_node_id), dtype=int),
+                              source_id=virtual_node_id,
+                              target_id=node_id,
+                              data=edge_data)
+
+        edge_types_file_csv = f"{virtual_neuron_population}_edge_types.csv"
+        edge_type_id = np.array([0])
+        edge_data_csv = {"model_template": ["static_synapse"]}
+
+        conv_hurt.write_edges_csv(edge_csv_file=edge_types_file_csv,
+                                  edge_type_id=edge_type_id,
+                                  data=edge_data_csv)
+
+        return virtual_node_file, csv_virtual_node_types_file, edge_file, edge_types_file_csv
+
+    def add_edges_for_virtual_neurons_input(self):
+
+        pass
+
     ############################################################################
 
 
 if __name__ == "__main__":
 
     if len(sys.argv) > 1:
         networkFile = sys.argv[1]
```

### Comparing `snudda-1.4.4/snudda/utils/fake_load.py` & `snudda-1.4.71/snudda/utils/fake_load.py`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/utils/load.py` & `snudda-1.4.71/snudda/utils/load.py`

 * *Files 0% similar despite different names*

```diff
@@ -731,30 +731,32 @@
             return neuron_types
 
     ############################################################################
 
     # Returns neuron_id of all neurons of neuron_type
     # OBS, random_permute is not using a controled rng, so not affected by random seed set
 
-    def get_neuron_id_of_type(self, neuron_type, num_neurons=None, random_permute=False):
+    def get_neuron_id_of_type(self, neuron_type, num_neurons=None, random_permute=False, volume=None):
 
         """
         Find all neuron ID of a specific neuron type.
 
         Args:
             neuron_type (string) : Neuron type (e.g. "FS")
             num_neurons (int) : Maximum number of neurons to return
             random_permute (bool) : Shuffle the resulting neuron IDs?
+            volume (string) : VolumeID containing neurons (default None -- all neurons of type)
 
         Returns:
             List of neuron ID of specified neuron type
 
         """
 
-        neuron_id = np.array([x["neuronID"] for x in self.data["neurons"] if x["type"] == neuron_type])
+        neuron_id = np.array([x["neuronID"] for x in self.data["neurons"]
+                              if (neuron_type is None or x["type"] == neuron_type) and (volume is None or x["volumeID"] == volume)])
 
         assert not random_permute or num_neurons is not None, "random_permute is only valid when num_neurons is given"
 
         if num_neurons is not None:
             if random_permute:
                 # Do not use this if you have a simulation with multiple
                 # workers... they might randomize differently, and you might
@@ -769,16 +771,17 @@
                 neuron_id = neuron_id[:num_neurons]
 
             if len(neuron_id) < num_neurons:
                 if self.verbose:
                     print(f"get_neuron_id_of_type: wanted {num_neurons} only got {len(neuron_id)} "
                           f"neurons of type {neuron_type}")
 
-        # Double check that all of the same type
-        assert np.array([self.data["neurons"][x]["type"] == neuron_type for x in neuron_id]).all()
+        # Double check that all of the same type (or neuron_type is None)
+        assert neuron_type is None or np.array([self.data["neurons"][x]["type"] == neuron_type for x in neuron_id]).all()
+        assert volume is None or np.array([self.data["neurons"][x]["volumeID"] == volume for x in neuron_id]).all()
 
         return neuron_id
 
     def get_neuron_id(self):
 
         neuron_id = np.array([x["neuronID"] for x in self.data["neurons"]])
 
@@ -926,24 +929,26 @@
         gj_coords = gap_junctions[:, 6:9][:gj_ctr, :] * self.data["voxelSize"] + self.data["simulationOrigo"]
 
         if return_index:
             return gap_junctions[:gj_ctr, :], gj_coords, gj_index_list[:gj_ctr]
         else:
             return gap_junctions[:gj_ctr, :], gj_coords
 
-    def get_centre_neurons_iterator(self, n_neurons=None, neuron_type=None, centre_point=None, max_distance=None):
+    def get_centre_neurons_iterator(self, n_neurons=None, neuron_type=None, centre_point=None, max_distance=None,
+                                    return_distance=True):
 
         """ Return neuron id:s, starting from the centre most and moving outwards
 
         Args:
             n_neurons (int) : Number of neurons to return, None = all available
             neuron_type (str) : Type of neurons to return, None = all available
             centre_point (np.array) : x,y,z of centre position, None = auto detect centre
         """
 
+
         if centre_point is None:
             centre_point = np.mean(self.data["neuronPositions"], axis=0)
 
         dist_to_centre = np.linalg.norm(self.data["neuronPositions"] - centre_point, axis=-1)
         idx = np.argsort(dist_to_centre)
 
         neuron_ctr = 0
@@ -952,29 +957,33 @@
             if neuron_type is not None and self.data["neurons"][neuron_id]["type"] != neuron_type:
                 continue
 
             if max_distance is not None and dist_to_centre[neuron_id] > max_distance:
                 # Stop iterator if max distance is reached
                 return
 
-            yield neuron_id, dist_to_centre[neuron_id]
+            if return_distance:
+                yield neuron_id, dist_to_centre[neuron_id]
+            else:
+                yield neuron_id
+
             neuron_ctr += 1
 
             if n_neurons is not None and neuron_ctr >= n_neurons:
                 # Stop iterator if n_neurons are delivered
                 return
 
     ############################################################################
 
     def create_connection_matrix(self, sparse_matrix=True):
 
         if sparse_matrix:
-            connection_matrix = sparse.lil_matrix((self.data["nNeurons"], self.data["nNeurons"]), dtype=np.ushort)
+            connection_matrix = sparse.lil_matrix((self.data["nNeurons"], self.data["nNeurons"]), dtype=np.int16)
         else:
-            connection_matrix = np.zeros((self.data["nNeurons"], self.data["nNeurons"]), dtype=np.ushort)
+            connection_matrix = np.zeros((self.data["nNeurons"], self.data["nNeurons"]), dtype=np.int16)
 
         for syn_row in self.data["synapses"]:
             connection_matrix[syn_row[0], syn_row[1]] += 1
 
         return connection_matrix
 
     def create_distance_matrix(self, neuron_id=None, pre_id=None, post_id=None):
```

### Comparing `snudda-1.4.4/snudda/utils/load_network_simulation.py` & `snudda-1.4.71/snudda/utils/load_network_simulation.py`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/utils/merge_synapse_files.py` & `snudda-1.4.71/snudda/utils/merge_synapse_files.py`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/utils/numpy_encoder.py` & `snudda-1.4.71/snudda/utils/numpy_encoder.py`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/utils/reposition_neurons.py` & `snudda-1.4.71/snudda/utils/reposition_neurons.py`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/utils/snudda_path.py` & `snudda-1.4.71/snudda/utils/snudda_path.py`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/utils/swap_to_degenerated_morphologies.py` & `snudda-1.4.71/snudda/utils/swap_to_degenerated_morphologies.py`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/utils/swap_to_degenerated_morphologies_extended.py` & `snudda-1.4.71/snudda/utils/swap_to_degenerated_morphologies_extended.py`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda/utils/upgrade_old_network_file.py` & `snudda-1.4.71/snudda/utils/upgrade_old_network_file.py`

 * *Files identical despite different names*

### Comparing `snudda-1.4.4/snudda.egg-info/PKG-INFO` & `snudda-1.4.71/snudda.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snudda
-Version: 1.4.4
+Version: 1.4.71
 Summary: Create realistic networks of neurons, synapses placed using touch detection between axons and dendrites.
 Home-page: https://github.com/Hjorthmedh/Snudda
 Author: Johannes Hjorth
 Author-email: hjorth@kth.se
 License: GPLv3
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -18,15 +18,15 @@
 
 ## Contact details
 Johannes Hjorth, Royal Institute of Technology (KTH)
 Human Brain Project
 hjorth@kth.se
 
 ## Funding
-Horizon 2020 Framework Programme (785907, HBP SGA2); Horizon 2020 Framework Programme (945539, HBP SGA3); Vetenskapsrådet (VR-M-2017-02806, VR-M-2020-01652); Swedish e-science Research Center (SeRC); KTH Digital Futures. The computations are enabled by resources provided by the Swedish National Infrastructure for Computing (SNIC) at PDC KTH partially funded by the Swedish Research Council through grant agreement no. 2018-05973. We acknowledge the use of Fenix Infrastructure resources, which are partially funded from the European Union's Horizon 2020 research and innovation programme through the ICEI project under the grant agreement No. 800858.
+Horizon 2020 Framework Programme (785907, HBP SGA2); Horizon 2020 Framework Programme (945539, HBP SGA3); Vetenskapsrådet (VR-M-2017-02806, VR-M-2020-01652); Swedish e-science Research Center (SeRC); KTH Digital Futures. The computations are enabled by resources provided by the Swedish National Infrastructure for Computing (SNIC) at PDC KTH partially funded by the Swedish Research Council through grant agreement no. 2018-05973. We acknowledge the use of Fenix Infrastructure resources, which are partially funded from the European Union's Horizon 2020 research and innovation programme through the ICEI project under the grant agreement No. 800858. Snudda is supported and featured on EBRAINS.
 
 ## Citation
 Please cite the first paper for the general Snudda network creation and simulation methods, and the second paper for the Striatal microcircutiry model.
 
 * *Predicting Synaptic Connectivity for Large-Scale Microcircuit Simulations Using Snudda.* J. J. Johannes Hjorth, Jeanette Hellgren Kotaleski, Alexander Kozlov. Neuroinform (2021). https://doi.org/10.1007/s12021-021-09531-w
 
 * *The microcircuits of striatum in silico.* J. J. Johannes Hjorth, Alexander Kozlov, Ilaria Carannante, Johanna Frost Nylén, Robert Lindroos, Yvonne Johansson, Anna Tokarska, Matthijs C. Dorst, Shreyas M. Suryanarayana, Gilad Silberberg, Jeanette Hellgren Kotaleski, Sten Grillner. Proceedings of the National Academy of Sciences (2020). https://doi.org/10.1073/pnas.2000671117
```

### Comparing `snudda-1.4.4/snudda.egg-info/SOURCES.txt` & `snudda-1.4.71/snudda.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -76,14 +76,22 @@
 snudda/data/mesh/Striatum-dorsal-left-hemisphere.obj
 snudda/data/mesh/Striatum-dorsal-right-hemisphere.obj
 snudda/data/mesh/Striatum-v.obj
 snudda/data/mesh/get_mesh.ipynb
 snudda/data/nest/models/FS.json
 snudda/data/nest/models/dSPN.json
 snudda/data/nest/models/iSPN.json
+snudda/data/nest/synapses/excitatory.json
+snudda/data/nest/synapses/excitatory_distal.json
+snudda/data/nest/synapses/excitatory_proximal.json
+snudda/data/nest/synapses/excitatory_soma.json
+snudda/data/nest/synapses/inhibitory.json
+snudda/data/nest/synapses/inhibitory_distal.json
+snudda/data/nest/synapses/inhibitory_proximal.json
+snudda/data/nest/synapses/inhibitory_soma.json
 snudda/data/neurons/mechanisms/Im_ms.mod
 snudda/data/neurons/mechanisms/Kv3_ch.mod
 snudda/data/neurons/mechanisms/NO.mod
 snudda/data/neurons/mechanisms/bk_ch.mod
 snudda/data/neurons/mechanisms/bk_fs.mod
 snudda/data/neurons/mechanisms/bk_ms.mod
 snudda/data/neurons/mechanisms/ca_ch.mod
```

