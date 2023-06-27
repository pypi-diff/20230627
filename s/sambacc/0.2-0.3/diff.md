# Comparing `tmp/sambacc-0.2.tar.gz` & `tmp/sambacc-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sambacc-0.2.tar", last modified: Wed May 25 18:41:58 2022, max compression
+gzip compressed data, was "sambacc-0.3.tar", last modified: Mon Jun 26 20:09:30 2023, max compression
```

## Comparing `sambacc-0.2.tar` & `sambacc-0.3.tar`

### file list

```diff
@@ -1,81 +1,95 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-25 18:41:58.252889 sambacc-0.2/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-25 18:41:58.246888 sambacc-0.2/.github/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-25 18:41:58.247889 sambacc-0.2/.github/workflows/
--rw-rw-r--   0 root         (0) root         (0)      898 2022-05-25 18:36:09.000000 sambacc-0.2/.github/workflows/ci.yml
--rw-rw-r--   0 root         (0) root         (0)       92 2022-05-25 18:36:09.000000 sambacc-0.2/.gitignore
--rw-rw-r--   0 root         (0) root         (0)      122 2022-05-25 18:36:09.000000 sambacc-0.2/.hgignore
--rw-rw-r--   0 root         (0) root         (0)    35149 2022-05-25 18:36:09.000000 sambacc-0.2/COPYING
--rw-rw-r--   0 root         (0) root         (0)       53 2022-05-25 18:36:09.000000 sambacc-0.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      246 2022-05-25 18:41:58.252889 sambacc-0.2/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     5306 2022-05-25 18:36:09.000000 sambacc-0.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-25 18:41:58.247889 sambacc-0.2/examples/
--rw-rw-r--   0 root         (0) root         (0)     2972 2022-05-25 18:36:09.000000 sambacc-0.2/examples/addc.json
--rw-rw-r--   0 root         (0) root         (0)      906 2022-05-25 18:36:09.000000 sambacc-0.2/examples/ctdb.json
--rw-rw-r--   0 root         (0) root         (0)     1014 2022-05-25 18:36:09.000000 sambacc-0.2/examples/example1.json
--rw-rw-r--   0 root         (0) root         (0)      842 2022-05-25 18:36:09.000000 sambacc-0.2/examples/minimal.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-25 18:41:58.247889 sambacc-0.2/extras/
--rw-rw-r--   0 root         (0) root         (0)     1646 2022-05-25 18:36:09.000000 sambacc-0.2/extras/python-sambacc.spec
--rw-rw-r--   0 root         (0) root         (0)      531 2022-05-25 18:36:09.000000 sambacc-0.2/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-25 18:41:58.249889 sambacc-0.2/sambacc/
--rw-rw-r--   0 root         (0) root         (0)        0 2022-05-25 18:36:09.000000 sambacc-0.2/sambacc/__init__.py
--rw-r--r--   0 root         (0) root         (0)       90 2022-05-25 18:41:57.000000 sambacc-0.2/sambacc/_version.py
--rw-rw-r--   0 root         (0) root         (0)     2455 2022-05-25 18:36:09.000000 sambacc-0.2/sambacc/_xattr.py
--rw-rw-r--   0 root         (0) root         (0)     4595 2022-05-25 18:36:09.000000 sambacc-0.2/sambacc/addc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-25 18:41:58.250889 sambacc-0.2/sambacc/commands/
--rw-rw-r--   0 root         (0) root         (0)        0 2022-05-25 18:36:09.000000 sambacc-0.2/sambacc/commands/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     4965 2022-05-25 18:36:09.000000 sambacc-0.2/sambacc/commands/addc.py
--rw-rw-r--   0 root         (0) root         (0)     1391 2022-05-25 18:36:09.000000 sambacc-0.2/sambacc/commands/check.py
--rw-rw-r--   0 root         (0) root         (0)     5523 2022-05-25 18:36:09.000000 sambacc-0.2/sambacc/commands/cli.py
--rw-rw-r--   0 root         (0) root         (0)     5266 2022-05-25 18:36:09.000000 sambacc-0.2/sambacc/commands/config.py
--rw-rw-r--   0 root         (0) root         (0)     8412 2022-05-25 18:36:09.000000 sambacc-0.2/sambacc/commands/ctdb.py
--rw-rw-r--   0 root         (0) root         (0)     1400 2022-05-25 18:36:09.000000 sambacc-0.2/sambacc/commands/dcmain.py
--rw-rw-r--   0 root         (0) root         (0)     3359 2022-05-25 18:36:09.000000 sambacc-0.2/sambacc/commands/dns.py
--rw-rw-r--   0 root         (0) root         (0)     3741 2022-05-25 18:36:09.000000 sambacc-0.2/sambacc/commands/initialize.py
--rw-rw-r--   0 root         (0) root         (0)     4563 2022-05-25 18:36:09.000000 sambacc-0.2/sambacc/commands/join.py
--rw-rw-r--   0 root         (0) root         (0)     6064 2022-05-25 18:36:09.000000 sambacc-0.2/sambacc/commands/main.py
--rw-rw-r--   0 root         (0) root         (0)     3248 2022-05-25 18:36:09.000000 sambacc-0.2/sambacc/commands/run.py
--rw-rw-r--   0 root         (0) root         (0)     1976 2022-05-25 18:36:09.000000 sambacc-0.2/sambacc/commands/users.py
--rw-rw-r--   0 root         (0) root         (0)    14216 2022-05-25 18:36:09.000000 sambacc-0.2/sambacc/config.py
--rw-rw-r--   0 root         (0) root         (0)     3606 2022-05-25 18:36:09.000000 sambacc-0.2/sambacc/container_dns.py
--rw-rw-r--   0 root         (0) root         (0)    17390 2022-05-25 18:36:09.000000 sambacc-0.2/sambacc/ctdb.py
--rw-rw-r--   0 root         (0) root         (0)     3040 2022-05-25 18:36:09.000000 sambacc-0.2/sambacc/inotify_waiter.py
--rw-rw-r--   0 root         (0) root         (0)     1797 2022-05-25 18:36:09.000000 sambacc-0.2/sambacc/jfile.py
--rw-rw-r--   0 root         (0) root         (0)     6097 2022-05-25 18:36:09.000000 sambacc-0.2/sambacc/join.py
--rw-rw-r--   0 root         (0) root         (0)     1239 2022-05-25 18:36:09.000000 sambacc-0.2/sambacc/leader.py
--rw-rw-r--   0 root         (0) root         (0)     2989 2022-05-25 18:36:09.000000 sambacc-0.2/sambacc/netcmd_loader.py
--rw-rw-r--   0 root         (0) root         (0)     2307 2022-05-25 18:36:09.000000 sambacc-0.2/sambacc/nsswitch_loader.py
--rw-rw-r--   0 root         (0) root         (0)     2827 2022-05-25 18:36:09.000000 sambacc-0.2/sambacc/passdb_loader.py
--rw-rw-r--   0 root         (0) root         (0)     2854 2022-05-25 18:36:09.000000 sambacc-0.2/sambacc/passwd_loader.py
--rw-rw-r--   0 root         (0) root         (0)     1803 2022-05-25 18:36:09.000000 sambacc-0.2/sambacc/paths.py
--rw-rw-r--   0 root         (0) root         (0)     5115 2022-05-25 18:36:09.000000 sambacc-0.2/sambacc/permissions.py
--rw-rw-r--   0 root         (0) root         (0)     4968 2022-05-25 18:36:09.000000 sambacc-0.2/sambacc/samba_cmds.py
--rw-rw-r--   0 root         (0) root         (0)     2873 2022-05-25 18:36:09.000000 sambacc-0.2/sambacc/simple_waiter.py
--rw-rw-r--   0 root         (0) root         (0)     1635 2022-05-25 18:36:09.000000 sambacc-0.2/sambacc/textfile.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-25 18:41:58.249889 sambacc-0.2/sambacc.egg-info/
--rw-r--r--   0 root         (0) root         (0)      246 2022-05-25 18:41:57.000000 sambacc-0.2/sambacc.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1575 2022-05-25 18:41:58.000000 sambacc-0.2/sambacc.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-05-25 18:41:57.000000 sambacc-0.2/sambacc.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      113 2022-05-25 18:41:58.000000 sambacc-0.2/sambacc.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        8 2022-05-25 18:41:58.000000 sambacc-0.2/sambacc.egg-info/top_level.txt
--rw-rw-r--   0 root         (0) root         (0)      633 2022-05-25 18:41:58.252889 sambacc-0.2/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-25 18:41:58.252889 sambacc-0.2/tests/
--rw-rw-r--   0 root         (0) root         (0)        0 2022-05-25 18:36:09.000000 sambacc-0.2/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-25 18:41:58.252889 sambacc-0.2/tests/container/
--rw-rw-r--   0 root         (0) root         (0)      750 2022-05-25 18:36:09.000000 sambacc-0.2/tests/container/Containerfile
--rwxrwxr-x   0 root         (0) root         (0)     4074 2022-05-25 18:36:09.000000 sambacc-0.2/tests/container/build.sh
--rw-rw-r--   0 root         (0) root         (0)     7917 2022-05-25 18:36:09.000000 sambacc-0.2/tests/test_commands_config.py
--rw-rw-r--   0 root         (0) root         (0)    19347 2022-05-25 18:36:09.000000 sambacc-0.2/tests/test_config.py
--rw-rw-r--   0 root         (0) root         (0)     5637 2022-05-25 18:36:09.000000 sambacc-0.2/tests/test_container_dns.py
--rw-rw-r--   0 root         (0) root         (0)    18053 2022-05-25 18:36:09.000000 sambacc-0.2/tests/test_ctdb.py
--rw-rw-r--   0 root         (0) root         (0)     2350 2022-05-25 18:36:09.000000 sambacc-0.2/tests/test_inotify_waiter.py
--rw-rw-r--   0 root         (0) root         (0)     2537 2022-05-25 18:36:09.000000 sambacc-0.2/tests/test_jfile.py
--rw-rw-r--   0 root         (0) root         (0)     8248 2022-05-25 18:36:09.000000 sambacc-0.2/tests/test_join.py
--rw-rw-r--   0 root         (0) root         (0)     1979 2022-05-25 18:36:09.000000 sambacc-0.2/tests/test_main.py
--rw-rw-r--   0 root         (0) root         (0)     3702 2022-05-25 18:36:09.000000 sambacc-0.2/tests/test_netcmd_loader.py
--rw-rw-r--   0 root         (0) root         (0)     3435 2022-05-25 18:36:09.000000 sambacc-0.2/tests/test_passdb_loader.py
--rw-rw-r--   0 root         (0) root         (0)     3653 2022-05-25 18:36:09.000000 sambacc-0.2/tests/test_passwd_loader.py
--rw-rw-r--   0 root         (0) root         (0)     2193 2022-05-25 18:36:09.000000 sambacc-0.2/tests/test_paths.py
--rw-rw-r--   0 root         (0) root         (0)     2851 2022-05-25 18:36:09.000000 sambacc-0.2/tests/test_permissions.py
--rw-rw-r--   0 root         (0) root         (0)     4826 2022-05-25 18:36:09.000000 sambacc-0.2/tests/test_samba_cmds.py
--rw-rw-r--   0 root         (0) root         (0)     1761 2022-05-25 18:36:09.000000 sambacc-0.2/tests/test_simmple_waiter.py
--rw-rw-r--   0 root         (0) root         (0)      574 2022-05-25 18:36:09.000000 sambacc-0.2/tox.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 20:09:30.827397 sambacc-0.3/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 20:09:30.817397 sambacc-0.3/.copr/
+-rw-r--r--   0 root         (0) root         (0)      600 2023-06-26 19:41:37.000000 sambacc-0.3/.copr/Makefile
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 20:09:30.817397 sambacc-0.3/.github/
+-rw-r--r--   0 root         (0) root         (0)     2889 2023-06-26 19:41:37.000000 sambacc-0.3/.github/mergify.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 20:09:30.818397 sambacc-0.3/.github/workflows/
+-rw-r--r--   0 root         (0) root         (0)     2239 2023-06-26 19:41:37.000000 sambacc-0.3/.github/workflows/ci.yml
+-rw-r--r--   0 root         (0) root         (0)       92 2023-06-26 19:41:37.000000 sambacc-0.3/.gitignore
+-rw-r--r--   0 root         (0) root         (0)     4336 2023-06-26 19:41:37.000000 sambacc-0.3/.gitlint
+-rw-r--r--   0 root         (0) root         (0)      122 2023-06-26 19:41:37.000000 sambacc-0.3/.hgignore
+-rw-r--r--   0 root         (0) root         (0)    35149 2023-06-26 19:41:37.000000 sambacc-0.3/COPYING
+-rw-r--r--   0 root         (0) root         (0)      100 2023-06-26 19:41:37.000000 sambacc-0.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      315 2023-06-26 20:09:30.827397 sambacc-0.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     6709 2023-06-26 19:41:37.000000 sambacc-0.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 20:09:30.818397 sambacc-0.3/docs/
+-rw-r--r--   0 root         (0) root         (0)    11714 2023-06-26 19:41:37.000000 sambacc-0.3/docs/configuration.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 20:09:30.818397 sambacc-0.3/examples/
+-rw-r--r--   0 root         (0) root         (0)     2972 2023-06-26 19:41:37.000000 sambacc-0.3/examples/addc.json
+-rw-r--r--   0 root         (0) root         (0)      906 2023-06-26 19:41:37.000000 sambacc-0.3/examples/ctdb.json
+-rw-r--r--   0 root         (0) root         (0)     1014 2023-06-26 19:41:37.000000 sambacc-0.3/examples/example1.json
+-rw-r--r--   0 root         (0) root         (0)      842 2023-06-26 19:41:37.000000 sambacc-0.3/examples/minimal.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 20:09:30.819397 sambacc-0.3/extras/
+-rw-r--r--   0 root         (0) root         (0)     2102 2023-06-26 19:41:37.000000 sambacc-0.3/extras/python-sambacc.spec
+-rw-r--r--   0 root         (0) root         (0)      819 2023-06-26 19:41:37.000000 sambacc-0.3/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 20:09:30.821397 sambacc-0.3/sambacc/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-26 19:41:37.000000 sambacc-0.3/sambacc/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       90 2023-06-26 20:09:30.000000 sambacc-0.3/sambacc/_version.py
+-rw-r--r--   0 root         (0) root         (0)     2455 2023-06-26 19:41:37.000000 sambacc-0.3/sambacc/_xattr.py
+-rw-r--r--   0 root         (0) root         (0)     4540 2023-06-26 19:41:37.000000 sambacc-0.3/sambacc/addc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 20:09:30.824397 sambacc-0.3/sambacc/commands/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-26 19:41:37.000000 sambacc-0.3/sambacc/commands/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4965 2023-06-26 19:41:37.000000 sambacc-0.3/sambacc/commands/addc.py
+-rw-r--r--   0 root         (0) root         (0)     1391 2023-06-26 19:41:37.000000 sambacc-0.3/sambacc/commands/check.py
+-rw-r--r--   0 root         (0) root         (0)     5975 2023-06-26 19:41:37.000000 sambacc-0.3/sambacc/commands/cli.py
+-rw-r--r--   0 root         (0) root         (0)     5348 2023-06-26 19:41:37.000000 sambacc-0.3/sambacc/commands/config.py
+-rw-r--r--   0 root         (0) root         (0)     8412 2023-06-26 19:41:37.000000 sambacc-0.3/sambacc/commands/ctdb.py
+-rw-r--r--   0 root         (0) root         (0)     1456 2023-06-26 19:41:37.000000 sambacc-0.3/sambacc/commands/dcmain.py
+-rw-r--r--   0 root         (0) root         (0)     3447 2023-06-26 19:41:37.000000 sambacc-0.3/sambacc/commands/dns.py
+-rw-r--r--   0 root         (0) root         (0)     3802 2023-06-26 19:41:37.000000 sambacc-0.3/sambacc/commands/initialize.py
+-rw-r--r--   0 root         (0) root         (0)     4671 2023-06-26 19:41:37.000000 sambacc-0.3/sambacc/commands/join.py
+-rw-r--r--   0 root         (0) root         (0)     6807 2023-06-26 19:41:37.000000 sambacc-0.3/sambacc/commands/main.py
+-rw-r--r--   0 root         (0) root         (0)     3248 2023-06-26 19:41:37.000000 sambacc-0.3/sambacc/commands/run.py
+-rw-r--r--   0 root         (0) root         (0)     1976 2023-06-26 19:41:37.000000 sambacc-0.3/sambacc/commands/users.py
+-rw-r--r--   0 root         (0) root         (0)    17715 2023-06-26 19:41:37.000000 sambacc-0.3/sambacc/config.py
+-rw-r--r--   0 root         (0) root         (0)     4255 2023-06-26 19:41:37.000000 sambacc-0.3/sambacc/container_dns.py
+-rw-r--r--   0 root         (0) root         (0)    17972 2023-06-26 19:41:37.000000 sambacc-0.3/sambacc/ctdb.py
+-rw-r--r--   0 root         (0) root         (0)     3154 2023-06-26 19:41:37.000000 sambacc-0.3/sambacc/inotify_waiter.py
+-rw-r--r--   0 root         (0) root         (0)     1964 2023-06-26 19:41:37.000000 sambacc-0.3/sambacc/jfile.py
+-rw-r--r--   0 root         (0) root         (0)     6451 2023-06-26 19:41:37.000000 sambacc-0.3/sambacc/join.py
+-rw-r--r--   0 root         (0) root         (0)     1348 2023-06-26 19:41:37.000000 sambacc-0.3/sambacc/leader.py
+-rw-r--r--   0 root         (0) root         (0)     3120 2023-06-26 19:41:37.000000 sambacc-0.3/sambacc/netcmd_loader.py
+-rw-r--r--   0 root         (0) root         (0)     2347 2023-06-26 19:41:37.000000 sambacc-0.3/sambacc/nsswitch_loader.py
+-rw-r--r--   0 root         (0) root         (0)     2897 2023-06-26 19:41:37.000000 sambacc-0.3/sambacc/passdb_loader.py
+-rw-r--r--   0 root         (0) root         (0)     2928 2023-06-26 19:41:37.000000 sambacc-0.3/sambacc/passwd_loader.py
+-rw-r--r--   0 root         (0) root         (0)     1803 2023-06-26 19:41:37.000000 sambacc-0.3/sambacc/paths.py
+-rw-r--r--   0 root         (0) root         (0)     5147 2023-06-26 19:41:37.000000 sambacc-0.3/sambacc/permissions.py
+-rw-r--r--   0 root         (0) root         (0)     5230 2023-06-26 19:41:37.000000 sambacc-0.3/sambacc/samba_cmds.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 20:09:30.824397 sambacc-0.3/sambacc/schema/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-26 19:41:37.000000 sambacc-0.3/sambacc/schema/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9823 2023-06-26 19:41:37.000000 sambacc-0.3/sambacc/schema/conf-v0.schema.json
+-rw-r--r--   0 root         (0) root         (0)     9783 2023-06-26 19:41:37.000000 sambacc-0.3/sambacc/schema/conf-v0.schema.yaml
+-rw-r--r--   0 root         (0) root         (0)    12292 2023-06-26 19:41:37.000000 sambacc-0.3/sambacc/schema/conf_v0_schema.py
+-rw-r--r--   0 root         (0) root         (0)     4906 2023-06-26 19:41:37.000000 sambacc-0.3/sambacc/schema/tool.py
+-rw-r--r--   0 root         (0) root         (0)     2976 2023-06-26 19:41:37.000000 sambacc-0.3/sambacc/simple_waiter.py
+-rw-r--r--   0 root         (0) root         (0)     1635 2023-06-26 19:41:37.000000 sambacc-0.3/sambacc/textfile.py
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-06-26 19:41:37.000000 sambacc-0.3/sambacc/typelets.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 20:09:30.822397 sambacc-0.3/sambacc.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      315 2023-06-26 20:09:30.000000 sambacc-0.3/sambacc.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1844 2023-06-26 20:09:30.000000 sambacc-0.3/sambacc.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-26 20:09:30.000000 sambacc-0.3/sambacc.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      113 2023-06-26 20:09:30.000000 sambacc-0.3/sambacc.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       97 2023-06-26 20:09:30.000000 sambacc-0.3/sambacc.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-06-26 20:09:30.000000 sambacc-0.3/sambacc.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      765 2023-06-26 20:09:30.827397 sambacc-0.3/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 20:09:30.826397 sambacc-0.3/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-26 19:41:37.000000 sambacc-0.3/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 20:09:30.827397 sambacc-0.3/tests/container/
+-rw-r--r--   0 root         (0) root         (0)      626 2023-06-26 19:41:37.000000 sambacc-0.3/tests/container/Containerfile
+-rwxr-xr-x   0 root         (0) root         (0)     7060 2023-06-26 19:41:37.000000 sambacc-0.3/tests/container/build.sh
+-rw-r--r--   0 root         (0) root         (0)     7957 2023-06-26 19:41:37.000000 sambacc-0.3/tests/test_commands_config.py
+-rw-r--r--   0 root         (0) root         (0)    30050 2023-06-26 19:41:37.000000 sambacc-0.3/tests/test_config.py
+-rw-r--r--   0 root         (0) root         (0)     5707 2023-06-26 19:41:37.000000 sambacc-0.3/tests/test_container_dns.py
+-rw-r--r--   0 root         (0) root         (0)    18241 2023-06-26 19:41:37.000000 sambacc-0.3/tests/test_ctdb.py
+-rw-r--r--   0 root         (0) root         (0)     2350 2023-06-26 19:41:37.000000 sambacc-0.3/tests/test_inotify_waiter.py
+-rw-r--r--   0 root         (0) root         (0)     2537 2023-06-26 19:41:37.000000 sambacc-0.3/tests/test_jfile.py
+-rw-r--r--   0 root         (0) root         (0)     8248 2023-06-26 19:41:37.000000 sambacc-0.3/tests/test_join.py
+-rw-r--r--   0 root         (0) root         (0)     1979 2023-06-26 19:41:37.000000 sambacc-0.3/tests/test_main.py
+-rw-r--r--   0 root         (0) root         (0)     3702 2023-06-26 19:41:37.000000 sambacc-0.3/tests/test_netcmd_loader.py
+-rw-r--r--   0 root         (0) root         (0)     3435 2023-06-26 19:41:37.000000 sambacc-0.3/tests/test_passdb_loader.py
+-rw-r--r--   0 root         (0) root         (0)     3653 2023-06-26 19:41:37.000000 sambacc-0.3/tests/test_passwd_loader.py
+-rw-r--r--   0 root         (0) root         (0)     2193 2023-06-26 19:41:37.000000 sambacc-0.3/tests/test_paths.py
+-rw-r--r--   0 root         (0) root         (0)     2851 2023-06-26 19:41:37.000000 sambacc-0.3/tests/test_permissions.py
+-rw-r--r--   0 root         (0) root         (0)     4826 2023-06-26 19:41:37.000000 sambacc-0.3/tests/test_samba_cmds.py
+-rw-r--r--   0 root         (0) root         (0)     1761 2023-06-26 19:41:37.000000 sambacc-0.3/tests/test_simmple_waiter.py
+-rw-r--r--   0 root         (0) root         (0)     1585 2023-06-26 19:41:37.000000 sambacc-0.3/tox.ini
```

### Comparing `sambacc-0.2/COPYING` & `sambacc-0.3/COPYING`

 * *Files identical despite different names*

### Comparing `sambacc-0.2/README.md` & `sambacc-0.3/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 # sambacc - A Samba Container Configuration Tool
 
 ## About
 
