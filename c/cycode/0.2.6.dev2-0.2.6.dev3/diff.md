# Comparing `tmp/cycode-0.2.6.dev2.tar.gz` & `tmp/cycode-0.2.6.dev3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cycode-0.2.6.dev2.tar", max compression
+gzip compressed data, was "cycode-0.2.6.dev3.tar", max compression
```

## Comparing `cycode-0.2.6.dev2.tar` & `cycode-0.2.6.dev3.tar`

### file list

```diff
@@ -1,62 +1,62 @@
--rw-r--r--   0        0        0    32410 2023-06-23 10:46:05.930227 cycode-0.2.6.dev2/README.md
--rw-r--r--   0        0        0      115 2023-06-23 10:46:36.841831 cycode-0.2.6.dev2/cycode/__init__.py
--rw-r--r--   0        0        0        0 2023-06-23 10:46:05.930227 cycode-0.2.6.dev2/cycode/cli/__init__.py
--rw-r--r--   0        0        0        0 2023-06-23 10:46:05.930227 cycode-0.2.6.dev2/cycode/cli/auth/__init__.py
--rw-r--r--   0        0        0     2813 2023-06-23 10:46:05.930227 cycode-0.2.6.dev2/cycode/cli/auth/auth_command.py
--rw-r--r--   0        0        0     4761 2023-06-23 10:46:05.930227 cycode-0.2.6.dev2/cycode/cli/auth/auth_manager.py
--rw-r--r--   0        0        0     1652 2023-06-23 10:46:05.930227 cycode-0.2.6.dev2/cycode/cli/ci_integrations.py
--rw-r--r--   0        0        0    47480 2023-06-23 10:46:05.930227 cycode-0.2.6.dev2/cycode/cli/code_scanner.py
--rw-r--r--   0        0        0      453 2023-06-23 10:46:05.930227 cycode-0.2.6.dev2/cycode/cli/config.py
--rw-r--r--   0        0        0      387 2023-06-23 10:46:05.930227 cycode-0.2.6.dev2/cycode/cli/config.yaml
--rw-r--r--   0        0        0     5039 2023-06-23 10:46:05.930227 cycode-0.2.6.dev2/cycode/cli/consts.py
--rw-r--r--   0        0        0        0 2023-06-23 10:46:05.930227 cycode-0.2.6.dev2/cycode/cli/exceptions/__init__.py
--rw-r--r--   0        0        0     1698 2023-06-23 10:46:05.930227 cycode-0.2.6.dev2/cycode/cli/exceptions/custom_exceptions.py
--rw-r--r--   0        0        0        0 2023-06-23 10:46:05.930227 cycode-0.2.6.dev2/cycode/cli/helpers/__init__.py
--rw-r--r--   0        0        0        0 2023-06-23 10:46:05.930227 cycode-0.2.6.dev2/cycode/cli/helpers/maven/__init__.py
--rw-r--r--   0        0        0     2196 2023-06-23 10:46:05.930227 cycode-0.2.6.dev2/cycode/cli/helpers/maven/base_restore_maven_dependencies.py
--rw-r--r--   0        0        0      992 2023-06-23 10:46:05.930227 cycode-0.2.6.dev2/cycode/cli/helpers/maven/restore_gradle_dependencies.py
--rw-r--r--   0        0        0     2993 2023-06-23 10:46:05.930227 cycode-0.2.6.dev2/cycode/cli/helpers/maven/restore_maven_dependencies.py
--rw-r--r--   0        0        0     5835 2023-06-23 10:46:05.930227 cycode-0.2.6.dev2/cycode/cli/helpers/sca_code_scanner.py
--rw-r--r--   0        0        0     7243 2023-06-23 10:46:05.930227 cycode-0.2.6.dev2/cycode/cli/main.py
--rw-r--r--   0        0        0     1332 2023-06-23 10:46:05.930227 cycode-0.2.6.dev2/cycode/cli/models.py
--rw-r--r--   0        0        0       93 2023-06-23 10:46:05.930227 cycode-0.2.6.dev2/cycode/cli/printers/__init__.py
--rw-r--r--   0        0        0      626 2023-06-23 10:46:05.930227 cycode-0.2.6.dev2/cycode/cli/printers/base_printer.py
--rw-r--r--   0        0        0     1483 2023-06-23 10:46:05.930227 cycode-0.2.6.dev2/cycode/cli/printers/base_table_printer.py
--rw-r--r--   0        0        0     1891 2023-06-23 10:46:05.930227 cycode-0.2.6.dev2/cycode/cli/printers/console_printer.py
--rw-r--r--   0        0        0     1537 2023-06-23 10:46:05.930227 cycode-0.2.6.dev2/cycode/cli/printers/json_printer.py
--rw-r--r--   0        0        0     5272 2023-06-23 10:46:05.930227 cycode-0.2.6.dev2/cycode/cli/printers/sca_table_printer.py
--rw-r--r--   0        0        0     2277 2023-06-23 10:46:05.930227 cycode-0.2.6.dev2/cycode/cli/printers/table.py
--rw-r--r--   0        0        0      477 2023-06-23 10:46:05.930227 cycode-0.2.6.dev2/cycode/cli/printers/table_models.py
--rw-r--r--   0        0        0     4701 2023-06-23 10:46:05.930227 cycode-0.2.6.dev2/cycode/cli/printers/table_printer.py
--rw-r--r--   0        0        0     8955 2023-06-23 10:46:05.930227 cycode-0.2.6.dev2/cycode/cli/printers/text_printer.py
--rw-r--r--   0        0        0        0 2023-06-23 10:46:05.930227 cycode-0.2.6.dev2/cycode/cli/user_settings/__init__.py
--rw-r--r--   0        0        0      533 2023-06-23 10:46:05.930227 cycode-0.2.6.dev2/cycode/cli/user_settings/base_file_manager.py
--rw-r--r--   0        0        0     4821 2023-06-23 10:46:05.930227 cycode-0.2.6.dev2/cycode/cli/user_settings/config_file_manager.py
--rw-r--r--   0        0        0     6925 2023-06-23 10:46:05.930227 cycode-0.2.6.dev2/cycode/cli/user_settings/configuration_manager.py
--rw-r--r--   0        0        0     1908 2023-06-23 10:46:05.930227 cycode-0.2.6.dev2/cycode/cli/user_settings/credentials_manager.py
--rw-r--r--   0        0        0     6853 2023-06-23 10:46:05.930227 cycode-0.2.6.dev2/cycode/cli/user_settings/user_settings_commands.py
--rw-r--r--   0        0        0        0 2023-06-23 10:46:05.930227 cycode-0.2.6.dev2/cycode/cli/utils/__init__.py
--rw-r--r--   0        0        0     2162 2023-06-23 10:46:05.930227 cycode-0.2.6.dev2/cycode/cli/utils/path_utils.py
--rw-r--r--   0        0        0      195 2023-06-23 10:46:05.930227 cycode-0.2.6.dev2/cycode/cli/utils/scan_utils.py
--rw-r--r--   0        0        0      941 2023-06-23 10:46:05.930227 cycode-0.2.6.dev2/cycode/cli/utils/shell_executor.py
--rw-r--r--   0        0        0     1346 2023-06-23 10:46:05.930227 cycode-0.2.6.dev2/cycode/cli/utils/string_utils.py
--rw-r--r--   0        0        0     2700 2023-06-23 10:46:05.930227 cycode-0.2.6.dev2/cycode/cli/utils/task_timer.py
--rw-r--r--   0        0        0      815 2023-06-23 10:46:05.930227 cycode-0.2.6.dev2/cycode/cli/utils/yaml_utils.py
--rw-r--r--   0        0        0      929 2023-06-23 10:46:05.930227 cycode-0.2.6.dev2/cycode/cli/zip_file.py
--rw-r--r--   0        0        0       57 2023-06-23 10:46:05.930227 cycode-0.2.6.dev2/cycode/cyclient/__init__.py
--rw-r--r--   0        0        0     1708 2023-06-23 10:46:05.930227 cycode-0.2.6.dev2/cycode/cyclient/auth_client.py
--rw-r--r--   0        0        0     2458 2023-06-23 10:46:05.930227 cycode-0.2.6.dev2/cycode/cyclient/config.py
--rw-r--r--   0        0        0      126 2023-06-23 10:46:05.930227 cycode-0.2.6.dev2/cycode/cyclient/config.yaml
--rw-r--r--   0        0        0      119 2023-06-23 10:46:05.930227 cycode-0.2.6.dev2/cycode/cyclient/config_dev.py
--rw-r--r--   0        0        0      220 2023-06-23 10:46:05.930227 cycode-0.2.6.dev2/cycode/cyclient/cycode_client.py
--rw-r--r--   0        0        0     3617 2023-06-23 10:46:05.930227 cycode-0.2.6.dev2/cycode/cyclient/cycode_client_base.py
--rw-r--r--   0        0        0      543 2023-06-23 10:46:05.930227 cycode-0.2.6.dev2/cycode/cyclient/cycode_dev_based_client.py
--rw-r--r--   0        0        0     1705 2023-06-23 10:46:05.930227 cycode-0.2.6.dev2/cycode/cyclient/cycode_token_based_client.py
--rw-r--r--   0        0        0     9102 2023-06-23 10:46:05.930227 cycode-0.2.6.dev2/cycode/cyclient/models.py
--rw-r--r--   0        0        0     6222 2023-06-23 10:46:05.930227 cycode-0.2.6.dev2/cycode/cyclient/scan_client.py
--rw-r--r--   0        0        0        0 2023-06-23 10:46:05.930227 cycode-0.2.6.dev2/cycode/cyclient/scan_config/__init__.py
--rw-r--r--   0        0        0     1090 2023-06-23 10:46:05.930227 cycode-0.2.6.dev2/cycode/cyclient/scan_config/scan_config_base.py
--rw-r--r--   0        0        0     1021 2023-06-23 10:46:05.930227 cycode-0.2.6.dev2/cycode/cyclient/scan_config/scan_config_creator.py
--rw-r--r--   0        0        0      197 2023-06-23 10:46:05.930227 cycode-0.2.6.dev2/cycode/cyclient/utils.py
--rw-r--r--   0        0        0     2032 2023-06-23 10:46:36.837830 cycode-0.2.6.dev2/pyproject.toml
--rw-r--r--   0        0        0    33934 1970-01-01 00:00:00.000000 cycode-0.2.6.dev2/PKG-INFO
+-rw-r--r--   0        0        0    32410 2023-06-27 13:31:14.709250 cycode-0.2.6.dev3/README.md
+-rw-r--r--   0        0        0      115 2023-06-27 13:31:41.125309 cycode-0.2.6.dev3/cycode/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-27 13:31:14.709250 cycode-0.2.6.dev3/cycode/cli/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-27 13:31:14.709250 cycode-0.2.6.dev3/cycode/cli/auth/__init__.py
+-rw-r--r--   0        0        0     2813 2023-06-27 13:31:14.709250 cycode-0.2.6.dev3/cycode/cli/auth/auth_command.py
+-rw-r--r--   0        0        0     4761 2023-06-27 13:31:14.709250 cycode-0.2.6.dev3/cycode/cli/auth/auth_manager.py
+-rw-r--r--   0        0        0     1652 2023-06-27 13:31:14.709250 cycode-0.2.6.dev3/cycode/cli/ci_integrations.py
+-rw-r--r--   0        0        0    47480 2023-06-27 13:31:14.709250 cycode-0.2.6.dev3/cycode/cli/code_scanner.py
+-rw-r--r--   0        0        0      453 2023-06-27 13:31:14.709250 cycode-0.2.6.dev3/cycode/cli/config.py
+-rw-r--r--   0        0        0      387 2023-06-27 13:31:14.709250 cycode-0.2.6.dev3/cycode/cli/config.yaml
+-rw-r--r--   0        0        0     5039 2023-06-27 13:31:14.709250 cycode-0.2.6.dev3/cycode/cli/consts.py
+-rw-r--r--   0        0        0        0 2023-06-27 13:31:14.709250 cycode-0.2.6.dev3/cycode/cli/exceptions/__init__.py
+-rw-r--r--   0        0        0     1698 2023-06-27 13:31:14.709250 cycode-0.2.6.dev3/cycode/cli/exceptions/custom_exceptions.py
+-rw-r--r--   0        0        0        0 2023-06-27 13:31:14.709250 cycode-0.2.6.dev3/cycode/cli/helpers/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-27 13:31:14.709250 cycode-0.2.6.dev3/cycode/cli/helpers/maven/__init__.py
+-rw-r--r--   0        0        0     2196 2023-06-27 13:31:14.709250 cycode-0.2.6.dev3/cycode/cli/helpers/maven/base_restore_maven_dependencies.py
+-rw-r--r--   0        0        0      992 2023-06-27 13:31:14.709250 cycode-0.2.6.dev3/cycode/cli/helpers/maven/restore_gradle_dependencies.py
+-rw-r--r--   0        0        0     2993 2023-06-27 13:31:14.709250 cycode-0.2.6.dev3/cycode/cli/helpers/maven/restore_maven_dependencies.py
+-rw-r--r--   0        0        0     5835 2023-06-27 13:31:14.709250 cycode-0.2.6.dev3/cycode/cli/helpers/sca_code_scanner.py
+-rw-r--r--   0        0        0     7243 2023-06-27 13:31:14.709250 cycode-0.2.6.dev3/cycode/cli/main.py
+-rw-r--r--   0        0        0     1332 2023-06-27 13:31:14.709250 cycode-0.2.6.dev3/cycode/cli/models.py
+-rw-r--r--   0        0        0       93 2023-06-27 13:31:14.709250 cycode-0.2.6.dev3/cycode/cli/printers/__init__.py
+-rw-r--r--   0        0        0      626 2023-06-27 13:31:14.709250 cycode-0.2.6.dev3/cycode/cli/printers/base_printer.py
+-rw-r--r--   0        0        0     1483 2023-06-27 13:31:14.709250 cycode-0.2.6.dev3/cycode/cli/printers/base_table_printer.py
+-rw-r--r--   0        0        0     1891 2023-06-27 13:31:14.709250 cycode-0.2.6.dev3/cycode/cli/printers/console_printer.py
+-rw-r--r--   0        0        0     1537 2023-06-27 13:31:14.709250 cycode-0.2.6.dev3/cycode/cli/printers/json_printer.py
+-rw-r--r--   0        0        0     5838 2023-06-27 13:31:14.709250 cycode-0.2.6.dev3/cycode/cli/printers/sca_table_printer.py
+-rw-r--r--   0        0        0     2277 2023-06-27 13:31:14.709250 cycode-0.2.6.dev3/cycode/cli/printers/table.py
+-rw-r--r--   0        0        0      477 2023-06-27 13:31:14.709250 cycode-0.2.6.dev3/cycode/cli/printers/table_models.py
+-rw-r--r--   0        0        0     4701 2023-06-27 13:31:14.709250 cycode-0.2.6.dev3/cycode/cli/printers/table_printer.py
+-rw-r--r--   0        0        0     8955 2023-06-27 13:31:14.709250 cycode-0.2.6.dev3/cycode/cli/printers/text_printer.py
+-rw-r--r--   0        0        0        0 2023-06-27 13:31:14.709250 cycode-0.2.6.dev3/cycode/cli/user_settings/__init__.py
+-rw-r--r--   0        0        0      533 2023-06-27 13:31:14.709250 cycode-0.2.6.dev3/cycode/cli/user_settings/base_file_manager.py
+-rw-r--r--   0        0        0     4821 2023-06-27 13:31:14.709250 cycode-0.2.6.dev3/cycode/cli/user_settings/config_file_manager.py
+-rw-r--r--   0        0        0     6925 2023-06-27 13:31:14.709250 cycode-0.2.6.dev3/cycode/cli/user_settings/configuration_manager.py
+-rw-r--r--   0        0        0     1908 2023-06-27 13:31:14.709250 cycode-0.2.6.dev3/cycode/cli/user_settings/credentials_manager.py
+-rw-r--r--   0        0        0     6853 2023-06-27 13:31:14.709250 cycode-0.2.6.dev3/cycode/cli/user_settings/user_settings_commands.py
+-rw-r--r--   0        0        0        0 2023-06-27 13:31:14.709250 cycode-0.2.6.dev3/cycode/cli/utils/__init__.py
+-rw-r--r--   0        0        0     2162 2023-06-27 13:31:14.709250 cycode-0.2.6.dev3/cycode/cli/utils/path_utils.py
+-rw-r--r--   0        0        0      195 2023-06-27 13:31:14.709250 cycode-0.2.6.dev3/cycode/cli/utils/scan_utils.py
+-rw-r--r--   0        0        0      941 2023-06-27 13:31:14.709250 cycode-0.2.6.dev3/cycode/cli/utils/shell_executor.py
+-rw-r--r--   0        0        0     1346 2023-06-27 13:31:14.709250 cycode-0.2.6.dev3/cycode/cli/utils/string_utils.py
+-rw-r--r--   0        0        0     2700 2023-06-27 13:31:14.709250 cycode-0.2.6.dev3/cycode/cli/utils/task_timer.py
+-rw-r--r--   0        0        0      815 2023-06-27 13:31:14.709250 cycode-0.2.6.dev3/cycode/cli/utils/yaml_utils.py
+-rw-r--r--   0        0        0      929 2023-06-27 13:31:14.709250 cycode-0.2.6.dev3/cycode/cli/zip_file.py
+-rw-r--r--   0        0        0       57 2023-06-27 13:31:14.709250 cycode-0.2.6.dev3/cycode/cyclient/__init__.py
+-rw-r--r--   0        0        0     1708 2023-06-27 13:31:14.713250 cycode-0.2.6.dev3/cycode/cyclient/auth_client.py
+-rw-r--r--   0        0        0     2458 2023-06-27 13:31:14.713250 cycode-0.2.6.dev3/cycode/cyclient/config.py
+-rw-r--r--   0        0        0      126 2023-06-27 13:31:14.713250 cycode-0.2.6.dev3/cycode/cyclient/config.yaml
+-rw-r--r--   0        0        0      119 2023-06-27 13:31:14.713250 cycode-0.2.6.dev3/cycode/cyclient/config_dev.py
+-rw-r--r--   0        0        0      220 2023-06-27 13:31:14.713250 cycode-0.2.6.dev3/cycode/cyclient/cycode_client.py
+-rw-r--r--   0        0        0     3617 2023-06-27 13:31:14.713250 cycode-0.2.6.dev3/cycode/cyclient/cycode_client_base.py
+-rw-r--r--   0        0        0      543 2023-06-27 13:31:14.713250 cycode-0.2.6.dev3/cycode/cyclient/cycode_dev_based_client.py
+-rw-r--r--   0        0        0     1705 2023-06-27 13:31:14.713250 cycode-0.2.6.dev3/cycode/cyclient/cycode_token_based_client.py
+-rw-r--r--   0        0        0     9102 2023-06-27 13:31:14.713250 cycode-0.2.6.dev3/cycode/cyclient/models.py
+-rw-r--r--   0        0        0     6222 2023-06-27 13:31:14.713250 cycode-0.2.6.dev3/cycode/cyclient/scan_client.py
+-rw-r--r--   0        0        0        0 2023-06-27 13:31:14.713250 cycode-0.2.6.dev3/cycode/cyclient/scan_config/__init__.py
+-rw-r--r--   0        0        0     1090 2023-06-27 13:31:14.713250 cycode-0.2.6.dev3/cycode/cyclient/scan_config/scan_config_base.py
+-rw-r--r--   0        0        0     1021 2023-06-27 13:31:14.713250 cycode-0.2.6.dev3/cycode/cyclient/scan_config/scan_config_creator.py
+-rw-r--r--   0        0        0      197 2023-06-27 13:31:14.713250 cycode-0.2.6.dev3/cycode/cyclient/utils.py
+-rw-r--r--   0        0        0     2032 2023-06-27 13:31:41.121309 cycode-0.2.6.dev3/pyproject.toml
+-rw-r--r--   0        0        0    33934 1970-01-01 00:00:00.000000 cycode-0.2.6.dev3/PKG-INFO
```

### Comparing `cycode-0.2.6.dev2/README.md` & `cycode-0.2.6.dev3/README.md`

 * *Files identical despite different names*

### Comparing `cycode-0.2.6.dev2/cycode/cli/auth/auth_command.py` & `cycode-0.2.6.dev3/cycode/cli/auth/auth_command.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.6.dev2/cycode/cli/auth/auth_manager.py` & `cycode-0.2.6.dev3/cycode/cli/auth/auth_manager.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.6.dev2/cycode/cli/ci_integrations.py` & `cycode-0.2.6.dev3/cycode/cli/ci_integrations.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.6.dev2/cycode/cli/code_scanner.py` & `cycode-0.2.6.dev3/cycode/cli/code_scanner.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.6.dev2/cycode/cli/consts.py` & `cycode-0.2.6.dev3/cycode/cli/consts.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.6.dev2/cycode/cli/exceptions/custom_exceptions.py` & `cycode-0.2.6.dev3/cycode/cli/exceptions/custom_exceptions.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.6.dev2/cycode/cli/helpers/maven/base_restore_maven_dependencies.py` & `cycode-0.2.6.dev3/cycode/cli/helpers/maven/base_restore_maven_dependencies.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.6.dev2/cycode/cli/helpers/maven/restore_gradle_dependencies.py` & `cycode-0.2.6.dev3/cycode/cli/helpers/maven/restore_gradle_dependencies.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.6.dev2/cycode/cli/helpers/maven/restore_maven_dependencies.py` & `cycode-0.2.6.dev3/cycode/cli/helpers/maven/restore_maven_dependencies.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.6.dev2/cycode/cli/helpers/sca_code_scanner.py` & `cycode-0.2.6.dev3/cycode/cli/helpers/sca_code_scanner.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.6.dev2/cycode/cli/main.py` & `cycode-0.2.6.dev3/cycode/cli/main.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.6.dev2/cycode/cli/models.py` & `cycode-0.2.6.dev3/cycode/cli/models.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.6.dev2/cycode/cli/printers/base_printer.py` & `cycode-0.2.6.dev3/cycode/cli/printers/base_printer.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.6.dev2/cycode/cli/printers/base_table_printer.py` & `cycode-0.2.6.dev3/cycode/cli/printers/base_table_printer.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.6.dev2/cycode/cli/printers/console_printer.py` & `cycode-0.2.6.dev3/cycode/cli/printers/console_printer.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.6.dev2/cycode/cli/printers/json_printer.py` & `cycode-0.2.6.dev3/cycode/cli/printers/json_printer.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.6.dev2/cycode/cli/printers/sca_table_printer.py` & `cycode-0.2.6.dev3/cycode/cli/printers/sca_table_printer.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,15 +15,16 @@
 CVE_COLUMN = 'CVE'
 
 PREVIEW_DETECTIONS_COMMON_HEADERS = [
     'File Path',
     'Ecosystem',
     'Dependency Name',
     'Direct Dependency',
-    'Development Dependency'
+    'Development Dependency',
+    'Dependency Paths',
 ]
 
 
 class SCATablePrinter(BaseTablePrinter):
     def _print_results(self, results: List[DocumentDetections]) -> None:
         detections_per_detection_type_id = self._extract_detections_per_detection_type_id(results)
         self._print_detection_per_detection_type_id(detections_per_detection_type_id)
