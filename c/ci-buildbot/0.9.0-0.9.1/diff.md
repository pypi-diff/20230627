# Comparing `tmp/ci-buildbot-0.9.0.tar.gz` & `tmp/ci-buildbot-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ci-buildbot-0.9.0.tar", last modified: Mon Jun 26 17:24:19 2023, max compression
+gzip compressed data, was "dist/ci-buildbot-0.9.1.tar", last modified: Tue Jun 27 17:51:27 2023, max compression
```

## Comparing `ci-buildbot-0.9.0.tar` & `ci-buildbot-0.9.1.tar`

### file list

```diff
@@ -1,63 +1,62 @@
-drwxrwxr-x   0 cmalek     (501) staff       (20)        0 2023-06-26 17:24:19.000000 ci-buildbot-0.9.0/
--rw-rw-r--   0 cmalek     (501) staff       (20)      100 2020-06-03 23:17:09.000000 ci-buildbot-0.9.0/MANIFEST.in
--rw-rw-r--   0 cmalek     (501) staff       (20)     3588 2023-06-26 17:24:19.000000 ci-buildbot-0.9.0/PKG-INFO
--rw-rw-r--   0 cmalek     (501) staff       (20)     2660 2022-08-12 23:28:44.000000 ci-buildbot-0.9.0/README.md
-drwxrwxr-x   0 cmalek     (501) staff       (20)        0 2023-06-26 17:24:19.000000 ci-buildbot-0.9.0/ci_buildbot/
--rw-rw-r--   0 cmalek     (501) staff       (20)       22 2023-06-26 17:23:45.000000 ci-buildbot-0.9.0/ci_buildbot/__init__.py
--rw-rw-r--   0 cmalek     (501) staff       (20)    12633 2023-06-26 17:23:34.000000 ci-buildbot-0.9.0/ci_buildbot/cli.py
-drwxrwxr-x   0 cmalek     (501) staff       (20)        0 2023-06-26 17:24:19.000000 ci-buildbot-0.9.0/ci_buildbot/context_processors/
--rw-rw-r--   0 cmalek     (501) staff       (20)      366 2023-06-26 17:23:34.000000 ci-buildbot-0.9.0/ci_buildbot/context_processors/__init__.py
--rw-rw-r--   0 cmalek     (501) staff       (20)      564 2023-06-26 17:23:34.000000 ci-buildbot-0.9.0/ci_buildbot/context_processors/base.py
--rw-rw-r--   0 cmalek     (501) staff       (20)     3092 2023-06-26 17:23:34.000000 ci-buildbot-0.9.0/ci_buildbot/context_processors/codebuild.py
--rw-rw-r--   0 cmalek     (501) staff       (20)      881 2023-06-26 17:23:34.000000 ci-buildbot-0.9.0/ci_buildbot/context_processors/deployfish.py
--rw-rw-r--   0 cmalek     (501) staff       (20)     1144 2023-06-26 17:23:34.000000 ci-buildbot-0.9.0/ci_buildbot/context_processors/docker.py
--rw-rw-r--   0 cmalek     (501) staff       (20)      489 2023-06-26 17:23:34.000000 ci-buildbot-0.9.0/ci_buildbot/context_processors/generic.py
--rw-rw-r--   0 cmalek     (501) staff       (20)     9516 2023-06-26 17:23:34.000000 ci-buildbot-0.9.0/ci_buildbot/context_processors/git.py
--rw-rw-r--   0 cmalek     (501) staff       (20)     1773 2023-06-26 17:23:34.000000 ci-buildbot-0.9.0/ci_buildbot/context_processors/project.py
--rw-rw-r--   0 cmalek     (501) staff       (20)      617 2023-06-26 17:23:34.000000 ci-buildbot-0.9.0/ci_buildbot/context_processors/sphinx.py
--rw-rw-r--   0 cmalek     (501) staff       (20)     1477 2023-06-26 17:23:34.000000 ci-buildbot-0.9.0/ci_buildbot/context_processors/unittest.py
--rw-rw-r--   0 cmalek     (501) staff       (20)      116 2023-06-26 17:23:34.000000 ci-buildbot-0.9.0/ci_buildbot/exc.py
-drwxrwxr-x   0 cmalek     (501) staff       (20)        0 2023-06-26 17:24:19.000000 ci-buildbot-0.9.0/ci_buildbot/messages/
--rw-rw-r--   0 cmalek     (501) staff       (20)      833 2023-06-26 17:23:34.000000 ci-buildbot-0.9.0/ci_buildbot/messages/__init__.py
--rw-rw-r--   0 cmalek     (501) staff       (20)      467 2023-06-26 17:23:34.000000 ci-buildbot-0.9.0/ci_buildbot/messages/archive.py
--rw-rw-r--   0 cmalek     (501) staff       (20)     2007 2023-06-26 17:23:34.000000 ci-buildbot-0.9.0/ci_buildbot/messages/base.py
--rw-rw-r--   0 cmalek     (501) staff       (20)     1116 2023-06-26 17:23:34.000000 ci-buildbot-0.9.0/ci_buildbot/messages/deployfish.py
--rw-rw-r--   0 cmalek     (501) staff       (20)     1165 2023-06-26 17:23:34.000000 ci-buildbot-0.9.0/ci_buildbot/messages/deployfish_tasks.py
--rw-rw-r--   0 cmalek     (501) staff       (20)     1109 2023-06-26 17:23:34.000000 ci-buildbot-0.9.0/ci_buildbot/messages/docker.py
--rw-rw-r--   0 cmalek     (501) staff       (20)     1008 2023-06-26 17:23:34.000000 ci-buildbot-0.9.0/ci_buildbot/messages/docs.py
--rw-rw-r--   0 cmalek     (501) staff       (20)      798 2023-06-26 17:23:34.000000 ci-buildbot-0.9.0/ci_buildbot/messages/general.py
--rw-rw-r--   0 cmalek     (501) staff       (20)      817 2023-06-26 17:23:34.000000 ci-buildbot-0.9.0/ci_buildbot/messages/unittests.py
--rw-rw-r--   0 cmalek     (501) staff       (20)      834 2023-06-26 17:23:34.000000 ci-buildbot-0.9.0/ci_buildbot/settings.py
-drwxrwxr-x   0 cmalek     (501) staff       (20)        0 2023-06-26 17:24:19.000000 ci-buildbot-0.9.0/ci_buildbot/templates/
--rw-rw-r--   0 cmalek     (501) staff       (20)      949 2020-06-04 00:25:48.000000 ci-buildbot-0.9.0/ci_buildbot/templates/archive.tpl
--rw-rw-r--   0 cmalek     (501) staff       (20)      653 2020-07-15 23:30:13.000000 ci-buildbot-0.9.0/ci_buildbot/templates/deploy_failed.tpl
--rw-rw-r--   0 cmalek     (501) staff       (20)      609 2020-06-04 00:52:42.000000 ci-buildbot-0.9.0/ci_buildbot/templates/deploy_start.tpl
--rw-rw-r--   0 cmalek     (501) staff       (20)      656 2020-07-15 23:30:01.000000 ci-buildbot-0.9.0/ci_buildbot/templates/deploy_success.tpl
--rw-rw-r--   0 cmalek     (501) staff       (20)      672 2020-07-16 17:06:32.000000 ci-buildbot-0.9.0/ci_buildbot/templates/deploy_tasks_failed.tpl
--rw-rw-r--   0 cmalek     (501) staff       (20)      636 2020-07-16 17:06:29.000000 ci-buildbot-0.9.0/ci_buildbot/templates/deploy_tasks_start.tpl
--rw-rw-r--   0 cmalek     (501) staff       (20)      673 2020-07-16 17:06:23.000000 ci-buildbot-0.9.0/ci_buildbot/templates/deploy_tasks_success.tpl
--rw-rw-r--   0 cmalek     (501) staff       (20)      674 2020-07-15 23:31:55.000000 ci-buildbot-0.9.0/ci_buildbot/templates/docker_failed.tpl
--rw-rw-r--   0 cmalek     (501) staff       (20)      635 2020-07-15 23:32:00.000000 ci-buildbot-0.9.0/ci_buildbot/templates/docker_start.tpl
--rw-rw-r--   0 cmalek     (501) staff       (20)      726 2020-07-15 23:30:24.000000 ci-buildbot-0.9.0/ci_buildbot/templates/docker_success.tpl
--rw-rw-r--   0 cmalek     (501) staff       (20)      623 2023-06-26 17:23:34.000000 ci-buildbot-0.9.0/ci_buildbot/templates/docs_failed.tpl
--rw-rw-r--   0 cmalek     (501) staff       (20)      584 2023-06-26 17:23:34.000000 ci-buildbot-0.9.0/ci_buildbot/templates/docs_start.tpl
--rw-rw-r--   0 cmalek     (501) staff       (20)      649 2023-06-26 17:23:34.000000 ci-buildbot-0.9.0/ci_buildbot/templates/docs_success.tpl
--rw-rw-r--   0 cmalek     (501) staff       (20)      627 2023-06-26 17:23:34.000000 ci-buildbot-0.9.0/ci_buildbot/templates/general_failed.tpl
--rw-rw-r--   0 cmalek     (501) staff       (20)      592 2020-09-15 21:58:53.000000 ci-buildbot-0.9.0/ci_buildbot/templates/general_start.tpl
--rw-rw-r--   0 cmalek     (501) staff       (20)      628 2023-06-26 17:23:34.000000 ci-buildbot-0.9.0/ci_buildbot/templates/general_success.tpl
--rw-rw-r--   0 cmalek     (501) staff       (20)      667 2021-01-07 23:14:54.000000 ci-buildbot-0.9.0/ci_buildbot/templates/unittests_failed.tpl
--rw-rw-r--   0 cmalek     (501) staff       (20)      597 2021-01-07 00:11:19.000000 ci-buildbot-0.9.0/ci_buildbot/templates/unittests_start.tpl
--rw-rw-r--   0 cmalek     (501) staff       (20)      669 2021-01-07 23:15:01.000000 ci-buildbot-0.9.0/ci_buildbot/templates/unittests_success.tpl
--rw-rw-r--   0 cmalek     (501) staff       (20)       63 2023-06-26 17:23:34.000000 ci-buildbot-0.9.0/ci_buildbot/typedefs.py
-drwxrwxr-x   0 cmalek     (501) staff       (20)        0 2023-06-26 17:24:19.000000 ci-buildbot-0.9.0/ci_buildbot.egg-info/
--rw-rw-r--   0 cmalek     (501) staff       (20)     3588 2023-06-26 17:24:19.000000 ci-buildbot-0.9.0/ci_buildbot.egg-info/PKG-INFO
--rw-rw-r--   0 cmalek     (501) staff       (20)     1891 2023-06-26 17:24:19.000000 ci-buildbot-0.9.0/ci_buildbot.egg-info/SOURCES.txt
--rw-rw-r--   0 cmalek     (501) staff       (20)        1 2023-06-26 17:24:19.000000 ci-buildbot-0.9.0/ci_buildbot.egg-info/dependency_links.txt
--rw-rw-r--   0 cmalek     (501) staff       (20)       51 2023-06-26 17:24:19.000000 ci-buildbot-0.9.0/ci_buildbot.egg-info/entry_points.txt
--rw-rw-r--   0 cmalek     (501) staff       (20)      135 2023-06-26 17:24:19.000000 ci-buildbot-0.9.0/ci_buildbot.egg-info/requires.txt
--rw-rw-r--   0 cmalek     (501) staff       (20)       12 2023-06-26 17:24:19.000000 ci-buildbot-0.9.0/ci_buildbot.egg-info/top_level.txt
-drwxrwxr-x   0 cmalek     (501) staff       (20)        0 2023-06-26 17:24:19.000000 ci-buildbot-0.9.0/etc/
--rw-rw-r--   0 cmalek     (501) staff       (20)      313 2020-06-03 21:28:58.000000 ci-buildbot-0.9.0/etc/environment.txt
--rw-rw-r--   0 cmalek     (501) staff       (20)     2275 2023-06-26 17:23:34.000000 ci-buildbot-0.9.0/requirements.txt
--rw-rw-r--   0 cmalek     (501) staff       (20)      986 2023-06-26 17:24:19.000000 ci-buildbot-0.9.0/setup.cfg
--rw-rw-r--   0 cmalek     (501) staff       (20)     1040 2023-06-26 17:23:45.000000 ci-buildbot-0.9.0/setup.py
+drwxrwxr-x   0 cmalek     (501) staff       (20)        0 2023-06-27 17:51:27.000000 ci-buildbot-0.9.1/
+-rw-rw-r--   0 cmalek     (501) staff       (20)      100 2020-06-03 23:17:09.000000 ci-buildbot-0.9.1/MANIFEST.in
+-rw-rw-r--   0 cmalek     (501) staff       (20)     3588 2023-06-27 17:51:27.000000 ci-buildbot-0.9.1/PKG-INFO
+-rw-rw-r--   0 cmalek     (501) staff       (20)     2660 2022-08-12 23:28:44.000000 ci-buildbot-0.9.1/README.md
+drwxrwxr-x   0 cmalek     (501) staff       (20)        0 2023-06-27 17:51:27.000000 ci-buildbot-0.9.1/ci_buildbot/
+-rw-rw-r--   0 cmalek     (501) staff       (20)       22 2023-06-27 17:51:14.000000 ci-buildbot-0.9.1/ci_buildbot/__init__.py
+-rw-rw-r--   0 cmalek     (501) staff       (20)    12633 2023-06-26 17:23:34.000000 ci-buildbot-0.9.1/ci_buildbot/cli.py
+drwxrwxr-x   0 cmalek     (501) staff       (20)        0 2023-06-27 17:51:27.000000 ci-buildbot-0.9.1/ci_buildbot/context_processors/
+-rw-rw-r--   0 cmalek     (501) staff       (20)      326 2023-06-27 17:48:28.000000 ci-buildbot-0.9.1/ci_buildbot/context_processors/__init__.py
+-rw-rw-r--   0 cmalek     (501) staff       (20)      564 2023-06-26 17:23:34.000000 ci-buildbot-0.9.1/ci_buildbot/context_processors/base.py
+-rw-rw-r--   0 cmalek     (501) staff       (20)     3092 2023-06-26 17:23:34.000000 ci-buildbot-0.9.1/ci_buildbot/context_processors/codebuild.py
+-rw-rw-r--   0 cmalek     (501) staff       (20)      881 2023-06-26 17:23:34.000000 ci-buildbot-0.9.1/ci_buildbot/context_processors/deployfish.py
+-rw-rw-r--   0 cmalek     (501) staff       (20)     1144 2023-06-26 17:23:34.000000 ci-buildbot-0.9.1/ci_buildbot/context_processors/docker.py
+-rw-rw-r--   0 cmalek     (501) staff       (20)      489 2023-06-26 17:23:34.000000 ci-buildbot-0.9.1/ci_buildbot/context_processors/generic.py
+-rw-rw-r--   0 cmalek     (501) staff       (20)     9516 2023-06-26 17:23:34.000000 ci-buildbot-0.9.1/ci_buildbot/context_processors/git.py
+-rw-rw-r--   0 cmalek     (501) staff       (20)     1773 2023-06-26 17:23:34.000000 ci-buildbot-0.9.1/ci_buildbot/context_processors/project.py
+-rw-rw-r--   0 cmalek     (501) staff       (20)     1477 2023-06-26 17:23:34.000000 ci-buildbot-0.9.1/ci_buildbot/context_processors/unittest.py
+-rw-rw-r--   0 cmalek     (501) staff       (20)      116 2023-06-26 17:23:34.000000 ci-buildbot-0.9.1/ci_buildbot/exc.py
+drwxrwxr-x   0 cmalek     (501) staff       (20)        0 2023-06-27 17:51:27.000000 ci-buildbot-0.9.1/ci_buildbot/messages/
+-rw-rw-r--   0 cmalek     (501) staff       (20)      833 2023-06-26 17:23:34.000000 ci-buildbot-0.9.1/ci_buildbot/messages/__init__.py
+-rw-rw-r--   0 cmalek     (501) staff       (20)      467 2023-06-26 17:23:34.000000 ci-buildbot-0.9.1/ci_buildbot/messages/archive.py
+-rw-rw-r--   0 cmalek     (501) staff       (20)     2007 2023-06-26 17:23:34.000000 ci-buildbot-0.9.1/ci_buildbot/messages/base.py
+-rw-rw-r--   0 cmalek     (501) staff       (20)     1116 2023-06-26 17:23:34.000000 ci-buildbot-0.9.1/ci_buildbot/messages/deployfish.py
+-rw-rw-r--   0 cmalek     (501) staff       (20)     1165 2023-06-26 17:23:34.000000 ci-buildbot-0.9.1/ci_buildbot/messages/deployfish_tasks.py
+-rw-rw-r--   0 cmalek     (501) staff       (20)     1109 2023-06-26 17:23:34.000000 ci-buildbot-0.9.1/ci_buildbot/messages/docker.py
+-rw-rw-r--   0 cmalek     (501) staff       (20)      916 2023-06-27 17:48:48.000000 ci-buildbot-0.9.1/ci_buildbot/messages/docs.py
+-rw-rw-r--   0 cmalek     (501) staff       (20)      798 2023-06-26 17:23:34.000000 ci-buildbot-0.9.1/ci_buildbot/messages/general.py
+-rw-rw-r--   0 cmalek     (501) staff       (20)      817 2023-06-26 17:23:34.000000 ci-buildbot-0.9.1/ci_buildbot/messages/unittests.py
+-rw-rw-r--   0 cmalek     (501) staff       (20)      834 2023-06-26 17:23:34.000000 ci-buildbot-0.9.1/ci_buildbot/settings.py
+drwxrwxr-x   0 cmalek     (501) staff       (20)        0 2023-06-27 17:51:27.000000 ci-buildbot-0.9.1/ci_buildbot/templates/
+-rw-rw-r--   0 cmalek     (501) staff       (20)      949 2020-06-04 00:25:48.000000 ci-buildbot-0.9.1/ci_buildbot/templates/archive.tpl
+-rw-rw-r--   0 cmalek     (501) staff       (20)      653 2020-07-15 23:30:13.000000 ci-buildbot-0.9.1/ci_buildbot/templates/deploy_failed.tpl
+-rw-rw-r--   0 cmalek     (501) staff       (20)      609 2020-06-04 00:52:42.000000 ci-buildbot-0.9.1/ci_buildbot/templates/deploy_start.tpl
+-rw-rw-r--   0 cmalek     (501) staff       (20)      656 2020-07-15 23:30:01.000000 ci-buildbot-0.9.1/ci_buildbot/templates/deploy_success.tpl
+-rw-rw-r--   0 cmalek     (501) staff       (20)      672 2020-07-16 17:06:32.000000 ci-buildbot-0.9.1/ci_buildbot/templates/deploy_tasks_failed.tpl
+-rw-rw-r--   0 cmalek     (501) staff       (20)      636 2020-07-16 17:06:29.000000 ci-buildbot-0.9.1/ci_buildbot/templates/deploy_tasks_start.tpl
+-rw-rw-r--   0 cmalek     (501) staff       (20)      673 2020-07-16 17:06:23.000000 ci-buildbot-0.9.1/ci_buildbot/templates/deploy_tasks_success.tpl
+-rw-rw-r--   0 cmalek     (501) staff       (20)      674 2020-07-15 23:31:55.000000 ci-buildbot-0.9.1/ci_buildbot/templates/docker_failed.tpl
+-rw-rw-r--   0 cmalek     (501) staff       (20)      635 2020-07-15 23:32:00.000000 ci-buildbot-0.9.1/ci_buildbot/templates/docker_start.tpl
+-rw-rw-r--   0 cmalek     (501) staff       (20)      726 2020-07-15 23:30:24.000000 ci-buildbot-0.9.1/ci_buildbot/templates/docker_success.tpl
+-rw-rw-r--   0 cmalek     (501) staff       (20)      623 2023-06-26 17:23:34.000000 ci-buildbot-0.9.1/ci_buildbot/templates/docs_failed.tpl
+-rw-rw-r--   0 cmalek     (501) staff       (20)      584 2023-06-26 17:23:34.000000 ci-buildbot-0.9.1/ci_buildbot/templates/docs_start.tpl
+-rw-rw-r--   0 cmalek     (501) staff       (20)      649 2023-06-26 17:23:34.000000 ci-buildbot-0.9.1/ci_buildbot/templates/docs_success.tpl
+-rw-rw-r--   0 cmalek     (501) staff       (20)      627 2023-06-26 17:23:34.000000 ci-buildbot-0.9.1/ci_buildbot/templates/general_failed.tpl
+-rw-rw-r--   0 cmalek     (501) staff       (20)      592 2020-09-15 21:58:53.000000 ci-buildbot-0.9.1/ci_buildbot/templates/general_start.tpl
+-rw-rw-r--   0 cmalek     (501) staff       (20)      628 2023-06-26 17:23:34.000000 ci-buildbot-0.9.1/ci_buildbot/templates/general_success.tpl
+-rw-rw-r--   0 cmalek     (501) staff       (20)      667 2021-01-07 23:14:54.000000 ci-buildbot-0.9.1/ci_buildbot/templates/unittests_failed.tpl
+-rw-rw-r--   0 cmalek     (501) staff       (20)      597 2021-01-07 00:11:19.000000 ci-buildbot-0.9.1/ci_buildbot/templates/unittests_start.tpl
+-rw-rw-r--   0 cmalek     (501) staff       (20)      669 2021-01-07 23:15:01.000000 ci-buildbot-0.9.1/ci_buildbot/templates/unittests_success.tpl
+-rw-rw-r--   0 cmalek     (501) staff       (20)       63 2023-06-26 17:23:34.000000 ci-buildbot-0.9.1/ci_buildbot/typedefs.py
+drwxrwxr-x   0 cmalek     (501) staff       (20)        0 2023-06-27 17:51:27.000000 ci-buildbot-0.9.1/ci_buildbot.egg-info/
+-rw-rw-r--   0 cmalek     (501) staff       (20)     3588 2023-06-27 17:51:27.000000 ci-buildbot-0.9.1/ci_buildbot.egg-info/PKG-INFO
+-rw-rw-r--   0 cmalek     (501) staff       (20)     1850 2023-06-27 17:51:27.000000 ci-buildbot-0.9.1/ci_buildbot.egg-info/SOURCES.txt
+-rw-rw-r--   0 cmalek     (501) staff       (20)        1 2023-06-27 17:51:27.000000 ci-buildbot-0.9.1/ci_buildbot.egg-info/dependency_links.txt
+-rw-rw-r--   0 cmalek     (501) staff       (20)       51 2023-06-27 17:51:27.000000 ci-buildbot-0.9.1/ci_buildbot.egg-info/entry_points.txt
+-rw-rw-r--   0 cmalek     (501) staff       (20)      135 2023-06-27 17:51:27.000000 ci-buildbot-0.9.1/ci_buildbot.egg-info/requires.txt
+-rw-rw-r--   0 cmalek     (501) staff       (20)       12 2023-06-27 17:51:27.000000 ci-buildbot-0.9.1/ci_buildbot.egg-info/top_level.txt
+drwxrwxr-x   0 cmalek     (501) staff       (20)        0 2023-06-27 17:51:27.000000 ci-buildbot-0.9.1/etc/
+-rw-rw-r--   0 cmalek     (501) staff       (20)      313 2020-06-03 21:28:58.000000 ci-buildbot-0.9.1/etc/environment.txt
+-rw-rw-r--   0 cmalek     (501) staff       (20)     2275 2023-06-26 17:23:34.000000 ci-buildbot-0.9.1/requirements.txt
+-rw-rw-r--   0 cmalek     (501) staff       (20)      986 2023-06-27 17:51:27.000000 ci-buildbot-0.9.1/setup.cfg
+-rw-rw-r--   0 cmalek     (501) staff       (20)     1040 2023-06-27 17:51:14.000000 ci-buildbot-0.9.1/setup.py
```

### Comparing `ci-buildbot-0.9.0/PKG-INFO` & `ci-buildbot-0.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ci-buildbot
-Version: 0.9.0
+Version: 0.9.1
 Summary: Slack client for reporting on CodePipeline runs
 Home-page: https://github.com/caltechads/ci-buildbot
 Author: Caltech IMSS ADS
 Author-email: imss-ads-staff@caltech.edu
 License: UNKNOWN
 Description: # ci-buildbot