-The sambacc is an young project that aims to consolidate and coordinate
-configuration of [Samba](http://samba.org), and related components, when
-running in a container. The configuration of one or many instances can be
-provided to the tool by way of a JSON file which then handles the low level
-details of actually configuring smbd and other elements in the container
+The sambacc project aims to consolidate and coordinate configuration of
+[Samba](http://samba.org), and related components, when running in a
+container. The configuration of one or many server instances can be
+managed by the tool with the use of configuration files.  These
+configuration files act as a superset of the well-known smb.conf, to
+configure Samba, as well as other low level details of the container
 environment.
 
 
 ## Rationale
 
-Samba is a powerful and unique tool for implementing the SMB protocol and a
-software stack to support it on unix-like systems. However, it's potentially
-challenging to set up and manage many instances of Samba by-hand, especially
-when running under a container orchestration system.
-
-The idea behind sambacc is mainly to automate all of the low level steps of
-setting up smbd, users, groups, and other supporting components. The tool is
-also designed to consume one "site-wide" configuration file that can be
-maintained across many container instances. sambacc is written in Python as
-samba provides Python bindings for some of the aspects of samba we need to
-control.
+Samba is a powerful and unique tool for implementing the SMB protocol and
+a software stack to support it on unix-like systems. However, it's
+potentially challenging to set up and manage many instances of Samba
+by-hand, especially when running under a container orchestration system.
+
+The idea behind sambacc is to automate much of the low level steps needed
+to set up samba daemons, users, groups, and other supporting
+components. The tool is also designed to consume configuration files that
+can be used across many container instances. sambacc is written in Python
+as samba provides Python bindings for some of the aspects of samba we need
+to control.
 
 The sambacc library and samba-container CLI command are used by the
 [samba-container project](https://github.com/samba-in-kubernetes/samba-container/)
 as part of the server container images.
 
 
 ## Usage
@@ -70,16 +71,16 @@
 samba-dc-container --help
 ```
 
 
 ## Features
 
 * Abstracts away some of the nitty-gritty details about what Samba expects
-  in it's environment
-* Imports specific smb.conf settings from "site wide" JSON configuration.
+  in its environment
+* Imports specific smb.conf settings from "site wide" configuration files.
 * Imports users and groups
 * Starts smbd with container friendly settings
 * Starts winbindd with container friendly settings
 * Support for joining AD
 * Support for managing CTDB clustering
 * Support for creating/joining Samba Active Directory servers
 
@@ -87,18 +88,33 @@
 
 A lot. Various things that are missing include:
 
 * Features to perform more secure (password-less) domain joins
 * Better integration (as opposed to unit) testing
 * Better use of APIs versus executing CLI commands
 
+Contributions and feedback would be very much appreciated.
+
 
 ## Install
 
-Currently the only method of install is from source control.
+The sambacc library, samba-container command, and samba-dc-container are
+written assuming the software is being run within an OCI container environment.
+While there's nothing stopping you from trying to install it on something else
+the value of doing that will be rather limited.
+
+The (samba-container
+project)[https://github.com/samba-in-kubernetes/samba-container] includes
+sambacc and samba packages. If you are looking to use sambacc and not
+contribute to it, that's probably what you want.
+
+Builds of sambacc are continuously produced within our (COPR repository)[https://copr.fedorainfracloud.org/coprs/phlogistonjohn/sambacc/].
+These builds are then consumed by the container image builds.
+
+Otherwise, the only method of install is from source control.
 
 * Clone the repo: `git clone https://github.com/samba-in-kubernetes/sambacc`
 * `cd sambacc`
 * Install locally: `python -m pip install --user .`
 
 The test & build container may also be used to build source tarballs and
 wheels. Then you can distribute and install from the wheel if you need to.
@@ -106,40 +122,57 @@
 ### Testing
 
 #### Local testing
 
 To run the entire unit test suite locally install `tox` and run `tox` in
 the repo root.
 
-Because of the library and tooling that interacts with samba has some system level dependencies, not all test can be run locally.
+Because of the library and tooling that interacts with samba has some
+system level dependencies, not all tests can be run locally in
+isolated (virtualenv) environments.
+
 
 #### Containerized testing
 
-In addition to running the unit tests locally, I've created a container image
-for testing and building sambacc. It lives at ./tests/container. This is
-canonical way to run the test suite and is what is used by the CI tests. When
-run this way certain system packages can be installed, etc. to support
-running a wider range of test cases.
-
-To produce builds using the container, mount a directory into the container at
-"/srv/dist" and set the environment variable `SAMBACC_DISTNAME` to a term of
-your choice (example: "latest"). This will then save the builds in a dir of
-that name in your output dir. Example:
+A more robust and isolated testing environment is provided in
+the form of the sambacc container image.
+
+The container file and other sources are available at ./tests/container in
+the sambacc repo. This is the canonical way to run the test suite and is
+what is used by the CI tests. When run this way certain system packages
+can be installed, etc. to support running a wider range of test cases.
+
+By default the container image is configured to check out sambacc master
+branch and execute the tests and build python source distributions,
+wheels, and RPM packages. You can test your local git checkout using the
+image by mounting it at /var/tmp/build/sambacc (example: `podman run -v
+$PWD:/var/tmp/build/sambacc sambacc:ci`).
+
+To access the packages that are built using the container, mount a
+directory into the container at "/srv/dist" and set the environment
+variable `SAMBACC_DISTNAME` to a term of your choice (example: "latest").
+This will then save the builds in a directory of that name in your output
+directory.
+Example:
 ```
 $ mkdir -p $HOME/tmp/sambacc
 $ podman run --rm \
   -v $HOME/tmp/sambacc:/srv/dist -e SAMBACC_DISTNAME=latest \
   quay.io/samba.org/sambacc:latest
 $ ls $HOME/tmp/sambacc
 latest
 $ ls $HOME/tmp/sambacc/latest
 sambacc-0.1.dev225+g10059ff-py3-none-any.whl  sha512sums
 sambacc-0.1.dev225+g10059ff.tar.gz
 ```
 
+You can combine the source directory mount and distribution directory
+mount in one command to produce builds for your own local development work
+if needed.
+
 ## License
 
 GPLv3 as per the COPYING file.
 
 This is the same license as used by Samba.
```

### Comparing `sambacc-0.2/examples/addc.json` & `sambacc-0.3/examples/addc.json`

 * *Files identical despite different names*

### Comparing `sambacc-0.2/examples/ctdb.json` & `sambacc-0.3/examples/ctdb.json`

 * *Files identical despite different names*

### Comparing `sambacc-0.2/examples/example1.json` & `sambacc-0.3/examples/example1.json`

 * *Files identical despite different names*

### Comparing `sambacc-0.2/examples/minimal.json` & `sambacc-0.3/examples/minimal.json`

 * *Files identical despite different names*

### Comparing `sambacc-0.2/extras/python-sambacc.spec` & `sambacc-0.3/extras/python-sambacc.spec`

 * *Files 10% similar despite different names*

```diff
@@ -16,54 +16,70 @@
 URL:            https://github.com/samba-in-kubernetes/sambacc
 # sambacc is not released yet so we're leaving off the url for now
 # once packaged and released we can update this field
 Source:         %{bname}-%{pversion}.tar.gz
 
 BuildArch:      noarch
 BuildRequires:  python3-devel
+# we need python3-samba as a build dependency in order to run
+# the test suite
+BuildRequires:  python3-samba
+# ditto for the net binary
+BuildRequires: /usr/bin/net
 
 %global _description %{expand:
 A Python library and set of CLI tools intended to act as a bridge between a container
 environment and Samba servers and utilities. It aims to consolidate, coordinate and
 automate all of the low level steps of setting up smbd, users, groups, and other
 supporting components.
 }
 
 %description %_description
 
 %package -n python3-%{bname}
 Summary: %{summary}
-# Distro requires that are technially optional for the lib
+# Distro requires that are technically optional for the lib
 Requires: python3-samba
 Requires: python3-pyxattr
+%if 0%{?fedora} >= 37
+Recommends: %{name}+toml
+Recommends: %{name}+validation
+Recommends: %{name}+yaml
+%endif
 
 %description -n python3-%{bname}  %_description
 
 
 %prep
 %autosetup -n %{bname}-%{pversion}
 
 %generate_buildrequires
-%pyproject_buildrequires -e py3
+%pyproject_buildrequires -e py3-sys
 
 
 %build
 %pyproject_wheel
 
 
 %install
 %pyproject_install
 %pyproject_save_files %{bname}
 
 
 %check
-%tox -e py3
+%tox -e py3-sys
 
 
 %files -n python3-%{bname} -f %{pyproject_files}
 %doc README.*
 %{_bindir}/samba-container
 %{_bindir}/samba-dc-container
 %{_datadir}/%{bname}/examples/
 
 
+%pyproject_extras_subpkg -n python3-%{bname} validation
+%pyproject_extras_subpkg -n python3-%{bname} toml
+%pyproject_extras_subpkg -n python3-%{bname} yaml
+
+
 %changelog
+%autochangelog
```

### Comparing `sambacc-0.2/sambacc/_xattr.py` & `sambacc-0.3/sambacc/_xattr.py`

 * *Files identical despite different names*

### Comparing `sambacc-0.2/sambacc/addc.py` & `sambacc-0.3/sambacc/addc.py`

 * *Files 10% similar despite different names*

```diff
@@ -79,27 +79,27 @@
 
 def create_group(name: str) -> None:
     cmd = _group_add_cmd(name)
     _logger.info("Creating group: %r", name)
     subprocess.check_call(cmd)
 
 
-def add_group_members(group_name: str, members: typing.List[str]) -> None:
+def add_group_members(group_name: str, members: list[str]) -> None:
     cmd = _group_add_members_cmd(group_name, members)
     _logger.info("Adding group members: %r", cmd)
     subprocess.check_call(cmd)
 
 
 def _provision_cmd(
     realm: str,
     dcname: str,
     admin_password: str,
     dns_backend: typing.Optional[str] = None,
     domain: typing.Optional[str] = None,
-) -> typing.List[str]:
+) -> list[str]:
     if not dns_backend:
         dns_backend = "SAMBA_INTERNAL"
     if not domain:
         domain = realm.split(".")[0].upper()
     cmd = samba_cmds.sambatool[
         "domain",
         "provision",
@@ -116,15 +116,15 @@
 
 def _join_cmd(
     realm: str,
     dcname: str,
     admin_password: str,
     dns_backend: typing.Optional[str] = None,
     domain: typing.Optional[str] = None,
-) -> typing.List[str]:
+) -> list[str]:
     if not dns_backend:
         dns_backend = "SAMBA_INTERNAL"
     if not domain:
         domain = realm.split(".")[0].upper()
     cmd = samba_cmds.sambatool[
         "domain",
         "join",
@@ -139,40 +139,38 @@
 
 
 def _user_create_cmd(
     name: str,
     password: str,
     surname: typing.Optional[str],
     given_name: typing.Optional[str],
-) -> typing.List[str]:
+) -> list[str]:
     cmd = samba_cmds.sambatool[
         "user",
         "create",
         name,
         password,
     ].argv()
     if surname:
         cmd.append(f"--surname={surname}")
     if given_name:
         cmd.append(f"--given-name={given_name}")
     return cmd
 
 
-def _group_add_cmd(name: str) -> typing.List[str]:
+def _group_add_cmd(name: str) -> list[str]:
     cmd = samba_cmds.sambatool[
         "group",
         "add",
         name,
     ].argv()
     return cmd
 
 
-def _group_add_members_cmd(
-    group_name: str, members: typing.List[str]
-) -> typing.List[str]:
+def _group_add_members_cmd(group_name: str, members: list[str]) -> list[str]:
     cmd = samba_cmds.sambatool[
         "group",
         "addmembers",
         group_name,
         ",".join(members),
     ].argv()
     return cmd
```

### Comparing `sambacc-0.2/sambacc/commands/addc.py` & `sambacc-0.3/sambacc/commands/addc.py`

 * *Files identical despite different names*

### Comparing `sambacc-0.2/sambacc/commands/check.py` & `sambacc-0.3/sambacc/commands/check.py`

 * *Files identical despite different names*

### Comparing `sambacc-0.2/sambacc/commands/cli.py` & `sambacc-0.3/sambacc/commands/cli.py`

 * *Files 12% similar despite different names*

```diff
@@ -35,20 +35,31 @@
 _logger = logging.getLogger(__name__)
 
 
 class Fail(ValueError):
     pass
 
 
+class Parser(typing.Protocol):
+    def frank(self, x: str) -> str:
+        ...  # pragma: no cover
+
+    def set_defaults(self, **kwargs: typing.Any) -> None:
+        ...  # pragma: no cover
+
+    def add_argument(
+        self, *args: typing.Any, **kwargs: typing.Any
+    ) -> typing.Any:
+        ...  # pragma: no cover
+
+
 Command = namedtuple("Command", "name cmd_func arg_func cmd_help")
 
 
-def toggle_option(
-    parser: argparse.ArgumentParser, arg: str, dest: str, helpfmt: str
-) -> argparse.ArgumentParser:
+def toggle_option(parser: Parser, arg: str, dest: str, helpfmt: str) -> Parser:
     parser.add_argument(
         arg,
         action="store_true",
         dest=dest,
         help=helpfmt.format("Enable"),
     )
     negarg = arg.replace("--", "--no-")
@@ -65,15 +76,15 @@
     if cmd.cmd_help is not None:
         return cmd.cmd_help
     if cmd.cmd_func.__doc__:
         return cmd.cmd_func.__doc__
     return ""
 
 
-def add_command(subparsers, cmd) -> None:
+def add_command(subparsers: typing.Any, cmd: Command) -> None:
     subparser = subparsers.add_parser(cmd.name, help=get_help(cmd))
     subparser.set_defaults(cfunc=cmd.cmd_func)
     if cmd.arg_func is not None:
         cmd.arg_func(subparser)
 
 
 class CommandBuilder:
@@ -92,24 +103,26 @@
                     name=name, cmd_func=f, arg_func=arg_func, cmd_help=cmd_help
                 )
             )
             return f
 
         return _wrapper
 
