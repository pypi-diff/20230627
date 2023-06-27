# Comparing `tmp/pdm-2.8.0a0.tar.gz` & `tmp/pdm-2.8.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdm-2.8.0a0.tar", last modified: Tue Jun 27 02:38:15 2023, max compression
+gzip compressed data, was "pdm-2.8.0a1.tar", last modified: Tue Jun 27 07:57:26 2023, max compression
```

## Comparing `pdm-2.8.0a0.tar` & `pdm-2.8.0a1.tar`

### file list

```diff
@@ -1,280 +1,280 @@
--rw-r--r--   0        0        0   125971 2023-06-27 02:38:06.416159 pdm-2.8.0a0/CHANGELOG.md
--rw-r--r--   0        0        0     1075 2023-06-27 02:38:06.416159 pdm-2.8.0a0/LICENSE
--rw-r--r--   0        0        0     1075 2023-06-27 02:38:06.416159 pdm-2.8.0a0/LICENSE
--rw-r--r--   0        0        0     7937 2023-06-27 02:38:06.416159 pdm-2.8.0a0/README.md
--rw-r--r--   0        0        0     7937 2023-06-27 02:38:06.416159 pdm-2.8.0a0/README.md
--rw-r--r--   0        0        0     4454 2023-06-27 02:38:15.224328 pdm-2.8.0a0/pyproject.toml
--rw-r--r--   0        0        0       65 2023-06-27 02:38:06.420159 pdm-2.8.0a0/src/pdm/__main__.py
--rw-r--r--   0        0        0      316 2023-06-27 02:38:06.420159 pdm-2.8.0a0/src/pdm/__version__.py
--rw-r--r--   0        0        0     3282 2023-06-27 02:38:06.420159 pdm-2.8.0a0/src/pdm/_types.py
--rw-r--r--   0        0        0      237 2023-06-27 02:38:06.420159 pdm-2.8.0a0/src/pdm/builders/__init__.py
--rw-r--r--   0        0        0    11850 2023-06-27 02:38:06.420159 pdm-2.8.0a0/src/pdm/builders/base.py
--rw-r--r--   0        0        0     1755 2023-06-27 02:38:06.420159 pdm-2.8.0a0/src/pdm/builders/editable.py
--rw-r--r--   0        0        0      656 2023-06-27 02:38:06.420159 pdm-2.8.0a0/src/pdm/builders/sdist.py
--rw-r--r--   0        0        0     1073 2023-06-27 02:38:06.420159 pdm-2.8.0a0/src/pdm/builders/wheel.py
--rw-r--r--   0        0        0        0 2023-06-27 02:38:06.420159 pdm-2.8.0a0/src/pdm/cli/__init__.py
--rw-r--r--   0        0        0    16131 2023-06-27 02:38:06.420159 pdm-2.8.0a0/src/pdm/cli/actions.py
--rw-r--r--   0        0        0        0 2023-06-27 02:38:06.420159 pdm-2.8.0a0/src/pdm/cli/commands/__init__.py
--rw-r--r--   0        0        0     7104 2023-06-27 02:38:06.420159 pdm-2.8.0a0/src/pdm/cli/commands/add.py
--rw-r--r--   0        0        0     2857 2023-06-27 02:38:06.420159 pdm-2.8.0a0/src/pdm/cli/commands/base.py
--rw-r--r--   0        0        0     4236 2023-06-27 02:38:06.424159 pdm-2.8.0a0/src/pdm/cli/commands/build.py
--rw-r--r--   0        0        0     6542 2023-06-27 02:38:06.424159 pdm-2.8.0a0/src/pdm/cli/commands/cache.py
--rw-r--r--   0        0        0     1324 2023-06-27 02:38:06.424159 pdm-2.8.0a0/src/pdm/cli/commands/completion.py
--rw-r--r--   0        0        0     7165 2023-06-27 02:38:06.424159 pdm-2.8.0a0/src/pdm/cli/commands/config.py
--rw-r--r--   0        0        0     3066 2023-06-27 02:38:06.424159 pdm-2.8.0a0/src/pdm/cli/commands/export.py
--rw-r--r--   0        0        0     3136 2023-06-27 02:38:06.424159 pdm-2.8.0a0/src/pdm/cli/commands/fix/__init__.py
--rw-r--r--   0        0        0     2309 2023-06-27 02:38:06.424159 pdm-2.8.0a0/src/pdm/cli/commands/fix/fixers.py
--rw-r--r--   0        0        0     3689 2023-06-27 02:38:06.424159 pdm-2.8.0a0/src/pdm/cli/commands/import_cmd.py
--rw-r--r--   0        0        0     3032 2023-06-27 02:38:06.424159 pdm-2.8.0a0/src/pdm/cli/commands/info.py
--rw-r--r--   0        0        0     7605 2023-06-27 02:38:06.424159 pdm-2.8.0a0/src/pdm/cli/commands/init.py
--rw-r--r--   0        0        0     3589 2023-06-27 02:38:06.424159 pdm-2.8.0a0/src/pdm/cli/commands/install.py
--rw-r--r--   0        0        0    15754 2023-06-27 02:38:06.424159 pdm-2.8.0a0/src/pdm/cli/commands/list.py
--rw-r--r--   0        0        0     2196 2023-06-27 02:38:06.424159 pdm-2.8.0a0/src/pdm/cli/commands/lock.py
--rw-r--r--   0        0        0     6596 2023-06-27 02:38:06.424159 pdm-2.8.0a0/src/pdm/cli/commands/publish/__init__.py
--rw-r--r--   0        0        0     8112 2023-06-27 02:38:06.424159 pdm-2.8.0a0/src/pdm/cli/commands/publish/package.py
--rw-r--r--   0        0        0     6782 2023-06-27 02:38:06.424159 pdm-2.8.0a0/src/pdm/cli/commands/publish/repository.py
--rw-r--r--   0        0        0     4271 2023-06-27 02:38:06.424159 pdm-2.8.0a0/src/pdm/cli/commands/remove.py
--rw-r--r--   0        0        0    15489 2023-06-27 02:38:06.424159 pdm-2.8.0a0/src/pdm/cli/commands/run.py
--rw-r--r--   0        0        0     2436 2023-06-27 02:38:06.424159 pdm-2.8.0a0/src/pdm/cli/commands/search.py
--rw-r--r--   0        0        0     9370 2023-06-27 02:38:06.424159 pdm-2.8.0a0/src/pdm/cli/commands/self_cmd.py
--rw-r--r--   0        0        0     2896 2023-06-27 02:38:06.424159 pdm-2.8.0a0/src/pdm/cli/commands/show.py
--rw-r--r--   0        0        0     1447 2023-06-27 02:38:06.424159 pdm-2.8.0a0/src/pdm/cli/commands/sync.py
--rw-r--r--   0        0        0     6898 2023-06-27 02:38:06.424159 pdm-2.8.0a0/src/pdm/cli/commands/update.py
--rw-r--r--   0        0        0     6489 2023-06-27 02:38:06.424159 pdm-2.8.0a0/src/pdm/cli/commands/use.py
--rw-r--r--   0        0        0     1723 2023-06-27 02:38:06.424159 pdm-2.8.0a0/src/pdm/cli/commands/venv/__init__.py
--rw-r--r--   0        0        0     2426 2023-06-27 02:38:06.424159 pdm-2.8.0a0/src/pdm/cli/commands/venv/activate.py
--rw-r--r--   0        0        0     6149 2023-06-27 02:38:06.424159 pdm-2.8.0a0/src/pdm/cli/commands/venv/backends.py
--rw-r--r--   0        0        0     2155 2023-06-27 02:38:06.424159 pdm-2.8.0a0/src/pdm/cli/commands/venv/create.py
--rw-r--r--   0        0        0      819 2023-06-27 02:38:06.424159 pdm-2.8.0a0/src/pdm/cli/commands/venv/list.py
--rw-r--r--   0        0        0     2195 2023-06-27 02:38:06.424159 pdm-2.8.0a0/src/pdm/cli/commands/venv/purge.py
--rw-r--r--   0        0        0     1279 2023-06-27 02:38:06.424159 pdm-2.8.0a0/src/pdm/cli/commands/venv/remove.py
--rw-r--r--   0        0        0     2759 2023-06-27 02:38:06.424159 pdm-2.8.0a0/src/pdm/cli/commands/venv/utils.py
--rw-r--r--   0        0        0        0 2023-06-27 02:38:06.424159 pdm-2.8.0a0/src/pdm/cli/completions/__init__.py
--rw-r--r--   0        0        0     5113 2023-06-27 02:38:06.424159 pdm-2.8.0a0/src/pdm/cli/completions/pdm.bash
--rw-r--r--   0        0        0    50280 2023-06-27 02:38:06.424159 pdm-2.8.0a0/src/pdm/cli/completions/pdm.fish
--rw-r--r--   0        0        0    18599 2023-06-27 02:38:06.424159 pdm-2.8.0a0/src/pdm/cli/completions/pdm.ps1
--rw-r--r--   0        0        0    25289 2023-06-27 02:38:06.424159 pdm-2.8.0a0/src/pdm/cli/completions/pdm.zsh
--rw-r--r--   0        0        0     3840 2023-06-27 02:38:06.424159 pdm-2.8.0a0/src/pdm/cli/filters.py
--rw-r--r--   0        0        0     1481 2023-06-27 02:38:06.424159 pdm-2.8.0a0/src/pdm/cli/hooks.py
--rw-r--r--   0        0        0    10461 2023-06-27 02:38:06.424159 pdm-2.8.0a0/src/pdm/cli/options.py
--rw-r--r--   0        0        0     6235 2023-06-27 02:38:06.424159 pdm-2.8.0a0/src/pdm/cli/templates/__init__.py
--rw-r--r--   0        0        0     3102 2023-06-27 02:38:06.424159 pdm-2.8.0a0/src/pdm/cli/templates/default/.gitignore
--rw-r--r--   0        0        0       18 2023-06-27 02:38:06.424159 pdm-2.8.0a0/src/pdm/cli/templates/default/README.md
--rw-r--r--   0        0        0        0 2023-06-27 02:38:06.424159 pdm-2.8.0a0/src/pdm/cli/templates/default/__init__.py
--rw-r--r--   0        0        0      278 2023-06-27 02:38:06.424159 pdm-2.8.0a0/src/pdm/cli/templates/default/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-27 02:38:06.424159 pdm-2.8.0a0/src/pdm/cli/templates/default/src/example_package/__init__.py
--rw-r--r--   0        0        0        0 2023-06-27 02:38:06.424159 pdm-2.8.0a0/src/pdm/cli/templates/default/tests/__init__.py
--rw-r--r--   0        0        0    25152 2023-06-27 02:38:06.424159 pdm-2.8.0a0/src/pdm/cli/utils.py
--rw-r--r--   0        0        0     2373 2023-06-27 02:38:06.424159 pdm-2.8.0a0/src/pdm/compat.py
--rw-r--r--   0        0        0    10667 2023-06-27 02:38:06.424159 pdm-2.8.0a0/src/pdm/core.py
--rw-r--r--   0        0        0      825 2023-06-27 02:38:06.424159 pdm-2.8.0a0/src/pdm/environments/__init__.py
--rw-r--r--   0        0        0     8850 2023-06-27 02:38:06.424159 pdm-2.8.0a0/src/pdm/environments/base.py
--rw-r--r--   0        0        0     4255 2023-06-27 02:38:06.424159 pdm-2.8.0a0/src/pdm/environments/local.py
--rw-r--r--   0        0        0     1600 2023-06-27 02:38:06.424159 pdm-2.8.0a0/src/pdm/environments/python.py
--rw-r--r--   0        0        0     1362 2023-06-27 02:38:06.424159 pdm-2.8.0a0/src/pdm/exceptions.py
--rw-r--r--   0        0        0     1202 2023-06-27 02:38:06.424159 pdm-2.8.0a0/src/pdm/formats/__init__.py
--rw-r--r--   0        0        0     3215 2023-06-27 02:38:06.424159 pdm-2.8.0a0/src/pdm/formats/base.py
--rw-r--r--   0        0        0     5788 2023-06-27 02:38:06.424159 pdm-2.8.0a0/src/pdm/formats/flit.py
--rw-r--r--   0        0        0     2614 2023-06-27 02:38:06.424159 pdm-2.8.0a0/src/pdm/formats/pipfile.py
--rw-r--r--   0        0        0     7490 2023-06-27 02:38:06.424159 pdm-2.8.0a0/src/pdm/formats/poetry.py
--rw-r--r--   0        0        0     7502 2023-06-27 02:38:06.424159 pdm-2.8.0a0/src/pdm/formats/requirements.py
--rw-r--r--   0        0        0     2309 2023-06-27 02:38:06.428159 pdm-2.8.0a0/src/pdm/formats/setup_py.py
--rw-r--r--   0        0        0      119 2023-06-27 02:38:06.428159 pdm-2.8.0a0/src/pdm/installers/__init__.py
--rw-r--r--   0        0        0     1390 2023-06-27 02:38:06.428159 pdm-2.8.0a0/src/pdm/installers/core.py
--rw-r--r--   0        0        0    10901 2023-06-27 02:38:06.428159 pdm-2.8.0a0/src/pdm/installers/installers.py
--rw-r--r--   0        0        0     2091 2023-06-27 02:38:06.428159 pdm-2.8.0a0/src/pdm/installers/manager.py
--rw-r--r--   0        0        0     2226 2023-06-27 02:38:06.428159 pdm-2.8.0a0/src/pdm/installers/packages.py
--rw-r--r--   0        0        0    18161 2023-06-27 02:38:06.428159 pdm-2.8.0a0/src/pdm/installers/synchronizers.py
--rw-r--r--   0        0        0    10990 2023-06-27 02:38:06.428159 pdm-2.8.0a0/src/pdm/installers/uninstallers.py
--rw-r--r--   0        0        0        0 2023-06-27 02:38:06.428159 pdm-2.8.0a0/src/pdm/models/__init__.py
--rw-r--r--   0        0        0     3162 2023-06-27 02:38:06.428159 pdm-2.8.0a0/src/pdm/models/auth.py
--rw-r--r--   0        0        0     4698 2023-06-27 02:38:06.428159 pdm-2.8.0a0/src/pdm/models/backends.py
--rw-r--r--   0        0        0    11710 2023-06-27 02:38:06.428159 pdm-2.8.0a0/src/pdm/models/caches.py
--rw-r--r--   0        0        0    26580 2023-06-27 02:38:06.428159 pdm-2.8.0a0/src/pdm/models/candidates.py
--rw-r--r--   0        0        0      287 2023-06-27 02:38:06.428159 pdm-2.8.0a0/src/pdm/models/environment.py
--rw-r--r--   0        0        0     1845 2023-06-27 02:38:06.428159 pdm-2.8.0a0/src/pdm/models/in_process/__init__.py
--rw-r--r--   0        0        0     2049 2023-06-27 02:38:06.428159 pdm-2.8.0a0/src/pdm/models/in_process/get_abi_tag.py
--rw-r--r--   0        0        0     6323 2023-06-27 02:38:06.428159 pdm-2.8.0a0/src/pdm/models/in_process/parse_setup.py
--rw-r--r--   0        0        0     1165 2023-06-27 02:38:06.428159 pdm-2.8.0a0/src/pdm/models/in_process/pep508.py
--rw-r--r--   0        0        0     1653 2023-06-27 02:38:06.428159 pdm-2.8.0a0/src/pdm/models/in_process/sysconfig_get_paths.py
--rw-r--r--   0        0        0     5701 2023-06-27 02:38:06.428159 pdm-2.8.0a0/src/pdm/models/markers.py
--rw-r--r--   0        0        0     3507 2023-06-27 02:38:06.428159 pdm-2.8.0a0/src/pdm/models/project_info.py
--rw-r--r--   0        0        0     2195 2023-06-27 02:38:06.428159 pdm-2.8.0a0/src/pdm/models/python.py
--rw-r--r--   0        0        0      318 2023-06-27 02:38:06.428159 pdm-2.8.0a0/src/pdm/models/python_max_versions.json
--rw-r--r--   0        0        0    21340 2023-06-27 02:38:06.428159 pdm-2.8.0a0/src/pdm/models/repositories.py
--rw-r--r--   0        0        0    18792 2023-06-27 02:38:06.428159 pdm-2.8.0a0/src/pdm/models/requirements.py
--rw-r--r--   0        0        0     2313 2023-06-27 02:38:06.428159 pdm-2.8.0a0/src/pdm/models/search.py
--rw-r--r--   0        0        0     3225 2023-06-27 02:38:06.428159 pdm-2.8.0a0/src/pdm/models/session.py
--rw-r--r--   0        0        0    14482 2023-06-27 02:38:06.428159 pdm-2.8.0a0/src/pdm/models/setup.py
--rw-r--r--   0        0        0    16337 2023-06-27 02:38:06.428159 pdm-2.8.0a0/src/pdm/models/specifiers.py
--rw-r--r--   0        0        0     1300 2023-06-27 02:38:06.428159 pdm-2.8.0a0/src/pdm/models/venv.py
--rw-r--r--   0        0        0     5924 2023-06-27 02:38:06.428159 pdm-2.8.0a0/src/pdm/models/versions.py
--rw-r--r--   0        0        0     2766 2023-06-27 02:38:06.428159 pdm-2.8.0a0/src/pdm/models/working_set.py
--rw-r--r--   0        0        0        0 2023-06-27 02:38:06.428159 pdm-2.8.0a0/src/pdm/pep582/__init__.py
--rw-r--r--   0        0        0     4481 2023-06-27 02:38:06.428159 pdm-2.8.0a0/src/pdm/pep582/sitecustomize.py
--rw-r--r--   0        0        0      134 2023-06-27 02:38:06.428159 pdm-2.8.0a0/src/pdm/project/__init__.py
--rw-r--r--   0        0        0    16757 2023-06-27 02:38:06.428159 pdm-2.8.0a0/src/pdm/project/config.py
--rw-r--r--   0        0        0    26292 2023-06-27 02:38:06.428159 pdm-2.8.0a0/src/pdm/project/core.py
--rw-r--r--   0        0        0     2093 2023-06-27 02:38:06.428159 pdm-2.8.0a0/src/pdm/project/lockfile.py
--rw-r--r--   0        0        0     3385 2023-06-27 02:38:06.428159 pdm-2.8.0a0/src/pdm/project/project_file.py
--rw-r--r--   0        0        0     1070 2023-06-27 02:38:06.428159 pdm-2.8.0a0/src/pdm/project/toml_file.py
--rw-r--r--   0        0        0        0 2023-06-27 02:38:06.428159 pdm-2.8.0a0/src/pdm/py.typed
--rw-r--r--   0        0        0    20185 2023-06-27 02:38:06.428159 pdm-2.8.0a0/src/pdm/pytest.py
--rw-r--r--   0        0        0       61 2023-06-27 02:38:06.428159 pdm-2.8.0a0/src/pdm/resolver/__init__.py
--rw-r--r--   0        0        0     1954 2023-06-27 02:38:06.428159 pdm-2.8.0a0/src/pdm/resolver/core.py
--rw-r--r--   0        0        0    13176 2023-06-27 02:38:06.428159 pdm-2.8.0a0/src/pdm/resolver/providers.py
--rw-r--r--   0        0        0     1580 2023-06-27 02:38:06.428159 pdm-2.8.0a0/src/pdm/resolver/python.py
--rw-r--r--   0        0        0     3742 2023-06-27 02:38:06.428159 pdm-2.8.0a0/src/pdm/resolver/reporters.py
--rw-r--r--   0        0        0     4027 2023-06-27 02:38:06.428159 pdm-2.8.0a0/src/pdm/signals.py
--rw-r--r--   0        0        0     8054 2023-06-27 02:38:06.428159 pdm-2.8.0a0/src/pdm/termui.py
--rw-r--r--   0        0        0    13856 2023-06-27 02:38:06.428159 pdm-2.8.0a0/src/pdm/utils.py
--rw-r--r--   0        0        0       72 2023-06-27 02:38:06.428159 pdm-2.8.0a0/tests/__init__.py
--rw-r--r--   0        0        0        0 2023-06-27 02:38:06.428159 pdm-2.8.0a0/tests/cli/__init__.py
--rw-r--r--   0        0        0     3723 2023-06-27 02:38:06.428159 pdm-2.8.0a0/tests/cli/conftest.py
--rw-r--r--   0        0        0    12362 2023-06-27 02:38:06.428159 pdm-2.8.0a0/tests/cli/test_add.py
--rw-r--r--   0        0        0     5775 2023-06-27 02:38:06.428159 pdm-2.8.0a0/tests/cli/test_build.py
--rw-r--r--   0        0        0     5229 2023-06-27 02:38:06.428159 pdm-2.8.0a0/tests/cli/test_cache.py
--rw-r--r--   0        0        0     9286 2023-06-27 02:38:06.428159 pdm-2.8.0a0/tests/cli/test_config.py
--rw-r--r--   0        0        0     2029 2023-06-27 02:38:06.428159 pdm-2.8.0a0/tests/cli/test_fix.py
--rw-r--r--   0        0        0    10375 2023-06-27 02:38:06.432159 pdm-2.8.0a0/tests/cli/test_hooks.py
--rw-r--r--   0        0        0     4950 2023-06-27 02:38:06.432159 pdm-2.8.0a0/tests/cli/test_init.py
--rw-r--r--   0        0        0    11265 2023-06-27 02:38:06.432159 pdm-2.8.0a0/tests/cli/test_install.py
--rw-r--r--   0        0        0    28998 2023-06-27 02:38:06.432159 pdm-2.8.0a0/tests/cli/test_list.py
--rw-r--r--   0        0        0     6324 2023-06-27 02:38:06.432159 pdm-2.8.0a0/tests/cli/test_lock.py
--rw-r--r--   0        0        0     7796 2023-06-27 02:38:06.432159 pdm-2.8.0a0/tests/cli/test_others.py
--rw-r--r--   0        0        0     6052 2023-06-27 02:38:06.432159 pdm-2.8.0a0/tests/cli/test_publish.py
--rw-r--r--   0        0        0     3888 2023-06-27 02:38:06.432159 pdm-2.8.0a0/tests/cli/test_remove.py
--rw-r--r--   0        0        0    29259 2023-06-27 02:38:06.432159 pdm-2.8.0a0/tests/cli/test_run.py
--rw-r--r--   0        0        0     3599 2023-06-27 02:38:06.432159 pdm-2.8.0a0/tests/cli/test_self_command.py
--rw-r--r--   0        0        0     2778 2023-06-27 02:38:06.432159 pdm-2.8.0a0/tests/cli/test_template.py
--rw-r--r--   0        0        0     8876 2023-06-27 02:38:06.432159 pdm-2.8.0a0/tests/cli/test_update.py
--rw-r--r--   0        0        0     2997 2023-06-27 02:38:06.432159 pdm-2.8.0a0/tests/cli/test_use.py
--rw-r--r--   0        0        0    10808 2023-06-27 02:38:06.432159 pdm-2.8.0a0/tests/cli/test_venv.py
--rw-r--r--   0        0        0     3079 2023-06-27 02:38:06.432159 pdm-2.8.0a0/tests/conftest.py
--rw-r--r--   0        0        0      235 2023-06-27 02:38:06.432159 pdm-2.8.0a0/tests/fixtures/Pipfile
--rw-r--r--   0        0        0        0 2023-06-27 02:38:06.432159 pdm-2.8.0a0/tests/fixtures/__init__.py
--rw-r--r--   0        0        0    49497 2023-06-27 02:38:06.432159 pdm-2.8.0a0/tests/fixtures/artifacts/PyFunctional-1.4.3-py3-none-any.whl
--rw-r--r--   0        0        0      546 2023-06-27 02:38:06.432159 pdm-2.8.0a0/tests/fixtures/artifacts/caj2pdf-restructured-0.1.0a6.tar.gz
--rw-r--r--   0        0        0   422824 2023-06-27 02:38:06.436159 pdm-2.8.0a0/tests/fixtures/artifacts/celery-4.4.2-py2.py3-none-any.whl
--rw-r--r--   0        0        0     1254 2023-06-27 02:38:06.436159 pdm-2.8.0a0/tests/fixtures/artifacts/demo-0.0.1-cp36-cp36m-win_amd64.whl
--rw-r--r--   0        0        0     1254 2023-06-27 02:38:06.436159 pdm-2.8.0a0/tests/fixtures/artifacts/demo-0.0.1-py2.py3-none-any.whl
--rw-r--r--   0        0        0     1038 2023-06-27 02:38:06.436159 pdm-2.8.0a0/tests/fixtures/artifacts/demo-0.0.1.tar.gz
--rw-r--r--   0        0        0     2615 2023-06-27 02:38:06.436159 pdm-2.8.0a0/tests/fixtures/artifacts/demo-0.0.1.zip
--rw-r--r--   0        0        0     4595 2023-06-27 02:38:06.436159 pdm-2.8.0a0/tests/fixtures/artifacts/editables-0.2-py3-none-any.whl
--rw-r--r--   0        0        0     5359 2023-06-27 02:38:06.436159 pdm-2.8.0a0/tests/fixtures/artifacts/first-2.0.2-py2.py3-none-any.whl
--rw-r--r--   0        0        0    56715 2023-06-27 02:38:06.436159 pdm-2.8.0a0/tests/fixtures/artifacts/flit_core-3.6.0-py3-none-any.whl
--rw-r--r--   0        0        0     6138 2023-06-27 02:38:06.436159 pdm-2.8.0a0/tests/fixtures/artifacts/future_fstrings-1.2.0-py2.py3-none-any.whl
--rw-r--r--   0        0        0     5786 2023-06-27 02:38:06.436159 pdm-2.8.0a0/tests/fixtures/artifacts/future_fstrings-1.2.0.tar.gz
--rw-r--r--   0        0        0    17978 2023-06-27 02:38:06.436159 pdm-2.8.0a0/tests/fixtures/artifacts/importlib_metadata-4.8.3-py3-none-any.whl
--rw-r--r--   0        0        0    24489 2023-06-27 02:38:06.436159 pdm-2.8.0a0/tests/fixtures/artifacts/jmespath-0.10.0-py2.py3-none-any.whl
--rw-r--r--   0        0        0   156727 2023-06-27 02:38:06.436159 pdm-2.8.0a0/tests/fixtures/artifacts/pdm_backend-2.0.2-py3-none-any.whl
--rw-r--r--   0        0        0     1401 2023-06-27 02:38:06.436159 pdm-2.8.0a0/tests/fixtures/artifacts/pdm_hello-0.1.0-py3-none-any.whl
--rw-r--r--   0        0        0     1405 2023-06-27 02:38:06.436159 pdm-2.8.0a0/tests/fixtures/artifacts/pdm_hello-0.1.0-py3-none-win_amd64.whl
--rw-r--r--   0        0        0   305481 2023-06-27 02:38:06.440159 pdm-2.8.0a0/tests/fixtures/artifacts/pdm_pep517-1.0.0-py3-none-any.whl
--rw-r--r--   0        0        0   531270 2023-06-27 02:38:06.440159 pdm-2.8.0a0/tests/fixtures/artifacts/poetry_core-1.3.2-py3-none-any.whl
--rw-r--r--   0        0        0  1232518 2023-06-27 02:38:06.448160 pdm-2.8.0a0/tests/fixtures/artifacts/setuptools-65.4.1-py3-none-any.whl
--rw-r--r--   0        0        0    26662 2023-06-27 02:38:06.448160 pdm-2.8.0a0/tests/fixtures/artifacts/typing_extensions-4.4.0-py3-none-any.whl
--rw-r--r--   0        0        0    35301 2023-06-27 02:38:06.448160 pdm-2.8.0a0/tests/fixtures/artifacts/wheel-0.37.1-py2.py3-none-any.whl
--rw-r--r--   0        0        0     5312 2023-06-27 02:38:06.448160 pdm-2.8.0a0/tests/fixtures/artifacts/zipp-3.7.0-py3-none-any.whl
--rw-r--r--   0        0        0      326 2023-06-27 02:38:06.448160 pdm-2.8.0a0/tests/fixtures/index/demo.html
--rw-r--r--   0        0        0      511 2023-06-27 02:38:06.448160 pdm-2.8.0a0/tests/fixtures/index/future-fstrings.html
--rw-r--r--   0        0        0      262 2023-06-27 02:38:06.448160 pdm-2.8.0a0/tests/fixtures/index/pep345-legacy.html
--rw-r--r--   0        0        0      262 2023-06-27 02:38:06.448160 pdm-2.8.0a0/tests/fixtures/index/wheel.html
--rw-r--r--   0        0        0        0 2023-06-27 02:38:06.448160 pdm-2.8.0a0/tests/fixtures/projects/__init__.py
--rw-r--r--   0        0        0       42 2023-06-27 02:38:06.448160 pdm-2.8.0a0/tests/fixtures/projects/demo-#-with-hash/demo.py
--rw-r--r--   0        0        0      332 2023-06-27 02:38:06.448160 pdm-2.8.0a0/tests/fixtures/projects/demo-#-with-hash/setup.py
--rw-r--r--   0        0        0       26 2023-06-27 02:38:06.448160 pdm-2.8.0a0/tests/fixtures/projects/demo-combined-extras/demo.py
--rw-r--r--   0        0        0      462 2023-06-27 02:38:06.448160 pdm-2.8.0a0/tests/fixtures/projects/demo-combined-extras/pyproject.toml
--rw-r--r--   0        0        0       42 2023-06-27 02:38:06.448160 pdm-2.8.0a0/tests/fixtures/projects/demo-failure-no-dep/demo.py
--rw-r--r--   0        0        0      246 2023-06-27 02:38:06.448160 pdm-2.8.0a0/tests/fixtures/projects/demo-failure-no-dep/setup.py
--rw-r--r--   0        0        0       42 2023-06-27 02:38:06.448160 pdm-2.8.0a0/tests/fixtures/projects/demo-failure/demo.py
--rw-r--r--   0        0        0      345 2023-06-27 02:38:06.448160 pdm-2.8.0a0/tests/fixtures/projects/demo-failure/setup.py
--rw-r--r--   0        0        0       12 2023-06-27 02:38:06.448160 pdm-2.8.0a0/tests/fixtures/projects/demo-module/LICENSE
--rw-r--r--   0        0        0       24 2023-06-27 02:38:06.448160 pdm-2.8.0a0/tests/fixtures/projects/demo-module/README.md
--rw-r--r--   0        0        0       14 2023-06-27 02:38:06.448160 pdm-2.8.0a0/tests/fixtures/projects/demo-module/bar_module.py
--rw-r--r--   0        0        0       36 2023-06-27 02:38:06.448160 pdm-2.8.0a0/tests/fixtures/projects/demo-module/foo_module.py
--rw-r--r--   0        0        0      442 2023-06-27 02:38:06.448160 pdm-2.8.0a0/tests/fixtures/projects/demo-module/pyproject.toml
--rw-r--r--   0        0        0     3983 2023-06-27 02:38:06.448160 pdm-2.8.0a0/tests/fixtures/projects/demo-package-has-dep-with-extras/pdm.lock
--rw-r--r--   0        0        0      318 2023-06-27 02:38:06.448160 pdm-2.8.0a0/tests/fixtures/projects/demo-package-has-dep-with-extras/pyproject.toml
--rw-r--r--   0        0        0      157 2023-06-27 02:38:06.448160 pdm-2.8.0a0/tests/fixtures/projects/demo-package-has-dep-with-extras/requirements.txt
--rw-r--r--   0        0        0       12 2023-06-27 02:38:06.448160 pdm-2.8.0a0/tests/fixtures/projects/demo-package/LICENSE
--rw-r--r--   0        0        0       13 2023-06-27 02:38:06.448160 pdm-2.8.0a0/tests/fixtures/projects/demo-package/README.md
--rw-r--r--   0        0        0       16 2023-06-27 02:38:06.448160 pdm-2.8.0a0/tests/fixtures/projects/demo-package/data_out.json
--rw-r--r--   0        0        0       22 2023-06-27 02:38:06.448160 pdm-2.8.0a0/tests/fixtures/projects/demo-package/my_package/__init__.py
--rw-r--r--   0        0        0       24 2023-06-27 02:38:06.448160 pdm-2.8.0a0/tests/fixtures/projects/demo-package/my_package/data.json
--rw-r--r--   0        0        0    29800 2023-06-27 02:38:06.448160 pdm-2.8.0a0/tests/fixtures/projects/demo-package/pdm.lock
--rw-r--r--   0        0        0      572 2023-06-27 02:38:06.448160 pdm-2.8.0a0/tests/fixtures/projects/demo-package/pyproject.toml
--rw-r--r--   0        0        0      122 2023-06-27 02:38:06.448160 pdm-2.8.0a0/tests/fixtures/projects/demo-package/requirements.ini
--rw-r--r--   0        0        0     7521 2023-06-27 02:38:06.448160 pdm-2.8.0a0/tests/fixtures/projects/demo-package/requirements.txt
--rw-r--r--   0        0        0      211 2023-06-27 02:38:06.448160 pdm-2.8.0a0/tests/fixtures/projects/demo-package/requirements_simple.txt
--rw-r--r--   0        0        0      726 2023-06-27 02:38:06.448160 pdm-2.8.0a0/tests/fixtures/projects/demo-package/setup.txt
--rw-r--r--   0        0        0       21 2023-06-27 02:38:06.448160 pdm-2.8.0a0/tests/fixtures/projects/demo-package/single_module.py
--rw-r--r--   0        0        0       18 2023-06-27 02:38:06.448160 pdm-2.8.0a0/tests/fixtures/projects/demo-parent-package/README.md
--rw-r--r--   0        0        0       22 2023-06-27 02:38:06.448160 pdm-2.8.0a0/tests/fixtures/projects/demo-parent-package/package-a/foo.py
--rw-r--r--   0        0        0      120 2023-06-27 02:38:06.448160 pdm-2.8.0a0/tests/fixtures/projects/demo-parent-package/package-a/setup.py
--rw-r--r--   0        0        0       22 2023-06-27 02:38:06.448160 pdm-2.8.0a0/tests/fixtures/projects/demo-parent-package/package-b/bar.py
--rw-r--r--   0        0        0      197 2023-06-27 02:38:06.448160 pdm-2.8.0a0/tests/fixtures/projects/demo-parent-package/package-b/pyproject.toml
--rw-r--r--   0        0        0       42 2023-06-27 02:38:06.448160 pdm-2.8.0a0/tests/fixtures/projects/demo-prerelease/demo.py
--rw-r--r--   0        0        0      334 2023-06-27 02:38:06.448160 pdm-2.8.0a0/tests/fixtures/projects/demo-prerelease/setup.py
--rw-r--r--   0        0        0       12 2023-06-27 02:38:06.448160 pdm-2.8.0a0/tests/fixtures/projects/demo-src-package/LICENSE
--rw-r--r--   0        0        0       24 2023-06-27 02:38:06.448160 pdm-2.8.0a0/tests/fixtures/projects/demo-src-package/README.md
--rw-r--r--   0        0        0       16 2023-06-27 02:38:06.448160 pdm-2.8.0a0/tests/fixtures/projects/demo-src-package/data_out.json
--rw-r--r--   0        0        0      456 2023-06-27 02:38:06.448160 pdm-2.8.0a0/tests/fixtures/projects/demo-src-package/pyproject.toml
--rw-r--r--   0        0        0       21 2023-06-27 02:38:06.448160 pdm-2.8.0a0/tests/fixtures/projects/demo-src-package/single_module.py
--rw-r--r--   0        0        0       22 2023-06-27 02:38:06.448160 pdm-2.8.0a0/tests/fixtures/projects/demo-src-package/src/my_package/__init__.py
--rw-r--r--   0        0        0       24 2023-06-27 02:38:06.448160 pdm-2.8.0a0/tests/fixtures/projects/demo-src-package/src/my_package/data.json
--rw-r--r--   0        0        0       42 2023-06-27 02:38:06.448160 pdm-2.8.0a0/tests/fixtures/projects/demo/demo.py
--rw-r--r--   0        0        0      344 2023-06-27 02:38:06.448160 pdm-2.8.0a0/tests/fixtures/projects/demo/pyproject.toml
--rw-r--r--   0        0        0       26 2023-06-27 02:38:06.448160 pdm-2.8.0a0/tests/fixtures/projects/demo_extras/demo.py
--rw-r--r--   0        0        0      250 2023-06-27 02:38:06.448160 pdm-2.8.0a0/tests/fixtures/projects/demo_extras/setup.py
--rw-r--r--   0        0        0        0 2023-06-27 02:38:06.448160 pdm-2.8.0a0/tests/fixtures/projects/flit-demo/README.rst
--rw-r--r--   0        0        0        0 2023-06-27 02:38:06.448160 pdm-2.8.0a0/tests/fixtures/projects/flit-demo/doc/index.html
--rw-r--r--   0        0        0       49 2023-06-27 02:38:06.448160 pdm-2.8.0a0/tests/fixtures/projects/flit-demo/flit.py
--rw-r--r--   0        0        0      969 2023-06-27 02:38:06.448160 pdm-2.8.0a0/tests/fixtures/projects/flit-demo/pyproject.toml
--rw-r--r--   0        0        0       12 2023-06-27 02:38:06.448160 pdm-2.8.0a0/tests/fixtures/projects/poetry-demo/mylib.py
--rw-r--r--   0        0        0      863 2023-06-27 02:38:06.448160 pdm-2.8.0a0/tests/fixtures/projects/poetry-demo/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-27 02:38:06.448160 pdm-2.8.0a0/tests/fixtures/projects/test-hatch-static/README.md
--rw-r--r--   0        0        0      386 2023-06-27 02:38:06.448160 pdm-2.8.0a0/tests/fixtures/projects/test-hatch-static/pyproject.toml
--rw-r--r--   0        0        0       11 2023-06-27 02:38:06.448160 pdm-2.8.0a0/tests/fixtures/projects/test-monorepo/README.md
--rw-r--r--   0        0        0        0 2023-06-27 02:38:06.452160 pdm-2.8.0a0/tests/fixtures/projects/test-monorepo/core/core.py
--rw-r--r--   0        0        0      179 2023-06-27 02:38:06.452160 pdm-2.8.0a0/tests/fixtures/projects/test-monorepo/core/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-27 02:38:06.452160 pdm-2.8.0a0/tests/fixtures/projects/test-monorepo/package_a/alice.py
--rw-r--r--   0        0        0      231 2023-06-27 02:38:06.452160 pdm-2.8.0a0/tests/fixtures/projects/test-monorepo/package_a/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-27 02:38:06.452160 pdm-2.8.0a0/tests/fixtures/projects/test-monorepo/package_b/bob.py
--rw-r--r--   0        0        0      231 2023-06-27 02:38:06.452160 pdm-2.8.0a0/tests/fixtures/projects/test-monorepo/package_b/pyproject.toml
--rw-r--r--   0        0        0      237 2023-06-27 02:38:06.452160 pdm-2.8.0a0/tests/fixtures/projects/test-monorepo/pyproject.toml
--rw-r--r--   0        0        0      380 2023-06-27 02:38:06.452160 pdm-2.8.0a0/tests/fixtures/projects/test-plugin-pdm/hello.py
--rw-r--r--   0        0        0      312 2023-06-27 02:38:06.452160 pdm-2.8.0a0/tests/fixtures/projects/test-plugin-pdm/pyproject.toml
--rw-r--r--   0        0        0      380 2023-06-27 02:38:06.452160 pdm-2.8.0a0/tests/fixtures/projects/test-plugin/hello.py
--rw-r--r--   0        0        0      168 2023-06-27 02:38:06.452160 pdm-2.8.0a0/tests/fixtures/projects/test-plugin/setup.py
--rw-r--r--   0        0        0        0 2023-06-27 02:38:06.452160 pdm-2.8.0a0/tests/fixtures/projects/test-removal/__init__.py
--rw-r--r--   0        0        0        0 2023-06-27 02:38:06.452160 pdm-2.8.0a0/tests/fixtures/projects/test-removal/bar.py
--rw-r--r--   0        0        0        0 2023-06-27 02:38:06.452160 pdm-2.8.0a0/tests/fixtures/projects/test-removal/foo.py
--rw-r--r--   0        0        0        0 2023-06-27 02:38:06.452160 pdm-2.8.0a0/tests/fixtures/projects/test-removal/subdir/__init__.py
--rw-r--r--   0        0        0       10 2023-06-27 02:38:06.452160 pdm-2.8.0a0/tests/fixtures/projects/test-setuptools/AUTHORS
--rw-r--r--   0        0        0       12 2023-06-27 02:38:06.452160 pdm-2.8.0a0/tests/fixtures/projects/test-setuptools/README.md
--rw-r--r--   0        0        0       22 2023-06-27 02:38:06.452160 pdm-2.8.0a0/tests/fixtures/projects/test-setuptools/mymodule.py
--rw-r--r--   0        0        0      398 2023-06-27 02:38:06.452160 pdm-2.8.0a0/tests/fixtures/projects/test-setuptools/setup.cfg
--rw-r--r--   0        0        0      308 2023-06-27 02:38:06.452160 pdm-2.8.0a0/tests/fixtures/projects/test-setuptools/setup.py
--rw-r--r--   0        0        0     1525 2023-06-27 02:38:06.452160 pdm-2.8.0a0/tests/fixtures/pypi.json
--rw-r--r--   0        0        0     1330 2023-06-27 02:38:06.452160 pdm-2.8.0a0/tests/fixtures/pyproject.toml
--rw-r--r--   0        0        0       20 2023-06-27 02:38:06.452160 pdm-2.8.0a0/tests/fixtures/requirements-include.txt
--rw-r--r--   0        0        0      502 2023-06-27 02:38:06.452160 pdm-2.8.0a0/tests/fixtures/requirements.txt
--rw-r--r--   0        0        0        0 2023-06-27 02:38:06.452160 pdm-2.8.0a0/tests/models/__init__.py
--rw-r--r--   0        0        0     3814 2023-06-27 02:38:06.452160 pdm-2.8.0a0/tests/models/test_backends.py
--rw-r--r--   0        0        0    13344 2023-06-27 02:38:06.452160 pdm-2.8.0a0/tests/models/test_candidates.py
--rw-r--r--   0        0        0     1971 2023-06-27 02:38:06.452160 pdm-2.8.0a0/tests/models/test_marker.py
--rw-r--r--   0        0        0     2679 2023-06-27 02:38:06.452160 pdm-2.8.0a0/tests/models/test_requirements.py
--rw-r--r--   0        0        0     2556 2023-06-27 02:38:06.452160 pdm-2.8.0a0/tests/models/test_setup_parsing.py
--rw-r--r--   0        0        0     3418 2023-06-27 02:38:06.452160 pdm-2.8.0a0/tests/models/test_specifiers.py
--rw-r--r--   0        0        0     2703 2023-06-27 02:38:06.452160 pdm-2.8.0a0/tests/models/test_versions.py
--rw-r--r--   0        0        0        0 2023-06-27 02:38:06.452160 pdm-2.8.0a0/tests/resolver/__init__.py
--rw-r--r--   0        0        0    11567 2023-06-27 02:38:06.452160 pdm-2.8.0a0/tests/resolver/test_resolve.py
--rw-r--r--   0        0        0     7704 2023-06-27 02:38:06.452160 pdm-2.8.0a0/tests/test_formats.py
--rw-r--r--   0        0        0     7231 2023-06-27 02:38:06.452160 pdm-2.8.0a0/tests/test_installer.py
--rw-r--r--   0        0        0     1829 2023-06-27 02:38:06.452160 pdm-2.8.0a0/tests/test_integration.py
--rw-r--r--   0        0        0     3435 2023-06-27 02:38:06.452160 pdm-2.8.0a0/tests/test_plugin.py
--rw-r--r--   0        0        0    12085 2023-06-27 02:38:06.452160 pdm-2.8.0a0/tests/test_project.py
--rw-r--r--   0        0        0     1103 2023-06-27 02:38:06.452160 pdm-2.8.0a0/tests/test_signals.py
--rw-r--r--   0        0        0     4409 2023-06-27 02:38:06.452160 pdm-2.8.0a0/tests/test_utils.py
--rw-r--r--   0        0        0     9626 1970-01-01 00:00:00.000000 pdm-2.8.0a0/PKG-INFO
+-rw-r--r--   0        0        0   126343 2023-06-27 07:57:18.746300 pdm-2.8.0a1/CHANGELOG.md
+-rw-r--r--   0        0        0     1075 2023-06-27 07:57:18.746300 pdm-2.8.0a1/LICENSE
+-rw-r--r--   0        0        0     1075 2023-06-27 07:57:18.746300 pdm-2.8.0a1/LICENSE
+-rw-r--r--   0        0        0     7937 2023-06-27 07:57:18.746300 pdm-2.8.0a1/README.md
+-rw-r--r--   0        0        0     7937 2023-06-27 07:57:18.746300 pdm-2.8.0a1/README.md
+-rw-r--r--   0        0        0     4559 2023-06-27 07:57:26.526371 pdm-2.8.0a1/pyproject.toml
+-rw-r--r--   0        0        0       65 2023-06-27 07:57:18.750300 pdm-2.8.0a1/src/pdm/__main__.py
+-rw-r--r--   0        0        0      316 2023-06-27 07:57:18.750300 pdm-2.8.0a1/src/pdm/__version__.py
+-rw-r--r--   0        0        0     3282 2023-06-27 07:57:18.750300 pdm-2.8.0a1/src/pdm/_types.py
+-rw-r--r--   0        0        0      237 2023-06-27 07:57:18.750300 pdm-2.8.0a1/src/pdm/builders/__init__.py
+-rw-r--r--   0        0        0    11850 2023-06-27 07:57:18.754300 pdm-2.8.0a1/src/pdm/builders/base.py
+-rw-r--r--   0        0        0     1755 2023-06-27 07:57:18.754300 pdm-2.8.0a1/src/pdm/builders/editable.py
+-rw-r--r--   0        0        0      656 2023-06-27 07:57:18.754300 pdm-2.8.0a1/src/pdm/builders/sdist.py
+-rw-r--r--   0        0        0     1073 2023-06-27 07:57:18.754300 pdm-2.8.0a1/src/pdm/builders/wheel.py
+-rw-r--r--   0        0        0        0 2023-06-27 07:57:18.754300 pdm-2.8.0a1/src/pdm/cli/__init__.py
+-rw-r--r--   0        0        0    16131 2023-06-27 07:57:18.754300 pdm-2.8.0a1/src/pdm/cli/actions.py
+-rw-r--r--   0        0        0        0 2023-06-27 07:57:18.754300 pdm-2.8.0a1/src/pdm/cli/commands/__init__.py
+-rw-r--r--   0        0        0     7104 2023-06-27 07:57:18.754300 pdm-2.8.0a1/src/pdm/cli/commands/add.py
+-rw-r--r--   0        0        0     2857 2023-06-27 07:57:18.754300 pdm-2.8.0a1/src/pdm/cli/commands/base.py
+-rw-r--r--   0        0        0     4236 2023-06-27 07:57:18.754300 pdm-2.8.0a1/src/pdm/cli/commands/build.py
+-rw-r--r--   0        0        0     6542 2023-06-27 07:57:18.754300 pdm-2.8.0a1/src/pdm/cli/commands/cache.py
+-rw-r--r--   0        0        0     1324 2023-06-27 07:57:18.754300 pdm-2.8.0a1/src/pdm/cli/commands/completion.py
+-rw-r--r--   0        0        0     7165 2023-06-27 07:57:18.754300 pdm-2.8.0a1/src/pdm/cli/commands/config.py
+-rw-r--r--   0        0        0     3066 2023-06-27 07:57:18.754300 pdm-2.8.0a1/src/pdm/cli/commands/export.py
+-rw-r--r--   0        0        0     3136 2023-06-27 07:57:18.754300 pdm-2.8.0a1/src/pdm/cli/commands/fix/__init__.py
+-rw-r--r--   0        0        0     2309 2023-06-27 07:57:18.754300 pdm-2.8.0a1/src/pdm/cli/commands/fix/fixers.py
+-rw-r--r--   0        0        0     3689 2023-06-27 07:57:18.754300 pdm-2.8.0a1/src/pdm/cli/commands/import_cmd.py
+-rw-r--r--   0        0        0     3032 2023-06-27 07:57:18.754300 pdm-2.8.0a1/src/pdm/cli/commands/info.py
+-rw-r--r--   0        0        0    10543 2023-06-27 07:57:18.754300 pdm-2.8.0a1/src/pdm/cli/commands/init.py
+-rw-r--r--   0        0        0     3589 2023-06-27 07:57:18.754300 pdm-2.8.0a1/src/pdm/cli/commands/install.py
+-rw-r--r--   0        0        0    15754 2023-06-27 07:57:18.754300 pdm-2.8.0a1/src/pdm/cli/commands/list.py
+-rw-r--r--   0        0        0     2196 2023-06-27 07:57:18.754300 pdm-2.8.0a1/src/pdm/cli/commands/lock.py
+-rw-r--r--   0        0        0     6596 2023-06-27 07:57:18.754300 pdm-2.8.0a1/src/pdm/cli/commands/publish/__init__.py
+-rw-r--r--   0        0        0     8112 2023-06-27 07:57:18.754300 pdm-2.8.0a1/src/pdm/cli/commands/publish/package.py
+-rw-r--r--   0        0        0     6782 2023-06-27 07:57:18.754300 pdm-2.8.0a1/src/pdm/cli/commands/publish/repository.py
+-rw-r--r--   0        0        0     4271 2023-06-27 07:57:18.754300 pdm-2.8.0a1/src/pdm/cli/commands/remove.py
+-rw-r--r--   0        0        0    15489 2023-06-27 07:57:18.754300 pdm-2.8.0a1/src/pdm/cli/commands/run.py
+-rw-r--r--   0        0        0     2436 2023-06-27 07:57:18.754300 pdm-2.8.0a1/src/pdm/cli/commands/search.py
+-rw-r--r--   0        0        0     9370 2023-06-27 07:57:18.754300 pdm-2.8.0a1/src/pdm/cli/commands/self_cmd.py
+-rw-r--r--   0        0        0     2896 2023-06-27 07:57:18.754300 pdm-2.8.0a1/src/pdm/cli/commands/show.py
+-rw-r--r--   0        0        0     1447 2023-06-27 07:57:18.754300 pdm-2.8.0a1/src/pdm/cli/commands/sync.py
+-rw-r--r--   0        0        0     6898 2023-06-27 07:57:18.754300 pdm-2.8.0a1/src/pdm/cli/commands/update.py
+-rw-r--r--   0        0        0     6489 2023-06-27 07:57:18.754300 pdm-2.8.0a1/src/pdm/cli/commands/use.py
+-rw-r--r--   0        0        0     1723 2023-06-27 07:57:18.754300 pdm-2.8.0a1/src/pdm/cli/commands/venv/__init__.py
+-rw-r--r--   0        0        0     2426 2023-06-27 07:57:18.754300 pdm-2.8.0a1/src/pdm/cli/commands/venv/activate.py
+-rw-r--r--   0        0        0     6149 2023-06-27 07:57:18.754300 pdm-2.8.0a1/src/pdm/cli/commands/venv/backends.py
+-rw-r--r--   0        0        0     2155 2023-06-27 07:57:18.754300 pdm-2.8.0a1/src/pdm/cli/commands/venv/create.py
+-rw-r--r--   0        0        0      819 2023-06-27 07:57:18.754300 pdm-2.8.0a1/src/pdm/cli/commands/venv/list.py
+-rw-r--r--   0        0        0     2195 2023-06-27 07:57:18.754300 pdm-2.8.0a1/src/pdm/cli/commands/venv/purge.py
+-rw-r--r--   0        0        0     1279 2023-06-27 07:57:18.754300 pdm-2.8.0a1/src/pdm/cli/commands/venv/remove.py
+-rw-r--r--   0        0        0     2759 2023-06-27 07:57:18.754300 pdm-2.8.0a1/src/pdm/cli/commands/venv/utils.py
+-rw-r--r--   0        0        0        0 2023-06-27 07:57:18.754300 pdm-2.8.0a1/src/pdm/cli/completions/__init__.py
+-rw-r--r--   0        0        0     5137 2023-06-27 07:57:18.754300 pdm-2.8.0a1/src/pdm/cli/completions/pdm.bash
+-rw-r--r--   0        0        0    50498 2023-06-27 07:57:18.754300 pdm-2.8.0a1/src/pdm/cli/completions/pdm.fish
+-rw-r--r--   0        0        0    18629 2023-06-27 07:57:18.754300 pdm-2.8.0a1/src/pdm/cli/completions/pdm.ps1
+-rw-r--r--   0        0        0    25397 2023-06-27 07:57:18.754300 pdm-2.8.0a1/src/pdm/cli/completions/pdm.zsh
+-rw-r--r--   0        0        0     3840 2023-06-27 07:57:18.754300 pdm-2.8.0a1/src/pdm/cli/filters.py
+-rw-r--r--   0        0        0     1481 2023-06-27 07:57:18.754300 pdm-2.8.0a1/src/pdm/cli/hooks.py
+-rw-r--r--   0        0        0    10461 2023-06-27 07:57:18.754300 pdm-2.8.0a1/src/pdm/cli/options.py
+-rw-r--r--   0        0        0     6235 2023-06-27 07:57:18.754300 pdm-2.8.0a1/src/pdm/cli/templates/__init__.py
+-rw-r--r--   0        0        0     3102 2023-06-27 07:57:18.754300 pdm-2.8.0a1/src/pdm/cli/templates/default/.gitignore
+-rw-r--r--   0        0        0       18 2023-06-27 07:57:18.754300 pdm-2.8.0a1/src/pdm/cli/templates/default/README.md
+-rw-r--r--   0        0        0        0 2023-06-27 07:57:18.754300 pdm-2.8.0a1/src/pdm/cli/templates/default/__init__.py
+-rw-r--r--   0        0        0      278 2023-06-27 07:57:18.754300 pdm-2.8.0a1/src/pdm/cli/templates/default/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-27 07:57:18.754300 pdm-2.8.0a1/src/pdm/cli/templates/default/src/example_package/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-27 07:57:18.754300 pdm-2.8.0a1/src/pdm/cli/templates/default/tests/__init__.py
+-rw-r--r--   0        0        0    25152 2023-06-27 07:57:18.754300 pdm-2.8.0a1/src/pdm/cli/utils.py
+-rw-r--r--   0        0        0     2373 2023-06-27 07:57:18.754300 pdm-2.8.0a1/src/pdm/compat.py
+-rw-r--r--   0        0        0    10667 2023-06-27 07:57:18.754300 pdm-2.8.0a1/src/pdm/core.py
+-rw-r--r--   0        0        0      825 2023-06-27 07:57:18.754300 pdm-2.8.0a1/src/pdm/environments/__init__.py
+-rw-r--r--   0        0        0     8850 2023-06-27 07:57:18.754300 pdm-2.8.0a1/src/pdm/environments/base.py
+-rw-r--r--   0        0        0     4255 2023-06-27 07:57:18.754300 pdm-2.8.0a1/src/pdm/environments/local.py
+-rw-r--r--   0        0        0     1600 2023-06-27 07:57:18.754300 pdm-2.8.0a1/src/pdm/environments/python.py
+-rw-r--r--   0        0        0     1362 2023-06-27 07:57:18.754300 pdm-2.8.0a1/src/pdm/exceptions.py
+-rw-r--r--   0        0        0     1202 2023-06-27 07:57:18.754300 pdm-2.8.0a1/src/pdm/formats/__init__.py
+-rw-r--r--   0        0        0     3215 2023-06-27 07:57:18.754300 pdm-2.8.0a1/src/pdm/formats/base.py
+-rw-r--r--   0        0        0     5788 2023-06-27 07:57:18.754300 pdm-2.8.0a1/src/pdm/formats/flit.py
+-rw-r--r--   0        0        0     2614 2023-06-27 07:57:18.754300 pdm-2.8.0a1/src/pdm/formats/pipfile.py
+-rw-r--r--   0        0        0     7490 2023-06-27 07:57:18.754300 pdm-2.8.0a1/src/pdm/formats/poetry.py
+-rw-r--r--   0        0        0     7502 2023-06-27 07:57:18.754300 pdm-2.8.0a1/src/pdm/formats/requirements.py
+-rw-r--r--   0        0        0     2309 2023-06-27 07:57:18.754300 pdm-2.8.0a1/src/pdm/formats/setup_py.py
+-rw-r--r--   0        0        0      119 2023-06-27 07:57:18.754300 pdm-2.8.0a1/src/pdm/installers/__init__.py
+-rw-r--r--   0        0        0     1390 2023-06-27 07:57:18.754300 pdm-2.8.0a1/src/pdm/installers/core.py
+-rw-r--r--   0        0        0    10901 2023-06-27 07:57:18.758300 pdm-2.8.0a1/src/pdm/installers/installers.py
+-rw-r--r--   0        0        0     2091 2023-06-27 07:57:18.758300 pdm-2.8.0a1/src/pdm/installers/manager.py
+-rw-r--r--   0        0        0     2226 2023-06-27 07:57:18.758300 pdm-2.8.0a1/src/pdm/installers/packages.py
+-rw-r--r--   0        0        0    18161 2023-06-27 07:57:18.758300 pdm-2.8.0a1/src/pdm/installers/synchronizers.py
+-rw-r--r--   0        0        0    10990 2023-06-27 07:57:18.758300 pdm-2.8.0a1/src/pdm/installers/uninstallers.py
+-rw-r--r--   0        0        0        0 2023-06-27 07:57:18.758300 pdm-2.8.0a1/src/pdm/models/__init__.py
+-rw-r--r--   0        0        0     3162 2023-06-27 07:57:18.758300 pdm-2.8.0a1/src/pdm/models/auth.py
+-rw-r--r--   0        0        0     4698 2023-06-27 07:57:18.758300 pdm-2.8.0a1/src/pdm/models/backends.py
+-rw-r--r--   0        0        0    11710 2023-06-27 07:57:18.758300 pdm-2.8.0a1/src/pdm/models/caches.py
+-rw-r--r--   0        0        0    26580 2023-06-27 07:57:18.758300 pdm-2.8.0a1/src/pdm/models/candidates.py
+-rw-r--r--   0        0        0      287 2023-06-27 07:57:18.758300 pdm-2.8.0a1/src/pdm/models/environment.py
+-rw-r--r--   0        0        0     1845 2023-06-27 07:57:18.758300 pdm-2.8.0a1/src/pdm/models/in_process/__init__.py
+-rw-r--r--   0        0        0     2049 2023-06-27 07:57:18.758300 pdm-2.8.0a1/src/pdm/models/in_process/get_abi_tag.py
+-rw-r--r--   0        0        0     6323 2023-06-27 07:57:18.758300 pdm-2.8.0a1/src/pdm/models/in_process/parse_setup.py
+-rw-r--r--   0        0        0     1165 2023-06-27 07:57:18.758300 pdm-2.8.0a1/src/pdm/models/in_process/pep508.py
+-rw-r--r--   0        0        0     1653 2023-06-27 07:57:18.758300 pdm-2.8.0a1/src/pdm/models/in_process/sysconfig_get_paths.py
+-rw-r--r--   0        0        0     5701 2023-06-27 07:57:18.758300 pdm-2.8.0a1/src/pdm/models/markers.py
+-rw-r--r--   0        0        0     3507 2023-06-27 07:57:18.758300 pdm-2.8.0a1/src/pdm/models/project_info.py
+-rw-r--r--   0        0        0     2195 2023-06-27 07:57:18.758300 pdm-2.8.0a1/src/pdm/models/python.py
+-rw-r--r--   0        0        0      318 2023-06-27 07:57:18.758300 pdm-2.8.0a1/src/pdm/models/python_max_versions.json
+-rw-r--r--   0        0        0    21340 2023-06-27 07:57:18.758300 pdm-2.8.0a1/src/pdm/models/repositories.py
+-rw-r--r--   0        0        0    18792 2023-06-27 07:57:18.758300 pdm-2.8.0a1/src/pdm/models/requirements.py
+-rw-r--r--   0        0        0     2313 2023-06-27 07:57:18.758300 pdm-2.8.0a1/src/pdm/models/search.py
+-rw-r--r--   0        0        0     3363 2023-06-27 07:57:18.758300 pdm-2.8.0a1/src/pdm/models/session.py
+-rw-r--r--   0        0        0    14482 2023-06-27 07:57:18.758300 pdm-2.8.0a1/src/pdm/models/setup.py
+-rw-r--r--   0        0        0    16337 2023-06-27 07:57:18.758300 pdm-2.8.0a1/src/pdm/models/specifiers.py
+-rw-r--r--   0        0        0     1300 2023-06-27 07:57:18.758300 pdm-2.8.0a1/src/pdm/models/venv.py
+-rw-r--r--   0        0        0     5924 2023-06-27 07:57:18.758300 pdm-2.8.0a1/src/pdm/models/versions.py
+-rw-r--r--   0        0        0     2766 2023-06-27 07:57:18.758300 pdm-2.8.0a1/src/pdm/models/working_set.py
+-rw-r--r--   0        0        0        0 2023-06-27 07:57:18.758300 pdm-2.8.0a1/src/pdm/pep582/__init__.py
+-rw-r--r--   0        0        0     4481 2023-06-27 07:57:18.758300 pdm-2.8.0a1/src/pdm/pep582/sitecustomize.py
+-rw-r--r--   0        0        0      134 2023-06-27 07:57:18.758300 pdm-2.8.0a1/src/pdm/project/__init__.py
+-rw-r--r--   0        0        0    16757 2023-06-27 07:57:18.758300 pdm-2.8.0a1/src/pdm/project/config.py
+-rw-r--r--   0        0        0    26292 2023-06-27 07:57:18.758300 pdm-2.8.0a1/src/pdm/project/core.py
+-rw-r--r--   0        0        0     2093 2023-06-27 07:57:18.758300 pdm-2.8.0a1/src/pdm/project/lockfile.py
+-rw-r--r--   0        0        0     3385 2023-06-27 07:57:18.758300 pdm-2.8.0a1/src/pdm/project/project_file.py
+-rw-r--r--   0        0        0     1070 2023-06-27 07:57:18.758300 pdm-2.8.0a1/src/pdm/project/toml_file.py
+-rw-r--r--   0        0        0        0 2023-06-27 07:57:18.758300 pdm-2.8.0a1/src/pdm/py.typed
+-rw-r--r--   0        0        0    20067 2023-06-27 07:57:18.758300 pdm-2.8.0a1/src/pdm/pytest.py
+-rw-r--r--   0        0        0       61 2023-06-27 07:57:18.758300 pdm-2.8.0a1/src/pdm/resolver/__init__.py
+-rw-r--r--   0        0        0     1954 2023-06-27 07:57:18.758300 pdm-2.8.0a1/src/pdm/resolver/core.py
+-rw-r--r--   0        0        0    13176 2023-06-27 07:57:18.758300 pdm-2.8.0a1/src/pdm/resolver/providers.py
+-rw-r--r--   0        0        0     1580 2023-06-27 07:57:18.758300 pdm-2.8.0a1/src/pdm/resolver/python.py
+-rw-r--r--   0        0        0     3742 2023-06-27 07:57:18.758300 pdm-2.8.0a1/src/pdm/resolver/reporters.py
+-rw-r--r--   0        0        0     4027 2023-06-27 07:57:18.758300 pdm-2.8.0a1/src/pdm/signals.py
+-rw-r--r--   0        0        0     8054 2023-06-27 07:57:18.758300 pdm-2.8.0a1/src/pdm/termui.py
+-rw-r--r--   0        0        0    14101 2023-06-27 07:57:18.758300 pdm-2.8.0a1/src/pdm/utils.py
+-rw-r--r--   0        0        0       72 2023-06-27 07:57:18.758300 pdm-2.8.0a1/tests/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-27 07:57:18.758300 pdm-2.8.0a1/tests/cli/__init__.py
+-rw-r--r--   0        0        0     3723 2023-06-27 07:57:18.758300 pdm-2.8.0a1/tests/cli/conftest.py
+-rw-r--r--   0        0        0    12362 2023-06-27 07:57:18.758300 pdm-2.8.0a1/tests/cli/test_add.py
+-rw-r--r--   0        0        0     5775 2023-06-27 07:57:18.758300 pdm-2.8.0a1/tests/cli/test_build.py
+-rw-r--r--   0        0        0     5229 2023-06-27 07:57:18.758300 pdm-2.8.0a1/tests/cli/test_cache.py
+-rw-r--r--   0        0        0     9286 2023-06-27 07:57:18.758300 pdm-2.8.0a1/tests/cli/test_config.py
+-rw-r--r--   0        0        0     2029 2023-06-27 07:57:18.758300 pdm-2.8.0a1/tests/cli/test_fix.py
+-rw-r--r--   0        0        0    10375 2023-06-27 07:57:18.758300 pdm-2.8.0a1/tests/cli/test_hooks.py
+-rw-r--r--   0        0        0     4950 2023-06-27 07:57:18.758300 pdm-2.8.0a1/tests/cli/test_init.py
+-rw-r--r--   0        0        0    11265 2023-06-27 07:57:18.758300 pdm-2.8.0a1/tests/cli/test_install.py
+-rw-r--r--   0        0        0    28998 2023-06-27 07:57:18.758300 pdm-2.8.0a1/tests/cli/test_list.py
+-rw-r--r--   0        0        0     6324 2023-06-27 07:57:18.758300 pdm-2.8.0a1/tests/cli/test_lock.py
+-rw-r--r--   0        0        0     7796 2023-06-27 07:57:18.758300 pdm-2.8.0a1/tests/cli/test_others.py
+-rw-r--r--   0        0        0     6052 2023-06-27 07:57:18.758300 pdm-2.8.0a1/tests/cli/test_publish.py
+-rw-r--r--   0        0        0     3888 2023-06-27 07:57:18.758300 pdm-2.8.0a1/tests/cli/test_remove.py
+-rw-r--r--   0        0        0    29259 2023-06-27 07:57:18.758300 pdm-2.8.0a1/tests/cli/test_run.py
+-rw-r--r--   0        0        0     3599 2023-06-27 07:57:18.758300 pdm-2.8.0a1/tests/cli/test_self_command.py
+-rw-r--r--   0        0        0     2778 2023-06-27 07:57:18.758300 pdm-2.8.0a1/tests/cli/test_template.py
+-rw-r--r--   0        0        0     8876 2023-06-27 07:57:18.762300 pdm-2.8.0a1/tests/cli/test_update.py
+-rw-r--r--   0        0        0     2997 2023-06-27 07:57:18.762300 pdm-2.8.0a1/tests/cli/test_use.py
+-rw-r--r--   0        0        0    10808 2023-06-27 07:57:18.762300 pdm-2.8.0a1/tests/cli/test_venv.py
+-rw-r--r--   0        0        0     3079 2023-06-27 07:57:18.762300 pdm-2.8.0a1/tests/conftest.py
+-rw-r--r--   0        0        0      235 2023-06-27 07:57:18.762300 pdm-2.8.0a1/tests/fixtures/Pipfile
+-rw-r--r--   0        0        0        0 2023-06-27 07:57:18.762300 pdm-2.8.0a1/tests/fixtures/__init__.py
+-rw-r--r--   0        0        0    49497 2023-06-27 07:57:18.762300 pdm-2.8.0a1/tests/fixtures/artifacts/PyFunctional-1.4.3-py3-none-any.whl
+-rw-r--r--   0        0        0      546 2023-06-27 07:57:18.762300 pdm-2.8.0a1/tests/fixtures/artifacts/caj2pdf-restructured-0.1.0a6.tar.gz
+-rw-r--r--   0        0        0   422824 2023-06-27 07:57:18.762300 pdm-2.8.0a1/tests/fixtures/artifacts/celery-4.4.2-py2.py3-none-any.whl
+-rw-r--r--   0        0        0     1254 2023-06-27 07:57:18.762300 pdm-2.8.0a1/tests/fixtures/artifacts/demo-0.0.1-cp36-cp36m-win_amd64.whl
+-rw-r--r--   0        0        0     1254 2023-06-27 07:57:18.762300 pdm-2.8.0a1/tests/fixtures/artifacts/demo-0.0.1-py2.py3-none-any.whl
+-rw-r--r--   0        0        0     1038 2023-06-27 07:57:18.762300 pdm-2.8.0a1/tests/fixtures/artifacts/demo-0.0.1.tar.gz
+-rw-r--r--   0        0        0     2615 2023-06-27 07:57:18.762300 pdm-2.8.0a1/tests/fixtures/artifacts/demo-0.0.1.zip
+-rw-r--r--   0        0        0     4595 2023-06-27 07:57:18.762300 pdm-2.8.0a1/tests/fixtures/artifacts/editables-0.2-py3-none-any.whl
+-rw-r--r--   0        0        0     5359 2023-06-27 07:57:18.762300 pdm-2.8.0a1/tests/fixtures/artifacts/first-2.0.2-py2.py3-none-any.whl
+-rw-r--r--   0        0        0    56715 2023-06-27 07:57:18.762300 pdm-2.8.0a1/tests/fixtures/artifacts/flit_core-3.6.0-py3-none-any.whl
+-rw-r--r--   0        0        0     6138 2023-06-27 07:57:18.762300 pdm-2.8.0a1/tests/fixtures/artifacts/future_fstrings-1.2.0-py2.py3-none-any.whl
+-rw-r--r--   0        0        0     5786 2023-06-27 07:57:18.762300 pdm-2.8.0a1/tests/fixtures/artifacts/future_fstrings-1.2.0.tar.gz
+-rw-r--r--   0        0        0    17978 2023-06-27 07:57:18.762300 pdm-2.8.0a1/tests/fixtures/artifacts/importlib_metadata-4.8.3-py3-none-any.whl
+-rw-r--r--   0        0        0    24489 2023-06-27 07:57:18.762300 pdm-2.8.0a1/tests/fixtures/artifacts/jmespath-0.10.0-py2.py3-none-any.whl
+-rw-r--r--   0        0        0   156727 2023-06-27 07:57:18.766300 pdm-2.8.0a1/tests/fixtures/artifacts/pdm_backend-2.0.2-py3-none-any.whl
+-rw-r--r--   0        0        0     1401 2023-06-27 07:57:18.766300 pdm-2.8.0a1/tests/fixtures/artifacts/pdm_hello-0.1.0-py3-none-any.whl
+-rw-r--r--   0        0        0     1405 2023-06-27 07:57:18.766300 pdm-2.8.0a1/tests/fixtures/artifacts/pdm_hello-0.1.0-py3-none-win_amd64.whl
+-rw-r--r--   0        0        0   305481 2023-06-27 07:57:18.766300 pdm-2.8.0a1/tests/fixtures/artifacts/pdm_pep517-1.0.0-py3-none-any.whl
+-rw-r--r--   0        0        0   531270 2023-06-27 07:57:18.770300 pdm-2.8.0a1/tests/fixtures/artifacts/poetry_core-1.3.2-py3-none-any.whl
+-rw-r--r--   0        0        0  1232518 2023-06-27 07:57:18.774300 pdm-2.8.0a1/tests/fixtures/artifacts/setuptools-65.4.1-py3-none-any.whl
+-rw-r--r--   0        0        0    26662 2023-06-27 07:57:18.774300 pdm-2.8.0a1/tests/fixtures/artifacts/typing_extensions-4.4.0-py3-none-any.whl
+-rw-r--r--   0        0        0    35301 2023-06-27 07:57:18.774300 pdm-2.8.0a1/tests/fixtures/artifacts/wheel-0.37.1-py2.py3-none-any.whl
+-rw-r--r--   0        0        0     5312 2023-06-27 07:57:18.774300 pdm-2.8.0a1/tests/fixtures/artifacts/zipp-3.7.0-py3-none-any.whl
+-rw-r--r--   0        0        0      326 2023-06-27 07:57:18.774300 pdm-2.8.0a1/tests/fixtures/index/demo.html
+-rw-r--r--   0        0        0      511 2023-06-27 07:57:18.774300 pdm-2.8.0a1/tests/fixtures/index/future-fstrings.html
+-rw-r--r--   0        0        0      262 2023-06-27 07:57:18.774300 pdm-2.8.0a1/tests/fixtures/index/pep345-legacy.html
+-rw-r--r--   0        0        0      262 2023-06-27 07:57:18.774300 pdm-2.8.0a1/tests/fixtures/index/wheel.html
+-rw-r--r--   0        0        0        0 2023-06-27 07:57:18.774300 pdm-2.8.0a1/tests/fixtures/projects/__init__.py
+-rw-r--r--   0        0        0       42 2023-06-27 07:57:18.774300 pdm-2.8.0a1/tests/fixtures/projects/demo-#-with-hash/demo.py
+-rw-r--r--   0        0        0      332 2023-06-27 07:57:18.774300 pdm-2.8.0a1/tests/fixtures/projects/demo-#-with-hash/setup.py
+-rw-r--r--   0        0        0       26 2023-06-27 07:57:18.774300 pdm-2.8.0a1/tests/fixtures/projects/demo-combined-extras/demo.py
+-rw-r--r--   0        0        0      462 2023-06-27 07:57:18.774300 pdm-2.8.0a1/tests/fixtures/projects/demo-combined-extras/pyproject.toml
+-rw-r--r--   0        0        0       42 2023-06-27 07:57:18.774300 pdm-2.8.0a1/tests/fixtures/projects/demo-failure-no-dep/demo.py
+-rw-r--r--   0        0        0      246 2023-06-27 07:57:18.774300 pdm-2.8.0a1/tests/fixtures/projects/demo-failure-no-dep/setup.py
+-rw-r--r--   0        0        0       42 2023-06-27 07:57:18.774300 pdm-2.8.0a1/tests/fixtures/projects/demo-failure/demo.py
+-rw-r--r--   0        0        0      345 2023-06-27 07:57:18.774300 pdm-2.8.0a1/tests/fixtures/projects/demo-failure/setup.py
+-rw-r--r--   0        0        0       12 2023-06-27 07:57:18.774300 pdm-2.8.0a1/tests/fixtures/projects/demo-module/LICENSE
+-rw-r--r--   0        0        0       24 2023-06-27 07:57:18.774300 pdm-2.8.0a1/tests/fixtures/projects/demo-module/README.md
+-rw-r--r--   0        0        0       14 2023-06-27 07:57:18.774300 pdm-2.8.0a1/tests/fixtures/projects/demo-module/bar_module.py
+-rw-r--r--   0        0        0       36 2023-06-27 07:57:18.774300 pdm-2.8.0a1/tests/fixtures/projects/demo-module/foo_module.py
+-rw-r--r--   0        0        0      442 2023-06-27 07:57:18.774300 pdm-2.8.0a1/tests/fixtures/projects/demo-module/pyproject.toml
+-rw-r--r--   0        0        0     3983 2023-06-27 07:57:18.774300 pdm-2.8.0a1/tests/fixtures/projects/demo-package-has-dep-with-extras/pdm.lock
+-rw-r--r--   0        0        0      318 2023-06-27 07:57:18.774300 pdm-2.8.0a1/tests/fixtures/projects/demo-package-has-dep-with-extras/pyproject.toml
+-rw-r--r--   0        0        0      157 2023-06-27 07:57:18.774300 pdm-2.8.0a1/tests/fixtures/projects/demo-package-has-dep-with-extras/requirements.txt
+-rw-r--r--   0        0        0       12 2023-06-27 07:57:18.774300 pdm-2.8.0a1/tests/fixtures/projects/demo-package/LICENSE
+-rw-r--r--   0        0        0       13 2023-06-27 07:57:18.774300 pdm-2.8.0a1/tests/fixtures/projects/demo-package/README.md
+-rw-r--r--   0        0        0       16 2023-06-27 07:57:18.774300 pdm-2.8.0a1/tests/fixtures/projects/demo-package/data_out.json
+-rw-r--r--   0        0        0       22 2023-06-27 07:57:18.774300 pdm-2.8.0a1/tests/fixtures/projects/demo-package/my_package/__init__.py
+-rw-r--r--   0        0        0       24 2023-06-27 07:57:18.774300 pdm-2.8.0a1/tests/fixtures/projects/demo-package/my_package/data.json
+-rw-r--r--   0        0        0    29800 2023-06-27 07:57:18.774300 pdm-2.8.0a1/tests/fixtures/projects/demo-package/pdm.lock
+-rw-r--r--   0        0        0      572 2023-06-27 07:57:18.774300 pdm-2.8.0a1/tests/fixtures/projects/demo-package/pyproject.toml
+-rw-r--r--   0        0        0      122 2023-06-27 07:57:18.774300 pdm-2.8.0a1/tests/fixtures/projects/demo-package/requirements.ini
+-rw-r--r--   0        0        0     7521 2023-06-27 07:57:18.774300 pdm-2.8.0a1/tests/fixtures/projects/demo-package/requirements.txt
+-rw-r--r--   0        0        0      211 2023-06-27 07:57:18.774300 pdm-2.8.0a1/tests/fixtures/projects/demo-package/requirements_simple.txt
+-rw-r--r--   0        0        0      726 2023-06-27 07:57:18.774300 pdm-2.8.0a1/tests/fixtures/projects/demo-package/setup.txt
+-rw-r--r--   0        0        0       21 2023-06-27 07:57:18.774300 pdm-2.8.0a1/tests/fixtures/projects/demo-package/single_module.py
+-rw-r--r--   0        0        0       18 2023-06-27 07:57:18.774300 pdm-2.8.0a1/tests/fixtures/projects/demo-parent-package/README.md
+-rw-r--r--   0        0        0       22 2023-06-27 07:57:18.774300 pdm-2.8.0a1/tests/fixtures/projects/demo-parent-package/package-a/foo.py
+-rw-r--r--   0        0        0      120 2023-06-27 07:57:18.774300 pdm-2.8.0a1/tests/fixtures/projects/demo-parent-package/package-a/setup.py
+-rw-r--r--   0        0        0       22 2023-06-27 07:57:18.774300 pdm-2.8.0a1/tests/fixtures/projects/demo-parent-package/package-b/bar.py
+-rw-r--r--   0        0        0      197 2023-06-27 07:57:18.774300 pdm-2.8.0a1/tests/fixtures/projects/demo-parent-package/package-b/pyproject.toml
+-rw-r--r--   0        0        0       42 2023-06-27 07:57:18.774300 pdm-2.8.0a1/tests/fixtures/projects/demo-prerelease/demo.py
+-rw-r--r--   0        0        0      334 2023-06-27 07:57:18.774300 pdm-2.8.0a1/tests/fixtures/projects/demo-prerelease/setup.py
+-rw-r--r--   0        0        0       12 2023-06-27 07:57:18.774300 pdm-2.8.0a1/tests/fixtures/projects/demo-src-package/LICENSE
+-rw-r--r--   0        0        0       24 2023-06-27 07:57:18.778300 pdm-2.8.0a1/tests/fixtures/projects/demo-src-package/README.md
+-rw-r--r--   0        0        0       16 2023-06-27 07:57:18.778300 pdm-2.8.0a1/tests/fixtures/projects/demo-src-package/data_out.json
+-rw-r--r--   0        0        0      456 2023-06-27 07:57:18.778300 pdm-2.8.0a1/tests/fixtures/projects/demo-src-package/pyproject.toml
+-rw-r--r--   0        0        0       21 2023-06-27 07:57:18.778300 pdm-2.8.0a1/tests/fixtures/projects/demo-src-package/single_module.py
+-rw-r--r--   0        0        0       22 2023-06-27 07:57:18.778300 pdm-2.8.0a1/tests/fixtures/projects/demo-src-package/src/my_package/__init__.py
+-rw-r--r--   0        0        0       24 2023-06-27 07:57:18.778300 pdm-2.8.0a1/tests/fixtures/projects/demo-src-package/src/my_package/data.json
+-rw-r--r--   0        0        0       42 2023-06-27 07:57:18.778300 pdm-2.8.0a1/tests/fixtures/projects/demo/demo.py
+-rw-r--r--   0        0        0      344 2023-06-27 07:57:18.778300 pdm-2.8.0a1/tests/fixtures/projects/demo/pyproject.toml
+-rw-r--r--   0        0        0       26 2023-06-27 07:57:18.778300 pdm-2.8.0a1/tests/fixtures/projects/demo_extras/demo.py
+-rw-r--r--   0        0        0      250 2023-06-27 07:57:18.778300 pdm-2.8.0a1/tests/fixtures/projects/demo_extras/setup.py
+-rw-r--r--   0        0        0        0 2023-06-27 07:57:18.778300 pdm-2.8.0a1/tests/fixtures/projects/flit-demo/README.rst
+-rw-r--r--   0        0        0        0 2023-06-27 07:57:18.778300 pdm-2.8.0a1/tests/fixtures/projects/flit-demo/doc/index.html
+-rw-r--r--   0        0        0       49 2023-06-27 07:57:18.778300 pdm-2.8.0a1/tests/fixtures/projects/flit-demo/flit.py
+-rw-r--r--   0        0        0      969 2023-06-27 07:57:18.778300 pdm-2.8.0a1/tests/fixtures/projects/flit-demo/pyproject.toml
+-rw-r--r--   0        0        0       12 2023-06-27 07:57:18.778300 pdm-2.8.0a1/tests/fixtures/projects/poetry-demo/mylib.py
+-rw-r--r--   0        0        0      863 2023-06-27 07:57:18.778300 pdm-2.8.0a1/tests/fixtures/projects/poetry-demo/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-27 07:57:18.778300 pdm-2.8.0a1/tests/fixtures/projects/test-hatch-static/README.md
+-rw-r--r--   0        0        0      386 2023-06-27 07:57:18.778300 pdm-2.8.0a1/tests/fixtures/projects/test-hatch-static/pyproject.toml
+-rw-r--r--   0        0        0       11 2023-06-27 07:57:18.778300 pdm-2.8.0a1/tests/fixtures/projects/test-monorepo/README.md
+-rw-r--r--   0        0        0        0 2023-06-27 07:57:18.778300 pdm-2.8.0a1/tests/fixtures/projects/test-monorepo/core/core.py
+-rw-r--r--   0        0        0      179 2023-06-27 07:57:18.778300 pdm-2.8.0a1/tests/fixtures/projects/test-monorepo/core/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-27 07:57:18.778300 pdm-2.8.0a1/tests/fixtures/projects/test-monorepo/package_a/alice.py
+-rw-r--r--   0        0        0      231 2023-06-27 07:57:18.778300 pdm-2.8.0a1/tests/fixtures/projects/test-monorepo/package_a/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-27 07:57:18.778300 pdm-2.8.0a1/tests/fixtures/projects/test-monorepo/package_b/bob.py
+-rw-r--r--   0        0        0      231 2023-06-27 07:57:18.778300 pdm-2.8.0a1/tests/fixtures/projects/test-monorepo/package_b/pyproject.toml
+-rw-r--r--   0        0        0      237 2023-06-27 07:57:18.778300 pdm-2.8.0a1/tests/fixtures/projects/test-monorepo/pyproject.toml
+-rw-r--r--   0        0        0      380 2023-06-27 07:57:18.778300 pdm-2.8.0a1/tests/fixtures/projects/test-plugin-pdm/hello.py
+-rw-r--r--   0        0        0      312 2023-06-27 07:57:18.778300 pdm-2.8.0a1/tests/fixtures/projects/test-plugin-pdm/pyproject.toml
+-rw-r--r--   0        0        0      380 2023-06-27 07:57:18.778300 pdm-2.8.0a1/tests/fixtures/projects/test-plugin/hello.py
+-rw-r--r--   0        0        0      168 2023-06-27 07:57:18.778300 pdm-2.8.0a1/tests/fixtures/projects/test-plugin/setup.py
+-rw-r--r--   0        0        0        0 2023-06-27 07:57:18.778300 pdm-2.8.0a1/tests/fixtures/projects/test-removal/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-27 07:57:18.778300 pdm-2.8.0a1/tests/fixtures/projects/test-removal/bar.py
+-rw-r--r--   0        0        0        0 2023-06-27 07:57:18.778300 pdm-2.8.0a1/tests/fixtures/projects/test-removal/foo.py
+-rw-r--r--   0        0        0        0 2023-06-27 07:57:18.778300 pdm-2.8.0a1/tests/fixtures/projects/test-removal/subdir/__init__.py
+-rw-r--r--   0        0        0       10 2023-06-27 07:57:18.778300 pdm-2.8.0a1/tests/fixtures/projects/test-setuptools/AUTHORS
+-rw-r--r--   0        0        0       12 2023-06-27 07:57:18.778300 pdm-2.8.0a1/tests/fixtures/projects/test-setuptools/README.md
+-rw-r--r--   0        0        0       22 2023-06-27 07:57:18.778300 pdm-2.8.0a1/tests/fixtures/projects/test-setuptools/mymodule.py
+-rw-r--r--   0        0        0      398 2023-06-27 07:57:18.778300 pdm-2.8.0a1/tests/fixtures/projects/test-setuptools/setup.cfg
+-rw-r--r--   0        0        0      308 2023-06-27 07:57:18.778300 pdm-2.8.0a1/tests/fixtures/projects/test-setuptools/setup.py
+-rw-r--r--   0        0        0     1525 2023-06-27 07:57:18.778300 pdm-2.8.0a1/tests/fixtures/pypi.json
+-rw-r--r--   0        0        0     1330 2023-06-27 07:57:18.778300 pdm-2.8.0a1/tests/fixtures/pyproject.toml
+-rw-r--r--   0        0        0       20 2023-06-27 07:57:18.778300 pdm-2.8.0a1/tests/fixtures/requirements-include.txt
+-rw-r--r--   0        0        0      502 2023-06-27 07:57:18.778300 pdm-2.8.0a1/tests/fixtures/requirements.txt
+-rw-r--r--   0        0        0        0 2023-06-27 07:57:18.778300 pdm-2.8.0a1/tests/models/__init__.py
+-rw-r--r--   0        0        0     3814 2023-06-27 07:57:18.778300 pdm-2.8.0a1/tests/models/test_backends.py
+-rw-r--r--   0        0        0    13344 2023-06-27 07:57:18.778300 pdm-2.8.0a1/tests/models/test_candidates.py
+-rw-r--r--   0        0        0     1971 2023-06-27 07:57:18.778300 pdm-2.8.0a1/tests/models/test_marker.py
+-rw-r--r--   0        0        0     2679 2023-06-27 07:57:18.778300 pdm-2.8.0a1/tests/models/test_requirements.py
+-rw-r--r--   0        0        0     2556 2023-06-27 07:57:18.778300 pdm-2.8.0a1/tests/models/test_setup_parsing.py
+-rw-r--r--   0        0        0     3418 2023-06-27 07:57:18.778300 pdm-2.8.0a1/tests/models/test_specifiers.py
+-rw-r--r--   0        0        0     2703 2023-06-27 07:57:18.778300 pdm-2.8.0a1/tests/models/test_versions.py
+-rw-r--r--   0        0        0        0 2023-06-27 07:57:18.778300 pdm-2.8.0a1/tests/resolver/__init__.py
+-rw-r--r--   0        0        0    11567 2023-06-27 07:57:18.778300 pdm-2.8.0a1/tests/resolver/test_resolve.py
+-rw-r--r--   0        0        0     7704 2023-06-27 07:57:18.778300 pdm-2.8.0a1/tests/test_formats.py
+-rw-r--r--   0        0        0     7231 2023-06-27 07:57:18.778300 pdm-2.8.0a1/tests/test_installer.py
+-rw-r--r--   0        0        0     1829 2023-06-27 07:57:18.778300 pdm-2.8.0a1/tests/test_integration.py
+-rw-r--r--   0        0        0     3435 2023-06-27 07:57:18.778300 pdm-2.8.0a1/tests/test_plugin.py
+-rw-r--r--   0        0        0    12085 2023-06-27 07:57:18.778300 pdm-2.8.0a1/tests/test_project.py
+-rw-r--r--   0        0        0     1103 2023-06-27 07:57:18.778300 pdm-2.8.0a1/tests/test_signals.py
+-rw-r--r--   0        0        0     4409 2023-06-27 07:57:18.778300 pdm-2.8.0a1/tests/test_utils.py
+-rw-r--r--   0        0        0     9838 1970-01-01 00:00:00.000000 pdm-2.8.0a1/PKG-INFO
```

### Comparing `pdm-2.8.0a0/CHANGELOG.md` & `pdm-2.8.0a1/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,21 @@
+Release v2.8.0a1 (2023-06-27)
+-----------------------------
+
+### Features & Improvements
+
+- Add support for `cookiecutter` and `copier` as project generator. [#2059](https://github.com/pdm-project/pdm/issues/2059)
+
+
 Release v2.8.0a0 (2023-06-27)
 -----------------------------
 
 ### Features & Improvements
 
+- `pdm init` now accepts a template argument to initialize project from a built-in or Git template. [#2053](https://github.com/pdm-project/pdm/issues/2053)
 - Replace the `DeprecationWarning` with `FutureWarning` for better exposure. [#2012](https://github.com/pdm-project/pdm/issues/2012)
 - Serve `install-pdm.py` and its checksum file on the docs site. [#2026](https://github.com/pdm-project/pdm/issues/2026)
 - Add new option `--edit/-e` to `pdm config` to edit the config file in default editor. [#2028](https://github.com/pdm-project/pdm/issues/2028)
 - Add `--project` option to `pdm venv` to support another path as the project root. [#2042](https://github.com/pdm-project/pdm/issues/2042)
 - Add support for using `truststore` as the SSL backend. This only works on Python 3.10 or newer. [#2049](https://github.com/pdm-project/pdm/issues/2049)
 
 ### Bug Fixes
```

### Comparing `pdm-2.8.0a0/LICENSE` & `pdm-2.8.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a0/README.md` & `pdm-2.8.0a1/README.md`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a0/pyproject.toml` & `pdm-2.8.0a1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
-version = "2.8.0a0"
+version = "2.8.0a1"
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 Homepage = "https://pdm.fming.dev"
 Repository = "https://github.com/pdm-project/pdm"
@@ -54,14 +54,20 @@
 Changelog = "https://pdm.fming.dev/latest/dev/changelog/"
 
 [project.optional-dependencies]
 pytest = [
     "pytest",
     "pytest-mock",
 ]
+all = [
+    "copier",
+    "cookiecutter",
+    "keyring",
+    "truststore; python_version >= \"3.10\"",
+]
 
 [project.scripts]
 pdm = "pdm.core:main"
 
 [tool.pdm.version]
 source = "scm"
 write_to = "pdm/models/VERSION"
```

### Comparing `pdm-2.8.0a0/src/pdm/_types.py` & `pdm-2.8.0a1/src/pdm/_types.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a0/src/pdm/builders/base.py` & `pdm-2.8.0a1/src/pdm/builders/base.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a0/src/pdm/builders/editable.py` & `pdm-2.8.0a1/src/pdm/builders/editable.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a0/src/pdm/builders/sdist.py` & `pdm-2.8.0a1/src/pdm/builders/sdist.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a0/src/pdm/builders/wheel.py` & `pdm-2.8.0a1/src/pdm/builders/wheel.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a0/src/pdm/cli/actions.py` & `pdm-2.8.0a1/src/pdm/cli/actions.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a0/src/pdm/cli/commands/add.py` & `pdm-2.8.0a1/src/pdm/cli/commands/add.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a0/src/pdm/cli/commands/base.py` & `pdm-2.8.0a1/src/pdm/cli/commands/base.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a0/src/pdm/cli/commands/build.py` & `pdm-2.8.0a1/src/pdm/cli/commands/build.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a0/src/pdm/cli/commands/cache.py` & `pdm-2.8.0a1/src/pdm/cli/commands/cache.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a0/src/pdm/cli/commands/completion.py` & `pdm-2.8.0a1/src/pdm/cli/commands/completion.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a0/src/pdm/cli/commands/config.py` & `pdm-2.8.0a1/src/pdm/cli/commands/config.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a0/src/pdm/cli/commands/export.py` & `pdm-2.8.0a1/src/pdm/cli/commands/export.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a0/src/pdm/cli/commands/fix/__init__.py` & `pdm-2.8.0a1/src/pdm/cli/commands/fix/__init__.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a0/src/pdm/cli/commands/fix/fixers.py` & `pdm-2.8.0a1/src/pdm/cli/commands/fix/fixers.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a0/src/pdm/cli/commands/import_cmd.py` & `pdm-2.8.0a1/src/pdm/cli/commands/import_cmd.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a0/src/pdm/cli/commands/info.py` & `pdm-2.8.0a1/src/pdm/cli/commands/info.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a0/src/pdm/cli/commands/init.py` & `pdm-2.8.0a1/src/pdm/cli/commands/init.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,38 +5,83 @@
 
 from pdm import termui
 from pdm.cli import actions
 from pdm.cli.commands.base import BaseCommand
 from pdm.cli.hooks import HookManager
 from pdm.cli.options import skip_option
 from pdm.cli.templates import ProjectTemplate
+from pdm.exceptions import PdmUsageError
 from pdm.models.backends import _BACKENDS, DEFAULT_BACKEND, BuildBackend, get_backend
 from pdm.models.python import PythonInfo
 from pdm.models.specifiers import get_specifier
 from pdm.models.venv import get_venv_python
-from pdm.utils import get_user_email_from_git
+from pdm.utils import get_user_email_from_git, package_installed
 
 if TYPE_CHECKING:
     from pdm.project import Project
 
 
 class Command(BaseCommand):
     """Initialize a pyproject.toml for PDM"""
 
     def __init__(self) -> None:
         self.interactive = True
 
-    def do_init(
-        self, project: Project, metadata: dict[str, Any], hooks: HookManager, options: argparse.Namespace
-    ) -> None:
+    def do_init(self, project: Project, options: argparse.Namespace) -> None:
         """Bootstrap the project and create a pyproject.toml"""
+        hooks = HookManager(project, options.skip)
+        if options.generator == "copier":
+            self._init_copier(project, options)
+        elif options.generator == "cookiecutter":
+            self._init_cookiecutter(project, options)
+        else:
+            self.set_python(project, options.python, hooks)
+            self._init_builtin(project, options)
+        hooks.try_emit("post_init")
+
+    def _init_copier(self, project: Project, options: argparse.Namespace) -> None:
+        if not package_installed("copier"):
+            raise PdmUsageError(
+                "--copier is passed but copier is not installed. Install it by `pdm self add copier`"
+            ) from None
+
+        from copier.cli import CopierApp
+
+        if not options.template:
+            raise PdmUsageError("template argument is required when --copier is passed")
+        _, retval = CopierApp.run([options.template, str(project.root), *options.generator_args], exit=False)
+        if retval != 0:
+            raise RuntimeError("Copier exited with non-zero status code")
+
+    def _init_cookiecutter(self, project: Project, options: argparse.Namespace) -> None:
+        if not package_installed("cookiecutter"):
+            raise PdmUsageError(
+                "--cookiecutter is passed but cookiecutter is not installed. Install it by `pdm self add cookiecutter`"
+            ) from None
+
+        from cookiecutter.cli import main as cookiecutter
+
+        if not options.template:
+            raise PdmUsageError("template argument is required when --cookiecutter is passed")
+        if options.project_path:
+            project.core.ui.echo(
+                "Cookiecutter generator does not respect --project option. "
+                "It will always create a project dir under the current directory",
+                err=True,
+                style="warning",
+            )
+        retval = cookiecutter.main([options.template, *options.generator_args], standalone_mode=False)
+        if retval != 0:
+            raise RuntimeError("Cookiecutter exited with non-zero status code")
+
+    def _init_builtin(self, project: Project, options: argparse.Namespace) -> None:
+        metadata = self.get_metadata_from_input(project, options)
         with ProjectTemplate(options.template) as template:
             template.generate(project.root, metadata)
         project.pyproject.reload()
-        hooks.try_emit("post_init")
 
     def set_interactive(self, value: bool) -> None:
         self.interactive = value
 
     def ask(self, question: str, default: str) -> str:
         if not self.interactive:
             return default
@@ -102,27 +147,49 @@
         if build_backend is not None:
             data["build-system"] = build_backend.build_system()
 
         return data
 
     def add_arguments(self, parser: argparse.ArgumentParser) -> None:
         skip_option.add_to_parser(parser)
-        parser.add_argument(
+
+        status = {
+            False: termui.style("\\[not installed]", style="error"),
+            True: termui.style("\\[installed]", style="success"),
+        }
+        generator = parser.add_mutually_exclusive_group()
+        generator.add_argument(
+            "--copier",
+            action="store_const",
+            dest="generator",
+            const="copier",
+            help=f"Use Copier to generate project {status[package_installed('copier')]}",
+        )
+        generator.add_argument(
+            "--cookiecutter",
+            action="store_const",
+            dest="generator",
+            const="cookiecutter",
+            help=f"Use Cookiecutter to generate project {status[package_installed('cookiecutter')]}",
+        )
+        group = parser.add_argument_group("builtin generator options")
+        group.add_argument(
             "-n",
             "--non-interactive",
             action="store_true",
             help="Don't ask questions but use default values",
         )
-        parser.add_argument("--python", help="Specify the Python version/path to use")
-        parser.add_argument("--backend", choices=list(_BACKENDS), help="Specify the build backend")
-        parser.add_argument("--lib", action="store_true", help="Create a library project")
+        group.add_argument("--python", help="Specify the Python version/path to use")
+        group.add_argument("--backend", choices=list(_BACKENDS), help="Specify the build backend")
+        group.add_argument("--lib", action="store_true", help="Create a library project")
         parser.add_argument(
             "template", nargs="?", help="Specify the project template, which can be a local path or a Git URL"
         )
-        parser.set_defaults(search_parent=False)
+        parser.add_argument("generator_args", nargs=argparse.REMAINDER, help="Arguments passed to the generator")
+        parser.set_defaults(search_parent=False, generator="builtin")
 
     def set_python(self, project: Project, python: str | None, hooks: HookManager) -> None:
         from pdm.cli.commands.use import Command as UseCommand
 
         do_use = UseCommand().do_use
         if self.interactive:
             python_info = do_use(
@@ -164,21 +231,16 @@
                 "You are using the PEP 582 mode, no virtualenv is created.\n"
                 "For more info, please visit https://peps.python.org/pep-0582/",
                 style="success",
             )
         project.python = python_info
 
     def handle(self, project: Project, options: argparse.Namespace) -> None:
-        hooks = HookManager(project, options.skip)
         if project.pyproject.exists():
             project.core.ui.echo("pyproject.toml already exists, update it now.", style="primary")
         else:
             project.core.ui.echo("Creating a pyproject.toml for PDM...", style="primary")
         self.set_interactive(not options.non_interactive)
-
-        self.set_python(project, options.python, hooks)
-
-        metadata = self.get_metadata_from_input(project, options)
-        self.do_init(project, metadata, hooks=hooks, options=options)
+        self.do_init(project, options=options)
         project.core.ui.echo("Project is initialized successfully", style="primary")
         if self.interactive:
             actions.ask_for_import(project)
```

### Comparing `pdm-2.8.0a0/src/pdm/cli/commands/install.py` & `pdm-2.8.0a1/src/pdm/cli/commands/install.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a0/src/pdm/cli/commands/list.py` & `pdm-2.8.0a1/src/pdm/cli/commands/list.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a0/src/pdm/cli/commands/lock.py` & `pdm-2.8.0a1/src/pdm/cli/commands/lock.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a0/src/pdm/cli/commands/publish/__init__.py` & `pdm-2.8.0a1/src/pdm/cli/commands/publish/__init__.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a0/src/pdm/cli/commands/publish/package.py` & `pdm-2.8.0a1/src/pdm/cli/commands/publish/package.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a0/src/pdm/cli/commands/publish/repository.py` & `pdm-2.8.0a1/src/pdm/cli/commands/publish/repository.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a0/src/pdm/cli/commands/remove.py` & `pdm-2.8.0a1/src/pdm/cli/commands/remove.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a0/src/pdm/cli/commands/run.py` & `pdm-2.8.0a1/src/pdm/cli/commands/run.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a0/src/pdm/cli/commands/search.py` & `pdm-2.8.0a1/src/pdm/cli/commands/search.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a0/src/pdm/cli/commands/self_cmd.py` & `pdm-2.8.0a1/src/pdm/cli/commands/self_cmd.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a0/src/pdm/cli/commands/show.py` & `pdm-2.8.0a1/src/pdm/cli/commands/show.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a0/src/pdm/cli/commands/sync.py` & `pdm-2.8.0a1/src/pdm/cli/commands/sync.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a0/src/pdm/cli/commands/update.py` & `pdm-2.8.0a1/src/pdm/cli/commands/update.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a0/src/pdm/cli/commands/use.py` & `pdm-2.8.0a1/src/pdm/cli/commands/use.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a0/src/pdm/cli/commands/venv/__init__.py` & `pdm-2.8.0a1/src/pdm/cli/commands/venv/__init__.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a0/src/pdm/cli/commands/venv/activate.py` & `pdm-2.8.0a1/src/pdm/cli/commands/venv/activate.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a0/src/pdm/cli/commands/venv/backends.py` & `pdm-2.8.0a1/src/pdm/cli/commands/venv/backends.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a0/src/pdm/cli/commands/venv/create.py` & `pdm-2.8.0a1/src/pdm/cli/commands/venv/create.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a0/src/pdm/cli/commands/venv/list.py` & `pdm-2.8.0a1/src/pdm/cli/commands/venv/list.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a0/src/pdm/cli/commands/venv/purge.py` & `pdm-2.8.0a1/src/pdm/cli/commands/venv/purge.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a0/src/pdm/cli/commands/venv/remove.py` & `pdm-2.8.0a1/src/pdm/cli/commands/venv/remove.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a0/src/pdm/cli/commands/venv/utils.py` & `pdm-2.8.0a1/src/pdm/cli/commands/venv/utils.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a0/src/pdm/cli/completions/pdm.bash` & `pdm-2.8.0a1/src/pdm/cli/completions/pdm.bash`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # BASH completion script for pdm
-# Generated by pycomplete 0.3.2
+# Generated by pycomplete 0.4.0
 
-_pdm_c6f4c6c1a82f2f50_complete()
+_pdm_a919b69078acdf0a_complete()
 {
     local cur script coms opts com
     COMPREPLY=()
     _get_comp_words_by_ref -n : cur words
 
     # for an alias, get the real script behind it
     if [[ $(type -t ${words[0]}) == "alias" ]]; then
@@ -61,15 +61,15 @@
             ;;
 
             (info)
             opts="--env --global --help --json --packages --project --python --venv --verbose --where"
             ;;
 
             (init)
-            opts="--backend --global --help --lib --non-interactive --project --python --skip --verbose"
+            opts="--backend --cookiecutter --copier --global --help --lib --non-interactive --project --python --skip --verbose"
             ;;
 
             (install)
             opts="--check --dev --dry-run --fail-fast --global --group --help --lockfile --no-default --no-editable --no-isolation --no-lock --no-self --plugins --production --project --skip --venv --verbose"
             ;;
 
             (list)
@@ -139,8 +139,8 @@
         COMPREPLY=($(compgen -W "${coms}" -- ${cur}))
         __ltrim_colon_completions "$cur"
 
         return 0
     fi
 }
 
-complete -o default -F _pdm_c6f4c6c1a82f2f50_complete pdm
+complete -o default -F _pdm_a919b69078acdf0a_complete pdm
```

### Comparing `pdm-2.8.0a0/src/pdm/cli/completions/pdm.fish` & `pdm-2.8.0a1/src/pdm/cli/completions/pdm.fish`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 # FISH completion script for pdm
-# Generated by pycomplete 0.3.2
+# Generated by pycomplete 0.4.0
 
-function __fish_pdm_c6f4c6c1a82f2f50_complete_no_subcommand
+function __fish_pdm_a919b69078acdf0a_complete_no_subcommand
     for i in (commandline -opc)
         if contains -- $i add build cache completion config export fix import info init install list lock plugin publish remove run search self show sync update use venv
             return 1
         end
     end
     return 0
 end
 
 # global options
-complete -c pdm -n '__fish_pdm_c6f4c6c1a82f2f50_complete_no_subcommand' -l config -d 'Specify another config file path [env var: PDM_CONFIG_FILE] '
-complete -c pdm -n '__fish_pdm_c6f4c6c1a82f2f50_complete_no_subcommand' -l help -d 'Show this help message and exit.'
-complete -c pdm -n '__fish_pdm_c6f4c6c1a82f2f50_complete_no_subcommand' -l ignore-python -d 'Ignore the Python path saved in .pdm-python. [env var: PDM_IGNORE_SAVED_PYTHON]'
-complete -c pdm -n '__fish_pdm_c6f4c6c1a82f2f50_complete_no_subcommand' -l pep582 -d 'Print the command line to be eval\'d by the shell'
-complete -c pdm -n '__fish_pdm_c6f4c6c1a82f2f50_complete_no_subcommand' -l verbose -d 'Use `-v` for detailed output and `-vv` for more detailed'
-complete -c pdm -n '__fish_pdm_c6f4c6c1a82f2f50_complete_no_subcommand' -l version -d 'Show the version and exit'
+complete -c pdm -n '__fish_pdm_a919b69078acdf0a_complete_no_subcommand' -l config -d 'Specify another config file path [env var: PDM_CONFIG_FILE] '
+complete -c pdm -n '__fish_pdm_a919b69078acdf0a_complete_no_subcommand' -l help -d 'Show this help message and exit.'
+complete -c pdm -n '__fish_pdm_a919b69078acdf0a_complete_no_subcommand' -l ignore-python -d 'Ignore the Python path saved in .pdm-python. [env var: PDM_IGNORE_SAVED_PYTHON]'
+complete -c pdm -n '__fish_pdm_a919b69078acdf0a_complete_no_subcommand' -l pep582 -d 'Print the command line to be eval\'d by the shell'
+complete -c pdm -n '__fish_pdm_a919b69078acdf0a_complete_no_subcommand' -l verbose -d 'Use `-v` for detailed output and `-vv` for more detailed'
+complete -c pdm -n '__fish_pdm_a919b69078acdf0a_complete_no_subcommand' -l version -d 'Show the version and exit'
 
 # commands
 # add
-complete -c pdm -f -n '__fish_pdm_c6f4c6c1a82f2f50_complete_no_subcommand' -a add -d 'Add package(s) to pyproject.toml and install them'
+complete -c pdm -f -n '__fish_pdm_a919b69078acdf0a_complete_no_subcommand' -a add -d 'Add package(s) to pyproject.toml and install them'
 complete -c pdm -A -n '__fish_seen_subcommand_from add' -l dev -d 'Add packages into dev dependencies'
 complete -c pdm -A -n '__fish_seen_subcommand_from add' -l dry-run -d 'Show the difference only and don\'t perform any action'
 complete -c pdm -A -n '__fish_seen_subcommand_from add' -l editable -d 'Specify editable packages'
 complete -c pdm -A -n '__fish_seen_subcommand_from add' -l fail-fast -d 'Abort on first installation error'
 complete -c pdm -A -n '__fish_seen_subcommand_from add' -l global -d 'Use the global project, supply the project root with `-p` option'
 complete -c pdm -A -n '__fish_seen_subcommand_from add' -l group -d 'Specify the target dependency group to add into'
 complete -c pdm -A -n '__fish_seen_subcommand_from add' -l help -d 'Show this help message and exit.'
@@ -44,28 +44,28 @@
 complete -c pdm -A -n '__fish_seen_subcommand_from add' -l update-all -d 'Update all dependencies and sub-dependencies'
 complete -c pdm -A -n '__fish_seen_subcommand_from add' -l update-eager -d 'Try to update the packages and their dependencies recursively'
 complete -c pdm -A -n '__fish_seen_subcommand_from add' -l update-reuse -d 'Reuse pinned versions already present in lock file if possible'
 complete -c pdm -A -n '__fish_seen_subcommand_from add' -l venv -d 'Run the command in the virtual environment with the given key. [env var: PDM_IN_VENV]'
 complete -c pdm -A -n '__fish_seen_subcommand_from add' -l verbose -d 'Use `-v` for detailed output and `-vv` for more detailed'
 
 # build
-complete -c pdm -f -n '__fish_pdm_c6f4c6c1a82f2f50_complete_no_subcommand' -a build -d 'Build artifacts for distribution'
+complete -c pdm -f -n '__fish_pdm_a919b69078acdf0a_complete_no_subcommand' -a build -d 'Build artifacts for distribution'
 complete -c pdm -A -n '__fish_seen_subcommand_from build' -l config-setting -d 'Pass options to the backend. options with a value must be specified after "=": `--config-setting=--opt(=value)` or `-C--opt(=value)`'
 complete -c pdm -A -n '__fish_seen_subcommand_from build' -l dest -d 'Target directory to put artifacts'
 complete -c pdm -A -n '__fish_seen_subcommand_from build' -l help -d 'Show this help message and exit.'
 complete -c pdm -A -n '__fish_seen_subcommand_from build' -l no-clean -d 'Do not clean the target directory'
 complete -c pdm -A -n '__fish_seen_subcommand_from build' -l no-isolation -d 'Do not isolate the build in a clean environment'
 complete -c pdm -A -n '__fish_seen_subcommand_from build' -l no-sdist -d 'Don\'t build source tarballs'
 complete -c pdm -A -n '__fish_seen_subcommand_from build' -l no-wheel -d 'Don\'t build wheels'
 complete -c pdm -A -n '__fish_seen_subcommand_from build' -l project -d 'Specify another path as the project root, which changes the base of pyproject.toml and __pypackages__'
 complete -c pdm -A -n '__fish_seen_subcommand_from build' -l skip -d 'Skip some tasks and/or hooks by their comma-separated names. Can be supplied multiple times. Use ":all" to skip all hooks. Use ":pre" and ":post" to skip all pre or post hooks.'
 complete -c pdm -A -n '__fish_seen_subcommand_from build' -l verbose -d 'Use `-v` for detailed output and `-vv` for more detailed'
 
 # cache
-complete -c pdm -f -n '__fish_pdm_c6f4c6c1a82f2f50_complete_no_subcommand' -a cache -d 'Control the caches of PDM'
+complete -c pdm -f -n '__fish_pdm_a919b69078acdf0a_complete_no_subcommand' -a cache -d 'Control the caches of PDM'
 complete -c pdm -A -n '__fish_seen_subcommand_from cache' -l help -d 'Show this help message and exit.'
 complete -c pdm -A -n '__fish_seen_subcommand_from cache' -l verbose -d 'Use `-v` for detailed output and `-vv` for more detailed'
 # cache subcommands
 set -l cache_subcommands clear info list remove
 # cache clear
 complete -c pdm -f -n '__fish_seen_subcommand_from cache; and not __fish_seen_subcommand_from $cache_subcommands' -a clear -d 'Clean all the files under cache directory'
 complete -c pdm -A -n '__fish_seen_subcommand_from cache; and __fish_seen_subcommand_from clear' -l help -d 'Show this help message and exit.'
@@ -83,29 +83,29 @@
 
 # cache remove
 complete -c pdm -f -n '__fish_seen_subcommand_from cache; and not __fish_seen_subcommand_from $cache_subcommands' -a remove -d 'Remove files matching the given pattern'
 complete -c pdm -A -n '__fish_seen_subcommand_from cache; and __fish_seen_subcommand_from remove' -l help -d 'Show this help message and exit.'
 complete -c pdm -A -n '__fish_seen_subcommand_from cache; and __fish_seen_subcommand_from remove' -l verbose -d 'Use `-v` for detailed output and `-vv` for more detailed'
 
 # completion
-complete -c pdm -f -n '__fish_pdm_c6f4c6c1a82f2f50_complete_no_subcommand' -a completion -d 'Generate completion scripts for the given shell'
+complete -c pdm -f -n '__fish_pdm_a919b69078acdf0a_complete_no_subcommand' -a completion -d 'Generate completion scripts for the given shell'
 complete -c pdm -A -n '__fish_seen_subcommand_from completion' -l help -d 'Show this help message and exit.'
 
 # config
-complete -c pdm -f -n '__fish_pdm_c6f4c6c1a82f2f50_complete_no_subcommand' -a config -d 'Display the current configuration'
+complete -c pdm -f -n '__fish_pdm_a919b69078acdf0a_complete_no_subcommand' -a config -d 'Display the current configuration'
 complete -c pdm -A -n '__fish_seen_subcommand_from config' -l delete -d 'Unset a configuration key'
 complete -c pdm -A -n '__fish_seen_subcommand_from config' -l edit -d 'Edit the configuration file in the default editor(defined by EDITOR env var)'
 complete -c pdm -A -n '__fish_seen_subcommand_from config' -l global -d 'Use the global project, supply the project root with `-p` option'
 complete -c pdm -A -n '__fish_seen_subcommand_from config' -l help -d 'Show this help message and exit.'
 complete -c pdm -A -n '__fish_seen_subcommand_from config' -l local -d 'Set config in the project\'s local configuration file'
 complete -c pdm -A -n '__fish_seen_subcommand_from config' -l project -d 'Specify another path as the project root, which changes the base of pyproject.toml and __pypackages__'
 complete -c pdm -A -n '__fish_seen_subcommand_from config' -l verbose -d 'Use `-v` for detailed output and `-vv` for more detailed'
 
 # export
-complete -c pdm -f -n '__fish_pdm_c6f4c6c1a82f2f50_complete_no_subcommand' -a export -d 'Export the locked packages set to other formats'
+complete -c pdm -f -n '__fish_pdm_a919b69078acdf0a_complete_no_subcommand' -a export -d 'Export the locked packages set to other formats'
 complete -c pdm -A -n '__fish_seen_subcommand_from export' -l dev -d 'Select dev dependencies'
 complete -c pdm -A -n '__fish_seen_subcommand_from export' -l expandvars -d 'Expand environment variables in requirements'
 complete -c pdm -A -n '__fish_seen_subcommand_from export' -l format -d 'Specify the export file format'
 complete -c pdm -A -n '__fish_seen_subcommand_from export' -l global -d 'Use the global project, supply the project root with `-p` option'
 complete -c pdm -A -n '__fish_seen_subcommand_from export' -l group -d 'Select group of optional-dependencies separated by comma or dev-dependencies (with `-d`). Can be supplied multiple times, use ":all" to include all groups under the same species.'
 complete -c pdm -A -n '__fish_seen_subcommand_from export' -l help -d 'Show this help message and exit.'
 complete -c pdm -A -n '__fish_seen_subcommand_from export' -l lockfile -d 'Specify another lockfile path. Default: pdm.lock. [env var: PDM_LOCKFILE]'
@@ -114,58 +114,60 @@
 complete -c pdm -A -n '__fish_seen_subcommand_from export' -l production -d 'Unselect dev dependencies'
 complete -c pdm -A -n '__fish_seen_subcommand_from export' -l project -d 'Specify another path as the project root, which changes the base of pyproject.toml and __pypackages__'
 complete -c pdm -A -n '__fish_seen_subcommand_from export' -l pyproject -d 'Read the list of packages from pyproject.toml'
 complete -c pdm -A -n '__fish_seen_subcommand_from export' -l verbose -d 'Use `-v` for detailed output and `-vv` for more detailed'
 complete -c pdm -A -n '__fish_seen_subcommand_from export' -l without-hashes -d 'Don\'t include artifact hashes'
 
 # fix
-complete -c pdm -f -n '__fish_pdm_c6f4c6c1a82f2f50_complete_no_subcommand' -a fix -d 'Fix the project problems according to the latest version of PDM'
+complete -c pdm -f -n '__fish_pdm_a919b69078acdf0a_complete_no_subcommand' -a fix -d 'Fix the project problems according to the latest version of PDM'
 complete -c pdm -A -n '__fish_seen_subcommand_from fix' -l dry-run -d 'Only show the problems'
 complete -c pdm -A -n '__fish_seen_subcommand_from fix' -l global -d 'Use the global project, supply the project root with `-p` option'
 complete -c pdm -A -n '__fish_seen_subcommand_from fix' -l help -d 'Show this help message and exit.'
 complete -c pdm -A -n '__fish_seen_subcommand_from fix' -l project -d 'Specify another path as the project root, which changes the base of pyproject.toml and __pypackages__'
 complete -c pdm -A -n '__fish_seen_subcommand_from fix' -l verbose -d 'Use `-v` for detailed output and `-vv` for more detailed'
 
 # import
-complete -c pdm -f -n '__fish_pdm_c6f4c6c1a82f2f50_complete_no_subcommand' -a import -d 'Import project metadata from other formats'
+complete -c pdm -f -n '__fish_pdm_a919b69078acdf0a_complete_no_subcommand' -a import -d 'Import project metadata from other formats'
 complete -c pdm -A -n '__fish_seen_subcommand_from import' -l dev -d 'import packages into dev dependencies'
 complete -c pdm -A -n '__fish_seen_subcommand_from import' -l format -d 'Specify the file format explicitly'
 complete -c pdm -A -n '__fish_seen_subcommand_from import' -l global -d 'Use the global project, supply the project root with `-p` option'
 complete -c pdm -A -n '__fish_seen_subcommand_from import' -l group -d 'Specify the target dependency group to import into'
 complete -c pdm -A -n '__fish_seen_subcommand_from import' -l help -d 'Show this help message and exit.'
 complete -c pdm -A -n '__fish_seen_subcommand_from import' -l project -d 'Specify another path as the project root, which changes the base of pyproject.toml and __pypackages__'
 complete -c pdm -A -n '__fish_seen_subcommand_from import' -l verbose -d 'Use `-v` for detailed output and `-vv` for more detailed'
 
 # info
-complete -c pdm -f -n '__fish_pdm_c6f4c6c1a82f2f50_complete_no_subcommand' -a info -d 'Show the project information'
+complete -c pdm -f -n '__fish_pdm_a919b69078acdf0a_complete_no_subcommand' -a info -d 'Show the project information'
 complete -c pdm -A -n '__fish_seen_subcommand_from info' -l env -d 'Show PEP 508 environment markers'
 complete -c pdm -A -n '__fish_seen_subcommand_from info' -l global -d 'Use the global project, supply the project root with `-p` option'
 complete -c pdm -A -n '__fish_seen_subcommand_from info' -l help -d 'Show this help message and exit.'
 complete -c pdm -A -n '__fish_seen_subcommand_from info' -l json -d 'Dump the information in JSON'
 complete -c pdm -A -n '__fish_seen_subcommand_from info' -l packages -d 'Show the local packages root'
 complete -c pdm -A -n '__fish_seen_subcommand_from info' -l project -d 'Specify another path as the project root, which changes the base of pyproject.toml and __pypackages__'
 complete -c pdm -A -n '__fish_seen_subcommand_from info' -l python -d 'Show the interpreter path'
 complete -c pdm -A -n '__fish_seen_subcommand_from info' -l venv -d 'Run the command in the virtual environment with the given key. [env var: PDM_IN_VENV]'
 complete -c pdm -A -n '__fish_seen_subcommand_from info' -l verbose -d 'Use `-v` for detailed output and `-vv` for more detailed'
 complete -c pdm -A -n '__fish_seen_subcommand_from info' -l where -d 'Show the project root path'
 
 # init
-complete -c pdm -f -n '__fish_pdm_c6f4c6c1a82f2f50_complete_no_subcommand' -a init -d 'Initialize a pyproject.toml for PDM'
+complete -c pdm -f -n '__fish_pdm_a919b69078acdf0a_complete_no_subcommand' -a init -d 'Initialize a pyproject.toml for PDM'
 complete -c pdm -A -n '__fish_seen_subcommand_from init' -l backend -d 'Specify the build backend'
+complete -c pdm -A -n '__fish_seen_subcommand_from init' -l cookiecutter -d 'Use Cookiecutter to generate project'
+complete -c pdm -A -n '__fish_seen_subcommand_from init' -l copier -d 'Use Copier to generate project'
 complete -c pdm -A -n '__fish_seen_subcommand_from init' -l global -d 'Use the global project, supply the project root with `-p` option'
 complete -c pdm -A -n '__fish_seen_subcommand_from init' -l help -d 'Show this help message and exit.'
 complete -c pdm -A -n '__fish_seen_subcommand_from init' -l lib -d 'Create a library project'
 complete -c pdm -A -n '__fish_seen_subcommand_from init' -l non-interactive -d 'Don\'t ask questions but use default values'
 complete -c pdm -A -n '__fish_seen_subcommand_from init' -l project -d 'Specify another path as the project root, which changes the base of pyproject.toml and __pypackages__'
 complete -c pdm -A -n '__fish_seen_subcommand_from init' -l python -d 'Specify the Python version/path to use'
 complete -c pdm -A -n '__fish_seen_subcommand_from init' -l skip -d 'Skip some tasks and/or hooks by their comma-separated names. Can be supplied multiple times. Use ":all" to skip all hooks. Use ":pre" and ":post" to skip all pre or post hooks.'
 complete -c pdm -A -n '__fish_seen_subcommand_from init' -l verbose -d 'Use `-v` for detailed output and `-vv` for more detailed'
 
 # install
-complete -c pdm -f -n '__fish_pdm_c6f4c6c1a82f2f50_complete_no_subcommand' -a install -d 'Install dependencies from lock file'
+complete -c pdm -f -n '__fish_pdm_a919b69078acdf0a_complete_no_subcommand' -a install -d 'Install dependencies from lock file'
 complete -c pdm -A -n '__fish_seen_subcommand_from install' -l check -d 'Check if the lock file is up to date and fail otherwise'
 complete -c pdm -A -n '__fish_seen_subcommand_from install' -l dev -d 'Select dev dependencies'
 complete -c pdm -A -n '__fish_seen_subcommand_from install' -l dry-run -d 'Show the difference only and don\'t perform any action'
 complete -c pdm -A -n '__fish_seen_subcommand_from install' -l fail-fast -d 'Abort on first installation error'
 complete -c pdm -A -n '__fish_seen_subcommand_from install' -l global -d 'Use the global project, supply the project root with `-p` option'
 complete -c pdm -A -n '__fish_seen_subcommand_from install' -l group -d 'Select group of optional-dependencies separated by comma or dev-dependencies (with `-d`). Can be supplied multiple times, use ":all" to include all groups under the same species.'
 complete -c pdm -A -n '__fish_seen_subcommand_from install' -l help -d 'Show this help message and exit.'
@@ -179,15 +181,15 @@
 complete -c pdm -A -n '__fish_seen_subcommand_from install' -l production -d 'Unselect dev dependencies'
 complete -c pdm -A -n '__fish_seen_subcommand_from install' -l project -d 'Specify another path as the project root, which changes the base of pyproject.toml and __pypackages__'
 complete -c pdm -A -n '__fish_seen_subcommand_from install' -l skip -d 'Skip some tasks and/or hooks by their comma-separated names. Can be supplied multiple times. Use ":all" to skip all hooks. Use ":pre" and ":post" to skip all pre or post hooks.'
 complete -c pdm -A -n '__fish_seen_subcommand_from install' -l venv -d 'Run the command in the virtual environment with the given key. [env var: PDM_IN_VENV]'
 complete -c pdm -A -n '__fish_seen_subcommand_from install' -l verbose -d 'Use `-v` for detailed output and `-vv` for more detailed'
 
 # list
-complete -c pdm -f -n '__fish_pdm_c6f4c6c1a82f2f50_complete_no_subcommand' -a list -d 'List packages installed in the current working set'
+complete -c pdm -f -n '__fish_pdm_a919b69078acdf0a_complete_no_subcommand' -a list -d 'List packages installed in the current working set'
 complete -c pdm -A -n '__fish_seen_subcommand_from list' -l csv -d 'Output dependencies in CSV document format'
 complete -c pdm -A -n '__fish_seen_subcommand_from list' -l exclude -d 'Exclude dependency groups from the output'
 complete -c pdm -A -n '__fish_seen_subcommand_from list' -l fields -d 'Select information to output as a comma separated string. For example: name,version,homepage,licenses,groups.'
 complete -c pdm -A -n '__fish_seen_subcommand_from list' -l freeze -d 'Show the installed dependencies in pip\'s requirements.txt format'
 complete -c pdm -A -n '__fish_seen_subcommand_from list' -l global -d 'Use the global project, supply the project root with `-p` option'
 complete -c pdm -A -n '__fish_seen_subcommand_from list' -l graph -d 'Display a graph of dependencies'
 complete -c pdm -A -n '__fish_seen_subcommand_from list' -l help -d 'Show this help message and exit.'
@@ -198,15 +200,15 @@
 complete -c pdm -A -n '__fish_seen_subcommand_from list' -l resolve -d 'Resolve all requirements to output licenses (instead of just showing those currently installed)'
 complete -c pdm -A -n '__fish_seen_subcommand_from list' -l reverse -d 'Reverse the dependency graph'
 complete -c pdm -A -n '__fish_seen_subcommand_from list' -l sort -d 'Sort the output using a given field name. If nothing is set, no sort is applied. Multiple fields can be combined with \',\'.'
 complete -c pdm -A -n '__fish_seen_subcommand_from list' -l venv -d 'Run the command in the virtual environment with the given key. [env var: PDM_IN_VENV]'
 complete -c pdm -A -n '__fish_seen_subcommand_from list' -l verbose -d 'Use `-v` for detailed output and `-vv` for more detailed'
 
 # lock
-complete -c pdm -f -n '__fish_pdm_c6f4c6c1a82f2f50_complete_no_subcommand' -a lock -d 'Resolve and lock dependencies'
+complete -c pdm -f -n '__fish_pdm_a919b69078acdf0a_complete_no_subcommand' -a lock -d 'Resolve and lock dependencies'
 complete -c pdm -A -n '__fish_seen_subcommand_from lock' -l check -d 'Check if the lock file is up to date and quit'
 complete -c pdm -A -n '__fish_seen_subcommand_from lock' -l dev -d 'Select dev dependencies'
 complete -c pdm -A -n '__fish_seen_subcommand_from lock' -l global -d 'Use the global project, supply the project root with `-p` option'
 complete -c pdm -A -n '__fish_seen_subcommand_from lock' -l group -d 'Select group of optional-dependencies separated by comma or dev-dependencies (with `-d`). Can be supplied multiple times, use ":all" to include all groups under the same species.'
 complete -c pdm -A -n '__fish_seen_subcommand_from lock' -l help -d 'Show this help message and exit.'
 complete -c pdm -A -n '__fish_seen_subcommand_from lock' -l lockfile -d 'Specify another lockfile path. Default: pdm.lock. [env var: PDM_LOCKFILE]'
 complete -c pdm -A -n '__fish_seen_subcommand_from lock' -l no-cross-platform -d 'Only lock packages for the current platform'
@@ -215,15 +217,15 @@
 complete -c pdm -A -n '__fish_seen_subcommand_from lock' -l production -d 'Unselect dev dependencies'
 complete -c pdm -A -n '__fish_seen_subcommand_from lock' -l project -d 'Specify another path as the project root, which changes the base of pyproject.toml and __pypackages__'
 complete -c pdm -A -n '__fish_seen_subcommand_from lock' -l refresh -d 'Don\'t update pinned versions, only refresh the lock file'
 complete -c pdm -A -n '__fish_seen_subcommand_from lock' -l skip -d 'Skip some tasks and/or hooks by their comma-separated names. Can be supplied multiple times. Use ":all" to skip all hooks. Use ":pre" and ":post" to skip all pre or post hooks.'
 complete -c pdm -A -n '__fish_seen_subcommand_from lock' -l verbose -d 'Use `-v` for detailed output and `-vv` for more detailed'
 
 # plugin
-complete -c pdm -f -n '__fish_pdm_c6f4c6c1a82f2f50_complete_no_subcommand' -a plugin -d 'Manage the PDM program itself (previously known as plugin)'
+complete -c pdm -f -n '__fish_pdm_a919b69078acdf0a_complete_no_subcommand' -a plugin -d 'Manage the PDM program itself (previously known as plugin)'
 complete -c pdm -A -n '__fish_seen_subcommand_from plugin' -l help -d 'Show this help message and exit.'
 complete -c pdm -A -n '__fish_seen_subcommand_from plugin' -l verbose -d 'Use `-v` for detailed output and `-vv` for more detailed'
 # plugin subcommands
 set -l plugin_subcommands add list remove update
 # plugin add
 complete -c pdm -f -n '__fish_seen_subcommand_from plugin; and not __fish_seen_subcommand_from $plugin_subcommands' -a add -d 'Install packages to the PDM\'s environment'
 complete -c pdm -A -n '__fish_seen_subcommand_from plugin; and __fish_seen_subcommand_from add' -l help -d 'Show this help message and exit.'
@@ -248,15 +250,15 @@
 complete -c pdm -A -n '__fish_seen_subcommand_from plugin; and __fish_seen_subcommand_from update' -l head -d 'Update to the latest commit on the main branch'
 complete -c pdm -A -n '__fish_seen_subcommand_from plugin; and __fish_seen_subcommand_from update' -l help -d 'Show this help message and exit.'
 complete -c pdm -A -n '__fish_seen_subcommand_from plugin; and __fish_seen_subcommand_from update' -l pip-args -d 'Additional arguments that will be passed to pip install'
 complete -c pdm -A -n '__fish_seen_subcommand_from plugin; and __fish_seen_subcommand_from update' -l pre -d 'Update to the latest prerelease version'
 complete -c pdm -A -n '__fish_seen_subcommand_from plugin; and __fish_seen_subcommand_from update' -l verbose -d 'Use `-v` for detailed output and `-vv` for more detailed'
 
 # publish
-complete -c pdm -f -n '__fish_pdm_c6f4c6c1a82f2f50_complete_no_subcommand' -a publish -d 'Build and publish the project to PyPI'
+complete -c pdm -f -n '__fish_pdm_a919b69078acdf0a_complete_no_subcommand' -a publish -d 'Build and publish the project to PyPI'
 complete -c pdm -A -n '__fish_seen_subcommand_from publish' -l ca-certs -d 'The path to a PEM-encoded Certificate Authority bundle to use for publish server validation [env var: PDM_PUBLISH_CA_CERTS]'
 complete -c pdm -A -n '__fish_seen_subcommand_from publish' -l comment -d 'The comment to include with the distribution file.'
 complete -c pdm -A -n '__fish_seen_subcommand_from publish' -l help -d 'Show this help message and exit.'
 complete -c pdm -A -n '__fish_seen_subcommand_from publish' -l identity -d 'GPG identity used to sign files.'
 complete -c pdm -A -n '__fish_seen_subcommand_from publish' -l no-build -d 'Don\'t build the package before publishing'
 complete -c pdm -A -n '__fish_seen_subcommand_from publish' -l no-very-ssl -d 'Disable SSL verification'
 complete -c pdm -A -n '__fish_seen_subcommand_from publish' -l password -d 'The password to access the repository [env var: PDM_PUBLISH_PASSWORD]'
@@ -264,15 +266,15 @@
 complete -c pdm -A -n '__fish_seen_subcommand_from publish' -l repository -d 'The repository name or url to publish the package to [env var: PDM_PUBLISH_REPO]'
 complete -c pdm -A -n '__fish_seen_subcommand_from publish' -l sign -d 'Upload the package with PGP signature'
 complete -c pdm -A -n '__fish_seen_subcommand_from publish' -l skip -d 'Skip some tasks and/or hooks by their comma-separated names. Can be supplied multiple times. Use ":all" to skip all hooks. Use ":pre" and ":post" to skip all pre or post hooks.'
 complete -c pdm -A -n '__fish_seen_subcommand_from publish' -l username -d 'The username to access the repository [env var: PDM_PUBLISH_USERNAME]'
 complete -c pdm -A -n '__fish_seen_subcommand_from publish' -l verbose -d 'Use `-v` for detailed output and `-vv` for more detailed'
 
 # remove
-complete -c pdm -f -n '__fish_pdm_c6f4c6c1a82f2f50_complete_no_subcommand' -a remove -d 'Remove packages from pyproject.toml'
+complete -c pdm -f -n '__fish_pdm_a919b69078acdf0a_complete_no_subcommand' -a remove -d 'Remove packages from pyproject.toml'
 complete -c pdm -A -n '__fish_seen_subcommand_from remove' -l dev -d 'Remove packages from dev dependencies'
 complete -c pdm -A -n '__fish_seen_subcommand_from remove' -l dry-run -d 'Show the difference only and don\'t perform any action'
 complete -c pdm -A -n '__fish_seen_subcommand_from remove' -l fail-fast -d 'Abort on first installation error'
 complete -c pdm -A -n '__fish_seen_subcommand_from remove' -l global -d 'Use the global project, supply the project root with `-p` option'
 complete -c pdm -A -n '__fish_seen_subcommand_from remove' -l group -d 'Specify the target dependency group to remove from'
 complete -c pdm -A -n '__fish_seen_subcommand_from remove' -l help -d 'Show this help message and exit.'
 complete -c pdm -A -n '__fish_seen_subcommand_from remove' -l lockfile -d 'Specify another lockfile path. Default: pdm.lock. [env var: PDM_LOCKFILE]'
@@ -282,32 +284,32 @@
 complete -c pdm -A -n '__fish_seen_subcommand_from remove' -l no-sync -d 'Only write pyproject.toml and do not uninstall packages'
 complete -c pdm -A -n '__fish_seen_subcommand_from remove' -l project -d 'Specify another path as the project root, which changes the base of pyproject.toml and __pypackages__'
 complete -c pdm -A -n '__fish_seen_subcommand_from remove' -l skip -d 'Skip some tasks and/or hooks by their comma-separated names. Can be supplied multiple times. Use ":all" to skip all hooks. Use ":pre" and ":post" to skip all pre or post hooks.'
 complete -c pdm -A -n '__fish_seen_subcommand_from remove' -l venv -d 'Run the command in the virtual environment with the given key. [env var: PDM_IN_VENV]'
 complete -c pdm -A -n '__fish_seen_subcommand_from remove' -l verbose -d 'Use `-v` for detailed output and `-vv` for more detailed'
 
 # run
-complete -c pdm -f -n '__fish_pdm_c6f4c6c1a82f2f50_complete_no_subcommand' -a run -d 'Run commands or scripts with local packages loaded'
+complete -c pdm -f -n '__fish_pdm_a919b69078acdf0a_complete_no_subcommand' -a run -d 'Run commands or scripts with local packages loaded'
 complete -c pdm -A -n '__fish_seen_subcommand_from run' -l global -d 'Use the global project, supply the project root with `-p` option'
 complete -c pdm -A -n '__fish_seen_subcommand_from run' -l help -d 'Show this help message and exit.'
 complete -c pdm -A -n '__fish_seen_subcommand_from run' -l json -d 'Output all scripts infos in JSON'
 complete -c pdm -A -n '__fish_seen_subcommand_from run' -l list -d 'Show all available scripts defined in pyproject.toml'
 complete -c pdm -A -n '__fish_seen_subcommand_from run' -l project -d 'Specify another path as the project root, which changes the base of pyproject.toml and __pypackages__'
 complete -c pdm -A -n '__fish_seen_subcommand_from run' -l site-packages -d 'Load site-packages from the selected interpreter'
 complete -c pdm -A -n '__fish_seen_subcommand_from run' -l skip -d 'Skip some tasks and/or hooks by their comma-separated names. Can be supplied multiple times. Use ":all" to skip all hooks. Use ":pre" and ":post" to skip all pre or post hooks.'
 complete -c pdm -A -n '__fish_seen_subcommand_from run' -l venv -d 'Run the command in the virtual environment with the given key. [env var: PDM_IN_VENV]'
 complete -c pdm -A -n '__fish_seen_subcommand_from run' -l verbose -d 'Use `-v` for detailed output and `-vv` for more detailed'
 
 # search
-complete -c pdm -f -n '__fish_pdm_c6f4c6c1a82f2f50_complete_no_subcommand' -a search -d 'Search for PyPI packages'
+complete -c pdm -f -n '__fish_pdm_a919b69078acdf0a_complete_no_subcommand' -a search -d 'Search for PyPI packages'
 complete -c pdm -A -n '__fish_seen_subcommand_from search' -l help -d 'Show this help message and exit.'
 complete -c pdm -A -n '__fish_seen_subcommand_from search' -l verbose -d 'Use `-v` for detailed output and `-vv` for more detailed'
 
 # self
-complete -c pdm -f -n '__fish_pdm_c6f4c6c1a82f2f50_complete_no_subcommand' -a self -d 'Manage the PDM program itself (previously known as plugin)'
+complete -c pdm -f -n '__fish_pdm_a919b69078acdf0a_complete_no_subcommand' -a self -d 'Manage the PDM program itself (previously known as plugin)'
 complete -c pdm -A -n '__fish_seen_subcommand_from self' -l help -d 'Show this help message and exit.'
 complete -c pdm -A -n '__fish_seen_subcommand_from self' -l verbose -d 'Use `-v` for detailed output and `-vv` for more detailed'
 # self subcommands
 set -l self_subcommands add list remove update
 # self add
 complete -c pdm -f -n '__fish_seen_subcommand_from self; and not __fish_seen_subcommand_from $self_subcommands' -a add -d 'Install packages to the PDM\'s environment'
 complete -c pdm -A -n '__fish_seen_subcommand_from self; and __fish_seen_subcommand_from add' -l help -d 'Show this help message and exit.'
@@ -332,29 +334,29 @@
 complete -c pdm -A -n '__fish_seen_subcommand_from self; and __fish_seen_subcommand_from update' -l head -d 'Update to the latest commit on the main branch'
 complete -c pdm -A -n '__fish_seen_subcommand_from self; and __fish_seen_subcommand_from update' -l help -d 'Show this help message and exit.'
 complete -c pdm -A -n '__fish_seen_subcommand_from self; and __fish_seen_subcommand_from update' -l pip-args -d 'Additional arguments that will be passed to pip install'
 complete -c pdm -A -n '__fish_seen_subcommand_from self; and __fish_seen_subcommand_from update' -l pre -d 'Update to the latest prerelease version'
 complete -c pdm -A -n '__fish_seen_subcommand_from self; and __fish_seen_subcommand_from update' -l verbose -d 'Use `-v` for detailed output and `-vv` for more detailed'
 
 # show
-complete -c pdm -f -n '__fish_pdm_c6f4c6c1a82f2f50_complete_no_subcommand' -a show -d 'Show the package information'
+complete -c pdm -f -n '__fish_pdm_a919b69078acdf0a_complete_no_subcommand' -a show -d 'Show the package information'
 complete -c pdm -A -n '__fish_seen_subcommand_from show' -l global -d 'Use the global project, supply the project root with `-p` option'
 complete -c pdm -A -n '__fish_seen_subcommand_from show' -l help -d 'Show this help message and exit.'
 complete -c pdm -A -n '__fish_seen_subcommand_from show' -l keywords -d 'Show keywords'
 complete -c pdm -A -n '__fish_seen_subcommand_from show' -l license -d 'Show license'
 complete -c pdm -A -n '__fish_seen_subcommand_from show' -l name -d 'Show name'
 complete -c pdm -A -n '__fish_seen_subcommand_from show' -l platform -d 'Show platform'
 complete -c pdm -A -n '__fish_seen_subcommand_from show' -l project -d 'Specify another path as the project root, which changes the base of pyproject.toml and __pypackages__'
 complete -c pdm -A -n '__fish_seen_subcommand_from show' -l summary -d 'Show summary'
 complete -c pdm -A -n '__fish_seen_subcommand_from show' -l venv -d 'Run the command in the virtual environment with the given key. [env var: PDM_IN_VENV]'
 complete -c pdm -A -n '__fish_seen_subcommand_from show' -l verbose -d 'Use `-v` for detailed output and `-vv` for more detailed'
 complete -c pdm -A -n '__fish_seen_subcommand_from show' -l version -d 'Show version'
 
 # sync
-complete -c pdm -f -n '__fish_pdm_c6f4c6c1a82f2f50_complete_no_subcommand' -a sync -d 'Synchronize the current working set with lock file'
+complete -c pdm -f -n '__fish_pdm_a919b69078acdf0a_complete_no_subcommand' -a sync -d 'Synchronize the current working set with lock file'
 complete -c pdm -A -n '__fish_seen_subcommand_from sync' -l clean -d 'Clean packages not in the lockfile'
 complete -c pdm -A -n '__fish_seen_subcommand_from sync' -l dev -d 'Select dev dependencies'
 complete -c pdm -A -n '__fish_seen_subcommand_from sync' -l dry-run -d 'Show the difference only and don\'t perform any action'
 complete -c pdm -A -n '__fish_seen_subcommand_from sync' -l fail-fast -d 'Abort on first installation error'
 complete -c pdm -A -n '__fish_seen_subcommand_from sync' -l global -d 'Use the global project, supply the project root with `-p` option'
 complete -c pdm -A -n '__fish_seen_subcommand_from sync' -l group -d 'Select group of optional-dependencies separated by comma or dev-dependencies (with `-d`). Can be supplied multiple times, use ":all" to include all groups under the same species.'
 complete -c pdm -A -n '__fish_seen_subcommand_from sync' -l help -d 'Show this help message and exit.'
@@ -368,15 +370,15 @@
 complete -c pdm -A -n '__fish_seen_subcommand_from sync' -l project -d 'Specify another path as the project root, which changes the base of pyproject.toml and __pypackages__'
 complete -c pdm -A -n '__fish_seen_subcommand_from sync' -l reinstall -d 'Force reinstall existing dependencies'
 complete -c pdm -A -n '__fish_seen_subcommand_from sync' -l skip -d 'Skip some tasks and/or hooks by their comma-separated names. Can be supplied multiple times. Use ":all" to skip all hooks. Use ":pre" and ":post" to skip all pre or post hooks.'
 complete -c pdm -A -n '__fish_seen_subcommand_from sync' -l venv -d 'Run the command in the virtual environment with the given key. [env var: PDM_IN_VENV]'
 complete -c pdm -A -n '__fish_seen_subcommand_from sync' -l verbose -d 'Use `-v` for detailed output and `-vv` for more detailed'
 
 # update
-complete -c pdm -f -n '__fish_pdm_c6f4c6c1a82f2f50_complete_no_subcommand' -a update -d 'Update package(s) in pyproject.toml'
+complete -c pdm -f -n '__fish_pdm_a919b69078acdf0a_complete_no_subcommand' -a update -d 'Update package(s) in pyproject.toml'
 complete -c pdm -A -n '__fish_seen_subcommand_from update' -l dev -d 'Select dev dependencies'
 complete -c pdm -A -n '__fish_seen_subcommand_from update' -l fail-fast -d 'Abort on first installation error'
 complete -c pdm -A -n '__fish_seen_subcommand_from update' -l global -d 'Use the global project, supply the project root with `-p` option'
 complete -c pdm -A -n '__fish_seen_subcommand_from update' -l group -d 'Select group of optional-dependencies separated by comma or dev-dependencies (with `-d`). Can be supplied multiple times, use ":all" to include all groups under the same species.'
 complete -c pdm -A -n '__fish_seen_subcommand_from update' -l help -d 'Show this help message and exit.'
 complete -c pdm -A -n '__fish_seen_subcommand_from update' -l lockfile -d 'Specify another lockfile path. Default: pdm.lock. [env var: PDM_LOCKFILE]'
 complete -c pdm -A -n '__fish_seen_subcommand_from update' -l no-default -d 'Don\'t include dependencies from the default group'
@@ -398,26 +400,26 @@
 complete -c pdm -A -n '__fish_seen_subcommand_from update' -l update-all -d 'Update all dependencies and sub-dependencies'
 complete -c pdm -A -n '__fish_seen_subcommand_from update' -l update-eager -d 'Try to update the packages and their dependencies recursively'
 complete -c pdm -A -n '__fish_seen_subcommand_from update' -l update-reuse -d 'Reuse pinned versions already present in lock file if possible'
 complete -c pdm -A -n '__fish_seen_subcommand_from update' -l venv -d 'Run the command in the virtual environment with the given key. [env var: PDM_IN_VENV]'
 complete -c pdm -A -n '__fish_seen_subcommand_from update' -l verbose -d 'Use `-v` for detailed output and `-vv` for more detailed'
 
 # use
-complete -c pdm -f -n '__fish_pdm_c6f4c6c1a82f2f50_complete_no_subcommand' -a use -d 'Use the given python version or path as base interpreter'
+complete -c pdm -f -n '__fish_pdm_a919b69078acdf0a_complete_no_subcommand' -a use -d 'Use the given python version or path as base interpreter'
 complete -c pdm -A -n '__fish_seen_subcommand_from use' -l first -d 'Select the first matched interpreter'
 complete -c pdm -A -n '__fish_seen_subcommand_from use' -l global -d 'Use the global project, supply the project root with `-p` option'
 complete -c pdm -A -n '__fish_seen_subcommand_from use' -l help -d 'Show this help message and exit.'
 complete -c pdm -A -n '__fish_seen_subcommand_from use' -l ignore-remembered -d 'Ignore the remembered selection'
 complete -c pdm -A -n '__fish_seen_subcommand_from use' -l project -d 'Specify another path as the project root, which changes the base of pyproject.toml and __pypackages__'
 complete -c pdm -A -n '__fish_seen_subcommand_from use' -l skip -d 'Skip some tasks and/or hooks by their comma-separated names. Can be supplied multiple times. Use ":all" to skip all hooks. Use ":pre" and ":post" to skip all pre or post hooks.'
 complete -c pdm -A -n '__fish_seen_subcommand_from use' -l venv -d 'Use the interpreter in the virtual environment with the given name'
 complete -c pdm -A -n '__fish_seen_subcommand_from use' -l verbose -d 'Use `-v` for detailed output and `-vv` for more detailed'
 
 # venv
-complete -c pdm -f -n '__fish_pdm_c6f4c6c1a82f2f50_complete_no_subcommand' -a venv -d 'Virtualenv management'
+complete -c pdm -f -n '__fish_pdm_a919b69078acdf0a_complete_no_subcommand' -a venv -d 'Virtualenv management'
 complete -c pdm -A -n '__fish_seen_subcommand_from venv' -l help -d 'Show this help message and exit.'
 complete -c pdm -A -n '__fish_seen_subcommand_from venv' -l path -d 'Show the path to the given virtualenv'
 complete -c pdm -A -n '__fish_seen_subcommand_from venv' -l project -d 'Specify another path as the project root, which changes the base of pyproject.toml and __pypackages__'
 complete -c pdm -A -n '__fish_seen_subcommand_from venv' -l python -d 'Show the python interpreter path for the given virtualenv'
 # venv subcommands
 set -l venv_subcommands activate create list purge remove
 # venv activate
```

### Comparing `pdm-2.8.0a0/src/pdm/cli/completions/pdm.ps1` & `pdm-2.8.0a1/src/pdm/cli/completions/pdm.ps1`

 * *Files 0% similar despite different names*

```diff
@@ -278,15 +278,15 @@
                         $venvOption
                     ))
                 break
             }
             "init" {
                 $completer.AddOpts(
                     @(
-                        [Option]::new(@("-g", "--global", "--non-interactive", "-n", "--python", "--lib")),
+                        [Option]::new(@("-g", "--global", "--non-interactive", "-n", "--python", "--lib", "--copier", "--cookiecutter")),
                         $projectOption,
                         $skipOption,
                         [Option]::new(@("--backend")).WithValues(@("pdm-backend", "setuptools", "flit", "hatching", "pdm-pep517"))
                     ))
                 break
             }
             "install" {
```

### Comparing `pdm-2.8.0a0/src/pdm/cli/completions/pdm.zsh` & `pdm-2.8.0a1/src/pdm/cli/completions/pdm.zsh`

 * *Files 1% similar despite different names*

```diff
@@ -184,15 +184,17 @@
       arguments+=(
         {-g,--global}'[Use the global project, supply the project root with `-p` option]'
         {-n,--non-interactive}"[Don't ask questions but use default values]"
         {-k,--skip}'[Skip some tasks and/or hooks by their comma-separated names]'
         '--backend[Specify the build backend]:backend:(pdm-backend setuptools hatchling flit pdm-pep517)'
         '--lib[Create a library project]'
         '--python[Specify the Python version/path to use]:python:'
-        '1:filename:_files'
+        '--copier[Use Copier to generate project]'
+        '--cookiecutter[Use Cookiecutter to generate project]'
+        '1:template:'
       )
       ;;
     install)
       arguments+=(
         {-g,--global}'[Use the global project, supply the project root with `-p` option]'
         {-G+,--group+}'[Select group of optional-dependencies or dev-dependencies(with -d). Can be supplied multiple times, use ":all" to include all groups under the same species]:group:_pdm_groups'
         {-d,--dev}"[Select dev dependencies]"
```

### Comparing `pdm-2.8.0a0/src/pdm/cli/filters.py` & `pdm-2.8.0a1/src/pdm/cli/filters.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a0/src/pdm/cli/hooks.py` & `pdm-2.8.0a1/src/pdm/cli/hooks.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a0/src/pdm/cli/options.py` & `pdm-2.8.0a1/src/pdm/cli/options.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a0/src/pdm/cli/templates/__init__.py` & `pdm-2.8.0a1/src/pdm/cli/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a0/src/pdm/cli/templates/default/.gitignore` & `pdm-2.8.0a1/src/pdm/cli/templates/default/.gitignore`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a0/src/pdm/cli/utils.py` & `pdm-2.8.0a1/src/pdm/cli/utils.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a0/src/pdm/compat.py` & `pdm-2.8.0a1/src/pdm/compat.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a0/src/pdm/core.py` & `pdm-2.8.0a1/src/pdm/core.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a0/src/pdm/environments/__init__.py` & `pdm-2.8.0a1/src/pdm/environments/__init__.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a0/src/pdm/environments/base.py` & `pdm-2.8.0a1/src/pdm/environments/base.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a0/src/pdm/environments/local.py` & `pdm-2.8.0a1/src/pdm/environments/local.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a0/src/pdm/environments/python.py` & `pdm-2.8.0a1/src/pdm/environments/python.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a0/src/pdm/exceptions.py` & `pdm-2.8.0a1/src/pdm/exceptions.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a0/src/pdm/formats/__init__.py` & `pdm-2.8.0a1/src/pdm/formats/__init__.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a0/src/pdm/formats/base.py` & `pdm-2.8.0a1/src/pdm/formats/base.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a0/src/pdm/formats/flit.py` & `pdm-2.8.0a1/src/pdm/formats/flit.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a0/src/pdm/formats/pipfile.py` & `pdm-2.8.0a1/src/pdm/formats/pipfile.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a0/src/pdm/formats/poetry.py` & `pdm-2.8.0a1/src/pdm/formats/poetry.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a0/src/pdm/formats/requirements.py` & `pdm-2.8.0a1/src/pdm/formats/requirements.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a0/src/pdm/formats/setup_py.py` & `pdm-2.8.0a1/src/pdm/formats/setup_py.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a0/src/pdm/installers/core.py` & `pdm-2.8.0a1/src/pdm/installers/core.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a0/src/pdm/installers/installers.py` & `pdm-2.8.0a1/src/pdm/installers/installers.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a0/src/pdm/installers/manager.py` & `pdm-2.8.0a1/src/pdm/installers/manager.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a0/src/pdm/installers/packages.py` & `pdm-2.8.0a1/src/pdm/installers/packages.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a0/src/pdm/installers/synchronizers.py` & `pdm-2.8.0a1/src/pdm/installers/synchronizers.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a0/src/pdm/installers/uninstallers.py` & `pdm-2.8.0a1/src/pdm/installers/uninstallers.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a0/src/pdm/models/auth.py` & `pdm-2.8.0a1/src/pdm/models/auth.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a0/src/pdm/models/backends.py` & `pdm-2.8.0a1/src/pdm/models/backends.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a0/src/pdm/models/caches.py` & `pdm-2.8.0a1/src/pdm/models/caches.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a0/src/pdm/models/candidates.py` & `pdm-2.8.0a1/src/pdm/models/candidates.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a0/src/pdm/models/in_process/__init__.py` & `pdm-2.8.0a1/src/pdm/models/in_process/__init__.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a0/src/pdm/models/in_process/get_abi_tag.py` & `pdm-2.8.0a1/src/pdm/models/in_process/get_abi_tag.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a0/src/pdm/models/in_process/parse_setup.py` & `pdm-2.8.0a1/src/pdm/models/in_process/parse_setup.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a0/src/pdm/models/in_process/pep508.py` & `pdm-2.8.0a1/src/pdm/models/in_process/pep508.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a0/src/pdm/models/in_process/sysconfig_get_paths.py` & `pdm-2.8.0a1/src/pdm/models/in_process/sysconfig_get_paths.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a0/src/pdm/models/markers.py` & `pdm-2.8.0a1/src/pdm/models/markers.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a0/src/pdm/models/project_info.py` & `pdm-2.8.0a1/src/pdm/models/project_info.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a0/src/pdm/models/python.py` & `pdm-2.8.0a1/src/pdm/models/python.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a0/src/pdm/models/repositories.py` & `pdm-2.8.0a1/src/pdm/models/repositories.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a0/src/pdm/models/requirements.py` & `pdm-2.8.0a1/src/pdm/models/requirements.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a0/src/pdm/models/search.py` & `pdm-2.8.0a1/src/pdm/models/search.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a0/src/pdm/models/session.py` & `pdm-2.8.0a1/src/pdm/models/session.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from __future__ import annotations
 
 import functools
+import sys
 from pathlib import Path
 from typing import IO, TYPE_CHECKING, Any, Mapping
 
 from cachecontrol import CacheControlAdapter as BaseCCAdapter
 from cachecontrol.serialize import Serializer
 from requests import Request
 from requests_toolbelt.utils import user_agent
@@ -16,14 +17,18 @@
 if TYPE_CHECKING:
     from ssl import SSLContext
 
     from urllib3 import HTTPResponse
 
 
 def _create_truststore_ssl_context() -> SSLContext | None:
+    if sys.version_info < (3, 10):
+        logger.warning("truststore is not available on Python < 3.10")
+        return None
+
     try:
         import ssl
     except ImportError:
         logger.warning("Disabling truststore since ssl support is missing")
         return None
 
     try:
```

### Comparing `pdm-2.8.0a0/src/pdm/models/setup.py` & `pdm-2.8.0a1/src/pdm/models/setup.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a0/src/pdm/models/specifiers.py` & `pdm-2.8.0a1/src/pdm/models/specifiers.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a0/src/pdm/models/venv.py` & `pdm-2.8.0a1/src/pdm/models/venv.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a0/src/pdm/models/versions.py` & `pdm-2.8.0a1/src/pdm/models/versions.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a0/src/pdm/models/working_set.py` & `pdm-2.8.0a1/src/pdm/models/working_set.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a0/src/pdm/pep582/sitecustomize.py` & `pdm-2.8.0a1/src/pdm/pep582/sitecustomize.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a0/src/pdm/project/config.py` & `pdm-2.8.0a1/src/pdm/project/config.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a0/src/pdm/project/core.py` & `pdm-2.8.0a1/src/pdm/project/core.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a0/src/pdm/project/lockfile.py` & `pdm-2.8.0a1/src/pdm/project/lockfile.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a0/src/pdm/project/project_file.py` & `pdm-2.8.0a1/src/pdm/project/project_file.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a0/src/pdm/project/toml_file.py` & `pdm-2.8.0a1/src/pdm/project/toml_file.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a0/src/pdm/pytest.py` & `pdm-2.8.0a1/src/pdm/pytest.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,14 @@
 from __future__ import annotations
 
 import collections
 import json
 import os
 import shutil
 import sys
-from argparse import Namespace
 from dataclasses import dataclass
 from io import BufferedReader, BytesIO, StringIO
 from pathlib import Path
 from typing import (
     TYPE_CHECKING,
     Any,
     BinaryIO,
@@ -46,15 +45,14 @@
 
 import pytest
 import requests
 from packaging.version import parse as parse_version
 from pytest_mock import MockerFixture
 from unearth import Link
 
-from pdm.cli.hooks import HookManager
 from pdm.core import Core
 from pdm.environments import BaseEnvironment, PythonEnvironment
 from pdm.exceptions import CandidateInfoNotFound
 from pdm.installers.installers import install_wheel
 from pdm.models.backends import DEFAULT_BACKEND
 from pdm.models.candidates import Candidate
 from pdm.models.repositories import BaseRepository
@@ -416,31 +414,31 @@
 def project(project_no_init: Project) -> Project:
     """
     A fixture creating an initialized test project for the current test.
 
     Returns:
         The initialized project
     """
-    from pdm.cli.commands.init import Command
+    from pdm.cli.utils import merge_dictionary
 
-    hooks = HookManager(project_no_init, ["post_init"])
     data = {
         "project": {
             "name": "test-project",
             "version": "0.0.0",
             "description": "",
             "authors": [],
             "license": {"text": "MIT"},
             "dependencies": [],
             "requires-python": ">=3.7",
         },
         "build-system": DEFAULT_BACKEND.build_system(),
     }
 
-    Command().do_init(project_no_init, data, hooks=hooks, options=Namespace(template=None))
+    merge_dictionary(project_no_init.pyproject._data, data)
+    project_no_init.pyproject.write()
     # Clean the cached property
     project_no_init._environment = None
     return project_no_init
 
 
 @pytest.fixture
 def working_set(mocker: MockerFixture, repository: TestRepository) -> MockWorkingSet:
```

### Comparing `pdm-2.8.0a0/src/pdm/resolver/core.py` & `pdm-2.8.0a1/src/pdm/resolver/core.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a0/src/pdm/resolver/providers.py` & `pdm-2.8.0a1/src/pdm/resolver/providers.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a0/src/pdm/resolver/python.py` & `pdm-2.8.0a1/src/pdm/resolver/python.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a0/src/pdm/resolver/reporters.py` & `pdm-2.8.0a1/src/pdm/resolver/reporters.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a0/src/pdm/signals.py` & `pdm-2.8.0a1/src/pdm/signals.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a0/src/pdm/termui.py` & `pdm-2.8.0a1/src/pdm/termui.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a0/src/pdm/utils.py` & `pdm-2.8.0a1/src/pdm/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -434,7 +434,17 @@
         return Path(path)
     return Path(match.group(1))
 
 
 def is_in_zipapp() -> bool:
     """Check if the current process is running in a zipapp"""
     return not os.path.exists(__file__)
+
+
+@functools.lru_cache(None)
+def package_installed(package_name: str) -> bool:
+    try:
+        importlib_metadata.distribution(package_name)
+    except importlib_metadata.PackageNotFoundError:
+        return False
+    else:
+        return True
```

### Comparing `pdm-2.8.0a0/tests/cli/conftest.py` & `pdm-2.8.0a1/tests/cli/conftest.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a0/tests/cli/test_add.py` & `pdm-2.8.0a1/tests/cli/test_add.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a0/tests/cli/test_build.py` & `pdm-2.8.0a1/tests/cli/test_build.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a0/tests/cli/test_cache.py` & `pdm-2.8.0a1/tests/cli/test_cache.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a0/tests/cli/test_config.py` & `pdm-2.8.0a1/tests/cli/test_config.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a0/tests/cli/test_fix.py` & `pdm-2.8.0a1/tests/cli/test_fix.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a0/tests/cli/test_hooks.py` & `pdm-2.8.0a1/tests/cli/test_hooks.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a0/tests/cli/test_init.py` & `pdm-2.8.0a1/tests/cli/test_init.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a0/tests/cli/test_install.py` & `pdm-2.8.0a1/tests/cli/test_install.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a0/tests/cli/test_list.py` & `pdm-2.8.0a1/tests/cli/test_list.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a0/tests/cli/test_lock.py` & `pdm-2.8.0a1/tests/cli/test_lock.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a0/tests/cli/test_others.py` & `pdm-2.8.0a1/tests/cli/test_others.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a0/tests/cli/test_publish.py` & `pdm-2.8.0a1/tests/cli/test_publish.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a0/tests/cli/test_remove.py` & `pdm-2.8.0a1/tests/cli/test_remove.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a0/tests/cli/test_run.py` & `pdm-2.8.0a1/tests/cli/test_run.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a0/tests/cli/test_self_command.py` & `pdm-2.8.0a1/tests/cli/test_self_command.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a0/tests/cli/test_template.py` & `pdm-2.8.0a1/tests/cli/test_template.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a0/tests/cli/test_update.py` & `pdm-2.8.0a1/tests/cli/test_update.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a0/tests/cli/test_use.py` & `pdm-2.8.0a1/tests/cli/test_use.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a0/tests/cli/test_venv.py` & `pdm-2.8.0a1/tests/cli/test_venv.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a0/tests/conftest.py` & `pdm-2.8.0a1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a0/tests/fixtures/artifacts/PyFunctional-1.4.3-py3-none-any.whl` & `pdm-2.8.0a1/tests/fixtures/artifacts/PyFunctional-1.4.3-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a0/tests/fixtures/artifacts/caj2pdf-restructured-0.1.0a6.tar.gz` & `pdm-2.8.0a1/tests/fixtures/artifacts/caj2pdf-restructured-0.1.0a6.tar.gz`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a0/tests/fixtures/artifacts/celery-4.4.2-py2.py3-none-any.whl` & `pdm-2.8.0a1/tests/fixtures/artifacts/celery-4.4.2-py2.py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a0/tests/fixtures/artifacts/demo-0.0.1-cp36-cp36m-win_amd64.whl` & `pdm-2.8.0a1/tests/fixtures/artifacts/demo-0.0.1-cp36-cp36m-win_amd64.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a0/tests/fixtures/artifacts/demo-0.0.1-py2.py3-none-any.whl` & `pdm-2.8.0a1/tests/fixtures/artifacts/demo-0.0.1-py2.py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a0/tests/fixtures/artifacts/demo-0.0.1.tar.gz` & `pdm-2.8.0a1/tests/fixtures/artifacts/demo-0.0.1.tar.gz`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a0/tests/fixtures/artifacts/demo-0.0.1.zip` & `pdm-2.8.0a1/tests/fixtures/artifacts/demo-0.0.1.zip`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a0/tests/fixtures/artifacts/editables-0.2-py3-none-any.whl` & `pdm-2.8.0a1/tests/fixtures/artifacts/editables-0.2-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a0/tests/fixtures/artifacts/first-2.0.2-py2.py3-none-any.whl` & `pdm-2.8.0a1/tests/fixtures/artifacts/first-2.0.2-py2.py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a0/tests/fixtures/artifacts/flit_core-3.6.0-py3-none-any.whl` & `pdm-2.8.0a1/tests/fixtures/artifacts/flit_core-3.6.0-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a0/tests/fixtures/artifacts/future_fstrings-1.2.0-py2.py3-none-any.whl` & `pdm-2.8.0a1/tests/fixtures/artifacts/future_fstrings-1.2.0-py2.py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a0/tests/fixtures/artifacts/future_fstrings-1.2.0.tar.gz` & `pdm-2.8.0a1/tests/fixtures/artifacts/future_fstrings-1.2.0.tar.gz`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a0/tests/fixtures/artifacts/importlib_metadata-4.8.3-py3-none-any.whl` & `pdm-2.8.0a1/tests/fixtures/artifacts/importlib_metadata-4.8.3-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a0/tests/fixtures/artifacts/jmespath-0.10.0-py2.py3-none-any.whl` & `pdm-2.8.0a1/tests/fixtures/artifacts/jmespath-0.10.0-py2.py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a0/tests/fixtures/artifacts/pdm_backend-2.0.2-py3-none-any.whl` & `pdm-2.8.0a1/tests/fixtures/artifacts/pdm_backend-2.0.2-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a0/tests/fixtures/artifacts/pdm_hello-0.1.0-py3-none-any.whl` & `pdm-2.8.0a1/tests/fixtures/artifacts/pdm_hello-0.1.0-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a0/tests/fixtures/artifacts/pdm_hello-0.1.0-py3-none-win_amd64.whl` & `pdm-2.8.0a1/tests/fixtures/artifacts/pdm_hello-0.1.0-py3-none-win_amd64.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a0/tests/fixtures/artifacts/pdm_pep517-1.0.0-py3-none-any.whl` & `pdm-2.8.0a1/tests/fixtures/artifacts/pdm_pep517-1.0.0-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a0/tests/fixtures/artifacts/poetry_core-1.3.2-py3-none-any.whl` & `pdm-2.8.0a1/tests/fixtures/artifacts/poetry_core-1.3.2-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a0/tests/fixtures/artifacts/setuptools-65.4.1-py3-none-any.whl` & `pdm-2.8.0a1/tests/fixtures/artifacts/setuptools-65.4.1-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a0/tests/fixtures/artifacts/typing_extensions-4.4.0-py3-none-any.whl` & `pdm-2.8.0a1/tests/fixtures/artifacts/typing_extensions-4.4.0-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a0/tests/fixtures/artifacts/wheel-0.37.1-py2.py3-none-any.whl` & `pdm-2.8.0a1/tests/fixtures/artifacts/wheel-0.37.1-py2.py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a0/tests/fixtures/artifacts/zipp-3.7.0-py3-none-any.whl` & `pdm-2.8.0a1/tests/fixtures/artifacts/zipp-3.7.0-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a0/tests/fixtures/projects/demo-package-has-dep-with-extras/pdm.lock` & `pdm-2.8.0a1/tests/fixtures/projects/demo-package-has-dep-with-extras/pdm.lock`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a0/tests/fixtures/projects/demo-package/pdm.lock` & `pdm-2.8.0a1/tests/fixtures/projects/demo-package/pdm.lock`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a0/tests/fixtures/projects/demo-package/pyproject.toml` & `pdm-2.8.0a1/tests/fixtures/projects/demo-package/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a0/tests/fixtures/projects/demo-package/requirements.txt` & `pdm-2.8.0a1/tests/fixtures/projects/demo-package/requirements.txt`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a0/tests/fixtures/projects/demo-package/setup.txt` & `pdm-2.8.0a1/tests/fixtures/projects/demo-package/setup.txt`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a0/tests/fixtures/projects/flit-demo/pyproject.toml` & `pdm-2.8.0a1/tests/fixtures/projects/flit-demo/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a0/tests/fixtures/projects/poetry-demo/pyproject.toml` & `pdm-2.8.0a1/tests/fixtures/projects/poetry-demo/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a0/tests/fixtures/pypi.json` & `pdm-2.8.0a1/tests/fixtures/pypi.json`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a0/tests/fixtures/pyproject.toml` & `pdm-2.8.0a1/tests/fixtures/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a0/tests/models/test_backends.py` & `pdm-2.8.0a1/tests/models/test_backends.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a0/tests/models/test_candidates.py` & `pdm-2.8.0a1/tests/models/test_candidates.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a0/tests/models/test_marker.py` & `pdm-2.8.0a1/tests/models/test_marker.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a0/tests/models/test_requirements.py` & `pdm-2.8.0a1/tests/models/test_requirements.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a0/tests/models/test_setup_parsing.py` & `pdm-2.8.0a1/tests/models/test_setup_parsing.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a0/tests/models/test_specifiers.py` & `pdm-2.8.0a1/tests/models/test_specifiers.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a0/tests/models/test_versions.py` & `pdm-2.8.0a1/tests/models/test_versions.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a0/tests/resolver/test_resolve.py` & `pdm-2.8.0a1/tests/resolver/test_resolve.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a0/tests/test_formats.py` & `pdm-2.8.0a1/tests/test_formats.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a0/tests/test_installer.py` & `pdm-2.8.0a1/tests/test_installer.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a0/tests/test_integration.py` & `pdm-2.8.0a1/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a0/tests/test_plugin.py` & `pdm-2.8.0a1/tests/test_plugin.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a0/tests/test_project.py` & `pdm-2.8.0a1/tests/test_project.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a0/tests/test_signals.py` & `pdm-2.8.0a1/tests/test_signals.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a0/tests/test_utils.py` & `pdm-2.8.0a1/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `pdm-2.8.0a0/PKG-INFO` & `pdm-2.8.0a1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdm
-Version: 2.8.0a0
+Version: 2.8.0a1
 Summary: A modern Python package and dependency manager supporting the latest PEP standards
 Keywords: packaging dependency workflow
 Author-Email: Frost Ming <mianghong@gmail.com>
 License: MIT
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
@@ -34,15 +34,20 @@
 Requires-Dist: installer<0.8,>=0.7
 Requires-Dist: cachecontrol[filecache]>=0.13.0
 Requires-Dist: tomli>=1.1.0; python_version < "3.11"
 Requires-Dist: importlib-resources>=5; python_version < "3.9"
 Requires-Dist: importlib-metadata>=3.6; python_version < "3.10"
 Requires-Dist: pytest; extra == "pytest"
 Requires-Dist: pytest-mock; extra == "pytest"
+Requires-Dist: copier; extra == "all"
+Requires-Dist: cookiecutter; extra == "all"
+Requires-Dist: keyring; extra == "all"
+Requires-Dist: truststore; python_version >= "3.10" and extra == "all"
 Provides-Extra: pytest
+Provides-Extra: all
 Description-Content-Type: text/markdown
 
 <div align="center">
 
 # PDM
 
 A modern Python package and dependency manager supporting the latest PEP standards.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pdm Version: 2.8.0a0 Summary: A modern Python
+Metadata-Version: 2.1 Name: pdm Version: 2.8.0a1 Summary: A modern Python
 package and dependency manager supporting the latest PEP standards Keywords:
 packaging dependency workflow Author-Email: Frost Ming
 gmail.com> License: MIT Classifier: Topic :: Software Development :: Build
 Tools Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
@@ -15,16 +15,19 @@
 requests-toolbelt Requires-Dist: unearth>=0.9.0 Requires-Dist:
 findpython>=0.2.2 Requires-Dist: tomlkit<1,>=0.11.1 Requires-Dist:
 shellingham>=1.3.2 Requires-Dist: python-dotenv>=0.15 Requires-Dist:
 resolvelib>=1.0.1 Requires-Dist: installer<0.8,>=0.7 Requires-Dist:
 cachecontrol[filecache]>=0.13.0 Requires-Dist: tomli>=1.1.0; python_version <
 "3.11" Requires-Dist: importlib-resources>=5; python_version < "3.9" Requires-
 Dist: importlib-metadata>=3.6; python_version < "3.10" Requires-Dist: pytest;
-extra == "pytest" Requires-Dist: pytest-mock; extra == "pytest" Provides-Extra:
-pytest Description-Content-Type: text/markdown
+extra == "pytest" Requires-Dist: pytest-mock; extra == "pytest" Requires-Dist:
+copier; extra == "all" Requires-Dist: cookiecutter; extra == "all" Requires-
+Dist: keyring; extra == "all" Requires-Dist: truststore; python_version >=
+"3.10" and extra == "all" Provides-Extra: pytest Provides-Extra: all
+Description-Content-Type: text/markdown
 # PDM A modern Python package and dependency manager supporting the latest PEP
       standards. [ä¸­æçæ¬è¯´æ](README_zh.md) ![PDM logo](https://
 raw.githubusercontent.com/pdm-project/pdm/main/docs/docs/assets/logo_big.png)
  [![Docs](https://img.shields.io/badge/Docs-mkdocs-blue?style=for-the-badge)]
   (https://pdm.fming.dev) [![Twitter Follow](https://img.shields.io/twitter/
    follow/pdm_project?label=get%20updates&logo=twitter&style=for-the-badge)]
  (https://twitter.com/pdm_project) [![Discord](https://img.shields.io/discord/
```

