# Comparing `tmp/blackboardsync-0.9.5.tar.gz` & `tmp/blackboardsync-0.9.5a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blackboardsync-0.9.5.tar", last modified: Tue Jun 27 17:09:45 2023, max compression
+gzip compressed data, was "blackboardsync-0.9.5a1.tar", last modified: Tue Jun 27 16:01:39 2023, max compression
```

## Comparing `blackboardsync-0.9.5.tar` & `blackboardsync-0.9.5a1.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:09:45.533728 blackboardsync-0.9.5/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:09:45.525728 blackboardsync-0.9.5/.github/
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-27 17:09:03.000000 blackboardsync-0.9.5/.github/FUNDING.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:09:45.525728 blackboardsync-0.9.5/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)     2659 2023-06-27 17:09:03.000000 blackboardsync-0.9.5/.github/ISSUE_TEMPLATE/unisupport.yml
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-06-27 17:09:03.000000 blackboardsync-0.9.5/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:09:45.525728 blackboardsync-0.9.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     3907 2023-06-27 17:09:03.000000 blackboardsync-0.9.5/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3291 2023-06-27 17:09:03.000000 blackboardsync-0.9.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     2892 2023-06-27 17:09:03.000000 blackboardsync-0.9.5/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-06-27 17:09:03.000000 blackboardsync-0.9.5/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-06-27 17:09:03.000000 blackboardsync-0.9.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6044 2023-06-27 17:09:45.529728 blackboardsync-0.9.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-06-27 17:09:03.000000 blackboardsync-0.9.5/Pipfile
--rw-r--r--   0 runner    (1001) docker     (123)   107308 2023-06-27 17:09:03.000000 blackboardsync-0.9.5/Pipfile.lock
--rw-r--r--   0 runner    (1001) docker     (123)     5382 2023-06-27 17:09:03.000000 blackboardsync-0.9.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3265 2023-06-27 17:09:03.000000 blackboardsync-0.9.5/UNIVERSITIES.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:09:45.525728 blackboardsync-0.9.5/blackboard_sync/
--rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-06-27 17:09:03.000000 blackboardsync-0.9.5/blackboard_sync/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-06-27 17:09:03.000000 blackboardsync-0.9.5/blackboard_sync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-06-27 17:09:03.000000 blackboardsync-0.9.5/blackboard_sync/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:09:45.525728 blackboardsync-0.9.5/blackboard_sync/assets/
--rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-06-27 17:09:03.000000 blackboardsync-0.9.5/blackboard_sync/assets/alert.png
--rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-06-27 17:09:03.000000 blackboardsync-0.9.5/blackboard_sync/assets/alert.svg
--rw-r--r--   0 runner    (1001) docker     (123)   110234 2023-06-27 17:09:03.000000 blackboardsync-0.9.5/blackboard_sync/assets/logo.ico
--rw-r--r--   0 runner    (1001) docker     (123)    31742 2023-06-27 17:09:03.000000 blackboardsync-0.9.5/blackboard_sync/assets/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)    36877 2023-06-27 17:09:03.000000 blackboardsync-0.9.5/blackboard_sync/assets/watermark.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:09:45.525728 blackboardsync-0.9.5/blackboard_sync/blackboard/
--rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-06-27 17:09:03.000000 blackboardsync-0.9.5/blackboard_sync/blackboard/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29665 2023-06-27 17:09:03.000000 blackboardsync-0.9.5/blackboard_sync/blackboard/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6003 2023-06-27 17:09:03.000000 blackboardsync-0.9.5/blackboard_sync/blackboard/blackboard.py
--rw-r--r--   0 runner    (1001) docker     (123)     3957 2023-06-27 17:09:03.000000 blackboardsync-0.9.5/blackboard_sync/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    10622 2023-06-27 17:09:03.000000 blackboardsync-0.9.5/blackboard_sync/download.py
--rw-r--r--   0 runner    (1001) docker     (123)     4065 2023-06-27 17:09:03.000000 blackboardsync-0.9.5/blackboard_sync/institutions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:09:45.529728 blackboardsync-0.9.5/blackboard_sync/qt/
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-06-27 17:09:03.000000 blackboardsync-0.9.5/blackboard_sync/qt/LoginWebView.ui
--rw-r--r--   0 runner    (1001) docker     (123)     5032 2023-06-27 17:09:03.000000 blackboardsync-0.9.5/blackboard_sync/qt/PersistenceWarning.ui
--rw-r--r--   0 runner    (1001) docker     (123)     8488 2023-06-27 17:09:03.000000 blackboardsync-0.9.5/blackboard_sync/qt/SettingsWindow.ui
--rw-r--r--   0 runner    (1001) docker     (123)     6564 2023-06-27 17:09:03.000000 blackboardsync-0.9.5/blackboard_sync/qt/SetupWizard.ui
--rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-06-27 17:09:03.000000 blackboardsync-0.9.5/blackboard_sync/qt/UniNotSupportedDialog.ui
--rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-06-27 17:09:03.000000 blackboardsync-0.9.5/blackboard_sync/qt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21434 2023-06-27 17:09:03.000000 blackboardsync-0.9.5/blackboard_sync/qt/qt_elements.py
--rw-r--r--   0 runner    (1001) docker     (123)    10613 2023-06-27 17:09:03.000000 blackboardsync-0.9.5/blackboard_sync/sync.py
--rw-r--r--   0 runner    (1001) docker     (123)     7573 2023-06-27 17:09:03.000000 blackboardsync-0.9.5/blackboard_sync/sync_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)    13794 2023-06-27 17:09:03.000000 blackboardsync-0.9.5/blackboard_sync/universities.json
--rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-06-27 17:09:03.000000 blackboardsync-0.9.5/blackboard_sync/updates.py
--rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-06-27 17:09:03.000000 blackboardsync-0.9.5/blackboard_sync/webdav.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:09:45.529728 blackboardsync-0.9.5/blackboardsync.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6044 2023-06-27 17:09:45.000000 blackboardsync-0.9.5/blackboardsync.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-06-27 17:09:45.000000 blackboardsync-0.9.5/blackboardsync.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 17:09:45.000000 blackboardsync-0.9.5/blackboardsync.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-06-27 17:09:45.000000 blackboardsync-0.9.5/blackboardsync.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-27 17:09:45.000000 blackboardsync-0.9.5/blackboardsync.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:09:45.529728 blackboardsync-0.9.5/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-06-27 17:09:03.000000 blackboardsync-0.9.5/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:09:45.529728 blackboardsync-0.9.5/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-27 17:09:03.000000 blackboardsync-0.9.5/docs/_static/custom.css
--rw-r--r--   0 runner    (1001) docker     (123)     3080 2023-06-27 17:09:03.000000 blackboardsync-0.9.5/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:09:45.529728 blackboardsync-0.9.5/docs/dev/
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-06-27 17:09:03.000000 blackboardsync-0.9.5/docs/dev/bb_api.rst
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-27 17:09:03.000000 blackboardsync-0.9.5/docs/dev/qt_api.rst
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-06-27 17:09:03.000000 blackboardsync-0.9.5/docs/dev/sync_api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-06-27 17:09:03.000000 blackboardsync-0.9.5/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-06-27 17:09:03.000000 blackboardsync-0.9.5/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-06-27 17:09:03.000000 blackboardsync-0.9.5/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:09:45.529728 blackboardsync-0.9.5/packaging/
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-06-27 17:09:03.000000 blackboardsync-0.9.5/packaging/pkg_macos.sh
--rw-r--r--   0 runner    (1001) docker     (123)     2757 2023-06-27 17:09:03.000000 blackboardsync-0.9.5/packaging/pkg_win.nsi
--rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-06-27 17:09:03.000000 blackboardsync-0.9.5/packaging/pyinst.py
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-06-27 17:09:03.000000 blackboardsync-0.9.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 17:09:45.533728 blackboardsync-0.9.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:09:45.529728 blackboardsync-0.9.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 17:09:03.000000 blackboardsync-0.9.5/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3120 2023-06-27 17:09:03.000000 blackboardsync-0.9.5/tests/strategies.py
--rw-r--r--   0 runner    (1001) docker     (123)     4589 2023-06-27 17:09:03.000000 blackboardsync-0.9.5/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-06-27 17:09:03.000000 blackboardsync-0.9.5/tests/test_blackboard.py
--rw-r--r--   0 runner    (1001) docker     (123)     5336 2023-06-27 17:09:03.000000 blackboardsync-0.9.5/tests/test_download.py
--rw-r--r--   0 runner    (1001) docker     (123)    12707 2023-06-27 17:09:03.000000 blackboardsync-0.9.5/tests/test_qt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-06-27 17:09:03.000000 blackboardsync-0.9.5/tests/test_sync_config.py
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

