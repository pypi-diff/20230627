# Comparing `tmp/nihtest-1.1.0.tar.gz` & `tmp/nihtest-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nihtest-1.1.0.tar", last modified: Thu Jun 15 13:17:21 2023, max compression
+gzip compressed data, was "nihtest-1.1.1.tar", last modified: Tue Jun 27 09:54:11 2023, max compression
```

## Comparing `nihtest-1.1.0.tar` & `nihtest-1.1.1.tar`

### file list

```diff
@@ -1,143 +1,144 @@
-drwxr-xr-x   0 dillo      (501) staff       (20)        0 2023-06-15 13:17:21.228451 nihtest-1.1.0/
--rw-r--r--   0 dillo      (501) staff       (20)      993 2023-06-15 12:45:47.000000 nihtest-1.1.0/CMakeLists.txt
--rw-r--r--   0 dillo      (501) staff       (20)     1406 2023-04-15 19:42:21.000000 nihtest-1.1.0/LICENSE
--rw-r--r--   0 dillo      (501) staff       (20)      142 2023-06-15 10:18:02.000000 nihtest-1.1.0/MANIFEST.in
--rw-r--r--   0 dillo      (501) staff       (20)      200 2023-06-15 13:17:15.000000 nihtest-1.1.0/NEWS.md
--rw-r--r--   0 dillo      (501) staff       (20)     1366 2023-06-15 13:17:21.228506 nihtest-1.1.0/PKG-INFO
--rw-r--r--   0 dillo      (501) staff       (20)      808 2023-06-15 10:18:02.000000 nihtest-1.1.0/README.md
--rw-r--r--   0 dillo      (501) staff       (20)      116 2023-06-15 13:14:31.000000 nihtest-1.1.0/TODO.md
-drwxr-xr-x   0 dillo      (501) staff       (20)        0 2023-06-15 13:17:21.213201 nihtest-1.1.0/manpages/
--rw-r--r--   0 dillo      (501) staff       (20)     9383 2023-06-15 10:18:02.000000 nihtest-1.1.0/manpages/nihtest-case.html
--rw-r--r--   0 dillo      (501) staff       (20)     5701 2023-06-15 10:18:02.000000 nihtest-1.1.0/manpages/nihtest-case.man
--rw-r--r--   0 dillo      (501) staff       (20)     6209 2023-06-15 13:12:39.000000 nihtest-1.1.0/manpages/nihtest-case.mdoc
--rw-r--r--   0 dillo      (501) staff       (20)    10371 2023-06-15 10:18:02.000000 nihtest-1.1.0/manpages/nihtest.conf.html
--rw-r--r--   0 dillo      (501) staff       (20)     6000 2023-06-15 10:18:02.000000 nihtest-1.1.0/manpages/nihtest.conf.man
--rw-r--r--   0 dillo      (501) staff       (20)     6163 2023-06-15 13:09:51.000000 nihtest-1.1.0/manpages/nihtest.conf.mdoc
--rw-r--r--   0 dillo      (501) staff       (20)     7738 2023-06-15 10:18:02.000000 nihtest-1.1.0/manpages/nihtest.html
--rw-r--r--   0 dillo      (501) staff       (20)     4599 2023-06-15 10:18:02.000000 nihtest-1.1.0/manpages/nihtest.man
--rw-r--r--   0 dillo      (501) staff       (20)     4141 2023-06-15 10:18:02.000000 nihtest-1.1.0/manpages/nihtest.mdoc
-drwxr-xr-x   0 dillo      (501) staff       (20)        0 2023-06-15 13:17:21.215211 nihtest-1.1.0/nihtest/
--rw-r--r--   0 dillo      (501) staff       (20)     1333 2023-06-15 12:45:46.000000 nihtest-1.1.0/nihtest/Command.py
--rw-r--r--   0 dillo      (501) staff       (20)     4976 2023-05-01 09:06:04.000000 nihtest-1.1.0/nihtest/CompareArrays.py
--rw-r--r--   0 dillo      (501) staff       (20)     5040 2023-06-15 12:45:46.000000 nihtest-1.1.0/nihtest/Configuration.py
--rw-r--r--   0 dillo      (501) staff       (20)      676 2023-06-15 12:45:46.000000 nihtest-1.1.0/nihtest/Environment.py
--rw-r--r--   0 dillo      (501) staff       (20)      667 2023-05-01 09:06:04.000000 nihtest-1.1.0/nihtest/Features.py
--rw-r--r--   0 dillo      (501) staff       (20)     3282 2023-06-15 12:45:46.000000 nihtest-1.1.0/nihtest/File.py
--rw-r--r--   0 dillo      (501) staff       (20)     1056 2023-04-15 19:42:21.000000 nihtest-1.1.0/nihtest/Sandbox.py
--rw-r--r--   0 dillo      (501) staff       (20)     4471 2023-06-15 12:45:46.000000 nihtest-1.1.0/nihtest/Test.py
--rw-r--r--   0 dillo      (501) staff       (20)     9392 2023-06-15 12:45:46.000000 nihtest-1.1.0/nihtest/TestCase.py
--rw-r--r--   0 dillo      (501) staff       (20)      665 2023-05-01 09:06:04.000000 nihtest-1.1.0/nihtest/Utility.py
--rw-r--r--   0 dillo      (501) staff       (20)        0 2023-04-15 19:42:21.000000 nihtest-1.1.0/nihtest/__init__.py
--rw-r--r--   0 dillo      (501) staff       (20)     1453 2023-06-15 12:45:47.000000 nihtest-1.1.0/nihtest/__main__.py
-drwxr-xr-x   0 dillo      (501) staff       (20)        0 2023-06-15 13:17:21.215727 nihtest-1.1.0/nihtest.egg-info/
--rw-r--r--   0 dillo      (501) staff       (20)     1366 2023-06-15 13:17:21.000000 nihtest-1.1.0/nihtest.egg-info/PKG-INFO
--rw-r--r--   0 dillo      (501) staff       (20)     3348 2023-06-15 13:17:21.000000 nihtest-1.1.0/nihtest.egg-info/SOURCES.txt
--rw-r--r--   0 dillo      (501) staff       (20)        1 2023-06-15 13:17:21.000000 nihtest-1.1.0/nihtest.egg-info/dependency_links.txt
--rw-r--r--   0 dillo      (501) staff       (20)       50 2023-06-15 13:17:21.000000 nihtest-1.1.0/nihtest.egg-info/entry_points.txt
--rw-r--r--   0 dillo      (501) staff       (20)        8 2023-06-15 13:17:21.000000 nihtest-1.1.0/nihtest.egg-info/top_level.txt
--rw-r--r--   0 dillo      (501) staff       (20)      977 2023-06-15 12:45:47.000000 nihtest-1.1.0/pyproject.toml
--rw-r--r--   0 dillo      (501) staff       (20)       76 2023-06-15 13:17:21.228707 nihtest-1.1.0/setup.cfg
-drwxr-xr-x   0 dillo      (501) staff       (20)        0 2023-06-15 13:17:21.228337 nihtest-1.1.0/tests/
--rw-r--r--   0 dillo      (501) staff       (20)     2116 2023-06-03 15:23:12.000000 nihtest-1.1.0/tests/CMakeLists.txt
--rw-r--r--   0 dillo      (501) staff       (20)      143 2023-06-15 10:18:02.000000 nihtest-1.1.0/tests/argument-escaped.input
--rw-r--r--   0 dillo      (501) staff       (20)      138 2023-06-15 10:18:02.000000 nihtest-1.1.0/tests/argument-escaped.test
--rw-r--r--   0 dillo      (501) staff       (20)        4 2023-06-15 10:18:02.000000 nihtest-1.1.0/tests/binary-1
--rw-r--r--   0 dillo      (501) staff       (20)        4 2023-06-15 10:18:02.000000 nihtest-1.1.0/tests/binary-2
--rw-r--r--   0 dillo      (501) staff       (20)     1803 2023-04-15 19:42:21.000000 nihtest-1.1.0/tests/can-preload.c
--rw-r--r--   0 dillo      (501) staff       (20)     2586 2023-06-15 10:18:02.000000 nihtest-1.1.0/tests/cat.c
--rw-r--r--   0 dillo      (501) staff       (20)       59 2023-06-03 15:23:12.000000 nihtest-1.1.0/tests/comparator-fail.input
--rw-r--r--   0 dillo      (501) staff       (20)      305 2023-06-03 15:23:12.000000 nihtest-1.1.0/tests/comparator-fail.test
--rw-r--r--   0 dillo      (501) staff       (20)       66 2023-06-03 15:23:12.000000 nihtest-1.1.0/tests/comparator-pass.input
--rw-r--r--   0 dillo      (501) staff       (20)      219 2023-06-03 15:23:12.000000 nihtest-1.1.0/tests/comparator-pass.test
--rw-r--r--   0 dillo      (501) staff       (20)     1585 2023-06-03 15:23:12.000000 nihtest-1.1.0/tests/comparator.c
--rw-r--r--   0 dillo      (501) staff       (20)       65 2023-06-15 10:18:02.000000 nihtest-1.1.0/tests/compare-binary-fail.input
--rw-r--r--   0 dillo      (501) staff       (20)      249 2023-06-15 10:18:02.000000 nihtest-1.1.0/tests/compare-binary-fail.test
--rw-r--r--   0 dillo      (501) staff       (20)       56 2023-06-15 10:18:02.000000 nihtest-1.1.0/tests/compare-binary-pass.input
--rw-r--r--   0 dillo      (501) staff       (20)      140 2023-06-15 10:18:02.000000 nihtest-1.1.0/tests/compare-binary-pass.test
--rw-r--r--   0 dillo      (501) staff       (20)       64 2023-04-15 19:42:21.000000 nihtest-1.1.0/tests/config.h
--rw-r--r--   0 dillo      (501) staff       (20)      125 2023-06-15 10:18:02.000000 nihtest-1.1.0/tests/default-stderr-replace.input
--rw-r--r--   0 dillo      (501) staff       (20)      219 2023-06-15 10:18:02.000000 nihtest-1.1.0/tests/default-stderr-replace.test
--rw-r--r--   0 dillo      (501) staff       (20)      103 2023-04-15 19:42:21.000000 nihtest-1.1.0/tests/description-pass.test
--rw-r--r--   0 dillo      (501) staff       (20)      136 2023-04-15 19:42:21.000000 nihtest-1.1.0/tests/diff-1.input
--rw-r--r--   0 dillo      (501) staff       (20)      218 2023-05-01 09:06:04.000000 nihtest-1.1.0/tests/diff-1.test
--rw-r--r--   0 dillo      (501) staff       (20)      106 2023-04-15 19:42:21.000000 nihtest-1.1.0/tests/diff-2.input
--rw-r--r--   0 dillo      (501) staff       (20)      188 2023-05-01 09:06:04.000000 nihtest-1.1.0/tests/diff-2.test
--rw-r--r--   0 dillo      (501) staff       (20)     1963 2023-04-15 19:42:21.000000 nihtest-1.1.0/tests/echo.c
--rw-r--r--   0 dillo      (501) staff       (20)      103 2023-06-15 12:45:46.000000 nihtest-1.1.0/tests/environment-clear-pass.input
--rw-r--r--   0 dillo      (501) staff       (20)      120 2023-06-15 12:45:46.000000 nihtest-1.1.0/tests/environment-clear-pass.test
--rw-r--r--   0 dillo      (501) staff       (20)       99 2023-06-15 12:45:46.000000 nihtest-1.1.0/tests/environment-not-passed-pass.input
--rw-r--r--   0 dillo      (501) staff       (20)      172 2023-06-15 12:45:46.000000 nihtest-1.1.0/tests/environment-not-passed-pass.test
--rw-r--r--   0 dillo      (501) staff       (20)      155 2023-06-15 12:45:46.000000 nihtest-1.1.0/tests/environment-passthrough-pass.input
--rw-r--r--   0 dillo      (501) staff       (20)      173 2023-06-15 12:45:46.000000 nihtest-1.1.0/tests/environment-passthrough-pass.test
--rw-r--r--   0 dillo      (501) staff       (20)      133 2023-06-15 12:45:46.000000 nihtest-1.1.0/tests/environment-set-config-pass.input
--rw-r--r--   0 dillo      (501) staff       (20)      125 2023-06-15 12:45:46.000000 nihtest-1.1.0/tests/environment-set-config-pass.test
--rw-r--r--   0 dillo      (501) staff       (20)      167 2023-06-15 12:45:46.000000 nihtest-1.1.0/tests/environment-set-pass.input
--rw-r--r--   0 dillo      (501) staff       (20)      118 2023-06-15 12:45:46.000000 nihtest-1.1.0/tests/environment-set-pass.test
--rw-r--r--   0 dillo      (501) staff       (20)      108 2023-06-15 12:45:46.000000 nihtest-1.1.0/tests/environment-unset-pass.input
--rw-r--r--   0 dillo      (501) staff       (20)      120 2023-06-15 12:45:46.000000 nihtest-1.1.0/tests/environment-unset-pass.test
--rw-r--r--   0 dillo      (501) staff       (20)       31 2023-04-15 19:42:21.000000 nihtest-1.1.0/tests/failure.txt
--rw-r--r--   0 dillo      (501) staff       (20)       31 2023-04-15 19:42:21.000000 nihtest-1.1.0/tests/false-fail.input
--rw-r--r--   0 dillo      (501) staff       (20)      201 2023-04-15 19:42:21.000000 nihtest-1.1.0/tests/false-fail.test
--rw-r--r--   0 dillo      (501) staff       (20)       31 2023-04-15 19:42:21.000000 nihtest-1.1.0/tests/false-pass.input
--rw-r--r--   0 dillo      (501) staff       (20)      120 2023-04-15 19:42:21.000000 nihtest-1.1.0/tests/false-pass.test
--rw-r--r--   0 dillo      (501) staff       (20)     1664 2023-04-15 19:42:21.000000 nihtest-1.1.0/tests/false.c
--rw-r--r--   0 dillo      (501) staff       (20)       62 2023-04-15 19:42:21.000000 nihtest-1.1.0/tests/features-fail.input
--rw-r--r--   0 dillo      (501) staff       (20)      236 2023-04-15 19:42:21.000000 nihtest-1.1.0/tests/features-fail.test
--rw-r--r--   0 dillo      (501) staff       (20)       61 2023-04-15 19:42:21.000000 nihtest-1.1.0/tests/features-pass.input
--rw-r--r--   0 dillo      (501) staff       (20)      152 2023-04-15 19:42:21.000000 nihtest-1.1.0/tests/features-pass.test
--rw-r--r--   0 dillo      (501) staff       (20)       61 2023-04-15 19:42:21.000000 nihtest-1.1.0/tests/features-skip.input
--rw-r--r--   0 dillo      (501) staff       (20)      153 2023-04-15 19:42:21.000000 nihtest-1.1.0/tests/features-skip.test
--rw-r--r--   0 dillo      (501) staff       (20)       59 2023-04-15 19:42:21.000000 nihtest-1.1.0/tests/file-del-fail.input
--rw-r--r--   0 dillo      (501) staff       (20)      246 2023-04-15 19:42:21.000000 nihtest-1.1.0/tests/file-del-fail.test
--rw-r--r--   0 dillo      (501) staff       (20)       85 2023-04-15 19:42:21.000000 nihtest-1.1.0/tests/file-del-pass.input
--rw-r--r--   0 dillo      (501) staff       (20)      158 2023-04-15 19:42:21.000000 nihtest-1.1.0/tests/file-del-pass.test
--rw-r--r--   0 dillo      (501) staff       (20)       68 2023-04-15 19:42:21.000000 nihtest-1.1.0/tests/file-fail.input
--rw-r--r--   0 dillo      (501) staff       (20)      254 2023-04-15 19:42:21.000000 nihtest-1.1.0/tests/file-fail.test
--rw-r--r--   0 dillo      (501) staff       (20)      398 2023-04-15 19:42:21.000000 nihtest-1.1.0/tests/file-inline-fail.input
--rw-r--r--   0 dillo      (501) staff       (20)      320 2023-04-15 19:42:21.000000 nihtest-1.1.0/tests/file-inline-fail.test
--rw-r--r--   0 dillo      (501) staff       (20)       59 2023-04-15 19:42:21.000000 nihtest-1.1.0/tests/file-new-fail.input
--rw-r--r--   0 dillo      (501) staff       (20)      217 2023-04-15 19:42:21.000000 nihtest-1.1.0/tests/file-new-fail.test
--rw-r--r--   0 dillo      (501) staff       (20)      111 2023-04-15 19:42:21.000000 nihtest-1.1.0/tests/file-new-pass.input
--rw-r--r--   0 dillo      (501) staff       (20)      129 2023-04-15 19:42:21.000000 nihtest-1.1.0/tests/file-new-pass.test
--rw-r--r--   0 dillo      (501) staff       (20)      120 2023-04-15 19:42:21.000000 nihtest-1.1.0/tests/file-pass.input
--rw-r--r--   0 dillo      (501) staff       (20)      117 2023-04-15 19:42:21.000000 nihtest-1.1.0/tests/file-pass.test
--rw-r--r--   0 dillo      (501) staff       (20)      165 2023-04-15 19:42:21.000000 nihtest-1.1.0/tests/file-subdirectory-pass.input
--rw-r--r--   0 dillo      (501) staff       (20)      156 2023-04-15 19:42:21.000000 nihtest-1.1.0/tests/file-subdirectory-pass.test
--rw-r--r--   0 dillo      (501) staff       (20)     3290 2023-04-15 19:42:21.000000 nihtest-1.1.0/tests/file.c
--rw-r--r--   0 dillo      (501) staff       (20)     2138 2023-04-15 19:42:21.000000 nihtest-1.1.0/tests/getenv.c
--rw-r--r--   0 dillo      (501) staff       (20)     1736 2023-04-15 19:42:21.000000 nihtest-1.1.0/tests/ineffective-remove.c
--rw-r--r--   0 dillo      (501) staff       (20)      330 2023-06-15 12:45:46.000000 nihtest-1.1.0/tests/nihtest-conf.in
--rw-r--r--   0 dillo      (501) staff       (20)      172 2023-04-15 19:42:21.000000 nihtest-1.1.0/tests/nihtest.conf.in
--rw-r--r--   0 dillo      (501) staff       (20)      415 2023-06-15 12:45:46.000000 nihtest-1.1.0/tests/parameter-tests-1.input
--rw-r--r--   0 dillo      (501) staff       (20)     1647 2023-06-15 12:45:46.000000 nihtest-1.1.0/tests/parameter-tests-1.test
--rw-r--r--   0 dillo      (501) staff       (20)       79 2023-04-15 19:42:21.000000 nihtest-1.1.0/tests/parameter-tests-2.input
--rw-r--r--   0 dillo      (501) staff       (20)      340 2023-04-15 19:42:21.000000 nihtest-1.1.0/tests/parameter-tests-2.test
--rw-r--r--   0 dillo      (501) staff       (20)       53 2023-04-15 19:42:21.000000 nihtest-1.1.0/tests/precheck-fail.input
--rw-r--r--   0 dillo      (501) staff       (20)      213 2023-04-15 19:42:21.000000 nihtest-1.1.0/tests/precheck-fail.test
--rw-r--r--   0 dillo      (501) staff       (20)       52 2023-04-15 19:42:21.000000 nihtest-1.1.0/tests/precheck-pass.input
--rw-r--r--   0 dillo      (501) staff       (20)      129 2023-04-15 19:42:21.000000 nihtest-1.1.0/tests/precheck-pass.test
--rw-r--r--   0 dillo      (501) staff       (20)       54 2023-04-15 19:42:21.000000 nihtest-1.1.0/tests/precheck-skip.input
--rw-r--r--   0 dillo      (501) staff       (20)      130 2023-04-15 19:42:21.000000 nihtest-1.1.0/tests/precheck-skip.test
--rw-r--r--   0 dillo      (501) staff       (20)      174 2023-04-15 19:42:21.000000 nihtest-1.1.0/tests/preload-pass.input
--rw-r--r--   0 dillo      (501) staff       (20)      161 2023-04-15 19:42:21.000000 nihtest-1.1.0/tests/preload-pass.test
--rw-r--r--   0 dillo      (501) staff       (20)      163 2023-04-15 19:42:21.000000 nihtest-1.1.0/tests/preload-skip.test
--rw-r--r--   0 dillo      (501) staff       (20)      127 2023-04-15 19:42:21.000000 nihtest-1.1.0/tests/stderr-fail.input
--rw-r--r--   0 dillo      (501) staff       (20)      265 2023-04-15 19:42:21.000000 nihtest-1.1.0/tests/stderr-fail.test
--rw-r--r--   0 dillo      (501) staff       (20)      123 2023-04-15 19:42:21.000000 nihtest-1.1.0/tests/stderr-pass.input
--rw-r--r--   0 dillo      (501) staff       (20)      123 2023-04-15 19:42:21.000000 nihtest-1.1.0/tests/stderr-pass.test
--rw-r--r--   0 dillo      (501) staff       (20)      211 2023-04-15 19:42:21.000000 nihtest-1.1.0/tests/stderr-replace-pass.input
--rw-r--r--   0 dillo      (501) staff       (20)      147 2023-04-15 19:42:21.000000 nihtest-1.1.0/tests/stderr-replace-pass.test
--rw-r--r--   0 dillo      (501) staff       (20)      112 2023-04-15 19:42:21.000000 nihtest-1.1.0/tests/stdin-file-pass.input
--rw-r--r--   0 dillo      (501) staff       (20)      135 2023-04-15 19:42:21.000000 nihtest-1.1.0/tests/stdin-file-pass.test
--rw-r--r--   0 dillo      (501) staff       (20)      146 2023-04-15 19:42:21.000000 nihtest-1.1.0/tests/stdin-pass.input
--rw-r--r--   0 dillo      (501) staff       (20)      120 2023-04-15 19:42:21.000000 nihtest-1.1.0/tests/stdin-pass.test
--rw-r--r--   0 dillo      (501) staff       (20)      124 2023-04-15 19:42:21.000000 nihtest-1.1.0/tests/stdout-fail.input
--rw-r--r--   0 dillo      (501) staff       (20)      253 2023-04-15 19:42:21.000000 nihtest-1.1.0/tests/stdout-fail.test
--rw-r--r--   0 dillo      (501) staff       (20)      120 2023-04-15 19:42:21.000000 nihtest-1.1.0/tests/stdout-pass.input
--rw-r--r--   0 dillo      (501) staff       (20)      123 2023-04-15 19:42:21.000000 nihtest-1.1.0/tests/stdout-pass.test
--rw-r--r--   0 dillo      (501) staff       (20)       27 2023-04-15 19:42:21.000000 nihtest-1.1.0/tests/success.txt
--rw-r--r--   0 dillo      (501) staff       (20)       30 2023-04-15 19:42:21.000000 nihtest-1.1.0/tests/true-fail.input
--rw-r--r--   0 dillo      (501) staff       (20)      197 2023-04-15 19:42:21.000000 nihtest-1.1.0/tests/true-fail.test
--rw-r--r--   0 dillo      (501) staff       (20)       30 2023-04-15 19:42:21.000000 nihtest-1.1.0/tests/true-pass.input
--rw-r--r--   0 dillo      (501) staff       (20)      117 2023-04-15 19:42:21.000000 nihtest-1.1.0/tests/true-pass.test
--rw-r--r--   0 dillo      (501) staff       (20)     1663 2023-04-15 19:42:21.000000 nihtest-1.1.0/tests/true.c
+drwxr-xr-x   0 dillo      (501) staff       (20)        0 2023-06-27 09:54:11.590022 nihtest-1.1.1/
+-rw-r--r--   0 dillo      (501) staff       (20)      993 2023-06-27 09:52:14.000000 nihtest-1.1.1/CMakeLists.txt
+-rw-r--r--   0 dillo      (501) staff       (20)     1406 2023-03-22 09:46:53.000000 nihtest-1.1.1/LICENSE
+-rw-r--r--   0 dillo      (501) staff       (20)      168 2023-06-27 09:50:58.000000 nihtest-1.1.1/MANIFEST.in
+-rw-r--r--   0 dillo      (501) staff       (20)      253 2023-06-27 09:53:03.000000 nihtest-1.1.1/NEWS.md
+-rw-r--r--   0 dillo      (501) staff       (20)     1366 2023-06-27 09:54:11.590087 nihtest-1.1.1/PKG-INFO
+-rw-r--r--   0 dillo      (501) staff       (20)      808 2023-06-09 15:21:43.000000 nihtest-1.1.1/README.md
+-rw-r--r--   0 dillo      (501) staff       (20)      116 2023-06-15 13:24:22.000000 nihtest-1.1.1/TODO.md
+drwxr-xr-x   0 dillo      (501) staff       (20)        0 2023-06-27 09:54:11.571639 nihtest-1.1.1/manpages/
+-rw-r--r--   0 dillo      (501) staff       (20)      576 2023-06-09 14:53:27.000000 nihtest-1.1.1/manpages/Makefile
+-rw-r--r--   0 dillo      (501) staff       (20)    10231 2023-06-15 13:25:55.000000 nihtest-1.1.1/manpages/nihtest-case.html
+-rw-r--r--   0 dillo      (501) staff       (20)     6101 2023-06-15 13:24:22.000000 nihtest-1.1.1/manpages/nihtest-case.man
+-rw-r--r--   0 dillo      (501) staff       (20)     6209 2023-06-15 13:24:22.000000 nihtest-1.1.1/manpages/nihtest-case.mdoc
+-rw-r--r--   0 dillo      (501) staff       (20)    11339 2023-06-15 13:25:55.000000 nihtest-1.1.1/manpages/nihtest.conf.html
+-rw-r--r--   0 dillo      (501) staff       (20)     6480 2023-06-15 13:25:55.000000 nihtest-1.1.1/manpages/nihtest.conf.man
+-rw-r--r--   0 dillo      (501) staff       (20)     6168 2023-06-23 09:31:48.000000 nihtest-1.1.1/manpages/nihtest.conf.mdoc
+-rw-r--r--   0 dillo      (501) staff       (20)     7738 2023-06-15 13:25:55.000000 nihtest-1.1.1/manpages/nihtest.html
+-rw-r--r--   0 dillo      (501) staff       (20)     4599 2023-06-15 13:25:55.000000 nihtest-1.1.1/manpages/nihtest.man
+-rw-r--r--   0 dillo      (501) staff       (20)     4141 2023-06-09 14:24:21.000000 nihtest-1.1.1/manpages/nihtest.mdoc
+drwxr-xr-x   0 dillo      (501) staff       (20)        0 2023-06-27 09:54:11.573690 nihtest-1.1.1/nihtest/
+-rw-r--r--   0 dillo      (501) staff       (20)     1321 2023-06-27 09:50:58.000000 nihtest-1.1.1/nihtest/Command.py
+-rw-r--r--   0 dillo      (501) staff       (20)     4976 2023-04-17 17:35:22.000000 nihtest-1.1.1/nihtest/CompareArrays.py
+-rw-r--r--   0 dillo      (501) staff       (20)     5192 2023-06-27 09:50:58.000000 nihtest-1.1.1/nihtest/Configuration.py
+-rw-r--r--   0 dillo      (501) staff       (20)      676 2023-06-15 13:24:22.000000 nihtest-1.1.1/nihtest/Environment.py
+-rw-r--r--   0 dillo      (501) staff       (20)      667 2023-04-24 10:05:06.000000 nihtest-1.1.1/nihtest/Features.py
+-rw-r--r--   0 dillo      (501) staff       (20)     3254 2023-06-27 09:50:58.000000 nihtest-1.1.1/nihtest/File.py
+-rw-r--r--   0 dillo      (501) staff       (20)     1056 2023-04-15 14:24:35.000000 nihtest-1.1.1/nihtest/Sandbox.py
+-rw-r--r--   0 dillo      (501) staff       (20)     4490 2023-06-27 09:50:58.000000 nihtest-1.1.1/nihtest/Test.py
+-rw-r--r--   0 dillo      (501) staff       (20)     9410 2023-06-27 09:50:58.000000 nihtest-1.1.1/nihtest/TestCase.py
+-rw-r--r--   0 dillo      (501) staff       (20)      677 2023-06-27 09:50:58.000000 nihtest-1.1.1/nihtest/Utility.py
+-rw-r--r--   0 dillo      (501) staff       (20)        0 2023-03-22 10:19:23.000000 nihtest-1.1.1/nihtest/__init__.py
+-rw-r--r--   0 dillo      (501) staff       (20)     1452 2023-06-27 09:52:14.000000 nihtest-1.1.1/nihtest/__main__.py
+drwxr-xr-x   0 dillo      (501) staff       (20)        0 2023-06-27 09:54:11.574224 nihtest-1.1.1/nihtest.egg-info/
+-rw-r--r--   0 dillo      (501) staff       (20)     1366 2023-06-27 09:54:11.000000 nihtest-1.1.1/nihtest.egg-info/PKG-INFO
+-rw-r--r--   0 dillo      (501) staff       (20)     3366 2023-06-27 09:54:11.000000 nihtest-1.1.1/nihtest.egg-info/SOURCES.txt
+-rw-r--r--   0 dillo      (501) staff       (20)        1 2023-06-27 09:54:11.000000 nihtest-1.1.1/nihtest.egg-info/dependency_links.txt
+-rw-r--r--   0 dillo      (501) staff       (20)       50 2023-06-27 09:54:11.000000 nihtest-1.1.1/nihtest.egg-info/entry_points.txt
+-rw-r--r--   0 dillo      (501) staff       (20)        8 2023-06-27 09:54:11.000000 nihtest-1.1.1/nihtest.egg-info/top_level.txt
+-rw-r--r--   0 dillo      (501) staff       (20)      977 2023-06-27 09:52:14.000000 nihtest-1.1.1/pyproject.toml
+-rw-r--r--   0 dillo      (501) staff       (20)       76 2023-06-27 09:54:11.590290 nihtest-1.1.1/setup.cfg
+drwxr-xr-x   0 dillo      (501) staff       (20)        0 2023-06-27 09:54:11.589854 nihtest-1.1.1/tests/
+-rw-r--r--   0 dillo      (501) staff       (20)     2116 2023-05-19 12:07:31.000000 nihtest-1.1.1/tests/CMakeLists.txt
+-rw-r--r--   0 dillo      (501) staff       (20)      143 2023-06-09 14:24:21.000000 nihtest-1.1.1/tests/argument-escaped.input
+-rw-r--r--   0 dillo      (501) staff       (20)      138 2023-06-09 14:24:21.000000 nihtest-1.1.1/tests/argument-escaped.test
+-rw-r--r--   0 dillo      (501) staff       (20)        4 2023-06-09 14:24:21.000000 nihtest-1.1.1/tests/binary-1
+-rw-r--r--   0 dillo      (501) staff       (20)        4 2023-06-09 14:24:21.000000 nihtest-1.1.1/tests/binary-2
+-rw-r--r--   0 dillo      (501) staff       (20)     1803 2023-04-12 13:00:35.000000 nihtest-1.1.1/tests/can-preload.c
+-rw-r--r--   0 dillo      (501) staff       (20)     2586 2023-06-09 14:24:21.000000 nihtest-1.1.1/tests/cat.c
+-rw-r--r--   0 dillo      (501) staff       (20)       59 2023-05-19 12:10:40.000000 nihtest-1.1.1/tests/comparator-fail.input
+-rw-r--r--   0 dillo      (501) staff       (20)      305 2023-05-19 12:16:34.000000 nihtest-1.1.1/tests/comparator-fail.test
+-rw-r--r--   0 dillo      (501) staff       (20)       66 2023-05-19 12:12:53.000000 nihtest-1.1.1/tests/comparator-pass.input
+-rw-r--r--   0 dillo      (501) staff       (20)      219 2023-05-19 12:10:40.000000 nihtest-1.1.1/tests/comparator-pass.test
+-rw-r--r--   0 dillo      (501) staff       (20)     1585 2023-05-19 12:16:03.000000 nihtest-1.1.1/tests/comparator.c
+-rw-r--r--   0 dillo      (501) staff       (20)       65 2023-06-09 14:24:21.000000 nihtest-1.1.1/tests/compare-binary-fail.input
+-rw-r--r--   0 dillo      (501) staff       (20)      249 2023-06-09 14:24:21.000000 nihtest-1.1.1/tests/compare-binary-fail.test
+-rw-r--r--   0 dillo      (501) staff       (20)       56 2023-06-09 14:24:21.000000 nihtest-1.1.1/tests/compare-binary-pass.input
+-rw-r--r--   0 dillo      (501) staff       (20)      140 2023-06-09 14:24:21.000000 nihtest-1.1.1/tests/compare-binary-pass.test
+-rw-r--r--   0 dillo      (501) staff       (20)       64 2023-03-31 09:51:38.000000 nihtest-1.1.1/tests/config.h
+-rw-r--r--   0 dillo      (501) staff       (20)      125 2023-06-09 14:24:21.000000 nihtest-1.1.1/tests/default-stderr-replace.input
+-rw-r--r--   0 dillo      (501) staff       (20)      219 2023-06-09 14:24:21.000000 nihtest-1.1.1/tests/default-stderr-replace.test
+-rw-r--r--   0 dillo      (501) staff       (20)      103 2023-04-12 10:10:55.000000 nihtest-1.1.1/tests/description-pass.test
+-rw-r--r--   0 dillo      (501) staff       (20)      136 2023-03-31 09:51:38.000000 nihtest-1.1.1/tests/diff-1.input
+-rw-r--r--   0 dillo      (501) staff       (20)      218 2023-04-17 17:35:49.000000 nihtest-1.1.1/tests/diff-1.test
+-rw-r--r--   0 dillo      (501) staff       (20)      106 2023-03-31 09:51:38.000000 nihtest-1.1.1/tests/diff-2.input
+-rw-r--r--   0 dillo      (501) staff       (20)      188 2023-04-17 17:36:44.000000 nihtest-1.1.1/tests/diff-2.test
+-rw-r--r--   0 dillo      (501) staff       (20)     1963 2023-03-31 09:51:38.000000 nihtest-1.1.1/tests/echo.c
+-rw-r--r--   0 dillo      (501) staff       (20)      103 2023-06-15 13:24:22.000000 nihtest-1.1.1/tests/environment-clear-pass.input
+-rw-r--r--   0 dillo      (501) staff       (20)      120 2023-06-15 13:24:22.000000 nihtest-1.1.1/tests/environment-clear-pass.test
+-rw-r--r--   0 dillo      (501) staff       (20)       99 2023-06-15 13:24:22.000000 nihtest-1.1.1/tests/environment-not-passed-pass.input
+-rw-r--r--   0 dillo      (501) staff       (20)      172 2023-06-15 13:24:22.000000 nihtest-1.1.1/tests/environment-not-passed-pass.test
+-rw-r--r--   0 dillo      (501) staff       (20)      155 2023-06-15 13:24:22.000000 nihtest-1.1.1/tests/environment-passthrough-pass.input
+-rw-r--r--   0 dillo      (501) staff       (20)      173 2023-06-15 13:24:22.000000 nihtest-1.1.1/tests/environment-passthrough-pass.test
+-rw-r--r--   0 dillo      (501) staff       (20)      133 2023-06-15 13:24:22.000000 nihtest-1.1.1/tests/environment-set-config-pass.input
+-rw-r--r--   0 dillo      (501) staff       (20)      125 2023-06-15 13:24:22.000000 nihtest-1.1.1/tests/environment-set-config-pass.test
+-rw-r--r--   0 dillo      (501) staff       (20)      167 2023-06-15 13:24:22.000000 nihtest-1.1.1/tests/environment-set-pass.input
+-rw-r--r--   0 dillo      (501) staff       (20)      118 2023-06-15 13:24:22.000000 nihtest-1.1.1/tests/environment-set-pass.test
+-rw-r--r--   0 dillo      (501) staff       (20)      108 2023-06-15 13:24:22.000000 nihtest-1.1.1/tests/environment-unset-pass.input
+-rw-r--r--   0 dillo      (501) staff       (20)      120 2023-06-15 13:24:22.000000 nihtest-1.1.1/tests/environment-unset-pass.test
+-rw-r--r--   0 dillo      (501) staff       (20)       31 2023-03-31 09:51:38.000000 nihtest-1.1.1/tests/failure.txt
+-rw-r--r--   0 dillo      (501) staff       (20)       31 2023-03-31 09:51:38.000000 nihtest-1.1.1/tests/false-fail.input
+-rw-r--r--   0 dillo      (501) staff       (20)      201 2023-04-12 10:10:55.000000 nihtest-1.1.1/tests/false-fail.test
+-rw-r--r--   0 dillo      (501) staff       (20)       31 2023-03-31 09:51:38.000000 nihtest-1.1.1/tests/false-pass.input
+-rw-r--r--   0 dillo      (501) staff       (20)      120 2023-04-12 10:10:55.000000 nihtest-1.1.1/tests/false-pass.test
+-rw-r--r--   0 dillo      (501) staff       (20)     1664 2023-03-31 09:51:38.000000 nihtest-1.1.1/tests/false.c
+-rw-r--r--   0 dillo      (501) staff       (20)       62 2023-03-31 09:51:38.000000 nihtest-1.1.1/tests/features-fail.input
+-rw-r--r--   0 dillo      (501) staff       (20)      236 2023-04-12 10:10:55.000000 nihtest-1.1.1/tests/features-fail.test
+-rw-r--r--   0 dillo      (501) staff       (20)       61 2023-03-31 09:51:38.000000 nihtest-1.1.1/tests/features-pass.input
+-rw-r--r--   0 dillo      (501) staff       (20)      152 2023-04-12 10:10:55.000000 nihtest-1.1.1/tests/features-pass.test
+-rw-r--r--   0 dillo      (501) staff       (20)       61 2023-03-31 09:51:38.000000 nihtest-1.1.1/tests/features-skip.input
+-rw-r--r--   0 dillo      (501) staff       (20)      153 2023-04-12 10:10:55.000000 nihtest-1.1.1/tests/features-skip.test
+-rw-r--r--   0 dillo      (501) staff       (20)       59 2023-03-31 09:51:38.000000 nihtest-1.1.1/tests/file-del-fail.input
+-rw-r--r--   0 dillo      (501) staff       (20)      246 2023-04-12 10:14:06.000000 nihtest-1.1.1/tests/file-del-fail.test
+-rw-r--r--   0 dillo      (501) staff       (20)       85 2023-03-31 09:51:38.000000 nihtest-1.1.1/tests/file-del-pass.input
+-rw-r--r--   0 dillo      (501) staff       (20)      158 2023-04-12 10:10:55.000000 nihtest-1.1.1/tests/file-del-pass.test
+-rw-r--r--   0 dillo      (501) staff       (20)       68 2023-03-31 09:51:38.000000 nihtest-1.1.1/tests/file-fail.input
+-rw-r--r--   0 dillo      (501) staff       (20)      254 2023-04-15 15:28:11.000000 nihtest-1.1.1/tests/file-fail.test
+-rw-r--r--   0 dillo      (501) staff       (20)      398 2023-04-15 14:27:28.000000 nihtest-1.1.1/tests/file-inline-fail.input
+-rw-r--r--   0 dillo      (501) staff       (20)      320 2023-04-15 15:28:58.000000 nihtest-1.1.1/tests/file-inline-fail.test
+-rw-r--r--   0 dillo      (501) staff       (20)       59 2023-03-31 09:51:38.000000 nihtest-1.1.1/tests/file-new-fail.input
+-rw-r--r--   0 dillo      (501) staff       (20)      217 2023-04-12 10:14:06.000000 nihtest-1.1.1/tests/file-new-fail.test
+-rw-r--r--   0 dillo      (501) staff       (20)      111 2023-04-12 10:55:14.000000 nihtest-1.1.1/tests/file-new-pass.input
+-rw-r--r--   0 dillo      (501) staff       (20)      129 2023-04-12 10:10:55.000000 nihtest-1.1.1/tests/file-new-pass.test
+-rw-r--r--   0 dillo      (501) staff       (20)      120 2023-04-12 10:53:21.000000 nihtest-1.1.1/tests/file-pass.input
+-rw-r--r--   0 dillo      (501) staff       (20)      117 2023-04-12 10:10:55.000000 nihtest-1.1.1/tests/file-pass.test
+-rw-r--r--   0 dillo      (501) staff       (20)      165 2023-04-12 11:02:07.000000 nihtest-1.1.1/tests/file-subdirectory-pass.input
+-rw-r--r--   0 dillo      (501) staff       (20)      156 2023-04-12 10:10:55.000000 nihtest-1.1.1/tests/file-subdirectory-pass.test
+-rw-r--r--   0 dillo      (501) staff       (20)     3290 2023-04-12 11:02:07.000000 nihtest-1.1.1/tests/file.c
+-rw-r--r--   0 dillo      (501) staff       (20)     2138 2023-03-31 09:51:38.000000 nihtest-1.1.1/tests/getenv.c
+-rw-r--r--   0 dillo      (501) staff       (20)     1736 2023-03-31 09:51:38.000000 nihtest-1.1.1/tests/ineffective-remove.c
+-rw-r--r--   0 dillo      (501) staff       (20)      394 2023-06-27 09:50:58.000000 nihtest-1.1.1/tests/nihtest-conf.in
+-rw-r--r--   0 dillo      (501) staff       (20)      236 2023-06-27 09:50:58.000000 nihtest-1.1.1/tests/nihtest.conf.in
+-rw-r--r--   0 dillo      (501) staff       (20)      415 2023-06-15 13:24:22.000000 nihtest-1.1.1/tests/parameter-tests-1.input
+-rw-r--r--   0 dillo      (501) staff       (20)     1694 2023-06-27 09:50:58.000000 nihtest-1.1.1/tests/parameter-tests-1.test
+-rw-r--r--   0 dillo      (501) staff       (20)       79 2023-03-31 09:51:38.000000 nihtest-1.1.1/tests/parameter-tests-2.input
+-rw-r--r--   0 dillo      (501) staff       (20)      387 2023-06-27 09:50:58.000000 nihtest-1.1.1/tests/parameter-tests-2.test
+-rw-r--r--   0 dillo      (501) staff       (20)       53 2023-03-31 09:51:38.000000 nihtest-1.1.1/tests/precheck-fail.input
+-rw-r--r--   0 dillo      (501) staff       (20)      213 2023-04-12 12:29:19.000000 nihtest-1.1.1/tests/precheck-fail.test
+-rw-r--r--   0 dillo      (501) staff       (20)       52 2023-03-31 09:51:38.000000 nihtest-1.1.1/tests/precheck-pass.input
+-rw-r--r--   0 dillo      (501) staff       (20)      129 2023-04-12 10:10:55.000000 nihtest-1.1.1/tests/precheck-pass.test
+-rw-r--r--   0 dillo      (501) staff       (20)       54 2023-03-31 09:51:38.000000 nihtest-1.1.1/tests/precheck-skip.input
+-rw-r--r--   0 dillo      (501) staff       (20)      130 2023-04-12 12:29:19.000000 nihtest-1.1.1/tests/precheck-skip.test
+-rw-r--r--   0 dillo      (501) staff       (20)      174 2023-03-31 09:51:38.000000 nihtest-1.1.1/tests/preload-pass.input
+-rw-r--r--   0 dillo      (501) staff       (20)      161 2023-04-12 13:00:35.000000 nihtest-1.1.1/tests/preload-pass.test
+-rw-r--r--   0 dillo      (501) staff       (20)      163 2023-04-12 13:00:35.000000 nihtest-1.1.1/tests/preload-skip.test
+-rw-r--r--   0 dillo      (501) staff       (20)      127 2023-03-31 09:51:38.000000 nihtest-1.1.1/tests/stderr-fail.input
+-rw-r--r--   0 dillo      (501) staff       (20)      265 2023-04-12 10:10:55.000000 nihtest-1.1.1/tests/stderr-fail.test
+-rw-r--r--   0 dillo      (501) staff       (20)      123 2023-03-31 09:51:38.000000 nihtest-1.1.1/tests/stderr-pass.input
+-rw-r--r--   0 dillo      (501) staff       (20)      123 2023-04-12 10:10:55.000000 nihtest-1.1.1/tests/stderr-pass.test
+-rw-r--r--   0 dillo      (501) staff       (20)      211 2023-04-12 11:16:36.000000 nihtest-1.1.1/tests/stderr-replace-pass.input
+-rw-r--r--   0 dillo      (501) staff       (20)      147 2023-04-12 10:10:55.000000 nihtest-1.1.1/tests/stderr-replace-pass.test
+-rw-r--r--   0 dillo      (501) staff       (20)      112 2023-03-31 09:51:38.000000 nihtest-1.1.1/tests/stdin-file-pass.input
+-rw-r--r--   0 dillo      (501) staff       (20)      135 2023-04-12 10:10:55.000000 nihtest-1.1.1/tests/stdin-file-pass.test
+-rw-r--r--   0 dillo      (501) staff       (20)      146 2023-03-31 09:51:38.000000 nihtest-1.1.1/tests/stdin-pass.input
+-rw-r--r--   0 dillo      (501) staff       (20)      120 2023-04-12 10:10:55.000000 nihtest-1.1.1/tests/stdin-pass.test
+-rw-r--r--   0 dillo      (501) staff       (20)      124 2023-03-31 09:51:38.000000 nihtest-1.1.1/tests/stdout-fail.input
+-rw-r--r--   0 dillo      (501) staff       (20)      253 2023-04-12 10:10:55.000000 nihtest-1.1.1/tests/stdout-fail.test
+-rw-r--r--   0 dillo      (501) staff       (20)      120 2023-03-31 09:51:38.000000 nihtest-1.1.1/tests/stdout-pass.input
+-rw-r--r--   0 dillo      (501) staff       (20)      123 2023-04-12 10:10:55.000000 nihtest-1.1.1/tests/stdout-pass.test
+-rw-r--r--   0 dillo      (501) staff       (20)       27 2023-03-31 09:51:38.000000 nihtest-1.1.1/tests/success.txt
+-rw-r--r--   0 dillo      (501) staff       (20)       30 2023-03-31 09:51:38.000000 nihtest-1.1.1/tests/true-fail.input
+-rw-r--r--   0 dillo      (501) staff       (20)      197 2023-04-12 10:10:55.000000 nihtest-1.1.1/tests/true-fail.test
+-rw-r--r--   0 dillo      (501) staff       (20)       30 2023-03-31 09:51:38.000000 nihtest-1.1.1/tests/true-pass.input
+-rw-r--r--   0 dillo      (501) staff       (20)      117 2023-04-12 10:10:55.000000 nihtest-1.1.1/tests/true-pass.test
+-rw-r--r--   0 dillo      (501) staff       (20)     1663 2023-06-27 09:50:54.000000 nihtest-1.1.1/tests/true.c
```

### Comparing `nihtest-1.1.0/CMakeLists.txt` & `nihtest-1.1.1/CMakeLists.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 cmake_minimum_required(VERSION 3.12)
 
 # Also update version in nihtest/__main__.py and pyproject.toml
 project(nihtest
-        VERSION 1.1.0
+        VERSION 1.1.1
         DESCRIPTION "NiH testing framework"
         HOMEPAGE_URL "https://github.com/nih-at/nihtest"
         LANGUAGES C)
 
 enable_testing()
 
 find_package(Python3 REQUIRED COMPONENTS Interpreter)
