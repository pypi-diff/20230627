# Comparing `tmp/siriuspy-2.76.1.tar.gz` & `tmp/siriuspy-2.77.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "siriuspy-2.76.1.tar", last modified: Tue Jun 20 14:19:46 2023, max compression
+gzip compressed data, was "siriuspy-2.77.0.tar", last modified: Tue Jun 27 19:16:13 2023, max compression
```

## Comparing `siriuspy-2.76.1.tar` & `siriuspy-2.77.0.tar`

### file list

```diff
@@ -1,395 +1,396 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 14:19:46.874279 siriuspy-2.76.1/
--rw-r--r--   0 runner    (1001) docker     (122)    34494 2023-06-20 14:19:38.000000 siriuspy-2.76.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       90 2023-06-20 14:19:38.000000 siriuspy-2.76.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     1423 2023-06-20 14:19:46.870279 siriuspy-2.76.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      954 2023-06-20 14:19:38.000000 siriuspy-2.76.1/README.md
--rw-r--r--   0 runner    (1001) docker     (122)      128 2023-06-20 14:19:38.000000 siriuspy-2.76.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-20 14:19:46.874279 siriuspy-2.76.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (122)     1243 2023-06-20 14:19:38.000000 siriuspy-2.76.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 14:19:46.826279 siriuspy-2.76.1/siriuspy/
--rw-r--r--   0 runner    (1001) docker     (122)        7 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/VERSION
--rw-r--r--   0 runner    (1001) docker     (122)      515 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 14:19:46.826279 siriuspy-2.76.1/siriuspy/bsmp/
--rw-r--r--   0 runner    (1001) docker     (122)      422 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/bsmp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    15885 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/bsmp/commands.py
--rw-r--r--   0 runner    (1001) docker     (122)     1904 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/bsmp/constants.py
--rw-r--r--   0 runner    (1001) docker     (122)    11790 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/bsmp/entities.py
--rw-r--r--   0 runner    (1001) docker     (122)      610 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/bsmp/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)     8110 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/bsmp/serial.py
--rw-r--r--   0 runner    (1001) docker     (122)     1204 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/bsmp/types.py
--rw-r--r--   0 runner    (1001) docker     (122)     2992 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/callbacks.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 14:19:46.826279 siriuspy-2.76.1/siriuspy/clientarch/
--rw-r--r--   0 runner    (1001) docker     (122)      306 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/clientarch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    13813 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/clientarch/client.py
--rw-r--r--   0 runner    (1001) docker     (122)     6392 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/clientarch/devices.py
--rw-r--r--   0 runner    (1001) docker     (122)      643 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/clientarch/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)    20400 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/clientarch/pvarch.py
--rw-r--r--   0 runner    (1001) docker     (122)     5003 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/clientarch/time.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 14:19:46.826279 siriuspy-2.76.1/siriuspy/clientconfigdb/
--rw-r--r--   0 runner    (1001) docker     (122)      227 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/clientconfigdb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3345 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/clientconfigdb/_templates.py
--rw-r--r--   0 runner    (1001) docker     (122)     9599 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/clientconfigdb/configdb_client.py
--rw-r--r--   0 runner    (1001) docker     (122)     5448 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/clientconfigdb/configdb_document.py
--rw-r--r--   0 runner    (1001) docker     (122)     4785 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/clientconfigdb/pvsconfig.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 14:19:46.830278 siriuspy-2.76.1/siriuspy/clientconfigdb/types/
--rw-r--r--   0 runner    (1001) docker     (122)      286 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/clientconfigdb/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    13746 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/clientconfigdb/types/as_corrloop_params.py
--rw-r--r--   0 runner    (1001) docker     (122)    57636 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/clientconfigdb/types/as_diagnostics.py
--rw-r--r--   0 runner    (1001) docker     (122)     6681 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/clientconfigdb/types/as_pwrstate.py
--rw-r--r--   0 runner    (1001) docker     (122)    34247 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/clientconfigdb/types/as_rf.py
--rw-r--r--   0 runner    (1001) docker     (122)     1135 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/clientconfigdb/types/bo_chromcorr_params.py
--rw-r--r--   0 runner    (1001) docker     (122)     3984 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/clientconfigdb/types/bo_normalized.py
--rw-r--r--   0 runner    (1001) docker     (122)     1135 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/clientconfigdb/types/bo_orbcorr_respm.py
--rw-r--r--   0 runner    (1001) docker     (122)      700 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/clientconfigdb/types/bo_orbit.py
--rw-r--r--   0 runner    (1001) docker     (122)     3042 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/clientconfigdb/types/bo_ramp.py
--rw-r--r--   0 runner    (1001) docker     (122)      975 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/clientconfigdb/types/bo_tunecorr_params.py
--rw-r--r--   0 runner    (1001) docker     (122)   123230 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/clientconfigdb/types/global_config.py
--rw-r--r--   0 runner    (1001) docker     (122)      735 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/clientconfigdb/types/si_bbadata.py
--rw-r--r--   0 runner    (1001) docker     (122)    18619 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/clientconfigdb/types/si_bbbproc.py
--rw-r--r--   0 runner    (1001) docker     (122)     1697 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/clientconfigdb/types/si_chromcorr_params.py
--rw-r--r--   0 runner    (1001) docker     (122)     1146 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/clientconfigdb/types/si_fastorbcorr_respm.py
--rw-r--r--   0 runner    (1001) docker     (122)     4741 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/clientconfigdb/types/si_fofb.py
--rw-r--r--   0 runner    (1001) docker     (122)      957 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/clientconfigdb/types/si_id.py
--rw-r--r--   0 runner    (1001) docker     (122)     3181 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/clientconfigdb/types/si_idff.py
--rw-r--r--   0 runner    (1001) docker     (122)     1136 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/clientconfigdb/types/si_orbcorr_respm.py
--rw-r--r--   0 runner    (1001) docker     (122)      701 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/clientconfigdb/types/si_orbit.py
--rw-r--r--   0 runner    (1001) docker     (122)     1290 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/clientconfigdb/types/si_tunecorr_params.py
--rw-r--r--   0 runner    (1001) docker     (122)     1738 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/clientconfigdb/types/tb_normalized.py
--rw-r--r--   0 runner    (1001) docker     (122)      969 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/clientconfigdb/types/tb_orbcorr_respm.py
--rw-r--r--   0 runner    (1001) docker     (122)      693 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/clientconfigdb/types/tb_orbit.py
--rw-r--r--   0 runner    (1001) docker     (122)     1651 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/clientconfigdb/types/tb_posang_respm.py
--rw-r--r--   0 runner    (1001) docker     (122)      969 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/clientconfigdb/types/ts_orbcorr_respm.py
--rw-r--r--   0 runner    (1001) docker     (122)      693 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/clientconfigdb/types/ts_orbit.py
--rw-r--r--   0 runner    (1001) docker     (122)     1721 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/clientconfigdb/types/ts_posang_respm.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 14:19:46.830278 siriuspy-2.76.1/siriuspy/clientweb/
--rw-r--r--   0 runner    (1001) docker     (122)       50 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/clientweb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5896 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/clientweb/implementation.py
--rw-r--r--   0 runner    (1001) docker     (122)     2236 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/csdev.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 14:19:46.830278 siriuspy-2.76.1/siriuspy/currinfo/
--rw-r--r--   0 runner    (1001) docker     (122)      144 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/currinfo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     9620 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/currinfo/csdev.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 14:19:46.830278 siriuspy-2.76.1/siriuspy/currinfo/lifetime/
--rw-r--r--   0 runner    (1001) docker     (122)       72 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/currinfo/lifetime/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    12607 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/currinfo/lifetime/main.py
--rw-r--r--   0 runner    (1001) docker     (122)    23275 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/currinfo/main.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 14:19:46.830278 siriuspy-2.76.1/siriuspy/cycle/
--rw-r--r--   0 runner    (1001) docker     (122)      514 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/cycle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)   104994 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/cycle/bo_cycle_data.py
--rw-r--r--   0 runner    (1001) docker     (122)    31135 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/cycle/conn.py
--rw-r--r--   0 runner    (1001) docker     (122)     9781 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/cycle/fc_cycle_data.py
--rw-r--r--   0 runner    (1001) docker     (122)     3286 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/cycle/li_cycle_data.py
--rw-r--r--   0 runner    (1001) docker     (122)    38408 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/cycle/main.py
--rw-r--r--   0 runner    (1001) docker     (122)     3574 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/cycle/util.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 14:19:46.834278 siriuspy-2.76.1/siriuspy/devices/
--rw-r--r--   0 runner    (1001) docker     (122)     1784 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/devices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    48546 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/devices/bbb.py
--rw-r--r--   0 runner    (1001) docker     (122)     2786 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/devices/blctrl.py
--rw-r--r--   0 runner    (1001) docker     (122)    41475 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/devices/bpm.py
--rw-r--r--   0 runner    (1001) docker     (122)     7380 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/devices/currinfo.py
--rw-r--r--   0 runner    (1001) docker     (122)     2402 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/devices/dcct.py
--rw-r--r--   0 runner    (1001) docker     (122)    13949 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/devices/device.py
--rw-r--r--   0 runner    (1001) docker     (122)    16522 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/devices/dvf.py
--rw-r--r--   0 runner    (1001) docker     (122)    30814 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/devices/egun.py
--rw-r--r--   0 runner    (1001) docker     (122)     1743 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/devices/energy.py
--rw-r--r--   0 runner    (1001) docker     (122)    51622 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/devices/fofb.py
--rw-r--r--   0 runner    (1001) docker     (122)     2121 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/devices/ict.py
--rw-r--r--   0 runner    (1001) docker     (122)     9838 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/devices/idff.py
--rw-r--r--   0 runner    (1001) docker     (122)    21325 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/devices/ids.py
--rw-r--r--   0 runner    (1001) docker     (122)    20741 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/devices/injctrl.py
--rw-r--r--   0 runner    (1001) docker     (122)    36024 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/devices/injsys.py
--rw-r--r--   0 runner    (1001) docker     (122)     1630 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/devices/lienergy.py
--rw-r--r--   0 runner    (1001) docker     (122)     6948 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/devices/lillrf.py
--rw-r--r--   0 runner    (1001) docker     (122)      964 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/devices/machshift.py
--rw-r--r--   0 runner    (1001) docker     (122)     2290 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/devices/modltr.py
--rw-r--r--   0 runner    (1001) docker     (122)    36060 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/devices/orbit_interlock.py
--rw-r--r--   0 runner    (1001) docker     (122)     2427 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/devices/posang.py
--rw-r--r--   0 runner    (1001) docker     (122)    10195 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/devices/psconv.py
--rw-r--r--   0 runner    (1001) docker     (122)    12184 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/devices/pssofb.py
--rw-r--r--   0 runner    (1001) docker     (122)    20070 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/devices/pstesters.py
--rw-r--r--   0 runner    (1001) docker     (122)    30064 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/devices/pwrsupply.py
--rw-r--r--   0 runner    (1001) docker     (122)    35448 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/devices/rf.py
--rw-r--r--   0 runner    (1001) docker     (122)     3836 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/devices/screen.py
--rw-r--r--   0 runner    (1001) docker     (122)    22629 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/devices/sofb.py
--rw-r--r--   0 runner    (1001) docker     (122)     2652 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/devices/syncd.py
--rw-r--r--   0 runner    (1001) docker     (122)    17907 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/devices/timing.py
--rw-r--r--   0 runner    (1001) docker     (122)     5055 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/devices/tune.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 14:19:46.834278 siriuspy-2.76.1/siriuspy/diagbeam/
--rw-r--r--   0 runner    (1001) docker     (122)       30 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/diagbeam/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 14:19:46.834278 siriuspy-2.76.1/siriuspy/diagbeam/bpm/
--rw-r--r--   0 runner    (1001) docker     (122)       24 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/diagbeam/bpm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    24052 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/diagbeam/bpm/csdev.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 14:19:46.834278 siriuspy-2.76.1/siriuspy/diagbeam/dcct/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/diagbeam/dcct/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8215 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/diagbeam/dcct/csdev.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 14:19:46.834278 siriuspy-2.76.1/siriuspy/diagbeam/ict/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/diagbeam/ict/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4878 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/diagbeam/ict/csdev.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 14:19:46.834278 siriuspy-2.76.1/siriuspy/diagbeam/screen/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/diagbeam/screen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    12756 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/diagbeam/screen/csdev.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 14:19:46.834278 siriuspy-2.76.1/siriuspy/diagbeam/slit/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/diagbeam/slit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6750 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/diagbeam/slit/csdev.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 14:19:46.834278 siriuspy-2.76.1/siriuspy/diagsys/
--rw-r--r--   0 runner    (1001) docker     (122)       26 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/diagsys/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1444 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/diagsys/app.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 14:19:46.838279 siriuspy-2.76.1/siriuspy/diagsys/lidiag/
--rw-r--r--   0 runner    (1001) docker     (122)       29 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/diagsys/lidiag/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5193 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/diagsys/lidiag/csdev.py
--rw-r--r--   0 runner    (1001) docker     (122)     8168 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/diagsys/lidiag/main.py
--rw-r--r--   0 runner    (1001) docker     (122)     8774 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/diagsys/lidiag/pvs.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 14:19:46.838279 siriuspy-2.76.1/siriuspy/diagsys/psdiag/
--rw-r--r--   0 runner    (1001) docker     (122)       25 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/diagsys/psdiag/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2699 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/diagsys/psdiag/csdev.py
--rw-r--r--   0 runner    (1001) docker     (122)     4582 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/diagsys/psdiag/main.py
--rw-r--r--   0 runner    (1001) docker     (122)     7692 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/diagsys/psdiag/pvs.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 14:19:46.838279 siriuspy-2.76.1/siriuspy/diagsys/pudiag/
--rw-r--r--   0 runner    (1001) docker     (122)       25 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/diagsys/pudiag/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1418 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/diagsys/pudiag/csdev.py
--rw-r--r--   0 runner    (1001) docker     (122)     2871 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/diagsys/pudiag/main.py
--rw-r--r--   0 runner    (1001) docker     (122)     4099 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/diagsys/pudiag/pvs.py
--rw-r--r--   0 runner    (1001) docker     (122)     6824 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/diagsys/pvs.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 14:19:46.838279 siriuspy-2.76.1/siriuspy/diagsys/rfdiag/
--rw-r--r--   0 runner    (1001) docker     (122)       25 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/diagsys/rfdiag/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2409 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/diagsys/rfdiag/csdev.py
--rw-r--r--   0 runner    (1001) docker     (122)     3783 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/diagsys/rfdiag/main.py
--rw-r--r--   0 runner    (1001) docker     (122)     4891 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/diagsys/rfdiag/pvs.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 14:19:46.838279 siriuspy-2.76.1/siriuspy/dvfimgproc/
--rw-r--r--   0 runner    (1001) docker     (122)       39 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/dvfimgproc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7611 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/dvfimgproc/csdev.py
--rw-r--r--   0 runner    (1001) docker     (122)    15404 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/dvfimgproc/main.py
--rw-r--r--   0 runner    (1001) docker     (122)     7057 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/dvfimgproc/meas.py
--rw-r--r--   0 runner    (1001) docker     (122)     2135 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/envars.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 14:19:46.838279 siriuspy-2.76.1/siriuspy/epics/
--rw-r--r--   0 runner    (1001) docker     (122)      379 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/epics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      624 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/epics/multiproc.py
--rw-r--r--   0 runner    (1001) docker     (122)     9097 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/epics/properties.py
--rw-r--r--   0 runner    (1001) docker     (122)      209 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/epics/pv.py
--rw-r--r--   0 runner    (1001) docker     (122)    29251 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/epics/pv_fake.py
--rw-r--r--   0 runner    (1001) docker     (122)     9170 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/epics/pv_time_serie.py
--rw-r--r--   0 runner    (1001) docker     (122)      100 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/epics/threading.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 14:19:46.838279 siriuspy-2.76.1/siriuspy/fofb/
--rw-r--r--   0 runner    (1001) docker     (122)       34 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/fofb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    20125 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/fofb/csdev.py
--rw-r--r--   0 runner    (1001) docker     (122)    79363 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/fofb/main.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 14:19:46.838279 siriuspy-2.76.1/siriuspy/idff/
--rw-r--r--   0 runner    (1001) docker     (122)       76 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/idff/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7475 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/idff/config.py
--rw-r--r--   0 runner    (1001) docker     (122)     3408 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/idff/csdev.py
--rw-r--r--   0 runner    (1001) docker     (122)    13812 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/idff/main.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 14:19:46.842279 siriuspy-2.76.1/siriuspy/injctrl/
--rw-r--r--   0 runner    (1001) docker     (122)       36 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/injctrl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    15244 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/injctrl/bias_feedback.py
--rw-r--r--   0 runner    (1001) docker     (122)    26067 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/injctrl/csdev.py
--rw-r--r--   0 runner    (1001) docker     (122)    67948 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/injctrl/main.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 14:19:46.842279 siriuspy-2.76.1/siriuspy/machshift/
--rw-r--r--   0 runner    (1001) docker     (122)       32 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/machshift/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1297 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/machshift/csdev.py
--rw-r--r--   0 runner    (1001) docker     (122)    77640 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/machshift/macreport.py
--rw-r--r--   0 runner    (1001) docker     (122)     8913 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/machshift/macschedule.py
--rw-r--r--   0 runner    (1001) docker     (122)     2237 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/machshift/main.py
--rw-r--r--   0 runner    (1001) docker     (122)     5429 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/machshift/test_macreport.py
--rw-r--r--   0 runner    (1001) docker     (122)     2012 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/machshift/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 14:19:46.842279 siriuspy-2.76.1/siriuspy/magnet/
--rw-r--r--   0 runner    (1001) docker     (122)       25 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/magnet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1126 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/magnet/data.py
--rw-r--r--   0 runner    (1001) docker     (122)     8736 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/magnet/excdata.py
--rw-r--r--   0 runner    (1001) docker     (122)     1390 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/magnet/factory.py
--rw-r--r--   0 runner    (1001) docker     (122)    15453 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/magnet/normalizer.py
--rw-r--r--   0 runner    (1001) docker     (122)     7185 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/magnet/util.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 14:19:46.842279 siriuspy-2.76.1/siriuspy/meas/
--rw-r--r--   0 runner    (1001) docker     (122)       41 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/meas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    11826 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/meas/csdev.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 14:19:46.842279 siriuspy-2.76.1/siriuspy/meas/liemit/
--rw-r--r--   0 runner    (1001) docker     (122)       57 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/meas/liemit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1455 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/meas/liemit/csdev.py
--rw-r--r--   0 runner    (1001) docker     (122)    13017 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/meas/liemit/main.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 14:19:46.846279 siriuspy-2.76.1/siriuspy/meas/lienergy/
--rw-r--r--   0 runner    (1001) docker     (122)       80 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/meas/lienergy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2821 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/meas/lienergy/csdev.py
--rw-r--r--   0 runner    (1001) docker     (122)     8714 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/meas/lienergy/main.py
--rw-r--r--   0 runner    (1001) docker     (122)    25137 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/meas/util.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 14:19:46.846279 siriuspy-2.76.1/siriuspy/namesys/
--rw-r--r--   0 runner    (1001) docker     (122)       82 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/namesys/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    15210 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/namesys/implementation.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 14:19:46.846279 siriuspy-2.76.1/siriuspy/optics/
--rw-r--r--   0 runner    (1001) docker     (122)       25 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/optics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      363 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/optics/constants.py
--rw-r--r--   0 runner    (1001) docker     (122)     8749 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/optics/lattice_survey.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 14:19:46.846279 siriuspy-2.76.1/siriuspy/opticscorr/
--rw-r--r--   0 runner    (1001) docker     (122)       29 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/opticscorr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    34878 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/opticscorr/base.py
--rw-r--r--   0 runner    (1001) docker     (122)    16096 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/opticscorr/chrom.py
--rw-r--r--   0 runner    (1001) docker     (122)    13454 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/opticscorr/csdev.py
--rw-r--r--   0 runner    (1001) docker     (122)    18765 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/opticscorr/opticscorr.py
--rw-r--r--   0 runner    (1001) docker     (122)     8006 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/opticscorr/tune.py
--rw-r--r--   0 runner    (1001) docker     (122)     1846 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/opticscorr/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 14:19:46.846279 siriuspy-2.76.1/siriuspy/oscilloscope/
--rw-r--r--   0 runner    (1001) docker     (122)      104 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/oscilloscope/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6691 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/oscilloscope/keysight.py
--rw-r--r--   0 runner    (1001) docker     (122)     1467 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/oscilloscope/scopes.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 14:19:46.846279 siriuspy-2.76.1/siriuspy/posang/
--rw-r--r--   0 runner    (1001) docker     (122)       25 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/posang/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4935 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/posang/csdev.py
--rw-r--r--   0 runner    (1001) docker     (122)    19747 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/posang/main.py
--rw-r--r--   0 runner    (1001) docker     (122)     1678 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/posang/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 14:19:46.850279 siriuspy-2.76.1/siriuspy/pwrsupply/
--rw-r--r--   0 runner    (1001) docker     (122)      132 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/pwrsupply/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8950 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/pwrsupply/beaglebone.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 14:19:46.850279 siriuspy-2.76.1/siriuspy/pwrsupply/bsmp/
--rw-r--r--   0 runner    (1001) docker     (122)       48 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/pwrsupply/bsmp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    25156 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/pwrsupply/bsmp/commands.py
--rw-r--r--   0 runner    (1001) docker     (122)    19464 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/pwrsupply/bsmp/constants.py
--rw-r--r--   0 runner    (1001) docker     (122)    53763 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/pwrsupply/bsmp/entities.py
--rw-r--r--   0 runner    (1001) docker     (122)      850 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/pwrsupply/bsmp/factory.py
--rw-r--r--   0 runner    (1001) docker     (122)   150426 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/pwrsupply/csdev.py
--rw-r--r--   0 runner    (1001) docker     (122)     3624 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/pwrsupply/data.py
--rw-r--r--   0 runner    (1001) docker     (122)    10620 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/pwrsupply/factory.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 14:19:46.850279 siriuspy-2.76.1/siriuspy/pwrsupply/pructrl/
--rw-r--r--   0 runner    (1001) docker     (122)      841 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/pwrsupply/pructrl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3393 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/pwrsupply/pructrl/pru.py
--rw-r--r--   0 runner    (1001) docker     (122)    26340 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/pwrsupply/pructrl/prucontroller.py
--rw-r--r--   0 runner    (1001) docker     (122)     6133 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/pwrsupply/pructrl/prucparms.py
--rw-r--r--   0 runner    (1001) docker     (122)    10280 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/pwrsupply/pructrl/psdevstate.py
--rw-r--r--   0 runner    (1001) docker     (122)     7712 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/pwrsupply/pructrl/udc.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 14:19:46.854279 siriuspy-2.76.1/siriuspy/pwrsupply/psctrl/
--rw-r--r--   0 runner    (1001) docker     (122)      866 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/pwrsupply/psctrl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7884 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/pwrsupply/psctrl/pscontroller.py
--rw-r--r--   0 runner    (1001) docker     (122)     6262 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/pwrsupply/psctrl/pscreaders.py
--rw-r--r--   0 runner    (1001) docker     (122)     5502 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/pwrsupply/psctrl/pscstatus.py
--rw-r--r--   0 runner    (1001) docker     (122)    17064 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/pwrsupply/psctrl/pscwriters.py
--rw-r--r--   0 runner    (1001) docker     (122)    42124 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/pwrsupply/psctrl/psmodel.py
--rw-r--r--   0 runner    (1001) docker     (122)    34142 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/pwrsupply/pssofb.py
--rw-r--r--   0 runner    (1001) docker     (122)    12500 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/pwrsupply/siggen.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 14:19:46.854279 siriuspy-2.76.1/siriuspy/ramp/
--rw-r--r--   0 runner    (1001) docker     (122)       23 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/ramp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    28999 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/ramp/conn.py
--rw-r--r--   0 runner    (1001) docker     (122)      346 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/ramp/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)     3969 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/ramp/magnet.py
--rw-r--r--   0 runner    (1001) docker     (122)    45093 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/ramp/ramp.py
--rw-r--r--   0 runner    (1001) docker     (122)    29333 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/ramp/reconst_factory.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     6985 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/ramp/test_reconst_factory.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     4158 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/ramp/testwfm.py
--rw-r--r--   0 runner    (1001) docker     (122)     5584 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/ramp/util.py
--rw-r--r--   0 runner    (1001) docker     (122)    30145 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/ramp/waveform.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 14:19:46.858279 siriuspy-2.76.1/siriuspy/search/
--rw-r--r--   0 runner    (1001) docker     (122)      359 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/search/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3537 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/search/bpms_search.py
--rw-r--r--   0 runner    (1001) docker     (122)     6612 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/search/hl_time_search.py
--rw-r--r--   0 runner    (1001) docker     (122)     5566 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/search/id_search.py
--rw-r--r--   0 runner    (1001) docker     (122)     4152 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/search/ioc_search.py
--rw-r--r--   0 runner    (1001) docker     (122)    16917 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/search/ll_time_search.py
--rw-r--r--   0 runner    (1001) docker     (122)     7219 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/search/ma_search.py
--rw-r--r--   0 runner    (1001) docker     (122)    23882 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/search/ps_search.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 14:19:46.858279 siriuspy-2.76.1/siriuspy/simul/
--rw-r--r--   0 runner    (1001) docker     (122)      311 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/simul/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2202 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/simul/simfactory.py
--rw-r--r--   0 runner    (1001) docker     (122)     6298 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/simul/simps.py
--rw-r--r--   0 runner    (1001) docker     (122)     2324 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/simul/simpv.py
--rw-r--r--   0 runner    (1001) docker     (122)     7391 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/simul/simulation.py
--rw-r--r--   0 runner    (1001) docker     (122)     4266 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/simul/simulator.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 14:19:46.858279 siriuspy-2.76.1/siriuspy/sofb/
--rw-r--r--   0 runner    (1001) docker     (122)       78 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/sofb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4646 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/sofb/base_class.py
--rw-r--r--   0 runner    (1001) docker     (122)    28072 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/sofb/bpms.py
--rw-r--r--   0 runner    (1001) docker     (122)    32149 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/sofb/correctors.py
--rw-r--r--   0 runner    (1001) docker     (122)    47045 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/sofb/csdev.py
--rw-r--r--   0 runner    (1001) docker     (122)    46519 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/sofb/main.py
--rw-r--r--   0 runner    (1001) docker     (122)    12220 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/sofb/matrix.py
--rw-r--r--   0 runner    (1001) docker     (122)    39936 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/sofb/orbit.py
--rw-r--r--   0 runner    (1001) docker     (122)     3030 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/sofb/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 14:19:46.858279 siriuspy-2.76.1/siriuspy/stabinfo/
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/stabinfo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3558 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/stabinfo/csdev.py
--rw-r--r--   0 runner    (1001) docker     (122)     7708 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/stabinfo/main.py
--rw-r--r--   0 runner    (1001) docker     (122)     8093 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/thread.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 14:19:46.862279 siriuspy-2.76.1/siriuspy/timesys/
--rw-r--r--   0 runner    (1001) docker     (122)       26 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/timesys/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    20220 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/timesys/csdev.py
--rw-r--r--   0 runner    (1001) docker     (122)    12705 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/timesys/hl_classes.py
--rw-r--r--   0 runner    (1001) docker     (122)    33256 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/timesys/ll_classes.py
--rw-r--r--   0 runner    (1001) docker     (122)     6015 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/timesys/plot_network.py
--rw-r--r--   0 runner    (1001) docker     (122)     5957 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/timesys/static_table.py
--rw-r--r--   0 runner    (1001) docker     (122)     8732 2023-06-20 14:19:38.000000 siriuspy-2.76.1/siriuspy/util.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 14:19:46.826279 siriuspy-2.76.1/siriuspy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     1423 2023-06-20 14:19:46.000000 siriuspy-2.76.1/siriuspy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    10089 2023-06-20 14:19:46.000000 siriuspy-2.76.1/siriuspy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-20 14:19:46.000000 siriuspy-2.76.1/siriuspy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-20 14:19:46.000000 siriuspy-2.76.1/siriuspy.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)      128 2023-06-20 14:19:46.000000 siriuspy-2.76.1/siriuspy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       15 2023-06-20 14:19:46.000000 siriuspy-2.76.1/siriuspy.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 14:19:46.862279 siriuspy-2.76.1/tests/
--rw-r--r--   0 runner    (1001) docker     (122)      441 2023-06-20 14:19:38.000000 siriuspy-2.76.1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 14:19:46.862279 siriuspy-2.76.1/tests/bsmp/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-20 14:19:38.000000 siriuspy-2.76.1/tests/bsmp/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     5698 2023-06-20 14:19:38.000000 siriuspy-2.76.1/tests/bsmp/test_bsmp.py
--rwxr-xr-x   0 runner    (1001) docker     (122)    14788 2023-06-20 14:19:38.000000 siriuspy-2.76.1/tests/bsmp/test_commands.py
--rwxr-xr-x   0 runner    (1001) docker     (122)    13382 2023-06-20 14:19:38.000000 siriuspy-2.76.1/tests/bsmp/test_entities.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     7719 2023-06-20 14:19:38.000000 siriuspy-2.76.1/tests/bsmp/test_serial.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     1837 2023-06-20 14:19:38.000000 siriuspy-2.76.1/tests/bsmp/test_types.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 14:19:46.862279 siriuspy-2.76.1/tests/clientconfigdb/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-20 14:19:38.000000 siriuspy-2.76.1/tests/clientconfigdb/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     2843 2023-06-20 14:19:38.000000 siriuspy-2.76.1/tests/clientconfigdb/test_configdb_client.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 14:19:46.862279 siriuspy-2.76.1/tests/clientweb/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-20 14:19:38.000000 siriuspy-2.76.1/tests/clientweb/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (122)    11633 2023-06-20 14:19:38.000000 siriuspy-2.76.1/tests/clientweb/test_implementation.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 14:19:46.866279 siriuspy-2.76.1/tests/currinfo/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-20 14:19:38.000000 siriuspy-2.76.1/tests/currinfo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 14:19:46.866279 siriuspy-2.76.1/tests/currinfo/lifetime/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-20 14:19:38.000000 siriuspy-2.76.1/tests/currinfo/lifetime/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     1908 2023-06-20 14:19:38.000000 siriuspy-2.76.1/tests/currinfo/lifetime/test_main.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     6495 2023-06-20 14:19:38.000000 siriuspy-2.76.1/tests/currinfo/test_csdev.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     2653 2023-06-20 14:19:38.000000 siriuspy-2.76.1/tests/currinfo/test_main.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 14:19:46.866279 siriuspy-2.76.1/tests/magnet/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-20 14:19:38.000000 siriuspy-2.76.1/tests/magnet/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     2275 2023-06-20 14:19:38.000000 siriuspy-2.76.1/tests/magnet/test_factory.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     2687 2023-06-20 14:19:38.000000 siriuspy-2.76.1/tests/magnet/tests_normalizer.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     3618 2023-06-20 14:19:38.000000 siriuspy-2.76.1/tests/mock_servweb.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 14:19:46.866279 siriuspy-2.76.1/tests/namesys/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-20 14:19:38.000000 siriuspy-2.76.1/tests/namesys/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     4896 2023-06-20 14:19:38.000000 siriuspy-2.76.1/tests/namesys/test_implementation.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 14:19:46.866279 siriuspy-2.76.1/tests/opticscorr/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-20 14:19:38.000000 siriuspy-2.76.1/tests/opticscorr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5490 2023-06-20 14:19:38.000000 siriuspy-2.76.1/tests/opticscorr/test_chrom.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     4609 2023-06-20 14:19:38.000000 siriuspy-2.76.1/tests/opticscorr/test_csdev.py
--rwxr-xr-x   0 runner    (1001) docker     (122)    23381 2023-06-20 14:19:38.000000 siriuspy-2.76.1/tests/opticscorr/test_opticscorr.py
--rw-r--r--   0 runner    (1001) docker     (122)     5692 2023-06-20 14:19:38.000000 siriuspy-2.76.1/tests/opticscorr/test_tune.py
--rw-r--r--   0 runner    (1001) docker     (122)     1145 2023-06-20 14:19:38.000000 siriuspy-2.76.1/tests/opticscorr/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 14:19:46.866279 siriuspy-2.76.1/tests/posang/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-20 14:19:38.000000 siriuspy-2.76.1/tests/posang/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     2872 2023-06-20 14:19:38.000000 siriuspy-2.76.1/tests/posang/test_csdev.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     3164 2023-06-20 14:19:38.000000 siriuspy-2.76.1/tests/posang/test_main.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 14:19:46.870279 siriuspy-2.76.1/tests/pwrsupply/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-20 14:19:38.000000 siriuspy-2.76.1/tests/pwrsupply/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    18979 2023-06-20 14:19:38.000000 siriuspy-2.76.1/tests/pwrsupply/db.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 14:19:46.870279 siriuspy-2.76.1/tests/pwrsupply/pructrl/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-20 14:19:38.000000 siriuspy-2.76.1/tests/pwrsupply/pructrl/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     2257 2023-06-20 14:19:38.000000 siriuspy-2.76.1/tests/pwrsupply/pructrl/test_pru.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 14:19:46.870279 siriuspy-2.76.1/tests/pwrsupply/psctrl/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-20 14:19:38.000000 siriuspy-2.76.1/tests/pwrsupply/psctrl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4853 2023-06-20 14:19:38.000000 siriuspy-2.76.1/tests/pwrsupply/psctrl/test_pscwriters.py
--rwxr-xr-x   0 runner    (1001) docker     (122)      166 2023-06-20 14:19:38.000000 siriuspy-2.76.1/tests/pwrsupply/test_beaglebone.py
--rwxr-xr-x   0 runner    (1001) docker     (122)       89 2023-06-20 14:19:38.000000 siriuspy-2.76.1/tests/pwrsupply/test_bsmp.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     6439 2023-06-20 14:19:38.000000 siriuspy-2.76.1/tests/pwrsupply/test_csdev.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     7331 2023-06-20 14:19:38.000000 siriuspy-2.76.1/tests/pwrsupply/test_data.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     2323 2023-06-20 14:19:38.000000 siriuspy-2.76.1/tests/pwrsupply/test_siggen.py
--rw-r--r--   0 runner    (1001) docker     (122)     3146 2023-06-20 14:19:38.000000 siriuspy-2.76.1/tests/pwrsupply/variables.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 14:19:46.870279 siriuspy-2.76.1/tests/ramp/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-20 14:19:38.000000 siriuspy-2.76.1/tests/ramp/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     5699 2023-06-20 14:19:38.000000 siriuspy-2.76.1/tests/ramp/test_magnet.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     7235 2023-06-20 14:19:38.000000 siriuspy-2.76.1/tests/ramp/test_waveform.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 14:19:46.870279 siriuspy-2.76.1/tests/search/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-20 14:19:38.000000 siriuspy-2.76.1/tests/search/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     2412 2023-06-20 14:19:38.000000 siriuspy-2.76.1/tests/search/test_hl_time_search.py
--rwxr-xr-x   0 runner    (1001) docker     (122)      559 2023-06-20 14:19:38.000000 siriuspy-2.76.1/tests/search/test_init.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     3831 2023-06-20 14:19:38.000000 siriuspy-2.76.1/tests/search/test_ll_time_search.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     6120 2023-06-20 14:19:38.000000 siriuspy-2.76.1/tests/search/test_ma_search.py
--rwxr-xr-x   0 runner    (1001) docker     (122)    13502 2023-06-20 14:19:38.000000 siriuspy-2.76.1/tests/search/test_ps_search.py
--rw-r--r--   0 runner    (1001) docker     (122)     3478 2023-06-20 14:19:38.000000 siriuspy-2.76.1/tests/test_callbacks.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     1009 2023-06-20 14:19:38.000000 siriuspy-2.76.1/tests/test_csdev.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     1605 2023-06-20 14:19:38.000000 siriuspy-2.76.1/tests/test_envars.py
--rwxr-xr-x   0 runner    (1001) docker     (122)    11533 2023-06-20 14:19:38.000000 siriuspy-2.76.1/tests/test_util.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 14:19:46.870279 siriuspy-2.76.1/tests/timesys/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-20 14:19:38.000000 siriuspy-2.76.1/tests/timesys/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     4999 2023-06-20 14:19:38.000000 siriuspy-2.76.1/tests/timesys/test_csdev.py
--rw-r--r--   0 runner    (1001) docker     (122)      978 2023-06-20 14:19:38.000000 siriuspy-2.76.1/tests/timesys/test_plot_network.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 19:16:13.604366 siriuspy-2.77.0/
+-rw-r--r--   0 runner    (1001) docker     (122)    34494 2023-06-27 19:16:04.000000 siriuspy-2.77.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       90 2023-06-27 19:16:04.000000 siriuspy-2.77.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     1423 2023-06-27 19:16:13.604366 siriuspy-2.77.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      954 2023-06-27 19:16:04.000000 siriuspy-2.77.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)      128 2023-06-27 19:16:04.000000 siriuspy-2.77.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-27 19:16:13.604366 siriuspy-2.77.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (122)     1243 2023-06-27 19:16:04.000000 siriuspy-2.77.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 19:16:13.572365 siriuspy-2.77.0/siriuspy/
+-rw-r--r--   0 runner    (1001) docker     (122)        7 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/VERSION
+-rw-r--r--   0 runner    (1001) docker     (122)      515 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 19:16:13.572365 siriuspy-2.77.0/siriuspy/bsmp/
+-rw-r--r--   0 runner    (1001) docker     (122)      422 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/bsmp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15885 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/bsmp/commands.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1904 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/bsmp/constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11790 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/bsmp/entities.py
+-rw-r--r--   0 runner    (1001) docker     (122)      610 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/bsmp/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8110 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/bsmp/serial.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1204 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/bsmp/types.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2992 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/callbacks.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 19:16:13.572365 siriuspy-2.77.0/siriuspy/clientarch/
+-rw-r--r--   0 runner    (1001) docker     (122)      306 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/clientarch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13813 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/clientarch/client.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6392 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/clientarch/devices.py
+-rw-r--r--   0 runner    (1001) docker     (122)      643 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/clientarch/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20400 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/clientarch/pvarch.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5003 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/clientarch/time.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 19:16:13.576365 siriuspy-2.77.0/siriuspy/clientconfigdb/
+-rw-r--r--   0 runner    (1001) docker     (122)      227 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/clientconfigdb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3345 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/clientconfigdb/_templates.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9599 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/clientconfigdb/configdb_client.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5448 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/clientconfigdb/configdb_document.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4785 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/clientconfigdb/pvsconfig.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 19:16:13.576365 siriuspy-2.77.0/siriuspy/clientconfigdb/types/
+-rw-r--r--   0 runner    (1001) docker     (122)      286 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/clientconfigdb/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13746 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/clientconfigdb/types/as_corrloop_params.py
+-rw-r--r--   0 runner    (1001) docker     (122)    57636 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/clientconfigdb/types/as_diagnostics.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6681 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/clientconfigdb/types/as_pwrstate.py
+-rw-r--r--   0 runner    (1001) docker     (122)    34247 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/clientconfigdb/types/as_rf.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1135 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/clientconfigdb/types/bo_chromcorr_params.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3984 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/clientconfigdb/types/bo_normalized.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1135 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/clientconfigdb/types/bo_orbcorr_respm.py
+-rw-r--r--   0 runner    (1001) docker     (122)      700 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/clientconfigdb/types/bo_orbit.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3042 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/clientconfigdb/types/bo_ramp.py
+-rw-r--r--   0 runner    (1001) docker     (122)      975 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/clientconfigdb/types/bo_tunecorr_params.py
+-rw-r--r--   0 runner    (1001) docker     (122)   123230 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/clientconfigdb/types/global_config.py
+-rw-r--r--   0 runner    (1001) docker     (122)      735 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/clientconfigdb/types/si_bbadata.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18619 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/clientconfigdb/types/si_bbbproc.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1697 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/clientconfigdb/types/si_chromcorr_params.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1146 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/clientconfigdb/types/si_fastorbcorr_respm.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4741 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/clientconfigdb/types/si_fofb.py
+-rw-r--r--   0 runner    (1001) docker     (122)      957 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/clientconfigdb/types/si_id.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3181 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/clientconfigdb/types/si_idff.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1136 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/clientconfigdb/types/si_orbcorr_respm.py
+-rw-r--r--   0 runner    (1001) docker     (122)      701 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/clientconfigdb/types/si_orbit.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1290 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/clientconfigdb/types/si_tunecorr_params.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1738 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/clientconfigdb/types/tb_normalized.py
+-rw-r--r--   0 runner    (1001) docker     (122)      969 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/clientconfigdb/types/tb_orbcorr_respm.py
+-rw-r--r--   0 runner    (1001) docker     (122)      693 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/clientconfigdb/types/tb_orbit.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1651 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/clientconfigdb/types/tb_posang_respm.py
+-rw-r--r--   0 runner    (1001) docker     (122)      969 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/clientconfigdb/types/ts_orbcorr_respm.py
+-rw-r--r--   0 runner    (1001) docker     (122)      693 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/clientconfigdb/types/ts_orbit.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1721 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/clientconfigdb/types/ts_posang_respm.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 19:16:13.576365 siriuspy-2.77.0/siriuspy/clientweb/
+-rw-r--r--   0 runner    (1001) docker     (122)       50 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/clientweb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5896 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/clientweb/implementation.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2236 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/csdev.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 19:16:13.576365 siriuspy-2.77.0/siriuspy/currinfo/
+-rw-r--r--   0 runner    (1001) docker     (122)      144 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/currinfo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9620 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/currinfo/csdev.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 19:16:13.576365 siriuspy-2.77.0/siriuspy/currinfo/lifetime/
+-rw-r--r--   0 runner    (1001) docker     (122)       72 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/currinfo/lifetime/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12607 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/currinfo/lifetime/main.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23275 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/currinfo/main.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 19:16:13.580366 siriuspy-2.77.0/siriuspy/cycle/
+-rw-r--r--   0 runner    (1001) docker     (122)      514 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/cycle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)   104994 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/cycle/bo_cycle_data.py
+-rw-r--r--   0 runner    (1001) docker     (122)    31135 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/cycle/conn.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9781 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/cycle/fc_cycle_data.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3286 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/cycle/li_cycle_data.py
+-rw-r--r--   0 runner    (1001) docker     (122)    38408 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/cycle/main.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3574 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/cycle/util.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 19:16:13.584365 siriuspy-2.77.0/siriuspy/devices/
+-rw-r--r--   0 runner    (1001) docker     (122)     1784 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/devices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    48546 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/devices/bbb.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2786 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/devices/blctrl.py
+-rw-r--r--   0 runner    (1001) docker     (122)    41475 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/devices/bpm.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7380 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/devices/currinfo.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2402 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/devices/dcct.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13949 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/devices/device.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16525 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/devices/dvf.py
+-rw-r--r--   0 runner    (1001) docker     (122)    30814 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/devices/egun.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1743 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/devices/energy.py
+-rw-r--r--   0 runner    (1001) docker     (122)    51622 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/devices/fofb.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2121 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/devices/ict.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10043 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/devices/idff.py
+-rw-r--r--   0 runner    (1001) docker     (122)    21328 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/devices/ids.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20741 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/devices/injctrl.py
+-rw-r--r--   0 runner    (1001) docker     (122)    36024 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/devices/injsys.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1630 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/devices/lienergy.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6948 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/devices/lillrf.py
+-rw-r--r--   0 runner    (1001) docker     (122)      964 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/devices/machshift.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2290 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/devices/modltr.py
+-rw-r--r--   0 runner    (1001) docker     (122)    36060 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/devices/orbit_interlock.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2427 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/devices/posang.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10195 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/devices/psconv.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12184 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/devices/pssofb.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20070 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/devices/pstesters.py
+-rw-r--r--   0 runner    (1001) docker     (122)    30064 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/devices/pwrsupply.py
+-rw-r--r--   0 runner    (1001) docker     (122)    35448 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/devices/rf.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3836 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/devices/screen.py
+-rw-r--r--   0 runner    (1001) docker     (122)    22629 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/devices/sofb.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2652 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/devices/syncd.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17907 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/devices/timing.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5055 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/devices/tune.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 19:16:13.584365 siriuspy-2.77.0/siriuspy/diagbeam/
+-rw-r--r--   0 runner    (1001) docker     (122)       30 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/diagbeam/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 19:16:13.584365 siriuspy-2.77.0/siriuspy/diagbeam/bpm/
+-rw-r--r--   0 runner    (1001) docker     (122)       24 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/diagbeam/bpm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    24052 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/diagbeam/bpm/csdev.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 19:16:13.584365 siriuspy-2.77.0/siriuspy/diagbeam/dcct/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/diagbeam/dcct/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8215 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/diagbeam/dcct/csdev.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 19:16:13.584365 siriuspy-2.77.0/siriuspy/diagbeam/ict/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/diagbeam/ict/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4878 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/diagbeam/ict/csdev.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 19:16:13.584365 siriuspy-2.77.0/siriuspy/diagbeam/screen/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/diagbeam/screen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12756 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/diagbeam/screen/csdev.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 19:16:13.584365 siriuspy-2.77.0/siriuspy/diagbeam/slit/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/diagbeam/slit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6750 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/diagbeam/slit/csdev.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 19:16:13.584365 siriuspy-2.77.0/siriuspy/diagsys/
+-rw-r--r--   0 runner    (1001) docker     (122)       26 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/diagsys/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1484 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/diagsys/app.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 19:16:13.584365 siriuspy-2.77.0/siriuspy/diagsys/lidiag/
+-rw-r--r--   0 runner    (1001) docker     (122)       29 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/diagsys/lidiag/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5193 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/diagsys/lidiag/csdev.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8168 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/diagsys/lidiag/main.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8774 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/diagsys/lidiag/pvs.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 19:16:13.584365 siriuspy-2.77.0/siriuspy/diagsys/psdiag/
+-rw-r--r--   0 runner    (1001) docker     (122)       25 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/diagsys/psdiag/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2699 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/diagsys/psdiag/csdev.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4582 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/diagsys/psdiag/main.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7692 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/diagsys/psdiag/pvs.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 19:16:13.584365 siriuspy-2.77.0/siriuspy/diagsys/pudiag/
+-rw-r--r--   0 runner    (1001) docker     (122)       25 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/diagsys/pudiag/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1418 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/diagsys/pudiag/csdev.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2871 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/diagsys/pudiag/main.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4099 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/diagsys/pudiag/pvs.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6792 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/diagsys/pvs.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 19:16:13.584365 siriuspy-2.77.0/siriuspy/diagsys/rfdiag/
+-rw-r--r--   0 runner    (1001) docker     (122)       25 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/diagsys/rfdiag/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2409 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/diagsys/rfdiag/csdev.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3783 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/diagsys/rfdiag/main.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4891 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/diagsys/rfdiag/pvs.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 19:16:13.584365 siriuspy-2.77.0/siriuspy/dvfimgproc/
+-rw-r--r--   0 runner    (1001) docker     (122)       39 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/dvfimgproc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7692 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/dvfimgproc/csdev.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15295 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/dvfimgproc/main.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7082 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/dvfimgproc/meas.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2135 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/envars.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 19:16:13.588366 siriuspy-2.77.0/siriuspy/epics/
+-rw-r--r--   0 runner    (1001) docker     (122)      379 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/epics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      624 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/epics/multiproc.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9097 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/epics/properties.py
+-rw-r--r--   0 runner    (1001) docker     (122)      209 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/epics/pv.py
+-rw-r--r--   0 runner    (1001) docker     (122)    29251 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/epics/pv_fake.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9170 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/epics/pv_time_serie.py
+-rw-r--r--   0 runner    (1001) docker     (122)      100 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/epics/threading.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 19:16:13.588366 siriuspy-2.77.0/siriuspy/fofb/
+-rw-r--r--   0 runner    (1001) docker     (122)       34 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/fofb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20125 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/fofb/csdev.py
+-rw-r--r--   0 runner    (1001) docker     (122)    79363 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/fofb/main.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 19:16:13.588366 siriuspy-2.77.0/siriuspy/idff/
+-rw-r--r--   0 runner    (1001) docker     (122)       76 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/idff/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7475 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/idff/config.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3408 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/idff/csdev.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14114 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/idff/main.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 19:16:13.588366 siriuspy-2.77.0/siriuspy/injctrl/
+-rw-r--r--   0 runner    (1001) docker     (122)       36 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/injctrl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15253 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/injctrl/bias_feedback.py
+-rw-r--r--   0 runner    (1001) docker     (122)    24738 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/injctrl/csdev.py
+-rw-r--r--   0 runner    (1001) docker     (122)    70365 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/injctrl/main.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 19:16:13.588366 siriuspy-2.77.0/siriuspy/machshift/
+-rw-r--r--   0 runner    (1001) docker     (122)       32 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/machshift/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1297 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/machshift/csdev.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6903 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/machshift/gensumm_macreport.py
+-rw-r--r--   0 runner    (1001) docker     (122)    78928 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/machshift/macreport.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9197 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/machshift/macschedule.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2237 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/machshift/main.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2539 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/machshift/savedata_macreport.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2012 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/machshift/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 19:16:13.588366 siriuspy-2.77.0/siriuspy/magnet/
+-rw-r--r--   0 runner    (1001) docker     (122)       25 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/magnet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1126 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/magnet/data.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8736 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/magnet/excdata.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1390 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/magnet/factory.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15453 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/magnet/normalizer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7185 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/magnet/util.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 19:16:13.588366 siriuspy-2.77.0/siriuspy/meas/
+-rw-r--r--   0 runner    (1001) docker     (122)       41 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/meas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11826 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/meas/csdev.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 19:16:13.592366 siriuspy-2.77.0/siriuspy/meas/liemit/
+-rw-r--r--   0 runner    (1001) docker     (122)       57 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/meas/liemit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1455 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/meas/liemit/csdev.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13017 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/meas/liemit/main.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 19:16:13.592366 siriuspy-2.77.0/siriuspy/meas/lienergy/
+-rw-r--r--   0 runner    (1001) docker     (122)       80 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/meas/lienergy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2821 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/meas/lienergy/csdev.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8714 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/meas/lienergy/main.py
+-rw-r--r--   0 runner    (1001) docker     (122)    25137 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/meas/util.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 19:16:13.592366 siriuspy-2.77.0/siriuspy/namesys/
+-rw-r--r--   0 runner    (1001) docker     (122)       82 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/namesys/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15210 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/namesys/implementation.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 19:16:13.592366 siriuspy-2.77.0/siriuspy/optics/
+-rw-r--r--   0 runner    (1001) docker     (122)       25 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/optics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      363 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/optics/constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8749 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/optics/lattice_survey.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 19:16:13.592366 siriuspy-2.77.0/siriuspy/opticscorr/
+-rw-r--r--   0 runner    (1001) docker     (122)       29 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/opticscorr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    34878 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/opticscorr/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16096 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/opticscorr/chrom.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13454 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/opticscorr/csdev.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18765 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/opticscorr/opticscorr.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8006 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/opticscorr/tune.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1846 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/opticscorr/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 19:16:13.592366 siriuspy-2.77.0/siriuspy/oscilloscope/
+-rw-r--r--   0 runner    (1001) docker     (122)      104 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/oscilloscope/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6691 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/oscilloscope/keysight.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1467 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/oscilloscope/scopes.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 19:16:13.592366 siriuspy-2.77.0/siriuspy/posang/
+-rw-r--r--   0 runner    (1001) docker     (122)       25 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/posang/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4935 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/posang/csdev.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19747 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/posang/main.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1678 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/posang/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 19:16:13.592366 siriuspy-2.77.0/siriuspy/pwrsupply/
+-rw-r--r--   0 runner    (1001) docker     (122)      132 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/pwrsupply/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8950 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/pwrsupply/beaglebone.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 19:16:13.592366 siriuspy-2.77.0/siriuspy/pwrsupply/bsmp/
+-rw-r--r--   0 runner    (1001) docker     (122)       48 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/pwrsupply/bsmp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    25156 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/pwrsupply/bsmp/commands.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19464 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/pwrsupply/bsmp/constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)    53763 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/pwrsupply/bsmp/entities.py
+-rw-r--r--   0 runner    (1001) docker     (122)      850 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/pwrsupply/bsmp/factory.py
+-rw-r--r--   0 runner    (1001) docker     (122)   150426 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/pwrsupply/csdev.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3624 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/pwrsupply/data.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10629 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/pwrsupply/factory.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 19:16:13.596366 siriuspy-2.77.0/siriuspy/pwrsupply/pructrl/
+-rw-r--r--   0 runner    (1001) docker     (122)      841 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/pwrsupply/pructrl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3393 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/pwrsupply/pructrl/pru.py
+-rw-r--r--   0 runner    (1001) docker     (122)    25723 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/pwrsupply/pructrl/prucontroller.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6133 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/pwrsupply/pructrl/prucparms.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10280 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/pwrsupply/pructrl/psdevstate.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7712 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/pwrsupply/pructrl/udc.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 19:16:13.596366 siriuspy-2.77.0/siriuspy/pwrsupply/psctrl/
+-rw-r--r--   0 runner    (1001) docker     (122)      866 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/pwrsupply/psctrl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7884 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/pwrsupply/psctrl/pscontroller.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6262 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/pwrsupply/psctrl/pscreaders.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5502 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/pwrsupply/psctrl/pscstatus.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17064 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/pwrsupply/psctrl/pscwriters.py
+-rw-r--r--   0 runner    (1001) docker     (122)    42124 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/pwrsupply/psctrl/psmodel.py
+-rw-r--r--   0 runner    (1001) docker     (122)    34142 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/pwrsupply/pssofb.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12500 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/pwrsupply/siggen.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 19:16:13.596366 siriuspy-2.77.0/siriuspy/ramp/
+-rw-r--r--   0 runner    (1001) docker     (122)       23 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/ramp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    28999 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/ramp/conn.py
+-rw-r--r--   0 runner    (1001) docker     (122)      346 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/ramp/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3969 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/ramp/magnet.py
+-rw-r--r--   0 runner    (1001) docker     (122)    45093 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/ramp/ramp.py
+-rw-r--r--   0 runner    (1001) docker     (122)    29333 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/ramp/reconst_factory.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     6985 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/ramp/test_reconst_factory.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     4158 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/ramp/testwfm.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5584 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/ramp/util.py
+-rw-r--r--   0 runner    (1001) docker     (122)    30145 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/ramp/waveform.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 19:16:13.596366 siriuspy-2.77.0/siriuspy/search/
+-rw-r--r--   0 runner    (1001) docker     (122)      359 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/search/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3537 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/search/bpms_search.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6612 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/search/hl_time_search.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5566 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/search/id_search.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4152 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/search/ioc_search.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16917 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/search/ll_time_search.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7219 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/search/ma_search.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23882 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/search/ps_search.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 19:16:13.596366 siriuspy-2.77.0/siriuspy/simul/
+-rw-r--r--   0 runner    (1001) docker     (122)      311 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/simul/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2202 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/simul/simfactory.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6298 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/simul/simps.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2324 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/simul/simpv.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7391 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/simul/simulation.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4266 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/simul/simulator.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 19:16:13.600366 siriuspy-2.77.0/siriuspy/sofb/
+-rw-r--r--   0 runner    (1001) docker     (122)       78 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/sofb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4869 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/sofb/base_class.py
+-rw-r--r--   0 runner    (1001) docker     (122)    28072 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/sofb/bpms.py
+-rw-r--r--   0 runner    (1001) docker     (122)    32010 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/sofb/correctors.py
+-rw-r--r--   0 runner    (1001) docker     (122)    47062 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/sofb/csdev.py
+-rw-r--r--   0 runner    (1001) docker     (122)    46398 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/sofb/main.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11841 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/sofb/matrix.py
+-rw-r--r--   0 runner    (1001) docker     (122)    36357 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/sofb/orbit.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3030 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/sofb/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 19:16:13.600366 siriuspy-2.77.0/siriuspy/stabinfo/
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/stabinfo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3558 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/stabinfo/csdev.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7708 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/stabinfo/main.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8598 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/thread.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 19:16:13.600366 siriuspy-2.77.0/siriuspy/timesys/
+-rw-r--r--   0 runner    (1001) docker     (122)       26 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/timesys/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20220 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/timesys/csdev.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12705 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/timesys/hl_classes.py
+-rw-r--r--   0 runner    (1001) docker     (122)    33256 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/timesys/ll_classes.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6015 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/timesys/plot_network.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5957 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/timesys/static_table.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8732 2023-06-27 19:16:04.000000 siriuspy-2.77.0/siriuspy/util.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 19:16:13.572365 siriuspy-2.77.0/siriuspy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     1423 2023-06-27 19:16:13.000000 siriuspy-2.77.0/siriuspy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    10133 2023-06-27 19:16:13.000000 siriuspy-2.77.0/siriuspy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-27 19:16:13.000000 siriuspy-2.77.0/siriuspy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-27 19:16:13.000000 siriuspy-2.77.0/siriuspy.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)      128 2023-06-27 19:16:13.000000 siriuspy-2.77.0/siriuspy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       15 2023-06-27 19:16:13.000000 siriuspy-2.77.0/siriuspy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 19:16:13.600366 siriuspy-2.77.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)      441 2023-06-27 19:16:04.000000 siriuspy-2.77.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 19:16:13.600366 siriuspy-2.77.0/tests/bsmp/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-27 19:16:04.000000 siriuspy-2.77.0/tests/bsmp/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     5698 2023-06-27 19:16:04.000000 siriuspy-2.77.0/tests/bsmp/test_bsmp.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)    14788 2023-06-27 19:16:04.000000 siriuspy-2.77.0/tests/bsmp/test_commands.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)    13382 2023-06-27 19:16:04.000000 siriuspy-2.77.0/tests/bsmp/test_entities.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     7719 2023-06-27 19:16:04.000000 siriuspy-2.77.0/tests/bsmp/test_serial.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     1837 2023-06-27 19:16:04.000000 siriuspy-2.77.0/tests/bsmp/test_types.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 19:16:13.600366 siriuspy-2.77.0/tests/clientconfigdb/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-27 19:16:04.000000 siriuspy-2.77.0/tests/clientconfigdb/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     2843 2023-06-27 19:16:04.000000 siriuspy-2.77.0/tests/clientconfigdb/test_configdb_client.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 19:16:13.600366 siriuspy-2.77.0/tests/clientweb/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-27 19:16:04.000000 siriuspy-2.77.0/tests/clientweb/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)    11633 2023-06-27 19:16:04.000000 siriuspy-2.77.0/tests/clientweb/test_implementation.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 19:16:13.600366 siriuspy-2.77.0/tests/currinfo/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-27 19:16:04.000000 siriuspy-2.77.0/tests/currinfo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 19:16:13.600366 siriuspy-2.77.0/tests/currinfo/lifetime/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-27 19:16:04.000000 siriuspy-2.77.0/tests/currinfo/lifetime/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     1908 2023-06-27 19:16:04.000000 siriuspy-2.77.0/tests/currinfo/lifetime/test_main.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     6495 2023-06-27 19:16:04.000000 siriuspy-2.77.0/tests/currinfo/test_csdev.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     2653 2023-06-27 19:16:04.000000 siriuspy-2.77.0/tests/currinfo/test_main.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 19:16:13.600366 siriuspy-2.77.0/tests/magnet/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-27 19:16:04.000000 siriuspy-2.77.0/tests/magnet/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     2275 2023-06-27 19:16:04.000000 siriuspy-2.77.0/tests/magnet/test_factory.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     2687 2023-06-27 19:16:04.000000 siriuspy-2.77.0/tests/magnet/tests_normalizer.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     3618 2023-06-27 19:16:04.000000 siriuspy-2.77.0/tests/mock_servweb.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 19:16:13.600366 siriuspy-2.77.0/tests/namesys/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-27 19:16:04.000000 siriuspy-2.77.0/tests/namesys/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     4896 2023-06-27 19:16:04.000000 siriuspy-2.77.0/tests/namesys/test_implementation.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 19:16:13.604366 siriuspy-2.77.0/tests/opticscorr/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-27 19:16:04.000000 siriuspy-2.77.0/tests/opticscorr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5490 2023-06-27 19:16:04.000000 siriuspy-2.77.0/tests/opticscorr/test_chrom.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     4609 2023-06-27 19:16:04.000000 siriuspy-2.77.0/tests/opticscorr/test_csdev.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)    23381 2023-06-27 19:16:04.000000 siriuspy-2.77.0/tests/opticscorr/test_opticscorr.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5692 2023-06-27 19:16:04.000000 siriuspy-2.77.0/tests/opticscorr/test_tune.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1145 2023-06-27 19:16:04.000000 siriuspy-2.77.0/tests/opticscorr/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 19:16:13.604366 siriuspy-2.77.0/tests/posang/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-27 19:16:04.000000 siriuspy-2.77.0/tests/posang/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     2872 2023-06-27 19:16:04.000000 siriuspy-2.77.0/tests/posang/test_csdev.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     3164 2023-06-27 19:16:04.000000 siriuspy-2.77.0/tests/posang/test_main.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 19:16:13.604366 siriuspy-2.77.0/tests/pwrsupply/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-27 19:16:04.000000 siriuspy-2.77.0/tests/pwrsupply/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18979 2023-06-27 19:16:04.000000 siriuspy-2.77.0/tests/pwrsupply/db.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 19:16:13.604366 siriuspy-2.77.0/tests/pwrsupply/pructrl/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-27 19:16:04.000000 siriuspy-2.77.0/tests/pwrsupply/pructrl/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     2257 2023-06-27 19:16:04.000000 siriuspy-2.77.0/tests/pwrsupply/pructrl/test_pru.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 19:16:13.604366 siriuspy-2.77.0/tests/pwrsupply/psctrl/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-27 19:16:04.000000 siriuspy-2.77.0/tests/pwrsupply/psctrl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4853 2023-06-27 19:16:04.000000 siriuspy-2.77.0/tests/pwrsupply/psctrl/test_pscwriters.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)      166 2023-06-27 19:16:04.000000 siriuspy-2.77.0/tests/pwrsupply/test_beaglebone.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)       89 2023-06-27 19:16:04.000000 siriuspy-2.77.0/tests/pwrsupply/test_bsmp.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     6439 2023-06-27 19:16:04.000000 siriuspy-2.77.0/tests/pwrsupply/test_csdev.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     7331 2023-06-27 19:16:04.000000 siriuspy-2.77.0/tests/pwrsupply/test_data.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     2323 2023-06-27 19:16:04.000000 siriuspy-2.77.0/tests/pwrsupply/test_siggen.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3146 2023-06-27 19:16:04.000000 siriuspy-2.77.0/tests/pwrsupply/variables.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 19:16:13.604366 siriuspy-2.77.0/tests/ramp/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-27 19:16:04.000000 siriuspy-2.77.0/tests/ramp/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     5699 2023-06-27 19:16:04.000000 siriuspy-2.77.0/tests/ramp/test_magnet.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     7235 2023-06-27 19:16:04.000000 siriuspy-2.77.0/tests/ramp/test_waveform.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 19:16:13.604366 siriuspy-2.77.0/tests/search/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-27 19:16:04.000000 siriuspy-2.77.0/tests/search/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     2412 2023-06-27 19:16:04.000000 siriuspy-2.77.0/tests/search/test_hl_time_search.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)      559 2023-06-27 19:16:04.000000 siriuspy-2.77.0/tests/search/test_init.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     3831 2023-06-27 19:16:04.000000 siriuspy-2.77.0/tests/search/test_ll_time_search.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     6120 2023-06-27 19:16:04.000000 siriuspy-2.77.0/tests/search/test_ma_search.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)    13502 2023-06-27 19:16:04.000000 siriuspy-2.77.0/tests/search/test_ps_search.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3478 2023-06-27 19:16:04.000000 siriuspy-2.77.0/tests/test_callbacks.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     1009 2023-06-27 19:16:04.000000 siriuspy-2.77.0/tests/test_csdev.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     1605 2023-06-27 19:16:04.000000 siriuspy-2.77.0/tests/test_envars.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)    11533 2023-06-27 19:16:04.000000 siriuspy-2.77.0/tests/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 19:16:13.604366 siriuspy-2.77.0/tests/timesys/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-27 19:16:04.000000 siriuspy-2.77.0/tests/timesys/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     4999 2023-06-27 19:16:04.000000 siriuspy-2.77.0/tests/timesys/test_csdev.py
+-rw-r--r--   0 runner    (1001) docker     (122)      978 2023-06-27 19:16:04.000000 siriuspy-2.77.0/tests/timesys/test_plot_network.py
```

### Comparing `siriuspy-2.76.1/LICENSE` & `siriuspy-2.77.0/LICENSE`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/PKG-INFO` & `siriuspy-2.77.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: siriuspy
-Version: 2.76.1
+Version: 2.77.0
 Summary: Development packages for Sirius
 Home-page: https://github.com/lnls-sirius/dev-packages
 Download-URL: https://github.com/lnls-sirius/dev-packages
 Author: lnls-sirius
 License: GNU GPLv3
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python
```