-    def assemble(self, arg_func=None) -> argparse.ArgumentParser:
+    def assemble(
+        self, arg_func: typing.Optional[typing.Callable] = None
+    ) -> argparse.ArgumentParser:
         parser = argparse.ArgumentParser()
         if arg_func is not None:
             arg_func(parser)
         subparsers = parser.add_subparsers()
         for cmd in self._commands:
             add_command(subparsers, cmd)
         return parser
 
-    def dict(self) -> typing.Dict[str, Command]:
+    def dict(self) -> dict[str, Command]:
         """Return a dict mapping command names to Command object."""
         return {c.name: c for c in self._commands}
 
 
 class Context(typing.Protocol):
     """Protocol type for CLI Context.
     Used to share simple, common state, derived from the CLI, across individual
@@ -124,14 +137,18 @@
     def cli(self) -> argparse.Namespace:
         ...  # pragma: no cover
 
     @property
     def instance_config(self) -> config.InstanceConfig:
         ...  # pragma: no cover
 
+    @property
+    def require_validation(self) -> typing.Optional[bool]:
+        ...  # pragma: no cover
+
 
 def best_waiter(
     filename: typing.Optional[str] = None,
     max_timeout: typing.Optional[int] = None,
 ) -> simple_waiter.Waiter:
     """Fetch the best waiter type for our sambacc command."""
     if filename and _INOTIFY_OK:
```

### Comparing `sambacc-0.2/sambacc/commands/config.py` & `sambacc-0.3/sambacc/commands/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,15 +68,17 @@
         action="store_true",
         help=("If set, watch the source for changes and update config."),
     )
 
 
 def _read_config(ctx: Context) -> config.InstanceConfig:
     cfgs = ctx.cli.config or []
-    return config.read_config_files(cfgs).get(ctx.cli.identity)
+    return config.read_config_files(
+        cfgs, require_validation=ctx.require_validation
+    ).get(ctx.cli.identity)
 
 
 def _update_config(
     current: config.InstanceConfig,
     previous: typing.Optional[config.InstanceConfig],
     ensure_paths: bool = True,
     notify_server: bool = True,
@@ -112,26 +114,28 @@
 
 
 def _exec_if_leader(
     ctx: Context,
     cond_func: typing.Callable[..., typing.Tuple[config.InstanceConfig, bool]],
 ) -> typing.Callable[..., typing.Tuple[config.InstanceConfig, bool]]:
     """Run the cond func only on "nodes" that are the cluster leader."""
+
     # CTDB status and leader detection is not changeable at runtime.
     # we do not need to account for it changing in the updated config file(s)
     @functools.wraps(cond_func)
     def _call_if_leader(
         current: config.InstanceConfig, previous: config.InstanceConfig
     ) -> typing.Tuple[config.InstanceConfig, bool]:
         with best_leader_locator(ctx.instance_config) as ll:
             if not ll.is_leader():
                 _logger.info("skipping config update. node not leader")
                 return previous, False
             _logger.info("checking for update. node is leader")
-            return cond_func(current, previous)
+            result = cond_func(current, previous)
+        return result
 
     return _call_if_leader
 
 
 @commands.command(name="update-config", arg_func=_update_config_args)
 def update_config(ctx: Context) -> None:
     _get_config = functools.partial(_read_config, ctx)
```

### Comparing `sambacc-0.2/sambacc/commands/ctdb.py` & `sambacc-0.3/sambacc/commands/ctdb.py`

 * *Files identical despite different names*

### Comparing `sambacc-0.2/sambacc/commands/dcmain.py` & `sambacc-0.3/sambacc/commands/dcmain.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,14 +12,16 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>
 #
 
+import typing
+
 from . import addc
 from .cli import Fail
 from .main import (
     CommandContext,
     action_filter,
     enable_logging,
     env_to_cli,
@@ -27,15 +29,15 @@
     pre_action,
 )
 
 
 default_cfunc = addc.summary
 
 
-def main(args=None) -> None:
+def main(args: typing.Optional[typing.Sequence[str]] = None) -> None:
     cli = addc.dccommands.assemble(arg_func=global_args).parse_args(args)
     env_to_cli(cli)
     enable_logging(cli)
     if not cli.identity:
         raise Fail("missing container identity")
 
     pre_action(cli)
```

### Comparing `sambacc-0.2/sambacc/commands/dns.py` & `sambacc-0.3/sambacc/commands/dns.py`

 * *Files 4% similar despite different names*

```diff
@@ -87,16 +87,17 @@
 
 
 def _exec_if_leader(iconfig, update_func):
     def leader_update_func(
         domain: str,
         source: str,
         previous: typing.Optional[container_dns.HostState] = None,
-    ):
+    ) -> typing.Tuple[typing.Optional[container_dns.HostState], bool]:
         with best_leader_locator(iconfig) as ll:
             if not ll.is_leader():
                 _logger.info("skipping dns update. node not leader")
                 return previous, False
             _logger.info("checking for update. node is leader")
-            return update_func(domain, source, previous)
+            result = update_func(domain, source, previous)
+        return result
 
     return leader_update_func
```

### Comparing `sambacc-0.2/sambacc/commands/initialize.py` & `sambacc-0.3/sambacc/commands/initialize.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>
 #
 
 import logging
+import typing
 
 from sambacc import ctdb
 from sambacc import paths
 import sambacc.nsswitch_loader as nsswitch
 
 from . import config  # noqa: F401
 from . import users  # noqa: F401
@@ -101,13 +102,15 @@
 
 def setup_step_names():
     """Return a list of names for the steps that init supports."""
     return list(setup_steps.dict().keys())
 
 
 @commands.command(name="init")
-def init_container(ctx: Context, steps=None) -> None:
+def init_container(
+    ctx: Context, steps: typing.Optional[typing.Iterable[str]] = None
+) -> None:
     """Initialize the entire container environment."""
     steps = _default_setup_steps if steps is None else list(steps)
     cmds = setup_steps.dict()
     for step_name in steps:
         cmds[step_name].cmd_func(ctx)
```

### Comparing `sambacc-0.2/sambacc/commands/join.py` & `sambacc-0.3/sambacc/commands/join.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,39 +13,47 @@
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>
 #
 
 import sys
+import typing
 
 import sambacc.join as joinutil
 
-from .cli import commands, Context, toggle_option, best_waiter, Fail
+from .cli import (
+    Context,
+    Fail,
+    Parser,
+    best_waiter,
+    commands,
+    toggle_option,
+)
 
 
-def _print_join_error(err) -> None:
+def _print_join_error(err: typing.Any) -> None:
     print(f"ERROR: {err}", file=sys.stderr)
     for suberr in getattr(err, "errors", []):
         print(f"  - {suberr}", file=sys.stderr)
 
 
-def _add_join_sources(joiner, cli) -> None:
+def _add_join_sources(joiner: joinutil.Joiner, cli: typing.Any) -> None:
     if cli.insecure or getattr(cli, "insecure_auto_join", False):
         upass = joinutil.UserPass(cli.username, cli.password)
         joiner.add_source(joinutil.JoinBy.PASSWORD, upass)
     if cli.files:
         for path in cli.join_files or []:
             joiner.add_source(joinutil.JoinBy.FILE, path)
     if cli.interactive:
         upass = joinutil.UserPass(cli.username)
         joiner.add_source(joinutil.JoinBy.INTERACTIVE, upass)
 
 
-def _join_args(parser) -> None:
+def _join_args(parser: Parser) -> None:
     parser.set_defaults(insecure=False, files=True, interactive=True)
     toggle_option(
         parser,
         arg="--insecure",
         dest="insecure",
         helpfmt="{} taking user/password from CLI or environment.",
     )
@@ -84,15 +92,15 @@
     try:
         joiner.join()
     except joinutil.JoinError as err:
         _print_join_error(err)
         raise Fail("failed to join to a domain")
 
 
-def _must_join_args(parser) -> None:
+def _must_join_args(parser: Parser) -> None:
     parser.set_defaults(insecure=False, files=True, wait=True)
     toggle_option(
         parser,
         arg="--insecure",
         dest="insecure",
         helpfmt="{} taking user/password from CLI or environment.",
     )
```

### Comparing `sambacc-0.2/sambacc/commands/main.py` & `sambacc-0.3/sambacc/commands/main.py`

 * *Files 12% similar despite different names*

```diff
@@ -29,23 +29,23 @@
 from . import config as config_cmds
 from . import ctdb  # noqa: F401
 from . import dns  # noqa: F401
 from . import initialize  # noqa: F401
 from . import join  # noqa: F401
 from . import run  # noqa: F401
 from . import users  # noqa: F401
-from .cli import commands, Fail
+from .cli import commands, Fail, Parser
 
 DEFAULT_CONFIG = "/etc/samba/container/config.json"
 DEFAULT_JOIN_MARKER = "/var/lib/samba/container-join-marker.json"
 
 default_cfunc = config_cmds.print_config
 
 
-def global_args(parser) -> None:
+def global_args(parser: Parser) -> None:
     parser.add_argument(
         "--config",
         action="append",
         help=(
             "Specify source configuration"
             " (can also be set in the environment by SAMBACC_CONFIG)."
         ),
@@ -95,17 +95,28 @@
         help="Wrap samba commands within a supplied command prefix",
     )
     parser.add_argument(
         "--skip-if-file",
         action="append",
         help=("Perform no action if the specified path exists."),
     )
+    parser.add_argument(
+        "--validate-config",
+        choices=("auto", "required", "true", "false"),
+        help=("Perform schema based validation of configuration."),
+    )
 
 
-def from_env(ns, var, ename, default=None, vtype=str) -> None:
+def from_env(
+    ns: typing.Any,
+    var: str,
+    ename: str,
+    default: typing.Any = None,
+    vtype: typing.Optional[typing.Callable] = str,
+) -> None:
     value = getattr(ns, var, None)
     if not value:
         value = os.environ.get(ename, "")
     if vtype is not None:
         value = vtype(value)
     if value:
         setattr(ns, var, value)
@@ -119,15 +130,15 @@
     out = []
     for v in value:
         for part in v.split(":"):
             out.append(part)
     return out
 
 
-def env_to_cli(cli) -> None:
+def env_to_cli(cli: typing.Any) -> None:
     from_env(
         cli,
         "config",
         "SAMBACC_CONFIG",
         vtype=split_paths,
         default=DEFAULT_CONFIG,
     )
@@ -137,14 +148,15 @@
         "SAMBACC_JOIN_FILES",
         vtype=split_paths,
     )
     from_env(cli, "identity", "SAMBA_CONTAINER_ID")
     from_env(cli, "username", "JOIN_USERNAME")
     from_env(cli, "password", "INSECURE_JOIN_PASSWORD")
     from_env(cli, "samba_debug_level", "SAMBA_DEBUG_LEVEL")
+    from_env(cli, "validate_config", "SAMBACC_VALIDATE_CONFIG")
 
 
 class CommandContext:
     """CLI Context for standard samba-container commands."""
 
     def __init__(self, cli_args: argparse.Namespace):
         self._cli = cli_args
@@ -155,51 +167,59 @@
     def cli(self) -> argparse.Namespace:
         return self._cli
 
     @property
     def instance_config(self) -> config.InstanceConfig:
         if self._iconfig is None:
             cfgs = self.cli.config or []
-            self._iconfig = config.read_config_files(cfgs).get(
-                self.cli.identity
-            )
+            self._iconfig = config.read_config_files(
+                cfgs, require_validation=self.require_validation
+            ).get(self.cli.identity)
         return self._iconfig
 
+    @property
+    def require_validation(self) -> typing.Optional[bool]:
+        if self.cli.validate_config in ("required", "true"):
+            return True
+        if self.cli.validate_config == "false":
+            return False
+        return None
+
 
-def pre_action(cli) -> None:
+def pre_action(cli: typing.Any) -> None:
     """Handle debugging/diagnostic related options before the target
     action of the command is performed.
     """
     if cli.debug_delay:
         time.sleep(int(cli.debug_delay))
     if cli.samba_debug_level:
         samba_cmds.set_global_debug(cli.samba_debug_level)
     if cli.samba_command_prefix:
         samba_cmds.set_global_prefix([cli.samba_command_prefix])
 
 
-def enable_logging(cli) -> None:
+def enable_logging(cli: typing.Any) -> None:
     logger = logging.getLogger()
     logger.setLevel(logging.INFO)
     handler = logging.StreamHandler()
     handler.setFormatter(
         logging.Formatter("{asctime}: {levelname}: {message}", style="{")
     )
     handler.setLevel(logging.INFO)
     logger.addHandler(handler)
 
 
-def action_filter(cli) -> typing.Optional[str]:
+def action_filter(cli: typing.Any) -> typing.Optional[str]:
     for path in cli.skip_if_file or []:
         if os.path.exists(path):
             return f"skip-if-file: {path} exists"
     return None
 
 
-def main(args=None) -> None:
+def main(args: typing.Optional[typing.Sequence[str]] = None) -> None:
     cli = commands.assemble(arg_func=global_args).parse_args(args)
     env_to_cli(cli)
     enable_logging(cli)
     if not cli.identity:
         raise Fail("missing container identity")
 
     pre_action(cli)
```

### Comparing `sambacc-0.2/sambacc/commands/run.py` & `sambacc-0.3/sambacc/commands/run.py`

 * *Files identical despite different names*

### Comparing `sambacc-0.2/sambacc/commands/users.py` & `sambacc-0.3/sambacc/commands/users.py`

 * *Files identical despite different names*

### Comparing `sambacc-0.2/sambacc/config.py` & `sambacc-0.3/sambacc/config.py`

 * *Files 24% similar despite different names*

```diff
@@ -15,92 +15,217 @@
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>
 #
 
 from __future__ import annotations
 
 import binascii
+import enum
 import errno
 import json
+import sys
 import typing
 
 _VALID_VERSIONS = ["v0"]
 
 # alias open to _open to support test assertions when running
 # as UID 0
 _open = open
 
 PasswdEntryTuple = typing.Tuple[str, str, str, str, str, str, str]
 GroupEntryTuple = typing.Tuple[str, str, str, str]
 
+# JSONData is not really a completely valid representation of json in
+# the type system, but it's good enough for now. Using it can help
+# clarify what works with json and what works with real python dicts.
+JSONData = dict[str, typing.Any]
+
 # the standard location for samba's smb.conf
 SMB_CONF = "/etc/samba/smb.conf"
 
 CTDB: typing.Final[str] = "ctdb"
 ADDC: typing.Final[str] = "addc"
 FEATURES: typing.Final[str] = "instance_features"
 
+# cache for json schema data
+_JSON_SCHEMA: dict[str, typing.Any] = {}
+
+
+class ConfigFormat(enum.Enum):
+    JSON = "json"
+    TOML = "toml"
+    YAML = "yaml"
+
+
+class ValidationUnsupported(Exception):
+    pass
+
+
+class _FakeRefResolutionError(Exception):
+    pass
+
+
+class ConfigFormatUnsupported(Exception):
+    pass
+
+
+if sys.version_info >= (3, 11):
+
+    def _load_toml(source: typing.IO) -> JSONData:
+        try:
+            import tomllib
+        except ImportError:
+            raise ConfigFormatUnsupported(ConfigFormat.TOML)
+        return tomllib.load(source)
+
+else:
+
+    def _load_toml(source: typing.IO) -> JSONData:
+        try:
+            import tomli
+        except ImportError:
+            raise ConfigFormatUnsupported(ConfigFormat.TOML)
+        if typing.TYPE_CHECKING:
+            assert isinstance(source, typing.BinaryIO)
+        return tomli.load(source)
+
+
+def _load_yaml(source: typing.IO) -> JSONData:
+    try:
+        import yaml
+    except ImportError:
+        raise ConfigFormatUnsupported(ConfigFormat.YAML)
+    return yaml.safe_load(source) or {}
+
+
+def _detect_format(fname: str) -> ConfigFormat:
+    if fname.endswith(".toml"):
+        return ConfigFormat.TOML
+    if fname.endswith((".yaml", ".yml")):
+        return ConfigFormat.YAML
+    return ConfigFormat.JSON
+
+
+def _schema_validate(data: dict[str, typing.Any], version: str) -> None:
+    try:
+        import jsonschema  # type: ignore[import]
+    except ImportError:
+        raise ValidationUnsupported()
+    try:
+        _refreserror = getattr(jsonschema, "RefResolutionError")
+    except AttributeError:
+        _refreserror = _FakeRefResolutionError
+
+    global _JSON_SCHEMA
+    if version == "v0" and version not in _JSON_SCHEMA:
+        try:
+            import sambacc.schema.conf_v0_schema
+
+            _JSON_SCHEMA[version] = sambacc.schema.conf_v0_schema.SCHEMA
+        except ImportError:
+            raise ValidationUnsupported()
+    try:
+        jsonschema.validate(instance=data, schema=_JSON_SCHEMA[version])
+    except _refreserror:
+        raise ValidationUnsupported()
+
+
+def _check_config_version(data: JSONData) -> str:
+    """Return the config data or raise a ValueError if the config
+    is invalid or incomplete.
+    """
+    # short-cut to validate that this is something we want to consume
+    version = data.get("samba-container-config")
+    if version is None:
+        raise ValueError("Invalid config: no samba-container-config key")
+    elif version not in _VALID_VERSIONS:
+        raise ValueError(f"Invalid config: unknown version {version}")
+    return version
+
+
+def _check_config_valid(
+    data: JSONData, version: str, required: typing.Optional[bool] = None
+) -> None:
+    if required or required is None:
+        try:
+            _schema_validate(data, version)
+        except ValidationUnsupported:
+            if required:
+                raise
+
 
-def read_config_files(fnames) -> GlobalConfig:
+def read_config_files(
+    fnames: list[str], *, require_validation: typing.Optional[bool] = None
+) -> GlobalConfig:
     """Read the global container config from the given filenames.
     At least one of the files from the fnames list must exist and contain
     a valid config. If none of the file names exist an error will be raised.
     """
     # NOTE: Right now if more than one config exists they'll be "merged" but
     # the merging is very simplistic right now. Mainly we expect that the
     # users will be split from the main config (for security reasons) but
     # it would be nicer to have a good merge algorithm handle everything
     # smarter at some point.
     gconfig = GlobalConfig()
     readfiles = set()
     for fname in fnames:
+        config_format = _detect_format(str(fname))
         try:
-            with _open(fname) as fh:
-                gconfig.load(fh)
+            with _open(fname, "rb") as fh:
+                gconfig.load(
+                    fh,
+                    require_validation=require_validation,
+                    config_format=config_format,
+                )
             readfiles.add(fname)
         except OSError as err:
             if getattr(err, "errno", 0) != errno.ENOENT:
                 raise
     if not readfiles:
         # we read nothing! don't proceed
         raise ValueError(f"None of the config file paths exist: {fnames}")
-    # Verify that we loaded something
-    check_config_data(gconfig.data)
     return gconfig
 
 
-def check_config_data(data) -> dict:
-    """Return the config data or raise a ValueError if the config
-    is invalid or incomplete.
-    """
-    # short-cut to validate that this is something we want to consume
-    version = data.get("samba-container-config")
-    if version is None:
-        raise ValueError("Invalid config: no samba-container-config key")
-    elif version not in _VALID_VERSIONS:
-        raise ValueError(f"Invalid config: unknown version {version}")
-    return data
-
-
 class SambaConfig(typing.Protocol):
     def global_options(self) -> typing.Iterable[typing.Tuple[str, str]]:
         ...  # pragma: no cover
 
     def shares(self) -> typing.Iterable[ShareConfig]:
         ...  # pragma: no cover
 
 
 class GlobalConfig:
-    def __init__(self, source=None):
-        self.data = {}
+    def __init__(
+        self,
+        source: typing.Optional[typing.IO] = None,
+        *,
+        initial_data: typing.Optional[JSONData] = None,
+    ) -> None:
+        self.data: JSONData = {} if initial_data is None else initial_data
         if source is not None:
             self.load(source)
 
-    def load(self, source: typing.IO) -> None:
-        data = check_config_data(json.load(source))
+    def load(
+        self,
+        source: typing.IO,
+        *,
+        require_validation: typing.Optional[bool] = None,
+        config_format: typing.Optional[ConfigFormat] = None,
+    ) -> None:
+        config_format = config_format or ConfigFormat.JSON
+        if config_format == ConfigFormat.TOML:
+            data = _load_toml(source)
+        elif config_format == ConfigFormat.YAML:
+            data = _load_yaml(source)
+        else:
+            data = json.load(source)
+        _check_config_valid(
+            data, _check_config_version(data), require_validation
+        )
         self.data.update(data)
 
     def get(self, ident: str) -> InstanceConfig:
         iconfig = self.data["configs"][ident]
         return InstanceConfig(self, iconfig)
 
 
@@ -158,15 +283,15 @@
         return ADDC in self.iconfig.get(FEATURES, [])
 
     def ctdb_smb_config(self) -> CTDBSambaConfig:
         if not self.with_ctdb:
             raise ValueError("ctdb not supported in configuration")
         return CTDBSambaConfig()
 
-    def ctdb_config(self) -> typing.Dict[str, str]:
+    def ctdb_config(self) -> dict[str, str]:
         """Common configuration of CTDB itself."""
         if not self.with_ctdb:
             return {}
         ctdb = dict(self.gconfig.data.get("ctdb", {}))
         ctdb.setdefault("nodes_json", "/var/lib/ctdb/shared/ctdb-nodes.json")
         ctdb.setdefault("nodes_path", "/var/lib/ctdb/shared/nodes")
         ctdb.setdefault("recovery_lock", "/var/lib/ctdb/shared/RECOVERY")
```

### Comparing `sambacc-0.2/sambacc/container_dns.py` & `sambacc-0.3/sambacc/container_dns.py`

 * *Files 24% similar despite different names*

```diff
@@ -12,80 +12,95 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>
 #
 
+from __future__ import annotations
+
 import json
 import subprocess
 import typing
 
 from sambacc import samba_cmds
 
 EXTERNAL: str = "external"
 INTERNAL: str = "internal"
 
 
 class HostState:
-    def __init__(self, ref="", items=[]):
-        self.ref = ref
-        self.items = items
+    T = typing.TypeVar("T", bound="HostState")
+
+    def __init__(
+        self, ref: str = "", items: typing.Optional[list[HostInfo]] = None
+    ) -> None:
+        self.ref: str = ref
+        self.items: list[HostInfo] = items or []
 
     @classmethod
-    def from_dict(cls, d):
+    def from_dict(cls: typing.Type[T], d: dict[str, typing.Any]) -> T:
         return cls(
             ref=d["ref"],
             items=[HostInfo.from_dict(i) for i in d.get("items", [])],
         )
 
-    def __eq__(self, other):
+    def __eq__(self, other: typing.Any) -> bool:
         return (
             self.ref == other.ref
             and len(self.items) == len(other.items)
             and all(s == o for (s, o) in zip(self.items, other.items))
         )
 
 
 class HostInfo:
-    def __init__(self, name="", ipv4_addr="", target=""):
+    T = typing.TypeVar("T", bound="HostInfo")
+
+    def __init__(
+        self, name: str = "", ipv4_addr: str = "", target: str = ""
+    ) -> None:
         self.name = name
         self.ipv4_addr = ipv4_addr
         self.target = target
 
     @classmethod
-    def from_dict(cls, d):
+    def from_dict(cls: typing.Type[T], d: dict[str, typing.Any]) -> T:
         return cls(
             name=d["name"],
             ipv4_addr=d["ipv4"],
             target=d.get("target", ""),
         )
 
-    def __eq__(self, other):
+    def __eq__(self, other: typing.Any) -> bool:
         return (
             self.name == other.name
             and self.ipv4_addr == other.ipv4_addr
             and self.target == other.target
         )
 
 
-def parse(fh):
+def parse(fh: typing.IO) -> HostState:
     return HostState.from_dict(json.load(fh))
 
 
-def parse_file(path):
+def parse_file(path: str) -> HostState:
     with open(path) as fh:
         return parse(fh)
 
 
-def match_target(state: HostState, target_name: str) -> typing.List[HostInfo]:
+def match_target(state: HostState, target_name: str) -> list[HostInfo]:
     return [h for h in state.items if h.target == target_name]
 
 
-def register(domain, hs, prefix=None, target_name: str = EXTERNAL) -> bool:
+def register(
+    domain: str,
+    hs: HostState,
+    prefix: typing.Optional[list[str]] = None,
+    target_name: str = EXTERNAL,
+) -> bool:
     updated = False
     for item in match_target(hs, target_name):
         ip = item.ipv4_addr
         fqdn = "{}.{}".format(item.name, domain)
         cmd = samba_cmds.net["ads", "-P", "dns", "register", fqdn, ip]
         if prefix is not None:
             cmd.cmd_prefix = prefix
@@ -95,32 +110,39 @@
 
 
 def parse_and_update(
     domain: str,
     source: str,
     previous: typing.Optional[HostState] = None,
     target_name: str = EXTERNAL,
-    reg_func=register,
+    reg_func: typing.Callable = register,
 ) -> typing.Tuple[HostState, bool]:
     hs = parse_file(source)
     if previous is not None and hs == previous:
         # no changes
         return hs, False
     updated = reg_func(domain, hs, target_name=target_name)
     return hs, updated
 
 
 # TODO: replace this with the common version added to simple_waiter
-def watch(domain, source, update_func, pause_func, print_func=None):
+def watch(
+    domain: str,
+    source: str,
+    update_func: typing.Callable,
+    pause_func: typing.Callable,
+    print_func: typing.Optional[typing.Callable],
+) -> None:
     previous = None
     while True:
         try:
             previous, updated = update_func(domain, source, previous)
         except FileNotFoundError:
-            print_func(f"Source file [{source}] not found")
+            if print_func:
+                print_func(f"Source file [{source}] not found")
             updated = False
             previous = None
         if updated and print_func:
             print_func("Updating external dns registrations")
         try:
             pause_func()
         except KeyboardInterrupt:
```

### Comparing `sambacc-0.2/sambacc/ctdb.py` & `sambacc-0.3/sambacc/ctdb.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 import subprocess
 import typing
 
 from sambacc import config
 from sambacc import jfile
 from sambacc import samba_cmds
 from sambacc.netcmd_loader import template_config
+from sambacc.typelets import ExcType, ExcValue, ExcTraceback
 
 _logger = logging.getLogger(__name__)
 
 
 DB_DIR = "/var/lib/ctdb/persistent"
 ETC_DIR = "/etc/ctdb"
 SHARE_DIR = "/usr/share/ctdb"
@@ -53,15 +54,19 @@
         return NodeState.REPLACED
     elif state == NodeState.REPLACED:
         return NodeState.READY
     return state
 
 
 class NodeNotPresent(KeyError):
-    def __init__(self, identity, pnn=None):
+    def __init__(
+        self,
+        identity: typing.Any,
+        pnn: typing.Optional[typing.Union[str, int]] = None,
+    ) -> None:
         super().__init__(identity)
         self.identity = identity
         self.pnn = pnn
 
 
 def ensure_smb_conf(
     iconfig: config.InstanceConfig, path: str = config.SMB_CONF
@@ -80,15 +85,17 @@
     iconfig: config.InstanceConfig, path: str = CTDB_CONF
 ) -> None:
     """Ensure that the ctdb.conf on disk matches our desired state."""
     with open(path, "w") as fh:
         write_ctdb_conf(fh, iconfig.ctdb_config())
 
 
-def write_ctdb_conf(fh: typing.IO, ctdb_params: typing.Dict, enc=str) -> None:
+def write_ctdb_conf(
+    fh: typing.IO, ctdb_params: dict, enc: typing.Callable = str
+) -> None:
     """Write a ctdb.conf style output."""
 
     def _write_param(fh: typing.IO, name: str, key: str) -> None:
         value = ctdb_params.get(key)
         if value is None:
             return
         fh.write(enc(f"{name} = {value}\n"))
@@ -102,15 +109,15 @@
     fh.write(enc("[legacy]\n"))
     _write_param(fh, "realtime scheduling", "realtime_scheduling")
     _write_param(fh, "script log level", "script_log_level")
     fh.write(enc("\n"))
 
 
 def ensure_ctdb_nodes(
-    ctdb_nodes: typing.List[str], real_path: str, canon_path: str = CTDB_NODES
+    ctdb_nodes: list[str], real_path: str, canon_path: str = CTDB_NODES
 ) -> None:
     """Ensure a real nodes file exists, containing the specificed content,
     and has a symlink in the proper place for ctdb.
     """
     try:
         os.unlink(canon_path)
     except FileNotFoundError:
@@ -118,30 +125,30 @@
     os.symlink(real_path, canon_path)
     # XXX: add locking?
     with open(real_path, "w") as fh:
         write_nodes_file(fh, ctdb_nodes)
 
 
 def write_nodes_file(
-    fh: typing.IO, ctdb_nodes: typing.List[str], enc=str
+    fh: typing.IO, ctdb_nodes: list[str], enc: typing.Callable = str
 ) -> None:
     """Write the ctdb nodes file."""
     for node in ctdb_nodes:
         fh.write(enc(f"{node}\n"))
 
 
-def read_nodes_file(fh: typing.IO) -> typing.List[str]:
+def read_nodes_file(fh: typing.IO) -> list[str]:
     """Read content from an open ctdb nodes file."""
     entries = []
     for line in fh:
         entries.append(line.strip())
     return entries
 
 
-def read_ctdb_nodes(path: str = CTDB_NODES) -> typing.List[str]:
+def read_ctdb_nodes(path: str = CTDB_NODES) -> list[str]:
     """Read the content of the ctdb nodes file."""
     try:
         with open(path, "r") as fh:
             entries = read_nodes_file(fh)
     except FileNotFoundError:
         return []
     return entries
@@ -194,15 +201,19 @@
         jfile.flock(fh)
         data = jfile.load(fh, {})
         _refresh_statefile(data, identity, node, pnn)
         jfile.dump(data, fh)
 
 
 def _update_statefile(
-    data, identity: str, node: str, pnn: int, in_nodes: bool = False
+    data: dict[str, typing.Any],
+    identity: str,
+    node: str,
+    pnn: int,
+    in_nodes: bool = False,
 ) -> None:
     data.setdefault("nodes", [])
     for entry in data["nodes"]:
         if pnn == entry["pnn"]:
             raise ValueError("duplicate pnn")
         if identity == entry["identity"]:
             raise ValueError("duplicate identity")
@@ -216,15 +227,19 @@
             "pnn": pnn,
             "state": state,
         }
     )
 
 
 def _refresh_statefile(
-    data, identity: str, node: str, pnn: int, in_nodes: bool = False
+    data: dict[str, typing.Any],
+    identity: str,
+    node: str,
+    pnn: int,
+    in_nodes: bool = False,
 ) -> None:
     data.setdefault("nodes", [])
     node_entry = None
     for entry in data["nodes"]:
         if pnn == entry["pnn"] and identity == entry["identity"]:
             node_entry = entry
             break
@@ -237,19 +252,19 @@
     if node_entry["node"] == node:
         # do nothing
         return
     node_entry["node"] = node
     node_entry["state"] = NodeState.CHANGED
 
 
-def _get_state(entry) -> NodeState:
+def _get_state(entry: dict[str, typing.Any]) -> NodeState:
     return NodeState(entry["state"])
 
 
-def _get_state_ok(entry) -> bool:
+def _get_state_ok(entry: dict[str, typing.Any]) -> bool:
     return _get_state(entry) == NodeState.READY
 
 
 def pnn_in_nodes(pnn: int, nodes_json: str, real_path: str) -> bool:
     """Returns true if the specified pnn has an entry in the nodes json
     file and that the node is already added to the ctdb nodes file.
     """
@@ -260,15 +275,18 @@
         for entry in current_nodes:
             if pnn == entry["pnn"] and _get_state_ok(entry):
                 return True
     return False
 
 
 def manage_nodes(
-    pnn: int, nodes_json: str, real_path: str, pause_func
+    pnn: int,
+    nodes_json: str,
+    real_path: str,
+    pause_func: typing.Callable,
 ) -> None:
     """Monitor nodes json for updates, reflecting those changes into ctdb."""
     while True:
         _logger.info("checking if node is able to make updates")
         if _node_check(pnn, nodes_json, real_path):
             _logger.info("checking for node updates")
             if _node_update(nodes_json, real_path):
@@ -294,15 +312,17 @@
         # this current node is not in the nodes file.
         # it is ineligible to make changes to the nodes file
         return False
     # this node is already in the nodes file!
     return True
 
 
-def _node_update_check(json_data, nodes_json: str, real_path: str):
+def _node_update_check(
+    json_data: dict[str, typing.Any], nodes_json: str, real_path: str
+) -> tuple[list[str], list[typing.Any], list[typing.Any]]:
     desired = json_data.get("nodes", [])
     ctdb_nodes = read_ctdb_nodes(real_path)
     update_nodes = []
     need_reload = []
     _update_states = (NodeState.NEW, NodeState.CHANGED, NodeState.REPLACED)
     for entry in desired:
         pnn = entry["pnn"]
@@ -320,23 +340,23 @@
         else:
             # node present but state indicates
             # update is not finalized
             need_reload.append(entry)
     return ctdb_nodes, update_nodes, need_reload
 
 
-def _node_line(ctdb_nodes, pnn) -> str:
+def _node_line(ctdb_nodes: list[str], pnn: int) -> str:
     try:
         return ctdb_nodes[pnn]
     except IndexError:
         return ""
 
 
-def _entry_to_node(ctdb_nodes, entry) -> str:
-    pnn = entry["pnn"]
+def _entry_to_node(ctdb_nodes: list[str], entry: dict[str, typing.Any]) -> str:
+    pnn: int = entry["pnn"]
     if entry["state"] == NodeState.CHANGED:
         return "#{}".format(ctdb_nodes[pnn].strip("#"))
     return entry["node"]
 
 
 def _node_update(nodes_json: str, real_path: str) -> bool:
     # open r/o so that we don't initailly open for write.  we do a probe and
@@ -479,15 +499,15 @@
     orig_name = os.path.basename(tdb_path)
     opath = os.path.join(dest_dir, f"{orig_name}.{pnn}")
     _logger.info(f"Converting {tdb_path} to {opath} ...")
     cmd = samba_cmds.ltdbtool["convert", "-s0", tdb_path, opath]
     subprocess.check_call(list(cmd))
 
 
-def check_nodestatus(cmd: samba_cmds.SambaCommand = samba_cmds.ctdb):
+def check_nodestatus(cmd: samba_cmds.SambaCommand = samba_cmds.ctdb) -> None:
     cmd_ctdb_check = cmd["nodestatus"]
     samba_cmds.execute(cmd_ctdb_check)
 
 
 class CLILeaderStatus:
     _isleader = False
 
@@ -507,23 +527,26 @@
         try:
             out = subprocess.check_output(list(pnn_cmd))
             mypnn = out.decode("utf8").strip()
         except subprocess.CalledProcessError as err:
             _logger.error(f"command {pnn_cmd!r} failed: {err!r}")
         except FileNotFoundError:
             _logger.error(f"ctdb command ({pnn_cmd!r}) not found")
-        # recmaster = <ctdb recmaster>
-        recmaster_cmd = samba_cmds.ctdb["recmaster"]
+        # recmaster = <ctdb recmaster|leader>
+        admin_cmd = samba_cmds.ctdb_leader_admin_cmd()
+        recmaster_cmd = samba_cmds.ctdb[admin_cmd]
         try:
             out = subprocess.check_output(list(recmaster_cmd))
             recmaster = out.decode("utf8").strip()
         except subprocess.CalledProcessError as err:
             _logger.error(f"command {recmaster_cmd!r} failed: {err!r}")
         except FileNotFoundError:
             _logger.error(f"ctdb command ({recmaster_cmd!r}) not found")
 
         sts = CLILeaderStatus()
         sts._isleader = bool(mypnn) and mypnn == recmaster
         return sts
 
-    def __exit__(self, exc_type, exc_val, exc_tb) -> None:
-        pass
+    def __exit__(
+        self, exc_type: ExcType, exc_val: ExcValue, exc_tb: ExcTraceback
+    ) -> bool:
+        return True
```

### Comparing `sambacc-0.2/sambacc/inotify_waiter.py` & `sambacc-0.3/sambacc/inotify_waiter.py`

 * *Files 7% similar despite different names*

```diff
@@ -33,16 +33,19 @@
     A `print_func` can be specified as a simple logging method.
     """
 
     timeout: int = DEFAULT_TIMEOUT
     print_func = None
 
     def __init__(
-        self, path: str, print_func=None, timeout: typing.Optional[int] = None
-    ):
+        self,
+        path: str,
+        print_func: typing.Optional[typing.Callable] = None,
+        timeout: typing.Optional[int] = None,
+    ) -> None:
         if timeout is not None:
             self.timeout = timeout
         self.print_func = print_func
         self._inotify = _inotify.INotify()
         dirpath, fpath = os.path.split(path)
         if not dirpath:
             dirpath = "."
