# Comparing `tmp/control-lab-ly-1.1.0b1.tar.gz` & `tmp/control-lab-ly-1.1.1a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "control-lab-ly-1.1.0b1.tar", last modified: Thu Jun 15 06:28:57 2023, max compression
+gzip compressed data, was "control-lab-ly-1.1.1a1.tar", last modified: Tue Jun 27 03:19:45 2023, max compression
```

## Comparing `control-lab-ly-1.1.0b1.tar` & `control-lab-ly-1.1.1a1.tar`

### file list

```diff
@@ -1,221 +1,204 @@
-drwxrwxrwx   0        0        0        0 2023-06-15 06:28:57.315276 control-lab-ly-1.1.0b1/
--rw-rw-rw-   0        0        0     1093 2023-02-24 13:59:16.000000 control-lab-ly-1.1.0b1/LICENSE.md
--rw-rw-rw-   0        0        0       44 2023-06-15 05:55:28.000000 control-lab-ly-1.1.0b1/MANIFEST.in
--rw-rw-rw-   0        0        0    20812 2023-06-15 06:28:57.315276 control-lab-ly-1.1.0b1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-15 06:28:55.633108 control-lab-ly-1.1.0b1/docs/
--rw-rw-rw-   0        0        0     6576 2023-06-15 05:47:20.000000 control-lab-ly-1.1.0b1/docs/CHANGELOG.md
--rw-rw-rw-   0        0        0     5356 2023-02-24 14:06:11.000000 control-lab-ly-1.1.0b1/docs/CODE_OF_CONDUCT.md
--rw-rw-rw-   0        0        0       33 2023-02-23 06:19:52.000000 control-lab-ly-1.1.0b1/docs/CONTRIBUTING.md
--rw-rw-rw-   0        0        0     1093 2023-02-24 13:59:16.000000 control-lab-ly-1.1.0b1/docs/LICENSE.md
--rw-rw-rw-   0        0        0    13118 2023-06-15 06:27:50.000000 control-lab-ly-1.1.0b1/docs/README.md
-drwxrwxrwx   0        0        0        0 2023-06-15 06:28:55.641155 control-lab-ly-1.1.0b1/docs/assets/
--rw-rw-rw-   0        0        0   203629 2023-06-15 02:22:15.000000 control-lab-ly-1.1.0b1/docs/assets/Documentation guide.png
--rw-rw-rw-   0        0        0      108 2023-02-23 06:19:52.000000 control-lab-ly-1.1.0b1/pyproject.toml
--rw-rw-rw-   0        0        0     1500 2023-06-15 06:28:57.324760 control-lab-ly-1.1.0b1/setup.cfg
--rw-rw-rw-   0        0        0       37 2023-03-10 02:02:34.000000 control-lab-ly-1.1.0b1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-15 06:28:55.235800 control-lab-ly-1.1.0b1/src/
-drwxrwxrwx   0        0        0        0 2023-06-15 06:28:55.676638 control-lab-ly-1.1.0b1/src/control_lab_ly.egg-info/
--rw-rw-rw-   0        0        0    20812 2023-06-15 06:28:54.000000 control-lab-ly-1.1.0b1/src/control_lab_ly.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     7587 2023-06-15 06:28:55.000000 control-lab-ly-1.1.0b1/src/control_lab_ly.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-15 06:28:54.000000 control-lab-ly-1.1.0b1/src/control_lab_ly.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      162 2023-06-15 06:28:54.000000 control-lab-ly-1.1.0b1/src/control_lab_ly.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-06-15 06:28:54.000000 control-lab-ly-1.1.0b1/src/control_lab_ly.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-15 06:28:55.684653 control-lab-ly-1.1.0b1/src/controllably/
-drwxrwxrwx   0        0        0        0 2023-06-15 06:28:55.710318 control-lab-ly-1.1.0b1/src/controllably/Compound/
-drwxrwxrwx   0        0        0        0 2023-06-15 06:28:55.728730 control-lab-ly-1.1.0b1/src/controllably/Compound/LiquidMover/
-drwxrwxrwx   0        0        0        0 2023-06-15 06:28:55.781362 control-lab-ly-1.1.0b1/src/controllably/Compound/LiquidMover/Opentrons/
--rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.1.0b1/src/controllably/Compound/LiquidMover/Opentrons/__init__.py
--rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.1.0b1/src/controllably/Compound/LiquidMover/Opentrons/opentrons_utils.py
--rw-rw-rw-   0        0        0      259 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0b1/src/controllably/Compound/LiquidMover/__init__.py
--rw-rw-rw-   0        0        0    17618 2023-06-07 08:08:37.000000 control-lab-ly-1.1.0b1/src/controllably/Compound/LiquidMover/liquidmover_utils.py
--rw-rw-rw-   0        0        0      241 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0b1/src/controllably/Compound/__init__.py
--rw-rw-rw-   0        0        0     8197 2023-06-07 15:06:53.000000 control-lab-ly-1.1.0b1/src/controllably/Compound/compound_utils.py
-drwxrwxrwx   0        0        0        0 2023-06-15 06:28:55.799953 control-lab-ly-1.1.0b1/src/controllably/Control/
-drwxrwxrwx   0        0        0        0 2023-06-15 06:28:55.903515 control-lab-ly-1.1.0b1/src/controllably/Control/GUI/
-drwxrwxrwx   0        0        0        0 2023-06-15 06:28:55.963518 control-lab-ly-1.1.0b1/src/controllably/Control/GUI/Basic/
--rw-rw-rw-   0        0        0      569 2023-06-07 07:31:49.000000 control-lab-ly-1.1.0b1/src/controllably/Control/GUI/Basic/__init__.py
--rw-rw-rw-   0        0        0     7129 2023-06-07 08:09:06.000000 control-lab-ly-1.1.0b1/src/controllably/Control/GUI/Basic/maker_panel.py
--rw-rw-rw-   0        0        0     7976 2023-06-09 02:26:55.000000 control-lab-ly-1.1.0b1/src/controllably/Control/GUI/Basic/measurer_panel.py
--rw-rw-rw-   0        0        0    16355 2023-06-09 02:26:45.000000 control-lab-ly-1.1.0b1/src/controllably/Control/GUI/Basic/mover_panel.py
--rw-rw-rw-   0        0        0     8767 2023-06-07 07:59:03.000000 control-lab-ly-1.1.0b1/src/controllably/Control/GUI/Basic/transfer_liquid_panel.py
--rw-rw-rw-   0        0        0     3780 2023-06-07 08:09:39.000000 control-lab-ly-1.1.0b1/src/controllably/Control/GUI/Basic/viewer_panel.py
-drwxrwxrwx   0        0        0        0 2023-06-15 06:28:56.009365 control-lab-ly-1.1.0b1/src/controllably/Control/GUI/Elements/
--rw-rw-rw-   0        0        0      406 2023-06-07 07:37:47.000000 control-lab-ly-1.1.0b1/src/controllably/Control/GUI/Elements/__init__.py
--rw-rw-rw-   0        0        0      888 2023-06-07 07:29:39.000000 control-lab-ly-1.1.0b1/src/controllably/Control/GUI/Elements/loader_panel.py
--rw-rw-rw-   0        0        0     8681 2023-06-07 15:28:23.000000 control-lab-ly-1.1.0b1/src/controllably/Control/GUI/Elements/pop_ups.py
--rw-rw-rw-   0        0        0     4573 2023-06-07 15:28:30.000000 control-lab-ly-1.1.0b1/src/controllably/Control/GUI/Elements/templates.py
--rw-rw-rw-   0        0        0      519 2023-06-07 15:50:08.000000 control-lab-ly-1.1.0b1/src/controllably/Control/GUI/__init__.py
--rw-rw-rw-   0        0        0    20954 2023-04-24 02:45:08.000000 control-lab-ly-1.1.0b1/src/controllably/Control/GUI/_guibuilder.py
--rw-rw-rw-   0        0        0     5544 2023-06-07 08:08:44.000000 control-lab-ly-1.1.0b1/src/controllably/Control/GUI/compound_panel.py
--rw-rw-rw-   0        0        0    16264 2023-06-07 08:08:56.000000 control-lab-ly-1.1.0b1/src/controllably/Control/GUI/gui_utils.py
--rw-rw-rw-   0        0        0    14530 2023-06-15 02:18:22.000000 control-lab-ly-1.1.0b1/src/controllably/Control/GUI/guide_panel.py
--rw-rw-rw-   0        0        0     3481 2023-06-07 07:35:28.000000 control-lab-ly-1.1.0b1/src/controllably/Control/GUI/multichannel_panel.py
--rw-rw-rw-   0        0        0        0 2023-06-05 18:40:54.000000 control-lab-ly-1.1.0b1/src/controllably/Control/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-15 06:28:56.025413 control-lab-ly-1.1.0b1/src/controllably/Make/
-drwxrwxrwx   0        0        0        0 2023-06-15 06:28:56.077219 control-lab-ly-1.1.0b1/src/controllably/Make/Heat/
--rw-rw-rw-   0        0        0      225 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0b1/src/controllably/Make/Heat/__init__.py
--rw-rw-rw-   0        0        0    11244 2023-06-07 08:09:49.000000 control-lab-ly-1.1.0b1/src/controllably/Make/Heat/peltier_utils.py
-drwxrwxrwx   0        0        0        0 2023-06-15 06:28:56.100685 control-lab-ly-1.1.0b1/src/controllably/Make/Light/
--rw-rw-rw-   0        0        0      218 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0b1/src/controllably/Make/Light/__init__.py
--rw-rw-rw-   0        0        0     9882 2023-06-07 08:09:54.000000 control-lab-ly-1.1.0b1/src/controllably/Make/Light/led_utils.py
-drwxrwxrwx   0        0        0        0 2023-06-15 06:28:56.108732 control-lab-ly-1.1.0b1/src/controllably/Make/Mixture/
-drwxrwxrwx   0        0        0        0 2023-06-15 06:28:56.134458 control-lab-ly-1.1.0b1/src/controllably/Make/Mixture/QInstruments/
--rw-rw-rw-   0        0        0      252 2023-05-25 07:11:07.000000 control-lab-ly-1.1.0b1/src/controllably/Make/Mixture/QInstruments/__init__.py
--rw-rw-rw-   0        0        0    27552 2023-06-05 10:20:45.000000 control-lab-ly-1.1.0b1/src/controllably/Make/Mixture/QInstruments/orbital_shaker_utils.py
-drwxrwxrwx   0        0        0        0 2023-06-15 06:28:56.166902 control-lab-ly-1.1.0b1/src/controllably/Make/Mixture/QInstruments/qinstruments_api/
--rw-rw-rw-   0        0        0      171 2023-05-25 07:11:07.000000 control-lab-ly-1.1.0b1/src/controllably/Make/Mixture/QInstruments/qinstruments_api/__init__.py
--rw-rw-rw-   0        0        0    37854 2023-06-05 10:20:45.000000 control-lab-ly-1.1.0b1/src/controllably/Make/Mixture/QInstruments/qinstruments_api/qinstruments_api.py
--rw-rw-rw-   0        0        0     4984 2023-05-25 07:11:07.000000 control-lab-ly-1.1.0b1/src/controllably/Make/Mixture/QInstruments/qinstruments_api/qinstruments_lib.py
--rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.1.0b1/src/controllably/Make/Mixture/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-15 06:28:56.188087 control-lab-ly-1.1.0b1/src/controllably/Make/ThinFilm/
--rw-rw-rw-   0        0        0      268 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0b1/src/controllably/Make/ThinFilm/__init__.py
--rw-rw-rw-   0        0        0    10777 2023-06-07 08:10:11.000000 control-lab-ly-1.1.0b1/src/controllably/Make/ThinFilm/spinner_utils.py
--rw-rw-rw-   0        0        0      217 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0b1/src/controllably/Make/__init__.py
--rw-rw-rw-   0        0        0     4220 2023-06-05 10:20:45.000000 control-lab-ly-1.1.0b1/src/controllably/Make/make_utils.py
-drwxrwxrwx   0        0        0        0 2023-06-15 06:28:56.232611 control-lab-ly-1.1.0b1/src/controllably/Measure/
-drwxrwxrwx   0        0        0        0 2023-06-15 06:28:56.248032 control-lab-ly-1.1.0b1/src/controllably/Measure/Electrical/
-drwxrwxrwx   0        0        0        0 2023-06-15 06:28:56.312523 control-lab-ly-1.1.0b1/src/controllably/Measure/Electrical/Keithley/
--rw-rw-rw-   0        0        0      314 2023-05-25 07:11:07.000000 control-lab-ly-1.1.0b1/src/controllably/Measure/Electrical/Keithley/__init__.py
--rw-rw-rw-   0        0        0    18010 2023-06-07 08:10:41.000000 control-lab-ly-1.1.0b1/src/controllably/Measure/Electrical/Keithley/keithley_device.py
--rw-rw-rw-   0        0        0     7484 2023-06-07 08:10:49.000000 control-lab-ly-1.1.0b1/src/controllably/Measure/Electrical/Keithley/keithley_lib.py
--rw-rw-rw-   0        0        0     1993 2023-06-07 08:10:55.000000 control-lab-ly-1.1.0b1/src/controllably/Measure/Electrical/Keithley/keithley_utils.py
-drwxrwxrwx   0        0        0        0 2023-06-15 06:28:56.337117 control-lab-ly-1.1.0b1/src/controllably/Measure/Electrical/Keithley/programs/
--rw-rw-rw-   0        0        0      287 2023-05-25 07:11:07.000000 control-lab-ly-1.1.0b1/src/controllably/Measure/Electrical/Keithley/programs/__init__.py
--rw-rw-rw-   0        0        0    10637 2023-06-07 15:30:15.000000 control-lab-ly-1.1.0b1/src/controllably/Measure/Electrical/Keithley/programs/base_programs.py
--rw-rw-rw-   0        0        0        0 2023-04-11 09:18:51.000000 control-lab-ly-1.1.0b1/src/controllably/Measure/Electrical/__init__.py
--rw-rw-rw-   0        0        0      298 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0b1/src/controllably/Measure/Electrical/electrical_utils.py
-drwxrwxrwx   0        0        0        0 2023-06-15 06:28:56.354994 control-lab-ly-1.1.0b1/src/controllably/Measure/Mechanical/
-drwxrwxrwx   0        0        0        0 2023-06-15 06:28:56.394443 control-lab-ly-1.1.0b1/src/controllably/Measure/Mechanical/PiezoRobotics/
--rw-rw-rw-   0        0        0      334 2023-05-18 08:27:22.000000 control-lab-ly-1.1.0b1/src/controllably/Measure/Mechanical/PiezoRobotics/__init__.py
--rw-rw-rw-   0        0        0    10341 2023-06-07 08:11:13.000000 control-lab-ly-1.1.0b1/src/controllably/Measure/Mechanical/PiezoRobotics/piezorobotics_device.py
--rw-rw-rw-   0        0        0     3159 2023-06-07 08:11:18.000000 control-lab-ly-1.1.0b1/src/controllably/Measure/Mechanical/PiezoRobotics/piezorobotics_lib.py
--rw-rw-rw-   0        0        0     2012 2023-06-07 08:11:22.000000 control-lab-ly-1.1.0b1/src/controllably/Measure/Mechanical/PiezoRobotics/piezorobotics_utils.py
-drwxrwxrwx   0        0        0        0 2023-06-15 06:28:56.410444 control-lab-ly-1.1.0b1/src/controllably/Measure/Mechanical/PiezoRobotics/programs/
--rw-rw-rw-   0        0        0      236 2023-05-25 07:11:07.000000 control-lab-ly-1.1.0b1/src/controllably/Measure/Mechanical/PiezoRobotics/programs/__init__.py
--rw-rw-rw-   0        0        0     3534 2023-06-07 08:11:26.000000 control-lab-ly-1.1.0b1/src/controllably/Measure/Mechanical/PiezoRobotics/programs/base_programs.py
--rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.1.0b1/src/controllably/Measure/Mechanical/__init__.py
--rw-rw-rw-   0        0        0      298 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0b1/src/controllably/Measure/Mechanical/mechanical_utils.py
-drwxrwxrwx   0        0        0        0 2023-06-15 06:28:56.451924 control-lab-ly-1.1.0b1/src/controllably/Measure/Physical/
--rw-rw-rw-   0        0        0      249 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0b1/src/controllably/Measure/Physical/__init__.py
--rw-rw-rw-   0        0        0     8358 2023-06-07 08:11:32.000000 control-lab-ly-1.1.0b1/src/controllably/Measure/Physical/balance_utils.py
--rw-rw-rw-   0        0        0     8199 2023-06-07 08:11:37.000000 control-lab-ly-1.1.0b1/src/controllably/Measure/Physical/force_sensor_utils.py
--rw-rw-rw-   0        0        0      535 2023-06-06 08:07:20.000000 control-lab-ly-1.1.0b1/src/controllably/Measure/__init__.py
--rw-rw-rw-   0        0        0     5437 2023-05-25 07:11:07.000000 control-lab-ly-1.1.0b1/src/controllably/Measure/instrument_utils.py
--rw-rw-rw-   0        0        0    14062 2023-05-25 07:11:07.000000 control-lab-ly-1.1.0b1/src/controllably/Measure/measure_utils.py
--rw-rw-rw-   0        0        0     4180 2023-06-07 08:10:29.000000 control-lab-ly-1.1.0b1/src/controllably/Measure/program_utils.py
-drwxrwxrwx   0        0        0        0 2023-06-15 06:28:56.478387 control-lab-ly-1.1.0b1/src/controllably/Move/
-drwxrwxrwx   0        0        0        0 2023-06-15 06:28:56.530473 control-lab-ly-1.1.0b1/src/controllably/Move/Cartesian/
--rw-rw-rw-   0        0        0      346 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0b1/src/controllably/Move/Cartesian/__init__.py
--rw-rw-rw-   0        0        0     9077 2023-05-25 07:11:07.000000 control-lab-ly-1.1.0b1/src/controllably/Move/Cartesian/cartesian_utils.py
--rw-rw-rw-   0        0        0     3450 2023-05-25 07:11:07.000000 control-lab-ly-1.1.0b1/src/controllably/Move/Cartesian/ender_utils.py
--rw-rw-rw-   0        0        0     2852 2023-06-06 07:14:55.000000 control-lab-ly-1.1.0b1/src/controllably/Move/Cartesian/primitiv_utils.py
-drwxrwxrwx   0        0        0        0 2023-06-15 06:28:56.550498 control-lab-ly-1.1.0b1/src/controllably/Move/Jointed/
-drwxrwxrwx   0        0        0        0 2023-06-15 06:28:56.576440 control-lab-ly-1.1.0b1/src/controllably/Move/Jointed/Dobot/
--rw-rw-rw-   0        0        0      336 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0b1/src/controllably/Move/Jointed/Dobot/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-15 06:28:56.592649 control-lab-ly-1.1.0b1/src/controllably/Move/Jointed/Dobot/dobot_api/
--rw-rw-rw-   0        0        0       62 2023-02-23 06:19:51.000000 control-lab-ly-1.1.0b1/src/controllably/Move/Jointed/Dobot/dobot_api/__init__.py
--rw-rw-rw-   0        0        0    24280 2023-05-25 07:11:07.000000 control-lab-ly-1.1.0b1/src/controllably/Move/Jointed/Dobot/dobot_api/dobot_api.py
--rw-rw-rw-   0        0        0    15776 2023-06-07 08:12:14.000000 control-lab-ly-1.1.0b1/src/controllably/Move/Jointed/Dobot/dobot_utils.py
--rw-rw-rw-   0        0        0     7128 2023-06-15 03:26:52.000000 control-lab-ly-1.1.0b1/src/controllably/Move/Jointed/Dobot/m1pro_utils.py
--rw-rw-rw-   0        0        0     4325 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0b1/src/controllably/Move/Jointed/Dobot/mg400_utils.py
--rw-rw-rw-   0        0        0      233 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0b1/src/controllably/Move/Jointed/__init__.py
--rw-rw-rw-   0        0        0    10566 2023-06-07 08:12:11.000000 control-lab-ly-1.1.0b1/src/controllably/Move/Jointed/jointed_utils.py
--rw-rw-rw-   0        0        0      217 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0b1/src/controllably/Move/__init__.py
--rw-rw-rw-   0        0        0    32385 2023-06-05 18:48:48.000000 control-lab-ly-1.1.0b1/src/controllably/Move/move_utils.py
-drwxrwxrwx   0        0        0        0 2023-06-15 06:28:56.613438 control-lab-ly-1.1.0b1/src/controllably/Transfer/
-drwxrwxrwx   0        0        0        0 2023-06-15 06:28:56.674765 control-lab-ly-1.1.0b1/src/controllably/Transfer/Liquid/
-drwxrwxrwx   0        0        0        0 2023-06-15 06:28:56.714528 control-lab-ly-1.1.0b1/src/controllably/Transfer/Liquid/Pumps/
-drwxrwxrwx   0        0        0        0 2023-06-15 06:28:56.762359 control-lab-ly-1.1.0b1/src/controllably/Transfer/Liquid/Pumps/TriContinent/
--rw-rw-rw-   0        0        0      255 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0b1/src/controllably/Transfer/Liquid/Pumps/TriContinent/__init__.py
--rw-rw-rw-   0        0        0     3440 2023-05-25 07:11:07.000000 control-lab-ly-1.1.0b1/src/controllably/Transfer/Liquid/Pumps/TriContinent/tricontinent_lib.py
--rw-rw-rw-   0        0        0    29858 2023-06-07 08:12:55.000000 control-lab-ly-1.1.0b1/src/controllably/Transfer/Liquid/Pumps/TriContinent/tricontinent_utils.py
--rw-rw-rw-   0        0        0      332 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0b1/src/controllably/Transfer/Liquid/Pumps/__init__.py
--rw-rw-rw-   0        0        0     7672 2023-05-25 07:11:07.000000 control-lab-ly-1.1.0b1/src/controllably/Transfer/Liquid/Pumps/peristaltic_utils.py
--rw-rw-rw-   0        0        0     3097 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0b1/src/controllably/Transfer/Liquid/Pumps/pump_utils.py
-drwxrwxrwx   0        0        0        0 2023-06-15 06:28:56.782331 control-lab-ly-1.1.0b1/src/controllably/Transfer/Liquid/Sartorius/
--rw-rw-rw-   0        0        0      252 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0b1/src/controllably/Transfer/Liquid/Sartorius/__init__.py
--rw-rw-rw-   0        0        0     2792 2023-05-25 07:11:07.000000 control-lab-ly-1.1.0b1/src/controllably/Transfer/Liquid/Sartorius/sartorius_lib.py
--rw-rw-rw-   0        0        0    31695 2023-06-07 15:33:06.000000 control-lab-ly-1.1.0b1/src/controllably/Transfer/Liquid/Sartorius/sartorius_utils.py
--rw-rw-rw-   0        0        0      364 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0b1/src/controllably/Transfer/Liquid/__init__.py
--rw-rw-rw-   0        0        0    13230 2023-05-25 07:11:07.000000 control-lab-ly-1.1.0b1/src/controllably/Transfer/Liquid/liquid_utils.py
--rw-rw-rw-   0        0        0     3451 2023-04-21 08:27:57.000000 control-lab-ly-1.1.0b1/src/controllably/Transfer/Liquid/syringe_lib.py
--rw-rw-rw-   0        0        0    14600 2023-05-25 07:11:07.000000 control-lab-ly-1.1.0b1/src/controllably/Transfer/Liquid/syringe_utils.py
-drwxrwxrwx   0        0        0        0 2023-06-15 06:28:56.795317 control-lab-ly-1.1.0b1/src/controllably/Transfer/Powder/
--rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.1.0b1/src/controllably/Transfer/Powder/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-15 06:28:56.809214 control-lab-ly-1.1.0b1/src/controllably/Transfer/Substrate/
-drwxrwxrwx   0        0        0        0 2023-06-15 06:28:56.826776 control-lab-ly-1.1.0b1/src/controllably/Transfer/Substrate/Dobot/
--rw-rw-rw-   0        0        0      397 2023-06-07 02:20:21.000000 control-lab-ly-1.1.0b1/src/controllably/Transfer/Substrate/Dobot/__init__.py
--rw-rw-rw-   0        0        0     8844 2023-06-07 08:13:13.000000 control-lab-ly-1.1.0b1/src/controllably/Transfer/Substrate/Dobot/dobot_attachments.py
--rw-rw-rw-   0        0        0      238 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0b1/src/controllably/Transfer/Substrate/__init__.py
--rw-rw-rw-   0        0        0     1366 2023-05-25 07:11:07.000000 control-lab-ly-1.1.0b1/src/controllably/Transfer/Substrate/substrate_utils.py
--rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.1.0b1/src/controllably/Transfer/__init__.py
--rw-rw-rw-   0        0        0        0 2023-04-11 09:18:51.000000 control-lab-ly-1.1.0b1/src/controllably/Transfer/transfer_utils.py
-drwxrwxrwx   0        0        0        0 2023-06-15 06:28:56.904830 control-lab-ly-1.1.0b1/src/controllably/View/
-drwxrwxrwx   0        0        0        0 2023-06-15 06:28:56.926575 control-lab-ly-1.1.0b1/src/controllably/View/Classifiers/
--rw-rw-rw-   0        0        0      333 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0b1/src/controllably/View/Classifiers/__init__.py
--rw-rw-rw-   0        0        0     2584 2023-06-08 02:41:36.000000 control-lab-ly-1.1.0b1/src/controllably/View/Classifiers/classifier_utils.py
-drwxrwxrwx   0        0        0        0 2023-06-15 06:28:56.957284 control-lab-ly-1.1.0b1/src/controllably/View/Optical/
--rw-rw-rw-   0        0        0      219 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0b1/src/controllably/View/Optical/__init__.py
--rw-rw-rw-   0        0        0     3163 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0b1/src/controllably/View/Optical/optical_utils.py
-drwxrwxrwx   0        0        0        0 2023-06-15 06:28:56.974305 control-lab-ly-1.1.0b1/src/controllably/View/Optical/placeholders/
--rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.1.0b1/src/controllably/View/Optical/placeholders/__init__.py
--rw-rw-rw-   0        0        0    15567 2023-02-23 06:19:52.000000 control-lab-ly-1.1.0b1/src/controllably/View/Optical/placeholders/optical_camera.png
-drwxrwxrwx   0        0        0        0 2023-06-15 06:28:56.982357 control-lab-ly-1.1.0b1/src/controllably/View/Thermal/
-drwxrwxrwx   0        0        0        0 2023-06-15 06:28:56.992333 control-lab-ly-1.1.0b1/src/controllably/View/Thermal/Flir/
--rw-rw-rw-   0        0        0        0 2023-05-18 07:04:15.000000 control-lab-ly-1.1.0b1/src/controllably/View/Thermal/Flir/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-15 06:28:57.030189 control-lab-ly-1.1.0b1/src/controllably/View/Thermal/Flir/ax8/
--rw-rw-rw-   0        0        0       33 2023-02-23 06:19:52.000000 control-lab-ly-1.1.0b1/src/controllably/View/Thermal/Flir/ax8/__init__.py
--rw-rw-rw-   0        0        0    10147 2023-02-23 06:19:52.000000 control-lab-ly-1.1.0b1/src/controllably/View/Thermal/Flir/ax8/ax8.py
--rw-rw-rw-   0        0        0     3821 2023-02-23 06:19:52.000000 control-lab-ly-1.1.0b1/src/controllably/View/Thermal/Flir/ax8/ax8_camera_feed.py
--rw-rw-rw-   0        0        0      636 2023-02-23 06:19:52.000000 control-lab-ly-1.1.0b1/src/controllably/View/Thermal/Flir/ax8/ax8_modbus_regs.py
--rw-rw-rw-   0        0        0      819 2023-02-23 06:19:52.000000 control-lab-ly-1.1.0b1/src/controllably/View/Thermal/Flir/ax8/ax8_modbus_utils.py
--rw-rw-rw-   0        0        0      219 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0b1/src/controllably/View/Thermal/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-15 06:28:57.047742 control-lab-ly-1.1.0b1/src/controllably/View/Thermal/placeholders/
--rw-rw-rw-   0        0        0        0 2023-02-23 06:19:52.000000 control-lab-ly-1.1.0b1/src/controllably/View/Thermal/placeholders/__init__.py
--rw-rw-rw-   0        0        0   148660 2023-02-23 06:19:52.000000 control-lab-ly-1.1.0b1/src/controllably/View/Thermal/placeholders/infrared_camera.png
--rw-rw-rw-   0        0        0     2988 2023-05-25 07:11:07.000000 control-lab-ly-1.1.0b1/src/controllably/View/Thermal/thermal_utils.py
--rw-rw-rw-   0        0        0      304 2023-06-08 02:41:32.000000 control-lab-ly-1.1.0b1/src/controllably/View/__init__.py
--rw-rw-rw-   0        0        0    15703 2023-06-07 14:50:19.000000 control-lab-ly-1.1.0b1/src/controllably/View/image.py
--rw-rw-rw-   0        0        0    15898 2023-06-08 02:41:35.000000 control-lab-ly-1.1.0b1/src/controllably/View/view_utils.py
--rw-rw-rw-   0        0        0      131 2023-06-05 18:11:26.000000 control-lab-ly-1.1.0b1/src/controllably/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-15 06:28:57.106130 control-lab-ly-1.1.0b1/src/controllably/misc/
--rw-rw-rw-   0        0        0      627 2023-06-07 15:16:27.000000 control-lab-ly-1.1.0b1/src/controllably/misc/__init__.py
--rw-rw-rw-   0        0        0     2522 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0b1/src/controllably/misc/decorators.py
--rw-rw-rw-   0        0        0     9596 2023-06-09 02:42:47.000000 control-lab-ly-1.1.0b1/src/controllably/misc/factory.py
--rw-rw-rw-   0        0        0     7940 2023-06-13 09:57:18.000000 control-lab-ly-1.1.0b1/src/controllably/misc/helper.py
--rw-rw-rw-   0        0        0    17547 2023-06-07 14:53:56.000000 control-lab-ly-1.1.0b1/src/controllably/misc/layout.py
--rw-rw-rw-   0        0        0     2863 2023-06-07 08:11:52.000000 control-lab-ly-1.1.0b1/src/controllably/misc/logger.py
--rw-rw-rw-   0        0        0     4543 2023-06-14 09:42:31.000000 control-lab-ly-1.1.0b1/src/controllably/misc/misc_utils.py
-drwxrwxrwx   0        0        0        0 2023-06-15 06:28:57.110310 control-lab-ly-1.1.0b1/src/controllably/misc/templates/
--rw-rw-rw-   0        0        0        0 2023-02-23 06:19:52.000000 control-lab-ly-1.1.0b1/src/controllably/misc/templates/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-15 06:28:57.133215 control-lab-ly-1.1.0b1/src/controllably/misc/templates/configs/
--rw-rw-rw-   0        0        0        0 2023-02-23 14:08:10.000000 control-lab-ly-1.1.0b1/src/controllably/misc/templates/configs/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-15 06:28:57.149724 control-lab-ly-1.1.0b1/src/controllably/misc/templates/configs/plugins/
--rw-rw-rw-   0        0        0        0 2023-04-11 09:18:51.000000 control-lab-ly-1.1.0b1/src/controllably/misc/templates/configs/plugins/__init__.py
--rw-rw-rw-   0        0        0     1091 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0b1/src/controllably/misc/templates/configs/plugins/plugin_template.py
--rw-rw-rw-   0        0        0      439 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0b1/src/controllably/misc/templates/configs/registry.yaml
-drwxrwxrwx   0        0        0        0 2023-06-15 06:28:57.178290 control-lab-ly-1.1.0b1/src/controllably/misc/templates/setup/
--rw-rw-rw-   0        0        0      772 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0b1/src/controllably/misc/templates/setup/__init__.py
--rw-rw-rw-   0        0        0     1434 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0b1/src/controllably/misc/templates/setup/config.yaml
--rw-rw-rw-   0        0        0      987 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0b1/src/controllably/misc/templates/setup/layout.json
-drwxrwxrwx   0        0        0        0 2023-06-15 06:28:57.312029 control-lab-ly-1.1.0b1/tests/
--rw-rw-rw-   0        0        0      197 2023-04-21 15:18:23.000000 control-lab-ly-1.1.0b1/tests/test_camera_optical.py
--rw-rw-rw-   0        0        0      230 2023-04-11 09:18:51.000000 control-lab-ly-1.1.0b1/tests/test_camera_thermal.py
--rw-rw-rw-   0        0        0      509 2023-04-11 09:18:51.000000 control-lab-ly-1.1.0b1/tests/test_cartesian_ender.py
--rw-rw-rw-   0        0        0      429 2023-04-11 09:18:51.000000 control-lab-ly-1.1.0b1/tests/test_cartesian_primitiv.py
--rw-rw-rw-   0        0        0      629 2023-05-04 14:05:17.000000 control-lab-ly-1.1.0b1/tests/test_compound_liquidmover.py
--rw-rw-rw-   0        0        0      801 2023-04-11 09:18:51.000000 control-lab-ly-1.1.0b1/tests/test_compound_spin_printer.py
--rw-rw-rw-   0        0        0      616 2023-04-11 09:18:51.000000 control-lab-ly-1.1.0b1/tests/test_dobot_m1pro.py
--rw-rw-rw-   0        0        0      651 2023-04-11 09:18:51.000000 control-lab-ly-1.1.0b1/tests/test_dobot_mg400.py
--rw-rw-rw-   0        0        0      324 2023-04-11 09:18:51.000000 control-lab-ly-1.1.0b1/tests/test_electrical_keithley.py
--rw-rw-rw-   0        0        0      392 2023-04-11 09:18:51.000000 control-lab-ly-1.1.0b1/tests/test_film_spin.py
--rw-rw-rw-   0        0        0      586 2023-05-25 07:11:07.000000 control-lab-ly-1.1.0b1/tests/test_heat_peltier.py
--rw-rw-rw-   0        0        0      349 2023-04-11 09:18:51.000000 control-lab-ly-1.1.0b1/tests/test_light_led_array.py
--rw-rw-rw-   0        0        0      390 2023-05-04 14:05:17.000000 control-lab-ly-1.1.0b1/tests/test_liquid_sartorius.py
--rw-rw-rw-   0        0        0      412 2023-04-11 09:18:51.000000 control-lab-ly-1.1.0b1/tests/test_liquid_syringe_assembly.py
--rw-rw-rw-   0        0        0      538 2023-05-04 09:11:29.000000 control-lab-ly-1.1.0b1/tests/test_liquid_tricontinent.py
--rw-rw-rw-   0        0        0      239 2023-04-11 09:18:51.000000 control-lab-ly-1.1.0b1/tests/test_mechanical_piezorobotics.py
--rw-rw-rw-   0        0        0     1011 2023-05-25 07:11:07.000000 control-lab-ly-1.1.0b1/tests/test_mixture_shaker.py
--rw-rw-rw-   0        0        0     2365 2023-06-15 02:45:10.000000 control-lab-ly-1.1.0b1/tests/test_panels.py
--rw-rw-rw-   0        0        0      273 2023-04-11 09:18:51.000000 control-lab-ly-1.1.0b1/tests/test_physical_balance.py
--rw-rw-rw-   0        0        0      337 2023-04-11 09:18:51.000000 control-lab-ly-1.1.0b1/tests/test_pump_peristaltic.py
+drwxrwxrwx   0        0        0        0 2023-06-27 03:19:45.700366 control-lab-ly-1.1.1a1/
+-rw-rw-rw-   0        0        0     1093 2023-02-24 13:59:16.000000 control-lab-ly-1.1.1a1/LICENSE.md
+-rw-rw-rw-   0        0        0       44 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a1/MANIFEST.in
+-rw-rw-rw-   0        0        0    20808 2023-06-27 03:19:45.701375 control-lab-ly-1.1.1a1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-27 03:19:44.811404 control-lab-ly-1.1.1a1/docs/
+-rw-rw-rw-   0        0        0     6576 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a1/docs/CHANGELOG.md
+-rw-rw-rw-   0        0        0     5356 2023-02-24 14:06:11.000000 control-lab-ly-1.1.1a1/docs/CODE_OF_CONDUCT.md
+-rw-rw-rw-   0        0        0       33 2023-02-23 06:19:52.000000 control-lab-ly-1.1.1a1/docs/CONTRIBUTING.md
+-rw-rw-rw-   0        0        0     1093 2023-02-24 13:59:16.000000 control-lab-ly-1.1.1a1/docs/LICENSE.md
+-rw-rw-rw-   0        0        0    13114 2023-06-15 07:16:26.000000 control-lab-ly-1.1.1a1/docs/README.md
+drwxrwxrwx   0        0        0        0 2023-06-27 03:19:44.815913 control-lab-ly-1.1.1a1/docs/assets/
+-rw-rw-rw-   0        0        0   203629 2023-06-15 06:52:40.000000 control-lab-ly-1.1.1a1/docs/assets/Documentation guide.png
+-rw-rw-rw-   0        0        0      108 2023-02-23 06:19:52.000000 control-lab-ly-1.1.1a1/pyproject.toml
+-rw-rw-rw-   0        0        0     1500 2023-06-27 03:19:45.702909 control-lab-ly-1.1.1a1/setup.cfg
+-rw-rw-rw-   0        0        0       37 2023-03-10 02:02:34.000000 control-lab-ly-1.1.1a1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-27 03:19:44.638387 control-lab-ly-1.1.1a1/src/
+drwxrwxrwx   0        0        0        0 2023-06-27 03:19:44.834325 control-lab-ly-1.1.1a1/src/control_lab_ly.egg-info/
+-rw-rw-rw-   0        0        0    20808 2023-06-27 03:19:44.000000 control-lab-ly-1.1.1a1/src/control_lab_ly.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     7087 2023-06-27 03:19:44.000000 control-lab-ly-1.1.1a1/src/control_lab_ly.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-27 03:19:44.000000 control-lab-ly-1.1.1a1/src/control_lab_ly.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      162 2023-06-27 03:19:44.000000 control-lab-ly-1.1.1a1/src/control_lab_ly.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-06-27 03:19:44.000000 control-lab-ly-1.1.1a1/src/control_lab_ly.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-27 03:19:44.839214 control-lab-ly-1.1.1a1/src/controllably/
+drwxrwxrwx   0        0        0        0 2023-06-27 03:19:44.848094 control-lab-ly-1.1.1a1/src/controllably/Compound/
+drwxrwxrwx   0        0        0        0 2023-06-27 03:19:44.855579 control-lab-ly-1.1.1a1/src/controllably/Compound/LiquidMover/
+drwxrwxrwx   0        0        0        0 2023-06-27 03:19:44.866374 control-lab-ly-1.1.1a1/src/controllably/Compound/LiquidMover/Opentrons/
+-rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.1.1a1/src/controllably/Compound/LiquidMover/Opentrons/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.1.1a1/src/controllably/Compound/LiquidMover/Opentrons/opentrons_utils.py
+-rw-rw-rw-   0        0        0      259 2023-04-12 15:51:49.000000 control-lab-ly-1.1.1a1/src/controllably/Compound/LiquidMover/__init__.py
+-rw-rw-rw-   0        0        0    17618 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a1/src/controllably/Compound/LiquidMover/liquidmover_utils.py
+-rw-rw-rw-   0        0        0      241 2023-04-12 15:51:49.000000 control-lab-ly-1.1.1a1/src/controllably/Compound/__init__.py
+-rw-rw-rw-   0        0        0     8197 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a1/src/controllably/Compound/compound_utils.py
+drwxrwxrwx   0        0        0        0 2023-06-27 03:19:44.910249 control-lab-ly-1.1.1a1/src/controllably/Control/
+drwxrwxrwx   0        0        0        0 2023-06-27 03:19:44.930520 control-lab-ly-1.1.1a1/src/controllably/Control/GUI/
+drwxrwxrwx   0        0        0        0 2023-06-27 03:19:44.970517 control-lab-ly-1.1.1a1/src/controllably/Control/GUI/Basic/
+-rw-rw-rw-   0        0        0      569 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a1/src/controllably/Control/GUI/Basic/__init__.py
+-rw-rw-rw-   0        0        0     7129 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a1/src/controllably/Control/GUI/Basic/maker_panel.py
+-rw-rw-rw-   0        0        0     7976 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a1/src/controllably/Control/GUI/Basic/measurer_panel.py
+-rw-rw-rw-   0        0        0    16416 2023-06-23 06:16:42.000000 control-lab-ly-1.1.1a1/src/controllably/Control/GUI/Basic/mover_panel.py
+-rw-rw-rw-   0        0        0     8767 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a1/src/controllably/Control/GUI/Basic/transfer_liquid_panel.py
+-rw-rw-rw-   0        0        0     3780 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a1/src/controllably/Control/GUI/Basic/viewer_panel.py
+drwxrwxrwx   0        0        0        0 2023-06-27 03:19:45.004680 control-lab-ly-1.1.1a1/src/controllably/Control/GUI/Elements/
+-rw-rw-rw-   0        0        0      406 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a1/src/controllably/Control/GUI/Elements/__init__.py
+-rw-rw-rw-   0        0        0      888 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a1/src/controllably/Control/GUI/Elements/loader_panel.py
+-rw-rw-rw-   0        0        0     8681 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a1/src/controllably/Control/GUI/Elements/pop_ups.py
+-rw-rw-rw-   0        0        0     4573 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a1/src/controllably/Control/GUI/Elements/templates.py
+-rw-rw-rw-   0        0        0      519 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a1/src/controllably/Control/GUI/__init__.py
+-rw-rw-rw-   0        0        0    20954 2023-04-24 02:45:08.000000 control-lab-ly-1.1.1a1/src/controllably/Control/GUI/_guibuilder.py
+-rw-rw-rw-   0        0        0     5544 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a1/src/controllably/Control/GUI/compound_panel.py
+-rw-rw-rw-   0        0        0    16264 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a1/src/controllably/Control/GUI/gui_utils.py
+-rw-rw-rw-   0        0        0    14530 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a1/src/controllably/Control/GUI/guide_panel.py
+-rw-rw-rw-   0        0        0     3481 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a1/src/controllably/Control/GUI/multichannel_panel.py
+-rw-rw-rw-   0        0        0        0 2023-06-05 18:40:54.000000 control-lab-ly-1.1.1a1/src/controllably/Control/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-27 03:19:45.030170 control-lab-ly-1.1.1a1/src/controllably/Make/
+drwxrwxrwx   0        0        0        0 2023-06-27 03:19:45.053481 control-lab-ly-1.1.1a1/src/controllably/Make/Heat/
+-rw-rw-rw-   0        0        0      225 2023-04-12 15:51:49.000000 control-lab-ly-1.1.1a1/src/controllably/Make/Heat/__init__.py
+-rw-rw-rw-   0        0        0    11192 2023-06-27 03:00:08.000000 control-lab-ly-1.1.1a1/src/controllably/Make/Heat/peltier_utils.py
+drwxrwxrwx   0        0        0        0 2023-06-27 03:19:45.068444 control-lab-ly-1.1.1a1/src/controllably/Make/Light/
+-rw-rw-rw-   0        0        0      218 2023-04-12 15:51:49.000000 control-lab-ly-1.1.1a1/src/controllably/Make/Light/__init__.py
+-rw-rw-rw-   0        0        0     9890 2023-06-21 10:05:07.000000 control-lab-ly-1.1.1a1/src/controllably/Make/Light/led_utils.py
+drwxrwxrwx   0        0        0        0 2023-06-27 03:19:45.073761 control-lab-ly-1.1.1a1/src/controllably/Make/Mixture/
+drwxrwxrwx   0        0        0        0 2023-06-27 03:19:45.105185 control-lab-ly-1.1.1a1/src/controllably/Make/Mixture/QInstruments/
+-rw-rw-rw-   0        0        0      252 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a1/src/controllably/Make/Mixture/QInstruments/__init__.py
+-rw-rw-rw-   0        0        0    27504 2023-06-27 03:00:08.000000 control-lab-ly-1.1.1a1/src/controllably/Make/Mixture/QInstruments/orbital_shaker_utils.py
+drwxrwxrwx   0        0        0        0 2023-06-27 03:19:45.139238 control-lab-ly-1.1.1a1/src/controllably/Make/Mixture/QInstruments/qinstruments_api/
+-rw-rw-rw-   0        0        0      171 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a1/src/controllably/Make/Mixture/QInstruments/qinstruments_api/__init__.py
+-rw-rw-rw-   0        0        0    37854 2023-06-27 03:00:08.000000 control-lab-ly-1.1.1a1/src/controllably/Make/Mixture/QInstruments/qinstruments_api/qinstruments_api.py
+-rw-rw-rw-   0        0        0     4984 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a1/src/controllably/Make/Mixture/QInstruments/qinstruments_api/qinstruments_lib.py
+-rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.1.1a1/src/controllably/Make/Mixture/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-27 03:19:45.162356 control-lab-ly-1.1.1a1/src/controllably/Make/ThinFilm/
+-rw-rw-rw-   0        0        0      268 2023-04-12 15:51:49.000000 control-lab-ly-1.1.1a1/src/controllably/Make/ThinFilm/__init__.py
+-rw-rw-rw-   0        0        0    10875 2023-06-27 03:00:08.000000 control-lab-ly-1.1.1a1/src/controllably/Make/ThinFilm/spinner_utils.py
+-rw-rw-rw-   0        0        0      217 2023-04-12 15:51:49.000000 control-lab-ly-1.1.1a1/src/controllably/Make/__init__.py
+-rw-rw-rw-   0        0        0     4220 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a1/src/controllably/Make/make_utils.py
+drwxrwxrwx   0        0        0        0 2023-06-27 03:19:45.187936 control-lab-ly-1.1.1a1/src/controllably/Measure/
+drwxrwxrwx   0        0        0        0 2023-06-27 03:19:45.204619 control-lab-ly-1.1.1a1/src/controllably/Measure/Electrical/
+drwxrwxrwx   0        0        0        0 2023-06-27 03:19:45.233919 control-lab-ly-1.1.1a1/src/controllably/Measure/Electrical/Keithley/
+-rw-rw-rw-   0        0        0      359 2023-06-27 03:00:08.000000 control-lab-ly-1.1.1a1/src/controllably/Measure/Electrical/Keithley/__init__.py
+-rw-rw-rw-   0        0        0    18010 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a1/src/controllably/Measure/Electrical/Keithley/keithley_device.py
+-rw-rw-rw-   0        0        0     7484 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a1/src/controllably/Measure/Electrical/Keithley/keithley_lib.py
+-rw-rw-rw-   0        0        0     1993 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a1/src/controllably/Measure/Electrical/Keithley/keithley_utils.py
+drwxrwxrwx   0        0        0        0 2023-06-27 03:19:45.253997 control-lab-ly-1.1.1a1/src/controllably/Measure/Electrical/Keithley/programs/
+-rw-rw-rw-   0        0        0      287 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a1/src/controllably/Measure/Electrical/Keithley/programs/__init__.py
+-rw-rw-rw-   0        0        0    10637 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a1/src/controllably/Measure/Electrical/Keithley/programs/base_programs.py
+-rw-rw-rw-   0        0        0        0 2023-04-11 09:18:51.000000 control-lab-ly-1.1.1a1/src/controllably/Measure/Electrical/__init__.py
+-rw-rw-rw-   0        0        0      298 2023-04-12 15:51:49.000000 control-lab-ly-1.1.1a1/src/controllably/Measure/Electrical/electrical_utils.py
+drwxrwxrwx   0        0        0        0 2023-06-27 03:19:45.265568 control-lab-ly-1.1.1a1/src/controllably/Measure/Mechanical/
+drwxrwxrwx   0        0        0        0 2023-06-27 03:19:45.287848 control-lab-ly-1.1.1a1/src/controllably/Measure/Mechanical/PiezoRobotics/
+-rw-rw-rw-   0        0        0      389 2023-06-27 03:00:08.000000 control-lab-ly-1.1.1a1/src/controllably/Measure/Mechanical/PiezoRobotics/__init__.py
+-rw-rw-rw-   0        0        0    10372 2023-06-27 03:00:08.000000 control-lab-ly-1.1.1a1/src/controllably/Measure/Mechanical/PiezoRobotics/piezorobotics_device.py
+-rw-rw-rw-   0        0        0     3159 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a1/src/controllably/Measure/Mechanical/PiezoRobotics/piezorobotics_lib.py
+-rw-rw-rw-   0        0        0     2012 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a1/src/controllably/Measure/Mechanical/PiezoRobotics/piezorobotics_utils.py
+drwxrwxrwx   0        0        0        0 2023-06-27 03:19:45.298379 control-lab-ly-1.1.1a1/src/controllably/Measure/Mechanical/PiezoRobotics/programs/
+-rw-rw-rw-   0        0        0      236 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a1/src/controllably/Measure/Mechanical/PiezoRobotics/programs/__init__.py
+-rw-rw-rw-   0        0        0     3542 2023-06-27 03:00:08.000000 control-lab-ly-1.1.1a1/src/controllably/Measure/Mechanical/PiezoRobotics/programs/base_programs.py
+-rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.1.1a1/src/controllably/Measure/Mechanical/__init__.py
+-rw-rw-rw-   0        0        0      298 2023-04-12 15:51:49.000000 control-lab-ly-1.1.1a1/src/controllably/Measure/Mechanical/mechanical_utils.py
+drwxrwxrwx   0        0        0        0 2023-06-27 03:19:45.318543 control-lab-ly-1.1.1a1/src/controllably/Measure/Physical/
+-rw-rw-rw-   0        0        0      249 2023-06-26 05:50:00.000000 control-lab-ly-1.1.1a1/src/controllably/Measure/Physical/__init__.py
+-rw-rw-rw-   0        0        0     8358 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a1/src/controllably/Measure/Physical/balance_utils.py
+-rw-rw-rw-   0        0        0     8199 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a1/src/controllably/Measure/Physical/force_sensor_utils.py
+-rw-rw-rw-   0        0        0      535 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a1/src/controllably/Measure/__init__.py
+-rw-rw-rw-   0        0        0     5437 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a1/src/controllably/Measure/instrument_utils.py
+-rw-rw-rw-   0        0        0    14473 2023-06-27 03:07:03.000000 control-lab-ly-1.1.1a1/src/controllably/Measure/measure_utils.py
+-rw-rw-rw-   0        0        0     4180 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a1/src/controllably/Measure/program_utils.py
+drwxrwxrwx   0        0        0        0 2023-06-27 03:19:45.334434 control-lab-ly-1.1.1a1/src/controllably/Move/
+drwxrwxrwx   0        0        0        0 2023-06-27 03:19:45.355224 control-lab-ly-1.1.1a1/src/controllably/Move/Cartesian/
+-rw-rw-rw-   0        0        0      346 2023-04-12 15:51:49.000000 control-lab-ly-1.1.1a1/src/controllably/Move/Cartesian/__init__.py
+-rw-rw-rw-   0        0        0     9407 2023-06-27 03:00:08.000000 control-lab-ly-1.1.1a1/src/controllably/Move/Cartesian/cartesian_utils.py
+-rw-rw-rw-   0        0        0     3450 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a1/src/controllably/Move/Cartesian/ender_utils.py
+-rw-rw-rw-   0        0        0     6355 2023-06-22 05:19:20.000000 control-lab-ly-1.1.1a1/src/controllably/Move/Cartesian/grbl_lib.py
+-rw-rw-rw-   0        0        0     4858 2023-06-27 03:00:08.000000 control-lab-ly-1.1.1a1/src/controllably/Move/Cartesian/primitiv_utils.py
+drwxrwxrwx   0        0        0        0 2023-06-27 03:19:45.367626 control-lab-ly-1.1.1a1/src/controllably/Move/Jointed/
+drwxrwxrwx   0        0        0        0 2023-06-27 03:19:45.382878 control-lab-ly-1.1.1a1/src/controllably/Move/Jointed/Dobot/
+-rw-rw-rw-   0        0        0      336 2023-04-12 15:51:49.000000 control-lab-ly-1.1.1a1/src/controllably/Move/Jointed/Dobot/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-27 03:19:45.388912 control-lab-ly-1.1.1a1/src/controllably/Move/Jointed/Dobot/dobot_api/
+-rw-rw-rw-   0        0        0       62 2023-02-23 06:19:51.000000 control-lab-ly-1.1.1a1/src/controllably/Move/Jointed/Dobot/dobot_api/__init__.py
+-rw-rw-rw-   0        0        0    24280 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a1/src/controllably/Move/Jointed/Dobot/dobot_api/dobot_api.py
+-rw-rw-rw-   0        0        0    15776 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a1/src/controllably/Move/Jointed/Dobot/dobot_utils.py
+-rw-rw-rw-   0        0        0     7128 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a1/src/controllably/Move/Jointed/Dobot/m1pro_utils.py
+-rw-rw-rw-   0        0        0     4325 2023-04-12 15:51:49.000000 control-lab-ly-1.1.1a1/src/controllably/Move/Jointed/Dobot/mg400_utils.py
+-rw-rw-rw-   0        0        0      233 2023-04-12 15:51:49.000000 control-lab-ly-1.1.1a1/src/controllably/Move/Jointed/__init__.py
+-rw-rw-rw-   0        0        0    10566 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a1/src/controllably/Move/Jointed/jointed_utils.py
+-rw-rw-rw-   0        0        0      217 2023-04-12 15:51:49.000000 control-lab-ly-1.1.1a1/src/controllably/Move/__init__.py
+-rw-rw-rw-   0        0        0    32385 2023-06-21 10:10:48.000000 control-lab-ly-1.1.1a1/src/controllably/Move/move_utils.py
+drwxrwxrwx   0        0        0        0 2023-06-27 03:19:45.401275 control-lab-ly-1.1.1a1/src/controllably/Transfer/
+drwxrwxrwx   0        0        0        0 2023-06-27 03:19:45.415877 control-lab-ly-1.1.1a1/src/controllably/Transfer/Liquid/
+drwxrwxrwx   0        0        0        0 2023-06-27 03:19:45.424834 control-lab-ly-1.1.1a1/src/controllably/Transfer/Liquid/Pumps/
+drwxrwxrwx   0        0        0        0 2023-06-27 03:19:45.439487 control-lab-ly-1.1.1a1/src/controllably/Transfer/Liquid/Pumps/TriContinent/
+-rw-rw-rw-   0        0        0      255 2023-04-12 15:51:49.000000 control-lab-ly-1.1.1a1/src/controllably/Transfer/Liquid/Pumps/TriContinent/__init__.py
+-rw-rw-rw-   0        0        0     3440 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a1/src/controllably/Transfer/Liquid/Pumps/TriContinent/tricontinent_lib.py
+-rw-rw-rw-   0        0        0    29858 2023-06-27 03:00:08.000000 control-lab-ly-1.1.1a1/src/controllably/Transfer/Liquid/Pumps/TriContinent/tricontinent_utils.py
+-rw-rw-rw-   0        0        0      332 2023-04-12 15:51:49.000000 control-lab-ly-1.1.1a1/src/controllably/Transfer/Liquid/Pumps/__init__.py
+-rw-rw-rw-   0        0        0     7672 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a1/src/controllably/Transfer/Liquid/Pumps/peristaltic_utils.py
+-rw-rw-rw-   0        0        0     3159 2023-06-27 03:00:08.000000 control-lab-ly-1.1.1a1/src/controllably/Transfer/Liquid/Pumps/pump_utils.py
+drwxrwxrwx   0        0        0        0 2023-06-27 03:19:45.453486 control-lab-ly-1.1.1a1/src/controllably/Transfer/Liquid/Sartorius/
+-rw-rw-rw-   0        0        0      252 2023-04-12 15:51:49.000000 control-lab-ly-1.1.1a1/src/controllably/Transfer/Liquid/Sartorius/__init__.py
+-rw-rw-rw-   0        0        0     2792 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a1/src/controllably/Transfer/Liquid/Sartorius/sartorius_lib.py
+-rw-rw-rw-   0        0        0    32163 2023-06-27 03:00:08.000000 control-lab-ly-1.1.1a1/src/controllably/Transfer/Liquid/Sartorius/sartorius_utils.py
+-rw-rw-rw-   0        0        0      364 2023-04-12 15:51:49.000000 control-lab-ly-1.1.1a1/src/controllably/Transfer/Liquid/__init__.py
+-rw-rw-rw-   0        0        0    13230 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a1/src/controllably/Transfer/Liquid/liquid_utils.py
+-rw-rw-rw-   0        0        0     3451 2023-04-21 08:27:57.000000 control-lab-ly-1.1.1a1/src/controllably/Transfer/Liquid/syringe_lib.py
+-rw-rw-rw-   0        0        0    14600 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a1/src/controllably/Transfer/Liquid/syringe_utils.py
+drwxrwxrwx   0        0        0        0 2023-06-27 03:19:45.464023 control-lab-ly-1.1.1a1/src/controllably/Transfer/Powder/
+-rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.1.1a1/src/controllably/Transfer/Powder/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-27 03:19:45.469661 control-lab-ly-1.1.1a1/src/controllably/Transfer/Substrate/
+drwxrwxrwx   0        0        0        0 2023-06-27 03:19:45.482708 control-lab-ly-1.1.1a1/src/controllably/Transfer/Substrate/Dobot/
+-rw-rw-rw-   0        0        0      397 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a1/src/controllably/Transfer/Substrate/Dobot/__init__.py
+-rw-rw-rw-   0        0        0     8844 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a1/src/controllably/Transfer/Substrate/Dobot/dobot_attachments.py
+-rw-rw-rw-   0        0        0      238 2023-04-12 15:51:49.000000 control-lab-ly-1.1.1a1/src/controllably/Transfer/Substrate/__init__.py
+-rw-rw-rw-   0        0        0     1366 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a1/src/controllably/Transfer/Substrate/substrate_utils.py
+-rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.1.1a1/src/controllably/Transfer/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-04-11 09:18:51.000000 control-lab-ly-1.1.1a1/src/controllably/Transfer/transfer_utils.py
+drwxrwxrwx   0        0        0        0 2023-06-27 03:19:45.497957 control-lab-ly-1.1.1a1/src/controllably/View/
+drwxrwxrwx   0        0        0        0 2023-06-27 03:19:45.504957 control-lab-ly-1.1.1a1/src/controllably/View/Classifiers/
+-rw-rw-rw-   0        0        0      333 2023-04-12 15:51:49.000000 control-lab-ly-1.1.1a1/src/controllably/View/Classifiers/__init__.py
+-rw-rw-rw-   0        0        0     2584 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a1/src/controllably/View/Classifiers/classifier_utils.py
+drwxrwxrwx   0        0        0        0 2023-06-27 03:19:45.516813 control-lab-ly-1.1.1a1/src/controllably/View/Optical/
+-rw-rw-rw-   0        0        0      219 2023-04-12 15:51:49.000000 control-lab-ly-1.1.1a1/src/controllably/View/Optical/__init__.py
+-rw-rw-rw-   0        0        0     3163 2023-04-12 15:51:49.000000 control-lab-ly-1.1.1a1/src/controllably/View/Optical/optical_utils.py
+drwxrwxrwx   0        0        0        0 2023-06-27 03:19:45.528814 control-lab-ly-1.1.1a1/src/controllably/View/Optical/placeholders/
+-rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.1.1a1/src/controllably/View/Optical/placeholders/__init__.py
+-rw-rw-rw-   0        0        0    15567 2023-02-23 06:19:52.000000 control-lab-ly-1.1.1a1/src/controllably/View/Optical/placeholders/optical_camera.png
+drwxrwxrwx   0        0        0        0 2023-06-27 03:19:45.538781 control-lab-ly-1.1.1a1/src/controllably/View/Thermal/
+drwxrwxrwx   0        0        0        0 2023-06-27 03:19:45.550728 control-lab-ly-1.1.1a1/src/controllably/View/Thermal/Flir/
+-rw-rw-rw-   0        0        0        0 2023-05-18 07:04:15.000000 control-lab-ly-1.1.1a1/src/controllably/View/Thermal/Flir/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-27 03:19:45.574636 control-lab-ly-1.1.1a1/src/controllably/View/Thermal/Flir/ax8/
+-rw-rw-rw-   0        0        0       33 2023-02-23 06:19:52.000000 control-lab-ly-1.1.1a1/src/controllably/View/Thermal/Flir/ax8/__init__.py
+-rw-rw-rw-   0        0        0    10147 2023-06-22 09:26:34.000000 control-lab-ly-1.1.1a1/src/controllably/View/Thermal/Flir/ax8/ax8.py
+-rw-rw-rw-   0        0        0     3821 2023-02-23 06:19:52.000000 control-lab-ly-1.1.1a1/src/controllably/View/Thermal/Flir/ax8/ax8_camera_feed.py
+-rw-rw-rw-   0        0        0      636 2023-02-23 06:19:52.000000 control-lab-ly-1.1.1a1/src/controllably/View/Thermal/Flir/ax8/ax8_modbus_regs.py
+-rw-rw-rw-   0        0        0      819 2023-02-23 06:19:52.000000 control-lab-ly-1.1.1a1/src/controllably/View/Thermal/Flir/ax8/ax8_modbus_utils.py
+-rw-rw-rw-   0        0        0     1836 2023-06-27 03:00:08.000000 control-lab-ly-1.1.1a1/src/controllably/View/Thermal/Flir/ax8_utils.py
+-rw-rw-rw-   0        0        0      219 2023-04-12 15:51:49.000000 control-lab-ly-1.1.1a1/src/controllably/View/Thermal/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-27 03:19:45.588936 control-lab-ly-1.1.1a1/src/controllably/View/Thermal/placeholders/
+-rw-rw-rw-   0        0        0        0 2023-02-23 06:19:52.000000 control-lab-ly-1.1.1a1/src/controllably/View/Thermal/placeholders/__init__.py
+-rw-rw-rw-   0        0        0   148660 2023-02-23 06:19:52.000000 control-lab-ly-1.1.1a1/src/controllably/View/Thermal/placeholders/infrared_camera.png
+-rw-rw-rw-   0        0        0     2988 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a1/src/controllably/View/Thermal/thermal_utils.py
+-rw-rw-rw-   0        0        0      304 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a1/src/controllably/View/__init__.py
+-rw-rw-rw-   0        0        0    15703 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a1/src/controllably/View/image.py
+-rw-rw-rw-   0        0        0    15898 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a1/src/controllably/View/view_utils.py
+-rw-rw-rw-   0        0        0      131 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a1/src/controllably/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-27 03:19:45.633386 control-lab-ly-1.1.1a1/src/controllably/misc/
+-rw-rw-rw-   0        0        0      627 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a1/src/controllably/misc/__init__.py
+-rw-rw-rw-   0        0        0     2522 2023-04-12 15:51:49.000000 control-lab-ly-1.1.1a1/src/controllably/misc/decorators.py
+-rw-rw-rw-   0        0        0     9596 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a1/src/controllably/misc/factory.py
+-rw-rw-rw-   0        0        0     7940 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a1/src/controllably/misc/helper.py
+-rw-rw-rw-   0        0        0    17547 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a1/src/controllably/misc/layout.py
+-rw-rw-rw-   0        0        0     2863 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a1/src/controllably/misc/logger.py
+-rw-rw-rw-   0        0        0     4543 2023-06-15 06:52:39.000000 control-lab-ly-1.1.1a1/src/controllably/misc/misc_utils.py
+drwxrwxrwx   0        0        0        0 2023-06-27 03:19:45.637386 control-lab-ly-1.1.1a1/src/controllably/misc/templates/
+-rw-rw-rw-   0        0        0        0 2023-02-23 06:19:52.000000 control-lab-ly-1.1.1a1/src/controllably/misc/templates/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-27 03:19:45.651030 control-lab-ly-1.1.1a1/src/controllably/misc/templates/configs/
+-rw-rw-rw-   0        0        0        0 2023-02-23 14:08:10.000000 control-lab-ly-1.1.1a1/src/controllably/misc/templates/configs/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-27 03:19:45.669039 control-lab-ly-1.1.1a1/src/controllably/misc/templates/configs/plugins/
+-rw-rw-rw-   0        0        0        0 2023-04-11 09:18:51.000000 control-lab-ly-1.1.1a1/src/controllably/misc/templates/configs/plugins/__init__.py
+-rw-rw-rw-   0        0        0     1091 2023-04-12 15:51:49.000000 control-lab-ly-1.1.1a1/src/controllably/misc/templates/configs/plugins/plugin_template.py
+-rw-rw-rw-   0        0        0      439 2023-04-12 15:51:49.000000 control-lab-ly-1.1.1a1/src/controllably/misc/templates/configs/registry.yaml
+drwxrwxrwx   0        0        0        0 2023-06-27 03:19:45.687769 control-lab-ly-1.1.1a1/src/controllably/misc/templates/setup/
+-rw-rw-rw-   0        0        0      772 2023-04-12 15:51:49.000000 control-lab-ly-1.1.1a1/src/controllably/misc/templates/setup/__init__.py
+-rw-rw-rw-   0        0        0     1434 2023-04-12 15:51:49.000000 control-lab-ly-1.1.1a1/src/controllably/misc/templates/setup/config.yaml
+-rw-rw-rw-   0        0        0      987 2023-04-12 15:51:49.000000 control-lab-ly-1.1.1a1/src/controllably/misc/templates/setup/layout.json
+drwxrwxrwx   0        0        0        0 2023-06-27 03:19:45.697770 control-lab-ly-1.1.1a1/tests/
+-rw-rw-rw-   0        0        0     2365 2023-06-15 06:52:40.000000 control-lab-ly-1.1.1a1/tests/test_panels.py
```

### Comparing `control-lab-ly-1.1.0b1/LICENSE.md` & `control-lab-ly-1.1.1a1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.0b1/PKG-INFO` & `control-lab-ly-1.1.1a1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: control-lab-ly
-Version: 1.1.0b1
+Version: 1.1.1a1
 Summary: Lab Equipment Automation Package
 Home-page: https://github.com/kylejeanlewis/control-lab-le
 Author: Chang Jie Leong
 Author-email: changjie.leong@outlook.com
 License: MIT
 Project-URL: GitHub, https://github.com/kylejeanlewis/control-lab-le
 Project-URL: Documentation, https://github.com/kylejeanlewis/control-lab-le/blob/main/docs/README.md
@@ -36,15 +36,15 @@
 4. Measure
 5. Move
 6. Transfer
 7. View
 
 ## Device support
 - Make
-  - (QInstruments) Bioshake Orbital Shaker
+  - (QInstruments) BioShake Orbital Shaker
   - Multi-channel LED array \[Arduino\]
   - Multi-channel spin-coater \[Arduino\]
   - Peltier device \[Arduino\]
 - Measure
   - (Keithley) 2450 Source Measure Unit (SMU) Instrument
   - (PiezoRobotics) Dynamic Mechanical Analyser (DMA)
   - (Sentron) SI series pH meters - *full functionality in development*
@@ -288,15 +288,15 @@
 
 ### 4. Using plugins
 *Optional: if drivers for your hardware components are already included, plugins may not be required*
 
 User-defined plugins can be easily written and integrated into Control.lab.ly. All available classes and functions can be found in `lab.modules`.
 ```python
 lab.guide_me()                              # Use guide to view imported objects
-lab.modules.at.Make.Something.Good.MyClass  # Access the the class 
+lab.modules.at.Make.Something.Good.MyClass  # Access the class 
 ```
 
 #### 4.1 Registering a Class or Function
 You can import the class and register the object using the `Factory.register()` function.
 ```python
 from my_module import MyClass
 lab.Factory.register(MyClass, "Make.Something.Good")
```

### Comparing `control-lab-ly-1.1.0b1/docs/CHANGELOG.md` & `control-lab-ly-1.1.1a1/docs/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.0b1/docs/CODE_OF_CONDUCT.md` & `control-lab-ly-1.1.1a1/docs/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.0b1/docs/LICENSE.md` & `control-lab-ly-1.1.1a1/docs/LICENSE.md`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.0b1/docs/README.md` & `control-lab-ly-1.1.1a1/docs/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 4. Measure
 5. Move
 6. Transfer
 7. View
 
 ## Device support
 - Make
-  - (QInstruments) Bioshake Orbital Shaker
+  - (QInstruments) BioShake Orbital Shaker
   - Multi-channel LED array \[Arduino\]
   - Multi-channel spin-coater \[Arduino\]
   - Peltier device \[Arduino\]
 - Measure
   - (Keithley) 2450 Source Measure Unit (SMU) Instrument
   - (PiezoRobotics) Dynamic Mechanical Analyser (DMA)
   - (Sentron) SI series pH meters - *full functionality in development*
@@ -263,15 +263,15 @@
 
 ### 4. Using plugins
 *Optional: if drivers for your hardware components are already included, plugins may not be required*
 
 User-defined plugins can be easily written and integrated into Control.lab.ly. All available classes and functions can be found in `lab.modules`.
 ```python
 lab.guide_me()                              # Use guide to view imported objects
-lab.modules.at.Make.Something.Good.MyClass  # Access the the class 
+lab.modules.at.Make.Something.Good.MyClass  # Access the class 
 ```
 
 #### 4.1 Registering a Class or Function
 You can import the class and register the object using the `Factory.register()` function.
 ```python
 from my_module import MyClass
 lab.Factory.register(MyClass, "Make.Something.Good")
```

### Comparing `control-lab-ly-1.1.0b1/docs/assets/Documentation guide.png` & `control-lab-ly-1.1.1a1/docs/assets/Documentation guide.png`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.0b1/setup.cfg` & `control-lab-ly-1.1.1a1/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2063 6f6e 7472 6f6c 2d6c 6162 2d6c   = control-lab-l
 00000020: 790d 0a76 6572 7369 6f6e 203d 2031 2e31  y..version = 1.1
-00000030: 2e30 2d62 310d 0a64 6573 6372 6970 7469  .0-b1..descripti
+00000030: 2e31 2d61 310d 0a64 6573 6372 6970 7469  .1-a1..descripti
 00000040: 6f6e 203d 204c 6162 2045 7175 6970 6d65  on = Lab Equipme
 00000050: 6e74 2041 7574 6f6d 6174 696f 6e20 5061  nt Automation Pa
 00000060: 636b 6167 650d 0a6c 6f6e 675f 6465 7363  ckage..long_desc
 00000070: 7269 7074 696f 6e20 3d20 6669 6c65 3a20  ription = file: 
 00000080: 646f 6373 2f52 4541 444d 452e 6d64 2c20  docs/README.md, 
 00000090: 646f 6373 2f43 4841 4e47 454c 4f47 2e6d  docs/CHANGELOG.m
 000000a0: 640d 0a6c 6f6e 675f 6465 7363 7269 7074  d..long_descript
```

### Comparing `control-lab-ly-1.1.0b1/src/control_lab_ly.egg-info/PKG-INFO` & `control-lab-ly-1.1.1a1/src/control_lab_ly.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: control-lab-ly
-Version: 1.1.0b1
+Version: 1.1.1a1
 Summary: Lab Equipment Automation Package
 Home-page: https://github.com/kylejeanlewis/control-lab-le
 Author: Chang Jie Leong
 Author-email: changjie.leong@outlook.com
 License: MIT
 Project-URL: GitHub, https://github.com/kylejeanlewis/control-lab-le
 Project-URL: Documentation, https://github.com/kylejeanlewis/control-lab-le/blob/main/docs/README.md
@@ -36,15 +36,15 @@
 4. Measure
 5. Move
 6. Transfer
 7. View
 
 ## Device support
 - Make
-  - (QInstruments) Bioshake Orbital Shaker
+  - (QInstruments) BioShake Orbital Shaker
   - Multi-channel LED array \[Arduino\]
   - Multi-channel spin-coater \[Arduino\]
   - Peltier device \[Arduino\]
 - Measure
   - (Keithley) 2450 Source Measure Unit (SMU) Instrument
   - (PiezoRobotics) Dynamic Mechanical Analyser (DMA)
   - (Sentron) SI series pH meters - *full functionality in development*
@@ -288,15 +288,15 @@
 
 ### 4. Using plugins
 *Optional: if drivers for your hardware components are already included, plugins may not be required*
 
 User-defined plugins can be easily written and integrated into Control.lab.ly. All available classes and functions can be found in `lab.modules`.
 ```python
 lab.guide_me()                              # Use guide to view imported objects
-lab.modules.at.Make.Something.Good.MyClass  # Access the the class 
+lab.modules.at.Make.Something.Good.MyClass  # Access the class 
 ```
 
 #### 4.1 Registering a Class or Function
 You can import the class and register the object using the `Factory.register()` function.
 ```python
 from my_module import MyClass
 lab.Factory.register(MyClass, "Make.Something.Good")
```

### Comparing `control-lab-ly-1.1.0b1/src/control_lab_ly.egg-info/SOURCES.txt` & `control-lab-ly-1.1.1a1/src/control_lab_ly.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -76,14 +76,15 @@
 src/controllably/Measure/Physical/balance_utils.py
 src/controllably/Measure/Physical/force_sensor_utils.py
 src/controllably/Move/__init__.py
 src/controllably/Move/move_utils.py
 src/controllably/Move/Cartesian/__init__.py
 src/controllably/Move/Cartesian/cartesian_utils.py
 src/controllably/Move/Cartesian/ender_utils.py
+src/controllably/Move/Cartesian/grbl_lib.py
 src/controllably/Move/Cartesian/primitiv_utils.py
 src/controllably/Move/Jointed/__init__.py
 src/controllably/Move/Jointed/jointed_utils.py
 src/controllably/Move/Jointed/Dobot/__init__.py
 src/controllably/Move/Jointed/Dobot/dobot_utils.py
 src/controllably/Move/Jointed/Dobot/m1pro_utils.py
 src/controllably/Move/Jointed/Dobot/mg400_utils.py
@@ -117,14 +118,15 @@
 src/controllably/View/Optical/__init__.py
 src/controllably/View/Optical/optical_utils.py
 src/controllably/View/Optical/placeholders/__init__.py
 src/controllably/View/Optical/placeholders/optical_camera.png
 src/controllably/View/Thermal/__init__.py
 src/controllably/View/Thermal/thermal_utils.py
 src/controllably/View/Thermal/Flir/__init__.py
+src/controllably/View/Thermal/Flir/ax8_utils.py
 src/controllably/View/Thermal/Flir/ax8/__init__.py
 src/controllably/View/Thermal/Flir/ax8/ax8.py
 src/controllably/View/Thermal/Flir/ax8/ax8_camera_feed.py
 src/controllably/View/Thermal/Flir/ax8/ax8_modbus_regs.py
 src/controllably/View/Thermal/Flir/ax8/ax8_modbus_utils.py
 src/controllably/View/Thermal/placeholders/__init__.py
 src/controllably/View/Thermal/placeholders/infrared_camera.png
@@ -139,27 +141,8 @@
 src/controllably/misc/templates/configs/__init__.py
 src/controllably/misc/templates/configs/registry.yaml
 src/controllably/misc/templates/configs/plugins/__init__.py
 src/controllably/misc/templates/configs/plugins/plugin_template.py
 src/controllably/misc/templates/setup/__init__.py
 src/controllably/misc/templates/setup/config.yaml
 src/controllably/misc/templates/setup/layout.json
-tests/test_camera_optical.py
-tests/test_camera_thermal.py
-tests/test_cartesian_ender.py
-tests/test_cartesian_primitiv.py
-tests/test_compound_liquidmover.py
-tests/test_compound_spin_printer.py
-tests/test_dobot_m1pro.py
-tests/test_dobot_mg400.py
-tests/test_electrical_keithley.py
-tests/test_film_spin.py
-tests/test_heat_peltier.py
-tests/test_light_led_array.py
-tests/test_liquid_sartorius.py
-tests/test_liquid_syringe_assembly.py
-tests/test_liquid_tricontinent.py
-tests/test_mechanical_piezorobotics.py
-tests/test_mixture_shaker.py
-tests/test_panels.py
-tests/test_physical_balance.py
-tests/test_pump_peristaltic.py
+tests/test_panels.py
```

### Comparing `control-lab-ly-1.1.0b1/src/controllably/Compound/LiquidMover/liquidmover_utils.py` & `control-lab-ly-1.1.1a1/src/controllably/Compound/LiquidMover/liquidmover_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.0b1/src/controllably/Compound/compound_utils.py` & `control-lab-ly-1.1.1a1/src/controllably/Compound/compound_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.0b1/src/controllably/Control/GUI/Basic/__init__.py` & `control-lab-ly-1.1.1a1/src/controllably/Control/GUI/Basic/__init__.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.0b1/src/controllably/Control/GUI/Basic/maker_panel.py` & `control-lab-ly-1.1.1a1/src/controllably/Control/GUI/Basic/maker_panel.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.0b1/src/controllably/Control/GUI/Basic/measurer_panel.py` & `control-lab-ly-1.1.1a1/src/controllably/Control/GUI/Basic/measurer_panel.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.0b1/src/controllably/Control/GUI/Basic/mover_panel.py` & `control-lab-ly-1.1.1a1/src/controllably/Control/GUI/Basic/mover_panel.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,14 +32,16 @@
         ...
     def moveTo(self, *args, **kwargs):
         ...
     def reset(self, *args, **kwargs):
         ...
     def rotateTo(self, *args, **kwargs):
         ...
+    def safeMoveTo(self, *args, **kwargs):
+        ...
     def _transform_out(self, *args, **kwargs):
         ...
         
 class MoverPanel(Panel):
     """
     MoverPanel provides methods to create a control panel for a mover
 
@@ -237,15 +239,15 @@
             self.flags['update_position'] = True
             tool_position = list(np.concatenate(self.mover.tool_position))
             
         # 5. Go to position
         if event == self._mangle(f'-Go-'):
             coord = [float(values[self._mangle(f'-{axis}-VALUE-')]) for axis in ['X','Y','Z']]
             orientation = [float(values[self._mangle(f'-{axis}-VALUE-')]) for axis in ['a','b','c']]
-            self.mover.moveTo(coord, orientation)
+            self.mover.safeMoveTo(coord, orientation)
             tool_position = list(np.concatenate(self.mover.tool_position))
         
         # 6. Reset mover
         if event == self._mangle(f'-Reset-'):
             self.mover.reset()
             tool_position = cache_position
```

### Comparing `control-lab-ly-1.1.0b1/src/controllably/Control/GUI/Basic/transfer_liquid_panel.py` & `control-lab-ly-1.1.1a1/src/controllably/Control/GUI/Basic/transfer_liquid_panel.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.0b1/src/controllably/Control/GUI/Basic/viewer_panel.py` & `control-lab-ly-1.1.1a1/src/controllably/Control/GUI/Basic/viewer_panel.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.0b1/src/controllably/Control/GUI/Elements/loader_panel.py` & `control-lab-ly-1.1.1a1/src/controllably/Control/GUI/Elements/loader_panel.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.0b1/src/controllably/Control/GUI/Elements/pop_ups.py` & `control-lab-ly-1.1.1a1/src/controllably/Control/GUI/Elements/pop_ups.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.0b1/src/controllably/Control/GUI/Elements/templates.py` & `control-lab-ly-1.1.1a1/src/controllably/Control/GUI/Elements/templates.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.0b1/src/controllably/Control/GUI/__init__.py` & `control-lab-ly-1.1.1a1/src/controllably/Control/GUI/__init__.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.0b1/src/controllably/Control/GUI/_guibuilder.py` & `control-lab-ly-1.1.1a1/src/controllably/Control/GUI/_guibuilder.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.0b1/src/controllably/Control/GUI/compound_panel.py` & `control-lab-ly-1.1.1a1/src/controllably/Control/GUI/compound_panel.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.0b1/src/controllably/Control/GUI/gui_utils.py` & `control-lab-ly-1.1.1a1/src/controllably/Control/GUI/gui_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.0b1/src/controllably/Control/GUI/guide_panel.py` & `control-lab-ly-1.1.1a1/src/controllably/Control/GUI/guide_panel.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.0b1/src/controllably/Control/GUI/multichannel_panel.py` & `control-lab-ly-1.1.1a1/src/controllably/Control/GUI/multichannel_panel.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.0b1/src/controllably/Make/Heat/peltier_utils.py` & `control-lab-ly-1.1.1a1/src/controllably/Make/Heat/peltier_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -156,17 +156,16 @@
             elif (self._power <= self.power_threshold) or (time.perf_counter()-self._stabilize_time >= self.stabilize_buffer_time):
                 print(response)
                 self.setFlag(temperature_reached=True)
                 print(f"Temperature of {self.set_temperature}°C reached!")
             if self.flags['record']:
                 values = [now] + values
                 row = {k:v for k,v in zip(self._columns, values)}
-                # self.buffer_df = self.buffer_df.append(row, ignore_index=True)
-                new_row_df = pd.DataFrame(row)
-                self.buffer_df = pd.concat([self.buffer_df, new_row_df])
+                new_row_df = pd.DataFrame(row, index=[0])
+                self.buffer_df = pd.concat([self.buffer_df, new_row_df], ignore_index=True)
         return response
     
     def holdTemperature(self, temperature:float, time_s:float):
         """
         Hold target temperature for desired duration
 
         Args:
```

### Comparing `control-lab-ly-1.1.0b1/src/controllably/Make/Light/led_utils.py` & `control-lab-ly-1.1.1a1/src/controllably/Make/Light/led_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -246,15 +246,15 @@
             device = serial.Serial(port, baudrate, timeout=timeout)
         except Exception as e:
             print(f"Could not connect to {port}")
             if self.verbose:
                 print(e)
         else:
             time.sleep(5)   # Wait for grbl to initialize
-            device.flushInput()
+            device.reset_input_buffer()
             self.turnOff()
             print(f"Connection opened to {port}")
             self.setFlag(connected=True)
         self.device = device
         return
         
     def _loop_timer(self):
```

### Comparing `control-lab-ly-1.1.0b1/src/controllably/Make/Mixture/QInstruments/orbital_shaker_utils.py` & `control-lab-ly-1.1.1a1/src/controllably/Make/Mixture/QInstruments/orbital_shaker_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -320,17 +320,16 @@
         
         flag = (abs(self.temperature - self.set_temperature) <= self.tolerance*self.set_temperature) if self.set_temperature else False
         self.setFlag(temperature_reached=flag)
         
         if self.flags['record']:
             values = [now, self.set_temperature, self.temperature]
             row = {k:v for k,v in zip(self._columns, values)}
-            # self.buffer_df = self.buffer_df.append(row, ignore_index=True)
-            new_row_df = pd.DataFrame(row)
-            self.buffer_df = pd.concat([self.buffer_df, new_row_df])
+            new_row_df = pd.DataFrame(row, index=[0])
+            self.buffer_df = pd.concat([self.buffer_df, new_row_df], ignore_index=True)
         return self.set_temperature, self.temperature
     
     def getUserLimits(self):
         """Retrieve the user defined limits for speed and temperature"""
         if not self.isConnected():
             return
         try:
```

### Comparing `control-lab-ly-1.1.0b1/src/controllably/Make/Mixture/QInstruments/qinstruments_api/qinstruments_api.py` & `control-lab-ly-1.1.1a1/src/controllably/Make/Mixture/QInstruments/qinstruments_api/qinstruments_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -992,18 +992,18 @@
 
         Args:
             command (str): <command code><value>
 
         Returns:
             bool: whether command was sent successfully
         """
-        if self.verbose:
-            print(command)
         fstring = f'{command}\r' # command template: <long_form><\r> | <short_form><\r>
         # bstring = bytearray.fromhex(fstring.encode('utf-8').hex())
+        if self.verbose:
+            print(fstring)
         try:
             # Typical timeout wait is 400ms
             self.device.write(fstring.encode('utf-8'))
         except AttributeError:
             pass
         except Exception as e:
             if self.verbose:
```

### Comparing `control-lab-ly-1.1.0b1/src/controllably/Make/Mixture/QInstruments/qinstruments_api/qinstruments_lib.py` & `control-lab-ly-1.1.1a1/src/controllably/Make/Mixture/QInstruments/qinstruments_api/qinstruments_lib.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.0b1/src/controllably/Make/ThinFilm/spinner_utils.py` & `control-lab-ly-1.1.1a1/src/controllably/Make/ThinFilm/spinner_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -169,15 +169,15 @@
             device = serial.Serial(port, baudrate, timeout=timeout)
         except Exception as e:
             print(f"Could not connect to {port}")
             if self.verbose:
                 print(e)
         else:
             time.sleep(2)   # Wait for grbl to initialize
-            device.flushInput()
+            device.reset_input_buffer()
             print(f"Connection opened to {port}")
             self.setFlag(connected=True)
         self.device = device
         return
     
     def _diagnostic(self):
         """Run diagnostic test"""
@@ -189,16 +189,19 @@
     def _write(self, speed:int):
         """
         Relay spin speed to spinner
 
         Args:
             speed (int): spin speed in rpm
         """
+        fstring = f"{speed}\n", 'utf-8'
+        if self.verbose:
+            print(fstring)
         try:
-            self.device.write(bytes(f"{speed}\n", 'utf-8'))
+            self.device.write(fstring.encode('utf-8'))
         except AttributeError:
             pass
         print(f"Spin speed (channel {self.channel}): {speed}")
         return
 
 
 class SpinnerAssembly(Maker):
```

### Comparing `control-lab-ly-1.1.0b1/src/controllably/Make/make_utils.py` & `control-lab-ly-1.1.1a1/src/controllably/Make/make_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.0b1/src/controllably/Measure/Electrical/Keithley/keithley_device.py` & `control-lab-ly-1.1.1a1/src/controllably/Measure/Electrical/Keithley/keithley_device.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.0b1/src/controllably/Measure/Electrical/Keithley/keithley_lib.py` & `control-lab-ly-1.1.1a1/src/controllably/Measure/Electrical/Keithley/keithley_lib.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.0b1/src/controllably/Measure/Electrical/Keithley/keithley_utils.py` & `control-lab-ly-1.1.1a1/src/controllably/Measure/Electrical/Keithley/keithley_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.0b1/src/controllably/Measure/Electrical/Keithley/programs/base_programs.py` & `control-lab-ly-1.1.1a1/src/controllably/Measure/Electrical/Keithley/programs/base_programs.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.0b1/src/controllably/Measure/Mechanical/PiezoRobotics/piezorobotics_device.py` & `control-lab-ly-1.1.1a1/src/controllably/Measure/Mechanical/PiezoRobotics/piezorobotics_device.py`

 * *Files 1% similar despite different names*

```diff
@@ -198,14 +198,15 @@
         except Exception as e:
             print(f"Could not connect to {port}")
             if self.verbose:
                 print(e)
         else:
             print(f"Connection opened to {port}")
             self.setFlag(connected=True)
+            self.initialise()
         self.device = device
         return
     
     def _query(self, command:str, timeout_s:int = 60) -> Union[str, tuple[str]]:
         """
         Write command to and read response from device
 
@@ -286,18 +287,18 @@
 
         Args:
             command (str): <command code>,<option 1>[,<option 2>]
         
         Returns:
             bool: whether command was sent successfully
         """
-        if self.verbose:
-            print(command)
         fstring = f'DMA,SN{self.channel},{command},END' # command template: <PRE>,<SN>,<CODE>,<OPTIONS>,<POST>
         # bstring = bytearray.fromhex(fstring.encode('utf-8').hex())
+        if self.verbose:
+            print(fstring)
         try:
             self.device.write(fstring.encode('utf-8'))
         except AttributeError:
             pass
         except Exception as e:
             if self.verbose:
                 print(e)
```

### Comparing `control-lab-ly-1.1.0b1/src/controllably/Measure/Mechanical/PiezoRobotics/piezorobotics_lib.py` & `control-lab-ly-1.1.1a1/src/controllably/Measure/Mechanical/PiezoRobotics/piezorobotics_lib.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.0b1/src/controllably/Measure/Mechanical/PiezoRobotics/piezorobotics_utils.py` & `control-lab-ly-1.1.1a1/src/controllably/Measure/Mechanical/PiezoRobotics/piezorobotics_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.0b1/src/controllably/Measure/Mechanical/PiezoRobotics/programs/base_programs.py` & `control-lab-ly-1.1.1a1/src/controllably/Measure/Mechanical/PiezoRobotics/programs/base_programs.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,18 +79,18 @@
         return
     
     def run(self):
         """Run the measurement program"""
         device = self.device
         repeat = self.parameters.get('repeat', 1)
         device.toggleClamp(False)
-        device.initialise(
-            low_frequency=self.parameters.get('low_frequency', FREQUENCIES[0]), 
-            high_frequency=self.parameters.get('high_frequency', FREQUENCIES[-1])
-        )
+        # device.initialise(
+        #     low_frequency=self.parameters.get('low_frequency', FREQUENCIES[0]), 
+        #     high_frequency=self.parameters.get('high_frequency', FREQUENCIES[-1])
+        # )
         
         if self.parameters.get('pause', True):
             input("Please load sample. Press 'Enter' to proceed")
         device.toggleClamp(True)
         for i in range(repeat):
             print(f"Start run {i+1} at {datetime.now()}")
             device.run(sample_thickness=self.parameters.get('sample_thickness', 1E-3))
```

### Comparing `control-lab-ly-1.1.0b1/src/controllably/Measure/Physical/balance_utils.py` & `control-lab-ly-1.1.1a1/src/controllably/Measure/Physical/balance_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.0b1/src/controllably/Measure/Physical/force_sensor_utils.py` & `control-lab-ly-1.1.1a1/src/controllably/Measure/Physical/force_sensor_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.0b1/src/controllably/Measure/__init__.py` & `control-lab-ly-1.1.1a1/src/controllably/Measure/__init__.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.0b1/src/controllably/Measure/instrument_utils.py` & `control-lab-ly-1.1.1a1/src/controllably/Measure/instrument_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.0b1/src/controllably/Measure/measure_utils.py` & `control-lab-ly-1.1.1a1/src/controllably/Measure/measure_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -35,18 +35,18 @@
         `verbose` (bool, optional): verbosity of class. Defaults to False.
     
     ### Attributes
     - `buffer_df` (pd.DataFrame): buffer dataframe to store collected data
     - `connection_details` (dict): dictionary of connection details (e.g. COM port / IP address)
     - `device` (Callable): device object that communicates with physical tool
     - `flags` (dict[str, bool]): keywords paired with boolean flags
-    - `verbose` (bool): verbosity of class
     
     ### Properties
     - `instrument` (Callable): Alias for `device`
+    - `verbose` (bool): verbosity of class
     
     ### Methods
     #### Abstract
     - `clearCache`: clear most recent data and configurations
     - `disconnect`: disconnect from device
     - `_connect`: connection procedure for tool
     #### Public
@@ -101,14 +101,31 @@
     # Properties
     @property
     def instrument(self) -> Callable:
         return self.device
     @instrument.setter
     def instrument(self, device:Callable):
         self.device = device
+        return
+    
+    @property
+    def verbose(self) -> bool:
+        return self._verbose
+    @verbose.setter
+    def verbose(self, value:bool):
+        self._verbose = bool(value)
+        try:
+            self.device.verbose = self._verbose
+        except AttributeError:
+            pass
+        return
+    @verbose.deleter
+    def verbose(self):
+        del self._verbose
+        return
     
     def connect(self):
         """Establish connection with device"""
         return self._connect(**self.connection_details)
 
     def isBusy(self) -> bool:
         """
```

### Comparing `control-lab-ly-1.1.0b1/src/controllably/Measure/program_utils.py` & `control-lab-ly-1.1.1a1/src/controllably/Measure/program_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.0b1/src/controllably/Move/Cartesian/cartesian_utils.py` & `control-lab-ly-1.1.1a1/src/controllably/Move/Cartesian/cartesian_utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -177,25 +177,28 @@
     
     def reset(self):
         """Reset the robot"""
         self.disconnect()
         self.connect()
         return super().reset()
     
-    def setSpeed(self, speed: int):
+    def setSpeed(self, speed: int) -> tuple[bool, float]:
         """
         Set the speed of the robot
 
         Args:
             speed (int): speed in mm/s
+        
+        Returns:
+            tuple[bool, float]: whether speed has changed; speed
         """
         print(f'Speed: {speed} mm/s')
-        self._speed_fraction = (speed/self._speed_max)
-        speed = int(self._speed_max*self._speed_fraction * 60)   # get speed in mm/min
-        self._query(f"G01 F{speed}\n")  # feed rate (i.e. speed) in mm/min
+        # self._speed_fraction = (speed/self._speed_max)
+        # speed = int(self._speed_max*self._speed_fraction * 60)   # get speed in mm/min
+        # self._query(f"G01 F{speed}\n")  # feed rate (i.e. speed) in mm/min
         return False, self.speed
     
     def shutdown(self):
         """Shutdown procedure for tool"""
         # self.home()
         return super().shutdown()
     
@@ -224,45 +227,47 @@
         else:
             time.sleep(2)
             print(f"Connection opened to {port}")
             self.setFlag(connected=True)
         self.device = device
         return
 
-    def _query(self, command:str) -> str:
+    def _query(self, command:str) -> list[str]:
         """
         Write command to and read response from device
 
         Args:
             command (str): command string to send to device
 
         Returns:
-            str: response string from device
+            list[str]: list of response string(s) from device
         """
-        response = ''
+        responses = [b'']
         self._write(command)
         try:
-            response = self.device.readline()
+            responses = self.device.readlines()
         except Exception as e:
             if self.verbose:
                 print(e)
         else:
-            print(response)
-        return response
+            print(responses)
+        # self._handle_alarms_and_errors(response=response.decode())
+        return [r.decode().strip() for r in responses]
 
     def _write(self, command:str) -> bool:
         """
         Write command to device
 
         Args:
             command (str): command string to send to device
 
         Returns:
             bool: whether the command is sent successfully
         """
+        command = f"{command}\n" if not command.endswith('\n') else command
         if self.verbose:
             print(command)
         try:
             self.device.write(command.encode('utf-8'))
         except Exception as e:
             if self.verbose:
                 print(e)
```

### Comparing `control-lab-ly-1.1.0b1/src/controllably/Move/Cartesian/ender_utils.py` & `control-lab-ly-1.1.1a1/src/controllably/Move/Cartesian/ender_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.0b1/src/controllably/Move/Jointed/Dobot/dobot_api/dobot_api.py` & `control-lab-ly-1.1.1a1/src/controllably/Move/Jointed/Dobot/dobot_api/dobot_api.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.0b1/src/controllably/Move/Jointed/Dobot/dobot_utils.py` & `control-lab-ly-1.1.1a1/src/controllably/Move/Jointed/Dobot/dobot_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.0b1/src/controllably/Move/Jointed/Dobot/m1pro_utils.py` & `control-lab-ly-1.1.1a1/src/controllably/Move/Jointed/Dobot/m1pro_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.0b1/src/controllably/Move/Jointed/Dobot/mg400_utils.py` & `control-lab-ly-1.1.1a1/src/controllably/Move/Jointed/Dobot/mg400_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.0b1/src/controllably/Move/Jointed/jointed_utils.py` & `control-lab-ly-1.1.1a1/src/controllably/Move/Jointed/jointed_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.0b1/src/controllably/Move/move_utils.py` & `control-lab-ly-1.1.1a1/src/controllably/Move/move_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.0b1/src/controllably/Transfer/Liquid/Pumps/TriContinent/tricontinent_lib.py` & `control-lab-ly-1.1.1a1/src/controllably/Transfer/Liquid/Pumps/TriContinent/tricontinent_lib.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.0b1/src/controllably/Transfer/Liquid/Pumps/TriContinent/tricontinent_utils.py` & `control-lab-ly-1.1.1a1/src/controllably/Transfer/Liquid/Pumps/TriContinent/tricontinent_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -839,17 +839,17 @@
 
         Args:
             command (str): <command code><value>
 
         Returns:
             bool: whether command was sent successfully
         """
-        if self.verbose:
-            print(command)
         fstring = f'/{self.channel}{command}\r' # command template: <PRE><ADR><STRING><POST>
+        if self.verbose:
+            print(fstring)
         try:
             # Typical timeout wait is 2s
             self.device.write(fstring.encode('utf-8'))
         except AttributeError:
             pass
         except Exception as e:
             if self.verbose:
```

### Comparing `control-lab-ly-1.1.0b1/src/controllably/Transfer/Liquid/Pumps/peristaltic_utils.py` & `control-lab-ly-1.1.1a1/src/controllably/Transfer/Liquid/Pumps/peristaltic_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.0b1/src/controllably/Transfer/Liquid/Pumps/pump_utils.py` & `control-lab-ly-1.1.1a1/src/controllably/Transfer/Liquid/Pumps/pump_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -83,15 +83,15 @@
             device = serial.Serial(port, baudrate, timeout=timeout)
         except Exception as e:
             print(f"Could not connect to {port}")
             if self.verbose:
                 print(e)
         else:
             time.sleep(2)   # Wait for grbl to initialize
-            device.flushInput()
+            device.reset_input_buffer()
             print(f"Connection opened to {port}")
             self.setFlag(connected=True)
         self.device = device
         return
     
     def _write(self, command:str) -> bool:
         """
@@ -99,14 +99,16 @@
 
         Args:
             command (str): command string
 
         Returns:
             bool: whether command was sent successfully
         """
+        if self.verbose:
+            print(command)
         try:
             self.device.write(command.encode('utf-8'))
         except Exception as e:
             if self.verbose:
                 print(e)
             return False
         return True
```

### Comparing `control-lab-ly-1.1.0b1/src/controllably/Transfer/Liquid/Sartorius/sartorius_lib.py` & `control-lab-ly-1.1.1a1/src/controllably/Transfer/Liquid/Sartorius/sartorius_lib.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.0b1/src/controllably/Transfer/Liquid/Sartorius/sartorius_utils.py` & `control-lab-ly-1.1.1a1/src/controllably/Transfer/Liquid/Sartorius/sartorius_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,1912 +70,1942 @@
 00000450: 742c 206f 7074 696f 6e61 6c29 3a20 6465  t, optional): de
 00000460: 6c61 7920 6265 7477 6565 6e20 7365 6e64  lay between send
 00000470: 696e 6720 6120 636f 6d6d 616e 6420 616e  ing a command an
 00000480: 6420 7265 6365 6976 696e 6720 6120 7265  d receiving a re
 00000490: 7370 6f6e 7365 2c20 696e 2073 6563 6f6e  sponse, in secon
 000004a0: 6473 2e20 4465 6661 756c 7473 2074 6f20  ds. Defaults to 
 000004b0: 312e 3033 2e0d 0a20 2020 2020 2020 2060  1.03...        `
-000004c0: 7469 705f 7468 7265 7368 6f6c 6460 2028  tip_threshold` (
-000004d0: 696e 742c 206f 7074 696f 6e61 6c29 3a20  int, optional): 
-000004e0: 7468 7265 7368 6f6c 6420 6162 6f76 6520  threshold above 
-000004f0: 7768 6963 6820 6120 636f 6e64 7563 7469  which a conducti
-00000500: 7665 2070 6970 6574 7465 2074 6970 2069  ve pipette tip i
-00000510: 7320 636f 6e73 6964 6572 6564 2074 6f20  s considered to 
-00000520: 6265 2061 7474 6163 6865 642e 2044 6566  be attached. Def
-00000530: 6175 6c74 7320 746f 2032 3736 2e0d 0a20  aults to 276... 
-00000540: 2020 200d 0a20 2020 2023 2323 2041 7474     ..    ### Att
-00000550: 7269 6275 7465 730d 0a20 2020 202d 2060  ributes..    - `
-00000560: 6368 616e 6e65 6c60 2028 696e 7429 3a20  channel` (int): 
-00000570: 6368 616e 6e65 6c20 6964 0d0a 2020 2020  channel id..    
-00000580: 2d20 606c 696d 6974 7360 2028 7475 706c  - `limits` (tupl
-00000590: 655b 696e 745d 293a 206c 6f77 6572 2061  e[int]): lower a
-000005a0: 6e64 2075 7070 6572 2073 7465 7020 6c69  nd upper step li
-000005b0: 6d69 7473 0d0a 2020 2020 2d20 606d 6f64  mits..    - `mod
-000005c0: 656c 5f69 6e66 6f60 2028 5361 7274 6f72  el_info` (Sartor
-000005d0: 6975 7350 6970 6574 7465 4d6f 6465 6c29  iusPipetteModel)
-000005e0: 3a20 5361 7274 6f72 6975 7320 6d6f 6465  : Sartorius mode
-000005f0: 6c20 696e 666f 0d0a 2020 2020 2d20 606f  l info..    - `o
-00000600: 6666 7365 7460 2028 7475 706c 655b 666c  ffset` (tuple[fl
-00000610: 6f61 745d 293a 2078 2c79 2c7a 206f 6666  oat]): x,y,z off
-00000620: 7365 7420 6f66 2074 6970 0d0a 2020 2020  set of tip..    
-00000630: 2d20 6070 6f73 6974 696f 6e60 2028 696e  - `position` (in
-00000640: 7429 3a20 706f 7369 7469 6f6e 206f 6620  t): position of 
-00000650: 706c 756e 6765 720d 0a20 2020 202d 2060  plunger..    - `
-00000660: 7265 7370 6f6e 7365 5f74 696d 6560 2028  response_time` (
-00000670: 666c 6f61 7429 3a20 6465 6c61 7920 6265  float): delay be
-00000680: 7477 6565 6e20 7365 6e64 696e 6720 6120  tween sending a 
-00000690: 636f 6d6d 616e 6420 616e 6420 7265 6365  command and rece
-000006a0: 6976 696e 6720 6120 7265 7370 6f6e 7365  iving a response
-000006b0: 2c20 696e 2073 6563 6f6e 6473 0d0a 2020  , in seconds..  
-000006c0: 2020 2d20 6073 7065 6564 5f63 6f64 6560    - `speed_code`
-000006d0: 2028 5370 6565 6429 3a20 636f 6465 7320   (Speed): codes 
-000006e0: 666f 7220 6173 7069 7261 7465 2061 6e64  for aspirate and
-000006f0: 2064 6973 7065 6e73 6520 7370 6565 6473   dispense speeds
-00000700: 0d0a 2020 2020 2d20 6073 7065 6564 5f70  ..    - `speed_p
-00000710: 7265 7365 7473 6020 2850 7265 7365 7453  resets` (PresetS
-00000720: 7065 6564 7329 3a20 7072 6573 6574 2073  peeds): preset s
-00000730: 7065 6564 7320 6176 6169 6c61 626c 650d  peeds available.
-00000740: 0a20 2020 202d 2060 7469 705f 6c65 6e67  .    - `tip_leng
-00000750: 7468 6020 2866 6c6f 6174 293a 206c 656e  th` (float): len
-00000760: 6774 6820 6f66 2070 6970 6574 7465 2074  gth of pipette t
-00000770: 6970 0d0a 2020 2020 2d20 6074 6970 5f74  ip..    - `tip_t
-00000780: 6872 6573 686f 6c64 6020 2869 6e74 293a  hreshold` (int):
-00000790: 2074 6872 6573 686f 6c64 2061 626f 7665   threshold above
-000007a0: 2077 6869 6368 2061 2063 6f6e 6475 6374   which a conduct
-000007b0: 6976 6520 7069 7065 7474 6520 7469 7020  ive pipette tip 
-000007c0: 6973 2063 6f6e 7369 6465 7265 6420 746f  is considered to
-000007d0: 2062 6520 6174 7461 6368 6564 0d0a 2020   be attached..  
-000007e0: 2020 0d0a 2020 2020 2323 2320 5072 6f70    ..    ### Prop
-000007f0: 6572 7469 6573 0d0a 2020 2020 2d20 6063  erties..    - `c
-00000800: 6170 6163 6974 616e 6365 6020 2869 6e74  apacitance` (int
-00000810: 293a 2063 6170 6163 6974 616e 6365 2061  ): capacitance a
-00000820: 7320 6d65 6173 7572 6564 2061 7420 7468  s measured at th
-00000830: 6520 656e 6420 6f66 2074 6865 2070 6970  e end of the pip
-00000840: 6574 7465 0d0a 2020 2020 2d20 6068 6f6d  ette..    - `hom
-00000850: 655f 706f 7369 7469 6f6e 6020 2869 6e74  e_position` (int
-00000860: 293a 2068 6f6d 6520 706f 7369 7469 6f6e  ): home position
-00000870: 206f 6620 7069 7065 7474 650d 0a20 2020   of pipette..   
-00000880: 202d 2060 706f 7274 6020 2873 7472 293a   - `port` (str):
-00000890: 2043 4f4d 2070 6f72 7420 6164 6472 6573   COM port addres
-000008a0: 730d 0a20 2020 202d 2060 7265 736f 6c75  s..    - `resolu
-000008b0: 7469 6f6e 6020 2866 6c6f 6174 293a 2076  tion` (float): v
-000008c0: 6f6c 756d 6520 7265 736f 6c75 7469 6f6e  olume resolution
-000008d0: 206f 6620 7069 7065 7474 6520 2869 2e65   of pipette (i.e
-000008e0: 2e20 754c 2070 6572 2073 7465 7029 0d0a  . uL per step)..
-000008f0: 2020 2020 2d20 6073 7461 7475 7360 2028      - `status` (
-00000900: 7374 7229 3a20 7069 7065 7474 6520 7374  str): pipette st
-00000910: 6174 7573 0d0a 2020 2020 0d0a 2020 2020  atus..    ..    
-00000920: 2323 2320 4d65 7468 6f64 730d 0a20 2020  ### Methods..   
-00000930: 202d 2060 6164 6441 6972 4761 7060 3a20   - `addAirGap`: 
-00000940: 6372 6561 7465 2061 6e20 6169 7220 6761  create an air ga
-00000950: 7020 6265 7477 6565 6e20 7477 6f20 766f  p between two vo
-00000960: 6c75 6d65 7320 6f66 206c 6971 7569 6420  lumes of liquid 
-00000970: 696e 2070 6970 6574 7465 0d0a 2020 2020  in pipette..    
-00000980: 2d20 6061 7370 6972 6174 6560 3a20 6173  - `aspirate`: as
-00000990: 7069 7261 7465 2064 6573 6972 6564 2076  pirate desired v
-000009a0: 6f6c 756d 6520 6f66 2072 6561 6765 6e74  olume of reagent
-000009b0: 2069 6e74 6f20 7069 7065 7474 650d 0a20   into pipette.. 
-000009c0: 2020 202d 2060 626c 6f77 6f75 7460 3a20     - `blowout`: 
-000009d0: 626c 6f77 6f75 7420 6c69 7175 6964 2066  blowout liquid f
-000009e0: 726f 6d20 7469 700d 0a20 2020 202d 2060  rom tip..    - `
-000009f0: 6469 7370 656e 7365 603a 2064 6973 7065  dispense`: dispe
-00000a00: 6e73 6520 6465 7369 7265 6420 766f 6c75  nse desired volu
-00000a10: 6d65 206f 6620 7265 6167 656e 740d 0a20  me of reagent.. 
-00000a20: 2020 202d 2060 656a 6563 7460 3a20 656a     - `eject`: ej
-00000a30: 6563 7420 7468 6520 7069 7065 7474 6520  ect the pipette 
-00000a40: 7469 700d 0a20 2020 202d 2060 656d 7074  tip..    - `empt
-00000a50: 7960 3a20 656d 7074 7920 7468 6520 7069  y`: empty the pi
-00000a60: 7065 7474 650d 0a20 2020 202d 2060 6765  pette..    - `ge
-00000a70: 7443 6170 6163 6974 616e 6365 603a 2067  tCapacitance`: g
-00000a80: 6574 2074 6865 2063 6170 6163 6974 616e  et the capacitan
-00000a90: 6365 2061 7320 6d65 6173 7572 6564 2061  ce as measured a
-00000aa0: 7420 7468 6520 656e 6420 6f66 2074 6865  t the end of the
-00000ab0: 2070 6970 6574 7465 0d0a 2020 2020 2d20   pipette..    - 
-00000ac0: 6067 6574 4572 726f 7273 603a 2067 6574  `getErrors`: get
-00000ad0: 2065 7272 6f72 7320 6672 6f6d 2074 6865   errors from the
-00000ae0: 2064 6576 6963 650d 0a20 2020 202d 2060   device..    - `
-00000af0: 6765 7449 6e66 6f60 3a20 6765 7420 6465  getInfo`: get de
-00000b00: 7461 696c 7320 6f66 2074 6865 2053 6172  tails of the Sar
-00000b10: 746f 7269 7573 2070 6970 6574 7465 206d  torius pipette m
-00000b20: 6f64 656c 0d0a 2020 2020 2d20 6067 6574  odel..    - `get
-00000b30: 506f 7369 7469 6f6e 603a 2067 6574 2074  Position`: get t
-00000b40: 6865 2063 7572 7265 6e74 2070 6f73 6974  he current posit
-00000b50: 696f 6e20 6f66 2074 6865 2070 6970 6574  ion of the pipet
-00000b60: 7465 0d0a 2020 2020 2d20 6067 6574 5374  te..    - `getSt
-00000b70: 6174 7573 603a 2067 6574 2074 6865 2073  atus`: get the s
-00000b80: 7461 7475 7320 6f66 2074 6865 2070 6970  tatus of the pip
-00000b90: 6574 7465 0d0a 2020 2020 2d20 6068 6f6d  ette..    - `hom
-00000ba0: 6560 3a20 7265 7475 726e 2070 6c75 6e67  e`: return plung
-00000bb0: 6572 2074 6f20 686f 6d65 2070 6f73 6974  er to home posit
-00000bc0: 696f 6e0d 0a20 2020 202d 2060 6973 4665  ion..    - `isFe
-00000bd0: 6173 6962 6c65 603a 2063 6865 636b 7320  asible`: checks 
-00000be0: 616e 6420 7265 7475 726e 7320 7768 6574  and returns whet
-00000bf0: 6865 7220 7468 6520 706c 756e 6765 7220  her the plunger 
-00000c00: 706f 7369 7469 6f6e 2069 7320 6665 6173  position is feas
-00000c10: 6962 6c65 0d0a 2020 2020 2d20 6069 7354  ible..    - `isT
-00000c20: 6970 4f6e 603a 2063 6865 636b 7320 616e  ipOn`: checks an
-00000c30: 6420 7265 7475 726e 7320 7768 6574 6865  d returns whethe
-00000c40: 7220 6120 7069 7065 7474 6520 7469 7020  r a pipette tip 
-00000c50: 6973 2061 7474 6163 6865 640d 0a20 2020  is attached..   
-00000c60: 202d 2060 6d6f 7665 603a 206d 6f76 6520   - `move`: move 
-00000c70: 7468 6520 706c 756e 6765 7220 6569 7468  the plunger eith
-00000c80: 6572 2075 7020 6f72 2064 6f77 6e20 6279  er up or down by
-00000c90: 2061 2073 7065 6369 6669 6564 206e 756d   a specified num
-00000ca0: 6265 7220 6f66 2073 7465 7073 0d0a 2020  ber of steps..  
-00000cb0: 2020 2d20 606d 6f76 6542 7960 3a20 6d6f    - `moveBy`: mo
-00000cc0: 7665 2074 6865 2070 6c75 6e67 6572 2062  ve the plunger b
-00000cd0: 7920 6120 7370 6563 6966 6965 6420 6e75  y a specified nu
-00000ce0: 6d62 6572 206f 6620 7374 6570 730d 0a20  mber of steps.. 
-00000cf0: 2020 202d 2060 6d6f 7665 546f 603a 206d     - `moveTo`: m
-00000d00: 6f76 6520 7468 6520 706c 756e 6765 7220  ove the plunger 
-00000d10: 746f 2061 2073 7065 6369 6669 6564 2070  to a specified p
-00000d20: 6f73 6974 696f 6e0d 0a20 2020 202d 2060  osition..    - `
-00000d30: 7075 6c6c 6261 636b 603a 2070 756c 6c62  pullback`: pullb
-00000d40: 6163 6b20 6c69 7175 6964 2066 726f 6d20  ack liquid from 
-00000d50: 7469 700d 0a20 2020 202d 2060 7265 7365  tip..    - `rese
-00000d60: 7460 3a20 7265 7365 7420 7468 6520 7069  t`: reset the pi
-00000d70: 7065 7474 650d 0a20 2020 202d 2060 7365  pette..    - `se
-00000d80: 7453 7065 6564 603a 2073 6574 2074 6865  tSpeed`: set the
-00000d90: 2073 7065 6564 206f 6620 7468 6520 706c   speed of the pl
-00000da0: 756e 6765 720d 0a20 2020 202d 2060 7368  unger..    - `sh
-00000db0: 7574 646f 776e 603a 2073 6875 7464 6f77  utdown`: shutdow
-00000dc0: 6e20 7072 6f63 6564 7572 6520 666f 7220  n procedure for 
-00000dd0: 746f 6f6c 0d0a 2020 2020 2d20 6074 6f67  tool..    - `tog
-00000de0: 676c 6546 6565 6462 6163 6b4c 6f6f 7060  gleFeedbackLoop`
-00000df0: 3a20 7374 6172 7420 6f72 2073 746f 7020  : start or stop 
-00000e00: 6665 6564 6261 636b 206c 6f6f 700d 0a20  feedback loop.. 
-00000e10: 2020 202d 2060 7a65 726f 603a 207a 6572     - `zero`: zer
-00000e20: 6f20 7468 6520 706c 756e 6765 7220 706f  o the plunger po
-00000e30: 7369 7469 6f6e 0d0a 2020 2020 2222 220d  sition..    """.
-00000e40: 0a20 2020 200d 0a20 2020 205f 6465 6661  .    ..    _defa
-00000e50: 756c 745f 666c 6167 7320 3d20 7b0d 0a20  ult_flags = {.. 
-00000e60: 2020 2020 2020 2027 6275 7379 273a 2046         'busy': F
-00000e70: 616c 7365 2c0d 0a20 2020 2020 2020 2027  alse,..        '
-00000e80: 636f 6e64 7563 7469 7665 5f74 6970 7327  conductive_tips'
-00000e90: 3a20 4661 6c73 652c 0d0a 2020 2020 2020  : False,..      
-00000ea0: 2020 2763 6f6e 6e65 6374 6564 273a 2046    'connected': F
-00000eb0: 616c 7365 2c0d 0a20 2020 2020 2020 2027  alse,..        '
-00000ec0: 6765 745f 6665 6564 6261 636b 273a 2046  get_feedback': F
-00000ed0: 616c 7365 2c0d 0a20 2020 2020 2020 2027  alse,..        '
-00000ee0: 6f63 6375 7069 6564 273a 2046 616c 7365  occupied': False
-00000ef0: 2c0d 0a20 2020 2020 2020 2027 7061 7573  ,..        'paus
-00000f00: 655f 6665 6564 6261 636b 273a 4661 6c73  e_feedback':Fals
-00000f10: 652c 0d0a 2020 2020 2020 2020 2774 6970  e,..        'tip
-00000f20: 5f6f 6e27 3a20 4661 6c73 650d 0a20 2020  _on': False..   
-00000f30: 207d 0d0a 2020 2020 696d 706c 656d 656e   }..    implemen
-00000f40: 745f 6f66 6673 6574 203d 2028 302c 302c  t_offset = (0,0,
-00000f50: 2d32 3530 290d 0a20 2020 2074 6970 5f69  -250)..    tip_i
-00000f60: 6e73 6574 5f6d 6d20 3d20 3132 0d0a 2020  nset_mm = 12..  
-00000f70: 2020 6465 6620 5f5f 696e 6974 5f5f 2873    def __init__(s
-00000f80: 656c 662c 200d 0a20 2020 2020 2020 2070  elf, ..        p
-00000f90: 6f72 743a 7374 722c 200d 0a20 2020 2020  ort:str, ..     
-00000fa0: 2020 2063 6861 6e6e 656c 3a20 696e 7420     channel: int 
-00000fb0: 3d20 312c 200d 0a20 2020 2020 2020 206f  = 1, ..        o
-00000fc0: 6666 7365 743a 2074 7570 6c65 5b66 6c6f  ffset: tuple[flo
-00000fd0: 6174 5d20 3d20 2830 2c30 2c30 292c 0d0a  at] = (0,0,0),..
-00000fe0: 2020 2020 2020 2020 7265 7370 6f6e 7365          response
-00000ff0: 5f74 696d 653a 2066 6c6f 6174 203d 2031  _time: float = 1
-00001000: 2e30 332c 0d0a 2020 2020 2020 2020 7469  .03,..        ti
-00001010: 705f 7468 7265 7368 6f6c 643a 2069 6e74  p_threshold: int
-00001020: 203d 2032 3736 2c0d 0a20 2020 2020 2020   = 276,..       
-00001030: 202a 2a6b 7761 7267 730d 0a20 2020 2029   **kwargs..    )
-00001040: 3a0d 0a20 2020 2020 2020 2022 2222 0d0a  :..        """..
-00001050: 2020 2020 2020 2020 496e 7374 616e 7469          Instanti
-00001060: 6174 6520 7468 6520 636c 6173 730d 0a0d  ate the class...
-00001070: 0a20 2020 2020 2020 2041 7267 733a 0d0a  .        Args:..
-00001080: 2020 2020 2020 2020 2020 2020 706f 7274              port
-00001090: 2028 7374 7229 3a20 434f 4d20 706f 7274   (str): COM port
-000010a0: 2061 6464 7265 7373 0d0a 2020 2020 2020   address..      
-000010b0: 2020 2020 2020 6368 616e 6e65 6c20 2869        channel (i
-000010c0: 6e74 2c20 6f70 7469 6f6e 616c 293a 2063  nt, optional): c
-000010d0: 6861 6e6e 656c 2069 642e 2044 6566 6175  hannel id. Defau
-000010e0: 6c74 7320 746f 2031 2e0d 0a20 2020 2020  lts to 1...     
-000010f0: 2020 2020 2020 206f 6666 7365 7420 2874         offset (t
-00001100: 7570 6c65 5b66 6c6f 6174 5d2c 206f 7074  uple[float], opt
-00001110: 696f 6e61 6c29 3a20 782c 792c 7a20 6f66  ional): x,y,z of
-00001120: 6673 6574 206f 6620 7469 702e 2044 6566  fset of tip. Def
-00001130: 6175 6c74 7320 746f 2028 302c 302c 3029  aults to (0,0,0)
-00001140: 2e0d 0a20 2020 2020 2020 2020 2020 2072  ...            r
-00001150: 6573 706f 6e73 655f 7469 6d65 2028 666c  esponse_time (fl
-00001160: 6f61 742c 206f 7074 696f 6e61 6c29 3a20  oat, optional): 
-00001170: 6465 6c61 7920 6265 7477 6565 6e20 7365  delay between se
-00001180: 6e64 696e 6720 6120 636f 6d6d 616e 6420  nding a command 
-00001190: 616e 6420 7265 6365 6976 696e 6720 6120  and receiving a 
-000011a0: 7265 7370 6f6e 7365 2c20 696e 2073 6563  response, in sec
-000011b0: 6f6e 6473 2e20 4465 6661 756c 7473 2074  onds. Defaults t
-000011c0: 6f20 312e 3033 2e0d 0a20 2020 2020 2020  o 1.03...       
-000011d0: 2020 2020 2074 6970 5f74 6872 6573 686f       tip_thresho
-000011e0: 6c64 2028 696e 742c 206f 7074 696f 6e61  ld (int, optiona
-000011f0: 6c29 3a20 7468 7265 7368 6f6c 6420 6162  l): threshold ab
-00001200: 6f76 6520 7768 6963 6820 6120 636f 6e64  ove which a cond
-00001210: 7563 7469 7665 2070 6970 6574 7465 2074  uctive pipette t
-00001220: 6970 2069 7320 636f 6e73 6964 6572 6564  ip is considered
-00001230: 2074 6f20 6265 2061 7474 6163 6865 642e   to be attached.
-00001240: 2044 6566 6175 6c74 7320 746f 2032 3736   Defaults to 276
-00001250: 2e0d 0a20 2020 2020 2020 2022 2222 0d0a  ...        """..
-00001260: 2020 2020 2020 2020 7375 7065 7228 292e          super().
-00001270: 5f5f 696e 6974 5f5f 282a 2a6b 7761 7267  __init__(**kwarg
-00001280: 7329 0d0a 2020 2020 2020 2020 7365 6c66  s)..        self
-00001290: 2e63 6861 6e6e 656c 203d 2063 6861 6e6e  .channel = chann
-000012a0: 656c 0d0a 2020 2020 2020 2020 7365 6c66  el..        self
-000012b0: 2e6f 6666 7365 7420 3d20 6f66 6673 6574  .offset = offset
-000012c0: 0d0a 2020 2020 2020 2020 7365 6c66 2e72  ..        self.r
-000012d0: 6573 706f 6e73 655f 7469 6d65 203d 2072  esponse_time = r
-000012e0: 6573 706f 6e73 655f 7469 6d65 0d0a 2020  esponse_time..  
-000012f0: 2020 2020 2020 7365 6c66 2e74 6970 5f74        self.tip_t
-00001300: 6872 6573 686f 6c64 203d 2074 6970 5f74  hreshold = tip_t
-00001310: 6872 6573 686f 6c64 0d0a 2020 2020 2020  hreshold..      
-00001320: 2020 0d0a 2020 2020 2020 2020 7365 6c66    ..        self
-00001330: 2e6d 6f64 656c 5f69 6e66 6f3a 206c 6962  .model_info: lib
-00001340: 2e4d 6f64 656c 203d 204e 6f6e 650d 0a20  .Model = None.. 
-00001350: 2020 2020 2020 2073 656c 662e 6c69 6d69         self.limi
-00001360: 7473 203d 2028 302c 3029 0d0a 2020 2020  ts = (0,0)..    
-00001370: 2020 2020 7365 6c66 2e70 6f73 6974 696f      self.positio
-00001380: 6e20 3d20 300d 0a20 2020 2020 2020 2073  n = 0..        s
-00001390: 656c 662e 7370 6565 645f 636f 6465 203d  elf.speed_code =
-000013a0: 2053 7065 6564 2833 2c33 290d 0a20 2020   Speed(3,3)..   
-000013b0: 2020 2020 2073 656c 662e 7370 6565 645f       self.speed_
-000013c0: 7072 6573 6574 7320 3d20 4e6f 6e65 0d0a  presets = None..
-000013d0: 2020 2020 2020 2020 7365 6c66 2e74 6970          self.tip
-000013e0: 5f6c 656e 6774 6820 3d20 300d 0a20 2020  _length = 0..   
-000013f0: 2020 2020 200d 0a20 2020 2020 2020 2073       ..        s
-00001400: 656c 662e 5f63 6170 6163 6974 616e 6365  elf._capacitance
-00001410: 203d 2030 0d0a 2020 2020 2020 2020 7365   = 0..        se
-00001420: 6c66 2e5f 7374 6174 7573 5f63 6f64 6520  lf._status_code 
-00001430: 3d20 2727 0d0a 2020 2020 2020 2020 7365  = ''..        se
-00001440: 6c66 2e5f 7468 7265 6164 7320 3d20 7b7d  lf._threads = {}
-00001450: 0d0a 2020 2020 2020 2020 0d0a 2020 2020  ..        ..    
-00001460: 2020 2020 7072 696e 7428 2241 6e79 2061      print("Any a
-00001470: 7474 6163 6865 6420 7069 7065 7474 6520  ttached pipette 
-00001480: 7469 7020 6d61 7920 6472 6f70 2064 7572  tip may drop dur
-00001490: 696e 6720 696e 6974 6961 6c69 7361 7469  ing initialisati
-000014a0: 6f6e 2e22 290d 0a20 2020 2020 2020 2073  on.")..        s
-000014b0: 656c 662e 5f63 6f6e 6e65 6374 2870 6f72  elf._connect(por
-000014c0: 7429 0d0a 2020 2020 2020 2020 7265 7475  t)..        retu
-000014d0: 726e 0d0a 2020 2020 0d0a 2020 2020 2320  rn..    ..    # 
-000014e0: 5072 6f70 6572 7469 6573 0d0a 2020 2020  Properties..    
-000014f0: 4070 726f 7065 7274 790d 0a20 2020 2064  @property..    d
-00001500: 6566 2063 6170 6163 6974 616e 6365 2873  ef capacitance(s
-00001510: 656c 6629 202d 3e20 696e 743a 0d0a 2020  elf) -> int:..  
-00001520: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
-00001530: 662e 5f63 6170 6163 6974 616e 6365 0d0a  f._capacitance..
-00001540: 2020 2020 2020 2020 0d0a 2020 2020 4070          ..    @p
-00001550: 726f 7065 7274 790d 0a20 2020 2064 6566  roperty..    def
-00001560: 2068 6f6d 655f 706f 7369 7469 6f6e 2873   home_position(s
-00001570: 656c 6629 202d 3e20 696e 743a 0d0a 2020  elf) -> int:..  
-00001580: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
-00001590: 662e 6d6f 6465 6c5f 696e 666f 2e68 6f6d  f.model_info.hom
-000015a0: 655f 706f 7369 7469 6f6e 0d0a 2020 2020  e_position..    
-000015b0: 0d0a 2020 2020 4070 726f 7065 7274 790d  ..    @property.
-000015c0: 0a20 2020 2064 6566 2070 6f72 7428 7365  .    def port(se
-000015d0: 6c66 2920 2d3e 2073 7472 3a0d 0a20 2020  lf) -> str:..   
-000015e0: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
-000015f0: 2e63 6f6e 6e65 6374 696f 6e5f 6465 7461  .connection_deta
-00001600: 696c 732e 6765 7428 2770 6f72 7427 2c20  ils.get('port', 
-00001610: 2727 290d 0a20 2020 200d 0a20 2020 2040  '')..    ..    @
-00001620: 7072 6f70 6572 7479 0d0a 2020 2020 6465  property..    de
-00001630: 6620 7265 736f 6c75 7469 6f6e 2873 656c  f resolution(sel
-00001640: 6629 202d 3e20 666c 6f61 743a 0d0a 2020  f) -> float:..  
-00001650: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
-00001660: 662e 6d6f 6465 6c5f 696e 666f 2e72 6573  f.model_info.res
-00001670: 6f6c 7574 696f 6e0d 0a20 2020 200d 0a20  olution..    .. 
-00001680: 2020 2040 7072 6f70 6572 7479 0d0a 2020     @property..  
-00001690: 2020 6465 6620 7374 6174 7573 2873 656c    def status(sel
-000016a0: 6629 202d 3e20 7374 723a 0d0a 2020 2020  f) -> str:..    
-000016b0: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
-000016c0: 6765 7453 7461 7475 7328 290d 0a20 2020  getStatus()..   
-000016d0: 200d 0a20 2020 2064 6566 205f 5f63 7963   ..    def __cyc
-000016e0: 6c65 735f 5f28 7365 6c66 2920 2d3e 2055  les__(self) -> U
-000016f0: 6e69 6f6e 5b69 6e74 2c20 7374 725d 3a0d  nion[int, str]:.
-00001700: 0a20 2020 2020 2020 2022 2222 0d0a 2020  .        """..  
-00001710: 2020 2020 2020 5265 7472 6965 7665 2074        Retrieve t
-00001720: 6f74 616c 2063 7963 6c65 206c 6966 6574  otal cycle lifet
-00001730: 696d 650d 0a0d 0a20 2020 2020 2020 2052  ime....        R
-00001740: 6574 7572 6e73 3a0d 0a20 2020 2020 2020  eturns:..       
-00001750: 2020 2020 2055 6e69 6f6e 5b69 6e74 2c20       Union[int, 
-00001760: 7374 725d 3a20 6e75 6d62 6572 206f 6620  str]: number of 
-00001770: 6c69 6665 7469 6d65 2063 7963 6c65 732c  lifetime cycles,
-00001780: 206f 7220 7265 7370 6f6e 7365 2073 7472   or response str
-00001790: 696e 670d 0a20 2020 2020 2020 2022 2222  ing..        """
-000017a0: 0d0a 2020 2020 2020 2020 7265 7370 6f6e  ..        respon
-000017b0: 7365 203d 2073 656c 662e 5f71 7565 7279  se = self._query
-000017c0: 2827 4458 2729 0d0a 2020 2020 2020 2020  ('DX')..        
-000017d0: 7472 793a 0d0a 2020 2020 2020 2020 2020  try:..          
-000017e0: 2020 6379 636c 6573 203d 2069 6e74 2872    cycles = int(r
-000017f0: 6573 706f 6e73 6529 0d0a 2020 2020 2020  esponse)..      
-00001800: 2020 6578 6365 7074 2056 616c 7565 4572    except ValueEr
-00001810: 726f 723a 0d0a 2020 2020 2020 2020 2020  ror:..          
-00001820: 2020 7265 7475 726e 2072 6573 706f 6e73    return respons
-00001830: 650d 0a20 2020 2020 2020 2070 7269 6e74  e..        print
-00001840: 2866 2754 6f74 616c 2063 7963 6c65 733a  (f'Total cycles:
-00001850: 207b 6379 636c 6573 7d27 290d 0a20 2020   {cycles}')..   
-00001860: 2020 2020 2072 6574 7572 6e20 6379 636c       return cycl
-00001870: 6573 0d0a 2020 2020 0d0a 2020 2020 6465  es..    ..    de
-00001880: 6620 5f5f 6d6f 6465 6c5f 5f28 7365 6c66  f __model__(self
-00001890: 2920 2d3e 2073 7472 3a0d 0a20 2020 2020  ) -> str:..     
-000018a0: 2020 2022 2222 0d0a 2020 2020 2020 2020     """..        
-000018b0: 5265 7472 6965 7665 2074 6865 206d 6f64  Retrieve the mod
-000018c0: 656c 206f 6620 7468 6520 6465 7669 6365  el of the device
-000018d0: 0d0a 0d0a 2020 2020 2020 2020 5265 7475  ....        Retu
-000018e0: 726e 733a 0d0a 2020 2020 2020 2020 2020  rns:..          
-000018f0: 2020 7374 723a 206d 6f64 656c 206e 616d    str: model nam
-00001900: 650d 0a20 2020 2020 2020 2022 2222 0d0a  e..        """..
-00001910: 2020 2020 2020 2020 7265 7370 6f6e 7365          response
-00001920: 203d 2073 656c 662e 5f71 7565 7279 2827   = self._query('
-00001930: 444d 2729 0d0a 2020 2020 2020 2020 7072  DM')..        pr
-00001940: 696e 7428 6627 4d6f 6465 6c3a 207b 7265  int(f'Model: {re
-00001950: 7370 6f6e 7365 7d27 290d 0a20 2020 2020  sponse}')..     
-00001960: 2020 2072 6574 7572 6e20 7265 7370 6f6e     return respon
-00001970: 7365 0d0a 2020 2020 0d0a 2020 2020 6465  se..    ..    de
-00001980: 6620 5f5f 7265 736f 6c75 7469 6f6e 5f5f  f __resolution__
-00001990: 2873 656c 6629 202d 3e20 556e 696f 6e5b  (self) -> Union[
-000019a0: 696e 742c 2073 7472 5d3a 0d0a 2020 2020  int, str]:..    
-000019b0: 2020 2020 2222 220d 0a20 2020 2020 2020      """..       
-000019c0: 2052 6574 7269 6576 6520 7468 6520 7265   Retrieve the re
-000019d0: 736f 6c75 7469 6f6e 206f 6620 7468 6520  solution of the 
-000019e0: 6465 7669 6365 0d0a 0d0a 2020 2020 2020  device....      
-000019f0: 2020 5265 7475 726e 733a 0d0a 2020 2020    Returns:..    
-00001a00: 2020 2020 2020 2020 556e 696f 6e5b 696e          Union[in
-00001a10: 742c 2073 7472 5d3a 2076 6f6c 756d 6520  t, str]: volume 
-00001a20: 7265 736f 6c75 7469 6f6e 206f 6620 6465  resolution of de
-00001a30: 7669 6365 2069 6e20 6e4c 2c20 6f72 2072  vice in nL, or r
-00001a40: 6573 706f 6e73 6520 7374 7269 6e67 0d0a  esponse string..
-00001a50: 2020 2020 2020 2020 2222 220d 0a20 2020          """..   
-00001a60: 2020 2020 2072 6573 706f 6e73 6520 3d20       response = 
-00001a70: 7365 6c66 2e5f 7175 6572 7928 2744 5227  self._query('DR'
-00001a80: 290d 0a20 2020 2020 2020 2074 7279 3a0d  )..        try:.
-00001a90: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
-00001aa0: 6f6c 7574 696f 6e20 3d20 696e 7428 7265  olution = int(re
-00001ab0: 7370 6f6e 7365 290d 0a20 2020 2020 2020  sponse)..       
-00001ac0: 2065 7863 6570 7420 5661 6c75 6545 7272   except ValueErr
-00001ad0: 6f72 3a0d 0a20 2020 2020 2020 2020 2020  or:..           
-00001ae0: 2072 6574 7572 6e20 7265 7370 6f6e 7365   return response
-00001af0: 0d0a 2020 2020 2020 2020 7072 696e 7428  ..        print(
-00001b00: 6627 7b72 6573 6f6c 7574 696f 6e2f 3130  f'{resolution/10
-00001b10: 3030 7d20 754c 202f 2073 7465 7027 290d  00} uL / step').
-00001b20: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00001b30: 7265 736f 6c75 7469 6f6e 0d0a 2020 2020  resolution..    
-00001b40: 0d0a 2020 2020 6465 6620 5f5f 7665 7273  ..    def __vers
-00001b50: 696f 6e5f 5f28 7365 6c66 2920 2d3e 2073  ion__(self) -> s
-00001b60: 7472 3a0d 0a20 2020 2020 2020 2022 2222  tr:..        """
-00001b70: 0d0a 2020 2020 2020 2020 5265 7472 6965  ..        Retrie
-00001b80: 7665 2074 6865 2073 6f66 7477 6172 6520  ve the software 
-00001b90: 7665 7273 696f 6e20 6f6e 2074 6865 2064  version on the d
-00001ba0: 6576 6963 650d 0a0d 0a20 2020 2020 2020  evice....       
-00001bb0: 2052 6574 7572 6e73 3a0d 0a20 2020 2020   Returns:..     
-00001bc0: 2020 2020 2020 2073 7472 3a20 6465 7669         str: devi
-00001bd0: 6365 2076 6572 7369 6f6e 0d0a 2020 2020  ce version..    
-00001be0: 2020 2020 2222 220d 0a20 2020 2020 2020      """..       
-00001bf0: 2072 6574 7572 6e20 7365 6c66 2e5f 7175   return self._qu
-00001c00: 6572 7928 2744 5627 290d 0a0d 0a20 2020  ery('DV')....   
-00001c10: 2064 6566 2061 6464 4169 7247 6170 2873   def addAirGap(s
-00001c20: 656c 662c 2073 7465 7073 3a69 6e74 203d  elf, steps:int =
-00001c30: 2031 3029 202d 3e20 7374 723a 0d0a 2020   10) -> str:..  
-00001c40: 2020 2020 2020 2222 220d 0a20 2020 2020        """..     
-00001c50: 2020 2043 7265 6174 6520 616e 2061 6972     Create an air
-00001c60: 2067 6170 2062 6574 7765 656e 2074 776f   gap between two
-00001c70: 2076 6f6c 756d 6573 206f 6620 6c69 7175   volumes of liqu
-00001c80: 6964 2069 6e20 7069 7065 7474 650d 0a20  id in pipette.. 
-00001c90: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-00001ca0: 2041 7267 733a 0d0a 2020 2020 2020 2020   Args:..        
-00001cb0: 2020 2020 7374 6570 7320 2869 6e74 2c20      steps (int, 
-00001cc0: 6f70 7469 6f6e 616c 293a 206e 756d 6265  optional): numbe
-00001cd0: 7220 6f66 2073 7465 7073 2066 6f72 2061  r of steps for a
-00001ce0: 6972 2067 6170 2e20 4465 6661 756c 7473  ir gap. Defaults
-00001cf0: 2074 6f20 4445 4641 554c 545f 4149 5247   to DEFAULT_AIRG
-00001d00: 4150 2e0d 0a20 2020 2020 2020 2020 2020  AP...           
-00001d10: 2063 6861 6e6e 656c 2028 696e 742c 206f   channel (int, o
-00001d20: 7074 696f 6e61 6c29 3a20 6368 616e 6e65  ptional): channe
-00001d30: 6c20 746f 2061 6464 2061 6972 2067 6170  l to add air gap
-00001d40: 2e20 4465 6661 756c 7473 2074 6f20 4e6f  . Defaults to No
-00001d50: 6e65 2e0d 0a0d 0a20 2020 2020 2020 2052  ne.....        R
-00001d60: 6574 7572 6e73 3a0d 0a20 2020 2020 2020  eturns:..       
-00001d70: 2020 2020 2073 7472 3a20 6465 7669 6365       str: device
-00001d80: 2072 6573 706f 6e73 650d 0a20 2020 2020   response..     
-00001d90: 2020 2022 2222 0d0a 2020 2020 2020 2020     """..        
-00001da0: 7265 7370 6f6e 7365 203d 2073 656c 662e  response = self.
-00001db0: 5f71 7565 7279 2866 2752 497b 7374 6570  _query(f'RI{step
-00001dc0: 737d 2729 0d0a 2020 2020 2020 2020 7469  s}')..        ti
-00001dd0: 6d65 2e73 6c65 6570 2831 290d 0a20 2020  me.sleep(1)..   
-00001de0: 2020 2020 2072 6574 7572 6e20 7265 7370       return resp
-00001df0: 6f6e 7365 0d0a 2020 2020 2020 2020 0d0a  onse..        ..
-00001e00: 2020 2020 6465 6620 6173 7069 7261 7465      def aspirate
-00001e10: 2873 656c 662c 200d 0a20 2020 2020 2020  (self, ..       
-00001e20: 2076 6f6c 756d 653a 2066 6c6f 6174 2c20   volume: float, 
-00001e30: 0d0a 2020 2020 2020 2020 7370 6565 643a  ..        speed:
-00001e40: 204f 7074 696f 6e61 6c5b 666c 6f61 745d   Optional[float]
-00001e50: 203d 204e 6f6e 652c 200d 0a20 2020 2020   = None, ..     
-00001e60: 2020 2077 6169 743a 2069 6e74 203d 2030     wait: int = 0
-00001e70: 2c20 0d0a 2020 2020 2020 2020 7061 7573  , ..        paus
-00001e80: 653a 2062 6f6f 6c20 3d20 4661 6c73 652c  e: bool = False,
-00001e90: 200d 0a20 2020 2020 2020 2072 6561 6765   ..        reage
-00001ea0: 6e74 3a20 4f70 7469 6f6e 616c 5b73 7472  nt: Optional[str
-00001eb0: 5d20 3d20 4e6f 6e65 2c0d 0a20 2020 2020  ] = None,..     
-00001ec0: 2020 202a 2a6b 7761 7267 730d 0a20 2020     **kwargs..   
-00001ed0: 2029 202d 3e20 7374 723a 0d0a 2020 2020   ) -> str:..    
-00001ee0: 2020 2020 2222 220d 0a20 2020 2020 2020      """..       
-00001ef0: 2041 7370 6972 6174 6520 6465 7369 7265   Aspirate desire
-00001f00: 6420 766f 6c75 6d65 206f 6620 7265 6167  d volume of reag
-00001f10: 656e 740d 0a0d 0a20 2020 2020 2020 2041  ent....        A
-00001f20: 7267 733a 0d0a 2020 2020 2020 2020 2020  rgs:..          
-00001f30: 2020 766f 6c75 6d65 2028 666c 6f61 7429    volume (float)
-00001f40: 3a20 7461 7267 6574 2076 6f6c 756d 650d  : target volume.
-00001f50: 0a20 2020 2020 2020 2020 2020 2073 7065  .            spe
-00001f60: 6564 2028 4f70 7469 6f6e 616c 5b66 6c6f  ed (Optional[flo
-00001f70: 6174 5d2c 206f 7074 696f 6e61 6c29 3a20  at], optional): 
-00001f80: 7370 6565 6420 746f 2061 7370 6972 6174  speed to aspirat
-00001f90: 6520 6174 2e20 4465 6661 756c 7473 2074  e at. Defaults t
-00001fa0: 6f20 4e6f 6e65 2e0d 0a20 2020 2020 2020  o None...       
-00001fb0: 2020 2020 2077 6169 7420 2869 6e74 2c20       wait (int, 
-00001fc0: 6f70 7469 6f6e 616c 293a 2074 696d 6520  optional): time 
-00001fd0: 6465 6c61 7920 6166 7465 7220 6173 7069  delay after aspi
-00001fe0: 7261 7465 2e20 4465 6661 756c 7473 2074  rate. Defaults t
-00001ff0: 6f20 302e 0d0a 2020 2020 2020 2020 2020  o 0...          
-00002000: 2020 7061 7573 6520 2862 6f6f 6c2c 206f    pause (bool, o
-00002010: 7074 696f 6e61 6c29 3a20 7768 6574 6865  ptional): whethe
-00002020: 7220 746f 2070 6175 7365 2066 6f72 2075  r to pause for u
-00002030: 7365 7220 696e 7465 7276 656e 7469 6f6e  ser intervention
-00002040: 2e20 4465 6661 756c 7473 2074 6f20 4661  . Defaults to Fa
-00002050: 6c73 652e 0d0a 2020 2020 2020 2020 2020  lse...          
-00002060: 2020 7265 6167 656e 7420 284f 7074 696f    reagent (Optio
-00002070: 6e61 6c5b 7374 725d 2c20 6f70 7469 6f6e  nal[str], option
-00002080: 616c 293a 206e 616d 6520 6f66 2072 6561  al): name of rea
-00002090: 6765 6e74 2e20 4465 6661 756c 7473 2074  gent. Defaults t
-000020a0: 6f20 4e6f 6e65 2e0d 0a20 2020 2020 2020  o None...       
-000020b0: 2020 2020 200d 0a20 2020 2020 2020 2052       ..        R
-000020c0: 6574 7572 6e73 3a0d 0a20 2020 2020 2020  eturns:..       
-000020d0: 2020 2020 2073 7472 3a20 6465 7669 6365       str: device
-000020e0: 2072 6573 706f 6e73 650d 0a20 2020 2020   response..     
-000020f0: 2020 2022 2222 200d 0a20 2020 2020 2020     """ ..       
-00002100: 2073 656c 662e 7365 7446 6c61 6728 7061   self.setFlag(pa
-00002110: 7573 655f 6665 6564 6261 636b 3d54 7275  use_feedback=Tru
-00002120: 652c 206f 6363 7570 6965 643d 5472 7565  e, occupied=True
-00002130: 290d 0a20 2020 2020 2020 2076 6f6c 756d  )..        volum
-00002140: 6520 3d20 6d69 6e28 766f 6c75 6d65 2c20  e = min(volume, 
-00002150: 7365 6c66 2e63 6170 6163 6974 7920 2d20  self.capacity - 
-00002160: 7365 6c66 2e76 6f6c 756d 6529 0d0a 2020  self.volume)..  
-00002170: 2020 2020 2020 7374 6570 7320 3d20 696e        steps = in
-00002180: 7428 766f 6c75 6d65 202f 2073 656c 662e  t(volume / self.
-00002190: 7265 736f 6c75 7469 6f6e 290d 0a20 2020  resolution)..   
-000021a0: 2020 2020 2076 6f6c 756d 6520 3d20 7374       volume = st
-000021b0: 6570 7320 2a20 7365 6c66 2e72 6573 6f6c  eps * self.resol
-000021c0: 7574 696f 6e0d 0a20 2020 2020 2020 2069  ution..        i
-000021d0: 6620 766f 6c75 6d65 203d 3d20 303a 0d0a  f volume == 0:..
-000021e0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-000021f0: 726e 2027 270d 0a20 2020 2020 2020 2070  rn ''..        p
-00002200: 7269 6e74 2866 2741 7370 6972 6174 696e  rint(f'Aspiratin
-00002210: 6720 7b76 6f6c 756d 657d 2075 4c2e 2e2e  g {volume} uL...
-00002220: 2729 0d0a 2020 2020 2020 2020 7374 6172  ')..        star
-00002230: 745f 6173 7069 7261 7465 203d 2074 696d  t_aspirate = tim
-00002240: 652e 7065 7266 5f63 6f75 6e74 6572 2829  e.perf_counter()
-00002250: 0d0a 2020 2020 2020 2020 7370 6565 6420  ..        speed 
-00002260: 3d20 7365 6c66 2e73 7065 6564 2e75 7020  = self.speed.up 
-00002270: 6966 2073 7065 6564 2069 7320 4e6f 6e65  if speed is None
-00002280: 2065 6c73 6520 7370 6565 640d 0a20 2020   else speed..   
-00002290: 2020 2020 200d 0a20 2020 2020 2020 2069       ..        i
-000022a0: 6620 7370 6565 6420 696e 2073 656c 662e  f speed in self.
-000022b0: 7370 6565 645f 7072 6573 6574 733a 0d0a  speed_presets:..
-000022c0: 2020 2020 2020 2020 2020 2020 6966 2073              if s
-000022d0: 7065 6564 2021 3d20 7365 6c66 2e73 7065  peed != self.spe
-000022e0: 6564 2e75 703a 0d0a 2020 2020 2020 2020  ed.up:..        
-000022f0: 2020 2020 2020 2020 7365 6c66 2e73 6574          self.set
-00002300: 5370 6565 6428 7370 6565 643d 7370 6565  Speed(speed=spee
-00002310: 642c 2075 703d 5472 7565 2c20 6465 6661  d, up=True, defa
-00002320: 756c 743d 4661 6c73 6529 0d0a 2020 2020  ult=False)..    
-00002330: 2020 2020 2020 2020 7374 6172 745f 6173          start_as
-00002340: 7069 7261 7465 203d 2074 696d 652e 7065  pirate = time.pe
-00002350: 7266 5f63 6f75 6e74 6572 2829 0d0a 2020  rf_counter()..  
-00002360: 2020 2020 2020 2020 2020 7265 7370 6f6e            respon
-00002370: 7365 203d 2073 656c 662e 5f71 7565 7279  se = self._query
-00002380: 2866 2752 497b 7374 6570 737d 2729 0d0a  (f'RI{steps}')..
-00002390: 2020 2020 2020 2020 2020 2020 6d6f 7665              move
-000023a0: 5f74 696d 6520 3d20 7374 6570 732a 7365  _time = steps*se
-000023b0: 6c66 2e72 6573 6f6c 7574 696f 6e20 2f20  lf.resolution / 
-000023c0: 7370 6565 640d 0a20 2020 2020 2020 2020  speed..         
-000023d0: 2020 2064 7572 6174 696f 6e20 3d20 7469     duration = ti
-000023e0: 6d65 2e70 6572 665f 636f 756e 7465 7228  me.perf_counter(
-000023f0: 2920 2d20 7374 6172 745f 6173 7069 7261  ) - start_aspira
-00002400: 7465 0d0a 2020 2020 2020 2020 2020 2020  te..            
-00002410: 6966 2064 7572 6174 696f 6e20 3c20 286d  if duration < (m
-00002420: 6f76 655f 7469 6d65 293a 0d0a 2020 2020  ove_time):..    
-00002430: 2020 2020 2020 2020 2020 2020 7469 6d65              time
-00002440: 2e73 6c65 6570 286d 6f76 655f 7469 6d65  .sleep(move_time
-00002450: 2d64 7572 6174 696f 6e29 0d0a 2020 2020  -duration)..    
-00002460: 2020 2020 2020 2020 2320 6966 2072 6573          # if res
-00002470: 706f 6e73 6520 213d 2027 6f6b 273a 0d0a  ponse != 'ok':..
-00002480: 2020 2020 2020 2020 2020 2020 2320 2020              #   
-00002490: 2020 7265 7475 726e 2072 6573 706f 6e73    return respons
-000024a0: 650d 0a20 2020 2020 2020 2020 2020 200d  e..            .
-000024b0: 0a20 2020 2020 2020 2065 6c69 6620 7370  .        elif sp
-000024c0: 6565 6420 6e6f 7420 696e 2073 656c 662e  eed not in self.
-000024d0: 7370 6565 645f 7072 6573 6574 733a 0d0a  speed_presets:..
-000024e0: 2020 2020 2020 2020 2020 2020 7072 696e              prin
-000024f0: 7428 6622 5461 7267 6574 3a20 7b76 6f6c  t(f"Target: {vol
-00002500: 756d 657d 2075 4c20 6174 207b 7370 6565  ume} uL at {spee
-00002510: 647d 2075 4c2f 732e 2e2e 2229 0d0a 2020  d} uL/s...")..  
-00002520: 2020 2020 2020 2020 2020 7370 6565 645f            speed_
-00002530: 7061 7261 6d65 7465 7273 203d 2073 656c  parameters = sel
-00002540: 662e 5f63 616c 6375 6c61 7465 5f73 7065  f._calculate_spe
-00002550: 6564 5f70 6172 616d 6574 6572 7328 766f  ed_parameters(vo
-00002560: 6c75 6d65 3d76 6f6c 756d 652c 2073 7065  lume=volume, spe
-00002570: 6564 3d73 7065 6564 290d 0a20 2020 2020  ed=speed)..     
-00002580: 2020 2020 2020 2070 7269 6e74 2873 7065         print(spe
-00002590: 6564 5f70 6172 616d 6574 6572 7329 0d0a  ed_parameters)..
-000025a0: 2020 2020 2020 2020 2020 2020 7072 6573              pres
-000025b0: 6574 203d 2073 7065 6564 5f70 6172 616d  et = speed_param
-000025c0: 6574 6572 732e 7072 6573 6574 0d0a 2020  eters.preset..  
-000025d0: 2020 2020 2020 2020 2020 6966 2070 7265            if pre
-000025e0: 7365 7420 6973 204e 6f6e 653a 0d0a 2020  set is None:..  
-000025f0: 2020 2020 2020 2020 2020 2020 2020 2320                # 
-00002600: 7261 6973 6520 5275 6e74 696d 6545 7272  raise RuntimeErr
-00002610: 6f72 2827 5461 7267 6574 2073 7065 6564  or('Target speed
-00002620: 206e 6f74 2070 6f73 7369 626c 652e 2729   not possible.')
-00002630: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00002640: 2020 7072 696e 7428 2754 6172 6765 7420    print('Target 
-00002650: 7370 6565 6420 6e6f 7420 706f 7373 6962  speed not possib
-00002660: 6c65 2e27 290d 0a20 2020 2020 2020 2020  le.')..         
-00002670: 2020 2020 2020 2072 6574 7572 6e0d 0a20         return.. 
-00002680: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00002690: 7365 7453 7065 6564 2873 7065 6564 3d70  setSpeed(speed=p
-000026a0: 7265 7365 742c 2075 703d 5472 7565 2c20  reset, up=True, 
-000026b0: 6465 6661 756c 743d 4661 6c73 6529 0d0a  default=False)..
-000026c0: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
-000026d0: 2020 2020 2020 2020 2020 7374 6570 735f            steps_
-000026e0: 6c65 6674 203d 2073 7465 7073 0d0a 2020  left = steps..  
-000026f0: 2020 2020 2020 2020 2020 6465 6c61 7920            delay 
-00002700: 3d20 7370 6565 645f 7061 7261 6d65 7465  = speed_paramete
-00002710: 7273 2e64 656c 6179 0d0a 2020 2020 2020  rs.delay..      
-00002720: 2020 2020 2020 7374 6570 5f73 697a 6520        step_size 
-00002730: 3d20 7370 6565 645f 7061 7261 6d65 7465  = speed_paramete
-00002740: 7273 2e73 7465 705f 7369 7a65 0d0a 2020  rs.step_size..  
-00002750: 2020 2020 2020 2020 2020 696e 7465 7276            interv
-00002760: 616c 7320 3d20 7370 6565 645f 7061 7261  als = speed_para
-00002770: 6d65 7465 7273 2e69 6e74 6572 7661 6c73  meters.intervals
-00002780: 0d0a 2020 2020 2020 2020 2020 2020 7374  ..            st
-00002790: 6172 745f 6173 7069 7261 7465 203d 2074  art_aspirate = t
-000027a0: 696d 652e 7065 7266 5f63 6f75 6e74 6572  ime.perf_counter
-000027b0: 2829 0d0a 2020 2020 2020 2020 2020 2020  ()..            
-000027c0: 666f 7220 6920 696e 2072 616e 6765 2869  for i in range(i
-000027d0: 6e74 6572 7661 6c73 293a 0d0a 2020 2020  ntervals):..    
-000027e0: 2020 2020 2020 2020 2020 2020 7374 6172              star
-000027f0: 745f 7469 6d65 203d 2074 696d 652e 7065  t_time = time.pe
-00002800: 7266 5f63 6f75 6e74 6572 2829 0d0a 2020  rf_counter()..  
-00002810: 2020 2020 2020 2020 2020 2020 2020 7374                st
-00002820: 6570 203d 2073 7465 705f 7369 7a65 2069  ep = step_size i
-00002830: 6620 2869 2b31 2021 3d20 696e 7465 7276  f (i+1 != interv
-00002840: 616c 7329 2065 6c73 6520 7374 6570 735f  als) else steps_
-00002850: 6c65 6674 0d0a 2020 2020 2020 2020 2020  left..          
-00002860: 2020 2020 2020 6d6f 7665 5f74 696d 6520        move_time 
-00002870: 3d20 7374 6570 2a73 656c 662e 7265 736f  = step*self.reso
-00002880: 6c75 7469 6f6e 202f 2070 7265 7365 740d  lution / preset.
-00002890: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000028a0: 2072 6573 706f 6e73 6520 3d20 7365 6c66   response = self
-000028b0: 2e5f 7175 6572 7928 6627 5249 7b73 7465  ._query(f'RI{ste
-000028c0: 707d 272c 2072 6573 756d 655f 6665 6564  p}', resume_feed
-000028d0: 6261 636b 3d46 616c 7365 2c20 6765 745f  back=False, get_
-000028e0: 706f 7369 7469 6f6e 3d46 616c 7365 290d  position=False).
-000028f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002900: 2023 2069 6620 7265 7370 6f6e 7365 2021   # if response !
-00002910: 3d20 276f 6b27 3a0d 0a20 2020 2020 2020  = 'ok':..       
-00002920: 2020 2020 2020 2020 2023 2020 2020 2070           #     p
-00002930: 7269 6e74 2822 4173 7069 7261 7469 6f6e  rint("Aspiration
-00002940: 2066 6169 6c65 6422 290d 0a20 2020 2020   failed")..     
-00002950: 2020 2020 2020 2020 2020 2023 2020 2020             #    
-00002960: 2072 6574 7572 6e20 7265 7370 6f6e 7365   return response
-00002970: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00002980: 2020 7374 6570 735f 6c65 6674 202d 3d20    steps_left -= 
-00002990: 7374 6570 0d0a 2020 2020 2020 2020 2020  step..          
-000029a0: 2020 2020 2020 6475 7261 7469 6f6e 203d        duration =
-000029b0: 2074 696d 652e 7065 7266 5f63 6f75 6e74   time.perf_count
-000029c0: 6572 2829 202d 2073 7461 7274 5f74 696d  er() - start_tim
-000029d0: 650d 0a20 2020 2020 2020 2020 2020 2020  e..             
-000029e0: 2020 2069 6620 6475 7261 7469 6f6e 203c     if duration <
-000029f0: 2028 6465 6c61 792b 6d6f 7665 5f74 696d   (delay+move_tim
-00002a00: 6529 3a0d 0a20 2020 2020 2020 2020 2020  e):..           
-00002a10: 2020 2020 2020 2020 2074 696d 652e 736c           time.sl
-00002a20: 6565 7028 6465 6c61 792b 6d6f 7665 5f74  eep(delay+move_t
-00002a30: 696d 652d 6475 7261 7469 6f6e 290d 0a20  ime-duration).. 
-00002a40: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-00002a50: 2023 2055 7064 6174 6520 7661 6c75 6573   # Update values
-00002a60: 0d0a 2020 2020 2020 2020 7072 696e 7428  ..        print(
-00002a70: 6627 4173 7069 7261 7469 6f6e 2074 696d  f'Aspiration tim
-00002a80: 653a 207b 7469 6d65 2e70 6572 665f 636f  e: {time.perf_co
-00002a90: 756e 7465 7228 292d 7374 6172 745f 6173  unter()-start_as
-00002aa0: 7069 7261 7465 7d73 2729 0d0a 2020 2020  pirate}s')..    
-00002ab0: 2020 2020 7469 6d65 2e73 6c65 6570 2877      time.sleep(w
-00002ac0: 6169 7429 0d0a 2020 2020 2020 2020 7365  ait)..        se
-00002ad0: 6c66 2e73 6574 466c 6167 286f 6363 7570  lf.setFlag(occup
-00002ae0: 6965 643d 4661 6c73 652c 2070 6175 7365  ied=False, pause
-00002af0: 5f66 6565 6462 6163 6b3d 4661 6c73 6529  _feedback=False)
-00002b00: 0d0a 2020 2020 2020 2020 7365 6c66 2e67  ..        self.g
-00002b10: 6574 506f 7369 7469 6f6e 2829 0d0a 2020  etPosition()..  
-00002b20: 2020 2020 2020 7365 6c66 2e76 6f6c 756d        self.volum
-00002b30: 6520 2b3d 2076 6f6c 756d 650d 0a20 2020  e += volume..   
-00002b40: 2020 2020 2073 656c 662e 706f 7369 7469       self.positi
-00002b50: 6f6e 202b 3d20 7374 6570 730d 0a20 2020  on += steps..   
-00002b60: 2020 2020 2069 6620 7265 6167 656e 7420       if reagent 
-00002b70: 6973 206e 6f74 204e 6f6e 653a 0d0a 2020  is not None:..  
-00002b80: 2020 2020 2020 2020 2020 7365 6c66 2e72            self.r
-00002b90: 6561 6765 6e74 203d 2072 6561 6765 6e74  eagent = reagent
-00002ba0: 0d0a 2020 2020 2020 2020 6966 2070 6175  ..        if pau
-00002bb0: 7365 3a0d 0a20 2020 2020 2020 2020 2020  se:..           
-00002bc0: 2069 6e70 7574 2822 5072 6573 7320 2745   input("Press 'E
-00002bd0: 6e74 6572 2720 746f 2070 726f 6365 6564  nter' to proceed
-00002be0: 2e22 290d 0a20 2020 2020 2020 2072 6574  .")..        ret
-00002bf0: 7572 6e20 7265 7370 6f6e 7365 0d0a 2020  urn response..  
-00002c00: 2020 0d0a 2020 2020 6465 6620 626c 6f77    ..    def blow
-00002c10: 6f75 7428 7365 6c66 2c20 686f 6d65 3a62  out(self, home:b
-00002c20: 6f6f 6c20 3d20 5472 7565 2c20 2a2a 6b77  ool = True, **kw
-00002c30: 6172 6773 2920 2d3e 2073 7472 3a0d 0a20  args) -> str:.. 
-00002c40: 2020 2020 2020 2022 2222 0d0a 2020 2020         """..    
-00002c50: 2020 2020 426c 6f77 6f75 7420 6c69 7175      Blowout liqu
-00002c60: 6964 2066 726f 6d20 7469 700d 0a0d 0a20  id from tip.... 
-00002c70: 2020 2020 2020 2041 7267 733a 0d0a 2020         Args:..  
-00002c80: 2020 2020 2020 2020 2020 686f 6d65 2028            home (
-00002c90: 626f 6f6c 2c20 6f70 7469 6f6e 616c 293a  bool, optional):
-00002ca0: 2077 6865 7468 6572 2074 6f20 7265 7475   whether to retu
-00002cb0: 726e 2070 6c75 6e67 6572 2074 6f20 686f  rn plunger to ho
-00002cc0: 6d65 2070 6f73 6974 696f 6e2e 2044 6566  me position. Def
-00002cd0: 6175 6c74 7320 746f 2054 7275 652e 0d0a  aults to True...
-00002ce0: 0d0a 2020 2020 2020 2020 5265 7475 726e  ..        Return
-00002cf0: 733a 0d0a 2020 2020 2020 2020 2020 2020  s:..            
-00002d00: 7374 723a 2064 6576 6963 6520 7265 7370  str: device resp
-00002d10: 6f6e 7365 0d0a 2020 2020 2020 2020 2222  onse..        ""
-00002d20: 220d 0a20 2020 2020 2020 2063 6f6d 6d61  "..        comma
-00002d30: 6e64 203d 2066 2752 427b 7365 6c66 2e68  nd = f'RB{self.h
-00002d40: 6f6d 655f 706f 7369 7469 6f6e 7d27 2069  ome_position}' i
-00002d50: 6620 686f 6d65 2065 6c73 6520 2752 4227  f home else 'RB'
-00002d60: 0d0a 2020 2020 2020 2020 7265 7370 6f6e  ..        respon
-00002d70: 7365 203d 2073 656c 662e 5f71 7565 7279  se = self._query
-00002d80: 2863 6f6d 6d61 6e64 290d 0a20 2020 2020  (command)..     
-00002d90: 2020 2073 656c 662e 706f 7369 7469 6f6e     self.position
-00002da0: 203d 2073 656c 662e 686f 6d65 5f70 6f73   = self.home_pos
-00002db0: 6974 696f 6e0d 0a20 2020 2020 2020 2074  ition..        t
-00002dc0: 696d 652e 736c 6565 7028 3129 0d0a 2020  ime.sleep(1)..  
-00002dd0: 2020 2020 2020 7265 7475 726e 2072 6573        return res
-00002de0: 706f 6e73 650d 0a20 2020 200d 0a20 2020  ponse..    ..   
-00002df0: 2064 6566 2064 6973 7065 6e73 6528 7365   def dispense(se
-00002e00: 6c66 2c20 0d0a 2020 2020 2020 2020 766f  lf, ..        vo
-00002e10: 6c75 6d65 3a20 666c 6f61 742c 200d 0a20  lume: float, .. 
-00002e20: 2020 2020 2020 2073 7065 6564 3a20 4f70         speed: Op
-00002e30: 7469 6f6e 616c 5b66 6c6f 6174 5d20 3d20  tional[float] = 
-00002e40: 4e6f 6e65 2c20 0d0a 2020 2020 2020 2020  None, ..        
-00002e50: 7761 6974 3a20 696e 7420 3d20 302c 200d  wait: int = 0, .
-00002e60: 0a20 2020 2020 2020 2070 6175 7365 3a20  .        pause: 
-00002e70: 626f 6f6c 203d 2046 616c 7365 2c20 0d0a  bool = False, ..
-00002e80: 2020 2020 2020 2020 626c 6f77 6f75 743a          blowout:
-00002e90: 2062 6f6f 6c20 3d20 4661 6c73 652c 0d0a   bool = False,..
-00002ea0: 2020 2020 2020 2020 626c 6f77 6f75 745f          blowout_
-00002eb0: 686f 6d65 3a20 626f 6f6c 203d 2054 7275  home: bool = Tru
-00002ec0: 652c 0d0a 2020 2020 2020 2020 666f 7263  e,..        forc
-00002ed0: 655f 6469 7370 656e 7365 3a20 626f 6f6c  e_dispense: bool
-00002ee0: 203d 2046 616c 7365 2c20 0d0a 2020 2020   = False, ..    
-00002ef0: 2020 2020 2a2a 6b77 6172 6773 0d0a 2020      **kwargs..  
-00002f00: 2020 2920 2d3e 2073 7472 3a0d 0a20 2020    ) -> str:..   
-00002f10: 2020 2020 2022 2222 0d0a 2020 2020 2020       """..      
-00002f20: 2020 4469 7370 656e 7365 2064 6573 6972    Dispense desir
-00002f30: 6564 2076 6f6c 756d 6520 6f66 2072 6561  ed volume of rea
-00002f40: 6765 6e74 0d0a 0d0a 2020 2020 2020 2020  gent....        
-00002f50: 4172 6773 3a0d 0a20 2020 2020 2020 2020  Args:..         
-00002f60: 2020 2076 6f6c 756d 6520 2866 6c6f 6174     volume (float
-00002f70: 293a 2074 6172 6765 7420 766f 6c75 6d65  ): target volume
-00002f80: 0d0a 2020 2020 2020 2020 2020 2020 7370  ..            sp
-00002f90: 6565 6420 284f 7074 696f 6e61 6c5b 666c  eed (Optional[fl
-00002fa0: 6f61 745d 2c20 6f70 7469 6f6e 616c 293a  oat], optional):
-00002fb0: 2073 7065 6564 2074 6f20 6469 7370 656e   speed to dispen
-00002fc0: 7365 2061 742e 2044 6566 6175 6c74 7320  se at. Defaults 
-00002fd0: 746f 204e 6f6e 652e 0d0a 2020 2020 2020  to None...      
-00002fe0: 2020 2020 2020 7761 6974 2028 696e 742c        wait (int,
-00002ff0: 206f 7074 696f 6e61 6c29 3a20 7469 6d65   optional): time
-00003000: 2064 656c 6179 2061 6674 6572 2064 6973   delay after dis
-00003010: 7065 6e73 652e 2044 6566 6175 6c74 7320  pense. Defaults 
-00003020: 746f 2030 2e0d 0a20 2020 2020 2020 2020  to 0...         
-00003030: 2020 2070 6175 7365 2028 626f 6f6c 2c20     pause (bool, 
-00003040: 6f70 7469 6f6e 616c 293a 2077 6865 7468  optional): wheth
-00003050: 6572 2074 6f20 7061 7573 6520 666f 7220  er to pause for 
-00003060: 7573 6572 2069 6e74 6572 7665 6e74 696f  user interventio
-00003070: 6e2e 2044 6566 6175 6c74 7320 746f 2046  n. Defaults to F
-00003080: 616c 7365 2e0d 0a20 2020 2020 2020 2020  alse...         
-00003090: 2020 2062 6c6f 776f 7574 2028 626f 6f6c     blowout (bool
-000030a0: 2c20 6f70 7469 6f6e 616c 293a 2077 6865  , optional): whe
-000030b0: 7468 6572 2070 6572 666f 726d 2062 6c6f  ther perform blo
-000030c0: 776f 7574 2e20 4465 6661 756c 7473 2074  wout. Defaults t
-000030d0: 6f20 4661 6c73 652e 0d0a 2020 2020 2020  o False...      
-000030e0: 2020 2020 2020 626c 6f77 6f75 745f 686f        blowout_ho
-000030f0: 6d65 2028 626f 6f6c 2c20 6f70 7469 6f6e  me (bool, option
-00003100: 616c 293a 2077 6865 7468 6572 2074 6f20  al): whether to 
-00003110: 7265 7475 726e 2074 6865 2070 6c75 6e67  return the plung
-00003120: 6572 2068 6f6d 6520 6166 7465 7220 626c  er home after bl
-00003130: 6f77 6f75 742e 2044 6566 6175 6c74 7320  owout. Defaults 
-00003140: 746f 2054 7275 652e 0d0a 2020 2020 2020  to True...      
-00003150: 2020 2020 2020 666f 7263 655f 6469 7370        force_disp
-00003160: 656e 7365 2028 626f 6f6c 2c20 6f70 7469  ense (bool, opti
-00003170: 6f6e 616c 293a 2077 6865 7468 6572 2074  onal): whether t
-00003180: 6f20 6469 7370 656e 7365 2072 6561 6765  o dispense reage
-00003190: 6e74 2072 6567 6172 646c 6573 732e 2044  nt regardless. D
-000031a0: 6566 6175 6c74 7320 746f 2046 616c 7365  efaults to False
-000031b0: 2e0d 0a0d 0a20 2020 2020 2020 2052 6169  .....        Rai
-000031c0: 7365 733a 0d0a 2020 2020 2020 2020 2020  ses:..          
-000031d0: 2020 5661 6c75 6545 7272 6f72 3a20 5265    ValueError: Re
-000031e0: 7175 6972 6564 2064 6973 7065 6e73 6520  quired dispense 
-000031f0: 766f 6c75 6d65 2069 7320 6772 6561 7465  volume is greate
-00003200: 7220 7468 616e 2076 6f6c 756d 6520 696e  r than volume in
-00003210: 2074 6970 0d0a 0d0a 2020 2020 2020 2020   tip....        
-00003220: 5265 7475 726e 733a 0d0a 2020 2020 2020  Returns:..      
-00003230: 2020 2020 2020 7374 723a 2064 6576 6963        str: devic
-00003240: 6520 7265 7370 6f6e 7365 0d0a 2020 2020  e response..    
-00003250: 2020 2020 2222 220d 0a20 2020 2020 2020      """..       
-00003260: 2073 656c 662e 7365 7446 6c61 6728 7061   self.setFlag(pa
-00003270: 7573 655f 6665 6564 6261 636b 3d54 7275  use_feedback=Tru
-00003280: 652c 206f 6363 7570 6965 643d 5472 7565  e, occupied=True
-00003290: 290d 0a20 2020 2020 2020 2069 6620 666f  )..        if fo
-000032a0: 7263 655f 6469 7370 656e 7365 3a0d 0a20  rce_dispense:.. 
-000032b0: 2020 2020 2020 2020 2020 2076 6f6c 756d             volum
-000032c0: 6520 3d20 6d69 6e28 766f 6c75 6d65 2c20  e = min(volume, 
-000032d0: 7365 6c66 2e76 6f6c 756d 6529 0d0a 2020  self.volume)..  
-000032e0: 2020 2020 2020 656c 6966 2076 6f6c 756d        elif volum
-000032f0: 6520 3e20 7365 6c66 2e76 6f6c 756d 653a  e > self.volume:
-00003300: 0d0a 2020 2020 2020 2020 2020 2020 7261  ..            ra
-00003310: 6973 6520 5661 6c75 6545 7272 6f72 2827  ise ValueError('
-00003320: 5265 7175 6972 6564 2064 6973 7065 6e73  Required dispens
-00003330: 6520 766f 6c75 6d65 2069 7320 6772 6561  e volume is grea
-00003340: 7465 7220 7468 616e 2076 6f6c 756d 6520  ter than volume 
-00003350: 696e 2074 6970 2e27 290d 0a20 2020 2020  in tip.')..     
-00003360: 2020 2073 7465 7073 203d 2069 6e74 2876     steps = int(v
-00003370: 6f6c 756d 6520 2f20 7365 6c66 2e72 6573  olume / self.res
-00003380: 6f6c 7574 696f 6e29 0d0a 2020 2020 2020  olution)..      
-00003390: 2020 766f 6c75 6d65 203d 2073 7465 7073    volume = steps
-000033a0: 202a 2073 656c 662e 7265 736f 6c75 7469   * self.resoluti
-000033b0: 6f6e 0d0a 2020 2020 2020 2020 6966 2076  on..        if v
-000033c0: 6f6c 756d 6520 3d3d 2030 3a0d 0a20 2020  olume == 0:..   
-000033d0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-000033e0: 2727 0d0a 2020 2020 2020 2020 7072 696e  ''..        prin
-000033f0: 7428 6627 4469 7370 656e 7369 6e67 207b  t(f'Dispensing {
-00003400: 766f 6c75 6d65 7d20 754c 2e2e 2e27 290d  volume} uL...').
-00003410: 0a20 2020 2020 2020 2073 7461 7274 5f64  .        start_d
-00003420: 6973 7065 6e73 6520 3d20 7469 6d65 2e70  ispense = time.p
-00003430: 6572 665f 636f 756e 7465 7228 290d 0a20  erf_counter().. 
-00003440: 2020 2020 2020 2073 7065 6564 203d 2073         speed = s
-00003450: 656c 662e 7370 6565 642e 646f 776e 2069  elf.speed.down i
-00003460: 6620 7370 6565 6420 6973 204e 6f6e 6520  f speed is None 
-00003470: 656c 7365 2073 7065 6564 0d0a 0d0a 2020  else speed....  
-00003480: 2020 2020 2020 6966 2073 7065 6564 2069        if speed i
-00003490: 6e20 7365 6c66 2e73 7065 6564 5f70 7265  n self.speed_pre
-000034a0: 7365 7473 3a0d 0a20 2020 2020 2020 2020  sets:..         
-000034b0: 2020 2069 6620 7370 6565 6420 213d 2073     if speed != s
-000034c0: 656c 662e 7370 6565 642e 646f 776e 3a0d  elf.speed.down:.
-000034d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000034e0: 2073 656c 662e 7365 7453 7065 6564 2873   self.setSpeed(s
-000034f0: 7065 6564 3d73 7065 6564 2c20 7570 3d46  peed=speed, up=F
-00003500: 616c 7365 2c20 6465 6661 756c 743d 4661  alse, default=Fa
-00003510: 6c73 6529 0d0a 2020 2020 2020 2020 2020  lse)..          
-00003520: 2020 7374 6172 745f 6469 7370 656e 7365    start_dispense
-00003530: 203d 2074 696d 652e 7065 7266 5f63 6f75   = time.perf_cou
-00003540: 6e74 6572 2829 0d0a 2020 2020 2020 2020  nter()..        
-00003550: 2020 2020 7265 7370 6f6e 7365 203d 2073      response = s
-00003560: 656c 662e 5f71 7565 7279 2866 2752 4f7b  elf._query(f'RO{
-00003570: 7374 6570 737d 2729 0d0a 2020 2020 2020  steps}')..      
-00003580: 2020 2020 2020 6d6f 7665 5f74 696d 6520        move_time 
-00003590: 3d20 7374 6570 732a 7365 6c66 2e72 6573  = steps*self.res
-000035a0: 6f6c 7574 696f 6e20 2f20 7370 6565 640d  olution / speed.
-000035b0: 0a20 2020 2020 2020 2020 2020 2064 7572  .            dur
-000035c0: 6174 696f 6e20 3d20 7469 6d65 2e70 6572  ation = time.per
-000035d0: 665f 636f 756e 7465 7228 2920 2d20 7374  f_counter() - st
-000035e0: 6172 745f 6469 7370 656e 7365 0d0a 2020  art_dispense..  
-000035f0: 2020 2020 2020 2020 2020 6966 2064 7572            if dur
-00003600: 6174 696f 6e20 3c20 286d 6f76 655f 7469  ation < (move_ti
-00003610: 6d65 293a 0d0a 2020 2020 2020 2020 2020  me):..          
-00003620: 2020 2020 2020 7469 6d65 2e73 6c65 6570        time.sleep
-00003630: 286d 6f76 655f 7469 6d65 2d64 7572 6174  (move_time-durat
-00003640: 696f 6e29 0d0a 2020 2020 2020 2020 2020  ion)..          
-00003650: 2020 2320 6966 2072 6573 706f 6e73 6520    # if response 
-00003660: 213d 2027 6f6b 273a 0d0a 2020 2020 2020  != 'ok':..      
-00003670: 2020 2020 2020 2320 2020 2020 7265 7475        #     retu
-00003680: 726e 2072 6573 706f 6e73 650d 0a20 2020  rn response..   
-00003690: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
-000036a0: 2020 2065 6c69 6620 7370 6565 6420 6e6f     elif speed no
-000036b0: 7420 696e 2073 656c 662e 7370 6565 645f  t in self.speed_
-000036c0: 7072 6573 6574 733a 0d0a 2020 2020 2020  presets:..      
-000036d0: 2020 2020 2020 7072 696e 7428 6622 5461        print(f"Ta
-000036e0: 7267 6574 3a20 7b76 6f6c 756d 657d 2075  rget: {volume} u
-000036f0: 4c20 6174 207b 7370 6565 647d 2075 4c2f  L at {speed} uL/
-00003700: 732e 2e2e 2229 0d0a 2020 2020 2020 2020  s...")..        
-00003710: 2020 2020 7370 6565 645f 7061 7261 6d65      speed_parame
-00003720: 7465 7273 203d 2073 656c 662e 5f63 616c  ters = self._cal
-00003730: 6375 6c61 7465 5f73 7065 6564 5f70 6172  culate_speed_par
-00003740: 616d 6574 6572 7328 766f 6c75 6d65 3d76  ameters(volume=v
-00003750: 6f6c 756d 652c 2073 7065 6564 3d73 7065  olume, speed=spe
-00003760: 6564 290d 0a20 2020 2020 2020 2020 2020  ed)..           
-00003770: 2070 7269 6e74 2873 7065 6564 5f70 6172   print(speed_par
-00003780: 616d 6574 6572 7329 0d0a 2020 2020 2020  ameters)..      
-00003790: 2020 2020 2020 7072 6573 6574 203d 2073        preset = s
-000037a0: 7065 6564 5f70 6172 616d 6574 6572 732e  peed_parameters.
-000037b0: 7072 6573 6574 0d0a 2020 2020 2020 2020  preset..        
-000037c0: 2020 2020 6966 2070 7265 7365 7420 6973      if preset is
-000037d0: 204e 6f6e 653a 0d0a 2020 2020 2020 2020   None:..        
-000037e0: 2020 2020 2020 2020 2320 7261 6973 6520          # raise 
-000037f0: 5275 6e74 696d 6545 7272 6f72 2827 5461  RuntimeError('Ta
-00003800: 7267 6574 2073 7065 6564 206e 6f74 2070  rget speed not p
-00003810: 6f73 7369 626c 652e 2729 0d0a 2020 2020  ossible.')..    
-00003820: 2020 2020 2020 2020 2020 2020 7072 696e              prin
-00003830: 7428 2754 6172 6765 7420 7370 6565 6420  t('Target speed 
-00003840: 6e6f 7420 706f 7373 6962 6c65 2e27 290d  not possible.').
-00003850: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00003860: 2072 6574 7572 6e0d 0a20 2020 2020 2020   return..       
-00003870: 2020 2020 2073 656c 662e 7365 7453 7065       self.setSpe
-00003880: 6564 2873 7065 6564 3d70 7265 7365 742c  ed(speed=preset,
-00003890: 2075 703d 4661 6c73 652c 2064 6566 6175   up=False, defau
-000038a0: 6c74 3d46 616c 7365 290d 0a20 2020 2020  lt=False)..     
-000038b0: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
-000038c0: 2073 7465 7073 5f6c 6566 7420 3d20 7374   steps_left = st
-000038d0: 6570 730d 0a20 2020 2020 2020 2020 2020  eps..           
-000038e0: 2064 656c 6179 203d 2073 7065 6564 5f70   delay = speed_p
-000038f0: 6172 616d 6574 6572 732e 6465 6c61 790d  arameters.delay.
-00003900: 0a20 2020 2020 2020 2020 2020 2073 7465  .            ste
-00003910: 705f 7369 7a65 203d 2073 7065 6564 5f70  p_size = speed_p
-00003920: 6172 616d 6574 6572 732e 7374 6570 5f73  arameters.step_s
-00003930: 697a 650d 0a20 2020 2020 2020 2020 2020  ize..           
-00003940: 2069 6e74 6572 7661 6c73 203d 2073 7065   intervals = spe
-00003950: 6564 5f70 6172 616d 6574 6572 732e 696e  ed_parameters.in
-00003960: 7465 7276 616c 730d 0a20 2020 2020 2020  tervals..       
-00003970: 2020 2020 2073 7461 7274 5f64 6973 7065       start_dispe
-00003980: 6e73 6520 3d20 7469 6d65 2e70 6572 665f  nse = time.perf_
-00003990: 636f 756e 7465 7228 290d 0a20 2020 2020  counter()..     
-000039a0: 2020 2020 2020 2066 6f72 2069 2069 6e20         for i in 
-000039b0: 7261 6e67 6528 696e 7465 7276 616c 7329  range(intervals)
-000039c0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-000039d0: 2020 2073 7461 7274 5f74 696d 6520 3d20     start_time = 
-000039e0: 7469 6d65 2e70 6572 665f 636f 756e 7465  time.perf_counte
-000039f0: 7228 290d 0a20 2020 2020 2020 2020 2020  r()..           
-00003a00: 2020 2020 2073 7465 7020 3d20 7374 6570       step = step
-00003a10: 5f73 697a 6520 6966 2028 692b 3120 213d  _size if (i+1 !=
-00003a20: 2069 6e74 6572 7661 6c73 2920 656c 7365   intervals) else
-00003a30: 2073 7465 7073 5f6c 6566 740d 0a20 2020   steps_left..   
-00003a40: 2020 2020 2020 2020 2020 2020 206d 6f76               mov
-00003a50: 655f 7469 6d65 203d 2073 7465 702a 7365  e_time = step*se
-00003a60: 6c66 2e72 6573 6f6c 7574 696f 6e20 2f20  lf.resolution / 
-00003a70: 7072 6573 6574 0d0a 2020 2020 2020 2020  preset..        
-00003a80: 2020 2020 2020 2020 7265 7370 6f6e 7365          response
-00003a90: 203d 2073 656c 662e 5f71 7565 7279 2866   = self._query(f
-00003aa0: 2752 4f7b 7374 6570 7d27 2c20 7265 7375  'RO{step}', resu
-00003ab0: 6d65 5f66 6565 6462 6163 6b3d 4661 6c73  me_feedback=Fals
-00003ac0: 652c 2067 6574 5f70 6f73 6974 696f 6e3d  e, get_position=
-00003ad0: 4661 6c73 6529 0d0a 2020 2020 2020 2020  False)..        
-00003ae0: 2020 2020 2020 2020 2320 6966 2072 6573          # if res
-00003af0: 706f 6e73 6520 213d 2027 6f6b 273a 0d0a  ponse != 'ok':..
-00003b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003b10: 2320 2020 2020 7072 696e 7428 2244 6973  #     print("Dis
-00003b20: 7065 6e73 6520 6661 696c 6564 2229 0d0a  pense failed")..
-00003b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003b40: 2320 2020 2020 7265 7475 726e 2072 6573  #     return res
-00003b50: 706f 6e73 650d 0a20 2020 2020 2020 2020  ponse..         
-00003b60: 2020 2020 2020 2073 7465 7073 5f6c 6566         steps_lef
-00003b70: 7420 2d3d 2073 7465 700d 0a20 2020 2020  t -= step..     
-00003b80: 2020 2020 2020 2020 2020 2064 7572 6174             durat
-00003b90: 696f 6e20 3d20 7469 6d65 2e70 6572 665f  ion = time.perf_
-00003ba0: 636f 756e 7465 7228 2920 2d20 7374 6172  counter() - star
-00003bb0: 745f 7469 6d65 0d0a 2020 2020 2020 2020  t_time..        
-00003bc0: 2020 2020 2020 2020 6966 2064 7572 6174          if durat
-00003bd0: 696f 6e20 3c20 2864 656c 6179 2b6d 6f76  ion < (delay+mov
-00003be0: 655f 7469 6d65 293a 0d0a 2020 2020 2020  e_time):..      
-00003bf0: 2020 2020 2020 2020 2020 2020 2020 7469                ti
-00003c00: 6d65 2e73 6c65 6570 2864 656c 6179 2b6d  me.sleep(delay+m
-00003c10: 6f76 655f 7469 6d65 2d64 7572 6174 696f  ove_time-duratio
-00003c20: 6e29 0d0a 0d0a 2020 2020 2020 2020 2320  n)....        # 
-00003c30: 5570 6461 7465 2076 616c 7565 730d 0a20  Update values.. 
-00003c40: 2020 2020 2020 2070 7269 6e74 2866 2744         print(f'D
-00003c50: 6973 7065 6e73 6520 7469 6d65 3a20 7b74  ispense time: {t
-00003c60: 696d 652e 7065 7266 5f63 6f75 6e74 6572  ime.perf_counter
-00003c70: 2829 2d73 7461 7274 5f64 6973 7065 6e73  ()-start_dispens
-00003c80: 657d 7327 290d 0a20 2020 2020 2020 2074  e}s')..        t
-00003c90: 696d 652e 736c 6565 7028 7761 6974 290d  ime.sleep(wait).
-00003ca0: 0a20 2020 2020 2020 2073 656c 662e 7365  .        self.se
-00003cb0: 7446 6c61 6728 6f63 6375 7069 6564 3d46  tFlag(occupied=F
-00003cc0: 616c 7365 2c20 7061 7573 655f 6665 6564  alse, pause_feed
-00003cd0: 6261 636b 3d46 616c 7365 290d 0a20 2020  back=False)..   
-00003ce0: 2020 2020 2073 656c 662e 6765 7450 6f73       self.getPos
-00003cf0: 6974 696f 6e28 290d 0a20 2020 2020 2020  ition()..       
-00003d00: 2073 656c 662e 766f 6c75 6d65 203d 206d   self.volume = m
-00003d10: 6178 2873 656c 662e 766f 6c75 6d65 202d  ax(self.volume -
-00003d20: 2076 6f6c 756d 652c 2030 290d 0a20 2020   volume, 0)..   
-00003d30: 2020 2020 2073 656c 662e 706f 7369 7469       self.positi
-00003d40: 6f6e 202d 3d20 7374 6570 730d 0a20 2020  on -= steps..   
-00003d50: 2020 2020 2069 6620 7365 6c66 2e76 6f6c       if self.vol
-00003d60: 756d 6520 3d3d 2030 2061 6e64 2062 6c6f  ume == 0 and blo
-00003d70: 776f 7574 3a0d 0a20 2020 2020 2020 2020  wout:..         
-00003d80: 2020 2073 656c 662e 626c 6f77 6f75 7428     self.blowout(
-00003d90: 686f 6d65 3d62 6c6f 776f 7574 5f68 6f6d  home=blowout_hom
-00003da0: 6529 0d0a 2020 2020 2020 2020 6966 2070  e)..        if p
-00003db0: 6175 7365 3a0d 0a20 2020 2020 2020 2020  ause:..         
-00003dc0: 2020 2069 6e70 7574 2822 5072 6573 7320     input("Press 
-00003dd0: 2745 6e74 6572 2720 746f 2070 726f 6365  'Enter' to proce
-00003de0: 6564 2e22 290d 0a20 2020 2020 2020 2072  ed.")..        r
-00003df0: 6574 7572 6e20 7265 7370 6f6e 7365 0d0a  eturn response..
-00003e00: 2020 2020 0d0a 2020 2020 6465 6620 656a      ..    def ej
-00003e10: 6563 7428 7365 6c66 2c20 686f 6d65 3a62  ect(self, home:b
-00003e20: 6f6f 6c20 3d20 5472 7565 2920 2d3e 2073  ool = True) -> s
-00003e30: 7472 3a0d 0a20 2020 2020 2020 2022 2222  tr:..        """
-00003e40: 0d0a 2020 2020 2020 2020 456a 6563 7420  ..        Eject 
-00003e50: 7468 6520 7069 7065 7474 6520 7469 700d  the pipette tip.
-00003e60: 0a0d 0a20 2020 2020 2020 2041 7267 733a  ...        Args:
-00003e70: 0d0a 2020 2020 2020 2020 2020 2020 686f  ..            ho
-00003e80: 6d65 2028 626f 6f6c 2c20 6f70 7469 6f6e  me (bool, option
-00003e90: 616c 293a 2077 6865 7468 6572 2074 6f20  al): whether to 
-00003ea0: 7265 7475 726e 2070 6c75 6e67 6572 2074  return plunger t
-00003eb0: 6f20 686f 6d65 2070 6f73 6974 696f 6e2e  o home position.
-00003ec0: 2044 6566 6175 6c74 7320 746f 2054 7275   Defaults to Tru
-00003ed0: 652e 0d0a 0d0a 2020 2020 2020 2020 5265  e.....        Re
-00003ee0: 7475 726e 733a 0d0a 2020 2020 2020 2020  turns:..        
-00003ef0: 2020 2020 7374 723a 2064 6576 6963 6520      str: device 
-00003f00: 7265 7370 6f6e 7365 0d0a 2020 2020 2020  response..      
-00003f10: 2020 2222 220d 0a20 2020 2020 2020 2073    """..        s
-00003f20: 656c 662e 7265 6167 656e 7420 3d20 2727  elf.reagent = ''
-00003f30: 0d0a 2020 2020 2020 2020 636f 6d6d 616e  ..        comman
-00003f40: 6420 3d20 6627 5245 7b73 656c 662e 686f  d = f'RE{self.ho
-00003f50: 6d65 5f70 6f73 6974 696f 6e7d 2720 6966  me_position}' if
-00003f60: 2068 6f6d 6520 656c 7365 2027 5245 270d   home else 'RE'.
-00003f70: 0a20 2020 2020 2020 2072 6573 706f 6e73  .        respons
-00003f80: 6520 3d20 7365 6c66 2e5f 7175 6572 7928  e = self._query(
-00003f90: 636f 6d6d 616e 6429 0d0a 2020 2020 2020  command)..      
-00003fa0: 2020 7365 6c66 2e70 6f73 6974 696f 6e20    self.position 
-00003fb0: 3d20 7365 6c66 2e68 6f6d 655f 706f 7369  = self.home_posi
-00003fc0: 7469 6f6e 2069 6620 686f 6d65 2065 6c73  tion if home els
-00003fd0: 6520 300d 0a20 2020 2020 2020 2074 696d  e 0..        tim
-00003fe0: 652e 736c 6565 7028 3129 0d0a 2020 2020  e.sleep(1)..    
-00003ff0: 2020 2020 7265 7475 726e 2072 6573 706f      return respo
-00004000: 6e73 650d 0a20 2020 200d 0a20 2020 2064  nse..    ..    d
-00004010: 6566 2067 6574 4361 7061 6369 7461 6e63  ef getCapacitanc
-00004020: 6528 7365 6c66 2920 2d3e 2055 6e69 6f6e  e(self) -> Union
-00004030: 5b69 6e74 2c20 7374 725d 3a0d 0a20 2020  [int, str]:..   
-00004040: 2020 2020 2022 2222 0d0a 2020 2020 2020       """..      
-00004050: 2020 4765 7420 7468 6520 6361 7061 6369    Get the capaci
-00004060: 7461 6e63 6520 6173 206d 6561 7375 7265  tance as measure
-00004070: 6420 6174 2074 6865 2065 6e64 206f 6620  d at the end of 
-00004080: 7468 6520 7069 7065 7474 650d 0a20 2020  the pipette..   
-00004090: 2020 2020 200d 0a20 2020 2020 2020 2052       ..        R
-000040a0: 6574 7572 6e73 3a0d 0a20 2020 2020 2020  eturns:..       
-000040b0: 2020 2020 2055 6e69 6f6e 5b69 6e74 2c20       Union[int, 
-000040c0: 7374 725d 3a20 6361 7061 6369 7461 6e63  str]: capacitanc
-000040d0: 6520 7661 6c75 652c 206f 7220 6465 7669  e value, or devi
-000040e0: 6365 2072 6573 706f 6e73 650d 0a20 2020  ce response..   
-000040f0: 2020 2020 2022 2222 0d0a 2020 2020 2020       """..      
-00004100: 2020 7265 7370 6f6e 7365 203d 2073 656c    response = sel
-00004110: 662e 5f71 7565 7279 2827 444e 2729 0d0a  f._query('DN')..
-00004120: 2020 2020 2020 2020 7472 793a 0d0a 2020          try:..  
-00004130: 2020 2020 2020 2020 2020 6361 7061 6369            capaci
-00004140: 7461 6e63 6520 3d20 696e 7428 7265 7370  tance = int(resp
-00004150: 6f6e 7365 290d 0a20 2020 2020 2020 2065  onse)..        e
-00004160: 7863 6570 7420 5661 6c75 6545 7272 6f72  xcept ValueError
-00004170: 3a0d 0a20 2020 2020 2020 2020 2020 2072  :..            r
-00004180: 6574 7572 6e20 7265 7370 6f6e 7365 0d0a  eturn response..
-00004190: 2020 2020 2020 2020 7365 6c66 2e5f 6361          self._ca
-000041a0: 7061 6369 7461 6e63 6520 3d20 6361 7061  pacitance = capa
-000041b0: 6369 7461 6e63 650d 0a20 2020 2020 2020  citance..       
-000041c0: 2072 6574 7572 6e20 6361 7061 6369 7461   return capacita
-000041d0: 6e63 650d 0a20 0d0a 2020 2020 6465 6620  nce.. ..    def 
-000041e0: 6765 7445 7272 6f72 7328 7365 6c66 2920  getErrors(self) 
-000041f0: 2d3e 2073 7472 3a0d 0a20 2020 2020 2020  -> str:..       
-00004200: 2022 2222 0d0a 2020 2020 2020 2020 4765   """..        Ge
-00004210: 7420 6572 726f 7273 2066 726f 6d20 7468  t errors from th
-00004220: 6520 6465 7669 6365 0d0a 0d0a 2020 2020  e device....    
-00004230: 2020 2020 5265 7475 726e 733a 0d0a 2020      Returns:..  
-00004240: 2020 2020 2020 2020 2020 7374 723a 2064            str: d
-00004250: 6576 6963 6520 7265 7370 6f6e 7365 0d0a  evice response..
-00004260: 2020 2020 2020 2020 2222 220d 0a20 2020          """..   
-00004270: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
-00004280: 2e5f 7175 6572 7928 2744 4527 290d 0a20  ._query('DE').. 
-00004290: 2020 200d 0a20 2020 2064 6566 2067 6574     ..    def get
-000042a0: 496e 666f 2873 656c 662c 206d 6f64 656c  Info(self, model
-000042b0: 3a20 4f70 7469 6f6e 616c 5b73 7472 5d20  : Optional[str] 
-000042c0: 3d20 4e6f 6e65 293a 0d0a 2020 2020 2020  = None):..      
-000042d0: 2020 2222 2247 6574 2064 6574 6169 6c73    """Get details
-000042e0: 206f 6620 7468 6520 5361 7274 6f72 6975   of the Sartoriu
-000042f0: 7320 7069 7065 7474 6520 6d6f 6465 6c22  s pipette model"
-00004300: 2222 0d0a 2020 2020 2020 2020 6d6f 6465  ""..        mode
-00004310: 6c20 3d20 7365 6c66 2e5f 5f6d 6f64 656c  l = self.__model
-00004320: 5f5f 2829 2e73 706c 6974 2827 2d27 295b  __().split('-')[
-00004330: 305d 2069 6620 6d6f 6465 6c20 6973 204e  0] if model is N
-00004340: 6f6e 6520 656c 7365 206d 6f64 656c 0d0a  one else model..
-00004350: 2020 2020 2020 2020 6966 206d 6f64 656c          if model
-00004360: 206e 6f74 2069 6e20 6c69 622e 4d6f 6465   not in lib.Mode
-00004370: 6c49 6e66 6f2e 5f6d 656d 6265 725f 6e61  lInfo._member_na
-00004380: 6d65 735f 3a0d 0a20 2020 2020 2020 2020  mes_:..         
-00004390: 2020 2070 7269 6e74 2866 2752 6563 6569     print(f'Recei
-000043a0: 7665 643a 207b 6d6f 6465 6c7d 2729 0d0a  ved: {model}')..
-000043b0: 2020 2020 2020 2020 2020 2020 6d6f 6465              mode
-000043c0: 6c20 3d20 2742 524c 3027 0d0a 2020 2020  l = 'BRL0'..    
-000043d0: 2020 2020 2020 2020 7072 696e 7428 6622          print(f"
-000043e0: 4465 6661 756c 7469 6e67 2074 6f3a 207b  Defaulting to: {
-000043f0: 2742 524c 3027 7d22 290d 0a20 2020 2020  'BRL0'}")..     
-00004400: 2020 2020 2020 2070 7269 6e74 2866 2256         print(f"V
-00004410: 616c 6964 206d 6f64 656c 7320 6172 653a  alid models are:
-00004420: 207b 272c 2027 2e6a 6f69 6e28 6c69 622e   {', '.join(lib.
-00004430: 4d6f 6465 6c49 6e66 6f2e 5f6d 656d 6265  ModelInfo._membe
-00004440: 725f 6e61 6d65 735f 297d 2229 0d0a 2020  r_names_)}")..  
-00004450: 2020 2020 2020 696e 666f 3a20 6c69 622e        info: lib.
-00004460: 4d6f 6465 6c20 3d20 6c69 622e 4d6f 6465  Model = lib.Mode
-00004470: 6c49 6e66 6f5b 6d6f 6465 6c5d 2e76 616c  lInfo[model].val
-00004480: 7565 0d0a 2020 2020 2020 2020 7072 696e  ue..        prin
-00004490: 7428 696e 666f 290d 0a20 2020 2020 2020  t(info)..       
-000044a0: 2073 656c 662e 6d6f 6465 6c5f 696e 666f   self.model_info
-000044b0: 203d 2069 6e66 6f0d 0a20 2020 2020 2020   = info..       
-000044c0: 2073 656c 662e 6361 7061 6369 7479 203d   self.capacity =
-000044d0: 2069 6e66 6f2e 6361 7061 6369 7479 0d0a   info.capacity..
-000044e0: 2020 2020 2020 2020 7365 6c66 2e6c 696d          self.lim
-000044f0: 6974 7320 3d20 2869 6e66 6f2e 7469 705f  its = (info.tip_
-00004500: 656a 6563 745f 706f 7369 7469 6f6e 2c20  eject_position, 
-00004510: 696e 666f 2e6d 6178 5f70 6f73 6974 696f  info.max_positio
-00004520: 6e29 0d0a 2020 2020 2020 2020 7365 6c66  n)..        self
-00004530: 2e73 7065 6564 5f70 7265 7365 7473 203d  .speed_presets =
-00004540: 2069 6e66 6f2e 7072 6573 6574 5f73 7065   info.preset_spe
-00004550: 6564 730d 0a20 2020 2020 2020 2073 656c  eds..        sel
-00004560: 662e 7370 6565 642e 7570 203d 2073 656c  f.speed.up = sel
-00004570: 662e 7370 6565 645f 7072 6573 6574 735b  f.speed_presets[
-00004580: 7365 6c66 2e73 7065 6564 5f63 6f64 652e  self.speed_code.
-00004590: 7570 2d31 5d0d 0a20 2020 2020 2020 2073  up-1]..        s
-000045a0: 656c 662e 7370 6565 642e 646f 776e 203d  elf.speed.down =
-000045b0: 2073 656c 662e 7370 6565 645f 7072 6573   self.speed_pres
-000045c0: 6574 735b 7365 6c66 2e73 7065 6564 5f63  ets[self.speed_c
-000045d0: 6f64 652e 646f 776e 2d31 5d0d 0a20 2020  ode.down-1]..   
-000045e0: 2020 2020 2072 6574 7572 6e0d 0a20 2020       return..   
-000045f0: 200d 0a20 2020 2064 6566 2067 6574 506f   ..    def getPo
-00004600: 7369 7469 6f6e 2873 656c 662c 202a 2a6b  sition(self, **k
-00004610: 7761 7267 7329 202d 3e20 696e 743a 0d0a  wargs) -> int:..
-00004620: 2020 2020 2020 2020 2222 2247 6574 2074          """Get t
-00004630: 6865 2063 7572 7265 6e74 2070 6f73 6974  he current posit
-00004640: 696f 6e20 6f66 2074 6865 2070 6970 6574  ion of the pipet
-00004650: 7465 2222 220d 0a20 2020 2020 2020 2072  te"""..        r
-00004660: 6573 706f 6e73 6520 3d20 7365 6c66 2e5f  esponse = self._
-00004670: 7175 6572 7928 2744 5027 290d 0a20 2020  query('DP')..   
-00004680: 2020 2020 2074 7279 3a0d 0a20 2020 2020       try:..     
-00004690: 2020 2020 2020 2070 6f73 6974 696f 6e20         position 
-000046a0: 3d20 696e 7428 7265 7370 6f6e 7365 290d  = int(response).
-000046b0: 0a20 2020 2020 2020 2065 7863 6570 7420  .        except 
-000046c0: 5661 6c75 6545 7272 6f72 3a0d 0a20 2020  ValueError:..   
-000046d0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-000046e0: 7265 7370 6f6e 7365 0d0a 2020 2020 2020  response..      
-000046f0: 2020 7365 6c66 2e70 6f73 6974 696f 6e20    self.position 
-00004700: 3d20 706f 7369 7469 6f6e 0d0a 2020 2020  = position..    
-00004710: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
-00004720: 706f 7369 7469 6f6e 0d0a 2020 2020 2020  position..      
-00004730: 0d0a 2020 2020 6465 6620 6765 7453 7461  ..    def getSta
-00004740: 7475 7328 7365 6c66 2c20 2a2a 6b77 6172  tus(self, **kwar
-00004750: 6773 2920 2d3e 2073 7472 3a0d 0a20 2020  gs) -> str:..   
-00004760: 2020 2020 2022 2222 0d0a 2020 2020 2020       """..      
-00004770: 2020 4765 7420 7468 6520 7374 6174 7573    Get the status
-00004780: 206f 6620 7468 6520 7069 7065 7474 650d   of the pipette.
-00004790: 0a0d 0a20 2020 2020 2020 2052 6574 7572  ...        Retur
-000047a0: 6e73 3a0d 0a20 2020 2020 2020 2020 2020  ns:..           
-000047b0: 2073 7472 3a20 6465 7669 6365 2072 6573   str: device res
-000047c0: 706f 6e73 650d 0a20 2020 2020 2020 2022  ponse..        "
-000047d0: 2222 0d0a 2020 2020 2020 2020 7265 7370  ""..        resp
-000047e0: 6f6e 7365 203d 2073 656c 662e 5f71 7565  onse = self._que
-000047f0: 7279 2827 4453 2729 0d0a 2020 2020 2020  ry('DS')..      
-00004800: 2020 7472 793a 0d0a 2020 2020 2020 2020    try:..        
-00004810: 2020 2020 7374 6174 7573 203d 2069 6e74      status = int
-00004820: 2872 6573 706f 6e73 6529 0d0a 2020 2020  (response)..    
-00004830: 2020 2020 6578 6365 7074 2056 616c 7565      except Value
-00004840: 4572 726f 723a 0d0a 2020 2020 2020 2020  Error:..        
-00004850: 2020 2020 7265 7475 726e 2072 6573 706f      return respo
-00004860: 6e73 650d 0a20 2020 2020 2020 2069 6620  nse..        if 
-00004870: 7265 7370 6f6e 7365 206e 6f74 2069 6e20  response not in 
-00004880: 5b5f 7374 6174 7573 2e76 616c 7565 2066  [_status.value f
-00004890: 6f72 205f 7374 6174 7573 2069 6e20 6c69  or _status in li
-000048a0: 622e 5374 6174 7573 436f 6465 5d3a 0d0a  b.StatusCode]:..
-000048b0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-000048c0: 726e 2072 6573 706f 6e73 650d 0a20 2020  rn response..   
-000048d0: 2020 2020 200d 0a20 2020 2020 2020 2073       ..        s
-000048e0: 656c 662e 5f73 7461 7475 735f 636f 6465  elf._status_code
-000048f0: 203d 2073 7461 7475 730d 0a20 2020 2020   = status..     
-00004900: 2020 2069 6620 7374 6174 7573 2069 6e20     if status in 
-00004910: 5b34 2c36 2c38 5d3a 0d0a 2020 2020 2020  [4,6,8]:..      
-00004920: 2020 2020 2020 7365 6c66 2e73 6574 466c        self.setFl
-00004930: 6167 2862 7573 793d 5472 7565 290d 0a20  ag(busy=True).. 
-00004940: 2020 2020 2020 2020 2020 2069 6620 7365             if se
-00004950: 6c66 2e76 6572 626f 7365 3a0d 0a20 2020  lf.verbose:..   
-00004960: 2020 2020 2020 2020 2020 2020 2070 7269               pri
-00004970: 6e74 286c 6962 2e53 7461 7475 7343 6f64  nt(lib.StatusCod
-00004980: 6528 7374 6174 7573 292e 6e61 6d65 290d  e(status).name).
-00004990: 0a20 2020 2020 2020 2065 6c69 6620 7374  .        elif st
-000049a0: 6174 7573 203d 3d20 303a 0d0a 2020 2020  atus == 0:..    
-000049b0: 2020 2020 2020 2020 7365 6c66 2e73 6574          self.set
-000049c0: 466c 6167 2862 7573 793d 4661 6c73 6529  Flag(busy=False)
-000049d0: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
-000049e0: 206c 6962 2e53 7461 7475 7343 6f64 6528   lib.StatusCode(
-000049f0: 7365 6c66 2e5f 7374 6174 7573 5f63 6f64  self._status_cod
-00004a00: 6529 2e6e 616d 650d 0a20 2020 200d 0a20  e).name..    .. 
-00004a10: 2020 2064 6566 2068 6f6d 6528 7365 6c66     def home(self
-00004a20: 2920 2d3e 2073 7472 3a0d 0a20 2020 2020  ) -> str:..     
-00004a30: 2020 2022 2222 0d0a 2020 2020 2020 2020     """..        
-00004a40: 5265 7475 726e 2070 6c75 6e67 6572 2074  Return plunger t
-00004a50: 6f20 686f 6d65 2070 6f73 6974 696f 6e0d  o home position.
-00004a60: 0a20 2020 2020 2020 200d 0a20 2020 2020  .        ..     
-00004a70: 2020 2052 6574 7572 6e73 3a0d 0a20 2020     Returns:..   
-00004a80: 2020 2020 2020 2020 2073 7472 3a20 6465           str: de
-00004a90: 7669 6365 2072 6573 706f 6e73 650d 0a20  vice response.. 
-00004aa0: 2020 2020 2020 2022 2222 0d0a 2020 2020         """..    
-00004ab0: 2020 2020 7265 7370 6f6e 7365 203d 2073      response = s
-00004ac0: 656c 662e 5f71 7565 7279 2866 2752 507b  elf._query(f'RP{
-00004ad0: 7365 6c66 2e68 6f6d 655f 706f 7369 7469  self.home_positi
-00004ae0: 6f6e 7d27 290d 0a20 2020 2020 2020 2073  on}')..        s
-00004af0: 656c 662e 766f 6c75 6d65 203d 2030 0d0a  elf.volume = 0..
-00004b00: 2020 2020 2020 2020 7365 6c66 2e70 6f73          self.pos
-00004b10: 6974 696f 6e20 3d20 7365 6c66 2e68 6f6d  ition = self.hom
-00004b20: 655f 706f 7369 7469 6f6e 0d0a 2020 2020  e_position..    
-00004b30: 2020 2020 7469 6d65 2e73 6c65 6570 2831      time.sleep(1
-00004b40: 290d 0a20 2020 2020 2020 2072 6574 7572  )..        retur
-00004b50: 6e20 7265 7370 6f6e 7365 0d0a 2020 2020  n response..    
-00004b60: 0d0a 2020 2020 6465 6620 6973 4665 6173  ..    def isFeas
-00004b70: 6962 6c65 2873 656c 662c 2070 6f73 6974  ible(self, posit
-00004b80: 696f 6e3a 696e 7429 202d 3e20 626f 6f6c  ion:int) -> bool
-00004b90: 3a0d 0a20 2020 2020 2020 2022 2222 0d0a  :..        """..
-00004ba0: 2020 2020 2020 2020 4368 6563 6b73 2061          Checks a
-00004bb0: 6e64 2072 6574 7572 6e73 2077 6865 7468  nd returns wheth
-00004bc0: 6572 2074 6865 2070 6c75 6e67 6572 2070  er the plunger p
-00004bd0: 6f73 6974 696f 6e20 6973 2066 6561 7369  osition is feasi
-00004be0: 626c 650d 0a0d 0a20 2020 2020 2020 2041  ble....        A
-00004bf0: 7267 733a 0d0a 2020 2020 2020 2020 2020  rgs:..          
-00004c00: 2020 706f 7369 7469 6f6e 2028 696e 7429    position (int)
-00004c10: 3a20 706c 756e 6765 7220 706f 7369 7469  : plunger positi
-00004c20: 6f6e 0d0a 0d0a 2020 2020 2020 2020 5265  on....        Re
-00004c30: 7475 726e 733a 0d0a 2020 2020 2020 2020  turns:..        
-00004c40: 2020 2020 626f 6f6c 3a20 7768 6574 6865      bool: whethe
-00004c50: 7220 706c 756e 6765 7220 706f 7369 7469  r plunger positi
-00004c60: 6f6e 2069 7320 6665 6173 6962 6c65 0d0a  on is feasible..
-00004c70: 2020 2020 2020 2020 2222 220d 0a20 2020          """..   
-00004c80: 2020 2020 2069 6620 2873 656c 662e 6c69       if (self.li
-00004c90: 6d69 7473 5b30 5d20 3c3d 2070 6f73 6974  mits[0] <= posit
-00004ca0: 696f 6e20 3c3d 2073 656c 662e 6c69 6d69  ion <= self.limi
-00004cb0: 7473 5b31 5d29 3a0d 0a20 2020 2020 2020  ts[1]):..       
-00004cc0: 2020 2020 2072 6574 7572 6e20 5472 7565       return True
-00004cd0: 0d0a 2020 2020 2020 2020 7072 696e 7428  ..        print(
-00004ce0: 6622 5261 6e67 6520 6c69 6d69 7473 2072  f"Range limits r
-00004cf0: 6561 6368 6564 2120 7b73 656c 662e 6c69  eached! {self.li
-00004d00: 6d69 7473 7d22 290d 0a20 2020 2020 2020  mits}")..       
-00004d10: 2072 6574 7572 6e20 4661 6c73 650d 0a20   return False.. 
-00004d20: 2020 200d 0a20 2020 2064 6566 2069 7354     ..    def isT
-00004d30: 6970 4f6e 2873 656c 6629 202d 3e20 626f  ipOn(self) -> bo
-00004d40: 6f6c 3a0d 0a20 2020 2020 2020 2022 2222  ol:..        """
-00004d50: 0d0a 2020 2020 2020 2020 4368 6563 6b73  ..        Checks
-00004d60: 2061 6e64 2072 6574 7572 6e73 2077 6865   and returns whe
-00004d70: 7468 6572 2061 2070 6970 6574 7465 2074  ther a pipette t
-00004d80: 6970 2069 7320 6174 7461 6368 6564 0d0a  ip is attached..
-00004d90: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
-00004da0: 2020 5265 7475 726e 733a 0d0a 2020 2020    Returns:..    
-00004db0: 2020 2020 2020 2020 626f 6f6c 3a20 7768          bool: wh
-00004dc0: 6574 6865 7220 6120 7069 7065 7474 6520  ether a pipette 
-00004dd0: 7469 7020 696e 2061 7474 6163 6865 640d  tip in attached.
-00004de0: 0a20 2020 2020 2020 2022 2222 0d0a 2020  .        """..  
-00004df0: 2020 2020 2020 7365 6c66 2e67 6574 4361        self.getCa
-00004e00: 7061 6369 7461 6e63 6528 290d 0a20 2020  pacitance()..   
-00004e10: 2020 2020 2070 7269 6e74 2866 2754 6970       print(f'Tip
-00004e20: 2063 6170 6163 6974 616e 6365 3a20 7b73   capacitance: {s
-00004e30: 656c 662e 6361 7061 6369 7461 6e63 657d  elf.capacitance}
-00004e40: 2729 0d0a 2020 2020 2020 2020 6966 2073  ')..        if s
-00004e50: 656c 662e 666c 6167 735b 2763 6f6e 6475  elf.flags['condu
-00004e60: 6374 6976 655f 7469 7073 275d 3a0d 0a20  ctive_tips']:.. 
-00004e70: 2020 2020 2020 2020 2020 2074 6970 5f6f             tip_o
-00004e80: 6e20 3d20 2873 656c 662e 6361 7061 6369  n = (self.capaci
-00004e90: 7461 6e63 6520 3e20 7365 6c66 2e74 6970  tance > self.tip
-00004ea0: 5f74 6872 6573 686f 6c64 290d 0a20 2020  _threshold)..   
-00004eb0: 2020 2020 2020 2020 2073 656c 662e 7365           self.se
-00004ec0: 7446 6c61 6728 7469 705f 6f6e 3d74 6970  tFlag(tip_on=tip
-00004ed0: 5f6f 6e29 0d0a 2020 2020 2020 2020 7469  _on)..        ti
-00004ee0: 705f 6f6e 203d 2073 656c 662e 666c 6167  p_on = self.flag
-00004ef0: 735b 2774 6970 5f6f 6e27 5d0d 0a20 2020  s['tip_on']..   
-00004f00: 2020 2020 2072 6574 7572 6e20 7469 705f       return tip_
-00004f10: 6f6e 0d0a 2020 2020 0d0a 2020 2020 6465  on..    ..    de
-00004f20: 6620 6d6f 7665 2873 656c 662c 2073 7465  f move(self, ste
-00004f30: 7073 3a69 6e74 2c20 7570 3a62 6f6f 6c2c  ps:int, up:bool,
-00004f40: 202a 2a6b 7761 7267 7329 202d 3e20 7374   **kwargs) -> st
-00004f50: 723a 0d0a 2020 2020 2020 2020 2222 220d  r:..        """.
-00004f60: 0a20 2020 2020 2020 204d 6f76 6520 7468  .        Move th
-00004f70: 6520 706c 756e 6765 7220 6569 7468 6572  e plunger either
-00004f80: 2075 7020 6f72 2064 6f77 6e20 6279 2061   up or down by a
-00004f90: 2073 7065 6369 6669 6564 206e 756d 6265   specified numbe
-00004fa0: 7220 6f66 2073 7465 7073 0d0a 0d0a 2020  r of steps....  
-00004fb0: 2020 2020 2020 4172 6773 3a0d 0a20 2020        Args:..   
-00004fc0: 2020 2020 2020 2020 2073 7465 7073 2028           steps (
-00004fd0: 696e 7429 3a20 6e75 6d62 6572 206f 6620  int): number of 
-00004fe0: 7374 6570 7320 746f 206d 6f76 6520 706c  steps to move pl
-00004ff0: 756e 6765 7220 6279 0d0a 2020 2020 2020  unger by..      
-00005000: 2020 2020 2020 7570 2028 626f 6f6c 293a        up (bool):
-00005010: 2077 6865 7468 6572 2074 6f20 6d6f 7665   whether to move
-00005020: 2074 6865 2070 6c75 6e67 6572 2075 700d   the plunger up.
-00005030: 0a0d 0a20 2020 2020 2020 2052 6574 7572  ...        Retur
-00005040: 6e73 3a0d 0a20 2020 2020 2020 2020 2020  ns:..           
-00005050: 2073 7472 3a20 6465 7669 6365 2072 6573   str: device res
-00005060: 706f 6e73 650d 0a20 2020 2020 2020 2022  ponse..        "
-00005070: 2222 0d0a 2020 2020 2020 2020 7374 6570  ""..        step
-00005080: 7320 3d20 6162 7328 7374 6570 7329 2069  s = abs(steps) i
-00005090: 6620 7570 2065 6c73 6520 2d61 6273 2873  f up else -abs(s
-000050a0: 7465 7073 290d 0a20 2020 2020 2020 2072  teps)..        r
-000050b0: 6574 7572 6e20 7365 6c66 2e6d 6f76 6542  eturn self.moveB
-000050c0: 7928 7374 6570 7329 0d0a 2020 2020 0d0a  y(steps)..    ..
-000050d0: 2020 2020 6465 6620 6d6f 7665 4279 2873      def moveBy(s
-000050e0: 656c 662c 2073 7465 7073 3a69 6e74 2c20  elf, steps:int, 
-000050f0: 2a2a 6b77 6172 6773 2920 2d3e 2073 7472  **kwargs) -> str
-00005100: 3a0d 0a20 2020 2020 2020 2022 2222 0d0a  :..        """..
-00005110: 2020 2020 2020 2020 4d6f 7665 2074 6865          Move the
-00005120: 2070 6c75 6e67 6572 2062 7920 7370 6563   plunger by spec
-00005130: 6966 6965 6420 6e75 6d62 6572 206f 6620  ified number of 
-00005140: 7374 6570 730d 0a0d 0a20 2020 2020 2020  steps....       
-00005150: 2041 7267 733a 0d0a 2020 2020 2020 2020   Args:..        
-00005160: 2020 2020 7374 6570 7320 2869 6e74 293a      steps (int):
-00005170: 206e 756d 6265 7220 6f66 2073 7465 7073   number of steps
-00005180: 2074 6f20 6d6f 7665 2070 6c75 6e67 6572   to move plunger
-00005190: 2062 7920 283c 303a 206d 6f76 6520 646f   by (<0: move do
-000051a0: 776e 2f64 6973 7065 6e73 653b 203e 3020  wn/dispense; >0 
-000051b0: 6d6f 7665 2075 702f 6173 7069 7261 7465  move up/aspirate
-000051c0: 290d 0a0d 0a20 2020 2020 2020 2052 6574  )....        Ret
-000051d0: 7572 6e73 3a0d 0a20 2020 2020 2020 2020  urns:..         
-000051e0: 2020 2073 7472 3a20 6465 7669 6365 2072     str: device r
-000051f0: 6573 706f 6e73 650d 0a20 2020 2020 2020  esponse..       
-00005200: 2022 2222 0d0a 2020 2020 2020 2020 636f   """..        co
-00005210: 6d6d 616e 6420 3d20 6627 5249 7b73 7465  mmand = f'RI{ste
-00005220: 7073 7d27 2069 6620 7374 6570 7320 3e20  ps}' if steps > 
-00005230: 3020 656c 7365 2066 2752 4f7b 2d73 7465  0 else f'RO{-ste
-00005240: 7073 7d27 0d0a 2020 2020 2020 2020 7365  ps}'..        se
-00005250: 6c66 2e70 6f73 6974 696f 6e20 2b3d 2073  lf.position += s
-00005260: 7465 7073 0d0a 2020 2020 2020 2020 7265  teps..        re
-00005270: 7475 726e 2073 656c 662e 5f71 7565 7279  turn self._query
-00005280: 2863 6f6d 6d61 6e64 290d 0a20 2020 200d  (command)..    .
-00005290: 0a20 2020 2064 6566 206d 6f76 6554 6f28  .    def moveTo(
-000052a0: 7365 6c66 2c20 706f 7369 7469 6f6e 3a69  self, position:i
-000052b0: 6e74 2c20 2a2a 6b77 6172 6773 2920 2d3e  nt, **kwargs) ->
-000052c0: 2073 7472 3a0d 0a20 2020 2020 2020 2022   str:..        "
-000052d0: 2222 0d0a 2020 2020 2020 2020 4d6f 7665  ""..        Move
-000052e0: 2074 6865 2070 6c75 6e67 6572 2074 6f20   the plunger to 
-000052f0: 6120 7370 6563 6966 6965 6420 706f 7369  a specified posi
-00005300: 7469 6f6e 0d0a 0d0a 2020 2020 2020 2020  tion....        
-00005310: 4172 6773 3a0d 0a20 2020 2020 2020 2020  Args:..         
-00005320: 2020 2070 6f73 6974 696f 6e20 2869 6e74     position (int
-00005330: 293a 2074 6172 6765 7420 706c 756e 6765  ): target plunge
-00005340: 7220 706f 7369 7469 6f6e 0d0a 0d0a 2020  r position....  
-00005350: 2020 2020 2020 5265 7475 726e 733a 0d0a        Returns:..
-00005360: 2020 2020 2020 2020 2020 2020 7374 723a              str:
-00005370: 2064 6576 6963 6520 7265 7370 6f6e 7365   device response
-00005380: 0d0a 2020 2020 2020 2020 2222 220d 0a20  ..        """.. 
-00005390: 2020 2020 2020 2073 656c 662e 706f 7369         self.posi
-000053a0: 7469 6f6e 203d 2070 6f73 6974 696f 6e0d  tion = position.
-000053b0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-000053c0: 7365 6c66 2e5f 7175 6572 7928 6627 5250  self._query(f'RP
-000053d0: 7b70 6f73 6974 696f 6e7d 2729 0d0a 2020  {position}')..  
-000053e0: 2020 0d0a 2020 2020 6465 6620 7075 6c6c    ..    def pull
-000053f0: 6261 636b 2873 656c 662c 2073 7465 7073  back(self, steps
-00005400: 3a69 6e74 203d 2035 2c20 2a2a 6b77 6172  :int = 5, **kwar
-00005410: 6773 2920 2d3e 2073 7472 3a0d 0a20 2020  gs) -> str:..   
-00005420: 2020 2020 2022 2222 0d0a 2020 2020 2020       """..      
-00005430: 2020 5075 6c6c 6261 636b 206c 6971 7569    Pullback liqui
-00005440: 6420 6672 6f6d 2074 6970 0d0a 2020 2020  d from tip..    
-00005450: 2020 2020 0d0a 2020 2020 2020 2020 4172      ..        Ar
-00005460: 6773 3a0d 0a20 2020 2020 2020 2020 2020  gs:..           
-00005470: 2073 7465 7073 2028 696e 742c 206f 7074   steps (int, opt
-00005480: 696f 6e61 6c29 3a20 6e75 6d62 6572 206f  ional): number o
-00005490: 6620 7374 6570 7320 746f 2070 756c 6c62  f steps to pullb
-000054a0: 6163 6b2e 2044 6566 6175 6c74 7320 746f  ack. Defaults to
-000054b0: 2035 2e0d 0a0d 0a20 2020 2020 2020 2052   5.....        R
-000054c0: 6574 7572 6e73 3a0d 0a20 2020 2020 2020  eturns:..       
-000054d0: 2020 2020 2073 7472 3a20 6465 7669 6365       str: device
-000054e0: 2072 6573 706f 6e73 650d 0a20 2020 2020   response..     
-000054f0: 2020 2022 2222 0d0a 2020 2020 2020 2020     """..        
-00005500: 7265 7370 6f6e 7365 203d 2073 656c 662e  response = self.
-00005510: 5f71 7565 7279 2866 2752 497b 7374 6570  _query(f'RI{step
-00005520: 737d 2729 0d0a 2020 2020 2020 2020 7365  s}')..        se
-00005530: 6c66 2e70 6f73 6974 696f 6e20 2b3d 2073  lf.position += s
-00005540: 7465 7073 0d0a 2020 2020 2020 2020 7469  teps..        ti
-00005550: 6d65 2e73 6c65 6570 2831 290d 0a20 2020  me.sleep(1)..   
-00005560: 2020 2020 2072 6574 7572 6e20 7265 7370       return resp
-00005570: 6f6e 7365 0d0a 2020 2020 0d0a 2020 2020  onse..    ..    
-00005580: 6465 6620 7265 7365 7428 7365 6c66 2920  def reset(self) 
-00005590: 2d3e 2073 7472 3a0d 0a20 2020 2020 2020  -> str:..       
-000055a0: 2022 2222 0d0a 2020 2020 2020 2020 5265   """..        Re
-000055b0: 7365 7420 7468 6520 7069 7065 7474 650d  set the pipette.
-000055c0: 0a0d 0a20 2020 2020 2020 2052 6574 7572  ...        Retur
-000055d0: 6e73 3a0d 0a20 2020 2020 2020 2020 2020  ns:..           
-000055e0: 2073 7472 3a20 6465 7669 6365 2072 6573   str: device res
-000055f0: 706f 6e73 650d 0a20 2020 2020 2020 2022  ponse..        "
-00005600: 2222 0d0a 2020 2020 2020 2020 7365 6c66  ""..        self
-00005610: 2e7a 6572 6f28 290d 0a20 2020 2020 2020  .zero()..       
-00005620: 2072 6574 7572 6e20 7365 6c66 2e68 6f6d   return self.hom
-00005630: 6528 290d 0a20 2020 200d 0a20 2020 2064  e()..    ..    d
-00005640: 6566 2073 6574 5370 6565 6428 7365 6c66  ef setSpeed(self
-00005650: 2c20 7370 6565 643a 696e 742c 2075 703a  , speed:int, up:
-00005660: 626f 6f6c 2c20 6465 6661 756c 743a 626f  bool, default:bo
-00005670: 6f6c 203d 2046 616c 7365 2c20 2a2a 6b77  ol = False, **kw
-00005680: 6172 6773 2920 2d3e 2073 7472 3a0d 0a20  args) -> str:.. 
-00005690: 2020 2020 2020 2022 2222 0d0a 2020 2020         """..    
-000056a0: 2020 2020 5365 7420 7468 6520 7370 6565      Set the spee
-000056b0: 6420 6f66 2074 6865 2070 6c75 6e67 6572  d of the plunger
-000056c0: 0d0a 0d0a 2020 2020 2020 2020 4172 6773  ....        Args
-000056d0: 3a0d 0a20 2020 2020 2020 2020 2020 2073  :..            s
-000056e0: 7065 6564 2028 696e 7429 3a20 7370 6565  peed (int): spee
-000056f0: 6420 6f66 2070 6c75 6e67 6572 0d0a 2020  d of plunger..  
-00005700: 2020 2020 2020 2020 2020 7570 2028 626f            up (bo
-00005710: 6f6c 293a 2064 6972 6563 7469 6f6e 206f  ol): direction o
-00005720: 6620 7472 6176 656c 0d0a 2020 2020 2020  f travel..      
-00005730: 2020 2020 2020 6465 6661 756c 7420 2862        default (b
-00005740: 6f6f 6c2c 206f 7074 696f 6e61 6c29 3a20  ool, optional): 
-00005750: 7768 6574 6865 7220 746f 2073 6574 2073  whether to set s
-00005760: 7065 6564 2061 7320 6120 6465 6661 756c  peed as a defaul
-00005770: 742e 2044 6566 6175 6c74 7320 746f 2046  t. Defaults to F
-00005780: 616c 7365 2e0d 0a0d 0a20 2020 2020 2020  alse.....       
-00005790: 2052 6574 7572 6e73 3a0d 0a20 2020 2020   Returns:..     
-000057a0: 2020 2020 2020 2073 7472 3a20 6465 7669         str: devi
-000057b0: 6365 2072 6573 706f 6e73 650d 0a20 2020  ce response..   
-000057c0: 2020 2020 2022 2222 0d0a 2020 2020 2020       """..      
-000057d0: 2020 7370 6565 645f 636f 6465 203d 2031    speed_code = 1
-000057e0: 202b 205b 7820 666f 7220 782c 7661 6c20   + [x for x,val 
-000057f0: 696e 2065 6e75 6d65 7261 7465 286e 702e  in enumerate(np.
-00005800: 6172 7261 7928 7365 6c66 2e73 7065 6564  array(self.speed
-00005810: 5f70 7265 7365 7473 292d 7370 6565 6429  _presets)-speed)
-00005820: 2069 6620 7661 6c20 3e3d 2030 5d5b 305d   if val >= 0][0]
-00005830: 0d0a 2020 2020 2020 2020 7072 696e 7428  ..        print(
-00005840: 6627 5370 6565 6420 7b73 7065 6564 5f63  f'Speed {speed_c
-00005850: 6f64 657d 3a20 7b73 656c 662e 7370 6565  ode}: {self.spee
-00005860: 645f 7072 6573 6574 735b 7370 6565 645f  d_presets[speed_
-00005870: 636f 6465 2d31 5d7d 2075 4c2f 7327 290d  code-1]} uL/s').
-00005880: 0a20 2020 2020 2020 2064 6972 6563 7469  .        directi
-00005890: 6f6e 203d 2027 4927 2069 6620 7570 2065  on = 'I' if up e
-000058a0: 6c73 6520 274f 270d 0a20 2020 2020 2020  lse 'O'..       
-000058b0: 2073 656c 662e 5f71 7565 7279 2866 2753   self._query(f'S
-000058c0: 7b64 6972 6563 7469 6f6e 7d7b 7370 6565  {direction}{spee
-000058d0: 645f 636f 6465 7d27 290d 0a20 2020 2020  d_code}')..     
-000058e0: 2020 2069 6620 6e6f 7420 6465 6661 756c     if not defaul
-000058f0: 743a 0d0a 2020 2020 2020 2020 2020 2020  t:..            
-00005900: 7265 7475 726e 2073 656c 662e 5f71 7565  return self._que
-00005910: 7279 2866 2744 7b64 6972 6563 7469 6f6e  ry(f'D{direction
-00005920: 7d27 290d 0a20 2020 2020 2020 2069 6620  }')..        if 
-00005930: 7570 3a0d 0a20 2020 2020 2020 2020 2020  up:..           
-00005940: 2073 656c 662e 7370 6565 645f 636f 6465   self.speed_code
-00005950: 2e75 7020 3d20 7370 6565 645f 636f 6465  .up = speed_code
-00005960: 0d0a 2020 2020 2020 2020 2020 2020 7365  ..            se
-00005970: 6c66 2e73 7065 6564 2e75 7020 3d20 7365  lf.speed.up = se
-00005980: 6c66 2e73 7065 6564 5f70 7265 7365 7473  lf.speed_presets
-00005990: 5b73 7065 6564 5f63 6f64 652d 315d 0d0a  [speed_code-1]..
-000059a0: 2020 2020 2020 2020 656c 7365 3a0d 0a20          else:.. 
-000059b0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-000059c0: 7370 6565 645f 636f 6465 2e64 6f77 6e20  speed_code.down 
-000059d0: 3d20 7370 6565 645f 636f 6465 0d0a 2020  = speed_code..  
-000059e0: 2020 2020 2020 2020 2020 7365 6c66 2e73            self.s
-000059f0: 7065 6564 2e64 6f77 6e20 3d20 7365 6c66  peed.down = self
-00005a00: 2e73 7065 6564 5f70 7265 7365 7473 5b73  .speed_presets[s
-00005a10: 7065 6564 5f63 6f64 652d 315d 0d0a 2020  peed_code-1]..  
-00005a20: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
-00005a30: 662e 5f71 7565 7279 2866 2744 7b64 6972  f._query(f'D{dir
-00005a40: 6563 7469 6f6e 7d27 290d 0a20 2020 200d  ection}')..    .
-00005a50: 0a20 2020 2064 6566 2073 6875 7464 6f77  .    def shutdow
-00005a60: 6e28 7365 6c66 293a 0d0a 2020 2020 2020  n(self):..      
-00005a70: 2020 2222 2253 6875 7464 6f77 6e20 7072    """Shutdown pr
-00005a80: 6f63 6564 7572 6520 666f 7220 746f 6f6c  ocedure for tool
-00005a90: 2222 220d 0a20 2020 2020 2020 2073 656c  """..        sel
-00005aa0: 662e 746f 6767 6c65 4665 6564 6261 636b  f.toggleFeedback
-00005ab0: 4c6f 6f70 286f 6e3d 4661 6c73 6529 0d0a  Loop(on=False)..
-00005ac0: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-00005ad0: 7570 6572 2829 2e73 6875 7464 6f77 6e28  uper().shutdown(
-00005ae0: 290d 0a20 2020 200d 0a20 2020 2064 6566  )..    ..    def
-00005af0: 2074 6f67 676c 6546 6565 6462 6163 6b4c   toggleFeedbackL
-00005b00: 6f6f 7028 7365 6c66 2c20 6f6e 3a62 6f6f  oop(self, on:boo
-00005b10: 6c29 3a0d 0a20 2020 2020 2020 2022 2222  l):..        """
-00005b20: 0d0a 2020 2020 2020 2020 5374 6172 7420  ..        Start 
-00005b30: 6f72 2073 746f 7020 6665 6564 6261 636b  or stop feedback
-00005b40: 206c 6f6f 700d 0a20 2020 2020 2020 200d   loop..        .
-00005b50: 0a20 2020 2020 2020 2041 7267 733a 0d0a  .        Args:..
-00005b60: 2020 2020 2020 2020 2020 2020 6f6e 2028              on (
-00005b70: 626f 6f6c 293a 2077 6865 7468 6572 2074  bool): whether t
-00005b80: 6f20 7374 6172 7420 6665 6564 6261 636b  o start feedback
-00005b90: 206c 6f6f 700d 0a20 2020 2020 2020 2022   loop..        "
-00005ba0: 2222 0d0a 2020 2020 2020 2020 7365 6c66  ""..        self
-00005bb0: 2e73 6574 466c 6167 2867 6574 5f66 6565  .setFlag(get_fee
-00005bc0: 6462 6163 6b3d 6f6e 290d 0a20 2020 2020  dback=on)..     
-00005bd0: 2020 2069 6620 6f6e 3a0d 0a20 2020 2020     if on:..     
-00005be0: 2020 2020 2020 2069 6620 2766 6565 6462         if 'feedb
-00005bf0: 6163 6b5f 6c6f 6f70 2720 696e 2073 656c  ack_loop' in sel
-00005c00: 662e 5f74 6872 6561 6473 3a0d 0a20 2020  f._threads:..   
-00005c10: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00005c20: 662e 5f74 6872 6561 6473 5b27 6665 6564  f._threads['feed
-00005c30: 6261 636b 5f6c 6f6f 7027 5d2e 6a6f 696e  back_loop'].join
-00005c40: 2829 0d0a 2020 2020 2020 2020 2020 2020  ()..            
-00005c50: 7468 7265 6164 203d 2054 6872 6561 6428  thread = Thread(
-00005c60: 7461 7267 6574 3d73 656c 662e 5f6c 6f6f  target=self._loo
-00005c70: 705f 6665 6564 6261 636b 290d 0a20 2020  p_feedback)..   
-00005c80: 2020 2020 2020 2020 2074 6872 6561 642e           thread.
-00005c90: 7374 6172 7428 290d 0a20 2020 2020 2020  start()..       
-00005ca0: 2020 2020 2073 656c 662e 5f74 6872 6561       self._threa
-00005cb0: 6473 5b27 6665 6564 6261 636b 5f6c 6f6f  ds['feedback_loo
-00005cc0: 7027 5d20 3d20 7468 7265 6164 0d0a 2020  p'] = thread..  
-00005cd0: 2020 2020 2020 656c 7365 3a0d 0a20 2020        else:..   
-00005ce0: 2020 2020 2020 2020 2069 6620 2766 6565           if 'fee
-00005cf0: 6462 6163 6b5f 6c6f 6f70 2720 696e 2073  dback_loop' in s
-00005d00: 656c 662e 5f74 6872 6561 6473 3a0d 0a20  elf._threads:.. 
-00005d10: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00005d20: 656c 662e 5f74 6872 6561 6473 5b27 6665  elf._threads['fe
-00005d30: 6564 6261 636b 5f6c 6f6f 7027 5d2e 6a6f  edback_loop'].jo
-00005d40: 696e 2829 0d0a 2020 2020 2020 2020 7265  in()..        re
-00005d50: 7475 726e 0d0a 0d0a 2020 2020 6465 6620  turn....    def 
-00005d60: 7a65 726f 2873 656c 6629 202d 3e20 7374  zero(self) -> st
-00005d70: 723a 0d0a 2020 2020 2020 2020 2222 220d  r:..        """.
-00005d80: 0a20 2020 2020 2020 205a 6572 6f20 7468  .        Zero th
-00005d90: 6520 706c 756e 6765 7220 706f 7369 7469  e plunger positi
-00005da0: 6f6e 0d0a 2020 2020 2020 2020 0d0a 2020  on..        ..  
-00005db0: 2020 2020 2020 5265 7475 726e 733a 0d0a        Returns:..
-00005dc0: 2020 2020 2020 2020 2020 2020 7374 723a              str:
-00005dd0: 2064 6576 6963 6520 7265 7370 6f6e 7365   device response
-00005de0: 0d0a 2020 2020 2020 2020 2222 220d 0a20  ..        """.. 
-00005df0: 2020 2020 2020 2073 656c 662e 656a 6563         self.ejec
-00005e00: 7428 290d 0a20 2020 2020 2020 2072 6573  t()..        res
-00005e10: 706f 6e73 6520 3d20 7365 6c66 2e5f 7175  ponse = self._qu
-00005e20: 6572 7928 2752 5a27 290d 0a20 2020 2020  ery('RZ')..     
-00005e30: 2020 2073 656c 662e 706f 7369 7469 6f6e     self.position
-00005e40: 203d 2030 0d0a 2020 2020 2020 2020 7469   = 0..        ti
-00005e50: 6d65 2e73 6c65 6570 2832 290d 0a20 2020  me.sleep(2)..   
-00005e60: 2020 2020 2072 6574 7572 6e20 7265 7370       return resp
-00005e70: 6f6e 7365 0d0a 0d0a 2020 2020 2320 5072  onse....    # Pr
-00005e80: 6f74 6563 7465 6420 6d65 7468 6f64 2873  otected method(s
-00005e90: 290d 0a20 2020 2064 6566 205f 6361 6c63  )..    def _calc
-00005ea0: 756c 6174 655f 7370 6565 645f 7061 7261  ulate_speed_para
-00005eb0: 6d65 7465 7273 2873 656c 662c 2076 6f6c  meters(self, vol
-00005ec0: 756d 653a 696e 742c 2073 7065 6564 3a69  ume:int, speed:i
-00005ed0: 6e74 2920 2d3e 206c 6962 2e53 7065 6564  nt) -> lib.Speed
-00005ee0: 5061 7261 6d65 7465 7273 3a0d 0a20 2020  Parameters:..   
-00005ef0: 2020 2020 2022 2222 0d0a 2020 2020 2020       """..      
-00005f00: 2020 4361 6c63 756c 6174 6573 2074 6865    Calculates the
-00005f10: 2062 6573 7420 7061 7261 6d65 7465 7273   best parameters
-00005f20: 2066 6f72 2076 6f6c 756d 6520 616e 6420   for volume and 
-00005f30: 7370 6565 640d 0a0d 0a20 2020 2020 2020  speed....       
-00005f40: 2041 7267 733a 0d0a 2020 2020 2020 2020   Args:..        
-00005f50: 2020 2020 766f 6c75 6d65 2028 696e 7429      volume (int)
-00005f60: 3a20 766f 6c75 6d65 2074 6f20 6265 2074  : volume to be t
-00005f70: 7261 6e73 6665 7272 6564 0d0a 2020 2020  ransferred..    
-00005f80: 2020 2020 2020 2020 7370 6565 6420 2869          speed (i
-00005f90: 6e74 293a 2073 7065 6564 2061 7420 7768  nt): speed at wh
-00005fa0: 6963 6820 6c69 7175 6964 2069 7320 7472  ich liquid is tr
-00005fb0: 616e 7366 6572 7265 640d 0a0d 0a20 2020  ansferred....   
-00005fc0: 2020 2020 2052 6574 7572 6e73 3a0d 0a20       Returns:.. 
-00005fd0: 2020 2020 2020 2020 2020 2064 6963 743a             dict:
-00005fe0: 2064 6963 7469 6f6e 6172 7920 6f66 2062   dictionary of b
-00005ff0: 6573 7420 7061 7261 6d65 7465 7273 0d0a  est parameters..
-00006000: 2020 2020 2020 2020 2222 220d 0a20 2020          """..   
-00006010: 2020 2020 206f 7574 636f 6d65 7320 3d20       outcomes = 
-00006020: 7b7d 0d0a 2020 2020 2020 2020 7374 6570  {}..        step
-00006030: 5f69 6e74 6572 7661 6c5f 6c69 6d69 7420  _interval_limit 
-00006040: 3d20 696e 7428 766f 6c75 6d65 2f73 656c  = int(volume/sel
-00006050: 662e 7265 736f 6c75 7469 6f6e 2f53 5445  f.resolution/STE
-00006060: 505f 5245 534f 4c55 5449 4f4e 290d 0a20  P_RESOLUTION).. 
-00006070: 2020 2020 2020 2066 6f72 2070 7265 7365         for prese
-00006080: 7420 696e 2073 656c 662e 7370 6565 645f  t in self.speed_
-00006090: 7072 6573 6574 733a 0d0a 2020 2020 2020  presets:..      
-000060a0: 2020 2020 2020 6966 2070 7265 7365 7420        if preset 
-000060b0: 3c20 7370 6565 643a 0d0a 2020 2020 2020  < speed:..      
-000060c0: 2020 2020 2020 2020 2020 2320 7072 6573            # pres
-000060d0: 6574 2069 7320 736c 6f77 6572 2074 6861  et is slower tha
-000060e0: 6e20 7461 7267 6574 2073 7065 6564 2c20  n target speed, 
-000060f0: 6974 2077 696c 6c20 6e65 7665 7220 6869  it will never hi
-00006100: 7420 7461 7267 6574 2073 7065 6564 0d0a  t target speed..
-00006110: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006120: 636f 6e74 696e 7565 0d0a 2020 2020 2020  continue..      
-00006130: 2020 2020 2020 7469 6d65 5f69 6e74 6572        time_inter
-00006140: 7661 6c5f 6c69 6d69 7420 3d20 696e 7428  val_limit = int(
-00006150: 766f 6c75 6d65 2a28 312f 7370 6565 6420  volume*(1/speed 
-00006160: 2d20 312f 7072 6573 6574 292f 7365 6c66  - 1/preset)/self
-00006170: 2e72 6573 706f 6e73 655f 7469 6d65 290d  .response_time).
-00006180: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-00006190: 6e6f 7420 7374 6570 5f69 6e74 6572 7661  not step_interva
-000061a0: 6c5f 6c69 6d69 7420 6f72 206e 6f74 2074  l_limit or not t
-000061b0: 696d 655f 696e 7465 7276 616c 5f6c 696d  ime_interval_lim
-000061c0: 6974 3a0d 0a20 2020 2020 2020 2020 2020  it:..           
-000061d0: 2020 2020 2063 6f6e 7469 6e75 650d 0a20       continue.. 
-000061e0: 2020 2020 2020 2020 2020 2069 6e74 6572             inter
-000061f0: 7661 6c73 203d 206d 6178 286d 696e 2873  vals = max(min(s
-00006200: 7465 705f 696e 7465 7276 616c 5f6c 696d  tep_interval_lim
-00006210: 6974 2c20 7469 6d65 5f69 6e74 6572 7661  it, time_interva
-00006220: 6c5f 6c69 6d69 7429 2c20 3129 0d0a 2020  l_limit), 1)..  
-00006230: 2020 2020 2020 2020 2020 6561 6368 5f73            each_s
-00006240: 7465 7073 203d 2076 6f6c 756d 652f 7365  teps = volume/se
-00006250: 6c66 2e72 6573 6f6c 7574 696f 6e2f 696e  lf.resolution/in
-00006260: 7465 7276 616c 730d 0a20 2020 2020 2020  tervals..       
-00006270: 2020 2020 2065 6163 685f 6465 6c61 7920       each_delay 
-00006280: 3d20 766f 6c75 6d65 2a28 312f 7370 6565  = volume*(1/spee
-00006290: 6420 2d20 312f 7072 6573 6574 292f 696e  d - 1/preset)/in
-000062a0: 7465 7276 616c 730d 0a20 2020 2020 2020  tervals..       
-000062b0: 2020 2020 2061 7265 6120 3d20 302e 3520       area = 0.5 
-000062c0: 2a20 2876 6f6c 756d 652a 2a32 2920 2a20  * (volume**2) * 
-000062d0: 2831 2f73 656c 662e 7265 736f 6c75 7469  (1/self.resoluti
-000062e0: 6f6e 2920 2a20 2831 2f69 6e74 6572 7661  on) * (1/interva
-000062f0: 6c73 2920 2a20 2831 2f73 7065 6564 202d  ls) * (1/speed -
-00006300: 2031 2f70 7265 7365 7429 0d0a 2020 2020   1/preset)..    
-00006310: 2020 2020 2020 2020 6f75 7463 6f6d 6573          outcomes
-00006320: 5b61 7265 615d 203d 206c 6962 2e53 7065  [area] = lib.Spe
-00006330: 6564 5061 7261 6d65 7465 7273 2870 7265  edParameters(pre
-00006340: 7365 742c 2069 6e74 6572 7661 6c73 2c20  set, intervals, 
-00006350: 696e 7428 6561 6368 5f73 7465 7073 292c  int(each_steps),
-00006360: 2065 6163 685f 6465 6c61 7929 0d0a 2020   each_delay)..  
-00006370: 2020 2020 2020 6966 206c 656e 286f 7574        if len(out
-00006380: 636f 6d65 7329 203d 3d20 303a 0d0a 2020  comes) == 0:..  
-00006390: 2020 2020 2020 2020 2020 7072 696e 7428            print(
-000063a0: 224e 6f20 6665 6173 6962 6c65 2073 7065  "No feasible spe
-000063b0: 6564 2070 6172 616d 6574 6572 732e 2229  ed parameters.")
-000063c0: 0d0a 2020 2020 2020 2020 2020 2020 7265  ..            re
-000063d0: 7475 726e 206c 6962 2e53 7065 6564 5061  turn lib.SpeedPa
-000063e0: 7261 6d65 7465 7273 284e 6f6e 652c 2053  rameters(None, S
-000063f0: 5445 505f 5245 534f 4c55 5449 4f4e 2c20  TEP_RESOLUTION, 
-00006400: 5354 4550 5f52 4553 4f4c 5554 494f 4e2c  STEP_RESOLUTION,
-00006410: 2073 656c 662e 7265 7370 6f6e 7365 5f74   self.response_t
-00006420: 696d 6529 0d0a 2020 2020 2020 2020 7072  ime)..        pr
-00006430: 696e 7428 6627 4265 7374 2070 6172 616d  int(f'Best param
-00006440: 6574 6572 733a 207b 6f75 7463 6f6d 6573  eters: {outcomes
-00006450: 5b6d 696e 286f 7574 636f 6d65 7329 5d7d  [min(outcomes)]}
-00006460: 2729 0d0a 2020 2020 2020 2020 7265 7475  ')..        retu
-00006470: 726e 206f 7574 636f 6d65 735b 6d69 6e28  rn outcomes[min(
-00006480: 6f75 7463 6f6d 6573 295d 0d0a 2020 2020  outcomes)]..    
-00006490: 0d0a 2020 2020 6465 6620 5f63 6f6e 6e65  ..    def _conne
-000064a0: 6374 2873 656c 662c 2070 6f72 743a 7374  ct(self, port:st
-000064b0: 722c 2062 6175 6472 6174 653a 696e 7420  r, baudrate:int 
-000064c0: 3d20 3936 3030 2c20 7469 6d65 6f75 743a  = 9600, timeout:
-000064d0: 696e 7420 3d20 3129 3a0d 0a20 2020 2020  int = 1):..     
-000064e0: 2020 2022 2222 0d0a 2020 2020 2020 2020     """..        
-000064f0: 436f 6e6e 6563 7469 6f6e 2070 726f 6365  Connection proce
-00006500: 6475 7265 2066 6f72 2074 6f6f 6c0d 0a0d  dure for tool...
-00006510: 0a20 2020 2020 2020 2041 7267 733a 0d0a  .        Args:..
-00006520: 2020 2020 2020 2020 2020 2020 706f 7274              port
-00006530: 2028 7374 7229 3a20 434f 4d20 706f 7274   (str): COM port
-00006540: 2061 6464 7265 7373 0d0a 2020 2020 2020   address..      
-00006550: 2020 2020 2020 6261 7564 7261 7465 2028        baudrate (
-00006560: 696e 742c 206f 7074 696f 6e61 6c29 3a20  int, optional): 
-00006570: 6261 7564 7261 7465 2e20 4465 6661 756c  baudrate. Defaul
-00006580: 7473 2074 6f20 3936 3030 2e0d 0a20 2020  ts to 9600...   
-00006590: 2020 2020 2020 2020 2074 696d 656f 7574           timeout
-000065a0: 2028 696e 742c 206f 7074 696f 6e61 6c29   (int, optional)
-000065b0: 3a20 7469 6d65 6f75 7420 696e 2073 6563  : timeout in sec
-000065c0: 6f6e 6473 2e20 4465 6661 756c 7473 2074  onds. Defaults t
-000065d0: 6f20 312e 0d0a 2020 2020 2020 2020 2222  o 1...        ""
-000065e0: 220d 0a20 2020 2020 2020 2073 656c 662e  "..        self.
-000065f0: 636f 6e6e 6563 7469 6f6e 5f64 6574 6169  connection_detai
-00006600: 6c73 203d 207b 0d0a 2020 2020 2020 2020  ls = {..        
-00006610: 2020 2020 2770 6f72 7427 3a20 706f 7274      'port': port
-00006620: 2c0d 0a20 2020 2020 2020 2020 2020 2027  ,..            '
-00006630: 6261 7564 7261 7465 273a 2062 6175 6472  baudrate': baudr
-00006640: 6174 652c 0d0a 2020 2020 2020 2020 2020  ate,..          
-00006650: 2020 2774 696d 656f 7574 273a 2074 696d    'timeout': tim
-00006660: 656f 7574 0d0a 2020 2020 2020 2020 7d0d  eout..        }.
-00006670: 0a20 2020 2020 2020 2064 6576 6963 6520  .        device 
-00006680: 3d20 4e6f 6e65 0d0a 2020 2020 2020 2020  = None..        
-00006690: 7472 793a 0d0a 2020 2020 2020 2020 2020  try:..          
-000066a0: 2020 6465 7669 6365 203d 2073 6572 6961    device = seria
-000066b0: 6c2e 5365 7269 616c 2870 6f72 742c 2062  l.Serial(port, b
-000066c0: 6175 6472 6174 652c 2074 696d 656f 7574  audrate, timeout
-000066d0: 3d74 696d 656f 7574 290d 0a20 2020 2020  =timeout)..     
-000066e0: 2020 2065 7863 6570 7420 4578 6365 7074     except Except
-000066f0: 696f 6e20 6173 2065 3a0d 0a20 2020 2020  ion as e:..     
-00006700: 2020 2020 2020 2070 7269 6e74 2866 2243         print(f"C
-00006710: 6f75 6c64 206e 6f74 2063 6f6e 6e65 6374  ould not connect
-00006720: 2074 6f20 7b70 6f72 747d 2229 0d0a 2020   to {port}")..  
-00006730: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
-00006740: 662e 7665 7262 6f73 653a 0d0a 2020 2020  f.verbose:..    
-00006750: 2020 2020 2020 2020 2020 2020 7072 696e              prin
-00006760: 7428 6529 0d0a 2020 2020 2020 2020 656c  t(e)..        el
-00006770: 7365 3a0d 0a20 2020 2020 2020 2020 2020  se:..           
-00006780: 2074 696d 652e 736c 6565 7028 3229 2020   time.sleep(2)  
-00006790: 2023 2057 6169 7420 666f 7220 6772 626c   # Wait for grbl
-000067a0: 2074 6f20 696e 6974 6961 6c69 7a65 0d0a   to initialize..
-000067b0: 2020 2020 2020 2020 2020 2020 6465 7669              devi
-000067c0: 6365 2e66 6c75 7368 496e 7075 7428 290d  ce.flushInput().
-000067d0: 0a20 2020 2020 2020 2020 2020 2070 7269  .            pri
-000067e0: 6e74 2866 2243 6f6e 6e65 6374 696f 6e20  nt(f"Connection 
-000067f0: 6f70 656e 6564 2074 6f20 7b70 6f72 747d  opened to {port}
-00006800: 2229 0d0a 2020 2020 2020 2020 2020 2020  ")..            
-00006810: 7365 6c66 2e73 6574 466c 6167 2863 6f6e  self.setFlag(con
-00006820: 6e65 6374 6564 3d54 7275 6529 0d0a 2020  nected=True)..  
-00006830: 2020 2020 2020 7365 6c66 2e64 6576 6963        self.devic
-00006840: 6520 3d20 6465 7669 6365 0d0a 2020 2020  e = device..    
-00006850: 2020 2020 7365 6c66 2e67 6574 496e 666f      self.getInfo
-00006860: 2829 0d0a 2020 2020 2020 2020 7365 6c66  ()..        self
-00006870: 2e72 6573 6574 2829 0d0a 2020 2020 2020  .reset()..      
-00006880: 2020 7265 7475 726e 0d0a 2020 2020 0d0a    return..    ..
-00006890: 2020 2020 6465 6620 5f69 735f 6578 7065      def _is_expe
-000068a0: 6374 6564 5f72 6570 6c79 2873 656c 662c  cted_reply(self,
-000068b0: 2072 6573 706f 6e73 653a 7374 722c 2063   response:str, c
-000068c0: 6f6d 6d61 6e64 5f63 6f64 653a 7374 722c  ommand_code:str,
-000068d0: 202a 2a6b 7761 7267 7329 202d 3e20 626f   **kwargs) -> bo
-000068e0: 6f6c 3a0d 0a20 2020 2020 2020 2022 2222  ol:..        """
-000068f0: 0d0a 2020 2020 2020 2020 4368 6563 6b73  ..        Checks
-00006900: 2061 6e64 2072 6574 7572 6e73 2077 6865   and returns whe
-00006910: 7468 6572 2074 6865 2072 6573 706f 6e73  ther the respons
-00006920: 6520 6973 2061 6e20 6578 7065 6374 6564  e is an expected
-00006930: 2072 6570 6c79 0d0a 0d0a 2020 2020 2020   reply....      
-00006940: 2020 4172 6773 3a0d 0a20 2020 2020 2020    Args:..       
-00006950: 2020 2020 2072 6573 706f 6e73 6520 2873       response (s
-00006960: 7472 293a 2072 6573 706f 6e73 6520 7374  tr): response st
-00006970: 7269 6e67 2066 726f 6d20 6465 7669 6365  ring from device
-00006980: 0d0a 2020 2020 2020 2020 2020 2020 636f  ..            co
-00006990: 6d6d 616e 645f 636f 6465 2028 7374 7229  mmand_code (str)
-000069a0: 3a20 7477 6f2d 6368 6172 6163 7465 7220  : two-character 
-000069b0: 636f 6d6d 616e 6420 636f 6465 0d0a 0d0a  command code....
-000069c0: 2020 2020 2020 2020 5265 7475 726e 733a          Returns:
-000069d0: 0d0a 2020 2020 2020 2020 2020 2020 626f  ..            bo
-000069e0: 6f6c 3a20 7768 6574 6865 7220 7468 6520  ol: whether the 
-000069f0: 7265 7370 6f6e 7365 2069 7320 616e 2065  response is an e
-00006a00: 7870 6563 7465 6420 7265 706c 790d 0a20  xpected reply.. 
-00006a10: 2020 2020 2020 2022 2222 0d0a 2020 2020         """..    
-00006a20: 2020 2020 6966 2072 6573 706f 6e73 6520      if response 
-00006a30: 696e 206c 6962 2e45 7272 6f72 436f 6465  in lib.ErrorCode
-00006a40: 2e5f 6d65 6d62 6572 5f6e 616d 6573 5f3a  ._member_names_:
-00006a50: 0d0a 2020 2020 2020 2020 2020 2020 7265  ..            re
-00006a60: 7475 726e 2054 7275 650d 0a20 2020 2020  turn True..     
-00006a70: 2020 2069 6620 636f 6d6d 616e 645f 636f     if command_co
-00006a80: 6465 206e 6f74 2069 6e20 5155 4552 4945  de not in QUERIE
-00006a90: 5320 616e 6420 7265 7370 6f6e 7365 203d  S and response =
-00006aa0: 3d20 276f 6b27 3a0d 0a20 2020 2020 2020  = 'ok':..       
-00006ab0: 2020 2020 2072 6574 7572 6e20 5472 7565       return True
-00006ac0: 0d0a 2020 2020 2020 2020 6966 2063 6f6d  ..        if com
-00006ad0: 6d61 6e64 5f63 6f64 6520 696e 2051 5545  mand_code in QUE
-00006ae0: 5249 4553 2061 6e64 2072 6573 706f 6e73  RIES and respons
-00006af0: 655b 3a32 5d20 3d3d 2063 6f6d 6d61 6e64  e[:2] == command
-00006b00: 5f63 6f64 652e 6c6f 7765 7228 293a 0d0a  _code.lower():..
-00006b10: 2020 2020 2020 2020 2020 2020 7265 706c              repl
-00006b20: 795f 636f 6465 2c20 6461 7461 203d 2072  y_code, data = r
-00006b30: 6573 706f 6e73 655b 3a32 5d2c 2072 6573  esponse[:2], res
-00006b40: 706f 6e73 655b 323a 5d0d 0a20 2020 2020  ponse[2:]..     
-00006b50: 2020 2020 2020 2069 6620 7365 6c66 2e76         if self.v
-00006b60: 6572 626f 7365 3a0d 0a20 2020 2020 2020  erbose:..       
-00006b70: 2020 2020 2020 2020 2070 7269 6e74 2866           print(f
-00006b80: 275b 7b72 6570 6c79 5f63 6f64 657d 5d20  '[{reply_code}] 
-00006b90: 7b64 6174 617d 2729 0d0a 2020 2020 2020  {data}')..      
-00006ba0: 2020 2020 2020 7265 7475 726e 2054 7275        return Tru
-00006bb0: 650d 0a20 2020 2020 2020 2072 6574 7572  e..        retur
-00006bc0: 6e20 4661 6c73 650d 0a0d 0a20 2020 2064  n False....    d
-00006bd0: 6566 205f 6c6f 6f70 5f66 6565 6462 6163  ef _loop_feedbac
-00006be0: 6b28 7365 6c66 293a 0d0a 2020 2020 2020  k(self):..      
-00006bf0: 2020 2222 224c 6f6f 7020 746f 2063 6f6e    """Loop to con
-00006c00: 7374 616e 746c 7920 7265 6164 2066 726f  stantly read fro
-00006c10: 6d20 6465 7669 6365 2222 220d 0a20 2020  m device"""..   
-00006c20: 2020 2020 2070 7269 6e74 2827 4c69 7374       print('List
-00006c30: 656e 696e 672e 2e2e 2729 0d0a 2020 2020  ening...')..    
-00006c40: 2020 2020 7768 696c 6520 7365 6c66 2e66      while self.f
-00006c50: 6c61 6773 5b27 6765 745f 6665 6564 6261  lags['get_feedba
-00006c60: 636b 275d 3a0d 0a20 2020 2020 2020 2020  ck']:..         
-00006c70: 2020 2069 6620 7365 6c66 2e66 6c61 6773     if self.flags
-00006c80: 5b27 7061 7573 655f 6665 6564 6261 636b  ['pause_feedback
-00006c90: 275d 3a0d 0a20 2020 2020 2020 2020 2020  ']:..           
-00006ca0: 2020 2020 2063 6f6e 7469 6e75 650d 0a20       continue.. 
-00006cb0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00006cc0: 6765 7453 7461 7475 7328 290d 0a20 2020  getStatus()..   
-00006cd0: 2020 2020 2020 2020 2073 656c 662e 6765           self.ge
-00006ce0: 7443 6170 6163 6974 616e 6365 2829 0d0a  tCapacitance()..
-00006cf0: 2020 2020 2020 2020 7072 696e 7428 2753          print('S
-00006d00: 746f 7020 6c69 7374 656e 696e 672e 2e2e  top listening...
-00006d10: 2729 0d0a 2020 2020 2020 2020 7265 7475  ')..        retu
-00006d20: 726e 0d0a 2020 2020 0d0a 2020 2020 6465  rn..    ..    de
-00006d30: 6620 5f71 7565 7279 2873 656c 662c 200d  f _query(self, .
-00006d40: 0a20 2020 2020 2020 2063 6f6d 6d61 6e64  .        command
-00006d50: 3a20 7374 722c 200d 0a20 2020 2020 2020  : str, ..       
-00006d60: 2074 696d 656f 7574 5f73 3a20 666c 6f61   timeout_s: floa
-00006d70: 7420 3d20 302e 332c 200d 0a20 2020 2020  t = 0.3, ..     
-00006d80: 2020 2072 6573 756d 655f 6665 6564 6261     resume_feedba
-00006d90: 636b 3a20 626f 6f6c 203d 2046 616c 7365  ck: bool = False
-00006da0: 2c0d 0a20 2020 2020 2020 2067 6574 5f70  ,..        get_p
-00006db0: 6f73 6974 696f 6e3a 2062 6f6f 6c20 3d20  osition: bool = 
-00006dc0: 5472 7565 0d0a 2020 2020 2920 2d3e 2073  True..    ) -> s
-00006dd0: 7472 3a0d 0a20 2020 2020 2020 2022 2222  tr:..        """
-00006de0: 0d0a 2020 2020 2020 2020 5772 6974 6520  ..        Write 
-00006df0: 636f 6d6d 616e 6420 746f 2061 6e64 2072  command to and r
-00006e00: 6561 6420 7265 7370 6f6e 7365 2066 726f  ead response fro
-00006e10: 6d20 6465 7669 6365 0d0a 0d0a 2020 2020  m device....    
-00006e20: 2020 2020 4172 6773 3a0d 0a20 2020 2020      Args:..     
-00006e30: 2020 2020 2020 2063 6f6d 6d61 6e64 2028         command (
-00006e40: 7374 7229 3a20 636f 6d6d 616e 6420 7374  str): command st
-00006e50: 7269 6e67 0d0a 2020 2020 2020 2020 2020  ring..          
-00006e60: 2020 7469 6d65 6f75 745f 7320 2866 6c6f    timeout_s (flo
-00006e70: 6174 2c20 6f70 7469 6f6e 616c 293a 2064  at, optional): d
-00006e80: 7572 6174 696f 6e20 746f 2077 6169 7420  uration to wait 
-00006e90: 6265 666f 7265 2074 696d 656f 7574 2e20  before timeout. 
-00006ea0: 4465 6661 756c 7473 2074 6f20 302e 332e  Defaults to 0.3.
-00006eb0: 0d0a 2020 2020 2020 2020 2020 2020 7265  ..            re
-00006ec0: 7375 6d65 5f66 6565 6462 6163 6b20 2862  sume_feedback (b
-00006ed0: 6f6f 6c2c 206f 7074 696f 6e61 6c29 3a20  ool, optional): 
-00006ee0: 7768 6574 6865 7220 746f 2072 6573 756d  whether to resum
-00006ef0: 6520 7265 6164 696e 6720 6672 6f6d 2064  e reading from d
-00006f00: 6576 6963 652e 2044 6566 6175 6c74 7320  evice. Defaults 
-00006f10: 746f 2046 616c 7365 2e0d 0a20 2020 2020  to False...     
-00006f20: 2020 2020 2020 2067 6574 5f70 6f73 6974         get_posit
-00006f30: 696f 6e20 2862 6f6f 6c2c 206f 7074 696f  ion (bool, optio
-00006f40: 6e61 6c29 3a20 7768 6574 6865 7220 746f  nal): whether to
-00006f50: 2067 6574 2074 6865 2070 6f73 6974 696f   get the positio
-00006f60: 6e20 6f66 2074 6865 2070 6c75 6e67 6572  n of the plunger
-00006f70: 2e20 4465 6661 756c 7473 2074 6f20 5472  . Defaults to Tr
-00006f80: 7565 2e0d 0a20 2020 2020 2020 2052 6574  ue...        Ret
-00006f90: 7572 6e73 3a0d 0a20 2020 2020 2020 2020  urns:..         
-00006fa0: 2020 2073 7472 3a20 7265 7370 6f6e 7365     str: response
-00006fb0: 2073 7472 696e 670d 0a20 2020 2020 2020   string..       
-00006fc0: 2022 2222 0d0a 2020 2020 2020 2020 636f   """..        co
-00006fd0: 6d6d 616e 645f 636f 6465 203d 2063 6f6d  mmand_code = com
-00006fe0: 6d61 6e64 5b3a 325d 0d0a 2020 2020 2020  mand[:2]..      
-00006ff0: 2020 6966 2063 6f6d 6d61 6e64 5f63 6f64    if command_cod
-00007000: 6520 6e6f 7420 696e 206c 6962 2e53 7461  e not in lib.Sta
-00007010: 7475 7351 7565 7279 436f 6465 2e5f 6d65  tusQueryCode._me
-00007020: 6d62 6572 5f6e 616d 6573 5f3a 0d0a 2020  mber_names_:..  
-00007030: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
-00007040: 662e 666c 6167 735b 2767 6574 5f66 6565  f.flags['get_fee
-00007050: 6462 6163 6b27 5d20 616e 6420 6e6f 7420  dback'] and not 
-00007060: 7365 6c66 2e66 6c61 6773 5b27 7061 7573  self.flags['paus
-00007070: 655f 6665 6564 6261 636b 275d 3a0d 0a20  e_feedback']:.. 
-00007080: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00007090: 656c 662e 7365 7446 6c61 6728 7061 7573  elf.setFlag(paus
-000070a0: 655f 6665 6564 6261 636b 3d54 7275 6529  e_feedback=True)
-000070b0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000070c0: 2020 7469 6d65 2e73 6c65 6570 2874 696d    time.sleep(tim
-000070d0: 656f 7574 5f73 290d 0a20 2020 2020 2020  eout_s)..       
-000070e0: 2020 2020 2023 2073 656c 662e 6765 7453       # self.getS
-000070f0: 7461 7475 7328 290d 0a20 2020 2020 2020  tatus()..       
-00007100: 2020 2020 2023 2077 6869 6c65 2073 656c       # while sel
-00007110: 662e 6973 4275 7379 2829 3a0d 0a20 2020  f.isBusy():..   
-00007120: 2020 2020 2020 2020 2023 2020 2020 2073           #     s
-00007130: 656c 662e 6765 7453 7461 7475 7328 290d  elf.getStatus().
-00007140: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-00007150: 7365 6c66 2e69 7342 7573 7928 293a 0d0a  self.isBusy():..
-00007160: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007170: 7469 6d65 2e73 6c65 6570 2874 696d 656f  time.sleep(timeo
-00007180: 7574 5f73 290d 0a20 2020 2020 2020 200d  ut_s)..        .
-00007190: 0a20 2020 2020 2020 2073 7461 7274 5f74  .        start_t
-000071a0: 696d 6520 3d20 7469 6d65 2e70 6572 665f  ime = time.perf_
-000071b0: 636f 756e 7465 7228 290d 0a20 2020 2020  counter()..     
-000071c0: 2020 2073 656c 662e 5f77 7269 7465 2863     self._write(c
-000071d0: 6f6d 6d61 6e64 290d 0a20 2020 2020 2020  ommand)..       
-000071e0: 2072 6573 706f 6e73 6520 3d20 2727 0d0a   response = ''..
-000071f0: 2020 2020 2020 2020 7768 696c 6520 6e6f          while no
-00007200: 7420 7365 6c66 2e5f 6973 5f65 7870 6563  t self._is_expec
-00007210: 7465 645f 7265 706c 7928 7265 7370 6f6e  ted_reply(respon
-00007220: 7365 2c20 636f 6d6d 616e 645f 636f 6465  se, command_code
-00007230: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
-00007240: 6966 2074 696d 652e 7065 7266 5f63 6f75  if time.perf_cou
-00007250: 6e74 6572 2829 202d 2073 7461 7274 5f74  nter() - start_t
-00007260: 696d 6520 3e20 7469 6d65 6f75 745f 733a  ime > timeout_s:
-00007270: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00007280: 2020 6272 6561 6b0d 0a20 2020 2020 2020    break..       
-00007290: 2020 2020 2072 6573 706f 6e73 6520 3d20       response = 
-000072a0: 7365 6c66 2e5f 7265 6164 2829 0d0a 2020  self._read()..  
-000072b0: 2020 2020 2020 2320 7072 696e 7428 7469        # print(ti
-000072c0: 6d65 2e70 6572 665f 636f 756e 7465 7228  me.perf_counter(
-000072d0: 2920 2d20 7374 6172 745f 7469 6d65 290d  ) - start_time).
-000072e0: 0a20 2020 2020 2020 2069 6620 636f 6d6d  .        if comm
-000072f0: 616e 645f 636f 6465 2069 6e20 5155 4552  and_code in QUER
-00007300: 4945 533a 0d0a 2020 2020 2020 2020 2020  IES:..          
-00007310: 2020 7265 7370 6f6e 7365 203d 2072 6573    response = res
-00007320: 706f 6e73 655b 323a 5d0d 0a20 2020 2020  ponse[2:]..     
-00007330: 2020 2069 6620 636f 6d6d 616e 645f 636f     if command_co
-00007340: 6465 206e 6f74 2069 6e20 6c69 622e 5374  de not in lib.St
-00007350: 6174 7573 5175 6572 7943 6f64 652e 5f6d  atusQueryCode._m
-00007360: 656d 6265 725f 6e61 6d65 735f 3a0d 0a20  ember_names_:.. 
-00007370: 2020 2020 2020 2020 2020 2069 6620 6765             if ge
-00007380: 745f 706f 7369 7469 6f6e 3a0d 0a20 2020  t_position:..   
-00007390: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-000073a0: 662e 6765 7450 6f73 6974 696f 6e28 290d  f.getPosition().
-000073b0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-000073c0: 7265 7375 6d65 5f66 6565 6462 6163 6b3a  resume_feedback:
-000073d0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000073e0: 2020 7365 6c66 2e73 6574 466c 6167 2870    self.setFlag(p
-000073f0: 6175 7365 5f66 6565 6462 6163 6b3d 4661  ause_feedback=Fa
-00007400: 6c73 6529 0d0a 2020 2020 2020 2020 7265  lse)..        re
-00007410: 7475 726e 2072 6573 706f 6e73 650d 0a0d  turn response...
-00007420: 0a20 2020 2064 6566 205f 7265 6164 2873  .    def _read(s
-00007430: 656c 6629 202d 3e20 7374 723a 0d0a 2020  elf) -> str:..  
-00007440: 2020 2020 2020 2222 220d 0a20 2020 2020        """..     
-00007450: 2020 2052 6561 6420 7265 7370 6f6e 7365     Read response
-00007460: 2066 726f 6d20 6465 7669 6365 0d0a 0d0a   from device....
-00007470: 2020 2020 2020 2020 5265 7475 726e 733a          Returns:
-00007480: 0d0a 2020 2020 2020 2020 2020 2020 7374  ..            st
-00007490: 723a 2072 6573 706f 6e73 6520 7374 7269  r: response stri
-000074a0: 6e67 0d0a 2020 2020 2020 2020 2222 220d  ng..        """.
-000074b0: 0a20 2020 2020 2020 2072 6573 706f 6e73  .        respons
-000074c0: 6520 3d20 2727 0d0a 2020 2020 2020 2020  e = ''..        
-000074d0: 7472 793a 0d0a 2020 2020 2020 2020 2020  try:..          
-000074e0: 2020 7265 7370 6f6e 7365 203d 2073 656c    response = sel
-000074f0: 662e 6465 7669 6365 2e72 6561 646c 696e  f.device.readlin
-00007500: 6528 290d 0a20 2020 2020 2020 2020 2020  e()..           
-00007510: 2069 6620 6c65 6e28 7265 7370 6f6e 7365   if len(response
-00007520: 2920 3d3d 2030 3a0d 0a20 2020 2020 2020  ) == 0:..       
-00007530: 2020 2020 2020 2020 2072 6573 706f 6e73           respons
-00007540: 6520 3d20 7365 6c66 2e64 6576 6963 652e  e = self.device.
-00007550: 7265 6164 6c69 6e65 2829 0d0a 2020 2020  readline()..    
-00007560: 2020 2020 2020 2020 7265 7370 6f6e 7365          response
-00007570: 203d 2072 6573 706f 6e73 655b 323a 2d32   = response[2:-2
-00007580: 5d2e 6465 636f 6465 2827 7574 662d 3827  ].decode('utf-8'
-00007590: 290d 0a20 2020 2020 2020 2065 7863 6570  )..        excep
-000075a0: 7420 4174 7472 6962 7574 6545 7272 6f72  t AttributeError
-000075b0: 3a0d 0a20 2020 2020 2020 2020 2020 2070  :..            p
-000075c0: 6173 730d 0a20 2020 2020 2020 2065 7863  ass..        exc
-000075d0: 6570 7420 4578 6365 7074 696f 6e20 6173  ept Exception as
-000075e0: 2065 3a0d 0a20 2020 2020 2020 2020 2020   e:..           
-000075f0: 2069 6620 7365 6c66 2e76 6572 626f 7365   if self.verbose
-00007600: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-00007610: 2020 2070 7269 6e74 2865 290d 0a20 2020     print(e)..   
-00007620: 2020 2020 2069 6620 7265 7370 6f6e 7365       if response
-00007630: 2069 6e20 6c69 622e 4572 726f 7243 6f64   in lib.ErrorCod
-00007640: 652e 5f6d 656d 6265 725f 6e61 6d65 735f  e._member_names_
-00007650: 3a0d 0a20 2020 2020 2020 2020 2020 2070  :..            p
-00007660: 7269 6e74 286c 6962 2e45 7272 6f72 436f  rint(lib.ErrorCo
-00007670: 6465 5b72 6573 706f 6e73 655d 2e76 616c  de[response].val
-00007680: 7565 290d 0a20 2020 2020 2020 2072 6574  ue)..        ret
-00007690: 7572 6e20 7265 7370 6f6e 7365 0d0a 2020  urn response..  
-000076a0: 2020 0d0a 2020 2020 6465 6620 5f73 6574    ..    def _set
-000076b0: 5f63 6861 6e6e 656c 5f69 6428 7365 6c66  _channel_id(self
-000076c0: 2c20 6e65 775f 6368 616e 6e65 6c5f 6964  , new_channel_id
-000076d0: 3a69 6e74 293a 0d0a 2020 2020 2020 2020  :int):..        
-000076e0: 2222 220d 0a20 2020 2020 2020 2053 6574  """..        Set
-000076f0: 2063 6861 6e6e 656c 2069 6420 6f66 2064   channel id of d
-00007700: 6576 6963 650d 0a0d 0a20 2020 2020 2020  evice....       
-00007710: 2041 7267 733a 0d0a 2020 2020 2020 2020   Args:..        
-00007720: 2020 2020 6e65 775f 6368 616e 6e65 6c20      new_channel 
-00007730: 2869 6e74 293a 206e 6577 2063 6861 6e6e  (int): new chann
-00007740: 656c 2069 640d 0a0d 0a20 2020 2020 2020  el id....       
-00007750: 2052 6169 7365 733a 0d0a 2020 2020 2020   Raises:..      
-00007760: 2020 2020 2020 5661 6c75 6545 7272 6f72        ValueError
-00007770: 3a20 506c 6561 7365 2073 656c 6563 7420  : Please select 
-00007780: 6120 7661 6c69 6420 724c 696e 6520 6164  a valid rLine ad
-00007790: 6472 6573 7320 6672 6f6d 2031 2074 6f20  dress from 1 to 
-000077a0: 390d 0a20 2020 2020 2020 2022 2222 0d0a  9..        """..
-000077b0: 2020 2020 2020 2020 6966 206e 6f74 2028          if not (
-000077c0: 3020 3c20 6e65 775f 6368 616e 6e65 6c5f  0 < new_channel_
-000077d0: 6964 203c 2031 3029 3a0d 0a20 2020 2020  id < 10):..     
-000077e0: 2020 2020 2020 2072 6169 7365 2056 616c         raise Val
-000077f0: 7565 4572 726f 7228 2750 6c65 6173 6520  ueError('Please 
-00007800: 7365 6c65 6374 2061 2076 616c 6964 2072  select a valid r
-00007810: 4c69 6e65 2061 6464 7265 7373 2066 726f  Line address fro
-00007820: 6d20 3120 746f 2039 2e27 290d 0a20 2020  m 1 to 9.')..   
-00007830: 2020 2020 2072 6573 706f 6e73 6520 3d20       response = 
-00007840: 7365 6c66 2e5f 7175 6572 7928 6627 2a41  self._query(f'*A
-00007850: 7b6e 6577 5f63 6861 6e6e 656c 5f69 647d  {new_channel_id}
-00007860: 2729 0d0a 2020 2020 2020 2020 6966 2072  ')..        if r
-00007870: 6573 706f 6e73 6520 3d3d 2027 6f6b 273a  esponse == 'ok':
-00007880: 0d0a 2020 2020 2020 2020 2020 2020 7365  ..            se
-00007890: 6c66 2e63 6861 6e6e 656c 203d 206e 6577  lf.channel = new
-000078a0: 5f63 6861 6e6e 656c 5f69 640d 0a20 2020  _channel_id..   
-000078b0: 2020 2020 2072 6574 7572 6e0d 0a20 2020       return..   
-000078c0: 200d 0a20 2020 2064 6566 205f 7772 6974   ..    def _writ
-000078d0: 6528 7365 6c66 2c20 636f 6d6d 616e 643a  e(self, command:
-000078e0: 7374 7229 202d 3e20 626f 6f6c 3a0d 0a20  str) -> bool:.. 
-000078f0: 2020 2020 2020 2022 2222 0d0a 2020 2020         """..    
-00007900: 2020 2020 5772 6974 6520 636f 6d6d 616e      Write comman
-00007910: 6420 746f 2064 6576 6963 650d 0a0d 0a20  d to device.... 
-00007920: 2020 2020 2020 2041 7267 733a 0d0a 2020         Args:..  
-00007930: 2020 2020 2020 2020 2020 636f 6d6d 616e            comman
-00007940: 6420 2873 7472 293a 203c 636f 6d6d 616e  d (str): <comman
-00007950: 6420 636f 6465 3e3c 7661 6c75 653e 0d0a  d code><value>..
-00007960: 0d0a 2020 2020 2020 2020 5265 7475 726e  ..        Return
-00007970: 733a 0d0a 2020 2020 2020 2020 2020 2020  s:..            
-00007980: 626f 6f6c 3a20 7768 6574 6865 7220 636f  bool: whether co
-00007990: 6d6d 616e 6420 7761 7320 7365 6e74 2073  mmand was sent s
-000079a0: 7563 6365 7373 6675 6c6c 790d 0a20 2020  uccessfully..   
-000079b0: 2020 2020 2022 2222 0d0a 2020 2020 2020       """..      
-000079c0: 2020 6966 2073 656c 662e 7665 7262 6f73    if self.verbos
-000079d0: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
-000079e0: 7072 696e 7428 636f 6d6d 616e 6429 0d0a  print(command)..
-000079f0: 2020 2020 2020 2020 6673 7472 696e 6720          fstring 
-00007a00: 3d20 6627 017b 7365 6c66 2e63 6861 6e6e  = f'.{self.chann
-00007a10: 656c 7d7b 636f 6d6d 616e 647d c2ba 5c72  el}{command}..\r
-00007a20: 2720 2320 636f 6d6d 616e 6420 7465 6d70  ' # command temp
-00007a30: 6c61 7465 3a20 3c50 5245 3e3c 4144 523e  late: <PRE><ADR>
-00007a40: 3c43 4f44 453e 3c44 4154 413e 3c4c 5243  <CODE><DATA><LRC
-00007a50: 3e3c 504f 5354 3e0d 0a20 2020 2020 2020  ><POST>..       
-00007a60: 2023 2062 7374 7269 6e67 203d 2062 7974   # bstring = byt
-00007a70: 6561 7272 6179 2e66 726f 6d68 6578 2866  earray.fromhex(f
-00007a80: 7374 7269 6e67 2e65 6e63 6f64 6528 2775  string.encode('u
-00007a90: 7466 2d38 2729 2e68 6578 2829 290d 0a20  tf-8').hex()).. 
-00007aa0: 2020 2020 2020 2074 7279 3a0d 0a20 2020         try:..   
-00007ab0: 2020 2020 2020 2020 2023 2054 7970 6963           # Typic
-00007ac0: 616c 2074 696d 656f 7574 2077 6169 7420  al timeout wait 
-00007ad0: 6973 2034 3030 6d73 0d0a 2020 2020 2020  is 400ms..      
-00007ae0: 2020 2020 2020 7365 6c66 2e64 6576 6963        self.devic
-00007af0: 652e 7772 6974 6528 6673 7472 696e 672e  e.write(fstring.
-00007b00: 656e 636f 6465 2827 7574 662d 3827 2929  encode('utf-8'))
-00007b10: 0d0a 2020 2020 2020 2020 6578 6365 7074  ..        except
-00007b20: 2041 7474 7269 6275 7465 4572 726f 723a   AttributeError:
-00007b30: 0d0a 2020 2020 2020 2020 2020 2020 7061  ..            pa
-00007b40: 7373 0d0a 2020 2020 2020 2020 6578 6365  ss..        exce
-00007b50: 7074 2045 7863 6570 7469 6f6e 2061 7320  pt Exception as 
-00007b60: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
-00007b70: 6966 2073 656c 662e 7665 7262 6f73 653a  if self.verbose:
-00007b80: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00007b90: 2020 7072 696e 7428 6529 0d0a 2020 2020    print(e)..    
-00007ba0: 2020 2020 2020 2020 7265 7475 726e 2046          return F
-00007bb0: 616c 7365 0d0a 2020 2020 2020 2020 7265  alse..        re
-00007bc0: 7475 726e 2054 7275 650d 0a20 2020 20    turn True..    
+000004c0: 7469 705f 696e 7365 745f 6d6d 6020 2866  tip_inset_mm` (f
+000004d0: 6c6f 6174 2c20 6f70 7469 6f6e 616c 293a  loat, optional):
+000004e0: 206c 656e 6774 6820 6f66 2070 6970 6574   length of pipet
+000004f0: 7465 2074 6861 7420 6973 2069 6e73 6572  te that is inser
+00000500: 7465 6420 696e 746f 2074 6865 2070 6970  ted into the pip
+00000510: 6574 7465 2074 6970 2e20 4465 6661 756c  ette tip. Defaul
+00000520: 7473 2074 6f20 3132 2e0d 0a20 2020 2020  ts to 12...     
+00000530: 2020 2060 7469 705f 7468 7265 7368 6f6c     `tip_threshol
+00000540: 6460 2028 696e 742c 206f 7074 696f 6e61  d` (int, optiona
+00000550: 6c29 3a20 7468 7265 7368 6f6c 6420 6162  l): threshold ab
+00000560: 6f76 6520 7768 6963 6820 6120 636f 6e64  ove which a cond
+00000570: 7563 7469 7665 2070 6970 6574 7465 2074  uctive pipette t
+00000580: 6970 2069 7320 636f 6e73 6964 6572 6564  ip is considered
+00000590: 2074 6f20 6265 2061 7474 6163 6865 642e   to be attached.
+000005a0: 2044 6566 6175 6c74 7320 746f 2032 3736   Defaults to 276
+000005b0: 2e0d 0a20 2020 200d 0a20 2020 2023 2323  ...    ..    ###
+000005c0: 2041 7474 7269 6275 7465 730d 0a20 2020   Attributes..   
+000005d0: 202d 2060 6368 616e 6e65 6c60 2028 696e   - `channel` (in
+000005e0: 7429 3a20 6368 616e 6e65 6c20 6964 0d0a  t): channel id..
+000005f0: 2020 2020 2d20 606c 696d 6974 7360 2028      - `limits` (
+00000600: 7475 706c 655b 696e 745d 293a 206c 6f77  tuple[int]): low
+00000610: 6572 2061 6e64 2075 7070 6572 2073 7465  er and upper ste
+00000620: 7020 6c69 6d69 7473 0d0a 2020 2020 2d20  p limits..    - 
+00000630: 606d 6f64 656c 5f69 6e66 6f60 2028 5361  `model_info` (Sa
+00000640: 7274 6f72 6975 7350 6970 6574 7465 4d6f  rtoriusPipetteMo
+00000650: 6465 6c29 3a20 5361 7274 6f72 6975 7320  del): Sartorius 
+00000660: 6d6f 6465 6c20 696e 666f 0d0a 2020 2020  model info..    
+00000670: 2d20 606f 6666 7365 7460 2028 7475 706c  - `offset` (tupl
+00000680: 655b 666c 6f61 745d 293a 2078 2c79 2c7a  e[float]): x,y,z
+00000690: 206f 6666 7365 7420 6f66 2074 6970 0d0a   offset of tip..
+000006a0: 2020 2020 2d20 6070 6f73 6974 696f 6e60      - `position`
+000006b0: 2028 696e 7429 3a20 706f 7369 7469 6f6e   (int): position
+000006c0: 206f 6620 706c 756e 6765 720d 0a20 2020   of plunger..   
+000006d0: 202d 2060 7265 7370 6f6e 7365 5f74 696d   - `response_tim
+000006e0: 6560 2028 666c 6f61 7429 3a20 6465 6c61  e` (float): dela
+000006f0: 7920 6265 7477 6565 6e20 7365 6e64 696e  y between sendin
+00000700: 6720 6120 636f 6d6d 616e 6420 616e 6420  g a command and 
+00000710: 7265 6365 6976 696e 6720 6120 7265 7370  receiving a resp
+00000720: 6f6e 7365 2c20 696e 2073 6563 6f6e 6473  onse, in seconds
+00000730: 0d0a 2020 2020 2d20 6073 7065 6564 5f63  ..    - `speed_c
+00000740: 6f64 6560 2028 5370 6565 6429 3a20 636f  ode` (Speed): co
+00000750: 6465 7320 666f 7220 6173 7069 7261 7465  des for aspirate
+00000760: 2061 6e64 2064 6973 7065 6e73 6520 7370   and dispense sp
+00000770: 6565 6473 0d0a 2020 2020 2d20 6073 7065  eeds..    - `spe
+00000780: 6564 5f70 7265 7365 7473 6020 2850 7265  ed_presets` (Pre
+00000790: 7365 7453 7065 6564 7329 3a20 7072 6573  setSpeeds): pres
+000007a0: 6574 2073 7065 6564 7320 6176 6169 6c61  et speeds availa
+000007b0: 626c 650d 0a20 2020 202d 2060 7469 705f  ble..    - `tip_
+000007c0: 696e 7365 745f 6d6d 6020 2866 6c6f 6174  inset_mm` (float
+000007d0: 293a 206c 656e 6774 6820 6f66 2070 6970  ): length of pip
+000007e0: 6574 7465 2074 6861 7420 6973 2069 6e73  ette that is ins
+000007f0: 6572 7465 6420 696e 746f 2074 6865 2070  erted into the p
+00000800: 6970 6574 7465 2074 6970 0d0a 2020 2020  ipette tip..    
+00000810: 2d20 6074 6970 5f6c 656e 6774 6860 2028  - `tip_length` (
+00000820: 666c 6f61 7429 3a20 6c65 6e67 7468 206f  float): length o
+00000830: 6620 7069 7065 7474 6520 7469 700d 0a20  f pipette tip.. 
+00000840: 2020 202d 2060 7469 705f 7468 7265 7368     - `tip_thresh
+00000850: 6f6c 6460 2028 696e 7429 3a20 7468 7265  old` (int): thre
+00000860: 7368 6f6c 6420 6162 6f76 6520 7768 6963  shold above whic
+00000870: 6820 6120 636f 6e64 7563 7469 7665 2070  h a conductive p
+00000880: 6970 6574 7465 2074 6970 2069 7320 636f  ipette tip is co
+00000890: 6e73 6964 6572 6564 2074 6f20 6265 2061  nsidered to be a
+000008a0: 7474 6163 6865 640d 0a20 2020 200d 0a20  ttached..    .. 
+000008b0: 2020 2023 2323 2050 726f 7065 7274 6965     ### Propertie
+000008c0: 730d 0a20 2020 202d 2060 6361 7061 6369  s..    - `capaci
+000008d0: 7461 6e63 6560 2028 696e 7429 3a20 6361  tance` (int): ca
+000008e0: 7061 6369 7461 6e63 6520 6173 206d 6561  pacitance as mea
+000008f0: 7375 7265 6420 6174 2074 6865 2065 6e64  sured at the end
+00000900: 206f 6620 7468 6520 7069 7065 7474 650d   of the pipette.
+00000910: 0a20 2020 202d 2060 686f 6d65 5f70 6f73  .    - `home_pos
+00000920: 6974 696f 6e60 2028 696e 7429 3a20 686f  ition` (int): ho
+00000930: 6d65 2070 6f73 6974 696f 6e20 6f66 2070  me position of p
+00000940: 6970 6574 7465 0d0a 2020 2020 2d20 6070  ipette..    - `p
+00000950: 6f72 7460 2028 7374 7229 3a20 434f 4d20  ort` (str): COM 
+00000960: 706f 7274 2061 6464 7265 7373 0d0a 2020  port address..  
+00000970: 2020 2d20 6072 6573 6f6c 7574 696f 6e60    - `resolution`
+00000980: 2028 666c 6f61 7429 3a20 766f 6c75 6d65   (float): volume
+00000990: 2072 6573 6f6c 7574 696f 6e20 6f66 2070   resolution of p
+000009a0: 6970 6574 7465 2028 692e 652e 2075 4c20  ipette (i.e. uL 
+000009b0: 7065 7220 7374 6570 290d 0a20 2020 202d  per step)..    -
+000009c0: 2060 7374 6174 7573 6020 2873 7472 293a   `status` (str):
+000009d0: 2070 6970 6574 7465 2073 7461 7475 730d   pipette status.
+000009e0: 0a20 2020 200d 0a20 2020 2023 2323 204d  .    ..    ### M
+000009f0: 6574 686f 6473 0d0a 2020 2020 2d20 6061  ethods..    - `a
+00000a00: 6464 4169 7247 6170 603a 2063 7265 6174  ddAirGap`: creat
+00000a10: 6520 616e 2061 6972 2067 6170 2062 6574  e an air gap bet
+00000a20: 7765 656e 2074 776f 2076 6f6c 756d 6573  ween two volumes
+00000a30: 206f 6620 6c69 7175 6964 2069 6e20 7069   of liquid in pi
+00000a40: 7065 7474 650d 0a20 2020 202d 2060 6173  pette..    - `as
+00000a50: 7069 7261 7465 603a 2061 7370 6972 6174  pirate`: aspirat
+00000a60: 6520 6465 7369 7265 6420 766f 6c75 6d65  e desired volume
+00000a70: 206f 6620 7265 6167 656e 7420 696e 746f   of reagent into
+00000a80: 2070 6970 6574 7465 0d0a 2020 2020 2d20   pipette..    - 
+00000a90: 6062 6c6f 776f 7574 603a 2062 6c6f 776f  `blowout`: blowo
+00000aa0: 7574 206c 6971 7569 6420 6672 6f6d 2074  ut liquid from t
+00000ab0: 6970 0d0a 2020 2020 2d20 6064 6973 7065  ip..    - `dispe
+00000ac0: 6e73 6560 3a20 6469 7370 656e 7365 2064  nse`: dispense d
+00000ad0: 6573 6972 6564 2076 6f6c 756d 6520 6f66  esired volume of
+00000ae0: 2072 6561 6765 6e74 0d0a 2020 2020 2d20   reagent..    - 
+00000af0: 6065 6a65 6374 603a 2065 6a65 6374 2074  `eject`: eject t
+00000b00: 6865 2070 6970 6574 7465 2074 6970 0d0a  he pipette tip..
+00000b10: 2020 2020 2d20 6065 6d70 7479 603a 2065      - `empty`: e
+00000b20: 6d70 7479 2074 6865 2070 6970 6574 7465  mpty the pipette
+00000b30: 0d0a 2020 2020 2d20 6067 6574 4361 7061  ..    - `getCapa
+00000b40: 6369 7461 6e63 6560 3a20 6765 7420 7468  citance`: get th
+00000b50: 6520 6361 7061 6369 7461 6e63 6520 6173  e capacitance as
+00000b60: 206d 6561 7375 7265 6420 6174 2074 6865   measured at the
+00000b70: 2065 6e64 206f 6620 7468 6520 7069 7065   end of the pipe
+00000b80: 7474 650d 0a20 2020 202d 2060 6765 7445  tte..    - `getE
+00000b90: 7272 6f72 7360 3a20 6765 7420 6572 726f  rrors`: get erro
+00000ba0: 7273 2066 726f 6d20 7468 6520 6465 7669  rs from the devi
+00000bb0: 6365 0d0a 2020 2020 2d20 6067 6574 496e  ce..    - `getIn
+00000bc0: 666f 603a 2067 6574 2064 6574 6169 6c73  fo`: get details
+00000bd0: 206f 6620 7468 6520 5361 7274 6f72 6975   of the Sartoriu
+00000be0: 7320 7069 7065 7474 6520 6d6f 6465 6c0d  s pipette model.
+00000bf0: 0a20 2020 202d 2060 6765 7450 6f73 6974  .    - `getPosit
+00000c00: 696f 6e60 3a20 6765 7420 7468 6520 6375  ion`: get the cu
+00000c10: 7272 656e 7420 706f 7369 7469 6f6e 206f  rrent position o
+00000c20: 6620 7468 6520 7069 7065 7474 650d 0a20  f the pipette.. 
+00000c30: 2020 202d 2060 6765 7453 7461 7475 7360     - `getStatus`
+00000c40: 3a20 6765 7420 7468 6520 7374 6174 7573  : get the status
+00000c50: 206f 6620 7468 6520 7069 7065 7474 650d   of the pipette.
+00000c60: 0a20 2020 202d 2060 686f 6d65 603a 2072  .    - `home`: r
+00000c70: 6574 7572 6e20 706c 756e 6765 7220 746f  eturn plunger to
+00000c80: 2068 6f6d 6520 706f 7369 7469 6f6e 0d0a   home position..
+00000c90: 2020 2020 2d20 6069 7346 6561 7369 626c      - `isFeasibl
+00000ca0: 6560 3a20 6368 6563 6b73 2061 6e64 2072  e`: checks and r
+00000cb0: 6574 7572 6e73 2077 6865 7468 6572 2074  eturns whether t
+00000cc0: 6865 2070 6c75 6e67 6572 2070 6f73 6974  he plunger posit
+00000cd0: 696f 6e20 6973 2066 6561 7369 626c 650d  ion is feasible.
+00000ce0: 0a20 2020 202d 2060 6973 5469 704f 6e60  .    - `isTipOn`
+00000cf0: 3a20 6368 6563 6b73 2061 6e64 2072 6574  : checks and ret
+00000d00: 7572 6e73 2077 6865 7468 6572 2061 2070  urns whether a p
+00000d10: 6970 6574 7465 2074 6970 2069 7320 6174  ipette tip is at
+00000d20: 7461 6368 6564 0d0a 2020 2020 2d20 606d  tached..    - `m
+00000d30: 6f76 6560 3a20 6d6f 7665 2074 6865 2070  ove`: move the p
+00000d40: 6c75 6e67 6572 2065 6974 6865 7220 7570  lunger either up
+00000d50: 206f 7220 646f 776e 2062 7920 6120 7370   or down by a sp
+00000d60: 6563 6966 6965 6420 6e75 6d62 6572 206f  ecified number o
+00000d70: 6620 7374 6570 730d 0a20 2020 202d 2060  f steps..    - `
+00000d80: 6d6f 7665 4279 603a 206d 6f76 6520 7468  moveBy`: move th
+00000d90: 6520 706c 756e 6765 7220 6279 2061 2073  e plunger by a s
+00000da0: 7065 6369 6669 6564 206e 756d 6265 7220  pecified number 
+00000db0: 6f66 2073 7465 7073 0d0a 2020 2020 2d20  of steps..    - 
+00000dc0: 606d 6f76 6554 6f60 3a20 6d6f 7665 2074  `moveTo`: move t
+00000dd0: 6865 2070 6c75 6e67 6572 2074 6f20 6120  he plunger to a 
+00000de0: 7370 6563 6966 6965 6420 706f 7369 7469  specified positi
+00000df0: 6f6e 0d0a 2020 2020 2d20 6070 756c 6c62  on..    - `pullb
+00000e00: 6163 6b60 3a20 7075 6c6c 6261 636b 206c  ack`: pullback l
+00000e10: 6971 7569 6420 6672 6f6d 2074 6970 0d0a  iquid from tip..
+00000e20: 2020 2020 2d20 6072 6573 6574 603a 2072      - `reset`: r
+00000e30: 6573 6574 2074 6865 2070 6970 6574 7465  eset the pipette
+00000e40: 0d0a 2020 2020 2d20 6073 6574 5370 6565  ..    - `setSpee
+00000e50: 6460 3a20 7365 7420 7468 6520 7370 6565  d`: set the spee
+00000e60: 6420 6f66 2074 6865 2070 6c75 6e67 6572  d of the plunger
+00000e70: 0d0a 2020 2020 2d20 6073 6875 7464 6f77  ..    - `shutdow
+00000e80: 6e60 3a20 7368 7574 646f 776e 2070 726f  n`: shutdown pro
+00000e90: 6365 6475 7265 2066 6f72 2074 6f6f 6c0d  cedure for tool.
+00000ea0: 0a20 2020 202d 2060 746f 6767 6c65 4665  .    - `toggleFe
+00000eb0: 6564 6261 636b 4c6f 6f70 603a 2073 7461  edbackLoop`: sta
+00000ec0: 7274 206f 7220 7374 6f70 2066 6565 6462  rt or stop feedb
+00000ed0: 6163 6b20 6c6f 6f70 0d0a 2020 2020 2d20  ack loop..    - 
+00000ee0: 607a 6572 6f60 3a20 7a65 726f 2074 6865  `zero`: zero the
+00000ef0: 2070 6c75 6e67 6572 2070 6f73 6974 696f   plunger positio
+00000f00: 6e0d 0a20 2020 2022 2222 0d0a 2020 2020  n..    """..    
+00000f10: 0d0a 2020 2020 5f64 6566 6175 6c74 5f66  ..    _default_f
+00000f20: 6c61 6773 203d 207b 0d0a 2020 2020 2020  lags = {..      
+00000f30: 2020 2762 7573 7927 3a20 4661 6c73 652c    'busy': False,
+00000f40: 0d0a 2020 2020 2020 2020 2763 6f6e 6475  ..        'condu
+00000f50: 6374 6976 655f 7469 7073 273a 2046 616c  ctive_tips': Fal
+00000f60: 7365 2c0d 0a20 2020 2020 2020 2027 636f  se,..        'co
+00000f70: 6e6e 6563 7465 6427 3a20 4661 6c73 652c  nnected': False,
+00000f80: 0d0a 2020 2020 2020 2020 2767 6574 5f66  ..        'get_f
+00000f90: 6565 6462 6163 6b27 3a20 4661 6c73 652c  eedback': False,
+00000fa0: 0d0a 2020 2020 2020 2020 276f 6363 7570  ..        'occup
+00000fb0: 6965 6427 3a20 4661 6c73 652c 0d0a 2020  ied': False,..  
+00000fc0: 2020 2020 2020 2770 6175 7365 5f66 6565        'pause_fee
+00000fd0: 6462 6163 6b27 3a46 616c 7365 2c0d 0a20  dback':False,.. 
+00000fe0: 2020 2020 2020 2027 7469 705f 6f6e 273a         'tip_on':
+00000ff0: 2046 616c 7365 0d0a 2020 2020 7d0d 0a20   False..    }.. 
+00001000: 2020 2069 6d70 6c65 6d65 6e74 5f6f 6666     implement_off
+00001010: 7365 7420 3d20 2830 2c30 2c2d 3235 3029  set = (0,0,-250)
+00001020: 0d0a 2020 2020 6465 6620 5f5f 696e 6974  ..    def __init
+00001030: 5f5f 2873 656c 662c 200d 0a20 2020 2020  __(self, ..     
+00001040: 2020 2070 6f72 743a 7374 722c 200d 0a20     port:str, .. 
+00001050: 2020 2020 2020 2063 6861 6e6e 656c 3a20         channel: 
+00001060: 696e 7420 3d20 312c 200d 0a20 2020 2020  int = 1, ..     
+00001070: 2020 206f 6666 7365 743a 2074 7570 6c65     offset: tuple
+00001080: 5b66 6c6f 6174 5d20 3d20 2830 2c30 2c30  [float] = (0,0,0
+00001090: 292c 0d0a 2020 2020 2020 2020 7265 7370  ),..        resp
+000010a0: 6f6e 7365 5f74 696d 653a 2066 6c6f 6174  onse_time: float
+000010b0: 203d 2031 2e30 332c 0d0a 2020 2020 2020   = 1.03,..      
+000010c0: 2020 7469 705f 696e 7365 745f 6d6d 3a20    tip_inset_mm: 
+000010d0: 696e 7420 3d20 3132 2c0d 0a20 2020 2020  int = 12,..     
+000010e0: 2020 2074 6970 5f74 6872 6573 686f 6c64     tip_threshold
+000010f0: 3a20 696e 7420 3d20 3237 362c 0d0a 2020  : int = 276,..  
+00001100: 2020 2020 2020 2a2a 6b77 6172 6773 0d0a        **kwargs..
+00001110: 2020 2020 293a 0d0a 2020 2020 2020 2020      ):..        
+00001120: 2222 220d 0a20 2020 2020 2020 2049 6e73  """..        Ins
+00001130: 7461 6e74 6961 7465 2074 6865 2063 6c61  tantiate the cla
+00001140: 7373 0d0a 0d0a 2020 2020 2020 2020 4172  ss....        Ar
+00001150: 6773 3a0d 0a20 2020 2020 2020 2020 2020  gs:..           
+00001160: 2070 6f72 7420 2873 7472 293a 2043 4f4d   port (str): COM
+00001170: 2070 6f72 7420 6164 6472 6573 730d 0a20   port address.. 
+00001180: 2020 2020 2020 2020 2020 2063 6861 6e6e             chann
+00001190: 656c 2028 696e 742c 206f 7074 696f 6e61  el (int, optiona
+000011a0: 6c29 3a20 6368 616e 6e65 6c20 6964 2e20  l): channel id. 
+000011b0: 4465 6661 756c 7473 2074 6f20 312e 0d0a  Defaults to 1...
+000011c0: 2020 2020 2020 2020 2020 2020 6f66 6673              offs
+000011d0: 6574 2028 7475 706c 655b 666c 6f61 745d  et (tuple[float]
+000011e0: 2c20 6f70 7469 6f6e 616c 293a 2078 2c79  , optional): x,y
+000011f0: 2c7a 206f 6666 7365 7420 6f66 2074 6970  ,z offset of tip
+00001200: 2e20 4465 6661 756c 7473 2074 6f20 2830  . Defaults to (0
+00001210: 2c30 2c30 292e 0d0a 2020 2020 2020 2020  ,0,0)...        
+00001220: 2020 2020 7265 7370 6f6e 7365 5f74 696d      response_tim
+00001230: 6520 2866 6c6f 6174 2c20 6f70 7469 6f6e  e (float, option
+00001240: 616c 293a 2064 656c 6179 2062 6574 7765  al): delay betwe
+00001250: 656e 2073 656e 6469 6e67 2061 2063 6f6d  en sending a com
+00001260: 6d61 6e64 2061 6e64 2072 6563 6569 7669  mand and receivi
+00001270: 6e67 2061 2072 6573 706f 6e73 652c 2069  ng a response, i
+00001280: 6e20 7365 636f 6e64 732e 2044 6566 6175  n seconds. Defau
+00001290: 6c74 7320 746f 2031 2e30 332e 0d0a 2020  lts to 1.03...  
+000012a0: 2020 2020 2020 2020 2020 7469 705f 696e            tip_in
+000012b0: 7365 745f 6d6d 2028 666c 6f61 742c 206f  set_mm (float, o
+000012c0: 7074 696f 6e61 6c29 3a20 6c65 6e67 7468  ptional): length
+000012d0: 206f 6620 7069 7065 7474 6520 7468 6174   of pipette that
+000012e0: 2069 7320 696e 7365 7274 6564 2069 6e74   is inserted int
+000012f0: 6f20 7468 6520 7069 7065 7474 6520 7469  o the pipette ti
+00001300: 702e 2044 6566 6175 6c74 7320 746f 2031  p. Defaults to 1
+00001310: 322e 0d0a 2020 2020 2020 2020 2020 2020  2...            
+00001320: 7469 705f 7468 7265 7368 6f6c 6420 2869  tip_threshold (i
+00001330: 6e74 2c20 6f70 7469 6f6e 616c 293a 2074  nt, optional): t
+00001340: 6872 6573 686f 6c64 2061 626f 7665 2077  hreshold above w
+00001350: 6869 6368 2061 2063 6f6e 6475 6374 6976  hich a conductiv
+00001360: 6520 7069 7065 7474 6520 7469 7020 6973  e pipette tip is
+00001370: 2063 6f6e 7369 6465 7265 6420 746f 2062   considered to b
+00001380: 6520 6174 7461 6368 6564 2e20 4465 6661  e attached. Defa
+00001390: 756c 7473 2074 6f20 3237 362e 0d0a 2020  ults to 276...  
+000013a0: 2020 2020 2020 2222 220d 0a20 2020 2020        """..     
+000013b0: 2020 2073 7570 6572 2829 2e5f 5f69 6e69     super().__ini
+000013c0: 745f 5f28 2a2a 6b77 6172 6773 290d 0a20  t__(**kwargs).. 
+000013d0: 2020 2020 2020 2073 656c 662e 6368 616e         self.chan
+000013e0: 6e65 6c20 3d20 6368 616e 6e65 6c0d 0a20  nel = channel.. 
+000013f0: 2020 2020 2020 2073 656c 662e 6f66 6673         self.offs
+00001400: 6574 203d 206f 6666 7365 740d 0a20 2020  et = offset..   
+00001410: 2020 2020 2073 656c 662e 7265 7370 6f6e       self.respon
+00001420: 7365 5f74 696d 6520 3d20 7265 7370 6f6e  se_time = respon
+00001430: 7365 5f74 696d 650d 0a20 2020 2020 2020  se_time..       
+00001440: 2073 656c 662e 7469 705f 7468 7265 7368   self.tip_thresh
+00001450: 6f6c 6420 3d20 7469 705f 7468 7265 7368  old = tip_thresh
+00001460: 6f6c 640d 0a20 2020 2020 2020 2073 656c  old..        sel
+00001470: 662e 7469 705f 696e 7365 745f 6d6d 203d  f.tip_inset_mm =
+00001480: 2074 6970 5f69 6e73 6574 5f6d 6d0d 0a20   tip_inset_mm.. 
+00001490: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
+000014a0: 2073 656c 662e 6d6f 6465 6c5f 696e 666f   self.model_info
+000014b0: 3a20 6c69 622e 4d6f 6465 6c20 3d20 4e6f  : lib.Model = No
+000014c0: 6e65 0d0a 2020 2020 2020 2020 7365 6c66  ne..        self
+000014d0: 2e6c 696d 6974 7320 3d20 2830 2c30 290d  .limits = (0,0).
+000014e0: 0a20 2020 2020 2020 2073 656c 662e 706f  .        self.po
+000014f0: 7369 7469 6f6e 203d 2030 0d0a 2020 2020  sition = 0..    
+00001500: 2020 2020 7365 6c66 2e73 7065 6564 5f63      self.speed_c
+00001510: 6f64 6520 3d20 5370 6565 6428 332c 3329  ode = Speed(3,3)
+00001520: 0d0a 2020 2020 2020 2020 7365 6c66 2e73  ..        self.s
+00001530: 7065 6564 5f70 7265 7365 7473 203d 204e  peed_presets = N
+00001540: 6f6e 650d 0a20 2020 2020 2020 2073 656c  one..        sel
+00001550: 662e 7469 705f 6c65 6e67 7468 203d 2030  f.tip_length = 0
+00001560: 0d0a 2020 2020 2020 2020 0d0a 2020 2020  ..        ..    
+00001570: 2020 2020 7365 6c66 2e5f 6361 7061 6369      self._capaci
+00001580: 7461 6e63 6520 3d20 300d 0a20 2020 2020  tance = 0..     
+00001590: 2020 2073 656c 662e 5f73 7461 7475 735f     self._status_
+000015a0: 636f 6465 203d 2027 270d 0a20 2020 2020  code = ''..     
+000015b0: 2020 2073 656c 662e 5f74 6872 6561 6473     self._threads
+000015c0: 203d 207b 7d0d 0a20 2020 2020 2020 200d   = {}..        .
+000015d0: 0a20 2020 2020 2020 2070 7269 6e74 2822  .        print("
+000015e0: 416e 7920 6174 7461 6368 6564 2070 6970  Any attached pip
+000015f0: 6574 7465 2074 6970 206d 6179 2064 726f  ette tip may dro
+00001600: 7020 6475 7269 6e67 2069 6e69 7469 616c  p during initial
+00001610: 6973 6174 696f 6e2e 2229 0d0a 2020 2020  isation.")..    
+00001620: 2020 2020 7365 6c66 2e5f 636f 6e6e 6563      self._connec
+00001630: 7428 706f 7274 290d 0a20 2020 2020 2020  t(port)..       
+00001640: 2072 6574 7572 6e0d 0a20 2020 200d 0a20   return..    .. 
+00001650: 2020 2023 2050 726f 7065 7274 6965 730d     # Properties.
+00001660: 0a20 2020 2040 7072 6f70 6572 7479 0d0a  .    @property..
+00001670: 2020 2020 6465 6620 6361 7061 6369 7461      def capacita
+00001680: 6e63 6528 7365 6c66 2920 2d3e 2069 6e74  nce(self) -> int
+00001690: 3a0d 0a20 2020 2020 2020 2072 6574 7572  :..        retur
+000016a0: 6e20 7365 6c66 2e5f 6361 7061 6369 7461  n self._capacita
+000016b0: 6e63 650d 0a20 2020 2020 2020 200d 0a20  nce..        .. 
+000016c0: 2020 2040 7072 6f70 6572 7479 0d0a 2020     @property..  
+000016d0: 2020 6465 6620 686f 6d65 5f70 6f73 6974    def home_posit
+000016e0: 696f 6e28 7365 6c66 2920 2d3e 2069 6e74  ion(self) -> int
+000016f0: 3a0d 0a20 2020 2020 2020 2072 6574 7572  :..        retur
+00001700: 6e20 7365 6c66 2e6d 6f64 656c 5f69 6e66  n self.model_inf
+00001710: 6f2e 686f 6d65 5f70 6f73 6974 696f 6e0d  o.home_position.
+00001720: 0a20 2020 200d 0a20 2020 2040 7072 6f70  .    ..    @prop
+00001730: 6572 7479 0d0a 2020 2020 6465 6620 706f  erty..    def po
+00001740: 7274 2873 656c 6629 202d 3e20 7374 723a  rt(self) -> str:
+00001750: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
+00001760: 2073 656c 662e 636f 6e6e 6563 7469 6f6e   self.connection
+00001770: 5f64 6574 6169 6c73 2e67 6574 2827 706f  _details.get('po
+00001780: 7274 272c 2027 2729 0d0a 2020 2020 0d0a  rt', '')..    ..
+00001790: 2020 2020 4070 726f 7065 7274 790d 0a20      @property.. 
+000017a0: 2020 2064 6566 2072 6573 6f6c 7574 696f     def resolutio
+000017b0: 6e28 7365 6c66 2920 2d3e 2066 6c6f 6174  n(self) -> float
+000017c0: 3a0d 0a20 2020 2020 2020 2072 6574 7572  :..        retur
+000017d0: 6e20 7365 6c66 2e6d 6f64 656c 5f69 6e66  n self.model_inf
+000017e0: 6f2e 7265 736f 6c75 7469 6f6e 0d0a 2020  o.resolution..  
+000017f0: 2020 0d0a 2020 2020 4070 726f 7065 7274    ..    @propert
+00001800: 790d 0a20 2020 2064 6566 2073 7461 7475  y..    def statu
+00001810: 7328 7365 6c66 2920 2d3e 2073 7472 3a0d  s(self) -> str:.
+00001820: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00001830: 7365 6c66 2e67 6574 5374 6174 7573 2829  self.getStatus()
+00001840: 0d0a 2020 2020 0d0a 2020 2020 6465 6620  ..    ..    def 
+00001850: 5f5f 6379 636c 6573 5f5f 2873 656c 6629  __cycles__(self)
+00001860: 202d 3e20 556e 696f 6e5b 696e 742c 2073   -> Union[int, s
+00001870: 7472 5d3a 0d0a 2020 2020 2020 2020 2222  tr]:..        ""
+00001880: 220d 0a20 2020 2020 2020 2052 6574 7269  "..        Retri
+00001890: 6576 6520 746f 7461 6c20 6379 636c 6520  eve total cycle 
+000018a0: 6c69 6665 7469 6d65 0d0a 0d0a 2020 2020  lifetime....    
+000018b0: 2020 2020 5265 7475 726e 733a 0d0a 2020      Returns:..  
+000018c0: 2020 2020 2020 2020 2020 556e 696f 6e5b            Union[
+000018d0: 696e 742c 2073 7472 5d3a 206e 756d 6265  int, str]: numbe
+000018e0: 7220 6f66 206c 6966 6574 696d 6520 6379  r of lifetime cy
+000018f0: 636c 6573 2c20 6f72 2072 6573 706f 6e73  cles, or respons
+00001900: 6520 7374 7269 6e67 0d0a 2020 2020 2020  e string..      
+00001910: 2020 2222 220d 0a20 2020 2020 2020 2072    """..        r
+00001920: 6573 706f 6e73 6520 3d20 7365 6c66 2e5f  esponse = self._
+00001930: 7175 6572 7928 2744 5827 290d 0a20 2020  query('DX')..   
+00001940: 2020 2020 2074 7279 3a0d 0a20 2020 2020       try:..     
+00001950: 2020 2020 2020 2063 7963 6c65 7320 3d20         cycles = 
+00001960: 696e 7428 7265 7370 6f6e 7365 290d 0a20  int(response).. 
+00001970: 2020 2020 2020 2065 7863 6570 7420 5661         except Va
+00001980: 6c75 6545 7272 6f72 3a0d 0a20 2020 2020  lueError:..     
+00001990: 2020 2020 2020 2072 6574 7572 6e20 7265         return re
+000019a0: 7370 6f6e 7365 0d0a 2020 2020 2020 2020  sponse..        
+000019b0: 7072 696e 7428 6627 546f 7461 6c20 6379  print(f'Total cy
+000019c0: 636c 6573 3a20 7b63 7963 6c65 737d 2729  cles: {cycles}')
+000019d0: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
+000019e0: 2063 7963 6c65 730d 0a20 2020 200d 0a20   cycles..    .. 
+000019f0: 2020 2064 6566 205f 5f6d 6f64 656c 5f5f     def __model__
+00001a00: 2873 656c 6629 202d 3e20 7374 723a 0d0a  (self) -> str:..
+00001a10: 2020 2020 2020 2020 2222 220d 0a20 2020          """..   
+00001a20: 2020 2020 2052 6574 7269 6576 6520 7468       Retrieve th
+00001a30: 6520 6d6f 6465 6c20 6f66 2074 6865 2064  e model of the d
+00001a40: 6576 6963 650d 0a0d 0a20 2020 2020 2020  evice....       
+00001a50: 2052 6574 7572 6e73 3a0d 0a20 2020 2020   Returns:..     
+00001a60: 2020 2020 2020 2073 7472 3a20 6d6f 6465         str: mode
+00001a70: 6c20 6e61 6d65 0d0a 2020 2020 2020 2020  l name..        
+00001a80: 2222 220d 0a20 2020 2020 2020 2072 6573  """..        res
+00001a90: 706f 6e73 6520 3d20 7365 6c66 2e5f 7175  ponse = self._qu
+00001aa0: 6572 7928 2744 4d27 290d 0a20 2020 2020  ery('DM')..     
+00001ab0: 2020 2070 7269 6e74 2866 274d 6f64 656c     print(f'Model
+00001ac0: 3a20 7b72 6573 706f 6e73 657d 2729 0d0a  : {response}')..
+00001ad0: 2020 2020 2020 2020 7265 7475 726e 2072          return r
+00001ae0: 6573 706f 6e73 650d 0a20 2020 200d 0a20  esponse..    .. 
+00001af0: 2020 2064 6566 205f 5f72 6573 6f6c 7574     def __resolut
+00001b00: 696f 6e5f 5f28 7365 6c66 2920 2d3e 2055  ion__(self) -> U
+00001b10: 6e69 6f6e 5b69 6e74 2c20 7374 725d 3a0d  nion[int, str]:.
+00001b20: 0a20 2020 2020 2020 2022 2222 0d0a 2020  .        """..  
+00001b30: 2020 2020 2020 5265 7472 6965 7665 2074        Retrieve t
+00001b40: 6865 2072 6573 6f6c 7574 696f 6e20 6f66  he resolution of
+00001b50: 2074 6865 2064 6576 6963 650d 0a0d 0a20   the device.... 
+00001b60: 2020 2020 2020 2052 6574 7572 6e73 3a0d         Returns:.
+00001b70: 0a20 2020 2020 2020 2020 2020 2055 6e69  .            Uni
+00001b80: 6f6e 5b69 6e74 2c20 7374 725d 3a20 766f  on[int, str]: vo
+00001b90: 6c75 6d65 2072 6573 6f6c 7574 696f 6e20  lume resolution 
+00001ba0: 6f66 2064 6576 6963 6520 696e 206e 4c2c  of device in nL,
+00001bb0: 206f 7220 7265 7370 6f6e 7365 2073 7472   or response str
+00001bc0: 696e 670d 0a20 2020 2020 2020 2022 2222  ing..        """
+00001bd0: 0d0a 2020 2020 2020 2020 7265 7370 6f6e  ..        respon
+00001be0: 7365 203d 2073 656c 662e 5f71 7565 7279  se = self._query
+00001bf0: 2827 4452 2729 0d0a 2020 2020 2020 2020  ('DR')..        
+00001c00: 7472 793a 0d0a 2020 2020 2020 2020 2020  try:..          
+00001c10: 2020 7265 736f 6c75 7469 6f6e 203d 2069    resolution = i
+00001c20: 6e74 2872 6573 706f 6e73 6529 0d0a 2020  nt(response)..  
+00001c30: 2020 2020 2020 6578 6365 7074 2056 616c        except Val
+00001c40: 7565 4572 726f 723a 0d0a 2020 2020 2020  ueError:..      
+00001c50: 2020 2020 2020 7265 7475 726e 2072 6573        return res
+00001c60: 706f 6e73 650d 0a20 2020 2020 2020 2070  ponse..        p
+00001c70: 7269 6e74 2866 277b 7265 736f 6c75 7469  rint(f'{resoluti
+00001c80: 6f6e 2f31 3030 307d 2075 4c20 2f20 7374  on/1000} uL / st
+00001c90: 6570 2729 0d0a 2020 2020 2020 2020 7265  ep')..        re
+00001ca0: 7475 726e 2072 6573 6f6c 7574 696f 6e0d  turn resolution.
+00001cb0: 0a20 2020 200d 0a20 2020 2064 6566 205f  .    ..    def _
+00001cc0: 5f76 6572 7369 6f6e 5f5f 2873 656c 6629  _version__(self)
+00001cd0: 202d 3e20 7374 723a 0d0a 2020 2020 2020   -> str:..      
+00001ce0: 2020 2222 220d 0a20 2020 2020 2020 2052    """..        R
+00001cf0: 6574 7269 6576 6520 7468 6520 736f 6674  etrieve the soft
+00001d00: 7761 7265 2076 6572 7369 6f6e 206f 6e20  ware version on 
+00001d10: 7468 6520 6465 7669 6365 0d0a 0d0a 2020  the device....  
+00001d20: 2020 2020 2020 5265 7475 726e 733a 0d0a        Returns:..
+00001d30: 2020 2020 2020 2020 2020 2020 7374 723a              str:
+00001d40: 2064 6576 6963 6520 7665 7273 696f 6e0d   device version.
+00001d50: 0a20 2020 2020 2020 2022 2222 0d0a 2020  .        """..  
+00001d60: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
+00001d70: 662e 5f71 7565 7279 2827 4456 2729 0d0a  f._query('DV')..
+00001d80: 0d0a 2020 2020 6465 6620 6164 6441 6972  ..    def addAir
+00001d90: 4761 7028 7365 6c66 2c20 7374 6570 733a  Gap(self, steps:
+00001da0: 696e 7420 3d20 3130 2920 2d3e 2073 7472  int = 10) -> str
+00001db0: 3a0d 0a20 2020 2020 2020 2022 2222 0d0a  :..        """..
+00001dc0: 2020 2020 2020 2020 4372 6561 7465 2061          Create a
+00001dd0: 6e20 6169 7220 6761 7020 6265 7477 6565  n air gap betwee
+00001de0: 6e20 7477 6f20 766f 6c75 6d65 7320 6f66  n two volumes of
+00001df0: 206c 6971 7569 6420 696e 2070 6970 6574   liquid in pipet
+00001e00: 7465 0d0a 2020 2020 2020 2020 0d0a 2020  te..        ..  
+00001e10: 2020 2020 2020 4172 6773 3a0d 0a20 2020        Args:..   
+00001e20: 2020 2020 2020 2020 2073 7465 7073 2028           steps (
+00001e30: 696e 742c 206f 7074 696f 6e61 6c29 3a20  int, optional): 
+00001e40: 6e75 6d62 6572 206f 6620 7374 6570 7320  number of steps 
+00001e50: 666f 7220 6169 7220 6761 702e 2044 6566  for air gap. Def
+00001e60: 6175 6c74 7320 746f 2044 4546 4155 4c54  aults to DEFAULT
+00001e70: 5f41 4952 4741 502e 0d0a 2020 2020 2020  _AIRGAP...      
+00001e80: 2020 2020 2020 6368 616e 6e65 6c20 2869        channel (i
+00001e90: 6e74 2c20 6f70 7469 6f6e 616c 293a 2063  nt, optional): c
+00001ea0: 6861 6e6e 656c 2074 6f20 6164 6420 6169  hannel to add ai
+00001eb0: 7220 6761 702e 2044 6566 6175 6c74 7320  r gap. Defaults 
+00001ec0: 746f 204e 6f6e 652e 0d0a 0d0a 2020 2020  to None.....    
+00001ed0: 2020 2020 5265 7475 726e 733a 0d0a 2020      Returns:..  
+00001ee0: 2020 2020 2020 2020 2020 7374 723a 2064            str: d
+00001ef0: 6576 6963 6520 7265 7370 6f6e 7365 0d0a  evice response..
+00001f00: 2020 2020 2020 2020 2222 220d 0a20 2020          """..   
+00001f10: 2020 2020 2072 6573 706f 6e73 6520 3d20       response = 
+00001f20: 7365 6c66 2e5f 7175 6572 7928 6627 5249  self._query(f'RI
+00001f30: 7b73 7465 7073 7d27 290d 0a20 2020 2020  {steps}')..     
+00001f40: 2020 2074 696d 652e 736c 6565 7028 3129     time.sleep(1)
+00001f50: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
+00001f60: 2072 6573 706f 6e73 650d 0a20 2020 2020   response..     
+00001f70: 2020 200d 0a20 2020 2064 6566 2061 7370     ..    def asp
+00001f80: 6972 6174 6528 7365 6c66 2c20 0d0a 2020  irate(self, ..  
+00001f90: 2020 2020 2020 766f 6c75 6d65 3a20 666c        volume: fl
+00001fa0: 6f61 742c 200d 0a20 2020 2020 2020 2073  oat, ..        s
+00001fb0: 7065 6564 3a20 4f70 7469 6f6e 616c 5b66  peed: Optional[f
+00001fc0: 6c6f 6174 5d20 3d20 4e6f 6e65 2c20 0d0a  loat] = None, ..
+00001fd0: 2020 2020 2020 2020 7761 6974 3a20 696e          wait: in
+00001fe0: 7420 3d20 302c 200d 0a20 2020 2020 2020  t = 0, ..       
+00001ff0: 2070 6175 7365 3a20 626f 6f6c 203d 2046   pause: bool = F
+00002000: 616c 7365 2c20 0d0a 2020 2020 2020 2020  alse, ..        
+00002010: 7265 6167 656e 743a 204f 7074 696f 6e61  reagent: Optiona
+00002020: 6c5b 7374 725d 203d 204e 6f6e 652c 0d0a  l[str] = None,..
+00002030: 2020 2020 2020 2020 2a2a 6b77 6172 6773          **kwargs
+00002040: 0d0a 2020 2020 2920 2d3e 2073 7472 3a0d  ..    ) -> str:.
+00002050: 0a20 2020 2020 2020 2022 2222 0d0a 2020  .        """..  
+00002060: 2020 2020 2020 4173 7069 7261 7465 2064        Aspirate d
+00002070: 6573 6972 6564 2076 6f6c 756d 6520 6f66  esired volume of
+00002080: 2072 6561 6765 6e74 0d0a 0d0a 2020 2020   reagent....    
+00002090: 2020 2020 4172 6773 3a0d 0a20 2020 2020      Args:..     
+000020a0: 2020 2020 2020 2076 6f6c 756d 6520 2866         volume (f
+000020b0: 6c6f 6174 293a 2074 6172 6765 7420 766f  loat): target vo
+000020c0: 6c75 6d65 0d0a 2020 2020 2020 2020 2020  lume..          
+000020d0: 2020 7370 6565 6420 284f 7074 696f 6e61    speed (Optiona
+000020e0: 6c5b 666c 6f61 745d 2c20 6f70 7469 6f6e  l[float], option
+000020f0: 616c 293a 2073 7065 6564 2074 6f20 6173  al): speed to as
+00002100: 7069 7261 7465 2061 742e 2044 6566 6175  pirate at. Defau
+00002110: 6c74 7320 746f 204e 6f6e 652e 0d0a 2020  lts to None...  
+00002120: 2020 2020 2020 2020 2020 7761 6974 2028            wait (
+00002130: 696e 742c 206f 7074 696f 6e61 6c29 3a20  int, optional): 
+00002140: 7469 6d65 2064 656c 6179 2061 6674 6572  time delay after
+00002150: 2061 7370 6972 6174 652e 2044 6566 6175   aspirate. Defau
+00002160: 6c74 7320 746f 2030 2e0d 0a20 2020 2020  lts to 0...     
+00002170: 2020 2020 2020 2070 6175 7365 2028 626f         pause (bo
+00002180: 6f6c 2c20 6f70 7469 6f6e 616c 293a 2077  ol, optional): w
+00002190: 6865 7468 6572 2074 6f20 7061 7573 6520  hether to pause 
+000021a0: 666f 7220 7573 6572 2069 6e74 6572 7665  for user interve
+000021b0: 6e74 696f 6e2e 2044 6566 6175 6c74 7320  ntion. Defaults 
+000021c0: 746f 2046 616c 7365 2e0d 0a20 2020 2020  to False...     
+000021d0: 2020 2020 2020 2072 6561 6765 6e74 2028         reagent (
+000021e0: 4f70 7469 6f6e 616c 5b73 7472 5d2c 206f  Optional[str], o
+000021f0: 7074 696f 6e61 6c29 3a20 6e61 6d65 206f  ptional): name o
+00002200: 6620 7265 6167 656e 742e 2044 6566 6175  f reagent. Defau
+00002210: 6c74 7320 746f 204e 6f6e 652e 0d0a 2020  lts to None...  
+00002220: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
+00002230: 2020 2020 5265 7475 726e 733a 0d0a 2020      Returns:..  
+00002240: 2020 2020 2020 2020 2020 7374 723a 2064            str: d
+00002250: 6576 6963 6520 7265 7370 6f6e 7365 0d0a  evice response..
+00002260: 2020 2020 2020 2020 2222 2220 0d0a 2020          """ ..  
+00002270: 2020 2020 2020 7365 6c66 2e73 6574 466c        self.setFl
+00002280: 6167 2870 6175 7365 5f66 6565 6462 6163  ag(pause_feedbac
+00002290: 6b3d 5472 7565 2c20 6f63 6375 7069 6564  k=True, occupied
+000022a0: 3d54 7275 6529 0d0a 2020 2020 2020 2020  =True)..        
+000022b0: 766f 6c75 6d65 203d 206d 696e 2876 6f6c  volume = min(vol
+000022c0: 756d 652c 2073 656c 662e 6361 7061 6369  ume, self.capaci
+000022d0: 7479 202d 2073 656c 662e 766f 6c75 6d65  ty - self.volume
+000022e0: 290d 0a20 2020 2020 2020 2073 7465 7073  )..        steps
+000022f0: 203d 2069 6e74 2876 6f6c 756d 6520 2f20   = int(volume / 
+00002300: 7365 6c66 2e72 6573 6f6c 7574 696f 6e29  self.resolution)
+00002310: 0d0a 2020 2020 2020 2020 766f 6c75 6d65  ..        volume
+00002320: 203d 2073 7465 7073 202a 2073 656c 662e   = steps * self.
+00002330: 7265 736f 6c75 7469 6f6e 0d0a 2020 2020  resolution..    
+00002340: 2020 2020 6966 2076 6f6c 756d 6520 3d3d      if volume ==
+00002350: 2030 3a0d 0a20 2020 2020 2020 2020 2020   0:..           
+00002360: 2072 6574 7572 6e20 2727 0d0a 2020 2020   return ''..    
+00002370: 2020 2020 7072 696e 7428 6627 4173 7069      print(f'Aspi
+00002380: 7261 7469 6e67 207b 766f 6c75 6d65 7d20  rating {volume} 
+00002390: 754c 2e2e 2e27 290d 0a20 2020 2020 2020  uL...')..       
+000023a0: 2073 7461 7274 5f61 7370 6972 6174 6520   start_aspirate 
+000023b0: 3d20 7469 6d65 2e70 6572 665f 636f 756e  = time.perf_coun
+000023c0: 7465 7228 290d 0a20 2020 2020 2020 2073  ter()..        s
+000023d0: 7065 6564 203d 2073 656c 662e 7370 6565  peed = self.spee
+000023e0: 642e 7570 2069 6620 7370 6565 6420 6973  d.up if speed is
+000023f0: 204e 6f6e 6520 656c 7365 2073 7065 6564   None else speed
+00002400: 0d0a 2020 2020 2020 2020 0d0a 2020 2020  ..        ..    
+00002410: 2020 2020 6966 2073 7065 6564 2069 6e20      if speed in 
+00002420: 7365 6c66 2e73 7065 6564 5f70 7265 7365  self.speed_prese
+00002430: 7473 3a0d 0a20 2020 2020 2020 2020 2020  ts:..           
+00002440: 2069 6620 7370 6565 6420 213d 2073 656c   if speed != sel
+00002450: 662e 7370 6565 642e 7570 3a0d 0a20 2020  f.speed.up:..   
+00002460: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00002470: 662e 7365 7453 7065 6564 2873 7065 6564  f.setSpeed(speed
+00002480: 3d73 7065 6564 2c20 7570 3d54 7275 652c  =speed, up=True,
+00002490: 2064 6566 6175 6c74 3d46 616c 7365 290d   default=False).
+000024a0: 0a20 2020 2020 2020 2020 2020 2073 7461  .            sta
+000024b0: 7274 5f61 7370 6972 6174 6520 3d20 7469  rt_aspirate = ti
+000024c0: 6d65 2e70 6572 665f 636f 756e 7465 7228  me.perf_counter(
+000024d0: 290d 0a20 2020 2020 2020 2020 2020 2072  )..            r
+000024e0: 6573 706f 6e73 6520 3d20 7365 6c66 2e5f  esponse = self._
+000024f0: 7175 6572 7928 6627 5249 7b73 7465 7073  query(f'RI{steps
+00002500: 7d27 290d 0a20 2020 2020 2020 2020 2020  }')..           
+00002510: 206d 6f76 655f 7469 6d65 203d 2073 7465   move_time = ste
+00002520: 7073 2a73 656c 662e 7265 736f 6c75 7469  ps*self.resoluti
+00002530: 6f6e 202f 2073 7065 6564 0d0a 2020 2020  on / speed..    
+00002540: 2020 2020 2020 2020 6475 7261 7469 6f6e          duration
+00002550: 203d 2074 696d 652e 7065 7266 5f63 6f75   = time.perf_cou
+00002560: 6e74 6572 2829 202d 2073 7461 7274 5f61  nter() - start_a
+00002570: 7370 6972 6174 650d 0a20 2020 2020 2020  spirate..       
+00002580: 2020 2020 2069 6620 6475 7261 7469 6f6e       if duration
+00002590: 203c 2028 6d6f 7665 5f74 696d 6529 3a0d   < (move_time):.
+000025a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000025b0: 2074 696d 652e 736c 6565 7028 6d6f 7665   time.sleep(move
+000025c0: 5f74 696d 652d 6475 7261 7469 6f6e 290d  _time-duration).
+000025d0: 0a20 2020 2020 2020 2020 2020 2023 2069  .            # i
+000025e0: 6620 7265 7370 6f6e 7365 2021 3d20 276f  f response != 'o
+000025f0: 6b27 3a0d 0a20 2020 2020 2020 2020 2020  k':..           
+00002600: 2023 2020 2020 2072 6574 7572 6e20 7265   #     return re
+00002610: 7370 6f6e 7365 0d0a 2020 2020 2020 2020  sponse..        
+00002620: 2020 2020 0d0a 2020 2020 2020 2020 656c      ..        el
+00002630: 6966 2073 7065 6564 206e 6f74 2069 6e20  if speed not in 
+00002640: 7365 6c66 2e73 7065 6564 5f70 7265 7365  self.speed_prese
+00002650: 7473 3a0d 0a20 2020 2020 2020 2020 2020  ts:..           
+00002660: 2070 7269 6e74 2866 2254 6172 6765 743a   print(f"Target:
+00002670: 207b 766f 6c75 6d65 7d20 754c 2061 7420   {volume} uL at 
+00002680: 7b73 7065 6564 7d20 754c 2f73 2e2e 2e22  {speed} uL/s..."
+00002690: 290d 0a20 2020 2020 2020 2020 2020 2073  )..            s
+000026a0: 7065 6564 5f70 6172 616d 6574 6572 7320  peed_parameters 
+000026b0: 3d20 7365 6c66 2e5f 6361 6c63 756c 6174  = self._calculat
+000026c0: 655f 7370 6565 645f 7061 7261 6d65 7465  e_speed_paramete
+000026d0: 7273 2876 6f6c 756d 653d 766f 6c75 6d65  rs(volume=volume
+000026e0: 2c20 7370 6565 643d 7370 6565 6429 0d0a  , speed=speed)..
+000026f0: 2020 2020 2020 2020 2020 2020 7072 696e              prin
+00002700: 7428 7370 6565 645f 7061 7261 6d65 7465  t(speed_paramete
+00002710: 7273 290d 0a20 2020 2020 2020 2020 2020  rs)..           
+00002720: 2070 7265 7365 7420 3d20 7370 6565 645f   preset = speed_
+00002730: 7061 7261 6d65 7465 7273 2e70 7265 7365  parameters.prese
+00002740: 740d 0a20 2020 2020 2020 2020 2020 2069  t..            i
+00002750: 6620 7072 6573 6574 2069 7320 4e6f 6e65  f preset is None
+00002760: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00002770: 2020 2023 2072 6169 7365 2052 756e 7469     # raise Runti
+00002780: 6d65 4572 726f 7228 2754 6172 6765 7420  meError('Target 
+00002790: 7370 6565 6420 6e6f 7420 706f 7373 6962  speed not possib
+000027a0: 6c65 2e27 290d 0a20 2020 2020 2020 2020  le.')..         
+000027b0: 2020 2020 2020 2070 7269 6e74 2827 5461         print('Ta
+000027c0: 7267 6574 2073 7065 6564 206e 6f74 2070  rget speed not p
+000027d0: 6f73 7369 626c 652e 2729 0d0a 2020 2020  ossible.')..    
+000027e0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+000027f0: 726e 0d0a 2020 2020 2020 2020 2020 2020  rn..            
+00002800: 7365 6c66 2e73 6574 5370 6565 6428 7370  self.setSpeed(sp
+00002810: 6565 643d 7072 6573 6574 2c20 7570 3d54  eed=preset, up=T
+00002820: 7275 652c 2064 6566 6175 6c74 3d46 616c  rue, default=Fal
+00002830: 7365 290d 0a20 2020 2020 2020 2020 2020  se)..           
+00002840: 200d 0a20 2020 2020 2020 2020 2020 2073   ..            s
+00002850: 7465 7073 5f6c 6566 7420 3d20 7374 6570  teps_left = step
+00002860: 730d 0a20 2020 2020 2020 2020 2020 2064  s..            d
+00002870: 656c 6179 203d 2073 7065 6564 5f70 6172  elay = speed_par
+00002880: 616d 6574 6572 732e 6465 6c61 790d 0a20  ameters.delay.. 
+00002890: 2020 2020 2020 2020 2020 2073 7465 705f             step_
+000028a0: 7369 7a65 203d 2073 7065 6564 5f70 6172  size = speed_par
+000028b0: 616d 6574 6572 732e 7374 6570 5f73 697a  ameters.step_siz
+000028c0: 650d 0a20 2020 2020 2020 2020 2020 2069  e..            i
+000028d0: 6e74 6572 7661 6c73 203d 2073 7065 6564  ntervals = speed
+000028e0: 5f70 6172 616d 6574 6572 732e 696e 7465  _parameters.inte
+000028f0: 7276 616c 730d 0a20 2020 2020 2020 2020  rvals..         
+00002900: 2020 2073 7461 7274 5f61 7370 6972 6174     start_aspirat
+00002910: 6520 3d20 7469 6d65 2e70 6572 665f 636f  e = time.perf_co
+00002920: 756e 7465 7228 290d 0a20 2020 2020 2020  unter()..       
+00002930: 2020 2020 2066 6f72 2069 2069 6e20 7261       for i in ra
+00002940: 6e67 6528 696e 7465 7276 616c 7329 3a0d  nge(intervals):.
+00002950: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002960: 2073 7461 7274 5f74 696d 6520 3d20 7469   start_time = ti
+00002970: 6d65 2e70 6572 665f 636f 756e 7465 7228  me.perf_counter(
+00002980: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00002990: 2020 2073 7465 7020 3d20 7374 6570 5f73     step = step_s
+000029a0: 697a 6520 6966 2028 692b 3120 213d 2069  ize if (i+1 != i
+000029b0: 6e74 6572 7661 6c73 2920 656c 7365 2073  ntervals) else s
+000029c0: 7465 7073 5f6c 6566 740d 0a20 2020 2020  teps_left..     
+000029d0: 2020 2020 2020 2020 2020 206d 6f76 655f             move_
+000029e0: 7469 6d65 203d 2073 7465 702a 7365 6c66  time = step*self
+000029f0: 2e72 6573 6f6c 7574 696f 6e20 2f20 7072  .resolution / pr
+00002a00: 6573 6574 0d0a 2020 2020 2020 2020 2020  eset..          
+00002a10: 2020 2020 2020 7265 7370 6f6e 7365 203d        response =
+00002a20: 2073 656c 662e 5f71 7565 7279 2866 2752   self._query(f'R
+00002a30: 497b 7374 6570 7d27 2c20 7265 7375 6d65  I{step}', resume
+00002a40: 5f66 6565 6462 6163 6b3d 4661 6c73 652c  _feedback=False,
+00002a50: 2067 6574 5f70 6f73 6974 696f 6e3d 4661   get_position=Fa
+00002a60: 6c73 6529 0d0a 2020 2020 2020 2020 2020  lse)..          
+00002a70: 2020 2020 2020 2320 6966 2072 6573 706f        # if respo
+00002a80: 6e73 6520 213d 2027 6f6b 273a 0d0a 2020  nse != 'ok':..  
+00002a90: 2020 2020 2020 2020 2020 2020 2020 2320                # 
+00002aa0: 2020 2020 7072 696e 7428 2241 7370 6972      print("Aspir
+00002ab0: 6174 696f 6e20 6661 696c 6564 2229 0d0a  ation failed")..
+00002ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002ad0: 2320 2020 2020 7265 7475 726e 2072 6573  #     return res
+00002ae0: 706f 6e73 650d 0a20 2020 2020 2020 2020  ponse..         
+00002af0: 2020 2020 2020 2073 7465 7073 5f6c 6566         steps_lef
+00002b00: 7420 2d3d 2073 7465 700d 0a20 2020 2020  t -= step..     
+00002b10: 2020 2020 2020 2020 2020 2064 7572 6174             durat
+00002b20: 696f 6e20 3d20 7469 6d65 2e70 6572 665f  ion = time.perf_
+00002b30: 636f 756e 7465 7228 2920 2d20 7374 6172  counter() - star
+00002b40: 745f 7469 6d65 0d0a 2020 2020 2020 2020  t_time..        
+00002b50: 2020 2020 2020 2020 6966 2064 7572 6174          if durat
+00002b60: 696f 6e20 3c20 2864 656c 6179 2b6d 6f76  ion < (delay+mov
+00002b70: 655f 7469 6d65 293a 0d0a 2020 2020 2020  e_time):..      
+00002b80: 2020 2020 2020 2020 2020 2020 2020 7469                ti
+00002b90: 6d65 2e73 6c65 6570 2864 656c 6179 2b6d  me.sleep(delay+m
+00002ba0: 6f76 655f 7469 6d65 2d64 7572 6174 696f  ove_time-duratio
+00002bb0: 6e29 0d0a 2020 2020 2020 2020 0d0a 2020  n)..        ..  
+00002bc0: 2020 2020 2020 2320 5570 6461 7465 2076        # Update v
+00002bd0: 616c 7565 730d 0a20 2020 2020 2020 2070  alues..        p
+00002be0: 7269 6e74 2866 2741 7370 6972 6174 696f  rint(f'Aspiratio
+00002bf0: 6e20 7469 6d65 3a20 7b74 696d 652e 7065  n time: {time.pe
+00002c00: 7266 5f63 6f75 6e74 6572 2829 2d73 7461  rf_counter()-sta
+00002c10: 7274 5f61 7370 6972 6174 657d 7327 290d  rt_aspirate}s').
+00002c20: 0a20 2020 2020 2020 2074 696d 652e 736c  .        time.sl
+00002c30: 6565 7028 7761 6974 290d 0a20 2020 2020  eep(wait)..     
+00002c40: 2020 2073 656c 662e 7365 7446 6c61 6728     self.setFlag(
+00002c50: 6f63 6375 7069 6564 3d46 616c 7365 2c20  occupied=False, 
+00002c60: 7061 7573 655f 6665 6564 6261 636b 3d46  pause_feedback=F
+00002c70: 616c 7365 290d 0a20 2020 2020 2020 2073  alse)..        s
+00002c80: 656c 662e 6765 7450 6f73 6974 696f 6e28  elf.getPosition(
+00002c90: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
+00002ca0: 766f 6c75 6d65 202b 3d20 766f 6c75 6d65  volume += volume
+00002cb0: 0d0a 2020 2020 2020 2020 7365 6c66 2e70  ..        self.p
+00002cc0: 6f73 6974 696f 6e20 2b3d 2073 7465 7073  osition += steps
+00002cd0: 0d0a 2020 2020 2020 2020 6966 2072 6561  ..        if rea
+00002ce0: 6765 6e74 2069 7320 6e6f 7420 4e6f 6e65  gent is not None
+00002cf0: 3a0d 0a20 2020 2020 2020 2020 2020 2073  :..            s
+00002d00: 656c 662e 7265 6167 656e 7420 3d20 7265  elf.reagent = re
+00002d10: 6167 656e 740d 0a20 2020 2020 2020 2069  agent..        i
+00002d20: 6620 7061 7573 653a 0d0a 2020 2020 2020  f pause:..      
+00002d30: 2020 2020 2020 696e 7075 7428 2250 7265        input("Pre
+00002d40: 7373 2027 456e 7465 7227 2074 6f20 7072  ss 'Enter' to pr
+00002d50: 6f63 6565 642e 2229 0d0a 2020 2020 2020  oceed.")..      
+00002d60: 2020 7265 7475 726e 2072 6573 706f 6e73    return respons
+00002d70: 650d 0a20 2020 200d 0a20 2020 2064 6566  e..    ..    def
+00002d80: 2062 6c6f 776f 7574 2873 656c 662c 2068   blowout(self, h
+00002d90: 6f6d 653a 626f 6f6c 203d 2054 7275 652c  ome:bool = True,
+00002da0: 202a 2a6b 7761 7267 7329 202d 3e20 7374   **kwargs) -> st
+00002db0: 723a 0d0a 2020 2020 2020 2020 2222 220d  r:..        """.
+00002dc0: 0a20 2020 2020 2020 2042 6c6f 776f 7574  .        Blowout
+00002dd0: 206c 6971 7569 6420 6672 6f6d 2074 6970   liquid from tip
+00002de0: 0d0a 0d0a 2020 2020 2020 2020 4172 6773  ....        Args
+00002df0: 3a0d 0a20 2020 2020 2020 2020 2020 2068  :..            h
+00002e00: 6f6d 6520 2862 6f6f 6c2c 206f 7074 696f  ome (bool, optio
+00002e10: 6e61 6c29 3a20 7768 6574 6865 7220 746f  nal): whether to
+00002e20: 2072 6574 7572 6e20 706c 756e 6765 7220   return plunger 
+00002e30: 746f 2068 6f6d 6520 706f 7369 7469 6f6e  to home position
+00002e40: 2e20 4465 6661 756c 7473 2074 6f20 5472  . Defaults to Tr
+00002e50: 7565 2e0d 0a0d 0a20 2020 2020 2020 2052  ue.....        R
+00002e60: 6574 7572 6e73 3a0d 0a20 2020 2020 2020  eturns:..       
+00002e70: 2020 2020 2073 7472 3a20 6465 7669 6365       str: device
+00002e80: 2072 6573 706f 6e73 650d 0a20 2020 2020   response..     
+00002e90: 2020 2022 2222 0d0a 2020 2020 2020 2020     """..        
+00002ea0: 636f 6d6d 616e 6420 3d20 6627 5242 7b73  command = f'RB{s
+00002eb0: 656c 662e 686f 6d65 5f70 6f73 6974 696f  elf.home_positio
+00002ec0: 6e7d 2720 6966 2068 6f6d 6520 656c 7365  n}' if home else
+00002ed0: 2027 5242 270d 0a20 2020 2020 2020 2072   'RB'..        r
+00002ee0: 6573 706f 6e73 6520 3d20 7365 6c66 2e5f  esponse = self._
+00002ef0: 7175 6572 7928 636f 6d6d 616e 6429 0d0a  query(command)..
+00002f00: 2020 2020 2020 2020 7365 6c66 2e70 6f73          self.pos
+00002f10: 6974 696f 6e20 3d20 7365 6c66 2e68 6f6d  ition = self.hom
+00002f20: 655f 706f 7369 7469 6f6e 0d0a 2020 2020  e_position..    
+00002f30: 2020 2020 7469 6d65 2e73 6c65 6570 2831      time.sleep(1
+00002f40: 290d 0a20 2020 2020 2020 2072 6574 7572  )..        retur
+00002f50: 6e20 7265 7370 6f6e 7365 0d0a 2020 2020  n response..    
+00002f60: 0d0a 2020 2020 6465 6620 6469 7370 656e  ..    def dispen
+00002f70: 7365 2873 656c 662c 200d 0a20 2020 2020  se(self, ..     
+00002f80: 2020 2076 6f6c 756d 653a 2066 6c6f 6174     volume: float
+00002f90: 2c20 0d0a 2020 2020 2020 2020 7370 6565  , ..        spee
+00002fa0: 643a 204f 7074 696f 6e61 6c5b 666c 6f61  d: Optional[floa
+00002fb0: 745d 203d 204e 6f6e 652c 200d 0a20 2020  t] = None, ..   
+00002fc0: 2020 2020 2077 6169 743a 2069 6e74 203d       wait: int =
+00002fd0: 2030 2c20 0d0a 2020 2020 2020 2020 7061   0, ..        pa
+00002fe0: 7573 653a 2062 6f6f 6c20 3d20 4661 6c73  use: bool = Fals
+00002ff0: 652c 200d 0a20 2020 2020 2020 2062 6c6f  e, ..        blo
+00003000: 776f 7574 3a20 626f 6f6c 203d 2046 616c  wout: bool = Fal
+00003010: 7365 2c0d 0a20 2020 2020 2020 2062 6c6f  se,..        blo
+00003020: 776f 7574 5f68 6f6d 653a 2062 6f6f 6c20  wout_home: bool 
+00003030: 3d20 5472 7565 2c0d 0a20 2020 2020 2020  = True,..       
+00003040: 2066 6f72 6365 5f64 6973 7065 6e73 653a   force_dispense:
+00003050: 2062 6f6f 6c20 3d20 4661 6c73 652c 200d   bool = False, .
+00003060: 0a20 2020 2020 2020 202a 2a6b 7761 7267  .        **kwarg
+00003070: 730d 0a20 2020 2029 202d 3e20 7374 723a  s..    ) -> str:
+00003080: 0d0a 2020 2020 2020 2020 2222 220d 0a20  ..        """.. 
+00003090: 2020 2020 2020 2044 6973 7065 6e73 6520         Dispense 
+000030a0: 6465 7369 7265 6420 766f 6c75 6d65 206f  desired volume o
+000030b0: 6620 7265 6167 656e 740d 0a0d 0a20 2020  f reagent....   
+000030c0: 2020 2020 2041 7267 733a 0d0a 2020 2020       Args:..    
+000030d0: 2020 2020 2020 2020 766f 6c75 6d65 2028          volume (
+000030e0: 666c 6f61 7429 3a20 7461 7267 6574 2076  float): target v
+000030f0: 6f6c 756d 650d 0a20 2020 2020 2020 2020  olume..         
+00003100: 2020 2073 7065 6564 2028 4f70 7469 6f6e     speed (Option
+00003110: 616c 5b66 6c6f 6174 5d2c 206f 7074 696f  al[float], optio
+00003120: 6e61 6c29 3a20 7370 6565 6420 746f 2064  nal): speed to d
+00003130: 6973 7065 6e73 6520 6174 2e20 4465 6661  ispense at. Defa
+00003140: 756c 7473 2074 6f20 4e6f 6e65 2e0d 0a20  ults to None... 
+00003150: 2020 2020 2020 2020 2020 2077 6169 7420             wait 
+00003160: 2869 6e74 2c20 6f70 7469 6f6e 616c 293a  (int, optional):
+00003170: 2074 696d 6520 6465 6c61 7920 6166 7465   time delay afte
+00003180: 7220 6469 7370 656e 7365 2e20 4465 6661  r dispense. Defa
+00003190: 756c 7473 2074 6f20 302e 0d0a 2020 2020  ults to 0...    
+000031a0: 2020 2020 2020 2020 7061 7573 6520 2862          pause (b
+000031b0: 6f6f 6c2c 206f 7074 696f 6e61 6c29 3a20  ool, optional): 
+000031c0: 7768 6574 6865 7220 746f 2070 6175 7365  whether to pause
+000031d0: 2066 6f72 2075 7365 7220 696e 7465 7276   for user interv
+000031e0: 656e 7469 6f6e 2e20 4465 6661 756c 7473  ention. Defaults
+000031f0: 2074 6f20 4661 6c73 652e 0d0a 2020 2020   to False...    
+00003200: 2020 2020 2020 2020 626c 6f77 6f75 7420          blowout 
+00003210: 2862 6f6f 6c2c 206f 7074 696f 6e61 6c29  (bool, optional)
+00003220: 3a20 7768 6574 6865 7220 7065 7266 6f72  : whether perfor
+00003230: 6d20 626c 6f77 6f75 742e 2044 6566 6175  m blowout. Defau
+00003240: 6c74 7320 746f 2046 616c 7365 2e0d 0a20  lts to False... 
+00003250: 2020 2020 2020 2020 2020 2062 6c6f 776f             blowo
+00003260: 7574 5f68 6f6d 6520 2862 6f6f 6c2c 206f  ut_home (bool, o
+00003270: 7074 696f 6e61 6c29 3a20 7768 6574 6865  ptional): whethe
+00003280: 7220 746f 2072 6574 7572 6e20 7468 6520  r to return the 
+00003290: 706c 756e 6765 7220 686f 6d65 2061 6674  plunger home aft
+000032a0: 6572 2062 6c6f 776f 7574 2e20 4465 6661  er blowout. Defa
+000032b0: 756c 7473 2074 6f20 5472 7565 2e0d 0a20  ults to True... 
+000032c0: 2020 2020 2020 2020 2020 2066 6f72 6365             force
+000032d0: 5f64 6973 7065 6e73 6520 2862 6f6f 6c2c  _dispense (bool,
+000032e0: 206f 7074 696f 6e61 6c29 3a20 7768 6574   optional): whet
+000032f0: 6865 7220 746f 2064 6973 7065 6e73 6520  her to dispense 
+00003300: 7265 6167 656e 7420 7265 6761 7264 6c65  reagent regardle
+00003310: 7373 2e20 4465 6661 756c 7473 2074 6f20  ss. Defaults to 
+00003320: 4661 6c73 652e 0d0a 0d0a 2020 2020 2020  False.....      
+00003330: 2020 5261 6973 6573 3a0d 0a20 2020 2020    Raises:..     
+00003340: 2020 2020 2020 2056 616c 7565 4572 726f         ValueErro
+00003350: 723a 2052 6571 7569 7265 6420 6469 7370  r: Required disp
+00003360: 656e 7365 2076 6f6c 756d 6520 6973 2067  ense volume is g
+00003370: 7265 6174 6572 2074 6861 6e20 766f 6c75  reater than volu
+00003380: 6d65 2069 6e20 7469 700d 0a0d 0a20 2020  me in tip....   
+00003390: 2020 2020 2052 6574 7572 6e73 3a0d 0a20       Returns:.. 
+000033a0: 2020 2020 2020 2020 2020 2073 7472 3a20             str: 
+000033b0: 6465 7669 6365 2072 6573 706f 6e73 650d  device response.
+000033c0: 0a20 2020 2020 2020 2022 2222 0d0a 2020  .        """..  
+000033d0: 2020 2020 2020 7365 6c66 2e73 6574 466c        self.setFl
+000033e0: 6167 2870 6175 7365 5f66 6565 6462 6163  ag(pause_feedbac
+000033f0: 6b3d 5472 7565 2c20 6f63 6375 7069 6564  k=True, occupied
+00003400: 3d54 7275 6529 0d0a 2020 2020 2020 2020  =True)..        
+00003410: 6966 2066 6f72 6365 5f64 6973 7065 6e73  if force_dispens
+00003420: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
+00003430: 766f 6c75 6d65 203d 206d 696e 2876 6f6c  volume = min(vol
+00003440: 756d 652c 2073 656c 662e 766f 6c75 6d65  ume, self.volume
+00003450: 290d 0a20 2020 2020 2020 2065 6c69 6620  )..        elif 
+00003460: 766f 6c75 6d65 203e 2073 656c 662e 766f  volume > self.vo
+00003470: 6c75 6d65 3a0d 0a20 2020 2020 2020 2020  lume:..         
+00003480: 2020 2072 6169 7365 2056 616c 7565 4572     raise ValueEr
+00003490: 726f 7228 2752 6571 7569 7265 6420 6469  ror('Required di
+000034a0: 7370 656e 7365 2076 6f6c 756d 6520 6973  spense volume is
+000034b0: 2067 7265 6174 6572 2074 6861 6e20 766f   greater than vo
+000034c0: 6c75 6d65 2069 6e20 7469 702e 2729 0d0a  lume in tip.')..
+000034d0: 2020 2020 2020 2020 7374 6570 7320 3d20          steps = 
+000034e0: 696e 7428 766f 6c75 6d65 202f 2073 656c  int(volume / sel
+000034f0: 662e 7265 736f 6c75 7469 6f6e 290d 0a20  f.resolution).. 
+00003500: 2020 2020 2020 2076 6f6c 756d 6520 3d20         volume = 
+00003510: 7374 6570 7320 2a20 7365 6c66 2e72 6573  steps * self.res
+00003520: 6f6c 7574 696f 6e0d 0a20 2020 2020 2020  olution..       
+00003530: 2069 6620 766f 6c75 6d65 203d 3d20 303a   if volume == 0:
+00003540: 0d0a 2020 2020 2020 2020 2020 2020 7265  ..            re
+00003550: 7475 726e 2027 270d 0a20 2020 2020 2020  turn ''..       
+00003560: 2070 7269 6e74 2866 2744 6973 7065 6e73   print(f'Dispens
+00003570: 696e 6720 7b76 6f6c 756d 657d 2075 4c2e  ing {volume} uL.
+00003580: 2e2e 2729 0d0a 2020 2020 2020 2020 7374  ..')..        st
+00003590: 6172 745f 6469 7370 656e 7365 203d 2074  art_dispense = t
+000035a0: 696d 652e 7065 7266 5f63 6f75 6e74 6572  ime.perf_counter
+000035b0: 2829 0d0a 2020 2020 2020 2020 7370 6565  ()..        spee
+000035c0: 6420 3d20 7365 6c66 2e73 7065 6564 2e64  d = self.speed.d
+000035d0: 6f77 6e20 6966 2073 7065 6564 2069 7320  own if speed is 
+000035e0: 4e6f 6e65 2065 6c73 6520 7370 6565 640d  None else speed.
+000035f0: 0a0d 0a20 2020 2020 2020 2069 6620 7370  ...        if sp
+00003600: 6565 6420 696e 2073 656c 662e 7370 6565  eed in self.spee
+00003610: 645f 7072 6573 6574 733a 0d0a 2020 2020  d_presets:..    
+00003620: 2020 2020 2020 2020 6966 2073 7065 6564          if speed
+00003630: 2021 3d20 7365 6c66 2e73 7065 6564 2e64   != self.speed.d
+00003640: 6f77 6e3a 0d0a 2020 2020 2020 2020 2020  own:..          
+00003650: 2020 2020 2020 7365 6c66 2e73 6574 5370        self.setSp
+00003660: 6565 6428 7370 6565 643d 7370 6565 642c  eed(speed=speed,
+00003670: 2075 703d 4661 6c73 652c 2064 6566 6175   up=False, defau
+00003680: 6c74 3d46 616c 7365 290d 0a20 2020 2020  lt=False)..     
+00003690: 2020 2020 2020 2073 7461 7274 5f64 6973         start_dis
+000036a0: 7065 6e73 6520 3d20 7469 6d65 2e70 6572  pense = time.per
+000036b0: 665f 636f 756e 7465 7228 290d 0a20 2020  f_counter()..   
+000036c0: 2020 2020 2020 2020 2072 6573 706f 6e73           respons
+000036d0: 6520 3d20 7365 6c66 2e5f 7175 6572 7928  e = self._query(
+000036e0: 6627 524f 7b73 7465 7073 7d27 290d 0a20  f'RO{steps}').. 
+000036f0: 2020 2020 2020 2020 2020 206d 6f76 655f             move_
+00003700: 7469 6d65 203d 2073 7465 7073 2a73 656c  time = steps*sel
+00003710: 662e 7265 736f 6c75 7469 6f6e 202f 2073  f.resolution / s
+00003720: 7065 6564 0d0a 2020 2020 2020 2020 2020  peed..          
+00003730: 2020 6475 7261 7469 6f6e 203d 2074 696d    duration = tim
+00003740: 652e 7065 7266 5f63 6f75 6e74 6572 2829  e.perf_counter()
+00003750: 202d 2073 7461 7274 5f64 6973 7065 6e73   - start_dispens
+00003760: 650d 0a20 2020 2020 2020 2020 2020 2069  e..            i
+00003770: 6620 6475 7261 7469 6f6e 203c 2028 6d6f  f duration < (mo
+00003780: 7665 5f74 696d 6529 3a0d 0a20 2020 2020  ve_time):..     
+00003790: 2020 2020 2020 2020 2020 2074 696d 652e             time.
+000037a0: 736c 6565 7028 6d6f 7665 5f74 696d 652d  sleep(move_time-
+000037b0: 6475 7261 7469 6f6e 290d 0a20 2020 2020  duration)..     
+000037c0: 2020 2020 2020 2023 2069 6620 7265 7370         # if resp
+000037d0: 6f6e 7365 2021 3d20 276f 6b27 3a0d 0a20  onse != 'ok':.. 
+000037e0: 2020 2020 2020 2020 2020 2023 2020 2020             #    
+000037f0: 2072 6574 7572 6e20 7265 7370 6f6e 7365   return response
+00003800: 0d0a 2020 2020 2020 2020 2020 2020 0d0a  ..            ..
+00003810: 2020 2020 2020 2020 656c 6966 2073 7065          elif spe
+00003820: 6564 206e 6f74 2069 6e20 7365 6c66 2e73  ed not in self.s
+00003830: 7065 6564 5f70 7265 7365 7473 3a0d 0a20  peed_presets:.. 
+00003840: 2020 2020 2020 2020 2020 2070 7269 6e74             print
+00003850: 2866 2254 6172 6765 743a 207b 766f 6c75  (f"Target: {volu
+00003860: 6d65 7d20 754c 2061 7420 7b73 7065 6564  me} uL at {speed
+00003870: 7d20 754c 2f73 2e2e 2e22 290d 0a20 2020  } uL/s...")..   
+00003880: 2020 2020 2020 2020 2073 7065 6564 5f70           speed_p
+00003890: 6172 616d 6574 6572 7320 3d20 7365 6c66  arameters = self
+000038a0: 2e5f 6361 6c63 756c 6174 655f 7370 6565  ._calculate_spee
+000038b0: 645f 7061 7261 6d65 7465 7273 2876 6f6c  d_parameters(vol
+000038c0: 756d 653d 766f 6c75 6d65 2c20 7370 6565  ume=volume, spee
+000038d0: 643d 7370 6565 6429 0d0a 2020 2020 2020  d=speed)..      
+000038e0: 2020 2020 2020 7072 696e 7428 7370 6565        print(spee
+000038f0: 645f 7061 7261 6d65 7465 7273 290d 0a20  d_parameters).. 
+00003900: 2020 2020 2020 2020 2020 2070 7265 7365             prese
+00003910: 7420 3d20 7370 6565 645f 7061 7261 6d65  t = speed_parame
+00003920: 7465 7273 2e70 7265 7365 740d 0a20 2020  ters.preset..   
+00003930: 2020 2020 2020 2020 2069 6620 7072 6573           if pres
+00003940: 6574 2069 7320 4e6f 6e65 3a0d 0a20 2020  et is None:..   
+00003950: 2020 2020 2020 2020 2020 2020 2023 2072               # r
+00003960: 6169 7365 2052 756e 7469 6d65 4572 726f  aise RuntimeErro
+00003970: 7228 2754 6172 6765 7420 7370 6565 6420  r('Target speed 
+00003980: 6e6f 7420 706f 7373 6962 6c65 2e27 290d  not possible.').
+00003990: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000039a0: 2070 7269 6e74 2827 5461 7267 6574 2073   print('Target s
+000039b0: 7065 6564 206e 6f74 2070 6f73 7369 626c  peed not possibl
+000039c0: 652e 2729 0d0a 2020 2020 2020 2020 2020  e.')..          
+000039d0: 2020 2020 2020 7265 7475 726e 0d0a 2020        return..  
+000039e0: 2020 2020 2020 2020 2020 7365 6c66 2e73            self.s
+000039f0: 6574 5370 6565 6428 7370 6565 643d 7072  etSpeed(speed=pr
+00003a00: 6573 6574 2c20 7570 3d46 616c 7365 2c20  eset, up=False, 
+00003a10: 6465 6661 756c 743d 4661 6c73 6529 0d0a  default=False)..
+00003a20: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
+00003a30: 2020 2020 2020 7374 6570 735f 6c65 6674        steps_left
+00003a40: 203d 2073 7465 7073 0d0a 2020 2020 2020   = steps..      
+00003a50: 2020 2020 2020 6465 6c61 7920 3d20 7370        delay = sp
+00003a60: 6565 645f 7061 7261 6d65 7465 7273 2e64  eed_parameters.d
+00003a70: 656c 6179 0d0a 2020 2020 2020 2020 2020  elay..          
+00003a80: 2020 7374 6570 5f73 697a 6520 3d20 7370    step_size = sp
+00003a90: 6565 645f 7061 7261 6d65 7465 7273 2e73  eed_parameters.s
+00003aa0: 7465 705f 7369 7a65 0d0a 2020 2020 2020  tep_size..      
+00003ab0: 2020 2020 2020 696e 7465 7276 616c 7320        intervals 
+00003ac0: 3d20 7370 6565 645f 7061 7261 6d65 7465  = speed_paramete
+00003ad0: 7273 2e69 6e74 6572 7661 6c73 0d0a 2020  rs.intervals..  
+00003ae0: 2020 2020 2020 2020 2020 7374 6172 745f            start_
+00003af0: 6469 7370 656e 7365 203d 2074 696d 652e  dispense = time.
+00003b00: 7065 7266 5f63 6f75 6e74 6572 2829 0d0a  perf_counter()..
+00003b10: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+00003b20: 6920 696e 2072 616e 6765 2869 6e74 6572  i in range(inter
+00003b30: 7661 6c73 293a 0d0a 2020 2020 2020 2020  vals):..        
+00003b40: 2020 2020 2020 2020 7374 6172 745f 7469          start_ti
+00003b50: 6d65 203d 2074 696d 652e 7065 7266 5f63  me = time.perf_c
+00003b60: 6f75 6e74 6572 2829 0d0a 2020 2020 2020  ounter()..      
+00003b70: 2020 2020 2020 2020 2020 7374 6570 203d            step =
+00003b80: 2073 7465 705f 7369 7a65 2069 6620 2869   step_size if (i
+00003b90: 2b31 2021 3d20 696e 7465 7276 616c 7329  +1 != intervals)
+00003ba0: 2065 6c73 6520 7374 6570 735f 6c65 6674   else steps_left
+00003bb0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00003bc0: 2020 6d6f 7665 5f74 696d 6520 3d20 7374    move_time = st
+00003bd0: 6570 2a73 656c 662e 7265 736f 6c75 7469  ep*self.resoluti
+00003be0: 6f6e 202f 2070 7265 7365 740d 0a20 2020  on / preset..   
+00003bf0: 2020 2020 2020 2020 2020 2020 2072 6573               res
+00003c00: 706f 6e73 6520 3d20 7365 6c66 2e5f 7175  ponse = self._qu
+00003c10: 6572 7928 6627 524f 7b73 7465 707d 272c  ery(f'RO{step}',
+00003c20: 2072 6573 756d 655f 6665 6564 6261 636b   resume_feedback
+00003c30: 3d46 616c 7365 2c20 6765 745f 706f 7369  =False, get_posi
+00003c40: 7469 6f6e 3d46 616c 7365 290d 0a20 2020  tion=False)..   
+00003c50: 2020 2020 2020 2020 2020 2020 2023 2069               # i
+00003c60: 6620 7265 7370 6f6e 7365 2021 3d20 276f  f response != 'o
+00003c70: 6b27 3a0d 0a20 2020 2020 2020 2020 2020  k':..           
+00003c80: 2020 2020 2023 2020 2020 2070 7269 6e74       #     print
+00003c90: 2822 4469 7370 656e 7365 2066 6169 6c65  ("Dispense faile
+00003ca0: 6422 290d 0a20 2020 2020 2020 2020 2020  d")..           
+00003cb0: 2020 2020 2023 2020 2020 2072 6574 7572       #     retur
+00003cc0: 6e20 7265 7370 6f6e 7365 0d0a 2020 2020  n response..    
+00003cd0: 2020 2020 2020 2020 2020 2020 7374 6570              step
+00003ce0: 735f 6c65 6674 202d 3d20 7374 6570 0d0a  s_left -= step..
+00003cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003d00: 6475 7261 7469 6f6e 203d 2074 696d 652e  duration = time.
+00003d10: 7065 7266 5f63 6f75 6e74 6572 2829 202d  perf_counter() -
+00003d20: 2073 7461 7274 5f74 696d 650d 0a20 2020   start_time..   
+00003d30: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+00003d40: 6475 7261 7469 6f6e 203c 2028 6465 6c61  duration < (dela
+00003d50: 792b 6d6f 7665 5f74 696d 6529 3a0d 0a20  y+move_time):.. 
+00003d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003d70: 2020 2074 696d 652e 736c 6565 7028 6465     time.sleep(de
+00003d80: 6c61 792b 6d6f 7665 5f74 696d 652d 6475  lay+move_time-du
+00003d90: 7261 7469 6f6e 290d 0a0d 0a20 2020 2020  ration)....     
+00003da0: 2020 2023 2055 7064 6174 6520 7661 6c75     # Update valu
+00003db0: 6573 0d0a 2020 2020 2020 2020 7072 696e  es..        prin
+00003dc0: 7428 6627 4469 7370 656e 7365 2074 696d  t(f'Dispense tim
+00003dd0: 653a 207b 7469 6d65 2e70 6572 665f 636f  e: {time.perf_co
+00003de0: 756e 7465 7228 292d 7374 6172 745f 6469  unter()-start_di
+00003df0: 7370 656e 7365 7d73 2729 0d0a 2020 2020  spense}s')..    
+00003e00: 2020 2020 7469 6d65 2e73 6c65 6570 2877      time.sleep(w
+00003e10: 6169 7429 0d0a 2020 2020 2020 2020 7365  ait)..        se
+00003e20: 6c66 2e73 6574 466c 6167 286f 6363 7570  lf.setFlag(occup
+00003e30: 6965 643d 4661 6c73 652c 2070 6175 7365  ied=False, pause
+00003e40: 5f66 6565 6462 6163 6b3d 4661 6c73 6529  _feedback=False)
+00003e50: 0d0a 2020 2020 2020 2020 7365 6c66 2e67  ..        self.g
+00003e60: 6574 506f 7369 7469 6f6e 2829 0d0a 2020  etPosition()..  
+00003e70: 2020 2020 2020 7365 6c66 2e76 6f6c 756d        self.volum
+00003e80: 6520 3d20 6d61 7828 7365 6c66 2e76 6f6c  e = max(self.vol
+00003e90: 756d 6520 2d20 766f 6c75 6d65 2c20 3029  ume - volume, 0)
+00003ea0: 0d0a 2020 2020 2020 2020 7365 6c66 2e70  ..        self.p
+00003eb0: 6f73 6974 696f 6e20 2d3d 2073 7465 7073  osition -= steps
+00003ec0: 0d0a 2020 2020 2020 2020 6966 2073 656c  ..        if sel
+00003ed0: 662e 766f 6c75 6d65 203d 3d20 3020 616e  f.volume == 0 an
+00003ee0: 6420 626c 6f77 6f75 743a 0d0a 2020 2020  d blowout:..    
+00003ef0: 2020 2020 2020 2020 7365 6c66 2e62 6c6f          self.blo
+00003f00: 776f 7574 2868 6f6d 653d 626c 6f77 6f75  wout(home=blowou
+00003f10: 745f 686f 6d65 290d 0a20 2020 2020 2020  t_home)..       
+00003f20: 2069 6620 7061 7573 653a 0d0a 2020 2020   if pause:..    
+00003f30: 2020 2020 2020 2020 696e 7075 7428 2250          input("P
+00003f40: 7265 7373 2027 456e 7465 7227 2074 6f20  ress 'Enter' to 
+00003f50: 7072 6f63 6565 642e 2229 0d0a 2020 2020  proceed.")..    
+00003f60: 2020 2020 7265 7475 726e 2072 6573 706f      return respo
+00003f70: 6e73 650d 0a20 2020 200d 0a20 2020 2064  nse..    ..    d
+00003f80: 6566 2065 6a65 6374 2873 656c 662c 2068  ef eject(self, h
+00003f90: 6f6d 653a 626f 6f6c 203d 2054 7275 6529  ome:bool = True)
+00003fa0: 202d 3e20 7374 723a 0d0a 2020 2020 2020   -> str:..      
+00003fb0: 2020 2222 220d 0a20 2020 2020 2020 2045    """..        E
+00003fc0: 6a65 6374 2074 6865 2070 6970 6574 7465  ject the pipette
+00003fd0: 2074 6970 0d0a 0d0a 2020 2020 2020 2020   tip....        
+00003fe0: 4172 6773 3a0d 0a20 2020 2020 2020 2020  Args:..         
+00003ff0: 2020 2068 6f6d 6520 2862 6f6f 6c2c 206f     home (bool, o
+00004000: 7074 696f 6e61 6c29 3a20 7768 6574 6865  ptional): whethe
+00004010: 7220 746f 2072 6574 7572 6e20 706c 756e  r to return plun
+00004020: 6765 7220 746f 2068 6f6d 6520 706f 7369  ger to home posi
+00004030: 7469 6f6e 2e20 4465 6661 756c 7473 2074  tion. Defaults t
+00004040: 6f20 5472 7565 2e0d 0a0d 0a20 2020 2020  o True.....     
+00004050: 2020 2052 6574 7572 6e73 3a0d 0a20 2020     Returns:..   
+00004060: 2020 2020 2020 2020 2073 7472 3a20 6465           str: de
+00004070: 7669 6365 2072 6573 706f 6e73 650d 0a20  vice response.. 
+00004080: 2020 2020 2020 2022 2222 0d0a 2020 2020         """..    
+00004090: 2020 2020 7365 6c66 2e72 6561 6765 6e74      self.reagent
+000040a0: 203d 2027 270d 0a20 2020 2020 2020 2063   = ''..        c
+000040b0: 6f6d 6d61 6e64 203d 2066 2752 457b 7365  ommand = f'RE{se
+000040c0: 6c66 2e68 6f6d 655f 706f 7369 7469 6f6e  lf.home_position
+000040d0: 7d27 2069 6620 686f 6d65 2065 6c73 6520  }' if home else 
+000040e0: 2752 4527 0d0a 2020 2020 2020 2020 7265  'RE'..        re
+000040f0: 7370 6f6e 7365 203d 2073 656c 662e 5f71  sponse = self._q
+00004100: 7565 7279 2863 6f6d 6d61 6e64 290d 0a20  uery(command).. 
+00004110: 2020 2020 2020 2073 656c 662e 706f 7369         self.posi
+00004120: 7469 6f6e 203d 2073 656c 662e 686f 6d65  tion = self.home
+00004130: 5f70 6f73 6974 696f 6e20 6966 2068 6f6d  _position if hom
+00004140: 6520 656c 7365 2030 0d0a 2020 2020 2020  e else 0..      
+00004150: 2020 7469 6d65 2e73 6c65 6570 2831 290d    time.sleep(1).
+00004160: 0a20 2020 2020 2020 2069 6620 6e6f 7420  .        if not 
+00004170: 7365 6c66 2e66 6c61 6773 5b27 636f 6e64  self.flags['cond
+00004180: 7563 7469 7665 5f74 6970 7327 5d3a 0d0a  uctive_tips']:..
+00004190: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+000041a0: 2e73 6574 466c 6167 2874 6970 5f6f 6e3d  .setFlag(tip_on=
+000041b0: 4661 6c73 6529 0d0a 2020 2020 2020 2020  False)..        
+000041c0: 7265 7475 726e 2072 6573 706f 6e73 650d  return response.
+000041d0: 0a20 2020 200d 0a20 2020 2064 6566 2067  .    ..    def g
+000041e0: 6574 4361 7061 6369 7461 6e63 6528 7365  etCapacitance(se
+000041f0: 6c66 2920 2d3e 2055 6e69 6f6e 5b69 6e74  lf) -> Union[int
+00004200: 2c20 7374 725d 3a0d 0a20 2020 2020 2020  , str]:..       
+00004210: 2022 2222 0d0a 2020 2020 2020 2020 4765   """..        Ge
+00004220: 7420 7468 6520 6361 7061 6369 7461 6e63  t the capacitanc
+00004230: 6520 6173 206d 6561 7375 7265 6420 6174  e as measured at
+00004240: 2074 6865 2065 6e64 206f 6620 7468 6520   the end of the 
+00004250: 7069 7065 7474 650d 0a20 2020 2020 2020  pipette..       
+00004260: 200d 0a20 2020 2020 2020 2052 6574 7572   ..        Retur
+00004270: 6e73 3a0d 0a20 2020 2020 2020 2020 2020  ns:..           
+00004280: 2055 6e69 6f6e 5b69 6e74 2c20 7374 725d   Union[int, str]
+00004290: 3a20 6361 7061 6369 7461 6e63 6520 7661  : capacitance va
+000042a0: 6c75 652c 206f 7220 6465 7669 6365 2072  lue, or device r
+000042b0: 6573 706f 6e73 650d 0a20 2020 2020 2020  esponse..       
+000042c0: 2022 2222 0d0a 2020 2020 2020 2020 7265   """..        re
+000042d0: 7370 6f6e 7365 203d 2073 656c 662e 5f71  sponse = self._q
+000042e0: 7565 7279 2827 444e 2729 0d0a 2020 2020  uery('DN')..    
+000042f0: 2020 2020 7472 793a 0d0a 2020 2020 2020      try:..      
+00004300: 2020 2020 2020 6361 7061 6369 7461 6e63        capacitanc
+00004310: 6520 3d20 696e 7428 7265 7370 6f6e 7365  e = int(response
+00004320: 290d 0a20 2020 2020 2020 2065 7863 6570  )..        excep
+00004330: 7420 5661 6c75 6545 7272 6f72 3a0d 0a20  t ValueError:.. 
+00004340: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+00004350: 6e20 7265 7370 6f6e 7365 0d0a 2020 2020  n response..    
+00004360: 2020 2020 7365 6c66 2e5f 6361 7061 6369      self._capaci
+00004370: 7461 6e63 6520 3d20 6361 7061 6369 7461  tance = capacita
+00004380: 6e63 650d 0a20 2020 2020 2020 2072 6574  nce..        ret
+00004390: 7572 6e20 6361 7061 6369 7461 6e63 650d  urn capacitance.
+000043a0: 0a20 0d0a 2020 2020 6465 6620 6765 7445  . ..    def getE
+000043b0: 7272 6f72 7328 7365 6c66 2920 2d3e 2073  rrors(self) -> s
+000043c0: 7472 3a0d 0a20 2020 2020 2020 2022 2222  tr:..        """
+000043d0: 0d0a 2020 2020 2020 2020 4765 7420 6572  ..        Get er
+000043e0: 726f 7273 2066 726f 6d20 7468 6520 6465  rors from the de
+000043f0: 7669 6365 0d0a 0d0a 2020 2020 2020 2020  vice....        
+00004400: 5265 7475 726e 733a 0d0a 2020 2020 2020  Returns:..      
+00004410: 2020 2020 2020 7374 723a 2064 6576 6963        str: devic
+00004420: 6520 7265 7370 6f6e 7365 0d0a 2020 2020  e response..    
+00004430: 2020 2020 2222 220d 0a20 2020 2020 2020      """..       
+00004440: 2072 6574 7572 6e20 7365 6c66 2e5f 7175   return self._qu
+00004450: 6572 7928 2744 4527 290d 0a20 2020 200d  ery('DE')..    .
+00004460: 0a20 2020 2064 6566 2067 6574 496e 666f  .    def getInfo
+00004470: 2873 656c 662c 206d 6f64 656c 3a20 4f70  (self, model: Op
+00004480: 7469 6f6e 616c 5b73 7472 5d20 3d20 4e6f  tional[str] = No
+00004490: 6e65 293a 0d0a 2020 2020 2020 2020 2222  ne):..        ""
+000044a0: 2247 6574 2064 6574 6169 6c73 206f 6620  "Get details of 
+000044b0: 7468 6520 5361 7274 6f72 6975 7320 7069  the Sartorius pi
+000044c0: 7065 7474 6520 6d6f 6465 6c22 2222 0d0a  pette model"""..
+000044d0: 2020 2020 2020 2020 6d6f 6465 6c20 3d20          model = 
+000044e0: 7365 6c66 2e5f 5f6d 6f64 656c 5f5f 2829  self.__model__()
+000044f0: 2e73 706c 6974 2827 2d27 295b 305d 2069  .split('-')[0] i
+00004500: 6620 6d6f 6465 6c20 6973 204e 6f6e 6520  f model is None 
+00004510: 656c 7365 206d 6f64 656c 0d0a 2020 2020  else model..    
+00004520: 2020 2020 6966 206d 6f64 656c 206e 6f74      if model not
+00004530: 2069 6e20 6c69 622e 4d6f 6465 6c49 6e66   in lib.ModelInf
+00004540: 6f2e 5f6d 656d 6265 725f 6e61 6d65 735f  o._member_names_
+00004550: 3a0d 0a20 2020 2020 2020 2020 2020 2070  :..            p
+00004560: 7269 6e74 2866 2752 6563 6569 7665 643a  rint(f'Received:
+00004570: 207b 6d6f 6465 6c7d 2729 0d0a 2020 2020   {model}')..    
+00004580: 2020 2020 2020 2020 6d6f 6465 6c20 3d20          model = 
+00004590: 2742 524c 3027 0d0a 2020 2020 2020 2020  'BRL0'..        
+000045a0: 2020 2020 7072 696e 7428 6622 4465 6661      print(f"Defa
+000045b0: 756c 7469 6e67 2074 6f3a 207b 2742 524c  ulting to: {'BRL
+000045c0: 3027 7d22 290d 0a20 2020 2020 2020 2020  0'}")..         
+000045d0: 2020 2070 7269 6e74 2866 2256 616c 6964     print(f"Valid
+000045e0: 206d 6f64 656c 7320 6172 653a 207b 272c   models are: {',
+000045f0: 2027 2e6a 6f69 6e28 6c69 622e 4d6f 6465   '.join(lib.Mode
+00004600: 6c49 6e66 6f2e 5f6d 656d 6265 725f 6e61  lInfo._member_na
+00004610: 6d65 735f 297d 2229 0d0a 2020 2020 2020  mes_)}")..      
+00004620: 2020 696e 666f 3a20 6c69 622e 4d6f 6465    info: lib.Mode
+00004630: 6c20 3d20 6c69 622e 4d6f 6465 6c49 6e66  l = lib.ModelInf
+00004640: 6f5b 6d6f 6465 6c5d 2e76 616c 7565 0d0a  o[model].value..
+00004650: 2020 2020 2020 2020 7072 696e 7428 696e          print(in
+00004660: 666f 290d 0a20 2020 2020 2020 2073 656c  fo)..        sel
+00004670: 662e 6d6f 6465 6c5f 696e 666f 203d 2069  f.model_info = i
+00004680: 6e66 6f0d 0a20 2020 2020 2020 2073 656c  nfo..        sel
+00004690: 662e 6361 7061 6369 7479 203d 2069 6e66  f.capacity = inf
+000046a0: 6f2e 6361 7061 6369 7479 0d0a 2020 2020  o.capacity..    
+000046b0: 2020 2020 7365 6c66 2e6c 696d 6974 7320      self.limits 
+000046c0: 3d20 2869 6e66 6f2e 7469 705f 656a 6563  = (info.tip_ejec
+000046d0: 745f 706f 7369 7469 6f6e 2c20 696e 666f  t_position, info
+000046e0: 2e6d 6178 5f70 6f73 6974 696f 6e29 0d0a  .max_position)..
+000046f0: 2020 2020 2020 2020 7365 6c66 2e73 7065          self.spe
+00004700: 6564 5f70 7265 7365 7473 203d 2069 6e66  ed_presets = inf
+00004710: 6f2e 7072 6573 6574 5f73 7065 6564 730d  o.preset_speeds.
+00004720: 0a20 2020 2020 2020 2073 656c 662e 7370  .        self.sp
+00004730: 6565 642e 7570 203d 2073 656c 662e 7370  eed.up = self.sp
+00004740: 6565 645f 7072 6573 6574 735b 7365 6c66  eed_presets[self
+00004750: 2e73 7065 6564 5f63 6f64 652e 7570 2d31  .speed_code.up-1
+00004760: 5d0d 0a20 2020 2020 2020 2073 656c 662e  ]..        self.
+00004770: 7370 6565 642e 646f 776e 203d 2073 656c  speed.down = sel
+00004780: 662e 7370 6565 645f 7072 6573 6574 735b  f.speed_presets[
+00004790: 7365 6c66 2e73 7065 6564 5f63 6f64 652e  self.speed_code.
+000047a0: 646f 776e 2d31 5d0d 0a20 2020 2020 2020  down-1]..       
+000047b0: 2072 6574 7572 6e0d 0a20 2020 200d 0a20   return..    .. 
+000047c0: 2020 2064 6566 2067 6574 506f 7369 7469     def getPositi
+000047d0: 6f6e 2873 656c 662c 202a 2a6b 7761 7267  on(self, **kwarg
+000047e0: 7329 202d 3e20 696e 743a 0d0a 2020 2020  s) -> int:..    
+000047f0: 2020 2020 2222 2247 6574 2074 6865 2063      """Get the c
+00004800: 7572 7265 6e74 2070 6f73 6974 696f 6e20  urrent position 
+00004810: 6f66 2074 6865 2070 6970 6574 7465 2222  of the pipette""
+00004820: 220d 0a20 2020 2020 2020 2072 6573 706f  "..        respo
+00004830: 6e73 6520 3d20 7365 6c66 2e5f 7175 6572  nse = self._quer
+00004840: 7928 2744 5027 290d 0a20 2020 2020 2020  y('DP')..       
+00004850: 2074 7279 3a0d 0a20 2020 2020 2020 2020   try:..         
+00004860: 2020 2070 6f73 6974 696f 6e20 3d20 696e     position = in
+00004870: 7428 7265 7370 6f6e 7365 290d 0a20 2020  t(response)..   
+00004880: 2020 2020 2065 7863 6570 7420 5661 6c75       except Valu
+00004890: 6545 7272 6f72 3a0d 0a20 2020 2020 2020  eError:..       
+000048a0: 2020 2020 2072 6574 7572 6e20 7265 7370       return resp
+000048b0: 6f6e 7365 0d0a 2020 2020 2020 2020 7365  onse..        se
+000048c0: 6c66 2e70 6f73 6974 696f 6e20 3d20 706f  lf.position = po
+000048d0: 7369 7469 6f6e 0d0a 2020 2020 2020 2020  sition..        
+000048e0: 7265 7475 726e 2073 656c 662e 706f 7369  return self.posi
+000048f0: 7469 6f6e 0d0a 2020 2020 2020 0d0a 2020  tion..      ..  
+00004900: 2020 6465 6620 6765 7453 7461 7475 7328    def getStatus(
+00004910: 7365 6c66 2c20 2a2a 6b77 6172 6773 2920  self, **kwargs) 
+00004920: 2d3e 2073 7472 3a0d 0a20 2020 2020 2020  -> str:..       
+00004930: 2022 2222 0d0a 2020 2020 2020 2020 4765   """..        Ge
+00004940: 7420 7468 6520 7374 6174 7573 206f 6620  t the status of 
+00004950: 7468 6520 7069 7065 7474 650d 0a0d 0a20  the pipette.... 
+00004960: 2020 2020 2020 2052 6574 7572 6e73 3a0d         Returns:.
+00004970: 0a20 2020 2020 2020 2020 2020 2073 7472  .            str
+00004980: 3a20 6465 7669 6365 2072 6573 706f 6e73  : device respons
+00004990: 650d 0a20 2020 2020 2020 2022 2222 0d0a  e..        """..
+000049a0: 2020 2020 2020 2020 7265 7370 6f6e 7365          response
+000049b0: 203d 2073 656c 662e 5f71 7565 7279 2827   = self._query('
+000049c0: 4453 2729 0d0a 2020 2020 2020 2020 7472  DS')..        tr
+000049d0: 793a 0d0a 2020 2020 2020 2020 2020 2020  y:..            
+000049e0: 7374 6174 7573 203d 2069 6e74 2872 6573  status = int(res
+000049f0: 706f 6e73 6529 0d0a 2020 2020 2020 2020  ponse)..        
+00004a00: 6578 6365 7074 2056 616c 7565 4572 726f  except ValueErro
+00004a10: 723a 0d0a 2020 2020 2020 2020 2020 2020  r:..            
+00004a20: 7265 7475 726e 2072 6573 706f 6e73 650d  return response.
+00004a30: 0a20 2020 2020 2020 2069 6620 7265 7370  .        if resp
+00004a40: 6f6e 7365 206e 6f74 2069 6e20 5b5f 7374  onse not in [_st
+00004a50: 6174 7573 2e76 616c 7565 2066 6f72 205f  atus.value for _
+00004a60: 7374 6174 7573 2069 6e20 6c69 622e 5374  status in lib.St
+00004a70: 6174 7573 436f 6465 5d3a 0d0a 2020 2020  atusCode]:..    
+00004a80: 2020 2020 2020 2020 7265 7475 726e 2072          return r
+00004a90: 6573 706f 6e73 650d 0a20 2020 2020 2020  esponse..       
+00004aa0: 200d 0a20 2020 2020 2020 2073 656c 662e   ..        self.
+00004ab0: 5f73 7461 7475 735f 636f 6465 203d 2073  _status_code = s
+00004ac0: 7461 7475 730d 0a20 2020 2020 2020 2069  tatus..        i
+00004ad0: 6620 7374 6174 7573 2069 6e20 5b34 2c36  f status in [4,6
+00004ae0: 2c38 5d3a 0d0a 2020 2020 2020 2020 2020  ,8]:..          
+00004af0: 2020 7365 6c66 2e73 6574 466c 6167 2862    self.setFlag(b
+00004b00: 7573 793d 5472 7565 290d 0a20 2020 2020  usy=True)..     
+00004b10: 2020 2020 2020 2069 6620 7365 6c66 2e76         if self.v
+00004b20: 6572 626f 7365 3a0d 0a20 2020 2020 2020  erbose:..       
+00004b30: 2020 2020 2020 2020 2070 7269 6e74 286c           print(l
+00004b40: 6962 2e53 7461 7475 7343 6f64 6528 7374  ib.StatusCode(st
+00004b50: 6174 7573 292e 6e61 6d65 290d 0a20 2020  atus).name)..   
+00004b60: 2020 2020 2065 6c69 6620 7374 6174 7573       elif status
+00004b70: 203d 3d20 303a 0d0a 2020 2020 2020 2020   == 0:..        
+00004b80: 2020 2020 7365 6c66 2e73 6574 466c 6167      self.setFlag
+00004b90: 2862 7573 793d 4661 6c73 6529 0d0a 2020  (busy=False)..  
+00004ba0: 2020 2020 2020 7265 7475 726e 206c 6962        return lib
+00004bb0: 2e53 7461 7475 7343 6f64 6528 7365 6c66  .StatusCode(self
+00004bc0: 2e5f 7374 6174 7573 5f63 6f64 6529 2e6e  ._status_code).n
+00004bd0: 616d 650d 0a20 2020 200d 0a20 2020 2064  ame..    ..    d
+00004be0: 6566 2068 6f6d 6528 7365 6c66 2920 2d3e  ef home(self) ->
+00004bf0: 2073 7472 3a0d 0a20 2020 2020 2020 2022   str:..        "
+00004c00: 2222 0d0a 2020 2020 2020 2020 5265 7475  ""..        Retu
+00004c10: 726e 2070 6c75 6e67 6572 2074 6f20 686f  rn plunger to ho
+00004c20: 6d65 2070 6f73 6974 696f 6e0d 0a20 2020  me position..   
+00004c30: 2020 2020 200d 0a20 2020 2020 2020 2052       ..        R
+00004c40: 6574 7572 6e73 3a0d 0a20 2020 2020 2020  eturns:..       
+00004c50: 2020 2020 2073 7472 3a20 6465 7669 6365       str: device
+00004c60: 2072 6573 706f 6e73 650d 0a20 2020 2020   response..     
+00004c70: 2020 2022 2222 0d0a 2020 2020 2020 2020     """..        
+00004c80: 7265 7370 6f6e 7365 203d 2073 656c 662e  response = self.
+00004c90: 5f71 7565 7279 2866 2752 507b 7365 6c66  _query(f'RP{self
+00004ca0: 2e68 6f6d 655f 706f 7369 7469 6f6e 7d27  .home_position}'
+00004cb0: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
+00004cc0: 766f 6c75 6d65 203d 2030 0d0a 2020 2020  volume = 0..    
+00004cd0: 2020 2020 7365 6c66 2e70 6f73 6974 696f      self.positio
+00004ce0: 6e20 3d20 7365 6c66 2e68 6f6d 655f 706f  n = self.home_po
+00004cf0: 7369 7469 6f6e 0d0a 2020 2020 2020 2020  sition..        
+00004d00: 7469 6d65 2e73 6c65 6570 2831 290d 0a20  time.sleep(1).. 
+00004d10: 2020 2020 2020 2072 6574 7572 6e20 7265         return re
+00004d20: 7370 6f6e 7365 0d0a 2020 2020 0d0a 2020  sponse..    ..  
+00004d30: 2020 6465 6620 6973 4665 6173 6962 6c65    def isFeasible
+00004d40: 2873 656c 662c 2070 6f73 6974 696f 6e3a  (self, position:
+00004d50: 696e 7429 202d 3e20 626f 6f6c 3a0d 0a20  int) -> bool:.. 
+00004d60: 2020 2020 2020 2022 2222 0d0a 2020 2020         """..    
+00004d70: 2020 2020 4368 6563 6b73 2061 6e64 2072      Checks and r
+00004d80: 6574 7572 6e73 2077 6865 7468 6572 2074  eturns whether t
+00004d90: 6865 2070 6c75 6e67 6572 2070 6f73 6974  he plunger posit
+00004da0: 696f 6e20 6973 2066 6561 7369 626c 650d  ion is feasible.
+00004db0: 0a0d 0a20 2020 2020 2020 2041 7267 733a  ...        Args:
+00004dc0: 0d0a 2020 2020 2020 2020 2020 2020 706f  ..            po
+00004dd0: 7369 7469 6f6e 2028 696e 7429 3a20 706c  sition (int): pl
+00004de0: 756e 6765 7220 706f 7369 7469 6f6e 0d0a  unger position..
+00004df0: 0d0a 2020 2020 2020 2020 5265 7475 726e  ..        Return
+00004e00: 733a 0d0a 2020 2020 2020 2020 2020 2020  s:..            
+00004e10: 626f 6f6c 3a20 7768 6574 6865 7220 706c  bool: whether pl
+00004e20: 756e 6765 7220 706f 7369 7469 6f6e 2069  unger position i
+00004e30: 7320 6665 6173 6962 6c65 0d0a 2020 2020  s feasible..    
+00004e40: 2020 2020 2222 220d 0a20 2020 2020 2020      """..       
+00004e50: 2069 6620 2873 656c 662e 6c69 6d69 7473   if (self.limits
+00004e60: 5b30 5d20 3c3d 2070 6f73 6974 696f 6e20  [0] <= position 
+00004e70: 3c3d 2073 656c 662e 6c69 6d69 7473 5b31  <= self.limits[1
+00004e80: 5d29 3a0d 0a20 2020 2020 2020 2020 2020  ]):..           
+00004e90: 2072 6574 7572 6e20 5472 7565 0d0a 2020   return True..  
+00004ea0: 2020 2020 2020 7072 696e 7428 6622 5261        print(f"Ra
+00004eb0: 6e67 6520 6c69 6d69 7473 2072 6561 6368  nge limits reach
+00004ec0: 6564 2120 7b73 656c 662e 6c69 6d69 7473  ed! {self.limits
+00004ed0: 7d22 290d 0a20 2020 2020 2020 2072 6574  }")..        ret
+00004ee0: 7572 6e20 4661 6c73 650d 0a20 2020 200d  urn False..    .
+00004ef0: 0a20 2020 2064 6566 2069 7354 6970 4f6e  .    def isTipOn
+00004f00: 2873 656c 6629 202d 3e20 626f 6f6c 3a0d  (self) -> bool:.
+00004f10: 0a20 2020 2020 2020 2022 2222 0d0a 2020  .        """..  
+00004f20: 2020 2020 2020 4368 6563 6b73 2061 6e64        Checks and
+00004f30: 2072 6574 7572 6e73 2077 6865 7468 6572   returns whether
+00004f40: 2061 2070 6970 6574 7465 2074 6970 2069   a pipette tip i
+00004f50: 7320 6174 7461 6368 6564 0d0a 2020 2020  s attached..    
+00004f60: 2020 2020 0d0a 2020 2020 2020 2020 5265      ..        Re
+00004f70: 7475 726e 733a 0d0a 2020 2020 2020 2020  turns:..        
+00004f80: 2020 2020 626f 6f6c 3a20 7768 6574 6865      bool: whethe
+00004f90: 7220 6120 7069 7065 7474 6520 7469 7020  r a pipette tip 
+00004fa0: 696e 2061 7474 6163 6865 640d 0a20 2020  in attached..   
+00004fb0: 2020 2020 2022 2222 0d0a 2020 2020 2020       """..      
+00004fc0: 2020 7365 6c66 2e67 6574 4361 7061 6369    self.getCapaci
+00004fd0: 7461 6e63 6528 290d 0a20 2020 2020 2020  tance()..       
+00004fe0: 2070 7269 6e74 2866 2754 6970 2063 6170   print(f'Tip cap
+00004ff0: 6163 6974 616e 6365 3a20 7b73 656c 662e  acitance: {self.
+00005000: 6361 7061 6369 7461 6e63 657d 2729 0d0a  capacitance}')..
+00005010: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+00005020: 666c 6167 735b 2763 6f6e 6475 6374 6976  flags['conductiv
+00005030: 655f 7469 7073 275d 3a0d 0a20 2020 2020  e_tips']:..     
+00005040: 2020 2020 2020 2074 6970 5f6f 6e20 3d20         tip_on = 
+00005050: 2873 656c 662e 6361 7061 6369 7461 6e63  (self.capacitanc
+00005060: 6520 3e20 7365 6c66 2e74 6970 5f74 6872  e > self.tip_thr
+00005070: 6573 686f 6c64 290d 0a20 2020 2020 2020  eshold)..       
+00005080: 2020 2020 2073 656c 662e 7365 7446 6c61       self.setFla
+00005090: 6728 7469 705f 6f6e 3d74 6970 5f6f 6e29  g(tip_on=tip_on)
+000050a0: 0d0a 2020 2020 2020 2020 7469 705f 6f6e  ..        tip_on
+000050b0: 203d 2073 656c 662e 666c 6167 735b 2774   = self.flags['t
+000050c0: 6970 5f6f 6e27 5d0d 0a20 2020 2020 2020  ip_on']..       
+000050d0: 2072 6574 7572 6e20 7469 705f 6f6e 0d0a   return tip_on..
+000050e0: 2020 2020 0d0a 2020 2020 6465 6620 6d6f      ..    def mo
+000050f0: 7665 2873 656c 662c 2073 7465 7073 3a69  ve(self, steps:i
+00005100: 6e74 2c20 7570 3a62 6f6f 6c2c 202a 2a6b  nt, up:bool, **k
+00005110: 7761 7267 7329 202d 3e20 7374 723a 0d0a  wargs) -> str:..
+00005120: 2020 2020 2020 2020 2222 220d 0a20 2020          """..   
+00005130: 2020 2020 204d 6f76 6520 7468 6520 706c       Move the pl
+00005140: 756e 6765 7220 6569 7468 6572 2075 7020  unger either up 
+00005150: 6f72 2064 6f77 6e20 6279 2061 2073 7065  or down by a spe
+00005160: 6369 6669 6564 206e 756d 6265 7220 6f66  cified number of
+00005170: 2073 7465 7073 0d0a 0d0a 2020 2020 2020   steps....      
+00005180: 2020 4172 6773 3a0d 0a20 2020 2020 2020    Args:..       
+00005190: 2020 2020 2073 7465 7073 2028 696e 7429       steps (int)
+000051a0: 3a20 6e75 6d62 6572 206f 6620 7374 6570  : number of step
+000051b0: 7320 746f 206d 6f76 6520 706c 756e 6765  s to move plunge
+000051c0: 7220 6279 0d0a 2020 2020 2020 2020 2020  r by..          
+000051d0: 2020 7570 2028 626f 6f6c 293a 2077 6865    up (bool): whe
+000051e0: 7468 6572 2074 6f20 6d6f 7665 2074 6865  ther to move the
+000051f0: 2070 6c75 6e67 6572 2075 700d 0a0d 0a20   plunger up.... 
+00005200: 2020 2020 2020 2052 6574 7572 6e73 3a0d         Returns:.
+00005210: 0a20 2020 2020 2020 2020 2020 2073 7472  .            str
+00005220: 3a20 6465 7669 6365 2072 6573 706f 6e73  : device respons
+00005230: 650d 0a20 2020 2020 2020 2022 2222 0d0a  e..        """..
+00005240: 2020 2020 2020 2020 7374 6570 7320 3d20          steps = 
+00005250: 6162 7328 7374 6570 7329 2069 6620 7570  abs(steps) if up
+00005260: 2065 6c73 6520 2d61 6273 2873 7465 7073   else -abs(steps
+00005270: 290d 0a20 2020 2020 2020 2072 6574 7572  )..        retur
+00005280: 6e20 7365 6c66 2e6d 6f76 6542 7928 7374  n self.moveBy(st
+00005290: 6570 7329 0d0a 2020 2020 0d0a 2020 2020  eps)..    ..    
+000052a0: 6465 6620 6d6f 7665 4279 2873 656c 662c  def moveBy(self,
+000052b0: 2073 7465 7073 3a69 6e74 2c20 2a2a 6b77   steps:int, **kw
+000052c0: 6172 6773 2920 2d3e 2073 7472 3a0d 0a20  args) -> str:.. 
+000052d0: 2020 2020 2020 2022 2222 0d0a 2020 2020         """..    
+000052e0: 2020 2020 4d6f 7665 2074 6865 2070 6c75      Move the plu
+000052f0: 6e67 6572 2062 7920 7370 6563 6966 6965  nger by specifie
+00005300: 6420 6e75 6d62 6572 206f 6620 7374 6570  d number of step
+00005310: 730d 0a0d 0a20 2020 2020 2020 2041 7267  s....        Arg
+00005320: 733a 0d0a 2020 2020 2020 2020 2020 2020  s:..            
+00005330: 7374 6570 7320 2869 6e74 293a 206e 756d  steps (int): num
+00005340: 6265 7220 6f66 2073 7465 7073 2074 6f20  ber of steps to 
+00005350: 6d6f 7665 2070 6c75 6e67 6572 2062 7920  move plunger by 
+00005360: 283c 303a 206d 6f76 6520 646f 776e 2f64  (<0: move down/d
+00005370: 6973 7065 6e73 653b 203e 3020 6d6f 7665  ispense; >0 move
+00005380: 2075 702f 6173 7069 7261 7465 290d 0a0d   up/aspirate)...
+00005390: 0a20 2020 2020 2020 2052 6574 7572 6e73  .        Returns
+000053a0: 3a0d 0a20 2020 2020 2020 2020 2020 2073  :..            s
+000053b0: 7472 3a20 6465 7669 6365 2072 6573 706f  tr: device respo
+000053c0: 6e73 650d 0a20 2020 2020 2020 2022 2222  nse..        """
+000053d0: 0d0a 2020 2020 2020 2020 636f 6d6d 616e  ..        comman
+000053e0: 6420 3d20 6627 5249 7b73 7465 7073 7d27  d = f'RI{steps}'
+000053f0: 2069 6620 7374 6570 7320 3e20 3020 656c   if steps > 0 el
+00005400: 7365 2066 2752 4f7b 2d73 7465 7073 7d27  se f'RO{-steps}'
+00005410: 0d0a 2020 2020 2020 2020 7365 6c66 2e70  ..        self.p
+00005420: 6f73 6974 696f 6e20 2b3d 2073 7465 7073  osition += steps
+00005430: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
+00005440: 2073 656c 662e 5f71 7565 7279 2863 6f6d   self._query(com
+00005450: 6d61 6e64 290d 0a20 2020 200d 0a20 2020  mand)..    ..   
+00005460: 2064 6566 206d 6f76 6554 6f28 7365 6c66   def moveTo(self
+00005470: 2c20 706f 7369 7469 6f6e 3a69 6e74 2c20  , position:int, 
+00005480: 2a2a 6b77 6172 6773 2920 2d3e 2073 7472  **kwargs) -> str
+00005490: 3a0d 0a20 2020 2020 2020 2022 2222 0d0a  :..        """..
+000054a0: 2020 2020 2020 2020 4d6f 7665 2074 6865          Move the
+000054b0: 2070 6c75 6e67 6572 2074 6f20 6120 7370   plunger to a sp
+000054c0: 6563 6966 6965 6420 706f 7369 7469 6f6e  ecified position
+000054d0: 0d0a 0d0a 2020 2020 2020 2020 4172 6773  ....        Args
+000054e0: 3a0d 0a20 2020 2020 2020 2020 2020 2070  :..            p
+000054f0: 6f73 6974 696f 6e20 2869 6e74 293a 2074  osition (int): t
+00005500: 6172 6765 7420 706c 756e 6765 7220 706f  arget plunger po
+00005510: 7369 7469 6f6e 0d0a 0d0a 2020 2020 2020  sition....      
+00005520: 2020 5265 7475 726e 733a 0d0a 2020 2020    Returns:..    
+00005530: 2020 2020 2020 2020 7374 723a 2064 6576          str: dev
+00005540: 6963 6520 7265 7370 6f6e 7365 0d0a 2020  ice response..  
+00005550: 2020 2020 2020 2222 220d 0a20 2020 2020        """..     
+00005560: 2020 2073 656c 662e 706f 7369 7469 6f6e     self.position
+00005570: 203d 2070 6f73 6974 696f 6e0d 0a20 2020   = position..   
+00005580: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
+00005590: 2e5f 7175 6572 7928 6627 5250 7b70 6f73  ._query(f'RP{pos
+000055a0: 6974 696f 6e7d 2729 0d0a 2020 2020 0d0a  ition}')..    ..
+000055b0: 2020 2020 6465 6620 7075 6c6c 6261 636b      def pullback
+000055c0: 2873 656c 662c 2073 7465 7073 3a69 6e74  (self, steps:int
+000055d0: 203d 2035 2c20 2a2a 6b77 6172 6773 2920   = 5, **kwargs) 
+000055e0: 2d3e 2073 7472 3a0d 0a20 2020 2020 2020  -> str:..       
+000055f0: 2022 2222 0d0a 2020 2020 2020 2020 5075   """..        Pu
+00005600: 6c6c 6261 636b 206c 6971 7569 6420 6672  llback liquid fr
+00005610: 6f6d 2074 6970 0d0a 2020 2020 2020 2020  om tip..        
+00005620: 0d0a 2020 2020 2020 2020 4172 6773 3a0d  ..        Args:.
+00005630: 0a20 2020 2020 2020 2020 2020 2073 7465  .            ste
+00005640: 7073 2028 696e 742c 206f 7074 696f 6e61  ps (int, optiona
+00005650: 6c29 3a20 6e75 6d62 6572 206f 6620 7374  l): number of st
+00005660: 6570 7320 746f 2070 756c 6c62 6163 6b2e  eps to pullback.
+00005670: 2044 6566 6175 6c74 7320 746f 2035 2e0d   Defaults to 5..
+00005680: 0a0d 0a20 2020 2020 2020 2052 6574 7572  ...        Retur
+00005690: 6e73 3a0d 0a20 2020 2020 2020 2020 2020  ns:..           
+000056a0: 2073 7472 3a20 6465 7669 6365 2072 6573   str: device res
+000056b0: 706f 6e73 650d 0a20 2020 2020 2020 2022  ponse..        "
+000056c0: 2222 0d0a 2020 2020 2020 2020 7265 7370  ""..        resp
+000056d0: 6f6e 7365 203d 2073 656c 662e 5f71 7565  onse = self._que
+000056e0: 7279 2866 2752 497b 7374 6570 737d 2729  ry(f'RI{steps}')
+000056f0: 0d0a 2020 2020 2020 2020 7365 6c66 2e70  ..        self.p
+00005700: 6f73 6974 696f 6e20 2b3d 2073 7465 7073  osition += steps
+00005710: 0d0a 2020 2020 2020 2020 7469 6d65 2e73  ..        time.s
+00005720: 6c65 6570 2831 290d 0a20 2020 2020 2020  leep(1)..       
+00005730: 2072 6574 7572 6e20 7265 7370 6f6e 7365   return response
+00005740: 0d0a 2020 2020 0d0a 2020 2020 6465 6620  ..    ..    def 
+00005750: 7265 7365 7428 7365 6c66 2920 2d3e 2073  reset(self) -> s
+00005760: 7472 3a0d 0a20 2020 2020 2020 2022 2222  tr:..        """
+00005770: 0d0a 2020 2020 2020 2020 5265 7365 7420  ..        Reset 
+00005780: 7468 6520 7069 7065 7474 650d 0a0d 0a20  the pipette.... 
+00005790: 2020 2020 2020 2052 6574 7572 6e73 3a0d         Returns:.
+000057a0: 0a20 2020 2020 2020 2020 2020 2073 7472  .            str
+000057b0: 3a20 6465 7669 6365 2072 6573 706f 6e73  : device respons
+000057c0: 650d 0a20 2020 2020 2020 2022 2222 0d0a  e..        """..
+000057d0: 2020 2020 2020 2020 7365 6c66 2e7a 6572          self.zer
+000057e0: 6f28 290d 0a20 2020 2020 2020 2072 6574  o()..        ret
+000057f0: 7572 6e20 7365 6c66 2e68 6f6d 6528 290d  urn self.home().
+00005800: 0a20 2020 200d 0a20 2020 2064 6566 2073  .    ..    def s
+00005810: 6574 5370 6565 6428 7365 6c66 2c20 7370  etSpeed(self, sp
+00005820: 6565 643a 696e 742c 2075 703a 626f 6f6c  eed:int, up:bool
+00005830: 2c20 6465 6661 756c 743a 626f 6f6c 203d  , default:bool =
+00005840: 2046 616c 7365 2c20 2a2a 6b77 6172 6773   False, **kwargs
+00005850: 2920 2d3e 2073 7472 3a0d 0a20 2020 2020  ) -> str:..     
+00005860: 2020 2022 2222 0d0a 2020 2020 2020 2020     """..        
+00005870: 5365 7420 7468 6520 7370 6565 6420 6f66  Set the speed of
+00005880: 2074 6865 2070 6c75 6e67 6572 0d0a 0d0a   the plunger....
+00005890: 2020 2020 2020 2020 4172 6773 3a0d 0a20          Args:.. 
+000058a0: 2020 2020 2020 2020 2020 2073 7065 6564             speed
+000058b0: 2028 696e 7429 3a20 7370 6565 6420 6f66   (int): speed of
+000058c0: 2070 6c75 6e67 6572 0d0a 2020 2020 2020   plunger..      
+000058d0: 2020 2020 2020 7570 2028 626f 6f6c 293a        up (bool):
+000058e0: 2064 6972 6563 7469 6f6e 206f 6620 7472   direction of tr
+000058f0: 6176 656c 0d0a 2020 2020 2020 2020 2020  avel..          
+00005900: 2020 6465 6661 756c 7420 2862 6f6f 6c2c    default (bool,
+00005910: 206f 7074 696f 6e61 6c29 3a20 7768 6574   optional): whet
+00005920: 6865 7220 746f 2073 6574 2073 7065 6564  her to set speed
+00005930: 2061 7320 6120 6465 6661 756c 742e 2044   as a default. D
+00005940: 6566 6175 6c74 7320 746f 2046 616c 7365  efaults to False
+00005950: 2e0d 0a0d 0a20 2020 2020 2020 2052 6574  .....        Ret
+00005960: 7572 6e73 3a0d 0a20 2020 2020 2020 2020  urns:..         
+00005970: 2020 2073 7472 3a20 6465 7669 6365 2072     str: device r
+00005980: 6573 706f 6e73 650d 0a20 2020 2020 2020  esponse..       
+00005990: 2022 2222 0d0a 2020 2020 2020 2020 7370   """..        sp
+000059a0: 6565 645f 636f 6465 203d 2031 202b 205b  eed_code = 1 + [
+000059b0: 7820 666f 7220 782c 7661 6c20 696e 2065  x for x,val in e
+000059c0: 6e75 6d65 7261 7465 286e 702e 6172 7261  numerate(np.arra
+000059d0: 7928 7365 6c66 2e73 7065 6564 5f70 7265  y(self.speed_pre
+000059e0: 7365 7473 292d 7370 6565 6429 2069 6620  sets)-speed) if 
+000059f0: 7661 6c20 3e3d 2030 5d5b 305d 0d0a 2020  val >= 0][0]..  
+00005a00: 2020 2020 2020 7072 696e 7428 6627 5370        print(f'Sp
+00005a10: 6565 6420 7b73 7065 6564 5f63 6f64 657d  eed {speed_code}
+00005a20: 3a20 7b73 656c 662e 7370 6565 645f 7072  : {self.speed_pr
+00005a30: 6573 6574 735b 7370 6565 645f 636f 6465  esets[speed_code
+00005a40: 2d31 5d7d 2075 4c2f 7327 290d 0a20 2020  -1]} uL/s')..   
+00005a50: 2020 2020 2064 6972 6563 7469 6f6e 203d       direction =
+00005a60: 2027 4927 2069 6620 7570 2065 6c73 6520   'I' if up else 
+00005a70: 274f 270d 0a20 2020 2020 2020 2073 656c  'O'..        sel
+00005a80: 662e 5f71 7565 7279 2866 2753 7b64 6972  f._query(f'S{dir
+00005a90: 6563 7469 6f6e 7d7b 7370 6565 645f 636f  ection}{speed_co
+00005aa0: 6465 7d27 290d 0a20 2020 2020 2020 2069  de}')..        i
+00005ab0: 6620 6e6f 7420 6465 6661 756c 743a 0d0a  f not default:..
+00005ac0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00005ad0: 726e 2073 656c 662e 5f71 7565 7279 2866  rn self._query(f
+00005ae0: 2744 7b64 6972 6563 7469 6f6e 7d27 290d  'D{direction}').
+00005af0: 0a20 2020 2020 2020 2069 6620 7570 3a0d  .        if up:.
+00005b00: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00005b10: 662e 7370 6565 645f 636f 6465 2e75 7020  f.speed_code.up 
+00005b20: 3d20 7370 6565 645f 636f 6465 0d0a 2020  = speed_code..  
+00005b30: 2020 2020 2020 2020 2020 7365 6c66 2e73            self.s
+00005b40: 7065 6564 2e75 7020 3d20 7365 6c66 2e73  peed.up = self.s
+00005b50: 7065 6564 5f70 7265 7365 7473 5b73 7065  peed_presets[spe
+00005b60: 6564 5f63 6f64 652d 315d 0d0a 2020 2020  ed_code-1]..    
+00005b70: 2020 2020 656c 7365 3a0d 0a20 2020 2020      else:..     
+00005b80: 2020 2020 2020 2073 656c 662e 7370 6565         self.spee
+00005b90: 645f 636f 6465 2e64 6f77 6e20 3d20 7370  d_code.down = sp
+00005ba0: 6565 645f 636f 6465 0d0a 2020 2020 2020  eed_code..      
+00005bb0: 2020 2020 2020 7365 6c66 2e73 7065 6564        self.speed
+00005bc0: 2e64 6f77 6e20 3d20 7365 6c66 2e73 7065  .down = self.spe
+00005bd0: 6564 5f70 7265 7365 7473 5b73 7065 6564  ed_presets[speed
+00005be0: 5f63 6f64 652d 315d 0d0a 2020 2020 2020  _code-1]..      
+00005bf0: 2020 7265 7475 726e 2073 656c 662e 5f71    return self._q
+00005c00: 7565 7279 2866 2744 7b64 6972 6563 7469  uery(f'D{directi
+00005c10: 6f6e 7d27 290d 0a20 2020 200d 0a20 2020  on}')..    ..   
+00005c20: 2064 6566 2073 6875 7464 6f77 6e28 7365   def shutdown(se
+00005c30: 6c66 293a 0d0a 2020 2020 2020 2020 2222  lf):..        ""
+00005c40: 2253 6875 7464 6f77 6e20 7072 6f63 6564  "Shutdown proced
+00005c50: 7572 6520 666f 7220 746f 6f6c 2222 220d  ure for tool""".
+00005c60: 0a20 2020 2020 2020 2073 656c 662e 746f  .        self.to
+00005c70: 6767 6c65 4665 6564 6261 636b 4c6f 6f70  ggleFeedbackLoop
+00005c80: 286f 6e3d 4661 6c73 6529 0d0a 2020 2020  (on=False)..    
+00005c90: 2020 2020 7265 7475 726e 2073 7570 6572      return super
+00005ca0: 2829 2e73 6875 7464 6f77 6e28 290d 0a20  ().shutdown().. 
+00005cb0: 2020 200d 0a20 2020 2064 6566 2074 6f67     ..    def tog
+00005cc0: 676c 6546 6565 6462 6163 6b4c 6f6f 7028  gleFeedbackLoop(
+00005cd0: 7365 6c66 2c20 6f6e 3a62 6f6f 6c29 3a0d  self, on:bool):.
+00005ce0: 0a20 2020 2020 2020 2022 2222 0d0a 2020  .        """..  
+00005cf0: 2020 2020 2020 5374 6172 7420 6f72 2073        Start or s
+00005d00: 746f 7020 6665 6564 6261 636b 206c 6f6f  top feedback loo
+00005d10: 700d 0a20 2020 2020 2020 200d 0a20 2020  p..        ..   
+00005d20: 2020 2020 2041 7267 733a 0d0a 2020 2020       Args:..    
+00005d30: 2020 2020 2020 2020 6f6e 2028 626f 6f6c          on (bool
+00005d40: 293a 2077 6865 7468 6572 2074 6f20 7374  ): whether to st
+00005d50: 6172 7420 6665 6564 6261 636b 206c 6f6f  art feedback loo
+00005d60: 700d 0a20 2020 2020 2020 2022 2222 0d0a  p..        """..
+00005d70: 2020 2020 2020 2020 7365 6c66 2e73 6574          self.set
+00005d80: 466c 6167 2867 6574 5f66 6565 6462 6163  Flag(get_feedbac
+00005d90: 6b3d 6f6e 290d 0a20 2020 2020 2020 2069  k=on)..        i
+00005da0: 6620 6f6e 3a0d 0a20 2020 2020 2020 2020  f on:..         
+00005db0: 2020 2069 6620 2766 6565 6462 6163 6b5f     if 'feedback_
+00005dc0: 6c6f 6f70 2720 696e 2073 656c 662e 5f74  loop' in self._t
+00005dd0: 6872 6561 6473 3a0d 0a20 2020 2020 2020  hreads:..       
+00005de0: 2020 2020 2020 2020 2073 656c 662e 5f74           self._t
+00005df0: 6872 6561 6473 5b27 6665 6564 6261 636b  hreads['feedback
+00005e00: 5f6c 6f6f 7027 5d2e 6a6f 696e 2829 0d0a  _loop'].join()..
+00005e10: 2020 2020 2020 2020 2020 2020 7468 7265              thre
+00005e20: 6164 203d 2054 6872 6561 6428 7461 7267  ad = Thread(targ
+00005e30: 6574 3d73 656c 662e 5f6c 6f6f 705f 6665  et=self._loop_fe
+00005e40: 6564 6261 636b 290d 0a20 2020 2020 2020  edback)..       
+00005e50: 2020 2020 2074 6872 6561 642e 7374 6172       thread.star
+00005e60: 7428 290d 0a20 2020 2020 2020 2020 2020  t()..           
+00005e70: 2073 656c 662e 5f74 6872 6561 6473 5b27   self._threads['
+00005e80: 6665 6564 6261 636b 5f6c 6f6f 7027 5d20  feedback_loop'] 
+00005e90: 3d20 7468 7265 6164 0d0a 2020 2020 2020  = thread..      
+00005ea0: 2020 656c 7365 3a0d 0a20 2020 2020 2020    else:..       
+00005eb0: 2020 2020 2069 6620 2766 6565 6462 6163       if 'feedbac
+00005ec0: 6b5f 6c6f 6f70 2720 696e 2073 656c 662e  k_loop' in self.
+00005ed0: 5f74 6872 6561 6473 3a0d 0a20 2020 2020  _threads:..     
+00005ee0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00005ef0: 5f74 6872 6561 6473 5b27 6665 6564 6261  _threads['feedba
+00005f00: 636b 5f6c 6f6f 7027 5d2e 6a6f 696e 2829  ck_loop'].join()
+00005f10: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
+00005f20: 0d0a 0d0a 2020 2020 6465 6620 7a65 726f  ....    def zero
+00005f30: 2873 656c 6629 202d 3e20 7374 723a 0d0a  (self) -> str:..
+00005f40: 2020 2020 2020 2020 2222 220d 0a20 2020          """..   
+00005f50: 2020 2020 205a 6572 6f20 7468 6520 706c       Zero the pl
+00005f60: 756e 6765 7220 706f 7369 7469 6f6e 0d0a  unger position..
+00005f70: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
+00005f80: 2020 5265 7475 726e 733a 0d0a 2020 2020    Returns:..    
+00005f90: 2020 2020 2020 2020 7374 723a 2064 6576          str: dev
+00005fa0: 6963 6520 7265 7370 6f6e 7365 0d0a 2020  ice response..  
+00005fb0: 2020 2020 2020 2222 220d 0a20 2020 2020        """..     
+00005fc0: 2020 2073 656c 662e 656a 6563 7428 290d     self.eject().
+00005fd0: 0a20 2020 2020 2020 2072 6573 706f 6e73  .        respons
+00005fe0: 6520 3d20 7365 6c66 2e5f 7175 6572 7928  e = self._query(
+00005ff0: 2752 5a27 290d 0a20 2020 2020 2020 2073  'RZ')..        s
+00006000: 656c 662e 706f 7369 7469 6f6e 203d 2030  elf.position = 0
+00006010: 0d0a 2020 2020 2020 2020 7469 6d65 2e73  ..        time.s
+00006020: 6c65 6570 2832 290d 0a20 2020 2020 2020  leep(2)..       
+00006030: 2072 6574 7572 6e20 7265 7370 6f6e 7365   return response
+00006040: 0d0a 0d0a 2020 2020 2320 5072 6f74 6563  ....    # Protec
+00006050: 7465 6420 6d65 7468 6f64 2873 290d 0a20  ted method(s).. 
+00006060: 2020 2064 6566 205f 6361 6c63 756c 6174     def _calculat
+00006070: 655f 7370 6565 645f 7061 7261 6d65 7465  e_speed_paramete
+00006080: 7273 2873 656c 662c 2076 6f6c 756d 653a  rs(self, volume:
+00006090: 696e 742c 2073 7065 6564 3a69 6e74 2920  int, speed:int) 
+000060a0: 2d3e 206c 6962 2e53 7065 6564 5061 7261  -> lib.SpeedPara
+000060b0: 6d65 7465 7273 3a0d 0a20 2020 2020 2020  meters:..       
+000060c0: 2022 2222 0d0a 2020 2020 2020 2020 4361   """..        Ca
+000060d0: 6c63 756c 6174 6573 2074 6865 2062 6573  lculates the bes
+000060e0: 7420 7061 7261 6d65 7465 7273 2066 6f72  t parameters for
+000060f0: 2076 6f6c 756d 6520 616e 6420 7370 6565   volume and spee
+00006100: 640d 0a0d 0a20 2020 2020 2020 2041 7267  d....        Arg
+00006110: 733a 0d0a 2020 2020 2020 2020 2020 2020  s:..            
+00006120: 766f 6c75 6d65 2028 696e 7429 3a20 766f  volume (int): vo
+00006130: 6c75 6d65 2074 6f20 6265 2074 7261 6e73  lume to be trans
+00006140: 6665 7272 6564 0d0a 2020 2020 2020 2020  ferred..        
+00006150: 2020 2020 7370 6565 6420 2869 6e74 293a      speed (int):
+00006160: 2073 7065 6564 2061 7420 7768 6963 6820   speed at which 
+00006170: 6c69 7175 6964 2069 7320 7472 616e 7366  liquid is transf
+00006180: 6572 7265 640d 0a0d 0a20 2020 2020 2020  erred....       
+00006190: 2052 6574 7572 6e73 3a0d 0a20 2020 2020   Returns:..     
+000061a0: 2020 2020 2020 2064 6963 743a 2064 6963         dict: dic
+000061b0: 7469 6f6e 6172 7920 6f66 2062 6573 7420  tionary of best 
+000061c0: 7061 7261 6d65 7465 7273 0d0a 2020 2020  parameters..    
+000061d0: 2020 2020 2222 220d 0a20 2020 2020 2020      """..       
+000061e0: 206f 7574 636f 6d65 7320 3d20 7b7d 0d0a   outcomes = {}..
+000061f0: 2020 2020 2020 2020 7374 6570 5f69 6e74          step_int
+00006200: 6572 7661 6c5f 6c69 6d69 7420 3d20 696e  erval_limit = in
+00006210: 7428 766f 6c75 6d65 2f73 656c 662e 7265  t(volume/self.re
+00006220: 736f 6c75 7469 6f6e 2f53 5445 505f 5245  solution/STEP_RE
+00006230: 534f 4c55 5449 4f4e 290d 0a20 2020 2020  SOLUTION)..     
+00006240: 2020 2066 6f72 2070 7265 7365 7420 696e     for preset in
+00006250: 2073 656c 662e 7370 6565 645f 7072 6573   self.speed_pres
+00006260: 6574 733a 0d0a 2020 2020 2020 2020 2020  ets:..          
+00006270: 2020 6966 2070 7265 7365 7420 3c20 7370    if preset < sp
+00006280: 6565 643a 0d0a 2020 2020 2020 2020 2020  eed:..          
+00006290: 2020 2020 2020 2320 7072 6573 6574 2069        # preset i
+000062a0: 7320 736c 6f77 6572 2074 6861 6e20 7461  s slower than ta
+000062b0: 7267 6574 2073 7065 6564 2c20 6974 2077  rget speed, it w
+000062c0: 696c 6c20 6e65 7665 7220 6869 7420 7461  ill never hit ta
+000062d0: 7267 6574 2073 7065 6564 0d0a 2020 2020  rget speed..    
+000062e0: 2020 2020 2020 2020 2020 2020 636f 6e74              cont
+000062f0: 696e 7565 0d0a 2020 2020 2020 2020 2020  inue..          
+00006300: 2020 7469 6d65 5f69 6e74 6572 7661 6c5f    time_interval_
+00006310: 6c69 6d69 7420 3d20 696e 7428 766f 6c75  limit = int(volu
+00006320: 6d65 2a28 312f 7370 6565 6420 2d20 312f  me*(1/speed - 1/
+00006330: 7072 6573 6574 292f 7365 6c66 2e72 6573  preset)/self.res
+00006340: 706f 6e73 655f 7469 6d65 290d 0a20 2020  ponse_time)..   
+00006350: 2020 2020 2020 2020 2069 6620 6e6f 7420           if not 
+00006360: 7374 6570 5f69 6e74 6572 7661 6c5f 6c69  step_interval_li
+00006370: 6d69 7420 6f72 206e 6f74 2074 696d 655f  mit or not time_
+00006380: 696e 7465 7276 616c 5f6c 696d 6974 3a0d  interval_limit:.
+00006390: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000063a0: 2063 6f6e 7469 6e75 650d 0a20 2020 2020   continue..     
+000063b0: 2020 2020 2020 2069 6e74 6572 7661 6c73         intervals
+000063c0: 203d 206d 6178 286d 696e 2873 7465 705f   = max(min(step_
+000063d0: 696e 7465 7276 616c 5f6c 696d 6974 2c20  interval_limit, 
+000063e0: 7469 6d65 5f69 6e74 6572 7661 6c5f 6c69  time_interval_li
+000063f0: 6d69 7429 2c20 3129 0d0a 2020 2020 2020  mit), 1)..      
+00006400: 2020 2020 2020 6561 6368 5f73 7465 7073        each_steps
+00006410: 203d 2076 6f6c 756d 652f 7365 6c66 2e72   = volume/self.r
+00006420: 6573 6f6c 7574 696f 6e2f 696e 7465 7276  esolution/interv
+00006430: 616c 730d 0a20 2020 2020 2020 2020 2020  als..           
+00006440: 2065 6163 685f 6465 6c61 7920 3d20 766f   each_delay = vo
+00006450: 6c75 6d65 2a28 312f 7370 6565 6420 2d20  lume*(1/speed - 
+00006460: 312f 7072 6573 6574 292f 696e 7465 7276  1/preset)/interv
+00006470: 616c 730d 0a20 2020 2020 2020 2020 2020  als..           
+00006480: 2061 7265 6120 3d20 302e 3520 2a20 2876   area = 0.5 * (v
+00006490: 6f6c 756d 652a 2a32 2920 2a20 2831 2f73  olume**2) * (1/s
+000064a0: 656c 662e 7265 736f 6c75 7469 6f6e 2920  elf.resolution) 
+000064b0: 2a20 2831 2f69 6e74 6572 7661 6c73 2920  * (1/intervals) 
+000064c0: 2a20 2831 2f73 7065 6564 202d 2031 2f70  * (1/speed - 1/p
+000064d0: 7265 7365 7429 0d0a 2020 2020 2020 2020  reset)..        
+000064e0: 2020 2020 6f75 7463 6f6d 6573 5b61 7265      outcomes[are
+000064f0: 615d 203d 206c 6962 2e53 7065 6564 5061  a] = lib.SpeedPa
+00006500: 7261 6d65 7465 7273 2870 7265 7365 742c  rameters(preset,
+00006510: 2069 6e74 6572 7661 6c73 2c20 696e 7428   intervals, int(
+00006520: 6561 6368 5f73 7465 7073 292c 2065 6163  each_steps), eac
+00006530: 685f 6465 6c61 7929 0d0a 2020 2020 2020  h_delay)..      
+00006540: 2020 6966 206c 656e 286f 7574 636f 6d65    if len(outcome
+00006550: 7329 203d 3d20 303a 0d0a 2020 2020 2020  s) == 0:..      
+00006560: 2020 2020 2020 7072 696e 7428 224e 6f20        print("No 
+00006570: 6665 6173 6962 6c65 2073 7065 6564 2070  feasible speed p
+00006580: 6172 616d 6574 6572 732e 2229 0d0a 2020  arameters.")..  
+00006590: 2020 2020 2020 2020 2020 7265 7475 726e            return
+000065a0: 206c 6962 2e53 7065 6564 5061 7261 6d65   lib.SpeedParame
+000065b0: 7465 7273 284e 6f6e 652c 2053 5445 505f  ters(None, STEP_
+000065c0: 5245 534f 4c55 5449 4f4e 2c20 5354 4550  RESOLUTION, STEP
+000065d0: 5f52 4553 4f4c 5554 494f 4e2c 2073 656c  _RESOLUTION, sel
+000065e0: 662e 7265 7370 6f6e 7365 5f74 696d 6529  f.response_time)
+000065f0: 0d0a 2020 2020 2020 2020 7072 696e 7428  ..        print(
+00006600: 6627 4265 7374 2070 6172 616d 6574 6572  f'Best parameter
+00006610: 733a 207b 6f75 7463 6f6d 6573 5b6d 696e  s: {outcomes[min
+00006620: 286f 7574 636f 6d65 7329 5d7d 2729 0d0a  (outcomes)]}')..
+00006630: 2020 2020 2020 2020 7265 7475 726e 206f          return o
+00006640: 7574 636f 6d65 735b 6d69 6e28 6f75 7463  utcomes[min(outc
+00006650: 6f6d 6573 295d 0d0a 2020 2020 0d0a 2020  omes)]..    ..  
+00006660: 2020 6465 6620 5f63 6f6e 6e65 6374 2873    def _connect(s
+00006670: 656c 662c 2070 6f72 743a 7374 722c 2062  elf, port:str, b
+00006680: 6175 6472 6174 653a 696e 7420 3d20 3936  audrate:int = 96
+00006690: 3030 2c20 7469 6d65 6f75 743a 696e 7420  00, timeout:int 
+000066a0: 3d20 3129 3a0d 0a20 2020 2020 2020 2022  = 1):..        "
+000066b0: 2222 0d0a 2020 2020 2020 2020 436f 6e6e  ""..        Conn
+000066c0: 6563 7469 6f6e 2070 726f 6365 6475 7265  ection procedure
+000066d0: 2066 6f72 2074 6f6f 6c0d 0a0d 0a20 2020   for tool....   
+000066e0: 2020 2020 2041 7267 733a 0d0a 2020 2020       Args:..    
+000066f0: 2020 2020 2020 2020 706f 7274 2028 7374          port (st
+00006700: 7229 3a20 434f 4d20 706f 7274 2061 6464  r): COM port add
+00006710: 7265 7373 0d0a 2020 2020 2020 2020 2020  ress..          
+00006720: 2020 6261 7564 7261 7465 2028 696e 742c    baudrate (int,
+00006730: 206f 7074 696f 6e61 6c29 3a20 6261 7564   optional): baud
+00006740: 7261 7465 2e20 4465 6661 756c 7473 2074  rate. Defaults t
+00006750: 6f20 3936 3030 2e0d 0a20 2020 2020 2020  o 9600...       
+00006760: 2020 2020 2074 696d 656f 7574 2028 696e       timeout (in
+00006770: 742c 206f 7074 696f 6e61 6c29 3a20 7469  t, optional): ti
+00006780: 6d65 6f75 7420 696e 2073 6563 6f6e 6473  meout in seconds
+00006790: 2e20 4465 6661 756c 7473 2074 6f20 312e  . Defaults to 1.
+000067a0: 0d0a 2020 2020 2020 2020 2222 220d 0a20  ..        """.. 
+000067b0: 2020 2020 2020 2073 656c 662e 636f 6e6e         self.conn
+000067c0: 6563 7469 6f6e 5f64 6574 6169 6c73 203d  ection_details =
+000067d0: 207b 0d0a 2020 2020 2020 2020 2020 2020   {..            
+000067e0: 2770 6f72 7427 3a20 706f 7274 2c0d 0a20  'port': port,.. 
+000067f0: 2020 2020 2020 2020 2020 2027 6261 7564             'baud
+00006800: 7261 7465 273a 2062 6175 6472 6174 652c  rate': baudrate,
+00006810: 0d0a 2020 2020 2020 2020 2020 2020 2774  ..            't
+00006820: 696d 656f 7574 273a 2074 696d 656f 7574  imeout': timeout
+00006830: 0d0a 2020 2020 2020 2020 7d0d 0a20 2020  ..        }..   
+00006840: 2020 2020 2064 6576 6963 6520 3d20 4e6f       device = No
+00006850: 6e65 0d0a 2020 2020 2020 2020 7472 793a  ne..        try:
+00006860: 0d0a 2020 2020 2020 2020 2020 2020 6465  ..            de
+00006870: 7669 6365 203d 2073 6572 6961 6c2e 5365  vice = serial.Se
+00006880: 7269 616c 2870 6f72 742c 2062 6175 6472  rial(port, baudr
+00006890: 6174 652c 2074 696d 656f 7574 3d74 696d  ate, timeout=tim
+000068a0: 656f 7574 290d 0a20 2020 2020 2020 2065  eout)..        e
+000068b0: 7863 6570 7420 4578 6365 7074 696f 6e20  xcept Exception 
+000068c0: 6173 2065 3a0d 0a20 2020 2020 2020 2020  as e:..         
+000068d0: 2020 2070 7269 6e74 2866 2243 6f75 6c64     print(f"Could
+000068e0: 206e 6f74 2063 6f6e 6e65 6374 2074 6f20   not connect to 
+000068f0: 7b70 6f72 747d 2229 0d0a 2020 2020 2020  {port}")..      
+00006900: 2020 2020 2020 6966 2073 656c 662e 7665        if self.ve
+00006910: 7262 6f73 653a 0d0a 2020 2020 2020 2020  rbose:..        
+00006920: 2020 2020 2020 2020 7072 696e 7428 6529          print(e)
+00006930: 0d0a 2020 2020 2020 2020 656c 7365 3a0d  ..        else:.
+00006940: 0a20 2020 2020 2020 2020 2020 2074 696d  .            tim
+00006950: 652e 736c 6565 7028 3229 2020 2023 2057  e.sleep(2)   # W
+00006960: 6169 7420 666f 7220 6772 626c 2074 6f20  ait for grbl to 
+00006970: 696e 6974 6961 6c69 7a65 0d0a 2020 2020  initialize..    
+00006980: 2020 2020 2020 2020 6465 7669 6365 2e72          device.r
+00006990: 6573 6574 5f69 6e70 7574 5f62 7566 6665  eset_input_buffe
+000069a0: 7228 290d 0a20 2020 2020 2020 2020 2020  r()..           
+000069b0: 2070 7269 6e74 2866 2243 6f6e 6e65 6374   print(f"Connect
+000069c0: 696f 6e20 6f70 656e 6564 2074 6f20 7b70  ion opened to {p
+000069d0: 6f72 747d 2229 0d0a 2020 2020 2020 2020  ort}")..        
+000069e0: 2020 2020 7365 6c66 2e73 6574 466c 6167      self.setFlag
+000069f0: 2863 6f6e 6e65 6374 6564 3d54 7275 6529  (connected=True)
+00006a00: 0d0a 2020 2020 2020 2020 7365 6c66 2e64  ..        self.d
+00006a10: 6576 6963 6520 3d20 6465 7669 6365 0d0a  evice = device..
+00006a20: 2020 2020 2020 2020 7365 6c66 2e67 6574          self.get
+00006a30: 496e 666f 2829 0d0a 2020 2020 2020 2020  Info()..        
+00006a40: 7365 6c66 2e72 6573 6574 2829 0d0a 2020  self.reset()..  
+00006a50: 2020 2020 2020 7265 7475 726e 0d0a 2020        return..  
+00006a60: 2020 0d0a 2020 2020 6465 6620 5f69 735f    ..    def _is_
+00006a70: 6578 7065 6374 6564 5f72 6570 6c79 2873  expected_reply(s
+00006a80: 656c 662c 2072 6573 706f 6e73 653a 7374  elf, response:st
+00006a90: 722c 2063 6f6d 6d61 6e64 5f63 6f64 653a  r, command_code:
+00006aa0: 7374 722c 202a 2a6b 7761 7267 7329 202d  str, **kwargs) -
+00006ab0: 3e20 626f 6f6c 3a0d 0a20 2020 2020 2020  > bool:..       
+00006ac0: 2022 2222 0d0a 2020 2020 2020 2020 4368   """..        Ch
+00006ad0: 6563 6b73 2061 6e64 2072 6574 7572 6e73  ecks and returns
+00006ae0: 2077 6865 7468 6572 2074 6865 2072 6573   whether the res
+00006af0: 706f 6e73 6520 6973 2061 6e20 6578 7065  ponse is an expe
+00006b00: 6374 6564 2072 6570 6c79 0d0a 0d0a 2020  cted reply....  
+00006b10: 2020 2020 2020 4172 6773 3a0d 0a20 2020        Args:..   
+00006b20: 2020 2020 2020 2020 2072 6573 706f 6e73           respons
+00006b30: 6520 2873 7472 293a 2072 6573 706f 6e73  e (str): respons
+00006b40: 6520 7374 7269 6e67 2066 726f 6d20 6465  e string from de
+00006b50: 7669 6365 0d0a 2020 2020 2020 2020 2020  vice..          
+00006b60: 2020 636f 6d6d 616e 645f 636f 6465 2028    command_code (
+00006b70: 7374 7229 3a20 7477 6f2d 6368 6172 6163  str): two-charac
+00006b80: 7465 7220 636f 6d6d 616e 6420 636f 6465  ter command code
+00006b90: 0d0a 0d0a 2020 2020 2020 2020 5265 7475  ....        Retu
+00006ba0: 726e 733a 0d0a 2020 2020 2020 2020 2020  rns:..          
+00006bb0: 2020 626f 6f6c 3a20 7768 6574 6865 7220    bool: whether 
+00006bc0: 7468 6520 7265 7370 6f6e 7365 2069 7320  the response is 
+00006bd0: 616e 2065 7870 6563 7465 6420 7265 706c  an expected repl
+00006be0: 790d 0a20 2020 2020 2020 2022 2222 0d0a  y..        """..
+00006bf0: 2020 2020 2020 2020 6966 2072 6573 706f          if respo
+00006c00: 6e73 6520 696e 206c 6962 2e45 7272 6f72  nse in lib.Error
+00006c10: 436f 6465 2e5f 6d65 6d62 6572 5f6e 616d  Code._member_nam
+00006c20: 6573 5f3a 0d0a 2020 2020 2020 2020 2020  es_:..          
+00006c30: 2020 7265 7475 726e 2054 7275 650d 0a20    return True.. 
+00006c40: 2020 2020 2020 2069 6620 636f 6d6d 616e         if comman
+00006c50: 645f 636f 6465 206e 6f74 2069 6e20 5155  d_code not in QU
+00006c60: 4552 4945 5320 616e 6420 7265 7370 6f6e  ERIES and respon
+00006c70: 7365 203d 3d20 276f 6b27 3a0d 0a20 2020  se == 'ok':..   
+00006c80: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+00006c90: 5472 7565 0d0a 2020 2020 2020 2020 6966  True..        if
+00006ca0: 2063 6f6d 6d61 6e64 5f63 6f64 6520 696e   command_code in
+00006cb0: 2051 5545 5249 4553 2061 6e64 2072 6573   QUERIES and res
+00006cc0: 706f 6e73 655b 3a32 5d20 3d3d 2063 6f6d  ponse[:2] == com
+00006cd0: 6d61 6e64 5f63 6f64 652e 6c6f 7765 7228  mand_code.lower(
+00006ce0: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
+00006cf0: 7265 706c 795f 636f 6465 2c20 6461 7461  reply_code, data
+00006d00: 203d 2072 6573 706f 6e73 655b 3a32 5d2c   = response[:2],
+00006d10: 2072 6573 706f 6e73 655b 323a 5d0d 0a20   response[2:].. 
+00006d20: 2020 2020 2020 2020 2020 2069 6620 7365             if se
+00006d30: 6c66 2e76 6572 626f 7365 3a0d 0a20 2020  lf.verbose:..   
+00006d40: 2020 2020 2020 2020 2020 2020 2070 7269               pri
+00006d50: 6e74 2866 275b 7b72 6570 6c79 5f63 6f64  nt(f'[{reply_cod
+00006d60: 657d 5d20 7b64 6174 617d 2729 0d0a 2020  e}] {data}')..  
+00006d70: 2020 2020 2020 2020 2020 7265 7475 726e            return
+00006d80: 2054 7275 650d 0a20 2020 2020 2020 2072   True..        r
+00006d90: 6574 7572 6e20 4661 6c73 650d 0a0d 0a20  eturn False.... 
+00006da0: 2020 2064 6566 205f 6c6f 6f70 5f66 6565     def _loop_fee
+00006db0: 6462 6163 6b28 7365 6c66 293a 0d0a 2020  dback(self):..  
+00006dc0: 2020 2020 2020 2222 224c 6f6f 7020 746f        """Loop to
+00006dd0: 2063 6f6e 7374 616e 746c 7920 7265 6164   constantly read
+00006de0: 2066 726f 6d20 6465 7669 6365 2222 220d   from device""".
+00006df0: 0a20 2020 2020 2020 2070 7269 6e74 2827  .        print('
+00006e00: 4c69 7374 656e 696e 672e 2e2e 2729 0d0a  Listening...')..
+00006e10: 2020 2020 2020 2020 7768 696c 6520 7365          while se
+00006e20: 6c66 2e66 6c61 6773 5b27 6765 745f 6665  lf.flags['get_fe
+00006e30: 6564 6261 636b 275d 3a0d 0a20 2020 2020  edback']:..     
+00006e40: 2020 2020 2020 2069 6620 7365 6c66 2e66         if self.f
+00006e50: 6c61 6773 5b27 7061 7573 655f 6665 6564  lags['pause_feed
+00006e60: 6261 636b 275d 3a0d 0a20 2020 2020 2020  back']:..       
+00006e70: 2020 2020 2020 2020 2063 6f6e 7469 6e75           continu
+00006e80: 650d 0a20 2020 2020 2020 2020 2020 2073  e..            s
+00006e90: 656c 662e 6765 7453 7461 7475 7328 290d  elf.getStatus().
+00006ea0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00006eb0: 662e 6765 7443 6170 6163 6974 616e 6365  f.getCapacitance
+00006ec0: 2829 0d0a 2020 2020 2020 2020 7072 696e  ()..        prin
+00006ed0: 7428 2753 746f 7020 6c69 7374 656e 696e  t('Stop listenin
+00006ee0: 672e 2e2e 2729 0d0a 2020 2020 2020 2020  g...')..        
+00006ef0: 7265 7475 726e 0d0a 2020 2020 0d0a 2020  return..    ..  
+00006f00: 2020 6465 6620 5f71 7565 7279 2873 656c    def _query(sel
+00006f10: 662c 200d 0a20 2020 2020 2020 2063 6f6d  f, ..        com
+00006f20: 6d61 6e64 3a20 7374 722c 200d 0a20 2020  mand: str, ..   
+00006f30: 2020 2020 2074 696d 656f 7574 5f73 3a20       timeout_s: 
+00006f40: 666c 6f61 7420 3d20 302e 332c 200d 0a20  float = 0.3, .. 
+00006f50: 2020 2020 2020 2072 6573 756d 655f 6665         resume_fe
+00006f60: 6564 6261 636b 3a20 626f 6f6c 203d 2046  edback: bool = F
+00006f70: 616c 7365 2c0d 0a20 2020 2020 2020 2067  alse,..        g
+00006f80: 6574 5f70 6f73 6974 696f 6e3a 2062 6f6f  et_position: boo
+00006f90: 6c20 3d20 5472 7565 0d0a 2020 2020 2920  l = True..    ) 
+00006fa0: 2d3e 2073 7472 3a0d 0a20 2020 2020 2020  -> str:..       
+00006fb0: 2022 2222 0d0a 2020 2020 2020 2020 5772   """..        Wr
+00006fc0: 6974 6520 636f 6d6d 616e 6420 746f 2061  ite command to a
+00006fd0: 6e64 2072 6561 6420 7265 7370 6f6e 7365  nd read response
+00006fe0: 2066 726f 6d20 6465 7669 6365 0d0a 0d0a   from device....
+00006ff0: 2020 2020 2020 2020 4172 6773 3a0d 0a20          Args:.. 
+00007000: 2020 2020 2020 2020 2020 2063 6f6d 6d61             comma
+00007010: 6e64 2028 7374 7229 3a20 636f 6d6d 616e  nd (str): comman
+00007020: 6420 7374 7269 6e67 0d0a 2020 2020 2020  d string..      
+00007030: 2020 2020 2020 7469 6d65 6f75 745f 7320        timeout_s 
+00007040: 2866 6c6f 6174 2c20 6f70 7469 6f6e 616c  (float, optional
+00007050: 293a 2064 7572 6174 696f 6e20 746f 2077  ): duration to w
+00007060: 6169 7420 6265 666f 7265 2074 696d 656f  ait before timeo
+00007070: 7574 2e20 4465 6661 756c 7473 2074 6f20  ut. Defaults to 
+00007080: 302e 332e 0d0a 2020 2020 2020 2020 2020  0.3...          
+00007090: 2020 7265 7375 6d65 5f66 6565 6462 6163    resume_feedbac
+000070a0: 6b20 2862 6f6f 6c2c 206f 7074 696f 6e61  k (bool, optiona
+000070b0: 6c29 3a20 7768 6574 6865 7220 746f 2072  l): whether to r
+000070c0: 6573 756d 6520 7265 6164 696e 6720 6672  esume reading fr
+000070d0: 6f6d 2064 6576 6963 652e 2044 6566 6175  om device. Defau
+000070e0: 6c74 7320 746f 2046 616c 7365 2e0d 0a20  lts to False... 
+000070f0: 2020 2020 2020 2020 2020 2067 6574 5f70             get_p
+00007100: 6f73 6974 696f 6e20 2862 6f6f 6c2c 206f  osition (bool, o
+00007110: 7074 696f 6e61 6c29 3a20 7768 6574 6865  ptional): whethe
+00007120: 7220 746f 2067 6574 2074 6865 2070 6f73  r to get the pos
+00007130: 6974 696f 6e20 6f66 2074 6865 2070 6c75  ition of the plu
+00007140: 6e67 6572 2e20 4465 6661 756c 7473 2074  nger. Defaults t
+00007150: 6f20 5472 7565 2e0d 0a20 2020 2020 2020  o True...       
+00007160: 2052 6574 7572 6e73 3a0d 0a20 2020 2020   Returns:..     
+00007170: 2020 2020 2020 2073 7472 3a20 7265 7370         str: resp
+00007180: 6f6e 7365 2073 7472 696e 670d 0a20 2020  onse string..   
+00007190: 2020 2020 2022 2222 0d0a 2020 2020 2020       """..      
+000071a0: 2020 636f 6d6d 616e 645f 636f 6465 203d    command_code =
+000071b0: 2063 6f6d 6d61 6e64 5b3a 325d 0d0a 2020   command[:2]..  
+000071c0: 2020 2020 2020 6966 2063 6f6d 6d61 6e64        if command
+000071d0: 5f63 6f64 6520 6e6f 7420 696e 206c 6962  _code not in lib
+000071e0: 2e53 7461 7475 7351 7565 7279 436f 6465  .StatusQueryCode
+000071f0: 2e5f 6d65 6d62 6572 5f6e 616d 6573 5f3a  ._member_names_:
+00007200: 0d0a 2020 2020 2020 2020 2020 2020 6966  ..            if
+00007210: 2073 656c 662e 666c 6167 735b 2767 6574   self.flags['get
+00007220: 5f66 6565 6462 6163 6b27 5d20 616e 6420  _feedback'] and 
+00007230: 6e6f 7420 7365 6c66 2e66 6c61 6773 5b27  not self.flags['
+00007240: 7061 7573 655f 6665 6564 6261 636b 275d  pause_feedback']
+00007250: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00007260: 2020 2073 656c 662e 7365 7446 6c61 6728     self.setFlag(
+00007270: 7061 7573 655f 6665 6564 6261 636b 3d54  pause_feedback=T
+00007280: 7275 6529 0d0a 2020 2020 2020 2020 2020  rue)..          
+00007290: 2020 2020 2020 7469 6d65 2e73 6c65 6570        time.sleep
+000072a0: 2874 696d 656f 7574 5f73 290d 0a20 2020  (timeout_s)..   
+000072b0: 2020 2020 2020 2020 2023 2073 656c 662e           # self.
+000072c0: 6765 7453 7461 7475 7328 290d 0a20 2020  getStatus()..   
+000072d0: 2020 2020 2020 2020 2023 2077 6869 6c65           # while
+000072e0: 2073 656c 662e 6973 4275 7379 2829 3a0d   self.isBusy():.
+000072f0: 0a20 2020 2020 2020 2020 2020 2023 2020  .            #  
+00007300: 2020 2073 656c 662e 6765 7453 7461 7475     self.getStatu
+00007310: 7328 290d 0a20 2020 2020 2020 2020 2020  s()..           
+00007320: 2069 6620 7365 6c66 2e69 7342 7573 7928   if self.isBusy(
+00007330: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
+00007340: 2020 2020 7469 6d65 2e73 6c65 6570 2874      time.sleep(t
+00007350: 696d 656f 7574 5f73 290d 0a20 2020 2020  imeout_s)..     
+00007360: 2020 200d 0a20 2020 2020 2020 2073 7461     ..        sta
+00007370: 7274 5f74 696d 6520 3d20 7469 6d65 2e70  rt_time = time.p
+00007380: 6572 665f 636f 756e 7465 7228 290d 0a20  erf_counter().. 
+00007390: 2020 2020 2020 2073 656c 662e 5f77 7269         self._wri
+000073a0: 7465 2863 6f6d 6d61 6e64 290d 0a20 2020  te(command)..   
+000073b0: 2020 2020 2072 6573 706f 6e73 6520 3d20       response = 
+000073c0: 2727 0d0a 2020 2020 2020 2020 7768 696c  ''..        whil
+000073d0: 6520 6e6f 7420 7365 6c66 2e5f 6973 5f65  e not self._is_e
+000073e0: 7870 6563 7465 645f 7265 706c 7928 7265  xpected_reply(re
+000073f0: 7370 6f6e 7365 2c20 636f 6d6d 616e 645f  sponse, command_
+00007400: 636f 6465 293a 0d0a 2020 2020 2020 2020  code):..        
+00007410: 2020 2020 6966 2074 696d 652e 7065 7266      if time.perf
+00007420: 5f63 6f75 6e74 6572 2829 202d 2073 7461  _counter() - sta
+00007430: 7274 5f74 696d 6520 3e20 7469 6d65 6f75  rt_time > timeou
+00007440: 745f 733a 0d0a 2020 2020 2020 2020 2020  t_s:..          
+00007450: 2020 2020 2020 6272 6561 6b0d 0a20 2020        break..   
+00007460: 2020 2020 2020 2020 2072 6573 706f 6e73           respons
+00007470: 6520 3d20 7365 6c66 2e5f 7265 6164 2829  e = self._read()
+00007480: 0d0a 2020 2020 2020 2020 2320 7072 696e  ..        # prin
+00007490: 7428 7469 6d65 2e70 6572 665f 636f 756e  t(time.perf_coun
+000074a0: 7465 7228 2920 2d20 7374 6172 745f 7469  ter() - start_ti
+000074b0: 6d65 290d 0a20 2020 2020 2020 2069 6620  me)..        if 
+000074c0: 636f 6d6d 616e 645f 636f 6465 2069 6e20  command_code in 
+000074d0: 5155 4552 4945 533a 0d0a 2020 2020 2020  QUERIES:..      
+000074e0: 2020 2020 2020 7265 7370 6f6e 7365 203d        response =
+000074f0: 2072 6573 706f 6e73 655b 323a 5d0d 0a20   response[2:].. 
+00007500: 2020 2020 2020 2069 6620 636f 6d6d 616e         if comman
+00007510: 645f 636f 6465 206e 6f74 2069 6e20 6c69  d_code not in li
+00007520: 622e 5374 6174 7573 5175 6572 7943 6f64  b.StatusQueryCod
+00007530: 652e 5f6d 656d 6265 725f 6e61 6d65 735f  e._member_names_
+00007540: 3a0d 0a20 2020 2020 2020 2020 2020 2069  :..            i
+00007550: 6620 6765 745f 706f 7369 7469 6f6e 3a0d  f get_position:.
+00007560: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00007570: 2073 656c 662e 6765 7450 6f73 6974 696f   self.getPositio
+00007580: 6e28 290d 0a20 2020 2020 2020 2020 2020  n()..           
+00007590: 2069 6620 7265 7375 6d65 5f66 6565 6462   if resume_feedb
+000075a0: 6163 6b3a 0d0a 2020 2020 2020 2020 2020  ack:..          
+000075b0: 2020 2020 2020 7365 6c66 2e73 6574 466c        self.setFl
+000075c0: 6167 2870 6175 7365 5f66 6565 6462 6163  ag(pause_feedbac
+000075d0: 6b3d 4661 6c73 6529 0d0a 2020 2020 2020  k=False)..      
+000075e0: 2020 7265 7475 726e 2072 6573 706f 6e73    return respons
+000075f0: 650d 0a0d 0a20 2020 2064 6566 205f 7265  e....    def _re
+00007600: 6164 2873 656c 6629 202d 3e20 7374 723a  ad(self) -> str:
+00007610: 0d0a 2020 2020 2020 2020 2222 220d 0a20  ..        """.. 
+00007620: 2020 2020 2020 2052 6561 6420 7265 7370         Read resp
+00007630: 6f6e 7365 2066 726f 6d20 6465 7669 6365  onse from device
+00007640: 0d0a 0d0a 2020 2020 2020 2020 5265 7475  ....        Retu
+00007650: 726e 733a 0d0a 2020 2020 2020 2020 2020  rns:..          
+00007660: 2020 7374 723a 2072 6573 706f 6e73 6520    str: response 
+00007670: 7374 7269 6e67 0d0a 2020 2020 2020 2020  string..        
+00007680: 2222 220d 0a20 2020 2020 2020 2072 6573  """..        res
+00007690: 706f 6e73 6520 3d20 2727 0d0a 2020 2020  ponse = ''..    
+000076a0: 2020 2020 7472 793a 0d0a 2020 2020 2020      try:..      
+000076b0: 2020 2020 2020 7265 7370 6f6e 7365 203d        response =
+000076c0: 2073 656c 662e 6465 7669 6365 2e72 6561   self.device.rea
+000076d0: 646c 696e 6528 290d 0a20 2020 2020 2020  dline()..       
+000076e0: 2020 2020 2069 6620 6c65 6e28 7265 7370       if len(resp
+000076f0: 6f6e 7365 2920 3d3d 2030 3a0d 0a20 2020  onse) == 0:..   
+00007700: 2020 2020 2020 2020 2020 2020 2072 6573               res
+00007710: 706f 6e73 6520 3d20 7365 6c66 2e64 6576  ponse = self.dev
+00007720: 6963 652e 7265 6164 6c69 6e65 2829 0d0a  ice.readline()..
+00007730: 2020 2020 2020 2020 2020 2020 7265 7370              resp
+00007740: 6f6e 7365 203d 2072 6573 706f 6e73 655b  onse = response[
+00007750: 323a 2d32 5d2e 6465 636f 6465 2827 7574  2:-2].decode('ut
+00007760: 662d 3827 290d 0a20 2020 2020 2020 2065  f-8')..        e
+00007770: 7863 6570 7420 4174 7472 6962 7574 6545  xcept AttributeE
+00007780: 7272 6f72 3a0d 0a20 2020 2020 2020 2020  rror:..         
+00007790: 2020 2070 6173 730d 0a20 2020 2020 2020     pass..       
+000077a0: 2065 7863 6570 7420 4578 6365 7074 696f   except Exceptio
+000077b0: 6e20 6173 2065 3a0d 0a20 2020 2020 2020  n as e:..       
+000077c0: 2020 2020 2069 6620 7365 6c66 2e76 6572       if self.ver
+000077d0: 626f 7365 3a0d 0a20 2020 2020 2020 2020  bose:..         
+000077e0: 2020 2020 2020 2070 7269 6e74 2865 290d         print(e).
+000077f0: 0a20 2020 2020 2020 2069 6620 7265 7370  .        if resp
+00007800: 6f6e 7365 2069 6e20 6c69 622e 4572 726f  onse in lib.Erro
+00007810: 7243 6f64 652e 5f6d 656d 6265 725f 6e61  rCode._member_na
+00007820: 6d65 735f 3a0d 0a20 2020 2020 2020 2020  mes_:..         
+00007830: 2020 2070 7269 6e74 286c 6962 2e45 7272     print(lib.Err
+00007840: 6f72 436f 6465 5b72 6573 706f 6e73 655d  orCode[response]
+00007850: 2e76 616c 7565 290d 0a20 2020 2020 2020  .value)..       
+00007860: 2072 6574 7572 6e20 7265 7370 6f6e 7365   return response
+00007870: 0d0a 2020 2020 0d0a 2020 2020 6465 6620  ..    ..    def 
+00007880: 5f73 6574 5f63 6861 6e6e 656c 5f69 6428  _set_channel_id(
+00007890: 7365 6c66 2c20 6e65 775f 6368 616e 6e65  self, new_channe
+000078a0: 6c5f 6964 3a69 6e74 293a 0d0a 2020 2020  l_id:int):..    
+000078b0: 2020 2020 2222 220d 0a20 2020 2020 2020      """..       
+000078c0: 2053 6574 2063 6861 6e6e 656c 2069 6420   Set channel id 
+000078d0: 6f66 2064 6576 6963 650d 0a0d 0a20 2020  of device....   
+000078e0: 2020 2020 2041 7267 733a 0d0a 2020 2020       Args:..    
+000078f0: 2020 2020 2020 2020 6e65 775f 6368 616e          new_chan
+00007900: 6e65 6c20 2869 6e74 293a 206e 6577 2063  nel (int): new c
+00007910: 6861 6e6e 656c 2069 640d 0a0d 0a20 2020  hannel id....   
+00007920: 2020 2020 2052 6169 7365 733a 0d0a 2020       Raises:..  
+00007930: 2020 2020 2020 2020 2020 5661 6c75 6545            ValueE
+00007940: 7272 6f72 3a20 506c 6561 7365 2073 656c  rror: Please sel
+00007950: 6563 7420 6120 7661 6c69 6420 724c 696e  ect a valid rLin
+00007960: 6520 6164 6472 6573 7320 6672 6f6d 2031  e address from 1
+00007970: 2074 6f20 390d 0a20 2020 2020 2020 2022   to 9..        "
+00007980: 2222 0d0a 2020 2020 2020 2020 6966 206e  ""..        if n
+00007990: 6f74 2028 3020 3c20 6e65 775f 6368 616e  ot (0 < new_chan
+000079a0: 6e65 6c5f 6964 203c 2031 3029 3a0d 0a20  nel_id < 10):.. 
+000079b0: 2020 2020 2020 2020 2020 2072 6169 7365             raise
+000079c0: 2056 616c 7565 4572 726f 7228 2750 6c65   ValueError('Ple
+000079d0: 6173 6520 7365 6c65 6374 2061 2076 616c  ase select a val
+000079e0: 6964 2072 4c69 6e65 2061 6464 7265 7373  id rLine address
+000079f0: 2066 726f 6d20 3120 746f 2039 2e27 290d   from 1 to 9.').
+00007a00: 0a20 2020 2020 2020 2072 6573 706f 6e73  .        respons
+00007a10: 6520 3d20 7365 6c66 2e5f 7175 6572 7928  e = self._query(
+00007a20: 6627 2a41 7b6e 6577 5f63 6861 6e6e 656c  f'*A{new_channel
+00007a30: 5f69 647d 2729 0d0a 2020 2020 2020 2020  _id}')..        
+00007a40: 6966 2072 6573 706f 6e73 6520 3d3d 2027  if response == '
+00007a50: 6f6b 273a 0d0a 2020 2020 2020 2020 2020  ok':..          
+00007a60: 2020 7365 6c66 2e63 6861 6e6e 656c 203d    self.channel =
+00007a70: 206e 6577 5f63 6861 6e6e 656c 5f69 640d   new_channel_id.
+00007a80: 0a20 2020 2020 2020 2072 6574 7572 6e0d  .        return.
+00007a90: 0a20 2020 200d 0a20 2020 2064 6566 205f  .    ..    def _
+00007aa0: 7772 6974 6528 7365 6c66 2c20 636f 6d6d  write(self, comm
+00007ab0: 616e 643a 7374 7229 202d 3e20 626f 6f6c  and:str) -> bool
+00007ac0: 3a0d 0a20 2020 2020 2020 2022 2222 0d0a  :..        """..
+00007ad0: 2020 2020 2020 2020 5772 6974 6520 636f          Write co
+00007ae0: 6d6d 616e 6420 746f 2064 6576 6963 650d  mmand to device.
+00007af0: 0a0d 0a20 2020 2020 2020 2041 7267 733a  ...        Args:
+00007b00: 0d0a 2020 2020 2020 2020 2020 2020 636f  ..            co
+00007b10: 6d6d 616e 6420 2873 7472 293a 203c 636f  mmand (str): <co
+00007b20: 6d6d 616e 6420 636f 6465 3e3c 7661 6c75  mmand code><valu
+00007b30: 653e 0d0a 0d0a 2020 2020 2020 2020 5265  e>....        Re
+00007b40: 7475 726e 733a 0d0a 2020 2020 2020 2020  turns:..        
+00007b50: 2020 2020 626f 6f6c 3a20 7768 6574 6865      bool: whethe
+00007b60: 7220 636f 6d6d 616e 6420 7761 7320 7365  r command was se
+00007b70: 6e74 2073 7563 6365 7373 6675 6c6c 790d  nt successfully.
+00007b80: 0a20 2020 2020 2020 2022 2222 0d0a 2020  .        """..  
+00007b90: 2020 2020 2020 6673 7472 696e 6720 3d20        fstring = 
+00007ba0: 6627 017b 7365 6c66 2e63 6861 6e6e 656c  f'.{self.channel
+00007bb0: 7d7b 636f 6d6d 616e 647d c2ba 5c72 2720  }{command}..\r' 
+00007bc0: 2320 636f 6d6d 616e 6420 7465 6d70 6c61  # command templa
+00007bd0: 7465 3a20 3c50 5245 3e3c 4144 523e 3c43  te: <PRE><ADR><C
+00007be0: 4f44 453e 3c44 4154 413e 3c4c 5243 3e3c  ODE><DATA><LRC><
+00007bf0: 504f 5354 3e0d 0a20 2020 2020 2020 2023  POST>..        #
+00007c00: 2062 7374 7269 6e67 203d 2062 7974 6561   bstring = bytea
+00007c10: 7272 6179 2e66 726f 6d68 6578 2866 7374  rray.fromhex(fst
+00007c20: 7269 6e67 2e65 6e63 6f64 6528 2775 7466  ring.encode('utf
+00007c30: 2d38 2729 2e68 6578 2829 290d 0a20 2020  -8').hex())..   
+00007c40: 2020 2020 2069 6620 7365 6c66 2e76 6572       if self.ver
+00007c50: 626f 7365 3a0d 0a20 2020 2020 2020 2020  bose:..         
+00007c60: 2020 2070 7269 6e74 2866 7374 7269 6e67     print(fstring
+00007c70: 290d 0a20 2020 2020 2020 2074 7279 3a0d  )..        try:.
+00007c80: 0a20 2020 2020 2020 2020 2020 2023 2054  .            # T
+00007c90: 7970 6963 616c 2074 696d 656f 7574 2077  ypical timeout w
+00007ca0: 6169 7420 6973 2034 3030 6d73 0d0a 2020  ait is 400ms..  
+00007cb0: 2020 2020 2020 2020 2020 7365 6c66 2e64            self.d
+00007cc0: 6576 6963 652e 7772 6974 6528 6673 7472  evice.write(fstr
+00007cd0: 696e 672e 656e 636f 6465 2827 7574 662d  ing.encode('utf-
+00007ce0: 3827 2929 0d0a 2020 2020 2020 2020 6578  8'))..        ex
+00007cf0: 6365 7074 2041 7474 7269 6275 7465 4572  cept AttributeEr
+00007d00: 726f 723a 0d0a 2020 2020 2020 2020 2020  ror:..          
+00007d10: 2020 7061 7373 0d0a 2020 2020 2020 2020    pass..        
+00007d20: 6578 6365 7074 2045 7863 6570 7469 6f6e  except Exception
+00007d30: 2061 7320 653a 0d0a 2020 2020 2020 2020   as e:..        
+00007d40: 2020 2020 6966 2073 656c 662e 7665 7262      if self.verb
+00007d50: 6f73 653a 0d0a 2020 2020 2020 2020 2020  ose:..          
+00007d60: 2020 2020 2020 7072 696e 7428 6529 0d0a        print(e)..
+00007d70: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00007d80: 726e 2046 616c 7365 0d0a 2020 2020 2020  rn False..      
+00007d90: 2020 7265 7475 726e 2054 7275 650d 0a20    return True.. 
+00007da0: 2020 20
```

### Comparing `control-lab-ly-1.1.0b1/src/controllably/Transfer/Liquid/liquid_utils.py` & `control-lab-ly-1.1.1a1/src/controllably/Transfer/Liquid/liquid_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.0b1/src/controllably/Transfer/Liquid/syringe_lib.py` & `control-lab-ly-1.1.1a1/src/controllably/Transfer/Liquid/syringe_lib.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.0b1/src/controllably/Transfer/Liquid/syringe_utils.py` & `control-lab-ly-1.1.1a1/src/controllably/Transfer/Liquid/syringe_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.0b1/src/controllably/Transfer/Substrate/Dobot/dobot_attachments.py` & `control-lab-ly-1.1.1a1/src/controllably/Transfer/Substrate/Dobot/dobot_attachments.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.0b1/src/controllably/Transfer/Substrate/substrate_utils.py` & `control-lab-ly-1.1.1a1/src/controllably/Transfer/Substrate/substrate_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.0b1/src/controllably/View/Classifiers/classifier_utils.py` & `control-lab-ly-1.1.1a1/src/controllably/View/Classifiers/classifier_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.0b1/src/controllably/View/Optical/optical_utils.py` & `control-lab-ly-1.1.1a1/src/controllably/View/Optical/optical_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.0b1/src/controllably/View/Optical/placeholders/optical_camera.png` & `control-lab-ly-1.1.1a1/src/controllably/View/Optical/placeholders/optical_camera.png`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.0b1/src/controllably/View/Thermal/Flir/ax8/ax8.py` & `control-lab-ly-1.1.1a1/src/controllably/View/Thermal/Flir/ax8/ax8.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.0b1/src/controllably/View/Thermal/Flir/ax8/ax8_camera_feed.py` & `control-lab-ly-1.1.1a1/src/controllably/View/Thermal/Flir/ax8/ax8_camera_feed.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.0b1/src/controllably/View/Thermal/Flir/ax8/ax8_modbus_regs.py` & `control-lab-ly-1.1.1a1/src/controllably/View/Thermal/Flir/ax8/ax8_modbus_regs.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.0b1/src/controllably/View/Thermal/Flir/ax8/ax8_modbus_utils.py` & `control-lab-ly-1.1.1a1/src/controllably/View/Thermal/Flir/ax8/ax8_modbus_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.0b1/src/controllably/View/Thermal/placeholders/infrared_camera.png` & `control-lab-ly-1.1.1a1/src/controllably/View/Thermal/placeholders/infrared_camera.png`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.0b1/src/controllably/View/Thermal/thermal_utils.py` & `control-lab-ly-1.1.1a1/src/controllably/View/Thermal/thermal_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.0b1/src/controllably/View/image.py` & `control-lab-ly-1.1.1a1/src/controllably/View/image.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.0b1/src/controllably/View/view_utils.py` & `control-lab-ly-1.1.1a1/src/controllably/View/view_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.0b1/src/controllably/misc/__init__.py` & `control-lab-ly-1.1.1a1/src/controllably/misc/__init__.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.0b1/src/controllably/misc/decorators.py` & `control-lab-ly-1.1.1a1/src/controllably/misc/decorators.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.0b1/src/controllably/misc/factory.py` & `control-lab-ly-1.1.1a1/src/controllably/misc/factory.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.0b1/src/controllably/misc/helper.py` & `control-lab-ly-1.1.1a1/src/controllably/misc/helper.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.0b1/src/controllably/misc/layout.py` & `control-lab-ly-1.1.1a1/src/controllably/misc/layout.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.0b1/src/controllably/misc/logger.py` & `control-lab-ly-1.1.1a1/src/controllably/misc/logger.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.0b1/src/controllably/misc/misc_utils.py` & `control-lab-ly-1.1.1a1/src/controllably/misc/misc_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.0b1/src/controllably/misc/templates/configs/plugins/plugin_template.py` & `control-lab-ly-1.1.1a1/src/controllably/misc/templates/configs/plugins/plugin_template.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.0b1/src/controllably/misc/templates/setup/__init__.py` & `control-lab-ly-1.1.1a1/src/controllably/misc/templates/setup/__init__.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.0b1/src/controllably/misc/templates/setup/config.yaml` & `control-lab-ly-1.1.1a1/src/controllably/misc/templates/setup/config.yaml`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.0b1/src/controllably/misc/templates/setup/layout.json` & `control-lab-ly-1.1.1a1/src/controllably/misc/templates/setup/layout.json`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.0b1/tests/test_panels.py` & `control-lab-ly-1.1.1a1/tests/test_panels.py`

 * *Files identical despite different names*

