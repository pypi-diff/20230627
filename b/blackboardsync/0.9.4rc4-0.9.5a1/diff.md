# Comparing `tmp/blackboardsync-0.9.4rc4.tar.gz` & `tmp/blackboardsync-0.9.5a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blackboardsync-0.9.4rc4.tar", last modified: Mon Jun 26 15:12:27 2023, max compression
+gzip compressed data, was "blackboardsync-0.9.5a1.tar", last modified: Tue Jun 27 16:01:39 2023, max compression
```

## Comparing `blackboardsync-0.9.4rc4.tar` & `blackboardsync-0.9.5a1.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:12:27.368759 blackboardsync-0.9.4rc4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:12:27.360759 blackboardsync-0.9.4rc4/.github/
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-26 15:11:45.000000 blackboardsync-0.9.4rc4/.github/FUNDING.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:12:27.360759 blackboardsync-0.9.4rc4/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)     2659 2023-06-26 15:11:45.000000 blackboardsync-0.9.4rc4/.github/ISSUE_TEMPLATE/unisupport.yml
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-06-26 15:11:45.000000 blackboardsync-0.9.4rc4/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:12:27.360759 blackboardsync-0.9.4rc4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     3907 2023-06-26 15:11:45.000000 blackboardsync-0.9.4rc4/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3291 2023-06-26 15:11:45.000000 blackboardsync-0.9.4rc4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     2636 2023-06-26 15:11:45.000000 blackboardsync-0.9.4rc4/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-06-26 15:11:45.000000 blackboardsync-0.9.4rc4/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-06-26 15:11:45.000000 blackboardsync-0.9.4rc4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6047 2023-06-26 15:12:27.368759 blackboardsync-0.9.4rc4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-06-26 15:11:45.000000 blackboardsync-0.9.4rc4/Pipfile
--rw-r--r--   0 runner    (1001) docker     (123)   107308 2023-06-26 15:11:45.000000 blackboardsync-0.9.4rc4/Pipfile.lock
--rw-r--r--   0 runner    (1001) docker     (123)     5382 2023-06-26 15:11:45.000000 blackboardsync-0.9.4rc4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3265 2023-06-26 15:11:45.000000 blackboardsync-0.9.4rc4/UNIVERSITIES.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:12:27.364759 blackboardsync-0.9.4rc4/blackboard_sync/
--rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-06-26 15:11:45.000000 blackboardsync-0.9.4rc4/blackboard_sync/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-06-26 15:11:45.000000 blackboardsync-0.9.4rc4/blackboard_sync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-06-26 15:11:45.000000 blackboardsync-0.9.4rc4/blackboard_sync/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:12:27.364759 blackboardsync-0.9.4rc4/blackboard_sync/assets/
--rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-06-26 15:11:45.000000 blackboardsync-0.9.4rc4/blackboard_sync/assets/alert.png
--rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-06-26 15:11:45.000000 blackboardsync-0.9.4rc4/blackboard_sync/assets/alert.svg
--rw-r--r--   0 runner    (1001) docker     (123)   110234 2023-06-26 15:11:45.000000 blackboardsync-0.9.4rc4/blackboard_sync/assets/logo.ico
--rw-r--r--   0 runner    (1001) docker     (123)    31742 2023-06-26 15:11:45.000000 blackboardsync-0.9.4rc4/blackboard_sync/assets/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)    36877 2023-06-26 15:11:45.000000 blackboardsync-0.9.4rc4/blackboard_sync/assets/watermark.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:12:27.364759 blackboardsync-0.9.4rc4/blackboard_sync/blackboard/
--rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-06-26 15:11:45.000000 blackboardsync-0.9.4rc4/blackboard_sync/blackboard/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29665 2023-06-26 15:11:45.000000 blackboardsync-0.9.4rc4/blackboard_sync/blackboard/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6003 2023-06-26 15:11:45.000000 blackboardsync-0.9.4rc4/blackboard_sync/blackboard/blackboard.py
--rw-r--r--   0 runner    (1001) docker     (123)     3957 2023-06-26 15:11:45.000000 blackboardsync-0.9.4rc4/blackboard_sync/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    10622 2023-06-26 15:11:45.000000 blackboardsync-0.9.4rc4/blackboard_sync/download.py
--rw-r--r--   0 runner    (1001) docker     (123)     4065 2023-06-26 15:11:45.000000 blackboardsync-0.9.4rc4/blackboard_sync/institutions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:12:27.364759 blackboardsync-0.9.4rc4/blackboard_sync/qt/
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-06-26 15:11:45.000000 blackboardsync-0.9.4rc4/blackboard_sync/qt/LoginWebView.ui
--rw-r--r--   0 runner    (1001) docker     (123)     5032 2023-06-26 15:11:45.000000 blackboardsync-0.9.4rc4/blackboard_sync/qt/PersistenceWarning.ui
--rw-r--r--   0 runner    (1001) docker     (123)     8000 2023-06-26 15:11:45.000000 blackboardsync-0.9.4rc4/blackboard_sync/qt/SettingsWindow.ui
--rw-r--r--   0 runner    (1001) docker     (123)     6564 2023-06-26 15:11:45.000000 blackboardsync-0.9.4rc4/blackboard_sync/qt/SetupWizard.ui
--rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-06-26 15:11:45.000000 blackboardsync-0.9.4rc4/blackboard_sync/qt/UniNotSupportedDialog.ui
--rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-06-26 15:11:45.000000 blackboardsync-0.9.4rc4/blackboard_sync/qt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20757 2023-06-26 15:11:45.000000 blackboardsync-0.9.4rc4/blackboard_sync/qt/qt_elements.py
--rw-r--r--   0 runner    (1001) docker     (123)    10613 2023-06-26 15:11:45.000000 blackboardsync-0.9.4rc4/blackboard_sync/sync.py
--rw-r--r--   0 runner    (1001) docker     (123)     7130 2023-06-26 15:11:45.000000 blackboardsync-0.9.4rc4/blackboard_sync/sync_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)    13794 2023-06-26 15:11:45.000000 blackboardsync-0.9.4rc4/blackboard_sync/universities.json
--rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-06-26 15:11:45.000000 blackboardsync-0.9.4rc4/blackboard_sync/updates.py
--rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-06-26 15:11:45.000000 blackboardsync-0.9.4rc4/blackboard_sync/webdav.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:12:27.364759 blackboardsync-0.9.4rc4/blackboardsync.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6047 2023-06-26 15:12:27.000000 blackboardsync-0.9.4rc4/blackboardsync.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-06-26 15:12:27.000000 blackboardsync-0.9.4rc4/blackboardsync.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 15:12:27.000000 blackboardsync-0.9.4rc4/blackboardsync.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-06-26 15:12:27.000000 blackboardsync-0.9.4rc4/blackboardsync.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-26 15:12:27.000000 blackboardsync-0.9.4rc4/blackboardsync.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:12:27.364759 blackboardsync-0.9.4rc4/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-06-26 15:11:45.000000 blackboardsync-0.9.4rc4/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:12:27.364759 blackboardsync-0.9.4rc4/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-26 15:11:45.000000 blackboardsync-0.9.4rc4/docs/_static/custom.css
--rw-r--r--   0 runner    (1001) docker     (123)     3080 2023-06-26 15:11:45.000000 blackboardsync-0.9.4rc4/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:12:27.364759 blackboardsync-0.9.4rc4/docs/dev/
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-06-26 15:11:45.000000 blackboardsync-0.9.4rc4/docs/dev/bb_api.rst
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-26 15:11:45.000000 blackboardsync-0.9.4rc4/docs/dev/qt_api.rst
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-06-26 15:11:45.000000 blackboardsync-0.9.4rc4/docs/dev/sync_api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-06-26 15:11:45.000000 blackboardsync-0.9.4rc4/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-06-26 15:11:45.000000 blackboardsync-0.9.4rc4/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-06-26 15:11:45.000000 blackboardsync-0.9.4rc4/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:12:27.368759 blackboardsync-0.9.4rc4/packaging/
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-06-26 15:11:45.000000 blackboardsync-0.9.4rc4/packaging/pkg_macos.sh
--rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-06-26 15:11:45.000000 blackboardsync-0.9.4rc4/packaging/pkg_win.nsi
--rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-06-26 15:11:45.000000 blackboardsync-0.9.4rc4/packaging/pyinst.py
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-06-26 15:11:45.000000 blackboardsync-0.9.4rc4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 15:12:27.368759 blackboardsync-0.9.4rc4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:12:27.368759 blackboardsync-0.9.4rc4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 15:11:45.000000 blackboardsync-0.9.4rc4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3120 2023-06-26 15:11:45.000000 blackboardsync-0.9.4rc4/tests/strategies.py
--rw-r--r--   0 runner    (1001) docker     (123)     4589 2023-06-26 15:11:45.000000 blackboardsync-0.9.4rc4/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-06-26 15:11:45.000000 blackboardsync-0.9.4rc4/tests/test_blackboard.py
--rw-r--r--   0 runner    (1001) docker     (123)     5336 2023-06-26 15:11:45.000000 blackboardsync-0.9.4rc4/tests/test_download.py
--rw-r--r--   0 runner    (1001) docker     (123)    12154 2023-06-26 15:11:45.000000 blackboardsync-0.9.4rc4/tests/test_qt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-06-26 15:11:45.000000 blackboardsync-0.9.4rc4/tests/test_sync_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:01:39.754287 blackboardsync-0.9.5a1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:01:39.742287 blackboardsync-0.9.5a1/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-27 16:00:42.000000 blackboardsync-0.9.5a1/.github/FUNDING.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:01:39.742287 blackboardsync-0.9.5a1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)     2659 2023-06-27 16:00:42.000000 blackboardsync-0.9.5a1/.github/ISSUE_TEMPLATE/unisupport.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-06-27 16:00:42.000000 blackboardsync-0.9.5a1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:01:39.742287 blackboardsync-0.9.5a1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     3907 2023-06-27 16:00:42.000000 blackboardsync-0.9.5a1/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3291 2023-06-27 16:00:42.000000 blackboardsync-0.9.5a1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2892 2023-06-27 16:00:42.000000 blackboardsync-0.9.5a1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-06-27 16:00:42.000000 blackboardsync-0.9.5a1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-06-27 16:00:42.000000 blackboardsync-0.9.5a1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6046 2023-06-27 16:01:39.754287 blackboardsync-0.9.5a1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-06-27 16:00:42.000000 blackboardsync-0.9.5a1/Pipfile
+-rw-r--r--   0 runner    (1001) docker     (123)   107308 2023-06-27 16:00:42.000000 blackboardsync-0.9.5a1/Pipfile.lock
+-rw-r--r--   0 runner    (1001) docker     (123)     5382 2023-06-27 16:00:42.000000 blackboardsync-0.9.5a1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3265 2023-06-27 16:00:42.000000 blackboardsync-0.9.5a1/UNIVERSITIES.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:01:39.746287 blackboardsync-0.9.5a1/blackboard_sync/
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-06-27 16:00:42.000000 blackboardsync-0.9.5a1/blackboard_sync/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-06-27 16:00:42.000000 blackboardsync-0.9.5a1/blackboard_sync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-06-27 16:00:42.000000 blackboardsync-0.9.5a1/blackboard_sync/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:01:39.746287 blackboardsync-0.9.5a1/blackboard_sync/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-06-27 16:00:42.000000 blackboardsync-0.9.5a1/blackboard_sync/assets/alert.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-06-27 16:00:42.000000 blackboardsync-0.9.5a1/blackboard_sync/assets/alert.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   110234 2023-06-27 16:00:42.000000 blackboardsync-0.9.5a1/blackboard_sync/assets/logo.ico
+-rw-r--r--   0 runner    (1001) docker     (123)    31742 2023-06-27 16:00:42.000000 blackboardsync-0.9.5a1/blackboard_sync/assets/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    36877 2023-06-27 16:00:42.000000 blackboardsync-0.9.5a1/blackboard_sync/assets/watermark.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:01:39.746287 blackboardsync-0.9.5a1/blackboard_sync/blackboard/
+-rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-06-27 16:00:42.000000 blackboardsync-0.9.5a1/blackboard_sync/blackboard/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29665 2023-06-27 16:00:42.000000 blackboardsync-0.9.5a1/blackboard_sync/blackboard/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6003 2023-06-27 16:00:42.000000 blackboardsync-0.9.5a1/blackboard_sync/blackboard/blackboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3957 2023-06-27 16:00:42.000000 blackboardsync-0.9.5a1/blackboard_sync/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10622 2023-06-27 16:00:42.000000 blackboardsync-0.9.5a1/blackboard_sync/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4065 2023-06-27 16:00:42.000000 blackboardsync-0.9.5a1/blackboard_sync/institutions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:01:39.750287 blackboardsync-0.9.5a1/blackboard_sync/qt/
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-06-27 16:00:42.000000 blackboardsync-0.9.5a1/blackboard_sync/qt/LoginWebView.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     5032 2023-06-27 16:00:42.000000 blackboardsync-0.9.5a1/blackboard_sync/qt/PersistenceWarning.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     8488 2023-06-27 16:00:42.000000 blackboardsync-0.9.5a1/blackboard_sync/qt/SettingsWindow.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     6564 2023-06-27 16:00:42.000000 blackboardsync-0.9.5a1/blackboard_sync/qt/SetupWizard.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-06-27 16:00:42.000000 blackboardsync-0.9.5a1/blackboard_sync/qt/UniNotSupportedDialog.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-06-27 16:00:42.000000 blackboardsync-0.9.5a1/blackboard_sync/qt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21434 2023-06-27 16:00:42.000000 blackboardsync-0.9.5a1/blackboard_sync/qt/qt_elements.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10613 2023-06-27 16:00:42.000000 blackboardsync-0.9.5a1/blackboard_sync/sync.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7573 2023-06-27 16:00:42.000000 blackboardsync-0.9.5a1/blackboard_sync/sync_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13794 2023-06-27 16:00:42.000000 blackboardsync-0.9.5a1/blackboard_sync/universities.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-06-27 16:00:42.000000 blackboardsync-0.9.5a1/blackboard_sync/updates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-06-27 16:00:42.000000 blackboardsync-0.9.5a1/blackboard_sync/webdav.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:01:39.750287 blackboardsync-0.9.5a1/blackboardsync.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6046 2023-06-27 16:01:39.000000 blackboardsync-0.9.5a1/blackboardsync.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-06-27 16:01:39.000000 blackboardsync-0.9.5a1/blackboardsync.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 16:01:39.000000 blackboardsync-0.9.5a1/blackboardsync.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-06-27 16:01:39.000000 blackboardsync-0.9.5a1/blackboardsync.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-27 16:01:39.000000 blackboardsync-0.9.5a1/blackboardsync.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:01:39.750287 blackboardsync-0.9.5a1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-06-27 16:00:42.000000 blackboardsync-0.9.5a1/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:01:39.750287 blackboardsync-0.9.5a1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-27 16:00:42.000000 blackboardsync-0.9.5a1/docs/_static/custom.css
+-rw-r--r--   0 runner    (1001) docker     (123)     3080 2023-06-27 16:00:42.000000 blackboardsync-0.9.5a1/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:01:39.750287 blackboardsync-0.9.5a1/docs/dev/
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-06-27 16:00:42.000000 blackboardsync-0.9.5a1/docs/dev/bb_api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-27 16:00:42.000000 blackboardsync-0.9.5a1/docs/dev/qt_api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-06-27 16:00:42.000000 blackboardsync-0.9.5a1/docs/dev/sync_api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-06-27 16:00:42.000000 blackboardsync-0.9.5a1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-06-27 16:00:42.000000 blackboardsync-0.9.5a1/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-06-27 16:00:42.000000 blackboardsync-0.9.5a1/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:01:39.754287 blackboardsync-0.9.5a1/packaging/
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-06-27 16:00:42.000000 blackboardsync-0.9.5a1/packaging/pkg_macos.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     2757 2023-06-27 16:00:42.000000 blackboardsync-0.9.5a1/packaging/pkg_win.nsi
+-rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-06-27 16:00:42.000000 blackboardsync-0.9.5a1/packaging/pyinst.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-06-27 16:00:42.000000 blackboardsync-0.9.5a1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 16:01:39.754287 blackboardsync-0.9.5a1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 16:01:39.754287 blackboardsync-0.9.5a1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 16:00:42.000000 blackboardsync-0.9.5a1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3120 2023-06-27 16:00:42.000000 blackboardsync-0.9.5a1/tests/strategies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4589 2023-06-27 16:00:42.000000 blackboardsync-0.9.5a1/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-06-27 16:00:42.000000 blackboardsync-0.9.5a1/tests/test_blackboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5336 2023-06-27 16:00:42.000000 blackboardsync-0.9.5a1/tests/test_download.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12707 2023-06-27 16:00:42.000000 blackboardsync-0.9.5a1/tests/test_qt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-06-27 16:00:42.000000 blackboardsync-0.9.5a1/tests/test_sync_config.py
```

### Comparing `blackboardsync-0.9.4rc4/.github/ISSUE_TEMPLATE/unisupport.yml` & `blackboardsync-0.9.5a1/.github/ISSUE_TEMPLATE/unisupport.yml`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.4rc4/.github/workflows/build.yml` & `blackboardsync-0.9.5a1/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.4rc4/.gitignore` & `blackboardsync-0.9.5a1/.gitignore`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.4rc4/CHANGELOG.md` & `blackboardsync-0.9.5a1/CHANGELOG.md`

 * *Files 10% similar despite different names*

```diff
@@ -2,14 +2,26 @@
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
+## [0.9.5] - 2023-06-27
+
+### Added
+- Option to go over setup wizard again after initial setup
+
+### Fixed
+- Issue with session logging back in immediately after logout
+
+### Changed
+- Uninstalling the program in Windows will also delete user configuration
+
+
 ## [0.9.4] - 2023-06-26
 
 ### Added
 - Option to limit the courses downloaded by earliest creation date
 - Release notes from CHANGELOG
 
 ### Fixed