### Comparing `siriuspy-2.76.1/README.md` & `siriuspy-2.77.0/README.md`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/setup.py` & `siriuspy-2.77.0/setup.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/siriuspy/__init__.py` & `siriuspy-2.77.0/siriuspy/__init__.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/siriuspy/bsmp/commands.py` & `siriuspy-2.77.0/siriuspy/bsmp/commands.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/siriuspy/bsmp/constants.py` & `siriuspy-2.77.0/siriuspy/bsmp/constants.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/siriuspy/bsmp/entities.py` & `siriuspy-2.77.0/siriuspy/bsmp/entities.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/siriuspy/bsmp/exceptions.py` & `siriuspy-2.77.0/siriuspy/bsmp/exceptions.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/siriuspy/bsmp/serial.py` & `siriuspy-2.77.0/siriuspy/bsmp/serial.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/siriuspy/bsmp/types.py` & `siriuspy-2.77.0/siriuspy/bsmp/types.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/siriuspy/callbacks.py` & `siriuspy-2.77.0/siriuspy/callbacks.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/siriuspy/clientarch/client.py` & `siriuspy-2.77.0/siriuspy/clientarch/client.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/siriuspy/clientarch/devices.py` & `siriuspy-2.77.0/siriuspy/clientarch/devices.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/siriuspy/clientarch/exceptions.py` & `siriuspy-2.77.0/siriuspy/clientarch/exceptions.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/siriuspy/clientarch/pvarch.py` & `siriuspy-2.77.0/siriuspy/clientarch/pvarch.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/siriuspy/clientarch/time.py` & `siriuspy-2.77.0/siriuspy/clientarch/time.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/siriuspy/clientconfigdb/_templates.py` & `siriuspy-2.77.0/siriuspy/clientconfigdb/_templates.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/siriuspy/clientconfigdb/configdb_client.py` & `siriuspy-2.77.0/siriuspy/clientconfigdb/configdb_client.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/siriuspy/clientconfigdb/configdb_document.py` & `siriuspy-2.77.0/siriuspy/clientconfigdb/configdb_document.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/siriuspy/clientconfigdb/pvsconfig.py` & `siriuspy-2.77.0/siriuspy/clientconfigdb/pvsconfig.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/siriuspy/clientconfigdb/types/as_corrloop_params.py` & `siriuspy-2.77.0/siriuspy/clientconfigdb/types/as_corrloop_params.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/siriuspy/clientconfigdb/types/as_diagnostics.py` & `siriuspy-2.77.0/siriuspy/clientconfigdb/types/as_diagnostics.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/siriuspy/clientconfigdb/types/as_pwrstate.py` & `siriuspy-2.77.0/siriuspy/clientconfigdb/types/as_pwrstate.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/siriuspy/clientconfigdb/types/as_rf.py` & `siriuspy-2.77.0/siriuspy/clientconfigdb/types/as_rf.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/siriuspy/clientconfigdb/types/bo_chromcorr_params.py` & `siriuspy-2.77.0/siriuspy/clientconfigdb/types/bo_chromcorr_params.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/siriuspy/clientconfigdb/types/bo_normalized.py` & `siriuspy-2.77.0/siriuspy/clientconfigdb/types/bo_normalized.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/siriuspy/clientconfigdb/types/bo_orbcorr_respm.py` & `siriuspy-2.77.0/siriuspy/clientconfigdb/types/bo_orbcorr_respm.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/siriuspy/clientconfigdb/types/bo_orbit.py` & `siriuspy-2.77.0/siriuspy/clientconfigdb/types/bo_orbit.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/siriuspy/clientconfigdb/types/bo_ramp.py` & `siriuspy-2.77.0/siriuspy/clientconfigdb/types/bo_ramp.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/siriuspy/clientconfigdb/types/bo_tunecorr_params.py` & `siriuspy-2.77.0/siriuspy/clientconfigdb/types/bo_tunecorr_params.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/siriuspy/clientconfigdb/types/global_config.py` & `siriuspy-2.77.0/siriuspy/clientconfigdb/types/global_config.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/siriuspy/clientconfigdb/types/si_bbadata.py` & `siriuspy-2.77.0/siriuspy/clientconfigdb/types/si_bbadata.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/siriuspy/clientconfigdb/types/si_bbbproc.py` & `siriuspy-2.77.0/siriuspy/clientconfigdb/types/si_bbbproc.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/siriuspy/clientconfigdb/types/si_chromcorr_params.py` & `siriuspy-2.77.0/siriuspy/clientconfigdb/types/si_chromcorr_params.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/siriuspy/clientconfigdb/types/si_fastorbcorr_respm.py` & `siriuspy-2.77.0/siriuspy/clientconfigdb/types/si_fastorbcorr_respm.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/siriuspy/clientconfigdb/types/si_fofb.py` & `siriuspy-2.77.0/siriuspy/clientconfigdb/types/si_fofb.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/siriuspy/clientconfigdb/types/si_id.py` & `siriuspy-2.77.0/siriuspy/clientconfigdb/types/si_id.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/siriuspy/clientconfigdb/types/si_idff.py` & `siriuspy-2.77.0/siriuspy/clientconfigdb/types/si_idff.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/siriuspy/clientconfigdb/types/si_orbcorr_respm.py` & `siriuspy-2.77.0/siriuspy/clientconfigdb/types/si_orbcorr_respm.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/siriuspy/clientconfigdb/types/si_orbit.py` & `siriuspy-2.77.0/siriuspy/clientconfigdb/types/si_orbit.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/siriuspy/clientconfigdb/types/si_tunecorr_params.py` & `siriuspy-2.77.0/siriuspy/clientconfigdb/types/si_tunecorr_params.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/siriuspy/clientconfigdb/types/tb_normalized.py` & `siriuspy-2.77.0/siriuspy/clientconfigdb/types/tb_normalized.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/siriuspy/clientconfigdb/types/tb_orbcorr_respm.py` & `siriuspy-2.77.0/siriuspy/clientconfigdb/types/tb_orbcorr_respm.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/siriuspy/clientconfigdb/types/tb_orbit.py` & `siriuspy-2.77.0/siriuspy/clientconfigdb/types/tb_orbit.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/siriuspy/clientconfigdb/types/tb_posang_respm.py` & `siriuspy-2.77.0/siriuspy/clientconfigdb/types/tb_posang_respm.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/siriuspy/clientconfigdb/types/ts_orbcorr_respm.py` & `siriuspy-2.77.0/siriuspy/clientconfigdb/types/ts_orbcorr_respm.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/siriuspy/clientconfigdb/types/ts_orbit.py` & `siriuspy-2.77.0/siriuspy/clientconfigdb/types/ts_orbit.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/siriuspy/clientconfigdb/types/ts_posang_respm.py` & `siriuspy-2.77.0/siriuspy/clientconfigdb/types/ts_posang_respm.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/siriuspy/clientweb/implementation.py` & `siriuspy-2.77.0/siriuspy/clientweb/implementation.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/siriuspy/csdev.py` & `siriuspy-2.77.0/siriuspy/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/siriuspy/currinfo/csdev.py` & `siriuspy-2.77.0/siriuspy/currinfo/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/siriuspy/currinfo/lifetime/main.py` & `siriuspy-2.77.0/siriuspy/currinfo/lifetime/main.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/siriuspy/currinfo/main.py` & `siriuspy-2.77.0/siriuspy/currinfo/main.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/siriuspy/cycle/__init__.py` & `siriuspy-2.77.0/siriuspy/cycle/__init__.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/siriuspy/cycle/bo_cycle_data.py` & `siriuspy-2.77.0/siriuspy/cycle/bo_cycle_data.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/siriuspy/cycle/conn.py` & `siriuspy-2.77.0/siriuspy/cycle/conn.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/siriuspy/cycle/fc_cycle_data.py` & `siriuspy-2.77.0/siriuspy/cycle/fc_cycle_data.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/siriuspy/cycle/li_cycle_data.py` & `siriuspy-2.77.0/siriuspy/cycle/li_cycle_data.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/siriuspy/cycle/main.py` & `siriuspy-2.77.0/siriuspy/cycle/main.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/siriuspy/cycle/util.py` & `siriuspy-2.77.0/siriuspy/cycle/util.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/siriuspy/devices/__init__.py` & `siriuspy-2.77.0/siriuspy/devices/__init__.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/siriuspy/devices/bbb.py` & `siriuspy-2.77.0/siriuspy/devices/bbb.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/siriuspy/devices/blctrl.py` & `siriuspy-2.77.0/siriuspy/devices/blctrl.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/siriuspy/devices/bpm.py` & `siriuspy-2.77.0/siriuspy/devices/bpm.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/siriuspy/devices/currinfo.py` & `siriuspy-2.77.0/siriuspy/devices/currinfo.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/siriuspy/devices/dcct.py` & `siriuspy-2.77.0/siriuspy/devices/dcct.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/siriuspy/devices/device.py` & `siriuspy-2.77.0/siriuspy/devices/device.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/siriuspy/devices/dvf.py` & `siriuspy-2.77.0/siriuspy/devices/dvf.py`

 * *Files 0% similar despite different names*

