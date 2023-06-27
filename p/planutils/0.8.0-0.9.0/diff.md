# Comparing `tmp/planutils-0.8.0.tar.gz` & `tmp/planutils-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "planutils-0.8.0.tar", last modified: Fri Feb 24 14:40:16 2023, max compression
+gzip compressed data, was "planutils-0.9.0.tar", last modified: Mon Mar  6 15:01:05 2023, max compression
```

## Comparing `planutils-0.8.0.tar` & `planutils-0.9.0.tar`

### file list

```diff
@@ -1,230 +1,235 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 14:40:16.253754 planutils-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-02-24 14:39:59.000000 planutils-0.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-24 14:39:59.000000 planutils-0.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6225 2023-02-24 14:40:16.253754 planutils-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5736 2023-02-24 14:39:59.000000 planutils-0.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 14:40:16.213752 planutils-0.8.0/bin/
--rwxr-xr-x   0 runner    (1001) docker     (123)      610 2023-02-24 14:39:59.000000 planutils-0.8.0/bin/planutils
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 14:40:16.213752 planutils-0.8.0/planutils/
--rw-r--r--   0 runner    (1001) docker     (123)     6232 2023-02-24 14:39:59.000000 planutils-0.8.0/planutils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3021 2023-02-24 14:39:59.000000 planutils-0.8.0/planutils/manifest_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     7183 2023-02-24 14:39:59.000000 planutils-0.8.0/planutils/package_installation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 14:40:16.213752 planutils-0.8.0/planutils/packages/
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-02-24 14:39:59.000000 planutils-0.8.0/planutils/packages/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 14:40:16.217753 planutils-0.8.0/planutils/packages/TEMPLATE/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 14:40:16.217753 planutils-0.8.0/planutils/packages/TEMPLATE/SERVICE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-02-24 14:39:59.000000 planutils-0.8.0/planutils/packages/TEMPLATE/SERVICE_TEMPLATE/planner.json
--rwxr-xr-x   0 runner    (1001) docker     (123)      459 2023-02-24 14:39:59.000000 planutils-0.8.0/planutils/packages/TEMPLATE/install
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-02-24 14:39:59.000000 planutils-0.8.0/planutils/packages/TEMPLATE/manifest.json
--rwxr-xr-x   0 runner    (1001) docker     (123)       81 2023-02-24 14:39:59.000000 planutils-0.8.0/planutils/packages/TEMPLATE/run
--rwxr-xr-x   0 runner    (1001) docker     (123)      474 2023-02-24 14:39:59.000000 planutils-0.8.0/planutils/packages/TEMPLATE/uninstall
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 14:40:16.217753 planutils-0.8.0/planutils/packages/cerberus/
--rwxr-xr-x   0 runner    (1001) docker     (123)       92 2023-02-24 14:39:59.000000 planutils-0.8.0/planutils/packages/cerberus/install
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-02-24 14:39:59.000000 planutils-0.8.0/planutils/packages/cerberus/manifest.json
--rwxr-xr-x   0 runner    (1001) docker     (123)       62 2023-02-24 14:39:59.000000 planutils-0.8.0/planutils/packages/cerberus/run
--rwxr-xr-x   0 runner    (1001) docker     (123)       29 2023-02-24 14:39:59.000000 planutils-0.8.0/planutils/packages/cerberus/uninstall
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 14:40:16.217753 planutils-0.8.0/planutils/packages/cerberus-agl/
--rwxr-xr-x   0 runner    (1001) docker     (123)       30 2023-02-24 14:39:59.000000 planutils-0.8.0/planutils/packages/cerberus-agl/install
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-02-24 14:39:59.000000 planutils-0.8.0/planutils/packages/cerberus-agl/manifest.json
--rwxr-xr-x   0 runner    (1001) docker     (123)       99 2023-02-24 14:39:59.000000 planutils-0.8.0/planutils/packages/cerberus-agl/run
--rwxr-xr-x   0 runner    (1001) docker     (123)       30 2023-02-24 14:39:59.000000 planutils-0.8.0/planutils/packages/cerberus-agl/uninstall
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 14:40:16.217753 planutils-0.8.0/planutils/packages/cerberus-sat/
--rwxr-xr-x   0 runner    (1001) docker     (123)       30 2023-02-24 14:39:59.000000 planutils-0.8.0/planutils/packages/cerberus-sat/install
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-02-24 14:39:59.000000 planutils-0.8.0/planutils/packages/cerberus-sat/manifest.json
--rwxr-xr-x   0 runner    (1001) docker     (123)       99 2023-02-24 14:39:59.000000 planutils-0.8.0/planutils/packages/cerberus-sat/run
--rwxr-xr-x   0 runner    (1001) docker     (123)       30 2023-02-24 14:39:59.000000 planutils-0.8.0/planutils/packages/cerberus-sat/uninstall
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 14:40:16.221753 planutils-0.8.0/planutils/packages/cpor/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2463 2023-02-24 14:39:59.000000 planutils-0.8.0/planutils/packages/cpor/Dockerfile
--rwxr-xr-x   0 runner    (1001) docker     (123)       70 2023-02-24 14:39:59.000000 planutils-0.8.0/planutils/packages/cpor/install
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-02-24 14:39:59.000000 planutils-0.8.0/planutils/packages/cpor/manifest.json
--rwxr-xr-x   0 runner    (1001) docker     (123)       56 2023-02-24 14:39:59.000000 planutils-0.8.0/planutils/packages/cpor/run
--rwxr-xr-x   0 runner    (1001) docker     (123)       25 2023-02-24 14:39:59.000000 planutils-0.8.0/planutils/packages/cpor/uninstall
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 14:40:16.221753 planutils-0.8.0/planutils/packages/delfi/
--rwxr-xr-x   0 runner    (1001) docker     (123)       77 2023-02-24 14:39:59.000000 planutils-0.8.0/planutils/packages/delfi/install
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-02-24 14:39:59.000000 planutils-0.8.0/planutils/packages/delfi/manifest.json
--rwxr-xr-x   0 runner    (1001) docker     (123)       59 2023-02-24 14:39:59.000000 planutils-0.8.0/planutils/packages/delfi/run
--rwxr-xr-x   0 runner    (1001) docker     (123)       26 2023-02-24 14:39:59.000000 planutils-0.8.0/planutils/packages/delfi/uninstall
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 14:40:16.221753 planutils-0.8.0/planutils/packages/downward/
--rwxr-xr-x   0 runner    (1001) docker     (123)       75 2023-02-24 14:39:59.000000 planutils-0.8.0/planutils/packages/downward/install
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-02-24 14:39:59.000000 planutils-0.8.0/planutils/packages/downward/manifest.json
--rwxr-xr-x   0 runner    (1001) docker     (123)       62 2023-02-24 14:39:59.000000 planutils-0.8.0/planutils/packages/downward/run
--rwxr-xr-x   0 runner    (1001) docker     (123)       29 2023-02-24 14:39:59.000000 planutils-0.8.0/planutils/packages/downward/uninstall
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 14:40:16.221753 planutils-0.8.0/planutils/packages/dual-bfws-fdparser/
--rwxr-xr-x   0 runner    (1001) docker     (123)       31 2023-02-24 14:39:59.000000 planutils-0.8.0/planutils/packages/dual-bfws-fdparser/install
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-02-24 14:39:59.000000 planutils-0.8.0/planutils/packages/dual-bfws-fdparser/manifest.json
--rwxr-xr-x   0 runner    (1001) docker     (123)       62 2023-02-24 14:39:59.000000 planutils-0.8.0/planutils/packages/dual-bfws-fdparser/run
--rwxr-xr-x   0 runner    (1001) docker     (123)       31 2023-02-24 14:39:59.000000 planutils-0.8.0/planutils/packages/dual-bfws-fdparser/uninstall
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 14:40:16.225753 planutils-0.8.0/planutils/packages/dual-bfws-ffparser/
--rwxr-xr-x   0 runner    (1001) docker     (123)       31 2023-02-24 14:39:59.000000 planutils-0.8.0/planutils/packages/dual-bfws-ffparser/install
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-02-24 14:39:59.000000 planutils-0.8.0/planutils/packages/dual-bfws-ffparser/manifest.json
--rwxr-xr-x   0 runner    (1001) docker     (123)       85 2023-02-24 14:39:59.000000 planutils-0.8.0/planutils/packages/dual-bfws-ffparser/run
--rwxr-xr-x   0 runner    (1001) docker     (123)       31 2023-02-24 14:39:59.000000 planutils-0.8.0/planutils/packages/dual-bfws-ffparser/uninstall
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 14:40:16.225753 planutils-0.8.0/planutils/packages/enhsp/
--rwxr-xr-x   0 runner    (1001) docker     (123)       29 2023-02-24 14:39:59.000000 planutils-0.8.0/planutils/packages/enhsp/install
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-02-24 14:39:59.000000 planutils-0.8.0/planutils/packages/enhsp/manifest.json
--rwxr-xr-x   0 runner    (1001) docker     (123)       44 2023-02-24 14:39:59.000000 planutils-0.8.0/planutils/packages/enhsp/run
--rwxr-xr-x   0 runner    (1001) docker     (123)       29 2023-02-24 14:39:59.000000 planutils-0.8.0/planutils/packages/enhsp/uninstall
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 14:40:16.225753 planutils-0.8.0/planutils/packages/enhsp-2018/
--rwxr-xr-x   0 runner    (1001) docker     (123)       80 2023-02-24 14:39:59.000000 planutils-0.8.0/planutils/packages/enhsp-2018/install
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-02-24 14:39:59.000000 planutils-0.8.0/planutils/packages/enhsp-2018/manifest.json
--rwxr-xr-x   0 runner    (1001) docker     (123)       64 2023-02-24 14:39:59.000000 planutils-0.8.0/planutils/packages/enhsp-2018/run
--rwxr-xr-x   0 runner    (1001) docker     (123)       31 2023-02-24 14:39:59.000000 planutils-0.8.0/planutils/packages/enhsp-2018/uninstall
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 14:40:16.225753 planutils-0.8.0/planutils/packages/enhsp-2019/
--rwxr-xr-x   0 runner    (1001) docker     (123)       80 2023-02-24 14:39:59.000000 planutils-0.8.0/planutils/packages/enhsp-2019/install
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-02-24 14:39:59.000000 planutils-0.8.0/planutils/packages/enhsp-2019/manifest.json
--rwxr-xr-x   0 runner    (1001) docker     (123)       64 2023-02-24 14:39:59.000000 planutils-0.8.0/planutils/packages/enhsp-2019/run
--rwxr-xr-x   0 runner    (1001) docker     (123)       31 2023-02-24 14:39:59.000000 planutils-0.8.0/planutils/packages/enhsp-2019/uninstall
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 14:40:16.229753 planutils-0.8.0/planutils/packages/enhsp-2020/
--rwxr-xr-x   0 runner    (1001) docker     (123)       80 2023-02-24 14:39:59.000000 planutils-0.8.0/planutils/packages/enhsp-2020/install
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-02-24 14:39:59.000000 planutils-0.8.0/planutils/packages/enhsp-2020/manifest.json
--rwxr-xr-x   0 runner    (1001) docker     (123)       64 2023-02-24 14:39:59.000000 planutils-0.8.0/planutils/packages/enhsp-2020/run
--rwxr-xr-x   0 runner    (1001) docker     (123)       31 2023-02-24 14:39:59.000000 planutils-0.8.0/planutils/packages/enhsp-2020/uninstall
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 14:40:16.229753 planutils-0.8.0/planutils/packages/ff/
--rwxr-xr-x   0 runner    (1001) docker     (123)      137 2023-02-24 14:39:59.000000 planutils-0.8.0/planutils/packages/ff/install
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-02-24 14:39:59.000000 planutils-0.8.0/planutils/packages/ff/manifest.json
--rwxr-xr-x   0 runner    (1001) docker     (123)      988 2023-02-24 14:39:59.000000 planutils-0.8.0/planutils/packages/ff/run
--rwxr-xr-x   0 runner    (1001) docker     (123)       37 2023-02-24 14:39:59.000000 planutils-0.8.0/planutils/packages/ff/uninstall
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 14:40:16.229753 planutils-0.8.0/planutils/packages/fond4ltlf/
--rwxr-xr-x   0 runner    (1001) docker     (123)       87 2023-02-24 14:39:59.000000 planutils-0.8.0/planutils/packages/fond4ltlf/install
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-02-24 14:39:59.000000 planutils-0.8.0/planutils/packages/fond4ltlf/manifest.json
--rwxr-xr-x   0 runner    (1001) docker     (123)       61 2023-02-24 14:39:59.000000 planutils-0.8.0/planutils/packages/fond4ltlf/run
--rwxr-xr-x   0 runner    (1001) docker     (123)       30 2023-02-24 14:39:59.000000 planutils-0.8.0/planutils/packages/fond4ltlf/uninstall
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 14:40:16.229753 planutils-0.8.0/planutils/packages/forbiditerative/
--rwxr-xr-x   0 runner    (1001) docker     (123)       89 2023-02-24 14:39:59.000000 planutils-0.8.0/planutils/packages/forbiditerative/install
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-02-24 14:39:59.000000 planutils-0.8.0/planutils/packages/forbiditerative/manifest.json
--rwxr-xr-x   0 runner    (1001) docker     (123)       69 2023-02-24 14:39:59.000000 planutils-0.8.0/planutils/packages/forbiditerative/run
--rwxr-xr-x   0 runner    (1001) docker     (123)       36 2023-02-24 14:39:59.000000 planutils-0.8.0/planutils/packages/forbiditerative/uninstall
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 14:40:16.233753 planutils-0.8.0/planutils/packages/forbiditerative-diverse-agl/
--rwxr-xr-x   0 runner    (1001) docker     (123)       30 2023-02-24 14:39:59.000000 planutils-0.8.0/planutils/packages/forbiditerative-diverse-agl/install
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-02-24 14:39:59.000000 planutils-0.8.0/planutils/packages/forbiditerative-diverse-agl/manifest.json
--rwxr-xr-x   0 runner    (1001) docker     (123)      120 2023-02-24 14:39:59.000000 planutils-0.8.0/planutils/packages/forbiditerative-diverse-agl/run
--rwxr-xr-x   0 runner    (1001) docker     (123)       30 2023-02-24 14:39:59.000000 planutils-0.8.0/planutils/packages/forbiditerative-diverse-agl/uninstall
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 14:40:16.233753 planutils-0.8.0/planutils/packages/forbiditerative-diverse-sat/
--rwxr-xr-x   0 runner    (1001) docker     (123)       30 2023-02-24 14:39:59.000000 planutils-0.8.0/planutils/packages/forbiditerative-diverse-sat/install
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-02-24 14:39:59.000000 planutils-0.8.0/planutils/packages/forbiditerative-diverse-sat/manifest.json
--rwxr-xr-x   0 runner    (1001) docker     (123)      313 2023-02-24 14:39:59.000000 planutils-0.8.0/planutils/packages/forbiditerative-diverse-sat/run
--rwxr-xr-x   0 runner    (1001) docker     (123)       30 2023-02-24 14:39:59.000000 planutils-0.8.0/planutils/packages/forbiditerative-diverse-sat/uninstall
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 14:40:16.233753 planutils-0.8.0/planutils/packages/forbiditerative-topk/
--rwxr-xr-x   0 runner    (1001) docker     (123)       30 2023-02-24 14:39:59.000000 planutils-0.8.0/planutils/packages/forbiditerative-topk/install
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-02-24 14:39:59.000000 planutils-0.8.0/planutils/packages/forbiditerative-topk/manifest.json
--rwxr-xr-x   0 runner    (1001) docker     (123)      204 2023-02-24 14:39:59.000000 planutils-0.8.0/planutils/packages/forbiditerative-topk/run
--rwxr-xr-x   0 runner    (1001) docker     (123)       30 2023-02-24 14:39:59.000000 planutils-0.8.0/planutils/packages/forbiditerative-topk/uninstall
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 14:40:16.233753 planutils-0.8.0/planutils/packages/forbiditerative-topq/
--rwxr-xr-x   0 runner    (1001) docker     (123)       30 2023-02-24 14:39:59.000000 planutils-0.8.0/planutils/packages/forbiditerative-topq/install
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-02-24 14:39:59.000000 planutils-0.8.0/planutils/packages/forbiditerative-topq/manifest.json
--rwxr-xr-x   0 runner    (1001) docker     (123)      116 2023-02-24 14:39:59.000000 planutils-0.8.0/planutils/packages/forbiditerative-topq/run
--rwxr-xr-x   0 runner    (1001) docker     (123)       30 2023-02-24 14:39:59.000000 planutils-0.8.0/planutils/packages/forbiditerative-topq/uninstall
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 14:40:16.237753 planutils-0.8.0/planutils/packages/hpddl2pddl/
--rwxr-xr-x   0 runner    (1001) docker     (123)      142 2023-02-24 14:39:59.000000 planutils-0.8.0/planutils/packages/hpddl2pddl/install
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-02-24 14:39:59.000000 planutils-0.8.0/planutils/packages/hpddl2pddl/manifest.json
--rwxr-xr-x   0 runner    (1001) docker     (123)       72 2023-02-24 14:39:59.000000 planutils-0.8.0/planutils/packages/hpddl2pddl/run
--rwxr-xr-x   0 runner    (1001) docker     (123)       39 2023-02-24 14:39:59.000000 planutils-0.8.0/planutils/packages/hpddl2pddl/uninstall
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 14:40:16.237753 planutils-0.8.0/planutils/packages/kstar/
--rwxr-xr-x   0 runner    (1001) docker     (123)       70 2023-02-24 14:39:59.000000 planutils-0.8.0/planutils/packages/kstar/install
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-02-24 14:39:59.000000 planutils-0.8.0/planutils/packages/kstar/manifest.json
--rwxr-xr-x   0 runner    (1001) docker     (123)       59 2023-02-24 14:39:59.000000 planutils-0.8.0/planutils/packages/kstar/run
--rwxr-xr-x   0 runner    (1001) docker     (123)       26 2023-02-24 14:39:59.000000 planutils-0.8.0/planutils/packages/kstar/uninstall
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 14:40:16.237753 planutils-0.8.0/planutils/packages/lama/
--rwxr-xr-x   0 runner    (1001) docker     (123)       30 2023-02-24 14:39:59.000000 planutils-0.8.0/planutils/packages/lama/install
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-02-24 14:39:59.000000 planutils-0.8.0/planutils/packages/lama/manifest.json
--rwxr-xr-x   0 runner    (1001) docker     (123)       55 2023-02-24 14:39:59.000000 planutils-0.8.0/planutils/packages/lama/run
--rwxr-xr-x   0 runner    (1001) docker     (123)       30 2023-02-24 14:39:59.000000 planutils-0.8.0/planutils/packages/lama/uninstall
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 14:40:16.237753 planutils-0.8.0/planutils/packages/lama-first/
--rwxr-xr-x   0 runner    (1001) docker     (123)       30 2023-02-24 14:39:59.000000 planutils-0.8.0/planutils/packages/lama-first/install
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-02-24 14:39:59.000000 planutils-0.8.0/planutils/packages/lama-first/manifest.json
--rwxr-xr-x   0 runner    (1001) docker     (123)       61 2023-02-24 14:39:59.000000 planutils-0.8.0/planutils/packages/lama-first/run
--rwxr-xr-x   0 runner    (1001) docker     (123)       30 2023-02-24 14:39:59.000000 planutils-0.8.0/planutils/packages/lama-first/uninstall
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 14:40:16.237753 planutils-0.8.0/planutils/packages/lapkt/
--rwxr-xr-x   0 runner    (1001) docker     (123)      135 2023-02-24 14:39:59.000000 planutils-0.8.0/planutils/packages/lapkt/install
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-02-24 14:39:59.000000 planutils-0.8.0/planutils/packages/lapkt/manifest.json
--rwxr-xr-x   0 runner    (1001) docker     (123)       59 2023-02-24 14:39:59.000000 planutils-0.8.0/planutils/packages/lapkt/run
--rwxr-xr-x   0 runner    (1001) docker     (123)       24 2023-02-24 14:39:59.000000 planutils-0.8.0/planutils/packages/lapkt/uninstall
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 14:40:16.241754 planutils-0.8.0/planutils/packages/lpg-td/
--rwxr-xr-x   0 runner    (1001) docker     (123)      161 2023-02-24 14:39:59.000000 planutils-0.8.0/planutils/packages/lpg-td/install
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-02-24 14:39:59.000000 planutils-0.8.0/planutils/packages/lpg-td/manifest.json
--rwxr-xr-x   0 runner    (1001) docker     (123)     1305 2023-02-24 14:39:59.000000 planutils-0.8.0/planutils/packages/lpg-td/run
--rwxr-xr-x   0 runner    (1001) docker     (123)       41 2023-02-24 14:39:59.000000 planutils-0.8.0/planutils/packages/lpg-td/uninstall
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 14:40:16.241754 planutils-0.8.0/planutils/packages/machetli/
--rwxr-xr-x   0 runner    (1001) docker     (123)       68 2023-02-24 14:39:59.000000 planutils-0.8.0/planutils/packages/machetli/install
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-02-24 14:39:59.000000 planutils-0.8.0/planutils/packages/machetli/manifest.json
--rwxr-xr-x   0 runner    (1001) docker     (123)       37 2023-02-24 14:39:59.000000 planutils-0.8.0/planutils/packages/machetli/uninstall
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 14:40:16.241754 planutils-0.8.0/planutils/packages/macq/
--rwxr-xr-x   0 runner    (1001) docker     (123)       64 2023-02-24 14:39:59.000000 planutils-0.8.0/planutils/packages/macq/install
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-02-24 14:39:59.000000 planutils-0.8.0/planutils/packages/macq/manifest.json
--rwxr-xr-x   0 runner    (1001) docker     (123)       33 2023-02-24 14:39:59.000000 planutils-0.8.0/planutils/packages/macq/uninstall
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 14:40:16.241754 planutils-0.8.0/planutils/packages/metric-ff/
--rwxr-xr-x   0 runner    (1001) docker     (123)      145 2023-02-24 14:39:59.000000 planutils-0.8.0/planutils/packages/metric-ff/install
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-02-24 14:39:59.000000 planutils-0.8.0/planutils/packages/metric-ff/manifest.json
--rwxr-xr-x   0 runner    (1001) docker     (123)      988 2023-02-24 14:39:59.000000 planutils-0.8.0/planutils/packages/metric-ff/run
--rwxr-xr-x   0 runner    (1001) docker     (123)       37 2023-02-24 14:39:59.000000 planutils-0.8.0/planutils/packages/metric-ff/uninstall
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 14:40:16.245754 planutils-0.8.0/planutils/packages/optic/
--rwxr-xr-x   0 runner    (1001) docker     (123)      512 2023-02-24 14:39:59.000000 planutils-0.8.0/planutils/packages/optic/install
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-02-24 14:39:59.000000 planutils-0.8.0/planutils/packages/optic/manifest.json
--rwxr-xr-x   0 runner    (1001) docker     (123)      128 2023-02-24 14:39:59.000000 planutils-0.8.0/planutils/packages/optic/run
--rwxr-xr-x   0 runner    (1001) docker     (123)       26 2023-02-24 14:39:59.000000 planutils-0.8.0/planutils/packages/optic/uninstall
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 14:40:16.245754 planutils-0.8.0/planutils/packages/planning.domains/
--rwxr-xr-x   0 runner    (1001) docker     (123)       69 2023-02-24 14:39:59.000000 planutils-0.8.0/planutils/packages/planning.domains/install
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-02-24 14:39:59.000000 planutils-0.8.0/planutils/packages/planning.domains/manifest.json
--rwxr-xr-x   0 runner    (1001) docker     (123)       68 2023-02-24 14:39:59.000000 planutils-0.8.0/planutils/packages/planning.domains/run
--rwxr-xr-x   0 runner    (1001) docker     (123)       83 2023-02-24 14:39:59.000000 planutils-0.8.0/planutils/packages/planning.domains/uninstall
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 14:40:16.245754 planutils-0.8.0/planutils/packages/popf/
--rwxr-xr-x   0 runner    (1001) docker     (123)      153 2023-02-24 14:39:59.000000 planutils-0.8.0/planutils/packages/popf/install
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-02-24 14:39:59.000000 planutils-0.8.0/planutils/packages/popf/manifest.json
--rwxr-xr-x   0 runner    (1001) docker     (123)       58 2023-02-24 14:39:59.000000 planutils-0.8.0/planutils/packages/popf/run
--rwxr-xr-x   0 runner    (1001) docker     (123)       25 2023-02-24 14:39:59.000000 planutils-0.8.0/planutils/packages/popf/uninstall
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 14:40:16.245754 planutils-0.8.0/planutils/packages/poprp/
--rwxr-xr-x   0 runner    (1001) docker     (123)       72 2023-02-24 14:39:59.000000 planutils-0.8.0/planutils/packages/poprp/install
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-02-24 14:39:59.000000 planutils-0.8.0/planutils/packages/poprp/manifest.json
--rwxr-xr-x   0 runner    (1001) docker     (123)       57 2023-02-24 14:39:59.000000 planutils-0.8.0/planutils/packages/poprp/run
--rwxr-xr-x   0 runner    (1001) docker     (123)       26 2023-02-24 14:39:59.000000 planutils-0.8.0/planutils/packages/poprp/uninstall
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 14:40:16.249754 planutils-0.8.0/planutils/packages/prp/
--rwxr-xr-x   0 runner    (1001) docker     (123)       68 2023-02-24 14:39:59.000000 planutils-0.8.0/planutils/packages/prp/install
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-02-24 14:39:59.000000 planutils-0.8.0/planutils/packages/prp/manifest.json
--rwxr-xr-x   0 runner    (1001) docker     (123)       55 2023-02-24 14:39:59.000000 planutils-0.8.0/planutils/packages/prp/run
--rwxr-xr-x   0 runner    (1001) docker     (123)       24 2023-02-24 14:39:59.000000 planutils-0.8.0/planutils/packages/prp/uninstall
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 14:40:16.249754 planutils-0.8.0/planutils/packages/pyperplan/
--rwxr-xr-x   0 runner    (1001) docker     (123)       46 2023-02-24 14:39:59.000000 planutils-0.8.0/planutils/packages/pyperplan/install
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-02-24 14:39:59.000000 planutils-0.8.0/planutils/packages/pyperplan/manifest.json
--rwxr-xr-x   0 runner    (1001) docker     (123)       26 2023-02-24 14:39:59.000000 planutils-0.8.0/planutils/packages/pyperplan/run
--rwxr-xr-x   0 runner    (1001) docker     (123)       48 2023-02-24 14:39:59.000000 planutils-0.8.0/planutils/packages/pyperplan/uninstall
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 14:40:16.249754 planutils-0.8.0/planutils/packages/scorpion/
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-02-24 14:39:59.000000 planutils-0.8.0/planutils/packages/scorpion/.gitignore
--rwxr-xr-x   0 runner    (1001) docker     (123)       87 2023-02-24 14:39:59.000000 planutils-0.8.0/planutils/packages/scorpion/install
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-02-24 14:39:59.000000 planutils-0.8.0/planutils/packages/scorpion/manifest.json
--rwxr-xr-x   0 runner    (1001) docker     (123)      110 2023-02-24 14:39:59.000000 planutils-0.8.0/planutils/packages/scorpion/run
--rwxr-xr-x   0 runner    (1001) docker     (123)       29 2023-02-24 14:39:59.000000 planutils-0.8.0/planutils/packages/scorpion/uninstall
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 14:40:16.249754 planutils-0.8.0/planutils/packages/smtplan/
--rwxr-xr-x   0 runner    (1001) docker     (123)       91 2023-02-24 14:39:59.000000 planutils-0.8.0/planutils/packages/smtplan/install
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-02-24 14:39:59.000000 planutils-0.8.0/planutils/packages/smtplan/manifest.json
--rwxr-xr-x   0 runner    (1001) docker     (123)       70 2023-02-24 14:39:59.000000 planutils-0.8.0/planutils/packages/smtplan/run
--rwxr-xr-x   0 runner    (1001) docker     (123)       28 2023-02-24 14:39:59.000000 planutils-0.8.0/planutils/packages/smtplan/uninstall
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 14:40:16.253754 planutils-0.8.0/planutils/packages/symk/
--rwxr-xr-x   0 runner    (1001) docker     (123)       77 2023-02-24 14:39:59.000000 planutils-0.8.0/planutils/packages/symk/install
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-02-24 14:39:59.000000 planutils-0.8.0/planutils/packages/symk/manifest.json
--rwxr-xr-x   0 runner    (1001) docker     (123)       58 2023-02-24 14:39:59.000000 planutils-0.8.0/planutils/packages/symk/run
--rwxr-xr-x   0 runner    (1001) docker     (123)       25 2023-02-24 14:39:59.000000 planutils-0.8.0/planutils/packages/symk/uninstall
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 14:40:16.253754 planutils-0.8.0/planutils/packages/tarski/
--rwxr-xr-x   0 runner    (1001) docker     (123)      176 2023-02-24 14:39:59.000000 planutils-0.8.0/planutils/packages/tarski/install
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-02-24 14:39:59.000000 planutils-0.8.0/planutils/packages/tarski/manifest.json
--rwxr-xr-x   0 runner    (1001) docker     (123)       35 2023-02-24 14:39:59.000000 planutils-0.8.0/planutils/packages/tarski/uninstall
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 14:40:16.253754 planutils-0.8.0/planutils/packages/tfd/
--rwxr-xr-x   0 runner    (1001) docker     (123)      131 2023-02-24 14:39:59.000000 planutils-0.8.0/planutils/packages/tfd/install
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-02-24 14:39:59.000000 planutils-0.8.0/planutils/packages/tfd/manifest.json
--rwxr-xr-x   0 runner    (1001) docker     (123)       56 2023-02-24 14:39:59.000000 planutils-0.8.0/planutils/packages/tfd/run
--rwxr-xr-x   0 runner    (1001) docker     (123)       24 2023-02-24 14:39:59.000000 planutils-0.8.0/planutils/packages/tfd/uninstall
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 14:40:16.253754 planutils-0.8.0/planutils/packages/val/
--rwxr-xr-x   0 runner    (1001) docker     (123)      323 2023-02-24 14:39:59.000000 planutils-0.8.0/planutils/packages/val/install
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-02-24 14:39:59.000000 planutils-0.8.0/planutils/packages/val/manifest.json
--rwxr-xr-x   0 runner    (1001) docker     (123)      282 2023-02-24 14:39:59.000000 planutils-0.8.0/planutils/packages/val/run
--rwxr-xr-x   0 runner    (1001) docker     (123)       38 2023-02-24 14:39:59.000000 planutils-0.8.0/planutils/packages/val/uninstall
--rw-r--r--   0 runner    (1001) docker     (123)     7037 2023-02-24 14:39:59.000000 planutils-0.8.0/planutils/server.py
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-02-24 14:39:59.000000 planutils-0.8.0/planutils/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 14:40:16.213752 planutils-0.8.0/planutils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6225 2023-02-24 14:40:16.000000 planutils-0.8.0/planutils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6733 2023-02-24 14:40:16.000000 planutils-0.8.0/planutils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-24 14:40:16.000000 planutils-0.8.0/planutils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-24 14:40:15.000000 planutils-0.8.0/planutils.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-02-24 14:40:16.000000 planutils-0.8.0/planutils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-02-24 14:40:16.000000 planutils-0.8.0/planutils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-24 14:40:16.253754 planutils-0.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-02-24 14:39:59.000000 planutils-0.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 15:01:05.066416 planutils-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-03-06 15:00:55.000000 planutils-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-06 15:00:55.000000 planutils-0.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6225 2023-03-06 15:01:05.066416 planutils-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5736 2023-03-06 15:00:55.000000 planutils-0.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 15:01:05.042415 planutils-0.9.0/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      646 2023-03-06 15:00:55.000000 planutils-0.9.0/bin/planutils
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 15:01:05.042415 planutils-0.9.0/planutils/
+-rw-r--r--   0 runner    (1001) docker     (123)     6637 2023-03-06 15:00:55.000000 planutils-0.9.0/planutils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3021 2023-03-06 15:00:55.000000 planutils-0.9.0/planutils/manifest_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9465 2023-03-06 15:00:55.000000 planutils-0.9.0/planutils/package_installation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 15:01:05.042415 planutils-0.9.0/planutils/packages/
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-03-06 15:00:55.000000 planutils-0.9.0/planutils/packages/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 15:01:05.046415 planutils-0.9.0/planutils/packages/TEMPLATE/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 15:01:05.046415 planutils-0.9.0/planutils/packages/TEMPLATE/SERVICE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-03-06 15:00:55.000000 planutils-0.9.0/planutils/packages/TEMPLATE/SERVICE_TEMPLATE/planner.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)      459 2023-03-06 15:00:55.000000 planutils-0.9.0/planutils/packages/TEMPLATE/install
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-03-06 15:00:55.000000 planutils-0.9.0/planutils/packages/TEMPLATE/manifest.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)       81 2023-03-06 15:00:55.000000 planutils-0.9.0/planutils/packages/TEMPLATE/run
+-rwxr-xr-x   0 runner    (1001) docker     (123)      474 2023-03-06 15:00:55.000000 planutils-0.9.0/planutils/packages/TEMPLATE/uninstall
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 15:01:05.046415 planutils-0.9.0/planutils/packages/cerberus/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       92 2023-03-06 15:00:55.000000 planutils-0.9.0/planutils/packages/cerberus/install
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-03-06 15:00:55.000000 planutils-0.9.0/planutils/packages/cerberus/manifest.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)       62 2023-03-06 15:00:55.000000 planutils-0.9.0/planutils/packages/cerberus/run
+-rwxr-xr-x   0 runner    (1001) docker     (123)       29 2023-03-06 15:00:55.000000 planutils-0.9.0/planutils/packages/cerberus/uninstall
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 15:01:05.046415 planutils-0.9.0/planutils/packages/cerberus-agl/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       30 2023-03-06 15:00:55.000000 planutils-0.9.0/planutils/packages/cerberus-agl/install
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-03-06 15:00:55.000000 planutils-0.9.0/planutils/packages/cerberus-agl/manifest.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)       99 2023-03-06 15:00:55.000000 planutils-0.9.0/planutils/packages/cerberus-agl/run
+-rwxr-xr-x   0 runner    (1001) docker     (123)       30 2023-03-06 15:00:55.000000 planutils-0.9.0/planutils/packages/cerberus-agl/uninstall
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 15:01:05.046415 planutils-0.9.0/planutils/packages/cerberus-sat/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       30 2023-03-06 15:00:55.000000 planutils-0.9.0/planutils/packages/cerberus-sat/install
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-03-06 15:00:55.000000 planutils-0.9.0/planutils/packages/cerberus-sat/manifest.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)       99 2023-03-06 15:00:55.000000 planutils-0.9.0/planutils/packages/cerberus-sat/run
+-rwxr-xr-x   0 runner    (1001) docker     (123)       30 2023-03-06 15:00:55.000000 planutils-0.9.0/planutils/packages/cerberus-sat/uninstall
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 15:01:05.046415 planutils-0.9.0/planutils/packages/cpor/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2463 2023-03-06 15:00:55.000000 planutils-0.9.0/planutils/packages/cpor/Dockerfile
+-rwxr-xr-x   0 runner    (1001) docker     (123)       70 2023-03-06 15:00:55.000000 planutils-0.9.0/planutils/packages/cpor/install
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-03-06 15:00:55.000000 planutils-0.9.0/planutils/packages/cpor/manifest.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)       56 2023-03-06 15:00:55.000000 planutils-0.9.0/planutils/packages/cpor/run
+-rwxr-xr-x   0 runner    (1001) docker     (123)       25 2023-03-06 15:00:55.000000 planutils-0.9.0/planutils/packages/cpor/uninstall
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 15:01:05.046415 planutils-0.9.0/planutils/packages/delfi/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       77 2023-03-06 15:00:55.000000 planutils-0.9.0/planutils/packages/delfi/install
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-03-06 15:00:55.000000 planutils-0.9.0/planutils/packages/delfi/manifest.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)       59 2023-03-06 15:00:55.000000 planutils-0.9.0/planutils/packages/delfi/run
+-rwxr-xr-x   0 runner    (1001) docker     (123)       26 2023-03-06 15:00:55.000000 planutils-0.9.0/planutils/packages/delfi/uninstall
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 15:01:05.046415 planutils-0.9.0/planutils/packages/downward/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       75 2023-03-06 15:00:55.000000 planutils-0.9.0/planutils/packages/downward/install
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-03-06 15:00:55.000000 planutils-0.9.0/planutils/packages/downward/manifest.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)       62 2023-03-06 15:00:55.000000 planutils-0.9.0/planutils/packages/downward/run
+-rwxr-xr-x   0 runner    (1001) docker     (123)       29 2023-03-06 15:00:55.000000 planutils-0.9.0/planutils/packages/downward/uninstall
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 15:01:05.046415 planutils-0.9.0/planutils/packages/dual-bfws-fdparser/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       31 2023-03-06 15:00:55.000000 planutils-0.9.0/planutils/packages/dual-bfws-fdparser/install
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-03-06 15:00:55.000000 planutils-0.9.0/planutils/packages/dual-bfws-fdparser/manifest.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)      132 2023-03-06 15:00:55.000000 planutils-0.9.0/planutils/packages/dual-bfws-fdparser/run
+-rwxr-xr-x   0 runner    (1001) docker     (123)       31 2023-03-06 15:00:55.000000 planutils-0.9.0/planutils/packages/dual-bfws-fdparser/uninstall
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 15:01:05.050415 planutils-0.9.0/planutils/packages/dual-bfws-ffparser/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       31 2023-03-06 15:00:55.000000 planutils-0.9.0/planutils/packages/dual-bfws-ffparser/install
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-03-06 15:00:55.000000 planutils-0.9.0/planutils/packages/dual-bfws-ffparser/manifest.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)      149 2023-03-06 15:00:55.000000 planutils-0.9.0/planutils/packages/dual-bfws-ffparser/run
+-rwxr-xr-x   0 runner    (1001) docker     (123)       31 2023-03-06 15:00:55.000000 planutils-0.9.0/planutils/packages/dual-bfws-ffparser/uninstall
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 15:01:05.050415 planutils-0.9.0/planutils/packages/enhsp/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       29 2023-03-06 15:00:55.000000 planutils-0.9.0/planutils/packages/enhsp/install
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-03-06 15:00:55.000000 planutils-0.9.0/planutils/packages/enhsp/manifest.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)       44 2023-03-06 15:00:55.000000 planutils-0.9.0/planutils/packages/enhsp/run
+-rwxr-xr-x   0 runner    (1001) docker     (123)       29 2023-03-06 15:00:55.000000 planutils-0.9.0/planutils/packages/enhsp/uninstall
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 15:01:05.050415 planutils-0.9.0/planutils/packages/enhsp-2018/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       80 2023-03-06 15:00:55.000000 planutils-0.9.0/planutils/packages/enhsp-2018/install
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-03-06 15:00:55.000000 planutils-0.9.0/planutils/packages/enhsp-2018/manifest.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)       64 2023-03-06 15:00:55.000000 planutils-0.9.0/planutils/packages/enhsp-2018/run
+-rwxr-xr-x   0 runner    (1001) docker     (123)       31 2023-03-06 15:00:55.000000 planutils-0.9.0/planutils/packages/enhsp-2018/uninstall
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 15:01:05.050415 planutils-0.9.0/planutils/packages/enhsp-2019/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       80 2023-03-06 15:00:55.000000 planutils-0.9.0/planutils/packages/enhsp-2019/install
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-03-06 15:00:55.000000 planutils-0.9.0/planutils/packages/enhsp-2019/manifest.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)       64 2023-03-06 15:00:55.000000 planutils-0.9.0/planutils/packages/enhsp-2019/run
+-rwxr-xr-x   0 runner    (1001) docker     (123)       31 2023-03-06 15:00:55.000000 planutils-0.9.0/planutils/packages/enhsp-2019/uninstall
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 15:01:05.050415 planutils-0.9.0/planutils/packages/enhsp-2020/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       80 2023-03-06 15:00:55.000000 planutils-0.9.0/planutils/packages/enhsp-2020/install
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-03-06 15:00:55.000000 planutils-0.9.0/planutils/packages/enhsp-2020/manifest.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)       64 2023-03-06 15:00:55.000000 planutils-0.9.0/planutils/packages/enhsp-2020/run
+-rwxr-xr-x   0 runner    (1001) docker     (123)       31 2023-03-06 15:00:55.000000 planutils-0.9.0/planutils/packages/enhsp-2020/uninstall
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 15:01:05.050415 planutils-0.9.0/planutils/packages/ff/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      137 2023-03-06 15:00:55.000000 planutils-0.9.0/planutils/packages/ff/install
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-03-06 15:00:55.000000 planutils-0.9.0/planutils/packages/ff/manifest.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)      988 2023-03-06 15:00:55.000000 planutils-0.9.0/planutils/packages/ff/run
+-rwxr-xr-x   0 runner    (1001) docker     (123)       37 2023-03-06 15:00:55.000000 planutils-0.9.0/planutils/packages/ff/uninstall
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 15:01:05.050415 planutils-0.9.0/planutils/packages/fond4ltlf/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       87 2023-03-06 15:00:55.000000 planutils-0.9.0/planutils/packages/fond4ltlf/install
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-03-06 15:00:55.000000 planutils-0.9.0/planutils/packages/fond4ltlf/manifest.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)       61 2023-03-06 15:00:55.000000 planutils-0.9.0/planutils/packages/fond4ltlf/run
+-rwxr-xr-x   0 runner    (1001) docker     (123)       30 2023-03-06 15:00:55.000000 planutils-0.9.0/planutils/packages/fond4ltlf/uninstall
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 15:01:05.050415 planutils-0.9.0/planutils/packages/forbiditerative/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       89 2023-03-06 15:00:55.000000 planutils-0.9.0/planutils/packages/forbiditerative/install
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-03-06 15:00:55.000000 planutils-0.9.0/planutils/packages/forbiditerative/manifest.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)       69 2023-03-06 15:00:55.000000 planutils-0.9.0/planutils/packages/forbiditerative/run
+-rwxr-xr-x   0 runner    (1001) docker     (123)       36 2023-03-06 15:00:55.000000 planutils-0.9.0/planutils/packages/forbiditerative/uninstall
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 15:01:05.054415 planutils-0.9.0/planutils/packages/forbiditerative-diverse-agl/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       30 2023-03-06 15:00:55.000000 planutils-0.9.0/planutils/packages/forbiditerative-diverse-agl/install
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-03-06 15:00:55.000000 planutils-0.9.0/planutils/packages/forbiditerative-diverse-agl/manifest.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)      120 2023-03-06 15:00:55.000000 planutils-0.9.0/planutils/packages/forbiditerative-diverse-agl/run
+-rwxr-xr-x   0 runner    (1001) docker     (123)       30 2023-03-06 15:00:55.000000 planutils-0.9.0/planutils/packages/forbiditerative-diverse-agl/uninstall
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 15:01:05.054415 planutils-0.9.0/planutils/packages/forbiditerative-diverse-sat/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       30 2023-03-06 15:00:55.000000 planutils-0.9.0/planutils/packages/forbiditerative-diverse-sat/install
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-03-06 15:00:55.000000 planutils-0.9.0/planutils/packages/forbiditerative-diverse-sat/manifest.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)      313 2023-03-06 15:00:55.000000 planutils-0.9.0/planutils/packages/forbiditerative-diverse-sat/run
+-rwxr-xr-x   0 runner    (1001) docker     (123)       30 2023-03-06 15:00:55.000000 planutils-0.9.0/planutils/packages/forbiditerative-diverse-sat/uninstall
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 15:01:05.054415 planutils-0.9.0/planutils/packages/forbiditerative-topk/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       30 2023-03-06 15:00:55.000000 planutils-0.9.0/planutils/packages/forbiditerative-topk/install
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-03-06 15:00:55.000000 planutils-0.9.0/planutils/packages/forbiditerative-topk/manifest.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)      204 2023-03-06 15:00:55.000000 planutils-0.9.0/planutils/packages/forbiditerative-topk/run
+-rwxr-xr-x   0 runner    (1001) docker     (123)       30 2023-03-06 15:00:55.000000 planutils-0.9.0/planutils/packages/forbiditerative-topk/uninstall
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 15:01:05.054415 planutils-0.9.0/planutils/packages/forbiditerative-topq/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       30 2023-03-06 15:00:55.000000 planutils-0.9.0/planutils/packages/forbiditerative-topq/install
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-03-06 15:00:55.000000 planutils-0.9.0/planutils/packages/forbiditerative-topq/manifest.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)      116 2023-03-06 15:00:55.000000 planutils-0.9.0/planutils/packages/forbiditerative-topq/run
+-rwxr-xr-x   0 runner    (1001) docker     (123)       30 2023-03-06 15:00:55.000000 planutils-0.9.0/planutils/packages/forbiditerative-topq/uninstall
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 15:01:05.054415 planutils-0.9.0/planutils/packages/hpddl2pddl/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      142 2023-03-06 15:00:55.000000 planutils-0.9.0/planutils/packages/hpddl2pddl/install
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-03-06 15:00:55.000000 planutils-0.9.0/planutils/packages/hpddl2pddl/manifest.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)       72 2023-03-06 15:00:55.000000 planutils-0.9.0/planutils/packages/hpddl2pddl/run
+-rwxr-xr-x   0 runner    (1001) docker     (123)       39 2023-03-06 15:00:55.000000 planutils-0.9.0/planutils/packages/hpddl2pddl/uninstall
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 15:01:05.054415 planutils-0.9.0/planutils/packages/kstar/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       70 2023-03-06 15:00:55.000000 planutils-0.9.0/planutils/packages/kstar/install
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-03-06 15:00:55.000000 planutils-0.9.0/planutils/packages/kstar/manifest.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)       59 2023-03-06 15:00:55.000000 planutils-0.9.0/planutils/packages/kstar/run
+-rwxr-xr-x   0 runner    (1001) docker     (123)       26 2023-03-06 15:00:55.000000 planutils-0.9.0/planutils/packages/kstar/uninstall
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 15:01:05.054415 planutils-0.9.0/planutils/packages/lama/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       30 2023-03-06 15:00:55.000000 planutils-0.9.0/planutils/packages/lama/install
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-03-06 15:00:55.000000 planutils-0.9.0/planutils/packages/lama/manifest.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)       55 2023-03-06 15:00:55.000000 planutils-0.9.0/planutils/packages/lama/run
+-rwxr-xr-x   0 runner    (1001) docker     (123)       30 2023-03-06 15:00:55.000000 planutils-0.9.0/planutils/packages/lama/uninstall
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 15:01:05.058416 planutils-0.9.0/planutils/packages/lama-first/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       30 2023-03-06 15:00:55.000000 planutils-0.9.0/planutils/packages/lama-first/install
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-03-06 15:00:55.000000 planutils-0.9.0/planutils/packages/lama-first/manifest.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)       61 2023-03-06 15:00:55.000000 planutils-0.9.0/planutils/packages/lama-first/run
+-rwxr-xr-x   0 runner    (1001) docker     (123)       30 2023-03-06 15:00:55.000000 planutils-0.9.0/planutils/packages/lama-first/uninstall
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 15:01:05.058416 planutils-0.9.0/planutils/packages/lapkt/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      134 2023-03-06 15:00:55.000000 planutils-0.9.0/planutils/packages/lapkt/install
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-03-06 15:00:55.000000 planutils-0.9.0/planutils/packages/lapkt/manifest.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)       58 2023-03-06 15:00:55.000000 planutils-0.9.0/planutils/packages/lapkt/run
+-rwxr-xr-x   0 runner    (1001) docker     (123)       24 2023-03-06 15:00:55.000000 planutils-0.9.0/planutils/packages/lapkt/uninstall
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 15:01:05.058416 planutils-0.9.0/planutils/packages/lpg-td/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      161 2023-03-06 15:00:55.000000 planutils-0.9.0/planutils/packages/lpg-td/install
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-03-06 15:00:55.000000 planutils-0.9.0/planutils/packages/lpg-td/manifest.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1305 2023-03-06 15:00:55.000000 planutils-0.9.0/planutils/packages/lpg-td/run
+-rwxr-xr-x   0 runner    (1001) docker     (123)       41 2023-03-06 15:00:55.000000 planutils-0.9.0/planutils/packages/lpg-td/uninstall
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 15:01:05.058416 planutils-0.9.0/planutils/packages/machetli/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       68 2023-03-06 15:00:55.000000 planutils-0.9.0/planutils/packages/machetli/install
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-03-06 15:00:55.000000 planutils-0.9.0/planutils/packages/machetli/manifest.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)       37 2023-03-06 15:00:55.000000 planutils-0.9.0/planutils/packages/machetli/uninstall
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 15:01:05.058416 planutils-0.9.0/planutils/packages/macq/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       64 2023-03-06 15:00:55.000000 planutils-0.9.0/planutils/packages/macq/install
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-03-06 15:00:55.000000 planutils-0.9.0/planutils/packages/macq/manifest.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)       33 2023-03-06 15:00:55.000000 planutils-0.9.0/planutils/packages/macq/uninstall
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 15:01:05.058416 planutils-0.9.0/planutils/packages/metric-ff/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      145 2023-03-06 15:00:55.000000 planutils-0.9.0/planutils/packages/metric-ff/install
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-03-06 15:00:55.000000 planutils-0.9.0/planutils/packages/metric-ff/manifest.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)      988 2023-03-06 15:00:55.000000 planutils-0.9.0/planutils/packages/metric-ff/run
+-rwxr-xr-x   0 runner    (1001) docker     (123)       37 2023-03-06 15:00:55.000000 planutils-0.9.0/planutils/packages/metric-ff/uninstall
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 15:01:05.058416 planutils-0.9.0/planutils/packages/optic/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      512 2023-03-06 15:00:55.000000 planutils-0.9.0/planutils/packages/optic/install
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-03-06 15:00:55.000000 planutils-0.9.0/planutils/packages/optic/manifest.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)      128 2023-03-06 15:00:55.000000 planutils-0.9.0/planutils/packages/optic/run
+-rwxr-xr-x   0 runner    (1001) docker     (123)       26 2023-03-06 15:00:55.000000 planutils-0.9.0/planutils/packages/optic/uninstall
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 15:01:05.058416 planutils-0.9.0/planutils/packages/planning.domains/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       69 2023-03-06 15:00:55.000000 planutils-0.9.0/planutils/packages/planning.domains/install
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-03-06 15:00:55.000000 planutils-0.9.0/planutils/packages/planning.domains/manifest.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)       68 2023-03-06 15:00:55.000000 planutils-0.9.0/planutils/packages/planning.domains/run
+-rwxr-xr-x   0 runner    (1001) docker     (123)       83 2023-03-06 15:00:55.000000 planutils-0.9.0/planutils/packages/planning.domains/uninstall
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 15:01:05.058416 planutils-0.9.0/planutils/packages/popf/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      153 2023-03-06 15:00:55.000000 planutils-0.9.0/planutils/packages/popf/install
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-03-06 15:00:55.000000 planutils-0.9.0/planutils/packages/popf/manifest.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)       58 2023-03-06 15:00:55.000000 planutils-0.9.0/planutils/packages/popf/run
+-rwxr-xr-x   0 runner    (1001) docker     (123)       25 2023-03-06 15:00:55.000000 planutils-0.9.0/planutils/packages/popf/uninstall
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 15:01:05.062415 planutils-0.9.0/planutils/packages/poprp/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       72 2023-03-06 15:00:55.000000 planutils-0.9.0/planutils/packages/poprp/install
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-03-06 15:00:55.000000 planutils-0.9.0/planutils/packages/poprp/manifest.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)       57 2023-03-06 15:00:55.000000 planutils-0.9.0/planutils/packages/poprp/run
+-rwxr-xr-x   0 runner    (1001) docker     (123)       26 2023-03-06 15:00:55.000000 planutils-0.9.0/planutils/packages/poprp/uninstall
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 15:01:05.062415 planutils-0.9.0/planutils/packages/prp/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       68 2023-03-06 15:00:55.000000 planutils-0.9.0/planutils/packages/prp/install
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-03-06 15:00:55.000000 planutils-0.9.0/planutils/packages/prp/manifest.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)       55 2023-03-06 15:00:55.000000 planutils-0.9.0/planutils/packages/prp/run
+-rwxr-xr-x   0 runner    (1001) docker     (123)       24 2023-03-06 15:00:55.000000 planutils-0.9.0/planutils/packages/prp/uninstall
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 15:01:05.062415 planutils-0.9.0/planutils/packages/pyperplan/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       46 2023-03-06 15:00:55.000000 planutils-0.9.0/planutils/packages/pyperplan/install
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-03-06 15:00:55.000000 planutils-0.9.0/planutils/packages/pyperplan/manifest.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)       26 2023-03-06 15:00:55.000000 planutils-0.9.0/planutils/packages/pyperplan/run
+-rwxr-xr-x   0 runner    (1001) docker     (123)       48 2023-03-06 15:00:55.000000 planutils-0.9.0/planutils/packages/pyperplan/uninstall
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 15:01:05.062415 planutils-0.9.0/planutils/packages/rpmep/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       72 2023-03-06 15:00:55.000000 planutils-0.9.0/planutils/packages/rpmep/install
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-03-06 15:00:55.000000 planutils-0.9.0/planutils/packages/rpmep/manifest.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)       57 2023-03-06 15:00:55.000000 planutils-0.9.0/planutils/packages/rpmep/run
+-rwxr-xr-x   0 runner    (1001) docker     (123)       26 2023-03-06 15:00:55.000000 planutils-0.9.0/planutils/packages/rpmep/uninstall
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 15:01:05.062415 planutils-0.9.0/planutils/packages/scorpion/
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-03-06 15:00:55.000000 planutils-0.9.0/planutils/packages/scorpion/.gitignore
+-rwxr-xr-x   0 runner    (1001) docker     (123)       87 2023-03-06 15:00:55.000000 planutils-0.9.0/planutils/packages/scorpion/install
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-03-06 15:00:55.000000 planutils-0.9.0/planutils/packages/scorpion/manifest.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)      110 2023-03-06 15:00:55.000000 planutils-0.9.0/planutils/packages/scorpion/run
+-rwxr-xr-x   0 runner    (1001) docker     (123)       29 2023-03-06 15:00:55.000000 planutils-0.9.0/planutils/packages/scorpion/uninstall
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 15:01:05.062415 planutils-0.9.0/planutils/packages/smtplan/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       91 2023-03-06 15:00:55.000000 planutils-0.9.0/planutils/packages/smtplan/install
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-03-06 15:00:55.000000 planutils-0.9.0/planutils/packages/smtplan/manifest.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)       70 2023-03-06 15:00:55.000000 planutils-0.9.0/planutils/packages/smtplan/run
+-rwxr-xr-x   0 runner    (1001) docker     (123)       28 2023-03-06 15:00:55.000000 planutils-0.9.0/planutils/packages/smtplan/uninstall
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 15:01:05.062415 planutils-0.9.0/planutils/packages/symk/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       77 2023-03-06 15:00:55.000000 planutils-0.9.0/planutils/packages/symk/install
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-03-06 15:00:55.000000 planutils-0.9.0/planutils/packages/symk/manifest.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)       58 2023-03-06 15:00:55.000000 planutils-0.9.0/planutils/packages/symk/run
+-rwxr-xr-x   0 runner    (1001) docker     (123)       25 2023-03-06 15:00:55.000000 planutils-0.9.0/planutils/packages/symk/uninstall
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 15:01:05.062415 planutils-0.9.0/planutils/packages/tarski/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      176 2023-03-06 15:00:55.000000 planutils-0.9.0/planutils/packages/tarski/install
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-03-06 15:00:55.000000 planutils-0.9.0/planutils/packages/tarski/manifest.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)       35 2023-03-06 15:00:55.000000 planutils-0.9.0/planutils/packages/tarski/uninstall
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 15:01:05.066416 planutils-0.9.0/planutils/packages/tfd/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      131 2023-03-06 15:00:55.000000 planutils-0.9.0/planutils/packages/tfd/install
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-03-06 15:00:55.000000 planutils-0.9.0/planutils/packages/tfd/manifest.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)       56 2023-03-06 15:00:55.000000 planutils-0.9.0/planutils/packages/tfd/run
+-rwxr-xr-x   0 runner    (1001) docker     (123)       24 2023-03-06 15:00:55.000000 planutils-0.9.0/planutils/packages/tfd/uninstall
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 15:01:05.066416 planutils-0.9.0/planutils/packages/val/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      323 2023-03-06 15:00:55.000000 planutils-0.9.0/planutils/packages/val/install
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-03-06 15:00:55.000000 planutils-0.9.0/planutils/packages/val/manifest.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)      282 2023-03-06 15:00:55.000000 planutils-0.9.0/planutils/packages/val/run
+-rwxr-xr-x   0 runner    (1001) docker     (123)       38 2023-03-06 15:00:55.000000 planutils-0.9.0/planutils/packages/val/uninstall
+-rw-r--r--   0 runner    (1001) docker     (123)     7037 2023-03-06 15:00:55.000000 planutils-0.9.0/planutils/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-03-06 15:00:55.000000 planutils-0.9.0/planutils/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 15:01:05.042415 planutils-0.9.0/planutils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6225 2023-03-06 15:01:05.000000 planutils-0.9.0/planutils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6869 2023-03-06 15:01:05.000000 planutils-0.9.0/planutils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-06 15:01:05.000000 planutils-0.9.0/planutils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-06 15:01:04.000000 planutils-0.9.0/planutils.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-03-06 15:01:05.000000 planutils-0.9.0/planutils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-03-06 15:01:05.000000 planutils-0.9.0/planutils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-06 15:01:05.066416 planutils-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-03-06 15:00:55.000000 planutils-0.9.0/setup.py
```

### Comparing `planutils-0.8.0/LICENSE` & `planutils-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `planutils-0.8.0/PKG-INFO` & `planutils-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: planutils
-Version: 0.8.0
+Version: 0.9.0
 Summary: General library for setting up linux-based environments for developing, running, and evaluating planners.
 Home-page: https://github.com/AI-Planning/planutils
 Author: 
 Author-email: 
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `planutils-0.8.0/README.md` & `planutils-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `planutils-0.8.0/bin/planutils` & `planutils-0.9.0/bin/planutils`

 * *Files 11% similar despite different names*

