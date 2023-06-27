# Comparing `tmp/secureli-0.6.0.tar.gz` & `tmp/secureli-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "secureli-0.6.0.tar", max compression
+gzip compressed data, was "secureli-0.6.1.tar", max compression
```

## Comparing `secureli-0.6.0.tar` & `secureli-0.6.1.tar`

### file list

```diff
@@ -1,52 +1,52 @@
--rw-r--r--   0        0        0    11343 2023-06-27 18:43:27.961636 secureli-0.6.0/LICENSE
--rw-r--r--   0        0        0    11614 2023-06-27 18:43:27.961636 secureli-0.6.0/README.md
--rw-r--r--   0        0        0     2043 2023-06-27 18:43:27.961636 secureli-0.6.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-27 18:43:27.961636 secureli-0.6.0/secureli/__init__.py
--rw-r--r--   0        0        0        0 2023-06-27 18:43:27.961636 secureli-0.6.0/secureli/abstractions/__init__.py
--rw-r--r--   0        0        0     3919 2023-06-27 18:43:27.961636 secureli-0.6.0/secureli/abstractions/echo.py
--rw-r--r--   0        0        0      550 2023-06-27 18:43:27.961636 secureli-0.6.0/secureli/abstractions/lexer_guesser.py
--rw-r--r--   0        0        0    34629 2023-06-27 18:43:27.961636 secureli-0.6.0/secureli/abstractions/pre_commit.py
--rw-r--r--   0        0        0        0 2023-06-27 18:43:27.961636 secureli-0.6.0/secureli/actions/__init__.py
--rw-r--r--   0        0        0    11029 2023-06-27 18:43:27.961636 secureli-0.6.0/secureli/actions/action.py
--rw-r--r--   0        0        0      797 2023-06-27 18:43:27.965636 secureli-0.6.0/secureli/actions/build.py
--rw-r--r--   0        0        0     1186 2023-06-27 18:43:27.965636 secureli-0.6.0/secureli/actions/initializer.py
--rw-r--r--   0        0        0    10670 2023-06-27 18:43:27.965636 secureli-0.6.0/secureli/actions/scan.py
--rw-r--r--   0        0        0      791 2023-06-27 18:43:27.965636 secureli-0.6.0/secureli/actions/setup.py
--rw-r--r--   0        0        0     2205 2023-06-27 18:43:27.965636 secureli-0.6.0/secureli/actions/update.py
--rw-r--r--   0        0        0     6165 2023-06-27 18:43:27.965636 secureli-0.6.0/secureli/container.py
--rw-r--r--   0        0        0     3404 2023-06-27 18:43:27.965636 secureli-0.6.0/secureli/main.py
--rw-r--r--   0        0        0        0 2023-06-27 18:43:27.965636 secureli-0.6.0/secureli/repositories/__init__.py
--rw-r--r--   0        0        0     3685 2023-06-27 18:43:27.965636 secureli-0.6.0/secureli/repositories/repo_files.py
--rw-r--r--   0        0        0     1847 2023-06-27 18:43:27.965636 secureli-0.6.0/secureli/repositories/secureli_config.py
--rw-r--r--   0        0        0     3926 2023-06-27 18:43:27.965636 secureli-0.6.0/secureli/repositories/settings.py
--rw-r--r--   0        0        0       59 2023-06-27 18:43:27.965636 secureli-0.6.0/secureli/resources/__init__.py
--rw-r--r--   0        0        0     4883 2023-06-27 18:43:27.965636 secureli-0.6.0/secureli/resources/files/build.txt
--rw-r--r--   0        0        0       93 2023-06-27 18:43:27.965636 secureli-0.6.0/secureli/resources/files/configs/javascript.config.yaml
--rw-r--r--   0        0        0      161 2023-06-27 18:43:27.965636 secureli-0.6.0/secureli/resources/files/configs/typescript.config.yaml
--rw-r--r--   0        0        0     1271 2023-06-27 18:43:27.965636 secureli-0.6.0/secureli/resources/files/csharp-pre-commit.yaml
--rw-r--r--   0        0        0      461 2023-06-27 18:43:27.965636 secureli-0.6.0/secureli/resources/files/epilog.md
--rw-r--r--   0        0        0      748 2023-06-27 18:43:27.965636 secureli-0.6.0/secureli/resources/files/go-pre-commit.yaml
--rw-r--r--   0        0        0      619 2023-06-27 18:43:27.965636 secureli-0.6.0/secureli/resources/files/java-pre-commit.yaml
--rw-r--r--   0        0        0     1363 2023-06-27 18:43:27.965636 secureli-0.6.0/secureli/resources/files/javascript-pre-commit.yaml
--rw-r--r--   0        0        0     1151 2023-06-27 18:43:27.965636 secureli-0.6.0/secureli/resources/files/python-pre-commit.yaml
--rw-r--r--   0        0        0      356 2023-06-27 18:43:27.965636 secureli-0.6.0/secureli/resources/files/secrets_detecting_repos.yaml
--rw-r--r--   0        0        0      437 2023-06-27 18:43:27.965636 secureli-0.6.0/secureli/resources/files/swift-pre-commit.yaml
--rw-r--r--   0        0        0      433 2023-06-27 18:43:27.965636 secureli-0.6.0/secureli/resources/files/terraform-pre-commit.yaml
--rw-r--r--   0        0        0     1349 2023-06-27 18:43:27.965636 secureli-0.6.0/secureli/resources/files/typescript-pre-commit.yaml
--rw-r--r--   0        0        0      817 2023-06-27 18:43:27.965636 secureli-0.6.0/secureli/resources/read_resource.py
--rw-r--r--   0        0        0     1325 2023-06-27 18:43:27.965636 secureli-0.6.0/secureli/resources/slugify.py
--rw-r--r--   0        0        0        0 2023-06-27 18:43:27.965636 secureli-0.6.0/secureli/services/__init__.py
--rw-r--r--   0        0        0     3646 2023-06-27 18:43:27.965636 secureli-0.6.0/secureli/services/git_ignore.py
--rw-r--r--   0        0        0     3505 2023-06-27 18:43:27.965636 secureli-0.6.0/secureli/services/language_analyzer.py
--rw-r--r--   0        0        0     2332 2023-06-27 18:43:27.965636 secureli-0.6.0/secureli/services/language_support.py
--rw-r--r--   0        0        0     4687 2023-06-27 18:43:27.965636 secureli-0.6.0/secureli/services/logging.py
--rw-r--r--   0        0        0     6374 2023-06-27 18:43:27.965636 secureli-0.6.0/secureli/services/scanner.py
--rw-r--r--   0        0        0     1180 2023-06-27 18:43:27.965636 secureli-0.6.0/secureli/services/secureli_ignore.py
--rw-r--r--   0        0        0     3338 2023-06-27 18:43:27.965636 secureli-0.6.0/secureli/services/updater.py
--rw-r--r--   0        0        0     1482 2023-06-27 18:43:27.965636 secureli-0.6.0/secureli/settings.py
--rw-r--r--   0        0        0        0 2023-06-27 18:43:27.965636 secureli-0.6.0/secureli/utilities/__init__.py
--rw-r--r--   0        0        0     1170 2023-06-27 18:43:27.965636 secureli-0.6.0/secureli/utilities/git_meta.py
--rw-r--r--   0        0        0     1372 2023-06-27 18:43:27.965636 secureli-0.6.0/secureli/utilities/patterns.py
--rw-r--r--   0        0        0      198 2023-06-27 18:43:27.965636 secureli-0.6.0/secureli/utilities/secureli_meta.py
--rw-r--r--   0        0        0     1028 2023-06-27 18:43:27.965636 secureli-0.6.0/secureli/utilities/usage_stats.py
--rw-r--r--   0        0        0    12494 1970-01-01 00:00:00.000000 secureli-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0    11343 2023-06-27 19:39:27.962936 secureli-0.6.1/LICENSE
+-rw-r--r--   0        0        0    11614 2023-06-27 19:39:27.962936 secureli-0.6.1/README.md
+-rw-r--r--   0        0        0     2043 2023-06-27 19:39:27.962936 secureli-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-27 19:39:27.962936 secureli-0.6.1/secureli/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-27 19:39:27.962936 secureli-0.6.1/secureli/abstractions/__init__.py
+-rw-r--r--   0        0        0     3919 2023-06-27 19:39:27.962936 secureli-0.6.1/secureli/abstractions/echo.py
+-rw-r--r--   0        0        0      550 2023-06-27 19:39:27.962936 secureli-0.6.1/secureli/abstractions/lexer_guesser.py
+-rw-r--r--   0        0        0    34252 2023-06-27 19:39:27.962936 secureli-0.6.1/secureli/abstractions/pre_commit.py
+-rw-r--r--   0        0        0        0 2023-06-27 19:39:27.962936 secureli-0.6.1/secureli/actions/__init__.py
+-rw-r--r--   0        0        0    10730 2023-06-27 19:39:27.962936 secureli-0.6.1/secureli/actions/action.py
+-rw-r--r--   0        0        0      761 2023-06-27 19:39:27.962936 secureli-0.6.1/secureli/actions/build.py
+-rw-r--r--   0        0        0     1160 2023-06-27 19:39:27.962936 secureli-0.6.1/secureli/actions/initializer.py
+-rw-r--r--   0        0        0    10628 2023-06-27 19:39:27.962936 secureli-0.6.1/secureli/actions/scan.py
+-rw-r--r--   0        0        0      791 2023-06-27 19:39:27.962936 secureli-0.6.1/secureli/actions/setup.py
+-rw-r--r--   0        0        0     2087 2023-06-27 19:39:27.962936 secureli-0.6.1/secureli/actions/update.py
+-rw-r--r--   0        0        0     6165 2023-06-27 19:39:27.962936 secureli-0.6.1/secureli/container.py
+-rw-r--r--   0        0        0     2807 2023-06-27 19:39:27.962936 secureli-0.6.1/secureli/main.py
+-rw-r--r--   0        0        0        0 2023-06-27 19:39:27.962936 secureli-0.6.1/secureli/repositories/__init__.py
+-rw-r--r--   0        0        0     3685 2023-06-27 19:39:27.962936 secureli-0.6.1/secureli/repositories/repo_files.py
+-rw-r--r--   0        0        0     1752 2023-06-27 19:39:27.962936 secureli-0.6.1/secureli/repositories/secureli_config.py
+-rw-r--r--   0        0        0     3926 2023-06-27 19:39:27.962936 secureli-0.6.1/secureli/repositories/settings.py
+-rw-r--r--   0        0        0       59 2023-06-27 19:39:27.962936 secureli-0.6.1/secureli/resources/__init__.py
+-rw-r--r--   0        0        0     4883 2023-06-27 19:39:27.962936 secureli-0.6.1/secureli/resources/files/build.txt
+-rw-r--r--   0        0        0       93 2023-06-27 19:39:27.962936 secureli-0.6.1/secureli/resources/files/configs/javascript.config.yaml
+-rw-r--r--   0        0        0      161 2023-06-27 19:39:27.962936 secureli-0.6.1/secureli/resources/files/configs/typescript.config.yaml
+-rw-r--r--   0        0        0     1271 2023-06-27 19:39:27.962936 secureli-0.6.1/secureli/resources/files/csharp-pre-commit.yaml
+-rw-r--r--   0        0        0      461 2023-06-27 19:39:27.962936 secureli-0.6.1/secureli/resources/files/epilog.md
+-rw-r--r--   0        0        0      748 2023-06-27 19:39:27.966936 secureli-0.6.1/secureli/resources/files/go-pre-commit.yaml
+-rw-r--r--   0        0        0      619 2023-06-27 19:39:27.966936 secureli-0.6.1/secureli/resources/files/java-pre-commit.yaml
+-rw-r--r--   0        0        0     1363 2023-06-27 19:39:27.966936 secureli-0.6.1/secureli/resources/files/javascript-pre-commit.yaml
+-rw-r--r--   0        0        0     1151 2023-06-27 19:39:27.966936 secureli-0.6.1/secureli/resources/files/python-pre-commit.yaml
+-rw-r--r--   0        0        0      356 2023-06-27 19:39:27.966936 secureli-0.6.1/secureli/resources/files/secrets_detecting_repos.yaml
+-rw-r--r--   0        0        0      437 2023-06-27 19:39:27.966936 secureli-0.6.1/secureli/resources/files/swift-pre-commit.yaml
+-rw-r--r--   0        0        0      433 2023-06-27 19:39:27.966936 secureli-0.6.1/secureli/resources/files/terraform-pre-commit.yaml
+-rw-r--r--   0        0        0     1349 2023-06-27 19:39:27.966936 secureli-0.6.1/secureli/resources/files/typescript-pre-commit.yaml
+-rw-r--r--   0        0        0      817 2023-06-27 19:39:27.966936 secureli-0.6.1/secureli/resources/read_resource.py
+-rw-r--r--   0        0        0     1325 2023-06-27 19:39:27.966936 secureli-0.6.1/secureli/resources/slugify.py
+-rw-r--r--   0        0        0        0 2023-06-27 19:39:27.966936 secureli-0.6.1/secureli/services/__init__.py
+-rw-r--r--   0        0        0     3646 2023-06-27 19:39:27.966936 secureli-0.6.1/secureli/services/git_ignore.py
+-rw-r--r--   0        0        0     3505 2023-06-27 19:39:27.966936 secureli-0.6.1/secureli/services/language_analyzer.py
+-rw-r--r--   0        0        0     2275 2023-06-27 19:39:27.966936 secureli-0.6.1/secureli/services/language_support.py
+-rw-r--r--   0        0        0     4413 2023-06-27 19:39:27.966936 secureli-0.6.1/secureli/services/logging.py
+-rw-r--r--   0        0        0     6374 2023-06-27 19:39:27.966936 secureli-0.6.1/secureli/services/scanner.py
+-rw-r--r--   0        0        0     1180 2023-06-27 19:39:27.966936 secureli-0.6.1/secureli/services/secureli_ignore.py
+-rw-r--r--   0        0        0     3074 2023-06-27 19:39:27.966936 secureli-0.6.1/secureli/services/updater.py
+-rw-r--r--   0        0        0     1482 2023-06-27 19:39:27.966936 secureli-0.6.1/secureli/settings.py
+-rw-r--r--   0        0        0        0 2023-06-27 19:39:27.966936 secureli-0.6.1/secureli/utilities/__init__.py
+-rw-r--r--   0        0        0     1080 2023-06-27 19:39:27.966936 secureli-0.6.1/secureli/utilities/git_meta.py
+-rw-r--r--   0        0        0     1372 2023-06-27 19:39:27.966936 secureli-0.6.1/secureli/utilities/patterns.py
+-rw-r--r--   0        0        0      198 2023-06-27 19:39:27.966936 secureli-0.6.1/secureli/utilities/secureli_meta.py
+-rw-r--r--   0        0        0     1028 2023-06-27 19:39:27.966936 secureli-0.6.1/secureli/utilities/usage_stats.py
+-rw-r--r--   0        0        0    12494 1970-01-01 00:00:00.000000 secureli-0.6.1/PKG-INFO
```

### Comparing `secureli-0.6.0/LICENSE` & `secureli-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `secureli-0.6.0/README.md` & `secureli-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `secureli-0.6.0/pyproject.toml` & `secureli-0.6.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "secureli"
-version = "0.6.0"
+version = "0.6.1"
 description = "Secure Project Manager"
 authors = ["Caleb Tonn <caleb.tonn@slalom.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 
 [tool.poetry.scripts]
 secureli = "secureli.main:app"
```

### Comparing `secureli-0.6.0/secureli/abstractions/echo.py` & `secureli-0.6.1/secureli/abstractions/echo.py`

 * *Files identical despite different names*

### Comparing `secureli-0.6.0/secureli/abstractions/lexer_guesser.py` & `secureli-0.6.1/secureli/abstractions/lexer_guesser.py`

 * *Files identical despite different names*

### Comparing `secureli-0.6.0/secureli/abstractions/pre_commit.py` & `secureli-0.6.1/secureli/abstractions/pre_commit.py`

 * *Files 2% similar despite different names*

```diff
@@ -185,36 +185,37 @@
                 if hook_id in secrets_detecting_repos[repo_name]
             ]
             if secrets_detecting_hooks:
                 return secrets_detecting_hooks[0]
 
         return None
 
