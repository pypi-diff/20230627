# Comparing `tmp/pluralkit-1.1.4.tar.gz` & `tmp/pluralkit-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pluralkit-1.1.4.tar", last modified: Wed Jun 21 22:04:08 2023, max compression
+gzip compressed data, was "pluralkit-1.1.5.tar", last modified: Tue Jun 27 14:15:25 2023, max compression
```

## Comparing `pluralkit-1.1.4.tar` & `pluralkit-1.1.5.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxrwxr-x   0 k         (1001) k         (1001)        0 2023-06-21 22:04:08.985604 pluralkit-1.1.4/
--rw-rw-r--   0 k         (1001) k         (1001)     1068 2022-12-30 16:02:53.000000 pluralkit-1.1.4/LICENSE
--rw-rw-r--   0 k         (1001) k         (1001)      267 2022-12-30 16:02:53.000000 pluralkit-1.1.4/MANIFEST.in
--rw-rw-r--   0 k         (1001) k         (1001)     4903 2023-06-21 22:04:08.985604 pluralkit-1.1.4/PKG-INFO
--rw-rw-r--   0 k         (1001) k         (1001)     3729 2023-06-19 13:14:23.000000 pluralkit-1.1.4/README.md
-drwxrwxr-x   0 k         (1001) k         (1001)        0 2023-06-21 22:04:08.977603 pluralkit-1.1.4/docs/
--rw-rw-r--   0 k         (1001) k         (1001)      634 2022-12-30 16:02:53.000000 pluralkit-1.1.4/docs/Makefile
--rw-rw-r--   0 k         (1001) k         (1001)      652 2022-12-30 16:02:53.000000 pluralkit-1.1.4/docs/README.md
-drwxrwxr-x   0 k         (1001) k         (1001)        0 2023-06-21 22:04:08.977603 pluralkit-1.1.4/docs/_build/
-drwxrwxr-x   0 k         (1001) k         (1001)        0 2023-06-21 22:04:08.977603 pluralkit-1.1.4/docs/_build/html/
-drwxrwxr-x   0 k         (1001) k         (1001)        0 2023-06-21 22:04:08.977603 pluralkit-1.1.4/docs/_build/html/_sources/
--rw-rw-r--   0 k         (1001) k         (1001)     1273 2022-12-30 16:02:53.000000 pluralkit-1.1.4/docs/_build/html/_sources/index.rst.txt
-drwxrwxr-x   0 k         (1001) k         (1001)        0 2023-06-21 22:04:08.977603 pluralkit-1.1.4/docs/_build/html/_sources/source/
--rw-rw-r--   0 k         (1001) k         (1001)     3929 2022-12-30 19:14:51.000000 pluralkit-1.1.4/docs/_build/html/_sources/source/changelog.rst.txt
--rw-rw-r--   0 k         (1001) k         (1001)    12062 2022-12-30 16:22:51.000000 pluralkit-1.1.4/docs/_build/html/_sources/source/quickstart.rst.txt
-drwxrwxr-x   0 k         (1001) k         (1001)        0 2023-06-21 22:04:08.977603 pluralkit-1.1.4/docs/_build/html/_sources/source/v1/
--rw-rw-r--   0 k         (1001) k         (1001)     1761 2022-12-30 16:02:53.000000 pluralkit-1.1.4/docs/_build/html/_sources/source/v1/api.rst.txt
-drwxrwxr-x   0 k         (1001) k         (1001)        0 2023-06-21 22:04:08.977603 pluralkit-1.1.4/docs/_build/html/_sources/source/v2/
--rw-rw-r--   0 k         (1001) k         (1001)     2943 2022-12-30 18:59:51.000000 pluralkit-1.1.4/docs/_build/html/_sources/source/v2/api.rst.txt
-drwxrwxr-x   0 k         (1001) k         (1001)        0 2023-06-21 22:04:08.977603 pluralkit-1.1.4/docs/_build/html/_static/
--rw-rw-r--   0 k         (1001) k         (1001)        0 2022-12-30 16:23:23.000000 pluralkit-1.1.4/docs/_build/html/_static/__init__.py
-drwxrwxr-x   0 k         (1001) k         (1001)        0 2023-06-21 22:04:08.977603 pluralkit-1.1.4/docs/_build/html/_static/vendor/
-drwxrwxr-x   0 k         (1001) k         (1001)        0 2023-06-21 22:04:08.977603 pluralkit-1.1.4/docs/_build/html/_static/vendor/fontawesome/
-drwxrwxr-x   0 k         (1001) k         (1001)        0 2023-06-21 22:04:08.977603 pluralkit-1.1.4/docs/_build/html/_static/vendor/fontawesome/5.13.0/
--rw-rw-r--   0 k         (1001) k         (1001)     1548 2022-12-30 16:23:23.000000 pluralkit-1.1.4/docs/_build/html/_static/vendor/fontawesome/5.13.0/LICENSE.txt
-drwxrwxr-x   0 k         (1001) k         (1001)        0 2023-06-21 22:04:08.977603 pluralkit-1.1.4/docs/_build/html/_static/vendor/lato_latin-ext/
-drwxrwxr-x   0 k         (1001) k         (1001)        0 2023-06-21 22:04:08.981603 pluralkit-1.1.4/docs/_build/html/_static/vendor/lato_latin-ext/1.44.1/
--rw-rw-r--   0 k         (1001) k         (1001)     1054 2022-12-30 16:23:23.000000 pluralkit-1.1.4/docs/_build/html/_static/vendor/lato_latin-ext/1.44.1/LICENSE.md
-drwxrwxr-x   0 k         (1001) k         (1001)        0 2023-06-21 22:04:08.977603 pluralkit-1.1.4/docs/_build/html/_static/vendor/open-sans_all/
-drwxrwxr-x   0 k         (1001) k         (1001)        0 2023-06-21 22:04:08.981603 pluralkit-1.1.4/docs/_build/html/_static/vendor/open-sans_all/1.44.1/
--rw-rw-r--   0 k         (1001) k         (1001)     1054 2022-12-30 16:23:23.000000 pluralkit-1.1.4/docs/_build/html/_static/vendor/open-sans_all/1.44.1/LICENSE.md
--rw-rw-r--   0 k         (1001) k         (1001)     3312 2022-12-30 16:02:53.000000 pluralkit-1.1.4/docs/conf.py
--rw-rw-r--   0 k         (1001) k         (1001)     1273 2022-12-30 16:02:53.000000 pluralkit-1.1.4/docs/index.rst
--rw-rw-r--   0 k         (1001) k         (1001)      234 2022-12-30 16:02:53.000000 pluralkit-1.1.4/docs/requirements.txt
-drwxrwxr-x   0 k         (1001) k         (1001)        0 2023-06-21 22:04:08.981603 pluralkit-1.1.4/docs/source/
--rw-rw-r--   0 k         (1001) k         (1001)     3932 2022-12-30 19:15:15.000000 pluralkit-1.1.4/docs/source/changelog.rst
--rw-rw-r--   0 k         (1001) k         (1001)    12092 2023-06-19 13:31:19.000000 pluralkit-1.1.4/docs/source/quickstart.rst
-drwxrwxr-x   0 k         (1001) k         (1001)        0 2023-06-21 22:04:08.981603 pluralkit-1.1.4/docs/source/v1/
--rw-rw-r--   0 k         (1001) k         (1001)     1761 2022-12-30 16:02:53.000000 pluralkit-1.1.4/docs/source/v1/api.rst
-drwxrwxr-x   0 k         (1001) k         (1001)        0 2023-06-21 22:04:08.981603 pluralkit-1.1.4/docs/source/v2/
--rw-rw-r--   0 k         (1001) k         (1001)     2943 2022-12-30 18:59:51.000000 pluralkit-1.1.4/docs/source/v2/api.rst
-drwxrwxr-x   0 k         (1001) k         (1001)        0 2023-06-21 22:04:08.981603 pluralkit-1.1.4/pluralkit/
--rw-rw-r--   0 k         (1001) k         (1001)      252 2022-12-31 00:26:34.000000 pluralkit-1.1.4/pluralkit/__init__.py
--rw-rw-r--   0 k         (1001) k         (1001)      248 2023-06-21 22:02:11.000000 pluralkit-1.1.4/pluralkit/__version__.py
-drwxrwxr-x   0 k         (1001) k         (1001)        0 2023-06-21 22:04:08.981603 pluralkit-1.1.4/pluralkit/v1/
--rw-rw-r--   0 k         (1001) k         (1001)      217 2022-12-30 16:02:53.000000 pluralkit-1.1.4/pluralkit/v1/__init__.py
--rw-rw-r--   0 k         (1001) k         (1001)    32468 2022-12-30 16:02:53.000000 pluralkit-1.1.4/pluralkit/v1/client.py
--rw-rw-r--   0 k         (1001) k         (1001)     2824 2022-12-30 16:02:53.000000 pluralkit-1.1.4/pluralkit/v1/errors.py
--rw-rw-r--   0 k         (1001) k         (1001)    38036 2022-12-30 16:02:53.000000 pluralkit-1.1.4/pluralkit/v1/models.py
--rw-rw-r--   0 k         (1001) k         (1001)     4302 2022-12-30 16:02:53.000000 pluralkit-1.1.4/pluralkit/v1/utils.py
-drwxrwxr-x   0 k         (1001) k         (1001)        0 2023-06-21 22:04:08.981603 pluralkit-1.1.4/pluralkit/v2/
--rw-rw-r--   0 k         (1001) k         (1001)      666 2022-12-30 18:59:05.000000 pluralkit-1.1.4/pluralkit/v2/__init__.py
--rw-rw-r--   0 k         (1001) k         (1001)    49625 2023-06-21 22:03:10.000000 pluralkit-1.1.4/pluralkit/v2/client.py
--rw-rw-r--   0 k         (1001) k         (1001)     2821 2022-12-30 16:02:53.000000 pluralkit-1.1.4/pluralkit/v2/errors.py
--rw-rw-r--   0 k         (1001) k         (1001)    39157 2023-06-19 13:12:49.000000 pluralkit-1.1.4/pluralkit/v2/models.py
-drwxrwxr-x   0 k         (1001) k         (1001)        0 2023-06-21 22:04:08.981603 pluralkit-1.1.4/pluralkit.egg-info/
--rw-rw-r--   0 k         (1001) k         (1001)     4903 2023-06-21 22:04:08.000000 pluralkit-1.1.4/pluralkit.egg-info/PKG-INFO
--rw-rw-r--   0 k         (1001) k         (1001)     1166 2023-06-21 22:04:08.000000 pluralkit-1.1.4/pluralkit.egg-info/SOURCES.txt
--rw-rw-r--   0 k         (1001) k         (1001)        1 2023-06-21 22:04:08.000000 pluralkit-1.1.4/pluralkit.egg-info/dependency_links.txt
--rw-rw-r--   0 k         (1001) k         (1001)      188 2023-06-21 22:04:08.000000 pluralkit-1.1.4/pluralkit.egg-info/requires.txt
--rw-rw-r--   0 k         (1001) k         (1001)       10 2023-06-21 22:04:08.000000 pluralkit-1.1.4/pluralkit.egg-info/top_level.txt
--rw-rw-r--   0 k         (1001) k         (1001)       38 2023-06-21 22:04:08.985604 pluralkit-1.1.4/setup.cfg
--rw-rw-r--   0 k         (1001) k         (1001)     2217 2022-12-31 00:34:09.000000 pluralkit-1.1.4/setup.py
-drwxrwxr-x   0 k         (1001) k         (1001)        0 2023-06-21 22:04:08.985604 pluralkit-1.1.4/tests/
--rw-rw-r--   0 k         (1001) k         (1001)     6785 2022-12-30 16:02:53.000000 pluralkit-1.1.4/tests/test_member.py
--rw-rw-r--   0 k         (1001) k         (1001)      503 2022-12-30 16:02:53.000000 pluralkit-1.1.4/tests/test_misc.py
--rw-rw-r--   0 k         (1001) k         (1001)     2671 2022-12-30 16:02:53.000000 pluralkit-1.1.4/tests/test_system.py
+drwxrwxr-x   0 k         (1001) k         (1001)        0 2023-06-27 14:15:25.139524 pluralkit-1.1.5/
+-rw-rw-r--   0 k         (1001) k         (1001)     1068 2022-12-30 16:02:53.000000 pluralkit-1.1.5/LICENSE
+-rw-rw-r--   0 k         (1001) k         (1001)      267 2022-12-30 16:02:53.000000 pluralkit-1.1.5/MANIFEST.in
+-rw-rw-r--   0 k         (1001) k         (1001)     4903 2023-06-27 14:15:25.139524 pluralkit-1.1.5/PKG-INFO
+-rw-rw-r--   0 k         (1001) k         (1001)     3729 2023-06-19 13:14:23.000000 pluralkit-1.1.5/README.md
+drwxrwxr-x   0 k         (1001) k         (1001)        0 2023-06-27 14:15:25.135524 pluralkit-1.1.5/docs/
+-rw-rw-r--   0 k         (1001) k         (1001)      634 2022-12-30 16:02:53.000000 pluralkit-1.1.5/docs/Makefile
+-rw-rw-r--   0 k         (1001) k         (1001)      652 2022-12-30 16:02:53.000000 pluralkit-1.1.5/docs/README.md
+drwxrwxr-x   0 k         (1001) k         (1001)        0 2023-06-27 14:15:25.131524 pluralkit-1.1.5/docs/_build/
+drwxrwxr-x   0 k         (1001) k         (1001)        0 2023-06-27 14:15:25.131524 pluralkit-1.1.5/docs/_build/html/
+drwxrwxr-x   0 k         (1001) k         (1001)        0 2023-06-27 14:15:25.135524 pluralkit-1.1.5/docs/_build/html/_sources/
+-rw-rw-r--   0 k         (1001) k         (1001)     1273 2022-12-30 16:02:53.000000 pluralkit-1.1.5/docs/_build/html/_sources/index.rst.txt
+drwxrwxr-x   0 k         (1001) k         (1001)        0 2023-06-27 14:15:25.135524 pluralkit-1.1.5/docs/_build/html/_sources/source/
+-rw-rw-r--   0 k         (1001) k         (1001)     3929 2022-12-30 19:14:51.000000 pluralkit-1.1.5/docs/_build/html/_sources/source/changelog.rst.txt
+-rw-rw-r--   0 k         (1001) k         (1001)    12062 2022-12-30 16:22:51.000000 pluralkit-1.1.5/docs/_build/html/_sources/source/quickstart.rst.txt
+drwxrwxr-x   0 k         (1001) k         (1001)        0 2023-06-27 14:15:25.135524 pluralkit-1.1.5/docs/_build/html/_sources/source/v1/
+-rw-rw-r--   0 k         (1001) k         (1001)     1761 2022-12-30 16:02:53.000000 pluralkit-1.1.5/docs/_build/html/_sources/source/v1/api.rst.txt
+drwxrwxr-x   0 k         (1001) k         (1001)        0 2023-06-27 14:15:25.135524 pluralkit-1.1.5/docs/_build/html/_sources/source/v2/
+-rw-rw-r--   0 k         (1001) k         (1001)     2943 2022-12-30 18:59:51.000000 pluralkit-1.1.5/docs/_build/html/_sources/source/v2/api.rst.txt
+drwxrwxr-x   0 k         (1001) k         (1001)        0 2023-06-27 14:15:25.135524 pluralkit-1.1.5/docs/_build/html/_static/
+-rw-rw-r--   0 k         (1001) k         (1001)        0 2022-12-30 16:23:23.000000 pluralkit-1.1.5/docs/_build/html/_static/__init__.py
+drwxrwxr-x   0 k         (1001) k         (1001)        0 2023-06-27 14:15:25.131524 pluralkit-1.1.5/docs/_build/html/_static/vendor/
+drwxrwxr-x   0 k         (1001) k         (1001)        0 2023-06-27 14:15:25.131524 pluralkit-1.1.5/docs/_build/html/_static/vendor/fontawesome/
+drwxrwxr-x   0 k         (1001) k         (1001)        0 2023-06-27 14:15:25.135524 pluralkit-1.1.5/docs/_build/html/_static/vendor/fontawesome/5.13.0/
+-rw-rw-r--   0 k         (1001) k         (1001)     1548 2022-12-30 16:23:23.000000 pluralkit-1.1.5/docs/_build/html/_static/vendor/fontawesome/5.13.0/LICENSE.txt
+drwxrwxr-x   0 k         (1001) k         (1001)        0 2023-06-27 14:15:25.131524 pluralkit-1.1.5/docs/_build/html/_static/vendor/lato_latin-ext/
+drwxrwxr-x   0 k         (1001) k         (1001)        0 2023-06-27 14:15:25.135524 pluralkit-1.1.5/docs/_build/html/_static/vendor/lato_latin-ext/1.44.1/
+-rw-rw-r--   0 k         (1001) k         (1001)     1054 2022-12-30 16:23:23.000000 pluralkit-1.1.5/docs/_build/html/_static/vendor/lato_latin-ext/1.44.1/LICENSE.md
+drwxrwxr-x   0 k         (1001) k         (1001)        0 2023-06-27 14:15:25.131524 pluralkit-1.1.5/docs/_build/html/_static/vendor/open-sans_all/
+drwxrwxr-x   0 k         (1001) k         (1001)        0 2023-06-27 14:15:25.135524 pluralkit-1.1.5/docs/_build/html/_static/vendor/open-sans_all/1.44.1/
+-rw-rw-r--   0 k         (1001) k         (1001)     1054 2022-12-30 16:23:23.000000 pluralkit-1.1.5/docs/_build/html/_static/vendor/open-sans_all/1.44.1/LICENSE.md
+-rw-rw-r--   0 k         (1001) k         (1001)     3312 2022-12-30 16:02:53.000000 pluralkit-1.1.5/docs/conf.py
+-rw-rw-r--   0 k         (1001) k         (1001)     1273 2022-12-30 16:02:53.000000 pluralkit-1.1.5/docs/index.rst
+-rw-rw-r--   0 k         (1001) k         (1001)      234 2022-12-30 16:02:53.000000 pluralkit-1.1.5/docs/requirements.txt
+drwxrwxr-x   0 k         (1001) k         (1001)        0 2023-06-27 14:15:25.135524 pluralkit-1.1.5/docs/source/
+-rw-rw-r--   0 k         (1001) k         (1001)     3932 2022-12-30 19:15:15.000000 pluralkit-1.1.5/docs/source/changelog.rst
+-rw-rw-r--   0 k         (1001) k         (1001)    12092 2023-06-19 13:31:19.000000 pluralkit-1.1.5/docs/source/quickstart.rst
+drwxrwxr-x   0 k         (1001) k         (1001)        0 2023-06-27 14:15:25.135524 pluralkit-1.1.5/docs/source/v1/
+-rw-rw-r--   0 k         (1001) k         (1001)     1761 2022-12-30 16:02:53.000000 pluralkit-1.1.5/docs/source/v1/api.rst
+drwxrwxr-x   0 k         (1001) k         (1001)        0 2023-06-27 14:15:25.135524 pluralkit-1.1.5/docs/source/v2/
+-rw-rw-r--   0 k         (1001) k         (1001)     2943 2022-12-30 18:59:51.000000 pluralkit-1.1.5/docs/source/v2/api.rst
+drwxrwxr-x   0 k         (1001) k         (1001)        0 2023-06-27 14:15:25.139524 pluralkit-1.1.5/pluralkit/
+-rw-rw-r--   0 k         (1001) k         (1001)      252 2022-12-31 00:26:34.000000 pluralkit-1.1.5/pluralkit/__init__.py
+-rw-rw-r--   0 k         (1001) k         (1001)      248 2023-06-27 14:11:00.000000 pluralkit-1.1.5/pluralkit/__version__.py
+drwxrwxr-x   0 k         (1001) k         (1001)        0 2023-06-27 14:15:25.139524 pluralkit-1.1.5/pluralkit/v1/
+-rw-rw-r--   0 k         (1001) k         (1001)      217 2022-12-30 16:02:53.000000 pluralkit-1.1.5/pluralkit/v1/__init__.py
+-rw-rw-r--   0 k         (1001) k         (1001)    32468 2022-12-30 16:02:53.000000 pluralkit-1.1.5/pluralkit/v1/client.py
+-rw-rw-r--   0 k         (1001) k         (1001)     2824 2022-12-30 16:02:53.000000 pluralkit-1.1.5/pluralkit/v1/errors.py
+-rw-rw-r--   0 k         (1001) k         (1001)    38036 2022-12-30 16:02:53.000000 pluralkit-1.1.5/pluralkit/v1/models.py
+-rw-rw-r--   0 k         (1001) k         (1001)     4302 2022-12-30 16:02:53.000000 pluralkit-1.1.5/pluralkit/v1/utils.py
+drwxrwxr-x   0 k         (1001) k         (1001)        0 2023-06-27 14:15:25.139524 pluralkit-1.1.5/pluralkit/v2/
+-rw-rw-r--   0 k         (1001) k         (1001)      666 2022-12-30 18:59:05.000000 pluralkit-1.1.5/pluralkit/v2/__init__.py
+-rw-rw-r--   0 k         (1001) k         (1001)    49625 2023-06-21 22:03:10.000000 pluralkit-1.1.5/pluralkit/v2/client.py
+-rw-rw-r--   0 k         (1001) k         (1001)     2821 2022-12-30 16:02:53.000000 pluralkit-1.1.5/pluralkit/v2/errors.py
+-rw-rw-r--   0 k         (1001) k         (1001)    39172 2023-06-27 14:12:14.000000 pluralkit-1.1.5/pluralkit/v2/models.py
+drwxrwxr-x   0 k         (1001) k         (1001)        0 2023-06-27 14:15:25.139524 pluralkit-1.1.5/pluralkit.egg-info/
+-rw-rw-r--   0 k         (1001) k         (1001)     4903 2023-06-27 14:15:25.000000 pluralkit-1.1.5/pluralkit.egg-info/PKG-INFO
+-rw-rw-r--   0 k         (1001) k         (1001)     1166 2023-06-27 14:15:25.000000 pluralkit-1.1.5/pluralkit.egg-info/SOURCES.txt
+-rw-rw-r--   0 k         (1001) k         (1001)        1 2023-06-27 14:15:25.000000 pluralkit-1.1.5/pluralkit.egg-info/dependency_links.txt
+-rw-rw-r--   0 k         (1001) k         (1001)      188 2023-06-27 14:15:25.000000 pluralkit-1.1.5/pluralkit.egg-info/requires.txt
+-rw-rw-r--   0 k         (1001) k         (1001)       10 2023-06-27 14:15:25.000000 pluralkit-1.1.5/pluralkit.egg-info/top_level.txt
+-rw-rw-r--   0 k         (1001) k         (1001)       38 2023-06-27 14:15:25.139524 pluralkit-1.1.5/setup.cfg
+-rw-rw-r--   0 k         (1001) k         (1001)     2217 2022-12-31 00:34:09.000000 pluralkit-1.1.5/setup.py
+drwxrwxr-x   0 k         (1001) k         (1001)        0 2023-06-27 14:15:25.139524 pluralkit-1.1.5/tests/
+-rw-rw-r--   0 k         (1001) k         (1001)     6785 2022-12-30 16:02:53.000000 pluralkit-1.1.5/tests/test_member.py
+-rw-rw-r--   0 k         (1001) k         (1001)      503 2022-12-30 16:02:53.000000 pluralkit-1.1.5/tests/test_misc.py
+-rw-rw-r--   0 k         (1001) k         (1001)     2671 2022-12-30 16:02:53.000000 pluralkit-1.1.5/tests/test_system.py
```

### Comparing `pluralkit-1.1.4/LICENSE` & `pluralkit-1.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pluralkit-1.1.4/PKG-INFO` & `pluralkit-1.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pluralkit
-Version: 1.1.4
+Version: 1.1.5
 Summary: Python wrapper for PluralKit's API.
 Home-page: https://github.com/almonds0166/pluralkit.py
 Author: Madison Landry, Alyx Warner
 Author-email: pkpy@mit.edu
 License: MIT
 Project-URL: Documentation, https://pluralkit.readthedocs.io/en/latest/
 Project-URL: Issue tracker, https://github.com/almonds0166/pluralkit.py/issues
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pluralkit Version: 1.1.4 Summary: Python wrapper
+Metadata-Version: 2.1 Name: pluralkit Version: 1.1.5 Summary: Python wrapper
 for PluralKit's API. Home-page: https://github.com/almonds0166/pluralkit.py
 Author: Madison Landry, Alyx Warner Author-email: pkpy@mit.edu License: MIT
 Project-URL: Documentation, https://pluralkit.readthedocs.io/en/latest/
 Project-URL: Issue tracker, https://github.com/almonds0166/pluralkit.py/issues
 Platform: UNKNOWN Classifier: Development Status :: 3 - Alpha Classifier:
 Programming Language :: Python :: 3.6 Classifier: Programming Language ::
 Python :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