```diff
@@ -4,21 +4,23 @@
 if [ "$1" = "activate" ]; then
 
     # Environment variables
     export PLANUTILS_PREFIX="~/.planutils"
     export PATH="$PATH:$PLANUTILS_PREFIX/bin"
 
     # Add a blue coloured shell prompt prefix (planutils)
-    export PS1="(\e[1;34mplanutils\e[0m) $PS1"
+    export PS1="(\[\e[1;34m\]planutils\[\e[0m\]) $PS1"
 
     echo
     echo "   Entering planutils environment..."
     echo
 
     # Enter the shell
     $SHELL --init-file <(echo "export PS1=\"$PS1\"")
 
 # Else, call planutils via python
 else
     python3 -c "import planutils; planutils.main()" "$@"
 fi
 
+# Clear history
+history -cw
```

### Comparing `planutils-0.8.0/planutils/__init__.py` & `planutils-0.9.0/planutils/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,14 +26,17 @@
             return
 
     minimal_setup()
     os.mkdir(os.path.join(os.path.expanduser('~'), '.planutils', 'bin'))
 
     print("Installing package scripts...")
     for p in PACKAGES:
+        # TODO: RENAME EXECUTABLE HERE
+        try: s = PACKAGES[p]['shortname']
+        except: s = p
         if PACKAGES[p]['runnable']:
             script  = "#!/bin/bash\n"
             script += "if $(planutils check-installed %s)\n" % p
             script += "then\n"
             script += "  ~/.planutils/packages/%s/run $@\n" % p
             script += "else\n"
             script += "  echo\n"
