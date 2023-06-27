# Comparing `tmp/mgtron-2.17.1.tar.gz` & `tmp/mgtron-2.18.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mgtron-2.17.1.tar", last modified: Tue Jun 20 15:46:57 2023, max compression
+gzip compressed data, was "mgtron-2.18.0.tar", last modified: Tue Jun 27 20:26:08 2023, max compression
```

## Comparing `mgtron-2.17.1.tar` & `mgtron-2.18.0.tar`

### file list

```diff
@@ -1,101 +1,112 @@
-drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-20 15:46:57.837773 mgtron-2.17.1/
-drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-20 15:46:57.827773 mgtron-2.17.1/.github/
-drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-20 15:46:57.827773 mgtron-2.17.1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      602 2023-06-09 13:32:26.000000 mgtron-2.17.1/.github/ISSUE_TEMPLATE/mgtron--.md
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     1524 2023-06-09 13:32:26.000000 mgtron-2.17.1/.github/ISSUE_TEMPLATE/mgtron_issue.yml
-drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-20 15:46:57.827773 mgtron-2.17.1/.github/workflows/
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      457 2023-06-09 13:32:26.000000 mgtron-2.17.1/.github/workflows/black_actions.yml
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      365 2023-06-19 20:47:25.000000 mgtron-2.17.1/.gitignore
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     7807 2023-06-20 15:44:45.000000 mgtron-2.17.1/CHANGELOG.md
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      957 2023-06-19 20:47:25.000000 mgtron-2.17.1/LICENSE.rst
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)    12098 2023-06-20 15:46:57.837773 mgtron-2.17.1/PKG-INFO
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     3794 2023-06-19 20:47:25.000000 mgtron-2.17.1/README.md
-drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-20 15:46:57.827773 mgtron-2.17.1/docs/
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)    17614 2023-06-09 13:32:26.000000 mgtron-2.17.1/docs/MGTron Command Description.docx
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)    23088 2023-06-09 13:32:26.000000 mgtron-2.17.1/docs/MGTron Function Descriptions.docx
-drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-20 15:46:57.827773 mgtron-2.17.1/mgtron.egg-info/
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)    12098 2023-06-20 15:46:56.000000 mgtron-2.17.1/mgtron.egg-info/PKG-INFO
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     2171 2023-06-20 15:46:57.000000 mgtron-2.17.1/mgtron.egg-info/SOURCES.txt
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)        1 2023-06-20 15:46:56.000000 mgtron-2.17.1/mgtron.egg-info/dependency_links.txt
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)       37 2023-06-20 15:46:56.000000 mgtron-2.17.1/mgtron.egg-info/entry_points.txt
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     1531 2023-06-20 15:46:56.000000 mgtron-2.17.1/mgtron.egg-info/requires.txt
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)       25 2023-06-20 15:46:56.000000 mgtron-2.17.1/mgtron.egg-info/top_level.txt
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     2786 2023-06-20 15:46:10.000000 mgtron-2.17.1/pyproject.toml
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     1553 2023-06-19 20:47:25.000000 mgtron-2.17.1/requirements.txt
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)       38 2023-06-20 15:46:57.837773 mgtron-2.17.1/setup.cfg
-drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-20 15:46:57.827773 mgtron-2.17.1/src/
--rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        1 2023-06-16 17:38:51.000000 mgtron-2.17.1/src/__init__.py
-drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-20 15:46:57.834440 mgtron-2.17.1/src/assets/
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)    83964 2023-06-09 13:32:26.000000 mgtron-2.17.1/src/assets/CA logo without subtext.JPG
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)    65978 2023-06-09 13:32:26.000000 mgtron-2.17.1/src/assets/CA_subheading.png
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     7807 2023-06-20 15:44:52.000000 mgtron-2.17.1/src/assets/CHANGELOG.cpy
--rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000) 12821408 2023-06-20 14:26:27.000000 mgtron-2.17.1/src/assets/blueio_rs
--rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)     1303 2023-06-09 13:32:26.000000 mgtron-2.17.1/src/assets/init_cellantenna.sh
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      291 2023-06-09 13:32:26.000000 mgtron-2.17.1/src/assets/mgtron.desktop
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     2655 2023-06-09 13:32:26.000000 mgtron-2.17.1/src/assets/mgtron.svg
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)    67646 2023-06-09 13:32:26.000000 mgtron-2.17.1/src/assets/network-wireless.ico
-drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-20 15:46:57.834440 mgtron-2.17.1/src/ble/
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-16 17:38:51.000000 mgtron-2.17.1/src/ble/__init__.py
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      832 2023-06-19 20:47:25.000000 mgtron-2.17.1/src/ble/ble.py
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     2728 2023-06-20 14:48:33.000000 mgtron-2.17.1/src/ble/ble_data.py
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     1738 2023-06-19 20:47:25.000000 mgtron-2.17.1/src/ble/helpers.py
-drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-20 15:46:57.834440 mgtron-2.17.1/src/gui/
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)       80 2023-06-09 13:32:26.000000 mgtron-2.17.1/src/gui/__init__.py
-drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-20 15:46:57.834440 mgtron-2.17.1/src/gui/_configs/
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      269 2023-06-09 13:32:26.000000 mgtron-2.17.1/src/gui/_configs/card_1.ini
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      269 2023-06-09 13:32:26.000000 mgtron-2.17.1/src/gui/_configs/card_2.ini
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      269 2023-06-09 13:32:26.000000 mgtron-2.17.1/src/gui/_configs/card_3.ini
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      269 2023-06-09 13:32:26.000000 mgtron-2.17.1/src/gui/_configs/card_4.ini
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      269 2023-06-09 13:32:26.000000 mgtron-2.17.1/src/gui/_configs/card_5.ini
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      269 2023-06-09 13:32:26.000000 mgtron-2.17.1/src/gui/_configs/card_6.ini
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      263 2023-06-09 13:32:26.000000 mgtron-2.17.1/src/gui/_configs/card_7.ini
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      269 2023-06-09 13:32:26.000000 mgtron-2.17.1/src/gui/_configs/card_8.ini
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      105 2023-06-20 15:45:17.000000 mgtron-2.17.1/src/gui/_configs/card_config.ini
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      317 2023-06-09 13:32:26.000000 mgtron-2.17.1/src/gui/_configs/mission_alpha.ini
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      292 2023-06-09 13:32:26.000000 mgtron-2.17.1/src/gui/_configs/mission_bravo.ini
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      324 2023-06-09 13:32:26.000000 mgtron-2.17.1/src/gui/_configs/mission_charlie.ini
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      312 2023-06-09 13:32:26.000000 mgtron-2.17.1/src/gui/_configs/mission_delta.ini
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      273 2023-06-09 13:32:26.000000 mgtron-2.17.1/src/gui/_configs/mission_echo.ini
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      313 2023-06-09 13:32:26.000000 mgtron-2.17.1/src/gui/_configs/mission_fox.ini
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      279 2023-06-09 13:32:26.000000 mgtron-2.17.1/src/gui/_configs/mission_golf.ini
-drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-20 15:46:57.834440 mgtron-2.17.1/src/gui/db/
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-09 13:32:26.000000 mgtron-2.17.1/src/gui/db/channel_1.sql
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-09 13:32:26.000000 mgtron-2.17.1/src/gui/db/channel_2.sql
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-09 13:32:26.000000 mgtron-2.17.1/src/gui/db/channel_3.sql
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-09 13:32:26.000000 mgtron-2.17.1/src/gui/db/channel_4.sql
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-09 13:32:26.000000 mgtron-2.17.1/src/gui/db/channel_5.sql
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-09 13:32:26.000000 mgtron-2.17.1/src/gui/db/channel_6.sql
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-09 13:32:26.000000 mgtron-2.17.1/src/gui/db/channel_7.sql
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-09 13:32:26.000000 mgtron-2.17.1/src/gui/db/channel_8.sql
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     2516 2023-06-09 13:32:26.000000 mgtron-2.17.1/src/gui/db/init_db.sql
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)    10906 2023-06-09 13:32:26.000000 mgtron-2.17.1/src/gui/db/long_save.json
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-09 13:32:26.000000 mgtron-2.17.1/src/gui/db/long_save.json.lock
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)    49152 2023-06-14 02:00:32.000000 mgtron-2.17.1/src/gui/db/mgtron_db.db
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     8856 2023-06-16 17:38:51.000000 mgtron-2.17.1/src/gui/db/models.py
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     1170 2023-06-16 17:38:51.000000 mgtron-2.17.1/src/gui/db/quick_save.json
-drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-20 15:46:57.834440 mgtron-2.17.1/src/gui/fonts/
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)  1260156 2023-06-09 13:32:26.000000 mgtron-2.17.1/src/gui/fonts/MesloLGS NF Bold Italic.ttf
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)  1251424 2023-06-09 13:32:26.000000 mgtron-2.17.1/src/gui/fonts/MesloLGS NF Italic.ttf
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)  1292408 2023-06-09 13:32:26.000000 mgtron-2.17.1/src/gui/fonts/MesloLGS NF Regular.ttf
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)    65281 2023-06-20 15:21:37.000000 mgtron-2.17.1/src/gui/helpers.py
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)    10789 2023-06-19 20:47:25.000000 mgtron-2.17.1/src/gui/interface.py
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)    43783 2023-06-20 15:14:36.000000 mgtron-2.17.1/src/main.py
-drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-20 15:46:57.837773 mgtron-2.17.1/src/tests/
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)       33 2023-06-09 13:32:26.000000 mgtron-2.17.1/src/tests/__init__.py
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)       70 2023-06-19 20:47:25.000000 mgtron-2.17.1/src/tests/test_ble.py
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)    63110 2023-06-09 13:32:26.000000 mgtron-2.17.1/src/tests/test_configfiles.py
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)    19813 2023-06-09 13:32:26.000000 mgtron-2.17.1/src/tests/test_helpers.py
-drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-20 15:46:57.827773 mgtron-2.17.1/venv/
-drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-20 15:46:57.837773 mgtron-2.17.1/venv/bin/
--rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)      661 2023-06-20 14:10:02.000000 mgtron-2.17.1/venv/bin/rst2html.py
--rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)      783 2023-06-20 14:10:02.000000 mgtron-2.17.1/venv/bin/rst2html4.py
--rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)     1118 2023-06-20 14:10:02.000000 mgtron-2.17.1/venv/bin/rst2html5.py
--rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)      860 2023-06-20 14:10:02.000000 mgtron-2.17.1/venv/bin/rst2latex.py
--rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)      683 2023-06-20 14:10:02.000000 mgtron-2.17.1/venv/bin/rst2man.py
--rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)      849 2023-06-20 14:10:02.000000 mgtron-2.17.1/venv/bin/rst2odt.py
--rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)      655 2023-06-20 14:10:02.000000 mgtron-2.17.1/venv/bin/rst2odt_prepstyles.py
--rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)      668 2023-06-20 14:10:02.000000 mgtron-2.17.1/venv/bin/rst2pseudoxml.py
--rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)      704 2023-06-20 14:10:02.000000 mgtron-2.17.1/venv/bin/rst2s5.py
--rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)      940 2023-06-20 14:10:02.000000 mgtron-2.17.1/venv/bin/rst2xetex.py
--rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)      669 2023-06-20 14:10:02.000000 mgtron-2.17.1/venv/bin/rst2xml.py
--rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)      737 2023-06-20 14:10:02.000000 mgtron-2.17.1/venv/bin/rstpep2html.py
+drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-27 20:26:08.570020 mgtron-2.18.0/
+drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-27 20:26:08.476686 mgtron-2.18.0/.github/
+drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-27 20:26:08.480019 mgtron-2.18.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      602 2023-06-23 15:16:00.000000 mgtron-2.18.0/.github/ISSUE_TEMPLATE/mgtron--.md
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     1524 2023-06-23 15:16:00.000000 mgtron-2.18.0/.github/ISSUE_TEMPLATE/mgtron_issue.yml
+drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-27 20:26:08.480019 mgtron-2.18.0/.github/workflows/
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      520 2023-06-27 20:21:35.000000 mgtron-2.18.0/.github/workflows/black_actions.yml
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      830 2023-06-27 20:21:35.000000 mgtron-2.18.0/.github/workflows/pypi_action.yml
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      365 2023-06-23 15:16:00.000000 mgtron-2.18.0/.gitignore
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     8278 2023-06-27 20:21:35.000000 mgtron-2.18.0/CHANGELOG.md
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      957 2023-06-23 15:16:00.000000 mgtron-2.18.0/LICENSE.rst
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)    12474 2023-06-27 20:26:08.570020 mgtron-2.18.0/PKG-INFO
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     3699 2023-06-23 15:16:00.000000 mgtron-2.18.0/README.md
+drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-27 20:26:08.490019 mgtron-2.18.0/docs/
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)    17614 2023-06-23 15:16:01.000000 mgtron-2.18.0/docs/MGTron Command Description.docx
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)    23088 2023-06-23 15:16:01.000000 mgtron-2.18.0/docs/MGTron Function Descriptions.docx
+drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-27 20:26:08.500019 mgtron-2.18.0/mgtron.egg-info/
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)    12474 2023-06-27 20:26:08.000000 mgtron-2.18.0/mgtron.egg-info/PKG-INFO
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     2323 2023-06-27 20:26:08.000000 mgtron-2.18.0/mgtron.egg-info/SOURCES.txt
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)        1 2023-06-27 20:26:08.000000 mgtron-2.18.0/mgtron.egg-info/dependency_links.txt
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)       37 2023-06-27 20:26:08.000000 mgtron-2.18.0/mgtron.egg-info/entry_points.txt
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     1531 2023-06-27 20:26:08.000000 mgtron-2.18.0/mgtron.egg-info/requires.txt
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)       25 2023-06-27 20:26:08.000000 mgtron-2.18.0/mgtron.egg-info/top_level.txt
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     2786 2023-06-27 20:21:35.000000 mgtron-2.18.0/pyproject.toml
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     1875 2023-06-27 20:21:35.000000 mgtron-2.18.0/requirements.txt
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)       38 2023-06-27 20:26:08.570020 mgtron-2.18.0/setup.cfg
+drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-27 20:26:08.500019 mgtron-2.18.0/src/
+-rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        1 2023-06-23 15:16:01.000000 mgtron-2.18.0/src/__init__.py
+drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-27 20:26:08.536687 mgtron-2.18.0/src/assets/
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)    83964 2023-06-23 15:16:01.000000 mgtron-2.18.0/src/assets/CA logo without subtext.JPG
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)    65978 2023-06-23 15:16:01.000000 mgtron-2.18.0/src/assets/CA_subheading.png
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     8278 2023-06-27 20:21:35.000000 mgtron-2.18.0/src/assets/CHANGELOG.cpy
+-rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000) 12821408 2023-06-23 15:16:01.000000 mgtron-2.18.0/src/assets/blueio_rs
+-rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)     1303 2023-06-23 15:16:01.000000 mgtron-2.18.0/src/assets/init_cellantenna.sh
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      291 2023-06-23 15:16:01.000000 mgtron-2.18.0/src/assets/mgtron.desktop
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     2655 2023-06-23 15:16:01.000000 mgtron-2.18.0/src/assets/mgtron.svg
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)    67646 2023-06-23 15:16:01.000000 mgtron-2.18.0/src/assets/network-wireless.ico
+drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-27 20:26:08.546687 mgtron-2.18.0/src/ble/
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-23 15:16:01.000000 mgtron-2.18.0/src/ble/__init__.py
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     3126 2023-06-27 20:21:35.000000 mgtron-2.18.0/src/ble/ble_data.py
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     8159 2023-06-27 20:21:35.000000 mgtron-2.18.0/src/ble/helpers.py
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      859 2023-06-27 20:21:35.000000 mgtron-2.18.0/src/ble/scanning.py
+drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-27 20:26:08.553353 mgtron-2.18.0/src/db/
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-27 20:21:35.000000 mgtron-2.18.0/src/db/__init__.py
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-27 20:21:35.000000 mgtron-2.18.0/src/db/channel_1.sql
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-27 20:21:35.000000 mgtron-2.18.0/src/db/channel_2.sql
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-27 20:21:35.000000 mgtron-2.18.0/src/db/channel_3.sql
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-27 20:21:35.000000 mgtron-2.18.0/src/db/channel_4.sql
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-27 20:21:35.000000 mgtron-2.18.0/src/db/channel_5.sql
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-27 20:21:35.000000 mgtron-2.18.0/src/db/channel_6.sql
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-27 20:21:35.000000 mgtron-2.18.0/src/db/channel_7.sql
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-27 20:21:35.000000 mgtron-2.18.0/src/db/channel_8.sql
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     9672 2023-06-27 20:21:35.000000 mgtron-2.18.0/src/db/helpers.py
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     2516 2023-06-27 20:21:35.000000 mgtron-2.18.0/src/db/init_db.sql
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)    10906 2023-06-27 20:21:35.000000 mgtron-2.18.0/src/db/long_save.json
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-27 20:21:35.000000 mgtron-2.18.0/src/db/long_save.json.lock
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)    49152 2023-06-27 19:48:39.000000 mgtron-2.18.0/src/db/mgtron_db.db
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     8808 2023-06-27 20:21:35.000000 mgtron-2.18.0/src/db/models.py
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     1170 2023-06-27 20:21:35.000000 mgtron-2.18.0/src/db/quick_save.json
+drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-27 20:26:08.553353 mgtron-2.18.0/src/globals/
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-27 20:21:35.000000 mgtron-2.18.0/src/globals/__init__.py
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     3392 2023-06-27 20:21:35.000000 mgtron-2.18.0/src/globals/helpers.py
+drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-27 20:26:08.553353 mgtron-2.18.0/src/gui/
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)       80 2023-06-23 15:16:01.000000 mgtron-2.18.0/src/gui/__init__.py
+drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-27 20:26:08.560020 mgtron-2.18.0/src/gui/_configs/
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      269 2023-06-23 15:16:01.000000 mgtron-2.18.0/src/gui/_configs/card_1.ini
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      269 2023-06-23 15:16:01.000000 mgtron-2.18.0/src/gui/_configs/card_2.ini
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      269 2023-06-23 15:16:01.000000 mgtron-2.18.0/src/gui/_configs/card_3.ini
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      269 2023-06-23 15:16:01.000000 mgtron-2.18.0/src/gui/_configs/card_4.ini
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      269 2023-06-23 15:16:01.000000 mgtron-2.18.0/src/gui/_configs/card_5.ini
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      269 2023-06-23 15:16:01.000000 mgtron-2.18.0/src/gui/_configs/card_6.ini
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      263 2023-06-23 15:16:01.000000 mgtron-2.18.0/src/gui/_configs/card_7.ini
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      269 2023-06-23 15:16:01.000000 mgtron-2.18.0/src/gui/_configs/card_8.ini
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)       98 2023-06-21 12:37:32.000000 mgtron-2.18.0/src/gui/_configs/card_config.ini
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      317 2023-06-23 15:16:01.000000 mgtron-2.18.0/src/gui/_configs/mission_alpha.ini
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      292 2023-06-23 15:16:01.000000 mgtron-2.18.0/src/gui/_configs/mission_bravo.ini
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      324 2023-06-23 15:16:01.000000 mgtron-2.18.0/src/gui/_configs/mission_charlie.ini
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      312 2023-06-23 15:16:01.000000 mgtron-2.18.0/src/gui/_configs/mission_delta.ini
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      273 2023-06-23 15:16:01.000000 mgtron-2.18.0/src/gui/_configs/mission_echo.ini
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      313 2023-06-23 15:16:01.000000 mgtron-2.18.0/src/gui/_configs/mission_fox.ini
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      279 2023-06-23 15:16:01.000000 mgtron-2.18.0/src/gui/_configs/mission_golf.ini
+drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-27 20:26:08.563354 mgtron-2.18.0/src/gui/fonts/
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)  1260156 2023-06-23 15:16:01.000000 mgtron-2.18.0/src/gui/fonts/MesloLGS NF Bold Italic.ttf
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)  1251424 2023-06-23 15:16:01.000000 mgtron-2.18.0/src/gui/fonts/MesloLGS NF Italic.ttf
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)  1292408 2023-06-23 15:16:01.000000 mgtron-2.18.0/src/gui/fonts/MesloLGS NF Regular.ttf
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)    49343 2023-06-27 20:21:35.000000 mgtron-2.18.0/src/gui/helpers.py
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)    10789 2023-06-23 15:16:01.000000 mgtron-2.18.0/src/gui/interface.py
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)    43487 2023-06-27 20:21:35.000000 mgtron-2.18.0/src/main.py
+drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-27 20:26:08.566687 mgtron-2.18.0/src/tests/
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)       33 2023-06-23 15:16:01.000000 mgtron-2.18.0/src/tests/__init__.py
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)       70 2023-06-23 15:16:01.000000 mgtron-2.18.0/src/tests/test_ble.py
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)    63110 2023-06-23 15:16:01.000000 mgtron-2.18.0/src/tests/test_configfiles.py
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)    19813 2023-06-23 15:16:01.000000 mgtron-2.18.0/src/tests/test_helpers.py
+drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-27 20:26:08.566687 mgtron-2.18.0/src/wifi/
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-27 20:21:35.000000 mgtron-2.18.0/src/wifi/__init__.py
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     9628 2023-06-27 20:21:35.000000 mgtron-2.18.0/src/wifi/helpers.py
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-27 20:21:35.000000 mgtron-2.18.0/src/wifi/processing.py
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     6170 2023-06-27 20:21:35.000000 mgtron-2.18.0/src/wifi/scanning.py
+drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-27 20:26:08.480019 mgtron-2.18.0/venv/
+drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-27 20:26:08.570020 mgtron-2.18.0/venv/bin/
+-rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)      665 2023-06-12 19:48:50.000000 mgtron-2.18.0/venv/bin/rst2html.py
+-rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)      787 2023-06-12 19:48:50.000000 mgtron-2.18.0/venv/bin/rst2html4.py
+-rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)     1122 2023-06-12 19:48:50.000000 mgtron-2.18.0/venv/bin/rst2html5.py
+-rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)      864 2023-06-12 19:48:50.000000 mgtron-2.18.0/venv/bin/rst2latex.py
+-rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)      687 2023-06-12 19:48:50.000000 mgtron-2.18.0/venv/bin/rst2man.py
+-rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)      853 2023-06-12 19:48:50.000000 mgtron-2.18.0/venv/bin/rst2odt.py
+-rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)      659 2023-06-12 19:48:50.000000 mgtron-2.18.0/venv/bin/rst2odt_prepstyles.py
+-rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)      672 2023-06-12 19:48:50.000000 mgtron-2.18.0/venv/bin/rst2pseudoxml.py
+-rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)      708 2023-06-12 19:48:50.000000 mgtron-2.18.0/venv/bin/rst2s5.py
+-rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)      944 2023-06-12 19:48:50.000000 mgtron-2.18.0/venv/bin/rst2xetex.py
+-rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)      673 2023-06-12 19:48:50.000000 mgtron-2.18.0/venv/bin/rst2xml.py
+-rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)      741 2023-06-12 19:48:50.000000 mgtron-2.18.0/venv/bin/rstpep2html.py
```

### Comparing `mgtron-2.17.1/.github/ISSUE_TEMPLATE/mgtron--.md` & `mgtron-2.18.0/.github/ISSUE_TEMPLATE/mgtron--.md`

 * *Files identical despite different names*

### Comparing `mgtron-2.17.1/.github/ISSUE_TEMPLATE/mgtron_issue.yml` & `mgtron-2.18.0/.github/ISSUE_TEMPLATE/mgtron_issue.yml`

 * *Files identical despite different names*

### Comparing `mgtron-2.17.1/CHANGELOG.md` & `mgtron-2.18.0/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -18,14 +18,28 @@
 
 ✴️ MINOR version when you add functionality in a backwards compatible manner
 
 ✳️ PATCH version when you make backwards compatible bug fixes.
 
 -------------------------------------------------------------------------------
 