```

### Comparing `ci-buildbot-0.9.0/README.md` & `ci-buildbot-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `ci-buildbot-0.9.0/ci_buildbot/cli.py` & `ci-buildbot-0.9.1/ci_buildbot/cli.py`

 * *Files identical despite different names*

### Comparing `ci-buildbot-0.9.0/ci_buildbot/context_processors/base.py` & `ci-buildbot-0.9.1/ci_buildbot/context_processors/base.py`

 * *Files identical despite different names*

### Comparing `ci-buildbot-0.9.0/ci_buildbot/context_processors/codebuild.py` & `ci-buildbot-0.9.1/ci_buildbot/context_processors/codebuild.py`

 * *Files identical despite different names*

### Comparing `ci-buildbot-0.9.0/ci_buildbot/context_processors/deployfish.py` & `ci-buildbot-0.9.1/ci_buildbot/context_processors/deployfish.py`

 * *Files identical despite different names*

### Comparing `ci-buildbot-0.9.0/ci_buildbot/context_processors/docker.py` & `ci-buildbot-0.9.1/ci_buildbot/context_processors/docker.py`

 * *Files identical despite different names*

### Comparing `ci-buildbot-0.9.0/ci_buildbot/context_processors/git.py` & `ci-buildbot-0.9.1/ci_buildbot/context_processors/git.py`

 * *Files identical despite different names*

