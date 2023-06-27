# Comparing `tmp/apf-ci-1.2.180.tar.gz` & `tmp/apf-ci-1.2.180.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apf-ci-1.2.180.tar", last modified: Tue Jun 27 07:05:04 2023, max compression
+gzip compressed data, was "apf-ci-1.2.180.1.tar", last modified: Tue Jun 27 07:11:19 2023, max compression
```

## Comparing `apf-ci-1.2.180.tar` & `apf-ci-1.2.180.1.tar`

### file list

```diff
@@ -1,332 +1,332 @@
-drwxrwxrwx   0        0        0        0 2023-06-27 07:05:04.079334 apf-ci-1.2.180/
--rw-rw-rw-   0        0        0     2533 2023-06-27 07:05:04.079334 apf-ci-1.2.180/PKG-INFO
--rw-rw-rw-   0        0        0     1268 2023-06-07 15:36:10.000000 apf-ci-1.2.180/README.md
-drwxrwxrwx   0        0        0        0 2023-06-27 07:05:03.857780 apf-ci-1.2.180/apf_ci/
--rw-rw-rw-   0        0        0      652 2023-06-27 07:04:23.000000 apf-ci-1.2.180/apf_ci/__init__.py
--rw-rw-rw-   0        0        0      425 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/__main__.py
-drwxrwxrwx   0        0        0        0 2023-06-27 07:05:03.871498 apf-ci-1.2.180/apf_ci/android/
--rw-rw-rw-   0        0        0        0 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/android/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-27 07:05:03.871498 apf-ci-1.2.180/apf_ci/android/build_prepare/
--rw-rw-rw-   0        0        0        0 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/android/build_prepare/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-27 07:05:03.881135 apf-ci-1.2.180/apf_ci/android/build_prepare/builder/
--rw-rw-rw-   0        0        0        0 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/android/build_prepare/builder/__init__.py
--rw-rw-rw-   0        0        0    20753 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/android/build_prepare/builder/android_build_prepare_builder.py
--rw-rw-rw-   0        0        0    10180 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/android/build_prepare/builder/certificate_builder.py
--rw-rw-rw-   0        0        0     5535 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/android/build_prepare/builder/clean_config_file_builder.py
--rw-rw-rw-   0        0        0    10616 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/android/build_prepare/builder/config_info_sync.py
--rw-rw-rw-   0        0        0     7782 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/android/build_prepare/builder/local_properties_builder.py
--rw-rw-rw-   0        0        0     4434 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/android/build_prepare/builder/multi_channel_builder.py
--rw-rw-rw-   0        0        0     9242 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/android/build_prepare/builder/update_project_info_builder.py
-drwxrwxrwx   0        0        0        0 2023-06-27 07:05:03.881135 apf-ci-1.2.180/apf_ci/android/prepare/
--rw-rw-rw-   0        0        0        0 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/android/prepare/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-27 07:05:03.884690 apf-ci-1.2.180/apf_ci/android/prepare/builder/
--rw-rw-rw-   0        0        0        0 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/android/prepare/builder/__init__.py
--rw-rw-rw-   0        0        0     9313 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/android/prepare/builder/android_injections_builder.py
--rw-rw-rw-   0        0        0     1571 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/android/prepare/builder/android_prepare_builder.py
--rw-rw-rw-   0        0        0    19270 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/android/prepare/builder/generate_dependency_builder.py
-drwxrwxrwx   0        0        0        0 2023-06-27 07:05:03.885710 apf-ci-1.2.180/apf_ci/android/prepare/model/
--rw-rw-rw-   0        0        0        0 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/android/prepare/model/__init__.py
--rw-rw-rw-   0        0        0      516 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/android/prepare/model/meta_data_note.py
-drwxrwxrwx   0        0        0        0 2023-06-27 07:05:03.886692 apf-ci-1.2.180/apf_ci/app_compare/
--rw-rw-rw-   0        0        0        0 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/app_compare/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-27 07:05:03.893118 apf-ci-1.2.180/apf_ci/app_compare/build/
--rw-rw-rw-   0        0        0        0 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/app_compare/build/__init__.py
--rw-rw-rw-   0        0        0     1035 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/app_compare/build/apk_utils.py
--rw-rw-rw-   0        0        0     3013 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/app_compare/build/app_compare.py
--rw-rw-rw-   0        0        0     4371 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/app_compare/build/app_compare_android.py
--rw-rw-rw-   0        0        0     4452 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/app_compare/build/app_compare_ios.py
--rw-rw-rw-   0        0        0     6139 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/app_compare/build/app_compare_utils.py
--rw-rw-rw-   0        0        0     5428 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/app_compare/build/dependency_utils.py
--rw-rw-rw-   0        0        0     2162 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/app_compare/build/test_app_compare.py
-drwxrwxrwx   0        0        0        0 2023-06-27 07:05:03.893693 apf-ci-1.2.180/apf_ci/app_component_compare/
--rw-rw-rw-   0        0        0        0 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/app_component_compare/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-27 07:05:03.895699 apf-ci-1.2.180/apf_ci/app_component_compare/build/
--rw-rw-rw-   0        0        0        0 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/app_component_compare/build/__init__.py
--rw-rw-rw-   0        0        0    12815 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/app_component_compare/build/app_component_compare.py
--rw-rw-rw-   0        0        0     1270 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/app_component_compare/build/test_app_component_compare.py
-drwxrwxrwx   0        0        0        0 2023-06-27 07:05:03.900698 apf-ci-1.2.180/apf_ci/app_init/
--rw-rw-rw-   0        0        0        0 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/app_init/__init__.py
--rw-rw-rw-   0        0        0    10701 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/app_init/app_config.py
--rw-rw-rw-   0        0        0     6117 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/app_init/app_init.py
--rw-rw-rw-   0        0        0     5011 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/app_init/app_resource.py
--rw-rw-rw-   0        0        0      969 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/app_init/test_after_app_init.py
--rw-rw-rw-   0        0        0     3212 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/app_init/test_app_init.py
--rw-rw-rw-   0        0        0    14399 2023-06-27 04:16:12.000000 apf-ci-1.2.180/apf_ci/app_init/update_variable_json.py
-drwxrwxrwx   0        0        0        0 2023-06-27 07:05:03.912721 apf-ci-1.2.180/apf_ci/app_init/utils/
--rw-rw-rw-   0        0        0      255 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/app_init/utils/__init__.py
--rw-rw-rw-   0        0        0     1141 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/app_init/utils/appinfo_utils.py
--rw-rw-rw-   0        0        0     1454 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/app_init/utils/apps_utils.py
--rw-rw-rw-   0        0        0    10365 2023-06-27 03:14:12.000000 apf-ci-1.2.180/apf_ci/app_init/utils/build_config_utils.py
--rw-rw-rw-   0        0        0     7510 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/app_init/utils/image_utils.py
--rw-rw-rw-   0        0        0     1710 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/app_init/utils/js_third_app_utils.py
--rw-rw-rw-   0        0        0     2607 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/app_init/utils/key_chain_utils.py
--rw-rw-rw-   0        0        0    37443 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/app_init/utils/language_utils.py
--rw-rw-rw-   0        0        0    15803 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/app_init/utils/variable_utils.py
--rw-rw-rw-   0        0        0      566 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/app_init/utils/variables_script_utils.py
-drwxrwxrwx   0        0        0        0 2023-06-27 07:05:03.918221 apf-ci-1.2.180/apf_ci/app_res/
--rw-rw-rw-   0        0        0        0 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/app_res/__init__.py
--rw-rw-rw-   0        0        0     1146 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/app_res/android_plugin.py
--rw-rw-rw-   0        0        0     2064 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/app_res/app_res.py
--rw-rw-rw-   0        0        0    10178 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/app_res/language_res.py
--rw-rw-rw-   0        0        0     5878 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/app_res/skin_res.py
--rw-rw-rw-   0        0        0     3118 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/app_res/test_skin_res.py
--rw-rw-rw-   0        0        0      833 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/cli.py
-drwxrwxrwx   0        0        0        0 2023-06-27 07:05:03.933989 apf-ci-1.2.180/apf_ci/commands/
--rw-rw-rw-   0        0        0        0 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/commands/__init__.py
--rw-rw-rw-   0        0        0      936 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/commands/android_build_prepare.py
--rw-rw-rw-   0        0        0      949 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/commands/android_prepare.py
--rw-rw-rw-   0        0        0     1413 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/commands/app_compare.py
--rw-rw-rw-   0        0        0     1563 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/commands/app_component_compare.py
--rw-rw-rw-   0        0        0     2482 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/commands/app_init.py
--rw-rw-rw-   0        0        0      426 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/commands/command_const.py
--rw-rw-rw-   0        0        0      695 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/commands/flutter.py
--rw-rw-rw-   0        0        0     1138 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/commands/h5_grain.py
--rw-rw-rw-   0        0        0     2719 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/commands/h5_grain_config.py
--rw-rw-rw-   0        0        0     1481 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/commands/h5_widget_resource.py
--rw-rw-rw-   0        0        0      883 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/commands/local_h5.py
--rw-rw-rw-   0        0        0     1520 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/commands/react_widget_resource.py
--rw-rw-rw-   0        0        0     2380 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/commands/rn.py
--rw-rw-rw-   0        0        0     2520 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/commands/rn_widget.py
--rw-rw-rw-   0        0        0     2420 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/commands/subapp_config.py
--rw-rw-rw-   0        0        0     2108 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/commands/tab_build.py
--rw-rw-rw-   0        0        0     1771 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/commands/variable.py
-drwxrwxrwx   0        0        0        0 2023-06-27 07:05:03.945627 apf-ci-1.2.180/apf_ci/config/
--rw-rw-rw-   0        0        0        0 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/config/__init__.py
--rw-rw-rw-   0        0        0    49911 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/config/app_config.py
--rw-rw-rw-   0        0        0    13448 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/config/biz_comp_transform.py
--rw-rw-rw-   0        0        0    20248 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/config/defines.py
--rw-rw-rw-   0        0        0     7793 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/config/env_service.py
--rw-rw-rw-   0        0        0     1953 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/config/h5_widget_i18n_utils.py
--rw-rw-rw-   0        0        0     5387 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/config/json_property_analysis.py
--rw-rw-rw-   0        0        0     5567 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/config/language_service.py
--rw-rw-rw-   0        0        0     3329 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/config/lite_app.py
--rw-rw-rw-   0        0        0     3201 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/config/page_attributes.py
--rw-rw-rw-   0        0        0     4553 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/config/page_i18n_utils.py
--rw-rw-rw-   0        0        0    20218 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/config/properties_transform.py
--rw-rw-rw-   0        0        0    13095 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/config/runtime.py
-drwxrwxrwx   0        0        0        0 2023-06-27 07:05:03.946674 apf-ci-1.2.180/apf_ci/config/test/
--rw-rw-rw-   0        0        0        0 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/config/test/__init__.py
--rw-rw-rw-   0        0        0     1198 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/config/test/widget_tree_test.py
--rw-rw-rw-   0        0        0     4594 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/config/widget_i18n_utils.py
--rw-rw-rw-   0        0        0     8942 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/config/widget_tree.py
-drwxrwxrwx   0        0        0        0 2023-06-27 07:05:03.949625 apf-ci-1.2.180/apf_ci/constant/
--rw-rw-rw-   0        0        0        0 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/constant/__init__.py
--rw-rw-rw-   0        0        0      693 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/constant/constants.py
--rw-rw-rw-   0        0        0     1581 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/constant/path_constant.py
-drwxrwxrwx   0        0        0        0 2023-06-27 07:05:03.954131 apf-ci-1.2.180/apf_ci/flutter/
--rw-rw-rw-   0        0        0        0 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/flutter/__init__.py
--rw-rw-rw-   0        0        0    15963 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/flutter/flutter.py
--rw-rw-rw-   0        0        0    29413 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/flutter/flutter_android_build.py
--rw-rw-rw-   0        0        0     6505 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/flutter/flutter_build.py
--rw-rw-rw-   0        0        0     2791 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/flutter/flutter_command_utils.py
--rw-rw-rw-   0        0        0     2384 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/flutter/flutter_ios_build.py
-drwxrwxrwx   0        0        0        0 2023-06-27 07:05:03.958147 apf-ci-1.2.180/apf_ci/flutter/resource/
--rw-rw-rw-   0        0        0        0 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/flutter/resource/__init__.py
--rw-rw-rw-   0        0        0     7945 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/flutter/resource/flutter_language_resource.py
--rw-rw-rw-   0        0        0     1677 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/flutter/resource/flutter_resource.py
--rw-rw-rw-   0        0        0     4466 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/flutter/resource/flutter_skin_resource.py
-drwxrwxrwx   0        0        0        0 2023-06-27 07:05:03.961197 apf-ci-1.2.180/apf_ci/h5_grain/
--rw-rw-rw-   0        0        0        0 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/h5_grain/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-27 07:05:03.967717 apf-ci-1.2.180/apf_ci/h5_grain/builder/
--rw-rw-rw-   0        0        0        0 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/h5_grain/builder/__init__.py
--rw-rw-rw-   0        0        0    12969 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/h5_grain/builder/analysis_pages_builder.py
--rw-rw-rw-   0        0        0     1192 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/h5_grain/builder/create_package_builder.py
--rw-rw-rw-   0        0        0     1586 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/h5_grain/builder/ensure_template_builder.py
--rw-rw-rw-   0        0        0     5892 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/h5_grain/builder/h5_grain_builder.py
--rw-rw-rw-   0        0        0    58946 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/h5_grain/builder/npm_operation_builder.py
--rw-rw-rw-   0        0        0     4275 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/h5_grain/builder/template_builder.py
--rw-rw-rw-   0        0        0      362 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/h5_grain/h5_page.py
--rw-rw-rw-   0        0        0      592 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/h5_grain/package_model.py
-drwxrwxrwx   0        0        0        0 2023-06-27 07:05:03.969705 apf-ci-1.2.180/apf_ci/h5_grain_config/
--rw-rw-rw-   0        0        0        0 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/h5_grain_config/__init__.py
--rw-rw-rw-   0        0        0     1812 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/h5_grain_config/h5_grain_config_test.py
--rw-rw-rw-   0        0        0     5028 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/h5_grain_config/h5_grain_init.py
-drwxrwxrwx   0        0        0        0 2023-06-27 07:05:03.969705 apf-ci-1.2.180/apf_ci/h5_widget_resource/
--rw-rw-rw-   0        0        0        0 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/h5_widget_resource/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-27 07:05:03.974025 apf-ci-1.2.180/apf_ci/h5_widget_resource/builder/
--rw-rw-rw-   0        0        0        0 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/h5_widget_resource/builder/__init__.py
--rw-rw-rw-   0        0        0     8017 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/h5_widget_resource/builder/create_package_builder.py
--rw-rw-rw-   0        0        0    10611 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/h5_widget_resource/builder/create_resource_builder.py
--rw-rw-rw-   0        0        0     2863 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/h5_widget_resource/builder/ensure_template_builder.py
--rw-rw-rw-   0        0        0     4504 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/h5_widget_resource/builder/h5_widget_resource_builder.py
-drwxrwxrwx   0        0        0        0 2023-06-27 07:05:03.977134 apf-ci-1.2.180/apf_ci/init/
--rw-rw-rw-   0        0        0        0 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/init/__init__.py
--rw-rw-rw-   0        0        0     7770 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/init/git_template_service.py
--rw-rw-rw-   0        0        0    29131 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/init/init_global_variable_service.py
--rw-rw-rw-   0        0        0     2221 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/init/validate_service.py
-drwxrwxrwx   0        0        0        0 2023-06-27 07:05:03.978043 apf-ci-1.2.180/apf_ci/lite_app/
--rw-rw-rw-   0        0        0        0 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/lite_app/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-27 07:05:03.987631 apf-ci-1.2.180/apf_ci/lite_app/cache/
--rw-rw-rw-   0        0        0        0 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/lite_app/cache/__init__.py
--rw-rw-rw-   0        0        0     1351 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/lite_app/cache/abstract_cache.py
--rw-rw-rw-   0        0        0     4771 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/lite_app/cache/abstract_first_level_cache.py
--rw-rw-rw-   0        0        0     3994 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/lite_app/cache/abstract_second_level_cache.py
--rw-rw-rw-   0        0        0     2736 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/lite_app/cache/abstract_three_level_cache.py
--rw-rw-rw-   0        0        0     1673 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/lite_app/cache/cache_factory.py
-drwxrwxrwx   0        0        0        0 2023-06-27 07:05:03.991138 apf-ci-1.2.180/apf_ci/lite_app/cache/factor/
--rw-rw-rw-   0        0        0        0 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/lite_app/cache/factor/__init__.py
--rw-rw-rw-   0        0        0     7153 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/lite_app/cache/factor/abstract_cache_factor.py
--rw-rw-rw-   0        0        0      117 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/lite_app/cache/factor/icache_factor.py
--rw-rw-rw-   0        0        0     4525 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/lite_app/cache/factor/local_h5_cache_factor.py
--rw-rw-rw-   0        0        0     5030 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/lite_app/cache/factor/react_cache_factor.py
--rw-rw-rw-   0        0        0      616 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/lite_app/cache/first_level_local_h5_cache.py
--rw-rw-rw-   0        0        0      888 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/lite_app/cache/first_level_react_cache.py
--rw-rw-rw-   0        0        0      541 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/lite_app/cache/icache.py
--rw-rw-rw-   0        0        0      742 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/lite_app/cache/second_level_local_h5_cache.py
--rw-rw-rw-   0        0        0      961 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/lite_app/cache/second_level_react_cache.py
--rw-rw-rw-   0        0        0     1095 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/lite_app/cache/three_level_local_h5_cache.py
--rw-rw-rw-   0        0        0     1504 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/lite_app/cache/three_level_react_cache.py
-drwxrwxrwx   0        0        0        0 2023-06-27 07:05:03.996164 apf-ci-1.2.180/apf_ci/lite_app/concurrent/
--rw-rw-rw-   0        0        0        0 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/lite_app/concurrent/__init__.py
--rw-rw-rw-   0        0        0     2077 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/lite_app/concurrent/concurrent_build_client.py
--rw-rw-rw-   0        0        0      350 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/lite_app/concurrent/local_h5_build_callable.py
--rw-rw-rw-   0        0        0      336 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/lite_app/concurrent/react_build_callable.py
-drwxrwxrwx   0        0        0        0 2023-06-27 07:05:03.999182 apf-ci-1.2.180/apf_ci/lite_app/lite_enum/
--rw-rw-rw-   0        0        0        0 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/lite_app/lite_enum/__init__.py
--rw-rw-rw-   0        0        0      429 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/lite_app/lite_enum/app_type_enum.py
--rw-rw-rw-   0        0        0      429 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/lite_app/lite_enum/cache_enum.py
--rw-rw-rw-   0        0        0      465 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/lite_app/lite_enum/component_type_enum.py
-drwxrwxrwx   0        0        0        0 2023-06-27 07:05:03.999182 apf-ci-1.2.180/apf_ci/lite_app/local_h5/
--rw-rw-rw-   0        0        0        0 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/lite_app/local_h5/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-27 07:05:04.000169 apf-ci-1.2.180/apf_ci/lite_app/local_h5/builder/
--rw-rw-rw-   0        0        0        0 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/lite_app/local_h5/builder/__init__.py
--rw-rw-rw-   0        0        0     4891 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/lite_app/local_h5/builder/local_h5_builder.py
-drwxrwxrwx   0        0        0        0 2023-06-27 07:05:04.004764 apf-ci-1.2.180/apf_ci/lite_app/model/
--rw-rw-rw-   0        0        0        0 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/lite_app/model/__init__.py
--rw-rw-rw-   0        0        0      835 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/lite_app/model/cache_bo.py
--rw-rw-rw-   0        0        0     1225 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/lite_app/model/cache_factor_bo.py
--rw-rw-rw-   0        0        0      520 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/lite_app/model/js_package_cache.py
--rw-rw-rw-   0        0        0     1002 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/lite_app/model/npm_dto.py
--rw-rw-rw-   0        0        0      394 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/lite_app/model/template_bo.py
-drwxrwxrwx   0        0        0        0 2023-06-27 07:05:04.006763 apf-ci-1.2.180/apf_ci/lite_app/parser/
--rw-rw-rw-   0        0        0        0 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/lite_app/parser/__init__.py
--rw-rw-rw-   0        0        0     3922 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/lite_app/parser/abstract_parser.py
--rw-rw-rw-   0        0        0      847 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/lite_app/parser/iparser.py
--rw-rw-rw-   0        0        0      982 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/lite_app/parser/local_h5_parser.py
--rw-rw-rw-   0        0        0     1319 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/lite_app/parser/react_parser.py
-drwxrwxrwx   0        0        0        0 2023-06-27 07:05:04.013783 apf-ci-1.2.180/apf_ci/lite_app/rn/
--rw-rw-rw-   0        0        0        0 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/lite_app/rn/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-27 07:05:04.014801 apf-ci-1.2.180/apf_ci/lite_app/rn/builder/
--rw-rw-rw-   0        0        0        0 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/lite_app/rn/builder/__init__.py
--rw-rw-rw-   0        0        0    23957 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/lite_app/rn/builder/react_builder.py
--rw-rw-rw-   0        0        0     4051 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/lite_app/rn/component.py
--rw-rw-rw-   0        0        0     7198 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/lite_app/rn/rn.py
--rw-rw-rw-   0        0        0      133 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/lite_app/rn/rn_init.py
--rw-rw-rw-   0        0        0     7705 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/lite_app/rn/template.py
--rw-rw-rw-   0        0        0     3532 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/lite_app/rn/terminal_interaction.py
-drwxrwxrwx   0        0        0        0 2023-06-27 07:05:04.017805 apf-ci-1.2.180/apf_ci/lite_app/service/
--rw-rw-rw-   0        0        0        0 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/lite_app/service/__init__.py
--rw-rw-rw-   0        0        0    11439 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/lite_app/service/apf_service.py
--rw-rw-rw-   0        0        0     6628 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/lite_app/service/config_service.py
--rw-rw-rw-   0        0        0    22272 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/lite_app/service/local_h5_service.py
--rw-rw-rw-   0        0        0    18712 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/lite_app/service/react_service.py
-drwxrwxrwx   0        0        0        0 2023-06-27 07:05:04.018805 apf-ci-1.2.180/apf_ci/react_widget_resource/
--rw-rw-rw-   0        0        0        0 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/react_widget_resource/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-27 07:05:04.023318 apf-ci-1.2.180/apf_ci/react_widget_resource/builder/
--rw-rw-rw-   0        0        0        0 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/react_widget_resource/builder/__init__.py
--rw-rw-rw-   0        0        0    21537 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/react_widget_resource/builder/create_resource_builder.py
--rw-rw-rw-   0        0        0     6765 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/react_widget_resource/builder/ensure_template_builder.py
--rw-rw-rw-   0        0        0     8095 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/react_widget_resource/builder/npm_builder.py
--rw-rw-rw-   0        0        0     7714 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/react_widget_resource/builder/react_widget_resource_builder.py
--rw-rw-rw-   0        0        0    12138 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/react_widget_resource/builder/rn_resource_analysis_pages_builder.py
-drwxrwxrwx   0        0        0        0 2023-06-27 07:05:04.026420 apf-ci-1.2.180/apf_ci/react_widget_resource/test/
--rw-rw-rw-   0        0        0        0 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/react_widget_resource/test/__init__.py
--rw-rw-rw-   0        0        0     2839 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/react_widget_resource/test/test_create_resource_builder.py
--rw-rw-rw-   0        0        0     1535 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/react_widget_resource/test/test_ensure_template_builder.py
--rw-rw-rw-   0        0        0     3608 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/react_widget_resource/test/test_npm_builder.py
--rw-rw-rw-   0        0        0     2925 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/react_widget_resource/test/test_rn_resource_analysis_pages_builder.py
-drwxrwxrwx   0        0        0        0 2023-06-27 07:05:04.029371 apf-ci-1.2.180/apf_ci/resource/
--rw-rw-rw-   0        0        0        0 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/resource/__init__.py
--rw-rw-rw-   0        0        0    10253 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/resource/cache_service.py
--rw-rw-rw-   0        0        0    12162 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/resource/language.py
--rw-rw-rw-   0        0        0    13045 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/resource/resource_builder.py
--rw-rw-rw-   0        0        0    10733 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/resource/skin.py
-drwxrwxrwx   0        0        0        0 2023-06-27 07:05:04.030343 apf-ci-1.2.180/apf_ci/resource/test/
--rw-rw-rw-   0        0        0        0 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/resource/test/__init__.py
--rw-rw-rw-   0        0        0      745 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/resource/test/test_resource_config.py
-drwxrwxrwx   0        0        0        0 2023-06-27 07:05:04.031352 apf-ci-1.2.180/apf_ci/rn_widget/
--rw-rw-rw-   0        0        0        0 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/rn_widget/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-27 07:05:04.037002 apf-ci-1.2.180/apf_ci/rn_widget/builder/
--rw-rw-rw-   0        0        0        0 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/rn_widget/builder/__init__.py
--rw-rw-rw-   0        0        0    18305 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/rn_widget/builder/analysis_pages_builder.py
--rw-rw-rw-   0        0        0     6383 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/rn_widget/builder/build_tool_builder.py
--rw-rw-rw-   0        0        0     2567 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/rn_widget/builder/check_env_name_builder.py
--rw-rw-rw-   0        0        0    18802 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/rn_widget/builder/multi_language_resource_builder.py
--rw-rw-rw-   0        0        0    55415 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/rn_widget/builder/npm_operation_builder.py
--rw-rw-rw-   0        0        0     6238 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/rn_widget/builder/react_widget_builder.py
--rw-rw-rw-   0        0        0     6861 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/rn_widget/builder/templater_builder.py
-drwxrwxrwx   0        0        0        0 2023-06-27 07:05:04.039006 apf-ci-1.2.180/apf_ci/rn_widget/model/
--rw-rw-rw-   0        0        0        0 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/rn_widget/model/__init__.py
--rw-rw-rw-   0        0        0      348 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/rn_widget/model/package_model.py
--rw-rw-rw-   0        0        0      420 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/rn_widget/model/page.py
--rw-rw-rw-   0        0        0      260 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/rn_widget/model/widget.py
--rw-rw-rw-   0        0        0     8427 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/rn_widget/rn_widget.py
-drwxrwxrwx   0        0        0        0 2023-06-27 07:05:04.041006 apf-ci-1.2.180/apf_ci/rn_widget/test/
--rw-rw-rw-   0        0        0       29 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/rn_widget/test/__init__.py
--rw-rw-rw-   0        0        0      777 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/rn_widget/test/rn_widget_build_test.py
--rw-rw-rw-   0        0        0     6868 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/rn_widget/test/test_multi_language_resource.py
--rw-rw-rw-   0        0        0    16704 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/rn_widget/widget.py
-drwxrwxrwx   0        0        0        0 2023-06-27 07:05:04.044683 apf-ci-1.2.180/apf_ci/subapp_config/
--rw-rw-rw-   0        0        0        0 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/subapp_config/__init__.py
--rw-rw-rw-   0        0        0     6582 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/subapp_config/subapp_config_init.py
-drwxrwxrwx   0        0        0        0 2023-06-27 07:05:04.045685 apf-ci-1.2.180/apf_ci/tab/
--rw-rw-rw-   0        0        0        0 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/tab/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-27 07:05:04.047705 apf-ci-1.2.180/apf_ci/tab/build/
--rw-rw-rw-   0        0        0        0 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/tab/build/__init__.py
--rw-rw-rw-   0        0        0    10128 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/tab/build/tab_build.py
--rw-rw-rw-   0        0        0     5678 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/tab/build/tab_init.py
--rw-rw-rw-   0        0        0     1664 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/tab/build/test_tab_build.py
-drwxrwxrwx   0        0        0        0 2023-06-27 07:05:04.061320 apf-ci-1.2.180/apf_ci/util/
--rw-rw-rw-   0        0        0        0 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/util/__init__.py
--rw-rw-rw-   0        0        0      392 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/util/content_service_config.py
-drwxrwxrwx   0        0        0        0 2023-06-27 07:05:04.065828 apf-ci-1.2.180/apf_ci/util/cs_sdk/
--rw-rw-rw-   0        0        0      650 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/util/cs_sdk/__init__.py
--rw-rw-rw-   0        0        0     1060 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/util/cs_sdk/chunk_utils.py
--rw-rw-rw-   0        0        0     4841 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/util/cs_sdk/dentry.py
--rw-rw-rw-   0        0        0      352 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/util/cs_sdk/extend_upload_data.py
--rw-rw-rw-   0        0        0     2290 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/util/cs_sdk/upload_test.py
--rw-rw-rw-   0        0        0     2284 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/util/execute_command_utils.py
--rw-rw-rw-   0        0        0    15972 2023-06-27 03:39:03.000000 apf-ci-1.2.180/apf_ci/util/file_utils.py
--rw-rw-rw-   0        0        0     2278 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/util/hook_service.py
--rw-rw-rw-   0        0        0     7315 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/util/http_utils.py
--rw-rw-rw-   0        0        0     2614 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/util/jenkins_utils.py
-drwxrwxrwx   0        0        0        0 2023-06-27 07:05:04.070828 apf-ci-1.2.180/apf_ci/util/log_factory/
--rw-rw-rw-   0        0        0        0 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/util/log_factory/__init__.py
--rw-rw-rw-   0        0        0     2267 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/util/log_factory/file_write_logger.py
--rw-rw-rw-   0        0        0      710 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/util/log_factory/ilogger.py
--rw-rw-rw-   0        0        0     1232 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/util/log_factory/log_error_message.py
--rw-rw-rw-   0        0        0      265 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/util/log_factory/logger_enum.py
--rw-rw-rw-   0        0        0     1935 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/util/log_factory/logger_error_enum.py
--rw-rw-rw-   0        0        0     1212 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/util/log_factory/logger_factory.py
--rw-rw-rw-   0        0        0     1753 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/util/log_factory/print_logger.py
--rw-rw-rw-   0        0        0     3407 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/util/log_utils.py
--rw-rw-rw-   0        0        0     3294 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/util/mac_token_utils.py
--rw-rw-rw-   0        0        0     1462 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/util/md5_utils.py
--rw-rw-rw-   0        0        0      415 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/util/parse_utils.py
--rw-rw-rw-   0        0        0     4255 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/util/private_support_utils.py
--rw-rw-rw-   0        0        0     2812 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/util/property.py
--rw-rw-rw-   0        0        0     3611 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/util/routes_to_json.py
--rw-rw-rw-   0        0        0     6654 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/util/rsa_utils.py
--rw-rw-rw-   0        0        0      462 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/util/string_utils.py
-drwxrwxrwx   0        0        0        0 2023-06-27 07:05:04.074331 apf-ci-1.2.180/apf_ci/util/uc_sdk/
--rw-rw-rw-   0        0        0        0 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/util/uc_sdk/__init__.py
--rw-rw-rw-   0        0        0    18304 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/util/uc_sdk/nd_uc_new.py
--rw-rw-rw-   0        0        0    19074 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/util/uc_sdk/nd_uc_new2.py
--rw-rw-rw-   0        0        0     1198 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/util/uc_sdk/rand.py
--rw-rw-rw-   0        0        0      221 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/util/uc_sdk/uc_sdk_code.py
--rw-rw-rw-   0        0        0     8979 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/util/upload_utils.py
--rw-rw-rw-   0        0        0     2326 2023-06-07 15:36:10.000000 apf-ci-1.2.180/apf_ci/util/version_utils.py
-drwxrwxrwx   0        0        0        0 2023-06-27 07:05:03.871498 apf-ci-1.2.180/apf_ci.egg-info/
--rw-rw-rw-   0        0        0     2533 2023-06-27 07:05:03.000000 apf-ci-1.2.180/apf_ci.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    10603 2023-06-27 07:05:03.000000 apf-ci-1.2.180/apf_ci.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-27 07:05:03.000000 apf-ci-1.2.180/apf_ci.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      869 2023-06-27 07:05:03.000000 apf-ci-1.2.180/apf_ci.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       16 2023-06-27 07:05:03.000000 apf-ci-1.2.180/apf_ci.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-06-27 07:05:03.000000 apf-ci-1.2.180/apf_ci.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-27 07:05:04.078335 apf-ci-1.2.180/data/
--rw-rw-rw-   0        0        0      665 2023-06-07 15:36:10.000000 apf-ci-1.2.180/data/config.json
--rw-rw-rw-   0        0        0      673 2023-06-07 15:36:10.000000 apf-ci-1.2.180/data/config_beta.json
--rw-rw-rw-   0        0        0      666 2023-06-07 15:36:10.000000 apf-ci-1.2.180/data/config_debug.json
--rw-rw-rw-   0        0        0      657 2023-06-07 15:36:10.000000 apf-ci-1.2.180/data/config_dev.json
--rw-rw-rw-   0        0        0       42 2023-06-27 07:05:04.079334 apf-ci-1.2.180/setup.cfg
--rw-rw-rw-   0        0        0     4301 2023-06-07 15:36:10.000000 apf-ci-1.2.180/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-27 07:11:19.690562 apf-ci-1.2.180.1/
+-rw-rw-rw-   0        0        0     2535 2023-06-27 07:11:19.690562 apf-ci-1.2.180.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1268 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-27 07:11:19.467087 apf-ci-1.2.180.1/apf_ci/
+-rw-rw-rw-   0        0        0      654 2023-06-27 07:11:08.000000 apf-ci-1.2.180.1/apf_ci/__init__.py
+-rw-rw-rw-   0        0        0      425 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/__main__.py
+drwxrwxrwx   0        0        0        0 2023-06-27 07:11:19.480155 apf-ci-1.2.180.1/apf_ci/android/
+-rw-rw-rw-   0        0        0        0 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/android/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-27 07:11:19.480155 apf-ci-1.2.180.1/apf_ci/android/build_prepare/
+-rw-rw-rw-   0        0        0        0 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/android/build_prepare/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-27 07:11:19.486746 apf-ci-1.2.180.1/apf_ci/android/build_prepare/builder/
+-rw-rw-rw-   0        0        0        0 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/android/build_prepare/builder/__init__.py
+-rw-rw-rw-   0        0        0    20753 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/android/build_prepare/builder/android_build_prepare_builder.py
+-rw-rw-rw-   0        0        0    10180 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/android/build_prepare/builder/certificate_builder.py
+-rw-rw-rw-   0        0        0     5535 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/android/build_prepare/builder/clean_config_file_builder.py
+-rw-rw-rw-   0        0        0    10616 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/android/build_prepare/builder/config_info_sync.py
+-rw-rw-rw-   0        0        0     7782 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/android/build_prepare/builder/local_properties_builder.py
+-rw-rw-rw-   0        0        0     4434 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/android/build_prepare/builder/multi_channel_builder.py
+-rw-rw-rw-   0        0        0     9242 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/android/build_prepare/builder/update_project_info_builder.py
+drwxrwxrwx   0        0        0        0 2023-06-27 07:11:19.486746 apf-ci-1.2.180.1/apf_ci/android/prepare/
+-rw-rw-rw-   0        0        0        0 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/android/prepare/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-27 07:11:19.490152 apf-ci-1.2.180.1/apf_ci/android/prepare/builder/
+-rw-rw-rw-   0        0        0        0 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/android/prepare/builder/__init__.py
+-rw-rw-rw-   0        0        0     9313 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/android/prepare/builder/android_injections_builder.py
+-rw-rw-rw-   0        0        0     1571 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/android/prepare/builder/android_prepare_builder.py
+-rw-rw-rw-   0        0        0    19270 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/android/prepare/builder/generate_dependency_builder.py
+drwxrwxrwx   0        0        0        0 2023-06-27 07:11:19.491155 apf-ci-1.2.180.1/apf_ci/android/prepare/model/
+-rw-rw-rw-   0        0        0        0 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/android/prepare/model/__init__.py
+-rw-rw-rw-   0        0        0      516 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/android/prepare/model/meta_data_note.py
+drwxrwxrwx   0        0        0        0 2023-06-27 07:11:19.491155 apf-ci-1.2.180.1/apf_ci/app_compare/
+-rw-rw-rw-   0        0        0        0 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/app_compare/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-27 07:11:19.497672 apf-ci-1.2.180.1/apf_ci/app_compare/build/
+-rw-rw-rw-   0        0        0        0 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/app_compare/build/__init__.py
+-rw-rw-rw-   0        0        0     1035 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/app_compare/build/apk_utils.py
+-rw-rw-rw-   0        0        0     3013 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/app_compare/build/app_compare.py
+-rw-rw-rw-   0        0        0     4371 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/app_compare/build/app_compare_android.py
+-rw-rw-rw-   0        0        0     4452 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/app_compare/build/app_compare_ios.py
+-rw-rw-rw-   0        0        0     6139 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/app_compare/build/app_compare_utils.py
+-rw-rw-rw-   0        0        0     5428 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/app_compare/build/dependency_utils.py
+-rw-rw-rw-   0        0        0     2162 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/app_compare/build/test_app_compare.py
+drwxrwxrwx   0        0        0        0 2023-06-27 07:11:19.498672 apf-ci-1.2.180.1/apf_ci/app_component_compare/
+-rw-rw-rw-   0        0        0        0 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/app_component_compare/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-27 07:11:19.499974 apf-ci-1.2.180.1/apf_ci/app_component_compare/build/
+-rw-rw-rw-   0        0        0        0 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/app_component_compare/build/__init__.py
+-rw-rw-rw-   0        0        0    12815 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/app_component_compare/build/app_component_compare.py
+-rw-rw-rw-   0        0        0     1270 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/app_component_compare/build/test_app_component_compare.py
+drwxrwxrwx   0        0        0        0 2023-06-27 07:11:19.511488 apf-ci-1.2.180.1/apf_ci/app_init/
+-rw-rw-rw-   0        0        0        0 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/app_init/__init__.py
+-rw-rw-rw-   0        0        0    10701 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/app_init/app_config.py
+-rw-rw-rw-   0        0        0     6117 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/app_init/app_init.py
+-rw-rw-rw-   0        0        0     5011 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/app_init/app_resource.py
+-rw-rw-rw-   0        0        0      969 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/app_init/test_after_app_init.py
+-rw-rw-rw-   0        0        0     3212 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/app_init/test_app_init.py
+-rw-rw-rw-   0        0        0    14399 2023-06-27 04:16:12.000000 apf-ci-1.2.180.1/apf_ci/app_init/update_variable_json.py
+drwxrwxrwx   0        0        0        0 2023-06-27 07:11:19.517998 apf-ci-1.2.180.1/apf_ci/app_init/utils/
+-rw-rw-rw-   0        0        0      255 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/app_init/utils/__init__.py
+-rw-rw-rw-   0        0        0     1141 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/app_init/utils/appinfo_utils.py
+-rw-rw-rw-   0        0        0     1454 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/app_init/utils/apps_utils.py
+-rw-rw-rw-   0        0        0    10365 2023-06-27 03:14:12.000000 apf-ci-1.2.180.1/apf_ci/app_init/utils/build_config_utils.py
+-rw-rw-rw-   0        0        0     7510 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/app_init/utils/image_utils.py
+-rw-rw-rw-   0        0        0     1710 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/app_init/utils/js_third_app_utils.py
+-rw-rw-rw-   0        0        0     2607 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/app_init/utils/key_chain_utils.py
+-rw-rw-rw-   0        0        0    37443 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/app_init/utils/language_utils.py
+-rw-rw-rw-   0        0        0    15803 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/app_init/utils/variable_utils.py
+-rw-rw-rw-   0        0        0      566 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/app_init/utils/variables_script_utils.py
+drwxrwxrwx   0        0        0        0 2023-06-27 07:11:19.522985 apf-ci-1.2.180.1/apf_ci/app_res/
+-rw-rw-rw-   0        0        0        0 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/app_res/__init__.py
+-rw-rw-rw-   0        0        0     1146 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/app_res/android_plugin.py
+-rw-rw-rw-   0        0        0     2064 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/app_res/app_res.py
+-rw-rw-rw-   0        0        0    10178 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/app_res/language_res.py
+-rw-rw-rw-   0        0        0     5878 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/app_res/skin_res.py
+-rw-rw-rw-   0        0        0     3118 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/app_res/test_skin_res.py
+-rw-rw-rw-   0        0        0      833 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/cli.py
+drwxrwxrwx   0        0        0        0 2023-06-27 07:11:19.538210 apf-ci-1.2.180.1/apf_ci/commands/
+-rw-rw-rw-   0        0        0        0 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/commands/__init__.py
+-rw-rw-rw-   0        0        0      936 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/commands/android_build_prepare.py
+-rw-rw-rw-   0        0        0      949 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/commands/android_prepare.py
+-rw-rw-rw-   0        0        0     1413 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/commands/app_compare.py
+-rw-rw-rw-   0        0        0     1563 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/commands/app_component_compare.py
+-rw-rw-rw-   0        0        0     2482 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/commands/app_init.py
+-rw-rw-rw-   0        0        0      426 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/commands/command_const.py
+-rw-rw-rw-   0        0        0      695 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/commands/flutter.py
+-rw-rw-rw-   0        0        0     1138 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/commands/h5_grain.py
+-rw-rw-rw-   0        0        0     2719 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/commands/h5_grain_config.py
+-rw-rw-rw-   0        0        0     1481 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/commands/h5_widget_resource.py
+-rw-rw-rw-   0        0        0      883 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/commands/local_h5.py
+-rw-rw-rw-   0        0        0     1520 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/commands/react_widget_resource.py
+-rw-rw-rw-   0        0        0     2380 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/commands/rn.py
+-rw-rw-rw-   0        0        0     2520 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/commands/rn_widget.py
+-rw-rw-rw-   0        0        0     2420 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/commands/subapp_config.py
+-rw-rw-rw-   0        0        0     2108 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/commands/tab_build.py
+-rw-rw-rw-   0        0        0     1771 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/commands/variable.py
+drwxrwxrwx   0        0        0        0 2023-06-27 07:11:19.552718 apf-ci-1.2.180.1/apf_ci/config/
+-rw-rw-rw-   0        0        0        0 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/config/__init__.py
+-rw-rw-rw-   0        0        0    49911 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/config/app_config.py
+-rw-rw-rw-   0        0        0    13448 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/config/biz_comp_transform.py
+-rw-rw-rw-   0        0        0    20248 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/config/defines.py
+-rw-rw-rw-   0        0        0     7793 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/config/env_service.py
+-rw-rw-rw-   0        0        0     1953 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/config/h5_widget_i18n_utils.py
+-rw-rw-rw-   0        0        0     5387 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/config/json_property_analysis.py
+-rw-rw-rw-   0        0        0     5567 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/config/language_service.py
+-rw-rw-rw-   0        0        0     3329 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/config/lite_app.py
+-rw-rw-rw-   0        0        0     3201 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/config/page_attributes.py
+-rw-rw-rw-   0        0        0     4553 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/config/page_i18n_utils.py
+-rw-rw-rw-   0        0        0    20218 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/config/properties_transform.py
+-rw-rw-rw-   0        0        0    13095 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/config/runtime.py
+drwxrwxrwx   0        0        0        0 2023-06-27 07:11:19.553237 apf-ci-1.2.180.1/apf_ci/config/test/
+-rw-rw-rw-   0        0        0        0 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/config/test/__init__.py
+-rw-rw-rw-   0        0        0     1198 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/config/test/widget_tree_test.py
+-rw-rw-rw-   0        0        0     4594 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/config/widget_i18n_utils.py
+-rw-rw-rw-   0        0        0     8942 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/config/widget_tree.py
+drwxrwxrwx   0        0        0        0 2023-06-27 07:11:19.555256 apf-ci-1.2.180.1/apf_ci/constant/
+-rw-rw-rw-   0        0        0        0 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/constant/__init__.py
+-rw-rw-rw-   0        0        0      693 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/constant/constants.py
+-rw-rw-rw-   0        0        0     1581 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/constant/path_constant.py
+drwxrwxrwx   0        0        0        0 2023-06-27 07:11:19.560247 apf-ci-1.2.180.1/apf_ci/flutter/
+-rw-rw-rw-   0        0        0        0 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/flutter/__init__.py
+-rw-rw-rw-   0        0        0    15963 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/flutter/flutter.py
+-rw-rw-rw-   0        0        0    29413 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/flutter/flutter_android_build.py
+-rw-rw-rw-   0        0        0     6505 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/flutter/flutter_build.py
+-rw-rw-rw-   0        0        0     2791 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/flutter/flutter_command_utils.py
+-rw-rw-rw-   0        0        0     2384 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/flutter/flutter_ios_build.py
+drwxrwxrwx   0        0        0        0 2023-06-27 07:11:19.562755 apf-ci-1.2.180.1/apf_ci/flutter/resource/
+-rw-rw-rw-   0        0        0        0 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/flutter/resource/__init__.py
+-rw-rw-rw-   0        0        0     7945 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/flutter/resource/flutter_language_resource.py
+-rw-rw-rw-   0        0        0     1677 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/flutter/resource/flutter_resource.py
+-rw-rw-rw-   0        0        0     4466 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/flutter/resource/flutter_skin_resource.py
+drwxrwxrwx   0        0        0        0 2023-06-27 07:11:19.564850 apf-ci-1.2.180.1/apf_ci/h5_grain/
+-rw-rw-rw-   0        0        0        0 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/h5_grain/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-27 07:11:19.570559 apf-ci-1.2.180.1/apf_ci/h5_grain/builder/
+-rw-rw-rw-   0        0        0        0 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/h5_grain/builder/__init__.py
+-rw-rw-rw-   0        0        0    12969 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/h5_grain/builder/analysis_pages_builder.py
+-rw-rw-rw-   0        0        0     1192 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/h5_grain/builder/create_package_builder.py
+-rw-rw-rw-   0        0        0     1586 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/h5_grain/builder/ensure_template_builder.py
+-rw-rw-rw-   0        0        0     5892 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/h5_grain/builder/h5_grain_builder.py
+-rw-rw-rw-   0        0        0    58946 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/h5_grain/builder/npm_operation_builder.py
+-rw-rw-rw-   0        0        0     4275 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/h5_grain/builder/template_builder.py
+-rw-rw-rw-   0        0        0      362 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/h5_grain/h5_page.py
+-rw-rw-rw-   0        0        0      592 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/h5_grain/package_model.py
+drwxrwxrwx   0        0        0        0 2023-06-27 07:11:19.571569 apf-ci-1.2.180.1/apf_ci/h5_grain_config/
+-rw-rw-rw-   0        0        0        0 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/h5_grain_config/__init__.py
+-rw-rw-rw-   0        0        0     1812 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/h5_grain_config/h5_grain_config_test.py
+-rw-rw-rw-   0        0        0     5028 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/h5_grain_config/h5_grain_init.py
+drwxrwxrwx   0        0        0        0 2023-06-27 07:11:19.573072 apf-ci-1.2.180.1/apf_ci/h5_widget_resource/
+-rw-rw-rw-   0        0        0        0 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/h5_widget_resource/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-27 07:11:19.577075 apf-ci-1.2.180.1/apf_ci/h5_widget_resource/builder/
+-rw-rw-rw-   0        0        0        0 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/h5_widget_resource/builder/__init__.py
+-rw-rw-rw-   0        0        0     8017 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/h5_widget_resource/builder/create_package_builder.py
+-rw-rw-rw-   0        0        0    10611 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/h5_widget_resource/builder/create_resource_builder.py
+-rw-rw-rw-   0        0        0     2863 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/h5_widget_resource/builder/ensure_template_builder.py
+-rw-rw-rw-   0        0        0     4504 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/h5_widget_resource/builder/h5_widget_resource_builder.py
+drwxrwxrwx   0        0        0        0 2023-06-27 07:11:19.580076 apf-ci-1.2.180.1/apf_ci/init/
+-rw-rw-rw-   0        0        0        0 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/init/__init__.py
+-rw-rw-rw-   0        0        0     7770 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/init/git_template_service.py
+-rw-rw-rw-   0        0        0    29131 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/init/init_global_variable_service.py
+-rw-rw-rw-   0        0        0     2221 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/init/validate_service.py
+drwxrwxrwx   0        0        0        0 2023-06-27 07:11:19.580076 apf-ci-1.2.180.1/apf_ci/lite_app/
+-rw-rw-rw-   0        0        0        0 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/lite_app/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-27 07:11:19.591821 apf-ci-1.2.180.1/apf_ci/lite_app/cache/
+-rw-rw-rw-   0        0        0        0 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/lite_app/cache/__init__.py
+-rw-rw-rw-   0        0        0     1351 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/lite_app/cache/abstract_cache.py
+-rw-rw-rw-   0        0        0     4771 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/lite_app/cache/abstract_first_level_cache.py
+-rw-rw-rw-   0        0        0     3994 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/lite_app/cache/abstract_second_level_cache.py
+-rw-rw-rw-   0        0        0     2736 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/lite_app/cache/abstract_three_level_cache.py
+-rw-rw-rw-   0        0        0     1673 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/lite_app/cache/cache_factory.py
+drwxrwxrwx   0        0        0        0 2023-06-27 07:11:19.596915 apf-ci-1.2.180.1/apf_ci/lite_app/cache/factor/
+-rw-rw-rw-   0        0        0        0 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/lite_app/cache/factor/__init__.py
+-rw-rw-rw-   0        0        0     7153 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/lite_app/cache/factor/abstract_cache_factor.py
+-rw-rw-rw-   0        0        0      117 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/lite_app/cache/factor/icache_factor.py
+-rw-rw-rw-   0        0        0     4525 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/lite_app/cache/factor/local_h5_cache_factor.py
+-rw-rw-rw-   0        0        0     5030 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/lite_app/cache/factor/react_cache_factor.py
+-rw-rw-rw-   0        0        0      616 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/lite_app/cache/first_level_local_h5_cache.py
+-rw-rw-rw-   0        0        0      888 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/lite_app/cache/first_level_react_cache.py
+-rw-rw-rw-   0        0        0      541 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/lite_app/cache/icache.py
+-rw-rw-rw-   0        0        0      742 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/lite_app/cache/second_level_local_h5_cache.py
+-rw-rw-rw-   0        0        0      961 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/lite_app/cache/second_level_react_cache.py
+-rw-rw-rw-   0        0        0     1095 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/lite_app/cache/three_level_local_h5_cache.py
+-rw-rw-rw-   0        0        0     1504 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/lite_app/cache/three_level_react_cache.py
+drwxrwxrwx   0        0        0        0 2023-06-27 07:11:19.599918 apf-ci-1.2.180.1/apf_ci/lite_app/concurrent/
+-rw-rw-rw-   0        0        0        0 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/lite_app/concurrent/__init__.py
+-rw-rw-rw-   0        0        0     2077 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/lite_app/concurrent/concurrent_build_client.py
+-rw-rw-rw-   0        0        0      350 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/lite_app/concurrent/local_h5_build_callable.py
+-rw-rw-rw-   0        0        0      336 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/lite_app/concurrent/react_build_callable.py
+drwxrwxrwx   0        0        0        0 2023-06-27 07:11:19.604381 apf-ci-1.2.180.1/apf_ci/lite_app/lite_enum/
+-rw-rw-rw-   0        0        0        0 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/lite_app/lite_enum/__init__.py
+-rw-rw-rw-   0        0        0      429 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/lite_app/lite_enum/app_type_enum.py
+-rw-rw-rw-   0        0        0      429 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/lite_app/lite_enum/cache_enum.py
+-rw-rw-rw-   0        0        0      465 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/lite_app/lite_enum/component_type_enum.py
+drwxrwxrwx   0        0        0        0 2023-06-27 07:11:19.605377 apf-ci-1.2.180.1/apf_ci/lite_app/local_h5/
+-rw-rw-rw-   0        0        0        0 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/lite_app/local_h5/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-27 07:11:19.606380 apf-ci-1.2.180.1/apf_ci/lite_app/local_h5/builder/
+-rw-rw-rw-   0        0        0        0 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/lite_app/local_h5/builder/__init__.py
+-rw-rw-rw-   0        0        0     4891 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/lite_app/local_h5/builder/local_h5_builder.py
+drwxrwxrwx   0        0        0        0 2023-06-27 07:11:19.610385 apf-ci-1.2.180.1/apf_ci/lite_app/model/
+-rw-rw-rw-   0        0        0        0 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/lite_app/model/__init__.py
+-rw-rw-rw-   0        0        0      835 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/lite_app/model/cache_bo.py
+-rw-rw-rw-   0        0        0     1225 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/lite_app/model/cache_factor_bo.py
+-rw-rw-rw-   0        0        0      520 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/lite_app/model/js_package_cache.py
+-rw-rw-rw-   0        0        0     1002 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/lite_app/model/npm_dto.py
+-rw-rw-rw-   0        0        0      394 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/lite_app/model/template_bo.py
+drwxrwxrwx   0        0        0        0 2023-06-27 07:11:19.614894 apf-ci-1.2.180.1/apf_ci/lite_app/parser/
+-rw-rw-rw-   0        0        0        0 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/lite_app/parser/__init__.py
+-rw-rw-rw-   0        0        0     3922 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/lite_app/parser/abstract_parser.py
+-rw-rw-rw-   0        0        0      847 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/lite_app/parser/iparser.py
+-rw-rw-rw-   0        0        0      982 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/lite_app/parser/local_h5_parser.py
+-rw-rw-rw-   0        0        0     1319 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/lite_app/parser/react_parser.py
+drwxrwxrwx   0        0        0        0 2023-06-27 07:11:19.619903 apf-ci-1.2.180.1/apf_ci/lite_app/rn/
+-rw-rw-rw-   0        0        0        0 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/lite_app/rn/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-27 07:11:19.620894 apf-ci-1.2.180.1/apf_ci/lite_app/rn/builder/
+-rw-rw-rw-   0        0        0        0 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/lite_app/rn/builder/__init__.py
+-rw-rw-rw-   0        0        0    23957 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/lite_app/rn/builder/react_builder.py
+-rw-rw-rw-   0        0        0     4051 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/lite_app/rn/component.py
+-rw-rw-rw-   0        0        0     7198 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/lite_app/rn/rn.py
+-rw-rw-rw-   0        0        0      133 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/lite_app/rn/rn_init.py
+-rw-rw-rw-   0        0        0     7705 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/lite_app/rn/template.py
+-rw-rw-rw-   0        0        0     3532 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/lite_app/rn/terminal_interaction.py
+drwxrwxrwx   0        0        0        0 2023-06-27 07:11:19.631405 apf-ci-1.2.180.1/apf_ci/lite_app/service/
+-rw-rw-rw-   0        0        0        0 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/lite_app/service/__init__.py
+-rw-rw-rw-   0        0        0    11439 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/lite_app/service/apf_service.py
+-rw-rw-rw-   0        0        0     6628 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/lite_app/service/config_service.py
+-rw-rw-rw-   0        0        0    22272 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/lite_app/service/local_h5_service.py
+-rw-rw-rw-   0        0        0    18712 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/lite_app/service/react_service.py
+drwxrwxrwx   0        0        0        0 2023-06-27 07:11:19.633914 apf-ci-1.2.180.1/apf_ci/react_widget_resource/
+-rw-rw-rw-   0        0        0        0 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/react_widget_resource/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-27 07:11:19.637914 apf-ci-1.2.180.1/apf_ci/react_widget_resource/builder/
+-rw-rw-rw-   0        0        0        0 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/react_widget_resource/builder/__init__.py
+-rw-rw-rw-   0        0        0    21537 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/react_widget_resource/builder/create_resource_builder.py
+-rw-rw-rw-   0        0        0     6765 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/react_widget_resource/builder/ensure_template_builder.py
+-rw-rw-rw-   0        0        0     8095 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/react_widget_resource/builder/npm_builder.py
+-rw-rw-rw-   0        0        0     7714 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/react_widget_resource/builder/react_widget_resource_builder.py
+-rw-rw-rw-   0        0        0    12138 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/react_widget_resource/builder/rn_resource_analysis_pages_builder.py
+drwxrwxrwx   0        0        0        0 2023-06-27 07:11:19.641915 apf-ci-1.2.180.1/apf_ci/react_widget_resource/test/
+-rw-rw-rw-   0        0        0        0 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/react_widget_resource/test/__init__.py
+-rw-rw-rw-   0        0        0     2839 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/react_widget_resource/test/test_create_resource_builder.py
+-rw-rw-rw-   0        0        0     1535 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/react_widget_resource/test/test_ensure_template_builder.py
+-rw-rw-rw-   0        0        0     3608 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/react_widget_resource/test/test_npm_builder.py
+-rw-rw-rw-   0        0        0     2925 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/react_widget_resource/test/test_rn_resource_analysis_pages_builder.py
+drwxrwxrwx   0        0        0        0 2023-06-27 07:11:19.645964 apf-ci-1.2.180.1/apf_ci/resource/
+-rw-rw-rw-   0        0        0        0 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/resource/__init__.py
+-rw-rw-rw-   0        0        0    10253 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/resource/cache_service.py
+-rw-rw-rw-   0        0        0    12162 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/resource/language.py
+-rw-rw-rw-   0        0        0    13045 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/resource/resource_builder.py
+-rw-rw-rw-   0        0        0    10733 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/resource/skin.py
+drwxrwxrwx   0        0        0        0 2023-06-27 07:11:19.646964 apf-ci-1.2.180.1/apf_ci/resource/test/
+-rw-rw-rw-   0        0        0        0 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/resource/test/__init__.py
+-rw-rw-rw-   0        0        0      745 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/resource/test/test_resource_config.py
+drwxrwxrwx   0        0        0        0 2023-06-27 07:11:19.648964 apf-ci-1.2.180.1/apf_ci/rn_widget/
+-rw-rw-rw-   0        0        0        0 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/rn_widget/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-27 07:11:19.654493 apf-ci-1.2.180.1/apf_ci/rn_widget/builder/
+-rw-rw-rw-   0        0        0        0 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/rn_widget/builder/__init__.py
+-rw-rw-rw-   0        0        0    18305 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/rn_widget/builder/analysis_pages_builder.py
+-rw-rw-rw-   0        0        0     6383 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/rn_widget/builder/build_tool_builder.py
+-rw-rw-rw-   0        0        0     2567 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/rn_widget/builder/check_env_name_builder.py
+-rw-rw-rw-   0        0        0    18802 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/rn_widget/builder/multi_language_resource_builder.py
+-rw-rw-rw-   0        0        0    55415 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/rn_widget/builder/npm_operation_builder.py
+-rw-rw-rw-   0        0        0     6238 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/rn_widget/builder/react_widget_builder.py
+-rw-rw-rw-   0        0        0     6861 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/rn_widget/builder/templater_builder.py
+drwxrwxrwx   0        0        0        0 2023-06-27 07:11:19.656494 apf-ci-1.2.180.1/apf_ci/rn_widget/model/
+-rw-rw-rw-   0        0        0        0 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/rn_widget/model/__init__.py
+-rw-rw-rw-   0        0        0      348 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/rn_widget/model/package_model.py
+-rw-rw-rw-   0        0        0      420 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/rn_widget/model/page.py
+-rw-rw-rw-   0        0        0      260 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/rn_widget/model/widget.py
+-rw-rw-rw-   0        0        0     8427 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/rn_widget/rn_widget.py
+drwxrwxrwx   0        0        0        0 2023-06-27 07:11:19.658494 apf-ci-1.2.180.1/apf_ci/rn_widget/test/
+-rw-rw-rw-   0        0        0       29 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/rn_widget/test/__init__.py
+-rw-rw-rw-   0        0        0      777 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/rn_widget/test/rn_widget_build_test.py
+-rw-rw-rw-   0        0        0     6868 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/rn_widget/test/test_multi_language_resource.py
+-rw-rw-rw-   0        0        0    16704 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/rn_widget/widget.py
+drwxrwxrwx   0        0        0        0 2023-06-27 07:11:19.659493 apf-ci-1.2.180.1/apf_ci/subapp_config/
+-rw-rw-rw-   0        0        0        0 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/subapp_config/__init__.py
+-rw-rw-rw-   0        0        0     6582 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/subapp_config/subapp_config_init.py
+drwxrwxrwx   0        0        0        0 2023-06-27 07:11:19.659493 apf-ci-1.2.180.1/apf_ci/tab/
+-rw-rw-rw-   0        0        0        0 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/tab/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-27 07:11:19.661493 apf-ci-1.2.180.1/apf_ci/tab/build/
+-rw-rw-rw-   0        0        0        0 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/tab/build/__init__.py
+-rw-rw-rw-   0        0        0    10128 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/tab/build/tab_build.py
+-rw-rw-rw-   0        0        0     5678 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/tab/build/tab_init.py
+-rw-rw-rw-   0        0        0     1664 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/tab/build/test_tab_build.py
+drwxrwxrwx   0        0        0        0 2023-06-27 07:11:19.674018 apf-ci-1.2.180.1/apf_ci/util/
+-rw-rw-rw-   0        0        0        0 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/util/__init__.py
+-rw-rw-rw-   0        0        0      392 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/util/content_service_config.py
+drwxrwxrwx   0        0        0        0 2023-06-27 07:11:19.677018 apf-ci-1.2.180.1/apf_ci/util/cs_sdk/
+-rw-rw-rw-   0        0        0      650 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/util/cs_sdk/__init__.py
+-rw-rw-rw-   0        0        0     1060 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/util/cs_sdk/chunk_utils.py
+-rw-rw-rw-   0        0        0     4841 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/util/cs_sdk/dentry.py
+-rw-rw-rw-   0        0        0      352 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/util/cs_sdk/extend_upload_data.py
+-rw-rw-rw-   0        0        0     2290 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/util/cs_sdk/upload_test.py
+-rw-rw-rw-   0        0        0     2284 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/util/execute_command_utils.py
+-rw-rw-rw-   0        0        0    15972 2023-06-27 03:39:03.000000 apf-ci-1.2.180.1/apf_ci/util/file_utils.py
+-rw-rw-rw-   0        0        0     2278 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/util/hook_service.py
+-rw-rw-rw-   0        0        0     7315 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/util/http_utils.py
+-rw-rw-rw-   0        0        0     2614 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/util/jenkins_utils.py
+drwxrwxrwx   0        0        0        0 2023-06-27 07:11:19.681028 apf-ci-1.2.180.1/apf_ci/util/log_factory/
+-rw-rw-rw-   0        0        0        0 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/util/log_factory/__init__.py
+-rw-rw-rw-   0        0        0     2267 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/util/log_factory/file_write_logger.py
+-rw-rw-rw-   0        0        0      710 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/util/log_factory/ilogger.py
+-rw-rw-rw-   0        0        0     1232 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/util/log_factory/log_error_message.py
+-rw-rw-rw-   0        0        0      265 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/util/log_factory/logger_enum.py
+-rw-rw-rw-   0        0        0     1935 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/util/log_factory/logger_error_enum.py
+-rw-rw-rw-   0        0        0     1212 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/util/log_factory/logger_factory.py
+-rw-rw-rw-   0        0        0     1753 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/util/log_factory/print_logger.py
+-rw-rw-rw-   0        0        0     3407 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/util/log_utils.py
+-rw-rw-rw-   0        0        0     3294 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/util/mac_token_utils.py
+-rw-rw-rw-   0        0        0     1462 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/util/md5_utils.py
+-rw-rw-rw-   0        0        0      415 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/util/parse_utils.py
+-rw-rw-rw-   0        0        0     4255 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/util/private_support_utils.py
+-rw-rw-rw-   0        0        0     2812 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/util/property.py
+-rw-rw-rw-   0        0        0     3611 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/util/routes_to_json.py
+-rw-rw-rw-   0        0        0     6654 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/util/rsa_utils.py
+-rw-rw-rw-   0        0        0      462 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/util/string_utils.py
+drwxrwxrwx   0        0        0        0 2023-06-27 07:11:19.686542 apf-ci-1.2.180.1/apf_ci/util/uc_sdk/
+-rw-rw-rw-   0        0        0        0 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/util/uc_sdk/__init__.py
+-rw-rw-rw-   0        0        0    18304 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/util/uc_sdk/nd_uc_new.py
+-rw-rw-rw-   0        0        0    19074 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/util/uc_sdk/nd_uc_new2.py
+-rw-rw-rw-   0        0        0     1198 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/util/uc_sdk/rand.py
+-rw-rw-rw-   0        0        0      221 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/util/uc_sdk/uc_sdk_code.py
+-rw-rw-rw-   0        0        0     8979 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/util/upload_utils.py
+-rw-rw-rw-   0        0        0     2326 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/apf_ci/util/version_utils.py
+drwxrwxrwx   0        0        0        0 2023-06-27 07:11:19.479155 apf-ci-1.2.180.1/apf_ci.egg-info/
+-rw-rw-rw-   0        0        0     2535 2023-06-27 07:11:19.000000 apf-ci-1.2.180.1/apf_ci.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    10603 2023-06-27 07:11:19.000000 apf-ci-1.2.180.1/apf_ci.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-27 07:11:19.000000 apf-ci-1.2.180.1/apf_ci.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      869 2023-06-27 07:11:19.000000 apf-ci-1.2.180.1/apf_ci.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       16 2023-06-27 07:11:19.000000 apf-ci-1.2.180.1/apf_ci.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-27 07:11:19.000000 apf-ci-1.2.180.1/apf_ci.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-27 07:11:19.689563 apf-ci-1.2.180.1/data/
+-rw-rw-rw-   0        0        0      665 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/data/config.json
+-rw-rw-rw-   0        0        0      673 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/data/config_beta.json
+-rw-rw-rw-   0        0        0      666 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/data/config_debug.json
+-rw-rw-rw-   0        0        0      657 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/data/config_dev.json
+-rw-rw-rw-   0        0        0       42 2023-06-27 07:11:19.691562 apf-ci-1.2.180.1/setup.cfg
+-rw-rw-rw-   0        0        0     4301 2023-06-07 15:36:10.000000 apf-ci-1.2.180.1/setup.py
```

### Comparing `apf-ci-1.2.180/PKG-INFO` & `apf-ci-1.2.180.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apf-ci
-Version: 1.2.180
+Version: 1.2.180.1
 Summary: App factory apf_ci build script
 Home-page: http://reference.sdp.nd/appfactory/userguide/light/react-native/React%20Native%E6%9C%AC%E5%9C%B0%E8%B0%83%E8%AF%95%E5%B7%A5%E5%85%B7%E4%BD%BF%E7%94%A8%E8%AF%B4%E6%98%8E.html
 Author: Lian Guo Qing
 Author-email: 765789371@qq.com
 License: ND License, Version 1.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `apf-ci-1.2.180/README.md` & `apf-ci-1.2.180.1/README.md`

 * *Files identical despite different names*