-    def install(self, folder_path: Path, language: str) -> InstallResult:
+    def install(self, language: str) -> InstallResult:
         """
         Identifies the template we hold for the specified language, writes it, installs it, and cleans up
         :param language: The language to identify a template for
         :raises LanguageNotSupportedError if a pre-commit template cannot be found for the specified language
         :raises InstallFailedError if the template was found, but an error occurred installing it
         """
-        path_to_pre_commit_file = Path(folder_path / ".pre-commit-config.yaml")
+
+        path_to_pre_commit_file = Path(".pre-commit-config.yaml")
 
         # Raises a LanguageNotSupportedError if language doesn't resolve to a yaml file
         language_config = self._get_language_config(language)
 
         with open(path_to_pre_commit_file, "w") as f:
             f.write(language_config.config_data)
 
-        completed_process = subprocess.run(["pre-commit", "install"], cwd=folder_path)
+        completed_process = subprocess.run(["pre-commit", "install"])
         if completed_process.returncode != 0:
             raise InstallFailedError(
                 f"Installing the pre-commit script for {language} failed"
             )
 
-        install_configs_result = self._install_pre_commit_configs(folder_path, language)
+        install_configs_result = self._install_pre_commit_configs(language)
 
         return InstallResult(
             successful=True,
             version_installed=language_config.version,
             configs_result=install_configs_result,
         )
 