```

### Comparing `pluralkit-1.1.4/README.md` & `pluralkit-1.1.5/README.md`

 * *Files identical despite different names*

### Comparing `pluralkit-1.1.4/docs/Makefile` & `pluralkit-1.1.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pluralkit-1.1.4/docs/README.md` & `pluralkit-1.1.5/docs/README.md`

 * *Files identical despite different names*

### Comparing `pluralkit-1.1.4/docs/_build/html/_sources/index.rst.txt` & `pluralkit-1.1.5/docs/_build/html/_sources/index.rst.txt`

 * *Files identical despite different names*

### Comparing `pluralkit-1.1.4/docs/_build/html/_sources/source/changelog.rst.txt` & `pluralkit-1.1.5/docs/_build/html/_sources/source/changelog.rst.txt`

 * *Files identical despite different names*

### Comparing `pluralkit-1.1.4/docs/_build/html/_sources/source/quickstart.rst.txt` & `pluralkit-1.1.5/docs/_build/html/_sources/source/quickstart.rst.txt`

 * *Files identical despite different names*

### Comparing `pluralkit-1.1.4/docs/_build/html/_sources/source/v1/api.rst.txt` & `pluralkit-1.1.5/docs/_build/html/_sources/source/v1/api.rst.txt`

 * *Files identical despite different names*

### Comparing `pluralkit-1.1.4/docs/_build/html/_sources/source/v2/api.rst.txt` & `pluralkit-1.1.5/docs/_build/html/_sources/source/v2/api.rst.txt`

 * *Files identical despite different names*

### Comparing `pluralkit-1.1.4/docs/_build/html/_static/vendor/fontawesome/5.13.0/LICENSE.txt` & `pluralkit-1.1.5/docs/_build/html/_static/vendor/fontawesome/5.13.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pluralkit-1.1.4/docs/_build/html/_static/vendor/lato_latin-ext/1.44.1/LICENSE.md` & `pluralkit-1.1.5/docs/_build/html/_static/vendor/lato_latin-ext/1.44.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pluralkit-1.1.4/docs/_build/html/_static/vendor/open-sans_all/1.44.1/LICENSE.md` & `pluralkit-1.1.5/docs/_build/html/_static/vendor/open-sans_all/1.44.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pluralkit-1.1.4/docs/conf.py` & `pluralkit-1.1.5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pluralkit-1.1.4/docs/index.rst` & `pluralkit-1.1.5/docs/index.rst`

 * *Files identical despite different names*

### Comparing `pluralkit-1.1.4/docs/source/changelog.rst` & `pluralkit-1.1.5/docs/source/changelog.rst`

 * *Files identical despite different names*

### Comparing `pluralkit-1.1.4/docs/source/quickstart.rst` & `pluralkit-1.1.5/docs/source/quickstart.rst`

 * *Files identical despite different names*

### Comparing `pluralkit-1.1.4/docs/source/v1/api.rst` & `pluralkit-1.1.5/docs/source/v1/api.rst`

 * *Files identical despite different names*

### Comparing `pluralkit-1.1.4/docs/source/v2/api.rst` & `pluralkit-1.1.5/docs/source/v2/api.rst`

 * *Files identical despite different names*

### Comparing `pluralkit-1.1.4/pluralkit/v1/client.py` & `pluralkit-1.1.5/pluralkit/v1/client.py`

 * *Files identical despite different names*

### Comparing `pluralkit-1.1.4/pluralkit/v1/errors.py` & `pluralkit-1.1.5/pluralkit/v1/errors.py`

 * *Files identical despite different names*

### Comparing `pluralkit-1.1.4/pluralkit/v1/models.py` & `pluralkit-1.1.5/pluralkit/v1/models.py`

 * *Files identical despite different names*

### Comparing `pluralkit-1.1.4/pluralkit/v1/utils.py` & `pluralkit-1.1.5/pluralkit/v1/utils.py`

 * *Files identical despite different names*

### Comparing `pluralkit-1.1.4/pluralkit/v2/__init__.py` & `pluralkit-1.1.5/pluralkit/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `pluralkit-1.1.4/pluralkit/v2/client.py` & `pluralkit-1.1.5/pluralkit/v2/client.py`

 * *Files identical despite different names*