### Comparing `apf-ci-1.2.180/apf_ci/__init__.py` & `apf-ci-1.2.180.1/apf_ci/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,14 @@
     "__email__", "__license__", "__copyright__",
 )
 
 __title__ = "apf-ci"
 __summary__ = "CI build script for app factory on PyPI"
 __uri__ = "http://reference.sdp.nd/appfactory/userguide/light/react-native/React%20Native%E6%9C%AC%E5%9C%B0%E8%B0%83%E8%AF%95%E5%B7%A5%E5%85%B7%E4%BD%BF%E7%94%A8%E8%AF%B4%E6%98%8E.html"
 
-__version__ = "1.2.180"
+__version__ = "1.2.180.1"
 
 __author__ = "Lian Guo Qing"
 __email__ = "765789371@qq.com"
 
 __license__ = "ND License, Version 1.0"
 __copyright__ = "nd.com (c) 2018 All Rights Reserved"
```

### Comparing `apf-ci-1.2.180/apf_ci/android/build_prepare/builder/android_build_prepare_builder.py` & `apf-ci-1.2.180.1/apf_ci/android/build_prepare/builder/android_build_prepare_builder.py`

 * *Files identical despite different names*

### Comparing `apf-ci-1.2.180/apf_ci/android/build_prepare/builder/certificate_builder.py` & `apf-ci-1.2.180.1/apf_ci/android/build_prepare/builder/certificate_builder.py`

 * *Files identical despite different names*

### Comparing `apf-ci-1.2.180/apf_ci/android/build_prepare/builder/clean_config_file_builder.py` & `apf-ci-1.2.180.1/apf_ci/android/build_prepare/builder/clean_config_file_builder.py`

 * *Files identical despite different names*

### Comparing `apf-ci-1.2.180/apf_ci/android/build_prepare/builder/config_info_sync.py` & `apf-ci-1.2.180.1/apf_ci/android/build_prepare/builder/config_info_sync.py`

 * *Files identical despite different names*

### Comparing `apf-ci-1.2.180/apf_ci/android/build_prepare/builder/local_properties_builder.py` & `apf-ci-1.2.180.1/apf_ci/android/build_prepare/builder/local_properties_builder.py`

 * *Files identical despite different names*

### Comparing `apf-ci-1.2.180/apf_ci/android/build_prepare/builder/multi_channel_builder.py` & `apf-ci-1.2.180.1/apf_ci/android/build_prepare/builder/multi_channel_builder.py`

 * *Files identical despite different names*

### Comparing `apf-ci-1.2.180/apf_ci/android/build_prepare/builder/update_project_info_builder.py` & `apf-ci-1.2.180.1/apf_ci/android/build_prepare/builder/update_project_info_builder.py`

 * *Files identical despite different names*

### Comparing `apf-ci-1.2.180/apf_ci/android/prepare/builder/android_injections_builder.py` & `apf-ci-1.2.180.1/apf_ci/android/prepare/builder/android_injections_builder.py`

 * *Files identical despite different names*

### Comparing `apf-ci-1.2.180/apf_ci/android/prepare/builder/android_prepare_builder.py` & `apf-ci-1.2.180.1/apf_ci/android/prepare/builder/android_prepare_builder.py`

 * *Files identical despite different names*

### Comparing `apf-ci-1.2.180/apf_ci/android/prepare/builder/generate_dependency_builder.py` & `apf-ci-1.2.180.1/apf_ci/android/prepare/builder/generate_dependency_builder.py`

 * *Files identical despite different names*

### Comparing `apf-ci-1.2.180/apf_ci/android/prepare/model/meta_data_note.py` & `apf-ci-1.2.180.1/apf_ci/android/prepare/model/meta_data_note.py`

 * *Files identical despite different names*

### Comparing `apf-ci-1.2.180/apf_ci/app_compare/build/apk_utils.py` & `apf-ci-1.2.180.1/apf_ci/app_compare/build/apk_utils.py`

 * *Files identical despite different names*

### Comparing `apf-ci-1.2.180/apf_ci/app_compare/build/app_compare.py` & `apf-ci-1.2.180.1/apf_ci/app_compare/build/app_compare.py`

 * *Files identical despite different names*

### Comparing `apf-ci-1.2.180/apf_ci/app_compare/build/app_compare_android.py` & `apf-ci-1.2.180.1/apf_ci/app_compare/build/app_compare_android.py`

 * *Files identical despite different names*

### Comparing `apf-ci-1.2.180/apf_ci/app_compare/build/app_compare_ios.py` & `apf-ci-1.2.180.1/apf_ci/app_compare/build/app_compare_ios.py`

 * *Files identical despite different names*

### Comparing `apf-ci-1.2.180/apf_ci/app_compare/build/app_compare_utils.py` & `apf-ci-1.2.180.1/apf_ci/app_compare/build/app_compare_utils.py`

 * *Files identical despite different names*

### Comparing `apf-ci-1.2.180/apf_ci/app_compare/build/dependency_utils.py` & `apf-ci-1.2.180.1/apf_ci/app_compare/build/dependency_utils.py`

 * *Files identical despite different names*

### Comparing `apf-ci-1.2.180/apf_ci/app_compare/build/test_app_compare.py` & `apf-ci-1.2.180.1/apf_ci/app_compare/build/test_app_compare.py`

 * *Files identical despite different names*

### Comparing `apf-ci-1.2.180/apf_ci/app_component_compare/build/app_component_compare.py` & `apf-ci-1.2.180.1/apf_ci/app_component_compare/build/app_component_compare.py`

 * *Files identical despite different names*

### Comparing `apf-ci-1.2.180/apf_ci/app_component_compare/build/test_app_component_compare.py` & `apf-ci-1.2.180.1/apf_ci/app_component_compare/build/test_app_component_compare.py`

 * *Files identical despite different names*

### Comparing `apf-ci-1.2.180/apf_ci/app_init/app_config.py` & `apf-ci-1.2.180.1/apf_ci/app_init/app_config.py`

 * *Files identical despite different names*

### Comparing `apf-ci-1.2.180/apf_ci/app_init/app_init.py` & `apf-ci-1.2.180.1/apf_ci/app_init/app_init.py`

 * *Files identical despite different names*

### Comparing `apf-ci-1.2.180/apf_ci/app_init/app_resource.py` & `apf-ci-1.2.180.1/apf_ci/app_init/app_resource.py`

 * *Files identical despite different names*

### Comparing `apf-ci-1.2.180/apf_ci/app_init/test_after_app_init.py` & `apf-ci-1.2.180.1/apf_ci/app_init/test_after_app_init.py`

 * *Files identical despite different names*

### Comparing `apf-ci-1.2.180/apf_ci/app_init/test_app_init.py` & `apf-ci-1.2.180.1/apf_ci/app_init/test_app_init.py`

 * *Files identical despite different names*

### Comparing `apf-ci-1.2.180/apf_ci/app_init/update_variable_json.py` & `apf-ci-1.2.180.1/apf_ci/app_init/update_variable_json.py`

 * *Files identical despite different names*

### Comparing `apf-ci-1.2.180/apf_ci/app_init/utils/appinfo_utils.py` & `apf-ci-1.2.180.1/apf_ci/app_init/utils/appinfo_utils.py`

 * *Files identical despite different names*

### Comparing `apf-ci-1.2.180/apf_ci/app_init/utils/apps_utils.py` & `apf-ci-1.2.180.1/apf_ci/app_init/utils/apps_utils.py`

 * *Files identical despite different names*

### Comparing `apf-ci-1.2.180/apf_ci/app_init/utils/build_config_utils.py` & `apf-ci-1.2.180.1/apf_ci/app_init/utils/build_config_utils.py`

 * *Files identical despite different names*

### Comparing `apf-ci-1.2.180/apf_ci/app_init/utils/image_utils.py` & `apf-ci-1.2.180.1/apf_ci/app_init/utils/image_utils.py`

 * *Files identical despite different names*

### Comparing `apf-ci-1.2.180/apf_ci/app_init/utils/js_third_app_utils.py` & `apf-ci-1.2.180.1/apf_ci/app_init/utils/js_third_app_utils.py`

 * *Files identical despite different names*

### Comparing `apf-ci-1.2.180/apf_ci/app_init/utils/key_chain_utils.py` & `apf-ci-1.2.180.1/apf_ci/app_init/utils/key_chain_utils.py`

 * *Files identical despite different names*

### Comparing `apf-ci-1.2.180/apf_ci/app_init/utils/language_utils.py` & `apf-ci-1.2.180.1/apf_ci/app_init/utils/language_utils.py`

 * *Files identical despite different names*

### Comparing `apf-ci-1.2.180/apf_ci/app_init/utils/variable_utils.py` & `apf-ci-1.2.180.1/apf_ci/app_init/utils/variable_utils.py`

 * *Files identical despite different names*

### Comparing `apf-ci-1.2.180/apf_ci/app_init/utils/variables_script_utils.py` & `apf-ci-1.2.180.1/apf_ci/app_init/utils/variables_script_utils.py`

 * *Files identical despite different names*

### Comparing `apf-ci-1.2.180/apf_ci/app_res/android_plugin.py` & `apf-ci-1.2.180.1/apf_ci/app_res/android_plugin.py`

 * *Files identical despite different names*

### Comparing `apf-ci-1.2.180/apf_ci/app_res/app_res.py` & `apf-ci-1.2.180.1/apf_ci/app_res/app_res.py`

 * *Files identical despite different names*

### Comparing `apf-ci-1.2.180/apf_ci/app_res/language_res.py` & `apf-ci-1.2.180.1/apf_ci/app_res/language_res.py`

 * *Files identical despite different names*

### Comparing `apf-ci-1.2.180/apf_ci/app_res/skin_res.py` & `apf-ci-1.2.180.1/apf_ci/app_res/skin_res.py`

 * *Files identical despite different names*

### Comparing `apf-ci-1.2.180/apf_ci/app_res/test_skin_res.py` & `apf-ci-1.2.180.1/apf_ci/app_res/test_skin_res.py`

 * *Files identical despite different names*

### Comparing `apf-ci-1.2.180/apf_ci/cli.py` & `apf-ci-1.2.180.1/apf_ci/cli.py`

 * *Files identical despite different names*

### Comparing `apf-ci-1.2.180/apf_ci/commands/android_build_prepare.py` & `apf-ci-1.2.180.1/apf_ci/commands/android_build_prepare.py`

 * *Files identical despite different names*

### Comparing `apf-ci-1.2.180/apf_ci/commands/android_prepare.py` & `apf-ci-1.2.180.1/apf_ci/commands/android_prepare.py`

 * *Files identical despite different names*

### Comparing `apf-ci-1.2.180/apf_ci/commands/app_compare.py` & `apf-ci-1.2.180.1/apf_ci/commands/app_compare.py`

 * *Files identical despite different names*

### Comparing `apf-ci-1.2.180/apf_ci/commands/app_component_compare.py` & `apf-ci-1.2.180.1/apf_ci/commands/app_component_compare.py`

 * *Files identical despite different names*

### Comparing `apf-ci-1.2.180/apf_ci/commands/app_init.py` & `apf-ci-1.2.180.1/apf_ci/commands/app_init.py`

 * *Files identical despite different names*

### Comparing `apf-ci-1.2.180/apf_ci/commands/flutter.py` & `apf-ci-1.2.180.1/apf_ci/commands/flutter.py`

 * *Files identical despite different names*

### Comparing `apf-ci-1.2.180/apf_ci/commands/h5_grain.py` & `apf-ci-1.2.180.1/apf_ci/commands/h5_grain.py`

 * *Files identical despite different names*

### Comparing `apf-ci-1.2.180/apf_ci/commands/h5_grain_config.py` & `apf-ci-1.2.180.1/apf_ci/commands/h5_grain_config.py`

 * *Files identical despite different names*

### Comparing `apf-ci-1.2.180/apf_ci/commands/h5_widget_resource.py` & `apf-ci-1.2.180.1/apf_ci/commands/h5_widget_resource.py`

 * *Files identical despite different names*

### Comparing `apf-ci-1.2.180/apf_ci/commands/local_h5.py` & `apf-ci-1.2.180.1/apf_ci/commands/local_h5.py`

 * *Files identical despite different names*

### Comparing `apf-ci-1.2.180/apf_ci/commands/react_widget_resource.py` & `apf-ci-1.2.180.1/apf_ci/commands/react_widget_resource.py`

 * *Files identical despite different names*

### Comparing `apf-ci-1.2.180/apf_ci/commands/rn.py` & `apf-ci-1.2.180.1/apf_ci/commands/rn.py`

 * *Files identical despite different names*

### Comparing `apf-ci-1.2.180/apf_ci/commands/rn_widget.py` & `apf-ci-1.2.180.1/apf_ci/commands/rn_widget.py`

 * *Files identical despite different names*

### Comparing `apf-ci-1.2.180/apf_ci/commands/subapp_config.py` & `apf-ci-1.2.180.1/apf_ci/commands/subapp_config.py`

 * *Files identical despite different names*

### Comparing `apf-ci-1.2.180/apf_ci/commands/tab_build.py` & `apf-ci-1.2.180.1/apf_ci/commands/tab_build.py`

 * *Files identical despite different names*

### Comparing `apf-ci-1.2.180/apf_ci/commands/variable.py` & `apf-ci-1.2.180.1/apf_ci/commands/variable.py`

 * *Files identical despite different names*

### Comparing `apf-ci-1.2.180/apf_ci/config/app_config.py` & `apf-ci-1.2.180.1/apf_ci/config/app_config.py`

 * *Files identical despite different names*

### Comparing `apf-ci-1.2.180/apf_ci/config/biz_comp_transform.py` & `apf-ci-1.2.180.1/apf_ci/config/biz_comp_transform.py`

 * *Files identical despite different names*

### Comparing `apf-ci-1.2.180/apf_ci/config/defines.py` & `apf-ci-1.2.180.1/apf_ci/config/defines.py`

 * *Files identical despite different names*

### Comparing `apf-ci-1.2.180/apf_ci/config/env_service.py` & `apf-ci-1.2.180.1/apf_ci/config/env_service.py`

 * *Files identical despite different names*

### Comparing `apf-ci-1.2.180/apf_ci/config/h5_widget_i18n_utils.py` & `apf-ci-1.2.180.1/apf_ci/config/h5_widget_i18n_utils.py`

 * *Files identical despite different names*

### Comparing `apf-ci-1.2.180/apf_ci/config/json_property_analysis.py` & `apf-ci-1.2.180.1/apf_ci/config/json_property_analysis.py`

 * *Files identical despite different names*

### Comparing `apf-ci-1.2.180/apf_ci/config/language_service.py` & `apf-ci-1.2.180.1/apf_ci/config/language_service.py`

 * *Files identical despite different names*

### Comparing `apf-ci-1.2.180/apf_ci/config/lite_app.py` & `apf-ci-1.2.180.1/apf_ci/config/lite_app.py`

 * *Files identical despite different names*

### Comparing `apf-ci-1.2.180/apf_ci/config/page_attributes.py` & `apf-ci-1.2.180.1/apf_ci/config/page_attributes.py`

 * *Files identical despite different names*

### Comparing `apf-ci-1.2.180/apf_ci/config/page_i18n_utils.py` & `apf-ci-1.2.180.1/apf_ci/config/page_i18n_utils.py`

 * *Files identical despite different names*

### Comparing `apf-ci-1.2.180/apf_ci/config/properties_transform.py` & `apf-ci-1.2.180.1/apf_ci/config/properties_transform.py`

 * *Files identical despite different names*

### Comparing `apf-ci-1.2.180/apf_ci/config/runtime.py` & `apf-ci-1.2.180.1/apf_ci/config/runtime.py`

 * *Files identical despite different names*

### Comparing `apf-ci-1.2.180/apf_ci/config/test/widget_tree_test.py` & `apf-ci-1.2.180.1/apf_ci/config/test/widget_tree_test.py`

 * *Files identical despite different names*

### Comparing `apf-ci-1.2.180/apf_ci/config/widget_i18n_utils.py` & `apf-ci-1.2.180.1/apf_ci/config/widget_i18n_utils.py`

 * *Files identical despite different names*

### Comparing `apf-ci-1.2.180/apf_ci/config/widget_tree.py` & `apf-ci-1.2.180.1/apf_ci/config/widget_tree.py`

 * *Files identical despite different names*

### Comparing `apf-ci-1.2.180/apf_ci/constant/constants.py` & `apf-ci-1.2.180.1/apf_ci/constant/constants.py`

 * *Files identical despite different names*

### Comparing `apf-ci-1.2.180/apf_ci/constant/path_constant.py` & `apf-ci-1.2.180.1/apf_ci/constant/path_constant.py`

 * *Files identical despite different names*

### Comparing `apf-ci-1.2.180/apf_ci/flutter/flutter.py` & `apf-ci-1.2.180.1/apf_ci/flutter/flutter.py`

 * *Files identical despite different names*

### Comparing `apf-ci-1.2.180/apf_ci/flutter/flutter_android_build.py` & `apf-ci-1.2.180.1/apf_ci/flutter/flutter_android_build.py`

 * *Files identical despite different names*

### Comparing `apf-ci-1.2.180/apf_ci/flutter/flutter_build.py` & `apf-ci-1.2.180.1/apf_ci/flutter/flutter_build.py`

 * *Files identical despite different names*

### Comparing `apf-ci-1.2.180/apf_ci/flutter/flutter_command_utils.py` & `apf-ci-1.2.180.1/apf_ci/flutter/flutter_command_utils.py`

 * *Files identical despite different names*

### Comparing `apf-ci-1.2.180/apf_ci/flutter/flutter_ios_build.py` & `apf-ci-1.2.180.1/apf_ci/flutter/flutter_ios_build.py`

 * *Files identical despite different names*

### Comparing `apf-ci-1.2.180/apf_ci/flutter/resource/flutter_language_resource.py` & `apf-ci-1.2.180.1/apf_ci/flutter/resource/flutter_language_resource.py`

 * *Files identical despite different names*

### Comparing `apf-ci-1.2.180/apf_ci/flutter/resource/flutter_resource.py` & `apf-ci-1.2.180.1/apf_ci/flutter/resource/flutter_resource.py`

 * *Files identical despite different names*

### Comparing `apf-ci-1.2.180/apf_ci/flutter/resource/flutter_skin_resource.py` & `apf-ci-1.2.180.1/apf_ci/flutter/resource/flutter_skin_resource.py`

 * *Files identical despite different names*

### Comparing `apf-ci-1.2.180/apf_ci/h5_grain/builder/analysis_pages_builder.py` & `apf-ci-1.2.180.1/apf_ci/h5_grain/builder/analysis_pages_builder.py`

 * *Files identical despite different names*

### Comparing `apf-ci-1.2.180/apf_ci/h5_grain/builder/create_package_builder.py` & `apf-ci-1.2.180.1/apf_ci/h5_grain/builder/create_package_builder.py`

 * *Files identical despite different names*

### Comparing `apf-ci-1.2.180/apf_ci/h5_grain/builder/ensure_template_builder.py` & `apf-ci-1.2.180.1/apf_ci/h5_grain/builder/ensure_template_builder.py`

 * *Files identical despite different names*

### Comparing `apf-ci-1.2.180/apf_ci/h5_grain/builder/h5_grain_builder.py` & `apf-ci-1.2.180.1/apf_ci/h5_grain/builder/h5_grain_builder.py`

 * *Files identical despite different names*

### Comparing `apf-ci-1.2.180/apf_ci/h5_grain/builder/npm_operation_builder.py` & `apf-ci-1.2.180.1/apf_ci/h5_grain/builder/npm_operation_builder.py`

 * *Files identical despite different names*

### Comparing `apf-ci-1.2.180/apf_ci/h5_grain/builder/template_builder.py` & `apf-ci-1.2.180.1/apf_ci/h5_grain/builder/template_builder.py`

 * *Files identical despite different names*

### Comparing `apf-ci-1.2.180/apf_ci/h5_grain/package_model.py` & `apf-ci-1.2.180.1/apf_ci/h5_grain/package_model.py`

 * *Files identical despite different names*

### Comparing `apf-ci-1.2.180/apf_ci/h5_grain_config/h5_grain_config_test.py` & `apf-ci-1.2.180.1/apf_ci/h5_grain_config/h5_grain_config_test.py`

 * *Files identical despite different names*

### Comparing `apf-ci-1.2.180/apf_ci/h5_grain_config/h5_grain_init.py` & `apf-ci-1.2.180.1/apf_ci/h5_grain_config/h5_grain_init.py`

 * *Files identical despite different names*

### Comparing `apf-ci-1.2.180/apf_ci/h5_widget_resource/builder/create_package_builder.py` & `apf-ci-1.2.180.1/apf_ci/h5_widget_resource/builder/create_package_builder.py`

 * *Files identical despite different names*

### Comparing `apf-ci-1.2.180/apf_ci/h5_widget_resource/builder/create_resource_builder.py` & `apf-ci-1.2.180.1/apf_ci/h5_widget_resource/builder/create_resource_builder.py`

 * *Files identical despite different names*

### Comparing `apf-ci-1.2.180/apf_ci/h5_widget_resource/builder/ensure_template_builder.py` & `apf-ci-1.2.180.1/apf_ci/h5_widget_resource/builder/ensure_template_builder.py`

 * *Files identical despite different names*

### Comparing `apf-ci-1.2.180/apf_ci/h5_widget_resource/builder/h5_widget_resource_builder.py` & `apf-ci-1.2.180.1/apf_ci/h5_widget_resource/builder/h5_widget_resource_builder.py`

 * *Files identical despite different names*

### Comparing `apf-ci-1.2.180/apf_ci/init/git_template_service.py` & `apf-ci-1.2.180.1/apf_ci/init/git_template_service.py`

 * *Files identical despite different names*

### Comparing `apf-ci-1.2.180/apf_ci/init/init_global_variable_service.py` & `apf-ci-1.2.180.1/apf_ci/init/init_global_variable_service.py`

 * *Files identical despite different names*

### Comparing `apf-ci-1.2.180/apf_ci/init/validate_service.py` & `apf-ci-1.2.180.1/apf_ci/init/validate_service.py`

 * *Files identical despite different names*

### Comparing `apf-ci-1.2.180/apf_ci/lite_app/cache/abstract_cache.py` & `apf-ci-1.2.180.1/apf_ci/lite_app/cache/abstract_cache.py`

 * *Files identical despite different names*

### Comparing `apf-ci-1.2.180/apf_ci/lite_app/cache/abstract_first_level_cache.py` & `apf-ci-1.2.180.1/apf_ci/lite_app/cache/abstract_first_level_cache.py`

 * *Files identical despite different names*

### Comparing `apf-ci-1.2.180/apf_ci/lite_app/cache/abstract_second_level_cache.py` & `apf-ci-1.2.180.1/apf_ci/lite_app/cache/abstract_second_level_cache.py`

 * *Files identical despite different names*

### Comparing `apf-ci-1.2.180/apf_ci/lite_app/cache/abstract_three_level_cache.py` & `apf-ci-1.2.180.1/apf_ci/lite_app/cache/abstract_three_level_cache.py`

 * *Files identical despite different names*

### Comparing `apf-ci-1.2.180/apf_ci/lite_app/cache/cache_factory.py` & `apf-ci-1.2.180.1/apf_ci/lite_app/cache/cache_factory.py`

 * *Files identical despite different names*

### Comparing `apf-ci-1.2.180/apf_ci/lite_app/cache/factor/abstract_cache_factor.py` & `apf-ci-1.2.180.1/apf_ci/lite_app/cache/factor/abstract_cache_factor.py`

 * *Files identical despite different names*

### Comparing `apf-ci-1.2.180/apf_ci/lite_app/cache/factor/local_h5_cache_factor.py` & `apf-ci-1.2.180.1/apf_ci/lite_app/cache/factor/local_h5_cache_factor.py`

 * *Files identical despite different names*

### Comparing `apf-ci-1.2.180/apf_ci/lite_app/cache/factor/react_cache_factor.py` & `apf-ci-1.2.180.1/apf_ci/lite_app/cache/factor/react_cache_factor.py`

 * *Files identical despite different names*

### Comparing `apf-ci-1.2.180/apf_ci/lite_app/cache/first_level_local_h5_cache.py` & `apf-ci-1.2.180.1/apf_ci/lite_app/cache/first_level_local_h5_cache.py`

 * *Files identical despite different names*

### Comparing `apf-ci-1.2.180/apf_ci/lite_app/cache/first_level_react_cache.py` & `apf-ci-1.2.180.1/apf_ci/lite_app/cache/first_level_react_cache.py`

 * *Files identical despite different names*

### Comparing `apf-ci-1.2.180/apf_ci/lite_app/cache/icache.py` & `apf-ci-1.2.180.1/apf_ci/lite_app/cache/icache.py`

 * *Files identical despite different names*

### Comparing `apf-ci-1.2.180/apf_ci/lite_app/cache/second_level_local_h5_cache.py` & `apf-ci-1.2.180.1/apf_ci/lite_app/cache/second_level_local_h5_cache.py`

 * *Files identical despite different names*

### Comparing `apf-ci-1.2.180/apf_ci/lite_app/cache/second_level_react_cache.py` & `apf-ci-1.2.180.1/apf_ci/lite_app/cache/second_level_react_cache.py`

 * *Files identical despite different names*

### Comparing `apf-ci-1.2.180/apf_ci/lite_app/cache/three_level_local_h5_cache.py` & `apf-ci-1.2.180.1/apf_ci/lite_app/cache/three_level_local_h5_cache.py`

 * *Files identical despite different names*

### Comparing `apf-ci-1.2.180/apf_ci/lite_app/cache/three_level_react_cache.py` & `apf-ci-1.2.180.1/apf_ci/lite_app/cache/three_level_react_cache.py`

 * *Files identical despite different names*

### Comparing `apf-ci-1.2.180/apf_ci/lite_app/concurrent/concurrent_build_client.py` & `apf-ci-1.2.180.1/apf_ci/lite_app/concurrent/concurrent_build_client.py`

 * *Files identical despite different names*

### Comparing `apf-ci-1.2.180/apf_ci/lite_app/local_h5/builder/local_h5_builder.py` & `apf-ci-1.2.180.1/apf_ci/lite_app/local_h5/builder/local_h5_builder.py`

 * *Files identical despite different names*

### Comparing `apf-ci-1.2.180/apf_ci/lite_app/model/cache_bo.py` & `apf-ci-1.2.180.1/apf_ci/lite_app/model/cache_bo.py`

 * *Files identical despite different names*

### Comparing `apf-ci-1.2.180/apf_ci/lite_app/model/cache_factor_bo.py` & `apf-ci-1.2.180.1/apf_ci/lite_app/model/cache_factor_bo.py`

 * *Files identical despite different names*

### Comparing `apf-ci-1.2.180/apf_ci/lite_app/model/js_package_cache.py` & `apf-ci-1.2.180.1/apf_ci/lite_app/model/js_package_cache.py`

 * *Files identical despite different names*

### Comparing `apf-ci-1.2.180/apf_ci/lite_app/model/npm_dto.py` & `apf-ci-1.2.180.1/apf_ci/lite_app/model/npm_dto.py`

 * *Files identical despite different names*

### Comparing `apf-ci-1.2.180/apf_ci/lite_app/parser/abstract_parser.py` & `apf-ci-1.2.180.1/apf_ci/lite_app/parser/abstract_parser.py`

 * *Files identical despite different names*

### Comparing `apf-ci-1.2.180/apf_ci/lite_app/parser/iparser.py` & `apf-ci-1.2.180.1/apf_ci/lite_app/parser/iparser.py`

 * *Files identical despite different names*

### Comparing `apf-ci-1.2.180/apf_ci/lite_app/parser/local_h5_parser.py` & `apf-ci-1.2.180.1/apf_ci/lite_app/parser/local_h5_parser.py`

 * *Files identical despite different names*

### Comparing `apf-ci-1.2.180/apf_ci/lite_app/parser/react_parser.py` & `apf-ci-1.2.180.1/apf_ci/lite_app/parser/react_parser.py`

 * *Files identical despite different names*

### Comparing `apf-ci-1.2.180/apf_ci/lite_app/rn/builder/react_builder.py` & `apf-ci-1.2.180.1/apf_ci/lite_app/rn/builder/react_builder.py`

 * *Files identical despite different names*

### Comparing `apf-ci-1.2.180/apf_ci/lite_app/rn/component.py` & `apf-ci-1.2.180.1/apf_ci/lite_app/rn/component.py`

 * *Files identical despite different names*

### Comparing `apf-ci-1.2.180/apf_ci/lite_app/rn/rn.py` & `apf-ci-1.2.180.1/apf_ci/lite_app/rn/rn.py`

 * *Files identical despite different names*

### Comparing `apf-ci-1.2.180/apf_ci/lite_app/rn/template.py` & `apf-ci-1.2.180.1/apf_ci/lite_app/rn/template.py`

 * *Files identical despite different names*

### Comparing `apf-ci-1.2.180/apf_ci/lite_app/rn/terminal_interaction.py` & `apf-ci-1.2.180.1/apf_ci/lite_app/rn/terminal_interaction.py`

 * *Files identical despite different names*

### Comparing `apf-ci-1.2.180/apf_ci/lite_app/service/apf_service.py` & `apf-ci-1.2.180.1/apf_ci/lite_app/service/apf_service.py`

 * *Files identical despite different names*

### Comparing `apf-ci-1.2.180/apf_ci/lite_app/service/config_service.py` & `apf-ci-1.2.180.1/apf_ci/lite_app/service/config_service.py`

 * *Files identical despite different names*

### Comparing `apf-ci-1.2.180/apf_ci/lite_app/service/local_h5_service.py` & `apf-ci-1.2.180.1/apf_ci/lite_app/service/local_h5_service.py`

 * *Files identical despite different names*

### Comparing `apf-ci-1.2.180/apf_ci/lite_app/service/react_service.py` & `apf-ci-1.2.180.1/apf_ci/lite_app/service/react_service.py`

 * *Files identical despite different names*

### Comparing `apf-ci-1.2.180/apf_ci/react_widget_resource/builder/create_resource_builder.py` & `apf-ci-1.2.180.1/apf_ci/react_widget_resource/builder/create_resource_builder.py`

 * *Files identical despite different names*

### Comparing `apf-ci-1.2.180/apf_ci/react_widget_resource/builder/ensure_template_builder.py` & `apf-ci-1.2.180.1/apf_ci/react_widget_resource/builder/ensure_template_builder.py`

 * *Files identical despite different names*

### Comparing `apf-ci-1.2.180/apf_ci/react_widget_resource/builder/npm_builder.py` & `apf-ci-1.2.180.1/apf_ci/react_widget_resource/builder/npm_builder.py`

 * *Files identical despite different names*

### Comparing `apf-ci-1.2.180/apf_ci/react_widget_resource/builder/react_widget_resource_builder.py` & `apf-ci-1.2.180.1/apf_ci/react_widget_resource/builder/react_widget_resource_builder.py`

 * *Files identical despite different names*

### Comparing `apf-ci-1.2.180/apf_ci/react_widget_resource/builder/rn_resource_analysis_pages_builder.py` & `apf-ci-1.2.180.1/apf_ci/react_widget_resource/builder/rn_resource_analysis_pages_builder.py`

 * *Files identical despite different names*

### Comparing `apf-ci-1.2.180/apf_ci/react_widget_resource/test/test_create_resource_builder.py` & `apf-ci-1.2.180.1/apf_ci/react_widget_resource/test/test_create_resource_builder.py`

 * *Files identical despite different names*

### Comparing `apf-ci-1.2.180/apf_ci/react_widget_resource/test/test_ensure_template_builder.py` & `apf-ci-1.2.180.1/apf_ci/react_widget_resource/test/test_ensure_template_builder.py`

 * *Files identical despite different names*

### Comparing `apf-ci-1.2.180/apf_ci/react_widget_resource/test/test_npm_builder.py` & `apf-ci-1.2.180.1/apf_ci/react_widget_resource/test/test_npm_builder.py`

 * *Files identical despite different names*

### Comparing `apf-ci-1.2.180/apf_ci/react_widget_resource/test/test_rn_resource_analysis_pages_builder.py` & `apf-ci-1.2.180.1/apf_ci/react_widget_resource/test/test_rn_resource_analysis_pages_builder.py`

 * *Files identical despite different names*

### Comparing `apf-ci-1.2.180/apf_ci/resource/cache_service.py` & `apf-ci-1.2.180.1/apf_ci/resource/cache_service.py`

 * *Files identical despite different names*

### Comparing `apf-ci-1.2.180/apf_ci/resource/language.py` & `apf-ci-1.2.180.1/apf_ci/resource/language.py`

 * *Files identical despite different names*

### Comparing `apf-ci-1.2.180/apf_ci/resource/resource_builder.py` & `apf-ci-1.2.180.1/apf_ci/resource/resource_builder.py`

 * *Files identical despite different names*

### Comparing `apf-ci-1.2.180/apf_ci/resource/skin.py` & `apf-ci-1.2.180.1/apf_ci/resource/skin.py`

 * *Files identical despite different names*

### Comparing `apf-ci-1.2.180/apf_ci/resource/test/test_resource_config.py` & `apf-ci-1.2.180.1/apf_ci/resource/test/test_resource_config.py`

 * *Files identical despite different names*

### Comparing `apf-ci-1.2.180/apf_ci/rn_widget/builder/analysis_pages_builder.py` & `apf-ci-1.2.180.1/apf_ci/rn_widget/builder/analysis_pages_builder.py`

 * *Files identical despite different names*

### Comparing `apf-ci-1.2.180/apf_ci/rn_widget/builder/build_tool_builder.py` & `apf-ci-1.2.180.1/apf_ci/rn_widget/builder/build_tool_builder.py`

 * *Files identical despite different names*

### Comparing `apf-ci-1.2.180/apf_ci/rn_widget/builder/check_env_name_builder.py` & `apf-ci-1.2.180.1/apf_ci/rn_widget/builder/check_env_name_builder.py`

 * *Files identical despite different names*

### Comparing `apf-ci-1.2.180/apf_ci/rn_widget/builder/multi_language_resource_builder.py` & `apf-ci-1.2.180.1/apf_ci/rn_widget/builder/multi_language_resource_builder.py`

 * *Files identical despite different names*

### Comparing `apf-ci-1.2.180/apf_ci/rn_widget/builder/npm_operation_builder.py` & `apf-ci-1.2.180.1/apf_ci/rn_widget/builder/npm_operation_builder.py`

 * *Files identical despite different names*

### Comparing `apf-ci-1.2.180/apf_ci/rn_widget/builder/react_widget_builder.py` & `apf-ci-1.2.180.1/apf_ci/rn_widget/builder/react_widget_builder.py`

 * *Files identical despite different names*

### Comparing `apf-ci-1.2.180/apf_ci/rn_widget/builder/templater_builder.py` & `apf-ci-1.2.180.1/apf_ci/rn_widget/builder/templater_builder.py`

 * *Files identical despite different names*

### Comparing `apf-ci-1.2.180/apf_ci/rn_widget/rn_widget.py` & `apf-ci-1.2.180.1/apf_ci/rn_widget/rn_widget.py`

 * *Files identical despite different names*

### Comparing `apf-ci-1.2.180/apf_ci/rn_widget/test/rn_widget_build_test.py` & `apf-ci-1.2.180.1/apf_ci/rn_widget/test/rn_widget_build_test.py`

 * *Files identical despite different names*

### Comparing `apf-ci-1.2.180/apf_ci/rn_widget/test/test_multi_language_resource.py` & `apf-ci-1.2.180.1/apf_ci/rn_widget/test/test_multi_language_resource.py`

 * *Files identical despite different names*

### Comparing `apf-ci-1.2.180/apf_ci/rn_widget/widget.py` & `apf-ci-1.2.180.1/apf_ci/rn_widget/widget.py`

 * *Files identical despite different names*

### Comparing `apf-ci-1.2.180/apf_ci/subapp_config/subapp_config_init.py` & `apf-ci-1.2.180.1/apf_ci/subapp_config/subapp_config_init.py`

 * *Files identical despite different names*

### Comparing `apf-ci-1.2.180/apf_ci/tab/build/tab_build.py` & `apf-ci-1.2.180.1/apf_ci/tab/build/tab_build.py`

 * *Files identical despite different names*

### Comparing `apf-ci-1.2.180/apf_ci/tab/build/tab_init.py` & `apf-ci-1.2.180.1/apf_ci/tab/build/tab_init.py`

 * *Files identical despite different names*

### Comparing `apf-ci-1.2.180/apf_ci/tab/build/test_tab_build.py` & `apf-ci-1.2.180.1/apf_ci/tab/build/test_tab_build.py`

 * *Files identical despite different names*

### Comparing `apf-ci-1.2.180/apf_ci/util/cs_sdk/__init__.py` & `apf-ci-1.2.180.1/apf_ci/util/cs_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `apf-ci-1.2.180/apf_ci/util/cs_sdk/chunk_utils.py` & `apf-ci-1.2.180.1/apf_ci/util/cs_sdk/chunk_utils.py`

 * *Files identical despite different names*