@@ -322,23 +323,21 @@
         if completed_process.returncode != 0:
             return ExecuteResult(successful=False, output=output)
         else:
             return ExecuteResult(successful=True, output=output)
 
     def autoupdate_hooks(
         self,
-        folder_path: Path,
         bleeding_edge: bool = False,
         freeze: bool = False,
         repos: Optional[list] = None,
     ) -> ExecuteResult:
         """
         Updates the precommit hooks but executing precommit's autoupdate command.  Additional info at
         https://pre-commit.com/#pre-commit-autoupdate
-        :param folder path: specified full path directory (default to current directory)
         :param bleeding edge: True if updating to the bleeding edge of the default branch instead of
         the latest tagged version (which is the default behavior)
         :param freeze: Set to True to store "frozen" hashes in rev instead of tag names.
         :param repos: List of repos (url as a string) to update. This is used to target specific repos instead of all repos.
         :return: ExecuteResult, indicating success or failure.
         """
         subprocess_args = [
@@ -364,55 +363,49 @@
                     repo_args.append(arg)
                 else:
                     output = "Unable to update repo, string validation failed. Repo parameter should be a dictionary of strings."
                     return ExecuteResult(successful=False, output=output)
 
             subprocess_args.extend(repo_args)
 
-        completed_process = subprocess.run(
-            subprocess_args, cwd=folder_path, stdout=subprocess.PIPE
-        )
+        completed_process = subprocess.run(subprocess_args, stdout=subprocess.PIPE)
         output = (
             completed_process.stdout.decode("utf8") if completed_process.stdout else ""
         )
         if completed_process.returncode != 0:
             return ExecuteResult(successful=False, output=output)
         else:
             return ExecuteResult(successful=True, output=output)
 
-    def update(self, folder_path: Path) -> ExecuteResult:
+    def update(self) -> ExecuteResult:
         """
         Installs the hooks defined in pre-commit-config.yml.
         :return: ExecuteResult, indicating success or failure.
         """
         subprocess_args = ["pre-commit", "install-hooks", "--color", "always"]
 
-        completed_process = subprocess.run(
-            subprocess_args, cwd=folder_path, stdout=subprocess.PIPE
-        )
+        completed_process = subprocess.run(subprocess_args, stdout=subprocess.PIPE)
         output = (
             completed_process.stdout.decode("utf8") if completed_process.stdout else ""
         )
         if completed_process.returncode != 0:
             return ExecuteResult(successful=False, output=output)
         else:
             return ExecuteResult(successful=True, output=output)
 
-    def remove_unused_hooks(self, folder_path: Path) -> ExecuteResult:
+    def remove_unused_hooks(self) -> ExecuteResult:
         """
         Removes unused hook repos from the cache.  Pre-commit determines which flags are "unused" by comparing
         the repos to the pre-commit-config.yaml file.  Any cached hook repos that are not in the config file
         will be removed from the cache.
         :return: ExecuteResult, indicating success or failure.
         """
         subprocess_args = ["pre-commit", "gc", "--color", "always"]
 
-        completed_process = subprocess.run(
-            subprocess_args, cwd=folder_path, stdout=subprocess.PIPE
-        )
+        completed_process = subprocess.run(subprocess_args, stdout=subprocess.PIPE)
         output = (
             completed_process.stdout.decode("utf8") if completed_process.stdout else ""
         )
         if completed_process.returncode != 0:
             return ExecuteResult(successful=False, output=output)
         else:
             return ExecuteResult(successful=True, output=output)
@@ -822,15 +815,15 @@
             language_configs = yaml.safe_load_all(language_configs_data)
 
             return LoadLanguageConfigsResult(success=True, config_data=language_configs)
 
         return LoadLanguageConfigsResult(success=False, config_data=list())
 
     def _install_pre_commit_configs(
-        self, folder_path: Path, language: str
+        self, language: str
     ) -> LanguagePreCommitConfigInstallResult:
         """
         Install any config files for given language to support any pre-commit commands.
         i.e. Javascript ESLint requires a .eslintrc file to sufficiently use plugins and allow
         for further customization for repo's flavor of Javascript
         :param language: repo language
         :return: LanguagePreCommitConfigInstallResult
@@ -844,21 +837,21 @@
 
         # if successfully loaded any language specific configs
         if language_configs_result.success:
             for config in language_configs_result.config_data:
                 try:
                     for key in config:
                         config_name = f"{slugify(language)}.{key}.yaml"
-                        path_to_config_file = folder_path / f".secureli/{config_name}"
+                        path_to_config_file = Path(f".secureli/{config_name}")
 
                         with open(path_to_config_file, "w") as f:
                             f.write(yaml.dump(config[key]))
 
                         completed_process = subprocess.run(
-                            ["pre-commit", "install-language-config"], cwd=folder_path
+                            ["pre-commit", "install-language-config"]
                         )
 
                         if completed_process.returncode != 0:
                             raise InstallLanguageConfigError(
                                 f"Installing config: {key}, was not successful"
                             )
                         num_configs_wrote += 1
```

### Comparing `secureli-0.6.0/secureli/actions/action.py` & `secureli-0.6.1/secureli/actions/action.py`

 * *Files 6% similar despite different names*

```diff
@@ -83,57 +83,47 @@
         """
         Installs, upgrades or verifies the current SeCureLI installation
         :param folder_path: The folder path to initialize the repo for
         :param reset: If true, disregard existing configuration and start fresh
         :param always_yes: Assume "Yes" to all prompts
         """
 
-        config = (
-            SecureliConfig()
-            if reset
-            else self.action_deps.secureli_config.load(folder_path=folder_path)
-        )
+        config = SecureliConfig() if reset else self.action_deps.secureli_config.load()
 
         if not config.overall_language or not config.version_installed:
             return self._install_secureli(folder_path, always_yes)
         else:
             available_version = self.action_deps.language_support.version_for_language(
                 config.overall_language
             )
 
             # Check for a new version and prompt for upgrade if available
             if available_version != config.version_installed:
-                return self._upgrade_secureli(
-                    folder_path, config, available_version, always_yes
-                )
+                return self._upgrade_secureli(config, available_version, always_yes)
 
             # Validates the current .pre-commit-config.yaml against the generated config
             config_validation_result = self.action_deps.pre_commit.validate_config(
                 language=config.overall_language
             )
 
             # If config mismatch between available version and current version prompt for upgrade
             if not config_validation_result.successful:
                 self.action_deps.echo.print(config_validation_result.output)
-                return self._update_secureli(folder_path, always_yes)
+                return self._update_secureli(always_yes)
 
             self.action_deps.echo.print(
                 f"SeCureLI is installed and up-to-date (language = {config.overall_language})"
             )
             return VerifyResult(
                 outcome=VerifyOutcome.UP_TO_DATE,
                 config=config,
             )
 
     def _upgrade_secureli(
-        self,
-        folder_path: Path,
-        config: SecureliConfig,
-        available_version: str,
-        always_yes: bool,
+        self, config: SecureliConfig, available_version: str, always_yes: bool
     ) -> VerifyResult:
         """
         Installs SeCureLI into the given folder path and returns the new configuration
         :param config: The existing configuration for SeCureLI
         :param available_version: The new version we're upgrading to
         :param always_yes: Assume "Yes" to all prompts
         :return: The new SecureliConfig after upgrade or None if upgrading did not complete
@@ -150,20 +140,20 @@
             return VerifyResult(
                 outcome=VerifyOutcome.UPGRADE_CANCELED,
                 config=config,
             )
 
         try:
             metadata = self.action_deps.language_support.apply_support(
-                folder_path, config.overall_language
+                config.overall_language
             )
 
             # Update config with new version installed and save it
             config.version_installed = metadata.version
-            self.action_deps.secureli_config.save(folder_path, config)
+            self.action_deps.secureli_config.save(config)
             self.action_deps.echo.print("SeCureLI has been upgraded successfully")
             return VerifyResult(
                 outcome=VerifyOutcome.UPGRADE_SUCCEEDED,
                 config=config,
             )
         except InstallFailedError:
             self.action_deps.echo.error(
@@ -211,31 +201,29 @@
                     f"- {language}: {percentage:.0%}", color=Color.MAGENTA, bold=True
                 )
             overall_language = list(analyze_result.language_proportions.keys())[0]
             self.action_deps.echo.print(
                 f"Overall Detected Language: {overall_language}"
             )
 
-            metadata = self.action_deps.language_support.apply_support(
-                folder_path, overall_language
-            )
+            metadata = self.action_deps.language_support.apply_support(overall_language)
 
         except (ValueError, LanguageNotSupportedError, InstallFailedError) as e:
             self.action_deps.echo.error(
                 f"SeCureLI could not be installed due to an error: {str(e)}"
             )
             return VerifyResult(
                 outcome=VerifyOutcome.INSTALL_FAILED,
             )
 
         config = SecureliConfig(
             overall_language=overall_language,
             version_installed=metadata.version,
         )
-        self.action_deps.secureli_config.save(folder_path, config)
+        self.action_deps.secureli_config.save(config)
 
         if secret_test_id := metadata.security_hook_id:
             self.action_deps.echo.print(
                 f"{config.overall_language} supports secrets detection; running {secret_test_id}."
             )
             self.action_deps.scanner.scan_repo(
                 ScanMode.ALL_FILES, specific_test=secret_test_id
@@ -251,15 +239,15 @@
 
         return VerifyResult(
             outcome=VerifyOutcome.INSTALL_SUCCEEDED,
             config=config,
             analyze_result=analyze_result,
         )
 
-    def _update_secureli(self, folder_path: Path, always_yes: bool):
+    def _update_secureli(self, always_yes: bool):
         """
         Prompts the user to update to the latest secureli install.
         :param always_yes: Assume "Yes" to all prompts
         :return: Outcome of update
         """
         update_prompt = "Would you like to update your pre-commit configuration to the latest secureli config?\n"
         update_prompt += "This will reset any manual changes that may have been made to the .pre-commit-config.yaml file.\n"
@@ -268,15 +256,15 @@
             update_prompt, default_response=True
         )
 
         if not update_confirmed:
             self.action_deps.echo.print("\nUpdate declined.\n")
             return VerifyResult(outcome=VerifyOutcome.UPDATE_CANCELED)
 
-        update_result = self.action_deps.updater.update(folder_path)
+        update_result = self.action_deps.updater.update()
         details = update_result.output
         self.action_deps.echo.print(details)
 
         if update_result.successful:
             return VerifyResult(outcome=VerifyOutcome.UPDATE_SUCCEEDED)
         else:
             return VerifyResult(outcome=VerifyOutcome.UPDATE_FAILED)
```

### Comparing `secureli-0.6.0/secureli/actions/build.py` & `secureli-0.6.1/secureli/actions/build.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from pathlib import Path
 from secureli.abstractions.echo import EchoAbstraction, Color
 from secureli.services.logging import LoggingService, LogAction
 
 
 class BuildAction:
     """
     An action responsible for displaying the Securbuild ASCII art in the terminal during the `build` command.
@@ -17,8 +16,8 @@
         """
         Use the provided color and echo service to print the Securbuild to the terminal
         :param color:
         :return:
         """
         self.echo.print(self.build_data, color=color, bold=True)
 
-        self.logging.success(Path("."), LogAction.build)
+        self.logging.success(LogAction.build)
```

### Comparing `secureli-0.6.0/secureli/actions/initializer.py` & `secureli-0.6.1/secureli/actions/initializer.py`

 * *Files 24% similar despite different names*

```diff
@@ -21,10 +21,10 @@
         Initializes SeCureLI for the specified folder path
         :param folder_path: The folder path to initialize the repo for
         :param reset: If true, disregard existing configuration and start fresh
         :param always_yes: Assume "Yes" to all prompts
         """
         verify_result = self.verify_install(folder_path, reset, always_yes)
         if verify_result.outcome in ScanAction.halting_outcomes:
-            self.logging.failure(folder_path, LogAction.init, verify_result.outcome)
+            self.logging.failure(LogAction.init, verify_result.outcome)
         else:
-            self.logging.success(folder_path, LogAction.init)
+            self.logging.success(LogAction.init)
```

### Comparing `secureli-0.6.0/secureli/actions/scan.py` & `secureli-0.6.1/secureli/actions/scan.py`

 * *Files 1% similar despite different names*

```diff
@@ -81,25 +81,24 @@
         )
 
         if failure_count > 0:
             self._process_failures(scan_result.failures, always_yes=always_yes)
 
         if not scan_result.successful:
             log_data = self.logging.failure(
-                folder_path,
                 LogAction.scan,
                 scan_result_failures_json_string,
                 failure_count,
                 individual_failure_count,
             )
 
             post_log(log_data.json(exclude_none=True))
         else:
             self.echo.print("Scan executed successfully and detected no issues!")