+## ✴️️️ [2.18.0] - 2023 JUNE 26
+
+- 'SEND ALL' button send requisite command depending on the state of wifi and bluetooth.
+- Disable all action and mission buttons during a wifi or bluetooth scan.
+- Implement an incremental print during wifi scan.
+
+## ✳️ [2.17.3] - 2023 JUNE 21
+
+- Fixed a bug in which the GUI would delete custom save when they were chosen.
+
+## ✳️ [2.17.2] - 2023 JUNE 20
+
+- Updated the README.md to reflect the new installation method.
+
 ## ✳️ [2.17.1] - 2023 JUNE 20
 
 - Fixed a bug in which the GUI would hang if the BLE server was running.
 
 ## ✴️️️ [2.17.0] - 2023 JUNE 19
 
 - Stabilized the BLE server starting and stopping.
```

### Comparing `mgtron-2.17.1/LICENSE.rst` & `mgtron-2.18.0/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `mgtron-2.17.1/PKG-INFO` & `mgtron-2.18.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mgtron
-Version: 2.17.1
+Version: 2.18.0
 Summary: Package for MGTron GUI, a user interface for signal generation
 Author-email: Christerpher Hunter <chunter@cellantenna.com>
 Project-URL: Source, https://github.com/cellantenna/mg_tron
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: POSIX :: Linux
 Requires-Python: >=3.10
@@ -44,25 +44,21 @@
 ### Requirements
 
 * Python 3.10+
 * git
 
 ### install from GitHub
 
-`git clone https://github.com/cellantenna/mg_tron.git`
-
-`cd mg_tron`
-
-`python3.10 -m venv venv` - Optional, but recommended.
+`python -m venv venv` - Optional, but recommended.
 
 `source venv/bin/activate` - Required, if last line is executed.
 
-`pip install -r requirements.txt`
+`pip install mgtron`
 
-`python -m main`
+`mgtron`
 
 ## Known Issues
 
 ### Permissions
 - Depending on your OS of choice, you may need to change the permissions of the serial port.  The following commands may be required to change the permissions of the serial port.
 * `sudo chmod 777 /dev/ttyACM*` - temporary fix
 * `sudo usermod -a -G dialout $USER` - permanent fix; reboot required
@@ -102,14 +98,28 @@
 
 ✴️ MINOR version when you add functionality in a backwards compatible manner
 
 ✳️ PATCH version when you make backwards compatible bug fixes.
 
 -------------------------------------------------------------------------------
 
+## ✴️️️ [2.18.0] - 2023 JUNE 26
+
+- 'SEND ALL' button send requisite command depending on the state of wifi and bluetooth.
+- Disable all action and mission buttons during a wifi or bluetooth scan.
+- Implement an incremental print during wifi scan.
+
+## ✳️ [2.17.3] - 2023 JUNE 21
+
+- Fixed a bug in which the GUI would delete custom save when they were chosen.
+
+## ✳️ [2.17.2] - 2023 JUNE 20
+
+- Updated the README.md to reflect the new installation method.
+
 ## ✳️ [2.17.1] - 2023 JUNE 20
 
 - Fixed a bug in which the GUI would hang if the BLE server was running.
 
 ## ✴️️️ [2.17.0] - 2023 JUNE 19
 
 - Stabilized the BLE server starting and stopping.
```

### Comparing `mgtron-2.17.1/README.md` & `mgtron-2.18.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -30,25 +30,21 @@
 ### Requirements
 
 * Python 3.10+
 * git
 
 ### install from GitHub
 
-`git clone https://github.com/cellantenna/mg_tron.git`
-
-`cd mg_tron`
-
-`python3.10 -m venv venv` - Optional, but recommended.
+`python -m venv venv` - Optional, but recommended.
 
 `source venv/bin/activate` - Required, if last line is executed.
 
-`pip install -r requirements.txt`
+`pip install mgtron`
 
-`python -m main`
+`mgtron`
 
 ## Known Issues
 
 ### Permissions
 - Depending on your OS of choice, you may need to change the permissions of the serial port.  The following commands may be required to change the permissions of the serial port.
 * `sudo chmod 777 /dev/ttyACM*` - temporary fix
 * `sudo usermod -a -G dialout $USER` - permanent fix; reboot required
```

### Comparing `mgtron-2.17.1/docs/MGTron Command Description.docx` & `mgtron-2.18.0/docs/MGTron Command Description.docx`

 * *Files identical despite different names*

### Comparing `mgtron-2.17.1/docs/MGTron Function Descriptions.docx` & `mgtron-2.18.0/docs/MGTron Function Descriptions.docx`

 * *Files identical despite different names*

### Comparing `mgtron-2.17.1/mgtron.egg-info/PKG-INFO` & `mgtron-2.18.0/mgtron.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mgtron
-Version: 2.17.1
+Version: 2.18.0
 Summary: Package for MGTron GUI, a user interface for signal generation
 Author-email: Christerpher Hunter <chunter@cellantenna.com>
 Project-URL: Source, https://github.com/cellantenna/mg_tron
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: POSIX :: Linux
 Requires-Python: >=3.10