@@ -62,15 +65,15 @@
 
     def acted(self) -> None:
         return  # noop for inotify waiter
 
     def wait(self) -> None:
         next(self._wait())
 
-    def _get_events(self):
+    def _get_events(self) -> list[typing.Any]:
         timeout = 1000 * self.timeout
         self._print("waiting {}ms for activity...".format(timeout))
         events = self._inotify.read(timeout=timeout)
         if not events:
             # use "None" as a sentinel for a timeout, otherwise we can not
             # tell if its all events that didn't match or a true timeout
             return [None]
@@ -78,15 +81,15 @@
         return [
             event
             for event in events
             if (event.name == self._name)
             and ((event.mask & _inotify.flags.CLOSE_WRITE) != 0)
         ]
 
-    def _wait(self):
+    def _wait(self) -> typing.Iterator[None]:
         while True:
             for event in self._get_events():
                 if event is None:
                     self._print("timed out")
                     yield None
                 else:
                     self._print(f"{self._name} modified")
```

### Comparing `sambacc-0.2/sambacc/jfile.py` & `sambacc-0.3/sambacc/jfile.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,44 +17,47 @@
 #
 """Utilities for working with JSON data stored in a file system file.
 """
 
 import fcntl
 import json
 import os
+import typing
 
 OPEN_RO = os.O_RDONLY
 OPEN_RW = os.O_CREAT | os.O_RDWR
 
 