```

### Comparing `nihtest-1.1.0/LICENSE` & `nihtest-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nihtest-1.1.0/PKG-INFO` & `nihtest-1.1.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nihtest
-Version: 1.1.0
+Version: 1.1.1
 Summary: A testing tool for command line utilities.
 Author-email: Dieter Baron <dillo@nih.at>, Thomas Klausner <wiz@gatalith.at>
 License: BSD-3-Clause
 Project-URL: Homepage, https://github.com/nih-at/nihtest
 Project-URL: Bug Tracker, https://github.com/nih-at/nihtest/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `nihtest-1.1.0/README.md` & `nihtest-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `nihtest-1.1.0/manpages/nihtest-case.html` & `nihtest-1.1.1/manpages/nihtest-case.html`

 * *Files 8% similar despite different names*

```diff
@@ -64,14 +64,29 @@
   <dt><a class="permalink" href="#arguments"><code class="Ic" id="arguments">arguments</code></a>
     [<var class="Ar">argument ...</var>]</dt>
   <dd>Run the program with command line arguments <var class="Ar">args</var>.
       Shell style quoting is supported.</dd>
   <dt><a class="permalink" href="#description"><code class="Ic" id="description">description</code></a>
     <var class="Ar">text</var></dt>
   <dd>Describes the purpose of the test.</dd>
+  <dt><a class="permalink" href="#environment-clear"><code class="Ic" id="environment-clear">environment-clear</code></a></dt>
+  <dd>Only variables explicitly set or passed through are included in the
+      environment passed to the tested program.</dd>
+  <dt><a class="permalink" href="#environment-passthrough"><code class="Ic" id="environment-passthrough">environment-passthrough</code></a>
+    <var class="Ar">variable ...</var></dt>
+  <dd>Passes the named environment variables from the environment
+      <a class="Xr" href="nihtest.html">nihtest(1)</a> is run in to the tested
+      program.</dd>
+  <dt><a class="permalink" href="#environment-set"><code class="Ic" id="environment-set">environment-set</code></a>
+    <var class="Ar">variable value</var></dt>
+  <dd>Set the environment variable <var class="Ar">variable</var> to
+      <var class="Ar">value</var>.</dd>
+  <dt><a class="permalink" href="#environment-unset"><code class="Ic" id="environment-unset">environment-unset</code></a>
+    <var class="Ar">variable ...</var></dt>
+  <dd>Removes the named environment variables.</dd>
   <dt><a class="permalink" href="#features"><code class="Ic" id="features">features</code></a>
     <var class="Ar">feature ...</var></dt>
   <dd>Only run test if all
       <var class="Ar">feature</var><span class="No">s</span> are present,
       otherwise skip it. The features are extracted from a top-level
       <span class="Pa">config.h</span> file. If the string
       <code class="Dv">FOO</code> is defined in the file, the feature
@@ -116,18 +131,14 @@
       <code class="Ic">arguments</code> above for its command line arguments. If
       this directive is omitted, <code class="Ic">default-program</code> from
       <span class="Pa">nihtest.conf</span> is run.</dd>
   <dt><a class="permalink" href="#return"><code class="Ic" id="return">return</code></a>
     <var class="Ar">exit-code</var></dt>
   <dd><var class="Ar">exit-code</var> is the expected exit code (usually 0 on
       success).</dd>
-  <dt><a class="permalink" href="#setenv"><code class="Ic" id="setenv">setenv</code></a>
-    <var class="Ar">variable value</var></dt>
-  <dd>Set the environment variable <var class="Ar">variable</var> to
-      <var class="Ar">value</var>.</dd>
   <dt><a class="permalink" href="#stderr"><code class="Ic" id="stderr">stderr</code></a>
     [<var class="Ar">file</var>]</dt>
   <dd>Specify the expect standard error output (stderr). If
       <var class="Ar">file</var> is given, the output is compared with that
       file, otherwise the expected text is taken from the following lines of the
       test case, up to a line consisting of
     &#x201C;end-of-inline-data&#x201D;.</dd>
```