```diff
@@ -502,15 +502,15 @@
     def roix_fwhm_factor(self, value):
         """."""
         self['ImgROIXUpdateWithFWHMFactor-SP'] = value
 
     @property
     def roi_update_with_fwhm(self):
         """."""
-        return self['ImgROIUpdateWithFWHM-Sts']
+        return bool(self['ImgROIUpdateWithFWHM-Sts'])
 
     @roi_update_with_fwhm.setter
     def roi_update_with_fwhm(self, value):
         """."""
         self['ImgROIUpdateWithFWHM-Sel'] = bool(value)
 
     @property
@@ -547,10 +547,10 @@
     def log(self):
         """."""
         return self['ImgLog-Mon']
 
     def create_image2dfit(self):
         """Return a Image2DFit object with current image as data."""
         imgfit2d = _Image2D_Fit(
-            data=self.image, fitgaussian=self._fitgaussian,
+            data=self.image, fitgauss=self._fitgaussian,
             roix=self.roix, roiy=self.roiy)
         return imgfit2d
```

### Comparing `siriuspy-2.76.1/siriuspy/devices/egun.py` & `siriuspy-2.77.0/siriuspy/devices/egun.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/siriuspy/devices/energy.py` & `siriuspy-2.77.0/siriuspy/devices/energy.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/siriuspy/devices/fofb.py` & `siriuspy-2.77.0/siriuspy/devices/fofb.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/siriuspy/devices/ict.py` & `siriuspy-2.77.0/siriuspy/devices/ict.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/siriuspy/devices/idff.py` & `siriuspy-2.77.0/siriuspy/devices/idff.py`

 * *Files 6% similar despite different names*

```diff
@@ -216,15 +216,19 @@
                 raise ValueError(msg)
 
         return True
 
     def get_polarization_state(
             self, pparameter_value=None, kparameter_value=None):
         """."""
-        if pparameter_value is None:
+        if self.pparametername is None:
+            if kparameter_value is None:
+                kparameter_value = self.kparameter_mon
+            return self.polarizations[0], pparameter_value, kparameter_value
+        if pparameter_value:
             pparameter_value = self.pparameter_mon
         if kparameter_value is None:
             kparameter_value = self.kparameter_mon
         if None in (pparameter_value, kparameter_value):
             return None, pparameter_value, kparameter_value
         polarization = self.idffconfig.get_polarization_state(
             pparameter=pparameter_value, kparameter=kparameter_value)
```

### Comparing `siriuspy-2.76.1/siriuspy/devices/ids.py` & `siriuspy-2.77.0/siriuspy/devices/ids.py`

 * *Files 0% similar despite different names*

```diff
@@ -116,15 +116,15 @@
     TOLERANCE_PHASE = 0.01  # [mm]
 
     _SHORT_SHUT_EYE = 0.1  # [s]
     _default_timeout = 8  # [s]
 
     _properties_papu = (
         'Home-Cmd', 'EnblPwrPhase-Cmd', 'ClearErr-Cmd',
-        'BeamLineCtrl-Mon', 'Home-Mon',
+        'BeamLineCtrl-Mon',  # 'Home-Mon',
         )
     _properties = (
         'PeriodLength-Cte',
         'BeamLineCtrlEnbl-Sel', 'BeamLineCtrlEnbl-Sts',
         'Moving-Mon',
         'PwrPhase-Mon',
         'EnblAndReleasePhase-Sel', 'EnblAndReleasePhase-Sts',
```

### Comparing `siriuspy-2.76.1/siriuspy/devices/injctrl.py` & `siriuspy-2.77.0/siriuspy/devices/injctrl.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/siriuspy/devices/injsys.py` & `siriuspy-2.77.0/siriuspy/devices/injsys.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/siriuspy/devices/lienergy.py` & `siriuspy-2.77.0/siriuspy/devices/lienergy.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/siriuspy/devices/lillrf.py` & `siriuspy-2.77.0/siriuspy/devices/lillrf.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/siriuspy/devices/machshift.py` & `siriuspy-2.77.0/siriuspy/devices/machshift.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/siriuspy/devices/modltr.py` & `siriuspy-2.77.0/siriuspy/devices/modltr.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/siriuspy/devices/orbit_interlock.py` & `siriuspy-2.77.0/siriuspy/devices/orbit_interlock.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/siriuspy/devices/posang.py` & `siriuspy-2.77.0/siriuspy/devices/posang.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/siriuspy/devices/psconv.py` & `siriuspy-2.77.0/siriuspy/devices/psconv.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/siriuspy/devices/pssofb.py` & `siriuspy-2.77.0/siriuspy/devices/pssofb.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/siriuspy/devices/pstesters.py` & `siriuspy-2.77.0/siriuspy/devices/pstesters.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/siriuspy/devices/pwrsupply.py` & `siriuspy-2.77.0/siriuspy/devices/pwrsupply.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/siriuspy/devices/rf.py` & `siriuspy-2.77.0/siriuspy/devices/rf.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/siriuspy/devices/screen.py` & `siriuspy-2.77.0/siriuspy/devices/screen.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/siriuspy/devices/sofb.py` & `siriuspy-2.77.0/siriuspy/devices/sofb.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/siriuspy/devices/syncd.py` & `siriuspy-2.77.0/siriuspy/devices/syncd.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/siriuspy/devices/timing.py` & `siriuspy-2.77.0/siriuspy/devices/timing.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/siriuspy/devices/tune.py` & `siriuspy-2.77.0/siriuspy/devices/tune.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/siriuspy/diagbeam/bpm/csdev.py` & `siriuspy-2.77.0/siriuspy/diagbeam/bpm/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/siriuspy/diagbeam/dcct/csdev.py` & `siriuspy-2.77.0/siriuspy/diagbeam/dcct/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/siriuspy/diagbeam/ict/csdev.py` & `siriuspy-2.77.0/siriuspy/diagbeam/ict/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/siriuspy/diagbeam/screen/csdev.py` & `siriuspy-2.77.0/siriuspy/diagbeam/screen/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/siriuspy/diagbeam/slit/csdev.py` & `siriuspy-2.77.0/siriuspy/diagbeam/slit/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/siriuspy/diagsys/app.py` & `siriuspy-2.77.0/siriuspy/diagsys/app.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,27 +2,28 @@
 """Application module."""
 
 import time as _time
 from threading import Thread as _Thread
 
 from ..envars import VACA_PREFIX as _VACA_PREFIX
 from ..callbacks import Callback as _Callback
-from ..thread import QueueThread as _QueueThread
+from ..thread import LoopQueueThread as _LoopQueueThread
 
 
 class App(_Callback):
     """Main application responsible for updating DB."""
 
     SCAN_FREQUENCY = 2
 
     def __init__(self, *args):
         """Create Computed PVs."""
         super().__init__()
         self._prefix = _VACA_PREFIX
-        self._queue = _QueueThread()
+        self._queue = _LoopQueueThread()
+        self._queue.start()
         self.pvs = list()
         self.scanning = False
         self.quit = False
         self._create_computed_pvs(*args)
 
         self.thread = _Thread(target=self.scan, daemon=True)
         self.thread.start()
```

### Comparing `siriuspy-2.76.1/siriuspy/diagsys/lidiag/csdev.py` & `siriuspy-2.77.0/siriuspy/diagsys/lidiag/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/siriuspy/diagsys/lidiag/main.py` & `siriuspy-2.77.0/siriuspy/diagsys/lidiag/main.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/siriuspy/diagsys/lidiag/pvs.py` & `siriuspy-2.77.0/siriuspy/diagsys/lidiag/pvs.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/siriuspy/diagsys/psdiag/csdev.py` & `siriuspy-2.77.0/siriuspy/diagsys/psdiag/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/siriuspy/diagsys/psdiag/main.py` & `siriuspy-2.77.0/siriuspy/diagsys/psdiag/main.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/siriuspy/diagsys/psdiag/pvs.py` & `siriuspy-2.77.0/siriuspy/diagsys/psdiag/pvs.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/siriuspy/diagsys/pudiag/csdev.py` & `siriuspy-2.77.0/siriuspy/diagsys/pudiag/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/siriuspy/diagsys/pudiag/main.py` & `siriuspy-2.77.0/siriuspy/diagsys/pudiag/main.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/siriuspy/diagsys/pudiag/pvs.py` & `siriuspy-2.77.0/siriuspy/diagsys/pudiag/pvs.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/siriuspy/diagsys/pvs.py` & `siriuspy-2.77.0/siriuspy/diagsys/pvs.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,16 +17,15 @@
 
     def __init__(self, pvname, computer, queue, pvs, monitor=True):
         """Initialize PVs."""
         # print('compute_pv: ', pvname, pvs)
 
         # starts computer_pvs queue, if not started yet
         self._queue = queue
-        if not self._queue.running:
-            self._queue.start()
+        self._queue.start()
 
         # --- properties ---
 
         self.pvname = pvname
         self._value = None
         self._set_limits((None,)*6)
         self.computer = computer
@@ -188,12 +187,12 @@
                 kwargs['lolo'] != self.lower_alarm_limit:
             self._process_new_value(kwargs)
 
     def _value_update_callback(self, pvname, value, **kwargs):
         # if 'Current-Mon' not in pvname:
         #     print(pvname, value)
         if self.connected:
-            self._queue.add_callback(self._update_value, pvname, value)
+            self._queue.put((self._update_value, (pvname, value)), block=False)
 
     def _issue_callback(self, **kwargs):
         for callback in self._callbacks.values():
             callback(**kwargs)
```

### Comparing `siriuspy-2.76.1/siriuspy/diagsys/rfdiag/csdev.py` & `siriuspy-2.77.0/siriuspy/diagsys/rfdiag/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/siriuspy/diagsys/rfdiag/main.py` & `siriuspy-2.77.0/siriuspy/diagsys/rfdiag/main.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/siriuspy/diagsys/rfdiag/pvs.py` & `siriuspy-2.77.0/siriuspy/diagsys/rfdiag/pvs.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/siriuspy/dvfimgproc/csdev.py` & `siriuspy-2.77.0/siriuspy/dvfimgproc/csdev.py`

 * *Files 6% similar despite different names*

```diff
@@ -59,26 +59,27 @@
         database.update(self._get_others_db())
         database = _csdev.add_pvslist_cte(database)
 
         # rename Properties-Cte to ImgProperties-Cte
         database['ImgProperties-Cte'] = database['Properties-Cte']
         del database['Properties-Cte']
 
-        # TODO: Version here will take value from siriuspy package
-        # Is this what we want? maybe we should start composing the string
-        # from siriuspy + machine-applications?
+        # TODO: When the known bug related to the use of get_last_commit_hash
+        # for determining application version is solved, maybe the value of
+        # this PV should be composed in the driver layer, using the values of
+        # siriuspy + machine-applicaions versions.
         database['ImgVersion-Cte'] = {
             'type': 'string',
             'value': _util.get_last_commit_hash()
         }
 
         return database
 
     def _get_image_db(self):
-        dvf_params = _DVF.conv_devname2parameters[self.devname]
+        dvf_params = _DVF.conv_devname2parameters(self.devname)
         sufix = '-Mon'
         dbase = {
             'ImgDVFSizeX-Cte': {
                 'type': 'int', 'unit': 'px'
             },
             'ImgDVFSizeY-Cte': {
                 'type': 'int', 'unit': 'px'
@@ -114,15 +115,15 @@
             },
             'ImgIsWithBeamThreshold-SP': {
                 'type': 'int', 'unit': 'intensity', 'value': 10,
             },
             'ImgIsWithBeamThreshold-RB': {
                 'type': 'int', 'unit': 'intensity', 'value': 10,
             },
-            }
+        }
         return dbase
 
     def _get_roi_db(self):
         db = {}
         rb_ = '-RB'
         sp_ = '-SP'
         mon_ = '-Mon'
@@ -194,15 +195,15 @@
                 'type': 'enum', 'enums': _et.NO_YES,
                 'value': self.NoYes.No,
             },
             'ImgFitAngleUseCMomSVD-Sts': {
                 'type': 'enum', 'enums': _et.NO_YES,
                 'value': self.NoYes.No,
             },
-            })
+        })
         return db
 
     def _get_others_db(self):
         db = {}
         db.update({
             'ImgVersion-Cte': {
                 'type': 'string',
@@ -228,10 +229,10 @@
             'ImgDVFStatus-Mon': {
                 'type': 'int', 'value': 0b11111111,
             },
             'ImgDVFStatusLabels-Cte': {
                 'type': 'string', 'count': len(self.StsLblsDVF._fields),
                 'value': self.StsLblsDVF._fields,
             },
-            })
+        })
 
         return db