```

### Comparing `blackboardsync-0.9.4rc4/CONTRIBUTING.md` & `blackboardsync-0.9.5a1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.4rc4/LICENSE` & `blackboardsync-0.9.5a1/LICENSE`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.4rc4/PKG-INFO` & `blackboardsync-0.9.5a1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blackboardsync
-Version: 0.9.4rc4
+Version: 0.9.5a1
 Summary: Sync your blackboard content to your device
 Author-email: Jacob Sánchez <jacobszpz@protonmail.com>
 Project-URL: Homepage, https://bbsync.app
 Project-URL: Repository, https://github.com/jacobszpz/BlackboardSync
 Project-URL: Bug Tracker, https://github.com/jacobszpz/BlackboardSync/issues
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
```

### Comparing `blackboardsync-0.9.4rc4/Pipfile` & `blackboardsync-0.9.5a1/Pipfile`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.4rc4/Pipfile.lock` & `blackboardsync-0.9.5a1/Pipfile.lock`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.4rc4/README.md` & `blackboardsync-0.9.5a1/README.md`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.4rc4/UNIVERSITIES.md` & `blackboardsync-0.9.5a1/UNIVERSITIES.md`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.4rc4/blackboard_sync/__about__.py` & `blackboardsync-0.9.5a1/blackboard_sync/__about__.py`

 * *Files 9% similar despite different names*