#### html2text {}

```diff
@@ -11,14 +11,24 @@
 The following commands are recognized. The return and args commands must appear
 exactly once, the others are optional.
   arguments [argument ...]
       Run the program with command line arguments args. Shell style quoting is
       supported.
   description text
       Describes the purpose of the test.
+  environment-clear
+      Only variables explicitly set or passed through are included in the
+      environment passed to the tested program.
+  environment-passthrough variable ...
+      Passes the named environment variables from the environment nihtest(1) is
+      run in to the tested program.
+  environment-set variable value
+      Set the environment variable variable to value.
+  environment-unset variable ...
+      Removes the named environment variables.
   features feature ...
       Only run test if all features are present, otherwise skip it. The
       features are extracted from a top-level config.h file. If the string FOO
       is defined in the file, the feature FOO is assumed to be available,
       otherwise not. See also the description of top-build-directory in
       nihtest-config(5).
   file name in [out]
@@ -43,16 +53,14 @@
       be skipped.
   program name
       Run name. See the description of arguments above for its command line
       arguments. If this directive is omitted, default-program from
       nihtest.conf is run.
   return exit-code
       exit-code is the expected exit code (usually 0 on success).
-  setenv variable value
-      Set the environment variable variable to value.
   stderr [file]
       Specify the expect standard error output (stderr). If file is given, the
       output is compared with that file, otherwise the expected text is taken
       from the following lines of the test case, up to a line consisting of
       &#x201C;end-of-inline-data&#x201D;.
   stderr-replace pattern replacement
       Run regular expression replacement over the standard error output and the
```

