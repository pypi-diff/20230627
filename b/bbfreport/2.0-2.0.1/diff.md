# Comparing `tmp/bbfreport-2.0.tar.gz` & `tmp/bbfreport-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bbfreport-2.0.tar", last modified: Thu Jun 15 15:49:55 2023, max compression
+gzip compressed data, was "bbfreport-2.0.1.tar", last modified: Tue Jun 27 14:29:59 2023, max compression
```

## Comparing `bbfreport-2.0.tar` & `bbfreport-2.0.1.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 william    (501) staff       (20)        0 2023-06-15 15:49:55.935409 bbfreport-2.0/
--rw-r--r--   0 william    (501) staff       (20)     1783 2020-03-27 16:04:44.000000 bbfreport-2.0/LICENSE
--rw-r--r--   0 william    (501) staff       (20)     6575 2023-06-15 15:49:55.935275 bbfreport-2.0/PKG-INFO
--rw-r--r--   0 william    (501) staff       (20)     6035 2023-06-15 15:19:37.000000 bbfreport-2.0/README.md
-drwxr-xr-x   0 william    (501) staff       (20)        0 2023-06-15 15:49:55.927616 bbfreport-2.0/bbfreport/
--rw-r--r--   0 william    (501) staff       (20)     2760 2023-06-15 14:15:47.000000 bbfreport-2.0/bbfreport/__init__.py
--rw-r--r--   0 william    (501) staff       (20)    21138 2023-06-15 13:01:39.000000 bbfreport-2.0/bbfreport/content.py
--rw-r--r--   0 william    (501) staff       (20)     2623 2023-04-17 10:19:21.000000 bbfreport-2.0/bbfreport/exception.py
--rw-r--r--   0 william    (501) staff       (20)     9610 2023-06-12 13:34:38.000000 bbfreport-2.0/bbfreport/file.py
--rw-r--r--   0 william    (501) staff       (20)     2238 2023-04-17 10:19:21.000000 bbfreport-2.0/bbfreport/format.py
--rw-r--r--   0 william    (501) staff       (20)    17849 2023-06-15 13:01:39.000000 bbfreport-2.0/bbfreport/macro.py
-drwxr-xr-x   0 william    (501) staff       (20)        0 2023-06-15 15:49:55.928920 bbfreport-2.0/bbfreport/macros/
--rw-r--r--   0 william    (501) staff       (20)     2166 2023-04-17 10:19:21.000000 bbfreport-2.0/bbfreport/macros/__init__.py
--rw-r--r--   0 william    (501) staff       (20)    58134 2023-06-15 13:01:39.000000 bbfreport-2.0/bbfreport/macros/macros.py
--rw-r--r--   0 william    (501) staff       (20)      379 2023-04-17 10:19:21.000000 bbfreport-2.0/bbfreport/macros/test.py
--rw-r--r--   0 william    (501) staff       (20)   211706 2023-06-15 13:01:39.000000 bbfreport-2.0/bbfreport/node.py
--rw-r--r--   0 william    (501) staff       (20)    12419 2023-06-02 08:47:27.000000 bbfreport-2.0/bbfreport/parser.py
--rw-r--r--   0 william    (501) staff       (20)    19265 2023-06-12 13:34:38.000000 bbfreport-2.0/bbfreport/path.py
--rw-r--r--   0 william    (501) staff       (20)    11924 2023-04-17 10:19:21.000000 bbfreport-2.0/bbfreport/plugin.py
-drwxr-xr-x   0 william    (501) staff       (20)        0 2023-06-15 15:49:55.934023 bbfreport-2.0/bbfreport/plugins/
--rw-r--r--   0 william    (501) staff       (20)     1993 2023-01-02 15:02:10.000000 bbfreport-2.0/bbfreport/plugins/__init__.py
--rw-r--r--   0 william    (501) staff       (20)     1836 2023-06-12 13:34:38.000000 bbfreport-2.0/bbfreport/plugins/automodel.py
--rw-r--r--   0 william    (501) staff       (20)     3960 2023-06-12 13:34:38.000000 bbfreport-2.0/bbfreport/plugins/depend.py
--rw-r--r--   0 william    (501) staff       (20)    24338 2023-06-15 13:01:39.000000 bbfreport-2.0/bbfreport/plugins/diff.py
--rw-r--r--   0 william    (501) staff       (20)     4589 2023-01-02 15:02:10.000000 bbfreport-2.0/bbfreport/plugins/enumTransform.py
-drwxr-xr-x   0 william    (501) staff       (20)        0 2023-06-15 15:49:55.934646 bbfreport-2.0/bbfreport/plugins/examples/
--rw-r--r--   0 william    (501) staff       (20)        0 2023-01-02 15:02:10.000000 bbfreport-2.0/bbfreport/plugins/examples/__init__.py
--rw-r--r--   0 william    (501) staff       (20)     4738 2023-04-17 10:19:21.000000 bbfreport-2.0/bbfreport/plugins/examples/candenyTransform.py
--rw-r--r--   0 william    (501) staff       (20)     4718 2023-01-02 15:02:10.000000 bbfreport-2.0/bbfreport/plugins/examples/editTransform.py
--rw-r--r--   0 william    (501) staff       (20)     8099 2023-01-02 15:02:10.000000 bbfreport-2.0/bbfreport/plugins/expatParser.py
--rw-r--r--   0 william    (501) staff       (20)     2008 2023-06-02 08:47:27.000000 bbfreport-2.0/bbfreport/plugins/html.py
--rw-r--r--   0 william    (501) staff       (20)    29464 2023-06-15 13:01:39.000000 bbfreport-2.0/bbfreport/plugins/lint.py
--rw-r--r--   0 william    (501) staff       (20)    85005 2023-06-15 13:01:39.000000 bbfreport-2.0/bbfreport/plugins/markdown.py
--rw-r--r--   0 william    (501) staff       (20)     1934 2023-04-17 10:19:21.000000 bbfreport-2.0/bbfreport/plugins/null.py
--rw-r--r--   0 william    (501) staff       (20)     6442 2023-04-17 10:19:21.000000 bbfreport-2.0/bbfreport/plugins/pyxbParser.py
--rw-r--r--   0 william    (501) staff       (20)     9829 2023-04-17 10:19:21.000000 bbfreport-2.0/bbfreport/plugins/relrefTransform.py
--rw-r--r--   0 william    (501) staff       (20)     3379 2023-01-02 15:02:10.000000 bbfreport-2.0/bbfreport/plugins/split.py
--rw-r--r--   0 william    (501) staff       (20)     2808 2023-01-02 15:02:10.000000 bbfreport-2.0/bbfreport/plugins/statusTransform.py
--rw-r--r--   0 william    (501) staff       (20)    11955 2023-06-15 13:01:39.000000 bbfreport-2.0/bbfreport/plugins/textFormat.py
--rw-r--r--   0 william    (501) staff       (20)     4789 2023-05-29 07:43:27.000000 bbfreport-2.0/bbfreport/plugins/used.py
--rw-r--r--   0 william    (501) staff       (20)     8393 2023-04-17 10:19:21.000000 bbfreport-2.0/bbfreport/plugins/versionTransform.py
--rw-r--r--   0 william    (501) staff       (20)    22310 2023-06-15 13:01:39.000000 bbfreport-2.0/bbfreport/plugins/xmlFormat.py
--rw-r--r--   0 william    (501) staff       (20)     3881 2023-01-02 15:02:10.000000 bbfreport-2.0/bbfreport/plugins/xmltodictParser.py
--rw-r--r--   0 william    (501) staff       (20)    69903 2023-06-15 13:01:39.000000 bbfreport-2.0/bbfreport/property.py
--rw-r--r--   0 william    (501) staff       (20)     2218 2023-04-17 10:19:21.000000 bbfreport-2.0/bbfreport/transform.py
--rw-r--r--   0 william    (501) staff       (20)    29888 2023-06-12 13:34:38.000000 bbfreport-2.0/bbfreport/utility.py
--rw-r--r--   0 william    (501) staff       (20)    35865 2023-06-15 13:01:39.000000 bbfreport-2.0/bbfreport/visitor.py
-drwxr-xr-x   0 william    (501) staff       (20)        0 2023-06-15 15:49:55.928290 bbfreport-2.0/bbfreport.egg-info/
--rw-r--r--   0 william    (501) staff       (20)     6575 2023-06-15 15:49:55.000000 bbfreport-2.0/bbfreport.egg-info/PKG-INFO
--rw-r--r--   0 william    (501) staff       (20)     1263 2023-06-15 15:49:55.000000 bbfreport-2.0/bbfreport.egg-info/SOURCES.txt
--rw-r--r--   0 william    (501) staff       (20)        1 2023-06-15 15:49:55.000000 bbfreport-2.0/bbfreport.egg-info/dependency_links.txt
--rw-r--r--   0 william    (501) staff       (20)       10 2023-06-15 15:49:55.000000 bbfreport-2.0/bbfreport.egg-info/top_level.txt
-drwxr-xr-x   0 william    (501) staff       (20)        0 2023-06-15 15:49:55.934792 bbfreport-2.0/bin/
--rwxr-xr-x   0 william    (501) staff       (20)    18122 2023-06-15 15:10:48.000000 bbfreport-2.0/bin/report.py
--rw-r--r--   0 william    (501) staff       (20)      732 2023-06-15 15:38:02.000000 bbfreport-2.0/pyproject.toml
--rw-r--r--   0 william    (501) staff       (20)       38 2023-06-15 15:49:55.935448 bbfreport-2.0/setup.cfg
+drwxr-xr-x   0 william    (501) staff       (20)        0 2023-06-27 14:29:59.413690 bbfreport-2.0.1/
+-rw-r--r--   0 william    (501) staff       (20)     1788 2023-06-27 11:07:36.000000 bbfreport-2.0.1/LICENSE
+-rw-r--r--   0 william    (501) staff       (20)     7233 2023-06-27 14:29:59.413522 bbfreport-2.0.1/PKG-INFO
+-rw-r--r--   0 william    (501) staff       (20)     6691 2023-06-27 14:29:55.000000 bbfreport-2.0.1/README.md
+drwxr-xr-x   0 william    (501) staff       (20)        0 2023-06-27 14:29:59.403652 bbfreport-2.0.1/bbfreport/
+-rw-r--r--   0 william    (501) staff       (20)     3353 2023-06-27 12:28:54.000000 bbfreport-2.0.1/bbfreport/__init__.py
+-rw-r--r--   0 william    (501) staff       (20)    21138 2023-06-19 16:17:54.000000 bbfreport-2.0.1/bbfreport/content.py
+-rw-r--r--   0 william    (501) staff       (20)     2623 2023-06-19 16:17:04.000000 bbfreport-2.0.1/bbfreport/exception.py
+-rw-r--r--   0 william    (501) staff       (20)     9610 2023-06-19 16:17:54.000000 bbfreport-2.0.1/bbfreport/file.py
+-rw-r--r--   0 william    (501) staff       (20)     2238 2023-06-19 16:17:54.000000 bbfreport-2.0.1/bbfreport/format.py
+-rw-r--r--   0 william    (501) staff       (20)    17849 2023-06-19 16:17:54.000000 bbfreport-2.0.1/bbfreport/macro.py
+drwxr-xr-x   0 william    (501) staff       (20)        0 2023-06-27 14:29:59.405406 bbfreport-2.0.1/bbfreport/macros/
+-rw-r--r--   0 william    (501) staff       (20)     2166 2023-06-19 16:17:54.000000 bbfreport-2.0.1/bbfreport/macros/__init__.py
+-rw-r--r--   0 william    (501) staff       (20)    58134 2023-06-19 16:17:54.000000 bbfreport-2.0.1/bbfreport/macros/macros.py
+-rw-r--r--   0 william    (501) staff       (20)      379 2023-06-19 16:17:54.000000 bbfreport-2.0.1/bbfreport/macros/test.py
+-rw-r--r--   0 william    (501) staff       (20)   211706 2023-06-19 16:17:54.000000 bbfreport-2.0.1/bbfreport/node.py
+-rw-r--r--   0 william    (501) staff       (20)    12419 2023-06-19 16:17:54.000000 bbfreport-2.0.1/bbfreport/parser.py
+-rw-r--r--   0 william    (501) staff       (20)    19265 2023-06-19 16:17:54.000000 bbfreport-2.0.1/bbfreport/path.py
+-rw-r--r--   0 william    (501) staff       (20)    11924 2023-06-19 16:17:54.000000 bbfreport-2.0.1/bbfreport/plugin.py
+drwxr-xr-x   0 william    (501) staff       (20)        0 2023-06-27 14:29:59.410874 bbfreport-2.0.1/bbfreport/plugins/
+-rw-r--r--   0 william    (501) staff       (20)     1993 2023-06-19 16:17:05.000000 bbfreport-2.0.1/bbfreport/plugins/__init__.py
+-rw-r--r--   0 william    (501) staff       (20)     1836 2023-06-19 16:17:54.000000 bbfreport-2.0.1/bbfreport/plugins/automodel.py
+-rw-r--r--   0 william    (501) staff       (20)     3960 2023-06-19 16:17:54.000000 bbfreport-2.0.1/bbfreport/plugins/depend.py
+-rw-r--r--   0 william    (501) staff       (20)    24338 2023-06-19 16:17:54.000000 bbfreport-2.0.1/bbfreport/plugins/diff.py
+drwxr-xr-x   0 william    (501) staff       (20)        0 2023-06-27 14:29:59.412995 bbfreport-2.0.1/bbfreport/plugins/examples/
+-rw-r--r--   0 william    (501) staff       (20)        0 2023-06-19 16:17:05.000000 bbfreport-2.0.1/bbfreport/plugins/examples/__init__.py
+-rw-r--r--   0 william    (501) staff       (20)     4738 2023-06-19 16:17:54.000000 bbfreport-2.0.1/bbfreport/plugins/examples/candenyTransform.py
+-rw-r--r--   0 william    (501) staff       (20)     4718 2023-06-19 16:17:05.000000 bbfreport-2.0.1/bbfreport/plugins/examples/editTransform.py
+-rw-r--r--   0 william    (501) staff       (20)     4589 2023-06-27 12:28:54.000000 bbfreport-2.0.1/bbfreport/plugins/examples/enumTransform.py
+-rw-r--r--   0 william    (501) staff       (20)     6442 2023-06-27 12:28:54.000000 bbfreport-2.0.1/bbfreport/plugins/examples/pyxbParser.py
+-rw-r--r--   0 william    (501) staff       (20)     9829 2023-06-27 12:28:54.000000 bbfreport-2.0.1/bbfreport/plugins/examples/relrefTransform.py
+-rw-r--r--   0 william    (501) staff       (20)     2808 2023-06-27 12:28:54.000000 bbfreport-2.0.1/bbfreport/plugins/examples/statusTransform.py
+-rw-r--r--   0 william    (501) staff       (20)     8393 2023-06-27 12:28:54.000000 bbfreport-2.0.1/bbfreport/plugins/examples/versionTransform.py
+-rw-r--r--   0 william    (501) staff       (20)     3881 2023-06-27 12:28:54.000000 bbfreport-2.0.1/bbfreport/plugins/examples/xmltodictParser.py
+-rw-r--r--   0 william    (501) staff       (20)     8099 2023-06-19 16:17:05.000000 bbfreport-2.0.1/bbfreport/plugins/expatParser.py
+-rw-r--r--   0 william    (501) staff       (20)     2008 2023-06-19 16:17:54.000000 bbfreport-2.0.1/bbfreport/plugins/html.py
+-rw-r--r--   0 william    (501) staff       (20)    29464 2023-06-19 16:17:54.000000 bbfreport-2.0.1/bbfreport/plugins/lint.py
+-rw-r--r--   0 william    (501) staff       (20)    84585 2023-06-27 12:28:54.000000 bbfreport-2.0.1/bbfreport/plugins/markdown.py
+-rw-r--r--   0 william    (501) staff       (20)     1934 2023-06-19 16:17:54.000000 bbfreport-2.0.1/bbfreport/plugins/null.py
+-rw-r--r--   0 william    (501) staff       (20)     3379 2023-06-19 16:17:05.000000 bbfreport-2.0.1/bbfreport/plugins/split.py
+-rw-r--r--   0 william    (501) staff       (20)    11955 2023-06-19 16:17:54.000000 bbfreport-2.0.1/bbfreport/plugins/textFormat.py
+-rw-r--r--   0 william    (501) staff       (20)     4789 2023-06-19 16:17:54.000000 bbfreport-2.0.1/bbfreport/plugins/used.py
+-rw-r--r--   0 william    (501) staff       (20)    22310 2023-06-19 16:17:54.000000 bbfreport-2.0.1/bbfreport/plugins/xmlFormat.py
+-rw-r--r--   0 william    (501) staff       (20)    69903 2023-06-19 16:17:54.000000 bbfreport-2.0.1/bbfreport/property.py
+-rw-r--r--   0 william    (501) staff       (20)     2218 2023-06-19 16:17:05.000000 bbfreport-2.0.1/bbfreport/transform.py
+-rw-r--r--   0 william    (501) staff       (20)    29888 2023-06-19 16:17:54.000000 bbfreport-2.0.1/bbfreport/utility.py
+-rw-r--r--   0 william    (501) staff       (20)    35865 2023-06-19 16:17:54.000000 bbfreport-2.0.1/bbfreport/visitor.py
+drwxr-xr-x   0 william    (501) staff       (20)        0 2023-06-27 14:29:59.404779 bbfreport-2.0.1/bbfreport.egg-info/
+-rw-r--r--   0 william    (501) staff       (20)     7233 2023-06-27 14:29:59.000000 bbfreport-2.0.1/bbfreport.egg-info/PKG-INFO
+-rw-r--r--   0 william    (501) staff       (20)     1317 2023-06-27 14:29:59.000000 bbfreport-2.0.1/bbfreport.egg-info/SOURCES.txt
+-rw-r--r--   0 william    (501) staff       (20)        1 2023-06-27 14:29:59.000000 bbfreport-2.0.1/bbfreport.egg-info/dependency_links.txt
+-rw-r--r--   0 william    (501) staff       (20)       10 2023-06-27 14:29:59.000000 bbfreport-2.0.1/bbfreport.egg-info/top_level.txt
+drwxr-xr-x   0 william    (501) staff       (20)        0 2023-06-27 14:29:59.413195 bbfreport-2.0.1/bin/
+-rwxr-xr-x   0 william    (501) staff       (20)    18358 2023-06-27 12:28:54.000000 bbfreport-2.0.1/bin/report.py
+-rw-r--r--   0 william    (501) staff       (20)      808 2023-06-19 16:25:23.000000 bbfreport-2.0.1/pyproject.toml
+-rw-r--r--   0 william    (501) staff       (20)       38 2023-06-27 14:29:59.413736 bbfreport-2.0.1/setup.cfg
```

### Comparing `bbfreport-2.0/LICENSE` & `bbfreport-2.0.1/LICENSE`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (c) 2019, Broadband Forum
+Copyright (c) 2019-2023, Broadband Forum
 
 Redistribution and use in source and binary forms, with or
 without modification, are permitted provided that the following
 conditions are met:
 
 1. Redistributions of source code must retain the above copyright
    notice, this list of conditions and the following disclaimer.
```

