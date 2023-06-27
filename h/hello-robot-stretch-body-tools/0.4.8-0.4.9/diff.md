# Comparing `tmp/hello_robot_stretch_body_tools-0.4.8.tar.gz` & `tmp/hello_robot_stretch_body_tools-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hello_robot_stretch_body_tools-0.4.8.tar", last modified: Thu Feb  9 19:33:24 2023, max compression
+gzip compressed data, was "hello_robot_stretch_body_tools-0.4.9.tar", last modified: Tue Feb 14 00:40:45 2023, max compression
```

## Comparing `hello_robot_stretch_body_tools-0.4.8.tar` & `hello_robot_stretch_body_tools-0.4.9.tar`

### file list

```diff
@@ -1,50 +1,49 @@
-drwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)        0 2023-02-09 19:33:24.253929 hello_robot_stretch_body_tools-0.4.8/
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)      921 2022-09-08 01:07:04.000000 hello_robot_stretch_body_tools-0.4.8/LICENSE.md
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     2885 2023-02-09 19:33:24.253929 hello_robot_stretch_body_tools-0.4.8/PKG-INFO
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     2405 2023-02-06 19:05:11.000000 hello_robot_stretch_body_tools-0.4.8/README.md
-drwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)        0 2023-02-09 19:33:24.253929 hello_robot_stretch_body_tools-0.4.8/bin/
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     2338 2022-09-28 01:56:48.000000 hello_robot_stretch_body_tools-0.4.8/bin/stretch_about.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)      789 2022-09-28 01:56:48.000000 hello_robot_stretch_body_tools-0.4.8/bin/stretch_about_text.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)      365 2022-09-28 01:56:48.000000 hello_robot_stretch_body_tools-0.4.8/bin/stretch_arm_home.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     3239 2022-09-28 01:56:48.000000 hello_robot_stretch_body_tools-0.4.8/bin/stretch_arm_jog.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)      483 2022-09-28 01:56:48.000000 hello_robot_stretch_body_tools-0.4.8/bin/stretch_audio_test.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     6250 2022-09-08 01:07:04.000000 hello_robot_stretch_body_tools-0.4.8/bin/stretch_base_jog.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)      438 2022-09-08 01:07:04.000000 hello_robot_stretch_body_tools-0.4.8/bin/stretch_gripper_home.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     2603 2022-09-08 01:07:04.000000 hello_robot_stretch_body_tools-0.4.8/bin/stretch_gripper_jog.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     4383 2022-09-28 01:56:48.000000 hello_robot_stretch_body_tools-0.4.8/bin/stretch_hardware_echo.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     3997 2022-09-08 01:07:04.000000 hello_robot_stretch_body_tools-0.4.8/bin/stretch_head_jog.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)      384 2022-09-08 01:07:04.000000 hello_robot_stretch_body_tools-0.4.8/bin/stretch_lift_home.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     3244 2022-09-28 01:56:48.000000 hello_robot_stretch_body_tools-0.4.8/bin/stretch_lift_jog.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     1685 2022-09-28 01:56:48.000000 hello_robot_stretch_body_tools-0.4.8/bin/stretch_params.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     1964 2022-09-08 01:07:04.000000 hello_robot_stretch_body_tools-0.4.8/bin/stretch_pimu_jog.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     8676 2022-09-08 01:07:04.000000 hello_robot_stretch_body_tools-0.4.8/bin/stretch_pimu_scope.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)    15624 2022-09-08 01:07:04.000000 hello_robot_stretch_body_tools-0.4.8/bin/stretch_realsense_visualizer.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)    11373 2022-09-28 01:56:48.000000 hello_robot_stretch_body_tools-0.4.8/bin/stretch_respeaker_test.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)      996 2022-09-08 01:07:04.000000 hello_robot_stretch_body_tools-0.4.8/bin/stretch_robot_battery_check.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)      719 2022-09-08 01:07:04.000000 hello_robot_stretch_body_tools-0.4.8/bin/stretch_robot_dynamixel_reboot.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)      429 2022-09-08 01:07:04.000000 hello_robot_stretch_body_tools-0.4.8/bin/stretch_robot_home.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)      739 2022-09-08 01:07:04.000000 hello_robot_stretch_body_tools-0.4.8/bin/stretch_robot_jog.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     4425 2022-09-08 01:07:04.000000 hello_robot_stretch_body_tools-0.4.8/bin/stretch_robot_keyboard_teleop.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)      513 2022-09-08 01:07:04.000000 hello_robot_stretch_body_tools-0.4.8/bin/stretch_robot_monitor.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)      447 2022-09-28 01:56:48.000000 hello_robot_stretch_body_tools-0.4.8/bin/stretch_robot_stow.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     6060 2023-02-06 21:55:26.000000 hello_robot_stretch_body_tools-0.4.8/bin/stretch_robot_system_check.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     7943 2022-09-28 01:56:48.000000 hello_robot_stretch_body_tools-0.4.8/bin/stretch_robot_urdf_visualizer.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     1514 2023-01-16 20:45:15.000000 hello_robot_stretch_body_tools-0.4.8/bin/stretch_rp_lidar_jog.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)    17566 2022-09-28 01:56:48.000000 hello_robot_stretch_body_tools-0.4.8/bin/stretch_trajectory_jog.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     1874 2023-02-09 19:32:18.000000 hello_robot_stretch_body_tools-0.4.8/bin/stretch_version.sh
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     1335 2022-09-08 01:07:04.000000 hello_robot_stretch_body_tools-0.4.8/bin/stretch_wacc_jog.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     2881 2022-09-08 01:07:04.000000 hello_robot_stretch_body_tools-0.4.8/bin/stretch_wacc_scope.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)      403 2022-09-08 01:07:04.000000 hello_robot_stretch_body_tools-0.4.8/bin/stretch_wrist_yaw_home.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     2445 2022-09-08 01:07:04.000000 hello_robot_stretch_body_tools-0.4.8/bin/stretch_wrist_yaw_jog.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)    20929 2023-01-16 20:45:15.000000 hello_robot_stretch_body_tools-0.4.8/bin/stretch_xbox_controller_teleop.py
-drwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)        0 2023-02-09 19:33:24.253929 hello_robot_stretch_body_tools-0.4.8/hello_robot_stretch_body_tools.egg-info/
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     2885 2023-02-09 19:33:24.000000 hello_robot_stretch_body_tools-0.4.8/hello_robot_stretch_body_tools.egg-info/PKG-INFO
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     1363 2023-02-09 19:33:24.000000 hello_robot_stretch_body_tools-0.4.8/hello_robot_stretch_body_tools.egg-info/SOURCES.txt
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)        1 2023-02-09 19:33:24.000000 hello_robot_stretch_body_tools-0.4.8/hello_robot_stretch_body_tools.egg-info/dependency_links.txt
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)      309 2023-02-09 19:33:24.000000 hello_robot_stretch_body_tools-0.4.8/hello_robot_stretch_body_tools.egg-info/requires.txt
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)        5 2023-02-09 19:33:24.000000 hello_robot_stretch_body_tools-0.4.8/hello_robot_stretch_body_tools.egg-info/top_level.txt
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)       38 2023-02-09 19:33:24.253929 hello_robot_stretch_body_tools-0.4.8/setup.cfg
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     1604 2023-02-09 19:32:28.000000 hello_robot_stretch_body_tools-0.4.8/setup.py
-drwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)        0 2023-02-09 19:33:24.253929 hello_robot_stretch_body_tools-0.4.8/test/
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)       34 2022-09-08 01:07:04.000000 hello_robot_stretch_body_tools-0.4.8/test/__init__.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     2173 2022-09-08 01:07:04.000000 hello_robot_stretch_body_tools-0.4.8/test/test_tools_launch.py
+drwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)        0 2023-02-14 00:40:45.551651 hello_robot_stretch_body_tools-0.4.9/
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     3311 2023-02-14 00:40:45.551651 hello_robot_stretch_body_tools-0.4.9/PKG-INFO
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     2405 2023-02-14 00:39:41.000000 hello_robot_stretch_body_tools-0.4.9/README.md
+drwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)        0 2023-02-14 00:40:45.547651 hello_robot_stretch_body_tools-0.4.9/bin/
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     2338 2023-02-14 00:39:41.000000 hello_robot_stretch_body_tools-0.4.9/bin/stretch_about.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)      789 2023-02-14 00:39:41.000000 hello_robot_stretch_body_tools-0.4.9/bin/stretch_about_text.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)      365 2023-02-14 00:39:41.000000 hello_robot_stretch_body_tools-0.4.9/bin/stretch_arm_home.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     3239 2023-02-14 00:39:41.000000 hello_robot_stretch_body_tools-0.4.9/bin/stretch_arm_jog.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)      483 2023-02-14 00:39:41.000000 hello_robot_stretch_body_tools-0.4.9/bin/stretch_audio_test.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     6250 2023-02-14 00:39:41.000000 hello_robot_stretch_body_tools-0.4.9/bin/stretch_base_jog.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)      438 2023-02-14 00:39:41.000000 hello_robot_stretch_body_tools-0.4.9/bin/stretch_gripper_home.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     2603 2023-02-14 00:39:41.000000 hello_robot_stretch_body_tools-0.4.9/bin/stretch_gripper_jog.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     4383 2023-02-14 00:39:41.000000 hello_robot_stretch_body_tools-0.4.9/bin/stretch_hardware_echo.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     3997 2023-02-14 00:39:41.000000 hello_robot_stretch_body_tools-0.4.9/bin/stretch_head_jog.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)      384 2023-02-14 00:39:41.000000 hello_robot_stretch_body_tools-0.4.9/bin/stretch_lift_home.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     3244 2023-02-14 00:39:41.000000 hello_robot_stretch_body_tools-0.4.9/bin/stretch_lift_jog.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     1685 2023-02-14 00:39:41.000000 hello_robot_stretch_body_tools-0.4.9/bin/stretch_params.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     1964 2023-02-14 00:39:41.000000 hello_robot_stretch_body_tools-0.4.9/bin/stretch_pimu_jog.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     8676 2023-02-14 00:39:41.000000 hello_robot_stretch_body_tools-0.4.9/bin/stretch_pimu_scope.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)    15624 2023-02-14 00:39:41.000000 hello_robot_stretch_body_tools-0.4.9/bin/stretch_realsense_visualizer.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)    11373 2023-02-14 00:39:41.000000 hello_robot_stretch_body_tools-0.4.9/bin/stretch_respeaker_test.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)      996 2023-02-14 00:39:41.000000 hello_robot_stretch_body_tools-0.4.9/bin/stretch_robot_battery_check.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)      719 2023-02-14 00:39:41.000000 hello_robot_stretch_body_tools-0.4.9/bin/stretch_robot_dynamixel_reboot.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)      429 2023-02-14 00:39:41.000000 hello_robot_stretch_body_tools-0.4.9/bin/stretch_robot_home.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)      739 2023-02-14 00:39:41.000000 hello_robot_stretch_body_tools-0.4.9/bin/stretch_robot_jog.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     4425 2023-02-14 00:39:41.000000 hello_robot_stretch_body_tools-0.4.9/bin/stretch_robot_keyboard_teleop.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)      513 2023-02-14 00:39:41.000000 hello_robot_stretch_body_tools-0.4.9/bin/stretch_robot_monitor.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)      447 2023-02-14 00:39:41.000000 hello_robot_stretch_body_tools-0.4.9/bin/stretch_robot_stow.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     6609 2023-02-14 00:39:41.000000 hello_robot_stretch_body_tools-0.4.9/bin/stretch_robot_system_check.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     7943 2023-02-14 00:39:41.000000 hello_robot_stretch_body_tools-0.4.9/bin/stretch_robot_urdf_visualizer.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     1514 2023-02-14 00:39:41.000000 hello_robot_stretch_body_tools-0.4.9/bin/stretch_rp_lidar_jog.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)    17566 2023-02-14 00:39:41.000000 hello_robot_stretch_body_tools-0.4.9/bin/stretch_trajectory_jog.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     1874 2023-02-14 00:39:41.000000 hello_robot_stretch_body_tools-0.4.9/bin/stretch_version.sh
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     1335 2023-02-14 00:39:41.000000 hello_robot_stretch_body_tools-0.4.9/bin/stretch_wacc_jog.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     2881 2023-02-14 00:39:41.000000 hello_robot_stretch_body_tools-0.4.9/bin/stretch_wacc_scope.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)      403 2023-02-14 00:39:41.000000 hello_robot_stretch_body_tools-0.4.9/bin/stretch_wrist_yaw_home.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     2445 2023-02-14 00:39:41.000000 hello_robot_stretch_body_tools-0.4.9/bin/stretch_wrist_yaw_jog.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)    20929 2023-02-14 00:39:41.000000 hello_robot_stretch_body_tools-0.4.9/bin/stretch_xbox_controller_teleop.py
+drwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)        0 2023-02-14 00:40:45.551651 hello_robot_stretch_body_tools-0.4.9/hello_robot_stretch_body_tools.egg-info/
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     3311 2023-02-14 00:40:45.000000 hello_robot_stretch_body_tools-0.4.9/hello_robot_stretch_body_tools.egg-info/PKG-INFO
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     1352 2023-02-14 00:40:45.000000 hello_robot_stretch_body_tools-0.4.9/hello_robot_stretch_body_tools.egg-info/SOURCES.txt
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)        1 2023-02-14 00:40:45.000000 hello_robot_stretch_body_tools-0.4.9/hello_robot_stretch_body_tools.egg-info/dependency_links.txt
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)      309 2023-02-14 00:40:45.000000 hello_robot_stretch_body_tools-0.4.9/hello_robot_stretch_body_tools.egg-info/requires.txt
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)        5 2023-02-14 00:40:45.000000 hello_robot_stretch_body_tools-0.4.9/hello_robot_stretch_body_tools.egg-info/top_level.txt
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)       38 2023-02-14 00:40:45.551651 hello_robot_stretch_body_tools-0.4.9/setup.cfg
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     1604 2023-02-14 00:40:13.000000 hello_robot_stretch_body_tools-0.4.9/setup.py
+drwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)        0 2023-02-14 00:40:45.551651 hello_robot_stretch_body_tools-0.4.9/test/
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)       34 2023-02-14 00:39:41.000000 hello_robot_stretch_body_tools-0.4.9/test/__init__.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     2173 2023-02-14 00:39:41.000000 hello_robot_stretch_body_tools-0.4.9/test/test_tools_launch.py
```

### Comparing `hello_robot_stretch_body_tools-0.4.8/PKG-INFO` & `hello_robot_stretch_body_tools-0.4.9/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: hello_robot_stretch_body_tools
-Version: 0.4.8
-Summary: Stretch Body Tools
-Home-page: https://github.com/hello-robot/stretch_body
-Author: Hello Robot Inc
-Author-email: support@hello-robot.com
-License: UNKNOWN
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: OS Independent
-Classifier: License :: OSI Approved :: Apache Software License
-Description-Content-Type: text/markdown
-License-File: LICENSE.md
-
 Stretch Body Command Line Tools
 ===============================
 
 This package provides Python tools that work with the Hello Robot Stretch Body package. These tools perform common tasks when working with Stretch (e.g. homing and stowing), and serve as tutorial code for working on various parts of the robot. This package comes pre-installed on Stretch robots. A tutorial for using this package can be found [on the docs](https://docs.hello-robot.com/0.2/stretch-tutorials/stretch_body/tutorial_command_line_tools/).
 
 Installing
 ----------
@@ -64,9 +49,7 @@
 
 Now, make desired edits to the [stretch_robot_home.py](./bin/stretch_robot_home.py) file. Executing the script on the command-line will now run your modified version.
 
 Deploying
 ---------
 
 Increment the version number and run the `deploy.sh` script. Verify the new release is reflected [on PyPI](https://pypi.org/project/hello-robot-stretch-body-tools/).
-
-
```

### Comparing `hello_robot_stretch_body_tools-0.4.8/README.md` & `hello_robot_stretch_body_tools-0.4.9/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,55 +1,69 @@
-Stretch Body Command Line Tools
-===============================
-
-This package provides Python tools that work with the Hello Robot Stretch Body package. These tools perform common tasks when working with Stretch (e.g. homing and stowing), and serve as tutorial code for working on various parts of the robot. This package comes pre-installed on Stretch robots. A tutorial for using this package can be found [on the docs](https://docs.hello-robot.com/0.2/stretch-tutorials/stretch_body/tutorial_command_line_tools/).
-
-Installing
-----------
-
-This package comes pre-installed on Stretch robots. To install or upgrade to a stable Stretch Body Command Line Tools for Python3, run:
-
-```bash
-$ python3 -m pip install --upgrade hello-robot-stretch-body-tools
-```
-
-To install or upgrade to a pre-release of the Command Line Tools for Python3, run:
-
-```bash
-$ python3 -m pip install --upgrade --pre hello-robot-stretch-body-tools
-```
-
-Please report feedback on the [Issue Tracker](https://github.com/hello-robot/stretch_body/issues) or the [Forum](https://forum.hello-robot.com/).
-
-Usage
------
-
-All of the command-line tools reside within the `bin/` folder. When this package is installed, they are accessible from anywhere as command-line tools. For example, to perform a robot system check, run:
-
-```bash
-$ stretch_robot_system_check.py
-```
-
-For more info on these tools, see the [tutorial](https://docs.hello-robot.com/0.2/stretch-tutorials/stretch_body/tutorial_command_line_tools/).
-
-Developing
-----------
-
-The source code for the command-line tools resides within the `bin/` folder. You can install the tools package as "editable", and directly edit the source code to test changes.
-
-In Python3, run `python3 -m pip install -e .`
-
-For example, to test changes to the  `stretch_robot_home.py` script, run
-
-```bash
-$ python3 -m pip uninstall hello-robot-stretch-body-tools # ensure previous Stretch Body Tools installations are removed
-$ git clone https://github.com/hello-robot/stretch_body.git
-$ cd stretch_body/tools
-$ python3 -m pip install -e .
-```
-
-Now, make desired edits to the [stretch_robot_home.py](./bin/stretch_robot_home.py) file. Executing the script on the command-line will now run your modified version.
-
-Deploying
----------
-
-Increment the version number and run the `deploy.sh` script. Verify the new release is reflected [on PyPI](https://pypi.org/project/hello-robot-stretch-body-tools/).
+Metadata-Version: 2.1
+Name: hello_robot_stretch_body_tools
+Version: 0.4.9
+Summary: Stretch Body Tools
+Home-page: https://github.com/hello-robot/stretch_body
+Author: Hello Robot Inc
+Author-email: support@hello-robot.com
+License: UNKNOWN
+Description: Stretch Body Command Line Tools
+        ===============================
+        
+        This package provides Python tools that work with the Hello Robot Stretch Body package. These tools perform common tasks when working with Stretch (e.g. homing and stowing), and serve as tutorial code for working on various parts of the robot. This package comes pre-installed on Stretch robots. A tutorial for using this package can be found [on the docs](https://docs.hello-robot.com/0.2/stretch-tutorials/stretch_body/tutorial_command_line_tools/).
+        
+        Installing
+        ----------
+        
+        This package comes pre-installed on Stretch robots. To install or upgrade to a stable Stretch Body Command Line Tools for Python3, run:
+        
+        ```bash
+        $ python3 -m pip install --upgrade hello-robot-stretch-body-tools
+        ```
+        
+        To install or upgrade to a pre-release of the Command Line Tools for Python3, run:
+        
+        ```bash
+        $ python3 -m pip install --upgrade --pre hello-robot-stretch-body-tools
+        ```
+        
+        Please report feedback on the [Issue Tracker](https://github.com/hello-robot/stretch_body/issues) or the [Forum](https://forum.hello-robot.com/).
+        
+        Usage
+        -----
+        
+        All of the command-line tools reside within the `bin/` folder. When this package is installed, they are accessible from anywhere as command-line tools. For example, to perform a robot system check, run:
+        
+        ```bash
+        $ stretch_robot_system_check.py
+        ```
+        
+        For more info on these tools, see the [tutorial](https://docs.hello-robot.com/0.2/stretch-tutorials/stretch_body/tutorial_command_line_tools/).
+        
+        Developing
+        ----------
+        
+        The source code for the command-line tools resides within the `bin/` folder. You can install the tools package as "editable", and directly edit the source code to test changes.
+        
+        In Python3, run `python3 -m pip install -e .`
+        
+        For example, to test changes to the  `stretch_robot_home.py` script, run
+        
+        ```bash
+        $ python3 -m pip uninstall hello-robot-stretch-body-tools # ensure previous Stretch Body Tools installations are removed
+        $ git clone https://github.com/hello-robot/stretch_body.git
+        $ cd stretch_body/tools
+        $ python3 -m pip install -e .
+        ```
+        
+        Now, make desired edits to the [stretch_robot_home.py](./bin/stretch_robot_home.py) file. Executing the script on the command-line will now run your modified version.
+        
+        Deploying
+        ---------
+        
+        Increment the version number and run the `deploy.sh` script. Verify the new release is reflected [on PyPI](https://pypi.org/project/hello-robot-stretch-body-tools/).
+        
+Platform: UNKNOWN
+Classifier: Programming Language :: Python :: 3
+Classifier: Operating System :: OS Independent
+Classifier: License :: OSI Approved :: Apache Software License
+Description-Content-Type: text/markdown
```

### Comparing `hello_robot_stretch_body_tools-0.4.8/bin/stretch_about.py` & `hello_robot_stretch_body_tools-0.4.9/bin/stretch_about.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body_tools-0.4.8/bin/stretch_about_text.py` & `hello_robot_stretch_body_tools-0.4.9/bin/stretch_about_text.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body_tools-0.4.8/bin/stretch_arm_jog.py` & `hello_robot_stretch_body_tools-0.4.9/bin/stretch_arm_jog.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body_tools-0.4.8/bin/stretch_base_jog.py` & `hello_robot_stretch_body_tools-0.4.9/bin/stretch_base_jog.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body_tools-0.4.8/bin/stretch_gripper_jog.py` & `hello_robot_stretch_body_tools-0.4.9/bin/stretch_gripper_jog.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body_tools-0.4.8/bin/stretch_hardware_echo.py` & `hello_robot_stretch_body_tools-0.4.9/bin/stretch_hardware_echo.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body_tools-0.4.8/bin/stretch_head_jog.py` & `hello_robot_stretch_body_tools-0.4.9/bin/stretch_head_jog.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body_tools-0.4.8/bin/stretch_lift_jog.py` & `hello_robot_stretch_body_tools-0.4.9/bin/stretch_lift_jog.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body_tools-0.4.8/bin/stretch_params.py` & `hello_robot_stretch_body_tools-0.4.9/bin/stretch_params.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body_tools-0.4.8/bin/stretch_pimu_jog.py` & `hello_robot_stretch_body_tools-0.4.9/bin/stretch_pimu_jog.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body_tools-0.4.8/bin/stretch_pimu_scope.py` & `hello_robot_stretch_body_tools-0.4.9/bin/stretch_pimu_scope.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body_tools-0.4.8/bin/stretch_realsense_visualizer.py` & `hello_robot_stretch_body_tools-0.4.9/bin/stretch_realsense_visualizer.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body_tools-0.4.8/bin/stretch_respeaker_test.py` & `hello_robot_stretch_body_tools-0.4.9/bin/stretch_respeaker_test.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body_tools-0.4.8/bin/stretch_robot_battery_check.py` & `hello_robot_stretch_body_tools-0.4.9/bin/stretch_robot_battery_check.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body_tools-0.4.8/bin/stretch_robot_dynamixel_reboot.py` & `hello_robot_stretch_body_tools-0.4.9/bin/stretch_robot_dynamixel_reboot.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body_tools-0.4.8/bin/stretch_robot_jog.py` & `hello_robot_stretch_body_tools-0.4.9/bin/stretch_robot_jog.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body_tools-0.4.8/bin/stretch_robot_keyboard_teleop.py` & `hello_robot_stretch_body_tools-0.4.9/bin/stretch_robot_keyboard_teleop.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body_tools-0.4.8/bin/stretch_robot_monitor.py` & `hello_robot_stretch_body_tools-0.4.9/bin/stretch_robot_monitor.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body_tools-0.4.8/bin/stretch_robot_system_check.py` & `hello_robot_stretch_body_tools-0.4.9/bin/stretch_robot_system_check.py`

 * *Files 20% similar despite different names*

```diff
@@ -18,14 +18,21 @@
 def val_in_range(val_name, val,vmin, vmax):
     p=val <=vmax and val>=vmin
     if p:
         print(Fore.GREEN +'[Pass] ' + val_name + ' = ' + str(val))
     else:
         print(Fore.RED +'[Fail] ' + val_name + ' = ' +str(val)+ ' out of range ' +str(vmin) + ' to ' + str(vmax))
 
+def val_in_range_warn(val_name, val,vmin, vmax, hint=""):
+    p=val <=vmax and val>=vmin
+    if p:
+        print(Fore.GREEN +'[Pass] ' + val_name + ' = ' + str(val))
+    else:
+        print(Fore.YELLOW +'[Warn] ' + val_name + ' = ' +str(val)+ ' out of range ' +str(vmin) + ' to ' + str(vmax) + hint)
+
 def val_is_not(val_name, val,vnot):
     if val is not vnot:
         print(Fore.GREEN +'[Pass] ' + val_name + ' = ' + str(val))
     else:
         print(Fore.RED +'[Fail] ' + val_name + ' = ' +str(val))
 
 #Turn off logging so get a clean output
@@ -55,18 +62,18 @@
 print(Style.RESET_ALL)
 if robot_devices['hello-pimu']:
     print('---- Checking Pimu ----')
     p=r.pimu
     val_in_range('Voltage',p.status['voltage'], vmin=p.config['low_voltage_alert'], vmax=14.5)
     val_in_range('Current',p.status['current'], vmin=0.5, vmax=p.config['high_current_alert'])
     val_in_range('Temperature',p.status['temp'], vmin=10, vmax=40)
-    val_in_range('Cliff-0',p.status['cliff_range'][0], vmin=p.config['cliff_thresh'], vmax=60)
-    val_in_range('Cliff-1',p.status['cliff_range'][1], vmin=p.config['cliff_thresh'], vmax=60)
-    val_in_range('Cliff-2',p.status['cliff_range'][2], vmin=p.config['cliff_thresh'], vmax=60)
-    val_in_range('Cliff-3',p.status['cliff_range'][3], vmin=p.config['cliff_thresh'], vmax=60)
+    val_in_range_warn('Cliff-0',p.status['cliff_range'][0], vmin=p.config['cliff_thresh'], vmax=60, hint=' - calibrate using REx_cliff_sensor_calibrate.py')
+    val_in_range_warn('Cliff-1',p.status['cliff_range'][1], vmin=p.config['cliff_thresh'], vmax=60, hint=' - calibrate using REx_cliff_sensor_calibrate.py')
+    val_in_range_warn('Cliff-2',p.status['cliff_range'][2], vmin=p.config['cliff_thresh'], vmax=60, hint=' - calibrate using REx_cliff_sensor_calibrate.py')
+    val_in_range_warn('Cliff-3',p.status['cliff_range'][3], vmin=p.config['cliff_thresh'], vmax=60, hint=' - calibrate using REx_cliff_sensor_calibrate.py')
     val_in_range('IMU AZ',p.status['imu']['az'], vmin=-10.1, vmax=-9.5)
     val_in_range('IMU Pitch', hu.rad_to_deg(p.status['imu']['pitch']), vmin=-12, vmax=12)
     val_in_range('IMU Roll', hu.rad_to_deg(p.status['imu']['roll']), vmin=-12, vmax=12)
     print(Style.RESET_ALL)
 
 # #####################################################
 print(Style.RESET_ALL)
```

### Comparing `hello_robot_stretch_body_tools-0.4.8/bin/stretch_robot_urdf_visualizer.py` & `hello_robot_stretch_body_tools-0.4.9/bin/stretch_robot_urdf_visualizer.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body_tools-0.4.8/bin/stretch_rp_lidar_jog.py` & `hello_robot_stretch_body_tools-0.4.9/bin/stretch_rp_lidar_jog.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body_tools-0.4.8/bin/stretch_trajectory_jog.py` & `hello_robot_stretch_body_tools-0.4.9/bin/stretch_trajectory_jog.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body_tools-0.4.8/bin/stretch_version.sh` & `hello_robot_stretch_body_tools-0.4.9/bin/stretch_version.sh`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body_tools-0.4.8/bin/stretch_wacc_jog.py` & `hello_robot_stretch_body_tools-0.4.9/bin/stretch_wacc_jog.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body_tools-0.4.8/bin/stretch_wacc_scope.py` & `hello_robot_stretch_body_tools-0.4.9/bin/stretch_wacc_scope.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body_tools-0.4.8/bin/stretch_wrist_yaw_jog.py` & `hello_robot_stretch_body_tools-0.4.9/bin/stretch_wrist_yaw_jog.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body_tools-0.4.8/bin/stretch_xbox_controller_teleop.py` & `hello_robot_stretch_body_tools-0.4.9/bin/stretch_xbox_controller_teleop.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body_tools-0.4.8/hello_robot_stretch_body_tools.egg-info/PKG-INFO` & `hello_robot_stretch_body_tools-0.4.9/hello_robot_stretch_body_tools.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,72 +1,69 @@
 Metadata-Version: 2.1
 Name: hello-robot-stretch-body-tools
-Version: 0.4.8
+Version: 0.4.9
 Summary: Stretch Body Tools
 Home-page: https://github.com/hello-robot/stretch_body
 Author: Hello Robot Inc
 Author-email: support@hello-robot.com
 License: UNKNOWN
+Description: Stretch Body Command Line Tools
+        ===============================
+        
+        This package provides Python tools that work with the Hello Robot Stretch Body package. These tools perform common tasks when working with Stretch (e.g. homing and stowing), and serve as tutorial code for working on various parts of the robot. This package comes pre-installed on Stretch robots. A tutorial for using this package can be found [on the docs](https://docs.hello-robot.com/0.2/stretch-tutorials/stretch_body/tutorial_command_line_tools/).
+        
+        Installing
+        ----------
+        
+        This package comes pre-installed on Stretch robots. To install or upgrade to a stable Stretch Body Command Line Tools for Python3, run:
+        
+        ```bash
+        $ python3 -m pip install --upgrade hello-robot-stretch-body-tools
+        ```
+        
+        To install or upgrade to a pre-release of the Command Line Tools for Python3, run:
+        
+        ```bash
+        $ python3 -m pip install --upgrade --pre hello-robot-stretch-body-tools
+        ```
+        
+        Please report feedback on the [Issue Tracker](https://github.com/hello-robot/stretch_body/issues) or the [Forum](https://forum.hello-robot.com/).
+        
+        Usage
+        -----
+        
+        All of the command-line tools reside within the `bin/` folder. When this package is installed, they are accessible from anywhere as command-line tools. For example, to perform a robot system check, run:
+        
+        ```bash
+        $ stretch_robot_system_check.py
+        ```
+        
+        For more info on these tools, see the [tutorial](https://docs.hello-robot.com/0.2/stretch-tutorials/stretch_body/tutorial_command_line_tools/).
+        
+        Developing
+        ----------
+        
+        The source code for the command-line tools resides within the `bin/` folder. You can install the tools package as "editable", and directly edit the source code to test changes.
+        
+        In Python3, run `python3 -m pip install -e .`
+        
+        For example, to test changes to the  `stretch_robot_home.py` script, run
+        
+        ```bash
+        $ python3 -m pip uninstall hello-robot-stretch-body-tools # ensure previous Stretch Body Tools installations are removed
+        $ git clone https://github.com/hello-robot/stretch_body.git
+        $ cd stretch_body/tools
+        $ python3 -m pip install -e .
+        ```
+        
+        Now, make desired edits to the [stretch_robot_home.py](./bin/stretch_robot_home.py) file. Executing the script on the command-line will now run your modified version.
+        
+        Deploying
+        ---------
+        
+        Increment the version number and run the `deploy.sh` script. Verify the new release is reflected [on PyPI](https://pypi.org/project/hello-robot-stretch-body-tools/).
+        
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: Apache Software License
 Description-Content-Type: text/markdown
-License-File: LICENSE.md
-
-Stretch Body Command Line Tools
-===============================
-
-This package provides Python tools that work with the Hello Robot Stretch Body package. These tools perform common tasks when working with Stretch (e.g. homing and stowing), and serve as tutorial code for working on various parts of the robot. This package comes pre-installed on Stretch robots. A tutorial for using this package can be found [on the docs](https://docs.hello-robot.com/0.2/stretch-tutorials/stretch_body/tutorial_command_line_tools/).
-
-Installing
-----------
-
-This package comes pre-installed on Stretch robots. To install or upgrade to a stable Stretch Body Command Line Tools for Python3, run:
-
-```bash
-$ python3 -m pip install --upgrade hello-robot-stretch-body-tools
-```
-
-To install or upgrade to a pre-release of the Command Line Tools for Python3, run:
-
-```bash
-$ python3 -m pip install --upgrade --pre hello-robot-stretch-body-tools
-```
-
-Please report feedback on the [Issue Tracker](https://github.com/hello-robot/stretch_body/issues) or the [Forum](https://forum.hello-robot.com/).
-
-Usage
------
-
-All of the command-line tools reside within the `bin/` folder. When this package is installed, they are accessible from anywhere as command-line tools. For example, to perform a robot system check, run:
-
-```bash
-$ stretch_robot_system_check.py
-```
-
-For more info on these tools, see the [tutorial](https://docs.hello-robot.com/0.2/stretch-tutorials/stretch_body/tutorial_command_line_tools/).
-
-Developing
-----------
-
-The source code for the command-line tools resides within the `bin/` folder. You can install the tools package as "editable", and directly edit the source code to test changes.
-
-In Python3, run `python3 -m pip install -e .`
-
-For example, to test changes to the  `stretch_robot_home.py` script, run
-
-```bash
-$ python3 -m pip uninstall hello-robot-stretch-body-tools # ensure previous Stretch Body Tools installations are removed
-$ git clone https://github.com/hello-robot/stretch_body.git
-$ cd stretch_body/tools
-$ python3 -m pip install -e .
-```
-
-Now, make desired edits to the [stretch_robot_home.py](./bin/stretch_robot_home.py) file. Executing the script on the command-line will now run your modified version.
-
-Deploying
----------
-
-Increment the version number and run the `deploy.sh` script. Verify the new release is reflected [on PyPI](https://pypi.org/project/hello-robot-stretch-body-tools/).
-
-
```

### Comparing `hello_robot_stretch_body_tools-0.4.8/hello_robot_stretch_body_tools.egg-info/SOURCES.txt` & `hello_robot_stretch_body_tools-0.4.9/hello_robot_stretch_body_tools.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-LICENSE.md
 README.md
 setup.py
 ./bin/stretch_about.py
 ./bin/stretch_about_text.py
 ./bin/stretch_arm_home.py
 ./bin/stretch_arm_jog.py
 ./bin/stretch_audio_test.py
```

### Comparing `hello_robot_stretch_body_tools-0.4.8/setup.py` & `hello_robot_stretch_body_tools-0.4.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 script_path='./bin'
 ex_scripts = glob.glob(script_path+'/*.py') + glob.glob(script_path+'/*.sh')
 stretch_scripts=[f for f in ex_scripts if isfile(f)]
 
 setuptools.setup(
     name="hello_robot_stretch_body_tools",
-    version="0.4.8",
+    version="0.4.9",
     author="Hello Robot Inc",
     author_email="support@hello-robot.com",
     description="Stretch Body Tools",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/hello-robot/stretch_body",
     scripts = stretch_scripts,
```

### Comparing `hello_robot_stretch_body_tools-0.4.8/test/test_tools_launch.py` & `hello_robot_stretch_body_tools-0.4.9/test/test_tools_launch.py`

 * *Files identical despite different names*

