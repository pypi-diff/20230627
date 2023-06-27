# Comparing `tmp/dccs_logo-1.0.0.tar.gz` & `tmp/dccs_logo-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dccs_logo-1.0.0.tar", last modified: Mon Jun 26 17:00:11 2023, max compression
+gzip compressed data, was "dccs_logo-1.0.1.tar", last modified: Tue Jun 27 08:00:23 2023, max compression
```

## Comparing `dccs_logo-1.0.0.tar` & `dccs_logo-1.0.1.tar`

### file list

```diff
@@ -1,10 +1,14 @@
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-26 17:00:11.063000 dccs_logo-1.0.0/
--rw-rw----   0 root         (0) everybody  (9997)      268 2023-06-26 17:00:11.063000 dccs_logo-1.0.0/PKG-INFO
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-26 17:00:11.063000 dccs_logo-1.0.0/dccs_logo.egg-info/
--rw-rw----   0 root         (0) everybody  (9997)      268 2023-06-26 17:00:10.000000 dccs_logo-1.0.0/dccs_logo.egg-info/PKG-INFO
--rw-rw----   0 root         (0) everybody  (9997)      172 2023-06-26 17:00:11.000000 dccs_logo-1.0.0/dccs_logo.egg-info/SOURCES.txt
--rw-rw----   0 root         (0) everybody  (9997)        1 2023-06-26 17:00:10.000000 dccs_logo-1.0.0/dccs_logo.egg-info/dependency_links.txt
--rw-rw----   0 root         (0) everybody  (9997)        5 2023-06-26 17:00:10.000000 dccs_logo-1.0.0/dccs_logo.egg-info/requires.txt
--rw-rw----   0 root         (0) everybody  (9997)       10 2023-06-26 17:00:10.000000 dccs_logo-1.0.0/dccs_logo.egg-info/top_level.txt
--rw-rw----   0 root         (0) everybody  (9997)       38 2023-06-26 17:00:11.067000 dccs_logo-1.0.0/setup.cfg
--rw-rw----   0 root         (0) everybody  (9997)      396 2023-06-26 16:57:43.000000 dccs_logo-1.0.0/setup.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-27 08:00:23.057335 dccs_logo-1.0.1/
+-rw-rw----   0 root         (0) everybody  (9997)      268 2023-06-27 08:00:23.057335 dccs_logo-1.0.1/PKG-INFO
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-27 08:00:23.053336 dccs_logo-1.0.1/dccs_logo/
+-rw-rw----   0 root         (0) everybody  (9997)     2098 2023-06-27 07:49:40.000000 dccs_logo-1.0.1/dccs_logo/__init__.py
+-rw-rw----   0 root         (0) everybody  (9997)     2098 2023-06-27 07:41:24.000000 dccs_logo-1.0.1/dccs_logo/dccs_logo.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-27 08:00:23.057335 dccs_logo-1.0.1/dccs_logo.egg-info/
+-rw-rw----   0 root         (0) everybody  (9997)      268 2023-06-27 08:00:22.000000 dccs_logo-1.0.1/dccs_logo.egg-info/PKG-INFO
+-rw-rw----   0 root         (0) everybody  (9997)      249 2023-06-27 08:00:23.000000 dccs_logo-1.0.1/dccs_logo.egg-info/SOURCES.txt
+-rw-rw----   0 root         (0) everybody  (9997)        1 2023-06-27 08:00:22.000000 dccs_logo-1.0.1/dccs_logo.egg-info/dependency_links.txt
+-rw-rw----   0 root         (0) everybody  (9997)        1 2023-06-27 08:00:22.000000 dccs_logo-1.0.1/dccs_logo.egg-info/not-zip-safe
+-rw-rw----   0 root         (0) everybody  (9997)        5 2023-06-27 08:00:23.000000 dccs_logo-1.0.1/dccs_logo.egg-info/requires.txt
+-rw-rw----   0 root         (0) everybody  (9997)       10 2023-06-27 08:00:23.000000 dccs_logo-1.0.1/dccs_logo.egg-info/top_level.txt
+-rw-rw----   0 root         (0) everybody  (9997)       38 2023-06-27 08:00:23.057335 dccs_logo-1.0.1/setup.cfg
+-rw-rw----   0 root         (0) everybody  (9997)      413 2023-06-27 07:53:01.000000 dccs_logo-1.0.1/setup.py
```