-            log_data = self.logging.success(folder_path, LogAction.scan)
+            log_data = self.logging.success(LogAction.scan)
 
             post_log(log_data.json(exclude_none=True))
 
     def _process_failures(
         self,
         failures: list[Failure],
         always_yes: bool,
```

### Comparing `secureli-0.6.0/secureli/actions/setup.py` & `secureli-0.6.1/secureli/actions/setup.py`

 * *Files identical despite different names*

### Comparing `secureli-0.6.0/secureli/actions/update.py` & `secureli-0.6.1/secureli/actions/update.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from typing import Optional
 
-from pathlib import Path
 from secureli.abstractions.echo import EchoAbstraction
 from secureli.services.logging import LoggingService, LogAction
 from secureli.services.updater import UpdaterService
 from secureli.actions.action import Action, ActionDependencies
 
 
 class UpdateAction(Action):
@@ -16,39 +15,39 @@
         updater: UpdaterService,
     ):
         super().__init__(action_deps)
         self.echo = echo
         self.logging = logging
         self.updater = updater
 
-    def update_hooks(self, folder_path: Path, latest: Optional[bool] = False):
+    def update_hooks(self, latest: Optional[bool] = False):
         """
         Installs the hooks defined in pre-commit-config.yml.
         :param latest: Indicates whether you want to update to the latest versions
         of the installed hooks.
         :return: ExecuteResult, indicating success or failure.
         """
         if latest:
             self.echo.print("Updating hooks to the latest version...")
