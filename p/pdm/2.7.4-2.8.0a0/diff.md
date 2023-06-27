# Comparing `tmp/pdm-2.7.4.tar.gz` & `tmp/pdm-2.8.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdm-2.7.4.tar", last modified: Tue Jun 13 04:51:14 2023, max compression
+gzip compressed data, was "pdm-2.8.0a0.tar", last modified: Tue Jun 27 02:38:15 2023, max compression
```

## Comparing `pdm-2.7.4.tar` & `pdm-2.8.0a0.tar`

### file list

```diff
@@ -1,272 +1,280 @@
--rw-r--r--   0        0        0   124084 2023-06-13 04:51:05.335390 pdm-2.7.4/CHANGELOG.md
--rw-r--r--   0        0        0     1075 2023-06-13 04:51:05.335390 pdm-2.7.4/LICENSE
--rw-r--r--   0        0        0     1075 2023-06-13 04:51:05.335390 pdm-2.7.4/LICENSE
--rw-r--r--   0        0        0     7986 2023-06-13 04:51:05.335390 pdm-2.7.4/README.md
--rw-r--r--   0        0        0     7986 2023-06-13 04:51:05.335390 pdm-2.7.4/README.md
--rw-r--r--   0        0        0     4396 2023-06-13 04:51:14.599513 pdm-2.7.4/pyproject.toml
--rw-r--r--   0        0        0       65 2023-06-13 04:51:05.339390 pdm-2.7.4/src/pdm/__main__.py
--rw-r--r--   0        0        0      316 2023-06-13 04:51:05.339390 pdm-2.7.4/src/pdm/__version__.py
--rw-r--r--   0        0        0     3282 2023-06-13 04:51:05.339390 pdm-2.7.4/src/pdm/_types.py
--rw-r--r--   0        0        0      237 2023-06-13 04:51:05.339390 pdm-2.7.4/src/pdm/builders/__init__.py
--rw-r--r--   0        0        0    11850 2023-06-13 04:51:05.339390 pdm-2.7.4/src/pdm/builders/base.py
--rw-r--r--   0        0        0     1755 2023-06-13 04:51:05.339390 pdm-2.7.4/src/pdm/builders/editable.py
--rw-r--r--   0        0        0      656 2023-06-13 04:51:05.339390 pdm-2.7.4/src/pdm/builders/sdist.py
--rw-r--r--   0        0        0     1073 2023-06-13 04:51:05.339390 pdm-2.7.4/src/pdm/builders/wheel.py
--rw-r--r--   0        0        0        0 2023-06-13 04:51:05.339390 pdm-2.7.4/src/pdm/cli/__init__.py
--rw-r--r--   0        0        0    14229 2023-06-13 04:51:05.339390 pdm-2.7.4/src/pdm/cli/actions.py
--rw-r--r--   0        0        0        0 2023-06-13 04:51:05.339390 pdm-2.7.4/src/pdm/cli/commands/__init__.py
--rw-r--r--   0        0        0     7095 2023-06-13 04:51:05.339390 pdm-2.7.4/src/pdm/cli/commands/add.py
--rw-r--r--   0        0        0     2857 2023-06-13 04:51:05.339390 pdm-2.7.4/src/pdm/cli/commands/base.py
--rw-r--r--   0        0        0     4236 2023-06-13 04:51:05.339390 pdm-2.7.4/src/pdm/cli/commands/build.py
--rw-r--r--   0        0        0     6542 2023-06-13 04:51:05.339390 pdm-2.7.4/src/pdm/cli/commands/cache.py
--rw-r--r--   0        0        0     1324 2023-06-13 04:51:05.339390 pdm-2.7.4/src/pdm/cli/commands/completion.py
--rw-r--r--   0        0        0     5812 2023-06-13 04:51:05.339390 pdm-2.7.4/src/pdm/cli/commands/config.py
--rw-r--r--   0        0        0     3066 2023-06-13 04:51:05.339390 pdm-2.7.4/src/pdm/cli/commands/export.py
--rw-r--r--   0        0        0     3136 2023-06-13 04:51:05.339390 pdm-2.7.4/src/pdm/cli/commands/fix/__init__.py
--rw-r--r--   0        0        0     2309 2023-06-13 04:51:05.339390 pdm-2.7.4/src/pdm/cli/commands/fix/fixers.py
--rw-r--r--   0        0        0     3689 2023-06-13 04:51:05.339390 pdm-2.7.4/src/pdm/cli/commands/import_cmd.py
--rw-r--r--   0        0        0     3032 2023-06-13 04:51:05.339390 pdm-2.7.4/src/pdm/cli/commands/info.py
--rw-r--r--   0        0        0     8612 2023-06-13 04:51:05.339390 pdm-2.7.4/src/pdm/cli/commands/init.py
--rw-r--r--   0        0        0     3589 2023-06-13 04:51:05.339390 pdm-2.7.4/src/pdm/cli/commands/install.py
--rw-r--r--   0        0        0    15754 2023-06-13 04:51:05.339390 pdm-2.7.4/src/pdm/cli/commands/list.py
--rw-r--r--   0        0        0     2196 2023-06-13 04:51:05.339390 pdm-2.7.4/src/pdm/cli/commands/lock.py
--rw-r--r--   0        0        0     6596 2023-06-13 04:51:05.339390 pdm-2.7.4/src/pdm/cli/commands/publish/__init__.py
--rw-r--r--   0        0        0     8165 2023-06-13 04:51:05.339390 pdm-2.7.4/src/pdm/cli/commands/publish/package.py
--rw-r--r--   0        0        0     6782 2023-06-13 04:51:05.339390 pdm-2.7.4/src/pdm/cli/commands/publish/repository.py
--rw-r--r--   0        0        0     4271 2023-06-13 04:51:05.339390 pdm-2.7.4/src/pdm/cli/commands/remove.py
--rw-r--r--   0        0        0    15427 2023-06-13 04:51:05.339390 pdm-2.7.4/src/pdm/cli/commands/run.py
--rw-r--r--   0        0        0     2436 2023-06-13 04:51:05.339390 pdm-2.7.4/src/pdm/cli/commands/search.py
--rw-r--r--   0        0        0     9373 2023-06-13 04:51:05.339390 pdm-2.7.4/src/pdm/cli/commands/self_cmd.py
--rw-r--r--   0        0        0     2896 2023-06-13 04:51:05.339390 pdm-2.7.4/src/pdm/cli/commands/show.py
--rw-r--r--   0        0        0     1447 2023-06-13 04:51:05.339390 pdm-2.7.4/src/pdm/cli/commands/sync.py
--rw-r--r--   0        0        0     6898 2023-06-13 04:51:05.339390 pdm-2.7.4/src/pdm/cli/commands/update.py
--rw-r--r--   0        0        0     6489 2023-06-13 04:51:05.339390 pdm-2.7.4/src/pdm/cli/commands/use.py
--rw-r--r--   0        0        0     1715 2023-06-13 04:51:05.339390 pdm-2.7.4/src/pdm/cli/commands/venv/__init__.py
--rw-r--r--   0        0        0     2426 2023-06-13 04:51:05.339390 pdm-2.7.4/src/pdm/cli/commands/venv/activate.py
--rw-r--r--   0        0        0     6149 2023-06-13 04:51:05.339390 pdm-2.7.4/src/pdm/cli/commands/venv/backends.py
--rw-r--r--   0        0        0     2155 2023-06-13 04:51:05.339390 pdm-2.7.4/src/pdm/cli/commands/venv/create.py
--rw-r--r--   0        0        0      819 2023-06-13 04:51:05.339390 pdm-2.7.4/src/pdm/cli/commands/venv/list.py
--rw-r--r--   0        0        0     2195 2023-06-13 04:51:05.339390 pdm-2.7.4/src/pdm/cli/commands/venv/purge.py
--rw-r--r--   0        0        0     1279 2023-06-13 04:51:05.339390 pdm-2.7.4/src/pdm/cli/commands/venv/remove.py
--rw-r--r--   0        0        0     2759 2023-06-13 04:51:05.339390 pdm-2.7.4/src/pdm/cli/commands/venv/utils.py
--rw-r--r--   0        0        0        0 2023-06-13 04:51:05.339390 pdm-2.7.4/src/pdm/cli/completions/__init__.py
--rw-r--r--   0        0        0     5096 2023-06-13 04:51:05.339390 pdm-2.7.4/src/pdm/cli/completions/pdm.bash
--rw-r--r--   0        0        0    38130 2023-06-13 04:51:05.339390 pdm-2.7.4/src/pdm/cli/completions/pdm.fish
--rw-r--r--   0        0        0    18583 2023-06-13 04:51:05.339390 pdm-2.7.4/src/pdm/cli/completions/pdm.ps1
--rw-r--r--   0        0        0    25158 2023-06-13 04:51:05.339390 pdm-2.7.4/src/pdm/cli/completions/pdm.zsh
--rw-r--r--   0        0        0     3840 2023-06-13 04:51:05.339390 pdm-2.7.4/src/pdm/cli/filters.py
--rw-r--r--   0        0        0     1481 2023-06-13 04:51:05.339390 pdm-2.7.4/src/pdm/cli/hooks.py
--rw-r--r--   0        0        0    10461 2023-06-13 04:51:05.339390 pdm-2.7.4/src/pdm/cli/options.py
--rw-r--r--   0        0        0    25081 2023-06-13 04:51:05.339390 pdm-2.7.4/src/pdm/cli/utils.py
--rw-r--r--   0        0        0     2226 2023-06-13 04:51:05.343390 pdm-2.7.4/src/pdm/compat.py
--rw-r--r--   0        0        0    10667 2023-06-13 04:51:05.343390 pdm-2.7.4/src/pdm/core.py
--rw-r--r--   0        0        0      825 2023-06-13 04:51:05.343390 pdm-2.7.4/src/pdm/environments/__init__.py
--rw-r--r--   0        0        0     8850 2023-06-13 04:51:05.343390 pdm-2.7.4/src/pdm/environments/base.py
--rw-r--r--   0        0        0     3560 2023-06-13 04:51:05.343390 pdm-2.7.4/src/pdm/environments/local.py
--rw-r--r--   0        0        0     1600 2023-06-13 04:51:05.343390 pdm-2.7.4/src/pdm/environments/python.py
--rw-r--r--   0        0        0     1362 2023-06-13 04:51:05.343390 pdm-2.7.4/src/pdm/exceptions.py
--rw-r--r--   0        0        0     1202 2023-06-13 04:51:05.343390 pdm-2.7.4/src/pdm/formats/__init__.py
--rw-r--r--   0        0        0     3215 2023-06-13 04:51:05.343390 pdm-2.7.4/src/pdm/formats/base.py
--rw-r--r--   0        0        0     5788 2023-06-13 04:51:05.343390 pdm-2.7.4/src/pdm/formats/flit.py
--rw-r--r--   0        0        0     2400 2023-06-13 04:51:05.343390 pdm-2.7.4/src/pdm/formats/pipfile.py
--rw-r--r--   0        0        0     7490 2023-06-13 04:51:05.343390 pdm-2.7.4/src/pdm/formats/poetry.py
--rw-r--r--   0        0        0     7502 2023-06-13 04:51:05.343390 pdm-2.7.4/src/pdm/formats/requirements.py
--rw-r--r--   0        0        0     2309 2023-06-13 04:51:05.343390 pdm-2.7.4/src/pdm/formats/setup_py.py
--rw-r--r--   0        0        0      119 2023-06-13 04:51:05.343390 pdm-2.7.4/src/pdm/installers/__init__.py
--rw-r--r--   0        0        0     1390 2023-06-13 04:51:05.343390 pdm-2.7.4/src/pdm/installers/core.py
--rw-r--r--   0        0        0    10901 2023-06-13 04:51:05.343390 pdm-2.7.4/src/pdm/installers/installers.py
--rw-r--r--   0        0        0     2091 2023-06-13 04:51:05.343390 pdm-2.7.4/src/pdm/installers/manager.py
--rw-r--r--   0        0        0     2226 2023-06-13 04:51:05.343390 pdm-2.7.4/src/pdm/installers/packages.py
--rw-r--r--   0        0        0    18161 2023-06-13 04:51:05.343390 pdm-2.7.4/src/pdm/installers/synchronizers.py
--rw-r--r--   0        0        0    10990 2023-06-13 04:51:05.343390 pdm-2.7.4/src/pdm/installers/uninstallers.py
--rw-r--r--   0        0        0        0 2023-06-13 04:51:05.343390 pdm-2.7.4/src/pdm/models/__init__.py
--rw-r--r--   0        0        0     3162 2023-06-13 04:51:05.343390 pdm-2.7.4/src/pdm/models/auth.py
--rw-r--r--   0        0        0     4698 2023-06-13 04:51:05.343390 pdm-2.7.4/src/pdm/models/backends.py
--rw-r--r--   0        0        0    11466 2023-06-13 04:51:05.343390 pdm-2.7.4/src/pdm/models/caches.py
--rw-r--r--   0        0        0    26568 2023-06-13 04:51:05.343390 pdm-2.7.4/src/pdm/models/candidates.py
--rw-r--r--   0        0        0      287 2023-06-13 04:51:05.343390 pdm-2.7.4/src/pdm/models/environment.py
--rw-r--r--   0        0        0     1845 2023-06-13 04:51:05.343390 pdm-2.7.4/src/pdm/models/in_process/__init__.py
--rw-r--r--   0        0        0     2049 2023-06-13 04:51:05.343390 pdm-2.7.4/src/pdm/models/in_process/get_abi_tag.py
--rw-r--r--   0        0        0     6323 2023-06-13 04:51:05.343390 pdm-2.7.4/src/pdm/models/in_process/parse_setup.py
--rw-r--r--   0        0        0     1165 2023-06-13 04:51:05.343390 pdm-2.7.4/src/pdm/models/in_process/pep508.py
--rw-r--r--   0        0        0     1653 2023-06-13 04:51:05.343390 pdm-2.7.4/src/pdm/models/in_process/sysconfig_get_paths.py
--rw-r--r--   0        0        0     5701 2023-06-13 04:51:05.343390 pdm-2.7.4/src/pdm/models/markers.py
--rw-r--r--   0        0        0     3507 2023-06-13 04:51:05.343390 pdm-2.7.4/src/pdm/models/project_info.py
--rw-r--r--   0        0        0     2195 2023-06-13 04:51:05.343390 pdm-2.7.4/src/pdm/models/python.py
--rw-r--r--   0        0        0      318 2023-06-13 04:51:05.343390 pdm-2.7.4/src/pdm/models/python_max_versions.json
--rw-r--r--   0        0        0    21340 2023-06-13 04:51:05.343390 pdm-2.7.4/src/pdm/models/repositories.py
--rw-r--r--   0        0        0    18726 2023-06-13 04:51:05.343390 pdm-2.7.4/src/pdm/models/requirements.py
--rw-r--r--   0        0        0     2313 2023-06-13 04:51:05.343390 pdm-2.7.4/src/pdm/models/search.py
--rw-r--r--   0        0        0     2426 2023-06-13 04:51:05.343390 pdm-2.7.4/src/pdm/models/session.py
--rw-r--r--   0        0        0    14482 2023-06-13 04:51:05.343390 pdm-2.7.4/src/pdm/models/setup.py
--rw-r--r--   0        0        0    16337 2023-06-13 04:51:05.343390 pdm-2.7.4/src/pdm/models/specifiers.py
--rw-r--r--   0        0        0     1300 2023-06-13 04:51:05.343390 pdm-2.7.4/src/pdm/models/venv.py
--rw-r--r--   0        0        0     5924 2023-06-13 04:51:05.343390 pdm-2.7.4/src/pdm/models/versions.py
--rw-r--r--   0        0        0     2766 2023-06-13 04:51:05.343390 pdm-2.7.4/src/pdm/models/working_set.py
--rw-r--r--   0        0        0        0 2023-06-13 04:51:05.343390 pdm-2.7.4/src/pdm/pep582/__init__.py
--rw-r--r--   0        0        0     4481 2023-06-13 04:51:05.343390 pdm-2.7.4/src/pdm/pep582/sitecustomize.py
--rw-r--r--   0        0        0      134 2023-06-13 04:51:05.343390 pdm-2.7.4/src/pdm/project/__init__.py
--rw-r--r--   0        0        0    16748 2023-06-13 04:51:05.343390 pdm-2.7.4/src/pdm/project/config.py
--rw-r--r--   0        0        0    26273 2023-06-13 04:51:05.343390 pdm-2.7.4/src/pdm/project/core.py
--rw-r--r--   0        0        0     2093 2023-06-13 04:51:05.343390 pdm-2.7.4/src/pdm/project/lockfile.py
--rw-r--r--   0        0        0     3385 2023-06-13 04:51:05.343390 pdm-2.7.4/src/pdm/project/project_file.py
--rw-r--r--   0        0        0     1070 2023-06-13 04:51:05.343390 pdm-2.7.4/src/pdm/project/toml_file.py
--rw-r--r--   0        0        0        0 2023-06-13 04:51:05.343390 pdm-2.7.4/src/pdm/py.typed
--rw-r--r--   0        0        0    19876 2023-06-13 04:51:05.343390 pdm-2.7.4/src/pdm/pytest.py
--rw-r--r--   0        0        0       61 2023-06-13 04:51:05.343390 pdm-2.7.4/src/pdm/resolver/__init__.py
--rw-r--r--   0        0        0     1954 2023-06-13 04:51:05.343390 pdm-2.7.4/src/pdm/resolver/core.py
--rw-r--r--   0        0        0    13119 2023-06-13 04:51:05.343390 pdm-2.7.4/src/pdm/resolver/providers.py
--rw-r--r--   0        0        0     1580 2023-06-13 04:51:05.343390 pdm-2.7.4/src/pdm/resolver/python.py
--rw-r--r--   0        0        0     3742 2023-06-13 04:51:05.347390 pdm-2.7.4/src/pdm/resolver/reporters.py
--rw-r--r--   0        0        0     4027 2023-06-13 04:51:05.347390 pdm-2.7.4/src/pdm/signals.py
--rw-r--r--   0        0        0     8054 2023-06-13 04:51:05.347390 pdm-2.7.4/src/pdm/termui.py
--rw-r--r--   0        0        0    13866 2023-06-13 04:51:05.347390 pdm-2.7.4/src/pdm/utils.py
--rw-r--r--   0        0        0       72 2023-06-13 04:51:05.347390 pdm-2.7.4/tests/__init__.py
--rw-r--r--   0        0        0        0 2023-06-13 04:51:05.347390 pdm-2.7.4/tests/cli/__init__.py
--rw-r--r--   0        0        0     3723 2023-06-13 04:51:05.347390 pdm-2.7.4/tests/cli/conftest.py
--rw-r--r--   0        0        0    12362 2023-06-13 04:51:05.347390 pdm-2.7.4/tests/cli/test_add.py
--rw-r--r--   0        0        0     5799 2023-06-13 04:51:05.347390 pdm-2.7.4/tests/cli/test_build.py
--rw-r--r--   0        0        0     5229 2023-06-13 04:51:05.347390 pdm-2.7.4/tests/cli/test_cache.py
--rw-r--r--   0        0        0     9286 2023-06-13 04:51:05.347390 pdm-2.7.4/tests/cli/test_config.py
--rw-r--r--   0        0        0     2029 2023-06-13 04:51:05.347390 pdm-2.7.4/tests/cli/test_fix.py
--rw-r--r--   0        0        0    10375 2023-06-13 04:51:05.347390 pdm-2.7.4/tests/cli/test_hooks.py
--rw-r--r--   0        0        0     4481 2023-06-13 04:51:05.347390 pdm-2.7.4/tests/cli/test_init.py
--rw-r--r--   0        0        0    11265 2023-06-13 04:51:05.347390 pdm-2.7.4/tests/cli/test_install.py
--rw-r--r--   0        0        0    28998 2023-06-13 04:51:05.347390 pdm-2.7.4/tests/cli/test_list.py
--rw-r--r--   0        0        0     6324 2023-06-13 04:51:05.347390 pdm-2.7.4/tests/cli/test_lock.py
--rw-r--r--   0        0        0     7796 2023-06-13 04:51:05.347390 pdm-2.7.4/tests/cli/test_others.py
--rw-r--r--   0        0        0     6052 2023-06-13 04:51:05.347390 pdm-2.7.4/tests/cli/test_publish.py
--rw-r--r--   0        0        0     3888 2023-06-13 04:51:05.347390 pdm-2.7.4/tests/cli/test_remove.py
--rw-r--r--   0        0        0    29259 2023-06-13 04:51:05.347390 pdm-2.7.4/tests/cli/test_run.py
--rw-r--r--   0        0        0     3599 2023-06-13 04:51:05.347390 pdm-2.7.4/tests/cli/test_self_command.py
--rw-r--r--   0        0        0     8876 2023-06-13 04:51:05.347390 pdm-2.7.4/tests/cli/test_update.py
--rw-r--r--   0        0        0     2997 2023-06-13 04:51:05.347390 pdm-2.7.4/tests/cli/test_use.py
--rw-r--r--   0        0        0    10430 2023-06-13 04:51:05.347390 pdm-2.7.4/tests/cli/test_venv.py
--rw-r--r--   0        0        0     3079 2023-06-13 04:51:05.347390 pdm-2.7.4/tests/conftest.py
--rw-r--r--   0        0        0      235 2023-06-13 04:51:05.347390 pdm-2.7.4/tests/fixtures/Pipfile
--rw-r--r--   0        0        0        0 2023-06-13 04:51:05.347390 pdm-2.7.4/tests/fixtures/__init__.py
--rw-r--r--   0        0        0    49497 2023-06-13 04:51:05.347390 pdm-2.7.4/tests/fixtures/artifacts/PyFunctional-1.4.3-py3-none-any.whl
--rw-r--r--   0        0        0      546 2023-06-13 04:51:05.347390 pdm-2.7.4/tests/fixtures/artifacts/caj2pdf-restructured-0.1.0a6.tar.gz
--rw-r--r--   0        0        0   422824 2023-06-13 04:51:05.351390 pdm-2.7.4/tests/fixtures/artifacts/celery-4.4.2-py2.py3-none-any.whl
--rw-r--r--   0        0        0     1254 2023-06-13 04:51:05.351390 pdm-2.7.4/tests/fixtures/artifacts/demo-0.0.1-cp36-cp36m-win_amd64.whl
--rw-r--r--   0        0        0     1254 2023-06-13 04:51:05.351390 pdm-2.7.4/tests/fixtures/artifacts/demo-0.0.1-py2.py3-none-any.whl
--rw-r--r--   0        0        0     1038 2023-06-13 04:51:05.351390 pdm-2.7.4/tests/fixtures/artifacts/demo-0.0.1.tar.gz
--rw-r--r--   0        0        0     2615 2023-06-13 04:51:05.351390 pdm-2.7.4/tests/fixtures/artifacts/demo-0.0.1.zip
--rw-r--r--   0        0        0     4595 2023-06-13 04:51:05.351390 pdm-2.7.4/tests/fixtures/artifacts/editables-0.2-py3-none-any.whl
--rw-r--r--   0        0        0     5359 2023-06-13 04:51:05.351390 pdm-2.7.4/tests/fixtures/artifacts/first-2.0.2-py2.py3-none-any.whl
--rw-r--r--   0        0        0    56715 2023-06-13 04:51:05.351390 pdm-2.7.4/tests/fixtures/artifacts/flit_core-3.6.0-py3-none-any.whl
--rw-r--r--   0        0        0     6138 2023-06-13 04:51:05.351390 pdm-2.7.4/tests/fixtures/artifacts/future_fstrings-1.2.0-py2.py3-none-any.whl
--rw-r--r--   0        0        0     5786 2023-06-13 04:51:05.351390 pdm-2.7.4/tests/fixtures/artifacts/future_fstrings-1.2.0.tar.gz
--rw-r--r--   0        0        0    17978 2023-06-13 04:51:05.351390 pdm-2.7.4/tests/fixtures/artifacts/importlib_metadata-4.8.3-py3-none-any.whl
--rw-r--r--   0        0        0    24489 2023-06-13 04:51:05.351390 pdm-2.7.4/tests/fixtures/artifacts/jmespath-0.10.0-py2.py3-none-any.whl
--rw-r--r--   0        0        0   156727 2023-06-13 04:51:05.351390 pdm-2.7.4/tests/fixtures/artifacts/pdm_backend-2.0.2-py3-none-any.whl
--rw-r--r--   0        0        0     1401 2023-06-13 04:51:05.351390 pdm-2.7.4/tests/fixtures/artifacts/pdm_hello-0.1.0-py3-none-any.whl
--rw-r--r--   0        0        0     1405 2023-06-13 04:51:05.351390 pdm-2.7.4/tests/fixtures/artifacts/pdm_hello-0.1.0-py3-none-win_amd64.whl
--rw-r--r--   0        0        0   305481 2023-06-13 04:51:05.355390 pdm-2.7.4/tests/fixtures/artifacts/pdm_pep517-1.0.0-py3-none-any.whl
--rw-r--r--   0        0        0   531270 2023-06-13 04:51:05.359390 pdm-2.7.4/tests/fixtures/artifacts/poetry_core-1.3.2-py3-none-any.whl
--rw-r--r--   0        0        0  1232518 2023-06-13 04:51:05.363391 pdm-2.7.4/tests/fixtures/artifacts/setuptools-65.4.1-py3-none-any.whl
--rw-r--r--   0        0        0    26662 2023-06-13 04:51:05.363391 pdm-2.7.4/tests/fixtures/artifacts/typing_extensions-4.4.0-py3-none-any.whl
--rw-r--r--   0        0        0    35301 2023-06-13 04:51:05.363391 pdm-2.7.4/tests/fixtures/artifacts/wheel-0.37.1-py2.py3-none-any.whl
--rw-r--r--   0        0        0     5312 2023-06-13 04:51:05.363391 pdm-2.7.4/tests/fixtures/artifacts/zipp-3.7.0-py3-none-any.whl
--rw-r--r--   0        0        0      326 2023-06-13 04:51:05.363391 pdm-2.7.4/tests/fixtures/index/demo.html
--rw-r--r--   0        0        0      511 2023-06-13 04:51:05.363391 pdm-2.7.4/tests/fixtures/index/future-fstrings.html
--rw-r--r--   0        0        0      262 2023-06-13 04:51:05.363391 pdm-2.7.4/tests/fixtures/index/pep345-legacy.html
--rw-r--r--   0        0        0      262 2023-06-13 04:51:05.363391 pdm-2.7.4/tests/fixtures/index/wheel.html
--rw-r--r--   0        0        0        0 2023-06-13 04:51:05.363391 pdm-2.7.4/tests/fixtures/projects/__init__.py
--rw-r--r--   0        0        0       42 2023-06-13 04:51:05.363391 pdm-2.7.4/tests/fixtures/projects/demo-#-with-hash/demo.py
--rw-r--r--   0        0        0      332 2023-06-13 04:51:05.363391 pdm-2.7.4/tests/fixtures/projects/demo-#-with-hash/setup.py
--rw-r--r--   0        0        0       26 2023-06-13 04:51:05.363391 pdm-2.7.4/tests/fixtures/projects/demo-combined-extras/demo.py
--rw-r--r--   0        0        0      462 2023-06-13 04:51:05.363391 pdm-2.7.4/tests/fixtures/projects/demo-combined-extras/pyproject.toml
--rw-r--r--   0        0        0       42 2023-06-13 04:51:05.363391 pdm-2.7.4/tests/fixtures/projects/demo-failure-no-dep/demo.py
--rw-r--r--   0        0        0      246 2023-06-13 04:51:05.363391 pdm-2.7.4/tests/fixtures/projects/demo-failure-no-dep/setup.py
--rw-r--r--   0        0        0       42 2023-06-13 04:51:05.363391 pdm-2.7.4/tests/fixtures/projects/demo-failure/demo.py
--rw-r--r--   0        0        0      345 2023-06-13 04:51:05.363391 pdm-2.7.4/tests/fixtures/projects/demo-failure/setup.py
--rw-r--r--   0        0        0       12 2023-06-13 04:51:05.363391 pdm-2.7.4/tests/fixtures/projects/demo-module/LICENSE
--rw-r--r--   0        0        0       24 2023-06-13 04:51:05.363391 pdm-2.7.4/tests/fixtures/projects/demo-module/README.md
--rw-r--r--   0        0        0       14 2023-06-13 04:51:05.363391 pdm-2.7.4/tests/fixtures/projects/demo-module/bar_module.py
--rw-r--r--   0        0        0       36 2023-06-13 04:51:05.363391 pdm-2.7.4/tests/fixtures/projects/demo-module/foo_module.py
--rw-r--r--   0        0        0      442 2023-06-13 04:51:05.363391 pdm-2.7.4/tests/fixtures/projects/demo-module/pyproject.toml
--rw-r--r--   0        0        0     3983 2023-06-13 04:51:05.363391 pdm-2.7.4/tests/fixtures/projects/demo-package-has-dep-with-extras/pdm.lock
--rw-r--r--   0        0        0      318 2023-06-13 04:51:05.363391 pdm-2.7.4/tests/fixtures/projects/demo-package-has-dep-with-extras/pyproject.toml
--rw-r--r--   0        0        0      157 2023-06-13 04:51:05.363391 pdm-2.7.4/tests/fixtures/projects/demo-package-has-dep-with-extras/requirements.txt
--rw-r--r--   0        0        0       12 2023-06-13 04:51:05.363391 pdm-2.7.4/tests/fixtures/projects/demo-package/LICENSE
--rw-r--r--   0        0        0       24 2023-06-13 04:51:05.363391 pdm-2.7.4/tests/fixtures/projects/demo-package/README.md
--rw-r--r--   0        0        0       16 2023-06-13 04:51:05.363391 pdm-2.7.4/tests/fixtures/projects/demo-package/data_out.json
--rw-r--r--   0        0        0       22 2023-06-13 04:51:05.367390 pdm-2.7.4/tests/fixtures/projects/demo-package/my_package/__init__.py
--rw-r--r--   0        0        0       24 2023-06-13 04:51:05.367390 pdm-2.7.4/tests/fixtures/projects/demo-package/my_package/data.json
--rw-r--r--   0        0        0    29800 2023-06-13 04:51:05.367390 pdm-2.7.4/tests/fixtures/projects/demo-package/pdm.lock
--rw-r--r--   0        0        0      574 2023-06-13 04:51:05.367390 pdm-2.7.4/tests/fixtures/projects/demo-package/pyproject.toml
--rw-r--r--   0        0        0      122 2023-06-13 04:51:05.367390 pdm-2.7.4/tests/fixtures/projects/demo-package/requirements.ini
--rw-r--r--   0        0        0     7521 2023-06-13 04:51:05.367390 pdm-2.7.4/tests/fixtures/projects/demo-package/requirements.txt
--rw-r--r--   0        0        0      211 2023-06-13 04:51:05.367390 pdm-2.7.4/tests/fixtures/projects/demo-package/requirements_simple.txt
--rw-r--r--   0        0        0      728 2023-06-13 04:51:05.367390 pdm-2.7.4/tests/fixtures/projects/demo-package/setup.txt
--rw-r--r--   0        0        0       21 2023-06-13 04:51:05.367390 pdm-2.7.4/tests/fixtures/projects/demo-package/single_module.py
--rw-r--r--   0        0        0       18 2023-06-13 04:51:05.367390 pdm-2.7.4/tests/fixtures/projects/demo-parent-package/README.md
--rw-r--r--   0        0        0       22 2023-06-13 04:51:05.367390 pdm-2.7.4/tests/fixtures/projects/demo-parent-package/package-a/foo.py
--rw-r--r--   0        0        0      120 2023-06-13 04:51:05.367390 pdm-2.7.4/tests/fixtures/projects/demo-parent-package/package-a/setup.py
--rw-r--r--   0        0        0       22 2023-06-13 04:51:05.367390 pdm-2.7.4/tests/fixtures/projects/demo-parent-package/package-b/bar.py
--rw-r--r--   0        0        0      197 2023-06-13 04:51:05.367390 pdm-2.7.4/tests/fixtures/projects/demo-parent-package/package-b/pyproject.toml
--rw-r--r--   0        0        0       42 2023-06-13 04:51:05.367390 pdm-2.7.4/tests/fixtures/projects/demo-prerelease/demo.py
--rw-r--r--   0        0        0      334 2023-06-13 04:51:05.367390 pdm-2.7.4/tests/fixtures/projects/demo-prerelease/setup.py
--rw-r--r--   0        0        0       12 2023-06-13 04:51:05.367390 pdm-2.7.4/tests/fixtures/projects/demo-src-package/LICENSE
--rw-r--r--   0        0        0       24 2023-06-13 04:51:05.367390 pdm-2.7.4/tests/fixtures/projects/demo-src-package/README.md
--rw-r--r--   0        0        0       16 2023-06-13 04:51:05.367390 pdm-2.7.4/tests/fixtures/projects/demo-src-package/data_out.json
--rw-r--r--   0        0        0      456 2023-06-13 04:51:05.367390 pdm-2.7.4/tests/fixtures/projects/demo-src-package/pyproject.toml
--rw-r--r--   0        0        0       21 2023-06-13 04:51:05.367390 pdm-2.7.4/tests/fixtures/projects/demo-src-package/single_module.py
--rw-r--r--   0        0        0       22 2023-06-13 04:51:05.367390 pdm-2.7.4/tests/fixtures/projects/demo-src-package/src/my_package/__init__.py
--rw-r--r--   0        0        0       24 2023-06-13 04:51:05.367390 pdm-2.7.4/tests/fixtures/projects/demo-src-package/src/my_package/data.json
--rw-r--r--   0        0        0       42 2023-06-13 04:51:05.367390 pdm-2.7.4/tests/fixtures/projects/demo/demo.py
--rw-r--r--   0        0        0      332 2023-06-13 04:51:05.367390 pdm-2.7.4/tests/fixtures/projects/demo/setup.py
--rw-r--r--   0        0        0       26 2023-06-13 04:51:05.367390 pdm-2.7.4/tests/fixtures/projects/demo_extras/demo.py
--rw-r--r--   0        0        0      250 2023-06-13 04:51:05.367390 pdm-2.7.4/tests/fixtures/projects/demo_extras/setup.py
--rw-r--r--   0        0        0        0 2023-06-13 04:51:05.367390 pdm-2.7.4/tests/fixtures/projects/flit-demo/README.rst
--rw-r--r--   0        0        0        0 2023-06-13 04:51:05.367390 pdm-2.7.4/tests/fixtures/projects/flit-demo/doc/index.html
--rw-r--r--   0        0        0       49 2023-06-13 04:51:05.367390 pdm-2.7.4/tests/fixtures/projects/flit-demo/flit.py
--rw-r--r--   0        0        0      969 2023-06-13 04:51:05.367390 pdm-2.7.4/tests/fixtures/projects/flit-demo/pyproject.toml
--rw-r--r--   0        0        0       12 2023-06-13 04:51:05.367390 pdm-2.7.4/tests/fixtures/projects/poetry-demo/mylib.py
--rw-r--r--   0        0        0      863 2023-06-13 04:51:05.367390 pdm-2.7.4/tests/fixtures/projects/poetry-demo/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-13 04:51:05.367390 pdm-2.7.4/tests/fixtures/projects/test-hatch-static/README.md
--rw-r--r--   0        0        0      386 2023-06-13 04:51:05.367390 pdm-2.7.4/tests/fixtures/projects/test-hatch-static/pyproject.toml
--rw-r--r--   0        0        0       11 2023-06-13 04:51:05.367390 pdm-2.7.4/tests/fixtures/projects/test-monorepo/README.md
--rw-r--r--   0        0        0        0 2023-06-13 04:51:05.367390 pdm-2.7.4/tests/fixtures/projects/test-monorepo/core/core.py
--rw-r--r--   0        0        0      179 2023-06-13 04:51:05.367390 pdm-2.7.4/tests/fixtures/projects/test-monorepo/core/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-13 04:51:05.367390 pdm-2.7.4/tests/fixtures/projects/test-monorepo/package_a/alice.py
--rw-r--r--   0        0        0      231 2023-06-13 04:51:05.367390 pdm-2.7.4/tests/fixtures/projects/test-monorepo/package_a/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-13 04:51:05.367390 pdm-2.7.4/tests/fixtures/projects/test-monorepo/package_b/bob.py
--rw-r--r--   0        0        0      231 2023-06-13 04:51:05.367390 pdm-2.7.4/tests/fixtures/projects/test-monorepo/package_b/pyproject.toml
--rw-r--r--   0        0        0      237 2023-06-13 04:51:05.367390 pdm-2.7.4/tests/fixtures/projects/test-monorepo/pyproject.toml
--rw-r--r--   0        0        0      380 2023-06-13 04:51:05.367390 pdm-2.7.4/tests/fixtures/projects/test-plugin-pdm/hello.py
--rw-r--r--   0        0        0      312 2023-06-13 04:51:05.367390 pdm-2.7.4/tests/fixtures/projects/test-plugin-pdm/pyproject.toml
--rw-r--r--   0        0        0      380 2023-06-13 04:51:05.367390 pdm-2.7.4/tests/fixtures/projects/test-plugin/hello.py
--rw-r--r--   0        0        0      168 2023-06-13 04:51:05.367390 pdm-2.7.4/tests/fixtures/projects/test-plugin/setup.py
--rw-r--r--   0        0        0        0 2023-06-13 04:51:05.367390 pdm-2.7.4/tests/fixtures/projects/test-removal/__init__.py
--rw-r--r--   0        0        0        0 2023-06-13 04:51:05.367390 pdm-2.7.4/tests/fixtures/projects/test-removal/bar.py
--rw-r--r--   0        0        0        0 2023-06-13 04:51:05.367390 pdm-2.7.4/tests/fixtures/projects/test-removal/foo.py
--rw-r--r--   0        0        0        0 2023-06-13 04:51:05.367390 pdm-2.7.4/tests/fixtures/projects/test-removal/subdir/__init__.py
--rw-r--r--   0        0        0       10 2023-06-13 04:51:05.367390 pdm-2.7.4/tests/fixtures/projects/test-setuptools/AUTHORS
--rw-r--r--   0        0        0       12 2023-06-13 04:51:05.367390 pdm-2.7.4/tests/fixtures/projects/test-setuptools/README.md
--rw-r--r--   0        0        0       22 2023-06-13 04:51:05.367390 pdm-2.7.4/tests/fixtures/projects/test-setuptools/mymodule.py
--rw-r--r--   0        0        0      398 2023-06-13 04:51:05.367390 pdm-2.7.4/tests/fixtures/projects/test-setuptools/setup.cfg
--rw-r--r--   0        0        0      308 2023-06-13 04:51:05.367390 pdm-2.7.4/tests/fixtures/projects/test-setuptools/setup.py
--rw-r--r--   0        0        0     1525 2023-06-13 04:51:05.367390 pdm-2.7.4/tests/fixtures/pypi.json
--rw-r--r--   0        0        0     1330 2023-06-13 04:51:05.367390 pdm-2.7.4/tests/fixtures/pyproject.toml
--rw-r--r--   0        0        0       20 2023-06-13 04:51:05.367390 pdm-2.7.4/tests/fixtures/requirements-include.txt
--rw-r--r--   0        0        0      502 2023-06-13 04:51:05.367390 pdm-2.7.4/tests/fixtures/requirements.txt
--rw-r--r--   0        0        0        0 2023-06-13 04:51:05.367390 pdm-2.7.4/tests/models/__init__.py
--rw-r--r--   0        0        0     3814 2023-06-13 04:51:05.367390 pdm-2.7.4/tests/models/test_backends.py
--rw-r--r--   0        0        0    13344 2023-06-13 04:51:05.367390 pdm-2.7.4/tests/models/test_candidates.py
--rw-r--r--   0        0        0     1971 2023-06-13 04:51:05.367390 pdm-2.7.4/tests/models/test_marker.py
--rw-r--r--   0        0        0     2679 2023-06-13 04:51:05.367390 pdm-2.7.4/tests/models/test_requirements.py
--rw-r--r--   0        0        0     2556 2023-06-13 04:51:05.367390 pdm-2.7.4/tests/models/test_setup_parsing.py
--rw-r--r--   0        0        0     3418 2023-06-13 04:51:05.367390 pdm-2.7.4/tests/models/test_specifiers.py
--rw-r--r--   0        0        0     2703 2023-06-13 04:51:05.367390 pdm-2.7.4/tests/models/test_versions.py
--rw-r--r--   0        0        0        0 2023-06-13 04:51:05.367390 pdm-2.7.4/tests/resolver/__init__.py
--rw-r--r--   0        0        0    11567 2023-06-13 04:51:05.367390 pdm-2.7.4/tests/resolver/test_resolve.py
--rw-r--r--   0        0        0     7704 2023-06-13 04:51:05.367390 pdm-2.7.4/tests/test_formats.py
--rw-r--r--   0        0        0     7231 2023-06-13 04:51:05.367390 pdm-2.7.4/tests/test_installer.py
--rw-r--r--   0        0        0     1829 2023-06-13 04:51:05.367390 pdm-2.7.4/tests/test_integration.py
--rw-r--r--   0        0        0     3435 2023-06-13 04:51:05.367390 pdm-2.7.4/tests/test_plugin.py
--rw-r--r--   0        0        0    12085 2023-06-13 04:51:05.367390 pdm-2.7.4/tests/test_project.py
--rw-r--r--   0        0        0     1103 2023-06-13 04:51:05.367390 pdm-2.7.4/tests/test_signals.py
--rw-r--r--   0        0        0     4419 2023-06-13 04:51:05.367390 pdm-2.7.4/tests/test_utils.py
--rw-r--r--   0        0        0     9611 1970-01-01 00:00:00.000000 pdm-2.7.4/PKG-INFO
+-rw-r--r--   0        0        0   125971 2023-06-27 02:38:06.416159 pdm-2.8.0a0/CHANGELOG.md
+-rw-r--r--   0        0        0     1075 2023-06-27 02:38:06.416159 pdm-2.8.0a0/LICENSE
+-rw-r--r--   0        0        0     1075 2023-06-27 02:38:06.416159 pdm-2.8.0a0/LICENSE
+-rw-r--r--   0        0        0     7937 2023-06-27 02:38:06.416159 pdm-2.8.0a0/README.md
+-rw-r--r--   0        0        0     7937 2023-06-27 02:38:06.416159 pdm-2.8.0a0/README.md
+-rw-r--r--   0        0        0     4454 2023-06-27 02:38:15.224328 pdm-2.8.0a0/pyproject.toml
+-rw-r--r--   0        0        0       65 2023-06-27 02:38:06.420159 pdm-2.8.0a0/src/pdm/__main__.py
+-rw-r--r--   0        0        0      316 2023-06-27 02:38:06.420159 pdm-2.8.0a0/src/pdm/__version__.py
+-rw-r--r--   0        0        0     3282 2023-06-27 02:38:06.420159 pdm-2.8.0a0/src/pdm/_types.py
+-rw-r--r--   0        0        0      237 2023-06-27 02:38:06.420159 pdm-2.8.0a0/src/pdm/builders/__init__.py
+-rw-r--r--   0        0        0    11850 2023-06-27 02:38:06.420159 pdm-2.8.0a0/src/pdm/builders/base.py
+-rw-r--r--   0        0        0     1755 2023-06-27 02:38:06.420159 pdm-2.8.0a0/src/pdm/builders/editable.py
+-rw-r--r--   0        0        0      656 2023-06-27 02:38:06.420159 pdm-2.8.0a0/src/pdm/builders/sdist.py
+-rw-r--r--   0        0        0     1073 2023-06-27 02:38:06.420159 pdm-2.8.0a0/src/pdm/builders/wheel.py
+-rw-r--r--   0        0        0        0 2023-06-27 02:38:06.420159 pdm-2.8.0a0/src/pdm/cli/__init__.py
+-rw-r--r--   0        0        0    16131 2023-06-27 02:38:06.420159 pdm-2.8.0a0/src/pdm/cli/actions.py
+-rw-r--r--   0        0        0        0 2023-06-27 02:38:06.420159 pdm-2.8.0a0/src/pdm/cli/commands/__init__.py
+-rw-r--r--   0        0        0     7104 2023-06-27 02:38:06.420159 pdm-2.8.0a0/src/pdm/cli/commands/add.py
+-rw-r--r--   0        0        0     2857 2023-06-27 02:38:06.420159 pdm-2.8.0a0/src/pdm/cli/commands/base.py
+-rw-r--r--   0        0        0     4236 2023-06-27 02:38:06.424159 pdm-2.8.0a0/src/pdm/cli/commands/build.py
+-rw-r--r--   0        0        0     6542 2023-06-27 02:38:06.424159 pdm-2.8.0a0/src/pdm/cli/commands/cache.py
+-rw-r--r--   0        0        0     1324 2023-06-27 02:38:06.424159 pdm-2.8.0a0/src/pdm/cli/commands/completion.py
+-rw-r--r--   0        0        0     7165 2023-06-27 02:38:06.424159 pdm-2.8.0a0/src/pdm/cli/commands/config.py
+-rw-r--r--   0        0        0     3066 2023-06-27 02:38:06.424159 pdm-2.8.0a0/src/pdm/cli/commands/export.py
+-rw-r--r--   0        0        0     3136 2023-06-27 02:38:06.424159 pdm-2.8.0a0/src/pdm/cli/commands/fix/__init__.py
+-rw-r--r--   0        0        0     2309 2023-06-27 02:38:06.424159 pdm-2.8.0a0/src/pdm/cli/commands/fix/fixers.py
+-rw-r--r--   0        0        0     3689 2023-06-27 02:38:06.424159 pdm-2.8.0a0/src/pdm/cli/commands/import_cmd.py
+-rw-r--r--   0        0        0     3032 2023-06-27 02:38:06.424159 pdm-2.8.0a0/src/pdm/cli/commands/info.py
+-rw-r--r--   0        0        0     7605 2023-06-27 02:38:06.424159 pdm-2.8.0a0/src/pdm/cli/commands/init.py
+-rw-r--r--   0        0        0     3589 2023-06-27 02:38:06.424159 pdm-2.8.0a0/src/pdm/cli/commands/install.py
+-rw-r--r--   0        0        0    15754 2023-06-27 02:38:06.424159 pdm-2.8.0a0/src/pdm/cli/commands/list.py
+-rw-r--r--   0        0        0     2196 2023-06-27 02:38:06.424159 pdm-2.8.0a0/src/pdm/cli/commands/lock.py
+-rw-r--r--   0        0        0     6596 2023-06-27 02:38:06.424159 pdm-2.8.0a0/src/pdm/cli/commands/publish/__init__.py
+-rw-r--r--   0        0        0     8112 2023-06-27 02:38:06.424159 pdm-2.8.0a0/src/pdm/cli/commands/publish/package.py
+-rw-r--r--   0        0        0     6782 2023-06-27 02:38:06.424159 pdm-2.8.0a0/src/pdm/cli/commands/publish/repository.py
+-rw-r--r--   0        0        0     4271 2023-06-27 02:38:06.424159 pdm-2.8.0a0/src/pdm/cli/commands/remove.py
+-rw-r--r--   0        0        0    15489 2023-06-27 02:38:06.424159 pdm-2.8.0a0/src/pdm/cli/commands/run.py
+-rw-r--r--   0        0        0     2436 2023-06-27 02:38:06.424159 pdm-2.8.0a0/src/pdm/cli/commands/search.py
+-rw-r--r--   0        0        0     9370 2023-06-27 02:38:06.424159 pdm-2.8.0a0/src/pdm/cli/commands/self_cmd.py
+-rw-r--r--   0        0        0     2896 2023-06-27 02:38:06.424159 pdm-2.8.0a0/src/pdm/cli/commands/show.py
+-rw-r--r--   0        0        0     1447 2023-06-27 02:38:06.424159 pdm-2.8.0a0/src/pdm/cli/commands/sync.py
+-rw-r--r--   0        0        0     6898 2023-06-27 02:38:06.424159 pdm-2.8.0a0/src/pdm/cli/commands/update.py
+-rw-r--r--   0        0        0     6489 2023-06-27 02:38:06.424159 pdm-2.8.0a0/src/pdm/cli/commands/use.py
+-rw-r--r--   0        0        0     1723 2023-06-27 02:38:06.424159 pdm-2.8.0a0/src/pdm/cli/commands/venv/__init__.py
+-rw-r--r--   0        0        0     2426 2023-06-27 02:38:06.424159 pdm-2.8.0a0/src/pdm/cli/commands/venv/activate.py
+-rw-r--r--   0        0        0     6149 2023-06-27 02:38:06.424159 pdm-2.8.0a0/src/pdm/cli/commands/venv/backends.py
+-rw-r--r--   0        0        0     2155 2023-06-27 02:38:06.424159 pdm-2.8.0a0/src/pdm/cli/commands/venv/create.py
+-rw-r--r--   0        0        0      819 2023-06-27 02:38:06.424159 pdm-2.8.0a0/src/pdm/cli/commands/venv/list.py
+-rw-r--r--   0        0        0     2195 2023-06-27 02:38:06.424159 pdm-2.8.0a0/src/pdm/cli/commands/venv/purge.py
+-rw-r--r--   0        0        0     1279 2023-06-27 02:38:06.424159 pdm-2.8.0a0/src/pdm/cli/commands/venv/remove.py
+-rw-r--r--   0        0        0     2759 2023-06-27 02:38:06.424159 pdm-2.8.0a0/src/pdm/cli/commands/venv/utils.py
+-rw-r--r--   0        0        0        0 2023-06-27 02:38:06.424159 pdm-2.8.0a0/src/pdm/cli/completions/__init__.py
+-rw-r--r--   0        0        0     5113 2023-06-27 02:38:06.424159 pdm-2.8.0a0/src/pdm/cli/completions/pdm.bash
+-rw-r--r--   0        0        0    50280 2023-06-27 02:38:06.424159 pdm-2.8.0a0/src/pdm/cli/completions/pdm.fish
+-rw-r--r--   0        0        0    18599 2023-06-27 02:38:06.424159 pdm-2.8.0a0/src/pdm/cli/completions/pdm.ps1
+-rw-r--r--   0        0        0    25289 2023-06-27 02:38:06.424159 pdm-2.8.0a0/src/pdm/cli/completions/pdm.zsh
+-rw-r--r--   0        0        0     3840 2023-06-27 02:38:06.424159 pdm-2.8.0a0/src/pdm/cli/filters.py
+-rw-r--r--   0        0        0     1481 2023-06-27 02:38:06.424159 pdm-2.8.0a0/src/pdm/cli/hooks.py
+-rw-r--r--   0        0        0    10461 2023-06-27 02:38:06.424159 pdm-2.8.0a0/src/pdm/cli/options.py
+-rw-r--r--   0        0        0     6235 2023-06-27 02:38:06.424159 pdm-2.8.0a0/src/pdm/cli/templates/__init__.py
+-rw-r--r--   0        0        0     3102 2023-06-27 02:38:06.424159 pdm-2.8.0a0/src/pdm/cli/templates/default/.gitignore
+-rw-r--r--   0        0        0       18 2023-06-27 02:38:06.424159 pdm-2.8.0a0/src/pdm/cli/templates/default/README.md
+-rw-r--r--   0        0        0        0 2023-06-27 02:38:06.424159 pdm-2.8.0a0/src/pdm/cli/templates/default/__init__.py
+-rw-r--r--   0        0        0      278 2023-06-27 02:38:06.424159 pdm-2.8.0a0/src/pdm/cli/templates/default/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-27 02:38:06.424159 pdm-2.8.0a0/src/pdm/cli/templates/default/src/example_package/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-27 02:38:06.424159 pdm-2.8.0a0/src/pdm/cli/templates/default/tests/__init__.py
+-rw-r--r--   0        0        0    25152 2023-06-27 02:38:06.424159 pdm-2.8.0a0/src/pdm/cli/utils.py
+-rw-r--r--   0        0        0     2373 2023-06-27 02:38:06.424159 pdm-2.8.0a0/src/pdm/compat.py
+-rw-r--r--   0        0        0    10667 2023-06-27 02:38:06.424159 pdm-2.8.0a0/src/pdm/core.py
+-rw-r--r--   0        0        0      825 2023-06-27 02:38:06.424159 pdm-2.8.0a0/src/pdm/environments/__init__.py
+-rw-r--r--   0        0        0     8850 2023-06-27 02:38:06.424159 pdm-2.8.0a0/src/pdm/environments/base.py
+-rw-r--r--   0        0        0     4255 2023-06-27 02:38:06.424159 pdm-2.8.0a0/src/pdm/environments/local.py
+-rw-r--r--   0        0        0     1600 2023-06-27 02:38:06.424159 pdm-2.8.0a0/src/pdm/environments/python.py
+-rw-r--r--   0        0        0     1362 2023-06-27 02:38:06.424159 pdm-2.8.0a0/src/pdm/exceptions.py
+-rw-r--r--   0        0        0     1202 2023-06-27 02:38:06.424159 pdm-2.8.0a0/src/pdm/formats/__init__.py
+-rw-r--r--   0        0        0     3215 2023-06-27 02:38:06.424159 pdm-2.8.0a0/src/pdm/formats/base.py
+-rw-r--r--   0        0        0     5788 2023-06-27 02:38:06.424159 pdm-2.8.0a0/src/pdm/formats/flit.py
+-rw-r--r--   0        0        0     2614 2023-06-27 02:38:06.424159 pdm-2.8.0a0/src/pdm/formats/pipfile.py
+-rw-r--r--   0        0        0     7490 2023-06-27 02:38:06.424159 pdm-2.8.0a0/src/pdm/formats/poetry.py
+-rw-r--r--   0        0        0     7502 2023-06-27 02:38:06.424159 pdm-2.8.0a0/src/pdm/formats/requirements.py
+-rw-r--r--   0        0        0     2309 2023-06-27 02:38:06.428159 pdm-2.8.0a0/src/pdm/formats/setup_py.py
+-rw-r--r--   0        0        0      119 2023-06-27 02:38:06.428159 pdm-2.8.0a0/src/pdm/installers/__init__.py
+-rw-r--r--   0        0        0     1390 2023-06-27 02:38:06.428159 pdm-2.8.0a0/src/pdm/installers/core.py
+-rw-r--r--   0        0        0    10901 2023-06-27 02:38:06.428159 pdm-2.8.0a0/src/pdm/installers/installers.py
+-rw-r--r--   0        0        0     2091 2023-06-27 02:38:06.428159 pdm-2.8.0a0/src/pdm/installers/manager.py
+-rw-r--r--   0        0        0     2226 2023-06-27 02:38:06.428159 pdm-2.8.0a0/src/pdm/installers/packages.py
+-rw-r--r--   0        0        0    18161 2023-06-27 02:38:06.428159 pdm-2.8.0a0/src/pdm/installers/synchronizers.py
+-rw-r--r--   0        0        0    10990 2023-06-27 02:38:06.428159 pdm-2.8.0a0/src/pdm/installers/uninstallers.py
+-rw-r--r--   0        0        0        0 2023-06-27 02:38:06.428159 pdm-2.8.0a0/src/pdm/models/__init__.py
+-rw-r--r--   0        0        0     3162 2023-06-27 02:38:06.428159 pdm-2.8.0a0/src/pdm/models/auth.py
+-rw-r--r--   0        0        0     4698 2023-06-27 02:38:06.428159 pdm-2.8.0a0/src/pdm/models/backends.py
+-rw-r--r--   0        0        0    11710 2023-06-27 02:38:06.428159 pdm-2.8.0a0/src/pdm/models/caches.py
+-rw-r--r--   0        0        0    26580 2023-06-27 02:38:06.428159 pdm-2.8.0a0/src/pdm/models/candidates.py
+-rw-r--r--   0        0        0      287 2023-06-27 02:38:06.428159 pdm-2.8.0a0/src/pdm/models/environment.py
+-rw-r--r--   0        0        0     1845 2023-06-27 02:38:06.428159 pdm-2.8.0a0/src/pdm/models/in_process/__init__.py
+-rw-r--r--   0        0        0     2049 2023-06-27 02:38:06.428159 pdm-2.8.0a0/src/pdm/models/in_process/get_abi_tag.py
+-rw-r--r--   0        0        0     6323 2023-06-27 02:38:06.428159 pdm-2.8.0a0/src/pdm/models/in_process/parse_setup.py
+-rw-r--r--   0        0        0     1165 2023-06-27 02:38:06.428159 pdm-2.8.0a0/src/pdm/models/in_process/pep508.py
+-rw-r--r--   0        0        0     1653 2023-06-27 02:38:06.428159 pdm-2.8.0a0/src/pdm/models/in_process/sysconfig_get_paths.py
+-rw-r--r--   0        0        0     5701 2023-06-27 02:38:06.428159 pdm-2.8.0a0/src/pdm/models/markers.py
+-rw-r--r--   0        0        0     3507 2023-06-27 02:38:06.428159 pdm-2.8.0a0/src/pdm/models/project_info.py
+-rw-r--r--   0        0        0     2195 2023-06-27 02:38:06.428159 pdm-2.8.0a0/src/pdm/models/python.py
+-rw-r--r--   0        0        0      318 2023-06-27 02:38:06.428159 pdm-2.8.0a0/src/pdm/models/python_max_versions.json
+-rw-r--r--   0        0        0    21340 2023-06-27 02:38:06.428159 pdm-2.8.0a0/src/pdm/models/repositories.py
+-rw-r--r--   0        0        0    18792 2023-06-27 02:38:06.428159 pdm-2.8.0a0/src/pdm/models/requirements.py
+-rw-r--r--   0        0        0     2313 2023-06-27 02:38:06.428159 pdm-2.8.0a0/src/pdm/models/search.py
+-rw-r--r--   0        0        0     3225 2023-06-27 02:38:06.428159 pdm-2.8.0a0/src/pdm/models/session.py
+-rw-r--r--   0        0        0    14482 2023-06-27 02:38:06.428159 pdm-2.8.0a0/src/pdm/models/setup.py
+-rw-r--r--   0        0        0    16337 2023-06-27 02:38:06.428159 pdm-2.8.0a0/src/pdm/models/specifiers.py
+-rw-r--r--   0        0        0     1300 2023-06-27 02:38:06.428159 pdm-2.8.0a0/src/pdm/models/venv.py
+-rw-r--r--   0        0        0     5924 2023-06-27 02:38:06.428159 pdm-2.8.0a0/src/pdm/models/versions.py
+-rw-r--r--   0        0        0     2766 2023-06-27 02:38:06.428159 pdm-2.8.0a0/src/pdm/models/working_set.py
+-rw-r--r--   0        0        0        0 2023-06-27 02:38:06.428159 pdm-2.8.0a0/src/pdm/pep582/__init__.py
+-rw-r--r--   0        0        0     4481 2023-06-27 02:38:06.428159 pdm-2.8.0a0/src/pdm/pep582/sitecustomize.py
+-rw-r--r--   0        0        0      134 2023-06-27 02:38:06.428159 pdm-2.8.0a0/src/pdm/project/__init__.py
+-rw-r--r--   0        0        0    16757 2023-06-27 02:38:06.428159 pdm-2.8.0a0/src/pdm/project/config.py
+-rw-r--r--   0        0        0    26292 2023-06-27 02:38:06.428159 pdm-2.8.0a0/src/pdm/project/core.py
+-rw-r--r--   0        0        0     2093 2023-06-27 02:38:06.428159 pdm-2.8.0a0/src/pdm/project/lockfile.py
+-rw-r--r--   0        0        0     3385 2023-06-27 02:38:06.428159 pdm-2.8.0a0/src/pdm/project/project_file.py
+-rw-r--r--   0        0        0     1070 2023-06-27 02:38:06.428159 pdm-2.8.0a0/src/pdm/project/toml_file.py
+-rw-r--r--   0        0        0        0 2023-06-27 02:38:06.428159 pdm-2.8.0a0/src/pdm/py.typed
+-rw-r--r--   0        0        0    20185 2023-06-27 02:38:06.428159 pdm-2.8.0a0/src/pdm/pytest.py
+-rw-r--r--   0        0        0       61 2023-06-27 02:38:06.428159 pdm-2.8.0a0/src/pdm/resolver/__init__.py
+-rw-r--r--   0        0        0     1954 2023-06-27 02:38:06.428159 pdm-2.8.0a0/src/pdm/resolver/core.py
+-rw-r--r--   0        0        0    13176 2023-06-27 02:38:06.428159 pdm-2.8.0a0/src/pdm/resolver/providers.py
+-rw-r--r--   0        0        0     1580 2023-06-27 02:38:06.428159 pdm-2.8.0a0/src/pdm/resolver/python.py
+-rw-r--r--   0        0        0     3742 2023-06-27 02:38:06.428159 pdm-2.8.0a0/src/pdm/resolver/reporters.py
+-rw-r--r--   0        0        0     4027 2023-06-27 02:38:06.428159 pdm-2.8.0a0/src/pdm/signals.py
+-rw-r--r--   0        0        0     8054 2023-06-27 02:38:06.428159 pdm-2.8.0a0/src/pdm/termui.py
+-rw-r--r--   0        0        0    13856 2023-06-27 02:38:06.428159 pdm-2.8.0a0/src/pdm/utils.py
+-rw-r--r--   0        0        0       72 2023-06-27 02:38:06.428159 pdm-2.8.0a0/tests/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-27 02:38:06.428159 pdm-2.8.0a0/tests/cli/__init__.py
+-rw-r--r--   0        0        0     3723 2023-06-27 02:38:06.428159 pdm-2.8.0a0/tests/cli/conftest.py
+-rw-r--r--   0        0        0    12362 2023-06-27 02:38:06.428159 pdm-2.8.0a0/tests/cli/test_add.py
+-rw-r--r--   0        0        0     5775 2023-06-27 02:38:06.428159 pdm-2.8.0a0/tests/cli/test_build.py
+-rw-r--r--   0        0        0     5229 2023-06-27 02:38:06.428159 pdm-2.8.0a0/tests/cli/test_cache.py
+-rw-r--r--   0        0        0     9286 2023-06-27 02:38:06.428159 pdm-2.8.0a0/tests/cli/test_config.py
+-rw-r--r--   0        0        0     2029 2023-06-27 02:38:06.428159 pdm-2.8.0a0/tests/cli/test_fix.py
+-rw-r--r--   0        0        0    10375 2023-06-27 02:38:06.432159 pdm-2.8.0a0/tests/cli/test_hooks.py
+-rw-r--r--   0        0        0     4950 2023-06-27 02:38:06.432159 pdm-2.8.0a0/tests/cli/test_init.py
+-rw-r--r--   0        0        0    11265 2023-06-27 02:38:06.432159 pdm-2.8.0a0/tests/cli/test_install.py
+-rw-r--r--   0        0        0    28998 2023-06-27 02:38:06.432159 pdm-2.8.0a0/tests/cli/test_list.py
+-rw-r--r--   0        0        0     6324 2023-06-27 02:38:06.432159 pdm-2.8.0a0/tests/cli/test_lock.py
+-rw-r--r--   0        0        0     7796 2023-06-27 02:38:06.432159 pdm-2.8.0a0/tests/cli/test_others.py
+-rw-r--r--   0        0        0     6052 2023-06-27 02:38:06.432159 pdm-2.8.0a0/tests/cli/test_publish.py
+-rw-r--r--   0        0        0     3888 2023-06-27 02:38:06.432159 pdm-2.8.0a0/tests/cli/test_remove.py
+-rw-r--r--   0        0        0    29259 2023-06-27 02:38:06.432159 pdm-2.8.0a0/tests/cli/test_run.py
+-rw-r--r--   0        0        0     3599 2023-06-27 02:38:06.432159 pdm-2.8.0a0/tests/cli/test_self_command.py
+-rw-r--r--   0        0        0     2778 2023-06-27 02:38:06.432159 pdm-2.8.0a0/tests/cli/test_template.py
+-rw-r--r--   0        0        0     8876 2023-06-27 02:38:06.432159 pdm-2.8.0a0/tests/cli/test_update.py
+-rw-r--r--   0        0        0     2997 2023-06-27 02:38:06.432159 pdm-2.8.0a0/tests/cli/test_use.py
+-rw-r--r--   0        0        0    10808 2023-06-27 02:38:06.432159 pdm-2.8.0a0/tests/cli/test_venv.py
+-rw-r--r--   0        0        0     3079 2023-06-27 02:38:06.432159 pdm-2.8.0a0/tests/conftest.py
+-rw-r--r--   0        0        0      235 2023-06-27 02:38:06.432159 pdm-2.8.0a0/tests/fixtures/Pipfile
+-rw-r--r--   0        0        0        0 2023-06-27 02:38:06.432159 pdm-2.8.0a0/tests/fixtures/__init__.py
+-rw-r--r--   0        0        0    49497 2023-06-27 02:38:06.432159 pdm-2.8.0a0/tests/fixtures/artifacts/PyFunctional-1.4.3-py3-none-any.whl
+-rw-r--r--   0        0        0      546 2023-06-27 02:38:06.432159 pdm-2.8.0a0/tests/fixtures/artifacts/caj2pdf-restructured-0.1.0a6.tar.gz
+-rw-r--r--   0        0        0   422824 2023-06-27 02:38:06.436159 pdm-2.8.0a0/tests/fixtures/artifacts/celery-4.4.2-py2.py3-none-any.whl
+-rw-r--r--   0        0        0     1254 2023-06-27 02:38:06.436159 pdm-2.8.0a0/tests/fixtures/artifacts/demo-0.0.1-cp36-cp36m-win_amd64.whl
+-rw-r--r--   0        0        0     1254 2023-06-27 02:38:06.436159 pdm-2.8.0a0/tests/fixtures/artifacts/demo-0.0.1-py2.py3-none-any.whl
+-rw-r--r--   0        0        0     1038 2023-06-27 02:38:06.436159 pdm-2.8.0a0/tests/fixtures/artifacts/demo-0.0.1.tar.gz
+-rw-r--r--   0        0        0     2615 2023-06-27 02:38:06.436159 pdm-2.8.0a0/tests/fixtures/artifacts/demo-0.0.1.zip
+-rw-r--r--   0        0        0     4595 2023-06-27 02:38:06.436159 pdm-2.8.0a0/tests/fixtures/artifacts/editables-0.2-py3-none-any.whl
+-rw-r--r--   0        0        0     5359 2023-06-27 02:38:06.436159 pdm-2.8.0a0/tests/fixtures/artifacts/first-2.0.2-py2.py3-none-any.whl
+-rw-r--r--   0        0        0    56715 2023-06-27 02:38:06.436159 pdm-2.8.0a0/tests/fixtures/artifacts/flit_core-3.6.0-py3-none-any.whl
+-rw-r--r--   0        0        0     6138 2023-06-27 02:38:06.436159 pdm-2.8.0a0/tests/fixtures/artifacts/future_fstrings-1.2.0-py2.py3-none-any.whl
+-rw-r--r--   0        0        0     5786 2023-06-27 02:38:06.436159 pdm-2.8.0a0/tests/fixtures/artifacts/future_fstrings-1.2.0.tar.gz
+-rw-r--r--   0        0        0    17978 2023-06-27 02:38:06.436159 pdm-2.8.0a0/tests/fixtures/artifacts/importlib_metadata-4.8.3-py3-none-any.whl
+-rw-r--r--   0        0        0    24489 2023-06-27 02:38:06.436159 pdm-2.8.0a0/tests/fixtures/artifacts/jmespath-0.10.0-py2.py3-none-any.whl
+-rw-r--r--   0        0        0   156727 2023-06-27 02:38:06.436159 pdm-2.8.0a0/tests/fixtures/artifacts/pdm_backend-2.0.2-py3-none-any.whl
+-rw-r--r--   0        0        0     1401 2023-06-27 02:38:06.436159 pdm-2.8.0a0/tests/fixtures/artifacts/pdm_hello-0.1.0-py3-none-any.whl
+-rw-r--r--   0        0        0     1405 2023-06-27 02:38:06.436159 pdm-2.8.0a0/tests/fixtures/artifacts/pdm_hello-0.1.0-py3-none-win_amd64.whl
+-rw-r--r--   0        0        0   305481 2023-06-27 02:38:06.440159 pdm-2.8.0a0/tests/fixtures/artifacts/pdm_pep517-1.0.0-py3-none-any.whl
+-rw-r--r--   0        0        0   531270 2023-06-27 02:38:06.440159 pdm-2.8.0a0/tests/fixtures/artifacts/poetry_core-1.3.2-py3-none-any.whl
+-rw-r--r--   0        0        0  1232518 2023-06-27 02:38:06.448160 pdm-2.8.0a0/tests/fixtures/artifacts/setuptools-65.4.1-py3-none-any.whl
+-rw-r--r--   0        0        0    26662 2023-06-27 02:38:06.448160 pdm-2.8.0a0/tests/fixtures/artifacts/typing_extensions-4.4.0-py3-none-any.whl
+-rw-r--r--   0        0        0    35301 2023-06-27 02:38:06.448160 pdm-2.8.0a0/tests/fixtures/artifacts/wheel-0.37.1-py2.py3-none-any.whl
+-rw-r--r--   0        0        0     5312 2023-06-27 02:38:06.448160 pdm-2.8.0a0/tests/fixtures/artifacts/zipp-3.7.0-py3-none-any.whl
+-rw-r--r--   0        0        0      326 2023-06-27 02:38:06.448160 pdm-2.8.0a0/tests/fixtures/index/demo.html
+-rw-r--r--   0        0        0      511 2023-06-27 02:38:06.448160 pdm-2.8.0a0/tests/fixtures/index/future-fstrings.html
+-rw-r--r--   0        0        0      262 2023-06-27 02:38:06.448160 pdm-2.8.0a0/tests/fixtures/index/pep345-legacy.html
+-rw-r--r--   0        0        0      262 2023-06-27 02:38:06.448160 pdm-2.8.0a0/tests/fixtures/index/wheel.html
+-rw-r--r--   0        0        0        0 2023-06-27 02:38:06.448160 pdm-2.8.0a0/tests/fixtures/projects/__init__.py
+-rw-r--r--   0        0        0       42 2023-06-27 02:38:06.448160 pdm-2.8.0a0/tests/fixtures/projects/demo-#-with-hash/demo.py
+-rw-r--r--   0        0        0      332 2023-06-27 02:38:06.448160 pdm-2.8.0a0/tests/fixtures/projects/demo-#-with-hash/setup.py
+-rw-r--r--   0        0        0       26 2023-06-27 02:38:06.448160 pdm-2.8.0a0/tests/fixtures/projects/demo-combined-extras/demo.py
+-rw-r--r--   0        0        0      462 2023-06-27 02:38:06.448160 pdm-2.8.0a0/tests/fixtures/projects/demo-combined-extras/pyproject.toml
+-rw-r--r--   0        0        0       42 2023-06-27 02:38:06.448160 pdm-2.8.0a0/tests/fixtures/projects/demo-failure-no-dep/demo.py
+-rw-r--r--   0        0        0      246 2023-06-27 02:38:06.448160 pdm-2.8.0a0/tests/fixtures/projects/demo-failure-no-dep/setup.py
+-rw-r--r--   0        0        0       42 2023-06-27 02:38:06.448160 pdm-2.8.0a0/tests/fixtures/projects/demo-failure/demo.py
+-rw-r--r--   0        0        0      345 2023-06-27 02:38:06.448160 pdm-2.8.0a0/tests/fixtures/projects/demo-failure/setup.py
+-rw-r--r--   0        0        0       12 2023-06-27 02:38:06.448160 pdm-2.8.0a0/tests/fixtures/projects/demo-module/LICENSE
+-rw-r--r--   0        0        0       24 2023-06-27 02:38:06.448160 pdm-2.8.0a0/tests/fixtures/projects/demo-module/README.md
+-rw-r--r--   0        0        0       14 2023-06-27 02:38:06.448160 pdm-2.8.0a0/tests/fixtures/projects/demo-module/bar_module.py
+-rw-r--r--   0        0        0       36 2023-06-27 02:38:06.448160 pdm-2.8.0a0/tests/fixtures/projects/demo-module/foo_module.py
+-rw-r--r--   0        0        0      442 2023-06-27 02:38:06.448160 pdm-2.8.0a0/tests/fixtures/projects/demo-module/pyproject.toml
+-rw-r--r--   0        0        0     3983 2023-06-27 02:38:06.448160 pdm-2.8.0a0/tests/fixtures/projects/demo-package-has-dep-with-extras/pdm.lock
+-rw-r--r--   0        0        0      318 2023-06-27 02:38:06.448160 pdm-2.8.0a0/tests/fixtures/projects/demo-package-has-dep-with-extras/pyproject.toml
+-rw-r--r--   0        0        0      157 2023-06-27 02:38:06.448160 pdm-2.8.0a0/tests/fixtures/projects/demo-package-has-dep-with-extras/requirements.txt
+-rw-r--r--   0        0        0       12 2023-06-27 02:38:06.448160 pdm-2.8.0a0/tests/fixtures/projects/demo-package/LICENSE
+-rw-r--r--   0        0        0       13 2023-06-27 02:38:06.448160 pdm-2.8.0a0/tests/fixtures/projects/demo-package/README.md
+-rw-r--r--   0        0        0       16 2023-06-27 02:38:06.448160 pdm-2.8.0a0/tests/fixtures/projects/demo-package/data_out.json
+-rw-r--r--   0        0        0       22 2023-06-27 02:38:06.448160 pdm-2.8.0a0/tests/fixtures/projects/demo-package/my_package/__init__.py
+-rw-r--r--   0        0        0       24 2023-06-27 02:38:06.448160 pdm-2.8.0a0/tests/fixtures/projects/demo-package/my_package/data.json
+-rw-r--r--   0        0        0    29800 2023-06-27 02:38:06.448160 pdm-2.8.0a0/tests/fixtures/projects/demo-package/pdm.lock
+-rw-r--r--   0        0        0      572 2023-06-27 02:38:06.448160 pdm-2.8.0a0/tests/fixtures/projects/demo-package/pyproject.toml
+-rw-r--r--   0        0        0      122 2023-06-27 02:38:06.448160 pdm-2.8.0a0/tests/fixtures/projects/demo-package/requirements.ini
+-rw-r--r--   0        0        0     7521 2023-06-27 02:38:06.448160 pdm-2.8.0a0/tests/fixtures/projects/demo-package/requirements.txt
+-rw-r--r--   0        0        0      211 2023-06-27 02:38:06.448160 pdm-2.8.0a0/tests/fixtures/projects/demo-package/requirements_simple.txt
+-rw-r--r--   0        0        0      726 2023-06-27 02:38:06.448160 pdm-2.8.0a0/tests/fixtures/projects/demo-package/setup.txt
+-rw-r--r--   0        0        0       21 2023-06-27 02:38:06.448160 pdm-2.8.0a0/tests/fixtures/projects/demo-package/single_module.py
+-rw-r--r--   0        0        0       18 2023-06-27 02:38:06.448160 pdm-2.8.0a0/tests/fixtures/projects/demo-parent-package/README.md
+-rw-r--r--   0        0        0       22 2023-06-27 02:38:06.448160 pdm-2.8.0a0/tests/fixtures/projects/demo-parent-package/package-a/foo.py
+-rw-r--r--   0        0        0      120 2023-06-27 02:38:06.448160 pdm-2.8.0a0/tests/fixtures/projects/demo-parent-package/package-a/setup.py
+-rw-r--r--   0        0        0       22 2023-06-27 02:38:06.448160 pdm-2.8.0a0/tests/fixtures/projects/demo-parent-package/package-b/bar.py
+-rw-r--r--   0        0        0      197 2023-06-27 02:38:06.448160 pdm-2.8.0a0/tests/fixtures/projects/demo-parent-package/package-b/pyproject.toml
+-rw-r--r--   0        0        0       42 2023-06-27 02:38:06.448160 pdm-2.8.0a0/tests/fixtures/projects/demo-prerelease/demo.py
+-rw-r--r--   0        0        0      334 2023-06-27 02:38:06.448160 pdm-2.8.0a0/tests/fixtures/projects/demo-prerelease/setup.py
+-rw-r--r--   0        0        0       12 2023-06-27 02:38:06.448160 pdm-2.8.0a0/tests/fixtures/projects/demo-src-package/LICENSE
+-rw-r--r--   0        0        0       24 2023-06-27 02:38:06.448160 pdm-2.8.0a0/tests/fixtures/projects/demo-src-package/README.md
+-rw-r--r--   0        0        0       16 2023-06-27 02:38:06.448160 pdm-2.8.0a0/tests/fixtures/projects/demo-src-package/data_out.json
+-rw-r--r--   0        0        0      456 2023-06-27 02:38:06.448160 pdm-2.8.0a0/tests/fixtures/projects/demo-src-package/pyproject.toml
+-rw-r--r--   0        0        0       21 2023-06-27 02:38:06.448160 pdm-2.8.0a0/tests/fixtures/projects/demo-src-package/single_module.py
+-rw-r--r--   0        0        0       22 2023-06-27 02:38:06.448160 pdm-2.8.0a0/tests/fixtures/projects/demo-src-package/src/my_package/__init__.py
+-rw-r--r--   0        0        0       24 2023-06-27 02:38:06.448160 pdm-2.8.0a0/tests/fixtures/projects/demo-src-package/src/my_package/data.json
+-rw-r--r--   0        0        0       42 2023-06-27 02:38:06.448160 pdm-2.8.0a0/tests/fixtures/projects/demo/demo.py
+-rw-r--r--   0        0        0      344 2023-06-27 02:38:06.448160 pdm-2.8.0a0/tests/fixtures/projects/demo/pyproject.toml
+-rw-r--r--   0        0        0       26 2023-06-27 02:38:06.448160 pdm-2.8.0a0/tests/fixtures/projects/demo_extras/demo.py
+-rw-r--r--   0        0        0      250 2023-06-27 02:38:06.448160 pdm-2.8.0a0/tests/fixtures/projects/demo_extras/setup.py
+-rw-r--r--   0        0        0        0 2023-06-27 02:38:06.448160 pdm-2.8.0a0/tests/fixtures/projects/flit-demo/README.rst
+-rw-r--r--   0        0        0        0 2023-06-27 02:38:06.448160 pdm-2.8.0a0/tests/fixtures/projects/flit-demo/doc/index.html
+-rw-r--r--   0        0        0       49 2023-06-27 02:38:06.448160 pdm-2.8.0a0/tests/fixtures/projects/flit-demo/flit.py
+-rw-r--r--   0        0        0      969 2023-06-27 02:38:06.448160 pdm-2.8.0a0/tests/fixtures/projects/flit-demo/pyproject.toml
+-rw-r--r--   0        0        0       12 2023-06-27 02:38:06.448160 pdm-2.8.0a0/tests/fixtures/projects/poetry-demo/mylib.py
+-rw-r--r--   0        0        0      863 2023-06-27 02:38:06.448160 pdm-2.8.0a0/tests/fixtures/projects/poetry-demo/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-27 02:38:06.448160 pdm-2.8.0a0/tests/fixtures/projects/test-hatch-static/README.md
+-rw-r--r--   0        0        0      386 2023-06-27 02:38:06.448160 pdm-2.8.0a0/tests/fixtures/projects/test-hatch-static/pyproject.toml
+-rw-r--r--   0        0        0       11 2023-06-27 02:38:06.448160 pdm-2.8.0a0/tests/fixtures/projects/test-monorepo/README.md
+-rw-r--r--   0        0        0        0 2023-06-27 02:38:06.452160 pdm-2.8.0a0/tests/fixtures/projects/test-monorepo/core/core.py
+-rw-r--r--   0        0        0      179 2023-06-27 02:38:06.452160 pdm-2.8.0a0/tests/fixtures/projects/test-monorepo/core/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-27 02:38:06.452160 pdm-2.8.0a0/tests/fixtures/projects/test-monorepo/package_a/alice.py
+-rw-r--r--   0        0        0      231 2023-06-27 02:38:06.452160 pdm-2.8.0a0/tests/fixtures/projects/test-monorepo/package_a/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-27 02:38:06.452160 pdm-2.8.0a0/tests/fixtures/projects/test-monorepo/package_b/bob.py
+-rw-r--r--   0        0        0      231 2023-06-27 02:38:06.452160 pdm-2.8.0a0/tests/fixtures/projects/test-monorepo/package_b/pyproject.toml
+-rw-r--r--   0        0        0      237 2023-06-27 02:38:06.452160 pdm-2.8.0a0/tests/fixtures/projects/test-monorepo/pyproject.toml
+-rw-r--r--   0        0        0      380 2023-06-27 02:38:06.452160 pdm-2.8.0a0/tests/fixtures/projects/test-plugin-pdm/hello.py
+-rw-r--r--   0        0        0      312 2023-06-27 02:38:06.452160 pdm-2.8.0a0/tests/fixtures/projects/test-plugin-pdm/pyproject.toml
+-rw-r--r--   0        0        0      380 2023-06-27 02:38:06.452160 pdm-2.8.0a0/tests/fixtures/projects/test-plugin/hello.py
+-rw-r--r--   0        0        0      168 2023-06-27 02:38:06.452160 pdm-2.8.0a0/tests/fixtures/projects/test-plugin/setup.py
+-rw-r--r--   0        0        0        0 2023-06-27 02:38:06.452160 pdm-2.8.0a0/tests/fixtures/projects/test-removal/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-27 02:38:06.452160 pdm-2.8.0a0/tests/fixtures/projects/test-removal/bar.py
+-rw-r--r--   0        0        0        0 2023-06-27 02:38:06.452160 pdm-2.8.0a0/tests/fixtures/projects/test-removal/foo.py
+-rw-r--r--   0        0        0        0 2023-06-27 02:38:06.452160 pdm-2.8.0a0/tests/fixtures/projects/test-removal/subdir/__init__.py
+-rw-r--r--   0        0        0       10 2023-06-27 02:38:06.452160 pdm-2.8.0a0/tests/fixtures/projects/test-setuptools/AUTHORS
+-rw-r--r--   0        0        0       12 2023-06-27 02:38:06.452160 pdm-2.8.0a0/tests/fixtures/projects/test-setuptools/README.md
+-rw-r--r--   0        0        0       22 2023-06-27 02:38:06.452160 pdm-2.8.0a0/tests/fixtures/projects/test-setuptools/mymodule.py
+-rw-r--r--   0        0        0      398 2023-06-27 02:38:06.452160 pdm-2.8.0a0/tests/fixtures/projects/test-setuptools/setup.cfg
+-rw-r--r--   0        0        0      308 2023-06-27 02:38:06.452160 pdm-2.8.0a0/tests/fixtures/projects/test-setuptools/setup.py
+-rw-r--r--   0        0        0     1525 2023-06-27 02:38:06.452160 pdm-2.8.0a0/tests/fixtures/pypi.json
+-rw-r--r--   0        0        0     1330 2023-06-27 02:38:06.452160 pdm-2.8.0a0/tests/fixtures/pyproject.toml
+-rw-r--r--   0        0        0       20 2023-06-27 02:38:06.452160 pdm-2.8.0a0/tests/fixtures/requirements-include.txt
+-rw-r--r--   0        0        0      502 2023-06-27 02:38:06.452160 pdm-2.8.0a0/tests/fixtures/requirements.txt
+-rw-r--r--   0        0        0        0 2023-06-27 02:38:06.452160 pdm-2.8.0a0/tests/models/__init__.py
+-rw-r--r--   0        0        0     3814 2023-06-27 02:38:06.452160 pdm-2.8.0a0/tests/models/test_backends.py
+-rw-r--r--   0        0        0    13344 2023-06-27 02:38:06.452160 pdm-2.8.0a0/tests/models/test_candidates.py
+-rw-r--r--   0        0        0     1971 2023-06-27 02:38:06.452160 pdm-2.8.0a0/tests/models/test_marker.py
+-rw-r--r--   0        0        0     2679 2023-06-27 02:38:06.452160 pdm-2.8.0a0/tests/models/test_requirements.py
+-rw-r--r--   0        0        0     2556 2023-06-27 02:38:06.452160 pdm-2.8.0a0/tests/models/test_setup_parsing.py
+-rw-r--r--   0        0        0     3418 2023-06-27 02:38:06.452160 pdm-2.8.0a0/tests/models/test_specifiers.py
+-rw-r--r--   0        0        0     2703 2023-06-27 02:38:06.452160 pdm-2.8.0a0/tests/models/test_versions.py
+-rw-r--r--   0        0        0        0 2023-06-27 02:38:06.452160 pdm-2.8.0a0/tests/resolver/__init__.py
+-rw-r--r--   0        0        0    11567 2023-06-27 02:38:06.452160 pdm-2.8.0a0/tests/resolver/test_resolve.py
+-rw-r--r--   0        0        0     7704 2023-06-27 02:38:06.452160 pdm-2.8.0a0/tests/test_formats.py
+-rw-r--r--   0        0        0     7231 2023-06-27 02:38:06.452160 pdm-2.8.0a0/tests/test_installer.py
+-rw-r--r--   0        0        0     1829 2023-06-27 02:38:06.452160 pdm-2.8.0a0/tests/test_integration.py
+-rw-r--r--   0        0        0     3435 2023-06-27 02:38:06.452160 pdm-2.8.0a0/tests/test_plugin.py
+-rw-r--r--   0        0        0    12085 2023-06-27 02:38:06.452160 pdm-2.8.0a0/tests/test_project.py
+-rw-r--r--   0        0        0     1103 2023-06-27 02:38:06.452160 pdm-2.8.0a0/tests/test_signals.py
+-rw-r--r--   0        0        0     4409 2023-06-27 02:38:06.452160 pdm-2.8.0a0/tests/test_utils.py
+-rw-r--r--   0        0        0     9626 1970-01-01 00:00:00.000000 pdm-2.8.0a0/PKG-INFO
```

### Comparing `pdm-2.7.4/CHANGELOG.md` & `pdm-2.8.0a0/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,30 @@
+Release v2.8.0a0 (2023-06-27)
+-----------------------------
+
+### Features & Improvements
+
+- Replace the `DeprecationWarning` with `FutureWarning` for better exposure. [#2012](https://github.com/pdm-project/pdm/issues/2012)
+- Serve `install-pdm.py` and its checksum file on the docs site. [#2026](https://github.com/pdm-project/pdm/issues/2026)
+- Add new option `--edit/-e` to `pdm config` to edit the config file in default editor. [#2028](https://github.com/pdm-project/pdm/issues/2028)
+- Add `--project` option to `pdm venv` to support another path as the project root. [#2042](https://github.com/pdm-project/pdm/issues/2042)
+- Add support for using `truststore` as the SSL backend. This only works on Python 3.10 or newer. [#2049](https://github.com/pdm-project/pdm/issues/2049)
+
+### Bug Fixes
+
+- Fix the breaking change by adding the functions back to the old location with deprecation warnings. [#2013](https://github.com/pdm-project/pdm/issues/2013)
+- Fix the duplicate entries in the output of `pdm self list`. [#2018](https://github.com/pdm-project/pdm/issues/2018)
+- Disable hashes caching for local files. [#2019](https://github.com/pdm-project/pdm/issues/2019)
+- Populate the `url` field when converting requirements from a Pipfile-style file requirement. [#2032](https://github.com/pdm-project/pdm/issues/2032)
+- Fix a bug that empty source tables in configuration files causes errors when running pdm commands. [#2034](https://github.com/pdm-project/pdm/issues/2034)
+- Fix a resolution conflict caused by requested yanked version also in other transitive dependencies. [#2038](https://github.com/pdm-project/pdm/issues/2038)
+- Fix a bug that binary executables are corrupted when replacing shebangs. [#2045](https://github.com/pdm-project/pdm/issues/2045)
+- Do not normalize the package name when uploading to PyPI. [#2057](https://github.com/pdm-project/pdm/issues/2057)
+
+
 Release v2.7.4 (2023-06-13)
 ---------------------------
 
 No significant changes.
 
 
 Release v2.7.3 (2023-06-13)
```

### Comparing `pdm-2.7.4/LICENSE` & `pdm-2.8.0a0/LICENSE`

 * *Files identical despite different names*

### Comparing `pdm-2.7.4/README.md` & `pdm-2.8.0a0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -81,25 +81,25 @@
 ### Via Install Script
 
 Like Pip, PDM provides an installation script that will install PDM into an isolated environment.
 
 **For Linux/Mac**
 
 ```bash
-curl -sSL https://raw.githubusercontent.com/pdm-project/pdm/main/install-pdm.py | python3 -
+curl -sSL https://pdm.fming.dev/dev/install-pdm.py | python3 -
 ```
 
 **For Windows**
 
 ```powershell
-(Invoke-WebRequest -Uri https://raw.githubusercontent.com/pdm-project/pdm/main/install-pdm.py -UseBasicParsing).Content | python -
+(Invoke-WebRequest -Uri https://pdm.fming.dev/dev/install-pdm.py -UseBasicParsing).Content | python -
 ```
 
 For security reasons, you should verify the checksum of `install-pdm.py`.
-The sha256 checksum is: `965900c551b4d1ba5127ecf95c127c99b5a1cccef4c183a5ecf447e876fa3160`
+It can be downloaded from [install-pdm.py.sha256](https://pdm.fming.dev/dev/install-pdm.py.sha256).
 
 The installer will install PDM into the user site and the location depends on the system:
 
 - `$HOME/.local/bin` for Unix
 - `%APPDATA%\Python\Scripts` on Windows
 
 You can pass additional options to the script to control how PDM is installed:
```

#### html2text {}

```diff
@@ -52,25 +52,24 @@
 `pyproject.toml` file and supports lockfiles. Users can add additional
 functionality through plugins, which can be shared by uploading them as
 distributions. Unlike Poetry and Hatch, PDM is not limited to a specific build
 backend; users have the freedom to choose any build backend they prefer. ##
 Installation PDM requires python version 3.7 or higher. ### Via Install Script
 Like Pip, PDM provides an installation script that will install PDM into an
 isolated environment. **For Linux/Mac** ```bash curl -sSL https://
-raw.githubusercontent.com/pdm-project/pdm/main/install-pdm.py | python3 - ```
-**For Windows** ```powershell (Invoke-WebRequest -Uri https://
-raw.githubusercontent.com/pdm-project/pdm/main/install-pdm.py -
+pdm.fming.dev/dev/install-pdm.py | python3 - ``` **For Windows** ```powershell
+(Invoke-WebRequest -Uri https://pdm.fming.dev/dev/install-pdm.py -
 UseBasicParsing).Content | python - ``` For security reasons, you should verify
-the checksum of `install-pdm.py`. The sha256 checksum is:
-`965900c551b4d1ba5127ecf95c127c99b5a1cccef4c183a5ecf447e876fa3160` The
-installer will install PDM into the user site and the location depends on the
-system: - `$HOME/.local/bin` for Unix - `%APPDATA%\Python\Scripts` on Windows
-You can pass additional options to the script to control how PDM is installed:
-``` usage: install-pdm.py [-h] [-v VERSION] [--prerelease] [--remove] [-p PATH]
-[-d DEP] optional arguments: -h, --help show this help message and exit -
+the checksum of `install-pdm.py`. It can be downloaded from [install-
+pdm.py.sha256](https://pdm.fming.dev/dev/install-pdm.py.sha256). The installer
+will install PDM into the user site and the location depends on the system: -
+`$HOME/.local/bin` for Unix - `%APPDATA%\Python\Scripts` on Windows You can
+pass additional options to the script to control how PDM is installed: ```
+usage: install-pdm.py [-h] [-v VERSION] [--prerelease] [--remove] [-p PATH] [-
+d DEP] optional arguments: -h, --help show this help message and exit -
 v VERSION, --version VERSION | envvar: PDM_VERSION Specify the version to be
 installed, or HEAD to install from the main branch --prerelease | envvar:
 PDM_PRERELEASE Allow prereleases to be installed --remove | envvar: PDM_REMOVE
 Remove the PDM installation -p PATH, --path PATH | envvar: PDM_HOME Specify the
 location to install PDM -d DEP, --dep DEP | envvar: PDM_DEPS Specify additional
 dependencies, can be given multiple times ``` You can either pass the options
 after the script or set the env var value. ### Alternative Installation Methods
```

### Comparing `pdm-2.7.4/pyproject.toml` & `pdm-2.8.0a0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,15 @@
     "tomlkit>=0.11.1,<1",
     "shellingham>=1.3.2",
     "python-dotenv>=0.15",
     "resolvelib>=1.0.1",
     "installer<0.8,>=0.7",
     "cachecontrol[filecache]>=0.13.0",
     "tomli>=1.1.0; python_version < \"3.11\"",
+    "importlib-resources>=5; python_version < \"3.9\"",
     "importlib-metadata>=3.6; python_version < \"3.10\"",
 ]
 readme = "README.md"
 keywords = [
     "packaging",
     "dependency",
     "workflow",
@@ -37,15 +38,15 @@
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
-version = "2.7.4"
+version = "2.8.0a0"
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 Homepage = "https://pdm.fming.dev"
 Repository = "https://github.com/pdm-project/pdm"
```

### Comparing `pdm-2.7.4/src/pdm/_types.py` & `pdm-2.8.0a0/src/pdm/_types.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.4/src/pdm/builders/base.py` & `pdm-2.8.0a0/src/pdm/builders/base.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.4/src/pdm/builders/editable.py` & `pdm-2.8.0a0/src/pdm/builders/editable.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.4/src/pdm/builders/sdist.py` & `pdm-2.8.0a0/src/pdm/builders/sdist.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.4/src/pdm/builders/wheel.py` & `pdm-2.8.0a0/src/pdm/builders/wheel.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.4/src/pdm/cli/actions.py` & `pdm-2.8.0a0/src/pdm/cli/actions.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import datetime
 import hashlib
 import json
 import os
 import sys
 import textwrap
 import warnings
-from typing import Collection, Iterable, cast
+from typing import Any, Collection, Iterable, cast
 
 from resolvelib.reporters import BaseReporter
 from resolvelib.resolvers import ResolutionImpossible, ResolutionTooDeep, Resolver
 
 from pdm import termui
 from pdm.cli.filters import GroupSelection
 from pdm.cli.hooks import HookManager
@@ -27,14 +27,15 @@
 )
 from pdm.environments import BareEnvironment
 from pdm.exceptions import PdmUsageError, ProjectError
 from pdm.models.candidates import Candidate
 from pdm.models.requirements import Requirement, parse_requirement
 from pdm.project import Project
 from pdm.resolver import resolve
+from pdm.utils import deprecation_warning
 
 
 def do_lock(
     project: Project,
     strategy: str = "all",
     tracked_names: Iterable[str] | None = None,
     requirements: list[Requirement] | None = None,
@@ -347,7 +348,58 @@
         " is available.\n",
         f"Please run [req]`{install_command}`[/]",
         " to upgrade.\n",
         f"Run [req]`{disable_command}`[/]",
         " to disable the check.",
     ]
     project.core.ui.echo("".join(message), err=True, style="info")
+
+
+# Moved functions
+def do_add(*args: Any, **kwargs: Any) -> None:  # pragma: no cover
+    from pdm.cli.commands.add import Command as AddCommand
+
+    deprecation_warning(
+        "`pdm.actions.do_add` has been moved to `pdm.cli.commands.add:Command.do_add` method, "
+        "This function will be removed in the future."
+    )
+    AddCommand().do_add(*args, **kwargs)
+
+
+def do_update(*args: Any, **kwargs: Any) -> None:  # pragma: no cover
+    from pdm.cli.commands.update import Command as UpdateCommand
+
+    deprecation_warning(
+        "`pdm.actions.do_update` has been moved to `pdm.cli.commands.update:Command.do_update` method, "
+        "This function will be removed in the future."
+    )
+    UpdateCommand().do_update(*args, **kwargs)
+
+
+def do_use(*args: Any, **kwargs: Any) -> None:  # pragma: no cover
+    from pdm.cli.commands.use import Command as UseCommand
+
+    deprecation_warning(
+        "`pdm.actions.do_use` has been moved to `pdm.cli.commands.use:Command.do_use` method, "
+        "This function will be removed in the future."
+    )
+    UseCommand().do_use(*args, **kwargs)
+
+
+def do_remove(*args: Any, **kwargs: Any) -> None:  # pragma: no cover
+    from pdm.cli.commands.remove import Command as RemoveCommand
+
+    deprecation_warning(
+        "`pdm.actions.do_remove` has been moved to `pdm.cli.commands.remove:Command.do_remove` method, "
+        "This function will be removed in the future."
+    )
+    RemoveCommand().do_remove(*args, **kwargs)
+
+
+def do_import(*args: Any, **kwargs: Any) -> None:  # pragma: no cover
+    from pdm.cli.commands.import_cmd import Command as ImportCommand
+
+    deprecation_warning(
+        "`pdm.actions.do_import` has been moved to `pdm.cli.commands.import_:Command.do_import` method, "
+        "This function will be removed in the future."
+    )
+    ImportCommand().do_import(*args, **kwargs)
```

### Comparing `pdm-2.7.4/src/pdm/cli/commands/add.py` & `pdm-2.8.0a0/src/pdm/cli/commands/add.py`

 * *Files 0% similar despite different names*

```diff
@@ -109,15 +109,15 @@
         hooks = hooks or HookManager(project)
         check_project_file(project)
         if editables and no_editable:
             raise PdmUsageError("Cannot use --no-editable with editable packages given.")
         group = selection.one()
         tracked_names: set[str] = set()
         requirements: dict[str, Requirement] = {}
-        lock_groups = [] if project.lockfile.empty() else project.lockfile.groups
+        lock_groups = ["default"] if project.lockfile.empty() else project.lockfile.groups
         if lock_groups is not None and group not in lock_groups:
             project.core.ui.echo(f"Adding group [success]{group}[/] to lockfile", err=True, style="info")
             lock_groups.append(group)
         if (
             group == "default"
             or not selection.dev
             and group not in project.pyproject.settings.get("dev-dependencies", {})
```

### Comparing `pdm-2.7.4/src/pdm/cli/commands/base.py` & `pdm-2.8.0a0/src/pdm/cli/commands/base.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.4/src/pdm/cli/commands/build.py` & `pdm-2.8.0a0/src/pdm/cli/commands/build.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.4/src/pdm/cli/commands/cache.py` & `pdm-2.8.0a0/src/pdm/cli/commands/cache.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.4/src/pdm/cli/commands/completion.py` & `pdm-2.8.0a0/src/pdm/cli/commands/completion.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.4/src/pdm/cli/commands/config.py` & `pdm-2.8.0a0/src/pdm/cli/commands/config.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 import argparse
+import os
+from pathlib import Path
 from typing import Any, Mapping
 
 from pdm import termui
 from pdm._types import RepositoryConfig
 from pdm.cli.commands.base import BaseCommand
+from pdm.exceptions import PdmUsageError
 from pdm.project import Project
 from pdm.project.config import DEFAULT_REPOSITORIES, REPOSITORY, SOURCE, Config
 
 
 class Command(BaseCommand):
     """Display the current configuration"""
 
@@ -17,18 +20,54 @@
         parser.add_argument(
             "-l",
             "--local",
             action="store_true",
             help="Set config in the project's local configuration file",
         )
         parser.add_argument("-d", "--delete", action="store_true", help="Unset a configuration key")
+        parser.add_argument(
+            "-e",
+            "--edit",
+            action="store_true",
+            help="Edit the configuration file in the default editor(defined by EDITOR env var)",
+        )
         parser.add_argument("key", help="Config key", nargs="?")
         parser.add_argument("value", help="Config value", nargs="?")
 
+    @staticmethod
+    def get_editor() -> str:
+        for key in "VISUAL", "EDITOR":
+            rv = os.getenv(key)
+            if rv:
+                return rv
+        if os.name == "nt":
+            return "notepad"
+        for editor in "sensible-editor", "vim", "nano":
+            if os.system(f"which {editor} >/dev/null 2>&1") == 0:
+                return editor
+        return "vi"
+
+    def edit_file(self, path: Path) -> None:
+        import subprocess
+
+        editor = self.get_editor()
+        proc = subprocess.Popen(f'{editor} "{path}"', shell=True)
+
+        if proc.wait() != 0:
+            raise PdmUsageError(f"Editor {editor} exited abnormally")
+
     def handle(self, project: Project, options: argparse.Namespace) -> None:
+        self.ui = project.core.ui
+        if options.edit:
+            if options.key:
+                raise PdmUsageError("Cannot specify an argument when `--edit` is given")
+            if options.delete:
+                raise PdmUsageError("`--delete` doesn't work when `--edit` is given")
+            config = project.project_config if options.local else project.global_config
+            return self.edit_file(config.config_file)
         if options.delete:
             self._delete_config(project, options)
         elif options.value:
             self._set_config(project, options)
         elif options.key:
             self._get_config(project, options)
         else:
@@ -97,15 +136,14 @@
             value = "[i]<hidden>[/]" if key.endswith("password") else config[key]
             self.ui.echo(
                 f"[primary]{canonical_key}[/]{deprecated} = {value}",
                 style=extra_style,
             )
 
     def _list_config(self, project: Project, options: argparse.Namespace) -> None:
-        self.ui = project.core.ui
         assert Config.site is not None
         self.ui.echo(
             f"Site/default configuration ([success]{Config.site.config_file}[/]):",
             style="bold",
         )
         self._show_config(
             Config.get_defaults(),
```

### Comparing `pdm-2.7.4/src/pdm/cli/commands/export.py` & `pdm-2.8.0a0/src/pdm/cli/commands/export.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.4/src/pdm/cli/commands/fix/__init__.py` & `pdm-2.8.0a0/src/pdm/cli/commands/fix/__init__.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.4/src/pdm/cli/commands/fix/fixers.py` & `pdm-2.8.0a0/src/pdm/cli/commands/fix/fixers.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.4/src/pdm/cli/commands/import_cmd.py` & `pdm-2.8.0a0/src/pdm/cli/commands/import_cmd.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.4/src/pdm/cli/commands/info.py` & `pdm-2.8.0a0/src/pdm/cli/commands/info.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.4/src/pdm/cli/commands/init.py` & `pdm-2.8.0a0/src/pdm/cli/commands/init.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from __future__ import annotations
 
 import argparse
-from pathlib import Path
-from typing import TYPE_CHECKING
+from typing import TYPE_CHECKING, Any
 
 from pdm import termui
 from pdm.cli import actions
 from pdm.cli.commands.base import BaseCommand
 from pdm.cli.hooks import HookManager
 from pdm.cli.options import skip_option
+from pdm.cli.templates import ProjectTemplate
 from pdm.models.backends import _BACKENDS, DEFAULT_BACKEND, BuildBackend, get_backend
 from pdm.models.python import PythonInfo
 from pdm.models.specifiers import get_specifier
 from pdm.models.venv import get_venv_python
 from pdm.utils import get_user_email_from_git
 
 if TYPE_CHECKING:
@@ -21,197 +21,164 @@
 
 class Command(BaseCommand):
     """Initialize a pyproject.toml for PDM"""
 
     def __init__(self) -> None:
         self.interactive = True
 
-    @staticmethod
     def do_init(
-        project: Project,
-        name: str = "",
-        version: str = "",
-        description: str = "",
-        license: str = "MIT",
-        author: str = "",
-        email: str = "",
-        python_requires: str = "",
-        build_backend: type[BuildBackend] | None = None,
-        hooks: HookManager | None = None,
+        self, project: Project, metadata: dict[str, Any], hooks: HookManager, options: argparse.Namespace
     ) -> None:
         """Bootstrap the project and create a pyproject.toml"""
+        with ProjectTemplate(options.template) as template:
+            template.generate(project.root, metadata)
+        project.pyproject.reload()
+        hooks.try_emit("post_init")
+
+    def set_interactive(self, value: bool) -> None:
+        self.interactive = value
+
+    def ask(self, question: str, default: str) -> str:
+        if not self.interactive:
+            return default
+        return termui.ask(question, default=default)
+
+    def get_metadata_from_input(self, project: Project, options: argparse.Namespace) -> dict[str, Any]:
         from pdm.formats.base import array_of_inline_tables, make_array, make_inline_table
 
-        hooks = hooks or HookManager(project)
+        is_library = options.lib
+        if not is_library and self.interactive:
+            is_library = termui.confirm(
+                "Is the project a library that is installable?\n"
+                "If yes, we will need to ask a few more questions to include "
+                "the project name and build backend"
+            )
+        build_backend: type[BuildBackend] | None = None
+        if is_library:
+            name = self.ask("Project name", project.root.name)
+            version = self.ask("Project version", "0.1.0")
+            description = self.ask("Project description", "")
+            if options.backend:
+                build_backend = get_backend(options.backend)
+            elif self.interactive:
+                all_backends = list(_BACKENDS)
+                project.core.ui.echo("Which build backend to use?")
+                for i, backend in enumerate(all_backends):
+                    project.core.ui.echo(f"{i}. [success]{backend}[/]")
+                selected_backend = termui.ask(
+                    "Please select",
+                    prompt_type=int,
+                    choices=[str(i) for i in range(len(all_backends))],
+                    show_choices=False,
+                    default=0,
+                )
+                build_backend = get_backend(all_backends[int(selected_backend)])
+            else:
+                build_backend = DEFAULT_BACKEND
+        else:
+            name, version, description = "", "", ""
+        license = self.ask("License(SPDX name)", "MIT")
+
+        git_user, git_email = get_user_email_from_git()
+        author = self.ask("Author name", git_user)
+        email = self.ask("Author email", git_email)
+        python = project.python
+        python_version = f"{python.major}.{python.minor}"
+        python_requires = self.ask("Python requires('*' to allow any)", f">={python_version}")
+
         data = {
             "project": {
                 "name": name,
                 "version": version,
                 "description": description,
                 "authors": array_of_inline_tables([{"name": author, "email": email}]),
                 "license": make_inline_table({"text": license}),
                 "dependencies": make_array([], True),
             },
         }
-        if build_backend is not None:
-            data["build-system"] = build_backend.build_system()
+
         if python_requires and python_requires != "*":
+            get_specifier(python_requires)
             data["project"]["requires-python"] = python_requires
-        if name and version:
-            readme = next(project.root.glob("README*"), None)
-            if readme is None:
-                readme = project.root.joinpath("README.md")
-                readme.write_text(f"# {name}\n\n{description}\n", encoding="utf-8")
-            data["project"]["readme"] = readme.name
-        get_specifier(python_requires)
-        project.pyproject._data.update(data)
-        project.pyproject.write()
-        Command._write_gitignore(project.root.joinpath(".gitignore"))
-        hooks.try_emit("post_init")
-
-    @staticmethod
-    def _write_gitignore(path: Path) -> None:
-        import requests
-
-        url = "https://raw.githubusercontent.com/github/gitignore/master/Python.gitignore"
-        if not path.exists():
-            try:
-                resp = requests.get(url, timeout=5)
-                resp.raise_for_status()
-            except requests.exceptions.RequestException:
-                content = "\n".join(["build/", "dist/", "*.egg-info/", "__pycache__/", "*.py[cod]"]) + "\n"
-            else:
-                content = resp.text
-            content += ".pdm-python\n"
-        else:
-            content = path.read_text(encoding="utf-8")
-            if ".pdm-python" in content:
-                return
-            content += ".pdm-python\n"
-        path.write_text(content, encoding="utf-8")
-
-    def set_interactive(self, value: bool) -> None:
-        self.interactive = value
+        if build_backend is not None:
+            data["build-system"] = build_backend.build_system()
 
-    def ask(self, question: str, default: str) -> str:
-        if not self.interactive:
-            return default
-        return termui.ask(question, default=default)
+        return data
 
     def add_arguments(self, parser: argparse.ArgumentParser) -> None:
         skip_option.add_to_parser(parser)
         parser.add_argument(
             "-n",
             "--non-interactive",
             action="store_true",
             help="Don't ask questions but use default values",
         )
         parser.add_argument("--python", help="Specify the Python version/path to use")
         parser.add_argument("--backend", choices=list(_BACKENDS), help="Specify the build backend")
         parser.add_argument("--lib", action="store_true", help="Create a library project")
+        parser.add_argument(
+            "template", nargs="?", help="Specify the project template, which can be a local path or a Git URL"
+        )
         parser.set_defaults(search_parent=False)
 
-    def handle(self, project: Project, options: argparse.Namespace) -> None:
+    def set_python(self, project: Project, python: str | None, hooks: HookManager) -> None:
         from pdm.cli.commands.use import Command as UseCommand
 
-        hooks = HookManager(project, options.skip)
-        if project.pyproject.exists():
-            project.core.ui.echo("pyproject.toml already exists, update it now.", style="primary")
-        else:
-            project.core.ui.echo("Creating a pyproject.toml for PDM...", style="primary")
-        self.set_interactive(not options.non_interactive)
         do_use = UseCommand().do_use
         if self.interactive:
-            python = do_use(
+            python_info = do_use(
                 project,
-                options.python or "",
-                first=bool(options.python),
+                python or "",
+                first=bool(python),
                 ignore_remembered=True,
                 ignore_requires_python=True,
                 save=False,
                 hooks=hooks,
             )
         else:
-            python = do_use(
+            python_info = do_use(
                 project,
-                options.python or "3",
+                python or "3",
                 first=True,
                 ignore_remembered=True,
                 ignore_requires_python=True,
                 save=False,
                 hooks=hooks,
             )
-        if project.config["python.use_venv"] and python.get_venv() is None:
+        if project.config["python.use_venv"] and python_info.get_venv() is None:
             if not self.interactive or termui.confirm(
-                f"Would you like to create a virtualenv with [success]{python.executable}[/]?",
+                f"Would you like to create a virtualenv with [success]{python_info.executable}[/]?",
                 default=True,
             ):
-                project._python = python
+                project._python = python_info
                 try:
                     path = project._create_virtualenv()
-                    python = PythonInfo.from_path(get_venv_python(path))
+                    python_info = PythonInfo.from_path(get_venv_python(path))
                 except Exception as e:  # pragma: no cover
                     project.core.ui.echo(
                         f"Error occurred when creating virtualenv: {e}\nPlease fix it and create later.",
                         style="error",
                         err=True,
                     )
-        if python.get_venv() is None:
+        if python_info.get_venv() is None:
             project.core.ui.echo(
                 "You are using the PEP 582 mode, no virtualenv is created.\n"
                 "For more info, please visit https://peps.python.org/pep-0582/",
                 style="success",
             )
-        is_library = options.lib
-        if not is_library and self.interactive:
-            is_library = termui.confirm(
-                "Is the project a library that is installable?\n"
-                "If yes, we will need to ask a few more questions to include "
-                "the project name and build backend"
-            )
-        build_backend: type[BuildBackend] | None = None
-        if is_library:
-            name = self.ask("Project name", project.root.name)
-            version = self.ask("Project version", "0.1.0")
-            description = self.ask("Project description", "")
-            if options.backend:
-                build_backend = get_backend(options.backend)
-            elif self.interactive:
-                all_backends = list(_BACKENDS)
-                project.core.ui.echo("Which build backend to use?")
-                for i, backend in enumerate(all_backends):
-                    project.core.ui.echo(f"{i}. [success]{backend}[/]")
-                selected_backend = termui.ask(
-                    "Please select",
-                    prompt_type=int,
-                    choices=[str(i) for i in range(len(all_backends))],
-                    show_choices=False,
-                    default=0,
-                )
-                build_backend = get_backend(all_backends[int(selected_backend)])
-            else:
-                build_backend = DEFAULT_BACKEND
+        project.python = python_info
+
+    def handle(self, project: Project, options: argparse.Namespace) -> None:
+        hooks = HookManager(project, options.skip)
+        if project.pyproject.exists():
+            project.core.ui.echo("pyproject.toml already exists, update it now.", style="primary")
         else:
-            name, version, description = "", "", ""
-        license = self.ask("License(SPDX name)", "MIT")
+            project.core.ui.echo("Creating a pyproject.toml for PDM...", style="primary")
+        self.set_interactive(not options.non_interactive)
 
-        git_user, git_email = get_user_email_from_git()
-        author = self.ask("Author name", git_user)
-        email = self.ask("Author email", git_email)
-        python_version = f"{python.major}.{python.minor}"
-        python_requires = self.ask("Python requires('*' to allow any)", f">={python_version}")
-        project.python = python
+        self.set_python(project, options.python, hooks)
 
-        self.do_init(
-            project,
-            name=name,
-            version=version,
-            description=description,
-            license=license,
-            author=author,
-            email=email,
-            python_requires=python_requires,
-            build_backend=build_backend,
-            hooks=hooks,
-        )
+        metadata = self.get_metadata_from_input(project, options)
+        self.do_init(project, metadata, hooks=hooks, options=options)
+        project.core.ui.echo("Project is initialized successfully", style="primary")
         if self.interactive:
             actions.ask_for_import(project)
```

### Comparing `pdm-2.7.4/src/pdm/cli/commands/install.py` & `pdm-2.8.0a0/src/pdm/cli/commands/install.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.4/src/pdm/cli/commands/list.py` & `pdm-2.8.0a0/src/pdm/cli/commands/list.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.4/src/pdm/cli/commands/lock.py` & `pdm-2.8.0a0/src/pdm/cli/commands/lock.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.4/src/pdm/cli/commands/publish/__init__.py` & `pdm-2.8.0a0/src/pdm/cli/commands/publish/__init__.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.4/src/pdm/cli/commands/publish/package.py` & `pdm-2.8.0a0/src/pdm/cli/commands/publish/package.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 import re
 import subprocess
 from dataclasses import dataclass
 from typing import IO, Any, cast
 
 from pdm.exceptions import PdmUsageError, ProjectError
 from pdm.termui import logger
-from pdm.utils import normalize_name
 
 DIST_EXTENSIONS = {
     ".whl": "bdist_wheel",
     ".tar.bz2": "sdist",
     ".tar.gz": "sdist",
     ".zip": "sdist",
 }
@@ -175,15 +174,15 @@
             ) from None
 
     @property
     def metadata_dict(self) -> dict[str, Any]:
         meta = self.metadata
         data = {
             # identify release
-            "name": normalize_name(meta["Name"]),
+            "name": meta["Name"],
             "version": meta["Version"],
             # file content
             "filetype": self.filetype,
             "pyversion": self.py_version,
             # additional meta-data
             "metadata_version": meta["Metadata-Version"],
             "summary": meta["Summary"],
```

### Comparing `pdm-2.7.4/src/pdm/cli/commands/publish/repository.py` & `pdm-2.8.0a0/src/pdm/cli/commands/publish/repository.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.4/src/pdm/cli/commands/remove.py` & `pdm-2.8.0a0/src/pdm/cli/commands/remove.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.4/src/pdm/cli/commands/run.py` & `pdm-2.8.0a0/src/pdm/cli/commands/run.py`

 * *Files 1% similar despite different names*

```diff
@@ -244,26 +244,26 @@
             code = 0
             for script in value:
                 if should_interpolate:
                     script, _ = interpolate(script, args)
                 split = shlex.split(script)
                 cmd = split[0]
                 subargs = split[1:] + ([] if should_interpolate else args)
-                code = self.run(cmd, subargs, options)
+                code = self.run(cmd, subargs, options, chdir=True)
                 if code != 0:
                     return code
             return code
         return self._run_process(
             args,
             chdir=True,
             shell=shell,
             **exec_opts(self.global_options, options, opts),
         )
 
-    def run(self, command: str, args: list[str], opts: TaskOptions | None = None) -> int:
+    def run(self, command: str, args: list[str], opts: TaskOptions | None = None, chdir: bool = False) -> int:
         if command in self.hooks.skip:
             return 0
         task = self.get_task(command)
         if task is not None:
             self.hooks.try_emit("pre_script", script=command, args=args)
             pre_task = self.get_task(f"pre_{command}")
             if pre_task is not None and self.hooks.should_run(pre_task.name):
@@ -277,14 +277,15 @@
             if post_task is not None and self.hooks.should_run(post_task.name):
                 code = self.run_task(post_task, opts=opts)
             self.hooks.try_emit("post_script", script=command, args=args)
             return code
         else:
             return self._run_process(
                 [command, *args],
+                chdir=chdir,
                 **exec_opts(self.global_options, opts),
             )
 
     def show_list(self) -> None:
         if not self.project.scripts:
             return
         columns = ["Name", "Type", "Description"]
```

### Comparing `pdm-2.7.4/src/pdm/cli/commands/search.py` & `pdm-2.8.0a0/src/pdm/cli/commands/search.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.4/src/pdm/cli/commands/self_cmd.py` & `pdm-2.8.0a0/src/pdm/cli/commands/self_cmd.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,25 +9,26 @@
 from packaging.version import parse
 
 from pdm import termui
 from pdm.cli.actions import get_latest_pdm_version_from_pypi
 from pdm.cli.commands.base import BaseCommand
 from pdm.cli.options import verbose_option
 from pdm.cli.utils import Package, build_dependency_graph
-from pdm.compat import Distribution, importlib_metadata
+from pdm.compat import Distribution
 from pdm.environments import BareEnvironment
 from pdm.models.working_set import WorkingSet
 from pdm.project import Project
 from pdm.utils import is_in_zipapp, normalize_name
 
 PDM_REPO = "https://github.com/pdm-project/pdm"
 
 
 def _get_distributions() -> Iterable[Distribution]:
-    return importlib_metadata.distributions()
+    working_set = WorkingSet()
+    return working_set.values()
 
 
 def list_distributions(plugin_only: bool = False) -> list[Distribution]:
     result: list[Distribution] = []
     for dist in _get_distributions():
         if not plugin_only or any(ep.group in ("pdm", "pdm.plugin") for ep in dist.entry_points):
             result.append(dist)
```

### Comparing `pdm-2.7.4/src/pdm/cli/commands/show.py` & `pdm-2.8.0a0/src/pdm/cli/commands/show.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.4/src/pdm/cli/commands/sync.py` & `pdm-2.8.0a0/src/pdm/cli/commands/sync.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.4/src/pdm/cli/commands/update.py` & `pdm-2.8.0a0/src/pdm/cli/commands/update.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.4/src/pdm/cli/commands/use.py` & `pdm-2.8.0a0/src/pdm/cli/commands/use.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.4/src/pdm/cli/commands/venv/__init__.py` & `pdm-2.8.0a0/src/pdm/cli/commands/venv/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,23 +5,23 @@
 from pdm.cli.commands.base import BaseCommand
 from pdm.cli.commands.venv.activate import ActivateCommand
 from pdm.cli.commands.venv.create import CreateCommand
 from pdm.cli.commands.venv.list import ListCommand
 from pdm.cli.commands.venv.purge import PurgeCommand
 from pdm.cli.commands.venv.remove import RemoveCommand
 from pdm.cli.commands.venv.utils import get_venv_with_name
-from pdm.cli.options import Option
+from pdm.cli.options import project_option
 from pdm.project import Project
 
 
 class Command(BaseCommand):
     """Virtualenv management"""
 
     name = "venv"
-    arguments: list[Option] = []
+    arguments = [project_option]
 
     def add_arguments(self, parser: argparse.ArgumentParser) -> None:
         group = parser.add_mutually_exclusive_group()
         group.add_argument("--path", help="Show the path to the given virtualenv")
         group.add_argument("--python", help="Show the python interpreter path for the given virtualenv")
         subparser = parser.add_subparsers(metavar="venv", title="commands")
         CreateCommand.register_to(subparser, "create")
```

### Comparing `pdm-2.7.4/src/pdm/cli/commands/venv/activate.py` & `pdm-2.8.0a0/src/pdm/cli/commands/venv/activate.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.4/src/pdm/cli/commands/venv/backends.py` & `pdm-2.8.0a0/src/pdm/cli/commands/venv/backends.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.4/src/pdm/cli/commands/venv/create.py` & `pdm-2.8.0a0/src/pdm/cli/commands/venv/create.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.4/src/pdm/cli/commands/venv/list.py` & `pdm-2.8.0a0/src/pdm/cli/commands/venv/list.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.4/src/pdm/cli/commands/venv/purge.py` & `pdm-2.8.0a0/src/pdm/cli/commands/venv/purge.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.4/src/pdm/cli/commands/venv/remove.py` & `pdm-2.8.0a0/src/pdm/cli/commands/venv/remove.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.4/src/pdm/cli/commands/venv/utils.py` & `pdm-2.8.0a0/src/pdm/cli/commands/venv/utils.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.4/src/pdm/cli/completions/pdm.bash` & `pdm-2.8.0a0/src/pdm/cli/completions/pdm.bash`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # BASH completion script for pdm
 # Generated by pycomplete 0.3.2
 
-_pdm_a919b69078acdf0a_complete()
+_pdm_c6f4c6c1a82f2f50_complete()
 {
     local cur script coms opts com
     COMPREPLY=()
     _get_comp_words_by_ref -n : cur words
 
     # for an alias, get the real script behind it
     if [[ $(type -t ${words[0]}) == "alias" ]]; then
@@ -41,15 +41,15 @@
             ;;
 
             (completion)
             opts="--help"
             ;;
 
             (config)
-            opts="--delete --global --help --local --project --verbose"
+            opts="--delete --edit --global --help --local --project --verbose"
             ;;
 
             (export)
             opts="--dev --expandvars --format --global --group --help --lockfile --no-default --output --production --project --pyproject --verbose --without-hashes"
             ;;
 
             (fix)
@@ -117,15 +117,15 @@
             ;;
 
             (use)
             opts="--first --global --help --ignore-remembered --project --skip --venv --verbose"
             ;;
 
             (venv)
-            opts="--help --path --python"
+            opts="--help --path --project --python"
             ;;
 
         esac
 
         COMPREPLY=($(compgen -W "${opts}" -- ${cur}))
         __ltrim_colon_completions "$cur"
 
@@ -139,8 +139,8 @@
         COMPREPLY=($(compgen -W "${coms}" -- ${cur}))
         __ltrim_colon_completions "$cur"
 
         return 0
     fi
 }
 
-complete -o default -F _pdm_a919b69078acdf0a_complete pdm
+complete -o default -F _pdm_c6f4c6c1a82f2f50_complete pdm
```

### Comparing `pdm-2.7.4/src/pdm/cli/completions/pdm.ps1` & `pdm-2.8.0a0/src/pdm/cli/completions/pdm.ps1`

 * *Files 0% similar despite different names*

```diff
@@ -237,15 +237,15 @@
                         $completer.AddParams(@("clear", "remove", "info", "list"), $false)
                     }
                 }
                 break
             }
             "completion" { $completer.AddParams(@("powershell", "bash", "zsh", "fish")); break }
             "config" {
-                $completer.AddOpts(@([Option]::new(@("--delete", "--global", "--local", "-d", "-l", "-g")), $projectOption))
+                $completer.AddOpts(@([Option]::new(@("--delete", "--global", "--local", "--edit", "-e", "-d", "-l", "-g")), $projectOption))
                 $completer.AddParams(@(getConfigKeys), $false)
                 break
             }
             "export" {
                 $completer.AddOpts(@(
                         [Option]::new(@("--dev", "--output", "--global", "--no-default", "--expandvars", "--prod", "--production", "-g", "-d", "-o", "--without-hashes", "-L", "--lockfile")),
                         $formatOption,
```

### Comparing `pdm-2.7.4/src/pdm/cli/completions/pdm.zsh` & `pdm-2.8.0a0/src/pdm/cli/completions/pdm.zsh`

 * *Files 1% similar despite different names*

```diff
@@ -124,14 +124,15 @@
       return $ret
       ;;
     config)
       _arguments -s  \
          {-g,--global}'[Use the global project, supply the project root with `-p` option]' \
          {-l,--local}"[Set config in the project's local configuration file]" \
          {-d,--delete}'[Unset a configuration key]' \
+         {-e,--edit}'[Edit the configuration file in the default editor(defined by EDITOR env var)]' \
          '1:key:->keys' \
          '2:value:_files' && return 0
       if [[ $state == keys ]]; then
         local l mbegin mend match keys=()
         for l in ${(f)"$(command ${PDM_PYTHON} -m pdm config)"}; do
           if [[ $l == (#b)" "#(*)" = "(*) ]]; then
             keys+=("$match[1]:$match[2]")
@@ -183,14 +184,15 @@
       arguments+=(
         {-g,--global}'[Use the global project, supply the project root with `-p` option]'
         {-n,--non-interactive}"[Don't ask questions but use default values]"
         {-k,--skip}'[Skip some tasks and/or hooks by their comma-separated names]'
         '--backend[Specify the build backend]:backend:(pdm-backend setuptools hatchling flit pdm-pep517)'
         '--lib[Create a library project]'
         '--python[Specify the Python version/path to use]:python:'
+        '1:filename:_files'
       )
       ;;
     install)
       arguments+=(
         {-g,--global}'[Use the global project, supply the project root with `-p` option]'
         {-G+,--group+}'[Select group of optional-dependencies or dev-dependencies(with -d). Can be supplied multiple times, use ":all" to include all groups under the same species]:group:_pdm_groups'
         {-d,--dev}"[Select dev dependencies]"
```

### Comparing `pdm-2.7.4/src/pdm/cli/filters.py` & `pdm-2.8.0a0/src/pdm/cli/filters.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.4/src/pdm/cli/hooks.py` & `pdm-2.8.0a0/src/pdm/cli/hooks.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.4/src/pdm/cli/options.py` & `pdm-2.8.0a0/src/pdm/cli/options.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.4/src/pdm/cli/utils.py` & `pdm-2.8.0a0/src/pdm/cli/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -597,25 +597,25 @@
         "To fix this, you could loosen the dependency version constraints in "
         "pyproject.toml. See https://pdm.fming.dev/latest/usage/dependency/"
         "#solve-the-locking-failure for more details."
     )
     return "\n".join(result)
 
 
-def merge_dictionary(target: MutableMapping[Any, Any], input: Mapping[Any, Any]) -> None:
+def merge_dictionary(target: MutableMapping[Any, Any], input: Mapping[Any, Any], append_array: bool = True) -> None:
     """Merge the input dict with the target while preserving the existing values
     properly. This will update the target dictionary in place.
     List values will be extended, but only if the value is not already in the list.
     """
     for key, value in input.items():
         if key not in target:
             target[key] = value
         elif isinstance(value, dict):
-            merge_dictionary(target[key], value)
-        elif isinstance(value, list):
+            merge_dictionary(target[key], value, append_array=append_array)
+        elif isinstance(value, list) and append_array:
             target[key].extend(x for x in value if x not in target[key])
             if hasattr(target[key], "multiline"):
                 target[key].multiline(True)  # type: ignore[attr-defined]
         else:
             target[key] = value
```

### Comparing `pdm-2.7.4/src/pdm/compat.py` & `pdm-2.8.0a0/src/pdm/compat.py`

 * *Files 3% similar despite different names*

```diff
@@ -63,11 +63,17 @@
 
 if sys.version_info >= (3, 10):
     import importlib.metadata as importlib_metadata
 else:
     import importlib_metadata
 
 
+if sys.version_info >= (3, 9):
+    import importlib.resources as importlib_resources
+else:
+    import importlib_resources
+
+
 Distribution = importlib_metadata.Distribution
 
 
-__all__ = ["tomllib", "cached_property", "importlib_metadata", "Distribution"]
+__all__ = ["tomllib", "cached_property", "importlib_metadata", "Distribution", "importlib_resources"]
```

### Comparing `pdm-2.7.4/src/pdm/core.py` & `pdm-2.8.0a0/src/pdm/core.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.4/src/pdm/environments/__init__.py` & `pdm-2.8.0a0/src/pdm/environments/__init__.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.4/src/pdm/environments/base.py` & `pdm-2.8.0a0/src/pdm/environments/base.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.4/src/pdm/environments/local.py` & `pdm-2.8.0a0/src/pdm/environments/local.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,55 +1,79 @@
 from __future__ import annotations
 
 import os
 import re
 import shlex
 from pathlib import Path
-from typing import TYPE_CHECKING
 
 from pdm.compat import cached_property
 from pdm.environments.base import BaseEnvironment
 from pdm.utils import pdm_scheme
 
-if TYPE_CHECKING:
-    pass
-
 
 def _get_shebang_path(executable: str, is_launcher: bool) -> bytes:
     """Get the interpreter path in the shebang line
 
     The launcher can just use the command as-is.
     Otherwise if the path contains whitespace or is too long, both distlib
     and installer use a clever hack to make the shebang after ``/bin/sh``,
     where the interpreter path is quoted.
     """
     if is_launcher or " " not in executable and (len(executable) + 3) <= 127:
         return executable.encode("utf-8")
     return shlex.quote(executable).encode("utf-8")
 
 
+def _is_console_script(content: bytes) -> bool:
+    import io
+    import zipfile
+
+    if os.name == "nt":  # Windows .exe should be a zip file.
+        try:
+            with zipfile.ZipFile(io.BytesIO(content)) as zf:
+                return zf.namelist() == ["__main__.py"]
+        except zipfile.BadZipFile:
+            return False
+
+    try:
+        text = content.decode("utf-8")
+        return text.startswith("#!")
+    except UnicodeDecodeError:
+        return False
+
+
 def _replace_shebang(path: Path, new_executable: bytes) -> None:
     """Replace the python executable from the shebeng line, which can be in two forms:
 
     1. #!python_executable
     2. #!/bin/sh
        '''exec' '/path to/python' "$0" "$@"
        ' '''
     """
-    _complex_shebang_re = rb"^'''exec' ('.+?') \"\$0\""
-    _simple_shebang_re = rb"^#!(.+?)\s*$"
+    _complex_shebang_re = rb"^(#!/bin/sh\n'''exec' )('.+?')( \"\$0\")"
+    _simple_shebang_re = rb"^(#!)(.+?)\s*(?=\n)"
     contents = path.read_bytes()
-    match = re.search(_complex_shebang_re, contents, flags=re.M)
-    if match:
-        path.write_bytes(contents.replace(match.group(1), new_executable, 1))
+
+    if not _is_console_script(contents):
+        return
+
+    if os.name == "nt":
+        new_content, count = re.subn(_simple_shebang_re, rb"\1" + new_executable, contents, 1, flags=re.M)
+        if count > 0:
+            path.write_bytes(new_content)
+        return
+
+    new_content, count = re.subn(_complex_shebang_re, rb"\1" + new_executable + rb"\3", contents, 1)
+    if count > 0:
+        path.write_bytes(new_content)
         return
 
-    match = re.search(_simple_shebang_re, contents, flags=re.M)
-    if match:
-        path.write_bytes(contents.replace(match.group(1), new_executable, 1))
+    new_content, count = re.subn(_simple_shebang_re, rb"\1" + new_executable, contents, 1)
+    if count > 0:
+        path.write_bytes(new_content)
 
 
 class PythonLocalEnvironment(BaseEnvironment):
     """A project environment that installs packages into
     the local `__pypackages__` directory(PEP 582).
     """
```

### Comparing `pdm-2.7.4/src/pdm/environments/python.py` & `pdm-2.8.0a0/src/pdm/environments/python.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.4/src/pdm/exceptions.py` & `pdm-2.8.0a0/src/pdm/exceptions.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.4/src/pdm/formats/__init__.py` & `pdm-2.8.0a0/src/pdm/formats/__init__.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.4/src/pdm/formats/base.py` & `pdm-2.8.0a0/src/pdm/formats/base.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.4/src/pdm/formats/flit.py` & `pdm-2.8.0a0/src/pdm/formats/flit.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.4/src/pdm/formats/pipfile.py` & `pdm-2.8.0a0/src/pdm/formats/pipfile.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,66 +6,71 @@
 from typing import TYPE_CHECKING, Any
 
 from packaging.markers import default_environment
 
 from pdm.compat import tomllib
 from pdm.formats.base import make_array
 from pdm.models.markers import Marker
-from pdm.models.requirements import Requirement
+from pdm.models.requirements import FileRequirement, Requirement
 
 if TYPE_CHECKING:
     from argparse import Namespace
     from os import PathLike
 
     from pdm._types import RequirementDict
+    from pdm.models.backends import BuildBackend
     from pdm.project import Project
 
 MARKER_KEYS = list(default_environment().keys())
 
 
-def convert_pipfile_requirement(name: str, req: RequirementDict) -> str:
+def convert_pipfile_requirement(name: str, req: RequirementDict, backend: BuildBackend) -> str:
     if isinstance(req, dict):
         markers: list[Marker] = []
         if "markers" in req:
             markers.append(Marker(req["markers"]))  # type: ignore[arg-type]
         for key in MARKER_KEYS:
             if key in req:
                 marker = Marker(f"{key}{req[key]}")
                 markers.append(marker)
                 del req[key]
 
         if markers:
             marker = functools.reduce(operator.and_, markers)
             req["marker"] = str(marker).replace('"', "'")
-    return Requirement.from_req_dict(name, req).as_line()
+    r = Requirement.from_req_dict(name, req)
+    if isinstance(r, FileRequirement):
+        r.relocate(backend)
+    return r.as_line()
 
 
 def check_fingerprint(project: Project, filename: PathLike) -> bool:
     return os.path.basename(filename) == "Pipfile"
 
 
 def convert(project: Project, filename: PathLike, options: Namespace | None) -> tuple[dict[str, Any], dict[str, Any]]:
     with open(filename, "rb") as fp:
         data = tomllib.load(fp)
     result = {}
     settings = {}
+    backend = project.backend
     if "pipenv" in data:
         settings["allow_prereleases"] = data["pipenv"].get("allow_prereleases", False)
     if "requires" in data:
         python_version = data["requires"].get("python_full_version") or data["requires"].get("python_version")
         result["requires-python"] = f">={python_version}"
     if "source" in data:
         settings["source"] = data["source"]
     result["dependencies"] = make_array(  # type: ignore[assignment]
-        [convert_pipfile_requirement(k, req) for k, req in data.get("packages", {}).items()],
+        [convert_pipfile_requirement(k, req, backend) for k, req in data.get("packages", {}).items()],
         True,
     )
     settings["dev-dependencies"] = {
         "dev": make_array(
-            [convert_pipfile_requirement(k, req) for k, req in data.get("dev-packages", {}).items()],
+            [convert_pipfile_requirement(k, req, backend) for k, req in data.get("dev-packages", {}).items()],
             True,
         )
     }
     return result, settings
 
 
 def export(project: Project, candidates: list, options: Any) -> None:
```

### Comparing `pdm-2.7.4/src/pdm/formats/poetry.py` & `pdm-2.8.0a0/src/pdm/formats/poetry.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.4/src/pdm/formats/requirements.py` & `pdm-2.8.0a0/src/pdm/formats/requirements.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.4/src/pdm/formats/setup_py.py` & `pdm-2.8.0a0/src/pdm/formats/setup_py.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.4/src/pdm/installers/core.py` & `pdm-2.8.0a0/src/pdm/installers/core.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.4/src/pdm/installers/installers.py` & `pdm-2.8.0a0/src/pdm/installers/installers.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.4/src/pdm/installers/manager.py` & `pdm-2.8.0a0/src/pdm/installers/manager.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.4/src/pdm/installers/packages.py` & `pdm-2.8.0a0/src/pdm/installers/packages.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.4/src/pdm/installers/synchronizers.py` & `pdm-2.8.0a0/src/pdm/installers/synchronizers.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.4/src/pdm/installers/uninstallers.py` & `pdm-2.8.0a0/src/pdm/installers/uninstallers.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.4/src/pdm/models/auth.py` & `pdm-2.8.0a0/src/pdm/models/auth.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.4/src/pdm/models/backends.py` & `pdm-2.8.0a0/src/pdm/models/backends.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.4/src/pdm/models/caches.py` & `pdm-2.8.0a0/src/pdm/models/caches.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from functools import lru_cache
 from pathlib import Path
 from typing import TYPE_CHECKING, BinaryIO, Generic, Iterable, TypeVar, cast
 
 from cachecontrol.cache import SeparateBodyBaseCache
 from cachecontrol.caches import FileCache
 from packaging.utils import canonicalize_name, parse_wheel_filename
+
 from pdm._types import CandidateInfo
 from pdm.exceptions import PdmException
 from pdm.models.candidates import Candidate
 from pdm.termui import logger
 from pdm.utils import atomic_open_for_write, create_tracked_tempdir
 
 if TYPE_CHECKING:
@@ -124,29 +125,35 @@
     def _get_file_hash(self, link: Link, session: Session) -> str:
         h = hashlib.new(self.FAVORITE_HASH)
         logger.debug("Downloading link %s for calculating hash", link.redacted)
         for chunk in self._read_from_link(link, session):
             h.update(chunk)
         return ":".join([h.name, h.hexdigest()])
 
+    def _should_cache(self, link: Link) -> bool:
+        # For now, we only disable caching for local files.
+        # We may add more when we know better about it.
+        return not link.is_file
+
     def get_hash(self, link: Link, session: Session) -> str:
         # If there is no link hash (i.e., md5, sha256, etc.), we don't want
         # to store it.
         hash_value = self.get(link.url_without_fragment)
         if not hash_value:
             if link.hashes and link.hashes.keys() & self.STRONG_HASHES:
                 logger.debug("Using hash in link for %s", link.redacted)
                 hash_name = next(k for k in self.STRONG_HASHES if k in link.hashes)
                 hash_value = f"{hash_name}:{link.hashes[hash_name]}"
             elif link.hash and link.hash_name in self.STRONG_HASHES:
                 logger.debug("Using hash in link for %s", link.redacted)
                 hash_value = f"{link.hash_name}:{link.hash}"
             else:
                 hash_value = self._get_file_hash(link, session)
-            self.set(link.url_without_fragment, hash_value)
+            if self._should_cache(link):
+                self.set(link.url_without_fragment, hash_value)
         return hash_value
 
     def _get_path_for_key(self, key: str) -> Path:
         hashed = hashlib.sha224(key.encode("utf-8")).hexdigest()
         parts = (hashed[:2], hashed[2:4], hashed[4:6], hashed[6:8], hashed[8:])
         return self.directory.joinpath(*parts)
```

### Comparing `pdm-2.7.4/src/pdm/models/candidates.py` & `pdm-2.8.0a0/src/pdm/models/candidates.py`

 * *Files 1% similar despite different names*

```diff
@@ -477,15 +477,15 @@
         self, link: Link, medata_hash: bool | dict[str, str] | None
     ) -> im.Distribution | None:
         with self.environment.get_finder() as finder:
             resp = finder.session.get(link.normalized, headers={"Cache-Control": "max-age=0"})
             if isinstance(medata_hash, dict):
                 hash_name, hash_value = next(iter(medata_hash.items()))
                 if hashlib.new(hash_name, resp.content).hexdigest() != hash_value:
-                    termui.logger.warn("Metadata hash mismatch for %s, ignoring the metadata", link)
+                    termui.logger.warning("Metadata hash mismatch for %s, ignoring the metadata", link)
                     return None
             return MetadataDistribution(resp.text)
 
     def _get_metadata_from_wheel(self, wheel: Path, metadata_parent: str) -> im.Distribution:
         # Get metadata from METADATA inside the wheel
         self._metadata_dir = _get_wheel_metadata_from_wheel(wheel, metadata_parent)
         return im.PathDistribution(Path(self._metadata_dir))
@@ -493,15 +493,15 @@
     def _get_metadata_from_project(self, pyproject_toml: Path) -> im.Distribution | None:
         # Try getting from PEP 621 metadata
         from pdm.project.project_file import PyProject
 
         pyproject = PyProject(pyproject_toml, ui=self.environment.project.core.ui)
         metadata = pyproject.metadata.unwrap()
         if not metadata:
-            termui.logger.warn("Failed to parse pyproject.toml")
+            termui.logger.warning("Failed to parse pyproject.toml")
             return None
 
         dynamic_fields = metadata.get("dynamic", [])
         # Use the parse result only when all are static
         if not set(dynamic_fields).isdisjoint(
             {
                 "name",
@@ -538,20 +538,20 @@
 
     def _get_metadata_from_build(self, source_dir: Path, metadata_parent: str) -> im.Distribution:
         builder = EditableBuilder if self.req.editable else WheelBuilder
         try:
             termui.logger.info("Running PEP 517 backend to get metadata for %s", self.link)
             self._metadata_dir = builder(source_dir, self.environment).prepare_metadata(metadata_parent)
         except BuildError:
-            termui.logger.warn("Failed to build package, try parsing project files.")
+            termui.logger.warning("Failed to build package, try parsing project files.")
             try:
                 setup = Setup.from_directory(source_dir)
             except Exception:
                 message = "Failed to parse the project files, dependencies may be missing"
-                termui.logger.warn(message)
+                termui.logger.warning(message)
                 warnings.warn(message, RuntimeWarning, stacklevel=1)
                 setup = Setup()
             return setup.as_dist()
         else:
             return im.PathDistribution(Path(cast(str, self._metadata_dir)))
 
     @property
```

### Comparing `pdm-2.7.4/src/pdm/models/in_process/__init__.py` & `pdm-2.8.0a0/src/pdm/models/in_process/__init__.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.4/src/pdm/models/in_process/get_abi_tag.py` & `pdm-2.8.0a0/src/pdm/models/in_process/get_abi_tag.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.4/src/pdm/models/in_process/parse_setup.py` & `pdm-2.8.0a0/src/pdm/models/in_process/parse_setup.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.4/src/pdm/models/in_process/pep508.py` & `pdm-2.8.0a0/src/pdm/models/in_process/pep508.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.4/src/pdm/models/in_process/sysconfig_get_paths.py` & `pdm-2.8.0a0/src/pdm/models/in_process/sysconfig_get_paths.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.4/src/pdm/models/markers.py` & `pdm-2.8.0a0/src/pdm/models/markers.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.4/src/pdm/models/project_info.py` & `pdm-2.8.0a0/src/pdm/models/project_info.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.4/src/pdm/models/python.py` & `pdm-2.8.0a0/src/pdm/models/python.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.4/src/pdm/models/repositories.py` & `pdm-2.8.0a0/src/pdm/models/repositories.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.4/src/pdm/models/requirements.py` & `pdm-2.8.0a0/src/pdm/models/requirements.py`

 * *Files 1% similar despite different names*

```diff
@@ -328,15 +328,18 @@
 
     def relocate(self, backend: BuildBackend) -> None:
         """Change the project root to the given path"""
         if self.path is None or self.path.is_absolute():
             return
         # self.path is relative
         self.path = path_without_fragments(os.path.relpath(self.path, backend.root))
-        self.url = backend.relative_path_to_url(self.path.as_posix())
+        path = self.path.as_posix()
+        if path == ".":
+            path = ""
+        self.url = backend.relative_path_to_url(path)
 
     @property
     def is_local(self) -> bool:
         return self.path and self.path.exists() or False
 
     @property
     def is_local_dir(self) -> bool:
```

### Comparing `pdm-2.7.4/src/pdm/models/search.py` & `pdm-2.8.0a0/src/pdm/models/search.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.4/src/pdm/models/setup.py` & `pdm-2.8.0a0/src/pdm/models/setup.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.4/src/pdm/models/specifiers.py` & `pdm-2.8.0a0/src/pdm/models/specifiers.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.4/src/pdm/models/venv.py` & `pdm-2.8.0a0/src/pdm/models/venv.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.4/src/pdm/models/versions.py` & `pdm-2.8.0a0/src/pdm/models/versions.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.4/src/pdm/models/working_set.py` & `pdm-2.8.0a0/src/pdm/models/working_set.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.4/src/pdm/pep582/sitecustomize.py` & `pdm-2.8.0a0/src/pdm/pep582/sitecustomize.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.4/src/pdm/project/config.py` & `pdm-2.8.0a0/src/pdm/project/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -256,15 +256,15 @@
 
     @property
     def self_data(self) -> dict[str, Any]:
         return dict(self._file_data)
 
     def iter_sources(self) -> Iterator[RepositoryConfig]:
         for name, data in self._data.items():
-            if name.startswith(f"{SOURCE}.") and name not in self._config_map:
+            if name.startswith(f"{SOURCE}.") and name not in self._config_map and data:
                 yield RepositoryConfig(**data, name=name[len(SOURCE) + 1 :], config_prefix=SOURCE)
 
     def _save_config(self) -> None:
         """Save the changed to config file."""
         self.config_file.parent.mkdir(parents=True, exist_ok=True)
         toml_data: dict[str, Any] = {}
         for key, value in self._file_data.items():
```

### Comparing `pdm-2.7.4/src/pdm/project/core.py` & `pdm-2.8.0a0/src/pdm/project/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -376,15 +376,15 @@
             if "pypi" not in result:  # put pypi source at the beginning
                 result = {"pypi": self.default_source, **result}
             else:
                 result["pypi"].passive_update(self.default_source)
             merge_sources(self.project_config.iter_sources())
             merge_sources(self.global_config.iter_sources())
         for source in result.values():
-            assert source.url, "Source URL must not be empty"
+            assert source.url, f"Source URL must not be empty for {source.name}"
             source.url = expand_env_vars_in_auth(source.url)
         return list(result.values())
 
     def get_repository(
         self, cls: type[BaseRepository] | None = None, ignore_compatibility: bool = True
     ) -> BaseRepository:
         """Get the repository object"""
```

### Comparing `pdm-2.7.4/src/pdm/project/lockfile.py` & `pdm-2.8.0a0/src/pdm/project/lockfile.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.4/src/pdm/project/project_file.py` & `pdm-2.8.0a0/src/pdm/project/project_file.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.4/src/pdm/project/toml_file.py` & `pdm-2.8.0a0/src/pdm/project/toml_file.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.4/src/pdm/pytest.py` & `pdm-2.8.0a0/src/pdm/pytest.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 from __future__ import annotations
 
 import collections
 import json
 import os
 import shutil
 import sys
+from argparse import Namespace
 from dataclasses import dataclass
 from io import BufferedReader, BytesIO, StringIO
 from pathlib import Path
 from typing import (
     TYPE_CHECKING,
     Any,
     BinaryIO,
@@ -50,15 +51,15 @@
 from unearth import Link
 
 from pdm.cli.hooks import HookManager
 from pdm.core import Core
 from pdm.environments import BaseEnvironment, PythonEnvironment
 from pdm.exceptions import CandidateInfoNotFound
 from pdm.installers.installers import install_wheel
-from pdm.models.backends import get_backend
+from pdm.models.backends import DEFAULT_BACKEND
 from pdm.models.candidates import Candidate
 from pdm.models.repositories import BaseRepository
 from pdm.models.requirements import (
     Requirement,
     filter_requirements_with_extras,
     parse_requirement,
 )
@@ -418,21 +419,28 @@
 
     Returns:
         The initialized project
     """
     from pdm.cli.commands.init import Command
 
     hooks = HookManager(project_no_init, ["post_init"])
-    Command.do_init(
-        project_no_init,
-        "test_project",
-        "0.0.0",
-        hooks=hooks,
-        build_backend=get_backend("pdm-pep517"),
-    )
+    data = {
+        "project": {
+            "name": "test-project",
+            "version": "0.0.0",
+            "description": "",
+            "authors": [],
+            "license": {"text": "MIT"},
+            "dependencies": [],
+            "requires-python": ">=3.7",
+        },
+        "build-system": DEFAULT_BACKEND.build_system(),
+    }
+
+    Command().do_init(project_no_init, data, hooks=hooks, options=Namespace(template=None))
     # Clean the cached property
     project_no_init._environment = None
     return project_no_init
 
 
 @pytest.fixture
 def working_set(mocker: MockerFixture, repository: TestRepository) -> MockWorkingSet:
@@ -579,15 +587,15 @@
             """
             ...
 
 
 @pytest.fixture
 def pdm(core: Core, monkeypatch: pytest.MonkeyPatch) -> PDMCallable:
     """
-    A fixture alloowing to execute PDM commands
+    A fixture allowing to execute PDM commands
 
     Returns:
         A `pdm` fixture command.
     """
     # Hide the spinner text from testing output to not break existing tests
     monkeypatch.setattr("pdm.termui.DummySpinner._show", lambda self: None)
```

### Comparing `pdm-2.7.4/src/pdm/resolver/core.py` & `pdm-2.8.0a0/src/pdm/resolver/core.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.4/src/pdm/resolver/providers.py` & `pdm-2.8.0a0/src/pdm/resolver/providers.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,19 +46,20 @@
 
         - Editable requirements are preferered.
         - File links are preferred.
         - The one with narrower specifierset is preferred.
         """
         editable = requirement.editable
         is_named = requirement.is_named
+        is_pinned = requirement.is_pinned
         is_prerelease = (
             requirement.prerelease or requirement.specifier is not None and bool(requirement.specifier.prereleases)
         )
         specifier_parts = len(requirement.specifier) if requirement.specifier else 0
-        return (not editable, is_named, not is_prerelease, -specifier_parts)
+        return (not editable, is_named, not is_pinned, not is_prerelease, -specifier_parts)
 
     def identify(self, requirement_or_candidate: Requirement | Candidate) -> str:
         return requirement_or_candidate.identify()
 
     def get_preference(
         self,
         identifier: str,
```

### Comparing `pdm-2.7.4/src/pdm/resolver/python.py` & `pdm-2.8.0a0/src/pdm/resolver/python.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.4/src/pdm/resolver/reporters.py` & `pdm-2.8.0a0/src/pdm/resolver/reporters.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.4/src/pdm/signals.py` & `pdm-2.8.0a0/src/pdm/signals.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.4/src/pdm/termui.py` & `pdm-2.8.0a0/src/pdm/termui.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.4/src/pdm/utils.py` & `pdm-2.8.0a0/src/pdm/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -409,16 +409,16 @@
     """Show a deprecation warning with the given message and raise an error
     after a specified version.
     """
     from pdm.__version__ import __version__
 
     if raise_since is not None:
         if Version(__version__) >= Version(raise_since):
-            raise DeprecationWarning(message)
-    warnings.warn(message, DeprecationWarning, stacklevel=stacklevel + 1)
+            raise FutureWarning(message)
+    warnings.warn(message, FutureWarning, stacklevel=stacklevel + 1)
 
 
 def is_pip_compatible_with_python(python_version: Version | str) -> bool:
     """Check the given python version is compatible with the pip installed"""
     from pdm.compat import importlib_metadata
     from pdm.models.specifiers import get_specifier
```

### Comparing `pdm-2.7.4/tests/cli/conftest.py` & `pdm-2.8.0a0/tests/cli/conftest.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.4/tests/cli/test_add.py` & `pdm-2.8.0a0/tests/cli/test_add.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.4/tests/cli/test_build.py` & `pdm-2.8.0a0/tests/cli/test_build.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,21 +59,21 @@
     assert "demo-module-0.1.0/README.md" in get_tarball_names(project.root / "dist/demo-module-0.1.0.tar.gz")
 
 
 def test_build_package(fixture_project):
     project = fixture_project("demo-package")
     Command.do_build(project)
 
-    tar_names = get_tarball_names(project.root / "dist/demo-package-0.1.0.tar.gz")
-    assert "demo-package-0.1.0/my_package/__init__.py" in tar_names
-    assert "demo-package-0.1.0/my_package/data.json" in tar_names
-    assert "demo-package-0.1.0/single_module.py" not in tar_names
-    assert "demo-package-0.1.0/data_out.json" not in tar_names
+    tar_names = get_tarball_names(project.root / "dist/my-package-0.1.0.tar.gz")
+    assert "my-package-0.1.0/my_package/__init__.py" in tar_names
+    assert "my-package-0.1.0/my_package/data.json" in tar_names
+    assert "my-package-0.1.0/single_module.py" not in tar_names
+    assert "my-package-0.1.0/data_out.json" not in tar_names
 
-    zip_names = get_wheel_names(project.root / "dist/demo_package-0.1.0-py3-none-any.whl")
+    zip_names = get_wheel_names(project.root / "dist/my_package-0.1.0-py3-none-any.whl")
     assert "my_package/__init__.py" in zip_names
     assert "my_package/data.json" in zip_names
     assert "single_module.py" not in zip_names
     assert "data_out.json" not in zip_names
 
 
 def test_build_src_package(fixture_project):
@@ -96,21 +96,21 @@
         "single_module.py",
         "data_out.json",
     ]
     project.pyproject.settings["excludes"] = ["my_package/*.json"]
     project.pyproject.write()
     Command.do_build(project)
 
-    tar_names = get_tarball_names(project.root / "dist/demo-package-0.1.0.tar.gz")
-    assert "demo-package-0.1.0/my_package/__init__.py" in tar_names
-    assert "demo-package-0.1.0/my_package/data.json" not in tar_names
-    assert "demo-package-0.1.0/single_module.py" in tar_names
-    assert "demo-package-0.1.0/data_out.json" in tar_names
+    tar_names = get_tarball_names(project.root / "dist/my-package-0.1.0.tar.gz")
+    assert "my-package-0.1.0/my_package/__init__.py" in tar_names
+    assert "my-package-0.1.0/my_package/data.json" not in tar_names
+    assert "my-package-0.1.0/single_module.py" in tar_names
+    assert "my-package-0.1.0/data_out.json" in tar_names
 
-    zip_names = get_wheel_names(project.root / "dist/demo_package-0.1.0-py3-none-any.whl")
+    zip_names = get_wheel_names(project.root / "dist/my_package-0.1.0-py3-none-any.whl")
     assert "my_package/__init__.py" in zip_names
     assert "my_package/data.json" not in zip_names
     assert "single_module.py" in zip_names
     assert "data_out.json" in zip_names
 
 
 def test_build_src_package_by_include(fixture_project):
```

### Comparing `pdm-2.7.4/tests/cli/test_cache.py` & `pdm-2.8.0a0/tests/cli/test_cache.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.4/tests/cli/test_config.py` & `pdm-2.8.0a0/tests/cli/test_config.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.4/tests/cli/test_fix.py` & `pdm-2.8.0a0/tests/cli/test_fix.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.4/tests/cli/test_hooks.py` & `pdm-2.8.0a0/tests/cli/test_hooks.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.4/tests/cli/test_init.py` & `pdm-2.8.0a0/tests/cli/test_init.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,104 +1,109 @@
 import sys
 from unittest.mock import ANY
 
-import pytest
-
-from pdm.cli.commands.init import Command
-from pdm.models.backends import get_backend
+from pdm.compat import tomllib
 from pdm.models.python import PythonInfo
 
 PYTHON_VERSION = f"{sys.version_info[0]}.{sys.version_info[1]}"
 
 
-def test_init_validate_python_requires(project_no_init):
-    with pytest.raises(ValueError):
-        Command.do_init(project_no_init, python_requires="3.7")
+def test_init_validate_python_requires(project_no_init, pdm):
+    result = pdm(["init"], input="\n\n\n\n\n3.7\n", obj=project_no_init)
+    assert result.exit_code != 0
+    assert "InvalidSpecifier" in result.stderr
 
 
 def test_init_command(project_no_init, pdm, mocker):
     mocker.patch(
         "pdm.cli.commands.init.get_user_email_from_git",
         return_value=("Testing", "me@example.org"),
     )
-    do_init = mocker.patch.object(Command, "do_init")
     pdm(["init"], input="\n\n\n\n\n\n", strict=True, obj=project_no_init)
     python_version = f"{project_no_init.python.major}.{project_no_init.python.minor}"
-    do_init.assert_called_with(
-        project_no_init,
-        name="",
-        version="",
-        description="",
-        license="MIT",
-        author="Testing",
-        email="me@example.org",
-        python_requires=f">={python_version}",
-        build_backend=None,
-        hooks=ANY,
-    )
+    data = {
+        "project": {
+            "authors": [{"email": "me@example.org", "name": "Testing"}],
+            "dependencies": [],
+            "description": "",
+            "license": {"text": "MIT"},
+            "name": "",
+            "requires-python": f">={python_version}",
+            "readme": "README.md",
+            "version": "",
+        },
+    }
+
+    with open(project_no_init.root.joinpath("pyproject.toml"), "rb") as fp:
+        assert tomllib.load(fp) == data
 
 
 def test_init_command_library(project_no_init, pdm, mocker):
     mocker.patch(
         "pdm.cli.commands.init.get_user_email_from_git",
         return_value=("Testing", "me@example.org"),
     )
-    do_init = mocker.patch.object(Command, "do_init")
     result = pdm(
         ["init"],
         input="\ny\ntest-project\n\nTest Project\n1\n\n\n\n\n",
         obj=project_no_init,
     )
     assert result.exit_code == 0
     python_version = f"{project_no_init.python.major}.{project_no_init.python.minor}"
-    do_init.assert_called_with(
-        project_no_init,
-        name="test-project",
-        version="0.1.0",
-        description="Test Project",
-        license="MIT",
-        author="Testing",
-        email="me@example.org",
-        python_requires=f">={python_version}",
-        build_backend=get_backend("setuptools"),
-        hooks=ANY,
-    )
+    data = {
+        "project": {
+            "authors": [{"email": "me@example.org", "name": "Testing"}],
+            "dependencies": [],
+            "description": "Test Project",
+            "license": {"text": "MIT"},
+            "name": "test-project",
+            "requires-python": f">={python_version}",
+            "readme": "README.md",
+            "version": "0.1.0",
+        },
+        "build-system": {"build-backend": "setuptools.build_meta", "requires": ["setuptools>=61", "wheel"]},
+    }
+
+    with open(project_no_init.root.joinpath("pyproject.toml"), "rb") as fp:
+        assert tomllib.load(fp) == data
 
 
 def test_init_non_interactive(project_no_init, pdm, mocker):
     mocker.patch(
         "pdm.cli.commands.init.get_user_email_from_git",
         return_value=("Testing", "me@example.org"),
     )
-    do_init = mocker.patch.object(Command, "do_init")
     do_use = mocker.patch("pdm.cli.commands.use.Command.do_use", return_value=PythonInfo.from_path(sys.executable))
     result = pdm(["init", "-n"], obj=project_no_init)
     assert result.exit_code == 0
     python_version = f"{project_no_init.python.major}.{project_no_init.python.minor}"
     do_use.assert_called_once_with(
         project_no_init,
         ANY,
         first=True,
         ignore_remembered=True,
         ignore_requires_python=True,
         save=False,
         hooks=ANY,
     )
-    do_init.assert_called_with(
-        project_no_init,
-        name="",
-        version="",
-        description="",
-        license="MIT",
-        author="Testing",
-        email="me@example.org",
-        python_requires=f">={python_version}",
-        build_backend=None,
-        hooks=ANY,
-    )
+    data = {
+        "project": {
+            "authors": [{"email": "me@example.org", "name": "Testing"}],
+            "dependencies": [],
+            "description": "",
+            "license": {"text": "MIT"},
+            "name": "",
+            "requires-python": f">={python_version}",
+            "readme": "README.md",
+            "version": "",
+        },
+    }
+
+    with open(project_no_init.root.joinpath("pyproject.toml"), "rb") as fp:
+        assert tomllib.load(fp) == data
 
 
 def test_init_auto_create_venv(project_no_init, pdm, mocker):
     mocker.patch("pdm.models.python.PythonInfo.get_venv", return_value=None)
     project_no_init.project_config["python.use_venv"] = True
     result = pdm(["init"], input="\n\n\n\n\n\n\n", obj=project_no_init)
     assert result.exit_code == 0
```

### Comparing `pdm-2.7.4/tests/cli/test_install.py` & `pdm-2.8.0a0/tests/cli/test_install.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.4/tests/cli/test_list.py` & `pdm-2.8.0a0/tests/cli/test_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -620,15 +620,15 @@
     assert expected == json.loads(result.outputs)
 
 
 @pytest.mark.usefixtures("fake_working_set")
 def test_list_markdown_fields_licences(project, pdm):
     result = pdm(["list", "--markdown", "--fields", "name,version,licenses"], obj=project)
     expected = (
-        "# test_project licenses\n"
+        "# test-project licenses\n"
         "## foo\n\n"
         "| Name | foo |\n"
         "|----|----|\n"
         "| Version | 0.1.0 |\n"
         "| Licenses | A License |\n\n"
         "foo-0.1.0.dist-info/LICENSE\n\n\n"
         "````\n"
```

### Comparing `pdm-2.7.4/tests/cli/test_lock.py` & `pdm-2.8.0a0/tests/cli/test_lock.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.4/tests/cli/test_others.py` & `pdm-2.8.0a0/tests/cli/test_others.py`

 * *Files 0% similar despite different names*

```diff
@@ -158,15 +158,15 @@
 
 def test_show_self_package(project, pdm):
     result = pdm(["show"], obj=project)
     assert result.exit_code == 0, result.stderr
 
     result = pdm(["show", "--name", "--version"], obj=project)
     assert result.exit_code == 0
-    assert "test_project\n0.0.0\n" == result.output
+    assert "test-project\n0.0.0\n" == result.output
 
 
 def test_export_to_requirements_txt(pdm, fixture_project):
     project = fixture_project("demo-package")
     requirements_txt = project.root / "requirements.txt"
     requirements_no_hashes = project.root / "requirements_simple.txt"
     requirements_pyproject = project.root / "requirements.ini"
```

### Comparing `pdm-2.7.4/tests/cli/test_publish.py` & `pdm-2.8.0a0/tests/cli/test_publish.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.4/tests/cli/test_remove.py` & `pdm-2.8.0a0/tests/cli/test_remove.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.4/tests/cli/test_run.py` & `pdm-2.8.0a0/tests/cli/test_run.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.4/tests/cli/test_self_command.py` & `pdm-2.8.0a0/tests/cli/test_self_command.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.4/tests/cli/test_update.py` & `pdm-2.8.0a0/tests/cli/test_update.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.4/tests/cli/test_use.py` & `pdm-2.8.0a0/tests/cli/test_use.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.4/tests/cli/test_venv.py` & `pdm-2.8.0a0/tests/cli/test_venv.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,14 +47,24 @@
     assert venv_path.exists()
     result = pdm(["venv", "create"], obj=project)
     assert result.exit_code == 1
     assert "is not empty" in result.stderr
 
 
 @pytest.mark.usefixtures("fake_create")
+def test_venv_create_other_location(pdm, project):
+    pdm(["venv", "-p", project.root.as_posix(), "create"], strict=True)
+    venv_path = project.root / ".venv"
+    assert venv_path.exists()
+    result = pdm(["venv", "-p", project.root.as_posix(), "create"])
+    assert result.exit_code == 1
+    assert "is not empty" in result.stderr
+
+
+@pytest.mark.usefixtures("fake_create")
 def test_venv_show_path(pdm, project):
     project.project_config["venv.in_project"] = True
     pdm(["venv", "create"], obj=project, strict=True)
     pdm(["venv", "create", "--name", "test"], obj=project, strict=True)
     result = pdm(["venv", "--path", "in-project"], obj=project, strict=True)
     assert result.output.strip() == str(project.root / ".venv")
     result = pdm(["venv", "--path", "test"], obj=project)
```

### Comparing `pdm-2.7.4/tests/conftest.py` & `pdm-2.8.0a0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.4/tests/fixtures/artifacts/PyFunctional-1.4.3-py3-none-any.whl` & `pdm-2.8.0a0/tests/fixtures/artifacts/PyFunctional-1.4.3-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.7.4/tests/fixtures/artifacts/caj2pdf-restructured-0.1.0a6.tar.gz` & `pdm-2.8.0a0/tests/fixtures/artifacts/caj2pdf-restructured-0.1.0a6.tar.gz`

 * *Files identical despite different names*

### Comparing `pdm-2.7.4/tests/fixtures/artifacts/celery-4.4.2-py2.py3-none-any.whl` & `pdm-2.8.0a0/tests/fixtures/artifacts/celery-4.4.2-py2.py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.7.4/tests/fixtures/artifacts/demo-0.0.1-cp36-cp36m-win_amd64.whl` & `pdm-2.8.0a0/tests/fixtures/artifacts/demo-0.0.1-cp36-cp36m-win_amd64.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.7.4/tests/fixtures/artifacts/demo-0.0.1-py2.py3-none-any.whl` & `pdm-2.8.0a0/tests/fixtures/artifacts/demo-0.0.1-py2.py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.7.4/tests/fixtures/artifacts/demo-0.0.1.tar.gz` & `pdm-2.8.0a0/tests/fixtures/artifacts/demo-0.0.1.tar.gz`

 * *Files identical despite different names*

### Comparing `pdm-2.7.4/tests/fixtures/artifacts/demo-0.0.1.zip` & `pdm-2.8.0a0/tests/fixtures/artifacts/demo-0.0.1.zip`

 * *Files identical despite different names*

### Comparing `pdm-2.7.4/tests/fixtures/artifacts/editables-0.2-py3-none-any.whl` & `pdm-2.8.0a0/tests/fixtures/artifacts/editables-0.2-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.7.4/tests/fixtures/artifacts/first-2.0.2-py2.py3-none-any.whl` & `pdm-2.8.0a0/tests/fixtures/artifacts/first-2.0.2-py2.py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.7.4/tests/fixtures/artifacts/flit_core-3.6.0-py3-none-any.whl` & `pdm-2.8.0a0/tests/fixtures/artifacts/flit_core-3.6.0-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.7.4/tests/fixtures/artifacts/future_fstrings-1.2.0-py2.py3-none-any.whl` & `pdm-2.8.0a0/tests/fixtures/artifacts/future_fstrings-1.2.0-py2.py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.7.4/tests/fixtures/artifacts/future_fstrings-1.2.0.tar.gz` & `pdm-2.8.0a0/tests/fixtures/artifacts/future_fstrings-1.2.0.tar.gz`

 * *Files identical despite different names*

### Comparing `pdm-2.7.4/tests/fixtures/artifacts/importlib_metadata-4.8.3-py3-none-any.whl` & `pdm-2.8.0a0/tests/fixtures/artifacts/importlib_metadata-4.8.3-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.7.4/tests/fixtures/artifacts/jmespath-0.10.0-py2.py3-none-any.whl` & `pdm-2.8.0a0/tests/fixtures/artifacts/jmespath-0.10.0-py2.py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.7.4/tests/fixtures/artifacts/pdm_backend-2.0.2-py3-none-any.whl` & `pdm-2.8.0a0/tests/fixtures/artifacts/pdm_backend-2.0.2-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.7.4/tests/fixtures/artifacts/pdm_hello-0.1.0-py3-none-any.whl` & `pdm-2.8.0a0/tests/fixtures/artifacts/pdm_hello-0.1.0-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.7.4/tests/fixtures/artifacts/pdm_hello-0.1.0-py3-none-win_amd64.whl` & `pdm-2.8.0a0/tests/fixtures/artifacts/pdm_hello-0.1.0-py3-none-win_amd64.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.7.4/tests/fixtures/artifacts/pdm_pep517-1.0.0-py3-none-any.whl` & `pdm-2.8.0a0/tests/fixtures/artifacts/pdm_pep517-1.0.0-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.7.4/tests/fixtures/artifacts/poetry_core-1.3.2-py3-none-any.whl` & `pdm-2.8.0a0/tests/fixtures/artifacts/poetry_core-1.3.2-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.7.4/tests/fixtures/artifacts/setuptools-65.4.1-py3-none-any.whl` & `pdm-2.8.0a0/tests/fixtures/artifacts/setuptools-65.4.1-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.7.4/tests/fixtures/artifacts/typing_extensions-4.4.0-py3-none-any.whl` & `pdm-2.8.0a0/tests/fixtures/artifacts/typing_extensions-4.4.0-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.7.4/tests/fixtures/artifacts/wheel-0.37.1-py2.py3-none-any.whl` & `pdm-2.8.0a0/tests/fixtures/artifacts/wheel-0.37.1-py2.py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.7.4/tests/fixtures/artifacts/zipp-3.7.0-py3-none-any.whl` & `pdm-2.8.0a0/tests/fixtures/artifacts/zipp-3.7.0-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.7.4/tests/fixtures/projects/demo-package-has-dep-with-extras/pdm.lock` & `pdm-2.8.0a0/tests/fixtures/projects/demo-package-has-dep-with-extras/pdm.lock`

 * *Files identical despite different names*

### Comparing `pdm-2.7.4/tests/fixtures/projects/demo-package/pdm.lock` & `pdm-2.8.0a0/tests/fixtures/projects/demo-package/pdm.lock`

 * *Files identical despite different names*

### Comparing `pdm-2.7.4/tests/fixtures/projects/demo-package/pyproject.toml` & `pdm-2.8.0a0/tests/fixtures/projects/demo-package/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     {name = "frostming", email = "mianghong@gmail.com"},
 ]
 dynamic = ["version"]
 requires-python = ">=3.5"
 license = {text = "MIT"}
 dependencies = ["flask"]
 description = ""
-name = "demo-package"
+name = "my-package"
 readme = "README.md"
 
 [project.optional-dependencies]
 
 [tool.pdm]
 version = { from = "my_package/__init__.py" }
```

### Comparing `pdm-2.7.4/tests/fixtures/projects/demo-package/requirements.txt` & `pdm-2.8.0a0/tests/fixtures/projects/demo-package/requirements.txt`

 * *Files identical despite different names*

### Comparing `pdm-2.7.4/tests/fixtures/projects/demo-package/setup.txt` & `pdm-2.8.0a0/tests/fixtures/projects/demo-package/setup.txt`

 * *Files 14% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 with codecs.open('README.md', encoding="utf-8") as fp:
     long_description = fp.read()
 INSTALL_REQUIRES = [
     'flask',
 ]
 
 setup_kwargs = {
-    'name': 'demo-package',
+    'name': 'my-package',
     'version': '0.1.0',
     'description': '',
     'long_description': long_description,
     'license': 'MIT',
     'author': '',
     'author_email': 'frostming <mianghong@gmail.com>',
     'maintainer': None,
```

### Comparing `pdm-2.7.4/tests/fixtures/projects/flit-demo/pyproject.toml` & `pdm-2.8.0a0/tests/fixtures/projects/flit-demo/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pdm-2.7.4/tests/fixtures/projects/poetry-demo/pyproject.toml` & `pdm-2.8.0a0/tests/fixtures/projects/poetry-demo/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pdm-2.7.4/tests/fixtures/pypi.json` & `pdm-2.8.0a0/tests/fixtures/pypi.json`

 * *Files identical despite different names*

### Comparing `pdm-2.7.4/tests/fixtures/pyproject.toml` & `pdm-2.8.0a0/tests/fixtures/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pdm-2.7.4/tests/models/test_backends.py` & `pdm-2.8.0a0/tests/models/test_backends.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.4/tests/models/test_candidates.py` & `pdm-2.8.0a0/tests/models/test_candidates.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.4/tests/models/test_marker.py` & `pdm-2.8.0a0/tests/models/test_marker.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.4/tests/models/test_requirements.py` & `pdm-2.8.0a0/tests/models/test_requirements.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.4/tests/models/test_setup_parsing.py` & `pdm-2.8.0a0/tests/models/test_setup_parsing.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.4/tests/models/test_specifiers.py` & `pdm-2.8.0a0/tests/models/test_specifiers.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.4/tests/models/test_versions.py` & `pdm-2.8.0a0/tests/models/test_versions.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.4/tests/resolver/test_resolve.py` & `pdm-2.8.0a0/tests/resolver/test_resolve.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.4/tests/test_formats.py` & `pdm-2.8.0a0/tests/test_formats.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.4/tests/test_installer.py` & `pdm-2.8.0a0/tests/test_installer.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.4/tests/test_integration.py` & `pdm-2.8.0a0/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.4/tests/test_plugin.py` & `pdm-2.8.0a0/tests/test_plugin.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.4/tests/test_project.py` & `pdm-2.8.0a0/tests/test_project.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.4/tests/test_signals.py` & `pdm-2.8.0a0/tests/test_signals.py`

 * *Files identical despite different names*

### Comparing `pdm-2.7.4/tests/test_utils.py` & `pdm-2.8.0a0/tests/test_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -134,14 +134,14 @@
     setup_dependencies(project)
     selection = GroupSelection(project, default=True, dev=False, groups=["test"])
     with pytest.raises(PdmUsageError):
         list(selection)
 
 
 def test_deprecation_warning():
-    with pytest.warns(DeprecationWarning) as record:
+    with pytest.warns(FutureWarning) as record:
         utils.deprecation_warning("Test warning", raise_since="99.99")
     assert len(record) == 1
     assert str(record[0].message) == "Test warning"
 
-    with pytest.raises(DeprecationWarning):
+    with pytest.raises(FutureWarning):
         utils.deprecation_warning("Test warning", raise_since="0.0")
```

### Comparing `pdm-2.7.4/PKG-INFO` & `pdm-2.8.0a0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdm
-Version: 2.7.4
+Version: 2.8.0a0
 Summary: A modern Python package and dependency manager supporting the latest PEP standards
 Keywords: packaging dependency workflow
 Author-Email: Frost Ming <mianghong@gmail.com>
 License: MIT
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
@@ -30,14 +30,15 @@
 Requires-Dist: tomlkit<1,>=0.11.1
 Requires-Dist: shellingham>=1.3.2
 Requires-Dist: python-dotenv>=0.15
 Requires-Dist: resolvelib>=1.0.1
 Requires-Dist: installer<0.8,>=0.7
 Requires-Dist: cachecontrol[filecache]>=0.13.0
 Requires-Dist: tomli>=1.1.0; python_version < "3.11"
+Requires-Dist: importlib-resources>=5; python_version < "3.9"
 Requires-Dist: importlib-metadata>=3.6; python_version < "3.10"
 Requires-Dist: pytest; extra == "pytest"
 Requires-Dist: pytest-mock; extra == "pytest"
 Provides-Extra: pytest
 Description-Content-Type: text/markdown
 
 <div align="center">
@@ -123,25 +124,25 @@
 ### Via Install Script
 
 Like Pip, PDM provides an installation script that will install PDM into an isolated environment.
 
 **For Linux/Mac**
 
 ```bash
-curl -sSL https://raw.githubusercontent.com/pdm-project/pdm/main/install-pdm.py | python3 -
+curl -sSL https://pdm.fming.dev/dev/install-pdm.py | python3 -
 ```
 
 **For Windows**
 
 ```powershell
-(Invoke-WebRequest -Uri https://raw.githubusercontent.com/pdm-project/pdm/main/install-pdm.py -UseBasicParsing).Content | python -
+(Invoke-WebRequest -Uri https://pdm.fming.dev/dev/install-pdm.py -UseBasicParsing).Content | python -
 ```
 
 For security reasons, you should verify the checksum of `install-pdm.py`.
-The sha256 checksum is: `965900c551b4d1ba5127ecf95c127c99b5a1cccef4c183a5ecf447e876fa3160`
+It can be downloaded from [install-pdm.py.sha256](https://pdm.fming.dev/dev/install-pdm.py.sha256).
 
 The installer will install PDM into the user site and the location depends on the system:
 
 - `$HOME/.local/bin` for Unix
 - `%APPDATA%\Python\Scripts` on Windows
 
 You can pass additional options to the script to control how PDM is installed:
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1 Name: pdm Version: 2.7.4 Summary: A modern Python package
-and dependency manager supporting the latest PEP standards Keywords: packaging
-dependency workflow Author-Email: Frost Ming
+Metadata-Version: 2.1 Name: pdm Version: 2.8.0a0 Summary: A modern Python
+package and dependency manager supporting the latest PEP standards Keywords:
+packaging dependency workflow Author-Email: Frost Ming
 gmail.com> License: MIT Classifier: Topic :: Software Development :: Build
 Tools Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Project-URL: Homepage, https://pdm.fming.dev Project-URL: Repository, https://
 github.com/pdm-project/pdm Project-URL: Documentation, https://pdm.fming.dev
@@ -13,17 +13,18 @@
 packaging!=22.0,>=20.9 Requires-Dist: platformdirs Requires-Dist: rich>=12.3.0
 Requires-Dist: virtualenv>=20 Requires-Dist: pyproject-hooks Requires-Dist:
 requests-toolbelt Requires-Dist: unearth>=0.9.0 Requires-Dist:
 findpython>=0.2.2 Requires-Dist: tomlkit<1,>=0.11.1 Requires-Dist:
 shellingham>=1.3.2 Requires-Dist: python-dotenv>=0.15 Requires-Dist:
 resolvelib>=1.0.1 Requires-Dist: installer<0.8,>=0.7 Requires-Dist:
 cachecontrol[filecache]>=0.13.0 Requires-Dist: tomli>=1.1.0; python_version <
-"3.11" Requires-Dist: importlib-metadata>=3.6; python_version < "3.10"
-Requires-Dist: pytest; extra == "pytest" Requires-Dist: pytest-mock; extra ==
-"pytest" Provides-Extra: pytest Description-Content-Type: text/markdown
+"3.11" Requires-Dist: importlib-resources>=5; python_version < "3.9" Requires-
+Dist: importlib-metadata>=3.6; python_version < "3.10" Requires-Dist: pytest;
+extra == "pytest" Requires-Dist: pytest-mock; extra == "pytest" Provides-Extra:
+pytest Description-Content-Type: text/markdown
 # PDM A modern Python package and dependency manager supporting the latest PEP
       standards. [ä¸­æçæ¬è¯´æ](README_zh.md) ![PDM logo](https://
 raw.githubusercontent.com/pdm-project/pdm/main/docs/docs/assets/logo_big.png)
  [![Docs](https://img.shields.io/badge/Docs-mkdocs-blue?style=for-the-badge)]
   (https://pdm.fming.dev) [![Twitter Follow](https://img.shields.io/twitter/
    follow/pdm_project?label=get%20updates&logo=twitter&style=for-the-badge)]
  (https://twitter.com/pdm_project) [![Discord](https://img.shields.io/discord/
@@ -74,25 +75,24 @@
 `pyproject.toml` file and supports lockfiles. Users can add additional
 functionality through plugins, which can be shared by uploading them as
 distributions. Unlike Poetry and Hatch, PDM is not limited to a specific build
 backend; users have the freedom to choose any build backend they prefer. ##
 Installation PDM requires python version 3.7 or higher. ### Via Install Script
 Like Pip, PDM provides an installation script that will install PDM into an
 isolated environment. **For Linux/Mac** ```bash curl -sSL https://
-raw.githubusercontent.com/pdm-project/pdm/main/install-pdm.py | python3 - ```
-**For Windows** ```powershell (Invoke-WebRequest -Uri https://
-raw.githubusercontent.com/pdm-project/pdm/main/install-pdm.py -
+pdm.fming.dev/dev/install-pdm.py | python3 - ``` **For Windows** ```powershell
+(Invoke-WebRequest -Uri https://pdm.fming.dev/dev/install-pdm.py -
 UseBasicParsing).Content | python - ``` For security reasons, you should verify
-the checksum of `install-pdm.py`. The sha256 checksum is:
-`965900c551b4d1ba5127ecf95c127c99b5a1cccef4c183a5ecf447e876fa3160` The
-installer will install PDM into the user site and the location depends on the
-system: - `$HOME/.local/bin` for Unix - `%APPDATA%\Python\Scripts` on Windows
-You can pass additional options to the script to control how PDM is installed:
-``` usage: install-pdm.py [-h] [-v VERSION] [--prerelease] [--remove] [-p PATH]
-[-d DEP] optional arguments: -h, --help show this help message and exit -
+the checksum of `install-pdm.py`. It can be downloaded from [install-
+pdm.py.sha256](https://pdm.fming.dev/dev/install-pdm.py.sha256). The installer
+will install PDM into the user site and the location depends on the system: -
+`$HOME/.local/bin` for Unix - `%APPDATA%\Python\Scripts` on Windows You can
+pass additional options to the script to control how PDM is installed: ```
+usage: install-pdm.py [-h] [-v VERSION] [--prerelease] [--remove] [-p PATH] [-
+d DEP] optional arguments: -h, --help show this help message and exit -
 v VERSION, --version VERSION | envvar: PDM_VERSION Specify the version to be
 installed, or HEAD to install from the main branch --prerelease | envvar:
 PDM_PRERELEASE Allow prereleases to be installed --remove | envvar: PDM_REMOVE
 Remove the PDM installation -p PATH, --path PATH | envvar: PDM_HOME Specify the
 location to install PDM -d DEP, --dep DEP | envvar: PDM_DEPS Specify additional
 dependencies, can be given multiple times ``` You can either pass the options
 after the script or set the env var value. ### Alternative Installation Methods
```