```diff
@@ -29,14 +29,14 @@
     "__copyright__",
 ]
 
 __title__ = "BlackboardSync"
 __summary__ = "Automatic Syncing Of Your Blackboard Content"
 __uri__ = "https://github.com/jacobszpz/BlackboardSync"
 
-__version__ = "0.9.4-rc.4"
+__version__ = "0.9.5-alpha.1"
 
 __author__ = "Jacob Sánchez"
 __email__ = "jacobszpz@protonmail.com"
 
 __license__ = "GNU General Public License v2"
 __copyright__ = f"2023, {__author__}"
```

### Comparing `blackboardsync-0.9.4rc4/blackboard_sync/__init__.py` & `blackboardsync-0.9.5a1/blackboard_sync/__init__.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.4rc4/blackboard_sync/__main__.py` & `blackboardsync-0.9.5a1/blackboard_sync/__main__.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.4rc4/blackboard_sync/assets/alert.png` & `blackboardsync-0.9.5a1/blackboard_sync/assets/alert.png`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.4rc4/blackboard_sync/assets/alert.svg` & `blackboardsync-0.9.5a1/blackboard_sync/assets/alert.svg`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.4rc4/blackboard_sync/assets/logo.ico` & `blackboardsync-0.9.5a1/blackboard_sync/assets/logo.ico`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.4rc4/blackboard_sync/assets/logo.png` & `blackboardsync-0.9.5a1/blackboard_sync/assets/logo.png`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.4rc4/blackboard_sync/assets/watermark.png` & `blackboardsync-0.9.5a1/blackboard_sync/assets/watermark.png`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.4rc4/blackboard_sync/blackboard/__init__.py` & `blackboardsync-0.9.5a1/blackboard_sync/blackboard/__init__.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.4rc4/blackboard_sync/blackboard/api.py` & `blackboardsync-0.9.5a1/blackboard_sync/blackboard/api.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.4rc4/blackboard_sync/blackboard/blackboard.py` & `blackboardsync-0.9.5a1/blackboard_sync/blackboard/blackboard.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.4rc4/blackboard_sync/config.py` & `blackboardsync-0.9.5a1/blackboard_sync/config.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.4rc4/blackboard_sync/download.py` & `blackboardsync-0.9.5a1/blackboard_sync/download.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.4rc4/blackboard_sync/institutions.py` & `blackboardsync-0.9.5a1/blackboard_sync/institutions.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.4rc4/blackboard_sync/qt/LoginWebView.ui` & `blackboardsync-0.9.5a1/blackboard_sync/qt/LoginWebView.ui`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.4rc4/blackboard_sync/qt/PersistenceWarning.ui` & `blackboardsync-0.9.5a1/blackboard_sync/qt/PersistenceWarning.ui`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.4rc4/blackboard_sync/qt/SettingsWindow.ui` & `blackboardsync-0.9.5a1/blackboard_sync/qt/SettingsWindow.ui`

 * *Files 2% similar despite different names*