-            update_result = self.updater.update_hooks(folder_path)
+            update_result = self.updater.update_hooks()
             details = (
                 update_result.output
                 or "Unknown output while updating hooks to latest version"
             )
             self.echo.print(details)
             if not update_result.successful:
                 self.echo.print(details)
-                self.logging.failure(folder_path, LogAction.update, details)
+                self.logging.failure(LogAction.update, details)
             else:
                 self.echo.print("Hooks successfully updated to latest version")
-                self.logging.success(folder_path, LogAction.update)
+                self.logging.success(LogAction.update)
         else:
             self.echo.print("Beginning update...")
-            install_result = self.updater.update(folder_path)
+            install_result = self.updater.update()
             details = install_result.output or "Unknown output during hook installation"
             self.echo.print(details)
             if not install_result.successful:
                 self.echo.print(details)
-                self.logging.failure(folder_path, LogAction.update, details)
+                self.logging.failure(LogAction.update, details)
             else:
                 self.echo.print("Update executed successfully.")
-                self.logging.success(folder_path, LogAction.update)
+                self.logging.success(LogAction.update)
```

### Comparing `secureli-0.6.0/secureli/container.py` & `secureli-0.6.1/secureli/container.py`

 * *Files identical despite different names*

### Comparing `secureli-0.6.0/secureli/main.py` & `secureli-0.6.1/secureli/main.py`

 * *Files 18% similar despite different names*

```diff
@@ -44,25 +44,19 @@
     ),
     yes: bool = Option(
         False,
         "--yes",
         "-y",
         help="Say 'yes' to every prompt automatically without input",
     ),