### Comparing `blackboardsync-0.9.5/.github/ISSUE_TEMPLATE/unisupport.yml` & `blackboardsync-0.9.5a1/.github/ISSUE_TEMPLATE/unisupport.yml`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.5/.github/workflows/build.yml` & `blackboardsync-0.9.5a1/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.5/.gitignore` & `blackboardsync-0.9.5a1/.gitignore`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.5/CHANGELOG.md` & `blackboardsync-0.9.5a1/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.5/CONTRIBUTING.md` & `blackboardsync-0.9.5a1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.5/LICENSE` & `blackboardsync-0.9.5a1/LICENSE`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.5/PKG-INFO` & `blackboardsync-0.9.5a1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blackboardsync
-Version: 0.9.5
+Version: 0.9.5a1
 Summary: Sync your blackboard content to your device
 Author-email: Jacob Sánchez <jacobszpz@protonmail.com>
 Project-URL: Homepage, https://bbsync.app
 Project-URL: Repository, https://github.com/jacobszpz/BlackboardSync
 Project-URL: Bug Tracker, https://github.com/jacobszpz/BlackboardSync/issues
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
```

### Comparing `blackboardsync-0.9.5/Pipfile` & `blackboardsync-0.9.5a1/Pipfile`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.5/Pipfile.lock` & `blackboardsync-0.9.5a1/Pipfile.lock`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.5/README.md` & `blackboardsync-0.9.5a1/README.md`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.5/UNIVERSITIES.md` & `blackboardsync-0.9.5a1/UNIVERSITIES.md`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.5/blackboard_sync/__about__.py` & `blackboardsync-0.9.5a1/blackboard_sync/__about__.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,14 +29,14 @@
     "__copyright__",
 ]
 
 __title__ = "BlackboardSync"
 __summary__ = "Automatic Syncing Of Your Blackboard Content"
 __uri__ = "https://github.com/jacobszpz/BlackboardSync"
 