@@ -44,25 +44,21 @@
 ### Requirements
 
 * Python 3.10+
 * git
 
 ### install from GitHub
 
-`git clone https://github.com/cellantenna/mg_tron.git`
-
-`cd mg_tron`
-
-`python3.10 -m venv venv` - Optional, but recommended.
+`python -m venv venv` - Optional, but recommended.
 
 `source venv/bin/activate` - Required, if last line is executed.
 
-`pip install -r requirements.txt`
+`pip install mgtron`
 
-`python -m main`
+`mgtron`
 
 ## Known Issues
 
 ### Permissions
 - Depending on your OS of choice, you may need to change the permissions of the serial port.  The following commands may be required to change the permissions of the serial port.
 * `sudo chmod 777 /dev/ttyACM*` - temporary fix
 * `sudo usermod -a -G dialout $USER` - permanent fix; reboot required
@@ -102,14 +98,28 @@
 
 ✴️ MINOR version when you add functionality in a backwards compatible manner
 
 ✳️ PATCH version when you make backwards compatible bug fixes.
 
 -------------------------------------------------------------------------------
 
+## ✴️️️ [2.18.0] - 2023 JUNE 26
+
+- 'SEND ALL' button send requisite command depending on the state of wifi and bluetooth.
+- Disable all action and mission buttons during a wifi or bluetooth scan.
+- Implement an incremental print during wifi scan.
+
+## ✳️ [2.17.3] - 2023 JUNE 21
+
+- Fixed a bug in which the GUI would delete custom save when they were chosen.
+
+## ✳️ [2.17.2] - 2023 JUNE 20
+
+- Updated the README.md to reflect the new installation method.
+
 ## ✳️ [2.17.1] - 2023 JUNE 20
 
 - Fixed a bug in which the GUI would hang if the BLE server was running.
 
 ## ✴️️️ [2.17.0] - 2023 JUNE 19
 
 - Stabilized the BLE server starting and stopping.
```

### Comparing `mgtron-2.17.1/mgtron.egg-info/SOURCES.txt` & `mgtron-2.18.0/mgtron.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 LICENSE.rst
 README.md
 pyproject.toml
 requirements.txt
 .github/ISSUE_TEMPLATE/mgtron--.md
 .github/ISSUE_TEMPLATE/mgtron_issue.yml
 .github/workflows/black_actions.yml
+.github/workflows/pypi_action.yml
 docs/MGTron Command Description.docx
 docs/MGTron Function Descriptions.docx
 mgtron.egg-info/PKG-INFO
 mgtron.egg-info/SOURCES.txt
 mgtron.egg-info/dependency_links.txt
 mgtron.egg-info/entry_points.txt
 mgtron.egg-info/requires.txt
@@ -22,17 +23,35 @@
 src/assets/CHANGELOG.cpy
 src/assets/blueio_rs
 src/assets/init_cellantenna.sh
 src/assets/mgtron.desktop
 src/assets/mgtron.svg
 src/assets/network-wireless.ico
 src/ble/__init__.py
-src/ble/ble.py
 src/ble/ble_data.py
 src/ble/helpers.py
+src/ble/scanning.py
+src/db/__init__.py
+src/db/channel_1.sql
+src/db/channel_2.sql
+src/db/channel_3.sql
+src/db/channel_4.sql
+src/db/channel_5.sql
+src/db/channel_6.sql
+src/db/channel_7.sql
+src/db/channel_8.sql
+src/db/helpers.py
+src/db/init_db.sql
+src/db/long_save.json
+src/db/long_save.json.lock
+src/db/mgtron_db.db
+src/db/models.py
+src/db/quick_save.json
+src/globals/__init__.py
+src/globals/helpers.py
 src/gui/__init__.py
 src/gui/helpers.py
 src/gui/interface.py
 src/gui/_configs/card_1.ini
 src/gui/_configs/card_2.ini
 src/gui/_configs/card_3.ini
 src/gui/_configs/card_4.ini
@@ -44,35 +63,25 @@
 src/gui/_configs/mission_alpha.ini
 src/gui/_configs/mission_bravo.ini
 src/gui/_configs/mission_charlie.ini
 src/gui/_configs/mission_delta.ini
 src/gui/_configs/mission_echo.ini
 src/gui/_configs/mission_fox.ini
 src/gui/_configs/mission_golf.ini
-src/gui/db/channel_1.sql
-src/gui/db/channel_2.sql
-src/gui/db/channel_3.sql
-src/gui/db/channel_4.sql
-src/gui/db/channel_5.sql
-src/gui/db/channel_6.sql
-src/gui/db/channel_7.sql
-src/gui/db/channel_8.sql
-src/gui/db/init_db.sql
-src/gui/db/long_save.json
-src/gui/db/long_save.json.lock
-src/gui/db/mgtron_db.db
-src/gui/db/models.py
-src/gui/db/quick_save.json
 src/gui/fonts/MesloLGS NF Bold Italic.ttf
 src/gui/fonts/MesloLGS NF Italic.ttf
 src/gui/fonts/MesloLGS NF Regular.ttf
 src/tests/__init__.py
 src/tests/test_ble.py
 src/tests/test_configfiles.py
 src/tests/test_helpers.py
+src/wifi/__init__.py
+src/wifi/helpers.py
+src/wifi/processing.py
+src/wifi/scanning.py
 venv/bin/rst2html.py
 venv/bin/rst2html4.py
 venv/bin/rst2html5.py
 venv/bin/rst2latex.py
 venv/bin/rst2man.py
 venv/bin/rst2odt.py
 venv/bin/rst2odt_prepstyles.py
```

### Comparing `mgtron-2.17.1/mgtron.egg-info/requires.txt` & `mgtron-2.18.0/mgtron.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `mgtron-2.17.1/pyproject.toml` & `mgtron-2.18.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 [project]
 name = "mgtron"
 authors = [
   { name="Christerpher Hunter", email="chunter@cellantenna.com" },
 ]
 dynamic = ["readme"]
 description = "Package for MGTron GUI, a user interface for signal generation"
-version = "2.17.1"
+version = "2.18.0"
 requires-python = ">=3.10"
 classifiers = [
 "Programming Language :: Python :: 3",
 "License :: Other/Proprietary License",
 "Operating System :: POSIX :: Linux",
 ]
```

### Comparing `mgtron-2.17.1/requirements.txt` & `mgtron-2.18.0/requirements.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,31 +1,42 @@
 aiosqlite==0.19.0
+anyio==3.7.0
 astroid==2.15.5
+asyncio==3.4.3
 attrs==23.1.0
 autopep8==2.0.2
 beautifultable==1.1.0
 bleach==6.0.0
 bleuio==1.2.0
 build==0.10.0
 certifi==2023.5.7
 cffi==1.15.1
 charset-normalizer==3.1.0
+click==8.1.3
 colorama==0.4.6
 coverage==7.2.7
 cryptography==41.0.1
 dearpygui==1.9.1
 dill==0.3.6
+distlib==0.3.6
 docstring-to-markdown==0.12
 docutils==0.20.1
+editables==0.3
 exceptiongroup==1.1.1
 filelock==3.12.1
 flake8==6.0.0
 gevent==22.10.2
 greenlet==2.0.2
 grequests==0.7.0
+h11==0.14.0
+hatch==1.7.0
+hatchling==1.18.0
+httpcore==0.17.2
+httpx==0.24.1
+hyperlink==21.0.0
 idna==3.4
 importlib-metadata==6.6.0
 iniconfig==2.0.0
 isort==5.12.0
 jaraco.classes==3.2.3
 jedi==0.18.2
 jeepney==0.8.0
@@ -33,28 +44,30 @@
 lazy-object-proxy==1.9.0
 markdown-it-py==3.0.0
 mccabe==0.7.0
 mdurl==0.1.2
 more-itertools==9.1.0
 mypy==1.3.0
 mypy-extensions==1.0.0
-numpy==1.24.3
 packaging==23.1
-pandas==2.0.2
 parso==0.8.3
+pathspec==0.11.1
+pexpect==4.8.0
 pkginfo==1.9.6
 platformdirs==3.5.3
 pluggy==1.0.0
+ptyprocess==0.7.0
 pycodestyle==2.10.0
 pycparser==2.21
 pydocstyle==6.3.0
 pyflakes==3.0.1
 Pygments==2.15.1
 pylint==2.17.4
 pyparsing==3.0.9
+pyperclip==1.8.2
 pyproject_hooks==1.0.0
 pyserial==3.5
 pysondb==1.6.7
 pytest==7.3.2
 pytest-asyncio==0.21.0
 pytest-cov==4.1.0
 python-dateutil==2.8.2
@@ -66,24 +79,30 @@
 readme-renderer==37.3
 requests==2.31.0
 requests-toolbelt==1.0.0
 rfc3986==2.0.0
 rich==13.4.2
 rope==1.8.0
 SecretStorage==3.3.3
+shellingham==1.5.0.post1
 six==1.16.0
+sniffio==1.3.0
 snowballstemmer==2.2.0
 toml==0.10.2
 tomli==2.0.1
+tomli_w==1.0.0
 tomlkit==0.11.8
+trove-classifiers==2023.5.24
 twine==4.0.2
 typing_extensions==4.6.3
 tzdata==2023.3
 ujson==5.8.0
 urllib3==2.0.3
+userpath==1.8.0
+virtualenv==20.23.0
 wcwidth==0.2.6
 webencodings==0.5.1
 whatthepatch==1.0.5
 wrapt==1.15.0
 yapf==0.33.0
 zipp==3.15.0
 zope.event==4.6
```

### Comparing `mgtron-2.17.1/src/assets/CA logo without subtext.JPG` & `mgtron-2.18.0/src/assets/CA logo without subtext.JPG`

 * *Files identical despite different names*

### Comparing `mgtron-2.17.1/src/assets/CA_subheading.png` & `mgtron-2.18.0/src/assets/CA_subheading.png`

 * *Files identical despite different names*

### Comparing `mgtron-2.17.1/src/assets/CHANGELOG.cpy` & `mgtron-2.18.0/src/assets/CHANGELOG.cpy`

 * *Files 6% similar despite different names*

```diff
@@ -18,14 +18,28 @@
 
 ✴️ MINOR version when you add functionality in a backwards compatible manner
 
 ✳️ PATCH version when you make backwards compatible bug fixes.
 
 -------------------------------------------------------------------------------
 
+## ✴️️️ [2.18.0] - 2023 JUNE 26
+
+- 'SEND ALL' button send requisite command depending on the state of wifi and bluetooth.
+- Disable all action and mission buttons during a wifi or bluetooth scan.
+- Implement an incremental print during wifi scan.
+
+## ✳️ [2.17.3] - 2023 JUNE 21
+
+- Fixed a bug in which the GUI would delete custom save when they were chosen.
+
+## ✳️ [2.17.2] - 2023 JUNE 20
+
+- Updated the README.md to reflect the new installation method.
+
 ## ✳️ [2.17.1] - 2023 JUNE 20
 
 - Fixed a bug in which the GUI would hang if the BLE server was running.
 
 ## ✴️️️ [2.17.0] - 2023 JUNE 19
 
 - Stabilized the BLE server starting and stopping.
```

### Comparing `mgtron-2.17.1/src/assets/blueio_rs` & `mgtron-2.18.0/src/assets/blueio_rs`

 * *Files identical despite different names*

### Comparing `mgtron-2.17.1/src/assets/init_cellantenna.sh` & `mgtron-2.18.0/src/assets/init_cellantenna.sh`

 * *Files identical despite different names*

### Comparing `mgtron-2.17.1/src/assets/mgtron.svg` & `mgtron-2.18.0/src/assets/mgtron.svg`

 * *Files identical despite different names*

### Comparing `mgtron-2.17.1/src/assets/network-wireless.ico` & `mgtron-2.18.0/src/assets/network-wireless.ico`

 * *Files identical despite different names*

### Comparing `mgtron-2.17.1/src/ble/ble.py` & `mgtron-2.18.0/src/ble/scanning.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 """Make the API calls directly to the Rust API."""
 
-import requests
 import logging
+import requests
 
 loggei = logging.getLogger(name=__name__)
 
 
 def ble_rs(target: str) -> dict:
     """Call the BLE RS API and return the data."""
     loggei.debug(msg=f"{ble_rs.__name__}()")
 
     port = 8080
 
     try:
         data = requests.get(
             url=f"http://localhost:{port}/{target}",
             headers={"Content-Type": "application/json"},
+            timeout=8,
         )
 
         if data.status_code != 200:
             loggei.error(msg=f"BLE API returned {data.status_code}")
             return {}
 
         loggei.info(msg=f"BLE API raw response: {data}")
 
         data: dict = data.json()
 
         return data
 
-    except requests.exceptions.ConnectionError as e:
-        loggei.error(msg=f"BLE API not running: {e}")
+    except requests.exceptions.ConnectionError as err:
+        loggei.error(msg=f"BLE API not running: {err}")
         return {"Status": requests.status_codes}
```

### Comparing `mgtron-2.17.1/src/ble/ble_data.py` & `mgtron-2.18.0/src/ble/ble_data.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,20 @@
 """Process the BLE data."""
 
-import dearpygui.dearpygui as dpg
+
 import time
-from src.ble.helpers import ThreadWithReturnValue
-from src.ble.ble import ble_rs
 import logging
 
+import dearpygui.dearpygui as dpg
+
+from .scanning import ble_rs
+
+from ..globals.helpers import ThreadWithReturnValue
+
+
 loggei = logging.getLogger(name=__name__)
 
 
 def ble_data(company: bool) -> list:
     """Collate the da from the BLE API and return it."""
     loggei.debug(msg=f"{ble_data.__name__}()")
 
@@ -40,26 +45,31 @@
         list(rssi)
     ] if not company else [
         list(macs),
         list(companies)
     ]
 
 
-def ble_data_complete() -> list[tuple[str, tuple[str, str]]]:
-    """Get the MAC address, Manufacturer, and RSSI."""
-    company = True, False
+def threaded_scan(company: bool) -> tuple[list]:
+    """Scan for BLE signals and frequencies in a thread."""
+    loggei.debug(msg=f"{threaded_scan.__name__}()")
+
+    dpg.configure_item(
+        item=12,
+        modal=True,
+    )
 
     dpg.add_text(
         tag="scan_text",
         default_value="Scanning"
     )
 
     dpg.add_text(
         tag="scan_text_",
-        default_value='-' * 78
+        default_value='-' * 89
     )
 
     ble = ThreadWithReturnValue(
         target=ble_data,
         args=(company[0],)
     )
     ble.start()