### Comparing `apf-ci-1.2.180/apf_ci/util/cs_sdk/dentry.py` & `apf-ci-1.2.180.1/apf_ci/util/cs_sdk/dentry.py`

 * *Files identical despite different names*

### Comparing `apf-ci-1.2.180/apf_ci/util/cs_sdk/upload_test.py` & `apf-ci-1.2.180.1/apf_ci/util/cs_sdk/upload_test.py`

 * *Files identical despite different names*

### Comparing `apf-ci-1.2.180/apf_ci/util/execute_command_utils.py` & `apf-ci-1.2.180.1/apf_ci/util/execute_command_utils.py`

 * *Files identical despite different names*

### Comparing `apf-ci-1.2.180/apf_ci/util/file_utils.py` & `apf-ci-1.2.180.1/apf_ci/util/file_utils.py`

 * *Files identical despite different names*

### Comparing `apf-ci-1.2.180/apf_ci/util/hook_service.py` & `apf-ci-1.2.180.1/apf_ci/util/hook_service.py`

 * *Files identical despite different names*

### Comparing `apf-ci-1.2.180/apf_ci/util/http_utils.py` & `apf-ci-1.2.180.1/apf_ci/util/http_utils.py`

 * *Files identical despite different names*

### Comparing `apf-ci-1.2.180/apf_ci/util/jenkins_utils.py` & `apf-ci-1.2.180.1/apf_ci/util/jenkins_utils.py`

 * *Files identical despite different names*