-def open(path, flags, mode=0o644):
+def open(path: str, flags: int, mode: int = 0o644) -> typing.IO:
     """A wrapper around open to open JSON files for read or read/write.
     `flags` must be os.open type flags. Use `OPEN_RO` and `OPEN_RW` for
     convenience.
     """
     return os.fdopen(os.open(path, flags, mode), "r+")
 
 
-def load(fh, default=None):
+def load(
+    fh: typing.IO, default: typing.Optional[dict[str, typing.Any]] = None
+) -> typing.Any:
     """Similar to json.load, but returns the `default` value if fh refers to an
     empty file. fh must be seekable."""
     if fh.read(4) == "":
         # probe it to see if its an empty file
         data = default
     else:
         fh.seek(0)
         data = json.load(fh)
     return data
 
 
-def dump(data, fh):
+def dump(data: typing.Any, fh: typing.IO) -> None:
     """Similar to json.dump, but truncates the file before writing in order
     to avoid appending data to the file. fh must be seekable.
     """
     fh.seek(0)
     fh.truncate(0)
     json.dump(data, fh)
 
 
-def flock(fh):
+def flock(fh: typing.IO) -> None:
     """A simple wrapper around flock."""
     fcntl.flock(fh.fileno(), fcntl.LOCK_EX)