### Comparing `ci-buildbot-0.9.0/ci_buildbot/context_processors/project.py` & `ci-buildbot-0.9.1/ci_buildbot/context_processors/project.py`

 * *Files identical despite different names*

### Comparing `ci-buildbot-0.9.0/ci_buildbot/context_processors/unittest.py` & `ci-buildbot-0.9.1/ci_buildbot/context_processors/unittest.py`

 * *Files identical despite different names*

### Comparing `ci-buildbot-0.9.0/ci_buildbot/messages/__init__.py` & `ci-buildbot-0.9.1/ci_buildbot/messages/__init__.py`

 * *Files identical despite different names*

### Comparing `ci-buildbot-0.9.0/ci_buildbot/messages/base.py` & `ci-buildbot-0.9.1/ci_buildbot/messages/base.py`

 * *Files identical despite different names*

### Comparing `ci-buildbot-0.9.0/ci_buildbot/messages/deployfish.py` & `ci-buildbot-0.9.1/ci_buildbot/messages/deployfish.py`

 * *Files identical despite different names*

### Comparing `ci-buildbot-0.9.0/ci_buildbot/messages/deployfish_tasks.py` & `ci-buildbot-0.9.1/ci_buildbot/messages/deployfish_tasks.py`

 * *Files identical despite different names*