@@ -53,17 +56,17 @@
             script += "      then\n"
             script += "        ~/.planutils/packages/%s/run $@\n" % p
             script += "      fi\n"
             script += "    fi\n"
             script += "  fi\n"
             script += "  echo\n"
             script += "fi\n"
-            with open(os.path.join(os.path.expanduser('~'), '.planutils', 'bin', p), 'w') as f:
+            with open(os.path.join(os.path.expanduser('~'), '.planutils', 'bin', s), 'w') as f:
                 f.write(script)
-            os.chmod(os.path.join(os.path.expanduser('~'), '.planutils', 'bin', p), 0o0755)
+            os.chmod(os.path.join(os.path.expanduser('~'), '.planutils', 'bin', s), 0o0755)
 
 
     print("\nAll set! Use \"planutils activate\" to activate the environment, or run through \"planutils\" directly.\n")
 
 
 def setup_done():
     return os.path.exists(os.path.join(os.path.expanduser('~'), '.planutils'))
@@ -99,14 +102,17 @@
     parser_server.add_argument('-p', '--port', type=int, help='port to listen on', default=8080)
     parser_server.add_argument('-i', '--host', type=str, help='host to listen on', default='127.0.0.1')
 
     parser_list = subparsers.add_parser('list', help='list the available packages')
     parser_setup = subparsers.add_parser('setup', help='setup planutils for current user')
     parser_upgrade = subparsers.add_parser('upgrade', help='upgrade all of the installed packages')
 