```

### Comparing `sambacc-0.2/sambacc/join.py` & `sambacc-0.3/sambacc/join.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,35 +25,41 @@
 from sambacc import samba_cmds
 from sambacc.simple_waiter import Waiter
 
 _logger = logging.getLogger(__name__)
 
 
 class JoinError(Exception):
-    def __init__(self, v):
+    def __init__(self, v: typing.Any) -> None:
         super().__init__(v)
-        self.errors = []
+        self.errors: list[typing.Any] = []
 
 
 _PROMPT = object()
+_PT = typing.TypeVar("_PT")
+_PW = typing.Union[str, _PT]
 
 
 class JoinBy(enum.Enum):
     PASSWORD = "password"
     FILE = "file"
     INTERACTIVE = "interactive"
 
 
 class UserPass:
     """Encapsulate a username/password pair."""
 
     username: str = "Administrator"
-    password: typing.Optional[str] = None
+    password: typing.Optional[_PW] = None
 
-    def __init__(self, username=None, password=None):
+    def __init__(
+        self,
+        username: typing.Optional[str] = None,
+        password: typing.Optional[_PW] = None,
+    ) -> None:
         if username is not None:
             self.username = username
         if password is not None:
             self.password = password
 
 
 class Joiner:
@@ -61,32 +67,34 @@
 
     Use the `add_source` method to add one or more sources of join auth
     data. Call `join` to commit and join the "host" to AD.
     """
 
     _net_ads_join = samba_cmds.net["ads", "join"]
 
-    def __init__(self, marker=None):
-        self._sources = []
+    def __init__(self, marker: typing.Optional[str] = None) -> None:
+        self._sources: list[tuple[JoinBy, typing.Any]] = []
         self.marker = marker
 
     def add_source(
-        self, method: JoinBy, value: typing.Optional[str] = None
+        self,
+        method: JoinBy,
+        value: typing.Optional[typing.Union[str, UserPass]] = None,
     ) -> None:
         if method in {JoinBy.PASSWORD, JoinBy.INTERACTIVE}:
             if not isinstance(value, UserPass):
                 raise ValueError("expected UserPass value")
         elif method in {JoinBy.FILE}:
             if not isinstance(value, str):
                 raise ValueError("expected str value")
         else:
             raise ValueError(f"invalid method: {method}")
         self._sources.append((method, value))
 
-    def join(self, dns_updates=False) -> None:
+    def join(self, dns_updates: bool = False) -> None:
         if not self._sources:
             raise JoinError("no sources for join data")
         errors = []
         for method, value in self._sources:
             try:
                 if method is JoinBy.PASSWORD:
                     upass = value
@@ -104,15 +112,15 @@
         if errors:
             if len(errors) == 1:
                 raise errors[0]
             err = JoinError("failed {} join attempts".format(len(errors)))
             err.errors = errors
             raise err
 
-    def _read_from(self, path) -> UserPass:
+    def _read_from(self, path: str) -> UserPass:
         try:
             with open(path) as fh:
                 data = json.load(fh)
         except FileNotFoundError:
             raise JoinError(f"source file not found: {path}")
         upass = UserPass()
         try:
@@ -122,15 +130,15 @@
             raise JoinError(f"invalid file content: {err}")
         if not isinstance(upass.username, str):
             raise JoinError("invalid file content: invalid username")
         if not isinstance(upass.password, str):
             raise JoinError("invalid file content: invalid password")
         return upass
 
-    def _join(self, upass: UserPass, dns_updates=False) -> None:
+    def _join(self, upass: UserPass, dns_updates: bool = False) -> None:
         args = []
         if not dns_updates:
             args.append("--no-dns-updates")
         args.extend(["-U", upass.username])
 
         if upass.password is _PROMPT:
             cmd = list(self._net_ads_join[args])
@@ -167,15 +175,17 @@
         try:
             return data["joined"]
         except (TypeError, KeyError):
             return False
 
 
 def join_when_possible(
-    joiner: Joiner, waiter: Waiter, error_handler=None
+    joiner: Joiner,
+    waiter: Waiter,
+    error_handler: typing.Optional[typing.Callable] = None,
 ) -> None:
     while True:
         if joiner.did_join():
             _logger.info("found valid join marker")
             return
         try:
             joiner.join()
```

### Comparing `sambacc-0.2/sambacc/leader.py` & `sambacc-0.3/sambacc/leader.py`

 * *Files 16% similar despite different names*

```diff
@@ -14,14 +14,16 @@
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>
 #
 
 import typing
 
+from sambacc.typelets import ExcType, ExcValue, ExcTraceback
+
 
 class LeaderStatus(typing.Protocol):
     """Fetches information about the current cluster leader."""
 
     def is_leader(self) -> bool:
         ...
 
@@ -31,9 +33,11 @@
     Can be used for purely informational types or types that
     actually acquire cluster leadership if needed.
     """
 
     def __enter__(self) -> LeaderStatus:
         ...
 
-    def __exit__(self, exc_type, exc_val, exc_tb) -> None:
+    def __exit__(
+        self, exc_type: ExcType, exc_val: ExcValue, exc_tb: ExcTraceback
+    ) -> bool:
         ...
```

### Comparing `sambacc-0.2/sambacc/netcmd_loader.py` & `sambacc-0.3/sambacc/netcmd_loader.py`

 * *Files 12% similar despite different names*

```diff
@@ -24,53 +24,55 @@
 
 
 class LoaderError(Exception):
     pass
 
 
 def template_config(
-    fh: typing.IO, iconfig: config.SambaConfig, enc=str
+    fh: typing.IO, iconfig: config.SambaConfig, enc: typing.Callable = str
 ) -> None:
     fh.write(enc("[global]\n"))
     for gkey, gval in iconfig.global_options():
         fh.write(enc(f"\t{gkey} = {gval}\n"))
 
     for share in iconfig.shares():
         fh.write(enc("\n[{}]\n".format(share.name)))
         for skey, sval in share.share_options():
             fh.write(enc(f"\t{skey} = {sval}\n"))
 
 
 class NetCmdLoader:
     _net_conf = samba_cmds.net["conf"]
 
-    def _cmd(self, *args, **kwargs):
+    def _cmd(
+        self, *args: str, **kwargs: typing.Any
+    ) -> tuple[list[str], typing.Any]:
         cmd = list(self._net_conf[args])
         return cmd, subprocess.Popen(cmd, **kwargs)
 
-    def _check(self, cli, proc) -> None:
+    def _check(self, cli: typing.Any, proc: subprocess.Popen) -> None:
         ret = proc.wait()
         if ret != 0:
             raise LoaderError("failed to run {}".format(cli))
 
     def import_config(self, iconfig: config.InstanceConfig) -> None:
         """Import to entire instance config to samba config."""
         cli, proc = self._cmd("import", "/dev/stdin", stdin=subprocess.PIPE)
         template_config(proc.stdin, iconfig, enc=samba_cmds.encode)
         proc.stdin.close()
         self._check(cli, proc)
 
-    def dump(self, out: typing.IO):
+    def dump(self, out: typing.IO) -> None:
         """Dump the current smb config in an smb.conf format.
         Writes the dump to `out`.
         """
         cli, proc = self._cmd("list", stdout=out)
         self._check(cli, proc)
 
-    def _parse_shares(self, fh) -> typing.Iterable[str]:
+    def _parse_shares(self, fh: typing.IO) -> typing.Iterable[str]:
         out = []
         for line in fh.readlines():
             line = line.strip().decode("utf8")
             if line == "global":
                 continue
             out.append(line)
         return out
```

### Comparing `sambacc-0.2/sambacc/nsswitch_loader.py` & `sambacc-0.3/sambacc/nsswitch_loader.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,18 +18,18 @@
 
 import typing
 
 from .textfile import TextFileLoader
 
 
 class NameServiceSwitchLoader(TextFileLoader):
-    def __init__(self, path):
+    def __init__(self, path: str) -> None:
         super().__init__(path)
-        self.lines = []
-        self.idx = {}
+        self.lines: list[str] = []
+        self.idx: dict[str, int] = {}
 
     def loadlines(self, lines: typing.Iterable[str]) -> None:
         """Load in the lines from the text source."""
         # Ignore comments and blank lines
         for line in lines:
             if not line.strip() or line.startswith("#"):
                 continue
```

### Comparing `sambacc-0.2/sambacc/passdb_loader.py` & `sambacc-0.3/sambacc/passdb_loader.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,31 +12,33 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>
 #
 
+import typing
+
 from sambacc import config
 
 # Do the samba python bindings not export any useful constants?
 ACB_DISABLED = 0x00000001
 ACB_NORMAL = 0x00000010
 ACB_PWNOEXP = 0x00000200
 
 
-def _samba_modules():
+def _samba_modules() -> tuple[typing.Any, typing.Any]:
     from samba.samba3 import param  # type: ignore
     from samba.samba3 import passdb  # type: ignore
 
     return param, passdb
 
 
 class PassDBLoader:
-    def __init__(self, smbconf=None):
+    def __init__(self, smbconf: typing.Any = None) -> None:
         param, passdb = _samba_modules()
         lp = param.get_context()
         if smbconf is None:
             lp.load_default()
         else:
             lp.load(smbconf)
         passdb.set_secrets_dir(lp.get("private dir"))
```

### Comparing `sambacc-0.2/sambacc/passwd_loader.py` & `sambacc-0.3/sambacc/passwd_loader.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,17 +19,17 @@
 import typing
 
 from .textfile import TextFileLoader
 from sambacc import config
 
 
 class LineFileLoader(TextFileLoader):
-    def __init__(self, path):
+    def __init__(self, path: str) -> None:
         super().__init__(path)
-        self.lines = []
+        self.lines: list[str] = []
 
     def loadlines(self, lines: typing.Iterable[str]) -> None:
         """Load in the lines from the text source."""
         for line in lines:
             self.lines.append(line)
 
     def dumplines(self) -> typing.Iterable[str]:
@@ -39,17 +39,17 @@
             if prev and not prev.endswith("\n"):
                 yield "\n"
             yield line
             prev = line
 
 
 class PasswdFileLoader(LineFileLoader):
-    def __init__(self, path="/etc/passwd"):
+    def __init__(self, path: str = "/etc/passwd") -> None:
         super().__init__(path)
-        self._usernames = set()
+        self._usernames: set[str] = set()
 
     def readfp(self, fp: typing.IO) -> None:
         super().readfp(fp)
         self._update_usernames_cache()
 
     def _update_usernames_cache(self) -> None:
         for line in self.lines:
@@ -62,17 +62,17 @@
             return
         line = "{}\n".format(":".join(user_entry.passwd_fields()))
         self.lines.append(line)
         self._usernames.add(user_entry.username)
 
 
 class GroupFileLoader(LineFileLoader):
-    def __init__(self, path="/etc/group"):
+    def __init__(self, path: str = "/etc/group") -> None:
         super().__init__(path)
-        self._groupnames = set()
+        self._groupnames: set[str] = set()
 
     def readfp(self, fp: typing.IO) -> None:
         super().readfp(fp)
         self._update_groupnames_cache()
 
     def _update_groupnames_cache(self) -> None:
         for line in self.lines:
```

### Comparing `sambacc-0.2/sambacc/paths.py` & `sambacc-0.3/sambacc/paths.py`

 * *Files identical despite different names*

### Comparing `sambacc-0.2/sambacc/permissions.py` & `sambacc-0.3/sambacc/permissions.py`

 * *Files 6% similar despite different names*

```diff
@@ -120,30 +120,30 @@
 
     def path(self) -> str:
         return self._path
 
     def _full_path(self) -> str:
         return os.path.join(self._root, self._path.lstrip("/"))
 
-    def has_status(self):
+    def has_status(self) -> bool:
         try:
             self._get_status()
             return True
         except KeyError:
             return False
 
-    def status_ok(self):
+    def status_ok(self) -> bool:
         try:
             sval = self._get_status()
         except KeyError:
             return False
         curr_prefix = sval.split("/")[0]
         return curr_prefix == self._prefix
 
-    def update(self):
+    def update(self) -> None:
         if self.status_ok():
             return
         self._set_perms()
         self._set_status()
 
     def _get_status(self) -> str:
         path = self._full_path()
@@ -178,10 +178,10 @@
 
 class AlwaysPosixPermsHandler(InitPosixPermsHandler):
     """Works like the init handler, but always sets the permissions,
     even if the status xattr exists and is valid.
     May be useful for testing and debugging.
     """
 
-    def update(self):
+    def update(self) -> None:
         self._set_perms()
         self._set_status()