#### Comparing `blackboardsync-0.9.4rc4/blackboard_sync/qt/SettingsWindow.ui` & `blackboardsync-0.9.5a1/blackboard_sync/qt/SettingsWindow.ui`

```diff
@@ -122,15 +122,15 @@
               </property>
               <property name="sizeType">
                 <enum>QSizePolicy::Fixed</enum>
               </property>
               <property name="sizeHint" stdset="0">
                 <size>
                   <width>0</width>
-                  <height>18</height>
+                  <height>12</height>
                 </size>
               </property>
             </spacer>
           </item>
           <item>
             <widget class="QLabel" name="frequency_label">
               <property name="font">
@@ -179,15 +179,15 @@
               </property>
               <property name="sizeType">
                 <enum>QSizePolicy::Fixed</enum>
               </property>
               <property name="sizeHint" stdset="0">
                 <size>
                   <width>0</width>
-                  <height>18</height>
+                  <height>12</height>
                 </size>
               </property>
             </spacer>
           </item>
           <item>
             <widget class="QLabel" name="session_label">
               <property name="font">
@@ -214,38 +214,55 @@
               </property>
               <property name="text">
                 <string>Logged in as</string>
               </property>
             </widget>
           </item>
           <item>
-            <widget class="QPushButton" name="log_out_button">
-              <property name="font">
-                <font>
-                  <family>Open Sans</family>
-                  <pointsize>11</pointsize>
-                </font>
-              </property>
-              <property name="text">
-                <string>Log Out</string>
-              </property>
-            </widget>
+            <layout class="QHBoxLayout" name="horizontalLayout_2">
+              <item>
+                <widget class="QPushButton" name="log_out_button">
+                  <property name="font">
+                    <font>
+                      <family>Open Sans</family>
+                      <pointsize>11</pointsize>
+                    </font>
+                  </property>
+                  <property name="text">
+                    <string>Log Out</string>
+                  </property>
+                </widget>
+              </item>
+              <item>
+                <widget class="QPushButton" name="setup_button">
+                  <property name="font">
+                    <font>
+                      <family>Open Sans</family>
+                      <pointsize>11</pointsize>
+                    </font>
+                  </property>
+                  <property name="text">
+                    <string>Setup Wizard</string>
+                  </property>
+                </widget>
+              </item>
+            </layout>
           </item>
           <item>
             <spacer name="verticalSpacer_4">
               <property name="orientation">
                 <enum>Qt::Vertical</enum>
               </property>
               <property name="sizeType">
                 <enum>QSizePolicy::Fixed</enum>
               </property>
               <property name="sizeHint" stdset="0">
                 <size>
                   <width>0</width>
-                  <height>27</height>
+                  <height>24</height>
                 </size>
               </property>
             </spacer>
           </item>
           <item>
             <widget class="QDialogButtonBox" name="button_box">
               <property name="font">
```