+    parser_show = subparsers.add_parser('show', help='show details about a particular package')
+    parser_show.add_argument('package', help='package name', nargs='+')
+
     args = parser.parse_args()
 
     if 'setup' == args.command:
         setup()
         return
     else:
         minimal_setup()
@@ -143,9 +149,13 @@
         from planutils.package_installation import upgrade
         upgrade()
 
     elif 'server' == args.command:
         from planutils.server import run_server
         run_server(args.port, args.host)
 
+    elif 'show' == args.command:
+        from planutils.package_installation import package_info
+        package_info(args.package)
+
     else:
         parser.print_help()
```

### Comparing `planutils-0.8.0/planutils/manifest_converter.py` & `planutils-0.9.0/planutils/manifest_converter.py`

 * *Files identical despite different names*

### Comparing `planutils-0.8.0/planutils/package_installation.py` & `planutils-0.9.0/planutils/package_installation.py`

 * *Files 23% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import json, os, glob, subprocess, sys, time
 from collections import defaultdict
 from pathlib import Path
 
 from planutils import settings
 
 PACKAGES = {}
+ALIASES = {}
 
 CUR_DIR = os.path.dirname(os.path.abspath(__file__))
 
 
 def check_package(target, manifest):
     assert os.path.exists(manifest), "Error: Manifest must be defined for %s" % target
     with open(manifest, 'r') as f:
@@ -21,31 +22,37 @@
 for conf_file in glob.glob(os.path.join(CUR_DIR, 'packages', '*')):
     base = os.path.basename(conf_file)
     if base not in ['README.md', 'TEMPLATE']:
         assert base not in PACKAGES, "Error: Duplicate package config -- %s" % base
         check_package(base, os.path.join(conf_file, 'manifest.json'))
         with open(os.path.join(conf_file, 'manifest.json'), 'r') as f:
             config = json.load(f)
+        try: ALIASES[config['shortname']] = base
+        except: pass
         PACKAGES[base] = config
         PACKAGES[base]['runnable'] = os.path.exists(os.path.join(conf_file, 'run'))
 
 
 def check_installed(target):
     return target in settings.load()['installed']
 
 
 def uninstall(targets):
 
     for target in targets:
+        try: target = ALIASES[target]
+        except: pass
         if target not in PACKAGES:
             print("Error: Package not found -- %s" % target)
             return
 
     to_check = []
     for target in targets:
+        try: target = ALIASES[target]
+        except: pass
         if check_installed(target):
             to_check.append(target)
         else:
             print("%s isn't installed." % target)
 
     if not to_check:
         return
@@ -91,41 +98,81 @@
                 s['installed'].remove(package)
                 possible_deletions.extend(PACKAGES[package]['dependencies'])
 
     settings.save(s)
 
 
 def package_list():
-    print("\nInstalled:")
     installed = set(settings.load()['installed'])
-    for p in installed:
-        print("  %s: %s" % (p, PACKAGES[p]['name']))
+    installed_names = []
 
-    print("\nAvailable:")
+    terminal_width = 120
+    width_name = 20
+    width_desc = terminal_width - (width_name + 1)
+
+    if installed:
+        for p in installed:
+            try: installed_names.append(PACKAGES[p]['shortname'])
+            except: installed_names.append(p)
+        print("%-*s %s" % (width_name, 'Installed', 'Summary'))
+        print("%-*s %s" % (width_name, ''.ljust(width_name,'-'), ''.ljust(width_desc,'-')))
+        for p in sorted(installed_names):
+            print("%-*s %s" % (width_name, p, PACKAGES[p]['name']))
+        print()
+
+    available_names = []
     for p in PACKAGES:
-        if p not in installed:
-            print("  %s: %s" % (p, PACKAGES[p]['name']))
-    print()
+        try: available_names.append(PACKAGES[p]['shortname'])
+        except: available_names.append(p)
+    if available_names:
+        print("%-*s %s" % (width_name, 'Available', 'Summary'))
+        print("%-*s %s" % (width_name, ''.ljust(width_name,'-'), ''.ljust(width_desc,'-')))
+        for p in sorted(available_names):
+            if p not in installed_names:
+                try: print("%-*s %s" % (width_name, p, PACKAGES[p]['name']))
+                except: print("%-*s %s" % (width_name, p, PACKAGES[ALIASES[p]]['name']))
 
 def upgrade():
     s = settings.load()
     for package in s['installed']:
         print("Upgrading %s..." % package)
         subprocess.call('./uninstall', cwd=os.path.join(CUR_DIR, 'packages', package))
         subprocess.call('./install', cwd=os.path.join(CUR_DIR, 'packages', package))
 
+def package_info(targets):
+    for target in targets:
+        try: target = ALIASES[target]
+        except: pass
+        if target not in PACKAGES:
+            print("Error: Package not found -- %s" % target)
+            return
+        print("Name: %s" % target)
+        try: print("Version: %s" % PACKAGES[target]['version'])
+        except: pass
+        print("Description: %s" % PACKAGES[target]['description'])
+        try: print("Homepage: %s" % PACKAGES[target]['homepage'])
+        except: pass
+        try: print("Author: %s" % PACKAGES[target]['author'])
+        except: pass
+        print("Requires: %s" % ', '.join(PACKAGES[target]['dependencies']))
+        if len(targets) > 1: print("---")
+
 def install(targets, forced=False, always_yes=False):
     for target in targets:
+        try: target = ALIASES[target]
+        except: pass
         if target not in PACKAGES:
             print("Error: Package not found -- %s" % target)
             return False
 
     # Compute all those that will need to be installed
     to_check = []
     for target in targets:
+        try: target = ALIASES[target]
+        except: pass
         if check_installed(target):
             if forced:
                 to_check.append(target)
                 print("%s is present, will be re-installed (forced installation)." % target)
             else:
                 print("%s is present, not installed." % target)
         else:
@@ -136,30 +183,36 @@
     to_install = []
     while to_check:
         check = to_check.pop(0)
         if check not in done:
             done.add(check)
             if not check_installed(check):
                 to_install.append(check)
-                to_check.extend(PACKAGES[check]['dependencies'])
+                try: to_check.extend(PACKAGES[ALIASES[check]]['dependencies'])
+                except: to_check.extend(PACKAGES[check]['dependencies'])
 
     to_install.reverse()
 
     if to_install:
-        to_install_desc = ["%s (%s)" % (pkg, PACKAGES[pkg]['install-size']) for pkg in to_install]
+        to_install_desc = []
+        for pkg in to_install:
+            try: to_install_desc.append("%s (%s)" % (pkg, PACKAGES[ALIASES[pkg]]['install-size']))
+            except: to_install_desc.append("%s (%s)" % (pkg, PACKAGES[pkg]['install-size']))
         print("\nAbout to install the following packages: %s" % ', '.join(to_install_desc))
 
         if always_yes:
             user_response = True
         else:
             user_response = input("  Proceed? [Y/n] ").lower() in ['', 'y', 'yes']
 
         if user_response:
             installed = []
             for package in to_install:
+                try: package = ALIASES[package]
+                except: pass
                 package_path = os.path.join(CUR_DIR, 'packages', package)
                 print("Installing %s..." % package)
                 try:
                     installed.append(package)
                     subprocess.check_call('./install', cwd=package_path, shell=True)
                     size = subprocess.check_output('du -sh .',
                                                    cwd=package_path,
@@ -181,15 +234,16 @@
     else:
         print("Nothing left to install.")
 
     return False
 
 
 def run(target, options):
+    try: target = ALIASES[target]
+    except: pass
     if target not in PACKAGES:
         sys.exit(f"Package {target} not found")
     if not check_installed(target):
         sys.exit(f"Package {target} is not installed")
     if not PACKAGES[target]["runnable"]:
         sys.exit(f"Package {target} is not executable")
     subprocess.run([Path(settings.PLANUTILS_PREFIX) / "packages" / target / "run"] + options)
-
```