@@ -103,21 +104,36 @@
                 header_width_size_cols.append(header_len)
         text_table.set_cols_width(header_width_size_cols)
 
     @staticmethod
     def _print_summary_issues(detections: List, title: str) -> None:
         click.echo(f'⛔ Found {len(detections)} issues of type: {click.style(title, bold=True)}')
 
+    @staticmethod
+    def _shortcut_dependency_paths(dependency_paths: str) -> str:
+        dependencies = dependency_paths.split(' -> ')
+
+        if len(dependencies) < 2:
+            return dependencies[0]
+
+        return f'{dependencies[0]} -> ... -> {dependencies[-1]}'
+
     def _get_common_detection_fields(self, detection: Detection) -> List[str]:
+        dependency_paths = 'N/A'
+        dependency_paths_raw = detection.detection_details.get('dependency_paths')
+        if dependency_paths_raw:
+            dependency_paths = self._shortcut_dependency_paths(dependency_paths_raw)
+
         row = [
             detection.detection_details.get('file_name'),
             detection.detection_details.get('ecosystem'),
             detection.detection_details.get('package_name'),
             detection.detection_details.get('is_direct_dependency_str'),
-            detection.detection_details.get('is_dev_dependency_str')
+            detection.detection_details.get('is_dev_dependency_str'),
+            dependency_paths,
         ]
 
         if self._is_git_repository():
             row = [detection.detection_details.get('repository_name')] + row
 
         return row
