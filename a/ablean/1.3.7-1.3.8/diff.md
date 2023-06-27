# Comparing `tmp/ablean-1.3.7.tar.gz` & `tmp/ablean-1.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ablean-1.3.7.tar", last modified: Wed Jun 21 05:42:54 2023, max compression
+gzip compressed data, was "ablean-1.3.8.tar", last modified: Tue Jun 27 01:25:05 2023, max compression
```

## Comparing `ablean-1.3.7.tar` & `ablean-1.3.8.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxrwxr-x   0 hetao     (1000) hetao     (1000)        0 2023-06-21 05:42:54.362232 ablean-1.3.7/
--rw-rw-r--   0 hetao     (1000) hetao     (1000)     2044 2023-06-21 04:54:40.000000 ablean-1.3.7/.gitignore
-drwxrwxr-x   0 hetao     (1000) hetao     (1000)        0 2023-06-21 05:42:54.358232 ablean-1.3.7/.vscode/
--rw-rw-r--   0 hetao     (1000) hetao     (1000)     1454 2023-06-21 05:23:20.000000 ablean-1.3.7/.vscode/launch.json
--rw-rw-r--   0 hetao     (1000) hetao     (1000)    54640 2023-06-21 05:42:54.362232 ablean-1.3.7/PKG-INFO
--rw-rw-r--   0 hetao     (1000) hetao     (1000)    53240 2023-06-21 04:54:40.000000 ablean-1.3.7/README.md
-drwxrwxr-x   0 hetao     (1000) hetao     (1000)        0 2023-06-21 05:42:54.358232 ablean-1.3.7/ablean/
--rw-rw-r--   0 hetao     (1000) hetao     (1000)      913 2023-06-21 05:41:53.000000 ablean-1.3.7/ablean/__init__.py
-drwxrwxr-x   0 hetao     (1000) hetao     (1000)        0 2023-06-21 05:42:54.358232 ablean-1.3.7/ablean/commands/
--rw-rw-r--   0 hetao     (1000) hetao     (1000)     1241 2023-06-21 04:54:40.000000 ablean-1.3.7/ablean/commands/__init__.py
--rw-rw-r--   0 hetao     (1000) hetao     (1000)    12217 2023-06-21 04:54:40.000000 ablean-1.3.7/ablean/commands/backtest.py
--rw-rw-r--   0 hetao     (1000) hetao     (1000)     9936 2023-06-21 04:54:40.000000 ablean-1.3.7/ablean/commands/create_project.py
--rw-rw-r--   0 hetao     (1000) hetao     (1000)     1271 2023-06-21 04:54:40.000000 ablean-1.3.7/ablean/commands/download.py
--rw-rw-r--   0 hetao     (1000) hetao     (1000)     2034 2023-06-21 04:54:40.000000 ablean-1.3.7/ablean/commands/init.py
-drwxrwxr-x   0 hetao     (1000) hetao     (1000)        0 2023-06-21 05:42:54.358232 ablean-1.3.7/ablean/components/
--rw-rw-r--   0 hetao     (1000) hetao     (1000)      664 2023-06-21 04:54:40.000000 ablean-1.3.7/ablean/components/__init__.py
-drwxrwxr-x   0 hetao     (1000) hetao     (1000)        0 2023-06-21 05:42:54.358232 ablean-1.3.7/ablean/components/config/
--rw-rw-r--   0 hetao     (1000) hetao     (1000)      664 2023-06-21 04:54:40.000000 ablean-1.3.7/ablean/components/config/__init__.py
--rw-rw-r--   0 hetao     (1000) hetao     (1000)     2715 2023-06-21 04:54:40.000000 ablean-1.3.7/ablean/components/config/cli_config_manager.py
--rw-rw-r--   0 hetao     (1000) hetao     (1000)    13716 2023-06-21 05:30:03.000000 ablean-1.3.7/ablean/components/config/lean_config_manager.py
--rw-rw-r--   0 hetao     (1000) hetao     (1000)     5302 2023-06-21 04:54:40.000000 ablean-1.3.7/ablean/components/config/output_config_manager.py
--rw-rw-r--   0 hetao     (1000) hetao     (1000)     2378 2023-06-21 04:54:40.000000 ablean-1.3.7/ablean/components/config/project_config_manager.py
--rw-rw-r--   0 hetao     (1000) hetao     (1000)     3184 2023-06-21 04:54:40.000000 ablean-1.3.7/ablean/components/config/storage.py
--rw-rw-r--   0 hetao     (1000) hetao     (1000)     5106 2023-06-21 05:39:09.000000 ablean-1.3.7/ablean/components/lean_runner.py
--rw-rw-r--   0 hetao     (1000) hetao     (1000)     2727 2023-06-21 04:54:40.000000 ablean-1.3.7/ablean/components/module_manager.py
-drwxrwxr-x   0 hetao     (1000) hetao     (1000)        0 2023-06-21 05:42:54.358232 ablean-1.3.7/ablean/components/util/
--rw-rw-r--   0 hetao     (1000) hetao     (1000)      664 2023-06-21 04:54:40.000000 ablean-1.3.7/ablean/components/util/__init__.py
--rw-rw-r--   0 hetao     (1000) hetao     (1000)     6186 2023-06-21 04:54:40.000000 ablean-1.3.7/ablean/components/util/logger.py
--rw-rw-r--   0 hetao     (1000) hetao     (1000)     1335 2023-06-21 04:54:40.000000 ablean-1.3.7/ablean/components/util/name_extraction.py
--rw-rw-r--   0 hetao     (1000) hetao     (1000)     3156 2023-06-21 04:54:40.000000 ablean-1.3.7/ablean/components/util/name_generator.py
--rw-rw-r--   0 hetao     (1000) hetao     (1000)     3190 2023-06-21 04:54:40.000000 ablean-1.3.7/ablean/components/util/path_manager.py
--rw-rw-r--   0 hetao     (1000) hetao     (1000)     4474 2023-06-21 04:54:40.000000 ablean-1.3.7/ablean/components/util/platform_manager.py
--rw-rw-r--   0 hetao     (1000) hetao     (1000)    21386 2023-06-21 04:54:40.000000 ablean-1.3.7/ablean/components/util/project_manager.py
--rw-rw-r--   0 hetao     (1000) hetao     (1000)     1647 2023-06-21 04:54:40.000000 ablean-1.3.7/ablean/components/util/temp_manager.py
--rw-rw-r--   0 hetao     (1000) hetao     (1000)     1641 2023-06-21 04:54:40.000000 ablean-1.3.7/ablean/components/util/xml_manager.py
--rw-rw-r--   0 hetao     (1000) hetao     (1000)     4367 2023-06-21 04:54:40.000000 ablean-1.3.7/ablean/constants.py
--rw-rw-r--   0 hetao     (1000) hetao     (1000)     3766 2023-06-21 04:54:40.000000 ablean-1.3.7/ablean/container.py
--rw-rw-r--   0 hetao     (1000) hetao     (1000)     8201 2023-06-21 04:54:40.000000 ablean-1.3.7/ablean/data_manager.py
-drwxrwxr-x   0 hetao     (1000) hetao     (1000)        0 2023-06-21 05:42:54.358232 ablean-1.3.7/ablean/icons/
--rw-rw-r--   0 hetao     (1000) hetao     (1000)    34808 2023-06-21 04:54:40.000000 ablean-1.3.7/ablean/icons/icon.icns
--rw-rw-r--   0 hetao     (1000) hetao     (1000)    14816 2023-06-21 04:54:40.000000 ablean-1.3.7/ablean/icons/icon.ico
--rw-rw-r--   0 hetao     (1000) hetao     (1000)     5826 2023-06-21 04:54:40.000000 ablean-1.3.7/ablean/main.py
-drwxrwxr-x   0 hetao     (1000) hetao     (1000)        0 2023-06-21 05:42:54.362232 ablean-1.3.7/ablean/models/
--rw-rw-r--   0 hetao     (1000) hetao     (1000)      664 2023-06-21 04:54:40.000000 ablean-1.3.7/ablean/models/__init__.py
--rw-rw-r--   0 hetao     (1000) hetao     (1000)     2248 2023-06-21 04:54:40.000000 ablean-1.3.7/ablean/models/errors.py
--rw-rw-r--   0 hetao     (1000) hetao     (1000)     1515 2023-06-21 04:54:40.000000 ablean-1.3.7/ablean/models/modules.py
--rw-rw-r--   0 hetao     (1000) hetao     (1000)     3938 2023-06-21 04:54:40.000000 ablean-1.3.7/ablean/models/options.py
--rw-rw-r--   0 hetao     (1000) hetao     (1000)     1469 2023-06-21 04:54:40.000000 ablean-1.3.7/ablean/models/pydantic.py
--rw-rw-r--   0 hetao     (1000) hetao     (1000)     1415 2023-06-21 04:54:40.000000 ablean-1.3.7/ablean/models/utils.py
--rw-rw-r--   0 hetao     (1000) hetao     (1000)     9715 2023-06-21 04:54:40.000000 ablean-1.3.7/ablean/myclick.py
-drwxrwxr-x   0 hetao     (1000) hetao     (1000)        0 2023-06-21 05:42:54.358232 ablean-1.3.7/ablean.egg-info/
--rw-rw-r--   0 hetao     (1000) hetao     (1000)    54640 2023-06-21 05:42:54.000000 ablean-1.3.7/ablean.egg-info/PKG-INFO
--rw-rw-r--   0 hetao     (1000) hetao     (1000)     1428 2023-06-21 05:42:54.000000 ablean-1.3.7/ablean.egg-info/SOURCES.txt
--rw-rw-r--   0 hetao     (1000) hetao     (1000)        1 2023-06-21 05:42:54.000000 ablean-1.3.7/ablean.egg-info/dependency_links.txt
--rw-rw-r--   0 hetao     (1000) hetao     (1000)       44 2023-06-21 05:42:54.000000 ablean-1.3.7/ablean.egg-info/entry_points.txt
--rw-rw-r--   0 hetao     (1000) hetao     (1000)      302 2023-06-21 05:42:54.000000 ablean-1.3.7/ablean.egg-info/requires.txt
--rw-rw-r--   0 hetao     (1000) hetao     (1000)        7 2023-06-21 05:42:54.000000 ablean-1.3.7/ablean.egg-info/top_level.txt
--rw-rw-r--   0 hetao     (1000) hetao     (1000)      894 2023-06-21 04:54:40.000000 ablean-1.3.7/pub.ps1
-drwxrwxr-x   0 hetao     (1000) hetao     (1000)        0 2023-06-21 05:42:54.362232 ablean-1.3.7/scripts/
--rw-rw-r--   0 hetao     (1000) hetao     (1000)     3792 2023-06-21 04:54:40.000000 ablean-1.3.7/scripts/readme.py
--rw-rw-r--   0 hetao     (1000) hetao     (1000)       38 2023-06-21 05:42:54.362232 ablean-1.3.7/setup.cfg
--rw-rw-r--   0 hetao     (1000) hetao     (1000)     3341 2023-06-21 04:54:40.000000 ablean-1.3.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-27 01:25:05.309051 ablean-1.3.8/
+-rw-rw-rw-   0        0        0     2184 2022-06-06 10:43:40.000000 ablean-1.3.8/.gitignore
+drwxrwxrwx   0        0        0        0 2023-06-27 01:25:05.257661 ablean-1.3.8/.vscode/
+-rw-rw-rw-   0        0        0     1442 2023-04-20 14:13:20.000000 ablean-1.3.8/.vscode/launch.json
+-rw-rw-rw-   0        0        0    55778 2023-06-27 01:25:05.309051 ablean-1.3.8/PKG-INFO
+-rw-rw-rw-   0        0        0    53240 2022-06-05 03:11:14.000000 ablean-1.3.8/README.md
+drwxrwxrwx   0        0        0        0 2023-06-27 01:25:05.263335 ablean-1.3.8/ablean/
+-rw-rw-rw-   0        0        0      930 2023-06-26 09:01:52.000000 ablean-1.3.8/ablean/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-27 01:25:05.284410 ablean-1.3.8/ablean/commands/
+-rw-rw-rw-   0        0        0     1273 2022-06-06 09:45:38.000000 ablean-1.3.8/ablean/commands/__init__.py
+-rw-rw-rw-   0        0        0    12597 2023-06-21 04:52:15.000000 ablean-1.3.8/ablean/commands/backtest.py
+-rw-rw-rw-   0        0        0    11132 2023-06-26 09:01:36.000000 ablean-1.3.8/ablean/commands/create_project.py
+-rw-rw-rw-   0        0        0     1322 2022-06-10 02:17:02.000000 ablean-1.3.8/ablean/commands/download.py
+-rw-rw-rw-   0        0        0     2098 2022-06-06 10:41:51.000000 ablean-1.3.8/ablean/commands/init.py
+drwxrwxrwx   0        0        0        0 2023-06-27 01:25:05.286463 ablean-1.3.8/ablean/components/
+-rw-rw-rw-   0        0        0      676 2022-06-05 03:11:14.000000 ablean-1.3.8/ablean/components/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-27 01:25:05.292185 ablean-1.3.8/ablean/components/config/
+-rw-rw-rw-   0        0        0      676 2022-06-05 03:11:14.000000 ablean-1.3.8/ablean/components/config/__init__.py
+-rw-rw-rw-   0        0        0     2786 2022-06-05 03:11:14.000000 ablean-1.3.8/ablean/components/config/cli_config_manager.py
+-rw-rw-rw-   0        0        0    14072 2023-06-21 01:14:02.000000 ablean-1.3.8/ablean/components/config/lean_config_manager.py
+-rw-rw-rw-   0        0        0     5417 2022-06-05 03:11:14.000000 ablean-1.3.8/ablean/components/config/output_config_manager.py
+-rw-rw-rw-   0        0        0     2435 2022-06-05 03:11:14.000000 ablean-1.3.8/ablean/components/config/project_config_manager.py
+-rw-rw-rw-   0        0        0     3279 2022-06-05 07:48:48.000000 ablean-1.3.8/ablean/components/config/storage.py
+-rw-rw-rw-   0        0        0     5080 2022-06-05 03:11:14.000000 ablean-1.3.8/ablean/components/lean_runner.py
+-rw-rw-rw-   0        0        0     2787 2022-06-05 03:11:14.000000 ablean-1.3.8/ablean/components/module_manager.py
+drwxrwxrwx   0        0        0        0 2023-06-27 01:25:05.299835 ablean-1.3.8/ablean/components/util/
+-rw-rw-rw-   0        0        0      676 2022-06-05 08:19:14.000000 ablean-1.3.8/ablean/components/util/__init__.py
+-rw-rw-rw-   0        0        0     6356 2022-06-05 03:11:14.000000 ablean-1.3.8/ablean/components/util/logger.py
+-rw-rw-rw-   0        0        0     1368 2022-06-05 03:11:14.000000 ablean-1.3.8/ablean/components/util/name_extraction.py
+-rw-rw-rw-   0        0        0     3205 2022-06-05 03:11:14.000000 ablean-1.3.8/ablean/components/util/name_generator.py
+-rw-rw-rw-   0        0        0     3261 2022-06-05 03:11:14.000000 ablean-1.3.8/ablean/components/util/path_manager.py
+-rw-rw-rw-   0        0        0     4584 2022-06-05 03:11:14.000000 ablean-1.3.8/ablean/components/util/platform_manager.py
+-rw-rw-rw-   0        0        0    21926 2022-06-05 04:02:32.000000 ablean-1.3.8/ablean/components/util/project_manager.py
+-rw-rw-rw-   0        0        0     1689 2022-06-05 03:11:14.000000 ablean-1.3.8/ablean/components/util/temp_manager.py
+-rw-rw-rw-   0        0        0     1680 2022-06-05 03:11:14.000000 ablean-1.3.8/ablean/components/util/xml_manager.py
+-rw-rw-rw-   0        0        0     4485 2023-06-21 00:58:59.000000 ablean-1.3.8/ablean/constants.py
+-rw-rw-rw-   0        0        0     3838 2022-06-05 03:11:14.000000 ablean-1.3.8/ablean/container.py
+-rw-rw-rw-   0        0        0     8436 2022-06-22 06:13:42.000000 ablean-1.3.8/ablean/data_manager.py
+drwxrwxrwx   0        0        0        0 2023-06-27 01:25:05.301080 ablean-1.3.8/ablean/icons/
+-rw-rw-rw-   0        0        0    34808 2022-06-05 03:11:14.000000 ablean-1.3.8/ablean/icons/icon.icns
+-rw-rw-rw-   0        0        0    14816 2022-06-05 03:11:14.000000 ablean-1.3.8/ablean/icons/icon.ico
+-rw-rw-rw-   0        0        0     5968 2022-06-06 09:47:56.000000 ablean-1.3.8/ablean/main.py
+drwxrwxrwx   0        0        0        0 2023-06-27 01:25:05.307067 ablean-1.3.8/ablean/models/
+-rw-rw-rw-   0        0        0      676 2022-06-05 03:11:14.000000 ablean-1.3.8/ablean/models/__init__.py
+-rw-rw-rw-   0        0        0     2305 2022-06-05 03:11:14.000000 ablean-1.3.8/ablean/models/errors.py
+-rw-rw-rw-   0        0        0     1555 2022-06-05 03:11:14.000000 ablean-1.3.8/ablean/models/modules.py
+-rw-rw-rw-   0        0        0     4037 2022-06-05 03:11:14.000000 ablean-1.3.8/ablean/models/options.py
+-rw-rw-rw-   0        0        0     1507 2022-06-05 03:11:14.000000 ablean-1.3.8/ablean/models/pydantic.py
+-rw-rw-rw-   0        0        0     1456 2022-06-05 03:11:14.000000 ablean-1.3.8/ablean/models/utils.py
+-rw-rw-rw-   0        0        0     9966 2022-06-05 03:11:14.000000 ablean-1.3.8/ablean/myclick.py
+drwxrwxrwx   0        0        0        0 2023-06-27 01:25:05.279923 ablean-1.3.8/ablean.egg-info/
+-rw-rw-rw-   0        0        0    55778 2023-06-27 01:25:05.000000 ablean-1.3.8/ablean.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1428 2023-06-27 01:25:05.000000 ablean-1.3.8/ablean.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-27 01:25:05.000000 ablean-1.3.8/ablean.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2023-06-27 01:25:05.000000 ablean-1.3.8/ablean.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      302 2023-06-27 01:25:05.000000 ablean-1.3.8/ablean.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-27 01:25:05.000000 ablean-1.3.8/ablean.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      920 2023-06-22 13:16:53.000000 ablean-1.3.8/pub.ps1
+drwxrwxrwx   0        0        0        0 2023-06-27 01:25:05.308049 ablean-1.3.8/scripts/
+-rw-rw-rw-   0        0        0     3900 2022-06-05 03:31:44.000000 ablean-1.3.8/scripts/readme.py
+-rw-rw-rw-   0        0        0       42 2023-06-27 01:25:05.310049 ablean-1.3.8/setup.cfg
+-rw-rw-rw-   0        0        0     3443 2022-06-05 05:42:03.000000 ablean-1.3.8/setup.py
```

### Comparing `ablean-1.3.7/.gitignore` & `ablean-1.3.8/.gitignore`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,141 +1,141 @@
-# Byte-compiled / optimized / DLL files
-__pycache__/
-*.py[cod]
-*$py.class
-
-# C extensions
-*.so
-
-# Distribution / packaging
-.Python
-build/
-develop-eggs/
-dist/
-downloads/
-eggs/
-.eggs/
-lib/
-lib64/
-parts/
-sdist/
-var/
-wheels/
-share/python-wheels/
-*.egg-info/
-.installed.cfg
-*.egg
-MANIFEST
-
-# PyInstaller
-#  Usually these files are written by a python script from a template
-#  before PyInstaller builds the exe, so as to inject date/other infos into it.
-*.manifest
-*.spec
-
-# Installer logs
-pip-log.txt
-pip-delete-this-directory.txt
-
-# Unit test / coverage reports
-htmlcov/
-.tox/
-.nox/
-.coverage
-.coverage.*
-.cache
-nosetests.xml
-coverage.xml
-*.cover
-*.py,cover
-.hypothesis/
-.pytest_cache/
-cover/
-
-# Translations
-*.mo
-*.pot
-
-# Django stuff:
-*.log
-local_settings.py
-db.sqlite3
-db.sqlite3-journal
-
-# Flask stuff:
-instance/
-.webassets-cache
-
-# Scrapy stuff:
-.scrapy
-
-# Sphinx documentation
-docs/_build/
-
-# PyBuilder
-.pybuilder/
-target/
-
-# Jupyter Notebook
-.ipynb_checkpoints
-
-# IPython
-profile_default/
-ipython_config.py
-
-# pyenv
-#   For a library or package, you might want to ignore these files since the code is
-#   intended to run in multiple environments; otherwise, check them in:
-# .python-version
-
-# pipenv
-#   According to pypa/pipenv#598, it is recommended to include Pipfile.lock in version control.
-#   However, in case of collaboration, if having platform-specific dependencies or dependencies
-#   having no cross-platform support, pipenv may install dependencies that don't work, or not
-#   install all needed dependencies.
-#Pipfile.lock
-
-# PEP 582; used by e.g. github.com/David-OConnor/pyflow
-__pypackages__/
-
-# Celery stuff
-celerybeat-schedule
-celerybeat.pid
-
-# SageMath parsed files
-*.sage.py
-
-# Environments
-.env
-.venv
-env/
-venv/
-ENV/
-env.bak/
-venv.bak/
-
-# Spyder project settings
-.spyderproject
-.spyproject
-
-# Rope project settings
-.ropeproject
-
-# mkdocs documentation
-/site
-
-# mypy
-.mypy_cache/
-.dmypy.json
-dmypy.json
-
-# Pyre type checker
-.pyre/
-
-# pytype static type analyzer
-.pytype/
-
-# Cython debug symbols
-cython_debug/
-
-.vs
+# Byte-compiled / optimized / DLL files
+__pycache__/
+*.py[cod]
+*$py.class
+
+# C extensions
+*.so
+
+# Distribution / packaging
+.Python
+build/
+develop-eggs/
+dist/
+downloads/
+eggs/
+.eggs/
+lib/
+lib64/
+parts/
+sdist/
+var/
+wheels/
+share/python-wheels/
+*.egg-info/
+.installed.cfg
+*.egg
+MANIFEST
+
+# PyInstaller
+#  Usually these files are written by a python script from a template
+#  before PyInstaller builds the exe, so as to inject date/other infos into it.
+*.manifest
+*.spec
+
+# Installer logs
+pip-log.txt
+pip-delete-this-directory.txt
+
+# Unit test / coverage reports
+htmlcov/
+.tox/
+.nox/
+.coverage
+.coverage.*
+.cache
+nosetests.xml
+coverage.xml
+*.cover
+*.py,cover
+.hypothesis/
+.pytest_cache/
+cover/
+
+# Translations
+*.mo
+*.pot
+
+# Django stuff:
+*.log
+local_settings.py
+db.sqlite3
+db.sqlite3-journal
+
+# Flask stuff:
+instance/
+.webassets-cache
+
+# Scrapy stuff:
+.scrapy
+
+# Sphinx documentation
+docs/_build/
+
+# PyBuilder
+.pybuilder/
+target/
+
+# Jupyter Notebook
+.ipynb_checkpoints
+
+# IPython
+profile_default/
+ipython_config.py
+
+# pyenv
+#   For a library or package, you might want to ignore these files since the code is
+#   intended to run in multiple environments; otherwise, check them in:
+# .python-version
+
+# pipenv
+#   According to pypa/pipenv#598, it is recommended to include Pipfile.lock in version control.
+#   However, in case of collaboration, if having platform-specific dependencies or dependencies
+#   having no cross-platform support, pipenv may install dependencies that don't work, or not
+#   install all needed dependencies.
+#Pipfile.lock
+
+# PEP 582; used by e.g. github.com/David-OConnor/pyflow
+__pypackages__/
+
+# Celery stuff
+celerybeat-schedule
+celerybeat.pid
+
+# SageMath parsed files
+*.sage.py
+
+# Environments
+.env
+.venv
+env/
+venv/
+ENV/
+env.bak/
+venv.bak/
+
+# Spyder project settings
+.spyderproject
+.spyproject
+
+# Rope project settings
+.ropeproject
+
+# mkdocs documentation
+/site
+
+# mypy
+.mypy_cache/
+.dmypy.json
+dmypy.json
+
+# Pyre type checker
+.pyre/
+
+# pytype static type analyzer
+.pytype/
+
+# Cython debug symbols
+cython_debug/
+
+.vs
 temp
```

### Comparing `ablean-1.3.7/PKG-INFO` & `ablean-1.3.8/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,1138 +1,1138 @@
-Metadata-Version: 2.1
-Name: ablean
-Version: 1.3.7
-Summary: A CLI aimed at making it easier to run QuantConnect's LEAN engine locally and in the cloud
-Home-page: https://lean.io/cli
-Author: abl
-Author-email: support@quantconnect.com
-Project-URL: Documentation, https://www.lean.io/docs/lean-cli/key-concepts/getting-started
-Project-URL: Source, https://github.com/QuantConnect/lean-cli
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Financial and Insurance Industry
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Requires-Python: >= 3.8
-Description-Content-Type: text/markdown
-
-![Lean CLI](http://cdn.quantconnect.com.s3.us-east-1.amazonaws.com/i/github/lean-cli-splash.png)
-
-# QuantConnect Lean CLI
- 
-[![Build Status](https://github.com/QuantConnect/lean-cli/workflows/Build/badge.svg)](https://github.com/QuantConnect/lean-cli/actions?query=workflow%3ABuild)
-[![PyPI Version](https://img.shields.io/pypi/v/lean)](https://pypi.org/project/lean/)
-[![Project Status](https://img.shields.io/pypi/status/lean)](https://pypi.org/project/lean/)
-
-The Lean CLI is a cross-platform CLI aimed at making it easier to develop with the LEAN engine locally and in the cloud.
-
-Visit the [documentation website](https://www.lean.io/docs/lean-cli/key-concepts/getting-started) for comprehensive and up-to-date documentation.
-
-## Highlights
-
-- [Project scaffolding](https://www.lean.io/docs/lean-cli/projects/project-management)
-- [Local autocomplete](https://www.lean.io/docs/lean-cli/projects/autocomplete)
-- [Local data downloading](https://www.lean.io/docs/lean-cli/datasets/downloading-quantconnect-data)
-- [Local backtesting](https://www.lean.io/docs/lean-cli/backtesting/deployment#02-Run-Local-Backtests)
-- [Local debugging](https://www.lean.io/docs/lean-cli/backtesting/debugging)
-- [Local research environment](https://www.lean.io/docs/lean-cli/research)
-- [Local optimization](https://www.lean.io/docs/lean-cli/optimization/deployment#02-Run-Local-Optimizations)
-- [Local live trading](https://www.lean.io/docs/lean-cli/live-trading/quantconnect-paper-trading#02-Deploy-Local-Algorithms)
-- [Local backtest report creation](https://www.lean.io/docs/lean-cli/backtesting/report#02-Generate-a-Report)
-- [Cloud synchronization](https://www.lean.io/docs/lean-cli/projects/cloud-synchronization)
-- [Cloud backtesting](https://www.lean.io/docs/lean-cli/backtesting/deployment#03-Run-Cloud-Backtests)
-- [Cloud optimization](https://www.lean.io/docs/lean-cli/optimization/deployment#03-Run-Cloud-Optimizations)
-- [Cloud live trading](https://www.lean.io/docs/lean-cli/live-trading/quantconnect-paper-trading#03-Deploy-Cloud-Algorithms)
-
-## Installation
-
-The CLI can be installed and updated by running `pip install --upgrade lean`.
-
-Note that many commands in the CLI require Docker to run. See [Get Docker](https://docs.docker.com/get-docker/) for instructions on how to install Docker for your operating system.
-
-**Note:** Some Linux users may need to install `tkinter` using the following commands:
-
-``` 
-For Python 3
-
-sudo apt-get install python3-tk
-
-For Python 2.7
-
-sudo apt-get install python-tk
-```
-After installing the CLI, open a terminal in an empty directory and run `lean init`. This command downloads the latest configuration file and sample data from the [QuantConnect/Lean](https://github.com/QuantConnect/Lean) repository. We recommend running all Lean CLI commands in the same directory `lean init` was ran in.
-
-## Usage
-
-The Lean CLI supports multiple workflows. The examples below serve as a starting point, you're free to mix local and cloud features in any way you'd like.
-
-A cloud-focused workflow (local development, cloud execution) with the CLI may look like this:
-1. Open a terminal in the directory you ran `lean init` in.
-2. Run `lean cloud pull` to pull remotely changed files.
-3. Start programming locally and run backtests in the cloud with `lean cloud backtest "Project Name" --open --push` whenever there is something to backtest. The `--open` flag means that the backtest results will be opened in the browser when done, while the `--push` flag means that local changes are pushed to the cloud before running the backtest.
-4. Whenever you want to create a new project, run `lean create-project "Project Name"` and `lean cloud push --project "Project Name"` to create a new project containing some basic code and to push it to the cloud.
-5. When you're finished for the moment, run `lean cloud push` to push all locally changed files to the cloud.
-
-A locally-focused workflow (local development, local execution) with the CLI may look like this:
-1. Open a terminal in the directory you ran `lean init` in.
-2. Run `lean create-project "Project Name"` to create a new project with some basic code to get you started.
-3. Work on your strategy in `./Project Name`.
-4. Run `lean research "Project Name"` to start a Jupyter Lab session to perform research in.
-5. Run `lean backtest "Project Name"` to run a backtest whenever there's something to test. This runs your strategy in a Docker container containing the same packages as the ones used on QuantConnect.com, but with your own data.
-
-## Commands
-
-*Note: the readme only contains the `--help` text of all commands. Visit the [documentation website](https://www.lean.io/docs/lean-cli/key-concepts/getting-started) for more comprehensive documentation.*
-
-<!-- commands start -->
-- [`lean backtest`](#lean-backtest)
-- [`lean build`](#lean-build)
-- [`lean cloud backtest`](#lean-cloud-backtest)
-- [`lean cloud live`](#lean-cloud-live)
-- [`lean cloud optimize`](#lean-cloud-optimize)
-- [`lean cloud pull`](#lean-cloud-pull)
-- [`lean cloud push`](#lean-cloud-push)
-- [`lean cloud status`](#lean-cloud-status)
-- [`lean config get`](#lean-config-get)
-- [`lean config list`](#lean-config-list)
-- [`lean config set`](#lean-config-set)
-- [`lean config unset`](#lean-config-unset)
-- [`lean create-project`](#lean-create-project)
-- [`lean data download`](#lean-data-download)
-- [`lean data generate`](#lean-data-generate)
-- [`lean gui logs`](#lean-gui-logs)
-- [`lean gui restart`](#lean-gui-restart)
-- [`lean gui start`](#lean-gui-start)
-- [`lean gui stop`](#lean-gui-stop)
-- [`lean init`](#lean-init)
-- [`lean library add`](#lean-library-add)
-- [`lean library remove`](#lean-library-remove)
-- [`lean live`](#lean-live)
-- [`lean login`](#lean-login)
-- [`lean logout`](#lean-logout)
-- [`lean logs`](#lean-logs)
-- [`lean optimize`](#lean-optimize)
-- [`lean report`](#lean-report)
-- [`lean research`](#lean-research)
-- [`lean whoami`](#lean-whoami)
-
-### `lean backtest`
-
-Backtest a project locally using Docker.
-
-```
-Usage: lean backtest [OPTIONS] PROJECT
-
-  Backtest a project locally using Docker.
-
-  If PROJECT is a directory, the algorithm in the main.py or Main.cs file inside it will be executed.
-  If PROJECT is a file, the algorithm in the specified file will be executed.
-
-  Go to the following url to learn how to debug backtests locally using the Lean CLI:
-  https://www.lean.io/docs/lean-cli/backtesting/debugging
-
-  By default the official LEAN engine image is used. You can override this using the --image option. Alternatively you
-  can set the default engine image for all commands using `lean config set engine-image <image>`.
-
-Options:
-  --output DIRECTORY              Directory to store results in (defaults to PROJECT/backtests/TIMESTAMP)
-  -d, --detach                    Run the backtest in a detached Docker container and return immediately
-  --debug [pycharm|ptvsd|vsdbg|rider]
-                                  Enable a certain debugging method (see --help for more information)
-  --data-provider [Terminal Link|QuantConnect|Local]
-                                  Update the Lean configuration file to retrieve data from the given provider
-  --download-data                 Update the Lean configuration file to download data from the QuantConnect API, alias
-                                  for --data-provider QuantConnect
-
-  --data-purchase-limit INTEGER   The maximum amount of QCC to spend on downloading data during the backtest when using
-                                  QuantConnect as data provider
-
-  --release                       Compile C# projects in release configuration instead of debug
-  --image TEXT                    The LEAN engine image to use (defaults to quantconnect/lean:latest)
-  --update                        Pull the LEAN engine image before running the backtest
-  --lean-config FILE              The Lean configuration file that should be used (defaults to the nearest lean.json)
-  --verbose                       Enable debug logging
-  --help                          Show this message and exit.
-```
-
-_See code: [lean/commands/backtest.py](https://github.com/QuantConnect/lean-cli/blob/master/lean/commands/backtest.py)_
-
-### `lean build`
-
-Build Docker images of your own version of LEAN and the Alpha Streams SDK.
-
-```
-Usage: lean build [OPTIONS] [ROOT]
-
-  Build Docker images of your own version of LEAN and the Alpha Streams SDK.
-
-  ROOT must point to a directory containing the LEAN repository and the Alpha Streams SDK repository:
-  https://github.com/QuantConnect/Lean & https://github.com/QuantConnect/AlphaStreams
-
-  When ROOT is not given, the current directory is used as root directory.
-
-  This command performs the following actions:
-  1. The lean-cli/foundation:latest image is built from Lean/DockerfileLeanFoundation(ARM).
-  2. LEAN is compiled in a Docker container using the lean-cli/foundation:latest image.
-  3. The Alpha Streams SDK is compiled in a Docker container using the lean-cli/foundation:latest image.
-  4. The lean-cli/engine:latest image is built from Lean/Dockerfile using lean-cli/foundation:latest as base image.
-  5. The lean-cli/research:latest image is built from Lean/DockerfileJupyter using lean-cli/engine:latest as base image.
-  6. The default engine image is set to lean-cli/engine:latest.
-  7. The default research image is set to lean-cli/research:latest.
-
-  When the foundation Dockerfile is the same as the official foundation Dockerfile, quantconnect/lean:foundation is
-  used instead of building a custom foundation image.
-
-Options:
-  --tag TEXT  The tag to apply to custom images (defaults to latest)
-  --verbose   Enable debug logging
-  --help      Show this message and exit.
-```
-
-_See code: [lean/commands/build.py](https://github.com/QuantConnect/lean-cli/blob/master/lean/commands/build.py)_
-
-### `lean cloud backtest`
-
-Backtest a project in the cloud.
-
-```
-Usage: lean cloud backtest [OPTIONS] PROJECT
-
-  Backtest a project in the cloud.
-
-  PROJECT must be the name or id of the project to run a backtest for.
-
-  If the project that has to be backtested has been pulled to the local drive with `lean cloud pull` it is possible to
-  use the --push option to push local modifications to the cloud before running the backtest.
-
-Options:
-  --name TEXT  The name of the backtest (a random one is generated if not specified)
-  --push       Push local modifications to the cloud before running the backtest
-  --open       Automatically open the results in the browser when the backtest is finished
-  --verbose    Enable debug logging
-  --help       Show this message and exit.
-```
-
-_See code: [lean/commands/cloud/backtest.py](https://github.com/QuantConnect/lean-cli/blob/master/lean/commands/cloud/backtest.py)_
-
-### `lean cloud live`
-
-Start live trading for a project in the cloud.
-
-```
-Usage: lean cloud live [OPTIONS] PROJECT
-
-  Start live trading for a project in the cloud.
-
-  PROJECT must be the name or the id of the project to start live trading for.
-
-  By default an interactive wizard is shown letting you configure the deployment. If --brokerage is given the command
-  runs in non-interactive mode. In this mode the CLI does not prompt for input or confirmation. In non-interactive
-  mode the options specific to the given brokerage are required, as well as --node, --auto-restart, --notify-order-
-  events and --notify-insights.
-
-Options:
-  --brokerage [Paper Trading|Interactive Brokers|Tradier|Oanda|Bitfinex|Coinbase Pro|Binance|Zerodha|Samco|Kraken|FTX]
-                                  The brokerage to use
-  --ib-user-name TEXT             Your Interactive Brokers username
-  --ib-account TEXT               Your Interactive Brokers account id
-  --ib-password TEXT              Your Interactive Brokers password
-  --ib-data-feed BOOLEAN          Whether the Interactive Brokers price data feed must be used instead of the
-                                  QuantConnect price data feed
-
-  --tradier-account-id TEXT       Your Tradier account id
-  --tradier-access-token TEXT     Your Tradier access token
-  --tradier-environment [live|paper]
-                                  Whether the developer sandbox should be used
-  --oanda-environment [Practice|Trade]
-                                  The environment to run in, Practice for fxTrade Practice, Trade for fxTrade
-  --oanda-account-id TEXT         Your OANDA account id
-  --oanda-access-token TEXT       Your OANDA API token
-  --bitfinex-api-key TEXT         Your Bitfinex API key
-  --bitfinex-api-secret TEXT      Your Bitfinex API secret
-  --gdax-use-sandbox [live|paper]
-                                  Whether the sandbox should be used
-  --gdax-api-key TEXT             Your Coinbase Pro API key
-  --gdax-api-secret TEXT          Your Coinbase Pro API secret
-  --gdax-passphrase TEXT          Your Coinbase Pro API passphrase
-  --binance-use-testnet [live|paper]
-                                  Whether the testnet should be used
-  --binance-api-key TEXT          Your Binance API key
-  --binance-api-secret TEXT       Your Binance API secret
-  --zerodha-api-key TEXT          Your Kite Connect API key
-  --zerodha-access-token TEXT     Your Kite Connect access token
-  --zerodha-product-type [MIS|CNC|NRML]
-                                  MIS if you are targeting intraday products, CNC if you are targeting delivery
-                                  products, NRML if you are targeting carry forward products
-
-  --zerodha-trading-segment [EQUITY|COMMODITY]
-                                  EQUITY if you are trading equities on NSE or BSE, COMMODITY if you are trading
-                                  commodities on MCX
-
-  --samco-client-id TEXT          Your Samco account Client ID
-  --samco-client-password TEXT    Your Samco account password
-  --samco-year-of-birth TEXT      Your year of birth (YYYY) registered with Samco
-  --samco-product-type [MIS|CNC|NRML]
-                                  MIS if you are targeting intraday products, CNC if you are targeting delivery
-                                  products, NRML if you are targeting carry forward products
-
-  --samco-trading-segment [EQUITY|COMMODITY]
-                                  EQUITY if you are trading equities on NSE or BSE, COMMODITY if you are trading
-                                  commodities on MCX
-
-  --kraken-api-key TEXT           Your Kraken API key
-  --kraken-api-secret TEXT        Your Kraken API secret
-  --kraken-verification-tier [Starter|Intermediate|Pro]
-                                  Your Kraken Verification Tier
-  --ftx-exchange-name [FTX|FTXUS]
-                                  FTX exchange name [FTX, FTXUS]
-  --ftx-api-key TEXT              Your FTX API key
-  --ftxus-api-key TEXT            Your FTX API key
-  --ftx-api-secret TEXT           Your FTX API secret
-  --ftxus-api-secret TEXT         Your FTX API secret
-  --ftx-account-tier [Tier1|Tier2|Tier3|Tier4|Tier5|Tier6]
-                                  Your FTX Account Tier
-  --ftxus-account-tier [Tier1|Tier2|Tier3|Tier4|Tier5|Tier6]
-                                  Your FTX Account Tier
-  --node TEXT                     The name or id of the live node to run on
-  --auto-restart BOOLEAN          Whether automatic algorithm restarting must be enabled
-  --notify-order-events BOOLEAN   Whether notifications must be sent for order events
-  --notify-insights BOOLEAN       Whether notifications must be sent for emitted insights
-  --notify-emails TEXT            A comma-separated list of 'email:subject' pairs configuring email-notifications
-  --notify-webhooks TEXT          A comma-separated list of 'url:HEADER_1=VALUE_1:HEADER_2=VALUE_2:etc' pairs
-                                  configuring webhook-notifications
-
-  --notify-sms TEXT               A comma-separated list of phone numbers configuring SMS-notifications
-  --push                          Push local modifications to the cloud before starting live trading
-  --open                          Automatically open the live results in the browser once the deployment starts
-  --verbose                       Enable debug logging
-  --help                          Show this message and exit.
-```
-
-_See code: [lean/commands/cloud/live.py](https://github.com/QuantConnect/lean-cli/blob/master/lean/commands/cloud/live.py)_
-
-### `lean cloud optimize`
-
-Optimize a project in the cloud.
-
-```
-Usage: lean cloud optimize [OPTIONS] PROJECT
-
-  Optimize a project in the cloud.
-
-  PROJECT must be the name or id of the project to optimize.
-
-  An interactive prompt will be shown to configure the optimizer. If --target is given the command runs in non-
-  interactive mode. In this mode the CLI does not prompt for input and the following options become required:
-  --target, --target-direction, --parameter, --node and --parallel-nodes.
-
-  In non-interactive mode the --parameter option can be provided multiple times to configure multiple parameters:
-  - --parameter <name> <min value> <max value> <step size>
-  - --parameter my-first-parameter 1 10 0.5 --parameter my-second-parameter 20 30 5
-
-  In non-interactive mode the --constraint option can be provided multiple times to configure multiple constraints:
-  - --constraint "<statistic> <operator> <value>"
-  - --constraint "Sharpe Ratio >= 0.5" --constraint "Drawdown < 0.25"
-
-  If the project that has to be optimized has been pulled to the local drive with `lean cloud pull` it is possible to
-  use the --push option to push local modifications to the cloud before running the optimization.
-
-Options:
-  --target TEXT                   The target statistic of the optimization
-  --target-direction [min|max]    Whether the target must be minimized or maximized
-  --parameter <TEXT FLOAT FLOAT FLOAT>...
-                                  The 'parameter min max step' pairs configuring the parameters to optimize
-  --constraint TEXT               The 'statistic operator value' pairs configuring the constraints of the optimization
-  --node [O2-8|O4-12|O8-16]       The node type to run the optimization on
-  --parallel-nodes INTEGER        The number of nodes that may be run in parallel
-  --name TEXT                     The name of the optimization (a random one is generated if not specified)
-  --push                          Push local modifications to the cloud before starting the optimization
-  --verbose                       Enable debug logging
-  --help                          Show this message and exit.
-```
-
-_See code: [lean/commands/cloud/optimize.py](https://github.com/QuantConnect/lean-cli/blob/master/lean/commands/cloud/optimize.py)_
-
-### `lean cloud pull`
-
-Pull projects from QuantConnect to the local drive.
-
-```
-Usage: lean cloud pull [OPTIONS]
-
-  Pull projects from QuantConnect to the local drive.
-
-  This command overrides the content of local files with the content of their respective counterparts in the cloud.
-
-  This command will not delete local files for which there is no counterpart in the cloud.
-
-Options:
-  --project TEXT   Name or id of the project to pull (all cloud projects if not specified)
-  --pull-bootcamp  Pull Boot Camp projects (disabled by default)
-  --verbose        Enable debug logging
-  --help           Show this message and exit.
-```
-
-_See code: [lean/commands/cloud/pull.py](https://github.com/QuantConnect/lean-cli/blob/master/lean/commands/cloud/pull.py)_
-
-### `lean cloud push`
-
-Push local projects to QuantConnect.
-
-```
-Usage: lean cloud push [OPTIONS]
-
-  Push local projects to QuantConnect.
-
-  This command overrides the content of cloud files with the content of their respective local counterparts.
-
-  This command will not delete cloud files which don't have a local counterpart.
-
-Options:
-  --project DIRECTORY  Path to the local project to push (all local projects if not specified)
-  --verbose            Enable debug logging
-  --help               Show this message and exit.
-```
-
-_See code: [lean/commands/cloud/push.py](https://github.com/QuantConnect/lean-cli/blob/master/lean/commands/cloud/push.py)_
-
-### `lean cloud status`
-
-Show the live trading status of a project in the cloud.
-
-```
-Usage: lean cloud status [OPTIONS] PROJECT
-
-  Show the live trading status of a project in the cloud.
-
-  PROJECT must be the name or the id of the project to show the status for.
-
-Options:
-  --verbose  Enable debug logging
-  --help     Show this message and exit.
-```
-
-_See code: [lean/commands/cloud/status.py](https://github.com/QuantConnect/lean-cli/blob/master/lean/commands/cloud/status.py)_
-
-### `lean config get`
-
-Get the current value of a configurable option.
-
-```
-Usage: lean config get [OPTIONS] KEY
-
-  Get the current value of a configurable option.
-
-  Sensitive options like credentials cannot be retrieved this way for security reasons. Please open
-  ~/.lean/credentials if you want to see your currently stored credentials.
-
-  Run `lean config list` to show all available options.
-
-Options:
-  --verbose  Enable debug logging
-  --help     Show this message and exit.
-```
-
-_See code: [lean/commands/config/get.py](https://github.com/QuantConnect/lean-cli/blob/master/lean/commands/config/get.py)_
-
-### `lean config list`
-
-List the configurable options and their current values.
-
-```
-Usage: lean config list [OPTIONS]
-
-  List the configurable options and their current values.
-
-Options:
-  --verbose  Enable debug logging
-  --help     Show this message and exit.
-```
-
-_See code: [lean/commands/config/list.py](https://github.com/QuantConnect/lean-cli/blob/master/lean/commands/config/list.py)_
-
-### `lean config set`
-
-Set a configurable option.
-
-```
-Usage: lean config set [OPTIONS] KEY VALUE
-
-  Set a configurable option.
-
-  Run `lean config list` to show all available options.
-
-Options:
-  --verbose  Enable debug logging
-  --help     Show this message and exit.
-```
-
-_See code: [lean/commands/config/set.py](https://github.com/QuantConnect/lean-cli/blob/master/lean/commands/config/set.py)_
-
-### `lean config unset`
-
-Unset a configurable option.
-
-```
-Usage: lean config unset [OPTIONS] KEY
-
-  Unset a configurable option.
-
-  Run `lean config list` to show all available options.
-
-Options:
-  --verbose  Enable debug logging
-  --help     Show this message and exit.
-```
-
-_See code: [lean/commands/config/unset.py](https://github.com/QuantConnect/lean-cli/blob/master/lean/commands/config/unset.py)_
-
-### `lean create-project`
-
-Create a new project containing starter code.
-
-```
-Usage: lean create-project [OPTIONS] NAME
-
-  Create a new project containing starter code.
-
-  If NAME is a path containing subdirectories those will be created automatically.
-
-  The default language can be set using `lean config set default-language python/csharp`.
-
-Options:
-  -l, --language [python|csharp]  The language of the project to create
-  --verbose                       Enable debug logging
-  --help                          Show this message and exit.
-```
-
-_See code: [lean/commands/create_project.py](https://github.com/QuantConnect/lean-cli/blob/master/lean/commands/create_project.py)_
-
-### `lean data download`
-
-Purchase and download data from QuantConnect Datasets.
-
-```
-Usage: lean data download [OPTIONS]
-
-  Purchase and download data from QuantConnect Datasets.
-
-  An interactive wizard will show to walk you through the process of selecting data, accepting the CLI API Access and
-  Data Agreement and payment. After this wizard the selected data will be downloaded automatically.
-
-  If --dataset is given the command runs in non-interactive mode. In this mode the CLI does not prompt for input or
-  confirmation but only halts when the agreement must be accepted. In non-interactive mode all options specific to the
-  selected dataset as well as --organization are required.
-
-  See the following url for the data that can be purchased and downloaded with this command:
-  https://www.quantconnect.com/datasets
-
-Options:
-  --dataset TEXT       The name of the dataset to download non-interactively
-  --organization TEXT  The name or id of the organization to purchase and download data with
-  --overwrite          Overwrite existing local data
-  --lean-config FILE   The Lean configuration file that should be used (defaults to the nearest lean.json)
-  --verbose            Enable debug logging
-  --help               Show this message and exit.
-```
-
-_See code: [lean/commands/data/download.py](https://github.com/QuantConnect/lean-cli/blob/master/lean/commands/data/download.py)_
-
-### `lean data generate`
-
-Generate random market data.
-
-```
-Usage: lean data generate [OPTIONS]
-
-  Generate random market data.
-
-  This uses the random data generator in LEAN to generate realistic market data using a Brownian motion model.
-  This generator supports the following security types, tick types and resolutions:
-  | Security type | Generated tick types | Supported resolutions                |
-  | ------------- | -------------------- | ------------------------------------ |
-  | Equity        | Trade                | Tick, Second, Minute, Hour and Daily |
-  | Forex         | Quote                | Tick, Second, Minute, Hour and Daily |
-  | CFD           | Quote                | Tick, Second, Minute, Hour and Daily |
-  | Future        | Trade and Quote      | Tick, Second, Minute, Hour and Daily |
-  | Crypto        | Trade and Quote      | Tick, Second, Minute, Hour and Daily |
-  | Option        | Trade and Quote      | Minute                               |
-
-  The following data densities are available:
-  - Dense: at least one data point per resolution step.
-  - Sparse: at least one data point per 5 resolution steps.
-  - VerySparse: at least one data point per 50 resolution steps.
-
-  Example which generates minute data for 100 equity symbols since 2015-01-01:
-  $ lean data generate --start=20150101 --symbol-count=100
-
-  Example which generates daily data for 100 crypto symbols since 2015-01-01:
-  $ lean data generate --start=20150101 --symbol-count=100 --security-type=Crypto --resolution=Daily
-
-  By default the official LEAN engine image is used. You can override this using the --image option. Alternatively you
-  can set the default engine image for all commands using `lean config set engine-image <image>`.
-
-Options:
-  --start [yyyyMMdd]              Start date for the data to generate in yyyyMMdd format  [required]
-  --end [yyyyMMdd]                End date for the data to generate in yyyyMMdd format (defaults to today)
-  --symbol-count INTEGER RANGE    The number of symbols to generate data for  [required]
-  --security-type [Equity|Forex|Cfd|Future|Crypto|Option]
-                                  The security type to generate data for (defaults to Equity)
-  --resolution [Tick|Second|Minute|Hour|Daily]
-                                  The resolution of the generated data (defaults to Minute)
-  --data-density [Dense|Sparse|VerySparse]
-                                  The density of the generated data (defaults to Dense)
-  --include-coarse BOOLEAN        Whether coarse universe data should be generated for Equity data (defaults to True)
-  --market TEXT                   The market to generate data for (defaults to standard market for the security type)
-  --image TEXT                    The LEAN engine image to use (defaults to quantconnect/lean:latest)
-  --update                        Pull the LEAN engine image before running the generator
-  --lean-config FILE              The Lean configuration file that should be used (defaults to the nearest lean.json)
-  --verbose                       Enable debug logging
-  --help                          Show this message and exit.
-```
-
-_See code: [lean/commands/data/generate.py](https://github.com/QuantConnect/lean-cli/blob/master/lean/commands/data/generate.py)_
-
-### `lean gui logs`
-
-See the logs of the local GUI.
-
-```
-Usage: lean gui logs [OPTIONS]
-
-  See the logs of the local GUI.
-
-Options:
-  -f, --follow  Update the logs in real-time while the GUI is running
-  --verbose     Enable debug logging
-  --help        Show this message and exit.
-```
-
-_See code: [lean/commands/gui/logs.py](https://github.com/QuantConnect/lean-cli/blob/master/lean/commands/gui/logs.py)_
-
-### `lean gui restart`
-
-Restart the local GUI and open it in the browser.
-
-```
-Usage: lean gui restart [OPTIONS]
-
-  Restart the local GUI and open it in the browser.
-
-Options:
-  --no-open  Skip opening the local GUI in the browser after restarting it
-  --verbose  Enable debug logging
-  --help     Show this message and exit.
-```
-
-_See code: [lean/commands/gui/restart.py](https://github.com/QuantConnect/lean-cli/blob/master/lean/commands/gui/restart.py)_
-
-### `lean gui start`
-
-Start the local GUI.
-
-```
-Usage: lean gui start [OPTIONS]
-
-  Start the local GUI.
-
-Options:
-  --organization TEXT  The name or id of the organization with the local GUI module subscription
-  --port INTEGER       The port to run the local GUI on (defaults to 5612)
-  --no-open            Skip opening the local GUI in the browser after starting it
-  --shortcut           Create a desktop shortcut for launching the local GUI
-  --lean-config FILE   The Lean configuration file that should be used (defaults to the nearest lean.json)
-  --verbose            Enable debug logging
-  --help               Show this message and exit.
-```
-
-_See code: [lean/commands/gui/start.py](https://github.com/QuantConnect/lean-cli/blob/master/lean/commands/gui/start.py)_
-
-### `lean gui stop`
-
-Stop the local GUI.
-
-```
-Usage: lean gui stop [OPTIONS]
-
-  Stop the local GUI.
-
-Options:
-  --verbose  Enable debug logging
-  --help     Show this message and exit.
-```
-
-_See code: [lean/commands/gui/stop.py](https://github.com/QuantConnect/lean-cli/blob/master/lean/commands/gui/stop.py)_
-
-### `lean init`
-
-Scaffold a Lean configuration file and data directory.
-
-```
-Usage: lean init [OPTIONS]
-
-  Scaffold a Lean configuration file and data directory.
-
-Options:
-  --verbose  Enable debug logging
-  --help     Show this message and exit.
-```
-
-_See code: [lean/commands/init.py](https://github.com/QuantConnect/lean-cli/blob/master/lean/commands/init.py)_
-
-### `lean library add`
-
-Add a custom library to a project.
-
-```
-Usage: lean library add [OPTIONS] PROJECT NAME
-
-  Add a custom library to a project.
-
-  PROJECT must be the path to the project.
-
-  NAME must be the name of a NuGet package (for C# projects) or of a PyPI package (for Python projects).
-
-  If --version is not given, the package is pinned to the latest compatible version. For C# projects, this is the
-  latest available version. For Python projects, this is the latest version compatible with Python 3.6 (which is what
-  the Docker images use).
-
-  Custom C# libraries are added to your project's .csproj file, which is then restored if dotnet is on your PATH and
-  the --no-local flag has not been given.
-
-  Custom Python libraries are added to your project's requirements.txt file and are installed in your local Python
-  environment so you get local autocomplete for the library. The last step can be skipped with the --no-local flag.
-
-  C# example usage:
-  $ lean library add "My CSharp Project" Microsoft.ML
-  $ lean library add "My CSharp Project" Microsoft.ML --version 1.5.5
-
-  Python example usage:
-  $ lean library add "My Python Project" tensorflow
-  $ lean library add "My Python Project" tensorflow --version 2.5.0
-
-Options:
-  --version TEXT  The version of the library to add (defaults to latest compatible version)
-  --no-local      Skip making changes to your local environment
-  --verbose       Enable debug logging
-  --help          Show this message and exit.
-```
-
-_See code: [lean/commands/library/add.py](https://github.com/QuantConnect/lean-cli/blob/master/lean/commands/library/add.py)_
-
-### `lean library remove`
-
-Remove a custom library from a project.
-
-```
-Usage: lean library remove [OPTIONS] PROJECT NAME
-
-  Remove a custom library from a project.
-
-  PROJECT must be the path to the project directory.
-
-  NAME must be the name of the NuGet package (for C# projects) or of the PyPI package (for Python projects) to remove.
-
-  Custom C# libraries are removed from the project's .csproj file, which is then restored if dotnet is on your PATH
-  and the --no-local flag has not been given.
-
-  Custom Python libraries are removed from the project's requirements.txt file.
-
-  C# example usage:
-  $ lean library remove "My CSharp Project" Microsoft.ML
-
-  Python example usage:
-  $ lean library remove "My Python Project" tensorflow
-
-Options:
-  --no-local  Skip making changes to your local environment
-  --verbose   Enable debug logging
-  --help      Show this message and exit.
-```
-
-_See code: [lean/commands/library/remove.py](https://github.com/QuantConnect/lean-cli/blob/master/lean/commands/library/remove.py)_
-
-### `lean live`
-
-Start live trading a project locally using Docker.
-
-```
-Usage: lean live [OPTIONS] PROJECT
-
-  Start live trading a project locally using Docker.
-
-  If PROJECT is a directory, the algorithm in the main.py or Main.cs file inside it will be executed.
-  If PROJECT is a file, the algorithm in the specified file will be executed.
-
-  By default an interactive wizard is shown letting you configure the brokerage and data feed to use. If
-  --environment, --brokerage or --data-feed are given the command runs in non-interactive mode. In this mode the CLI
-  does not prompt for input.
-
-  If --environment is given it must be the name of a live environment in the Lean configuration.
-
-  If --brokerage and --data-feed are given, the options specific to the given brokerage/data feed must also be given.
-  The Lean config is used as fallback when a brokerage/data feed-specific option hasn't been passed in. If a required
-  option is not given and cannot be found in the Lean config the command aborts.
-
-  By default the official LEAN engine image is used. You can override this using the --image option. Alternatively you
-  can set the default engine image for all commands using `lean config set engine-image <image>`.
-
-Options:
-  --environment TEXT              The environment to use
-  --output DIRECTORY              Directory to store results in (defaults to PROJECT/live/TIMESTAMP)
-  -d, --detach                    Run the live deployment in a detached Docker container and return immediately
-  --gui                           Enable monitoring and controlling of the deployment via the local GUI
-  --gui-organization TEXT         The name or id of the organization with the local GUI module subscription
-  --brokerage [Paper Trading|Interactive Brokers|Tradier|Oanda|Bitfinex|Coinbase Pro|Binance|Zerodha|Samco|Terminal Link|Atreyu|Trading Technologies|Kraken|FTX]
-                                  The brokerage to use
-  --data-feed [Interactive Brokers|Tradier|Oanda|Bitfinex|Coinbase Pro|Binance|Zerodha|Samco|Terminal Link|Trading Technologies|Kraken|FTX|IQFeed|Custom data only]
-                                  The data feed to use
-  --ib-organization TEXT          The name or id of the organization with the Interactive Brokers module subscription
-  --ib-user-name TEXT             Your Interactive Brokers username
-  --ib-account TEXT               Your Interactive Brokers account id
-  --ib-password TEXT              Your Interactive Brokers password
-  --ib-enable-delayed-streaming-data BOOLEAN
-                                  Whether delayed data may be used when your algorithm subscribes to a security you
-                                  don't have a market data subscription for
-
-  --tradier-account-id TEXT       Your Tradier account id
-  --tradier-access-token TEXT     Your Tradier access token
-  --tradier-environment [live|paper]
-                                  Whether the developer sandbox should be used
-  --oanda-environment [Practice|Trade]
-                                  The environment to run in, Practice for fxTrade Practice, Trade for fxTrade
-  --oanda-account-id TEXT         Your OANDA account id
-  --oanda-access-token TEXT       Your OANDA API token
-  --bitfinex-api-key TEXT         Your Bitfinex API key
-  --bitfinex-api-secret TEXT      Your Bitfinex API secret
-  --gdax-use-sandbox [live|paper]
-                                  Whether the sandbox should be used
-  --gdax-api-key TEXT             Your Coinbase Pro API key
-  --gdax-api-secret TEXT          Your Coinbase Pro API secret
-  --gdax-passphrase TEXT          Your Coinbase Pro API passphrase
-  --binance-use-testnet [live|paper]
-                                  Whether the testnet should be used
-  --binance-organization TEXT     The name or id of the organization with the Binance module subscription
-  --binance-api-key TEXT          Your Binance API key
-  --binance-api-secret TEXT       Your Binance API secret
-  --zerodha-organization TEXT     The name or id of the organization with the zerodha module subscription
-  --zerodha-api-key TEXT          Your Kite Connect API key
-  --zerodha-access-token TEXT     Your Kite Connect access token
-  --zerodha-product-type [MIS|CNC|NRML]
-                                  MIS if you are targeting intraday products, CNC if you are targeting delivery
-                                  products, NRML if you are targeting carry forward products
-
-  --zerodha-trading-segment [EQUITY|COMMODITY]
-                                  EQUITY if you are trading equities on NSE or BSE, COMMODITY if you are trading
-                                  commodities on MCX
-
-  --zerodha-history-subscription BOOLEAN
-                                  Whether you have a history API subscription for Zerodha
-  --samco-organization TEXT       The name or id of the organization with the samco module subscription
-  --samco-client-id TEXT          Your Samco account Client ID
-  --samco-client-password TEXT    Your Samco account password
-  --samco-year-of-birth TEXT      Your year of birth (YYYY) registered with Samco
-  --samco-product-type [MIS|CNC|NRML]
-                                  MIS if you are targeting intraday products, CNC if you are targeting delivery
-                                  products, NRML if you are targeting carry forward products
-
-  --samco-trading-segment [EQUITY|COMMODITY]
-                                  EQUITY if you are trading equities on NSE or BSE, COMMODITY if you are trading
-                                  commodities on MCX
-
-  --terminal-link-organization TEXT
-                                  The name or id of the organization with the Terminal Link module subscription
-  --bloomberg-environment [Production|Beta]
-                                  The environment to run in
-  --bloomberg-server-host TEXT    The host of the Bloomberg server
-  --bloomberg-server-port INTEGER
-                                  The port of the Bloomberg server
-  --bloomberg-symbol-map-file FILE
-                                  The path to the Bloomberg symbol map file
-  --bloomberg-emsx-broker TEXT    The EMSX broker to use
-  --bloomberg-emsx-user-time-zone TEXT
-                                  The EMSX user timezone to use
-  --bloomberg-emsx-account TEXT   The EMSX account to use
-  --bloomberg-emsx-strategy TEXT  The EMSX strategy to use
-  --bloomberg-emsx-notes TEXT     The EMSX notes to use
-  --bloomberg-emsx-handling TEXT  The EMSX handling to use
-  --bloomberg-allow-modification BOOLEAN
-                                  Whether modification is allowed
-  --atreyu-organization TEXT      The name or id of the organization with the Atreyu module subscription
-  --atreyu-host TEXT              The host of the Atreyu server
-  --atreyu-req-port INTEGER       The Atreyu request port
-  --atreyu-sub-port INTEGER       The Atreyu subscribe port
-  --atreyu-username TEXT          Your Atreyu username
-  --atreyu-password TEXT          Your Atreyu password
-  --atreyu-client-id TEXT         Your Atreyu client id
-  --atreyu-broker-mpid TEXT       The broker MPID to use
-  --atreyu-locate-rqd TEXT        The locate rqd to use
-  --tt-organization TEXT          The name or id of the organization with the Trading Technologies module subscription
-  --tt-user-name TEXT             Your Trading Technologies username
-  --tt-session-password TEXT      Your Trading Technologies session password
-  --tt-account-name TEXT          Your Trading Technologies account name
-  --tt-rest-app-key TEXT          Your Trading Technologies REST app key
-  --tt-rest-app-secret TEXT       Your Trading Technologies REST app secret
-  --tt-rest-environment TEXT      The REST environment to run in
-  --tt-market-data-sender-comp-id TEXT
-                                  The market data sender comp id to use
-  --tt-market-data-target-comp-id TEXT
-                                  The market data target comp id to use
-  --tt-market-data-host TEXT      The host of the market data server
-  --tt-market-data-port TEXT      The port of the market data server
-  --tt-order-routing-sender-comp-id TEXT
-                                  The order routing sender comp id to use
-  --tt-order-routing-target-comp-id TEXT
-                                  The order routing target comp id to use
-  --tt-order-routing-host TEXT    The host of the order routing server
-  --tt-order-routing-port TEXT    The port of the order routing server
-  --tt-log-fix-messages BOOLEAN   Whether FIX messages should be logged
-  --kraken-organization TEXT      The name or id of the organization with the kraken module subscription
-  --kraken-api-key TEXT           Your Kraken API key
-  --kraken-api-secret TEXT        Your Kraken API secret
-  --kraken-verification-tier [Starter|Intermediate|Pro]
-                                  Your Kraken Verification Tier
-  --ftx-exchange-name [FTX|FTXUS]
-                                  FTX exchange name [FTX, FTXUS]
-  --ftx-organization TEXT         The name or id of the organization with the FTX module subscription
-  --ftx-api-key TEXT              Your FTX API key
-  --ftxus-api-key TEXT            Your FTX API key
-  --ftx-api-secret TEXT           Your FTX API secret
-  --ftxus-api-secret TEXT         Your FTX API secret
-  --ftx-account-tier [Tier1|Tier2|Tier3|Tier4|Tier5|Tier6]
-                                  Your FTX Account Tier
-  --ftxus-account-tier [Tier1|Tier2|Tier3|Tier4|Tier5|Tier6]
-                                  Your FTX Account Tier
-  --iqfeed-iqconnect FILE         The path to the IQConnect binary
-  --iqfeed-username TEXT          Your IQFeed username
-  --iqfeed-password TEXT          Your IQFeed password
-  --iqfeed-productName TEXT       The product name of your IQFeed developer account
-  --iqfeed-version TEXT           The product version of your IQFeed developer account
-  --release                       Compile C# projects in release configuration instead of debug
-  --image TEXT                    The LEAN engine image to use (defaults to quantconnect/lean:latest)
-  --update                        Pull the LEAN engine image before starting live trading
-  --lean-config FILE              The Lean configuration file that should be used (defaults to the nearest lean.json)
-  --verbose                       Enable debug logging
-  --help                          Show this message and exit.
-```
-
-_See code: [lean/commands/live.py](https://github.com/QuantConnect/lean-cli/blob/master/lean/commands/live.py)_
-
-### `lean login`
-
-Log in with a QuantConnect account.
-
-```
-Usage: lean login [OPTIONS]
-
-  Log in with a QuantConnect account.
-
-  If user id or API token is not provided an interactive prompt will show.
-
-  Credentials are stored in ~/.lean/credentials and are removed upon running `lean logout`.
-
-Options:
-  -u, --user-id TEXT    QuantConnect user id
-  -t, --api-token TEXT  QuantConnect API token
-  --verbose             Enable debug logging
-  --help                Show this message and exit.
-```
-
-_See code: [lean/commands/login.py](https://github.com/QuantConnect/lean-cli/blob/master/lean/commands/login.py)_
-
-### `lean logout`
-
-Log out and remove stored credentials.
-
-```
-Usage: lean logout [OPTIONS]
-
-  Log out and remove stored credentials.
-
-Options:
-  --verbose  Enable debug logging
-  --help     Show this message and exit.
-```
-
-_See code: [lean/commands/logout.py](https://github.com/QuantConnect/lean-cli/blob/master/lean/commands/logout.py)_
-
-### `lean logs`
-
-Display the most recent backtest/live/optimization logs.
-
-```
-Usage: lean logs [OPTIONS]
-
-  Display the most recent backtest/live/optimization logs.
-
-Options:
-  --backtest           Display the most recent backtest logs (default)
-  --live               Display the most recent live logs
-  --optimization       Display the most recent optimization logs
-  --project DIRECTORY  The project to get the most recent logs from
-  --lean-config FILE   The Lean configuration file that should be used (defaults to the nearest lean.json)
-  --verbose            Enable debug logging
-  --help               Show this message and exit.
-```
-
-_See code: [lean/commands/logs.py](https://github.com/QuantConnect/lean-cli/blob/master/lean/commands/logs.py)_
-
-### `lean optimize`
-
-Optimize a project's parameters locally using Docker.
-
-```
-Usage: lean optimize [OPTIONS] PROJECT
-
-  Optimize a project's parameters locally using Docker.
-
-  If PROJECT is a directory, the algorithm in the main.py or Main.cs file inside it will be executed.
-  If PROJECT is a file, the algorithm in the specified file will be executed.
-
-  By default an interactive wizard is shown letting you configure the optimizer. If --optimizer-config or --strategy
-  is given the command runs in non-interactive mode. In this mode the CLI does not prompt for input.
-
-  The --optimizer-config option can be used to specify the configuration to run the optimizer with.
-  When using the option it should point to a file like this (the algorithm-* properties should be omitted):
-  https://github.com/QuantConnect/Lean/blob/master/Optimizer.Launcher/config.json
-
-  If --strategy is given the optimizer configuration is read from the given options. In this case --strategy,
-  --target, --target-direction and --parameter become required.
-
-  In non-interactive mode the --parameter option can be provided multiple times to configure multiple parameters:
-  - --parameter <name> <min value> <max value> <step size>
-  - --parameter my-first-parameter 1 10 0.5 --parameter my-second-parameter 20 30 5
-
-  In non-interactive mode the --constraint option can be provided multiple times to configure multiple constraints:
-  - --constraint "<statistic> <operator> <value>"
-  - --constraint "Sharpe Ratio >= 0.5" --constraint "Drawdown < 0.25"
-
-  By default the official LEAN engine image is used. You can override this using the --image option. Alternatively you
-  can set the default engine image for all commands using `lean config set engine-image <image>`.
-
-Options:
-  --output DIRECTORY              Directory to store results in (defaults to PROJECT/optimizations/TIMESTAMP)
-  -d, --detach                    Run the optimization in a detached Docker container and return immediately
-  --optimizer-config FILE         The optimizer configuration file that should be used
-  --strategy [Grid Search|Euler Search]
-                                  The optimization strategy to use
-  --target TEXT                   The target statistic of the optimization
-  --target-direction [min|max]    Whether the target must be minimized or maximized
-  --parameter <TEXT FLOAT FLOAT FLOAT>...
-                                  The 'parameter min max step' pairs configuring the parameters to optimize
-  --constraint TEXT               The 'statistic operator value' pairs configuring the constraints of the optimization
-  --release                       Compile C# projects in release configuration instead of debug
-  --image TEXT                    The LEAN engine image to use (defaults to quantconnect/lean:latest)
-  --update                        Pull the LEAN engine image before running the optimizer
-  --lean-config FILE              The Lean configuration file that should be used (defaults to the nearest lean.json)
-  --verbose                       Enable debug logging
-  --help                          Show this message and exit.
-```
-
-_See code: [lean/commands/optimize.py](https://github.com/QuantConnect/lean-cli/blob/master/lean/commands/optimize.py)_
-
-### `lean report`
-
-Generate a report of a backtest.
-
-```
-Usage: lean report [OPTIONS]
-
-  Generate a report of a backtest.
-
-  This runs the LEAN Report Creator in Docker to generate a polished, professional-grade report of a backtest.
-
-  If --backtest-results is not given, a report is generated for the most recent local backtest.
-
-  The name, description, and version are optional and will be blank if not given.
-
-  If the given backtest data source file is stored in a project directory (or one of its subdirectories, like the
-  default <project>/backtests/<timestamp>), the default name is the name of the project directory and the default
-  description is the description stored in the project's config.json file.
-
-  By default the official LEAN engine image is used. You can override this using the --image option. Alternatively you
-  can set the default engine image for all commands using `lean config set engine-image <image>`.
-
-Options:
-  --backtest-results FILE      Path to the JSON file containing the backtest results
-  --live-results FILE          Path to the JSON file containing the live trading results
-  --report-destination FILE    Path where the generated report is stored as HTML (defaults to ./report.html)
-  -d, --detach                 Run the report creator in a detached Docker container and return immediately
-  --strategy-name TEXT         Name of the strategy, will appear at the top-right corner of each page
-  --strategy-version TEXT      Version number of the strategy, will appear next to the project name
-  --strategy-description TEXT  Description of the strategy, will appear under the 'Strategy Description' section
-  --overwrite                  Overwrite --report-destination if it already contains a file
-  --image TEXT                 The LEAN engine image to use (defaults to quantconnect/lean:latest)
-  --update                     Pull the LEAN engine image before running the report creator
-  --lean-config FILE           The Lean configuration file that should be used (defaults to the nearest lean.json)
-  --verbose                    Enable debug logging
-  --help                       Show this message and exit.
-```
-
-_See code: [lean/commands/report.py](https://github.com/QuantConnect/lean-cli/blob/master/lean/commands/report.py)_
-
-### `lean research`
-
-Run a Jupyter Lab environment locally using Docker.
-
-```
-Usage: lean research [OPTIONS] PROJECT
-
-  Run a Jupyter Lab environment locally using Docker.
-
-  By default the official LEAN research image is used. You can override this using the --image option. Alternatively
-  you can set the default research image using `lean config set research-image <image>`.
-
-Options:
-  --port INTEGER                  The port to run Jupyter Lab on (defaults to 8888)
-  --data-provider [Terminal Link|QuantConnect|Local]
-                                  Update the Lean configuration file to retrieve data from the given provider
-  --download-data                 Update the Lean configuration file to download data from the QuantConnect API, alias
-                                  for --data-provider QuantConnect
-
-  --data-purchase-limit INTEGER   The maximum amount of QCC to spend on downloading data during the research session
-                                  when using QuantConnect as data provider
-
-  -d, --detach                    Run Jupyter Lab in a detached Docker container and return immediately
-  --no-open                       Don't open the Jupyter Lab environment in the browser after starting it
-  --image TEXT                    The LEAN research image to use (defaults to quantconnect/research:latest)
-  --update                        Pull the LEAN research image before starting the research environment
-  --lean-config FILE              The Lean configuration file that should be used (defaults to the nearest lean.json)
-  --verbose                       Enable debug logging
-  --help                          Show this message and exit.
-```
-
-_See code: [lean/commands/research.py](https://github.com/QuantConnect/lean-cli/blob/master/lean/commands/research.py)_
-
-### `lean whoami`
-
-Display who is logged in.
-
-```
-Usage: lean whoami [OPTIONS]
-
-  Display who is logged in.
-
-Options:
-  --verbose  Enable debug logging
-  --help     Show this message and exit.
-```
-
-_See code: [lean/commands/whoami.py](https://github.com/QuantConnect/lean-cli/blob/master/lean/commands/whoami.py)_
-<!-- commands end -->
-
-## Development
-
-To work on the Lean CLI, clone the repository, enter an environment containing Python 3.6+ and run `pip install -r requirements.txt`. This command will install the required dependencies and installs the CLI in editable mode. This means you'll be able to edit the code and immediately see the results the next time you run `lean`.
-
-If you need to add dependencies, first update `setup.py` (if it is a production dependency) or `requirements.txt` (if it is a development dependency) and then re-run `pip install -r requirements.txt`.
-
-The automated tests can be ran by running `pytest`. The filesystem and HTTP requests are mocked when running tests to make sure they run in an isolated environment.
-
-Can build the lean CLI by running `python setup.py sdist bdist_wheel` from the root of the project and to install it `pip install --force-reinstall dist/lean-dev-py3-none-any.whl`. To update the commands reference part of the readme run `python scripts/readme.py` from the root of the project, after installing the new version.
-
-Maintainers can publish new releases by pushing a Git tag containing the new version to GitHub. This will trigger a GitHub Actions workflow which releases the current `master` branch to PyPI with the value of the tag as version. Make sure the version is not prefixed with "v".
+Metadata-Version: 2.1
+Name: ablean
+Version: 1.3.8
+Summary: A CLI aimed at making it easier to run QuantConnect's LEAN engine locally and in the cloud
+Home-page: https://lean.io/cli
+Author: abl
+Author-email: support@quantconnect.com
+Project-URL: Documentation, https://www.lean.io/docs/lean-cli/key-concepts/getting-started
+Project-URL: Source, https://github.com/QuantConnect/lean-cli
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Financial and Insurance Industry
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Requires-Python: >= 3.8
+Description-Content-Type: text/markdown
+
+![Lean CLI](http://cdn.quantconnect.com.s3.us-east-1.amazonaws.com/i/github/lean-cli-splash.png)
+
+# QuantConnect Lean CLI
+ 
+[![Build Status](https://github.com/QuantConnect/lean-cli/workflows/Build/badge.svg)](https://github.com/QuantConnect/lean-cli/actions?query=workflow%3ABuild)
+[![PyPI Version](https://img.shields.io/pypi/v/lean)](https://pypi.org/project/lean/)
+[![Project Status](https://img.shields.io/pypi/status/lean)](https://pypi.org/project/lean/)
+
+The Lean CLI is a cross-platform CLI aimed at making it easier to develop with the LEAN engine locally and in the cloud.
+
+Visit the [documentation website](https://www.lean.io/docs/lean-cli/key-concepts/getting-started) for comprehensive and up-to-date documentation.
+
+## Highlights
+
+- [Project scaffolding](https://www.lean.io/docs/lean-cli/projects/project-management)
+- [Local autocomplete](https://www.lean.io/docs/lean-cli/projects/autocomplete)
+- [Local data downloading](https://www.lean.io/docs/lean-cli/datasets/downloading-quantconnect-data)
+- [Local backtesting](https://www.lean.io/docs/lean-cli/backtesting/deployment#02-Run-Local-Backtests)
+- [Local debugging](https://www.lean.io/docs/lean-cli/backtesting/debugging)
+- [Local research environment](https://www.lean.io/docs/lean-cli/research)
+- [Local optimization](https://www.lean.io/docs/lean-cli/optimization/deployment#02-Run-Local-Optimizations)
+- [Local live trading](https://www.lean.io/docs/lean-cli/live-trading/quantconnect-paper-trading#02-Deploy-Local-Algorithms)
+- [Local backtest report creation](https://www.lean.io/docs/lean-cli/backtesting/report#02-Generate-a-Report)
+- [Cloud synchronization](https://www.lean.io/docs/lean-cli/projects/cloud-synchronization)
+- [Cloud backtesting](https://www.lean.io/docs/lean-cli/backtesting/deployment#03-Run-Cloud-Backtests)
+- [Cloud optimization](https://www.lean.io/docs/lean-cli/optimization/deployment#03-Run-Cloud-Optimizations)
+- [Cloud live trading](https://www.lean.io/docs/lean-cli/live-trading/quantconnect-paper-trading#03-Deploy-Cloud-Algorithms)
+
+## Installation
+
+The CLI can be installed and updated by running `pip install --upgrade lean`.
+
+Note that many commands in the CLI require Docker to run. See [Get Docker](https://docs.docker.com/get-docker/) for instructions on how to install Docker for your operating system.
+
+**Note:** Some Linux users may need to install `tkinter` using the following commands:
+
+``` 
+For Python 3
+
+sudo apt-get install python3-tk
+
+For Python 2.7
+
+sudo apt-get install python-tk
+```
+After installing the CLI, open a terminal in an empty directory and run `lean init`. This command downloads the latest configuration file and sample data from the [QuantConnect/Lean](https://github.com/QuantConnect/Lean) repository. We recommend running all Lean CLI commands in the same directory `lean init` was ran in.
+
+## Usage
+
+The Lean CLI supports multiple workflows. The examples below serve as a starting point, you're free to mix local and cloud features in any way you'd like.
+
+A cloud-focused workflow (local development, cloud execution) with the CLI may look like this:
+1. Open a terminal in the directory you ran `lean init` in.
+2. Run `lean cloud pull` to pull remotely changed files.
+3. Start programming locally and run backtests in the cloud with `lean cloud backtest "Project Name" --open --push` whenever there is something to backtest. The `--open` flag means that the backtest results will be opened in the browser when done, while the `--push` flag means that local changes are pushed to the cloud before running the backtest.
+4. Whenever you want to create a new project, run `lean create-project "Project Name"` and `lean cloud push --project "Project Name"` to create a new project containing some basic code and to push it to the cloud.
+5. When you're finished for the moment, run `lean cloud push` to push all locally changed files to the cloud.
+
+A locally-focused workflow (local development, local execution) with the CLI may look like this:
+1. Open a terminal in the directory you ran `lean init` in.
+2. Run `lean create-project "Project Name"` to create a new project with some basic code to get you started.
+3. Work on your strategy in `./Project Name`.
+4. Run `lean research "Project Name"` to start a Jupyter Lab session to perform research in.
+5. Run `lean backtest "Project Name"` to run a backtest whenever there's something to test. This runs your strategy in a Docker container containing the same packages as the ones used on QuantConnect.com, but with your own data.
+
+## Commands
+
+*Note: the readme only contains the `--help` text of all commands. Visit the [documentation website](https://www.lean.io/docs/lean-cli/key-concepts/getting-started) for more comprehensive documentation.*
+
+<!-- commands start -->
+- [`lean backtest`](#lean-backtest)
+- [`lean build`](#lean-build)
+- [`lean cloud backtest`](#lean-cloud-backtest)
+- [`lean cloud live`](#lean-cloud-live)
+- [`lean cloud optimize`](#lean-cloud-optimize)
+- [`lean cloud pull`](#lean-cloud-pull)
+- [`lean cloud push`](#lean-cloud-push)
+- [`lean cloud status`](#lean-cloud-status)
+- [`lean config get`](#lean-config-get)
+- [`lean config list`](#lean-config-list)
+- [`lean config set`](#lean-config-set)
+- [`lean config unset`](#lean-config-unset)
+- [`lean create-project`](#lean-create-project)
+- [`lean data download`](#lean-data-download)
+- [`lean data generate`](#lean-data-generate)
+- [`lean gui logs`](#lean-gui-logs)
+- [`lean gui restart`](#lean-gui-restart)
+- [`lean gui start`](#lean-gui-start)
+- [`lean gui stop`](#lean-gui-stop)
+- [`lean init`](#lean-init)
+- [`lean library add`](#lean-library-add)
+- [`lean library remove`](#lean-library-remove)
+- [`lean live`](#lean-live)
+- [`lean login`](#lean-login)
+- [`lean logout`](#lean-logout)
+- [`lean logs`](#lean-logs)
+- [`lean optimize`](#lean-optimize)
+- [`lean report`](#lean-report)
+- [`lean research`](#lean-research)
+- [`lean whoami`](#lean-whoami)
+
+### `lean backtest`
+
+Backtest a project locally using Docker.
+
+```
+Usage: lean backtest [OPTIONS] PROJECT
+
+  Backtest a project locally using Docker.
+
+  If PROJECT is a directory, the algorithm in the main.py or Main.cs file inside it will be executed.
+  If PROJECT is a file, the algorithm in the specified file will be executed.
+
+  Go to the following url to learn how to debug backtests locally using the Lean CLI:
+  https://www.lean.io/docs/lean-cli/backtesting/debugging
+
+  By default the official LEAN engine image is used. You can override this using the --image option. Alternatively you
+  can set the default engine image for all commands using `lean config set engine-image <image>`.
+
+Options:
+  --output DIRECTORY              Directory to store results in (defaults to PROJECT/backtests/TIMESTAMP)
+  -d, --detach                    Run the backtest in a detached Docker container and return immediately
+  --debug [pycharm|ptvsd|vsdbg|rider]
+                                  Enable a certain debugging method (see --help for more information)
+  --data-provider [Terminal Link|QuantConnect|Local]
+                                  Update the Lean configuration file to retrieve data from the given provider
+  --download-data                 Update the Lean configuration file to download data from the QuantConnect API, alias
+                                  for --data-provider QuantConnect
+
+  --data-purchase-limit INTEGER   The maximum amount of QCC to spend on downloading data during the backtest when using
+                                  QuantConnect as data provider
+
+  --release                       Compile C# projects in release configuration instead of debug
+  --image TEXT                    The LEAN engine image to use (defaults to quantconnect/lean:latest)
+  --update                        Pull the LEAN engine image before running the backtest
+  --lean-config FILE              The Lean configuration file that should be used (defaults to the nearest lean.json)
+  --verbose                       Enable debug logging
+  --help                          Show this message and exit.
+```
+
+_See code: [lean/commands/backtest.py](https://github.com/QuantConnect/lean-cli/blob/master/lean/commands/backtest.py)_
+
+### `lean build`
+
+Build Docker images of your own version of LEAN and the Alpha Streams SDK.
+
+```
+Usage: lean build [OPTIONS] [ROOT]
+
+  Build Docker images of your own version of LEAN and the Alpha Streams SDK.
+
+  ROOT must point to a directory containing the LEAN repository and the Alpha Streams SDK repository:
+  https://github.com/QuantConnect/Lean & https://github.com/QuantConnect/AlphaStreams
+
+  When ROOT is not given, the current directory is used as root directory.
+
+  This command performs the following actions:
+  1. The lean-cli/foundation:latest image is built from Lean/DockerfileLeanFoundation(ARM).
+  2. LEAN is compiled in a Docker container using the lean-cli/foundation:latest image.
+  3. The Alpha Streams SDK is compiled in a Docker container using the lean-cli/foundation:latest image.
+  4. The lean-cli/engine:latest image is built from Lean/Dockerfile using lean-cli/foundation:latest as base image.
+  5. The lean-cli/research:latest image is built from Lean/DockerfileJupyter using lean-cli/engine:latest as base image.
+  6. The default engine image is set to lean-cli/engine:latest.
+  7. The default research image is set to lean-cli/research:latest.
+
+  When the foundation Dockerfile is the same as the official foundation Dockerfile, quantconnect/lean:foundation is
+  used instead of building a custom foundation image.
+
+Options:
+  --tag TEXT  The tag to apply to custom images (defaults to latest)
+  --verbose   Enable debug logging
+  --help      Show this message and exit.
+```
+
+_See code: [lean/commands/build.py](https://github.com/QuantConnect/lean-cli/blob/master/lean/commands/build.py)_
+
+### `lean cloud backtest`
+
+Backtest a project in the cloud.
+
+```
+Usage: lean cloud backtest [OPTIONS] PROJECT
+
+  Backtest a project in the cloud.
+
+  PROJECT must be the name or id of the project to run a backtest for.
+
+  If the project that has to be backtested has been pulled to the local drive with `lean cloud pull` it is possible to
+  use the --push option to push local modifications to the cloud before running the backtest.
+
+Options:
+  --name TEXT  The name of the backtest (a random one is generated if not specified)
+  --push       Push local modifications to the cloud before running the backtest
+  --open       Automatically open the results in the browser when the backtest is finished
+  --verbose    Enable debug logging
+  --help       Show this message and exit.
+```
+
+_See code: [lean/commands/cloud/backtest.py](https://github.com/QuantConnect/lean-cli/blob/master/lean/commands/cloud/backtest.py)_
+
+### `lean cloud live`
+
+Start live trading for a project in the cloud.
+
+```
+Usage: lean cloud live [OPTIONS] PROJECT
+
+  Start live trading for a project in the cloud.
+
+  PROJECT must be the name or the id of the project to start live trading for.
+
+  By default an interactive wizard is shown letting you configure the deployment. If --brokerage is given the command
+  runs in non-interactive mode. In this mode the CLI does not prompt for input or confirmation. In non-interactive
+  mode the options specific to the given brokerage are required, as well as --node, --auto-restart, --notify-order-
+  events and --notify-insights.
+
+Options:
+  --brokerage [Paper Trading|Interactive Brokers|Tradier|Oanda|Bitfinex|Coinbase Pro|Binance|Zerodha|Samco|Kraken|FTX]
+                                  The brokerage to use
+  --ib-user-name TEXT             Your Interactive Brokers username
+  --ib-account TEXT               Your Interactive Brokers account id
+  --ib-password TEXT              Your Interactive Brokers password
+  --ib-data-feed BOOLEAN          Whether the Interactive Brokers price data feed must be used instead of the
+                                  QuantConnect price data feed
+
+  --tradier-account-id TEXT       Your Tradier account id
+  --tradier-access-token TEXT     Your Tradier access token
+  --tradier-environment [live|paper]
+                                  Whether the developer sandbox should be used
+  --oanda-environment [Practice|Trade]
+                                  The environment to run in, Practice for fxTrade Practice, Trade for fxTrade
+  --oanda-account-id TEXT         Your OANDA account id
+  --oanda-access-token TEXT       Your OANDA API token
+  --bitfinex-api-key TEXT         Your Bitfinex API key
+  --bitfinex-api-secret TEXT      Your Bitfinex API secret
+  --gdax-use-sandbox [live|paper]
+                                  Whether the sandbox should be used
+  --gdax-api-key TEXT             Your Coinbase Pro API key
+  --gdax-api-secret TEXT          Your Coinbase Pro API secret
+  --gdax-passphrase TEXT          Your Coinbase Pro API passphrase
+  --binance-use-testnet [live|paper]
+                                  Whether the testnet should be used
+  --binance-api-key TEXT          Your Binance API key
+  --binance-api-secret TEXT       Your Binance API secret
+  --zerodha-api-key TEXT          Your Kite Connect API key
+  --zerodha-access-token TEXT     Your Kite Connect access token
+  --zerodha-product-type [MIS|CNC|NRML]
+                                  MIS if you are targeting intraday products, CNC if you are targeting delivery
+                                  products, NRML if you are targeting carry forward products
+
+  --zerodha-trading-segment [EQUITY|COMMODITY]
+                                  EQUITY if you are trading equities on NSE or BSE, COMMODITY if you are trading
+                                  commodities on MCX
+
+  --samco-client-id TEXT          Your Samco account Client ID
+  --samco-client-password TEXT    Your Samco account password
+  --samco-year-of-birth TEXT      Your year of birth (YYYY) registered with Samco
+  --samco-product-type [MIS|CNC|NRML]
+                                  MIS if you are targeting intraday products, CNC if you are targeting delivery
+                                  products, NRML if you are targeting carry forward products
+
+  --samco-trading-segment [EQUITY|COMMODITY]
+                                  EQUITY if you are trading equities on NSE or BSE, COMMODITY if you are trading
+                                  commodities on MCX
+
+  --kraken-api-key TEXT           Your Kraken API key
+  --kraken-api-secret TEXT        Your Kraken API secret
+  --kraken-verification-tier [Starter|Intermediate|Pro]
+                                  Your Kraken Verification Tier
+  --ftx-exchange-name [FTX|FTXUS]
+                                  FTX exchange name [FTX, FTXUS]
+  --ftx-api-key TEXT              Your FTX API key
+  --ftxus-api-key TEXT            Your FTX API key
+  --ftx-api-secret TEXT           Your FTX API secret
+  --ftxus-api-secret TEXT         Your FTX API secret
+  --ftx-account-tier [Tier1|Tier2|Tier3|Tier4|Tier5|Tier6]
+                                  Your FTX Account Tier
+  --ftxus-account-tier [Tier1|Tier2|Tier3|Tier4|Tier5|Tier6]
+                                  Your FTX Account Tier
+  --node TEXT                     The name or id of the live node to run on
+  --auto-restart BOOLEAN          Whether automatic algorithm restarting must be enabled
+  --notify-order-events BOOLEAN   Whether notifications must be sent for order events
+  --notify-insights BOOLEAN       Whether notifications must be sent for emitted insights
+  --notify-emails TEXT            A comma-separated list of 'email:subject' pairs configuring email-notifications
+  --notify-webhooks TEXT          A comma-separated list of 'url:HEADER_1=VALUE_1:HEADER_2=VALUE_2:etc' pairs
+                                  configuring webhook-notifications
+
+  --notify-sms TEXT               A comma-separated list of phone numbers configuring SMS-notifications
+  --push                          Push local modifications to the cloud before starting live trading
+  --open                          Automatically open the live results in the browser once the deployment starts
+  --verbose                       Enable debug logging
+  --help                          Show this message and exit.
+```
+
+_See code: [lean/commands/cloud/live.py](https://github.com/QuantConnect/lean-cli/blob/master/lean/commands/cloud/live.py)_
+
+### `lean cloud optimize`
+
+Optimize a project in the cloud.
+
+```
+Usage: lean cloud optimize [OPTIONS] PROJECT
+
+  Optimize a project in the cloud.
+
+  PROJECT must be the name or id of the project to optimize.
+
+  An interactive prompt will be shown to configure the optimizer. If --target is given the command runs in non-
+  interactive mode. In this mode the CLI does not prompt for input and the following options become required:
+  --target, --target-direction, --parameter, --node and --parallel-nodes.
+
+  In non-interactive mode the --parameter option can be provided multiple times to configure multiple parameters:
+  - --parameter <name> <min value> <max value> <step size>
+  - --parameter my-first-parameter 1 10 0.5 --parameter my-second-parameter 20 30 5
+
+  In non-interactive mode the --constraint option can be provided multiple times to configure multiple constraints:
+  - --constraint "<statistic> <operator> <value>"
+  - --constraint "Sharpe Ratio >= 0.5" --constraint "Drawdown < 0.25"
+
+  If the project that has to be optimized has been pulled to the local drive with `lean cloud pull` it is possible to
+  use the --push option to push local modifications to the cloud before running the optimization.
+
+Options:
+  --target TEXT                   The target statistic of the optimization
+  --target-direction [min|max]    Whether the target must be minimized or maximized
+  --parameter <TEXT FLOAT FLOAT FLOAT>...
+                                  The 'parameter min max step' pairs configuring the parameters to optimize
+  --constraint TEXT               The 'statistic operator value' pairs configuring the constraints of the optimization
+  --node [O2-8|O4-12|O8-16]       The node type to run the optimization on
+  --parallel-nodes INTEGER        The number of nodes that may be run in parallel
+  --name TEXT                     The name of the optimization (a random one is generated if not specified)
+  --push                          Push local modifications to the cloud before starting the optimization
+  --verbose                       Enable debug logging
+  --help                          Show this message and exit.
+```
+
+_See code: [lean/commands/cloud/optimize.py](https://github.com/QuantConnect/lean-cli/blob/master/lean/commands/cloud/optimize.py)_
+
+### `lean cloud pull`
+
+Pull projects from QuantConnect to the local drive.
+
+```
+Usage: lean cloud pull [OPTIONS]
+
+  Pull projects from QuantConnect to the local drive.
+
+  This command overrides the content of local files with the content of their respective counterparts in the cloud.
+
+  This command will not delete local files for which there is no counterpart in the cloud.
+
+Options:
+  --project TEXT   Name or id of the project to pull (all cloud projects if not specified)
+  --pull-bootcamp  Pull Boot Camp projects (disabled by default)
+  --verbose        Enable debug logging
+  --help           Show this message and exit.
+```
+
+_See code: [lean/commands/cloud/pull.py](https://github.com/QuantConnect/lean-cli/blob/master/lean/commands/cloud/pull.py)_
+
+### `lean cloud push`
+
+Push local projects to QuantConnect.
+
+```
+Usage: lean cloud push [OPTIONS]
+
+  Push local projects to QuantConnect.
+
+  This command overrides the content of cloud files with the content of their respective local counterparts.
+
+  This command will not delete cloud files which don't have a local counterpart.
+
+Options:
+  --project DIRECTORY  Path to the local project to push (all local projects if not specified)
+  --verbose            Enable debug logging
+  --help               Show this message and exit.
+```
+
+_See code: [lean/commands/cloud/push.py](https://github.com/QuantConnect/lean-cli/blob/master/lean/commands/cloud/push.py)_
+
+### `lean cloud status`
+
+Show the live trading status of a project in the cloud.
+
+```
+Usage: lean cloud status [OPTIONS] PROJECT
+
+  Show the live trading status of a project in the cloud.
+
+  PROJECT must be the name or the id of the project to show the status for.
+
+Options:
+  --verbose  Enable debug logging
+  --help     Show this message and exit.
+```
+
+_See code: [lean/commands/cloud/status.py](https://github.com/QuantConnect/lean-cli/blob/master/lean/commands/cloud/status.py)_
+
+### `lean config get`
+
+Get the current value of a configurable option.
+
+```
+Usage: lean config get [OPTIONS] KEY
+
+  Get the current value of a configurable option.
+
+  Sensitive options like credentials cannot be retrieved this way for security reasons. Please open
+  ~/.lean/credentials if you want to see your currently stored credentials.
+
+  Run `lean config list` to show all available options.
+
+Options:
+  --verbose  Enable debug logging
+  --help     Show this message and exit.
+```
+
+_See code: [lean/commands/config/get.py](https://github.com/QuantConnect/lean-cli/blob/master/lean/commands/config/get.py)_
+
+### `lean config list`
+
+List the configurable options and their current values.
+
+```
+Usage: lean config list [OPTIONS]
+
+  List the configurable options and their current values.
+
+Options:
+  --verbose  Enable debug logging
+  --help     Show this message and exit.
+```
+
+_See code: [lean/commands/config/list.py](https://github.com/QuantConnect/lean-cli/blob/master/lean/commands/config/list.py)_
+
+### `lean config set`
+
+Set a configurable option.
+
+```
+Usage: lean config set [OPTIONS] KEY VALUE
+
+  Set a configurable option.
+
+  Run `lean config list` to show all available options.
+
+Options:
+  --verbose  Enable debug logging
+  --help     Show this message and exit.
+```
+
+_See code: [lean/commands/config/set.py](https://github.com/QuantConnect/lean-cli/blob/master/lean/commands/config/set.py)_
+
+### `lean config unset`
+
+Unset a configurable option.
+
+```
+Usage: lean config unset [OPTIONS] KEY
+
+  Unset a configurable option.
+
+  Run `lean config list` to show all available options.
+
+Options:
+  --verbose  Enable debug logging
+  --help     Show this message and exit.
+```
+
+_See code: [lean/commands/config/unset.py](https://github.com/QuantConnect/lean-cli/blob/master/lean/commands/config/unset.py)_
+
+### `lean create-project`
+
+Create a new project containing starter code.
+
+```
+Usage: lean create-project [OPTIONS] NAME
+
+  Create a new project containing starter code.
+
+  If NAME is a path containing subdirectories those will be created automatically.
+
+  The default language can be set using `lean config set default-language python/csharp`.
+
+Options:
+  -l, --language [python|csharp]  The language of the project to create
+  --verbose                       Enable debug logging
+  --help                          Show this message and exit.
+```
+
+_See code: [lean/commands/create_project.py](https://github.com/QuantConnect/lean-cli/blob/master/lean/commands/create_project.py)_
+
+### `lean data download`
+
+Purchase and download data from QuantConnect Datasets.
+
+```
+Usage: lean data download [OPTIONS]
+
+  Purchase and download data from QuantConnect Datasets.
+
+  An interactive wizard will show to walk you through the process of selecting data, accepting the CLI API Access and
+  Data Agreement and payment. After this wizard the selected data will be downloaded automatically.
+
+  If --dataset is given the command runs in non-interactive mode. In this mode the CLI does not prompt for input or
+  confirmation but only halts when the agreement must be accepted. In non-interactive mode all options specific to the
+  selected dataset as well as --organization are required.
+
+  See the following url for the data that can be purchased and downloaded with this command:
+  https://www.quantconnect.com/datasets
+
+Options:
+  --dataset TEXT       The name of the dataset to download non-interactively
+  --organization TEXT  The name or id of the organization to purchase and download data with
+  --overwrite          Overwrite existing local data
+  --lean-config FILE   The Lean configuration file that should be used (defaults to the nearest lean.json)
+  --verbose            Enable debug logging
+  --help               Show this message and exit.
+```
+
+_See code: [lean/commands/data/download.py](https://github.com/QuantConnect/lean-cli/blob/master/lean/commands/data/download.py)_
+
+### `lean data generate`
+
+Generate random market data.
+
+```
+Usage: lean data generate [OPTIONS]
+
+  Generate random market data.
+
+  This uses the random data generator in LEAN to generate realistic market data using a Brownian motion model.
+  This generator supports the following security types, tick types and resolutions:
+  | Security type | Generated tick types | Supported resolutions                |
+  | ------------- | -------------------- | ------------------------------------ |
+  | Equity        | Trade                | Tick, Second, Minute, Hour and Daily |
+  | Forex         | Quote                | Tick, Second, Minute, Hour and Daily |
+  | CFD           | Quote                | Tick, Second, Minute, Hour and Daily |
+  | Future        | Trade and Quote      | Tick, Second, Minute, Hour and Daily |
+  | Crypto        | Trade and Quote      | Tick, Second, Minute, Hour and Daily |
+  | Option        | Trade and Quote      | Minute                               |
+
+  The following data densities are available:
+  - Dense: at least one data point per resolution step.
+  - Sparse: at least one data point per 5 resolution steps.
+  - VerySparse: at least one data point per 50 resolution steps.
+
+  Example which generates minute data for 100 equity symbols since 2015-01-01:
+  $ lean data generate --start=20150101 --symbol-count=100
+
+  Example which generates daily data for 100 crypto symbols since 2015-01-01:
+  $ lean data generate --start=20150101 --symbol-count=100 --security-type=Crypto --resolution=Daily
+
+  By default the official LEAN engine image is used. You can override this using the --image option. Alternatively you
+  can set the default engine image for all commands using `lean config set engine-image <image>`.
+
+Options:
+  --start [yyyyMMdd]              Start date for the data to generate in yyyyMMdd format  [required]
+  --end [yyyyMMdd]                End date for the data to generate in yyyyMMdd format (defaults to today)
+  --symbol-count INTEGER RANGE    The number of symbols to generate data for  [required]
+  --security-type [Equity|Forex|Cfd|Future|Crypto|Option]
+                                  The security type to generate data for (defaults to Equity)
+  --resolution [Tick|Second|Minute|Hour|Daily]
+                                  The resolution of the generated data (defaults to Minute)
+  --data-density [Dense|Sparse|VerySparse]
+                                  The density of the generated data (defaults to Dense)
+  --include-coarse BOOLEAN        Whether coarse universe data should be generated for Equity data (defaults to True)
+  --market TEXT                   The market to generate data for (defaults to standard market for the security type)
+  --image TEXT                    The LEAN engine image to use (defaults to quantconnect/lean:latest)
+  --update                        Pull the LEAN engine image before running the generator
+  --lean-config FILE              The Lean configuration file that should be used (defaults to the nearest lean.json)
+  --verbose                       Enable debug logging
+  --help                          Show this message and exit.
+```
+
+_See code: [lean/commands/data/generate.py](https://github.com/QuantConnect/lean-cli/blob/master/lean/commands/data/generate.py)_
+
+### `lean gui logs`
+
+See the logs of the local GUI.
+
+```
+Usage: lean gui logs [OPTIONS]
+
+  See the logs of the local GUI.
+
+Options:
+  -f, --follow  Update the logs in real-time while the GUI is running
+  --verbose     Enable debug logging
+  --help        Show this message and exit.
+```
+
+_See code: [lean/commands/gui/logs.py](https://github.com/QuantConnect/lean-cli/blob/master/lean/commands/gui/logs.py)_
+
+### `lean gui restart`
+
+Restart the local GUI and open it in the browser.
+
+```
+Usage: lean gui restart [OPTIONS]
+
+  Restart the local GUI and open it in the browser.
+
+Options:
+  --no-open  Skip opening the local GUI in the browser after restarting it
+  --verbose  Enable debug logging
+  --help     Show this message and exit.
+```
+
+_See code: [lean/commands/gui/restart.py](https://github.com/QuantConnect/lean-cli/blob/master/lean/commands/gui/restart.py)_
+
+### `lean gui start`
+
+Start the local GUI.
+
+```
+Usage: lean gui start [OPTIONS]
+
+  Start the local GUI.
+
+Options:
+  --organization TEXT  The name or id of the organization with the local GUI module subscription
+  --port INTEGER       The port to run the local GUI on (defaults to 5612)
+  --no-open            Skip opening the local GUI in the browser after starting it
+  --shortcut           Create a desktop shortcut for launching the local GUI
+  --lean-config FILE   The Lean configuration file that should be used (defaults to the nearest lean.json)
+  --verbose            Enable debug logging
+  --help               Show this message and exit.
+```
+
+_See code: [lean/commands/gui/start.py](https://github.com/QuantConnect/lean-cli/blob/master/lean/commands/gui/start.py)_
+
+### `lean gui stop`
+
+Stop the local GUI.
+
+```
+Usage: lean gui stop [OPTIONS]
+
+  Stop the local GUI.
+
+Options:
+  --verbose  Enable debug logging
+  --help     Show this message and exit.
+```
+
+_See code: [lean/commands/gui/stop.py](https://github.com/QuantConnect/lean-cli/blob/master/lean/commands/gui/stop.py)_
+
+### `lean init`
+
+Scaffold a Lean configuration file and data directory.
+
+```
+Usage: lean init [OPTIONS]
+
+  Scaffold a Lean configuration file and data directory.
+
+Options:
+  --verbose  Enable debug logging
+  --help     Show this message and exit.
+```
+
+_See code: [lean/commands/init.py](https://github.com/QuantConnect/lean-cli/blob/master/lean/commands/init.py)_
+
+### `lean library add`
+
+Add a custom library to a project.
+
+```
+Usage: lean library add [OPTIONS] PROJECT NAME
+
+  Add a custom library to a project.
+
+  PROJECT must be the path to the project.
+
+  NAME must be the name of a NuGet package (for C# projects) or of a PyPI package (for Python projects).
+
+  If --version is not given, the package is pinned to the latest compatible version. For C# projects, this is the
+  latest available version. For Python projects, this is the latest version compatible with Python 3.6 (which is what
+  the Docker images use).
+
+  Custom C# libraries are added to your project's .csproj file, which is then restored if dotnet is on your PATH and
+  the --no-local flag has not been given.
+
+  Custom Python libraries are added to your project's requirements.txt file and are installed in your local Python
+  environment so you get local autocomplete for the library. The last step can be skipped with the --no-local flag.
+
+  C# example usage:
+  $ lean library add "My CSharp Project" Microsoft.ML
+  $ lean library add "My CSharp Project" Microsoft.ML --version 1.5.5
+
+  Python example usage:
+  $ lean library add "My Python Project" tensorflow
+  $ lean library add "My Python Project" tensorflow --version 2.5.0
+
+Options:
+  --version TEXT  The version of the library to add (defaults to latest compatible version)
+  --no-local      Skip making changes to your local environment
+  --verbose       Enable debug logging
+  --help          Show this message and exit.
+```
+
+_See code: [lean/commands/library/add.py](https://github.com/QuantConnect/lean-cli/blob/master/lean/commands/library/add.py)_
+
+### `lean library remove`
+
+Remove a custom library from a project.
+
+```
+Usage: lean library remove [OPTIONS] PROJECT NAME
+
+  Remove a custom library from a project.
+
+  PROJECT must be the path to the project directory.
+
+  NAME must be the name of the NuGet package (for C# projects) or of the PyPI package (for Python projects) to remove.
+
+  Custom C# libraries are removed from the project's .csproj file, which is then restored if dotnet is on your PATH
+  and the --no-local flag has not been given.
+
+  Custom Python libraries are removed from the project's requirements.txt file.
+
+  C# example usage:
+  $ lean library remove "My CSharp Project" Microsoft.ML
+
+  Python example usage:
+  $ lean library remove "My Python Project" tensorflow
+
+Options:
+  --no-local  Skip making changes to your local environment
+  --verbose   Enable debug logging
+  --help      Show this message and exit.
+```
+
+_See code: [lean/commands/library/remove.py](https://github.com/QuantConnect/lean-cli/blob/master/lean/commands/library/remove.py)_
+
+### `lean live`
+
+Start live trading a project locally using Docker.
+
+```
+Usage: lean live [OPTIONS] PROJECT
+
+  Start live trading a project locally using Docker.
+
+  If PROJECT is a directory, the algorithm in the main.py or Main.cs file inside it will be executed.
+  If PROJECT is a file, the algorithm in the specified file will be executed.
+
+  By default an interactive wizard is shown letting you configure the brokerage and data feed to use. If
+  --environment, --brokerage or --data-feed are given the command runs in non-interactive mode. In this mode the CLI
+  does not prompt for input.
+
+  If --environment is given it must be the name of a live environment in the Lean configuration.
+
+  If --brokerage and --data-feed are given, the options specific to the given brokerage/data feed must also be given.
+  The Lean config is used as fallback when a brokerage/data feed-specific option hasn't been passed in. If a required
+  option is not given and cannot be found in the Lean config the command aborts.
+
+  By default the official LEAN engine image is used. You can override this using the --image option. Alternatively you
+  can set the default engine image for all commands using `lean config set engine-image <image>`.
+
+Options:
+  --environment TEXT              The environment to use
+  --output DIRECTORY              Directory to store results in (defaults to PROJECT/live/TIMESTAMP)
+  -d, --detach                    Run the live deployment in a detached Docker container and return immediately
+  --gui                           Enable monitoring and controlling of the deployment via the local GUI
+  --gui-organization TEXT         The name or id of the organization with the local GUI module subscription
+  --brokerage [Paper Trading|Interactive Brokers|Tradier|Oanda|Bitfinex|Coinbase Pro|Binance|Zerodha|Samco|Terminal Link|Atreyu|Trading Technologies|Kraken|FTX]
+                                  The brokerage to use
+  --data-feed [Interactive Brokers|Tradier|Oanda|Bitfinex|Coinbase Pro|Binance|Zerodha|Samco|Terminal Link|Trading Technologies|Kraken|FTX|IQFeed|Custom data only]
+                                  The data feed to use
+  --ib-organization TEXT          The name or id of the organization with the Interactive Brokers module subscription
+  --ib-user-name TEXT             Your Interactive Brokers username
+  --ib-account TEXT               Your Interactive Brokers account id
+  --ib-password TEXT              Your Interactive Brokers password
+  --ib-enable-delayed-streaming-data BOOLEAN
+                                  Whether delayed data may be used when your algorithm subscribes to a security you
+                                  don't have a market data subscription for
+
+  --tradier-account-id TEXT       Your Tradier account id
+  --tradier-access-token TEXT     Your Tradier access token
+  --tradier-environment [live|paper]
+                                  Whether the developer sandbox should be used
+  --oanda-environment [Practice|Trade]
+                                  The environment to run in, Practice for fxTrade Practice, Trade for fxTrade
+  --oanda-account-id TEXT         Your OANDA account id
+  --oanda-access-token TEXT       Your OANDA API token
+  --bitfinex-api-key TEXT         Your Bitfinex API key
+  --bitfinex-api-secret TEXT      Your Bitfinex API secret
+  --gdax-use-sandbox [live|paper]
+                                  Whether the sandbox should be used
+  --gdax-api-key TEXT             Your Coinbase Pro API key
+  --gdax-api-secret TEXT          Your Coinbase Pro API secret
+  --gdax-passphrase TEXT          Your Coinbase Pro API passphrase
+  --binance-use-testnet [live|paper]
+                                  Whether the testnet should be used
+  --binance-organization TEXT     The name or id of the organization with the Binance module subscription
+  --binance-api-key TEXT          Your Binance API key
+  --binance-api-secret TEXT       Your Binance API secret
+  --zerodha-organization TEXT     The name or id of the organization with the zerodha module subscription
+  --zerodha-api-key TEXT          Your Kite Connect API key
+  --zerodha-access-token TEXT     Your Kite Connect access token
+  --zerodha-product-type [MIS|CNC|NRML]
+                                  MIS if you are targeting intraday products, CNC if you are targeting delivery
+                                  products, NRML if you are targeting carry forward products
+
+  --zerodha-trading-segment [EQUITY|COMMODITY]
+                                  EQUITY if you are trading equities on NSE or BSE, COMMODITY if you are trading
+                                  commodities on MCX
+
+  --zerodha-history-subscription BOOLEAN
+                                  Whether you have a history API subscription for Zerodha
+  --samco-organization TEXT       The name or id of the organization with the samco module subscription
+  --samco-client-id TEXT          Your Samco account Client ID
+  --samco-client-password TEXT    Your Samco account password
+  --samco-year-of-birth TEXT      Your year of birth (YYYY) registered with Samco
+  --samco-product-type [MIS|CNC|NRML]
+                                  MIS if you are targeting intraday products, CNC if you are targeting delivery
+                                  products, NRML if you are targeting carry forward products
+
+  --samco-trading-segment [EQUITY|COMMODITY]
+                                  EQUITY if you are trading equities on NSE or BSE, COMMODITY if you are trading
+                                  commodities on MCX
+
+  --terminal-link-organization TEXT
+                                  The name or id of the organization with the Terminal Link module subscription
+  --bloomberg-environment [Production|Beta]
+                                  The environment to run in
+  --bloomberg-server-host TEXT    The host of the Bloomberg server
+  --bloomberg-server-port INTEGER
+                                  The port of the Bloomberg server
+  --bloomberg-symbol-map-file FILE
+                                  The path to the Bloomberg symbol map file
+  --bloomberg-emsx-broker TEXT    The EMSX broker to use
+  --bloomberg-emsx-user-time-zone TEXT
+                                  The EMSX user timezone to use
+  --bloomberg-emsx-account TEXT   The EMSX account to use
+  --bloomberg-emsx-strategy TEXT  The EMSX strategy to use
+  --bloomberg-emsx-notes TEXT     The EMSX notes to use
+  --bloomberg-emsx-handling TEXT  The EMSX handling to use
+  --bloomberg-allow-modification BOOLEAN
+                                  Whether modification is allowed
+  --atreyu-organization TEXT      The name or id of the organization with the Atreyu module subscription
+  --atreyu-host TEXT              The host of the Atreyu server
+  --atreyu-req-port INTEGER       The Atreyu request port
+  --atreyu-sub-port INTEGER       The Atreyu subscribe port
+  --atreyu-username TEXT          Your Atreyu username
+  --atreyu-password TEXT          Your Atreyu password
+  --atreyu-client-id TEXT         Your Atreyu client id
+  --atreyu-broker-mpid TEXT       The broker MPID to use
+  --atreyu-locate-rqd TEXT        The locate rqd to use
+  --tt-organization TEXT          The name or id of the organization with the Trading Technologies module subscription
+  --tt-user-name TEXT             Your Trading Technologies username
+  --tt-session-password TEXT      Your Trading Technologies session password
+  --tt-account-name TEXT          Your Trading Technologies account name
+  --tt-rest-app-key TEXT          Your Trading Technologies REST app key
+  --tt-rest-app-secret TEXT       Your Trading Technologies REST app secret
+  --tt-rest-environment TEXT      The REST environment to run in
+  --tt-market-data-sender-comp-id TEXT
+                                  The market data sender comp id to use
+  --tt-market-data-target-comp-id TEXT
+                                  The market data target comp id to use
+  --tt-market-data-host TEXT      The host of the market data server
+  --tt-market-data-port TEXT      The port of the market data server
+  --tt-order-routing-sender-comp-id TEXT
+                                  The order routing sender comp id to use
+  --tt-order-routing-target-comp-id TEXT
+                                  The order routing target comp id to use
+  --tt-order-routing-host TEXT    The host of the order routing server
+  --tt-order-routing-port TEXT    The port of the order routing server
+  --tt-log-fix-messages BOOLEAN   Whether FIX messages should be logged
+  --kraken-organization TEXT      The name or id of the organization with the kraken module subscription
+  --kraken-api-key TEXT           Your Kraken API key
+  --kraken-api-secret TEXT        Your Kraken API secret
+  --kraken-verification-tier [Starter|Intermediate|Pro]
+                                  Your Kraken Verification Tier
+  --ftx-exchange-name [FTX|FTXUS]
+                                  FTX exchange name [FTX, FTXUS]
+  --ftx-organization TEXT         The name or id of the organization with the FTX module subscription
+  --ftx-api-key TEXT              Your FTX API key
+  --ftxus-api-key TEXT            Your FTX API key
+  --ftx-api-secret TEXT           Your FTX API secret
+  --ftxus-api-secret TEXT         Your FTX API secret
+  --ftx-account-tier [Tier1|Tier2|Tier3|Tier4|Tier5|Tier6]
+                                  Your FTX Account Tier
+  --ftxus-account-tier [Tier1|Tier2|Tier3|Tier4|Tier5|Tier6]
+                                  Your FTX Account Tier
+  --iqfeed-iqconnect FILE         The path to the IQConnect binary
+  --iqfeed-username TEXT          Your IQFeed username
+  --iqfeed-password TEXT          Your IQFeed password
+  --iqfeed-productName TEXT       The product name of your IQFeed developer account
+  --iqfeed-version TEXT           The product version of your IQFeed developer account
+  --release                       Compile C# projects in release configuration instead of debug
+  --image TEXT                    The LEAN engine image to use (defaults to quantconnect/lean:latest)
+  --update                        Pull the LEAN engine image before starting live trading
+  --lean-config FILE              The Lean configuration file that should be used (defaults to the nearest lean.json)
+  --verbose                       Enable debug logging
+  --help                          Show this message and exit.
+```
+
+_See code: [lean/commands/live.py](https://github.com/QuantConnect/lean-cli/blob/master/lean/commands/live.py)_
+
+### `lean login`
+
+Log in with a QuantConnect account.
+
+```
+Usage: lean login [OPTIONS]
+
+  Log in with a QuantConnect account.
+
+  If user id or API token is not provided an interactive prompt will show.
+
+  Credentials are stored in ~/.lean/credentials and are removed upon running `lean logout`.
+
+Options:
+  -u, --user-id TEXT    QuantConnect user id
+  -t, --api-token TEXT  QuantConnect API token
+  --verbose             Enable debug logging
+  --help                Show this message and exit.
+```
+
+_See code: [lean/commands/login.py](https://github.com/QuantConnect/lean-cli/blob/master/lean/commands/login.py)_
+
+### `lean logout`
+
+Log out and remove stored credentials.
+
+```
+Usage: lean logout [OPTIONS]
+
+  Log out and remove stored credentials.
+
+Options:
+  --verbose  Enable debug logging
+  --help     Show this message and exit.
+```
+
+_See code: [lean/commands/logout.py](https://github.com/QuantConnect/lean-cli/blob/master/lean/commands/logout.py)_
+
+### `lean logs`
+
+Display the most recent backtest/live/optimization logs.
+
+```
+Usage: lean logs [OPTIONS]
+
+  Display the most recent backtest/live/optimization logs.
+
+Options:
+  --backtest           Display the most recent backtest logs (default)
+  --live               Display the most recent live logs
+  --optimization       Display the most recent optimization logs
+  --project DIRECTORY  The project to get the most recent logs from
+  --lean-config FILE   The Lean configuration file that should be used (defaults to the nearest lean.json)
+  --verbose            Enable debug logging
+  --help               Show this message and exit.
+```
+
+_See code: [lean/commands/logs.py](https://github.com/QuantConnect/lean-cli/blob/master/lean/commands/logs.py)_
+
+### `lean optimize`
+
+Optimize a project's parameters locally using Docker.
+
+```
+Usage: lean optimize [OPTIONS] PROJECT
+
+  Optimize a project's parameters locally using Docker.
+
+  If PROJECT is a directory, the algorithm in the main.py or Main.cs file inside it will be executed.
+  If PROJECT is a file, the algorithm in the specified file will be executed.
+
+  By default an interactive wizard is shown letting you configure the optimizer. If --optimizer-config or --strategy
+  is given the command runs in non-interactive mode. In this mode the CLI does not prompt for input.
+
+  The --optimizer-config option can be used to specify the configuration to run the optimizer with.
+  When using the option it should point to a file like this (the algorithm-* properties should be omitted):
+  https://github.com/QuantConnect/Lean/blob/master/Optimizer.Launcher/config.json
+
+  If --strategy is given the optimizer configuration is read from the given options. In this case --strategy,
+  --target, --target-direction and --parameter become required.
+
+  In non-interactive mode the --parameter option can be provided multiple times to configure multiple parameters:
+  - --parameter <name> <min value> <max value> <step size>
+  - --parameter my-first-parameter 1 10 0.5 --parameter my-second-parameter 20 30 5
+
+  In non-interactive mode the --constraint option can be provided multiple times to configure multiple constraints:
+  - --constraint "<statistic> <operator> <value>"
+  - --constraint "Sharpe Ratio >= 0.5" --constraint "Drawdown < 0.25"
+
+  By default the official LEAN engine image is used. You can override this using the --image option. Alternatively you
+  can set the default engine image for all commands using `lean config set engine-image <image>`.
+
+Options:
+  --output DIRECTORY              Directory to store results in (defaults to PROJECT/optimizations/TIMESTAMP)
+  -d, --detach                    Run the optimization in a detached Docker container and return immediately
+  --optimizer-config FILE         The optimizer configuration file that should be used
+  --strategy [Grid Search|Euler Search]
+                                  The optimization strategy to use
+  --target TEXT                   The target statistic of the optimization
+  --target-direction [min|max]    Whether the target must be minimized or maximized
+  --parameter <TEXT FLOAT FLOAT FLOAT>...
+                                  The 'parameter min max step' pairs configuring the parameters to optimize
+  --constraint TEXT               The 'statistic operator value' pairs configuring the constraints of the optimization
+  --release                       Compile C# projects in release configuration instead of debug
+  --image TEXT                    The LEAN engine image to use (defaults to quantconnect/lean:latest)
+  --update                        Pull the LEAN engine image before running the optimizer
+  --lean-config FILE              The Lean configuration file that should be used (defaults to the nearest lean.json)
+  --verbose                       Enable debug logging
+  --help                          Show this message and exit.
+```
+
+_See code: [lean/commands/optimize.py](https://github.com/QuantConnect/lean-cli/blob/master/lean/commands/optimize.py)_
+
+### `lean report`
+
+Generate a report of a backtest.
+
+```
+Usage: lean report [OPTIONS]
+
+  Generate a report of a backtest.
+
+  This runs the LEAN Report Creator in Docker to generate a polished, professional-grade report of a backtest.
+
+  If --backtest-results is not given, a report is generated for the most recent local backtest.
+
+  The name, description, and version are optional and will be blank if not given.
+
+  If the given backtest data source file is stored in a project directory (or one of its subdirectories, like the
+  default <project>/backtests/<timestamp>), the default name is the name of the project directory and the default
+  description is the description stored in the project's config.json file.
+
+  By default the official LEAN engine image is used. You can override this using the --image option. Alternatively you
+  can set the default engine image for all commands using `lean config set engine-image <image>`.
+
+Options:
+  --backtest-results FILE      Path to the JSON file containing the backtest results
+  --live-results FILE          Path to the JSON file containing the live trading results
+  --report-destination FILE    Path where the generated report is stored as HTML (defaults to ./report.html)
+  -d, --detach                 Run the report creator in a detached Docker container and return immediately
+  --strategy-name TEXT         Name of the strategy, will appear at the top-right corner of each page
+  --strategy-version TEXT      Version number of the strategy, will appear next to the project name
+  --strategy-description TEXT  Description of the strategy, will appear under the 'Strategy Description' section
+  --overwrite                  Overwrite --report-destination if it already contains a file
+  --image TEXT                 The LEAN engine image to use (defaults to quantconnect/lean:latest)
+  --update                     Pull the LEAN engine image before running the report creator
+  --lean-config FILE           The Lean configuration file that should be used (defaults to the nearest lean.json)
+  --verbose                    Enable debug logging
+  --help                       Show this message and exit.
+```
+
+_See code: [lean/commands/report.py](https://github.com/QuantConnect/lean-cli/blob/master/lean/commands/report.py)_
+
+### `lean research`
+
+Run a Jupyter Lab environment locally using Docker.
+
+```
+Usage: lean research [OPTIONS] PROJECT
+
+  Run a Jupyter Lab environment locally using Docker.
+
+  By default the official LEAN research image is used. You can override this using the --image option. Alternatively
+  you can set the default research image using `lean config set research-image <image>`.
+
+Options:
+  --port INTEGER                  The port to run Jupyter Lab on (defaults to 8888)
+  --data-provider [Terminal Link|QuantConnect|Local]
+                                  Update the Lean configuration file to retrieve data from the given provider
+  --download-data                 Update the Lean configuration file to download data from the QuantConnect API, alias
+                                  for --data-provider QuantConnect
+
+  --data-purchase-limit INTEGER   The maximum amount of QCC to spend on downloading data during the research session
+                                  when using QuantConnect as data provider
+
+  -d, --detach                    Run Jupyter Lab in a detached Docker container and return immediately
+  --no-open                       Don't open the Jupyter Lab environment in the browser after starting it
+  --image TEXT                    The LEAN research image to use (defaults to quantconnect/research:latest)
+  --update                        Pull the LEAN research image before starting the research environment
+  --lean-config FILE              The Lean configuration file that should be used (defaults to the nearest lean.json)
+  --verbose                       Enable debug logging
+  --help                          Show this message and exit.
+```
+
+_See code: [lean/commands/research.py](https://github.com/QuantConnect/lean-cli/blob/master/lean/commands/research.py)_
+
+### `lean whoami`
+
+Display who is logged in.
+
+```
+Usage: lean whoami [OPTIONS]
+
+  Display who is logged in.
+
+Options:
+  --verbose  Enable debug logging
+  --help     Show this message and exit.
+```
+
+_See code: [lean/commands/whoami.py](https://github.com/QuantConnect/lean-cli/blob/master/lean/commands/whoami.py)_
+<!-- commands end -->
+
+## Development
+
+To work on the Lean CLI, clone the repository, enter an environment containing Python 3.6+ and run `pip install -r requirements.txt`. This command will install the required dependencies and installs the CLI in editable mode. This means you'll be able to edit the code and immediately see the results the next time you run `lean`.
+
+If you need to add dependencies, first update `setup.py` (if it is a production dependency) or `requirements.txt` (if it is a development dependency) and then re-run `pip install -r requirements.txt`.
+
+The automated tests can be ran by running `pytest`. The filesystem and HTTP requests are mocked when running tests to make sure they run in an isolated environment.
+
+Can build the lean CLI by running `python setup.py sdist bdist_wheel` from the root of the project and to install it `pip install --force-reinstall dist/lean-dev-py3-none-any.whl`. To update the commands reference part of the readme run `python scripts/readme.py` from the root of the project, after installing the new version.
+
+Maintainers can publish new releases by pushing a Git tag containing the new version to GitHub. This will trigger a GitHub Actions workflow which releases the current `master` branch to PyPI with the value of the tag as version. Make sure the version is not prefixed with "v".
```

### Comparing `ablean-1.3.7/README.md` & `ablean-1.3.8/README.md`

 * *Files identical despite different names*

### Comparing `ablean-1.3.7/ablean/__init__.py` & `ablean-1.3.8/ablean/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-# QUANTCONNECT.COM - Democratizing Finance, Empowering Individuals.
-# Lean CLI v1.0. Copyright 2021 QuantConnect Corporation.
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-
-# The version is always set to "dev" in the Git repository. When a new release is ready,
-# a maintainer will push a new Git tag which will trigger GitHub Actions to publish a new
-# package to PyPI with the version of the tag.
-__version__ = "1.3.7"
+# QUANTCONNECT.COM - Democratizing Finance, Empowering Individuals.
+# Lean CLI v1.0. Copyright 2021 QuantConnect Corporation.
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+
+# The version is always set to "dev" in the Git repository. When a new release is ready,
+# a maintainer will push a new Git tag which will trigger GitHub Actions to publish a new
+# package to PyPI with the version of the tag.
+__version__ = "1.3.8"
```

### Comparing `ablean-1.3.7/ablean/commands/__init__.py` & `ablean-1.3.8/ablean/commands/__init__.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,33 +1,33 @@
-# QUANTCONNECT.COM - Democratizing Finance, Empowering Individuals.
-# Lean CLI v1.0. Copyright 2021 QuantConnect Corporation.
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-
-import click
-
-from ablean import __version__
-from ablean.commands.backtest import backtest
-from ablean.commands.create_project import create_project
-from ablean.commands.download import download
-from ablean.commands.init import init
-
-@click.group()
-@click.version_option(__version__)
-def lean() -> None:
-    """The Lean CLI by QuantConnect."""
-    # This method is intentionally empty
-    # It is used as the command group for all `lean <command>` commands
-    pass
-
-lean.add_command(backtest)
-lean.add_command(download)
-lean.add_command(create_project)
+# QUANTCONNECT.COM - Democratizing Finance, Empowering Individuals.
+# Lean CLI v1.0. Copyright 2021 QuantConnect Corporation.
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+
+import click
+
+from ablean import __version__
+from ablean.commands.backtest import backtest
+from ablean.commands.create_project import create_project
+from ablean.commands.download import download
+from ablean.commands.init import init
+
+@click.group()
+@click.version_option(__version__)
+def lean() -> None:
+    """The Lean CLI by QuantConnect."""
+    # This method is intentionally empty
+    # It is used as the command group for all `lean <command>` commands
+    pass
+
+lean.add_command(backtest)
+lean.add_command(download)
+lean.add_command(create_project)
 lean.add_command(init)
```

### Comparing `ablean-1.3.7/ablean/commands/backtest.py` & `ablean-1.3.8/ablean/commands/backtest.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,380 +1,380 @@
-# QUANTCONNECT.COM - Democratizing Finance, Empowering Individuals.
-# Lean CLI v1.0. Copyright 2021 QuantConnect Corporation.
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-
-import json5
-import os
-import sys
-import platform
-from pathlib import Path
-from datetime import datetime
-from pathlib import Path
-from typing import Optional
-
-import click
-from ablean.components.config.storage import Storage
-
-from ablean.myclick import LeanCommand, PathParameter
-from ablean.constants import DEFAULT_ENGINE_IMAGE
-from ablean.container import container
-from ablean.models.utils import DebuggingMethod
-from ablean.models.pydantic import Option
-
-def fix_ptvsd_signal_error():    
-    if platform.system() == 'Windows':
-        return
-    for s in sys.path:
-        if not s.endswith('site-packages'):
-            continue
-        file = Path(os.path.join(s, 'ptvsd', 'exit_handlers.py'))
-        if not file.exists():
-            continue
-        content = file.read_text()
-        if "# self._install_signal_handler()" in content:
-            return
-        content = content.replace("self._install_signal_handler()", "# self._install_signal_handler()")
-        file.write_text(content, encoding='utf-8')
-        return
-            
-
-
-# The _migrate_* methods automatically update launch configurations for a given debugging method.
-#
-# Occasionally we make changes which require updated launch configurations.
-# Projects which are created after these update have the correct configuration already,
-# but projects created before that need changes.
-#
-# These methods checks if the project has outdated configurations, and if so, update them to keep it working.
-
-
-def _migrate_python_pycharm(project_dir: Path) -> None:
-    workspace_xml_path = project_dir / ".idea" / "workspace.xml"
-    if not workspace_xml_path.is_file():
-        return
-
-    xml_manager = container.xml_manager()
-    current_content = xml_manager.parse(workspace_xml_path.read_text(encoding="utf-8"))
-
-    config = current_content.find('.//configuration[@name="Debug with Lean CLI"]')
-    if config is None:
-        return
-
-    path_mappings = config.find(
-        './/PathMappingSettings/option[@name="pathMappings"]/list'
-    )
-    if path_mappings is None:
-        return
-
-    made_changes = False
-    has_library_mapping = False
-
-    library_dir = container.lean_config_manager().get_cli_root_directory() / "Library"
-    if library_dir.is_dir():
-        library_dir = (
-            f"$PROJECT_DIR$/{os.path.relpath(library_dir, project_dir)}".replace(
-                "\\", "/"
-            )
-        )
-    else:
-        library_dir = None
-
-    for mapping in path_mappings.findall(".//mapping"):
-        if (
-            mapping.get("local-root") == "$PROJECT_DIR$"
-            and mapping.get("remote-root") == "/Lean/Launcher/bin/Debug"
-        ):
-            mapping.set("remote-root", "/LeanCLI")
-            made_changes = True
-
-        if (
-            library_dir is not None
-            and mapping.get("local-root") == library_dir
-            and mapping.get("remote-root") == "/Library"
-        ):
-            has_library_mapping = True
-
-    if library_dir is not None and not has_library_mapping:
-        library_mapping = xml_manager.parse("<mapping/>")
-        library_mapping.set("local-root", library_dir)
-        library_mapping.set("remote-root", "/Library")
-        path_mappings.append(library_mapping)
-        made_changes = True
-
-    if made_changes:
-        workspace_xml_path.write_text(
-            xml_manager.to_string(current_content), encoding="utf-8"
-        )
-
-        logger = container.logger()
-        logger.warn(
-            "Your run configuration has been updated to work with the latest version of LEAN"
-        )
-        logger.warn("Please restart the debugger in PyCharm and run this command again")
-
-        raise click.Abort()
-
-
-def _migrate_python_vscode(project_dir: Path) -> None:
-    launch_json_path = project_dir / ".vscode" / "launch.json"
-    if not launch_json_path.is_file():
-        return
-
-    current_content = json5.loads(launch_json_path.read_text(encoding="utf-8"))
-    if "configurations" not in current_content or not isinstance(
-        current_content["configurations"], list
-    ):
-        return
-
-    config = next(
-        (
-            c
-            for c in current_content["configurations"]
-            if c["name"] == "Debug with Lean CLI"
-        ),
-        None,
-    )
-    if config is None:
-        return
-
-    made_changes = False
-    has_library_mapping = False
-
-    library_dir = container.lean_config_manager().get_cli_root_directory() / "Library"
-    if not library_dir.is_dir():
-        library_dir = None
-
-    for mapping in config["pathMappings"]:
-        if (
-            mapping["localRoot"] == "${workspaceFolder}"
-            and mapping["remoteRoot"] == "/Lean/Launcher/bin/Debug"
-        ):
-            mapping["remoteRoot"] = "/LeanCLI"
-            made_changes = True
-
-        if (
-            library_dir is not None
-            and mapping["localRoot"] == str(library_dir)
-            and mapping["remoteRoot"] == "/Library"
-        ):
-            has_library_mapping = True
-
-    if library_dir is not None and not has_library_mapping:
-        config["pathMappings"].append(
-            {"localRoot": str(library_dir), "remoteRoot": "/Library"}
-        )
-        made_changes = True
-
-    if made_changes:
-        launch_json_path.write_text(
-            json5.dumps(current_content, indent=4), encoding="utf-8"
-        )
-
-
-def _migrate_csharp_rider(project_dir: Path) -> None:
-    made_changes = False
-    xml_manager = container.xml_manager()
-
-    for dir_name in [f".idea.{project_dir.stem}", f".idea.{project_dir.stem}.dir"]:
-        workspace_xml_path = (
-            project_dir / ".idea" / dir_name / ".idea" / "workspace.xml"
-        )
-        if not workspace_xml_path.is_file():
-            continue
-
-        current_content = xml_manager.parse(
-            workspace_xml_path.read_text(encoding="utf-8")
-        )
-
-        run_manager = current_content.find(".//component[@name='RunManager']")
-        if run_manager is None:
-            continue
-
-        config = run_manager.find(".//configuration[@name='Debug with Lean CLI']")
-        if config is None:
-            continue
-
-        run_manager.remove(config)
-
-        workspace_xml_path.write_text(
-            xml_manager.to_string(current_content), encoding="utf-8"
-        )
-        made_changes = True
-
-    if made_changes:
-        container.project_manager().generate_rider_config()
-
-        logger = container.logger()
-        logger.warn(
-            "Your run configuration has been updated to work with the .NET 5 version of LEAN"
-        )
-        logger.warn("Please restart Rider and start debugging again")
-        logger.warn(
-            "See https://www.lean.io/docs/lean-cli/backtesting/debugging#05-C-and-Rider for the updated instructions"
-        )
-
-        raise click.Abort()
-
-
-def _migrate_csharp_vscode(project_dir: Path) -> None:
-    launch_json_path = project_dir / ".vscode" / "launch.json"
-    if not launch_json_path.is_file():
-        return
-
-    current_content = json5.loads(launch_json_path.read_text(encoding="utf-8"))
-    if "configurations" not in current_content or not isinstance(
-        current_content["configurations"], list
-    ):
-        return
-
-    config = next(
-        (
-            c
-            for c in current_content["configurations"]
-            if c["name"] == "Debug with Lean CLI"
-        ),
-        None,
-    )
-    if config is None:
-        return
-
-    if (
-        config["type"] != "mono"
-        and config["processId"] != "${command:pickRemoteProcess}"
-    ):
-        return
-
-    config.pop("address", None)
-    config.pop("port", None)
-
-    config["type"] = "coreclr"
-    config["processId"] = "1"
-
-    config["pipeTransport"] = {
-        "pipeCwd": "${workspaceRoot}",
-        "pipeProgram": "docker",
-        "pipeArgs": ["exec", "-i", "lean_cli_vsdbg"],
-        "debuggerPath": "/root/vsdbg/vsdbg",
-        "quoteArgs": False,
-    }
-
-    config["logging"] = {"moduleLoad": False}
-
-    launch_json_path.write_text(json5.dumps(current_content, indent=4), encoding="utf-8")
-
-
-def _migrate_csharp_csproj(project_dir: Path) -> None:
-    csproj_path = next((f for f in project_dir.rglob("*.csproj")), None)
-    if csproj_path is None:
-        return
-
-    xml_manager = container.xml_manager()
-
-    current_content = xml_manager.parse(csproj_path.read_text(encoding="utf-8"))
-    if current_content.find(".//PropertyGroup/DefaultItemExcludes") is not None:
-        return
-
-    property_group = current_content.find(".//PropertyGroup")
-    if property_group is None:
-        property_group = xml_manager.parse("<PropertyGroup/>")
-        current_content.append(property_group)
-
-    default_item_excludes = xml_manager.parse(
-        "<DefaultItemExcludes>$(DefaultItemExcludes);backtests/*/code/**;live/*/code/**;optimizations/*/code/**</DefaultItemExcludes>"
-    )
-    property_group.append(default_item_excludes)
-
-    csproj_path.write_text(xml_manager.to_string(current_content), encoding="utf-8")
-
-
-@click.command(cls=LeanCommand, requires_lean_config=True)
-@click.argument(
-    "project", type=PathParameter(exists=True, file_okay=True, dir_okay=True)
-)
-@click.option(
-    "--config",
-    type=PathParameter(exists=True, file_okay=True, dir_okay=False),
-    help="用户指定的策略配置文件",
-)
-@click.option(
-    "--output",
-    type=PathParameter(exists=False, file_okay=False, dir_okay=True),
-    help="Directory to store results in (defaults to PROJECT/backtests/TIMESTAMP)",
-)
-@click.option(
-    "--debug",
-    is_flag=True,
-    default=False,
-    help="Enable debugger",
-)
-@click.option(
-    "--download-data",
-    is_flag=True,
-    default=False,
-    help="Update the backtest data",
-)
-def backtest(
-    project: Path,
-    config: Optional[Path],
-    output: Optional[Path],
-    debug: bool,
-    download_data: bool,
-) -> None:
-    """Backtest a project locally.
-
-    \b
-    If PROJECT is a directory, the algorithm in the main.py or Main.cs file inside it will be executed.
-    If PROJECT is a file, the algorithm in the specified file will be executed.
-
-    \b
-    Go to the following url to learn how to debug backtests locally using the Lean CLI:
-    https://www.lean.io/docs/lean-cli/backtesting/debugging
-
-    By default the official LEAN engine image is used.
-    You can override this using the --image option.
-    Alternatively you can set the default engine image for all commands using `lean config set engine-image <image>`.
-    """
-    project_manager = container.project_manager()
-    algorithm_file = project_manager.find_algorithm_file(Path(project))
-    lean_config_manager = container.lean_config_manager()
-
-    if output is None:
-        output = (
-            algorithm_file.parent
-            / "backtests"
-            / datetime.now().strftime("%Y-%m-%d_%H-%M-%S")
-        )
-
-    if not output.exists():
-        output.mkdir(parents=True)
-
-    debugging_method = None
-    if debug:
-        debugging_method = DebuggingMethod.PTVSD
-        fix_ptvsd_signal_error()
-        # _migrate_python_vscode(algorithm_file.parent)
-
-    lean_config = lean_config_manager.get_complete_lean_config(
-        "backtesting", algorithm_file, output, debugging_method
-    )
-
-    if config is not None:
-        for k, v in Storage(str(config)).data.items():
-            lean_config[k] = v
-
-    if download_data:
-        container.data_manager().update_data()
-
-    output_config_manager = container.output_config_manager()
-    lean_config["algorithm-id"] = str(output_config_manager.get_backtest_id(output))
-
-    lean_runner = container.lean_runner()
-    lean_runner.run_lean(lean_config, "backtesting", algorithm_file, output)
+# QUANTCONNECT.COM - Democratizing Finance, Empowering Individuals.
+# Lean CLI v1.0. Copyright 2021 QuantConnect Corporation.
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+
+import json5
+import os
+import sys
+import platform
+from pathlib import Path
+from datetime import datetime
+from pathlib import Path
+from typing import Optional
+
+import click
+from ablean.components.config.storage import Storage
+
+from ablean.myclick import LeanCommand, PathParameter
+from ablean.constants import DEFAULT_ENGINE_IMAGE
+from ablean.container import container
+from ablean.models.utils import DebuggingMethod
+from ablean.models.pydantic import Option
+
+def fix_ptvsd_signal_error():    
+    if platform.system() == 'Windows':
+        return
+    for s in sys.path:
+        if not s.endswith('site-packages'):
+            continue
+        file = Path(os.path.join(s, 'ptvsd', 'exit_handlers.py'))
+        if not file.exists():
+            continue
+        content = file.read_text()
+        if "# self._install_signal_handler()" in content:
+            return
+        content = content.replace("self._install_signal_handler()", "# self._install_signal_handler()")
+        file.write_text(content, encoding='utf-8')
+        return
+            
+
+
+# The _migrate_* methods automatically update launch configurations for a given debugging method.
+#
+# Occasionally we make changes which require updated launch configurations.
+# Projects which are created after these update have the correct configuration already,
+# but projects created before that need changes.
+#
+# These methods checks if the project has outdated configurations, and if so, update them to keep it working.
+
+
+def _migrate_python_pycharm(project_dir: Path) -> None:
+    workspace_xml_path = project_dir / ".idea" / "workspace.xml"
+    if not workspace_xml_path.is_file():
+        return
+
+    xml_manager = container.xml_manager()
+    current_content = xml_manager.parse(workspace_xml_path.read_text(encoding="utf-8"))
+
+    config = current_content.find('.//configuration[@name="Debug with Lean CLI"]')
+    if config is None:
+        return
+
+    path_mappings = config.find(
+        './/PathMappingSettings/option[@name="pathMappings"]/list'
+    )
+    if path_mappings is None:
+        return
+
+    made_changes = False
+    has_library_mapping = False
+
+    library_dir = container.lean_config_manager().get_cli_root_directory() / "Library"
+    if library_dir.is_dir():
+        library_dir = (
+            f"$PROJECT_DIR$/{os.path.relpath(library_dir, project_dir)}".replace(
+                "\\", "/"
+            )
+        )
+    else:
+        library_dir = None
+
+    for mapping in path_mappings.findall(".//mapping"):
+        if (
+            mapping.get("local-root") == "$PROJECT_DIR$"
+            and mapping.get("remote-root") == "/Lean/Launcher/bin/Debug"
+        ):
+            mapping.set("remote-root", "/LeanCLI")
+            made_changes = True
+
+        if (
+            library_dir is not None
+            and mapping.get("local-root") == library_dir
+            and mapping.get("remote-root") == "/Library"
+        ):
+            has_library_mapping = True
+
+    if library_dir is not None and not has_library_mapping:
+        library_mapping = xml_manager.parse("<mapping/>")
+        library_mapping.set("local-root", library_dir)
+        library_mapping.set("remote-root", "/Library")
+        path_mappings.append(library_mapping)
+        made_changes = True
+
+    if made_changes:
+        workspace_xml_path.write_text(
+            xml_manager.to_string(current_content), encoding="utf-8"
+        )
+
+        logger = container.logger()
+        logger.warn(
+            "Your run configuration has been updated to work with the latest version of LEAN"
+        )
+        logger.warn("Please restart the debugger in PyCharm and run this command again")
+
+        raise click.Abort()
+
+
+def _migrate_python_vscode(project_dir: Path) -> None:
+    launch_json_path = project_dir / ".vscode" / "launch.json"
+    if not launch_json_path.is_file():
+        return
+
+    current_content = json5.loads(launch_json_path.read_text(encoding="utf-8"))
+    if "configurations" not in current_content or not isinstance(
+        current_content["configurations"], list
+    ):
+        return
+
+    config = next(
+        (
+            c
+            for c in current_content["configurations"]
+            if c["name"] == "Debug with Lean CLI"
+        ),
+        None,
+    )
+    if config is None:
+        return
+
+    made_changes = False
+    has_library_mapping = False
+
+    library_dir = container.lean_config_manager().get_cli_root_directory() / "Library"
+    if not library_dir.is_dir():
+        library_dir = None
+
+    for mapping in config["pathMappings"]:
+        if (
+            mapping["localRoot"] == "${workspaceFolder}"
+            and mapping["remoteRoot"] == "/Lean/Launcher/bin/Debug"
+        ):
+            mapping["remoteRoot"] = "/LeanCLI"
+            made_changes = True
+
+        if (
+            library_dir is not None
+            and mapping["localRoot"] == str(library_dir)
+            and mapping["remoteRoot"] == "/Library"
+        ):
+            has_library_mapping = True
+
+    if library_dir is not None and not has_library_mapping:
+        config["pathMappings"].append(
+            {"localRoot": str(library_dir), "remoteRoot": "/Library"}
+        )
+        made_changes = True
+
+    if made_changes:
+        launch_json_path.write_text(
+            json5.dumps(current_content, indent=4), encoding="utf-8"
+        )
+
+
+def _migrate_csharp_rider(project_dir: Path) -> None:
+    made_changes = False
+    xml_manager = container.xml_manager()
+
+    for dir_name in [f".idea.{project_dir.stem}", f".idea.{project_dir.stem}.dir"]:
+        workspace_xml_path = (
+            project_dir / ".idea" / dir_name / ".idea" / "workspace.xml"
+        )
+        if not workspace_xml_path.is_file():
+            continue
+
+        current_content = xml_manager.parse(
+            workspace_xml_path.read_text(encoding="utf-8")
+        )
+
+        run_manager = current_content.find(".//component[@name='RunManager']")
+        if run_manager is None:
+            continue
+
+        config = run_manager.find(".//configuration[@name='Debug with Lean CLI']")
+        if config is None:
+            continue
+
+        run_manager.remove(config)
+
+        workspace_xml_path.write_text(
+            xml_manager.to_string(current_content), encoding="utf-8"
+        )
+        made_changes = True
+
+    if made_changes:
+        container.project_manager().generate_rider_config()
+
+        logger = container.logger()
+        logger.warn(
+            "Your run configuration has been updated to work with the .NET 5 version of LEAN"
+        )
+        logger.warn("Please restart Rider and start debugging again")
+        logger.warn(
+            "See https://www.lean.io/docs/lean-cli/backtesting/debugging#05-C-and-Rider for the updated instructions"
+        )
+
+        raise click.Abort()
+
+
+def _migrate_csharp_vscode(project_dir: Path) -> None:
+    launch_json_path = project_dir / ".vscode" / "launch.json"
+    if not launch_json_path.is_file():
+        return
+
+    current_content = json5.loads(launch_json_path.read_text(encoding="utf-8"))
+    if "configurations" not in current_content or not isinstance(
+        current_content["configurations"], list
+    ):
+        return
+
+    config = next(
+        (
+            c
+            for c in current_content["configurations"]
+            if c["name"] == "Debug with Lean CLI"
+        ),
+        None,
+    )
+    if config is None:
+        return
+
+    if (
+        config["type"] != "mono"
+        and config["processId"] != "${command:pickRemoteProcess}"
+    ):
+        return
+
+    config.pop("address", None)
+    config.pop("port", None)
+
+    config["type"] = "coreclr"
+    config["processId"] = "1"
+
+    config["pipeTransport"] = {
+        "pipeCwd": "${workspaceRoot}",
+        "pipeProgram": "docker",
+        "pipeArgs": ["exec", "-i", "lean_cli_vsdbg"],
+        "debuggerPath": "/root/vsdbg/vsdbg",
+        "quoteArgs": False,
+    }
+
+    config["logging"] = {"moduleLoad": False}
+
+    launch_json_path.write_text(json5.dumps(current_content, indent=4), encoding="utf-8")
+
+
+def _migrate_csharp_csproj(project_dir: Path) -> None:
+    csproj_path = next((f for f in project_dir.rglob("*.csproj")), None)
+    if csproj_path is None:
+        return
+
+    xml_manager = container.xml_manager()
+
+    current_content = xml_manager.parse(csproj_path.read_text(encoding="utf-8"))
+    if current_content.find(".//PropertyGroup/DefaultItemExcludes") is not None:
+        return
+
+    property_group = current_content.find(".//PropertyGroup")
+    if property_group is None:
+        property_group = xml_manager.parse("<PropertyGroup/>")
+        current_content.append(property_group)
+
+    default_item_excludes = xml_manager.parse(
+        "<DefaultItemExcludes>$(DefaultItemExcludes);backtests/*/code/**;live/*/code/**;optimizations/*/code/**</DefaultItemExcludes>"
+    )
+    property_group.append(default_item_excludes)
+
+    csproj_path.write_text(xml_manager.to_string(current_content), encoding="utf-8")
+
+
+@click.command(cls=LeanCommand, requires_lean_config=True)
+@click.argument(
+    "project", type=PathParameter(exists=True, file_okay=True, dir_okay=True)
+)
+@click.option(
+    "--config",
+    type=PathParameter(exists=True, file_okay=True, dir_okay=False),
+    help="用户指定的策略配置文件",
+)
+@click.option(
+    "--output",
+    type=PathParameter(exists=False, file_okay=False, dir_okay=True),
+    help="Directory to store results in (defaults to PROJECT/backtests/TIMESTAMP)",
+)
+@click.option(
+    "--debug",
+    is_flag=True,
+    default=False,
+    help="Enable debugger",
+)
+@click.option(
+    "--download-data",
+    is_flag=True,
+    default=False,
+    help="Update the backtest data",
+)
+def backtest(
+    project: Path,
+    config: Optional[Path],
+    output: Optional[Path],
+    debug: bool,
+    download_data: bool,
+) -> None:
+    """Backtest a project locally.
+
+    \b
+    If PROJECT is a directory, the algorithm in the main.py or Main.cs file inside it will be executed.
+    If PROJECT is a file, the algorithm in the specified file will be executed.
+
+    \b
+    Go to the following url to learn how to debug backtests locally using the Lean CLI:
+    https://www.lean.io/docs/lean-cli/backtesting/debugging
+
+    By default the official LEAN engine image is used.
+    You can override this using the --image option.
+    Alternatively you can set the default engine image for all commands using `lean config set engine-image <image>`.
+    """
+    project_manager = container.project_manager()
+    algorithm_file = project_manager.find_algorithm_file(Path(project))
+    lean_config_manager = container.lean_config_manager()
+
+    if output is None:
+        output = (
+            algorithm_file.parent
+            / "backtests"
+            / datetime.now().strftime("%Y-%m-%d_%H-%M-%S")
+        )
+
+    if not output.exists():
+        output.mkdir(parents=True)
+
+    debugging_method = None
+    if debug:
+        debugging_method = DebuggingMethod.PTVSD
+        fix_ptvsd_signal_error()
+        # _migrate_python_vscode(algorithm_file.parent)
+
+    lean_config = lean_config_manager.get_complete_lean_config(
+        "backtesting", algorithm_file, output, debugging_method
+    )
+
+    if config is not None:
+        for k, v in Storage(str(config)).data.items():
+            lean_config[k] = v
+
+    if download_data:
+        container.data_manager().update_data()
+
+    output_config_manager = container.output_config_manager()
+    lean_config["algorithm-id"] = str(output_config_manager.get_backtest_id(output))
+
+    lean_runner = container.lean_runner()
+    lean_runner.run_lean(lean_config, "backtesting", algorithm_file, output)
```

### Comparing `ablean-1.3.7/ablean/commands/create_project.py` & `ablean-1.3.8/ablean/commands/create_project.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,312 +1,366 @@
-# QUANTCONNECT.COM - Democratizing Finance, Empowering Individuals.
-# Lean CLI v1.0. Copyright 2021 QuantConnect Corporation.
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-
-from pathlib import Path
-import click
-from ablean.myclick import LeanCommand
-from ablean.container import container
-from ablean.models.errors import MoreInfoError
-from ablean.components.util.name_extraction import convert_to_class_name
-
-DEFAULT_PYTHON_MAIN = '''
-from AlgorithmImports import *
-
-
-class $CLASS_NAME$(QCAlgorithm):
-    def Initialize(self):
-        self.SetStartDate(2013, 10, 7)  # Set Start Date
-        self.SetEndDate(2013, 10, 11)  # Set End Date
-        self.SetCash(100000)  # Set Strategy Cash
-        self.AddEquity("SPY", Resolution.Minute)
-
-    def OnData(self, data):
-        """OnData event is the primary entry point for your algorithm. Each new data point will be pumped in here.
-            Arguments:
-                data: Slice object keyed by symbol containing the stock data
-        """
-        if not self.Portfolio.Invested:
-            self.SetHoldings("SPY", 1)
-            self.Debug("Purchased Stock")
-'''.strip() + "\n"
-
-LIBRARY_PYTHON_MAIN = '''
-from AlgorithmImports import *
-
-
-class $CLASS_NAME$:
-    """
-    To use this library place this at the top:
-    from $PROJECT_NAME$.main import $CLASS_NAME$
-
-    Then instantiate the class:
-    x = $CLASS_NAME$()
-    x.Add(1, 2)
-    """
-
-    def Add(self, a, b):
-        return a + b
-
-    def Subtract(self, a, b):
-        return a - b
-'''.strip() + "\n"
-
-DEFAULT_PYTHON_NOTEBOOK = """
-{
-    "cells": [
-        {
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
-                "![QuantConnect Logo](https://cdn.quantconnect.com/web/i/icon.png)\\n",
-                "<hr>"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "# QuantBook Analysis Tool\\n",
-                "# For more information see https://www.quantconnect.com/docs/research/overview\\n",
-                "qb = QuantBook()\\n",
-                "spy = qb.AddEquity(\\"SPY\\")\\n",
-                "history = qb.History(qb.Securities.Keys, 360, Resolution.Daily)\\n",
-                "\\n",
-                "# Indicator Analysis\\n",
-                "ema = qb.Indicator(ExponentialMovingAverage(10), spy.Symbol, 360, Resolution.Daily)\\n",
-                "ema.plot()"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {},
-            "outputs": [],
-            "source": []
-        }
-    ],
-    "metadata": {
-        "kernelspec": {
-            "display_name": "Python 3",
-            "language": "python",
-            "name": "python3"
-        },
-        "language_info": {
-            "codemirror_mode": {
-                "name": "ipython",
-                "version": 3
-            },
-            "file_extension": ".py",
-            "mimetype": "text/x-python",
-            "name": "python",
-            "nbconvert_exporter": "python",
-            "pygments_lexer": "ipython3",
-            "version": "3.6.8"
-        }
-    },
-    "nbformat": 4,
-    "nbformat_minor": 2
-}
-""".strip() + "\n"
-
-DEFAULT_CSHARP_MAIN = """
-using QuantConnect.Data;
-
-namespace QuantConnect.Algorithm.CSharp
-{
-    public class $CLASS_NAME$ : QCAlgorithm
-    {
-        public override void Initialize()
-        {
-            SetStartDate(2013, 10, 7); // Set Start Date
-            SetEndDate(2013, 10, 11); // Set Start Date
-            SetCash(100000); // Set Strategy Cash
-            AddEquity("SPY", Resolution.Minute);
-        }
-
-        /// OnData event is the primary entry point for your algorithm. Each new data point will be pumped in here.
-        /// Slice object keyed by symbol containing the stock data
-        public override void OnData(Slice data)
-        {
-            if (!Portfolio.Invested)
-            {
-                SetHoldings("SPY", 1);
-                Debug("Purchased Stock");
-            }
-        }
-    }
-}
-""".strip() + "\n"
-
-LIBRARY_CSHARP_MAIN = """
-namespace QuantConnect
-{
-    public class $CLASS_NAME$
-    {
-        /*
-         * To use this library, first add it to a solution and create a project reference in your algorithm project:
-         * https://www.lean.io/docs/lean-cli/projects/libraries/project-libraries#02-C-Libraries
-         *
-         * Then add its namespace at the top of the page:
-         * using QuantConnect;
-         *
-         * Then instantiate the class:
-         * var x = new $CLASS_NAME$();
-         * x.Add(1, 2);
-         */
-
-        public int Add(int a, int b)
-        {
-            return a + b;
-        }
-
-        public int Subtract(int a, int b)
-        {
-            return a - b;
-        }
-    }
-}
-""".strip() + "\n"
-
-DEFAULT_CSHARP_NOTEBOOK = """
-{
-    "cells": [
-        {
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
-                "![QuantConnect Logo](https://cdn.quantconnect.com/web/i/icon.png)\\n",
-                "<hr>"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "// We need to load assemblies at the start in their own cell\\n",
-                "#load \\"../Initialize.csx\\""
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "// QuantBook C# Research Environment\\n",
-                "// For more information see https://www.quantconnect.com/docs/research/overview\\n",
-                "#load \\"../QuantConnect.csx\\"\\n",
-                "\\n",
-                "using QuantConnect;\\n",
-                "using QuantConnect.Data;\\n",
-                "using QuantConnect.Research;\\n",
-                "using QuantConnect.Algorithm;\\n",
-                "\\n",
-                "var qb = new QuantBook();\\n",
-                "var spy = qb.AddEquity(\\"SPY\\");\\n",
-                "var history = qb.History(qb.Securities.Keys, 360, Resolution.Daily);"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "foreach (var slice in history.Take(5)) {\\n",
-                "    Console.WriteLine(slice.Bars[spy.Symbol].ToString());\\n",
-                "}"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {},
-            "outputs": [],
-            "source": []
-        }
-    ],
-    "metadata": {
-        "kernelspec": {
-            "display_name": ".NET (C#)",
-            "language": "C#",
-            "name": ".net-csharp"
-        },
-        "language_info": {
-            "file_extension": ".cs",
-            "mimetype": "text/x-csharp",
-            "name": "C#",
-            "pygments_lexer": "csharp",
-            "version": "9.0"
-        }
-    },
-    "nbformat": 4,
-    "nbformat_minor": 2
-}
-""".strip() + "\n"
-
-
-@click.command(cls=LeanCommand)
-@click.argument("name", type=str)
-def create_project(name: str) -> None:
-    """Create a new project containing starter code.
-
-    If NAME is a path containing subdirectories those will be created automatically.
-
-    """
-    language = "python"
-
-    full_path = Path.cwd() / name
-
-    if not container.path_manager().is_path_valid(full_path):
-        raise MoreInfoError(f"'{name}' is not a valid path",
-                            "https://www.lean.io/docs/lean-cli/key-concepts/troubleshooting#02-Common-Errors")
-
-    is_library_project = False
-    try:
-        library_dir = container.lean_config_manager().get_cli_root_directory() / "Library"
-        is_library_project = library_dir in full_path.parents
-    except:
-        # get_cli_root_directory() raises an error if there is no such directory
-        pass
-
-    if is_library_project and language == "python" and not full_path.name.isidentifier():
-        raise RuntimeError(
-            f"'{full_path.name}' is not a valid Python identifier, which is required for Python library projects to be importable")
-
-    if full_path.exists():
-        raise RuntimeError(f"A project named '{name}' already exists, please choose a different name")
-    else:
-        project_manager = container.project_manager()
-        project_manager.create_new_project(full_path)
-
-    class_name = convert_to_class_name(full_path)
-
-    if language == "python":
-        main_name = "main.py"
-        main_content = DEFAULT_PYTHON_MAIN if not is_library_project else LIBRARY_PYTHON_MAIN
-    else:
-        main_name = "Main.cs"
-        main_content = DEFAULT_CSHARP_MAIN if not is_library_project else LIBRARY_CSHARP_MAIN
-
-    with (full_path / main_name).open("w+", encoding="utf-8") as file:
-        file.write(main_content.replace("$CLASS_NAME$", class_name).replace("$PROJECT_NAME$", full_path.name))
-
-    with (full_path / "research.ipynb").open("w+", encoding="utf-8") as file:
-        file.write(DEFAULT_PYTHON_NOTEBOOK if language == "python" else DEFAULT_CSHARP_NOTEBOOK)
-
-    logger = container.logger()
-    logger.info(f"Successfully created {'Python' if language == 'python' else 'C#'} project '{name}'")
+# QUANTCONNECT.COM - Democratizing Finance, Empowering Individuals.
+# Lean CLI v1.0. Copyright 2021 QuantConnect Corporation.
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+
+from pathlib import Path
+import shutil
+import click
+from ablean.myclick import LeanCommand
+from ablean.container import container
+from ablean.models.errors import MoreInfoError
+from ablean.components.util.name_extraction import convert_to_class_name
+
+DEFAULT_PYTHON_MAIN = (
+    '''
+from AlgorithmImports import *
+
+
+class $CLASS_NAME$(QCAlgorithm):
+    def Initialize(self):
+        self.SetStartDate(2013, 10, 7)  # Set Start Date
+        self.SetEndDate(2013, 10, 11)  # Set End Date
+        self.SetCash(100000)  # Set Strategy Cash
+        self.AddEquity("SPY", Resolution.Minute)
+
+    def OnData(self, data):
+        """OnData event is the primary entry point for your algorithm. Each new data point will be pumped in here.
+            Arguments:
+                data: Slice object keyed by symbol containing the stock data
+        """
+        if not self.Portfolio.Invested:
+            self.SetHoldings("SPY", 1)
+            self.Debug("Purchased Stock")
+'''.strip()
+    + "\n"
+)
+
+LIBRARY_PYTHON_MAIN = (
+    '''
+from AlgorithmImports import *
+
+
+class $CLASS_NAME$:
+    """
+    To use this library place this at the top:
+    from $PROJECT_NAME$.main import $CLASS_NAME$
+
+    Then instantiate the class:
+    x = $CLASS_NAME$()
+    x.Add(1, 2)
+    """
+
+    def Add(self, a, b):
+        return a + b
+
+    def Subtract(self, a, b):
+        return a - b
+'''.strip()
+    + "\n"
+)
+
+DEFAULT_PYTHON_NOTEBOOK = (
+    """
+{
+    "cells": [
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "![QuantConnect Logo](https://cdn.quantconnect.com/web/i/icon.png)\\n",
+                "<hr>"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "%run \"#LEAN_ROOT_PATH#/launcher/start.py\""
+            ]
+        },        
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "# QuantBook Analysis Tool\\n",
+                "# For more information see https://www.quantconnect.com/docs/research/overview\\n",
+                "from AlgorithmImports import *\\n"
+                "qb = QuantBook()\\n",
+                "spy = qb.AddEquity(\\"SPY\\")\\n",
+                "history = qb.History(qb.Securities.Keys, 360, Resolution.Daily)\\n",
+                "\\n",
+                "# Indicator Analysis\\n",
+                "ema = qb.Indicator(ExponentialMovingAverage(10), spy.Symbol, 360, Resolution.Daily)\\n",
+                "ema.plot()"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": []
+        }
+    ],
+    "metadata": {
+        "kernelspec": {
+            "display_name": "Python 3",
+            "language": "python",
+            "name": "python3"
+        },
+        "language_info": {
+            "codemirror_mode": {
+                "name": "ipython",
+                "version": 3
+            },
+            "file_extension": ".py",
+            "mimetype": "text/x-python",
+            "name": "python",
+            "nbconvert_exporter": "python",
+            "pygments_lexer": "ipython3",
+            "version": "3.6.8"
+        }
+    },
+    "nbformat": 4,
+    "nbformat_minor": 2
+}
+""".strip()
+    + "\n"
+)
+
+DEFAULT_CSHARP_MAIN = (
+    """
+using QuantConnect.Data;
+
+namespace QuantConnect.Algorithm.CSharp
+{
+    public class $CLASS_NAME$ : QCAlgorithm
+    {
+        public override void Initialize()
+        {
+            SetStartDate(2013, 10, 7); // Set Start Date
+            SetEndDate(2013, 10, 11); // Set Start Date
+            SetCash(100000); // Set Strategy Cash
+            AddEquity("SPY", Resolution.Minute);
+        }
+
+        /// OnData event is the primary entry point for your algorithm. Each new data point will be pumped in here.
+        /// Slice object keyed by symbol containing the stock data
+        public override void OnData(Slice data)
+        {
+            if (!Portfolio.Invested)
+            {
+                SetHoldings("SPY", 1);
+                Debug("Purchased Stock");
+            }
+        }
+    }
+}
+""".strip()
+    + "\n"
+)
+
+LIBRARY_CSHARP_MAIN = (
+    """
+namespace QuantConnect
+{
+    public class $CLASS_NAME$
+    {
+        /*
+         * To use this library, first add it to a solution and create a project reference in your algorithm project:
+         * https://www.lean.io/docs/lean-cli/projects/libraries/project-libraries#02-C-Libraries
+         *
+         * Then add its namespace at the top of the page:
+         * using QuantConnect;
+         *
+         * Then instantiate the class:
+         * var x = new $CLASS_NAME$();
+         * x.Add(1, 2);
+         */
+
+        public int Add(int a, int b)
+        {
+            return a + b;
+        }
+
+        public int Subtract(int a, int b)
+        {
+            return a - b;
+        }
+    }
+}
+""".strip()
+    + "\n"
+)
+
+DEFAULT_CSHARP_NOTEBOOK = (
+    """
+{
+    "cells": [
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "![QuantConnect Logo](https://cdn.quantconnect.com/web/i/icon.png)\\n",
+                "<hr>"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "// We need to load assemblies at the start in their own cell\\n",
+                "#load \\"../Initialize.csx\\""
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "// QuantBook C# Research Environment\\n",
+                "// For more information see https://www.quantconnect.com/docs/research/overview\\n",
+                "#load \\"../QuantConnect.csx\\"\\n",
+                "\\n",
+                "using QuantConnect;\\n",
+                "using QuantConnect.Data;\\n",
+                "using QuantConnect.Research;\\n",
+                "using QuantConnect.Algorithm;\\n",
+                "\\n",
+                "var qb = new QuantBook();\\n",
+                "var spy = qb.AddEquity(\\"SPY\\");\\n",
+                "var history = qb.History(qb.Securities.Keys, 360, Resolution.Daily);"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "foreach (var slice in history.Take(5)) {\\n",
+                "    Console.WriteLine(slice.Bars[spy.Symbol].ToString());\\n",
+                "}"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": []
+        }
+    ],
+    "metadata": {
+        "kernelspec": {
+            "display_name": ".NET (C#)",
+            "language": "C#",
+            "name": ".net-csharp"
+        },
+        "language_info": {
+            "file_extension": ".cs",
+            "mimetype": "text/x-csharp",
+            "name": "C#",
+            "pygments_lexer": "csharp",
+            "version": "9.0"
+        }
+    },
+    "nbformat": 4,
+    "nbformat_minor": 2
+}
+""".strip()
+    + "\n"
+)
+
+
+@click.command(cls=LeanCommand)
+@click.argument("name", type=str)
+def create_project(name: str) -> None:
+    """Create a new project containing starter code.
+
+    If NAME is a path containing subdirectories those will be created automatically.
+
+    """
+    language = "python"
+
+    full_path = Path.cwd() / name
+    cli_root = container.lean_config_manager().get_cli_root_directory()
+
+    if not container.path_manager().is_path_valid(full_path):
+        raise MoreInfoError(
+            f"'{name}' is not a valid path",
+            "https://www.lean.io/docs/lean-cli/key-concepts/troubleshooting#02-Common-Errors",
+        )
+
+    is_library_project = False
+    try:
+        library_dir = cli_root / "Library"
+        is_library_project = library_dir in full_path.parents
+    except:
+        # get_cli_root_directory() raises an error if there is no such directory
+        pass
+
+    if (
+        is_library_project
+        and language == "python"
+        and not full_path.name.isidentifier()
+    ):
+        raise RuntimeError(
+            f"'{full_path.name}' is not a valid Python identifier, which is required for Python library projects to be importable"
+        )
+
+    if full_path.exists():
+        raise RuntimeError(
+            f"A project named '{name}' already exists, please choose a different name"
+        )
+    else:
+        project_manager = container.project_manager()
+        project_manager.create_new_project(full_path)
+
+    class_name = convert_to_class_name(full_path)
+
+    if language == "python":
+        main_name = "main.py"
+        main_content = (
+            DEFAULT_PYTHON_MAIN if not is_library_project else LIBRARY_PYTHON_MAIN
+        )
+    else:
+        main_name = "Main.cs"
+        main_content = (
+            DEFAULT_CSHARP_MAIN if not is_library_project else LIBRARY_CSHARP_MAIN
+        )
+
+    with (full_path / main_name).open("w+", encoding="utf-8") as file:
+        file.write(
+            main_content.replace("$CLASS_NAME$", class_name).replace(
+                "$PROJECT_NAME$", full_path.name
+            )
+        )
+
+    with (full_path / "research.ipynb").open("w+", encoding="utf-8") as file:
+        content = DEFAULT_PYTHON_NOTEBOOK.replace("#LEAN_ROOT_PATH#", cli_root)
+        file.write(content if language == "python" else DEFAULT_CSHARP_NOTEBOOK)
+
+    if language == "python":
+        pandas_mapper = cli_root / "launcher" / "PandasMapper.py"
+        shutil.copyfile(pandas_mapper, full_path / "PandasMapper.py")
+
+    logger = container.logger()
+    logger.info(
+        f"Successfully created {'Python' if language == 'python' else 'C#'} project '{name}'"
+    )
```

### Comparing `ablean-1.3.7/ablean/components/__init__.py` & `ablean-1.3.8/ablean/components/__init__.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-# QUANTCONNECT.COM - Democratizing Finance, Empowering Individuals.
-# Lean CLI v1.0. Copyright 2021 QuantConnect Corporation.
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
+# QUANTCONNECT.COM - Democratizing Finance, Empowering Individuals.
+# Lean CLI v1.0. Copyright 2021 QuantConnect Corporation.
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
```

### Comparing `ablean-1.3.7/ablean/components/config/__init__.py` & `ablean-1.3.8/ablean/components/config/__init__.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-# QUANTCONNECT.COM - Democratizing Finance, Empowering Individuals.
-# Lean CLI v1.0. Copyright 2021 QuantConnect Corporation.
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
+# QUANTCONNECT.COM - Democratizing Finance, Empowering Individuals.
+# Lean CLI v1.0. Copyright 2021 QuantConnect Corporation.
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
```

### Comparing `ablean-1.3.7/ablean/components/config/cli_config_manager.py` & `ablean-1.3.8/ablean/components/config/cli_config_manager.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,71 +1,71 @@
-# QUANTCONNECT.COM - Democratizing Finance, Empowering Individuals.
-# Lean CLI v1.0. Copyright 2021 QuantConnect Corporation.
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-
-from typing import Optional
-
-from ablean.components.config.storage import Storage
-from ablean.constants import DEFAULT_ENGINE_IMAGE, DEFAULT_RESEARCH_IMAGE
-from ablean.models.errors import MoreInfoError
-from ablean.models.options import ChoiceOption, Option
-
-
-class CLIConfigManager:
-    """The CLIConfigManager class contains all configurable CLI options."""
-
-    def __init__(self, general_storage: Storage, credentials_storage: Storage) -> None:
-        """Creates a new CLIConfigManager instance.
-
-        :param general_storage: the Storage instance for general, non-sensitive options
-        :param credentials_storage: the Storage instance for credentials
-        """
-        self.user_id = Option(
-            "user-id",
-            "The user id used when making authenticated requests to the QuantConnect API.",
-            True,
-            credentials_storage,
-        )
-
-        self.api_token = Option(
-            "api-token",
-            "The API token used when making authenticated requests to the QuantConnect API.",
-            True,
-            credentials_storage,
-        )
-
-        self.default_language = ChoiceOption(
-            "default-language",
-            "The default language used when creating new projects.",
-            ["python", "csharp"],
-            False,
-            general_storage,
-        )
-
-        self.all_options = [self.user_id, self.api_token, self.default_language]
-
-    def get_option_by_key(self, key: str) -> Option:
-        """Returns the option matching the given key.
-
-        If no option with the given key exists, an error is raised.
-
-        :param key: the key to look for
-        :return: the option having a key equal to the given key
-        """
-        option = next((x for x in self.all_options if x.key == key), None)
-
-        if option is None:
-            raise MoreInfoError(
-                f"There doesn't exist an option with key '{key}'",
-                "https://www.lean.io/docs/lean-cli/api-reference/lean-config-set#02-Description",
-            )
-
-        return option
+# QUANTCONNECT.COM - Democratizing Finance, Empowering Individuals.
+# Lean CLI v1.0. Copyright 2021 QuantConnect Corporation.
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+
+from typing import Optional
+
+from ablean.components.config.storage import Storage
+from ablean.constants import DEFAULT_ENGINE_IMAGE, DEFAULT_RESEARCH_IMAGE
+from ablean.models.errors import MoreInfoError
+from ablean.models.options import ChoiceOption, Option
+
+
+class CLIConfigManager:
+    """The CLIConfigManager class contains all configurable CLI options."""
+
+    def __init__(self, general_storage: Storage, credentials_storage: Storage) -> None:
+        """Creates a new CLIConfigManager instance.
+
+        :param general_storage: the Storage instance for general, non-sensitive options
+        :param credentials_storage: the Storage instance for credentials
+        """
+        self.user_id = Option(
+            "user-id",
+            "The user id used when making authenticated requests to the QuantConnect API.",
+            True,
+            credentials_storage,
+        )
+
+        self.api_token = Option(
+            "api-token",
+            "The API token used when making authenticated requests to the QuantConnect API.",
+            True,
+            credentials_storage,
+        )
+
+        self.default_language = ChoiceOption(
+            "default-language",
+            "The default language used when creating new projects.",
+            ["python", "csharp"],
+            False,
+            general_storage,
+        )
+
+        self.all_options = [self.user_id, self.api_token, self.default_language]
+
+    def get_option_by_key(self, key: str) -> Option:
+        """Returns the option matching the given key.
+
+        If no option with the given key exists, an error is raised.
+
+        :param key: the key to look for
+        :return: the option having a key equal to the given key
+        """
+        option = next((x for x in self.all_options if x.key == key), None)
+
+        if option is None:
+            raise MoreInfoError(
+                f"There doesn't exist an option with key '{key}'",
+                "https://www.lean.io/docs/lean-cli/api-reference/lean-config-set#02-Description",
+            )
+
+        return option
```

### Comparing `ablean-1.3.7/ablean/components/config/lean_config_manager.py` & `ablean-1.3.8/ablean/components/config/lean_config_manager.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,343 +1,343 @@
-# QUANTCONNECT.COM - Democratizing Finance, Empowering Individuals.
-# Lean CLI v1.0. Copyright 2021 QuantConnect Corporation.
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-
-import os
-import re
-from pathlib import Path
-from typing import Any, Dict, Optional, List
-
-import json5
-
-from ablean.components.config.cli_config_manager import CLIConfigManager
-from ablean.components.config.project_config_manager import ProjectConfigManager
-from ablean.components.module_manager import ModuleManager
-from ablean.components.config.storage import Storage
-from ablean.components.util.logger import Logger
-from ablean.constants import DEFAULT_LEAN_CONFIG_FILE_NAME, ENV_LEAN_PATH_NAME, GUI_PRODUCT_INSTALL_ID
-from ablean.models.errors import MoreInfoError
-from ablean.models.utils import DebuggingMethod
-
-
-class LeanConfigManager:
-    """The LeanConfigManager class contains utilities to work with files containing LEAN engine configuration."""
-
-    def __init__(
-        self,
-        logger: Logger,
-        cli_config_manager: CLIConfigManager,
-        project_config_manager: ProjectConfigManager,
-        module_manager: ModuleManager,
-        cache_storage: Storage,
-    ) -> None:
-        """Creates a new LeanConfigManager instance.
-
-        :param logger: the logger to log messages with
-        :param cache_storage: the Storage instance to store known Lean config paths in
-        """
-        self._logger = logger
-        self._module_manager = module_manager
-        self._cli_config_manager = cli_config_manager
-        self._project_config_manager = project_config_manager
-        self._cache_storage = cache_storage
-        self._default_path = None
-        self._lean_config_path = None
-
-    def get_lean_config_path(self) -> Path:
-        """Returns the path to the closest Lean config file.
-
-        This recurses upwards in the directory tree looking for a Lean config file.
-        This search can be overridden using set_default_lean_config_path().
-
-        Raises an error if no Lean config file can be found.
-
-        :return: the path to the closest Lean config file
-        """
-        if self._default_path is not None:
-            return self._default_path
-
-        if self._lean_config_path is not None:
-            return self._lean_config_path
-
-        # Recurse upwards in the directory tree until we find a Lean config file
-        list = self.get_search_paths()
-        for current_dir in list:
-            target_file = current_dir / DEFAULT_LEAN_CONFIG_FILE_NAME
-            if target_file.exists():
-                self._lean_config_path = target_file
-                self.store_known_lean_config_path(self._lean_config_path)
-                return self._lean_config_path
-            
-        raise MoreInfoError(
-            f"'{DEFAULT_LEAN_CONFIG_FILE_NAME}' not found",
-            "https://www.lean.io/docs/lean-cli/initialization/configuration#03-Lean-Configuration",
-        )
-    
-    def get_search_paths(self):
-        current_dir = Path.cwd()
-        dirs = [current_dir]
-        while True:
-            # If the parent directory is the same as the current directory we can't go up any more
-            if current_dir.parent == current_dir:
-                break
-            current_dir = current_dir.parent              
-            dirs.append(current_dir)
-        v = os.environ.get(ENV_LEAN_PATH_NAME)
-        if  v is not None:
-            dirs.append(Path(v))
-        return dirs
-
-    def set_default_lean_config_path(self, path: Path) -> None:
-        """Overrides the default search for the path to the Lean config file.
-
-        :param path: the path to the Lean config file to return in future calls to get_lean_config_path()
-        """
-        self.store_known_lean_config_path(path)
-        self._default_path = path
-
-    def get_known_lean_config_paths(self) -> List[Path]:
-        """Returns the known Lean config file paths.
-
-        :return: a list of paths to Lean config files that were used in the past
-        """
-        lean_config_paths = self._cache_storage.get("known-lean-config-paths", [])
-        lean_config_paths = [Path(p) for p in lean_config_paths]
-        lean_config_paths = [p for p in lean_config_paths if p.is_file()]
-
-        self._cache_storage.set(
-            "known-lean-config-paths", [str(p) for p in lean_config_paths]
-        )
-
-        return lean_config_paths
-
-    def store_known_lean_config_path(self, path: Path) -> None:
-        """Caches a path as being a known Lean configuration file path.
-
-        :param path: the path to the Lean configuration file
-        """
-        lean_config_paths = set(self._cache_storage.get("known-lean-config-paths", []))
-        lean_config_paths.add(str(path))
-        self._cache_storage.set("known-lean-config-paths", list(lean_config_paths))
-
-    def get_cli_root_directory(self) -> Path:
-        """Returns the path to the directory containing the Lean config file.
-
-        :return: the path to the directory containing the Lean config file
-        """
-        return self.get_lean_config_path().parent
-
-    def get_data_directory(self) -> Path:
-        """Returns the path to the data directory.
-
-        :return: the path to the data directory as it is configured in the Lean config
-        """
-        config = self.get_lean_config()
-        return self.get_cli_root_directory() / config["data-folder"]
-
-    def set_properties(self, updates: Dict[str, Any]) -> None:
-        """Sets a properties in the Lean config file.
-
-        If a property does not exist yet it is added automatically.
-        Comments in the Lean config file are preserved.
-
-        :param updates: the key -> new value updates to apply to the current config
-        """
-        config = self.get_lean_config()
-
-        config_path = self.get_lean_config_path()
-        config_text = config_path.read_text(encoding="utf-8")
-
-        for key, value in reversed(list(updates.items())):
-            if value is None:
-                continue
-            json_value = json5.dumps(value)
-
-            # We can only use regex to set the property because converting the config back to JSON drops all comments
-            if key in config:
-                config_text = re.sub(
-                    fr'"{key}":\s*("?[^",]*"?)', f'"{key}": {json_value}', config_text
-                )
-            else:
-                config_text = config_text.replace(
-                    "{", f'{{\n  "{key}": {json_value},', 1
-                )
-
-        config_path.write_text(config_text, encoding="utf-8")
-
-    def clean_lean_config(self, config: str) -> str:
-        """Removes the properties from a Lean config file which can be set in get_complete_lean_config().
-
-        This removes all the properties which the CLI can configure automatically based on the command that is ran.
-
-        For example, given the following config:
-        {
-            // Environment docs
-            "environment": "backtesting",
-
-            // Key2 docs
-            "key2": "value2"
-        }
-
-        Calling clean_lean_config(config) would return the following:
-        {
-            // Key2 docs
-            "key2": "value2"
-        }
-
-        Because "environment" can be set automatically based on the command that is ran.
-
-        :param config: the configuration to remove the auto-configurable keys from
-        :return: the same config as passed in with the config argument, but without the auto-configurable keys
-        """
-        # The keys that we can set automatically based on the command that is ran
-        keys_to_remove = [
-            "environment",
-            "composer-dll-directory",
-            "debugging",
-            "debugging-method",
-            "job-user-id",
-            "api-access-token",
-            "algorithm-type-name",
-            "algorithm-language",
-            "algorithm-location",
-            "parameters",
-            "intrinio-username",
-            "intrinio-password",
-            "ema-fast",
-            "ema-slow",
-        ]
-
-        # This function is implemented by doing string manipulation because the config contains comments
-        # If we were to parse it as JSON, we would have to remove the comments, which we don't want to do
-        sections = re.split(r"\n\s*\n", config)
-        for key in keys_to_remove:
-            sections = [
-                section for section in sections if f"\"{key}\": " not in section
-            ]
-        config = "\n\n".join(sections)
-
-        # For some keys we should only remove the key itself, instead of their entire section
-        lines = config.split("\n")
-        for key in ["ib-host", "ib-port", "ib-tws-dir", "ib-version"]:
-            lines = [line for line in lines if f"\"{key}\": " not in line]
-        config = "\n".join(lines)
-
-        # Instead of setting the IQFeed host we require the user to set the IQConnect location
-        config = config.replace(
-            '"iqfeed-host": "127.0.0.1"',
-            '"iqfeed-iqconnect": "C:/Program Files (x86)/DTN/IQFeed/iqconnect.exe"',
-        )
-
-        return config
-
-    def get_complete_lean_config(
-        self,
-        environment: str,
-        algorithm_file: Path,
-        output: Path,
-        debugging_method: Optional[DebuggingMethod],
-    ) -> Dict[str, Any]:
-        """Returns a complete Lean config object containing all properties needed for the engine to run.
-
-        This retrieves the path of the config, parses the file and adds all properties removed in clean_lean_config().
-
-        :param environment: the environment to set
-        :param algorithm_file: the path to the algorithm that will be ran
-        :param debugging_method: the debugging method to use, or None to disable debugging
-        """
-        config = self.get_lean_config()
-
-        config["environment"] = environment
-        config["close-automatically"] = True
-
-        config["composer-dll-directory"] = str(self.get_cli_root_directory() / "launcher")
-        config["results-destination-folder"] = str(output)
-
-        if debugging_method is not None:
-            config["debugging"] = True
-            config["debugging-method"] = debugging_method.get_internal_name()
-        else:
-            config["debugging"] = False
-            config["debugging-method"] = "LocalCmdline"
-
-        # The following key -> value pairs are added to the config unless they are already set by the user
-        config_defaults = {
-            "job-user-id": self._cli_config_manager.user_id.get_value(default="0"),
-            "api-access-token": self._cli_config_manager.api_token.get_value(
-                default=""
-            ),
-            "job-project-id": self._project_config_manager.get_local_id(
-                algorithm_file.parent
-            ),
-            "ib-host": "127.0.0.1",
-            "ib-port": "4002",
-            "ib-tws-dir": "/root/Jts",
-            "ib-version": "985",
-            "iqfeed-host": "host.docker.internal",
-        }
-
-        for key, value in config_defaults.items():
-            if config.get(key, "") == "":
-                config[key] = value
-
-        if algorithm_file.name.endswith(".py"):
-            config["algorithm-type-name"] = algorithm_file.name.split(".")[0]
-            config["algorithm-language"] = "Python"
-            config["algorithm-location"] = str(algorithm_file)
-        else:
-            algorithm_text = algorithm_file.read_text(encoding="utf-8")
-            config["algorithm-type-name"] = re.findall(
-                r"class\s*([^\s:]+)\s*:\s*QCAlgorithm", algorithm_text
-            )[0]
-            config["algorithm-language"] = "CSharp"
-            config["algorithm-location"] = f"{algorithm_file.parent.name}.dll"
-
-        project_config = self._project_config_manager.get_project_config(
-            algorithm_file.parent
-        )
-        config["parameters"] = project_config.get("parameters", {})
-
-        if self._module_manager.is_module_installed(GUI_PRODUCT_INSTALL_ID):
-            config["messaging-handler"] = "QuantConnect.GUI.LocalMessagingHandler"
-
-        return config
-
-    def configure_data_purchase_limit(
-        self, lean_config: Dict[str, Any], data_purchase_limit: Optional[int]
-    ) -> None:
-        """Updates the data purchase limit in the Lean config.
-
-        Logs a warning if the data provider is not configured to download from QuantConnect.
-
-        :param lean_config: the Lean config dict to update
-        :param data_purchase_limit: the data purchase limit provided by the user, or None if no such limit was provided
-        """
-        if data_purchase_limit is None:
-            return
-
-        if (
-            lean_config.get("data-provider", None)
-            != "QuantConnect.Lean.Engine.DataFeeds.ApiDataProvider"
-        ):
-            self._logger.warn(
-                "--data-purchase-limit is ignored because the data provider is not set to download from the QuantConnect API, use --download-data to set that up"
-            )
-            return
-
-        lean_config["data-purchase-limit"] = data_purchase_limit
-
-    def get_lean_config(self) -> Dict[str, Any]:
-        """Reads the Lean config into a dict.
-
-        :return: a dict containing the contents of the Lean config file
-        """
-        return json5.loads(self.get_lean_config_path().read_text(encoding="utf-8"))
+# QUANTCONNECT.COM - Democratizing Finance, Empowering Individuals.
+# Lean CLI v1.0. Copyright 2021 QuantConnect Corporation.
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+
+import os
+import re
+from pathlib import Path
+from typing import Any, Dict, Optional, List
+
+import json5
+
+from ablean.components.config.cli_config_manager import CLIConfigManager
+from ablean.components.config.project_config_manager import ProjectConfigManager
+from ablean.components.module_manager import ModuleManager
+from ablean.components.config.storage import Storage
+from ablean.components.util.logger import Logger
+from ablean.constants import DEFAULT_LEAN_CONFIG_FILE_NAME, ENV_LEAN_PATH_NAME, GUI_PRODUCT_INSTALL_ID
+from ablean.models.errors import MoreInfoError
+from ablean.models.utils import DebuggingMethod
+
+
+class LeanConfigManager:
+    """The LeanConfigManager class contains utilities to work with files containing LEAN engine configuration."""
+
+    def __init__(
+        self,
+        logger: Logger,
+        cli_config_manager: CLIConfigManager,
+        project_config_manager: ProjectConfigManager,
+        module_manager: ModuleManager,
+        cache_storage: Storage,
+    ) -> None:
+        """Creates a new LeanConfigManager instance.
+
+        :param logger: the logger to log messages with
+        :param cache_storage: the Storage instance to store known Lean config paths in
+        """
+        self._logger = logger
+        self._module_manager = module_manager
+        self._cli_config_manager = cli_config_manager
+        self._project_config_manager = project_config_manager
+        self._cache_storage = cache_storage
+        self._default_path = None
+        self._lean_config_path = None
+
+    def get_lean_config_path(self) -> Path:
+        """Returns the path to the closest Lean config file.
+
+        This recurses upwards in the directory tree looking for a Lean config file.
+        This search can be overridden using set_default_lean_config_path().
+
+        Raises an error if no Lean config file can be found.
+
+        :return: the path to the closest Lean config file
+        """
+        if self._default_path is not None:
+            return self._default_path
+
+        if self._lean_config_path is not None:
+            return self._lean_config_path
+
+        # Recurse upwards in the directory tree until we find a Lean config file
+        list = self.get_search_paths()
+        for current_dir in list:
+            target_file = os.path.join(current_dir, DEFAULT_LEAN_CONFIG_FILE_NAME)
+            if target_file.exists():
+                self._lean_config_path = target_file
+                self.store_known_lean_config_path(self._lean_config_path)
+                return self._lean_config_path
+            
+        raise MoreInfoError(
+            f"'{DEFAULT_LEAN_CONFIG_FILE_NAME}' not found",
+            "https://www.lean.io/docs/lean-cli/initialization/configuration#03-Lean-Configuration",
+        )
+    
+    def get_search_paths(self):
+        current_dir = Path.cwd()
+        dirs = [current_dir]
+        while True:
+            # If the parent directory is the same as the current directory we can't go up any more
+            if current_dir.parent == current_dir:
+                break
+            current_dir = current_dir.parent              
+            dirs.append(current_dir)
+        v = os.environ.get(ENV_LEAN_PATH_NAME)
+        if  v is not None:
+            dirs.append(Path(v))
+        return dirs
+
+    def set_default_lean_config_path(self, path: Path) -> None:
+        """Overrides the default search for the path to the Lean config file.
+
+        :param path: the path to the Lean config file to return in future calls to get_lean_config_path()
+        """
+        self.store_known_lean_config_path(path)
+        self._default_path = path
+
+    def get_known_lean_config_paths(self) -> List[Path]:
+        """Returns the known Lean config file paths.
+
+        :return: a list of paths to Lean config files that were used in the past
+        """
+        lean_config_paths = self._cache_storage.get("known-lean-config-paths", [])
+        lean_config_paths = [Path(p) for p in lean_config_paths]
+        lean_config_paths = [p for p in lean_config_paths if p.is_file()]
+
+        self._cache_storage.set(
+            "known-lean-config-paths", [str(p) for p in lean_config_paths]
+        )
+
+        return lean_config_paths
+
+    def store_known_lean_config_path(self, path: Path) -> None:
+        """Caches a path as being a known Lean configuration file path.
+
+        :param path: the path to the Lean configuration file
+        """
+        lean_config_paths = set(self._cache_storage.get("known-lean-config-paths", []))
+        lean_config_paths.add(str(path))
+        self._cache_storage.set("known-lean-config-paths", list(lean_config_paths))
+
+    def get_cli_root_directory(self) -> Path:
+        """Returns the path to the directory containing the Lean config file.
+
+        :return: the path to the directory containing the Lean config file
+        """
+        return self.get_lean_config_path().parent
+
+    def get_data_directory(self) -> Path:
+        """Returns the path to the data directory.
+
+        :return: the path to the data directory as it is configured in the Lean config
+        """
+        config = self.get_lean_config()
+        return self.get_cli_root_directory() / config["data-folder"]
+
+    def set_properties(self, updates: Dict[str, Any]) -> None:
+        """Sets a properties in the Lean config file.
+
+        If a property does not exist yet it is added automatically.
+        Comments in the Lean config file are preserved.
+
+        :param updates: the key -> new value updates to apply to the current config
+        """
+        config = self.get_lean_config()
+
+        config_path = self.get_lean_config_path()
+        config_text = config_path.read_text(encoding="utf-8")
+
+        for key, value in reversed(list(updates.items())):
+            if value is None:
+                continue
+            json_value = json5.dumps(value)
+
+            # We can only use regex to set the property because converting the config back to JSON drops all comments
+            if key in config:
+                config_text = re.sub(
+                    fr'"{key}":\s*("?[^",]*"?)', f'"{key}": {json_value}', config_text
+                )
+            else:
+                config_text = config_text.replace(
+                    "{", f'{{\n  "{key}": {json_value},', 1
+                )
+
+        config_path.write_text(config_text, encoding="utf-8")
+
+    def clean_lean_config(self, config: str) -> str:
+        """Removes the properties from a Lean config file which can be set in get_complete_lean_config().
+
+        This removes all the properties which the CLI can configure automatically based on the command that is ran.
+
+        For example, given the following config:
+        {
+            // Environment docs
+            "environment": "backtesting",
+
+            // Key2 docs
+            "key2": "value2"
+        }
+
+        Calling clean_lean_config(config) would return the following:
+        {
+            // Key2 docs
+            "key2": "value2"
+        }
+
+        Because "environment" can be set automatically based on the command that is ran.
+
+        :param config: the configuration to remove the auto-configurable keys from
+        :return: the same config as passed in with the config argument, but without the auto-configurable keys
+        """
+        # The keys that we can set automatically based on the command that is ran
+        keys_to_remove = [
+            "environment",
+            "composer-dll-directory",
+            "debugging",
+            "debugging-method",
+            "job-user-id",
+            "api-access-token",
+            "algorithm-type-name",
+            "algorithm-language",
+            "algorithm-location",
+            "parameters",
+            "intrinio-username",
+            "intrinio-password",
+            "ema-fast",
+            "ema-slow",
+        ]
+
+        # This function is implemented by doing string manipulation because the config contains comments
+        # If we were to parse it as JSON, we would have to remove the comments, which we don't want to do
+        sections = re.split(r"\n\s*\n", config)
+        for key in keys_to_remove:
+            sections = [
+                section for section in sections if f"\"{key}\": " not in section
+            ]
+        config = "\n\n".join(sections)
+
+        # For some keys we should only remove the key itself, instead of their entire section
+        lines = config.split("\n")
+        for key in ["ib-host", "ib-port", "ib-tws-dir", "ib-version"]:
+            lines = [line for line in lines if f"\"{key}\": " not in line]
+        config = "\n".join(lines)
+
+        # Instead of setting the IQFeed host we require the user to set the IQConnect location
+        config = config.replace(
+            '"iqfeed-host": "127.0.0.1"',
+            '"iqfeed-iqconnect": "C:/Program Files (x86)/DTN/IQFeed/iqconnect.exe"',
+        )
+
+        return config
+
+    def get_complete_lean_config(
+        self,
+        environment: str,
+        algorithm_file: Path,
+        output: Path,
+        debugging_method: Optional[DebuggingMethod],
+    ) -> Dict[str, Any]:
+        """Returns a complete Lean config object containing all properties needed for the engine to run.
+
+        This retrieves the path of the config, parses the file and adds all properties removed in clean_lean_config().
+
+        :param environment: the environment to set
+        :param algorithm_file: the path to the algorithm that will be ran
+        :param debugging_method: the debugging method to use, or None to disable debugging
+        """
+        config = self.get_lean_config()
+
+        config["environment"] = environment
+        config["close-automatically"] = True
+
+        config["composer-dll-directory"] = str(self.get_cli_root_directory() / "launcher")
+        config["results-destination-folder"] = str(output)
+
+        if debugging_method is not None:
+            config["debugging"] = True
+            config["debugging-method"] = debugging_method.get_internal_name()
+        else:
+            config["debugging"] = False
+            config["debugging-method"] = "LocalCmdline"
+
+        # The following key -> value pairs are added to the config unless they are already set by the user
+        config_defaults = {
+            "job-user-id": self._cli_config_manager.user_id.get_value(default="0"),
+            "api-access-token": self._cli_config_manager.api_token.get_value(
+                default=""
+            ),
+            "job-project-id": self._project_config_manager.get_local_id(
+                algorithm_file.parent
+            ),
+            "ib-host": "127.0.0.1",
+            "ib-port": "4002",
+            "ib-tws-dir": "/root/Jts",
+            "ib-version": "985",
+            "iqfeed-host": "host.docker.internal",
+        }
+
+        for key, value in config_defaults.items():
+            if config.get(key, "") == "":
+                config[key] = value
+
+        if algorithm_file.name.endswith(".py"):
+            config["algorithm-type-name"] = algorithm_file.name.split(".")[0]
+            config["algorithm-language"] = "Python"
+            config["algorithm-location"] = str(algorithm_file)
+        else:
+            algorithm_text = algorithm_file.read_text(encoding="utf-8")
+            config["algorithm-type-name"] = re.findall(
+                r"class\s*([^\s:]+)\s*:\s*QCAlgorithm", algorithm_text
+            )[0]
+            config["algorithm-language"] = "CSharp"
+            config["algorithm-location"] = f"{algorithm_file.parent.name}.dll"
+
+        project_config = self._project_config_manager.get_project_config(
+            algorithm_file.parent
+        )
+        config["parameters"] = project_config.get("parameters", {})
+
+        if self._module_manager.is_module_installed(GUI_PRODUCT_INSTALL_ID):
+            config["messaging-handler"] = "QuantConnect.GUI.LocalMessagingHandler"
+
+        return config
+
+    def configure_data_purchase_limit(
+        self, lean_config: Dict[str, Any], data_purchase_limit: Optional[int]
+    ) -> None:
+        """Updates the data purchase limit in the Lean config.
+
+        Logs a warning if the data provider is not configured to download from QuantConnect.
+
+        :param lean_config: the Lean config dict to update
+        :param data_purchase_limit: the data purchase limit provided by the user, or None if no such limit was provided
+        """
+        if data_purchase_limit is None:
+            return
+
+        if (
+            lean_config.get("data-provider", None)
+            != "QuantConnect.Lean.Engine.DataFeeds.ApiDataProvider"
+        ):
+            self._logger.warn(
+                "--data-purchase-limit is ignored because the data provider is not set to download from the QuantConnect API, use --download-data to set that up"
+            )
+            return
+
+        lean_config["data-purchase-limit"] = data_purchase_limit
+
+    def get_lean_config(self) -> Dict[str, Any]:
+        """Reads the Lean config into a dict.
+
+        :return: a dict containing the contents of the Lean config file
+        """
+        return json5.loads(self.get_lean_config_path().read_text(encoding="utf-8"))
```

### Comparing `ablean-1.3.7/ablean/components/config/output_config_manager.py` & `ablean-1.3.8/ablean/components/config/output_config_manager.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,115 +1,115 @@
-# QUANTCONNECT.COM - Democratizing Finance, Empowering Individuals.
-# Lean CLI v1.0. Copyright 2021 QuantConnect Corporation.
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-
-import random
-from pathlib import Path
-from typing import List, Optional
-
-from ablean.components.config.lean_config_manager import LeanConfigManager
-from ablean.components.config.storage import Storage
-
-
-class OutputConfigManager:
-    """The OutputConfigManager class manages the configuration of a backtest, optimization or live trading session."""
-
-    def __init__(self, lean_config_manager: LeanConfigManager) -> None:
-        """Creates a new OutputConfigManager instance.
-
-        :param lean_config_manager: the LeanConfigManager to get the CLI root directory from
-        """
-        self._lean_config_manager = lean_config_manager
-
-    def get_output_config(self, output_directory: Path) -> Storage:
-        """Returns a Storage instance to get/set the configuration of the contents of an output directory.
-
-        :param output_directory: the path to the project to retrieve the configuration of
-        :return: the Storage instance containing the configuration of the given backtest/optimization/live trading
-        """
-        return Storage(str(output_directory / "config"))
-
-    def get_backtest_id(self, backtest_directory: Path) -> int:
-        """Returns the id of a backtest.
-
-        :param backtest_directory: the path to the backtest to retrieve the id of
-        :return: the id of the given backtest
-        """
-        return self._get_id(backtest_directory, 1)
-
-    def get_backtest_by_id(self, backtest_id: int, root_directory: Optional[Path] = None) -> Path:
-        """Finds the directory of a backtest by its id.
-
-        :param backtest_id: the id of the backtest to get the directory of
-        :param root_directory: the directory to search from, defaults to the `lean init` directory
-        :return: the output directory of the backtest with the given id
-        """
-        return self._get_by_id("Backtest", backtest_id, ["backtests/*", "optimizations/*/*"], root_directory)
-
-    def get_optimization_id(self, optimization_directory: Path) -> int:
-        """Returns the id of an optimization.
-
-        :param optimization_directory: the path to the optimization to retrieve the id of
-        :return: the id of the given optimization
-        """
-        return self._get_id(optimization_directory, 2)
-
-    def get_optimization_by_id(self, optimization_id: int, root_directory: Optional[Path] = None) -> Path:
-        """Finds the directory of an optimization by its id.
-
-        :param optimization_id: the id of the optimization to get the directory of
-        :param root_directory: the directory to search from, defaults to the `lean init` directory
-        :return: the output directory of the optimization with the given id
-        """
-        return self._get_by_id("Optimization", optimization_id, ["optimizations/*"], root_directory)
-
-    def get_live_deployment_id(self, live_deployment_directory: Path) -> int:
-        """Returns the id of a live deployment.
-
-        :param live_deployment_directory: the path to the live deployment to retrieve the id of
-        :return: the id of the given optimization
-        """
-        return self._get_id(live_deployment_directory, 3)
-
-    def get_live_deployment_by_id(self, live_deployment_id: int, root_directory: Optional[Path] = None) -> Path:
-        """Finds the directory of a live deployment by its id.
-
-        :param live_deployment_id: the id of the live deployment to get the directory of
-        :param root_directory: the directory to search from, defaults to the `lean init` directory
-        :return: the output directory of the live deployment with the given id
-        """
-        return self._get_by_id("Live deployment", live_deployment_id, ["live/*"], root_directory)
-
-    def _get_id(self, output_directory: Path, prefix: int) -> int:
-        config = self.get_output_config(output_directory)
-
-        if config.has("id"):
-            return config.get("id")
-
-        new_id = int(str(prefix) + str(random.randint(100_000_000, 999_999_999)))
-        config.set("id", new_id)
-
-        return new_id
-
-    def _get_by_id(self, label: str, object_id: int, patterns: List[str], root_directory: Optional[Path]) -> Path:
-        if root_directory is None:
-            root_directory = self._lean_config_manager.get_cli_root_directory()
-
-        for pattern in patterns:
-            for directory in root_directory.rglob(pattern):
-                if not directory.is_dir():
-                    continue
-
-                config = self.get_output_config(directory)
-                if config.get("id", None) == object_id:
-                    return directory
-
-        raise ValueError(f"{label} with id '{object_id}' does not exist")
+# QUANTCONNECT.COM - Democratizing Finance, Empowering Individuals.
+# Lean CLI v1.0. Copyright 2021 QuantConnect Corporation.
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+
+import random
+from pathlib import Path
+from typing import List, Optional
+
+from ablean.components.config.lean_config_manager import LeanConfigManager
+from ablean.components.config.storage import Storage
+
+
+class OutputConfigManager:
+    """The OutputConfigManager class manages the configuration of a backtest, optimization or live trading session."""
+
+    def __init__(self, lean_config_manager: LeanConfigManager) -> None:
+        """Creates a new OutputConfigManager instance.
+
+        :param lean_config_manager: the LeanConfigManager to get the CLI root directory from
+        """
+        self._lean_config_manager = lean_config_manager
+
+    def get_output_config(self, output_directory: Path) -> Storage:
+        """Returns a Storage instance to get/set the configuration of the contents of an output directory.
+
+        :param output_directory: the path to the project to retrieve the configuration of
+        :return: the Storage instance containing the configuration of the given backtest/optimization/live trading
+        """
+        return Storage(str(output_directory / "config"))
+
+    def get_backtest_id(self, backtest_directory: Path) -> int:
+        """Returns the id of a backtest.
+
+        :param backtest_directory: the path to the backtest to retrieve the id of
+        :return: the id of the given backtest
+        """
+        return self._get_id(backtest_directory, 1)
+
+    def get_backtest_by_id(self, backtest_id: int, root_directory: Optional[Path] = None) -> Path:
+        """Finds the directory of a backtest by its id.
+
+        :param backtest_id: the id of the backtest to get the directory of
+        :param root_directory: the directory to search from, defaults to the `lean init` directory
+        :return: the output directory of the backtest with the given id
+        """
+        return self._get_by_id("Backtest", backtest_id, ["backtests/*", "optimizations/*/*"], root_directory)
+
+    def get_optimization_id(self, optimization_directory: Path) -> int:
+        """Returns the id of an optimization.
+
+        :param optimization_directory: the path to the optimization to retrieve the id of
+        :return: the id of the given optimization
+        """
+        return self._get_id(optimization_directory, 2)
+
+    def get_optimization_by_id(self, optimization_id: int, root_directory: Optional[Path] = None) -> Path:
+        """Finds the directory of an optimization by its id.
+
+        :param optimization_id: the id of the optimization to get the directory of
+        :param root_directory: the directory to search from, defaults to the `lean init` directory
+        :return: the output directory of the optimization with the given id
+        """
+        return self._get_by_id("Optimization", optimization_id, ["optimizations/*"], root_directory)
+
+    def get_live_deployment_id(self, live_deployment_directory: Path) -> int:
+        """Returns the id of a live deployment.
+
+        :param live_deployment_directory: the path to the live deployment to retrieve the id of
+        :return: the id of the given optimization
+        """
+        return self._get_id(live_deployment_directory, 3)
+
+    def get_live_deployment_by_id(self, live_deployment_id: int, root_directory: Optional[Path] = None) -> Path:
+        """Finds the directory of a live deployment by its id.
+
+        :param live_deployment_id: the id of the live deployment to get the directory of
+        :param root_directory: the directory to search from, defaults to the `lean init` directory
+        :return: the output directory of the live deployment with the given id
+        """
+        return self._get_by_id("Live deployment", live_deployment_id, ["live/*"], root_directory)
+
+    def _get_id(self, output_directory: Path, prefix: int) -> int:
+        config = self.get_output_config(output_directory)
+
+        if config.has("id"):
+            return config.get("id")
+
+        new_id = int(str(prefix) + str(random.randint(100_000_000, 999_999_999)))
+        config.set("id", new_id)
+
+        return new_id
+
+    def _get_by_id(self, label: str, object_id: int, patterns: List[str], root_directory: Optional[Path]) -> Path:
+        if root_directory is None:
+            root_directory = self._lean_config_manager.get_cli_root_directory()
+
+        for pattern in patterns:
+            for directory in root_directory.rglob(pattern):
+                if not directory.is_dir():
+                    continue
+
+                config = self.get_output_config(directory)
+                if config.get("id", None) == object_id:
+                    return directory
+
+        raise ValueError(f"{label} with id '{object_id}' does not exist")
```

### Comparing `ablean-1.3.7/ablean/components/config/project_config_manager.py` & `ablean-1.3.8/ablean/components/config/project_config_manager.py`

 * *Ordering differences only*

 * *Files 8% similar despite different names*

```diff
@@ -1,57 +1,57 @@
-# QUANTCONNECT.COM - Democratizing Finance, Empowering Individuals.
-# Lean CLI v1.0. Copyright 2021 QuantConnect Corporation.
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-
-import random
-from pathlib import Path
-from typing import List
-
-from ablean.components.config.storage import Storage
-from ablean.components.util.xml_manager import XMLManager
-from ablean.constants import PROJECT_CONFIG_FILE_NAME
-
-
-class ProjectConfigManager:
-    """The ProjectConfigManager class manages the configuration of a single project."""
-
-    def __init__(self, xml_manager: XMLManager) -> None:
-        """Creates a new ProjectConfigManager instance.
-
-        :param xml_manager: the XMLManager instance to use when parsing XML files
-        """
-        self._xml_manager = xml_manager
-
-    def get_project_config(self, project_directory: Path) -> Storage:
-        """Returns a Storage instance to get/set the configuration for a project.
-
-        :param project_directory: the path to the project to retrieve the configuration of
-        :return: the Storage instance containing the project-specific configuration of the given project
-        """
-        return Storage(str(project_directory / PROJECT_CONFIG_FILE_NAME))
-
-    def get_local_id(self, project_directory: Path) -> int:
-        """Returns the local id of a project.
-
-        Every Lean CLI project has a unique local id, regardless of whether the project is synchronized with the cloud.
-
-        :param project_directory: the path to the project to retrieve the local id of
-        :return: the local id of the given project
-        """
-        project_config = self.get_project_config(project_directory)
-
-        if project_config.has("local-id"):
-            return project_config.get("local-id")
-
-        project_id = random.randint(100_000_000, 999_999_999)
-        project_config.set("local-id", project_id)
-
-        return project_id
+# QUANTCONNECT.COM - Democratizing Finance, Empowering Individuals.
+# Lean CLI v1.0. Copyright 2021 QuantConnect Corporation.
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+
+import random
+from pathlib import Path
+from typing import List
+
+from ablean.components.config.storage import Storage
+from ablean.components.util.xml_manager import XMLManager
+from ablean.constants import PROJECT_CONFIG_FILE_NAME
+
+
+class ProjectConfigManager:
+    """The ProjectConfigManager class manages the configuration of a single project."""
+
+    def __init__(self, xml_manager: XMLManager) -> None:
+        """Creates a new ProjectConfigManager instance.
+
+        :param xml_manager: the XMLManager instance to use when parsing XML files
+        """
+        self._xml_manager = xml_manager
+
+    def get_project_config(self, project_directory: Path) -> Storage:
+        """Returns a Storage instance to get/set the configuration for a project.
+
+        :param project_directory: the path to the project to retrieve the configuration of
+        :return: the Storage instance containing the project-specific configuration of the given project
+        """
+        return Storage(str(project_directory / PROJECT_CONFIG_FILE_NAME))
+
+    def get_local_id(self, project_directory: Path) -> int:
+        """Returns the local id of a project.
+
+        Every Lean CLI project has a unique local id, regardless of whether the project is synchronized with the cloud.
+
+        :param project_directory: the path to the project to retrieve the local id of
+        :return: the local id of the given project
+        """
+        project_config = self.get_project_config(project_directory)
+
+        if project_config.has("local-id"):
+            return project_config.get("local-id")
+
+        project_id = random.randint(100_000_000, 999_999_999)
+        project_config.set("local-id", project_id)
+
+        return project_id
```

### Comparing `ablean-1.3.7/ablean/components/config/storage.py` & `ablean-1.3.8/ablean/components/config/storage.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,95 +1,95 @@
-# QUANTCONNECT.COM - Democratizing Finance, Empowering Individuals.
-# Lean CLI v1.0. Copyright 2021 QuantConnect Corporation.
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-
-import json
-from pathlib import Path
-from typing import Any
-
-import json5
-
-
-class Storage:
-    """A Storage instance manages the data in a single JSON file."""
-
-    def __init__(self, file: str) -> None:
-        """Creates a new Storage instance.
-
-        :param file: the path to the file this Storage instance should manage
-        """
-        self.file = Path(file)
-
-        if self.file.exists():
-            self._data = json5.loads(self.file.read_text(encoding="utf-8"))
-        else:
-            self._data = {}
-
-    @property
-    def data(self):
-        return self._data
-
-    def get(self, key: str, default: Any = None) -> Any:
-        """Returns the value assigned to the given key.
-
-        Returns a default value when nothing is assigned to the given key.
-
-        :param key: the key to retrieve the value of
-        :param default: the default value to return when key is not set
-        :return: the value assigned to the key or default if the key is not set
-        """
-        if key in self._data:
-            return self._data[key]
-        else:
-            return default
-
-    def set(self, key: str, value: Any) -> None:
-        """Assigns a value to a key.
-
-        The value is stored as json, so must be serializable using json.dump().
-
-        :param key: the key to assign the value to
-        :param value: the json-serializable value to assign to the given key
-        """
-        self._data[key] = value
-        self._save()
-
-    def delete(self, key: str) -> None:
-        """Deletes a key.
-
-        :param key: the key to delete
-        """
-        self._data.pop(key, None)
-        self._save()
-
-    def has(self, key: str) -> bool:
-        """Returns whether the Storage instance has a value assigned to the given key.
-
-        :param key: the key to check the existence of
-        :return: True if a value is assigned to the given key, False if not
-        """
-        return key in self._data
-
-    def clear(self) -> None:
-        """Clears the Storage instance and deletes the underlying file."""
-        self._data.clear()
-        self._save()
-
-    def _save(self) -> None:
-        """Saves the data to the underlying file, deleting the file if there is no data."""
-        if len(self._data) > 0:
-            self.file.parent.mkdir(parents=True, exist_ok=True)
-
-            with self.file.open("w+", encoding="utf-8") as file:
-                file.write(json.dumps(self._data, indent=4) + "\n")
-        else:
-            if self.file.exists():
-                self.file.unlink()
+# QUANTCONNECT.COM - Democratizing Finance, Empowering Individuals.
+# Lean CLI v1.0. Copyright 2021 QuantConnect Corporation.
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+
+import json
+from pathlib import Path
+from typing import Any
+
+import json5
+
+
+class Storage:
+    """A Storage instance manages the data in a single JSON file."""
+
+    def __init__(self, file: str) -> None:
+        """Creates a new Storage instance.
+
+        :param file: the path to the file this Storage instance should manage
+        """
+        self.file = Path(file)
+
+        if self.file.exists():
+            self._data = json5.loads(self.file.read_text(encoding="utf-8"))
+        else:
+            self._data = {}
+
+    @property
+    def data(self):
+        return self._data
+
+    def get(self, key: str, default: Any = None) -> Any:
+        """Returns the value assigned to the given key.
+
+        Returns a default value when nothing is assigned to the given key.
+
+        :param key: the key to retrieve the value of
+        :param default: the default value to return when key is not set
+        :return: the value assigned to the key or default if the key is not set
+        """
+        if key in self._data:
+            return self._data[key]
+        else:
+            return default
+
+    def set(self, key: str, value: Any) -> None:
+        """Assigns a value to a key.
+
+        The value is stored as json, so must be serializable using json.dump().
+
+        :param key: the key to assign the value to
+        :param value: the json-serializable value to assign to the given key
+        """
+        self._data[key] = value
+        self._save()
+
+    def delete(self, key: str) -> None:
+        """Deletes a key.
+
+        :param key: the key to delete
+        """
+        self._data.pop(key, None)
+        self._save()
+
+    def has(self, key: str) -> bool:
+        """Returns whether the Storage instance has a value assigned to the given key.
+
+        :param key: the key to check the existence of
+        :return: True if a value is assigned to the given key, False if not
+        """
+        return key in self._data
+
+    def clear(self) -> None:
+        """Clears the Storage instance and deletes the underlying file."""
+        self._data.clear()
+        self._save()
+
+    def _save(self) -> None:
+        """Saves the data to the underlying file, deleting the file if there is no data."""
+        if len(self._data) > 0:
+            self.file.parent.mkdir(parents=True, exist_ok=True)
+
+            with self.file.open("w+", encoding="utf-8") as file:
+                file.write(json.dumps(self._data, indent=4) + "\n")
+        else:
+            if self.file.exists():
+                self.file.unlink()
```

### Comparing `ablean-1.3.7/ablean/components/lean_runner.py` & `ablean-1.3.8/ablean/components/lean_runner.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,112 +1,108 @@
-# QUANTCONNECT.COM - Democratizing Finance, Empowering Individuals.
-# Lean CLI v1.0. Copyright 2021 QuantConnect Corporation.
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-
-import json
-import os
-import re
-import subprocess
-import uuid
-from datetime import datetime
-from pathlib import Path
-from typing import Any, Dict, Optional, List
-
-from pkg_resources import Requirement
-
-from ablean.components.module_manager import ModuleManager
-from ablean.components.config.lean_config_manager import LeanConfigManager
-from ablean.components.config.output_config_manager import OutputConfigManager
-from ablean.components.config.project_config_manager import ProjectConfigManager
-from ablean.components.util.logger import Logger
-from ablean.components.util.project_manager import ProjectManager
-from ablean.components.util.temp_manager import TempManager
-from ablean.components.util.xml_manager import XMLManager
-from ablean.constants import MODULES_DIRECTORY, TERMINAL_LINK_PRODUCT_ID, PROJECT_CONFIG_FILE_NAME
-from ablean.models.utils import DebuggingMethod
-
-
-class LeanRunner:
-    """The LeanRunner class contains the code that runs the LEAN engine locally."""
-
-    def __init__(
-        self,
-        logger: Logger,
-        project_config_manager: ProjectConfigManager,
-        lean_config_manager: LeanConfigManager,
-        output_config_manager: OutputConfigManager,
-        module_manager: ModuleManager,
-        project_manager: ProjectManager,
-        temp_manager: TempManager,
-        xml_manager: XMLManager,
-    ) -> None:
-        """Creates a new LeanRunner instance.
-
-        :param logger: the logger that is used to print messages
-        :param project_config_manager: the ProjectConfigManager instance to retrieve project configuration from
-        :param lean_config_manager: the LeanConfigManager instance to retrieve Lean configuration from
-        :param output_config_manager: the OutputConfigManager instance to retrieve backtest/live configuration from
-        :param docker_manager: the DockerManager instance which is used to interact with Docker
-        :param module_manager: the ModuleManager instance to retrieve the installed modules from
-        :param project_manager: the ProjectManager instance to use for copying source code to output directories
-        :param temp_manager: the TempManager instance to use for creating temporary directories
-        :param xml_manager: the XMLManager instance to use for reading/writing XML files
-        """
-        self._logger = logger
-        self._project_config_manager = project_config_manager
-        self._lean_config_manager = lean_config_manager
-        self._output_config_manager = output_config_manager
-        self._module_manager = module_manager
-        self._project_manager = project_manager
-        self._temp_manager = temp_manager
-        self._xml_manager = xml_manager
-
-    def run_lean(
-        self,
-        lean_config: Dict[str, Any],
-        environment: str,
-        algorithm_file: Path,
-        output_dir: Path
-    ) -> None:
-        """Runs the LEAN engine locally in Docker.
-
-        Raises an error if something goes wrong.
-
-        :param lean_config: the LEAN configuration to use
-        :param environment: the environment to run the algorithm in
-        :param algorithm_file: the path to the file containing the algorithm
-        :param output_dir: the directory to save output data to
-        :param debugging_method: the debugging method if debugging needs to be enabled, None if not
-        """
-        project_dir = algorithm_file.parent
-
-        # Copy the project's code to the output directory
-        self._project_manager.copy_code(algorithm_file.parent, output_dir / "code")
-
-        cli_root_dir = self._lean_config_manager.get_cli_root_directory()
-        try:
-            relative_project_dir = project_dir.relative_to(cli_root_dir)
-            relative_output_dir = output_dir.relative_to(cli_root_dir)
-        except:
-            relative_project_dir = project_dir
-            relative_output_dir = output_dir
-            
-        # Save config.json to ouput
-        config_path = output_dir / PROJECT_CONFIG_FILE_NAME
-        with config_path.open("w+", encoding="utf-8") as file:
-            file.write(json.dumps(lean_config, indent=4))
-        
-        cwd = str(cli_root_dir.joinpath("launcher"))
-        subprocess.run(["dotnet", "QuantConnect.Lean.Launcher.dll", "--config", f"{str(config_path)}"], cwd=cwd)
-
-        self._logger.info(
-            f"Successfully ran '{relative_project_dir}' in the '{environment}' environment and stored the output in '{relative_output_dir}'"
+# QUANTCONNECT.COM - Democratizing Finance, Empowering Individuals.
+# Lean CLI v1.0. Copyright 2021 QuantConnect Corporation.
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+
+import json
+import os
+import re
+import subprocess
+import uuid
+from datetime import datetime
+from pathlib import Path
+from typing import Any, Dict, Optional, List
+
+from pkg_resources import Requirement
+
+from ablean.components.module_manager import ModuleManager
+from ablean.components.config.lean_config_manager import LeanConfigManager
+from ablean.components.config.output_config_manager import OutputConfigManager
+from ablean.components.config.project_config_manager import ProjectConfigManager
+from ablean.components.util.logger import Logger
+from ablean.components.util.project_manager import ProjectManager
+from ablean.components.util.temp_manager import TempManager
+from ablean.components.util.xml_manager import XMLManager
+from ablean.constants import MODULES_DIRECTORY, TERMINAL_LINK_PRODUCT_ID, PROJECT_CONFIG_FILE_NAME
+from ablean.models.utils import DebuggingMethod
+
+
+class LeanRunner:
+    """The LeanRunner class contains the code that runs the LEAN engine locally."""
+
+    def __init__(
+        self,
+        logger: Logger,
+        project_config_manager: ProjectConfigManager,
+        lean_config_manager: LeanConfigManager,
+        output_config_manager: OutputConfigManager,
+        module_manager: ModuleManager,
+        project_manager: ProjectManager,
+        temp_manager: TempManager,
+        xml_manager: XMLManager,
+    ) -> None:
+        """Creates a new LeanRunner instance.
+
+        :param logger: the logger that is used to print messages
+        :param project_config_manager: the ProjectConfigManager instance to retrieve project configuration from
+        :param lean_config_manager: the LeanConfigManager instance to retrieve Lean configuration from
+        :param output_config_manager: the OutputConfigManager instance to retrieve backtest/live configuration from
+        :param docker_manager: the DockerManager instance which is used to interact with Docker
+        :param module_manager: the ModuleManager instance to retrieve the installed modules from
+        :param project_manager: the ProjectManager instance to use for copying source code to output directories
+        :param temp_manager: the TempManager instance to use for creating temporary directories
+        :param xml_manager: the XMLManager instance to use for reading/writing XML files
+        """
+        self._logger = logger
+        self._project_config_manager = project_config_manager
+        self._lean_config_manager = lean_config_manager
+        self._output_config_manager = output_config_manager
+        self._module_manager = module_manager
+        self._project_manager = project_manager
+        self._temp_manager = temp_manager
+        self._xml_manager = xml_manager
+
+    def run_lean(
+        self,
+        lean_config: Dict[str, Any],
+        environment: str,
+        algorithm_file: Path,
+        output_dir: Path
+    ) -> None:
+        """Runs the LEAN engine locally in Docker.
+
+        Raises an error if something goes wrong.
+
+        :param lean_config: the LEAN configuration to use
+        :param environment: the environment to run the algorithm in
+        :param algorithm_file: the path to the file containing the algorithm
+        :param output_dir: the directory to save output data to
+        :param debugging_method: the debugging method if debugging needs to be enabled, None if not
+        """
+        project_dir = algorithm_file.parent
+
+        # Copy the project's code to the output directory
+        self._project_manager.copy_code(algorithm_file.parent, output_dir / "code")
+
+        cli_root_dir = self._lean_config_manager.get_cli_root_directory()
+        relative_project_dir = project_dir.relative_to(cli_root_dir)
+        relative_output_dir = output_dir.relative_to(cli_root_dir)
+        
+        # Save config.json to ouput
+        config_path = output_dir / PROJECT_CONFIG_FILE_NAME
+        with config_path.open("w+", encoding="utf-8") as file:
+            file.write(json.dumps(lean_config, indent=4))
+        
+        cwd = str(cli_root_dir.joinpath("launcher"))
+        subprocess.run(["dotnet", "QuantConnect.Lean.Launcher.dll", "--config", f"{str(config_path)}"], cwd=cwd)
+
+        self._logger.info(
+            f"Successfully ran '{relative_project_dir}' in the '{environment}' environment and stored the output in '{relative_output_dir}'"
         )
```

### Comparing `ablean-1.3.7/ablean/components/module_manager.py` & `ablean-1.3.8/ablean/components/module_manager.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,60 +1,60 @@
-# QUANTCONNECT.COM - Democratizing Finance, Empowering Individuals.
-# Lean CLI v1.0. Copyright 2021 QuantConnect Corporation.
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-
-from pathlib import Path
-from typing import Set, List, Dict
-
-from ablean.components.util.logger import Logger
-from ablean.constants import MODULES_DIRECTORY
-from ablean.models.modules import NuGetPackage
-
-
-class ModuleManager:
-    """The ModuleManager class is responsible for downloading and updating modules."""
-
-    def __init__(self, logger: Logger) -> None:
-        """Creates a new ModuleManager instance.
-
-        :param logger: the logger to use
-        :param api_client: the APIClient instance to use when communicating with the cloud
-        :param http_client: the HTTPClient instance to use when downloading modules
-        """
-        self._logger = logger
-        self._installed_product_ids: Set[int] = set()
-        self._installed_packages: Dict[int, List[NuGetPackage]] = {}
-
-    def get_installed_packages(self) -> List[NuGetPackage]:
-        """Returns a list of NuGet packages that were installed by install_module() calls.
-
-        :return: a list of NuGet packages in the modules directory that should be made available when running LEAN
-        """
-        packages = []
-        for package_list in self._installed_packages.values():
-            packages.extend(package_list)
-        return packages
-
-    def get_installed_packages_by_module(self, product_id: int) -> List[NuGetPackage]:
-        """Returns a list of NuGet packages that were installed by install_module() for a given product id.
-
-        :param product_id: the product id to get the installed packages of
-        :return: a list of NuGet packages in are available for the given product id
-        """
-        return self._installed_packages.get(product_id, []).copy()
-
-    def is_module_installed(self, product_id: int) -> bool:
-        """Returns whether a module with a given producti d has been installed with install_module().
-
-        :param product_id: the product id to check the install status of
-        :return: True if the product id has been registered with install_module(), False if not
-        """
-        return product_id in self._installed_product_ids
+# QUANTCONNECT.COM - Democratizing Finance, Empowering Individuals.
+# Lean CLI v1.0. Copyright 2021 QuantConnect Corporation.
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+
+from pathlib import Path
+from typing import Set, List, Dict
+
+from ablean.components.util.logger import Logger
+from ablean.constants import MODULES_DIRECTORY
+from ablean.models.modules import NuGetPackage
+
+
+class ModuleManager:
+    """The ModuleManager class is responsible for downloading and updating modules."""
+
+    def __init__(self, logger: Logger) -> None:
+        """Creates a new ModuleManager instance.
+
+        :param logger: the logger to use
+        :param api_client: the APIClient instance to use when communicating with the cloud
+        :param http_client: the HTTPClient instance to use when downloading modules
+        """
+        self._logger = logger
+        self._installed_product_ids: Set[int] = set()
+        self._installed_packages: Dict[int, List[NuGetPackage]] = {}
+
+    def get_installed_packages(self) -> List[NuGetPackage]:
+        """Returns a list of NuGet packages that were installed by install_module() calls.
+
+        :return: a list of NuGet packages in the modules directory that should be made available when running LEAN
+        """
+        packages = []
+        for package_list in self._installed_packages.values():
+            packages.extend(package_list)
+        return packages
+
+    def get_installed_packages_by_module(self, product_id: int) -> List[NuGetPackage]:
+        """Returns a list of NuGet packages that were installed by install_module() for a given product id.
+
+        :param product_id: the product id to get the installed packages of
+        :return: a list of NuGet packages in are available for the given product id
+        """
+        return self._installed_packages.get(product_id, []).copy()
+
+    def is_module_installed(self, product_id: int) -> bool:
+        """Returns whether a module with a given producti d has been installed with install_module().
+
+        :param product_id: the product id to check the install status of
+        :return: True if the product id has been registered with install_module(), False if not
+        """
+        return product_id in self._installed_product_ids
```

### Comparing `ablean-1.3.7/ablean/components/util/__init__.py` & `ablean-1.3.8/ablean/components/util/__init__.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-# QUANTCONNECT.COM - Democratizing Finance, Empowering Individuals.
-# Lean CLI v1.0. Copyright 2021 QuantConnect Corporation.
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
+# QUANTCONNECT.COM - Democratizing Finance, Empowering Individuals.
+# Lean CLI v1.0. Copyright 2021 QuantConnect Corporation.
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
```

### Comparing `ablean-1.3.7/ablean/components/util/logger.py` & `ablean-1.3.8/ablean/components/util/logger.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,170 +1,170 @@
-# QUANTCONNECT.COM - Democratizing Finance, Empowering Individuals.
-# Lean CLI v1.0. Copyright 2021 QuantConnect Corporation.
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-
-import os
-import platform
-import sys
-from typing import Any, List, Optional
-
-import click
-import maskpass
-from rich.console import Console
-from rich.progress import BarColumn, Progress, TextColumn
-
-from ablean.models.pydantic import Option
-
-
-class Logger:
-    """The Logger class handles all output printing."""
-
-    def __init__(self) -> None:
-        """Creates a new Logger instance."""
-        # In Docker the terminal size is unknown, so we disable rich's text wrapping by setting width to a high value
-        if os.environ.get("QC_LOCAL_GUI", "false") == "true":
-            width = 999999
-        else:
-            width = None
-
-        self._console = Console(markup=False, highlight=False, emoji=False, width=width)
-        self.debug_logging_enabled = False
-
-    def debug(self, message: Any) -> None:
-        """Logs a debug message if debug logging is enabled.
-
-        :param message: the message to log
-        """
-        if self.debug_logging_enabled:
-            self._console.print(message, style="grey50")
-
-    def info(self, message: Any) -> None:
-        """Logs an info message.
-
-        :param message: the message to log
-        """
-        self._console.print(message)
-
-    def warn(self, message: Any) -> None:
-        """Logs a warning message.
-
-        :param message: the message to log
-        """
-        self._console.print(message, style="yellow")
-
-    def error(self, message: Any) -> None:
-        """Logs an error message.
-
-        :param message: the message to log
-        """
-        self._console.print(message, style="red")
-
-    def progress(
-        self, prefix: str = "", suffix: str = "{task.percentage:0.0f}%"
-    ) -> Progress:
-        """Creates a Progress instance.
-
-        :param prefix: the text to show before the bar (defaults to a blank string)
-        :param suffix: the text to show after the bar (defaults to the task's percentage)
-        :return: a Progress instance which can be used to display progress bars
-        """
-        progress = Progress(
-            TextColumn(prefix), BarColumn(), TextColumn(suffix), console=self._console
-        )
-        progress.start()
-        return progress
-
-    def prompt_list(
-        self,
-        text: str,
-        options: List[Option],
-        default: Optional[str] = None,
-        multiple: bool = False,
-    ) -> Any:
-        """Asks the user to select an option from a list of possible options.
-
-        The user will not be prompted for input if there is only a single option.
-
-        :param text: the text to display before prompting
-        :param options: the available options
-        :param default: the default value if no input is given
-        :return: the chosen option's id
-        """
-
-        def validate_option(input_value: Any):
-            try:
-                index = int(input_value)
-                if 0 < index <= len(options):
-                    return options[index - 1].id
-            except ValueError:
-                option = next(
-                    (option for option in options if option.label == input_value), None
-                )
-                if option is not None:
-                    return option.id
-
-            self.info("Please enter the number or label of an option")
-
-        if len(options) == 1:
-            self.info(f"{text}: {options[0].label}")
-            return options[0].id
-
-        self.info(f"{text}:")
-        for i, option in enumerate(options):
-            self.info(f"{i + 1}) {option.label}")
-
-        while True:
-            if not multiple:
-                user_input = click.prompt(
-                    "Enter an option", type=str, default=default, show_default=True
-                )
-                user_selected_value = validate_option(user_input)
-                if user_selected_value is not None:
-                    return user_selected_value
-            else:
-                user_selected_values = []
-                user_inputs = click.prompt(
-                    "To enter multiple options, seprate them with comma.",
-                    type=str,
-                    default=default,
-                    show_default=True,
-                )
-                user_inputs = str(user_inputs).strip(",").split(",")
-                expected_outputs = len(user_inputs)
-                for user_input in user_inputs:
-                    user_selected_value = validate_option(user_input)
-                    if user_selected_value is not None:
-                        user_selected_values.append(user_selected_value)
-                if len(user_selected_values) == expected_outputs:
-                    return user_selected_values
-
-    def prompt_password(self, text: str, default: Optional[str] = None) -> str:
-        """Asks the user for a string value while masking the given input.
-
-        :param text: the text to display before prompting
-        :param default: the default value if no input is given
-        :return: the given input
-        """
-        if default is not None:
-            text = f"{text} [{'*' * len(default)}]"
-
-        # Masking does not work properly in WSL2 and when the input is not coming from a keyboard
-        if "microsoft" in platform.uname().release.lower() or not sys.stdin.isatty():
-            return click.prompt(text, default=default, show_default=False)
-
-        while True:
-            user_input = maskpass.askpass(f"{text}: ")
-
-            if len(user_input) == 0 and default is not None:
-                return default
-
-            if len(user_input) > 0:
-                return user_input
+# QUANTCONNECT.COM - Democratizing Finance, Empowering Individuals.
+# Lean CLI v1.0. Copyright 2021 QuantConnect Corporation.
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+
+import os
+import platform
+import sys
+from typing import Any, List, Optional
+
+import click
+import maskpass
+from rich.console import Console
+from rich.progress import BarColumn, Progress, TextColumn
+
+from ablean.models.pydantic import Option
+
+
+class Logger:
+    """The Logger class handles all output printing."""
+
+    def __init__(self) -> None:
+        """Creates a new Logger instance."""
+        # In Docker the terminal size is unknown, so we disable rich's text wrapping by setting width to a high value
+        if os.environ.get("QC_LOCAL_GUI", "false") == "true":
+            width = 999999
+        else:
+            width = None
+
+        self._console = Console(markup=False, highlight=False, emoji=False, width=width)
+        self.debug_logging_enabled = False
+
+    def debug(self, message: Any) -> None:
+        """Logs a debug message if debug logging is enabled.
+
+        :param message: the message to log
+        """
+        if self.debug_logging_enabled:
+            self._console.print(message, style="grey50")
+
+    def info(self, message: Any) -> None:
+        """Logs an info message.
+
+        :param message: the message to log
+        """
+        self._console.print(message)
+
+    def warn(self, message: Any) -> None:
+        """Logs a warning message.
+
+        :param message: the message to log
+        """
+        self._console.print(message, style="yellow")
+
+    def error(self, message: Any) -> None:
+        """Logs an error message.
+
+        :param message: the message to log
+        """
+        self._console.print(message, style="red")
+
+    def progress(
+        self, prefix: str = "", suffix: str = "{task.percentage:0.0f}%"
+    ) -> Progress:
+        """Creates a Progress instance.
+
+        :param prefix: the text to show before the bar (defaults to a blank string)
+        :param suffix: the text to show after the bar (defaults to the task's percentage)
+        :return: a Progress instance which can be used to display progress bars
+        """
+        progress = Progress(
+            TextColumn(prefix), BarColumn(), TextColumn(suffix), console=self._console
+        )
+        progress.start()
+        return progress
+
+    def prompt_list(
+        self,
+        text: str,
+        options: List[Option],
+        default: Optional[str] = None,
+        multiple: bool = False,
+    ) -> Any:
+        """Asks the user to select an option from a list of possible options.
+
+        The user will not be prompted for input if there is only a single option.
+
+        :param text: the text to display before prompting
+        :param options: the available options
+        :param default: the default value if no input is given
+        :return: the chosen option's id
+        """
+
+        def validate_option(input_value: Any):
+            try:
+                index = int(input_value)
+                if 0 < index <= len(options):
+                    return options[index - 1].id
+            except ValueError:
+                option = next(
+                    (option for option in options if option.label == input_value), None
+                )
+                if option is not None:
+                    return option.id
+
+            self.info("Please enter the number or label of an option")
+
+        if len(options) == 1:
+            self.info(f"{text}: {options[0].label}")
+            return options[0].id
+
+        self.info(f"{text}:")
+        for i, option in enumerate(options):
+            self.info(f"{i + 1}) {option.label}")
+
+        while True:
+            if not multiple:
+                user_input = click.prompt(
+                    "Enter an option", type=str, default=default, show_default=True
+                )
+                user_selected_value = validate_option(user_input)
+                if user_selected_value is not None:
+                    return user_selected_value
+            else:
+                user_selected_values = []
+                user_inputs = click.prompt(
+                    "To enter multiple options, seprate them with comma.",
+                    type=str,
+                    default=default,
+                    show_default=True,
+                )
+                user_inputs = str(user_inputs).strip(",").split(",")
+                expected_outputs = len(user_inputs)
+                for user_input in user_inputs:
+                    user_selected_value = validate_option(user_input)
+                    if user_selected_value is not None:
+                        user_selected_values.append(user_selected_value)
+                if len(user_selected_values) == expected_outputs:
+                    return user_selected_values
+
+    def prompt_password(self, text: str, default: Optional[str] = None) -> str:
+        """Asks the user for a string value while masking the given input.
+
+        :param text: the text to display before prompting
+        :param default: the default value if no input is given
+        :return: the given input
+        """
+        if default is not None:
+            text = f"{text} [{'*' * len(default)}]"
+
+        # Masking does not work properly in WSL2 and when the input is not coming from a keyboard
+        if "microsoft" in platform.uname().release.lower() or not sys.stdin.isatty():
+            return click.prompt(text, default=default, show_default=False)
+
+        while True:
+            user_input = maskpass.askpass(f"{text}: ")
+
+            if len(user_input) == 0 and default is not None:
+                return default
+
+            if len(user_input) > 0:
+                return user_input
```

### Comparing `ablean-1.3.7/ablean/components/util/name_extraction.py` & `ablean-1.3.8/ablean/components/util/name_extraction.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,34 +1,34 @@
-# QUANTCONNECT.COM - Democratizing Finance, Empowering Individuals.
-# Lean CLI v1.0. Copyright 2021 QuantConnect Corporation.
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-
-import re
-from pathlib import Path
-
-def _capitalize(word: str) -> str:
-    """Capitalizes the given word.
-
-    :param word: the word to capitalize
-    :return: the word with the first letter capitalized (any other uppercase characters are preserved)
-    """
-    if word == "":
-        return word
-    return word[0].upper() + word[1:]
-
-
-def convert_to_class_name(file_path: Path):
-    """Converts the project name into a valid class name by removing all non-alphanumeric characters
-
-    :param file_path: Path to the root project
-    :return: returns a valid class name
-    """
+# QUANTCONNECT.COM - Democratizing Finance, Empowering Individuals.
+# Lean CLI v1.0. Copyright 2021 QuantConnect Corporation.
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+
+import re
+from pathlib import Path
+
+def _capitalize(word: str) -> str:
+    """Capitalizes the given word.
+
+    :param word: the word to capitalize
+    :return: the word with the first letter capitalized (any other uppercase characters are preserved)
+    """
+    if word == "":
+        return word
+    return word[0].upper() + word[1:]
+
+
+def convert_to_class_name(file_path: Path):
+    """Converts the project name into a valid class name by removing all non-alphanumeric characters
+
+    :param file_path: Path to the root project
+    :return: returns a valid class name
+    """
     return re.sub(f"[^a-zA-Z0-9]", "", "".join(map(_capitalize, file_path.name.split(" "))))
```

### Comparing `ablean-1.3.7/ablean/components/util/name_generator.py` & `ablean-1.3.8/ablean/components/util/name_generator.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,49 +1,49 @@
-# QUANTCONNECT.COM - Democratizing Finance, Empowering Individuals.
-# Lean CLI v1.0. Copyright 2021 QuantConnect Corporation.
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-
-from random import choice
-
-
-class NameGenerator:
-    """The NameGenerator generates random names."""
-
-    def __init__(self) -> None:
-        """Creates a new NameGenerator instance."""
-        self._verbs = ["Determined", "Pensive", "Adaptable", "Calculating", "Logical", "Energetic", "Creative",
-                       "Smooth", "Calm", "Hyper-Active", "Measured", "Fat", "Emotional", "Crying", "Jumping",
-                       "Swimming", "Crawling", "Dancing", "Focused", "Well Dressed", "Retrospective", "Hipster",
-                       "Square", "Upgraded", "Ugly", "Casual", "Formal", "Geeky", "Virtual", "Muscular", "Alert",
-                       "Sleepy"]
-
-        self._colors = ["Red", "Red-Orange", "Orange", "Yellow", "Tan", "Yellow-Green", "Yellow-Green",
-                        "Fluorescent Orange", "Apricot", "Green", "Fluorescent Pink", "Sky Blue", "Fluorescent Yellow",
-                        "Asparagus", "Blue", "Violet", "Light Brown", "Brown", "Magenta", "Black"]
-
-        self._animals = ["Horse", "Zebra", "Whale", "Tapir", "Barracuda", "Cow", "Cat", "Wolf", "Hamster", "Monkey",
-                         "Pelican", "Snake", "Albatross", "Viper", "Guanaco", "Anguilline", "Badger", "Dogfish", "Duck",
-                         "Butterfly", "Gaur", "Rat", "Termite", "Eagle", "Dinosaur", "Pig", "Seahorse", "Hornet",
-                         "Koala", "Hippopotamus", "Cormorant", "Jackal", "Rhinoceros", "Panda", "Elephant", "Penguin",
-                         "Beaver", "Hyena", "Parrot", "Crocodile", "Baboon", "Pony", "Chinchilla", "Fox", "Lion",
-                         "Mosquito", "Cobra", "Mule", "Coyote", "Alligator", "Pigeon", "Antelope", "Goat", "Falcon",
-                         "Owlet", "Llama", "Gull", "Chicken", "Caterpillar", "Giraffe", "Rabbit", "Flamingo", "Caribou",
-                         "Goshawk", "Galago", "Bee", "Jellyfish", "Buffalo", "Salmon", "Bison", "Dolphin", "Jaguar",
-                         "Dog", "Armadillo", "Gorilla", "Alpaca", "Kangaroo", "Dragonfly", "Salamander", "Owl", "Bat",
-                         "Sheep", "Frog", "Chimpanzee", "Bull", "Scorpion", "Lemur", "Camel", "Leopard", "Fish",
-                         "Donkey", "Manatee", "Shark", "Bear", "kitten", "Fly", "Ant", "Sardine"]
-
-    def generate_name(self) -> str:
-        """Returns a random name.
-
-        :return: a random name containing multiple words
-        """
-        return f"{choice(self._verbs)} {choice(self._colors)} {choice(self._animals)}"
+# QUANTCONNECT.COM - Democratizing Finance, Empowering Individuals.
+# Lean CLI v1.0. Copyright 2021 QuantConnect Corporation.
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+
+from random import choice
+
+
+class NameGenerator:
+    """The NameGenerator generates random names."""
+
+    def __init__(self) -> None:
+        """Creates a new NameGenerator instance."""
+        self._verbs = ["Determined", "Pensive", "Adaptable", "Calculating", "Logical", "Energetic", "Creative",
+                       "Smooth", "Calm", "Hyper-Active", "Measured", "Fat", "Emotional", "Crying", "Jumping",
+                       "Swimming", "Crawling", "Dancing", "Focused", "Well Dressed", "Retrospective", "Hipster",
+                       "Square", "Upgraded", "Ugly", "Casual", "Formal", "Geeky", "Virtual", "Muscular", "Alert",
+                       "Sleepy"]
+
+        self._colors = ["Red", "Red-Orange", "Orange", "Yellow", "Tan", "Yellow-Green", "Yellow-Green",
+                        "Fluorescent Orange", "Apricot", "Green", "Fluorescent Pink", "Sky Blue", "Fluorescent Yellow",
+                        "Asparagus", "Blue", "Violet", "Light Brown", "Brown", "Magenta", "Black"]
+
+        self._animals = ["Horse", "Zebra", "Whale", "Tapir", "Barracuda", "Cow", "Cat", "Wolf", "Hamster", "Monkey",
+                         "Pelican", "Snake", "Albatross", "Viper", "Guanaco", "Anguilline", "Badger", "Dogfish", "Duck",
+                         "Butterfly", "Gaur", "Rat", "Termite", "Eagle", "Dinosaur", "Pig", "Seahorse", "Hornet",
+                         "Koala", "Hippopotamus", "Cormorant", "Jackal", "Rhinoceros", "Panda", "Elephant", "Penguin",
+                         "Beaver", "Hyena", "Parrot", "Crocodile", "Baboon", "Pony", "Chinchilla", "Fox", "Lion",
+                         "Mosquito", "Cobra", "Mule", "Coyote", "Alligator", "Pigeon", "Antelope", "Goat", "Falcon",
+                         "Owlet", "Llama", "Gull", "Chicken", "Caterpillar", "Giraffe", "Rabbit", "Flamingo", "Caribou",
+                         "Goshawk", "Galago", "Bee", "Jellyfish", "Buffalo", "Salmon", "Bison", "Dolphin", "Jaguar",
+                         "Dog", "Armadillo", "Gorilla", "Alpaca", "Kangaroo", "Dragonfly", "Salamander", "Owl", "Bat",
+                         "Sheep", "Frog", "Chimpanzee", "Bull", "Scorpion", "Lemur", "Camel", "Leopard", "Fish",
+                         "Donkey", "Manatee", "Shark", "Bear", "kitten", "Fly", "Ant", "Sardine"]
+
+    def generate_name(self) -> str:
+        """Returns a random name.
+
+        :return: a random name containing multiple words
+        """
+        return f"{choice(self._verbs)} {choice(self._colors)} {choice(self._animals)}"
```

### Comparing `ablean-1.3.7/ablean/components/util/path_manager.py` & `ablean-1.3.8/ablean/components/util/path_manager.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,71 +1,71 @@
-# QUANTCONNECT.COM - Democratizing Finance, Empowering Individuals.
-# Lean CLI v1.0. Copyright 2021 QuantConnect Corporation.
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-
-from pathlib import Path
-
-from ablean.components.util.platform_manager import PlatformManager
-
-
-class PathManager:
-    """The PathManager class provides utilities for working with paths."""
-
-    def __init__(self, platform_manager: PlatformManager) -> None:
-        """Creates a new PathManager instance.
-
-        :param platform_manager: the PlatformManager used when checking which operating system is in use
-        """
-        self._platform_manager = platform_manager
-
-    def get_relative_path(self, destination: Path, source: Path = Path.cwd()) -> Path:
-        """Returns a path relative to another one.
-
-        :param destination: the path to point to
-        :param source: the root where the relative path is relative to
-        :return: the destination path relative to the source path, or destination path if it is not relative
-        """
-        try:
-            return destination.relative_to(source)
-        except ValueError:
-            return destination
-
-    def is_path_valid(self, path: Path) -> bool:
-        """Returns whether a path is valid on the current operating system.
-
-        :param path: the path to validate
-        :return: True if the path is valid on the current operating system, False if not
-        """
-        try:
-            # This call fails if the path contains invalid characters
-            path.exists()
-        except OSError:
-            return False
-
-        # On Windows path.exists() doesn't throw for paths like CON/file.txt
-        # Trying to create them does raise errors, so we manually validate path components
-        if self._platform_manager.is_system_windows():
-            # Skip the first component, which contains the drive name
-            for component in path.as_posix().split("/")[1:]:
-                if component.startswith(" ") or component.endswith(" ") or component.endswith("."):
-                    return False
-
-                for reserved_name in ["CON", "PRN", "AUX", "NUL",
-                                      "COM1", "COM2", "COM3", "COM4", "COM5", "COM6", "COM7", "COM8", "COM9",
-                                      "LPT1", "LPT2", "LPT3", "LPT4", "LPT5", "LPT6", "LPT7", "LPT8", "LPT9"]:
-                    if component.upper() == reserved_name or component.upper().startswith(reserved_name + "."):
-                        return False
-
-                for forbidden_character in [":", "*", "?", '"', "<", ">", "|"]:
-                    if forbidden_character in component:
-                        return False
-
-        return True
+# QUANTCONNECT.COM - Democratizing Finance, Empowering Individuals.
+# Lean CLI v1.0. Copyright 2021 QuantConnect Corporation.
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+
+from pathlib import Path
+
+from ablean.components.util.platform_manager import PlatformManager
+
+
+class PathManager:
+    """The PathManager class provides utilities for working with paths."""
+
+    def __init__(self, platform_manager: PlatformManager) -> None:
+        """Creates a new PathManager instance.
+
+        :param platform_manager: the PlatformManager used when checking which operating system is in use
+        """
+        self._platform_manager = platform_manager
+
+    def get_relative_path(self, destination: Path, source: Path = Path.cwd()) -> Path:
+        """Returns a path relative to another one.
+
+        :param destination: the path to point to
+        :param source: the root where the relative path is relative to
+        :return: the destination path relative to the source path, or destination path if it is not relative
+        """
+        try:
+            return destination.relative_to(source)
+        except ValueError:
+            return destination
+
+    def is_path_valid(self, path: Path) -> bool:
+        """Returns whether a path is valid on the current operating system.
+
+        :param path: the path to validate
+        :return: True if the path is valid on the current operating system, False if not
+        """
+        try:
+            # This call fails if the path contains invalid characters
+            path.exists()
+        except OSError:
+            return False
+
+        # On Windows path.exists() doesn't throw for paths like CON/file.txt
+        # Trying to create them does raise errors, so we manually validate path components
+        if self._platform_manager.is_system_windows():
+            # Skip the first component, which contains the drive name
+            for component in path.as_posix().split("/")[1:]:
+                if component.startswith(" ") or component.endswith(" ") or component.endswith("."):
+                    return False
+
+                for reserved_name in ["CON", "PRN", "AUX", "NUL",
+                                      "COM1", "COM2", "COM3", "COM4", "COM5", "COM6", "COM7", "COM8", "COM9",
+                                      "LPT1", "LPT2", "LPT3", "LPT4", "LPT5", "LPT6", "LPT7", "LPT8", "LPT9"]:
+                    if component.upper() == reserved_name or component.upper().startswith(reserved_name + "."):
+                        return False
+
+                for forbidden_character in [":", "*", "?", '"', "<", ">", "|"]:
+                    if forbidden_character in component:
+                        return False
+
+        return True
```

### Comparing `ablean-1.3.7/ablean/components/util/platform_manager.py` & `ablean-1.3.8/ablean/components/util/platform_manager.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,110 +1,110 @@
-# QUANTCONNECT.COM - Democratizing Finance, Empowering Individuals.
-# Lean CLI v1.0. Copyright 2021 QuantConnect Corporation.
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-
-import os
-import platform
-
-
-class PlatformManager:
-    """The PlatformManager class makes it easy to detect which platform the user is using."""
-
-    def __init__(self) -> None:
-        """Creates a new PlatformManager instance."""
-        self._system = platform.system()
-        self._machine = platform.machine()
-        self._host_system = os.environ.get("QC_DOCKER_HOST_SYSTEM", None)
-        self._host_machine = os.environ.get("QC_DOCKER_HOST_MACHINE", None)
-
-    def is_system_windows(self) -> bool:
-        """Returns whether the current system is running Windows.
-
-        If this method is called inside Docker, it returns whether the Docker container is running Windows.
-
-        :return: whether the current system is running Windows
-        """
-        return self._system == "Windows"
-
-    def is_system_macos(self) -> bool:
-        """Returns whether the current system is running macOS.
-
-        If this method is called inside Docker, it returns whether the Docker container is running macOS.
-
-        :return: whether the current system is running macOS
-        """
-        return self._system == "Darwin"
-
-    def is_system_linux(self) -> bool:
-        """Returns whether the current system is running Linux.
-
-        If this method is called inside Docker, it returns whether the Docker container is running Linux.
-
-        :return: whether the current system is running Linux
-        """
-        return self._system == "Linux"
-
-    def is_system_arm(self) -> bool:
-        """Returns whether the current system is running on the ARM architecture.
-
-        If this method is called inside Docker, it returns whether the Docker container is running on ARM.
-
-        :return: whether the current system is running on ARM
-        """
-        return self._machine in ["arm64", "aarch64"]
-
-    def is_host_windows(self) -> bool:
-        """Returns whether the current host is running Windows.
-
-        If this method is called outside Docker, it behaves identical to is_system_windows().
-        If this method is called inside Docker, it returns whether the Docker host is running Windows.
-
-        :return: whether the current host is running Windows
-        """
-        if self._host_system is None:
-            return self.is_system_windows()
-        return self._host_system == "Windows"
-
-    def is_host_macos(self) -> bool:
-        """Returns whether the current host is running macOS.
-
-        If this method is called outside Docker, it behaves identical to is_system_macos().
-        If this method is called inside Docker, it returns whether the Docker host is running macOS.
-
-        :return: whether the current host is running macOS
-        """
-        if self._host_system is None:
-            return self.is_system_macos()
-        return self._host_system == "Darwin"
-
-    def is_host_linux(self) -> bool:
-        """Returns whether the current host is running Linux.
-
-        If this method is called outside Docker, it behaves identical to is_system_linux().
-        If this method is called inside Docker, it returns whether the Docker host is running Linux.
-
-        :return: whether the current host is running Linux
-        """
-        if self._host_system is None:
-            return self.is_system_linux()
-        return self._host_system == "Linux"
-
-    def is_host_arm(self) -> bool:
-        """Returns whether the current host is running on the ARM architecture.
-
-        If this method is called outside Docker, it behaves identical to is_system_arm().
-        If this method is called inside Docker, it returns whether the Docker host is running on ARM.
-
-        :return: whether the current host is running on ARM
-        """
-        if self._host_machine is None:
-            return self.is_system_arm()
-        return self._host_machine in ["arm64", "aarch64"]
+# QUANTCONNECT.COM - Democratizing Finance, Empowering Individuals.
+# Lean CLI v1.0. Copyright 2021 QuantConnect Corporation.
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+
+import os
+import platform
+
+
+class PlatformManager:
+    """The PlatformManager class makes it easy to detect which platform the user is using."""
+
+    def __init__(self) -> None:
+        """Creates a new PlatformManager instance."""
+        self._system = platform.system()
+        self._machine = platform.machine()
+        self._host_system = os.environ.get("QC_DOCKER_HOST_SYSTEM", None)
+        self._host_machine = os.environ.get("QC_DOCKER_HOST_MACHINE", None)
+
+    def is_system_windows(self) -> bool:
+        """Returns whether the current system is running Windows.
+
+        If this method is called inside Docker, it returns whether the Docker container is running Windows.
+
+        :return: whether the current system is running Windows
+        """
+        return self._system == "Windows"
+
+    def is_system_macos(self) -> bool:
+        """Returns whether the current system is running macOS.
+
+        If this method is called inside Docker, it returns whether the Docker container is running macOS.
+
+        :return: whether the current system is running macOS
+        """
+        return self._system == "Darwin"
+
+    def is_system_linux(self) -> bool:
+        """Returns whether the current system is running Linux.
+
+        If this method is called inside Docker, it returns whether the Docker container is running Linux.
+
+        :return: whether the current system is running Linux
+        """
+        return self._system == "Linux"
+
+    def is_system_arm(self) -> bool:
+        """Returns whether the current system is running on the ARM architecture.
+
+        If this method is called inside Docker, it returns whether the Docker container is running on ARM.
+
+        :return: whether the current system is running on ARM
+        """
+        return self._machine in ["arm64", "aarch64"]
+
+    def is_host_windows(self) -> bool:
+        """Returns whether the current host is running Windows.
+
+        If this method is called outside Docker, it behaves identical to is_system_windows().
+        If this method is called inside Docker, it returns whether the Docker host is running Windows.
+
+        :return: whether the current host is running Windows
+        """
+        if self._host_system is None:
+            return self.is_system_windows()
+        return self._host_system == "Windows"
+
+    def is_host_macos(self) -> bool:
+        """Returns whether the current host is running macOS.
+
+        If this method is called outside Docker, it behaves identical to is_system_macos().
+        If this method is called inside Docker, it returns whether the Docker host is running macOS.
+
+        :return: whether the current host is running macOS
+        """
+        if self._host_system is None:
+            return self.is_system_macos()
+        return self._host_system == "Darwin"
+
+    def is_host_linux(self) -> bool:
+        """Returns whether the current host is running Linux.
+
+        If this method is called outside Docker, it behaves identical to is_system_linux().
+        If this method is called inside Docker, it returns whether the Docker host is running Linux.
+
+        :return: whether the current host is running Linux
+        """
+        if self._host_system is None:
+            return self.is_system_linux()
+        return self._host_system == "Linux"
+
+    def is_host_arm(self) -> bool:
+        """Returns whether the current host is running on the ARM architecture.
+
+        If this method is called outside Docker, it behaves identical to is_system_arm().
+        If this method is called inside Docker, it returns whether the Docker host is running on ARM.
+
+        :return: whether the current host is running on ARM
+        """
+        if self._host_machine is None:
+            return self.is_system_arm()
+        return self._host_machine in ["arm64", "aarch64"]
```

### Comparing `ablean-1.3.7/ablean/components/util/project_manager.py` & `ablean-1.3.8/ablean/components/util/project_manager.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,540 +1,540 @@
-# QUANTCONNECT.COM - Democratizing Finance, Empowering Individuals.
-# Lean CLI v1.0. Copyright 2021 QuantConnect Corporation.
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-
-import json
-import os
-import shutil
-import site
-import sys
-from datetime import datetime, timezone
-from pathlib import Path
-from typing import List
-
-import pkg_resources
-
-from ablean.components.config.lean_config_manager import LeanConfigManager
-from ablean.components.config.project_config_manager import ProjectConfigManager
-from ablean.components.util.platform_manager import PlatformManager
-from ablean.components.util.xml_manager import XMLManager
-from ablean.constants import PROJECT_CONFIG_FILE_NAME
-
-
-class ProjectManager:
-    """The ProjectManager class provides utilities for handling a single project."""
-
-    def __init__(
-        self,
-        project_config_manager: ProjectConfigManager,
-        lean_config_manager: LeanConfigManager,
-        xml_manager: XMLManager,
-        platform_manager: PlatformManager,
-    ) -> None:
-        """Creates a new ProjectManager instance.
-
-        :param project_config_manager: the ProjectConfigManager to use when creating new projects
-        :param lean_config_manager: the LeanConfigManager to get the CLI root directory from
-        :param xml_manager: the XMLManager to use when working with XML
-        :param platform_manager: the PlatformManager used when checking which operating system is in use
-        """
-        self._project_config_manager = project_config_manager
-        self._lean_config_manager = lean_config_manager
-        self._xml_manager = xml_manager
-        self._platform_manager = platform_manager
-
-    def find_algorithm_file(self, input: Path) -> Path:
-        """Returns the path to the file containing the algorithm.
-
-        Raises an error if the algorithm file cannot be found.
-
-        :param input: the path to the algorithm or the path to the project
-        :return: the path to the file containing the algorithm
-        """
-        if input.is_file():
-            return input
-
-        for file_name in ["main.py", "Main.cs"]:
-            target_file = input / file_name
-            if target_file.exists():
-                return target_file
-
-        raise ValueError(
-            "The specified project does not contain a main.py or Main.cs file"
-        )
-
-    def get_project_by_id(self, local_id: int) -> Path:
-        """Finds a project by its local id.
-
-        Raises an error if a project with the given local id cannot be found.
-
-        :param local_id: the local id of the project
-        :return: the path to the directory containing the project with the given local id
-        """
-        directories = [self._lean_config_manager.get_cli_root_directory()]
-        while len(directories) > 0:
-            directory = directories.pop(0)
-
-            config_file = directory / PROJECT_CONFIG_FILE_NAME
-            if config_file.is_file():
-                if self._project_config_manager.get_local_id(directory) == local_id:
-                    return directory
-            else:
-                directories.extend(d for d in directory.iterdir() if d.is_dir())
-
-        raise RuntimeError(f"Project with local id '{local_id}' does not exist")
-
-    def get_source_files(self, directory: Path) -> List[Path]:
-        """Returns the paths of all the source files in a directory.
-
-        :param directory: the path to the directory to get the source files of
-        :return: the list of source files in the given project directory
-        """
-        source_files = []
-
-        for obj in directory.iterdir():
-            if obj.is_dir():
-                if obj.name in [
-                    "bin",
-                    "obj",
-                    ".ipynb_checkpoints",
-                    "backtests",
-                    "live",
-                    "optimizations",
-                ]:
-                    continue
-
-                source_files.extend(self.get_source_files(obj))
-
-            if obj.suffix not in [".py", ".cs", ".ipynb"]:
-                continue
-
-            source_files.append(obj)
-
-        return source_files
-
-    def update_last_modified_time(
-        self, local_file_path: Path, cloud_timestamp: datetime
-    ) -> None:
-        """Updates the last modified time of a local path to that of the cloud counterpart.
-
-        :param local_file_path: the path to the local file to update the last modified time of
-        :param cloud_timestamp: the last modified time of the counterpart of the local file in the cloud
-        """
-        # Timestamps are stored in UTC in the cloud, but utime() requires them in the local timezone
-        time = cloud_timestamp.replace(tzinfo=timezone.utc).astimezone(tz=None)
-        time = round(time.timestamp() * 1e9)
-        os.utime(local_file_path, ns=(time, time))
-
-    def copy_code(self, project_dir: Path, output_dir: Path) -> None:
-        """Copies the source code of a project to another directory.
-
-        :param project_dir: the directory of the project
-        :param output_dir: the directory to copy the code to
-        """
-        output_dir.mkdir(parents=True, exist_ok=True)
-
-        for source_file in self.get_source_files(project_dir):
-            target_file = output_dir / source_file.relative_to(project_dir)
-            target_file.parent.mkdir(parents=True, exist_ok=True)
-            shutil.copyfile(source_file, target_file)
-
-    def create_new_project(self, project_dir: Path) -> None:
-        """Creates a new project directory and fills it with some useful files.
-
-        :param project_dir: the directory of the new project
-        :param language: the language of the new project
-        """
-        project_dir.mkdir(parents=True, exist_ok=True)
-
-        project_config = self._project_config_manager.get_project_config(project_dir)
-        project_config.set("algorithm-language", "Python")
-        project_config.set("parameters", {})
-        project_config.set("description", "")
-
-        self._generate_python_library_projects_config()
-        self._generate_vscode_python_config(project_dir)
-        self._generate_pycharm_config(project_dir)
-
-    def _generate_python_library_projects_config(self) -> None:
-        """Generates the required configuration to enable autocomplete on Python library projects."""
-        try:
-            cli_root_dir = self._lean_config_manager.get_cli_root_directory()
-        except:
-            return
-
-        library_dir = cli_root_dir / "Library"
-        if not library_dir.is_dir():
-            return
-
-        if site.ENABLE_USER_SITE:
-            site_packages_dir = site.getusersitepackages()
-        else:
-            site_packages_dir = site.getsitepackages()[0]
-
-        self._generate_file(Path(site_packages_dir) / "lean-cli.pth", str(library_dir))
-
-    def _generate_vscode_python_config(self, project_dir: Path) -> None:
-        """Generates Python interpreter configuration and Python debugging configuration for VS Code.
-
-        :param project_dir: the directory of the new project
-        """
-        self._generate_file(
-            project_dir / ".vscode" / "settings.json",
-            json.dumps(
-                {
-                    "python.pythonPath": sys.executable,
-                    "python.languageServer": "Pylance",
-                },
-                indent=4,
-            ),
-        )
-
-        launch_config = {
-            "version": "0.2.0",
-            "configurations": [
-                {
-                    "name": "Debug with Lean CLI",
-                    "type": "python",
-                    "request": "attach",
-                    "connect": {"host": "localhost", "port": 5678},
-                }
-            ],
-        }
-
-        self._generate_file(
-            project_dir / ".vscode" / "launch.json", json.dumps(launch_config, indent=4)
-        )
-
-    def _generate_pycharm_config(self, project_dir: Path) -> None:
-        """Generates Python interpreter configuration and Python debugging configuration for PyCharm.
-
-        :param project_dir: the directory of the new project
-        """
-        # Generate Python JDK entry for PyCharm Professional and PyCharm Community
-        for editor in ["PyCharm", "PyCharmCE"]:
-            for directory in self._get_jetbrains_config_dirs(editor):
-                self._generate_pycharm_jdk_entry(directory)
-
-        self._generate_file(
-            project_dir / ".idea" / f"{project_dir.name}.iml",
-            """
-<?xml version="1.0" encoding="UTF-8"?>
-<module type="PYTHON_MODULE" version="4">
-  <component name="NewModuleRootManager">
-    <content url="file://$MODULE_DIR$" />
-    <orderEntry type="jdk" jdkName="Lean CLI" jdkType="Python SDK" />
-    <orderEntry type="sourceFolder" forTests="false" />
-  </component>
-</module>
-        """,
-        )
-
-        self._generate_file(
-            project_dir / ".idea" / "misc.xml",
-            """
-<?xml version="1.0" encoding="UTF-8"?>
-<project version="4">
-  <component name="ProjectRootManager" version="2" project-jdk-name="Lean CLI" project-jdk-type="Python SDK" />
-</project>
-        """,
-        )
-
-        self._generate_file(
-            project_dir / ".idea" / "modules.xml",
-            f"""
-<?xml version="1.0" encoding="UTF-8"?>
-<project version="4">
-  <component name="ProjectModuleManager">
-    <modules>
-      <module fileurl="file://$PROJECT_DIR$/.idea/{project_dir.name}.iml" filepath="$PROJECT_DIR$/.idea/{project_dir.name}.iml" />
-    </modules>
-  </component>
-</project>
-        """,
-        )
-
-        self._generate_file(
-            project_dir / ".idea" / "workspace.xml",
-            f"""
-<?xml version="1.0" encoding="UTF-8"?>
-<project version="4">
-  <component name="RunManager" selected="Python Debug Server.Debug with Lean CLI">
-    <configuration name="Debug with Lean CLI" type="PyRemoteDebugConfigurationType" factoryName="Python Remote Debug">
-      <module name="LEAN" />
-      <option name="PORT" value="6000" />
-      <option name="HOST" value="localhost" />
-      <option name="REDIRECT_OUTPUT" value="true" />
-      <option name="SUSPEND_AFTER_CONNECT" value="true" />
-      <method v="2" />
-    </configuration>
-    <list>
-      <item itemvalue="Python Debug Server.Debug with Lean CLI" />
-    </list>
-  </component>
-</project>
-        """,
-        )
-
-    def _generate_pycharm_jdk_entry(self, pycharm_config_dir: Path) -> None:
-        """Generates a "Lean CLI" Python JDK entry to PyCharm's internal JDK table.
-
-        When we generate PyCharm's .idea directory we want to tell PyCharm where the Python interpreter is located.
-        PyCharm stores this bit of configuration globally, so we find the global location and update it to our needs.
-
-        If PyCharm is not installed yet, we create the configuration anyways.
-        Once the user installs PyCharm, it will then automatically pick up the configuration we created in the past.
-
-        :param pycharm_config_dir: the path to the global configuration directory of a PyCharm edition
-        """
-        # Parse the file containing PyCharm's internal table of Python interpreters
-        jdk_table_file = pycharm_config_dir / "options" / "jdk.table.xml"
-        if jdk_table_file.exists():
-            root = self._xml_manager.parse(jdk_table_file.read_text(encoding="utf-8"))
-        else:
-            root = self._xml_manager.parse(
-                """
-<application>
-  <component name="ProjectJdkTable">
-  </component>
-</application>
-            """
-            )
-
-        # Don't do anything if the Lean CLI interpreter entry already exists
-        if root.find(".//jdk/name[@value='Lean CLI']") is not None:
-            return
-
-        # Add the new JDK entry to the XML tree
-        classpath_entries = [
-            Path(p).as_posix() for p in sys.path if p != "" and not p.endswith(".zip")
-        ]
-        classpath_entries = [
-            f'<root url="{p}" type="simple" />' for p in classpath_entries
-        ]
-        classpath_entries = "\n".join(classpath_entries)
-
-        component_element = root.find(".//component[@name='ProjectJdkTable']")
-        component_element.append(
-            self._xml_manager.parse(
-                f"""
-<jdk version="2">
-  <name value="Lean CLI" />
-  <type value="Python SDK" />
-  <version value="Python {sys.version_info.major}.{sys.version_info.minor}.{sys.version_info.micro}" />
-  <homePath value="{Path(sys.executable).as_posix()}" />
-  <roots>
-    <classPath>
-      <root type="composite">
-        {classpath_entries}
-        <root url="file://$APPLICATION_HOME_DIR$/plugins/python/helpers/python-skeletons" type="simple" />
-        <root url="file://$APPLICATION_HOME_DIR$/plugins/python/helpers/typeshed/stdlib/3" type="simple" />
-        <root url="file://$APPLICATION_HOME_DIR$/plugins/python/helpers/typeshed/stdlib/2and3" type="simple" />
-        <root url="file://$APPLICATION_HOME_DIR$/plugins/python/helpers/typeshed/third_party/3" type="simple" />
-        <root url="file://$APPLICATION_HOME_DIR$/plugins/python/helpers/typeshed/third_party/2and3" type="simple" />
-      </root>
-    </classPath>
-    <sourcePath>
-      <root type="composite" />
-    </sourcePath>
-  </roots>
-</jdk>
-        """
-            )
-        )
-
-        # Save the modified XML tree
-        self._generate_file(jdk_table_file, self._xml_manager.to_string(root))
-
-    def _generate_vscode_csharp_config(self, project_dir: Path) -> None:
-        """Generates C# debugging configuration for VS Code.
-
-        :param project_dir: the directory of the new project
-        """
-        self._generate_file(
-            project_dir / ".vscode" / "launch.json",
-            """
-{
-    "version": "0.2.0",
-    "configurations": [
-        {
-            "name": "Debug with Lean CLI",
-            "request": "attach",
-            "type": "coreclr",
-            "processId": "1",
-            "pipeTransport": {
-                "pipeCwd": "${workspaceRoot}",
-                "pipeProgram": "docker",
-                "pipeArgs": ["exec", "-i", "lean_cli_vsdbg"],
-                "debuggerPath": "/root/vsdbg/vsdbg",
-                "quoteArgs": false
-            },
-            "logging": {
-                "moduleLoad": false
-            }
-        }
-    ]
-}
-        """,
-        )
-
-    def _generate_csproj(self, project_dir: Path) -> None:
-        """Generates a .csproj file for the given project and returns the path to it.
-
-        :param project_dir: the path of the new project
-        """
-        self._generate_file(
-            project_dir / f"{project_dir.name}.csproj",
-            """
-<Project Sdk="Microsoft.NET.Sdk">
-    <PropertyGroup>
-        <Configuration Condition=" '$(Configuration)' == '' ">Debug</Configuration>
-        <Platform Condition=" '$(Platform)' == '' ">AnyCPU</Platform>
-        <TargetFramework>net6.0</TargetFramework>
-        <OutputPath>bin/$(Configuration)</OutputPath>
-        <AppendTargetFrameworkToOutputPath>false</AppendTargetFrameworkToOutputPath>
-        <DefaultItemExcludes>$(DefaultItemExcludes);backtests/*/code/**;live/*/code/**;optimizations/*/code/**</DefaultItemExcludes>
-        <NoWarn>CS0618</NoWarn>
-    </PropertyGroup>
-    <ItemGroup>
-        <PackageReference Include="QuantConnect.Lean" Version="2.5.*"/>
-        <PackageReference Include="QuantConnect.DataSource.Libraries" Version="2.5.*"/>
-    </ItemGroup>
-</Project>
-        """,
-        )
-
-    def generate_rider_config(self) -> None:
-        """Generates C# debugging configuration for Rider."""
-        ssh_dir = Path("~/.lean/ssh").expanduser()
-
-        # Add SSH keys to .lean/ssh if necessary
-        if not ssh_dir.exists():
-            ssh_dir.mkdir(parents=True)
-            for name in ["key", "key.pub", "README.md"]:
-                with (ssh_dir / name).open("wb+") as file:
-                    file.write(pkg_resources.resource_string("lean", f"ssh/{name}"))
-
-        # Find Rider's global configuration directory
-        for directory in self._get_jetbrains_config_dirs("Rider"):
-            self._generate_rider_debugger_entry(directory, ssh_dir)
-
-    def _generate_rider_debugger_entry(
-        self, rider_config_dir: Path, ssh_dir: Path
-    ) -> None:
-        """Generates a "root@localhost:2222" remote debugger entry to Rider's internal debugger configuration.
-
-        If Rider is not installed yet, we create the configuration anyways.
-        Once the user installs Rider, it will then automatically pick up the configuration we created in the past.
-
-        :param rider_config_dir: the path to the global configuration directory of a Rider edition
-        :param ssh_dir: the path to the directory containing the SSH keys
-        """
-        # Parse the file containing Rider's internal list of remote hosts
-        debugger_file = rider_config_dir / "options" / "debugger.xml"
-        if debugger_file.exists():
-            root = self._xml_manager.parse(debugger_file.read_text(encoding="utf-8"))
-        else:
-            root = self._xml_manager.parse(
-                """
-<application>
-    <component name="XDebuggerSettings">
-    </component>
-</application>
-            """
-            )
-
-        component_element = root.find(".//component[@name='XDebuggerSettings']")
-
-        if root.find(".//debuggers") is None:
-            component_element.append(self._xml_manager.parse("<debuggers></debuggers>"))
-        debuggers = root.find(".//debuggers")
-
-        if debuggers.find(".//debugger[@id='dotnet_debugger']") is None:
-            debuggers.append(
-                self._xml_manager.parse('<debugger id="dotnet_debugger"></debugger>')
-            )
-        dotnet_debugger = debuggers.find(".//debugger[@id='dotnet_debugger']")
-
-        if dotnet_debugger.find(".//configuration") is None:
-            dotnet_debugger.append(
-                self._xml_manager.parse("<configuration></configuration>")
-            )
-        configuration = dotnet_debugger.find(".//configuration")
-
-        if configuration.find(".//option[@name='sshCredentials']") is None:
-            configuration.append(
-                self._xml_manager.parse('<option name="sshCredentials"></option>')
-            )
-        ssh_credentials = configuration.find(".//option[@name='sshCredentials']")
-
-        required_value = f"&lt;credentials HOST=&quot;localhost&quot; PORT=&quot;2222&quot; USERNAME=&quot;root&quot; PRIVATE_KEY_FILE=&quot;{ssh_dir.as_posix()}/key&quot; USE_KEY_PAIR=&quot;true&quot; USE_AUTH_AGENT=&quot;false&quot; /&gt;"
-
-        # Don't do anything if the required entry already exists
-        for option in ssh_credentials.findall(f".//option"):
-            if option.get("value") == required_value.replace("&lt;", "<").replace(
-                "&gt;", ">"
-            ).replace("&quot;", '"'):
-                return
-
-        # Add the new entry to the XML tree
-        ssh_credentials.append(
-            self._xml_manager.parse(f'<option value="{required_value}"/>')
-        )
-
-        # Save the modified XML tree
-        self._generate_file(debugger_file, self._xml_manager.to_string(root))
-
-    def _generate_file(self, file: Path, content: str) -> None:
-        """Writes to a file, which is created if it doesn't exist yet, and normalized the content before doing so.
-
-        :param file: the file to write to
-        :param content: the content to write to the file
-        """
-        file.parent.mkdir(parents=True, exist_ok=True)
-        with file.open("w+", encoding="utf-8") as file:
-            file.write(content.strip() + "\n")
-
-    def _get_jetbrains_config_dirs(self, editor_name: str) -> List[Path]:
-        """Returns the paths to the global configuration directories for all installed editions of a JetBrains IDE.
-
-        :param editor_name: the name of the JetBrains IDE
-        :return: the paths to the directories holding the global configuration for the specified IDE
-        """
-        # Find JetBrains' root directory containing the global configuration directories for all installed IDEs
-        # See https://www.jetbrains.com/help/pycharm/project-and-ide-settings.html#ide_settings
-        if self._platform_manager.is_host_windows():
-            root_dir = Path("~/AppData/Roaming/JetBrains").expanduser()
-        elif self._platform_manager.is_host_macos():
-            root_dir = Path("~/Library/Application Support/JetBrains").expanduser()
-        else:
-            root_dir = Path("~/.config/JetBrains").expanduser()
-
-        if not root_dir.exists():
-            root_dir.mkdir(parents=True)
-
-        # Find the global config directories for the given IDE
-        directories = []
-
-        for path in root_dir.iterdir():
-            if not path.is_dir() or not path.name.startswith(editor_name):
-                continue
-
-            suffix = path.name.replace(editor_name, "")
-            if len(suffix) > 0 and not suffix[0].isdigit():
-                continue
-
-            directories.append(path)
-
-        if len(directories) == 0:
-            directories.append(root_dir / editor_name)
-
-        return directories
+# QUANTCONNECT.COM - Democratizing Finance, Empowering Individuals.
+# Lean CLI v1.0. Copyright 2021 QuantConnect Corporation.
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+
+import json
+import os
+import shutil
+import site
+import sys
+from datetime import datetime, timezone
+from pathlib import Path
+from typing import List
+
+import pkg_resources
+
+from ablean.components.config.lean_config_manager import LeanConfigManager
+from ablean.components.config.project_config_manager import ProjectConfigManager
+from ablean.components.util.platform_manager import PlatformManager
+from ablean.components.util.xml_manager import XMLManager
+from ablean.constants import PROJECT_CONFIG_FILE_NAME
+
+
+class ProjectManager:
+    """The ProjectManager class provides utilities for handling a single project."""
+
+    def __init__(
+        self,
+        project_config_manager: ProjectConfigManager,
+        lean_config_manager: LeanConfigManager,
+        xml_manager: XMLManager,
+        platform_manager: PlatformManager,
+    ) -> None:
+        """Creates a new ProjectManager instance.
+
+        :param project_config_manager: the ProjectConfigManager to use when creating new projects
+        :param lean_config_manager: the LeanConfigManager to get the CLI root directory from
+        :param xml_manager: the XMLManager to use when working with XML
+        :param platform_manager: the PlatformManager used when checking which operating system is in use
+        """
+        self._project_config_manager = project_config_manager
+        self._lean_config_manager = lean_config_manager
+        self._xml_manager = xml_manager
+        self._platform_manager = platform_manager
+
+    def find_algorithm_file(self, input: Path) -> Path:
+        """Returns the path to the file containing the algorithm.
+
+        Raises an error if the algorithm file cannot be found.
+
+        :param input: the path to the algorithm or the path to the project
+        :return: the path to the file containing the algorithm
+        """
+        if input.is_file():
+            return input
+
+        for file_name in ["main.py", "Main.cs"]:
+            target_file = input / file_name
+            if target_file.exists():
+                return target_file
+
+        raise ValueError(
+            "The specified project does not contain a main.py or Main.cs file"
+        )
+
+    def get_project_by_id(self, local_id: int) -> Path:
+        """Finds a project by its local id.
+
+        Raises an error if a project with the given local id cannot be found.
+
+        :param local_id: the local id of the project
+        :return: the path to the directory containing the project with the given local id
+        """
+        directories = [self._lean_config_manager.get_cli_root_directory()]
+        while len(directories) > 0:
+            directory = directories.pop(0)
+
+            config_file = directory / PROJECT_CONFIG_FILE_NAME
+            if config_file.is_file():
+                if self._project_config_manager.get_local_id(directory) == local_id:
+                    return directory
+            else:
+                directories.extend(d for d in directory.iterdir() if d.is_dir())
+
+        raise RuntimeError(f"Project with local id '{local_id}' does not exist")
+
+    def get_source_files(self, directory: Path) -> List[Path]:
+        """Returns the paths of all the source files in a directory.
+
+        :param directory: the path to the directory to get the source files of
+        :return: the list of source files in the given project directory
+        """
+        source_files = []
+
+        for obj in directory.iterdir():
+            if obj.is_dir():
+                if obj.name in [
+                    "bin",
+                    "obj",
+                    ".ipynb_checkpoints",
+                    "backtests",
+                    "live",
+                    "optimizations",
+                ]:
+                    continue
+
+                source_files.extend(self.get_source_files(obj))
+
+            if obj.suffix not in [".py", ".cs", ".ipynb"]:
+                continue
+
+            source_files.append(obj)
+
+        return source_files
+
+    def update_last_modified_time(
+        self, local_file_path: Path, cloud_timestamp: datetime
+    ) -> None:
+        """Updates the last modified time of a local path to that of the cloud counterpart.
+
+        :param local_file_path: the path to the local file to update the last modified time of
+        :param cloud_timestamp: the last modified time of the counterpart of the local file in the cloud
+        """
+        # Timestamps are stored in UTC in the cloud, but utime() requires them in the local timezone
+        time = cloud_timestamp.replace(tzinfo=timezone.utc).astimezone(tz=None)
+        time = round(time.timestamp() * 1e9)
+        os.utime(local_file_path, ns=(time, time))
+
+    def copy_code(self, project_dir: Path, output_dir: Path) -> None:
+        """Copies the source code of a project to another directory.
+
+        :param project_dir: the directory of the project
+        :param output_dir: the directory to copy the code to
+        """
+        output_dir.mkdir(parents=True, exist_ok=True)
+
+        for source_file in self.get_source_files(project_dir):
+            target_file = output_dir / source_file.relative_to(project_dir)
+            target_file.parent.mkdir(parents=True, exist_ok=True)
+            shutil.copyfile(source_file, target_file)
+
+    def create_new_project(self, project_dir: Path) -> None:
+        """Creates a new project directory and fills it with some useful files.
+
+        :param project_dir: the directory of the new project
+        :param language: the language of the new project
+        """
+        project_dir.mkdir(parents=True, exist_ok=True)
+
+        project_config = self._project_config_manager.get_project_config(project_dir)
+        project_config.set("algorithm-language", "Python")
+        project_config.set("parameters", {})
+        project_config.set("description", "")
+
+        self._generate_python_library_projects_config()
+        self._generate_vscode_python_config(project_dir)
+        self._generate_pycharm_config(project_dir)
+
+    def _generate_python_library_projects_config(self) -> None:
+        """Generates the required configuration to enable autocomplete on Python library projects."""
+        try:
+            cli_root_dir = self._lean_config_manager.get_cli_root_directory()
+        except:
+            return
+
+        library_dir = cli_root_dir / "Library"
+        if not library_dir.is_dir():
+            return
+
+        if site.ENABLE_USER_SITE:
+            site_packages_dir = site.getusersitepackages()
+        else:
+            site_packages_dir = site.getsitepackages()[0]
+
+        self._generate_file(Path(site_packages_dir) / "lean-cli.pth", str(library_dir))
+
+    def _generate_vscode_python_config(self, project_dir: Path) -> None:
+        """Generates Python interpreter configuration and Python debugging configuration for VS Code.
+
+        :param project_dir: the directory of the new project
+        """
+        self._generate_file(
+            project_dir / ".vscode" / "settings.json",
+            json.dumps(
+                {
+                    "python.pythonPath": sys.executable,
+                    "python.languageServer": "Pylance",
+                },
+                indent=4,
+            ),
+        )
+
+        launch_config = {
+            "version": "0.2.0",
+            "configurations": [
+                {
+                    "name": "Debug with Lean CLI",
+                    "type": "python",
+                    "request": "attach",
+                    "connect": {"host": "localhost", "port": 5678},
+                }
+            ],
+        }
+
+        self._generate_file(
+            project_dir / ".vscode" / "launch.json", json.dumps(launch_config, indent=4)
+        )
+
+    def _generate_pycharm_config(self, project_dir: Path) -> None:
+        """Generates Python interpreter configuration and Python debugging configuration for PyCharm.
+
+        :param project_dir: the directory of the new project
+        """
+        # Generate Python JDK entry for PyCharm Professional and PyCharm Community
+        for editor in ["PyCharm", "PyCharmCE"]:
+            for directory in self._get_jetbrains_config_dirs(editor):
+                self._generate_pycharm_jdk_entry(directory)
+
+        self._generate_file(
+            project_dir / ".idea" / f"{project_dir.name}.iml",
+            """
+<?xml version="1.0" encoding="UTF-8"?>
+<module type="PYTHON_MODULE" version="4">
+  <component name="NewModuleRootManager">
+    <content url="file://$MODULE_DIR$" />
+    <orderEntry type="jdk" jdkName="Lean CLI" jdkType="Python SDK" />
+    <orderEntry type="sourceFolder" forTests="false" />
+  </component>
+</module>
+        """,
+        )
+
+        self._generate_file(
+            project_dir / ".idea" / "misc.xml",
+            """
+<?xml version="1.0" encoding="UTF-8"?>
+<project version="4">
+  <component name="ProjectRootManager" version="2" project-jdk-name="Lean CLI" project-jdk-type="Python SDK" />
+</project>
+        """,
+        )
+
+        self._generate_file(
+            project_dir / ".idea" / "modules.xml",
+            f"""
+<?xml version="1.0" encoding="UTF-8"?>
+<project version="4">
+  <component name="ProjectModuleManager">
+    <modules>
+      <module fileurl="file://$PROJECT_DIR$/.idea/{project_dir.name}.iml" filepath="$PROJECT_DIR$/.idea/{project_dir.name}.iml" />
+    </modules>
+  </component>
+</project>
+        """,
+        )
+
+        self._generate_file(
+            project_dir / ".idea" / "workspace.xml",
+            f"""
+<?xml version="1.0" encoding="UTF-8"?>
+<project version="4">
+  <component name="RunManager" selected="Python Debug Server.Debug with Lean CLI">
+    <configuration name="Debug with Lean CLI" type="PyRemoteDebugConfigurationType" factoryName="Python Remote Debug">
+      <module name="LEAN" />
+      <option name="PORT" value="6000" />
+      <option name="HOST" value="localhost" />
+      <option name="REDIRECT_OUTPUT" value="true" />
+      <option name="SUSPEND_AFTER_CONNECT" value="true" />
+      <method v="2" />
+    </configuration>
+    <list>
+      <item itemvalue="Python Debug Server.Debug with Lean CLI" />
+    </list>
+  </component>
+</project>
+        """,
+        )
+
+    def _generate_pycharm_jdk_entry(self, pycharm_config_dir: Path) -> None:
+        """Generates a "Lean CLI" Python JDK entry to PyCharm's internal JDK table.
+
+        When we generate PyCharm's .idea directory we want to tell PyCharm where the Python interpreter is located.
+        PyCharm stores this bit of configuration globally, so we find the global location and update it to our needs.
+
+        If PyCharm is not installed yet, we create the configuration anyways.
+        Once the user installs PyCharm, it will then automatically pick up the configuration we created in the past.
+
+        :param pycharm_config_dir: the path to the global configuration directory of a PyCharm edition
+        """
+        # Parse the file containing PyCharm's internal table of Python interpreters
+        jdk_table_file = pycharm_config_dir / "options" / "jdk.table.xml"
+        if jdk_table_file.exists():
+            root = self._xml_manager.parse(jdk_table_file.read_text(encoding="utf-8"))
+        else:
+            root = self._xml_manager.parse(
+                """
+<application>
+  <component name="ProjectJdkTable">
+  </component>
+</application>
+            """
+            )
+
+        # Don't do anything if the Lean CLI interpreter entry already exists
+        if root.find(".//jdk/name[@value='Lean CLI']") is not None:
+            return
+
+        # Add the new JDK entry to the XML tree
+        classpath_entries = [
+            Path(p).as_posix() for p in sys.path if p != "" and not p.endswith(".zip")
+        ]
+        classpath_entries = [
+            f'<root url="{p}" type="simple" />' for p in classpath_entries
+        ]
+        classpath_entries = "\n".join(classpath_entries)
+
+        component_element = root.find(".//component[@name='ProjectJdkTable']")
+        component_element.append(
+            self._xml_manager.parse(
+                f"""
+<jdk version="2">
+  <name value="Lean CLI" />
+  <type value="Python SDK" />
+  <version value="Python {sys.version_info.major}.{sys.version_info.minor}.{sys.version_info.micro}" />
+  <homePath value="{Path(sys.executable).as_posix()}" />
+  <roots>
+    <classPath>
+      <root type="composite">
+        {classpath_entries}
+        <root url="file://$APPLICATION_HOME_DIR$/plugins/python/helpers/python-skeletons" type="simple" />
+        <root url="file://$APPLICATION_HOME_DIR$/plugins/python/helpers/typeshed/stdlib/3" type="simple" />
+        <root url="file://$APPLICATION_HOME_DIR$/plugins/python/helpers/typeshed/stdlib/2and3" type="simple" />
+        <root url="file://$APPLICATION_HOME_DIR$/plugins/python/helpers/typeshed/third_party/3" type="simple" />
+        <root url="file://$APPLICATION_HOME_DIR$/plugins/python/helpers/typeshed/third_party/2and3" type="simple" />
+      </root>
+    </classPath>
+    <sourcePath>
+      <root type="composite" />
+    </sourcePath>
+  </roots>
+</jdk>
+        """
+            )
+        )
+
+        # Save the modified XML tree
+        self._generate_file(jdk_table_file, self._xml_manager.to_string(root))
+
+    def _generate_vscode_csharp_config(self, project_dir: Path) -> None:
+        """Generates C# debugging configuration for VS Code.
+
+        :param project_dir: the directory of the new project
+        """
+        self._generate_file(
+            project_dir / ".vscode" / "launch.json",
+            """
+{
+    "version": "0.2.0",
+    "configurations": [
+        {
+            "name": "Debug with Lean CLI",
+            "request": "attach",
+            "type": "coreclr",
+            "processId": "1",
+            "pipeTransport": {
+                "pipeCwd": "${workspaceRoot}",
+                "pipeProgram": "docker",
+                "pipeArgs": ["exec", "-i", "lean_cli_vsdbg"],
+                "debuggerPath": "/root/vsdbg/vsdbg",
+                "quoteArgs": false
+            },
+            "logging": {
+                "moduleLoad": false
+            }
+        }
+    ]
+}
+        """,
+        )
+
+    def _generate_csproj(self, project_dir: Path) -> None:
+        """Generates a .csproj file for the given project and returns the path to it.
+
+        :param project_dir: the path of the new project
+        """
+        self._generate_file(
+            project_dir / f"{project_dir.name}.csproj",
+            """
+<Project Sdk="Microsoft.NET.Sdk">
+    <PropertyGroup>
+        <Configuration Condition=" '$(Configuration)' == '' ">Debug</Configuration>
+        <Platform Condition=" '$(Platform)' == '' ">AnyCPU</Platform>
+        <TargetFramework>net6.0</TargetFramework>
+        <OutputPath>bin/$(Configuration)</OutputPath>
+        <AppendTargetFrameworkToOutputPath>false</AppendTargetFrameworkToOutputPath>
+        <DefaultItemExcludes>$(DefaultItemExcludes);backtests/*/code/**;live/*/code/**;optimizations/*/code/**</DefaultItemExcludes>
+        <NoWarn>CS0618</NoWarn>
+    </PropertyGroup>
+    <ItemGroup>
+        <PackageReference Include="QuantConnect.Lean" Version="2.5.*"/>
+        <PackageReference Include="QuantConnect.DataSource.Libraries" Version="2.5.*"/>
+    </ItemGroup>
+</Project>
+        """,
+        )
+
+    def generate_rider_config(self) -> None:
+        """Generates C# debugging configuration for Rider."""
+        ssh_dir = Path("~/.lean/ssh").expanduser()
+
+        # Add SSH keys to .lean/ssh if necessary
+        if not ssh_dir.exists():
+            ssh_dir.mkdir(parents=True)
+            for name in ["key", "key.pub", "README.md"]:
+                with (ssh_dir / name).open("wb+") as file:
+                    file.write(pkg_resources.resource_string("lean", f"ssh/{name}"))
+
+        # Find Rider's global configuration directory
+        for directory in self._get_jetbrains_config_dirs("Rider"):
+            self._generate_rider_debugger_entry(directory, ssh_dir)
+
+    def _generate_rider_debugger_entry(
+        self, rider_config_dir: Path, ssh_dir: Path
+    ) -> None:
+        """Generates a "root@localhost:2222" remote debugger entry to Rider's internal debugger configuration.
+
+        If Rider is not installed yet, we create the configuration anyways.
+        Once the user installs Rider, it will then automatically pick up the configuration we created in the past.
+
+        :param rider_config_dir: the path to the global configuration directory of a Rider edition
+        :param ssh_dir: the path to the directory containing the SSH keys
+        """
+        # Parse the file containing Rider's internal list of remote hosts
+        debugger_file = rider_config_dir / "options" / "debugger.xml"
+        if debugger_file.exists():
+            root = self._xml_manager.parse(debugger_file.read_text(encoding="utf-8"))
+        else:
+            root = self._xml_manager.parse(
+                """
+<application>
+    <component name="XDebuggerSettings">
+    </component>
+</application>
+            """
+            )
+
+        component_element = root.find(".//component[@name='XDebuggerSettings']")
+
+        if root.find(".//debuggers") is None:
+            component_element.append(self._xml_manager.parse("<debuggers></debuggers>"))
+        debuggers = root.find(".//debuggers")
+
+        if debuggers.find(".//debugger[@id='dotnet_debugger']") is None:
+            debuggers.append(
+                self._xml_manager.parse('<debugger id="dotnet_debugger"></debugger>')
+            )
+        dotnet_debugger = debuggers.find(".//debugger[@id='dotnet_debugger']")
+
+        if dotnet_debugger.find(".//configuration") is None:
+            dotnet_debugger.append(
+                self._xml_manager.parse("<configuration></configuration>")
+            )
+        configuration = dotnet_debugger.find(".//configuration")
+
+        if configuration.find(".//option[@name='sshCredentials']") is None:
+            configuration.append(
+                self._xml_manager.parse('<option name="sshCredentials"></option>')
+            )
+        ssh_credentials = configuration.find(".//option[@name='sshCredentials']")
+
+        required_value = f"&lt;credentials HOST=&quot;localhost&quot; PORT=&quot;2222&quot; USERNAME=&quot;root&quot; PRIVATE_KEY_FILE=&quot;{ssh_dir.as_posix()}/key&quot; USE_KEY_PAIR=&quot;true&quot; USE_AUTH_AGENT=&quot;false&quot; /&gt;"
+
+        # Don't do anything if the required entry already exists
+        for option in ssh_credentials.findall(f".//option"):
+            if option.get("value") == required_value.replace("&lt;", "<").replace(
+                "&gt;", ">"
+            ).replace("&quot;", '"'):
+                return
+
+        # Add the new entry to the XML tree
+        ssh_credentials.append(
+            self._xml_manager.parse(f'<option value="{required_value}"/>')
+        )
+
+        # Save the modified XML tree
+        self._generate_file(debugger_file, self._xml_manager.to_string(root))
+
+    def _generate_file(self, file: Path, content: str) -> None:
+        """Writes to a file, which is created if it doesn't exist yet, and normalized the content before doing so.
+
+        :param file: the file to write to
+        :param content: the content to write to the file
+        """
+        file.parent.mkdir(parents=True, exist_ok=True)
+        with file.open("w+", encoding="utf-8") as file:
+            file.write(content.strip() + "\n")
+
+    def _get_jetbrains_config_dirs(self, editor_name: str) -> List[Path]:
+        """Returns the paths to the global configuration directories for all installed editions of a JetBrains IDE.
+
+        :param editor_name: the name of the JetBrains IDE
+        :return: the paths to the directories holding the global configuration for the specified IDE
+        """
+        # Find JetBrains' root directory containing the global configuration directories for all installed IDEs
+        # See https://www.jetbrains.com/help/pycharm/project-and-ide-settings.html#ide_settings
+        if self._platform_manager.is_host_windows():
+            root_dir = Path("~/AppData/Roaming/JetBrains").expanduser()
+        elif self._platform_manager.is_host_macos():
+            root_dir = Path("~/Library/Application Support/JetBrains").expanduser()
+        else:
+            root_dir = Path("~/.config/JetBrains").expanduser()
+
+        if not root_dir.exists():
+            root_dir.mkdir(parents=True)
+
+        # Find the global config directories for the given IDE
+        directories = []
+
+        for path in root_dir.iterdir():
+            if not path.is_dir() or not path.name.startswith(editor_name):
+                continue
+
+            suffix = path.name.replace(editor_name, "")
+            if len(suffix) > 0 and not suffix[0].isdigit():
+                continue
+
+            directories.append(path)
+
+        if len(directories) == 0:
+            directories.append(root_dir / editor_name)
+
+        return directories
```

### Comparing `ablean-1.3.7/ablean/components/util/temp_manager.py` & `ablean-1.3.8/ablean/components/util/temp_manager.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,42 +1,42 @@
-# QUANTCONNECT.COM - Democratizing Finance, Empowering Individuals.
-# Lean CLI v1.0. Copyright 2021 QuantConnect Corporation.
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-
-import shutil
-import tempfile
-from pathlib import Path
-
-
-class TempManager:
-    """The TempManager class provides access to temporary directories."""
-
-    def __init__(self) -> None:
-        """Creates a new TempManager instance."""
-        self._temporary_directories = []
-        self.delete_temporary_directories_when_done = True
-
-    def create_temporary_directory(self) -> Path:
-        """Returns the path to an empty temporary directory.
-
-        :return: a path to an empty temporary directory
-        """
-        path = Path(tempfile.mkdtemp(prefix="lean-cli-"))
-        self._temporary_directories.append(path)
-        return path
-
-    def delete_temporary_directories(self) -> None:
-        """Deletes temporary directories that were created while the CLI ran.
-
-        Only the files that the user can delete are deleted, any permission errors are ignored.
-        """
-        for path in self._temporary_directories:
-            shutil.rmtree(path, ignore_errors=True)
+# QUANTCONNECT.COM - Democratizing Finance, Empowering Individuals.
+# Lean CLI v1.0. Copyright 2021 QuantConnect Corporation.
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+
+import shutil
+import tempfile
+from pathlib import Path
+
+
+class TempManager:
+    """The TempManager class provides access to temporary directories."""
+
+    def __init__(self) -> None:
+        """Creates a new TempManager instance."""
+        self._temporary_directories = []
+        self.delete_temporary_directories_when_done = True
+
+    def create_temporary_directory(self) -> Path:
+        """Returns the path to an empty temporary directory.
+
+        :return: a path to an empty temporary directory
+        """
+        path = Path(tempfile.mkdtemp(prefix="lean-cli-"))
+        self._temporary_directories.append(path)
+        return path
+
+    def delete_temporary_directories(self) -> None:
+        """Deletes temporary directories that were created while the CLI ran.
+
+        Only the files that the user can delete are deleted, any permission errors are ignored.
+        """
+        for path in self._temporary_directories:
+            shutil.rmtree(path, ignore_errors=True)
```

### Comparing `ablean-1.3.7/ablean/components/util/xml_manager.py` & `ablean-1.3.8/ablean/components/util/xml_manager.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,39 +1,39 @@
-# QUANTCONNECT.COM - Democratizing Finance, Empowering Individuals.
-# Lean CLI v1.0. Copyright 2021 QuantConnect Corporation.
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-
-from lxml import etree
-
-
-class XMLManager:
-    """The PathManager class provides utilities for working with XML."""
-
-    def __init__(self) -> None:
-        """Creates a new XMLManager instance."""
-        self._xml_parser = etree.XMLParser(remove_blank_text=True, encoding="utf-8")
-
-    def parse(self, xml_string: str) -> etree.Element:
-        """Parses an XML string to an XML element.
-
-        :param xml_string: the string to parse
-        :return: the parsed XML element
-        """
-        return etree.fromstring(xml_string.encode("utf-8"), parser=self._xml_parser)
-
-    def to_string(self, root: etree.Element) -> str:
-        """Turns an XML element into a pretty string.
-
-        :param root: the XML element to turn into a string
-        :return: the XML element as a pretty string using 4 spaces as indentation
-        """
-        etree.indent(root, " " * 4)
-        return etree.tostring(root, encoding="utf-8", method="xml", pretty_print=True).decode("utf-8")
+# QUANTCONNECT.COM - Democratizing Finance, Empowering Individuals.
+# Lean CLI v1.0. Copyright 2021 QuantConnect Corporation.
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+
+from lxml import etree
+
+
+class XMLManager:
+    """The PathManager class provides utilities for working with XML."""
+
+    def __init__(self) -> None:
+        """Creates a new XMLManager instance."""
+        self._xml_parser = etree.XMLParser(remove_blank_text=True, encoding="utf-8")
+
+    def parse(self, xml_string: str) -> etree.Element:
+        """Parses an XML string to an XML element.
+
+        :param xml_string: the string to parse
+        :return: the parsed XML element
+        """
+        return etree.fromstring(xml_string.encode("utf-8"), parser=self._xml_parser)
+
+    def to_string(self, root: etree.Element) -> str:
+        """Turns an XML element into a pretty string.
+
+        :param root: the XML element to turn into a string
+        :return: the XML element as a pretty string using 4 spaces as indentation
+        """
+        etree.indent(root, " " * 4)
+        return etree.tostring(root, encoding="utf-8", method="xml", pretty_print=True).decode("utf-8")
```

### Comparing `ablean-1.3.7/ablean/constants.py` & `ablean-1.3.8/ablean/constants.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,119 +1,119 @@
-# QUANTCONNECT.COM - Democratizing Finance, Empowering Individuals.
-# Lean CLI v1.0. Copyright 2021 QuantConnect Corporation.
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-
-import os
-from datetime import datetime, timezone
-from pathlib import Path
-
-# Due to the way the filesystem is mocked in unit tests, values should not be Path instances.
-
-# The file in which general CLI configuration is stored
-GENERAL_CONFIG_PATH = str(Path("~/.lean/config").expanduser())
-
-# The file in which credentials are stored
-CREDENTIALS_CONFIG_PATH = str(Path("~/.lean/credentials").expanduser())
-
-# The file in which we store when we last checked for updates
-CACHE_PATH = str(Path("~/.lean/cache").expanduser())
-
-# The directory in which modules are stored
-MODULES_DIRECTORY = str(Path("~/.lean/modules").expanduser())
-
-ENV_LEAN_PATH_NAME = "ABL_LEAN_PATH"
-
-# The default name of the file containing the Lean engine configuration
-DEFAULT_LEAN_CONFIG_FILE_NAME = "lean.json"
-
-# The default name of the directory containing the market data
-DEFAULT_DATA_DIRECTORY_NAME = "data"
-
-# The name of the file in containing the project configuration
-PROJECT_CONFIG_FILE_NAME = "config.json"
-
-# The default Docker image used when running the LEAN engine locally
-DEFAULT_ENGINE_IMAGE = "quantconnect/lean:latest"
-
-# The default Docker image used when running a Jupyter Lab environment locally
-DEFAULT_RESEARCH_IMAGE = "quantconnect/research:latest"
-
-# When we install custom Python libraries, we first mount a volume to the user site packages directory
-# This caches the installation and makes subsequent backtests much faster
-# Because the site packages are not versioned, we cannot reuse the volume between algorithms with different requirements
-# This constant defines how many site packages volumes get created before old ones are removed
-SITE_PACKAGES_VOLUME_LIMIT = 10
-
-# The base url of the QuantConnect API
-# This url should end with a forward slash
-_qc_api = os.environ.get("QC_API", "")
-if _qc_api == "local":
-    API_BASE_URL = "http://localhost:5612/api/v2/"
-elif _qc_api == "beta":
-    API_BASE_URL = "https://beta.quantconnect.com/api/v2/"
-else:
-    API_BASE_URL = "https://www.quantconnect.com/api/v2/"
-
-# The interval in hours at which the CLI checks for updates to itself
-UPDATE_CHECK_INTERVAL_CLI = 24
-
-# The interval in hours at which the CLI checks for updates to Docker images that are being ran
-UPDATE_CHECK_INTERVAL_DOCKER_IMAGE = 24 * 7
-
-# The interval in hours at which the CLI checks for new announcements
-UPDATE_CHECK_INTERVAL_ANNOUNCEMENTS = 24
-
-# The product id of the Equity Security Master subscription
-EQUITY_SECURITY_MASTER_PRODUCT_ID = 37
-
-# The product id of the Equity Bulk Security Master subscription
-BULK_EQUITY_SECURITY_MASTER_PRODUCT_ID = 180
-
-# The product id of the Terminal Link module
-TERMINAL_LINK_PRODUCT_ID = 44
-
-# The product id of the Trading Technologies module
-TRADING_TECHNOLOGIES_PRODUCT_ID = 64
-
-# The product id of the Atreyu module
-ATREYU_PRODUCT_ID = 65
-
-# The product id of the Kraken module
-KRAKEN_PRODUCT_ID = 130
-
-# The product id of the FTX module
-FTX_PRODUCT_ID = 138
-
-# The product id of the ZERODHA module
-ZERODHA_PRODUCT_ID = 174
-
-# The product id of the Binance module
-BINANCE_PRODUCT_ID = 176
-
-# The product id of the SAMCO module
-SAMCO_PRODUCT_ID = 173
-
-# The product id of the Interactive Brokers module
-INTERACTIVE_BROKERS_PRODUCT_ID = 181
-
-# The product ids for which a valid subscription is seen as a valid GUI module subscription
-GUI_PRODUCT_SUBSCRIPTION_IDS = [119, 120]
-
-# The product id of the product the files are retrieved from when installing the GUI module
-GUI_PRODUCT_INSTALL_ID = 119
-
-# The name of the Docker network which all Lean CLI containers are ran on
-DOCKER_NETWORK = "lean_cli"
-
-# The name of the Docker container running the local GUI
-LOCAL_GUI_CONTAINER_NAME = "lean_cli_gui"
-
+# QUANTCONNECT.COM - Democratizing Finance, Empowering Individuals.
+# Lean CLI v1.0. Copyright 2021 QuantConnect Corporation.
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+
+import os
+from datetime import datetime, timezone
+from pathlib import Path
+
+# Due to the way the filesystem is mocked in unit tests, values should not be Path instances.
+
+# The file in which general CLI configuration is stored
+GENERAL_CONFIG_PATH = str(Path("~/.lean/config").expanduser())
+
+# The file in which credentials are stored
+CREDENTIALS_CONFIG_PATH = str(Path("~/.lean/credentials").expanduser())
+
+# The file in which we store when we last checked for updates
+CACHE_PATH = str(Path("~/.lean/cache").expanduser())
+
+# The directory in which modules are stored
+MODULES_DIRECTORY = str(Path("~/.lean/modules").expanduser())
+
+ENV_LEAN_PATH_NAME = "ABL_LEAN_PATH"
+
+# The default name of the file containing the Lean engine configuration
+DEFAULT_LEAN_CONFIG_FILE_NAME = "lean.json"
+
+# The default name of the directory containing the market data
+DEFAULT_DATA_DIRECTORY_NAME = "data"
+
+# The name of the file in containing the project configuration
+PROJECT_CONFIG_FILE_NAME = "config.json"
+
+# The default Docker image used when running the LEAN engine locally
+DEFAULT_ENGINE_IMAGE = "quantconnect/lean:latest"
+
+# The default Docker image used when running a Jupyter Lab environment locally
+DEFAULT_RESEARCH_IMAGE = "quantconnect/research:latest"
+
+# When we install custom Python libraries, we first mount a volume to the user site packages directory
+# This caches the installation and makes subsequent backtests much faster
+# Because the site packages are not versioned, we cannot reuse the volume between algorithms with different requirements
+# This constant defines how many site packages volumes get created before old ones are removed
+SITE_PACKAGES_VOLUME_LIMIT = 10
+
+# The base url of the QuantConnect API
+# This url should end with a forward slash
+_qc_api = os.environ.get("QC_API", "")
+if _qc_api == "local":
+    API_BASE_URL = "http://localhost:5612/api/v2/"
+elif _qc_api == "beta":
+    API_BASE_URL = "https://beta.quantconnect.com/api/v2/"
+else:
+    API_BASE_URL = "https://www.quantconnect.com/api/v2/"
+
+# The interval in hours at which the CLI checks for updates to itself
+UPDATE_CHECK_INTERVAL_CLI = 24
+
+# The interval in hours at which the CLI checks for updates to Docker images that are being ran
+UPDATE_CHECK_INTERVAL_DOCKER_IMAGE = 24 * 7
+
+# The interval in hours at which the CLI checks for new announcements
+UPDATE_CHECK_INTERVAL_ANNOUNCEMENTS = 24
+
+# The product id of the Equity Security Master subscription
+EQUITY_SECURITY_MASTER_PRODUCT_ID = 37
+
+# The product id of the Equity Bulk Security Master subscription
+BULK_EQUITY_SECURITY_MASTER_PRODUCT_ID = 180
+
+# The product id of the Terminal Link module
+TERMINAL_LINK_PRODUCT_ID = 44
+
+# The product id of the Trading Technologies module
+TRADING_TECHNOLOGIES_PRODUCT_ID = 64
+
+# The product id of the Atreyu module
+ATREYU_PRODUCT_ID = 65
+
+# The product id of the Kraken module
+KRAKEN_PRODUCT_ID = 130
+
+# The product id of the FTX module
+FTX_PRODUCT_ID = 138
+
+# The product id of the ZERODHA module
+ZERODHA_PRODUCT_ID = 174
+
+# The product id of the Binance module
+BINANCE_PRODUCT_ID = 176
+
+# The product id of the SAMCO module
+SAMCO_PRODUCT_ID = 173
+
+# The product id of the Interactive Brokers module
+INTERACTIVE_BROKERS_PRODUCT_ID = 181
+
+# The product ids for which a valid subscription is seen as a valid GUI module subscription
+GUI_PRODUCT_SUBSCRIPTION_IDS = [119, 120]
+
+# The product id of the product the files are retrieved from when installing the GUI module
+GUI_PRODUCT_INSTALL_ID = 119
+
+# The name of the Docker network which all Lean CLI containers are ran on
+DOCKER_NETWORK = "lean_cli"
+
+# The name of the Docker container running the local GUI
+LOCAL_GUI_CONTAINER_NAME = "lean_cli_gui"
+
 DATA_HASH_FILE = 'data_hash.csv'
```

### Comparing `ablean-1.3.7/ablean/container.py` & `ablean-1.3.8/ablean/container.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,72 +1,72 @@
-# QUANTCONNECT.COM - Democratizing Finance, Empowering Individuals.
-# Lean CLI v1.0. Copyright 2021 QuantConnect Corporation.
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-
-from dependency_injector.containers import DeclarativeContainer
-from dependency_injector.providers import Factory, Singleton
-
-from ablean.components.config.cli_config_manager import CLIConfigManager
-from ablean.components.config.lean_config_manager import LeanConfigManager
-from ablean.components.config.output_config_manager import OutputConfigManager
-from ablean.components.config.project_config_manager import ProjectConfigManager
-from ablean.components.config.storage import Storage
-from ablean.components.util.logger import Logger
-from ablean.components.util.name_generator import NameGenerator
-from ablean.components.util.path_manager import PathManager
-from ablean.components.util.platform_manager import PlatformManager
-from ablean.components.util.project_manager import ProjectManager
-from ablean.components.util.temp_manager import TempManager
-from ablean.components.util.xml_manager import XMLManager
-from ablean.components.module_manager import ModuleManager
-from ablean.components.lean_runner import LeanRunner
-from ablean.constants import CACHE_PATH, CREDENTIALS_CONFIG_PATH, GENERAL_CONFIG_PATH
-from ablean.data_manager import DataManager
-
-class Container(DeclarativeContainer):
-    """The Container class wires all reusable components together."""
-
-    logger = Singleton(Logger)
-    xml_manager = Singleton(XMLManager)
-    platform_manager = Singleton(PlatformManager)
-    name_generator = Singleton(NameGenerator)
-    path_manager = Singleton(PathManager, platform_manager)
-    temp_manager = Singleton(TempManager)
-    module_manager = Singleton(ModuleManager, logger)
-    general_storage = Singleton(Storage, file=GENERAL_CONFIG_PATH)
-    credentials_storage = Singleton(Storage, file=CREDENTIALS_CONFIG_PATH)
-    cache_storage = Singleton(Storage, file=CACHE_PATH)
-    cli_config_manager = Singleton(CLIConfigManager, general_storage, credentials_storage)
-    project_config_manager = Singleton(ProjectConfigManager, xml_manager)
-    lean_config_manager = Singleton(LeanConfigManager,
-                                    logger,
-                                    cli_config_manager,
-                                    project_config_manager,
-                                    module_manager,
-                                    cache_storage)
-
-    output_config_manager = Singleton(OutputConfigManager, lean_config_manager)
-    project_manager = Singleton(ProjectManager,
-                                project_config_manager,
-                                lean_config_manager,
-                                xml_manager,
-                                platform_manager)    
-    data_manager = Singleton(DataManager, lean_config_manager, logger)
-    lean_runner = Singleton(LeanRunner,
-                            logger,
-                            project_config_manager,
-                            lean_config_manager,
-                            output_config_manager,
-                            module_manager,
-                            project_manager,
-                            temp_manager,
-                            xml_manager)
-container = Container()
+# QUANTCONNECT.COM - Democratizing Finance, Empowering Individuals.
+# Lean CLI v1.0. Copyright 2021 QuantConnect Corporation.
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+
+from dependency_injector.containers import DeclarativeContainer
+from dependency_injector.providers import Factory, Singleton
+
+from ablean.components.config.cli_config_manager import CLIConfigManager
+from ablean.components.config.lean_config_manager import LeanConfigManager
+from ablean.components.config.output_config_manager import OutputConfigManager
+from ablean.components.config.project_config_manager import ProjectConfigManager
+from ablean.components.config.storage import Storage
+from ablean.components.util.logger import Logger
+from ablean.components.util.name_generator import NameGenerator
+from ablean.components.util.path_manager import PathManager
+from ablean.components.util.platform_manager import PlatformManager
+from ablean.components.util.project_manager import ProjectManager
+from ablean.components.util.temp_manager import TempManager
+from ablean.components.util.xml_manager import XMLManager
+from ablean.components.module_manager import ModuleManager
+from ablean.components.lean_runner import LeanRunner
+from ablean.constants import CACHE_PATH, CREDENTIALS_CONFIG_PATH, GENERAL_CONFIG_PATH
+from ablean.data_manager import DataManager
+
+class Container(DeclarativeContainer):
+    """The Container class wires all reusable components together."""
+
+    logger = Singleton(Logger)
+    xml_manager = Singleton(XMLManager)
+    platform_manager = Singleton(PlatformManager)
+    name_generator = Singleton(NameGenerator)
+    path_manager = Singleton(PathManager, platform_manager)
+    temp_manager = Singleton(TempManager)
+    module_manager = Singleton(ModuleManager, logger)
+    general_storage = Singleton(Storage, file=GENERAL_CONFIG_PATH)
+    credentials_storage = Singleton(Storage, file=CREDENTIALS_CONFIG_PATH)
+    cache_storage = Singleton(Storage, file=CACHE_PATH)
+    cli_config_manager = Singleton(CLIConfigManager, general_storage, credentials_storage)
+    project_config_manager = Singleton(ProjectConfigManager, xml_manager)
+    lean_config_manager = Singleton(LeanConfigManager,
+                                    logger,
+                                    cli_config_manager,
+                                    project_config_manager,
+                                    module_manager,
+                                    cache_storage)
+
+    output_config_manager = Singleton(OutputConfigManager, lean_config_manager)
+    project_manager = Singleton(ProjectManager,
+                                project_config_manager,
+                                lean_config_manager,
+                                xml_manager,
+                                platform_manager)    
+    data_manager = Singleton(DataManager, lean_config_manager, logger)
+    lean_runner = Singleton(LeanRunner,
+                            logger,
+                            project_config_manager,
+                            lean_config_manager,
+                            output_config_manager,
+                            module_manager,
+                            project_manager,
+                            temp_manager,
+                            xml_manager)
+container = Container()
```

### Comparing `ablean-1.3.7/ablean/data_manager.py` & `ablean-1.3.8/ablean/data_manager.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,235 +1,235 @@
-import csv
-from datetime import datetime
-import hashlib
-from lib2to3.pytree import Node
-import math
-import shutil
-import sys
-import pathlib
-import logging
-import argparse
-from typing import Dict, Optional
-from os import listdir, scandir
-from os.path import join, exists, isfile, getsize
-from paramiko import SSHClient, AutoAddPolicy
-from scp import SCPClient
-from ablean.components.util.logger import Logger
-from ablean.components.config.lean_config_manager import LeanConfigManager
-from ablean.constants import DATA_HASH_FILE, DEFAULT_LEAN_CONFIG_FILE_NAME
-
-DATE_FORMAT = "%Y%m%d"
-OPTION_DATE_START_POS = -len('20220523_quote_european.zip')
-OPTION_DATE_END_POS = -len('_quote_european.zip')
-OTHER_DATE_START_POS = -len('20220523_quote.zip')
-OTHER_DATE_END_POS = -len('_quote.zip')
-
-
-def get_file_hash(local_file: str):
-    md5_object = hashlib.md5()
-    block_size = 64 * md5_object.block_size
-    with open(local_file, 'rb') as f:
-        chunk = f.read(block_size)
-        while chunk:
-            md5_object.update(chunk)
-            chunk = f.read(block_size)
-    return md5_object.hexdigest()
-
-
-def scantree(path):
-    """Recursively yield DirEntry objects for given directory."""
-    for entry in scandir(path):
-        if entry.is_dir(follow_symlinks=False):
-            yield from scantree(entry.path)  # see below for Python 2.x
-        else:
-            yield entry
-
-
-def convert_size(size_bytes):
-    if size_bytes == 0:
-        return "0B"
-    size_name = ("B", "KB", "MB", "GB", "TB", "PB", "EB", "ZB", "YB")
-    i = int(math.floor(math.log(size_bytes, 1024)))
-    p = math.pow(1024, i)
-    s = round(size_bytes / p, 2)
-    return "%s %s" % (s, size_name[i])
-
-
-class DataManager:
-    def __init__(
-        self,
-        lean_config_manager: LeanConfigManager,
-        logger: Logger,
-    ):
-        self.lean_config_manager = lean_config_manager
-        self.logger = logger
-        self.progress = None
-        self.progress_task = None
-        self._load_config()
-
-    def _load_data_hash(self, filename: str = DATA_HASH_FILE):
-        filename = join(self.output_path, filename)
-        if exists(filename):
-            with open(filename, mode='r') as infile:
-                reader = csv.reader(infile)
-                return {rows[0]: rows[1] for rows in reader}
-        else:
-            return {}
-
-    def _scp_get(
-        self, scp: SCPClient, remote_path: str, local_path: str, recursive: bool = False
-    ):
-        if self.progress is not None:
-            self.progress.stop()
-        self.progress = self.logger.progress()
-        self.progress_task = self.progress.add_task(remote_path)
-        try:
-            scp.get(remote_path, local_path, recursive)
-        except KeyboardInterrupt as e:
-            if self.progress is not None:
-                self.progress.stop()
-            raise e
-        pass
-
-    def _download_data_file(
-        self,
-        scp: SCPClient,
-        remote_file: str,
-        local_file: str,
-        hash: str = None,
-    ):
-        remote_file = f"{self.remote_path}/{remote_file}".replace('//', '/')
-        local_file = f"{self.output_path}/{local_file}".replace('//', '/')
-        if not exists(local_file):
-            local_path = pathlib.Path(local_file).parent.resolve()
-            local_path.mkdir(parents=True, exist_ok=True)
-        elif get_file_hash(local_file) == hash:
-            self.logger.info(f'{local_file} is OK!')
-            return
-
-        if hash is None:
-            self._scp_get(scp, remote_file, local_file)
-        else:
-            temp_file = f"{self.output_path}/{hash}.tmp".replace('//', '/')
-            self._scp_get(scp, remote_file, temp_file)
-            shutil.move(temp_file, local_file)
-
-    def _create_data_hash(self, hash_table: Dict):
-        for path in ['option', 'future', 'crypto']:
-            path = join(self.output_path, path)
-            if not exists(path):
-                continue
-            for item in scantree(path):
-                if not item.path.endswith(".zip"):
-                    continue
-                self._update_file_hash(item.path, hash_table)
-                self.logger.info(f"init {item.path} hash")
-
-    def _get_file_key(self, local_file: str):
-        return local_file[len(self.output_path) :].replace('\\', '/')
-
-    def _update_file_hash(self, local_file: str, hash_table: Dict):
-        md5 = get_file_hash(local_file)
-        key = self._get_file_key(local_file)
-        hash_table[key] = md5
-        pass
-
-    def _save_data_hash(self, hash_table: Dict):
-        filename = join(self.output_path, DATA_HASH_FILE)
-        with open(filename, mode='w') as outfile:
-            for k, v in hash_table.items():
-                outfile.write(f"{k},{v}\n")
-
-    def _on_data(self, filename: str, size: int, send: int):
-        if size >= send:
-            send_size = convert_size(send)
-            file_size = convert_size(size) + ' ' * 5
-            desc = f'{send_size}/{file_size}'
-            self.progress.update(
-                self.progress_task,
-                completed=(send / float(size) * 100),
-                description=desc,
-            )
-
-    def _load_config(self):
-        config = self.lean_config_manager.get_lean_config()
-        self.output_path = config["data-folder"]
-        self.remote_path = config["remote-data-folder"]
-        self.ssh_host = config["ssh-host"]
-        self.ssh_port = config["ssh-port"]
-        self.ssh_user = config["ssh-user"]
-        self.ssh_password = config["ssh-pwd"]
-        self.update_second_data = config["update-second-data"]
-
-    def _create_scp(self):
-        ssh = SSHClient()
-        ssh.load_system_host_keys()
-        ssh.set_missing_host_key_policy(AutoAddPolicy())
-        ssh.connect(
-            self.ssh_host,
-            port=self.ssh_port,
-            username=self.ssh_user,
-            password=self.ssh_password,
-            compress=True,
-        )
-        return SCPClient(ssh.get_transport(), progress=self._on_data)
-
-    def update_data(
-        self,
-        update_second_data=False,
-        force_update=False,
-        data_path: str = None,
-        date_start=Optional[datetime],
-        date_end=Optional[datetime],
-        market: str = None,
-    ):
-        self._load_config()
-        if data_path is not None:
-            self.output_path = data_path
-        self.logger.info(f"update data from {self.ssh_host}")
-        local_hash = self._load_data_hash()
-        if force_update or len(local_hash) == 0:
-            self._create_data_hash(local_hash)
-            self._save_data_hash(local_hash)
-
-        scp = self._create_scp()
-        self._download_data_file(scp, DATA_HASH_FILE, f'server_{DATA_HASH_FILE}')
-        remote_hash = self._load_data_hash(f'server_{DATA_HASH_FILE}')
-        update_second_data = update_second_data or self.update_second_data
-        
-        for k, v in remote_hash.items():
-            if k in local_hash and v == local_hash[k]:
-                continue
-            if 'second' in k and not update_second_data:
-                continue
-            
-            if market is not None:
-                if k[len('/crypto/'):len('/crypto/')+len(market)] != market:
-                    continue
-
-            if k.endswith('european.zip'):
-                file_date = datetime.strptime(
-                    k[OPTION_DATE_START_POS:OPTION_DATE_END_POS], DATE_FORMAT
-                )
-            else:
-                file_date = datetime.strptime(
-                    k[OTHER_DATE_START_POS:OTHER_DATE_END_POS], DATE_FORMAT
-                )
-
-            if date_start is not None and file_date < date_start:
-                continue
-
-            if date_end is not None and file_date > date_end:
-                continue
-
-            self.logger.info(f"download: {k}")
-            self._download_data_file(scp, k, k, v)
-            local_hash[k] = v
-        self._save_data_hash(local_hash)
-
-    def update_lean(self, output: str):
-        self._load_config()
-        scp = self._create_scp()
-        self.logger.info("download lean.json")
-        self._scp_get(scp, '/mnt/data/share/lean/lean.json', output)
-        self.logger.info("download launcher")
-        self._scp_get(scp, '/mnt/data/share/lean/launcher', output, True)
+import csv
+from datetime import datetime
+import hashlib
+from lib2to3.pytree import Node
+import math
+import shutil
+import sys
+import pathlib
+import logging
+import argparse
+from typing import Dict, Optional
+from os import listdir, scandir
+from os.path import join, exists, isfile, getsize
+from paramiko import SSHClient, AutoAddPolicy
+from scp import SCPClient
+from ablean.components.util.logger import Logger
+from ablean.components.config.lean_config_manager import LeanConfigManager
+from ablean.constants import DATA_HASH_FILE, DEFAULT_LEAN_CONFIG_FILE_NAME
+
+DATE_FORMAT = "%Y%m%d"
+OPTION_DATE_START_POS = -len('20220523_quote_european.zip')
+OPTION_DATE_END_POS = -len('_quote_european.zip')
+OTHER_DATE_START_POS = -len('20220523_quote.zip')
+OTHER_DATE_END_POS = -len('_quote.zip')
+
+
+def get_file_hash(local_file: str):
+    md5_object = hashlib.md5()
+    block_size = 64 * md5_object.block_size
+    with open(local_file, 'rb') as f:
+        chunk = f.read(block_size)
+        while chunk:
+            md5_object.update(chunk)
+            chunk = f.read(block_size)
+    return md5_object.hexdigest()
+
+
+def scantree(path):
+    """Recursively yield DirEntry objects for given directory."""
+    for entry in scandir(path):
+        if entry.is_dir(follow_symlinks=False):
+            yield from scantree(entry.path)  # see below for Python 2.x
+        else:
+            yield entry
+
+
+def convert_size(size_bytes):
+    if size_bytes == 0:
+        return "0B"
+    size_name = ("B", "KB", "MB", "GB", "TB", "PB", "EB", "ZB", "YB")
+    i = int(math.floor(math.log(size_bytes, 1024)))
+    p = math.pow(1024, i)
+    s = round(size_bytes / p, 2)
+    return "%s %s" % (s, size_name[i])
+
+
+class DataManager:
+    def __init__(
+        self,
+        lean_config_manager: LeanConfigManager,
+        logger: Logger,
+    ):
+        self.lean_config_manager = lean_config_manager
+        self.logger = logger
+        self.progress = None
+        self.progress_task = None
+        self._load_config()
+
+    def _load_data_hash(self, filename: str = DATA_HASH_FILE):
+        filename = join(self.output_path, filename)
+        if exists(filename):
+            with open(filename, mode='r') as infile:
+                reader = csv.reader(infile)
+                return {rows[0]: rows[1] for rows in reader}
+        else:
+            return {}
+
+    def _scp_get(
+        self, scp: SCPClient, remote_path: str, local_path: str, recursive: bool = False
+    ):
+        if self.progress is not None:
+            self.progress.stop()
+        self.progress = self.logger.progress()
+        self.progress_task = self.progress.add_task(remote_path)
+        try:
+            scp.get(remote_path, local_path, recursive)
+        except KeyboardInterrupt as e:
+            if self.progress is not None:
+                self.progress.stop()
+            raise e
+        pass
+
+    def _download_data_file(
+        self,
+        scp: SCPClient,
+        remote_file: str,
+        local_file: str,
+        hash: str = None,
+    ):
+        remote_file = f"{self.remote_path}/{remote_file}".replace('//', '/')
+        local_file = f"{self.output_path}/{local_file}".replace('//', '/')
+        if not exists(local_file):
+            local_path = pathlib.Path(local_file).parent.resolve()
+            local_path.mkdir(parents=True, exist_ok=True)
+        elif get_file_hash(local_file) == hash:
+            self.logger.info(f'{local_file} is OK!')
+            return
+
+        if hash is None:
+            self._scp_get(scp, remote_file, local_file)
+        else:
+            temp_file = f"{self.output_path}/{hash}.tmp".replace('//', '/')
+            self._scp_get(scp, remote_file, temp_file)
+            shutil.move(temp_file, local_file)
+
+    def _create_data_hash(self, hash_table: Dict):
+        for path in ['option', 'future', 'crypto']:
+            path = join(self.output_path, path)
+            if not exists(path):
+                continue
+            for item in scantree(path):
+                if not item.path.endswith(".zip"):
+                    continue
+                self._update_file_hash(item.path, hash_table)
+                self.logger.info(f"init {item.path} hash")
+
+    def _get_file_key(self, local_file: str):
+        return local_file[len(self.output_path) :].replace('\\', '/')
+
+    def _update_file_hash(self, local_file: str, hash_table: Dict):
+        md5 = get_file_hash(local_file)
+        key = self._get_file_key(local_file)
+        hash_table[key] = md5
+        pass
+
+    def _save_data_hash(self, hash_table: Dict):
+        filename = join(self.output_path, DATA_HASH_FILE)
+        with open(filename, mode='w') as outfile:
+            for k, v in hash_table.items():
+                outfile.write(f"{k},{v}\n")
+
+    def _on_data(self, filename: str, size: int, send: int):
+        if size >= send:
+            send_size = convert_size(send)
+            file_size = convert_size(size) + ' ' * 5
+            desc = f'{send_size}/{file_size}'
+            self.progress.update(
+                self.progress_task,
+                completed=(send / float(size) * 100),
+                description=desc,
+            )
+
+    def _load_config(self):
+        config = self.lean_config_manager.get_lean_config()
+        self.output_path = config["data-folder"]
+        self.remote_path = config["remote-data-folder"]
+        self.ssh_host = config["ssh-host"]
+        self.ssh_port = config["ssh-port"]
+        self.ssh_user = config["ssh-user"]
+        self.ssh_password = config["ssh-pwd"]
+        self.update_second_data = config["update-second-data"]
+
+    def _create_scp(self):
+        ssh = SSHClient()
+        ssh.load_system_host_keys()
+        ssh.set_missing_host_key_policy(AutoAddPolicy())
+        ssh.connect(
+            self.ssh_host,
+            port=self.ssh_port,
+            username=self.ssh_user,
+            password=self.ssh_password,
+            compress=True,
+        )
+        return SCPClient(ssh.get_transport(), progress=self._on_data)
+
+    def update_data(
+        self,
+        update_second_data=False,
+        force_update=False,
+        data_path: str = None,
+        date_start=Optional[datetime],
+        date_end=Optional[datetime],
+        market: str = None,
+    ):
+        self._load_config()
+        if data_path is not None:
+            self.output_path = data_path
+        self.logger.info(f"update data from {self.ssh_host}")
+        local_hash = self._load_data_hash()
+        if force_update or len(local_hash) == 0:
+            self._create_data_hash(local_hash)
+            self._save_data_hash(local_hash)
+
+        scp = self._create_scp()
+        self._download_data_file(scp, DATA_HASH_FILE, f'server_{DATA_HASH_FILE}')
+        remote_hash = self._load_data_hash(f'server_{DATA_HASH_FILE}')
+        update_second_data = update_second_data or self.update_second_data
+        
+        for k, v in remote_hash.items():
+            if k in local_hash and v == local_hash[k]:
+                continue
+            if 'second' in k and not update_second_data:
+                continue
+            
+            if market is not None:
+                if k[len('/crypto/'):len('/crypto/')+len(market)] != market:
+                    continue
+
+            if k.endswith('european.zip'):
+                file_date = datetime.strptime(
+                    k[OPTION_DATE_START_POS:OPTION_DATE_END_POS], DATE_FORMAT
+                )
+            else:
+                file_date = datetime.strptime(
+                    k[OTHER_DATE_START_POS:OTHER_DATE_END_POS], DATE_FORMAT
+                )
+
+            if date_start is not None and file_date < date_start:
+                continue
+
+            if date_end is not None and file_date > date_end:
+                continue
+
+            self.logger.info(f"download: {k}")
+            self._download_data_file(scp, k, k, v)
+            local_hash[k] = v
+        self._save_data_hash(local_hash)
+
+    def update_lean(self, output: str):
+        self._load_config()
+        scp = self._create_scp()
+        self.logger.info("download lean.json")
+        self._scp_get(scp, '/mnt/data/share/lean/lean.json', output)
+        self.logger.info("download launcher")
+        self._scp_get(scp, '/mnt/data/share/lean/launcher', output, True)
```

### Comparing `ablean-1.3.7/ablean/icons/icon.icns` & `ablean-1.3.8/ablean/icons/icon.icns`

 * *Files identical despite different names*

### Comparing `ablean-1.3.7/ablean/icons/icon.ico` & `ablean-1.3.8/ablean/icons/icon.ico`

 * *Files identical despite different names*

### Comparing `ablean-1.3.7/ablean/main.py` & `ablean-1.3.8/ablean/main.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,143 +1,143 @@
-# QUANTCONNECT.COM - Democratizing Finance, Empowering Individuals.
-# Lean CLI v1.0. Copyright 2021 QuantConnect Corporation.
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-
-import ctypes
-import os
-import platform
-import site
-import sys
-import time
-from pathlib import Path
-
-
-# Docker's pywin32 dependency on Windows is a common source of issues
-# In a lot of cases you'd have to manually run pywin32's post-install script as admin after pip installing the library
-# This is a hassle, so the CLI attempts to automate this step when it's necessary
-# Additionally, we can also fix the issues for some users by updating os.environ["PATH"]
-# If this works we use this fix instead as it removes the need to request admin permissions
-# This code must run before the Docker package is imported anywhere in the code
-
-def _is_win32_available() -> bool:
-    try:
-        # Try the win32 APIs used by https://github.com/docker/docker-py/blob/master/docker/transport/npipesocket.py
-        import win32file
-        import win32pipe
-        return True
-    except:
-        return False
-
-
-def _ensure_win32_available() -> None:
-    if _is_win32_available():
-        return
-
-    possible_paths = sys.path + [sys.prefix] + site.getsitepackages() + [site.getusersitepackages()]
-    possible_paths = [Path(p) for p in possible_paths]
-    possible_directories = set(p for p in possible_paths if p.is_dir())
-
-    for directory in possible_directories:
-        target_directory = directory / "pywin32_system32"
-        if not target_directory.is_dir():
-            continue
-
-        os.environ["PATH"] += ";" + str(target_directory)
-
-        if _is_win32_available():
-            return
-
-    for directory in possible_directories:
-        target_file = directory / "Scripts" / "pywin32_postinstall.py"
-        if not target_file.is_file():
-            continue
-
-        print(f"Running pywin32's post-install script at {target_file}")
-        ctypes.windll.shell32.ShellExecuteW(None, "runas", sys.executable, f'"{target_file}" -install', None, 1)
-
-        # ShellExecuteW returns immediately after the UAC dialog, we wait a second to give the script some time to run
-        time.sleep(1)
-
-        if _is_win32_available():
-            return
-
-    if any("AppData\\Local\\Packages\\PythonSoftwareFoundation.Python" in p for p in sys.path):
-        print("It looks like you're using the Python distribution from the Microsoft Store")
-        print("This distribution is not supported by the CLI, we recommend using the Anaconda distribution instead")
-        print(
-            "See https://www.lean.io/docs/lean-cli/installation/installing-pip#02-Install-on-Windows for more information")
-        sys.exit(1)
-
-    print("pywin32 has not been installed completely, which may lead to errors")
-    print("You can fix this issue by running pywin32's post-install script")
-    print(f"Run the following command in an elevated terminal from your Python environment's Scripts directory:")
-    print("python pywin32_postinstall.py -install")
-
-
-if platform.system() == "Windows":
-    _ensure_win32_available()
-
-import traceback
-from io import StringIO
-
-import click
-import requests
-from pydantic import ValidationError
-
-from ablean.commands import lean
-from ablean.container import container
-from ablean.models.errors import MoreInfoError
-
-
-def main() -> None:
-    """This function is the entrypoint when running a Lean command in a terminal."""
-    try:
-        lean.main(standalone_mode=False)
-
-        temp_manager = container.temp_manager()
-        if temp_manager.delete_temporary_directories_when_done:
-            temp_manager.delete_temporary_directories()
-    except Exception as exception:
-        logger = container.logger()
-        logger.debug(traceback.format_exc().strip())
-
-        if isinstance(exception, ValidationError) and hasattr(exception, "input_value"):
-            logger.debug("Value that failed validation:")
-            logger.debug(exception.input_value)
-            logger.error(f"Error: {exception}")
-        elif isinstance(exception, MoreInfoError):
-            logger.error(f"Error: {exception}")
-            logger.error(f"Visit {exception.link} for more information")
-        elif isinstance(exception, click.UsageError):
-            io = StringIO()
-            exception.show(file=io)
-
-            exception_str = io.getvalue().strip()
-            exception_str = exception_str.replace("Try 'lean", "\nTry 'lean")
-            exception_str = exception_str.replace("for help.",
-                                                  "for help or go to the following url for a list of common errors:\nhttps://www.lean.io/docs/lean-cli/key-concepts/troubleshooting#02-Common-Errors")
-            logger.info(exception_str)
-        elif isinstance(exception, click.Abort):
-            logger.info("Aborted!")
-        elif isinstance(exception, requests.exceptions.ConnectionError):
-            logger.error(f"Error: {exception}")
-            logger.error("It looks like you don't have an internet connection, please check your system settings")
-        else:
-            logger.error(f"Error: {exception}")
-
-        temp_manager = container.temp_manager()
-        if temp_manager.delete_temporary_directories_when_done:
-            temp_manager.delete_temporary_directories()
-
-        sys.exit(1)
-
-if __name__ == "__main__":
+# QUANTCONNECT.COM - Democratizing Finance, Empowering Individuals.
+# Lean CLI v1.0. Copyright 2021 QuantConnect Corporation.
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+
+import ctypes
+import os
+import platform
+import site
+import sys
+import time
+from pathlib import Path
+
+
+# Docker's pywin32 dependency on Windows is a common source of issues
+# In a lot of cases you'd have to manually run pywin32's post-install script as admin after pip installing the library
+# This is a hassle, so the CLI attempts to automate this step when it's necessary
+# Additionally, we can also fix the issues for some users by updating os.environ["PATH"]
+# If this works we use this fix instead as it removes the need to request admin permissions
+# This code must run before the Docker package is imported anywhere in the code
+
+def _is_win32_available() -> bool:
+    try:
+        # Try the win32 APIs used by https://github.com/docker/docker-py/blob/master/docker/transport/npipesocket.py
+        import win32file
+        import win32pipe
+        return True
+    except:
+        return False
+
+
+def _ensure_win32_available() -> None:
+    if _is_win32_available():
+        return
+
+    possible_paths = sys.path + [sys.prefix] + site.getsitepackages() + [site.getusersitepackages()]
+    possible_paths = [Path(p) for p in possible_paths]
+    possible_directories = set(p for p in possible_paths if p.is_dir())
+
+    for directory in possible_directories:
+        target_directory = directory / "pywin32_system32"
+        if not target_directory.is_dir():
+            continue
+
+        os.environ["PATH"] += ";" + str(target_directory)
+
+        if _is_win32_available():
+            return
+
+    for directory in possible_directories:
+        target_file = directory / "Scripts" / "pywin32_postinstall.py"
+        if not target_file.is_file():
+            continue
+
+        print(f"Running pywin32's post-install script at {target_file}")
+        ctypes.windll.shell32.ShellExecuteW(None, "runas", sys.executable, f'"{target_file}" -install', None, 1)
+
+        # ShellExecuteW returns immediately after the UAC dialog, we wait a second to give the script some time to run
+        time.sleep(1)
+
+        if _is_win32_available():
+            return
+
+    if any("AppData\\Local\\Packages\\PythonSoftwareFoundation.Python" in p for p in sys.path):
+        print("It looks like you're using the Python distribution from the Microsoft Store")
+        print("This distribution is not supported by the CLI, we recommend using the Anaconda distribution instead")
+        print(
+            "See https://www.lean.io/docs/lean-cli/installation/installing-pip#02-Install-on-Windows for more information")
+        sys.exit(1)
+
+    print("pywin32 has not been installed completely, which may lead to errors")
+    print("You can fix this issue by running pywin32's post-install script")
+    print(f"Run the following command in an elevated terminal from your Python environment's Scripts directory:")
+    print("python pywin32_postinstall.py -install")
+
+
+if platform.system() == "Windows":
+    _ensure_win32_available()
+
+import traceback
+from io import StringIO
+
+import click
+import requests
+from pydantic import ValidationError
+
+from ablean.commands import lean
+from ablean.container import container
+from ablean.models.errors import MoreInfoError
+
+
+def main() -> None:
+    """This function is the entrypoint when running a Lean command in a terminal."""
+    try:
+        lean.main(standalone_mode=False)
+
+        temp_manager = container.temp_manager()
+        if temp_manager.delete_temporary_directories_when_done:
+            temp_manager.delete_temporary_directories()
+    except Exception as exception:
+        logger = container.logger()
+        logger.debug(traceback.format_exc().strip())
+
+        if isinstance(exception, ValidationError) and hasattr(exception, "input_value"):
+            logger.debug("Value that failed validation:")
+            logger.debug(exception.input_value)
+            logger.error(f"Error: {exception}")
+        elif isinstance(exception, MoreInfoError):
+            logger.error(f"Error: {exception}")
+            logger.error(f"Visit {exception.link} for more information")
+        elif isinstance(exception, click.UsageError):
+            io = StringIO()
+            exception.show(file=io)
+
+            exception_str = io.getvalue().strip()
+            exception_str = exception_str.replace("Try 'lean", "\nTry 'lean")
+            exception_str = exception_str.replace("for help.",
+                                                  "for help or go to the following url for a list of common errors:\nhttps://www.lean.io/docs/lean-cli/key-concepts/troubleshooting#02-Common-Errors")
+            logger.info(exception_str)
+        elif isinstance(exception, click.Abort):
+            logger.info("Aborted!")
+        elif isinstance(exception, requests.exceptions.ConnectionError):
+            logger.error(f"Error: {exception}")
+            logger.error("It looks like you don't have an internet connection, please check your system settings")
+        else:
+            logger.error(f"Error: {exception}")
+
+        temp_manager = container.temp_manager()
+        if temp_manager.delete_temporary_directories_when_done:
+            temp_manager.delete_temporary_directories()
+
+        sys.exit(1)
+
+if __name__ == "__main__":
     main()
```

### Comparing `ablean-1.3.7/ablean/models/__init__.py` & `ablean-1.3.8/ablean/models/__init__.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-# QUANTCONNECT.COM - Democratizing Finance, Empowering Individuals.
-# Lean CLI v1.0. Copyright 2021 QuantConnect Corporation.
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
+# QUANTCONNECT.COM - Democratizing Finance, Empowering Individuals.
+# Lean CLI v1.0. Copyright 2021 QuantConnect Corporation.
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
```

### Comparing `ablean-1.3.7/ablean/models/errors.py` & `ablean-1.3.8/ablean/models/errors.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,57 +1,57 @@
-# QUANTCONNECT.COM - Democratizing Finance, Empowering Individuals.
-# Lean CLI v1.0. Copyright 2021 QuantConnect Corporation.
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-
-from typing import Optional
-
-import requests
-
-
-class RequestFailedError(Exception):
-    """A RequestFailedError indicates that an HTTP request has failed."""
-
-    def __init__(self, response: requests.Response, message: Optional[str] = None) -> None:
-        """Creates a new RequestFailedError instance.
-
-        :param response: the data of the failed response
-        :param message: a display-friendly error message, defaults to a message based on the response
-        """
-        if message is None:
-            request = response.request
-            message = f"{request.method} request to {request.url} failed with status code {response.status_code}"
-
-        super().__init__(message)
-
-        self.response = response
-
-
-class MoreInfoError(Exception):
-    """An error which consists of a message and a link to documentation with more information."""
-
-    def __init__(self, message: str, link: str) -> None:
-        """Creates a new MoreInfoError instance.
-
-        :param message: the error message
-        :param link: the link to documentation containing more information
-        """
-        super().__init__(message)
-
-        self.link = link
-
-
-class AuthenticationError(MoreInfoError):
-    """An error indicating that a request has failed because the used credentials were invalid."""
-
-    def __init__(self) -> None:
-        """Creates a new AuthenticationError instance."""
-        super().__init__("Invalid credentials, please log in using `lean login`",
-                         "https://www.lean.io/docs/lean-cli/initialization/authenticating-accounts#02-Log-In")
+# QUANTCONNECT.COM - Democratizing Finance, Empowering Individuals.
+# Lean CLI v1.0. Copyright 2021 QuantConnect Corporation.
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+
+from typing import Optional
+
+import requests
+
+
+class RequestFailedError(Exception):
+    """A RequestFailedError indicates that an HTTP request has failed."""
+
+    def __init__(self, response: requests.Response, message: Optional[str] = None) -> None:
+        """Creates a new RequestFailedError instance.
+
+        :param response: the data of the failed response
+        :param message: a display-friendly error message, defaults to a message based on the response
+        """
+        if message is None:
+            request = response.request
+            message = f"{request.method} request to {request.url} failed with status code {response.status_code}"
+
+        super().__init__(message)
+
+        self.response = response
+
+
+class MoreInfoError(Exception):
+    """An error which consists of a message and a link to documentation with more information."""
+
+    def __init__(self, message: str, link: str) -> None:
+        """Creates a new MoreInfoError instance.
+
+        :param message: the error message
+        :param link: the link to documentation containing more information
+        """
+        super().__init__(message)
+
+        self.link = link
+
+
+class AuthenticationError(MoreInfoError):
+    """An error indicating that a request has failed because the used credentials were invalid."""
+
+    def __init__(self) -> None:
+        """Creates a new AuthenticationError instance."""
+        super().__init__("Invalid credentials, please log in using `lean login`",
+                         "https://www.lean.io/docs/lean-cli/initialization/authenticating-accounts#02-Log-In")
```

### Comparing `ablean-1.3.7/ablean/models/modules.py` & `ablean-1.3.8/ablean/models/modules.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,40 +1,40 @@
-# QUANTCONNECT.COM - Democratizing Finance, Empowering Individuals.
-# Lean CLI v1.0. Copyright 2021 QuantConnect Corporation.
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-
-import re
-
-from ablean.models.pydantic import WrappedBaseModel
-
-
-class NuGetPackage(WrappedBaseModel):
-    name: str
-    version: str
-
-    def get_file_name(self) -> str:
-        """Returns the file name of the package.
-
-        :return: the file name of the NuGet package
-        """
-        return f"{self.name}.{self.version}.nupkg"
-
-    @classmethod
-    def parse(cls, file_name: str) -> 'NuGetPackage':
-        """Parses a file name into a NuGetPackage instance.
-
-        :param file_name: the file name of the NuGet package
-        :return: the NuGetPackage instance containing the name and version of the package with the given file name
-        """
-        name = re.search(r"([^\d]+)\.\d", file_name).group(1)
-        version = file_name.replace(f"{name}.", "").replace(".nupkg", "")
-
-        return NuGetPackage(name=name, version=version)
+# QUANTCONNECT.COM - Democratizing Finance, Empowering Individuals.
+# Lean CLI v1.0. Copyright 2021 QuantConnect Corporation.
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+
+import re
+
+from ablean.models.pydantic import WrappedBaseModel
+
+
+class NuGetPackage(WrappedBaseModel):
+    name: str
+    version: str
+
+    def get_file_name(self) -> str:
+        """Returns the file name of the package.
+
+        :return: the file name of the NuGet package
+        """
+        return f"{self.name}.{self.version}.nupkg"
+
+    @classmethod
+    def parse(cls, file_name: str) -> 'NuGetPackage':
+        """Parses a file name into a NuGetPackage instance.
+
+        :param file_name: the file name of the NuGet package
+        :return: the NuGetPackage instance containing the name and version of the package with the given file name
+        """
+        name = re.search(r"([^\d]+)\.\d", file_name).group(1)
+        version = file_name.replace(f"{name}.", "").replace(".nupkg", "")
+
+        return NuGetPackage(name=name, version=version)
```

### Comparing `ablean-1.3.7/ablean/models/options.py` & `ablean-1.3.8/ablean/models/options.py`

 * *Ordering differences only*

 * *Files 9% similar despite different names*

```diff
@@ -1,99 +1,99 @@
-# QUANTCONNECT.COM - Democratizing Finance, Empowering Individuals.
-# Lean CLI v1.0. Copyright 2021 QuantConnect Corporation.
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-
-from typing import List, Optional
-
-from ablean.components.config.storage import Storage
-
-
-class Option:
-    """An Option instance manages a single value in a Storage instance."""
-
-    def __init__(self, key: str, description: str, is_sensitive: bool, storage: Storage) -> None:
-        """Creates a new StringOption instance.
-
-        :param key: the name of the key of the option in the given Storage instance, using hyphens for separation
-        :param description: a display-friendly description of the option
-        :param is_sensitive: whether the contents of this option may be logged without masking it
-        :param storage: the Storage instance to store this option in
-        """
-        self.key = key
-        self.description = description
-        self.is_sensitive = is_sensitive
-
-        self._storage = storage
-        self.location = storage.file
-
-    def get_value(self, default: Optional[str] = None) -> Optional[str]:
-        """Retrieves the current value of the option.
-
-        :param default: the value to return if the option is not set
-        :return: the current value of the option, or the given default if the option is not set
-        """
-        return self._storage.get(self.key, default)
-
-    def set_value(self, value: str) -> None:
-        """Sets the new value of the option.
-
-        :param value: the non-empty new value of the option
-        """
-        if value == "":
-            raise ValueError("Value cannot be empty")
-
-        self._storage.set(self.key, value)
-
-    def unset(self) -> None:
-        """Unsets any value of the option."""
-        self._storage.delete(self.key)
-
-
-class ChoiceOption(Option):
-    """A variant of Option where only a few values are allowed.
-
-    The allowed values are considered to be case insensitive.
-    """
-
-    def __init__(self,
-                 key: str,
-                 description: str,
-                 allowed_values: List[str],
-                 is_sensitive: bool,
-                 storage: Storage) -> None:
-        """Creates a new ChoiceOption instance.
-
-        :param key: the name of the key of the option in the given file, should use hyphens for separation
-        :param description: a display-friendly description of the option
-        :param allowed_values: the values which can be set
-        :param is_sensitive: whether the contents of this option may be logged without masking it
-        :param storage: the Storage instance to store this option in
-        """
-        self.allowed_values = allowed_values
-
-        if description.endswith("."):
-            description = description[:-1]
-        description = description + f" (allowed values: {', '.join(allowed_values)})."
-
-        super().__init__(key, description, is_sensitive, storage)
-
-    def set_value(self, value: str) -> None:
-        """Sets the new value of the option.
-
-        :param value: the new value of the option, must be one of this option's allowed values
-        """
-        matching_value = next((x for x in self.allowed_values if x.lower() == value.lower()), None)
-
-        if matching_value is None:
-            raise ValueError(
-                f"Invalid value, '{self.key}' only accepts the following values: {', '.join(self.allowed_values)}")
-
-        super().set_value(matching_value)
+# QUANTCONNECT.COM - Democratizing Finance, Empowering Individuals.
+# Lean CLI v1.0. Copyright 2021 QuantConnect Corporation.
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+
+from typing import List, Optional
+
+from ablean.components.config.storage import Storage
+
+
+class Option:
+    """An Option instance manages a single value in a Storage instance."""
+
+    def __init__(self, key: str, description: str, is_sensitive: bool, storage: Storage) -> None:
+        """Creates a new StringOption instance.
+
+        :param key: the name of the key of the option in the given Storage instance, using hyphens for separation
+        :param description: a display-friendly description of the option
+        :param is_sensitive: whether the contents of this option may be logged without masking it
+        :param storage: the Storage instance to store this option in
+        """
+        self.key = key
+        self.description = description
+        self.is_sensitive = is_sensitive
+
+        self._storage = storage
+        self.location = storage.file
+
+    def get_value(self, default: Optional[str] = None) -> Optional[str]:
+        """Retrieves the current value of the option.
+
+        :param default: the value to return if the option is not set
+        :return: the current value of the option, or the given default if the option is not set
+        """
+        return self._storage.get(self.key, default)
+
+    def set_value(self, value: str) -> None:
+        """Sets the new value of the option.
+
+        :param value: the non-empty new value of the option
+        """
+        if value == "":
+            raise ValueError("Value cannot be empty")
+
+        self._storage.set(self.key, value)
+
+    def unset(self) -> None:
+        """Unsets any value of the option."""
+        self._storage.delete(self.key)
+
+
+class ChoiceOption(Option):
+    """A variant of Option where only a few values are allowed.
+
+    The allowed values are considered to be case insensitive.
+    """
+
+    def __init__(self,
+                 key: str,
+                 description: str,
+                 allowed_values: List[str],
+                 is_sensitive: bool,
+                 storage: Storage) -> None:
+        """Creates a new ChoiceOption instance.
+
+        :param key: the name of the key of the option in the given file, should use hyphens for separation
+        :param description: a display-friendly description of the option
+        :param allowed_values: the values which can be set
+        :param is_sensitive: whether the contents of this option may be logged without masking it
+        :param storage: the Storage instance to store this option in
+        """
+        self.allowed_values = allowed_values
+
+        if description.endswith("."):
+            description = description[:-1]
+        description = description + f" (allowed values: {', '.join(allowed_values)})."
+
+        super().__init__(key, description, is_sensitive, storage)
+
+    def set_value(self, value: str) -> None:
+        """Sets the new value of the option.
+
+        :param value: the new value of the option, must be one of this option's allowed values
+        """
+        matching_value = next((x for x in self.allowed_values if x.lower() == value.lower()), None)
+
+        if matching_value is None:
+            raise ValueError(
+                f"Invalid value, '{self.key}' only accepts the following values: {', '.join(self.allowed_values)}")
+
+        super().set_value(matching_value)
```

### Comparing `ablean-1.3.7/ablean/models/pydantic.py` & `ablean-1.3.8/ablean/models/pydantic.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,38 +1,38 @@
-# QUANTCONNECT.COM - Democratizing Finance, Empowering Individuals.
-# Lean CLI v1.0. Copyright 2021 QuantConnect Corporation.
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-
-from typing import Any
-from pydantic import BaseModel, ValidationError
-
-
-class WrappedBaseModel(BaseModel):
-    """A version of Pydantic's BaseModel which makes the input data accessible in case of a validation error."""
-
-    def __init__(self, *args, **kwargs) -> None:
-        """Creates a new WrappedBaseModel instance.
-
-        :param args: args to pass on to the BaseModel constructor
-        :param kwargs: kwargs to pass on to the BaseModel constructor
-        """
-        try:
-            super().__init__(*args, **kwargs)
-        except ValidationError as error:
-            error.input_value = kwargs
-            raise error
-
-
-class Option(WrappedBaseModel):
-    """The Option class represents a choosable option with an internal id and a display-friendly label."""
-
-    id: Any
-    label: str
+# QUANTCONNECT.COM - Democratizing Finance, Empowering Individuals.
+# Lean CLI v1.0. Copyright 2021 QuantConnect Corporation.
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+
+from typing import Any
+from pydantic import BaseModel, ValidationError
+
+
+class WrappedBaseModel(BaseModel):
+    """A version of Pydantic's BaseModel which makes the input data accessible in case of a validation error."""
+
+    def __init__(self, *args, **kwargs) -> None:
+        """Creates a new WrappedBaseModel instance.
+
+        :param args: args to pass on to the BaseModel constructor
+        :param kwargs: kwargs to pass on to the BaseModel constructor
+        """
+        try:
+            super().__init__(*args, **kwargs)
+        except ValidationError as error:
+            error.input_value = kwargs
+            raise error
+
+
+class Option(WrappedBaseModel):
+    """The Option class represents a choosable option with an internal id and a display-friendly label."""
+
+    id: Any
+    label: str
```

### Comparing `ablean-1.3.7/ablean/models/utils.py` & `ablean-1.3.8/ablean/models/utils.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,41 +1,41 @@
-# QUANTCONNECT.COM - Democratizing Finance, Empowering Individuals.
-# Lean CLI v1.0. Copyright 2021 QuantConnect Corporation.
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-
-from enum import Enum
-from ablean.models.pydantic import WrappedBaseModel
-
-
-class DebuggingMethod(Enum):
-    """The debugging methods supported by the CLI."""
-
-    PyCharm = 1
-    PTVSD = 2
-    VSDBG = 3
-    Rider = 4
-
-    def get_internal_name(self) -> str:
-        """Returns the LEAN debugging method that should be used for the current enum member.
-
-        :return: a valid LEAN debugging method that should be used for the current enum member
-        """
-        return {
-            DebuggingMethod.PyCharm: "PyCharm",
-            DebuggingMethod.PTVSD: "PTVSD",
-        }.get(self, "LocalCmdline")
-
-
-class CSharpLibrary(WrappedBaseModel):
-    """The information of a PackageReference tag in a .csproj file."""
-
-    name: str
-    version: str
+# QUANTCONNECT.COM - Democratizing Finance, Empowering Individuals.
+# Lean CLI v1.0. Copyright 2021 QuantConnect Corporation.
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+
+from enum import Enum
+from ablean.models.pydantic import WrappedBaseModel
+
+
+class DebuggingMethod(Enum):
+    """The debugging methods supported by the CLI."""
+
+    PyCharm = 1
+    PTVSD = 2
+    VSDBG = 3
+    Rider = 4
+
+    def get_internal_name(self) -> str:
+        """Returns the LEAN debugging method that should be used for the current enum member.
+
+        :return: a valid LEAN debugging method that should be used for the current enum member
+        """
+        return {
+            DebuggingMethod.PyCharm: "PyCharm",
+            DebuggingMethod.PTVSD: "PTVSD",
+        }.get(self, "LocalCmdline")
+
+
+class CSharpLibrary(WrappedBaseModel):
+    """The information of a PackageReference tag in a .csproj file."""
+
+    name: str
+    version: str
```

### Comparing `ablean-1.3.7/ablean/myclick.py` & `ablean-1.3.8/ablean/myclick.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,251 +1,251 @@
-# QUANTCONNECT.COM - Democratizing Finance, Empowering Individuals.
-# Lean CLI v1.0. Copyright 2021 QuantConnect Corporation.
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-
-import itertools
-import os
-import shutil
-import sys
-from datetime import datetime
-from pathlib import Path
-from typing import Optional, List
-
-import click
-
-from ablean.container import container
-from ablean.constants import DEFAULT_LEAN_CONFIG_FILE_NAME
-from ablean.models.errors import MoreInfoError
-from ablean.models.pydantic import Option
-
-
-class LeanCommand(click.Command):
-    """A click.Command wrapper with some Lean CLI customization."""
-
-    def __init__(
-        self,
-        requires_lean_config: bool = False,
-        allow_unknown_options: bool = False,
-        *args,
-        **kwargs,
-    ):
-        """Creates a new LeanCommand instance.
-
-        :param requires_lean_config: True if this command requires a Lean config, False if not
-        :param allow_unknown_options: True if unknown options are allowed, False if not
-        :param args: the args that are passed on to the click.Command constructor
-        :param kwargs: the kwargs that are passed on to the click.Command constructor
-        """
-        self._requires_lean_config = requires_lean_config
-        self._allow_unknown_options = allow_unknown_options
-
-        super().__init__(*args, **kwargs)
-
-        # By default the width of help messages is min(terminal_width, max_content_width)
-        # max_content_width defaults to 80, which we increase to 120 to improve readability on wide terminals
-        self.context_settings["max_content_width"] = 120
-
-        # Don't fail if unknown options are passed in when they're allowed
-        self.context_settings["ignore_unknown_options"] = allow_unknown_options
-        self.context_settings["allow_extra_args"] = allow_unknown_options
-
-    def invoke(self, ctx: click.Context):
-        if self._requires_lean_config:
-            lean_config_manager = container.lean_config_manager()
-            try:
-                # This method will raise an error if the directory cannot be found
-                lean_config_manager.get_cli_root_directory()
-            except Exception:
-                # Use one of the cached Lean config locations to avoid having to abort the command
-                lean_config_paths = lean_config_manager.get_known_lean_config_paths()
-                if len(lean_config_paths) > 0:
-                    lean_config_path = container.logger().prompt_list(
-                        "Select the Lean configuration file to use",
-                        [Option(id=p, label=str(p)) for p in lean_config_paths],
-                    )
-                    lean_config_manager.set_default_lean_config_path(lean_config_path)
-                else:
-                    # Abort with a display-friendly error message if the command requires a Lean config and none found
-                    raise MoreInfoError(
-                        "This command requires a Lean configuration file, run `lean init` in an empty directory to create one, or specify the file to use with --lean-config",
-                        "https://www.lean.io/docs/lean-cli/key-concepts/troubleshooting#02-Common-Errors",
-                    )
-        if self._allow_unknown_options:
-            # Unknown options are passed to ctx.args and need to be parsed manually
-            # We parse them to ctx.params so they're available like normal options
-            # Because of this all commands with allow_unknown_options=True must have a **kwargs argument
-            arguments = list(itertools.chain(*[arg.split("=") for arg in ctx.args]))
-
-            skip_next = False
-            for index in range(len(arguments) - 1):
-                if skip_next:
-                    skip_next = False
-                    continue
-
-                if arguments[index].startswith("--"):
-                    option = arguments[index].replace("--", "")
-                    value = arguments[index + 1]
-                    ctx.params[option] = value
-                    skip_next = True
-
-        result = super().invoke(ctx)
-        return result
-
-    def get_params(self, ctx: click.Context):
-        params = super().get_params(ctx)
-
-        # Add --lean-config option if the command requires a Lean config
-        if self._requires_lean_config:
-            params.insert(
-                len(params) - 1,
-                click.Option(
-                    ["--lean-config"],
-                    type=PathParameter(exists=True, file_okay=True, dir_okay=False),
-                    help=f"The Lean configuration file that should be used (defaults to the nearest {DEFAULT_LEAN_CONFIG_FILE_NAME})",
-                    expose_value=False,
-                    is_eager=True,
-                    callback=self._parse_config_option,
-                ),
-            )
-
-        # Add --verbose option
-        params.insert(
-            len(params) - 1,
-            click.Option(
-                ["--verbose"],
-                help="Enable debug logging",
-                is_flag=True,
-                default=False,
-                expose_value=False,
-                is_eager=True,
-                callback=self._parse_verbose_option,
-            ),
-        )
-
-        return params
-
-    def _parse_config_option(
-        self, ctx: click.Context, param: click.Parameter, value: Optional[Path]
-    ) -> None:
-        """Parses the --config option."""
-        if value is not None:
-            lean_config_manager = container.lean_config_manager()
-            lean_config_manager.set_default_lean_config_path(value)
-
-    def _parse_verbose_option(
-        self, ctx: click.Context, param: click.Parameter, value: Optional[bool]
-    ) -> None:
-        """Parses the --verbose option."""
-        if value:
-            logger = container.logger()
-            logger.debug_logging_enabled = True
-
-
-class PathParameter(click.ParamType):
-    """A limited version of click.Path which uses pathlib.Path."""
-
-    def __init__(
-        self, exists: bool = False, file_okay: bool = True, dir_okay: bool = True
-    ):
-        """Creates a new PathParameter instance.
-
-        :param exists: True if the path needs to point to an existing object, False if not
-        :param file_okay: True if the path may point to a file, False if not
-        :param dir_okay: True if the path may point to a directory, False if not
-        """
-        self._exists = exists
-        self._file_okay = file_okay
-        self._dir_okay = dir_okay
-
-        if file_okay and not dir_okay:
-            self.name = "file"
-            self._path_type = "File"
-        elif dir_okay and not file_okay:
-            self.name = "directory"
-            self._path_type = "Directory"
-        else:
-            self.name = "path"
-            self._path_type = "Path"
-
-    def convert(self, value: str, param: click.Parameter, ctx: click.Context) -> Path:
-        path = Path(value).expanduser().resolve()
-
-        if not container.path_manager().is_path_valid(path):
-            self.fail(f"{self._path_type} '{value}' is not a valid path.", param, ctx)
-
-        if self._exists and not path.exists():
-            self.fail(f"{self._path_type} '{value}' does not exist.", param, ctx)
-
-        if not self._file_okay and path.is_file():
-            self.fail(f"{self._path_type} '{value}' is a file.", param, ctx)
-
-        if not self._dir_okay and path.is_dir():
-            self.fail(f"{self._path_type} '{value}' is a directory.", param, ctx)
-
-        return path
-
-
-class DateParameter(click.ParamType):
-    """A click parameter which returns datetime.datetime objects and requires yyyyMMdd input."""
-
-    name = "date"
-
-    def get_metavar(self, param: click.Parameter) -> str:
-        return "[yyyyMMdd]"
-
-    def convert(
-        self, value: str, param: click.Parameter, ctx: click.Context
-    ) -> datetime:
-        for date_format in ["%Y%m%d", "%Y-%m-%d"]:
-            try:
-                return datetime.strptime(value, date_format)
-            except ValueError:
-                pass
-
-        self.fail(f"'{value}' does not match the yyyyMMdd format.", param, ctx)
-
-
-def ensure_options(options: List[str]) -> None:
-    """Ensures certain options have values, raises an error if not.
-
-    :param options: the Python names of the options that must have values
-    """
-    ctx = click.get_current_context()
-
-    missing_options = []
-    for key, value in ctx.params.items():
-        has_value = value is not None
-
-        if isinstance(value, tuple) and len(value) == 0:
-            has_value = False
-
-        if not has_value and key in options:
-            missing_options.append(key)
-
-    if len(missing_options) == 0:
-        return
-
-    missing_options = sorted(missing_options, key=lambda param: options.index(param))
-    help_records = []
-
-    for name in missing_options:
-        option = next(param for param in ctx.command.params if param.name == name)
-        help_records.append(option.get_help_record(ctx))
-
-    help_formatter = click.HelpFormatter(max_width=120)
-    help_formatter.write_dl(help_records)
-
-    raise RuntimeError(
-        f"""
-You are missing the following option{"s" if len(missing_options) > 1 else ""}:
-{''.join(help_formatter.buffer)}
-    """.strip()
-    )
+# QUANTCONNECT.COM - Democratizing Finance, Empowering Individuals.
+# Lean CLI v1.0. Copyright 2021 QuantConnect Corporation.
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+
+import itertools
+import os
+import shutil
+import sys
+from datetime import datetime
+from pathlib import Path
+from typing import Optional, List
+
+import click
+
+from ablean.container import container
+from ablean.constants import DEFAULT_LEAN_CONFIG_FILE_NAME
+from ablean.models.errors import MoreInfoError
+from ablean.models.pydantic import Option
+
+
+class LeanCommand(click.Command):
+    """A click.Command wrapper with some Lean CLI customization."""
+
+    def __init__(
+        self,
+        requires_lean_config: bool = False,
+        allow_unknown_options: bool = False,
+        *args,
+        **kwargs,
+    ):
+        """Creates a new LeanCommand instance.
+
+        :param requires_lean_config: True if this command requires a Lean config, False if not
+        :param allow_unknown_options: True if unknown options are allowed, False if not
+        :param args: the args that are passed on to the click.Command constructor
+        :param kwargs: the kwargs that are passed on to the click.Command constructor
+        """
+        self._requires_lean_config = requires_lean_config
+        self._allow_unknown_options = allow_unknown_options
+
+        super().__init__(*args, **kwargs)
+
+        # By default the width of help messages is min(terminal_width, max_content_width)
+        # max_content_width defaults to 80, which we increase to 120 to improve readability on wide terminals
+        self.context_settings["max_content_width"] = 120
+
+        # Don't fail if unknown options are passed in when they're allowed
+        self.context_settings["ignore_unknown_options"] = allow_unknown_options
+        self.context_settings["allow_extra_args"] = allow_unknown_options
+
+    def invoke(self, ctx: click.Context):
+        if self._requires_lean_config:
+            lean_config_manager = container.lean_config_manager()
+            try:
+                # This method will raise an error if the directory cannot be found
+                lean_config_manager.get_cli_root_directory()
+            except Exception:
+                # Use one of the cached Lean config locations to avoid having to abort the command
+                lean_config_paths = lean_config_manager.get_known_lean_config_paths()
+                if len(lean_config_paths) > 0:
+                    lean_config_path = container.logger().prompt_list(
+                        "Select the Lean configuration file to use",
+                        [Option(id=p, label=str(p)) for p in lean_config_paths],
+                    )
+                    lean_config_manager.set_default_lean_config_path(lean_config_path)
+                else:
+                    # Abort with a display-friendly error message if the command requires a Lean config and none found
+                    raise MoreInfoError(
+                        "This command requires a Lean configuration file, run `lean init` in an empty directory to create one, or specify the file to use with --lean-config",
+                        "https://www.lean.io/docs/lean-cli/key-concepts/troubleshooting#02-Common-Errors",
+                    )
+        if self._allow_unknown_options:
+            # Unknown options are passed to ctx.args and need to be parsed manually
+            # We parse them to ctx.params so they're available like normal options
+            # Because of this all commands with allow_unknown_options=True must have a **kwargs argument
+            arguments = list(itertools.chain(*[arg.split("=") for arg in ctx.args]))
+
+            skip_next = False
+            for index in range(len(arguments) - 1):
+                if skip_next:
+                    skip_next = False
+                    continue
+
+                if arguments[index].startswith("--"):
+                    option = arguments[index].replace("--", "")
+                    value = arguments[index + 1]
+                    ctx.params[option] = value
+                    skip_next = True
+
+        result = super().invoke(ctx)
+        return result
+
+    def get_params(self, ctx: click.Context):
+        params = super().get_params(ctx)
+
+        # Add --lean-config option if the command requires a Lean config
+        if self._requires_lean_config:
+            params.insert(
+                len(params) - 1,
+                click.Option(
+                    ["--lean-config"],
+                    type=PathParameter(exists=True, file_okay=True, dir_okay=False),
+                    help=f"The Lean configuration file that should be used (defaults to the nearest {DEFAULT_LEAN_CONFIG_FILE_NAME})",
+                    expose_value=False,
+                    is_eager=True,
+                    callback=self._parse_config_option,
+                ),
+            )
+
+        # Add --verbose option
+        params.insert(
+            len(params) - 1,
+            click.Option(
+                ["--verbose"],
+                help="Enable debug logging",
+                is_flag=True,
+                default=False,
+                expose_value=False,
+                is_eager=True,
+                callback=self._parse_verbose_option,
+            ),
+        )
+
+        return params
+
+    def _parse_config_option(
+        self, ctx: click.Context, param: click.Parameter, value: Optional[Path]
+    ) -> None:
+        """Parses the --config option."""
+        if value is not None:
+            lean_config_manager = container.lean_config_manager()
+            lean_config_manager.set_default_lean_config_path(value)
+
+    def _parse_verbose_option(
+        self, ctx: click.Context, param: click.Parameter, value: Optional[bool]
+    ) -> None:
+        """Parses the --verbose option."""
+        if value:
+            logger = container.logger()
+            logger.debug_logging_enabled = True
+
+
+class PathParameter(click.ParamType):
+    """A limited version of click.Path which uses pathlib.Path."""
+
+    def __init__(
+        self, exists: bool = False, file_okay: bool = True, dir_okay: bool = True
+    ):
+        """Creates a new PathParameter instance.
+
+        :param exists: True if the path needs to point to an existing object, False if not
+        :param file_okay: True if the path may point to a file, False if not
+        :param dir_okay: True if the path may point to a directory, False if not
+        """
+        self._exists = exists
+        self._file_okay = file_okay
+        self._dir_okay = dir_okay
+
+        if file_okay and not dir_okay:
+            self.name = "file"
+            self._path_type = "File"
+        elif dir_okay and not file_okay:
+            self.name = "directory"
+            self._path_type = "Directory"
+        else:
+            self.name = "path"
+            self._path_type = "Path"
+
+    def convert(self, value: str, param: click.Parameter, ctx: click.Context) -> Path:
+        path = Path(value).expanduser().resolve()
+
+        if not container.path_manager().is_path_valid(path):
+            self.fail(f"{self._path_type} '{value}' is not a valid path.", param, ctx)
+
+        if self._exists and not path.exists():
+            self.fail(f"{self._path_type} '{value}' does not exist.", param, ctx)
+
+        if not self._file_okay and path.is_file():
+            self.fail(f"{self._path_type} '{value}' is a file.", param, ctx)
+
+        if not self._dir_okay and path.is_dir():
+            self.fail(f"{self._path_type} '{value}' is a directory.", param, ctx)
+
+        return path
+
+
+class DateParameter(click.ParamType):
+    """A click parameter which returns datetime.datetime objects and requires yyyyMMdd input."""
+
+    name = "date"
+
+    def get_metavar(self, param: click.Parameter) -> str:
+        return "[yyyyMMdd]"
+
+    def convert(
+        self, value: str, param: click.Parameter, ctx: click.Context
+    ) -> datetime:
+        for date_format in ["%Y%m%d", "%Y-%m-%d"]:
+            try:
+                return datetime.strptime(value, date_format)
+            except ValueError:
+                pass
+
+        self.fail(f"'{value}' does not match the yyyyMMdd format.", param, ctx)
+
+
+def ensure_options(options: List[str]) -> None:
+    """Ensures certain options have values, raises an error if not.
+
+    :param options: the Python names of the options that must have values
+    """
+    ctx = click.get_current_context()
+
+    missing_options = []
+    for key, value in ctx.params.items():
+        has_value = value is not None
+
+        if isinstance(value, tuple) and len(value) == 0:
+            has_value = False
+
+        if not has_value and key in options:
+            missing_options.append(key)
+
+    if len(missing_options) == 0:
+        return
+
+    missing_options = sorted(missing_options, key=lambda param: options.index(param))
+    help_records = []
+
+    for name in missing_options:
+        option = next(param for param in ctx.command.params if param.name == name)
+        help_records.append(option.get_help_record(ctx))
+
+    help_formatter = click.HelpFormatter(max_width=120)
+    help_formatter.write_dl(help_records)
+
+    raise RuntimeError(
+        f"""
+You are missing the following option{"s" if len(missing_options) > 1 else ""}:
+{''.join(help_formatter.buffer)}
+    """.strip()
+    )
```

### Comparing `ablean-1.3.7/ablean.egg-info/PKG-INFO` & `ablean-1.3.8/ablean.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,1138 +1,1138 @@
-Metadata-Version: 2.1
-Name: ablean
-Version: 1.3.7
-Summary: A CLI aimed at making it easier to run QuantConnect's LEAN engine locally and in the cloud
-Home-page: https://lean.io/cli
-Author: abl
-Author-email: support@quantconnect.com
-Project-URL: Documentation, https://www.lean.io/docs/lean-cli/key-concepts/getting-started
-Project-URL: Source, https://github.com/QuantConnect/lean-cli
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Financial and Insurance Industry
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Requires-Python: >= 3.8
-Description-Content-Type: text/markdown
-
-![Lean CLI](http://cdn.quantconnect.com.s3.us-east-1.amazonaws.com/i/github/lean-cli-splash.png)
-
-# QuantConnect Lean CLI
- 
-[![Build Status](https://github.com/QuantConnect/lean-cli/workflows/Build/badge.svg)](https://github.com/QuantConnect/lean-cli/actions?query=workflow%3ABuild)
-[![PyPI Version](https://img.shields.io/pypi/v/lean)](https://pypi.org/project/lean/)
-[![Project Status](https://img.shields.io/pypi/status/lean)](https://pypi.org/project/lean/)
-
-The Lean CLI is a cross-platform CLI aimed at making it easier to develop with the LEAN engine locally and in the cloud.
-
-Visit the [documentation website](https://www.lean.io/docs/lean-cli/key-concepts/getting-started) for comprehensive and up-to-date documentation.
-
-## Highlights
-
-- [Project scaffolding](https://www.lean.io/docs/lean-cli/projects/project-management)
-- [Local autocomplete](https://www.lean.io/docs/lean-cli/projects/autocomplete)
-- [Local data downloading](https://www.lean.io/docs/lean-cli/datasets/downloading-quantconnect-data)
-- [Local backtesting](https://www.lean.io/docs/lean-cli/backtesting/deployment#02-Run-Local-Backtests)
-- [Local debugging](https://www.lean.io/docs/lean-cli/backtesting/debugging)
-- [Local research environment](https://www.lean.io/docs/lean-cli/research)
-- [Local optimization](https://www.lean.io/docs/lean-cli/optimization/deployment#02-Run-Local-Optimizations)
-- [Local live trading](https://www.lean.io/docs/lean-cli/live-trading/quantconnect-paper-trading#02-Deploy-Local-Algorithms)
-- [Local backtest report creation](https://www.lean.io/docs/lean-cli/backtesting/report#02-Generate-a-Report)
-- [Cloud synchronization](https://www.lean.io/docs/lean-cli/projects/cloud-synchronization)
-- [Cloud backtesting](https://www.lean.io/docs/lean-cli/backtesting/deployment#03-Run-Cloud-Backtests)
-- [Cloud optimization](https://www.lean.io/docs/lean-cli/optimization/deployment#03-Run-Cloud-Optimizations)
-- [Cloud live trading](https://www.lean.io/docs/lean-cli/live-trading/quantconnect-paper-trading#03-Deploy-Cloud-Algorithms)
-
-## Installation
-
-The CLI can be installed and updated by running `pip install --upgrade lean`.
-
-Note that many commands in the CLI require Docker to run. See [Get Docker](https://docs.docker.com/get-docker/) for instructions on how to install Docker for your operating system.
-
-**Note:** Some Linux users may need to install `tkinter` using the following commands:
-
-``` 
-For Python 3
-
-sudo apt-get install python3-tk
-
-For Python 2.7
-
-sudo apt-get install python-tk
-```
-After installing the CLI, open a terminal in an empty directory and run `lean init`. This command downloads the latest configuration file and sample data from the [QuantConnect/Lean](https://github.com/QuantConnect/Lean) repository. We recommend running all Lean CLI commands in the same directory `lean init` was ran in.
-
-## Usage
-
-The Lean CLI supports multiple workflows. The examples below serve as a starting point, you're free to mix local and cloud features in any way you'd like.
-
-A cloud-focused workflow (local development, cloud execution) with the CLI may look like this:
-1. Open a terminal in the directory you ran `lean init` in.
-2. Run `lean cloud pull` to pull remotely changed files.
-3. Start programming locally and run backtests in the cloud with `lean cloud backtest "Project Name" --open --push` whenever there is something to backtest. The `--open` flag means that the backtest results will be opened in the browser when done, while the `--push` flag means that local changes are pushed to the cloud before running the backtest.
-4. Whenever you want to create a new project, run `lean create-project "Project Name"` and `lean cloud push --project "Project Name"` to create a new project containing some basic code and to push it to the cloud.
-5. When you're finished for the moment, run `lean cloud push` to push all locally changed files to the cloud.
-
-A locally-focused workflow (local development, local execution) with the CLI may look like this:
-1. Open a terminal in the directory you ran `lean init` in.
-2. Run `lean create-project "Project Name"` to create a new project with some basic code to get you started.
-3. Work on your strategy in `./Project Name`.
-4. Run `lean research "Project Name"` to start a Jupyter Lab session to perform research in.
-5. Run `lean backtest "Project Name"` to run a backtest whenever there's something to test. This runs your strategy in a Docker container containing the same packages as the ones used on QuantConnect.com, but with your own data.
-
-## Commands
-
-*Note: the readme only contains the `--help` text of all commands. Visit the [documentation website](https://www.lean.io/docs/lean-cli/key-concepts/getting-started) for more comprehensive documentation.*
-
-<!-- commands start -->
-- [`lean backtest`](#lean-backtest)
-- [`lean build`](#lean-build)
-- [`lean cloud backtest`](#lean-cloud-backtest)
-- [`lean cloud live`](#lean-cloud-live)
-- [`lean cloud optimize`](#lean-cloud-optimize)
-- [`lean cloud pull`](#lean-cloud-pull)
-- [`lean cloud push`](#lean-cloud-push)
-- [`lean cloud status`](#lean-cloud-status)
-- [`lean config get`](#lean-config-get)
-- [`lean config list`](#lean-config-list)
-- [`lean config set`](#lean-config-set)
-- [`lean config unset`](#lean-config-unset)
-- [`lean create-project`](#lean-create-project)
-- [`lean data download`](#lean-data-download)
-- [`lean data generate`](#lean-data-generate)
-- [`lean gui logs`](#lean-gui-logs)
-- [`lean gui restart`](#lean-gui-restart)
-- [`lean gui start`](#lean-gui-start)
-- [`lean gui stop`](#lean-gui-stop)
-- [`lean init`](#lean-init)
-- [`lean library add`](#lean-library-add)
-- [`lean library remove`](#lean-library-remove)
-- [`lean live`](#lean-live)
-- [`lean login`](#lean-login)
-- [`lean logout`](#lean-logout)
-- [`lean logs`](#lean-logs)
-- [`lean optimize`](#lean-optimize)
-- [`lean report`](#lean-report)
-- [`lean research`](#lean-research)
-- [`lean whoami`](#lean-whoami)
-
-### `lean backtest`
-
-Backtest a project locally using Docker.
-
-```
-Usage: lean backtest [OPTIONS] PROJECT
-
-  Backtest a project locally using Docker.
-
-  If PROJECT is a directory, the algorithm in the main.py or Main.cs file inside it will be executed.
-  If PROJECT is a file, the algorithm in the specified file will be executed.
-
-  Go to the following url to learn how to debug backtests locally using the Lean CLI:
-  https://www.lean.io/docs/lean-cli/backtesting/debugging
-
-  By default the official LEAN engine image is used. You can override this using the --image option. Alternatively you
-  can set the default engine image for all commands using `lean config set engine-image <image>`.
-
-Options:
-  --output DIRECTORY              Directory to store results in (defaults to PROJECT/backtests/TIMESTAMP)
-  -d, --detach                    Run the backtest in a detached Docker container and return immediately
-  --debug [pycharm|ptvsd|vsdbg|rider]
-                                  Enable a certain debugging method (see --help for more information)
-  --data-provider [Terminal Link|QuantConnect|Local]
-                                  Update the Lean configuration file to retrieve data from the given provider
-  --download-data                 Update the Lean configuration file to download data from the QuantConnect API, alias
-                                  for --data-provider QuantConnect
-
-  --data-purchase-limit INTEGER   The maximum amount of QCC to spend on downloading data during the backtest when using
-                                  QuantConnect as data provider
-
-  --release                       Compile C# projects in release configuration instead of debug
-  --image TEXT                    The LEAN engine image to use (defaults to quantconnect/lean:latest)
-  --update                        Pull the LEAN engine image before running the backtest
-  --lean-config FILE              The Lean configuration file that should be used (defaults to the nearest lean.json)
-  --verbose                       Enable debug logging
-  --help                          Show this message and exit.
-```
-
-_See code: [lean/commands/backtest.py](https://github.com/QuantConnect/lean-cli/blob/master/lean/commands/backtest.py)_
-
-### `lean build`
-
-Build Docker images of your own version of LEAN and the Alpha Streams SDK.
-
-```
-Usage: lean build [OPTIONS] [ROOT]
-
-  Build Docker images of your own version of LEAN and the Alpha Streams SDK.
-
-  ROOT must point to a directory containing the LEAN repository and the Alpha Streams SDK repository:
-  https://github.com/QuantConnect/Lean & https://github.com/QuantConnect/AlphaStreams
-
-  When ROOT is not given, the current directory is used as root directory.
-
-  This command performs the following actions:
-  1. The lean-cli/foundation:latest image is built from Lean/DockerfileLeanFoundation(ARM).
-  2. LEAN is compiled in a Docker container using the lean-cli/foundation:latest image.
-  3. The Alpha Streams SDK is compiled in a Docker container using the lean-cli/foundation:latest image.
-  4. The lean-cli/engine:latest image is built from Lean/Dockerfile using lean-cli/foundation:latest as base image.
-  5. The lean-cli/research:latest image is built from Lean/DockerfileJupyter using lean-cli/engine:latest as base image.
-  6. The default engine image is set to lean-cli/engine:latest.
-  7. The default research image is set to lean-cli/research:latest.
-
-  When the foundation Dockerfile is the same as the official foundation Dockerfile, quantconnect/lean:foundation is
-  used instead of building a custom foundation image.
-
-Options:
-  --tag TEXT  The tag to apply to custom images (defaults to latest)
-  --verbose   Enable debug logging
-  --help      Show this message and exit.
-```
-
-_See code: [lean/commands/build.py](https://github.com/QuantConnect/lean-cli/blob/master/lean/commands/build.py)_
-
-### `lean cloud backtest`
-
-Backtest a project in the cloud.
-
-```
-Usage: lean cloud backtest [OPTIONS] PROJECT
-
-  Backtest a project in the cloud.
-
-  PROJECT must be the name or id of the project to run a backtest for.
-
-  If the project that has to be backtested has been pulled to the local drive with `lean cloud pull` it is possible to
-  use the --push option to push local modifications to the cloud before running the backtest.
-
-Options:
-  --name TEXT  The name of the backtest (a random one is generated if not specified)
-  --push       Push local modifications to the cloud before running the backtest
-  --open       Automatically open the results in the browser when the backtest is finished
-  --verbose    Enable debug logging
-  --help       Show this message and exit.
-```
-
-_See code: [lean/commands/cloud/backtest.py](https://github.com/QuantConnect/lean-cli/blob/master/lean/commands/cloud/backtest.py)_
-
-### `lean cloud live`
-
-Start live trading for a project in the cloud.
-
-```
-Usage: lean cloud live [OPTIONS] PROJECT
-
-  Start live trading for a project in the cloud.
-
-  PROJECT must be the name or the id of the project to start live trading for.
-
-  By default an interactive wizard is shown letting you configure the deployment. If --brokerage is given the command
-  runs in non-interactive mode. In this mode the CLI does not prompt for input or confirmation. In non-interactive
-  mode the options specific to the given brokerage are required, as well as --node, --auto-restart, --notify-order-
-  events and --notify-insights.
-
-Options:
-  --brokerage [Paper Trading|Interactive Brokers|Tradier|Oanda|Bitfinex|Coinbase Pro|Binance|Zerodha|Samco|Kraken|FTX]
-                                  The brokerage to use
-  --ib-user-name TEXT             Your Interactive Brokers username
-  --ib-account TEXT               Your Interactive Brokers account id
-  --ib-password TEXT              Your Interactive Brokers password
-  --ib-data-feed BOOLEAN          Whether the Interactive Brokers price data feed must be used instead of the
-                                  QuantConnect price data feed
-
-  --tradier-account-id TEXT       Your Tradier account id
-  --tradier-access-token TEXT     Your Tradier access token
-  --tradier-environment [live|paper]
-                                  Whether the developer sandbox should be used
-  --oanda-environment [Practice|Trade]
-                                  The environment to run in, Practice for fxTrade Practice, Trade for fxTrade
-  --oanda-account-id TEXT         Your OANDA account id
-  --oanda-access-token TEXT       Your OANDA API token
-  --bitfinex-api-key TEXT         Your Bitfinex API key
-  --bitfinex-api-secret TEXT      Your Bitfinex API secret
-  --gdax-use-sandbox [live|paper]
-                                  Whether the sandbox should be used
-  --gdax-api-key TEXT             Your Coinbase Pro API key
-  --gdax-api-secret TEXT          Your Coinbase Pro API secret
-  --gdax-passphrase TEXT          Your Coinbase Pro API passphrase
-  --binance-use-testnet [live|paper]
-                                  Whether the testnet should be used
-  --binance-api-key TEXT          Your Binance API key
-  --binance-api-secret TEXT       Your Binance API secret
-  --zerodha-api-key TEXT          Your Kite Connect API key
-  --zerodha-access-token TEXT     Your Kite Connect access token
-  --zerodha-product-type [MIS|CNC|NRML]
-                                  MIS if you are targeting intraday products, CNC if you are targeting delivery
-                                  products, NRML if you are targeting carry forward products
-
-  --zerodha-trading-segment [EQUITY|COMMODITY]
-                                  EQUITY if you are trading equities on NSE or BSE, COMMODITY if you are trading
-                                  commodities on MCX
-
-  --samco-client-id TEXT          Your Samco account Client ID
-  --samco-client-password TEXT    Your Samco account password
-  --samco-year-of-birth TEXT      Your year of birth (YYYY) registered with Samco
-  --samco-product-type [MIS|CNC|NRML]
-                                  MIS if you are targeting intraday products, CNC if you are targeting delivery
-                                  products, NRML if you are targeting carry forward products
-
-  --samco-trading-segment [EQUITY|COMMODITY]
-                                  EQUITY if you are trading equities on NSE or BSE, COMMODITY if you are trading
-                                  commodities on MCX
-
-  --kraken-api-key TEXT           Your Kraken API key
-  --kraken-api-secret TEXT        Your Kraken API secret
-  --kraken-verification-tier [Starter|Intermediate|Pro]
-                                  Your Kraken Verification Tier
-  --ftx-exchange-name [FTX|FTXUS]
-                                  FTX exchange name [FTX, FTXUS]
-  --ftx-api-key TEXT              Your FTX API key
-  --ftxus-api-key TEXT            Your FTX API key
-  --ftx-api-secret TEXT           Your FTX API secret
-  --ftxus-api-secret TEXT         Your FTX API secret
-  --ftx-account-tier [Tier1|Tier2|Tier3|Tier4|Tier5|Tier6]
-                                  Your FTX Account Tier
-  --ftxus-account-tier [Tier1|Tier2|Tier3|Tier4|Tier5|Tier6]
-                                  Your FTX Account Tier
-  --node TEXT                     The name or id of the live node to run on
-  --auto-restart BOOLEAN          Whether automatic algorithm restarting must be enabled
-  --notify-order-events BOOLEAN   Whether notifications must be sent for order events
-  --notify-insights BOOLEAN       Whether notifications must be sent for emitted insights
-  --notify-emails TEXT            A comma-separated list of 'email:subject' pairs configuring email-notifications
-  --notify-webhooks TEXT          A comma-separated list of 'url:HEADER_1=VALUE_1:HEADER_2=VALUE_2:etc' pairs
-                                  configuring webhook-notifications
-
-  --notify-sms TEXT               A comma-separated list of phone numbers configuring SMS-notifications
-  --push                          Push local modifications to the cloud before starting live trading
-  --open                          Automatically open the live results in the browser once the deployment starts
-  --verbose                       Enable debug logging
-  --help                          Show this message and exit.
-```
-
-_See code: [lean/commands/cloud/live.py](https://github.com/QuantConnect/lean-cli/blob/master/lean/commands/cloud/live.py)_
-
-### `lean cloud optimize`
-
-Optimize a project in the cloud.
-
-```
-Usage: lean cloud optimize [OPTIONS] PROJECT
-
-  Optimize a project in the cloud.
-
-  PROJECT must be the name or id of the project to optimize.
-
-  An interactive prompt will be shown to configure the optimizer. If --target is given the command runs in non-
-  interactive mode. In this mode the CLI does not prompt for input and the following options become required:
-  --target, --target-direction, --parameter, --node and --parallel-nodes.
-
-  In non-interactive mode the --parameter option can be provided multiple times to configure multiple parameters:
-  - --parameter <name> <min value> <max value> <step size>
-  - --parameter my-first-parameter 1 10 0.5 --parameter my-second-parameter 20 30 5
-
-  In non-interactive mode the --constraint option can be provided multiple times to configure multiple constraints:
-  - --constraint "<statistic> <operator> <value>"
-  - --constraint "Sharpe Ratio >= 0.5" --constraint "Drawdown < 0.25"
-
-  If the project that has to be optimized has been pulled to the local drive with `lean cloud pull` it is possible to
-  use the --push option to push local modifications to the cloud before running the optimization.
-
-Options:
-  --target TEXT                   The target statistic of the optimization
-  --target-direction [min|max]    Whether the target must be minimized or maximized
-  --parameter <TEXT FLOAT FLOAT FLOAT>...
-                                  The 'parameter min max step' pairs configuring the parameters to optimize
-  --constraint TEXT               The 'statistic operator value' pairs configuring the constraints of the optimization
-  --node [O2-8|O4-12|O8-16]       The node type to run the optimization on
-  --parallel-nodes INTEGER        The number of nodes that may be run in parallel
-  --name TEXT                     The name of the optimization (a random one is generated if not specified)
-  --push                          Push local modifications to the cloud before starting the optimization
-  --verbose                       Enable debug logging
-  --help                          Show this message and exit.
-```
-
-_See code: [lean/commands/cloud/optimize.py](https://github.com/QuantConnect/lean-cli/blob/master/lean/commands/cloud/optimize.py)_
-
-### `lean cloud pull`
-
-Pull projects from QuantConnect to the local drive.
-
-```
-Usage: lean cloud pull [OPTIONS]
-
-  Pull projects from QuantConnect to the local drive.
-
-  This command overrides the content of local files with the content of their respective counterparts in the cloud.
-
-  This command will not delete local files for which there is no counterpart in the cloud.
-
-Options:
-  --project TEXT   Name or id of the project to pull (all cloud projects if not specified)
-  --pull-bootcamp  Pull Boot Camp projects (disabled by default)
-  --verbose        Enable debug logging
-  --help           Show this message and exit.
-```
-
-_See code: [lean/commands/cloud/pull.py](https://github.com/QuantConnect/lean-cli/blob/master/lean/commands/cloud/pull.py)_
-
-### `lean cloud push`
-
-Push local projects to QuantConnect.
-
-```
-Usage: lean cloud push [OPTIONS]
-
-  Push local projects to QuantConnect.
-
-  This command overrides the content of cloud files with the content of their respective local counterparts.
-
-  This command will not delete cloud files which don't have a local counterpart.
-
-Options:
-  --project DIRECTORY  Path to the local project to push (all local projects if not specified)
-  --verbose            Enable debug logging
-  --help               Show this message and exit.
-```
-
-_See code: [lean/commands/cloud/push.py](https://github.com/QuantConnect/lean-cli/blob/master/lean/commands/cloud/push.py)_
-
-### `lean cloud status`
-
-Show the live trading status of a project in the cloud.
-
-```
-Usage: lean cloud status [OPTIONS] PROJECT
-
-  Show the live trading status of a project in the cloud.
-
-  PROJECT must be the name or the id of the project to show the status for.
-
-Options:
-  --verbose  Enable debug logging
-  --help     Show this message and exit.
-```
-
-_See code: [lean/commands/cloud/status.py](https://github.com/QuantConnect/lean-cli/blob/master/lean/commands/cloud/status.py)_
-
-### `lean config get`
-
-Get the current value of a configurable option.
-
-```
-Usage: lean config get [OPTIONS] KEY
-
-  Get the current value of a configurable option.
-
-  Sensitive options like credentials cannot be retrieved this way for security reasons. Please open
-  ~/.lean/credentials if you want to see your currently stored credentials.
-
-  Run `lean config list` to show all available options.
-
-Options:
-  --verbose  Enable debug logging
-  --help     Show this message and exit.
-```
-
-_See code: [lean/commands/config/get.py](https://github.com/QuantConnect/lean-cli/blob/master/lean/commands/config/get.py)_
-
-### `lean config list`
-
-List the configurable options and their current values.
-
-```
-Usage: lean config list [OPTIONS]
-
-  List the configurable options and their current values.
-
-Options:
-  --verbose  Enable debug logging
-  --help     Show this message and exit.
-```
-
-_See code: [lean/commands/config/list.py](https://github.com/QuantConnect/lean-cli/blob/master/lean/commands/config/list.py)_
-
-### `lean config set`
-
-Set a configurable option.
-
-```
-Usage: lean config set [OPTIONS] KEY VALUE
-
-  Set a configurable option.
-
-  Run `lean config list` to show all available options.
-
-Options:
-  --verbose  Enable debug logging
-  --help     Show this message and exit.
-```
-
-_See code: [lean/commands/config/set.py](https://github.com/QuantConnect/lean-cli/blob/master/lean/commands/config/set.py)_
-
-### `lean config unset`
-
-Unset a configurable option.
-
-```
-Usage: lean config unset [OPTIONS] KEY
-
-  Unset a configurable option.
-
-  Run `lean config list` to show all available options.
-
-Options:
-  --verbose  Enable debug logging
-  --help     Show this message and exit.
-```
-
-_See code: [lean/commands/config/unset.py](https://github.com/QuantConnect/lean-cli/blob/master/lean/commands/config/unset.py)_
-
-### `lean create-project`
-
-Create a new project containing starter code.
-
-```
-Usage: lean create-project [OPTIONS] NAME
-
-  Create a new project containing starter code.
-
-  If NAME is a path containing subdirectories those will be created automatically.
-
-  The default language can be set using `lean config set default-language python/csharp`.
-
-Options:
-  -l, --language [python|csharp]  The language of the project to create
-  --verbose                       Enable debug logging
-  --help                          Show this message and exit.
-```
-
-_See code: [lean/commands/create_project.py](https://github.com/QuantConnect/lean-cli/blob/master/lean/commands/create_project.py)_
-
-### `lean data download`
-
-Purchase and download data from QuantConnect Datasets.
-
-```
-Usage: lean data download [OPTIONS]
-
-  Purchase and download data from QuantConnect Datasets.
-
-  An interactive wizard will show to walk you through the process of selecting data, accepting the CLI API Access and
-  Data Agreement and payment. After this wizard the selected data will be downloaded automatically.
-
-  If --dataset is given the command runs in non-interactive mode. In this mode the CLI does not prompt for input or
-  confirmation but only halts when the agreement must be accepted. In non-interactive mode all options specific to the
-  selected dataset as well as --organization are required.
-
-  See the following url for the data that can be purchased and downloaded with this command:
-  https://www.quantconnect.com/datasets
-
-Options:
-  --dataset TEXT       The name of the dataset to download non-interactively
-  --organization TEXT  The name or id of the organization to purchase and download data with
-  --overwrite          Overwrite existing local data
-  --lean-config FILE   The Lean configuration file that should be used (defaults to the nearest lean.json)
-  --verbose            Enable debug logging
-  --help               Show this message and exit.
-```
-
-_See code: [lean/commands/data/download.py](https://github.com/QuantConnect/lean-cli/blob/master/lean/commands/data/download.py)_
-
-### `lean data generate`
-
-Generate random market data.
-
-```
-Usage: lean data generate [OPTIONS]
-
-  Generate random market data.
-
-  This uses the random data generator in LEAN to generate realistic market data using a Brownian motion model.
-  This generator supports the following security types, tick types and resolutions:
-  | Security type | Generated tick types | Supported resolutions                |
-  | ------------- | -------------------- | ------------------------------------ |
-  | Equity        | Trade                | Tick, Second, Minute, Hour and Daily |
-  | Forex         | Quote                | Tick, Second, Minute, Hour and Daily |
-  | CFD           | Quote                | Tick, Second, Minute, Hour and Daily |
-  | Future        | Trade and Quote      | Tick, Second, Minute, Hour and Daily |
-  | Crypto        | Trade and Quote      | Tick, Second, Minute, Hour and Daily |
-  | Option        | Trade and Quote      | Minute                               |
-
-  The following data densities are available:
-  - Dense: at least one data point per resolution step.
-  - Sparse: at least one data point per 5 resolution steps.
-  - VerySparse: at least one data point per 50 resolution steps.
-
-  Example which generates minute data for 100 equity symbols since 2015-01-01:
-  $ lean data generate --start=20150101 --symbol-count=100
-
-  Example which generates daily data for 100 crypto symbols since 2015-01-01:
-  $ lean data generate --start=20150101 --symbol-count=100 --security-type=Crypto --resolution=Daily
-
-  By default the official LEAN engine image is used. You can override this using the --image option. Alternatively you
-  can set the default engine image for all commands using `lean config set engine-image <image>`.
-
-Options:
-  --start [yyyyMMdd]              Start date for the data to generate in yyyyMMdd format  [required]
-  --end [yyyyMMdd]                End date for the data to generate in yyyyMMdd format (defaults to today)
-  --symbol-count INTEGER RANGE    The number of symbols to generate data for  [required]
-  --security-type [Equity|Forex|Cfd|Future|Crypto|Option]
-                                  The security type to generate data for (defaults to Equity)
-  --resolution [Tick|Second|Minute|Hour|Daily]
-                                  The resolution of the generated data (defaults to Minute)
-  --data-density [Dense|Sparse|VerySparse]
-                                  The density of the generated data (defaults to Dense)
-  --include-coarse BOOLEAN        Whether coarse universe data should be generated for Equity data (defaults to True)
-  --market TEXT                   The market to generate data for (defaults to standard market for the security type)
-  --image TEXT                    The LEAN engine image to use (defaults to quantconnect/lean:latest)
-  --update                        Pull the LEAN engine image before running the generator
-  --lean-config FILE              The Lean configuration file that should be used (defaults to the nearest lean.json)
-  --verbose                       Enable debug logging
-  --help                          Show this message and exit.
-```
-
-_See code: [lean/commands/data/generate.py](https://github.com/QuantConnect/lean-cli/blob/master/lean/commands/data/generate.py)_
-
-### `lean gui logs`
-
-See the logs of the local GUI.
-
-```
-Usage: lean gui logs [OPTIONS]
-
-  See the logs of the local GUI.
-
-Options:
-  -f, --follow  Update the logs in real-time while the GUI is running
-  --verbose     Enable debug logging
-  --help        Show this message and exit.
-```
-
-_See code: [lean/commands/gui/logs.py](https://github.com/QuantConnect/lean-cli/blob/master/lean/commands/gui/logs.py)_
-
-### `lean gui restart`
-
-Restart the local GUI and open it in the browser.
-
-```
-Usage: lean gui restart [OPTIONS]
-
-  Restart the local GUI and open it in the browser.
-
-Options:
-  --no-open  Skip opening the local GUI in the browser after restarting it
-  --verbose  Enable debug logging
-  --help     Show this message and exit.
-```
-
-_See code: [lean/commands/gui/restart.py](https://github.com/QuantConnect/lean-cli/blob/master/lean/commands/gui/restart.py)_
-
-### `lean gui start`
-
-Start the local GUI.
-
-```
-Usage: lean gui start [OPTIONS]
-
-  Start the local GUI.
-
-Options:
-  --organization TEXT  The name or id of the organization with the local GUI module subscription
-  --port INTEGER       The port to run the local GUI on (defaults to 5612)
-  --no-open            Skip opening the local GUI in the browser after starting it
-  --shortcut           Create a desktop shortcut for launching the local GUI
-  --lean-config FILE   The Lean configuration file that should be used (defaults to the nearest lean.json)
-  --verbose            Enable debug logging
-  --help               Show this message and exit.
-```
-
-_See code: [lean/commands/gui/start.py](https://github.com/QuantConnect/lean-cli/blob/master/lean/commands/gui/start.py)_
-
-### `lean gui stop`
-
-Stop the local GUI.
-
-```
-Usage: lean gui stop [OPTIONS]
-
-  Stop the local GUI.
-
-Options:
-  --verbose  Enable debug logging
-  --help     Show this message and exit.
-```
-
-_See code: [lean/commands/gui/stop.py](https://github.com/QuantConnect/lean-cli/blob/master/lean/commands/gui/stop.py)_
-
-### `lean init`
-
-Scaffold a Lean configuration file and data directory.
-
-```
-Usage: lean init [OPTIONS]
-
-  Scaffold a Lean configuration file and data directory.
-
-Options:
-  --verbose  Enable debug logging
-  --help     Show this message and exit.
-```
-
-_See code: [lean/commands/init.py](https://github.com/QuantConnect/lean-cli/blob/master/lean/commands/init.py)_
-
-### `lean library add`
-
-Add a custom library to a project.
-
-```
-Usage: lean library add [OPTIONS] PROJECT NAME
-
-  Add a custom library to a project.
-
-  PROJECT must be the path to the project.
-
-  NAME must be the name of a NuGet package (for C# projects) or of a PyPI package (for Python projects).
-
-  If --version is not given, the package is pinned to the latest compatible version. For C# projects, this is the
-  latest available version. For Python projects, this is the latest version compatible with Python 3.6 (which is what
-  the Docker images use).
-
-  Custom C# libraries are added to your project's .csproj file, which is then restored if dotnet is on your PATH and
-  the --no-local flag has not been given.
-
-  Custom Python libraries are added to your project's requirements.txt file and are installed in your local Python
-  environment so you get local autocomplete for the library. The last step can be skipped with the --no-local flag.
-
-  C# example usage:
-  $ lean library add "My CSharp Project" Microsoft.ML
-  $ lean library add "My CSharp Project" Microsoft.ML --version 1.5.5
-
-  Python example usage:
-  $ lean library add "My Python Project" tensorflow
-  $ lean library add "My Python Project" tensorflow --version 2.5.0
-
-Options:
-  --version TEXT  The version of the library to add (defaults to latest compatible version)
-  --no-local      Skip making changes to your local environment
-  --verbose       Enable debug logging
-  --help          Show this message and exit.
-```
-
-_See code: [lean/commands/library/add.py](https://github.com/QuantConnect/lean-cli/blob/master/lean/commands/library/add.py)_
-
-### `lean library remove`
-
-Remove a custom library from a project.
-
-```
-Usage: lean library remove [OPTIONS] PROJECT NAME
-
-  Remove a custom library from a project.
-
-  PROJECT must be the path to the project directory.
-
-  NAME must be the name of the NuGet package (for C# projects) or of the PyPI package (for Python projects) to remove.
-
-  Custom C# libraries are removed from the project's .csproj file, which is then restored if dotnet is on your PATH
-  and the --no-local flag has not been given.
-
-  Custom Python libraries are removed from the project's requirements.txt file.
-
-  C# example usage:
-  $ lean library remove "My CSharp Project" Microsoft.ML
-
-  Python example usage:
-  $ lean library remove "My Python Project" tensorflow
-
-Options:
-  --no-local  Skip making changes to your local environment
-  --verbose   Enable debug logging
-  --help      Show this message and exit.
-```
-
-_See code: [lean/commands/library/remove.py](https://github.com/QuantConnect/lean-cli/blob/master/lean/commands/library/remove.py)_
-
-### `lean live`
-
-Start live trading a project locally using Docker.
-
-```
-Usage: lean live [OPTIONS] PROJECT
-
-  Start live trading a project locally using Docker.
-
-  If PROJECT is a directory, the algorithm in the main.py or Main.cs file inside it will be executed.
-  If PROJECT is a file, the algorithm in the specified file will be executed.
-
-  By default an interactive wizard is shown letting you configure the brokerage and data feed to use. If
-  --environment, --brokerage or --data-feed are given the command runs in non-interactive mode. In this mode the CLI
-  does not prompt for input.
-
-  If --environment is given it must be the name of a live environment in the Lean configuration.
-
-  If --brokerage and --data-feed are given, the options specific to the given brokerage/data feed must also be given.
-  The Lean config is used as fallback when a brokerage/data feed-specific option hasn't been passed in. If a required
-  option is not given and cannot be found in the Lean config the command aborts.
-
-  By default the official LEAN engine image is used. You can override this using the --image option. Alternatively you
-  can set the default engine image for all commands using `lean config set engine-image <image>`.
-
-Options:
-  --environment TEXT              The environment to use
-  --output DIRECTORY              Directory to store results in (defaults to PROJECT/live/TIMESTAMP)
-  -d, --detach                    Run the live deployment in a detached Docker container and return immediately
-  --gui                           Enable monitoring and controlling of the deployment via the local GUI
-  --gui-organization TEXT         The name or id of the organization with the local GUI module subscription
-  --brokerage [Paper Trading|Interactive Brokers|Tradier|Oanda|Bitfinex|Coinbase Pro|Binance|Zerodha|Samco|Terminal Link|Atreyu|Trading Technologies|Kraken|FTX]
-                                  The brokerage to use
-  --data-feed [Interactive Brokers|Tradier|Oanda|Bitfinex|Coinbase Pro|Binance|Zerodha|Samco|Terminal Link|Trading Technologies|Kraken|FTX|IQFeed|Custom data only]
-                                  The data feed to use
-  --ib-organization TEXT          The name or id of the organization with the Interactive Brokers module subscription
-  --ib-user-name TEXT             Your Interactive Brokers username
-  --ib-account TEXT               Your Interactive Brokers account id
-  --ib-password TEXT              Your Interactive Brokers password
-  --ib-enable-delayed-streaming-data BOOLEAN
-                                  Whether delayed data may be used when your algorithm subscribes to a security you
-                                  don't have a market data subscription for
-
-  --tradier-account-id TEXT       Your Tradier account id
-  --tradier-access-token TEXT     Your Tradier access token
-  --tradier-environment [live|paper]
-                                  Whether the developer sandbox should be used
-  --oanda-environment [Practice|Trade]
-                                  The environment to run in, Practice for fxTrade Practice, Trade for fxTrade
-  --oanda-account-id TEXT         Your OANDA account id
-  --oanda-access-token TEXT       Your OANDA API token
-  --bitfinex-api-key TEXT         Your Bitfinex API key
-  --bitfinex-api-secret TEXT      Your Bitfinex API secret
-  --gdax-use-sandbox [live|paper]
-                                  Whether the sandbox should be used
-  --gdax-api-key TEXT             Your Coinbase Pro API key
-  --gdax-api-secret TEXT          Your Coinbase Pro API secret
-  --gdax-passphrase TEXT          Your Coinbase Pro API passphrase
-  --binance-use-testnet [live|paper]
-                                  Whether the testnet should be used
-  --binance-organization TEXT     The name or id of the organization with the Binance module subscription
-  --binance-api-key TEXT          Your Binance API key
-  --binance-api-secret TEXT       Your Binance API secret
-  --zerodha-organization TEXT     The name or id of the organization with the zerodha module subscription
-  --zerodha-api-key TEXT          Your Kite Connect API key
-  --zerodha-access-token TEXT     Your Kite Connect access token
-  --zerodha-product-type [MIS|CNC|NRML]
-                                  MIS if you are targeting intraday products, CNC if you are targeting delivery
-                                  products, NRML if you are targeting carry forward products
-
-  --zerodha-trading-segment [EQUITY|COMMODITY]
-                                  EQUITY if you are trading equities on NSE or BSE, COMMODITY if you are trading
-                                  commodities on MCX
-
-  --zerodha-history-subscription BOOLEAN
-                                  Whether you have a history API subscription for Zerodha
-  --samco-organization TEXT       The name or id of the organization with the samco module subscription
-  --samco-client-id TEXT          Your Samco account Client ID
-  --samco-client-password TEXT    Your Samco account password
-  --samco-year-of-birth TEXT      Your year of birth (YYYY) registered with Samco
-  --samco-product-type [MIS|CNC|NRML]
-                                  MIS if you are targeting intraday products, CNC if you are targeting delivery
-                                  products, NRML if you are targeting carry forward products
-
-  --samco-trading-segment [EQUITY|COMMODITY]
-                                  EQUITY if you are trading equities on NSE or BSE, COMMODITY if you are trading
-                                  commodities on MCX
-
-  --terminal-link-organization TEXT
-                                  The name or id of the organization with the Terminal Link module subscription
-  --bloomberg-environment [Production|Beta]
-                                  The environment to run in
-  --bloomberg-server-host TEXT    The host of the Bloomberg server
-  --bloomberg-server-port INTEGER
-                                  The port of the Bloomberg server
-  --bloomberg-symbol-map-file FILE
-                                  The path to the Bloomberg symbol map file
-  --bloomberg-emsx-broker TEXT    The EMSX broker to use
-  --bloomberg-emsx-user-time-zone TEXT
-                                  The EMSX user timezone to use
-  --bloomberg-emsx-account TEXT   The EMSX account to use
-  --bloomberg-emsx-strategy TEXT  The EMSX strategy to use
-  --bloomberg-emsx-notes TEXT     The EMSX notes to use
-  --bloomberg-emsx-handling TEXT  The EMSX handling to use
-  --bloomberg-allow-modification BOOLEAN
-                                  Whether modification is allowed
-  --atreyu-organization TEXT      The name or id of the organization with the Atreyu module subscription
-  --atreyu-host TEXT              The host of the Atreyu server
-  --atreyu-req-port INTEGER       The Atreyu request port
-  --atreyu-sub-port INTEGER       The Atreyu subscribe port
-  --atreyu-username TEXT          Your Atreyu username
-  --atreyu-password TEXT          Your Atreyu password
-  --atreyu-client-id TEXT         Your Atreyu client id
-  --atreyu-broker-mpid TEXT       The broker MPID to use
-  --atreyu-locate-rqd TEXT        The locate rqd to use
-  --tt-organization TEXT          The name or id of the organization with the Trading Technologies module subscription
-  --tt-user-name TEXT             Your Trading Technologies username
-  --tt-session-password TEXT      Your Trading Technologies session password
-  --tt-account-name TEXT          Your Trading Technologies account name
-  --tt-rest-app-key TEXT          Your Trading Technologies REST app key
-  --tt-rest-app-secret TEXT       Your Trading Technologies REST app secret
-  --tt-rest-environment TEXT      The REST environment to run in
-  --tt-market-data-sender-comp-id TEXT
-                                  The market data sender comp id to use
-  --tt-market-data-target-comp-id TEXT
-                                  The market data target comp id to use
-  --tt-market-data-host TEXT      The host of the market data server
-  --tt-market-data-port TEXT      The port of the market data server
-  --tt-order-routing-sender-comp-id TEXT
-                                  The order routing sender comp id to use
-  --tt-order-routing-target-comp-id TEXT
-                                  The order routing target comp id to use
-  --tt-order-routing-host TEXT    The host of the order routing server
-  --tt-order-routing-port TEXT    The port of the order routing server
-  --tt-log-fix-messages BOOLEAN   Whether FIX messages should be logged
-  --kraken-organization TEXT      The name or id of the organization with the kraken module subscription
-  --kraken-api-key TEXT           Your Kraken API key
-  --kraken-api-secret TEXT        Your Kraken API secret
-  --kraken-verification-tier [Starter|Intermediate|Pro]
-                                  Your Kraken Verification Tier
-  --ftx-exchange-name [FTX|FTXUS]
-                                  FTX exchange name [FTX, FTXUS]
-  --ftx-organization TEXT         The name or id of the organization with the FTX module subscription
-  --ftx-api-key TEXT              Your FTX API key
-  --ftxus-api-key TEXT            Your FTX API key
-  --ftx-api-secret TEXT           Your FTX API secret
-  --ftxus-api-secret TEXT         Your FTX API secret
-  --ftx-account-tier [Tier1|Tier2|Tier3|Tier4|Tier5|Tier6]
-                                  Your FTX Account Tier
-  --ftxus-account-tier [Tier1|Tier2|Tier3|Tier4|Tier5|Tier6]
-                                  Your FTX Account Tier
-  --iqfeed-iqconnect FILE         The path to the IQConnect binary
-  --iqfeed-username TEXT          Your IQFeed username
-  --iqfeed-password TEXT          Your IQFeed password
-  --iqfeed-productName TEXT       The product name of your IQFeed developer account
-  --iqfeed-version TEXT           The product version of your IQFeed developer account
-  --release                       Compile C# projects in release configuration instead of debug
-  --image TEXT                    The LEAN engine image to use (defaults to quantconnect/lean:latest)
-  --update                        Pull the LEAN engine image before starting live trading
-  --lean-config FILE              The Lean configuration file that should be used (defaults to the nearest lean.json)
-  --verbose                       Enable debug logging
-  --help                          Show this message and exit.
-```
-
-_See code: [lean/commands/live.py](https://github.com/QuantConnect/lean-cli/blob/master/lean/commands/live.py)_
-
-### `lean login`
-
-Log in with a QuantConnect account.
-
-```
-Usage: lean login [OPTIONS]
-
-  Log in with a QuantConnect account.
-
-  If user id or API token is not provided an interactive prompt will show.
-
-  Credentials are stored in ~/.lean/credentials and are removed upon running `lean logout`.
-
-Options:
-  -u, --user-id TEXT    QuantConnect user id
-  -t, --api-token TEXT  QuantConnect API token
-  --verbose             Enable debug logging
-  --help                Show this message and exit.
-```
-
-_See code: [lean/commands/login.py](https://github.com/QuantConnect/lean-cli/blob/master/lean/commands/login.py)_
-
-### `lean logout`
-
-Log out and remove stored credentials.
-
-```
-Usage: lean logout [OPTIONS]
-
-  Log out and remove stored credentials.
-
-Options:
-  --verbose  Enable debug logging
-  --help     Show this message and exit.
-```
-
-_See code: [lean/commands/logout.py](https://github.com/QuantConnect/lean-cli/blob/master/lean/commands/logout.py)_
-
-### `lean logs`
-
-Display the most recent backtest/live/optimization logs.
-
-```
-Usage: lean logs [OPTIONS]
-
-  Display the most recent backtest/live/optimization logs.
-
-Options:
-  --backtest           Display the most recent backtest logs (default)
-  --live               Display the most recent live logs
-  --optimization       Display the most recent optimization logs
-  --project DIRECTORY  The project to get the most recent logs from
-  --lean-config FILE   The Lean configuration file that should be used (defaults to the nearest lean.json)
-  --verbose            Enable debug logging
-  --help               Show this message and exit.
-```
-
-_See code: [lean/commands/logs.py](https://github.com/QuantConnect/lean-cli/blob/master/lean/commands/logs.py)_
-
-### `lean optimize`
-
-Optimize a project's parameters locally using Docker.
-
-```
-Usage: lean optimize [OPTIONS] PROJECT
-
-  Optimize a project's parameters locally using Docker.
-
-  If PROJECT is a directory, the algorithm in the main.py or Main.cs file inside it will be executed.
-  If PROJECT is a file, the algorithm in the specified file will be executed.
-
-  By default an interactive wizard is shown letting you configure the optimizer. If --optimizer-config or --strategy
-  is given the command runs in non-interactive mode. In this mode the CLI does not prompt for input.
-
-  The --optimizer-config option can be used to specify the configuration to run the optimizer with.
-  When using the option it should point to a file like this (the algorithm-* properties should be omitted):
-  https://github.com/QuantConnect/Lean/blob/master/Optimizer.Launcher/config.json
-
-  If --strategy is given the optimizer configuration is read from the given options. In this case --strategy,
-  --target, --target-direction and --parameter become required.
-
-  In non-interactive mode the --parameter option can be provided multiple times to configure multiple parameters:
-  - --parameter <name> <min value> <max value> <step size>
-  - --parameter my-first-parameter 1 10 0.5 --parameter my-second-parameter 20 30 5
-
-  In non-interactive mode the --constraint option can be provided multiple times to configure multiple constraints:
-  - --constraint "<statistic> <operator> <value>"
-  - --constraint "Sharpe Ratio >= 0.5" --constraint "Drawdown < 0.25"
-
-  By default the official LEAN engine image is used. You can override this using the --image option. Alternatively you
-  can set the default engine image for all commands using `lean config set engine-image <image>`.
-
-Options:
-  --output DIRECTORY              Directory to store results in (defaults to PROJECT/optimizations/TIMESTAMP)
-  -d, --detach                    Run the optimization in a detached Docker container and return immediately
-  --optimizer-config FILE         The optimizer configuration file that should be used
-  --strategy [Grid Search|Euler Search]
-                                  The optimization strategy to use
-  --target TEXT                   The target statistic of the optimization
-  --target-direction [min|max]    Whether the target must be minimized or maximized
-  --parameter <TEXT FLOAT FLOAT FLOAT>...
-                                  The 'parameter min max step' pairs configuring the parameters to optimize
-  --constraint TEXT               The 'statistic operator value' pairs configuring the constraints of the optimization
-  --release                       Compile C# projects in release configuration instead of debug
-  --image TEXT                    The LEAN engine image to use (defaults to quantconnect/lean:latest)
-  --update                        Pull the LEAN engine image before running the optimizer
-  --lean-config FILE              The Lean configuration file that should be used (defaults to the nearest lean.json)
-  --verbose                       Enable debug logging
-  --help                          Show this message and exit.
-```
-
-_See code: [lean/commands/optimize.py](https://github.com/QuantConnect/lean-cli/blob/master/lean/commands/optimize.py)_
-
-### `lean report`
-
-Generate a report of a backtest.
-
-```
-Usage: lean report [OPTIONS]
-
-  Generate a report of a backtest.
-
-  This runs the LEAN Report Creator in Docker to generate a polished, professional-grade report of a backtest.
-
-  If --backtest-results is not given, a report is generated for the most recent local backtest.
-
-  The name, description, and version are optional and will be blank if not given.
-
-  If the given backtest data source file is stored in a project directory (or one of its subdirectories, like the
-  default <project>/backtests/<timestamp>), the default name is the name of the project directory and the default
-  description is the description stored in the project's config.json file.
-
-  By default the official LEAN engine image is used. You can override this using the --image option. Alternatively you
-  can set the default engine image for all commands using `lean config set engine-image <image>`.
-
-Options:
-  --backtest-results FILE      Path to the JSON file containing the backtest results
-  --live-results FILE          Path to the JSON file containing the live trading results
-  --report-destination FILE    Path where the generated report is stored as HTML (defaults to ./report.html)
-  -d, --detach                 Run the report creator in a detached Docker container and return immediately
-  --strategy-name TEXT         Name of the strategy, will appear at the top-right corner of each page
-  --strategy-version TEXT      Version number of the strategy, will appear next to the project name
-  --strategy-description TEXT  Description of the strategy, will appear under the 'Strategy Description' section
-  --overwrite                  Overwrite --report-destination if it already contains a file
-  --image TEXT                 The LEAN engine image to use (defaults to quantconnect/lean:latest)
-  --update                     Pull the LEAN engine image before running the report creator
-  --lean-config FILE           The Lean configuration file that should be used (defaults to the nearest lean.json)
-  --verbose                    Enable debug logging
-  --help                       Show this message and exit.
-```
-
-_See code: [lean/commands/report.py](https://github.com/QuantConnect/lean-cli/blob/master/lean/commands/report.py)_
-
-### `lean research`
-
-Run a Jupyter Lab environment locally using Docker.
-
-```
-Usage: lean research [OPTIONS] PROJECT
-
-  Run a Jupyter Lab environment locally using Docker.
-
-  By default the official LEAN research image is used. You can override this using the --image option. Alternatively
-  you can set the default research image using `lean config set research-image <image>`.
-
-Options:
-  --port INTEGER                  The port to run Jupyter Lab on (defaults to 8888)
-  --data-provider [Terminal Link|QuantConnect|Local]
-                                  Update the Lean configuration file to retrieve data from the given provider
-  --download-data                 Update the Lean configuration file to download data from the QuantConnect API, alias
-                                  for --data-provider QuantConnect
-
-  --data-purchase-limit INTEGER   The maximum amount of QCC to spend on downloading data during the research session
-                                  when using QuantConnect as data provider
-
-  -d, --detach                    Run Jupyter Lab in a detached Docker container and return immediately
-  --no-open                       Don't open the Jupyter Lab environment in the browser after starting it
-  --image TEXT                    The LEAN research image to use (defaults to quantconnect/research:latest)
-  --update                        Pull the LEAN research image before starting the research environment
-  --lean-config FILE              The Lean configuration file that should be used (defaults to the nearest lean.json)
-  --verbose                       Enable debug logging
-  --help                          Show this message and exit.
-```
-
-_See code: [lean/commands/research.py](https://github.com/QuantConnect/lean-cli/blob/master/lean/commands/research.py)_
-
-### `lean whoami`
-
-Display who is logged in.
-
-```
-Usage: lean whoami [OPTIONS]
-
-  Display who is logged in.
-
-Options:
-  --verbose  Enable debug logging
-  --help     Show this message and exit.
-```
-
-_See code: [lean/commands/whoami.py](https://github.com/QuantConnect/lean-cli/blob/master/lean/commands/whoami.py)_
-<!-- commands end -->
-
-## Development
-
-To work on the Lean CLI, clone the repository, enter an environment containing Python 3.6+ and run `pip install -r requirements.txt`. This command will install the required dependencies and installs the CLI in editable mode. This means you'll be able to edit the code and immediately see the results the next time you run `lean`.
-
-If you need to add dependencies, first update `setup.py` (if it is a production dependency) or `requirements.txt` (if it is a development dependency) and then re-run `pip install -r requirements.txt`.
-
-The automated tests can be ran by running `pytest`. The filesystem and HTTP requests are mocked when running tests to make sure they run in an isolated environment.
-
-Can build the lean CLI by running `python setup.py sdist bdist_wheel` from the root of the project and to install it `pip install --force-reinstall dist/lean-dev-py3-none-any.whl`. To update the commands reference part of the readme run `python scripts/readme.py` from the root of the project, after installing the new version.
-
-Maintainers can publish new releases by pushing a Git tag containing the new version to GitHub. This will trigger a GitHub Actions workflow which releases the current `master` branch to PyPI with the value of the tag as version. Make sure the version is not prefixed with "v".
+Metadata-Version: 2.1
+Name: ablean
+Version: 1.3.8
+Summary: A CLI aimed at making it easier to run QuantConnect's LEAN engine locally and in the cloud
+Home-page: https://lean.io/cli
+Author: abl
+Author-email: support@quantconnect.com
+Project-URL: Documentation, https://www.lean.io/docs/lean-cli/key-concepts/getting-started
+Project-URL: Source, https://github.com/QuantConnect/lean-cli
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Financial and Insurance Industry
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Requires-Python: >= 3.8
+Description-Content-Type: text/markdown
+
+![Lean CLI](http://cdn.quantconnect.com.s3.us-east-1.amazonaws.com/i/github/lean-cli-splash.png)
+
+# QuantConnect Lean CLI
+ 
+[![Build Status](https://github.com/QuantConnect/lean-cli/workflows/Build/badge.svg)](https://github.com/QuantConnect/lean-cli/actions?query=workflow%3ABuild)
+[![PyPI Version](https://img.shields.io/pypi/v/lean)](https://pypi.org/project/lean/)
+[![Project Status](https://img.shields.io/pypi/status/lean)](https://pypi.org/project/lean/)
+
+The Lean CLI is a cross-platform CLI aimed at making it easier to develop with the LEAN engine locally and in the cloud.
+
+Visit the [documentation website](https://www.lean.io/docs/lean-cli/key-concepts/getting-started) for comprehensive and up-to-date documentation.
+
+## Highlights
+
+- [Project scaffolding](https://www.lean.io/docs/lean-cli/projects/project-management)
+- [Local autocomplete](https://www.lean.io/docs/lean-cli/projects/autocomplete)
+- [Local data downloading](https://www.lean.io/docs/lean-cli/datasets/downloading-quantconnect-data)
+- [Local backtesting](https://www.lean.io/docs/lean-cli/backtesting/deployment#02-Run-Local-Backtests)
+- [Local debugging](https://www.lean.io/docs/lean-cli/backtesting/debugging)
+- [Local research environment](https://www.lean.io/docs/lean-cli/research)
+- [Local optimization](https://www.lean.io/docs/lean-cli/optimization/deployment#02-Run-Local-Optimizations)
+- [Local live trading](https://www.lean.io/docs/lean-cli/live-trading/quantconnect-paper-trading#02-Deploy-Local-Algorithms)
+- [Local backtest report creation](https://www.lean.io/docs/lean-cli/backtesting/report#02-Generate-a-Report)
+- [Cloud synchronization](https://www.lean.io/docs/lean-cli/projects/cloud-synchronization)
+- [Cloud backtesting](https://www.lean.io/docs/lean-cli/backtesting/deployment#03-Run-Cloud-Backtests)
+- [Cloud optimization](https://www.lean.io/docs/lean-cli/optimization/deployment#03-Run-Cloud-Optimizations)
+- [Cloud live trading](https://www.lean.io/docs/lean-cli/live-trading/quantconnect-paper-trading#03-Deploy-Cloud-Algorithms)
+
+## Installation
+
+The CLI can be installed and updated by running `pip install --upgrade lean`.
+
+Note that many commands in the CLI require Docker to run. See [Get Docker](https://docs.docker.com/get-docker/) for instructions on how to install Docker for your operating system.
+
+**Note:** Some Linux users may need to install `tkinter` using the following commands:
+
+``` 
+For Python 3
+
+sudo apt-get install python3-tk
+
+For Python 2.7
+
+sudo apt-get install python-tk
+```
+After installing the CLI, open a terminal in an empty directory and run `lean init`. This command downloads the latest configuration file and sample data from the [QuantConnect/Lean](https://github.com/QuantConnect/Lean) repository. We recommend running all Lean CLI commands in the same directory `lean init` was ran in.
+
+## Usage
+
+The Lean CLI supports multiple workflows. The examples below serve as a starting point, you're free to mix local and cloud features in any way you'd like.
+
+A cloud-focused workflow (local development, cloud execution) with the CLI may look like this:
+1. Open a terminal in the directory you ran `lean init` in.
+2. Run `lean cloud pull` to pull remotely changed files.
+3. Start programming locally and run backtests in the cloud with `lean cloud backtest "Project Name" --open --push` whenever there is something to backtest. The `--open` flag means that the backtest results will be opened in the browser when done, while the `--push` flag means that local changes are pushed to the cloud before running the backtest.
+4. Whenever you want to create a new project, run `lean create-project "Project Name"` and `lean cloud push --project "Project Name"` to create a new project containing some basic code and to push it to the cloud.
+5. When you're finished for the moment, run `lean cloud push` to push all locally changed files to the cloud.
+
+A locally-focused workflow (local development, local execution) with the CLI may look like this:
+1. Open a terminal in the directory you ran `lean init` in.
+2. Run `lean create-project "Project Name"` to create a new project with some basic code to get you started.
+3. Work on your strategy in `./Project Name`.
+4. Run `lean research "Project Name"` to start a Jupyter Lab session to perform research in.
+5. Run `lean backtest "Project Name"` to run a backtest whenever there's something to test. This runs your strategy in a Docker container containing the same packages as the ones used on QuantConnect.com, but with your own data.
+
+## Commands
+
+*Note: the readme only contains the `--help` text of all commands. Visit the [documentation website](https://www.lean.io/docs/lean-cli/key-concepts/getting-started) for more comprehensive documentation.*
+
+<!-- commands start -->
+- [`lean backtest`](#lean-backtest)
+- [`lean build`](#lean-build)
+- [`lean cloud backtest`](#lean-cloud-backtest)
+- [`lean cloud live`](#lean-cloud-live)
+- [`lean cloud optimize`](#lean-cloud-optimize)
+- [`lean cloud pull`](#lean-cloud-pull)
+- [`lean cloud push`](#lean-cloud-push)
+- [`lean cloud status`](#lean-cloud-status)
+- [`lean config get`](#lean-config-get)
+- [`lean config list`](#lean-config-list)
+- [`lean config set`](#lean-config-set)
+- [`lean config unset`](#lean-config-unset)
+- [`lean create-project`](#lean-create-project)
+- [`lean data download`](#lean-data-download)
+- [`lean data generate`](#lean-data-generate)
+- [`lean gui logs`](#lean-gui-logs)
+- [`lean gui restart`](#lean-gui-restart)
+- [`lean gui start`](#lean-gui-start)
+- [`lean gui stop`](#lean-gui-stop)
+- [`lean init`](#lean-init)
+- [`lean library add`](#lean-library-add)
+- [`lean library remove`](#lean-library-remove)
+- [`lean live`](#lean-live)
+- [`lean login`](#lean-login)
+- [`lean logout`](#lean-logout)
+- [`lean logs`](#lean-logs)
+- [`lean optimize`](#lean-optimize)
+- [`lean report`](#lean-report)
+- [`lean research`](#lean-research)
+- [`lean whoami`](#lean-whoami)
+
+### `lean backtest`
+
+Backtest a project locally using Docker.
+
+```
+Usage: lean backtest [OPTIONS] PROJECT
+
+  Backtest a project locally using Docker.
+
+  If PROJECT is a directory, the algorithm in the main.py or Main.cs file inside it will be executed.
+  If PROJECT is a file, the algorithm in the specified file will be executed.
+
+  Go to the following url to learn how to debug backtests locally using the Lean CLI:
+  https://www.lean.io/docs/lean-cli/backtesting/debugging
+
+  By default the official LEAN engine image is used. You can override this using the --image option. Alternatively you
+  can set the default engine image for all commands using `lean config set engine-image <image>`.
+
+Options:
+  --output DIRECTORY              Directory to store results in (defaults to PROJECT/backtests/TIMESTAMP)
+  -d, --detach                    Run the backtest in a detached Docker container and return immediately
+  --debug [pycharm|ptvsd|vsdbg|rider]
+                                  Enable a certain debugging method (see --help for more information)
+  --data-provider [Terminal Link|QuantConnect|Local]
+                                  Update the Lean configuration file to retrieve data from the given provider
+  --download-data                 Update the Lean configuration file to download data from the QuantConnect API, alias
+                                  for --data-provider QuantConnect
+
+  --data-purchase-limit INTEGER   The maximum amount of QCC to spend on downloading data during the backtest when using
+                                  QuantConnect as data provider
+
+  --release                       Compile C# projects in release configuration instead of debug
+  --image TEXT                    The LEAN engine image to use (defaults to quantconnect/lean:latest)
+  --update                        Pull the LEAN engine image before running the backtest
+  --lean-config FILE              The Lean configuration file that should be used (defaults to the nearest lean.json)
+  --verbose                       Enable debug logging
+  --help                          Show this message and exit.
+```
+
+_See code: [lean/commands/backtest.py](https://github.com/QuantConnect/lean-cli/blob/master/lean/commands/backtest.py)_
+
+### `lean build`
+
+Build Docker images of your own version of LEAN and the Alpha Streams SDK.
+
+```
+Usage: lean build [OPTIONS] [ROOT]
+
+  Build Docker images of your own version of LEAN and the Alpha Streams SDK.
+
+  ROOT must point to a directory containing the LEAN repository and the Alpha Streams SDK repository:
+  https://github.com/QuantConnect/Lean & https://github.com/QuantConnect/AlphaStreams
+
+  When ROOT is not given, the current directory is used as root directory.
+
+  This command performs the following actions:
+  1. The lean-cli/foundation:latest image is built from Lean/DockerfileLeanFoundation(ARM).
+  2. LEAN is compiled in a Docker container using the lean-cli/foundation:latest image.
+  3. The Alpha Streams SDK is compiled in a Docker container using the lean-cli/foundation:latest image.
+  4. The lean-cli/engine:latest image is built from Lean/Dockerfile using lean-cli/foundation:latest as base image.
+  5. The lean-cli/research:latest image is built from Lean/DockerfileJupyter using lean-cli/engine:latest as base image.
+  6. The default engine image is set to lean-cli/engine:latest.
+  7. The default research image is set to lean-cli/research:latest.
+
+  When the foundation Dockerfile is the same as the official foundation Dockerfile, quantconnect/lean:foundation is
+  used instead of building a custom foundation image.
+
+Options:
+  --tag TEXT  The tag to apply to custom images (defaults to latest)
+  --verbose   Enable debug logging
+  --help      Show this message and exit.
+```
+
+_See code: [lean/commands/build.py](https://github.com/QuantConnect/lean-cli/blob/master/lean/commands/build.py)_
+
+### `lean cloud backtest`
+
+Backtest a project in the cloud.
+
+```
+Usage: lean cloud backtest [OPTIONS] PROJECT
+
+  Backtest a project in the cloud.
+
+  PROJECT must be the name or id of the project to run a backtest for.
+
+  If the project that has to be backtested has been pulled to the local drive with `lean cloud pull` it is possible to
+  use the --push option to push local modifications to the cloud before running the backtest.
+
+Options:
+  --name TEXT  The name of the backtest (a random one is generated if not specified)
+  --push       Push local modifications to the cloud before running the backtest
+  --open       Automatically open the results in the browser when the backtest is finished
+  --verbose    Enable debug logging
+  --help       Show this message and exit.
+```
+
+_See code: [lean/commands/cloud/backtest.py](https://github.com/QuantConnect/lean-cli/blob/master/lean/commands/cloud/backtest.py)_
+
+### `lean cloud live`
+
+Start live trading for a project in the cloud.
+
+```
+Usage: lean cloud live [OPTIONS] PROJECT
+
+  Start live trading for a project in the cloud.
+
+  PROJECT must be the name or the id of the project to start live trading for.
+
+  By default an interactive wizard is shown letting you configure the deployment. If --brokerage is given the command
+  runs in non-interactive mode. In this mode the CLI does not prompt for input or confirmation. In non-interactive
+  mode the options specific to the given brokerage are required, as well as --node, --auto-restart, --notify-order-
+  events and --notify-insights.
+
+Options:
+  --brokerage [Paper Trading|Interactive Brokers|Tradier|Oanda|Bitfinex|Coinbase Pro|Binance|Zerodha|Samco|Kraken|FTX]
+                                  The brokerage to use
+  --ib-user-name TEXT             Your Interactive Brokers username
+  --ib-account TEXT               Your Interactive Brokers account id
+  --ib-password TEXT              Your Interactive Brokers password
+  --ib-data-feed BOOLEAN          Whether the Interactive Brokers price data feed must be used instead of the
+                                  QuantConnect price data feed
+
+  --tradier-account-id TEXT       Your Tradier account id
+  --tradier-access-token TEXT     Your Tradier access token
+  --tradier-environment [live|paper]
+                                  Whether the developer sandbox should be used
+  --oanda-environment [Practice|Trade]
+                                  The environment to run in, Practice for fxTrade Practice, Trade for fxTrade
+  --oanda-account-id TEXT         Your OANDA account id
+  --oanda-access-token TEXT       Your OANDA API token
+  --bitfinex-api-key TEXT         Your Bitfinex API key
+  --bitfinex-api-secret TEXT      Your Bitfinex API secret
+  --gdax-use-sandbox [live|paper]
+                                  Whether the sandbox should be used
+  --gdax-api-key TEXT             Your Coinbase Pro API key
+  --gdax-api-secret TEXT          Your Coinbase Pro API secret
+  --gdax-passphrase TEXT          Your Coinbase Pro API passphrase
+  --binance-use-testnet [live|paper]
+                                  Whether the testnet should be used
+  --binance-api-key TEXT          Your Binance API key
+  --binance-api-secret TEXT       Your Binance API secret
+  --zerodha-api-key TEXT          Your Kite Connect API key
+  --zerodha-access-token TEXT     Your Kite Connect access token
+  --zerodha-product-type [MIS|CNC|NRML]
+                                  MIS if you are targeting intraday products, CNC if you are targeting delivery
+                                  products, NRML if you are targeting carry forward products
+
+  --zerodha-trading-segment [EQUITY|COMMODITY]
+                                  EQUITY if you are trading equities on NSE or BSE, COMMODITY if you are trading
+                                  commodities on MCX
+
+  --samco-client-id TEXT          Your Samco account Client ID
+  --samco-client-password TEXT    Your Samco account password
+  --samco-year-of-birth TEXT      Your year of birth (YYYY) registered with Samco
+  --samco-product-type [MIS|CNC|NRML]
+                                  MIS if you are targeting intraday products, CNC if you are targeting delivery
+                                  products, NRML if you are targeting carry forward products
+
+  --samco-trading-segment [EQUITY|COMMODITY]
+                                  EQUITY if you are trading equities on NSE or BSE, COMMODITY if you are trading
+                                  commodities on MCX
+
+  --kraken-api-key TEXT           Your Kraken API key
+  --kraken-api-secret TEXT        Your Kraken API secret
+  --kraken-verification-tier [Starter|Intermediate|Pro]
+                                  Your Kraken Verification Tier
+  --ftx-exchange-name [FTX|FTXUS]
+                                  FTX exchange name [FTX, FTXUS]
+  --ftx-api-key TEXT              Your FTX API key
+  --ftxus-api-key TEXT            Your FTX API key
+  --ftx-api-secret TEXT           Your FTX API secret
+  --ftxus-api-secret TEXT         Your FTX API secret
+  --ftx-account-tier [Tier1|Tier2|Tier3|Tier4|Tier5|Tier6]
+                                  Your FTX Account Tier
+  --ftxus-account-tier [Tier1|Tier2|Tier3|Tier4|Tier5|Tier6]
+                                  Your FTX Account Tier
+  --node TEXT                     The name or id of the live node to run on
+  --auto-restart BOOLEAN          Whether automatic algorithm restarting must be enabled
+  --notify-order-events BOOLEAN   Whether notifications must be sent for order events
+  --notify-insights BOOLEAN       Whether notifications must be sent for emitted insights
+  --notify-emails TEXT            A comma-separated list of 'email:subject' pairs configuring email-notifications
+  --notify-webhooks TEXT          A comma-separated list of 'url:HEADER_1=VALUE_1:HEADER_2=VALUE_2:etc' pairs
+                                  configuring webhook-notifications
+
+  --notify-sms TEXT               A comma-separated list of phone numbers configuring SMS-notifications
+  --push                          Push local modifications to the cloud before starting live trading
+  --open                          Automatically open the live results in the browser once the deployment starts
+  --verbose                       Enable debug logging
+  --help                          Show this message and exit.
+```
+
+_See code: [lean/commands/cloud/live.py](https://github.com/QuantConnect/lean-cli/blob/master/lean/commands/cloud/live.py)_
+
+### `lean cloud optimize`
+
+Optimize a project in the cloud.
+
+```
+Usage: lean cloud optimize [OPTIONS] PROJECT
+
+  Optimize a project in the cloud.
+
+  PROJECT must be the name or id of the project to optimize.
+
+  An interactive prompt will be shown to configure the optimizer. If --target is given the command runs in non-
+  interactive mode. In this mode the CLI does not prompt for input and the following options become required:
+  --target, --target-direction, --parameter, --node and --parallel-nodes.
+
+  In non-interactive mode the --parameter option can be provided multiple times to configure multiple parameters:
+  - --parameter <name> <min value> <max value> <step size>
+  - --parameter my-first-parameter 1 10 0.5 --parameter my-second-parameter 20 30 5
+
+  In non-interactive mode the --constraint option can be provided multiple times to configure multiple constraints:
+  - --constraint "<statistic> <operator> <value>"
+  - --constraint "Sharpe Ratio >= 0.5" --constraint "Drawdown < 0.25"
+
+  If the project that has to be optimized has been pulled to the local drive with `lean cloud pull` it is possible to
+  use the --push option to push local modifications to the cloud before running the optimization.
+
+Options:
+  --target TEXT                   The target statistic of the optimization
+  --target-direction [min|max]    Whether the target must be minimized or maximized
+  --parameter <TEXT FLOAT FLOAT FLOAT>...
+                                  The 'parameter min max step' pairs configuring the parameters to optimize
+  --constraint TEXT               The 'statistic operator value' pairs configuring the constraints of the optimization
+  --node [O2-8|O4-12|O8-16]       The node type to run the optimization on
+  --parallel-nodes INTEGER        The number of nodes that may be run in parallel
+  --name TEXT                     The name of the optimization (a random one is generated if not specified)
+  --push                          Push local modifications to the cloud before starting the optimization
+  --verbose                       Enable debug logging
+  --help                          Show this message and exit.
+```
+
+_See code: [lean/commands/cloud/optimize.py](https://github.com/QuantConnect/lean-cli/blob/master/lean/commands/cloud/optimize.py)_
+
+### `lean cloud pull`
+
+Pull projects from QuantConnect to the local drive.
+
+```
+Usage: lean cloud pull [OPTIONS]
+
+  Pull projects from QuantConnect to the local drive.
+
+  This command overrides the content of local files with the content of their respective counterparts in the cloud.
+
+  This command will not delete local files for which there is no counterpart in the cloud.
+
+Options:
+  --project TEXT   Name or id of the project to pull (all cloud projects if not specified)
+  --pull-bootcamp  Pull Boot Camp projects (disabled by default)
+  --verbose        Enable debug logging
+  --help           Show this message and exit.
+```
+
+_See code: [lean/commands/cloud/pull.py](https://github.com/QuantConnect/lean-cli/blob/master/lean/commands/cloud/pull.py)_
+
+### `lean cloud push`
+
+Push local projects to QuantConnect.
+
+```
+Usage: lean cloud push [OPTIONS]
+
+  Push local projects to QuantConnect.
+
+  This command overrides the content of cloud files with the content of their respective local counterparts.
+
+  This command will not delete cloud files which don't have a local counterpart.
+
+Options:
+  --project DIRECTORY  Path to the local project to push (all local projects if not specified)
+  --verbose            Enable debug logging
+  --help               Show this message and exit.
+```
+
+_See code: [lean/commands/cloud/push.py](https://github.com/QuantConnect/lean-cli/blob/master/lean/commands/cloud/push.py)_
+
+### `lean cloud status`
+
+Show the live trading status of a project in the cloud.
+
+```
+Usage: lean cloud status [OPTIONS] PROJECT
+
+  Show the live trading status of a project in the cloud.
+
+  PROJECT must be the name or the id of the project to show the status for.
+
+Options:
+  --verbose  Enable debug logging
+  --help     Show this message and exit.
+```
+
+_See code: [lean/commands/cloud/status.py](https://github.com/QuantConnect/lean-cli/blob/master/lean/commands/cloud/status.py)_
+
+### `lean config get`
+
+Get the current value of a configurable option.
+
+```
+Usage: lean config get [OPTIONS] KEY
+
+  Get the current value of a configurable option.
+
+  Sensitive options like credentials cannot be retrieved this way for security reasons. Please open
+  ~/.lean/credentials if you want to see your currently stored credentials.
+
+  Run `lean config list` to show all available options.
+
+Options:
+  --verbose  Enable debug logging
+  --help     Show this message and exit.
+```
+
+_See code: [lean/commands/config/get.py](https://github.com/QuantConnect/lean-cli/blob/master/lean/commands/config/get.py)_
+
+### `lean config list`
+
+List the configurable options and their current values.
+
+```
+Usage: lean config list [OPTIONS]
+
+  List the configurable options and their current values.
+
+Options:
+  --verbose  Enable debug logging
+  --help     Show this message and exit.
+```
+
+_See code: [lean/commands/config/list.py](https://github.com/QuantConnect/lean-cli/blob/master/lean/commands/config/list.py)_
+
+### `lean config set`
+
+Set a configurable option.
+
+```
+Usage: lean config set [OPTIONS] KEY VALUE
+
+  Set a configurable option.
+
+  Run `lean config list` to show all available options.
+
+Options:
+  --verbose  Enable debug logging
+  --help     Show this message and exit.
+```
+
+_See code: [lean/commands/config/set.py](https://github.com/QuantConnect/lean-cli/blob/master/lean/commands/config/set.py)_
+
+### `lean config unset`
+
+Unset a configurable option.
+
+```
+Usage: lean config unset [OPTIONS] KEY
+
+  Unset a configurable option.
+
+  Run `lean config list` to show all available options.
+
+Options:
+  --verbose  Enable debug logging
+  --help     Show this message and exit.
+```
+
+_See code: [lean/commands/config/unset.py](https://github.com/QuantConnect/lean-cli/blob/master/lean/commands/config/unset.py)_
+
+### `lean create-project`
+
+Create a new project containing starter code.
+
+```
+Usage: lean create-project [OPTIONS] NAME
+
+  Create a new project containing starter code.
+
+  If NAME is a path containing subdirectories those will be created automatically.
+
+  The default language can be set using `lean config set default-language python/csharp`.
+
+Options:
+  -l, --language [python|csharp]  The language of the project to create
+  --verbose                       Enable debug logging
+  --help                          Show this message and exit.
+```
+
+_See code: [lean/commands/create_project.py](https://github.com/QuantConnect/lean-cli/blob/master/lean/commands/create_project.py)_
+
+### `lean data download`
+
+Purchase and download data from QuantConnect Datasets.
+
+```
+Usage: lean data download [OPTIONS]
+
+  Purchase and download data from QuantConnect Datasets.
+
+  An interactive wizard will show to walk you through the process of selecting data, accepting the CLI API Access and
+  Data Agreement and payment. After this wizard the selected data will be downloaded automatically.
+
+  If --dataset is given the command runs in non-interactive mode. In this mode the CLI does not prompt for input or
+  confirmation but only halts when the agreement must be accepted. In non-interactive mode all options specific to the
+  selected dataset as well as --organization are required.
+
+  See the following url for the data that can be purchased and downloaded with this command:
+  https://www.quantconnect.com/datasets
+
+Options:
+  --dataset TEXT       The name of the dataset to download non-interactively
+  --organization TEXT  The name or id of the organization to purchase and download data with
+  --overwrite          Overwrite existing local data
+  --lean-config FILE   The Lean configuration file that should be used (defaults to the nearest lean.json)
+  --verbose            Enable debug logging
+  --help               Show this message and exit.
+```
+
+_See code: [lean/commands/data/download.py](https://github.com/QuantConnect/lean-cli/blob/master/lean/commands/data/download.py)_
+
+### `lean data generate`
+
+Generate random market data.
+
+```
+Usage: lean data generate [OPTIONS]
+
+  Generate random market data.
+
+  This uses the random data generator in LEAN to generate realistic market data using a Brownian motion model.
+  This generator supports the following security types, tick types and resolutions:
+  | Security type | Generated tick types | Supported resolutions                |
+  | ------------- | -------------------- | ------------------------------------ |
+  | Equity        | Trade                | Tick, Second, Minute, Hour and Daily |
+  | Forex         | Quote                | Tick, Second, Minute, Hour and Daily |
+  | CFD           | Quote                | Tick, Second, Minute, Hour and Daily |
+  | Future        | Trade and Quote      | Tick, Second, Minute, Hour and Daily |
+  | Crypto        | Trade and Quote      | Tick, Second, Minute, Hour and Daily |
+  | Option        | Trade and Quote      | Minute                               |
+
+  The following data densities are available:
+  - Dense: at least one data point per resolution step.
+  - Sparse: at least one data point per 5 resolution steps.
+  - VerySparse: at least one data point per 50 resolution steps.
+
+  Example which generates minute data for 100 equity symbols since 2015-01-01:
+  $ lean data generate --start=20150101 --symbol-count=100
+
+  Example which generates daily data for 100 crypto symbols since 2015-01-01:
+  $ lean data generate --start=20150101 --symbol-count=100 --security-type=Crypto --resolution=Daily
+
+  By default the official LEAN engine image is used. You can override this using the --image option. Alternatively you
+  can set the default engine image for all commands using `lean config set engine-image <image>`.
+
+Options:
+  --start [yyyyMMdd]              Start date for the data to generate in yyyyMMdd format  [required]
+  --end [yyyyMMdd]                End date for the data to generate in yyyyMMdd format (defaults to today)
+  --symbol-count INTEGER RANGE    The number of symbols to generate data for  [required]
+  --security-type [Equity|Forex|Cfd|Future|Crypto|Option]
+                                  The security type to generate data for (defaults to Equity)
+  --resolution [Tick|Second|Minute|Hour|Daily]
+                                  The resolution of the generated data (defaults to Minute)
+  --data-density [Dense|Sparse|VerySparse]
+                                  The density of the generated data (defaults to Dense)
+  --include-coarse BOOLEAN        Whether coarse universe data should be generated for Equity data (defaults to True)
+  --market TEXT                   The market to generate data for (defaults to standard market for the security type)
+  --image TEXT                    The LEAN engine image to use (defaults to quantconnect/lean:latest)
+  --update                        Pull the LEAN engine image before running the generator
+  --lean-config FILE              The Lean configuration file that should be used (defaults to the nearest lean.json)
+  --verbose                       Enable debug logging
+  --help                          Show this message and exit.
+```
+
+_See code: [lean/commands/data/generate.py](https://github.com/QuantConnect/lean-cli/blob/master/lean/commands/data/generate.py)_
+
+### `lean gui logs`
+
+See the logs of the local GUI.
+
+```
+Usage: lean gui logs [OPTIONS]
+
+  See the logs of the local GUI.
+
+Options:
+  -f, --follow  Update the logs in real-time while the GUI is running
+  --verbose     Enable debug logging
+  --help        Show this message and exit.
+```
+
+_See code: [lean/commands/gui/logs.py](https://github.com/QuantConnect/lean-cli/blob/master/lean/commands/gui/logs.py)_
+
+### `lean gui restart`
+
+Restart the local GUI and open it in the browser.
+
+```
+Usage: lean gui restart [OPTIONS]
+
+  Restart the local GUI and open it in the browser.
+
+Options:
+  --no-open  Skip opening the local GUI in the browser after restarting it
+  --verbose  Enable debug logging
+  --help     Show this message and exit.
+```
+
+_See code: [lean/commands/gui/restart.py](https://github.com/QuantConnect/lean-cli/blob/master/lean/commands/gui/restart.py)_
+
+### `lean gui start`
+
+Start the local GUI.
+
+```
+Usage: lean gui start [OPTIONS]
+
+  Start the local GUI.
+
+Options:
+  --organization TEXT  The name or id of the organization with the local GUI module subscription
+  --port INTEGER       The port to run the local GUI on (defaults to 5612)
+  --no-open            Skip opening the local GUI in the browser after starting it
+  --shortcut           Create a desktop shortcut for launching the local GUI
+  --lean-config FILE   The Lean configuration file that should be used (defaults to the nearest lean.json)
+  --verbose            Enable debug logging
+  --help               Show this message and exit.
+```
+
+_See code: [lean/commands/gui/start.py](https://github.com/QuantConnect/lean-cli/blob/master/lean/commands/gui/start.py)_
+
+### `lean gui stop`
+
+Stop the local GUI.
+
+```
+Usage: lean gui stop [OPTIONS]
+
+  Stop the local GUI.
+
+Options:
+  --verbose  Enable debug logging
+  --help     Show this message and exit.
+```
+
+_See code: [lean/commands/gui/stop.py](https://github.com/QuantConnect/lean-cli/blob/master/lean/commands/gui/stop.py)_
+
+### `lean init`
+
+Scaffold a Lean configuration file and data directory.
+
+```
+Usage: lean init [OPTIONS]
+
+  Scaffold a Lean configuration file and data directory.
+
+Options:
+  --verbose  Enable debug logging
+  --help     Show this message and exit.
+```
+
+_See code: [lean/commands/init.py](https://github.com/QuantConnect/lean-cli/blob/master/lean/commands/init.py)_
+
+### `lean library add`
+
+Add a custom library to a project.
+
+```
+Usage: lean library add [OPTIONS] PROJECT NAME
+
+  Add a custom library to a project.
+
+  PROJECT must be the path to the project.
+
+  NAME must be the name of a NuGet package (for C# projects) or of a PyPI package (for Python projects).
+
+  If --version is not given, the package is pinned to the latest compatible version. For C# projects, this is the
+  latest available version. For Python projects, this is the latest version compatible with Python 3.6 (which is what
+  the Docker images use).
+
+  Custom C# libraries are added to your project's .csproj file, which is then restored if dotnet is on your PATH and
+  the --no-local flag has not been given.
+
+  Custom Python libraries are added to your project's requirements.txt file and are installed in your local Python
+  environment so you get local autocomplete for the library. The last step can be skipped with the --no-local flag.
+
+  C# example usage:
+  $ lean library add "My CSharp Project" Microsoft.ML
+  $ lean library add "My CSharp Project" Microsoft.ML --version 1.5.5
+
+  Python example usage:
+  $ lean library add "My Python Project" tensorflow
+  $ lean library add "My Python Project" tensorflow --version 2.5.0
+
+Options:
+  --version TEXT  The version of the library to add (defaults to latest compatible version)
+  --no-local      Skip making changes to your local environment
+  --verbose       Enable debug logging
+  --help          Show this message and exit.
+```
+
+_See code: [lean/commands/library/add.py](https://github.com/QuantConnect/lean-cli/blob/master/lean/commands/library/add.py)_
+
+### `lean library remove`
+
+Remove a custom library from a project.
+
+```
+Usage: lean library remove [OPTIONS] PROJECT NAME
+
+  Remove a custom library from a project.
+
+  PROJECT must be the path to the project directory.
+
+  NAME must be the name of the NuGet package (for C# projects) or of the PyPI package (for Python projects) to remove.
+
+  Custom C# libraries are removed from the project's .csproj file, which is then restored if dotnet is on your PATH
+  and the --no-local flag has not been given.
+
+  Custom Python libraries are removed from the project's requirements.txt file.
+
+  C# example usage:
+  $ lean library remove "My CSharp Project" Microsoft.ML
+
+  Python example usage:
+  $ lean library remove "My Python Project" tensorflow
+
+Options:
+  --no-local  Skip making changes to your local environment
+  --verbose   Enable debug logging
+  --help      Show this message and exit.
+```
+
+_See code: [lean/commands/library/remove.py](https://github.com/QuantConnect/lean-cli/blob/master/lean/commands/library/remove.py)_
+
+### `lean live`
+
+Start live trading a project locally using Docker.
+
+```
+Usage: lean live [OPTIONS] PROJECT
+
+  Start live trading a project locally using Docker.
+
+  If PROJECT is a directory, the algorithm in the main.py or Main.cs file inside it will be executed.
+  If PROJECT is a file, the algorithm in the specified file will be executed.
+
+  By default an interactive wizard is shown letting you configure the brokerage and data feed to use. If
+  --environment, --brokerage or --data-feed are given the command runs in non-interactive mode. In this mode the CLI
+  does not prompt for input.
+
+  If --environment is given it must be the name of a live environment in the Lean configuration.
+
+  If --brokerage and --data-feed are given, the options specific to the given brokerage/data feed must also be given.
+  The Lean config is used as fallback when a brokerage/data feed-specific option hasn't been passed in. If a required
+  option is not given and cannot be found in the Lean config the command aborts.
+
+  By default the official LEAN engine image is used. You can override this using the --image option. Alternatively you
+  can set the default engine image for all commands using `lean config set engine-image <image>`.
+
+Options:
+  --environment TEXT              The environment to use
+  --output DIRECTORY              Directory to store results in (defaults to PROJECT/live/TIMESTAMP)
+  -d, --detach                    Run the live deployment in a detached Docker container and return immediately
+  --gui                           Enable monitoring and controlling of the deployment via the local GUI
+  --gui-organization TEXT         The name or id of the organization with the local GUI module subscription
+  --brokerage [Paper Trading|Interactive Brokers|Tradier|Oanda|Bitfinex|Coinbase Pro|Binance|Zerodha|Samco|Terminal Link|Atreyu|Trading Technologies|Kraken|FTX]
+                                  The brokerage to use
+  --data-feed [Interactive Brokers|Tradier|Oanda|Bitfinex|Coinbase Pro|Binance|Zerodha|Samco|Terminal Link|Trading Technologies|Kraken|FTX|IQFeed|Custom data only]
+                                  The data feed to use
+  --ib-organization TEXT          The name or id of the organization with the Interactive Brokers module subscription
+  --ib-user-name TEXT             Your Interactive Brokers username
+  --ib-account TEXT               Your Interactive Brokers account id
+  --ib-password TEXT              Your Interactive Brokers password
+  --ib-enable-delayed-streaming-data BOOLEAN
+                                  Whether delayed data may be used when your algorithm subscribes to a security you
+                                  don't have a market data subscription for
+
+  --tradier-account-id TEXT       Your Tradier account id
+  --tradier-access-token TEXT     Your Tradier access token
+  --tradier-environment [live|paper]
+                                  Whether the developer sandbox should be used
+  --oanda-environment [Practice|Trade]
+                                  The environment to run in, Practice for fxTrade Practice, Trade for fxTrade
+  --oanda-account-id TEXT         Your OANDA account id
+  --oanda-access-token TEXT       Your OANDA API token
+  --bitfinex-api-key TEXT         Your Bitfinex API key
+  --bitfinex-api-secret TEXT      Your Bitfinex API secret
+  --gdax-use-sandbox [live|paper]
+                                  Whether the sandbox should be used
+  --gdax-api-key TEXT             Your Coinbase Pro API key
+  --gdax-api-secret TEXT          Your Coinbase Pro API secret
+  --gdax-passphrase TEXT          Your Coinbase Pro API passphrase
+  --binance-use-testnet [live|paper]
+                                  Whether the testnet should be used
+  --binance-organization TEXT     The name or id of the organization with the Binance module subscription
+  --binance-api-key TEXT          Your Binance API key
+  --binance-api-secret TEXT       Your Binance API secret
+  --zerodha-organization TEXT     The name or id of the organization with the zerodha module subscription
+  --zerodha-api-key TEXT          Your Kite Connect API key
+  --zerodha-access-token TEXT     Your Kite Connect access token
+  --zerodha-product-type [MIS|CNC|NRML]
+                                  MIS if you are targeting intraday products, CNC if you are targeting delivery
+                                  products, NRML if you are targeting carry forward products
+
+  --zerodha-trading-segment [EQUITY|COMMODITY]
+                                  EQUITY if you are trading equities on NSE or BSE, COMMODITY if you are trading
+                                  commodities on MCX
+
+  --zerodha-history-subscription BOOLEAN
+                                  Whether you have a history API subscription for Zerodha
+  --samco-organization TEXT       The name or id of the organization with the samco module subscription
+  --samco-client-id TEXT          Your Samco account Client ID
+  --samco-client-password TEXT    Your Samco account password
+  --samco-year-of-birth TEXT      Your year of birth (YYYY) registered with Samco
+  --samco-product-type [MIS|CNC|NRML]
+                                  MIS if you are targeting intraday products, CNC if you are targeting delivery
+                                  products, NRML if you are targeting carry forward products
+
+  --samco-trading-segment [EQUITY|COMMODITY]
+                                  EQUITY if you are trading equities on NSE or BSE, COMMODITY if you are trading
+                                  commodities on MCX
+
+  --terminal-link-organization TEXT
+                                  The name or id of the organization with the Terminal Link module subscription
+  --bloomberg-environment [Production|Beta]
+                                  The environment to run in
+  --bloomberg-server-host TEXT    The host of the Bloomberg server
+  --bloomberg-server-port INTEGER
+                                  The port of the Bloomberg server
+  --bloomberg-symbol-map-file FILE
+                                  The path to the Bloomberg symbol map file
+  --bloomberg-emsx-broker TEXT    The EMSX broker to use
+  --bloomberg-emsx-user-time-zone TEXT
+                                  The EMSX user timezone to use
+  --bloomberg-emsx-account TEXT   The EMSX account to use
+  --bloomberg-emsx-strategy TEXT  The EMSX strategy to use
+  --bloomberg-emsx-notes TEXT     The EMSX notes to use
+  --bloomberg-emsx-handling TEXT  The EMSX handling to use
+  --bloomberg-allow-modification BOOLEAN
+                                  Whether modification is allowed
+  --atreyu-organization TEXT      The name or id of the organization with the Atreyu module subscription
+  --atreyu-host TEXT              The host of the Atreyu server
+  --atreyu-req-port INTEGER       The Atreyu request port
+  --atreyu-sub-port INTEGER       The Atreyu subscribe port
+  --atreyu-username TEXT          Your Atreyu username
+  --atreyu-password TEXT          Your Atreyu password
+  --atreyu-client-id TEXT         Your Atreyu client id
+  --atreyu-broker-mpid TEXT       The broker MPID to use
+  --atreyu-locate-rqd TEXT        The locate rqd to use
+  --tt-organization TEXT          The name or id of the organization with the Trading Technologies module subscription
+  --tt-user-name TEXT             Your Trading Technologies username
+  --tt-session-password TEXT      Your Trading Technologies session password
+  --tt-account-name TEXT          Your Trading Technologies account name
+  --tt-rest-app-key TEXT          Your Trading Technologies REST app key
+  --tt-rest-app-secret TEXT       Your Trading Technologies REST app secret
+  --tt-rest-environment TEXT      The REST environment to run in
+  --tt-market-data-sender-comp-id TEXT
+                                  The market data sender comp id to use
+  --tt-market-data-target-comp-id TEXT
+                                  The market data target comp id to use
+  --tt-market-data-host TEXT      The host of the market data server
+  --tt-market-data-port TEXT      The port of the market data server
+  --tt-order-routing-sender-comp-id TEXT
+                                  The order routing sender comp id to use
+  --tt-order-routing-target-comp-id TEXT
+                                  The order routing target comp id to use
+  --tt-order-routing-host TEXT    The host of the order routing server
+  --tt-order-routing-port TEXT    The port of the order routing server
+  --tt-log-fix-messages BOOLEAN   Whether FIX messages should be logged
+  --kraken-organization TEXT      The name or id of the organization with the kraken module subscription
+  --kraken-api-key TEXT           Your Kraken API key
+  --kraken-api-secret TEXT        Your Kraken API secret
+  --kraken-verification-tier [Starter|Intermediate|Pro]
+                                  Your Kraken Verification Tier
+  --ftx-exchange-name [FTX|FTXUS]
+                                  FTX exchange name [FTX, FTXUS]
+  --ftx-organization TEXT         The name or id of the organization with the FTX module subscription
+  --ftx-api-key TEXT              Your FTX API key
+  --ftxus-api-key TEXT            Your FTX API key
+  --ftx-api-secret TEXT           Your FTX API secret
+  --ftxus-api-secret TEXT         Your FTX API secret
+  --ftx-account-tier [Tier1|Tier2|Tier3|Tier4|Tier5|Tier6]
+                                  Your FTX Account Tier
+  --ftxus-account-tier [Tier1|Tier2|Tier3|Tier4|Tier5|Tier6]
+                                  Your FTX Account Tier
+  --iqfeed-iqconnect FILE         The path to the IQConnect binary
+  --iqfeed-username TEXT          Your IQFeed username
+  --iqfeed-password TEXT          Your IQFeed password
+  --iqfeed-productName TEXT       The product name of your IQFeed developer account
+  --iqfeed-version TEXT           The product version of your IQFeed developer account
+  --release                       Compile C# projects in release configuration instead of debug
+  --image TEXT                    The LEAN engine image to use (defaults to quantconnect/lean:latest)
+  --update                        Pull the LEAN engine image before starting live trading
+  --lean-config FILE              The Lean configuration file that should be used (defaults to the nearest lean.json)
+  --verbose                       Enable debug logging
+  --help                          Show this message and exit.
+```
+
+_See code: [lean/commands/live.py](https://github.com/QuantConnect/lean-cli/blob/master/lean/commands/live.py)_
+
+### `lean login`
+
+Log in with a QuantConnect account.
+
+```
+Usage: lean login [OPTIONS]
+
+  Log in with a QuantConnect account.
+
+  If user id or API token is not provided an interactive prompt will show.
+
+  Credentials are stored in ~/.lean/credentials and are removed upon running `lean logout`.
+
+Options:
+  -u, --user-id TEXT    QuantConnect user id
+  -t, --api-token TEXT  QuantConnect API token
+  --verbose             Enable debug logging
+  --help                Show this message and exit.
+```
+
+_See code: [lean/commands/login.py](https://github.com/QuantConnect/lean-cli/blob/master/lean/commands/login.py)_
+
+### `lean logout`
+
+Log out and remove stored credentials.
+
+```
+Usage: lean logout [OPTIONS]
+
+  Log out and remove stored credentials.
+
+Options:
+  --verbose  Enable debug logging
+  --help     Show this message and exit.
+```
+
+_See code: [lean/commands/logout.py](https://github.com/QuantConnect/lean-cli/blob/master/lean/commands/logout.py)_
+
+### `lean logs`
+
+Display the most recent backtest/live/optimization logs.
+
+```
+Usage: lean logs [OPTIONS]
+
+  Display the most recent backtest/live/optimization logs.
+
+Options:
+  --backtest           Display the most recent backtest logs (default)
+  --live               Display the most recent live logs
+  --optimization       Display the most recent optimization logs
+  --project DIRECTORY  The project to get the most recent logs from
+  --lean-config FILE   The Lean configuration file that should be used (defaults to the nearest lean.json)
+  --verbose            Enable debug logging
+  --help               Show this message and exit.
+```
+
+_See code: [lean/commands/logs.py](https://github.com/QuantConnect/lean-cli/blob/master/lean/commands/logs.py)_
+
+### `lean optimize`
+
+Optimize a project's parameters locally using Docker.
+
+```
+Usage: lean optimize [OPTIONS] PROJECT
+
+  Optimize a project's parameters locally using Docker.
+
+  If PROJECT is a directory, the algorithm in the main.py or Main.cs file inside it will be executed.
+  If PROJECT is a file, the algorithm in the specified file will be executed.
+
+  By default an interactive wizard is shown letting you configure the optimizer. If --optimizer-config or --strategy
+  is given the command runs in non-interactive mode. In this mode the CLI does not prompt for input.
+
+  The --optimizer-config option can be used to specify the configuration to run the optimizer with.
+  When using the option it should point to a file like this (the algorithm-* properties should be omitted):
+  https://github.com/QuantConnect/Lean/blob/master/Optimizer.Launcher/config.json
+
+  If --strategy is given the optimizer configuration is read from the given options. In this case --strategy,
+  --target, --target-direction and --parameter become required.
+
+  In non-interactive mode the --parameter option can be provided multiple times to configure multiple parameters:
+  - --parameter <name> <min value> <max value> <step size>
+  - --parameter my-first-parameter 1 10 0.5 --parameter my-second-parameter 20 30 5
+
+  In non-interactive mode the --constraint option can be provided multiple times to configure multiple constraints:
+  - --constraint "<statistic> <operator> <value>"
+  - --constraint "Sharpe Ratio >= 0.5" --constraint "Drawdown < 0.25"
+
+  By default the official LEAN engine image is used. You can override this using the --image option. Alternatively you
+  can set the default engine image for all commands using `lean config set engine-image <image>`.
+
+Options:
+  --output DIRECTORY              Directory to store results in (defaults to PROJECT/optimizations/TIMESTAMP)
+  -d, --detach                    Run the optimization in a detached Docker container and return immediately
+  --optimizer-config FILE         The optimizer configuration file that should be used
+  --strategy [Grid Search|Euler Search]
+                                  The optimization strategy to use
+  --target TEXT                   The target statistic of the optimization
+  --target-direction [min|max]    Whether the target must be minimized or maximized
+  --parameter <TEXT FLOAT FLOAT FLOAT>...
+                                  The 'parameter min max step' pairs configuring the parameters to optimize
+  --constraint TEXT               The 'statistic operator value' pairs configuring the constraints of the optimization
+  --release                       Compile C# projects in release configuration instead of debug
+  --image TEXT                    The LEAN engine image to use (defaults to quantconnect/lean:latest)
+  --update                        Pull the LEAN engine image before running the optimizer
+  --lean-config FILE              The Lean configuration file that should be used (defaults to the nearest lean.json)
+  --verbose                       Enable debug logging
+  --help                          Show this message and exit.
+```
+
+_See code: [lean/commands/optimize.py](https://github.com/QuantConnect/lean-cli/blob/master/lean/commands/optimize.py)_
+
+### `lean report`
+
+Generate a report of a backtest.
+
+```
+Usage: lean report [OPTIONS]
+
+  Generate a report of a backtest.
+
+  This runs the LEAN Report Creator in Docker to generate a polished, professional-grade report of a backtest.
+
+  If --backtest-results is not given, a report is generated for the most recent local backtest.
+
+  The name, description, and version are optional and will be blank if not given.
+
+  If the given backtest data source file is stored in a project directory (or one of its subdirectories, like the
+  default <project>/backtests/<timestamp>), the default name is the name of the project directory and the default
+  description is the description stored in the project's config.json file.
+
+  By default the official LEAN engine image is used. You can override this using the --image option. Alternatively you
+  can set the default engine image for all commands using `lean config set engine-image <image>`.
+
+Options:
+  --backtest-results FILE      Path to the JSON file containing the backtest results
+  --live-results FILE          Path to the JSON file containing the live trading results
+  --report-destination FILE    Path where the generated report is stored as HTML (defaults to ./report.html)
+  -d, --detach                 Run the report creator in a detached Docker container and return immediately
+  --strategy-name TEXT         Name of the strategy, will appear at the top-right corner of each page
+  --strategy-version TEXT      Version number of the strategy, will appear next to the project name
+  --strategy-description TEXT  Description of the strategy, will appear under the 'Strategy Description' section
+  --overwrite                  Overwrite --report-destination if it already contains a file
+  --image TEXT                 The LEAN engine image to use (defaults to quantconnect/lean:latest)
+  --update                     Pull the LEAN engine image before running the report creator
+  --lean-config FILE           The Lean configuration file that should be used (defaults to the nearest lean.json)
+  --verbose                    Enable debug logging
+  --help                       Show this message and exit.
+```
+
+_See code: [lean/commands/report.py](https://github.com/QuantConnect/lean-cli/blob/master/lean/commands/report.py)_
+
+### `lean research`
+
+Run a Jupyter Lab environment locally using Docker.
+
+```
+Usage: lean research [OPTIONS] PROJECT
+
+  Run a Jupyter Lab environment locally using Docker.
+
+  By default the official LEAN research image is used. You can override this using the --image option. Alternatively
+  you can set the default research image using `lean config set research-image <image>`.
+
+Options:
+  --port INTEGER                  The port to run Jupyter Lab on (defaults to 8888)
+  --data-provider [Terminal Link|QuantConnect|Local]
+                                  Update the Lean configuration file to retrieve data from the given provider
+  --download-data                 Update the Lean configuration file to download data from the QuantConnect API, alias
+                                  for --data-provider QuantConnect
+
+  --data-purchase-limit INTEGER   The maximum amount of QCC to spend on downloading data during the research session
+                                  when using QuantConnect as data provider
+
+  -d, --detach                    Run Jupyter Lab in a detached Docker container and return immediately
+  --no-open                       Don't open the Jupyter Lab environment in the browser after starting it
+  --image TEXT                    The LEAN research image to use (defaults to quantconnect/research:latest)
+  --update                        Pull the LEAN research image before starting the research environment
+  --lean-config FILE              The Lean configuration file that should be used (defaults to the nearest lean.json)
+  --verbose                       Enable debug logging
+  --help                          Show this message and exit.
+```
+
+_See code: [lean/commands/research.py](https://github.com/QuantConnect/lean-cli/blob/master/lean/commands/research.py)_
+
+### `lean whoami`
+
+Display who is logged in.
+
+```
+Usage: lean whoami [OPTIONS]
+
+  Display who is logged in.
+
+Options:
+  --verbose  Enable debug logging
+  --help     Show this message and exit.
+```
+
+_See code: [lean/commands/whoami.py](https://github.com/QuantConnect/lean-cli/blob/master/lean/commands/whoami.py)_
+<!-- commands end -->
+
+## Development
+
+To work on the Lean CLI, clone the repository, enter an environment containing Python 3.6+ and run `pip install -r requirements.txt`. This command will install the required dependencies and installs the CLI in editable mode. This means you'll be able to edit the code and immediately see the results the next time you run `lean`.
+
+If you need to add dependencies, first update `setup.py` (if it is a production dependency) or `requirements.txt` (if it is a development dependency) and then re-run `pip install -r requirements.txt`.
+
+The automated tests can be ran by running `pytest`. The filesystem and HTTP requests are mocked when running tests to make sure they run in an isolated environment.
+
+Can build the lean CLI by running `python setup.py sdist bdist_wheel` from the root of the project and to install it `pip install --force-reinstall dist/lean-dev-py3-none-any.whl`. To update the commands reference part of the readme run `python scripts/readme.py` from the root of the project, after installing the new version.
+
+Maintainers can publish new releases by pushing a Git tag containing the new version to GitHub. This will trigger a GitHub Actions workflow which releases the current `master` branch to PyPI with the value of the tag as version. Make sure the version is not prefixed with "v".
```

### Comparing `ablean-1.3.7/ablean.egg-info/SOURCES.txt` & `ablean-1.3.8/ablean.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ablean-1.3.7/scripts/readme.py` & `ablean-1.3.8/scripts/readme.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,108 +1,108 @@
-# QUANTCONNECT.COM - Democratizing Finance, Empowering Individuals.
-# Lean CLI v1.0. Copyright 2021 QuantConnect Corporation.
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-
-# This program automatically updates the commands reference part of the readme
-# It should be ran using `python scripts/readme.py` from the root of the project
-
-import os
-
-os.environ["__README__"] = "true"
-
-import re
-from pathlib import Path
-from typing import List
-
-from click import Command, Group
-from click.testing import CliRunner
-
-from ablean.commands import lean
-from ablean.models.pydantic import WrappedBaseModel
-
-
-class NamedCommand(WrappedBaseModel):
-    name: str
-    command: Command
-
-    class Config:
-        arbitrary_types_allowed = True
-
-
-def get_commands(group: Group, parent_names: List[str] = []) -> List[NamedCommand]:
-    """Returns all lean commands by name.
-
-    :param group: the group to get the commands from
-    :param parent_names: the names of the groups leading up to the current group
-    :return: a list containing all commands in the current group with their full names
-    """
-    all_commands = []
-
-    for obj in group.commands.values():
-        if isinstance(obj, Group):
-            all_commands.extend(get_commands(obj, parent_names + [group.name]))
-        else:
-            name_parts = parent_names + [group.name, obj.name]
-            all_commands.append(NamedCommand(name=" ".join(name_parts), command=obj))
-
-    return all_commands
-
-
-def get_header_id(name: str) -> str:
-    """Returns the id of the header with the given name in a GitHub readme.
-
-    :param name: the name of the header to get the id of
-    :return: the id of the header with the given name when rendered on GitHub
-    """
-    name = name.lower()
-    name = re.sub(r"\s", "-", name)
-    name = re.sub(r"[^a-zA-Z0-9-]", "", name)
-    return name
-
-
-def main() -> None:
-    named_commands = get_commands(lean)
-    named_commands = sorted(named_commands, key=lambda c: c.name)
-
-    table_of_contents = []
-    command_sections = []
-
-    for c in named_commands:
-        header = f"### `{c.name}`"
-        help_str = c.command.get_short_help_str(limit=120)
-
-        help_output = CliRunner().invoke(c.command, ["--help"], prog_name=c.name, terminal_width=120).output.strip()
-        help_output = f"```\n{help_output}\n```"
-
-        command_source = f"lean/commands/{c.name.replace('lean ', '').replace(' ', '/').replace('-', '_')}.py"
-        command_source = f"_See code: [{command_source}]({command_source})_"
-
-        section_parts = [header, help_str, help_output, command_source]
-
-        table_of_contents.append(f"- [`{c.name}`](#{get_header_id(c.name)})")
-        command_sections.append("\n\n".join(section_parts))
-
-    full_text = "\n".join(table_of_contents) + "\n\n" + "\n\n".join(command_sections)
-    full_text = "\n".join(["<!-- commands start -->", full_text, "<!-- commands end -->"])
-
-    readme_path = Path.cwd() / "README.md"
-    readme_content = readme_path.read_text(encoding="utf-8")
-
-    readme_content = re.sub(r"<!-- commands start -->.*<!-- commands end -->",
-                            full_text,
-                            readme_content,
-                            flags=re.DOTALL)
-
-    readme_path.write_text(readme_content, encoding="utf-8")
-
-
-if __name__ == "__main__":
-    main()
+# QUANTCONNECT.COM - Democratizing Finance, Empowering Individuals.
+# Lean CLI v1.0. Copyright 2021 QuantConnect Corporation.
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+
+# This program automatically updates the commands reference part of the readme
+# It should be ran using `python scripts/readme.py` from the root of the project
+
+import os
+
+os.environ["__README__"] = "true"
+
+import re
+from pathlib import Path
+from typing import List
+
+from click import Command, Group
+from click.testing import CliRunner
+
+from ablean.commands import lean
+from ablean.models.pydantic import WrappedBaseModel
+
+
+class NamedCommand(WrappedBaseModel):
+    name: str
+    command: Command
+
+    class Config:
+        arbitrary_types_allowed = True
+
+
+def get_commands(group: Group, parent_names: List[str] = []) -> List[NamedCommand]:
+    """Returns all lean commands by name.
+
+    :param group: the group to get the commands from
+    :param parent_names: the names of the groups leading up to the current group
+    :return: a list containing all commands in the current group with their full names
+    """
+    all_commands = []
+
+    for obj in group.commands.values():
+        if isinstance(obj, Group):
+            all_commands.extend(get_commands(obj, parent_names + [group.name]))
+        else:
+            name_parts = parent_names + [group.name, obj.name]
+            all_commands.append(NamedCommand(name=" ".join(name_parts), command=obj))
+
+    return all_commands
+
+
+def get_header_id(name: str) -> str:
+    """Returns the id of the header with the given name in a GitHub readme.
+
+    :param name: the name of the header to get the id of
+    :return: the id of the header with the given name when rendered on GitHub
+    """
+    name = name.lower()
+    name = re.sub(r"\s", "-", name)
+    name = re.sub(r"[^a-zA-Z0-9-]", "", name)
+    return name
+
+
+def main() -> None:
+    named_commands = get_commands(lean)
+    named_commands = sorted(named_commands, key=lambda c: c.name)
+
+    table_of_contents = []
+    command_sections = []
+
+    for c in named_commands:
+        header = f"### `{c.name}`"
+        help_str = c.command.get_short_help_str(limit=120)
+
+        help_output = CliRunner().invoke(c.command, ["--help"], prog_name=c.name, terminal_width=120).output.strip()
+        help_output = f"```\n{help_output}\n```"
+
+        command_source = f"lean/commands/{c.name.replace('lean ', '').replace(' ', '/').replace('-', '_')}.py"
+        command_source = f"_See code: [{command_source}]({command_source})_"
+
+        section_parts = [header, help_str, help_output, command_source]
+
+        table_of_contents.append(f"- [`{c.name}`](#{get_header_id(c.name)})")
+        command_sections.append("\n\n".join(section_parts))
+
+    full_text = "\n".join(table_of_contents) + "\n\n" + "\n\n".join(command_sections)
+    full_text = "\n".join(["<!-- commands start -->", full_text, "<!-- commands end -->"])
+
+    readme_path = Path.cwd() / "README.md"
+    readme_content = readme_path.read_text(encoding="utf-8")
+
+    readme_content = re.sub(r"<!-- commands start -->.*<!-- commands end -->",
+                            full_text,
+                            readme_content,
+                            flags=re.DOTALL)
+
+    readme_path.write_text(readme_content, encoding="utf-8")
+
+
+if __name__ == "__main__":
+    main()
```

