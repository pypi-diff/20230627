# Comparing `tmp/scikit-rt-0.5.1.tar.gz` & `tmp/scikit-rt-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scikit-rt-0.5.1.tar", last modified: Tue Jun 27 09:58:37 2023, max compression
+gzip compressed data, was "scikit-rt-0.5.2.tar", last modified: Tue Jun 27 10:58:28 2023, max compression
```

## Comparing `scikit-rt-0.5.1.tar` & `scikit-rt-0.5.2.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:58:37.967545 scikit-rt-0.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)    35129 2023-06-27 09:54:26.000000 scikit-rt-0.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-06-27 09:58:37.967545 scikit-rt-0.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-06-27 09:54:26.000000 scikit-rt-0.5.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-06-27 09:54:26.000000 scikit-rt-0.5.1/pypi.md
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-27 09:54:26.000000 scikit-rt-0.5.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-06-27 09:58:37.967545 scikit-rt-0.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-27 09:54:26.000000 scikit-rt-0.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:58:37.939545 scikit-rt-0.5.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:58:37.943545 scikit-rt-0.5.1/src/scikit_rt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-06-27 09:58:37.000000 scikit-rt-0.5.1/src/scikit_rt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-06-27 09:58:37.000000 scikit-rt-0.5.1/src/scikit_rt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 09:58:37.000000 scikit-rt-0.5.1/src/scikit_rt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-06-27 09:58:37.000000 scikit-rt-0.5.1/src/scikit_rt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-27 09:58:37.000000 scikit-rt-0.5.1/src/scikit_rt.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:58:37.951545 scikit-rt-0.5.1/src/skrt/
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-06-27 09:54:26.000000 scikit-rt-0.5.1/src/skrt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12816 2023-06-27 09:54:26.000000 scikit-rt-0.5.1/src/skrt/application.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:58:37.955545 scikit-rt-0.5.1/src/skrt/better_viewer/
--rw-r--r--   0 runner    (1001) docker     (123)   132535 2023-06-27 09:54:26.000000 scikit-rt-0.5.1/src/skrt/better_viewer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3958 2023-06-27 09:54:26.000000 scikit-rt-0.5.1/src/skrt/better_viewer/options.py
--rw-r--r--   0 runner    (1001) docker     (123)    76116 2023-06-27 09:54:26.000000 scikit-rt-0.5.1/src/skrt/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:58:37.943545 scikit-rt-0.5.1/src/skrt/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:58:37.955545 scikit-rt-0.5.1/src/skrt/data/elastix_parameter_files/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1732 2023-06-27 09:54:26.000000 scikit-rt-0.5.1/src/skrt/data/elastix_parameter_files/BE_BSpline05.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)     1801 2023-06-27 09:54:26.000000 scikit-rt-0.5.1/src/skrt/data/elastix_parameter_files/MI_Affine.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)     1649 2023-06-27 09:54:26.000000 scikit-rt-0.5.1/src/skrt/data/elastix_parameter_files/MI_BSpline05.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)     1650 2023-06-27 09:54:26.000000 scikit-rt-0.5.1/src/skrt/data/elastix_parameter_files/MI_BSpline15.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)     1650 2023-06-27 09:54:26.000000 scikit-rt-0.5.1/src/skrt/data/elastix_parameter_files/MI_BSpline30.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)     1798 2023-06-27 09:54:26.000000 scikit-rt-0.5.1/src/skrt/data/elastix_parameter_files/MI_Rigid.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)     1804 2023-06-27 09:54:26.000000 scikit-rt-0.5.1/src/skrt/data/elastix_parameter_files/MI_Translation.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:58:37.955545 scikit-rt-0.5.1/src/skrt/data/niftyreg_parameter_files/
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-06-27 09:54:26.000000 scikit-rt-0.5.1/src/skrt/data/niftyreg_parameter_files/Affine.txt
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-27 09:54:26.000000 scikit-rt-0.5.1/src/skrt/data/niftyreg_parameter_files/BE_BSpline05.txt
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-27 09:54:26.000000 scikit-rt-0.5.1/src/skrt/data/niftyreg_parameter_files/NMI_BSpline05.txt
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-27 09:54:26.000000 scikit-rt-0.5.1/src/skrt/data/niftyreg_parameter_files/NMI_BSpline15.txt
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-27 09:54:26.000000 scikit-rt-0.5.1/src/skrt/data/niftyreg_parameter_files/NMI_BSpline30.txt
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-06-27 09:54:26.000000 scikit-rt-0.5.1/src/skrt/data/niftyreg_parameter_files/Rigid.txt
--rw-r--r--   0 runner    (1001) docker     (123)    27334 2023-06-27 09:54:26.000000 scikit-rt-0.5.1/src/skrt/dicom_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)    39944 2023-06-27 09:54:26.000000 scikit-rt-0.5.1/src/skrt/dose.py
--rw-r--r--   0 runner    (1001) docker     (123)   257103 2023-06-27 09:54:26.000000 scikit-rt-0.5.1/src/skrt/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-06-27 09:54:26.000000 scikit-rt-0.5.1/src/skrt/multi.py
--rw-r--r--   0 runner    (1001) docker     (123)   118936 2023-06-27 09:54:26.000000 scikit-rt-0.5.1/src/skrt/patient.py
--rw-r--r--   0 runner    (1001) docker     (123)   152018 2023-06-27 09:54:26.000000 scikit-rt-0.5.1/src/skrt/registration.py
--rw-r--r--   0 runner    (1001) docker     (123)    60958 2023-06-27 09:54:26.000000 scikit-rt-0.5.1/src/skrt/segmentation.py
--rw-r--r--   0 runner    (1001) docker     (123)    25041 2023-06-27 09:54:26.000000 scikit-rt-0.5.1/src/skrt/simulation.py
--rw-r--r--   0 runner    (1001) docker     (123)   358501 2023-06-27 09:54:26.000000 scikit-rt-0.5.1/src/skrt/structures.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:58:37.959545 scikit-rt-0.5.1/src/skrt/viewer/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-27 09:54:26.000000 scikit-rt-0.5.1/src/skrt/viewer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   154795 2023-06-27 09:54:26.000000 scikit-rt-0.5.1/src/skrt/viewer/core.py
--rw-r--r--   0 runner    (1001) docker     (123)   113136 2023-06-27 09:54:26.000000 scikit-rt-0.5.1/src/skrt/viewer/viewer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:58:37.963545 scikit-rt-0.5.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-06-27 09:54:26.000000 scikit-rt-0.5.1/tests/test_01_setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    10063 2023-06-27 09:54:26.000000 scikit-rt-0.5.1/tests/test_application.py
--rw-r--r--   0 runner    (1001) docker     (123)    15414 2023-06-27 09:54:26.000000 scikit-rt-0.5.1/tests/test_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     7248 2023-06-27 09:54:26.000000 scikit-rt-0.5.1/tests/test_dose.py
--rw-r--r--   0 runner    (1001) docker     (123)    61981 2023-06-27 09:54:26.000000 scikit-rt-0.5.1/tests/test_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-06-27 09:54:26.000000 scikit-rt-0.5.1/tests/test_multi.py
--rw-r--r--   0 runner    (1001) docker     (123)     9592 2023-06-27 09:54:26.000000 scikit-rt-0.5.1/tests/test_patient.py
--rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-06-27 09:54:26.000000 scikit-rt-0.5.1/tests/test_qv_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     8791 2023-06-27 09:54:26.000000 scikit-rt-0.5.1/tests/test_qv_quickviewer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6165 2023-06-27 09:54:26.000000 scikit-rt-0.5.1/tests/test_qv_struct_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     3876 2023-06-27 09:54:26.000000 scikit-rt-0.5.1/tests/test_qv_struct_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-06-27 09:54:26.000000 scikit-rt-0.5.1/tests/test_qv_structs.py
--rw-r--r--   0 runner    (1001) docker     (123)    34841 2023-06-27 09:54:26.000000 scikit-rt-0.5.1/tests/test_registration.py
--rw-r--r--   0 runner    (1001) docker     (123)    21138 2023-06-27 09:54:26.000000 scikit-rt-0.5.1/tests/test_roi_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     5429 2023-06-27 09:54:26.000000 scikit-rt-0.5.1/tests/test_segmentation.py
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-27 09:54:26.000000 scikit-rt-0.5.1/tests/test_simulation.py
--rw-r--r--   0 runner    (1001) docker     (123)    65888 2023-06-27 09:54:26.000000 scikit-rt-0.5.1/tests/test_structs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2513 2023-06-27 09:54:26.000000 scikit-rt-0.5.1/tests/test_synthetic_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     7725 2023-06-27 09:54:26.000000 scikit-rt-0.5.1/tests/test_viewer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:58:28.360134 scikit-rt-0.5.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    35129 2023-06-27 10:54:20.000000 scikit-rt-0.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-06-27 10:58:28.360134 scikit-rt-0.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-06-27 10:54:20.000000 scikit-rt-0.5.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-06-27 10:54:20.000000 scikit-rt-0.5.2/pypi.md
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-27 10:54:20.000000 scikit-rt-0.5.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-06-27 10:58:28.360134 scikit-rt-0.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-27 10:54:20.000000 scikit-rt-0.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:58:28.332134 scikit-rt-0.5.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:58:28.336134 scikit-rt-0.5.2/src/scikit_rt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-06-27 10:58:28.000000 scikit-rt-0.5.2/src/scikit_rt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-06-27 10:58:28.000000 scikit-rt-0.5.2/src/scikit_rt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 10:58:28.000000 scikit-rt-0.5.2/src/scikit_rt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-06-27 10:58:28.000000 scikit-rt-0.5.2/src/scikit_rt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-27 10:58:28.000000 scikit-rt-0.5.2/src/scikit_rt.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:58:28.344134 scikit-rt-0.5.2/src/skrt/
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-06-27 10:54:20.000000 scikit-rt-0.5.2/src/skrt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12816 2023-06-27 10:54:20.000000 scikit-rt-0.5.2/src/skrt/application.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:58:28.344134 scikit-rt-0.5.2/src/skrt/better_viewer/
+-rw-r--r--   0 runner    (1001) docker     (123)   132535 2023-06-27 10:54:20.000000 scikit-rt-0.5.2/src/skrt/better_viewer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3958 2023-06-27 10:54:20.000000 scikit-rt-0.5.2/src/skrt/better_viewer/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)    76116 2023-06-27 10:54:20.000000 scikit-rt-0.5.2/src/skrt/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:58:28.332134 scikit-rt-0.5.2/src/skrt/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:58:28.348134 scikit-rt-0.5.2/src/skrt/data/elastix_parameter_files/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1732 2023-06-27 10:54:20.000000 scikit-rt-0.5.2/src/skrt/data/elastix_parameter_files/BE_BSpline05.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1801 2023-06-27 10:54:20.000000 scikit-rt-0.5.2/src/skrt/data/elastix_parameter_files/MI_Affine.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1649 2023-06-27 10:54:20.000000 scikit-rt-0.5.2/src/skrt/data/elastix_parameter_files/MI_BSpline05.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1650 2023-06-27 10:54:20.000000 scikit-rt-0.5.2/src/skrt/data/elastix_parameter_files/MI_BSpline15.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1650 2023-06-27 10:54:20.000000 scikit-rt-0.5.2/src/skrt/data/elastix_parameter_files/MI_BSpline30.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1798 2023-06-27 10:54:20.000000 scikit-rt-0.5.2/src/skrt/data/elastix_parameter_files/MI_Rigid.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1804 2023-06-27 10:54:20.000000 scikit-rt-0.5.2/src/skrt/data/elastix_parameter_files/MI_Translation.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:58:28.348134 scikit-rt-0.5.2/src/skrt/data/niftyreg_parameter_files/
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-06-27 10:54:20.000000 scikit-rt-0.5.2/src/skrt/data/niftyreg_parameter_files/Affine.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-27 10:54:20.000000 scikit-rt-0.5.2/src/skrt/data/niftyreg_parameter_files/BE_BSpline05.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-27 10:54:20.000000 scikit-rt-0.5.2/src/skrt/data/niftyreg_parameter_files/NMI_BSpline05.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-27 10:54:20.000000 scikit-rt-0.5.2/src/skrt/data/niftyreg_parameter_files/NMI_BSpline15.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-27 10:54:20.000000 scikit-rt-0.5.2/src/skrt/data/niftyreg_parameter_files/NMI_BSpline30.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-06-27 10:54:20.000000 scikit-rt-0.5.2/src/skrt/data/niftyreg_parameter_files/Rigid.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    27334 2023-06-27 10:54:20.000000 scikit-rt-0.5.2/src/skrt/dicom_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39944 2023-06-27 10:54:20.000000 scikit-rt-0.5.2/src/skrt/dose.py
+-rw-r--r--   0 runner    (1001) docker     (123)   257103 2023-06-27 10:54:20.000000 scikit-rt-0.5.2/src/skrt/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-06-27 10:54:20.000000 scikit-rt-0.5.2/src/skrt/multi.py
+-rw-r--r--   0 runner    (1001) docker     (123)   118936 2023-06-27 10:54:20.000000 scikit-rt-0.5.2/src/skrt/patient.py
+-rw-r--r--   0 runner    (1001) docker     (123)   152018 2023-06-27 10:54:20.000000 scikit-rt-0.5.2/src/skrt/registration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60958 2023-06-27 10:54:20.000000 scikit-rt-0.5.2/src/skrt/segmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25041 2023-06-27 10:54:20.000000 scikit-rt-0.5.2/src/skrt/simulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)   358501 2023-06-27 10:54:20.000000 scikit-rt-0.5.2/src/skrt/structures.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:58:28.352134 scikit-rt-0.5.2/src/skrt/viewer/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-27 10:54:20.000000 scikit-rt-0.5.2/src/skrt/viewer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   154795 2023-06-27 10:54:20.000000 scikit-rt-0.5.2/src/skrt/viewer/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)   113136 2023-06-27 10:54:20.000000 scikit-rt-0.5.2/src/skrt/viewer/viewer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:58:28.360134 scikit-rt-0.5.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-06-27 10:54:20.000000 scikit-rt-0.5.2/tests/test_01_setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10063 2023-06-27 10:54:20.000000 scikit-rt-0.5.2/tests/test_application.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15414 2023-06-27 10:54:20.000000 scikit-rt-0.5.2/tests/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7248 2023-06-27 10:54:20.000000 scikit-rt-0.5.2/tests/test_dose.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61981 2023-06-27 10:54:20.000000 scikit-rt-0.5.2/tests/test_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-06-27 10:54:20.000000 scikit-rt-0.5.2/tests/test_multi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9592 2023-06-27 10:54:20.000000 scikit-rt-0.5.2/tests/test_patient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-06-27 10:54:20.000000 scikit-rt-0.5.2/tests/test_qv_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8791 2023-06-27 10:54:20.000000 scikit-rt-0.5.2/tests/test_qv_quickviewer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6165 2023-06-27 10:54:20.000000 scikit-rt-0.5.2/tests/test_qv_struct_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3876 2023-06-27 10:54:20.000000 scikit-rt-0.5.2/tests/test_qv_struct_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-06-27 10:54:20.000000 scikit-rt-0.5.2/tests/test_qv_structs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34841 2023-06-27 10:54:20.000000 scikit-rt-0.5.2/tests/test_registration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21138 2023-06-27 10:54:20.000000 scikit-rt-0.5.2/tests/test_roi_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5429 2023-06-27 10:54:20.000000 scikit-rt-0.5.2/tests/test_segmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-27 10:54:20.000000 scikit-rt-0.5.2/tests/test_simulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65888 2023-06-27 10:54:20.000000 scikit-rt-0.5.2/tests/test_structs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2513 2023-06-27 10:54:20.000000 scikit-rt-0.5.2/tests/test_synthetic_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7725 2023-06-27 10:54:20.000000 scikit-rt-0.5.2/tests/test_viewer.py
```

### Comparing `scikit-rt-0.5.1/LICENSE` & `scikit-rt-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.5.1/PKG-INFO` & `scikit-rt-0.5.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scikit-rt
-Version: 0.5.1
+Version: 0.5.2
 Summary: Toolkit for analysis of radiotherapy data
 Home-page: https://github.com/scikit-rt/scikit-rt
 Author: H. Pullen, K. Harrison
 Author-email: scikit-rt@hep.phy.cam.ac.uk
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/scikit-rt/scikit-rt/issues
 Description: # Scikit-rt
