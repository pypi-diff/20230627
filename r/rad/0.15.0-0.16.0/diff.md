# Comparing `tmp/rad-0.15.0.tar.gz` & `tmp/rad-0.16.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rad-0.15.0.tar", last modified: Fri May 12 21:12:44 2023, max compression
+gzip compressed data, was "rad-0.16.0.tar", last modified: Tue Jun 27 14:59:48 2023, max compression
```

## Comparing `rad-0.15.0.tar` & `rad-0.16.0.tar`

### file list

```diff
@@ -1,127 +1,130 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:12:44.595994 rad-0.15.0/
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-12 21:12:33.000000 rad-0.15.0/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:12:44.583994 rad-0.15.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-05-12 21:12:33.000000 rad-0.15.0/.github/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-05-12 21:12:33.000000 rad-0.15.0/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:12:44.583994 rad-0.15.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-05-12 21:12:33.000000 rad-0.15.0/.github/workflows/changelog.yml
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-05-12 21:12:33.000000 rad-0.15.0/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-05-12 21:12:33.000000 rad-0.15.0/.github/workflows/ci_cron.yml
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-05-12 21:12:33.000000 rad-0.15.0/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-05-12 21:12:33.000000 rad-0.15.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-05-12 21:12:33.000000 rad-0.15.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-05-12 21:12:33.000000 rad-0.15.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-05-12 21:12:33.000000 rad-0.15.0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     9336 2023-05-12 21:12:33.000000 rad-0.15.0/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3206 2023-05-12 21:12:33.000000 rad-0.15.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-05-12 21:12:33.000000 rad-0.15.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-05-12 21:12:33.000000 rad-0.15.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 21:12:33.000000 rad-0.15.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3033 2023-05-12 21:12:44.595994 rad-0.15.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-05-12 21:12:33.000000 rad-0.15.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:12:44.583994 rad-0.15.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     4743 2023-05-12 21:12:33.000000 rad-0.15.0/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:12:44.583994 rad-0.15.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-05-12 21:12:33.000000 rad-0.15.0/docs/_static/custom.css
--rw-r--r--   0 runner    (1001) docker     (123)    59966 2023-05-12 21:12:33.000000 rad-0.15.0/docs/_static/stsci_logo.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:12:44.579994 rad-0.15.0/docs/_templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:12:44.583994 rad-0.15.0/docs/_templates/autosummary/
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-05-12 21:12:33.000000 rad-0.15.0/docs/_templates/autosummary/base.rst
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-05-12 21:12:33.000000 rad-0.15.0/docs/_templates/autosummary/class.rst
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-05-12 21:12:33.000000 rad-0.15.0/docs/_templates/autosummary/module.rst
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-12 21:12:33.000000 rad-0.15.0/docs/changes.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6688 2023-05-12 21:12:33.000000 rad-0.15.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-05-12 21:12:33.000000 rad-0.15.0/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-05-12 21:12:33.000000 rad-0.15.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4513 2023-05-12 21:12:33.000000 rad-0.15.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-05-12 21:12:33.000000 rad-0.15.0/docs/manifests.rst
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-05-12 21:12:33.000000 rad-0.15.0/docs/reference_files.rst
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-05-12 21:12:33.000000 rad-0.15.0/docs/schemas.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-05-12 21:12:33.000000 rad-0.15.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:12:44.583994 rad-0.15.0/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)      986 2023-05-12 21:12:33.000000 rad-0.15.0/scripts/insert_next_release.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      954 2023-05-12 21:12:33.000000 rad-0.15.0/scripts/set_release_date.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 21:12:44.595994 rad-0.15.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:12:44.579994 rad-0.15.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:12:44.587994 rad-0.15.0/src/rad/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-12 21:12:33.000000 rad-0.15.0/src/rad/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-12 21:12:44.000000 rad-0.15.0/src/rad/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      796 2023-05-12 21:12:33.000000 rad-0.15.0/src/rad/integration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:12:44.587994 rad-0.15.0/src/rad/resources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 21:12:33.000000 rad-0.15.0/src/rad/resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:12:44.587994 rad-0.15.0/src/rad/resources/manifests/
--rw-r--r--   0 runner    (1001) docker     (123)    11520 2023-05-12 21:12:33.000000 rad-0.15.0/src/rad/resources/manifests/datamodels-1.0.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:12:44.591994 rad-0.15.0/src/rad/resources/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-05-12 21:12:33.000000 rad-0.15.0/src/rad/resources/schemas/aperture-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-05-12 21:12:33.000000 rad-0.15.0/src/rad/resources/schemas/associations-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-12 21:12:33.000000 rad-0.15.0/src/rad/resources/schemas/basic-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-12 21:12:33.000000 rad-0.15.0/src/rad/resources/schemas/cal_logs-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2809 2023-05-12 21:12:33.000000 rad-0.15.0/src/rad/resources/schemas/cal_step-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-05-12 21:12:33.000000 rad-0.15.0/src/rad/resources/schemas/common-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-05-12 21:12:33.000000 rad-0.15.0/src/rad/resources/schemas/coordinates-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4183 2023-05-12 21:12:33.000000 rad-0.15.0/src/rad/resources/schemas/ephemeris-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13874 2023-05-12 21:12:33.000000 rad-0.15.0/src/rad/resources/schemas/exposure-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-05-12 21:12:33.000000 rad-0.15.0/src/rad/resources/schemas/exposure_type-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     9046 2023-05-12 21:12:33.000000 rad-0.15.0/src/rad/resources/schemas/guidestar-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     9255 2023-05-12 21:12:33.000000 rad-0.15.0/src/rad/resources/schemas/guidewindow-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-05-12 21:12:33.000000 rad-0.15.0/src/rad/resources/schemas/guidewindow_modes-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6364 2023-05-12 21:12:33.000000 rad-0.15.0/src/rad/resources/schemas/observation-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-05-12 21:12:33.000000 rad-0.15.0/src/rad/resources/schemas/photometry-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-05-12 21:12:33.000000 rad-0.15.0/src/rad/resources/schemas/pointing-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-05-12 21:12:33.000000 rad-0.15.0/src/rad/resources/schemas/program-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3311 2023-05-12 21:12:33.000000 rad-0.15.0/src/rad/resources/schemas/rad_schema-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4432 2023-05-12 21:12:33.000000 rad-0.15.0/src/rad/resources/schemas/ramp-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3432 2023-05-12 21:12:33.000000 rad-0.15.0/src/rad/resources/schemas/ramp_fit_output-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-05-12 21:12:33.000000 rad-0.15.0/src/rad/resources/schemas/ref_file-1.0.0.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:12:44.595994 rad-0.15.0/src/rad/resources/schemas/reference_files/
--rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-05-12 21:12:33.000000 rad-0.15.0/src/rad/resources/schemas/reference_files/dark-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-12 21:12:33.000000 rad-0.15.0/src/rad/resources/schemas/reference_files/distortion-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-05-12 21:12:33.000000 rad-0.15.0/src/rad/resources/schemas/reference_files/flat-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-05-12 21:12:33.000000 rad-0.15.0/src/rad/resources/schemas/reference_files/gain-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-05-12 21:12:33.000000 rad-0.15.0/src/rad/resources/schemas/reference_files/inverse_linearity-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-05-12 21:12:33.000000 rad-0.15.0/src/rad/resources/schemas/reference_files/ipc-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-05-12 21:12:33.000000 rad-0.15.0/src/rad/resources/schemas/reference_files/linearity-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-05-12 21:12:33.000000 rad-0.15.0/src/rad/resources/schemas/reference_files/mask-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-05-12 21:12:33.000000 rad-0.15.0/src/rad/resources/schemas/reference_files/pixelarea-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-05-12 21:12:33.000000 rad-0.15.0/src/rad/resources/schemas/reference_files/readnoise-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-05-12 21:12:33.000000 rad-0.15.0/src/rad/resources/schemas/reference_files/ref_common-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-05-12 21:12:33.000000 rad-0.15.0/src/rad/resources/schemas/reference_files/ref_exposure_type-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-05-12 21:12:33.000000 rad-0.15.0/src/rad/resources/schemas/reference_files/ref_optical_element-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-05-12 21:12:33.000000 rad-0.15.0/src/rad/resources/schemas/reference_files/saturation-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-05-12 21:12:33.000000 rad-0.15.0/src/rad/resources/schemas/reference_files/superbias-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-05-12 21:12:33.000000 rad-0.15.0/src/rad/resources/schemas/reference_files/wfi_img_photom-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-05-12 21:12:33.000000 rad-0.15.0/src/rad/resources/schemas/resample-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-12 21:12:33.000000 rad-0.15.0/src/rad/resources/schemas/source_detection-1.0.0.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:12:44.595994 rad-0.15.0/src/rad/resources/schemas/tagged_scalars/
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-05-12 21:12:33.000000 rad-0.15.0/src/rad/resources/schemas/tagged_scalars/calibration_software_version-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-05-12 21:12:33.000000 rad-0.15.0/src/rad/resources/schemas/tagged_scalars/file_date-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-12 21:12:33.000000 rad-0.15.0/src/rad/resources/schemas/tagged_scalars/filename-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-05-12 21:12:33.000000 rad-0.15.0/src/rad/resources/schemas/tagged_scalars/model_type-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-05-12 21:12:33.000000 rad-0.15.0/src/rad/resources/schemas/tagged_scalars/origin-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-05-12 21:12:33.000000 rad-0.15.0/src/rad/resources/schemas/tagged_scalars/prd_software_version-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-05-12 21:12:33.000000 rad-0.15.0/src/rad/resources/schemas/tagged_scalars/sdf_software_version-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-05-12 21:12:33.000000 rad-0.15.0/src/rad/resources/schemas/tagged_scalars/telescope-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4683 2023-05-12 21:12:33.000000 rad-0.15.0/src/rad/resources/schemas/target-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-05-12 21:12:33.000000 rad-0.15.0/src/rad/resources/schemas/variance-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-05-12 21:12:33.000000 rad-0.15.0/src/rad/resources/schemas/velocity_aberration-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3309 2023-05-12 21:12:33.000000 rad-0.15.0/src/rad/resources/schemas/visit-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2615 2023-05-12 21:12:33.000000 rad-0.15.0/src/rad/resources/schemas/wcsinfo-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-05-12 21:12:33.000000 rad-0.15.0/src/rad/resources/schemas/wfi_detector-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     5203 2023-05-12 21:12:33.000000 rad-0.15.0/src/rad/resources/schemas/wfi_image-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-05-12 21:12:33.000000 rad-0.15.0/src/rad/resources/schemas/wfi_mode-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2563 2023-05-12 21:12:33.000000 rad-0.15.0/src/rad/resources/schemas/wfi_mosaic-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-05-12 21:12:33.000000 rad-0.15.0/src/rad/resources/schemas/wfi_optical_element-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-05-12 21:12:33.000000 rad-0.15.0/src/rad/resources/schemas/wfi_science_raw-1.0.0.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:12:44.587994 rad-0.15.0/src/rad.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3033 2023-05-12 21:12:44.000000 rad-0.15.0/src/rad.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4348 2023-05-12 21:12:44.000000 rad-0.15.0/src/rad.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 21:12:44.000000 rad-0.15.0/src/rad.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-12 21:12:44.000000 rad-0.15.0/src/rad.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-12 21:12:44.000000 rad-0.15.0/src/rad.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-12 21:12:44.000000 rad-0.15.0/src/rad.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:12:44.595994 rad-0.15.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-05-12 21:12:33.000000 rad-0.15.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-05-12 21:12:33.000000 rad-0.15.0/tests/test_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-05-12 21:12:33.000000 rad-0.15.0/tests/test_manifest.py
--rw-r--r--   0 runner    (1001) docker     (123)     5530 2023-05-12 21:12:33.000000 rad-0.15.0/tests/test_schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-05-12 21:12:33.000000 rad-0.15.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 14:59:48.357072 rad-0.16.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-27 14:59:35.000000 rad-0.16.0/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 14:59:48.341072 rad-0.16.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-06-27 14:59:35.000000 rad-0.16.0/.github/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-06-27 14:59:35.000000 rad-0.16.0/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 14:59:48.341072 rad-0.16.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-06-27 14:59:35.000000 rad-0.16.0/.github/workflows/changelog.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-06-27 14:59:35.000000 rad-0.16.0/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-27 14:59:35.000000 rad-0.16.0/.github/workflows/ci_cron.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-06-27 14:59:35.000000 rad-0.16.0/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-06-27 14:59:35.000000 rad-0.16.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-06-27 14:59:35.000000 rad-0.16.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-06-27 14:59:35.000000 rad-0.16.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-06-27 14:59:35.000000 rad-0.16.0/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     9799 2023-06-27 14:59:35.000000 rad-0.16.0/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3206 2023-06-27 14:59:35.000000 rad-0.16.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-27 14:59:35.000000 rad-0.16.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-06-27 14:59:35.000000 rad-0.16.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 14:59:35.000000 rad-0.16.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3033 2023-06-27 14:59:48.357072 rad-0.16.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-06-27 14:59:35.000000 rad-0.16.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 14:59:48.345072 rad-0.16.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     4743 2023-06-27 14:59:35.000000 rad-0.16.0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 14:59:48.345072 rad-0.16.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-06-27 14:59:35.000000 rad-0.16.0/docs/_static/custom.css
+-rw-r--r--   0 runner    (1001) docker     (123)    59966 2023-06-27 14:59:35.000000 rad-0.16.0/docs/_static/stsci_logo.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 14:59:48.337072 rad-0.16.0/docs/_templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 14:59:48.345072 rad-0.16.0/docs/_templates/autosummary/
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-06-27 14:59:35.000000 rad-0.16.0/docs/_templates/autosummary/base.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-06-27 14:59:35.000000 rad-0.16.0/docs/_templates/autosummary/class.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-06-27 14:59:35.000000 rad-0.16.0/docs/_templates/autosummary/module.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-27 14:59:35.000000 rad-0.16.0/docs/changes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6688 2023-06-27 14:59:35.000000 rad-0.16.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-06-27 14:59:35.000000 rad-0.16.0/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-06-27 14:59:35.000000 rad-0.16.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4513 2023-06-27 14:59:35.000000 rad-0.16.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-27 14:59:35.000000 rad-0.16.0/docs/manifests.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-06-27 14:59:35.000000 rad-0.16.0/docs/reference_files.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-06-27 14:59:35.000000 rad-0.16.0/docs/schemas.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-06-27 14:59:35.000000 rad-0.16.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 14:59:48.345072 rad-0.16.0/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      986 2023-06-27 14:59:35.000000 rad-0.16.0/scripts/insert_next_release.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      954 2023-06-27 14:59:35.000000 rad-0.16.0/scripts/set_release_date.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 14:59:48.361072 rad-0.16.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 14:59:48.341072 rad-0.16.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 14:59:48.345072 rad-0.16.0/src/rad/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-27 14:59:35.000000 rad-0.16.0/src/rad/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-27 14:59:48.000000 rad-0.16.0/src/rad/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-06-27 14:59:35.000000 rad-0.16.0/src/rad/integration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 14:59:48.349072 rad-0.16.0/src/rad/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 14:59:35.000000 rad-0.16.0/src/rad/resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 14:59:48.349072 rad-0.16.0/src/rad/resources/manifests/
+-rw-r--r--   0 runner    (1001) docker     (123)    12063 2023-06-27 14:59:35.000000 rad-0.16.0/src/rad/resources/manifests/datamodels-1.0.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 14:59:48.353072 rad-0.16.0/src/rad/resources/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-06-27 14:59:35.000000 rad-0.16.0/src/rad/resources/schemas/aperture-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-06-27 14:59:35.000000 rad-0.16.0/src/rad/resources/schemas/associations-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-27 14:59:35.000000 rad-0.16.0/src/rad/resources/schemas/basic-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-06-27 14:59:35.000000 rad-0.16.0/src/rad/resources/schemas/cal_logs-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2809 2023-06-27 14:59:35.000000 rad-0.16.0/src/rad/resources/schemas/cal_step-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-06-27 14:59:35.000000 rad-0.16.0/src/rad/resources/schemas/common-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-06-27 14:59:35.000000 rad-0.16.0/src/rad/resources/schemas/coordinates-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4183 2023-06-27 14:59:35.000000 rad-0.16.0/src/rad/resources/schemas/ephemeris-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13875 2023-06-27 14:59:35.000000 rad-0.16.0/src/rad/resources/schemas/exposure-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-06-27 14:59:35.000000 rad-0.16.0/src/rad/resources/schemas/exposure_type-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     9046 2023-06-27 14:59:35.000000 rad-0.16.0/src/rad/resources/schemas/guidestar-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     9288 2023-06-27 14:59:35.000000 rad-0.16.0/src/rad/resources/schemas/guidewindow-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-06-27 14:59:35.000000 rad-0.16.0/src/rad/resources/schemas/guidewindow_modes-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-06-27 14:59:35.000000 rad-0.16.0/src/rad/resources/schemas/msos_stack-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6364 2023-06-27 14:59:35.000000 rad-0.16.0/src/rad/resources/schemas/observation-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-06-27 14:59:35.000000 rad-0.16.0/src/rad/resources/schemas/photometry-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-27 14:59:35.000000 rad-0.16.0/src/rad/resources/schemas/pointing-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-06-27 14:59:35.000000 rad-0.16.0/src/rad/resources/schemas/program-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3443 2023-06-27 14:59:35.000000 rad-0.16.0/src/rad/resources/schemas/rad_schema-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4195 2023-06-27 14:59:35.000000 rad-0.16.0/src/rad/resources/schemas/ramp-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-06-27 14:59:35.000000 rad-0.16.0/src/rad/resources/schemas/ramp_fit_output-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-06-27 14:59:35.000000 rad-0.16.0/src/rad/resources/schemas/ref_file-1.0.0.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 14:59:48.357072 rad-0.16.0/src/rad/resources/schemas/reference_files/
+-rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-06-27 14:59:35.000000 rad-0.16.0/src/rad/resources/schemas/reference_files/dark-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-06-27 14:59:35.000000 rad-0.16.0/src/rad/resources/schemas/reference_files/distortion-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-06-27 14:59:35.000000 rad-0.16.0/src/rad/resources/schemas/reference_files/flat-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-06-27 14:59:35.000000 rad-0.16.0/src/rad/resources/schemas/reference_files/gain-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-06-27 14:59:35.000000 rad-0.16.0/src/rad/resources/schemas/reference_files/inverse_linearity-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-06-27 14:59:35.000000 rad-0.16.0/src/rad/resources/schemas/reference_files/ipc-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-06-27 14:59:35.000000 rad-0.16.0/src/rad/resources/schemas/reference_files/linearity-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-06-27 14:59:35.000000 rad-0.16.0/src/rad/resources/schemas/reference_files/mask-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-06-27 14:59:35.000000 rad-0.16.0/src/rad/resources/schemas/reference_files/pixelarea-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-06-27 14:59:35.000000 rad-0.16.0/src/rad/resources/schemas/reference_files/readnoise-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-06-27 14:59:35.000000 rad-0.16.0/src/rad/resources/schemas/reference_files/ref_common-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-06-27 14:59:35.000000 rad-0.16.0/src/rad/resources/schemas/reference_files/ref_exposure_type-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-06-27 14:59:35.000000 rad-0.16.0/src/rad/resources/schemas/reference_files/ref_optical_element-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-06-27 14:59:35.000000 rad-0.16.0/src/rad/resources/schemas/reference_files/refpix-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      937 2023-06-27 14:59:35.000000 rad-0.16.0/src/rad/resources/schemas/reference_files/saturation-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-06-27 14:59:35.000000 rad-0.16.0/src/rad/resources/schemas/reference_files/superbias-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-06-27 14:59:35.000000 rad-0.16.0/src/rad/resources/schemas/reference_files/wfi_img_photom-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-06-27 14:59:35.000000 rad-0.16.0/src/rad/resources/schemas/resample-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-06-27 14:59:35.000000 rad-0.16.0/src/rad/resources/schemas/source_detection-1.0.0.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 14:59:48.357072 rad-0.16.0/src/rad/resources/schemas/tagged_scalars/
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-06-27 14:59:35.000000 rad-0.16.0/src/rad/resources/schemas/tagged_scalars/calibration_software_version-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-06-27 14:59:35.000000 rad-0.16.0/src/rad/resources/schemas/tagged_scalars/file_date-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-06-27 14:59:35.000000 rad-0.16.0/src/rad/resources/schemas/tagged_scalars/filename-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-06-27 14:59:35.000000 rad-0.16.0/src/rad/resources/schemas/tagged_scalars/model_type-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-06-27 14:59:35.000000 rad-0.16.0/src/rad/resources/schemas/tagged_scalars/origin-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-06-27 14:59:35.000000 rad-0.16.0/src/rad/resources/schemas/tagged_scalars/prd_software_version-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-06-27 14:59:35.000000 rad-0.16.0/src/rad/resources/schemas/tagged_scalars/sdf_software_version-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-06-27 14:59:35.000000 rad-0.16.0/src/rad/resources/schemas/tagged_scalars/telescope-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4683 2023-06-27 14:59:35.000000 rad-0.16.0/src/rad/resources/schemas/target-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-06-27 14:59:35.000000 rad-0.16.0/src/rad/resources/schemas/variance-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-06-27 14:59:35.000000 rad-0.16.0/src/rad/resources/schemas/velocity_aberration-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3309 2023-06-27 14:59:35.000000 rad-0.16.0/src/rad/resources/schemas/visit-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2615 2023-06-27 14:59:35.000000 rad-0.16.0/src/rad/resources/schemas/wcsinfo-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-06-27 14:59:35.000000 rad-0.16.0/src/rad/resources/schemas/wfi_detector-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5231 2023-06-27 14:59:35.000000 rad-0.16.0/src/rad/resources/schemas/wfi_image-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-06-27 14:59:35.000000 rad-0.16.0/src/rad/resources/schemas/wfi_mode-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-06-27 14:59:35.000000 rad-0.16.0/src/rad/resources/schemas/wfi_mosaic-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-06-27 14:59:35.000000 rad-0.16.0/src/rad/resources/schemas/wfi_optical_element-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-06-27 14:59:35.000000 rad-0.16.0/src/rad/resources/schemas/wfi_science_raw-1.0.0.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 14:59:48.345072 rad-0.16.0/src/rad.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3033 2023-06-27 14:59:48.000000 rad-0.16.0/src/rad.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4474 2023-06-27 14:59:48.000000 rad-0.16.0/src/rad.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 14:59:48.000000 rad-0.16.0/src/rad.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-27 14:59:48.000000 rad-0.16.0/src/rad.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-06-27 14:59:48.000000 rad-0.16.0/src/rad.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-27 14:59:48.000000 rad-0.16.0/src/rad.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 14:59:48.357072 rad-0.16.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 14:59:35.000000 rad-0.16.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-27 14:59:35.000000 rad-0.16.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-06-27 14:59:35.000000 rad-0.16.0/tests/test_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-06-27 14:59:35.000000 rad-0.16.0/tests/test_manifest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6358 2023-06-27 14:59:35.000000 rad-0.16.0/tests/test_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-06-27 14:59:35.000000 rad-0.16.0/tox.ini
```

### Comparing `rad-0.15.0/.github/pull_request_template.md` & `rad-0.16.0/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `rad-0.15.0/.github/workflows/changelog.yml` & `rad-0.16.0/.github/workflows/changelog.yml`

 * *Files identical despite different names*