-__version__ = "0.9.5"
+__version__ = "0.9.5-alpha.1"
 
 __author__ = "Jacob Sánchez"
 __email__ = "jacobszpz@protonmail.com"
 
 __license__ = "GNU General Public License v2"
 __copyright__ = f"2023, {__author__}"
```

### Comparing `blackboardsync-0.9.5/blackboard_sync/__init__.py` & `blackboardsync-0.9.5a1/blackboard_sync/__init__.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.5/blackboard_sync/__main__.py` & `blackboardsync-0.9.5a1/blackboard_sync/__main__.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.5/blackboard_sync/assets/alert.png` & `blackboardsync-0.9.5a1/blackboard_sync/assets/alert.png`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.5/blackboard_sync/assets/alert.svg` & `blackboardsync-0.9.5a1/blackboard_sync/assets/alert.svg`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.5/blackboard_sync/assets/logo.ico` & `blackboardsync-0.9.5a1/blackboard_sync/assets/logo.ico`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.5/blackboard_sync/assets/logo.png` & `blackboardsync-0.9.5a1/blackboard_sync/assets/logo.png`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.5/blackboard_sync/assets/watermark.png` & `blackboardsync-0.9.5a1/blackboard_sync/assets/watermark.png`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.5/blackboard_sync/blackboard/__init__.py` & `blackboardsync-0.9.5a1/blackboard_sync/blackboard/__init__.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.5/blackboard_sync/blackboard/api.py` & `blackboardsync-0.9.5a1/blackboard_sync/blackboard/api.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.5/blackboard_sync/blackboard/blackboard.py` & `blackboardsync-0.9.5a1/blackboard_sync/blackboard/blackboard.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.5/blackboard_sync/config.py` & `blackboardsync-0.9.5a1/blackboard_sync/config.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.5/blackboard_sync/download.py` & `blackboardsync-0.9.5a1/blackboard_sync/download.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.5/blackboard_sync/institutions.py` & `blackboardsync-0.9.5a1/blackboard_sync/institutions.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.5/blackboard_sync/qt/LoginWebView.ui` & `blackboardsync-0.9.5a1/blackboard_sync/qt/LoginWebView.ui`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.5/blackboard_sync/qt/PersistenceWarning.ui` & `blackboardsync-0.9.5a1/blackboard_sync/qt/PersistenceWarning.ui`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.5/blackboard_sync/qt/SettingsWindow.ui` & `blackboardsync-0.9.5a1/blackboard_sync/qt/SettingsWindow.ui`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.5/blackboard_sync/qt/SetupWizard.ui` & `blackboardsync-0.9.5a1/blackboard_sync/qt/SetupWizard.ui`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.5/blackboard_sync/qt/UniNotSupportedDialog.ui` & `blackboardsync-0.9.5a1/blackboard_sync/qt/UniNotSupportedDialog.ui`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.5/blackboard_sync/qt/__init__.py` & `blackboardsync-0.9.5a1/blackboard_sync/qt/__init__.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.5/blackboard_sync/qt/qt_elements.py` & `blackboardsync-0.9.5a1/blackboard_sync/qt/qt_elements.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.5/blackboard_sync/sync.py` & `blackboardsync-0.9.5a1/blackboard_sync/sync.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.5/blackboard_sync/sync_controller.py` & `blackboardsync-0.9.5a1/blackboard_sync/sync_controller.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.5/blackboard_sync/universities.json` & `blackboardsync-0.9.5a1/blackboard_sync/universities.json`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.5/blackboard_sync/updates.py` & `blackboardsync-0.9.5a1/blackboard_sync/updates.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.5/blackboard_sync/webdav.py` & `blackboardsync-0.9.5a1/blackboard_sync/webdav.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.5/blackboardsync.egg-info/PKG-INFO` & `blackboardsync-0.9.5a1/blackboardsync.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blackboardsync
-Version: 0.9.5
+Version: 0.9.5a1
 Summary: Sync your blackboard content to your device
 Author-email: Jacob Sánchez <jacobszpz@protonmail.com>
 Project-URL: Homepage, https://bbsync.app
 Project-URL: Repository, https://github.com/jacobszpz/BlackboardSync
 Project-URL: Bug Tracker, https://github.com/jacobszpz/BlackboardSync/issues
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
```