### Comparing `nihtest-1.1.0/manpages/nihtest-case.man` & `nihtest-1.1.1/manpages/nihtest-case.man`

 * *Files 12% similar despite different names*

```diff
@@ -59,14 +59,31 @@
 Run the program with command line arguments
 \fIargs\fR.
 Shell style quoting is supported.
 .TP 22n
 \fBdescription\fR \fItext\fR
 Describes the purpose of the test.
 .TP 22n
+\fBenvironment-clear\fR
+Only variables explicitly set or passed through are included in the environment passed to the tested program.
+.TP 22n
+\fBenvironment-passthrough\fR \fIvariable ...\fR
+Passes the named environment variables from the environment
+nihtest(1)
+is run in to the tested program.
+.TP 22n
+\fBenvironment-set\fR \fIvariable value\fR
+Set the environment variable
+\fIvariable\fR
+to
+\fIvalue\fR.
+.TP 22n
+\fBenvironment-unset\fR \fIvariable ...\fR
+Removes the named environment variables.
+.TP 22n
 \fBfeatures\fR \fIfeature ...\fR
 Only run test if all
 \fIfeature\fRs
 are present, otherwise skip it.
 The features are extracted from a top-level
 \fIconfig.h\fR
 file.
@@ -139,21 +156,14 @@
 \fInihtest.conf\fR
 is run.
 .TP 22n
 \fBreturn\fR \fIexit-code\fR
 \fIexit-code\fR
 is the expected exit code (usually 0 on success).
 .TP 22n
-\fBsetenv\fR \fIvariable value\fR
-.br
-Set the environment variable
-\fIvariable\fR
-to
-\fIvalue\fR.
-.TP 22n
 \fBstderr\fR [\fIfile\fR]
 Specify the expect standard error output (stderr).
 If
 \fIfile\fR
 is given, the output is compared with that file,
 otherwise the expected text is taken from the following lines of the test case, up to a line consisting of
 \(lqend-of-inline-data\(rq.
```