### Comparing `rad-0.15.0/.github/workflows/ci.yml` & `rad-0.16.0/.github/workflows/ci.yml`

 * *Files 15% similar despite different names*

```diff
@@ -13,15 +13,14 @@
     - cron: '0 9 * * 1'
 
 jobs:
   check:
     uses: OpenAstronomy/github-actions-workflows/.github/workflows/tox.yml@v1
     with:
       envs: |
-        - linux: check-style
         - linux: build-dist
   test:
     uses: OpenAstronomy/github-actions-workflows/.github/workflows/tox.yml@v1
     with:
       envs: |
         - linux: test-xdist
           python-version: 3.8
```

### Comparing `rad-0.15.0/.github/workflows/publish-to-pypi.yml` & `rad-0.16.0/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `rad-0.15.0/.github/workflows/release.yml` & `rad-0.16.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `rad-0.15.0/.gitignore` & `rad-0.16.0/.gitignore`

 * *Files identical despite different names*

### Comparing `rad-0.15.0/.pre-commit-config.yaml` & `rad-0.16.0/.pre-commit-config.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -22,29 +22,29 @@
     - id: python-check-blanket-noqa
     - id: python-check-mock-methods
     - id: rst-directive-colons
     - id: rst-inline-touching-normal
     - id: text-unicode-replacement-char
 
 - repo: https://github.com/codespell-project/codespell
