# Comparing `tmp/botsy-0.0.1.tar.gz` & `tmp/botsy-0.0.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
+gzip compressed data, was "botsy-0.0.15.tar", max compression
```

## Comparing `botsy-0.0.1.tar` & `botsy-0.0.15.tar`

### file list

```diff
@@ -1,12 +1,13 @@
--rw-r--r--   0        0        0     1040 2020-02-02 00:00:00.000000 botsy-0.0.1/audio.py
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 botsy-0.0.1/requirements.txt
--rwxr-xr-x   0        0        0      415 2020-02-02 00:00:00.000000 botsy-0.0.1/transcribe_waves.py
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 botsy-0.0.1/.vscode/settings.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 botsy-0.0.1/botsy/__init__.py
--rwxr-xr-x   0        0        0     2491 2020-02-02 00:00:00.000000 botsy-0.0.1/botsy/botsy.py
--rw-r--r--   0        0        0     6336 2020-02-02 00:00:00.000000 botsy-0.0.1/botsy/prompt.mp3
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 botsy-0.0.1/.gitignore
--rw-r--r--   0        0        0     1298 2020-02-02 00:00:00.000000 botsy-0.0.1/LICENSE
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 botsy-0.0.1/README.md
--rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 botsy-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 botsy-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1298 2023-05-31 14:11:15.005456 botsy-0.0.15/LICENSE
+-rw-r--r--   0        0        0       55 2023-05-31 14:15:25.257330 botsy-0.0.15/README.md
+-rw-r--r--   0        0        0       26 2023-05-31 14:11:15.011469 botsy-0.0.15/botsy/__init__.py
+-rwxr-xr-x   0        0        0     3468 2023-06-27 18:02:50.391367 botsy-0.0.15/botsy/botsy.py
+-rwxr-xr-x   0        0        0 16190384 2023-05-31 14:11:15.109613 botsy-0.0.15/botsy/chromedriver
+-rw-r--r--   0        0        0      131 2023-05-31 14:11:15.110137 botsy-0.0.15/botsy/constants.py
+-rw-r--r--   0        0        0     6336 2023-05-31 14:11:15.110400 botsy-0.0.15/botsy/prompt.mp3
+-rw-r--r--   0        0        0   100208 2023-05-31 14:11:15.117508 botsy-0.0.15/botsy/sounds/prompt.m4a
+-rw-r--r--   0        0        0   307116 2023-05-31 14:11:15.121445 botsy-0.0.15/botsy/sounds/prompt.wav
+-rw-r--r--   0        0        0   141334 2023-05-31 14:11:15.122589 botsy-0.0.15/botsy/sounds/startrek_ computer_thinking.m4a
+-rw-r--r--   0        0        0   436174 2023-05-31 14:11:15.126182 botsy-0.0.15/botsy/sounds/thinking.wav
+-rw-r--r--   0        0        0     1263 2023-06-27 19:28:00.808519 botsy-0.0.15/pyproject.toml
+-rw-r--r--   0        0        0     1358 1970-01-01 00:00:00.000000 botsy-0.0.15/PKG-INFO
```

### Comparing `botsy-0.0.1/botsy/prompt.mp3` & `botsy-0.0.15/botsy/prompt.mp3`

 * *Files identical despite different names*

### Comparing `botsy-0.0.1/LICENSE` & `botsy-0.0.15/LICENSE`

 * *Files identical despite different names*