### Comparing `nihtest-1.1.0/manpages/nihtest-case.mdoc` & `nihtest-1.1.1/manpages/nihtest-case.mdoc`

 * *Files identical despite different names*

### Comparing `nihtest-1.1.0/manpages/nihtest.conf.html` & `nihtest-1.1.1/manpages/nihtest.conf.html`

 * *Files 12% similar despite different names*

```diff
@@ -85,14 +85,28 @@
     =</code></a> <var class="Ar">pattern replacement ...</var></dt>
   <dd>Each line consists of two values, <var class="Ar">pattern</var> is a
       regular expression and <var class="Ar">replacement</var> the corresponding
       replacement string. These are used for test cases without
       <code class="Ic">stderr-replace</code> directives. See
       <a class="Xr" href="nihtest-case.html">nihtest-case(5)</a> for details on
       <code class="Ic">stderr-replace</code>.</dd>
+  <dt><a class="permalink" href="#environment-clear_=_true"><code class="Ic" id="environment-clear_=_true">environment-clear
+    = true</code></a></dt>
+  <dd>If <code class="Ic">environment-clear</code> is set to
+      <code class="Dv">true</code>, only variables explicitly set or passed
+      through are included in the environment passed to the tested program.</dd>
+  <dt><a class="permalink" href="#environment-passthrough_="><code class="Ic" id="environment-passthrough_=">environment-passthrough
+    =</code></a> <var class="Ar">variable ...</var></dt>
+  <dd>The named environment variables are passed through from the environment
+      <a class="Xr" href="nihtest.html">nihtest(1)</a> is run in to the
+      environment passed to the tested program.</dd>
+  <dt><a class="permalink" href="#environment-unset_="><code class="Ic" id="environment-unset_=">environment-unset
+    =</code></a> <var class="Ar">variable ...</var></dt>
+  <dd>The named environment variables are removed from the environment passed to
+      the tested program.</dd>
   <dt><a class="permalink" href="#features-files_="><code class="Ic" id="features-files_=">features-files
     =</code></a> <var class="Ar">file ...</var></dt>
   <dd>Specifies the files to search for feature defines. This is used in the
       <code class="Ic">features</code> directive in test cases.</dd>
   <dt><a class="permalink" href="#keep-sandbox_="><code class="Ic" id="keep-sandbox_=">keep-sandbox
     =</code></a> <var class="Ar">when</var></dt>
   <dd>Describe when to keep the sandbox (i.e., not delete it) after running the
@@ -145,19 +159,17 @@
     =</code></a> <var class="Ar">directory ...</var></dt>
   <dd><a class="Xr" href="nihtest.html">nihtest(1)</a> searches the current
       directory and <var class="Ar">directory</var> for test cases, input and
       output files.</dd>
 </dl>
 </section>
 <section class="Sh">
-<h1 class="Sh" id="SETENV"><a class="permalink" href="#SETENV">SETENV</a></h1>
-The <code class="Ic">setenv</code> section contains variable and values that
-  will be added as environment variables when the test program is run. If the
-  test case contains a <code class="Ic">setenv</code> directive, this section
-  will be ignored.
+<h1 class="Sh" id="ENVIRONMENT"><a class="permalink" href="#ENVIRONMENT">ENVIRONMENT</a></h1>
+The <code class="Ic">environment</code> section contains variable and values
+  that will be added as environment variables when the test program is run.
 </section>
 <section class="Sh">
 <h1 class="Sh" id="COMPARATORS"><a class="permalink" href="#COMPARATORS">COMPARATORS</a></h1>
 The <code class="Ic">comparators</code> section specifies programs to use to
   compare files of certain types. The variable names have the format
   <var class="Ar">got-extension</var>. <var class="Ar">expected-extension</var>,
   the value specifies the command line to use to compare these files. The
@@ -181,15 +193,15 @@
 <h1 class="Sh" id="EXAMPLES"><a class="permalink" href="#EXAMPLES">EXAMPLES</a></h1>
 <div class="Bd">
 <pre>
 [settings]
 default-program = program_to_test
 program-directories = bin
     tests
-[setenv]
+[environment]
 LC_ALL=en_US.UTF-8
 [comparators]
 zip.zip = zipcmp -v
 </pre>
 </div>
 </section>
 <section class="Sh">
```