```

### Comparing `sambacc-0.2/sambacc/samba_cmds.py` & `sambacc-0.3/sambacc/samba_cmds.py`

 * *Files 9% similar despite different names*

```diff
@@ -18,22 +18,23 @@
 
 from __future__ import annotations
 
 import os
 import typing
 
 DebugLevel = typing.Optional[str]
-ArgList = typing.Optional[typing.List[str]]
+ArgList = typing.Optional[list[str]]
 
-_GLOBAL_PREFIX: typing.List[str] = []
+_GLOBAL_PREFIX: list[str] = []
 _GLOBAL_DEBUG: str = ""
 
 
 # Known flags for SAMBA_SPECIFICS env variable
 _DAEMON_CLI_STDOUT_OPT: str = "daemon_cli_debug_output"
+_CTDB_LEADER_ADMIN_CMD: str = "ctdb_leader_admin_command"
 
 
 def get_samba_specifics() -> typing.Set[str]:
     value = os.environ.get("SAMBA_SPECIFICS", "")
     out = set()
     if value:
         for v in value.split(","):
@@ -48,51 +49,59 @@
         opt = "--stdout"
     opt_lst = get_samba_specifics()
     if _DAEMON_CLI_STDOUT_OPT in opt_lst:
         opt = "--debug-stdout"
     return opt
 
 
-def set_global_prefix(lst: typing.List[str]) -> None:
+def ctdb_leader_admin_cmd() -> str:
+    leader_cmd = "recmaster"
+    opt_lst = get_samba_specifics()
+    if _CTDB_LEADER_ADMIN_CMD in opt_lst:
+        leader_cmd = "leader"
+    return leader_cmd
+
+
+def set_global_prefix(lst: list[str]) -> None:
     _GLOBAL_PREFIX[:] = lst
 
 
 def set_global_debug(level: str) -> None:
     global _GLOBAL_DEBUG
     _GLOBAL_DEBUG = level
 
 
-def _to_args(value) -> typing.List[str]:
+def _to_args(value: typing.Any) -> list[str]:
     if isinstance(value, str):
         return [value]
     return [str(v) for v in value]
 
 
 class CommandArgs:
     """A utility class for building command line commands."""
 
     _name: str
-    args: typing.List[str]
-    cmd_prefix: typing.List[str]
+    args: list[str]
+    cmd_prefix: list[str]
 
     def __init__(self, name: str, args: ArgList = None):
         self._name = name
         self.args = args or []
         self.cmd_prefix = []
 
-    def __getitem__(self, new_value) -> CommandArgs:
+    def __getitem__(self, new_value: typing.Any) -> CommandArgs:
         return self.__class__(self._name, args=self.args + _to_args(new_value))
 
-    def raw_args(self) -> typing.List[str]:
+    def raw_args(self) -> list[str]:
         return [self._name] + self.args
 
-    def prefix_args(self) -> typing.List[str]:
+    def prefix_args(self) -> list[str]:
         return list(_GLOBAL_PREFIX) + list(self.cmd_prefix)
 
-    def argv(self) -> typing.List[str]:
+    def argv(self) -> list[str]:
         return self.prefix_args() + self.raw_args()
 
     def __iter__(self) -> typing.Iterator[str]:
         return iter(self.argv())
 
     def __repr__(self) -> str:
         return "CommandArgs({!r}, {!r})".format(self._name, self.args)
@@ -112,29 +121,29 @@
 
     def __init__(
         self, name: str, args: ArgList = None, debug: DebugLevel = None
     ):
         super().__init__(name, args)
         self.debug = debug
 
-    def __getitem__(self, new_value) -> SambaCommand:
+    def __getitem__(self, new_value: typing.Any) -> SambaCommand:
         return self.__class__(
             self._name,
             args=self.args + _to_args(new_value),
             debug=self.debug,
         )
 
-    def _debug_args(self, dlvl: str = "--debuglevel={}") -> typing.List[str]:
+    def _debug_args(self, dlvl: str = "--debuglevel={}") -> list[str]:
         if self.debug:
             return [dlvl.format(self.debug)]
         if _GLOBAL_DEBUG:
             return [dlvl.format(_GLOBAL_DEBUG)]
         return []
 
-    def raw_args(self) -> typing.List[str]:
+    def raw_args(self) -> list[str]:
         return [self._name] + self._debug_args() + self.args
 
     def __repr__(self) -> str:
         return "SambaCommand({!r}, {!r}, {!r})".format(
             self._name, self.args, self.debug
         )
 
@@ -146,27 +155,27 @@
 smbd = SambaCommand("/usr/sbin/smbd")
 
 winbindd = SambaCommand("/usr/sbin/winbindd")
 
 samba_dc = SambaCommand("/usr/sbin/samba")
 
 
-def smbd_foreground():
+def smbd_foreground() -> SambaCommand:
     return smbd[
         "--foreground", _daemon_stdout_opt("smbd"), "--no-process-group"
     ]
 
 
-def winbindd_foreground():
+def winbindd_foreground() -> SambaCommand:
     return winbindd[
         "--foreground", _daemon_stdout_opt("winbindd"), "--no-process-group"
     ]
 
 
-def samba_dc_foreground():
+def samba_dc_foreground() -> SambaCommand:
     return samba_dc["--foreground"]
 
 
 ctdbd = SambaCommand("/usr/sbin/ctdbd")
 
 ctdbd_foreground = ctdbd["--interactive"]
```

### Comparing `sambacc-0.2/sambacc/simple_waiter.py` & `sambacc-0.3/sambacc/simple_waiter.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 # along with this program.  If not, see <http://www.gnu.org/licenses/>
 #
 
 import time
 import typing
 
 
-def generate_sleeps():
+def generate_sleeps() -> typing.Iterator[int]:
     """Generate sleep times starting with short sleeps and then
     getting longer. This assumes that resources may take a bit of
     time to settle, but eventually reach a steadier state and don't
     require being checked as often.
     """
     total = 0
     while True:
@@ -40,24 +40,26 @@
 
 # It's a bit overkill to have a class for this but I didn't like messing
 # around with functools.partial or functions returning functions for this.
 # It's also nice to replace the sleep function for unit tests.
 class Sleeper:
     """It waits only by sleeping. Nothing fancy."""
 
-    def __init__(self, times=None):
+    def __init__(
+        self, times: typing.Optional[typing.Iterator[int]] = None
+    ) -> None:
         if times is None:
             times = generate_sleeps()
         self._times = times
         self._sleep = time.sleep
 
-    def wait(self):
+    def wait(self) -> None:
         self._sleep(next(self._times))
 
-    def acted(self):
+    def acted(self) -> None:
         """Inform the sleeper the caller reacted to a change and
         the sleeps should be reset.
         """
         self.times = generate_sleeps()
 
 
 class Waiter(typing.Protocol):
```

### Comparing `sambacc-0.2/sambacc/textfile.py` & `sambacc-0.3/sambacc/textfile.py`

 * *Files identical despite different names*

### Comparing `sambacc-0.2/sambacc.egg-info/SOURCES.txt` & `sambacc-0.3/sambacc.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 .gitignore
+.gitlint
 .hgignore
 COPYING
 MANIFEST.in
 README.md
 pyproject.toml
 setup.cfg
 tox.ini
+.copr/Makefile
+.github/mergify.yml
 .github/workflows/ci.yml
+docs/configuration.md
 examples/addc.json
 examples/ctdb.json
 examples/example1.json
 examples/minimal.json
 extras/python-sambacc.spec
 sambacc/__init__.py
 sambacc/_version.py
@@ -28,32 +32,39 @@
 sambacc/passdb_loader.py
 sambacc/passwd_loader.py
 sambacc/paths.py
 sambacc/permissions.py
 sambacc/samba_cmds.py
 sambacc/simple_waiter.py
 sambacc/textfile.py
+sambacc/typelets.py
 sambacc.egg-info/PKG-INFO
 sambacc.egg-info/SOURCES.txt
 sambacc.egg-info/dependency_links.txt
 sambacc.egg-info/entry_points.txt
+sambacc.egg-info/requires.txt
 sambacc.egg-info/top_level.txt
 sambacc/commands/__init__.py
 sambacc/commands/addc.py
 sambacc/commands/check.py
 sambacc/commands/cli.py
 sambacc/commands/config.py
 sambacc/commands/ctdb.py
 sambacc/commands/dcmain.py
 sambacc/commands/dns.py
 sambacc/commands/initialize.py
 sambacc/commands/join.py
 sambacc/commands/main.py
 sambacc/commands/run.py
 sambacc/commands/users.py
+sambacc/schema/__init__.py
+sambacc/schema/conf-v0.schema.json
+sambacc/schema/conf-v0.schema.yaml
+sambacc/schema/conf_v0_schema.py
+sambacc/schema/tool.py
 tests/__init__.py
 tests/test_commands_config.py
 tests/test_config.py
 tests/test_container_dns.py
 tests/test_ctdb.py
 tests/test_inotify_waiter.py
 tests/test_jfile.py
```

### Comparing `sambacc-0.2/setup.cfg` & `sambacc-0.3/setup.cfg`

 * *Files 22% similar despite different names*

```diff
@@ -5,26 +5,34 @@
 author = John Mulligan
 author_email = phlogistonjohn@asynchrono.us
 readme = file: README.md
 url = https://github.com/samba-in-kubernetes/sambacc
 license = GPL3
 
 [options]
-packages = sambacc, sambacc.commands
+packages = sambacc, sambacc.commands, sambacc.schema
 include_package_data = True
 
 [options.entry_points]
 console_scripts = 
 	samba-container = sambacc.commands.main:main
 	samba-dc-container = sambacc.commands.dcmain:main
 
 [options.data_files]
 share/sambacc/examples = 
 	examples/ctdb.json
 	examples/example1.json
 	examples/minimal.json
 	examples/addc.json
 
+[options.extras_require]
+validation = 
+	jsonschema>=4.10
+yaml = 
+	PyYAML>=5.4
+toml = 
+	tomli;python_version<"3.11"
+
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `sambacc-0.2/tests/test_commands_config.py` & `sambacc-0.3/tests/test_commands_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,14 +90,15 @@
     instance_config: sambacc.config.InstanceConfig
 
     def __init__(self, opts, instance_config):
         self.cli = argparse.Namespace()
         self.instance_config = instance_config
         for k, v in opts.items():
             setattr(self.cli, k, v)
+        self.require_validation = False
 
     @classmethod
     def defaults(cls, cfg_path, watch=False):
         with open(cfg_path, "w") as fh:
             fh.write(config1)
 
         config = [cfg_path]
```

### Comparing `sambacc-0.2/tests/test_config.py` & `sambacc-0.3/tests/test_config.py`

 * *Files 27% similar despite different names*