### Comparing `planutils-0.8.0/planutils/packages/README.md` & `planutils-0.9.0/planutils/packages/README.md`

 * *Files identical despite different names*

### Comparing `planutils-0.8.0/planutils/packages/cpor/Dockerfile` & `planutils-0.9.0/planutils/packages/cpor/Dockerfile`

 * *Files identical despite different names*

### Comparing `planutils-0.8.0/planutils/packages/ff/run` & `planutils-0.9.0/planutils/packages/ff/run`

 * *Files identical despite different names*

### Comparing `planutils-0.8.0/planutils/packages/forbiditerative-topk/manifest.json` & `planutils-0.9.0/planutils/packages/forbiditerative-topk/manifest.json`

 * *Files 22% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6666666666666666%*

 * *Differences: {"'description'": "'A novel iterative approach to top-k planning, exploiting any cost-optimal "*

 * *                  'planner and reformulating a planning task to forbid exactly the given set of '*

 * *                  "solutions.'",*

 * * "'name'": "'FI -- top-k planner'",*

 * * "'shortname'": "'fi-topk'"}*

```diff
@@ -1,12 +1,12 @@
 {
     "dependencies": [
         "forbiditerative"
     ],
-    "description": "https://github.com/IBM/forbiditerative",
+    "description": "A novel iterative approach to top-k planning, exploiting any cost-optimal planner and reformulating a planning task to forbid exactly the given set of solutions.",
     "endpoint": {
         "services": {
             "solve": {
                 "args": [
                     {
                         "default": 3,
                         "description": "Number of Plans",
@@ -20,9 +20,10 @@
                     "type": "generic"
                 },
                 "template": "planner"
             }
         }
     },
     "install-size": "20K",
-    "name": "Forbid-Iterative top-k planner"
+    "name": "FI -- top-k planner",
+    "shortname": "fi-topk"
 }
```