```

### Comparing `siriuspy-2.76.1/siriuspy/dvfimgproc/main.py` & `siriuspy-2.77.0/siriuspy/dvfimgproc/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Module with main IOC Class."""
 
 import time as _time
 import logging as _log
+import numpy as _np
 
 from pcaspy import Alarm as _Alarm
 from pcaspy import Severity as _Severity
 
 from .. import util as _util
 
 from .meas import MeasDVF
@@ -13,58 +14,58 @@
 
 class App:
     """BL Image Processing IOC Application."""
 
     CHECK_IMG_ACQUIRE = True
 
     _MON_PVS_2_IMGFIT = {
-            # These PVs are updated at evry image processing
-            # --- image intensity ---
-            'ImgSizeX-Mon': ('fitx', 'size'),
-            'ImgSizeY-Mon': ('fity', 'size'),
-            'ImgIntensityMin-Mon': 'intensity_min',
-            'ImgIntensityMax-Mon': 'intensity_max',
-            'ImgIntensitySum-Mon': 'intensity_sum',
-            'ImgIsSaturated-Mon': 'is_saturated',
-            # --- image projection ---
-            'ImgProjX-Mon': ('imagex', 'data'),
-            'ImgProjY-Mon': ('imagey', 'data'),
-            'ImgIsWithBeam-Mon': 'is_with_image',
-            # --- roix ---
-            'ImgROIX-RB': ('fitx', 'roi'),
-            'ImgROIXCenter-Mon': ('fitx', 'roi_center'),
-            'ImgROIXFWHM-Mon': ('fitx', 'roi_fwhm'),
-            # --- roix_fit ---
-            'ImgROIXFitAmplitude-Mon': ('fitx', 'roi_amplitude'),
-            'ImgROIXFitMean-Mon': ('fitx', 'roi_mean'),
-            'ImgROIXFitSigma-Mon': ('fitx', 'roi_sigma'),
-            'ImgROIXFitError-Mon': ('fitx', 'roi_fit_error'),
-            # --- roixy ---
-            'ImgROIY-RB': ('fity', 'roi'),
-            'ImgROIYCenter-Mon': ('fity', 'roi_center'),
-            'ImgROIYFWHM-Mon': ('fity', 'roi_fwhm'),
-            # --- roiy_fit ---
-            'ImgROIYFitAmplitude-Mon': ('fity', 'roi_amplitude'),
-            'ImgROIYFitMean-Mon': ('fity', 'roi_mean'),
-            'ImgROIYFitSigma-Mon': ('fity', 'roi_sigma'),
-            'ImgROIYFitError-Mon': ('fity', 'roi_fit_error'),
-            # --- gauss2d fit ---
-            'ImgFitAngle-Mon': 'angle',
-            'ImgFitSigma1-Mon': 'sigma1',
-            'ImgFitSigma2-Mon': 'sigma2',
-        }
+        # These PVs are updated at evry image processing
+        # --- image intensity ---
+        'ImgSizeX-Mon': ('fitx', 'size'),
+        'ImgSizeY-Mon': ('fity', 'size'),
+        'ImgIntensityMin-Mon': 'intensity_min',
+        'ImgIntensityMax-Mon': 'intensity_max',
+        'ImgIntensitySum-Mon': 'intensity_sum',
+        'ImgIsSaturated-Mon': 'is_saturated',
+        # --- image projection ---
+        'ImgProjX-Mon': ('fitx', 'data'),
+        'ImgProjY-Mon': ('fity', 'data'),
+        'ImgIsWithBeam-Mon': 'is_with_image',
+        # --- roix ---
+        'ImgROIX-RB': ('fitx', 'roi'),
+        'ImgROIXCenter-Mon': ('fitx', 'roi_center'),
+        'ImgROIXFWHM-Mon': ('fitx', 'roi_fwhm'),
+        # --- roix_fit ---
+        'ImgROIXFitAmplitude-Mon': ('fitx', 'roi_amplitude'),
+        'ImgROIXFitMean-Mon': ('fitx', 'roi_mean'),
+        'ImgROIXFitSigma-Mon': ('fitx', 'roi_sigma'),
+        'ImgROIXFitError-Mon': ('fitx', 'roi_fit_error'),
+        # --- roixy ---
+        'ImgROIY-RB': ('fity', 'roi'),
+        'ImgROIYCenter-Mon': ('fity', 'roi_center'),
+        'ImgROIYFWHM-Mon': ('fity', 'roi_fwhm'),
+        # --- roiy_fit ---
+        'ImgROIYFitAmplitude-Mon': ('fity', 'roi_amplitude'),
+        'ImgROIYFitMean-Mon': ('fity', 'roi_mean'),
+        'ImgROIYFitSigma-Mon': ('fity', 'roi_sigma'),
+        'ImgROIYFitError-Mon': ('fity', 'roi_fit_error'),
+        # --- gauss2d fit ---
+        'ImgFitAngle-Mon': 'angle',
+        'ImgFitSigma1-Mon': 'sigma1',
+        'ImgFitSigma2-Mon': 'sigma2',
+    }
 
     _INIT_PVS_2_IMGFIT = {
-            # These are either constant PVs or readback PVs whose
-            # initializations need external input
-            'ImgROIX-RB': ('fitx', 'roi'),
-            'ImgROIY-RB': ('fity', 'roi'),
-            'ImgROIX-SP': ('fitx', 'roi'),
-            'ImgROIY-SP': ('fity', 'roi'),
-        }
+        # These are either constant PVs or readback PVs whose
+        # initializations need external input
+        'ImgROIX-RB': ('fitx', 'roi'),
+        'ImgROIY-RB': ('fity', 'roi'),
+        'ImgROIX-SP': ('fitx', 'roi'),
+        'ImgROIY-SP': ('fity', 'roi'),
+    }
 
     def __init__(self, driver=None, const=None):
         """Initialize the instance."""
         self._driver = driver
         self._const = const
         self._database = const.get_database()
         self._heartbeat = 0
@@ -270,38 +271,38 @@
         else:
             new_value = value
         return invalid_fit, new_value
 
     def _create_meas(self):
         # build arguments
         fwhmx_factor = \
-            self._database['ImgROIXUpdateWithFWHMFactor-RB']['value']
+            float(self._database['ImgROIXUpdateWithFWHMFactor-RB']['value'])
         fwhmy_factor = \
-            self._database['ImgROIYUpdateWithFWHMFactor-RB']['value']
+            float(self._database['ImgROIYUpdateWithFWHMFactor-RB']['value'])
         roi_with_fwhm = \
-            self._database['ImgROIUpdateWithFWHM-Sts']['value']
+            float(self._database['ImgROIUpdateWithFWHM-Sts']['value'])
         intensity_threshold = \
-            self._database['ImgIsWithBeamThreshold-RB']['value']
+            int(self._database['ImgIsWithBeamThreshold-RB']['value'])
         use_svd4theta = \
-            self._database['ImgFitAngleUseCMomSVD-Sts']['value']
+            int(self._database['ImgFitAngleUseCMomSVD-Sts']['value'])
 
         # create object
         meas = MeasDVF(
             self.const.devname,
             fwhmx_factor=fwhmx_factor, fwhmy_factor=fwhmy_factor,
             roi_with_fwhm=roi_with_fwhm,
             intensity_threshold=intensity_threshold,
             use_svd4theta=use_svd4theta,
-            )
+        )
         return meas
 
     def _write_pv(self, pvname, value=None, success=True):
         """."""
         if success:
-            if value in (True, False):
+            if isinstance(value, (bool, _np.bool, _np.bool_)):
                 value = 1 if value else 0
             try:
                 self._driver.setParam(pvname, value)
                 self._driver.updatePV(pvname)
             except TypeError:
                 _log.warning(
                     '_write_pv: error in updatePV for ', pvname, value)
@@ -422,15 +423,15 @@
         message = f'[{self.heartbeat}] ' + message
         _log.warning(message)
 
     def _write_fwhm_factor(self, reason, value):
         if reason not in (
                 'ImgROIXUpdateWithFWHMFactor-SP',
                 'ImgROIYUpdateWithFWHMFactor-SP'
-                ):
+        ):
             return None
         if 'X' in reason:
             self.meas.fwhmx_factor = value
         else:
             self.meas.fwhmy_factor = value
         self._write_pv_sp_rb(reason, value)
```

### Comparing `siriuspy-2.76.1/siriuspy/dvfimgproc/meas.py` & `siriuspy-2.77.0/siriuspy/dvfimgproc/meas.py`

 * *Files 0% similar despite different names*

```diff
@@ -132,14 +132,15 @@
     def acquisition_timeout(self, interval):
         """Check if given interval defines an image update timeout."""
         if self.dvf.acquisition_time:
             return interval > 10 * self.dvf.acquisition_time
         return False
 
     def reset_dvf(self):
+        """Reset DVF."""
         if self.dvf.connected:
             return self._dvf.cmd_reset()
         else:
             return False
 
     def set_acquire(self):
         """."""
```

### Comparing `siriuspy-2.76.1/siriuspy/envars.py` & `siriuspy-2.77.0/siriuspy/envars.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/siriuspy/epics/multiproc.py` & `siriuspy-2.77.0/siriuspy/epics/multiproc.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/siriuspy/epics/properties.py` & `siriuspy-2.77.0/siriuspy/epics/properties.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/siriuspy/epics/pv_fake.py` & `siriuspy-2.77.0/siriuspy/epics/pv_fake.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/siriuspy/epics/pv_time_serie.py` & `siriuspy-2.77.0/siriuspy/epics/pv_time_serie.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/siriuspy/fofb/csdev.py` & `siriuspy-2.77.0/siriuspy/fofb/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/siriuspy/fofb/main.py` & `siriuspy-2.77.0/siriuspy/fofb/main.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/siriuspy/idff/config.py` & `siriuspy-2.77.0/siriuspy/idff/config.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/siriuspy/idff/csdev.py` & `siriuspy-2.77.0/siriuspy/idff/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/siriuspy/idff/main.py` & `siriuspy-2.77.0/siriuspy/idff/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import epics as _epics
 import numpy as _np
 
 from PRUserial485 import EthBridgeClient as _EthBridgeClient
 
 from ..util import update_bit as _updt_bit
 from ..callbacks import Callback as _Callback
+from ..clientconfigdb import ConfigDBException as _ConfigDBException
 from ..devices import IDFF as _IDFF
 from ..pwrsupply.pssofb import PSConnSOFB as _PSConnSOFB
 from ..pwrsupply.pssofb import PSNamesSOFB as _PSNamesSOFB
 
 from .csdev import IDFFConst as _Const, ETypes as _ETypes
 
 
@@ -62,24 +63,27 @@
     def init_database(self):
         """Set initial PV values."""
         pvn2vals = {
             'LoopState-Sel': self._loop_state,
             'LoopState-Sts': self._loop_state,
             'LoopFreq-SP': self._loop_freq,
             'LoopFreq-RB': self._loop_freq,
-            'ControlQS-Sel': self._control_qs,
-            'ControlQS-Sts': self._control_qs,
             'ConfigName-SP': self._config_name,
             'ConfigName-RB': self._config_name,
             'Polarization-Mon': self._polarization,
             'SOFBMode-Sel': self._pssofb_isused,
             'SOFBMode-Sts': self._pssofb_isused,
             'CorrConfig-Cmd': 0,
             'CorrStatus-Mon': 0b1111,
         }
+        if self._const.has_qscorrs:
+            pvn2vals.ipdate({
+                'ControlQS-Sel': self._control_qs,
+                'ControlQS-Sts': self._control_qs,
+                })
         for pvn, val in pvn2vals.items():
             self.run_callbacks(pvn, val)
         self._update_log('Started.')
 
     @property
     def pvs_prefix(self):
         """Return pvs_prefix."""
@@ -92,17 +96,18 @@
 
     def process(self, interval):
         """Sleep."""
         # check correctors state periodically
         _t0 = _time.time()
         self._update_corr_status()
         dtime = _time.time() - _t0
+        sleep_time = interval - dtime
         # sleep
-        if dtime > 0:
-            _time.sleep(interval - dtime)
+        if sleep_time > 0:
+            _time.sleep(sleep_time)
         else:
             _log.debug('process took {0:f}ms.'.format((dtime)*1000))
 
     def read(self, reason):
         """Read from IOC database."""
         value = None
         return value
@@ -202,15 +207,15 @@
 
         return True
 
     def _load_config(self, config_name):
         try:
             self._idff.load_config(config_name)
             self._update_log(f'Updated configuration: {config_name}.')
-        except ValueError as err:
+        except (ValueError, _ConfigDBException) as err:
             self._update_log('ERR:'+str(err))
             return False
         return True
 
     @property
     def quit(self):
         """Quit and shutdown threads."""
@@ -260,14 +265,16 @@
         _os.makedirs(path, exist_ok=True)
         with open(self._const.autosave_fname, 'w+') as fil:
             fil.write(self._config_name)
 
     def _get_default_configname(self):
         if self._const.idname.dev == 'EPU50':
             return 'epu50_ref'
+        elif self._const.idname.dev == 'PAPU50':
+            return 'papu50_ref'
         return ''
 
     # ----- update pvs methods -----
 
     def _do_sleep(self, time0, tplanned):
         ttook = _time.time() - time0
         tsleep = tplanned - ttook
```

### Comparing `siriuspy-2.76.1/siriuspy/injctrl/bias_feedback.py` & `siriuspy-2.77.0/siriuspy/injctrl/bias_feedback.py`

 * *Files 2% similar despite different names*

```diff
@@ -258,24 +258,24 @@
             self.bias_data, self.linmodel_coeffs_inverse)
 
         x = self.bias_data[:, None].copy()
         y = self.injc_data[:, None].copy()
 
         kernel = gpy.kern.RBF(input_dim=1)
         db_ = self.database['BiasFBGPModKernStd-RB']
-        kernel.variance.constrain_bounded(db_['low']**2, db_['high']**2)
+        kernel.variance.constrain_bounded(db_['lolim']**2, db_['hilim']**2)
         kernel.variance = db_['value']**2
         db_ = self.database['BiasFBGPModKernLenScl-RB']
-        kernel.lengthscale.constrain_bounded(db_['low'], db_['high'])
+        kernel.lengthscale.constrain_bounded(db_['lolim'], db_['hilim'])
         kernel.lengthscale = db_['value']
 
         gpmodel = gpy.models.GPRegression(x, y, kernel)
         db_ = self.database['BiasFBGPModNoiseStd-RB']
         gpmodel.likelihood.variance.constrain_bounded(
-            db_['low']**2, db_['high']**2)
+            db_['lolim']**2, db_['hilim']**2)
         gpmodel.likelihood.variance = db_['value']**2
         self.gpmodel = gpmodel
         self._update_predictions()
 
     def _update_data(self, **kwgs):
         bias = self._injctrl.egun_dev.bias.voltage
         dcurr = kwgs['value']
```

### Comparing `siriuspy-2.76.1/siriuspy/injctrl/csdev.py` & `siriuspy-2.77.0/siriuspy/injctrl/csdev.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,21 +4,22 @@
 
 
 # --- Enumeration Types ---
 
 class ETypes(_csdev.ETypes):
     """Local enumerate types."""
 
-    INJMODE = ('Decay', 'TopUp')
+    INJMODE = ('Decay', 'TopUp', 'Accum')
     INJTYPE = ('SingleBunch', 'MultiBunch')
     INJTYPE_MON = INJTYPE + ('Undefined', )
     PUMODE = ('Accumulation', 'Optimization', 'OnAxis')
     PUMODE_MON = PUMODE + ('Undefined', )
     TOPUPSTS = (
         'Off', 'Waiting', 'TurningOn', 'Injecting', 'TurningOff', 'Skipping')
+    ACCUMSTS = ('Off', 'Waiting', 'TurningOn', 'Injecting')
     INJSYSCMDSTS = ('Idle', 'On', 'Off')
     RFKILLBEAMMON = ('Idle', 'Kill')
     IDLERUNNING = ('Idle', 'Running')
     IDLEINJECTING = ('Idle', 'Injecting')
     BIASFB_MODEL_TYPES = ('Linear', 'GaussianProcess')
     STANDBY_INJECT = ('Standby', 'Inject')
 
@@ -33,14 +34,15 @@
 
     InjMode = _csdev.Const.register('InjMode', _et.INJMODE)
     InjType = _csdev.Const.register('InjType', _et.INJTYPE)
     InjTypeMon = _csdev.Const.register('InjTypeMon', _et.INJTYPE_MON)
     PUMode = _csdev.Const.register('PUMode', _et.PUMODE)
     PUModeMon = _csdev.Const.register('PUModeMon', _et.PUMODE_MON)
     TopUpSts = _csdev.Const.register('TopUpSts', _et.TOPUPSTS)
+    AccumSts = _csdev.Const.register('AccumSts', _et.ACCUMSTS)
     InjSysCmdSts = _csdev.Const.register('InjSysCmdSts', _et.INJSYSCMDSTS)
     RFKillBeamMon = _csdev.Const.register('RFKillBeamMon', _et.RFKILLBEAMMON)
     IdleRunning = _csdev.Const.register('IdleRunning', _et.IDLERUNNING)
     IdleInjecting = _csdev.Const.register('IdleInjecting', _et.IDLEINJECTING)
     BiasFBModelTypes = _csdev.Const.register(
         'ModelTypes', _et.BIASFB_MODEL_TYPES)
     StandbyInject = _csdev.Const.register('StandbyInject', _et.STANDBY_INJECT)
@@ -243,25 +245,38 @@
         'IsInjDuration-SP': {
             'type': 'int', 'value': 300, 'unit': 'ms',
             'lolim': 0, 'hilim': 1000},
         'IsInjDuration-RB': {
             'type': 'int', 'value': 300, 'unit': 'ms',
             'lolim': 0, 'hilim': 1000},
 
+        'AccumState-Sel': {
+            'type': 'enum', 'value': _ct.OffOn.Off,
+            'enums': _et.OFF_ON, 'unit': 'Off_On'},
+        'AccumState-Sts': {
+            'type': 'enum', 'value': _ct.AccumSts.Off, 'enums': _et.ACCUMSTS,
+            'unit': 'Off_Wai_TOn_Inj_TOff_Skip'},
+        'AccumPeriod-SP': {
+            'type': 'int', 'value': 5, 'unit': 's',
+            'lolim': 1, 'hilim': 60*60},
+        'AccumPeriod-RB': {
+            'type': 'int', 'value': 5, 'unit': 's',
+            'lolim': 1, 'hilim': 60*60},
+
         'TopUpState-Sel': {
             'type': 'enum', 'value': _ct.OffOn.Off,
             'enums': _et.OFF_ON, 'unit': 'Off_On'},
         'TopUpState-Sts': {
             'type': 'enum', 'value': _ct.TopUpSts.Off, 'enums': _et.TOPUPSTS,
             'unit': 'Off_Wai_TOn_Inj_TOff_Skip'},
         'TopUpPeriod-SP': {
-            'type': 'int', 'value': 5, 'unit': 'min',
+            'type': 'int', 'value': 3, 'unit': 'min',
             'lolim': 1, 'hilim': 6*60},
         'TopUpPeriod-RB': {
-            'type': 'int', 'value': 5, 'unit': 'min',
+            'type': 'int', 'value': 3, 'unit': 'min',
             'lolim': 1, 'hilim': 6*60},
         'TopUpHeadStartTime-SP': {
             'type': 'float', 'value': 0, 'unit': 's', 'prec': 2,
             'lolim': 0, 'hilim': 2*60},
         'TopUpHeadStartTime-RB': {
             'type': 'float', 'value': 0, 'unit': 's', 'prec': 2,
             'lolim': 0, 'hilim': 2*60},
@@ -392,90 +407,68 @@
     return dbase
 
 
 def get_biasfb_database():
     """."""
     dbase = {
         'LoopState-Sel': {
-            'type': 'enum', 'value': _ct.OffOn.Off, 'enums': _et.OFF_ON,
+            'type': 'enum', 'value': _ct.OffOn.On, 'enums': _et.OFF_ON,
             'unit': 'Off_On'},
         'LoopState-Sts': {
-            'type': 'enum', 'value': _ct.OffOn.Off, 'enums': _et.OFF_ON,
+            'type': 'enum', 'value': _ct.OffOn.On, 'enums': _et.OFF_ON,
             'unit': 'Off_On'},
         'MinVoltage-SP': {
             'type': 'float', 'value': -52, 'unit': 'V',
-            'prec': 1, 'lolim': -120, 'low': -120, 'lolo': -120,
-            'hilim': -30.0, 'high': -30.0, 'hihi': -30.0},
+            'prec': 1, 'lolim': -120, 'hilim': -30.0},
         'MinVoltage-RB': {
             'type': 'float', 'value': -52, 'unit': 'V',
-            'prec': 1, 'lolim': -120, 'low': -120, 'lolo': -120,
-            'hilim': -30.0, 'high': -30.0, 'hihi': -30.0},
+            'prec': 1, 'lolim': -120, 'hilim': -30.0},
         'MaxVoltage-SP': {
-            'type': 'float', 'value': -40, 'unit': 'V',
-            'prec': 1, 'lolim': -120, 'low': -120, 'lolo': -120,
-            'hilim': -30.0, 'high': -30.0, 'hihi': -30.0},
+            'type': 'float', 'value': -45, 'unit': 'V',
+            'prec': 1, 'lolim': -120, 'hilim': -30.0},
         'MaxVoltage-RB': {
-            'type': 'float', 'value': -40, 'unit': 'V',
-            'prec': 1, 'lolim': -120, 'low': -120, 'lolo': -120,
-            'hilim': -30.0, 'high': -30.0, 'hihi': -30.0},
+            'type': 'float', 'value': -45, 'unit': 'V',
+            'prec': 1, 'lolim': -120, 'hilim': -30.0},
 
         'ModelType-Sel': {
             'type': 'enum', 'value': _ct.BiasFBModelTypes.GaussianProcess,
             'enums': _et.BIASFB_MODEL_TYPES, 'unit': 'Lin_GP'},
         'ModelType-Sts': {
             'type': 'enum', 'value': _ct.BiasFBModelTypes.GaussianProcess,
             'enums': _et.BIASFB_MODEL_TYPES, 'unit': 'Lin_GP'},
         'ModelMaxNrPts-SP': {
             'type': 'int', 'value': 20, 'unit': '#',
-            'lolim': 2, 'low': 2, 'lolo': 2,
-            'hilim': _ct.BIASFB_MAX_DATA_SIZE,
-            'high': _ct.BIASFB_MAX_DATA_SIZE,
-            'hihi': _ct.BIASFB_MAX_DATA_SIZE},
+            'lolim': 2, 'hilim': _ct.BIASFB_MAX_DATA_SIZE},
         'ModelMaxNrPts-RB': {
             'type': 'int', 'value': 20, 'unit': '#',
-            'lolim': 0, 'low': 0, 'lolo': 0,
-            'hilim': _ct.BIASFB_MAX_DATA_SIZE,
-            'high': _ct.BIASFB_MAX_DATA_SIZE,
-            'hihi': _ct.BIASFB_MAX_DATA_SIZE},
+            'lolim': 2, 'hilim': _ct.BIASFB_MAX_DATA_SIZE},
         'ModelNrPts-Mon': {
             'type': 'int', 'value': 20, 'unit': '#',
-            'lolim': 2, 'low': 2, 'lolo': 2,
-            'hilim': _ct.BIASFB_MAX_DATA_SIZE,
-            'high': _ct.BIASFB_MAX_DATA_SIZE,
-            'hihi': _ct.BIASFB_MAX_DATA_SIZE},
+            'lolim': 2, 'hilim': _ct.BIASFB_MAX_DATA_SIZE},
         'ModelFitParamsNow-Cmd': {'type': 'int', 'value': 0},
         'ModelAutoFitParams-Sel': {
-            'type': 'enum', 'value': _ct.OffOn.Off, 'enums': _et.OFF_ON,
+            'type': 'enum', 'value': _ct.OffOn.On, 'enums': _et.OFF_ON,
             'unit': 'Off_On'},
         'ModelAutoFitParams-Sts': {
-            'type': 'enum', 'value': _ct.OffOn.Off, 'enums': _et.OFF_ON,
+            'type': 'enum', 'value': _ct.OffOn.On, 'enums': _et.OFF_ON,
             'unit': 'Off_On'},
         'ModelAutoFitEveryNrPts-SP': {
-            'type': 'int', 'value': 10, 'unit': '#',
-            'lolim': 1, 'low': 1, 'lolo': 1,
-            'hilim': _ct.BIASFB_MAX_DATA_SIZE,
-            'high': _ct.BIASFB_MAX_DATA_SIZE,
-            'hihi': _ct.BIASFB_MAX_DATA_SIZE},
+            'type': 'int', 'value': 1, 'unit': '#',
+            'lolim': 1, 'hilim': _ct.BIASFB_MAX_DATA_SIZE},
         'ModelAutoFitEveryNrPts-RB': {
-            'type': 'int', 'value': 10, 'unit': '#',
-            'lolim': 1, 'low': 1, 'lolo': 1,
-            'hilim': _ct.BIASFB_MAX_DATA_SIZE,
-            'high': _ct.BIASFB_MAX_DATA_SIZE,
-            'hihi': _ct.BIASFB_MAX_DATA_SIZE},
+            'type': 'int', 'value': 1, 'unit': '#',
+            'lolim': 1, 'hilim': _ct.BIASFB_MAX_DATA_SIZE},
         'ModelNrPtsAfterFit-Mon': {
-            'type': 'int', 'value': 10, 'unit': '#',
-            'lolim': 1, 'low': 1, 'lolo': 1,
-            'hilim': _ct.BIASFB_MAX_DATA_SIZE,
-            'high': _ct.BIASFB_MAX_DATA_SIZE,
-            'hihi': _ct.BIASFB_MAX_DATA_SIZE},
+            'type': 'int', 'value': 1, 'unit': '#',
+            'lolim': 1, 'hilim': _ct.BIASFB_MAX_DATA_SIZE},
         'ModelUpdateData-Sel': {
-            'type': 'enum', 'value': _ct.OffOn.Off, 'enums': _et.OFF_ON,
+            'type': 'enum', 'value': _ct.OffOn.On, 'enums': _et.OFF_ON,
             'unit': 'Off_On'},
         'ModelUpdateData-Sts': {
-            'type': 'enum', 'value': _ct.OffOn.Off, 'enums': _et.OFF_ON,
+            'type': 'enum', 'value': _ct.OffOn.On, 'enums': _et.OFF_ON,
             'unit': 'Off_On'},
         'ModelDataBias-SP': {
             'type': 'float', 'count': _ct.BIASFB_MAX_DATA_SIZE,
             'value': [0]*_ct.BIASFB_MAX_DATA_SIZE, 'unit': 'V'},
         'ModelDataBias-RB': {
             'type': 'float', 'count': _ct.BIASFB_MAX_DATA_SIZE,
             'value': [0]*_ct.BIASFB_MAX_DATA_SIZE, 'unit': 'V'},
@@ -489,37 +482,31 @@
             'type': 'float', 'count': _ct.BIASFB_MAX_DATA_SIZE,
             'value': [0]*_ct.BIASFB_MAX_DATA_SIZE, 'unit': 'mA'},
         'ModelDataInjCurr-Mon': {
             'type': 'float', 'count': _ct.BIASFB_MAX_DATA_SIZE,
             'value': [0]*_ct.BIASFB_MAX_DATA_SIZE, 'unit': 'mA'},
 
         'LinModAngCoeff-SP': {
-            'type': 'float', 'value': 10, 'unit': 'V/mA',
-            'prec': 2, 'lolim': 0.1, 'low': 0.1, 'lolo': 0.1,
-            'hilim': 30.0, 'high': 30.0, 'hihi': 30.0},
+            'type': 'float', 'value': 15, 'unit': 'V/mA',
+            'prec': 2, 'lolim': 0.1, 'hilim': 30.0},
         'LinModAngCoeff-RB': {
-            'type': 'float', 'value': 10, 'unit': 'V/mA',
-            'prec': 2, 'lolim': 0.1, 'low': 0.1, 'lolo': 0.1,
-            'hilim': 30.0, 'high': 30.0, 'hihi': 30.0},
+            'type': 'float', 'value': 15, 'unit': 'V/mA',
+            'prec': 2, 'lolim': 0.1, 'hilim': 30.0},
         'LinModAngCoeff-Mon': {
-            'type': 'float', 'value': 10, 'unit': 'V/mA',
-            'prec': 2, 'lolim': 0.1, 'low': 0.1, 'lolo': 0.1,
-            'hilim': 30.0, 'high': 30.0, 'hihi': 30.0},
+            'type': 'float', 'value': 15, 'unit': 'V/mA',
+            'prec': 2, 'lolim': 0.1, 'hilim': 30.0},
         'LinModOffCoeff-SP': {
             'type': 'float', 'value': -52, 'unit': 'V/mA',
-            'prec': 2, 'lolim': -120, 'low': -120, 'lolo': -120,
-            'hilim': -30.0, 'high': -30.0, 'hihi': -30.0},
+            'prec': 2, 'lolim': -120, 'hilim': -30.0},
         'LinModOffCoeff-RB': {
             'type': 'float', 'value': -52, 'unit': 'V/mA',
-            'prec': 2, 'lolim': -120, 'low': -120, 'lolo': -120,
-            'hilim': -30.0, 'high': -30.0, 'hihi': -30.0},
+            'prec': 2, 'lolim': -120, 'hilim': -30.0},
         'LinModOffCoeff-Mon': {
             'type': 'float', 'value': -52, 'unit': 'V/mA',
-            'prec': 2, 'lolim': -120, 'low': -120, 'lolo': -120,
-            'hilim': -30.0, 'high': -30.0, 'hihi': -30.0},
+            'prec': 2, 'lolim': -120, 'hilim': -30.0},
 
         # These are used to give the model inference about the bias
         # Generally ploted in Injcurr X Bias graphs
         'LinModInferenceInjCurr-Mon': {
             'type': 'float', 'count': 100, 'value': [0]*100, 'unit': 'mA'},
         'LinModInferenceBias-Mon': {
             'type': 'float', 'count': 100, 'value': [0]*100, 'unit': 'V'},
@@ -529,48 +516,39 @@
         'LinModPredBias-Mon': {
             'type': 'float', 'count': 100, 'value': [0]*100, 'unit': 'V'},
         'LinModPredInjCurrAvg-Mon': {
             'type': 'float', 'count': 100, 'value': [0]*100, 'unit': 'mA'},
 
         'GPModNoiseStd-SP': {
             'type': 'float', 'value': 0.05, 'unit': 'mA', 'prec': 4,
-            'lolim': 0.005, 'low': 0.005, 'lolo': 0.005,
-            'hilim': 0.5, 'high': 0.5, 'hihi': 0.5},
+            'lolim': 0.005, 'hilim': 0.5},
         'GPModNoiseStd-RB': {
             'type': 'float', 'value': 0.05, 'unit': 'mA', 'prec': 4,
-            'lolim': 0.005, 'low': 0.005, 'lolo': 0.005,
-            'hilim': 0.5, 'high': 0.5, 'hihi': 0.5},
+            'lolim': 0.005, 'hilim': 0.5},
         'GPModNoiseStd-Mon': {
             'type': 'float', 'value': 0.05, 'unit': 'mA', 'prec': 4,
-            'lolim': 0.005, 'low': 0.005, 'lolo': 0.005,
-            'hilim': 0.5, 'high': 0.5, 'hihi': 0.5},
+            'lolim': 0.005, 'hilim': 0.5},
         'GPModKernStd-SP': {
             'type': 'float', 'value': 0.4, 'unit': 'mA', 'prec': 3,
-            'lolim': 0.05, 'low': 0.05, 'lolo': 0.05,
-            'hilim': 1, 'high': 1, 'hihi': 1},
+            'lolim': 0.05, 'hilim': 1},
         'GPModKernStd-RB': {
             'type': 'float', 'value': 0.4, 'unit': 'mA', 'prec': 3,
-            'lolim': 0.05, 'low': 0.05, 'lolo': 0.05,
-            'hilim': 1, 'high': 1, 'hihi': 1},
+            'lolim': 0.05, 'hilim': 1},
         'GPModKernStd-Mon': {
             'type': 'float', 'value': 0.4, 'unit': 'mA', 'prec': 3,
-            'lolim': 0.05, 'low': 0.05, 'lolo': 0.05,
-            'hilim': 1, 'high': 1, 'hihi': 1},
+            'lolim': 0.05, 'hilim': 1},
         'GPModKernLenScl-SP': {
             'type': 'float', 'value': 5, 'unit': 'V', 'prec': 3,
-            'lolim': 1, 'low': 1, 'lolo': 1,
-            'hilim': 10, 'high': 10, 'hihi': 10},
+            'lolim': 1, 'hilim': 10},
         'GPModKernLenScl-RB': {
             'type': 'float', 'value': 5, 'unit': 'V', 'prec': 3,
-            'lolim': 1, 'low': 1, 'lolo': 1,
-            'hilim': 10, 'high': 10, 'hihi': 10},
+            'lolim': 1, 'hilim': 10},
         'GPModKernLenScl-Mon': {
             'type': 'float', 'value': 5, 'unit': 'V', 'prec': 3,
-            'lolim': 1, 'low': 1, 'lolo': 1,
-            'hilim': 10, 'high': 10, 'hihi': 10},
+            'lolim': 1, 'hilim': 10},
 
         # These are used to give the model inference about the bias
         # Generally ploted in Injcurr X Bias graphs
         'GPModInferenceInjCurr-Mon': {
             'type': 'float', 'count': 100, 'value': [0]*100, 'unit': 'mA'},
         'GPModInferenceBias-Mon': {
             'type': 'float', 'count': 100, 'value': [0]*100, 'unit': 'V'},
```

### Comparing `siriuspy-2.76.1/siriuspy/injctrl/main.py` & `siriuspy-2.77.0/siriuspy/injctrl/main.py`

 * *Files 7% similar despite different names*

```diff
@@ -56,38 +56,41 @@
                 'status': _Const.IdleRunning.Idle
             },
         }
         self._thread_watdev = None
         self._target_current = 100.0
         self._bucketlist_start = 1
         self._bucketlist_stop = 864
-        self._bucketlist_step = 15
+        self._bucketlist_step = 29
         self._isinj_delay = 0
         self._isinj_duration = 300
 
-        self._topup_state_sel = _Const.OffOn.Off
+        self._accum_state_sts = _Const.AccumSts.Off
+        self._accum_period = 5  # [s]
+
         self._topup_state_sts = _Const.TopUpSts.Off
-        self._topup_period = 5*60  # [s]
-        self._topup_headstarttime = 0
+        self._topup_period = 3*60  # [s]
+        self._topup_headstarttime = 2.43  # [s]
         self._topup_pustandbyenbl = _Const.DsblEnbl.Dsbl
         self._topup_puwarmuptime = 30
-        self._topup_pu_prepared = True
-        self._topup_liwarmupenbl = _Const.DsblEnbl.Dsbl
+        self._aspu_standby_state = None
+        self._topup_liwarmupenbl = _Const.DsblEnbl.Enbl
         self._topup_liwarmuptime = 30
-        self._topup_li_prepared = True
+        self._liti_warmup_state = None
         self._topup_bopsstandbyenbl = _Const.DsblEnbl.Dsbl
         self._topup_bopswarmuptime = 10
-        self._topup_bops_prepared = True
+        self._bops_standby_state = None
         self._topup_borfstandbyenbl = _Const.DsblEnbl.Dsbl
         self._topup_borfwarmuptime = 10
-        self._topup_borf_prepared = True
+        self._borf_standby_state = None
         now = _Time.now().timestamp()
         self._topup_next = now - (now % (24*60*60)) + 3*60*60
         self._topup_nrpulses = 1
-        self._topup_thread = None
+        self._topup_job = None
+        self._accum_job = None
         self._abort = False
         self._setting_mode = False
 
         self._rfkillbeam_mon = _Const.RFKillBeamMon.Idle
 
         self._thread_autostop = None
 
@@ -169,16 +172,14 @@
         self._pumode_dev = InjSysPUModeHandler(
             print_log=False, callback=self._update_dev_status)
 
         self._evg_dev = EVG()
         self._init_injevt = False
         self._evg_dev.pv_object('InjectionEvt-Sel').add_callback(
             self._callback_watch_injectionevt)
-        self._evg_dev.pv_object('RepeatBucketList-RB').add_callback(
-            self._callback_watch_repeatbucketlist)
         self._evg_dev.set_auto_monitor('TotalInjCount-Mon', True)
         self._evg_dev.pv_object('TotalInjCount-Mon').add_callback(
             self._callback_is_injecting)
 
         self._injsys_dev = InjSysStandbyHandler()
 
         self.currinfo_dev = CurrInfoSI()
@@ -188,15 +189,14 @@
         curr_pvo.connection_callbacks.append(self._callback_conn_autostop)
 
         self._pu_names = _PSSearch.get_psnames({
             'dis': 'PU', 'dev': '.*(InjKckr|EjeKckr|InjNLKckr|Sept)',
             'propty_name': '(?!:CCoil).*'})
         self._pu_devs = [PowerSupplyPU(pun) for pun in self._pu_names]
         self._pu_refvolt = list()
-        self._topup_puref_ignore = False
         for dev in self._pu_devs:
             pvo = dev.pv_object('Voltage-SP')
             self._pu_refvolt.append(pvo.value)
             pvo.add_callback(self._callback_update_pu_refvolt)
 
         self._rfkillbeam = RFKillBeam()
 
@@ -228,14 +228,16 @@
             'PUModeDpKckrKick-SP': self.set_pumode_dpkckr_kick,
             'TargetCurrent-SP': self.set_target_current,
             'BucketListStart-SP': self.set_bucketlist_start,
             'BucketListStop-SP': self.set_bucketlist_stop,
             'BucketListStep-SP': self.set_bucketlist_step,
             'IsInjDelay-SP': self.set_isinj_delay,
             'IsInjDuration-SP': self.set_isinj_duration,
+            'AccumState-Sel': self.set_accum_state,
+            'AccumPeriod-SP': self.set_accum_period,
             'TopUpState-Sel': self.set_topup_state,
             'TopUpPeriod-SP': self.set_topup_period,
             'TopUpHeadStartTime-SP': self.set_topup_headstarttime,
             'TopUpPUStandbyEnbl-Sel': self.set_topup_pustandbyenbl,
             'TopUpPUWarmUpTime-SP': self.set_topup_puwarmuptime,
             'TopUpLIWarmUpEnbl-Sel': self.set_topup_liwarmupenbl,
             'TopUpLIWarmUpTime-SP': self.set_topup_liwarmuptime,
@@ -325,15 +327,19 @@
             'BucketListStep-SP': self._bucketlist_step,
             'BucketListStep-RB': self._bucketlist_step,
             'IsInjecting-Mon': _Const.IdleInjecting.Idle,
             'IsInjDelay-SP': self._isinj_delay,
             'IsInjDelay-RB': self._isinj_delay,
             'IsInjDuration-SP': self._isinj_duration,
             'IsInjDuration-RB': self._isinj_duration,
-            'TopUpState-Sel': self._topup_state_sel,
+            'AccumState-Sel': _Const.OffOn.Off,
+            'AccumState-Sts': self._accum_state_sts,
+            'AccumPeriod-SP': self._accum_period,
+            'AccumPeriod-RB': self._accum_period,
+            'TopUpState-Sel': _Const.OffOn.Off,
             'TopUpState-Sts': self._topup_state_sts,
             'TopUpPeriod-SP': self._topup_period/60,
             'TopUpPeriod-RB': self._topup_period/60,
             'TopUpHeadStartTime-SP': self._topup_headstarttime,
             'TopUpHeadStartTime-RB': self._topup_headstarttime,
             'TopUpPUStandbyEnbl-Sel': self._topup_pustandbyenbl,
             'TopUpPUStandbyEnbl-Sts': self._topup_pustandbyenbl,
@@ -429,36 +435,45 @@
     # ----- handle writes -----
 
     def set_mode(self, value):
         """Set injection mode."""
         if not 0 <= value < len(_ETypes.INJMODE):
             return False
 
-        if value == _Const.InjMode.TopUp and \
-                self._topup_state_sts == _Const.TopUpSts.Off:
+        if value == self._mode:
+            self.run_callbacks('Mode-Sts', self._mode)
+            return True
+
+        # stop topup and accum threads:
+        if self._topup_job and self._topup_job.is_alive():
+            self._setting_mode = True
+            self._stop_topup_job()
+            self._setting_mode = False
+        if self._accum_job and self._accum_job.is_alive():
+            self._setting_mode = True
+            self._stop_accum_job()
+            self._setting_mode = False
+
+        if value != _Const.InjMode.Decay:
+            stg = 'top-up' if value == _Const.InjMode.TopUp else 'accumulation'
             self._update_log('Configuring EVG RepeatBucketList...')
             self._evg_dev['RepeatBucketList-SP'] = 1
-            self._update_log('...done. Waiting to start top-up.')
-        else:
-            if self._topup_thread and self._topup_thread.is_alive():
-                self._setting_mode = True
-                self._stop_topup_thread()
-                self._setting_mode = False
+            self._update_log(f'...done. Ready to start {stg:s}.')
 
         self._mode = value
         self.run_callbacks('Mode-Sts', self._mode)
         return True
 
     def set_type(self, value):
         """Set injection type."""
         if not 0 <= value < len(_ETypes.INJTYPE):
             return False
-        if self._mode == _Const.InjMode.TopUp:
+        if self._mode != _Const.InjMode.Decay:
             self._update_log(
-                'ERR:Turn off top-up mode before changing inj.type.')
+                f'ERR:InjType can only be changed in Decay mode.')
             return False
         if self._p2w['Type']['watcher'] is not None and \
                 self._p2w['Type']['watcher'].is_alive():
             self._update_log('WARN:Interrupting type change command..')
             self.egun_dev.cmd_abort_chg_type()
             self._p2w['Type']['watcher'].join()
 
@@ -556,17 +571,19 @@
         self._launch_watch_dev_thread()
         return True
 
     def set_pumode(self, value):
         """Set PU mode."""
         if not 0 <= value < len(_ETypes.PUMODE):
             return False
-        if self._mode == _Const.InjMode.TopUp:
+        if self._mode != _Const.InjMode.Decay:
+            topup = _Const.InjMode.TopUp
+            stg = 'top-up' if self._mode == topup else 'accumulation'
             self._update_log(
-                'ERR:Turn off top-up mode before changing PUMode.')
+                f'ERR:PUMode can only be changed in Decay mode.')
             return False
         if self._p2w['PUMode']['watcher'] is not None and \
                 self._p2w['PUMode']['watcher'].is_alive():
             self._update_log('WARN:Interrupting PUMode change command')
             self._pumode_dev.cmd_abort()
             self._p2w['PUMode']['watcher'].join()
 
@@ -584,15 +601,15 @@
         self._p2w['PUMode']['status'] = _Const.IdleRunning.Running
         self.run_callbacks('PUModeCmdSts-Mon', self._p2w['PUMode']['status'])
 
         self._launch_watch_dev_thread()
         return True
 
     def set_pumode_delta_posang(self, value):
-        """Set PU mode delta posang"""
+        """Set PU mode delta posang."""
         self._pumode_dev.delta_posang = value
         self.run_callbacks('PUModeDeltaPosAng-RB', value)
         return True
 
     def set_pumode_dpkckr_dlyref(self, value):
         """Set PU mode DpKckr delay."""
         self._pumode_dev.dpkckr_dlyref = value
@@ -615,40 +632,40 @@
 
     def set_bucketlist_start(self, start):
         """Set bucketlist_start."""
         if not _Const.MIN_BKT <= start <= _Const.MAX_BKT:
             return False
         stop = self._bucketlist_stop
         step = self._bucketlist_step
-        if self._mode != _Const.InjMode.TopUp:
+        if self._mode == _Const.InjMode.TopUp:
             if not self._cmd_bucketlist_fill(stop, start, step):
                 return False
         self._bucketlist_start = start
         self.run_callbacks('BucketListStart-RB', start)
         return True
 
     def set_bucketlist_stop(self, stop):
         """Set bucketlist_stop."""
         if not _Const.MIN_BKT <= stop <= _Const.MAX_BKT:
             return False
         start = self._bucketlist_start
         step = self._bucketlist_step
-        if self._mode != _Const.InjMode.TopUp:
+        if self._mode == _Const.InjMode.TopUp:
             if not self._cmd_bucketlist_fill(stop, start, step):
                 return False
         self._bucketlist_stop = stop
         self.run_callbacks('BucketListStop-RB', stop)
         return True
 
     def set_bucketlist_step(self, step):
         """Set bucketlist_step."""
         if not -_Const.MAX_BKT+1 <= step <= _Const.MAX_BKT-1:
             return False
-        if self._mode == _Const.InjMode.TopUp:
-            if not self._update_bucket_list_topup(step=step):
+        if self._mode != _Const.InjMode.Decay:
+            if not self._update_bucket_list(step=step):
                 return False
         else:
             start = self._bucketlist_start
             stop = self._bucketlist_stop
             if not self._cmd_bucketlist_fill(stop, start, step):
                 return False
         self._bucketlist_step = step
@@ -687,50 +704,73 @@
         return False
 
     def set_topup_state(self, value):
         """Set top-up state."""
         if self._mode != _Const.InjMode.TopUp:
             return False
 
-        self._topup_state_sel = value
         if value == _Const.OffOn.On:
             self._update_log('Start received!')
             if not self._check_allok_2_inject():
                 return False
-            if self._topup_thread is not None and \
-                    not self._topup_thread.is_alive() or\
-                    self._topup_thread is None:
-                self._launch_topup_thread()
+            if self._topup_job is None or not self._topup_job.is_alive():
+                self._launch_topup_job()
         else:
             self._update_log('Stop received!')
-            if self._topup_thread is not None and \
-                    self._topup_thread.is_alive():
-                self._stop_topup_thread()
+            if self._topup_job is not None and \
+                    self._topup_job.is_alive():
+                self._stop_topup_job()
+        return True
+
+    def set_accum_state(self, value):
+        """Set accum state."""
+        if self._mode != _Const.InjMode.Accum:
+            return False
 
+        if value == _Const.OffOn.On:
+            self._update_log('Start received!')
+            if not self._check_allok_2_inject():
+                return False
+            if self._accum_job is None or not self._accum_job.is_alive():
+                self._launch_accum_job()
+        else:
+            self._update_log('Stop received!')
+            if self._accum_job is not None and self._accum_job.is_alive():
+                self._stop_accum_job()
         return True
 
     def set_topup_period(self, value):
         """Set top-up period [min]."""
         if not 1 <= value <= 6*60:
             return False
 
-        sec = value*60
+        sec = value * 60
         if self._topup_state_sts != _Const.TopUpSts.Off:
             now = _Time.now().timestamp()
             self._topup_next = now - (now % sec) + sec
             self.run_callbacks('TopUpNextInj-Mon', self._topup_next)
 
         self._topup_period = sec
         self._update_log('Changed top-up period to '+str(value)+'min.')
         self.run_callbacks('TopUpPeriod-RB', value)
         return True
 
+    def set_accum_period(self, value):
+        """Set accumulation period [s]."""
+        if not 1 <= value <= 60*60:
+            return False
+
+        self._accum_period = value
+        self._update_log('Changed accumulation period to '+str(value)+'s.')
+        self.run_callbacks('AccumPeriod-RB', value)
+        return True
+
     def set_topup_headstarttime(self, value):
         """Set top-up head start time [s]."""
-        if not 0 <= value <= 10*60:
+        if not 0 <= value <= 2*60:
             return False
         self._topup_headstarttime = value
         self._update_log('Changed top-up head start time to '+str(value)+'s.')
         self.run_callbacks('TopUpHeadStartTime-RB', self._topup_headstarttime)
 
         minwut = _np.ceil(value+1)
         self._topup_puwarmuptime = max(minwut, self._topup_puwarmuptime)
@@ -749,19 +789,16 @@
         return True
 
     def set_topup_pustandbyenbl(self, value):
         """Enable/disable PU standby between top-up injections."""
         if not 0 <= value < len(_ETypes.DSBL_ENBL):
             return False
 
-        if value:
-            if not self._update_topup_pu_refvolt():
-                return False
-        else:
-            self._handle_topup_pu_voltage(_Const.StandbyInject.Inject)
+        if value == _Const.DsblEnbl.Dsbl:
+            self._handle_aspu_standby_state(_Const.StandbyInject.Inject)
         self._topup_pustandbyenbl = value
         text = 'En' if value else 'Dis'
         self._update_log(text+'abled PU standby between injections.')
         self.run_callbacks('TopUpPUStandbyEnbl-Sts', self._topup_pustandbyenbl)
         return True
 
     def set_topup_puwarmuptime(self, value):
@@ -774,15 +811,15 @@
 
     def set_topup_liwarmupenbl(self, value):
         """Enable/disable LI warm up before top-up injections."""
         if not 0 <= value < len(_ETypes.DSBL_ENBL):
             return False
 
         if value == _Const.DsblEnbl.Dsbl:
-            self._handle_topup_linac_timing(state=_Const.StandbyInject.Inject)
+            self._handle_liti_warmup_state(state=_Const.StandbyInject.Inject)
         self._topup_liwarmupenbl = value
         text = 'En' if value else 'Dis'
         self._update_log(text+'abled LI warm up before injections.')
         self.run_callbacks('TopUpLIWarmUpEnbl-Sts', self._topup_liwarmupenbl)
         return True
 
     def set_topup_liwarmuptime(self, value):
@@ -795,15 +832,15 @@
 
     def set_topup_bopsstandbyenbl(self, value):
         """Enable/disable BO PS standby between top-up injections."""
         if not 0 <= value < len(_ETypes.DSBL_ENBL):
             return False
 
         if value == _Const.DsblEnbl.Dsbl:
-            self._handle_topup_bops_timing(state=_Const.StandbyInject.Inject)
+            self._handle_bops_standby_state(state=_Const.StandbyInject.Inject)
         self._topup_bopsstandbyenbl = value
         text = 'En' if value else 'Dis'
         self._update_log(text+'abled BO PS standby between injections.')
         self.run_callbacks(
             'TopUpBOPSStandbyEnbl-Sts', self._topup_bopsstandbyenbl)
         return True
 
@@ -818,15 +855,15 @@
 
     def set_topup_borfstandbyenbl(self, value):
         """Enable/disable BO RF standby between top-up injections."""
         if not 0 <= value < len(_ETypes.DSBL_ENBL):
             return False
 
         if value == _Const.DsblEnbl.Dsbl:
-            self._handle_topup_borf_timing(state=_Const.StandbyInject.Inject)
+            self._handle_borf_standby_state(state=_Const.StandbyInject.Inject)
         self._topup_borfstandbyenbl = value
         text = 'En' if value else 'Dis'
         self._update_log(text+'abled BO RF standby between injections.')
         self.run_callbacks(
             'TopUpBORFStandbyEnbl-Sts', self._topup_borfstandbyenbl)
         return True
 
@@ -842,15 +879,15 @@
     def set_topup_nrpulses(self, value):
         """Set top-up number of injection pulses."""
         if not 1 <= value <= 1000:
             return False
 
         self._topup_nrpulses = value
         if self._mode == _Const.InjMode.TopUp:
-            if not self._update_bucket_list_topup():
+            if not self._update_bucket_list():
                 return False
         self._update_log('Changed top-up nr.pulses to '+str(value)+'.')
         self.run_callbacks('TopUpNrPulses-RB', self._topup_nrpulses)
         return True
 
     def cmd_injsys_turn_on(self, value=None, wait_finish=False):
         """Set turn on Injection System."""
@@ -961,15 +998,15 @@
 
     # --- callbacks ---
 
     def _callback_watch_eguntrig(self, value, **kws):
         if not self._init_egun:
             self._init_egun = True
             return
-        if self._mode == _Const.InjMode.TopUp:
+        if self._mode != _Const.InjMode.Decay:
             return
         _epics.ca.CAThread(
             target=self._watch_eguntrig, args=[value, ], daemon=True).start()
 
     def _watch_eguntrig(self, value, **kws):
         cmd = 'on' if value else 'off'
         _t0 = _time.time()
@@ -982,15 +1019,15 @@
             msg = 'WARN:Timed out in turn '+cmd+' Egun.'
         self._update_log(msg)
 
     def _callback_watch_injectionevt(self, value, **kws):
         if not self._init_injevt:
             self._init_injevt = True
             return
-        if self._mode == _Const.InjMode.TopUp:
+        if self._mode != _Const.InjMode.Decay:
             return
         _epics.ca.CAThread(
             target=self._watch_injti, args=[value, ], daemon=True).start()
 
     def _watch_injti(self, value, timeout=_Const.TI_INJ_TIMEOUT):
         cmd = 'on' if value else 'off'
         _t0 = _time.time()
@@ -1003,40 +1040,40 @@
             msg = 'WARN:Timed out in turn '+cmd+' InjectionEvt.'
         self._update_log(msg)
 
     def _callback_autostop(self, value, **kws):
         if self._thread_autostop is not None and \
                 self._thread_autostop.is_alive():
             return
+        if value is None or value < self._target_current:
+            return
         self._thread_autostop = _epics.ca.CAThread(
             target=self._thread_run_autostop, args=[value, 'cb_val'])
         self._thread_autostop.start()
 
     def _callback_conn_autostop(self, conn, **kws):
         if self._thread_autostop is not None and \
                 self._thread_autostop.is_alive():
             return
+        if conn:
+            return
         self._thread_autostop = _epics.ca.CAThread(
             target=self._thread_run_autostop, args=[conn, 'cb_conn'])
         self._thread_autostop.start()
 
     def _thread_run_autostop(self, value, cb_type):
-        if self._mode == _Const.InjMode.TopUp:
+        if self._mode != _Const.InjMode.Decay:
             return
         if not self._evg_dev['InjectionEvt-Sel']:
             return
         if not self.egun_dev.trigps.is_on():
             return
         if cb_type == 'cb_val':
-            if value is None or value < self._target_current:
-                return
             msg = 'Target current reached!'
         else:
-            if value:
-                return
             msg = 'ERR:Current PV disconnected.'
         self._update_log(msg)
         self._run_autostop()
 
     def _run_autostop(self):
         self._update_log('Running Auto Stop...')
         if self._stop_injection():
@@ -1075,25 +1112,18 @@
         if 'init' in kws and kws['init']:
             if self._pumode_mon != _Const.PUModeMon.Undefined:
                 self._pumode = _ETypes.PUMODE.index(
                     _ETypes.PUMODE_MON[self._pumode_mon])
             self.run_callbacks('PUMode-Sel', self._pumode)
             self.run_callbacks('PUMode-Sts', self._pumode)
 
-    def _callback_watch_repeatbucketlist(self, value, **kws):
-        if self._mode == _Const.InjMode.TopUp:
-            if value != 1:
-                self._update_log('WARN:RepeatBucketList is diff. from 1.')
-                self._update_log('WARN:Aborting top-up...')
-            return
-
     def _callback_update_pu_refvolt(self, pvname, value, **kws):
         if value is None:
             return
-        if self._topup_puref_ignore:
+        if self._aspu_standby_state == _Const.StandbyInject.Standby:
             return
         devname = _PVName(pvname).device_name
         index = self._pu_names.index(devname)
         self._pu_refvolt[index] = value
 
     def _callback_is_injecting(self, value, **kws):
         if value is None:
@@ -1133,15 +1163,15 @@
 
             if self._injstatus != 0:
                 self._update_log('WARN:InjStatus not ok:')
                 for bit, prob in enumerate(_Const.INJ_STATUS_LABELS):
                     if _get_bit(self._injstatus, bit):
                         self._update_log('WARN:'+prob)
 
-        if self._mode == _Const.InjMode.TopUp:
+        if self._mode != _Const.InjMode.Decay:
             if self._evg_dev.nrpulses != 1:
                 self._update_log('ERR:Aborted. RepeatBucketList must be 1.')
                 return False
 
             if self._abort:
                 self._update_log('Abort received.')
                 return False
@@ -1206,28 +1236,29 @@
         old_bucklist = self._evg_dev.bucketlist_mon
         injcount = self._evg_dev.injection_count
         blistlen = self._evg_dev.bucketlist_len
         proll = int(injcount % blistlen)
         new_bucklist = _np.roll(old_bucklist, -1 * proll)
         return self._set_bucket_list(new_bucklist)
 
-    def _update_bucket_list_topup(self, step=None):
+    def _update_bucket_list(self, step=None, nrpulses=None):
         if not self._evg_dev.connected:
             self._update_log('ERR:Could not update bucket list,')
             self._update_log('ERR:EVG is disconnected.')
             return False
 
         if step is None:
             step = self._bucketlist_step
 
         lastfilledbucket = self._evg_dev.bucketlist_mon[-1]
         if not _Const.MIN_BKT <= lastfilledbucket <= _Const.MAX_BKT:
             lastfilledbucket = 1
 
-        bucket = _np.arange(self._topup_nrpulses) + 1
+        nrpulses = nrpulses or self._topup_nrpulses
+        bucket = _np.arange(nrpulses) + 1
         bucket *= step
         bucket += lastfilledbucket - 1
         bucket %= 864
         bucket += 1
         return self._set_bucket_list(bucket)
 
     def _set_bucket_list(self, value):
@@ -1236,42 +1267,107 @@
         while _time.time() - _t0 < 5:
             if _np.all(self._evg_dev.bucketlist == value):
                 self._update_log('Updated BucketList.')
                 return True
         self._update_log('WARN:Could not update BucketList.')
         return False
 
+    # --- auxiliary accumulation methods ---
+
+    def _launch_accum_job(self):
+        while self._abort:
+            _time.sleep(0.1)
+        self._update_log('Launching accumulation thread...')
+        self._accum_job = _epics.ca.CAThread(
+            target=self._do_accumulation, daemon=True)
+        self._accum_job.start()
+
+    def _stop_accum_job(self):
+        if self._abort:
+            return
+        self._update_log('Stopping accumulation thread...')
+        self._abort = True
+        self._accum_job.join()
+        self._accum_job = None
+        self._update_log('Stopped accumulation thread.')
+        self._abort = False
+
+    def _do_accumulation(self):
+        # update bucket list according to settings
+        self._update_bucket_list(nrpulses=1)
+
+        self._handle_aspu_standby_state(_Const.StandbyInject.Inject)
+        self._handle_liti_warmup_state(_Const.StandbyInject.Inject)
+        self._handle_bops_standby_state(_Const.StandbyInject.Inject)
+        self._handle_borf_standby_state(_Const.StandbyInject.Inject)
+
+        while self._mode == _Const.InjMode.Accum:
+            t0_ = _time.time()
+            if not self.currinfo_dev.connected:
+                self._update_log('ERR:CurrInfo device disconnected.')
+                break
+            if self.currinfo_dev.current >= self._target_current:
+                self._update_log(
+                    'Target Current reached. Stopping accumulation...')
+                break
+
+            if not self._check_allok_2_inject():
+                break
+
+            self.run_callbacks('AccumState-Sts', _Const.AccumSts.TurningOn)
+            if not self._start_injection():
+                break
+
+            self.run_callbacks('AccumState-Sts', _Const.AccumSts.Injecting)
+            if not self._wait_injection():
+                break
+            self._update_bucket_list(nrpulses=1)
+
+            dt_ = self._accum_period - (_time.time() - t0_)
+            if dt_ > 0:
+                self.run_callbacks('AccumState-Sts', _Const.AccumSts.Waiting)
+                self._update_log('Waiting for next injection...')
+                _time.sleep(dt_)
+
+        self._handle_liti_warmup_state(_Const.StandbyInject.Standby)
+
+        # update top-up status
+        self.run_callbacks('AccumState-Sts', _Const.AccumSts.Off)
+        self._update_log('Stopped accumulation loop.')
+        if not self._abort or self._setting_mode:
+            self.run_callbacks('AccumState-Sel', _Const.OffOn.Off)
+
     # --- auxiliary top-up methods ---
 
-    def _launch_topup_thread(self):
+    def _launch_topup_job(self):
         while self._abort:
             _time.sleep(0.1)
         self._update_log('Launching top-up thread...')
-        self._topup_thread = _epics.ca.CAThread(
+        self._topup_job = _epics.ca.CAThread(
             target=self._do_topup, daemon=True)
-        self._topup_thread.start()
+        self._topup_job.start()
 
-    def _stop_topup_thread(self):
+    def _stop_topup_job(self):
         if self._abort:
             return
         self._update_log('Stopping top-up thread...')
         self._abort = True
-        self._topup_thread.join()
-        self._topup_thread = None
+        self._topup_job.join()
+        self._topup_job = None
         self._update_log('Stopped top-up thread.')
         self._abort = False
 
         # reset next injection schedule
         now = _Time.now().timestamp()
         self._topup_next = now - (now % (24*60*60)) + 3*60*60
         self.run_callbacks('TopUpNextInj-Mon', self._topup_next)
 
     def _do_topup(self):
         # update bucket list according to settings
-        self._update_bucket_list_topup()
+        self._update_bucket_list()
 
         # update next injection schedule
         now, period = _Time.now().timestamp(), self._topup_period
         self._topup_next = now - (now % period) + period
         self.run_callbacks('TopUpNextInj-Mon', self._topup_next)
 
         # prepare subsystems state
@@ -1300,42 +1396,44 @@
                     break
 
                 self._update_topupsts(_Const.TopUpSts.Injecting)
                 self._update_log('Injecting...')
                 if not self._wait_injection():
                     break
 
-                self._update_topupsts(_Const.TopUpSts.TurningOff)
-                self._update_bucket_list_topup()
+                self._update_bucket_list()
             else:
                 self._update_topupsts(_Const.TopUpSts.Skipping)
                 self._update_log('Skipping injection...')
                 _time.sleep(2)
 
-            self._handle_topup_pu_voltage(_Const.StandbyInject.Standby)
-            self._handle_topup_linac_timing(_Const.StandbyInject.Standby)
-            self._handle_topup_bops_timing(_Const.StandbyInject.Standby)
-            self._handle_topup_borf_timing(_Const.StandbyInject.Standby)
+            if self._topup_pustandbyenbl:
+                self._handle_aspu_standby_state(_Const.StandbyInject.Standby)
+            if self._topup_liwarmupenbl:
+                self._handle_liti_warmup_state(_Const.StandbyInject.Standby)
+            if self._topup_bopsstandbyenbl:
+                self._handle_bops_standby_state(_Const.StandbyInject.Standby)
+            if self._topup_borfstandbyenbl:
+                self._handle_borf_standby_state(_Const.StandbyInject.Standby)
 
             self._topup_next += self._topup_period
             self.run_callbacks('TopUpNextInj-Mon', self._topup_next)
 
-        self._handle_topup_pu_voltage(_Const.StandbyInject.Inject)
-        self._handle_topup_linac_timing(_Const.StandbyInject.Inject)
-        self._handle_topup_bops_timing(_Const.StandbyInject.Inject)
-        self._handle_topup_borf_timing(_Const.StandbyInject.Inject)
+        self._handle_aspu_standby_state(_Const.StandbyInject.Inject)
+        self._handle_liti_warmup_state(_Const.StandbyInject.Standby)
+        self._handle_bops_standby_state(_Const.StandbyInject.Inject)
+        self._handle_borf_standby_state(_Const.StandbyInject.Inject)
 
         self._bias_feedback.do_update_models = False
 
         # update top-up status
         self._update_topupsts(_Const.TopUpSts.Off)
         self._update_log('Stopped top-up loop.')
         if not self._abort or self._setting_mode:
-            self._topup_state_sel = _Const.OffOn.Off
-            self.run_callbacks('TopUpState-Sel', self._topup_state_sel)
+            self.run_callbacks('TopUpState-Sel', _Const.OffOn.Off)
 
     def _wait_topup_period(self):
         while _time.time() < self._topup_next:
             if not self._check_allok_2_inject(show_warn=False):
                 return False
             _time.sleep(1)
 
@@ -1343,21 +1441,21 @@
             text = 'Remaining time: {}s'.format(remaining)
             self.run_callbacks('Log-Mon', text)
             if remaining % 60 == 0:
                 _log.info(text)
 
             # prepare subsystems
             if remaining <= self._topup_puwarmuptime:
-                self._handle_topup_pu_voltage(_Const.StandbyInject.Inject)
+                self._handle_aspu_standby_state(_Const.StandbyInject.Inject)
             if remaining <= self._topup_liwarmuptime:
-                self._handle_topup_linac_timing(_Const.StandbyInject.Inject)
+                self._handle_liti_warmup_state(_Const.StandbyInject.Inject)
             if remaining <= self._topup_bopswarmuptime:
-                self._handle_topup_bops_timing(_Const.StandbyInject.Inject)
+                self._handle_bops_standby_state(_Const.StandbyInject.Inject)
             if remaining <= self._topup_borfwarmuptime:
-                self._handle_topup_borf_timing(_Const.StandbyInject.Inject)
+                self._handle_borf_standby_state(_Const.StandbyInject.Inject)
 
             # bias fb
             cond = remaining <= _Const.BIASFB_AHEADSETIME
             cond &= bool(self._bias_feedback.loop_state)
             cond &= not self._bias_feedback.already_set
             if cond and self.currinfo_dev.connected:
                 dcur = self._bias_feedback.get_delta_current_per_pulse(
@@ -1374,110 +1472,79 @@
             if _time.time() >= self._topup_next - self._topup_headstarttime:
                 return True
 
         self._update_log('Remaining time: 0s')
         return True
 
     def _prepare_topup(self):
+        # If remaining time is too short do not put in standby or warmup
         # PU
-        if self._topup_pustandbyenbl:
-            if not self._update_topup_pu_refvolt():
-                self._update_log('ERR:...aborted top-up loop.')
-                return
-            # set PU voltage standby if remaining time is not too short
-            if self._topup_next - _time.time() > self._topup_puwarmuptime*2:
-                self._handle_topup_pu_voltage(_Const.StandbyInject.Standby)
+        standby = _Const.StandbyInject.Standby
+        if self._topup_pustandbyenbl and \
+                self._topup_next - _time.time() > self._topup_puwarmuptime*2:
+            self._handle_aspu_standby_state(standby)
 
         # LI
-        if self._topup_liwarmupenbl:
-            if self._topup_next - _time.time() > self._topup_liwarmuptime*2:
-                self._handle_topup_linac_timing(
-                    state=_Const.StandbyInject.Standby)
+        if self._topup_liwarmupenbl and \
+                self._topup_next - _time.time() > self._topup_liwarmuptime*2:
+            self._handle_liti_warmup_state(standby)
 
         # BO PS
-        if self._topup_bopsstandbyenbl:
-            if self._topup_next - _time.time() > self._topup_bopswarmuptime*2:
-                self._handle_topup_bops_timing(
-                    state=_Const.StandbyInject.Standby)
+        if self._topup_bopsstandbyenbl and \
+                self._topup_next - _time.time() > self._topup_bopswarmuptime*2:
+            self._handle_bops_standby_state(standby)
 
         # BO RF
-        if self._topup_borfstandbyenbl:
-            if self._topup_next - _time.time() > self._topup_borfwarmuptime*2:
-                self._handle_topup_borf_timing(
-                    state=_Const.StandbyInject.Standby)
-
-    def _handle_topup_pu_voltage(self, state):
-        if not self._topup_pustandbyenbl:
-            return
-        is_inj = state == _Const.StandbyInject.Inject
-        if is_inj and self._topup_pu_prepared:
-            return
-        self._topup_puref_ignore = True
-        self._topup_pu_prepared = is_inj
-        factor = 1 if is_inj else 0.5
+        if self._topup_borfstandbyenbl and \
+                self._topup_next - _time.time() > self._topup_borfwarmuptime*2:
+            self._handle_borf_standby_state(standby)
+
+    def _handle_aspu_standby_state(self, state):
+        if self._aspu_standby_state == state:
+            return
+        self._aspu_standby_state = state
+
+        factor = 1 if state == _Const.StandbyInject.Inject else 0.5
         self._update_log(f'Setting PU Voltage to {factor*100}%...')
         for idx, dev in enumerate(self._pu_devs):
             if not dev.connected:
                 self._update_log('WARN:'+dev.devname+' disconnected.')
                 continue
             dev.voltage = self._pu_refvolt[idx] * factor
         self._update_log('...done.')
-        _time.sleep(1)
-        self._topup_puref_ignore = False
 
-    def _update_topup_pu_refvolt(self):
-        # get PU voltage reference
-        for idx, dev in enumerate(self._pu_devs):
-            spv = dev['Voltage-SP']
-            if spv is None:
-                self._update_topupsts(_Const.TopUpSts.Off)
-                self._update_log('ERR:Could not read voltage of')
-                self._update_log('ERR:'+dev.devname+'...')
-                return False
-            self._pu_refvolt[idx] = dev['Voltage-SP']
-        return True
-
-    def _handle_topup_linac_timing(self, state):
-        if not self._topup_liwarmupenbl:
+    def _handle_liti_warmup_state(self, state):
+        if self._liti_warmup_state == state:
             return
-        is_inj = state == _Const.StandbyInject.Inject
-        if is_inj and self._topup_li_prepared:
-            return
-        self._topup_li_prepared = is_inj
-        event = 'RmpBO' if is_inj else 'Linac'
+        self._liti_warmup_state = state
+
+        event = 'RmpBO' if state == _Const.StandbyInject.Inject else 'Linac'
         self._hlti_dev.change_triggers_source(
             self._li_trig_names, new_src=event, printlog=False)
         self._update_log('LI timing configured.')
-        return
 
-    def _handle_topup_bops_timing(self, state):
-        if not self._topup_bopsstandbyenbl:
+    def _handle_bops_standby_state(self, state):
+        if self._bops_standby_state == state:
             return
-        is_inj = state == _Const.StandbyInject.Inject
-        if is_inj and self._topup_bops_prepared:
-            return
-        self._topup_bops_prepared = is_inj
-        trigstate = int(is_inj)
+        self._bops_standby_state = state
+
+        trigstate = int(state == _Const.StandbyInject.Inject)
         for trig in self._bops_trig_devs:
             trig.state = trigstate
         self._update_log('BO PS timing configured.')
-        return
 
-    def _handle_topup_borf_timing(self, state):
-        if not self._topup_borfstandbyenbl:
+    def _handle_borf_standby_state(self, state):
+        if self._borf_standby_state == state:
             return
-        is_inj = state == _Const.StandbyInject.Inject
-        if is_inj and self._topup_borf_prepared:
-            return
-        self._topup_borf_prepared = is_inj
-        trigstate = int(is_inj)
+        self._borf_standby_state = state
+
+        trigstate = int(state == _Const.StandbyInject.Inject)
         for trig in self._borf_trig_devs:
             trig.state = trigstate
         self._update_log('BO RF timing configured.')
-        return
 
     # --- auxiliary log methods ---
 
     def _launch_watch_dev_thread(self):
         if self._thread_watdev is None or not self._thread_watdev.is_alive():
             self._thread_watdev = _epics.ca.CAThread(
                 target=self._watch_dev_process, daemon=True)
@@ -1556,15 +1623,15 @@
                     problems = set()
                     for pvo in d2pv.values():
                         if pvo.connected:
                             value = pvo.value
                             # disregard alarms
                             if sub == 'PS':
                                 value = _np.bitwise_and(int(value), psalrm)
-                            elif self._mode == _Const.InjMode.TopUp and \
+                            elif self._mode != _Const.InjMode.Decay and \
                                     sec == 'LI' and sub == 'PU':
                                 value = _np.bitwise_and(int(value), lipualrm)
                             nok = value > 0
                         else:
                             nok = True
                         if nok:
                             problems.add(_PVName(pvo.pvname).device_name)
@@ -1609,15 +1676,15 @@
 
             # TI ContinuousEvt is off
             val = 1 if not self._evg_dev.connected else \
                 self._evg_dev.continuous_state != 1
             value = _updt_bit(value, 0, val)
 
             # BucketList not synced
-            if self._mode != _Const.InjMode.TopUp:
+            if self._mode == _Const.InjMode.Decay:
                 val = 1 if not self._evg_dev.connected else \
                     self._evg_dev.bucketlist_sync != 1
                 value = _updt_bit(value, 1, val)
 
             if self.egun_dev.connected:
                 # EGBiasPS voltage diff. from desired
                 volt = self._sglbunbiasvolt \
```

### Comparing `siriuspy-2.76.1/siriuspy/machshift/csdev.py` & `siriuspy-2.77.0/siriuspy/machshift/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/siriuspy/machshift/macreport.py` & `siriuspy-2.77.0/siriuspy/machshift/macreport.py`

 * *Files 1% similar despite different names*

```diff
@@ -249,14 +249,19 @@
         'MachineStudy',
         'Commissioning',
         'Conditioning',
         'Maintenance',
         'Users',
     ]
 
+    FAILURES_MANUAL = [
+        # power grid failure, archiver was down
+        [_Time(2023, 5, 18, 5, 55, 0, 0), _Time(2023, 5, 18, 9, 8, 0, 0)],
+    ]
+
     def __init__(self, connector=None, logger=None):
         """Initialize object."""
         # client archiver connector
         self._connector = connector or _CltArch()
 
         # auxiliary logger
         self.logger = logger
@@ -1071,15 +1076,15 @@
         """Plot raw data for period timestamp_start to timestamp_stop."""
         if not self._raw_data:
             print('No data to display. Call update() to get data.')
             return
 
         datetimes = _np.array([_Time(t) for t in self._raw_data['Timestamp']])
 
-        fig, axs = _plt.subplots(16, 1, sharex=True)
+        fig, axs = _plt.subplots(17, 1, sharex=True)
         fig.set_size_inches(9, 10)
         fig.subplots_adjust(top=0.96, left=0.08, bottom=0.05, right=0.96)
         axs[0].set_title('Raw data', fontsize=12)
 
         axs[0].xaxis.axis_date()
         axs[0].plot(
             datetimes, self._raw_data['Current'], '-',
@@ -1148,77 +1153,84 @@
             datetimes, self._raw_data['Failures']['SubsystemsNOk'], '-',
             color='red', label='Failures - PS, RF and MPS')
         axs[9].legend(loc='upper left', fontsize=9)
         axs[9].grid()
 
         axs[10].xaxis.axis_date()
         axs[10].plot(
-            datetimes, self._raw_data['Distortions']['SOFBLoop'], '-',
-            color='orangered', label='Distortions - SOFB Loop Open')
+            datetimes, self._raw_data['Failures']['ManualAnnotated'], '-',
+            color='red', label='Failures - Manual Annotated')
         axs[10].legend(loc='upper left', fontsize=9)
         axs[10].grid()
 
         axs[11].xaxis.axis_date()
         axs[11].plot(
-            datetimes, self._raw_data['Distortions']['FOFBLoop'], '-',
-            color='orangered', label='Distortions - FOFB Loop Open')
+            datetimes, self._raw_data['Distortions']['SOFBLoop'], '-',
+            color='orangered', label='Distortions - SOFB Loop Open')
         axs[11].legend(loc='upper left', fontsize=9)
         axs[11].grid()
 
         axs[12].xaxis.axis_date()
         axs[12].plot(
+            datetimes, self._raw_data['Distortions']['FOFBLoop'], '-',
+            color='orangered', label='Distortions - FOFB Loop Open')
+        axs[12].legend(loc='upper left', fontsize=9)
+        axs[12].grid()
+
+        axs[13].xaxis.axis_date()
+        axs[13].plot(
             datetimes[0], 0, '.', color='white',
             label='Distortions - BbB Instabilities:')
-        axs[12].plot(
+        axs[13].plot(
             datetimes, self._raw_data['Distortions']['BbBHStab'], '-',
             color='blue', label='H')
-        axs[12].plot(
+        axs[13].plot(
             datetimes, self._raw_data['Distortions']['BbBVStab'], '-',
             color='red', label='V')
-        axs[12].plot(
+        axs[13].plot(
             datetimes, self._raw_data['Distortions']['BbBLStab'], '-',
             color='green', label='L')
-        axs[12].legend(loc='upper left', fontsize=9, ncol=4)
-        axs[12].grid()
+        axs[13].legend(loc='upper left', fontsize=9, ncol=4)
+        axs[13].grid()
 
-        axs[13].xaxis.axis_date()
-        axs[13].plot(
+        axs[14].xaxis.axis_date()
+        axs[14].plot(
             datetimes, self._raw_data['Shift']['Injection'], '-',
             color='lightsalmon', label='Injection Shifts')
-        axs[13].legend(loc='upper left', fontsize=9)
-        axs[13].grid()
+        axs[14].legend(loc='upper left', fontsize=9)
+        axs[14].grid()
 
         shift2color = {
             'MachineStudy': ['MacStudy', 'skyblue'],
             'Commissioning': ['Commi', 'royalblue'],
             'Conditioning': ['Condit', 'orchid'],
             'Maintenance': ['Maint', 'green']}
         for shift, auxdata in shift2color.items():
             ydata = self._raw_data['Shift'][shift]
 
-            axs[14].xaxis.axis_date()
-            axs[14].plot(
+            axs[15].xaxis.axis_date()
+            axs[15].plot(
                 datetimes, ydata, '-',
                 color=auxdata[1], label=auxdata[0])
-        axs[14].legend(loc='upper left', ncol=4, fontsize=9)
-        axs[14].set_ylim(0.0, 2.0)
-        axs[14].grid()
+        axs[15].legend(loc='upper left', ncol=4, fontsize=9)
+        axs[15].set_ylim(0.0, 2.0)
+        axs[15].grid()
 
         egmodes2color = {
             'MultiBunch': 'orangered', 'SingleBunch': 'orange'}
         for egmode, color in egmodes2color.items():
             ydata = self._raw_data['EgunModes'][egmode]
 
-            axs[15].xaxis.axis_date()
-            axs[15].plot(
+            axs[16].xaxis.axis_date()
+            axs[16].plot(
                 datetimes, ydata, '-',
                 color=color, label=egmode)
-        axs[15].legend(loc='upper left', ncol=2, fontsize=9)
-        axs[15].set_ylim(0.0, 2.0)
-        axs[15].grid()
+        axs[16].legend(loc='upper left', ncol=2, fontsize=9)
+        axs[16].set_ylim(0.0, 2.0)
+        axs[16].grid()
 
         return fig
 
     def plot_progmd_vs_delivd_hours(self):
         """Plot programmed vs. delivered hours graph."""
         if not self._raw_data:
             print('No data to display. Call update() to get data.')
@@ -1335,14 +1347,18 @@
         self._raw_data['EgunModes'] = dict()
         self._raw_data['EgunModes']['SingleBunch'] = self._singlebunch_values
         self._raw_data['EgunModes']['MultiBunch'] = self._multibunch_values
 
         # get pvs data and calculate failures
         self._raw_data['Failures'] = dict()
 
+        # - manual annotated failures
+        self._raw_data['Failures']['ManualAnnotated'] = \
+            self._get_man_annotated_fails_data()
+
         # - subsystems status
         self._ps_fail_values, self._mps_fail_values = \
             self._get_subsystems_status_data()
         self._raw_data['Failures']['SubsystemsNOk'] = _np.logical_or(
             self._ps_fail_values, self._mps_fail_values)
 
         # - gamma
@@ -1555,16 +1571,16 @@
 
         if beg_idcs.size:
             beg_val = [i for i in range(beg_idcs.size-1) if
                        beg_idcs[i+1]-beg_idcs[i] > 15]
             beg_val += [beg_idcs.size-1]
             beg1, beg2 = beg_idcs[beg_val], beg_idcs[beg_val] + 15
             if beg2[-1] > self._users_shift_delivd_values.size-1:
-                beg1.pop()
-                beg2.pop()
+                beg1 = _np.delete(beg1, -1)
+                beg2 = _np.delete(beg2, -1)
             beg_val = [i for i in range(beg1.size) if not
                        any([beg1[i] < e < beg2[i] for e in end_idcs])]
             beg1, beg2 = beg1[beg_val], beg2[beg_val]
             stats_vals = [_np.mean(self._curr_values[beg1[i]:beg2[i]])
                           for i in range(beg1.size)]
             self._usershift_current_beg_average = _np.mean(stats_vals)
             self._usershift_current_beg_stddev = _np.std(stats_vals)
@@ -1573,30 +1589,31 @@
             self._usershift_current_beg_stddev = 0
 
         if end_idcs.size:
             end_val = [0] + [i for i in range(end_idcs.size)
                              if end_idcs[i]-end_idcs[i-1] > 15]
             end1, end2 = end_idcs[end_val] - 15, end_idcs[end_val]
             if end1[0] < 0:
-                end1.pop(0)
-                end2.pop(0)
+                end1 = _np.delete(end1, 0)
+                end2 = _np.delete(end2, 0)
             end_val = [i for i in range(end1.size-1) if not
                        any([end1[i] < b < end2[i] for b in beg_idcs])]
             end1, end2 = end1[end_val], end2[end_val]
             stats_vals = [_np.mean(self._curr_values[end1[i]:end2[i]])
                           for i in range(end1.size)]
             self._usershift_current_end_average = _np.mean(stats_vals)
             self._usershift_current_end_stddev = _np.std(stats_vals)
         else:
             self._usershift_current_end_average = 0
             self._usershift_current_end_stddev = 0
 
         # # # ----- failures -----
         beam_dump_values = _np.logical_not(
             self._raw_data['Failures']['WrongShift']) * \
+            self._raw_data['Failures']['ManualAnnotated'] * \
             self._raw_data['Failures']['NoEBeam']
         self._usershift_beam_dump_count = _np.sum(
             _np.diff(beam_dump_values) > 0)
 
         ave, std, count = self._calc_interval_stats(
             self._failures_users, dtimes_failures_users)
         self._usershift_time_to_recover_average = ave
@@ -1750,14 +1767,28 @@
             if times[0] > t_start + MacReport.QUERY_AVG_TIME:
                 times = _np.r_[t_start, times]
                 values = _np.r_[defv, values]
             idcsdefv = _np.where(times <= tstr.timestamp())[0]
             values[idcsdefv] = defv
         return times, values
 
+    def _get_man_annotated_fails_data(self):
+        # get all annotated failures
+        t2vs = _np.array([[], []])
+        for ini, end in MacReport.FAILURES_MANUAL:
+            t2vs = _np.c_[t2vs, [ini.timestamp(), 1], [end.timestamp(), 0]]
+        # insert initial point indicating not failure
+        t2vs = _np.c_[t2vs, [t2vs[0, 0]-1, 0]]
+        # sort by dates
+        t2vs = t2vs[:, t2vs[0, :].argsort()]
+        # calculate failures data in current timestamp base
+        failures = _interp1d_previous(
+            t2vs[0, :], t2vs[1, :], self._curr_times)
+        return failures
+
     def _calc_current_stats(self, dtimes):
         interval = _np.sum(dtimes)
         if not interval:
             average = 0.0
             stddev = 0.0
         else:
             average = _np.sum(self._curr_values*dtimes)/interval
```

### Comparing `siriuspy-2.76.1/siriuspy/machshift/macschedule.py` & `siriuspy-2.77.0/siriuspy/machshift/macschedule.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,20 +46,28 @@
         """Get users shift count for a period."""
         begin, end = MacScheduleData._handle_interval_data(begin, end)
         _, tags = MacScheduleData._get_numeric_data_for_interval(
             begin, end, dtype='macsched_byshift')
         return _np.sum(tags) if begin != end else 0
 
     @staticmethod
-    def get_users_shift_day_count(begin, end):
+    def get_users_shift_day_count(begin, end, count_sundays=True):
         """Get users shift day count for a period."""
         begin, end = MacScheduleData._handle_interval_data(begin, end)
-        _, tags = MacScheduleData._get_numeric_data_for_interval(
+        tims, tags = MacScheduleData._get_numeric_data_for_interval(
             begin, end, dtype='macsched_byday')
-        return _np.sum(tags) if begin != end else 0
+
+        count = 0
+        if begin != end:
+            for tim, tag in zip(tims, tags):
+                weekday = _Time(tim).weekday()
+                if (weekday == 6 and count_sundays) or weekday != 6:
+                    count += tag
+        return count
+
 
     @staticmethod
     def is_user_shift_programmed(
             timestamp=None, datetime=None,
             year=None, month=None, day=None, hour=0, minute=0):
         """Return whether a day is a predefined user shift."""
         timestamp, datetime, ret_uni = MacScheduleData._handle_timestamp_data(
@@ -113,26 +121,27 @@
             print('No data provided for year ' + str(year) + '. '
                   'Getting template data.')
             data, _ = _util.read_text_data(_web.mac_schedule_read('template'))
 
         databyshift = list()
         databyday = list()
         datainicurr = list()
+        flag_bit, inicurr = 0, 0.0
         for datum in data:
             if len(datum) < 2:
                 raise Exception(
                     'there is a date ({0}) with problem in {1} '
                     'machine schedule'.format(datum, year))
 
             month, day = int(datum[0]), int(datum[1])
             if len(datum) == 2:
                 timestamp = _Time(year, month, day, 0, 0).timestamp()
-                databyshift.append((timestamp, 0))
-                databyday.append((timestamp, 0))
-                datainicurr.append((timestamp, 0.0))
+                databyshift.append((timestamp, flag_bit))
+                databyday.append((timestamp, flag_bit))
+                datainicurr.append((timestamp, inicurr))
             else:
                 timestamp = _Time(year, month, day, 0, 0).timestamp()
                 databyday.append((timestamp, 1))
                 for tag in datum[2:]:
                     if 'B' in tag:
                         hour, minute, flag, inicurr = _re.findall(
                             MacScheduleData._TAG_FORMAT_BEG, tag)[0]
```

### Comparing `siriuspy-2.76.1/siriuspy/machshift/main.py` & `siriuspy-2.77.0/siriuspy/machshift/main.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/siriuspy/machshift/utils.py` & `siriuspy-2.77.0/siriuspy/machshift/utils.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/siriuspy/magnet/data.py` & `siriuspy-2.77.0/siriuspy/magnet/data.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/siriuspy/magnet/excdata.py` & `siriuspy-2.77.0/siriuspy/magnet/excdata.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/siriuspy/magnet/factory.py` & `siriuspy-2.77.0/siriuspy/magnet/factory.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/siriuspy/magnet/normalizer.py` & `siriuspy-2.77.0/siriuspy/magnet/normalizer.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/siriuspy/magnet/util.py` & `siriuspy-2.77.0/siriuspy/magnet/util.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/siriuspy/meas/csdev.py` & `siriuspy-2.77.0/siriuspy/meas/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/siriuspy/meas/liemit/csdev.py` & `siriuspy-2.77.0/siriuspy/meas/liemit/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/siriuspy/meas/liemit/main.py` & `siriuspy-2.77.0/siriuspy/meas/liemit/main.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/siriuspy/meas/lienergy/csdev.py` & `siriuspy-2.77.0/siriuspy/meas/lienergy/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/siriuspy/meas/lienergy/main.py` & `siriuspy-2.77.0/siriuspy/meas/lienergy/main.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/siriuspy/meas/util.py` & `siriuspy-2.77.0/siriuspy/meas/util.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/siriuspy/namesys/implementation.py` & `siriuspy-2.77.0/siriuspy/namesys/implementation.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/siriuspy/optics/lattice_survey.py` & `siriuspy-2.77.0/siriuspy/optics/lattice_survey.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/siriuspy/opticscorr/base.py` & `siriuspy-2.77.0/siriuspy/opticscorr/base.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/siriuspy/opticscorr/chrom.py` & `siriuspy-2.77.0/siriuspy/opticscorr/chrom.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/siriuspy/opticscorr/csdev.py` & `siriuspy-2.77.0/siriuspy/opticscorr/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/siriuspy/opticscorr/opticscorr.py` & `siriuspy-2.77.0/siriuspy/opticscorr/opticscorr.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/siriuspy/opticscorr/tune.py` & `siriuspy-2.77.0/siriuspy/opticscorr/tune.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/siriuspy/opticscorr/utils.py` & `siriuspy-2.77.0/siriuspy/opticscorr/utils.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/siriuspy/oscilloscope/keysight.py` & `siriuspy-2.77.0/siriuspy/oscilloscope/keysight.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/siriuspy/oscilloscope/scopes.py` & `siriuspy-2.77.0/siriuspy/oscilloscope/scopes.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/siriuspy/posang/csdev.py` & `siriuspy-2.77.0/siriuspy/posang/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/siriuspy/posang/main.py` & `siriuspy-2.77.0/siriuspy/posang/main.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/siriuspy/posang/utils.py` & `siriuspy-2.77.0/siriuspy/posang/utils.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/siriuspy/pwrsupply/beaglebone.py` & `siriuspy-2.77.0/siriuspy/pwrsupply/beaglebone.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/siriuspy/pwrsupply/bsmp/commands.py` & `siriuspy-2.77.0/siriuspy/pwrsupply/bsmp/commands.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/siriuspy/pwrsupply/bsmp/constants.py` & `siriuspy-2.77.0/siriuspy/pwrsupply/bsmp/constants.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/siriuspy/pwrsupply/bsmp/entities.py` & `siriuspy-2.77.0/siriuspy/pwrsupply/bsmp/entities.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/siriuspy/pwrsupply/bsmp/factory.py` & `siriuspy-2.77.0/siriuspy/pwrsupply/bsmp/factory.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/siriuspy/pwrsupply/csdev.py` & `siriuspy-2.77.0/siriuspy/pwrsupply/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/siriuspy/pwrsupply/data.py` & `siriuspy-2.77.0/siriuspy/pwrsupply/data.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/siriuspy/pwrsupply/factory.py` & `siriuspy-2.77.0/siriuspy/pwrsupply/factory.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Power Supply factory classes."""
 
 import time as _time
 import re as _re
 from copy import deepcopy as _deepcopy
 
 from ..search import PSSearch as _PSSearch