### Comparing `ci-buildbot-0.9.0/ci_buildbot/messages/docker.py` & `ci-buildbot-0.9.1/ci_buildbot/messages/docker.py`

 * *Files identical despite different names*

### Comparing `ci-buildbot-0.9.0/ci_buildbot/messages/docs.py` & `ci-buildbot-0.9.1/ci_buildbot/messages/docs.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,46 +1,42 @@
 from ..context_processors import (
     NameVersionProcessor,
     GitProcessor,
     CodebuildProcessor,
-    SphinxProcessor
 )
 from .base import Message
 
 
 class DocsStartMessage(Message):
     """
     Send a slack message about starting a Sphinx docs build.
     """
     template = 'docs_start.tpl'
     context_processors = [
         NameVersionProcessor,
         GitProcessor,
         CodebuildProcessor,
-        SphinxProcessor
     ]
 
 
 class DocsSuccessMessage(Message):
     """
     Send a slack message about a successful Sphinx docs build.
     """
     template = 'docs_success.tpl'
     context_processors = [
         NameVersionProcessor,
         GitProcessor,
         CodebuildProcessor,
-        SphinxProcessor
     ]
 
 
 class DocsFailureMessage(Message):
     """
     Send a slack message about an unsuccessful Sphinx docs build.
     """
     template = 'docs_failed.tpl'
     context_processors = [
         NameVersionProcessor,
         GitProcessor,
         CodebuildProcessor,
-        SphinxProcessor
     ]