### Comparing `blackboardsync-0.9.5/blackboardsync.egg-info/SOURCES.txt` & `blackboardsync-0.9.5a1/blackboardsync.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.5/docs/Makefile` & `blackboardsync-0.9.5a1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.5/docs/conf.py` & `blackboardsync-0.9.5a1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.5/docs/index.rst` & `blackboardsync-0.9.5a1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.5/docs/make.bat` & `blackboardsync-0.9.5a1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.5/main.py` & `blackboardsync-0.9.5a1/main.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.5/packaging/pkg_macos.sh` & `blackboardsync-0.9.5a1/packaging/pkg_macos.sh`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.5/packaging/pkg_win.nsi` & `blackboardsync-0.9.5a1/packaging/pkg_win.nsi`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.5/packaging/pyinst.py` & `blackboardsync-0.9.5a1/packaging/pyinst.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.5/pyproject.toml` & `blackboardsync-0.9.5a1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.5/tests/strategies.py` & `blackboardsync-0.9.5a1/tests/strategies.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.5/tests/test_api.py` & `blackboardsync-0.9.5a1/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.5/tests/test_blackboard.py` & `blackboardsync-0.9.5a1/tests/test_blackboard.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.5/tests/test_download.py` & `blackboardsync-0.9.5a1/tests/test_download.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.5/tests/test_qt.py` & `blackboardsync-0.9.5a1/tests/test_qt.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.5/tests/test_sync_config.py` & `blackboardsync-0.9.5a1/tests/test_sync_config.py`

 * *Files identical despite different names*

