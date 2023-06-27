# Comparing `tmp/regrez-1.0.0.tar.gz` & `tmp/regrez-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "regrez-1.0.0.tar", last modified: Tue Jun 27 12:06:25 2023, max compression
+gzip compressed data, was "regrez-1.0.1.tar", last modified: Tue Jun 27 18:32:02 2023, max compression
```

## Comparing `regrez-1.0.0.tar` & `regrez-1.0.1.tar`

### file list

```diff
@@ -1,10 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-06-27 12:06:25.795291 regrez-1.0.0/
--rw-rw-rw-   0        0        0      551 2023-06-27 12:06:25.786321 regrez-1.0.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-27 12:06:25.778866 regrez-1.0.0/regrez.egg-info/
--rw-rw-rw-   0        0        0      551 2023-06-27 12:06:25.000000 regrez-1.0.0/regrez.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      157 2023-06-27 12:06:25.000000 regrez-1.0.0/regrez.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-27 12:06:25.000000 regrez-1.0.0/regrez.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2023-06-27 12:06:25.000000 regrez-1.0.0/regrez.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-06-27 12:06:25.000000 regrez-1.0.0/regrez.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-27 12:06:25.796299 regrez-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      870 2023-06-27 12:00:05.000000 regrez-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-27 18:32:02.550679 regrez-1.0.1/
+-rw-rw-rw-   0        0        0     1407 2023-06-27 18:32:02.538034 regrez-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0      953 2023-06-27 18:26:50.000000 regrez-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-27 18:32:02.524472 regrez-1.0.1/regrez.egg-info/
+-rw-rw-rw-   0        0        0     1407 2023-06-27 18:32:02.000000 regrez-1.0.1/regrez.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      167 2023-06-27 18:32:02.000000 regrez-1.0.1/regrez.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-27 18:32:02.000000 regrez-1.0.1/regrez.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2023-06-27 18:32:02.000000 regrez-1.0.1/regrez.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-06-27 18:32:02.000000 regrez-1.0.1/regrez.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-27 18:32:02.553412 regrez-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      789 2023-06-27 18:31:47.000000 regrez-1.0.1/setup.py
```

