# Comparing `tmp/hesperos-0.2.tar.gz` & `tmp/hesperos-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hesperos-0.2.tar", last modified: Fri Jun 16 14:05:46 2023, max compression
+gzip compressed data, was "hesperos-0.2.1.tar", last modified: Tue Jun 27 15:47:32 2023, max compression
```

## Comparing `hesperos-0.2.tar` & `hesperos-0.2.1.tar`

### file list

```diff
@@ -1,121 +1,121 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:05:46.339913 hesperos-0.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:05:46.323913 hesperos-0.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:05:46.327913 hesperos-0.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-06-16 14:05:27.000000 hesperos-0.2/.github/workflows/plugin_preview.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2796 2023-06-16 14:05:27.000000 hesperos-0.2/.github/workflows/test_and_deploy.yml
--rw-r--r--   0 runner    (1001) docker     (123)      992 2023-06-16 14:05:27.000000 hesperos-0.2/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:05:46.327913 hesperos-0.2/.napari/
--rw-r--r--   0 runner    (1001) docker     (123)     4201 2023-06-16 14:05:27.000000 hesperos-0.2/.napari/DESCRIPTION.md
--rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-06-16 14:05:27.000000 hesperos-0.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-06-16 14:05:27.000000 hesperos-0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-16 14:05:27.000000 hesperos-0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    24224 2023-06-16 14:05:46.339913 hesperos-0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    23147 2023-06-16 14:05:27.000000 hesperos-0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:05:46.323913 hesperos-0.2/materials/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:05:46.331913 hesperos-0.2/materials/interface_tools_screenshots/
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-06-16 14:05:27.000000 hesperos-0.2/materials/interface_tools_screenshots/annotation_delete_button.PNG
--rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-06-16 14:05:27.000000 hesperos-0.2/materials/interface_tools_screenshots/annotation_export_button.png
--rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-06-16 14:05:27.000000 hesperos-0.2/materials/interface_tools_screenshots/annotation_load_button.PNG
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-06-16 14:05:27.000000 hesperos-0.2/materials/interface_tools_screenshots/annotation_lock_button.PNG
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-06-16 14:05:27.000000 hesperos-0.2/materials/interface_tools_screenshots/annotation_save_button.PNG
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-06-16 14:05:27.000000 hesperos-0.2/materials/interface_tools_screenshots/annotation_undo_button.PNG
--rw-r--r--   0 runner    (1001) docker     (123)      854 2023-06-16 14:05:27.000000 hesperos-0.2/materials/interface_tools_screenshots/annotation_unlock_button.PNG
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-06-16 14:05:27.000000 hesperos-0.2/materials/interface_tools_screenshots/contrast_add_button.PNG
--rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-06-16 14:05:27.000000 hesperos-0.2/materials/interface_tools_screenshots/contrast_choose.PNG
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-06-16 14:05:27.000000 hesperos-0.2/materials/interface_tools_screenshots/contrast_export_button.PNG
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-06-16 14:05:27.000000 hesperos-0.2/materials/interface_tools_screenshots/contrast_import_button.PNG
--rw-r--r--   0 runner    (1001) docker     (123)   454140 2023-06-16 14:05:27.000000 hesperos-0.2/materials/interface_tools_screenshots/hesperos_manual_interface.PNG
--rw-r--r--   0 runner    (1001) docker     (123)   510686 2023-06-16 14:05:27.000000 hesperos-0.2/materials/interface_tools_screenshots/hesperos_oneshot_interface.PNG
--rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-06-16 14:05:27.000000 hesperos-0.2/materials/interface_tools_screenshots/image_change_axis_button.PNG
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-06-16 14:05:27.000000 hesperos-0.2/materials/interface_tools_screenshots/image_transpose_button.PNG
--rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-06-16 14:05:27.000000 hesperos-0.2/materials/interface_tools_screenshots/layer_label_erase_button.PNG
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-06-16 14:05:27.000000 hesperos-0.2/materials/interface_tools_screenshots/layer_label_fill_button.PNG
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-06-16 14:05:27.000000 hesperos-0.2/materials/interface_tools_screenshots/layer_label_paint_button.PNG
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-06-16 14:05:27.000000 hesperos-0.2/materials/interface_tools_screenshots/layer_label_zoom_button.PNG
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-06-16 14:05:27.000000 hesperos-0.2/materials/interface_tools_screenshots/open_dicom_serie_button.PNG
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-06-16 14:05:27.000000 hesperos-0.2/materials/interface_tools_screenshots/open_image_file_button.PNG
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-06-16 14:05:27.000000 hesperos-0.2/materials/interface_tools_screenshots/proba_threshold_slider.PNG
--rw-r--r--   0 runner    (1001) docker     (123)      905 2023-06-16 14:05:27.000000 hesperos-0.2/materials/interface_tools_screenshots/run_segmentation_button.PNG
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-06-16 14:05:27.000000 hesperos-0.2/materials/interface_tools_screenshots/save_probabilities_button.PNG
--rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-06-16 14:05:27.000000 hesperos-0.2/materials/interface_tools_screenshots/save_segmentation_button.PNG
--rw-r--r--   0 runner    (1001) docker     (123)   301806 2023-06-16 14:05:27.000000 hesperos-0.2/materials/interface_tools_screenshots/screen_tagging_step.PNG
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-06-16 14:05:27.000000 hesperos-0.2/materials/interface_tools_screenshots/slice_selection_add_button.png
--rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-06-16 14:05:27.000000 hesperos-0.2/materials/interface_tools_screenshots/slice_selection_drop_down_menu.png
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-06-16 14:05:27.000000 hesperos-0.2/materials/interface_tools_screenshots/slice_selection_goto_button.png
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-16 14:05:27.000000 hesperos-0.2/materials/interface_tools_screenshots/slice_selection_remove_button.png
--rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-06-16 14:05:27.000000 hesperos-0.2/materials/interface_tools_screenshots/zoom_slider.PNG
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-06-16 14:05:27.000000 hesperos-0.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:05:46.323913 hesperos-0.2/script_files/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:05:46.331913 hesperos-0.2/script_files/for_Macos/
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-06-16 14:05:27.000000 hesperos-0.2/script_files/for_Macos/install_hesperos_env.command
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-16 14:05:27.000000 hesperos-0.2/script_files/for_Macos/run_hesperos.command
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:05:46.331913 hesperos-0.2/script_files/for_Windows/
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-06-16 14:05:27.000000 hesperos-0.2/script_files/for_Windows/install_hesperos_env.bat
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-16 14:05:27.000000 hesperos-0.2/script_files/for_Windows/run_hesperos.bat
--rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-06-16 14:05:46.343913 hesperos-0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:05:46.331913 hesperos-0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:05:46.331913 hesperos-0.2/src/_tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 14:05:27.000000 hesperos-0.2/src/_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-06-16 14:05:27.000000 hesperos-0.2/src/_tests/test_widget.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:05:46.335913 hesperos-0.2/src/hesperos/
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-16 14:05:27.000000 hesperos-0.2/src/hesperos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   117963 2023-06-16 14:05:27.000000 hesperos-0.2/src/hesperos/_manual_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)    44800 2023-06-16 14:05:27.000000 hesperos-0.2/src/hesperos/_oneshot_widget.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:05:46.335913 hesperos-0.2/src/hesperos/annotation/
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-16 14:05:27.000000 hesperos-0.2/src/hesperos/annotation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-06-16 14:05:27.000000 hesperos-0.2/src/hesperos/annotation/feta.py
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-06-16 14:05:27.000000 hesperos-0.2/src/hesperos/annotation/fetus.py
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-06-16 14:05:27.000000 hesperos-0.2/src/hesperos/annotation/larva.py
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-06-16 14:05:27.000000 hesperos-0.2/src/hesperos/annotation/mouse_embryon.py
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-06-16 14:05:27.000000 hesperos-0.2/src/hesperos/annotation/oneshot.py
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-06-16 14:05:27.000000 hesperos-0.2/src/hesperos/annotation/shoulder.py
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-06-16 14:05:27.000000 hesperos-0.2/src/hesperos/annotation/shoulder_bone_border.py
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-06-16 14:05:27.000000 hesperos-0.2/src/hesperos/annotation/shoulder_bones.py
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-06-16 14:05:27.000000 hesperos-0.2/src/hesperos/annotation/shoulder_deltoid.py
--rw-r--r--   0 runner    (1001) docker     (123)     5206 2023-06-16 14:05:27.000000 hesperos-0.2/src/hesperos/annotation/structuresubpanel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:05:46.335913 hesperos-0.2/src/hesperos/layout/
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-16 14:05:27.000000 hesperos-0.2/src/hesperos/layout/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22740 2023-06-16 14:05:27.000000 hesperos-0.2/src/hesperos/layout/gui_elements.py
--rw-r--r--   0 runner    (1001) docker     (123)     7879 2023-06-16 14:05:27.000000 hesperos-0.2/src/hesperos/layout/napari_elements.py
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-06-16 14:05:27.000000 hesperos-0.2/src/hesperos/napari.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:05:46.339913 hesperos-0.2/src/hesperos/one_shot_learning/
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-16 14:05:27.000000 hesperos-0.2/src/hesperos/one_shot_learning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4094 2023-06-16 14:05:27.000000 hesperos-0.2/src/hesperos/one_shot_learning/classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)    10693 2023-06-16 14:05:27.000000 hesperos-0.2/src/hesperos/one_shot_learning/features2d.py
--rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-06-16 14:05:27.000000 hesperos-0.2/src/hesperos/one_shot_learning/features3d.py
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-06-16 14:05:27.000000 hesperos-0.2/src/hesperos/one_shot_learning/kernel.py
--rw-r--r--   0 runner    (1001) docker     (123)     5547 2023-06-16 14:05:27.000000 hesperos-0.2/src/hesperos/one_shot_learning/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:05:46.339913 hesperos-0.2/src/hesperos/resources/
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-16 14:05:27.000000 hesperos-0.2/src/hesperos/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-06-16 14:05:27.000000 hesperos-0.2/src/hesperos/resources/_icons.py
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-06-16 14:05:27.000000 hesperos-0.2/src/hesperos/resources/group_box_stylesheet.qss
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:05:46.339913 hesperos-0.2/src/hesperos/resources/icons/
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-16 14:05:27.000000 hesperos-0.2/src/hesperos/resources/icons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-06-16 14:05:27.000000 hesperos-0.2/src/hesperos/resources/icons/back.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-06-16 14:05:27.000000 hesperos-0.2/src/hesperos/resources/icons/backup.svg
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-06-16 14:05:27.000000 hesperos-0.2/src/hesperos/resources/icons/chevron_down.svg
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-06-16 14:05:27.000000 hesperos-0.2/src/hesperos/resources/icons/chevron_left.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-06-16 14:05:27.000000 hesperos-0.2/src/hesperos/resources/icons/chevron_right.svg
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-06-16 14:05:27.000000 hesperos-0.2/src/hesperos/resources/icons/chevron_up.svg
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-06-16 14:05:27.000000 hesperos-0.2/src/hesperos/resources/icons/export.svg
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-06-16 14:05:27.000000 hesperos-0.2/src/hesperos/resources/icons/import.svg
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-06-16 14:05:27.000000 hesperos-0.2/src/hesperos/resources/icons/lock.svg
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-06-16 14:05:27.000000 hesperos-0.2/src/hesperos/resources/icons/map.svg
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-06-16 14:05:27.000000 hesperos-0.2/src/hesperos/resources/icons/minus.svg
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-06-16 14:05:27.000000 hesperos-0.2/src/hesperos/resources/icons/minus2.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-06-16 14:05:27.000000 hesperos-0.2/src/hesperos/resources/icons/next.svg
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-06-16 14:05:27.000000 hesperos-0.2/src/hesperos/resources/icons/plus.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-06-16 14:05:27.000000 hesperos-0.2/src/hesperos/resources/icons/reset.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-06-16 14:05:27.000000 hesperos-0.2/src/hesperos/resources/icons/save.svg
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-06-16 14:05:27.000000 hesperos-0.2/src/hesperos/resources/icons/undo.svg
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-06-16 14:05:27.000000 hesperos-0.2/src/hesperos/resources/icons/unlock.svg
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-06-16 14:05:27.000000 hesperos-0.2/src/hesperos/resources/icons/zoom.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:05:46.335913 hesperos-0.2/src/hesperos.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    24224 2023-06-16 14:05:46.000000 hesperos-0.2/src/hesperos.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4541 2023-06-16 14:05:46.000000 hesperos-0.2/src/hesperos.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 14:05:46.000000 hesperos-0.2/src/hesperos.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-16 14:05:46.000000 hesperos-0.2/src/hesperos.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-06-16 14:05:46.000000 hesperos-0.2/src/hesperos.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-16 14:05:46.000000 hesperos-0.2/src/hesperos.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-06-16 14:05:27.000000 hesperos-0.2/src/test_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-06-16 14:05:27.000000 hesperos-0.2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 15:47:32.892045 hesperos-0.2.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 15:47:32.868043 hesperos-0.2.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 15:47:32.872043 hesperos-0.2.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-06-27 15:46:54.000000 hesperos-0.2.1/.github/workflows/plugin_preview.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2796 2023-06-27 15:46:54.000000 hesperos-0.2.1/.github/workflows/test_and_deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-06-27 15:46:54.000000 hesperos-0.2.1/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 15:47:32.872043 hesperos-0.2.1/.napari/
+-rw-r--r--   0 runner    (1001) docker     (123)     4201 2023-06-27 15:46:54.000000 hesperos-0.2.1/.napari/DESCRIPTION.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-06-27 15:46:54.000000 hesperos-0.2.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-06-27 15:46:54.000000 hesperos-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-27 15:46:54.000000 hesperos-0.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    24226 2023-06-27 15:47:32.892045 hesperos-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    23147 2023-06-27 15:46:54.000000 hesperos-0.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 15:47:32.872043 hesperos-0.2.1/materials/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 15:47:32.880044 hesperos-0.2.1/materials/interface_tools_screenshots/
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-06-27 15:46:54.000000 hesperos-0.2.1/materials/interface_tools_screenshots/annotation_delete_button.PNG
+-rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-06-27 15:46:54.000000 hesperos-0.2.1/materials/interface_tools_screenshots/annotation_export_button.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-06-27 15:46:54.000000 hesperos-0.2.1/materials/interface_tools_screenshots/annotation_load_button.PNG
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-06-27 15:46:54.000000 hesperos-0.2.1/materials/interface_tools_screenshots/annotation_lock_button.PNG
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-06-27 15:46:54.000000 hesperos-0.2.1/materials/interface_tools_screenshots/annotation_save_button.PNG
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-06-27 15:46:54.000000 hesperos-0.2.1/materials/interface_tools_screenshots/annotation_undo_button.PNG
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-06-27 15:46:54.000000 hesperos-0.2.1/materials/interface_tools_screenshots/annotation_unlock_button.PNG
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-06-27 15:46:54.000000 hesperos-0.2.1/materials/interface_tools_screenshots/contrast_add_button.PNG
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-06-27 15:46:54.000000 hesperos-0.2.1/materials/interface_tools_screenshots/contrast_choose.PNG
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-06-27 15:46:54.000000 hesperos-0.2.1/materials/interface_tools_screenshots/contrast_export_button.PNG
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-06-27 15:46:54.000000 hesperos-0.2.1/materials/interface_tools_screenshots/contrast_import_button.PNG
+-rw-r--r--   0 runner    (1001) docker     (123)   454140 2023-06-27 15:46:54.000000 hesperos-0.2.1/materials/interface_tools_screenshots/hesperos_manual_interface.PNG
+-rw-r--r--   0 runner    (1001) docker     (123)   510686 2023-06-27 15:46:54.000000 hesperos-0.2.1/materials/interface_tools_screenshots/hesperos_oneshot_interface.PNG
+-rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-06-27 15:46:54.000000 hesperos-0.2.1/materials/interface_tools_screenshots/image_change_axis_button.PNG
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-06-27 15:46:54.000000 hesperos-0.2.1/materials/interface_tools_screenshots/image_transpose_button.PNG
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-06-27 15:46:54.000000 hesperos-0.2.1/materials/interface_tools_screenshots/layer_label_erase_button.PNG
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-06-27 15:46:54.000000 hesperos-0.2.1/materials/interface_tools_screenshots/layer_label_fill_button.PNG
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-06-27 15:46:54.000000 hesperos-0.2.1/materials/interface_tools_screenshots/layer_label_paint_button.PNG
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-06-27 15:46:54.000000 hesperos-0.2.1/materials/interface_tools_screenshots/layer_label_zoom_button.PNG
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-06-27 15:46:54.000000 hesperos-0.2.1/materials/interface_tools_screenshots/open_dicom_serie_button.PNG
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-06-27 15:46:54.000000 hesperos-0.2.1/materials/interface_tools_screenshots/open_image_file_button.PNG
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-06-27 15:46:54.000000 hesperos-0.2.1/materials/interface_tools_screenshots/proba_threshold_slider.PNG
+-rw-r--r--   0 runner    (1001) docker     (123)      905 2023-06-27 15:46:54.000000 hesperos-0.2.1/materials/interface_tools_screenshots/run_segmentation_button.PNG
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-06-27 15:46:54.000000 hesperos-0.2.1/materials/interface_tools_screenshots/save_probabilities_button.PNG
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-06-27 15:46:54.000000 hesperos-0.2.1/materials/interface_tools_screenshots/save_segmentation_button.PNG
+-rw-r--r--   0 runner    (1001) docker     (123)   301806 2023-06-27 15:46:54.000000 hesperos-0.2.1/materials/interface_tools_screenshots/screen_tagging_step.PNG
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-06-27 15:46:54.000000 hesperos-0.2.1/materials/interface_tools_screenshots/slice_selection_add_button.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-06-27 15:46:54.000000 hesperos-0.2.1/materials/interface_tools_screenshots/slice_selection_drop_down_menu.png
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-06-27 15:46:54.000000 hesperos-0.2.1/materials/interface_tools_screenshots/slice_selection_goto_button.png
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-27 15:46:54.000000 hesperos-0.2.1/materials/interface_tools_screenshots/slice_selection_remove_button.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-06-27 15:46:54.000000 hesperos-0.2.1/materials/interface_tools_screenshots/zoom_slider.PNG
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-06-27 15:46:54.000000 hesperos-0.2.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 15:47:32.872043 hesperos-0.2.1/script_files/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 15:47:32.880044 hesperos-0.2.1/script_files/for_Macos/
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-06-27 15:46:54.000000 hesperos-0.2.1/script_files/for_Macos/install_hesperos_env.command
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-27 15:46:54.000000 hesperos-0.2.1/script_files/for_Macos/run_hesperos.command
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 15:47:32.880044 hesperos-0.2.1/script_files/for_Windows/
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-06-27 15:46:54.000000 hesperos-0.2.1/script_files/for_Windows/install_hesperos_env.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-27 15:46:54.000000 hesperos-0.2.1/script_files/for_Windows/run_hesperos.bat
+-rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-06-27 15:47:32.892045 hesperos-0.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 15:47:32.880044 hesperos-0.2.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 15:47:32.884044 hesperos-0.2.1/src/_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 15:46:54.000000 hesperos-0.2.1/src/_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-06-27 15:46:54.000000 hesperos-0.2.1/src/_tests/test_widget.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 15:47:32.884044 hesperos-0.2.1/src/hesperos/
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-27 15:46:54.000000 hesperos-0.2.1/src/hesperos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   118492 2023-06-27 15:46:54.000000 hesperos-0.2.1/src/hesperos/_manual_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44800 2023-06-27 15:46:54.000000 hesperos-0.2.1/src/hesperos/_oneshot_widget.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 15:47:32.884044 hesperos-0.2.1/src/hesperos/annotation/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-27 15:46:54.000000 hesperos-0.2.1/src/hesperos/annotation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-06-27 15:46:54.000000 hesperos-0.2.1/src/hesperos/annotation/feta.py
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-06-27 15:46:54.000000 hesperos-0.2.1/src/hesperos/annotation/fetus.py
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-06-27 15:46:54.000000 hesperos-0.2.1/src/hesperos/annotation/larva.py
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-06-27 15:46:54.000000 hesperos-0.2.1/src/hesperos/annotation/mouse_embryon.py
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-06-27 15:46:54.000000 hesperos-0.2.1/src/hesperos/annotation/oneshot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-06-27 15:46:54.000000 hesperos-0.2.1/src/hesperos/annotation/shoulder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-06-27 15:46:54.000000 hesperos-0.2.1/src/hesperos/annotation/shoulder_bone_border.py
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-06-27 15:46:54.000000 hesperos-0.2.1/src/hesperos/annotation/shoulder_bones.py
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-06-27 15:46:54.000000 hesperos-0.2.1/src/hesperos/annotation/shoulder_deltoid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5206 2023-06-27 15:46:54.000000 hesperos-0.2.1/src/hesperos/annotation/structuresubpanel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 15:47:32.884044 hesperos-0.2.1/src/hesperos/layout/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-27 15:46:54.000000 hesperos-0.2.1/src/hesperos/layout/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22740 2023-06-27 15:46:54.000000 hesperos-0.2.1/src/hesperos/layout/gui_elements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7879 2023-06-27 15:46:54.000000 hesperos-0.2.1/src/hesperos/layout/napari_elements.py
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-06-27 15:46:54.000000 hesperos-0.2.1/src/hesperos/napari.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 15:47:32.888044 hesperos-0.2.1/src/hesperos/one_shot_learning/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-27 15:46:54.000000 hesperos-0.2.1/src/hesperos/one_shot_learning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4094 2023-06-27 15:46:54.000000 hesperos-0.2.1/src/hesperos/one_shot_learning/classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10693 2023-06-27 15:46:54.000000 hesperos-0.2.1/src/hesperos/one_shot_learning/features2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-06-27 15:46:54.000000 hesperos-0.2.1/src/hesperos/one_shot_learning/features3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-06-27 15:46:54.000000 hesperos-0.2.1/src/hesperos/one_shot_learning/kernel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5547 2023-06-27 15:46:54.000000 hesperos-0.2.1/src/hesperos/one_shot_learning/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 15:47:32.888044 hesperos-0.2.1/src/hesperos/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-27 15:46:54.000000 hesperos-0.2.1/src/hesperos/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-06-27 15:46:54.000000 hesperos-0.2.1/src/hesperos/resources/_icons.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-06-27 15:46:54.000000 hesperos-0.2.1/src/hesperos/resources/group_box_stylesheet.qss
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 15:47:32.892045 hesperos-0.2.1/src/hesperos/resources/icons/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-27 15:46:54.000000 hesperos-0.2.1/src/hesperos/resources/icons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-06-27 15:46:54.000000 hesperos-0.2.1/src/hesperos/resources/icons/back.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-06-27 15:46:54.000000 hesperos-0.2.1/src/hesperos/resources/icons/backup.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-06-27 15:46:54.000000 hesperos-0.2.1/src/hesperos/resources/icons/chevron_down.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-06-27 15:46:54.000000 hesperos-0.2.1/src/hesperos/resources/icons/chevron_left.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-06-27 15:46:54.000000 hesperos-0.2.1/src/hesperos/resources/icons/chevron_right.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-06-27 15:46:54.000000 hesperos-0.2.1/src/hesperos/resources/icons/chevron_up.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-06-27 15:46:54.000000 hesperos-0.2.1/src/hesperos/resources/icons/export.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-06-27 15:46:54.000000 hesperos-0.2.1/src/hesperos/resources/icons/import.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-06-27 15:46:54.000000 hesperos-0.2.1/src/hesperos/resources/icons/lock.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-06-27 15:46:54.000000 hesperos-0.2.1/src/hesperos/resources/icons/map.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-06-27 15:46:54.000000 hesperos-0.2.1/src/hesperos/resources/icons/minus.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-06-27 15:46:54.000000 hesperos-0.2.1/src/hesperos/resources/icons/minus2.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-06-27 15:46:54.000000 hesperos-0.2.1/src/hesperos/resources/icons/next.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-06-27 15:46:54.000000 hesperos-0.2.1/src/hesperos/resources/icons/plus.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-06-27 15:46:54.000000 hesperos-0.2.1/src/hesperos/resources/icons/reset.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-06-27 15:46:54.000000 hesperos-0.2.1/src/hesperos/resources/icons/save.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-06-27 15:46:54.000000 hesperos-0.2.1/src/hesperos/resources/icons/undo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-06-27 15:46:54.000000 hesperos-0.2.1/src/hesperos/resources/icons/unlock.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-06-27 15:46:54.000000 hesperos-0.2.1/src/hesperos/resources/icons/zoom.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 15:47:32.884044 hesperos-0.2.1/src/hesperos.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    24226 2023-06-27 15:47:32.000000 hesperos-0.2.1/src/hesperos.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4541 2023-06-27 15:47:32.000000 hesperos-0.2.1/src/hesperos.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 15:47:32.000000 hesperos-0.2.1/src/hesperos.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-27 15:47:32.000000 hesperos-0.2.1/src/hesperos.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-06-27 15:47:32.000000 hesperos-0.2.1/src/hesperos.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-27 15:47:32.000000 hesperos-0.2.1/src/hesperos.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-06-27 15:46:54.000000 hesperos-0.2.1/src/test_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-06-27 15:46:54.000000 hesperos-0.2.1/tox.ini
```

### Comparing `hesperos-0.2/.github/workflows/plugin_preview.yml` & `hesperos-0.2.1/.github/workflows/plugin_preview.yml`

 * *Files identical despite different names*

### Comparing `hesperos-0.2/.github/workflows/test_and_deploy.yml` & `hesperos-0.2.1/.github/workflows/test_and_deploy.yml`

 * *Files identical despite different names*

### Comparing `hesperos-0.2/.gitignore` & `hesperos-0.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `hesperos-0.2/.napari/DESCRIPTION.md` & `hesperos-0.2.1/.napari/DESCRIPTION.md`

 * *Files identical despite different names*