#### html2text {}

```diff
@@ -22,14 +22,24 @@
   default-program_= program
       Test program if no program directive is found in the test.
   default-stderr-replace_= pattern replacement ...
       Each line consists of two values, pattern is a regular expression and
       replacement the corresponding replacement string. These are used for test
       cases without stderr-replace directives. See nihtest-case(5) for details
       on stderr-replace.
+  environment-clear_=_true
+      If environment-clear is set to true, only variables explicitly set or
+      passed through are included in the environment passed to the tested
+      program.
+  environment-passthrough_= variable ...
+      The named environment variables are passed through from the environment
+      nihtest(1) is run in to the environment passed to the tested program.
+  environment-unset_= variable ...
+      The named environment variables are removed from the environment passed
+      to the tested program.
   features-files_= file ...
       Specifies the files to search for feature defines. This is used in the
       features directive in test cases.
   keep-sandbox_= when
       Describe when to keep the sandbox (i.e., not delete it) after running the
       test. The following values are supported:
         never
@@ -58,18 +68,17 @@
       Create sandboxes in directory. By default, the sandboxes will be created
       in the current directory. A random directory of the pattern sandbox_*
       will be used.
   test-input-directories_= directory ...
       nihtest(1) searches the current directory and directory for test cases,
       input and output files.
 
-****** SETENV ******
-The setenv section contains variable and values that will be added as
-environment variables when the test program is run. If the test case contains a
-setenv directive, this section will be ignored.
+****** ENVIRONMENT ******
+The environment section contains variable and values that will be added as
+environment variables when the test program is run.
 ****** COMPARATORS ******
 The comparators section specifies programs to use to compare files of certain
 types. The variable names have the format got-extension. expected-extension,
 the value specifies the command line to use to compare these files. The command
 will be run with the two files as arguments, the file in the sandbox first and
 the expected last.
 The command is expected to exit with code 0 if the two files are considered
@@ -83,15 +92,15 @@
 zipcmp -v got.zip expected.zip
 will be run to compare the files.
 ****** EXAMPLES ******
 [settings]
 default-program = program_to_test
 program-directories = bin
     tests
-[setenv]
+[environment]
 LC_ALL=en_US.UTF-8
 [comparators]
 zip.zip = zipcmp -v
 
 ****** SEE_ALSO ******
 nihtest(1)
 June 15, 2023 NiH
```