-    directory: Optional[str] = Option(
-        ".",
-        "--directory",
-        "-d",
-        help="Run seCureLI on specified full path directory (default to current directory)",
-    ),
 ):
     """
     Detect languages and initialize pre-commit hooks and linters for the project
     """
-    container.initializer_action().initialize_repo(Path(directory), reset, yes)
+    container.initializer_action().initialize_repo(Path("."), reset, yes)
 
 
 @app.command()
 def scan(
     yes: bool = Option(
         False,
         "--yes",
@@ -77,25 +71,19 @@
     ),
     specific_test: Optional[str] = Option(
         None,
         "--specific-test",
         "-t",
         help="Limit the scan to a specific hook ID from your pre-commit config",
     ),
-    directory: Optional[str] = Option(
-        ".",
-        "--directory",
-        "-d",
-        help="Run seCureLI on specified full path directory (default to current directory)",
-    ),
 ):
     """
     Performs an explicit check of the repository to detect security issues without remote logging.
     """
-    container.scan_action().scan_repo(Path(directory), mode, yes, specific_test)
+    container.scan_action().scan_repo(Path("."), mode, yes, specific_test)
 
 
 @app.command(hidden=True)
 def build(color: Color = Color.BLUE):
     """
     (Easter Egg) Arrange a visit with our fearless security leader!
     """
@@ -105,23 +93,17 @@
 @app.command()
 def update(
     latest: bool = Option(
         False,
         "--latest",
         "-l",
         help="Update the installed pre-commit hooks to their latest versions",
-    ),
-    directory: Optional[str] = Option(
-        ".",
-        "--directory",
-        "-d",
-        help="Run seCureLI on specified full path directory (default to current directory)",
-    ),
+    )
 ):
     """
     Update linters, configuration, and all else needed to maintain a secure repository.
     """
-    container.update_action().update_hooks(Path(directory), latest)
+    container.update_action().update_hooks(latest)
 
 
 if __name__ == "__main__":
     app()
```

### Comparing `secureli-0.6.0/secureli/repositories/repo_files.py` & `secureli-0.6.1/secureli/repositories/repo_files.py`

 * *Files identical despite different names*

### Comparing `secureli-0.6.0/secureli/repositories/secureli_config.py` & `secureli-0.6.1/secureli/repositories/secureli_config.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,41 +9,39 @@
     overall_language: Optional[str]
     version_installed: Optional[str]
 
 
 class SecureliConfigRepository:
     """Save and retrieve the SeCureLI configuration"""
 
-    def save(self, folder_path: Path, secureli_config: SecureliConfig):
+    def save(self, secureli_config: SecureliConfig):
         """
         Save the specified configuration to the .secureli folder
         :param secureli_config: The populated configuration to save
         """
-        secureli_folder_path = self._initialize_secureli_directory(folder_path)
+        secureli_folder_path = self._initialize_secureli_directory()
         secureli_config_path = secureli_folder_path / "repo-config.yaml"
         with open(secureli_config_path, "w") as f:
             yaml.dump(secureli_config.dict(), f)
 
-    def load(self, folder_path: Path) -> SecureliConfig:
+    def load(self) -> SecureliConfig:
         """
         Load the SeCureLI config from the expected configuration file path or return a new
         configuration object, capable of being modified and saved via the `save` method
         """
-        secureli_folder_path = self._initialize_secureli_directory(folder_path)
-        secureli_config_path = Path(secureli_folder_path / "repo-config.yaml")
-
+        secureli_folder_path = self._initialize_secureli_directory()
+        secureli_config_path = secureli_folder_path / "repo-config.yaml"
         if not secureli_config_path.exists():
             return SecureliConfig()
 
         with open(secureli_config_path, "r") as f:
             data = yaml.safe_load(f)
             return SecureliConfig.parse_obj(data)
 
-    def _initialize_secureli_directory(self, folder_path: Path):
+    def _initialize_secureli_directory(self):
         """
         Creates the .secureli folder within the current directory if needed.
         :return: The folder path of the .secureli folder that either exists or was just created.
         """
-        secureli_folder_path = Path(folder_path / ".secureli")
-
+        secureli_folder_path = Path(".") / ".secureli"
         secureli_folder_path.mkdir(parents=True, exist_ok=True)
         return secureli_folder_path