### Comparing `pluralkit-1.1.4/pluralkit/v2/errors.py` & `pluralkit-1.1.5/pluralkit/v2/errors.py`

 * *Files identical despite different names*

### Comparing `pluralkit-1.1.4/pluralkit/v2/models.py` & `pluralkit-1.1.5/pluralkit/v2/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -575,15 +575,15 @@
         prefix (Optional[str]): Prefix that will enclose proxied messages.
         suffix (Optional[str]): Suffix that will enclose proxied messages.
     """
     def __init__(self,
         prefix: Optional[str]=None,
         suffix: Optional[str]=None,
         *,
-        proxy_tag: Dict[str,str],
+        proxy_tag: Optional[Dict[str,str]]=None,
     ):
 
         if proxy_tag is not None:
             prefix = prefix or proxy_tag["prefix"]
             suffix = suffix or proxy_tag["suffix"]
 
         assert prefix or suffix, \
```

### Comparing `pluralkit-1.1.4/pluralkit.egg-info/PKG-INFO` & `pluralkit-1.1.5/pluralkit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pluralkit
-Version: 1.1.4
+Version: 1.1.5
 Summary: Python wrapper for PluralKit's API.
 Home-page: https://github.com/almonds0166/pluralkit.py
 Author: Madison Landry, Alyx Warner
 Author-email: pkpy@mit.edu
 License: MIT
 Project-URL: Documentation, https://pluralkit.readthedocs.io/en/latest/
 Project-URL: Issue tracker, https://github.com/almonds0166/pluralkit.py/issues
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pluralkit Version: 1.1.4 Summary: Python wrapper
+Metadata-Version: 2.1 Name: pluralkit Version: 1.1.5 Summary: Python wrapper
 for PluralKit's API. Home-page: https://github.com/almonds0166/pluralkit.py
 Author: Madison Landry, Alyx Warner Author-email: pkpy@mit.edu License: MIT
 Project-URL: Documentation, https://pluralkit.readthedocs.io/en/latest/
 Project-URL: Issue tracker, https://github.com/almonds0166/pluralkit.py/issues
 Platform: UNKNOWN Classifier: Development Status :: 3 - Alpha Classifier:
 Programming Language :: Python :: 3.6 Classifier: Programming Language ::
 Python :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
```

### Comparing `pluralkit-1.1.4/pluralkit.egg-info/SOURCES.txt` & `pluralkit-1.1.5/pluralkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pluralkit-1.1.4/setup.py` & `pluralkit-1.1.5/setup.py`

 * *Files identical despite different names*

### Comparing `pluralkit-1.1.4/tests/test_member.py` & `pluralkit-1.1.5/tests/test_member.py`

 * *Files identical despite different names*

### Comparing `pluralkit-1.1.4/tests/test_system.py` & `pluralkit-1.1.5/tests/test_system.py`

 * *Files identical despite different names*