### Comparing `nihtest-1.1.0/manpages/nihtest.conf.man` & `nihtest-1.1.1/manpages/nihtest.conf.man`

 * *Files 10% similar despite different names*

```diff
@@ -84,14 +84,29 @@
 \fBstderr-replace\fR
 directives.
 See
 nihtest-case(5)
 for details on
 \fBstderr-replace\fR.
 .TP 22n
+\fBenvironment-clear = true\fR
+If
+\fBenvironment-clear\fR
+is set to
+\fRtrue\fR,
+only variables explicitly set or passed through are included in the environment passed to the tested program.
+.TP 22n
+\fBenvironment-passthrough =\fR \fIvariable ...\fR
+The named environment variables are passed through from the environment
+nihtest(1)
+is run in to the environment passed to the tested program.
+.TP 22n
+\fBenvironment-unset =\fR \fIvariable ...\fR
+The named environment variables are removed from the environment passed to the tested program.
+.TP 22n
 \fBfeatures-files =\fR \fIfile ...\fR
 Specifies the files to search for feature defines.
 This is used in the
 \fBfeatures\fR
 directive in test cases.
 .TP 22n
 \fBkeep-sandbox =\fR \fIwhen\fR
@@ -162,21 +177,18 @@
 will be used.
 .TP 22n
 \fBtest-input-directories =\fR \fIdirectory ...\fR
 nihtest(1)
 searches the current directory and
 \fIdirectory\fR
 for test cases, input and output files.
-.SH "SETENV"
+.SH "ENVIRONMENT"
 The
-\fBsetenv\fR
+\fBenvironment\fR
 section contains variable and values that will be added as environment variables when the test program is run.
-If the test case contains a
-\fBsetenv\fR
-directive, this section will be ignored.
 .SH "COMPARATORS"
 The
 \fBcomparators\fR
 section specifies programs to use to compare files of certain types.
 The variable names have the format
 \fIgot-extension\fR. \fIexpected-extension\fR,
 the value specifies the command line to use to compare these files.
@@ -203,15 +215,15 @@
 .SH "EXAMPLES"
 .nf
 .RS 0n
 [settings]
 default-program = program_to_test
 program-directories = bin
     tests
-[setenv]
+[environment]
 LC_ALL=en_US.UTF-8
 [comparators]
 zip.zip = zipcmp -v
 .RE
 .fi
 .SH "SEE ALSO"
 nihtest(1)
```

### Comparing `nihtest-1.1.0/manpages/nihtest.conf.mdoc` & `nihtest-1.1.1/manpages/nihtest.conf.mdoc`

 * *Files 1% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 flag.
 This man page describes the format of this configuration file.
 .Sh FILE FORMAT
 The configuration file consists of multiple sections, which are started with
 .Ar [ section-name ] .
 The supported sections are
 .Ic settings ,
-.Ic setenv ,
+.Ic environment ,
 and
 .Ic comparators .
 .Pp
 Each section consists of variable assignments in the format
 .Ar name =
 .Ar value ,
 one per line.
```

### Comparing `nihtest-1.1.0/manpages/nihtest.html` & `nihtest-1.1.1/manpages/nihtest.html`

 * *Files identical despite different names*

### Comparing `nihtest-1.1.0/manpages/nihtest.man` & `nihtest-1.1.1/manpages/nihtest.man`

 * *Files identical despite different names*

### Comparing `nihtest-1.1.0/manpages/nihtest.mdoc` & `nihtest-1.1.1/manpages/nihtest.mdoc`

 * *Files identical despite different names*

### Comparing `nihtest-1.1.0/nihtest/Command.py` & `nihtest-1.1.1/nihtest/Command.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,15 @@
         self.stdin = None
         self.stdin_file = None
         if stdin is None:
             stdin = []
         if isinstance(stdin, str):
             self.stdin_file = stdin
         else:
-            self.stdin = os.linesep.join(stdin) + os.linesep
+            self.stdin = "\n".join(stdin) + "\n"
         self.stdout = None
         self.stderr = None
         self.exit_code = None
 
     def run(self):
         program = self.program if os.path.exists(self.program) else shutil.which(self.program)
         if program is None:
```

### Comparing `nihtest-1.1.0/nihtest/CompareArrays.py` & `nihtest-1.1.1/nihtest/CompareArrays.py`

 * *Files identical despite different names*

### Comparing `nihtest-1.1.0/nihtest/Configuration.py` & `nihtest-1.1.1/nihtest/Configuration.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import configparser
 import enum
 import os.path