@@ -80,38 +90,52 @@
 
     ble = ble.join()
     ble_rssi = ble_rssi.join()
 
     dpg.delete_item(item="scan_text")
     dpg.delete_item(item="scan_text_")
 
+    dpg.configure_item(
+        item=12,
+        modal=False,
+    )
+
+    return ble, ble_rssi
+
+
+def ble_data_complete() -> list[tuple[str, tuple[str, str]]]:
+    """Get the MAC address, Manufacturer, and RSSI."""
+    company = True, False
+
+    ble, ble_rssi = threaded_scan(company=company)
+
     if ble[0][0] == "Status":
         loggei.error(msg="BLE API not running")
         ble = [("status", ("BLE API not running", "BLE API not running"))]
         return ble
 
     ble.insert(3, [])
 
-    loggei.info(f"ble_company length: {len(ble[0])}")
-    loggei.info(f"ble_rssi length: {len(ble_rssi[0])}")
+    loggei.info("ble_company length: %s", len(ble[0]))
+    loggei.info("ble_rssi length: %s", len(ble_rssi[0]))
 
     try:
         for i, mac in enumerate(ble_rssi[0]):
             mac = mac.split(']')[1]
             for mac_2 in ble[0]:
                 if mac_2 == mac:
                     ble[2].insert(i, int(ble_rssi[-1][i]))
                     break
-    except IndexError as e:
-        loggei.warning(msg=f"BLE fail: {e}")
+    except IndexError as _error:
+        loggei.warning(msg=f"BLE fail: {_error}")
 
     for i in range(len(ble)):
 
         if len(ble[0]) != len(ble[2]):
-            loggei.warn(msg="ble[0] != ble[2]")
+            loggei.warning(msg="ble[0] != ble[2]")
             loggei.debug(msg=f"ble after insert: {ble}")
 
     ble = dict(zip(ble[0], zip(ble[1], ble[2])))
 
     ble = sorted(ble.items(), key=lambda x: x[1][1], reverse=True)
 
     return ble
```

### Comparing `mgtron-2.17.1/src/gui/db/init_db.sql` & `mgtron-2.18.0/src/db/init_db.sql`

 * *Files identical despite different names*

### Comparing `mgtron-2.17.1/src/gui/db/long_save.json` & `mgtron-2.18.0/src/db/long_save.json`

 * *Files identical despite different names*

### Comparing `mgtron-2.17.1/src/gui/db/models.py` & `mgtron-2.18.0/src/db/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,36 +2,34 @@
 
 from pathlib import Path
 import pathlib
 import sqlite3
 from datetime import datetime
 
 
-ROOT = pathlib.Path(__file__).resolve().parent.parent.parent.parent
-WORKING = ROOT / "src" / "gui"
+ROOT = pathlib.Path(__file__).resolve().parent.parent.parent
+WORKING = ROOT / "src"
 
 # Define the input values
+now = datetime.now()
 date_accessed_value = datetime.now().strftime("%Y-%m-%d")
 
 # If the file does not exist create it
 db_path: Path = Path(f"{WORKING}/db/mgtron_db.db")
 init_path: Path = Path(f"{WORKING}/db/init_db.sql")
 
 
 def read_sql_query(sql_path: pathlib.Path) -> str:
     """Read an SQL query from a file and returns it as a string."""
     return pathlib.Path(sql_path).read_text()
 
 
-print("initializing the db")
-
 # init the database
 init_db = read_sql_query(init_path)
 
-print("db initialized")
 
 # Populate db if it does not exist
 with sqlite3.connect(db_path) as conn:
     cursor = conn.cursor()
     cursor.executescript(init_db)
     conn.commit()
     # conn.close()
```

### Comparing `mgtron-2.17.1/src/gui/db/quick_save.json` & `mgtron-2.18.0/src/db/quick_save.json`

 * *Files identical despite different names*

### Comparing `mgtron-2.17.1/src/gui/fonts/MesloLGS NF Bold Italic.ttf` & `mgtron-2.18.0/src/gui/fonts/MesloLGS NF Bold Italic.ttf`

 * *Files identical despite different names*

### Comparing `mgtron-2.17.1/src/gui/fonts/MesloLGS NF Italic.ttf` & `mgtron-2.18.0/src/gui/fonts/MesloLGS NF Italic.ttf`

 * *Files identical despite different names*

### Comparing `mgtron-2.17.1/src/gui/fonts/MesloLGS NF Regular.ttf` & `mgtron-2.18.0/src/gui/fonts/MesloLGS NF Regular.ttf`

 * *Files identical despite different names*

### Comparing `mgtron-2.17.1/src/gui/helpers.py` & `mgtron-2.18.0/src/gui/helpers.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,97 +1,46 @@
 """Helper functions for the GUI. Intended design is functional programming."""
-#!/usr/bin/env python
 
 import os
-import signal
 import configparser
-import itertools
-import json
 import threading
 import logging
 import pathlib
 import platform
-import sqlite3
 
 import subprocess
 import sys
+from typing import Callable
 from datetime import datetime
 
-import dearpygui.dearpygui as dpg
-from interface import Megatron, format_output
+from colorama import Fore as F
 
-from src.gui.db.models import delete_sql_save_data
-from src.gui.db.models import get_sql_details
-from src.gui.db.models import get_sql_save_names
+import dearpygui.dearpygui as dpg
+from ..gui.interface import Megatron
+from ..gui.interface import format_output
 
-from src.ble.ble_data import ble_data_complete
+from ..db.helpers import check_and_load_config
 
+R = F.RESET
 ROOT = pathlib.Path(__file__).resolve().parent.parent.parent
 WORKING = ROOT / "src" / "gui"
 
 
 # datetime object containing current date and time
 now = datetime.now()
 
 loggey = logging.getLogger(name=__name__)
 
-# dd/mm/YY H:M:S
-dt_string = now.strftime("%d/%m/%Y %H:%M:%S")
-
 loggey.info(msg="class Megatron instatiated")
 data_vehicle: Megatron = Megatron()
 
 dpg.create_context()
 loggey.info(msg="Remote colors initialized")
 
 
-FREQ: dict[str, int] = {
-    "chan_1": 0,
-    "chan_2": 3,
-    "chan_3": 6,
-    "chan_4": 9,
-    "chan_5": 12,
-    "chan_6": 15,
-    "chan_7": 18,
-    "chan_8": 21,
-}
-
-POWS: dict[str, int] = {
-    "chan_1": 1,
-    "chan_2": 4,
-    "chan_3": 7,
-    "chan_4": 10,
-    "chan_5": 13,
-    "chan_6": 16,
-    "chan_7": 19,
-    "chan_8": 22,
-}
-
-BANDS: dict[str, int] = {
-    "chan_1": 2,
-    "chan_2": 5,
-    "chan_3": 8,
-    "chan_4": 11,
-    "chan_5": 14,
-    "chan_6": 17,
-    "chan_7": 20,
-    "chan_8": 23,
-}
-
-NAME: dict[str, int] = {
-    "chan_1": 24,
-    "chan_2": 25,
-    "chan_3": 26,
-    "chan_4": 27,
-    "chan_5": 28,
-    "chan_6": 29,
-    "chan_7": 30,
-    "chan_8": 31,
-}
-
 # Green Button Theme
 with dpg.theme() as grn_btn_theme, dpg.theme_component(dpg.mvAll):
     dpg.add_theme_color(dpg.mvThemeCol_Button, (0, 255, 0, 255))  # GREEN
 # Red Button Theme
 with dpg.theme() as red_btn_theme, dpg.theme_component(dpg.mvAll):
     dpg.add_theme_color(dpg.mvThemeCol_Button, (255, 0, 0, 255))  # RED
 # Blue Button Theme
@@ -104,32 +53,14 @@
 with dpg.theme() as orng_btn_theme, dpg.theme_component(dpg.mvAll):
     dpg.add_theme_color(dpg.mvThemeCol_Button, (255, 165, 0, 255))  # ORANGE
 
 # load the intial contents of the database for comparison upon new save
 loggey.info(msg="initial loading database")
 
 