### Comparing `hesperos-0.2/.pre-commit-config.yaml` & `hesperos-0.2.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `hesperos-0.2/LICENSE` & `hesperos-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hesperos-0.2/PKG-INFO` & `hesperos-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hesperos
-Version: 0.2
+Version: 0.2.1
 Summary: A plugin to manually or semi-automatically segment medical data and correct previous segmentation data.
 Home-page: https://github.com/chgodard/hesperos
 Author: Charlotte Godard
 Author-email: charlotte.godard@pasteur.fr
 License: BSD-3-Clause
 Project-URL: Documentation, https://github.com/chgodard/hesperos/blob/main/README.md
 Project-URL: Source Code, https://github.com/chgodard/hesperos
```

### Comparing `hesperos-0.2/README.md` & `hesperos-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `hesperos-0.2/materials/interface_tools_screenshots/annotation_delete_button.PNG` & `hesperos-0.2.1/materials/interface_tools_screenshots/annotation_delete_button.PNG`

 * *Files identical despite different names*

### Comparing `hesperos-0.2/materials/interface_tools_screenshots/annotation_export_button.png` & `hesperos-0.2.1/materials/interface_tools_screenshots/annotation_export_button.png`

 * *Files identical despite different names*

### Comparing `hesperos-0.2/materials/interface_tools_screenshots/annotation_load_button.PNG` & `hesperos-0.2.1/materials/interface_tools_screenshots/annotation_load_button.PNG`

 * *Files identical despite different names*