+import platform
 import re
 import shlex
 import sys
 
 config_schema = {
     "comparators": True,
     "environment": True,
@@ -145,14 +146,16 @@
 
     def find_input_file(self, filename):
         if file := self.find_file(filename, self.test_input_directories):
             return file
         raise RuntimeError(f"can't find input file '{filename}'")
 
     def find_program(self, program):
+        if platform.system() == "Windows" and not (program.endswith(".exe") or program.endswith(".com")):
+            program += ".exe"
         if file := self.find_file(program, self.program_directories):
             return file
         return program
 
     def find_file(self, filename, directories):
         if os.path.exists(filename):
             return filename
```

### Comparing `nihtest-1.1.0/nihtest/Environment.py` & `nihtest-1.1.1/nihtest/Environment.py`

 * *Files identical despite different names*

### Comparing `nihtest-1.1.0/nihtest/Features.py` & `nihtest-1.1.1/nihtest/Features.py`

 * *Files identical despite different names*

### Comparing `nihtest-1.1.0/nihtest/File.py` & `nihtest-1.1.1/nihtest/File.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,15 +53,15 @@
             output_data = self.result.data
 
         if not output_is_binary:
             try:
                 input_data = Utility.read_lines(input_file_name)
                 return Utility.compare_lines(self.name, output_data, input_data, configuration.verbose != Configuration.When.NEVER)
             except UnicodeDecodeError:
-                output_data = os.linesep.join(output_data)
+                output_data = "\n".join(output_data)
 
         with open(input_file_name, "rb") as file:
             input_data = file.read()
         if input_data != output_data:
             if configuration.verbose != Configuration.When.NEVER:
                 print(f"{self.name} differs:")
                 print("Binary files differ.")
@@ -72,10 +72,9 @@
         if self.input:
             output_file_name = os.path.join(directory, self.name)
             # TODO: create sub-directories in sandbox
             if self.input.file_name is not None:
                 input_file_name = configuration.find_input_file(self.input.file_name)
                 shutil.copyfile(input_file_name, output_file_name)
             else:
-                with open(output_file_name, "w") as file:
-                    for line in self.input.data:
-                        file.write(line + os.linesep)
+                with open(output_file_name, "w", encoding='utf-8') as file:
+                    Utility.write_lines(file, self.input.data)
```

### Comparing `nihtest-1.1.0/nihtest/Sandbox.py` & `nihtest-1.1.1/nihtest/Sandbox.py`

 * *Files identical despite different names*

### Comparing `nihtest-1.1.0/nihtest/Test.py` & `nihtest-1.1.1/nihtest/Test.py`

 * *Files 1% similar despite different names*

```diff
@@ -103,15 +103,15 @@
     def list_files(self):
         files = []
         for directory, _, sub_files in os.walk("."):
             for file in sub_files:
                 if directory == ".":
                     name = file
                 else:
-                    name = os.path.join(directory, file)[2:]
+                    name = os.path.join(directory, file)[2:].replace("\\", "/")
                 files.append(name)
         return files
 
     def precheck_passed(self):
         if not self.case.precheck:
             return True
         program = self.case.configuration.find_program(self.case.precheck[0])
```

### Comparing `nihtest-1.1.0/nihtest/TestCase.py` & `nihtest-1.1.1/nihtest/TestCase.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
         self.environment_clear = configuration.environment_clear
         self.environment_passthrough = configuration.environment_passthrough.copy()
         self.environment_unset = configuration.environment_unset.copy()
         file_name = args.testcase
         if file_name[-5:] != ".test":
             file_name += ".test"
         self.file_name = self.configuration.find_input_file(file_name)
-        self.file = open(self.file_name, mode="r")
+        self.file = open(self.file_name, mode="r", encoding='utf-8')
         self.line_number = 0
         self.directives_seen = {}
         self.arguments = []
         self.description = ""
         self.features = []
         self.files = []
         self.precheck = None
```

### Comparing `nihtest-1.1.0/nihtest/Utility.py` & `nihtest-1.1.1/nihtest/Utility.py`

 * *Files 15% similar despite different names*

```diff
@@ -15,16 +15,16 @@
         write_lines(sys.stdout, diff)
         return False
     return True
 
 
 def read_lines(file_name):
     lines = []
-    with open(file_name, "r") as file:
+    with open(file_name, "r", encoding='utf-8') as file:
         while line := file.readline():
             lines.append(line.rstrip("\r\n"))
     return lines
 
 
 def write_lines(file, lines):
     for line in lines:
-        file.writelines(line + os.linesep)
+        file.writelines(line + "\n")
```

### Comparing `nihtest-1.1.0/nihtest/__main__.py` & `nihtest-1.1.1/nihtest/__main__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import argparse
 import sys
 
 from nihtest import Test
 from nihtest import Configuration
 
-VERSION = "1.1.0"
+VERSION = "1.1.1"
 
 
 def main():
     parser = argparse.ArgumentParser(
         prog='nihtest',
-        description="nihtest " + VERSION  + "\nCopyright (C) 2023 Dieter Baron and Thomas Klausner")
+        description="nihtest " + VERSION + "\nCopyright (C) 2023 Dieter Baron and Thomas Klausner")
     parser.add_argument('testcase', help='Testcase to run')
     parser.add_argument('-C', '--config-file', metavar='FILE', help='use FILE as config file', default="nihtest.conf")
     parser.add_argument('--keep-broken', action='store_true', help='keep sandbox if test fails')
     parser.add_argument('--no-cleanup', action='store_true', help='keep sandbox')
     parser.add_argument('-q', '--quiet', action='store_true', help="don't print test result")
     parser.add_argument('--setup-only', action='store_true', help="set up sandbox, but don't run test")
     parser.add_argument('-v', '--verbose', action='store_true', help="print detailed test results")
```

### Comparing `nihtest-1.1.0/nihtest.egg-info/PKG-INFO` & `nihtest-1.1.1/nihtest.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nihtest
-Version: 1.1.0
+Version: 1.1.1
 Summary: A testing tool for command line utilities.
 Author-email: Dieter Baron <dillo@nih.at>, Thomas Klausner <wiz@gatalith.at>
 License: BSD-3-Clause
 Project-URL: Homepage, https://github.com/nih-at/nihtest
 Project-URL: Bug Tracker, https://github.com/nih-at/nihtest/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `nihtest-1.1.0/nihtest.egg-info/SOURCES.txt` & `nihtest-1.1.1/nihtest.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 LICENSE
 MANIFEST.in
 NEWS.md
 README.md
 TODO.md
 pyproject.toml
 setup.cfg
+manpages/Makefile
 manpages/nihtest-case.html
 manpages/nihtest-case.man
 manpages/nihtest-case.mdoc
 manpages/nihtest.conf.html
 manpages/nihtest.conf.man
 manpages/nihtest.conf.mdoc
 manpages/nihtest.html
```

### Comparing `nihtest-1.1.0/pyproject.toml` & `nihtest-1.1.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "nihtest"
-version = "1.1.0"
+version = "1.1.1"
 authors = [
     { name="Dieter Baron", email="dillo@nih.at" },
     { name="Thomas Klausner", email="wiz@gatalith.at"}
 ]
 description = "A testing tool for command line utilities."
 license = {text = "BSD-3-Clause"}
 readme = "README.md"
@@ -23,15 +23,15 @@
 "Homepage" = "https://github.com/nih-at/nihtest"
 "Bug Tracker" = "https://github.com/nih-at/nihtest/issues"
 
 [project.scripts]
 nihtest = "nihtest.__main__:main"
 
 [tool.bumpver]
-current_version = "1.1.0"
+current_version = "1.1.1"
 version_pattern = "MAJOR.MINOR.PATCH"
 
 [tool.bumpver.file_patterns]
 "nihtest/__main__.py" = [
     'VERSION = "{version}"'
 ]
 "pyproject.toml" = [
```

### Comparing `nihtest-1.1.0/tests/CMakeLists.txt` & `nihtest-1.1.1/tests/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `nihtest-1.1.0/tests/can-preload.c` & `nihtest-1.1.1/tests/can-preload.c`

 * *Files identical despite different names*

### Comparing `nihtest-1.1.0/tests/cat.c` & `nihtest-1.1.1/tests/cat.c`

 * *Files identical despite different names*

### Comparing `nihtest-1.1.0/tests/comparator.c` & `nihtest-1.1.1/tests/comparator.c`

 * *Files identical despite different names*

### Comparing `nihtest-1.1.0/tests/echo.c` & `nihtest-1.1.1/tests/echo.c`

 * *Files identical despite different names*

### Comparing `nihtest-1.1.0/tests/false.c` & `nihtest-1.1.1/tests/false.c`

 * *Files identical despite different names*

### Comparing `nihtest-1.1.0/tests/file.c` & `nihtest-1.1.1/tests/file.c`

 * *Files identical despite different names*

### Comparing `nihtest-1.1.0/tests/getenv.c` & `nihtest-1.1.1/tests/getenv.c`

 * *Files identical despite different names*

### Comparing `nihtest-1.1.0/tests/ineffective-remove.c` & `nihtest-1.1.1/tests/ineffective-remove.c`

 * *Files identical despite different names*

### Comparing `nihtest-1.1.0/tests/parameter-tests-1.test` & `nihtest-1.1.1/tests/parameter-tests-1.test`

 * *Files 4% similar despite different names*

```diff
@@ -25,7 +25,8 @@
 parameter-tests-1.test:22: too few arguments for 'stderr-replace'
 parameter-tests-1.test:23: too many arguments for 'stderr-replace'
 parameter-tests-1.test:24: too many arguments for 'stdin'
 parameter-tests-1.test:25: too many arguments for 'stdout'
 nihtest: invalid test case
 end-of-inline-data
 stderr-replace ^.*/([^/:]*): "\1:"
+stderr-replace "([A-Z]:)?.*\\\\\\\\(.*):" "\2:"
```

### Comparing `nihtest-1.1.0/tests/true.c` & `nihtest-1.1.1/tests/true.c`

 * *Files identical despite different names*