```

### Comparing `secureli-0.6.0/secureli/repositories/settings.py` & `secureli-0.6.1/secureli/repositories/settings.py`

 * *Files identical despite different names*

### Comparing `secureli-0.6.0/secureli/resources/files/build.txt` & `secureli-0.6.1/secureli/resources/files/build.txt`

 * *Files identical despite different names*

### Comparing `secureli-0.6.0/secureli/resources/files/csharp-pre-commit.yaml` & `secureli-0.6.1/secureli/resources/files/csharp-pre-commit.yaml`

 * *Files identical despite different names*

### Comparing `secureli-0.6.0/secureli/resources/files/go-pre-commit.yaml` & `secureli-0.6.1/secureli/resources/files/go-pre-commit.yaml`

 * *Files identical despite different names*

### Comparing `secureli-0.6.0/secureli/resources/files/java-pre-commit.yaml` & `secureli-0.6.1/secureli/resources/files/java-pre-commit.yaml`

 * *Files identical despite different names*

### Comparing `secureli-0.6.0/secureli/resources/files/javascript-pre-commit.yaml` & `secureli-0.6.1/secureli/resources/files/javascript-pre-commit.yaml`

 * *Files identical despite different names*

### Comparing `secureli-0.6.0/secureli/resources/files/python-pre-commit.yaml` & `secureli-0.6.1/secureli/resources/files/python-pre-commit.yaml`

 * *Files identical despite different names*

### Comparing `secureli-0.6.0/secureli/resources/files/typescript-pre-commit.yaml` & `secureli-0.6.1/secureli/resources/files/typescript-pre-commit.yaml`

 * *Files identical despite different names*

### Comparing `secureli-0.6.0/secureli/resources/read_resource.py` & `secureli-0.6.1/secureli/resources/read_resource.py`

 * *Files identical despite different names*

### Comparing `secureli-0.6.0/secureli/resources/slugify.py` & `secureli-0.6.1/secureli/resources/slugify.py`

 * *Files identical despite different names*

### Comparing `secureli-0.6.0/secureli/services/git_ignore.py` & `secureli-0.6.1/secureli/services/git_ignore.py`

 * *Files identical despite different names*

### Comparing `secureli-0.6.0/secureli/services/language_analyzer.py` & `secureli-0.6.1/secureli/services/language_analyzer.py`

 * *Files identical despite different names*

### Comparing `secureli-0.6.0/secureli/services/language_support.py` & `secureli-0.6.1/secureli/services/language_support.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from typing import Optional
 
 import pydantic
 
-from pathlib import Path
 from secureli.abstractions.pre_commit import PreCommitAbstraction
 from secureli.services.git_ignore import GitIgnoreService
 
 supported_languages = [
     "C#",
     "Python",
     "Java",
@@ -43,25 +42,25 @@
         :param language: The language to determine the version of the current config
         :raises LanguageNotSupportedError if support for the language is not provided
         :return: The version of the current config for the provided language available for install
         """
         # For now, just a passthrough to pre-commit hook abstraction
         return self.pre_commit_hook.version_for_language(language)
 
-    def apply_support(self, folder_path: Path, language: str) -> LanguageMetadata:
+    def apply_support(self, language: str) -> LanguageMetadata:
         """
         Applies Secure Build support for the provided language
         :param language: The language to provide support for
         :raises LanguageNotSupportedError if support for the language is not provided
         :return: Metadata including version of the language configuration that was just installed
         as well as a secret-detection hook ID, if present.
         """
 
         # Start by identifying and installing the appropriate pre-commit template (if we have one)
-        install_result = self.pre_commit_hook.install(folder_path, language)
+        install_result = self.pre_commit_hook.install(language)
 
         # Add .secureli/ to the gitignore folder if needed
         self.git_ignore.ignore_secureli_files()
 
         return LanguageMetadata(
             version=install_result.version_installed,
             security_hook_id=self.pre_commit_hook.secret_detection_hook_id(language),
```

### Comparing `secureli-0.6.0/secureli/services/logging.py` & `secureli-0.6.1/secureli/services/logging.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,20 +9,20 @@
 
 from secureli.abstractions.pre_commit import PreCommitAbstraction, HookConfiguration
 from secureli.repositories.secureli_config import SecureliConfigRepository
 from secureli.utilities.git_meta import current_branch_name, git_user_email, origin_url
 from secureli.utilities.secureli_meta import secureli_version
 
 
-def generate_unique_id(folder_path: Path) -> str:
+def generate_unique_id() -> str:
     """
     A unique identifier representing the log entry, including various
     bits specific to the user and environment
     """
-    origin_email_branch = f"{origin_url(folder_path)}|{git_user_email()}|{current_branch_name(folder_path)}"
+    origin_email_branch = f"{origin_url()}|{git_user_email()}|{current_branch_name()}"
     return f"{uuid4()}|{origin_email_branch}"
 
 
 class LogStatus(str, Enum):
     """Whether the entry represents a successful or failing entry"""
 
     success = "SUCCESS"
@@ -43,15 +43,15 @@
 
     details: str
 
 
 class LogEntry(pydantic.BaseModel):
     """A distinct entry in the log captured following actions like scan and init"""
 
-    id: str
+    id: str = generate_unique_id()
     timestamp: datetime = datetime.utcnow()
     username: str = git_user_email()
     machineid: str = platform.uname().node
     secureli_version: str = secureli_version()
     primary_language: Optional[str]
     status: LogStatus
     action: LogAction
@@ -68,75 +68,71 @@
         self,
         pre_commit: PreCommitAbstraction,
         secureli_config: SecureliConfigRepository,
     ):
         self.pre_commit = pre_commit
         self.secureli_config = secureli_config
 
-    def success(self, folder_path: Path, action: LogAction) -> LogEntry:
+    def success(self, action: LogAction) -> LogEntry:
         """
         Capture that a successful conclusion has been reached for an action
         :param action: The action that succeeded
         """
-        secureli_config = self.secureli_config.load(folder_path=folder_path)
+        secureli_config = self.secureli_config.load()
         hook_config = (
             self.pre_commit.get_configuration(secureli_config.overall_language)
             if secureli_config.overall_language
             else None
         )
         log_entry = LogEntry(
-            id=generate_unique_id(folder_path),
             status=LogStatus.success,
             action=action,
             hook_config=hook_config,
             primary_language=secureli_config.overall_language,
         )
-
-        self._log(folder_path, log_entry)
+        self._log(log_entry)
 
         return log_entry
 
     def failure(
         self,
-        folder_path: Path,
         action: LogAction,
         details: str,
         total_failure_count: Optional[int],
         individual_failure_count: Optional[object],
     ) -> LogEntry:
         """
         Capture a failure against an action, with details
         :param action: The action that failed
         :param details: Details about the failure
         """
-        secureli_config = self.secureli_config.load(folder_path=folder_path)
+        secureli_config = self.secureli_config.load()
         hook_config = (
             None
             if not secureli_config.overall_language
             else self.pre_commit.get_configuration(secureli_config.overall_language)
         )
         log_entry = LogEntry(
-            id=generate_unique_id(folder_path),
             status=LogStatus.failure,
             action=action,
             failure=LogFailure(
                 details=details,
             ),
             total_failure_count=total_failure_count,
             failure_count_details=individual_failure_count,
             hook_config=hook_config,
             primary_language=secureli_config.overall_language,
         )
-        self._log(folder_path, log_entry)
+        self._log(log_entry)
 
         return log_entry
 
-    def _log(self, folder_path: Path, log_entry: LogEntry):
+    def _log(self, log_entry: LogEntry):
         """Commit a log entry to the branch log file"""
-        log_folder_path = Path(folder_path / ".secureli/logs")
-        path_to_log = log_folder_path / f"{current_branch_name(folder_path)}"
+        log_folder_path = Path(f".secureli/logs")
+        path_to_log = log_folder_path / f"{current_branch_name()}"
 
         # Do not simply mkdir the log folder path, in case the branch name contains
         # additional folder structure, like `bugfix/` or `feature/`
         path_to_log.parent.mkdir(parents=True, exist_ok=True)
         with open(path_to_log, "a") as f:
             f.writelines([log_entry.json(exclude_none=True) + "\n"])
```

### Comparing `secureli-0.6.0/secureli/services/scanner.py` & `secureli-0.6.1/secureli/services/scanner.py`

 * *Files identical despite different names*

### Comparing `secureli-0.6.0/secureli/services/secureli_ignore.py` & `secureli-0.6.1/secureli/services/secureli_ignore.py`

 * *Files identical despite different names*

### Comparing `secureli-0.6.0/secureli/services/updater.py` & `secureli-0.6.1/secureli/services/updater.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from typing import Optional
 
 import pydantic
 
-from pathlib import Path
 from secureli.abstractions.pre_commit import PreCommitAbstraction
 from secureli.repositories.secureli_config import SecureliConfigRepository
 
 
 class UpdateResult(pydantic.BaseModel):
     """
     The results of calling scan_repo
@@ -27,64 +26,60 @@
         config: SecureliConfigRepository,
     ):
         self.pre_commit = pre_commit
         self.config = config
 
     def update_hooks(
         self,
-        folder_path: Path,
         bleeding_edge: bool = False,
         freeze: bool = False,
         repos: Optional[list] = None,
     ):
         """
         Updates the precommit hooks but executing precommit's autoupdate command.  Additional info at
         https://pre-commit.com/#pre-commit-autoupdate
-        :param folder path: specified full path directory (default to current directory)
         :param bleeding edge: True if updating to the bleeding edge of the default branch instead of
         the latest tagged version (which is the default behavior)
         :param freeze: Set to True to store "frozen" hashes in rev instead of tag names.
         :param repos: Dectionary of repos to update. This is used to target specific repos instead of all repos.
         :return: ExecuteResult, indicating success or failure.
         """