-def version_getter() -> str | None:
-    """Get the latest version from the CHANGELOG file."""
-    # Touch the file if it doesn't exist
-    # pathlib.Path(ROOT / "CHANGELOG.md").touch()
-    with open(ROOT / "src" / "assets" / "CHANGELOG.cpy") as f:
-        for line in f:
-            if line.__contains__("##") and not line.__contains__(
-                    "YEAR MONTH DAY"):
-                correct_line = line.split("-")[0].strip()
-                version = correct_line.split("[")[1]
-
-                return version.strip("]")
-        return None
-
-
-VERSION: str | None = version_getter()
-
-
 def device_names() -> list[str]:
     """Use a bash script to list connected microarchitectures."""
     if platform.system().lower != "windows":
         # Avoid crashing program if there are no devices detected
         try:
             listing_script = [
                 # f'#!/bin/bash\n'
@@ -145,14 +76,15 @@
             devices: subprocess.CompletedProcess[str] = subprocess.run(
                 args=listing_script,
                 shell=True,
                 stdout=subprocess.PIPE,
                 text=True,
                 encoding="utf-8",
                 capture_output=False,
+                check=True,
             )
         except TypeError:
             loggey.warning(
                 msg=f"No devices detected | {device_names.__name__}")
             devices = subprocess.CompletedProcess(
                 args="",
                 returncode=1,
@@ -319,37 +251,39 @@
         serial_number: str = str(dpg.get_value(
             item="device_indicator"
         )).split(sep=":")[
             1
         ]
     except IndexError:
         loggey.error(
-            msg=f"No serial number found |{get_device_path_from_serial_number.__name__}()"
+            msg=f"No serial number found "
+            f"|{get_device_path_from_serial_number.__name__}()"
         )
         return "/dev/ttyACM0"
 
     # Get the list of devices in a list of dictionaries
     devices = return_teensy(DEVICE).items()
 
     # Loop through the list of devices and compare to serial number
     for device in devices:
         if int(device[0]) == int(serial_number):
             device_path = device[1]
             loggey.debug(msg=f"Device path: {device_path}")
 
             loggey.info(
-                f"Device path: {device_path} | {get_device_path_from_serial_number.__name__}()"
+                f"Device path: {device_path} |"
+                f" {get_device_path_from_serial_number.__name__}()"
             )
 
             return device_path
 
     return "No Match"
 
 
-TEENSY_DETAILS: dict() = return_teensy()
+TEENSY_DETAILS: dict = return_teensy()
 
 
 def compare_device_serial_to_config(serial_num: str) -> bool:
     """Compare the selected serial to the serial in the config."""
     # Get the device serial number directly from the GUI
 
     # Get the list of devices in a list of dictionaries
@@ -364,65 +298,68 @@
         loggey.warning(msg="No serial number found")
 
     # Loop through the list of devices and compare to serial number
     for device in devices:
         if device == int(serial_num):
             serial_number = device
             loggey.debug(
-                msg=f"Serial Number: {serial_number} matched | {compare_device_serial_to_config.__name__}()"
+                msg=f"Serial Number: {serial_number} matched |"
+                f" {compare_device_serial_to_config.__name__}()"
             )
             return True
 
     return False
 
 
 def validate_user_input(
     channel: int
 ):
     """Ensure the input fields respond as expected."""
     power_input = dpg.get_value(item=f"power_{channel}")
     band_input = dpg.get_value(item=f"bandwidth_{channel}")
     freq_input = dpg.get_value(item=f"freq_{channel}")
-    is_powerValid = True
-    is_bandValid = True
-    is_freqValid = True
+    is_power_valid = True
+    is_band_valid = True
+    is_freq_valid = True
     forbidden = ["*", "!", "@", "#", "$", "%", "^", "&", "*",
                  "(", ")", "_", "+", "=", """/""", "-", "?", ".."]
+
     # Checks if user input is blank, or has invalid characters
     for invalid in forbidden:
         match power_input, invalid:
             case ("", invalid):
                 dpg.set_value(item=f"power_{channel}", value="0")
-            case (powerString, invalid) if invalid in powerString:
+            case (power_string, invalid) if invalid in power_string:
                 dpg.set_value(item=f"power_{channel}", value="0")
-                is_powerValid = False
+                is_power_valid = False
         match band_input, invalid:
             case ("", invalid):
                 dpg.set_value(item=f"bandwidth_{channel}", value="0")
-            case (bandString, invalid) if invalid in bandString:
+            case (band_string, invalid) if invalid in band_string:
                 dpg.set_value(item=f"bandwidth_{channel}", value="0")
-                is_bandValid = False
+                is_band_valid = False
         match freq_input, invalid:
             case ("", invalid):
                 dpg.set_value(item=f"freq_{channel}", value="50")
-            case (freqString, invalid) if invalid in freqString:
+            case (freq_string, invalid) if invalid in freq_string:
                 dpg.set_value(item=f"freq_{channel}", value="50")
-                is_freqValid = False
-    # Checks if user inputs numbers past max value or below minimum value for all inputs
-    match is_powerValid, int(dpg.get_value(item=f"power_{channel}")):
+                is_freq_valid = False
+
+    # Checks if user inputs numbers past max value or below minimum value
+    match is_power_valid, int(dpg.get_value(item=f"power_{channel}")):
         case (True, value) if value > 100:
             dpg.set_value(item=f"power_{channel}", value="100")
         case (True, value) if value < 0:
             dpg.set_value(item=f"power_{channel}", value="0")
-    match is_bandValid, int(dpg.get_value(item=f"bandwidth_{channel}")):
+    match is_band_valid, int(dpg.get_value(item=f"bandwidth_{channel}")):
         case (True, value) if value > 100:
             dpg.set_value(item=f"bandwidth_{channel}", value="100")
         case (True, value) if value < 0:
             dpg.set_value(item=f"bandwidth_{channel}", value="0")
-    match is_freqValid, float(dpg.get_value(item=f"freq_{channel}")):
+    match is_freq_valid, float(dpg.get_value(item=f"freq_{channel}")):
         case (True, value) if value > 6400:
             dpg.set_value(item=f"freq_{channel}", value="6400")
         case (True, value) if value < 50:
             dpg.set_value(item=f"freq_{channel}", value="50")
 
 
 def callstack_helper(
@@ -520,254 +457,76 @@
     loggey.info("Kill All command Sent")
 
     [
         dpg.bind_item_theme(f"stats_{i+1}", orng_btn_theme)
         for i in range(8)
     ]
 
-    # data_vehicle.save_state(
-    # state=True,
-    # PORT=get_device_path_from_serial_number(),
-    # )
     data_vehicle.reset_board(
         PORT=get_device_path_from_serial_number(),
     )
 
     [
-        # Only change the Power to 0; No longer change the power level to 0
         (
             dpg.bind_item_theme(
                 f"stats_{i+1}",
                 grey_btn_theme),
-
-            # dpg.set_value(item=f"power_{i+1}", value=0),
         )
         for i in range(8)
     ]
 
     loggey.info("Ready for next command.\n")
 
 
-def send_all_channels(sender=None, app_data=None, user_data=None) -> None:
+def send_all_channels(
+        user_data=None,
+        sender=None,
+        app_data: tuple[Callable[[None], None]] = None
+) -> None:
     """Send the data from all channels at once."""
-    loggey.info(f"{send_all_channels.__name__}() executed")
-    for i in range(1, 9):
-        validate_user_input(channel=i)
-    callstack_helper(channel=1)
-    callstack_helper(channel=2)
-    callstack_helper(channel=3)
-    callstack_helper(channel=4)
-    callstack_helper(channel=5)
-    callstack_helper(channel=6)
-    callstack_helper(channel=7)
-    callstack_helper(channel=8)
+    loggey.debug("%s() executed", send_all_channels.__name__)
+    loggey.info("sender: %s", sender)
+    loggey.info("app_data: %s", app_data)
+    loggey.info("user_data: %s", user_data)
+
+    wifi_button_color = dpg.get_item_theme(item="mssn_scan_jam")
+    ble_button_color = dpg.get_item_theme(item="mssn_bluetooth_scan")
+    blue_theme = dpg.get_item_theme(item="send_btn_1")
+
+    if wifi_button_color != blue_theme:
+        app_data[0](callstack_helper)
+
+    elif ble_button_color != blue_theme:
+        app_data[1](callstack_helper)
+
+    else:
+        for i in range(1, 9):
+            validate_user_input(channel=i)
+
+        # This broke when in a for loop
+        callstack_helper(channel=1)
+        callstack_helper(channel=2)
+        callstack_helper(channel=3)
+        callstack_helper(channel=4)
+        callstack_helper(channel=5)
+        callstack_helper(channel=6)
+        callstack_helper(channel=7)
+        callstack_helper(channel=8)
 
-    no_power()
+        no_power()
 
     loggey.info("Ready for next command.\n")
 
 
-def quick_save(sender, app_data, user_data) -> None:
-    """Save the present inputs of the fields."""
-    prelim_data: list[dict[str, dict[str, str]]] = [
-        {
-            f"channel {channel}": {
-                "Power": dpg.get_value(f"power_{channel}"),
-                "Bandwidth": dpg.get_value(f"bandwidth_{channel}"),
-                "Frequency": dpg.get_value(f"freq_{channel}"),
-                "Date": dt_string,
-            },
-        }
-        for channel in range(1, 9)
-    ]
-
-    with open(file=f"{WORKING}/db/quick_save.json", mode="w") as file:
-        file.write(json.dumps(obj=prelim_data, indent=2))
-        loggey.info("Save Complete")
-
-
-def quick_load(sender, app_data, user_data) -> None:
-    """Load the last daved data."""
-    saved_data: list = []
-    try:
-        loggey.info("Opening the quick save file: quick_save.json")
-        with open(file=f"{WORKING}/db/quick_save.json") as file:
-            saved_data = json.loads(file.read())
-            [
-                (
-                    dpg.set_value(
-                        item=f"power_{channel}",
-                        value=saved_data[channel -
-                                         1][f"channel {channel}"]["Power"],
-                    ),
-                    dpg.set_value(
-                        item=f"bandwidth_{channel}",
-                        value=saved_data[channel -
-                                         1][f"channel {channel}"]["Bandwidth"],
-                    ),
-                    dpg.set_value(
-                        item=f"freq_{channel}",
-                        value=saved_data[channel -
-                                         1][f"channel {channel}"]["Frequency"],
-                    ),
-                )
-                for channel in range(1, 9)
-            ]
-            loggey.info("Quick load complete")
-
-    except SystemError:
-        loggey.error("No saved data found")
-        return
-
-
-def custom_save(sender, app_data, user_data) -> None:
-    """Save config w/ a custom name."""
-    loggey.debug(f"{custom_save.__name__}() executed")
-
-    try:
-        get_save_data()
-
-    except (
-            TypeError,
-            IndexError,
-            KeyError,
-            AttributeError,
-            ValueError,
-    ):
-        loggey.warning(msg=f"database failure | {custom_save.__name__}()")
-
-    # Clear input and close input
-    dpg.set_value(item="save_custom_input", value="")
-    dpg.configure_item(item="modal_save", show=False)
-
-
-def get_save_data() -> list[dict[str, str]]:
-    """Get the save data."""
-    return [
-        {
-            "save_name": dpg.get_value(item="save_custom_input"),
-            "power": dpg.get_value(f"power_{channel}"),
-            "bandwidth": dpg.get_value(f"bandwidth_{channel}"),
-            "frequency": dpg.get_value(f"freq_{channel}"),
-            "date": dt_string,
-        }
-        for channel in range(1, 9)
-    ]
-
-
-def custom_load(sender, app_data=None, user_data=None) -> None:
-    """Load config /w a custom name."""
-    loggey.info(f"{custom_load.__name__}() executed")
-
-    loggey.debug(msg="Attempting to load custom save data")
-
-    custom_load_to_sql: list[str] = []
-    try:
-        custom_load_to_sql = get_sql_save_names()
-    except sqlite3.DatabaseError:
-        loggey.warning(msg="No custom save file found")
-    init_save_data_length = custom_load_to_sql.__len__()
-
-    live_refresh(alias=["load", "delete"])
-    loggey.info(msg=f"Sender: {sender}")
-    with dpg.window(
-            modal=True,
-            popup=True,
-            tag="modal_loaded",
-            pos=(
-                0,  # dpg.get_viewport_client_width() // 2 - 100,
-                0,  # dpg.get_viewport_client_height() // 2 - 100,
-            ),
-    ):
-        {
-            (
-                dpg.add_menu_item(
-                    parent="modal_loaded",
-                    label=unique,
-                    tag=f"load_{itera + init_save_data_length}",
-                    callback=load_chosen,
-                    user_data=(unique, itera + init_save_data_length),
-                ),
-            )
-            if sender == "custom_load_button" or sender == 210
-            else (
-                dpg.add_menu_item(
-                    parent="modal_delete",
-                    label=unique,
-                    callback=delete_chosen,
-                    user_data=(unique, itera + init_save_data_length),
-                    tag=f"delete_{itera + init_save_data_length}",
-                    show=True,
-                )
-            )
-            for itera, unique in enumerate(custom_load_to_sql, start=0)
-        }
-        dpg.add_button(
-            label="Close",
-            parent="modal_loaded",
-            tag="close_modal_loaded",
-            callback=lambda: dpg.configure_item(
-                item="modal_loaded", show=False),
-        )
-
-
-def load_chosen(
-        sender=None, app_data=None, user_data: tuple[str, int] = ("", 0)
-) -> None:
-    """Take in the chosen file to be loaded to the input fields of the gui."""
-    loggey.info(f"{load_chosen.__name__}() executed")
-
-    _custom_load = get_sql_details(save_name=user_data[0])
-    _ret_data: tuple = _custom_load
-
-    [
-        (
-            dpg.set_value(item=f"freq_{itera}",
-                          value=_ret_data[FREQ[f"chan_{itera}"]]),
-            dpg.set_value(
-                item=f"power_{itera}", value=_ret_data[POWS[f"chan_{itera}"]]
-            ),
-            dpg.set_value(
-                item=f"bandwidth_{itera}", value=_ret_data[BANDS[f"chan_{itera}"]]
-            ),
-        )
-        for itera in range(1, 9)
-    ]
-
-
-def delete_chosen(
-        sender=None,
-        app_data=None,
-        user_data: tuple[str, int] = (str(), int()),
-) -> None:
-    """Delete a saved file."""
-    # Get the list of saved objects
-    _custom_load = get_sql_save_names()
-
-    # Get primary key for every name in the database matching the chosen name
-    if user_data[0] in _custom_load:
-        # Delete the chosen name and data from the database
-        loggey.info(f"Deleting {user_data[0]} | {delete_chosen.__name__}()")
-        delete_sql_save_data(save_name=user_data[0])
-
-    loggey.info(
-        f"Live update of delete and load menu items complete\
-            | {delete_chosen.__name__}()"
-    )
-
-
 def auto_fill_freq(
-        sender=None,
-        app_data=None,
-        user_data=None,
         freq_val: float = 0.0,
         freq_constant: float = 5.0,
 ) -> None:
     """Auto fill the frequency column based on the first input."""
-    [
+    _ = [
         dpg.set_value(
             item=f"freq_{i}",
             value=(
                 abs(
                     float(dpg.get_value(f"freq_{i-2}"))
                     - float(dpg.get_value(f"freq_{i-1}"))
                 )
@@ -776,15 +535,15 @@
             if float(dpg.get_value(item=f"freq_{i}")) <= 6400
             else 6400.00,
         )
         for i in range(3, 9)
         if not freq_constant
     ]
 
-    [
+    _ = [
         dpg.set_value(
             item=f"freq_{i}",
             value=freq_val + freq_constant * (i - 1)
         )
         for i in range(1, 9)
         if freq_constant
     ]
@@ -796,15 +555,15 @@
 
     # Ensure power_1 is greater than 0 and less than 100
     if int(power_1) <= 0:
         power_1 = 0
     elif int(power_1) >= 100:
         power_1 = 100
 
-    [
+    _ = [
         dpg.set_value(item=f"power_{i}", value=power_1)
         for i in range(1, 9)
     ]
 
 
 def auto_fill_bandwidth() -> None:
     """Auto fill the bandwidth column based on the first input."""
@@ -812,26 +571,28 @@
 
     # Ensure bandwidth_1 is greater than 0 and less than 100
     if int(bandwidth_1) <= 0:
         bandwidth_1 = 0
     elif int(bandwidth_1) >= 100:
         bandwidth_1 = 100
 
-    [
+    _ = [
         dpg.set_value(
             item=f"bandwidth_{i}",
             value=bandwidth_1,
         )
         for i in range(1, 9)
     ]
 
 
 def change_inputs(sender, app_data, user_data) -> None:
     """Use the mouse wheel to change the field inputs."""
-    loggey.info(f"app data: {app_data}")
+    loggey.info("app data: %s", app_data)
+    loggey.info("user data: %s", user_data)
+    loggey.info("sender: %s", sender)
 
     if dpg.is_item_focused(item="power_1"):
         loggey.debug(dpg.get_value("power_1"))
 
 
 def read_config(file: str) -> tuple[configparser.ConfigParser, list[str]]:
     """Read the config file and return the contents."""
@@ -843,26 +604,30 @@
     return parser, devices
 
 
 def auto_send(sender, app_data, user_data) -> None:
     """Set a flag to indicate when mission buttons should auto send."""
     loggey.debug(msg=f"{auto_send.__name__}()")
 
+    loggey.info("sender: %s", sender)
+    loggey.info("app_data: %s", app_data)
+    loggey.info("user_data: %s", user_data)
+
     # Set the button to green
     dpg.bind_item_theme(
         theme=grn_btn_theme if not dpg.get_item_theme(
             item=sender) == grn_btn_theme else None,
         item=sender,
     )
 
     global AUTO_SEND_FLAG
 
     # Set the flag
-    AUTO_SEND_FLAG = True if dpg.get_item_theme(
-        item=sender) == grn_btn_theme else False
+    AUTO_SEND_FLAG = dpg.get_item_theme(
+        item=sender) == grn_btn_theme
 
     loggey.debug(msg=f"Auto send flag: {AUTO_SEND_FLAG}")
 
 
 def mission(sender, app_data, user_data) -> None:
     """Mission alpha user facing button configuration."""
     name = sender.split("\n")[0].lower()
@@ -915,42 +680,44 @@
         # If SEND_AUTO_FLAG then SEND_ALL
         if AUTO_SEND_FLAG:
             loggey.info(msg=f"auto send flag: {AUTO_SEND_FLAG}")
             send_all_channels()
         else:
             loggey.info(msg=f"auto send flag: {AUTO_SEND_FLAG}")
 
-    except (KeyError, SystemError, NameError) as e:
-        loggey.warning(msg=f"Error: {e}")
+    except (KeyError, SystemError, NameError) as an_error:
+        loggey.warning(msg=f"Error: {an_error}")
 
 
-def kill_channel(sender, app_data, user_data: int) -> None:
+def kill_channel(user_data: int) -> None:
     """Kill channel w/out resetting power on user facing screen."""
     data_vehicle.change_power(
         channel=user_data,
         power_level=0,
         PORT=get_device_path_from_serial_number(),
     )
 
     dpg.bind_item_theme(
-        item=f"stats_{user_data}",
+        item=f"stats_{user_data.split('_')[-1]}",
         theme=grey_btn_theme)
 
 
-def device_finder(sender=None, app_data=None, user_data: int = int()) -> None:
+def device_finder(user_data: int = int()) -> None:
     """Filter all connected devices and present only Teensy devices."""
+
     loggey.info(msg=f"{device_finder.__name__}() executed")
     teensy_info: dict[str, str] = {}
 
     # Initial process the device names
     device = [device.split(sep="_") for device in device_names()]
 
     # filter and return only Teensy devices
     desired_device = [device for device in device if "Teensy" in device[0]]
-    loggey.info(msg=f"Devices filtered check: {desired_device} | {device_names.__name__}")
+    loggey.info(msg=f"Devices filtered check: {desired_device} |"
+                f"{device_names.__name__}")
 
     # Create the dictionary of the Teensy path and serial number
     for _i, val in enumerate(desired_device):
         teensy_info[val[-1]] = val[0].split(sep="-")[0]
     loggey.info(msg=f"Teensy info: {teensy_info} | {device_names.__name__}")
     # Can only choose a 'Teensy' device
     for _i, dev in enumerate(teensy_info, start=1):
@@ -1031,15 +798,17 @@
             if str(
                     dpg.get_value(item=f"power_{i}"),
             ) != str(card_stats["power"][i - 1]):
                 dpg.set_value(
                     item=f"power_{i}",
                     value=rev_convert_power(int(card_stats["power"][i - 1])),
                 )
-                dpg.bind_item_theme(item=f"stats_{i}", theme=grey_btn_theme) if str(
+                dpg.bind_item_theme(
+                    item=f"stats_{i}",
+                    theme=grey_btn_theme) if str(
                     dpg.get_value(item=f"power_{i}")
                 ) == "0" else dpg.bind_item_theme(
                     item=f"stats_{i}", theme=grn_btn_theme
                 )
 
             if str(
                     dpg.get_value(item=f"freq_{i}"),
@@ -1132,149 +901,83 @@
                             dpg.bind_item_theme(
                                 item=f"card_{dev_count}",
                                 theme=blue_btn_theme,
                             )
                             dpg.configure_item(
                                 item=f"card_{dev_count}", enabled=True)
                             loggey.debug(
-                                f"{card} is assigned to {parser['mgtron'][f'card_{dev_count}']}"
+                                f"{card} is assigned to "
+                                f"{parser['mgtron'][f'card_{dev_count}']}"
                             )
                         case False if len(card) == 1:
                             loggey.info(
-                                msg=f"No device filled in on this line {platform.machine()} | {config_intake.__name__}"
+                                msg="No device filled in on this line "
+                                f"{platform.machine()} | "
+                                f"{config_intake.__name__}"
                             )
                         case False:
                             loggey.warning(
-                                msg=f"Device ID not detected in order OR not at all on {platform.machine()} | {config_intake.__name__}"
+                                msg="Device ID not detected in order OR "
+                                f"not at all on {platform.machine()} | "
+                                f"{config_intake.__name__}"
                             )
         except (KeyError, SystemError):
             loggey.warning(
                 msg=f"No config file error | {config_intake.__name__}")
 
 
-def find_signals_and_frequencies() -> dict[int, float]:
-    """Use the linux host to scan for wifi signals and frequencies."""
-    output: subprocess.CompletedProcess = subprocess.run(
-        [
-            "nmcli",
-            "-g",
-            "FREQ",
-            "-c",
-            "no",
-            "dev",
-            "wifi",
-            "list",
-            "--rescan",
-            "yes",
-        ],
-        capture_output=True,
-        encoding="utf-8",
-    )
-
-    output_2: subprocess.CompletedProcess = subprocess.run(
-        [
-            "nmcli",
-            "-g",
-            "SIGNAL",
-            "-c",
-            "no",
-            "dev",
-            "wifi",
-            "list",
-        ],
-        capture_output=True,
-        encoding="utf-8",
-    )
-
-    signal_column: set[str] = set(output_2.stdout.split(sep="\n"))
-
-    freq_column: set[str] = set(output.stdout.split(sep="\n"))
-
-    matched_sigs_and_freqs: dict[int, float] = {
-        int(sig): float(freq.strip("MHz"))
-        for sig, freq in zip(signal_column, freq_column)
-        if sig != "" and freq != ""
-    }
-
-    # Sort the dictionary by the signal strength
-    matched_sigs_and_freqs = dict(
-        sorted(
-            matched_sigs_and_freqs.items(),
-            key=lambda item: item[0],
-            reverse=True)
-    )
-
-    loggey.info(
-        msg=f"Freq and Strength: {matched_sigs_and_freqs} | {find_signals_and_frequencies.__name__}"
-    )
-
-    # reduce the dictionary to the top 8 strongest signals
-    matched_sigs_and_freqs = dict(
-        itertools.islice(
-            matched_sigs_and_freqs.items(), 8))
-
-    # if the dictionry is not eight items long, fill it with zeros
-    if len(matched_sigs_and_freqs) < 8:
-        [
-            matched_sigs_and_freqs.update({1 + i: 50}) for i in range(
-                8 - len(matched_sigs_and_freqs)
-            )
-        ]
-        loggey.warning(
-            msg=f"Dictionary is not eight items long | {find_signals_and_frequencies.__name__}"
-        )
-
-    return matched_sigs_and_freqs
-
-
 def find_bluetooth_and_frequencies() -> bool:
     """Use the linux host to scan for bluetooth signals and frequencies."""
     # send the command: bluetootctl scan on
     subprocess.run(
         ["bluetoothctl", "scan", "on"],
         capture_output=True,
         encoding="utf-8",
+        check=False,
     )
 
     output: subprocess.CompletedProcess = subprocess.run(
         [
             "bluetoothctl",
             "scan",
             "on",
         ],
         capture_output=True,
         encoding="utf-8",
+        check=False,
     )
 
     hardware_column: set[str] = set(output.stdout.split(sep="\n"))
 
     hardware_ids = {
         int(hardware.split(sep=" ")[0]): int(hardware.split(sep=" ")[-1])
         for hardware in hardware_column
         if hardware != ""
     }
 
     # print the ordered dictionary
     loggey.info(
-        msg=f"Freq and Strength: {hardware_ids} | {find_bluetooth_and_frequencies.__name__}"
+        msg=f"Freq and Strength: {hardware_ids} | "
+        f"{find_bluetooth_and_frequencies.__name__}"
     )
 
     return len(hardware_ids) > 0
 
 
 def card_config(card_number: int = int()) -> None:
     """Read the config file and set the values in the GUI."""
     try:
         parser, _ = read_config(
             file=f"{WORKING}/_configs/card_{card_number}.ini")
 
         [
             (
                 dpg.set_value(
-                    item=f"freq_{config}", value=float(parser["freq"][f"freq_{config}"])
+                    item=f"freq_{config}",
+                    value=float(parser["freq"][f"freq_{config}"])
                 ),
                 dpg.set_value(
                     item=f"power_{config}",
                     value=int(parser["power"][f"power_{config}"]),
                 ),
                 dpg.set_value(
                     item=f"bandwidth_{config}",
@@ -1347,15 +1050,16 @@
                 msg=f"Card 1 config loaded | {card_selection.__name__}")
 
         case 2:
             dpg.bind_item_theme(
                 item=f"card_{user_data}", theme=grn_btn_theme
             )
             dpg.set_value(
-                item="device_indicator", value=f"Device:{parser['mgtron']['card_2']}"
+                item="device_indicator",
+                value=f"Device:{parser['mgtron']['card_2']}"
             )
             device_finder(user_data=int(parser["mgtron"]["card_2"]))
 
             card_list.remove(2)
 
             try:
                 [
@@ -1376,15 +1080,16 @@
 
         case 3:
             card_list.remove(3)
             dpg.bind_item_theme(
                 item=f"card_{user_data}", theme=grn_btn_theme
             )
             dpg.set_value(
-                item="device_indicator", value=f"Device:{parser['mgtron']['card_3']}"
+                item="device_indicator",
+                value=f"Device:{parser['mgtron']['card_3']}"
             )
             device_finder(user_data=int(parser["mgtron"]["card_3"]))
 
             try:
                 [
                     dpg.bind_item_theme(
                         item=f"card_{greyed_card}",
@@ -1402,15 +1107,16 @@
 
         case 4:
             card_list.remove(4)
             dpg.bind_item_theme(
                 item=f"card_{user_data}", theme=grn_btn_theme
             )
             dpg.set_value(
-                item="device_indicator", value=f"Device:{parser['mgtron']['card_4']}"
+                item="device_indicator",
+                value=f"Device:{parser['mgtron']['card_4']}"
             )
             device_finder(user_data=int(parser["mgtron"]["card_4"]))
 
             try:
                 [
                     dpg.bind_item_theme(
                         item=f"card_{greyed_card}",
@@ -1428,15 +1134,16 @@
 
         case 5:
             card_list.remove(5)
             dpg.bind_item_theme(
                 item=f"card_{user_data}", theme=grn_btn_theme
             )
             dpg.set_value(
-                item="device_indicator", value=f"Device:{parser['mgtron']['card_4']}"
+                item="device_indicator",
+                value=f"Device:{parser['mgtron']['card_4']}"
             )
             device_finder(user_data=int(parser["mgtron"]["card_4"]))
 
             try:
                 [
                     dpg.bind_item_theme(
                         item=f"card_{greyed_card}",
@@ -1454,15 +1161,16 @@
 
         case 6:
             card_list.remove(6)
             dpg.bind_item_theme(
                 item=f"card_{user_data}", theme=grn_btn_theme
             )
             dpg.set_value(
-                item="device_indicator", value=f"Device:{parser['mgtron']['card_6']}"
+                item="device_indicator",
+                value=f"Device:{parser['mgtron']['card_6']}"
             )
             device_finder(user_data=int(parser["mgtron"]["card_6"]))
 
             try:
                 [
                     dpg.bind_item_theme(
                         item=f"card_{greyed_card}",
@@ -1480,15 +1188,16 @@
 
         case 7:
             card_list.remove(7)
             dpg.bind_item_theme(
                 item=f"card_{user_data}", theme=grn_btn_theme
             )
             dpg.set_value(
-                item="device_indicator", value=f"Device:{parser['mgtron']['card_7']}"
+                item="device_indicator",
+                value=f"Device:{parser['mgtron']['card_7']}"
             )
             device_finder(user_data=int(parser["mgtron"]["card_7"]))
 
             try:
                 [
                     dpg.bind_item_theme(
                         item=f"card_{greyed_card}",
@@ -1506,15 +1215,16 @@
 
         case 8:
             card_list.remove(8)
             dpg.bind_item_theme(
                 item=f"card_{user_data}", theme=grn_btn_theme
             )
             dpg.set_value(
-                item="device_indicator", value=f"Device:{parser['mgtron']['card_8']}"
+                item="device_indicator",
+                value=f"Device:{parser['mgtron']['card_8']}"
             )
             device_finder(user_data=int(parser["mgtron"]["card_8"]))
 
             try:
                 [
                     dpg.bind_item_theme(
                         item=f"card_{greyed_card}",
@@ -1546,171 +1256,14 @@
                 loggey.error(
                     msg=f"No card data loaded | {card_selection.__name__}")
             except SystemError:
                 loggey.warning(msg="Other cards not found")
                 return
 
 
-def wifi_scan_jam(sender, app_data, user_data) -> None:
-    """Scan the local wifi channels and jam them."""
-    loggey.info(msg="Scan jammer method called")
-
-    dpg.configure_item(item=sender, label="SCANNING...")
-    dpg.bind_item_theme(item=sender, theme=red_btn_theme)
-
-    loggey.info(msg="SCANNING...")
-    freq_and_strength: dict[int, float] = find_signals_and_frequencies()
-
-    loggey.warning(msg=f"Freq & Strength sorted: {freq_and_strength}")
-
-    [
-        (
-            dpg.set_value(
-                item=f"freq_{i}", value=float(freq) if isinstance(
-                    freq, float
-                ) else 50.0
-            ),
-            dpg.set_value(
-                item=f"power_{i}",
-                value=100 if int(freq) != 50 else 0),
-            dpg.set_value(
-                item=f"bandwidth_{i}",
-                value=10 if int(freq) != 50 else 0),
-            loggey.debug(
-                msg=f"Frequency, in sig strength order, discovered: {freq}"
-            ),
-            # Automatically send the command to the MGTron board
-        )
-        for i, freq in enumerate(freq_and_strength.values(), start=1)
-    ]
-
-    # # Stop looping scan jam if 'KILL ALL' is pressed and hovered over
-    # if dpg.is_item_focused(test
-    #         item="Stop_all_channels"):
-
-    # Change the button back to blue
-    dpg.bind_item_theme(
-        item=sender,
-        theme=blue_btn_theme,
-    )
-
-    # Change the button text back to normal
-    dpg.configure_item(
-        item=sender,
-        label="WIFI",
-    )
-
-    loggey.debug(msg="Scan jammer method finished")
-
-
-def bluetooth_scan_jam(sender, app_data, user_data) -> None:
-    """Scan the local bluetooth channels and jam them."""
-    loggey.info(msg="Scan jammer method called")
-
-    try:
-        # Conditional lgic to determine if the scan is in progress
-        if dpg.get_item_theme(item=sender) == orng_btn_theme:
-            dpg.bind_item_theme(
-                item=sender,
-                theme=blue_btn_theme,
-            )
-            dpg.configure_item(
-                item=sender,
-                label="  BLUETOOTH\n   SCAN",
-            )
-            loggey.debug(msg="Bluetooth scan button disabled")
-
-            # Delete the open bluetooth scan window
-            dpg.delete_item(item=12)
-            loggey.debug(msg="Bluetooth scan window deleted")
-
-        else:
-
-            # Launch the window that will show the bluetooth information
-            dpg.bind_item_theme(
-                item=sender,
-                theme=orng_btn_theme,
-            )
-            dpg.configure_item(
-                item=sender,
-                label="  CLOSE\n  BLUETOOTH\n   SCAN",
-            )
-            loggey.debug(msg="Bluetooth scan button enabled")
-
-            with dpg.window(
-                tag=12,
-                no_scrollbar=True,
-                no_collapse=True,
-                no_resize=True,
-                no_title_bar=True,
-                no_move=True,
-                pos=(0, 0),
-                width=880,
-                height=735,
-            ):
-                with dpg.child_window(
-                    tag="ble_labels",
-                    pos=(0, 0),
-                    width=880,
-                    height=715,
-                ):
-                    dpg.add_text(
-                        default_value=" " * 14 + "MAC" + " " * 5 + "|" + " " * 2 +
-                        "MANUFACTURER" + " " * 1 + "|" + " " +
-                        "RSSI" + " " * 2 + "|" + " " * 12 + "DATE",
-                        label="BLUETOOTH LIST",
-                    )
-                    dpg.add_text(
-                        default_value='-'*89
-                    )
-
-                with dpg.child_window(
-                    tag="ble_list",
-                    no_scrollbar=True,
-                    pos=(0, 60),
-                    width=880,
-                    height=680,
-                ):
-
-                    # Get the BLE dict information and print to GUI
-                    all_data: dict = ble_data_complete()
-
-                    for i, data in enumerate(all_data, start=1):
-
-                        try:
-                            # MAC | MANUFACTURER | RSSI | DATE
-                            print_to_user = f"{i}. "\
-                                f"{data[0]}"\
-                                f"{' '* (1 if i > 9 else 2)}|"\
-                                f"{' '* (1 if i > 9 else 1)}"\
-                                f"{data[1][0]}"\
-                                f"{' '* (14 - len(data[1][0]) + 1) if i > 9 else ' ' * (15 - len(data[1][0]))}|"\
-                                f"  {data[1][1]}  | "\
-                                f" {datetime.now().strftime('%H:%M:%S')}"
-                        except TypeError:
-                            print_to_user = f"{i}. "\
-                                "NO CONNECTION ESTABLISHED"
-
-                        loggey.info(data)
-
-                        dpg.add_text(
-                            default_value=print_to_user
-                        )
-                        dpg.add_text(
-                            default_value='-' * 78
-                        )
-
-    except SystemError:
-        loggey.error(msg="Bluetooth scan window not found")
-        no_power()
-        return
-
-    no_power()
-
-
 def get_card_status() -> dict[str, list]:
     """Grab the status of the card for state tracking."""
     card_data: dict[str, list] = {}
 
     # Get the path of the presently selected device
     path = get_device_path_from_serial_number()
 
@@ -1760,62 +1313,14 @@
     dpg.configure_item(item=f"bandwidth_{channel}_indicator", show=False)
 
 
 def db_error(sender=None, app_data=None, user_data=None) -> None:
     """Display a modal popup with the error message."""
 
 
-def check_and_load_config(button_name: str) -> dict[str, list]:
-    """Check database for config button as the name of the saved config."""
-    loggey.debug(msg=f"{check_and_load_config}()")
-    config_data: dict[str, list] = {}
-
-    # Check the sql database for the name of the button
-    save_names = get_sql_save_names()
-
-    # Remove new lines and rejoin sentence; this is ! robust
-    button_name = button_name.replace("  ", " ").replace("\n", "")
-
-    loggey.info(f"DB names: {save_names}")
-    loggey.info(f"Button name: '{button_name}'")
-
-    if button_name in save_names:
-        loggey.debug(f"Button name: {button_name} found in DB")
-
-        # Get the config from the database
-        config = get_sql_details(save_name=button_name)
-
-        loggey.debug(config)
-
-        # Get the channel, frequency, power, and bandwidth
-        channel: list[int] = [int(i) for i in range(1, 9)]
-        frequency: list[float] = [
-            float(config[FREQ[
-                f"chan_{i}"]]) for i, _ in enumerate(FREQ, start=1)
-        ]
-        power: list[int] = [
-            int(config[POWS[
-                f"chan_{i}"]]) for i, _ in enumerate(POWS, start=1)
-        ]
-        bandwidth: list[int] = [
-            int(config[BANDS[
-                f"chan_{i}"]]) for i, _ in enumerate(BANDS, start=1)
-        ]
-
-        # Store the config in a dictionary
-        config_data: dict[str, list] = {
-            "channel": channel,
-            "freq": frequency,
-            "power": power,
-            "bw": bandwidth,
-        }
-
-    return config_data
-
-
 def convert_power(power: int) -> int:
     """Map the input from 0 to 100 and convert to 0 to 63."""
     loggey.debug(msg=f"{convert_power.__name__}()")
 
     loggey.info(msg=f"Power prior to conversion: {power}")
     # Map the input from 0 to 100 and convert to 0 to 63
     try:
@@ -1846,15 +1351,15 @@
     if power > 63:
         power = 63
 
     return power
 
 
 def rev_convert_power(power: int) -> int:
-    """Map the input from 0 to 63 and convert to 0 to 100"""
+    """Map the input from 0 to 63 and convert to 0 to 100."""
     loggey.debug(msg=f"{rev_convert_power.__name__}()")
 
     loggey.info(msg=f"Power prior to conversion: {power}")
 
     # Map the input from 0 to 63 and convert to 0 to 100
     power = int(
         round(
@@ -1876,15 +1381,15 @@
 def map_range(
     x: int,
     in_min: int,
     in_max: int,
     out_min: int,
     out_max: int,
 ) -> float:
-    """Map the input from 0 to 100 and convert to 0 to 63"""
+    """Map the input from 0 to 100 and convert to 0 to 63."""
     return (x - in_min) * (out_max - out_min) / (in_max - in_min) + out_min
 
 
 def change_card_name(sender, app_data, user_data) -> None:
     """Change the name of the card select button that is currently selected."""
     # Parse the sender to get the card select button
     # by splitting the sender string on the underscore
@@ -1911,26 +1416,14 @@
 def save_init():
     """Save the current config to the init file."""
     loggey.debug(msg="Saving init file")
 
     dpg.save_init_file("dpg.ini")
 
 
-def live_refresh(alias: list[str]):
-    """For as many aliases passed in, remove from the dpg registry."""
-    loggey.debug(msg=f"{live_refresh.__name__}()")
-
-    for i in dpg.get_aliases():
-        for j in alias:
-            if i.__contains__(j):
-                dpg.remove_alias(alias=i)
-                loggey.debug(f"Removed alias: {i}")
-                loggey.debug(msg=f"Removed alias: {i}")
-
-
 def connect_device(sender, app_data, user_data) -> None:
     """Connect to the device and send the config to the GUI."""
     try:
         # Grab the list of Teensy devices connected
         devices: dict[str, str] = return_teensy(DEVICE)
 
         if len(devices) == 1:
```

### Comparing `mgtron-2.17.1/src/gui/interface.py` & `mgtron-2.18.0/src/gui/interface.py`

 * *Files identical despite different names*

### Comparing `mgtron-2.17.1/src/main.py` & `mgtron-2.18.0/src/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,45 +1,50 @@
 """GUI especially used to utilize the MGTron API."""
 
-#!/usr/bin/env python3  # noqa: E265
-# -*- coding: utf-8 -*-
+#!/usr/bin/env python3 # noqa: E265 -*- coding: utf-8 -*-
 
 
+import sys
 import logging
 import pathlib
 from typing import Any
 
-
 import dearpygui.dearpygui as dpg
 
-from src.gui.helpers import DEVICE
-from src.gui.helpers import change_card_name
-from src.gui.helpers import compare_device_serial_to_config
-from src.gui.helpers import mission
-from src.gui.helpers import populate_right_side_buttons
-from src.gui.helpers import bluetooth_scan_jam
-from src.gui.helpers import custom_save
-from src.gui.helpers import VERSION
-from src.gui.helpers import auto_fill_bandwidth
-from src.gui.helpers import auto_fill_freq
-from src.gui.helpers import auto_fill_power
-from src.gui.helpers import card_selection
-from src.gui.helpers import custom_load
-from src.gui.helpers import device_finder
-from src.gui.helpers import device_refresh
-from src.gui.helpers import fill_config
-from src.gui.helpers import kill_channel
-from src.gui.helpers import quick_load
-from src.gui.helpers import quick_save
-from src.gui.helpers import reset_button
-from src.gui.helpers import return_teensy
-from src.gui.helpers import send_all_channels
-from src.gui.helpers import send_vals
-from src.gui.helpers import wifi_scan_jam
-from src.gui.helpers import auto_send
+from .gui.helpers import DEVICE
+from .gui.helpers import change_card_name
+from .gui.helpers import compare_device_serial_to_config
+from .gui.helpers import mission
+from .gui.helpers import populate_right_side_buttons
+from .gui.helpers import auto_fill_bandwidth
+from .gui.helpers import auto_fill_freq
+from .gui.helpers import auto_fill_power
+from .gui.helpers import card_selection
+from .gui.helpers import device_finder
+from .gui.helpers import device_refresh
+from .gui.helpers import kill_channel
+from .gui.helpers import reset_button
+from .gui.helpers import return_teensy
+from .gui.helpers import send_all_channels
+from .gui.helpers import send_vals
+from .gui.helpers import auto_send
+
+from .wifi.helpers import wifi_scan_jam
+from .wifi.helpers import wifi_kill_all
+
+from .db.helpers import custom_save
+from .db.helpers import quick_load
+from .db.helpers import quick_save
+from .db.helpers import custom_load
+from .db.helpers import delete_chosen
+
+from .ble.helpers import bluetooth_scan_jam
+from .ble.helpers import bluetooth_defeat
+
+from .globals.helpers import version_getter
 
 
 ROOT = pathlib.Path(__file__).resolve().parent
 
 logger = logging.getLogger(name=__name__)
 
 logger.debug(msg=f"Working dir: {ROOT}")
@@ -59,29 +64,20 @@
 CELLUAR_HEIGHT: int = -560
 MAIN_TABLE_HEIGHT: int = 1
 BUTTON_WIDTH = 120
 
 
 def main() -> None:
     """Function for ci/cd purpose for the GUI."""
-    # launch_ble_server(path=f"{ROOT}/assets/blueio_rs")
 
     dpg.create_context()
 
-    # print(f"\nID: {process_id}\n")
-    # os.kill(process_id+1, signal.SIGTERM)
-
-    # start_server._stop()
-    # Print in red that the thread is killed
-    # print("\n\033[91m{}\033[00m\n" .format("Thread killed"))
-    # start_server.join()
-
     logger.info(msg="creating dpg context")
 
-    fill_config()
+    # fill_config()
 
     logger.info(msg="Setting GUI colors")
     # Green Button Theme
     with dpg.theme() as grn_btn_theme:
         with dpg.theme_component(dpg.mvAll):
             dpg.add_theme_color(
                 dpg.mvThemeCol_Button, (0, 255, 0, 255))  # GREEN
@@ -228,29 +224,27 @@
                     height=ROW_HEIGHT,
                 ):
 
                     dpg.add_input_text(
                         tag=f"freq_{i+1}",
                         decimal=True,
                         # default_value=650.00 * ((i + 1)),
-                        # min_value=50.00,
-                        # max_value=6400.00,
-                        # min_clamped=True,
-                        # max_clamped=True,
+                        # min_value=50.00, max_value=6400.00,
+                        # min_clamped=True, max_clamped=True,
                         width=dpg.get_item_width(
                             item=f"freq_win_{i+1}") // 1.8,
-                        # step=1,
-                        # step_fast=100,
+                        # step=1, step_fast=100,
                         pos=(
                             dpg.get_item_pos(item="freq_win_1")[0],  # x
                             ROW_HEIGHT // 2 - 15  # y
                         ),
                     )
 
-                    # Indicate the frequency as queried from the device
+                    # Indicate the frequency as queried from the
+                    # device
                     dpg.add_text(
                         default_value="",
                         tag=f"frequency_{i+1}_indicator",
                         pos=(
                             dpg.get_item_width(
                                 item=f"freq_{i+1}") / 1.36,
                             0
@@ -266,18 +260,16 @@
                     width=180,
                     height=ROW_HEIGHT,
                 ):
 
                     dpg.add_input_text(
                         tag=f"power_{i+1}",
                         decimal=True,
-                        # min_value=0,
-                        # max_value=100,
-                        # min_clamped=True,
-                        # max_clamped=True,
+                        # min_value=0, max_value=100,
+                        # min_clamped=True, max_clamped=True,
                         width=dpg.get_item_width(
                             item=f"power_win_{i+1}") / 2.5,
                         # step_fast=3,
                         pos=(
                             dpg.get_item_pos(item="power_win_1")[
                                 0] // 2 - dpg.get_item_width(
                                     item=f"power_win_{i+1}") / 1.8,
@@ -305,30 +297,29 @@
                     width=180,
                     height=ROW_HEIGHT,
                 ):
 
                     dpg.add_input_text(
                         tag=f"bandwidth_{i+1}",
                         decimal=True,
-                        # min_value=0,
-                        # max_value=100,
-                        # min_clamped=True,
-                        # max_clamped=True,
+                        # min_value=0, max_value=100,
+                        # min_clamped=True, max_clamped=True,
                         width=dpg.get_item_width(
                             item=f"bandwidth_win_{i+1}") / 2.5,
                         # step_fast=10,
                         pos=(
                             dpg.get_item_pos(item="bandwidth_win_1")[
                                 0] // 2 - dpg.get_item_width(
                                     item=f"bandwidth_win_{i+1}"),
                             ROW_HEIGHT // 2 - 15
                         )
                     )
 
-                    # Indicate the bandwidth as queried from the device
+                    # Indicate the bandwidth as queried from the
+                    # device
                     dpg.add_text(
                         default_value="",
                         tag=f"bandwidth_{i+1}_indicator",
                         pos=(
                             dpg.get_item_width(
                                 item=f"bandwidth_{i+1}") / 0.9,
                             0
@@ -417,23 +408,24 @@
                     pos=(
                         dpg.get_item_width(item="auto_fill") / 1.3,
                         dpg.get_item_height(
                             item="auto_fill") / 3 - 10,
                     ),
                 )
 
-            [
+            _ = [
                 (
                     dpg.bind_item_theme(
                         item=f"send_btn_{i+1}", theme=blue_btn_theme),
                     dpg.bind_item_theme(
                         item=f"stats_{i+1}", theme=grey_btn_theme),
                 )
                 for i in range(8)
-            ]  # Propgation loop; Start the GUI w/ the indicator buttons grey
+            ]  # Propgation loop; Start the GUI w/ the indicator
+            # buttons grey
 
             ##################
             # ACTION BUTTONS #
             ##################
             with dpg.child_window(
                 pos=(680,),
                 tag="device_config",
@@ -470,20 +462,21 @@
 
                     try:
                         # Grab the list of Teensy devices connected
                         devices: dict[str, str] = return_teensy(DEVICE)
 
                         if len(devices) == 1:
 
-                            # Get the serial number of the device directly
+                            # Get the serial number of the device
+                            # directly
                             dpg.add_menu_item(
                                 label=f"{devices.popitem()[0].upper()}", )
 
                         elif len(devices) > 1:
-                            [
+                            _ = [
                                 (
                                     dpg.add_menu_item(
                                         label=f"{device.upper()}",
                                         callback=device_finder,
                                         user_data=device,
                                     )
                                 )
@@ -491,15 +484,16 @@
                             ]
                         else:
                             pass  # Error handled elsewhere
 
                         dpg.add_text(
                             parent="device_config",
                             tag="device_indicator",
-                            default_value=f"Device:{(k for k in return_teensy(DEVICE)).__next__()}",
+                            default_value="Device: "
+                            f"{(k for k in return_teensy(DEVICE)).__next__()}",
                             pos=(
                                 5,
                                 35
                             ),
                         )
 
                     except (
@@ -515,15 +509,15 @@
                             label="DEVICE NUMBER: NOT FOUND",
                             callback=lambda: dpg.configure_item(
                                 item="modal_device_config", show=False
                             ),
                         )
                         logger.error(msg="No device detected")
 
-                        [
+                        _ = [
                             dpg.bind_item_theme(
                                 item=f"stats_{channel}",
                                 theme=red_btn_theme,
                             )
                             for channel in range(1, 9)
                         ]
                         dpg.add_text(
@@ -543,15 +537,15 @@
                 height=dpg.get_item_height(
                     item="Primary Window") // 1.72,
                 no_scrollbar=True,
                 border=False,
             ):
 
                 ####################
-                # Reset All button #
+                # Stop All button #
                 ####################
                 logger.info(msg="Stop ALL button initialized")
                 reset_all = dpg.add_button(
                     tag="Stop_all_channels",
                     height=85,
                     width=BUTTON_WIDTH,
                     callback=reset_button,
@@ -585,22 +579,23 @@
                 ###################
                 logger.info(msg="SEND ALL button initialized")
                 send_all = dpg.add_button(
                     tag="Send All",
                     height=85,
                     width=BUTTON_WIDTH,
                     callback=send_all_channels,
+                    user_data=(wifi_kill_all, bluetooth_defeat),
                     pos=(
                         (
                             dpg.get_item_width(
                                 item="big_buttons"
-                            ) - 260) /
+                            ) - 260
+                        ) /
                         DIVISOR,
                         (
-
                             dpg.get_item_height(item="big_buttons") -
                             SEND_RESET_ALL_HEIGHT
                         ) / 2,
                     ),
                 )
 
                 dpg.add_text(
@@ -644,16 +639,16 @@
                     ),
                 )
 
                 #####################
                 # Quick Load button #
                 #####################
                 logger.info(msg="Quick Load button initialized")
-                load_all = dpg.add_button(
-                    tag="load_all",
+                quick__load = dpg.add_button(
+                    tag="quick_load",
                     callback=quick_load,
                     label="QUICK\n LOAD",
                     height=70,
                     width=BUTTON_WIDTH,
                     pos=(
                         (
                             dpg.get_item_width(
@@ -732,17 +727,17 @@
                     ),
                 )
 
                 ############################
                 # Delete Saved Item button #
                 ############################
                 dpg.add_button(
-                    parent="big_buttons",
+                    parent="delete_buttons",
                     label="DELETE",
-                    callback=custom_load,
+                    callback=delete_chosen,
                     tag="delete_button",
                     pos=(
                         (
                             dpg.get_item_width(item="big_buttons") - 10) /
                         DIVISOR,
                         (
                             dpg.get_item_height(
@@ -992,25 +987,25 @@
                 pos=(
                     RESOLUTION[0] - 86,
                     10,
                 ),
                 border=False,
             ):
 
-                [
+                _ = [
                     (
                         dpg.add_button(
                             label=f"CARD {card}",
                             tag=f"card_{card}",
                             height=60,
                             width=65,
                             pos=(0, 85 * card - 72),
                             callback=card_selection,
                             user_data=card,
-                            enabled=True if exists else False,
+                            enabled=bool(exists),
                         ),
                         dpg.bind_item_theme(
                             item=f"card_{card}",
                             theme=blue_btn_theme
                         ),
                     )
                     for card, exists in
@@ -1020,18 +1015,18 @@
                 with dpg.popup(
                     tag="card_popup",
                     parent="card_1",
                     modal=True,
                     mousebutton=dpg.mvMouseButton_Right,
                 ):
 
-                    [
+                    _ = [
                         (
-                            # Input text, if the card exists, to change
-                            # the name of the card
+                            # Input text, if the card exists, to
+                            # change the name of the card
                             dpg.add_input_text(
                                 label=f"Card {card} Name",
                                 tag=f"card_{card}_input",
                                 default_value=f"card_{card}",
                                 callback=change_card_name,
                                 width=200,
                                 # user_data=dpg.get_item_parent(item=f"card_{1}_input:"),
@@ -1091,15 +1086,14 @@
                                 )) else dpg.bind_item_theme(
                                 item="card_1",
                                 theme=grn_btn_theme
                             )
                         except KeyError:
                             logger.error(
                                 msg="No devices detected, disabling card 1")
-                            pass
 
             ###############
             # Version Tag #
             ###############
 
             with dpg.child_window(
                 tag="version",
@@ -1110,41 +1104,40 @@
                 pos=(
                     RESOLUTION[0] - 80,
                     RESOLUTION[1] - 30,
                 ),
             ):
 
                 dpg.add_text(
-                    default_value=f"ver. {VERSION}",
+                    default_value=f"ver. {version_getter()}",
                     tag="ver_num",
                 )
     except SystemError:
         logger.error(msg="No devices detected")
 
     try:  # Stop gap in case the font files cannot be found
         dpg.bind_font(font=ital_font)
         dpg.bind_item_font(item="ver_num", font=small_font)
 
-        [
+        _ = [
             (
                 dpg.bind_item_font(item=f"freq_{i}", font=bold_font),
                 dpg.bind_item_font(item=f"power_{i}", font=bold_font),
                 dpg.bind_item_font(item=f"bandwidth_{i}", font=bold_font),
                 dpg.bind_item_font(item=f"channel_{i}",
                                    font=default_font_added
                                    ),
             )
             for i in range(1, 9)
         ]
 
     except SystemError:
         logger.warning(msg="Font files error")
 
-    # Get the start up state of the card
-    # start_up_card_state()
+    # Get the start up state of the card start_up_card_state()
 
     # Global Theme
     with dpg.theme() as global_theme:
 
         with dpg.theme_component(dpg.mvAll):
             dpg.add_theme_style(
                 dpg.mvStyleVar_FrameRounding, 5, category=dpg.mvThemeCat_Core
@@ -1154,45 +1147,44 @@
             dpg.add_theme_style(
                 dpg.mvStyleVar_FrameRounding, 5, category=dpg.mvThemeCat_Core
             )
 
     # Button colors and global theme
     blue_btn_list: list[Any] = [
         save_all,
-        load_all,
+        quick__load,
         custom_save_button,
         mission_golf_button,
         mission_alpha_button,
         custom_load_button,
         mission_bravo_button,
         mission_charlie_button,
         mission_delta_button,
         mission_echo_button,
         mission_fox_button,
         wifi_scan_jam_button,
     ]
 
     dpg.bind_theme(global_theme)
 
-    [
+    _ = [
         dpg.bind_item_theme(
             item=btn,
             theme=blue_btn_theme,
         )
         for btn in blue_btn_list
     ]
     dpg.bind_item_theme(item=send_all, theme=grn_btn_theme)
     dpg.bind_item_theme(item=reset_all, theme=red_btn_theme)
 
     ############################
     # DearPyGUI required setup #
     ############################
-    TM = ""  # chr(169) #to_superscript('TM')
     dpg.create_viewport(
-        title=f"CellAntenna MGTron {TM}",
+        title="CellAntenna MGTron",
         width=RESOLUTION[0],
         height=RESOLUTION[1],
         resizable=True,
         always_on_top=True,
         x_pos=0,
         y_pos=0,
         small_icon=f"{ROOT}/gui/assets/network_wireless.ico",
@@ -1206,14 +1198,14 @@
         while dpg.is_dearpygui_running():
             # Place per frame code here
 
             dpg.render_dearpygui_frame()
     except KeyboardInterrupt:
         logger.info(msg="Ctrl C executed")
 
-        exit(0)
+        sys.exit(0)
 
     dpg.destroy_context()
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `mgtron-2.17.1/src/tests/test_configfiles.py` & `mgtron-2.18.0/src/tests/test_configfiles.py`

 * *Files identical despite different names*

### Comparing `mgtron-2.17.1/src/tests/test_helpers.py` & `mgtron-2.18.0/src/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `mgtron-2.17.1/venv/bin/rst2html.py` & `mgtron-2.18.0/venv/bin/rst2pseudoxml.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-#!/home/djhunter67/Documents/work_worK_woRk_wOrk_Work/mg_tron/venv/bin/python
+#!/home/djhunter67/Documents/work_worK_woRk_wOrk_Work/mg_tron/venv/bin/python3.11
 
-# $Id: rst2html.py 9115 2022-07-28 17:06:24Z milde $
+# $Id: rst2pseudoxml.py 9115 2022-07-28 17:06:24Z milde $
 # Author: David Goodger <goodger@python.org>
 # Copyright: This module has been placed in the public domain.
 
 """
-A minimal front end to the Docutils Publisher, producing HTML.
+A minimal front end to the Docutils Publisher, producing pseudo-XML.
 """
 
 try:
     import locale
     locale.setlocale(locale.LC_ALL, '')
 except Exception:
     pass
 
 from docutils.core import publish_cmdline, default_description
 
 
-description = ('Generates (X)HTML documents from standalone reStructuredText '
-               'sources.  ' + default_description)
+description = ('Generates pseudo-XML from standalone reStructuredText '
+               'sources (for testing purposes).  ' + default_description)
 
-publish_cmdline(writer_name='html', description=description)
+publish_cmdline(description=description)
```

### Comparing `mgtron-2.17.1/venv/bin/rst2html4.py` & `mgtron-2.18.0/venv/bin/rst2html4.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#!/home/djhunter67/Documents/work_worK_woRk_wOrk_Work/mg_tron/venv/bin/python
+#!/home/djhunter67/Documents/work_worK_woRk_wOrk_Work/mg_tron/venv/bin/python3.11
 
 # $Id: rst2html4.py 9115 2022-07-28 17:06:24Z milde $
 # Author: David Goodger <goodger@python.org>
 # Copyright: This module has been placed in the public domain.
 
 """
 A minimal front end to the Docutils Publisher, producing (X)HTML.
```

### Comparing `mgtron-2.17.1/venv/bin/rst2html5.py` & `mgtron-2.18.0/venv/bin/rst2html5.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#!/home/djhunter67/Documents/work_worK_woRk_wOrk_Work/mg_tron/venv/bin/python
+#!/home/djhunter67/Documents/work_worK_woRk_wOrk_Work/mg_tron/venv/bin/python3.11
 # :Copyright: © 2015 Günter Milde.
 # :License: Released under the terms of the `2-Clause BSD license`_, in short:
 #
 #    Copying and distribution of this file, with or without modification,
 #    are permitted in any medium without royalty provided the copyright
 #    notice and this notice are preserved.
 #    This file is offered as-is, without any warranty.
```

### Comparing `mgtron-2.17.1/venv/bin/rst2latex.py` & `mgtron-2.18.0/venv/bin/rst2latex.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#!/home/djhunter67/Documents/work_worK_woRk_wOrk_Work/mg_tron/venv/bin/python
+#!/home/djhunter67/Documents/work_worK_woRk_wOrk_Work/mg_tron/venv/bin/python3.11
 
 # $Id: rst2latex.py 9115 2022-07-28 17:06:24Z milde $
 # Author: David Goodger <goodger@python.org>
 # Copyright: This module has been placed in the public domain.
 
 """
 A minimal front end to the Docutils Publisher, producing LaTeX.
```

### Comparing `mgtron-2.17.1/venv/bin/rst2man.py` & `mgtron-2.18.0/venv/bin/rst2man.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#!/home/djhunter67/Documents/work_worK_woRk_wOrk_Work/mg_tron/venv/bin/python
+#!/home/djhunter67/Documents/work_worK_woRk_wOrk_Work/mg_tron/venv/bin/python3.11
 
 # Author:
 # Contact: grubert@users.sf.net
 # Copyright: This module has been placed in the public domain.
 
 """
 man.py
```

### Comparing `mgtron-2.17.1/venv/bin/rst2odt.py` & `mgtron-2.18.0/venv/bin/rst2odt.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#!/home/djhunter67/Documents/work_worK_woRk_wOrk_Work/mg_tron/venv/bin/python
+#!/home/djhunter67/Documents/work_worK_woRk_wOrk_Work/mg_tron/venv/bin/python3.11
 
 # $Id: rst2odt.py 9115 2022-07-28 17:06:24Z milde $
 # Author: Dave Kuhlman <dkuhlman@rexx.com>
 # Copyright: This module has been placed in the public domain.
 
 """
 A front end to the Docutils Publisher, producing OpenOffice documents.
```

### Comparing `mgtron-2.17.1/venv/bin/rst2odt_prepstyles.py` & `mgtron-2.18.0/venv/bin/rst2odt_prepstyles.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#!/home/djhunter67/Documents/work_worK_woRk_wOrk_Work/mg_tron/venv/bin/python
+#!/home/djhunter67/Documents/work_worK_woRk_wOrk_Work/mg_tron/venv/bin/python3.11
 
 # Copyright: This module has been placed in the public domain.
 
 """
 Adapt a word-processor-generated styles.odt for odtwriter use:
 
 Drop page size specifications from styles.xml in STYLE_FILE.odt.
```

### Comparing `mgtron-2.17.1/venv/bin/rst2s5.py` & `mgtron-2.18.0/venv/bin/rst2s5.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#!/home/djhunter67/Documents/work_worK_woRk_wOrk_Work/mg_tron/venv/bin/python
+#!/home/djhunter67/Documents/work_worK_woRk_wOrk_Work/mg_tron/venv/bin/python3.11
 
 # $Id: rst2s5.py 9115 2022-07-28 17:06:24Z milde $
 # Author: Chris Liechti <cliechti@gmx.net>
 # Copyright: This module has been placed in the public domain.
 
 """
 A minimal front end to the Docutils Publisher, producing HTML slides using
```

### Comparing `mgtron-2.17.1/venv/bin/rst2xetex.py` & `mgtron-2.18.0/venv/bin/rst2xetex.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#!/home/djhunter67/Documents/work_worK_woRk_wOrk_Work/mg_tron/venv/bin/python
+#!/home/djhunter67/Documents/work_worK_woRk_wOrk_Work/mg_tron/venv/bin/python3.11
 
 # $Id: rst2xetex.py 9115 2022-07-28 17:06:24Z milde $
 # Author: Guenter Milde
 # Copyright: This module has been placed in the public domain.
 
 """
 A minimal front end to the Docutils Publisher, producing Lua/XeLaTeX code.
```

### Comparing `mgtron-2.17.1/venv/bin/rst2xml.py` & `mgtron-2.18.0/venv/bin/rst2xml.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#!/home/djhunter67/Documents/work_worK_woRk_wOrk_Work/mg_tron/venv/bin/python
+#!/home/djhunter67/Documents/work_worK_woRk_wOrk_Work/mg_tron/venv/bin/python3.11
 
 # $Id: rst2xml.py 9115 2022-07-28 17:06:24Z milde $
 # Author: David Goodger <goodger@python.org>
 # Copyright: This module has been placed in the public domain.
 
 """
 A minimal front end to the Docutils Publisher, producing Docutils XML.
```

### Comparing `mgtron-2.17.1/venv/bin/rstpep2html.py` & `mgtron-2.18.0/venv/bin/rstpep2html.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#!/home/djhunter67/Documents/work_worK_woRk_wOrk_Work/mg_tron/venv/bin/python
+#!/home/djhunter67/Documents/work_worK_woRk_wOrk_Work/mg_tron/venv/bin/python3.11
 
 # $Id: rstpep2html.py 9115 2022-07-28 17:06:24Z milde $
 # Author: David Goodger <goodger@python.org>
 # Copyright: This module has been placed in the public domain.
 
 """
 A minimal front end to the Docutils Publisher, producing HTML from PEP
```