### Comparing `apf-ci-1.2.180/apf_ci/util/log_factory/file_write_logger.py` & `apf-ci-1.2.180.1/apf_ci/util/log_factory/file_write_logger.py`

 * *Files identical despite different names*

### Comparing `apf-ci-1.2.180/apf_ci/util/log_factory/ilogger.py` & `apf-ci-1.2.180.1/apf_ci/util/log_factory/ilogger.py`

 * *Files identical despite different names*

### Comparing `apf-ci-1.2.180/apf_ci/util/log_factory/log_error_message.py` & `apf-ci-1.2.180.1/apf_ci/util/log_factory/log_error_message.py`

 * *Files identical despite different names*

### Comparing `apf-ci-1.2.180/apf_ci/util/log_factory/logger_error_enum.py` & `apf-ci-1.2.180.1/apf_ci/util/log_factory/logger_error_enum.py`

 * *Files identical despite different names*

### Comparing `apf-ci-1.2.180/apf_ci/util/log_factory/logger_factory.py` & `apf-ci-1.2.180.1/apf_ci/util/log_factory/logger_factory.py`

 * *Files identical despite different names*

### Comparing `apf-ci-1.2.180/apf_ci/util/log_factory/print_logger.py` & `apf-ci-1.2.180.1/apf_ci/util/log_factory/print_logger.py`

 * *Files identical despite different names*