### Comparing `bbfreport-2.0/PKG-INFO` & `bbfreport-2.0.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,33 +1,49 @@
 Metadata-Version: 2.1
 Name: bbfreport
-Version: 2.0
+Version: 2.0.1
 Summary: Broadband Forum (BBF) Data Model Report Tool
 Author-email: William Lupton <wlupton@broadband-forum.org>
 Project-URL: Homepage, https://github.com/BroadbandForum/bbfreport
 Project-URL: Bug Tracker, https://github.com/BroadbandForum/bbfreport/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
+<!-- do not edit! this file was created from PROJECT.yaml by project-parser.py -->
+
 # Broadband Forum (BBF) Data Model Report Tool
 
-Detailed documentation will be added in a future release. In the meantime, see below for
-command-line help.
+The BBF Report Tool processes one or more Data Model (DM) XML files. Having
+read the files, it always performs various "lint" checks and then it
+optionally generates an output format, e.g., "full" XML (a single file in
+which all imports have been resolved) or markdown (which can be converted to
+HTML by [pandoc]).
+
+The tool requires at least python 3.9, and can be installed from [PyPI]. It
+replaces an earlier [report.pl] tool.
+
+[pandoc]: https://pandoc.org
+[PyPI]: https://pypi.org/search/?q=bbfreport
+[report.pl]: https://github.com/BroadbandForum/cwmp-xml-tools
+
+Detailed documentation will be added in a future release. In the meantime,
+see below for command-line help.
 
