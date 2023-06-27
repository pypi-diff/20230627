# Comparing `tmp/lightcon-1.4.2.post1.tar.gz` & `tmp/lightcon-1.4.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lightcon-1.4.2.post1.tar", last modified: Tue Jun 27 11:54:42 2023, max compression
+gzip compressed data, was "lightcon-1.4.2.post2.tar", last modified: Tue Jun 27 12:50:23 2023, max compression
```

## Comparing `lightcon-1.4.2.post1.tar` & `lightcon-1.4.2.post2.tar`

### file list

```diff
@@ -1,76 +1,86 @@
-drwxrwxrwx   0        0        0        0 2023-06-27 11:54:42.369257 lightcon-1.4.2.post1/
--rw-rw-rw-   0        0        0     1082 2023-06-27 11:52:52.000000 lightcon-1.4.2.post1/LICENCE
--rw-rw-rw-   0        0        0      249 2023-06-27 11:52:52.000000 lightcon-1.4.2.post1/MANIFEST.in
--rw-rw-rw-   0        0        0     6258 2023-06-27 11:54:42.369257 lightcon-1.4.2.post1/PKG-INFO
--rw-rw-rw-   0        0        0     5605 2023-06-27 11:52:52.000000 lightcon-1.4.2.post1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-27 11:54:41.892080 lightcon-1.4.2.post1/lightcon/
--rw-rw-rw-   0        0        0        0 2023-06-27 11:52:52.000000 lightcon-1.4.2.post1/lightcon/__config__.py
--rw-rw-rw-   0        0        0      717 2023-06-27 11:52:52.000000 lightcon-1.4.2.post1/lightcon/__init__.py
--rw-rw-rw-   0        0        0        0 2023-06-27 11:52:52.000000 lightcon-1.4.2.post1/lightcon/_globals.py
-drwxrwxrwx   0        0        0        0 2023-06-27 11:54:41.907724 lightcon-1.4.2.post1/lightcon/beam_alignment/
--rw-rw-rw-   0        0        0       93 2023-06-27 11:52:52.000000 lightcon-1.4.2.post1/lightcon/beam_alignment/__init__.py
--rw-rw-rw-   0        0        0     2105 2023-06-27 11:52:52.000000 lightcon-1.4.2.post1/lightcon/beam_alignment/_beam_alignment.py
-drwxrwxrwx   0        0        0        0 2023-06-27 11:54:41.907724 lightcon-1.4.2.post1/lightcon/calculate/
--rw-rw-rw-   0        0        0      190 2023-06-27 11:52:52.000000 lightcon-1.4.2.post1/lightcon/calculate/__init__.py
--rw-rw-rw-   0        0        0     2997 2023-06-27 11:52:52.000000 lightcon-1.4.2.post1/lightcon/calculate/_beam_profiling_gauss.py
--rw-rw-rw-   0        0        0     3393 2023-06-27 11:52:52.000000 lightcon-1.4.2.post1/lightcon/calculate/_beam_profiling_iso.py
--rw-rw-rw-   0        0        0     1407 2023-06-27 11:52:52.000000 lightcon-1.4.2.post1/lightcon/calculate/_calculate_motor_parameters.py
-drwxrwxrwx   0        0        0        0 2023-06-27 11:54:41.907724 lightcon-1.4.2.post1/lightcon/camera_app_client/
--rw-rw-rw-   0        0        0       76 2023-06-27 11:52:52.000000 lightcon-1.4.2.post1/lightcon/camera_app_client/__init__.py
--rw-rw-rw-   0        0        0     2965 2023-06-27 11:52:52.000000 lightcon-1.4.2.post1/lightcon/camera_app_client/_camera_app_client.py
-drwxrwxrwx   0        0        0        0 2023-06-27 11:54:41.907724 lightcon-1.4.2.post1/lightcon/common/
--rw-rw-rw-   0        0        0      614 2023-06-27 11:52:52.000000 lightcon-1.4.2.post1/lightcon/common/__init__.py
--rw-rw-rw-   0        0        0      931 2023-06-27 11:52:52.000000 lightcon-1.4.2.post1/lightcon/common/_converters.py
--rw-rw-rw-   0        0        0     3155 2023-06-27 11:52:52.000000 lightcon-1.4.2.post1/lightcon/common/_http_methods.py
--rw-rw-rw-   0        0        0     5607 2023-06-27 11:52:52.000000 lightcon-1.4.2.post1/lightcon/common/_leprecan_provider.py
--rw-rw-rw-   0        0        0      336 2023-06-27 11:52:52.000000 lightcon-1.4.2.post1/lightcon/common/_load_motor_and_stage_parameters.py
--rw-rw-rw-   0        0        0     1042 2023-06-27 11:52:52.000000 lightcon-1.4.2.post1/lightcon/common/_serial_tools.py
--rw-rw-rw-   0        0        0     5151 2023-06-27 11:52:52.000000 lightcon-1.4.2.post1/lightcon/common/_udp_locator.py
--rw-rw-rw-   0        0        0      506 2023-06-27 11:52:52.000000 lightcon-1.4.2.post1/lightcon/common/stage_parameters.py
-drwxrwxrwx   0        0        0        0 2023-06-27 11:54:41.907724 lightcon-1.4.2.post1/lightcon/datasets/
--rw-rw-rw-   0        0        0      159 2023-06-27 11:52:52.000000 lightcon-1.4.2.post1/lightcon/datasets/__init__.py
--rw-rw-rw-   0        0        0     3055 2023-06-27 11:52:52.000000 lightcon-1.4.2.post1/lightcon/datasets/_base.py
-drwxrwxrwx   0        0        0        0 2023-06-27 11:54:42.369257 lightcon-1.4.2.post1/lightcon/datasets/data/
--rw-rw-rw-   0        0        0        0 2023-06-27 11:52:52.000000 lightcon-1.4.2.post1/lightcon/datasets/data/__init__.py
--rw-rw-rw-   0        0        0    11968 2023-06-27 11:53:57.000000 lightcon-1.4.2.post1/lightcon/datasets/data/motor_parameters.json
--rw-rw-rw-   0        0        0     4990 2023-06-27 11:53:57.000000 lightcon-1.4.2.post1/lightcon/datasets/data/stage_parameters.json
-drwxrwxrwx   0        0        0        0 2023-06-27 11:54:42.369257 lightcon-1.4.2.post1/lightcon/eth_motor_board/
--rw-rw-rw-   0        0        0      204 2023-06-27 11:52:52.000000 lightcon-1.4.2.post1/lightcon/eth_motor_board/__init__.py
--rw-rw-rw-   0        0        0    15177 2023-06-27 11:52:52.000000 lightcon-1.4.2.post1/lightcon/eth_motor_board/_eth_motor_board.py
--rw-rw-rw-   0        0        0     1920 2023-06-27 11:52:52.000000 lightcon-1.4.2.post1/lightcon/eth_motor_board/_eth_motor_board_leprecan_provider.py
-drwxrwxrwx   0        0        0        0 2023-06-27 11:54:42.369257 lightcon-1.4.2.post1/lightcon/fast_daq/
--rw-rw-rw-   0        0        0      130 2023-06-27 11:52:52.000000 lightcon-1.4.2.post1/lightcon/fast_daq/__init__.py
--rw-rw-rw-   0        0        0     5442 2023-06-27 11:52:52.000000 lightcon-1.4.2.post1/lightcon/fast_daq/_fast_daq.py
-drwxrwxrwx   0        0        0        0 2023-06-27 11:54:42.369257 lightcon-1.4.2.post1/lightcon/harpia/
--rw-rw-rw-   0        0        0      237 2023-06-27 11:52:52.000000 lightcon-1.4.2.post1/lightcon/harpia/__init__.py
--rw-rw-rw-   0        0        0    24803 2023-06-27 11:52:52.000000 lightcon-1.4.2.post1/lightcon/harpia/_harpia.py
--rw-rw-rw-   0        0        0     2222 2023-06-27 11:52:52.000000 lightcon-1.4.2.post1/lightcon/harpia/_harpia_leprecan_provider.py
--rw-rw-rw-   0        0        0     8813 2023-06-27 11:52:52.000000 lightcon-1.4.2.post1/lightcon/harpia/_harpia_model_decoder.py
-drwxrwxrwx   0        0        0        0 2023-06-27 11:54:42.369257 lightcon-1.4.2.post1/lightcon/harpia_daq/
--rw-rw-rw-   0        0        0       84 2023-06-27 11:52:52.000000 lightcon-1.4.2.post1/lightcon/harpia_daq/__init__.py
--rw-rw-rw-   0        0        0     5744 2023-06-27 11:52:52.000000 lightcon-1.4.2.post1/lightcon/harpia_daq/_harpia_daq.py
-drwxrwxrwx   0        0        0        0 2023-06-27 11:54:42.369257 lightcon-1.4.2.post1/lightcon/laser_clients/
--rw-rw-rw-   0        0        0       91 2023-06-27 11:52:52.000000 lightcon-1.4.2.post1/lightcon/laser_clients/__init__.py
--rw-rw-rw-   0        0        0     8634 2023-06-27 11:52:52.000000 lightcon-1.4.2.post1/lightcon/laser_clients/_laser_clients.py
-drwxrwxrwx   0        0        0        0 2023-06-27 11:54:42.369257 lightcon-1.4.2.post1/lightcon/style/
--rw-rw-rw-   0        0        0      229 2023-06-27 11:52:52.000000 lightcon-1.4.2.post1/lightcon/style/__init__.py
--rw-rw-rw-   0        0        0     7848 2023-06-27 11:52:52.000000 lightcon-1.4.2.post1/lightcon/style/_plotstyle_1d.py
--rw-rw-rw-   0        0        0     7839 2023-06-27 11:52:52.000000 lightcon-1.4.2.post1/lightcon/style/plotstyle_1d.py
-drwxrwxrwx   0        0        0        0 2023-06-27 11:54:42.369257 lightcon-1.4.2.post1/lightcon/timing_controller/
--rw-rw-rw-   0        0        0      172 2023-06-27 11:52:52.000000 lightcon-1.4.2.post1/lightcon/timing_controller/__init__.py
--rw-rw-rw-   0        0        0     6326 2023-06-27 11:52:52.000000 lightcon-1.4.2.post1/lightcon/timing_controller/_timing_controller.py
--rw-rw-rw-   0        0        0     7234 2023-06-27 11:52:52.000000 lightcon-1.4.2.post1/lightcon/timing_controller/_timing_controller_v2.py
-drwxrwxrwx   0        0        0        0 2023-06-27 11:54:42.369257 lightcon-1.4.2.post1/lightcon/utils/
--rw-rw-rw-   0        0        0       50 2023-06-27 11:52:52.000000 lightcon-1.4.2.post1/lightcon/utils/__init__.py
--rw-rw-rw-   0        0        0      591 2023-06-27 11:52:52.000000 lightcon-1.4.2.post1/lightcon/utils/_fixes.py
-drwxrwxrwx   0        0        0        0 2023-06-27 11:54:42.369257 lightcon-1.4.2.post1/lightcon/wintopas/
--rw-rw-rw-   0        0        0       65 2023-06-27 11:52:52.000000 lightcon-1.4.2.post1/lightcon/wintopas/__init__.py
--rw-rw-rw-   0        0        0     1567 2023-06-27 11:52:52.000000 lightcon-1.4.2.post1/lightcon/wintopas/_wintopas.py
-drwxrwxrwx   0        0        0        0 2023-06-27 11:54:41.907724 lightcon-1.4.2.post1/lightcon.egg-info/
--rw-rw-rw-   0        0        0     6258 2023-06-27 11:54:41.000000 lightcon-1.4.2.post1/lightcon.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1894 2023-06-27 11:54:41.000000 lightcon-1.4.2.post1/lightcon.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-27 11:54:41.000000 lightcon-1.4.2.post1/lightcon.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       90 2023-06-27 11:54:41.000000 lightcon-1.4.2.post1/lightcon.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-27 11:54:41.000000 lightcon-1.4.2.post1/lightcon.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-27 11:54:42.369257 lightcon-1.4.2.post1/setup.cfg
--rw-rw-rw-   0        0        0     1745 2023-06-27 11:52:52.000000 lightcon-1.4.2.post1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-27 12:50:23.442321 lightcon-1.4.2.post2/
+-rw-rw-rw-   0        0        0     1082 2023-06-27 12:48:14.000000 lightcon-1.4.2.post2/LICENCE
+-rw-rw-rw-   0        0        0      317 2023-06-27 12:48:14.000000 lightcon-1.4.2.post2/MANIFEST.in
+-rw-rw-rw-   0        0        0     6258 2023-06-27 12:50:23.442321 lightcon-1.4.2.post2/PKG-INFO
+-rw-rw-rw-   0        0        0     5605 2023-06-27 12:48:14.000000 lightcon-1.4.2.post2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-27 12:50:23.411070 lightcon-1.4.2.post2/lightcon/
+-rw-rw-rw-   0        0        0        0 2023-06-27 12:48:14.000000 lightcon-1.4.2.post2/lightcon/__config__.py
+-rw-rw-rw-   0        0        0      717 2023-06-27 12:48:14.000000 lightcon-1.4.2.post2/lightcon/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-06-27 12:48:14.000000 lightcon-1.4.2.post2/lightcon/_globals.py
+drwxrwxrwx   0        0        0        0 2023-06-27 12:50:23.411070 lightcon-1.4.2.post2/lightcon/beam_alignment/
+-rw-rw-rw-   0        0        0       93 2023-06-27 12:48:14.000000 lightcon-1.4.2.post2/lightcon/beam_alignment/__init__.py
+-rw-rw-rw-   0        0        0     2105 2023-06-27 12:48:14.000000 lightcon-1.4.2.post2/lightcon/beam_alignment/_beam_alignment.py
+drwxrwxrwx   0        0        0        0 2023-06-27 12:50:23.411070 lightcon-1.4.2.post2/lightcon/calculate/
+-rw-rw-rw-   0        0        0      190 2023-06-27 12:48:14.000000 lightcon-1.4.2.post2/lightcon/calculate/__init__.py
+-rw-rw-rw-   0        0        0     2997 2023-06-27 12:48:14.000000 lightcon-1.4.2.post2/lightcon/calculate/_beam_profiling_gauss.py
+-rw-rw-rw-   0        0        0     3393 2023-06-27 12:48:14.000000 lightcon-1.4.2.post2/lightcon/calculate/_beam_profiling_iso.py
+-rw-rw-rw-   0        0        0     1407 2023-06-27 12:48:14.000000 lightcon-1.4.2.post2/lightcon/calculate/_calculate_motor_parameters.py
+drwxrwxrwx   0        0        0        0 2023-06-27 12:50:23.411070 lightcon-1.4.2.post2/lightcon/camera_app_client/
+-rw-rw-rw-   0        0        0       76 2023-06-27 12:48:14.000000 lightcon-1.4.2.post2/lightcon/camera_app_client/__init__.py
+-rw-rw-rw-   0        0        0     2965 2023-06-27 12:48:14.000000 lightcon-1.4.2.post2/lightcon/camera_app_client/_camera_app_client.py
+drwxrwxrwx   0        0        0        0 2023-06-27 12:50:23.411070 lightcon-1.4.2.post2/lightcon/common/
+-rw-rw-rw-   0        0        0      614 2023-06-27 12:48:14.000000 lightcon-1.4.2.post2/lightcon/common/__init__.py
+-rw-rw-rw-   0        0        0      931 2023-06-27 12:48:14.000000 lightcon-1.4.2.post2/lightcon/common/_converters.py
+-rw-rw-rw-   0        0        0     3155 2023-06-27 12:48:14.000000 lightcon-1.4.2.post2/lightcon/common/_http_methods.py
+-rw-rw-rw-   0        0        0     5607 2023-06-27 12:48:14.000000 lightcon-1.4.2.post2/lightcon/common/_leprecan_provider.py
+-rw-rw-rw-   0        0        0      336 2023-06-27 12:48:14.000000 lightcon-1.4.2.post2/lightcon/common/_load_motor_and_stage_parameters.py
+-rw-rw-rw-   0        0        0     1042 2023-06-27 12:48:14.000000 lightcon-1.4.2.post2/lightcon/common/_serial_tools.py
+-rw-rw-rw-   0        0        0     5151 2023-06-27 12:48:14.000000 lightcon-1.4.2.post2/lightcon/common/_udp_locator.py
+-rw-rw-rw-   0        0        0      506 2023-06-27 12:48:14.000000 lightcon-1.4.2.post2/lightcon/common/stage_parameters.py
+drwxrwxrwx   0        0        0        0 2023-06-27 12:50:23.411070 lightcon-1.4.2.post2/lightcon/datasets/
+-rw-rw-rw-   0        0        0      159 2023-06-27 12:48:14.000000 lightcon-1.4.2.post2/lightcon/datasets/__init__.py
+-rw-rw-rw-   0        0        0     3055 2023-06-27 12:48:14.000000 lightcon-1.4.2.post2/lightcon/datasets/_base.py
+drwxrwxrwx   0        0        0        0 2023-06-27 12:50:23.411070 lightcon-1.4.2.post2/lightcon/datasets/data/
+-rw-rw-rw-   0        0        0        0 2023-06-27 12:48:14.000000 lightcon-1.4.2.post2/lightcon/datasets/data/__init__.py
+-rw-rw-rw-   0        0        0    11968 2023-06-27 12:49:31.000000 lightcon-1.4.2.post2/lightcon/datasets/data/motor_parameters.json
+-rw-rw-rw-   0        0        0     4990 2023-06-27 12:49:31.000000 lightcon-1.4.2.post2/lightcon/datasets/data/stage_parameters.json
+drwxrwxrwx   0        0        0        0 2023-06-27 12:50:23.411070 lightcon-1.4.2.post2/lightcon/eth_motor_board/
+-rw-rw-rw-   0        0        0      204 2023-06-27 12:48:14.000000 lightcon-1.4.2.post2/lightcon/eth_motor_board/__init__.py
+-rw-rw-rw-   0        0        0    15177 2023-06-27 12:48:14.000000 lightcon-1.4.2.post2/lightcon/eth_motor_board/_eth_motor_board.py
+-rw-rw-rw-   0        0        0     1920 2023-06-27 12:48:14.000000 lightcon-1.4.2.post2/lightcon/eth_motor_board/_eth_motor_board_leprecan_provider.py
+drwxrwxrwx   0        0        0        0 2023-06-27 12:50:23.426696 lightcon-1.4.2.post2/lightcon/fast_daq/
+-rw-rw-rw-   0        0        0    70144 2023-06-27 12:48:14.000000 lightcon-1.4.2.post2/lightcon/fast_daq/FTD2XX_NET.dll
+-rw-rw-rw-   0        0        0    25088 2023-06-27 12:48:14.000000 lightcon-1.4.2.post2/lightcon/fast_daq/LightConversion.Abstractions.dll
+-rw-rw-rw-   0        0        0    23552 2023-06-27 12:48:14.000000 lightcon-1.4.2.post2/lightcon/fast_daq/LightConversion.Hardware.FastDaq.dll
+-rw-rw-rw-   0        0        0    29600 2023-06-27 12:48:14.000000 lightcon-1.4.2.post2/lightcon/fast_daq/System.Threading.dll
+-rw-rw-rw-   0        0        0      130 2023-06-27 12:48:14.000000 lightcon-1.4.2.post2/lightcon/fast_daq/__init__.py
+-rw-rw-rw-   0        0        0     5442 2023-06-27 12:48:14.000000 lightcon-1.4.2.post2/lightcon/fast_daq/_fast_daq.py
+drwxrwxrwx   0        0        0        0 2023-06-27 12:50:23.426696 lightcon-1.4.2.post2/lightcon/harpia/
+-rw-rw-rw-   0        0        0      237 2023-06-27 12:48:14.000000 lightcon-1.4.2.post2/lightcon/harpia/__init__.py
+-rw-rw-rw-   0        0        0    24803 2023-06-27 12:48:14.000000 lightcon-1.4.2.post2/lightcon/harpia/_harpia.py
+-rw-rw-rw-   0        0        0     2222 2023-06-27 12:48:14.000000 lightcon-1.4.2.post2/lightcon/harpia/_harpia_leprecan_provider.py
+-rw-rw-rw-   0        0        0     8813 2023-06-27 12:48:14.000000 lightcon-1.4.2.post2/lightcon/harpia/_harpia_model_decoder.py
+drwxrwxrwx   0        0        0        0 2023-06-27 12:50:23.426696 lightcon-1.4.2.post2/lightcon/harpia_daq/
+-rw-rw-rw-   0        0        0    70144 2023-06-27 12:48:14.000000 lightcon-1.4.2.post2/lightcon/harpia_daq/FTD2XX_NET.dll
+-rw-rw-rw-   0        0        0   108908 2023-06-27 12:48:14.000000 lightcon-1.4.2.post2/lightcon/harpia_daq/FTD2XX_NET.xml
+-rw-rw-rw-   0        0        0    17920 2023-06-27 12:48:14.000000 lightcon-1.4.2.post2/lightcon/harpia_daq/LightConversion.Abstractions.dll
+-rw-rw-rw-   0        0        0    26624 2023-06-27 12:48:14.000000 lightcon-1.4.2.post2/lightcon/harpia_daq/LightConversion.Hardware.HarpiaDaq.dll
+-rw-rw-rw-   0        0        0    18130 2023-06-27 12:48:14.000000 lightcon-1.4.2.post2/lightcon/harpia_daq/LightConversion.Hardware.HarpiaDaq.xml
+-rw-rw-rw-   0        0        0    29600 2023-06-27 12:48:14.000000 lightcon-1.4.2.post2/lightcon/harpia_daq/System.Threading.dll
+-rw-rw-rw-   0        0        0       84 2023-06-27 12:48:14.000000 lightcon-1.4.2.post2/lightcon/harpia_daq/__init__.py
+-rw-rw-rw-   0        0        0     5744 2023-06-27 12:48:14.000000 lightcon-1.4.2.post2/lightcon/harpia_daq/_harpia_daq.py
+drwxrwxrwx   0        0        0        0 2023-06-27 12:50:23.426696 lightcon-1.4.2.post2/lightcon/laser_clients/
+-rw-rw-rw-   0        0        0       91 2023-06-27 12:48:14.000000 lightcon-1.4.2.post2/lightcon/laser_clients/__init__.py
+-rw-rw-rw-   0        0        0     8634 2023-06-27 12:48:14.000000 lightcon-1.4.2.post2/lightcon/laser_clients/_laser_clients.py
+drwxrwxrwx   0        0        0        0 2023-06-27 12:50:23.426696 lightcon-1.4.2.post2/lightcon/style/
+-rw-rw-rw-   0        0        0      229 2023-06-27 12:48:14.000000 lightcon-1.4.2.post2/lightcon/style/__init__.py
+-rw-rw-rw-   0        0        0     7848 2023-06-27 12:48:14.000000 lightcon-1.4.2.post2/lightcon/style/_plotstyle_1d.py
+-rw-rw-rw-   0        0        0     7839 2023-06-27 12:48:14.000000 lightcon-1.4.2.post2/lightcon/style/plotstyle_1d.py
+drwxrwxrwx   0        0        0        0 2023-06-27 12:50:23.426696 lightcon-1.4.2.post2/lightcon/timing_controller/
+-rw-rw-rw-   0        0        0      172 2023-06-27 12:48:14.000000 lightcon-1.4.2.post2/lightcon/timing_controller/__init__.py
+-rw-rw-rw-   0        0        0     6326 2023-06-27 12:48:14.000000 lightcon-1.4.2.post2/lightcon/timing_controller/_timing_controller.py
+-rw-rw-rw-   0        0        0     7234 2023-06-27 12:48:14.000000 lightcon-1.4.2.post2/lightcon/timing_controller/_timing_controller_v2.py
+drwxrwxrwx   0        0        0        0 2023-06-27 12:50:23.426696 lightcon-1.4.2.post2/lightcon/utils/
+-rw-rw-rw-   0        0        0       50 2023-06-27 12:48:14.000000 lightcon-1.4.2.post2/lightcon/utils/__init__.py
+-rw-rw-rw-   0        0        0      591 2023-06-27 12:48:14.000000 lightcon-1.4.2.post2/lightcon/utils/_fixes.py
+drwxrwxrwx   0        0        0        0 2023-06-27 12:50:23.442321 lightcon-1.4.2.post2/lightcon/wintopas/
+-rw-rw-rw-   0        0        0       65 2023-06-27 12:48:14.000000 lightcon-1.4.2.post2/lightcon/wintopas/__init__.py
+-rw-rw-rw-   0        0        0     1567 2023-06-27 12:48:14.000000 lightcon-1.4.2.post2/lightcon/wintopas/_wintopas.py
+drwxrwxrwx   0        0        0        0 2023-06-27 12:50:23.411070 lightcon-1.4.2.post2/lightcon.egg-info/
+-rw-rw-rw-   0        0        0     6258 2023-06-27 12:50:23.000000 lightcon-1.4.2.post2/lightcon.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2354 2023-06-27 12:50:23.000000 lightcon-1.4.2.post2/lightcon.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-27 12:50:23.000000 lightcon-1.4.2.post2/lightcon.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       90 2023-06-27 12:50:23.000000 lightcon-1.4.2.post2/lightcon.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-27 12:50:23.000000 lightcon-1.4.2.post2/lightcon.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-27 12:50:23.442321 lightcon-1.4.2.post2/setup.cfg
+-rw-rw-rw-   0        0        0     1745 2023-06-27 12:48:14.000000 lightcon-1.4.2.post2/setup.py
```

### Comparing `lightcon-1.4.2.post1/LICENCE` & `lightcon-1.4.2.post2/LICENCE`

 * *Files identical despite different names*

### Comparing `lightcon-1.4.2.post1/PKG-INFO` & `lightcon-1.4.2.post2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lightcon
-Version: 1.4.2.post1
+Version: 1.4.2.post2
 Summary: A set of APIs to Light Conversion devices
 Home-page: https://bitbucket.org/harpiasoftware/light-conversion-apis.git
 Author: Vytautas Butkus
 Author-email: vytautas.butkus@lightcon.com
 Project-URL: Documentation, https://lightconupdater.blob.core.windows.net/documentation/lightcon/index.html
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `lightcon-1.4.2.post1/README.md` & `lightcon-1.4.2.post2/README.md`

 * *Files identical despite different names*