-        update_result = self.pre_commit.autoupdate_hooks(
-            folder_path, bleeding_edge, freeze, repos
-        )
+        update_result = self.pre_commit.autoupdate_hooks(bleeding_edge, freeze, repos)
         output = update_result.output
 
         if update_result.successful and not output:
             output = "No changes necessary.\n"
 
         if update_result.successful and update_result.output:
-            prune_result = self.pre_commit.remove_unused_hooks(folder_path)
+            prune_result = self.pre_commit.remove_unused_hooks()
             output = output + "\nRemoving unused environments:\n" + prune_result.output
 
         return UpdateResult(successful=update_result.successful, output=output)
 
-    def update(self, folder_path: Path):
+    def update(self):
         """
         Updates secureli with the latest local configuration.
         :return: ExecuteResult, indicating success or failure.
         """
-        secureli_config = self.config.load(folder_path)
+        secureli_config = self.config.load()
         output = "Updating .pre-commit-config.yaml...\n"
         install_result = self.pre_commit.install(
-            folder_path=folder_path, language=secureli_config.overall_language
+            language=secureli_config.overall_language
         )
         if not install_result.successful:
             output += "Failed to update .pre-commit-config.yaml prior to hook install\n"
             return UpdateResult(successful=install_result.successful, output=output)
 
-        hook_install_result = self.pre_commit.update(folder_path)
+        hook_install_result = self.pre_commit.update()
         output += hook_install_result.output
 
         if (
             hook_install_result.successful
             and output == "Updating .pre-commit-config.yaml...\n"
         ):
             output += "No changes necessary.\n"
 
         if hook_install_result.successful and hook_install_result.output:
-            prune_result = self.pre_commit.remove_unused_hooks(folder_path)
+            prune_result = self.pre_commit.remove_unused_hooks()
             output += "\nRemoving unused environments:\n" + prune_result.output
 
         return UpdateResult(successful=hook_install_result.successful, output=output)
```

### Comparing `secureli-0.6.0/secureli/settings.py` & `secureli-0.6.1/secureli/settings.py`

 * *Files identical despite different names*

### Comparing `secureli-0.6.0/secureli/utilities/git_meta.py` & `secureli-0.6.1/secureli/utilities/git_meta.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,35 +1,33 @@
-from pathlib import Path
-
 import subprocess
 import configparser
 
 
 def git_user_email() -> str:
     """Leverage the command prompt to derive the user's email address"""
     args = ["git", "config", "user.email"]
     completed_process = subprocess.run(args, stdout=subprocess.PIPE)
     output = completed_process.stdout.decode("utf8").strip()
     return output
 
 
-def origin_url(folder_path: Path) -> str:
+def origin_url() -> str:
     """Leverage the git config file to determine the remote origin URL"""
     git_config_parser = configparser.ConfigParser()
-    git_config_parser.read(f"{folder_path}/.git/config")
+    git_config_parser.read(".git/config")
     return (
         git_config_parser['remote "origin"'].get("url", "UNKNOWN")
         if git_config_parser.has_section('remote "origin"')
         else "UNKNOWN"
     )
 
 
-def current_branch_name(folder_path: Path) -> str:
+def current_branch_name() -> str:
     """Leverage the git HEAD file to determine the current branch name"""
     try:
-        with open(f"{folder_path}/.git/HEAD", "r") as f:
+        with open(".git/HEAD", "r") as f:
             content = f.readlines()
             for line in content:
                 if line[0:4] == "ref:":
                     return line.partition("refs/heads/")[2].strip()
     except IOError:
         return "UNKNOWN"
```

### Comparing `secureli-0.6.0/secureli/utilities/patterns.py` & `secureli-0.6.1/secureli/utilities/patterns.py`

 * *Files identical despite different names*

### Comparing `secureli-0.6.0/secureli/utilities/usage_stats.py` & `secureli-0.6.1/secureli/utilities/usage_stats.py`

 * *Files identical despite different names*

### Comparing `secureli-0.6.0/PKG-INFO` & `secureli-0.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: secureli
-Version: 0.6.0
+Version: 0.6.1
 Summary: Secure Project Manager
 License: Apache-2.0
 Author: Caleb Tonn
 Author-email: caleb.tonn@slalom.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