```

### Comparing `scikit-rt-0.5.1/README.md` & `scikit-rt-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.5.1/pypi.md` & `scikit-rt-0.5.2/pypi.md`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.5.1/setup.cfg` & `scikit-rt-0.5.2/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = scikit-rt
-version = 0.5.1
+version = 0.5.2
 author = H. Pullen, K. Harrison
 author_email = scikit-rt@hep.phy.cam.ac.uk
 description = Toolkit for analysis of radiotherapy data
 long_description = file: pypi.md
 long_description_content_type = text/markdown
 url = https://github.com/scikit-rt/scikit-rt
 project_urls =
```

### Comparing `scikit-rt-0.5.1/src/scikit_rt.egg-info/PKG-INFO` & `scikit-rt-0.5.2/src/scikit_rt.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scikit-rt
-Version: 0.5.1
+Version: 0.5.2
 Summary: Toolkit for analysis of radiotherapy data
 Home-page: https://github.com/scikit-rt/scikit-rt
 Author: H. Pullen, K. Harrison
 Author-email: scikit-rt@hep.phy.cam.ac.uk
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/scikit-rt/scikit-rt/issues
 Description: # Scikit-rt
```

### Comparing `scikit-rt-0.5.1/src/scikit_rt.egg-info/SOURCES.txt` & `scikit-rt-0.5.2/src/scikit_rt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.5.1/src/scikit_rt.egg-info/requires.txt` & `scikit-rt-0.5.2/src/scikit_rt.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.5.1/src/skrt/__init__.py` & `scikit-rt-0.5.2/src/skrt/__init__.py`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.5.1/src/skrt/application.py` & `scikit-rt-0.5.2/src/skrt/application.py`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.5.1/src/skrt/better_viewer/__init__.py` & `scikit-rt-0.5.2/src/skrt/better_viewer/__init__.py`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.5.1/src/skrt/better_viewer/options.py` & `scikit-rt-0.5.2/src/skrt/better_viewer/options.py`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.5.1/src/skrt/core.py` & `scikit-rt-0.5.2/src/skrt/core.py`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.5.1/src/skrt/data/elastix_parameter_files/BE_BSpline05.txt` & `scikit-rt-0.5.2/src/skrt/data/elastix_parameter_files/BE_BSpline05.txt`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.5.1/src/skrt/data/elastix_parameter_files/MI_Affine.txt` & `scikit-rt-0.5.2/src/skrt/data/elastix_parameter_files/MI_Affine.txt`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.5.1/src/skrt/data/elastix_parameter_files/MI_BSpline05.txt` & `scikit-rt-0.5.2/src/skrt/data/elastix_parameter_files/MI_BSpline05.txt`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.5.1/src/skrt/data/elastix_parameter_files/MI_BSpline15.txt` & `scikit-rt-0.5.2/src/skrt/data/elastix_parameter_files/MI_BSpline15.txt`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.5.1/src/skrt/data/elastix_parameter_files/MI_BSpline30.txt` & `scikit-rt-0.5.2/src/skrt/data/elastix_parameter_files/MI_BSpline30.txt`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.5.1/src/skrt/data/elastix_parameter_files/MI_Rigid.txt` & `scikit-rt-0.5.2/src/skrt/data/elastix_parameter_files/MI_Rigid.txt`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.5.1/src/skrt/data/elastix_parameter_files/MI_Translation.txt` & `scikit-rt-0.5.2/src/skrt/data/elastix_parameter_files/MI_Translation.txt`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.5.1/src/skrt/dicom_writer.py` & `scikit-rt-0.5.2/src/skrt/dicom_writer.py`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.5.1/src/skrt/dose.py` & `scikit-rt-0.5.2/src/skrt/dose.py`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.5.1/src/skrt/image.py` & `scikit-rt-0.5.2/src/skrt/image.py`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.5.1/src/skrt/multi.py` & `scikit-rt-0.5.2/src/skrt/multi.py`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.5.1/src/skrt/patient.py` & `scikit-rt-0.5.2/src/skrt/patient.py`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.5.1/src/skrt/registration.py` & `scikit-rt-0.5.2/src/skrt/registration.py`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.5.1/src/skrt/segmentation.py` & `scikit-rt-0.5.2/src/skrt/segmentation.py`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.5.1/src/skrt/simulation.py` & `scikit-rt-0.5.2/src/skrt/simulation.py`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.5.1/src/skrt/structures.py` & `scikit-rt-0.5.2/src/skrt/structures.py`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.5.1/src/skrt/viewer/core.py` & `scikit-rt-0.5.2/src/skrt/viewer/core.py`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.5.1/src/skrt/viewer/viewer.py` & `scikit-rt-0.5.2/src/skrt/viewer/viewer.py`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.5.1/tests/test_01_setup.py` & `scikit-rt-0.5.2/tests/test_01_setup.py`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.5.1/tests/test_application.py` & `scikit-rt-0.5.2/tests/test_application.py`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.5.1/tests/test_core.py` & `scikit-rt-0.5.2/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.5.1/tests/test_dose.py` & `scikit-rt-0.5.2/tests/test_dose.py`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.5.1/tests/test_image.py` & `scikit-rt-0.5.2/tests/test_image.py`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.5.1/tests/test_multi.py` & `scikit-rt-0.5.2/tests/test_multi.py`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.5.1/tests/test_patient.py` & `scikit-rt-0.5.2/tests/test_patient.py`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.5.1/tests/test_qv_image.py` & `scikit-rt-0.5.2/tests/test_qv_image.py`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.5.1/tests/test_qv_quickviewer.py` & `scikit-rt-0.5.2/tests/test_qv_quickviewer.py`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.5.1/tests/test_qv_struct_loader.py` & `scikit-rt-0.5.2/tests/test_qv_struct_loader.py`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.5.1/tests/test_qv_struct_metrics.py` & `scikit-rt-0.5.2/tests/test_qv_struct_metrics.py`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.5.1/tests/test_qv_structs.py` & `scikit-rt-0.5.2/tests/test_qv_structs.py`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.5.1/tests/test_registration.py` & `scikit-rt-0.5.2/tests/test_registration.py`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.5.1/tests/test_roi_metrics.py` & `scikit-rt-0.5.2/tests/test_roi_metrics.py`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.5.1/tests/test_segmentation.py` & `scikit-rt-0.5.2/tests/test_segmentation.py`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.5.1/tests/test_structs.py` & `scikit-rt-0.5.2/tests/test_structs.py`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.5.1/tests/test_synthetic_image.py` & `scikit-rt-0.5.2/tests/test_synthetic_image.py`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.5.1/tests/test_viewer.py` & `scikit-rt-0.5.2/tests/test_viewer.py`

 * *Files identical despite different names*