-from ..thread import DequeThread as _DequeThread
+from ..thread import LoopQueueThread as _LoopQueueThread
 from ..bsmp.serial import Channel as _Channel
 
 from .csdev import get_ps_propty_database as _get_ps_propty_database
 from .beaglebone import BeagleBone as _BeagleBone
 from .siggen import SigGenFactory as _SigGenfactory
 
 from .bsmp.factory import PSBSMPFactory as _PSBSMPFactory
@@ -33,27 +33,27 @@
         """Return BBB object."""
         # create timestamp used in all TimestampBoot-Cte PVs
         timestamp = _time.time()
 
         # create PRU used for low-level communication
         pru = _PRU(ethbridgeclnt_class, bbbname=bbbname)
 
-        # create DequeThread that queue all serial operations
-        prucqueue = _DequeThread()
+        # create LoopQueueThread that queue all serial operations
+        prucqueue = _LoopQueueThread()
 
         # build dicts for grouped udc.
         psmodels, devices, freqs = \
             BBBFactory._build_udcgrouped(bbbname)
 
         if len(psmodels) > 1:
-            # more than one psmodel under the same beagle. there will be two 
-            # PRUController objects pushing operation requests into the common 
-            # DequeThread. we have to use to lock mechanism in bsmp.Channel in 
-            # order to avoid one PRUController process thread interpreting the
-            # operation request of the other PRUController scan thread.
+            # more than one psmodel under the same beagle. there will be two
+            # PRUController objects pushing operation requests into the common
+            # LoopQueueThread. we have to use to lock mechanism in bsmp.Channel
+            # in order to avoid one PRUController process thread interpreting
+            # the operation request of the other PRUController scan thread.
             _Channel.create_lock()
 
         # power supply controllers and databases
         # dbase: a pvname-epicsdbase dictionary containing all
         # beaglebone PVs. the epics server database is initialized
         # using this dictionary.
         controllers, databases, dbase = \