### Comparing `planutils-0.8.0/planutils/packages/kstar/manifest.json` & `planutils-0.9.0/planutils/packages/kstar/manifest.json`

 * *Files 17% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6666666666666666%*

 * *Differences: {"'description'": "'The first K∗ based solver for PDDL planning tasks; it is best suited for "*

 * *                  "problems with very large solution set-size requirements (>1,000).'",*

 * * "'homepage'": "'https://github.com/ctpelok77/kstar'",*

 * * "'name'": "'K* planner: integrating the K* algorithm into Fast Downward'"}*

```diff
@@ -1,10 +1,10 @@
 {
     "dependencies": [],
-    "description": "https://github.com/ctpelok77/kstar",
+    "description": "The first K\u2217 based solver for PDDL planning tasks; it is best suited for problems with very large solution set-size requirements (>1,000).",
     "endpoint": {
         "services": {
             "solve": {
                 "args": [
                     {
                         "choices": [
                             {
@@ -27,10 +27,11 @@
                     "files": "found_plans/sas_plan.*",
                     "type": "generic"
                 },
                 "template": "planner"
             }
         }
     },
+    "homepage": "https://github.com/ctpelok77/kstar",
     "install-size": "36M",
-    "name": "K* planner for the top-k planning problem"
+    "name": "K* planner: integrating the K* algorithm into Fast Downward"
 }
```