### Comparing `hesperos-0.2/materials/interface_tools_screenshots/annotation_lock_button.PNG` & `hesperos-0.2.1/materials/interface_tools_screenshots/annotation_lock_button.PNG`

 * *Files identical despite different names*

### Comparing `hesperos-0.2/materials/interface_tools_screenshots/annotation_save_button.PNG` & `hesperos-0.2.1/materials/interface_tools_screenshots/annotation_save_button.PNG`

 * *Files identical despite different names*

### Comparing `hesperos-0.2/materials/interface_tools_screenshots/annotation_undo_button.PNG` & `hesperos-0.2.1/materials/interface_tools_screenshots/annotation_undo_button.PNG`

 * *Files identical despite different names*

### Comparing `hesperos-0.2/materials/interface_tools_screenshots/annotation_unlock_button.PNG` & `hesperos-0.2.1/materials/interface_tools_screenshots/annotation_unlock_button.PNG`

 * *Files identical despite different names*

### Comparing `hesperos-0.2/materials/interface_tools_screenshots/contrast_choose.PNG` & `hesperos-0.2.1/materials/interface_tools_screenshots/contrast_choose.PNG`

 * *Files identical despite different names*

### Comparing `hesperos-0.2/materials/interface_tools_screenshots/contrast_export_button.PNG` & `hesperos-0.2.1/materials/interface_tools_screenshots/contrast_export_button.PNG`

 * *Files identical despite different names*