```

### Comparing `ci-buildbot-0.9.0/ci_buildbot/messages/general.py` & `ci-buildbot-0.9.1/ci_buildbot/messages/general.py`

 * *Files identical despite different names*

### Comparing `ci-buildbot-0.9.0/ci_buildbot/messages/unittests.py` & `ci-buildbot-0.9.1/ci_buildbot/messages/unittests.py`

 * *Files identical despite different names*

### Comparing `ci-buildbot-0.9.0/ci_buildbot/settings.py` & `ci-buildbot-0.9.1/ci_buildbot/settings.py`

 * *Files identical despite different names*

### Comparing `ci-buildbot-0.9.0/ci_buildbot/templates/archive.tpl` & `ci-buildbot-0.9.1/ci_buildbot/templates/archive.tpl`

 * *Files identical despite different names*

### Comparing `ci-buildbot-0.9.0/ci_buildbot/templates/deploy_failed.tpl` & `ci-buildbot-0.9.1/ci_buildbot/templates/deploy_failed.tpl`

 * *Files identical despite different names*

### Comparing `ci-buildbot-0.9.0/ci_buildbot/templates/deploy_start.tpl` & `ci-buildbot-0.9.1/ci_buildbot/templates/deploy_start.tpl`

 * *Files identical despite different names*

### Comparing `ci-buildbot-0.9.0/ci_buildbot/templates/deploy_success.tpl` & `ci-buildbot-0.9.1/ci_buildbot/templates/deploy_success.tpl`

 * *Files identical despite different names*

### Comparing `ci-buildbot-0.9.0/ci_buildbot/templates/deploy_tasks_failed.tpl` & `ci-buildbot-0.9.1/ci_buildbot/templates/deploy_tasks_failed.tpl`

 * *Files identical despite different names*

### Comparing `ci-buildbot-0.9.0/ci_buildbot/templates/deploy_tasks_start.tpl` & `ci-buildbot-0.9.1/ci_buildbot/templates/deploy_tasks_start.tpl`

 * *Files identical despite different names*

### Comparing `ci-buildbot-0.9.0/ci_buildbot/templates/deploy_tasks_success.tpl` & `ci-buildbot-0.9.1/ci_buildbot/templates/deploy_tasks_success.tpl`

 * *Files identical despite different names*

### Comparing `ci-buildbot-0.9.0/ci_buildbot/templates/docker_failed.tpl` & `ci-buildbot-0.9.1/ci_buildbot/templates/docker_failed.tpl`

 * *Files identical despite different names*

### Comparing `ci-buildbot-0.9.0/ci_buildbot/templates/docker_start.tpl` & `ci-buildbot-0.9.1/ci_buildbot/templates/docker_start.tpl`

 * *Files identical despite different names*

### Comparing `ci-buildbot-0.9.0/ci_buildbot/templates/docker_success.tpl` & `ci-buildbot-0.9.1/ci_buildbot/templates/docker_success.tpl`

 * *Files identical despite different names*

### Comparing `ci-buildbot-0.9.0/ci_buildbot/templates/docs_failed.tpl` & `ci-buildbot-0.9.1/ci_buildbot/templates/docs_failed.tpl`

 * *Files identical despite different names*

### Comparing `ci-buildbot-0.9.0/ci_buildbot/templates/docs_start.tpl` & `ci-buildbot-0.9.1/ci_buildbot/templates/docs_start.tpl`

 * *Files identical despite different names*

### Comparing `ci-buildbot-0.9.0/ci_buildbot/templates/docs_success.tpl` & `ci-buildbot-0.9.1/ci_buildbot/templates/docs_success.tpl`

 * *Files identical despite different names*

### Comparing `ci-buildbot-0.9.0/ci_buildbot/templates/general_failed.tpl` & `ci-buildbot-0.9.1/ci_buildbot/templates/general_failed.tpl`

 * *Files identical despite different names*

### Comparing `ci-buildbot-0.9.0/ci_buildbot/templates/general_start.tpl` & `ci-buildbot-0.9.1/ci_buildbot/templates/general_start.tpl`

 * *Files identical despite different names*

### Comparing `ci-buildbot-0.9.0/ci_buildbot/templates/general_success.tpl` & `ci-buildbot-0.9.1/ci_buildbot/templates/general_success.tpl`

 * *Files identical despite different names*

### Comparing `ci-buildbot-0.9.0/ci_buildbot/templates/unittests_failed.tpl` & `ci-buildbot-0.9.1/ci_buildbot/templates/unittests_failed.tpl`

 * *Files identical despite different names*

### Comparing `ci-buildbot-0.9.0/ci_buildbot/templates/unittests_start.tpl` & `ci-buildbot-0.9.1/ci_buildbot/templates/unittests_start.tpl`

 * *Files identical despite different names*

### Comparing `ci-buildbot-0.9.0/ci_buildbot/templates/unittests_success.tpl` & `ci-buildbot-0.9.1/ci_buildbot/templates/unittests_success.tpl`

 * *Files identical despite different names*

### Comparing `ci-buildbot-0.9.0/ci_buildbot.egg-info/PKG-INFO` & `ci-buildbot-0.9.1/ci_buildbot.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ci-buildbot
-Version: 0.9.0
+Version: 0.9.1
 Summary: Slack client for reporting on CodePipeline runs
 Home-page: https://github.com/caltechads/ci-buildbot
 Author: Caltech IMSS ADS
 Author-email: imss-ads-staff@caltech.edu
 License: UNKNOWN
 Description: # ci-buildbot