### Comparing `planutils-0.8.0/planutils/packages/lpg-td/run` & `planutils-0.9.0/planutils/packages/lpg-td/run`

 * *Files identical despite different names*

### Comparing `planutils-0.8.0/planutils/packages/metric-ff/run` & `planutils-0.9.0/planutils/packages/metric-ff/run`

 * *Files identical despite different names*

### Comparing `planutils-0.8.0/planutils/packages/optic/install` & `planutils-0.9.0/planutils/packages/optic/install`

 * *Files identical despite different names*

### Comparing `planutils-0.8.0/planutils/packages/symk/manifest.json` & `planutils-0.9.0/planutils/packages/symk/manifest.json`

 * *Files 15% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6666666666666666%*

 * *Differences: {"'description'": "'A novel approach to top-k planning, called sym-k, which is based on symbolic "*

 * *                  'search. The objective of top-k planning is to determine a set of k different '*

 * *                  "plans with lowest cost for a given planning task.'",*

 * * "'homepage'": "'https://github.com/speckdavid/symk'",*

 * * "'name'": "'Sym-k: symbolic top-k planning'"}*

```diff
@@ -1,10 +1,10 @@
 {
     "dependencies": [],
-    "description": "https://github.com/speckdavid/symk",
+    "description": "A novel approach to top-k planning, called sym-k, which is based on symbolic search. The objective of top-k planning is to determine a set of k different plans with lowest cost for a given planning task.",
     "endpoint": {
         "services": {
             "solve": {
                 "args": [
                     {
                         "choices": [
                             {
@@ -27,10 +27,11 @@
                     "files": "found_plans/sas_plan.*",
                     "type": "generic"
                 },
                 "template": "planner"
             }
         }
     },
+    "homepage": "https://github.com/speckdavid/symk",
     "install-size": "40M",
-    "name": "Symk is a state-of-the-art optimal and top-k planner."
+    "name": "Sym-k: symbolic top-k planning"
 }
```