### Comparing `lightcon-1.4.2.post1/lightcon/__init__.py` & `lightcon-1.4.2.post2/lightcon/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "1.4.2-1"
+__version__ = "1.4.2-2"
 
 from . import wintopas
 from . import timing_controller
 from . import style
 from . import laser_clients
 from . import harpia
 from . import harpia_daq
```

### Comparing `lightcon-1.4.2.post1/lightcon/beam_alignment/_beam_alignment.py` & `lightcon-1.4.2.post2/lightcon/beam_alignment/_beam_alignment.py`

 * *Files identical despite different names*

### Comparing `lightcon-1.4.2.post1/lightcon/calculate/_beam_profiling_gauss.py` & `lightcon-1.4.2.post2/lightcon/calculate/_beam_profiling_gauss.py`

 * *Files identical despite different names*

### Comparing `lightcon-1.4.2.post1/lightcon/calculate/_beam_profiling_iso.py` & `lightcon-1.4.2.post2/lightcon/calculate/_beam_profiling_iso.py`

 * *Files identical despite different names*

### Comparing `lightcon-1.4.2.post1/lightcon/calculate/_calculate_motor_parameters.py` & `lightcon-1.4.2.post2/lightcon/calculate/_calculate_motor_parameters.py`

 * *Files identical despite different names*

### Comparing `lightcon-1.4.2.post1/lightcon/camera_app_client/_camera_app_client.py` & `lightcon-1.4.2.post2/lightcon/camera_app_client/_camera_app_client.py`

 * *Files identical despite different names*

### Comparing `lightcon-1.4.2.post1/lightcon/common/__init__.py` & `lightcon-1.4.2.post2/lightcon/common/__init__.py`

 * *Files identical despite different names*

### Comparing `lightcon-1.4.2.post1/lightcon/common/_converters.py` & `lightcon-1.4.2.post2/lightcon/common/_converters.py`

 * *Files identical despite different names*

### Comparing `lightcon-1.4.2.post1/lightcon/common/_http_methods.py` & `lightcon-1.4.2.post2/lightcon/common/_http_methods.py`

 * *Files identical despite different names*

### Comparing `lightcon-1.4.2.post1/lightcon/common/_leprecan_provider.py` & `lightcon-1.4.2.post2/lightcon/common/_leprecan_provider.py`

 * *Files identical despite different names*

### Comparing `lightcon-1.4.2.post1/lightcon/common/_serial_tools.py` & `lightcon-1.4.2.post2/lightcon/common/_serial_tools.py`

 * *Files identical despite different names*

### Comparing `lightcon-1.4.2.post1/lightcon/common/_udp_locator.py` & `lightcon-1.4.2.post2/lightcon/common/_udp_locator.py`

 * *Files identical despite different names*

### Comparing `lightcon-1.4.2.post1/lightcon/datasets/_base.py` & `lightcon-1.4.2.post2/lightcon/datasets/_base.py`

 * *Files identical despite different names*

### Comparing `lightcon-1.4.2.post1/lightcon/datasets/data/motor_parameters.json` & `lightcon-1.4.2.post2/lightcon/datasets/data/motor_parameters.json`

 * *Files identical despite different names*

### Comparing `lightcon-1.4.2.post1/lightcon/datasets/data/stage_parameters.json` & `lightcon-1.4.2.post2/lightcon/datasets/data/stage_parameters.json`

 * *Files identical despite different names*

### Comparing `lightcon-1.4.2.post1/lightcon/eth_motor_board/_eth_motor_board.py` & `lightcon-1.4.2.post2/lightcon/eth_motor_board/_eth_motor_board.py`

 * *Files identical despite different names*

### Comparing `lightcon-1.4.2.post1/lightcon/eth_motor_board/_eth_motor_board_leprecan_provider.py` & `lightcon-1.4.2.post2/lightcon/eth_motor_board/_eth_motor_board_leprecan_provider.py`

 * *Files identical despite different names*

### Comparing `lightcon-1.4.2.post1/lightcon/fast_daq/_fast_daq.py` & `lightcon-1.4.2.post2/lightcon/fast_daq/_fast_daq.py`

 * *Files identical despite different names*

### Comparing `lightcon-1.4.2.post1/lightcon/harpia/_harpia.py` & `lightcon-1.4.2.post2/lightcon/harpia/_harpia.py`

 * *Files identical despite different names*

### Comparing `lightcon-1.4.2.post1/lightcon/harpia/_harpia_leprecan_provider.py` & `lightcon-1.4.2.post2/lightcon/harpia/_harpia_leprecan_provider.py`

 * *Files identical despite different names*

### Comparing `lightcon-1.4.2.post1/lightcon/harpia/_harpia_model_decoder.py` & `lightcon-1.4.2.post2/lightcon/harpia/_harpia_model_decoder.py`

 * *Files identical despite different names*

### Comparing `lightcon-1.4.2.post1/lightcon/harpia_daq/_harpia_daq.py` & `lightcon-1.4.2.post2/lightcon/harpia_daq/_harpia_daq.py`

 * *Files identical despite different names*

### Comparing `lightcon-1.4.2.post1/lightcon/laser_clients/_laser_clients.py` & `lightcon-1.4.2.post2/lightcon/laser_clients/_laser_clients.py`

 * *Files identical despite different names*

### Comparing `lightcon-1.4.2.post1/lightcon/style/_plotstyle_1d.py` & `lightcon-1.4.2.post2/lightcon/style/_plotstyle_1d.py`

 * *Files identical despite different names*

### Comparing `lightcon-1.4.2.post1/lightcon/style/plotstyle_1d.py` & `lightcon-1.4.2.post2/lightcon/style/plotstyle_1d.py`

 * *Files identical despite different names*

### Comparing `lightcon-1.4.2.post1/lightcon/timing_controller/_timing_controller.py` & `lightcon-1.4.2.post2/lightcon/timing_controller/_timing_controller.py`

 * *Files identical despite different names*

### Comparing `lightcon-1.4.2.post1/lightcon/timing_controller/_timing_controller_v2.py` & `lightcon-1.4.2.post2/lightcon/timing_controller/_timing_controller_v2.py`

 * *Files identical despite different names*

### Comparing `lightcon-1.4.2.post1/lightcon/utils/_fixes.py` & `lightcon-1.4.2.post2/lightcon/utils/_fixes.py`

 * *Files identical despite different names*

### Comparing `lightcon-1.4.2.post1/lightcon/wintopas/_wintopas.py` & `lightcon-1.4.2.post2/lightcon/wintopas/_wintopas.py`

 * *Files identical despite different names*

### Comparing `lightcon-1.4.2.post1/lightcon.egg-info/PKG-INFO` & `lightcon-1.4.2.post2/lightcon.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lightcon
-Version: 1.4.2.post1
+Version: 1.4.2.post2
 Summary: A set of APIs to Light Conversion devices
 Home-page: https://bitbucket.org/harpiasoftware/light-conversion-apis.git
 Author: Vytautas Butkus
 Author-email: vytautas.butkus@lightcon.com
 Project-URL: Documentation, https://lightconupdater.blob.core.windows.net/documentation/lightcon/index.html
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `lightcon-1.4.2.post1/lightcon.egg-info/SOURCES.txt` & `lightcon-1.4.2.post2/lightcon.egg-info/SOURCES.txt`

 * *Files 23% similar despite different names*

