# Comparing `tmp/wok_code-2.0.8.tar.gz` & `tmp/wok_code-2.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/wok_code-2.0.8.tar", last modified: Thu May 25 08:46:35 2023, max compression
+gzip compressed data, was "dist/wok_code-2.0.9.tar", last modified: Tue Jun 27 19:00:57 2023, max compression
```

## Comparing `wok_code-2.0.8.tar` & `wok_code-2.0.9.tar`

### file list

```diff
@@ -1,73 +1,78 @@
-drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-05-25 08:46:35.000000 wok_code-2.0.8/
-drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-05-25 08:46:35.000000 wok_code-2.0.8/wok_code.egg-info/
--rw-rw-r--   0 odoo      (1000) odoo      (1000)        9 2023-05-25 08:46:35.000000 wok_code-2.0.8/wok_code.egg-info/top_level.txt
--rw-rw-r--   0 odoo      (1000) odoo      (1000)        1 2023-05-25 08:46:35.000000 wok_code-2.0.8/wok_code.egg-info/dependency_links.txt
--rw-rw-r--   0 odoo      (1000) odoo      (1000)        1 2022-12-09 06:35:40.000000 wok_code-2.0.8/wok_code.egg-info/not-zip-safe
--rw-rw-r--   0 odoo      (1000) odoo      (1000)      948 2023-05-25 08:46:35.000000 wok_code-2.0.8/wok_code.egg-info/entry_points.txt
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     1931 2023-05-25 08:46:35.000000 wok_code-2.0.8/wok_code.egg-info/SOURCES.txt
--rw-rw-r--   0 odoo      (1000) odoo      (1000)       64 2023-05-25 08:46:35.000000 wok_code-2.0.8/wok_code.egg-info/requires.txt
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     1730 2023-05-25 08:46:35.000000 wok_code-2.0.8/wok_code.egg-info/PKG-INFO
--rw-rw-r--   0 odoo      (1000) odoo      (1000)       38 2023-05-25 08:46:35.000000 wok_code-2.0.8/setup.cfg
-drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-05-25 08:46:35.000000 wok_code-2.0.8/wok_code/
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)      164 2022-12-09 05:08:44.000000 wok_code-2.0.8/wok_code/__main__.py
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     3053 2023-05-13 12:31:38.000000 wok_code-2.0.8/wok_code/do_gitignore.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)     7186 2023-05-20 07:43:28.000000 wok_code-2.0.8/wok_code/gen_addons_table.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)      205 2022-12-09 05:08:44.000000 wok_code-2.0.8/wok_code/rm_dir_with_space.py
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     3082 2023-04-23 10:48:07.000000 wok_code-2.0.8/wok_code/pgconf.py
-drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-05-25 08:46:35.000000 wok_code-2.0.8/wok_code/tests/
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)     6517 2023-05-20 15:28:26.000000 wok_code-2.0.8/wok_code/tests/test_gen_readme.py
--rw-r--r--   0 odoo      (1000) odoo      (1000)     2229 2023-05-20 07:43:28.000000 wok_code-2.0.8/wok_code/tests/test_please.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)     2028 2022-12-09 05:08:44.000000 wok_code-2.0.8/wok_code/tests/test_filepo.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)     4939 2023-05-20 07:43:28.000000 wok_code-2.0.8/wok_code/tests/test_license_mgnt.py
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     7806 2023-05-20 07:43:28.000000 wok_code-2.0.8/wok_code/ssh.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)     9119 2023-05-21 13:36:02.000000 wok_code-2.0.8/wok_code/pypi.sh
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)     6744 2023-05-20 07:43:28.000000 wok_code-2.0.8/wok_code/cvt_csv_2_xml.py
-drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-05-25 08:46:35.000000 wok_code-2.0.8/wok_code/scripts/
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)    61313 2023-05-25 08:46:18.000000 wok_code-2.0.8/wok_code/scripts/please.sh
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)    71159 2023-05-20 07:43:28.000000 wok_code-2.0.8/wok_code/scripts/to_pep8.py
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     3910 2023-05-25 06:21:29.000000 wok_code-2.0.8/wok_code/scripts/setup.info
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)     6865 2023-05-20 07:43:28.000000 wok_code-2.0.8/wok_code/scripts/main.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)     4990 2023-05-20 07:43:28.000000 wok_code-2.0.8/wok_code/scripts/makepo_it.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)    21516 2023-05-20 07:43:28.000000 wok_code-2.0.8/wok_code/scripts/cvt_csv_coa.py
--rw-r--r--   0 odoo      (1000) odoo      (1000)      992 2022-12-09 05:08:44.000000 wok_code-2.0.8/wok_code/scripts/run_odoo_debug.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)    17944 2023-05-21 05:45:17.000000 wok_code-2.0.8/wok_code/scripts/dist_pkg.sh
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)     1225 2023-05-20 07:43:28.000000 wok_code-2.0.8/wok_code/scripts/generate_random_codes.py
--rwxr-xr-x   0 odoo      (1000) odoo      (1000)    29393 2023-05-25 06:20:46.000000 wok_code-2.0.8/wok_code/scripts/run_odoo_debug.sh
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)    30263 2023-05-20 07:43:28.000000 wok_code-2.0.8/wok_code/scripts/wget_odoo_repositories.py
-drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-05-25 08:46:35.000000 wok_code-2.0.8/wok_code/scripts/config/
--rw-r--r--   0 odoo      (1000) odoo      (1000)      224 2023-04-12 07:55:02.000000 wok_code-2.0.8/wok_code/scripts/config/to_odoo_py2.yml
--rw-r--r--   0 odoo      (1000) odoo      (1000)      173 2023-04-12 07:50:10.000000 wok_code-2.0.8/wok_code/scripts/config/to_odoo_py3.yml
--rw-r--r--   0 odoo      (1000) odoo      (1000)      893 2023-04-12 07:02:48.000000 wok_code-2.0.8/wok_code/scripts/config/to_new_api.yml
--rw-r--r--   0 odoo      (1000) odoo      (1000)      373 2023-04-12 10:49:14.000000 wok_code-2.0.8/wok_code/scripts/config/globals.yml
--rw-r--r--   0 odoo      (1000) odoo      (1000)      698 2023-04-12 06:43:18.000000 wok_code-2.0.8/wok_code/scripts/config/to_old_api.yml
--rw-r--r--   0 odoo      (1000) odoo      (1000)        0 2023-04-12 07:23:52.000000 wok_code-2.0.8/wok_code/scripts/config/globals_xml.yml
--rw-r--r--   0 odoo      (1000) odoo      (1000)     7066 2023-05-20 07:43:28.000000 wok_code-2.0.8/wok_code/scripts/please_apache.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)      992 2022-12-09 05:08:44.000000 wok_code-2.0.8/wok_code/scripts/dist_pkg.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)    26568 2023-05-20 07:43:28.000000 wok_code-2.0.8/wok_code/scripts/do_migrate.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)    25546 2023-05-20 07:43:28.000000 wok_code-2.0.8/wok_code/scripts/odoo_translation_old.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)    86505 2023-05-22 09:12:11.000000 wok_code-2.0.8/wok_code/scripts/gen_readme.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)    11743 2023-05-20 07:43:28.000000 wok_code-2.0.8/wok_code/scripts/lint_2_compare.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)    42912 2023-05-20 07:43:28.000000 wok_code-2.0.8/wok_code/scripts/deploy_odoo.py
--rw-r--r--   0 odoo      (1000) odoo      (1000)     5550 2023-05-20 07:43:28.000000 wok_code-2.0.8/wok_code/scripts/please_z0bug.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)    46376 2023-05-20 07:43:28.000000 wok_code-2.0.8/wok_code/scripts/odoo_translation.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)    31823 2023-05-20 07:43:28.000000 wok_code-2.0.8/wok_code/scripts/odoo_dependencies.py
--rw-r--r--   0 odoo      (1000) odoo      (1000)    10070 2023-01-27 08:05:01.000000 wok_code-2.0.8/wok_code/scripts/license_mgnt.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)     5357 2023-05-20 07:43:28.000000 wok_code-2.0.8/wok_code/scripts/cvt_csv_2_rst.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)    22434 2023-05-20 07:43:28.000000 wok_code-2.0.8/wok_code/scripts/please.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)     5937 2023-05-20 07:43:28.000000 wok_code-2.0.8/wok_code/scripts/do_odoo_site.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)      606 2023-04-21 11:43:14.000000 wok_code-2.0.8/wok_code/scripts/__init__.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)     2176 2022-12-09 05:08:44.000000 wok_code-2.0.8/wok_code/eval_gtin.py
--rw-r--r--   0 odoo      (1000) odoo      (1000)    14663 2023-05-20 07:43:28.000000 wok_code-2.0.8/wok_code/do_git_checkout_new_branch.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)    32228 2023-05-20 07:43:28.000000 wok_code-2.0.8/wok_code/topep8
--rwxr-xr-x   0 odoo      (1000) odoo      (1000)     2242 2023-05-02 18:41:06.000000 wok_code-2.0.8/wok_code/install_python_3_from_source.sh
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     1150 2022-12-09 05:08:44.000000 wok_code-2.0.8/wok_code/cvt_script.man
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)     1672 2022-12-09 05:08:44.000000 wok_code-2.0.8/wok_code/to_oca.2p8
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     2646 2022-12-09 05:08:44.000000 wok_code-2.0.8/wok_code/do_set_utf8.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)     6897 2023-05-18 06:33:56.000000 wok_code-2.0.8/wok_code/please.man
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)     2667 2022-12-09 05:08:44.000000 wok_code-2.0.8/wok_code/to_zero.2p8
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)     5228 2022-12-09 05:08:44.000000 wok_code-2.0.8/wok_code/to_pep8.2p8
--rw-rw-r--   0 odoo      (1000) odoo      (1000)       81 2023-01-27 10:18:10.000000 wok_code-2.0.8/wok_code/__init__.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)    20904 2023-05-20 07:43:28.000000 wok_code-2.0.8/wok_code/cvt_script
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     3910 2023-05-20 07:43:28.000000 wok_code-2.0.8/setup.py
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     1730 2023-05-25 08:46:35.000000 wok_code-2.0.8/PKG-INFO
--rw-rw-r--   0 odoo      (1000) odoo      (1000)    46083 2023-05-25 06:21:25.000000 wok_code-2.0.8/README.rst
+drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-06-27 19:00:57.000000 wok_code-2.0.9/
+drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-06-27 19:00:57.000000 wok_code-2.0.9/wok_code.egg-info/
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)        9 2023-06-27 19:00:57.000000 wok_code-2.0.9/wok_code.egg-info/top_level.txt
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)        1 2023-06-27 19:00:57.000000 wok_code-2.0.9/wok_code.egg-info/dependency_links.txt
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)        1 2022-12-09 06:35:40.000000 wok_code-2.0.9/wok_code.egg-info/not-zip-safe
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      946 2023-06-27 19:00:57.000000 wok_code-2.0.9/wok_code.egg-info/entry_points.txt
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     2118 2023-06-27 19:00:57.000000 wok_code-2.0.9/wok_code.egg-info/SOURCES.txt
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)       64 2023-06-27 19:00:57.000000 wok_code-2.0.9/wok_code.egg-info/requires.txt
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     1730 2023-06-27 19:00:57.000000 wok_code-2.0.9/wok_code.egg-info/PKG-INFO
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)       38 2023-06-27 19:00:57.000000 wok_code-2.0.9/setup.cfg
+drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-06-27 19:00:57.000000 wok_code-2.0.9/wok_code/
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      164 2023-06-24 06:17:11.000000 wok_code-2.0.9/wok_code/__main__.py
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     3051 2023-06-24 06:17:11.000000 wok_code-2.0.9/wok_code/do_gitignore.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)     7160 2023-06-27 17:52:42.000000 wok_code-2.0.9/wok_code/gen_addons_table.py
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      206 2023-06-24 06:17:11.000000 wok_code-2.0.9/wok_code/rm_dir_with_space.py
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     3106 2023-06-24 06:17:11.000000 wok_code-2.0.9/wok_code/pgconf.py
+drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-06-27 19:00:57.000000 wok_code-2.0.9/wok_code/tests/
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     6526 2023-06-27 17:52:42.000000 wok_code-2.0.9/wok_code/tests/test_gen_readme.py
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)    13796 2023-06-27 17:52:42.000000 wok_code-2.0.9/wok_code/tests/test_please.py
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     2028 2023-06-22 01:46:22.000000 wok_code-2.0.9/wok_code/tests/test_filepo.py
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     4939 2023-06-27 17:52:42.000000 wok_code-2.0.9/wok_code/tests/test_license_mgnt.py
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     7868 2023-06-27 17:52:42.000000 wok_code-2.0.9/wok_code/ssh.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)     9119 2023-06-27 17:52:42.000000 wok_code-2.0.9/wok_code/pypi.sh
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)     6744 2023-06-27 17:52:42.000000 wok_code-2.0.9/wok_code/cvt_csv_2_xml.py
+drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-06-27 19:00:57.000000 wok_code-2.0.9/wok_code/scripts/
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)    62370 2023-06-24 06:25:16.000000 wok_code-2.0.9/wok_code/scripts/please.sh
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)    71159 2023-06-27 17:52:42.000000 wok_code-2.0.9/wok_code/scripts/to_pep8.py
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     3908 2023-06-27 17:52:42.000000 wok_code-2.0.9/wok_code/scripts/setup.info
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)    14663 2023-06-27 17:52:42.000000 wok_code-2.0.9/wok_code/scripts/please_cwd.py
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     3406 2023-06-27 17:52:42.000000 wok_code-2.0.9/wok_code/scripts/please_python.py
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     6873 2023-06-27 17:52:42.000000 wok_code-2.0.9/wok_code/scripts/main.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)     5026 2023-06-27 17:52:42.000000 wok_code-2.0.9/wok_code/scripts/makepo_it.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)    21764 2023-06-27 17:52:42.000000 wok_code-2.0.9/wok_code/scripts/cvt_csv_coa.py
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      992 2023-06-24 06:17:11.000000 wok_code-2.0.9/wok_code/scripts/run_odoo_debug.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)    17943 2023-06-27 17:52:42.000000 wok_code-2.0.9/wok_code/scripts/dist_pkg.sh
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     1218 2023-06-27 17:52:42.000000 wok_code-2.0.9/wok_code/scripts/generate_random_codes.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)    30047 2023-06-27 17:52:42.000000 wok_code-2.0.9/wok_code/scripts/run_odoo_debug.sh
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)    30273 2023-06-27 17:52:42.000000 wok_code-2.0.9/wok_code/scripts/wget_odoo_repositories.py
+drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-06-27 19:00:57.000000 wok_code-2.0.9/wok_code/scripts/config/
+-rw-r--r--   0 odoo      (1000) odoo      (1000)      224 2023-04-12 07:55:02.000000 wok_code-2.0.9/wok_code/scripts/config/to_odoo_py2.yml
+-rw-r--r--   0 odoo      (1000) odoo      (1000)      173 2023-04-12 07:50:10.000000 wok_code-2.0.9/wok_code/scripts/config/to_odoo_py3.yml
+-rw-r--r--   0 odoo      (1000) odoo      (1000)      893 2023-04-12 07:02:48.000000 wok_code-2.0.9/wok_code/scripts/config/to_new_api.yml
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)       79 2023-06-25 02:59:16.000000 wok_code-2.0.9/wok_code/scripts/config/to_pypi_py3.yml
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)       93 2023-06-25 02:59:16.000000 wok_code-2.0.9/wok_code/scripts/config/to_pypi_py2.yml
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)       93 2023-06-25 01:54:53.000000 wok_code-2.0.9/wok_code/scripts/config/to_pypi_future.yml
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      469 2023-06-25 02:59:16.000000 wok_code-2.0.9/wok_code/scripts/config/globals.yml
+-rw-r--r--   0 odoo      (1000) odoo      (1000)      698 2023-04-12 06:43:18.000000 wok_code-2.0.9/wok_code/scripts/config/to_old_api.yml
+-rw-r--r--   0 odoo      (1000) odoo      (1000)        0 2023-04-12 07:23:52.000000 wok_code-2.0.9/wok_code/scripts/config/globals_xml.yml
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     7179 2023-06-27 17:52:42.000000 wok_code-2.0.9/wok_code/scripts/please_apache.py
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      992 2023-06-24 06:17:11.000000 wok_code-2.0.9/wok_code/scripts/dist_pkg.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)    25638 2023-06-27 17:52:42.000000 wok_code-2.0.9/wok_code/scripts/odoo_translation_old.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)    86773 2023-06-27 17:52:42.000000 wok_code-2.0.9/wok_code/scripts/gen_readme.py
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)    11775 2023-06-27 17:52:42.000000 wok_code-2.0.9/wok_code/scripts/lint_2_compare.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)    43527 2023-06-27 17:52:42.000000 wok_code-2.0.9/wok_code/scripts/deploy_odoo.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)    29595 2023-06-27 17:52:42.000000 wok_code-2.0.9/wok_code/scripts/arcangelo.py
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     9130 2023-06-27 17:52:42.000000 wok_code-2.0.9/wok_code/scripts/please_z0bug.py
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)    47199 2023-06-27 17:52:42.000000 wok_code-2.0.9/wok_code/scripts/odoo_translation.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)    32254 2023-06-27 17:52:42.000000 wok_code-2.0.9/wok_code/scripts/odoo_dependencies.py
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)    10070 2023-06-24 06:17:11.000000 wok_code-2.0.9/wok_code/scripts/license_mgnt.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)     5357 2023-06-27 17:52:42.000000 wok_code-2.0.9/wok_code/scripts/cvt_csv_2_rst.py
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)    25681 2023-06-27 17:52:42.000000 wok_code-2.0.9/wok_code/scripts/please.py
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     5934 2023-06-27 17:52:42.000000 wok_code-2.0.9/wok_code/scripts/do_odoo_site.py
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      659 2023-06-24 06:17:11.000000 wok_code-2.0.9/wok_code/scripts/__init__.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)     2176 2023-06-22 01:42:32.000000 wok_code-2.0.9/wok_code/eval_gtin.py
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)    14875 2023-06-27 17:52:42.000000 wok_code-2.0.9/wok_code/do_git_checkout_new_branch.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)    32228 2023-06-27 17:52:42.000000 wok_code-2.0.9/wok_code/topep8
+-rwxr-xr-x   0 odoo      (1000) odoo      (1000)     2242 2023-05-02 18:41:06.000000 wok_code-2.0.9/wok_code/install_python_3_from_source.sh
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     1150 2022-12-09 05:08:44.000000 wok_code-2.0.9/wok_code/cvt_script.man
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)     1672 2022-12-09 05:08:44.000000 wok_code-2.0.9/wok_code/to_oca.2p8
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     2695 2023-06-24 06:17:11.000000 wok_code-2.0.9/wok_code/do_set_utf8.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)     6897 2023-06-24 06:17:11.000000 wok_code-2.0.9/wok_code/please.man
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)     2667 2022-12-09 05:08:44.000000 wok_code-2.0.9/wok_code/to_zero.2p8
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)     5228 2022-12-09 05:08:44.000000 wok_code-2.0.9/wok_code/to_pep8.2p8
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)       82 2023-06-24 06:17:11.000000 wok_code-2.0.9/wok_code/__init__.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)    20904 2023-06-27 17:52:42.000000 wok_code-2.0.9/wok_code/cvt_script
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     3932 2023-06-27 17:52:42.000000 wok_code-2.0.9/setup.py
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     1730 2023-06-27 19:00:57.000000 wok_code-2.0.9/PKG-INFO
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)    43163 2023-06-27 17:52:42.000000 wok_code-2.0.9/README.rst
```

### Comparing `wok_code-2.0.8/wok_code.egg-info/entry_points.txt` & `wok_code-2.0.9/wok_code.egg-info/entry_points.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [console_scripts]
+arcangelo = wok_code.scripts.arcangelo:main
 cvt_csv_2_rst.py = wok_code.scripts.cvt_csv_2_rst:main
 cvt_csv_coa = wok_code.scripts.cvt_csv_coa:main
 deploy_odoo = wok_code.scripts.deploy_odoo:main
 dist_pkg = wok_code.scripts.dist_pkg:main
 do_git_checkout_new_branch = wok_code.do_git_checkout_new_branch:main
 do_gitignore = wok_code.do_gitignore:main
-do_migrate = wok_code.scripts.do_migrate:main
 do_odoo_site.py = wok_code.scripts.do_odoo_site:main
 gen_readme.py = wok_code.scripts.gen_readme:main
 lint_2_compare = wok_code.scripts.lint_2_compare:main
 makepo_it.py = wok_code.scripts.makepo_it:main
 odoo_dependencies.py = wok_code.scripts.odoo_dependencies:main
 odoo_translation.py = wok_code.scripts.odoo_translation:main
 please = wok_code.scripts.please:main
```

### Comparing `wok_code-2.0.8/wok_code.egg-info/SOURCES.txt` & `wok_code-2.0.9/wok_code.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -24,42 +24,47 @@
 wok_code.egg-info/SOURCES.txt
 wok_code.egg-info/dependency_links.txt
 wok_code.egg-info/entry_points.txt
 wok_code.egg-info/not-zip-safe
 wok_code.egg-info/requires.txt
 wok_code.egg-info/top_level.txt
 wok_code/scripts/__init__.py
+wok_code/scripts/arcangelo.py
 wok_code/scripts/cvt_csv_2_rst.py
 wok_code/scripts/cvt_csv_coa.py
 wok_code/scripts/deploy_odoo.py
 wok_code/scripts/dist_pkg.py
 wok_code/scripts/dist_pkg.sh
-wok_code/scripts/do_migrate.py
 wok_code/scripts/do_odoo_site.py
 wok_code/scripts/gen_readme.py
 wok_code/scripts/generate_random_codes.py
 wok_code/scripts/license_mgnt.py
 wok_code/scripts/lint_2_compare.py
 wok_code/scripts/main.py
 wok_code/scripts/makepo_it.py
 wok_code/scripts/odoo_dependencies.py
 wok_code/scripts/odoo_translation.py
 wok_code/scripts/odoo_translation_old.py
 wok_code/scripts/please.py
 wok_code/scripts/please.sh
 wok_code/scripts/please_apache.py
+wok_code/scripts/please_cwd.py
+wok_code/scripts/please_python.py
 wok_code/scripts/please_z0bug.py
 wok_code/scripts/run_odoo_debug.py
 wok_code/scripts/run_odoo_debug.sh
 wok_code/scripts/setup.info
 wok_code/scripts/to_pep8.py
 wok_code/scripts/wget_odoo_repositories.py
 wok_code/scripts/config/globals.yml
 wok_code/scripts/config/globals_xml.yml
 wok_code/scripts/config/to_new_api.yml
 wok_code/scripts/config/to_odoo_py2.yml
 wok_code/scripts/config/to_odoo_py3.yml
 wok_code/scripts/config/to_old_api.yml
+wok_code/scripts/config/to_pypi_future.yml
+wok_code/scripts/config/to_pypi_py2.yml
+wok_code/scripts/config/to_pypi_py3.yml
 wok_code/tests/test_filepo.py
 wok_code/tests/test_gen_readme.py
 wok_code/tests/test_license_mgnt.py
 wok_code/tests/test_please.py
```

### Comparing `wok_code-2.0.8/wok_code.egg-info/PKG-INFO` & `wok_code-2.0.9/wok_code.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: wok-code
-Version: 2.0.8
+Version: 2.0.9
 Summary: Python developers tools
 Home-page: https://zeroincombenze-tools.readthedocs.io
 Author: Antonio Maria Vigliotti
 Author-email: antoniomaria.vigliotti@gmail.com
 License: Affero GPL
 Project-URL: Source, https://github.com/zeroincombenze/tools
 Project-URL: Documentation, https://zeroincombenze-tools.readthedocs.io
```

### Comparing `wok_code-2.0.8/wok_code/do_gitignore.py` & `wok_code-2.0.9/wok_code/do_gitignore.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,94 +1,94 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 import sys
 import os
 
 
 def do_create_gitignore(path, submodules):
-    root = os.environ.get('HOME_DEVEL')
+    root = os.environ.get("HOME_DEVEL")
     if not root or not os.path.isdir(root):
-        if os.path.isdir(os.path.expanduser('~/odoo/devel')):
-            root = os.path.expanduser('~/odoo/devel')
-        elif os.path.isdir(os.path.expanduser('~/devel')):
-            root = os.path.expanduser('~/devel')
+        if os.path.isdir(os.path.expanduser("~/odoo/devel")):
+            root = os.path.expanduser("~/odoo/devel")
+        elif os.path.isdir(os.path.expanduser("~/devel")):
+            root = os.path.expanduser("~/devel")
         else:
-            print('Development directory ~/devel not found!')
+            print("Development directory ~/devel not found!")
             return 1
-    template = os.path.join(root, 'pypi', 'tools', 'templates', 'gitignore')
+    template = os.path.join(root, "pypi", "tools", "templates", "gitignore")
     if not os.path.isfile(template):
-        print('Template %s not found!' % template)
+        print("Template %s not found!" % template)
         return 2
-    target = ''
-    with open(template, 'r') as fd:
+    target = ""
+    with open(template, "r") as fd:
         trig = ""
-        for line in fd.read().split('\n'):
+        for line in fd.read().split("\n"):
             found = line.startswith("!")
             if trig == "odoo":
                 for x in submodules:
                     if x == line:
                         found = True
                         break
             elif trig == "pypi":
                 if (
                     # "/docs/_build/" not in line
                     ".egg-info/" not in line
                     and os.path.join(*[path] + [x for x in line.split("/") if x])
                 ):
                     found = True
             if not trig or found:
-                target += ('%s\n' % line)
-            if line.startswith('# odoo repositories'):
+                target += "%s\n" % line
+            if line.startswith("# odoo repositories"):
                 trig = "odoo"
             if line.startswith("# tools building path"):
                 trig = "pypi"
     if target:
-        ffn = os.path.join(path, '.gitignore')
-        bakfile = '%s~' % ffn
+        ffn = os.path.join(path, ".gitignore")
+        bakfile = "%s~" % ffn
         if os.path.isfile(bakfile):
             os.remove(bakfile)
         if os.path.isfile(ffn):
             os.rename(ffn, bakfile)
-        with open(ffn, 'w') as fd:
+        with open(ffn, "w") as fd:
             fd.write(target)
-            print('Created file %s' % ffn)
+            print("Created file %s" % ffn)
 
 
 def main(argv=None):
     argv = argv or sys.argv[1:]
     path = None
     for param in argv:
-        if param.startswith('-'):
+        if param.startswith("-"):
             pass
         else:
             path = os.path.expanduser(param)
     if not path:
-        print('No path supplied! Use %s PATH' % sys.argv[0])
+        print("No path supplied! Use %s PATH" % sys.argv[0])
         return 1
     if os.path.isdir(path):
-        if not os.path.isdir(os.path.join(path, '.git')):
-            print('Path %s is not a git project!' % sys.argv[0])
+        if not os.path.isdir(os.path.join(path, ".git")):
+            print("Path %s is not a git project!" % sys.argv[0])
             return 1
         submodules = []
         for fn in os.listdir(path):
             if fn in (
-                'addons_kalamitica',
-                'coverage',
-                'generic',
-                'nardo_modules',
-                'venv_odoo',
-                'website-themes',
+                "addons_kalamitica",
+                "coverage",
+                "generic",
+                "nardo_modules",
+                "venv_odoo",
+                "website-themes",
             ):
-                submodules.append('/%s' % fn)
+                submodules.append("/%s" % fn)
                 continue
             ffn = os.path.join(path, fn)
-            if os.path.isdir(os.path.join(ffn, '.git')):
-                submodules.append('/%s' % fn)
+            if os.path.isdir(os.path.join(ffn, ".git")):
+                submodules.append("/%s" % fn)
         return do_create_gitignore(path, submodules)
     else:
-        print('Path %s does not exist!' % sys.argv[0])
+        print("Path %s does not exist!" % sys.argv[0])
         return 2
     return 0
 
 
 if __name__ == "__main__":
     exit(main())
```

### Comparing `wok_code-2.0.8/wok_code/gen_addons_table.py` & `wok_code-2.0.9/wok_code/gen_addons_table.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,16 +12,15 @@
 Markers in README.md must have the form:
 [//]: # (addons)
 Insert list of modules with version and description; if path supplied, insert
 OCA version of module
 [//]: # (end addons)
 """
 
-from __future__ import (absolute_import, division, print_function,
-                        unicode_literals)
+from __future__ import absolute_import, division, print_function, unicode_literals
 
 # from builtins import *                                             # noqa: F403
 import ast
 import os
 import re
 import sys
 
@@ -29,15 +28,15 @@
 from past.builtins import cmp
 
 standard_library.install_aliases()  # noqa: E402
 
 
 MARKERS = r'(\[//\]: # \(addons\))|(\[//\]: # \(end addons\))'
 MANIFESTS = ('__openerp__.py', '__manifest__.py')
-__version__ = "2.0.8"
+__version__ = "2.0.9"
 
 
 class UserError(Exception):
     def __init__(self, msg):
         self.msg = msg
```

### Comparing `wok_code-2.0.8/wok_code/pgconf.py` & `wok_code-2.0.9/wok_code/pgconf.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 #!/usr/bin/env python
+# -*- coding: utf-8 -*-
 import sys
 import os
 import re
 
 
 def fmt_line(user, dbtype):
     if dbtype == "local":
@@ -15,16 +16,16 @@
 
 
 def do_conf_pg(ffn):
     found_tag = False
     done = False
     target = []
     # import pdb; pdb.set_trace()
-    with open(ffn, 'r') as fd:
-        lines = fd.read().split('\n')
+    with open(ffn, "r") as fd:
+        lines = fd.read().split("\n")
         for nro, line in enumerate(lines):
             if re.match(r"^[\s]*local[\s]*all[\s]*postgres", line):
                 found_tag = True
             elif found_tag and re.match(r"^[\s]*local[\s]*all[\s]", line):
                 if not done:
                     for role in ("odoo", "oca"):
                         for version in (
@@ -54,41 +55,41 @@
                     target.append(fmt_line("kalamitica", "ipv4"))
                     target.append(fmt_line("kalamitica", "ipv6"))
                     done = True
                 continue
             target.append(line)
 
     if found_tag:
-        bakfile = '%s.bak' % ffn
+        bakfile = "%s.bak" % ffn
         if os.path.isfile(bakfile):
             os.remove(bakfile)
         if os.path.isfile(ffn):
             os.rename(ffn, bakfile)
-        with open(ffn, 'w') as fd:
+        with open(ffn, "w") as fd:
             fd.write("\n".join(target))
             print(ffn)
 
 
 def main(argv):
     argv = argv or sys.argv[1:]
     path = None
     for param in argv:
-        if param.startswith('-'):
+        if param.startswith("-"):
             pass
         else:
             path = os.path.expanduser(param)
     if not path:
-        print('No path supplied! Use %s PATH' % sys.argv[0])
+        print("No path supplied! Use %s PATH" % sys.argv[0])
         return 1
     if os.path.isdir(path):
-        print('Supplied path is not a file')
+        print("Supplied path is not a file")
         return 1
     elif os.path.isfile(path):
         do_conf_pg(path)
     else:
-        print('Path %s does not exist!' % sys.argv[0])
+        print("Path %s does not exist!" % sys.argv[0])
         return 2
     return 0
 
 
 if __name__ == "__main__":
     exit(main(None))
```

### Comparing `wok_code-2.0.8/wok_code/tests/test_gen_readme.py` & `wok_code-2.0.9/wok_code/tests/test_gen_readme.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import os
 import sys
 
 from python_plus import _c
 from z0lib import z0lib
 from zerobug import z0test, z0testodoo
 
-__version__ = "2.0.8"
+__version__ = "2.0.9"
 
 MODULE_ID = "z0bug_odoo"
 TEST_FAILED = 1
 TEST_SUCCESS = 0
 ODOO_VERSIONS = ("7.0", "10.0", "12.0")
 
 DESCR_FN = r"""Lorem ipsum
@@ -84,145 +84,146 @@
 def version():
     return __version__
 
 
 class RegressionTest:
     def __init__(self, z):
         self.templatedir = os.path.join(
-            os.path.expanduser('~'), 'devel', 'pypi', 'tools', 'templates'
+            os.path.expanduser("~"), "devel", "pypi", "tools", "templates"
         )
         if not os.path.isdir(self.templatedir):
             os.makedirs(self.templatedir)
-        with open(os.path.join(self.templatedir, 'footer.rst'), 'w') as fd:
+        with open(os.path.join(self.templatedir, "footer.rst"), "w") as fd:
             fd.write(
                 _c(
                     """
 ----------------------
 
 .. |en| image:: {{grymb_image_en}}
    :target: {{grymb_url_en}}
 .. |it| image:: {{grymb_image_it}}
    :target: {{grymb_url_it}}
 """
                 )
             )
-        with open(os.path.join(self.templatedir, 'header_authors.txt'), 'w') as fd:
+        with open(os.path.join(self.templatedir, "header_authors.txt"), "w") as fd:
             fd.write(
                 _c(
                     """
 Authors
 -------
 """
                 )
             )
-        with open(os.path.join(self.templatedir, 'header_contributors.txt'), 'w') as fd:
+        with open(os.path.join(self.templatedir, "header_contributors.txt"), "w") as fd:
             fd.write(
                 _c(
                     """
 Contributors
 ------------
 """
                 )
             )
-        with open(os.path.join(self.templatedir, 'header_acknowledges.txt'), 'w') as fd:
+        with open(os.path.join(self.templatedir, "header_acknowledges.txt"), "w") as fd:
             fd.write(
                 _c(
                     """
 Acknoledges to
 --------------
 """
                 )
             )
-        with open(os.path.join(self.templatedir, 'readme_main_module.rst'), 'w') as fd:
+        with open(os.path.join(self.templatedir, "readme_main_module.rst"), "w") as fd:
             fd.write(
                 _c(
                     """
 {{description}}
 """
                 )
             )
         with open(
-            os.path.join(self.templatedir, 'readme_main_repository.rst'), 'w'
+            os.path.join(self.templatedir, "readme_main_repository.rst"), "w"
         ) as fd:
             fd.write(
                 _c(
                     """
 {{description}}
 """
                 )
             )
-        with open(os.path.join(self.templatedir, 'readme_main_ocb.rst'), 'w') as fd:
+        with open(os.path.join(self.templatedir, "readme_main_ocb.rst"), "w") as fd:
             fd.write(
                 _c(
                     """
 {{description}}
 """
                 )
             )
         self.Z = z
 
     def setup(self, z0ctx):
         z0lib.run_traced(
-            "build_cmd %s" % os.path.join(self.Z.rundir, "scripts", "gen_readme.py"))
+            "build_cmd %s" % os.path.join(self.Z.rundir, "scripts", "gen_readme.py")
+        )
 
     def get_doc_path(self, odoo_path, gitorg):
-        if gitorg == 'zero':
-            doc_path = os.path.join(odoo_path, 'egg-info')
+        if gitorg == "zero":
+            doc_path = os.path.join(odoo_path, "egg-info")
         else:
-            doc_path = os.path.join(odoo_path, 'readme')
+            doc_path = os.path.join(odoo_path, "readme")
         if not os.path.isdir(doc_path):
             os.mkdir(doc_path)
         return doc_path
 
     def create_description_file(self, moduledir, odoo_version, gitorg):
         egg_info_path = self.get_doc_path(moduledir, gitorg)
-        if gitorg == 'zero':
-            descr_fn = os.path.join(egg_info_path, 'description.rst')
+        if gitorg == "zero":
+            descr_fn = os.path.join(egg_info_path, "description.rst")
         else:
-            descr_fn = os.path.join(egg_info_path, 'DESCRIPTION.rst')
-        with open(descr_fn, 'w') as fd:
+            descr_fn = os.path.join(egg_info_path, "DESCRIPTION.rst")
+        with open(descr_fn, "w") as fd:
             fd.write(_c(DESCR_FN % odoo_version))
 
     def create_authors_file(self, moduledir, odoo_version, gitorg):
         egg_info_path = self.get_doc_path(moduledir, gitorg)
-        if gitorg == 'zero':
-            descr_fn = os.path.join(egg_info_path, 'authors.rst')
-            with open(descr_fn, 'w') as fd:
+        if gitorg == "zero":
+            descr_fn = os.path.join(egg_info_path, "authors.rst")
+            with open(descr_fn, "w") as fd:
                 fd.write(_c(AUTHORS_FN % odoo_version))
 
     def create_contributors_file(self, moduledir, odoo_version, gitorg):
         egg_info_path = self.get_doc_path(moduledir, gitorg)
-        if gitorg == 'zero':
-            descr_fn = os.path.join(egg_info_path, 'contributors.rst')
+        if gitorg == "zero":
+            descr_fn = os.path.join(egg_info_path, "contributors.rst")
         else:
-            descr_fn = os.path.join(egg_info_path, 'CONTRIBUTORS.rst')
-        with open(descr_fn, 'w') as fd:
+            descr_fn = os.path.join(egg_info_path, "CONTRIBUTORS.rst")
+        with open(descr_fn, "w") as fd:
             fd.write(_c(CONTRIBUTORS_FN % odoo_version))
 
     def test_01(self, z0ctx):
         sts = 0
         # home = os.path.expanduser('~')
-        cmd = os.path.join(self.Z.rundir, 'gen_readme.py')
-        gitorg = 'zero'
+        cmd = os.path.join(self.Z.rundir, "gen_readme.py")
+        gitorg = "zero"
         for odoo_version in ODOO_VERSIONS:
-            if not z0ctx['dry_run']:
+            if not z0ctx["dry_run"]:
                 self.root = z0testodoo.build_odoo_env(z0ctx, odoo_version)
                 odoo_root = os.path.join(self.root, odoo_version)
                 repodir = z0testodoo.create_repo(
-                    z0ctx, odoo_root, 'test_repo', odoo_version
+                    z0ctx, odoo_root, "test_repo", odoo_version
                 )
                 moduledir = z0testodoo.create_module(
-                    z0ctx, repodir, 'test_module', '%s.0.1.0' % odoo_version
+                    z0ctx, repodir, "test_module", "%s.0.1.0" % odoo_version
                 )
                 self.create_description_file(moduledir, odoo_version, gitorg)
                 self.create_authors_file(moduledir, odoo_version, gitorg)
                 self.create_contributors_file(moduledir, odoo_version, gitorg)
                 os.chdir(moduledir)
                 # os.system('%s -B' % cmd)
-                sts, stdout, stderr = z0lib.run_traced('%s -Bw .G %s' % (cmd, gitorg))
+                sts, stdout, stderr = z0lib.run_traced("%s -Bw .G %s" % (cmd, gitorg))
                 if sts:
                     break
 
 
 # Run main if executed as a script
 if __name__ == "__main__":
     exit(
```

### Comparing `wok_code-2.0.8/wok_code/tests/test_filepo.py` & `wok_code-2.0.9/wok_code/tests/test_filepo.py`

 * *Files identical despite different names*

### Comparing `wok_code-2.0.8/wok_code/tests/test_license_mgnt.py` & `wok_code-2.0.9/wok_code/tests/test_license_mgnt.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 """
 import os
 import sys
 
 from wok_code.scripts import license_mgnt
 from zerobug import z0test, z0testodoo
 
-__version__ = "2.0.8"
+__version__ = "2.0.9"
 
-MODULE_ID = 'devel_tool'
+MODULE_ID = "devel_tool"
 TEST_FAILED = 1
 TEST_SUCCESS = 0
 
 
 def version():
     return __version__
 
@@ -40,114 +40,114 @@
 
 
 class RegressionTest:
     def __init__(self, z0bug):
         self.Z = z0bug
 
     def create_file_author_1(self, path):
-        fn = os.path.join(path, 'authors.txt')
-        with open(fn, 'w') as fd:
+        fn = os.path.join(path, "authors.txt")
+        with open(fn, "w") as fd:
             fd.write("""* Powerp <http://www.powerp.it/>""")
 
     def create_file_contributor_1(self, path):
-        fn = os.path.join(path, 'contributors.txt')
-        with open(fn, 'w') as fd:
+        fn = os.path.join(path, "contributors.txt")
+        with open(fn, "w") as fd:
             fd.write("""* <antonio.vigliotti@libero.it>""")
 
     def create_file_manifest_1(self, path):
-        fn = os.path.join(path, '__manifest__.py')
-        with open(fn, 'w') as fd:
+        fn = os.path.join(path, "__manifest__.py")
+        with open(fn, "w") as fd:
             fd.write(MANIFEST_1)
 
     def create_file_author_2(self, path):
-        fn = os.path.join(path, 'authors.txt')
-        with open(fn, 'w') as fd:
+        fn = os.path.join(path, "authors.txt")
+        with open(fn, "w") as fd:
             fd.write(AUTHOR_2)
 
     def create_file_contributor_2(self, path):
-        fn = os.path.join(path, 'contributors.txt')
-        with open(fn, 'w') as fd:
+        fn = os.path.join(path, "contributors.txt")
+        with open(fn, "w") as fd:
             fd.write(CONTRIBUTORS_2)
 
     def create_file_manifest_2(self, path):
-        fn = os.path.join(path, '__manifest__.py')
-        with open(fn, 'w') as fd:
+        fn = os.path.join(path, "__manifest__.py")
+        with open(fn, "w") as fd:
             fd.write(MANIFEST_2)
 
     def prepare_env(self, z0ctx, odoo_ver=None, step=None):
         step = step or 1
         if not odoo_ver:
-            raise (ValueError, 'No odoo version supplied')
+            raise (ValueError, "No odoo version supplied")
         odoo_root = z0testodoo.build_odoo_env(z0ctx, odoo_ver)
         odoo_root = os.path.join(odoo_root, odoo_ver)
         for ldir in (
-            ['egg-info'],
-            ['test_repository'],
-            ['test_repository', 'egg-info'],
-            ['test_repository', 'test_module'],
-            ['test_repository', 'test_module', 'egg-info'],
+            ["egg-info"],
+            ["test_repository"],
+            ["test_repository", "egg-info"],
+            ["test_repository", "test_module"],
+            ["test_repository", "test_module", "egg-info"],
         ):
             path = os.path.join(odoo_root, *ldir)
             if not os.path.isdir(path):
                 os.mkdir(path)
-        path = os.path.join(odoo_root, 'test_repository', 'test_module', 'egg-info')
+        path = os.path.join(odoo_root, "test_repository", "test_module", "egg-info")
         if step == 1:
             self.create_file_author_1(path)
             self.create_file_contributor_1(path)
         elif step == 2:
             self.create_file_author_2(path)
             self.create_file_contributor_2(path)
-        path = os.path.join(odoo_root, 'test_repository', 'test_module')
+        path = os.path.join(odoo_root, "test_repository", "test_module")
         if step == 1:
             self.create_file_manifest_1(path)
         elif step == 1:
             self.create_file_manifest_2(path)
         return path
 
     def test_01(self, z0ctx):
         sts = TEST_SUCCESS
         author = False
         website = False
         devman = False
-        if not z0ctx['dry_run']:
-            module_path = self.prepare_env(z0ctx, odoo_ver='12.0')
+        if not z0ctx["dry_run"]:
+            module_path = self.prepare_env(z0ctx, odoo_ver="12.0")
             license = license_mgnt.License(module_path)
             author = license.summary_authors()
             website = license.get_website()
             devman = license.get_maintainer()
         sts += self.Z.test_result(
-            z0ctx, 'License author', 'powERP enterprise network', author
+            z0ctx, "License author", "powERP enterprise network", author
         )
         sts += self.Z.test_result(
-            z0ctx, 'License website', 'https://www.powerp.it', website
+            z0ctx, "License website", "https://www.powerp.it", website
         )
         sts += self.Z.test_result(
-            z0ctx, 'License maintainer', 'powERP enterprise network', devman
+            z0ctx, "License maintainer", "powERP enterprise network", devman
         )
         return sts
 
     def test_02(self, z0ctx):
         sts = TEST_SUCCESS
         author = False
         website = False
         devman = False
-        if not z0ctx['dry_run']:
-            module_path = self.prepare_env(z0ctx, odoo_ver='12.0', step=2)
+        if not z0ctx["dry_run"]:
+            module_path = self.prepare_env(z0ctx, odoo_ver="12.0", step=2)
             license = license_mgnt.License(module_path)
             author = license.summary_authors()
             website = license.get_website()
             devman = license.get_maintainer()
         sts += self.Z.test_result(
-            z0ctx, 'License author', 'powERP enterprise network, SHS-AV s.r.l.', author
+            z0ctx, "License author", "powERP enterprise network, SHS-AV s.r.l.", author
         )
         sts += self.Z.test_result(
-            z0ctx, 'License website', 'https://www.powerp.it', website
+            z0ctx, "License website", "https://www.powerp.it", website
         )
         sts += self.Z.test_result(
-            z0ctx, 'License maintainer', 'powERP enterprise network', devman
+            z0ctx, "License maintainer", "powERP enterprise network", devman
         )
         return sts
 
 
 #
 # Run main if executed as a script
 if __name__ == "__main__":
```

### Comparing `wok_code-2.0.8/wok_code/ssh.py` & `wok_code-2.0.9/wok_code/ssh.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,128 +1,131 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 import os
 import sys
 
-__version__ = '2.0.8'
+__version__ = "2.0.9"
 
 
 def get_remote_user():
-    local_user = os.environ['USER']
+    local_user = os.environ["USER"]
     user = None
     default_user = None
     for key, item in DATA[host].items():
         if "users" in item and local_user not in item["users"]:
             continue
         if not default_user or key == local_user:
             default_user = key
-        if (
-            (not root_user and key == local_user) or
-            (root_user and key != local_user)
-        ):
+        if (not root_user and key == local_user) or (root_user and key != local_user):
             user = key
             break
     if not user:
         user = default_user
     return user
 
 
 def get_cmd(host, user):
-    param = DATA[host][user].get('param')
-    passwd = DATA[host][user].get('passwd')
+    param = DATA[host][user].get("param")
+    passwd = DATA[host][user].get("passwd")
     if passwd:
-        os.environ['SSHPASS'] = passwd
-        return 'sshpass -e ssh %s %s@%s' % (
-            param, user, host) if param else 'sshpass -e ssh %s@%s' % (user, host)
-    return 'ssh %s %s@%s' % (
-        param, user, host) if param else 'ssh %s@%s' % (user, host)
+        os.environ["SSHPASS"] = passwd
+        return (
+            "sshpass -e ssh %s %s@%s" % (param, user, host)
+            if param
+            else "sshpass -e ssh %s@%s" % (user, host)
+        )
+    return "ssh %s %s@%s" % (param, user, host) if param else "ssh %s@%s" % (user, host)
 
 
 def get_cmd_rsync(host, user, source, dest, recurse):
-    param = DATA[host][user].get('param', "")
+    param = DATA[host][user].get("param", "")
     port = ""
     if param.startswith("-p"):
         port = param.split(" ")[1]
         param = ""
-    passwd = DATA[host][user].get('passwd')
+    passwd = DATA[host][user].get("passwd")
     if recurse and not source.endswith("/"):
         source = "%s/" % source
     if recurse and not dest.endswith("/"):
         dest = "%s/" % dest
     if source.startswith("@"):
         source = "%s@%s:%s" % (user, host, source[1:])
     elif dest.startswith("@"):
         dest = "%s@%s:%s" % (user, host, dest[1:])
     if passwd:
-        os.environ['SSHPASS'] = passwd
-        return 'sshpass -e rsync -avz %s %s %s' % (param, source, dest)
+        os.environ["SSHPASS"] = passwd
+        return "sshpass -e rsync -avz %s %s %s" % (param, source, dest)
     if port:
-        return 'rsync -avz -e \'ssh -p %s\' %s %s %s' % (port, param, source, dest)
-    return 'rsync -avz %s %s %s' % (param, source, dest)
+        return "rsync -avz -e 'ssh -p %s' %s %s %s" % (port, param, source, dest)
+    return "rsync -avz %s %s %s" % (param, source, dest)
 
 
 def get_cmd_scp(host, user, source, dest, recurse):
-    param = DATA[host][user].get('param', "").replace("-p", "-P")
+    param = DATA[host][user].get("param", "").replace("-p", "-P")
     if recurse:
         if param.startswith("-"):
             param += " -r"
         else:
             param = "-r"
-    passwd = DATA[host][user].get('passwd')
+    passwd = DATA[host][user].get("passwd")
     if source.startswith("@"):
         source = "%s@%s:%s" % (user, host, source[1:])
     elif dest.startswith("@"):
         dest = "%s@%s:%s" % (user, host, dest[1:])
     if passwd:
-        os.environ['SSHPASS'] = passwd
-        return 'sshpass -e scp %s %s %s' % (param, source, dest)
-    return 'scp %s %s %s' % (param, source, dest)
+        os.environ["SSHPASS"] = passwd
+        return "sshpass -e scp %s %s %s" % (param, source, dest)
+    return "scp %s %s %s" % (param, source, dest)
 
 
 def show_host(sel_host=None):
     valid_hosts = []
-    prior_host = ''
+    prior_host = ""
     for host in DATA.keys():
         if sel_host and host != sel_host:
             continue
         if host != prior_host:
-            print('')
+            print("")
             prior_host = host
         for user in DATA[host].keys():
-            if os.environ['USER'] not in DATA[host][user].get('users'):
-                print('      %-48.48s# %s' % (
-                    get_cmd(host, user), DATA[host][user]['users']))
+            if os.environ["USER"] not in DATA[host][user].get("users"):
+                print(
+                    "      %-48.48s# %s"
+                    % (get_cmd(host, user), DATA[host][user]["users"])
+                )
             else:
-                print('    $ %-48.48s# %s' % (
-                    get_cmd(host, user), DATA[host][user]['users']))
+                print(
+                    "    $ %-48.48s# %s"
+                    % (get_cmd(host, user), DATA[host][user]["users"])
+                )
                 if host not in valid_hosts:
                     valid_hosts.append(host)
     if not valid_hosts:
-        print('')
-        print('No host for this user!')
+        print("")
+        print("No host for this user!")
     else:
-        print('You should type:')
+        print("You should type:")
         for host in valid_hosts:
             if host in REV_ALIAS:
-                print('$ ssh %-30.30s # %s' % (host, REV_ALIAS[host]))
+                print("$ ssh %-30.30s # %s" % (host, REV_ALIAS[host]))
             else:
-                print('$ ssh %s' % host)
+                print("$ ssh %s" % host)
 
 
 def show_alias():
     for key, alias in ALIAS.items():
         print("%s=%s" % (key, alias))
     return
 
 
 def show_pwd():
     user = get_remote_user()
     if host in DATA.keys():
         if user in DATA[host]:
-            passwd = DATA[host][user].get('passwd')
+            passwd = DATA[host][user].get("passwd")
             if passwd:
                 print("%s (%s)" % (passwd, user))
             else:
                 print("<certificate> (%s)" % user)
 
 
 # import pdb; pdb.set_trace()
@@ -152,19 +155,19 @@
 scp = False
 rsync = False
 sh_alias = False
 do_dir = False
 root_user = False
 ctr = 0
 for param in sys.argv[1:]:
-    if param.startswith('-'):
+    if param.startswith("-"):
         if "h" in param:
-            print('ssh.py [-adlnvwz] host [user]  # ssh')
-            print('ssh.py -[n][r]s[vz] host [user] source destination  # scp')
-            print('ssh.py -[n][r]m[vz] host [user] source destination  # rsync')
+            print("ssh.py [-adlnvwz] host [user]  # ssh")
+            print("ssh.py -[n][r]s[vz] host [user] source destination  # scp")
+            print("ssh.py -[n][r]m[vz] host [user] source destination  # rsync")
             # show_host()
             exit(0)
         if "a" in param:
             sh_alias = True
         if "d" in param:
             do_dir = True
         if "l" in param:
@@ -233,45 +236,45 @@
     show_alias()
     exit(0)
 if list_pwd:
     show_pwd()
     exit(0)
 if host not in DATA:
     if host:
-        print('Host %s not found!' % host)
+        print("Host %s not found!" % host)
     show_host()
     exit(1)
 
 if not user:
     user = get_remote_user()
 if not user:
-    print('No user supplied!')
+    print("No user supplied!")
     show_host(sel_host=host)
     exit(1)
 if user not in DATA[host]:
-    print('User %s not found for host %s!' % (user, host))
+    print("User %s not found for host %s!" % (user, host))
     show_host(sel_host=host)
     exit(1)
-if os.environ['USER'] not in DATA[host][user].get('users'):
-    print('No valid connection parameter for current user!')
+if os.environ["USER"] not in DATA[host][user].get("users"):
+    print("No valid connection parameter for current user!")
     show_host(sel_host=host)
     exit(1)
 
 if do_dir:
     if not source:
-        print('No source path supplied!')
+        print("No source path supplied!")
         exit(1)
     cmd = get_cmd(host, user)
     cmd = "%s dir '%s'" % (cmd, source)
 elif scp or rsync:
     if not source:
-        print('No source path supplied!')
+        print("No source path supplied!")
         exit(1)
     if not dest:
-        print('No destination path supplied!')
+        print("No destination path supplied!")
         exit(1)
     if rsync:
         cmd = get_cmd_rsync(host, user, source, dest, recurse)
     else:
         cmd = get_cmd_scp(host, user, source, dest, recurse)
 else:
     cmd = get_cmd(host, user)
```

### Comparing `wok_code-2.0.8/wok_code/pypi.sh` & `wok_code-2.0.9/wok_code/pypi.sh`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # set -x
-__version__=2.0.8
+__version__=2.0.9
 if [[ -z $HOME_DEVEL || ! -d $HOME_DEVEL ]]; then
   [[ -d $HOME/odoo/devel ]] && HOME_DEVEL="$HOME/odoo/devel" || HOME_DEVEL="$HOME/devel"
 fi
 
 run_traced() {
     local xcmd="$1"
     local sts=0
```

### Comparing `wok_code-2.0.8/wok_code/cvt_csv_2_xml.py` & `wok_code-2.0.9/wok_code/cvt_csv_2_xml.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 
 try:
     from z0lib import z0lib
 except ImportError:
     import z0lib
 
 
-__version__ = "2.0.8"
+__version__ = "2.0.9"
 
 msg_time = time.time()
 
 
 def msg_burst(text):
     global msg_time
     t = time.time() - msg_time
```

### Comparing `wok_code-2.0.8/wok_code/scripts/please.sh` & `wok_code-2.0.9/wok_code/scripts/please.sh`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 #! /bin/bash
-# -*- coding: utf-8 -*-
 #
 # please
 # Developer shell
 #
 # This free software is released under GNU Affero GPL3
 # author: Antonio M. Vigliotti - antoniomaria.vigliotti@gmail.com
 # (C) 2015-2023 by SHS-AV s.r.l. - http://www.shs-av.com - info@shs-av.com
@@ -419,14 +418,15 @@
         run_traced "python setup.py build sdist"
         s=$?; [[ ${s-0} -ne 0 ]] && sts=$s
       fi
       p=$(find dist -name "${n}-${v}.tar.gz")
       [[ -z $p ]] && echo "Internal error: file tar not found!" && return 127
       run_traced "twine upload $p -r $rpt"
       s=$?; [[ ${s-0} -ne 0 ]] && sts=$s
+      [[ $sts -ne 0 ]] && run_traced "twine check $p"
     else
       echo "Command twine not found!"
       echo "Do pip install twine"
       sts=1
     fi
   fi
   return $sts
@@ -1116,39 +1116,59 @@
   # run_traced "odoo_translation.py $opts -b$odoo_fver -m $module -c $confn -p $pofile"
   sts=$?
   return $sts
 }
 
 do_lint() {
     wlog "do_lint '$1' '$2' '$3'"
-    local sts=$STS_FAILED s x
+    local sts=$STS_FAILED s x VDIR
+    [[ $PRJNAME == "Odoo" ]] && VDIR=$(build_odoo_param VDIR ./)
     [[ -z $FLAKE8_CONFIG && -f $HOME_DEVEL/maintainer-quality-tools/travis/cfg/travis_run_flake8.cfg ]] && run_traced "export FLAKE8_CONFIG_DIR=$($READLINK -f $HOME_DEVEL/maintainer-quality-tools/travis/cfg/travis_run_flake8.cfg)"
     if [[ -z $FLAKE8_CONFIG ]]; then
       x=$(find $HOME_DEVEL/venv/lib -type d -name site-packages)
       [[ -n $x ]] && run_traced "export FLAKE8_CONFIG=$($READLINK -f $x/zerobug/_travis/cfg/travis_run_flake8.cfg)"
     fi
     [[ -z $FLAKE8_CONFIG ]] && echo "Non flake8 configuration file found!" && return 1
-    run_traced "flake8 --config=$FLAKE8_CONFIG --extend-ignore=B006 --max-line-length=88 ./"
+    if [[ -n $VDIR ]]; then
+      x=$(vem $VDIR info flake8 2>/dev/null|grep -Eo "[0-9]+\.[0-9]+"|head -n1|tr -d ".")
+      [[ $x -lt 39 ]] && vem $VDIR exec "pip install -U \"flake8>3.9.0,<=6.0.0\""
+      run_traced "vem $VDIR exec \"flake8 --config=$FLAKE8_CONFIG --extend-ignore=B006 --max-line-length=88 ./\""
+    else
+      run_traced "flake8 --config=$FLAKE8_CONFIG --extend-ignore=B006 --max-line-length=88 ./"
+    fi
     sts=$?
     [[ -z $PYLINT_CONFIG_DIR && -f $HOME_DEVEL/maintainer-quality-tools/travis/cfg/travis_run_pylint_beta.cfg ]] && run_traced "export FLAKE8_CONFIG_DIR=$($READLINK -f $HOME_DEVEL/maintainer-quality-tools/travis/cfg)"
     if [[ -z $PYLINT_CONFIG_DIR ]]; then
       x=$(find $HOME_DEVEL/venv/lib -type d -name site-packages)
       [[ -n $x ]] && run_traced "export PYLINT_CONFIG_DIR=$($READLINK -f $x/zerobug/_travis/cfg)"
     fi
     [[ -z $PYLINT_CONFIG_DIR ]] && echo "Non pylint configuration file found!" && return 1
-    run_traced "pylint --rcfile=$PYLINT_CONFIG_DIR/travis_run_pylint_beta.cfg ./"
+    if [[ -n $VDIR ]]; then
+      run_traced "vem $VDIR exec \"pylint --rcfile=$PYLINT_CONFIG_DIR/travis_run_pylint_beta.cfg ./\""
+    else
+      run_traced "pylint --rcfile=$PYLINT_CONFIG_DIR/travis_run_pylint_beta.cfg ./"
+    fi
     s=$?; [[ $s -ne 0 ]] && sts=$s
     return $sts
 }
 
 do_test() {
+    local x y
     wlog "do_test '$1' '$2' '$3'"
     set_opts_4_action
     run_traced "run_odoo_debug $opts -Tm $module"
     sts=$?
+    if [[ -x tests/logs/show-log.sh ]]; then
+      x=$(tests/logs/show-log.sh|grep -E "^TOTAL"|grep -Eo "[0-9]+%?"|tr "\n" " "|awk '{print "* [QUA] Test coverage " $3 " (" $1 ": " $2 "+" ($1 - $2) ")"}')
+      y=$(tests/logs/show-log.sh|grep -E "SUCCESSFULLY completed"|grep -Eo "[0-9]+ tests"|grep -Eo "[0-9]+"|awk '{print "[" $1 " TestPoint]"}')
+      echo ""
+      echo "$x $y"
+      echo ""
+      arcangelo egg-info/history.rst --test-res-msg="$x $y"
+    fi
     return $sts
 }
 
 do_lsearch() {
   # search n log ([date] db token)
   wlog "do_lsearch '$1' '$2' '$3'"
   local CM cmd db f LOGDIRS odoo_fver odoo_ver PM sts=$STS_FAILED tok_dt token
```

### Comparing `wok_code-2.0.8/wok_code/scripts/to_pep8.py` & `wok_code-2.0.9/wok_code/scripts/to_pep8.py`

 * *Files 0% similar despite different names*

```diff
@@ -78,15 +78,15 @@
 except ImportError:
     import z0lib
 try:
     from python_plus.python_plus import _c, _u
 except ImportError:
     from python_plus import _c, _u
 
-__version__ = "2.0.8"
+__version__ = "2.0.9"
 
 LICENSES = ('gpl', 'agpl', 'lgpl', 'opl', 'oee')
 METAS = ('0', '6.1', '7.0', '8.0', '9.0', '10.0', '11.0', '12.0', '13.0', '14.0')
 AUTHORS_TEMPLATE = """
 * LibrERP enterprise network <LibrERP-network>
 * SHS-AV s.r.l. <https://www.zeroincombenze.it>
 * Didotech s.r.l. <https://www.didotech.com>
```

### Comparing `wok_code-2.0.8/wok_code/scripts/setup.info` & `wok_code-2.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,23 @@
+# -*- coding: utf-8 -*-
 import sys
 from setuptools import find_packages, setup
 
 install_requires = [
     'z0lib', 'future', 'Babel', 'lxml', 'openpyxl', 'pyyaml', 'vatnumber'
 ]
 if sys.version_info >= (3, 0):
     install_requires.append('translators')
     install_requires.append('twine')
 else:
     install_requires.append('twine==1.15.0')
 
 setup(
     name='wok_code',
-    version='2.0.8',
+    version='2.0.9',
     description='Python developers tools',
     long_description="""
 Various tools at your fingertips.
 
 The available tools are:
 
 * cvt_csv_2_rst.py: convert csv file into rst file
@@ -77,15 +78,15 @@
             'wok_code-info = wok_code.scripts.main:main',
             'cvt_csv_2_rst.py = wok_code.scripts.cvt_csv_2_rst:main',
             'cvt_csv_coa = wok_code.scripts.cvt_csv_coa:main',
             'deploy_odoo = wok_code.scripts.deploy_odoo:main',
             'dist_pkg = wok_code.scripts.dist_pkg:main',
             'do_gitignore = wok_code.do_gitignore:main',
             'do_git_checkout_new_branch = wok_code.do_git_checkout_new_branch:main',
-            'do_migrate = wok_code.scripts.do_migrate:main',
+            'arcangelo = wok_code.scripts.arcangelo:main',
             'do_odoo_site.py = wok_code.scripts.do_odoo_site:main',
             'gen_readme.py = wok_code.scripts.gen_readme:main',
             'lint_2_compare = wok_code.scripts.lint_2_compare:main',
             'makepo_it.py = wok_code.scripts.makepo_it:main',
             'odoo_dependencies.py = wok_code.scripts.odoo_dependencies:main',
             'odoo_translation.py = wok_code.scripts.odoo_translation:main',
             'please = wok_code.scripts.please:main',
```

### Comparing `wok_code-2.0.8/wok_code/scripts/main.py` & `wok_code-2.0.9/wok_code/scripts/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 import os
 import sys
 import pkg_resources
 import gzip
 import shutil
 
 
-__version__ = "2.0.8"
+__version__ = "2.0.9"
 
 
 def fake_setup(**kwargs):
     globals()["setup_args"] = kwargs
 
 
 def read_setup():
@@ -57,16 +57,17 @@
     local_venv = "/devel/venv/"
     pkgpath = os.path.abspath(os.path.join(os.path.dirname(__file__), ".."))
     bin_path = lib_path = ""
     path = pkgpath
     while not bin_path and path != "/" and path != os.environ["HOME"]:
         path = os.path.dirname(path)
         if os.path.isdir(path) and os.path.basename(path) in ("bin", "lib"):
-            if (os.path.isdir(os.path.join(os.path.dirname(path), "bin")) and
-                    os.path.isdir(os.path.join(os.path.dirname(path), "lib"))):
+            if os.path.isdir(
+                os.path.join(os.path.dirname(path), "bin")
+            ) and os.path.isdir(os.path.join(os.path.dirname(path), "lib")):
                 bin_path = os.path.join(os.path.dirname(path), "bin")
                 lib_path = os.path.join(os.path.dirname(path), "lib")
     if not bin_path and local_venv:
         for path in sys.path:
             if local_venv in path:
                 bin_path = os.path.join(
                     path[: path.find(local_venv)],
```

### Comparing `wok_code-2.0.8/wok_code/scripts/makepo_it.py` & `wok_code-2.0.9/wok_code/scripts/makepo_it.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,17 +4,18 @@
 """
 
 from __future__ import print_function
 
 import os.path
 import sys
 import argparse
+
 # import pdb
 
-__version__ = "2.0.8"
+__version__ = "2.0.9"
 
 PO_DEFAULT = """
 # Translation of Odoo Server.
 # This file contains the translation of the following modules:
 #   * MODULE
 #
 msgid ""
@@ -80,33 +81,35 @@
                 potext = add_po_line(potext, r'"# %s\n"' % opt_args.module)
             elif line.startswith('"# *'):
                 potext = add_po_line(potext, r'"# %s\n"' % opt_args.module)
             elif line.startswith('#. module:'):
                 potext = add_po_line(potext, r'#. module: %s' % opt_args.module)
             elif line.startswith('"Project-Id-Version:'):
                 potext = add_po_line(
-                    potext, r'"Project-Id-Version: Odoo (%s)\n"' % opt_args.branch)
+                    potext, r'"Project-Id-Version: Odoo (%s)\n"' % opt_args.branch
+                )
             elif line.startswith('"Last-Translator:'):
                 potext = add_po_line(
                     potext,
-                    r'"Last-Translator: %s <%s>\n"' % (LAST_TNL_NAME, LAST_TNL_MAIL)
+                    r'"Last-Translator: %s <%s>\n"' % (LAST_TNL_NAME, LAST_TNL_MAIL),
                 )
             elif line.startswith('"Language-Team:'):
                 potext = add_po_line(
                     potext,
-                    r'"Language-Team: %s (%s)\n"' % (LAST_TEAM_NAME, LAST_TEAM_URL)
+                    r'"Language-Team: %s (%s)\n"' % (LAST_TEAM_NAME, LAST_TEAM_URL),
                 )
                 potext = add_po_line(potext, r'"Language: it_IT\n"')
             elif line.startswith('"Language:'):
                 pass
             elif line.startswith('"language'):
                 pass
             elif line.startswith('"Plural-Forms:'):
                 potext = add_po_line(
-                    potext,  r'"Plural-Forms: nplurals=2; plural=(n != 1);\n"')
+                    potext, r'"Plural-Forms: nplurals=2; plural=(n != 1);\n"'
+                )
             elif opt_args.clear_base_tnl:
                 if line.startswith('#: model:ir.module.module,description'):
                     saved_lines.append(line)
                     discard_saved_lines = True
                 elif line.startswith('#: model:ir.module.module,shortdesc'):
                     saved_lines.append(line)
                     discard_saved_lines = True
```

### Comparing `wok_code-2.0.8/wok_code/scripts/cvt_csv_coa.py` & `wok_code-2.0.9/wok_code/scripts/cvt_csv_coa.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 import argparse
 import time
 
 from os0 import os0
 from python_plus import unicodes
 from clodoo import transodoo
 
-__version__ = "2.0.8"
+__version__ = "2.0.9"
 
 msg_time = time.time()
 VALID_ACTIONS = ("export-comparable", "export-full", "export-z0bug", "export-group")
 VERSIONS = ["6.1", "7.0", "8.0", "9.0", "10.0", "11.0", "12.0", "13.0", "14.0"]
 
 
 class CvtCsvFile(object):
@@ -307,31 +307,37 @@
                         ("account.tax", "export-group"): self.set_hdr_out_group_tax,
                     }[self.opt_args.model, self.opt_args.action]()
 
                     next_id = len(row)
                     for name in self.hdr.keys():
                         ttype = ""
                         if name.endswith(":id"):
-                            name = transodoo.translate_from_to(
-                                self.ctx,
-                                self.opt_args.model,
-                                name.replace(":id", ""),
-                                self.opt_args.to_version,
-                                self.opt_args.from_version,
-                                ttype="field",
-                            ) + ":id"
+                            name = (
+                                transodoo.translate_from_to(
+                                    self.ctx,
+                                    self.opt_args.model,
+                                    name.replace(":id", ""),
+                                    self.opt_args.to_version,
+                                    self.opt_args.from_version,
+                                    ttype="field",
+                                )
+                                + ":id"
+                            )
                         elif name.endswith("/id"):
-                            name = transodoo.translate_from_to(
-                                self.ctx,
-                                self.opt_args.model,
-                                name.replace(":id", ""),
-                                self.opt_args.to_version,
-                                self.opt_args.from_version,
-                                ttype="field",
-                            ) + ":id"
+                            name = (
+                                transodoo.translate_from_to(
+                                    self.ctx,
+                                    self.opt_args.model,
+                                    name.replace(":id", ""),
+                                    self.opt_args.to_version,
+                                    self.opt_args.from_version,
+                                    ttype="field",
+                                )
+                                + ":id"
+                            )
                         else:
                             name = transodoo.translate_from_to(
                                 self.ctx,
                                 self.opt_args.model,
                                 name,
                                 self.opt_args.to_version,
                                 self.opt_args.from_version,
```

### Comparing `wok_code-2.0.8/wok_code/scripts/run_odoo_debug.py` & `wok_code-2.0.9/wok_code/scripts/run_odoo_debug.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,33 +3,33 @@
 import os
 import sys
 
 
 def main(cli_args=None):
     if not cli_args:
         cli_args = sys.argv[1:]
-    cmd = '%s.sh' % os.path.splitext(os.path.abspath(__file__))[0]
+    cmd = "%s.sh" % os.path.splitext(os.path.abspath(__file__))[0]
     if not os.path.isfile(cmd):
         cmd = os.path.split(cmd)
         cmd = os.path.join(os.path.dirname(cmd[0]), cmd[1])
     if not os.path.isfile(cmd):
-        print('Internal package error: file %s not found!' % cmd)
+        print("Internal package error: file %s not found!" % cmd)
     for arg in cli_args:
-        if '<' in arg or '>' in arg:
+        if "<" in arg or ">" in arg:
             arg = "'%s'" % arg.replace("'", r"\'")
-        elif ' ' in arg:
+        elif " " in arg:
             if '"' in arg:
-                arg = '"%s"' % arg.replace('"', r'\"')
+                arg = '"%s"' % arg.replace('"', r"\"")
             else:
                 arg = '"%s"' % arg
         elif '"' in arg:
-            arg = '"%s"' % arg.replace('"', r'\"')
+            arg = '"%s"' % arg.replace('"', r"\"")
         elif "'" in arg:
             arg = '"%s"' % arg
         else:
-            arg = '%s' % arg
-        cmd = '%s %s' % (cmd, arg)
+            arg = "%s" % arg
+        cmd = "%s %s" % (cmd, arg)
     return os.system(cmd)
 
 
 if __name__ == "__main__":
     exit(main())
```

### Comparing `wok_code-2.0.8/wok_code/scripts/dist_pkg.sh` & `wok_code-2.0.9/wok_code/scripts/dist_pkg.sh`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 link_cfg $DIST_CONF $TCONF
 [[ $TRAVIS_DEBUG_MODE -ge 8 ]] && echo "DIST_CONF=$DIST_CONF" && echo "TCONF=$TCONF"
 get_pypi_param ALL
 RED="\e[1;31m"
 GREEN="\e[1;32m"
 CLR="\e[0m"
 
-__version__=2.0.8
+__version__=2.0.9
 
 # main
 OPTOPTS=(h        C         c        D        F         f         n            O         o        P         p         q           R         S        u       V           v           W          w         -)
 OPTDEST=(opt_help opt_cpush opt_conf opt_push opt_fetch opt_force opt_dry_run  opt_cpush opt_ids  opt_cpush opt_dpath opt_verbose opt_cpush opt_sts  opt_upd opt_version opt_verbose opt_whatis opt_cpush opt_sync)
 OPTACTI=("+"      "*>"      "="      "*>"     "1>"      1         1            "*>"      "=>"     "*>"      "="       0           "*>"      "=>"     1       "*"         "+"         "=>"       "*>"      "1>")
 OPTDEFL=(1        ""        ""       ""       0         0         0            ""        ""       ""        ""        0           ""        ""       0       ""          -1          ""         ""        0)
 OPTMETA=("help"   "commit"  "file"   ""       "fetch"   ""        "do nothing" ""        "prj_id" "push"    "path"    "quiet"     "replace" "status" "upd"   "version"   "verbose"   "param"    "wep"     "sync")
@@ -365,15 +365,15 @@
   fi
   exit $STS_SUCCESS
 fi
 
 [[ ! -d $LGITPATH ]] && echo "Destination path $LGITPATH not found!" && exit $STS_FAILED
 robocopy_init "$PRJNAME" "$PKGNAME"
 if [[ $opt_fetch -eq 0 ]]; then
-  [[ $PKGNAME != "tools" ]] &&  run_traced "cp $PKGPATH/setup.py $PRJPATH/scripts/setup.info"
+  [[ $PKGNAME != "tools" ]] && run_traced "cp $PKGPATH/setup.py $PRJPATH/scripts/setup.info"
   [[ -f $PRJPATH/setup.py && -f $PRJPATH/scripts/setup.info ]] &&  run_traced "rm -f $PRJPATH/setup.py"
   [[ -x $PRJPATH/replace.sh ]] && run_traced "$PRJPATH/replace.sh"
   [[ ! -x $PRJPATH/replace.sh ]] && robocopy "$PRJPATH" "$LGITPATH"
   if [[ $PKGNAME != "tools" ]]; then
     [[ -f $PKGPATH/setup.py ]] &&  run_traced "cp $PKGPATH/setup.py $LGITPATH/setup.py"
     [[ -f $PKGPATH/README.rst ]] &&  run_traced "cp $PKGPATH/README.rst $LGITPATH/README.rst"
     [[ -f "$PRJPATH/scripts/setup.info" ]] &&  run_traced "cp $PRJPATH/scripts/setup.info $LGITPATH/scripts/setup.info"
```

### Comparing `wok_code-2.0.8/wok_code/scripts/generate_random_codes.py` & `wok_code-2.0.9/wok_code/scripts/generate_random_codes.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 import sys
+
 # import os
 import argparse
 from random import random, randint
 import vatnumber
 
 
-__version__ = "2.0.8"
+__version__ = "2.0.9"
 
 
 def gen_vatnumber(opt_args):
     found = False
     while not found:
         seed = "%7.7s%3.03i" % (random() * 10000000, randint(1, 99))
         for i in range(10):
@@ -22,21 +23,20 @@
     print(vat)
     return 0
 
 
 def main(cli_args=None):
     cli_args = cli_args or sys.argv[1:]
     parser = argparse.ArgumentParser(
-        description="Generate random VAT number",
-        epilog="© 2021-2023 by SHS-AV s.r.l."
+        description="Generate random VAT number", epilog="© 2021-2023 by SHS-AV s.r.l."
     )
-    parser.add_argument('-i', '--iso', default="IT")
-    parser.add_argument('-v', '--verbose', action='count', default=0)
-    parser.add_argument('-V', '--version', action="version", version=__version__)
-    parser.add_argument('-w', "--what", help="Kind of code: mey be vat")
+    parser.add_argument("-i", "--iso", default="IT")
+    parser.add_argument("-v", "--verbose", action="count", default=0)
+    parser.add_argument("-V", "--version", action="version", version=__version__)
+    parser.add_argument("-w", "--what", help="Kind of code: mey be vat")
     opt_args = parser.parse_args(cli_args)
     sts = 0
     if opt_args.what == "vat":
         return gen_vatnumber(opt_args)
     else:
         print("Invalid kind of code!")
     return sts
```

### Comparing `wok_code-2.0.8/wok_code/scripts/run_odoo_debug.sh` & `wok_code-2.0.9/wok_code/scripts/run_odoo_debug.sh`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 link_cfg $DIST_CONF $TCONF
 [[ $TRAVIS_DEBUG_MODE -ge 8 ]] && echo "DIST_CONF=$DIST_CONF" && echo "TCONF=$TCONF"
 get_pypi_param ALL
 RED="\e[1;31m"
 GREEN="\e[1;32m"
 CLR="\e[0m"
 
-__version__=2.0.8
+__version__=2.0.9
 
 run_traced_debug() {
     if [[ $opt_verbose -gt 1 ]]; then
         run_traced "$1"
     elif [[ $opt_dry_run -eq 0 ]]; then
         eval $1
     fi
@@ -58,18 +58,18 @@
         OPTU="-uall"
     else
         mods=${opt_modules//,/ }
         for m in $mods; do
             r=$(psql -U$DB_USER $opt_db -tc "select state from ir_module_module where name='$m'" 2>/dev/null)
             if [[ $r =~ uninstallable ]]; then
                 XXX="$XXX $m"
-            elif [[ $r =~ uninstalled ]]; then
+            elif [[ $r =~ (uninstalled|to install) ]]; then
                 OPTI="$OPTI$xi$m"
                 xi=,
-            elif [[ $r =~ installed ]]; then
+            elif [[ $r =~ (installed|to upgrade) ]]; then
                 OPTU="$OPTU$xu$m"
                 xu=,
             elif [[ $opt_force -ne 0 ]]; then
                 OPTI="$OPTI$xi$m"
                 OPTU="$OPTU$xu$m"
                 xu=,
             else
@@ -125,15 +125,14 @@
 #      LOGFILE="$LOGDIR/${UMLI}.log"
 #    fi
     LOGDIR="$PKGPATH/tests/logs"
     # [[ -d $LOGDIR ]] || mkdir $LOGDIR
     LOGFILE="$LOGDIR/${PKGNAME}_$(date +%Y%m%d).txt"
     [[ -f $LOGFILE ]] && rm -f $LOGFILE
     # OLD_LOGFILE=${LOGFILE/.log/_old.log}
-    # set +x  #debug
 }
 
 check_path_n_branch() {
     # check_path_n_branch(path branch)
     local x
     [[ -n $1 ]] && odoo_fver=$(build_odoo_param FULLVER "$1") || odoo_fver=""
     [[ -n $2 ]] && x=$(build_odoo_param FULLVER "$2") || x=""
@@ -531,31 +530,36 @@
             TEMPLATE="${opt_db/test/template}"
             [[ $opt_keep -ne 0 ]] && TEMPLATE="${MQT_TEMPLATE_DB}_${odoo_ver}"
             [[ opt_dbg -gt 1 && $opt_keep -eq 0 ]] && TEMPLATE="template_${UDI}"
             cmd="${cmd/$opt_db/$TEMPLATE}"
             fnparam="$LOGDIR/${UDI}.sh"
             if [[ $opt_force -ne 0 || ! -f $fnparam ]] || ! echo $c|diff -qw $fnparam - || ! psql -U$DB_USER -Atl|cut -d"|" -f1|grep -q "$TEMPLATE"; then
               # Create DB for test
-              run_traced "pg_db_active -L -wa '$TEMPLATE' && dropdb $opts --if-exists '$TEMPLATE'"
-              if [[ $opt_dry_run -eq 0 ]]; then
-                psql -U$DB_USER -Atl|cut -d"|" -f1|grep -q "$TEMPLATE" && echo "Database $TEMPLATE removal failed!" && exit 1
+              run_traced "pg_db_active -L -wa \"$TEMPLATE\" && dropdb $opts --if-exists \"$TEMPLATE\""
+              c=$(pg_db_active -c "$TEMPLATE")
+              [[ $c -ne 0 ]] && echo "FATAL! There are $c other sessions using the database \"$TEMPLATE\"" && exit 1
+              # if [[ $opt_dry_run -eq 0 ]]; then
+                psql -U$DB_USER -Atl|cut -d"|" -f1|grep -q "$TEMPLATE" && echo "Database \"$TEMPLATE\" removal failed!" && exit 1
+                [[ $odoo_ver -lt 10 ]] && run_traced "psql -U$DB_USER template1 -c 'create database \"$TEMPLATE\" owner $DB_USER'"
                 run_traced "$cmd"
-                run_traced "pg_db_active -L '$TEMPLATE'"
-              fi
+                run_traced "pg_db_active -L \"$TEMPLATE\""
+              # fi
             fi
             if psql -U$DB_USER -Atl|cut -d"|" -f1|grep -q "$TEMPLATE"; then
               [[ $opt_dry_run -eq 0 ]] && echo $c > $fnparam
-              run_traced "pg_db_active -L -wa '$opt_db' && dropdb $opts --if-exists '$opt_db'"
-              if [[ $opt_dry_run -eq 0 ]]; then
-                psql -U$DB_USER -Atl|cut -d"|" -f1|grep -q "$opt_db" && echo "Database $opt_db removal failed!" && exit 1
-                run_traced "pg_db_active -L -wa '$TEMPLATE'"
+              run_traced "pg_db_active -L -wa \"$opt_db\" && dropdb $opts --if-exists \"$opt_db\""
+              c=$(pg_db_active -c \"$opt_db\")
+              [[ $c -ne 0 ]] && echo "FATAL! There are $c other sessions using the database \"$opt_db\"" && exit 1
+              # if [[ $opt_dry_run -eq 0 ]]; then
+                psql -U$DB_USER -Atl|cut -d"|" -f1|grep -q "$opt_db" && echo "Database \"$opt_db\" removal failed!" && exit 1
+                run_traced "pg_db_active -L -wa \"$TEMPLATE\""
                 run_traced "psql -U$DB_USER template1 -c 'create database \"$opt_db\" owner $DB_USER template \"$TEMPLATE\"'"
-              fi
+              # fi
             else
-              echo "Template $TEMPLATE not found!"
+              echo "Template \"$TEMPLATE\" not found!"
               cmd="${cmd/$TEMPLATE$opt_db/}"
               run_traced "$cmd"
             fi
        else
             run_traced "cd $ODOO_RUNDIR; $script $OPTDB $OPT_CONF --log-level=error"
        fi
     fi
@@ -620,12 +624,14 @@
     elif [[ $opt_imp -ne 0 ]]; then
         echo "# Translation imported from '$src' file"
     fi
 
     if [[ $drop_db -gt 0 ]]; then
         if [[ -z "$opt_modules" || $opt_stop -eq 0 ]]; then
             [[ -n "$DB_PORT" ]] && opts="-U$DB_USER -p$DB_PORT" || opts="-U$DB_USER"
-            run_traced "pg_db_active -L -wa '$opt_db'; dropdb $opts --if-exists '$opt_db'"
-            [[ opt_dbg -ne 1 ]] && run_traced "pg_db_active -L -wa '$TEMPLATE'; dropdb $opts --if-exists '$TEMPLATE'"
+            run_traced "pg_db_active -L -wa \"$opt_db\"; dropdb $opts --if-exists '$opt_db'"
+            c=$(pg_db_active -c "$opt_db")
+            [[ $c -ne 0 ]] && echo "FATAL! There are $c other sessions using the database \"$opt_db\"" && exit 1
+            # [[ opt_dbg -ne 1 ]] && run_traced "pg_db_active -L -wa '$TEMPLATE'; dropdb $opts --if-exists '$TEMPLATE'"
         fi
     fi
 fi
```

### Comparing `wok_code-2.0.8/wok_code/scripts/wget_odoo_repositories.py` & `wok_code-2.0.9/wok_code/scripts/wget_odoo_repositories.py`

 * *Files 22% similar despite different names*

```diff
@@ -21,694 +21,696 @@
 #     from z0lib.z0lib import z0lib
 # except ImportError:
 #     try:
 #         from z0lib import z0lib
 #     except ImportError:
 #         import z0lib
 
-__version__ = '2.0.8'
+__version__ = "2.0.9"
 
-ROOT_URL = 'https://api.github.com/repos/zeroincombenze/'
-USER_URL = 'https://api.github.com/users/'
-REPNAME_ACC_CLO = 'OCB'
+ROOT_URL = "https://api.github.com/repos/zeroincombenze/"
+USER_URL = "https://api.github.com/users/"
+REPNAME_ACC_CLO = "OCB"
 DEVEL_REPS = [
-    'Odoo-samples',
-    'VME',
-    'OpenUpgrade',
-    'dotnet',
-    'grymb',
-    'interface-github',
-    'odoorpc',
-    'openupgradelib',
-    'project-agile',
-    'pylint-odoo',
-    'python-plus',
-    'rest-framework',
-    'runbot-addons',
-    'z0bug_odoo',
-    'zerobug',
-    'zeroincombenze',
+    "Odoo-samples",
+    "VME",
+    "OpenUpgrade",
+    "dotnet",
+    "grymb",
+    "interface-github",
+    "odoorpc",
+    "openupgradelib",
+    "project-agile",
+    "pylint-odoo",
+    "python-plus",
+    "rest-framework",
+    "runbot-addons",
+    "z0bug_odoo",
+    "zerobug",
+    "zeroincombenze",
 ]
-REPNAME_OCB = 'OCB'
+REPNAME_OCB = "OCB"
 TEST_REP_OCB = {
-    'issues_url': '%s%s/issues{/number}' % (ROOT_URL, REPNAME_OCB),
-    'deployments_url': '%s%s/deployments' % (ROOT_URL, REPNAME_OCB),
-    'stargazers_count': 0,
-    'forks_url': '%s%s/forks' % (ROOT_URL, REPNAME_OCB),
-    'mirror_url': None,
-    'subscription_url': '%s%s/subscription' % (ROOT_URL, REPNAME_OCB),
-    'notifications_url': '%s%s/notifications{?since,all,participating}'
+    "issues_url": "%s%s/issues{/number}" % (ROOT_URL, REPNAME_OCB),
+    "deployments_url": "%s%s/deployments" % (ROOT_URL, REPNAME_OCB),
+    "stargazers_count": 0,
+    "forks_url": "%s%s/forks" % (ROOT_URL, REPNAME_OCB),
+    "mirror_url": None,
+    "subscription_url": "%s%s/subscription" % (ROOT_URL, REPNAME_OCB),
+    "notifications_url": "%s%s/notifications{?since,all,participating}"
     % (ROOT_URL, REPNAME_OCB),
-    'collaborators_url': '%s%s/collaborators{collaborator}' % (ROOT_URL, REPNAME_OCB),
-    'updated_at': '2013-07-15T20:26:20Z',
-    'private': False,
-    'pulls_url': '%s%s/pulls{/number}' % (ROOT_URL, REPNAME_OCB),
-    'disabled': False,
-    'issue_comment_url': '%s%s/issues/comments{number}' % (ROOT_URL, REPNAME_OCB),
-    'labels_url': '%s%s/labels{/name}' % (ROOT_URL, REPNAME_OCB),
-    'has_wiki': True,
-    'full_name': 'zeroincombenze/%s' % REPNAME_OCB,
-    'owner': {
-        'following_url': '%s%s/following{other_user}' % (ROOT_URL, REPNAME_OCB),
-        'events_url': '%s%s/events{/privacy}' % (ROOT_URL, REPNAME_OCB),
-        'avatar_url': 'https://avatars2.githubusercontent.com/u/234?v=4',
-        'url': '%s%s' % (USER_URL, REPNAME_OCB),
-        'gists_url': '%s%s/gists{/gist_id}' % (USER_URL, REPNAME_OCB),
-        'html_url': 'https://github.com/%s' % REPNAME_OCB,
-        'subscriptions_url': '%s%s/subscriptions' % (USER_URL, REPNAME_OCB),
-        'node_id': 'MDQ6VXNlcjY5NzI1NTU=',
-        'test_repos_url': '%s%s/test_repos' % (USER_URL, REPNAME_OCB),
-        'received_events_url': '%s%s/received_events' % (USER_URL, REPNAME_OCB),
-        'gravatar_id': '',
-        'starred_url': '%s%s/starred{/owner}{/TEST_REPo}' % (USER_URL, REPNAME_OCB),
-        'site_admin': False,
-        'login': 'zeroincombenze',
-        'type': 'User',
-        'id': 6972533,
-        'followers_url': '%s%s/followers' % (USER_URL, REPNAME_OCB),
-        'organizations_url': '%s%s/orgs' % (USER_URL, REPNAME_OCB),
+    "collaborators_url": "%s%s/collaborators{collaborator}" % (ROOT_URL, REPNAME_OCB),
+    "updated_at": "2013-07-15T20:26:20Z",
+    "private": False,
+    "pulls_url": "%s%s/pulls{/number}" % (ROOT_URL, REPNAME_OCB),
+    "disabled": False,
+    "issue_comment_url": "%s%s/issues/comments{number}" % (ROOT_URL, REPNAME_OCB),
+    "labels_url": "%s%s/labels{/name}" % (ROOT_URL, REPNAME_OCB),
+    "has_wiki": True,
+    "full_name": "zeroincombenze/%s" % REPNAME_OCB,
+    "owner": {
+        "following_url": "%s%s/following{other_user}" % (ROOT_URL, REPNAME_OCB),
+        "events_url": "%s%s/events{/privacy}" % (ROOT_URL, REPNAME_OCB),
+        "avatar_url": "https://avatars2.githubusercontent.com/u/234?v=4",
+        "url": "%s%s" % (USER_URL, REPNAME_OCB),
+        "gists_url": "%s%s/gists{/gist_id}" % (USER_URL, REPNAME_OCB),
+        "html_url": "https://github.com/%s" % REPNAME_OCB,
+        "subscriptions_url": "%s%s/subscriptions" % (USER_URL, REPNAME_OCB),
+        "node_id": "MDQ6VXNlcjY5NzI1NTU=",
+        "test_repos_url": "%s%s/test_repos" % (USER_URL, REPNAME_OCB),
+        "received_events_url": "%s%s/received_events" % (USER_URL, REPNAME_OCB),
+        "gravatar_id": "",
+        "starred_url": "%s%s/starred{/owner}{/TEST_REPo}" % (USER_URL, REPNAME_OCB),
+        "site_admin": False,
+        "login": "zeroincombenze",
+        "type": "User",
+        "id": 6972533,
+        "followers_url": "%s%s/followers" % (USER_URL, REPNAME_OCB),
+        "organizations_url": "%s%s/orgs" % (USER_URL, REPNAME_OCB),
     },
-    'statuses_url': '%s%s/statuses/{sha}' % (ROOT_URL, REPNAME_OCB),
-    'id': 58389479,
-    'keys_url': '%s%s/keys{/key_id}' % (ROOT_URL, REPNAME_OCB),
-    'description': 'Odoo Accountant closing tools',
-    'tags_url': '%s%s/tags' % (ROOT_URL, REPNAME_OCB),
-    'archived': False,
-    'downloads_url': '%s%s/downloads' % (ROOT_URL, REPNAME_OCB),
-    'assignees_url': '%s%s/assignees{/user}' % (ROOT_URL, REPNAME_OCB),
-    'contents_url': '%s%s/contents/{+path}' % (ROOT_URL, REPNAME_OCB),
-    'has_pages': False,
-    'git_refs_url': '%s%s/git/refs{/sha}' % (ROOT_URL, REPNAME_OCB),
-    'open_issues_count': 0,
-    'has_projects': True,
-    'clone_url': '%s%s.git' % (ROOT_URL, REPNAME_OCB),
-    'watchers_count': 0,
-    'git_tags_url': '%s%s/git/tags{/sha}' % (ROOT_URL, REPNAME_OCB),
-    'milestones_url': '%s%s/milestones{/number}' % (ROOT_URL, REPNAME_OCB),
-    'languages_url': '%s%s/languages' % (ROOT_URL, REPNAME_OCB),
-    'size': 1884251,
-    'homepage': '',
-    'fork': True,
-    'commits_url': '%s%s/commits{/sha}' % (ROOT_URL, REPNAME_OCB),
-    'releases_url': '%s%s/releases{id}' % (ROOT_URL, REPNAME_OCB),
-    'issue_events_url': '%s%s/issues/events{/number}' % (ROOT_URL, REPNAME_OCB),
-    'archive_url': '%s%s/{archive_format}{/ref}' % (ROOT_URL, REPNAME_OCB),
-    'comments_url': '%s%s/comments{number}' % (ROOT_URL, REPNAME_OCB),
-    'events_url': '%s%s/events' % (ROOT_URL, REPNAME_OCB),
-    'contributors_url': '%s%s/contributors' % (ROOT_URL, REPNAME_OCB),
-    'html_url': '%s%s' % (ROOT_URL, REPNAME_OCB),
-    'forks': 0,
-    'compare_url': '%s%s/compare/{base}...{ead}' % (ROOT_URL, REPNAME_OCB),
-    'open_issues': 0,
-    'node_id': 'MDEwOlJlcG9zaXRvcnk1ODM4OTkzNg==',
-    'git_url': 'git://github.com/zeroincombenze/%s.git' % REPNAME_OCB,
-    'svn_url': '%s%s/%s' % (ROOT_URL, REPNAME_OCB, REPNAME_OCB),
-    'merges_url': '%s%s/merges' % (ROOT_URL, REPNAME_OCB),
-    'has_issues': False,
-    'ssh_url': 'git@github.com:zeroincombenze/%s.git' % REPNAME_OCB,
-    'blobs_url': '%s%s/git/blobs{/sha}' % (ROOT_URL, REPNAME_OCB),
-    'git_commits_url': '%s%s/git/commits{/sha}' % (ROOT_URL, REPNAME_OCB),
-    'hooks_url': '%s%s/hooks' % (ROOT_URL, REPNAME_OCB),
-    'has_downloads': True,
-    'license': {
-        'spdx_id': 'AGPL-3.0',
-        'url': 'https://api.github.com/licenses/agpl-3.0',
-        'node_id': 'MDc6TGljZW5zZTE=',
-        'name': 'GNU Affero General Public License v3.0',
-        'key': 'agpl-3.0',
+    "statuses_url": "%s%s/statuses/{sha}" % (ROOT_URL, REPNAME_OCB),
+    "id": 58389479,
+    "keys_url": "%s%s/keys{/key_id}" % (ROOT_URL, REPNAME_OCB),
+    "description": "Odoo Accountant closing tools",
+    "tags_url": "%s%s/tags" % (ROOT_URL, REPNAME_OCB),
+    "archived": False,
+    "downloads_url": "%s%s/downloads" % (ROOT_URL, REPNAME_OCB),
+    "assignees_url": "%s%s/assignees{/user}" % (ROOT_URL, REPNAME_OCB),
+    "contents_url": "%s%s/contents/{+path}" % (ROOT_URL, REPNAME_OCB),
+    "has_pages": False,
+    "git_refs_url": "%s%s/git/refs{/sha}" % (ROOT_URL, REPNAME_OCB),
+    "open_issues_count": 0,
+    "has_projects": True,
+    "clone_url": "%s%s.git" % (ROOT_URL, REPNAME_OCB),
+    "watchers_count": 0,
+    "git_tags_url": "%s%s/git/tags{/sha}" % (ROOT_URL, REPNAME_OCB),
+    "milestones_url": "%s%s/milestones{/number}" % (ROOT_URL, REPNAME_OCB),
+    "languages_url": "%s%s/languages" % (ROOT_URL, REPNAME_OCB),
+    "size": 1884251,
+    "homepage": "",
+    "fork": True,
+    "commits_url": "%s%s/commits{/sha}" % (ROOT_URL, REPNAME_OCB),
+    "releases_url": "%s%s/releases{id}" % (ROOT_URL, REPNAME_OCB),
+    "issue_events_url": "%s%s/issues/events{/number}" % (ROOT_URL, REPNAME_OCB),
+    "archive_url": "%s%s/{archive_format}{/ref}" % (ROOT_URL, REPNAME_OCB),
+    "comments_url": "%s%s/comments{number}" % (ROOT_URL, REPNAME_OCB),
+    "events_url": "%s%s/events" % (ROOT_URL, REPNAME_OCB),
+    "contributors_url": "%s%s/contributors" % (ROOT_URL, REPNAME_OCB),
+    "html_url": "%s%s" % (ROOT_URL, REPNAME_OCB),
+    "forks": 0,
+    "compare_url": "%s%s/compare/{base}...{ead}" % (ROOT_URL, REPNAME_OCB),
+    "open_issues": 0,
+    "node_id": "MDEwOlJlcG9zaXRvcnk1ODM4OTkzNg==",
+    "git_url": "git://github.com/zeroincombenze/%s.git" % REPNAME_OCB,
+    "svn_url": "%s%s/%s" % (ROOT_URL, REPNAME_OCB, REPNAME_OCB),
+    "merges_url": "%s%s/merges" % (ROOT_URL, REPNAME_OCB),
+    "has_issues": False,
+    "ssh_url": "git@github.com:zeroincombenze/%s.git" % REPNAME_OCB,
+    "blobs_url": "%s%s/git/blobs{/sha}" % (ROOT_URL, REPNAME_OCB),
+    "git_commits_url": "%s%s/git/commits{/sha}" % (ROOT_URL, REPNAME_OCB),
+    "hooks_url": "%s%s/hooks" % (ROOT_URL, REPNAME_OCB),
+    "has_downloads": True,
+    "license": {
+        "spdx_id": "AGPL-3.0",
+        "url": "https://api.github.com/licenses/agpl-3.0",
+        "node_id": "MDc6TGljZW5zZTE=",
+        "name": "GNU Affero General Public License v3.0",
+        "key": "agpl-3.0",
     },
-    'name': '%s' % REPNAME_OCB,
-    'language': 'Python',
-    'url': '%s%s' % (ROOT_URL, REPNAME_OCB),
-    'created_at': '2016-05-09T16:03:20Z',
-    'watchers': 0,
-    'pushed_at': '2018-06-06T12:58:38Z',
-    'forks_count': 0,
-    'default_branch': '7.0',
-    'teams_url': '%s%s/teams' % (ROOT_URL, REPNAME_OCB),
-    'trees_url': '%s%s/git/trees{/sha}' % (ROOT_URL, REPNAME_OCB),
-    'branches_url': '%s%s/branches{/branch}' % (ROOT_URL, REPNAME_OCB),
-    'subscribers_url': '%s%s/subscribers' % (ROOT_URL, REPNAME_OCB),
-    'stargazers_url': '%s%s/stargazers' % (ROOT_URL, REPNAME_OCB),
+    "name": "%s" % REPNAME_OCB,
+    "language": "Python",
+    "url": "%s%s" % (ROOT_URL, REPNAME_OCB),
+    "created_at": "2016-05-09T16:03:20Z",
+    "watchers": 0,
+    "pushed_at": "2018-06-06T12:58:38Z",
+    "forks_count": 0,
+    "default_branch": "7.0",
+    "teams_url": "%s%s/teams" % (ROOT_URL, REPNAME_OCB),
+    "trees_url": "%s%s/git/trees{/sha}" % (ROOT_URL, REPNAME_OCB),
+    "branches_url": "%s%s/branches{/branch}" % (ROOT_URL, REPNAME_OCB),
+    "subscribers_url": "%s%s/subscribers" % (ROOT_URL, REPNAME_OCB),
+    "stargazers_url": "%s%s/stargazers" % (ROOT_URL, REPNAME_OCB),
 }
-REPNAME_ACC_CLO = 'account-closing'
+REPNAME_ACC_CLO = "account-closing"
 TEST_REP_ACC_CLO = {
-    'issues_url': '%s%s/issues{/number}' % (ROOT_URL, REPNAME_ACC_CLO),
-    'deployments_url': '%s%s/deployments' % (ROOT_URL, REPNAME_ACC_CLO),
-    'stargazers_count': 0,
-    'forks_url': '%s%s/forks' % (ROOT_URL, REPNAME_ACC_CLO),
-    'mirror_url': None,
-    'subscription_url': '%s%s/subscription' % (ROOT_URL, REPNAME_ACC_CLO),
-    'notifications_url': '%s%s/notifications{?since,all,participating}'
+    "issues_url": "%s%s/issues{/number}" % (ROOT_URL, REPNAME_ACC_CLO),
+    "deployments_url": "%s%s/deployments" % (ROOT_URL, REPNAME_ACC_CLO),
+    "stargazers_count": 0,
+    "forks_url": "%s%s/forks" % (ROOT_URL, REPNAME_ACC_CLO),
+    "mirror_url": None,
+    "subscription_url": "%s%s/subscription" % (ROOT_URL, REPNAME_ACC_CLO),
+    "notifications_url": "%s%s/notifications{?since,all,participating}"
     % (ROOT_URL, REPNAME_ACC_CLO),
-    'collaborators_url':
-        '%s%s/collaborators{collaborator}' % (ROOT_URL, REPNAME_ACC_CLO),
-    'updated_at': '2018-03-29T20:26:20Z',
-    'private': False,
-    'pulls_url': '%s%s/pulls{/number}' % (ROOT_URL, REPNAME_ACC_CLO),
-    'disabled': False,
-    'issue_comment_url': '%s%s/issues/comments{number}' % (ROOT_URL, REPNAME_ACC_CLO),
-    'labels_url': '%s%s/labels{/name}' % (ROOT_URL, REPNAME_ACC_CLO),
-    'has_wiki': True,
-    'full_name': 'zeroincombenze/%s' % REPNAME_ACC_CLO,
-    'owner': {
-        'following_url': '%s%s/following{other_user}' % (ROOT_URL, REPNAME_ACC_CLO),
-        'events_url': '%s%s/events{/privacy}' % (ROOT_URL, REPNAME_ACC_CLO),
-        'avatar_url': 'https://avatars2.githubusercontent.com/u/123?v=4',
-        'url': '%s%s' % (USER_URL, REPNAME_ACC_CLO),
-        'gists_url': '%s%s/gists{/gist_id}' % (USER_URL, REPNAME_ACC_CLO),
-        'html_url': 'https://github.com/%s' % REPNAME_ACC_CLO,
-        'subscriptions_url': '%s%s/subscriptions' % (USER_URL, REPNAME_ACC_CLO),
-        'node_id': 'MDQ6VXNlcjY5NzI1NTU=',
-        'test_repos_url': '%s%s/test_repos' % (USER_URL, REPNAME_ACC_CLO),
-        'received_events_url': '%s%s/received_events' % (USER_URL, REPNAME_ACC_CLO),
-        'gravatar_id': '',
-        'starred_url':
-            '%s%s/starred{/owner}{/TEST_REPo}' % (USER_URL, REPNAME_ACC_CLO),
-        'site_admin': False,
-        'login': 'zeroincombenze',
-        'type': 'User',
-        'id': 6972555,
-        'followers_url': '%s%s/followers' % (USER_URL, REPNAME_ACC_CLO),
-        'organizations_url': '%s%s/orgs' % (USER_URL, REPNAME_ACC_CLO),
+    "collaborators_url": "%s%s/collaborators{collaborator}"
+    % (ROOT_URL, REPNAME_ACC_CLO),
+    "updated_at": "2018-03-29T20:26:20Z",
+    "private": False,
+    "pulls_url": "%s%s/pulls{/number}" % (ROOT_URL, REPNAME_ACC_CLO),
+    "disabled": False,
+    "issue_comment_url": "%s%s/issues/comments{number}" % (ROOT_URL, REPNAME_ACC_CLO),
+    "labels_url": "%s%s/labels{/name}" % (ROOT_URL, REPNAME_ACC_CLO),
+    "has_wiki": True,
+    "full_name": "zeroincombenze/%s" % REPNAME_ACC_CLO,
+    "owner": {
+        "following_url": "%s%s/following{other_user}" % (ROOT_URL, REPNAME_ACC_CLO),
+        "events_url": "%s%s/events{/privacy}" % (ROOT_URL, REPNAME_ACC_CLO),
+        "avatar_url": "https://avatars2.githubusercontent.com/u/123?v=4",
+        "url": "%s%s" % (USER_URL, REPNAME_ACC_CLO),
+        "gists_url": "%s%s/gists{/gist_id}" % (USER_URL, REPNAME_ACC_CLO),
+        "html_url": "https://github.com/%s" % REPNAME_ACC_CLO,
+        "subscriptions_url": "%s%s/subscriptions" % (USER_URL, REPNAME_ACC_CLO),
+        "node_id": "MDQ6VXNlcjY5NzI1NTU=",
+        "test_repos_url": "%s%s/test_repos" % (USER_URL, REPNAME_ACC_CLO),
+        "received_events_url": "%s%s/received_events" % (USER_URL, REPNAME_ACC_CLO),
+        "gravatar_id": "",
+        "starred_url": "%s%s/starred{/owner}{/TEST_REPo}" % (USER_URL, REPNAME_ACC_CLO),
+        "site_admin": False,
+        "login": "zeroincombenze",
+        "type": "User",
+        "id": 6972555,
+        "followers_url": "%s%s/followers" % (USER_URL, REPNAME_ACC_CLO),
+        "organizations_url": "%s%s/orgs" % (USER_URL, REPNAME_ACC_CLO),
     },
-    'statuses_url': '%s%s/statuses/{sha}' % (ROOT_URL, REPNAME_ACC_CLO),
-    'id': 58389936,
-    'keys_url': '%s%s/keys{/key_id}' % (ROOT_URL, REPNAME_ACC_CLO),
-    'description': 'Odoo Accountant closing tools',
-    'tags_url': '%s%s/tags' % (ROOT_URL, REPNAME_ACC_CLO),
-    'archived': False,
-    'downloads_url': '%s%s/downloads' % (ROOT_URL, REPNAME_ACC_CLO),
-    'assignees_url': '%s%s/assignees{/user}' % (ROOT_URL, REPNAME_ACC_CLO),
-    'contents_url': '%s%s/contents/{+path}' % (ROOT_URL, REPNAME_ACC_CLO),
-    'has_pages': False,
-    'git_refs_url': '%s%s/git/refs{/sha}' % (ROOT_URL, REPNAME_ACC_CLO),
-    'open_issues_count': 0,
-    'has_projects': True,
-    'clone_url': '%s%s.git' % (ROOT_URL, REPNAME_ACC_CLO),
-    'watchers_count': 0,
-    'git_tags_url': '%s%s/git/tags{/sha}' % (ROOT_URL, REPNAME_ACC_CLO),
-    'milestones_url': '%s%s/milestones{/number}' % (ROOT_URL, REPNAME_ACC_CLO),
-    'languages_url': '%s%s/languages' % (ROOT_URL, REPNAME_ACC_CLO),
-    'size': 1884706,
-    'homepage': '',
-    'fork': True,
-    'commits_url': '%s%s/commits{/sha}' % (ROOT_URL, REPNAME_ACC_CLO),
-    'releases_url': '%s%s/releases{id}' % (ROOT_URL, REPNAME_ACC_CLO),
-    'issue_events_url': '%s%s/issues/events{/number}' % (ROOT_URL, REPNAME_ACC_CLO),
-    'archive_url': '%s%s/{archive_format}{/ref}' % (ROOT_URL, REPNAME_ACC_CLO),
-    'comments_url': '%s%s/comments{number}' % (ROOT_URL, REPNAME_ACC_CLO),
-    'events_url': '%s%s/events' % (ROOT_URL, REPNAME_ACC_CLO),
-    'contributors_url': '%s%s/contributors' % (ROOT_URL, REPNAME_ACC_CLO),
-    'html_url': '%s%s' % (ROOT_URL, REPNAME_ACC_CLO),
-    'forks': 0,
-    'compare_url': '%s%s/compare/{base}...{ead}' % (ROOT_URL, REPNAME_ACC_CLO),
-    'open_issues': 0,
-    'node_id': 'MDEwOlJlcG9zaXRvcnk1ODM4OTkzNg==',
-    'git_url': 'git://github.com/zeroincombenze/%s.git' % REPNAME_ACC_CLO,
-    'svn_url': '%s%s/%s' % (ROOT_URL, REPNAME_ACC_CLO, REPNAME_ACC_CLO),
-    'merges_url': '%s%s/merges' % (ROOT_URL, REPNAME_ACC_CLO),
-    'has_issues': False,
-    'ssh_url': 'git@github.com:zeroincombenze/%s.git' % REPNAME_ACC_CLO,
-    'blobs_url': '%s%s/git/blobs{/sha}' % (ROOT_URL, REPNAME_ACC_CLO),
-    'git_commits_url': '%s%s/git/commits{/sha}' % (ROOT_URL, REPNAME_ACC_CLO),
-    'hooks_url': '%s%s/hooks' % (ROOT_URL, REPNAME_ACC_CLO),
-    'has_downloads': True,
-    'license': {
-        'spdx_id': 'AGPL-3.0',
-        'url': 'https://api.github.com/licenses/agpl-3.0',
-        'node_id': 'MDc6TGljZW5zZTE=',
-        'name': 'GNU Affero General Public License v3.0',
-        'key': 'agpl-3.0',
+    "statuses_url": "%s%s/statuses/{sha}" % (ROOT_URL, REPNAME_ACC_CLO),
+    "id": 58389936,
+    "keys_url": "%s%s/keys{/key_id}" % (ROOT_URL, REPNAME_ACC_CLO),
+    "description": "Odoo Accountant closing tools",
+    "tags_url": "%s%s/tags" % (ROOT_URL, REPNAME_ACC_CLO),
+    "archived": False,
+    "downloads_url": "%s%s/downloads" % (ROOT_URL, REPNAME_ACC_CLO),
+    "assignees_url": "%s%s/assignees{/user}" % (ROOT_URL, REPNAME_ACC_CLO),
+    "contents_url": "%s%s/contents/{+path}" % (ROOT_URL, REPNAME_ACC_CLO),
+    "has_pages": False,
+    "git_refs_url": "%s%s/git/refs{/sha}" % (ROOT_URL, REPNAME_ACC_CLO),
+    "open_issues_count": 0,
+    "has_projects": True,
+    "clone_url": "%s%s.git" % (ROOT_URL, REPNAME_ACC_CLO),
+    "watchers_count": 0,
+    "git_tags_url": "%s%s/git/tags{/sha}" % (ROOT_URL, REPNAME_ACC_CLO),
+    "milestones_url": "%s%s/milestones{/number}" % (ROOT_URL, REPNAME_ACC_CLO),
+    "languages_url": "%s%s/languages" % (ROOT_URL, REPNAME_ACC_CLO),
+    "size": 1884706,
+    "homepage": "",
+    "fork": True,
+    "commits_url": "%s%s/commits{/sha}" % (ROOT_URL, REPNAME_ACC_CLO),
+    "releases_url": "%s%s/releases{id}" % (ROOT_URL, REPNAME_ACC_CLO),
+    "issue_events_url": "%s%s/issues/events{/number}" % (ROOT_URL, REPNAME_ACC_CLO),
+    "archive_url": "%s%s/{archive_format}{/ref}" % (ROOT_URL, REPNAME_ACC_CLO),
+    "comments_url": "%s%s/comments{number}" % (ROOT_URL, REPNAME_ACC_CLO),
+    "events_url": "%s%s/events" % (ROOT_URL, REPNAME_ACC_CLO),
+    "contributors_url": "%s%s/contributors" % (ROOT_URL, REPNAME_ACC_CLO),
+    "html_url": "%s%s" % (ROOT_URL, REPNAME_ACC_CLO),
+    "forks": 0,
+    "compare_url": "%s%s/compare/{base}...{ead}" % (ROOT_URL, REPNAME_ACC_CLO),
+    "open_issues": 0,
+    "node_id": "MDEwOlJlcG9zaXRvcnk1ODM4OTkzNg==",
+    "git_url": "git://github.com/zeroincombenze/%s.git" % REPNAME_ACC_CLO,
+    "svn_url": "%s%s/%s" % (ROOT_URL, REPNAME_ACC_CLO, REPNAME_ACC_CLO),
+    "merges_url": "%s%s/merges" % (ROOT_URL, REPNAME_ACC_CLO),
+    "has_issues": False,
+    "ssh_url": "git@github.com:zeroincombenze/%s.git" % REPNAME_ACC_CLO,
+    "blobs_url": "%s%s/git/blobs{/sha}" % (ROOT_URL, REPNAME_ACC_CLO),
+    "git_commits_url": "%s%s/git/commits{/sha}" % (ROOT_URL, REPNAME_ACC_CLO),
+    "hooks_url": "%s%s/hooks" % (ROOT_URL, REPNAME_ACC_CLO),
+    "has_downloads": True,
+    "license": {
+        "spdx_id": "AGPL-3.0",
+        "url": "https://api.github.com/licenses/agpl-3.0",
+        "node_id": "MDc6TGljZW5zZTE=",
+        "name": "GNU Affero General Public License v3.0",
+        "key": "agpl-3.0",
     },
-    'name': '%s' % REPNAME_ACC_CLO,
-    'language': 'Python',
-    'url': '%s%s' % (ROOT_URL, REPNAME_ACC_CLO),
-    'created_at': '2016-05-09T16:03:20Z',
-    'watchers': 0,
-    'pushed_at': '2018-06-06T12:58:38Z',
-    'forks_count': 0,
-    'default_branch': '7.0',
-    'teams_url': '%s%s/teams' % (ROOT_URL, REPNAME_ACC_CLO),
-    'trees_url': '%s%s/git/trees{/sha}' % (ROOT_URL, REPNAME_ACC_CLO),
-    'branches_url': '%s%s/branches{/branch}' % (ROOT_URL, REPNAME_ACC_CLO),
-    'subscribers_url': '%s%s/subscribers' % (ROOT_URL, REPNAME_ACC_CLO),
-    'stargazers_url': '%s%s/stargazers' % (ROOT_URL, REPNAME_ACC_CLO),
+    "name": "%s" % REPNAME_ACC_CLO,
+    "language": "Python",
+    "url": "%s%s" % (ROOT_URL, REPNAME_ACC_CLO),
+    "created_at": "2016-05-09T16:03:20Z",
+    "watchers": 0,
+    "pushed_at": "2018-06-06T12:58:38Z",
+    "forks_count": 0,
+    "default_branch": "7.0",
+    "teams_url": "%s%s/teams" % (ROOT_URL, REPNAME_ACC_CLO),
+    "trees_url": "%s%s/git/trees{/sha}" % (ROOT_URL, REPNAME_ACC_CLO),
+    "branches_url": "%s%s/branches{/branch}" % (ROOT_URL, REPNAME_ACC_CLO),
+    "subscribers_url": "%s%s/subscribers" % (ROOT_URL, REPNAME_ACC_CLO),
+    "stargazers_url": "%s%s/stargazers" % (ROOT_URL, REPNAME_ACC_CLO),
 }
-REPNAME_L10N_IT = 'l10n-italy'
+REPNAME_L10N_IT = "l10n-italy"
 TEST_REP_L10N_IT = {
-    'issues_url': '%s%s/issues{/number}' % (ROOT_URL, REPNAME_L10N_IT),
-    'deployments_url': '%s%s/deployments' % (ROOT_URL, REPNAME_L10N_IT),
-    'stargazers_count': 0,
-    'forks_url': '%s%s/forks' % (ROOT_URL, REPNAME_L10N_IT),
-    'mirror_url': None,
-    'subscription_url': '%s%s/subscription' % (ROOT_URL, REPNAME_L10N_IT),
-    'notifications_url': '%s%s/notifications{?since,all,participating}'
+    "issues_url": "%s%s/issues{/number}" % (ROOT_URL, REPNAME_L10N_IT),
+    "deployments_url": "%s%s/deployments" % (ROOT_URL, REPNAME_L10N_IT),
+    "stargazers_count": 0,
+    "forks_url": "%s%s/forks" % (ROOT_URL, REPNAME_L10N_IT),
+    "mirror_url": None,
+    "subscription_url": "%s%s/subscription" % (ROOT_URL, REPNAME_L10N_IT),
+    "notifications_url": "%s%s/notifications{?since,all,participating}"
+    % (ROOT_URL, REPNAME_L10N_IT),
+    "collaborators_url": "%s%s/collaborators{collaborator}"
     % (ROOT_URL, REPNAME_L10N_IT),
-    'collaborators_url':
-        '%s%s/collaborators{collaborator}' % (ROOT_URL, REPNAME_L10N_IT),
-    'updated_at': '2018-03-29T20:26:20Z',
-    'private': False,
-    'pulls_url': '%s%s/pulls{/number}' % (ROOT_URL, REPNAME_L10N_IT),
-    'disabled': False,
-    'issue_comment_url': '%s%s/issues/comments{number}' % (ROOT_URL, REPNAME_L10N_IT),
-    'labels_url': '%s%s/labels{/name}' % (ROOT_URL, REPNAME_L10N_IT),
-    'has_wiki': True,
-    'full_name': 'zeroincombenze/%s' % REPNAME_L10N_IT,
-    'owner': {
-        'following_url': '%s%s/following{other_user}' % (ROOT_URL, REPNAME_L10N_IT),
-        'events_url': '%s%s/events{/privacy}' % (ROOT_URL, REPNAME_L10N_IT),
-        'avatar_url': 'https://avatars2.githubusercontent.com/u/123?v=4',
-        'url': '%s%s' % (USER_URL, REPNAME_L10N_IT),
-        'gists_url': '%s%s/gists{/gist_id}' % (USER_URL, REPNAME_L10N_IT),
-        'html_url': 'https://github.com/%s' % REPNAME_L10N_IT,
-        'subscriptions_url': '%s%s/subscriptions' % (USER_URL, REPNAME_L10N_IT),
-        'node_id': 'MDQ6VXNlcjY5NzI1NTU=',
-        'test_repos_url': '%s%s/test_repos' % (USER_URL, REPNAME_L10N_IT),
-        'received_events_url': '%s%s/received_events' % (USER_URL, REPNAME_L10N_IT),
-        'gravatar_id': '',
-        'starred_url':
-            '%s%s/starred{/owner}{/TEST_REPo}' % (USER_URL, REPNAME_L10N_IT),
-        'site_admin': False,
-        'login': 'zeroincombenze',
-        'type': 'User',
-        'id': 6972556,
-        'followers_url': '%s%s/followers' % (USER_URL, REPNAME_L10N_IT),
-        'organizations_url': '%s%s/orgs' % (USER_URL, REPNAME_L10N_IT),
+    "updated_at": "2018-03-29T20:26:20Z",
+    "private": False,
+    "pulls_url": "%s%s/pulls{/number}" % (ROOT_URL, REPNAME_L10N_IT),
+    "disabled": False,
+    "issue_comment_url": "%s%s/issues/comments{number}" % (ROOT_URL, REPNAME_L10N_IT),
+    "labels_url": "%s%s/labels{/name}" % (ROOT_URL, REPNAME_L10N_IT),
+    "has_wiki": True,
+    "full_name": "zeroincombenze/%s" % REPNAME_L10N_IT,
+    "owner": {
+        "following_url": "%s%s/following{other_user}" % (ROOT_URL, REPNAME_L10N_IT),
+        "events_url": "%s%s/events{/privacy}" % (ROOT_URL, REPNAME_L10N_IT),
+        "avatar_url": "https://avatars2.githubusercontent.com/u/123?v=4",
+        "url": "%s%s" % (USER_URL, REPNAME_L10N_IT),
+        "gists_url": "%s%s/gists{/gist_id}" % (USER_URL, REPNAME_L10N_IT),
+        "html_url": "https://github.com/%s" % REPNAME_L10N_IT,
+        "subscriptions_url": "%s%s/subscriptions" % (USER_URL, REPNAME_L10N_IT),
+        "node_id": "MDQ6VXNlcjY5NzI1NTU=",
+        "test_repos_url": "%s%s/test_repos" % (USER_URL, REPNAME_L10N_IT),
+        "received_events_url": "%s%s/received_events" % (USER_URL, REPNAME_L10N_IT),
+        "gravatar_id": "",
+        "starred_url": "%s%s/starred{/owner}{/TEST_REPo}" % (USER_URL, REPNAME_L10N_IT),
+        "site_admin": False,
+        "login": "zeroincombenze",
+        "type": "User",
+        "id": 6972556,
+        "followers_url": "%s%s/followers" % (USER_URL, REPNAME_L10N_IT),
+        "organizations_url": "%s%s/orgs" % (USER_URL, REPNAME_L10N_IT),
     },
-    'statuses_url': '%s%s/statuses/{sha}' % (ROOT_URL, REPNAME_L10N_IT),
-    'id': 58389937,
-    'keys_url': '%s%s/keys{/key_id}' % (ROOT_URL, REPNAME_L10N_IT),
-    'description': 'Italy localization',
-    'tags_url': '%s%s/tags' % (ROOT_URL, REPNAME_L10N_IT),
-    'archived': False,
-    'downloads_url': '%s%s/downloads' % (ROOT_URL, REPNAME_L10N_IT),
-    'assignees_url': '%s%s/assignees{/user}' % (ROOT_URL, REPNAME_L10N_IT),
-    'contents_url': '%s%s/contents/{+path}' % (ROOT_URL, REPNAME_L10N_IT),
-    'has_pages': False,
-    'git_refs_url': '%s%s/git/refs{/sha}' % (ROOT_URL, REPNAME_L10N_IT),
-    'open_issues_count': 0,
-    'has_projects': True,
-    'clone_url': '%s%s.git' % (ROOT_URL, REPNAME_L10N_IT),
-    'watchers_count': 0,
-    'git_tags_url': '%s%s/git/tags{/sha}' % (ROOT_URL, REPNAME_L10N_IT),
-    'milestones_url': '%s%s/milestones{/number}' % (ROOT_URL, REPNAME_L10N_IT),
-    'languages_url': '%s%s/languages' % (ROOT_URL, REPNAME_L10N_IT),
-    'size': 1884707,
-    'homepage': '',
-    'fork': True,
-    'commits_url': '%s%s/commits{/sha}' % (ROOT_URL, REPNAME_L10N_IT),
-    'releases_url': '%s%s/releases{id}' % (ROOT_URL, REPNAME_L10N_IT),
-    'issue_events_url': '%s%s/issues/events{/number}' % (ROOT_URL, REPNAME_L10N_IT),
-    'archive_url': '%s%s/{archive_format}{/ref}' % (ROOT_URL, REPNAME_L10N_IT),
-    'comments_url': '%s%s/comments{number}' % (ROOT_URL, REPNAME_L10N_IT),
-    'events_url': '%s%s/events' % (ROOT_URL, REPNAME_L10N_IT),
-    'contributors_url': '%s%s/contributors' % (ROOT_URL, REPNAME_L10N_IT),
-    'html_url': '%s%s' % (ROOT_URL, REPNAME_L10N_IT),
-    'forks': 0,
-    'compare_url': '%s%s/compare/{base}...{ead}' % (ROOT_URL, REPNAME_L10N_IT),
-    'open_issues': 0,
-    'node_id': 'MDEwOlJlcG9zaXRvcnk1ODM4OTkzNg==',
-    'git_url': 'git://github.com/zeroincombenze/%s.git' % REPNAME_L10N_IT,
-    'svn_url': '%s%s/%s' % (ROOT_URL, REPNAME_L10N_IT, REPNAME_L10N_IT),
-    'merges_url': '%s%s/merges' % (ROOT_URL, REPNAME_L10N_IT),
-    'has_issues': False,
-    'ssh_url': 'git@github.com:zeroincombenze/%s.git' % REPNAME_L10N_IT,
-    'blobs_url': '%s%s/git/blobs{/sha}' % (ROOT_URL, REPNAME_L10N_IT),
-    'git_commits_url': '%s%s/git/commits{/sha}' % (ROOT_URL, REPNAME_L10N_IT),
-    'hooks_url': '%s%s/hooks' % (ROOT_URL, REPNAME_L10N_IT),
-    'has_downloads': True,
-    'license': {
-        'spdx_id': 'AGPL-3.0',
-        'url': 'https://api.github.com/licenses/agpl-3.0',
-        'node_id': 'MDc6TGljZW5zZTE=',
-        'name': 'GNU Affero General Public License v3.0',
-        'key': 'agpl-3.0',
+    "statuses_url": "%s%s/statuses/{sha}" % (ROOT_URL, REPNAME_L10N_IT),
+    "id": 58389937,
+    "keys_url": "%s%s/keys{/key_id}" % (ROOT_URL, REPNAME_L10N_IT),
+    "description": "Italy localization",
+    "tags_url": "%s%s/tags" % (ROOT_URL, REPNAME_L10N_IT),
+    "archived": False,
+    "downloads_url": "%s%s/downloads" % (ROOT_URL, REPNAME_L10N_IT),
+    "assignees_url": "%s%s/assignees{/user}" % (ROOT_URL, REPNAME_L10N_IT),
+    "contents_url": "%s%s/contents/{+path}" % (ROOT_URL, REPNAME_L10N_IT),
+    "has_pages": False,
+    "git_refs_url": "%s%s/git/refs{/sha}" % (ROOT_URL, REPNAME_L10N_IT),
+    "open_issues_count": 0,
+    "has_projects": True,
+    "clone_url": "%s%s.git" % (ROOT_URL, REPNAME_L10N_IT),
+    "watchers_count": 0,
+    "git_tags_url": "%s%s/git/tags{/sha}" % (ROOT_URL, REPNAME_L10N_IT),
+    "milestones_url": "%s%s/milestones{/number}" % (ROOT_URL, REPNAME_L10N_IT),
+    "languages_url": "%s%s/languages" % (ROOT_URL, REPNAME_L10N_IT),
+    "size": 1884707,
+    "homepage": "",
+    "fork": True,
+    "commits_url": "%s%s/commits{/sha}" % (ROOT_URL, REPNAME_L10N_IT),
+    "releases_url": "%s%s/releases{id}" % (ROOT_URL, REPNAME_L10N_IT),
+    "issue_events_url": "%s%s/issues/events{/number}" % (ROOT_URL, REPNAME_L10N_IT),
+    "archive_url": "%s%s/{archive_format}{/ref}" % (ROOT_URL, REPNAME_L10N_IT),
+    "comments_url": "%s%s/comments{number}" % (ROOT_URL, REPNAME_L10N_IT),
+    "events_url": "%s%s/events" % (ROOT_URL, REPNAME_L10N_IT),
+    "contributors_url": "%s%s/contributors" % (ROOT_URL, REPNAME_L10N_IT),
+    "html_url": "%s%s" % (ROOT_URL, REPNAME_L10N_IT),
+    "forks": 0,
+    "compare_url": "%s%s/compare/{base}...{ead}" % (ROOT_URL, REPNAME_L10N_IT),
+    "open_issues": 0,
+    "node_id": "MDEwOlJlcG9zaXRvcnk1ODM4OTkzNg==",
+    "git_url": "git://github.com/zeroincombenze/%s.git" % REPNAME_L10N_IT,
+    "svn_url": "%s%s/%s" % (ROOT_URL, REPNAME_L10N_IT, REPNAME_L10N_IT),
+    "merges_url": "%s%s/merges" % (ROOT_URL, REPNAME_L10N_IT),
+    "has_issues": False,
+    "ssh_url": "git@github.com:zeroincombenze/%s.git" % REPNAME_L10N_IT,
+    "blobs_url": "%s%s/git/blobs{/sha}" % (ROOT_URL, REPNAME_L10N_IT),
+    "git_commits_url": "%s%s/git/commits{/sha}" % (ROOT_URL, REPNAME_L10N_IT),
+    "hooks_url": "%s%s/hooks" % (ROOT_URL, REPNAME_L10N_IT),
+    "has_downloads": True,
+    "license": {
+        "spdx_id": "AGPL-3.0",
+        "url": "https://api.github.com/licenses/agpl-3.0",
+        "node_id": "MDc6TGljZW5zZTE=",
+        "name": "GNU Affero General Public License v3.0",
+        "key": "agpl-3.0",
     },
-    'name': '%s' % REPNAME_L10N_IT,
-    'language': 'Python',
-    'url': '%s%s' % (ROOT_URL, REPNAME_L10N_IT),
-    'created_at': '2016-05-09T16:03:20Z',
-    'watchers': 0,
-    'pushed_at': '2018-06-06T12:58:38Z',
-    'forks_count': 0,
-    'default_branch': '7.0',
-    'teams_url': '%s%s/teams' % (ROOT_URL, REPNAME_L10N_IT),
-    'trees_url': '%s%s/git/trees{/sha}' % (ROOT_URL, REPNAME_L10N_IT),
-    'branches_url': '%s%s/branches{/branch}' % (ROOT_URL, REPNAME_L10N_IT),
-    'subscribers_url': '%s%s/subscribers' % (ROOT_URL, REPNAME_L10N_IT),
-    'stargazers_url': '%s%s/stargazers' % (ROOT_URL, REPNAME_L10N_IT),
+    "name": "%s" % REPNAME_L10N_IT,
+    "language": "Python",
+    "url": "%s%s" % (ROOT_URL, REPNAME_L10N_IT),
+    "created_at": "2016-05-09T16:03:20Z",
+    "watchers": 0,
+    "pushed_at": "2018-06-06T12:58:38Z",
+    "forks_count": 0,
+    "default_branch": "7.0",
+    "teams_url": "%s%s/teams" % (ROOT_URL, REPNAME_L10N_IT),
+    "trees_url": "%s%s/git/trees{/sha}" % (ROOT_URL, REPNAME_L10N_IT),
+    "branches_url": "%s%s/branches{/branch}" % (ROOT_URL, REPNAME_L10N_IT),
+    "subscribers_url": "%s%s/subscribers" % (ROOT_URL, REPNAME_L10N_IT),
+    "stargazers_url": "%s%s/stargazers" % (ROOT_URL, REPNAME_L10N_IT),
 }
 
 
 def get_list_from_url(opt_args, git_org):
     def name_is_valid(opt_args, name):
         if (
             (
-                not name.startswith('.')
-                and not name.startswith('connector-')
-                and not name.startswith('maintainer-')
-                and not name.startswith('oca-')
-                and not name.startswith('odoo-')
-                and not name.startswith('vertical-')
-                and not name.startswith('l10n-')
+                not name.startswith(".")
+                and not name.startswith("connector-")
+                and not name.startswith("maintainer-")
+                and not name.startswith("oca-")
+                and not name.startswith("odoo-")
+                and not name.startswith("vertical-")
+                and not name.startswith("l10n-")
                 and name not in DEVEL_REPS
             )
-            or (name.startswith('connector-') and 'connector' in opt_args.extra)
-            or (name.startswith('maintainer-') and 'maintainer' in opt_args.extra)
-            or (name.startswith('oca-') and 'oca' in opt_args.extra)
-            or (name.startswith('odoo-') and 'odoo' in opt_args.extra)
-            or (name.startswith('vertical-') and 'vertical' in opt_args.extra)
-            or (name in DEVEL_REPS and 'devel' in opt_args.extra)
-            or (name.startswith('l10n-') and name in opt_args.l10n)
+            or (name.startswith("connector-") and "connector" in opt_args.extra)
+            or (name.startswith("maintainer-") and "maintainer" in opt_args.extra)
+            or (name.startswith("oca-") and "oca" in opt_args.extra)
+            or (name.startswith("odoo-") and "odoo" in opt_args.extra)
+            or (name.startswith("vertical-") and "vertical" in opt_args.extra)
+            or (name in DEVEL_REPS and "devel" in opt_args.extra)
+            or (name.startswith("l10n-") and name in opt_args.l10n)
         ):
             return True
         return False
 
     def default_repositories(opt_args, git_org):
         data = []
-        if git_org == 'odoo':
+        if git_org == "odoo":
             data = [
-                {'url': '//odoo'},
+                {"url": "//odoo"},
             ]
-        elif git_org == 'librerp':
+        elif git_org == "librerp":
             data = [
-                {'url': '//accounting'},
-                {'url': '//custom-addons'},
-                {'url': '//l10n-italy'},
+                {"url": "//accounting"},
+                {"url": "//custom-addons"},
+                {"url": "//l10n-italy"},
             ]
-        elif git_org == 'oca':
+        elif git_org == "oca":
             data = [
-                {'url': '//account-analytic'},
-                {'url': '//account-budgeting'},
-                {'url': '//account-closing'},
-                {'url': '//account-consolidation'},
-                {'url': '//account-financial-reporting'},
-                {'url': '//account-financial-tools'},
-                {'url': '//account-fiscal-rule'},
-                {'url': '//account-invoice-reporting'},
-                {'url': '//account-invoicing'},
-                {'url': '//account-payment'},
-                {'url': '//account-reconcile'},
-                {'url': '//apps-store'},
-                {'url': '//bank-payment'},
-                {'url': '//bank-statement-import'},
-                {'url': '//brand'},
-                {'url': '//business-requirement'},
-                {'url': '//calendar'},
-                {'url': '//commission'},
-                {'url': '//community-data-files'},
-                {'url': '//connector'},
-                {'url': '//connector-ecommerce'},
-                {'url': '//connector-magento'},
-                {'url': '//contract'},
-                {'url': '//credit-control'},
-                {'url': '//crm'},
-                {'url': '//currency'},
-                {'url': '//data-protection'},
-                {'url': '//ddmrp'},
-                {'url': '//delivery-carrier'},
-                {'url': '//dms'},
-                {'url': '//e-commerce'},
-                {'url': '//edi'},
-                {'url': '//geospatial'},
-                {'url': '//helpdesk'},
-                {'url': '//hr'},
-                {'url': '//intrastat-extrastat'},
-                {'url': '//iot'},
-                {'url': '//knowledge'},
-                {'url': '//l10n-italy'},
-                {'url': '//l10n-switzerland'},
-                {'url': '//l10n-usa'},
-                {'url': '//maintainer-quality-tools'},
-                {'url': '//maintainer-tools'},
-                {'url': '//maintenance'},
-                {'url': '//management-system'},
-                {'url': '//manufacture'},
-                {'url': '//manufacture-reporting'},
-                {'url': '//margin-analysis'},
-                {'url': '//mis-builder'},
-                {'url': '//mis-builder-contrib'},
-                {'url': '//mgmtsystem'},
-                {'url': '//multi-company'},
-                {'url': '//OCB'},
-                {'url': '//partner-contact'},
-                {'url': '//pos'},
-                {'url': '//product-attribute'},
-                {'url': '//product-kitting'},
-                {'url': '//product-pack'},
-                {'url': '//product-variant'},
-                {'url': '//project'},
-                {'url': '//project-agile'},
-                {'url': '//project-reporting'},
-                {'url': '//purchase-reporting'},
-                {'url': '//purchase-workflow'},
-                {'url': '//queue'},
-                {'url': '//reporting-engine'},
-                {'url': '//report-print-send'},
-                {'url': '//rma'},
-                {'url': '//sale-financial'},
-                {'url': '//sale-reporting'},
-                {'url': '//sale-workflow'},
-                {'url': '//search-engine'},
-                {'url': '//server-auth'},
-                {'url': '//server-backend'},
-                {'url': '//server-brand'},
-                {'url': '//server-env'},
-                {'url': '//server-tools'},
-                {'url': '//server-ux'},
-                {'url': '//social'},
-                {'url': '//stock-logistics-barcode'},
-                {'url': '//stock-logistics-reporting'},
-                {'url': '//stock-logistics-tracking'},
-                {'url': '//stock-logistics-transport'},
-                {'url': '//stock-logistics-warehouse'},
-                {'url': '//stock-logistics-workflow'},
-                {'url': '//storage'},
-                {'url': '//timesheet'},
-                {'url': '//vertical-association'},
-                {'url': '//vertical-hotel'},
-                {'url': '//vertical-isp'},
-                {'url': '//web'},
-                {'url': '//webhook'},
-                {'url': '//webkit-tools'},
-                {'url': '//website'},
-                {'url': '//website-cms'},
-                {'url': '//wms'},
+                {"url": "//account-analytic"},
+                {"url": "//account-budgeting"},
+                {"url": "//account-closing"},
+                {"url": "//account-consolidation"},
+                {"url": "//account-financial-reporting"},
+                {"url": "//account-financial-tools"},
+                {"url": "//account-fiscal-rule"},
+                {"url": "//account-invoice-reporting"},
+                {"url": "//account-invoicing"},
+                {"url": "//account-payment"},
+                {"url": "//account-reconcile"},
+                {"url": "//apps-store"},
+                {"url": "//bank-payment"},
+                {"url": "//bank-statement-import"},
+                {"url": "//brand"},
+                {"url": "//business-requirement"},
+                {"url": "//calendar"},
+                {"url": "//commission"},
+                {"url": "//community-data-files"},
+                {"url": "//connector"},
+                {"url": "//connector-ecommerce"},
+                {"url": "//connector-magento"},
+                {"url": "//contract"},
+                {"url": "//credit-control"},
+                {"url": "//crm"},
+                {"url": "//currency"},
+                {"url": "//data-protection"},
+                {"url": "//ddmrp"},
+                {"url": "//delivery-carrier"},
+                {"url": "//dms"},
+                {"url": "//e-commerce"},
+                {"url": "//edi"},
+                {"url": "//geospatial"},
+                {"url": "//helpdesk"},
+                {"url": "//hr"},
+                {"url": "//intrastat-extrastat"},
+                {"url": "//iot"},
+                {"url": "//knowledge"},
+                {"url": "//l10n-italy"},
+                {"url": "//l10n-switzerland"},
+                {"url": "//l10n-usa"},
+                {"url": "//maintainer-quality-tools"},
+                {"url": "//maintainer-tools"},
+                {"url": "//maintenance"},
+                {"url": "//management-system"},
+                {"url": "//manufacture"},
+                {"url": "//manufacture-reporting"},
+                {"url": "//margin-analysis"},
+                {"url": "//mis-builder"},
+                {"url": "//mis-builder-contrib"},
+                {"url": "//mgmtsystem"},
+                {"url": "//multi-company"},
+                {"url": "//OCB"},
+                {"url": "//partner-contact"},
+                {"url": "//pos"},
+                {"url": "//product-attribute"},
+                {"url": "//product-kitting"},
+                {"url": "//product-pack"},
+                {"url": "//product-variant"},
+                {"url": "//project"},
+                {"url": "//project-agile"},
+                {"url": "//project-reporting"},
+                {"url": "//purchase-reporting"},
+                {"url": "//purchase-workflow"},
+                {"url": "//queue"},
+                {"url": "//reporting-engine"},
+                {"url": "//report-print-send"},
+                {"url": "//rma"},
+                {"url": "//sale-financial"},
+                {"url": "//sale-reporting"},
+                {"url": "//sale-workflow"},
+                {"url": "//search-engine"},
+                {"url": "//server-auth"},
+                {"url": "//server-backend"},
+                {"url": "//server-brand"},
+                {"url": "//server-env"},
+                {"url": "//server-tools"},
+                {"url": "//server-ux"},
+                {"url": "//social"},
+                {"url": "//stock-logistics-barcode"},
+                {"url": "//stock-logistics-reporting"},
+                {"url": "//stock-logistics-tracking"},
+                {"url": "//stock-logistics-transport"},
+                {"url": "//stock-logistics-warehouse"},
+                {"url": "//stock-logistics-workflow"},
+                {"url": "//storage"},
+                {"url": "//timesheet"},
+                {"url": "//vertical-association"},
+                {"url": "//vertical-hotel"},
+                {"url": "//vertical-isp"},
+                {"url": "//web"},
+                {"url": "//webhook"},
+                {"url": "//webkit-tools"},
+                {"url": "//website"},
+                {"url": "//website-cms"},
+                {"url": "//wms"},
             ]
-        elif git_org == 'zeroincombenze':
+        elif git_org == "zeroincombenze":
             data = [
-                {'url': '//account-closing'},
-                {'url': '//account-financial-reporting'},
-                {'url': '//account-financial-tools'},
-                {'url': '//account-invoicing'},
-                {'url': '//account-payment'},
-                {'url': '//bank-payment'},
-                {'url': '//commission'},
-                {'url': '//connector'},
-                {'url': '//contract'},
-                {'url': '//crm'},
-                {'url': '//grymb'},
-                {'url': '//knowledge'},
-                {'url': '//l10n-italy'},
-                {'url': '//l10n-italy-supplemental'},
-                {'url': '//management-system'},
-                {'url': '//OCB'},
-                {'url': '//Odoo-samples'},
-                {'url': '//partner-contact'},
-                {'url': '//product-attribute'},
-                {'url': '//profiles'},
-                {'url': '//project'},
-                {'url': '//purchase-workflow'},
-                {'url': '//report-print-send'},
-                {'url': '//reporting-engine'},
-                {'url': '//sale-workflow'},
-                {'url': '//server-ux'},
-                {'url': '//stock-logistics-barcode'},
-                {'url': '//stock-logistics-tracking'},
-                {'url': '//stock-logistics-workflow'},
-                {'url': '//tools'},
-                {'url': '//uncovered'},
-                {'url': '//VME'},
-                {'url': '//zerobug'},
-                {'url': '//zerobug-test'},
-                {'url': '//zeroincombenze'},
+                {"url": "//account-closing"},
+                {"url": "//account-financial-reporting"},
+                {"url": "//account-financial-tools"},
+                {"url": "//account-invoicing"},
+                {"url": "//account-payment"},
+                {"url": "//bank-payment"},
+                {"url": "//commission"},
+                {"url": "//connector"},
+                {"url": "//contract"},
+                {"url": "//crm"},
+                {"url": "//grymb"},
+                {"url": "//knowledge"},
+                {"url": "//l10n-italy"},
+                {"url": "//l10n-italy-supplemental"},
+                {"url": "//management-system"},
+                {"url": "//OCB"},
+                {"url": "//Odoo-samples"},
+                {"url": "//partner-contact"},
+                {"url": "//product-attribute"},
+                {"url": "//profiles"},
+                {"url": "//project"},
+                {"url": "//purchase-workflow"},
+                {"url": "//report-print-send"},
+                {"url": "//reporting-engine"},
+                {"url": "//sale-workflow"},
+                {"url": "//server-ux"},
+                {"url": "//stock-logistics-barcode"},
+                {"url": "//stock-logistics-tracking"},
+                {"url": "//stock-logistics-workflow"},
+                {"url": "//tools"},
+                {"url": "//uncovered"},
+                {"url": "//VME"},
+                {"url": "//zerobug"},
+                {"url": "//zerobug-test"},
+                {"url": "//zeroincombenze"},
             ]
-            if opt_args.odoo_vid == '7.0':
-                data.append({'url': '//account_banking_cscs'})
-                data.append({'url': '//cscs_addons'})
+            if opt_args.odoo_vid == "7.0":
+                data.append({"url": "//account_banking_cscs"})
+                data.append({"url": "//cscs_addons"})
         return data
 
     def add_repo(name):
         if opt_args.verbose:
             print(name)
         repositories.append(name)
 
     fn = os.path.join(
-        os.path.dirname(__file__), '.%s.dat' % os.path.splitext(
-            os.path.basename(__file__))[0]
+        os.path.dirname(__file__),
+        ".%s.dat" % os.path.splitext(os.path.basename(__file__))[0],
     )
     cache = {}
     if os.path.isfile(fn):
-        with open(fn, 'r') as fd:
+        with open(fn, "r") as fd:
             cache = eval(fd.read())
-    baseurl = 'https://api.github.com/users/%s/repos' % git_org
-    branchurl = 'https://api.github.com/repos/%s' % git_org
+    baseurl = "https://api.github.com/users/%s/repos" % git_org
+    branchurl = "https://api.github.com/repos/%s" % git_org
     done_default = False
     page = 0
     repositories = []
     while 1:
         page += 1
-        pageurl = '%s?q=addClass+user:mozilla&page=%d' % (baseurl, page)
+        pageurl = "%s?q=addClass+user:mozilla&page=%d" % (baseurl, page)
         if opt_args.verbose:
-            print('Acquire data from github.com (page=%d)...' % page)
+            print("Acquire data from github.com (page=%d)..." % page)
         if opt_args.dry_run:
             data = [TEST_REP_OCB, TEST_REP_ACC_CLO, TEST_REP_L10N_IT]
             if page > 1:
                 data = []
         elif opt_args.def_repo:
             data = []
             if not done_default:
                 data = default_repositories(opt_args, git_org)
                 done_default = True
         else:
             try:
                 response = urlopen(pageurl)
                 data = json.loads(response.read())
             except BaseException:
-                if (not repositories and
-                        git_org in cache and
-                        opt_args.odoo_vid in cache[git_org]):
+                if (
+                    not repositories
+                    and git_org in cache
+                    and opt_args.odoo_vid in cache[git_org]
+                ):
                     break
                 data = []
                 if not done_default:
                     data = default_repositories(opt_args, git_org)
                     done_default = True
         if not data:
             break
         if opt_args.verbose:
-            print('Analyzing received data ...')
+            print("Analyzing received data ...")
         for repos in data:
-            name = os.path.basename(repos['url'])
+            name = os.path.basename(repos["url"])
             if name_is_valid(opt_args, name):
                 if opt_args.odoo_vid:
-                    pageurl = '%s/%s/branches' % (branchurl, name)
+                    pageurl = "%s/%s/branches" % (branchurl, name)
                     try:
                         branch_response = urlopen(pageurl)
                         branches = json.loads(branch_response.read())
                     except BaseException:
                         branches = [
-                            {'name': '6.1'},
-                            {'name': '7.0'},
-                            {'name': '8.0'},
-                            {'name': '9.0'},
-                            {'name': '10.0'},
-                            {'name': '11.0'},
-                            {'name': '12.0'},
-                            {'name': '13.0'},
-                            {'name': '14.0'},
-                            {'name': '15.0'},
-                            {'name': '16.0'},
+                            {"name": "6.1"},
+                            {"name": "7.0"},
+                            {"name": "8.0"},
+                            {"name": "9.0"},
+                            {"name": "10.0"},
+                            {"name": "11.0"},
+                            {"name": "12.0"},
+                            {"name": "13.0"},
+                            {"name": "14.0"},
+                            {"name": "15.0"},
+                            {"name": "16.0"},
                         ]
                     if not branches or not any(
-                        [x for x in branches if x['name'] == opt_args.odoo_vid]
+                        [x for x in branches if x["name"] == opt_args.odoo_vid]
                     ):
                         continue
                 add_repo(name)
             elif opt_args.verbose:
-                print('discarded %s' % name)
+                print("discarded %s" % name)
 
     if repositories:
         cache[git_org] = cache.get(git_org, {})
         cache[git_org][opt_args.odoo_vid] = repositories
-        with open(fn, 'w') as fd:
+        with open(fn, "w") as fd:
             fd.write(str(cache))
     elif git_org in cache and opt_args.odoo_vid in cache[git_org]:
         repositories = cache[git_org][opt_args.odoo_vid]
     return repositories
 
 
 def main(cli_args=None):
     cli_args = cli_args or sys.argv[1:]
     parser = argparse.ArgumentParser(
         description="Get repository list from github",
         epilog="© 2019-2023 by SHS-AV s.r.l.",
     )
     parser.add_argument(
-        '-b',
-        '--odoo-branch',
+        "-b",
+        "--odoo-branch",
         help="may be one of 6.1 7.0 8.0 9.0 10.0 11.0 12.0 13.0 14.0 15.0 or 16.0",
-        action='store',
-        dest='odoo_vid',
+        action="store",
+        dest="odoo_vid",
     )
     parser.add_argument(
-        '-D', '--default', help="Default repositories", action='store_true',
-        dest='def_repo'
+        "-D",
+        "--default",
+        help="Default repositories",
+        action="store_true",
+        dest="def_repo",
     )
     parser.add_argument(
-        '-G', '--git-org', help="select repository", action='store', dest='git_org'
+        "-G", "--git-org", help="select repository", action="store", dest="git_org"
     )
     parser.add_argument(
-        '-l',
-        '--local-reps',
+        "-l",
+        "--local-reps",
         help="select local repositories",
-        action='store',
-        dest='l10n',
+        action="store",
+        dest="l10n",
     )
-    parser.add_argument('-n', '--dry-run', action='store_true')
+    parser.add_argument("-n", "--dry-run", action="store_true")
     parser.add_argument(
-        '-O', '--oca', help="repository OCA", action='store_true', dest='oca'
+        "-O", "--oca", help="repository OCA", action="store_true", dest="oca"
     )
     # parser.add_argument('-q')
+    parser.add_argument("-v", "--verbose", action="count", default=0)
+    parser.add_argument("-V", "--version", action="version", version=__version__)
     parser.add_argument(
-        '-v', '--verbose', action='count', default=0)
-    parser.add_argument('-V', '--version', action="version", version=__version__)
-    parser.add_argument(
-        '-x',
-        '--extra-reps',
+        "-x",
+        "--extra-reps",
         help="may be: all,none,connector,devel,maintainer,oca,odoo,vertical",
-        action='store',
-        dest='extra',
+        action="store",
+        dest="extra",
     )
     parser.add_argument(
-        '-Z',
-        '--zeroincombenze',
+        "-Z",
+        "--zeroincombenze",
         help="repository zeroincombenze",
-        action='store_true',
-        dest='zero',
+        action="store_true",
+        dest="zero",
     )
-    parser.add_argument('--return-repos', action='store_true')
+    parser.add_argument("--return-repos", action="store_true")
     opt_args = parser.parse_args(cli_args)
 
     git_orgs = []
     repositories = []
     if opt_args.git_org:
         git_orgs = []
-        for x in opt_args.git_org.split(','):
-            x = x if x != 'zero' else 'zeroincombenze'
-            x = x if x != 'OCA' else 'oca'
+        for x in opt_args.git_org.split(","):
+            x = x if x != "zero" else "zeroincombenze"
+            x = x if x != "OCA" else "oca"
             git_orgs.append(x)
     else:
         if opt_args.zero:
-            git_orgs.append('zeroincombenze')
+            git_orgs.append("zeroincombenze")
         if opt_args.oca:
-            git_orgs.append('oca')
+            git_orgs.append("oca")
     if not opt_args.l10n:
-        opt_args.l10n = 'l10n-italy,l10n-italy-supplemental'
-    opt_args.l10n = opt_args.l10n.split(',')
+        opt_args.l10n = "l10n-italy,l10n-italy-supplemental"
+    opt_args.l10n = opt_args.l10n.split(",")
     if not opt_args.extra:
-        opt_args.extra = 'none'
+        opt_args.extra = "none"
     elif opt_args.extra == "all":
-        opt_args.extra = 'connector,maintainer,oca,odoo,vertical,devel'
-    opt_args.extra = opt_args.extra.split(',')
+        opt_args.extra = "connector,maintainer,oca,odoo,vertical,devel"
+    opt_args.extra = opt_args.extra.split(",")
     for git_org in git_orgs:
         repository = get_list_from_url(opt_args, git_org)
         repositories = list(set(repositories) | set(repository))
     if opt_args.return_repos:
         return repositories
-    print('Found %d repositories of %s' % (len(repositories), git_orgs))
-    print('\t' + ' '.join(sorted(repositories)))
+    print("Found %d repositories of %s" % (len(repositories), git_orgs))
+    print("\t" + " ".join(sorted(repositories)))
     return 0
 
 
 if __name__ == "__main__":
     exit(main())
```

### Comparing `wok_code-2.0.8/wok_code/scripts/config/to_new_api.yml` & `wok_code-2.0.9/wok_code/scripts/config/to_new_api.yml`

 * *Files identical despite different names*

### Comparing `wok_code-2.0.8/wok_code/scripts/config/to_old_api.yml` & `wok_code-2.0.9/wok_code/scripts/config/to_old_api.yml`

 * *Files identical despite different names*

### Comparing `wok_code-2.0.8/wok_code/scripts/please_apache.py` & `wok_code-2.0.9/wok_code/scripts/please_apache.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 try:
     import ConfigParser
 except ImportError:
     import configparser as ConfigParser
 
 
-__version__ = "2.0.8"
+__version__ = "2.0.9"
 
 APACHE_TEMPLATE = """##################################################################
 # Odoo service %(odoo_branch)s
 # Domain: <%(protocol)s://%(domain)s>
 #
 <VirtualHost *:%(apache_port)s>
     ServerAdmin %(email)s
@@ -52,88 +52,94 @@
     SSLCertificateKeyFile %(SSLCertificateKeyFile)s
     Include /etc/letsencrypt/options-ssl-apache.conf
     # SSLCertificateChainFile
 """
 
 
 class PleaseApache(object):
+    """NAME
+        create apache configuration file
+
+    SYNOPSIS
+        please create apache URL
+
+    DESCRIPTION
+        This command creates the apache configuration file for URL Odoo website.
+        The configuration file may be deployed on /etc/apache2/site-available path
+        or in equivalent path, i.e. /etc/httpd/conf
+
+    OPTIONS
+      %(options)s
+
+    EXAMPLES
+        please create apache odoo.example.com
+
+    BUGS
+        No known bugs.
+
+    SEE ALSO
+        Full documentation at: <https://zeroincombenze-tools.readthedocs.io/>
+    """
+
     def __init__(self, please):
         self.please = please
 
-    def get_actions(self):
-        return ["create"]
-
-    def action_opts(self, parser):
-        parser.add_argument(
-            "-o",
-            "--out-file",
-        )
+    def action_opts(self, parser, for_help=False):
+        self.please.add_argument(parser, "-b")
+        self.please.add_argument(parser, "-c")
+        self.please.add_argument(parser, "-l")
+        if not for_help:
+            self.please.add_argument(parser, "-n")
+        parser.add_argument("-o", "--out-file")
         parser.add_argument(
             "-P",
             "--protocol",
             help="http or https",
             default="http",
         )
         parser.add_argument(
             "-p",
             "--http-port",
-            help="http port (default 8069)",
+            help="http port (default from config file or 8069)",
         )
-        parser.add_argument("-L", "--long-port", help="logn port (default 8070)")
+        parser.add_argument(
+            "-L",
+            "--long-port",
+            help="long polling port(default from config file or 8070)",
+        )
+        if not for_help:
+            self.please.add_argument(parser, "-q")
         parser.add_argument(
             "-S",
             "--https-proxy",
             action="store_true",
             help="add https proxy statements",
         )
+        if not for_help:
+            self.please.add_argument(parser, "-v")
         parser.add_argument(
             "-x",
             "--xmlrpc-port",
-            help="xmlrpc port (default 8069)",
+            help="xmlrpc port (default from config file or 8069)",
         )
+        parser.add_argument("args", nargs="*")
         return parser
 
-    def do_action(self):
-        """
-        NAME
-            create apache configuration
-
-        SYNOPSIS
-            please create apache URL
-
-        DESCRIPTION
-            This command creates the apache configuration file for URL Odoo website.
-            The configuration file may be deployed on /etc/apache2/site-available path
-            or in equivalent path, i.e. /etc/httpd/conf
-
-        OPTIONS
-            -c      Odoo configuration file to URL
-            -l      Apache logs path: may be "logs" or ${APACHE_LOG_DIR}
-            -n      Do nothing (dry-run)
-            -P      Website protocol: may be "http" or "https"
-            -p      Odoo http port (default 8069)
-            -S      Add https proxy redirect statements
-            -x      Odoo xmlrpc port (default 8069, Odoo 10.0-)
-
-        EXAMPLES
-            please create apache odoo.example.com
-
-        BUGS
-            No known bugs."""
+    def do_create(self):
         please = self.please
         odoo_confn = please.opt_args.odoo_config
         if odoo_confn:
             params = self._get_params_from_csv(
                 odoo_confn, odoo_branch=please.opt_args.odoo_branch
             )
         else:
             params = self.default_config(please.opt_args.odoo_branch)
         params["odoo_branch"] = please.opt_args.odoo_branch
-        if please.opt_args.sub1:
-            params["domain"] = please.opt_args.sub1
+        if please.opt_args.args[0]:
+            params["domain"] = please.opt_args.args[0]
         else:
             params["domain"] = "zeroincombenze.it"
         params["domain_2L"] = ".".join(params["domain"].split(".")[-2:])
         params["email"] = "postmaster@%s" % params["domain_2L"]
         if please.opt_args.log:
             params["logs"] = please.opt_args.log
         else:
@@ -155,16 +161,15 @@
             params["http_proxy_block"] = ""
         if params["protocol"] == "https":
             params["https_block"] = APACHE_HTTPS_BLOCK % params
         else:
             params["https_block"] = ""
         content = APACHE_TEMPLATE % params
         out_file = (
-            please.opt_args.out_file
-            or ("~/%s-le-ssl.conf" % params["domain"])
+            please.opt_args.out_file or ("~/%s-le-ssl.conf" % params["domain"])
             if params["protocol"] == "https"
             else "~/%s.conf" % params["domain"]
         )
         if please.opt_args.dry_run:
             if please.opt_args.verbose:
                 print(content)
             print("File %s will be created" % out_file)
```

### Comparing `wok_code-2.0.8/wok_code/scripts/dist_pkg.py` & `wok_code-2.0.9/wok_code/scripts/dist_pkg.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,33 +3,33 @@
 import os
 import sys
 
 
 def main(cli_args=None):
     if not cli_args:
         cli_args = sys.argv[1:]
-    cmd = '%s.sh' % os.path.splitext(os.path.abspath(__file__))[0]
+    cmd = "%s.sh" % os.path.splitext(os.path.abspath(__file__))[0]
     if not os.path.isfile(cmd):
         cmd = os.path.split(cmd)
         cmd = os.path.join(os.path.dirname(cmd[0]), cmd[1])
     if not os.path.isfile(cmd):
-        print('Internal package error: file %s not found!' % cmd)
+        print("Internal package error: file %s not found!" % cmd)
     for arg in cli_args:
-        if '<' in arg or '>' in arg:
+        if "<" in arg or ">" in arg:
             arg = "'%s'" % arg.replace("'", r"\'")
-        elif ' ' in arg:
+        elif " " in arg:
             if '"' in arg:
-                arg = '"%s"' % arg.replace('"', r'\"')
+                arg = '"%s"' % arg.replace('"', r"\"")
             else:
                 arg = '"%s"' % arg
         elif '"' in arg:
-            arg = '"%s"' % arg.replace('"', r'\"')
+            arg = '"%s"' % arg.replace('"', r"\"")
         elif "'" in arg:
             arg = '"%s"' % arg
         else:
-            arg = '%s' % arg
-        cmd = '%s %s' % (cmd, arg)
+            arg = "%s" % arg
+        cmd = "%s %s" % (cmd, arg)
     return os.system(cmd)
 
 
 if __name__ == "__main__":
     exit(main())
```

### Comparing `wok_code-2.0.8/wok_code/scripts/do_migrate.py` & `wok_code-2.0.9/wok_code/scripts/arcangelo.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 from past.builtins import basestring
 import sys
 import os
+from datetime import datetime
 import argparse
 import re
 import lxml.etree as ET
 import yaml
 from python_plus import _b
 from z0lib import z0lib
 
-__version__ = "2.0.8"
+__version__ = "2.0.9"
 
 # RULES: every rule is list has the following format:
 # EREGEX, (ACTION, PARAMETERS), ...
 # where
 # - EREGEX is an enhanced regular expression to apply the rule.
 # - ACTION is the action to apply on current line
 # - PARAMETERS are the values to supply on action
@@ -22,22 +23,22 @@
 #
 # EREGEX
 # EREGEX is an enhanced regular expression; the format are
 # - REGEX is a python re: current line is processed if it matches REGEX
 # - !REGEX is a python re: current line is processes if it does not match REGEX
 #   If you will match "!" (exclamation point) user escape char "\": i.e. "\!match"
 #   Escape before "!" is needed just at the beginning of the REGEX
-# - !(RE)REGEX are two python re; if current line matches (BY search) the RE, rule is
-#   skipped otherwise current line is processed if IT matches REGEX; i.e:  !pkg^import
+# - !(RE)REGEX are two python re; if current line matches (by search) the RE, rule is
+#   skipped otherwise current line is processed if it matches REGEX; i.e:  !pkg^import
 #   Rule is applied on every line beginning with "import" but not on "import pkg"
 # - {{EXPR}}EREGEX is double expression; EREGEX is validated if pythonic EXPR is true
 #   Some test are useful, like:
 #   * self.to_major_version -> to process rule against specific Odoo major version
 #   * self.from_major_version -> to process rule against source Odoo major version
-#   * self.python_version -> to proces rule against python version
+#   * self.pythonsion -> to proces rule against python version
 #   * self.py23 -> to proces rule against python major version
 # ACTION is the action will be executed: it can be prefixed by some simple expression
 # if action begins with "/" (slash) it will be executed if EREGEX fails
 # usually ACTION is executed when EREGEX is True
 # i.e. ("s", "a", "b"), ("/d") -> If EREGEX, replace "a" with "b" else delete line
 # ACTION can submitted to Odoo or python version:
 # +[0-9] means from Odoo/python version
@@ -52,112 +53,36 @@
 #   - The 1.st item is the EREGEX to search for replace (negate is not applied)
 #   - The 2.nd item is the text to replace which can contain macros like %(classname)s
 # - "d": delete line; stop immediately rule processing and re-read the line
 # - "$": execute FUNCTION
 #        All functions must have the format:    def my_fun(self, nro)
 #                                                   [...]
 #                                                   return do_break, offset
-#        Function may ask for break: this means no other rules will be processed.
+#        Function may requires break: this means no other rules will be processed.
 #        Function returns the offset for next line: the value 0 means read next line,
 #        the value -1 re-read the current line, +1 skip next line, and so on
 # - "=": execute python code
 #
-_RULES_GLOBALS = [
-    (
-        r"^# -\*- coding: utf-8 -\*-",
-        ("$", "matches_utf8"),
-    ),
-    (
-        "^# (flake8|pylint):",
-        ("$", "matches_lint"),
-    ),
-    (
-        "!(coding|flake8|pylint|python)^#",
-        ("$", "matches_no_lint"),
-    ),
-    (
-        "!^#",
-        ("$", "matches_no_lint"),
-    ),
-    (
-        r"^ *class [^(]+\(",
-        ("$", "matches_class"),
-    ),
-    (
-        r"^# -\*- encoding: utf-8 -\*-",
-        ("d",),
-    ),
-]
-_RULES_GLOBALS_XML = [
-]
-_RULES_TO_NEW_API = [
-    (
-        "^from openerp.osv import",
-        ("s", "from openerp.osv import", "from odoo import"),
-        ("s", "orm", "models"),
-    ),
-    (
-        r"^ *class [^(]+\([^)]*\)",
-        ("s", "orm.Model", "models.Model"),
-        ("s", "osv.osv_memory", "models.TransientModel"),
-    ),
-    (
-        r"^ *def [^(]+\(self, *cr, *uid, [^)]*\)",
-        ("s", r"\(self, *cr, *uid,", "(self,"),
-        ("s", r", *context=[^)]+", ""),
-    ),
-    ("^from openerp", ("s", "openerp", "odoo")),
-    ("!(import).*osv.except_osv", ("s", "osv.except_osv", "UserError")),
-]
-_RULES_TO_OLD_API = [
-    (
-        "^from odoo import",
-        ("s", "models", "orm"),
-        ("s", "odoo", "openerp.osv"),
-        ("s", "models.TransientModel", "osv.osv_memory"),
-    ),
-    (
-        r"^ *class [^(]+\([^)]*\)",
-        ("s", "models.Model", "orm.Model"),
-    ),
-    (
-        r"^ *def [^(]+\(self, [^)]*\)",
-        ("s", r"\(self,", "(self, cr, uid,"),
-        ("s", r"\)", ", context=None)"),
-    ),
-    (
-        "^from odoo.exceptions import UserError",
-        ("s", "import UserError", "import Warning as UserError"),
-    ),
-    ("^from odoo", ("s", "odoo", "openerp")),
-    (
-        "from odoo.exceptions import UserError",
-        (
-            "s",
-            "from odoo.exceptions import UserError",
-            "from openerp.osv.osv import except_osv"
-        ),
-    ),
-]
-_RULES_TO_ODOO_PY3 = [
-    (
-        r"^ *super\([^)]*\)",
-        ("s", r"super\([^)]*\)", "super()"),
-        ("s", r"\(cr, *uid, *", "("),
-        ("s", r", *context=[^)]+", ""),
-    ),
-]
-_RULES_TO_ODOO_PY2 = [
-    (
-        r"^ *super\([^)]*\)",
-        ("s", r"super\(\)", "super(%(classname)s, self)"),
-        ("-8s", r"(\)\.[^(]+)\(", r"\1(cr, uid, "),
-        ("-8s", r"(super[^)]+\)[^)]+)", r"\1, context=context"),
-    ),
-]
+
+# _RULES_TO_ODOO_PY3 = [
+#     (
+#         r"^ *super\([^)]*\)",
+#         ("s", r"super\([^)]*\)", "super()"),
+#         ("s", r"\(cr, *uid, *", "("),
+#         ("s", r", *context=[^)]+", ""),
+#     ),
+# ]
+# _RULES_TO_ODOO_PY2 = [
+#     (
+#         r"^ *super\([^)]*\)",
+#         ("s", r"super\(\)", "super(%(classname)s, self)"),
+#         ("-8s", r"(\)\.[^(]+)\(", r"\1(cr, uid, "),
+#         ("-8s", r"(super[^)]+\)[^)]+)", r"\1, context=context"),
+#     ),
+# ]
 RULES_TO_XML_NEW = [
     (
         "^ *<openerp",
         ("$", "matches_openerp_tag"),
     ),
     (
         "^ *</openerp>",
@@ -202,60 +127,84 @@
         ("$", "matches_data_tag"),
     ),
     (
         "^ *</data>",
         ("$", "matches_data_endtag"),
     ),
 ]
-RULES_TO_PYPI_PY3 = [
-    (
-        r"^ *super\([^)]*\)",
-        ("s", r"super\([^)]*\)", "super()"),
-    ),
-]
-RULES_TO_PYPI_PY2 = [
-    (
-        r"^ *super\(\)",
-        ("s", r"super\(\)", "super(%(classname)s, self)"),
-    ),
-]
-RULES_TO_PYPI_FUTURE = [
-    (
-        r"^ *super\(\)",
-        ("s", r"super\(\)", "super(%(classname)s, self)"),
-    ),
-]
+# RULES_TO_PYPI_PY3 = [
+#     (
+#         r"^ *super\([^)]*\)",
+#         ("s", r"super\([^)]*\)", "super()"),
+#     ),
+# ]
+# RULES_TO_PYPI_PY2 = [
+#     (
+#         r"^ *super\(\)",
+#         ("s", r"super\(\)", "super(%(classname)s, self)"),
+#     ),
+# ]
+# RULES_TO_PYPI_FUTURE = [
+#     (
+#         r"^ *super\(\)",
+#         ("s", r"super\(\)", "super(%(classname)s, self)"),
+#     ),
+# ]
 
 
 class MigrateFile(object):
-
     def __init__(self, ffn, opt_args):
         self.sts = 0
         if opt_args.verbose > 0:
             print("Reading %s ..." % ffn)
         self.ffn = ffn
         self.is_xml = ffn.endswith(".xml")
         if opt_args.from_version:
             self.from_major_version = int(opt_args.from_version.split('.')[0])
         else:
             self.from_major_version = 0
+        self.def_python_future = False
+        if not opt_args.to_version or opt_args.to_version == "0.0":
+            branch = ""
+            sts, stdout, stderr = z0lib.run_traced(
+                "git branch", verbose=False, dry_run=False
+            )
+            if sts == 0 and stdout:
+                sts = 1
+                for ln in stdout.split("\n"):
+                    if ln.startswith("*"):
+                        branch = ln[2:]
+                        sts = 0
+                        break
+            if sts == 0:
+                x = re.match(r"[0-9]+\.[0-9]+", branch)
+                if not x:
+                    sts = 1
+            if sts == 0:
+                branch = branch[x.start(): x.end()]
+                opt_args.to_version = branch
+            else:
+                opt_args.to_version = "12.0"
         self.to_major_version = int(opt_args.to_version.split('.')[0])
         if not opt_args.pypi_package:
             if self.to_major_version <= 10:
-                opt_args.python_ver = "2.7"
+                opt_args.python = "2.7"
+                self.def_python_future = True
             elif self.to_major_version <= 14:
-                opt_args.python_ver = "3.7"
+                opt_args.python = "3.7"
             else:
-                opt_args.python_ver = "3.8"
-        if opt_args.python_ver:
-            self.python_version = opt_args.python_ver
-            self.py23 = int(opt_args.python_ver.split(".")[0])
+                opt_args.python = "3.8"
+        if opt_args.python:
+            self.python_version = opt_args.python
+            self.py23 = int(opt_args.python.split(".")[0])
         else:
             self.python_version = "3.7"
             self.py23 = 3
+            if opt_args.pypi_package:
+                self.def_python_future = True
         self.opt_args = opt_args
         self.lines = []
         with open(ffn, 'r') as fd:
             self.source = fd.read()
         self.lines = self.source.split('\n')
         self.analyze_source()
 
@@ -269,39 +218,51 @@
             x = re.match(regex, line)
         except BaseException as e:
             self.raise_error("Invalid regex: match('%s','%s') -> %s" % (regex, line, e))
             x = None
         return x
 
     def analyze_source(self):
-        self.python_future = False
-        if "from __future__ import" in self.source:
-            self.python_future = True
+        self.python_future = self.def_python_future
         self.ignore_file = False
-        if (
-            not self.opt_args.force
-            and ("# flake8: noqa" in self.source
-                 or "# pylint: skip-file" in self.source)
+        for ln in self.lines:
+            if not ln:
+                continue
+            if not ln.startswith("#"):
+                break
+            if "from __future__ import" in ln or "from past.builtins import " in ln:
+                self.python_future = True
+            if not self.opt_args.force and (
+                "# flake8: noqa" in ln or "# pylint: skip-file" in ln
+            ):
+                self.ignore_file = True
+        if not self.opt_args.force and (
+            os.path.basename(self.ffn) in ("testenv.py", "conf.py", "_check4deps_.py")
+            or "/tests/data/" in os.path.abspath(self.ffn)
         ):
             self.ignore_file = True
-        elif not self.opt_args.force and os.path.basename(self.ffn) == "testenv.py":
-            self.ignore_file = True
 
     def get_noupdate_property(self, nro):
         if "noupdate" in self.lines[nro]:
             x = re.search("noupdate *=\"[01]\"", self.lines[nro])
-            return self.lines[nro][x.start():x.end()]
+            return self.lines[nro][x.start(): x.end()]
         return ""
 
+    def matches_ignore(self, nro):
+        return True, 0
+
     def matches_class(self, nro):
         x = self.re_match(r"^ *class [^(]+", self.lines[nro])
         self.classname = self.lines[nro][x.start() + 6: x.end()].strip()
         return False, 0
 
-    def matches_odoo_tag(self, nro,):
+    def matches_odoo_tag(
+        self,
+        nro,
+    ):
         if self.to_major_version < 8 and self.ctr_tag_openerp == 0:
             property_noupdate = self.get_noupdate_property(nro)
             if property_noupdate:
                 self.lines.insert(nro + 1, "    <data %s>" % property_noupdate)
             else:
                 self.lines.insert(nro + 1, "    <data>")
             self.lines[nro] = "<openerp>"
@@ -365,106 +326,95 @@
         else:
             self.ctr_tag_odoo -= 1
         return True, offset
 
     def matches_utf8(self, nro):
         offset = 0
         if (
-            self.opt_args.python_ver
-            and self.py23 == 2 or self.python_future
+            (self.python_future
+             or self.opt_args.ignore_pragma
+             or (self.opt_args.python and self.py23 == 2))
             and self.utf8_decl_nro < 0
         ):
             self.utf8_decl_nro = nro
         else:
             del self.lines[nro]
             offset = -1
         return False, offset
 
+    def matches_end_utf8(self, nro):
+        offset = 0
+        if self.utf8_decl_nro < 0 and (self.py23 == 2 or self.python_future):
+            if not self.opt_args.ignore_pragma:
+                self.lines.insert(nro, "# -*- coding: utf-8 -*-")
+                self.utf8_decl_nro = nro
+        return False, offset
+
     def matches_lint(self, nro):
         offset = 0
         if self.utf8_decl_nro >= 0:
             del self.lines[self.utf8_decl_nro]
             self.utf8_decl_nro = -1
             offset = -1
         return False, offset
 
-    def matches_no_lint(self, nro):
-        offset = 0
-        if (
-            not self.utf8_decl_nro >= 0
-            and self.py23 == 2
-        ):
-            self.lines.insert(nro, "# -*- coding: utf-8 -*-")
-            self.utf8_decl_nro = nro
-        return False, offset
-
     def comparable_version(self, version):
-        return ".".join(
-            [
-                "%03d" % int(x)
-                for x in version.split(".")
-            ]
-        )
+        return ".".join(["%03d" % int(x) for x in version.split(".")])
 
     def update_line(self, nro, items, regex):
         action = items[0]
         params = items[1:] if len(items) > 1 else []
         if action.startswith("/"):
             not_expr = True
             action = action[1:]
         else:
             not_expr = False
             action = action
-        if (
-            (not_expr and regex)
-            or (not not_expr and not regex)
-        ):
+        if (not_expr and regex) or (not not_expr and not regex):
             return False, 0
         if action.startswith("+"):
             x = self.re_match(r"\+[0-9]+\.[0-9]", action)
             if x:
-                ver = action[x.start():x.end()]
-                if (
-                    self.comparable_version(self.opt_args.python_ver)
-                    < self.comparable_version(ver)
-                ):
+                ver = action[x.start(): x.end()]
+                if self.comparable_version(
+                    self.opt_args.python
+                ) < self.comparable_version(ver):
                     return False, 0
             else:
                 x = self.re_match(r"\+[0-9]+", action)
-                ver = int(action[x.start() + 1:x.end()])
+                ver = int(action[x.start() + 1: x.end()])
                 if ver and ver < 6 and self.py23 < ver:
                     return False, 0
                 if ver and ver >= 6 and self.to_major_version < ver:
                     return False, 0
             action = action[x.end():]
         if action.startswith("-"):
             x = self.re_match(r"\-[0-9]+\.[0-9]", action)
             if x:
-                ver = action[x.start():x.end()]
-                if (
-                    self.comparable_version(self.opt_args.python_ver)
-                    > self.comparable_version(ver)
-                ):
+                ver = action[x.start(): x.end()]
+                if self.comparable_version(
+                    self.opt_args.python
+                ) > self.comparable_version(ver):
                     return False, 0
             else:
                 x = self.re_match(r"-[0-9]+", action)
-                ver = int(action[x.start() + 1:x.end()])
+                ver = int(action[x.start() + 1: x.end()])
                 if ver and ver < 6 and self.py23 > ver:
                     return False, 0
                 if ver and ver >= 6 and self.to_major_version > ver:
                     return False, 0
             action = action[x.end():]
         if action == "s":
             rule, expr, res, regex, not_expr, sre = self.split_py_re_rules(params[0])
             if sre and re.search(sre, self.lines[nro]):
                 return False, 0
             if regex:
-                self.lines[nro] = re.sub(regex,
-                                         params[1] % self.__dict__,
-                                         self.lines[nro])
+                self.lines[nro] = re.sub(
+                    regex, params[1] % self.__dict__, self.lines[nro]
+                )
             return False, 0
         elif action == "d":
             del self.lines[nro]
             return False, -1
         elif action == "$":
             if not hasattr(self, params[0]):
                 self.raise_error("Function %s not found!" % params[0])
@@ -520,26 +470,26 @@
         rule, expr, res, regex, not_expr, sre = self.split_py_re_rules(rule)
         if not res:
             return res
 
         if sre and re.search(sre, self.lines[nro]):
             return False
 
-        if (
-            (not not_expr and not self.re_match(regex, self.lines[nro]))
-            or (not_expr and self.re_match(regex, self.lines[nro]))
+        if (not not_expr and not self.re_match(regex, self.lines[nro])) or (
+            not_expr and self.re_match(regex, self.lines[nro])
         ):
             return False
         return regex
 
     def load_config2(self, confname):
         configpath = os.path.join(
             os.path.dirname(os.path.abspath(os.path.expanduser(__file__))),
             "config",
-            confname + ".yml")
+            confname + ".yml",
+        )
         if os.path.isfile(configpath):
             with open(configpath, "r") as fd:
                 return yaml.safe_load(fd)
         internal_name = "RULES_%s" % confname.upper()
         if internal_name not in globals():
             self.raise_error("File %s not found!" % configpath)
             return []
@@ -575,75 +525,149 @@
         self.utf8_decl_nro = -1
         self.lines_2_rm = []
 
         TARGET = self.load_config("globals_xml" if self.is_xml else "globals")
         if self.opt_args.pypi_package:
             if self.python_future:
                 TARGET += self.load_config("to_pypi_future")
-            TARGET += self.load_config("to_pypi_py2" if self.py23 == 2
-                                       else "to_pypi_py3")
+            else:
+                TARGET += self.load_config(
+                    "to_pypi_py2" if self.py23 == 2 else "to_pypi_py3"
+                )
         elif self.is_xml:
-            TARGET += self.load_config("to_xml_old" if self.to_major_version < 8
-                                       else "to_xml_new")
+            TARGET += self.load_config(
+                "to_xml_old" if self.to_major_version < 8 else "to_xml_new"
+            )
         elif self.from_major_version:
             if self.from_major_version < 8 and self.to_major_version >= 8:
                 TARGET += self.load_config("to_new_api")
             elif self.from_major_version >= 8 and self.to_major_version < 8:
                 TARGET += self.load_config("to_old_api")
-            TARGET += self.load_config("to_odoo_py2" if self.to_major_version <= 10
-                                       else "to_odoo_py3")
+            TARGET += self.load_config(
+                "to_odoo_py2" if self.to_major_version <= 10 else "to_odoo_py3"
+            )
         else:
-            TARGET += self.load_config("to_odoo_py2" if self.to_major_version <= 10
-                                       else "to_odoo_py3")
+            TARGET += self.load_config(
+                "to_odoo_py2" if self.to_major_version <= 10 else "to_odoo_py3"
+            )
         return TARGET
 
-    def do_migrate_source(self):
+    def do_process_source(self):
         if self.ignore_file:
             return
+        if os.path.basename(self.ffn) in (
+                "history.rst", "HISTORY.rst", "CHANGELOG.rst"):
+            return self.do_upgrade_history()
+        if self.ffn.endswith('.py') or self.ffn.endswith('.xml'):
+            return self.do_migrate_source()
+        return False
+
+    def do_migrate_source(self):
+
+        def run_sub_rules(rule, nro, regex, next_nro):
+            do_continue = do_break = False
+            for subrule in rule[1:]:
+                # subrule may be: ("s", src, tgt) or ("d") or ...
+                do_break, offset = self.update_line(nro, subrule, regex)
+                if offset:
+                    next_nro = nro + 1 + offset
+                    if offset < 0:
+                        do_continue = True
+                        break
+                elif do_break:
+                    break
+            return do_continue, do_break, next_nro
+
         TGT_RULES = self.init_env()
         nro = 0
         while nro < len(self.lines):
             next_nro = nro + 1
             do_continue = False
-            if not self.lines[nro]:
-                do_continue = True
-            else:
-                for rule in TGT_RULES:
-                    # rule format: (action, )
-                    #              (action, (params), ...)
-                    # Match python expression and extract REGEX from EREGEX
-                    regex = self.rule_matches(rule[0], nro)
-                    for subrule in rule[1:]:
-                        # subrule may be: ("s", src, tgt) or ("d") or ...
-                        do_break, offset = self.update_line(nro, subrule, regex)
-                        if offset:
-                            next_nro = nro + 1 + offset
-                            if offset < 0:
-                                do_continue = True
-                                break
-                        elif do_break:
-                            break
-                    if do_continue or do_break:
-                        break
+            # if not self.lines[nro]:
+            #     for rule in TGT_RULES:
+            #         if rule[0] != "$":
+            #             continue
+            #         do_continue, do_break, next_nro = run_sub_rules(
+            #             rule, nro, rule[0], next_nro)
+            #         if do_continue or do_break:
+            #             break
+            #     do_continue = True
+            # else:
+            for rule in TGT_RULES:
+                # rule format: (action, )
+                #              (action, (params), ...)
+                # Match python expression and extract REGEX from EREGEX
+                regex = self.rule_matches(rule[0], nro)
+                do_continue, do_break, next_nro = run_sub_rules(
+                    rule, nro, regex, next_nro)
+                # for subrule in rule[1:]:
+                #     # subrule may be: ("s", src, tgt) or ("d") or ...
+                #     do_break, offset = self.update_line(nro, subrule, regex)
+                #     if offset:
+                #         next_nro = nro + 1 + offset
+                #         if offset < 0:
+                #             do_continue = True
+                #             break
+                #     elif do_break:
+                #         break
+                if do_continue or do_break:
+                    break
             if do_continue:
                 nro = next_nro
                 continue
             nro += 1
 
+    def do_upgrade_history(self):
+        if not self.opt_args.test_res_msg:
+            return
+        last_date = ""
+        found_list = False
+        title_nro = qua_nro = i_start = i_end = -1
+        for nro, ln in enumerate(self.lines):
+            if not ln:
+                if found_list:
+                    break
+                continue
+            if not last_date and re.match(r"[0-9]+\.[0-9]+\.[0-9]+.*\([0-9]+", ln):
+                x = re.search(r"\([0-9]{4}-[0-9]{2}-[0-9]{2}\)", ln)
+                i_start = x.start() + 1
+                i_end = x.end() - 1
+                last_date = ln[i_start: i_end]
+                title_nro = nro
+                continue
+            if qua_nro < 0 and ln.startswith("* [QUA]"):
+                qua_nro = nro
+            if last_date and ln.startswith("*"):
+                found_list = True
+        if (
+            last_date
+            and found_list
+            and (datetime.now() - datetime.strptime(last_date, "%Y-%m-%d")).days < 20
+        ):
+            if qua_nro:
+                self.lines[qua_nro] = self.opt_args.test_res_msg
+            else:
+                nro -= nro - 1
+                self.lines.insert(nro, self.opt_args.test_res_msg)
+                if not self.opt_args.dry_run:
+                    with open(self.ffn, 'w') as fd:
+                        fd.write("\n".join(self.lines))
+            self.lines[title_nro] = (
+                self.lines[title_nro][:i_start]
+                + datetime.strftime(datetime.now(), "%Y-%m-%d")
+                + self.lines[title_nro][i_end:])
+
     def write_xml(self, out_ffn):
         with open(out_ffn, 'w') as fd:
-            xml = ET.fromstring(
-                _b("\n".join(self.lines).replace('\t', '    '))
-            )
+            xml = ET.fromstring(_b("\n".join(self.lines).replace('\t', '    ')))
             fd.write("<?xml version=\"1.0\" encoding=\"utf-8\" ?>\n")
-            fd.write(ET.tostring(
-                xml,
-                encoding="unicode",
-                with_comments=True,
-                pretty_print=True)
+            fd.write(
+                ET.tostring(
+                    xml, encoding="unicode", with_comments=True, pretty_print=True
+                )
             )
 
     def format_file(self, out_ffn):
         prettier_config = False
         black_config = False
         path = os.path.dirname(os.path.abspath(os.path.expanduser(out_ffn)))
         while not prettier_config and not black_config:
@@ -652,112 +676,130 @@
             if os.path.isfile(os.path.join(path, ".prettierrc.yml")):
                 prettier_config = os.path.join(path, ".prettierrc.yml")
             if path == os.path.abspath(os.path.expanduser("~")) or path == "/":
                 break
             path = os.path.dirname(path)
         if self.is_xml:
             if prettier_config:
-                cmd = ("npx prettier --plugin=@prettier/plugin-xml --config=%s"
-                       % prettier_config)
+                cmd = (
+                    "npx prettier --plugin=@prettier/plugin-xml --config=%s"
+                    % prettier_config
+                )
             else:
                 cmd = "npx prettier --plugin=@prettier/plugin-xml --print-width=88"
             cmd += " --no-xml-self-closing-space --tab-width=4 --prose-wrap=always"
             cmd += " --write "
             cmd += out_ffn
-            z0lib.run_traced(cmd)
+            z0lib.run_traced(cmd, dry_run=self.opt_args.dry_run)
         else:
             opts = "--skip-source-first-line"
             if self.py23 == 2 or self.python_future:
                 opts += " --skip-string-normalization"
             cmd = "black %s -q %s" % (opts, out_ffn)
-            z0lib.run_traced(cmd)
+            z0lib.run_traced(cmd, dry_run=self.opt_args.dry_run)
 
     def close(self):
         if self.opt_args.output:
             if os.path.isdir(self.opt_args.output):
-                out_ffn = os.path.join(self.opt_args.output,
-                                       os.path.basename(self.ffn))
+                out_ffn = os.path.join(self.opt_args.output, os.path.basename(self.ffn))
             else:
                 out_ffn = self.opt_args.output
             if not os.path.isdir(os.path.dirname(out_ffn)):
                 os.mkdir(os.path.isdir(os.path.dirname(out_ffn)))
         else:
             out_ffn = self.ffn
-        if not self.ignore_file and self.source != "\n".join(self.lines):
-            bakfile = '%s.bak' % out_ffn
-            if os.path.isfile(bakfile):
-                os.remove(bakfile)
-            if os.path.isfile(out_ffn):
-                os.rename(out_ffn, bakfile)
-            if self.is_xml:
-                self.write_xml(out_ffn)
-            else:
-                with open(out_ffn, 'w') as fd:
-                    fd.write("\n".join(self.lines))
+        if not self.ignore_file and (out_ffn != self.ffn
+                                     or self.source != "\n".join(self.lines)):
+            if not self.opt_args.in_place:
+                bakfile = '%s.bak' % out_ffn
+                if os.path.isfile(bakfile):
+                    os.remove(bakfile)
+                if os.path.isfile(out_ffn):
+                    os.rename(out_ffn, bakfile)
+            if not self.opt_args.dry_run:
+                if self.is_xml:
+                    self.write_xml(out_ffn)
+                else:
+                    with open(out_ffn, 'w') as fd:
+                        fd.write("\n".join(self.lines))
             if self.opt_args.verbose > 0:
                 print('👽 %s' % out_ffn)
             if not self.opt_args.no_parse_with_formatter:
                 self.format_file(out_ffn)
         elif self.opt_args.lint_anyway:
             self.format_file(out_ffn)
 
 
 def main(cli_args=None):
     cli_args = cli_args or sys.argv[1:]
     parser = argparse.ArgumentParser(
-        description="Migrate source file",
-        epilog="© 2021-2023 by SHS-AV s.r.l."
+        description="Beautiful source file", epilog="© 2021-2023 by SHS-AV s.r.l."
     )
     parser.add_argument('-a', '--lint-anyway', action='store_true')
-    parser.add_argument('-b', '--to-version', default="12.0")
+    parser.add_argument('-b', '--to-version')
     parser.add_argument('-F', '--from-version')
     parser.add_argument(
-        '-f', '--force',
+        '-f',
+        '--force',
         action='store_true',
-        help="Parse file containing '# flake8: noqa' or '# pylint: skip-file'"
+        help="Parse file containing '# flake8: noqa' or '# pylint: skip-file'",
+    )
+    parser.add_argument('--ignore-pragma', action='store_true')
+    parser.add_argument('-i', '--in-place', action='store_true')
+    parser.add_argument('-j', '--python')
+    parser.add_argument(
+        "-n",
+        "--dry-run",
+        help="do nothing (dry-run)",
+        action="store_true",
     )
     parser.add_argument('-o', '--output')
     parser.add_argument('-P', '--pypi-package', action='store_true')
+    parser.add_argument('--test-res-msg')
     parser.add_argument('-v', '--verbose', action='count', default=0)
     parser.add_argument('-V', '--version', action="version", version=__version__)
     parser.add_argument(
-        '-w', '--no-parse-with-formatter',
+        '-w',
+        '--no-parse-with-formatter',
         action='store_true',
-        help="do nor execute black or prettier on modified files"
+        help="do nor execute black or prettier on modified files",
     )
-    parser.add_argument('-y', '--python-ver')
-    parser.add_argument('path')
+    parser.add_argument('path', nargs="*")
     opt_args = parser.parse_args(cli_args)
     sts = 0
     if (
         opt_args.output
         and not os.path.isdir(opt_args.output)
         and not os.path.isdir(os.path.dirname(opt_args.output))
     ):
         sys.stderr.write('Path %s does not exist!' % os.path.dirname(opt_args.output))
         sts = 2
-    elif os.path.isdir(opt_args.path):
-        for root, dirs, files in os.walk(opt_args.path):
-            if 'setup' in dirs:
-                del dirs[dirs.index('setup')]
-            for fn in files:
-                if not fn.endswith('.py') and not fn.endswith('.xml'):
-                    continue
-                source = MigrateFile(os.path.join(root, fn), opt_args)
-                source.do_migrate_source()
+    else:
+        for path in opt_args.path or ("./",):
+            if os.path.isdir(os.path.expanduser(path)):
+                for root, dirs, files in os.walk(os.path.expanduser(path)):
+                    if 'setup' in dirs:
+                        del dirs[dirs.index('setup')]
+                    for fn in files:
+                        if not fn.endswith('.py') and not fn.endswith('.xml'):
+                            continue
+                        source = MigrateFile(
+                            os.path.abspath(os.path.join(root, fn)), opt_args
+                        )
+                        source.do_process_source()
+                        source.close()
+                        sts = source.sts
+                        if sts:
+                            break
+            elif os.path.isfile(path):
+                source = MigrateFile(os.path.abspath(path), opt_args)
+                source.do_process_source()
                 source.close()
                 sts = source.sts
-                if sts:
-                    break
-    elif os.path.isfile(opt_args.path):
-        source = MigrateFile(opt_args.path, opt_args)
-        source.do_migrate_source()
-        source.close()
-        sts = source.sts
-    else:
-        sys.stderr.write('Path %s does not exist!' % opt_args.path)
-        sts = 2
+            else:
+                sys.stderr.write('Path %s does not exist!' % path)
+                sts = 2
     return sts
 
 
 if __name__ == "__main__":
     exit(main())
```

### Comparing `wok_code-2.0.8/wok_code/scripts/odoo_translation_old.py` & `wok_code-2.0.9/wok_code/scripts/odoo_translation_old.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 
 import csv
 import os
 import re
 import sys
 import time
 from builtins import input
+
 # from subprocess import PIPE, Popen
 
 from babel.messages import pofile
 from openpyxl import load_workbook
 
 from os0 import os0
 from python_plus import _c
@@ -30,23 +31,34 @@
     from z0lib import z0lib
 try:
     from clodoo import clodoo
 except ImportError:
     import clodoo
 
 
-__version__ = "2.0.8"
+__version__ = "2.0.9"
 
 MAX_RECS = 100
 PUNCT = [' ', '.', ',', '!', ':']
 TNL_DICT = {}
 TNL_ACTION = {}
 SYNTAX = {'string': re.compile('"([^"\\\n]|\\.|\\\n)*"')}
-VERSIONS = ('16.0', '15.0', '14.0', '13.0', '12.0', '11.0',
-            '10.0', '9.0', '8.0', '7.0', '6.1')
+VERSIONS = (
+    '16.0',
+    '15.0',
+    '14.0',
+    '13.0',
+    '12.0',
+    '11.0',
+    '10.0',
+    '9.0',
+    '8.0',
+    '7.0',
+    '6.1',
+)
 PROTECT_TOKENS = [
     'Adviser',
     'Apply',
     'Approve',
     'Cancel',
     'Close',
     'Compute',
@@ -149,21 +161,21 @@
 
 
 def term_wo_tag(msgid):
     ltag = ''
     rtag = ''
     x = re.match('<[^>]+>', msgid)
     while x:
-        ltag += msgid[:x.end()]
-        rtag = msgid[:x.end()].replace("<", "</") + rtag
-        msgid = msgid[x.end():]
+        ltag += msgid[: x.end()]
+        rtag = msgid[: x.end()].replace("<", "</") + rtag
+        msgid = msgid[x.end() :]
         x = re.match('<[^>]+>', msgid)
     x = re.search(rtag, msgid)
     if x:
-        msgid = msgid[:x.start()]
+        msgid = msgid[: x.start()]
     return ltag, rtag
 
 
 def term_with_punct(msgid, msgstr, lpunct, rpunct):
     if msgid:
         return lpunct + msgid + rpunct, lpunct + msgstr + rpunct
     return lpunct + msgstr + rpunct
@@ -244,16 +256,17 @@
         hdr = True
         for nrow in sheet.rows:
             if hdr:
                 hdr = False
                 continue
             row = {}
             for ncol, cell in enumerate(nrow):
-                row[colnames[ncol]] = cell.value.replace(
-                    '\\n', '\n') if cell.value else cell.value
+                row[colnames[ncol]] = (
+                    cell.value.replace('\\n', '\n') if cell.value else cell.value
+                )
             ctr += process_row(ctx, module_rows, row)
         for row in module_rows:
             ctr += process_row(ctx, None, row)
         if ctx['opt_verbose']:
             print("\t... Read %d records" % ctr)
         return ctr
 
@@ -317,16 +330,18 @@
                 msgstr = translate_html(ctx, msgstr)
             if msgid2 not in TNL_DICT:
                 TNL_DICT[msgid2] = msgstr2
                 TNL_ACTION[msgid2] = 'P'
                 ctr += 1
             elif msgstr2 != TNL_DICT[msgid2]:
                 print('  Duplicate key "%s"' % msgid)
-                print('    Dictionary="%s"' % term_with_punct(
-                    None, TNL_DICT[msgid2], lpunct, rpunct))
+                print(
+                    '    Dictionary="%s"'
+                    % term_with_punct(None, TNL_DICT[msgid2], lpunct, rpunct)
+                )
                 print('    %-60.60s' % trline)
                 print('    Po="%s"' % msgstr)
                 print('    %-60.60s' % trline)
                 dummy = ''
                 if msgid2 in PROTECT_TOKENS:
                     dummy = 'D'
                 elif not msgstr:
@@ -382,19 +397,19 @@
                     elif value:
                         setattr(message, k, value)
                 ctr += 1
             elif msgid2 in TNL_DICT and msgstr != TNL_DICT[msgid2]:
                 for k, value in message.__dict__.items():
                     if k == 'string':
                         if ltag and rtag:
-                            message.string = term_with_tag(
-                                TNL_DICT[msgid2], ltag, rtag)
+                            message.string = term_with_tag(TNL_DICT[msgid2], ltag, rtag)
                         else:
                             message.string = term_with_punct(
-                                None, TNL_DICT[msgid2], lpunct, rpunct)
+                                None, TNL_DICT[msgid2], lpunct, rpunct
+                            )
                     elif value:
                         setattr(message, k, value)
                 ctr += 1
                 fdiff = True
             elif msgid and msgid2 not in TNL_DICT and msgid2 not in untnl:
                 if ctx['opt_verbose']:
                     print('\tWarning: key <%s> not found in translation!' % msgid2)
```

### Comparing `wok_code-2.0.8/wok_code/scripts/gen_readme.py` & `wok_code-2.0.9/wok_code/scripts/gen_readme.py`

 * *Files 0% similar despite different names*

```diff
@@ -113,15 +113,15 @@
     from python_plus.python_plus import _b, _c, _u
 except ImportError:
     from python_plus import _b, _c, _u
 # import pdb
 standard_library.install_aliases()
 
 
-__version__ = "2.0.8"
+__version__ = "2.0.9"
 
 RED = "\033[1;31m"
 GREEN = "\033[1;32m"
 YELLOW = "\033[1;33m"
 CLEAR = "\033[0;m"
 RMODE = "rU" if sys.version_info[0] == 2 else "r"
 GIT_USER = {
@@ -1698,15 +1698,15 @@
             for module in ctx["manifest"].get(item, []):
                 new_module = transodoo.translate_from_to(
                     ctx,
                     "ir.module.module",
                     module,
                     ctx["from_version"],
                     ctx["odoo_vid"],
-                    ttype="module"
+                    ttype="module",
                 )
                 if isinstance(new_module, (list, tuple)):
                     if module in new_module:
                         modules.append(module)
                     else:
                         module.update(new_module)
                 else:
@@ -1844,32 +1844,43 @@
             ctx["repos_name"],
         )
 
 
 def setup_names(fn, email=None):
     if email == "name":
         with open(fn, RMODE) as fd:
-            return ", ".join([
-                x.split("*", 1)[1].split("<", 1)[0].strip()
-                if x.startswith("*") else x.split("<", 1)[0].strip()
-                for x in fd.read().split("\n") if x
-            ])
+            return ", ".join(
+                [
+                    x.split("*", 1)[1].split("<", 1)[0].strip()
+                    if x.startswith("*")
+                    else x.split("<", 1)[0].strip()
+                    for x in fd.read().split("\n")
+                    if x
+                ]
+            )
     elif email == "email":
         with open(fn, RMODE) as fd:
-            return ", ".join([
-                "<" + x.split("*", 1)[1].split("<", 1)[1].strip()
-                if x.startswith("*") else "<" + x.split("<", 1)[1].strip()
-                for x in fd.read().split("\n") if x
-            ])
+            return ", ".join(
+                [
+                    "<" + x.split("*", 1)[1].split("<", 1)[1].strip()
+                    if x.startswith("*")
+                    else "<" + x.split("<", 1)[1].strip()
+                    for x in fd.read().split("\n")
+                    if x
+                ]
+            )
     else:
         with open(fn, RMODE) as fd:
-            return ", ".join([
-                x.split("*", 1)[0].strip() if x.startswith("*") else x.strip()
-                for x in fd.read().split("\n") if x
-            ])
+            return ", ".join(
+                [
+                    x.split("*", 1)[0].strip() if x.startswith("*") else x.strip()
+                    for x in fd.read().split("\n")
+                    if x
+                ]
+            )
 
 
 def complete_setup(ctx, setup_fn):
     with open(setup_fn, RMODE) as fd:
         AUTH_RE = re.compile("^author *=")
         EMAIL_RE = re.compile("^author_email *=")
         SOURCE_ROOT = "https://github.com/zeroincombenze/tools"
@@ -1880,18 +1891,20 @@
         DOC_URL = "https://zeroincombenze-tools.readthedocs.io/en/latest/%s"
         CHANGELOG_RE = re.compile("^changelog_url *=")
         CHANGELOG_URL = SOURCE_ROOT + "/blob/master/%s/egg-info/CHANGELOG.rst"
         contents = ""
         for line in fd.read().split("\n"):
             if AUTH_RE.match(line):
                 line = "author = \"%s\"" % setup_names(
-                    "egg-info/CONTRIBUTORS.txt", email="name")
+                    "egg-info/CONTRIBUTORS.txt", email="name"
+                )
             elif EMAIL_RE.match(line):
                 line = "author_email = \"%s\"" % setup_names(
-                    "egg-info/CONTRIBUTORS.txt",  email="email")
+                    "egg-info/CONTRIBUTORS.txt", email="email"
+                )
             elif URL_RE.match(line):
                 line = line.split("=")[0] + ("=\"%s\"," % SOURCE_ROOT)
             elif SOURCE_URL_RE.match(line):
                 line = "source_url = \"%s\"" % (SOURCE_URL % ctx["module_name"])
             elif DOC_URL_RE.match(line):
                 line = "doc_url = \"%s\"" % (DOC_URL % ctx["module_name"])
             elif CHANGELOG_RE.match(line):
```

### Comparing `wok_code-2.0.8/wok_code/scripts/lint_2_compare.py` & `wok_code-2.0.9/wok_code/scripts/lint_2_compare.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,34 +5,34 @@
 import argparse
 from lxml import etree
 import re
 
 from python_plus import _b, _u
 from z0lib import z0lib
 
-__version__ = "2.0.8"
+__version__ = "2.0.9"
 
 
 IGNORE_DIRS = (".idea", ".git", "egg-info", "setup")
 REGEX_CM = re.compile("(^ *#|^.* #)")
 REGEX_OE = re.compile(r"([\"'])https?://www.openerp.com([\"'])")
 REGEX_OO = re.compile(r"([\"'])https?://(www.)?odoo.com([\"'])")
 
 
 def get_names(left_path, right_path):
-    left_base = right_base = ''
+    left_base = right_base = ""
     while left_path and right_path and left_path != right_path:
         left_base = os.path.basename(left_path)
         right_base = os.path.basename(right_path)
         left_path = os.path.dirname(left_path)
         right_path = os.path.dirname(right_path)
     if not left_base:
-        left_base = 'left'
+        left_base = "left"
     if not right_base:
-        right_base = 'right'
+        right_base = "right"
     return left_base, right_base
 
 
 def format_xml(opt_args, source, target):
     with open(source, "r") as fd:
         try:
             root = etree.XML(_b(fd.read()))
@@ -48,17 +48,17 @@
             xml_text = None
     if xml_text:
         xml_text = xml_text.replace("\n\n", "\n")
         with open(target, "w") as fd:
             fd.write(xml_text)
     else:
         z0lib.run_traced(
-            'cp %s %s' % (source, target),
+            "cp %s %s" % (source, target),
             verbose=opt_args.dry_run,
-            dry_run=opt_args.dry_run
+            dry_run=opt_args.dry_run,
         )
 
 
 def cp_file(opt_args, left_diff_path, right_diff_path, left_path, right_path, base):
     if (
         base.endswith(".pyc")
         or ((base.endswith(".po") or base.endswith(".pot")) and opt_args.ignore_po)
@@ -67,227 +67,264 @@
     ):
         return
     elif os.path.isfile(left_path):
         if base.endswith(".xml"):
             format_xml(opt_args, left_path, os.path.join(left_diff_path, base))
         else:
             z0lib.run_traced(
-                'cp %s %s' % (left_path, os.path.join(left_diff_path, base)),
+                "cp %s %s" % (left_path, os.path.join(left_diff_path, base)),
                 verbose=opt_args.dry_run,
-                dry_run=opt_args.dry_run)
+                dry_run=opt_args.dry_run,
+            )
     if os.path.isfile(right_path):
         if base.endswith(".xml"):
             format_xml(opt_args, right_path, os.path.join(right_diff_path, base))
         else:
             z0lib.run_traced(
-                'cp %s %s' % (right_path, os.path.join(right_diff_path, base)),
+                "cp %s %s" % (right_path, os.path.join(right_diff_path, base)),
                 verbose=opt_args.dry_run,
-                dry_run=opt_args.dry_run)
+                dry_run=opt_args.dry_run,
+            )
 
 
 def match(opt_args, left_diff_path, right_diff_path, left_path, right_path):
     if os.path.isfile(left_path):
         base = os.path.basename(left_path)
         cp_file(opt_args, left_diff_path, right_diff_path, left_path, right_path, base)
     elif os.path.isfile(right_path):
         base = os.path.basename(right_path)
         cp_file(opt_args, left_diff_path, right_diff_path, left_path, right_path, base)
 
 
-def matchdir_based(opt_args, left_diff_path, right_diff_path, left_path, right_path,
-                   base):
+def matchdir_based(
+    opt_args, left_diff_path, right_diff_path, left_path, right_path, base
+):
     left_diff_path = os.path.join(left_diff_path, base)
     if not os.path.isdir(left_diff_path):
-        z0lib.run_traced('mkdir %s' % left_diff_path,
-                         verbose=opt_args.dry_run,
-                         dry_run=opt_args.dry_run)
+        z0lib.run_traced(
+            "mkdir %s" % left_diff_path,
+            verbose=opt_args.dry_run,
+            dry_run=opt_args.dry_run,
+        )
     right_diff_path = os.path.join(right_diff_path, base)
     if not os.path.isdir(right_diff_path):
-        z0lib.run_traced('mkdir %s' % right_diff_path,
-                         verbose=opt_args.dry_run,
-                         dry_run=opt_args.dry_run)
+        z0lib.run_traced(
+            "mkdir %s" % right_diff_path,
+            verbose=opt_args.dry_run,
+            dry_run=opt_args.dry_run,
+        )
     if os.path.isdir(left_path):
         for fn in os.listdir(left_path):
             base = os.path.basename(fn)
-            matchdir(opt_args,
-                     left_diff_path,
-                     right_diff_path,
-                     os.path.join(left_path, fn),
-                     os.path.join(right_path, base))
+            matchdir(
+                opt_args,
+                left_diff_path,
+                right_diff_path,
+                os.path.join(left_path, fn),
+                os.path.join(right_path, base),
+            )
     if os.path.isdir(right_path):
         for fn in os.listdir(right_path):
             base = os.path.basename(fn)
             if not os.path.exists(os.path.join(left_path, base)):
-                matchdir(opt_args,
-                         left_diff_path,
-                         right_diff_path,
-                         os.path.join(left_path, base),
-                         os.path.join(right_path, fn), )
+                matchdir(
+                    opt_args,
+                    left_diff_path,
+                    right_diff_path,
+                    os.path.join(left_path, base),
+                    os.path.join(right_path, fn),
+                )
 
 
 def matchdir(opt_args, left_diff_path, right_diff_path, left_path, right_path):
     if os.path.isdir(left_path):
         base = os.path.basename(left_path)
-        if base not in IGNORE_DIRS :
+        if base not in IGNORE_DIRS:
             matchdir_based(
                 opt_args, left_diff_path, right_diff_path, left_path, right_path, base
             )
     elif os.path.isdir(right_path):
         base = os.path.basename(right_path)
-        if base not in IGNORE_DIRS :
+        if base not in IGNORE_DIRS:
             matchdir_based(
                 opt_args, left_diff_path, right_diff_path, left_path, right_path, base
             )
     else:
         match(opt_args, left_diff_path, right_diff_path, left_path, right_path)
 
 
 def remove_comment(opt_args, root, files, compare_path=None):
     def remove_identical_files(left_dir, right_dir, fn):
         left_path = os.path.join(left_dir, fn)
         right_path = os.path.join(right_dir, fn)
         sts, stdout, stderr = z0lib.run_traced(
-            'diff -r %s %s' % (left_path, right_path),
+            "diff -r %s %s" % (left_path, right_path),
             verbose=False,
-            dry_run=opt_args.dry_run)
+            dry_run=opt_args.dry_run,
+        )
         if sts == 0:
             os.unlink(left_path)
             os.unlink(right_path)
+
     for fn in files:
         ffn = os.path.join(root, fn)
         if not ffn.endswith(".py"):
             if opt_args.purge and compare_path:
                 remove_identical_files(root, compare_path, fn)
             continue
         source = ""
         with open(ffn, "r") as fd:
             for line in fd.read().split("\n"):
                 line = REGEX_OE.sub(r"\1https://www.odoo.com\2", line)
                 line = REGEX_OO.sub(r"\1https://www.odoo.com\2", line)
                 x = REGEX_CM.match(line)
                 if x:
-                    source += ("%s\n" % (line[x.start():x.end()-1].rstrip() or "#"))
+                    source += "%s\n" % (line[x.start() : x.end() - 1].rstrip() or "#")
                 else:
-                    source += ("%s\n" % line.rstrip())
+                    source += "%s\n" % line.rstrip()
         with open(ffn, "w") as fd:
             fd.write(source)
         if opt_args.purge and compare_path:
             remove_identical_files(root, compare_path, fn)
 
 
 def lintdir(opt_args, left_path, right_path):
-    z0lib.run_traced('black %s' % left_path,
-                     verbose=opt_args.dry_run,
-                     dry_run=opt_args.dry_run)
-    z0lib.run_traced('black %s' % right_path,
-                     verbose=opt_args.dry_run,
-                     dry_run=opt_args.dry_run)
+    z0lib.run_traced(
+        "black %s" % left_path, verbose=opt_args.dry_run, dry_run=opt_args.dry_run
+    )
+    z0lib.run_traced(
+        "black %s" % right_path, verbose=opt_args.dry_run, dry_run=opt_args.dry_run
+    )
     if opt_args.ignore_doc:
         for root, _dirs, files in os.walk(left_path):
             remove_comment(opt_args, root, files)
         for root, _dirs, files in os.walk(right_path):
             compare_path = None
             if root.startswith(right_path):
-                compare_path = left_path + root[len(right_path):]
+                compare_path = left_path + root[len(right_path) :]
             remove_comment(opt_args, root, files, compare_path=compare_path)
 
 
 def main(cli_args=None):
     cli_args = cli_args or sys.argv[1:]
     parser = argparse.ArgumentParser(
         description="Compare 2 paths after formatted them in the same way",
-        epilog="© 2021-2023 by SHS-AV s.r.l."
+        epilog="© 2021-2023 by SHS-AV s.r.l.",
     )
-    parser.add_argument('-b', '--odoo-version')
-    parser.add_argument('-c', '--cache', action="store_true", help="Use cached values")
+    parser.add_argument("-b", "--odoo-version")
+    parser.add_argument("-c", "--cache", action="store_true", help="Use cached values")
     parser.add_argument(
-        "-d", "--ignore-doc",
+        "-d",
+        "--ignore-doc",
         action="store_true",
-        help="Ignore README, docs and comment in files")
+        help="Ignore README, docs and comment in files",
+    )
     parser.add_argument("-i", "--ignore-po", action="store_true")
-    parser.add_argument("-m", "--meld", action="store_true", help='Use meld')
+    parser.add_argument("-m", "--meld", action="store_true", help="Use meld")
     parser.add_argument(
-        "-P", "--purge",
+        "-P",
+        "--purge",
         action="store_true",
-        help='Purge identical files on temporary dirs')
+        help="Purge identical files on temporary dirs",
+    )
     parser.add_argument("-n", "--dry-run", dest="dry_run", action="store_true")
-    parser.add_argument('-v', '--verbose', action='count', default=0)
-    parser.add_argument('-V', '--version', action="version", version=__version__)
-    parser.add_argument('left_path')
-    parser.add_argument('right_path', nargs='?')
+    parser.add_argument("-v", "--verbose", action="count", default=0)
+    parser.add_argument("-V", "--version", action="version", version=__version__)
+    parser.add_argument("left_path")
+    parser.add_argument("right_path", nargs="?")
     opt_args = parser.parse_args(cli_args)
     if not opt_args.right_path:
         # When just 1 path is issued, current directory become the left path
         # that is the reference path
         opt_args.right_path = os.path.abspath(opt_args.left_path)
         opt_args.left_path = os.path.abspath(os.getcwd())
     else:
         opt_args.right_path = os.path.abspath(opt_args.right_path)
     opt_args.left_path = os.path.abspath(opt_args.left_path)
     if (
-        os.path.isfile(opt_args.left_path) and os.path.isdir(opt_args.right_path) or
-        os.path.isdir(opt_args.left_path) and os.path.isfile(opt_args.right_path)
+        os.path.isfile(opt_args.left_path)
+        and os.path.isdir(opt_args.right_path)
+        or os.path.isdir(opt_args.left_path)
+        and os.path.isfile(opt_args.right_path)
     ):
-        print('Cannot compare file against dir!')
-    diff_path = os.path.expanduser('~/tmp/diff')
+        print("Cannot compare file against dir!")
+    diff_path = os.path.expanduser("~/tmp/diff")
     if not os.path.isdir(os.path.dirname(diff_path)):
         os.mkdir(os.path.dirname(diff_path))
     if not os.path.isdir(diff_path):
         os.mkdir(diff_path)
     left_base, right_base = get_names(opt_args.left_path, opt_args.right_path)
     left_diff_path = os.path.join(diff_path, left_base)
     right_diff_path = os.path.join(diff_path, right_base)
     if (
-        not opt_args.cache or
-        not os.path.isdir(left_diff_path) or
-        not os.path.isdir(right_diff_path)
+        not opt_args.cache
+        or not os.path.isdir(left_diff_path)
+        or not os.path.isdir(right_diff_path)
     ):
         if os.path.isdir(left_diff_path):
-            z0lib.run_traced('chmod -R +w %s' % left_diff_path,
-                             verbose=opt_args.dry_run,
-                             dry_run=opt_args.dry_run)
-            z0lib.run_traced('rm -fR %s' % left_diff_path,
-                             verbose=opt_args.dry_run,
-                             dry_run=opt_args.dry_run)
+            z0lib.run_traced(
+                "chmod -R +w %s" % left_diff_path,
+                verbose=opt_args.dry_run,
+                dry_run=opt_args.dry_run,
+            )
+            z0lib.run_traced(
+                "rm -fR %s" % left_diff_path,
+                verbose=opt_args.dry_run,
+                dry_run=opt_args.dry_run,
+            )
         if os.path.isdir(right_diff_path):
-            z0lib.run_traced('chmod -R +w %s' % right_diff_path,
-                             verbose=opt_args.dry_run,
-                             dry_run=opt_args.dry_run)
-            z0lib.run_traced('rm -fR %s' % right_diff_path,
-                             verbose=opt_args.dry_run,
-                             dry_run=opt_args.dry_run)
-        z0lib.run_traced('mkdir %s' % left_diff_path,
-                         verbose=opt_args.dry_run,
-                         dry_run=opt_args.dry_run)
-        z0lib.run_traced('mkdir %s' % right_diff_path,
-                         verbose=opt_args.dry_run,
-                         dry_run=opt_args.dry_run)
-        matchdir(opt_args,
-                 left_diff_path,
-                 right_diff_path,
-                 opt_args.left_path,
-                 opt_args.right_path)
-        lintdir(opt_args,
-                left_diff_path,
-                right_diff_path)
-        z0lib.run_traced('chmod -R -w %s' % left_diff_path,
-                         verbose=opt_args.dry_run,
-                         dry_run=opt_args.dry_run)
-        z0lib.run_traced('chmod -R -w %s' % right_diff_path,
-                         verbose=opt_args.dry_run,
-                         dry_run=opt_args.dry_run)
+            z0lib.run_traced(
+                "chmod -R +w %s" % right_diff_path,
+                verbose=opt_args.dry_run,
+                dry_run=opt_args.dry_run,
+            )
+            z0lib.run_traced(
+                "rm -fR %s" % right_diff_path,
+                verbose=opt_args.dry_run,
+                dry_run=opt_args.dry_run,
+            )
+        z0lib.run_traced(
+            "mkdir %s" % left_diff_path,
+            verbose=opt_args.dry_run,
+            dry_run=opt_args.dry_run,
+        )
+        z0lib.run_traced(
+            "mkdir %s" % right_diff_path,
+            verbose=opt_args.dry_run,
+            dry_run=opt_args.dry_run,
+        )
+        matchdir(
+            opt_args,
+            left_diff_path,
+            right_diff_path,
+            opt_args.left_path,
+            opt_args.right_path,
+        )
+        lintdir(opt_args, left_diff_path, right_diff_path)
+        z0lib.run_traced(
+            "chmod -R -w %s" % left_diff_path,
+            verbose=opt_args.dry_run,
+            dry_run=opt_args.dry_run,
+        )
+        z0lib.run_traced(
+            "chmod -R -w %s" % right_diff_path,
+            verbose=opt_args.dry_run,
+            dry_run=opt_args.dry_run,
+        )
     if opt_args.meld:
         sts, stdout, stderr = z0lib.run_traced(
-            'meld.exe %s %s' % (left_diff_path, right_diff_path),
+            "meld %s %s" % (left_diff_path, right_diff_path),
             verbose=True,
-            dry_run=opt_args.dry_run)
+            dry_run=opt_args.dry_run,
+        )
     else:
         sts, stdout, stderr = z0lib.run_traced(
-            'diff -r %s %s' % (left_diff_path, right_diff_path),
+            "diff -r %s %s" % (left_diff_path, right_diff_path),
             verbose=True,
-            dry_run=opt_args.dry_run)
+            dry_run=opt_args.dry_run,
+        )
     print(stdout, stderr)
     return sts
 
 
 if __name__ == "__main__":
     exit(main())
```

### Comparing `wok_code-2.0.8/wok_code/scripts/deploy_odoo.py` & `wok_code-2.0.9/wok_code/scripts/deploy_odoo.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     from wok_code.scripts.wget_odoo_repositories import main as get_list_from_url
 try:
     from clodoo.clodoo import build_odoo_param
 except ImportError:
     from clodoo import build_odoo_param
 
 
-__version__ = "2.0.8"
+__version__ = "2.0.9"
 
 MANIFEST_FILES = ["__manifest__.py", "__odoo__.py", "__openerp__.py", "__terp__.py"]
 
 ODOO_VALID_VERSIONS = (
     "16.0",
     "15.0",
     "14.0",
@@ -114,14 +114,16 @@
     "branch": "%(branch)-10.10s",
     "dif_branch": "%(branch)-10.10s",
     "git_org": "%(git_org)-14.14s",
     "git_url": "%(git_url)-64.64s",
     "path": "%(path)-56.56s",
     "stash": "%(stash)5.5s",
     "status": "%(status)s",
+    "brief": "%(brief)s",
+    "stage": "%(stage)-10.10s",
 }
 
 
 class OdooDeploy(object):
     """Odoo's organization/branch repositories
     self.repo_list is the repositories list of self.repo_info
     self.repo_info contains repository information
@@ -148,18 +150,15 @@
                 print("***** Missing git orgs: oca will be used!")
                 self.opt_args.git_orgs = ["oca"]
 
         if self.opt_args.action == "clone":
             self.master_branch = build_odoo_param(
                 "FULLVER", odoo_vid=opt_args.odoo_branch
             )
-        if (
-            self.opt_args.action in ("clone", "reclone")
-            and not self.opt_args.repos
-        ):
+        if self.opt_args.action in ("clone", "reclone") and not self.opt_args.repos:
             for git_org in opt_args.git_orgs:
                 self.get_repo_from_github(git_org=git_org)
             if "OCB" not in self.repo_list:
                 git_org = "odoo"
                 self.get_repo_from_github(git_org=git_org, only_ocb=True)
             if opt_args.link_oca and "oca" not in self.opt_args.git_orgs:
                 self.get_repo_from_github(git_org="oca")
@@ -195,15 +194,15 @@
                     self.repo_info[repo]["STASH"] = stash_list
             if git_org and git_org not in self.opt_args.git_orgs:
                 self.opt_args.git_orgs.append(git_org)
             if repo == "OCB" or not self.master_branch:
                 self.master_branch = build_odoo_param(
                     "FULLVER", odoo_vid=self.repo_info[repo]["BRANCH"]
                 )
-            if opt_args.action in ("list", "status"):
+            if opt_args.action in ("list", "status", "unstaged"):
                 self.add_addons_path(path, repo)
 
         self.git_org = opt_args.git_orgs[0] if opt_args.git_orgs else "oca"
         if self.repo_list:
             if "OCB" in self.repo_list and self.repo_list[0] != "OCB":
                 del self.repo_list[self.repo_list.index("OCB")]
                 self.repo_list.insert(0, "OCB")
@@ -254,18 +253,15 @@
                 git_url = "https://github.com/%s" % git_org
         return git_url, git_org
 
     def get_repo_from_switch(self):
         self.repo_list = []
         self.repo_info = {}
         for repo in self.opt_args.repos.split(","):
-            self.repo_info[repo] = {
-                "PATH": self.get_path_of_repo(repo),
-                "#": 1
-            }
+            self.repo_info[repo] = {"PATH": self.get_path_of_repo(repo), "#": 1}
         self.repo_list = sorted(self.repo_info.keys())
         if "OCB" in self.repo_list:
             del self.repo_list[self.repo_list.index("OCB")]
             self.repo_list = ["OCB"] + self.repo_list
 
     def get_repo_from_config(self):
         opt_args = self.opt_args
@@ -318,17 +314,19 @@
                 self.repo_info[dir] = {"PATH": path, "#": 0}
                 if os.path.islink(path):
                     self.repo_info[dir]["#"] = 1
             elif self.is_module(path):
                 repo = os.path.basename(root)
                 if repo == "addons":
                     repo = os.path.basename(os.path.dirname(root))
-                    if repo in ("odoo", "openerp", os.path.basename(
-                        self.repo_info.get(
-                            "OCB", {}).get("PATH", ""))):
+                    if repo in (
+                        "odoo",
+                        "openerp",
+                        os.path.basename(self.repo_info.get("OCB", {}).get("PATH", "")),
+                    ):
                         repo = "OCB"
                 if repo in self.repo_info:
                     self.repo_info[repo]["#"] += 1
 
         if self.target_path:
             # repo = "OCB"
             # if self.is_git_repo(path=self.target_path):
@@ -418,17 +416,15 @@
                 url = DEFAULT_DATA.get(hash_key, {}).get(repo)
                 if not url:
                     url = DEFAULT_DATA.get(hash_key, {}).get("URL")
                 if not url:
                     if self.opt_args.use_git:
                         url = "git@github.com:%s" % REPO_NAMES.get(git_org, git_org)
                     else:
-                        url = "https://github.com/%s" % REPO_NAMES.get(
-                            git_org, git_org
-                        )
+                        url = "https://github.com/%s" % REPO_NAMES.get(git_org, git_org)
                 url = "%s/%s.git" % (url, repo)
                 tgtdir = self.get_path_of_repo(repo)
                 self.repo_list.append(repo)
                 self.repo_info[repo] = {
                     "GIT_ORG": git_org,
                     "BRANCH": branch,
                     "URL": url,
@@ -591,16 +587,17 @@
 
     def get_path_of_repo(self, repo):
         tgtdir = self.repo_info.get(repo, {}).get("PATH")
         if not tgtdir:
             if self.repo_is_ocb(repo):
                 tgtdir = self.target_path
             else:
-                tgtdir = os.path.join(self.target_path or self.opt_args.target_path,
-                                      repo)
+                tgtdir = os.path.join(
+                    self.target_path or self.opt_args.target_path, repo
+                )
         return tgtdir
 
     def get_remote_info(self, verbose=True):
         verbose = verbose and self.opt_args.verbose
         branch = self.master_branch
         stash_list = ""
         url = None
@@ -758,29 +755,33 @@
             self.run_traced("cd %s" % tgtdir)
         sts, repo_branch, git_url, stash_list = self.get_remote_info()
         if os.path.islink(tgtdir):
             return sts, repo_branch
         cmd = "git push"
         sts, stdout, stderr = self.run_traced(cmd, verbose=False)
         if sts:
-            sts, stdout, stderr = z0lib.run_traced("git branch -r",
-                                                   verbose=self.opt_args.verbose)
+            sts, stdout, stderr = z0lib.run_traced(
+                "git branch -r", verbose=self.opt_args.verbose
+            )
             tag = "origin/%s" % repo_branch
             for ln in stdout.split("\n"):
                 if tag in ln:
                     if not self.opt_args.assume_yes:
                         print("Remove remote branch %s of %s!" % (repo_branch, repo))
                         dummy = input("Delete (y/n)? ")
                     if self.opt_args.assume_yes or dummy.lower().startswith("y"):
-                        self.run_traced("git push origin -d %s" % repo_branch,
-                                        verbose=self.opt_args.verbose)
+                        self.run_traced(
+                            "git push origin -d %s" % repo_branch,
+                            verbose=self.opt_args.verbose,
+                        )
                     self.run_traced(
                         "git commit --no-verify -m \"[NEW] Initial setup %s\""
                         % repo_branch,
-                        verbose=self.opt_args.verbose)
+                        verbose=self.opt_args.verbose,
+                    )
                     break
             cmd = "git push --set-upstream origin %s" % repo_branch
             sts, stdout, stderr = self.run_traced(cmd, verbose=self.opt_args.verbose)
         sleep(1)
         if sts == 0:
             sts, repo_branch, git_url, stash_list = self.get_remote_info()
         if sts:
@@ -924,36 +925,49 @@
         datas = {}
         for item in fmt_list:
             fmt += " " + FMT_PARAMS[item]
             datas[item] = item.upper()
         fmt = fmt.strip()
         print(fmt % datas)
         for repo in self.repo_list:
-            git_org = git_stat = ""
+            git_org = git_stat = brief = ""
+            stage = "staged"
             tgtdir = self.get_path_of_repo(repo)
             self.run_traced("cd %s" % tgtdir, verbose=False)
             sts, repo_branch, git_url, stash_list = self.get_remote_info(verbose=False)
             if sts == 0:
                 org_url, repo, git_org = self.data_from_url(git_url)
                 sts, stdout, stderr = self.run_traced("git status", verbose=False)
                 if sts == 0:
                     git_stat = stdout
+                    for ln in stdout.split("\n"):
+                        if (
+                            ln.strip()
+                            and "Your branch is up to date" not in ln
+                            and "working tree clean" not in ln
+                        ):
+                            brief += ln + "\n"
+                            if "On branch" not in ln:
+                                stage = "unstaged"
 
             datas = {
                 "repo": repo,
                 "sts": sts,
                 "branch": repo_branch,
                 "dif_branch": repo_branch if repo_branch != self.master_branch else "",
                 "git_org": git_org,
                 "git_url": git_url,
                 "path": tgtdir,
-                "stash": "stash" if self.repo_info[repo].get("STASH") else "",
+                "stash": "stash" if self.repo_info.get(repo, {}).get("STASH") else "",
                 "status": git_stat,
+                "brief": brief,
+                "stage": stage,
             }
-            print(fmt % datas)
+            if self.opt_args.action != "unstaged" or stage == "unstaged":
+                print(fmt % datas)
         if self.opt_args.show_addons:
             print()
             print(",".join(self.addons_path))
 
     def action_download_or_pull_repo(self):
         print("Odoo main version..........: %s" % self.master_branch)
         if self.opt_args.config:
@@ -992,23 +1006,27 @@
         default="12.0",
         help="Default Odoo version",
     )
     parser.add_argument("-c", "--config", help="Odoo configuration file")
     parser.add_argument("-D", "--default-gitorg", default="zero")
     # parser.add_argument("-d", "--deployment-mode", help="may be tree,server,odoo")
     parser.add_argument(
-        "-e", "--skip-if-exist",
+        "-e",
+        "--skip-if-exist",
         action="store_true",
-        help="Use this switch to add missed repositories when you reclone"
+        help="Use this switch to add missed repositories when you reclone",
     )
     parser.add_argument(
         "-F",
         "--format",
-        help=("Use 1 or + of " "sts,repo,branch,git_org,git_url,path,stash,status"),
-        default="sts,repo,branch,git_org,git_url,path,stash",
+        help=(
+            "Use 1 or + of "
+            "sts,repo,branch,brief,git_org,git_url,path,stash,stage,status"
+        ),
+        default="repo,stage,branch,git_org,git_url,stash",
     )
     parser.add_argument(
         "-G",
         "--git-orgs",
         help="Git organizations, comma separated - " "May be: oca librerp or zero",
     )
     parser.add_argument(
@@ -1023,61 +1041,61 @@
         action="store_true",
         help="Keep OCB/odoo organization owner",
     )
     parser.add_argument(
         "-L", "--list", action="store_true", help="Deprecated: use 'list' action!"
     )
     parser.add_argument(
-        "-l", "--local-reps",
+        "-l",
+        "--local-reps",
         default="l10n-italy,l10n-italy-supplemental",
-        help="Local repositories to load; default: l10n-italy,l10n-italy-supplemental"
+        help="Local repositories to load; default: l10n-italy,l10n-italy-supplemental",
     )
     parser.add_argument(
         "-m", "--multi", action="store_true", help="Multi version environment"
     )
     parser.add_argument(
         "-N",
         "--clone",
         action="store_true",
         help="Deprecated: use 'clone' action!",
     )
     parser.add_argument("-n", "--dry-run", action="store_true")
-    parser.add_argument(
-        "-o", "--origin",
-        help="Declare origin repo for 'merge' action"
-    )
+    parser.add_argument("-o", "--origin", help="Declare origin repo for 'merge' action")
     parser.add_argument(
         "-O", "--link-oca", action="store_true", help="Link to more OCA repositories"
     )
     parser.add_argument("-p", "--target-path", help="Local directory")
     parser.add_argument(
         "-R", "--reclone", action="store_true", help="Deprecated: use 'reclone' action!"
     )
     parser.add_argument(
-        "-r", "--repos",
-        help="Declare specific repositories to manage, comma separated"
+        "-r", "--repos", help="Declare specific repositories to manage, comma separated"
     )
     parser.add_argument(
         "-S", "--status", action="store_true", help="Deprecated: use 'status' action!"
     )
     parser.add_argument(
         "-U",
         "--only-update",
         action="store_true",
         help="Deprecated: use 'update' action!",
     )
     parser.add_argument("-v", "--verbose", action="count", default=0)
     parser.add_argument("-V", "--version", action="version", version=__version__)
     parser.add_argument(
-        "-x", "--extra-repo",
-        help="May be: all,none,connector,devel,maintainer,oca,odoo,vertical"
+        "-x",
+        "--extra-repo",
+        help="May be: all,none,connector,devel,maintainer,oca,odoo,vertical",
     )
     parser.add_argument("-y", "--assume-yes", action="store_true")
     parser.add_argument(
-        "action", nargs="?", help="May be clone,git-push,list,reclone,status,update"
+        "action",
+        nargs="?",
+        help="May be clone,git-push,list,reclone,status,unstaged,update",
     )
     opt_args = parser.parse_args(cli_args)
 
     if not opt_args.action:
         if opt_args.clone:
             opt_args.action = "clone"
         elif opt_args.list:
@@ -1086,33 +1104,34 @@
             opt_args.action = "reclone"
         elif opt_args.status:
             opt_args.action = "status"
         elif opt_args.only_update:
             opt_args.action = "update"
     opt_args.git_orgs = opt_args.git_orgs.split(",") if opt_args.git_orgs else []
 
-    if (
-        opt_args.action not in ("clone",
-                                "git-push",
-                                "list",
-                                "reclone",
-                                "status",
-                                "update")
+    if opt_args.action not in (
+        "clone",
+        "git-push",
+        "list",
+        "reclone",
+        "status",
+        "update",
+        "unstaged",
     ):
         print("No valid action issued!")
         exit(1)
 
     if opt_args.repos and not opt_args.target_path:
         print("No path issued for declared repositories")
         exit(1)
 
     deploy = OdooDeploy(opt_args)
     if opt_args.action == "list":
         deploy.action_list()
-    elif opt_args.action == "status":
+    elif opt_args.action in ("status", "unstaged"):
         deploy.action_status()
     else:
         deploy.action_download_or_pull_repo()
     return 0
 
 
 if __name__ == "__main__":
```

### Comparing `wok_code-2.0.8/wok_code/scripts/odoo_translation.py` & `wok_code-2.0.9/wok_code/scripts/odoo_translation.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 try:
     from clodoo import clodoo
 except ImportError:
     import clodoo
 
 # from python_plus import unicodes
 
-__version__ = "2.0.8"
+__version__ = "2.0.9"
 
 
 MODULE_SEP = "\ufffa"
 
 # (<en>, <it>, <module>, <result>, ovverride)
 TEST_DATA = [
     ("name", "nome", None, "nome"),
@@ -52,59 +52,61 @@
     (" Invoice", "", None, " Fattura"),
     (" Invoice ", "", None, " Fattura "),
     ("Invoices.", "", None, "Fatture."),
     ("line", "riga", None, "riga"),
     ("lines", "", None, "righe"),
     ("Invoice lines", "Righe fattura", None, "Righe fattura"),
     ("Sale", "Vendite", None, "Vendite"),
-    ("Sale Invoice lines", "Righe fattura di vendita", None,
-     "Righe fattura di vendita"),
+    (
+        "Sale Invoice lines",
+        "Righe fattura di vendita",
+        None,
+        "Righe fattura di vendita",
+    ),
     ("Credit", "Credito", None, "Credito"),
     ("Credit", "Avere", "l10n_it", "Avere"),
     ("account.tax", "*WRONG*", None, "account.tax"),
     ("Dear", "Gentile", None, "Gentile"),
     ("Dear ${name}", "", None, "Gentile ${name}"),
     ("Purchase", "", None, "Acquistare"),
     ("&gt; 100%%", "", None, "&gt; 100%%"),
     ("/usr/name/line", "", None, "/usr/name/line"),
     ("%s invoice lines", "righe %s fattura", None, "righe %s fattura"),
     ("# invoice lines", None, None, "N.fattura righe"),
-    ("Acceptance Account", "Conto RI.BA. all'incasso", None,
-     "Conto RiBA all'incasso"),
+    ("Acceptance Account", "Conto RI.BA. all'incasso", None, "Conto RiBA all'incasso"),
     ("Ri.Ba. Bank", "Banca Ri.Ba", None, "Banca RiBA"),
     ("Created by", "Creato da", None, "Creato da"),
     ("Created by", "Creato da", None, "Creato da"),
     ("Customer SEPA account", None, None, "Conto cliente SEPA"),
     ("Customer SEPA account", "Conto cliente SEPA", None, "Conto cliente SEPA", True),
     ("Account (Credit)", "Conto (avere)", None, "Conto (avere)"),
     ("Account (Credit)", None, "l10n_it", "Conto (Avere)"),
     ("Other Info", "Altre informazioni", None, "Altre informazioni"),
     ("Other Info", "Altre info", "l10n_it", "Altre info"),
 ]
 
 TNL_TYPES = (
-    'ir.actions.act_window,name',
-    'ir.model,name',
-    'ir.model.fields.field_description',
-    'ir.module.category,name',
-    'ir.module.module,description'
-    'ir.module.module,shortdesc',
-    'ir.module.module,summary',
-    'ir.ui.menu,name',
-    'ir.ui.view,arch_db',
+    "ir.actions.act_window,name",
+    "ir.model,name",
+    "ir.model.fields.field_description",
+    "ir.module.category,name",
+    "ir.module.module,description" "ir.module.module,shortdesc",
+    "ir.module.module,summary",
+    "ir.ui.menu,name",
+    "ir.ui.view,arch_db",
 )
 
 msg_time = time()
 
 
 def msg_burst(text):
     global msg_time
     t = time() - msg_time
     if t > 5:
-        print(text, '\r')
+        print(text, "\r")
         msg_time = time()
 
 
 class OdooTranslation(object):
     """ """
 
     def __init__(self, opt_args):
@@ -117,45 +119,60 @@
         self.dict = {}
         if (
             opt_args.target_path
             and opt_args.target_path.endswith(".po")
             and os.path.basename(os.path.dirname(opt_args.target_path)) == "i18n"
         ):
             self.opt_args.target_path = os.path.dirname(
-                os.path.dirname(opt_args.target_path))
+                os.path.dirname(opt_args.target_path)
+            )
         if not opt_args.file_xlsx:
             root = self.get_home_devel()
             if opt_args.dbg_template:
-                dict_name = os.path.join(root, 'pypi', 'tools', 'odoo_default_tnl.xlsx')
+                dict_name = os.path.join(root, "pypi", "tools", "odoo_default_tnl.xlsx")
             else:
-                dict_name = os.path.join(root, 'venv', 'bin', 'odoo_default_tnl.xlsx')
+                dict_name = os.path.join(root, "venv", "bin", "odoo_default_tnl.xlsx")
             if os.path.isfile(dict_name):
                 self.opt_args.file_xlsx = dict_name
 
         # Type classification
         # Name, Translatable, Grouped, Regex, Nolast
         self.types_decl = [
-            ("odoo_model",
-             False,
-             False,
-             (
-                 r"^([a-z0-9]{2,}[\._][a-z0-9]{2,}([\._][a-z0-9]{2,})?"
-                 r"|[0-9]+|/[-\w._]{2,}(/[-\w._]{2,})+)"
-             ),
-             False),
-            ("word", True, True, (
-                r"([a-zA-Z]{1,2}[./]([a-zA-Z]{1,2}[./])*([a-zA-Z]{1,2})*"
-                r"|(\w|# )([-/]?\w| # |`)*)"),
-             False),
+            (
+                "odoo_model",
+                False,
+                False,
+                (
+                    r"^([a-z0-9]{2,}[\._][a-z0-9]{2,}([\._][a-z0-9]{2,})?"
+                    r"|[0-9]+|/[-\w._]{2,}(/[-\w._]{2,})+)"
+                ),
+                False,
+            ),
+            (
+                "word",
+                True,
+                True,
+                (
+                    r"([a-zA-Z]{1,2}[./]([a-zA-Z]{1,2}[./])*([a-zA-Z]{1,2})*"
+                    r"|(\w|# )([-/]?\w| # |`)*)"
+                ),
+                False,
+            ),
             ("punct", True, False, r"[.,:;!?]+", True),
             ("space", False, True, r"\s+", True),
-            ("tag", False, False, (
-                r"(</?\w+[^/>]*/?>|%[a-zA-Z]|%\(\w+\)[a-zA-Z]"
-                r"|/w+(/w+)*|\$\{[^}]+\}|&\w+;)"
-            ), False),
+            (
+                "tag",
+                False,
+                False,
+                (
+                    r"(</?\w+[^/>]*/?>|%[a-zA-Z]|%\(\w+\)[a-zA-Z]"
+                    r"|/w+(/w+)*|\$\{[^}]+\}|&\w+;)"
+                ),
+                False,
+            ),
             ("space2", False, True, r"['’\"«»&]", True),
         ]
         for item in self.types_decl:
             if item[0] == "word":
                 self.re_word = item[3]
             elif item[0] == "space":
                 self.re_space = item[3]
@@ -163,40 +180,40 @@
                 self.re_space2 = item[3]
             elif item[0] == "tag":
                 self.re_tag = item[3]
         self.re_to_upper = r".*[-.(]$"
         self.build_alias_dict()
 
     def get_home_devel(self):
-        root = os.environ.get('HOME_DEVEL')
+        root = os.environ.get("HOME_DEVEL")
         if not root or not os.path.isdir(root):
-            if os.path.isdir(os.path.expanduser('~/odoo/devel')):
-                root = os.path.expanduser('~/odoo/devel')
-            elif os.path.isdir(os.path.expanduser('~/devel')):
-                root = os.path.expanduser('~/devel')
+            if os.path.isdir(os.path.expanduser("~/odoo/devel")):
+                root = os.path.expanduser("~/odoo/devel")
+            elif os.path.isdir(os.path.expanduser("~/devel")):
+                root = os.path.expanduser("~/devel")
             else:
-                root = os.environ.get('HOME')
+                root = os.environ.get("HOME")
         return root
 
     def ismodule(self, path):
         if os.path.isdir(path):
             if (
                 os.path.isfile(os.path.join(path, "__manifest__.py"))
                 or os.path.isfile(os.path.join(path, "__openerp__.py"))
             ) and os.path.isfile(os.path.join(path, "__init__.py")):
                 return True
         return False
 
     def isplural(self, term):
-        return (term.endswith("s")
-                and not term.endswith("%s")
-                and not term.endswith(")s")) or term.endswith("(s)")
+        return (
+            term.endswith("s") and not term.endswith("%s") and not term.endswith(")s")
+        ) or term.endswith("(s)")
 
     def isfullupper(self, term):
-        return (term == term.upper())
+        return term == term.upper()
 
     def get_filenames(self, filename=None):
         filename = filename or self.opt_args.file_xlsx
         tmp_file = bak_file = None
         if filename:
             tmp_file = "%s.tmp" % filename
             bak_file = "%s.bak" % filename
@@ -230,17 +247,17 @@
                 ):
                     tnxl = tnxl[0].lower() + tnxl[1:]
         return tnxl
 
     def set_plural(self, orig, term):
         def plural_term(term, suffix, sep):
             if sep:
-                term += (sep + suffix)
+                term += sep + suffix
             else:
-                term = term[: -1] + suffix
+                term = term[:-1] + suffix
             return term
 
         sep = "/" if orig.endswith("(s)") else ""
         if term.endswith("ca") or term.endswith("ga"):
             term = plural_term(term, "he", sep)
         elif term.endswith("cia") or term.endswith("gia"):
             if term[-4] in ("a", "e", "i", "o", "u"):
@@ -251,19 +268,17 @@
             term = plural_term(term, "e", sep)
         elif term.endswith("e") or term.endswith("o"):
             term = plural_term(term, "i", sep)
         return term
 
     def set_plural_if(self, hash_key, orig, tnxl, adjust_case=None):
         if self.isplural(orig):
-            hkey = hash_key[: -3] if hash_key.endswith("(s)") else hash_key[: -1]
+            hkey = hash_key[:-3] if hash_key.endswith("(s)") else hash_key[:-1]
             if hkey in self.dict:
-                tnxl = self.adjust_case(
-                    orig,
-                    self.set_plural(orig, self.dict[hkey][1]))
+                tnxl = self.adjust_case(orig, self.set_plural(orig, self.dict[hkey][1]))
             elif adjust_case:
                 tnxl = self.adjust_case(orig, tnxl)
         elif adjust_case:
             tnxl = self.adjust_case(orig, tnxl)
         return tnxl
 
     def get_term(self, hash_key, orig, tnxl, adjust_case=None):
@@ -276,30 +291,30 @@
         return tnxl
 
     def store_1_item(
         self, hash_key, msg_orig, msg_tnxl, override=None, module=None, is_tag=None
     ):
         if len(msg_orig) <= 1 and not is_tag:
             return msg_orig
-        if collections.Counter(msg_orig)['%'] != collections.Counter(msg_tnxl)['%']:
+        if collections.Counter(msg_orig)["%"] != collections.Counter(msg_tnxl)["%"]:
             print("*** Warning: different macro: " + msg_orig + " / " + msg_tnxl)
         if not is_tag:
             for item in self.tags:
                 tnxls = self.dict[item]
                 ltoken = "%s " % tnxls[0]
                 rtoken = "%s " % tnxls[1]
                 if msg_tnxl.startswith(ltoken):
                     msg_tnxl = msg_tnxl.replace(ltoken, rtoken, 1)
                 ltoken = " %s " % tnxls[0]
                 rtoken = " %s " % tnxls[1]
                 msg_tnxl = msg_tnxl.replace(ltoken, rtoken)
                 ltoken = " %s" % tnxls[0]
                 rtoken = " %s" % tnxls[1]
                 if msg_tnxl.endswith(ltoken):
-                    msg_tnxl = msg_tnxl[0: -len(ltoken)] + rtoken
+                    msg_tnxl = msg_tnxl[0 : -len(ltoken)] + rtoken
         hash_key = self.get_hash_key(hash_key, False, module=module)
         if hash_key and (
             hash_key not in self.dict
             or override
             or is_tag
             or (msg_tnxl and self.dict[hash_key][0] == self.dict[hash_key][1])
         ):
@@ -307,17 +322,17 @@
             if is_tag and hash_key not in self.tags:
                 self.tags.append(hash_key)
         return self.get_term(hash_key, msg_orig, msg_tnxl)
 
     def split_items(self, message):
         def append_group(tokens, hash_keys, groups, hash_groups):
             if re.search(self.re_space, groups[-1]):
-                tokens.append(groups[: -1])
+                tokens.append(groups[:-1])
                 tokens.append(groups[-1])
-                hash_keys.append(hash_groups[: -1])
+                hash_keys.append(hash_groups[:-1])
                 hash_keys.append("")
             else:
                 tokens.append(groups)
                 hash_keys.append(hash_groups)
             groups = []
             hash_groups = []
             return tokens, hash_keys, groups, hash_groups
@@ -327,15 +342,15 @@
         hash_keys = []
         hash_groups = []
         ix = 0
         while ix < len(message):
             for tok_type in self.types_decl:
                 match = re.match(tok_type[3], message[ix:])
                 if match:
-                    token = message[ix: match.end() + ix]
+                    token = message[ix : match.end() + ix]
                     if token.startswith("# "):
                         token = "N."
                         hash_key = self.get_hash_key(token, tok_type[0])
                         grouped = tok_type[2]
                         ix += 2
                     else:
                         hash_key = self.get_hash_key(token, tok_type[0])
@@ -347,37 +362,38 @@
                 grouped = False
                 for tok_type in self.types_decl:
                     match = re.search(tok_type[3], message[ix:])
                     if match:
                         ii = min(ii, match.start())
                         break
                 tok_type = None
-                token = message[ix: ii + ix]
+                token = message[ix : ii + ix]
                 hash_key = self.get_hash_key(token, False)
                 ix += ii
             if (
-                (re.search(self.re_space, token) or re.search(self.re_space2, token))
-                and not groups
-            ):
+                re.search(self.re_space, token) or re.search(self.re_space2, token)
+            ) and not groups:
                 grouped = False
             if grouped:
                 groups.append(token)
                 hash_groups.append(hash_key)
             else:
                 if groups:
                     tokens, hash_keys, groups, hash_groups = append_group(
-                        tokens, hash_keys, groups, hash_groups)
+                        tokens, hash_keys, groups, hash_groups
+                    )
                 tokens.append(token)
                 if tok_type and tok_type[4] and ix >= len(message):
                     hash_keys.append("")
                 else:
                     hash_keys.append(hash_key)
         if groups:
             tokens, hash_keys, groups, hash_groups = append_group(
-                tokens, hash_keys, groups, hash_groups)
+                tokens, hash_keys, groups, hash_groups
+            )
         return tokens, hash_keys
 
     def get_untransable_token(self, msg_orig):
         for tok_type in self.types_decl:
             if not tok_type[1]:
                 if re.fullmatch(tok_type[3], msg_orig):
                     return msg_orig
@@ -389,50 +405,49 @@
             ix = 0
             while not learn_about and ix < len(hashes_orig):
                 if (
                     (
                         isinstance(hashes_orig[ix], (list, tuple))
                         and not isinstance(hashes_tnxl[ix], (list, tuple))
                     )
-                    or
-                    (
+                    or (
                         not isinstance(hashes_orig[ix], (list, tuple))
                         and isinstance(hashes_tnxl[ix], (list, tuple))
                     )
-                    or
-                    (
+                    or (
                         isinstance(hashes_orig[ix], (list, tuple))
                         and isinstance(hashes_tnxl[ix], (list, tuple))
                         and (
                             len(hashes_orig[ix]) != len(hashes_tnxl[ix])
                             or any(
                                 [
-                                    (len(hashes_orig[ix][x]) > 2
-                                     and hashes_orig[ix][x] != hashes_tnxl[ix][x]
-                                     and not self.isfullupper(hashes_orig[ix][x]))
+                                    (
+                                        len(hashes_orig[ix][x]) > 2
+                                        and hashes_orig[ix][x] != hashes_tnxl[ix][x]
+                                        and not self.isfullupper(hashes_orig[ix][x])
+                                    )
                                     for x in range(len(hashes_orig[ix]))
-                                ])
+                                ]
+                            )
                         )
                     )
                 ):
                     learn_about = True
                 ix += 1
         return learn_about
 
     def get_transated_tokens(self, tok_orig, module=None, adjust_case=None):
-        hkey_orig = self.get_hash_key(
-            "".join(tok_orig), True, module=module)
+        hkey_orig = self.get_hash_key("".join(tok_orig), True, module=module)
         if hkey_orig in self.dict:
             return (
                 self.get_term(
-                    hkey_orig,
-                    "".join(tok_orig),
-                    None,
-                    adjust_case=adjust_case),
-                hkey_orig)
+                    hkey_orig, "".join(tok_orig), None, adjust_case=adjust_case
+                ),
+                hkey_orig,
+            )
         return False, False
 
     def process_transable_tokens(self, tok_orig, hash_orig, tok_tnxl, adjust_case=None):
         term_tnxl = ""
         hash_key = ""
         ix = 0
         while ix < len(tok_orig):
@@ -447,29 +462,36 @@
             else:
                 term_tnxl += tok_tnxl[ix]
                 hash_key += hash_orig[ix]
             ix += 1
         return term_tnxl, hash_key
 
     def do_dict_item(
-        self, msg_orig, msg_tnxl, action=None, override=None, module=None, is_tag=None,
+        self,
+        msg_orig,
+        msg_tnxl,
+        action=None,
+        override=None,
+        module=None,
+        is_tag=None,
     ):
         if not msg_orig:
             return msg_orig
         action = action or ("build_dict" if override else "translate")
         if self.get_untransable_token(msg_orig):
             return msg_orig
         if not msg_tnxl:
             msg_tnxl = msg_orig
         msg_orig = msg_orig.replace("’", "'")
         msg_tnxl = msg_tnxl.replace("’", "'")
         tokens_orig, hashes_orig = self.split_items(msg_orig)
         tokens_tnxl, hashes_tnxl = self.split_items(msg_tnxl)
-        learn_about = True if is_tag else self.check_if_transable(
-            hashes_orig, hashes_tnxl)
+        learn_about = (
+            True if is_tag else self.check_if_transable(hashes_orig, hashes_tnxl)
+        )
         fullterm_orig = fullterm_tnxl = fulltermhk_orig = fulltermhk_tnxl = ""
         fullterm_2_store = False
         hash_key = ""
         hash_key_orig = "".join(
             ["".join(x) if isinstance(x, (list, tuple)) else x for x in hashes_orig]
         )
         if module:
@@ -482,23 +504,31 @@
         while (tok_orig or tok_tnxl) and (action == "build_dict" or not learn_about):
             if isinstance(tok_orig, (list, tuple)):
                 term_orig = "".join(tok_orig)
                 term_tnxl = "".join(tok_tnxl)
                 term_hkey = "".join(hash_orig)
                 if not learn_about:
                     term_tnxl, term_hkey = self.get_transated_tokens(
-                        tok_orig, module=module, adjust_case=adjust_case)
+                        tok_orig, module=module, adjust_case=adjust_case
+                    )
                     if not term_tnxl:
                         term_tnxl, term_hkey = self.process_transable_tokens(
-                            tok_orig, hash_orig, tok_tnxl, adjust_case=adjust_case)
-                if learn_about or (action == "build_dict"
-                                   and term_tnxl != "".join(tok_orig)):
+                            tok_orig, hash_orig, tok_tnxl, adjust_case=adjust_case
+                        )
+                if learn_about or (
+                    action == "build_dict" and term_tnxl != "".join(tok_orig)
+                ):
                     self.store_1_item(
-                        term_hkey, term_orig, term_tnxl,
-                        override=override, module=module, is_tag=is_tag)
+                        term_hkey,
+                        term_orig,
+                        term_tnxl,
+                        override=override,
+                        module=module,
+                        is_tag=is_tag,
+                    )
                     fullterm_2_store = True
 
                 hash_key += term_hkey
                 fullterm_orig += term_orig
                 fulltermhk_orig = fullterm_orig
                 fullterm_tnxl += term_tnxl
                 fulltermhk_tnxl = fullterm_tnxl
@@ -534,44 +564,54 @@
             fullterm_2_store = True
             fulltermhk_orig = hash_key = hash_key_orig
 
         if self.get_untransable_token(fullterm_orig):
             return fullterm_orig
 
         if action == "build_dict":
-            if not is_tag and (fullterm_orig.lower() == fullterm_tnxl.lower()
-                               or not fullterm_tnxl):
+            if not is_tag and (
+                fullterm_orig.lower() == fullterm_tnxl.lower() or not fullterm_tnxl
+            ):
                 if self.ts and not re.search(self.re_tag, fullterm_orig):
                     try:
                         # Use Google translator
                         fullterm_tnxl = self.adjust_case(
                             fullterm_orig,
-                            self.ts.google(fullterm_orig,
-                                           from_language='en',
-                                           to_language=self.opt_args.lang[:2],
-                                           timeout=5))
+                            self.ts.google(
+                                fullterm_orig,
+                                from_language="en",
+                                to_language=self.opt_args.lang[:2],
+                                timeout=5,
+                            ),
+                        )
                         sleep(0.2)
                         return self.store_1_item(
-                            hash_key, fullterm_orig, fullterm_tnxl, override=override)
+                            hash_key, fullterm_orig, fullterm_tnxl, override=override
+                        )
                     except BaseException:
                         pass
             elif (fullterm_orig and fullterm_2_store) or self.isplural(fulltermhk_orig):
                 return self.store_1_item(
-                    hash_key, fullterm_orig,
+                    hash_key,
+                    fullterm_orig,
                     fullterm_tnxl.replace(
                         fulltermhk_tnxl,
                         self.set_plural_if(
-                            hash_key, fulltermhk_orig, fulltermhk_tnxl,
-                            adjust_case=not is_tag)),
+                            hash_key,
+                            fulltermhk_orig,
+                            fulltermhk_tnxl,
+                            adjust_case=not is_tag,
+                        ),
+                    ),
                     override=override,
                     module=module,
-                    is_tag=is_tag)
+                    is_tag=is_tag,
+                )
         elif fullterm_2_store or (
-            fullterm_tnxl == fulltermhk_tnxl
-            and hash_key in self.dict
+            fullterm_tnxl == fulltermhk_tnxl and hash_key in self.dict
         ):
             return self.get_term(hash_key, fullterm_orig, fullterm_tnxl)
         return fullterm_tnxl
 
     def translate_item(self, msg_orig, msg_tnxl, module=None):
         return self.do_dict_item(msg_orig, msg_tnxl, action="translate", module=module)
 
@@ -608,48 +648,46 @@
                 if left_lines[left_ix] == right_lines[right_ix]:
                     return left_ix, right_ix, True
                 left_ix = saved_ix
             return left_ix, right_ix, False
 
         def find_diff(left_lines, right_lines, left_ix, right_ix):
             while left_ix < len(left_lines) and right_ix < len(right_lines):
-                if (
-                    left_lines[left_ix] == right_lines[right_ix]
-                    or (
-                        re.match(r"^\".*\"$", left_lines[left_ix])
-                        and re.match(r"^\".*\"$", right_lines[right_ix]))):
+                if left_lines[left_ix] == right_lines[right_ix] or (
+                    re.match(r"^\".*\"$", left_lines[left_ix])
+                    and re.match(r"^\".*\"$", right_lines[right_ix])
+                ):
                     left_ix += 1
                     right_ix += 1
                     continue
                 elif re.match(r"^\".*\"$", left_lines[left_ix]):
                     left_ix += 1
                     continue
                 elif re.match(r"^\".*\"$", right_lines[right_ix]):
                     right_ix += 1
                     continue
 
                 if left_lines[left_ix].startswith("#:"):
                     break
 
                 left_ix, right_ix, equals = try_to_sync(
-                    left_lines, right_lines, left_ix, right_ix)
+                    left_lines, right_lines, left_ix, right_ix
+                )
                 if equals:
                     continue
 
-                if (
-                    left_lines[left_ix].startswith("msgid")
-                    and right_lines[right_ix].startswith("msgid")
-                ):
+                if left_lines[left_ix].startswith("msgid") and right_lines[
+                    right_ix
+                ].startswith("msgid"):
                     right_ix += 1
                     left_ix += 1
                     continue
-                if (
-                    left_lines[left_ix].startswith("msgstr")
-                    and right_lines[right_ix].startswith("msgstr")
-                ):
+                if left_lines[left_ix].startswith("msgstr") and right_lines[
+                    right_ix
+                ].startswith("msgstr"):
                     right_ix += 1
                     left_ix += 1
                     continue
                 break
             return left_ix, right_ix
 
         if os.path.isfile(po_fn):
@@ -663,92 +701,94 @@
             except BaseException as e:
                 print("Error %s reading po file %s" % (e, po_fn))
                 return
             for message in catalog:
                 if not message.id:
                     continue
                 message.string = self.translate_item(
-                    message.id, message.string, module=module)
+                    message.id, message.string, module=module
+                )
 
-            pofile.write_po(open(tmp_file, 'wb'),
-                            catalog,
-                            include_previous=True)
+            pofile.write_po(open(tmp_file, "wb"), catalog, include_previous=True)
             with open(filename, "r") as fd:
                 left_lines = fd.read().split("\n")
             with open(tmp_file, "r") as fd:
                 right_lines = fd.read().split("\n")
             updated = False
             left_ix = right_ix = 0
             while left_ix < len(left_lines):
                 left_ix, right_ix = find_diff(
-                    left_lines, right_lines, left_ix, right_ix)
+                    left_lines, right_lines, left_ix, right_ix
+                )
                 if left_ix >= len(left_lines):
                     break
-                if (right_ix < len(right_lines)
+                if (
+                    right_ix < len(right_lines)
                     and left_lines[left_ix].startswith("#:")
-                    and (not right_lines[right_ix].startswith("#:")
-                         or left_lines[left_ix].split(":")[1]
-                         !=
-                         right_lines[right_ix].split(":")[1])):
+                    and (
+                        not right_lines[right_ix].startswith("#:")
+                        or left_lines[left_ix].split(":")[1]
+                        != right_lines[right_ix].split(":")[1]
+                    )
+                ):
                     updated = True
                     right_lines.insert(right_ix, left_lines[left_ix])
                 else:
                     saved_ix = left_ix
                     left_ix, right_ix, equals = try_to_sync(
-                        left_lines, right_lines, left_ix, right_ix)
+                        left_lines, right_lines, left_ix, right_ix
+                    )
                     if left_ix != saved_ix:
                         left_ix = saved_ix
                         updated = True
                         right_lines.insert(right_ix, left_lines[left_ix])
                 left_ix += 1
                 right_ix += 1
 
-            LAST_TNL_NAME = 'Antonio M. Vigliotti'
-            LAST_TNL_MAIL = 'antoniomaria.vigliotti@gmail.com'
-            LAST_TEAM_NAME = 'Zeroincombenze'
-            LAST_TEAM_URL = 'https://www.zeroincombenze.it'
+            LAST_TNL_NAME = "Antonio M. Vigliotti"
+            LAST_TNL_MAIL = "antoniomaria.vigliotti@gmail.com"
+            LAST_TEAM_NAME = "Zeroincombenze"
+            LAST_TEAM_URL = "https://www.zeroincombenze.it"
             LANGUAGE = r'"Language: it_IT\n"'
             PLURALS = r'"Plural-Forms: nplurals=2; plural=(n != 1);\n"'
             lang_it_lineno = False
             plurals_lineno = False
             for lineno, line in enumerate(right_lines):
-                if re.match(r"^#\s+\*",  line):
+                if re.match(r"^#\s+\*", line):
                     right_lines[lineno] = r"# * %s" % module
-                elif line.startswith('#. module:'):
+                elif line.startswith("#. module:"):
                     right_lines[lineno] = r"#. module: %s" % module
-                elif (
-                    self.opt_args.odoo_branch
-                    and line.startswith('"Project-Id-Version:')
+                elif self.opt_args.odoo_branch and line.startswith(
+                    '"Project-Id-Version:'
                 ):
                     right_lines[lineno] = (
-                        r'"Project-Id-Version: Odoo (%s)\n"'
-                        % self.opt_args.odoo_branch
+                        r'"Project-Id-Version: Odoo (%s)\n"' % self.opt_args.odoo_branch
                     )
                 elif line.startswith('"Last-Translator:'):
-                    right_lines[lineno] = (
-                        r'"Last-Translator: %s <%s>\n"'
-                        % (LAST_TNL_NAME, LAST_TNL_MAIL)
+                    right_lines[lineno] = r'"Last-Translator: %s <%s>\n"' % (
+                        LAST_TNL_NAME,
+                        LAST_TNL_MAIL,
                     )
                 elif line.startswith('"Language-Team:'):
-                    right_lines[lineno] = (
-                        r'"Language-Team: %s (%s)\n"'
-                        % (LAST_TEAM_NAME, LAST_TEAM_URL)
+                    right_lines[lineno] = r'"Language-Team: %s (%s)\n"' % (
+                        LAST_TEAM_NAME,
+                        LAST_TEAM_URL,
                     )
                     if not lang_it_lineno:
                         lang_it_lineno = lineno
                     if not plurals_lineno:
                         plurals_lineno = lineno
                 elif line.startswith('"Language:'):
                     right_lines[lineno] = LANGUAGE
                     lang_it_lineno = -1
                 elif line.startswith('"Plural-Forms:'):
                     right_lines[lineno] = PLURALS
                     plurals_lineno = -1
                 elif (
-                    line.startswith('#')
+                    line.startswith("#")
                     and lineno > 0
                     and right_lines[lineno] == right_lines[lineno - 1]
                 ):
                     del right_lines[lineno]
                     lineno -= 1
             if plurals_lineno and plurals_lineno >= 0:
                 right_lines.insert(plurals_lineno, PLURALS)
@@ -771,18 +811,17 @@
                 catalog = pofile.read_po(open(po_fn, "r"))
             except BaseException as e:
                 print("Error %s reading po file %s" % (e, po_fn))
                 return
             for message in catalog:
                 if not message.id:
                     continue
-                self.do_dict_item(message.id,
-                                  message.string,
-                                  action="build_dict",
-                                  override=override)
+                self.do_dict_item(
+                    message.id, message.string, action="build_dict", override=override
+                )
 
     def load_terms_from_xlsx(self, dict_fn):
         if os.path.isfile(dict_fn):
             if self.opt_args.verbose:
                 print("Loading terms from %s" % dict_fn)
             wb = load_workbook(dict_fn)
             sheet = wb.active
@@ -798,29 +837,35 @@
                 for ncol, cell in enumerate(nrow):
                     row[colnames[ncol]] = (
                         cell.value.replace("\\n", "\n") if cell.value else cell.value
                     )
                 if not row["msgid"] or not row["msgstr"]:
                     continue
                 if self.opt_args.verbose:
-                    msg_burst('%s ...' % row["msgid"])
+                    msg_burst("%s ..." % row["msgid"])
                 if "hashkey" in row and row["hashkey"]:
                     if row["hashkey"] not in self.dict:
                         self.dict[row["hashkey"]] = (row["msgid"], row["msgstr"])
                 else:
-                    self.do_dict_item(row["msgid"],
-                                      row["msgstr"],
-                                      action="build_dict",
-                                      module=row["module"])
+                    self.do_dict_item(
+                        row["msgid"],
+                        row["msgstr"],
+                        action="build_dict",
+                        module=row["module"],
+                    )
 
     def load_terms_for_test(self):
         for items in TEST_DATA:
             self.do_dict_item(
-                items[0], items[1], action="build_dict", module=items[2],
-                override=items[4] if len(items) > 4 else None)
+                items[0],
+                items[1],
+                action="build_dict",
+                module=items[2],
+                override=items[4] if len(items) > 4 else None,
+            )
 
     def do_work_on_path(self, root, base, action=None):
         action = action or "translate"
         path = os.path.join(root, base) if base else root
         if self.ismodule(path):
             i18n_path = os.path.join(path, "i18n")
             po_fn = os.path.join(i18n_path, "%s.po" % self.opt_args.lang)
@@ -836,75 +881,75 @@
             elif action == "translate":
                 self.translate_pofile(po_fn)
             else:
                 raise
 
     def build_alias_dict(self):
         self.tags = []
-        for (msg_orig, msg_tnxl, is_tag) in (
+        for msg_orig, msg_tnxl, is_tag in (
             ("I", "io", True),
             ("a", "un", False),
             ("iva", "IVA", True),
             ("sepa", "SEPA", True),
             ("UE", "EU", True),
             ("iban", "IBAN", True),
             ("Ri.Ba.", "RiBA", True),
             ("Ri.Ba", "RiBA", True),
             ("RI.BA.", "RiBA", True),
             ("DDT", "DdT", True),
             ("ddt", "DdT", True),
         ):
-            self.do_dict_item(msg_orig,
-                              msg_tnxl,
-                              action="build_dict",
-                              is_tag=is_tag)
+            self.do_dict_item(msg_orig, msg_tnxl, action="build_dict", is_tag=is_tag)
 
     def build_dict(self):
         if self.opt_args.database and self.opt_args.file_xlsx:
             self.load_terms_from_xlsx(self.opt_args.file_xlsx)
         elif not self.opt_args.module_name:
             target_path = os.path.abspath(self.opt_args.target_path)
             self.do_work_on_path(target_path, None)
-            for root, dirs, files in os.walk(target_path,
-                                             topdown=True,
-                                             followlinks=False):
+            for root, dirs, files in os.walk(
+                target_path, topdown=True, followlinks=False
+            ):
                 dirs[:] = [
                     d
                     for d in dirs
                     if d not in (".git", "__to_remove", "doc", "setup", ".idea")
                 ]
                 for base in dirs:
                     self.do_work_on_path(root, base, action="build_dict")
 
     def install_lang(self, lang, ctx):
-        model = 'res.lang'
+        model = "res.lang"
         vals = {
-            'lang': lang,
+            "lang": lang,
         }
-        ids = clodoo.searchL8(ctx, model, [('code', '=', lang)])
+        ids = clodoo.searchL8(ctx, model, [("code", "=", lang)])
+        force = False
         if not ids:
             if self.opt_args.verbose:
-                print('Language %s not installed: installing it now' % lang)
-            id = clodoo.createL8(ctx, 'base.language.install', vals)
-            clodoo.executeL8(ctx, 'base.language.install', 'lang_install', [id])
+                print("Language %s not installed: installing it now" % lang)
+            id = clodoo.createL8(ctx, "base.language.install", vals)
+            clodoo.executeL8(ctx, "base.language.install", "lang_install", [id])
             clodoo.writeL8(ctx, "res.users", ctx["user_id"], {"lang": lang})
+            force = True
         elif self.opt_args.verbose:
-            print('Found language %s' % lang)
-        if not clodoo.searchL8(ctx, "ir.translation", [("lang", "=", lang)]):
+            print("Found language %s" % lang)
+        if force or not clodoo.searchL8(ctx, "ir.translation", [("lang", "=", lang)]):
             if self.opt_args.verbose:
-                print('No term found for language %s: loading translation' % lang)
-            id = clodoo.createL8(ctx, 'base.update.translations', vals)
-            clodoo.executeL8(ctx, 'base.update.translations', 'act_update', [id])
+                print("No term found for language %s: loading translation" % lang)
+            id = clodoo.createL8(ctx, "base.update.translations", vals)
+            clodoo.executeL8(ctx, "base.update.translations", "act_update", [id])
 
     def connect_db(self, database):
         try:
             uid, ctx = clodoo.oerp_set_env(
                 confn=self.opt_args.config,
                 db=database,
-                oe_version=self.opt_args.odoo_branch)
+                oe_version=self.opt_args.odoo_branch,
+            )
         except BaseException:
             print("No DB %s found" % self.opt_args.database)
             ctx = None
         return ctx
 
     def translate_db(self):
         # ir.translation contains Odoo translation terms
@@ -931,16 +976,18 @@
                     ("lang", "=", self.opt_args.lang),
                     ("src", "=", term.src),
                     ("type", "=", term.type),
                     ("name", "=", term.name),
                     ("module", "=", term.module),
                 ]
                 term_tnl = clodoo.browseL8(
-                    ctx, model_translation, clodoo.searchL8(
-                        ctx, model_translation, domain))
+                    ctx,
+                    model_translation,
+                    clodoo.searchL8(ctx, model_translation, domain),
+                )
                 if len(term_tnl):
                     term_tnl = term_tnl[0]
             value = self.translate_item(term.src, term.value)
             if not term_tnl:
                 if value != term.value:
                     vals = {
                         "lang": self.opt_args.lang,
@@ -950,32 +997,37 @@
                     }
                     for name in ("src", "source", "type", "name", "module"):
                         vals[name] = term[name]
                     clodoo.createL8(ctx, model_translation, vals)
                     ctr_write += 1
             elif value != term_tnl.value:
                 try:
-                    clodoo.writeL8(ctx, model_translation, term.id,
-                                   {"value": value, "state": "translated"})
+                    clodoo.writeL8(
+                        ctx,
+                        model_translation,
+                        term.id,
+                        {"value": value, "state": "translated"},
+                    )
                 except BaseException as e:
-                    print("Error %s for term %s" % (e, term.src))
+                    if term.module == self.opt_args.module_name:
+                        print("Error <%s> for term '%s'" % (e, term.src))
                 ctr_write += 1
             return ctr_write
 
         if not os.path.isfile(self.opt_args.config):
             print("File %s not found!" % self.opt_args.config)
             return 1
         ctr_read = ctr_write = 0
         for database in self.opt_args.database.split(","):
             ctx = self.connect_db(database)
             if ctx is None:
                 continue
             ctx["lang"] = self.opt_args.lang
             self.install_lang(self.opt_args.lang, ctx)
-            model_translation = 'ir.translation'
+            model_translation = "ir.translation"
             # model_field = 'ir.model.fields'
             # last_term = ""
             # for field in clodoo.browseL8(
             #     ctx, model_field, clodoo.searchL8(
             #         ctx, model_field, [], order="field_description")):
             #     if field.field_description == last_term:
             #         continue
@@ -988,37 +1040,44 @@
             #     ]
             #     for term in clodoo.browseL8(
             #         ctx, model_translation, clodoo.searchL8(
             #             ctx, model_translation, domain)):
             #         ctr_read += 1
             #         ctr_write += write_term(term)
             for term in clodoo.browseL8(
-                ctx, model_translation, clodoo.searchL8(
-                    ctx, model_translation, [
+                ctx,
+                model_translation,
+                clodoo.searchL8(
+                    ctx,
+                    model_translation,
+                    [
                         # ("type", "!=", "code"),
-                        ('lang', 'in', ['en_US', self.opt_args.lang])])):
+                        ("lang", "in", ["en_US", self.opt_args.lang])
+                    ],
+                ),
+            ):
                 if self.opt_args.verbose:
-                    msg_burst('%s ...' % term.src)
+                    msg_burst("%s ..." % term.src[:60])
                 ctr_read += 1
                 ctr_write += write_term(term)
         if self.opt_args.verbose:
             print("%d records read, %d records written" % (ctr_read, ctr_write))
         return 0
 
     def translate_module(self):
         module = self.opt_args.module_name
         target_path = os.path.abspath(self.opt_args.target_path)
         if module == "OCB" and os.path.isfile(os.path.join(target_path, "odoo-bin")):
             self.do_work_on_path(target_path, None, action="translate")
         elif module == os.path.basename(target_path):
             self.do_work_on_path(target_path, None, action="translate")
         else:
-            for root, dirs, files in os.walk(target_path,
-                                             topdown=True,
-                                             followlinks=False):
+            for root, dirs, files in os.walk(
+                target_path, topdown=True, followlinks=False
+            ):
                 dirs[:] = [
                     d
                     for d in dirs
                     if d not in (".git", "__to_remove", "doc", "setup", ".idea")
                 ]
                 for base in dirs:
                     if module == base:
@@ -1058,15 +1117,15 @@
 
 def main(cli_args=None):
     cli_args = cli_args or sys.argv[1:]
     parser = argparse.ArgumentParser(
         description="Create translation file", epilog="© 2022-2023 by SHS-AV s.r.l."
     )
     parser.add_argument(
-        '-B', '--debug-template', action='store_true', dest='dbg_template'
+        "-B", "--debug-template", action="store_true", dest="dbg_template"
     )
     parser.add_argument(
         "-b",
         "--odoo-branch",
         dest="odoo_branch",
         default="12.0",
         help="Default Odoo version",
@@ -1086,17 +1145,17 @@
     parser.add_argument("-m", "--module-name")
     parser.add_argument("-n", "--dry-run", action="store_true")
     parser.add_argument("-p", "--target-path", help="Local directory")
     parser.add_argument("-q", "--quite", action="store_false")
     parser.add_argument("-T", "--test", action="store_true")
     parser.add_argument("-v", "--verbose", action="count", default=0)
     parser.add_argument("-V", "--version", action="version", version=__version__)
-    parser.add_argument("-W", "--rewrite-xlsx",
-                        action="store_true",
-                        help="Rewrite xlsx file")
+    parser.add_argument(
+        "-W", "--rewrite-xlsx", action="store_true", help="Rewrite xlsx file"
+    )
     parser.add_argument("-x", "--file-xlsx", help="Default dictionary")
 
     odoo_tnxl = OdooTranslation(parser.parse_args(cli_args))
     if odoo_tnxl.opt_args.test:
         odoo_tnxl.load_terms_for_test()
     elif odoo_tnxl.opt_args.file_xlsx or odoo_tnxl.opt_args.target_path:
         odoo_tnxl.build_dict()
```

### Comparing `wok_code-2.0.8/wok_code/scripts/odoo_dependencies.py` & `wok_code-2.0.9/wok_code/scripts/odoo_dependencies.py`

 * *Files 1% similar despite different names*

```diff
@@ -105,15 +105,15 @@
 except ImportError:
     from z0lib import z0lib
 try:
     from clodoo import clodoo
 except ImportError:
     import clodoo
 
-__version__ = '2.0.8'
+__version__ = '2.0.9'
 
 
 MANIFEST_FILES = ['__manifest__.py', '__odoo__.py', '__openerp__.py', '__terp__.py']
 MAX_DEEP = 20
 UNDEF_DEEP = MAX_DEEP + 5
 MISSED = 99
 
@@ -254,18 +254,29 @@
     if len(filtered) == 2 and '__init__.py' in filtered:
         return os.path.join(path, next(x for x in filtered if x != '__init__.py'))
     else:
         return False
 
 
 def read_manifest(manifest_path):
-    try:
-        manifest = ast.literal_eval(open(manifest_path).read())
-    except (IOError, ImportError):
-        raise Exception('Wrong manifest file %s' % manifest_path)
+    with open(manifest_path, "r") as fd:
+        # sometimes manifest contains BOM so we use encode() to assure right contents
+        if sys.version_info[0] == 2:
+            manifest_content = fd.read()
+        else:
+            manifest_content = fd.read().encode("utf-8")
+        try:
+            manifest = ast.literal_eval(manifest_content)
+        except BaseException:
+            manifest = None
+        if not manifest:
+            try:
+                manifest = eval(manifest_content)
+            except BaseException:
+                raise Exception('Wrong manifest file %s' % manifest_path)
     return manifest
 
 
 def read_valid_manifest(manifest_path, depends_by=None, ao_list=None):
     ao_list = ao_list or '|'
     manifest = read_manifest(manifest_path)
     if not manifest.get('installable', True):
```

### Comparing `wok_code-2.0.8/wok_code/scripts/license_mgnt.py` & `wok_code-2.0.9/wok_code/scripts/license_mgnt.py`

 * *Files 27% similar despite different names*

```diff
@@ -5,90 +5,90 @@
 
 try:
     from python_plus.python_plus import _u
 except ImportError:
     from python_plus import _u
 
 COPY = {
-    'zero': {
-        'author': 'SHS-AV s.r.l.',
-        'website': 'https://www.zeroincombenze.it',
-        'devman': 'Antonio M. Vigliotti <antoniomaria.vigliotti@gmail.com>',
-        'github-user': 'zeroincombenze',
-    },
-    'shs': {
-        'author': 'SHS-AV s.r.l.',
-        'website': 'https://www.shs-av.com',
-        'devman': 'Antonio M. Vigliotti <antoniomaria.vigliotti@gmail.com>',
-        'github-user': 'zeroincombenze',
-    },
-    'oca': {
-        'author': 'Odoo Community Association (OCA)',
-        'website': 'https://odoo-community.org',
-        'github-user': 'OCA',
-    },
-    'powerp': {
-        'author': 'powERP enterprise network',
-        'website': 'https://www.powerp.it',
-        'devman': 'powERP enterprise network',
-        'github-user': 'PowERP-cloud',
-    },
-    'librerp': {
-        'author': 'LibrERP enterprise network',
-        'website': 'https://www.librerp.it',
-        'devman': 'LibrERP enterprise network',
-        'github-user': 'LibrERP-network',
-    },
-    'didotech': {
-        'author': 'Didotech s.r.l.',
-        'website': 'https://www.didotech.com',
-        'github-user': 'iw3hxn',
+    "zero": {
+        "author": "SHS-AV s.r.l.",
+        "website": "https://www.zeroincombenze.it",
+        "devman": "Antonio M. Vigliotti <antoniomaria.vigliotti@gmail.com>",
+        "github-user": "zeroincombenze",
+    },
+    "shs": {
+        "author": "SHS-AV s.r.l.",
+        "website": "https://www.shs-av.com",
+        "devman": "Antonio M. Vigliotti <antoniomaria.vigliotti@gmail.com>",
+        "github-user": "zeroincombenze",
+    },
+    "oca": {
+        "author": "Odoo Community Association (OCA)",
+        "website": "https://odoo-community.org",
+        "github-user": "OCA",
+    },
+    "powerp": {
+        "author": "powERP enterprise network",
+        "website": "https://www.powerp.it",
+        "devman": "powERP enterprise network",
+        "github-user": "PowERP-cloud",
+    },
+    "librerp": {
+        "author": "LibrERP enterprise network",
+        "website": "https://www.librerp.it",
+        "devman": "LibrERP enterprise network",
+        "github-user": "LibrERP-network",
+    },
+    "didotech": {
+        "author": "Didotech s.r.l.",
+        "website": "https://www.didotech.com",
+        "github-user": "iw3hxn",
     },
 }
-ALIAS = {'shs-av': 'shs', 'zeroincombenze': 'zero'}
+ALIAS = {"shs-av": "shs", "zeroincombenze": "zero"}
 
 
 class License:
     def __init__(self, path=None):
         self.org_ids = {}
         self.authors = {}
         self.contributors = {}
         self.cur_year = datetime.today().year
-        path = path or '.'
-        author_file = os.path.join(path, 'egg-info', 'authors.txt')
+        path = path or "."
+        author_file = os.path.join(path, "egg-info", "authors.txt")
         if not os.path.isfile(author_file):
-            author_file = os.path.join(path, 'readme', 'AUTHORS.rst')
+            author_file = os.path.join(path, "readme", "AUTHORS.rst")
         if os.path.isfile(author_file):
             self.parse_file(author_file)
-        author_file = os.path.join(path, 'egg-info', 'contributors.txt')
+        author_file = os.path.join(path, "egg-info", "contributors.txt")
         if not os.path.isfile(author_file):
-            author_file = os.path.join(path, 'readme', 'CONTRIBUTORS.rst')
+            author_file = os.path.join(path, "readme", "CONTRIBUTORS.rst")
         if os.path.isfile(author_file):
             self.parse_file(author_file)
-        author_file = os.path.join(path, 'egg-info', 'acknowledges.txt')
+        author_file = os.path.join(path, "egg-info", "acknowledges.txt")
         if os.path.isfile(author_file):
             self.parse_file(author_file)
 
     def add_copyright(self, org_id, name, website, email, years):
         if org_id and org_id not in self.org_ids:
             if org_id in COPY:
                 if not name:
-                    name = COPY[org_id]['author']
+                    name = COPY[org_id]["author"]
                 if not website:
-                    website = COPY[org_id]['website']
+                    website = COPY[org_id]["website"]
             self.org_ids[org_id] = [name, website, email, years]
         elif email and email not in self.contributors:
             self.contributors[email] = [name, email, years]
         elif name and name not in self.authors:
             self.authors[name] = [name, website, years]
         self.purge_duplicate()
 
     def parse_file(self, author_file):
-        with open(author_file, 'r') as fd:
-            for line in _u(fd.read().split('\n')):
+        with open(author_file, "r") as fd:
+            for line in _u(fd.read().split("\n")):
                 self.add_copyright(*self.extract_info_from_line(line))
 
     def purge_duplicate(self):
         for name in self.authors.copy().keys():
             website = self.authors[name][1]
             for org_id in self.org_ids.keys():
                 if (
@@ -107,122 +107,122 @@
     def extract_info_from_line(self, line):
         """ "Return org_id, name, website, email, years from line"""
 
         def from_rst_line(line):
             org_id = False
             website = False
             email = False
-            ii = line.find('<')
-            jj = line.find('>')
+            ii = line.find("<")
+            jj = line.find(">")
             if ii == -1 and jj == -1:
-                ii = line.find('(')
-                jj = line.find(')')
+                ii = line.find("(")
+                jj = line.find(")")
             if 0 <= ii < jj and jj >= 0:
                 name = line[0:ii].strip()
                 url = line[ii + 1 : jj]
-                url = url.replace('http:', 'https:')
-                if url.endswith('/'):
+                url = url.replace("http:", "https:")
+                if url.endswith("/"):
                     url = url[0:-1]
-                if '@' in url or url.startswith('https://github.com/'):
+                if "@" in url or url.startswith("https://github.com/"):
                     email = url
                     if not name:
-                        name = ' '.join(
-                            [x.capitalize() for x in email.split('@')[0].split('.')]
+                        name = " ".join(
+                            [x.capitalize() for x in email.split("@")[0].split(".")]
                         )
                 else:
-                    website = '.'.join(os.path.basename(url).split('.')[-2:])
+                    website = ".".join(os.path.basename(url).split(".")[-2:])
                     for kk, item in COPY.items():
-                        if item['website'].endswith(website):
+                        if item["website"].endswith(website):
                             org_id = kk
-                            website = item['website']
-                            name = item['author']
+                            website = item["website"]
+                            name = item["author"]
                             break
                     if not org_id:
                         org_id = website
                         org_id = ALIAS.get(org_id, org_id)
                         COPY[org_id] = {
-                            'website': 'http://%s' % website,
-                            'author': name,
+                            "website": "http://%s" % website,
+                            "author": name,
                         }
             else:
                 name = line
-            return org_id, name, website, email, ''
+            return org_id, name, website, email, ""
 
         def from_comment_line(line):
-            head = r'^ *([Cc]opyright|\([Cc]\)|©)'
-            rex = '%s%s' % (head[0:-1], r'|http:|https:|\w+\@[a-zA-z0-9-.]+)')
+            head = r"^ *([Cc]opyright|\([Cc]\)|©)"
+            rex = "%s%s" % (head[0:-1], r"|http:|https:|\w+\@[a-zA-z0-9-.]+)")
             org_id = False
             name = False
             website = False
             email = False
-            years = ''
+            years = ""
             if re.match(rex, line):
                 ipos = 1
-                loom = re.match(r'^ *([Cc]opyright|\([Cc]\)|©)', line)
+                loom = re.match(r"^ *([Cc]opyright|\([Cc]\)|©)", line)
                 if loom:
                     ipos += loom.end() + 1
-                    loom = re.match('^ *[0-9]+', line[ipos:])
+                    loom = re.match("^ *[0-9]+", line[ipos:])
                     if loom:
                         ii = ipos + loom.end()
                         years = line[ipos:ii]
-                        if line[ii] == '-':
+                        if line[ii] == "-":
                             ipos = ii + 1
-                            loom = re.match('[0-9]+', line[ipos:])
+                            loom = re.match("[0-9]+", line[ipos:])
                             if loom:
                                 ii = loom.end()
                                 if ii == 4:
                                     ipos += 2
                                     ii = ipos + ii - 2
                                 else:
                                     ii += ipos
                                 if line[ipos:ii] == str(self.cur_year)[2:]:
-                                    years = '%s-%s' % (years, line[ipos:ii])
+                                    years = "%s-%s" % (years, line[ipos:ii])
                                 else:
-                                    years = '%s-%s' % (years, str(self.cur_year)[-2:])
+                                    years = "%s-%s" % (years, str(self.cur_year)[-2:])
                             elif years != str(self.cur_year):
-                                years = '%s-%s' % (years, str(self.cur_year)[-2:])
+                                years = "%s-%s" % (years, str(self.cur_year)[-2:])
                         elif years != str(self.cur_year):
-                            years = '%s-%s' % (years, str(self.cur_year)[-2:])
+                            years = "%s-%s" % (years, str(self.cur_year)[-2:])
                 org_id, name, website, email, dummy = from_rst_line(line[ipos:].strip())
             return org_id, name, website, email, years
 
-        line = line.replace('`__', '').replace('`', '')
-        if line.startswith('*'):
+        line = line.replace("`__", "").replace("`", "")
+        if line.startswith("*"):
             return from_rst_line(line[1:].strip())
-        elif line.startswith('#'):
+        elif line.startswith("#"):
             return from_comment_line(line[1:].strip())
         return False, False, False, False, False
 
     def summary_authors(self):
-        author = ''
+        author = ""
         if self.org_ids:
-            for org_id in ('oca', 'powerp', 'zero', 'shs', 'didotech'):
+            for org_id in ("oca", "powerp", "zero", "shs", "didotech"):
                 if org_id in self.org_ids:
                     author = self.org_ids[org_id][0]
                     break
             if author and len(self.org_ids) < 3:
                 for org_id in self.org_ids.keys():
                     if self.org_ids[org_id][0] not in author:
-                        author = '%s, %s' % (author, self.org_ids[org_id][0])
+                        author = "%s, %s" % (author, self.org_ids[org_id][0])
             elif author and len(self.org_ids) >= 3:
-                author += ' and other partners'
+                author += " and other partners"
             else:
                 for org_id in self.org_ids.keys():
-                    author = '%s, %s' % (author, self.org_ids[org_id][0])
+                    author = "%s, %s" % (author, self.org_ids[org_id][0])
                 author = author[2:]
         elif self.authors:
             for item in self.authors.keys():
-                author = '%s, %s' % (author, self.authors[item][0])
+                author = "%s, %s" % (author, self.authors[item][0])
             author = author[2:]
         return author
 
     def get_website(self):
-        website = ''
+        website = ""
         if self.org_ids:
-            for org_id in ('oca', 'powerp', 'zero', 'shs', 'didotech'):
+            for org_id in ("oca", "powerp", "zero", "shs", "didotech"):
                 if org_id in self.org_ids:
                     website = self.org_ids[org_id][1]
                     break
         if not website and self.org_ids:
             for item in self.org_ids.keys():
                 website = self.websites[item][1]
                 if website:
@@ -231,28 +231,28 @@
             for item in self.authors.keys():
                 website = self.authors[item][1]
                 if website:
                     break
         return website
 
     def get_maintainer(self):
-        maintainer = ''
+        maintainer = ""
         if self.org_ids:
-            for org_id in ('oca', 'powerp', 'zero', 'shs', 'didotech'):
+            for org_id in ("oca", "powerp", "zero", "shs", "didotech"):
                 if org_id in self.org_ids:
-                    maintainer = COPY[org_id].get('devman', '')
+                    maintainer = COPY[org_id].get("devman", "")
                     if maintainer:
                         break
         return maintainer
 
     def get_license(self, odoo_majver=None):
         odoo_majver = odoo_majver or 12.0
         if odoo_majver <= 8:
-            license = 'agpl'
+            license = "agpl"
         else:
-            if 'oca' in self.org_ids:
-                license = 'lgpl'
-            elif 'powerp' in self.org_ids:
-                license = 'opl'
+            if "oca" in self.org_ids:
+                license = "lgpl"
+            elif "powerp" in self.org_ids:
+                license = "opl"
             else:
-                license = 'lgpl'
+                license = "lgpl"
         return license
```

### Comparing `wok_code-2.0.8/wok_code/scripts/cvt_csv_2_rst.py` & `wok_code-2.0.9/wok_code/scripts/cvt_csv_2_rst.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 
 try:
     from z0lib import z0lib
 except ImportError:
     import z0lib
 
 
-__version__ = "2.0.8"
+__version__ = "2.0.9"
 
 msg_time = time.time()
 
 
 def msg_burst(text):
     global msg_time
     t = time.time() - msg_time
```

### Comparing `wok_code-2.0.8/wok_code/scripts/please.py` & `wok_code-2.0.9/wok_code/scripts/please.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,302 +1,370 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 """NAME
     please - developers shell
 
 SYNOPSIS
-    please [options] action
+    please [options] action [obj]
 
 DESCRIPTION
-    please is an interactive developers shell aim to help development and testing
+    please is an interactive developers shell aims to help development and testing
     software.
 
-    Action is one of:
-
-    * help - show this help or specific action help
-    * create - create some components (currently just apache conf)
-    * install - install some components (currently just python3)
-    * z0bug - execute lint and tests
-    * zerobug - execute lint and tests
+    The parameter action is one of: %(actions)s
+    The optional obj may be on of %(objs)s
 
 OPTIONS
-    -n      Do nothing (dry-run)
+  %(options)s
 
 EXAMPLES
     please help z0bug
 
 BUGS
     No known bugs.
 
-AUTHOR
-    Antonio Maria Vigliotti (antoniomaria.vigliotti@gmail.com)
+SEE ALSO
+    Full documentation at: <https://zeroincombenze-tools.readthedocs.io/>
 """
 import os
 import sys
 import argparse
+import re
+
+# import re
 import itertools
+
 from z0lib import z0lib
 
 try:
-    from please_z0bug import PleaseZ0bug                                   # noqa: F401
+    from please_z0bug import PleaseZ0bug  # noqa: F401
+except ImportError:
+    from .please_z0bug import PleaseZ0bug  # noqa: F401
+try:
+    from please_apache import PleaseApache  # noqa: F401
+except ImportError:
+    from .please_apache import PleaseApache  # noqa: F401
+try:
+    from please_cwd import PleaseCwd  # noqa: F401
 except ImportError:
-    from .please_z0bug import PleaseZ0bug                                  # noqa: F401
+    from .please_cwd import PleaseCwd  # noqa: F401
 try:
-    from please_apache import PleaseApache                                 # noqa: F401
+    from please_python import PleasePython  # noqa: F401
 except ImportError:
-    from .please_apache import PleaseApache                                # noqa: F401
+    from .please_python import PleasePython  # noqa: F401
 
-__version__ = "2.0.8"
+__version__ = "2.0.9"
 
 KNOWN_ACTIONS = [
     "help",
     "chkconfig",
     "config",
-    "docs",
     "duplicate",
-    "edit",
     "export",
     "import",
-    "install",
-    "lint",
     "list",
     "lsearch",
-    "publish",
     "push",
     "pythonhosted",
-    "replace",
     "replica",
-    "test",
-    "translate",
     "version",
-    "wep"
 ]
 
 
 class Please(object):
-
     def __init__(self, cli_args=[]):
         self.clsname = self.__class__.__name__
+        self.cls = self
         self.cli_args = []
         self.store_actions_n_aliases()
-        actions, param, sub1, self.opt_with_help = self.get_no_switches(
-            cli_args=cli_args)
-        self.actions = self.get_actions_list(actions=actions)
-        if param and param in self.knwon_objs:
-            clsname = self.clsname_of_action(param)
+        self.parse_top_cli_args(cli_args=cli_args)
+        if self.objname:
+            clsname = self.clsname_of_param(self.objname)
             if clsname != "Please" and clsname in globals():
                 self.clsname = clsname
-        elif sub1 and sub1 in self.knwon_objs:
-            clsname = self.clsname_of_action(sub1)
-            if clsname != "Please" and clsname in globals():
-                self.clsname = clsname
-        elif (
-            self.actions
-            and len(self.actions) == 1
-            and self.actions[0] in self.knwon_objs
-        ):
-            clsname = self.clsname_of_action(self.actions[0])
-            if clsname != "Please" and clsname in globals():
-                self.clsname = clsname
-            if param:
-                self.actions, param = [param], self.actions[0]
+            self.cls = self.get_cls_of_param(self.objname)
+
+        if not self.actions and self.objname:
+            if hasattr(self.cls, "get_default_action"):
+                self.actions = [getattr(self.cls, "get_default_action")()]
+
         self.main_action = None
-        for action in self.actions:
-            if action not in self.known_actions:
-                print("Unknown action %s" % action)
+        if not self.magic.startswith("-"):
+            if not self.actions and not self.magic:
+                print("No action declared for %s" % self.objname)
                 sys.exit(126)
-            if action == "help":
-                if param in self.known_actions:
-                    self.main_action = param
-            else:
-                self.main_action = action
-
-        self.opt_args = self.get_parser().parse_args([])
-        self.cli_args = cli_args
+            for action in self.actions or [self.magic]:
+                if action not in self.known_actions:
+                    print("Unknown action %s" % action)
+                    sys.exit(126)
+                if action != "help" and not self.objname:
+                    print("Missed object for action %s" % "+".join(self.actions))
+                    if self.main_action:
+                        print(
+                            "Please specify one of %s"
+                            % self.default_obj[self.main_action]
+                        )
+                    sys.exit(126)
+                if not self.main_action:
+                    self.main_action = action
+                    break
+            for action in self.actions:
+                if action != "help" and self.objname not in self.default_obj[action]:
+                    print("Invalid action %s for %s" % (action, self.objname))
+                    sys.exit(126)
+            self.opt_args = self.get_parser().parse_args(self.cli_args)
+            # TODO: workaround due to sub-commands?
+            if self.opt_args.verbose > 1:
+                self.opt_args.verbose -= 1
+        else:
+            self.opt_args = self.get_parser().parse_args(
+                [x for x in self.cli_args if x != self.magic]
+            )
         self.home_devel = self.opt_args.home_devel or os.environ.get(
             "HOME_DEVEL", os.path.expanduser("~/devel")
         )
         self.odoo_root = os.path.dirname(self.home_devel)
         self.pypi_list = self.get_pypi_list(act_tools=False)
         self.sh_subcmd = self.pickle_params()
 
+    def get_actfunctions_of_cls(self, cls, ignore_def=False, ret_action=False):
+        excl = ["do_external_cmd", "do_action_pypipkg", "do_iter_action"]
+        if ignore_def:
+            excl.append("do_action")
+        if ret_action:
+            excl.append("do_help")
+        if sys.version_info[0] == 2:
+            functon_list = [
+                x
+                for x in dir(cls)
+                if x.startswith("do_") and x not in excl and callable(getattr(cls, x))
+            ]
+        else:
+            functon_list = [
+                x
+                for x in cls.__dir__()
+                if x.startswith("do_") and x not in excl and callable(getattr(cls, x))
+            ]
+        if ret_action:
+            return [x[3:] for x in functon_list]
+        return functon_list
+
     def store_actions_n_aliases(self):
+        def store_defult_obj(action, clsname):
+            if action not in self.known_actions:
+                self.known_actions.append(action)
+            if action not in self.default_obj:
+                self.default_obj[action] = []
+            if clsname not in self.default_obj[action]:
+                self.default_obj[action].append(clsname)
+
         self.known_actions = KNOWN_ACTIONS
-        self.knwon_objs = ["cwd"]
+        self.known_objs = []
+        self.default_obj = {}
         self.aliases = {}
         for fn in sorted(os.listdir(os.path.dirname(__file__))):
             if not fn.startswith("please_") or not fn.endswith(".py"):
                 continue
-            action = fn[7: -3]
-            cls = self.get_cls_of_action(action)
+            # module_name = fn[: -3]
+            # clsname = "".join([x[0].upper() + x[1:].lower()
+            #                    for x in module_name.split("_")])
+            # try:
+            #     cls = getattr(__import__(module_name, fromlist=[clsname]), clsname)
+            # except ImportError:
+            #     print("Internal error: file %s is not valid!" % fn)
+            #     continue
+            param = fn[7:-3]
+            cls = self.get_cls_of_param(param)
             clsname = cls.__class__.__name__
             if clsname.startswith("Please"):
                 clsname = clsname[6:].lower()
-                self.knwon_objs.append(clsname)
+                if param != clsname:
+                    print("Invalid configuration %s" % fn)
+                    continue
 
+            self.known_objs.append(param)
             if hasattr(cls, "get_aliases"):
                 for alias in getattr(cls, "get_aliases")():
-                    # for alias in getattr(cls(self), "get_aliases")():
-                    self.aliases[alias] = action
-                    if alias not in self.known_actions:
-                        self.known_actions.append(alias)
+                    self.aliases[alias] = clsname
+                    if alias not in self.known_objs:
+                        self.known_objs.append(alias)
+            action_list = self.get_actfunctions_of_cls(cls, ret_action=True)
+            for action in action_list:
+                store_defult_obj(action, clsname)
             if hasattr(cls, "get_actions"):
                 for action in getattr(cls, "get_actions")():
-                    if action not in self.known_actions:
-                        self.known_actions.append(action)
-            else:
-                self.known_actions.append(action)
+                    store_defult_obj(action, clsname)
 
-    def clsname_of_action(self, action=None):
-        if action == "help":
+    def clsname_of_param(self, param=None):
+        if param == "help":
             return "Please"
-        if action in self.aliases:
-            action = self.aliases[action]
-        return "".join(["Please", action[0].upper(), action[1:].lower()])
+        if param in self.aliases:
+            param = self.aliases[param]
+        return "".join(["Please", param.capitalize()])
 
-    def get_cls_of_action(self, action=None):
-        if not action:
+    def get_cls_of_param(self, param=None):
+        if not param:
             return self
-        clsname = (
-            self.clsname
-            if self.clsname != "Please" else self.clsname_of_action(action)
-        )
-        return self.get_cls_from_clsname(clsname)
+        return self.get_cls_from_clsname(self.clsname_of_param(param))
 
     def get_cls_from_clsname(self, clsname):
         if clsname not in globals() or clsname == "Please":
             return self
         return globals()[clsname](self)
 
-    def get_fctname_of_cls(self, cls, action, param, sub1):
-        def build_fctname_of_cls(cls, params):
+    def build_function_name_of_cls(self, action):
+        def build_valid_name(cls, params):
             if not params:
                 fctname = "do_action"
-                if clsname == "Please" or not hasattr(cls, fctname):
+                if cls == "Please" or not hasattr(cls, fctname):
                     fctname = "do_external_cmd"
             else:
                 parms = []
                 rev_parms = []
                 for param in params:
-                    if param and param != clsname:
-                        parms.append(param)
-                        rev_parms.insert(0, param)
+                    parms.append(param)
+                    rev_parms.insert(0, param)
                 fctname = "do_" + "_".join(parms)
                 if not hasattr(cls, fctname):
                     fctname = "do_" + "_".join(rev_parms)
                 if not hasattr(cls, fctname):
-                    return build_fctname_of_cls(cls, params[: -1])
+                    return build_valid_name(cls, params[:-1])
             return fctname
 
-        clsname = cls.__class__.__name__
-        if clsname.startswith("Please"):
-            clsname = clsname[6:].lower()
         if action == "help":
             return "do_%s" % action
-        if sub1:
-            return build_fctname_of_cls(cls, [action, param, sub1])
-        elif param:
-            return build_fctname_of_cls(cls, [action, param])
-        return build_fctname_of_cls(cls, [action])
-
-    def get_parser(self, action=None):
-        parser = self.common_opts()
-        if action:
-            cls = self.get_cls_of_action(action)
-            if hasattr(cls, "action_opts"):
-                parser = getattr(cls, "action_opts")(parser)
-            else:
-                parser = self.action_opts(parser)
-        else:
-            parser = self.action_opts(parser)
+        if self.sub1:
+            return build_valid_name(self.cls, [action, self.sub1])
+        return build_valid_name(self.cls, [action])
+
+    def get_parser(self, param=None):
+        parser = self.base_opts()
+        param = param or self.objname
+        if param and hasattr(self.cls, "action_opts"):
+            sub_parser = parser.add_subparsers()
+            self.cls.action_opts(sub_parser.add_parser(param))
         return parser
 
-    def merge_action_parser(self, action, cli_args):
-        parser = self.get_parser(action)
-        self.opt_args = parser.parse_args(cli_args)
-
-    def run_traced(self, cmd):
-        if not self.opt_args.dry_run and self.opt_args.verbose:
-            print(">", cmd)
-        return os.system(cmd)
+    def run_traced(self, cmd, disable_output=False, rtime=False):
+        if rtime:
+            if self.opt_args.dry_run:
+                if self.opt_args.verbose:
+                    print("> " + cmd)
+                return 0
+            if self.opt_args.verbose:
+                print("$ " + cmd)
+            return os.system(cmd)
+        sts, stdout, stderr = z0lib.run_traced(
+            cmd, verbose=self.opt_args.verbose, dry_run=self.opt_args.dry_run
+        )
+        if not disable_output:
+            print(stdout + stderr)
+        return sts
+
+    def add_argument(self, parser, arg):
+        if arg in ("-B", "--debug"):
+            parser.add_argument(
+                "-B", "--debug", action="count", default=0, help="debug mode"
+            )
+        elif arg in ("-b", "--odoo-branch", "--branch"):
+            parser.add_argument(
+                "-b",
+                arg if arg != "-b" else "--odoo-branch",
+                metavar="BRANCH",
+                help="default Odoo version",
+            )
+        elif arg in ("-c", "--odoo-config"):
+            parser.add_argument(
+                "-c", "--odoo-config", metavar="FILE", help="Odoo configuration file"
+            )
+        elif arg in ("-d", "--database"):
+            parser.add_argument(
+                "-d", "--database", metavar="NAME", help="Database to manage"
+            )
+        elif arg in ("-f", "--force"):
+            parser.add_argument(
+                "-f",
+                "--force",
+                action="store_true",
+                help=(
+                    "force copy (push) | build (publish/test) | set_exec (wep) |"
+                    " full (status)"
+                ),
+            )
+        elif arg in ("-j", "--python"):
+            parser.add_argument(
+                "-j",
+                "--python",
+                metavar="PYVER",
+                help="Run test with specific python version",
+            )
+        elif arg in ("-l", "--log"):
+            parser.add_argument("-l", "--log", metavar="FILE", help="log file name")
+        elif arg in ("-n", "--dry-run"):
+            parser.add_argument(
+                "-n",
+                "--dry-run",
+                help="do nothing (dry-run)",
+                action="store_true",
+            )
+        elif arg in ("-q", "--quite"):
+            parser.add_argument(
+                "-q",
+                "--quiet",
+                action="store_false",
+                dest="verbose",
+                help="silent mode",
+            )
+        elif arg in ("-v", "--verbose"):
+            parser.add_argument(
+                "-v", "--verbose", help="verbose mode", action="count", default=0
+            )
+        elif arg in ("-y", "--assume-yes"):
+            parser.add_argument("-y", "--assume-yes", action="store_true")
+        else:
+            raise NotImplementedError
 
-    def common_opts(self):
+    def base_opts(self):
         parser = argparse.ArgumentParser(
             formatter_class=argparse.RawDescriptionHelpFormatter,
-            description="Zeroincombenze® developer shell",
+            description=(
+                "Zeroincombenze® developer shell.\n"
+                # "action is one of: " + ", ".join(self.actions) + "\n"
+                "obj after action may be on of "
+                + ", ".join(self.known_objs)
+                + "\n"
+            ),
             epilog=(
                 "Help available issuing: please help ACTION\n"
                 "© 2015-2023 by SHS-AV s.r.l.\n"
                 "Author: antoniomaria.vigliotti@gmail.com\n"
                 "Full documentation at: https://zeroincombenze-tools.readthedocs.io/\n"
             ),
         )
         parser.add_argument(
-            "-B", "--debug", action="count", default=0, help="debug mode"
-        )
-        parser.add_argument(
-            "-b", "--odoo-branch", default="12.0",
-            metavar="BRANCH_OR_VERSION",
-            help="default Odoo version"
+            "-H", "--home-devel", metavar="PATH", help="Home devel directory"
         )
+        self.add_argument(parser, "-n")
         parser.add_argument(
-            "-c", "--odoo-config", metavar="FILE",
-            help="Odoo configuration file"
+            "-Q", "--tools-config", metavar="FILE", help="Configuration file"
         )
-
-        parser.add_argument("-d", "--database", metavar="NAME",)
-        parser.add_argument(
-            "-f",
-            "--force",
-            action="store_true",
-            help=(
-                "force copy (push) | build (publish/test) | set_exec (wep) |"
-                " full (status)"
-            ),
-        )
-        parser.add_argument("-H", "--home-devel",  metavar="PATH",
-                            help="Home devel directory")
-        parser.add_argument("-l", "--log", metavar="FILE", help="log file name")
-        parser.add_argument("-n", "--dry-run", action="store_true")
-        parser.add_argument("-Q", "--tools-config", metavar="FILE",
-                            help="Configuration file")
-        parser.add_argument(
-            "-q", "--quiet", action="store_false", dest="verbose", help="silent mode"
-        )
-        parser.add_argument("-v", "--verbose", action="count", default=0)
+        self.add_argument(parser, "-q")
+        self.add_argument(parser, "-v")
         parser.add_argument("-V", "--version", action="version", version=__version__)
-        parser.add_argument("-y", "--assume-yes", action="store_true")
         parser.add_argument("action", nargs="?")
-        parser.add_argument("param", nargs="?")
-        parser.add_argument("sub1", nargs="?")
-        parser.add_argument("sub2", nargs="?")
-        parser.add_argument("sub3", nargs="?")
         return parser
 
-    def action_opts(self, parser):
-        parser.add_argument("--from-date diff", help="date to search in log")
-        parser.add_argument(
-            "-k",
-            "--keep",
-            action="store_true",
-            help=(
-                "keep coverage statistics in annotate test/keep original repository |"
-                " tests/ in publish"
-            ),
-        )
-        parser.add_argument("-p", "--target-path",  metavar="PATH",
-                            help="Local directory")
-        return parser
-
-    def pickle_params(self, cmd_subst=None):
+    def pickle_params(self, cmd_subst=None, rm_obj=None):
         params = ""
         for arg in self.cli_args:
             if cmd_subst and not arg.startswith("-"):
                 arg = cmd_subst
                 cmd_subst = None
+            if arg == self.objname and rm_obj:
+                continue
             if "<" in arg or ">" in arg:
                 arg = "'%s'" % arg.replace("'", r"\'")
             elif " " in arg:
                 if '"' in arg:
                     arg = '"%s"' % arg.replace('"', r"\"")
                 else:
                     arg = '"%s"' % arg
@@ -305,42 +373,68 @@
             elif "'" in arg:
                 arg = '"%s"' % arg
             else:
                 arg = "%s" % arg
             params += arg + " "
         return params.strip()
 
-    def actions_args(self, action):
-        args = []
-        for arg in self.cli_args:
-            if action and not arg.startswith("-"):
-                args.append(action)
-                action = None
-            else:
-                args.append(arg)
-        return args
-
-    def get_no_switches(self, cli_args=[]):
-        cmd = param = sub1 = ""
-        opt_with_help = False
-        cli_args = cli_args or self.cli_args
+    def parse_top_cli_args(self, cli_args=[]):
+        self.actions = self.objname = self.sub1 = self.magic = ""
+        cli_args = cli_args
         for arg in cli_args:
             if arg.startswith("-"):
                 if arg in ("-h", "--help", "-V", "--version"):
-                    opt_with_help = True
+                    self.magic = arg
             else:
-                if not cmd:
-                    cmd = arg
-                elif not param:
-                    param = arg
+                arg = arg.replace("-", "_")
+                arg0 = self.aliases.get(arg, arg)
+                if arg == "help":
+                    self.magic = self.magic or "help"
+                elif not self.actions and arg0 not in self.known_objs:
+                    self.actions = arg
+                elif not self.objname and arg0 in self.known_objs:
+                    self.objname = arg0
+                elif not self.sub1:
+                    self.sub1 = arg
                 else:
-                    sub1 = arg
-            if (cmd and param and sub1) or (cmd and opt_with_help):
+                    break
+            if (self.actions and self.objname and self.sub1) or (
+                self.actions and self.magic.startswith("-")
+            ):
                 break
-        return cmd, param, sub1, opt_with_help
+        if (
+            self.actions
+            and not self.objname
+            and len(self.default_obj.get(self.actions, [])) == 1
+        ):
+            self.objname = self.default_obj[self.actions][0]
+        if not self.objname and self.sub1 and self.sub1 in self.known_objs:
+            self.objname = self.sub1
+            self.sub1 = ""
+        if not self.magic and not self.actions and not self.objname:
+            self.actions = "help"
+        if self.magic.startswith("-"):
+            self.cli_args = cli_args
+        else:
+            args = []
+            head = True
+            while len(cli_args):
+                arg = cli_args.pop(0)
+                if arg.startswith("-"):
+                    args.append(arg)
+                elif head:
+                    # action is discarded!
+                    args.append(self.actions or self.magic)
+                    if self.objname:
+                        args.append(self.objname)
+                    head = False
+                elif arg != self.objname:
+                    args.append(arg)
+            self.cli_args = args
+        self.actions = self.get_actions_list(self.actions)
 
     def get_home_pypi(self):
         return os.path.join(self.home_devel, "pypi")
 
     def get_home_pypi_pkg(self, pkgname):
         root = self.get_home_pypi()
         if pkgname == "tools":
@@ -349,81 +443,120 @@
             return os.path.join(root, pkgname, pkgname)
 
     def get_home_tools(self):
         return os.path.join(self.odoo_root, "tools")
 
     def get_home_tools_pkg(self, pkgname):
         root = self.get_home_tools()
+        if pkgname == "tools":
+            return root
         return os.path.join(root, pkgname)
 
     def is_pypi_pkg(self, path=None):
         path = path or os.getcwd()
         pkgname = os.path.basename(path)
-        while pkgname in ("tests",
-                          "travis",
-                          "_travis",
-                          "docs",
-                          "examples",
-                          "egg-info",
-                          "junk"):
+        while pkgname in (
+            "tests",
+            "travis",
+            "_travis",
+            "docs",
+            "examples",
+            "egg-info",
+            "junk",
+            "scripts",
+        ):
             path = os.path.dirname(path)
             pkgname = os.path.basename(path)
         pkgpath = self.get_home_pypi_pkg(pkgname)
         root = pkgpath if pkgname == "tools" else os.path.dirname(pkgpath)
         pkgpath2 = self.get_home_tools_pkg(pkgname)
         return (
             os.path.isdir(pkgpath)
             and path.startswith(root)
             and os.path.isfile(os.path.join(root, "setup.py"))
+            and (
+                os.path.isfile(os.path.join(pkgpath, "__init__.py"))
+                or pkgname == "tools"
+            )
         ) or (
             os.path.isdir(pkgpath2)
             and path.startswith(pkgpath2)
-            and os.path.isfile(os.path.join(pkgpath2, "setup.py"))
+            and pkgname == "tools"
+            or (
+                os.path.isfile(os.path.join(pkgpath2, "setup.py"))
+                and os.path.isfile(os.path.join(pkgpath2, "__init__.py"))
+            )
         )
 
     def is_all_pypi(self, path=None):
         path = path or os.getcwd()
         return path == self.get_home_pypi()
 
     def is_odoo_pkg(self, path=None):
         path = path or os.getcwd()
         files = os.listdir(path)
-        filtered = [x for x in files
-                    if x in ("__manifest__.py",  "__openerp__.py", "__init__.py")]
+        filtered = [
+            x
+            for x in files
+            if x in ("__manifest__.py", "__openerp__.py", "__init__.py")
+        ]
         return len(filtered) == 2 and "__init__.py" in filtered
 
     def is_repo_ocb(self, path=None):
         path = path or os.getcwd()
         if (
             os.path.isdir(os.path.join(path, ".git"))
             and (
                 os.path.isfile(os.path.join(path, "odoo-bin"))
                 or os.path.isfile(os.path.join(path, "openerp-server"))
             )
-            and os.path.isfile(os.path.join(path, "__init__.py"))
             and os.path.isdir(os.path.join(path, "addons"))
             and (
                 os.path.isdir(os.path.join(path, "odoo"))
-                or os.path.isdir(os.path.join(path, "openerp"))
-            )
+                and os.path.isfile(os.path.join(path, "odoo", "__init__.py")))
+                or (os.path.isdir(os.path.join(path, "openerp"))
+                    and os.path.isfile(os.path.join(path, "odoo", "__init__.py")))
         ):
             return True
         if os.path.basename(path) in ("addons", "odoo", "openerp"):
             return self.is_repo_ocb(path=os.path.dirname(path))
         return False
 
     def is_repo_odoo(self, path=None):
         path = path or os.getcwd()
         if not os.path.isdir(os.path.join(path, ".git")):
             return False
         for fn in os.listdir(path):
-            if self.is_odoo_pkg(path=os.path.join(path, fn)):
+            subpath = os.path.join(path, fn)
+            if os.path.isdir(subpath) and self.is_odoo_pkg(path=subpath):
                 return True
         return self.is_repo_ocb(os.path.dirname(path))
 
+    def get_odoo_branch_from_git(self, raise_if_not_found=True):
+        branch = ""
+        sts, stdout, stderr = z0lib.run_traced(
+            "git branch", verbose=False, dry_run=False
+        )
+        if sts == 0 and stdout:
+            sts = 1
+            for ln in stdout.split("\n"):
+                if ln.startswith("*"):
+                    branch = ln[2:]
+                    sts = 0
+                    break
+        if sts == 0:
+            x = re.match(r"[0-9]+\.[0-9]+", branch)
+            if not x:
+                if raise_if_not_found:
+                    print("Unrecognized git branch")
+                sts = 1
+        if sts == 0:
+            branch = branch[x.start(): x.end()]
+        return sts, branch
+
     def get_pypi_list(self, path=None, act_tools=True):
         path = path or (
             self.get_home_pypi()
             if os.path.isdir(self.get_home_pypi())
             else self.get_home_tools()
         )
         pypi_list = []
@@ -438,35 +571,38 @@
                     pypi_list.append(fn)
         return sorted(pypi_list)
 
     def get_actions_list(self, actions=None):
         actions = actions.split("+") if actions else ""
         return list(itertools.chain.from_iterable([x.split(",") for x in actions]))
 
-    def build_sh_me_cmd(self, params=None):
-        cmd = "%s.sh" % os.path.splitext(os.path.abspath(__file__))[0]
-        if not os.path.isfile(cmd):
-            cmd = os.path.split(cmd)
-            cmd = os.path.join(os.path.dirname(cmd[0]), cmd[1])
-        if not os.path.isfile(cmd):
-            print("Internal package error: file %s not found!" % cmd)
-            return ""
+    def build_sh_me_cmd(self, cmd=None, params=None):
+        if not cmd:
+            cmd = "%s.sh" % os.path.splitext(os.path.abspath(__file__))[0]
+            if not os.path.isfile(cmd):
+                cmd = os.path.split(cmd)
+                cmd = os.path.join(os.path.dirname(cmd[0]), cmd[1])
+            if not os.path.isfile(cmd):
+                print("Internal package error: file %s not found!" % cmd)
+                return ""
         cmd += " " + (params or self.sh_subcmd)
         return cmd
 
     def do_external_cmd(self):
         cmd = self.build_sh_me_cmd()
         if not cmd:
             return 1
         return self.run_traced(cmd)
 
     def do_action_pypipkg(self, action, pkg, path=None):
         path = path or os.path.join(self.home_devel, "pypi", pkg, pkg)
+        if self.opt_args.verbose:
+            print("$ cd " + path)
         os.chdir(path)
-        return getattr(self, action)
+        return getattr(self.cls, action)()
 
     def do_iter_action(self, action, path=None, act_all_pypi=None, act_tools=None):
         """Iter multiple command on sub projects.
 
         Args:
             action (str): action name to execute
             act_all_pypi (bool): action on all pypi packages
@@ -494,156 +630,97 @@
             return self.run_traced(self.sh_subcmd)
         return 126
 
     ##########################
     # -----  Commands  ----- #
     ##########################
 
-    def travis_opts(self, parser):
-        parser.add_argument(
-            "-A", "--trace-after",
-            metavar="REGEX",
-            help="travis stops after executed yaml statement"
-        )
-        parser.add_argument(
-            "-C", "--no-cache", action="store_true", help="do not use stored PYPI"
-        )
-        parser.add_argument(
-            "-D",
-            "--debug-level",
-            help="travis_debug_mode: may be 0,1,2,3,8 or 9 (def yaml dependents)",
-        )
-        parser.add_argument(
-            "-E", "--no-savenv", action="store_true",
-            help="do not save virtual environment into ~/VME/... if does not exist"
-        )
-        parser.add_argument(
-            "-e", "--locale", help="use locale"
-        )
-        parser.add_argument(
-            "-f",
-            "--full",
-            action="store_true",
-            help="run final travis with full features",
-        )
-        parser.add_argument(
-            "-L",
-            "--lint-level",
-            help=("lint_check_level; may be: "
-                  "minimal,reduced,average,nearby,oca; def value from .travis.yml"),
-        )
-        parser.add_argument(
-            "-m",
-            "--missing",
-            action="store_true",
-            help="show missing line in report coverage after test",
-        )
-        parser.add_argument(
-            "-S", "--syspkg", metavar="true|false",
-            help="use python system packages (def yaml dependents)"
-        )
-        parser.add_argument(
-            "-T", "--trace",
-            metavar="REGEX",
-            help="trace stops before executing yaml statement"
-        )
-        parser.add_argument(
-            "-X", "--translation",
-            metavar="true|false",
-            help="enable translation test (def yaml dependents)"
-        )
-        parser.add_argument(
-            "-Y", "--yaml-file",
-            metavar="PATH",
-            help="file yaml to process (def .travis.yml)"
-        )
-        parser.add_argument(
-            "-Z", "--zero", action="store_true",
-            help="use local zeroincombenze tools"
-        )
-        return parser
-
-    def do_install_python3(self):
-        """
-NAME
-    please install python3 - install a specific python version
-
-SYNOPSIS
-    please install python3 PYTHON3_VERSION
-
-DESCRIPTION
-    This command installs a specific python version on system from source.
-    To install python you must be the root user o you must have the admin
-    privileges.
-
-OPTIONS
-    -n      Do nothing (dry-run)
-
-EXAMPLES
-    please python3 3.9
-
-BUGS
-    No known bugs."""
-        cmd = os.path.join(
-            os.path.dirname(os.path.dirname(os.path.abspath(__file__))),
-            "install_python_3_from_source.sh",
-        )
-        if not os.path.isfile(cmd):
-            print("Internal package error: file %s not found!" % cmd)
-            return 127
-        if not self.opt_args.sub2:
-            print("You must specify the python version: 3.6 or 3.7 or 3.8 or 3.9")
-            return 1
-        cmd += " " + self.opt_args.sub2
-        if self.opt_args.dry_run:
-            z0lib.run_traced(
-                cmd, verbose=self.opt_args.verbose, dry_run=self.opt_args.dry_run
-            )
-            return 0
-        return self.run_traced(cmd)
-
     def do_help(self):
-        cls = self.get_cls_from_clsname(self.clsname)
-        _, param, sub1, _ = self.get_no_switches(cli_args=self.cli_args)
-        action = self.get_fctname_of_cls(cls, param, sub1, None)
-        if hasattr(cls, action):
-            print(getattr(cls, action).__doc__)
-            return 0
-        print(__doc__)
+        actions = set()
+        if not self.objname:
+            for cls in [self.get_cls_of_param(x) for x in self.known_objs]:
+                actions |= set(
+                    [
+                        x.split("_")[0]
+                        for x in self.get_actfunctions_of_cls(
+                            cls, ignore_def=True, ret_action=True
+                        )
+                    ]
+                )
+            cls_doc = ""
+            parser = self.get_parser()
+        else:
+            actions |= set(
+                [
+                    x.split("_")[0]
+                    for x in self.get_actfunctions_of_cls(
+                        self.cls, ignore_def=True, ret_action=True
+                    )
+                ]
+            )
+            cls_doc = self.cls.__doc__
+            parser = self.base_opts()
+            if hasattr(self.cls, "action_opts"):
+                parser = self.cls.action_opts(parser, for_help=True)
+
+        actions = list(actions)
+        action = actions[0] if len(actions) == 1 else None
+        actions = ", ".join(sorted(actions))
+        options = []
+        valid = False
+        for ln in parser.format_help().split("\n"):
+            if ln.startswith("optional"):
+                valid = True
+            elif not ln.startswith(" "):
+                valid = False
+            elif valid:
+                options.append(ln)
+        options = "\n  ".join(options)
+        params = {
+            "actions": actions,
+            "objs": ", ".join(self.known_objs),
+            "options": options,
+        }
+        print(
+            (
+                action
+                and hasattr(self.cls, action)
+                and getattr(self.cls, action).__doc__
+                or cls_doc
+                or __doc__
+            )
+            % params
+        )
         return 0
 
 
 def main(cli_args=[]):
     if not cli_args:
         cli_args = sys.argv[1:]
     please = Please(cli_args)
-    _, param, sub1, _ = please.get_no_switches(cli_args=please.cli_args)
     done = False
-    if not please.opt_with_help:
-        for action in please.actions:
-            cls = please.get_cls_of_action(action)
-            cmd = please.get_fctname_of_cls(cls, action, param, sub1)
-            if hasattr(cls, cmd):
-                please.merge_action_parser(action, please.actions_args(action))
+    if not please.magic.startswith("-"):
+        for action in please.actions or [please.magic]:
+            cmd = please.build_function_name_of_cls(please.magic or action)
+            if hasattr(please.cls, cmd):
                 please.sh_subcmd = please.pickle_params(cmd_subst=action)
-                sts = getattr(cls, cmd)()
-            elif cmd != "do_help" and hasattr(cls, "do_action"):
-                please.merge_action_parser(action, please.actions_args(action))
+                sts = getattr(please.cls, cmd)()
+            elif cmd != "do_help" and hasattr(please.cls, "do_action"):
                 please.sh_subcmd = please.pickle_params(cmd_subst=action)
-                sts = getattr(cls, "do_action")()
+                sts = getattr(please.cls, "do_action")()
             elif hasattr(please, cmd):
                 sts = getattr(please, cmd)()
             else:
                 sts = 126
             if sts:
                 return sts
             done = True
     if not done:
-        if cli_args and please.opt_with_help:
-            please.get_parser(please.main_action).parse_args(cli_args)
+        if cli_args and please.magic.startswith("-"):
+            please.get_parser().parse_args([please.objname, please.magic])
         else:
             please.get_parser().print_help()
     return 0
 
 
 if __name__ == "__main__":
     exit(main())
```

### Comparing `wok_code-2.0.8/wok_code/scripts/do_odoo_site.py` & `wok_code-2.0.9/wok_code/scripts/do_odoo_site.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 import sys
 import os
 import argparse
+
 # import re
 try:
     import ConfigParser
 except ImportError:
     import configparser as ConfigParser
 
 TEMPLATE = """#############################################
@@ -75,19 +76,18 @@
     SSLCertificateKeyFile
     Include /etc/letsencrypt/options-ssl-apache.conf
     SSLCertificateChainFile
 </VirtualHost>
 </IfModule>
 """
 
-__version__ = "2.0.8"
+__version__ = "2.0.9"
 
 
 class CreateConfig(object):
-
     def __init__(self, domain, opt_args):
         self.opt_args = opt_args
         if "." in domain:
             self.domain = domain
         else:
             self.domain = "%s.zeroincombenze.it" % domain
         self.confn = "%s.conf" % self.domain
@@ -101,31 +101,31 @@
             config.read(self.opt_args.odoo_config)
             for param in ("http_port", "xmlrpc_port", "longpolling_port"):
                 if config.has_option("options", param):
                     self.odoo_config[param] = config.getint("options", param)
 
         self.email = "postmaster@%s" % ".".join(self.domain.split(".")[-2:])
         self.site_id = self.domain.split(".")[0]
-        self.odoo_major_version = int(opt_args.odoo_version.split('.')[0])
+        self.odoo_major_version = int(opt_args.odoo_version.split(".")[0])
         if opt_args.http_port:
             self.http_port = opt_args.http_port
         elif self.odoo_config.get("http_port"):
             self.http_port = self.odoo_config["http_port"]
         elif self.odoo_config.get("xmlrpc_port"):
             self.http_port = self.odoo_config["xmlrpc_port"]
         else:
-            self.http_port = (8160 + self.odoo_major_version)
+            self.http_port = 8160 + self.odoo_major_version
         if opt_args.longpolling_port:
             self.http_port = opt_args.longpolling_port
         elif self.odoo_config.get("longpolling_port"):
             self.longport = self.odoo_config["longpolling_port"]
         elif int(self.http_port) >= 19000:
             self.longport = "%s" % (int(self.http_port) - 19000 + 100)
         else:
-            self.longport = (8130 + self.odoo_major_version)
+            self.longport = 8130 + self.odoo_major_version
         params = {
             "domain": self.domain,
             "port": self.http_port,
             "longport": self.longport,
             "email": "%s" % self.email,
         }
         if self.opt_args.https:
@@ -151,25 +151,25 @@
             #     write_file("odoo12-%s.conf" % self.site_id, self.odoo_config)
 
 
 def main(cli_args=None):
     cli_args = cli_args or sys.argv[1:]
     parser = argparse.ArgumentParser(
         description="Create apache config file for Odoo instance",
-        epilog="© 2021-2023 by SHS-AV s.r.l."
+        epilog="© 2021-2023 by SHS-AV s.r.l.",
     )
-    parser.add_argument('-b', '--odoo-version', dest="odoo_version", default="12.0")
-    parser.add_argument('-c', '--odoo-config', dest="odoo_config")
+    parser.add_argument("-b", "--odoo-version", dest="odoo_version", default="12.0")
+    parser.add_argument("-c", "--odoo-config", dest="odoo_config")
     parser.add_argument("-n", "--dry-run", dest="dry_run", action="store_true")
-    parser.add_argument('-l', '--longpolling-port')
-    parser.add_argument('-p', '--http-port', dest="http_port")
-    parser.add_argument('-s', '--https', action="store_true", dest="https")
-    parser.add_argument('-v', '--verbose', action='count', default=0)
-    parser.add_argument('-V', '--version', action="version", version=__version__)
-    parser.add_argument('domain')
+    parser.add_argument("-l", "--longpolling-port")
+    parser.add_argument("-p", "--http-port", dest="http_port")
+    parser.add_argument("-s", "--https", action="store_true", dest="https")
+    parser.add_argument("-v", "--verbose", action="count", default=0)
+    parser.add_argument("-V", "--version", action="version", version=__version__)
+    parser.add_argument("domain")
     opt_args = parser.parse_args(cli_args)
     sts = 0
     source = CreateConfig(opt_args.domain, opt_args)
     # source.do_migrate_openerp()
     source.close()
     return sts
```

### Comparing `wok_code-2.0.8/wok_code/scripts/__init__.py` & `wok_code-2.0.9/wok_code/scripts/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 # -*- coding: utf-8 -*-
 from . import main
+
 # from . import create_translation_file
+from . import arcangelo
 from . import cvt_csv_2_rst
 from . import cvt_csv_coa
 from . import deploy_odoo
 from . import dist_pkg
-from . import do_migrate
 from . import do_odoo_site
 from . import gen_readme
 from . import generate_random_codes
 from . import license_mgnt
 from . import lint_2_compare
 from . import makepo_it
 from . import odoo_dependencies
 from . import odoo_translation
 from . import please
-from . import please_z0bug
 from . import please_apache
+from . import please_cwd
+from . import please_python
+from . import please_z0bug
 from . import run_odoo_debug
 from . import to_pep8
 from . import wget_odoo_repositories
```

### Comparing `wok_code-2.0.8/wok_code/eval_gtin.py` & `wok_code-2.0.9/wok_code/eval_gtin.py`

 * *Files identical despite different names*

### Comparing `wok_code-2.0.8/wok_code/do_git_checkout_new_branch.py` & `wok_code-2.0.9/wok_code/do_git_checkout_new_branch.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,28 +5,37 @@
 import re
 import sys
 import os
 import argparse
 
 from z0lib import z0lib
 
-__version__ = "2.0.8"
+__version__ = "2.0.9"
 
 
 class RepoCheckout(object):
-
     def __init__(self, opt_args):
         self.opt_args = opt_args
-        if opt_args.odoo_branch not in ("16.0", "15.0", "14.0", "13.0", "12.0", "11.0",
-                                        "10,0", "9.0", "8.0", "7.0", "6.1"):
+        if opt_args.odoo_branch not in (
+            "16.0",
+            "15.0",
+            "14.0",
+            "13.0",
+            "12.0",
+            "11.0",
+            "10,0",
+            "9.0",
+            "8.0",
+            "7.0",
+            "6.1",
+        ):
             print("Invalid Odoo branch")
             exit(2)
-        if (
-            not opt_args.origin_path
-            or not os.path.isdir(os.path.expanduser(opt_args.origin_path))
+        if not opt_args.origin_path or not os.path.isdir(
+            os.path.expanduser(opt_args.origin_path)
         ):
             print("Missed origin path: use --origin-path=PATH!")
             exit(2)
         if self.opt_args.origin_path not in (".", "./"):
             self.opt_args.origin_path = os.path.expanduser(opt_args.origin_path)
         if not opt_args.target_path:
             print("Missed target path: use -p PATH!")
@@ -68,95 +77,124 @@
 
     def is_git_repo(self, path):
         return os.path.isdir(os.path.join(path, ".git"))
 
     def build_new_repo(self, repo, origin_path):
         def git_clone(repo, target_path):
             if os.getcwd() != target_path:
-                z0lib.run_traced("cd %s" % os.path.dirname(target_path),
-                                 verbose=self.opt_args.verbose,
-                                 dry_run=self.opt_args.dry_run)
+                z0lib.run_traced(
+                    "cd %s" % os.path.dirname(target_path),
+                    verbose=self.opt_args.verbose,
+                    dry_run=self.opt_args.dry_run,
+                )
             git_repo = self.git_url + "/" + repo
             if repo == "OCB":
                 z0lib.run_traced(
-                    ("git clone %s %s --depth=1 --no-single-branch "
-                     "--no-recurse-submodules")
+                    (
+                        "git clone %s %s --depth=1 --no-single-branch "
+                        "--no-recurse-submodules"
+                    )
                     % (git_repo, os.path.basename(target_path)),
                     verbose=self.opt_args.verbose,
-                    dry_run=self.opt_args.dry_run)
+                    dry_run=self.opt_args.dry_run,
+                )
             else:
-                z0lib.run_traced("git clone %s --depth=1 --no-single-branch" % git_repo,
-                                 verbose=self.opt_args.verbose,
-                                 dry_run=self.opt_args.dry_run)
+                z0lib.run_traced(
+                    "git clone %s --depth=1 --no-single-branch" % git_repo,
+                    verbose=self.opt_args.verbose,
+                    dry_run=self.opt_args.dry_run,
+                )
 
         def git_checkout(target_path):
             if os.getcwd() != target_path:
-                z0lib.run_traced("cd %s" % target_path,
-                                 verbose=self.opt_args.verbose,
-                                 dry_run=self.opt_args.dry_run)
-            z0lib.run_traced("git checkout -b %s" % self.opt_args.odoo_branch,
-                             verbose=self.opt_args.verbose,
-                             dry_run=self.opt_args.dry_run)
+                z0lib.run_traced(
+                    "cd %s" % target_path,
+                    verbose=self.opt_args.verbose,
+                    dry_run=self.opt_args.dry_run,
+                )
+            z0lib.run_traced(
+                "git checkout -b %s" % self.opt_args.odoo_branch,
+                verbose=self.opt_args.verbose,
+                dry_run=self.opt_args.dry_run,
+            )
 
         def git_delete_unrelated_branch(target_path):
             if os.getcwd() != target_path:
-                z0lib.run_traced("cd %s" % target_path,
-                                 verbose=self.opt_args.verbose,
-                                 dry_run=self.opt_args.dry_run)
-            sts, stdout, stderr = z0lib.run_traced("git branch",
-                                                   verbose=self.opt_args.verbose,
-                                                   dry_run=self.opt_args.dry_run)
+                z0lib.run_traced(
+                    "cd %s" % target_path,
+                    verbose=self.opt_args.verbose,
+                    dry_run=self.opt_args.dry_run,
+                )
+            sts, stdout, stderr = z0lib.run_traced(
+                "git branch",
+                verbose=self.opt_args.verbose,
+                dry_run=self.opt_args.dry_run,
+            )
             for ln in stdout.split("\n"):
                 if not ln or ln.startswith("*"):
                     continue
-                z0lib.run_traced("git branch -D %s" % ln.strip(),
-                                 verbose=self.opt_args.verbose,
-                                 dry_run=self.opt_args.dry_run)
+                z0lib.run_traced(
+                    "git branch -D %s" % ln.strip(),
+                    verbose=self.opt_args.verbose,
+                    dry_run=self.opt_args.dry_run,
+                )
 
         def git_add_all(target_path):
             if os.getcwd() != target_path:
-                z0lib.run_traced("cd %s" % target_path,
-                                 verbose=self.opt_args.verbose,
-                                 dry_run=self.opt_args.dry_run)
-            z0lib.run_traced("git add ./",
-                             verbose=self.opt_args.verbose,
-                             dry_run=self.opt_args.dry_run)
+                z0lib.run_traced(
+                    "cd %s" % target_path,
+                    verbose=self.opt_args.verbose,
+                    dry_run=self.opt_args.dry_run,
+                )
+            z0lib.run_traced(
+                "git add ./",
+                verbose=self.opt_args.verbose,
+                dry_run=self.opt_args.dry_run,
+            )
 
         def git_push(target_path):
             if os.getcwd() != target_path:
-                z0lib.run_traced("cd %s" % target_path,
-                                 verbose=self.opt_args.verbose,
-                                 dry_run=self.opt_args.dry_run)
+                z0lib.run_traced(
+                    "cd %s" % target_path,
+                    verbose=self.opt_args.verbose,
+                    dry_run=self.opt_args.dry_run,
+                )
             found = False
             sts, stdout, stderr = z0lib.run_traced("git branch")
             if sts == 0 and stdout:
                 regex = r"^[*]* +" + self.opt_args.odoo_branch + r" *$"
                 for ln in stdout.split("\n"):
                     if re.match(regex, ln):
                         found = True
                         break
             if found and self.opt_args.remove_unrelated_branch:
-                z0lib.run_traced("git push origin delete %s"
-                                 % self.opt_args.odoo_branch,
-                                 verbose=self.opt_args.verbose,
-                                 dry_run=self.opt_args.dry_run)
+                z0lib.run_traced(
+                    "git push origin delete %s" % self.opt_args.odoo_branch,
+                    verbose=self.opt_args.verbose,
+                    dry_run=self.opt_args.dry_run,
+                )
                 found = False
-            z0lib.run_traced("git commit --no-verify -m \"[NEW] Initial setup %s\""
-                             % self.opt_args.odoo_branch,
-                             verbose=self.opt_args.verbose,
-                             dry_run=self.opt_args.dry_run)
+            z0lib.run_traced(
+                "git commit --no-verify -m \"[NEW] Initial setup %s\""
+                % self.opt_args.odoo_branch,
+                verbose=self.opt_args.verbose,
+                dry_run=self.opt_args.dry_run,
+            )
             if found:
-                z0lib.run_traced("git push",
-                                 verbose=self.opt_args.verbose,
-                                 dry_run=self.opt_args.dry_run)
+                z0lib.run_traced(
+                    "git push",
+                    verbose=self.opt_args.verbose,
+                    dry_run=self.opt_args.dry_run,
+                )
             else:
-                z0lib.run_traced("git push --set-upstream origin %s"
-                                 % self.opt_args.odoo_branch,
-                                 verbose=self.opt_args.verbose,
-                                 dry_run=self.opt_args.dry_run)
+                z0lib.run_traced(
+                    "git push --set-upstream origin %s" % self.opt_args.odoo_branch,
+                    verbose=self.opt_args.verbose,
+                    dry_run=self.opt_args.dry_run,
+                )
 
         def rsync_origin_path(repo, origin_path, target_path):
             exclude_path = self.opt_args.exclude_path.split(",")
             exclude_opt = "--exclude \".*/\""
             for p in exclude_path:
                 exclude_opt += " --exclude \"/%s\"" % p
             if repo == "OCB":
@@ -166,105 +204,131 @@
                         or p.startswith("_")
                         or os.path.isdir(os.path.join(origin_path, p, ".git"))
                         or p in exclude_path
                     ):
                         continue
                     src = os.path.join(origin_path, p)
                     if os.path.isfile(src):
-                        z0lib.run_traced("cp %s %s" % (src, target_path),
-                                         verbose=self.opt_args.verbose,
-                                         dry_run=self.opt_args.dry_run)
+                        z0lib.run_traced(
+                            "cp %s %s" % (src, target_path),
+                            verbose=self.opt_args.verbose,
+                            dry_run=self.opt_args.dry_run,
+                        )
                     else:
                         z0lib.run_traced(
                             "rsync -avz --delete %s %s/ %s/"
                             % (exclude_opt, src, os.path.join(target_path, p)),
                             verbose=self.opt_args.verbose,
-                            dry_run=self.opt_args.dry_run)
+                            dry_run=self.opt_args.dry_run,
+                        )
             else:
-                z0lib.run_traced("rsync -avz --delete %s %s/ %s/"
-                                 % (exclude_opt, origin_path, target_path),
-                                 verbose=self.opt_args.verbose,
-                                 dry_run=self.opt_args.dry_run)
+                z0lib.run_traced(
+                    "rsync -avz --delete %s %s/ %s/"
+                    % (exclude_opt, origin_path, target_path),
+                    verbose=self.opt_args.verbose,
+                    dry_run=self.opt_args.dry_run,
+                )
             for p in os.listdir(target_path):
                 if (
                     p.startswith(".")
                     or p.startswith("_")
                     or p in ("egg-info", "readme")
                     or os.path.isdir(os.path.join(origin_path, p, ".git"))
                 ):
                     continue
                 src = os.path.join(target_path, p)
                 if not os.path.exists(os.path.join(origin_path, p)):
                     if os.path.isfile(src):
-                        z0lib.run_traced("rm -f %s" % src,
-                                         verbose=self.opt_args.verbose,
-                                         dry_run=self.opt_args.dry_run)
+                        z0lib.run_traced(
+                            "rm -f %s" % src,
+                            verbose=self.opt_args.verbose,
+                            dry_run=self.opt_args.dry_run,
+                        )
                     else:
-                        z0lib.run_traced("rm -fR %s" % src,
-                                         verbose=self.opt_args.verbose,
-                                         dry_run=self.opt_args.dry_run)
+                        z0lib.run_traced(
+                            "rm -fR %s" % src,
+                            verbose=self.opt_args.verbose,
+                            dry_run=self.opt_args.dry_run,
+                        )
             if repo == "OCB":
-                z0lib.run_traced("do_gitignore ./",
-                                 verbose=self.opt_args.verbose,
-                                 dry_run=self.opt_args.dry_run)
+                z0lib.run_traced(
+                    "do_gitignore ./",
+                    verbose=self.opt_args.verbose,
+                    dry_run=self.opt_args.dry_run,
+                )
             if os.getcwd() != origin_path:
-                z0lib.run_traced("cd %s" % origin_path,
-                                 verbose=self.opt_args.verbose,
-                                 dry_run=self.opt_args.dry_run)
-            sts, stdout, stderr = z0lib.run_traced("git remote -v",
-                                                   verbose=self.opt_args.verbose,
-                                                   dry_run=self.opt_args.dry_run)
+                z0lib.run_traced(
+                    "cd %s" % origin_path,
+                    verbose=self.opt_args.verbose,
+                    dry_run=self.opt_args.dry_run,
+                )
+            sts, stdout, stderr = z0lib.run_traced(
+                "git remote -v",
+                verbose=self.opt_args.verbose,
+                dry_run=self.opt_args.dry_run,
+            )
             url = ""
             if sts == 0 and stdout:
                 for ln in stdout.split("\n"):
                     lns = ln.split()
                     if len(lns) < 2:
                         continue
                     elif lns[0] == "origin":
                         url = lns[1]
                         break
             if url:
                 if os.getcwd() != target_path:
-                    z0lib.run_traced("cd %s" % target_path,
-                                     verbose=self.opt_args.verbose,
-                                     dry_run=self.opt_args.dry_run)
+                    z0lib.run_traced(
+                        "cd %s" % target_path,
+                        verbose=self.opt_args.verbose,
+                        dry_run=self.opt_args.dry_run,
+                    )
                 url_upstream = ""
                 for ln in stdout.split("\n"):
                     lns = ln.split()
                     if len(lns) < 2:
                         continue
                     elif lns[0] == "upstream":
                         url_upstream = lns[1]
                         break
                 if url_upstream:
-                    z0lib.run_traced("git remote remove upstream",
-                                     verbose=self.opt_args.verbose,
-                                     dry_run=self.opt_args.dry_run)
-                z0lib.run_traced("git remote add upstream %s" % url,
-                                 verbose=self.opt_args.verbose,
-                                 dry_run=self.opt_args.dry_run)
+                    z0lib.run_traced(
+                        "git remote remove upstream",
+                        verbose=self.opt_args.verbose,
+                        dry_run=self.opt_args.dry_run,
+                    )
+                z0lib.run_traced(
+                    "git remote add upstream %s" % url,
+                    verbose=self.opt_args.verbose,
+                    dry_run=self.opt_args.dry_run,
+                )
 
-        target_path = self.opt_args.target_path if repo == "OCB" else os.path.join(
-            self.opt_args.target_path, repo)
+        target_path = (
+            self.opt_args.target_path
+            if repo == "OCB"
+            else os.path.join(self.opt_args.target_path, repo)
+        )
         if os.path.isdir(target_path):
             if not self.opt_args.update:
                 print("Path %s already exists!" % target_path)
                 return 1
         git_clone(repo, target_path)
         if not os.path.isdir(target_path):
             print("Directory %s not created" % target_path)
             return 0
         git_checkout(target_path)
         git_delete_unrelated_branch(target_path)
         if self.opt_args.origin_path not in (".", "./"):
             rsync_origin_path(repo, origin_path, target_path)
         elif repo == "OCB":
-            z0lib.run_traced("gitignore ./",
-                             verbose=self.opt_args.verbose,
-                             dry_run=self.opt_args.dry_run)
+            z0lib.run_traced(
+                "gitignore ./",
+                verbose=self.opt_args.verbose,
+                dry_run=self.opt_args.dry_run,
+            )
         git_add_all(target_path)
         if self.opt_args.save_git:
             git_push(target_path)
         return 0
 
     def do_git_checkout(self):
         path = self.opt_args.origin_path
@@ -279,44 +343,47 @@
                         break
         return sts
 
 
 def main(cli_args=None):
     cli_args = cli_args or sys.argv[1:]
     parser = argparse.ArgumentParser(
-        description="Create new repo branch",
-        epilog="© 2022-2023 by SHS-AV s.r.l."
+        description="Create new repo branch", epilog="© 2022-2023 by SHS-AV s.r.l."
+    )
+    parser.add_argument(
+        "-b", "--odoo-branch", dest="odoo_branch", help="New Odoo branch"
     )
-    parser.add_argument("-b", "--odoo-branch",
-                        dest="odoo_branch",
-                        help="New Odoo branch")
-    parser.add_argument("-G", "--git-org",
-                        help="Git organization to checkout")
+    parser.add_argument("-G", "--git-org", help="Git organization to checkout")
     parser.add_argument("-n", "--dry-run", action="store_true")
     parser.add_argument(
-        "-o", "--origin-path",
-        help="Local origin directory to merge or ./ if not origin (best is OCA path)")
-    parser.add_argument("-p", "--target-path",
-                        help="Local directory for checkout")
+        "-o",
+        "--origin-path",
+        help="Local origin directory to merge or ./ if not origin (best is OCA path)",
+    )
+    parser.add_argument("-p", "--target-path", help="Local directory for checkout")
     parser.add_argument(
-        "-R",  "--remove-unrelated-branch",
+        "-R",
+        "--remove-unrelated-branch",
         help="Remove not required unrelated branch from local directory",
-        action="store_true")
-    parser.add_argument("-S",  "--save-git",
-                        help="Execute git pull after checkout",
-                        action="store_true")
-    parser.add_argument("-U",
-                        "--update",
-                        help="Update target directory if exists",
-                        action="store_true")
+        action="store_true",
+    )
+    parser.add_argument(
+        "-S", "--save-git", help="Execute git pull after checkout", action="store_true"
+    )
+    parser.add_argument(
+        "-U", "--update", help="Update target directory if exists", action="store_true"
+    )
     parser.add_argument("-v", "--verbose", action="count", default=0)
     parser.add_argument("-V", "--version", action="version", version=__version__)
-    parser.add_argument("-x", "--exclude-path",
-                        help="Directories to exclude (comma separated)",
-                        default="setup,venv_odoo")
+    parser.add_argument(
+        "-x",
+        "--exclude-path",
+        help="Directories to exclude (comma separated)",
+        default="setup,venv_odoo",
+    )
     opt_args = parser.parse_args(cli_args)
     repo = RepoCheckout(opt_args)
     return repo.do_git_checkout()
 
 
 if __name__ == "__main__":
     exit(main(None))
```

### Comparing `wok_code-2.0.8/wok_code/topep8` & `wok_code-2.0.9/wok_code/topep8`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 link_cfg $DIST_CONF $TCONF
 [[ $TRAVIS_DEBUG_MODE -ge 8 ]] && echo "DIST_CONF=$DIST_CONF" && echo "TCONF=$TCONF"
 get_pypi_param ALL
 RED="\e[1;31m"
 GREEN="\e[1;32m"
 CLR="\e[0m"
 
-__version__=2.0.8
+__version__=2.0.9
 
 # [[ -f $TDIR/../../python_plus/list_requirements.py ]] && LISTREQ=$TDIR/../../python_plus/list_requirements.py || LISTREQ=list_requirements.py
 YAML_TMPL=~/dev/pypi/z0bug_odd/z0bug_odoo/sample_files/.travis.yml
 NO_APT_GET="(build-essential|curl|git|gradle|gzip|java|lessc|less-plugin-clean-css|nodejs|npm|openssl|python-setuptools|python-simplejson|PhantomJS|rvm|ruby|sass|scss|tesseract|wget|wkhtmltopdf|zip)"
 
 expand_macro() {
   local t p v lne lne1
```

### Comparing `wok_code-2.0.8/wok_code/install_python_3_from_source.sh` & `wok_code-2.0.9/wok_code/install_python_3_from_source.sh`

 * *Files identical despite different names*

### Comparing `wok_code-2.0.8/wok_code/cvt_script.man` & `wok_code-2.0.9/wok_code/cvt_script.man`

 * *Files identical despite different names*

### Comparing `wok_code-2.0.8/wok_code/to_oca.2p8` & `wok_code-2.0.9/wok_code/to_oca.2p8`

 * *Files identical despite different names*

### Comparing `wok_code-2.0.8/wok_code/do_set_utf8.py` & `wok_code-2.0.9/wok_code/do_set_utf8.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 
 TAG = "# -*- coding: utf-8 -*-"
 UNTAG = "# -*- encoding: utf-8 -*-"
 
 
 def do_set_utf8(ffn):
     found_tag = False
-    with open(ffn, 'r') as fd:
-        lines = fd.read().split('\n')
+    with open(ffn, "r") as fd:
+        lines = fd.read().split("\n")
         coding_line = -1
         rm_lines = []
         for nro, line in enumerate(lines):
             if line == TAG:
                 if coding_line < 0:
                     found_tag = True
                     coding_line = nro
@@ -28,60 +28,64 @@
             elif line.startswith("# flake8:") or line.startswith("# pylint:"):
                 if coding_line:
                     rm_lines.append(coding_line)
                     found_tag = False
                     coding_line = -1
                     continue
             if coding_line < 0 and (
-                not line or ((not line.startswith("#!") or nro)
-                             and not line.startswith("# flake8:")
-                             and not line.startswith("# pylint:"))):
+                not line
+                or (
+                    (not line.startswith("#!") or nro)
+                    and not line.startswith("# flake8:")
+                    and not line.startswith("# pylint:")
+                )
+            ):
                 coding_line = nro
-            if not line or not line.startswith('#') or nro > 3:
+            if not line or not line.startswith("#") or nro > 3:
                 break
         for nro in sorted(rm_lines, reverse=True):
             if nro < coding_line:
                 coding_line -= 1
             del lines[nro]
         if not found_tag and coding_line >= 0:
             lines.insert(coding_line, TAG)
     if not found_tag or rm_lines:
-        bakfile = '%s~' % ffn
+        bakfile = "%s~" % ffn
         if os.path.isfile(bakfile):
             os.remove(bakfile)
         if os.path.isfile(ffn):
             os.rename(ffn, bakfile)
-        with open(ffn, 'w') as fd:
+        with open(ffn, "w") as fd:
             fd.write("\n".join(lines))
             print(ffn)
 
 
 def main(argv):
     argv = argv or sys.argv[1:]
     path = None
     for param in argv:
-        if param.startswith('-'):
+        if param.startswith("-"):
             pass
         else:
             path = os.path.expanduser(param)
     if not path:
-        print('No path supplied! Use %s PATH' % sys.argv[0])
+        print("No path supplied! Use %s PATH" % sys.argv[0])
         return 1
     if os.path.isdir(path):
         for root, dirs, files in os.walk(path):
-            if 'setup' in dirs:
-                del dirs[dirs.index('setup')]
+            if "setup" in dirs:
+                del dirs[dirs.index("setup")]
             for fn in files:
-                if not fn.endswith('.py'):
+                if not fn.endswith(".py"):
                     continue
                 ffn = os.path.join(root, fn)
                 do_set_utf8(ffn)
     elif os.path.isfile(path):
         do_set_utf8(path)
     else:
-        print('Path %s does not exist!' % sys.argv[0])
+        print("Path %s does not exist!" % sys.argv[0])
         return 2
     return 0
 
 
 if __name__ == "__main__":
     exit(main(None))
```

### Comparing `wok_code-2.0.8/wok_code/please.man` & `wok_code-2.0.9/wok_code/please.man`

 * *Files identical despite different names*

### Comparing `wok_code-2.0.8/wok_code/to_zero.2p8` & `wok_code-2.0.9/wok_code/to_zero.2p8`

 * *Files identical despite different names*

### Comparing `wok_code-2.0.8/wok_code/to_pep8.2p8` & `wok_code-2.0.9/wok_code/to_pep8.2p8`

 * *Files identical despite different names*

### Comparing `wok_code-2.0.8/wok_code/cvt_script` & `wok_code-2.0.9/wok_code/cvt_script`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 link_cfg $DIST_CONF $TCONF
 [[ $TRAVIS_DEBUG_MODE -ge 8 ]] && echo "DIST_CONF=$DIST_CONF" && echo "TCONF=$TCONF"
 get_pypi_param ALL
 RED="\e[1;31m"
 GREEN="\e[1;32m"
 CLR="\e[0m"
 
-__version__=2.0.8
+__version__=2.0.9
 
 #//Only human upgradable code/
 # blk1 => z0librc
 # blk2 => odoorc
 # blk3 => travisrc
 # blk4 => zarrc
 # blk8 => TESTDIR= ...
```

### Comparing `wok_code-2.0.8/setup.py` & `wok_code-2.0.9/wok_code/scripts/setup.info`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     install_requires.append('translators')
     install_requires.append('twine')
 else:
     install_requires.append('twine==1.15.0')
 
 setup(
     name='wok_code',
-    version='2.0.8',
+    version='2.0.9',
     description='Python developers tools',
     long_description="""
 Various tools at your fingertips.
 
 The available tools are:
 
 * cvt_csv_2_rst.py: convert csv file into rst file
@@ -77,15 +77,15 @@
             'wok_code-info = wok_code.scripts.main:main',
             'cvt_csv_2_rst.py = wok_code.scripts.cvt_csv_2_rst:main',
             'cvt_csv_coa = wok_code.scripts.cvt_csv_coa:main',
             'deploy_odoo = wok_code.scripts.deploy_odoo:main',
             'dist_pkg = wok_code.scripts.dist_pkg:main',
             'do_gitignore = wok_code.do_gitignore:main',
             'do_git_checkout_new_branch = wok_code.do_git_checkout_new_branch:main',
-            'do_migrate = wok_code.scripts.do_migrate:main',
+            'arcangelo = wok_code.scripts.arcangelo:main',
             'do_odoo_site.py = wok_code.scripts.do_odoo_site:main',
             'gen_readme.py = wok_code.scripts.gen_readme:main',
             'lint_2_compare = wok_code.scripts.lint_2_compare:main',
             'makepo_it.py = wok_code.scripts.makepo_it:main',
             'odoo_dependencies.py = wok_code.scripts.odoo_dependencies:main',
             'odoo_translation.py = wok_code.scripts.odoo_translation:main',
             'please = wok_code.scripts.please:main',
```

### Comparing `wok_code-2.0.8/PKG-INFO` & `wok_code-2.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: wok_code
-Version: 2.0.8
+Version: 2.0.9
 Summary: Python developers tools
 Home-page: https://zeroincombenze-tools.readthedocs.io
 Author: Antonio Maria Vigliotti
 Author-email: antoniomaria.vigliotti@gmail.com
 License: Affero GPL
 Project-URL: Source, https://github.com/zeroincombenze/tools
 Project-URL: Documentation, https://zeroincombenze-tools.readthedocs.io
```

### Comparing `wok_code-2.0.8/README.rst` & `wok_code-2.0.9/README.rst`

 * *Files 11% similar despite different names*

```diff
@@ -1,38 +1,22 @@
 
-======
- 2.0.8
-======
+==============
+wok_code 2.0.9
+==============
 
 
 
 |Maturity| |license gpl|
 
 
 
 
 Overview
 ========
 
-Development tools
------------------
-
-Various tools at your fingertips.
-
-The available tools are:
-
-* cvt_csv_2_rst.py: convert csv file into rst file
-* cvt_csv_2_xml.py: convert csv file into xml file
-* cvt_script: parse bash script and convert to meet company standard
-* gen_readme.py: generate documentation files, mainly README.rst
-* odoo_dependency.py: show odoo dependencies and/or Odoo module tree
-* odoo_translation.py: manage Odoo translation
-* pep8: parse source .py file to meet pep8 and convert across Odoo versions
-* please: developer shell
-* wget_odoo_repositories.py: get repository names from github.com
 
 
 please: developer shell
 ~~~~~~~~~~~~~~~~~~~~~~~
 
 please is an interactive developer shell aim to help development and testing software.
 
@@ -311,16 +295,14 @@
 
 
 |
 
 Usage
 =====
 
-Module usage
-------------
 
 
 
 
 gen_readme.py usage
 ~~~~~~~~~~~~~~~~~~~
 
@@ -821,106 +803,14 @@
 ::
 
     cd $HOME
     ./install_tools.sh -U
     source $HOME/devel/activate_tools
 
 
-History
--------
-
-2.0.8 (2023-05-09)
-~~~~~~~~~~~~~~~~~~
-
-* [FIX] Install run_odoo_debug
-* [FIX] Install do_git_ignore
-* [IMP] lint_2_compare: ignore odoo/openerp test string and LICENSE files
-* [IMP] lint_2_compare: new switch ---purge do not load identical files (quick diff)
-
-2.0.7 (2023-05-08)
-~~~~~~~~~~~~~~~~~~
-
-* [IMP] deply_odoo: new action git-push
-* [REF] odoo_translation: new implementation
-* [FIX] run_odoo_debug: minor fixes
-* [NEW] do_git_checkout_new_branch: new command
-* [IMP] install_python3_from_source: improvements
-* [FIX] ssh.py: scp with port not 22
-
-2.0.6 (2023-02-23)
-~~~~~~~~~~~~~~~~~~
-
-* [IMP] ssh.py: -m -s switches accept path with user and host
-* [IMP] deploy_odoo: new property status to display
-* [IMP] deploy_odoo: new switches -l and -x
-* [NEW] do_git_checkout_new_branch.py
-* [IMP] do_migrate.py: new features
-* [IMP] run_odoo_debug.sh imported from odoo_score
-* [FIX] run_odoo_debug.sh: ODOO_COMMIT TEST not set when build template
-* [IMP] run_odoo_debug.sh: simulate server_wide_modules parameter for Odoo 7.0-
-
-
-2.0.5 (2023-01-13)
-~~~~~~~~~~~~~~~~~~
-
-* [IMP] please: wep now delete old travis-emulator logs
-* [IMP] install_python_3_from_source.sh: now can install python 3.9
-* [IMP] please: action docs, minor improvements
-* [IMP] deploy_odoo: format output list
-
-2.0.4 (2022-12-09)
-~~~~~~~~~~~~~~~~~~
-
-* [FIX] deploy_odoo: update from path
-* [FIX] build_cmd: best recognition of python version
-* [FIX] set_python_version.sh: best recognition of python version
-
-2.0.3 (2022-11-22)
-~~~~~~~~~~~~~~~~~~
-
-* [REF] odoo_translation
-
-2.0.2.1 (2022-10-31)
-~~~~~~~~~~~~~~~~~~~~
-
-* [IMP] lint_2_compare: ignoring .git .idea egg-info and setup directories
-* [IMP] lint_2_compare: new ignore switches
-* [FIX] please translate: do not execute export
-
-2.0.2 (2022-10-20)
-~~~~~~~~~~~~~~~~~~
-
-* [IMP] Clearing code
-
-2.0.1 (2022-10-12)
-~~~~~~~~~~~~~~~~~~
-
-* [IMP] minor improvements
-
-2.0.1 (2022-10-12)
-~~~~~~~~~~~~~~~~~~
-
-* [IMP] stable version
-
-2.0.0.4 (2022-10-05)
-~~~~~~~~~~~~~~~~~~~~
-
-* [IMP] New lint_2_compare command
-* [IMP] odoo_dependecies.py: minor upgrade
-
-2.0.0.3 (2022-09-14)
-~~~~~~~~~~~~~~~~~~~~
-
-* [FIX] deploy_odoo: show actual branch and organization
-* [FIX] deploy_odoo: update read from directory
-* [IMP] deploy_odoo: new command list repo info
-* [IMP] deploy_odoo: new feature link to repositories
-
-
-
 |
 |
 
 Credits
 =======
 
 Copyright
@@ -929,21 +819,24 @@
 SHS-AV s.r.l. <https://www.shs-av.com/>
 
 
 Contributors
 ------------
 
 * Antonio Maria Vigliotti <antoniomaria.vigliotti@gmail.com>
+Contributors
+------------
+
 
 
 |
 
-This module is part of  project.
+This module is part of tools project.
 
-Last Update / Ultimo aggiornamento: 
+Last Update / Ultimo aggiornamento: 2023-05-21
 
 .. |Maturity| image:: https://img.shields.io/badge/maturity-Beta-yellow.png
     :target: https://odoo-community.org/page/development-status
     :alt: 
 .. |license gpl| image:: https://img.shields.io/badge/licence-AGPL--3-blue.svg
     :target: http://www.gnu.org/licenses/agpl-3.0-standalone.html
     :alt: License: AGPL-3
```