### Comparing `planutils-0.8.0/planutils/server.py` & `planutils-0.9.0/planutils/server.py`

 * *Files identical despite different names*

### Comparing `planutils-0.8.0/planutils/settings.py` & `planutils-0.9.0/planutils/settings.py`

 * *Files identical despite different names*

### Comparing `planutils-0.8.0/planutils.egg-info/PKG-INFO` & `planutils-0.9.0/planutils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: planutils
-Version: 0.8.0
+Version: 0.9.0
 Summary: General library for setting up linux-based environments for developing, running, and evaluating planners.
 Home-page: https://github.com/AI-Planning/planutils
 Author: 
 Author-email: 
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `planutils-0.8.0/planutils.egg-info/SOURCES.txt` & `planutils-0.9.0/planutils.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -151,14 +151,18 @@
 planutils/packages/prp/manifest.json
 planutils/packages/prp/run
 planutils/packages/prp/uninstall
 planutils/packages/pyperplan/install
 planutils/packages/pyperplan/manifest.json
 planutils/packages/pyperplan/run
 planutils/packages/pyperplan/uninstall
+planutils/packages/rpmep/install
+planutils/packages/rpmep/manifest.json
+planutils/packages/rpmep/run
+planutils/packages/rpmep/uninstall
 planutils/packages/scorpion/.gitignore
 planutils/packages/scorpion/install
 planutils/packages/scorpion/manifest.json
 planutils/packages/scorpion/run
 planutils/packages/scorpion/uninstall
 planutils/packages/smtplan/install
 planutils/packages/smtplan/manifest.json
```

### Comparing `planutils-0.8.0/setup.py` & `planutils-0.9.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # Will force a check on the packages setup
 from planutils.package_installation import PACKAGES
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(name='planutils',
-      version='0.8.0',
+      version='0.9.0',
       description='General library for setting up linux-based environments for developing, running, and evaluating planners.',
       long_description=long_description,
       long_description_content_type="text/markdown",
       url='https://github.com/AI-Planning/planutils',
       author='',
       author_email='',
       license='MIT',
```