-  rev: v2.2.4
+  rev: v2.2.5
   hooks:
     - id: codespell
       args: ["--write-changes"]
       additional_dependencies:
         - tomli
 
 - repo: https://github.com/asottile/pyupgrade
-  rev: 'v3.4.0'
+  rev: 'v3.7.0'
   hooks:
     - id: pyupgrade
       args: ["--py38-plus"]
 
 - repo: https://github.com/charliermarsh/ruff-pre-commit
-  rev: 'v0.0.265'
+  rev: 'v0.0.272'
   hooks:
     - id: ruff
       args: ["--fix"]
 
 - repo: https://github.com/pycqa/isort
   rev: 5.12.0
   hooks:
```

### Comparing `rad-0.15.0/CHANGES.rst` & `rad-0.16.0/CHANGES.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+0.16.0 (2023-06-26)
+-------------------
+
+- Fix minor discrepancies found when looking over the schemas. [#267]
+
+- Bugfix for ``inverse_linearity-1.0.0``'s ``reftype`` so that it is CRDS
+  compatible. [#272]
+
+- Add schema ``refpix-1.0.0`` as a schema for the reference pixel correction's
+  reference file. [#270]
+
+- Add keyword to indicate if and which datamodel the schema describes. [#278]
+
+- Add schema ``msos_stack-1.0.0`` as a level 3 schema for SSC. [#276]
+
 0.15.0 (2023-05-12)
 -------------------
 
 - Update program to be a string to match association code [#255]
 
 - Add gw_science_file_source to GW file, update size of the filename [#258]
```

### Comparing `rad-0.15.0/CODE_OF_CONDUCT.md` & `rad-0.16.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `rad-0.15.0/LICENSE` & `rad-0.16.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rad-0.15.0/PKG-INFO` & `rad-0.16.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rad
-Version: 0.15.0
+Version: 0.16.0
 Summary: Roman Attribute Dictionary
 Author-email: STScI <help@stsci.edu>
 License: Copyright (C) 2021 Association of Universities for Research in Astronomy (AURA)
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
```

### Comparing `rad-0.15.0/README.md` & `rad-0.16.0/README.md`

 * *Files identical despite different names*

### Comparing `rad-0.15.0/docs/Makefile` & `rad-0.16.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `rad-0.15.0/docs/_static/custom.css` & `rad-0.16.0/docs/_static/custom.css`

 * *Files identical despite different names*

### Comparing `rad-0.15.0/docs/_static/stsci_logo.png` & `rad-0.16.0/docs/_static/stsci_logo.png`

 * *Files identical despite different names*

### Comparing `rad-0.15.0/docs/conf.py` & `rad-0.16.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `rad-0.15.0/docs/index.rst` & `rad-0.16.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `rad-0.15.0/docs/make.bat` & `rad-0.16.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `rad-0.15.0/docs/schemas.rst` & `rad-0.16.0/docs/schemas.rst`

 * *Files identical despite different names*

### Comparing `rad-0.15.0/pyproject.toml` & `rad-0.16.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 ]
 dynamic = ['version']
 
 [project.optional-dependencies]
 test = [
     'pytest>=4.6.0',
     'pytest-doctestplus>=0.11.1',
+    'crds>=11.16.16',
 ]
 docs = [
     'sphinx',
     'sphinx-asdf>=0.1.3',
     'sphinx-astropy',
     'astropy>=5.0.4',
     'graphviz',
```

### Comparing `rad-0.15.0/scripts/insert_next_release.py` & `rad-0.16.0/scripts/insert_next_release.py`

 * *Files identical despite different names*

### Comparing `rad-0.15.0/scripts/set_release_date.py` & `rad-0.16.0/scripts/set_release_date.py`

 * *Files identical despite different names*

### Comparing `rad-0.15.0/src/rad/integration.py` & `rad-0.16.0/src/rad/integration.py`

 * *Files identical despite different names*

### Comparing `rad-0.15.0/src/rad/resources/manifests/datamodels-1.0.yaml` & `rad-0.16.0/src/rad/resources/manifests/datamodels-1.0.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -172,14 +172,19 @@
   description: |-
     Pixel area reference schema
 - tag_uri: asdf://stsci.edu/datamodels/roman/tags/reference_files/readnoise-1.0.0
   schema_uri: asdf://stsci.edu/datamodels/roman/schemas/reference_files/readnoise-1.0.0
   title: Read noise reference schema
   description: |-
     Read noise reference schema
+- tag_uri: asdf://stsci.edu/datamodels/roman/tags/reference_files/refpix-1.0.0
+  schema_uri: asdf://stsci.edu/datamodels/roman/schemas/reference_files/refpix-1.0.0
+  title: Reference pixel correction reference schema
+  description: |-
+    Reference pixel correction reference schema
 - tag_uri: asdf://stsci.edu/datamodels/roman/tags/reference_files/saturation-1.0.0
   schema_uri: asdf://stsci.edu/datamodels/roman/schemas/reference_files/saturation-1.0.0
   title: Saturation reference schema
   description: |-
     Saturation reference schema
 - tag_uri: asdf://stsci.edu/datamodels/roman/tags/reference_files/superbias-1.0.0
   schema_uri: asdf://stsci.edu/datamodels/roman/schemas/reference_files/superbias-1.0.0
@@ -244,8 +249,14 @@
   description: |-
     SDF software version number
 - tag_uri: asdf://stsci.edu/datamodels/roman/tags/telescope-1.0.0
   schema_uri: asdf://stsci.edu/datamodels/roman/schemas/tagged_scalars/telescope-1.0.0
   title: Telescope used to acquire the data
   description: |-
     Telescope used to acquire the data
+# SSC data models
+- tag_uri: asdf://stsci.edu/datamodels/roman/tags/msos_stack-1.0.0
+  schema_uri: asdf://stsci.edu/datamodels/roman/schemas/msos_stack-1.0.0
+  title: MSOS Stack Level 3 Schema
+  description: |-
+    Level 3 schema for SSC's MSOS stack products
 ...
```

### Comparing `rad-0.15.0/src/rad/resources/schemas/aperture-1.0.0.yaml` & `rad-0.16.0/src/rad/resources/schemas/aperture-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.15.0/src/rad/resources/schemas/basic-1.0.0.yaml` & `rad-0.16.0/src/rad/resources/schemas/basic-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.15.0/src/rad/resources/schemas/cal_step-1.0.0.yaml` & `rad-0.16.0/src/rad/resources/schemas/cal_step-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.15.0/src/rad/resources/schemas/common-1.0.0.yaml` & `rad-0.16.0/src/rad/resources/schemas/common-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.15.0/src/rad/resources/schemas/coordinates-1.0.0.yaml` & `rad-0.16.0/src/rad/resources/schemas/coordinates-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.15.0/src/rad/resources/schemas/ephemeris-1.0.0.yaml` & `rad-0.16.0/src/rad/resources/schemas/ephemeris-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.15.0/src/rad/resources/schemas/exposure-1.0.0.yaml` & `rad-0.16.0/src/rad/resources/schemas/exposure-1.0.0.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -343,15 +343,15 @@
       destination: [ScienceCommon.ma_table_name, GuideWindow.ma_table_name]
   ma_table_number:
     title: Numerical identifier for the multi-accumulation table used
     description: |
         The number of the MA table used for the exposure as defined by the
         PRD (Project Reference Database). This is used for matching the exposure
         to the appropriate calibration data.
-    type: number
+    type: integer
     sdf:
       special_processing: VALUE_REQUIRED
       source:
         origin: TBD
     archive_catalog:
       datatype: smallint
       destination: [ScienceCommon.ma_table_number, GuideWindow.ma_table_number]
```

### Comparing `rad-0.15.0/src/rad/resources/schemas/guidestar-1.0.0.yaml` & `rad-0.16.0/src/rad/resources/schemas/guidestar-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.15.0/src/rad/resources/schemas/guidewindow-1.0.0.yaml` & `rad-0.16.0/src/rad/resources/schemas/guidewindow-1.0.0.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 %YAML 1.1
 ---
 $schema: asdf://stsci.edu/datamodels/roman/schemas/rad_schema-1.0.0
 id: asdf://stsci.edu/datamodels/roman/schemas/guidewindow-1.0.0
 
 title: Guide window information
+
+datamodel_name: GuidewindowModel
+
 type: object
 properties:
   meta:
     allOf:
       - $ref: common-1.0.0
       - type: object
         properties:
@@ -118,15 +121,15 @@
             type: string
             sdf:
               special_processing: VALUE_REQUIRED
               source:
                 origin: Science Data Formatting
             archive_catalog:
               datatype: nvarchar(120)
-              destination: [ScienceCommon.gw_science_file_source]
+              destination: [GuideWindow.gw_science_file_source]
           gw_mode:
             $ref: guidewindow_modes-1.0.0
             sdf:
               special_processing: VALUE_REQUIRED
               source:
                 origin: Science Data Formatting
             archive_catalog:
```

### Comparing `rad-0.15.0/src/rad/resources/schemas/observation-1.0.0.yaml` & `rad-0.16.0/src/rad/resources/schemas/observation-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.15.0/src/rad/resources/schemas/photometry-1.0.0.yaml` & `rad-0.16.0/src/rad/resources/schemas/photometry-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.15.0/src/rad/resources/schemas/pointing-1.0.0.yaml` & `rad-0.16.0/src/rad/resources/schemas/pointing-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.15.0/src/rad/resources/schemas/program-1.0.0.yaml` & `rad-0.16.0/src/rad/resources/schemas/program-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.15.0/src/rad/resources/schemas/rad_schema-1.0.0.yaml` & `rad-0.16.0/src/rad/resources/schemas/rad_schema-1.0.0.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,19 @@
   A metaschema extending the ASDF metaschema to add support for
   sdf and archive_catalog properties.
 
 allOf:
   - $ref: http://stsci.edu/schemas/asdf/asdf-schema-1.0.0
   - type: object
     properties:
+      datamodel_name:
+        description: |-
+          The name of the datamodel that this schema describes.
+        type: string
+
       sdf:
         description: |-
           Documents source of this attribute's value when level 1
           files are created.
         type: object
         properties:
           special_processing:
```

### Comparing `rad-0.15.0/src/rad/resources/schemas/ramp-1.0.0.yaml` & `rad-0.16.0/src/rad/resources/schemas/ramp-1.0.0.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -1,130 +1,130 @@
 %YAML 1.1
 ---
 $schema: asdf://stsci.edu/datamodels/roman/schemas/rad_schema-1.0.0
 id: asdf://stsci.edu/datamodels/roman/schemas/ramp-1.0.0
 
 title: Ramp schema
 
-allOf:
-- type: object
-  properties:
-    meta:
-      allOf:
-        - $ref: common-1.0.0
-    data:
-      title: Science data, including the border reference pixels.
-      tag: tag:stsci.edu:asdf/unit/quantity-1.1.0
-      properties:
-        value:
-          tag: tag:stsci.edu:asdf/core/ndarray-1.0.0
-          datatype: float32
-          ndim: 3
-        unit:
-          tag: tag:astropy.org:astropy/units/unit-1.0.0
-          enum: ["DN", "electron"]
-    pixeldq:
-      title: 2-D data quality array for all planes
-      tag: tag:stsci.edu:asdf/core/ndarray-1.0.0
-      ndim: 2
-      datatype: uint32
-    groupdq:
-      title: 3-D data quality array (plane dq for each group)
+datamodel_name: RampModel
+
+type: object
+properties:
+  meta:
+    $ref: common-1.0.0
+  data:
+    title: Science data, including the border reference pixels.
+    tag: tag:stsci.edu:asdf/unit/quantity-1.1.0
+    properties:
+      value:
+        tag: tag:stsci.edu:asdf/core/ndarray-1.0.0
+        datatype: float32
+        ndim: 3
+      unit:
+        tag: tag:astropy.org:astropy/units/unit-1.0.0
+        enum: ["DN", "electron"]
+  pixeldq:
+    title: 2-D data quality array for all planes
+    tag: tag:stsci.edu:asdf/core/ndarray-1.0.0
+    ndim: 2
+    datatype: uint32
+  groupdq:
+    title: 3-D data quality array (plane dq for each group)
+    tag: tag:stsci.edu:asdf/core/ndarray-1.0.0
+    ndim: 3
+    datatype: uint8
+  err:
+    title: Error array containing the square root of the exposure-level combined variance
+    tag: tag:stsci.edu:asdf/unit/quantity-1.1.0
+    properties:
+      value:
+        tag: tag:stsci.edu:asdf/core/ndarray-1.0.0
+        datatype: float32
+        ndim: 3
+      unit:
+        tag: tag:astropy.org:astropy/units/unit-1.0.0
+        enum: ["DN", "electron"]
+  amp33:
+    title: Amp 33 reference pixel data
+    tag: tag:stsci.edu:asdf/unit/quantity-1.1.0
+    properties:
+      value:
+        tag: tag:stsci.edu:asdf/core/ndarray-1.0.0
+        datatype: uint16
+        ndim: 3
+      unit:
+        tag: tag:astropy.org:astropy/units/unit-1.0.0
+        enum: ["DN"]
+  border_ref_pix_left:
+    title: Original border reference pixels, on left (from viewers perspective).
+    tag: tag:stsci.edu:asdf/unit/quantity-1.1.0
+    value:
       tag: tag:stsci.edu:asdf/core/ndarray-1.0.0
+      datatype: float32
       ndim: 3
-      datatype: uint8
-    err:
-      title: Error array containing the square root of the exposure-level combined variance
-      tag: tag:stsci.edu:asdf/unit/quantity-1.1.0
-      properties:
-        value:
-          tag: tag:stsci.edu:asdf/core/ndarray-1.0.0
-          datatype: float32
-          ndim: 3
-        unit:
-          tag: tag:astropy.org:astropy/units/unit-1.0.0
-          enum: ["DN", "electron"]
-    amp33:
-      title: Amp 33 reference pixel data
-      tag: tag:stsci.edu:asdf/unit/quantity-1.1.0
-      properties:
-        value:
-          tag: tag:stsci.edu:asdf/core/ndarray-1.0.0
-          datatype: uint16
-          ndim: 3
-        unit:
-          tag: tag:astropy.org:astropy/units/unit-1.0.0
-          enum: ["DN"]
-    border_ref_pix_left:
-      title: Original border reference pixels, on left (from viewers perspective).
-      tag: tag:stsci.edu:asdf/unit/quantity-1.1.0
+    unit:
+      tag: tag:astropy.org:astropy/units/unit-1.0.0
+      enum: ["DN"]
+  border_ref_pix_right:
+    title: Original border reference pixels, on right (from viewers perspective).
+    tag: tag:stsci.edu:asdf/unit/quantity-1.1.0
+    properties:
       value:
         tag: tag:stsci.edu:asdf/core/ndarray-1.0.0
         datatype: float32
         ndim: 3
       unit:
         tag: tag:astropy.org:astropy/units/unit-1.0.0
         enum: ["DN"]
-    border_ref_pix_right:
-      title: Original border reference pixels, on right (from viewers perspective).
-      tag: tag:stsci.edu:asdf/unit/quantity-1.1.0
-      properties:
-        value:
-          tag: tag:stsci.edu:asdf/core/ndarray-1.0.0
-          datatype: float32
-          ndim: 3
-        unit:
-          tag: tag:astropy.org:astropy/units/unit-1.0.0
-          enum: ["DN"]
-    border_ref_pix_top:
-      title: Original border reference pixels, on top.
-      tag: tag:stsci.edu:asdf/unit/quantity-1.1.0
-      properties:
-        value:
-          tag: tag:stsci.edu:asdf/core/ndarray-1.0.0
-          datatype: float32
-          ndim: 3
-        unit:
-          tag: tag:astropy.org:astropy/units/unit-1.0.0
-          enum: ["DN"]
-    border_ref_pix_bottom:
-      title: Original border reference pixels, on bottom.
-      tag: tag:stsci.edu:asdf/unit/quantity-1.1.0
-      properties:
-        value:
-          tag: tag:stsci.edu:asdf/core/ndarray-1.0.0
-          datatype: float32
-          ndim: 3
-        unit:
-          tag: tag:astropy.org:astropy/units/unit-1.0.0
-          enum: ["DN"]
-    dq_border_ref_pix_left:
-      title: DQ for border reference pixels, on left (from viewers perspective).
-      tag: tag:stsci.edu:asdf/core/ndarray-1.0.0
-      datatype: uint32
-      ndim: 2
-    dq_border_ref_pix_right:
-      title: DQ for border reference pixels, on right (from viewers perspective).
-      tag: tag:stsci.edu:asdf/core/ndarray-1.0.0
-      datatype: uint32
-      ndim: 2
-    dq_border_ref_pix_top:
-      title: DQ for border reference pixels, on top.
-      tag: tag:stsci.edu:asdf/core/ndarray-1.0.0
-      datatype: uint32
-      ndim: 2
-    dq_border_ref_pix_bottom:
-      title: DQ for border reference pixels, on bottom.
-      tag: tag:stsci.edu:asdf/core/ndarray-1.0.0
-      datatype: uint32
-      ndim: 2
-  propertyOrder: [meta, data, pixeldq, groupdq, err, amp33, border_ref_pix_left,
-                  border_ref_pix_right, border_ref_pix_top,
-                  border_ref_pix_bottom, dq_border_ref_pix_left,
-                  dq_border_ref_pix_right, dq_border_ref_pix_top,
-                  dq_border_ref_pix_bottom]
-  flowStyle: block
-  required: [meta, data, pixeldq, groupdq, err, amp33, border_ref_pix_left,
-             border_ref_pix_right, border_ref_pix_top, border_ref_pix_bottom,
-             dq_border_ref_pix_left, dq_border_ref_pix_right,
-             dq_border_ref_pix_top, dq_border_ref_pix_bottom]
+  border_ref_pix_top:
+    title: Original border reference pixels, on top.
+    tag: tag:stsci.edu:asdf/unit/quantity-1.1.0
+    properties:
+      value:
+        tag: tag:stsci.edu:asdf/core/ndarray-1.0.0
+        datatype: float32
+        ndim: 3
+      unit:
+        tag: tag:astropy.org:astropy/units/unit-1.0.0
+        enum: ["DN"]
+  border_ref_pix_bottom:
+    title: Original border reference pixels, on bottom.
+    tag: tag:stsci.edu:asdf/unit/quantity-1.1.0
+    properties:
+      value:
+        tag: tag:stsci.edu:asdf/core/ndarray-1.0.0
+        datatype: float32
+        ndim: 3
+      unit:
+        tag: tag:astropy.org:astropy/units/unit-1.0.0
+        enum: ["DN"]
+  dq_border_ref_pix_left:
+    title: DQ for border reference pixels, on left (from viewers perspective).
+    tag: tag:stsci.edu:asdf/core/ndarray-1.0.0
+    datatype: uint32
+    ndim: 2
+  dq_border_ref_pix_right:
+    title: DQ for border reference pixels, on right (from viewers perspective).
+    tag: tag:stsci.edu:asdf/core/ndarray-1.0.0
+    datatype: uint32
+    ndim: 2
+  dq_border_ref_pix_top:
+    title: DQ for border reference pixels, on top.
+    tag: tag:stsci.edu:asdf/core/ndarray-1.0.0
+    datatype: uint32
+    ndim: 2
+  dq_border_ref_pix_bottom:
+    title: DQ for border reference pixels, on bottom.
+    tag: tag:stsci.edu:asdf/core/ndarray-1.0.0
+    datatype: uint32
+    ndim: 2
+propertyOrder: [meta, data, pixeldq, groupdq, err, amp33, border_ref_pix_left,
+                border_ref_pix_right, border_ref_pix_top,
+                border_ref_pix_bottom, dq_border_ref_pix_left,
+                dq_border_ref_pix_right, dq_border_ref_pix_top,
+                dq_border_ref_pix_bottom]
+flowStyle: block
+required: [meta, data, pixeldq, groupdq, err, amp33, border_ref_pix_left,
+           border_ref_pix_right, border_ref_pix_top, border_ref_pix_bottom,
+           dq_border_ref_pix_left, dq_border_ref_pix_right,
+           dq_border_ref_pix_top, dq_border_ref_pix_bottom]
 ...
```

### Comparing `rad-0.15.0/src/rad/resources/schemas/ramp_fit_output-1.0.0.yaml` & `rad-0.16.0/src/rad/resources/schemas/ramp_fit_output-1.0.0.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -1,112 +1,112 @@
 %YAML 1.1
 ---
 $schema: asdf://stsci.edu/datamodels/roman/schemas/rad_schema-1.0.0
 id: asdf://stsci.edu/datamodels/roman/schemas/ramp_fit_output-1.0.0
 
 title: Ramp fit output schema
 
-allOf:
-- type: object
-  properties:
-    meta:
-      allOf:
-        - $ref: common-1.0.0
-    slope:
-      title: Segment-specific slope
-      tag: tag:stsci.edu:asdf/unit/quantity-1.1.0
-      properties:
-        value:
-          tag: tag:stsci.edu:asdf/core/ndarray-1.0.0
-          datatype: float32
-          ndim: 3
-        unit:
-          tag: tag:astropy.org:astropy/units/unit-1.0.0
-          enum: ["electron / s"]
-    sigslope:
-      title: Sigma for segment-specific slope
-      tag: tag:stsci.edu:asdf/unit/quantity-1.1.0
-      properties:
-        value:
-          tag: tag:stsci.edu:asdf/core/ndarray-1.0.0
-          datatype: float32
-          ndim: 3
-        unit:
-          tag: tag:astropy.org:astropy/units/unit-1.0.0
-          enum: ["electron / s"]
-    yint:
-      title: Segment-specific y-intercept
-      tag: tag:stsci.edu:asdf/unit/quantity-1.1.0
-      properties:
-        value:
-          tag: tag:stsci.edu:asdf/core/ndarray-1.0.0
-          datatype: float32
-          ndim: 3
-        unit:
-          tag: tag:astropy.org:astropy/units/unit-1.0.0
-          enum: ["electron"]
-    sigyint:
-      title: Sigma for segment-specific y-intercept
-      tag: tag:stsci.edu:asdf/unit/quantity-1.1.0
-      properties:
-        value:
-          tag: tag:stsci.edu:asdf/core/ndarray-1.0.0
-          datatype: float32
-          ndim: 3
-        unit:
-          tag: tag:astropy.org:astropy/units/unit-1.0.0
-          enum: ["electron"]
-    pedestal:
-      title: Pedestal array
-      tag: tag:stsci.edu:asdf/unit/quantity-1.1.0
-      properties:
-        value:
-          tag: tag:stsci.edu:asdf/core/ndarray-1.0.0
-          datatype: float32
-          ndim: 2
-        unit:
-          tag: tag:astropy.org:astropy/units/unit-1.0.0
-          enum: ["electron"]
-    weights:
-      title: Weights for segment-specific fits
-      tag: tag:stsci.edu:asdf/core/ndarray-1.0.0
-      ndim: 3
-      datatype: float32
-    crmag:
-      title: Approximate CR magnitudes
-      tag: tag:stsci.edu:asdf/unit/quantity-1.1.0
-      properties:
-        value:
-          tag: tag:stsci.edu:asdf/core/ndarray-1.0.0
-          datatype: float32
-          ndim: 3
-        unit:
-          tag: tag:astropy.org:astropy/units/unit-1.0.0
-          enum: ["electron"]
-    var_poisson:
-      title: Variance due to poisson noise for segment-specific slope
-      tag: tag:stsci.edu:asdf/unit/quantity-1.1.0
-      properties:
-        value:
-          tag: tag:stsci.edu:asdf/core/ndarray-1.0.0
-          datatype: float32
-          ndim: 3
-        unit:
-          tag: tag:astropy.org:astropy/units/unit-1.0.0
-          enum: ["electron2 / s2"]
-    var_rnoise:
-      title: Variance due to read noise for segment-specific slope
-      tag: tag:stsci.edu:asdf/unit/quantity-1.1.0
-      properties:
-        value:
-          tag: tag:stsci.edu:asdf/core/ndarray-1.0.0
-          datatype: float32
-          ndim: 3
-        unit:
-          tag: tag:astropy.org:astropy/units/unit-1.0.0
-          enum: ["electron2 / s2"]
-  required: [meta, slope, sigslope, yint, sigyint, pedestal, weights, crmag, var_poisson,
-             var_rnoise]
-  propertyOrder: [meta, slope, sigslope, yint, sigyint, pedestal, weights, crmag, var_poisson,
-                  var_rnoise]
+datamodel_name: RampFitOutputModel
+
+type: object
+properties:
+  meta:
+    $ref: common-1.0.0
+  slope:
+    title: Segment-specific slope
+    tag: tag:stsci.edu:asdf/unit/quantity-1.1.0
+    properties:
+      value:
+        tag: tag:stsci.edu:asdf/core/ndarray-1.0.0
+        datatype: float32
+        ndim: 3
+      unit:
+        tag: tag:astropy.org:astropy/units/unit-1.0.0
+        enum: ["electron / s"]
+  sigslope:
+    title: Sigma for segment-specific slope
+    tag: tag:stsci.edu:asdf/unit/quantity-1.1.0
+    properties:
+      value:
+        tag: tag:stsci.edu:asdf/core/ndarray-1.0.0
+        datatype: float32
+        ndim: 3
+      unit:
+        tag: tag:astropy.org:astropy/units/unit-1.0.0
+        enum: ["electron / s"]
+  yint:
+    title: Segment-specific y-intercept
+    tag: tag:stsci.edu:asdf/unit/quantity-1.1.0
+    properties:
+      value:
+        tag: tag:stsci.edu:asdf/core/ndarray-1.0.0
+        datatype: float32
+        ndim: 3
+      unit:
+        tag: tag:astropy.org:astropy/units/unit-1.0.0
+        enum: ["electron"]
+  sigyint:
+    title: Sigma for segment-specific y-intercept
+    tag: tag:stsci.edu:asdf/unit/quantity-1.1.0
+    properties:
+      value:
+        tag: tag:stsci.edu:asdf/core/ndarray-1.0.0
+        datatype: float32
+        ndim: 3
+      unit:
+        tag: tag:astropy.org:astropy/units/unit-1.0.0
+        enum: ["electron"]
+  pedestal:
+    title: Pedestal array
+    tag: tag:stsci.edu:asdf/unit/quantity-1.1.0
+    properties:
+      value:
+        tag: tag:stsci.edu:asdf/core/ndarray-1.0.0
+        datatype: float32
+        ndim: 2
+      unit:
+        tag: tag:astropy.org:astropy/units/unit-1.0.0
+        enum: ["electron"]
+  weights:
+    title: Weights for segment-specific fits
+    tag: tag:stsci.edu:asdf/core/ndarray-1.0.0
+    ndim: 3
+    datatype: float32
+  crmag:
+    title: Approximate CR magnitudes
+    tag: tag:stsci.edu:asdf/unit/quantity-1.1.0
+    properties:
+      value:
+        tag: tag:stsci.edu:asdf/core/ndarray-1.0.0
+        datatype: float32
+        ndim: 3
+      unit:
+        tag: tag:astropy.org:astropy/units/unit-1.0.0
+        enum: ["electron"]
+  var_poisson:
+    title: Variance due to poisson noise for segment-specific slope
+    tag: tag:stsci.edu:asdf/unit/quantity-1.1.0
+    properties:
+      value:
+        tag: tag:stsci.edu:asdf/core/ndarray-1.0.0
+        datatype: float32
+        ndim: 3
+      unit:
+        tag: tag:astropy.org:astropy/units/unit-1.0.0
+        enum: ["electron2 / s2"]
+  var_rnoise:
+    title: Variance due to read noise for segment-specific slope
+    tag: tag:stsci.edu:asdf/unit/quantity-1.1.0
+    properties:
+      value:
+        tag: tag:stsci.edu:asdf/core/ndarray-1.0.0
+        datatype: float32
+        ndim: 3
+      unit:
+        tag: tag:astropy.org:astropy/units/unit-1.0.0
+        enum: ["electron2 / s2"]
+required: [meta, slope, sigslope, yint, sigyint, pedestal, weights, crmag, var_poisson,
+           var_rnoise]
+propertyOrder: [meta, slope, sigslope, yint, sigyint, pedestal, weights, crmag, var_poisson,
+                var_rnoise]
 flowStyle: block
 ...
```

### Comparing `rad-0.15.0/src/rad/resources/schemas/ref_file-1.0.0.yaml` & `rad-0.16.0/src/rad/resources/schemas/ref_file-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.15.0/src/rad/resources/schemas/reference_files/dark-1.0.0.yaml` & `rad-0.16.0/src/rad/resources/schemas/reference_files/dark-1.0.0.yaml`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 %YAML 1.1
 ---
 $schema: asdf://stsci.edu/datamodels/roman/schemas/rad_schema-1.0.0
 id: asdf://stsci.edu/datamodels/roman/schemas/reference_files/dark-1.0.0
 
 title: Dark reference schema
 
+datamodel_name: DarkRefModel
+
 type: object
 properties:
   meta:
     allOf:
       - $ref: ref_common-1.0.0
       - type: object
         properties:
           reftype:
+            type: string
             enum: [DARK]
           exposure:
             type: object
             properties:
               ngroups:
                 title: Number of groups in integration
                 type: integer
```

### Comparing `rad-0.15.0/src/rad/resources/schemas/reference_files/distortion-1.0.0.yaml` & `rad-0.16.0/src/rad/resources/schemas/reference_files/distortion-1.0.0.yaml`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 %YAML 1.1
 ---
 $schema: asdf://stsci.edu/datamodels/roman/schemas/rad_schema-1.0.0
 id: asdf://stsci.edu/datamodels/roman/schemas/reference_files/distortion-1.0.0
 
 title: Distortion reference schema
 
+datamodel_name: DistortionRefModel
+
 type: object
 properties:
   meta:
     allOf:
       - $ref: ref_common-1.0.0
       - type: object
         properties:
           reftype:
+            type: string
             enum: [DISTORTION]
           input_units:
             title: Units of the detector coordinate inputs to this model.
             tag: tag:stsci.edu:asdf/unit/unit-1.0.0
             enum: ["pixel"]
           output_units:
             title: Output units of V2/V3 coordinates after the model is applied.
```

### Comparing `rad-0.15.0/src/rad/resources/schemas/reference_files/flat-1.0.0.yaml` & `rad-0.16.0/src/rad/resources/schemas/reference_files/superbias-1.0.0.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -1,37 +1,38 @@
 %YAML 1.1
 ---
 $schema: asdf://stsci.edu/datamodels/roman/schemas/rad_schema-1.0.0
-id: asdf://stsci.edu/datamodels/roman/schemas/reference_files/flat-1.0.0
+id: asdf://stsci.edu/datamodels/roman/schemas/reference_files/superbias-1.0.0
 
-title: Flat reference schema
+title: Super-bias reference schema
+
+datamodel_name: SuperbiasRefModel
 
 type: object
 properties:
   meta:
     allOf:
       - $ref: ref_common-1.0.0
       - type: object
         properties:
           reftype:
             type: string
-            enum: [FLAT]
-      - $ref: ref_optical_element-1.0.0
+            enum: [BIAS]
   data:
-    title: Flat data array
+    title: 2-D super-bias array
     tag: tag:stsci.edu:asdf/core/ndarray-1.0.0
     datatype: float32
     ndim: 2
   dq:
-    title: Data quality array
+    title: 2-D data quality array for all planes
     tag: tag:stsci.edu:asdf/core/ndarray-1.0.0
     datatype: uint32
     ndim: 2
   err:
-    title: Error array
+    title: 2-D Error array
     tag: tag:stsci.edu:asdf/core/ndarray-1.0.0
     datatype: float32
     ndim: 2
 required: [meta, data, dq, err]
 flowStyle: block
 propertyOrder: [meta, data, dq, err]
 ...
```

### Comparing `rad-0.15.0/src/rad/resources/schemas/reference_files/gain-1.0.0.yaml` & `rad-0.16.0/src/rad/resources/schemas/reference_files/mask-1.0.0.yaml`

 * *Files 16% similar despite different names*

```diff
@@ -1,32 +1,28 @@
 %YAML 1.1
 ---
 $schema: asdf://stsci.edu/datamodels/roman/schemas/rad_schema-1.0.0
-id: asdf://stsci.edu/datamodels/roman/schemas/reference_files/gain-1.0.0
+id: asdf://stsci.edu/datamodels/roman/schemas/reference_files/mask-1.0.0
 
-title: Gain reference schema
+title: DQ Mask reference schema
+
+datamodel_name: MaskRefModel
 
 type: object
 properties:
   meta:
     allOf:
       - $ref: ref_common-1.0.0
       - type: object
         properties:
           reftype:
             type: string
-            enum: [GAIN]
-  data:
-    title: The detector gain map
-    tag: tag:stsci.edu:asdf/unit/quantity-1.1.0
-    properties:
-      value:
-        tag: tag:stsci.edu:asdf/core/ndarray-1.0.0
-        datatype: float32
-        ndim: 2
-      unit:
-        tag: tag:astropy.org:astropy/units/unit-1.0.0
-        enum: ["electron / DN"]
-required: [meta, data]
+            enum: [MASK]
+  dq:
+    title: Data quality mask array
+    tag: tag:stsci.edu:asdf/core/ndarray-1.0.0
+    datatype: uint32
+    ndim: 2
+required: [meta, dq]
 flowStyle: block
-propertyOrder: [meta, data]
+propertyOrder: [meta, dq]
 ...
```

### Comparing `rad-0.15.0/src/rad/resources/schemas/reference_files/inverse_linearity-1.0.0.yaml` & `rad-0.16.0/src/rad/resources/schemas/reference_files/inverse_linearity-1.0.0.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 %YAML 1.1
 ---
 $schema: asdf://stsci.edu/datamodels/roman/schemas/rad_schema-1.0.0
 id: asdf://stsci.edu/datamodels/roman/schemas/reference_files/inverse_linearity-1.0.0
 
 title: Inverse linearity correction reference schema
 
+datamodel_name: InverseLinearityRefModel
+
 type: object
 properties:
   meta:
     allOf:
       - $ref: ref_common-1.0.0
       - type: object
         properties:
           reftype:
             type: string
-            enum: [INVERSE_LINEARITY]
+            enum: [INVERSELINEARITY]
           input_units:
             title: Units of the input to the inverse linearity polynomial.
             tag: tag:astropy.org:astropy/units/unit-1.0.0
             enum: ["DN"]
           output_units:
             title: Units of the output of the inverse linearity polynomial.
             tag: tag:astropy.org:astropy/units/unit-1.0.0
```

### Comparing `rad-0.15.0/src/rad/resources/schemas/reference_files/ipc-1.0.0.yaml` & `rad-0.16.0/src/rad/resources/schemas/reference_files/ipc-1.0.0.yaml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 %YAML 1.1
 ---
 $schema: asdf://stsci.edu/datamodels/roman/schemas/rad_schema-1.0.0
 id: asdf://stsci.edu/datamodels/roman/schemas/reference_files/ipc-1.0.0
 
 title: IPC kernel reference schema
 
+datamodel_name: IpcRefModel
+
 type: object
 properties:
   meta:
     allOf:
       - $ref: ref_common-1.0.0
       - $ref: ref_optical_element-1.0.0
       - type: object
```

### Comparing `rad-0.15.0/src/rad/resources/schemas/reference_files/linearity-1.0.0.yaml` & `rad-0.16.0/src/rad/resources/schemas/reference_files/linearity-1.0.0.yaml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 %YAML 1.1
 ---
 $schema: asdf://stsci.edu/datamodels/roman/schemas/rad_schema-1.0.0
 id: asdf://stsci.edu/datamodels/roman/schemas/reference_files/linearity-1.0.0
 
 title: Linearity correction  reference schema
 
+datamodel_name: LinearityRefModel
+
 type: object
 properties:
   meta:
     allOf:
       - $ref: ref_common-1.0.0
       - type: object
         properties:
```

### Comparing `rad-0.15.0/src/rad/resources/schemas/reference_files/mask-1.0.0.yaml` & `rad-0.16.0/src/rad/resources/schemas/reference_files/gain-1.0.0.yaml`

 * *Files 27% similar despite different names*

```diff
@@ -1,27 +1,34 @@
 %YAML 1.1
 ---
 $schema: asdf://stsci.edu/datamodels/roman/schemas/rad_schema-1.0.0
-id: asdf://stsci.edu/datamodels/roman/schemas/reference_files/mask-1.0.0
+id: asdf://stsci.edu/datamodels/roman/schemas/reference_files/gain-1.0.0
 
-title: DQ Mask reference schema
+title: Gain reference schema
 
+datamodel_name: GainRefModel
 
 type: object
 properties:
   meta:
     allOf:
       - $ref: ref_common-1.0.0
       - type: object
         properties:
           reftype:
             type: string
-            enum: [MASK]
-  dq:
-    title: Data quality mask array
-    tag: tag:stsci.edu:asdf/core/ndarray-1.0.0
-    datatype: uint32
-    ndim: 2
-required: [meta, dq]
+            enum: [GAIN]
+  data:
+    title: The detector gain map
+    tag: tag:stsci.edu:asdf/unit/quantity-1.1.0
+    properties:
+      value:
+        tag: tag:stsci.edu:asdf/core/ndarray-1.0.0
+        datatype: float32
+        ndim: 2
+      unit:
+        tag: tag:astropy.org:astropy/units/unit-1.0.0
+        enum: ["electron / DN"]
+required: [meta, data]
 flowStyle: block
-propertyOrder: [meta, dq]
+propertyOrder: [meta, data]
 ...
```

### Comparing `rad-0.15.0/src/rad/resources/schemas/reference_files/pixelarea-1.0.0.yaml` & `rad-0.16.0/src/rad/resources/schemas/reference_files/pixelarea-1.0.0.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 %YAML 1.1
 ---
 $schema: asdf://stsci.edu/datamodels/roman/schemas/rad_schema-1.0.0
 id: asdf://stsci.edu/datamodels/roman/schemas/reference_files/pixelarea-1.0.0
 
 title: Pixel area reference schema
 
+datamodel_name: PixelareaRefModel
+
 type: object
 properties:
   meta:
     allOf:
       - $ref: ref_common-1.0.0
       - type: object
         properties:
```

### Comparing `rad-0.15.0/src/rad/resources/schemas/reference_files/readnoise-1.0.0.yaml` & `rad-0.16.0/src/rad/resources/schemas/reference_files/readnoise-1.0.0.yaml`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 %YAML 1.1
 ---
 $schema: asdf://stsci.edu/datamodels/roman/schemas/rad_schema-1.0.0
 id: asdf://stsci.edu/datamodels/roman/schemas/reference_files/readnoise-1.0.0
 
 title: Read noise reference schema
 
+datamodel_name: ReadnoiseRefModel
+
 type: object
 properties:
   meta:
     allOf:
       - $ref: ref_common-1.0.0
       - type: object
         properties:
```

### Comparing `rad-0.15.0/src/rad/resources/schemas/reference_files/ref_common-1.0.0.yaml` & `rad-0.16.0/src/rad/resources/schemas/reference_files/ref_common-1.0.0.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -1,47 +1,46 @@
 %YAML 1.1
 ---
 $schema: asdf://stsci.edu/datamodels/roman/schemas/rad_schema-1.0.0
 id: asdf://stsci.edu/datamodels/roman/schemas/reference_files/ref_common-1.0.0
 
 title: Common reference metadata properties
 
-allOf:
-- type: object
-  properties:
-    reftype:
-      title: Reference File type
-      type: string
-    pedigree:
-      title: The pedigree of the reference file
-      type: string
-      enum: [GROUND, MODEL, DUMMY, SIMULATION]
-    description:
-      title: Description of the reference file
-      type: string
-    author:
-      title: Author of the reference file
-      type: string
-    useafter:
-      title: Use after date of the reference file
-      tag: tag:stsci.edu:asdf/time/time-1.1.0
-    telescope:
-      title: Telescope data reference data is used to calibrate
-      anyOf:
-        - tag: asdf://stsci.edu/datamodels/roman/tags/telescope-1.0.0
-        - type: string
-          enum: [ROMAN]
-    origin:
-      title: Organization responsible for creating file
-      type: string
-    instrument:
-      type: object
-      properties:
-        name:
-          title: Instrument used to acquire the data
-          type: string
-          enum: [WFI]
-        detector:
-          $ref: ../wfi_detector-1.0.0
-      required: [name, detector]
-  required: [reftype, author, description, pedigree, useafter, telescope, origin, instrument]
+type: object
+properties:
+  reftype:
+    title: Reference File type
+    type: string
+  pedigree:
+    title: The pedigree of the reference file
+    type: string
+    enum: [GROUND, MODEL, DUMMY, SIMULATION]
+  description:
+    title: Description of the reference file
+    type: string
+  author:
+    title: Author of the reference file
+    type: string
+  useafter:
+    title: Use after date of the reference file
+    tag: tag:stsci.edu:asdf/time/time-1.1.0
+  telescope:
+    title: Telescope data reference data is used to calibrate
+    anyOf:
+      - tag: asdf://stsci.edu/datamodels/roman/tags/telescope-1.0.0
+      - type: string
+        enum: [ROMAN]
+  origin:
+    title: Organization responsible for creating file
+    type: string
+  instrument:
+    type: object
+    properties:
+      name:
+        title: Instrument used to acquire the data
+        type: string
+        enum: [WFI]
+      detector:
+        $ref: ../wfi_detector-1.0.0
+    required: [name, detector]
+required: [reftype, author, description, pedigree, useafter, telescope, origin, instrument]
 ...
```

### Comparing `rad-0.15.0/src/rad/resources/schemas/reference_files/saturation-1.0.0.yaml` & `rad-0.16.0/src/rad/resources/schemas/reference_files/saturation-1.0.0.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 %YAML 1.1
 ---
 $schema: asdf://stsci.edu/datamodels/roman/schemas/rad_schema-1.0.0
 id: asdf://stsci.edu/datamodels/roman/schemas/reference_files/saturation-1.0.0
 
 title: Saturation reference schema
 
+datamodel_name: SaturationRefModel
+
 type: object
 properties:
   meta:
     allOf:
       - $ref: ref_common-1.0.0
       - type: object
         properties:
```

### Comparing `rad-0.15.0/src/rad/resources/schemas/reference_files/superbias-1.0.0.yaml` & `rad-0.16.0/src/rad/resources/schemas/msos_stack-1.0.0.yaml`

 * *Files 15% similar despite different names*

```diff
@@ -1,36 +1,45 @@
 %YAML 1.1
 ---
 $schema: asdf://stsci.edu/datamodels/roman/schemas/rad_schema-1.0.0
-id: asdf://stsci.edu/datamodels/roman/schemas/reference_files/superbias-1.0.0
+id: asdf://stsci.edu/datamodels/roman/schemas/msos_stack-1.0.0
 
-title: Super-bias reference schema
+title: |
+  MSOS Stack Level 3 Schema
+
+datamodel_name: MsosStackModel
 
 type: object
 properties:
   meta:
     allOf:
-      - $ref: ref_common-1.0.0
-      - type: object
-        properties:
-          reftype:
-            type: string
-            enum: [BIAS]
+      - $ref: common-1.0.0
+      - image_list:
+          type: string
   data:
-    title: 2-D super-bias array
-    tag: tag:stsci.edu:asdf/core/ndarray-1.0.0
-    datatype: float32
-    ndim: 2
-  dq:
-    title: 2-D data quality array for all planes
-    tag: tag:stsci.edu:asdf/core/ndarray-1.0.0
-    datatype: uint32
-    ndim: 2
-  err:
-    title: 2-D Error array
-    tag: tag:stsci.edu:asdf/core/ndarray-1.0.0
-    datatype: float32
-    ndim: 2
-required: [meta, data, dq, err]
+    title: Flux data
+    value:
+      tag: tag:stsci.edu:asdf/core/ndarray-1.0.0
+      datatype: float64
+      ndim: 2
+  uncertainty:
+    title: uncertainty data
+    value:
+      tag: tag:stsci.edu:asdf/core/ndarray-1.0.0
+      datatype: float64
+      ndim: 2
+  mask:
+    title: mask data
+    value:
+      tag: tag:stsci.edu:asdf/core/ndarray-1.0.0
+      datatype: uint8
+      ndim: 2
+  coverage:
+    title: coverage data
+    value:
+      tag: tag:stsci.edu:asdf/core/ndarray-1.0.0
+      datatype: uint8
+      ndim: 2
+propertyOrder: [meta, data, uncertainty, mask, coverage]
 flowStyle: block
-propertyOrder: [meta, data, dq, err]
+required: [meta, data, uncertainty, mask, coverage]
 ...
```

### Comparing `rad-0.15.0/src/rad/resources/schemas/reference_files/wfi_img_photom-1.0.0.yaml` & `rad-0.16.0/src/rad/resources/schemas/reference_files/wfi_img_photom-1.0.0.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 %YAML 1.1
 ---
 $schema: asdf://stsci.edu/datamodels/roman/schemas/rad_schema-1.0.0
 id: asdf://stsci.edu/datamodels/roman/schemas/reference_files/wfi_img_photom-1.0.0
 
 title: WFI imaging photometric flux conversion data model
 
+datamodel_name: WfiImgPhotomRefModel
+
 type: object
 properties:
   meta:
     allOf:
       - $ref: ref_common-1.0.0
       - type: object
         properties:
```

### Comparing `rad-0.15.0/src/rad/resources/schemas/resample-1.0.0.yaml` & `rad-0.16.0/src/rad/resources/schemas/resample-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.15.0/src/rad/resources/schemas/target-1.0.0.yaml` & `rad-0.16.0/src/rad/resources/schemas/target-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.15.0/src/rad/resources/schemas/variance-1.0.0.yaml` & `rad-0.16.0/src/rad/resources/schemas/variance-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.15.0/src/rad/resources/schemas/velocity_aberration-1.0.0.yaml` & `rad-0.16.0/src/rad/resources/schemas/velocity_aberration-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.15.0/src/rad/resources/schemas/visit-1.0.0.yaml` & `rad-0.16.0/src/rad/resources/schemas/visit-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.15.0/src/rad/resources/schemas/wcsinfo-1.0.0.yaml` & `rad-0.16.0/src/rad/resources/schemas/wcsinfo-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.15.0/src/rad/resources/schemas/wfi_image-1.0.0.yaml` & `rad-0.16.0/src/rad/resources/schemas/wfi_image-1.0.0.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 ---
 $schema: asdf://stsci.edu/datamodels/roman/schemas/rad_schema-1.0.0
 id: asdf://stsci.edu/datamodels/roman/schemas/wfi_image-1.0.0
 
 title: |
   The schema for WFI Level 2 images.
 
+datamodel_name: ImageModel
+
 type: object
 properties:
   meta:
     allOf:
       - $ref: common-1.0.0
       - type: object
         properties:
```

### Comparing `rad-0.15.0/src/rad/resources/schemas/wfi_mode-1.0.0.yaml` & `rad-0.16.0/src/rad/resources/schemas/wfi_mode-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.15.0/src/rad/resources/schemas/wfi_mosaic-1.0.0.yaml` & `rad-0.16.0/src/rad/resources/schemas/wfi_mosaic-1.0.0.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 ---
 $schema: asdf://stsci.edu/datamodels/roman/schemas/rad_schema-1.0.0
 id: asdf://stsci.edu/datamodels/roman/schemas/wfi_mosaic-1.0.0
 
 title: |
   The schema for WFI Level 3 mosaics.
 
+datamodel_name: MosaicModel
+
 type: object
 properties:
   meta:
     allOf:
       - $ref: common-1.0.0
       - type: object
         properties:
```

### Comparing `rad-0.15.0/src/rad/resources/schemas/wfi_science_raw-1.0.0.yaml` & `rad-0.16.0/src/rad/resources/schemas/wfi_science_raw-1.0.0.yaml`

 * *Files 9% similar despite different names*

```diff
@@ -2,19 +2,20 @@
 ---
 $schema: asdf://stsci.edu/datamodels/roman/schemas/rad_schema-1.0.0
 id: asdf://stsci.edu/datamodels/roman/schemas/wfi_science_raw-1.0.0
 
 title: |
   The schema for Level 1 WFI science data (both imaging and spectrographic).
 
+datamodel_name: ScienceRawModel
+
 type: object
 properties:
   meta:
-    allOf:
-      - $ref: common-1.0.0
+    $ref: common-1.0.0
   data:
     title: Science data, including the border reference pixels.
     tag: tag:stsci.edu:asdf/unit/quantity-1.1.0
     properties:
       value:
         tag: tag:stsci.edu:asdf/core/ndarray-1.0.0
         datatype: uint16
```

### Comparing `rad-0.15.0/src/rad.egg-info/PKG-INFO` & `rad-0.16.0/src/rad.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rad
-Version: 0.15.0
+Version: 0.16.0
 Summary: Roman Attribute Dictionary
 Author-email: STScI <help@stsci.edu>
 License: Copyright (C) 2021 Association of Universities for Research in Astronomy (AURA)
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
```

### Comparing `rad-0.15.0/src/rad.egg-info/SOURCES.txt` & `rad-0.16.0/src/rad.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -53,14 +53,15 @@
 src/rad/resources/schemas/coordinates-1.0.0.yaml
 src/rad/resources/schemas/ephemeris-1.0.0.yaml
 src/rad/resources/schemas/exposure-1.0.0.yaml
 src/rad/resources/schemas/exposure_type-1.0.0.yaml
 src/rad/resources/schemas/guidestar-1.0.0.yaml
 src/rad/resources/schemas/guidewindow-1.0.0.yaml
 src/rad/resources/schemas/guidewindow_modes-1.0.0.yaml
+src/rad/resources/schemas/msos_stack-1.0.0.yaml
 src/rad/resources/schemas/observation-1.0.0.yaml
 src/rad/resources/schemas/photometry-1.0.0.yaml
 src/rad/resources/schemas/pointing-1.0.0.yaml
 src/rad/resources/schemas/program-1.0.0.yaml
 src/rad/resources/schemas/rad_schema-1.0.0.yaml
 src/rad/resources/schemas/ramp-1.0.0.yaml
 src/rad/resources/schemas/ramp_fit_output-1.0.0.yaml
@@ -87,22 +88,24 @@
 src/rad/resources/schemas/reference_files/linearity-1.0.0.yaml
 src/rad/resources/schemas/reference_files/mask-1.0.0.yaml
 src/rad/resources/schemas/reference_files/pixelarea-1.0.0.yaml
 src/rad/resources/schemas/reference_files/readnoise-1.0.0.yaml
 src/rad/resources/schemas/reference_files/ref_common-1.0.0.yaml
 src/rad/resources/schemas/reference_files/ref_exposure_type-1.0.0.yaml
 src/rad/resources/schemas/reference_files/ref_optical_element-1.0.0.yaml
+src/rad/resources/schemas/reference_files/refpix-1.0.0.yaml
 src/rad/resources/schemas/reference_files/saturation-1.0.0.yaml
 src/rad/resources/schemas/reference_files/superbias-1.0.0.yaml
 src/rad/resources/schemas/reference_files/wfi_img_photom-1.0.0.yaml
 src/rad/resources/schemas/tagged_scalars/calibration_software_version-1.0.0.yaml
 src/rad/resources/schemas/tagged_scalars/file_date-1.0.0.yaml
 src/rad/resources/schemas/tagged_scalars/filename-1.0.0.yaml
 src/rad/resources/schemas/tagged_scalars/model_type-1.0.0.yaml
 src/rad/resources/schemas/tagged_scalars/origin-1.0.0.yaml
 src/rad/resources/schemas/tagged_scalars/prd_software_version-1.0.0.yaml
 src/rad/resources/schemas/tagged_scalars/sdf_software_version-1.0.0.yaml
 src/rad/resources/schemas/tagged_scalars/telescope-1.0.0.yaml
+tests/__init__.py
 tests/conftest.py
 tests/test_integration.py
 tests/test_manifest.py
 tests/test_schemas.py
```

### Comparing `rad-0.15.0/tests/test_integration.py` & `rad-0.16.0/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `rad-0.15.0/tests/test_manifest.py` & `rad-0.16.0/tests/test_manifest.py`

 * *Files identical despite different names*

### Comparing `rad-0.15.0/tox.ini` & `rad-0.16.0/tox.ini`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 [testenv]
 description =
     run tests
     cov: with coverage
     xdist: using parallel processing
 set_env =
-    devdeps: PIP_EXTRA_INDEX_URL = https://pypi.anaconda.org/scipy-wheels-nightly/simple
+    devdeps: PIP_EXTRA_INDEX_URL = https://pypi.anaconda.org/scientific-python-nightly-wheels/simple
 extras =
     test
 deps =
     xdist: pytest-xdist
     cov: pytest-cov
 commands_pre =
     devdeps: pip install numpy>=0.0.dev0 git+https://github.com/astropy/astropy.git -U --upgrade-strategy eager
```

