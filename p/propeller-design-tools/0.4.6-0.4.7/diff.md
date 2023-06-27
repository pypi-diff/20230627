# Comparing `tmp/propeller_design_tools-0.4.6.tar.gz` & `tmp/propeller_design_tools-0.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "propeller_design_tools-0.4.6.tar", last modified: Sat Jun 24 08:11:02 2023, max compression
+gzip compressed data, was "propeller_design_tools-0.4.7.tar", last modified: Tue Jun 27 17:04:18 2023, max compression
```

## Comparing `propeller_design_tools-0.4.6.tar` & `propeller_design_tools-0.4.7.tar`

### file list

```diff
@@ -1,219 +1,220 @@
-drwxrwxrwx   0        0        0        0 2023-06-24 08:11:02.277055 propeller_design_tools-0.4.6/
--rw-rw-rw-   0        0        0    35801 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.6/LICENSE
--rw-rw-rw-   0        0        0     1403 2023-06-19 04:50:38.000000 propeller_design_tools-0.4.6/MANIFEST.in
--rw-rw-rw-   0        0        0    54444 2023-06-24 08:11:02.276053 propeller_design_tools-0.4.6/PKG-INFO
--rw-rw-rw-   0        0        0    11892 2023-06-24 07:37:35.000000 propeller_design_tools-0.4.6/README.md
-drwxrwxrwx   0        0        0        0 2023-06-24 08:11:01.853723 propeller_design_tools-0.4.6/propeller_design_tools/
--rw-rw-rw-   0        0        0      479 2023-06-18 03:29:37.000000 propeller_design_tools-0.4.6/propeller_design_tools/__init__.py
--rw-rw-rw-   0        0        0    28820 2023-06-18 03:29:37.000000 propeller_design_tools-0.4.6/propeller_design_tools/airfoil.py
--rw-rw-rw-   0        0        0     4871 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.6/propeller_design_tools/custom_opengl_classes.py
-drwxrwxrwx   0        0        0        0 2023-06-24 08:11:01.875779 propeller_design_tools-0.4.6/propeller_design_tools/foil_database/
--rw-rw-rw-   0        0        0     1132 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.6/propeller_design_tools/foil_database/arad13.dat
--rw-rw-rw-   0        0        0     2730 2023-06-19 07:10:22.000000 propeller_design_tools-0.4.6/propeller_design_tools/foil_database/clarky.dat
--rw-rw-rw-   0        0        0     1520 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.6/propeller_design_tools/foil_database/e855.dat
--rw-rw-rw-   0        0        0     2778 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.6/propeller_design_tools/foil_database/hs1606.dat
--rw-rw-rw-   0        0        0     2768 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.6/propeller_design_tools/foil_database/mrc-16.dat
--rwxrwxrwx   0        0        0  1002125 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.6/propeller_design_tools/foil_database/xfoil.exe
--rw-rw-rw-   0        0        0    18378 2023-06-18 03:29:37.000000 propeller_design_tools-0.4.6/propeller_design_tools/foil_ui_classes.py
--rw-rw-rw-   0        0        0    50416 2023-06-18 03:29:37.000000 propeller_design_tools-0.4.6/propeller_design_tools/funcs.py
--rw-rw-rw-   0        0        0    17861 2023-06-18 03:29:37.000000 propeller_design_tools-0.4.6/propeller_design_tools/helper_ui_classes.py
--rw-rw-rw-   0        0        0    16315 2023-06-18 03:29:37.000000 propeller_design_tools-0.4.6/propeller_design_tools/helper_ui_subclasses.py
--rw-rw-rw-   0        0        0      401 2023-06-18 03:29:37.000000 propeller_design_tools-0.4.6/propeller_design_tools/opt_ui_classes.py
--rw-rw-rw-   0        0        0    11040 2023-06-18 03:29:37.000000 propeller_design_tools-0.4.6/propeller_design_tools/optimizations.py
--rw-rw-rw-   0        0        0    15622 2023-06-18 03:29:37.000000 propeller_design_tools-0.4.6/propeller_design_tools/prop_analysis_ui_classes.py
--rw-rw-rw-   0        0        0    37027 2023-06-19 04:50:38.000000 propeller_design_tools-0.4.6/propeller_design_tools/prop_creation_ui_classes.py
-drwxrwxrwx   0        0        0        0 2023-06-24 08:11:01.887780 propeller_design_tools-0.4.6/propeller_design_tools/prop_database/
-drwxrwxrwx   0        0        0        0 2023-06-24 08:11:01.907247 propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller/
--rw-rw-rw-   0        0        0    25993 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller/MyPropeller.meta
--rw-rw-rw-   0        0        0     8599 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller/MyPropeller.xrop
--rw-rw-rw-   0        0        0     6239 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller/MyPropeller.xrr
-drwxrwxrwx   0        0        0        0 2023-06-24 08:11:02.259054 propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller/blade_profiles/
--rw-rw-rw-   0        0        0     3813 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_0.txt
--rw-rw-rw-   0        0        0     3806 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_1.txt
--rw-rw-rw-   0        0        0     3803 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_10.txt
--rw-rw-rw-   0        0        0     3803 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_11.txt
--rw-rw-rw-   0        0        0     3803 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_12.txt
--rw-rw-rw-   0        0        0     3803 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_13.txt
--rw-rw-rw-   0        0        0     3804 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_14.txt
--rw-rw-rw-   0        0        0     3803 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_15.txt
--rw-rw-rw-   0        0        0     3803 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_16.txt
--rw-rw-rw-   0        0        0     3803 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_17.txt
--rw-rw-rw-   0        0        0     3803 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_18.txt
--rw-rw-rw-   0        0        0     3803 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_19.txt
--rw-rw-rw-   0        0        0     3804 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_2.txt
--rw-rw-rw-   0        0        0     3803 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_20.txt
--rw-rw-rw-   0        0        0     3803 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_21.txt
--rw-rw-rw-   0        0        0     3802 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_22.txt
--rw-rw-rw-   0        0        0     3802 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_23.txt
--rw-rw-rw-   0        0        0     3803 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_24.txt
--rw-rw-rw-   0        0        0     3803 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_25.txt
--rw-rw-rw-   0        0        0     3803 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_26.txt
--rw-rw-rw-   0        0        0     3803 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_27.txt
--rw-rw-rw-   0        0        0     3803 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_28.txt
--rw-rw-rw-   0        0        0     3803 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_29.txt
--rw-rw-rw-   0        0        0     3804 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_3.txt
--rw-rw-rw-   0        0        0     3802 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_30.txt
--rw-rw-rw-   0        0        0     3803 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_31.txt
--rw-rw-rw-   0        0        0     3804 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_32.txt
--rw-rw-rw-   0        0        0     3805 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_33.txt
--rw-rw-rw-   0        0        0     3805 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_34.txt
--rw-rw-rw-   0        0        0     3805 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_35.txt
--rw-rw-rw-   0        0        0     3805 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_36.txt
--rw-rw-rw-   0        0        0     3804 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_37.txt
--rw-rw-rw-   0        0        0     3805 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_38.txt
--rw-rw-rw-   0        0        0     3805 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_39.txt
--rw-rw-rw-   0        0        0     3804 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_4.txt
--rw-rw-rw-   0        0        0     3805 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_40.txt
--rw-rw-rw-   0        0        0     3805 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_41.txt
--rw-rw-rw-   0        0        0     3806 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_42.txt
--rw-rw-rw-   0        0        0     3806 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_43.txt
--rw-rw-rw-   0        0        0     3807 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_44.txt
--rw-rw-rw-   0        0        0     3806 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_45.txt
--rw-rw-rw-   0        0        0     3806 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_46.txt
--rw-rw-rw-   0        0        0     3806 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_47.txt
--rw-rw-rw-   0        0        0     3806 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_48.txt
--rw-rw-rw-   0        0        0     3808 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_49.txt
--rw-rw-rw-   0        0        0     3803 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_5.txt
--rw-rw-rw-   0        0        0     3803 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_6.txt
--rw-rw-rw-   0        0        0     3802 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_7.txt
--rw-rw-rw-   0        0        0     3802 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_8.txt
--rw-rw-rw-   0        0        0     3803 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_9.txt
-drwxrwxrwx   0        0        0        0 2023-06-24 08:11:02.262054 propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller/station_polars/
--rw-rw-rw-   0        0        0     4595 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller/station_polars/0.75_clarky.dat.polar
-drwxrwxrwx   0        0        0        0 2023-06-24 08:11:01.917809 propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller2/
--rw-rw-rw-   0        0        0    13191 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller2/MyPropeller2.meta
--rw-rw-rw-   0        0        0     4923 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller2/MyPropeller2.xrop
--rw-rw-rw-   0        0        0     3593 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller2/MyPropeller2.xrr
-drwxrwxrwx   0        0        0        0 2023-06-24 08:11:02.028054 propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/
--rw-rw-rw-   0        0        0     2066 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_0.txt
--rw-rw-rw-   0        0        0     2066 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_1.txt
--rw-rw-rw-   0        0        0     2065 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_10.txt
--rw-rw-rw-   0        0        0     2065 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_11.txt
--rw-rw-rw-   0        0        0     2065 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_12.txt
--rw-rw-rw-   0        0        0     2066 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_13.txt
--rw-rw-rw-   0        0        0     2065 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_14.txt
--rw-rw-rw-   0        0        0     2065 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_15.txt
--rw-rw-rw-   0        0        0     2065 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_16.txt
--rw-rw-rw-   0        0        0     2065 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_17.txt
--rw-rw-rw-   0        0        0     2065 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_18.txt
--rw-rw-rw-   0        0        0     2063 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_19.txt
--rw-rw-rw-   0        0        0     2066 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_2.txt
--rw-rw-rw-   0        0        0     2064 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_20.txt
--rw-rw-rw-   0        0        0     2064 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_21.txt
--rw-rw-rw-   0        0        0     2064 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_22.txt
--rw-rw-rw-   0        0        0     2064 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_23.txt
--rw-rw-rw-   0        0        0     2063 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_24.txt
--rw-rw-rw-   0        0        0     2063 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_25.txt
--rw-rw-rw-   0        0        0     2063 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_26.txt
--rw-rw-rw-   0        0        0     2063 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_27.txt
--rw-rw-rw-   0        0        0     2063 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_28.txt
--rw-rw-rw-   0        0        0     2063 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_29.txt
--rw-rw-rw-   0        0        0     2066 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_3.txt
--rw-rw-rw-   0        0        0     2062 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_30.txt
--rw-rw-rw-   0        0        0     2063 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_31.txt
--rw-rw-rw-   0        0        0     2063 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_32.txt
--rw-rw-rw-   0        0        0     2063 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_33.txt
--rw-rw-rw-   0        0        0     2063 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_34.txt
--rw-rw-rw-   0        0        0     2063 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_35.txt
--rw-rw-rw-   0        0        0     2063 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_36.txt
--rw-rw-rw-   0        0        0     2062 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_37.txt
--rw-rw-rw-   0        0        0     2063 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_38.txt
--rw-rw-rw-   0        0        0     2063 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_39.txt
--rw-rw-rw-   0        0        0     2066 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_4.txt
--rw-rw-rw-   0        0        0     2063 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_40.txt
--rw-rw-rw-   0        0        0     2063 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_41.txt
--rw-rw-rw-   0        0        0     2063 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_42.txt
--rw-rw-rw-   0        0        0     2063 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_43.txt
--rw-rw-rw-   0        0        0     2062 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_44.txt
--rw-rw-rw-   0        0        0     2062 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_45.txt
--rw-rw-rw-   0        0        0     2062 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_46.txt
--rw-rw-rw-   0        0        0     2062 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_47.txt
--rw-rw-rw-   0        0        0     2062 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_48.txt
--rw-rw-rw-   0        0        0     2063 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_49.txt
--rw-rw-rw-   0        0        0     2066 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_5.txt
--rw-rw-rw-   0        0        0     2065 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_6.txt
--rw-rw-rw-   0        0        0     2066 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_7.txt
--rw-rw-rw-   0        0        0     2066 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_8.txt
--rw-rw-rw-   0        0        0     2066 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_9.txt
-drwxrwxrwx   0        0        0        0 2023-06-24 08:11:02.030053 propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller2/station_polars/
--rw-rw-rw-   0        0        0     5160 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller2/station_polars/0.75_e855.dat.polar
-drwxrwxrwx   0        0        0        0 2023-06-24 08:11:02.037056 propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller3/
--rw-rw-rw-   0        0        0    13630 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller3/MyPropeller3.meta
--rw-rw-rw-   0        0        0     4875 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller3/MyPropeller3.xrop
--rw-rw-rw-   0        0        0     3593 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller3/MyPropeller3.xrr
-drwxrwxrwx   0        0        0        0 2023-06-24 08:11:02.147054 propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/
--rw-rw-rw-   0        0        0     3771 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_0.txt
--rw-rw-rw-   0        0        0     3769 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_1.txt
--rw-rw-rw-   0        0        0     3766 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_10.txt
--rw-rw-rw-   0        0        0     3765 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_11.txt
--rw-rw-rw-   0        0        0     3767 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_12.txt
--rw-rw-rw-   0        0        0     3766 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_13.txt
--rw-rw-rw-   0        0        0     3766 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_14.txt
--rw-rw-rw-   0        0        0     3767 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_15.txt
--rw-rw-rw-   0        0        0     3766 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_16.txt
--rw-rw-rw-   0        0        0     3766 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_17.txt
--rw-rw-rw-   0        0        0     3768 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_18.txt
--rw-rw-rw-   0        0        0     3767 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_19.txt
--rw-rw-rw-   0        0        0     3769 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_2.txt
--rw-rw-rw-   0        0        0     3769 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_20.txt
--rw-rw-rw-   0        0        0     3769 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_21.txt
--rw-rw-rw-   0        0        0     3770 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_22.txt
--rw-rw-rw-   0        0        0     3771 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_23.txt
--rw-rw-rw-   0        0        0     3771 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_24.txt
--rw-rw-rw-   0        0        0     3774 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_25.txt
--rw-rw-rw-   0        0        0     3775 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_26.txt
--rw-rw-rw-   0        0        0     3777 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_27.txt
--rw-rw-rw-   0        0        0     3778 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_28.txt
--rw-rw-rw-   0        0        0     3781 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_29.txt
--rw-rw-rw-   0        0        0     3769 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_3.txt
--rw-rw-rw-   0        0        0     3784 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_30.txt
--rw-rw-rw-   0        0        0     3795 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_31.txt
--rw-rw-rw-   0        0        0     3794 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_32.txt
--rw-rw-rw-   0        0        0     3795 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_33.txt
--rw-rw-rw-   0        0        0     3794 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_34.txt
--rw-rw-rw-   0        0        0     3794 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_35.txt
--rw-rw-rw-   0        0        0     3794 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_36.txt
--rw-rw-rw-   0        0        0     3794 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_37.txt
--rw-rw-rw-   0        0        0     3794 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_38.txt
--rw-rw-rw-   0        0        0     3793 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_39.txt
--rw-rw-rw-   0        0        0     3768 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_4.txt
--rw-rw-rw-   0        0        0     3793 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_40.txt
--rw-rw-rw-   0        0        0     3793 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_41.txt
--rw-rw-rw-   0        0        0     3793 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_42.txt
--rw-rw-rw-   0        0        0     3793 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_43.txt
--rw-rw-rw-   0        0        0     3793 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_44.txt
--rw-rw-rw-   0        0        0     3792 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_45.txt
--rw-rw-rw-   0        0        0     3792 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_46.txt
--rw-rw-rw-   0        0        0     3793 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_47.txt
--rw-rw-rw-   0        0        0     3792 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_48.txt
--rw-rw-rw-   0        0        0     3792 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_49.txt
--rw-rw-rw-   0        0        0     3767 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_5.txt
--rw-rw-rw-   0        0        0     3767 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_6.txt
--rw-rw-rw-   0        0        0     3766 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_7.txt
--rw-rw-rw-   0        0        0     3766 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_8.txt
--rw-rw-rw-   0        0        0     3766 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_9.txt
-drwxrwxrwx   0        0        0        0 2023-06-24 08:11:02.149054 propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller3/station_polars/
--rw-rw-rw-   0        0        0     6152 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller3/station_polars/0.75_mrc-16.dat.polar
--rwxrwxrwx   0        0        0  1176521 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.6/propeller_design_tools/prop_database/xrotor.exe
--rw-rw-rw-   0        0        0    53871 2023-06-18 03:29:37.000000 propeller_design_tools-0.4.6/propeller_design_tools/propeller.py
--rw-rw-rw-   0        0        0    17617 2023-06-18 03:29:37.000000 propeller_design_tools-0.4.6/propeller_design_tools/radialstation.py
--rw-rw-rw-   0        0        0     1674 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.6/propeller_design_tools/science_spinbox_class.py
--rw-rw-rw-   0        0        0     4111 2023-06-18 03:29:37.000000 propeller_design_tools-0.4.6/propeller_design_tools/settings.py
-drwxrwxrwx   0        0        0        0 2023-06-24 08:11:02.274054 propeller_design_tools-0.4.6/propeller_design_tools/supporting_files/
--rw-rw-rw-   0        0        0     1358 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.6/propeller_design_tools/supporting_files/crosshair_cursor.png
--rw-rw-rw-   0        0        0    10192 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.6/propeller_design_tools/supporting_files/gunshot1.wav
--rw-rw-rw-   0        0        0    18704 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.6/propeller_design_tools/supporting_files/gunshot2.wav
--rw-rw-rw-   0        0        0    23984 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.6/propeller_design_tools/supporting_files/gunshot3.wav
--rw-rw-rw-   0        0        0    24784 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.6/propeller_design_tools/supporting_files/gunshot4.wav
--rw-rw-rw-   0        0        0      292 2023-06-24 08:06:42.000000 propeller_design_tools-0.4.6/propeller_design_tools/supporting_files/user-settings.txt
--rw-rw-rw-   0        0        0     5857 2023-06-18 03:29:37.000000 propeller_design_tools-0.4.6/propeller_design_tools/user_interface.py
--rw-rw-rw-   0        0        0     2839 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.6/propeller_design_tools/user_io.py
-drwxrwxrwx   0        0        0        0 2023-06-24 08:11:01.862722 propeller_design_tools-0.4.6/propeller_design_tools.egg-info/
--rw-rw-rw-   0        0        0    54444 2023-06-24 08:11:01.000000 propeller_design_tools-0.4.6/propeller_design_tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    14426 2023-06-24 08:11:01.000000 propeller_design_tools-0.4.6/propeller_design_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-24 08:11:01.000000 propeller_design_tools-0.4.6/propeller_design_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      118 2023-06-24 08:11:01.000000 propeller_design_tools-0.4.6/propeller_design_tools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       23 2023-06-24 08:11:01.000000 propeller_design_tools-0.4.6/propeller_design_tools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2006 2023-06-24 08:10:46.000000 propeller_design_tools-0.4.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-24 08:11:02.277055 propeller_design_tools-0.4.6/setup.cfg
--rw-rw-rw-   0        0        0       43 2023-06-18 02:25:12.000000 propeller_design_tools-0.4.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-27 17:04:18.325255 propeller_design_tools-0.4.7/
+-rw-rw-rw-   0        0        0    35801 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.7/LICENSE
+-rw-rw-rw-   0        0        0     1403 2023-06-19 04:50:38.000000 propeller_design_tools-0.4.7/MANIFEST.in
+-rw-rw-rw-   0        0        0    54550 2023-06-27 17:04:18.325255 propeller_design_tools-0.4.7/PKG-INFO
+-rw-rw-rw-   0        0        0    11996 2023-06-24 08:24:37.000000 propeller_design_tools-0.4.7/README.md
+drwxrwxrwx   0        0        0        0 2023-06-27 17:04:18.027522 propeller_design_tools-0.4.7/propeller_design_tools/
+-rw-rw-rw-   0        0        0      479 2023-06-18 03:29:37.000000 propeller_design_tools-0.4.7/propeller_design_tools/__init__.py
+-rw-rw-rw-   0        0        0    28835 2023-06-27 16:53:37.000000 propeller_design_tools-0.4.7/propeller_design_tools/airfoil.py
+-rw-rw-rw-   0        0        0     4871 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.7/propeller_design_tools/custom_opengl_classes.py
+drwxrwxrwx   0        0        0        0 2023-06-27 17:04:18.048277 propeller_design_tools-0.4.7/propeller_design_tools/foil_database/
+-rw-rw-rw-   0        0        0     1132 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.7/propeller_design_tools/foil_database/arad13.dat
+-rw-rw-rw-   0        0        0     2730 2023-06-19 07:10:22.000000 propeller_design_tools-0.4.7/propeller_design_tools/foil_database/clarky.dat
+-rw-rw-rw-   0        0        0     1520 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.7/propeller_design_tools/foil_database/e855.dat
+-rw-rw-rw-   0        0        0     2778 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.7/propeller_design_tools/foil_database/hs1606.dat
+-rw-rw-rw-   0        0        0     2768 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.7/propeller_design_tools/foil_database/mrc-16.dat
+-rwxrwxrwx   0        0        0  1002125 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.7/propeller_design_tools/foil_database/xfoil.exe
+-rw-rw-rw-   0        0        0    18378 2023-06-18 03:29:37.000000 propeller_design_tools-0.4.7/propeller_design_tools/foil_ui_classes.py
+-rw-rw-rw-   0        0        0    50515 2023-06-27 16:53:37.000000 propeller_design_tools-0.4.7/propeller_design_tools/funcs.py
+-rw-rw-rw-   0        0        0    17861 2023-06-18 03:29:37.000000 propeller_design_tools-0.4.7/propeller_design_tools/helper_ui_classes.py
+-rw-rw-rw-   0        0        0    16315 2023-06-18 03:29:37.000000 propeller_design_tools-0.4.7/propeller_design_tools/helper_ui_subclasses.py
+-rw-rw-rw-   0        0        0     1216 2023-06-27 16:53:30.000000 propeller_design_tools-0.4.7/propeller_design_tools/mobapp.py
+-rw-rw-rw-   0        0        0      401 2023-06-18 03:29:37.000000 propeller_design_tools-0.4.7/propeller_design_tools/opt_ui_classes.py
+-rw-rw-rw-   0        0        0    11059 2023-06-27 16:53:37.000000 propeller_design_tools-0.4.7/propeller_design_tools/optimizations.py
+-rw-rw-rw-   0        0        0    15628 2023-06-27 16:53:37.000000 propeller_design_tools-0.4.7/propeller_design_tools/prop_analysis_ui_classes.py
+-rw-rw-rw-   0        0        0    36995 2023-06-27 16:53:38.000000 propeller_design_tools-0.4.7/propeller_design_tools/prop_creation_ui_classes.py
+drwxrwxrwx   0        0        0        0 2023-06-27 17:04:18.048277 propeller_design_tools-0.4.7/propeller_design_tools/prop_database/
+drwxrwxrwx   0        0        0        0 2023-06-27 17:04:18.055334 propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller/
+-rw-rw-rw-   0        0        0    25993 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller/MyPropeller.meta
+-rw-rw-rw-   0        0        0     8599 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller/MyPropeller.xrop
+-rw-rw-rw-   0        0        0     6239 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller/MyPropeller.xrr
+drwxrwxrwx   0        0        0        0 2023-06-27 17:04:18.308463 propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller/blade_profiles/
+-rw-rw-rw-   0        0        0     3813 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_0.txt
+-rw-rw-rw-   0        0        0     3806 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_1.txt
+-rw-rw-rw-   0        0        0     3803 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_10.txt
+-rw-rw-rw-   0        0        0     3803 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_11.txt
+-rw-rw-rw-   0        0        0     3803 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_12.txt
+-rw-rw-rw-   0        0        0     3803 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_13.txt
+-rw-rw-rw-   0        0        0     3804 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_14.txt
+-rw-rw-rw-   0        0        0     3803 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_15.txt
+-rw-rw-rw-   0        0        0     3803 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_16.txt
+-rw-rw-rw-   0        0        0     3803 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_17.txt
+-rw-rw-rw-   0        0        0     3803 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_18.txt
+-rw-rw-rw-   0        0        0     3803 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_19.txt
+-rw-rw-rw-   0        0        0     3804 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_2.txt
+-rw-rw-rw-   0        0        0     3803 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_20.txt
+-rw-rw-rw-   0        0        0     3803 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_21.txt
+-rw-rw-rw-   0        0        0     3802 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_22.txt
+-rw-rw-rw-   0        0        0     3802 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_23.txt
+-rw-rw-rw-   0        0        0     3803 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_24.txt
+-rw-rw-rw-   0        0        0     3803 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_25.txt
+-rw-rw-rw-   0        0        0     3803 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_26.txt
+-rw-rw-rw-   0        0        0     3803 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_27.txt
+-rw-rw-rw-   0        0        0     3803 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_28.txt
+-rw-rw-rw-   0        0        0     3803 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_29.txt
+-rw-rw-rw-   0        0        0     3804 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_3.txt
+-rw-rw-rw-   0        0        0     3802 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_30.txt
+-rw-rw-rw-   0        0        0     3803 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_31.txt
+-rw-rw-rw-   0        0        0     3804 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_32.txt
+-rw-rw-rw-   0        0        0     3805 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_33.txt
+-rw-rw-rw-   0        0        0     3805 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_34.txt
+-rw-rw-rw-   0        0        0     3805 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_35.txt
+-rw-rw-rw-   0        0        0     3805 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_36.txt
+-rw-rw-rw-   0        0        0     3804 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_37.txt
+-rw-rw-rw-   0        0        0     3805 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_38.txt
+-rw-rw-rw-   0        0        0     3805 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_39.txt
+-rw-rw-rw-   0        0        0     3804 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_4.txt
+-rw-rw-rw-   0        0        0     3805 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_40.txt
+-rw-rw-rw-   0        0        0     3805 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_41.txt
+-rw-rw-rw-   0        0        0     3806 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_42.txt
+-rw-rw-rw-   0        0        0     3806 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_43.txt
+-rw-rw-rw-   0        0        0     3807 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_44.txt
+-rw-rw-rw-   0        0        0     3806 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_45.txt
+-rw-rw-rw-   0        0        0     3806 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_46.txt
+-rw-rw-rw-   0        0        0     3806 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_47.txt
+-rw-rw-rw-   0        0        0     3806 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_48.txt
+-rw-rw-rw-   0        0        0     3808 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_49.txt
+-rw-rw-rw-   0        0        0     3803 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_5.txt
+-rw-rw-rw-   0        0        0     3803 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_6.txt
+-rw-rw-rw-   0        0        0     3802 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_7.txt
+-rw-rw-rw-   0        0        0     3802 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_8.txt
+-rw-rw-rw-   0        0        0     3803 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_9.txt
+drwxrwxrwx   0        0        0        0 2023-06-27 17:04:18.315008 propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller/station_polars/
+-rw-rw-rw-   0        0        0     4595 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller/station_polars/0.75_clarky.dat.polar
+drwxrwxrwx   0        0        0        0 2023-06-27 17:04:18.057884 propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller2/
+-rw-rw-rw-   0        0        0    13191 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller2/MyPropeller2.meta
+-rw-rw-rw-   0        0        0     4923 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller2/MyPropeller2.xrop
+-rw-rw-rw-   0        0        0     3593 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller2/MyPropeller2.xrr
+drwxrwxrwx   0        0        0        0 2023-06-27 17:04:18.138750 propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/
+-rw-rw-rw-   0        0        0     2066 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_0.txt
+-rw-rw-rw-   0        0        0     2066 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_1.txt
+-rw-rw-rw-   0        0        0     2065 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_10.txt
+-rw-rw-rw-   0        0        0     2065 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_11.txt
+-rw-rw-rw-   0        0        0     2065 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_12.txt
+-rw-rw-rw-   0        0        0     2066 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_13.txt
+-rw-rw-rw-   0        0        0     2065 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_14.txt
+-rw-rw-rw-   0        0        0     2065 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_15.txt
+-rw-rw-rw-   0        0        0     2065 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_16.txt
+-rw-rw-rw-   0        0        0     2065 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_17.txt
+-rw-rw-rw-   0        0        0     2065 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_18.txt
+-rw-rw-rw-   0        0        0     2063 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_19.txt
+-rw-rw-rw-   0        0        0     2066 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_2.txt
+-rw-rw-rw-   0        0        0     2064 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_20.txt
+-rw-rw-rw-   0        0        0     2064 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_21.txt
+-rw-rw-rw-   0        0        0     2064 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_22.txt
+-rw-rw-rw-   0        0        0     2064 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_23.txt
+-rw-rw-rw-   0        0        0     2063 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_24.txt
+-rw-rw-rw-   0        0        0     2063 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_25.txt
+-rw-rw-rw-   0        0        0     2063 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_26.txt
+-rw-rw-rw-   0        0        0     2063 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_27.txt
+-rw-rw-rw-   0        0        0     2063 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_28.txt
+-rw-rw-rw-   0        0        0     2063 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_29.txt
+-rw-rw-rw-   0        0        0     2066 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_3.txt
+-rw-rw-rw-   0        0        0     2062 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_30.txt
+-rw-rw-rw-   0        0        0     2063 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_31.txt
+-rw-rw-rw-   0        0        0     2063 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_32.txt
+-rw-rw-rw-   0        0        0     2063 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_33.txt
+-rw-rw-rw-   0        0        0     2063 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_34.txt
+-rw-rw-rw-   0        0        0     2063 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_35.txt
+-rw-rw-rw-   0        0        0     2063 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_36.txt
+-rw-rw-rw-   0        0        0     2062 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_37.txt
+-rw-rw-rw-   0        0        0     2063 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_38.txt
+-rw-rw-rw-   0        0        0     2063 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_39.txt
+-rw-rw-rw-   0        0        0     2066 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_4.txt
+-rw-rw-rw-   0        0        0     2063 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_40.txt
+-rw-rw-rw-   0        0        0     2063 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_41.txt
+-rw-rw-rw-   0        0        0     2063 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_42.txt
+-rw-rw-rw-   0        0        0     2063 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_43.txt
+-rw-rw-rw-   0        0        0     2062 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_44.txt
+-rw-rw-rw-   0        0        0     2062 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_45.txt
+-rw-rw-rw-   0        0        0     2062 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_46.txt
+-rw-rw-rw-   0        0        0     2062 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_47.txt
+-rw-rw-rw-   0        0        0     2062 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_48.txt
+-rw-rw-rw-   0        0        0     2063 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_49.txt
+-rw-rw-rw-   0        0        0     2066 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_5.txt
+-rw-rw-rw-   0        0        0     2065 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_6.txt
+-rw-rw-rw-   0        0        0     2066 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_7.txt
+-rw-rw-rw-   0        0        0     2066 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_8.txt
+-rw-rw-rw-   0        0        0     2066 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_9.txt
+drwxrwxrwx   0        0        0        0 2023-06-27 17:04:18.138750 propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller2/station_polars/
+-rw-rw-rw-   0        0        0     5160 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller2/station_polars/0.75_e855.dat.polar
+drwxrwxrwx   0        0        0        0 2023-06-27 17:04:18.157968 propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller3/
+-rw-rw-rw-   0        0        0    13630 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller3/MyPropeller3.meta
+-rw-rw-rw-   0        0        0     4875 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller3/MyPropeller3.xrop
+-rw-rw-rw-   0        0        0     3593 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller3/MyPropeller3.xrr
+drwxrwxrwx   0        0        0        0 2023-06-27 17:04:18.236811 propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/
+-rw-rw-rw-   0        0        0     3771 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_0.txt
+-rw-rw-rw-   0        0        0     3769 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_1.txt
+-rw-rw-rw-   0        0        0     3766 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_10.txt
+-rw-rw-rw-   0        0        0     3765 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_11.txt
+-rw-rw-rw-   0        0        0     3767 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_12.txt
+-rw-rw-rw-   0        0        0     3766 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_13.txt
+-rw-rw-rw-   0        0        0     3766 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_14.txt
+-rw-rw-rw-   0        0        0     3767 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_15.txt
+-rw-rw-rw-   0        0        0     3766 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_16.txt
+-rw-rw-rw-   0        0        0     3766 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_17.txt
+-rw-rw-rw-   0        0        0     3768 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_18.txt
+-rw-rw-rw-   0        0        0     3767 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_19.txt
+-rw-rw-rw-   0        0        0     3769 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_2.txt
+-rw-rw-rw-   0        0        0     3769 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_20.txt
+-rw-rw-rw-   0        0        0     3769 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_21.txt
+-rw-rw-rw-   0        0        0     3770 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_22.txt
+-rw-rw-rw-   0        0        0     3771 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_23.txt
+-rw-rw-rw-   0        0        0     3771 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_24.txt
+-rw-rw-rw-   0        0        0     3774 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_25.txt
+-rw-rw-rw-   0        0        0     3775 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_26.txt
+-rw-rw-rw-   0        0        0     3777 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_27.txt
+-rw-rw-rw-   0        0        0     3778 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_28.txt
+-rw-rw-rw-   0        0        0     3781 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_29.txt
+-rw-rw-rw-   0        0        0     3769 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_3.txt
+-rw-rw-rw-   0        0        0     3784 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_30.txt
+-rw-rw-rw-   0        0        0     3795 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_31.txt
+-rw-rw-rw-   0        0        0     3794 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_32.txt
+-rw-rw-rw-   0        0        0     3795 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_33.txt
+-rw-rw-rw-   0        0        0     3794 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_34.txt
+-rw-rw-rw-   0        0        0     3794 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_35.txt
+-rw-rw-rw-   0        0        0     3794 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_36.txt
+-rw-rw-rw-   0        0        0     3794 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_37.txt
+-rw-rw-rw-   0        0        0     3794 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_38.txt
+-rw-rw-rw-   0        0        0     3793 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_39.txt
+-rw-rw-rw-   0        0        0     3768 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_4.txt
+-rw-rw-rw-   0        0        0     3793 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_40.txt
+-rw-rw-rw-   0        0        0     3793 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_41.txt
+-rw-rw-rw-   0        0        0     3793 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_42.txt
+-rw-rw-rw-   0        0        0     3793 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_43.txt
+-rw-rw-rw-   0        0        0     3793 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_44.txt
+-rw-rw-rw-   0        0        0     3792 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_45.txt
+-rw-rw-rw-   0        0        0     3792 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_46.txt
+-rw-rw-rw-   0        0        0     3793 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_47.txt
+-rw-rw-rw-   0        0        0     3792 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_48.txt
+-rw-rw-rw-   0        0        0     3792 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_49.txt
+-rw-rw-rw-   0        0        0     3767 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_5.txt
+-rw-rw-rw-   0        0        0     3767 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_6.txt
+-rw-rw-rw-   0        0        0     3766 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_7.txt
+-rw-rw-rw-   0        0        0     3766 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_8.txt
+-rw-rw-rw-   0        0        0     3766 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_9.txt
+drwxrwxrwx   0        0        0        0 2023-06-27 17:04:18.237846 propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller3/station_polars/
+-rw-rw-rw-   0        0        0     6152 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller3/station_polars/0.75_mrc-16.dat.polar
+-rwxrwxrwx   0        0        0  1176521 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.7/propeller_design_tools/prop_database/xrotor.exe
+-rw-rw-rw-   0        0        0    53932 2023-06-27 16:53:37.000000 propeller_design_tools-0.4.7/propeller_design_tools/propeller.py
+-rw-rw-rw-   0        0        0    17638 2023-06-27 16:53:37.000000 propeller_design_tools-0.4.7/propeller_design_tools/radialstation.py
+-rw-rw-rw-   0        0        0     1674 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.7/propeller_design_tools/science_spinbox_class.py
+-rw-rw-rw-   0        0        0     4217 2023-06-27 16:53:38.000000 propeller_design_tools-0.4.7/propeller_design_tools/settings.py
+drwxrwxrwx   0        0        0        0 2023-06-27 17:04:18.320147 propeller_design_tools-0.4.7/propeller_design_tools/supporting_files/
+-rw-rw-rw-   0        0        0     1358 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.7/propeller_design_tools/supporting_files/crosshair_cursor.png
+-rw-rw-rw-   0        0        0    10192 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.7/propeller_design_tools/supporting_files/gunshot1.wav
+-rw-rw-rw-   0        0        0    18704 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.7/propeller_design_tools/supporting_files/gunshot2.wav
+-rw-rw-rw-   0        0        0    23984 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.7/propeller_design_tools/supporting_files/gunshot3.wav
+-rw-rw-rw-   0        0        0    24784 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.7/propeller_design_tools/supporting_files/gunshot4.wav
+-rw-rw-rw-   0        0        0      292 2023-06-27 16:00:27.000000 propeller_design_tools-0.4.7/propeller_design_tools/supporting_files/user-settings.txt
+-rw-rw-rw-   0        0        0     6084 2023-06-27 16:53:38.000000 propeller_design_tools-0.4.7/propeller_design_tools/user_interface.py
+-rw-rw-rw-   0        0        0     2860 2023-06-27 16:53:30.000000 propeller_design_tools-0.4.7/propeller_design_tools/user_io.py
+drwxrwxrwx   0        0        0        0 2023-06-27 17:04:18.038925 propeller_design_tools-0.4.7/propeller_design_tools.egg-info/
+-rw-rw-rw-   0        0        0    54550 2023-06-27 17:04:17.000000 propeller_design_tools-0.4.7/propeller_design_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    14459 2023-06-27 17:04:17.000000 propeller_design_tools-0.4.7/propeller_design_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-27 17:04:17.000000 propeller_design_tools-0.4.7/propeller_design_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      118 2023-06-27 17:04:17.000000 propeller_design_tools-0.4.7/propeller_design_tools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       23 2023-06-27 17:04:17.000000 propeller_design_tools-0.4.7/propeller_design_tools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1994 2023-06-27 16:59:50.000000 propeller_design_tools-0.4.7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-27 17:04:18.325255 propeller_design_tools-0.4.7/setup.cfg
+-rw-rw-rw-   0        0        0       43 2023-06-18 02:25:12.000000 propeller_design_tools-0.4.7/setup.py
```

### Comparing `propeller_design_tools-0.4.6/LICENSE` & `propeller_design_tools-0.4.7/LICENSE`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.6/MANIFEST.in` & `propeller_design_tools-0.4.7/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.6/PKG-INFO` & `propeller_design_tools-0.4.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: propeller_design_tools
-Version: 0.4.6
+Version: 0.4.7
 Summary: Python 3.7 package that provides exactly what it sounds like by automating usage of MIT professor Mark Drela's GNU-licensed CLI-utilities XFOIL and XROTOR.
 Author-email: Jacob Bronson <bronsoneering@gmail.com>
 License: GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -700,131 +700,96 @@
 ---
 **Work in progress / incomplete documentation (all current documentation is below, as well as a step-by-step typical 
 usage/workflow scenario)**
 
 Note: The graphical user interface for this should be functional for Linux now as well!
 
 ---
-
 Description
 ===========
 Python 3.7 package that provides exactly what it sounds like by automating usage of the GPL-licensed 
 CLI-utilities XFOIL and XROTOR.
 
 Both utilities are published by professor Mark Drela (MIT).
+
 - XFOIL: for arbitrary 2D airfoil analysis and design
 - XROTOR: for arbitrary propeller design schemes and analysis
 
-XFOIL and XROTOR Executables
--------------------------------------------
-In order to utilize any PDT functionality that depends on
-running XFOIL, the "xfoil.exe" executable file needs to be
-in the user-set "airfoil_database" location. *Current pip
-installations include the xfoil.exe file in the foil_database,
-there should theoretically be no need to download it manually,
-even if the user changes the foil_database location.*
-
-[XFOIL executable and docs](https://web.mit.edu/drela/Public/web/xfoil/)
-
-Likewise, in order to utilize any PDT functionality that
-depends on running XROTOR, the "xrotor.exe" executable file
-needs to be in the user-set "propeller_database" location.
-*Current pip installations include the xrotor.exe file in the
-default prop_database, there should theoretically be no need to
-download it manually, even if the user changes the prop_database
-location.*
-
-[CROTOR executable and docs](http://www.esotec.org/sw/crotor.html#download)
-*(this is actually a link to "CROTOR", which I find is
-the easiest way to obtain a windows-executable of XROTOR)*
-
-[actual XROTOR docs](https://web.mit.edu/drela/Public/web/xrotor/xrotor_doc.txt)
-
-Both XFOIL and XROTOR contain much, much more utility than PDT currently has integrated. They are part of an incredible
-set of aerodynamic (or hydrodynamic) modeling command-line-interface (CLI) utilities from MIT. The ones that I 
-personally know of include:
-1. XFOIL - for arbitrary 2D airfoil analysis and design
-2. XROTOR - for arbitrary propeller design schemes and analysis
-3. AVL - for arbitrary lifting planform analysis
-4. QPROP - another CLI utility for propeller design and analysis
-5. QMIL - for arbitrary windmill designs (and more)
-
-Combined, the above represents an amazing fluid-dynamics modeling capability that is completely free, and fast. While 
-it's unlikely they will ever get as accurate as true computational-fluid-dynamics (CFD) software, they still offer 
-great value for being free, and are several orders of magnitude faster than true CFD software. Personally, I have found
-them to be completely sufficient tools for all stages of engineering design, but then again I have only ever worked in 
-prototyping engineering.
-
+---
 Troubleshooting PDT Errors / Crashes (GUI and/or Scripting)
 ===========================================================
-So I just quit my job as a systems engineer to become a software developer, so hopefully this package starts to get 
+So I just quit my job as a systems engineer to become a software developer, so hopefully this package starts to get
 more frequent updates and support from me. If you encounter what you think is an error coming from this code, I would
 love to know about it, please submit an issue to:
 
 [LINK TO GITHUB ISSUES](https://github.com/helloDestroyerOfWorlds/propeller_design_tools/issues)
 
-and I will likely see it quickly and will at least answer you, if not just fix it and push the update. Please only do 
+and I will likely see it quickly and will at least answer you, if not just fix it and push the update. Please only do
 this though once you are sure the error is coming from the PDT code.
 
-If you think you have discovered a legitimate issue, before submitting it please also read through the list below to 
+If you think you have discovered a legitimate issue, before submitting it please also read through the list below to
 see if any of the listed things could fix your error.
 
-1. XFOIL or XROTOR executables: Errors might be coming from XFOIL or XROTOR in actuality rather than this source code 
-   - Currently PDT implements these as executables installed when pip installing this package
-   - This means if you are having pip install errors and are on Linux it might be caused by that, actually, if you are 
-     having any errors, even in the GUI, and you are on Linux it might be caused by me not understanding until now much 
-     about Linux. If this is the case, and you think you know what is causing the error, please feel free to reach out 
-     to me via the issues link above.
-   - Additionally, I just implemented a fix to automatically install all required dependencies when pip installing this 
-     package. This should fix many issues for Linux users, if not all the current ones. Note that if you want to use the
-     GUI, read the next point.
-   - Still submit an issue using the link above if this is the case -> in theory I can detect most of these
+1. XFOIL or XROTOR executables: Errors might be coming from XFOIL or XROTOR in actuality rather than this source code
+    - Currently PDT implements these as executables installed when pip installing this package
+    - This means if you are having pip install errors and are on Linux it might be caused by that, actually, if you are
+      having any errors, even in the GUI, and you are on Linux it might be caused by me not understanding until now much
+      about Linux. If this is the case, and you think you know what is causing the error, please feel free to reach out
+      to me via the issues link above.
+    - Additionally, I just implemented a fix to automatically install all required dependencies when pip installing this
+      package. This should fix many issues for Linux users, if not all the current ones. Note that if you want to use
+      the
+      GUI, read the next point.
+    - Still submit an issue using the link above if this is the case -> in theory I can detect most of these
 
 2. Did not install GUI version: To enable the ability to use the graphical-user-interface (GUI) you must:
 
-    `pip install propeller_design_tools[gui]` - or - `pip install --upgrade propeller_design_tools[gui]`
+   `pip install propeller_design_tools[gui]` - or - `pip install --upgrade propeller_design_tools[gui]`
 
-3. You're asking for an "impossible" propeller: XROTOR will error in this case.  
-   - Impossible in terms of the pure physics of what you're asking for (asking for too much thrust / power essentially)
-   - PDT has no way to know if your propeller is impossible, so I'm not sure how I could ever wrap this error in an 
-     appropriate python error wrapper even.
-   - I highly recommend to use only the "constant" blade cl distribution target option
-     - I have not had time yet to test any of the other options much
-     - Other options are disabled in the GUI until I can test them fully
-     - Other options in the future will be a "linear" option as well as "file" option (which essentially allows the 
-     - user to define an arbitrary, discreet function for the blade Cl distribution).
-   - It is also highly recommended to use only the 'grad' or 'pot' solver options until you know you have the code at 
-     least generating an output without failing. 
-     - I would only then recommend moving on to using the 'vrtx' solver. This solver is (in my opinion) the superior of 
-       the 3 options. Though it takes longest to solve by far, it seems to be the only one that reliably produces 
-       reasonable chord lengths near the hub. I think the 'vrtx' solver is somewhat less stable than the other two as 
-       well, so if you think you're having errors with PDT try to switch solvers.
+3. You're asking for an "impossible" propeller: XROTOR will error in this case.
+    - Impossible in terms of the pure physics of what you're asking for (asking for too much thrust / power essentially)
+    - PDT has no way to know if your propeller is impossible, so I'm not sure how I could ever wrap this error in an
+      appropriate python error wrapper even.
+    - I highly recommend to use only the "constant" blade cl distribution target option
+        - I have not had time yet to test any of the other options much
+        - Other options are disabled in the GUI until I can test them fully
+        - Other options in the future will be a "linear" option as well as "file" option (which essentially allows the
+        - user to define an arbitrary, discreet function for the blade Cl distribution).
+    - It is also highly recommended to use only the 'grad' or 'pot' solver options until you know you have the code at
+      least generating an output without failing.
+        - I would only then recommend moving on to using the 'vrtx' solver. This solver is (in my opinion) the superior
+          of
+          the 3 options. Though it takes longest to solve by far, it seems to be the only one that reliably produces
+          reasonable chord lengths near the hub. I think the 'vrtx' solver is somewhat less stable than the other two as
+          well, so if you think you're having errors with PDT try to switch solvers.
 
 4. You're asking for XFOIL to analyze your airfoil at too low or too high of an angle-of-attack (AoA)
-   - I have attempted to remove the need for the user to enter AoA, but my algorithm for this is far from perfect.
-   - If you think this is your error, please submit it via issue link above.
+    - I have attempted to remove the need for the user to enter AoA, but my algorithm for this is far from perfect.
+    - If you think this is your error, please submit it via issue link above.
 
 5. You're trying to open the STL file generated by PDT in SolidWorks: this is a known issue currently being worked on.
    - I've no idea why this happens, it seems to be a purely SolidWorks issue, the STL file seems to open just fine in
      everything else I have tried.
    - Try opening the file and re-saving it (I suggest MS Paint, I think the new version can save STLs).
    - Try opening the file and re-saving it after having very slightly changed it.
    - If you encounter this error but think you have figured it out or have useful information about it please submit an
      issue via the link above.
 
 Thank you all that is my TED talk.
 
+---
 Purpose
 =======
 PDT seeks to provide the user a set of python3 utilities that can be used for arbitrary scripting efforts to automate
 usage of both XFOIL and XROTOR while implementing its own unique python3-native algorithms to maintain local
 input files, meta files, databases, and results files and weave everything together for the user in a simple,
 meaningful way to aid in the initial / investigatory stage of well-behaved propeller designs (free-flow and non-ducted
 assumptions).
 
+---
 Getting Started
 ===============
 Installation
 ------------
 `pip install propeller_design_tools` - or - `pip install propeller_design_tools[gui]`
 
 Update
@@ -842,20 +807,21 @@
 `pdt.set_propeller_database(path: str)`
 
 **The user must set these two directories at the top of every script right after the imports**
 
 *The airfoil directory will be used to store any foil / XFOIL-related support files, and the propeller directory
 will be used similarly to store any propeller / XROTOR-related support files.*
 
+---
 Example Scripts / Workflow
 --------------------------
 At a high-level, the current concept for the PDT workflow is as follows (after pip-installing the PDT package):
 
 0. Try out the (currently extremely buggy and incomplete) user interface!
-[example0_user_interface.py](
+   [example0_user_interface.py](
    https://github.com/helloDestroyerOfWorlds/propeller_design_tools/blob/master/tests/example0_user_interface.py)
 
    ![ex0-1](./tests/ex0-1.png)
    ![ex0-2](./tests/ex0-2.png)
    ![ex0-3](./tests/ex0-3.png)
 
 
@@ -903,21 +869,63 @@
 [example4_stl_generation.py](
    https://github.com/helloDestroyerOfWorlds/propeller_design_tools/blob/master/tests/example4_stl_generation.py
    )
 
    ![ex4-1](./tests/ex4-1.png)
 
 
-5. Analyze a given `Propeller()` instance across a sweep of operating points -> see 
-[example5_prop_analysis.py](
+5. Analyze a given `Propeller()` instance across a sweep of operating points -> see
+   [example5_prop_analysis.py](
    https://github.com/helloDestroyerOfWorlds/propeller_design_tools/blob/master/tests/example5_prop_analysis.py
    )
 
    ![ex5-1](./tests/ex5-1.png)
 
 
-6. **WIP** Prop optimization 
-   - Will be a grid-search style generic optimizer for "optimal" prop design generation by means of minimizing overall 
-     energy usage. 
-   - Optionally takes into account different propeller operating points via the ability to define the propeller's 
-     "duty-cycle"
-     - This feature is coming soon! 
+6. **WIP** Prop optimization
+    - Will be a grid-search style generic optimizer for "optimal" prop design generation by means of minimizing overall
+      energy usage.
+    - Optionally takes into account different propeller operating points via the ability to define the propeller's
+      "duty-cycle"
+        - This feature is coming soon!
+
+---
+XFOIL, XROTOR and other MIT Aero-Modeling Executables
+-----------------------------------------------------
+In order to utilize any PDT functionality that depends on
+running XFOIL, the "xfoil.exe" executable file needs to be
+in the user-set "airfoil_database" location. *Current pip
+installations include the xfoil.exe file in the foil_database,
+there should theoretically be no need to download it manually,
+even if the user changes the foil_database location.*
+
+[XFOIL executable and docs](https://web.mit.edu/drela/Public/web/xfoil/)
+
+Likewise, in order to utilize any PDT functionality that
+depends on running XROTOR, the "xrotor.exe" executable file
+needs to be in the user-set "propeller_database" location.
+*Current pip installations include the xrotor.exe file in the
+default prop_database, there should theoretically be no need to
+download it manually, even if the user changes the prop_database
+location.*
+
+[CROTOR executable and docs](http://www.esotec.org/sw/crotor.html#download)
+*(this is actually a link to "CROTOR", which I find is
+the easiest way to obtain a windows-executable of XROTOR)*
+
+[actual XROTOR docs](https://web.mit.edu/drela/Public/web/xrotor/xrotor_doc.txt)
+
+Both XFOIL and XROTOR contain much, much more utility than PDT currently has integrated. They are part of an incredible
+set of aerodynamic (or hydrodynamic) modeling command-line-interface (CLI) utilities from MIT. The ones that I
+personally know of include:
+
+1. XFOIL - for arbitrary 2D airfoil analysis and design
+2. XROTOR - for arbitrary propeller design schemes and analysis
+3. AVL - for arbitrary lifting planform analysis
+4. QPROP - another CLI utility for propeller design and analysis
+5. QMIL - for arbitrary windmill designs (and more)
+
+Combined, the above represents an amazing fluid-dynamics modeling capability that is completely free, and fast. While
+it's unlikely they will ever get as accurate as true computational-fluid-dynamics (CFD) software, they still offer
+great value for being free, and are several orders of magnitude faster than true CFD software. Personally, I have found
+them to be completely sufficient tools for all stages of engineering design, but then again I have only ever worked in
+prototyping engineering.
```