@@ -128,15 +128,15 @@
         return controllers, databases, dbase
 
     @staticmethod
     def _build_udcgrouped(bbbname):
 
         # get names of all udcs under a beaglebone
         udcs = _PSSearch.conv_bbbname_2_udc(bbbname)
-        
+
         psmodels, devices, freqs = dict(), dict(), dict()
         for udc in udcs:
 
             # add udc devices
             devs = _PSSearch.conv_udc_2_bsmps(udc)
             print('UDC: ', udc, ', DEVICES: ', devs)
             psmodel_name = BBBFactory._check_psmodels(devs)
```

### Comparing `siriuspy-2.76.1/siriuspy/pwrsupply/pructrl/__init__.py` & `siriuspy-2.77.0/siriuspy/pwrsupply/pructrl/__init__.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/siriuspy/pwrsupply/pructrl/pru.py` & `siriuspy-2.77.0/siriuspy/pwrsupply/pructrl/pru.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/siriuspy/pwrsupply/pructrl/prucontroller.py` & `siriuspy-2.77.0/siriuspy/pwrsupply/pructrl/prucontroller.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,16 +28,14 @@
     of the Beaglebone computer connected through a serial line to power supply
     controllers.
     """
 
     # NOTE: All private methods starting with '_bsmp' string invoke serial
     #       bsmp communications.
 
-    _sleep_process_loop = 0.020  # [s]
-
     # --- public interface ---
 
     def __init__(self,
                  pru,
                  prucqueue,
                  psmodel,
                  devices,
@@ -97,15 +95,14 @@
         # attributes that control processing flow
         self._queue = prucqueue
         self._processing = processing
         self._scanning = scanning
 
         # starts communications
         self._dev_idx_last_scanned = None
-        self._thread_process = None
         self._thread_scan = None
         if init:
             self.bsmp_init_communication()
 
     # --- properties to read and set controller state and access functions ---
 
     @property
@@ -122,25 +119,29 @@
     def scanning(self, value):
         """Set scanning state."""
         self._scanning = value
 
     @property
     def processing(self):
         """Return processing state."""
-        return self._processing
+        return self._queue.is_running
 
     @processing.setter
     def processing(self, value):
         """Set processing state."""
         self._processing = value
+        if self._processing:
+            self._queue.start()
+        else:
+            self._queue.stop()
 
     @property
     def queue_length(self):
         """Store number of operations currently in the queue."""
-        return len(self._queue)
+        return self._queue.qsize()
 
     @property
     def params(self):
         """Return PRUController parameters."""
         return self._parms
 
     @property
@@ -153,18 +154,14 @@
         # TODO: may not be the true current connection state
         psupply = self._psupplies[device_id]
         return psupply.connected
 
     def timestamp_update(self):
         """Return tmestamp of last device update."""
         return self._timestamp_update
-        # psupply = self._psupplies[device_id]
-        # with self._lock:
-        #     tstamp = psupply.timestamp_update
-        # return tstamp
 
     # === queueing writes and local state copy reads ===
 
     # --- bsmp variables and parameters ---
 
     def read_variables(self, device_ids, variable_id=None):
         """
@@ -224,16 +221,15 @@
         # make copy
         with self._lock:
             if isinstance(device_ids, int):
                 return _dcopy(values[device_ids])
             return _dcopy(values)
 
     def exec_functions(self, device_ids, function_id, args=None):
-        """
-        Append BSMP function executions to opertations queue.
+        """Append BSMP function executions to opertations queue.
 
         Parameters
         ----------
         device_ids : int, tuple or list
             The BSMP device ids. It can be a list of ids or a singe id.
         function_id : int
             The BSMP function id to be executed for the devices.
@@ -241,15 +237,14 @@
             The list of BSMP function argument values
 
         Returns
         -------
         status : bool
             True is operation was queued or False, if operation was rejected
             because of the SOFBMode state.