### Comparing `hesperos-0.2/materials/interface_tools_screenshots/contrast_import_button.PNG` & `hesperos-0.2.1/materials/interface_tools_screenshots/contrast_import_button.PNG`

 * *Files identical despite different names*

### Comparing `hesperos-0.2/materials/interface_tools_screenshots/hesperos_manual_interface.PNG` & `hesperos-0.2.1/materials/interface_tools_screenshots/hesperos_manual_interface.PNG`

 * *Files identical despite different names*

### Comparing `hesperos-0.2/materials/interface_tools_screenshots/hesperos_oneshot_interface.PNG` & `hesperos-0.2.1/materials/interface_tools_screenshots/hesperos_oneshot_interface.PNG`

 * *Files identical despite different names*

### Comparing `hesperos-0.2/materials/interface_tools_screenshots/image_change_axis_button.PNG` & `hesperos-0.2.1/materials/interface_tools_screenshots/image_change_axis_button.PNG`

 * *Files identical despite different names*

### Comparing `hesperos-0.2/materials/interface_tools_screenshots/image_transpose_button.PNG` & `hesperos-0.2.1/materials/interface_tools_screenshots/image_transpose_button.PNG`

 * *Files identical despite different names*

### Comparing `hesperos-0.2/materials/interface_tools_screenshots/layer_label_erase_button.PNG` & `hesperos-0.2.1/materials/interface_tools_screenshots/layer_label_erase_button.PNG`

 * *Files identical despite different names*