### Comparing `blackboardsync-0.9.4rc4/blackboard_sync/qt/SetupWizard.ui` & `blackboardsync-0.9.5a1/blackboard_sync/qt/SetupWizard.ui`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.4rc4/blackboard_sync/qt/UniNotSupportedDialog.ui` & `blackboardsync-0.9.5a1/blackboard_sync/qt/UniNotSupportedDialog.ui`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.4rc4/blackboard_sync/qt/__init__.py` & `blackboardsync-0.9.5a1/blackboard_sync/qt/__init__.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.4rc4/blackboard_sync/qt/qt_elements.py` & `blackboardsync-0.9.5a1/blackboard_sync/qt/qt_elements.py`

 * *Files 2% similar despite different names*

```diff
@@ -160,22 +160,26 @@
         self._status = QAction(self._unauthenticated_status)
         self._status.setEnabled(False)
         self.addAction(self._status)
 
         self.log_in = QAction("Log In")
         self.addAction(self.log_in)
 
+        self.reset_setup = QAction("Redo Setup")
+        self.addAction(self.reset_setup)
+
         self.quit = QAction("Quit")
         self.quit.setIcon(close_icon)
         self.addAction(self.quit)
 
     def set_logged_in(self, logged: bool) -> None:
         """Set the UI to reflect logged-in status."""
         self.refresh.setVisible(logged)
         self.preferences.setVisible(logged)
+        self.reset_setup.setVisible(not logged)
         self.open_dir.setVisible(logged)
         self.log_in.setVisible(not logged)
 
         if logged:
             self._status.setText(f"Last Synced: {self._last_synced}")
         else:
             self._status.setText("Not Logged In")
@@ -196,14 +200,15 @@
 class SyncTrayIcon(QSystemTrayIcon):
     """BlackboardSync system tray icon."""
 
     _tooltip = "Blackboard Sync"
     _sync_signal = pyqtSignal()
     _login_signal = pyqtSignal()
     _settings_signal = pyqtSignal()
+    _reset_setup_signal = pyqtSignal()
     _quit_signal = pyqtSignal()
     _open_dir_signal = pyqtSignal()
     _show_menu_signal = pyqtSignal()
 
     def __init__(self):
         """Create a `QSystemTrayIcon`."""
         super().__init__()
@@ -219,14 +224,15 @@
 
         # Create the menu
         self._menu = SyncTrayMenu()
 
         self._sync_signal = self._menu.refresh.triggered
         self._login_signal = self._menu.log_in.triggered
         self._settings_signal = self._menu.preferences.triggered
+        self._reset_setup_signal = self._menu.reset_setup.triggered
         self._quit_signal = self._menu.quit.triggered
         self._open_dir_signal = self._menu.open_dir.triggered
         self._show_menu_signal = self._menu.aboutToShow
 
         # Add the menu to the tray
         self.setContextMenu(self._menu)
         self.setToolTip(self._tooltip)
@@ -265,14 +271,19 @@
 
     @property
     def settings_signal(self):
         """Fire when the settings menu is opened."""
         return self._settings_signal
 
     @property
+    def reset_setup_signal(self):
+        """Fire when the user wants to reset the initial setup."""
+        return self._reset_setup_signal
+
+    @property
     def quit_signal(self):
         """Fire once user decides to quit app."""
         return self._quit_signal
 
     @property
     def open_dir_signal(self):
         """Fire once user wants to open download directory."""
@@ -359,14 +370,15 @@
 
 class SettingsWindow(QWidget):
     """Settings windown UI element."""
 
     _window_title = "Settings"
     _initial_position = (300, 300)
     _log_out_signal = pyqtSignal()
+    _setup_wiz_signal = pyqtSignal()
     _save_signal = pyqtSignal()
 
     def __init__(self):
         """Create instance of SettingsWindow."""
         super().__init__()
         self._init_ui()
 
@@ -374,14 +386,15 @@
         Assets.load_ui(self)
 
         self.move(*self._initial_position)
         self.setWindowTitle(self._window_title)
 
         self.select_download_location.clicked.connect(self._choose_location)
         self._log_out_signal = self.log_out_button.clicked
+        self._setup_wiz_signal = self.setup_button.clicked
         self._save_signal = self.button_box.accepted
 
     def _choose_location(self) -> None:
         if (location := self._file_chooser_dialog()):
             self.download_location = location
 
     def _file_chooser_dialog(self) -> Optional[Path]:
@@ -427,14 +440,19 @@
 
     @property
     def log_out_signal(self):
         """Fire when user chooses to log out."""
         return self._log_out_signal
 
     @property
+    def setup_wiz_signal(self):
+        """Fire when user wants to redo initial setup."""
+        return self._setup_wiz_signal
+
+    @property
     def save_signal(self):
         """Fire when settings are saved."""
         return self._save_signal
 
 
 class LoginWindow(QWidget):
     """Deprecated widget previously used to login."""
@@ -470,14 +488,15 @@
             cookie.value().data().decode(),
             domain=cookie.domain(),
             path=cookie.path(),
             secure=cookie.isSecure()
         )
 
     def restore(self) -> None:
+        self.web_view.setPage(None)
         self.clear_cookie_store()
         self.web_view.load(QUrl.fromUserInput(self.start_url))
 
     def clear_cookie_store(self) -> None:
         """Clear the HTTP cache and cookies."""
         self._cookie_store.deleteAllCookies()
         self._engine_profile.clearHttpCache()
```