-
         """
         # if in SOFBMode on, do not accept exec functions
         if self._sofb_mode:
             return False
 
         # prepare arguments
         if isinstance(device_ids, int):
@@ -257,30 +252,30 @@
         if args is None:
             args = (device_ids, function_id)
         else:
             args = (device_ids, function_id, args)
 
         # append bsmp function exec operation to queue
         operation = (self._bsmp_exec_function, args)
-        self._queue.append(operation)
+        self._queue.put(operation, block=False)
         return True
 
     def update_parameters(self, device_ids):
         """Update device parameters."""
         # if in SOFBMode on, do not accept comm. commands
         if self._sofb_mode:
             return False
 
         if isinstance(device_ids, int):
             device_ids = (device_ids, )
 
         # append function operation to queue
         args = (device_ids, )
         operation = (self._bsmp_read_parameter_values, args)
-        self._queue.append(operation)
+        self._queue.put(operation, block=False)
         return True
 
     # --- wfmref and scope curves ---
 
     def scope_update_auto_enable(self):
         """Enable wfmref and scope curves updates."""
         self._scope_update = True
@@ -295,30 +290,30 @@
         return self._scope_update
 
     def wfm_update(self, device_ids, interval=None):
         """Queue update wfm and scope curves."""
         if isinstance(device_ids, int):
             device_ids = (device_ids, )
         operation = (self._bsmp_update_wfm, (device_ids, interval, ))
-        self._queue.append(operation)
+        self._queue.put(operation, block=False)
         return True
 
     def wfmref_write(self, device_ids, data):
         """Write wfm curves."""
         # if in SOFBMode on, do not accept exec functions
         if self._sofb_mode:
             return False
 
         # prepare arguments
         if isinstance(device_ids, int):
             device_ids = (device_ids, )
 
         # append bsmp function exec operation to queue
         operation = (self._bsmp_wfmref_write, (device_ids, data))
-        self._queue.append(operation)
+        self._queue.put(operation, block=False)
         return True
 
     def wfmref_rb_read(self, device_id):
         """Return wfmref_rb curve."""
         psupply = self._psupplies[device_id]
         # NOTE: investigate whether lock and copy are really necessary!
         with self._lock:
@@ -346,26 +341,25 @@
 
     # --- SOFBCurrent parameters ---
 
     def sofb_mode_set(self, state):
         """Change SOFB mode: True or False."""
         self._sofb_mode = state
         if state:
-            while self._queue:  # wait until queue is empty
+            while not self._queue.empty():  # wait until queue is empty
                 pass
 
     @property
     def sofb_mode(self):
         """Return SOFB mode."""
         return self._sofb_mode
 
     def sofb_current_set(self, value):
         """."""
-        # wait until queue is empty
-        while self._queue:
+        while not self._queue.empty():  # wait until queue is empty
             pass
 
         # execute SOFB setpoint
         self._bsmp_update_sofb_setpoint(value)
 
         return True
 
@@ -386,16 +380,15 @@
 
     def sofb_update_variables_state(self):
         """Update variables state mirror."""
         # do sofb update only if in SOFBMode On
         if not self._sofb_mode:
             return
 
-        # wait until queue is empty
-        while self._queue:
+        while not self._queue.empty():  # wait until queue is empty
             pass
 
         # select power supply dev_id for updating
         self._sofb_update_dev_idx = \
             (self._sofb_update_dev_idx + 1) % len(self._device_ids)
         dev_id = self._device_ids[self._sofb_update_dev_idx]
 
@@ -405,26 +398,21 @@
     # --- scan and process loop methods ---
 
     def bsmp_scan(self):
         """Run scan one."""
         # select devices and variable group, defining the read group
         # operation to be performed
         operation = (self._bsmp_update, ())
-        if not self._queue or operation != self._queue.last_operation:
-            self._queue.append(operation)
+        if self._queue.empty() or operation != self._queue.last_operation:
+            self._queue.put(operation, block=False)
         else:
             # do not append if last operation is the same as last one
             # operation appended to queue
             pass
 
-    def bsmp_process(self):
-        """Run process once."""
-        # process first operation in queue, if any.
-        self._queue.process()
-
     def bsmp_init_communication(self):
         """."""
         # --- BSMP communication ---
 
         print()
         print('PRUController: bsmp initialization')
         # init time interval
@@ -442,27 +430,25 @@
         # time interval
         t1_ = _time()
         print('TIMING bsmp init [{:.3f} ms]\n'.format(
             1000*(t1_ - t0_)))
 
         # after all initializations, threads are started
         self._running = True
-        self._thread_process.start()
+        if self._processing:
+            self._queue.start()
         self._thread_scan.start()
 
     # --- private methods: initializations ---
 
     def _init_threads(self):
 
         fmt = '  - {:<20s} ({:^20s}) [{:09.3f}] ms'
         t0_ = _time()
 
-        # define process thread
-        self._thread_process = _Thread(target=self._loop_process, daemon=True)
-
         # define scan thread
         self._dev_idx_last_scanned = \
             len(self._device_ids)-1  # the next will be the first bsmp dev
         self._thread_scan = _Thread(target=self._loop_scan, daemon=True)
 
         dt_ = _time() - t0_
         print(fmt.format('init_threads', 'create structures', 1e3*dt_))
@@ -500,16 +486,17 @@
             psupply = self._psupplies[dev_id]
             _firmware_version_udc = psupply.get_variable(
                 self._parms.CONST_PSBSMP.V_FIRMWARE_VERSION)
             _firmware_version_udc = \
                 self._udc.parse_firmware_version(_firmware_version_udc)
             if 'Simulation' not in _firmware_version_udc and \
                _firmware_version_udc != _firmware_version_siriuspy:
-                errmsg = ('PRUController: Incompatible bsmp implementation version '
-                          'for device id:{}')
+                errmsg = (
+                    'PRUController: Incompatible bsmp implementation version '
+                    'for device id:{}')
                 print(errmsg.format(dev_id))
                 errmsg = 'lib version: {}'
                 print(errmsg.format(_firmware_version_siriuspy))
                 errmsg = 'udc version: {}'
                 print(errmsg.format(_firmware_version_udc))
                 print()
                 # raise ValueError(errmsg)
@@ -534,24 +521,14 @@
             dt_ = _time() - t0_
             if dt_ < self._scan_interval:
                 _sleep(self._scan_interval - dt_)
 
             # update timestamp
             self._timestamp_update = _time()
 
-    def _loop_process(self):
-        while self._running:
-            if self.processing:
-                self.bsmp_process()
-            # if queue is empty, sleep a little
-            # _sleep(self._sleep_process_loop)
-            # NOTE: this optimization is being tested...
-            if not self._queue:
-                _sleep(self._sleep_process_loop)
-
     def _get_scan_interval(self):
         if self._parms.FREQ_SCAN == 0:
             return 0
         else:
             return 1.0/self._parms.FREQ_SCAN  # [s]
 
     def _serial_error(self, device_ids):
```

### Comparing `siriuspy-2.76.1/siriuspy/pwrsupply/pructrl/prucparms.py` & `siriuspy-2.77.0/siriuspy/pwrsupply/pructrl/prucparms.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/siriuspy/pwrsupply/pructrl/psdevstate.py` & `siriuspy-2.77.0/siriuspy/pwrsupply/pructrl/psdevstate.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/siriuspy/pwrsupply/pructrl/udc.py` & `siriuspy-2.77.0/siriuspy/pwrsupply/pructrl/udc.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/siriuspy/pwrsupply/psctrl/__init__.py` & `siriuspy-2.77.0/siriuspy/pwrsupply/psctrl/__init__.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/siriuspy/pwrsupply/psctrl/pscontroller.py` & `siriuspy-2.77.0/siriuspy/pwrsupply/psctrl/pscontroller.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/siriuspy/pwrsupply/psctrl/pscreaders.py` & `siriuspy-2.77.0/siriuspy/pwrsupply/psctrl/pscreaders.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/siriuspy/pwrsupply/psctrl/pscstatus.py` & `siriuspy-2.77.0/siriuspy/pwrsupply/psctrl/pscstatus.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/siriuspy/pwrsupply/psctrl/pscwriters.py` & `siriuspy-2.77.0/siriuspy/pwrsupply/psctrl/pscwriters.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/siriuspy/pwrsupply/psctrl/psmodel.py` & `siriuspy-2.77.0/siriuspy/pwrsupply/psctrl/psmodel.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/siriuspy/pwrsupply/pssofb.py` & `siriuspy-2.77.0/siriuspy/pwrsupply/pssofb.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/siriuspy/pwrsupply/siggen.py` & `siriuspy-2.77.0/siriuspy/pwrsupply/siggen.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/siriuspy/ramp/conn.py` & `siriuspy-2.77.0/siriuspy/ramp/conn.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/siriuspy/ramp/magnet.py` & `siriuspy-2.77.0/siriuspy/ramp/magnet.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/siriuspy/ramp/ramp.py` & `siriuspy-2.77.0/siriuspy/ramp/ramp.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/siriuspy/ramp/reconst_factory.py` & `siriuspy-2.77.0/siriuspy/ramp/reconst_factory.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/siriuspy/ramp/test_reconst_factory.py` & `siriuspy-2.77.0/siriuspy/ramp/test_reconst_factory.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/siriuspy/ramp/testwfm.py` & `siriuspy-2.77.0/siriuspy/ramp/testwfm.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/siriuspy/ramp/util.py` & `siriuspy-2.77.0/siriuspy/ramp/util.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/siriuspy/ramp/waveform.py` & `siriuspy-2.77.0/siriuspy/ramp/waveform.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/siriuspy/search/bpms_search.py` & `siriuspy-2.77.0/siriuspy/search/bpms_search.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/siriuspy/search/hl_time_search.py` & `siriuspy-2.77.0/siriuspy/search/hl_time_search.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/siriuspy/search/id_search.py` & `siriuspy-2.77.0/siriuspy/search/id_search.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/siriuspy/search/ioc_search.py` & `siriuspy-2.77.0/siriuspy/search/ioc_search.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/siriuspy/search/ll_time_search.py` & `siriuspy-2.77.0/siriuspy/search/ll_time_search.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/siriuspy/search/ma_search.py` & `siriuspy-2.77.0/siriuspy/search/ma_search.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/siriuspy/search/ps_search.py` & `siriuspy-2.77.0/siriuspy/search/ps_search.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/siriuspy/simul/simfactory.py` & `siriuspy-2.77.0/siriuspy/simul/simfactory.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/siriuspy/simul/simps.py` & `siriuspy-2.77.0/siriuspy/simul/simps.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/siriuspy/simul/simpv.py` & `siriuspy-2.77.0/siriuspy/simul/simpv.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/siriuspy/simul/simulation.py` & `siriuspy-2.77.0/siriuspy/simul/simulation.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/siriuspy/simul/simulator.py` & `siriuspy-2.77.0/siriuspy/simul/simulator.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/siriuspy/sofb/base_class.py` & `siriuspy-2.77.0/siriuspy/sofb/base_class.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Definition module."""
 import math as _math
 import logging as _log
 
 import numpy as _np
 
 from ..callbacks import Callback as _Callback
+from ..thread import LoopQueueThread as _LoopQueueThread
 
 from .csdev import SOFBFactory as _SOFBFactory, ConstTLines as _ConstTLines
 
 _CSACCELS = {}
 
 
 def _create_csorb(acc):
@@ -18,17 +19,22 @@
         _CSACCELS[acc] = csorb
     return csorb
 
 
 class BaseClass(_Callback):
     """Base Class."""
 
+    _LQTHREAD = None
+
     def __init__(self, acc, prefix='', callback=None):
         """Init method."""
         super().__init__(callback)
+        if BaseClass._LQTHREAD is None:
+            BaseClass._LQTHREAD = _LoopQueueThread(is_cathread=True)
+            self._LQTHREAD.start()
         self._csorb = _create_csorb(acc)
         self._prefix = prefix
         self._status = 0b0
         self._map2write = self.get_map2write()
 
     @property
     def prefix(self):
```

### Comparing `siriuspy-2.76.1/siriuspy/sofb/bpms.py` & `siriuspy-2.77.0/siriuspy/sofb/bpms.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/siriuspy/sofb/correctors.py` & `siriuspy-2.77.0/siriuspy/sofb/correctors.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import logging as _log
 import traceback as _traceback
 
 import numpy as _np
 from PRUserial485 import EthBridgeClient
 
 from .. import util as _util
-from ..epics import PV as _PV, CAThread as _Thread
+from ..epics import PV as _PV
 from ..thread import RepeaterThread as _Repeat
 from ..pwrsupply.csdev import Const as _PSConst
 from ..pwrsupply.bsmp.constants import ConstPSBSMP as _ConstPSBSMP
 from ..timesys.csdev import Const as _TIConst
 from ..search import HLTimeSearch as _HLTimesearch
 from ..envars import VACA_PREFIX as LL_PREF
 from ..namesys import SiriusPVName as _PVName
@@ -674,18 +674,16 @@
         except Exception as err:
             self._update_log('ERR: ' + str(err))
             _log.error(_traceback.format_exc())
 
     def set_corrs_mode(self, value, is_thread=False):
         """Set mode of CHs and CVs method. Only called when acc==SI."""
         if not is_thread:
-            _Thread(
-                target=self.set_corrs_mode,
-                args=(value, ), kwargs={'is_thread': True},
-                daemon=True).start()
+            self._LQTHREAD.put((
+                self.set_corrs_mode, (value, ), {'is_thread': True}))
             return True
 
         if value not in self._csorb.CorrSync:
             return False
         self.sync_kicks = value
         val = _PSConst.OpMode.SlowRefSync
         if value == self._csorb.CorrSync.Off:
@@ -761,18 +759,16 @@
 
         self.run_callbacks('CorrPSSOFBEnbl-Mon', val)
         return True
 
     def configure_correctors(self, val, is_thread=False):
         """Configure correctors method."""
         if not is_thread:
-            _Thread(
-                target=self.configure_correctors,
-                args=(val, ), kwargs={'is_thread': True},
-                daemon=True).start()
+            self._LQTHREAD.put((
+                self.configure_correctors, (val, ), {'is_thread': True}))
             return True
 
         corrs = self._get_used_corrs(include_rf=True)
         for corr in corrs:
             if not corr.connected:
                 msg = 'ERR: Failed to configure '
                 msg += corr.name
```

### Comparing `siriuspy-2.76.1/siriuspy/sofb/csdev.py` & `siriuspy-2.77.0/siriuspy/sofb/csdev.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 
     STS_LBLS_CORR_TLINES = (
         'CHCVConnected', 'CHCVModeConfigured', 'CHCVPwrStateOn')
     STS_LBLS_CORR_RINGS = STS_LBLS_CORR_TLINES + (
         'TimingConnected', 'TimingConfigured', 'RFConnected', 'RFPwrStateOn')
     STS_LBLS_ORB = (
         'TimingConnected', 'TimingConfigured', 'BPMsConnected',
-        'BPMsEnabled', 'BPMsConfigured')
+        'BPMsEnabled', 'BPMsConfigured', 'OrbRawConnected')
     STS_LBLS_GLOB = ('Ok', 'NotOk')
 
 
 _et = ETypes  # syntactic sugar
 
 
 # --- Const class ---
@@ -58,15 +58,15 @@
     MAX_MT_ORBS = 4000
     MAX_DRIVE_DATA = 3 * 5000
     MIN_SING_VAL = 0.2
     TIKHONOV_REG_CONST = 0
     TINY_KICK = 1e-3  # [urad]
     DEF_MAX_ORB_DISTORTION = 50  # [um]
     ACQRATE_TRIGMODE = 2  # [Hz]
-    ACQRATE_SLOWORB = 12  # [Hz]
+    ACQRATE_SLOWORB = 60  # [Hz]
     BPMsFreq = 10.48  # [Hz]
 
     TrigAcqCtrl = _csbpm.AcqEvents
     TrigAcqChan = _csdev.Const.register('TrigAcqChan', _et.ORB_ACQ_CHAN)
     TrigAcqRepeat = _csbpm.AcqRepeat
     SmoothMeth = _csdev.Const.register('SmoothMeth', _et.SMOOTH_METH)
     RespMatMode = _csdev.Const.register('RespMatMode', _et.RESPMAT_MODE)
@@ -763,18 +763,18 @@
             'LoopEffectiveRate-Mon': {
                 'type': 'float', 'value': 0, 'unit': 'Hz', 'prec': 3,
                 'lolim': 0, 'hilim': 100},
             'LoopNumIters-Mon': {
                 'type': 'float', 'value': 0, 'unit': '#', 'prec': 0,
                 'lolim': 0, 'hilim': 100000},
             'LoopPrintEveryNumIters-SP': {
-                'type': 'float', 'value': 1000, 'unit': '#', 'prec': 0,
+                'type': 'float', 'value': 200, 'unit': '#', 'prec': 0,
                 'lolim': 1, 'hilim': 100000},
             'LoopPrintEveryNumIters-RB': {
-                'type': 'float', 'value': 1000, 'unit': '#', 'prec': 0,
+                'type': 'float', 'value': 200, 'unit': '#', 'prec': 0,
                 'lolim': 1, 'hilim': 100000},
             'LoopPerfItersTOut-Mon': {
                 'type': 'float', 'value': 0, 'unit': '%', 'prec': 3,
                 'lolim': -1, 'hilim': 100},
             'LoopPerfItersDiff-Mon': {
                 'type': 'float', 'value': 0, 'unit': '%', 'prec': 3,
                 'lolim': -1, 'hilim': 100},
```

### Comparing `siriuspy-2.76.1/siriuspy/sofb/main.py` & `siriuspy-2.77.0/siriuspy/sofb/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,19 +23,20 @@
 
     def __init__(
             self, acc, prefix='', callback=None, orbit=None, matrix=None,
             correctors=None, tests=False):
         """Initialize Object."""
         super().__init__(acc, prefix=prefix, callback=callback)
         _log.info('Starting SOFB...')
+
         self._tests = tests
         self._orbit = self._correctors = self._matrix = None
         self._loop_state = self._csorb.LoopState.Open
         self._loop_freq = self._csorb.BPMsFreq