### Comparing `hesperos-0.2/materials/interface_tools_screenshots/layer_label_fill_button.PNG` & `hesperos-0.2.1/materials/interface_tools_screenshots/layer_label_fill_button.PNG`

 * *Files identical despite different names*

### Comparing `hesperos-0.2/materials/interface_tools_screenshots/layer_label_paint_button.PNG` & `hesperos-0.2.1/materials/interface_tools_screenshots/layer_label_paint_button.PNG`

 * *Files identical despite different names*

### Comparing `hesperos-0.2/materials/interface_tools_screenshots/layer_label_zoom_button.PNG` & `hesperos-0.2.1/materials/interface_tools_screenshots/layer_label_zoom_button.PNG`

 * *Files identical despite different names*

### Comparing `hesperos-0.2/materials/interface_tools_screenshots/open_dicom_serie_button.PNG` & `hesperos-0.2.1/materials/interface_tools_screenshots/open_dicom_serie_button.PNG`

 * *Files identical despite different names*

### Comparing `hesperos-0.2/materials/interface_tools_screenshots/open_image_file_button.PNG` & `hesperos-0.2.1/materials/interface_tools_screenshots/open_image_file_button.PNG`

 * *Files identical despite different names*

### Comparing `hesperos-0.2/materials/interface_tools_screenshots/proba_threshold_slider.PNG` & `hesperos-0.2.1/materials/interface_tools_screenshots/proba_threshold_slider.PNG`

 * *Files identical despite different names*