### Comparing `blackboardsync-0.9.4rc4/blackboard_sync/sync.py` & `blackboardsync-0.9.5a1/blackboard_sync/sync.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.4rc4/blackboard_sync/sync_controller.py` & `blackboardsync-0.9.5a1/blackboard_sync/sync_controller.py`

 * *Files 4% similar despite different names*

```diff
@@ -63,20 +63,22 @@
         self.setup_window.accepted.connect(self._setup_complete)
 
         self.login_window = None
 
         self.config_window = SettingsWindow()
 
         self.config_window.log_out_signal.connect(self._log_out)
+        self.config_window.setup_wiz_signal.connect(self._reset_setup)
         self.config_window.save_signal.connect(self._save_setting_changes)
 
         self.tray = SyncTrayIcon()
         self.tray.quit_signal.connect(self._stop)
         self.tray.login_signal.connect(self._show_login_window)
         self.tray.settings_signal.connect(self._show_config_window)
+        self.tray.reset_setup_signal.connect(self._reset_setup)
         self.tray.sync_signal.connect(self._force_sync)
         self.tray.activated.connect(self._tray_icon_activated)
         self.tray.open_dir_signal.connect(self._open_download_dir)
         self.tray.show_menu_signal.connect(self._update_tray_menu)
 
         self.app.setQuitOnLastWindowClosed(False)
 
@@ -100,14 +102,21 @@
         auth = self.model.auth(self.login_window.cookie_jar)
         self.tray.set_logged_in(auth)
         self.login_window.setVisible(False)
         self.app.restoreOverrideCursor()
         self._check_for_updates()
         self.tray.show_msg('The download has started', 'BlackboardSync is running in the background. Find it in the system tray.')
 
+    def _reset_setup(self) -> None:
+        # Hide login window and show setup wizard
+        if self.login_window is not None:
+            self._log_out()
+            self.login_window.setVisible(False)
+        self._show_setup_window()
+
     def _check_for_updates(self) -> None:
         if (html_url := check_for_updates()) is not None:
             if UpdateFoundDialog().update:
                 webbrowser.open(html_url)
 
     def _show_login_window(self) -> None:
         if self.login_window is not None:
@@ -137,14 +146,17 @@
             if self.model.university is None:
                 self._show_setup_window()
             # if not logged in
             elif not self.model.is_logged_in:
                 self._show_login_window()
 
     def _log_out(self) -> None:
+        if self.model.is_active:
+            self.model.stop_sync()
+
         self.model.log_out()
         self.tray.set_logged_in(False)
         self.login_window.restore()
         self.login_window.setVisible(True)
         self.config_window.setVisible(False)
 
     def _save_setting_changes(self) -> None:
```