```

### Comparing `cycode-0.2.6.dev2/cycode/cli/printers/table.py` & `cycode-0.2.6.dev3/cycode/cli/printers/table.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.6.dev2/cycode/cli/printers/table_printer.py` & `cycode-0.2.6.dev3/cycode/cli/printers/table_printer.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.6.dev2/cycode/cli/printers/text_printer.py` & `cycode-0.2.6.dev3/cycode/cli/printers/text_printer.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.6.dev2/cycode/cli/user_settings/base_file_manager.py` & `cycode-0.2.6.dev3/cycode/cli/user_settings/base_file_manager.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.6.dev2/cycode/cli/user_settings/config_file_manager.py` & `cycode-0.2.6.dev3/cycode/cli/user_settings/config_file_manager.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.6.dev2/cycode/cli/user_settings/configuration_manager.py` & `cycode-0.2.6.dev3/cycode/cli/user_settings/configuration_manager.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.6.dev2/cycode/cli/user_settings/credentials_manager.py` & `cycode-0.2.6.dev3/cycode/cli/user_settings/credentials_manager.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.6.dev2/cycode/cli/user_settings/user_settings_commands.py` & `cycode-0.2.6.dev3/cycode/cli/user_settings/user_settings_commands.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.6.dev2/cycode/cli/utils/path_utils.py` & `cycode-0.2.6.dev3/cycode/cli/utils/path_utils.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.6.dev2/cycode/cli/utils/shell_executor.py` & `cycode-0.2.6.dev3/cycode/cli/utils/shell_executor.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.6.dev2/cycode/cli/utils/string_utils.py` & `cycode-0.2.6.dev3/cycode/cli/utils/string_utils.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.6.dev2/cycode/cli/utils/task_timer.py` & `cycode-0.2.6.dev3/cycode/cli/utils/task_timer.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.6.dev2/cycode/cli/utils/yaml_utils.py` & `cycode-0.2.6.dev3/cycode/cli/utils/yaml_utils.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.6.dev2/cycode/cli/zip_file.py` & `cycode-0.2.6.dev3/cycode/cli/zip_file.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.6.dev2/cycode/cyclient/auth_client.py` & `cycode-0.2.6.dev3/cycode/cyclient/auth_client.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.6.dev2/cycode/cyclient/config.py` & `cycode-0.2.6.dev3/cycode/cyclient/config.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.6.dev2/cycode/cyclient/cycode_client_base.py` & `cycode-0.2.6.dev3/cycode/cyclient/cycode_client_base.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.6.dev2/cycode/cyclient/cycode_dev_based_client.py` & `cycode-0.2.6.dev3/cycode/cyclient/cycode_dev_based_client.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.6.dev2/cycode/cyclient/cycode_token_based_client.py` & `cycode-0.2.6.dev3/cycode/cyclient/cycode_token_based_client.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.6.dev2/cycode/cyclient/models.py` & `cycode-0.2.6.dev3/cycode/cyclient/models.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.6.dev2/cycode/cyclient/scan_client.py` & `cycode-0.2.6.dev3/cycode/cyclient/scan_client.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.6.dev2/cycode/cyclient/scan_config/scan_config_base.py` & `cycode-0.2.6.dev3/cycode/cyclient/scan_config/scan_config_base.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.6.dev2/cycode/cyclient/scan_config/scan_config_creator.py` & `cycode-0.2.6.dev3/cycode/cyclient/scan_config/scan_config_creator.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.6.dev2/pyproject.toml` & `cycode-0.2.6.dev3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cycode"
-version = "0.2.6.dev2" # DON'T TOUCH. Placeholder. Will be filled automatically on poetry build from Git Tag
+version = "0.2.6.dev3" # DON'T TOUCH. Placeholder. Will be filled automatically on poetry build from Git Tag
 description = "Perform secrets/iac scans for your sources using Cycode's engine"
 keywords=["secret-scan", "cycode", "devops", "token", "secret", "security", "cycode", "code"]
 authors = ["Cycode <support@cycode.com>"]
 license = "MIT"
 repository = "https://github.com/cycodehq-public/cycode-cli"
 readme = "README.md"
 classifiers = [
```

### Comparing `cycode-0.2.6.dev2/PKG-INFO` & `cycode-0.2.6.dev3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cycode
-Version: 0.2.6.dev2
+Version: 0.2.6.dev3
 Summary: Perform secrets/iac scans for your sources using Cycode's engine
 Home-page: https://github.com/cycodehq-public/cycode-cli
 License: MIT
 Keywords: secret-scan,cycode,devops,token,secret,security,cycode,code
 Author: Cycode
 Author-email: support@cycode.com
 Requires-Python: >=3.7,<3.12
```