```diff
@@ -30,20 +30,30 @@
 lightcon/datasets/_base.py
 lightcon/datasets/data/__init__.py
 lightcon/datasets/data/motor_parameters.json
 lightcon/datasets/data/stage_parameters.json
 lightcon/eth_motor_board/__init__.py
 lightcon/eth_motor_board/_eth_motor_board.py
 lightcon/eth_motor_board/_eth_motor_board_leprecan_provider.py
+lightcon/fast_daq/FTD2XX_NET.dll
+lightcon/fast_daq/LightConversion.Abstractions.dll
+lightcon/fast_daq/LightConversion.Hardware.FastDaq.dll
+lightcon/fast_daq/System.Threading.dll
 lightcon/fast_daq/__init__.py
 lightcon/fast_daq/_fast_daq.py
 lightcon/harpia/__init__.py
 lightcon/harpia/_harpia.py
 lightcon/harpia/_harpia_leprecan_provider.py
 lightcon/harpia/_harpia_model_decoder.py
+lightcon/harpia_daq/FTD2XX_NET.dll
+lightcon/harpia_daq/FTD2XX_NET.xml
+lightcon/harpia_daq/LightConversion.Abstractions.dll
+lightcon/harpia_daq/LightConversion.Hardware.HarpiaDaq.dll
+lightcon/harpia_daq/LightConversion.Hardware.HarpiaDaq.xml
+lightcon/harpia_daq/System.Threading.dll
 lightcon/harpia_daq/__init__.py
 lightcon/harpia_daq/_harpia_daq.py
 lightcon/laser_clients/__init__.py
 lightcon/laser_clients/_laser_clients.py
 lightcon/style/__init__.py
 lightcon/style/_plotstyle_1d.py
 lightcon/style/plotstyle_1d.py
```

### Comparing `lightcon-1.4.2.post1/setup.py` & `lightcon-1.4.2.post2/setup.py`

 * *Files identical despite different names*