### Comparing `blackboardsync-0.9.4rc4/blackboard_sync/universities.json` & `blackboardsync-0.9.5a1/blackboard_sync/universities.json`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.4rc4/blackboard_sync/updates.py` & `blackboardsync-0.9.5a1/blackboard_sync/updates.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.4rc4/blackboard_sync/webdav.py` & `blackboardsync-0.9.5a1/blackboard_sync/webdav.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.4rc4/blackboardsync.egg-info/PKG-INFO` & `blackboardsync-0.9.5a1/blackboardsync.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blackboardsync
-Version: 0.9.4rc4
+Version: 0.9.5a1
 Summary: Sync your blackboard content to your device
 Author-email: Jacob Sánchez <jacobszpz@protonmail.com>
 Project-URL: Homepage, https://bbsync.app
 Project-URL: Repository, https://github.com/jacobszpz/BlackboardSync
 Project-URL: Bug Tracker, https://github.com/jacobszpz/BlackboardSync/issues
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
```

### Comparing `blackboardsync-0.9.4rc4/blackboardsync.egg-info/SOURCES.txt` & `blackboardsync-0.9.5a1/blackboardsync.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.4rc4/docs/Makefile` & `blackboardsync-0.9.5a1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.4rc4/docs/conf.py` & `blackboardsync-0.9.5a1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.4rc4/docs/index.rst` & `blackboardsync-0.9.5a1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.4rc4/docs/make.bat` & `blackboardsync-0.9.5a1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.4rc4/main.py` & `blackboardsync-0.9.5a1/main.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.4rc4/packaging/pkg_macos.sh` & `blackboardsync-0.9.5a1/packaging/pkg_macos.sh`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.4rc4/packaging/pkg_win.nsi` & `blackboardsync-0.9.5a1/packaging/pkg_win.nsi`

 * *Files 2% similar despite different names*