```diff
@@ -444,15 +444,15 @@
         with pytest.raises(OSError):
             sambacc.config.read_config_files([fname])
     finally:
         os.unlink(fname)
 
 
 def test_tesd_config_files_realerr_rootok(monkeypatch):
-    def err_open(p):
+    def err_open(*args):
         raise OSError("test!")
 
     monkeypatch.setattr(sambacc.config, "_open", err_open)
     fname = "/etc/foobar"
     with pytest.raises(OSError):
         sambacc.config.read_config_files([fname])
 
@@ -525,51 +525,45 @@
     with pytest.raises(ValueError):
         list(i1.domain_users())
 
     with pytest.raises(ValueError):
         list(i1.domain_groups())
 
 
-def test_ad_dc_bad_memeber_of():
-    jdata = """
-{
-  "samba-container-config": "v0",
-  "configs": {
-    "demo": {
-      "instance_features": ["addc"],
-      "domain_settings": "sink",
-      "instance_name": "dc1"
-    }
-  },
-  "domain_settings": {
-    "sink": {
-      "realm": "DOMAIN1.SINK.TEST",
-      "short_domain": "DOMAIN1",
-      "admin_password": "Passw0rd"
+def test_ad_dc_bad_member_of():
+    jdata = {
+        "samba-container-config": "v0",
+        "configs": {
+            "demo": {
+                "instance_features": ["addc"],
+                "domain_settings": "sink",
+                "instance_name": "dc1",
+            }
+        },
+        "domain_settings": {
+            "sink": {
+                "realm": "DOMAIN1.SINK.TEST",
+                "short_domain": "DOMAIN1",
+                "admin_password": "Passw0rd",
+            }
+        },
+        "domain_groups": {"sink": [{"name": "friends"}]},
+        "domain_users": {
+            "sink": [
+                {
+                    "name": "ckent",
+                    "password": "1115Rose.",
+                    "given_name": "Clark",
+                    "surname": "Kent",
+                    "member_of": "friends",
+                }
+            ]
+        },
     }
-  },
-  "domain_groups": {
-    "sink": [
-      {"name": "friends"}
-    ]
-  },
-  "domain_users": {
-    "sink": [
-      {
-        "name": "ckent",
-        "password": "1115Rose.",
-        "given_name": "Clark",
-        "surname": "Kent",
-        "member_of": "friends"
-      }
-    ]
-  }
-}
-    """
-    c1 = sambacc.config.GlobalConfig(io.StringIO(jdata))
+    c1 = sambacc.config.GlobalConfig(initial_data=jdata)
     i1 = c1.get("demo")
     assert i1.with_addc
 
     dgroups = sorted(i1.domain_groups(), key=lambda v: v.groupname)
     assert len(dgroups) == 1
     assert dgroups[0].groupname == "friends"
 
@@ -756,7 +750,521 @@
             "friendship": "always",
         }
     )
     opts = pc.options
     assert len(opts) == 2
     assert "mode" in opts
     assert "friendship" in opts
+
+
+def _can_import_toml():
+    """Return true if one valid toml module can be imported.
+    Work around importorskip only supporting one module name.
+    """
+    try:
+        __import__("tomllib")
+        return True
+    except ImportError:
+        pass
+    try:
+        __import__("tomli")
+        return True
+    except ImportError:
+        pass
+    return False
+
+
+@pytest.mark.parametrize(
+    "json_str,ok",
+    [
+        pytest.param("{}", False, id="empty-json"),
+        pytest.param('{"samba-container-config":"v0"}', True, id="minimal"),
+        pytest.param(
+            """
+{
+    "samba-container-config": "v0",
+    "configs": {
+        "foobar": {
+            "shares": [
+                "foobar"
+            ]
+        }
+    },
+    "shares": {
+        "foobar": {
+            "options": {
+                "a": "b"
+            }
+        }
+    }
+}
+        """,
+            True,
+            id="one-share",
+        ),
+        pytest.param(
+            """
+{
+    "samba-container-config": "v0",
+    "configs": {
+        "foobar": {
+            "shares": [
+                "foobar"
+            ]
+        }
+    },
+    "shares": {
+        "foobar": {
+            "options": {
+                "a": "b"
+            }
+        }
+    },
+    "chairs": {"maple": true}
+}
+        """,
+            False,
+            id="invalid-section",
+        ),
+        pytest.param(
+            """
+{
+    "samba-container-config": "v0",
+    "configs": {
+        "foobar": {
+            "shares": [
+                "foobar"
+            ]
+        }
+    },
+    "shares": {
+        "foobar": {
+            "options": {
+                "a": "b"
+            }
+        }
+    },
+    "_chairs": {"maple": true}
+}
+        """,
+            True,
+            id="underscore-prefix",
+        ),
+        pytest.param(
+            """
+{
+    "samba-container-config": "v0",
+    "configs": {
+        "foobar": {
+            "lazlo": "quux",
+            "shares": [
+                "foobar"
+            ]
+        }
+    },
+    "shares": {
+        "foobar": {
+            "options": {
+                "a": "b"
+            }
+        }
+    }
+}
+        """,
+            False,
+            id="bad-config-param",
+        ),
+        pytest.param(
+            """
+{
+    "samba-container-config": "v0",
+    "configs": {
+        "foobar": {
+            "shares": "foobar"
+        }
+    },
+    "shares": {
+        "foobar": {
+            "options": {
+                "a": "b"
+            }
+        }
+    }
+}
+        """,
+            False,
+            id="bad-config-type",
+        ),
+        pytest.param(
+            """
+{
+    "samba-container-config": "v0",
+    "configs": {
+        "foobar": {
+            "shares": [
+                "foobar"
+            ]
+        }
+    },
+    "shares": {
+        "foobar": {
+            "blooper": true,
+            "options": {
+                "a": "b"
+            }
+        }
+    }
+}
+        """,
+            False,
+            id="bad-share-prop",
+        ),
+    ],
+)
+def test_jsonschema_validation(json_str, ok):
+    jsonschema = pytest.importorskip("jsonschema")
+
+    cfg = sambacc.config.GlobalConfig()
+    if ok:
+        cfg.load(io.StringIO(json_str), require_validation=True)
+    else:
+        with pytest.raises((ValueError, jsonschema.ValidationError)):
+            cfg.load(io.StringIO(json_str), require_validation=True)
+
+
+@pytest.mark.parametrize(
+    "toml_str,ok",
+    [
+        pytest.param("", False, id="empty"),
+        pytest.param("#####FOO", False, id="just-a-comment"),
+        pytest.param(
+            """
+samba-container-config = "v0"
+""",
+            True,
+            id="minimal",
+        ),
+        pytest.param(
+            """
+samba-container-config = "v0"
+
+# Define configurations
+[configs.foobar]
+shares = ["foobar"]
+
+# Define share options
+[shares.foobar.options]
+a = "b"
+""",
+            True,
+            id="one-share",
+        ),
+    ],
+)
+@pytest.mark.skipif(not _can_import_toml(), reason="no toml module")
+def test_toml_configs_no_validation(toml_str, ok):
+    cfg = sambacc.config.GlobalConfig()
+    fh = io.BytesIO(toml_str.encode("utf8"))
+    if ok:
+        cfg.load(
+            fh,
+            require_validation=False,
+            config_format=sambacc.config.ConfigFormat.TOML,
+        )
+    else:
+        with pytest.raises(ValueError):
+            cfg.load(
+                fh,
+                require_validation=False,
+                config_format=sambacc.config.ConfigFormat.TOML,
+            )
+
+
+@pytest.mark.parametrize(
+    "toml_str,ok",
+    [
+        pytest.param("", False, id="empty"),
+        pytest.param("#####FOO", False, id="just-a-comment"),
+        pytest.param(
+            """
+samba-container-config = "v0"
+""",
+            True,
+            id="minimal",
+        ),
+        pytest.param(
+            """
+samba-container-config = "v0"
+
+# Define configurations
+[configs.foobar]
+shares = ["foobar"]
+
+# Define share options
+[shares.foobar.options]
+a = "b"
+""",
+            True,
+            id="one-share",
+        ),
+        pytest.param(
+            """
+samba-container-config = "v0"
+
+# Define configurations
+[configs.foobar]
+shares = ["foobar"]
+instance_features = "Kibbe"
+
+# Define share options
+[shares.foobar.options]
+a = "b"
+""",
+            False,
+            id="bad-instance_features",
+        ),
+        pytest.param(
+            """
+samba-container-config = "v0"
+
+# Define configurations
+[configs.foobar]
+shares = ["foobar"]
+instance_features = ["ctdb"]
+
+# Define share options
+[shares.foobar.options]
+a = "b"
+""",
+            True,
+            id="ok-instance_features",
+        ),
+        pytest.param(
+            """
+samba-container-config = "v0"
+
+[configs.demo]
+shares = ["share"]
+globals = ["default"]
+instance_features = ["ctdb"]
+instance_name = "SAMBA"
+
+[shares.share.options]
+"path" = "/share"
+"read only" = "no"
+"valid users" = "sambauser, otheruser"
+
+[globals.default.options]
+"security" = "user"
+"server min protocol" = "SMB2"
+"load printers" = "no"
+"printing" = "bsd"
+"printcap name" = "/dev/null"
+"disable spoolss" = "yes"
+"guest ok" = "no"
+
+[[users.all_entries]]
+name = "sambauser"
+password = "samba"
+
+[[users.all_entries]]
+name = "otheruser"
+password = "insecure321"
+""",
+            True,
+            id="complex",
+        ),
+    ],
+)
+@pytest.mark.skipif(not _can_import_toml(), reason="no toml module")
+def test_toml_configs_validation(toml_str, ok):
+    jsonschema = pytest.importorskip("jsonschema")
+
+    cfg = sambacc.config.GlobalConfig()
+    fh = io.BytesIO(toml_str.encode("utf8"))
+    if ok:
+        cfg.load(
+            fh,
+            require_validation=True,
+            config_format=sambacc.config.ConfigFormat.TOML,
+        )
+    else:
+        with pytest.raises((ValueError, jsonschema.ValidationError)):
+            cfg.load(
+                fh,
+                require_validation=True,
+                config_format=sambacc.config.ConfigFormat.TOML,
+            )
+
+
+@pytest.mark.parametrize(
+    "yaml_str,ok",
+    [
+        pytest.param("", False, id="empty"),
+        pytest.param("#####FOO", False, id="just-a-comment"),
+        pytest.param(
+            """
+samba-container-config: "v0"
+""",
+            True,
+            id="minimal",
+        ),
+        pytest.param(
+            """
+samba-container-config: "v0"
+# Define configurations
+configs:
+  foobar:
+    shares:
+      - foobar
+shares:
+  foobar:
+    options:
+      a: b
+""",
+            True,
+            id="one-share",
+        ),
+    ],
+)
+def test_yaml_configs_no_validation(yaml_str, ok):
+    pytest.importorskip("yaml")
+
+    cfg = sambacc.config.GlobalConfig()
+    fh = io.BytesIO(yaml_str.encode("utf8"))
+    if ok:
+        cfg.load(
+            fh,
+            require_validation=False,
+            config_format=sambacc.config.ConfigFormat.YAML,
+        )
+    else:
+        with pytest.raises(ValueError):
+            cfg.load(
+                fh,
+                require_validation=False,
+                config_format=sambacc.config.ConfigFormat.YAML,
+            )
+
+
+@pytest.mark.parametrize(
+    "yaml_str,ok",
+    [
+        pytest.param("", False, id="empty"),
+        pytest.param("#####FOO", False, id="just-a-comment"),
+        pytest.param(
+            """
+samba-container-config: v0
+""",
+            True,
+            id="minimal",
+        ),
+        pytest.param(
+            """
+samba-container-config: v0
+# Define configurations
+configs:
+  foobar:
+    shares:
+      - foobar
+# Define shares
+shares:
+  foobar:
+    options:
+      a: b
+""",
+            True,
+            id="one-share",
+        ),
+        pytest.param(
+            """
+samba-container-config: v0
+configs:
+  foobar:
+    instance_features: baroof
+    shares:
+      - foobar
+shares:
+  foobar:
+    options:
+      a: b
+""",
+            False,
+            id="bad-instance_features",
+        ),
+        pytest.param(
+            """
+samba-container-config: v0
+configs:
+  foobar:
+    instance_features:
+      - ctdb
+    shares:
+      - foobar
+shares:
+  foobar:
+    options:
+      a: b
+""",
+            True,
+            id="ok-instance_features",
+        ),
+        pytest.param(
+            """
+samba-container-config: "v0"
+# Configure our demo instance
+configs:
+  demo:
+    shares: ["share"]
+    globals: ["default"]
+    instance_features: ["ctdb"]
+    instance_name: "SAMBA"
+# Configure the share
+shares:
+  share:
+    options:
+      "path": "/share"
+      "read only": "no"
+      "valid users": "sambauser, otheruser"
+# Configure globals
+globals:
+  default:
+    options:
+      "security": "user"
+      "server min protocol": "SMB2"
+      "load printers": "no"
+      "printing": "bsd"
+      "printcap name": "/dev/null"
+      "disable spoolss": "yes"
+      "guest ok": "no"
+# Configure users
+users:
+  all_entries:
+    - {"name": "sambauser", "password": "samba"}
+    - {"name": "otheruser", "password": "insecure321"}
+    - name: cooluser
+      password: snarf
+""",
+            True,
+            id="complex",
+        ),
+    ],
+)
+def test_yaml_configs_validation(yaml_str, ok):
+    pytest.importorskip("yaml")
+    jsonschema = pytest.importorskip("jsonschema")
+
+    cfg = sambacc.config.GlobalConfig()
+    fh = io.BytesIO(yaml_str.encode("utf8"))
+    if ok:
+        cfg.load(
+            fh,
+            require_validation=True,
+            config_format=sambacc.config.ConfigFormat.YAML,
+        )
+    else:
+        with pytest.raises((ValueError, jsonschema.ValidationError)):
+            cfg.load(
+                fh,
+                require_validation=True,
+                config_format=sambacc.config.ConfigFormat.YAML,
+            )
```

### Comparing `sambacc-0.2/tests/test_container_dns.py` & `sambacc-0.3/tests/test_container_dns.py`

 * *Files 2% similar despite different names*

```diff
@@ -197,14 +197,15 @@
         fh.write(J1)
 
     sambacc.container_dns.watch(
         "example.com",
         path,
         update_func=_update,
         pause_func=_sleep,
+        print_func=lambda x: None,
     )
     assert scount > 10
     assert len(reg_data) == 1
 
     with open(path, "w") as fh:
         fh.write(J1)
     scount = 0
@@ -223,10 +224,11 @@
         time.sleep(0.05)
 
     sambacc.container_dns.watch(
         "example.com",
         path,
         update_func=_update,
         pause_func=_sleep2,
+        print_func=lambda x: None,
     )
     assert scount > 20
     assert len(reg_data) == 3
```

### Comparing `sambacc-0.2/tests/test_ctdb.py` & `sambacc-0.3/tests/test_ctdb.py`

 * *Files 2% similar despite different names*

```diff
@@ -523,21 +523,23 @@
 
 def test_cli_leader_locator(tmpdir, monkeypatch, caplog):
     import logging
 
     caplog.set_level(logging.INFO)
     fake_ctdb = tmpdir / "fake_ctdb.sh"
     monkeypatch.setattr(sambacc.samba_cmds, "_GLOBAL_PREFIX", [fake_ctdb])
+    monkeypatch.setenv("SAMBA_SPECIFICS", "ctdb_leader_admin_command")
+    ldr_admin_cmd = sambacc.samba_cmds.ctdb_leader_admin_cmd()
 
     def _fake_ctdb_script(pnn, recmaster):
         with open(fake_ctdb, "w") as fh:
             fh.write("#!/bin/sh\n")
             fh.write("case $2 in\n")
             fh.write(f"pnn) {pnn};;\n")
-            fh.write(f"recmaster) {recmaster};;\n")
+            fh.write(f"{ldr_admin_cmd}) {recmaster};;\n")
             fh.write("esac\n")
             fh.write("exit 5\n")
         os.chmod(fake_ctdb, 0o700)
 
     _fake_ctdb_script(pnn="echo 0; exit 0", recmaster="echo 0; exit 0")
     with ctdb.CLILeaderLocator() as status:
         assert status.is_leader()
@@ -547,26 +549,26 @@
         assert not status.is_leader()
 
     # test error handling
     _fake_ctdb_script(pnn="exit 1", recmaster="echo 0; exit 0")
     with ctdb.CLILeaderLocator() as status:
         assert not status.is_leader()
     assert "pnn" in caplog.records[-1].getMessage()
-    assert "recmaster" not in caplog.records[-1].getMessage()
+    assert "['" + ldr_admin_cmd + "']" not in caplog.records[-1].getMessage()
     _fake_ctdb_script(pnn="echo 1; exit 0", recmaster="exit 1")
     with ctdb.CLILeaderLocator() as status:
         assert not status.is_leader()
     assert "pnn" not in caplog.records[-1].getMessage()
-    assert "recmaster" in caplog.records[-1].getMessage()
+    assert "['" + ldr_admin_cmd + "']" in caplog.records[-1].getMessage()
 
     os.unlink(fake_ctdb)
     with ctdb.CLILeaderLocator() as status:
         assert not status.is_leader()
     assert "pnn" in caplog.records[-2].getMessage()
-    assert "recmaster" in caplog.records[-1].getMessage()
+    assert "['" + ldr_admin_cmd + "']" in caplog.records[-1].getMessage()
 
 
 def test_check_nodestatus(tmp_path):
     import os
 
     datapath = tmp_path / "_ctdb"
     datapath.mkdir()
```

### Comparing `sambacc-0.2/tests/test_inotify_waiter.py` & `sambacc-0.3/tests/test_inotify_waiter.py`

 * *Files identical despite different names*

### Comparing `sambacc-0.2/tests/test_jfile.py` & `sambacc-0.3/tests/test_jfile.py`

 * *Files identical despite different names*

### Comparing `sambacc-0.2/tests/test_join.py` & `sambacc-0.3/tests/test_join.py`

 * *Files identical despite different names*

### Comparing `sambacc-0.2/tests/test_main.py` & `sambacc-0.3/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `sambacc-0.2/tests/test_netcmd_loader.py` & `sambacc-0.3/tests/test_netcmd_loader.py`

 * *Files identical despite different names*

### Comparing `sambacc-0.2/tests/test_passdb_loader.py` & `sambacc-0.3/tests/test_passdb_loader.py`

 * *Files identical despite different names*

### Comparing `sambacc-0.2/tests/test_passwd_loader.py` & `sambacc-0.3/tests/test_passwd_loader.py`

 * *Files identical despite different names*

### Comparing `sambacc-0.2/tests/test_paths.py` & `sambacc-0.3/tests/test_paths.py`

 * *Files identical despite different names*

### Comparing `sambacc-0.2/tests/test_permissions.py` & `sambacc-0.3/tests/test_permissions.py`

 * *Files identical despite different names*

### Comparing `sambacc-0.2/tests/test_samba_cmds.py` & `sambacc-0.3/tests/test_samba_cmds.py`

 * *Files identical despite different names*

### Comparing `sambacc-0.2/tests/test_simmple_waiter.py` & `sambacc-0.3/tests/test_simmple_waiter.py`

 * *Files identical despite different names*