### Comparing `hesperos-0.2/materials/interface_tools_screenshots/run_segmentation_button.PNG` & `hesperos-0.2.1/materials/interface_tools_screenshots/run_segmentation_button.PNG`

 * *Files identical despite different names*

### Comparing `hesperos-0.2/materials/interface_tools_screenshots/save_probabilities_button.PNG` & `hesperos-0.2.1/materials/interface_tools_screenshots/save_probabilities_button.PNG`

 * *Files identical despite different names*

### Comparing `hesperos-0.2/materials/interface_tools_screenshots/save_segmentation_button.PNG` & `hesperos-0.2.1/materials/interface_tools_screenshots/save_segmentation_button.PNG`

 * *Files identical despite different names*

### Comparing `hesperos-0.2/materials/interface_tools_screenshots/screen_tagging_step.PNG` & `hesperos-0.2.1/materials/interface_tools_screenshots/screen_tagging_step.PNG`

 * *Files identical despite different names*

### Comparing `hesperos-0.2/materials/interface_tools_screenshots/slice_selection_drop_down_menu.png` & `hesperos-0.2.1/materials/interface_tools_screenshots/slice_selection_drop_down_menu.png`

 * *Files identical despite different names*

### Comparing `hesperos-0.2/materials/interface_tools_screenshots/slice_selection_goto_button.png` & `hesperos-0.2.1/materials/interface_tools_screenshots/slice_selection_goto_button.png`

 * *Files identical despite different names*