### Comparing `apf-ci-1.2.180/apf_ci/util/log_utils.py` & `apf-ci-1.2.180.1/apf_ci/util/log_utils.py`

 * *Files identical despite different names*

### Comparing `apf-ci-1.2.180/apf_ci/util/mac_token_utils.py` & `apf-ci-1.2.180.1/apf_ci/util/mac_token_utils.py`

 * *Files identical despite different names*

### Comparing `apf-ci-1.2.180/apf_ci/util/md5_utils.py` & `apf-ci-1.2.180.1/apf_ci/util/md5_utils.py`

 * *Files identical despite different names*

### Comparing `apf-ci-1.2.180/apf_ci/util/private_support_utils.py` & `apf-ci-1.2.180.1/apf_ci/util/private_support_utils.py`

 * *Files identical despite different names*

### Comparing `apf-ci-1.2.180/apf_ci/util/property.py` & `apf-ci-1.2.180.1/apf_ci/util/property.py`

 * *Files identical despite different names*

### Comparing `apf-ci-1.2.180/apf_ci/util/routes_to_json.py` & `apf-ci-1.2.180.1/apf_ci/util/routes_to_json.py`

 * *Files identical despite different names*

### Comparing `apf-ci-1.2.180/apf_ci/util/rsa_utils.py` & `apf-ci-1.2.180.1/apf_ci/util/rsa_utils.py`

 * *Files identical despite different names*