```

### Comparing `ci-buildbot-0.9.0/ci_buildbot.egg-info/SOURCES.txt` & `ci-buildbot-0.9.1/ci_buildbot.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,14 @@
 ci_buildbot/context_processors/base.py
 ci_buildbot/context_processors/codebuild.py
 ci_buildbot/context_processors/deployfish.py
 ci_buildbot/context_processors/docker.py
 ci_buildbot/context_processors/generic.py
 ci_buildbot/context_processors/git.py
 ci_buildbot/context_processors/project.py
-ci_buildbot/context_processors/sphinx.py
 ci_buildbot/context_processors/unittest.py
 ci_buildbot/messages/__init__.py
 ci_buildbot/messages/archive.py
 ci_buildbot/messages/base.py
 ci_buildbot/messages/deployfish.py
 ci_buildbot/messages/deployfish_tasks.py
 ci_buildbot/messages/docker.py
```

### Comparing `ci-buildbot-0.9.0/requirements.txt` & `ci-buildbot-0.9.1/requirements.txt`

 * *Files identical despite different names*

### Comparing `ci-buildbot-0.9.0/setup.cfg` & `ci-buildbot-0.9.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `ci-buildbot-0.9.0/setup.py` & `ci-buildbot-0.9.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name="ci-buildbot",
-    version='0.9.0',
+    version='0.9.1',
     description="Slack client for reporting on CodePipeline runs",
     url="https://github.com/caltechads/ci-buildbot",
     author="Caltech IMSS ADS",
     author_email="imss-ads-staff@caltech.edu",
     packages=find_packages(exclude=["*.test", "*.test.*", "test.*", "test", "bin", "*.pyc"]),
     include_package_data=True,
     long_description=long_description,
```