### Comparing `hesperos-0.2/materials/interface_tools_screenshots/zoom_slider.PNG` & `hesperos-0.2.1/materials/interface_tools_screenshots/zoom_slider.PNG`

 * *Files identical despite different names*

### Comparing `hesperos-0.2/setup.cfg` & `hesperos-0.2.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = hesperos
-version = 0.2
+version = 0.2.1
 author = Charlotte Godard
 author_email = charlotte.godard@pasteur.fr
 url = https://github.com/chgodard/hesperos
 license = BSD-3-Clause
 description = A plugin to manually or semi-automatically segment medical data and correct previous segmentation data.
 long_description = file: README.md
 long_description_content_type = text/markdown
```

### Comparing `hesperos-0.2/src/_tests/test_widget.py` & `hesperos-0.2.1/src/_tests/test_widget.py`

 * *Files identical despite different names*

### Comparing `hesperos-0.2/src/hesperos/_manual_widget.py` & `hesperos-0.2.1/src/hesperos/_manual_widget.py`

 * *Files 1% similar despite different names*

```diff
@@ -1271,20 +1271,30 @@
         segmentation_sitk : SimpleITK image
             segmentation data in sitk format
 
         """
         try:
             description = json.loads(segmentation_sitk.GetMetaData('ImageDescription'))
             loaded_selected_slice_list = description['Hesperos_SelectedSlices']
-            # loaded_selected_slice_list = json.load(description['Hesperos_SelectedSlices'])
+            if loaded_selected_slice_list[0] == '[':
+                is_old_version = True
+                loaded_selected_slice_list = json.loads(description['Hesperos_SelectedSlices'])
+            else:
+                is_old_version = False
         except:
             return
         if loaded_selected_slice_list != []:
             if loaded_selected_slice_list != "[]":
-                self.selected_slice_list = loaded_selected_slice_list
+                # in old version : only the index number was saved : ['100x', '102y']
+                if is_old_version :
+                    self.selected_slice_list = [str(index) + 'z' for index in loaded_selected_slice_list]
+                else:
+                    self.selected_slice_list = loaded_selected_slice_list
+                    
+                # in new version the index number and the axe are saved as string  : "[136, 170, 255]"
                 self.selected_slice_list.sort(key=lambda text: int(text[:-1]))
 
                 for slice_index in self.selected_slice_list:
                     new_text = str(slice_index)
                     self.selected_slice_combo_box.addItem(new_text)
```

### Comparing `hesperos-0.2/src/hesperos/_oneshot_widget.py` & `hesperos-0.2.1/src/hesperos/_oneshot_widget.py`

 * *Files identical despite different names*

### Comparing `hesperos-0.2/src/hesperos/annotation/mouse_embryon.py` & `hesperos-0.2.1/src/hesperos/annotation/mouse_embryon.py`

 * *Files identical despite different names*

### Comparing `hesperos-0.2/src/hesperos/annotation/shoulder.py` & `hesperos-0.2.1/src/hesperos/annotation/shoulder.py`

 * *Files identical despite different names*

### Comparing `hesperos-0.2/src/hesperos/annotation/shoulder_bones.py` & `hesperos-0.2.1/src/hesperos/annotation/shoulder_bones.py`

 * *Files identical despite different names*

### Comparing `hesperos-0.2/src/hesperos/annotation/structuresubpanel.py` & `hesperos-0.2.1/src/hesperos/annotation/structuresubpanel.py`

 * *Files identical despite different names*

### Comparing `hesperos-0.2/src/hesperos/layout/gui_elements.py` & `hesperos-0.2.1/src/hesperos/layout/gui_elements.py`

 * *Files identical despite different names*

### Comparing `hesperos-0.2/src/hesperos/layout/napari_elements.py` & `hesperos-0.2.1/src/hesperos/layout/napari_elements.py`

 * *Files identical despite different names*

### Comparing `hesperos-0.2/src/hesperos/napari.yaml` & `hesperos-0.2.1/src/hesperos/napari.yaml`

 * *Files identical despite different names*

### Comparing `hesperos-0.2/src/hesperos/one_shot_learning/classifier.py` & `hesperos-0.2.1/src/hesperos/one_shot_learning/classifier.py`

 * *Files identical despite different names*

### Comparing `hesperos-0.2/src/hesperos/one_shot_learning/features2d.py` & `hesperos-0.2.1/src/hesperos/one_shot_learning/features2d.py`

 * *Files identical despite different names*

### Comparing `hesperos-0.2/src/hesperos/one_shot_learning/features3d.py` & `hesperos-0.2.1/src/hesperos/one_shot_learning/features3d.py`

 * *Files identical despite different names*

### Comparing `hesperos-0.2/src/hesperos/one_shot_learning/kernel.py` & `hesperos-0.2.1/src/hesperos/one_shot_learning/kernel.py`

 * *Files identical despite different names*

### Comparing `hesperos-0.2/src/hesperos/one_shot_learning/utilities.py` & `hesperos-0.2.1/src/hesperos/one_shot_learning/utilities.py`

 * *Files identical despite different names*

### Comparing `hesperos-0.2/src/hesperos/resources/_icons.py` & `hesperos-0.2.1/src/hesperos/resources/_icons.py`

 * *Files identical despite different names*

### Comparing `hesperos-0.2/src/hesperos/resources/icons/back.svg` & `hesperos-0.2.1/src/hesperos/resources/icons/back.svg`

 * *Files identical despite different names*

### Comparing `hesperos-0.2/src/hesperos/resources/icons/backup.svg` & `hesperos-0.2.1/src/hesperos/resources/icons/backup.svg`

 * *Files identical despite different names*

### Comparing `hesperos-0.2/src/hesperos/resources/icons/chevron_down.svg` & `hesperos-0.2.1/src/hesperos/resources/icons/chevron_down.svg`

 * *Files identical despite different names*

### Comparing `hesperos-0.2/src/hesperos/resources/icons/chevron_left.svg` & `hesperos-0.2.1/src/hesperos/resources/icons/chevron_left.svg`

 * *Files identical despite different names*

### Comparing `hesperos-0.2/src/hesperos/resources/icons/chevron_right.svg` & `hesperos-0.2.1/src/hesperos/resources/icons/chevron_right.svg`

 * *Files identical despite different names*

### Comparing `hesperos-0.2/src/hesperos/resources/icons/chevron_up.svg` & `hesperos-0.2.1/src/hesperos/resources/icons/chevron_up.svg`

 * *Files identical despite different names*

### Comparing `hesperos-0.2/src/hesperos/resources/icons/export.svg` & `hesperos-0.2.1/src/hesperos/resources/icons/export.svg`

 * *Files identical despite different names*

### Comparing `hesperos-0.2/src/hesperos/resources/icons/import.svg` & `hesperos-0.2.1/src/hesperos/resources/icons/import.svg`

 * *Files identical despite different names*

### Comparing `hesperos-0.2/src/hesperos/resources/icons/lock.svg` & `hesperos-0.2.1/src/hesperos/resources/icons/lock.svg`

 * *Files identical despite different names*

### Comparing `hesperos-0.2/src/hesperos/resources/icons/map.svg` & `hesperos-0.2.1/src/hesperos/resources/icons/map.svg`

 * *Files identical despite different names*

### Comparing `hesperos-0.2/src/hesperos/resources/icons/minus.svg` & `hesperos-0.2.1/src/hesperos/resources/icons/minus.svg`

 * *Files identical despite different names*

### Comparing `hesperos-0.2/src/hesperos/resources/icons/minus2.svg` & `hesperos-0.2.1/src/hesperos/resources/icons/minus2.svg`

 * *Files identical despite different names*

### Comparing `hesperos-0.2/src/hesperos/resources/icons/next.svg` & `hesperos-0.2.1/src/hesperos/resources/icons/next.svg`

 * *Files identical despite different names*

### Comparing `hesperos-0.2/src/hesperos/resources/icons/plus.svg` & `hesperos-0.2.1/src/hesperos/resources/icons/plus.svg`

 * *Files identical despite different names*

### Comparing `hesperos-0.2/src/hesperos/resources/icons/reset.svg` & `hesperos-0.2.1/src/hesperos/resources/icons/reset.svg`

 * *Files identical despite different names*

### Comparing `hesperos-0.2/src/hesperos/resources/icons/save.svg` & `hesperos-0.2.1/src/hesperos/resources/icons/save.svg`

 * *Files identical despite different names*

### Comparing `hesperos-0.2/src/hesperos/resources/icons/undo.svg` & `hesperos-0.2.1/src/hesperos/resources/icons/undo.svg`

 * *Files identical despite different names*

### Comparing `hesperos-0.2/src/hesperos/resources/icons/unlock.svg` & `hesperos-0.2.1/src/hesperos/resources/icons/unlock.svg`

 * *Files identical despite different names*

### Comparing `hesperos-0.2/src/hesperos/resources/icons/zoom.svg` & `hesperos-0.2.1/src/hesperos/resources/icons/zoom.svg`

 * *Files identical despite different names*

### Comparing `hesperos-0.2/src/hesperos.egg-info/PKG-INFO` & `hesperos-0.2.1/src/hesperos.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hesperos
-Version: 0.2
+Version: 0.2.1
 Summary: A plugin to manually or semi-automatically segment medical data and correct previous segmentation data.
 Home-page: https://github.com/chgodard/hesperos
 Author: Charlotte Godard
 Author-email: charlotte.godard@pasteur.fr
 License: BSD-3-Clause
 Project-URL: Documentation, https://github.com/chgodard/hesperos/blob/main/README.md
 Project-URL: Source Code, https://github.com/chgodard/hesperos
```

### Comparing `hesperos-0.2/src/hesperos.egg-info/SOURCES.txt` & `hesperos-0.2.1/src/hesperos.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hesperos-0.2/tox.ini` & `hesperos-0.2.1/tox.ini`

 * *Files identical despite different names*