```diff
@@ -67,15 +67,15 @@
     WriteRegStr HKCU ${UNINSTALL_REGKEY} "DisplayVersion" ${VERSION}
 
     WriteUninstaller "$INSTDIR\Uninstall.exe"
 SectionEnd
 
 
 Section "Uninstall"
-  # TODO: Add User Data if Chosen
+  Delete "$APPDATA\blackboard_sync"
 
   ; Remove Application
   RMDir /r $INSTDIR
 
   ; Run on Startup
   DeleteRegKey HKCU "Software\Microsoft\Windows\CurrentVersion\Run\BlackboardSync"
```

### Comparing `blackboardsync-0.9.4rc4/packaging/pyinst.py` & `blackboardsync-0.9.5a1/packaging/pyinst.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.4rc4/pyproject.toml` & `blackboardsync-0.9.5a1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.4rc4/tests/strategies.py` & `blackboardsync-0.9.5a1/tests/strategies.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.4rc4/tests/test_api.py` & `blackboardsync-0.9.5a1/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.4rc4/tests/test_blackboard.py` & `blackboardsync-0.9.5a1/tests/test_blackboard.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.4rc4/tests/test_download.py` & `blackboardsync-0.9.5a1/tests/test_download.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.4rc4/tests/test_qt.py` & `blackboardsync-0.9.5a1/tests/test_qt.py`

 * *Files 1% similar despite different names*

```diff
@@ -226,14 +226,22 @@
     def test_settings_window_log_out_signal(self, qtbot, settings_window):
         qtbot.addWidget(settings_window)
 
         with qtbot.waitSignal(settings_window.log_out_signal) as blocker:
             qtbot.mouseClick(settings_window.log_out_button, QtCore.Qt.LeftButton)
 
         assert blocker.signal_triggered
+    
+    def test_settings_window_setup_wizard_signal(self, qtbot, settings_window):
+        qtbot.addWidget(settings_window)
+
+        with qtbot.waitSignal(settings_window.setup_wiz_signal) as blocker:
+            qtbot.mouseClick(settings_window.setup_button, QtCore.Qt.LeftButton)
+
+        assert blocker.signal_triggered
 
     def test_settings_window_save_signal(self, qtbot, settings_window):
         qtbot.addWidget(settings_window)
 
         with qtbot.waitSignal(settings_window.save_signal) as blocker:
             qtbot.mouseClick(settings_window.button_box.button(QDialogButtonBox.Save),
                              QtCore.Qt.LeftButton)
@@ -271,14 +279,20 @@
 
     def test_tray_icon_login_signal(self, qtbot, tray_icon):
         with qtbot.waitSignal(tray_icon.login_signal) as blocker:
             tray_icon._menu.log_in.trigger()
 
         assert blocker.signal_triggered
 
+    def test_tray_icon_setupwiz_signal(self, qtbot, tray_icon):
+        with qtbot.waitSignal(tray_icon.reset_setup_signal) as blocker:
+            tray_icon._menu.reset_setup.trigger()
+
+        assert blocker.signal_triggered
+
     def test_tray_icon_quit_signal(self, qtbot, tray_icon):
         with qtbot.waitSignal(tray_icon.quit_signal) as blocker:
             tray_icon._menu.quit.trigger()
 
         assert blocker.signal_triggered
 
     def test_tray_icon_settings_signal(self, qtbot, tray_icon):
```

### Comparing `blackboardsync-0.9.4rc4/tests/test_sync_config.py` & `blackboardsync-0.9.5a1/tests/test_sync_config.py`

 * *Files identical despite different names*