-Note that the command-line help doesn't yet show help for `<transform>.py` and `<format>.py`
-plugins. You can also (for example) supply:
+Note that the command-line help doesn't yet show help for `<transform>.py`
+and `<format>.py` plugins. You can also (for example) supply:
 
 * `-t diff` (with two DM files) to generate diffs, or
 
-* `-f markdown` to generate [pandoc](https://pandoc.org) `commonmark_x` markdown that can then
-be converted to HTML. Direct HTML generation will be added in a future release
+* `-f markdown` to generate [pandoc](https://pandoc.org) `commonmark_x`
+  markdown that can then be converted to HTML. Direct HTML generation will
+  be added in a future release
 
 ```shell
 usage: report.py [-P PLUGINDIR] [-I INCLUDE] [-C] [-F FILTER] [-o OUTPUT]
                  [-l {none,fatal,error,warning,info,debug,0,1,2}]
                  [-L LOGGERNAME] [-T] [-A] [-S] [-D DEBUGPATH] [--profile]
                  [--parser-dump-json] [--parser-dump-tuple]
                  [--parser-warn-tabs]
```

### Comparing `bbfreport-2.0/README.md` & `bbfreport-2.0.1/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,35 @@
+<!-- do not edit! this file was created from PROJECT.yaml by project-parser.py -->
+
 # Broadband Forum (BBF) Data Model Report Tool
 
-Detailed documentation will be added in a future release. In the meantime, see below for
-command-line help.
+The BBF Report Tool processes one or more Data Model (DM) XML files. Having
+read the files, it always performs various "lint" checks and then it
+optionally generates an output format, e.g., "full" XML (a single file in
+which all imports have been resolved) or markdown (which can be converted to
+HTML by [pandoc]).
+
+The tool requires at least python 3.9, and can be installed from [PyPI]. It
+replaces an earlier [report.pl] tool.
+
+[pandoc]: https://pandoc.org
+[PyPI]: https://pypi.org/search/?q=bbfreport
+[report.pl]: https://github.com/BroadbandForum/cwmp-xml-tools
+
+Detailed documentation will be added in a future release. In the meantime,
+see below for command-line help.
 
-Note that the command-line help doesn't yet show help for `<transform>.py` and `<format>.py`
-plugins. You can also (for example) supply:
+Note that the command-line help doesn't yet show help for `<transform>.py`
+and `<format>.py` plugins. You can also (for example) supply:
 
 * `-t diff` (with two DM files) to generate diffs, or
 
-* `-f markdown` to generate [pandoc](https://pandoc.org) `commonmark_x` markdown that can then
-be converted to HTML. Direct HTML generation will be added in a future release
+* `-f markdown` to generate [pandoc](https://pandoc.org) `commonmark_x`
+  markdown that can then be converted to HTML. Direct HTML generation will
+  be added in a future release
 
 ```shell
 usage: report.py [-P PLUGINDIR] [-I INCLUDE] [-C] [-F FILTER] [-o OUTPUT]
                  [-l {none,fatal,error,warning,info,debug,0,1,2}]
                  [-L LOGGERNAME] [-T] [-A] [-S] [-D DEBUGPATH] [--profile]
                  [--parser-dump-json] [--parser-dump-tuple]
                  [--parser-warn-tabs]
```

### Comparing `bbfreport-2.0/bbfreport/__init__.py` & `bbfreport-2.0.1/bbfreport/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -39,16 +39,33 @@
 #
 # Any moral rights which are necessary to exercise under the above
 # license grant are also deemed granted under this license.
 
 # XXX should add more info here, but avoid duplication with setup.py
 # XXX is it OK to invent new dunder names such as __tool_name__?
 __tool_name__ = 'report.py'
-__version__ = '2.0'  # trailing '+' means 'interim version'
-__version_date__ = '2023-06-14'
+__version__ = '2.0.1'  # trailing '+' means 'interim version'
+__version_date__ = '2023-06-27'
+
+
+# use this when reporting the version
+def version(*, as_markdown: bool = False) -> str:
+    # derive the PyPI package name and URL
+    pypi_package = __package__.split('.')[0]
+    pypi_url = 'https://pypi.org/project/%s' % pypi_package
+
+    # if requested, convert to markdown
+    bbf, package = 'Broadband Forum', pypi_package
+    if as_markdown:
+        bbf = '[%s](https://www.broadband-forum.org)' % bbf
+        package = '[%s](%s)' % (pypi_package, pypi_url)
+
+    return '%s %s v%s (%s version)' % (bbf, package,
+                                       __version__, __version_date__)
+
 
 from .content import Content
 from .exception import BBFReportException
 from .format import Format
 from .macro import Macro
 from .macros import DummyMacros
 # XXX it's hard to know which node types to import; perhaps the main "public"
```

### Comparing `bbfreport-2.0/bbfreport/content.py` & `bbfreport-2.0.1/bbfreport/content.py`

 * *Files identical despite different names*

### Comparing `bbfreport-2.0/bbfreport/exception.py` & `bbfreport-2.0.1/bbfreport/exception.py`

 * *Files identical despite different names*

### Comparing `bbfreport-2.0/bbfreport/file.py` & `bbfreport-2.0.1/bbfreport/file.py`

 * *Files identical despite different names*

### Comparing `bbfreport-2.0/bbfreport/format.py` & `bbfreport-2.0.1/bbfreport/format.py`

 * *Files identical despite different names*

### Comparing `bbfreport-2.0/bbfreport/macro.py` & `bbfreport-2.0.1/bbfreport/macro.py`

 * *Files identical despite different names*

### Comparing `bbfreport-2.0/bbfreport/macros/__init__.py` & `bbfreport-2.0.1/bbfreport/macros/__init__.py`

 * *Files identical despite different names*

### Comparing `bbfreport-2.0/bbfreport/macros/macros.py` & `bbfreport-2.0.1/bbfreport/macros/macros.py`

 * *Files identical despite different names*

### Comparing `bbfreport-2.0/bbfreport/node.py` & `bbfreport-2.0.1/bbfreport/node.py`

 * *Files identical despite different names*

### Comparing `bbfreport-2.0/bbfreport/parser.py` & `bbfreport-2.0.1/bbfreport/parser.py`

 * *Files identical despite different names*

### Comparing `bbfreport-2.0/bbfreport/path.py` & `bbfreport-2.0.1/bbfreport/path.py`

 * *Files identical despite different names*

### Comparing `bbfreport-2.0/bbfreport/plugin.py` & `bbfreport-2.0.1/bbfreport/plugin.py`

 * *Files identical despite different names*

### Comparing `bbfreport-2.0/bbfreport/plugins/__init__.py` & `bbfreport-2.0.1/bbfreport/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `bbfreport-2.0/bbfreport/plugins/automodel.py` & `bbfreport-2.0.1/bbfreport/plugins/automodel.py`

 * *Files identical despite different names*

### Comparing `bbfreport-2.0/bbfreport/plugins/depend.py` & `bbfreport-2.0.1/bbfreport/plugins/depend.py`

 * *Files identical despite different names*

### Comparing `bbfreport-2.0/bbfreport/plugins/diff.py` & `bbfreport-2.0.1/bbfreport/plugins/diff.py`

 * *Files identical despite different names*

### Comparing `bbfreport-2.0/bbfreport/plugins/enumTransform.py` & `bbfreport-2.0.1/bbfreport/plugins/examples/enumTransform.py`

 * *Files identical despite different names*

### Comparing `bbfreport-2.0/bbfreport/plugins/examples/candenyTransform.py` & `bbfreport-2.0.1/bbfreport/plugins/examples/candenyTransform.py`

 * *Files identical despite different names*

### Comparing `bbfreport-2.0/bbfreport/plugins/examples/editTransform.py` & `bbfreport-2.0.1/bbfreport/plugins/examples/editTransform.py`

 * *Files identical despite different names*

### Comparing `bbfreport-2.0/bbfreport/plugins/expatParser.py` & `bbfreport-2.0.1/bbfreport/plugins/expatParser.py`

 * *Files identical despite different names*

### Comparing `bbfreport-2.0/bbfreport/plugins/html.py` & `bbfreport-2.0.1/bbfreport/plugins/html.py`

 * *Files identical despite different names*

### Comparing `bbfreport-2.0/bbfreport/plugins/lint.py` & `bbfreport-2.0.1/bbfreport/plugins/lint.py`

 * *Files identical despite different names*

### Comparing `bbfreport-2.0/bbfreport/plugins/markdown.py` & `bbfreport-2.0.1/bbfreport/plugins/markdown.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,20 +44,19 @@
 import re
 import textwrap
 import time
 
 from io import TextIOBase
 from typing import Callable, cast, List, Optional, Tuple, Union
 
-from .. import __tool_name__, __version__, __version_date__
+from .. import __tool_name__, __version__, version
 from ..macro import Macro, MacroArg, MacroException, MacroRef
 from ..node import AbbreviationsItem, Command, CommandRef, DataTypeAccessor, \
     Event, EventRef, GlossaryItem, Input, Model, Node, Object, ObjectRef, \
-    Output, Parameter, ParameterRef, Profile, Reference, ReferenceHyperlink, \
-    Root
+    Output, Parameter, ParameterRef, Profile, Reference, Root
 from ..path import Path
 from ..utility import Status, Utility
 
 # XXX could try to generate sensible output when --thisonly is specified
 
 # XXX could try to generate sensible output when multiple files are specified
 
@@ -672,36 +671,27 @@
                         for val in value:
                             prefix = '--%s ' % name if name not in positional \
                                 else ''
                             args.append('%s%s' % (prefix, val))
 
             return ' '.join(args)
 
-        # it never hurts to link to the BBF website
-        bbf_url = 'https://www.broadband-forum.org'
-
-        # derive the PyPI package name and URL
-        pypi_package = __package__.split('.')[0]
-        pypi_url = 'https://pypi.org/project/%s' % pypi_package
-
         # use UTC dates and times
         now = time.gmtime()
         now_date = time.strftime('%Y-%m-%d', now)
         now_time = time.strftime('%H:%M:%S', now)
 
         # version numbers ending in '+' are later interim versions
         extra = ' (INTERIM VERSION)' if __version__.endswith('+') else ''
 
         self.print('''
             ---
 
-            Generated by [Broadband Forum](%s) [%s](%s) v%s (%s version) on %s 
-            at %s UTC%s.\\
-            %s %s''' % (bbf_url, pypi_package, pypi_url, __version__,
-                        __version_date__, now_date, now_time, extra,
+            Generated by %s on %s at %s UTC%s.\\
+            %s %s''' % (version(as_markdown=True), now_date, now_time, extra,
                         __tool_name__, args_string()))
 
     def output_header(self, level: int, text: str, anchor: str = '', *,
                       stat: str = 'current', notoc: bool = False,
                       **kwargs) -> None:
         stat_ = ' [%s]' % stat.upper() if stat != 'current' else ''
         target = ' {#%s}' % anchor if anchor else ''
```

### Comparing `bbfreport-2.0/bbfreport/plugins/null.py` & `bbfreport-2.0.1/bbfreport/plugins/null.py`

 * *Files identical despite different names*

### Comparing `bbfreport-2.0/bbfreport/plugins/pyxbParser.py` & `bbfreport-2.0.1/bbfreport/plugins/examples/pyxbParser.py`

 * *Files identical despite different names*

### Comparing `bbfreport-2.0/bbfreport/plugins/relrefTransform.py` & `bbfreport-2.0.1/bbfreport/plugins/examples/relrefTransform.py`

 * *Files identical despite different names*

### Comparing `bbfreport-2.0/bbfreport/plugins/split.py` & `bbfreport-2.0.1/bbfreport/plugins/split.py`

 * *Files identical despite different names*

### Comparing `bbfreport-2.0/bbfreport/plugins/statusTransform.py` & `bbfreport-2.0.1/bbfreport/plugins/examples/statusTransform.py`

 * *Files identical despite different names*

### Comparing `bbfreport-2.0/bbfreport/plugins/textFormat.py` & `bbfreport-2.0.1/bbfreport/plugins/textFormat.py`

 * *Files identical despite different names*

### Comparing `bbfreport-2.0/bbfreport/plugins/used.py` & `bbfreport-2.0.1/bbfreport/plugins/used.py`

 * *Files identical despite different names*

### Comparing `bbfreport-2.0/bbfreport/plugins/versionTransform.py` & `bbfreport-2.0.1/bbfreport/plugins/examples/versionTransform.py`

 * *Files identical despite different names*

### Comparing `bbfreport-2.0/bbfreport/plugins/xmlFormat.py` & `bbfreport-2.0.1/bbfreport/plugins/xmlFormat.py`

 * *Files identical despite different names*

### Comparing `bbfreport-2.0/bbfreport/plugins/xmltodictParser.py` & `bbfreport-2.0.1/bbfreport/plugins/examples/xmltodictParser.py`

 * *Files identical despite different names*

### Comparing `bbfreport-2.0/bbfreport/property.py` & `bbfreport-2.0.1/bbfreport/property.py`

 * *Files identical despite different names*

### Comparing `bbfreport-2.0/bbfreport/transform.py` & `bbfreport-2.0.1/bbfreport/transform.py`

 * *Files identical despite different names*

### Comparing `bbfreport-2.0/bbfreport/utility.py` & `bbfreport-2.0.1/bbfreport/utility.py`

 * *Files identical despite different names*

### Comparing `bbfreport-2.0/bbfreport/visitor.py` & `bbfreport-2.0.1/bbfreport/visitor.py`

 * *Files identical despite different names*

### Comparing `bbfreport-2.0/bbfreport.egg-info/PKG-INFO` & `bbfreport-2.0.1/bbfreport.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,33 +1,49 @@
 Metadata-Version: 2.1
 Name: bbfreport
-Version: 2.0
+Version: 2.0.1
 Summary: Broadband Forum (BBF) Data Model Report Tool
 Author-email: William Lupton <wlupton@broadband-forum.org>
 Project-URL: Homepage, https://github.com/BroadbandForum/bbfreport
 Project-URL: Bug Tracker, https://github.com/BroadbandForum/bbfreport/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
+<!-- do not edit! this file was created from PROJECT.yaml by project-parser.py -->
+
 # Broadband Forum (BBF) Data Model Report Tool
 
-Detailed documentation will be added in a future release. In the meantime, see below for
-command-line help.
+The BBF Report Tool processes one or more Data Model (DM) XML files. Having
+read the files, it always performs various "lint" checks and then it
+optionally generates an output format, e.g., "full" XML (a single file in
+which all imports have been resolved) or markdown (which can be converted to
+HTML by [pandoc]).
+
+The tool requires at least python 3.9, and can be installed from [PyPI]. It
+replaces an earlier [report.pl] tool.
+
+[pandoc]: https://pandoc.org
+[PyPI]: https://pypi.org/search/?q=bbfreport
+[report.pl]: https://github.com/BroadbandForum/cwmp-xml-tools
+
+Detailed documentation will be added in a future release. In the meantime,
+see below for command-line help.
 
-Note that the command-line help doesn't yet show help for `<transform>.py` and `<format>.py`
-plugins. You can also (for example) supply:
+Note that the command-line help doesn't yet show help for `<transform>.py`
+and `<format>.py` plugins. You can also (for example) supply:
 
 * `-t diff` (with two DM files) to generate diffs, or
 
-* `-f markdown` to generate [pandoc](https://pandoc.org) `commonmark_x` markdown that can then
-be converted to HTML. Direct HTML generation will be added in a future release
+* `-f markdown` to generate [pandoc](https://pandoc.org) `commonmark_x`
+  markdown that can then be converted to HTML. Direct HTML generation will
+  be added in a future release
 
 ```shell
 usage: report.py [-P PLUGINDIR] [-I INCLUDE] [-C] [-F FILTER] [-o OUTPUT]
                  [-l {none,fatal,error,warning,info,debug,0,1,2}]
                  [-L LOGGERNAME] [-T] [-A] [-S] [-D DEBUGPATH] [--profile]
                  [--parser-dump-json] [--parser-dump-tuple]
                  [--parser-warn-tabs]
```

### Comparing `bbfreport-2.0/bbfreport.egg-info/SOURCES.txt` & `bbfreport-2.0.1/bbfreport.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -22,26 +22,26 @@
 bbfreport/macros/__init__.py
 bbfreport/macros/macros.py
 bbfreport/macros/test.py
 bbfreport/plugins/__init__.py
 bbfreport/plugins/automodel.py
 bbfreport/plugins/depend.py
 bbfreport/plugins/diff.py
-bbfreport/plugins/enumTransform.py
 bbfreport/plugins/expatParser.py
 bbfreport/plugins/html.py
 bbfreport/plugins/lint.py
 bbfreport/plugins/markdown.py
 bbfreport/plugins/null.py
-bbfreport/plugins/pyxbParser.py
-bbfreport/plugins/relrefTransform.py
 bbfreport/plugins/split.py
-bbfreport/plugins/statusTransform.py
 bbfreport/plugins/textFormat.py
 bbfreport/plugins/used.py
-bbfreport/plugins/versionTransform.py
 bbfreport/plugins/xmlFormat.py
-bbfreport/plugins/xmltodictParser.py
 bbfreport/plugins/examples/__init__.py
 bbfreport/plugins/examples/candenyTransform.py
 bbfreport/plugins/examples/editTransform.py
+bbfreport/plugins/examples/enumTransform.py
+bbfreport/plugins/examples/pyxbParser.py
+bbfreport/plugins/examples/relrefTransform.py
+bbfreport/plugins/examples/statusTransform.py
+bbfreport/plugins/examples/versionTransform.py
+bbfreport/plugins/examples/xmltodictParser.py
 bin/report.py
```

### Comparing `bbfreport-2.0/bin/report.py` & `bbfreport-2.0.1/bin/report.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,15 +80,15 @@
                                                MIN_VERSION)
 
 # if the bbfreport package is not installed, insert the current working
 # directory into the search path, so we can directly execute the tool from
 # the code
 try:
     from bbfreport import BBFReportException, Format, Null, Parser, Plugin, \
-        Root, Transform, Utility
+        Root, Transform, Utility, version
 except ModuleNotFoundError:
     sys.path.insert(0, os.getcwd())
     from bbfreport import BBFReportException, Format, Null, Parser, Plugin, \
         Root, Transform, Utility
 
 nice_list = Utility.nice_list
 
@@ -284,17 +284,19 @@
                             help="optional transforms to apply to node tree; "
                                  "choices: {%s}" % ','.join(transform_names))
     arg_parser.add_argument("-f", "--format", type=format_create,
                             default=default_format,
                             help="report format to generate; choices: {%s}; "
                                  "default: %r" % (
                                      ','.join(format_names), default_format))
-    arg_parser.add_argument('-h', '--help', action='help',
+    arg_parser.add_argument("-v", "--version", action="store_true",
+                            help="show the version number and exit")
+    arg_parser.add_argument("-h", "--help", action="help",
                             default=argparse.SUPPRESS,
-                            help='show this help message and exit')
+                            help="show this help message and exit")
     arg_parser.add_argument("file", type=str, nargs="*",
                             help="DM files to process")
 
     # 'before' and 'after' transforms
     # XXX there should be a more general list of 'before' and 'after' xforms
     # XXX there should be a way of suppressing the 'used' and/or 'lint'
     #     transforms; or use the log level?
@@ -320,14 +322,18 @@
     arg_parser = get_argparser(argv=argv, opts=opts)
 
     # parse remaining arguments
     argv_remaining = opts.get('argv_remaining', None)
     namespace = opts.get('namespace', None)
     args = arg_parser.parse_args(argv_remaining, namespace=namespace)
 
+    # handle --version
+    if args.version:
+        sys.stderr.write('%s\n' % version())
+
     # get the list of transforms
     transforms = opts.get('transforms_before', []) + \
         (args.transform or []) + opts.get('transforms_after', [])
 
     # rename a few arguments
     # XXX could use 'dest' but that shows up in the command line help
     args.dirs = args.include
```

### Comparing `bbfreport-2.0/pyproject.toml` & `bbfreport-2.0.1/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "bbfreport"
-version = "2.0"
+dynamic = ["version"]
 authors = [
   {name = "William Lupton", email = "wlupton@broadband-forum.org"}
 ]
 description = "Broadband Forum (BBF) Data Model Report Tool"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
@@ -20,10 +20,13 @@
 [project.urls]
 "Homepage" = "https://github.com/BroadbandForum/bbfreport"
 "Bug Tracker" = "https://github.com/BroadbandForum/bbfreport/issues"
 
 [tool.setuptools]
 script-files = ["bin/report.py"]
 
+[tool.setuptools.dynamic]
+version = {attr = "bbfreport.__version__"}
+
 [tool.setuptools.packages.find]
 where = ["."]
 include = ["bbfreport*"]
```