### Comparing `apf-ci-1.2.180/apf_ci/util/uc_sdk/nd_uc_new.py` & `apf-ci-1.2.180.1/apf_ci/util/uc_sdk/nd_uc_new.py`

 * *Files identical despite different names*

### Comparing `apf-ci-1.2.180/apf_ci/util/uc_sdk/nd_uc_new2.py` & `apf-ci-1.2.180.1/apf_ci/util/uc_sdk/nd_uc_new2.py`

 * *Files identical despite different names*

### Comparing `apf-ci-1.2.180/apf_ci/util/uc_sdk/rand.py` & `apf-ci-1.2.180.1/apf_ci/util/uc_sdk/rand.py`

 * *Files identical despite different names*

### Comparing `apf-ci-1.2.180/apf_ci/util/upload_utils.py` & `apf-ci-1.2.180.1/apf_ci/util/upload_utils.py`

 * *Files identical despite different names*

### Comparing `apf-ci-1.2.180/apf_ci/util/version_utils.py` & `apf-ci-1.2.180.1/apf_ci/util/version_utils.py`

 * *Files identical despite different names*

### Comparing `apf-ci-1.2.180/apf_ci.egg-info/PKG-INFO` & `apf-ci-1.2.180.1/apf_ci.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apf-ci
-Version: 1.2.180
+Version: 1.2.180.1
 Summary: App factory apf_ci build script
 Home-page: http://reference.sdp.nd/appfactory/userguide/light/react-native/React%20Native%E6%9C%AC%E5%9C%B0%E8%B0%83%E8%AF%95%E5%B7%A5%E5%85%B7%E4%BD%BF%E7%94%A8%E8%AF%B4%E6%98%8E.html
 Author: Lian Guo Qing
 Author-email: 765789371@qq.com
 License: ND License, Version 1.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `apf-ci-1.2.180/apf_ci.egg-info/SOURCES.txt` & `apf-ci-1.2.180.1/apf_ci.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apf-ci-1.2.180/apf_ci.egg-info/entry_points.txt` & `apf-ci-1.2.180.1/apf_ci.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `apf-ci-1.2.180/data/config.json` & `apf-ci-1.2.180.1/data/config.json`

 * *Files identical despite different names*

### Comparing `apf-ci-1.2.180/data/config_beta.json` & `apf-ci-1.2.180.1/data/config_beta.json`

 * *Files identical despite different names*

### Comparing `apf-ci-1.2.180/data/config_debug.json` & `apf-ci-1.2.180.1/data/config_debug.json`

 * *Files identical despite different names*

### Comparing `apf-ci-1.2.180/data/config_dev.json` & `apf-ci-1.2.180.1/data/config_dev.json`

 * *Files identical despite different names*

### Comparing `apf-ci-1.2.180/setup.py` & `apf-ci-1.2.180.1/setup.py`

 * *Files identical despite different names*