-        self._loop_print_every_num_iter = 1000
+        self._loop_print_every_num_iter = 200
         self._loop_use_pssofb = False
         self._loop_max_orb_distortion = self._csorb.DEF_MAX_ORB_DISTORTION
         zer = _np.zeros(self._csorb.nr_corrs, dtype=float)
         self._pid_errs = [zer, zer.copy(), zer.copy()]
         self._pid_gains = dict(
             ch=dict(kp=0.0, ki=0.2, kd=0.0),
             cv=dict(kp=0.0, ki=0.2, kd=0.0),
@@ -319,40 +320,38 @@
             _log.error(msg[5:])
             return False
         if self._dtheta is None:
             msg = 'ERR: Cannot Apply Kick. Calc Corr first.'
             self._update_log(msg)
             _log.error(msg[5:])
             return False
-        _Thread(
-            target=self._apply_corr, kwargs={'code': code},
-            daemon=True).start()
+        self._LQTHREAD.put((self._apply_corr, tuple(), {'code': code}))
         return True
 
     def calc_correction(self, _):
         """Calculate correction."""
         self.run_callbacks('ApplyDelta-Mon', self._csorb.ApplyDeltaMon.Idle)
         if self._thread and self._thread.is_alive():
             msg = 'ERR: Loop is Closed or MeasRespMat is On.'
             self._update_log(msg)
             _log.error(msg[5:])
             return False
-        _Thread(target=self._calc_correction, daemon=True).start()
+        self._LQTHREAD.put((self._calc_correction, ))
         return True
 
     def set_delta_kick(self, code, dkicks):
         """Calculate correction."""
         if self._thread and self._thread.is_alive():
             msg = 'ERR: Loop is Closed or MeasRespMat is On.'
             self._update_log(msg)
             _log.error(msg[5:])
             return False
-        _Thread(
-            target=self._set_delta_kick,
-            kwargs={'code': code, 'dkicks': dkicks}, daemon=True).start()
+        self._LQTHREAD.put((
+            self._set_delta_kick, tuple(),
+            {'code': code, 'dkicks': dkicks}))
         return True
 
     def set_respmat_meas_state(self, value):
         """."""
         if value == self._csorb.MeasRespMatCmd.Start:
             self._start_meas_respmat()
         elif value == self._csorb.MeasRespMatCmd.Stop:
@@ -473,16 +472,15 @@
                 self._update_log(msg)
                 _log.error(msg[5:])
                 return False
             msg = 'Closing the Drive Loop.'
             self._update_log(msg)
             _log.info(msg)
             self._drive_state = value
-            self._thread = _Thread(
-                target=self._do_drive, daemon=True)
+            self._thread = _Thread(target=self._do_drive, daemon=True)
             self._thread.start()
         elif value == self._csorb.LoopState.Open:
             msg = 'Opening the Drive Loop.'
             self._update_log(msg)
             _log.info(msg)
             self._drive_state = value
         return True
@@ -868,17 +866,16 @@
                 msg = 'ERR: At least one AMC is not locked!'
                 self._update_log(msg)
                 _log.error(msg[5:])
                 break
             itern = len(times)
             self.run_callbacks('LoopNumIters-Mon', itern)
             if itern >= self._loop_print_every_num_iter:
-                _Thread(
-                    target=self._print_auto_corr_info,
-                    args=(times, rets, _time()-tim0), daemon=True).start()
+                self._LQTHREAD.put((
+                    self._print_auto_corr_info, (times, rets, _time()-tim0)))
                 times, rets = [], []
                 tim0 = _time()
 
             interval = 1/self._loop_freq
             use_pssofb = self.correctors.use_pssofb
             norbs = 1
             if use_pssofb:
```

### Comparing `siriuspy-2.76.1/siriuspy/sofb/matrix.py` & `siriuspy-2.77.0/siriuspy/sofb/matrix.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 import os as _os
 import logging as _log
 from functools import partial as _part
 
 import numpy as _np
 
-from ..epics import PV as _PV, CAThread as _Thread
 from .base_class import BaseClass as _BaseClass
 
 
 class BaseMatrix(_BaseClass):
     """."""
 
 
@@ -84,18 +83,16 @@
         if self.isring:
             dbase['RFEnbl-Sel'] = _part(self.set_enbllist, 'rf')
         return dbase
 
     def set_respmat_mode(self, mode, is_thread=False):
         """Set the response matrix mode."""
         if not is_thread:
-            _Thread(
-                target=self.set_respmat_mode,
-                args=(mode, ), kwargs={'is_thread': True},
-                daemon=True).start()
+            self._LQTHREAD.put((
+                self.set_respmat_mode, (mode, ), {'is_thread': True}))
             return True
 
         msg = 'Setting New RespMatMode.'
         self._update_log(msg)
         _log.info(msg)
         if mode not in self._csorb.RespMatMode:
             self.run_callbacks('RespMatMode-Sel', self._respmat_mode)
@@ -107,18 +104,16 @@
             self.run_callbacks('RespMatMode-Sel', self._respmat_mode)
             return
         self.run_callbacks('RespMatMode-Sts', self._respmat_mode)
 
     def set_respmat(self, mat, is_thread=False):
         """Set the response matrix in memory and save it in file."""
         if not is_thread:
-            _Thread(
-                target=self.set_respmat,
-                args=(mat, ), kwargs={'is_thread': True},
-                daemon=True).start()
+            self._LQTHREAD.put((
+                self.set_respmat, (mat, ), {'is_thread': True}))
             return True
 
         msg = 'Setting New RespMat.'
         self._update_log(msg)
         _log.info(msg)
         if mat is None:
             self.run_callbacks('RespMat-SP', list(self.respmat.ravel()))
@@ -132,18 +127,16 @@
             return
         self._save_respmat(mat)
         self.run_callbacks('RespMat-RB', list(self.respmat.ravel()))
 
     def set_enbllist(self, key, val, is_thread=False):
         """."""
         if not is_thread:
-            _Thread(
-                target=self.set_enbllist,
-                args=(key, val), kwargs={'is_thread': True},
-                daemon=True).start()
+            self._LQTHREAD.put((
+                self.set_enbllist, (key, val), {'is_thread': True}))
             return True
 
         msg = 'Setting {0:s} EnblList'.format(key.upper())
         self._update_log(msg)
         _log.info(msg)
 
         bkup = self.select_items[key]
@@ -172,16 +165,15 @@
         if orbit.size != self.inv_respmat.shape[1]:
             msg = 'ERR: Orbit and matrix size not compatible.'
             self._update_log(msg)
             _log.error(msg[5:])
             return None
         kicks = _np.dot(self.inv_respmat, orbit)
         kicks *= -1
-        _Thread(
-            target=self._update_dkicks, args=(kicks, ), daemon=True).start()
+        self._LQTHREAD.put((self._update_dkicks, (kicks, )))
         return kicks
 
     def estimate_orbit_variation(self, kicks):
         """Estimate the orbit variation induced by kicks.
 
         Args:
             kicks (numpy.ndarray): Correctors kicks that will be used to
@@ -206,35 +198,31 @@
         self.run_callbacks('DeltaKickCV-Mon', kicks[nr_ch:nr_chcv])
         if self.isring:
             self.run_callbacks('DeltaKickRF-Mon', kicks[-1])
 
     def set_min_sing_value(self, num, is_thread=False):
         """."""
         if not is_thread:
-            _Thread(
-                target=self.set_min_sing_value,
-                args=(num, ), kwargs={'is_thread': True},
-                daemon=True).start()
+            self._LQTHREAD.put((
+                self.set_min_sing_value, (num, ), {'is_thread': True}))
             return True
 
         bkup = self.min_sing_val
         self.min_sing_val = float(num)
         if not self._calc_matrices():
             self.min_sing_val = bkup
             self.run_callbacks('MinSingValue-SP', self.min_sing_val)
             return
         self.run_callbacks('MinSingValue-RB', self.min_sing_val)
 
     def set_tikhonov_reg_const(self, num, is_thread=False):
         """."""
         if not is_thread:
-            _Thread(
-                target=self.set_tikhonov_reg_const,
-                args=(num, ), kwargs={'is_thread': True},
-                daemon=True).start()
+            self._LQTHREAD.put((
+                self.set_tikhonov_reg_const, (num, ), {'is_thread': True}))
             return True
 
         bkup = self.tikhonov_reg_const
         self.tikhonov_reg_const = float(num)
         if not self._calc_matrices():
             self.tikhonov_reg_const = bkup
             self.run_callbacks('TikhonovRegConst-SP', self.tikhonov_reg_const)
```

### Comparing `siriuspy-2.76.1/siriuspy/sofb/orbit.py` & `siriuspy-2.77.0/siriuspy/sofb/orbit.py`

 * *Files 21% similar despite different names*

```diff
@@ -19,78 +19,24 @@
 from .bpms import BPM, TimingConfig, TIMEOUT
 
 
 class BaseOrbit(_BaseClass):
     """."""
 
 
-def run_subprocess(pvs, send_pipe, recv_pipe):
-    """Run subprocesses."""
-    max_spread = 40/1000  # in [s]
-    timeout = 110/1000  # in [s]
-
-    ready_evt = _Event()
-
-    tstamps = _np.full(len(pvs), _np.nan)
-
-    def callback(*_, **kwargs):
-        pvo = kwargs['cb_info'][1]
-        # pvo._args['timestamp'] = _time.time()
-        tstamps[pvo.index] = pvo.timestamp
-        maxi = _bn.nanmax(tstamps)
-        mini = _bn.nanmin(tstamps)
-        if (maxi-mini) < max_spread:
-            ready_evt.set()
-
-    def conn_callback(pvname=None, conn=None, pv=None):
-        if not conn:
-            tstamps[pv.index] = _np.nan
-
-    pvsobj = []
-    for i, pvn in enumerate(pvs):
-        pvo = _PV(pvn, connection_timeout=TIMEOUT)
-        pvo.index = i
-        pvsobj.append(pvo)
-
-    for pvo in pvsobj:
-        pvo.wait_for_connection()
-
-    for pvo in pvsobj:
-        pvo.add_callback(callback)
-        pvo.connection_callbacks.append(conn_callback)
-
-    boo = True
-    while boo or recv_pipe.recv():
-        boo = False
-        ready_evt.clear()
-        nok = 0.0
-        if not ready_evt.wait(timeout=timeout):
-            nok = 1.0
-        out = []
-        for pvo in pvsobj:
-            if not pvo.connected:
-                out.append(_np.nan)
-                continue
-            # out.append(pvo.timestamp)
-            out.append(pvo.value)
-        out.append(nok)
-        send_pipe.send(out)
-
-
 class EpicsOrbit(BaseOrbit):
     """Class to deal with orbit acquisition."""
 
     def __init__(self, acc, prefix='', callback=None):
         """Initialize the instance."""
         super().__init__(acc, prefix=prefix, callback=callback)
 
         self._mode = 0  # first mode of the list
         self._sofb = None
         self._sync_with_inj = False
-        self._sloworb_timeout = 0
         self.ref_orbs = {
             'X': _np.zeros(self._csorb.nr_bpms),
             'Y': _np.zeros(self._csorb.nr_bpms)}
         self._load_ref_orbs()
         self.raw_orbs = {'X': [], 'Y': []}
         self.raw_sporbs = {'X': [], 'Y': [], 'Sum': []}
         self.raw_mtorbs = {'X': [], 'Y': [], 'Sum': []}
@@ -107,19 +53,19 @@
         self._acqtrignrshots = 1
         self._multiturnidx = 0
         self._mturndownsample = 1
         self._timevector = None
         self.bpms = [BPM(name, callback) for name in self._csorb.bpm_names]
         self.timing = TimingConfig(acc, callback)
         self.new_orbit = _Event()
+        self._new_orbraw_flag = _Event()
         if self.acc == 'SI':
-            self._processes = []
-            self._mypipes_recv = []
-            self._mypipes_send = []
-            self._create_processes(nrprocs=16)
+            self._sloworb_raw_pv = _PV(
+                'SI-Glob:AP-SOFB:SlowOrbRaw-Mon',
+                callback=self._update_sloworb_raw, auto_monitor=True)
         self._orbit_thread = _Repeat(
             1/self._csorb.ACQRATE_SLOWORB, self._update_orbits, niter=0)
         self._orbit_thread.start()
         self._thread_sync = None
         self._update_time_vector()
 
     @property
@@ -127,54 +73,19 @@
         """."""
         return self._sofb
 
     @sofb.setter
     def sofb(self, sofb):
         self._sofb = sofb
 
-    def _create_processes(self, nrprocs=8):
-        # get the start method of the Processes that will be launched:
-        spw = _mp.get_context('spawn')
-
-        pvs = []
-        for bpm in self._csorb.bpm_names:
-            pvs.append(bpm+':PosX-Mon')
-        for bpm in self._csorb.bpm_names:
-            pvs.append(bpm+':PosY-Mon')
-
-        # subdivide the pv list for the processes
-        div = len(pvs) // nrprocs
-        rem = len(pvs) % nrprocs
-        sub = [div*i + min(i, rem) for i in range(nrprocs+1)]
-
-        # create processes
-        for i in range(nrprocs):
-            mine, send_pipe = spw.Pipe(duplex=False)
-            self._mypipes_recv.append(mine)
-            recv_pipe, mine = spw.Pipe(duplex=False)
-            self._mypipes_send.append(mine)
-            pvsn = pvs[sub[i]:sub[i+1]]
-            self._processes.append(_Process(
-                target=run_subprocess,
-                args=(pvsn, send_pipe, recv_pipe),
-                daemon=True))
-        for proc in self._processes:
-            proc.start()
-
     def shutdown(self):
         """."""
         self._orbit_thread.resume()
         self._orbit_thread.stop()
         self._orbit_thread.join()
-        if self.acc == 'SI':
-            for pipe in self._mypipes_send:
-                pipe.send(False)
-                pipe.close()
-            for proc in self._processes:
-                proc.join()
 
     def get_map2write(self):
         """Get the write methods of the class."""
         dbase = {
             'SOFBMode-Sel': self.set_orbit_mode,
             'SyncWithInjection-Sel': self.set_sync_with_injection,
             'TrigAcqConfig-Cmd': self.acq_config_bpms,
@@ -241,20 +152,19 @@
             mode = self._mode
         return mode == self._csorb.SOFBMode.SinglePass
 
     def is_trigmode(self, mode=None):
         """Check is mode or self._mode is in any of the Triggered modes."""
         return self.is_singlepass(mode) or self.is_multiturn(mode)
 
-    def get_orbit(self, reset=False, synced=False, timeout=1/10):
+    def get_orbit(self, reset=False, synced=False, timeout=1/5):
         """Return the orbit distortion."""
         nrb = self._csorb.nr_bpms
         refx = self.ref_orbs['X'][:nrb]
         refy = self.ref_orbs['Y'][:nrb]
-
         if reset:
             with self._lock_raw_orbs:
                 msg = 'DEB: Reseting Orbit.'
                 _log.debug(msg)
                 self._reset_orbs()
                 msg = 'DEB: Reseted Orbit.'
                 _log.debug(msg)
@@ -320,35 +230,31 @@
         self._smooth_meth = meth
         self.run_callbacks('SmoothMethod-Sts', meth)
         return True
 
     def set_spass_mask(self, val, beg=True, is_thread=False):
         """."""
         if not is_thread:
-            _Thread(
-                target=self.set_spass_mask,
-                args=(val, ), kwargs={'beg': beg, 'is_thread': True},
-                daemon=True).start()
+            self._LQTHREAD.put((
+                self.set_spass_mask, (val, ), {'beg': beg, 'is_thread': True}))
             return True
 
         val = int(val) if val > 0 else 0
         other_mask = self._spass_mask[1 if beg else 0]
         maxsz = self.bpms[0].tbtrate - other_mask - 2
         val = val if val < maxsz else maxsz
         self._spass_mask[0 if beg else 1] = val
         name = 'Beg' if beg else 'End'
         self.run_callbacks('SPassMaskSpl' + name + '-RB', val)
 
     def set_mturn_sync(self, val, is_thread=False):
         """."""
         if not is_thread:
-            _Thread(
-                target=self.set_mturn_sync,
-                args=(val, ), kwargs={'is_thread': True},
-                daemon=True).start()
+            self._LQTHREAD.put((
+                self.set_mturn_sync, (val, ), {'is_thread': True}))
             return True
 
         value = _csbpm.DsblEnbl.enabled
         if val == self._csorb.DsblEnbl.Dsbl:
             value = _csbpm.DsblEnbl.disabled
 
         mask = self._get_mask()
@@ -356,18 +262,16 @@
             bpm.put_enable = mask[i]
             bpm.tbt_sync_enbl = value
         self.run_callbacks('MTurnSyncTim-Sts', val)
 
     def set_mturn_usemask(self, val, is_thread=False):
         """."""
         if not is_thread:
-            _Thread(
-                target=self.set_mturn_usemask,
-                args=(val, ), kwargs={'is_thread': True},
-                daemon=True).start()
+            self._LQTHREAD.put((
+                self.set_mturn_usemask, (val, ), {'is_thread': True}))
             return True
 
         value = _csbpm.DsblEnbl.enabled
         if val == self._csorb.DsblEnbl.Dsbl:
             value = _csbpm.DsblEnbl.disabled
 
         mask = self._get_mask()
@@ -376,18 +280,16 @@
             bpm.tbt_mask_enbl = value
 
         self.run_callbacks('MTurnUseMask-Sts', val)
 
     def set_mturnmask(self, val, beg=True, is_thread=False):
         """."""
         if not is_thread:
-            _Thread(
-                target=self.set_mturnmask,
-                args=(val, ), kwargs={'beg': beg, 'is_thread': True},
-                daemon=True).start()
+            self._LQTHREAD.put((
+                self.set_mturnmask, (val, ), {'beg': beg, 'is_thread': True}))
             return True
 
         val = int(val) if val > 0 else 0
         bpms = self._get_used_bpms()
         omsk = \
             bpms[0].tbt_mask_begin if not beg else \
             bpms[0].tbt_mask_end
@@ -405,18 +307,16 @@
 
         name = 'Beg' if beg else 'End'
         self.run_callbacks('MTurnMaskSpl' + name + '-RB', val)
 
     def set_spass_average(self, val, is_thread=False):
         """."""
         if not is_thread:
-            _Thread(
-                target=self.set_spass_average,
-                args=(val, ), kwargs={'is_thread': True},
-                daemon=True).start()
+            self._LQTHREAD.put((
+                self.set_spass_average, (val, ), {'is_thread': True}))
             return True
 
         val = int(val) if val > 1 else 1
         with self._lock_raw_orbs:
             self._spass_average = val
             self._reset_orbs()
         self.run_callbacks('SPassAvgNrTurns-RB', val)
@@ -427,18 +327,16 @@
         with self._lock_raw_orbs:
             self._reset_orbs()
         return True
 
     def set_reforb(self, plane, orb, is_thread=False):
         """."""
         if not is_thread:
-            _Thread(
-                target=self.set_reforb,
-                args=(plane, orb), kwargs={'is_thread': True},
-                daemon=True).start()
+            self._LQTHREAD.put((
+                self.set_reforb, (plane, orb), {'is_thread': True}))
             return True
 
         msg = 'Setting New Reference Orbit.'
         self._update_log(msg)
         _log.info(msg)
         orb = _np.array(orb, dtype=float)
         nrb = self._csorb.nr_bpms
@@ -460,18 +358,16 @@
         with self._lock_raw_orbs:
             self._reset_orbs()
         self.run_callbacks('RefOrb'+plane+'-RB', orb[:nrb])
 
     def set_orbit_mode(self, value, is_thread=False):
         """."""
         if not is_thread:
-            _Thread(
-                target=self.set_orbit_mode,
-                args=(value, ), kwargs={'is_thread': True},
-                daemon=True, ).start()
+            self._LQTHREAD.put((
+                self.set_orbit_mode, (value, ), {'is_thread': True}))
             return True
 
         omode = self._mode
         acqrate = self._csorb.ACQRATE_SLOWORB
         if self.is_trigmode(value):
             acqrate = self._csorb.ACQRATE_TRIGMODE
 
@@ -522,18 +418,16 @@
         self.set_trig_acq_control(
             self._csorb.TrigAcqCtrl.Start, is_thread=True)
         return True
 
     def set_orbit_multiturn_idx(self, value, is_thread=False):
         """."""
         if not is_thread:
-            _Thread(
-                target=self.set_orbit_multiturn_idx,
-                args=(value, ), kwargs={'is_thread': True},
-                daemon=True).start()
+            self._LQTHREAD.put((
+                self.set_orbit_multiturn_idx, (value, ), {'is_thread': True}))
             return True
 
         maxidx = self.acqtrignrsamples // self._mturndownsample
         maxidx *= self._acqtrignrshots
         if value >= maxidx:
             value = maxidx-1
             msg = 'WARN: MTurnIdx is too large. Redefining...'
@@ -546,18 +440,16 @@
             'MTurnIdxTime-Mon', self._timevector[self._multiturnidx])
         self._update_multiturn_orbit_pvs()
 
     def acq_config_bpms(self, *args, is_thread=False):
         """."""
         _ = args
         if not is_thread:
-            _Thread(
-                target=self.acq_config_bpms,
-                kwargs={'is_thread': True},
-                daemon=True).start()
+            self._LQTHREAD.put((
+                self.acq_config_bpms, tuple(), {'is_thread': True}))
             return True
 
         msg = 'Configuring BPMs...'
         self._update_log(msg)
         _log.info(msg)
 
         mask = self._get_mask()
@@ -626,33 +518,29 @@
         msg = 'Syncing BPMs is done!'
         self._update_log(msg)
         _log.info(msg)
 
     def set_trig_acq_control(self, value, is_thread=False):
         """."""
         if not is_thread:
-            _Thread(
-                target=self.set_trig_acq_control,
-                args=(value, ), kwargs={'is_thread': True},
-                daemon=True).start()
+            self._LQTHREAD.put((
+                self.set_trig_acq_control, (value, ), {'is_thread': True}))
             return True
 
         mask = self._get_mask()
         for i, bpm in enumerate(self.bpms):
             bpm.put_enable = mask[i]
             bpm.ctrl = value
         self.run_callbacks('TrigAcqCtrl-Sts', value)
 
     def set_trig_acq_channel(self, value, is_thread=False):
         """."""
         if not is_thread:
-            _Thread(
-                target=self.set_trig_acq_channel,
-                args=(value, ), kwargs={'is_thread': True},
-                daemon=True).start()
+            self._LQTHREAD.put((
+                self.set_trig_acq_channel, (value, ), {'is_thread': True}))
             return True
 
         try:
             val = self._csorb.TrigAcqChan._fields[value]
             val = _csbpm.AcqChan._fields.index(val)
         except (IndexError, ValueError):
             return False
@@ -664,33 +552,30 @@
 
         self.run_callbacks('TrigAcqChan-Sts', value)
         self._update_time_vector(channel=val)
 
     def set_trig_acq_repeat(self, value, is_thread=False):
         """."""
         if not is_thread:
-            _Thread(
-                target=self.set_trig_acq_repeat,
-                args=(value, ), kwargs={'is_thread': True},
-                daemon=True).start()
+            self._LQTHREAD.put((
+                self.set_trig_acq_repeat, (value, ), {'is_thread': True}))
             return True
 
         mask = self._get_mask()
         for i, bpm in enumerate(self.bpms):
             bpm.put_enable = mask[i]
             bpm.acq_repeat = value
         self.run_callbacks('TrigAcqRepeat-Sts', value)
 
     def set_acq_nrsamples(self, val, ispost=True, is_thread=False):
         """."""
         if not is_thread:
-            _Thread(
-                target=self.set_acq_nrsamples,
-                args=(val, ), kwargs={'ispost': ispost, 'is_thread': True},
-                daemon=True).start()
+            self._LQTHREAD.put((
+                self.set_acq_nrsamples, (val, ),
+                {'ispost': ispost, 'is_thread': True}))
             return True
 
         val = int(val) if val > 0 else 0
         val = val if val < 20000 else 20000
         suf = 'post' if ispost else 'pre'
         oth = 'post' if not ispost else 'pre'
         if getattr(self, '_acqtrignrsamples' + oth) == 0 and val == 0:
@@ -706,18 +591,16 @@
             setattr(self, '_acqtrignrsamples' + suf, val)
         self.run_callbacks('TrigNrSamples'+suf.title()+'-RB', val)
         self._update_time_vector()
 
     def set_trig_acq_nrshots(self, val, is_thread=False):
         """."""
         if not is_thread:
-            _Thread(
-                target=self.set_trig_acq_nrshots,
-                args=(val, ), kwargs={'is_thread': True},
-                daemon=True).start()
+            self._LQTHREAD.put((
+                self.set_trig_acq_nrshots, (val, ), {'is_thread': True}))
             return True
 
         val = int(val) if val > 1 else 1
         val = val if val < 1000 else 1000
         with self._lock_raw_orbs:
             mask = self._get_mask()
             for i, bpm in enumerate(self.bpms):
@@ -728,51 +611,46 @@
             self._acqtrignrshots = val
         self.run_callbacks('TrigNrShots-RB', val)
         self._update_time_vector()
 
     def set_poly_calibration(self, val, is_thread=False):
         """."""
         if not is_thread:
-            _Thread(
-                target=self.set_poly_calibration,
-                args=(val, ), kwargs={'is_thread': True},
-                daemon=True).start()
+            self._LQTHREAD.put((
+                self.set_poly_calibration, (val, ), {'is_thread': True}))
             return True
 
         value = _csbpm.DsblEnbl.enabled
         if val == self._csorb.DsblEnbl.Dsbl:
             value = _csbpm.DsblEnbl.disabled
         mask = self._get_mask()
         for i, bpm in enumerate(self.bpms):
             bpm.put_enable = mask[i]
             bpm.polycal = value
         self.run_callbacks('PolyCalibration-Sts', val)
 
     def set_mturndownsample(self, val, is_thread=False):
         """."""
         if not is_thread:
-            _Thread(
-                target=self.set_mturndownsample,
-                args=(val, ), kwargs={'is_thread': True},
-                daemon=True).start()
+            self._LQTHREAD.put((
+                self.set_mturndownsample, (val, ), {'is_thread': True}))
             return True
 
         val = int(val) if val > 1 else 1
         val = val if val < 1000 else 1000
         with self._lock_raw_orbs:
             self._mturndownsample = val
             self._reset_orbs()
         self.run_callbacks('MTurnDownSample-RB', val)
         self._prepare_mode()
 
     def acquire_mturn_orbit(self, _):
         """Acquire Multiturn data from BPMs."""
-        _Thread(
-            target=self._update_multiturn_orbits,
-            kwargs=dict(force_update=True), daemon=True).start()
+        self._LQTHREAD.put((
+            self._update_multiturn_orbits, tuple(), dict(force_update=True)))
         return True
 
     def _update_time_vector(self, delay=None, duration=None, channel=None):
         """."""
         if not self.isring:
             return
         dly = (delay or self.timing.totaldelay or 0.0) * 1e-6  # from us to s
@@ -861,17 +739,25 @@
             self.run_callbacks('BufferCount-Mon', count)
         except Exception as err:
             self._update_log('ERR: ' + str(err))
             _log.error(_traceback.format_exc())
 
     def _update_online_orbits(self):
         """."""
-        posx, posy, nok = self._get_orbit_from_processes()
-        posx /= 1000
-        posy /= 1000
+        timeout = 1000/1000
+        if not self._new_orbraw_flag.wait(timeout=timeout):
+            msg = 'ERR: Raw orbit did not update.'
+            self._update_log(msg)
+            _log.error(msg[5:])
+            return
+        else:
+            self._new_orbraw_flag.clear()
+
+        orb = self._sloworb_raw_pv.value
+        posx, posy = orb[:self._csorb.nr_bpms], orb[self._csorb.nr_bpms:]
         nanx = _np.isnan(posx)
         nany = _np.isnan(posy)
         posx[nanx] = self.ref_orbs['X'][nanx]
         posy[nany] = self.ref_orbs['Y'][nany]
         orbs = {'X': posx, 'Y': posy}
 
         for plane in ('X', 'Y'):
@@ -884,42 +770,28 @@
                 if self._smooth_meth == self._csorb.SmoothMeth.Average:
                     orb = _np.mean(raws[plane], axis=0)
                 else:
                     orb = _np.median(raws[plane], axis=0)
                 self.smooth_orb[plane] = orb
         self.new_orbit.set()
 
-        self._sloworb_timeout += nok
-        if self._sloworb_timeout >= 1000:
-            self._sloworb_timeout = 0
-        self.run_callbacks('SlowOrbTimeout-Mon', self._sloworb_timeout)
         for plane in ('X', 'Y'):
             orb = self.smooth_orb[plane]
             if orb is None:
                 return
             dorb = orb - self.ref_orbs[plane]
             self.run_callbacks(f'SlowOrb{plane:s}-Mon', _np.array(orb))
             self.run_callbacks(f'DeltaOrb{plane:s}Avg-Mon', _bn.nanmean(dorb))
             self.run_callbacks(f'DeltaOrb{plane:s}Std-Mon', _bn.nanstd(dorb))
             self.run_callbacks(f'DeltaOrb{plane:s}Min-Mon', _bn.nanmin(dorb))
             self.run_callbacks(f'DeltaOrb{plane:s}Max-Mon', _bn.nanmax(dorb))
 
-    def _get_orbit_from_processes(self):
-        nr_bpms = self._csorb.nr_bpms
-        out = []
-        nok = []
-        for pipe in self._mypipes_recv:
-            res = pipe.recv()
-            out.extend(res[:-1])
-            nok.append(res[-1])
-        for pipe in self._mypipes_send:
-            pipe.send(True)
-        orbx = _np.array(out[:nr_bpms], dtype=float)
-        orby = _np.array(out[nr_bpms:], dtype=float)
-        return orbx, orby, any(nok)
+    def _update_sloworb_raw(self, pvname, value, **kwrgs):
+        _ = pvname, value, kwrgs
+        self._new_orbraw_flag.set()
 
     def _update_multiturn_orbits(self, force_update=True):
         """."""
         orbs = {'X': [], 'Y': [], 'Sum': []}
         with self._lock_raw_orbs:  # I need the lock here to ensure consistency
             leng = len(self.raw_mtorbs['X'])
             samp = self.acqtrignrsamples
@@ -1077,14 +949,17 @@
         if self.is_trigmode():
             isok = all(map(lambda x: x.is_ok, bpms))
         elif self.is_sloworb():
             isok = all(map(
                 lambda x: x.switching_mode == _csbpm.SwModes.switching, bpms))
         status = _util.update_bit(v=status, bit_pos=4, bit_val=not isok)
 
+        orb_conn = self._sloworb_raw_pv.connected if self.acc == 'SI' else True
+        status = _util.update_bit(v=status, bit_pos=5, bit_val=not orb_conn)
+
         self._status = status
         self.run_callbacks('OrbStatus-Mon', status)
         self._update_bpmoffsets()
 
     def _update_bpmoffsets(self):
         """."""
         nrb = self._csorb.nr_bpms
@@ -1093,14 +968,15 @@
         for i, bpm in enumerate(self.bpms):
             orbx[i::nrb] = bpm.offsetx or 0.0
             orby[i::nrb] = bpm.offsety or 0.0
         self.run_callbacks('BPMOffsetX-Mon', orbx)
         self.run_callbacks('BPMOffsetY-Mon', orby)
 
     def _get_mask(self):
+        mask = _np.ones(self._csorb.nr_bpms, dtype=bool)
         if self.sofb is not None and self.sofb.matrix is not None:
             mask = self.sofb.matrix.bpm_enbllist
             mask = mask[:mask.size//2] & mask[mask.size//2:]
             mask = mask[:len(self.bpms)]
         return mask
 
     def _get_used_bpms(self):
```

### Comparing `siriuspy-2.76.1/siriuspy/sofb/utils.py` & `siriuspy-2.77.0/siriuspy/sofb/utils.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/siriuspy/stabinfo/csdev.py` & `siriuspy-2.77.0/siriuspy/stabinfo/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/siriuspy/stabinfo/main.py` & `siriuspy-2.77.0/siriuspy/stabinfo/main.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/siriuspy/thread.py` & `siriuspy-2.77.0/siriuspy/thread.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,25 +1,29 @@
 """Definition of thread classes to used across the package."""
 
 import time as _time
 from threading import Thread as _Thread, Event as _Event, \
     Lock as _Lock
-from queue import Queue as _Queue
-from collections import deque as _deque
+from queue import Queue as _Queue, Empty as _Empty, Full as _Full
+
+from epics.ca import use_initial_context as _use_initial_context
+
+from .epics import CAThread as _CAThread
 
 
 class AsyncWorker(_Thread):
     """Asynchronous Worker Thread.
 
     Performs asynchronous jobs indefinitely.
     """
 
-    def __init__(self, name=None):
+    def __init__(self, name=None, is_cathread=False):
         """."""
         super().__init__(name=name, daemon=True)
+        self.is_cathread = is_cathread
         self._evt_received = _Event()
         self._evt_ready = _Event()
         self._evt_ready.set()
         self._evt_stop = _Event()
         self.target = None
         self.args = tuple()
 
@@ -44,99 +48,63 @@
 
     def stop(self):
         """Stop thread."""
         self._evt_stop.set()
 
     def run(self):
         """."""
+        if self.is_cathread:
+            _use_initial_context()
         while not self._evt_stop.is_set():
             if self._evt_received.wait(0.5):
                 self._evt_received.clear()
                 self.target(*self.args)
                 self._evt_ready.set()
 
 
-class QueueThread(_Thread):
-    """Callback queue class.
-
-        Queues threads of this class are used to process callbacks of power
-    supplies (magnets) properties among others.
-    """
-
-    # NOTE: QueueThread was reported as generating unstable behaviour
-    # when used intensively in the SOFB IOC. Currently this class is
-    # used in as-ps-diag IOC classes.
-    # TODO: investigate this issue!
-
-    def __init__(self):
-        """Init method."""
-        super().__init__(daemon=True)
-        self._queue = _Queue()
-        self._running = False
-
-    @property
-    def running(self):
-        """Return whether thread is running."""
-        return self._running
-
-    def add_callback(self, func, *args, **kwargs):
-        """Add callback."""
-        if not hasattr(func, '__call__'):
-            raise TypeError('Argument "func" is not callable.')
-        self._queue.put((func, args, kwargs))
-
-    def run(self):
-        """Run method."""
-        self._running = True
-        while self.running:
-            func_item = self._queue.get()
-            nitems = self._queue.qsize()
-            if nitems and nitems % 500 == 0:
-                print("Warning: Queue size is {}!".format(nitems))
-            function, args, kwargs = func_item
-            function(*args, **kwargs)  # run the show!
-
-    def stop(self):
-        """Stop queue thread."""
-        self._running = False
-
-
 class RepeaterThread(_Thread):
     """Repeat execution of predefined function for a given number of times."""
 
-    def __init__(self, interval, function, args=None, kwargs=None, niter=0):
+    def __init__(
+            self, interval, function, args=None, kwargs=None, niter=0,
+            is_cathread=False):
         """Init method.
 
         Inputs:
         - interval: time to wait between sucessive calls to method.
         - function: method to be executed.
         - args: tuple of positional arguments of method
         - kwargs: dictionary with keyword arguments of method.
         - niter: number of times to execute method. If niter is zero or None
             it will be executed indefinetly until stop is called.
+        - whether to use CAThread logic .
         """
         if args is None:
             args = tuple()
         if kwargs is None:
             kwargs = dict()
         super().__init__(daemon=True)
+        self.is_cathread = is_cathread
         self.interval = interval
         if not hasattr(function, '__call__'):
             raise TypeError('Argument "function" is not callable.')
         self.function = function
         self.args = args
         self.kwargs = kwargs
         self.niters = niter
         self.cur_iter = 0
         self._stopped = _Event()
         self._unpaused = _Event()
         self._unpaused.set()
 
     def run(self):
         """Run method."""
+        if self.is_cathread:
+            _use_initial_context()
+
         self._unpaused.wait()
         self.function(*self.args, **self.kwargs)
         dtime = 0.0
         while ((not self._stopped.wait(self.interval - dtime)) and
                (not self.niters or self.niters > self.cur_iter)):
             self._unpaused.wait()
             if self._stopped.is_set():
@@ -172,103 +140,141 @@
 
     def stop(self):
         """Stop execution."""
         self._unpaused.set()
         self._stopped.set()
 
 
-class DequeThread(_deque):
-    """DequeThread.
+class _BaseQueueThread(_Queue):
+    """QueueThread.
 
-    This class manages generic operations (actions) using an append-right,
-    pop-left queue. Each operation processing is a method invoked as a separate
-    thread.
+    This class manages generic operations (actions) using a FIFO queue. Each
+    operation processing is a method invoked as a separate thread. It also has
+    process loop methods to continuously process its operation queue in a
+    single thread.
     """
 
-    def __init__(self):
+    def __init__(self, is_cathread=False):
         """Init."""
         super().__init__()
+        self.is_cathread = is_cathread
         self._last_operation = None
-        self._thread = None
-        self._ignore = False
-        self._enabled = True
-        self._lock = _Lock()
+        self._th = None
+        self._changing_queue = _Lock()
 
     @property
     def last_operation(self):
         """Return last operation."""
         return self._last_operation
 
     @property
-    def enabled(self):
-        """Enable process."""
-        return self._enabled
-
-    @enabled.setter
-    def enabled(self, value):
-        self._enabled = value
-
-    def ignore_set(self):
-        """Turn ignore state on."""
-        self._ignore = True
-
-    def ignore_clear(self):
-        """Turn ignore state on."""
-        self._ignore = False
-
-    def append(self, operation, unique=False):
-        """Append operation to queue."""
-        with self._lock:
-            if self._ignore or (unique and self.count(operation) > 0):
-                return False
+    def is_running(self):
+        """."""
+        return self._th is not None and self._th.is_alive()
+
+    def put(self, operation, block=True, timeout=None):
+        """Put operation to queue."""
+        if not hasattr(operation, '__len__'):
+            operation = (operation, )
+        if not hasattr(operation[0], '__call__'):
+            raise TypeError(
+                'First element of "operation" is not callable.')
 
-            if not hasattr(operation, '__len__'):
-                operation = (operation, )
-            if not hasattr(operation[0], '__call__'):
-                raise TypeError(
-                    'First element of "operation" is not callable.')
-            super().append(operation)
+        with self._changing_queue:
+            try:
+                super().put(operation, block=block, timeout=timeout)
+            except _Full:
+                return False
             self._last_operation = operation
-            return True
+        return True
+
+    def get(self, block=True, timeout=None):
+        """Get operation from queue."""
+        with self._changing_queue:
+            try:
+                return super().get(block=block, timeout=timeout)
+            except _Empty:
+                return None
+
+    def _get_operation(self, block=True, timeout=None):
+        """Raise queue.Empty exception in case of timeout or empty Queue."""
+        operation = super().get(block=block, timeout=timeout)
+        # process operation taken from queue
+        args, kws = tuple(), dict()
+        if len(operation) == 1:
+            func = operation[0]
+        elif len(operation) == 2:
+            func, args = operation
+        elif len(operation) >= 3:
+            func, args, kws = operation[:3]
+        return func, args, kws
+
+    def _run_process(self, func, args, kws):
+        """."""
+        try:
+            func(*args, **kws)
+        except Exception:
+            pass
+        self.task_done()
 
-    def clear(self):
-        """Clear deque."""
-        with self._lock:
-            super().clear()
-
-    def pop(self):
-        """Pop operation from queue."""
-        with self._lock:
-            return super().pop()
-
-    def popleft(self):
-        """Pop left operation from queue."""
-        with self._lock:
-            return super().popleft()
 
-    def process(self):
+class QueueThreads(_BaseQueueThread):
+    """QueueThreads.
+
+    This class manages generic operations (actions) using a FIFO queue. Each
+    operation processing is a method invoked as a separate thread.
+    """
+
+    def process(self, block=True, timeout=None):
         """Process operation from queue."""
-        # first check if a thread is already running
-        with self._lock:
-            donothing = not self._enabled
-            donothing |= self._thread is not None and self._thread.is_alive()
-            if donothing:
+        with self._changing_queue:
+            # first check if a thread is already running
+            if self.is_running:
                 return False
-
             # no thread is running, we can process queue
             try:
-                operation = super().popleft()
-            except IndexError:
-                # there is nothing in the queue
+                func, args, kws = self._get_operation(block, timeout)
+            except _Empty:
                 return False
-            # process operation taken from queue
-            args, kws = tuple(), dict()
-            if len(operation) == 1:
-                func = operation[0]
-            elif len(operation) == 2:
-                func, args = operation
-            elif len(operation) >= 3:
-                func, args, kws = operation[:3]
-            self._thread = _Thread(
-                target=func, args=args, kwargs=kws, daemon=True)
-            self._thread.start()
+            th_cls = _CAThread if self.is_cathread else _Thread
+            self._th = th_cls(
+                target=self._run_process, args=(func, args, kws), daemon=True)
+            self._th.start()
             return True
+
+
+class LoopQueueThread(_BaseQueueThread):
+    """LoopQueueThread.
+
+    This class manages generic operations (actions) using a FIFO queue.
+    It has a process loop to continuously process its operation queue in a
+    single thread.
+    """
+
+    def __init__(self, is_cathread=False):
+        """Init."""
+        super().__init__(is_cathread=is_cathread)
+        self._loop_stop_evt = _Event()
+
+    def start(self):
+        """Run deque process loop."""
+        # check if there is a previously running loop
+        self._loop_stop_evt.clear()
+        if self.is_running:
+            return
+        # start new process loop
+        th_cls = _CAThread if self.is_cathread else _Thread
+        self._th = th_cls(target=self._loop_run_process, daemon=True)
+        self._th.start()
+
+    def stop(self):
+        """Stop deque process loop."""
+        self._loop_stop_evt.set()
+
+    def _loop_run_process(self):
+        while not self._loop_stop_evt.is_set():
+            try:
+                func, args, kws = self._get_operation(True, timeout=1)
+                self._run_process(func, args, kws)
+            except _Empty:
+                continue
+        self._loop_stop_evt.clear()
```

### Comparing `siriuspy-2.76.1/siriuspy/timesys/csdev.py` & `siriuspy-2.77.0/siriuspy/timesys/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/siriuspy/timesys/hl_classes.py` & `siriuspy-2.77.0/siriuspy/timesys/hl_classes.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/siriuspy/timesys/ll_classes.py` & `siriuspy-2.77.0/siriuspy/timesys/ll_classes.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/siriuspy/timesys/plot_network.py` & `siriuspy-2.77.0/siriuspy/timesys/plot_network.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/siriuspy/timesys/static_table.py` & `siriuspy-2.77.0/siriuspy/timesys/static_table.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/siriuspy/util.py` & `siriuspy-2.77.0/siriuspy/util.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/siriuspy.egg-info/PKG-INFO` & `siriuspy-2.77.0/siriuspy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: siriuspy
-Version: 2.76.1
+Version: 2.77.0
 Summary: Development packages for Sirius
 Home-page: https://github.com/lnls-sirius/dev-packages
 Download-URL: https://github.com/lnls-sirius/dev-packages
 Author: lnls-sirius
 License: GNU GPLv3
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python
```

### Comparing `siriuspy-2.76.1/siriuspy.egg-info/SOURCES.txt` & `siriuspy-2.77.0/siriuspy.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -161,18 +161,19 @@
 siriuspy/idff/main.py
 siriuspy/injctrl/__init__.py
 siriuspy/injctrl/bias_feedback.py
 siriuspy/injctrl/csdev.py
 siriuspy/injctrl/main.py
 siriuspy/machshift/__init__.py
 siriuspy/machshift/csdev.py
+siriuspy/machshift/gensumm_macreport.py
 siriuspy/machshift/macreport.py
 siriuspy/machshift/macschedule.py
 siriuspy/machshift/main.py
-siriuspy/machshift/test_macreport.py
+siriuspy/machshift/savedata_macreport.py
 siriuspy/machshift/utils.py
 siriuspy/magnet/__init__.py
 siriuspy/magnet/data.py
 siriuspy/magnet/excdata.py
 siriuspy/magnet/factory.py
 siriuspy/magnet/normalizer.py
 siriuspy/magnet/util.py
```

### Comparing `siriuspy-2.76.1/tests/bsmp/test_bsmp.py` & `siriuspy-2.77.0/tests/bsmp/test_bsmp.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/tests/bsmp/test_commands.py` & `siriuspy-2.77.0/tests/bsmp/test_commands.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/tests/bsmp/test_entities.py` & `siriuspy-2.77.0/tests/bsmp/test_entities.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/tests/bsmp/test_serial.py` & `siriuspy-2.77.0/tests/bsmp/test_serial.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/tests/bsmp/test_types.py` & `siriuspy-2.77.0/tests/bsmp/test_types.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/tests/clientconfigdb/test_configdb_client.py` & `siriuspy-2.77.0/tests/clientconfigdb/test_configdb_client.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/tests/clientweb/test_implementation.py` & `siriuspy-2.77.0/tests/clientweb/test_implementation.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/tests/currinfo/lifetime/test_main.py` & `siriuspy-2.77.0/tests/currinfo/lifetime/test_main.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/tests/currinfo/test_csdev.py` & `siriuspy-2.77.0/tests/currinfo/test_csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/tests/currinfo/test_main.py` & `siriuspy-2.77.0/tests/currinfo/test_main.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/tests/magnet/test_factory.py` & `siriuspy-2.77.0/tests/magnet/test_factory.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/tests/magnet/tests_normalizer.py` & `siriuspy-2.77.0/tests/magnet/tests_normalizer.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/tests/mock_servweb.py` & `siriuspy-2.77.0/tests/mock_servweb.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/tests/namesys/test_implementation.py` & `siriuspy-2.77.0/tests/namesys/test_implementation.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/tests/opticscorr/test_chrom.py` & `siriuspy-2.77.0/tests/opticscorr/test_chrom.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/tests/opticscorr/test_csdev.py` & `siriuspy-2.77.0/tests/opticscorr/test_csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/tests/opticscorr/test_opticscorr.py` & `siriuspy-2.77.0/tests/opticscorr/test_opticscorr.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/tests/opticscorr/test_tune.py` & `siriuspy-2.77.0/tests/opticscorr/test_tune.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/tests/opticscorr/test_utils.py` & `siriuspy-2.77.0/tests/opticscorr/test_utils.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/tests/posang/test_csdev.py` & `siriuspy-2.77.0/tests/posang/test_csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/tests/posang/test_main.py` & `siriuspy-2.77.0/tests/posang/test_main.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/tests/pwrsupply/db.py` & `siriuspy-2.77.0/tests/pwrsupply/db.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/tests/pwrsupply/pructrl/test_pru.py` & `siriuspy-2.77.0/tests/pwrsupply/pructrl/test_pru.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/tests/pwrsupply/psctrl/test_pscwriters.py` & `siriuspy-2.77.0/tests/pwrsupply/psctrl/test_pscwriters.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/tests/pwrsupply/test_csdev.py` & `siriuspy-2.77.0/tests/pwrsupply/test_csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/tests/pwrsupply/test_data.py` & `siriuspy-2.77.0/tests/pwrsupply/test_data.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/tests/pwrsupply/test_siggen.py` & `siriuspy-2.77.0/tests/pwrsupply/test_siggen.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/tests/pwrsupply/variables.py` & `siriuspy-2.77.0/tests/pwrsupply/variables.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/tests/ramp/test_magnet.py` & `siriuspy-2.77.0/tests/ramp/test_magnet.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/tests/ramp/test_waveform.py` & `siriuspy-2.77.0/tests/ramp/test_waveform.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/tests/search/test_hl_time_search.py` & `siriuspy-2.77.0/tests/search/test_hl_time_search.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/tests/search/test_init.py` & `siriuspy-2.77.0/tests/search/test_init.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/tests/search/test_ll_time_search.py` & `siriuspy-2.77.0/tests/search/test_ll_time_search.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/tests/search/test_ma_search.py` & `siriuspy-2.77.0/tests/search/test_ma_search.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/tests/search/test_ps_search.py` & `siriuspy-2.77.0/tests/search/test_ps_search.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/tests/test_callbacks.py` & `siriuspy-2.77.0/tests/test_callbacks.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/tests/test_csdev.py` & `siriuspy-2.77.0/tests/test_csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/tests/test_envars.py` & `siriuspy-2.77.0/tests/test_envars.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/tests/test_util.py` & `siriuspy-2.77.0/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/tests/timesys/test_csdev.py` & `siriuspy-2.77.0/tests/timesys/test_csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.76.1/tests/timesys/test_plot_network.py` & `siriuspy-2.77.0/tests/timesys/test_plot_network.py`

 * *Files identical despite different names*