### Comparing `propeller_design_tools-0.4.6/README.md` & `propeller_design_tools-0.4.7/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -3,131 +3,96 @@
 ---
 **Work in progress / incomplete documentation (all current documentation is below, as well as a step-by-step typical 
 usage/workflow scenario)**
 
 Note: The graphical user interface for this should be functional for Linux now as well!
 
 ---
-
 Description
 ===========
 Python 3.7 package that provides exactly what it sounds like by automating usage of the GPL-licensed 
 CLI-utilities XFOIL and XROTOR.
 
 Both utilities are published by professor Mark Drela (MIT).
+
 - XFOIL: for arbitrary 2D airfoil analysis and design
 - XROTOR: for arbitrary propeller design schemes and analysis
 
-XFOIL and XROTOR Executables
--------------------------------------------
-In order to utilize any PDT functionality that depends on
-running XFOIL, the "xfoil.exe" executable file needs to be
-in the user-set "airfoil_database" location. *Current pip
-installations include the xfoil.exe file in the foil_database,
-there should theoretically be no need to download it manually,
-even if the user changes the foil_database location.*
-
-[XFOIL executable and docs](https://web.mit.edu/drela/Public/web/xfoil/)
-
-Likewise, in order to utilize any PDT functionality that
-depends on running XROTOR, the "xrotor.exe" executable file
-needs to be in the user-set "propeller_database" location.
-*Current pip installations include the xrotor.exe file in the
-default prop_database, there should theoretically be no need to
-download it manually, even if the user changes the prop_database
-location.*
-
-[CROTOR executable and docs](http://www.esotec.org/sw/crotor.html#download)
-*(this is actually a link to "CROTOR", which I find is
-the easiest way to obtain a windows-executable of XROTOR)*
-
-[actual XROTOR docs](https://web.mit.edu/drela/Public/web/xrotor/xrotor_doc.txt)
-
-Both XFOIL and XROTOR contain much, much more utility than PDT currently has integrated. They are part of an incredible
-set of aerodynamic (or hydrodynamic) modeling command-line-interface (CLI) utilities from MIT. The ones that I 
-personally know of include:
-1. XFOIL - for arbitrary 2D airfoil analysis and design
-2. XROTOR - for arbitrary propeller design schemes and analysis
-3. AVL - for arbitrary lifting planform analysis
-4. QPROP - another CLI utility for propeller design and analysis
-5. QMIL - for arbitrary windmill designs (and more)
-
-Combined, the above represents an amazing fluid-dynamics modeling capability that is completely free, and fast. While 
-it's unlikely they will ever get as accurate as true computational-fluid-dynamics (CFD) software, they still offer 
-great value for being free, and are several orders of magnitude faster than true CFD software. Personally, I have found
-them to be completely sufficient tools for all stages of engineering design, but then again I have only ever worked in 
-prototyping engineering.
-
+---
 Troubleshooting PDT Errors / Crashes (GUI and/or Scripting)
 ===========================================================
-So I just quit my job as a systems engineer to become a software developer, so hopefully this package starts to get 
+So I just quit my job as a systems engineer to become a software developer, so hopefully this package starts to get
 more frequent updates and support from me. If you encounter what you think is an error coming from this code, I would
 love to know about it, please submit an issue to:
 
 [LINK TO GITHUB ISSUES](https://github.com/helloDestroyerOfWorlds/propeller_design_tools/issues)
 
-and I will likely see it quickly and will at least answer you, if not just fix it and push the update. Please only do 
+and I will likely see it quickly and will at least answer you, if not just fix it and push the update. Please only do
 this though once you are sure the error is coming from the PDT code.
 
-If you think you have discovered a legitimate issue, before submitting it please also read through the list below to 
+If you think you have discovered a legitimate issue, before submitting it please also read through the list below to
 see if any of the listed things could fix your error.
 
-1. XFOIL or XROTOR executables: Errors might be coming from XFOIL or XROTOR in actuality rather than this source code 
-   - Currently PDT implements these as executables installed when pip installing this package
-   - This means if you are having pip install errors and are on Linux it might be caused by that, actually, if you are 
-     having any errors, even in the GUI, and you are on Linux it might be caused by me not understanding until now much 
-     about Linux. If this is the case, and you think you know what is causing the error, please feel free to reach out 
-     to me via the issues link above.
-   - Additionally, I just implemented a fix to automatically install all required dependencies when pip installing this 
-     package. This should fix many issues for Linux users, if not all the current ones. Note that if you want to use the
-     GUI, read the next point.
-   - Still submit an issue using the link above if this is the case -> in theory I can detect most of these
+1. XFOIL or XROTOR executables: Errors might be coming from XFOIL or XROTOR in actuality rather than this source code
+    - Currently PDT implements these as executables installed when pip installing this package
+    - This means if you are having pip install errors and are on Linux it might be caused by that, actually, if you are
+      having any errors, even in the GUI, and you are on Linux it might be caused by me not understanding until now much
+      about Linux. If this is the case, and you think you know what is causing the error, please feel free to reach out
+      to me via the issues link above.
+    - Additionally, I just implemented a fix to automatically install all required dependencies when pip installing this
+      package. This should fix many issues for Linux users, if not all the current ones. Note that if you want to use
+      the
+      GUI, read the next point.
+    - Still submit an issue using the link above if this is the case -> in theory I can detect most of these
 
 2. Did not install GUI version: To enable the ability to use the graphical-user-interface (GUI) you must:
 
-    `pip install propeller_design_tools[gui]` - or - `pip install --upgrade propeller_design_tools[gui]`
+   `pip install propeller_design_tools[gui]` - or - `pip install --upgrade propeller_design_tools[gui]`
 
-3. You're asking for an "impossible" propeller: XROTOR will error in this case.  
-   - Impossible in terms of the pure physics of what you're asking for (asking for too much thrust / power essentially)
-   - PDT has no way to know if your propeller is impossible, so I'm not sure how I could ever wrap this error in an 
-     appropriate python error wrapper even.
-   - I highly recommend to use only the "constant" blade cl distribution target option
-     - I have not had time yet to test any of the other options much
-     - Other options are disabled in the GUI until I can test them fully
-     - Other options in the future will be a "linear" option as well as "file" option (which essentially allows the 
-     - user to define an arbitrary, discreet function for the blade Cl distribution).
-   - It is also highly recommended to use only the 'grad' or 'pot' solver options until you know you have the code at 
-     least generating an output without failing. 
-     - I would only then recommend moving on to using the 'vrtx' solver. This solver is (in my opinion) the superior of 
-       the 3 options. Though it takes longest to solve by far, it seems to be the only one that reliably produces 
-       reasonable chord lengths near the hub. I think the 'vrtx' solver is somewhat less stable than the other two as 
-       well, so if you think you're having errors with PDT try to switch solvers.
+3. You're asking for an "impossible" propeller: XROTOR will error in this case.
+    - Impossible in terms of the pure physics of what you're asking for (asking for too much thrust / power essentially)
+    - PDT has no way to know if your propeller is impossible, so I'm not sure how I could ever wrap this error in an
+      appropriate python error wrapper even.
+    - I highly recommend to use only the "constant" blade cl distribution target option
+        - I have not had time yet to test any of the other options much
+        - Other options are disabled in the GUI until I can test them fully
+        - Other options in the future will be a "linear" option as well as "file" option (which essentially allows the
+        - user to define an arbitrary, discreet function for the blade Cl distribution).
+    - It is also highly recommended to use only the 'grad' or 'pot' solver options until you know you have the code at
+      least generating an output without failing.
+        - I would only then recommend moving on to using the 'vrtx' solver. This solver is (in my opinion) the superior
+          of
+          the 3 options. Though it takes longest to solve by far, it seems to be the only one that reliably produces
+          reasonable chord lengths near the hub. I think the 'vrtx' solver is somewhat less stable than the other two as
+          well, so if you think you're having errors with PDT try to switch solvers.
 
 4. You're asking for XFOIL to analyze your airfoil at too low or too high of an angle-of-attack (AoA)
-   - I have attempted to remove the need for the user to enter AoA, but my algorithm for this is far from perfect.
-   - If you think this is your error, please submit it via issue link above.
+    - I have attempted to remove the need for the user to enter AoA, but my algorithm for this is far from perfect.
+    - If you think this is your error, please submit it via issue link above.
 
 5. You're trying to open the STL file generated by PDT in SolidWorks: this is a known issue currently being worked on.
    - I've no idea why this happens, it seems to be a purely SolidWorks issue, the STL file seems to open just fine in
      everything else I have tried.
    - Try opening the file and re-saving it (I suggest MS Paint, I think the new version can save STLs).
    - Try opening the file and re-saving it after having very slightly changed it.
    - If you encounter this error but think you have figured it out or have useful information about it please submit an
      issue via the link above.
 
 Thank you all that is my TED talk.
 
+---
 Purpose
 =======
 PDT seeks to provide the user a set of python3 utilities that can be used for arbitrary scripting efforts to automate
 usage of both XFOIL and XROTOR while implementing its own unique python3-native algorithms to maintain local
 input files, meta files, databases, and results files and weave everything together for the user in a simple,
 meaningful way to aid in the initial / investigatory stage of well-behaved propeller designs (free-flow and non-ducted
 assumptions).
 
+---
 Getting Started
 ===============
 Installation
 ------------
 `pip install propeller_design_tools` - or - `pip install propeller_design_tools[gui]`
 
 Update
@@ -145,20 +110,21 @@
 `pdt.set_propeller_database(path: str)`
 
 **The user must set these two directories at the top of every script right after the imports**
 
 *The airfoil directory will be used to store any foil / XFOIL-related support files, and the propeller directory
 will be used similarly to store any propeller / XROTOR-related support files.*
 
+---
 Example Scripts / Workflow
 --------------------------
 At a high-level, the current concept for the PDT workflow is as follows (after pip-installing the PDT package):
 
 0. Try out the (currently extremely buggy and incomplete) user interface!
-[example0_user_interface.py](
+   [example0_user_interface.py](
    https://github.com/helloDestroyerOfWorlds/propeller_design_tools/blob/master/tests/example0_user_interface.py)
 
    ![ex0-1](./tests/ex0-1.png)
    ![ex0-2](./tests/ex0-2.png)
    ![ex0-3](./tests/ex0-3.png)
 
 
@@ -206,21 +172,63 @@
 [example4_stl_generation.py](
    https://github.com/helloDestroyerOfWorlds/propeller_design_tools/blob/master/tests/example4_stl_generation.py
    )
 
    ![ex4-1](./tests/ex4-1.png)
 
 
-5. Analyze a given `Propeller()` instance across a sweep of operating points -> see 
-[example5_prop_analysis.py](
+5. Analyze a given `Propeller()` instance across a sweep of operating points -> see
+   [example5_prop_analysis.py](
    https://github.com/helloDestroyerOfWorlds/propeller_design_tools/blob/master/tests/example5_prop_analysis.py
    )
 
    ![ex5-1](./tests/ex5-1.png)
 
 
-6. **WIP** Prop optimization 
-   - Will be a grid-search style generic optimizer for "optimal" prop design generation by means of minimizing overall 
-     energy usage. 
-   - Optionally takes into account different propeller operating points via the ability to define the propeller's 
-     "duty-cycle"
-     - This feature is coming soon! 
+6. **WIP** Prop optimization
+    - Will be a grid-search style generic optimizer for "optimal" prop design generation by means of minimizing overall
+      energy usage.
+    - Optionally takes into account different propeller operating points via the ability to define the propeller's
+      "duty-cycle"
+        - This feature is coming soon!
+
+---
+XFOIL, XROTOR and other MIT Aero-Modeling Executables
+-----------------------------------------------------
+In order to utilize any PDT functionality that depends on
+running XFOIL, the "xfoil.exe" executable file needs to be
+in the user-set "airfoil_database" location. *Current pip
+installations include the xfoil.exe file in the foil_database,
+there should theoretically be no need to download it manually,
+even if the user changes the foil_database location.*
+
+[XFOIL executable and docs](https://web.mit.edu/drela/Public/web/xfoil/)
+
+Likewise, in order to utilize any PDT functionality that
+depends on running XROTOR, the "xrotor.exe" executable file
+needs to be in the user-set "propeller_database" location.
+*Current pip installations include the xrotor.exe file in the
+default prop_database, there should theoretically be no need to
+download it manually, even if the user changes the prop_database
+location.*
+
+[CROTOR executable and docs](http://www.esotec.org/sw/crotor.html#download)
+*(this is actually a link to "CROTOR", which I find is
+the easiest way to obtain a windows-executable of XROTOR)*
+
+[actual XROTOR docs](https://web.mit.edu/drela/Public/web/xrotor/xrotor_doc.txt)
+
+Both XFOIL and XROTOR contain much, much more utility than PDT currently has integrated. They are part of an incredible
+set of aerodynamic (or hydrodynamic) modeling command-line-interface (CLI) utilities from MIT. The ones that I
+personally know of include:
+
+1. XFOIL - for arbitrary 2D airfoil analysis and design
+2. XROTOR - for arbitrary propeller design schemes and analysis
+3. AVL - for arbitrary lifting planform analysis
+4. QPROP - another CLI utility for propeller design and analysis
+5. QMIL - for arbitrary windmill designs (and more)
+
+Combined, the above represents an amazing fluid-dynamics modeling capability that is completely free, and fast. While
+it's unlikely they will ever get as accurate as true computational-fluid-dynamics (CFD) software, they still offer
+great value for being free, and are several orders of magnitude faster than true CFD software. Personally, I have found
+them to be completely sufficient tools for all stages of engineering design, but then again I have only ever worked in
+prototyping engineering.
```

### Comparing `propeller_design_tools-0.4.6/propeller_design_tools/airfoil.py` & `propeller_design_tools-0.4.7/propeller_design_tools/airfoil.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,40 +1,43 @@
 import os
 import warnings
+
+import matplotlib
+
 from propeller_design_tools import funcs
-from propeller_design_tools.user_io import Error, Info, Warning
 from propeller_design_tools.settings import get_foil_db
-import matplotlib
+from propeller_design_tools.user_io import DTError, DTInfo, DTWarning
+
 matplotlib.use('TKAgg')
 import matplotlib.pyplot as plt
 import numpy as np
 from scipy.interpolate import griddata, interp1d
 
 
 class Airfoil(object):
     def __init__(self, name: str, exact_namematch: bool = False, verbose: bool = True):
         name_in = name
         if '.' in name_in:
             name, ext = os.path.splitext(name_in)
             if not any([ex in ext.lower() for ex in ['.dat', '.txt']]):
-                raise Error('Only files with either ".dat" or ".txt" extensions may be used as airfoil '
+                raise DTError('Only files with either ".dat" or ".txt" extensions may be used as airfoil '
                               'coordinate files ({})'.format(name_in))
             else:
                 self.name = name
         else:
             self.name = name_in
 
         # check for foil database existence
         if get_foil_db() is None:
-            raise Error('No airfoil database set -> use "pdt.set_airfoil_database(str)" to set one.')
+            raise DTError('No airfoil database set -> use "pdt.set_airfoil_database(str)" to set one.')
 
         # get the airfoil filename, filepath
         fname = funcs.get_airfoil_file_from_db(self.name, exact_namematch=exact_namematch)
         if verbose:
-            Info('Found airfoil coordinate file: {}'.format(fname))
+            DTInfo('Found airfoil coordinate file: {}'.format(fname))
         self.coord_fpath = os.path.join(get_foil_db(), fname)
 
         name, x_coords, y_coords = funcs.read_airfoil_coordinate_file(fpath=self.coord_fpath, verbose=verbose)
         _, xc_closed_te, yc_closed_te = funcs.read_airfoil_coordinate_file(fpath=self.coord_fpath, verbose=False,
                                                                            te_gap_set=0.0)
         self.filename = os.path.basename(self.coord_fpath)
         self.x_coords = np.array(x_coords)
@@ -92,15 +95,15 @@
         ax.set_title(self.filename)
 
         return fig
 
     def alpha_auto_range(self, re: int, ncrit: int, mach: float, verbose: bool = True, xfoil_verbose: bool = False,
                          hide_windows: bool = True):
         if verbose:
-            Info('Detecting range for alpha sweep, finding zero-lift angle-of-attack...')
+            DTInfo('Detecting range for alpha sweep, finding zero-lift angle-of-attack...')
 
         def find_alpha_CL0():   # function to find zero lift aoa (A0deg)
             funcs.run_xfoil(foil_relpath=self.xfoil_relpath, re=re, cl=[0], ncrit=ncrit, mach=mach,
                             hide_windows=hide_windows, verbose=xfoil_verbose)
             xout = funcs.read_xfoil_pacc_file(delete_after=True)
             if xout is not None:    # just return if xfoil converged 1st try
                 return xout['alpha'][0]
@@ -112,27 +115,27 @@
             while xout is None:  # get an upper data point
                 cl += clinc
                 funcs.run_xfoil(foil_relpath=self.xfoil_relpath, re=re, cl=[cl], ncrit=ncrit, mach=mach,
                                 keypress_iternum=10, hide_windows=hide_windows, verbose=xfoil_verbose)
                 xout = funcs.read_xfoil_pacc_file(delete_after=True)
                 if xout is None and cl == cl_lim:
                     err_txt = 'Unable to find alpha @ CL0 (foil={}, re={:.0f})'.format(self.name, re)
-                    raise Error(err_txt)
+                    raise DTError(err_txt)
             a_up = xout['alpha'][0]
             cl_up = xout['CL'][0]
 
             cl = 0
             xout = None
             while xout is None:  # get a lower data point
                 cl -= clinc
                 funcs.run_xfoil(foil_relpath=self.xfoil_relpath, re=re, cl=[cl], ncrit=ncrit, mach=mach,
                                 keypress_iternum=10, hide_windows=hide_windows, verbose=xfoil_verbose)
                 xout = funcs.read_xfoil_pacc_file(delete_after=True)
                 if xout is None and cl == -cl_lim:
-                    raise Error('Unable to find alpha @ CL0 (foil={}, re={:.0f})'.format(self.name, re))
+                    raise DTError('Unable to find alpha @ CL0 (foil={}, re={:.0f})'.format(self.name, re))
 
             a_low = xout['alpha'][0]
             cl_low = xout['CL'][0]
 
             da_dcl = (a_up - a_low) / (cl_up - cl_low)
             dcl = 0 - cl_low
             A0deg = a_low + dcl * da_dcl
@@ -165,31 +168,31 @@
 
             if len(aa) > 0:     # made it to a_max, but converged at least once
                 return aa[-1] + 2
             else:   # made it all the way to max_a without converging
                 # trace_txt = 'Airfoil.alpha_auto_range.find_stall_angle()'
                 # err_txt = 'Unable to find stall angle, max_a reached (foil={}, re={:.0f})'.format(self.name, re)
                 #
-                # info_d = {'func/method': trace_txt, 'Error Text': err_txt, 'dclda_threshold':
+                # info_d = {'func/method': trace_txt, 'DTError Text': err_txt, 'dclda_threshold':
                 #     dclda_threshold, 'start_a': start_a, 'ainc': ainc, 'max_a': max_a}
                 # errplot_kwargs = {'x': aa, 'y': cl, 'xlbl': 'alpha (deg)', 'ylbl': 'CL', 'info_d': info_d}
-                # raise Error(err_txt, **errplot_kwargs)
+                # raise DTError(err_txt, **errplot_kwargs)
                 return max_a
 
         # use the functions above
         zero_lift_aoa = find_alpha_CL0()
         if verbose:
-            Info('Found alpha_CL0 = {}'.format(zero_lift_aoa), indent_level=1)
-            Info('Approximating stall angle...', indent_level=1)
+            DTInfo('Found alpha_CL0 = {}'.format(zero_lift_aoa), indent_level=1)
+            DTInfo('Approximating stall angle...', indent_level=1)
         a_stall = find_stall_angle(start_a=zero_lift_aoa + 12)
         if verbose:
-            Info('Found a_stall = {}'.format(a_stall), indent_level=1)
+            DTInfo('Found a_stall = {}'.format(a_stall), indent_level=1)
         alpha = np.arange(zero_lift_aoa - 1, a_stall + 2.5, 0.5)
         if verbose:
-            Info('Determined alpha values: {}'.format(alpha))
+            DTInfo('Determined alpha values: {}'.format(alpha))
 
         return alpha
 
     def calculate_xfoil_polars(self, hide_windows: bool = True, verbose: bool = True, xfoil_verbose: bool = False,
                                **kwargs):
         """
         Used to interface with XFOIL and save database data.
@@ -213,15 +216,15 @@
 
         # KWARG conditioning
         if 're' in kwargs:
             re_list = kwargs.pop('re')
             if not isinstance(re_list, list):
                 re_list = list(re_list)
         else:
-            raise Error('Must input a value for KWARG "re"')
+            raise DTError('Must input a value for KWARG "re"')
 
         if 'alpha' in kwargs:
             alpha_list = kwargs.pop('alpha')
             if not isinstance(alpha_list, list):
                 if alpha_list is not None:
                     alpha_list = list(alpha_list)
         else:
@@ -231,15 +234,15 @@
             ncrit_list = kwargs.pop('ncrit')
             if not isinstance(ncrit_list, list):
                 ncrit_list = list(ncrit_list)
         else:
             ncrit_list = [9]  # default
         for nc in ncrit_list:        # check ncrit in range
             if nc not in range(4, 15):
-                raise Error('Parameter ncrit must be an integer 4-14 (got {})'.format(nc))
+                raise DTError('Parameter ncrit must be an integer 4-14 (got {})'.format(nc))
 
         if 'mach' in kwargs:
             mach_list = kwargs.pop('mach')
             if not isinstance(mach_list, list):
                 mach_list = list(mach_list)
         else:
             mach_list = [0.0]  # default
@@ -255,62 +258,62 @@
         for ncrit in ncrit_list:
             for mach in mach_list:
                 for re in re_list:
                     count += 1
                     re = int(re)
                     if verbose:
                         print()
-                        Info('Running polar # {} / {} (Re={}, mach={}, ncrit={}) ...'.format(count, total_count, re,
-                                                                                             mach, ncrit))
+                        DTInfo('Running polar # {} / {} (Re={}, mach={}, ncrit={}) ...'.format(count, total_count, re,
+                            mach, ncrit))
 
                     if alpha_in is None:
                         alpha_list = self.alpha_auto_range(re=re, ncrit=ncrit, mach=mach, verbose=verbose,
                                                            xfoil_verbose=xfoil_verbose, hide_windows=hide_windows)
 
                     if verbose:
-                        Info('Running XFOIL for:')
-                        Info('Foil: {}'.format(self.name), indent_level=1)
-                        Info('Re: {}'.format(re), indent_level=1)
-                        Info('Mach: {}'.format(mach), indent_level=1)
-                        Info('Ncrit: {}'.format(ncrit), indent_level=1)
-                        Info('alpha: {}'.format(alpha_list), indent_level=1)
+                        DTInfo('Running XFOIL for:')
+                        DTInfo('Foil: {}'.format(self.name), indent_level=1)
+                        DTInfo('Re: {}'.format(re), indent_level=1)
+                        DTInfo('Mach: {}'.format(mach), indent_level=1)
+                        DTInfo('Ncrit: {}'.format(ncrit), indent_level=1)
+                        DTInfo('alpha: {}'.format(alpha_list), indent_level=1)
                     funcs.run_xfoil(foil_relpath=self.xfoil_relpath, re=re, alpha=alpha_list, ncrit=ncrit,
                                     mach=mach, verbose=xfoil_verbose, hide_windows=hide_windows)
                     if verbose:
-                        Info('Done')
+                        DTInfo('Done')
 
                     d = funcs.read_xfoil_pacc_file(delete_after=True)
                     self.polar_data[(re, mach, ncrit)] = d
 
         # exit method if not saving to database
         if not save_to_database:
             return
 
         # save/append to database, start by making folder if it doesn't already exist
         database_folder = os.path.join(get_foil_db(), 'polar_database')
         if not os.path.exists(database_folder):
             os.mkdir(database_folder)
             if verbose:
-                Info('Created a "polar_database" to store XFOIL results')
+                DTInfo('Created a "polar_database" to store XFOIL results')
 
         # savename will be coordinate file name with _polar_data appended
         savepath = self.get_database_savepath()
 
         # append/overwrite data if file exists already, otherwise write data to a new file
         if os.path.exists(savepath):
             if verbose:
-                Info('Detected existing polar data for "{}" -> merging datasets'.format(self.name))
+                DTInfo('Detected existing polar data for "{}" -> merging datasets'.format(self.name))
             old_polar_data = funcs.read_polar_data_file(fpath=savepath)
             merged = funcs.merge_polar_data_dicts(new=self.polar_data.copy(), old=old_polar_data)
             os.remove(savepath)
             funcs.save_polar_data_file(polar_data=merged, savepath=savepath, name=self.name)
         else:
             funcs.save_polar_data_file(polar_data=self.polar_data, savepath=savepath, name=self.name)
         if verbose:
-            Info('Saved new polar data for "{}"'.format(self.name))
+            DTInfo('Saved new polar data for "{}"'.format(self.name))
 
     def get_valid_xfoil_params(self):
         return ['alpha', 'CL', 'CD', 'CDp', 'CM', 'Top_Xtr', 'Bot_Xtr', 'CL/CD']
 
     def plot_polar_data(self, x_param: str, y_param: str, re_list: list = None, mach_list: list = None,
                         ncrit_list: list = None, xlims: tuple = None, ylims: tuple = None, rectified: bool = False,
                         rect_kwargs: dict = {}, fig=None, **plot_kwargs):
@@ -329,24 +332,24 @@
         :param rectified: bool, whether or not to plot the raw grid data, or rectify it first and plot that data
         :param rect_kwargs: dictionary, the key-word arguments to pass along to rectify_polar_grids
 
         :return fig: the pyplot.fig instance of the plot
         :return ax: the pyplot.axes instance of the plot
         """
         if x_param not in self.get_valid_xfoil_params() or y_param not in self.get_valid_xfoil_params():
-            raise Error('"{}" is not a valid polar parameter combo for plotting'.
-                          format('({}, {})'.format(x_param, y_param)))
+            raise DTError('"{}" is not a valid polar parameter combo for plotting'.
+            format('({}, {})'.format(x_param, y_param)))
 
         pol_data = self.polar_data
         if rectified:
             self.rectify_polar_grids(rect_kwargs=rect_kwargs)
             pol_data = self.rectified_polar_data
 
         if len(pol_data) == 0:
-            raise Error('No polar data to plot for "{}"! Use "calculate_xfoil_polars()" first'.format(self.name))
+            raise DTError('No polar data to plot for "{}"! Use "calculate_xfoil_polars()" first'.format(self.name))
 
         if 'marker' not in plot_kwargs:
             plot_kwargs['marker'] = 'o'
 
         # get the grid of polar lookup keys for the associated polar data
         re_l, mach_l, ncrit_l = self.get_polar_data_grid()
 
@@ -384,16 +387,16 @@
                 for ncrit_key in ncrit_list:
                     marker_cycle = ['o', 'v', '^', '<', '>', 's', '+', 'd', '2']
                     plot_kwargs['marker'] = marker_cycle[ncrit_list.index(ncrit_key) % len(marker_cycle)]
                     if (re_key, mach_key, ncrit_key) in pol_data.keys():
                         d = pol_data[(re_key, mach_key, ncrit_key)]
                         ax.plot(d[x_param], d[y_param], label='{:.1e}, {}, {}'.format(re_key, mach_key, ncrit_key), **plot_kwargs)
                     else:
-                        Warning('Cannot find polar for {} @ Re = {}, Mach = {}, Ncrit = {}, skipping this one...'
-                                .format(self.name, re_key, mach_key, ncrit_key))
+                        DTWarning('Cannot find polar for {} @ Re = {}, Mach = {}, Ncrit = {}, skipping this one...'
+                        .format(self.name, re_key, mach_key, ncrit_key))
 
         ax.grid(True)
         ax.set_title('{}\nrectified={}'.format(self.filename, rectified))
         ax.set_xlabel(x_param)
         ax.set_ylabel(y_param)
         if ylims is not None:
             ax.set_ylim(ylims)
@@ -448,19 +451,20 @@
 
         self.rectified_polar_data = rect_polar_data
 
     def interpolate_polar(self, npts: int, re: int, mach: float, ncrit: int, griddata_kwargs: dict = {}):
         # check for inside convex hull of known (Re, Mach, nCrit) grid points
         res, machs, ncrits = self.get_polar_data_grid()
         if re > max(res) or re < min(res):
-            raise Error('Cannot interpolate a polar @ re value outside database limits (re={:.0f})'.format(re))
+            raise DTError('Cannot interpolate a polar @ re value outside database limits (re={:.0f})'.format(re))
         if mach > max(machs) or re < min(machs):
-            raise Error('Cannot interpolate a polar @ mach value outside database limits (mach={:.2f})'.format(mach))
+            raise DTError('Cannot interpolate a polar @ mach value outside database limits (mach={:.2f})'.format(mach))
         if ncrit > max(ncrits) or re < min(ncrits):
-            raise Error('Cannot interpolate a polar @ ncrit value outside database limits (ncrit={:.0f})'.format(ncrit))
+            raise DTError(
+                'Cannot interpolate a polar @ ncrit value outside database limits (ncrit={:.0f})'.format(ncrit))
 
         if 'method' not in griddata_kwargs:
             griddata_kwargs['method'] = 'linear'
         if 'rescale' not in griddata_kwargs:
             griddata_kwargs['rescale'] = True
 
         # send em right back if their desired polar is one of the grid points
@@ -567,30 +571,30 @@
 
     def load_polar_data(self, verbose: bool = True):
         savepath = self.get_database_savepath()
         if os.path.exists(savepath):
             self.polar_data = funcs.read_polar_data_file(fpath=savepath)
             re, mach, ncrit = self.get_polar_data_grid()
             if verbose:
-                Info('Loaded existing polar data for "{}":'.format(self.name))
-                Info('Re={}\nMach={}\nNcrit={}'.format(re, mach, ncrit), indent_level=1)
+                DTInfo('Loaded existing polar data for "{}":'.format(self.name))
+                DTInfo('Re={}\nMach={}\nNcrit={}'.format(re, mach, ncrit), indent_level=1)
         else:
-            raise Error('Could not find polar data file: {}'.format(savepath))
+            raise DTError('Could not find polar data file: {}'.format(savepath))
 
     def get_coords(self, n_interp: int = None):
         if n_interp is None:
             return np.vstack([self.x_coords, self.y_coords])
         else:
-            raise Error('Code to interpolate more profile points is incomplete...')
+            raise DTError('Code to interpolate more profile points is incomplete...')
 
     def get_coords_closed_te(self, n_interp: int = None):
         if n_interp is None:
             return np.vstack([self.xc_closed_te, self.yc_closed_te])
         else:
-            raise Error('Code to interpolate more profile points is incomplete...')
+            raise DTError('Code to interpolate more profile points is incomplete...')
 
     def plot_2D_trimesh(self):
         fig = self.plot_geometry()
         ax = fig.axes[0]
 
         vectors = funcs.compute_profile_trimesh(profile_coords=self.get_coords())
         for vector in vectors:
```

### Comparing `propeller_design_tools-0.4.6/propeller_design_tools/custom_opengl_classes.py` & `propeller_design_tools-0.4.7/propeller_design_tools/custom_opengl_classes.py`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.6/propeller_design_tools/foil_database/arad13.dat` & `propeller_design_tools-0.4.7/propeller_design_tools/foil_database/arad13.dat`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.6/propeller_design_tools/foil_database/clarky.dat` & `propeller_design_tools-0.4.7/propeller_design_tools/foil_database/clarky.dat`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.6/propeller_design_tools/foil_database/e855.dat` & `propeller_design_tools-0.4.7/propeller_design_tools/foil_database/e855.dat`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.6/propeller_design_tools/foil_database/hs1606.dat` & `propeller_design_tools-0.4.7/propeller_design_tools/foil_database/hs1606.dat`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.6/propeller_design_tools/foil_database/mrc-16.dat` & `propeller_design_tools-0.4.7/propeller_design_tools/foil_database/mrc-16.dat`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.6/propeller_design_tools/foil_database/xfoil.exe` & `propeller_design_tools-0.4.7/propeller_design_tools/foil_database/xfoil.exe`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.6/propeller_design_tools/foil_ui_classes.py` & `propeller_design_tools-0.4.7/propeller_design_tools/foil_ui_classes.py`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.6/propeller_design_tools/funcs.py` & `propeller_design_tools-0.4.7/propeller_design_tools/funcs.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 import os
-import subprocess
 import shutil
+import subprocess
 import sys
 import urllib.request
 
 import matplotlib.pyplot as plt
 import numpy as np
+
 from propeller_design_tools.airfoil import Airfoil
-from propeller_design_tools.radialstation import RadialStation
 from propeller_design_tools.propeller import Propeller
-from propeller_design_tools.user_io import Info, Error, Warning
+from propeller_design_tools.radialstation import RadialStation
 from propeller_design_tools.settings import _get_user_settings, get_prop_db, get_foil_db
+from propeller_design_tools.user_io import DTInfo, DTError, DTWarning
 
 
 # =============== CONVENIENCE / UTILITY FUNCTIONS ===============
 def delete_propeller(prop, verbose: bool = True):
     fpaths = [prop.xrr_file, prop.xrop_file, prop.meta_file]
     rmvd = []
     for path in fpaths:
         if os.path.isfile(path):
             os.remove(path)
             rmvd.append(path)
     if verbose:
-        Info('Removed paths: {}'.format(rmvd))
+        DTInfo('Removed paths: {}'.format(rmvd))
 
 
 def clear_foil_database(single_foil: str = None, inside_root_db: bool = False, inside_polar_db: bool = True,
                         inside_for_xfoil: bool = True, verbose: bool = True):
     """
     Helper function to clear out files from foil database.
 
@@ -39,35 +40,35 @@
         single_foil = '{}.dat'.format(single_foil) if not single_foil.endswith('.dat') else single_foil
 
     foils_2_del = [single_foil] if single_foil is not None else get_all_airfoil_files()
 
     for foil_file in foils_2_del:
         foil_name = foil_file.replace('.dat', '')
         if verbose:
-            Info('Clearing files for "{}"'.format(foil_name))
+            DTInfo('Clearing files for "{}"'.format(foil_name))
 
         foil_fpath = os.path.join(_get_user_settings()['airfoil_database'], foil_file)
         polar_fpath = os.path.join(_get_user_settings()['airfoil_database'], 'polar_database', '{}_polar_data.txt'.format(foil_name))
         xfoil_fpath = os.path.join(_get_user_settings()['airfoil_database'], 'for_xfoil', '{}.txt'.format(foil_name))
 
         if inside_root_db:
             if os.path.exists(foil_fpath):
                 os.remove(foil_fpath)
                 if verbose:
-                    Info('Removed file "{}"'.format(foil_fpath), indent_level=1)
+                    DTInfo('Removed file "{}"'.format(foil_fpath), indent_level=1)
         if inside_polar_db:
             if os.path.exists(polar_fpath):
                 os.remove(polar_fpath)
                 if verbose:
-                    Info('Removed file "{}"'.format(polar_fpath), indent_level=1)
+                    DTInfo('Removed file "{}"'.format(polar_fpath), indent_level=1)
         if inside_for_xfoil:
             if os.path.exists(xfoil_fpath):
                 os.remove(xfoil_fpath)
                 if verbose:
-                    Info('Removed file "{}"'.format(xfoil_fpath), indent_level=1)
+                    DTInfo('Removed file "{}"'.format(xfoil_fpath), indent_level=1)
 
 
 def clear_prop_database(inside_root_db: bool = True, inside_xrotor_files: bool = True, inside_op_files: bool = True):
     """
     Helper function to clear out files from prop database.
 
     :param inside_op_files:
@@ -86,15 +87,15 @@
 def delete_files_from_folder(folder: str):
     if os.path.exists(folder):
         for filename in os.listdir(folder):
             fpath = os.path.join(folder, filename)
             if os.path.isfile(fpath):
                 os.remove(fpath)
     else:
-        raise Error('Cannot find folder: {}'.format(folder))
+        raise DTError('Cannot find folder: {}'.format(folder))
 
 
 def count_airfoil_db():
     return len(get_all_airfoil_files())
 
 
 def count_propeller_db():
@@ -129,15 +130,15 @@
     :param search_strs: a list of strings to search for in each filename
     :param contains_any: If True will return files that contain ANY of the search strings, defaults to False (returns only
         filenames that contain ALL of the search strings)
     :return: a list of filenames
     """
 
     if not os.path.exists(folder):
-        raise Error('PDT ERROR: No folder named "{}" found!'.format(folder))
+        raise DTError('PDT ERROR: No folder named "{}" found!'.format(folder))
 
     if include_dirs:
         files = os.listdir(folder)
     else:
         files = [f for f in os.listdir(folder) if os.path.isfile(os.path.join(folder, f))]
 
     if search_strs == []:
@@ -162,28 +163,28 @@
     if len(possible_files) == 1:
         if not exact_namematch:
             return possible_files[0]
         else:   # must match exactly
             if possible_files[0] == exact_fname:
                 return possible_files[0]
             else:
-                raise Error('Did not find an exact match for "{}"'.format(exact_fname))
+                raise DTError('Did not find an exact match for "{}"'.format(exact_fname))
 
     elif len(possible_files) == 0:
-        raise Error('Did not find any coordinate files containing name "{}" when looking in user-set airfoil '
-                    'database: {}'.format(foil_name, db_dir))
+        raise DTError('Did not find any coordinate files containing name "{}" when looking in user-set airfoil '
+                      'database: {}'.format(foil_name, db_dir))
 
     else:   # found multiple files
         if not exact_namematch:
-            raise Error('Found multiple coordinate files looking for airfoil "{}"!\n{}\n'
-                        'Consider using kwarg exact_namematch=True'.format(foil_name, possible_files))
+            raise DTError('Found multiple coordinate files looking for airfoil "{}"!\n{}\n'
+                          'Consider using kwarg exact_namematch=True'.format(foil_name, possible_files))
         else:
             possible_files = [f for f in possible_files if f == exact_fname]
             if len(possible_files) == 0:
-                raise Error('Did not find any coordinate files exactly matching "{}"'.format(exact_fname))
+                raise DTError('Did not find any coordinate files exactly matching "{}"'.format(exact_fname))
             else:
                 return possible_files[0]
 
 
 def merge_polar_data_dicts(new: dict, old: dict):
     if len(old) == 0:  # there was no old data
         return new
@@ -191,21 +192,21 @@
     new_pol_keys = new[list(new.keys())[0]].keys()
     merged = new.copy()  # merged starts out as copy of the new dict
     for old_pol_key, old_pol in old.items():  # cylce thru old dict
         if old_pol_key not in new.keys():  # if saved (re, mach, ncrit) data not in new data
             if old_pol.keys() == new_pol_keys:  # if keys are the same (alpha, CL, CD, etc)
                 merged[old_pol_key] = old_pol  # append and move on
             else:  # if keys aren't same, warn that data isn't being retained
-                print('Warning: found saved polar data of older/incorrect format -> deleting {}'.format(old_pol_key))
+                print('DTWarning: found saved polar data of older/incorrect format -> deleting {}'.format(old_pol_key))
         else:  # if saved (re, mach, ncrit) data in new data
             if old_pol.keys() == new_pol_keys:  # if same keys (alpha, CL, CD, etc) inform of overwrite
                 pass
-                # print('Warning: overwriting saved polar data for {}'.format(old_pol_key))
+                # print('DTWarning: overwriting saved polar data for {}'.format(old_pol_key))
             else:  # if not same keys
-                print('Warning: overwriting saved polar data for {} (was older/incorrect format)'.format(old_pol_key))
+                print('DTWarning: overwriting saved polar data for {} (was older/incorrect format)'.format(old_pol_key))
     return merged
 
 
 def scrub_nans(d: dict):
     # get all the indices where there's nans
     nan_idxs = []
     for key, val in d.items():
@@ -304,16 +305,17 @@
         lower_idxs = np.where(lower_coords[:, 0] > 0.8)[0]
         for i in lower_idxs:
             xc, yc = lower_coords[i]
             dy = total_dy * (xc - blend_start) / (1 - blend_start)
             yc -= dy
             lower_coords[i] = [xc, yc]
         if verbose:
-            Info('Detected airfoil ({}) with TE not equal to the requested value\n-> artificially adjusted TE gap to {} '
-                     '(normalized)'.format(name, te_gap_set))
+            DTInfo(
+                'Detected airfoil ({}) with TE not equal to the requested value\n-> artificially adjusted TE gap to {} '
+                '(normalized)'.format(name, te_gap_set))
 
     # re-combine upper and lower coords and split back into x, y arrays
     if upper_coords[-1][0] == lower_coords[0][0] and upper_coords[-1][1] == lower_coords[0][1]:  # check for double 0, 0
         coords = np.append(upper_coords, lower_coords[1:], axis=0)
     else:
         coords = np.append(upper_coords, lower_coords, axis=0)
 
@@ -325,21 +327,21 @@
               mach: float = 0.0, output_fpath: str = None, keypress_iternum: int = 1, tmout: int = 25,
               hide_windows: bool = True, verbose: bool = False):
     if not output_fpath:
         output_fpath = 'polar_output.txt'
 
     # swept pacc param
     if alpha is not None and cl is not None:
-        raise Error('Cannot give "run_xfoil" both "alpha" and "cl"')
+        raise DTError('Cannot give "run_xfoil" both "alpha" and "cl"')
     elif alpha is not None:
         swept_param = {'alpha': alpha}
     elif cl is not None:
         swept_param = {'cl': cl}
     else:
-        raise Error('Must give "run_xfoil" either a list of "alpha" to sweep or a list of "cl" to sweep')
+        raise DTError('Must give "run_xfoil" either a list of "alpha" to sweep or a list of "cl" to sweep')
 
     # sort the swept values
     vals = list(sorted(list(swept_param.values())[0]))
 
     # directory and temp command file, also xfoil path
     xfoil_dir = _get_user_settings()['airfoil_database']
     xfoil_cmnd_file = os.path.join(xfoil_dir, 'xfoil_inputs_temp.txt')
@@ -510,15 +512,15 @@
     return
 
 
 def read_xrotor_op_file(fpath: str):
     with open(fpath, 'r') as f:
         txt = f.read()
     if '********** NOT CONVERGED **********' in txt:
-        raise Error('XROTOR did not converge')
+        raise DTError('XROTOR did not converge')
     lines = txt.split('\n')
     d = {}
     headers = None
 
     for line in lines:
         if line.strip('-').strip('=').strip() == '':
             pass  # ignore blank lines
@@ -593,21 +595,21 @@
 
 
 # =============== INTERFACING WITH 3RD PARTY PROGRAMS ===============
 def download_foil_coordinates(foil_str: str):
     foil_str = '{}.dat'.format(foil_str) if not foil_str.endswith('.dat') else foil_str
     coord_url = 'https://m-selig.ae.illinois.edu/ads/coord/{}'.format(foil_str)
     savepath = os.path.join(get_foil_db(), foil_str)
-    Info('Attempting to download "{}"...'.format(coord_url))
+    DTInfo('Attempting to download "{}"...'.format(coord_url))
     try:
         urllib.request.urlretrieve(coord_url, savepath)
-        Info('saved to "{}"'.format(savepath), indent_level=1)
+        DTInfo('saved to "{}"'.format(savepath), indent_level=1)
         return True
     except urllib.error.HTTPError:
-        Warning('Unable to download, not found')
+        DTWarning('Unable to download, not found')
         return False
 
 
 def read_radial_stations(prop: Propeller, plot_also: bool = True, verbose: bool = False):
     stations = []
     if not os.path.exists(prop.station_polar_folder):
         return stations
@@ -651,16 +653,16 @@
     if 'dens' in prop.design_atmo_props:
         rho = prop.design_atmo_props['dens']
 
     t = ''
     stations = []
     for idx, xi in enumerate(prop.station_params):  # append station text all together and save
         if verbose:
-            Info('Auto-generating section inputs from airfoil database data for section {} ({})...'.
-                  format(idx + 1, prop.station_params[xi]))
+            DTInfo('Auto-generating section inputs from airfoil database data for section {} ({})...'.
+            format(idx + 1, prop.station_params[xi]))
         fn = prop.station_params[xi]
         foil = Airfoil(name=fn, verbose=verbose)
         re_est = int(calc_rotational_re(rho=rho, rpm=prop.design_rpm, radius=prop.radius * xi, chord=prop.radius / 10,
                                         mu=mu, vel=prop.design_speed_mps, adv=prop.design_adv))
         st = RadialStation(station_idx=idx, Xisection=xi, foil=foil, re_estimate=re_est, plot=plot_also, verbose=verbose)
         t += st.generate_txt_params()
         stations.append(st)
@@ -675,15 +677,15 @@
     if tmout is None and vorform.lower() == 'vrtx':
         tmout = 25
     elif tmout is None:
         tmout = 10
 
     # vorform has to be one of these three things
     if vorform.lower() not in ['grad', 'pot', 'vrtx']:
-        raise Error('Input "vorform" must be one of ["grad", "pot", "vrtx"]')
+        raise DTError('Input "vorform" must be one of ["grad", "pot", "vrtx"]')
 
     # filename stuff
     dirname, fname = os.path.split(xrr_file)
     relpath = os.path.join(os.path.split(dirname)[1], fname)
 
     # first we set the vorform
     cmnds = ['load {}\n'.format(relpath), 'oper', 'form', '{}\n'.format(vorform)]
@@ -691,15 +693,15 @@
     # if we are changing the velo, do that next
     if velo is not None:
         cmnds.extend(['velo', '{}'.format(velo), 'rein\n\ny'])
 
     # can only be changing 1 of the 5 at a time
     non_none_kwargs = [i for i in [adva, rpm, thrust, torque, power] if i is not None]
     if len(non_none_kwargs) > 1:
-        raise Error('Can only change 1 of (adva, rpm, thrust, torque, power) at a time')
+        raise DTError('Can only change 1 of (adva, rpm, thrust, torque, power) at a time')
 
     # command text based on which one was given
     if adva is not None:
         cmnds.extend(['adva', str(adva)])
     elif rpm is not None:
         cmnds.extend(['rpm', str(rpm)])
     elif thrust is not None:
@@ -728,15 +730,15 @@
     # run the mutha
     xrotor_fpath = os.path.join(get_prop_db(), 'xrotor.exe')
     with open(xrotor_cmnd_file, 'r') as f:
         sui = subprocess.STARTUPINFO()
         if hide_windows:
             sui.dwFlags |= subprocess.STARTF_USESHOWWINDOW
         if verbose:
-            Info('Running XROTOR for off-design operating point...', indent_level=1)
+            DTInfo('Running XROTOR for off-design operating point...', indent_level=1)
         if xrotor_verbose:
             out_err_kw = {}
         else:
             out_err_kw = {'stdout': subprocess.DEVNULL, 'stderr': subprocess.STDOUT}
 
         subprocess.run([xrotor_fpath], startupinfo=sui, stdin=f, **out_err_kw,
                        timeout=tmout, cwd=get_prop_db())
@@ -816,19 +818,19 @@
     if tmout is None and design_vorform == 'vrtx':
         tmout = 100
     elif tmout is None:
         tmout = 30
 
     # name must be less than 38? characters for XROTOR to be able to save it
     if len(name) > 38:
-        raise Error('"name" must be less than 38 characters when creating a propeller, "{}" is too long'.format(name))
+        raise DTError('"name" must be less than 38 characters when creating a propeller, "{}" is too long'.format(name))
 
     # must input an altitude in atmo props
     if 'altitude_km' not in design_atmo_props:
-        raise Error('You must include "altitude_km" as an input to create_propeller()')
+        raise DTError('You must include "altitude_km" as an input to create_propeller()')
 
     # delete if exists already, make save folder, point-cloud folder
     save_folder = os.path.join(get_prop_db(), name)
     if os.path.exists(save_folder):
         shutil.rmtree(save_folder)
     os.mkdir(save_folder)
 
@@ -870,19 +872,19 @@
         vorform_txt = 'pot\n'
     elif any([design_vorform.lower() == i for i in ['grad', 'pot', 'vrtx']]):
         vorform_txt = '{}\n'.format(design_vorform.lower())
 
     # prep XROTOR commands for the advance ratio OR RPM design specification
     if design_adv is not None:
         if design_rpm is not None:
-            raise Error('Cannot specify both "design_adv" and "design_rpm", must pick one or the other')
+            raise DTError('Cannot specify both "design_adv" and "design_rpm", must pick one or the other')
         adv_rpm_txt = '{}'.format(design_adv)
     elif design_rpm is not None:
         if design_adv is not None:
-            raise Error('Cannot specify both "design_adv" and "design_rpm", must pick one or the other')
+            raise DTError('Cannot specify both "design_adv" and "design_rpm", must pick one or the other')
         adv_rpm_txt = '{}\n{}'.format(0, design_rpm)
 
     # prep XROTOR commands for the thrust OR power design specification
     if design_thrust is not None:
         thr_pow_txt = '{}'.format(design_thrust)
     elif design_power is not None:
         thr_pow_txt = '{}\n{}'.format(0, design_power)
@@ -892,27 +894,27 @@
         if 'const' in design_cl:
             const_cl = design_cl['const']
             cl_txt = 'cc\n{}\n\n'.format(const_cl)
         elif 'file' in design_cl:
             fpath = design_cl['file']
             cl_txt = 'cr\n{}\n\n'.format(fpath)
         else:
-            raise Error('Must give either a "const" CL target (constant), a "root" and "tip" CL target '
-                        '(linearly varied), or specify a CL(r/R) .txt file')
+            raise DTError('Must give either a "const" CL target (constant), a "root" and "tip" CL target '
+                          '(linearly varied), or specify a CL(r/R) .txt file')
     elif len(design_cl) == 2:  # a linear cl was given
         if all([k in design_cl for k in ['root', 'tip']]):
             root_cl = design_cl['root']
             tip_cl = design_cl['tip']
             cl_txt = 'cl\n{}\n{}\n\n'.format(root_cl, tip_cl)
         else:
-            raise Error('If only 2 keywords are given in "design_cl", they must be "root" and "tip"')
+            raise DTError('If only 2 keywords are given in "design_cl", they must be "root" and "tip"')
     else:
-        raise Error('"design_cl" input dictionary error, either too many or not enough keys (if a single key'
-                    'is given, it must be either "const" or "file", if 2 keys are given they must be "root" '
-                    'and "tip"')
+        raise DTError('"design_cl" input dictionary error, either too many or not enough keys (if a single key'
+                      'is given, it must be either "const" or "file", if 2 keys are given they must be "root" '
+                      'and "tip"')
 
     # prep XROTOR commands for saving blade data r/R
     blade_data_keys = ['CH', 'BE', 'GAM', 'CL', 'CD', 'RE', 'EFP', 'Ub', 'VA', 'VT', 'VD', 'VA/V', 'VT/V', 'VD/V',
                        'VAslip', 'VTslip', 'Aslip', 'Ti', 'Pi', 'Tv', 'Pv', 'Ttot', 'Ptot', 'Xw', 'Vw', 'Tw', 'Pw']
     blade_data = {}
     blade_txt = 'plot\n12\n'
     for key in blade_data_keys:
@@ -942,15 +944,15 @@
 
     xrotor_fpath = os.path.join(get_prop_db(), 'xrotor.exe')
     with open(xrotor_cmnd_file, 'r') as f:
         sui = subprocess.STARTUPINFO()
         if hide_windows:
             sui.dwFlags |= subprocess.STARTF_USESHOWWINDOW
         if verbose:
-            Info('Running XROTOR to create new geometry...')
+            DTInfo('Running XROTOR to create new geometry...')
         if xrotor_verbose:
             subprocess.run([xrotor_fpath], startupinfo=sui, stdin=f, timeout=tmout, cwd=get_prop_db())
         else:
             subprocess.run([xrotor_fpath], startupinfo=sui, stdin=f, stdout=subprocess.DEVNULL, stderr=subprocess.STDOUT,
                            timeout=tmout, cwd=get_prop_db())
     os.remove(xrotor_cmnd_file)
     os.remove(aero_params_fpath)
@@ -977,15 +979,15 @@
     # save the PDT propeller meta-file, and then read in the operating point dictionary by calling load_from_savefile()
     prop.xrotor_op_dict = read_xrotor_op_file(prop.xrop_file)
     prop.save_station_polars()
     prop.save_meta_file()
     prop.load_from_savefile(verbose=verbose)   # reads meta, xrr, xrop, and point clouds
 
     if not verbose:
-        Info('"{}" Geometry Created!'.format(prop.name))
+        DTInfo('"{}" Geometry Created!'.format(prop.name))
     if plot_after:
         prop.plot_design_point_panel()
 
     return prop
 
 
 def write_blade_cl_file(r_pts: list, cl_pts: list, savepath: str = None):
@@ -1039,15 +1041,15 @@
                        radius: float = None, adv: float = None):
     if all([i is not None for i in [rho, rpm, radius, chord, mu]]):
         re = rho * (rpm / 60 * 2 * np.pi) * radius * chord / mu
     elif all([i is not None for i in [rho, vel, adv, radius, chord, mu]]):
         rpm = vel / np.pi / 2 / radius / adv * 60
         re = rho * (rpm / 60 * 2 * np.pi) * radius * chord / mu
     else:
-        raise Error('Must input all of either [rho, vel, chord, mu] or [rho, rpm, radius, chord, mu]')
+        raise DTError('Must input all of either [rho, vel, chord, mu] or [rho, rpm, radius, chord, mu]')
     return re
 
 
 def standard_atmosphere(altitude_km: float) -> dict:  # standard atmosphere eqs from Jake's college prof.
 
     alt_m = altitude_km * 1000
 
@@ -1061,29 +1063,29 @@
     rho1 = rho0 * (temp1 / temp0) ** (-g / slope0 / R_air - 1)
 
     temp2 = temp1
     p2 = p1 * np.exp(-g / R_air / temp2 * (alt2 - alt1))
     rho2 = rho1 * np.exp(-g / R_air / temp2 * (alt2 - alt1))
 
     if alt_m < 0:
-        raise Error('Cannot input negative values into standard_atmosphere()')
+        raise DTError('Cannot input negative values into standard_atmosphere()')
     elif alt_m < alt1:
         temp = temp0 + slope0 * alt_m
         p = p0 * (temp / temp0) ** (-g / slope0 / R_air)
         rho = rho0 * (temp / temp0) ** (-g / slope0 / R_air - 1)
     elif alt_m < alt2:
         temp = temp1
         p = p1 * np.exp(-g / slope1 / R_air / temp * (alt_m - alt1))
         rho = rho1 * np.exp(-g / R_air / temp * (alt_m - alt1))
     elif alt_m < alt3:
         temp = temp2 + slope2 * (alt_m - alt2)
         p = p2 * (temp / temp2) ** (-g / slope2 / R_air)
         rho = rho2 * (temp / temp2) ** (-g / slope2 / R_air - 1)
     else:
-        raise Error('Altitude out of range of atmosphere model')
+        raise DTError('Altitude out of range of atmosphere model')
 
     sonic_a = np.sqrt(gamma_air * R_air * temp)
     mu = mu0 * (temp / temp0) ** 1.5 * ((temp0 + 120) / (temp + 120))
 
     return {'temp': temp, 'p': p, 'rho': rho, 'sonic_a': sonic_a, 'mu': mu}
```

### Comparing `propeller_design_tools-0.4.6/propeller_design_tools/helper_ui_classes.py` & `propeller_design_tools-0.4.7/propeller_design_tools/helper_ui_classes.py`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.6/propeller_design_tools/helper_ui_subclasses.py` & `propeller_design_tools-0.4.7/propeller_design_tools/helper_ui_subclasses.py`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.6/propeller_design_tools/optimizations.py` & `propeller_design_tools-0.4.7/propeller_design_tools/optimizations.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,20 @@
-import shutil
 import os
-import numpy as np
+import shutil
+
 import matplotlib.pyplot as plt
+import numpy as np
 import pyqtgraph as pg
 from pyqtgraph import opengl as gl
+
 from propeller_design_tools import Propeller
-from propeller_design_tools.user_io import Error
-from propeller_design_tools.funcs import create_propeller, get_prop_db
-from propeller_design_tools.user_io import Info, Warning
 from propeller_design_tools.custom_opengl_classes import Custom3DAxis
+from propeller_design_tools.funcs import create_propeller, get_prop_db
+from propeller_design_tools.user_io import DTError
+from propeller_design_tools.user_io import DTInfo, DTWarning
 
 
 class VehicleRangeOptimization:
     def __init__(self):
         pass
 
 
@@ -32,28 +34,28 @@
         self.var2 = None
 
         # need to attempt to load any existing results here
         if os.path.exists(self.save_dir):
             prop_fpaths = [os.path.join(self.save_dir, f) for f in os.listdir(self.save_dir) if
                            os.path.isdir(os.path.join(self.save_dir, f))]
             if verbose:
-                Info('Detected existing optimization results for "{}", attempting to load them ({})...'
-                     .format(self.base_prop.name, len(prop_fpaths)))
+                DTInfo('Detected existing optimization results for "{}", attempting to load them ({})...'
+                .format(self.base_prop.name, len(prop_fpaths)))
             for fpath in prop_fpaths:
                 prop = Propeller(fpath, verbose=False)
                 name = os.path.split(fpath)[1]
                 vel, cl, val2 = name.split('_', 2)
                 vel = float(vel.replace('vel-', ''))
                 cl = float(cl.replace('cl-', ''))
                 var2, val2 = val2.split('-')
                 val2 = float(val2)
                 self.var2 = 'design_{}'.format(var2)
                 self.propellers[(vel, cl, val2)] = prop
             if verbose:
-                Info('Done!', indent_level=1)
+                DTInfo('Done!', indent_level=1)
 
     @property
     def var2base(self):
         return self.var2.replace('design_', '')
 
     @property
     def unique_vels(self):
@@ -80,30 +82,30 @@
                 shutil.rmtree(self.save_dir)
 
         if not os.path.exists(self.save_dir):
             os.mkdir(self.save_dir)
 
         # cant give both advs and rpms
         if advs is not None and rpms is not None:
-            raise Error('Cannot give both "advs" and "rpms" into create_prop_grid()')
+            raise DTError('Cannot give both "advs" and "rpms" into create_prop_grid()')
 
         # figure out oth sweep parameter = vel
         if vels is None:
             base_vel_val = getattr(self.base_prop, 'design_speed_mps')
             vel_sweep_vals = [v * base_vel_val for v in [0.7, 0.85, 1.0, 1.15, 1.3]]
         else:
             vel_sweep_vals = vels
 
         # figure out 1st sweep parameter = CL
         if cl_consts is None:
             base_cl_val = getattr(self.base_prop, 'design_cl')
             if 'const' in base_cl_val:
                 base_cl_val = base_cl_val['const']
             else:
-                raise Error('Optimizations only currently implemented for "const" cl')
+                raise DTError('Optimizations only currently implemented for "const" cl')
             cl_sweep_vals = [c * base_cl_val for c in [0.7, 0.85, 1.0, 1.15, 1.3]]
         else:
             cl_sweep_vals = cl_consts
 
         # figure out what seconds sweep parameter is and its values
         if advs is not None:
             self.var2 = 'design_adv'
@@ -119,15 +121,15 @@
         # run the sweeps
         total_cnt = len(vel_sweep_vals) * len(cl_sweep_vals) * len(var2_sweep_vals)
         cnt = 0
         for v, vel in enumerate(vel_sweep_vals):
             for i, cl in enumerate(cl_sweep_vals):
                 for k, val2 in enumerate(var2_sweep_vals):
                     cnt += 1
-                    Info('Creating propeller # {} / {}'.format(cnt, total_cnt))
+                    DTInfo('Creating propeller # {} / {}'.format(cnt, total_cnt))
                     opt_name = 'vel-{:.2f}_cl-{:.2f}_{}-{:.3f}'.format(vel, cl, self.var2.replace('design_', ''), val2)
                     adv_rpm_kwarg = {self.var2: val2}
                     try:
                         prop = create_propeller(name=opt_name,
                                              nblades=self.base_prop.nblades,
                                              radius=self.base_prop.radius,
                                              hub_radius=self.base_prop.hub_radius,
@@ -145,19 +147,19 @@
                                              show_station_fit_plots=False,
                                              plot_after=False)
                         shutil.move(prop.save_folder, self.save_dir)
                         vel = float('{:.2f}'.format(vel))
                         cl = float('{:.2f}'.format(cl))
                         val2 = float('{:.3f}'.format(val2))
                         self.propellers[(vel, cl, val2)] = prop
-                    except Error:
+                    except DTError:
                         vel = float('{:.2f}'.format(vel))
                         cl = float('{:.2f}'.format(cl))
                         val2 = float('{:.3f}'.format(val2))
-                        Warning('XROTOR did not converge for vel-{}_cl-{}_{}-{}'.format(vel, cl, self.var2base, val2))
+                        DTWarning('XROTOR did not converge for vel-{}_cl-{}_{}-{}'.format(vel, cl, self.var2base, val2))
                         hanging_folder = os.path.join(get_prop_db(), opt_name)
                         if os.path.exists(hanging_folder):
                             shutil.rmtree(hanging_folder)
 
     def thrust_eff(self, vel_val, cl_val, val2_val):
         prop = self.propellers[vel_val, cl_val, val2_val]
         return prop.xrotor_op_dict['thrust(N)'] / prop.xrotor_op_dict['power(W)']
```

### Comparing `propeller_design_tools-0.4.6/propeller_design_tools/prop_analysis_ui_classes.py` & `propeller_design_tools-0.4.7/propeller_design_tools/prop_analysis_ui_classes.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import numpy as np
-from matplotlib.backends.backend_qt5agg import NavigationToolbar2QT as NavigationToolbar
 import pyqtgraph.opengl as gl
-from propeller_design_tools.settings import VALID_OPER_PLOT_PARAMS
+from matplotlib.backends.backend_qt5agg import NavigationToolbar2QT as NavigationToolbar
+
 from propeller_design_tools.funcs import get_all_propeller_dirs
 from propeller_design_tools.propeller import Propeller
+from propeller_design_tools.settings import VALID_OPER_PLOT_PARAMS
+
 try:
     from PyQt5 import QtWidgets, QtCore
     from propeller_design_tools.helper_ui_subclasses import PDT_Label, PDT_GroupBox, PDT_ComboBox, PDT_PushButton, \
         PDT_CheckBox
     from propeller_design_tools.helper_ui_classes import SingleAxCanvas, PropellerCreationPanelCanvas, \
         CheckColumnWidget, AxesComboBoxWidget, RangeLineEditWidget, Capturing
 except:
@@ -233,15 +235,15 @@
         param = self.sweep_param_cb.currentText()
         min_val, max_val, val_step = self.sweep_vals_rle.get_start_stop_step()
         vals = list(np.arange(min_val, max_val, val_step))
         vor = self.vorform_cb.currentText()
 
         if self.prop is None:
             msgbox = QtWidgets.QMessageBox()
-            msgbox.about(self, 'Error', 'Must Select a Propeller() first!')
+            msgbox.about(self, 'DTError', 'Must Select a Propeller() first!')
             return
 
         self.prop.clear_sweep_data()
         self.thread = QtCore.QThread()
         self.prop_sweep_worker = PropellerSweepWorker(prop=self.prop, velos=velos, param2sweep=param, sweep_vals=vals,
                                                       vorform=vor)
         self.prop_sweep_worker.moveToThread(self.thread)
```

### Comparing `propeller_design_tools-0.4.6/propeller_design_tools/prop_creation_ui_classes.py` & `propeller_design_tools-0.4.7/propeller_design_tools/prop_creation_ui_classes.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
+import os
 import subprocess
+
 import numpy as np
-import os
-from propeller_design_tools.propeller import Propeller
+
 from propeller_design_tools.funcs import get_all_propeller_dirs, create_propeller, get_all_airfoil_files
-from propeller_design_tools.user_io import Error
+from propeller_design_tools.propeller import Propeller
 from propeller_design_tools.settings import get_prop_db
 
 try:
     from PyQt5 import QtWidgets, QtCore
     from propeller_design_tools.helper_ui_classes import SingleAxCanvas, Capturing, AxesComboBoxWidget, \
         PropellerCreationPanelCanvas, RadialStationFitParamsCanvas
     from propeller_design_tools.helper_ui_subclasses import PDT_ComboBox, PDT_Label, PDT_SpinBox, PDT_DoubleSpinBox, \
@@ -383,61 +384,61 @@
         self.n_profs_sb.setValue(prop.n_profs)
 
     def create_btn_clicked(self):
         msgbox = QtWidgets.QMessageBox()
 
         name = self.name_le.text()
         if len(name.strip()) == 0:
-            msgbox.about(self, 'Error', 'Invalid Name')
+            msgbox.about(self, 'DTError', 'Invalid Name')
             return
 
         nblades = self.nblades_sb.value()
         radius = self.radius_sb.value()
         hub_radius = self.hub_radius_sb.value()
         hub_wk_disp_br = self.hub_wake_disp_br_sb.value()
         speed = self.design_speed_sb.value()
         adv = self.design_adv_sb.value() if self.design_adv_sb.value() != self.design_adv_sb.minimum() else None
         rpm = self.design_rpm_sb.value() if self.design_rpm_sb.value() != self.design_rpm_sb.minimum() else None
         if adv == self.design_adv_sb.minimum() and rpm == self.design_rpm_sb.minimum():
-            msgbox.about(self, 'Error', 'Must give one of "adv" or "rpm"')
+            msgbox.about(self, 'DTError', 'Must give one of "adv" or "rpm"')
             return
 
         thrust = self.design_thrust_sb.value() if self.design_thrust_sb.value() != self.design_thrust_sb.minimum() else None
         power = self.design_power_sb.value() if self.design_power_sb.value() != self.design_power_sb.minimum() else None
         if thrust is None and power is None:
-            msgbox.about(self, 'Error', 'Must give one of "thrust" or "power"')
+            msgbox.about(self, 'DTError', 'Must give one of "thrust" or "power"')
             return
 
         nradial = self.nradial_sb.value()
         cl_txt = self.design_cl_le.text().strip()
         if len(cl_txt.split(',')) == 1:
             cl_dict = {'const': float(cl_txt)}
         elif len(cl_txt.split(',')) == 2:
             cl_dict = {'root': float(cl_txt.split(',')[0].strip()), 'tip': float(cl_txt.split(',')[1].strip())}
         else:
             msgbox = QtWidgets.QMessageBox()
-            msgbox.about(self, 'Error', 'Only "const" and "linear" CL currently supported')
+            msgbox.about(self, 'DTError', 'Only "const" and "linear" CL currently supported')
             return
 
         altitude = self.atmo_props_widg.altitude_sb.value()
         alt_ismin = altitude == self.atmo_props_widg.altitude_sb.minimum()
         rho = self.atmo_props_widg.rho_sb.value()
         rho_ismin = rho == self.atmo_props_widg.rho_sb.minimum()
         nu = self.atmo_props_widg.nu_sb.value()
         nu_ismin = nu == self.atmo_props_widg.nu_sb.minimum()
         vsou = self.atmo_props_widg.vsou_sb.value()
         vsou_ismin = vsou == self.atmo_props_widg.vsou_sb.minimum()
         if alt_ismin and any([rho_ismin, nu_ismin, vsou_ismin]):
-            msgbox.about(self, 'Error', 'Can only / must give "altitude" or all three "rho", "nu" and "vsou"')
+            msgbox.about(self, 'DTError', 'Can only / must give "altitude" or all three "rho", "nu" and "vsou"')
             return
 
         vorform = self.vorform_cb.currentText()
         stations_dict = self.station_params_widg.get_stations_dict()
         if stations_dict is None:
-            msgbox.about(self, 'Error', 'Must give at least 1 station')
+            msgbox.about(self, 'DTError', 'Must give at least 1 station')
             return
 
         skew = self.skew_sb.value()
         n_prof_pts = self.n_prof_pts_sb.value() if self.n_prof_pts_sb.value() != self.n_prof_pts_sb.minimum() else None
         n_profs = self.n_profs_sb.value()
 
         if altitude is not None:
@@ -620,15 +621,15 @@
 
     def add_row(self):
         rt_lay = QtWidgets.QHBoxLayout()
         rt_widg = QtWidgets.QWidget()
         rt_widg.setLayout(rt_lay)
         if self.rows_lay.rowCount() > 1:
             msgbox = QtWidgets.QMessageBox()
-            msgbox.about(self, 'Error', '> 1 station not yet implemented in PDT')
+            msgbox.about(self, 'DTError', '> 1 station not yet implemented in PDT')
             return
         num_lbl = PDT_Label('{}'.format(self.rows_lay.rowCount()), font_size=11)
         foil_cb = PDT_ComboBox(font_size=11, width=140)
         foil_cb.addItems(get_all_airfoil_files())
         roR_sb = PDT_DoubleSpinBox(font_size=11)
         roR_sb.setMaximum(1.0)
         roR_sb.setSingleStep(0.01)
```

### Comparing `propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller/MyPropeller.meta` & `propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller/MyPropeller.meta`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller/MyPropeller.xrop` & `propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller/MyPropeller.xrop`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller/MyPropeller.xrr` & `propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller/MyPropeller.xrr`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_0.txt` & `propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_0.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_1.txt` & `propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_1.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_10.txt` & `propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_10.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_11.txt` & `propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_11.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_12.txt` & `propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_12.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_13.txt` & `propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_13.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_14.txt` & `propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_14.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_15.txt` & `propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_15.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_16.txt` & `propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_16.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_17.txt` & `propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_17.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_18.txt` & `propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_18.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_19.txt` & `propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_19.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_2.txt` & `propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_2.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_20.txt` & `propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_20.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_21.txt` & `propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_21.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_22.txt` & `propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_22.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_23.txt` & `propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_23.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_24.txt` & `propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_24.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_25.txt` & `propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_25.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_26.txt` & `propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_26.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_27.txt` & `propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_27.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_28.txt` & `propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_28.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_29.txt` & `propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_29.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_3.txt` & `propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_3.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_30.txt` & `propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_30.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_31.txt` & `propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_31.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_32.txt` & `propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_32.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_33.txt` & `propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_33.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_34.txt` & `propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_34.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_35.txt` & `propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_35.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_36.txt` & `propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_36.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_37.txt` & `propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_37.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_38.txt` & `propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_38.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_39.txt` & `propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_39.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_4.txt` & `propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_4.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_40.txt` & `propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_40.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_41.txt` & `propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_41.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_42.txt` & `propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_42.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_43.txt` & `propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_43.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_44.txt` & `propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_44.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_45.txt` & `propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_45.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_46.txt` & `propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_46.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_47.txt` & `propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_47.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_48.txt` & `propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_48.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_49.txt` & `propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_49.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_5.txt` & `propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_5.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_6.txt` & `propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_6.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_7.txt` & `propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_7.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_8.txt` & `propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_8.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_9.txt` & `propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_9.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller/station_polars/0.75_clarky.dat.polar` & `propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller/station_polars/0.75_clarky.dat.polar`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller2/MyPropeller2.meta` & `propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller2/MyPropeller2.meta`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller2/MyPropeller2.xrop` & `propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller2/MyPropeller2.xrop`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller2/MyPropeller2.xrr` & `propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller2/MyPropeller2.xrr`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_0.txt` & `propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_0.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_1.txt` & `propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_1.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_10.txt` & `propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_10.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_11.txt` & `propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_11.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_12.txt` & `propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_12.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_13.txt` & `propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_13.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_14.txt` & `propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_14.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_15.txt` & `propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_15.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_16.txt` & `propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_16.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_17.txt` & `propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_17.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_18.txt` & `propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_18.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_19.txt` & `propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_19.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_2.txt` & `propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_2.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_20.txt` & `propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_20.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_21.txt` & `propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_21.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_22.txt` & `propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_22.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_23.txt` & `propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_23.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_24.txt` & `propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_24.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_25.txt` & `propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_25.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_26.txt` & `propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_26.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_27.txt` & `propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_27.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_28.txt` & `propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_28.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_29.txt` & `propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_29.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_3.txt` & `propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_3.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_30.txt` & `propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_30.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_31.txt` & `propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_31.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_32.txt` & `propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_32.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_33.txt` & `propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_33.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_34.txt` & `propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_34.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_35.txt` & `propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_35.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_36.txt` & `propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_36.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_37.txt` & `propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_37.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_38.txt` & `propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_38.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_39.txt` & `propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_39.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_4.txt` & `propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_4.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_40.txt` & `propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_40.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_41.txt` & `propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_41.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_42.txt` & `propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_42.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_43.txt` & `propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_43.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_44.txt` & `propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_44.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_45.txt` & `propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_45.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_46.txt` & `propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_46.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_47.txt` & `propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_47.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_48.txt` & `propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_48.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_49.txt` & `propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_49.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_5.txt` & `propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_5.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_6.txt` & `propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_6.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_7.txt` & `propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_7.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_8.txt` & `propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_8.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_9.txt` & `propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_9.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller2/station_polars/0.75_e855.dat.polar` & `propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller2/station_polars/0.75_e855.dat.polar`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller3/MyPropeller3.meta` & `propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller3/MyPropeller3.meta`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller3/MyPropeller3.xrop` & `propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller3/MyPropeller3.xrop`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller3/MyPropeller3.xrr` & `propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller3/MyPropeller3.xrr`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_0.txt` & `propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_0.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_1.txt` & `propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_1.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_10.txt` & `propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_10.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_11.txt` & `propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_11.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_12.txt` & `propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_12.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_13.txt` & `propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_13.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_14.txt` & `propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_14.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_15.txt` & `propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_15.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_16.txt` & `propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_16.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_17.txt` & `propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_17.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_18.txt` & `propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_18.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_19.txt` & `propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_19.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_2.txt` & `propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_2.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_20.txt` & `propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_20.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_21.txt` & `propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_21.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_22.txt` & `propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_22.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_23.txt` & `propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_23.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_24.txt` & `propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_24.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_25.txt` & `propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_25.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_26.txt` & `propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_26.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_27.txt` & `propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_27.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_28.txt` & `propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_28.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_29.txt` & `propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_29.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_3.txt` & `propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_3.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_30.txt` & `propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_30.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_31.txt` & `propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_31.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_32.txt` & `propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_32.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_33.txt` & `propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_33.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_34.txt` & `propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_34.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_35.txt` & `propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_35.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_36.txt` & `propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_36.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_37.txt` & `propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_37.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_38.txt` & `propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_38.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_39.txt` & `propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_39.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_4.txt` & `propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_4.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_40.txt` & `propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_40.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_41.txt` & `propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_41.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_42.txt` & `propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_42.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_43.txt` & `propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_43.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_44.txt` & `propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_44.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_45.txt` & `propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_45.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_46.txt` & `propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_46.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_47.txt` & `propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_47.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_48.txt` & `propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_48.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_49.txt` & `propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_49.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_5.txt` & `propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_5.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_6.txt` & `propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_6.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_7.txt` & `propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_7.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_8.txt` & `propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_8.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_9.txt` & `propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_9.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.6/propeller_design_tools/prop_database/MyPropeller3/station_polars/0.75_mrc-16.dat.polar` & `propeller_design_tools-0.4.7/propeller_design_tools/prop_database/MyPropeller3/station_polars/0.75_mrc-16.dat.polar`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.6/propeller_design_tools/prop_database/xrotor.exe` & `propeller_design_tools-0.4.7/propeller_design_tools/prop_database/xrotor.exe`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.6/propeller_design_tools/propeller.py` & `propeller_design_tools-0.4.7/propeller_design_tools/propeller.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 import os
 import shutil
-from propeller_design_tools import funcs
-from propeller_design_tools.user_io import Info, Error, Warning
-from propeller_design_tools.settings import get_setting
-from propeller_design_tools.airfoil import Airfoil
-from propeller_design_tools.settings import VALID_OPER_PLOT_PARAMS
-from propeller_design_tools.custom_opengl_classes import Custom3DArrow
-import matplotlib.pyplot as plt
+from typing import Union
+
 import matplotlib.gridspec as gridspec
-from mpl_toolkits import mplot3d
+import matplotlib.pyplot as plt
 import numpy as np
-from stl import mesh
-from typing import Union
 import pyqtgraph as pg
 import pyqtgraph.opengl as gl
+from stl import mesh
+
+from propeller_design_tools import funcs
+from propeller_design_tools.airfoil import Airfoil
+from propeller_design_tools.custom_opengl_classes import Custom3DArrow
+from propeller_design_tools.settings import VALID_OPER_PLOT_PARAMS
+from propeller_design_tools.settings import get_setting
+from propeller_design_tools.user_io import DTInfo, DTError, DTWarning
 
 
 class Propeller(object):
 
     creation_attrs = {'nblades': int, 'radius': float, 'hub_radius': float, 'hub_wake_disp_br': float,
                       'design_speed_mps': float, 'design_adv': float, 'design_rpm': float, 'design_thrust': float,
                       'design_power': float, 'design_cl': dict, 'design_atmo_props': dict, 'design_vorform': str,
@@ -34,36 +35,36 @@
         self.oper_data = None
         self.wvel_data = None
         self.stl_mesh = None
 
         # check if the prop db exists
         prop_db = get_setting('propeller_database')
         if prop_db is None:
-            raise Error(s='No Propeller Database is set!  First set one with "pdt.set_propeller_database(str)".')
+            raise DTError(s='No Propeller Database is set!  First set one with "pdt.set_propeller_database(str)".')
 
         # initialize all attrs to None for script auto-completion detection
         self.nblades, self.radius, self.hub_radius, self.hub_wake_disp_br, self.design_speed_mps, self.design_adv, \
         self.design_rpm, self.design_thrust, self.design_power, self.design_cl, self.design_atmo_props, \
         self.design_vorform, self.station_params, self.geo_params, self.xrotor_d, self.xrotor_op_dict, \
         self.blade_data, self.blade_xyz_profiles = [None] * 18
 
         # if no kwargs were given and there's a meta_file, load it
         if len(kwargs) == 0:
             if os.path.exists(self.meta_file):
                 if verbose:
-                    Info(s='Loading propeller "meta-file" ({})'.format(self.meta_file))
+                    DTInfo(s='Loading propeller "meta-file" ({})'.format(self.meta_file))
                 self.load_from_savefile(verbose=verbose)
             else:
                 raise FileNotFoundError('Could not find file {}'.format(self.meta_file))
         else:  # cycle thru kwargs and set if they're valid, if not ignore them
             for key, val in kwargs.items():
                 if key in self.creation_attrs:
                     setattr(self, key, val)
                 else:
-                    raise Error('Unknown KWARG input "{}"'.format(key))
+                    raise DTError('Unknown KWARG input "{}"'.format(key))
 
         # attempt to load any oper sweep data and any wvel sweep data
         self.oper_data = PropellerOperData(directory=self.oper_data_dir)
         self.oper_data.load_oper_sweep_results(verbose=verbose)
         self.wvel_data = PropellerWVelData(directory=self.wvel_data_dir)
         self.wvel_data.load_wvel_sweep_results(verbose=verbose)
 
@@ -281,40 +282,40 @@
 
         return d
 
     def load_from_savefile(self, verbose):
         # 1st set attrs from the PDT metafile
         self.read_pdt_metafile()
         if verbose:
-            Info(s='Successfully read meta-file (.meta)!', indent_level=1)
+            DTInfo(s='Successfully read meta-file (.meta)!', indent_level=1)
 
         # set the stations... why did I do it this way??
         self.set_stations(plot_also=False, verbose=verbose, from_loadsave_file=True)
         if verbose:
-            Info(s='Successfully read and set station polars!', indent_level=1)
+            DTInfo(s='Successfully read and set station polars!', indent_level=1)
 
         # then read in the XROTOR restart file (in the xrotor_geometry_files)
         self.xrotor_d = self.read_xrotor_restart()
         if verbose:
-            Info(s='Successfully read XROTOR restart file (.xrr)!', indent_level=1)
+            DTInfo(s='Successfully read XROTOR restart file (.xrr)!', indent_level=1)
 
         # then read the operating point output file (in xrotor_op_files)
         self.xrotor_op_dict = funcs.read_xrotor_op_file(fpath=self.xrop_file)
         if verbose:
-            Info(s='Successfully read XROTOR operating-point file (.xrop)!', indent_level=1)
+            DTInfo(s='Successfully read XROTOR operating-point file (.xrop)!', indent_level=1)
 
         # and finally read in the point cloud files
         self.blade_xyz_profiles = {}
         fnames = funcs.search_files(folder=self.bld_prof_folder)
         for fname in fnames:
             prof_num = int(fname.replace('profile_', '').replace('.txt', ''))
             xyz_prof = funcs.read_profile_xyz(fpath=os.path.join(self.bld_prof_folder, fname))
             self.blade_xyz_profiles[prof_num] = xyz_prof
         if verbose:
-            Info(s='Successfully read blade profiles!', indent_level=1)
+            DTInfo(s='Successfully read blade profiles!', indent_level=1)
 
         return
 
     def set_stations(self, plot_also: bool = True, verbose: bool = False, from_loadsave_file: bool = False):
         if not from_loadsave_file:
             self.stations, txt = funcs.create_radial_stations(prop=self, plot_also=plot_also, verbose=verbose)
         else:
@@ -401,19 +402,19 @@
         return chordlines
 
     def interp_foil_profiles(self, n_prof_pts: int = None, n_profs: int = 50, tot_skew: float = 0.0):
 
         assert len(self.stations) > 0
 
         if len(self.stations) != 1:
-            raise Error('> 1 profile interpolation not yet implemented')
+            raise DTError('> 1 profile interpolation not yet implemented')
 
         if tot_skew != 0.0:
-            Info('Blade "skew" is not implemented in XROTOR, and therefore not reflected in XROTOR results.\n'
-                 '  > Skew effects are considered negligible for PDT purposes for small enough skew angles.')
+            DTInfo('Blade "skew" is not implemented in XROTOR, and therefore not reflected in XROTOR results.\n'
+                   '  > Skew effects are considered negligible for PDT purposes for small enough skew angles.')
 
         # clear out the existing xyz profiles
         funcs.delete_files_from_folder(self.bld_prof_folder)
 
         station = self.stations[0]
         # nondim_coords = station.foil.get_coords(n_interp=n_prof_pts)
         nondim_coords = station.foil.get_coords_closed_te(n_interp=n_prof_pts)
@@ -610,15 +611,15 @@
         do_thrust_eff_ax()
         wsp = 0.60 if created_from_ui else 0.35
         fig.subplots_adjust(left=0.05, bottom=0.08, right=0.95, top=0.94, wspace=wsp, hspace=0.5)
 
         if savefig:
             savepath = os.path.join(os.getcwd(), '{}.png'.format(ax3d.get_title()))
             fig.savefig(savepath)
-            Info('Saved PNG to "{}"'.format(savepath))
+            DTInfo('Saved PNG to "{}"'.format(savepath))
 
         return fig
 
     def plot_mpl3d_geometry(self, LE: bool = True, TE: bool = True, chords_betas: bool = True, hub: bool = True,
                             input_stations: bool = True, interp_profiles: bool = True, savefig: bool = False, fig=None):
         if fig is not None:
             ax3d = fig.axes[0]
@@ -907,27 +908,27 @@
 
         if os.path.exists(self.stl_fpath):
             os.remove(self.stl_fpath)
         m.save(filename=self.stl_fpath)
 
         self.stl_mesh = mesh.Mesh.from_file(self.stl_fpath)
         if verbose:
-            Info('Saved STL file and reloaded into propeller object: "{}"'.format(self.stl_fpath))
+            DTInfo('Saved STL file and reloaded into propeller object: "{}"'.format(self.stl_fpath))
 
         if plot_after:
             self.plot_stl_mesh()
 
     def load_stl_geometry(self, verbose: bool = True):
         if os.path.exists(self.stl_fpath):
             self.stl_mesh = mesh.Mesh.from_file(self.stl_fpath)
             if verbose:
-                Info('Loaded STL mesh data from file: {}'.format(self.stl_fpath))
+                DTInfo('Loaded STL mesh data from file: {}'.format(self.stl_fpath))
         else:
             if verbose:
-                Warning('STL file does not exist, use "generate_stl_geometry()" first')
+                DTWarning('STL file does not exist, use "generate_stl_geometry()" first')
 
     def plot_stl_mesh(self):
         if not hasattr(self, 'stl_view'):
             pg.mkQApp()
             self.stl_view = gl.GLViewWidget()
         view = self.stl_view
         view.clear()
@@ -945,73 +946,74 @@
                                  shader='normalColor', smooth=False)
         mesh_itm.translate(dx=-0.5 * self.radius, dy=0, dz=0)
         view.addItem(mesh_itm)
 
         return view
 
     def plot_ideal_eff(self):
-        Info('"{}" ideal efficiency: {:.1f}%'.format(self.name, self.ideal_eff))
+        DTInfo('"{}" ideal efficiency: {:.1f}%'.format(self.name, self.ideal_eff))
         return
 
     def analyze_operating_point(self, velo: float = None, adva: float = None, rpm: float = None, thrust: float = None,
                                 power: float = None, torque: float = None, xrotor_verbose: bool = False):
 
         funcs.run_xrotor_oper(xrr_file=self.xrr_file, vorform=self.design_vorform, adva=adva, rpm=rpm, thrust=thrust,
                               torque=torque, power=power, velo=velo, xrotor_verbose=xrotor_verbose)
 
     def analyze_sweep(self, velo_vals: list, sweep_param: str, sweep_vals: list, verbose: bool = True,
                       xrotor_verbose: bool = False, vorform: str = None, prog_signal=None):
         if sweep_param not in ['adva', 'rpm', 'thrust', 'power', 'torque']:
-            raise Error('"sweep_param" must be one of ("adva", "rpm", "thrust", "power", "torque")')
+            raise DTError('"sweep_param" must be one of ("adva", "rpm", "thrust", "power", "torque")')
 
         vorform = self.design_vorform if vorform is None else vorform
 
         total_pnts = len(velo_vals) * len(sweep_vals)
         if verbose:
             info_str = 'Analyzing "{}" across a sweep of {} operating points'.format(self.name, total_pnts)
             if prog_signal is not None:
                 prog_signal.emit(0, [info_str])
             else:
-                Info(info_str)
+                DTInfo(info_str)
         count = 0
         for velo_val in velo_vals:
             for v, val in enumerate(sweep_vals):
                 count += 1
                 if verbose:
                     info_str = 'Analyzing sweep point # {} / {}'.format(count, total_pnts)
                     if prog_signal is not None:
                         prog_signal.emit(count / total_pnts * 100, [info_str])
                     else:
-                        Info(info_str)
+                        DTInfo(info_str)
                 try:
                     funcs.run_xrotor_oper(xrr_file=self.xrr_file, vorform=vorform, velo=velo_val, verbose=False,
                                           xrotor_verbose=xrotor_verbose, **{sweep_param: val})
-                except Error as e:
-                    warn_str = 'Failed to get XROTOR oper results for vel={}, {}={}\n{}'.format(velo_val, sweep_param, val, e)
+                except DTError as e:
+                    warn_str = 'Failed to get XROTOR oper results for vel={}, {}={}\n{}'.format(velo_val, sweep_param,
+                        val, e)
                     if prog_signal is not None:
                         prog_signal.emit(None, [warn_str])
                     else:
-                        Warning(warn_str)
+                        DTWarning(warn_str)
                         pass
 
         self.oper_data.load_oper_sweep_results()
         self.wvel_data.load_wvel_sweep_results()
         if verbose:
             if prog_signal is not None:
                 prog_signal.emit(0, 'Done!')
             else:
-                Info('Done!')
+                DTInfo('Done!')
 
     def clear_sweep_data(self):
         if os.path.exists(self.oper_data_dir):
             shutil.rmtree(self.oper_data_dir)
-            Info('Removed {} and its contents'.format(self.oper_data_dir))
+            DTInfo('Removed {} and its contents'.format(self.oper_data_dir))
         if os.path.exists(self.wvel_data_dir):
             shutil.rmtree(self.wvel_data_dir)
-            Info('Removed {} and its contents'.format(self.wvel_data_dir))
+            DTInfo('Removed {} and its contents'.format(self.wvel_data_dir))
 
 
 class PropellerOperData:
     def __init__(self, directory: str):
         self.directory = directory
         self.datapoints = {}
         self.prop_name = os.path.split(os.path.split(self.directory)[0])[1]
@@ -1048,15 +1050,15 @@
         fnames = self.get_oper_files(fullpath=False)
         for fname in fnames:
             vel_key, rpm_key = [float(num) for num in fname.strip('velo_').strip('.oper').split('_rpm_')]
             vel_key /= 100
             oper_fullpath = os.path.join(self.directory, fname)
             d[(vel_key, rpm_key)] = funcs.read_xrotor_op_file(fpath=oper_fullpath)
         if verbose and len(fnames) > 0:
-            Info('Loaded Existing Oper Results (.oper)!', indent_level=1)
+            DTInfo('Loaded Existing Oper Results (.oper)!', indent_level=1)
 
     def get_unique_param(self, param: str):
         uniq_vals = []
         for val in self.datapoints.values():
             if val[param] not in uniq_vals:
                 uniq_vals.append(val[param])
         return list(sorted(uniq_vals))
@@ -1096,21 +1098,21 @@
                     params[i] = 'Pvisc(W)'
             else:
                 params[i] = None
 
         x_param, y_param, family_param, iso_param = params
 
         if x_param not in valid_params:
-            raise Error('x_param "{}" is not one of the valid params ({})'.format(x_param, valid_params))
+            raise DTError('x_param "{}" is not one of the valid params ({})'.format(x_param, valid_params))
         if y_param not in valid_params:
-            raise Error('y_param "{}" is not one of the valid params ({})'.format(y_param, valid_params))
+            raise DTError('y_param "{}" is not one of the valid params ({})'.format(y_param, valid_params))
         if family_param not in valid_params and family_param is not None:
-            raise Error('family_param error, must be one of {}'.format(valid_params))
+            raise DTError('family_param error, must be one of {}'.format(valid_params))
         if iso_param not in valid_params and iso_param is not None:
-            raise Error('iso_param error, must be one of {}'.format(valid_params))
+            raise DTError('iso_param error, must be one of {}'.format(valid_params))
 
         if fig is None:
             fig = plt.figure(figsize=[10, 8])
             ax = fig.add_subplot(111)
         else:
             ax = fig.axes[0]
 
@@ -1173,8 +1175,8 @@
         fnames = self.get_wvel_files(fullpath=False)
         for fname in fnames:
             vel_key, rpm_key = [float(num) for num in fname.strip('velo_').strip('.wvel').split('_rpm_')]
             vel_key /= 100
             wvel_fullpath = os.path.join(self.directory, fname)
             d[(vel_key, rpm_key)] = funcs.read_xrotor_wvel_file(fpath=wvel_fullpath)
         if verbose and len(fnames) > 0:
-            Info('Loaded Existing WVel Results (.wvel)!', indent_level=1)
+            DTInfo('Loaded Existing WVel Results (.wvel)!', indent_level=1)
```

### Comparing `propeller_design_tools-0.4.6/propeller_design_tools/radialstation.py` & `propeller_design_tools-0.4.7/propeller_design_tools/radialstation.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 import os
-from propeller_design_tools import funcs
-from propeller_design_tools.airfoil import Airfoil
-from propeller_design_tools.user_io import Info, Error
+
 import matplotlib.pyplot as plt
 import numpy as np
 from scipy.optimize import curve_fit
 
+from propeller_design_tools import funcs
+from propeller_design_tools.airfoil import Airfoil
+from propeller_design_tools.user_io import DTInfo, DTError
+
 
 class RadialStation(object):
 
     req_xrotor_attrs = ['A0deg', 'dCLdA', 'dCLdAstall', 'CLmax', 'CLmin', 'CLinc2stall', 'CDmin', 'CLCDmin',
                         'dCDdCL2', 'REref', 'REexp', 'Cmconst', 'Mcrit']
 
     def __init__(self, station_idx: int = None, foil: Airfoil = None, re_estimate: int = None,
@@ -29,39 +31,39 @@
 
         # initialize required attrs as None
         self.A0deg, self.dCLdA, self.dCLdAstall, self.CLmax, self.CLmin, self.CLinc2stall, self.CDmin, self.CLCDmin, \
         self.dCDdCL2, self.REref, self.REexp, self.Cmconst, self.Mcrit = [None] * 13
 
         # need to give re_estimate
         if re_estimate is None:
-            raise Error('Must give an Re estimate at which to interpolate data / at which data was obtained')
+            raise DTError('Must give an Re estimate at which to interpolate data / at which data was obtained')
 
         # kick em out if no airfoil or no polar given
         if foil is None and foil_polar is None:
-            raise Error('Must give an Airfoil() or foil polar data as an input into RadialStation()')
+            raise DTError('Must give an Airfoil() or foil polar data as an input into RadialStation()')
             # for attr in self.req_xrotor_attrs:
             #     if attr not in xrotor_kwargs:
-            #         raise Error('Required argument "{}" not given'.format(attr))
+            #         raise DTError('Required argument "{}" not given'.format(attr))
             #     else:   # set the required inputs if one was given though
             #         setattr(self, attr, xrotor_kwargs[attr])
         # kick em out if both given
         elif foil is not None and foil_polar is not None:
-            raise Error('Cannot give both foil and foil_polar as inputs into RadialStation()')
+            raise DTError('Cannot give both foil and foil_polar as inputs into RadialStation()')
         elif isinstance(foil, Airfoil):  # initialize all the req_attrs automatically from airfoil's data
             if verbose:
-                Info('Initializing RadialStation() from foil "{}" interpolated @ Re={}'
-                     .format(self.foil.name, self.re_estimate))
+                DTInfo('Initializing RadialStation() from foil "{}" interpolated @ Re={}'
+                .format(self.foil.name, self.re_estimate))
             self.init_from_airfoil(foil=foil, re_estimate=re_estimate, plot_also=plot, verbose=verbose)
         elif isinstance(foil_polar, dict):  # initialize all req_attrs automatically from polar data
             if verbose:
-                Info('Initializing RadialStation() from given polar data @ Re={}'.format(self.re_estimate))
+                DTInfo('Initializing RadialStation() from given polar data @ Re={}'.format(self.re_estimate))
             self.init_from_polar(polar=foil_polar, plot_also=plot, verbose=verbose)
         else:
             inp = 'foil' if foil is not None else 'foil_polar'
-            raise Error('Input type not recognized for {}'.format(inp))
+            raise DTError('Input type not recognized for {}'.format(inp))
 
     @property
     def foil_name(self):
         if isinstance(self.foil, Airfoil):
             return self.foil.name
         else:
             return self.foil_name_str
@@ -188,18 +190,18 @@
         # pitching moment
         self.Cmconst = np.average(pol['CM'][min_idx:pre_stall_idx])
         self.REref = pol['re']
         self.REexp = funcs.get_xrotor_re_scaling_exp(re=pol['re'])
         self.Mcrit = 1
 
         if verbose:
-            Info('Found required XROTOR section inputs ->')
+            DTInfo('Found required XROTOR section inputs ->')
             for attr in self.req_xrotor_attrs:
                 val = getattr(self, attr)
-                Info('{}: {}'.format(attr, val), indent_level=1)
+                DTInfo('{}: {}'.format(attr, val), indent_level=1)
 
         return min_idx, pre_stall_idx
 
     def plot_xrotor_fit_params(self, fig=None):
         pol = self.foil_polar
         idx_lims = self.idx_lims
```

### Comparing `propeller_design_tools-0.4.6/propeller_design_tools/science_spinbox_class.py` & `propeller_design_tools-0.4.7/propeller_design_tools/science_spinbox_class.py`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.6/propeller_design_tools/settings.py` & `propeller_design_tools-0.4.7/propeller_design_tools/settings.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,15 @@
-import sys
 import os
-from propeller_design_tools.user_io import Error, Input, Info
+from propeller_design_tools.user_io import DTError
+import pkg_resources
+import os
+
 import pkg_resources
 
+from propeller_design_tools.user_io import DTError
 
 VALID_OPER_PLOT_PARAMS = ['adv. ratio', 'J', 'speed(m/s)', 'rpm', 'thrust(N)', 'power(W)', 'torque(N-m)', 'Efficiency',
                           'Eff induced', 'Eff ideal', 'Pvisc(W)', 'Ct', 'Tc', 'Cp', 'Pc', 'Sigma']
 
 
 def set_airfoil_database(path: str):
     _save_settings({'airfoil_database': path})
@@ -23,32 +26,34 @@
     if os.path.isdir(usr_db):
         return usr_db
     else:
         def_db = _get_default_propeller_database()
         if os.path.isdir(def_db):
             return def_db
         else:
-            raise Error('Cannot find either propeller database option (user-set = "{}", default = "{}")'.format(usr_db, def_db))
+            raise DTError(
+                'Cannot find either propeller database option (user-set = "{}", default = "{}")'.format(usr_db, def_db))
 
 
 def get_foil_db():
     usr_db = _get_user_settings()['airfoil_database']
     if os.path.isdir(usr_db):
         return usr_db
     else:
         def_db = _get_default_airfoil_database()
         if os.path.isdir(def_db):
             return def_db
         else:
-            raise Error('Cannot find either airfoil database option (user-set = "{}", default = "{}")'.format(usr_db, def_db))
+            raise DTError(
+                'Cannot find either airfoil database option (user-set = "{}", default = "{}")'.format(usr_db, def_db))
 
 
 def get_setting(s: str):
     if s not in _get_user_settings():
-        raise Error('"" is not a known PDT setting'.format(s))
+        raise DTError('"" is not a known PDT setting'.format(s))
     else:
         return _get_user_settings()[s]
 
 
 def _get_cursor_fpath():
     fname = pkg_resources.resource_filename(__name__, 'supporting_files/crosshair_cursor.png')
     return fname
```

### Comparing `propeller_design_tools-0.4.6/propeller_design_tools/supporting_files/crosshair_cursor.png` & `propeller_design_tools-0.4.7/propeller_design_tools/supporting_files/crosshair_cursor.png`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.6/propeller_design_tools/supporting_files/gunshot1.wav` & `propeller_design_tools-0.4.7/propeller_design_tools/supporting_files/gunshot1.wav`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.6/propeller_design_tools/supporting_files/gunshot2.wav` & `propeller_design_tools-0.4.7/propeller_design_tools/supporting_files/gunshot2.wav`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.6/propeller_design_tools/supporting_files/gunshot3.wav` & `propeller_design_tools-0.4.7/propeller_design_tools/supporting_files/gunshot3.wav`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.6/propeller_design_tools/supporting_files/gunshot4.wav` & `propeller_design_tools-0.4.7/propeller_design_tools/supporting_files/gunshot4.wav`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.6/propeller_design_tools/user_interface.py` & `propeller_design_tools-0.4.7/propeller_design_tools/user_interface.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,25 +1,32 @@
+"""
+File containing all the UI (user-interface) elements of the code
+"""
 import numpy as np
-import os
-import subprocess
+
 from propeller_design_tools.airfoil import Airfoil
+from propeller_design_tools.funcs import get_all_airfoil_files
 from propeller_design_tools.settings import _get_cursor_fpath, _get_gunshot_fpaths
-from propeller_design_tools.funcs import get_all_airfoil_files, get_all_propeller_dirs
+# import os
+# import subprocess
+from propeller_design_tools.user_io import DTWarning
+
 try:
     from PyQt5 import QtWidgets, QtGui, QtCore, QtMultimedia
-    from propeller_design_tools.helper_ui_classes import Capturing, DatabaseSelectionWidget, SingleAxCanvas, \
-        AxesComboBoxWidget, PdtGuiPrinter
-    from propeller_design_tools.foil_ui_classes import ExistingFoilDataWidget, FoilAnalysisWidget, AddFoilDataPointWidget
+    from propeller_design_tools.helper_ui_classes import (Capturing, DatabaseSelectionWidget, SingleAxCanvas,
+        AxesComboBoxWidget, PdtGuiPrinter)
+    from propeller_design_tools.foil_ui_classes import (ExistingFoilDataWidget, FoilAnalysisWidget,
+        AddFoilDataPointWidget)
     from propeller_design_tools.prop_creation_ui_classes import PropellerCreationWidget
     from propeller_design_tools.prop_analysis_ui_classes import PropellerSweepWidget
     from propeller_design_tools.opt_ui_classes import OptimizationWidget
-    from propeller_design_tools.helper_ui_subclasses import PDT_TextEdit, PDT_GroupBox, PDT_Label, PDT_PushButton, \
-        PDT_ComboBox, PDT_TabWidget
+    from propeller_design_tools.helper_ui_subclasses import (PDT_TextEdit, PDT_GroupBox, PDT_Label, PDT_PushButton,
+        PDT_ComboBox, PDT_TabWidget)
 except:
-    pass
+    raise DTWarning('Unable to import a package required for the GUI -> this may cause errors in the future.')
 
 
 class InterfaceMainWindow(QtWidgets.QMainWindow):
     def __init__(self, foil: Airfoil = None):
         super(InterfaceMainWindow, self).__init__()
         self.setWindowTitle('PDT Control Dashboard')
         self.setMinimumSize(1600, 900)
```

### Comparing `propeller_design_tools-0.4.6/propeller_design_tools/user_io.py` & `propeller_design_tools-0.4.7/propeller_design_tools/user_io.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,19 @@
+# ===== PDT - SPECIFIC ERRORS =====
+class PDTError(Exception):
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+
+
 # ===== PDT - SPECIFIC USER DIALOGUES =====
-def Warning(s: str):
+def DTWarning(s: str):
     print('PDT WARNING: {}'.format(s))
 
 
-def Info(s: str, indent_level: int = 0):
+def DTInfo(s: str, indent_level: int = 0):
     ind_txt = '    ' * indent_level
     offset_spaces = '          '
     print('PDT INFO: {}{}'.format(ind_txt, s.replace('\n', '\n{}{}'.format(offset_spaces, ind_txt))))
 
 
 def error_plot(**kwargs):
 
@@ -54,37 +60,32 @@
     if ax0_is_plot:
         axes[0].grid(True)
         axes[0].set_title('PDT Troubleshooting Plot')
         axes[0].set_xlabel(xlbl)
         axes[0].set_ylabel(ylbl)
         axes[0].plot(x, y)
 
-        axes[1].set_title('PDT Troubleshooting Info')
+        axes[1].set_title('PDT Troubleshooting DTInfo')
         axes[1].axes.xaxis.set_visible(False)
         axes[1].axes.yaxis.set_visible(False)
         if info_d is not None:
             plot_info_dict(ax=axes[1], info_dict=info_d)
 
     else:
         for ax in axes:
-            ax.set_title('PDT Troubleshooting Info')
+            ax.set_title('PDT Troubleshooting DTInfo')
             ax.axes.xaxis.set_visible(False)
             ax.axes.yaxis.set_visible(False)
 
         if info_d is not None:
             plot_info_dict(ax=axes[0], info_dict=info_d)
             if info_d2 is not None:
                 plot_info_dict(ax=axes[1], info_dict=info_d2)
 
     return fig
 
 
-class Error(Exception):
+class DTError(Exception):
     def __init__(self, s: str, errplot: bool = False, **errplot_kwargs):
         if errplot:
             error_plot(**errplot_kwargs)
         super().__init__('\nPDT ERROR: {}'.format(s.replace('\n', '\n           ')))
-
-
-class Input:
-    def __init__(self, s: str):
-        self.response = input('\n PDT INPUT: {}'.format(s.replace('\n', '\n           ')))
```

### Comparing `propeller_design_tools-0.4.6/propeller_design_tools.egg-info/PKG-INFO` & `propeller_design_tools-0.4.7/propeller_design_tools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: propeller-design-tools
-Version: 0.4.6
+Version: 0.4.7
 Summary: Python 3.7 package that provides exactly what it sounds like by automating usage of MIT professor Mark Drela's GNU-licensed CLI-utilities XFOIL and XROTOR.
 Author-email: Jacob Bronson <bronsoneering@gmail.com>
 License: GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -700,131 +700,96 @@
 ---
 **Work in progress / incomplete documentation (all current documentation is below, as well as a step-by-step typical 
 usage/workflow scenario)**
 
 Note: The graphical user interface for this should be functional for Linux now as well!
 
 ---
-
 Description
 ===========
 Python 3.7 package that provides exactly what it sounds like by automating usage of the GPL-licensed 
 CLI-utilities XFOIL and XROTOR.
 
 Both utilities are published by professor Mark Drela (MIT).
+
 - XFOIL: for arbitrary 2D airfoil analysis and design
 - XROTOR: for arbitrary propeller design schemes and analysis
 
-XFOIL and XROTOR Executables
--------------------------------------------
-In order to utilize any PDT functionality that depends on
-running XFOIL, the "xfoil.exe" executable file needs to be
-in the user-set "airfoil_database" location. *Current pip
-installations include the xfoil.exe file in the foil_database,
-there should theoretically be no need to download it manually,
-even if the user changes the foil_database location.*
-
-[XFOIL executable and docs](https://web.mit.edu/drela/Public/web/xfoil/)
-
-Likewise, in order to utilize any PDT functionality that
-depends on running XROTOR, the "xrotor.exe" executable file
-needs to be in the user-set "propeller_database" location.
-*Current pip installations include the xrotor.exe file in the
-default prop_database, there should theoretically be no need to
-download it manually, even if the user changes the prop_database
-location.*
-
-[CROTOR executable and docs](http://www.esotec.org/sw/crotor.html#download)
-*(this is actually a link to "CROTOR", which I find is
-the easiest way to obtain a windows-executable of XROTOR)*
-
-[actual XROTOR docs](https://web.mit.edu/drela/Public/web/xrotor/xrotor_doc.txt)
-
-Both XFOIL and XROTOR contain much, much more utility than PDT currently has integrated. They are part of an incredible
-set of aerodynamic (or hydrodynamic) modeling command-line-interface (CLI) utilities from MIT. The ones that I 
-personally know of include:
-1. XFOIL - for arbitrary 2D airfoil analysis and design
-2. XROTOR - for arbitrary propeller design schemes and analysis
-3. AVL - for arbitrary lifting planform analysis
-4. QPROP - another CLI utility for propeller design and analysis
-5. QMIL - for arbitrary windmill designs (and more)
-
-Combined, the above represents an amazing fluid-dynamics modeling capability that is completely free, and fast. While 
-it's unlikely they will ever get as accurate as true computational-fluid-dynamics (CFD) software, they still offer 
-great value for being free, and are several orders of magnitude faster than true CFD software. Personally, I have found
-them to be completely sufficient tools for all stages of engineering design, but then again I have only ever worked in 
-prototyping engineering.
-
+---
 Troubleshooting PDT Errors / Crashes (GUI and/or Scripting)
 ===========================================================
-So I just quit my job as a systems engineer to become a software developer, so hopefully this package starts to get 
+So I just quit my job as a systems engineer to become a software developer, so hopefully this package starts to get
 more frequent updates and support from me. If you encounter what you think is an error coming from this code, I would
 love to know about it, please submit an issue to:
 
 [LINK TO GITHUB ISSUES](https://github.com/helloDestroyerOfWorlds/propeller_design_tools/issues)
 
-and I will likely see it quickly and will at least answer you, if not just fix it and push the update. Please only do 
+and I will likely see it quickly and will at least answer you, if not just fix it and push the update. Please only do
 this though once you are sure the error is coming from the PDT code.
 
-If you think you have discovered a legitimate issue, before submitting it please also read through the list below to 
+If you think you have discovered a legitimate issue, before submitting it please also read through the list below to
 see if any of the listed things could fix your error.
 
-1. XFOIL or XROTOR executables: Errors might be coming from XFOIL or XROTOR in actuality rather than this source code 
-   - Currently PDT implements these as executables installed when pip installing this package
-   - This means if you are having pip install errors and are on Linux it might be caused by that, actually, if you are 
-     having any errors, even in the GUI, and you are on Linux it might be caused by me not understanding until now much 
-     about Linux. If this is the case, and you think you know what is causing the error, please feel free to reach out 
-     to me via the issues link above.
-   - Additionally, I just implemented a fix to automatically install all required dependencies when pip installing this 
-     package. This should fix many issues for Linux users, if not all the current ones. Note that if you want to use the
-     GUI, read the next point.
-   - Still submit an issue using the link above if this is the case -> in theory I can detect most of these
+1. XFOIL or XROTOR executables: Errors might be coming from XFOIL or XROTOR in actuality rather than this source code
+    - Currently PDT implements these as executables installed when pip installing this package
+    - This means if you are having pip install errors and are on Linux it might be caused by that, actually, if you are
+      having any errors, even in the GUI, and you are on Linux it might be caused by me not understanding until now much
+      about Linux. If this is the case, and you think you know what is causing the error, please feel free to reach out
+      to me via the issues link above.
+    - Additionally, I just implemented a fix to automatically install all required dependencies when pip installing this
+      package. This should fix many issues for Linux users, if not all the current ones. Note that if you want to use
+      the
+      GUI, read the next point.
+    - Still submit an issue using the link above if this is the case -> in theory I can detect most of these
 
 2. Did not install GUI version: To enable the ability to use the graphical-user-interface (GUI) you must:
 
-    `pip install propeller_design_tools[gui]` - or - `pip install --upgrade propeller_design_tools[gui]`
+   `pip install propeller_design_tools[gui]` - or - `pip install --upgrade propeller_design_tools[gui]`
 
-3. You're asking for an "impossible" propeller: XROTOR will error in this case.  
-   - Impossible in terms of the pure physics of what you're asking for (asking for too much thrust / power essentially)
-   - PDT has no way to know if your propeller is impossible, so I'm not sure how I could ever wrap this error in an 
-     appropriate python error wrapper even.
-   - I highly recommend to use only the "constant" blade cl distribution target option
-     - I have not had time yet to test any of the other options much
-     - Other options are disabled in the GUI until I can test them fully
-     - Other options in the future will be a "linear" option as well as "file" option (which essentially allows the 
-     - user to define an arbitrary, discreet function for the blade Cl distribution).
-   - It is also highly recommended to use only the 'grad' or 'pot' solver options until you know you have the code at 
-     least generating an output without failing. 
-     - I would only then recommend moving on to using the 'vrtx' solver. This solver is (in my opinion) the superior of 
-       the 3 options. Though it takes longest to solve by far, it seems to be the only one that reliably produces 
-       reasonable chord lengths near the hub. I think the 'vrtx' solver is somewhat less stable than the other two as 
-       well, so if you think you're having errors with PDT try to switch solvers.
+3. You're asking for an "impossible" propeller: XROTOR will error in this case.
+    - Impossible in terms of the pure physics of what you're asking for (asking for too much thrust / power essentially)
+    - PDT has no way to know if your propeller is impossible, so I'm not sure how I could ever wrap this error in an
+      appropriate python error wrapper even.
+    - I highly recommend to use only the "constant" blade cl distribution target option
+        - I have not had time yet to test any of the other options much
+        - Other options are disabled in the GUI until I can test them fully
+        - Other options in the future will be a "linear" option as well as "file" option (which essentially allows the
+        - user to define an arbitrary, discreet function for the blade Cl distribution).
+    - It is also highly recommended to use only the 'grad' or 'pot' solver options until you know you have the code at
+      least generating an output without failing.
+        - I would only then recommend moving on to using the 'vrtx' solver. This solver is (in my opinion) the superior
+          of
+          the 3 options. Though it takes longest to solve by far, it seems to be the only one that reliably produces
+          reasonable chord lengths near the hub. I think the 'vrtx' solver is somewhat less stable than the other two as
+          well, so if you think you're having errors with PDT try to switch solvers.
 
 4. You're asking for XFOIL to analyze your airfoil at too low or too high of an angle-of-attack (AoA)
-   - I have attempted to remove the need for the user to enter AoA, but my algorithm for this is far from perfect.
-   - If you think this is your error, please submit it via issue link above.
+    - I have attempted to remove the need for the user to enter AoA, but my algorithm for this is far from perfect.
+    - If you think this is your error, please submit it via issue link above.
 
 5. You're trying to open the STL file generated by PDT in SolidWorks: this is a known issue currently being worked on.
    - I've no idea why this happens, it seems to be a purely SolidWorks issue, the STL file seems to open just fine in
      everything else I have tried.
    - Try opening the file and re-saving it (I suggest MS Paint, I think the new version can save STLs).
    - Try opening the file and re-saving it after having very slightly changed it.
    - If you encounter this error but think you have figured it out or have useful information about it please submit an
      issue via the link above.
 
 Thank you all that is my TED talk.
 
+---
 Purpose
 =======
 PDT seeks to provide the user a set of python3 utilities that can be used for arbitrary scripting efforts to automate
 usage of both XFOIL and XROTOR while implementing its own unique python3-native algorithms to maintain local
 input files, meta files, databases, and results files and weave everything together for the user in a simple,
 meaningful way to aid in the initial / investigatory stage of well-behaved propeller designs (free-flow and non-ducted
 assumptions).
 
+---
 Getting Started
 ===============
 Installation
 ------------
 `pip install propeller_design_tools` - or - `pip install propeller_design_tools[gui]`
 
 Update
@@ -842,20 +807,21 @@
 `pdt.set_propeller_database(path: str)`
 
 **The user must set these two directories at the top of every script right after the imports**
 
 *The airfoil directory will be used to store any foil / XFOIL-related support files, and the propeller directory
 will be used similarly to store any propeller / XROTOR-related support files.*
 
+---
 Example Scripts / Workflow
 --------------------------
 At a high-level, the current concept for the PDT workflow is as follows (after pip-installing the PDT package):
 
 0. Try out the (currently extremely buggy and incomplete) user interface!
-[example0_user_interface.py](
+   [example0_user_interface.py](
    https://github.com/helloDestroyerOfWorlds/propeller_design_tools/blob/master/tests/example0_user_interface.py)
 
    ![ex0-1](./tests/ex0-1.png)
    ![ex0-2](./tests/ex0-2.png)
    ![ex0-3](./tests/ex0-3.png)
 
 
@@ -903,21 +869,63 @@
 [example4_stl_generation.py](
    https://github.com/helloDestroyerOfWorlds/propeller_design_tools/blob/master/tests/example4_stl_generation.py
    )
 
    ![ex4-1](./tests/ex4-1.png)
 
 
-5. Analyze a given `Propeller()` instance across a sweep of operating points -> see 
-[example5_prop_analysis.py](
+5. Analyze a given `Propeller()` instance across a sweep of operating points -> see
+   [example5_prop_analysis.py](
    https://github.com/helloDestroyerOfWorlds/propeller_design_tools/blob/master/tests/example5_prop_analysis.py
    )
 
    ![ex5-1](./tests/ex5-1.png)
 
 
-6. **WIP** Prop optimization 
-   - Will be a grid-search style generic optimizer for "optimal" prop design generation by means of minimizing overall 
-     energy usage. 
-   - Optionally takes into account different propeller operating points via the ability to define the propeller's 
-     "duty-cycle"
-     - This feature is coming soon! 
+6. **WIP** Prop optimization
+    - Will be a grid-search style generic optimizer for "optimal" prop design generation by means of minimizing overall
+      energy usage.
+    - Optionally takes into account different propeller operating points via the ability to define the propeller's
+      "duty-cycle"
+        - This feature is coming soon!
+
+---
+XFOIL, XROTOR and other MIT Aero-Modeling Executables
+-----------------------------------------------------
+In order to utilize any PDT functionality that depends on
+running XFOIL, the "xfoil.exe" executable file needs to be
+in the user-set "airfoil_database" location. *Current pip
+installations include the xfoil.exe file in the foil_database,
+there should theoretically be no need to download it manually,
+even if the user changes the foil_database location.*
+
+[XFOIL executable and docs](https://web.mit.edu/drela/Public/web/xfoil/)
+
+Likewise, in order to utilize any PDT functionality that
+depends on running XROTOR, the "xrotor.exe" executable file
+needs to be in the user-set "propeller_database" location.
+*Current pip installations include the xrotor.exe file in the
+default prop_database, there should theoretically be no need to
+download it manually, even if the user changes the prop_database
+location.*
+
+[CROTOR executable and docs](http://www.esotec.org/sw/crotor.html#download)
+*(this is actually a link to "CROTOR", which I find is
+the easiest way to obtain a windows-executable of XROTOR)*
+
+[actual XROTOR docs](https://web.mit.edu/drela/Public/web/xrotor/xrotor_doc.txt)
+
+Both XFOIL and XROTOR contain much, much more utility than PDT currently has integrated. They are part of an incredible
+set of aerodynamic (or hydrodynamic) modeling command-line-interface (CLI) utilities from MIT. The ones that I
+personally know of include:
+
+1. XFOIL - for arbitrary 2D airfoil analysis and design
+2. XROTOR - for arbitrary propeller design schemes and analysis
+3. AVL - for arbitrary lifting planform analysis
+4. QPROP - another CLI utility for propeller design and analysis
+5. QMIL - for arbitrary windmill designs (and more)
+
+Combined, the above represents an amazing fluid-dynamics modeling capability that is completely free, and fast. While
+it's unlikely they will ever get as accurate as true computational-fluid-dynamics (CFD) software, they still offer
+great value for being free, and are several orders of magnitude faster than true CFD software. Personally, I have found
+them to be completely sufficient tools for all stages of engineering design, but then again I have only ever worked in
+prototyping engineering.
```

### Comparing `propeller_design_tools-0.4.6/propeller_design_tools.egg-info/SOURCES.txt` & `propeller_design_tools-0.4.7/propeller_design_tools.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 propeller_design_tools/__init__.py
 propeller_design_tools/airfoil.py
 propeller_design_tools/custom_opengl_classes.py
 propeller_design_tools/foil_ui_classes.py
 propeller_design_tools/funcs.py
 propeller_design_tools/helper_ui_classes.py
 propeller_design_tools/helper_ui_subclasses.py
+propeller_design_tools/mobapp.py
 propeller_design_tools/opt_ui_classes.py
 propeller_design_tools/optimizations.py
 propeller_design_tools/prop_analysis_ui_classes.py
 propeller_design_tools/prop_creation_ui_classes.py
 propeller_design_tools/propeller.py
 propeller_design_tools/radialstation.py
 propeller_design_tools/science_spinbox_class.py
```

### Comparing `propeller_design_tools-0.4.6/pyproject.toml` & `propeller_design_tools-0.4.7/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [build-system]
 requires = ["setuptools>=67.8.0", "wheel>=0.40.0"]  # build requirements (don't include build or twine)
 build-backend = "setuptools.build_meta"
 
 
 [project]
-version = "0.4.6"                       # increment version number before pushing to pypi
+version = "0.4.7"                       # increment version number before pushing to pypi
 name = "propeller_design_tools"
-authors = [{name = "Jacob Bronson", email = "bronsoneering@gmail.com"}]
+authors = [{ name = "Jacob Bronson", email = "bronsoneering@gmail.com" }]
 description = "Python 3.7 package that provides exactly what it sounds like by automating usage of MIT professor Mark Drela's GNU-licensed CLI-utilities XFOIL and XROTOR."
 readme = "README.md"
 requires-python = ">=3.7"
 keywords = ['propeller', 'design', 'tools', 'computational', 'fluid', 'dynamics', 'CFD', 'STL', 'prop', 'rotor',
-            'xrotor', 'xfoil', 'MIT', 'Drela', 'Youngren', 'engineering', 'aero', 'dynamic', 'aerodynamic',
-            'hydrodynamic']
-license = {file = "LICENSE"}
+    'xrotor', 'xfoil', 'MIT', 'Drela', 'Youngren', 'engineering', 'aero', 'dynamic', 'aerodynamic',
+    'hydrodynamic']
+license = { file = "LICENSE" }
 
 classifiers = [
     "Intended Audience :: Science/Research",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Natural Language :: English",
     "Programming Language :: Python :: 3",
     "Operating System :: Microsoft :: Windows",
```

