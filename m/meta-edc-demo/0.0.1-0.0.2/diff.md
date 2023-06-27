# Comparing `tmp/meta-edc-demo-0.0.1.tar.gz` & `tmp/meta-edc-demo-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meta-edc-demo-0.0.1.tar", last modified: Tue Jun 27 05:23:34 2023, max compression
+gzip compressed data, was "meta-edc-demo-0.0.2.tar", last modified: Tue Jun 27 06:22:40 2023, max compression
```

## Comparing `meta-edc-demo-0.0.1.tar` & `meta-edc-demo-0.0.2.tar`

### file list

```diff
@@ -1,937 +1,937 @@
-drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-06-27 05:23:34.811914 meta-edc-demo-0.0.1/
--rw-r--r--   0 estellaye   (501) staff       (20)        0 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.1/AUTHORS
--rw-r--r--   0 estellaye   (501) staff       (20)    11828 2022-10-13 03:34:11.000000 meta-edc-demo-0.0.1/CHANGES
--rw-r--r--   0 estellaye   (501) staff       (20)    35149 2020-03-04 23:21:43.000000 meta-edc-demo-0.0.1/LICENSE
--rw-r--r--   0 estellaye   (501) staff       (20)      162 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.1/MANIFEST.in
--rw-r--r--   0 estellaye   (501) staff       (20)      585 2023-06-27 05:23:34.812001 meta-edc-demo-0.0.1/PKG-INFO
--rw-r--r--   0 estellaye   (501) staff       (20)     1714 2022-10-12 03:43:37.000000 meta-edc-demo-0.0.1/README.rst
--rw-r--r--   0 estellaye   (501) staff       (20)      893 2022-04-11 18:27:09.000000 meta-edc-demo-0.0.1/TODO.txt
--rw-r--r--   0 estellaye   (501) staff       (20)        6 2023-06-27 05:15:40.000000 meta-edc-demo-0.0.1/VERSION
-drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-06-27 05:23:34.661397 meta-edc-demo-0.0.1/label_templates/
-drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-06-27 05:23:34.671940 meta-edc-demo-0.0.1/label_templates/2.25x1.25in/
--rw-r--r--   0 estellaye   (501) staff       (20)      588 2020-03-04 23:21:43.000000 meta-edc-demo-0.0.1/label_templates/2.25x1.25in/aliquot.lbl
--rw-r--r--   0 estellaye   (501) staff       (20)      341 2020-03-04 23:21:43.000000 meta-edc-demo-0.0.1/label_templates/2.25x1.25in/box.lbl
--rw-r--r--   0 estellaye   (501) staff       (20)      337 2020-03-04 23:21:43.000000 meta-edc-demo-0.0.1/label_templates/2.25x1.25in/manifest.lbl
--rw-r--r--   0 estellaye   (501) staff       (20)      520 2020-03-04 23:21:43.000000 meta-edc-demo-0.0.1/label_templates/2.25x1.25in/requisition.lbl
--rw-r--r--   0 estellaye   (501) staff       (20)      299 2020-03-04 23:21:43.000000 meta-edc-demo-0.0.1/label_templates/2.25x1.25in/subject.lbl
-drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-06-27 05:23:34.672527 meta-edc-demo-0.0.1/label_templates/2x1cm/
--rw-r--r--   0 estellaye   (501) staff       (20)      412 2020-03-04 23:21:43.000000 meta-edc-demo-0.0.1/label_templates/2x1cm/aliquot.lbl
--rw-r--r--   0 estellaye   (501) staff       (20)      297 2020-03-04 23:21:43.000000 meta-edc-demo-0.0.1/label_templates/2x1cm/box.lbl
--rw-r--r--   0 estellaye   (501) staff       (20)      294 2020-03-04 23:21:43.000000 meta-edc-demo-0.0.1/label_templates/2x1cm/manifest.lbl
--rw-r--r--   0 estellaye   (501) staff       (20)      387 2020-03-04 23:21:43.000000 meta-edc-demo-0.0.1/label_templates/2x1cm/requisition.lbl
-drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-06-27 05:23:34.673987 meta-edc-demo-0.0.1/meta_ae/
--rw-r--r--   0 estellaye   (501) staff       (20)        0 2020-03-15 03:34:20.000000 meta-edc-demo-0.0.1/meta_ae/__init__.py
--rw-r--r--   0 estellaye   (501) staff       (20)    11256 2022-09-26 19:37:19.000000 meta-edc-demo-0.0.1/meta_ae/action_items.py
-drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-06-27 05:23:34.675919 meta-edc-demo-0.0.1/meta_ae/admin/
--rw-r--r--   0 estellaye   (501) staff       (20)      460 2021-08-09 19:25:29.000000 meta-edc-demo-0.0.1/meta_ae/admin/__init__.py
--rw-r--r--   0 estellaye   (501) staff       (20)      416 2022-08-23 13:24:02.000000 meta-edc-demo-0.0.1/meta_ae/admin/ae_followup_admin.py
--rw-r--r--   0 estellaye   (501) staff       (20)      766 2022-08-23 13:24:02.000000 meta-edc-demo-0.0.1/meta_ae/admin/ae_initial_admin.py
--rw-r--r--   0 estellaye   (501) staff       (20)      410 2022-08-23 13:24:02.000000 meta-edc-demo-0.0.1/meta_ae/admin/ae_local_review_admin.py
--rw-r--r--   0 estellaye   (501) staff       (20)      420 2022-08-23 13:24:02.000000 meta-edc-demo-0.0.1/meta_ae/admin/ae_sponsor_review_admin.py
--rw-r--r--   0 estellaye   (501) staff       (20)      395 2022-08-23 13:24:02.000000 meta-edc-demo-0.0.1/meta_ae/admin/ae_susar_admin.py
--rw-r--r--   0 estellaye   (501) staff       (20)      381 2022-08-23 13:24:02.000000 meta-edc-demo-0.0.1/meta_ae/admin/ae_tmg_admin.py
--rw-r--r--   0 estellaye   (501) staff       (20)     2183 2022-08-23 13:24:02.000000 meta-edc-demo-0.0.1/meta_ae/admin/death_report_admin.py
--rw-r--r--   0 estellaye   (501) staff       (20)      444 2022-08-23 13:24:02.000000 meta-edc-demo-0.0.1/meta_ae/admin/death_report_tmg_admin.py
--rw-r--r--   0 estellaye   (501) staff       (20)      474 2022-08-23 13:24:02.000000 meta-edc-demo-0.0.1/meta_ae/admin/death_report_tmg_second_admin.py
--rw-r--r--   0 estellaye   (501) staff       (20)     4157 2022-08-23 13:24:02.000000 meta-edc-demo-0.0.1/meta_ae/admin/modeladmin_mixins.py
--rw-r--r--   0 estellaye   (501) staff       (20)      159 2021-07-02 03:53:00.000000 meta-edc-demo-0.0.1/meta_ae/admin_site.py
--rw-r--r--   0 estellaye   (501) staff       (20)      284 2022-08-23 13:24:02.000000 meta-edc-demo-0.0.1/meta_ae/apps.py
--rw-r--r--   0 estellaye   (501) staff       (20)     1134 2022-08-26 02:59:33.000000 meta-edc-demo-0.0.1/meta_ae/baker_recipes.py
--rw-r--r--   0 estellaye   (501) staff       (20)      756 2022-04-11 18:27:09.000000 meta-edc-demo-0.0.1/meta_ae/choices.py
--rw-r--r--   0 estellaye   (501) staff       (20)       36 2022-04-11 18:27:09.000000 meta-edc-demo-0.0.1/meta_ae/constants.py
-drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-06-27 05:23:34.677620 meta-edc-demo-0.0.1/meta_ae/forms/
--rw-r--r--   0 estellaye   (501) staff       (20)      438 2021-08-09 19:25:29.000000 meta-edc-demo-0.0.1/meta_ae/forms/__init__.py
--rw-r--r--   0 estellaye   (501) staff       (20)      298 2022-09-26 19:37:19.000000 meta-edc-demo-0.0.1/meta_ae/forms/ae_followup_form.py
--rw-r--r--   0 estellaye   (501) staff       (20)      292 2022-09-26 19:37:19.000000 meta-edc-demo-0.0.1/meta_ae/forms/ae_initial_form.py
--rw-r--r--   0 estellaye   (501) staff       (20)      284 2022-07-19 13:21:21.000000 meta-edc-demo-0.0.1/meta_ae/forms/ae_local_review_form.py
--rw-r--r--   0 estellaye   (501) staff       (20)      290 2022-07-19 13:21:21.000000 meta-edc-demo-0.0.1/meta_ae/forms/ae_sponsor_review_form.py
--rw-r--r--   0 estellaye   (501) staff       (20)      280 2022-09-26 19:37:19.000000 meta-edc-demo-0.0.1/meta_ae/forms/ae_susar_form.py
--rw-r--r--   0 estellaye   (501) staff       (20)      268 2022-09-26 19:37:19.000000 meta-edc-demo-0.0.1/meta_ae/forms/ae_tmg_form.py
--rw-r--r--   0 estellaye   (501) staff       (20)     1425 2022-09-26 19:37:19.000000 meta-edc-demo-0.0.1/meta_ae/forms/death_report_form.py
--rw-r--r--   0 estellaye   (501) staff       (20)      322 2022-09-26 19:37:19.000000 meta-edc-demo-0.0.1/meta_ae/forms/death_report_tmg_form.py
--rw-r--r--   0 estellaye   (501) staff       (20)      340 2022-09-26 19:37:19.000000 meta-edc-demo-0.0.1/meta_ae/forms/death_report_tmg_second_form.py
--rw-r--r--   0 estellaye   (501) staff       (20)      874 2022-09-26 19:37:19.000000 meta-edc-demo-0.0.1/meta_ae/forms/modelform_mixins.py
--rw-r--r--   0 estellaye   (501) staff       (20)     1372 2021-08-09 19:25:29.000000 meta-edc-demo-0.0.1/meta_ae/list_data.py
-drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-06-27 05:23:34.680687 meta-edc-demo-0.0.1/meta_ae/migrations/
--rw-r--r--   0 estellaye   (501) staff       (20)   140318 2022-09-30 02:18:01.000000 meta-edc-demo-0.0.1/meta_ae/migrations/0001_initial.py
--rw-r--r--   0 estellaye   (501) staff       (20)     2700 2021-07-05 19:24:26.000000 meta-edc-demo-0.0.1/meta_ae/migrations/0002_auto_20191024_1000.py
--rw-r--r--   0 estellaye   (501) staff       (20)     2445 2021-07-05 19:24:26.000000 meta-edc-demo-0.0.1/meta_ae/migrations/0003_auto_20191102_0033.py
--rw-r--r--   0 estellaye   (501) staff       (20)      998 2021-07-05 19:24:26.000000 meta-edc-demo-0.0.1/meta_ae/migrations/0004_auto_20191114_0821.py
--rw-r--r--   0 estellaye   (501) staff       (20)    18485 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.1/meta_ae/migrations/0005_auto_20210624_0225.py
--rw-r--r--   0 estellaye   (501) staff       (20)    16967 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.1/meta_ae/migrations/0006_aelocalreview_aesponsorreview.py
--rw-r--r--   0 estellaye   (501) staff       (20)     2709 2022-06-24 08:52:48.000000 meta-edc-demo-0.0.1/meta_ae/migrations/0007_auto_20210911_2036.py
--rw-r--r--   0 estellaye   (501) staff       (20)     1241 2022-06-24 08:52:45.000000 meta-edc-demo-0.0.1/meta_ae/migrations/0008_auto_20211011_1657.py
--rw-r--r--   0 estellaye   (501) staff       (20)     1152 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.1/meta_ae/migrations/0009_auto_20220307_1929.py
--rw-r--r--   0 estellaye   (501) staff       (20)     4215 2022-08-22 17:23:22.000000 meta-edc-demo-0.0.1/meta_ae/migrations/0010_auto_20220704_1841.py
--rw-r--r--   0 estellaye   (501) staff       (20)     2828 2022-08-23 13:31:01.000000 meta-edc-demo-0.0.1/meta_ae/migrations/0011_alter_aefollowup_action_identifier_and_more.py
--rw-r--r--   0 estellaye   (501) staff       (20)     2997 2022-08-26 02:59:33.000000 meta-edc-demo-0.0.1/meta_ae/migrations/0012_auto_20220826_0258.py
--rw-r--r--   0 estellaye   (501) staff       (20)     2842 2022-08-26 02:59:33.000000 meta-edc-demo-0.0.1/meta_ae/migrations/0013_auto_20220826_0322.py
--rw-r--r--   0 estellaye   (501) staff       (20)     1858 2022-08-26 02:59:33.000000 meta-edc-demo-0.0.1/meta_ae/migrations/0014_auto_20220826_0406.py
--rw-r--r--   0 estellaye   (501) staff       (20)     1239 2022-09-08 15:51:35.000000 meta-edc-demo-0.0.1/meta_ae/migrations/0015_auto_20220907_0157.py
--rw-r--r--   0 estellaye   (501) staff       (20)        0 2020-03-15 03:34:20.000000 meta-edc-demo-0.0.1/meta_ae/migrations/__init__.py
-drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-06-27 05:23:34.681114 meta-edc-demo-0.0.1/meta_ae/model_mixins/
--rw-r--r--   0 estellaye   (501) staff       (20)      114 2020-05-15 02:40:42.000000 meta-edc-demo-0.0.1/meta_ae/model_mixins/__init__.py
--rw-r--r--   0 estellaye   (501) staff       (20)     2638 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.1/meta_ae/model_mixins/ae_review_model_mixin.py
--rw-r--r--   0 estellaye   (501) staff       (20)     1799 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.1/meta_ae/model_mixins/death_report_model_mixin.py
-drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-06-27 05:23:34.682824 meta-edc-demo-0.0.1/meta_ae/models/
--rw-r--r--   0 estellaye   (501) staff       (20)      357 2021-08-09 19:25:29.000000 meta-edc-demo-0.0.1/meta_ae/models/__init__.py
--rw-r--r--   0 estellaye   (501) staff       (20)      236 2020-03-15 03:34:20.000000 meta-edc-demo-0.0.1/meta_ae/models/ae_followup.py
--rw-r--r--   0 estellaye   (501) staff       (20)      343 2020-03-15 03:34:20.000000 meta-edc-demo-0.0.1/meta_ae/models/ae_initial.py
--rw-r--r--   0 estellaye   (501) staff       (20)      236 2021-08-09 19:25:29.000000 meta-edc-demo-0.0.1/meta_ae/models/ae_local_review.py
--rw-r--r--   0 estellaye   (501) staff       (20)      240 2021-08-09 19:25:29.000000 meta-edc-demo-0.0.1/meta_ae/models/ae_sponsor_review.py
--rw-r--r--   0 estellaye   (501) staff       (20)      208 2020-03-15 03:34:20.000000 meta-edc-demo-0.0.1/meta_ae/models/ae_susar.py
--rw-r--r--   0 estellaye   (501) staff       (20)      226 2020-03-15 03:34:20.000000 meta-edc-demo-0.0.1/meta_ae/models/ae_tmg.py
--rw-r--r--   0 estellaye   (501) staff       (20)      446 2020-05-15 02:40:42.000000 meta-edc-demo-0.0.1/meta_ae/models/death_report.py
--rw-r--r--   0 estellaye   (501) staff       (20)      236 2021-07-05 19:24:26.000000 meta-edc-demo-0.0.1/meta_ae/models/death_report_tmg.py
--rw-r--r--   0 estellaye   (501) staff       (20)      565 2020-03-15 03:34:20.000000 meta-edc-demo-0.0.1/meta_ae/models/death_report_tmg_second.py
--rw-r--r--   0 estellaye   (501) staff       (20)      621 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.1/meta_ae/models/managers.py
-drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-06-27 05:23:34.683476 meta-edc-demo-0.0.1/meta_ae/pdf_reports/
--rw-r--r--   0 estellaye   (501) staff       (20)       70 2020-03-15 03:34:20.000000 meta-edc-demo-0.0.1/meta_ae/pdf_reports/__init__.py
--rw-r--r--   0 estellaye   (501) staff       (20)      184 2020-03-15 03:34:20.000000 meta-edc-demo-0.0.1/meta_ae/pdf_reports/ae_report.py
--rw-r--r--   0 estellaye   (501) staff       (20)      196 2020-03-15 03:34:20.000000 meta-edc-demo-0.0.1/meta_ae/pdf_reports/death_report.py
--rw-r--r--   0 estellaye   (501) staff       (20)      535 2020-03-15 03:34:20.000000 meta-edc-demo-0.0.1/meta_ae/pdf_reports/meta_pdf_report_mixin.py
-drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-06-27 05:23:34.683747 meta-edc-demo-0.0.1/meta_ae/templatetags/
--rw-r--r--   0 estellaye   (501) staff       (20)        0 2020-03-15 03:34:20.000000 meta-edc-demo-0.0.1/meta_ae/templatetags/__init__.py
--rw-r--r--   0 estellaye   (501) staff       (20)     1154 2022-08-22 17:23:22.000000 meta-edc-demo-0.0.1/meta_ae/templatetags/meta_ae_extras.py
-drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-06-27 05:23:34.684023 meta-edc-demo-0.0.1/meta_ae/tests/
--rw-r--r--   0 estellaye   (501) staff       (20)        0 2020-03-15 03:34:20.000000 meta-edc-demo-0.0.1/meta_ae/tests/__init__.py
-drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-06-27 05:23:34.684288 meta-edc-demo-0.0.1/meta_ae/tests/tests/
--rw-r--r--   0 estellaye   (501) staff       (20)        0 2021-08-09 19:25:29.000000 meta-edc-demo-0.0.1/meta_ae/tests/tests/__init__.py
--rw-r--r--   0 estellaye   (501) staff       (20)     4915 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.1/meta_ae/tests/tests/test_actions.py
--rw-r--r--   0 estellaye   (501) staff       (20)      260 2021-07-05 19:24:26.000000 meta-edc-demo-0.0.1/meta_ae/tests/urls.py
--rw-r--r--   0 estellaye   (501) staff       (20)      197 2021-08-09 19:25:29.000000 meta-edc-demo-0.0.1/meta_ae/urls.py
-drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-06-27 05:23:34.685094 meta-edc-demo-0.0.1/meta_auth/
--rw-r--r--   0 estellaye   (501) staff       (20)        0 2020-03-15 03:34:20.000000 meta-edc-demo-0.0.1/meta_auth/__init__.py
--rw-r--r--   0 estellaye   (501) staff       (20)      298 2022-06-24 09:16:28.000000 meta-edc-demo-0.0.1/meta_auth/apps.py
--rw-r--r--   0 estellaye   (501) staff       (20)     1738 2022-08-26 02:59:33.000000 meta-edc-demo-0.0.1/meta_auth/auth_objects.py
--rw-r--r--   0 estellaye   (501) staff       (20)     2435 2022-09-08 21:41:58.000000 meta-edc-demo-0.0.1/meta_auth/auths.py
--rw-r--r--   0 estellaye   (501) staff       (20)      111 2022-06-24 09:16:34.000000 meta-edc-demo-0.0.1/meta_auth/urls.py
-drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-06-27 05:23:34.686572 meta-edc-demo-0.0.1/meta_consent/
--rw-r--r--   0 estellaye   (501) staff       (20)        0 2020-03-15 03:34:20.000000 meta-edc-demo-0.0.1/meta_consent/__init__.py
--rw-r--r--   0 estellaye   (501) staff       (20)      756 2022-06-24 09:14:24.000000 meta-edc-demo-0.0.1/meta_consent/action_items.py
-drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-06-27 05:23:34.687039 meta-edc-demo-0.0.1/meta_consent/admin/
--rw-r--r--   0 estellaye   (501) staff       (20)      114 2020-03-15 03:34:20.000000 meta-edc-demo-0.0.1/meta_consent/admin/__init__.py
-drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-06-27 05:23:34.687357 meta-edc-demo-0.0.1/meta_consent/admin/actions/
--rw-r--r--   0 estellaye   (501) staff       (20)       70 2022-07-08 07:31:04.000000 meta-edc-demo-0.0.1/meta_consent/admin/actions/__init__.py
--rw-r--r--   0 estellaye   (501) staff       (20)     1474 2022-07-08 07:31:04.000000 meta-edc-demo-0.0.1/meta_consent/admin/actions/create_missing_prescriptions.py
--rw-r--r--   0 estellaye   (501) staff       (20)     5444 2022-08-23 13:24:02.000000 meta-edc-demo-0.0.1/meta_consent/admin/subject_consent_admin.py
--rw-r--r--   0 estellaye   (501) staff       (20)     2971 2022-08-23 13:24:02.000000 meta-edc-demo-0.0.1/meta_consent/admin/subject_reconsent_admin.py
--rw-r--r--   0 estellaye   (501) staff       (20)      169 2022-06-24 09:14:27.000000 meta-edc-demo-0.0.1/meta_consent/admin_site.py
--rw-r--r--   0 estellaye   (501) staff       (20)      282 2022-08-23 13:24:02.000000 meta-edc-demo-0.0.1/meta_consent/apps.py
--rw-r--r--   0 estellaye   (501) staff       (20)     1258 2022-08-26 02:59:33.000000 meta-edc-demo-0.0.1/meta_consent/baker_recipes.py
--rw-r--r--   0 estellaye   (501) staff       (20)      436 2022-06-24 09:14:37.000000 meta-edc-demo-0.0.1/meta_consent/consents.py
--rw-r--r--   0 estellaye   (501) staff       (20)       31 2022-06-24 09:14:43.000000 meta-edc-demo-0.0.1/meta_consent/constants.py
-drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-06-27 05:23:34.687814 meta-edc-demo-0.0.1/meta_consent/forms/
--rw-r--r--   0 estellaye   (501) staff       (20)      139 2022-04-11 18:27:09.000000 meta-edc-demo-0.0.1/meta_consent/forms/__init__.py
--rw-r--r--   0 estellaye   (501) staff       (20)     2425 2022-10-04 03:17:15.000000 meta-edc-demo-0.0.1/meta_consent/forms/subject_consent_form.py
--rw-r--r--   0 estellaye   (501) staff       (20)     1306 2022-10-04 03:17:15.000000 meta-edc-demo-0.0.1/meta_consent/forms/subject_reconsent_form.py
-drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-06-27 05:23:34.687970 meta-edc-demo-0.0.1/meta_consent/management/
--rw-r--r--   0 estellaye   (501) staff       (20)        0 2022-04-11 18:27:09.000000 meta-edc-demo-0.0.1/meta_consent/management/__init__.py
-drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-06-27 05:23:34.688193 meta-edc-demo-0.0.1/meta_consent/management/commands/
--rw-r--r--   0 estellaye   (501) staff       (20)        0 2022-04-11 18:27:09.000000 meta-edc-demo-0.0.1/meta_consent/management/commands/__init__.py
--rw-r--r--   0 estellaye   (501) staff       (20)     1438 2022-07-08 07:31:04.000000 meta-edc-demo-0.0.1/meta_consent/management/commands/create_missing_prescriptions.py
-drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-06-27 05:23:34.691906 meta-edc-demo-0.0.1/meta_consent/migrations/
--rw-r--r--   0 estellaye   (501) staff       (20)    66733 2022-09-30 02:18:01.000000 meta-edc-demo-0.0.1/meta_consent/migrations/0001_initial.py
--rw-r--r--   0 estellaye   (501) staff       (20)      591 2021-07-05 19:24:26.000000 meta-edc-demo-0.0.1/meta_consent/migrations/0002_auto_20191024_1000.py
--rw-r--r--   0 estellaye   (501) staff       (20)     1611 2020-04-03 04:33:09.000000 meta-edc-demo-0.0.1/meta_consent/migrations/0003_auto_20200325_0901.py
--rw-r--r--   0 estellaye   (501) staff       (20)     3510 2021-07-05 19:24:26.000000 meta-edc-demo-0.0.1/meta_consent/migrations/0004_auto_20210624_0225.py
--rw-r--r--   0 estellaye   (501) staff       (20)      791 2022-04-11 18:27:09.000000 meta-edc-demo-0.0.1/meta_consent/migrations/0005_alter_subjectconsent_options.py
--rw-r--r--   0 estellaye   (501) staff       (20)      638 2022-06-24 09:13:48.000000 meta-edc-demo-0.0.1/meta_consent/migrations/0006_auto_20210911_2036.py
--rw-r--r--   0 estellaye   (501) staff       (20)     3052 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.1/meta_consent/migrations/0007_auto_20220128_1719.py
--rw-r--r--   0 estellaye   (501) staff       (20)      943 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.1/meta_consent/migrations/0008_auto_20220412_2151.py
--rw-r--r--   0 estellaye   (501) staff       (20)     1391 2022-08-22 17:23:22.000000 meta-edc-demo-0.0.1/meta_consent/migrations/0009_auto_20220704_1841.py
--rw-r--r--   0 estellaye   (501) staff       (20)      648 2022-08-23 13:31:01.000000 meta-edc-demo-0.0.1/meta_consent/migrations/0010_alter_historicalsubjectreconsent_action_identifier_and_more.py
--rw-r--r--   0 estellaye   (501) staff       (20)      712 2022-08-26 02:59:33.000000 meta-edc-demo-0.0.1/meta_consent/migrations/0011_auto_20220826_0258.py
--rw-r--r--   0 estellaye   (501) staff       (20)      651 2022-08-26 02:59:33.000000 meta-edc-demo-0.0.1/meta_consent/migrations/0012_auto_20220826_0322.py
--rw-r--r--   0 estellaye   (501) staff       (20)      493 2022-08-26 02:59:33.000000 meta-edc-demo-0.0.1/meta_consent/migrations/0013_auto_20220826_0406.py
--rw-r--r--   0 estellaye   (501) staff       (20)      605 2022-09-30 02:18:01.000000 meta-edc-demo-0.0.1/meta_consent/migrations/0014_alter_subjectconsent_managers.py
--rw-r--r--   0 estellaye   (501) staff       (20)      756 2022-09-15 02:57:38.000000 meta-edc-demo-0.0.1/meta_consent/migrations/0015_auto_20220914_0542.py
--rw-r--r--   0 estellaye   (501) staff       (20)      948 2022-09-15 02:57:38.000000 meta-edc-demo-0.0.1/meta_consent/migrations/0016_auto_20220914_0547.py
--rw-r--r--   0 estellaye   (501) staff       (20)      923 2022-09-30 02:18:01.000000 meta-edc-demo-0.0.1/meta_consent/migrations/0017_auto_20220929_1742.py
--rw-r--r--   0 estellaye   (501) staff       (20)        0 2020-03-15 03:34:20.000000 meta-edc-demo-0.0.1/meta_consent/migrations/__init__.py
-drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-06-27 05:23:34.692700 meta-edc-demo-0.0.1/meta_consent/models/
--rw-r--r--   0 estellaye   (501) staff       (20)      174 2021-08-09 19:25:29.000000 meta-edc-demo-0.0.1/meta_consent/models/__init__.py
--rw-r--r--   0 estellaye   (501) staff       (20)      296 2022-06-24 09:13:53.000000 meta-edc-demo-0.0.1/meta_consent/models/model_mixins.py
--rw-r--r--   0 estellaye   (501) staff       (20)     4303 2022-07-01 06:36:06.000000 meta-edc-demo-0.0.1/meta_consent/models/signals.py
--rw-r--r--   0 estellaye   (501) staff       (20)     4054 2022-09-30 02:18:01.000000 meta-edc-demo-0.0.1/meta_consent/models/subject_consent.py
--rw-r--r--   0 estellaye   (501) staff       (20)     3588 2022-09-30 02:18:01.000000 meta-edc-demo-0.0.1/meta_consent/models/subject_reconsent.py
-drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-06-27 05:23:34.692963 meta-edc-demo-0.0.1/meta_consent/tests/
--rw-r--r--   0 estellaye   (501) staff       (20)        0 2020-03-15 03:34:20.000000 meta-edc-demo-0.0.1/meta_consent/tests/__init__.py
-drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-06-27 05:23:34.693379 meta-edc-demo-0.0.1/meta_consent/tests/tests/
--rw-r--r--   0 estellaye   (501) staff       (20)        0 2021-08-09 19:25:29.000000 meta-edc-demo-0.0.1/meta_consent/tests/tests/__init__.py
--rw-r--r--   0 estellaye   (501) staff       (20)     3546 2022-08-22 17:23:22.000000 meta-edc-demo-0.0.1/meta_consent/tests/tests/test_form_validators.py
--rw-r--r--   0 estellaye   (501) staff       (20)      376 2022-06-24 09:14:16.000000 meta-edc-demo-0.0.1/meta_consent/tests/tests/test_subject_consent.py
--rw-r--r--   0 estellaye   (501) staff       (20)      916 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.1/meta_consent/tests/urls.py
--rw-r--r--   0 estellaye   (501) staff       (20)      206 2022-06-24 09:14:40.000000 meta-edc-demo-0.0.1/meta_consent/urls.py
-drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-06-27 05:23:34.694075 meta-edc-demo-0.0.1/meta_dashboard/
--rw-r--r--   0 estellaye   (501) staff       (20)        0 2020-03-15 03:34:20.000000 meta-edc-demo-0.0.1/meta_dashboard/__init__.py
--rw-r--r--   0 estellaye   (501) staff       (20)     1993 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.1/meta_dashboard/apps.py
-drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-06-27 05:23:34.694227 meta-edc-demo-0.0.1/meta_dashboard/migrations/
--rw-r--r--   0 estellaye   (501) staff       (20)        0 2020-03-15 03:34:20.000000 meta-edc-demo-0.0.1/meta_dashboard/migrations/__init__.py
-drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-06-27 05:23:34.695071 meta-edc-demo-0.0.1/meta_dashboard/model_wrappers/
--rw-r--r--   0 estellaye   (501) staff       (20)      343 2021-07-05 19:24:26.000000 meta-edc-demo-0.0.1/meta_dashboard/model_wrappers/__init__.py
--rw-r--r--   0 estellaye   (501) staff       (20)      161 2020-03-15 03:34:20.000000 meta-edc-demo-0.0.1/meta_dashboard/model_wrappers/ae_initial_model_wrapper.py
--rw-r--r--   0 estellaye   (501) staff       (20)      375 2020-03-15 03:34:20.000000 meta-edc-demo-0.0.1/meta_dashboard/model_wrappers/death_report_model_wrapper.py
--rw-r--r--   0 estellaye   (501) staff       (20)      407 2020-03-15 03:34:20.000000 meta-edc-demo-0.0.1/meta_dashboard/model_wrappers/subject_refusal_model_wrapper.py
--rw-r--r--   0 estellaye   (501) staff       (20)     2718 2022-04-11 18:27:09.000000 meta-edc-demo-0.0.1/meta_dashboard/model_wrappers/subject_screening_model_wrapper.py
--rw-r--r--   0 estellaye   (501) staff       (20)     1204 2022-08-26 02:59:33.000000 meta-edc-demo-0.0.1/meta_dashboard/navbars.py
--rw-r--r--   0 estellaye   (501) staff       (20)       47 2022-06-24 09:14:59.000000 meta-edc-demo-0.0.1/meta_dashboard/patterns.py
-drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-06-27 05:23:34.695362 meta-edc-demo-0.0.1/meta_dashboard/templatetags/
--rw-r--r--   0 estellaye   (501) staff       (20)        0 2020-03-15 03:34:20.000000 meta-edc-demo-0.0.1/meta_dashboard/templatetags/__init__.py
--rw-r--r--   0 estellaye   (501) staff       (20)     3845 2022-08-22 17:23:22.000000 meta-edc-demo-0.0.1/meta_dashboard/templatetags/meta_dashboard_extras.py
-drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-06-27 05:23:34.695764 meta-edc-demo-0.0.1/meta_dashboard/tests/
--rw-r--r--   0 estellaye   (501) staff       (20)        0 2020-03-15 03:34:20.000000 meta-edc-demo-0.0.1/meta_dashboard/tests/__init__.py
--rw-r--r--   0 estellaye   (501) staff       (20)      716 2021-07-05 19:24:26.000000 meta-edc-demo-0.0.1/meta_dashboard/tests/admin.py
-drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-06-27 05:23:34.696029 meta-edc-demo-0.0.1/meta_dashboard/tests/tests/
--rw-r--r--   0 estellaye   (501) staff       (20)        0 2020-03-15 03:34:20.000000 meta-edc-demo-0.0.1/meta_dashboard/tests/tests/__init__.py
--rw-r--r--   0 estellaye   (501) staff       (20)     2494 2021-07-05 19:24:26.000000 meta-edc-demo-0.0.1/meta_dashboard/tests/tests/test_model_wrappers.py
--rw-r--r--   0 estellaye   (501) staff       (20)     2913 2021-07-05 19:24:26.000000 meta-edc-demo-0.0.1/meta_dashboard/tests/urls.py
--rw-r--r--   0 estellaye   (501) staff       (20)     1098 2022-06-24 09:15:02.000000 meta-edc-demo-0.0.1/meta_dashboard/urls.py
-drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-06-27 05:23:34.696189 meta-edc-demo-0.0.1/meta_dashboard/views/
--rw-r--r--   0 estellaye   (501) staff       (20)      222 2022-08-26 02:59:33.000000 meta-edc-demo-0.0.1/meta_dashboard/views/__init__.py
-drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-06-27 05:23:34.696677 meta-edc-demo-0.0.1/meta_dashboard/views/ae/
--rw-r--r--   0 estellaye   (501) staff       (20)      113 2020-03-15 03:34:20.000000 meta-edc-demo-0.0.1/meta_dashboard/views/ae/__init__.py
--rw-r--r--   0 estellaye   (501) staff       (20)      454 2021-07-05 19:24:26.000000 meta-edc-demo-0.0.1/meta_dashboard/views/ae/ae_listboard_view.py
--rw-r--r--   0 estellaye   (501) staff       (20)      492 2020-03-15 03:34:20.000000 meta-edc-demo-0.0.1/meta_dashboard/views/ae/death_report_listboard_view.py
-drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-06-27 05:23:34.696997 meta-edc-demo-0.0.1/meta_dashboard/views/screening/
--rw-r--r--   0 estellaye   (501) staff       (20)       42 2020-03-15 03:34:20.000000 meta-edc-demo-0.0.1/meta_dashboard/views/screening/__init__.py
--rw-r--r--   0 estellaye   (501) staff       (20)      888 2022-08-26 02:59:33.000000 meta-edc-demo-0.0.1/meta_dashboard/views/screening/listboard_view.py
-drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-06-27 05:23:34.697150 meta-edc-demo-0.0.1/meta_dashboard/views/subject/
--rw-r--r--   0 estellaye   (501) staff       (20)       81 2022-08-26 02:59:33.000000 meta-edc-demo-0.0.1/meta_dashboard/views/subject/__init__.py
-drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-06-27 05:23:34.697476 meta-edc-demo-0.0.1/meta_dashboard/views/subject/dashboard/
--rw-r--r--   0 estellaye   (501) staff       (20)       42 2020-03-15 03:34:20.000000 meta-edc-demo-0.0.1/meta_dashboard/views/subject/dashboard/__init__.py
--rw-r--r--   0 estellaye   (501) staff       (20)      285 2022-09-08 15:51:35.000000 meta-edc-demo-0.0.1/meta_dashboard/views/subject/dashboard/dashboard_view.py
-drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-06-27 05:23:34.697778 meta-edc-demo-0.0.1/meta_dashboard/views/subject/listboard/
--rw-r--r--   0 estellaye   (501) staff       (20)       49 2022-08-26 02:59:33.000000 meta-edc-demo-0.0.1/meta_dashboard/views/subject/listboard/__init__.py
--rw-r--r--   0 estellaye   (501) staff       (20)      695 2022-08-26 13:10:52.000000 meta-edc-demo-0.0.1/meta_dashboard/views/subject/listboard/listboard_view.py
-drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-06-27 05:23:34.698330 meta-edc-demo-0.0.1/meta_data_manager/
--rw-r--r--   0 estellaye   (501) staff       (20)        0 2022-04-11 18:27:09.000000 meta-edc-demo-0.0.1/meta_data_manager/__init__.py
--rw-r--r--   0 estellaye   (501) staff       (20)      233 2022-04-11 18:27:09.000000 meta-edc-demo-0.0.1/meta_data_manager/apps.py
--rw-r--r--   0 estellaye   (501) staff       (20)      167 2022-04-11 18:27:09.000000 meta-edc-demo-0.0.1/meta_data_manager/data_manager.py
--rw-r--r--   0 estellaye   (501) staff       (20)      953 2022-06-24 09:13:03.000000 meta-edc-demo-0.0.1/meta_data_manager/handlers.py
-drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-06-27 05:23:34.700368 meta-edc-demo-0.0.1/meta_edc/
--rw-r--r--   0 estellaye   (501) staff       (20)        0 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.1/meta_edc/__init__.py
--rw-r--r--   0 estellaye   (501) staff       (20)      845 2022-08-22 17:23:22.000000 meta-edc-demo-0.0.1/meta_edc/admin.py
--rw-r--r--   0 estellaye   (501) staff       (20)      450 2022-06-24 09:07:19.000000 meta-edc-demo-0.0.1/meta_edc/apps.py
--rw-r--r--   0 estellaye   (501) staff       (20)      175 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.1/meta_edc/asgi.py
--rw-r--r--   0 estellaye   (501) staff       (20)      785 2020-03-04 23:21:43.000000 meta-edc-demo-0.0.1/meta_edc/celery.py
-drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-06-27 05:23:34.700511 meta-edc-demo-0.0.1/meta_edc/management/
--rw-r--r--   0 estellaye   (501) staff       (20)        0 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.1/meta_edc/management/__init__.py
-drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-06-27 05:23:34.700725 meta-edc-demo-0.0.1/meta_edc/management/commands/
--rw-r--r--   0 estellaye   (501) staff       (20)        0 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.1/meta_edc/management/commands/__init__.py
--rw-r--r--   0 estellaye   (501) staff       (20)     1006 2022-10-12 03:43:37.000000 meta-edc-demo-0.0.1/meta_edc/management/commands/update_forms_reference.py
--rw-r--r--   0 estellaye   (501) staff       (20)      211 2022-06-24 09:07:24.000000 meta-edc-demo-0.0.1/meta_edc/meta_version.py
--rw-r--r--   0 estellaye   (501) staff       (20)     1339 2022-07-19 13:21:21.000000 meta-edc-demo-0.0.1/meta_edc/model_callers.py
--rw-r--r--   0 estellaye   (501) staff       (20)       46 2020-03-04 23:21:43.000000 meta-edc-demo-0.0.1/meta_edc/models.py
--rw-r--r--   0 estellaye   (501) staff       (20)     1065 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.1/meta_edc/navbars.py
-drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-06-27 05:23:34.701950 meta-edc-demo-0.0.1/meta_edc/settings/
--rw-r--r--   0 estellaye   (501) staff       (20)        0 2020-04-03 04:33:09.000000 meta-edc-demo-0.0.1/meta_edc/settings/__init__.py
--rw-r--r--   0 estellaye   (501) staff       (20)      706 2023-06-27 05:13:04.000000 meta-edc-demo-0.0.1/meta_edc/settings/debug.py
--rw-r--r--   0 estellaye   (501) staff       (20)    19094 2022-10-10 22:11:43.000000 meta-edc-demo-0.0.1/meta_edc/settings/defaults.py
--rw-r--r--   0 estellaye   (501) staff       (20)      513 2023-06-27 05:12:29.000000 meta-edc-demo-0.0.1/meta_edc/settings/live.py
--rw-r--r--   0 estellaye   (501) staff       (20)     1855 2022-10-10 22:12:06.000000 meta-edc-demo-0.0.1/meta_edc/settings/logging.py
--rw-r--r--   0 estellaye   (501) staff       (20)      591 2022-08-22 17:23:22.000000 meta-edc-demo-0.0.1/meta_edc/settings/minimal.py
--rw-r--r--   0 estellaye   (501) staff       (20)      610 2023-06-27 05:12:49.000000 meta-edc-demo-0.0.1/meta_edc/settings/uat.py
-drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-06-27 05:23:34.664370 meta-edc-demo-0.0.1/meta_edc/templates/
-drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-06-27 05:23:34.664423 meta-edc-demo-0.0.1/meta_edc/templates/meta_edc/
-drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-06-27 05:23:34.702378 meta-edc-demo-0.0.1/meta_edc/templates/meta_edc/bootstrap3/
--rw-r--r--   0 estellaye   (501) staff       (20)      165 2021-08-09 19:25:29.000000 meta-edc-demo-0.0.1/meta_edc/templates/meta_edc/bootstrap3/base.html
--rw-r--r--   0 estellaye   (501) staff       (20)     3780 2022-08-26 02:59:33.000000 meta-edc-demo-0.0.1/meta_edc/templates/meta_edc/bootstrap3/home.html
-drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-06-27 05:23:34.702599 meta-edc-demo-0.0.1/meta_edc/tests/
--rw-r--r--   0 estellaye   (501) staff       (20)        0 2020-03-04 23:21:43.000000 meta-edc-demo-0.0.1/meta_edc/tests/__init__.py
-drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-06-27 05:23:34.702851 meta-edc-demo-0.0.1/meta_edc/tests/tests/
--rw-r--r--   0 estellaye   (501) staff       (20)        0 2021-08-09 19:25:29.000000 meta-edc-demo-0.0.1/meta_edc/tests/tests/__init__.py
--rw-r--r--   0 estellaye   (501) staff       (20)    22422 2022-09-15 02:57:38.000000 meta-edc-demo-0.0.1/meta_edc/tests/tests/test_endpoints.py
--rw-r--r--   0 estellaye   (501) staff       (20)     3330 2022-10-07 03:13:37.000000 meta-edc-demo-0.0.1/meta_edc/urls.py
--rw-r--r--   0 estellaye   (501) staff       (20)      342 2022-06-24 09:07:39.000000 meta-edc-demo-0.0.1/meta_edc/utils.py
-drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-06-27 05:23:34.703226 meta-edc-demo-0.0.1/meta_edc/views/
--rw-r--r--   0 estellaye   (501) staff       (20)       32 2020-03-04 23:21:43.000000 meta-edc-demo-0.0.1/meta_edc/views/__init__.py
--rw-r--r--   0 estellaye   (501) staff       (20)      992 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.1/meta_edc/views/home_view.py
--rw-r--r--   0 estellaye   (501) staff       (20)      175 2020-04-03 04:33:09.000000 meta-edc-demo-0.0.1/meta_edc/wsgi.py
--rw-r--r--   0 estellaye   (501) staff       (20)      174 2020-04-03 04:33:09.000000 meta-edc-demo-0.0.1/meta_edc/wsgi_live.py
--rw-r--r--   0 estellaye   (501) staff       (20)      173 2020-04-03 04:33:09.000000 meta-edc-demo-0.0.1/meta_edc/wsgi_uat.py
-drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-06-27 05:23:34.704079 meta-edc-demo-0.0.1/meta_edc_demo.egg-info/
--rw-r--r--   0 estellaye   (501) staff       (20)      585 2023-06-27 05:23:34.000000 meta-edc-demo-0.0.1/meta_edc_demo.egg-info/PKG-INFO
--rw-r--r--   0 estellaye   (501) staff       (20)    36359 2023-06-27 05:23:34.000000 meta-edc-demo-0.0.1/meta_edc_demo.egg-info/SOURCES.txt
--rw-r--r--   0 estellaye   (501) staff       (20)        1 2023-06-27 05:23:34.000000 meta-edc-demo-0.0.1/meta_edc_demo.egg-info/dependency_links.txt
--rw-r--r--   0 estellaye   (501) staff       (20)        1 2023-06-27 05:23:34.000000 meta-edc-demo-0.0.1/meta_edc_demo.egg-info/not-zip-safe
--rw-r--r--   0 estellaye   (501) staff       (20)       56 2023-06-27 05:23:34.000000 meta-edc-demo-0.0.1/meta_edc_demo.egg-info/requires.txt
--rw-r--r--   0 estellaye   (501) staff       (20)      233 2023-06-27 05:23:34.000000 meta-edc-demo-0.0.1/meta_edc_demo.egg-info/top_level.txt
-drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-06-27 05:23:34.704605 meta-edc-demo-0.0.1/meta_export/
--rw-r--r--   0 estellaye   (501) staff       (20)        0 2020-03-15 03:34:20.000000 meta-edc-demo-0.0.1/meta_export/__init__.py
--rw-r--r--   0 estellaye   (501) staff       (20)      167 2021-07-02 03:53:00.000000 meta-edc-demo-0.0.1/meta_export/admin_site.py
--rw-r--r--   0 estellaye   (501) staff       (20)      226 2021-08-09 19:25:29.000000 meta-edc-demo-0.0.1/meta_export/apps.py
--rw-r--r--   0 estellaye   (501) staff       (20)      205 2022-06-24 09:12:54.000000 meta-edc-demo-0.0.1/meta_export/urls.py
-drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-06-27 05:23:34.705746 meta-edc-demo-0.0.1/meta_labs/
--rw-r--r--   0 estellaye   (501) staff       (20)        0 2021-07-02 03:53:00.000000 meta-edc-demo-0.0.1/meta_labs/__init__.py
--rw-r--r--   0 estellaye   (501) staff       (20)       87 2021-07-05 19:24:26.000000 meta-edc-demo-0.0.1/meta_labs/aliquot_types.py
--rw-r--r--   0 estellaye   (501) staff       (20)      200 2022-08-23 13:24:02.000000 meta-edc-demo-0.0.1/meta_labs/apps.py
--rw-r--r--   0 estellaye   (501) staff       (20)      957 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.1/meta_labs/lab_profiles.py
--rw-r--r--   0 estellaye   (501) staff       (20)      128 2022-06-24 09:12:03.000000 meta-edc-demo-0.0.1/meta_labs/labs.py
--rw-r--r--   0 estellaye   (501) staff       (20)      477 2022-06-24 09:12:00.000000 meta-edc-demo-0.0.1/meta_labs/list_data.py
--rw-r--r--   0 estellaye   (501) staff       (20)      500 2022-06-24 09:11:58.000000 meta-edc-demo-0.0.1/meta_labs/processing_profiles.py
--rw-r--r--   0 estellaye   (501) staff       (20)      512 2022-07-19 19:44:25.000000 meta-edc-demo-0.0.1/meta_labs/reportables.py
-drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-06-27 05:23:34.706314 meta-edc-demo-0.0.1/meta_labs/tests/
--rw-r--r--   0 estellaye   (501) staff       (20)        0 2020-03-15 03:34:20.000000 meta-edc-demo-0.0.1/meta_labs/tests/__init__.py
--rw-r--r--   0 estellaye   (501) staff       (20)      967 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.1/meta_labs/tests/test_labs.py
--rw-r--r--   0 estellaye   (501) staff       (20)      516 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.1/meta_labs/tests/test_reportables.py
--rw-r--r--   0 estellaye   (501) staff       (20)      111 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.1/meta_labs/tests/urls.py
-drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-06-27 05:23:34.707298 meta-edc-demo-0.0.1/meta_lists/
--rw-r--r--   0 estellaye   (501) staff       (20)        0 2020-03-15 03:34:20.000000 meta-edc-demo-0.0.1/meta_lists/__init__.py
--rw-r--r--   0 estellaye   (501) staff       (20)     1400 2022-06-24 09:11:32.000000 meta-edc-demo-0.0.1/meta_lists/admin.py
--rw-r--r--   0 estellaye   (501) staff       (20)      165 2022-06-24 09:11:34.000000 meta-edc-demo-0.0.1/meta_lists/admin_site.py
--rw-r--r--   0 estellaye   (501) staff       (20)      278 2022-08-23 13:24:02.000000 meta-edc-demo-0.0.1/meta_lists/apps.py
--rw-r--r--   0 estellaye   (501) staff       (20)     7823 2022-07-08 07:31:04.000000 meta-edc-demo-0.0.1/meta_lists/list_data.py
-drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-06-27 05:23:34.709666 meta-edc-demo-0.0.1/meta_lists/migrations/
--rw-r--r--   0 estellaye   (501) staff       (20)    13882 2020-03-15 03:34:20.000000 meta-edc-demo-0.0.1/meta_lists/migrations/0001_initial.py
--rw-r--r--   0 estellaye   (501) staff       (20)     4609 2022-08-22 17:23:22.000000 meta-edc-demo-0.0.1/meta_lists/migrations/0002_auto_20191026_2231.py
--rw-r--r--   0 estellaye   (501) staff       (20)     2556 2020-03-15 03:34:20.000000 meta-edc-demo-0.0.1/meta_lists/migrations/0003_auto_20191102_0033.py
--rw-r--r--   0 estellaye   (501) staff       (20)     2548 2020-03-15 03:34:20.000000 meta-edc-demo-0.0.1/meta_lists/migrations/0004_auto_20191102_1859.py
--rw-r--r--   0 estellaye   (501) staff       (20)     2584 2020-03-15 03:34:20.000000 meta-edc-demo-0.0.1/meta_lists/migrations/0005_auto_20191104_0930.py
--rw-r--r--   0 estellaye   (501) staff       (20)     4479 2020-05-15 02:40:42.000000 meta-edc-demo-0.0.1/meta_lists/migrations/0006_auto_20200514_1959.py
--rw-r--r--   0 estellaye   (501) staff       (20)     2962 2020-05-20 04:57:20.000000 meta-edc-demo-0.0.1/meta_lists/migrations/0007_auto_20200516_2356.py
--rw-r--r--   0 estellaye   (501) staff       (20)      683 2021-08-09 19:25:29.000000 meta-edc-demo-0.0.1/meta_lists/migrations/0008_auto_20200528_1517.py
--rw-r--r--   0 estellaye   (501) staff       (20)      358 2020-06-18 19:11:34.000000 meta-edc-demo-0.0.1/meta_lists/migrations/0009_auto_20200613_2041.py
--rw-r--r--   0 estellaye   (501) staff       (20)     1195 2022-06-24 09:11:24.000000 meta-edc-demo-0.0.1/meta_lists/migrations/0010_auto_20200617_1738.py
--rw-r--r--   0 estellaye   (501) staff       (20)     1849 2022-06-24 09:11:21.000000 meta-edc-demo-0.0.1/meta_lists/migrations/0011_auto_20210624_0225.py
--rw-r--r--   0 estellaye   (501) staff       (20)     2812 2022-06-24 09:11:19.000000 meta-edc-demo-0.0.1/meta_lists/migrations/0012_auto_20210728_1809.py
--rw-r--r--   0 estellaye   (501) staff       (20)     2534 2022-08-22 17:23:22.000000 meta-edc-demo-0.0.1/meta_lists/migrations/0013_transferreasons_and_more.py
--rw-r--r--   0 estellaye   (501) staff       (20)     2528 2022-09-15 02:57:38.000000 meta-edc-demo-0.0.1/meta_lists/migrations/0014_auto_20220913_2139.py
--rw-r--r--   0 estellaye   (501) staff       (20)        0 2020-03-15 03:34:20.000000 meta-edc-demo-0.0.1/meta_lists/migrations/__init__.py
--rw-r--r--   0 estellaye   (501) staff       (20)     2011 2022-07-08 07:31:04.000000 meta-edc-demo-0.0.1/meta_lists/models.py
-drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-06-27 05:23:34.709873 meta-edc-demo-0.0.1/meta_lists/tests/
--rw-r--r--   0 estellaye   (501) staff       (20)        0 2020-03-15 03:34:20.000000 meta-edc-demo-0.0.1/meta_lists/tests/__init__.py
--rw-r--r--   0 estellaye   (501) staff       (20)      212 2022-06-24 09:11:29.000000 meta-edc-demo-0.0.1/meta_lists/tests/test_lists.py
--rw-r--r--   0 estellaye   (501) staff       (20)      204 2021-08-09 19:25:29.000000 meta-edc-demo-0.0.1/meta_lists/urls.py
-drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-06-27 05:23:34.710489 meta-edc-demo-0.0.1/meta_pharmacy/
--rw-r--r--   0 estellaye   (501) staff       (20)        0 2022-04-11 18:27:09.000000 meta-edc-demo-0.0.1/meta_pharmacy/__init__.py
--rw-r--r--   0 estellaye   (501) staff       (20)      599 2022-08-23 13:24:02.000000 meta-edc-demo-0.0.1/meta_pharmacy/apps.py
--rw-r--r--   0 estellaye   (501) staff       (20)       24 2022-04-11 18:27:09.000000 meta-edc-demo-0.0.1/meta_pharmacy/constants.py
-drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-06-27 05:23:34.710630 meta-edc-demo-0.0.1/meta_pharmacy/migrations/
--rw-r--r--   0 estellaye   (501) staff       (20)        0 2022-04-11 18:27:09.000000 meta-edc-demo-0.0.1/meta_pharmacy/migrations/__init__.py
--rw-r--r--   0 estellaye   (501) staff       (20)        0 2022-04-11 18:27:09.000000 meta-edc-demo-0.0.1/meta_pharmacy/models.py
--rw-r--r--   0 estellaye   (501) staff       (20)     2945 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.1/meta_pharmacy/prepare_meta_pharmacy.py
-drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-06-27 05:23:34.712127 meta-edc-demo-0.0.1/meta_prn/
--rw-r--r--   0 estellaye   (501) staff       (20)        0 2020-03-15 03:34:20.000000 meta-edc-demo-0.0.1/meta_prn/__init__.py
--rw-r--r--   0 estellaye   (501) staff       (20)     7449 2022-09-27 03:17:01.000000 meta-edc-demo-0.0.1/meta_prn/action_items.py
-drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-06-27 05:23:34.713937 meta-edc-demo-0.0.1/meta_prn/admin/
--rw-r--r--   0 estellaye   (501) staff       (20)      591 2022-09-26 19:37:19.000000 meta-edc-demo-0.0.1/meta_prn/admin/__init__.py
--rw-r--r--   0 estellaye   (501) staff       (20)     5155 2022-09-26 19:37:19.000000 meta-edc-demo-0.0.1/meta_prn/admin/end_of_study_admin.py
--rw-r--r--   0 estellaye   (501) staff       (20)     1770 2022-08-23 13:24:02.000000 meta-edc-demo-0.0.1/meta_prn/admin/loss_to_followup_admin.py
--rw-r--r--   0 estellaye   (501) staff       (20)     2411 2022-09-26 19:37:19.000000 meta-edc-demo-0.0.1/meta_prn/admin/off_study_medication_admin.py
--rw-r--r--   0 estellaye   (501) staff       (20)     1741 2022-08-23 13:24:02.000000 meta-edc-demo-0.0.1/meta_prn/admin/offschedule_admin.py
--rw-r--r--   0 estellaye   (501) staff       (20)     1655 2022-08-23 13:24:02.000000 meta-edc-demo-0.0.1/meta_prn/admin/offschedule_postnatal_admin.py
--rw-r--r--   0 estellaye   (501) staff       (20)     1737 2022-08-23 13:24:02.000000 meta-edc-demo-0.0.1/meta_prn/admin/offschedule_pregnancy_admin.py
--rw-r--r--   0 estellaye   (501) staff       (20)     1474 2022-08-23 13:24:02.000000 meta-edc-demo-0.0.1/meta_prn/admin/onschedule_admin.py
--rw-r--r--   0 estellaye   (501) staff       (20)     2178 2022-08-23 13:24:02.000000 meta-edc-demo-0.0.1/meta_prn/admin/pregnancy_notification_admin.py
--rw-r--r--   0 estellaye   (501) staff       (20)     4039 2022-09-26 19:37:19.000000 meta-edc-demo-0.0.1/meta_prn/admin/protocol_incident_admin.py
--rw-r--r--   0 estellaye   (501) staff       (20)      651 2022-08-23 13:24:02.000000 meta-edc-demo-0.0.1/meta_prn/admin/subject_transfer_admin.py
--rw-r--r--   0 estellaye   (501) staff       (20)      161 2022-06-24 09:09:37.000000 meta-edc-demo-0.0.1/meta_prn/admin_site.py
--rw-r--r--   0 estellaye   (501) staff       (20)      280 2022-08-23 13:24:02.000000 meta-edc-demo-0.0.1/meta_prn/apps.py
--rw-r--r--   0 estellaye   (501) staff       (20)      517 2022-04-11 18:27:09.000000 meta-edc-demo-0.0.1/meta_prn/baker_recipes.py
--rw-r--r--   0 estellaye   (501) staff       (20)     3157 2022-07-08 07:31:04.000000 meta-edc-demo-0.0.1/meta_prn/choices.py
--rw-r--r--   0 estellaye   (501) staff       (20)      882 2022-07-08 07:31:04.000000 meta-edc-demo-0.0.1/meta_prn/constants.py
-drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-06-27 05:23:34.714377 meta-edc-demo-0.0.1/meta_prn/form_validators/
--rw-r--r--   0 estellaye   (501) staff       (20)      111 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.1/meta_prn/form_validators/__init__.py
--rw-r--r--   0 estellaye   (501) staff       (20)    11247 2022-10-04 03:17:15.000000 meta-edc-demo-0.0.1/meta_prn/form_validators/end_of_study.py
--rw-r--r--   0 estellaye   (501) staff       (20)     1069 2022-10-04 03:17:15.000000 meta-edc-demo-0.0.1/meta_prn/form_validators/protocol_incident.py
-drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-06-27 05:23:34.715707 meta-edc-demo-0.0.1/meta_prn/forms/
--rw-r--r--   0 estellaye   (501) staff       (20)      452 2022-09-26 19:37:19.000000 meta-edc-demo-0.0.1/meta_prn/forms/__init__.py
--rw-r--r--   0 estellaye   (501) staff       (20)      927 2022-10-04 03:17:15.000000 meta-edc-demo-0.0.1/meta_prn/forms/end_of_study_form.py
--rw-r--r--   0 estellaye   (501) staff       (20)     1334 2022-10-04 03:17:15.000000 meta-edc-demo-0.0.1/meta_prn/forms/loss_to_followup_form.py
--rw-r--r--   0 estellaye   (501) staff       (20)     2296 2022-10-04 03:17:15.000000 meta-edc-demo-0.0.1/meta_prn/forms/off_study_medication_form.py
--rw-r--r--   0 estellaye   (501) staff       (20)      940 2022-10-04 03:17:15.000000 meta-edc-demo-0.0.1/meta_prn/forms/offschedule_form.py
--rw-r--r--   0 estellaye   (501) staff       (20)     1102 2022-10-04 03:17:15.000000 meta-edc-demo-0.0.1/meta_prn/forms/offschedule_pregnancy_form.py
--rw-r--r--   0 estellaye   (501) staff       (20)     4883 2022-10-04 03:17:15.000000 meta-edc-demo-0.0.1/meta_prn/forms/pregnancy_notification_form.py
--rw-r--r--   0 estellaye   (501) staff       (20)      231 2022-09-27 03:17:01.000000 meta-edc-demo-0.0.1/meta_prn/forms/protocol_incident_form.py
--rw-r--r--   0 estellaye   (501) staff       (20)      818 2022-10-04 03:17:15.000000 meta-edc-demo-0.0.1/meta_prn/forms/subject_transfer_form.py
--rw-r--r--   0 estellaye   (501) staff       (20)     2336 2022-09-27 03:17:01.000000 meta-edc-demo-0.0.1/meta_prn/list_data.py
-drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-06-27 05:23:34.724668 meta-edc-demo-0.0.1/meta_prn/migrations/
--rw-r--r--   0 estellaye   (501) staff       (20)   108120 2022-09-30 02:18:01.000000 meta-edc-demo-0.0.1/meta_prn/migrations/0001_initial.py
--rw-r--r--   0 estellaye   (501) staff       (20)     2332 2021-07-05 19:24:26.000000 meta-edc-demo-0.0.1/meta_prn/migrations/0002_auto_20191024_1000.py
--rw-r--r--   0 estellaye   (501) staff       (20)      882 2020-04-08 01:09:11.000000 meta-edc-demo-0.0.1/meta_prn/migrations/0003_auto_20200120_2020.py
--rw-r--r--   0 estellaye   (501) staff       (20)      756 2020-04-08 01:09:11.000000 meta-edc-demo-0.0.1/meta_prn/migrations/0004_auto_20200403_0332.py
--rw-r--r--   0 estellaye   (501) staff       (20)     4270 2021-07-05 19:24:26.000000 meta-edc-demo-0.0.1/meta_prn/migrations/0005_auto_20200524_1944.py
--rw-r--r--   0 estellaye   (501) staff       (20)    13109 2021-07-05 19:24:26.000000 meta-edc-demo-0.0.1/meta_prn/migrations/0006_auto_20210624_0225.py
--rw-r--r--   0 estellaye   (501) staff       (20)      880 2022-04-11 18:27:09.000000 meta-edc-demo-0.0.1/meta_prn/migrations/0007_auto_20210721_0335.py
--rw-r--r--   0 estellaye   (501) staff       (20)     3640 2022-09-27 03:17:01.000000 meta-edc-demo-0.0.1/meta_prn/migrations/0008_auto_20210910_0238.py
--rw-r--r--   0 estellaye   (501) staff       (20)     2873 2022-09-27 03:17:01.000000 meta-edc-demo-0.0.1/meta_prn/migrations/0009_auto_20210910_0239.py
--rw-r--r--   0 estellaye   (501) staff       (20)     2792 2022-09-27 03:17:01.000000 meta-edc-demo-0.0.1/meta_prn/migrations/0010_auto_20210910_1906.py
--rw-r--r--   0 estellaye   (501) staff       (20)      897 2022-09-27 03:17:01.000000 meta-edc-demo-0.0.1/meta_prn/migrations/0011_auto_20210910_1911.py
--rw-r--r--   0 estellaye   (501) staff       (20)      746 2022-09-27 03:17:01.000000 meta-edc-demo-0.0.1/meta_prn/migrations/0012_auto_20210911_0004.py
--rw-r--r--   0 estellaye   (501) staff       (20)     3118 2022-04-11 18:27:09.000000 meta-edc-demo-0.0.1/meta_prn/migrations/0013_auto_20210911_2036.py
--rw-r--r--   0 estellaye   (501) staff       (20)      766 2022-06-24 09:10:52.000000 meta-edc-demo-0.0.1/meta_prn/migrations/0014_auto_20211003_1709.py
--rw-r--r--   0 estellaye   (501) staff       (20)     5915 2022-09-27 03:17:01.000000 meta-edc-demo-0.0.1/meta_prn/migrations/0015_auto_20211104_1447.py
--rw-r--r--   0 estellaye   (501) staff       (20)     5844 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.1/meta_prn/migrations/0016_auto_20220128_1719.py
--rw-r--r--   0 estellaye   (501) staff       (20)    26859 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.1/meta_prn/migrations/0017_auto_20220307_1929.py
--rw-r--r--   0 estellaye   (501) staff       (20)    34942 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.1/meta_prn/migrations/0018_auto_20220309_2106.py
--rw-r--r--   0 estellaye   (501) staff       (20)     1166 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.1/meta_prn/migrations/0019_auto_20220309_2230.py
--rw-r--r--   0 estellaye   (501) staff       (20)     2042 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.1/meta_prn/migrations/0020_auto_20220310_0439.py
--rw-r--r--   0 estellaye   (501) staff       (20)    43329 2022-09-30 02:18:01.000000 meta-edc-demo-0.0.1/meta_prn/migrations/0021_auto_20220316_2147.py
--rw-r--r--   0 estellaye   (501) staff       (20)    27549 2022-09-30 02:18:01.000000 meta-edc-demo-0.0.1/meta_prn/migrations/0022_auto_20220318_0133.py
--rw-r--r--   0 estellaye   (501) staff       (20)     2419 2022-09-30 02:18:01.000000 meta-edc-demo-0.0.1/meta_prn/migrations/0023_auto_20220415_1747.py
--rw-r--r--   0 estellaye   (501) staff       (20)      793 2022-09-27 03:17:01.000000 meta-edc-demo-0.0.1/meta_prn/migrations/0024_alter_protocoldeviationviolation_violation.py
--rw-r--r--   0 estellaye   (501) staff       (20)     6265 2022-09-27 03:17:01.000000 meta-edc-demo-0.0.1/meta_prn/migrations/0025_alter_historicalprotocoldeviationviolation_options_and_more.py
--rw-r--r--   0 estellaye   (501) staff       (20)     3926 2022-09-27 03:17:01.000000 meta-edc-demo-0.0.1/meta_prn/migrations/0026_remove_historicalprotocoldeviationviolation_violation_type_and_more.py
--rw-r--r--   0 estellaye   (501) staff       (20)     1285 2022-09-27 03:17:01.000000 meta-edc-demo-0.0.1/meta_prn/migrations/0027_rename_historicalprotocoldeviationviolation_historicalprotocolincident_and_more.py
--rw-r--r--   0 estellaye   (501) staff       (20)     1920 2022-08-22 17:23:22.000000 meta-edc-demo-0.0.1/meta_prn/migrations/0028_historicalpregnancynotification_bhcg_date_and_more.py
--rw-r--r--   0 estellaye   (501) staff       (20)      662 2022-08-22 17:23:22.000000 meta-edc-demo-0.0.1/meta_prn/migrations/0029_alter_historicalpregnancynotification_edd_and_more.py
--rw-r--r--   0 estellaye   (501) staff       (20)     1255 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.1/meta_prn/migrations/0030_auto_20220627_1119.py
--rw-r--r--   0 estellaye   (501) staff       (20)     1841 2022-08-22 17:23:22.000000 meta-edc-demo-0.0.1/meta_prn/migrations/0031_alter_historicaloffschedule_options_and_more.py
--rw-r--r--   0 estellaye   (501) staff       (20)    17576 2022-09-30 02:18:01.000000 meta-edc-demo-0.0.1/meta_prn/migrations/0032_historicalegfrnotification_egfrnotification.py
--rw-r--r--   0 estellaye   (501) staff       (20)     1070 2022-08-22 17:23:22.000000 meta-edc-demo-0.0.1/meta_prn/migrations/0033_remove_historicalegfrnotification_action_item_and_more.py
--rw-r--r--   0 estellaye   (501) staff       (20)     2076 2022-09-27 03:17:01.000000 meta-edc-demo-0.0.1/meta_prn/migrations/0034_auto_20220630_1110.py
--rw-r--r--   0 estellaye   (501) staff       (20)     3448 2022-10-11 02:24:52.000000 meta-edc-demo-0.0.1/meta_prn/migrations/0035_auto_20220630_1140.py
--rw-r--r--   0 estellaye   (501) staff       (20)     1392 2022-08-22 17:23:22.000000 meta-edc-demo-0.0.1/meta_prn/migrations/0036_remove_endofstudy_meta_prn_en_id_a50384_idx_and_more.py
--rw-r--r--   0 estellaye   (501) staff       (20)     7339 2022-08-22 17:23:22.000000 meta-edc-demo-0.0.1/meta_prn/migrations/0037_endofstudy_delivery_date_endofstudy_pregnancy_date_and_more.py
--rw-r--r--   0 estellaye   (501) staff       (20)    21786 2022-09-30 02:18:01.000000 meta-edc-demo-0.0.1/meta_prn/migrations/0038_alter_endofstudy_delivery_date_and_more.py
--rw-r--r--   0 estellaye   (501) staff       (20)     1012 2022-08-22 17:23:22.000000 meta-edc-demo-0.0.1/meta_prn/migrations/0039_historicaloffstudymedication_reason_other_and_more.py
--rw-r--r--   0 estellaye   (501) staff       (20)     4594 2022-08-22 17:23:22.000000 meta-edc-demo-0.0.1/meta_prn/migrations/0040_remove_historicaloffstudymedication_expected_restart_date_and_more.py
--rw-r--r--   0 estellaye   (501) staff       (20)    26300 2022-09-30 02:18:01.000000 meta-edc-demo-0.0.1/meta_prn/migrations/0041_endofstudy_transfer_date_and_more.py
--rw-r--r--   0 estellaye   (501) staff       (20)     6199 2022-08-22 17:23:22.000000 meta-edc-demo-0.0.1/meta_prn/migrations/0042_remove_endofstudy_investigator_decision_and_more.py
--rw-r--r--   0 estellaye   (501) staff       (20)     7240 2022-08-22 17:23:22.000000 meta-edc-demo-0.0.1/meta_prn/migrations/0043_auto_20220704_1841.py
--rw-r--r--   0 estellaye   (501) staff       (20)     3926 2022-08-23 13:31:01.000000 meta-edc-demo-0.0.1/meta_prn/migrations/0044_alter_endofstudy_action_identifier_and_more.py
--rw-r--r--   0 estellaye   (501) staff       (20)     4150 2022-08-26 02:59:33.000000 meta-edc-demo-0.0.1/meta_prn/migrations/0045_auto_20220826_0258.py
--rw-r--r--   0 estellaye   (501) staff       (20)     3945 2022-08-26 02:59:33.000000 meta-edc-demo-0.0.1/meta_prn/migrations/0046_auto_20220826_0322.py
--rw-r--r--   0 estellaye   (501) staff       (20)     2587 2022-08-26 02:59:33.000000 meta-edc-demo-0.0.1/meta_prn/migrations/0047_auto_20220826_0406.py
--rw-r--r--   0 estellaye   (501) staff       (20)     2497 2022-09-26 19:37:19.000000 meta-edc-demo-0.0.1/meta_prn/migrations/0048_auto_20220922_2236.py
--rw-r--r--   0 estellaye   (501) staff       (20)     3937 2022-09-30 02:18:01.000000 meta-edc-demo-0.0.1/meta_prn/migrations/0049_auto_20220929_1742.py
--rw-r--r--   0 estellaye   (501) staff       (20)     1251 2022-10-04 03:32:52.000000 meta-edc-demo-0.0.1/meta_prn/migrations/0050_auto_20221004_0629.py
--rw-r--r--   0 estellaye   (501) staff       (20)        0 2020-03-15 03:34:20.000000 meta-edc-demo-0.0.1/meta_prn/migrations/__init__.py
-drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-06-27 05:23:34.726075 meta-edc-demo-0.0.1/meta_prn/models/
--rw-r--r--   0 estellaye   (501) staff       (20)      594 2022-09-26 19:37:19.000000 meta-edc-demo-0.0.1/meta_prn/models/__init__.py
--rw-r--r--   0 estellaye   (501) staff       (20)     5311 2022-09-30 02:18:01.000000 meta-edc-demo-0.0.1/meta_prn/models/end_of_study.py
--rw-r--r--   0 estellaye   (501) staff       (20)     2431 2022-09-30 02:18:01.000000 meta-edc-demo-0.0.1/meta_prn/models/loss_to_followup.py
--rw-r--r--   0 estellaye   (501) staff       (20)     1696 2022-10-04 03:17:15.000000 meta-edc-demo-0.0.1/meta_prn/models/off_study_medication.py
--rw-r--r--   0 estellaye   (501) staff       (20)     1310 2022-09-30 02:18:01.000000 meta-edc-demo-0.0.1/meta_prn/models/offschedule.py
--rw-r--r--   0 estellaye   (501) staff       (20)      672 2022-09-30 02:18:01.000000 meta-edc-demo-0.0.1/meta_prn/models/onschedule.py
--rw-r--r--   0 estellaye   (501) staff       (20)     3124 2022-09-30 02:18:01.000000 meta-edc-demo-0.0.1/meta_prn/models/pregnancy_notification.py
--rw-r--r--   0 estellaye   (501) staff       (20)     1084 2022-09-30 02:18:01.000000 meta-edc-demo-0.0.1/meta_prn/models/protocol_incident.py
--rw-r--r--   0 estellaye   (501) staff       (20)     2480 2022-09-26 19:37:19.000000 meta-edc-demo-0.0.1/meta_prn/models/signals.py
--rw-r--r--   0 estellaye   (501) staff       (20)      266 2022-09-30 02:18:01.000000 meta-edc-demo-0.0.1/meta_prn/models/subject_transfer.py
--rw-r--r--   0 estellaye   (501) staff       (20)      978 2022-09-26 19:37:19.000000 meta-edc-demo-0.0.1/meta_prn/pregnancy_action_item_mixin.py
-drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-06-27 05:23:34.726321 meta-edc-demo-0.0.1/meta_prn/tests/
--rw-r--r--   0 estellaye   (501) staff       (20)        0 2020-03-15 03:34:20.000000 meta-edc-demo-0.0.1/meta_prn/tests/__init__.py
-drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-06-27 05:23:34.726868 meta-edc-demo-0.0.1/meta_prn/tests/tests/
--rw-r--r--   0 estellaye   (501) staff       (20)        0 2020-03-15 03:34:20.000000 meta-edc-demo-0.0.1/meta_prn/tests/tests/__init__.py
--rw-r--r--   0 estellaye   (501) staff       (20)     3767 2022-07-08 07:31:04.000000 meta-edc-demo-0.0.1/meta_prn/tests/tests/test_actions.py
--rw-r--r--   0 estellaye   (501) staff       (20)      557 2022-10-04 03:17:15.000000 meta-edc-demo-0.0.1/meta_prn/tests/tests/test_manager_order.py
--rw-r--r--   0 estellaye   (501) staff       (20)     3983 2022-06-24 09:09:25.000000 meta-edc-demo-0.0.1/meta_prn/tests/tests/test_pregnancy_notification.py
--rw-r--r--   0 estellaye   (501) staff       (20)      270 2022-06-24 09:09:29.000000 meta-edc-demo-0.0.1/meta_prn/tests/urls.py
--rw-r--r--   0 estellaye   (501) staff       (20)      202 2022-06-24 09:09:57.000000 meta-edc-demo-0.0.1/meta_prn/urls.py
-drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-06-27 05:23:34.727397 meta-edc-demo-0.0.1/meta_rando/
--rw-r--r--   0 estellaye   (501) staff       (20)        0 2021-08-09 19:25:29.000000 meta-edc-demo-0.0.1/meta_rando/__init__.py
--rw-r--r--   0 estellaye   (501) staff       (20)      256 2022-08-23 13:24:02.000000 meta-edc-demo-0.0.1/meta_rando/apps.py
-drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-06-27 05:23:34.728145 meta-edc-demo-0.0.1/meta_rando/migrations/
--rw-r--r--   0 estellaye   (501) staff       (20)    13433 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.1/meta_rando/migrations/0001_initial.py
--rw-r--r--   0 estellaye   (501) staff       (20)      836 2022-08-22 17:23:22.000000 meta-edc-demo-0.0.1/meta_rando/migrations/0002_auto_20220704_1841.py
--rw-r--r--   0 estellaye   (501) staff       (20)     1226 2022-08-26 13:58:46.000000 meta-edc-demo-0.0.1/meta_rando/migrations/0003_auto_20220826_1640.py
--rw-r--r--   0 estellaye   (501) staff       (20)        0 2021-08-09 19:25:29.000000 meta-edc-demo-0.0.1/meta_rando/migrations/__init__.py
--rw-r--r--   0 estellaye   (501) staff       (20)      533 2022-08-26 02:59:33.000000 meta-edc-demo-0.0.1/meta_rando/models.py
--rw-r--r--   0 estellaye   (501) staff       (20)     1592 2022-08-22 17:23:22.000000 meta-edc-demo-0.0.1/meta_rando/randomizers.py
-drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-06-27 05:23:34.728262 meta-edc-demo-0.0.1/meta_rando/tests/
--rw-r--r--   0 estellaye   (501) staff       (20)        0 2021-08-09 19:25:29.000000 meta-edc-demo-0.0.1/meta_rando/tests/__init__.py
-drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-06-27 05:23:34.728530 meta-edc-demo-0.0.1/meta_rando/tests/tests/
--rw-r--r--   0 estellaye   (501) staff       (20)        0 2021-08-09 19:25:29.000000 meta-edc-demo-0.0.1/meta_rando/tests/tests/__init__.py
--rw-r--r--   0 estellaye   (501) staff       (20)     2279 2022-09-27 03:17:01.000000 meta-edc-demo-0.0.1/meta_rando/tests/tests/test_randomizers.py
-drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-06-27 05:23:34.729181 meta-edc-demo-0.0.1/meta_reference/
--rw-r--r--   0 estellaye   (501) staff       (20)        0 2020-03-15 03:34:20.000000 meta-edc-demo-0.0.1/meta_reference/__init__.py
--rw-r--r--   0 estellaye   (501) staff       (20)      153 2022-08-23 13:24:02.000000 meta-edc-demo-0.0.1/meta_reference/apps.py
-drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-06-27 05:23:34.729360 meta-edc-demo-0.0.1/meta_reference/migrations/
--rw-r--r--   0 estellaye   (501) staff       (20)        0 2020-06-18 19:11:34.000000 meta-edc-demo-0.0.1/meta_reference/migrations/__init__.py
--rw-r--r--   0 estellaye   (501) staff       (20)      183 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.1/meta_reference/reference_model_configs.py
-drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-06-27 05:23:34.730156 meta-edc-demo-0.0.1/meta_reports/
--rw-r--r--   0 estellaye   (501) staff       (20)        0 2020-03-15 03:34:20.000000 meta-edc-demo-0.0.1/meta_reports/__init__.py
--rw-r--r--   0 estellaye   (501) staff       (20)      143 2022-06-24 09:05:03.000000 meta-edc-demo-0.0.1/meta_reports/ae_report.py
--rw-r--r--   0 estellaye   (501) staff       (20)      734 2022-08-23 13:24:02.000000 meta-edc-demo-0.0.1/meta_reports/apps.py
--rw-r--r--   0 estellaye   (501) staff       (20)     4712 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.1/meta_reports/death_report.py
-drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-06-27 05:23:34.730334 meta-edc-demo-0.0.1/meta_reports/migrations/
--rw-r--r--   0 estellaye   (501) staff       (20)        0 2020-03-15 03:34:20.000000 meta-edc-demo-0.0.1/meta_reports/migrations/__init__.py
--rw-r--r--   0 estellaye   (501) staff       (20)        0 2020-03-15 03:34:20.000000 meta-edc-demo-0.0.1/meta_reports/models.py
--rw-r--r--   0 estellaye   (501) staff       (20)     2397 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.1/meta_reports/pdf_report.py
-drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-06-27 05:23:34.730766 meta-edc-demo-0.0.1/meta_reports/tests/
--rw-r--r--   0 estellaye   (501) staff       (20)        0 2020-03-15 03:34:20.000000 meta-edc-demo-0.0.1/meta_reports/tests/__init__.py
--rw-r--r--   0 estellaye   (501) staff       (20)     1282 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.1/meta_reports/tests/test_reports.py
--rw-r--r--   0 estellaye   (501) staff       (20)      111 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.1/meta_reports/tests/urls.py
-drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-06-27 05:23:34.732293 meta-edc-demo-0.0.1/meta_screening/
--rw-r--r--   0 estellaye   (501) staff       (20)        0 2020-03-15 03:34:20.000000 meta-edc-demo-0.0.1/meta_screening/__init__.py
-drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-06-27 05:23:34.733686 meta-edc-demo-0.0.1/meta_screening/admin/
--rw-r--r--   0 estellaye   (501) staff       (20)      298 2022-04-11 18:27:09.000000 meta-edc-demo-0.0.1/meta_screening/admin/__init__.py
--rw-r--r--   0 estellaye   (501) staff       (20)     5077 2022-08-22 17:23:22.000000 meta-edc-demo-0.0.1/meta_screening/admin/fieldsets.py
--rw-r--r--   0 estellaye   (501) staff       (20)     2749 2022-08-23 13:24:02.000000 meta-edc-demo-0.0.1/meta_screening/admin/list_filters.py
--rw-r--r--   0 estellaye   (501) staff       (20)      999 2022-08-22 17:23:22.000000 meta-edc-demo-0.0.1/meta_screening/admin/screening_part_one_admin.py
--rw-r--r--   0 estellaye   (501) staff       (20)     2524 2022-08-22 17:23:22.000000 meta-edc-demo-0.0.1/meta_screening/admin/screening_part_three_admin.py
--rw-r--r--   0 estellaye   (501) staff       (20)     1308 2022-08-22 17:23:22.000000 meta-edc-demo-0.0.1/meta_screening/admin/screening_part_two_admin.py
--rw-r--r--   0 estellaye   (501) staff       (20)     2170 2022-08-23 13:24:02.000000 meta-edc-demo-0.0.1/meta_screening/admin/subject_refusal_admin.py
--rw-r--r--   0 estellaye   (501) staff       (20)     6689 2022-10-04 03:17:15.000000 meta-edc-demo-0.0.1/meta_screening/admin/subject_screening_admin.py
--rw-r--r--   0 estellaye   (501) staff       (20)      173 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.1/meta_screening/admin_site.py
--rw-r--r--   0 estellaye   (501) staff       (20)      543 2022-08-23 13:24:02.000000 meta-edc-demo-0.0.1/meta_screening/apps.py
--rw-r--r--   0 estellaye   (501) staff       (20)     1705 2022-06-24 09:06:35.000000 meta-edc-demo-0.0.1/meta_screening/baker_recipes.py
--rw-r--r--   0 estellaye   (501) staff       (20)     1948 2022-06-24 09:06:38.000000 meta-edc-demo-0.0.1/meta_screening/calculators.py
--rw-r--r--   0 estellaye   (501) staff       (20)      789 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.1/meta_screening/choices.py
--rw-r--r--   0 estellaye   (501) staff       (20)      655 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.1/meta_screening/constants.py
-drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-06-27 05:23:34.734488 meta-edc-demo-0.0.1/meta_screening/eligibility/
--rw-r--r--   0 estellaye   (501) staff       (20)      284 2022-08-22 17:23:22.000000 meta-edc-demo-0.0.1/meta_screening/eligibility/__init__.py
--rw-r--r--   0 estellaye   (501) staff       (20)     7732 2022-07-08 07:31:04.000000 meta-edc-demo-0.0.1/meta_screening/eligibility/eligibility.py
--rw-r--r--   0 estellaye   (501) staff       (20)     1770 2022-10-13 03:34:11.000000 meta-edc-demo-0.0.1/meta_screening/eligibility/eligibility_part_one.py
-drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-06-27 05:23:34.735072 meta-edc-demo-0.0.1/meta_screening/eligibility/eligibility_part_three/
--rw-r--r--   0 estellaye   (501) staff       (20)       79 2022-04-11 18:27:09.000000 meta-edc-demo-0.0.1/meta_screening/eligibility/eligibility_part_three/__init__.py
--rw-r--r--   0 estellaye   (501) staff       (20)     5405 2022-10-13 03:34:11.000000 meta-edc-demo-0.0.1/meta_screening/eligibility/eligibility_part_three/base_eligibility_part_three.py
--rw-r--r--   0 estellaye   (501) staff       (20)     4296 2022-10-13 03:34:11.000000 meta-edc-demo-0.0.1/meta_screening/eligibility/eligibility_part_three/eligibility_part_three_phase_three.py
--rw-r--r--   0 estellaye   (501) staff       (20)     1809 2022-10-13 03:34:11.000000 meta-edc-demo-0.0.1/meta_screening/eligibility/eligibility_part_two.py
-drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-06-27 05:23:34.736192 meta-edc-demo-0.0.1/meta_screening/form_validators/
--rw-r--r--   0 estellaye   (501) staff       (20)      308 2022-04-11 18:27:09.000000 meta-edc-demo-0.0.1/meta_screening/form_validators/__init__.py
--rw-r--r--   0 estellaye   (501) staff       (20)     1361 2022-10-04 03:17:15.000000 meta-edc-demo-0.0.1/meta_screening/form_validators/screening_part_one.py
--rw-r--r--   0 estellaye   (501) staff       (20)     7745 2022-10-04 03:17:15.000000 meta-edc-demo-0.0.1/meta_screening/form_validators/screening_part_three.py
--rw-r--r--   0 estellaye   (501) staff       (20)     4712 2022-10-04 03:17:15.000000 meta-edc-demo-0.0.1/meta_screening/form_validators/screening_part_two.py
--rw-r--r--   0 estellaye   (501) staff       (20)      322 2022-10-04 03:17:15.000000 meta-edc-demo-0.0.1/meta_screening/form_validators/subject_refusal.py
--rw-r--r--   0 estellaye   (501) staff       (20)      309 2022-06-24 09:04:37.000000 meta-edc-demo-0.0.1/meta_screening/form_validators/subject_screening.py
-drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-06-27 05:23:34.737203 meta-edc-demo-0.0.1/meta_screening/forms/
--rw-r--r--   0 estellaye   (501) staff       (20)      614 2022-07-19 13:21:21.000000 meta-edc-demo-0.0.1/meta_screening/forms/__init__.py
--rw-r--r--   0 estellaye   (501) staff       (20)     3279 2022-08-22 17:23:22.000000 meta-edc-demo-0.0.1/meta_screening/forms/field_lists.py
--rw-r--r--   0 estellaye   (501) staff       (20)      518 2022-07-19 13:21:21.000000 meta-edc-demo-0.0.1/meta_screening/forms/screening_part_one_form.py
--rw-r--r--   0 estellaye   (501) staff       (20)      988 2022-07-19 13:21:21.000000 meta-edc-demo-0.0.1/meta_screening/forms/screening_part_three_form.py
--rw-r--r--   0 estellaye   (501) staff       (20)      702 2022-08-22 17:23:22.000000 meta-edc-demo-0.0.1/meta_screening/forms/screening_part_two_form.py
--rw-r--r--   0 estellaye   (501) staff       (20)      625 2022-08-22 17:23:22.000000 meta-edc-demo-0.0.1/meta_screening/forms/subject_refusal_form.py
--rw-r--r--   0 estellaye   (501) staff       (20)      560 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.1/meta_screening/forms/subject_screening_form.py
-drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-06-27 05:23:34.748259 meta-edc-demo-0.0.1/meta_screening/migrations/
--rw-r--r--   0 estellaye   (501) staff       (20)   186856 2022-08-22 17:23:22.000000 meta-edc-demo-0.0.1/meta_screening/migrations/0001_initial.py
--rw-r--r--   0 estellaye   (501) staff       (20)     4468 2020-04-08 01:09:11.000000 meta-edc-demo-0.0.1/meta_screening/migrations/0002_auto_20191020_0612.py
--rw-r--r--   0 estellaye   (501) staff       (20)     5514 2020-04-08 01:09:11.000000 meta-edc-demo-0.0.1/meta_screening/migrations/0003_auto_20191020_0627.py
--rw-r--r--   0 estellaye   (501) staff       (20)    14317 2020-04-08 01:09:11.000000 meta-edc-demo-0.0.1/meta_screening/migrations/0004_auto_20191020_0738.py
--rw-r--r--   0 estellaye   (501) staff       (20)    10373 2020-04-08 01:09:11.000000 meta-edc-demo-0.0.1/meta_screening/migrations/0005_auto_20191021_0353.py
--rw-r--r--   0 estellaye   (501) staff       (20)     6711 2020-04-08 01:09:11.000000 meta-edc-demo-0.0.1/meta_screening/migrations/0006_auto_20191022_0134.py
--rw-r--r--   0 estellaye   (501) staff       (20)      951 2021-07-05 19:24:26.000000 meta-edc-demo-0.0.1/meta_screening/migrations/0007_auto_20191024_1000.py
--rw-r--r--   0 estellaye   (501) staff       (20)     6149 2020-04-08 01:09:11.000000 meta-edc-demo-0.0.1/meta_screening/migrations/0008_auto_20191031_0745.py
--rw-r--r--   0 estellaye   (501) staff       (20)     6109 2020-04-08 01:09:11.000000 meta-edc-demo-0.0.1/meta_screening/migrations/0009_auto_20191105_0122.py
--rw-r--r--   0 estellaye   (501) staff       (20)    36964 2021-07-05 19:24:26.000000 meta-edc-demo-0.0.1/meta_screening/migrations/0010_auto_20191106_0828.py
--rw-r--r--   0 estellaye   (501) staff       (20)     7305 2021-07-05 19:24:26.000000 meta-edc-demo-0.0.1/meta_screening/migrations/0011_auto_20191107_0342.py
--rw-r--r--   0 estellaye   (501) staff       (20)      776 2022-04-11 18:27:09.000000 meta-edc-demo-0.0.1/meta_screening/migrations/0012_auto_20191107_0427.py
--rw-r--r--   0 estellaye   (501) staff       (20)     7883 2021-08-09 19:25:29.000000 meta-edc-demo-0.0.1/meta_screening/migrations/0013_auto_20191107_0442.py
--rw-r--r--   0 estellaye   (501) staff       (20)    17408 2020-04-08 01:09:11.000000 meta-edc-demo-0.0.1/meta_screening/migrations/0014_auto_20191107_0528.py
--rw-r--r--   0 estellaye   (501) staff       (20)     1187 2020-04-08 01:09:11.000000 meta-edc-demo-0.0.1/meta_screening/migrations/0015_auto_20191107_2249.py
--rw-r--r--   0 estellaye   (501) staff       (20)     4804 2020-04-08 01:09:11.000000 meta-edc-demo-0.0.1/meta_screening/migrations/0016_auto_20191119_2331.py
--rw-r--r--   0 estellaye   (501) staff       (20)     2822 2020-04-08 01:09:11.000000 meta-edc-demo-0.0.1/meta_screening/migrations/0017_auto_20191213_0314.py
--rw-r--r--   0 estellaye   (501) staff       (20)     5090 2021-08-09 19:25:29.000000 meta-edc-demo-0.0.1/meta_screening/migrations/0018_auto_20200118_1854.py
--rw-r--r--   0 estellaye   (501) staff       (20)     4109 2020-04-08 01:09:11.000000 meta-edc-demo-0.0.1/meta_screening/migrations/0019_auto_20200120_2256.py
--rw-r--r--   0 estellaye   (501) staff       (20)     8403 2020-06-18 19:11:34.000000 meta-edc-demo-0.0.1/meta_screening/migrations/0020_auto_20200524_1944.py
--rw-r--r--   0 estellaye   (501) staff       (20)    25509 2021-07-02 03:53:00.000000 meta-edc-demo-0.0.1/meta_screening/migrations/0021_auto_20210628_2105.py
--rw-r--r--   0 estellaye   (501) staff       (20)     2292 2021-07-05 19:24:26.000000 meta-edc-demo-0.0.1/meta_screening/migrations/0022_auto_20210702_0426.py
--rw-r--r--   0 estellaye   (501) staff       (20)     2893 2021-07-05 19:24:26.000000 meta-edc-demo-0.0.1/meta_screening/migrations/0023_auto_20210702_0533.py
--rw-r--r--   0 estellaye   (501) staff       (20)     4284 2022-04-11 18:27:09.000000 meta-edc-demo-0.0.1/meta_screening/migrations/0024_auto_20210710_1929.py
--rw-r--r--   0 estellaye   (501) staff       (20)     4816 2022-04-11 18:27:09.000000 meta-edc-demo-0.0.1/meta_screening/migrations/0025_auto_20210710_2247.py
--rw-r--r--   0 estellaye   (501) staff       (20)     2422 2022-06-24 08:57:53.000000 meta-edc-demo-0.0.1/meta_screening/migrations/0026_auto_20210712_0433.py
--rw-r--r--   0 estellaye   (501) staff       (20)      227 2022-06-24 08:57:50.000000 meta-edc-demo-0.0.1/meta_screening/migrations/0027_auto_20210804_0438.py
--rw-r--r--   0 estellaye   (501) staff       (20)    14430 2022-06-24 08:57:48.000000 meta-edc-demo-0.0.1/meta_screening/migrations/0028_auto_20210823_2353.py
--rw-r--r--   0 estellaye   (501) staff       (20)    25297 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.1/meta_screening/migrations/0029_auto_20211123_1645.py
--rw-r--r--   0 estellaye   (501) staff       (20)     1612 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.1/meta_screening/migrations/0030_auto_20220128_1719.py
--rw-r--r--   0 estellaye   (501) staff       (20)    10216 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.1/meta_screening/migrations/0031_auto_20220304_0448.py
--rw-r--r--   0 estellaye   (501) staff       (20)     5507 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.1/meta_screening/migrations/0032_auto_20220304_0501.py
--rw-r--r--   0 estellaye   (501) staff       (20)     2168 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.1/meta_screening/migrations/0033_auto_20220304_0504.py
--rw-r--r--   0 estellaye   (501) staff       (20)     6547 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.1/meta_screening/migrations/0034_auto_20220304_0508.py
--rw-r--r--   0 estellaye   (501) staff       (20)    36493 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.1/meta_screening/migrations/0035_auto_20220304_2233.py
--rw-r--r--   0 estellaye   (501) staff       (20)     5610 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.1/meta_screening/migrations/0036_auto_20220304_2307.py
--rw-r--r--   0 estellaye   (501) staff       (20)     5030 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.1/meta_screening/migrations/0037_auto_20220312_0339.py
--rw-r--r--   0 estellaye   (501) staff       (20)    10873 2022-06-24 08:57:21.000000 meta-edc-demo-0.0.1/meta_screening/migrations/0038_auto_20220312_1929.py
--rw-r--r--   0 estellaye   (501) staff       (20)     6643 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.1/meta_screening/migrations/0039_auto_20220312_1938.py
--rw-r--r--   0 estellaye   (501) staff       (20)    20941 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.1/meta_screening/migrations/0040_auto_20220316_2147.py
--rw-r--r--   0 estellaye   (501) staff       (20)     2663 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.1/meta_screening/migrations/0041_auto_20220403_1227.py
--rw-r--r--   0 estellaye   (501) staff       (20)    15666 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.1/meta_screening/migrations/0042_auto_20220403_1402.py
--rw-r--r--   0 estellaye   (501) staff       (20)     5505 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.1/meta_screening/migrations/0043_auto_20220407_1713.py
--rw-r--r--   0 estellaye   (501) staff       (20)     4909 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.1/meta_screening/migrations/0044_alter_historicalscreeningpartone_severe_htn_and_more.py
--rw-r--r--   0 estellaye   (501) staff       (20)     1919 2022-08-22 17:23:22.000000 meta-edc-demo-0.0.1/meta_screening/migrations/0045_historicalscreeningpartone_contact_number_and_more.py
--rw-r--r--   0 estellaye   (501) staff       (20)     1984 2022-08-22 17:23:22.000000 meta-edc-demo-0.0.1/meta_screening/migrations/0046_historicalscreeningpartone_hba1c_datetime_and_more.py
--rw-r--r--   0 estellaye   (501) staff       (20)     2354 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.1/meta_screening/migrations/0047_historicalscreeningpartone_appt_datetime_repeat_and_more.py
--rw-r--r--   0 estellaye   (501) staff       (20)     1192 2022-08-22 17:23:22.000000 meta-edc-demo-0.0.1/meta_screening/migrations/0048_rename_appt_datetime_repeat_historicalscreeningpartone_repeat_appt_datetime_and_more.py
--rw-r--r--   0 estellaye   (501) staff       (20)     9620 2022-08-22 17:23:22.000000 meta-edc-demo-0.0.1/meta_screening/migrations/0049_historicalscreeningpartone_p3_ltfu_and_more.py
--rw-r--r--   0 estellaye   (501) staff       (20)    11995 2022-08-22 17:23:22.000000 meta-edc-demo-0.0.1/meta_screening/migrations/0050_historicalscreeningpartone_agree_to_p3_and_more.py
--rw-r--r--   0 estellaye   (501) staff       (20)    11972 2022-08-22 17:23:22.000000 meta-edc-demo-0.0.1/meta_screening/migrations/0051_alter_historicalscreeningpartone_advised_to_fast_and_more.py
--rw-r--r--   0 estellaye   (501) staff       (20)     3891 2022-08-22 17:23:22.000000 meta-edc-demo-0.0.1/meta_screening/migrations/0052_alter_historicalscreeningpartone_p3_ltfu_and_more.py
--rw-r--r--   0 estellaye   (501) staff       (20)     3782 2022-08-22 17:23:22.000000 meta-edc-demo-0.0.1/meta_screening/migrations/0053_auto_20220704_1841.py
--rw-r--r--   0 estellaye   (501) staff       (20)     6029 2022-08-22 17:23:22.000000 meta-edc-demo-0.0.1/meta_screening/migrations/0054_auto_20220722_2130.py
--rw-r--r--   0 estellaye   (501) staff       (20)    18774 2022-08-22 17:23:22.000000 meta-edc-demo-0.0.1/meta_screening/migrations/0055_alter_historicalscreeningpartone_creatinine_value_and_more.py
--rw-r--r--   0 estellaye   (501) staff       (20)     4225 2022-08-23 13:24:02.000000 meta-edc-demo-0.0.1/meta_screening/migrations/0056_alter_historicalscreeningpartone_agree_to_p3_and_more.py
--rw-r--r--   0 estellaye   (501) staff       (20)    13644 2022-10-12 03:43:37.000000 meta-edc-demo-0.0.1/meta_screening/migrations/0057_alter_historicalscreeningpartone_calculated_egfr_value_and_more.py
--rw-r--r--   0 estellaye   (501) staff       (20)        0 2020-03-15 03:34:20.000000 meta-edc-demo-0.0.1/meta_screening/migrations/__init__.py
-drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-06-27 05:23:34.749298 meta-edc-demo-0.0.1/meta_screening/model_mixins/
--rw-r--r--   0 estellaye   (501) staff       (20)      315 2022-08-26 02:59:33.000000 meta-edc-demo-0.0.1/meta_screening/model_mixins/__init__.py
--rw-r--r--   0 estellaye   (501) staff       (20)     2762 2022-10-12 03:43:37.000000 meta-edc-demo-0.0.1/meta_screening/model_mixins/calculated_model_mixin.py
--rw-r--r--   0 estellaye   (501) staff       (20)      593 2022-10-12 03:43:37.000000 meta-edc-demo-0.0.1/meta_screening/model_mixins/creatinine_fields_model_mixin.py
--rw-r--r--   0 estellaye   (501) staff       (20)     1361 2022-08-26 02:59:33.000000 meta-edc-demo-0.0.1/meta_screening/model_mixins/eligibility_model_mixin.py
--rw-r--r--   0 estellaye   (501) staff       (20)     3712 2022-08-26 02:59:33.000000 meta-edc-demo-0.0.1/meta_screening/model_mixins/part_one_fields_model_mixin.py
--rw-r--r--   0 estellaye   (501) staff       (20)     5119 2022-08-26 02:59:33.000000 meta-edc-demo-0.0.1/meta_screening/model_mixins/part_three_fields_model_mixin.py
--rw-r--r--   0 estellaye   (501) staff       (20)     6693 2022-08-26 02:59:33.000000 meta-edc-demo-0.0.1/meta_screening/model_mixins/part_two_fields_model_mixin.py
-drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-06-27 05:23:34.750357 meta-edc-demo-0.0.1/meta_screening/models/
--rw-r--r--   0 estellaye   (501) staff       (20)      260 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.1/meta_screening/models/__init__.py
--rw-r--r--   0 estellaye   (501) staff       (20)     3429 2022-08-22 17:23:22.000000 meta-edc-demo-0.0.1/meta_screening/models/icp_referral.py
--rw-r--r--   0 estellaye   (501) staff       (20)     1018 2022-06-24 08:56:30.000000 meta-edc-demo-0.0.1/meta_screening/models/proxy_models.py
--rw-r--r--   0 estellaye   (501) staff       (20)      862 2022-08-26 02:59:33.000000 meta-edc-demo-0.0.1/meta_screening/models/signals.py
--rw-r--r--   0 estellaye   (501) staff       (20)     2218 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.1/meta_screening/models/subject_refusal.py
--rw-r--r--   0 estellaye   (501) staff       (20)     1592 2022-08-26 02:59:33.000000 meta-edc-demo-0.0.1/meta_screening/models/subject_screening.py
--rw-r--r--   0 estellaye   (501) staff       (20)      131 2022-06-24 09:06:52.000000 meta-edc-demo-0.0.1/meta_screening/offline_models.py
-drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-06-27 05:23:34.750872 meta-edc-demo-0.0.1/meta_screening/tests/
--rw-r--r--   0 estellaye   (501) staff       (20)        0 2020-03-15 03:34:20.000000 meta-edc-demo-0.0.1/meta_screening/tests/__init__.py
--rw-r--r--   0 estellaye   (501) staff       (20)     8283 2022-09-26 19:37:19.000000 meta-edc-demo-0.0.1/meta_screening/tests/meta_test_case_mixin.py
--rw-r--r--   0 estellaye   (501) staff       (20)     3871 2022-09-26 19:37:19.000000 meta-edc-demo-0.0.1/meta_screening/tests/options.py
-drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-06-27 05:23:34.751832 meta-edc-demo-0.0.1/meta_screening/tests/tests/
--rw-r--r--   0 estellaye   (501) staff       (20)        0 2021-08-09 19:25:30.000000 meta-edc-demo-0.0.1/meta_screening/tests/tests/__init__.py
--rw-r--r--   0 estellaye   (501) staff       (20)    16710 2022-10-04 03:16:43.000000 meta-edc-demo-0.0.1/meta_screening/tests/tests/test_forms.py
--rw-r--r--   0 estellaye   (501) staff       (20)     4723 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.1/meta_screening/tests/tests/test_screening_part_one.py
--rw-r--r--   0 estellaye   (501) staff       (20)    16775 2022-08-22 17:23:22.000000 meta-edc-demo-0.0.1/meta_screening/tests/tests/test_screening_part_three.py
--rw-r--r--   0 estellaye   (501) staff       (20)     3128 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.1/meta_screening/tests/tests/test_screening_part_two.py
--rw-r--r--   0 estellaye   (501) staff       (20)      208 2022-06-24 09:06:56.000000 meta-edc-demo-0.0.1/meta_screening/urls.py
-drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-06-27 05:23:34.752606 meta-edc-demo-0.0.1/meta_sites/
--rw-r--r--   0 estellaye   (501) staff       (20)       43 2021-07-05 19:24:26.000000 meta-edc-demo-0.0.1/meta_sites/__init__.py
--rw-r--r--   0 estellaye   (501) staff       (20)      934 2022-08-23 13:24:02.000000 meta-edc-demo-0.0.1/meta_sites/apps.py
-drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-06-27 05:23:34.752766 meta-edc-demo-0.0.1/meta_sites/migrations/
--rw-r--r--   0 estellaye   (501) staff       (20)        0 2020-06-18 19:11:34.000000 meta-edc-demo-0.0.1/meta_sites/migrations/__init__.py
--rw-r--r--   0 estellaye   (501) staff       (20)       46 2020-03-15 03:34:20.000000 meta-edc-demo-0.0.1/meta_sites/models.py
--rw-r--r--   0 estellaye   (501) staff       (20)     1420 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.1/meta_sites/sites.py
-drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-06-27 05:23:34.753153 meta-edc-demo-0.0.1/meta_sites/tests/
--rw-r--r--   0 estellaye   (501) staff       (20)        0 2020-03-15 03:34:20.000000 meta-edc-demo-0.0.1/meta_sites/tests/__init__.py
--rw-r--r--   0 estellaye   (501) staff       (20)      490 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.1/meta_sites/tests/test_sites.py
--rw-r--r--   0 estellaye   (501) staff       (20)      111 2022-06-24 09:03:07.000000 meta-edc-demo-0.0.1/meta_sites/tests/urls.py
-drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-06-27 05:23:34.755133 meta-edc-demo-0.0.1/meta_subject/
--rw-r--r--   0 estellaye   (501) staff       (20)        0 2020-03-15 03:34:20.000000 meta-edc-demo-0.0.1/meta_subject/__init__.py
--rw-r--r--   0 estellaye   (501) staff       (20)     5721 2022-08-22 17:23:22.000000 meta-edc-demo-0.0.1/meta_subject/action_items.py
-drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-06-27 05:23:34.760651 meta-edc-demo-0.0.1/meta_subject/admin/
--rw-r--r--   0 estellaye   (501) staff       (20)     1614 2022-08-23 01:12:55.000000 meta-edc-demo-0.0.1/meta_subject/admin/__init__.py
--rw-r--r--   0 estellaye   (501) staff       (20)     1158 2022-06-24 08:59:56.000000 meta-edc-demo-0.0.1/meta_subject/admin/autocomplete_admin.py
--rw-r--r--   0 estellaye   (501) staff       (20)     3223 2022-08-23 13:24:02.000000 meta-edc-demo-0.0.1/meta_subject/admin/birth_outcome_admin.py
-drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-06-27 05:23:34.762146 meta-edc-demo-0.0.1/meta_subject/admin/blood_results/
--rw-r--r--   0 estellaye   (501) staff       (20)      414 2021-08-09 19:25:30.000000 meta-edc-demo-0.0.1/meta_subject/admin/blood_results/__init__.py
--rw-r--r--   0 estellaye   (501) staff       (20)      708 2022-08-22 17:23:22.000000 meta-edc-demo-0.0.1/meta_subject/admin/blood_results/blood_results_fbc_admin.py
--rw-r--r--   0 estellaye   (501) staff       (20)      976 2022-08-22 17:23:22.000000 meta-edc-demo-0.0.1/meta_subject/admin/blood_results/blood_results_glu_admin.py
--rw-r--r--   0 estellaye   (501) staff       (20)      770 2022-08-22 17:23:22.000000 meta-edc-demo-0.0.1/meta_subject/admin/blood_results/blood_results_hba1c_admin.py
--rw-r--r--   0 estellaye   (501) staff       (20)      731 2022-08-22 17:23:22.000000 meta-edc-demo-0.0.1/meta_subject/admin/blood_results/blood_results_ins_admin.py
--rw-r--r--   0 estellaye   (501) staff       (20)      731 2022-08-22 17:23:22.000000 meta-edc-demo-0.0.1/meta_subject/admin/blood_results/blood_results_lft_admin.py
--rw-r--r--   0 estellaye   (501) staff       (20)      745 2022-08-22 17:23:22.000000 meta-edc-demo-0.0.1/meta_subject/admin/blood_results/blood_results_lipid_admin.py
--rw-r--r--   0 estellaye   (501) staff       (20)     5030 2022-09-15 05:11:27.000000 meta-edc-demo-0.0.1/meta_subject/admin/blood_results/blood_results_rft_admin.py
--rw-r--r--   0 estellaye   (501) staff       (20)     1035 2022-08-22 17:23:22.000000 meta-edc-demo-0.0.1/meta_subject/admin/complications_admin.py
--rw-r--r--   0 estellaye   (501) staff       (20)     3985 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.1/meta_subject/admin/complications_glycemia_admin.py
--rw-r--r--   0 estellaye   (501) staff       (20)      740 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.1/meta_subject/admin/concomitant_medication_admin.py
--rw-r--r--   0 estellaye   (501) staff       (20)     3427 2022-10-07 02:36:16.000000 meta-edc-demo-0.0.1/meta_subject/admin/delivery_admin.py
--rw-r--r--   0 estellaye   (501) staff       (20)      734 2022-08-23 13:24:02.000000 meta-edc-demo-0.0.1/meta_subject/admin/egfr_drop_notification_admin.py
--rw-r--r--   0 estellaye   (501) staff       (20)      676 2022-06-24 09:00:18.000000 meta-edc-demo-0.0.1/meta_subject/admin/eq5d3l_admin.py
--rw-r--r--   0 estellaye   (501) staff       (20)      277 2022-06-24 09:00:25.000000 meta-edc-demo-0.0.1/meta_subject/admin/fields.py
--rw-r--r--   0 estellaye   (501) staff       (20)     1523 2022-06-24 09:00:28.000000 meta-edc-demo-0.0.1/meta_subject/admin/fieldsets.py
--rw-r--r--   0 estellaye   (501) staff       (20)     5154 2022-08-26 02:59:33.000000 meta-edc-demo-0.0.1/meta_subject/admin/followup_examination_admin.py
--rw-r--r--   0 estellaye   (501) staff       (20)     1586 2022-08-23 13:24:02.000000 meta-edc-demo-0.0.1/meta_subject/admin/followup_vitals_admin.py
--rw-r--r--   0 estellaye   (501) staff       (20)     1613 2022-08-23 01:13:27.000000 meta-edc-demo-0.0.1/meta_subject/admin/glucose_admin.py
--rw-r--r--   0 estellaye   (501) staff       (20)      949 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.1/meta_subject/admin/health_economics_simple_admin.py
--rw-r--r--   0 estellaye   (501) staff       (20)     1320 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.1/meta_subject/admin/hepatitis_test_admin.py
--rw-r--r--   0 estellaye   (501) staff       (20)      978 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.1/meta_subject/admin/malaria_test_admin.py
--rw-r--r--   0 estellaye   (501) staff       (20)      610 2022-08-23 13:24:02.000000 meta-edc-demo-0.0.1/meta_subject/admin/medication_adherence_admin.py
--rw-r--r--   0 estellaye   (501) staff       (20)     1421 2022-08-23 13:24:02.000000 meta-edc-demo-0.0.1/meta_subject/admin/mnsi_admin.py
--rw-r--r--   0 estellaye   (501) staff       (20)      383 2022-08-23 13:24:02.000000 meta-edc-demo-0.0.1/meta_subject/admin/modeladmin.py
--rw-r--r--   0 estellaye   (501) staff       (20)     1512 2022-10-07 03:13:37.000000 meta-edc-demo-0.0.1/meta_subject/admin/other_arv_regimens_admin.py
--rw-r--r--   0 estellaye   (501) staff       (20)     1679 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.1/meta_subject/admin/patient_history_admin.py
--rw-r--r--   0 estellaye   (501) staff       (20)     1774 2022-10-05 21:51:43.000000 meta-edc-demo-0.0.1/meta_subject/admin/physical_exam_admin.py
--rw-r--r--   0 estellaye   (501) staff       (20)      829 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.1/meta_subject/admin/pregnancy_update_admin.py
--rw-r--r--   0 estellaye   (501) staff       (20)      658 2022-06-24 09:01:27.000000 meta-edc-demo-0.0.1/meta_subject/admin/sf12_admin.py
--rw-r--r--   0 estellaye   (501) staff       (20)     4232 2022-09-28 04:05:35.000000 meta-edc-demo-0.0.1/meta_subject/admin/study_medication_admin.py
--rw-r--r--   0 estellaye   (501) staff       (20)     1764 2022-08-23 13:24:02.000000 meta-edc-demo-0.0.1/meta_subject/admin/subject_requisition_admin.py
--rw-r--r--   0 estellaye   (501) staff       (20)     1315 2022-08-23 13:24:02.000000 meta-edc-demo-0.0.1/meta_subject/admin/subject_visit_admin.py
--rw-r--r--   0 estellaye   (501) staff       (20)     1399 2022-08-23 13:24:02.000000 meta-edc-demo-0.0.1/meta_subject/admin/subject_visit_missed_admin.py
--rw-r--r--   0 estellaye   (501) staff       (20)     1060 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.1/meta_subject/admin/urine_dipstick_test_admin.py
--rw-r--r--   0 estellaye   (501) staff       (20)      953 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.1/meta_subject/admin/urine_pregnancy_admin.py
--rw-r--r--   0 estellaye   (501) staff       (20)      169 2022-08-21 16:43:17.000000 meta-edc-demo-0.0.1/meta_subject/admin_site.py
--rw-r--r--   0 estellaye   (501) staff       (20)      282 2022-08-23 13:24:02.000000 meta-edc-demo-0.0.1/meta_subject/apps.py
--rw-r--r--   0 estellaye   (501) staff       (20)     2618 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.1/meta_subject/baker_recipes.py
--rw-r--r--   0 estellaye   (501) staff       (20)     6340 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.1/meta_subject/choices.py
--rw-r--r--   0 estellaye   (501) staff       (20)      599 2022-08-22 17:23:22.000000 meta-edc-demo-0.0.1/meta_subject/constants.py
-drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-06-27 05:23:34.766982 meta-edc-demo-0.0.1/meta_subject/forms/
--rw-r--r--   0 estellaye   (501) staff       (20)     1611 2022-08-22 17:23:22.000000 meta-edc-demo-0.0.1/meta_subject/forms/__init__.py
--rw-r--r--   0 estellaye   (501) staff       (20)      666 2022-09-26 19:37:19.000000 meta-edc-demo-0.0.1/meta_subject/forms/birth_outcomes_form.py
-drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-06-27 05:23:34.768320 meta-edc-demo-0.0.1/meta_subject/forms/blood_results/
--rw-r--r--   0 estellaye   (501) staff       (20)      400 2021-08-09 19:25:30.000000 meta-edc-demo-0.0.1/meta_subject/forms/blood_results/__init__.py
--rw-r--r--   0 estellaye   (501) staff       (20)      715 2022-09-26 19:37:19.000000 meta-edc-demo-0.0.1/meta_subject/forms/blood_results/blood_results_fbc_form.py
--rw-r--r--   0 estellaye   (501) staff       (20)      824 2022-09-26 19:37:19.000000 meta-edc-demo-0.0.1/meta_subject/forms/blood_results/blood_results_glu_form.py
--rw-r--r--   0 estellaye   (501) staff       (20)      766 2022-09-26 19:37:19.000000 meta-edc-demo-0.0.1/meta_subject/forms/blood_results/blood_results_hba1c_form.py
--rw-r--r--   0 estellaye   (501) staff       (20)      723 2022-09-26 19:37:19.000000 meta-edc-demo-0.0.1/meta_subject/forms/blood_results/blood_results_ins_form.py
--rw-r--r--   0 estellaye   (501) staff       (20)      715 2022-10-12 13:06:29.000000 meta-edc-demo-0.0.1/meta_subject/forms/blood_results/blood_results_lft_form.py
--rw-r--r--   0 estellaye   (501) staff       (20)      731 2022-09-26 19:37:19.000000 meta-edc-demo-0.0.1/meta_subject/forms/blood_results/blood_results_lipid_form.py
--rw-r--r--   0 estellaye   (501) staff       (20)     1363 2022-09-26 19:37:19.000000 meta-edc-demo-0.0.1/meta_subject/forms/blood_results/blood_results_rft_form.py
--rw-r--r--   0 estellaye   (501) staff       (20)      486 2022-09-26 19:37:19.000000 meta-edc-demo-0.0.1/meta_subject/forms/complications_glycemia_form.py
--rw-r--r--   0 estellaye   (501) staff       (20)      490 2022-09-26 19:37:19.000000 meta-edc-demo-0.0.1/meta_subject/forms/concomitant_medication_form.py
--rw-r--r--   0 estellaye   (501) staff       (20)     3564 2022-09-26 19:37:19.000000 meta-edc-demo-0.0.1/meta_subject/forms/delivery_form.py
--rw-r--r--   0 estellaye   (501) staff       (20)      974 2022-09-26 19:37:19.000000 meta-edc-demo-0.0.1/meta_subject/forms/egfr_drop_notification_form.py
--rw-r--r--   0 estellaye   (501) staff       (20)      598 2022-06-24 08:53:52.000000 meta-edc-demo-0.0.1/meta_subject/forms/eq53d3l_form.py
--rw-r--r--   0 estellaye   (501) staff       (20)     4591 2022-09-26 19:37:19.000000 meta-edc-demo-0.0.1/meta_subject/forms/followup_examination_form.py
--rw-r--r--   0 estellaye   (501) staff       (20)      430 2022-09-26 19:37:19.000000 meta-edc-demo-0.0.1/meta_subject/forms/followup_vitals_form.py
--rw-r--r--   0 estellaye   (501) staff       (20)      656 2022-09-26 19:37:19.000000 meta-edc-demo-0.0.1/meta_subject/forms/glucose_form.py
--rw-r--r--   0 estellaye   (501) staff       (20)      591 2022-09-26 19:37:19.000000 meta-edc-demo-0.0.1/meta_subject/forms/health_economics_simple_form.py
--rw-r--r--   0 estellaye   (501) staff       (20)      796 2022-09-26 19:37:19.000000 meta-edc-demo-0.0.1/meta_subject/forms/hepatitis_test_form.py
--rw-r--r--   0 estellaye   (501) staff       (20)      726 2022-09-26 19:37:19.000000 meta-edc-demo-0.0.1/meta_subject/forms/malaria_test_form.py
--rw-r--r--   0 estellaye   (501) staff       (20)      866 2022-09-26 19:37:19.000000 meta-edc-demo-0.0.1/meta_subject/forms/medication_adherence_form.py
--rw-r--r--   0 estellaye   (501) staff       (20)     2084 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.1/meta_subject/forms/mixins.py
--rw-r--r--   0 estellaye   (501) staff       (20)      324 2022-06-24 08:54:40.000000 meta-edc-demo-0.0.1/meta_subject/forms/mnsi_form.py
--rw-r--r--   0 estellaye   (501) staff       (20)      963 2022-10-10 11:55:19.000000 meta-edc-demo-0.0.1/meta_subject/forms/other_arv_regimens_detail_form.py
--rw-r--r--   0 estellaye   (501) staff       (20)     1688 2022-09-26 19:37:19.000000 meta-edc-demo-0.0.1/meta_subject/forms/other_arv_regimens_form.py
--rw-r--r--   0 estellaye   (501) staff       (20)     1809 2022-09-26 19:37:19.000000 meta-edc-demo-0.0.1/meta_subject/forms/patient_history_form.py
--rw-r--r--   0 estellaye   (501) staff       (20)      788 2022-10-04 20:17:27.000000 meta-edc-demo-0.0.1/meta_subject/forms/physical_exam_form.py
--rw-r--r--   0 estellaye   (501) staff       (20)      560 2022-09-26 19:37:19.000000 meta-edc-demo-0.0.1/meta_subject/forms/pregnancy_update_form.py
--rw-r--r--   0 estellaye   (501) staff       (20)      397 2022-06-24 08:54:57.000000 meta-edc-demo-0.0.1/meta_subject/forms/sf12_form.py
--rw-r--r--   0 estellaye   (501) staff       (20)      822 2022-06-24 08:55:00.000000 meta-edc-demo-0.0.1/meta_subject/forms/slider_widget.py
--rw-r--r--   0 estellaye   (501) staff       (20)     1574 2022-09-26 19:37:19.000000 meta-edc-demo-0.0.1/meta_subject/forms/study_medication_form.py
--rw-r--r--   0 estellaye   (501) staff       (20)      954 2022-09-26 19:37:19.000000 meta-edc-demo-0.0.1/meta_subject/forms/subject_requisition_form.py
--rw-r--r--   0 estellaye   (501) staff       (20)      757 2022-09-26 19:37:19.000000 meta-edc-demo-0.0.1/meta_subject/forms/subject_visit_form.py
--rw-r--r--   0 estellaye   (501) staff       (20)     2277 2022-09-26 19:37:19.000000 meta-edc-demo-0.0.1/meta_subject/forms/subject_visit_missed_form.py
--rw-r--r--   0 estellaye   (501) staff       (20)      829 2022-09-26 19:37:19.000000 meta-edc-demo-0.0.1/meta_subject/forms/urine_dipstick_test_form.py
--rw-r--r--   0 estellaye   (501) staff       (20)     1269 2022-09-26 19:37:19.000000 meta-edc-demo-0.0.1/meta_subject/forms/urine_pregnancy_form.py
--rw-r--r--   0 estellaye   (501) staff       (20)      325 2022-08-26 02:59:33.000000 meta-edc-demo-0.0.1/meta_subject/identifiers.py
-drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-06-27 05:23:34.768852 meta-edc-demo-0.0.1/meta_subject/metadata_rules/
--rw-r--r--   0 estellaye   (501) staff       (20)       53 2022-04-11 18:27:09.000000 meta-edc-demo-0.0.1/meta_subject/metadata_rules/__init__.py
--rw-r--r--   0 estellaye   (501) staff       (20)     3124 2022-08-22 17:23:22.000000 meta-edc-demo-0.0.1/meta_subject/metadata_rules/metadata_rules.py
--rw-r--r--   0 estellaye   (501) staff       (20)     6795 2022-08-22 17:23:22.000000 meta-edc-demo-0.0.1/meta_subject/metadata_rules/predicates.py
-drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-06-27 05:23:34.800341 meta-edc-demo-0.0.1/meta_subject/migrations/
--rw-r--r--   0 estellaye   (501) staff       (20)   408933 2022-09-30 02:18:01.000000 meta-edc-demo-0.0.1/meta_subject/migrations/0001_initial.py
--rw-r--r--   0 estellaye   (501) staff       (20)    29352 2022-08-22 17:23:22.000000 meta-edc-demo-0.0.1/meta_subject/migrations/0002_auto_20191021_0353.py
--rw-r--r--   0 estellaye   (501) staff       (20)     4025 2020-04-08 01:09:11.000000 meta-edc-demo-0.0.1/meta_subject/migrations/0003_auto_20191021_0534.py
--rw-r--r--   0 estellaye   (501) staff       (20)      740 2020-04-08 01:09:11.000000 meta-edc-demo-0.0.1/meta_subject/migrations/0004_auto_20191022_0134.py
--rw-r--r--   0 estellaye   (501) staff       (20)     5819 2021-07-05 19:24:26.000000 meta-edc-demo-0.0.1/meta_subject/migrations/0005_auto_20191024_1000.py
--rw-r--r--   0 estellaye   (501) staff       (20)    20051 2022-08-22 17:23:22.000000 meta-edc-demo-0.0.1/meta_subject/migrations/0006_auto_20191104_0756.py
--rw-r--r--   0 estellaye   (501) staff       (20)     1142 2020-04-08 01:09:11.000000 meta-edc-demo-0.0.1/meta_subject/migrations/0007_auto_20191107_2249.py
--rw-r--r--   0 estellaye   (501) staff       (20)    13944 2020-04-08 01:09:11.000000 meta-edc-demo-0.0.1/meta_subject/migrations/0008_auto_20191115_0132.py
--rw-r--r--   0 estellaye   (501) staff       (20)     1130 2020-04-08 01:09:11.000000 meta-edc-demo-0.0.1/meta_subject/migrations/0009_auto_20191119_2331.py
--rw-r--r--   0 estellaye   (501) staff       (20)     6880 2020-04-08 01:09:11.000000 meta-edc-demo-0.0.1/meta_subject/migrations/0010_auto_20191213_0314.py
--rw-r--r--   0 estellaye   (501) staff       (20)     2780 2022-08-22 17:23:22.000000 meta-edc-demo-0.0.1/meta_subject/migrations/0011_auto_20200118_1854.py
--rw-r--r--   0 estellaye   (501) staff       (20)    15555 2021-07-05 19:24:26.000000 meta-edc-demo-0.0.1/meta_subject/migrations/0012_auto_20200118_2334.py
--rw-r--r--   0 estellaye   (501) staff       (20)     1830 2020-04-08 01:09:11.000000 meta-edc-demo-0.0.1/meta_subject/migrations/0013_auto_20200119_0013.py
--rw-r--r--   0 estellaye   (501) staff       (20)    32039 2022-09-30 02:18:01.000000 meta-edc-demo-0.0.1/meta_subject/migrations/0014_auto_20200120_1622.py
--rw-r--r--   0 estellaye   (501) staff       (20)      786 2020-04-08 01:09:11.000000 meta-edc-demo-0.0.1/meta_subject/migrations/0015_auto_20200120_1943.py
--rw-r--r--   0 estellaye   (501) staff       (20)     2036 2020-04-08 01:09:11.000000 meta-edc-demo-0.0.1/meta_subject/migrations/0016_auto_20200123_1508.py
--rw-r--r--   0 estellaye   (501) staff       (20)     7292 2022-09-30 02:18:01.000000 meta-edc-demo-0.0.1/meta_subject/migrations/0017_auto_20200325_0901.py
--rw-r--r--   0 estellaye   (501) staff       (20)    59622 2022-08-22 17:23:22.000000 meta-edc-demo-0.0.1/meta_subject/migrations/0018_coronakap_historicalcoronakap.py
--rw-r--r--   0 estellaye   (501) staff       (20)     1561 2021-07-05 19:24:26.000000 meta-edc-demo-0.0.1/meta_subject/migrations/0019_auto_20200417_0315.py
--rw-r--r--   0 estellaye   (501) staff       (20)     7014 2021-07-05 19:24:26.000000 meta-edc-demo-0.0.1/meta_subject/migrations/0020_auto_20200417_0329.py
--rw-r--r--   0 estellaye   (501) staff       (20)     1178 2021-07-05 19:24:26.000000 meta-edc-demo-0.0.1/meta_subject/migrations/0021_auto_20200417_0332.py
--rw-r--r--   0 estellaye   (501) staff       (20)     5513 2021-08-09 19:25:30.000000 meta-edc-demo-0.0.1/meta_subject/migrations/0022_auto_20200419_2223.py
--rw-r--r--   0 estellaye   (501) staff       (20)    25416 2020-05-15 02:40:42.000000 meta-edc-demo-0.0.1/meta_subject/migrations/0023_auto_20200419_2305.py
--rw-r--r--   0 estellaye   (501) staff       (20)    14716 2020-05-15 02:40:42.000000 meta-edc-demo-0.0.1/meta_subject/migrations/0024_auto_20200419_2331.py
--rw-r--r--   0 estellaye   (501) staff       (20)     7348 2020-05-15 02:40:42.000000 meta-edc-demo-0.0.1/meta_subject/migrations/0025_auto_20200420_1455.py
--rw-r--r--   0 estellaye   (501) staff       (20)     1092 2020-05-15 02:40:42.000000 meta-edc-demo-0.0.1/meta_subject/migrations/0026_auto_20200420_1524.py
--rw-r--r--   0 estellaye   (501) staff       (20)     4756 2020-05-15 02:40:42.000000 meta-edc-demo-0.0.1/meta_subject/migrations/0027_auto_20200420_1645.py
--rw-r--r--   0 estellaye   (501) staff       (20)     6450 2021-07-05 19:24:26.000000 meta-edc-demo-0.0.1/meta_subject/migrations/0028_auto_20200420_1732.py
--rw-r--r--   0 estellaye   (501) staff       (20)     6004 2020-05-15 02:40:42.000000 meta-edc-demo-0.0.1/meta_subject/migrations/0029_auto_20200420_1751.py
--rw-r--r--   0 estellaye   (501) staff       (20)     5046 2020-05-15 02:40:42.000000 meta-edc-demo-0.0.1/meta_subject/migrations/0030_auto_20200420_1816.py
--rw-r--r--   0 estellaye   (501) staff       (20)     4610 2021-07-05 19:24:26.000000 meta-edc-demo-0.0.1/meta_subject/migrations/0031_auto_20200422_2039.py
--rw-r--r--   0 estellaye   (501) staff       (20)     7736 2021-07-05 19:24:26.000000 meta-edc-demo-0.0.1/meta_subject/migrations/0032_auto_20200515_0307.py
--rw-r--r--   0 estellaye   (501) staff       (20)    18673 2021-08-09 19:25:30.000000 meta-edc-demo-0.0.1/meta_subject/migrations/0033_auto_20200516_2356.py
--rw-r--r--   0 estellaye   (501) staff       (20)     1005 2020-05-20 04:57:20.000000 meta-edc-demo-0.0.1/meta_subject/migrations/0034_auto_20200517_0125.py
--rw-r--r--   0 estellaye   (501) staff       (20)     1317 2021-08-09 19:25:30.000000 meta-edc-demo-0.0.1/meta_subject/migrations/0035_auto_20200517_0128.py
--rw-r--r--   0 estellaye   (501) staff       (20)     2988 2021-07-05 19:24:26.000000 meta-edc-demo-0.0.1/meta_subject/migrations/0036_auto_20200517_0150.py
--rw-r--r--   0 estellaye   (501) staff       (20)      588 2020-05-20 04:57:20.000000 meta-edc-demo-0.0.1/meta_subject/migrations/0037_auto_20200517_0207.py
--rw-r--r--   0 estellaye   (501) staff       (20)    26377 2021-07-05 19:24:26.000000 meta-edc-demo-0.0.1/meta_subject/migrations/0038_auto_20200520_0020.py
--rw-r--r--   0 estellaye   (501) staff       (20)     6636 2020-06-18 19:11:34.000000 meta-edc-demo-0.0.1/meta_subject/migrations/0039_auto_20200524_1944.py
--rw-r--r--   0 estellaye   (501) staff       (20)    18300 2021-07-05 19:24:26.000000 meta-edc-demo-0.0.1/meta_subject/migrations/0040_auto_20200527_2155.py
--rw-r--r--   0 estellaye   (501) staff       (20)    12474 2021-07-05 19:24:26.000000 meta-edc-demo-0.0.1/meta_subject/migrations/0041_auto_20200528_0242.py
--rw-r--r--   0 estellaye   (501) staff       (20)      224 2020-06-18 19:11:34.000000 meta-edc-demo-0.0.1/meta_subject/migrations/0042_auto_20200528_0252.py
--rw-r--r--   0 estellaye   (501) staff       (20)     1510 2020-06-18 19:11:34.000000 meta-edc-demo-0.0.1/meta_subject/migrations/0043_auto_20200528_1555.py
--rw-r--r--   0 estellaye   (501) staff       (20)     2846 2020-06-18 19:11:34.000000 meta-edc-demo-0.0.1/meta_subject/migrations/0044_auto_20200528_1853.py
--rw-r--r--   0 estellaye   (501) staff       (20)     1245 2021-07-05 19:24:26.000000 meta-edc-demo-0.0.1/meta_subject/migrations/0045_auto_20200530_1801.py
--rw-r--r--   0 estellaye   (501) staff       (20)     3314 2021-07-05 19:24:26.000000 meta-edc-demo-0.0.1/meta_subject/migrations/0046_auto_20200530_1804.py
--rw-r--r--   0 estellaye   (501) staff       (20)      590 2022-09-30 02:18:01.000000 meta-edc-demo-0.0.1/meta_subject/migrations/0047_auto_20200530_1819.py
--rw-r--r--   0 estellaye   (501) staff       (20)      432 2020-06-18 19:11:34.000000 meta-edc-demo-0.0.1/meta_subject/migrations/0048_auto_20200530_1819.py
--rw-r--r--   0 estellaye   (501) staff       (20)      266 2021-07-05 19:24:26.000000 meta-edc-demo-0.0.1/meta_subject/migrations/0049_auto_20200613_2041.py
--rw-r--r--   0 estellaye   (501) staff       (20)      877 2021-08-09 19:25:30.000000 meta-edc-demo-0.0.1/meta_subject/migrations/0050_auto_20200614_1934.py
--rw-r--r--   0 estellaye   (501) staff       (20)    20317 2021-07-05 19:24:26.000000 meta-edc-demo-0.0.1/meta_subject/migrations/0051_auto_20200617_2117.py
--rw-r--r--   0 estellaye   (501) staff       (20)    40852 2021-07-05 19:24:26.000000 meta-edc-demo-0.0.1/meta_subject/migrations/0052_auto_20210624_0225.py
--rw-r--r--   0 estellaye   (501) staff       (20)    27485 2022-08-22 17:23:22.000000 meta-edc-demo-0.0.1/meta_subject/migrations/0053_auto_20210628_2105.py
--rw-r--r--   0 estellaye   (501) staff       (20)     3376 2021-07-05 19:24:26.000000 meta-edc-demo-0.0.1/meta_subject/migrations/0054_auto_20210628_2314.py
--rw-r--r--   0 estellaye   (501) staff       (20)     2932 2021-07-05 19:24:26.000000 meta-edc-demo-0.0.1/meta_subject/migrations/0055_auto_20210628_2331.py
--rw-r--r--   0 estellaye   (501) staff       (20)     3544 2021-07-02 03:53:00.000000 meta-edc-demo-0.0.1/meta_subject/migrations/0056_auto_20210702_0426.py
--rw-r--r--   0 estellaye   (501) staff       (20)     2828 2021-07-05 19:24:26.000000 meta-edc-demo-0.0.1/meta_subject/migrations/0057_auto_20210702_0458.py
--rw-r--r--   0 estellaye   (501) staff       (20)     1982 2021-07-05 19:24:26.000000 meta-edc-demo-0.0.1/meta_subject/migrations/0058_auto_20210702_0533.py
--rw-r--r--   0 estellaye   (501) staff       (20)    14818 2022-04-11 18:27:09.000000 meta-edc-demo-0.0.1/meta_subject/migrations/0059_auto_20210709_2056.py
--rw-r--r--   0 estellaye   (501) staff       (20)     1312 2022-04-11 18:27:09.000000 meta-edc-demo-0.0.1/meta_subject/migrations/0060_auto_20210709_2241.py
--rw-r--r--   0 estellaye   (501) staff       (20)    36062 2022-04-11 18:27:09.000000 meta-edc-demo-0.0.1/meta_subject/migrations/0061_auto_20210710_1929.py
--rw-r--r--   0 estellaye   (501) staff       (20)     1008 2022-04-11 18:27:09.000000 meta-edc-demo-0.0.1/meta_subject/migrations/0062_auto_20210713_0616.py
--rw-r--r--   0 estellaye   (501) staff       (20)    20741 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.1/meta_subject/migrations/0063_auto_20210715_0337.py
--rw-r--r--   0 estellaye   (501) staff       (20)    31934 2021-08-09 19:25:30.000000 meta-edc-demo-0.0.1/meta_subject/migrations/0064_auto_20210715_2336.py
--rw-r--r--   0 estellaye   (501) staff       (20)    10394 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.1/meta_subject/migrations/0065_auto_20210716_0813.py
--rw-r--r--   0 estellaye   (501) staff       (20)    27933 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.1/meta_subject/migrations/0066_auto_20210721_0335.py
--rw-r--r--   0 estellaye   (501) staff       (20)    47360 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.1/meta_subject/migrations/0067_auto_20210726_0340.py
--rw-r--r--   0 estellaye   (501) staff       (20)    41023 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.1/meta_subject/migrations/0068_auto_20210728_1809.py
--rw-r--r--   0 estellaye   (501) staff       (20)     2084 2022-04-11 18:27:09.000000 meta-edc-demo-0.0.1/meta_subject/migrations/0069_auto_20210801_2021.py
--rw-r--r--   0 estellaye   (501) staff       (20)     2866 2021-08-09 19:25:30.000000 meta-edc-demo-0.0.1/meta_subject/migrations/0070_auto_20210804_0438.py
--rw-r--r--   0 estellaye   (501) staff       (20)      996 2022-04-11 18:27:09.000000 meta-edc-demo-0.0.1/meta_subject/migrations/0071_auto_20210804_0715.py
--rw-r--r--   0 estellaye   (501) staff       (20)    25833 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.1/meta_subject/migrations/0072_auto_20210805_1545.py
--rw-r--r--   0 estellaye   (501) staff       (20)    41645 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.1/meta_subject/migrations/0073_auto_20210809_0055.py
--rw-r--r--   0 estellaye   (501) staff       (20)      290 2022-04-11 18:27:09.000000 meta-edc-demo-0.0.1/meta_subject/migrations/0074_auto_20210809_1744.py
--rw-r--r--   0 estellaye   (501) staff       (20)     1997 2021-08-09 19:33:52.000000 meta-edc-demo-0.0.1/meta_subject/migrations/0075_auto_20210809_1744.py
--rw-r--r--   0 estellaye   (501) staff       (20)      974 2022-04-11 18:27:09.000000 meta-edc-demo-0.0.1/meta_subject/migrations/0076_auto_20210809_1854.py
--rw-r--r--   0 estellaye   (501) staff       (20)     8021 2022-04-11 18:27:09.000000 meta-edc-demo-0.0.1/meta_subject/migrations/0077_auto_20210809_2323.py
--rw-r--r--   0 estellaye   (501) staff       (20)     1195 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.1/meta_subject/migrations/0078_auto_20210810_0857.py
--rw-r--r--   0 estellaye   (501) staff       (20)    35484 2022-04-11 18:27:09.000000 meta-edc-demo-0.0.1/meta_subject/migrations/0079_auto_20210812_0335.py
--rw-r--r--   0 estellaye   (501) staff       (20)    17308 2022-04-11 18:27:09.000000 meta-edc-demo-0.0.1/meta_subject/migrations/0080_auto_20210812_0400.py
--rw-r--r--   0 estellaye   (501) staff       (20)    27696 2022-04-11 18:27:09.000000 meta-edc-demo-0.0.1/meta_subject/migrations/0081_auto_20210817_2306.py
--rw-r--r--   0 estellaye   (501) staff       (20)    12294 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.1/meta_subject/migrations/0082_auto_20210823_1612.py
--rw-r--r--   0 estellaye   (501) staff       (20)    14439 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.1/meta_subject/migrations/0083_auto_20210823_1620.py
--rw-r--r--   0 estellaye   (501) staff       (20)    15219 2022-04-11 18:27:09.000000 meta-edc-demo-0.0.1/meta_subject/migrations/0084_auto_20210910_0234.py
--rw-r--r--   0 estellaye   (501) staff       (20)     2962 2022-04-11 18:27:09.000000 meta-edc-demo-0.0.1/meta_subject/migrations/0085_auto_20210911_2036.py
--rw-r--r--   0 estellaye   (501) staff       (20)    15645 2022-04-11 18:27:09.000000 meta-edc-demo-0.0.1/meta_subject/migrations/0086_auto_20210920_0229.py
--rw-r--r--   0 estellaye   (501) staff       (20)     2918 2022-04-11 18:27:09.000000 meta-edc-demo-0.0.1/meta_subject/migrations/0087_auto_20210922_2058.py
--rw-r--r--   0 estellaye   (501) staff       (20)    28869 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.1/meta_subject/migrations/0088_auto_20210924_0027.py
--rw-r--r--   0 estellaye   (501) staff       (20)     6594 2022-04-11 18:27:09.000000 meta-edc-demo-0.0.1/meta_subject/migrations/0089_auto_20210924_0121.py
--rw-r--r--   0 estellaye   (501) staff       (20)    15972 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.1/meta_subject/migrations/0090_auto_20210924_0424.py
--rw-r--r--   0 estellaye   (501) staff       (20)     1876 2022-06-24 08:50:42.000000 meta-edc-demo-0.0.1/meta_subject/migrations/0091_auto_20210929_2324.py
--rw-r--r--   0 estellaye   (501) staff       (20)    16400 2022-06-24 08:50:40.000000 meta-edc-demo-0.0.1/meta_subject/migrations/0092_auto_20211013_0447.py
--rw-r--r--   0 estellaye   (501) staff       (20)    33888 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.1/meta_subject/migrations/0093_auto_20211117_0352.py
--rw-r--r--   0 estellaye   (501) staff       (20)     4812 2022-06-24 08:50:38.000000 meta-edc-demo-0.0.1/meta_subject/migrations/0094_auto_20211123_1645.py
--rw-r--r--   0 estellaye   (501) staff       (20)    22479 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.1/meta_subject/migrations/0095_auto_20220128_1719.py
--rw-r--r--   0 estellaye   (501) staff       (20)     3419 2022-04-11 18:27:09.000000 meta-edc-demo-0.0.1/meta_subject/migrations/0096_auto_20220304_0501.py
--rw-r--r--   0 estellaye   (501) staff       (20)     2100 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.1/meta_subject/migrations/0097_auto_20220304_2233.py
--rw-r--r--   0 estellaye   (501) staff       (20)    21283 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.1/meta_subject/migrations/0098_auto_20220309_2106.py
--rw-r--r--   0 estellaye   (501) staff       (20)     1909 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.1/meta_subject/migrations/0099_auto_20220309_2218.py
--rw-r--r--   0 estellaye   (501) staff       (20)     1091 2022-06-24 08:50:29.000000 meta-edc-demo-0.0.1/meta_subject/migrations/0100_auto_20220309_2238.py
--rw-r--r--   0 estellaye   (501) staff       (20)    61584 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.1/meta_subject/migrations/0101_auto_20220316_2147.py
--rw-r--r--   0 estellaye   (501) staff       (20)    15291 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.1/meta_subject/migrations/0102_auto_20220324_0304.py
--rw-r--r--   0 estellaye   (501) staff       (20)      869 2022-06-24 08:50:27.000000 meta-edc-demo-0.0.1/meta_subject/migrations/0103_auto_20220324_0326.py
--rw-r--r--   0 estellaye   (501) staff       (20)      967 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.1/meta_subject/migrations/0104_auto_20220412_2151.py
--rw-r--r--   0 estellaye   (501) staff       (20)     1291 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.1/meta_subject/migrations/0105_auto_20220412_2310.py
--rw-r--r--   0 estellaye   (501) staff       (20)      773 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.1/meta_subject/migrations/0106_auto_20220414_1741.py
--rw-r--r--   0 estellaye   (501) staff       (20)     1493 2022-10-11 02:21:31.000000 meta-edc-demo-0.0.1/meta_subject/migrations/0107_auto_20220415_0043.py
--rw-r--r--   0 estellaye   (501) staff       (20)      689 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.1/meta_subject/migrations/0108_auto_20220415_1747.py
--rw-r--r--   0 estellaye   (501) staff       (20)      557 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.1/meta_subject/migrations/0109_auto_20220415_1758.py
--rw-r--r--   0 estellaye   (501) staff       (20)     2517 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.1/meta_subject/migrations/0110_auto_20220512_1811.py
--rw-r--r--   0 estellaye   (501) staff       (20)     3011 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.1/meta_subject/migrations/0111_alter_followupvitals_severe_htn_and_more.py
--rw-r--r--   0 estellaye   (501) staff       (20)     1036 2022-08-22 17:23:22.000000 meta-edc-demo-0.0.1/meta_subject/migrations/0112_historicalsubjectvisit_document_status_comments_and_more.py
--rw-r--r--   0 estellaye   (501) staff       (20)      720 2022-08-22 17:23:22.000000 meta-edc-demo-0.0.1/meta_subject/migrations/0113_bloodresultsrft_egfr_percent_change_and_more.py
--rw-r--r--   0 estellaye   (501) staff       (20)      992 2022-08-22 17:23:22.000000 meta-edc-demo-0.0.1/meta_subject/migrations/0114_alter_bloodresultsrft_egfr_percent_change_and_more.py
--rw-r--r--   0 estellaye   (501) staff       (20)    18447 2022-08-22 17:23:22.000000 meta-edc-demo-0.0.1/meta_subject/migrations/0115_historicalegfrnotification_egfrnotification.py
--rw-r--r--   0 estellaye   (501) staff       (20)     1177 2022-08-22 17:23:22.000000 meta-edc-demo-0.0.1/meta_subject/migrations/0116_egfrnotification_report_status_and_more.py
--rw-r--r--   0 estellaye   (501) staff       (20)     3279 2022-08-22 17:23:22.000000 meta-edc-demo-0.0.1/meta_subject/migrations/0117_alter_egfrnotification_managers_and_more.py
--rw-r--r--   0 estellaye   (501) staff       (20)     2050 2022-08-22 17:23:22.000000 meta-edc-demo-0.0.1/meta_subject/migrations/0118_delivery_crf_status_delivery_crf_status_comments_and_more.py
--rw-r--r--   0 estellaye   (501) staff       (20)      635 2022-08-22 17:23:22.000000 meta-edc-demo-0.0.1/meta_subject/migrations/0119_historicalstudymedication_roundup_divisible_by_and_more.py
--rw-r--r--   0 estellaye   (501) staff       (20)     2888 2022-08-22 17:23:22.000000 meta-edc-demo-0.0.1/meta_subject/migrations/0120_alter_birthoutcomes_managers_and_more.py
--rw-r--r--   0 estellaye   (501) staff       (20)    21741 2022-08-22 17:23:22.000000 meta-edc-demo-0.0.1/meta_subject/migrations/0121_auto_20220704_1841.py
--rw-r--r--   0 estellaye   (501) staff       (20)      813 2022-07-14 12:01:13.000000 meta-edc-demo-0.0.1/meta_subject/migrations/0122_auto_20220708_2144.py
--rw-r--r--   0 estellaye   (501) staff       (20)     8263 2022-08-22 17:23:22.000000 meta-edc-demo-0.0.1/meta_subject/migrations/0123_auto_20220714_2136.py
--rw-r--r--   0 estellaye   (501) staff       (20)     1207 2022-07-19 13:21:21.000000 meta-edc-demo-0.0.1/meta_subject/migrations/0124_auto_20220714_2303.py
--rw-r--r--   0 estellaye   (501) staff       (20)     1569 2022-08-22 17:23:22.000000 meta-edc-demo-0.0.1/meta_subject/migrations/0125_auto_20220719_2134.py
--rw-r--r--   0 estellaye   (501) staff       (20)      777 2022-08-22 17:23:22.000000 meta-edc-demo-0.0.1/meta_subject/migrations/0126_auto_20220719_2142.py
--rw-r--r--   0 estellaye   (501) staff       (20)     5489 2022-08-22 17:23:22.000000 meta-edc-demo-0.0.1/meta_subject/migrations/0127_auto_20220720_0053.py
--rw-r--r--   0 estellaye   (501) staff       (20)      779 2022-08-22 17:23:22.000000 meta-edc-demo-0.0.1/meta_subject/migrations/0128_auto_20220720_0055.py
--rw-r--r--   0 estellaye   (501) staff       (20)      491 2022-08-22 17:23:22.000000 meta-edc-demo-0.0.1/meta_subject/migrations/0129_auto_20220720_0108.py
--rw-r--r--   0 estellaye   (501) staff       (20)      684 2022-08-22 17:23:22.000000 meta-edc-demo-0.0.1/meta_subject/migrations/0130_auto_20220720_0216.py
--rw-r--r--   0 estellaye   (501) staff       (20)     1933 2022-08-22 17:23:22.000000 meta-edc-demo-0.0.1/meta_subject/migrations/0131_auto_20220722_0411.py
--rw-r--r--   0 estellaye   (501) staff       (20)      844 2022-08-22 17:23:22.000000 meta-edc-demo-0.0.1/meta_subject/migrations/0132_auto_20220722_1825.py
--rw-r--r--   0 estellaye   (501) staff       (20)    28131 2022-08-22 17:23:22.000000 meta-edc-demo-0.0.1/meta_subject/migrations/0133_auto_20220722_2140.py
--rw-r--r--   0 estellaye   (501) staff       (20)     1807 2022-08-22 17:23:22.000000 meta-edc-demo-0.0.1/meta_subject/migrations/0134_auto_20220722_2211.py
--rw-r--r--   0 estellaye   (501) staff       (20)     2264 2022-08-23 13:24:02.000000 meta-edc-demo-0.0.1/meta_subject/migrations/0135_auto_20220722_2212.py
--rw-r--r--   0 estellaye   (501) staff       (20)     8661 2022-08-22 17:23:22.000000 meta-edc-demo-0.0.1/meta_subject/migrations/0136_egfrdropnotification_creatinine_quantifier_and_more.py
--rw-r--r--   0 estellaye   (501) staff       (20)     1139 2022-08-22 17:23:22.000000 meta-edc-demo-0.0.1/meta_subject/migrations/0137_alter_egfrdropnotification_egfr_percent_change_and_more.py
--rw-r--r--   0 estellaye   (501) staff       (20)     3532 2022-08-22 17:23:22.000000 meta-edc-demo-0.0.1/meta_subject/migrations/0138_alter_glucose_fbg_datetime_and_more.py
--rw-r--r--   0 estellaye   (501) staff       (20)      939 2022-08-23 13:24:02.000000 meta-edc-demo-0.0.1/meta_subject/migrations/0139_alter_bloodresultsins_ins_units_and_more.py
--rw-r--r--   0 estellaye   (501) staff       (20)     4342 2022-08-23 13:31:01.000000 meta-edc-demo-0.0.1/meta_subject/migrations/0140_alter_bloodresultsfbc_action_identifier_and_more.py
--rw-r--r--   0 estellaye   (501) staff       (20)     4571 2022-08-26 02:59:33.000000 meta-edc-demo-0.0.1/meta_subject/migrations/0141_auto_20220826_0258.py
--rw-r--r--   0 estellaye   (501) staff       (20)     5197 2022-08-26 02:59:33.000000 meta-edc-demo-0.0.1/meta_subject/migrations/0142_auto_20220826_0322.py
--rw-r--r--   0 estellaye   (501) staff       (20)     3811 2022-08-26 02:59:33.000000 meta-edc-demo-0.0.1/meta_subject/migrations/0143_auto_20220826_0406.py
--rw-r--r--   0 estellaye   (501) staff       (20)      965 2022-09-08 15:51:35.000000 meta-edc-demo-0.0.1/meta_subject/migrations/0144_auto_20220907_0157.py
--rw-r--r--   0 estellaye   (501) staff       (20)     1786 2022-09-08 15:51:35.000000 meta-edc-demo-0.0.1/meta_subject/migrations/0145_auto_20220907_0202.py
--rw-r--r--   0 estellaye   (501) staff       (20)      619 2022-09-08 15:51:35.000000 meta-edc-demo-0.0.1/meta_subject/migrations/0146_auto_20220907_0207.py
--rw-r--r--   0 estellaye   (501) staff       (20)     1907 2022-09-08 21:41:58.000000 meta-edc-demo-0.0.1/meta_subject/migrations/0147_auto_20220907_1505.py
--rw-r--r--   0 estellaye   (501) staff       (20)     1815 2022-09-08 15:51:35.000000 meta-edc-demo-0.0.1/meta_subject/migrations/0148_auto_20220908_1826.py
--rw-r--r--   0 estellaye   (501) staff       (20)     1001 2022-09-15 02:57:38.000000 meta-edc-demo-0.0.1/meta_subject/migrations/0149_auto_20220913_2139.py
--rw-r--r--   0 estellaye   (501) staff       (20)     1224 2022-09-15 02:57:38.000000 meta-edc-demo-0.0.1/meta_subject/migrations/0150_auto_20220914_0039.py
--rw-r--r--   0 estellaye   (501) staff       (20)    52999 2022-09-26 19:37:19.000000 meta-edc-demo-0.0.1/meta_subject/migrations/0151_auto_20220918_0508.py
--rw-r--r--   0 estellaye   (501) staff       (20)      739 2022-09-26 19:37:19.000000 meta-edc-demo-0.0.1/meta_subject/migrations/0152_auto_20220925_0509.py
--rw-r--r--   0 estellaye   (501) staff       (20)     1173 2022-09-28 03:19:11.000000 meta-edc-demo-0.0.1/meta_subject/migrations/0153_auto_20220928_0250.py
--rw-r--r--   0 estellaye   (501) staff       (20)     1011 2022-09-28 03:19:11.000000 meta-edc-demo-0.0.1/meta_subject/migrations/0154_auto_20220928_0419.py
--rw-r--r--   0 estellaye   (501) staff       (20)     9272 2022-09-30 02:18:01.000000 meta-edc-demo-0.0.1/meta_subject/migrations/0155_auto_20220929_1742.py
--rw-r--r--   0 estellaye   (501) staff       (20)     5445 2022-10-05 21:55:17.000000 meta-edc-demo-0.0.1/meta_subject/migrations/0156_alter_bloodresultsfbc_assay_datetime_and_more.py
--rw-r--r--   0 estellaye   (501) staff       (20)        0 2020-03-15 03:34:20.000000 meta-edc-demo-0.0.1/meta_subject/migrations/__init__.py
-drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-06-27 05:23:34.801156 meta-edc-demo-0.0.1/meta_subject/model_mixins/
--rw-r--r--   0 estellaye   (501) staff       (20)      286 2022-09-26 19:37:19.000000 meta-edc-demo-0.0.1/meta_subject/model_mixins/__init__.py
--rw-r--r--   0 estellaye   (501) staff       (20)     2904 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.1/meta_subject/model_mixins/arv_history_model_mixin.py
--rw-r--r--   0 estellaye   (501) staff       (20)      248 2022-09-26 19:37:19.000000 meta-edc-demo-0.0.1/meta_subject/model_mixins/crf_model_mixin.py
--rw-r--r--   0 estellaye   (501) staff       (20)      298 2022-09-26 19:37:19.000000 meta-edc-demo-0.0.1/meta_subject/model_mixins/crf_with_action_model_mixin.py
--rw-r--r--   0 estellaye   (501) staff       (20)      296 2022-06-24 08:52:03.000000 meta-edc-demo-0.0.1/meta_subject/model_mixins/search_slug_model_mixin.py
--rw-r--r--   0 estellaye   (501) staff       (20)     1161 2022-06-24 08:49:55.000000 meta-edc-demo-0.0.1/meta_subject/model_mixins/vitals_fields_model_mixin.py
-drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-06-27 05:23:34.805797 meta-edc-demo-0.0.1/meta_subject/models/
--rw-r--r--   0 estellaye   (501) staff       (20)     1643 2022-08-23 01:10:14.000000 meta-edc-demo-0.0.1/meta_subject/models/__init__.py
--rw-r--r--   0 estellaye   (501) staff       (20)     2879 2022-09-30 02:18:01.000000 meta-edc-demo-0.0.1/meta_subject/models/birth_outcomes.py
-drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-06-27 05:23:34.807033 meta-edc-demo-0.0.1/meta_subject/models/blood_results/
--rw-r--r--   0 estellaye   (501) staff       (20)      337 2021-08-09 19:25:30.000000 meta-edc-demo-0.0.1/meta_subject/models/blood_results/__init__.py
--rw-r--r--   0 estellaye   (501) staff       (20)     1068 2022-09-26 19:37:19.000000 meta-edc-demo-0.0.1/meta_subject/models/blood_results/blood_results_fbc.py
--rw-r--r--   0 estellaye   (501) staff       (20)      818 2022-09-26 19:37:19.000000 meta-edc-demo-0.0.1/meta_subject/models/blood_results/blood_results_glu.py
--rw-r--r--   0 estellaye   (501) staff       (20)      776 2022-09-26 19:37:19.000000 meta-edc-demo-0.0.1/meta_subject/models/blood_results/blood_results_hba1c.py
--rw-r--r--   0 estellaye   (501) staff       (20)      790 2022-09-26 19:37:19.000000 meta-edc-demo-0.0.1/meta_subject/models/blood_results/blood_results_ins.py
--rw-r--r--   0 estellaye   (501) staff       (20)      977 2022-09-26 19:37:19.000000 meta-edc-demo-0.0.1/meta_subject/models/blood_results/blood_results_lft.py
--rw-r--r--   0 estellaye   (501) staff       (20)      907 2022-09-26 19:37:19.000000 meta-edc-demo-0.0.1/meta_subject/models/blood_results/blood_results_lipid.py
--rw-r--r--   0 estellaye   (501) staff       (20)     1417 2022-09-26 19:37:19.000000 meta-edc-demo-0.0.1/meta_subject/models/blood_results/blood_results_rft.py
--rw-r--r--   0 estellaye   (501) staff       (20)     1952 2022-08-22 17:23:22.000000 meta-edc-demo-0.0.1/meta_subject/models/complications.py
--rw-r--r--   0 estellaye   (501) staff       (20)     6079 2022-06-24 08:51:45.000000 meta-edc-demo-0.0.1/meta_subject/models/complications_glycemia.py
--rw-r--r--   0 estellaye   (501) staff       (20)      369 2022-09-26 19:37:19.000000 meta-edc-demo-0.0.1/meta_subject/models/concomitant_medication.py
--rw-r--r--   0 estellaye   (501) staff       (20)     5100 2022-09-29 13:40:10.000000 meta-edc-demo-0.0.1/meta_subject/models/delivery.py
--rw-r--r--   0 estellaye   (501) staff       (20)     1085 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.1/meta_subject/models/diet_and_lifestyle.py
--rw-r--r--   0 estellaye   (501) staff       (20)      558 2022-09-26 19:37:19.000000 meta-edc-demo-0.0.1/meta_subject/models/egfr_drop_notification.py
--rw-r--r--   0 estellaye   (501) staff       (20)      291 2022-09-26 19:37:19.000000 meta-edc-demo-0.0.1/meta_subject/models/eq5d3l.py
--rw-r--r--   0 estellaye   (501) staff       (20)     8075 2022-09-26 19:37:19.000000 meta-edc-demo-0.0.1/meta_subject/models/followup_examination.py
--rw-r--r--   0 estellaye   (501) staff       (20)      926 2022-06-24 08:51:51.000000 meta-edc-demo-0.0.1/meta_subject/models/followup_vitals.py
--rw-r--r--   0 estellaye   (501) staff       (20)     1314 2022-08-23 01:10:08.000000 meta-edc-demo-0.0.1/meta_subject/models/glucose.py
--rw-r--r--   0 estellaye   (501) staff       (20)     9736 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.1/meta_subject/models/health_economics.py
--rw-r--r--   0 estellaye   (501) staff       (20)      741 2022-09-26 19:37:19.000000 meta-edc-demo-0.0.1/meta_subject/models/health_economics_simple.py
--rw-r--r--   0 estellaye   (501) staff       (20)     1851 2022-08-22 17:23:22.000000 meta-edc-demo-0.0.1/meta_subject/models/hepatitis_test.py
--rw-r--r--   0 estellaye   (501) staff       (20)     1038 2022-09-26 19:37:19.000000 meta-edc-demo-0.0.1/meta_subject/models/malaria_test.py
--rw-r--r--   0 estellaye   (501) staff       (20)      399 2022-09-26 19:37:19.000000 meta-edc-demo-0.0.1/meta_subject/models/medication_adherence.py
--rw-r--r--   0 estellaye   (501) staff       (20)      284 2022-09-26 19:37:19.000000 meta-edc-demo-0.0.1/meta_subject/models/mnsi.py
--rw-r--r--   0 estellaye   (501) staff       (20)      707 2022-09-26 19:37:19.000000 meta-edc-demo-0.0.1/meta_subject/models/off_study_drug.py
--rw-r--r--   0 estellaye   (501) staff       (20)      607 2022-10-05 23:57:35.000000 meta-edc-demo-0.0.1/meta_subject/models/other_arv_regimens.py
--rw-r--r--   0 estellaye   (501) staff       (20)     1828 2022-09-26 19:37:19.000000 meta-edc-demo-0.0.1/meta_subject/models/other_arv_regimens_detail.py
--rw-r--r--   0 estellaye   (501) staff       (20)     4511 2022-09-26 19:37:19.000000 meta-edc-demo-0.0.1/meta_subject/models/patient_history.py
--rw-r--r--   0 estellaye   (501) staff       (20)     1994 2022-08-22 17:23:22.000000 meta-edc-demo-0.0.1/meta_subject/models/physical_exam.py
--rw-r--r--   0 estellaye   (501) staff       (20)      950 2022-09-26 19:37:19.000000 meta-edc-demo-0.0.1/meta_subject/models/pregnancy_update.py
--rw-r--r--   0 estellaye   (501) staff       (20)      345 2022-09-26 19:37:19.000000 meta-edc-demo-0.0.1/meta_subject/models/sf12.py
--rw-r--r--   0 estellaye   (501) staff       (20)     3989 2022-07-08 07:31:04.000000 meta-edc-demo-0.0.1/meta_subject/models/signals.py
--rw-r--r--   0 estellaye   (501) staff       (20)      462 2022-09-26 19:37:19.000000 meta-edc-demo-0.0.1/meta_subject/models/study_medication.py
--rw-r--r--   0 estellaye   (501) staff       (20)      422 2022-09-26 19:37:19.000000 meta-edc-demo-0.0.1/meta_subject/models/subject_requisition.py
--rw-r--r--   0 estellaye   (501) staff       (20)     2324 2022-10-13 03:34:11.000000 meta-edc-demo-0.0.1/meta_subject/models/subject_visit.py
--rw-r--r--   0 estellaye   (501) staff       (20)      748 2022-09-26 19:37:19.000000 meta-edc-demo-0.0.1/meta_subject/models/subject_visit_missed.py
--rw-r--r--   0 estellaye   (501) staff       (20)     1179 2022-06-24 08:49:07.000000 meta-edc-demo-0.0.1/meta_subject/models/urine_dipstick_test.py
--rw-r--r--   0 estellaye   (501) staff       (20)     1337 2022-09-26 19:37:19.000000 meta-edc-demo-0.0.1/meta_subject/models/urine_pregnancy.py
-drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-06-27 05:23:34.807284 meta-edc-demo-0.0.1/meta_subject/tests/
--rw-r--r--   0 estellaye   (501) staff       (20)        0 2020-03-15 03:34:20.000000 meta-edc-demo-0.0.1/meta_subject/tests/__init__.py
-drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-06-27 05:23:34.809117 meta-edc-demo-0.0.1/meta_subject/tests/tests/
--rw-r--r--   0 estellaye   (501) staff       (20)        0 2021-08-09 19:25:30.000000 meta-edc-demo-0.0.1/meta_subject/tests/tests/__init__.py
--rw-r--r--   0 estellaye   (501) staff       (20)     9294 2022-09-27 03:17:01.000000 meta-edc-demo-0.0.1/meta_subject/tests/tests/test_egfr.py
--rw-r--r--   0 estellaye   (501) staff       (20)     1760 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.1/meta_subject/tests/tests/test_followup.py
--rw-r--r--   0 estellaye   (501) staff       (20)     1376 2022-10-04 03:17:15.000000 meta-edc-demo-0.0.1/meta_subject/tests/tests/test_manager_order.py
--rw-r--r--   0 estellaye   (501) staff       (20)     2383 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.1/meta_subject/tests/tests/test_medication_adherence.py
--rw-r--r--   0 estellaye   (501) staff       (20)     4445 2022-08-22 17:23:22.000000 meta-edc-demo-0.0.1/meta_subject/tests/tests/test_metadata_rules.py
--rw-r--r--   0 estellaye   (501) staff       (20)     9809 2022-06-24 08:51:22.000000 meta-edc-demo-0.0.1/meta_subject/tests/tests/test_mnsi.py
--rw-r--r--   0 estellaye   (501) staff       (20)     2690 2022-09-26 19:37:19.000000 meta-edc-demo-0.0.1/meta_subject/tests/tests/test_patient_history_form.py
--rw-r--r--   0 estellaye   (501) staff       (20)     2810 2022-09-26 19:37:19.000000 meta-edc-demo-0.0.1/meta_subject/tests/tests/test_physical_exam.py
--rw-r--r--   0 estellaye   (501) staff       (20)     6926 2022-09-26 19:37:19.000000 meta-edc-demo-0.0.1/meta_subject/tests/tests/test_sf12.py
--rw-r--r--   0 estellaye   (501) staff       (20)    10161 2022-09-28 03:19:11.000000 meta-edc-demo-0.0.1/meta_subject/tests/tests/test_study_medication.py
--rw-r--r--   0 estellaye   (501) staff       (20)     1168 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.1/meta_subject/tests/urls.py
--rw-r--r--   0 estellaye   (501) staff       (20)      206 2022-06-24 09:02:28.000000 meta-edc-demo-0.0.1/meta_subject/urls.py
-drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-06-27 05:23:34.809722 meta-edc-demo-0.0.1/meta_visit_schedule/
--rw-r--r--   0 estellaye   (501) staff       (20)        0 2021-07-07 23:18:25.000000 meta-edc-demo-0.0.1/meta_visit_schedule/__init__.py
--rw-r--r--   0 estellaye   (501) staff       (20)      164 2021-07-02 03:53:00.000000 meta-edc-demo-0.0.1/meta_visit_schedule/apps.py
--rw-r--r--   0 estellaye   (501) staff       (20)      423 2022-04-11 18:27:09.000000 meta-edc-demo-0.0.1/meta_visit_schedule/constants.py
-drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-06-27 05:23:34.809836 meta-edc-demo-0.0.1/meta_visit_schedule/migrations/
--rw-r--r--   0 estellaye   (501) staff       (20)        0 2020-03-15 03:34:20.000000 meta-edc-demo-0.0.1/meta_visit_schedule/migrations/__init__.py
--rw-r--r--   0 estellaye   (501) staff       (20)        0 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.1/meta_visit_schedule/models.py
-drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-06-27 05:23:34.810050 meta-edc-demo-0.0.1/meta_visit_schedule/tests/
--rw-r--r--   0 estellaye   (501) staff       (20)        0 2020-03-15 03:34:20.000000 meta-edc-demo-0.0.1/meta_visit_schedule/tests/__init__.py
-drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-06-27 05:23:34.810321 meta-edc-demo-0.0.1/meta_visit_schedule/tests/tests/
--rw-r--r--   0 estellaye   (501) staff       (20)        0 2021-08-09 19:25:30.000000 meta-edc-demo-0.0.1/meta_visit_schedule/tests/tests/__init__.py
--rw-r--r--   0 estellaye   (501) staff       (20)     7206 2022-07-08 07:31:04.000000 meta-edc-demo-0.0.1/meta_visit_schedule/tests/tests/test_schedule.py
--rw-r--r--   0 estellaye   (501) staff       (20)      111 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.1/meta_visit_schedule/tests/urls.py
-drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-06-27 05:23:34.810476 meta-edc-demo-0.0.1/meta_visit_schedule/visit_schedules/
--rw-r--r--   0 estellaye   (501) staff       (20)      318 2022-04-11 18:27:09.000000 meta-edc-demo-0.0.1/meta_visit_schedule/visit_schedules/__init__.py
-drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-06-27 05:23:34.811639 meta-edc-demo-0.0.1/meta_visit_schedule/visit_schedules/phase_three/
--rw-r--r--   0 estellaye   (501) staff       (20)       74 2022-04-11 18:27:09.000000 meta-edc-demo-0.0.1/meta_visit_schedule/visit_schedules/phase_three/__init__.py
--rw-r--r--   0 estellaye   (501) staff       (20)    11160 2022-08-23 01:12:29.000000 meta-edc-demo-0.0.1/meta_visit_schedule/visit_schedules/phase_three/crfs.py
--rw-r--r--   0 estellaye   (501) staff       (20)      167 2022-06-24 08:46:02.000000 meta-edc-demo-0.0.1/meta_visit_schedule/visit_schedules/phase_three/crfs_pregnancy.py
--rw-r--r--   0 estellaye   (501) staff       (20)     5400 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.1/meta_visit_schedule/visit_schedules/phase_three/requisitions.py
--rw-r--r--   0 estellaye   (501) staff       (20)     6831 2022-09-26 19:37:19.000000 meta-edc-demo-0.0.1/meta_visit_schedule/visit_schedules/phase_three/schedule.py
--rw-r--r--   0 estellaye   (501) staff       (20)     1043 2022-08-22 17:23:22.000000 meta-edc-demo-0.0.1/meta_visit_schedule/visit_schedules/phase_three/schedule_pregnancy.py
--rw-r--r--   0 estellaye   (501) staff       (20)      522 2022-07-08 07:31:04.000000 meta-edc-demo-0.0.1/meta_visit_schedule/visit_schedules/phase_three/visit_schedule.py
--rw-r--r--   0 estellaye   (501) staff       (20)     1990 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.1/pyproject.toml
--rw-r--r--   0 estellaye   (501) staff       (20)     1218 2023-06-27 05:23:34.812401 meta-edc-demo-0.0.1/setup.cfg
--rw-r--r--   0 estellaye   (501) staff       (20)      642 2023-06-27 05:23:27.000000 meta-edc-demo-0.0.1/setup.py
-drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-06-27 05:23:34.811807 meta-edc-demo-0.0.1/tests/
--rw-r--r--   0 estellaye   (501) staff       (20)        0 2020-03-15 03:34:20.000000 meta-edc-demo-0.0.1/tests/__init__.py
+drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-06-27 06:22:40.373601 meta-edc-demo-0.0.2/
+-rw-r--r--   0 estellaye   (501) staff       (20)        0 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.2/AUTHORS
+-rw-r--r--   0 estellaye   (501) staff       (20)    11828 2022-10-13 03:34:11.000000 meta-edc-demo-0.0.2/CHANGES
+-rw-r--r--   0 estellaye   (501) staff       (20)    35149 2020-03-04 23:21:43.000000 meta-edc-demo-0.0.2/LICENSE
+-rw-r--r--   0 estellaye   (501) staff       (20)      162 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.2/MANIFEST.in
+-rw-r--r--   0 estellaye   (501) staff       (20)      585 2023-06-27 06:22:40.373692 meta-edc-demo-0.0.2/PKG-INFO
+-rw-r--r--   0 estellaye   (501) staff       (20)     1714 2022-10-12 03:43:37.000000 meta-edc-demo-0.0.2/README.rst
+-rw-r--r--   0 estellaye   (501) staff       (20)      893 2022-04-11 18:27:09.000000 meta-edc-demo-0.0.2/TODO.txt
+-rw-r--r--   0 estellaye   (501) staff       (20)        6 2022-10-14 13:07:30.000000 meta-edc-demo-0.0.2/VERSION
+drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-06-27 06:22:40.207108 meta-edc-demo-0.0.2/label_templates/
+drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-06-27 06:22:40.218483 meta-edc-demo-0.0.2/label_templates/2.25x1.25in/
+-rw-r--r--   0 estellaye   (501) staff       (20)      588 2020-03-04 23:21:43.000000 meta-edc-demo-0.0.2/label_templates/2.25x1.25in/aliquot.lbl
+-rw-r--r--   0 estellaye   (501) staff       (20)      341 2020-03-04 23:21:43.000000 meta-edc-demo-0.0.2/label_templates/2.25x1.25in/box.lbl
+-rw-r--r--   0 estellaye   (501) staff       (20)      337 2020-03-04 23:21:43.000000 meta-edc-demo-0.0.2/label_templates/2.25x1.25in/manifest.lbl
+-rw-r--r--   0 estellaye   (501) staff       (20)      520 2020-03-04 23:21:43.000000 meta-edc-demo-0.0.2/label_templates/2.25x1.25in/requisition.lbl
+-rw-r--r--   0 estellaye   (501) staff       (20)      299 2020-03-04 23:21:43.000000 meta-edc-demo-0.0.2/label_templates/2.25x1.25in/subject.lbl
+drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-06-27 06:22:40.219183 meta-edc-demo-0.0.2/label_templates/2x1cm/
+-rw-r--r--   0 estellaye   (501) staff       (20)      412 2020-03-04 23:21:43.000000 meta-edc-demo-0.0.2/label_templates/2x1cm/aliquot.lbl
+-rw-r--r--   0 estellaye   (501) staff       (20)      297 2020-03-04 23:21:43.000000 meta-edc-demo-0.0.2/label_templates/2x1cm/box.lbl
+-rw-r--r--   0 estellaye   (501) staff       (20)      294 2020-03-04 23:21:43.000000 meta-edc-demo-0.0.2/label_templates/2x1cm/manifest.lbl
+-rw-r--r--   0 estellaye   (501) staff       (20)      387 2020-03-04 23:21:43.000000 meta-edc-demo-0.0.2/label_templates/2x1cm/requisition.lbl
+drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-06-27 06:22:40.220707 meta-edc-demo-0.0.2/meta_ae/
+-rw-r--r--   0 estellaye   (501) staff       (20)        0 2020-03-15 03:34:20.000000 meta-edc-demo-0.0.2/meta_ae/__init__.py
+-rw-r--r--   0 estellaye   (501) staff       (20)    11256 2022-09-26 19:37:19.000000 meta-edc-demo-0.0.2/meta_ae/action_items.py
+drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-06-27 06:22:40.222671 meta-edc-demo-0.0.2/meta_ae/admin/
+-rw-r--r--   0 estellaye   (501) staff       (20)      460 2021-08-09 19:25:29.000000 meta-edc-demo-0.0.2/meta_ae/admin/__init__.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      416 2022-08-23 13:24:02.000000 meta-edc-demo-0.0.2/meta_ae/admin/ae_followup_admin.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      766 2022-08-23 13:24:02.000000 meta-edc-demo-0.0.2/meta_ae/admin/ae_initial_admin.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      410 2022-08-23 13:24:02.000000 meta-edc-demo-0.0.2/meta_ae/admin/ae_local_review_admin.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      420 2022-08-23 13:24:02.000000 meta-edc-demo-0.0.2/meta_ae/admin/ae_sponsor_review_admin.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      395 2022-08-23 13:24:02.000000 meta-edc-demo-0.0.2/meta_ae/admin/ae_susar_admin.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      381 2022-08-23 13:24:02.000000 meta-edc-demo-0.0.2/meta_ae/admin/ae_tmg_admin.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     2183 2022-08-23 13:24:02.000000 meta-edc-demo-0.0.2/meta_ae/admin/death_report_admin.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      444 2022-08-23 13:24:02.000000 meta-edc-demo-0.0.2/meta_ae/admin/death_report_tmg_admin.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      474 2022-08-23 13:24:02.000000 meta-edc-demo-0.0.2/meta_ae/admin/death_report_tmg_second_admin.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     4157 2022-08-23 13:24:02.000000 meta-edc-demo-0.0.2/meta_ae/admin/modeladmin_mixins.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      159 2021-07-02 03:53:00.000000 meta-edc-demo-0.0.2/meta_ae/admin_site.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      284 2022-08-23 13:24:02.000000 meta-edc-demo-0.0.2/meta_ae/apps.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     1134 2022-08-26 02:59:33.000000 meta-edc-demo-0.0.2/meta_ae/baker_recipes.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      756 2022-04-11 18:27:09.000000 meta-edc-demo-0.0.2/meta_ae/choices.py
+-rw-r--r--   0 estellaye   (501) staff       (20)       36 2022-04-11 18:27:09.000000 meta-edc-demo-0.0.2/meta_ae/constants.py
+drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-06-27 06:22:40.224851 meta-edc-demo-0.0.2/meta_ae/forms/
+-rw-r--r--   0 estellaye   (501) staff       (20)      438 2021-08-09 19:25:29.000000 meta-edc-demo-0.0.2/meta_ae/forms/__init__.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      298 2022-09-26 19:37:19.000000 meta-edc-demo-0.0.2/meta_ae/forms/ae_followup_form.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      292 2022-09-26 19:37:19.000000 meta-edc-demo-0.0.2/meta_ae/forms/ae_initial_form.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      284 2022-07-19 13:21:21.000000 meta-edc-demo-0.0.2/meta_ae/forms/ae_local_review_form.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      290 2022-07-19 13:21:21.000000 meta-edc-demo-0.0.2/meta_ae/forms/ae_sponsor_review_form.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      280 2022-09-26 19:37:19.000000 meta-edc-demo-0.0.2/meta_ae/forms/ae_susar_form.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      268 2022-09-26 19:37:19.000000 meta-edc-demo-0.0.2/meta_ae/forms/ae_tmg_form.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     1425 2022-09-26 19:37:19.000000 meta-edc-demo-0.0.2/meta_ae/forms/death_report_form.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      322 2022-09-26 19:37:19.000000 meta-edc-demo-0.0.2/meta_ae/forms/death_report_tmg_form.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      340 2022-09-26 19:37:19.000000 meta-edc-demo-0.0.2/meta_ae/forms/death_report_tmg_second_form.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      874 2022-09-26 19:37:19.000000 meta-edc-demo-0.0.2/meta_ae/forms/modelform_mixins.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     1372 2021-08-09 19:25:29.000000 meta-edc-demo-0.0.2/meta_ae/list_data.py
+drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-06-27 06:22:40.227864 meta-edc-demo-0.0.2/meta_ae/migrations/
+-rw-r--r--   0 estellaye   (501) staff       (20)   140318 2022-09-30 02:18:01.000000 meta-edc-demo-0.0.2/meta_ae/migrations/0001_initial.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     2700 2021-07-05 19:24:26.000000 meta-edc-demo-0.0.2/meta_ae/migrations/0002_auto_20191024_1000.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     2445 2021-07-05 19:24:26.000000 meta-edc-demo-0.0.2/meta_ae/migrations/0003_auto_20191102_0033.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      998 2021-07-05 19:24:26.000000 meta-edc-demo-0.0.2/meta_ae/migrations/0004_auto_20191114_0821.py
+-rw-r--r--   0 estellaye   (501) staff       (20)    18485 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.2/meta_ae/migrations/0005_auto_20210624_0225.py
+-rw-r--r--   0 estellaye   (501) staff       (20)    16967 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.2/meta_ae/migrations/0006_aelocalreview_aesponsorreview.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     2709 2022-06-24 08:52:48.000000 meta-edc-demo-0.0.2/meta_ae/migrations/0007_auto_20210911_2036.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     1241 2022-06-24 08:52:45.000000 meta-edc-demo-0.0.2/meta_ae/migrations/0008_auto_20211011_1657.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     1152 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.2/meta_ae/migrations/0009_auto_20220307_1929.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     4215 2022-08-22 17:23:22.000000 meta-edc-demo-0.0.2/meta_ae/migrations/0010_auto_20220704_1841.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     2828 2022-08-23 13:31:01.000000 meta-edc-demo-0.0.2/meta_ae/migrations/0011_alter_aefollowup_action_identifier_and_more.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     2997 2022-08-26 02:59:33.000000 meta-edc-demo-0.0.2/meta_ae/migrations/0012_auto_20220826_0258.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     2842 2022-08-26 02:59:33.000000 meta-edc-demo-0.0.2/meta_ae/migrations/0013_auto_20220826_0322.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     1858 2022-08-26 02:59:33.000000 meta-edc-demo-0.0.2/meta_ae/migrations/0014_auto_20220826_0406.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     1239 2022-09-08 15:51:35.000000 meta-edc-demo-0.0.2/meta_ae/migrations/0015_auto_20220907_0157.py
+-rw-r--r--   0 estellaye   (501) staff       (20)        0 2020-03-15 03:34:20.000000 meta-edc-demo-0.0.2/meta_ae/migrations/__init__.py
+drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-06-27 06:22:40.228260 meta-edc-demo-0.0.2/meta_ae/model_mixins/
+-rw-r--r--   0 estellaye   (501) staff       (20)      114 2020-05-15 02:40:42.000000 meta-edc-demo-0.0.2/meta_ae/model_mixins/__init__.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     2638 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.2/meta_ae/model_mixins/ae_review_model_mixin.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     1799 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.2/meta_ae/model_mixins/death_report_model_mixin.py
+drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-06-27 06:22:40.229894 meta-edc-demo-0.0.2/meta_ae/models/
+-rw-r--r--   0 estellaye   (501) staff       (20)      357 2021-08-09 19:25:29.000000 meta-edc-demo-0.0.2/meta_ae/models/__init__.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      236 2020-03-15 03:34:20.000000 meta-edc-demo-0.0.2/meta_ae/models/ae_followup.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      343 2020-03-15 03:34:20.000000 meta-edc-demo-0.0.2/meta_ae/models/ae_initial.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      236 2021-08-09 19:25:29.000000 meta-edc-demo-0.0.2/meta_ae/models/ae_local_review.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      240 2021-08-09 19:25:29.000000 meta-edc-demo-0.0.2/meta_ae/models/ae_sponsor_review.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      208 2020-03-15 03:34:20.000000 meta-edc-demo-0.0.2/meta_ae/models/ae_susar.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      226 2020-03-15 03:34:20.000000 meta-edc-demo-0.0.2/meta_ae/models/ae_tmg.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      446 2020-05-15 02:40:42.000000 meta-edc-demo-0.0.2/meta_ae/models/death_report.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      236 2021-07-05 19:24:26.000000 meta-edc-demo-0.0.2/meta_ae/models/death_report_tmg.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      565 2020-03-15 03:34:20.000000 meta-edc-demo-0.0.2/meta_ae/models/death_report_tmg_second.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      621 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.2/meta_ae/models/managers.py
+drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-06-27 06:22:40.230483 meta-edc-demo-0.0.2/meta_ae/pdf_reports/
+-rw-r--r--   0 estellaye   (501) staff       (20)       70 2020-03-15 03:34:20.000000 meta-edc-demo-0.0.2/meta_ae/pdf_reports/__init__.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      184 2020-03-15 03:34:20.000000 meta-edc-demo-0.0.2/meta_ae/pdf_reports/ae_report.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      196 2020-03-15 03:34:20.000000 meta-edc-demo-0.0.2/meta_ae/pdf_reports/death_report.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      535 2020-03-15 03:34:20.000000 meta-edc-demo-0.0.2/meta_ae/pdf_reports/meta_pdf_report_mixin.py
+drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-06-27 06:22:40.230724 meta-edc-demo-0.0.2/meta_ae/templatetags/
+-rw-r--r--   0 estellaye   (501) staff       (20)        0 2020-03-15 03:34:20.000000 meta-edc-demo-0.0.2/meta_ae/templatetags/__init__.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     1154 2022-08-22 17:23:22.000000 meta-edc-demo-0.0.2/meta_ae/templatetags/meta_ae_extras.py
+drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-06-27 06:22:40.230964 meta-edc-demo-0.0.2/meta_ae/tests/
+-rw-r--r--   0 estellaye   (501) staff       (20)        0 2020-03-15 03:34:20.000000 meta-edc-demo-0.0.2/meta_ae/tests/__init__.py
+drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-06-27 06:22:40.231210 meta-edc-demo-0.0.2/meta_ae/tests/tests/
+-rw-r--r--   0 estellaye   (501) staff       (20)        0 2021-08-09 19:25:29.000000 meta-edc-demo-0.0.2/meta_ae/tests/tests/__init__.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     4915 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.2/meta_ae/tests/tests/test_actions.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      260 2021-07-05 19:24:26.000000 meta-edc-demo-0.0.2/meta_ae/tests/urls.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      197 2021-08-09 19:25:29.000000 meta-edc-demo-0.0.2/meta_ae/urls.py
+drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-06-27 06:22:40.232188 meta-edc-demo-0.0.2/meta_auth/
+-rw-r--r--   0 estellaye   (501) staff       (20)        0 2020-03-15 03:34:20.000000 meta-edc-demo-0.0.2/meta_auth/__init__.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      298 2022-06-24 09:16:28.000000 meta-edc-demo-0.0.2/meta_auth/apps.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     1738 2022-08-26 02:59:33.000000 meta-edc-demo-0.0.2/meta_auth/auth_objects.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     2435 2022-09-08 21:41:58.000000 meta-edc-demo-0.0.2/meta_auth/auths.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      111 2022-06-24 09:16:34.000000 meta-edc-demo-0.0.2/meta_auth/urls.py
+drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-06-27 06:22:40.233491 meta-edc-demo-0.0.2/meta_consent/
+-rw-r--r--   0 estellaye   (501) staff       (20)        0 2020-03-15 03:34:20.000000 meta-edc-demo-0.0.2/meta_consent/__init__.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      756 2022-06-24 09:14:24.000000 meta-edc-demo-0.0.2/meta_consent/action_items.py
+drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-06-27 06:22:40.234212 meta-edc-demo-0.0.2/meta_consent/admin/
+-rw-r--r--   0 estellaye   (501) staff       (20)      114 2020-03-15 03:34:20.000000 meta-edc-demo-0.0.2/meta_consent/admin/__init__.py
+drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-06-27 06:22:40.234671 meta-edc-demo-0.0.2/meta_consent/admin/actions/
+-rw-r--r--   0 estellaye   (501) staff       (20)       70 2022-07-08 07:31:04.000000 meta-edc-demo-0.0.2/meta_consent/admin/actions/__init__.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     1474 2022-07-08 07:31:04.000000 meta-edc-demo-0.0.2/meta_consent/admin/actions/create_missing_prescriptions.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     5444 2022-08-23 13:24:02.000000 meta-edc-demo-0.0.2/meta_consent/admin/subject_consent_admin.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     2971 2022-08-23 13:24:02.000000 meta-edc-demo-0.0.2/meta_consent/admin/subject_reconsent_admin.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      169 2022-06-24 09:14:27.000000 meta-edc-demo-0.0.2/meta_consent/admin_site.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      282 2022-08-23 13:24:02.000000 meta-edc-demo-0.0.2/meta_consent/apps.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     1258 2022-08-26 02:59:33.000000 meta-edc-demo-0.0.2/meta_consent/baker_recipes.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      436 2022-06-24 09:14:37.000000 meta-edc-demo-0.0.2/meta_consent/consents.py
+-rw-r--r--   0 estellaye   (501) staff       (20)       31 2022-06-24 09:14:43.000000 meta-edc-demo-0.0.2/meta_consent/constants.py
+drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-06-27 06:22:40.235318 meta-edc-demo-0.0.2/meta_consent/forms/
+-rw-r--r--   0 estellaye   (501) staff       (20)      139 2022-04-11 18:27:09.000000 meta-edc-demo-0.0.2/meta_consent/forms/__init__.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     2425 2022-10-04 03:17:15.000000 meta-edc-demo-0.0.2/meta_consent/forms/subject_consent_form.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     1306 2022-10-04 03:17:15.000000 meta-edc-demo-0.0.2/meta_consent/forms/subject_reconsent_form.py
+drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-06-27 06:22:40.235533 meta-edc-demo-0.0.2/meta_consent/management/
+-rw-r--r--   0 estellaye   (501) staff       (20)        0 2022-04-11 18:27:09.000000 meta-edc-demo-0.0.2/meta_consent/management/__init__.py
+drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-06-27 06:22:40.235812 meta-edc-demo-0.0.2/meta_consent/management/commands/
+-rw-r--r--   0 estellaye   (501) staff       (20)        0 2022-04-11 18:27:09.000000 meta-edc-demo-0.0.2/meta_consent/management/commands/__init__.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     1438 2022-07-08 07:31:04.000000 meta-edc-demo-0.0.2/meta_consent/management/commands/create_missing_prescriptions.py
+drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-06-27 06:22:40.239194 meta-edc-demo-0.0.2/meta_consent/migrations/
+-rw-r--r--   0 estellaye   (501) staff       (20)    66733 2022-09-30 02:18:01.000000 meta-edc-demo-0.0.2/meta_consent/migrations/0001_initial.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      591 2021-07-05 19:24:26.000000 meta-edc-demo-0.0.2/meta_consent/migrations/0002_auto_20191024_1000.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     1611 2020-04-03 04:33:09.000000 meta-edc-demo-0.0.2/meta_consent/migrations/0003_auto_20200325_0901.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     3510 2021-07-05 19:24:26.000000 meta-edc-demo-0.0.2/meta_consent/migrations/0004_auto_20210624_0225.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      791 2022-04-11 18:27:09.000000 meta-edc-demo-0.0.2/meta_consent/migrations/0005_alter_subjectconsent_options.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      638 2022-06-24 09:13:48.000000 meta-edc-demo-0.0.2/meta_consent/migrations/0006_auto_20210911_2036.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     3052 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.2/meta_consent/migrations/0007_auto_20220128_1719.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      943 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.2/meta_consent/migrations/0008_auto_20220412_2151.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     1391 2022-08-22 17:23:22.000000 meta-edc-demo-0.0.2/meta_consent/migrations/0009_auto_20220704_1841.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      648 2022-08-23 13:31:01.000000 meta-edc-demo-0.0.2/meta_consent/migrations/0010_alter_historicalsubjectreconsent_action_identifier_and_more.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      712 2022-08-26 02:59:33.000000 meta-edc-demo-0.0.2/meta_consent/migrations/0011_auto_20220826_0258.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      651 2022-08-26 02:59:33.000000 meta-edc-demo-0.0.2/meta_consent/migrations/0012_auto_20220826_0322.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      493 2022-08-26 02:59:33.000000 meta-edc-demo-0.0.2/meta_consent/migrations/0013_auto_20220826_0406.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      605 2022-09-30 02:18:01.000000 meta-edc-demo-0.0.2/meta_consent/migrations/0014_alter_subjectconsent_managers.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      756 2022-09-15 02:57:38.000000 meta-edc-demo-0.0.2/meta_consent/migrations/0015_auto_20220914_0542.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      948 2022-09-15 02:57:38.000000 meta-edc-demo-0.0.2/meta_consent/migrations/0016_auto_20220914_0547.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      923 2022-09-30 02:18:01.000000 meta-edc-demo-0.0.2/meta_consent/migrations/0017_auto_20220929_1742.py
+-rw-r--r--   0 estellaye   (501) staff       (20)        0 2020-03-15 03:34:20.000000 meta-edc-demo-0.0.2/meta_consent/migrations/__init__.py
+drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-06-27 06:22:40.240430 meta-edc-demo-0.0.2/meta_consent/models/
+-rw-r--r--   0 estellaye   (501) staff       (20)      174 2021-08-09 19:25:29.000000 meta-edc-demo-0.0.2/meta_consent/models/__init__.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      296 2022-06-24 09:13:53.000000 meta-edc-demo-0.0.2/meta_consent/models/model_mixins.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     4303 2022-07-01 06:36:06.000000 meta-edc-demo-0.0.2/meta_consent/models/signals.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     4054 2022-09-30 02:18:01.000000 meta-edc-demo-0.0.2/meta_consent/models/subject_consent.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     3588 2022-09-30 02:18:01.000000 meta-edc-demo-0.0.2/meta_consent/models/subject_reconsent.py
+drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-06-27 06:22:40.240735 meta-edc-demo-0.0.2/meta_consent/tests/
+-rw-r--r--   0 estellaye   (501) staff       (20)        0 2020-03-15 03:34:20.000000 meta-edc-demo-0.0.2/meta_consent/tests/__init__.py
+drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-06-27 06:22:40.241246 meta-edc-demo-0.0.2/meta_consent/tests/tests/
+-rw-r--r--   0 estellaye   (501) staff       (20)        0 2021-08-09 19:25:29.000000 meta-edc-demo-0.0.2/meta_consent/tests/tests/__init__.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     3546 2022-08-22 17:23:22.000000 meta-edc-demo-0.0.2/meta_consent/tests/tests/test_form_validators.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      376 2022-06-24 09:14:16.000000 meta-edc-demo-0.0.2/meta_consent/tests/tests/test_subject_consent.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      916 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.2/meta_consent/tests/urls.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      206 2022-06-24 09:14:40.000000 meta-edc-demo-0.0.2/meta_consent/urls.py
+drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-06-27 06:22:40.242217 meta-edc-demo-0.0.2/meta_dashboard/
+-rw-r--r--   0 estellaye   (501) staff       (20)        0 2020-03-15 03:34:20.000000 meta-edc-demo-0.0.2/meta_dashboard/__init__.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     1993 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.2/meta_dashboard/apps.py
+drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-06-27 06:22:40.242416 meta-edc-demo-0.0.2/meta_dashboard/migrations/
+-rw-r--r--   0 estellaye   (501) staff       (20)        0 2020-03-15 03:34:20.000000 meta-edc-demo-0.0.2/meta_dashboard/migrations/__init__.py
+drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-06-27 06:22:40.243389 meta-edc-demo-0.0.2/meta_dashboard/model_wrappers/
+-rw-r--r--   0 estellaye   (501) staff       (20)      343 2021-07-05 19:24:26.000000 meta-edc-demo-0.0.2/meta_dashboard/model_wrappers/__init__.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      161 2020-03-15 03:34:20.000000 meta-edc-demo-0.0.2/meta_dashboard/model_wrappers/ae_initial_model_wrapper.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      375 2020-03-15 03:34:20.000000 meta-edc-demo-0.0.2/meta_dashboard/model_wrappers/death_report_model_wrapper.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      407 2020-03-15 03:34:20.000000 meta-edc-demo-0.0.2/meta_dashboard/model_wrappers/subject_refusal_model_wrapper.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     2718 2022-04-11 18:27:09.000000 meta-edc-demo-0.0.2/meta_dashboard/model_wrappers/subject_screening_model_wrapper.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     1204 2022-08-26 02:59:33.000000 meta-edc-demo-0.0.2/meta_dashboard/navbars.py
+-rw-r--r--   0 estellaye   (501) staff       (20)       47 2022-06-24 09:14:59.000000 meta-edc-demo-0.0.2/meta_dashboard/patterns.py
+drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-06-27 06:22:40.243665 meta-edc-demo-0.0.2/meta_dashboard/templatetags/
+-rw-r--r--   0 estellaye   (501) staff       (20)        0 2020-03-15 03:34:20.000000 meta-edc-demo-0.0.2/meta_dashboard/templatetags/__init__.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     3845 2022-08-22 17:23:22.000000 meta-edc-demo-0.0.2/meta_dashboard/templatetags/meta_dashboard_extras.py
+drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-06-27 06:22:40.244171 meta-edc-demo-0.0.2/meta_dashboard/tests/
+-rw-r--r--   0 estellaye   (501) staff       (20)        0 2020-03-15 03:34:20.000000 meta-edc-demo-0.0.2/meta_dashboard/tests/__init__.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      716 2021-07-05 19:24:26.000000 meta-edc-demo-0.0.2/meta_dashboard/tests/admin.py
+drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-06-27 06:22:40.244521 meta-edc-demo-0.0.2/meta_dashboard/tests/tests/
+-rw-r--r--   0 estellaye   (501) staff       (20)        0 2020-03-15 03:34:20.000000 meta-edc-demo-0.0.2/meta_dashboard/tests/tests/__init__.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     2494 2021-07-05 19:24:26.000000 meta-edc-demo-0.0.2/meta_dashboard/tests/tests/test_model_wrappers.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     2913 2021-07-05 19:24:26.000000 meta-edc-demo-0.0.2/meta_dashboard/tests/urls.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     1098 2022-06-24 09:15:02.000000 meta-edc-demo-0.0.2/meta_dashboard/urls.py
+drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-06-27 06:22:40.244788 meta-edc-demo-0.0.2/meta_dashboard/views/
+-rw-r--r--   0 estellaye   (501) staff       (20)      222 2022-08-26 02:59:33.000000 meta-edc-demo-0.0.2/meta_dashboard/views/__init__.py
+drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-06-27 06:22:40.245360 meta-edc-demo-0.0.2/meta_dashboard/views/ae/
+-rw-r--r--   0 estellaye   (501) staff       (20)      113 2020-03-15 03:34:20.000000 meta-edc-demo-0.0.2/meta_dashboard/views/ae/__init__.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      454 2021-07-05 19:24:26.000000 meta-edc-demo-0.0.2/meta_dashboard/views/ae/ae_listboard_view.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      492 2020-03-15 03:34:20.000000 meta-edc-demo-0.0.2/meta_dashboard/views/ae/death_report_listboard_view.py
+drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-06-27 06:22:40.245768 meta-edc-demo-0.0.2/meta_dashboard/views/screening/
+-rw-r--r--   0 estellaye   (501) staff       (20)       42 2020-03-15 03:34:20.000000 meta-edc-demo-0.0.2/meta_dashboard/views/screening/__init__.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      888 2022-08-26 02:59:33.000000 meta-edc-demo-0.0.2/meta_dashboard/views/screening/listboard_view.py
+drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-06-27 06:22:40.245947 meta-edc-demo-0.0.2/meta_dashboard/views/subject/
+-rw-r--r--   0 estellaye   (501) staff       (20)       81 2022-08-26 02:59:33.000000 meta-edc-demo-0.0.2/meta_dashboard/views/subject/__init__.py
+drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-06-27 06:22:40.246388 meta-edc-demo-0.0.2/meta_dashboard/views/subject/dashboard/
+-rw-r--r--   0 estellaye   (501) staff       (20)       42 2020-03-15 03:34:20.000000 meta-edc-demo-0.0.2/meta_dashboard/views/subject/dashboard/__init__.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      285 2022-09-08 15:51:35.000000 meta-edc-demo-0.0.2/meta_dashboard/views/subject/dashboard/dashboard_view.py
+drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-06-27 06:22:40.246757 meta-edc-demo-0.0.2/meta_dashboard/views/subject/listboard/
+-rw-r--r--   0 estellaye   (501) staff       (20)       49 2022-08-26 02:59:33.000000 meta-edc-demo-0.0.2/meta_dashboard/views/subject/listboard/__init__.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      695 2022-08-26 13:10:52.000000 meta-edc-demo-0.0.2/meta_dashboard/views/subject/listboard/listboard_view.py
+drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-06-27 06:22:40.247337 meta-edc-demo-0.0.2/meta_data_manager/
+-rw-r--r--   0 estellaye   (501) staff       (20)        0 2022-04-11 18:27:09.000000 meta-edc-demo-0.0.2/meta_data_manager/__init__.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      233 2022-04-11 18:27:09.000000 meta-edc-demo-0.0.2/meta_data_manager/apps.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      167 2022-04-11 18:27:09.000000 meta-edc-demo-0.0.2/meta_data_manager/data_manager.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      953 2022-06-24 09:13:03.000000 meta-edc-demo-0.0.2/meta_data_manager/handlers.py
+drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-06-27 06:22:40.249377 meta-edc-demo-0.0.2/meta_edc/
+-rw-r--r--   0 estellaye   (501) staff       (20)        0 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.2/meta_edc/__init__.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      845 2022-08-22 17:23:22.000000 meta-edc-demo-0.0.2/meta_edc/admin.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      450 2022-06-24 09:07:19.000000 meta-edc-demo-0.0.2/meta_edc/apps.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      175 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.2/meta_edc/asgi.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      785 2020-03-04 23:21:43.000000 meta-edc-demo-0.0.2/meta_edc/celery.py
+drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-06-27 06:22:40.249526 meta-edc-demo-0.0.2/meta_edc/management/
+-rw-r--r--   0 estellaye   (501) staff       (20)        0 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.2/meta_edc/management/__init__.py
+drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-06-27 06:22:40.249735 meta-edc-demo-0.0.2/meta_edc/management/commands/
+-rw-r--r--   0 estellaye   (501) staff       (20)        0 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.2/meta_edc/management/commands/__init__.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     1006 2022-10-12 03:43:37.000000 meta-edc-demo-0.0.2/meta_edc/management/commands/update_forms_reference.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      211 2022-06-24 09:07:24.000000 meta-edc-demo-0.0.2/meta_edc/meta_version.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     1339 2022-07-19 13:21:21.000000 meta-edc-demo-0.0.2/meta_edc/model_callers.py
+-rw-r--r--   0 estellaye   (501) staff       (20)       46 2020-03-04 23:21:43.000000 meta-edc-demo-0.0.2/meta_edc/models.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     1065 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.2/meta_edc/navbars.py
+drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-06-27 06:22:40.250751 meta-edc-demo-0.0.2/meta_edc/settings/
+-rw-r--r--   0 estellaye   (501) staff       (20)        0 2020-04-03 04:33:09.000000 meta-edc-demo-0.0.2/meta_edc/settings/__init__.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      675 2022-10-14 13:07:31.000000 meta-edc-demo-0.0.2/meta_edc/settings/debug.py
+-rw-r--r--   0 estellaye   (501) staff       (20)    19094 2022-10-10 22:11:43.000000 meta-edc-demo-0.0.2/meta_edc/settings/defaults.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      483 2022-08-26 02:59:33.000000 meta-edc-demo-0.0.2/meta_edc/settings/live.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     1855 2022-10-10 22:12:06.000000 meta-edc-demo-0.0.2/meta_edc/settings/logging.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      591 2022-08-22 17:23:22.000000 meta-edc-demo-0.0.2/meta_edc/settings/minimal.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      580 2022-08-26 02:59:33.000000 meta-edc-demo-0.0.2/meta_edc/settings/uat.py
+drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-06-27 06:22:40.210916 meta-edc-demo-0.0.2/meta_edc/templates/
+drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-06-27 06:22:40.210975 meta-edc-demo-0.0.2/meta_edc/templates/meta_edc/
+drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-06-27 06:22:40.251051 meta-edc-demo-0.0.2/meta_edc/templates/meta_edc/bootstrap3/
+-rw-r--r--   0 estellaye   (501) staff       (20)      165 2021-08-09 19:25:29.000000 meta-edc-demo-0.0.2/meta_edc/templates/meta_edc/bootstrap3/base.html
+-rw-r--r--   0 estellaye   (501) staff       (20)     3780 2022-08-26 02:59:33.000000 meta-edc-demo-0.0.2/meta_edc/templates/meta_edc/bootstrap3/home.html
+drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-06-27 06:22:40.251209 meta-edc-demo-0.0.2/meta_edc/tests/
+-rw-r--r--   0 estellaye   (501) staff       (20)        0 2020-03-04 23:21:43.000000 meta-edc-demo-0.0.2/meta_edc/tests/__init__.py
+drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-06-27 06:22:40.251433 meta-edc-demo-0.0.2/meta_edc/tests/tests/
+-rw-r--r--   0 estellaye   (501) staff       (20)        0 2021-08-09 19:25:29.000000 meta-edc-demo-0.0.2/meta_edc/tests/tests/__init__.py
+-rw-r--r--   0 estellaye   (501) staff       (20)    22422 2022-09-15 02:57:38.000000 meta-edc-demo-0.0.2/meta_edc/tests/tests/test_endpoints.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     3330 2022-10-07 03:13:37.000000 meta-edc-demo-0.0.2/meta_edc/urls.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      342 2022-06-24 09:07:39.000000 meta-edc-demo-0.0.2/meta_edc/utils.py
+drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-06-27 06:22:40.251773 meta-edc-demo-0.0.2/meta_edc/views/
+-rw-r--r--   0 estellaye   (501) staff       (20)       32 2020-03-04 23:21:43.000000 meta-edc-demo-0.0.2/meta_edc/views/__init__.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      992 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.2/meta_edc/views/home_view.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      175 2020-04-03 04:33:09.000000 meta-edc-demo-0.0.2/meta_edc/wsgi.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      174 2020-04-03 04:33:09.000000 meta-edc-demo-0.0.2/meta_edc/wsgi_live.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      173 2020-04-03 04:33:09.000000 meta-edc-demo-0.0.2/meta_edc/wsgi_uat.py
+drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-06-27 06:22:40.252513 meta-edc-demo-0.0.2/meta_edc_demo.egg-info/
+-rw-r--r--   0 estellaye   (501) staff       (20)      585 2023-06-27 06:22:40.000000 meta-edc-demo-0.0.2/meta_edc_demo.egg-info/PKG-INFO
+-rw-r--r--   0 estellaye   (501) staff       (20)    36359 2023-06-27 06:22:40.000000 meta-edc-demo-0.0.2/meta_edc_demo.egg-info/SOURCES.txt
+-rw-r--r--   0 estellaye   (501) staff       (20)        1 2023-06-27 06:22:40.000000 meta-edc-demo-0.0.2/meta_edc_demo.egg-info/dependency_links.txt
+-rw-r--r--   0 estellaye   (501) staff       (20)        1 2023-06-27 06:22:40.000000 meta-edc-demo-0.0.2/meta_edc_demo.egg-info/not-zip-safe
+-rw-r--r--   0 estellaye   (501) staff       (20)       56 2023-06-27 06:22:40.000000 meta-edc-demo-0.0.2/meta_edc_demo.egg-info/requires.txt
+-rw-r--r--   0 estellaye   (501) staff       (20)      233 2023-06-27 06:22:40.000000 meta-edc-demo-0.0.2/meta_edc_demo.egg-info/top_level.txt
+drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-06-27 06:22:40.253019 meta-edc-demo-0.0.2/meta_export/
+-rw-r--r--   0 estellaye   (501) staff       (20)        0 2020-03-15 03:34:20.000000 meta-edc-demo-0.0.2/meta_export/__init__.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      167 2021-07-02 03:53:00.000000 meta-edc-demo-0.0.2/meta_export/admin_site.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      226 2021-08-09 19:25:29.000000 meta-edc-demo-0.0.2/meta_export/apps.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      205 2022-06-24 09:12:54.000000 meta-edc-demo-0.0.2/meta_export/urls.py
+drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-06-27 06:22:40.254105 meta-edc-demo-0.0.2/meta_labs/
+-rw-r--r--   0 estellaye   (501) staff       (20)        0 2021-07-02 03:53:00.000000 meta-edc-demo-0.0.2/meta_labs/__init__.py
+-rw-r--r--   0 estellaye   (501) staff       (20)       87 2021-07-05 19:24:26.000000 meta-edc-demo-0.0.2/meta_labs/aliquot_types.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      200 2022-08-23 13:24:02.000000 meta-edc-demo-0.0.2/meta_labs/apps.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      957 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.2/meta_labs/lab_profiles.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      128 2022-06-24 09:12:03.000000 meta-edc-demo-0.0.2/meta_labs/labs.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      477 2022-06-24 09:12:00.000000 meta-edc-demo-0.0.2/meta_labs/list_data.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      500 2022-06-24 09:11:58.000000 meta-edc-demo-0.0.2/meta_labs/processing_profiles.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      512 2022-07-19 19:44:25.000000 meta-edc-demo-0.0.2/meta_labs/reportables.py
+drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-06-27 06:22:40.254631 meta-edc-demo-0.0.2/meta_labs/tests/
+-rw-r--r--   0 estellaye   (501) staff       (20)        0 2020-03-15 03:34:20.000000 meta-edc-demo-0.0.2/meta_labs/tests/__init__.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      967 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.2/meta_labs/tests/test_labs.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      516 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.2/meta_labs/tests/test_reportables.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      111 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.2/meta_labs/tests/urls.py
+drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-06-27 06:22:40.255633 meta-edc-demo-0.0.2/meta_lists/
+-rw-r--r--   0 estellaye   (501) staff       (20)        0 2020-03-15 03:34:20.000000 meta-edc-demo-0.0.2/meta_lists/__init__.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     1400 2022-06-24 09:11:32.000000 meta-edc-demo-0.0.2/meta_lists/admin.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      165 2022-06-24 09:11:34.000000 meta-edc-demo-0.0.2/meta_lists/admin_site.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      278 2022-08-23 13:24:02.000000 meta-edc-demo-0.0.2/meta_lists/apps.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     7823 2022-07-08 07:31:04.000000 meta-edc-demo-0.0.2/meta_lists/list_data.py
+drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-06-27 06:22:40.258002 meta-edc-demo-0.0.2/meta_lists/migrations/
+-rw-r--r--   0 estellaye   (501) staff       (20)    13882 2020-03-15 03:34:20.000000 meta-edc-demo-0.0.2/meta_lists/migrations/0001_initial.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     4609 2022-08-22 17:23:22.000000 meta-edc-demo-0.0.2/meta_lists/migrations/0002_auto_20191026_2231.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     2556 2020-03-15 03:34:20.000000 meta-edc-demo-0.0.2/meta_lists/migrations/0003_auto_20191102_0033.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     2548 2020-03-15 03:34:20.000000 meta-edc-demo-0.0.2/meta_lists/migrations/0004_auto_20191102_1859.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     2584 2020-03-15 03:34:20.000000 meta-edc-demo-0.0.2/meta_lists/migrations/0005_auto_20191104_0930.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     4479 2020-05-15 02:40:42.000000 meta-edc-demo-0.0.2/meta_lists/migrations/0006_auto_20200514_1959.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     2962 2020-05-20 04:57:20.000000 meta-edc-demo-0.0.2/meta_lists/migrations/0007_auto_20200516_2356.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      683 2021-08-09 19:25:29.000000 meta-edc-demo-0.0.2/meta_lists/migrations/0008_auto_20200528_1517.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      358 2020-06-18 19:11:34.000000 meta-edc-demo-0.0.2/meta_lists/migrations/0009_auto_20200613_2041.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     1195 2022-06-24 09:11:24.000000 meta-edc-demo-0.0.2/meta_lists/migrations/0010_auto_20200617_1738.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     1849 2022-06-24 09:11:21.000000 meta-edc-demo-0.0.2/meta_lists/migrations/0011_auto_20210624_0225.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     2812 2022-06-24 09:11:19.000000 meta-edc-demo-0.0.2/meta_lists/migrations/0012_auto_20210728_1809.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     2534 2022-08-22 17:23:22.000000 meta-edc-demo-0.0.2/meta_lists/migrations/0013_transferreasons_and_more.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     2528 2022-09-15 02:57:38.000000 meta-edc-demo-0.0.2/meta_lists/migrations/0014_auto_20220913_2139.py
+-rw-r--r--   0 estellaye   (501) staff       (20)        0 2020-03-15 03:34:20.000000 meta-edc-demo-0.0.2/meta_lists/migrations/__init__.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     2011 2022-07-08 07:31:04.000000 meta-edc-demo-0.0.2/meta_lists/models.py
+drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-06-27 06:22:40.258214 meta-edc-demo-0.0.2/meta_lists/tests/
+-rw-r--r--   0 estellaye   (501) staff       (20)        0 2020-03-15 03:34:20.000000 meta-edc-demo-0.0.2/meta_lists/tests/__init__.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      212 2022-06-24 09:11:29.000000 meta-edc-demo-0.0.2/meta_lists/tests/test_lists.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      204 2021-08-09 19:25:29.000000 meta-edc-demo-0.0.2/meta_lists/urls.py
+drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-06-27 06:22:40.258932 meta-edc-demo-0.0.2/meta_pharmacy/
+-rw-r--r--   0 estellaye   (501) staff       (20)        0 2022-04-11 18:27:09.000000 meta-edc-demo-0.0.2/meta_pharmacy/__init__.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      599 2022-08-23 13:24:02.000000 meta-edc-demo-0.0.2/meta_pharmacy/apps.py
+-rw-r--r--   0 estellaye   (501) staff       (20)       24 2022-04-11 18:27:09.000000 meta-edc-demo-0.0.2/meta_pharmacy/constants.py
+drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-06-27 06:22:40.259108 meta-edc-demo-0.0.2/meta_pharmacy/migrations/
+-rw-r--r--   0 estellaye   (501) staff       (20)        0 2022-04-11 18:27:09.000000 meta-edc-demo-0.0.2/meta_pharmacy/migrations/__init__.py
+-rw-r--r--   0 estellaye   (501) staff       (20)        0 2022-04-11 18:27:09.000000 meta-edc-demo-0.0.2/meta_pharmacy/models.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     2945 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.2/meta_pharmacy/prepare_meta_pharmacy.py
+drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-06-27 06:22:40.260618 meta-edc-demo-0.0.2/meta_prn/
+-rw-r--r--   0 estellaye   (501) staff       (20)        0 2020-03-15 03:34:20.000000 meta-edc-demo-0.0.2/meta_prn/__init__.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     7449 2022-09-27 03:17:01.000000 meta-edc-demo-0.0.2/meta_prn/action_items.py
+drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-06-27 06:22:40.262683 meta-edc-demo-0.0.2/meta_prn/admin/
+-rw-r--r--   0 estellaye   (501) staff       (20)      591 2022-09-26 19:37:19.000000 meta-edc-demo-0.0.2/meta_prn/admin/__init__.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     5155 2022-09-26 19:37:19.000000 meta-edc-demo-0.0.2/meta_prn/admin/end_of_study_admin.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     1770 2022-08-23 13:24:02.000000 meta-edc-demo-0.0.2/meta_prn/admin/loss_to_followup_admin.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     2411 2022-09-26 19:37:19.000000 meta-edc-demo-0.0.2/meta_prn/admin/off_study_medication_admin.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     1741 2022-08-23 13:24:02.000000 meta-edc-demo-0.0.2/meta_prn/admin/offschedule_admin.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     1655 2022-08-23 13:24:02.000000 meta-edc-demo-0.0.2/meta_prn/admin/offschedule_postnatal_admin.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     1737 2022-08-23 13:24:02.000000 meta-edc-demo-0.0.2/meta_prn/admin/offschedule_pregnancy_admin.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     1474 2022-08-23 13:24:02.000000 meta-edc-demo-0.0.2/meta_prn/admin/onschedule_admin.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     2178 2022-08-23 13:24:02.000000 meta-edc-demo-0.0.2/meta_prn/admin/pregnancy_notification_admin.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     4039 2022-09-26 19:37:19.000000 meta-edc-demo-0.0.2/meta_prn/admin/protocol_incident_admin.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      651 2022-08-23 13:24:02.000000 meta-edc-demo-0.0.2/meta_prn/admin/subject_transfer_admin.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      161 2022-06-24 09:09:37.000000 meta-edc-demo-0.0.2/meta_prn/admin_site.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      280 2022-08-23 13:24:02.000000 meta-edc-demo-0.0.2/meta_prn/apps.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      517 2022-04-11 18:27:09.000000 meta-edc-demo-0.0.2/meta_prn/baker_recipes.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     3157 2022-07-08 07:31:04.000000 meta-edc-demo-0.0.2/meta_prn/choices.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      882 2022-07-08 07:31:04.000000 meta-edc-demo-0.0.2/meta_prn/constants.py
+drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-06-27 06:22:40.263246 meta-edc-demo-0.0.2/meta_prn/form_validators/
+-rw-r--r--   0 estellaye   (501) staff       (20)      111 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.2/meta_prn/form_validators/__init__.py
+-rw-r--r--   0 estellaye   (501) staff       (20)    11247 2022-10-04 03:17:15.000000 meta-edc-demo-0.0.2/meta_prn/form_validators/end_of_study.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     1069 2022-10-04 03:17:15.000000 meta-edc-demo-0.0.2/meta_prn/form_validators/protocol_incident.py
+drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-06-27 06:22:40.264727 meta-edc-demo-0.0.2/meta_prn/forms/
+-rw-r--r--   0 estellaye   (501) staff       (20)      452 2022-09-26 19:37:19.000000 meta-edc-demo-0.0.2/meta_prn/forms/__init__.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      927 2022-10-04 03:17:15.000000 meta-edc-demo-0.0.2/meta_prn/forms/end_of_study_form.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     1334 2022-10-04 03:17:15.000000 meta-edc-demo-0.0.2/meta_prn/forms/loss_to_followup_form.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     2296 2022-10-04 03:17:15.000000 meta-edc-demo-0.0.2/meta_prn/forms/off_study_medication_form.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      940 2022-10-04 03:17:15.000000 meta-edc-demo-0.0.2/meta_prn/forms/offschedule_form.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     1102 2022-10-04 03:17:15.000000 meta-edc-demo-0.0.2/meta_prn/forms/offschedule_pregnancy_form.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     4883 2022-10-04 03:17:15.000000 meta-edc-demo-0.0.2/meta_prn/forms/pregnancy_notification_form.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      231 2022-09-27 03:17:01.000000 meta-edc-demo-0.0.2/meta_prn/forms/protocol_incident_form.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      818 2022-10-04 03:17:15.000000 meta-edc-demo-0.0.2/meta_prn/forms/subject_transfer_form.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     2336 2022-09-27 03:17:01.000000 meta-edc-demo-0.0.2/meta_prn/list_data.py
+drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-06-27 06:22:40.275043 meta-edc-demo-0.0.2/meta_prn/migrations/
+-rw-r--r--   0 estellaye   (501) staff       (20)   108120 2022-09-30 02:18:01.000000 meta-edc-demo-0.0.2/meta_prn/migrations/0001_initial.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     2332 2021-07-05 19:24:26.000000 meta-edc-demo-0.0.2/meta_prn/migrations/0002_auto_20191024_1000.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      882 2020-04-08 01:09:11.000000 meta-edc-demo-0.0.2/meta_prn/migrations/0003_auto_20200120_2020.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      756 2020-04-08 01:09:11.000000 meta-edc-demo-0.0.2/meta_prn/migrations/0004_auto_20200403_0332.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     4270 2021-07-05 19:24:26.000000 meta-edc-demo-0.0.2/meta_prn/migrations/0005_auto_20200524_1944.py
+-rw-r--r--   0 estellaye   (501) staff       (20)    13109 2021-07-05 19:24:26.000000 meta-edc-demo-0.0.2/meta_prn/migrations/0006_auto_20210624_0225.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      880 2022-04-11 18:27:09.000000 meta-edc-demo-0.0.2/meta_prn/migrations/0007_auto_20210721_0335.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     3640 2022-09-27 03:17:01.000000 meta-edc-demo-0.0.2/meta_prn/migrations/0008_auto_20210910_0238.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     2873 2022-09-27 03:17:01.000000 meta-edc-demo-0.0.2/meta_prn/migrations/0009_auto_20210910_0239.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     2792 2022-09-27 03:17:01.000000 meta-edc-demo-0.0.2/meta_prn/migrations/0010_auto_20210910_1906.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      897 2022-09-27 03:17:01.000000 meta-edc-demo-0.0.2/meta_prn/migrations/0011_auto_20210910_1911.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      746 2022-09-27 03:17:01.000000 meta-edc-demo-0.0.2/meta_prn/migrations/0012_auto_20210911_0004.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     3118 2022-04-11 18:27:09.000000 meta-edc-demo-0.0.2/meta_prn/migrations/0013_auto_20210911_2036.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      766 2022-06-24 09:10:52.000000 meta-edc-demo-0.0.2/meta_prn/migrations/0014_auto_20211003_1709.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     5915 2022-09-27 03:17:01.000000 meta-edc-demo-0.0.2/meta_prn/migrations/0015_auto_20211104_1447.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     5844 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.2/meta_prn/migrations/0016_auto_20220128_1719.py
+-rw-r--r--   0 estellaye   (501) staff       (20)    26859 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.2/meta_prn/migrations/0017_auto_20220307_1929.py
+-rw-r--r--   0 estellaye   (501) staff       (20)    34942 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.2/meta_prn/migrations/0018_auto_20220309_2106.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     1166 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.2/meta_prn/migrations/0019_auto_20220309_2230.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     2042 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.2/meta_prn/migrations/0020_auto_20220310_0439.py
+-rw-r--r--   0 estellaye   (501) staff       (20)    43329 2022-09-30 02:18:01.000000 meta-edc-demo-0.0.2/meta_prn/migrations/0021_auto_20220316_2147.py
+-rw-r--r--   0 estellaye   (501) staff       (20)    27549 2022-09-30 02:18:01.000000 meta-edc-demo-0.0.2/meta_prn/migrations/0022_auto_20220318_0133.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     2419 2022-09-30 02:18:01.000000 meta-edc-demo-0.0.2/meta_prn/migrations/0023_auto_20220415_1747.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      793 2022-09-27 03:17:01.000000 meta-edc-demo-0.0.2/meta_prn/migrations/0024_alter_protocoldeviationviolation_violation.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     6265 2022-09-27 03:17:01.000000 meta-edc-demo-0.0.2/meta_prn/migrations/0025_alter_historicalprotocoldeviationviolation_options_and_more.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     3926 2022-09-27 03:17:01.000000 meta-edc-demo-0.0.2/meta_prn/migrations/0026_remove_historicalprotocoldeviationviolation_violation_type_and_more.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     1285 2022-09-27 03:17:01.000000 meta-edc-demo-0.0.2/meta_prn/migrations/0027_rename_historicalprotocoldeviationviolation_historicalprotocolincident_and_more.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     1920 2022-08-22 17:23:22.000000 meta-edc-demo-0.0.2/meta_prn/migrations/0028_historicalpregnancynotification_bhcg_date_and_more.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      662 2022-08-22 17:23:22.000000 meta-edc-demo-0.0.2/meta_prn/migrations/0029_alter_historicalpregnancynotification_edd_and_more.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     1255 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.2/meta_prn/migrations/0030_auto_20220627_1119.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     1841 2022-08-22 17:23:22.000000 meta-edc-demo-0.0.2/meta_prn/migrations/0031_alter_historicaloffschedule_options_and_more.py
+-rw-r--r--   0 estellaye   (501) staff       (20)    17576 2022-09-30 02:18:01.000000 meta-edc-demo-0.0.2/meta_prn/migrations/0032_historicalegfrnotification_egfrnotification.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     1070 2022-08-22 17:23:22.000000 meta-edc-demo-0.0.2/meta_prn/migrations/0033_remove_historicalegfrnotification_action_item_and_more.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     2076 2022-09-27 03:17:01.000000 meta-edc-demo-0.0.2/meta_prn/migrations/0034_auto_20220630_1110.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     3448 2022-10-11 02:24:52.000000 meta-edc-demo-0.0.2/meta_prn/migrations/0035_auto_20220630_1140.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     1392 2022-08-22 17:23:22.000000 meta-edc-demo-0.0.2/meta_prn/migrations/0036_remove_endofstudy_meta_prn_en_id_a50384_idx_and_more.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     7339 2022-08-22 17:23:22.000000 meta-edc-demo-0.0.2/meta_prn/migrations/0037_endofstudy_delivery_date_endofstudy_pregnancy_date_and_more.py
+-rw-r--r--   0 estellaye   (501) staff       (20)    21786 2022-09-30 02:18:01.000000 meta-edc-demo-0.0.2/meta_prn/migrations/0038_alter_endofstudy_delivery_date_and_more.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     1012 2022-08-22 17:23:22.000000 meta-edc-demo-0.0.2/meta_prn/migrations/0039_historicaloffstudymedication_reason_other_and_more.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     4594 2022-08-22 17:23:22.000000 meta-edc-demo-0.0.2/meta_prn/migrations/0040_remove_historicaloffstudymedication_expected_restart_date_and_more.py
+-rw-r--r--   0 estellaye   (501) staff       (20)    26300 2022-09-30 02:18:01.000000 meta-edc-demo-0.0.2/meta_prn/migrations/0041_endofstudy_transfer_date_and_more.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     6199 2022-08-22 17:23:22.000000 meta-edc-demo-0.0.2/meta_prn/migrations/0042_remove_endofstudy_investigator_decision_and_more.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     7240 2022-08-22 17:23:22.000000 meta-edc-demo-0.0.2/meta_prn/migrations/0043_auto_20220704_1841.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     3926 2022-08-23 13:31:01.000000 meta-edc-demo-0.0.2/meta_prn/migrations/0044_alter_endofstudy_action_identifier_and_more.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     4150 2022-08-26 02:59:33.000000 meta-edc-demo-0.0.2/meta_prn/migrations/0045_auto_20220826_0258.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     3945 2022-08-26 02:59:33.000000 meta-edc-demo-0.0.2/meta_prn/migrations/0046_auto_20220826_0322.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     2587 2022-08-26 02:59:33.000000 meta-edc-demo-0.0.2/meta_prn/migrations/0047_auto_20220826_0406.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     2497 2022-09-26 19:37:19.000000 meta-edc-demo-0.0.2/meta_prn/migrations/0048_auto_20220922_2236.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     3937 2022-09-30 02:18:01.000000 meta-edc-demo-0.0.2/meta_prn/migrations/0049_auto_20220929_1742.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     1251 2022-10-04 03:32:52.000000 meta-edc-demo-0.0.2/meta_prn/migrations/0050_auto_20221004_0629.py
+-rw-r--r--   0 estellaye   (501) staff       (20)        0 2020-03-15 03:34:20.000000 meta-edc-demo-0.0.2/meta_prn/migrations/__init__.py
+drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-06-27 06:22:40.276601 meta-edc-demo-0.0.2/meta_prn/models/
+-rw-r--r--   0 estellaye   (501) staff       (20)      594 2022-09-26 19:37:19.000000 meta-edc-demo-0.0.2/meta_prn/models/__init__.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     5311 2022-09-30 02:18:01.000000 meta-edc-demo-0.0.2/meta_prn/models/end_of_study.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     2431 2022-09-30 02:18:01.000000 meta-edc-demo-0.0.2/meta_prn/models/loss_to_followup.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     1696 2022-10-04 03:17:15.000000 meta-edc-demo-0.0.2/meta_prn/models/off_study_medication.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     1310 2022-09-30 02:18:01.000000 meta-edc-demo-0.0.2/meta_prn/models/offschedule.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      672 2022-09-30 02:18:01.000000 meta-edc-demo-0.0.2/meta_prn/models/onschedule.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     3124 2022-09-30 02:18:01.000000 meta-edc-demo-0.0.2/meta_prn/models/pregnancy_notification.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     1084 2022-09-30 02:18:01.000000 meta-edc-demo-0.0.2/meta_prn/models/protocol_incident.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     2480 2022-09-26 19:37:19.000000 meta-edc-demo-0.0.2/meta_prn/models/signals.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      266 2022-09-30 02:18:01.000000 meta-edc-demo-0.0.2/meta_prn/models/subject_transfer.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      978 2022-09-26 19:37:19.000000 meta-edc-demo-0.0.2/meta_prn/pregnancy_action_item_mixin.py
+drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-06-27 06:22:40.276898 meta-edc-demo-0.0.2/meta_prn/tests/
+-rw-r--r--   0 estellaye   (501) staff       (20)        0 2020-03-15 03:34:20.000000 meta-edc-demo-0.0.2/meta_prn/tests/__init__.py
+drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-06-27 06:22:40.277513 meta-edc-demo-0.0.2/meta_prn/tests/tests/
+-rw-r--r--   0 estellaye   (501) staff       (20)        0 2020-03-15 03:34:20.000000 meta-edc-demo-0.0.2/meta_prn/tests/tests/__init__.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     3767 2022-07-08 07:31:04.000000 meta-edc-demo-0.0.2/meta_prn/tests/tests/test_actions.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      557 2022-10-04 03:17:15.000000 meta-edc-demo-0.0.2/meta_prn/tests/tests/test_manager_order.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     3983 2022-06-24 09:09:25.000000 meta-edc-demo-0.0.2/meta_prn/tests/tests/test_pregnancy_notification.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      270 2022-06-24 09:09:29.000000 meta-edc-demo-0.0.2/meta_prn/tests/urls.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      202 2022-06-24 09:09:57.000000 meta-edc-demo-0.0.2/meta_prn/urls.py
+drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-06-27 06:22:40.278131 meta-edc-demo-0.0.2/meta_rando/
+-rw-r--r--   0 estellaye   (501) staff       (20)        0 2021-08-09 19:25:29.000000 meta-edc-demo-0.0.2/meta_rando/__init__.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      256 2022-08-23 13:24:02.000000 meta-edc-demo-0.0.2/meta_rando/apps.py
+drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-06-27 06:22:40.278796 meta-edc-demo-0.0.2/meta_rando/migrations/
+-rw-r--r--   0 estellaye   (501) staff       (20)    13433 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.2/meta_rando/migrations/0001_initial.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      836 2022-08-22 17:23:22.000000 meta-edc-demo-0.0.2/meta_rando/migrations/0002_auto_20220704_1841.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     1226 2022-08-26 13:58:46.000000 meta-edc-demo-0.0.2/meta_rando/migrations/0003_auto_20220826_1640.py
+-rw-r--r--   0 estellaye   (501) staff       (20)        0 2021-08-09 19:25:29.000000 meta-edc-demo-0.0.2/meta_rando/migrations/__init__.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      533 2022-08-26 02:59:33.000000 meta-edc-demo-0.0.2/meta_rando/models.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     1592 2022-08-22 17:23:22.000000 meta-edc-demo-0.0.2/meta_rando/randomizers.py
+drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-06-27 06:22:40.278933 meta-edc-demo-0.0.2/meta_rando/tests/
+-rw-r--r--   0 estellaye   (501) staff       (20)        0 2021-08-09 19:25:29.000000 meta-edc-demo-0.0.2/meta_rando/tests/__init__.py
+drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-06-27 06:22:40.279212 meta-edc-demo-0.0.2/meta_rando/tests/tests/
+-rw-r--r--   0 estellaye   (501) staff       (20)        0 2021-08-09 19:25:29.000000 meta-edc-demo-0.0.2/meta_rando/tests/tests/__init__.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     2279 2022-09-27 03:17:01.000000 meta-edc-demo-0.0.2/meta_rando/tests/tests/test_randomizers.py
+drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-06-27 06:22:40.279897 meta-edc-demo-0.0.2/meta_reference/
+-rw-r--r--   0 estellaye   (501) staff       (20)        0 2020-03-15 03:34:20.000000 meta-edc-demo-0.0.2/meta_reference/__init__.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      153 2022-08-23 13:24:02.000000 meta-edc-demo-0.0.2/meta_reference/apps.py
+drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-06-27 06:22:40.280061 meta-edc-demo-0.0.2/meta_reference/migrations/
+-rw-r--r--   0 estellaye   (501) staff       (20)        0 2020-06-18 19:11:34.000000 meta-edc-demo-0.0.2/meta_reference/migrations/__init__.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      183 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.2/meta_reference/reference_model_configs.py
+drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-06-27 06:22:40.281307 meta-edc-demo-0.0.2/meta_reports/
+-rw-r--r--   0 estellaye   (501) staff       (20)        0 2020-03-15 03:34:20.000000 meta-edc-demo-0.0.2/meta_reports/__init__.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      143 2022-06-24 09:05:03.000000 meta-edc-demo-0.0.2/meta_reports/ae_report.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      734 2022-08-23 13:24:02.000000 meta-edc-demo-0.0.2/meta_reports/apps.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     4712 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.2/meta_reports/death_report.py
+drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-06-27 06:22:40.281545 meta-edc-demo-0.0.2/meta_reports/migrations/
+-rw-r--r--   0 estellaye   (501) staff       (20)        0 2020-03-15 03:34:20.000000 meta-edc-demo-0.0.2/meta_reports/migrations/__init__.py
+-rw-r--r--   0 estellaye   (501) staff       (20)        0 2020-03-15 03:34:20.000000 meta-edc-demo-0.0.2/meta_reports/models.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     2397 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.2/meta_reports/pdf_report.py
+drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-06-27 06:22:40.282327 meta-edc-demo-0.0.2/meta_reports/tests/
+-rw-r--r--   0 estellaye   (501) staff       (20)        0 2020-03-15 03:34:20.000000 meta-edc-demo-0.0.2/meta_reports/tests/__init__.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     1282 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.2/meta_reports/tests/test_reports.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      111 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.2/meta_reports/tests/urls.py
+drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-06-27 06:22:40.284169 meta-edc-demo-0.0.2/meta_screening/
+-rw-r--r--   0 estellaye   (501) staff       (20)        0 2020-03-15 03:34:20.000000 meta-edc-demo-0.0.2/meta_screening/__init__.py
+drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-06-27 06:22:40.285867 meta-edc-demo-0.0.2/meta_screening/admin/
+-rw-r--r--   0 estellaye   (501) staff       (20)      298 2022-04-11 18:27:09.000000 meta-edc-demo-0.0.2/meta_screening/admin/__init__.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     5077 2022-08-22 17:23:22.000000 meta-edc-demo-0.0.2/meta_screening/admin/fieldsets.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     2749 2022-08-23 13:24:02.000000 meta-edc-demo-0.0.2/meta_screening/admin/list_filters.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      999 2022-08-22 17:23:22.000000 meta-edc-demo-0.0.2/meta_screening/admin/screening_part_one_admin.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     2524 2022-08-22 17:23:22.000000 meta-edc-demo-0.0.2/meta_screening/admin/screening_part_three_admin.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     1308 2022-08-22 17:23:22.000000 meta-edc-demo-0.0.2/meta_screening/admin/screening_part_two_admin.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     2170 2022-08-23 13:24:02.000000 meta-edc-demo-0.0.2/meta_screening/admin/subject_refusal_admin.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     6689 2022-10-04 03:17:15.000000 meta-edc-demo-0.0.2/meta_screening/admin/subject_screening_admin.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      173 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.2/meta_screening/admin_site.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      543 2022-08-23 13:24:02.000000 meta-edc-demo-0.0.2/meta_screening/apps.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     1705 2022-06-24 09:06:35.000000 meta-edc-demo-0.0.2/meta_screening/baker_recipes.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     1948 2022-06-24 09:06:38.000000 meta-edc-demo-0.0.2/meta_screening/calculators.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      789 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.2/meta_screening/choices.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      655 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.2/meta_screening/constants.py
+drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-06-27 06:22:40.286548 meta-edc-demo-0.0.2/meta_screening/eligibility/
+-rw-r--r--   0 estellaye   (501) staff       (20)      284 2022-08-22 17:23:22.000000 meta-edc-demo-0.0.2/meta_screening/eligibility/__init__.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     7732 2022-07-08 07:31:04.000000 meta-edc-demo-0.0.2/meta_screening/eligibility/eligibility.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     1770 2022-10-13 03:34:11.000000 meta-edc-demo-0.0.2/meta_screening/eligibility/eligibility_part_one.py
+drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-06-27 06:22:40.287146 meta-edc-demo-0.0.2/meta_screening/eligibility/eligibility_part_three/
+-rw-r--r--   0 estellaye   (501) staff       (20)       79 2022-04-11 18:27:09.000000 meta-edc-demo-0.0.2/meta_screening/eligibility/eligibility_part_three/__init__.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     5405 2022-10-13 03:34:11.000000 meta-edc-demo-0.0.2/meta_screening/eligibility/eligibility_part_three/base_eligibility_part_three.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     4296 2022-10-13 03:34:11.000000 meta-edc-demo-0.0.2/meta_screening/eligibility/eligibility_part_three/eligibility_part_three_phase_three.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     1809 2022-10-13 03:34:11.000000 meta-edc-demo-0.0.2/meta_screening/eligibility/eligibility_part_two.py
+drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-06-27 06:22:40.288210 meta-edc-demo-0.0.2/meta_screening/form_validators/
+-rw-r--r--   0 estellaye   (501) staff       (20)      308 2022-04-11 18:27:09.000000 meta-edc-demo-0.0.2/meta_screening/form_validators/__init__.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     1361 2022-10-04 03:17:15.000000 meta-edc-demo-0.0.2/meta_screening/form_validators/screening_part_one.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     7745 2022-10-04 03:17:15.000000 meta-edc-demo-0.0.2/meta_screening/form_validators/screening_part_three.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     4712 2022-10-04 03:17:15.000000 meta-edc-demo-0.0.2/meta_screening/form_validators/screening_part_two.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      322 2022-10-04 03:17:15.000000 meta-edc-demo-0.0.2/meta_screening/form_validators/subject_refusal.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      309 2022-06-24 09:04:37.000000 meta-edc-demo-0.0.2/meta_screening/form_validators/subject_screening.py
+drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-06-27 06:22:40.289589 meta-edc-demo-0.0.2/meta_screening/forms/
+-rw-r--r--   0 estellaye   (501) staff       (20)      614 2022-07-19 13:21:21.000000 meta-edc-demo-0.0.2/meta_screening/forms/__init__.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     3279 2022-08-22 17:23:22.000000 meta-edc-demo-0.0.2/meta_screening/forms/field_lists.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      518 2022-07-19 13:21:21.000000 meta-edc-demo-0.0.2/meta_screening/forms/screening_part_one_form.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      988 2022-07-19 13:21:21.000000 meta-edc-demo-0.0.2/meta_screening/forms/screening_part_three_form.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      702 2022-08-22 17:23:22.000000 meta-edc-demo-0.0.2/meta_screening/forms/screening_part_two_form.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      625 2022-08-22 17:23:22.000000 meta-edc-demo-0.0.2/meta_screening/forms/subject_refusal_form.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      560 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.2/meta_screening/forms/subject_screening_form.py
+drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-06-27 06:22:40.303761 meta-edc-demo-0.0.2/meta_screening/migrations/
+-rw-r--r--   0 estellaye   (501) staff       (20)   186856 2022-08-22 17:23:22.000000 meta-edc-demo-0.0.2/meta_screening/migrations/0001_initial.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     4468 2020-04-08 01:09:11.000000 meta-edc-demo-0.0.2/meta_screening/migrations/0002_auto_20191020_0612.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     5514 2020-04-08 01:09:11.000000 meta-edc-demo-0.0.2/meta_screening/migrations/0003_auto_20191020_0627.py
+-rw-r--r--   0 estellaye   (501) staff       (20)    14317 2020-04-08 01:09:11.000000 meta-edc-demo-0.0.2/meta_screening/migrations/0004_auto_20191020_0738.py
+-rw-r--r--   0 estellaye   (501) staff       (20)    10373 2020-04-08 01:09:11.000000 meta-edc-demo-0.0.2/meta_screening/migrations/0005_auto_20191021_0353.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     6711 2020-04-08 01:09:11.000000 meta-edc-demo-0.0.2/meta_screening/migrations/0006_auto_20191022_0134.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      951 2021-07-05 19:24:26.000000 meta-edc-demo-0.0.2/meta_screening/migrations/0007_auto_20191024_1000.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     6149 2020-04-08 01:09:11.000000 meta-edc-demo-0.0.2/meta_screening/migrations/0008_auto_20191031_0745.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     6109 2020-04-08 01:09:11.000000 meta-edc-demo-0.0.2/meta_screening/migrations/0009_auto_20191105_0122.py
+-rw-r--r--   0 estellaye   (501) staff       (20)    36964 2021-07-05 19:24:26.000000 meta-edc-demo-0.0.2/meta_screening/migrations/0010_auto_20191106_0828.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     7305 2021-07-05 19:24:26.000000 meta-edc-demo-0.0.2/meta_screening/migrations/0011_auto_20191107_0342.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      776 2022-04-11 18:27:09.000000 meta-edc-demo-0.0.2/meta_screening/migrations/0012_auto_20191107_0427.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     7883 2021-08-09 19:25:29.000000 meta-edc-demo-0.0.2/meta_screening/migrations/0013_auto_20191107_0442.py
+-rw-r--r--   0 estellaye   (501) staff       (20)    17408 2020-04-08 01:09:11.000000 meta-edc-demo-0.0.2/meta_screening/migrations/0014_auto_20191107_0528.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     1187 2020-04-08 01:09:11.000000 meta-edc-demo-0.0.2/meta_screening/migrations/0015_auto_20191107_2249.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     4804 2020-04-08 01:09:11.000000 meta-edc-demo-0.0.2/meta_screening/migrations/0016_auto_20191119_2331.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     2822 2020-04-08 01:09:11.000000 meta-edc-demo-0.0.2/meta_screening/migrations/0017_auto_20191213_0314.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     5090 2021-08-09 19:25:29.000000 meta-edc-demo-0.0.2/meta_screening/migrations/0018_auto_20200118_1854.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     4109 2020-04-08 01:09:11.000000 meta-edc-demo-0.0.2/meta_screening/migrations/0019_auto_20200120_2256.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     8403 2020-06-18 19:11:34.000000 meta-edc-demo-0.0.2/meta_screening/migrations/0020_auto_20200524_1944.py
+-rw-r--r--   0 estellaye   (501) staff       (20)    25509 2021-07-02 03:53:00.000000 meta-edc-demo-0.0.2/meta_screening/migrations/0021_auto_20210628_2105.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     2292 2021-07-05 19:24:26.000000 meta-edc-demo-0.0.2/meta_screening/migrations/0022_auto_20210702_0426.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     2893 2021-07-05 19:24:26.000000 meta-edc-demo-0.0.2/meta_screening/migrations/0023_auto_20210702_0533.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     4284 2022-04-11 18:27:09.000000 meta-edc-demo-0.0.2/meta_screening/migrations/0024_auto_20210710_1929.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     4816 2022-04-11 18:27:09.000000 meta-edc-demo-0.0.2/meta_screening/migrations/0025_auto_20210710_2247.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     2422 2022-06-24 08:57:53.000000 meta-edc-demo-0.0.2/meta_screening/migrations/0026_auto_20210712_0433.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      227 2022-06-24 08:57:50.000000 meta-edc-demo-0.0.2/meta_screening/migrations/0027_auto_20210804_0438.py
+-rw-r--r--   0 estellaye   (501) staff       (20)    14430 2022-06-24 08:57:48.000000 meta-edc-demo-0.0.2/meta_screening/migrations/0028_auto_20210823_2353.py
+-rw-r--r--   0 estellaye   (501) staff       (20)    25297 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.2/meta_screening/migrations/0029_auto_20211123_1645.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     1612 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.2/meta_screening/migrations/0030_auto_20220128_1719.py
+-rw-r--r--   0 estellaye   (501) staff       (20)    10216 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.2/meta_screening/migrations/0031_auto_20220304_0448.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     5507 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.2/meta_screening/migrations/0032_auto_20220304_0501.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     2168 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.2/meta_screening/migrations/0033_auto_20220304_0504.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     6547 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.2/meta_screening/migrations/0034_auto_20220304_0508.py
+-rw-r--r--   0 estellaye   (501) staff       (20)    36493 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.2/meta_screening/migrations/0035_auto_20220304_2233.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     5610 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.2/meta_screening/migrations/0036_auto_20220304_2307.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     5030 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.2/meta_screening/migrations/0037_auto_20220312_0339.py
+-rw-r--r--   0 estellaye   (501) staff       (20)    10873 2022-06-24 08:57:21.000000 meta-edc-demo-0.0.2/meta_screening/migrations/0038_auto_20220312_1929.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     6643 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.2/meta_screening/migrations/0039_auto_20220312_1938.py
+-rw-r--r--   0 estellaye   (501) staff       (20)    20941 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.2/meta_screening/migrations/0040_auto_20220316_2147.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     2663 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.2/meta_screening/migrations/0041_auto_20220403_1227.py
+-rw-r--r--   0 estellaye   (501) staff       (20)    15666 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.2/meta_screening/migrations/0042_auto_20220403_1402.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     5505 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.2/meta_screening/migrations/0043_auto_20220407_1713.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     4909 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.2/meta_screening/migrations/0044_alter_historicalscreeningpartone_severe_htn_and_more.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     1919 2022-08-22 17:23:22.000000 meta-edc-demo-0.0.2/meta_screening/migrations/0045_historicalscreeningpartone_contact_number_and_more.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     1984 2022-08-22 17:23:22.000000 meta-edc-demo-0.0.2/meta_screening/migrations/0046_historicalscreeningpartone_hba1c_datetime_and_more.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     2354 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.2/meta_screening/migrations/0047_historicalscreeningpartone_appt_datetime_repeat_and_more.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     1192 2022-08-22 17:23:22.000000 meta-edc-demo-0.0.2/meta_screening/migrations/0048_rename_appt_datetime_repeat_historicalscreeningpartone_repeat_appt_datetime_and_more.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     9620 2022-08-22 17:23:22.000000 meta-edc-demo-0.0.2/meta_screening/migrations/0049_historicalscreeningpartone_p3_ltfu_and_more.py
+-rw-r--r--   0 estellaye   (501) staff       (20)    11995 2022-08-22 17:23:22.000000 meta-edc-demo-0.0.2/meta_screening/migrations/0050_historicalscreeningpartone_agree_to_p3_and_more.py
+-rw-r--r--   0 estellaye   (501) staff       (20)    11972 2022-08-22 17:23:22.000000 meta-edc-demo-0.0.2/meta_screening/migrations/0051_alter_historicalscreeningpartone_advised_to_fast_and_more.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     3891 2022-08-22 17:23:22.000000 meta-edc-demo-0.0.2/meta_screening/migrations/0052_alter_historicalscreeningpartone_p3_ltfu_and_more.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     3782 2022-08-22 17:23:22.000000 meta-edc-demo-0.0.2/meta_screening/migrations/0053_auto_20220704_1841.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     6029 2022-08-22 17:23:22.000000 meta-edc-demo-0.0.2/meta_screening/migrations/0054_auto_20220722_2130.py
+-rw-r--r--   0 estellaye   (501) staff       (20)    18774 2022-08-22 17:23:22.000000 meta-edc-demo-0.0.2/meta_screening/migrations/0055_alter_historicalscreeningpartone_creatinine_value_and_more.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     4225 2022-08-23 13:24:02.000000 meta-edc-demo-0.0.2/meta_screening/migrations/0056_alter_historicalscreeningpartone_agree_to_p3_and_more.py
+-rw-r--r--   0 estellaye   (501) staff       (20)    13644 2022-10-12 03:43:37.000000 meta-edc-demo-0.0.2/meta_screening/migrations/0057_alter_historicalscreeningpartone_calculated_egfr_value_and_more.py
+-rw-r--r--   0 estellaye   (501) staff       (20)        0 2020-03-15 03:34:20.000000 meta-edc-demo-0.0.2/meta_screening/migrations/__init__.py
+drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-06-27 06:22:40.305191 meta-edc-demo-0.0.2/meta_screening/model_mixins/
+-rw-r--r--   0 estellaye   (501) staff       (20)      315 2022-08-26 02:59:33.000000 meta-edc-demo-0.0.2/meta_screening/model_mixins/__init__.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     2762 2022-10-12 03:43:37.000000 meta-edc-demo-0.0.2/meta_screening/model_mixins/calculated_model_mixin.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      593 2022-10-12 03:43:37.000000 meta-edc-demo-0.0.2/meta_screening/model_mixins/creatinine_fields_model_mixin.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     1361 2022-08-26 02:59:33.000000 meta-edc-demo-0.0.2/meta_screening/model_mixins/eligibility_model_mixin.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     3712 2022-08-26 02:59:33.000000 meta-edc-demo-0.0.2/meta_screening/model_mixins/part_one_fields_model_mixin.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     5119 2022-08-26 02:59:33.000000 meta-edc-demo-0.0.2/meta_screening/model_mixins/part_three_fields_model_mixin.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     6693 2022-08-26 02:59:33.000000 meta-edc-demo-0.0.2/meta_screening/model_mixins/part_two_fields_model_mixin.py
+drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-06-27 06:22:40.306209 meta-edc-demo-0.0.2/meta_screening/models/
+-rw-r--r--   0 estellaye   (501) staff       (20)      260 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.2/meta_screening/models/__init__.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     3429 2022-08-22 17:23:22.000000 meta-edc-demo-0.0.2/meta_screening/models/icp_referral.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     1018 2022-06-24 08:56:30.000000 meta-edc-demo-0.0.2/meta_screening/models/proxy_models.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      862 2022-08-26 02:59:33.000000 meta-edc-demo-0.0.2/meta_screening/models/signals.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     2218 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.2/meta_screening/models/subject_refusal.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     1592 2022-08-26 02:59:33.000000 meta-edc-demo-0.0.2/meta_screening/models/subject_screening.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      131 2022-06-24 09:06:52.000000 meta-edc-demo-0.0.2/meta_screening/offline_models.py
+drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-06-27 06:22:40.306714 meta-edc-demo-0.0.2/meta_screening/tests/
+-rw-r--r--   0 estellaye   (501) staff       (20)        0 2020-03-15 03:34:20.000000 meta-edc-demo-0.0.2/meta_screening/tests/__init__.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     8283 2022-09-26 19:37:19.000000 meta-edc-demo-0.0.2/meta_screening/tests/meta_test_case_mixin.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     3871 2022-09-26 19:37:19.000000 meta-edc-demo-0.0.2/meta_screening/tests/options.py
+drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-06-27 06:22:40.307694 meta-edc-demo-0.0.2/meta_screening/tests/tests/
+-rw-r--r--   0 estellaye   (501) staff       (20)        0 2021-08-09 19:25:30.000000 meta-edc-demo-0.0.2/meta_screening/tests/tests/__init__.py
+-rw-r--r--   0 estellaye   (501) staff       (20)    16710 2022-10-04 03:16:43.000000 meta-edc-demo-0.0.2/meta_screening/tests/tests/test_forms.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     4723 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.2/meta_screening/tests/tests/test_screening_part_one.py
+-rw-r--r--   0 estellaye   (501) staff       (20)    16775 2022-08-22 17:23:22.000000 meta-edc-demo-0.0.2/meta_screening/tests/tests/test_screening_part_three.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     3128 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.2/meta_screening/tests/tests/test_screening_part_two.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      208 2022-06-24 09:06:56.000000 meta-edc-demo-0.0.2/meta_screening/urls.py
+drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-06-27 06:22:40.308306 meta-edc-demo-0.0.2/meta_sites/
+-rw-r--r--   0 estellaye   (501) staff       (20)       43 2021-07-05 19:24:26.000000 meta-edc-demo-0.0.2/meta_sites/__init__.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      934 2022-08-23 13:24:02.000000 meta-edc-demo-0.0.2/meta_sites/apps.py
+drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-06-27 06:22:40.308487 meta-edc-demo-0.0.2/meta_sites/migrations/
+-rw-r--r--   0 estellaye   (501) staff       (20)        0 2020-06-18 19:11:34.000000 meta-edc-demo-0.0.2/meta_sites/migrations/__init__.py
+-rw-r--r--   0 estellaye   (501) staff       (20)       46 2020-03-15 03:34:20.000000 meta-edc-demo-0.0.2/meta_sites/models.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     1420 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.2/meta_sites/sites.py
+drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-06-27 06:22:40.309061 meta-edc-demo-0.0.2/meta_sites/tests/
+-rw-r--r--   0 estellaye   (501) staff       (20)        0 2020-03-15 03:34:20.000000 meta-edc-demo-0.0.2/meta_sites/tests/__init__.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      490 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.2/meta_sites/tests/test_sites.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      111 2022-06-24 09:03:07.000000 meta-edc-demo-0.0.2/meta_sites/tests/urls.py
+drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-06-27 06:22:40.310704 meta-edc-demo-0.0.2/meta_subject/
+-rw-r--r--   0 estellaye   (501) staff       (20)        0 2020-03-15 03:34:20.000000 meta-edc-demo-0.0.2/meta_subject/__init__.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     5721 2022-08-22 17:23:22.000000 meta-edc-demo-0.0.2/meta_subject/action_items.py
+drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-06-27 06:22:40.316020 meta-edc-demo-0.0.2/meta_subject/admin/
+-rw-r--r--   0 estellaye   (501) staff       (20)     1614 2022-08-23 01:12:55.000000 meta-edc-demo-0.0.2/meta_subject/admin/__init__.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     1158 2022-06-24 08:59:56.000000 meta-edc-demo-0.0.2/meta_subject/admin/autocomplete_admin.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     3223 2022-08-23 13:24:02.000000 meta-edc-demo-0.0.2/meta_subject/admin/birth_outcome_admin.py
+drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-06-27 06:22:40.317578 meta-edc-demo-0.0.2/meta_subject/admin/blood_results/
+-rw-r--r--   0 estellaye   (501) staff       (20)      414 2021-08-09 19:25:30.000000 meta-edc-demo-0.0.2/meta_subject/admin/blood_results/__init__.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      708 2022-08-22 17:23:22.000000 meta-edc-demo-0.0.2/meta_subject/admin/blood_results/blood_results_fbc_admin.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      976 2022-08-22 17:23:22.000000 meta-edc-demo-0.0.2/meta_subject/admin/blood_results/blood_results_glu_admin.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      770 2022-08-22 17:23:22.000000 meta-edc-demo-0.0.2/meta_subject/admin/blood_results/blood_results_hba1c_admin.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      731 2022-08-22 17:23:22.000000 meta-edc-demo-0.0.2/meta_subject/admin/blood_results/blood_results_ins_admin.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      731 2022-08-22 17:23:22.000000 meta-edc-demo-0.0.2/meta_subject/admin/blood_results/blood_results_lft_admin.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      745 2022-08-22 17:23:22.000000 meta-edc-demo-0.0.2/meta_subject/admin/blood_results/blood_results_lipid_admin.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     5030 2022-09-15 05:11:27.000000 meta-edc-demo-0.0.2/meta_subject/admin/blood_results/blood_results_rft_admin.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     1035 2022-08-22 17:23:22.000000 meta-edc-demo-0.0.2/meta_subject/admin/complications_admin.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     3985 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.2/meta_subject/admin/complications_glycemia_admin.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      740 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.2/meta_subject/admin/concomitant_medication_admin.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     3427 2022-10-07 02:36:16.000000 meta-edc-demo-0.0.2/meta_subject/admin/delivery_admin.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      734 2022-08-23 13:24:02.000000 meta-edc-demo-0.0.2/meta_subject/admin/egfr_drop_notification_admin.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      676 2022-06-24 09:00:18.000000 meta-edc-demo-0.0.2/meta_subject/admin/eq5d3l_admin.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      277 2022-06-24 09:00:25.000000 meta-edc-demo-0.0.2/meta_subject/admin/fields.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     1523 2022-06-24 09:00:28.000000 meta-edc-demo-0.0.2/meta_subject/admin/fieldsets.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     5154 2022-08-26 02:59:33.000000 meta-edc-demo-0.0.2/meta_subject/admin/followup_examination_admin.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     1586 2022-08-23 13:24:02.000000 meta-edc-demo-0.0.2/meta_subject/admin/followup_vitals_admin.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     1613 2022-08-23 01:13:27.000000 meta-edc-demo-0.0.2/meta_subject/admin/glucose_admin.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      949 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.2/meta_subject/admin/health_economics_simple_admin.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     1320 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.2/meta_subject/admin/hepatitis_test_admin.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      978 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.2/meta_subject/admin/malaria_test_admin.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      610 2022-08-23 13:24:02.000000 meta-edc-demo-0.0.2/meta_subject/admin/medication_adherence_admin.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     1421 2022-08-23 13:24:02.000000 meta-edc-demo-0.0.2/meta_subject/admin/mnsi_admin.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      383 2022-08-23 13:24:02.000000 meta-edc-demo-0.0.2/meta_subject/admin/modeladmin.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     1512 2022-10-07 03:13:37.000000 meta-edc-demo-0.0.2/meta_subject/admin/other_arv_regimens_admin.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     1679 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.2/meta_subject/admin/patient_history_admin.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     1774 2022-10-05 21:51:43.000000 meta-edc-demo-0.0.2/meta_subject/admin/physical_exam_admin.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      829 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.2/meta_subject/admin/pregnancy_update_admin.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      658 2022-06-24 09:01:27.000000 meta-edc-demo-0.0.2/meta_subject/admin/sf12_admin.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     4232 2022-09-28 04:05:35.000000 meta-edc-demo-0.0.2/meta_subject/admin/study_medication_admin.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     1764 2022-08-23 13:24:02.000000 meta-edc-demo-0.0.2/meta_subject/admin/subject_requisition_admin.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     1315 2022-08-23 13:24:02.000000 meta-edc-demo-0.0.2/meta_subject/admin/subject_visit_admin.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     1399 2022-08-23 13:24:02.000000 meta-edc-demo-0.0.2/meta_subject/admin/subject_visit_missed_admin.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     1060 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.2/meta_subject/admin/urine_dipstick_test_admin.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      953 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.2/meta_subject/admin/urine_pregnancy_admin.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      169 2022-08-21 16:43:17.000000 meta-edc-demo-0.0.2/meta_subject/admin_site.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      282 2022-08-23 13:24:02.000000 meta-edc-demo-0.0.2/meta_subject/apps.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     2618 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.2/meta_subject/baker_recipes.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     6340 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.2/meta_subject/choices.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      599 2022-08-22 17:23:22.000000 meta-edc-demo-0.0.2/meta_subject/constants.py
+drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-06-27 06:22:40.323011 meta-edc-demo-0.0.2/meta_subject/forms/
+-rw-r--r--   0 estellaye   (501) staff       (20)     1611 2022-08-22 17:23:22.000000 meta-edc-demo-0.0.2/meta_subject/forms/__init__.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      666 2022-09-26 19:37:19.000000 meta-edc-demo-0.0.2/meta_subject/forms/birth_outcomes_form.py
+drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-06-27 06:22:40.324471 meta-edc-demo-0.0.2/meta_subject/forms/blood_results/
+-rw-r--r--   0 estellaye   (501) staff       (20)      400 2021-08-09 19:25:30.000000 meta-edc-demo-0.0.2/meta_subject/forms/blood_results/__init__.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      715 2022-09-26 19:37:19.000000 meta-edc-demo-0.0.2/meta_subject/forms/blood_results/blood_results_fbc_form.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      824 2022-09-26 19:37:19.000000 meta-edc-demo-0.0.2/meta_subject/forms/blood_results/blood_results_glu_form.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      766 2022-09-26 19:37:19.000000 meta-edc-demo-0.0.2/meta_subject/forms/blood_results/blood_results_hba1c_form.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      723 2022-09-26 19:37:19.000000 meta-edc-demo-0.0.2/meta_subject/forms/blood_results/blood_results_ins_form.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      715 2022-10-12 13:06:29.000000 meta-edc-demo-0.0.2/meta_subject/forms/blood_results/blood_results_lft_form.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      731 2022-09-26 19:37:19.000000 meta-edc-demo-0.0.2/meta_subject/forms/blood_results/blood_results_lipid_form.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     1363 2022-09-26 19:37:19.000000 meta-edc-demo-0.0.2/meta_subject/forms/blood_results/blood_results_rft_form.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      486 2022-09-26 19:37:19.000000 meta-edc-demo-0.0.2/meta_subject/forms/complications_glycemia_form.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      490 2022-09-26 19:37:19.000000 meta-edc-demo-0.0.2/meta_subject/forms/concomitant_medication_form.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     3564 2022-09-26 19:37:19.000000 meta-edc-demo-0.0.2/meta_subject/forms/delivery_form.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      974 2022-09-26 19:37:19.000000 meta-edc-demo-0.0.2/meta_subject/forms/egfr_drop_notification_form.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      598 2022-06-24 08:53:52.000000 meta-edc-demo-0.0.2/meta_subject/forms/eq53d3l_form.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     4591 2022-09-26 19:37:19.000000 meta-edc-demo-0.0.2/meta_subject/forms/followup_examination_form.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      430 2022-09-26 19:37:19.000000 meta-edc-demo-0.0.2/meta_subject/forms/followup_vitals_form.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      656 2022-09-26 19:37:19.000000 meta-edc-demo-0.0.2/meta_subject/forms/glucose_form.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      591 2022-09-26 19:37:19.000000 meta-edc-demo-0.0.2/meta_subject/forms/health_economics_simple_form.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      796 2022-09-26 19:37:19.000000 meta-edc-demo-0.0.2/meta_subject/forms/hepatitis_test_form.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      726 2022-09-26 19:37:19.000000 meta-edc-demo-0.0.2/meta_subject/forms/malaria_test_form.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      866 2022-09-26 19:37:19.000000 meta-edc-demo-0.0.2/meta_subject/forms/medication_adherence_form.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     2084 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.2/meta_subject/forms/mixins.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      324 2022-06-24 08:54:40.000000 meta-edc-demo-0.0.2/meta_subject/forms/mnsi_form.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      963 2022-10-10 11:55:19.000000 meta-edc-demo-0.0.2/meta_subject/forms/other_arv_regimens_detail_form.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     1688 2022-09-26 19:37:19.000000 meta-edc-demo-0.0.2/meta_subject/forms/other_arv_regimens_form.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     1809 2022-09-26 19:37:19.000000 meta-edc-demo-0.0.2/meta_subject/forms/patient_history_form.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      788 2022-10-04 20:17:27.000000 meta-edc-demo-0.0.2/meta_subject/forms/physical_exam_form.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      560 2022-09-26 19:37:19.000000 meta-edc-demo-0.0.2/meta_subject/forms/pregnancy_update_form.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      397 2022-06-24 08:54:57.000000 meta-edc-demo-0.0.2/meta_subject/forms/sf12_form.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      822 2022-06-24 08:55:00.000000 meta-edc-demo-0.0.2/meta_subject/forms/slider_widget.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     1574 2022-09-26 19:37:19.000000 meta-edc-demo-0.0.2/meta_subject/forms/study_medication_form.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      954 2022-09-26 19:37:19.000000 meta-edc-demo-0.0.2/meta_subject/forms/subject_requisition_form.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      757 2022-09-26 19:37:19.000000 meta-edc-demo-0.0.2/meta_subject/forms/subject_visit_form.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     2277 2022-09-26 19:37:19.000000 meta-edc-demo-0.0.2/meta_subject/forms/subject_visit_missed_form.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      829 2022-09-26 19:37:19.000000 meta-edc-demo-0.0.2/meta_subject/forms/urine_dipstick_test_form.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     1269 2022-09-26 19:37:19.000000 meta-edc-demo-0.0.2/meta_subject/forms/urine_pregnancy_form.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      325 2022-08-26 02:59:33.000000 meta-edc-demo-0.0.2/meta_subject/identifiers.py
+drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-06-27 06:22:40.325070 meta-edc-demo-0.0.2/meta_subject/metadata_rules/
+-rw-r--r--   0 estellaye   (501) staff       (20)       53 2022-04-11 18:27:09.000000 meta-edc-demo-0.0.2/meta_subject/metadata_rules/__init__.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     3124 2022-08-22 17:23:22.000000 meta-edc-demo-0.0.2/meta_subject/metadata_rules/metadata_rules.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     6795 2022-08-22 17:23:22.000000 meta-edc-demo-0.0.2/meta_subject/metadata_rules/predicates.py
+drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-06-27 06:22:40.359512 meta-edc-demo-0.0.2/meta_subject/migrations/
+-rw-r--r--   0 estellaye   (501) staff       (20)   408933 2022-09-30 02:18:01.000000 meta-edc-demo-0.0.2/meta_subject/migrations/0001_initial.py
+-rw-r--r--   0 estellaye   (501) staff       (20)    29352 2022-08-22 17:23:22.000000 meta-edc-demo-0.0.2/meta_subject/migrations/0002_auto_20191021_0353.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     4025 2020-04-08 01:09:11.000000 meta-edc-demo-0.0.2/meta_subject/migrations/0003_auto_20191021_0534.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      740 2020-04-08 01:09:11.000000 meta-edc-demo-0.0.2/meta_subject/migrations/0004_auto_20191022_0134.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     5819 2021-07-05 19:24:26.000000 meta-edc-demo-0.0.2/meta_subject/migrations/0005_auto_20191024_1000.py
+-rw-r--r--   0 estellaye   (501) staff       (20)    20051 2022-08-22 17:23:22.000000 meta-edc-demo-0.0.2/meta_subject/migrations/0006_auto_20191104_0756.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     1142 2020-04-08 01:09:11.000000 meta-edc-demo-0.0.2/meta_subject/migrations/0007_auto_20191107_2249.py
+-rw-r--r--   0 estellaye   (501) staff       (20)    13944 2020-04-08 01:09:11.000000 meta-edc-demo-0.0.2/meta_subject/migrations/0008_auto_20191115_0132.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     1130 2020-04-08 01:09:11.000000 meta-edc-demo-0.0.2/meta_subject/migrations/0009_auto_20191119_2331.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     6880 2020-04-08 01:09:11.000000 meta-edc-demo-0.0.2/meta_subject/migrations/0010_auto_20191213_0314.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     2780 2022-08-22 17:23:22.000000 meta-edc-demo-0.0.2/meta_subject/migrations/0011_auto_20200118_1854.py
+-rw-r--r--   0 estellaye   (501) staff       (20)    15555 2021-07-05 19:24:26.000000 meta-edc-demo-0.0.2/meta_subject/migrations/0012_auto_20200118_2334.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     1830 2020-04-08 01:09:11.000000 meta-edc-demo-0.0.2/meta_subject/migrations/0013_auto_20200119_0013.py
+-rw-r--r--   0 estellaye   (501) staff       (20)    32039 2022-09-30 02:18:01.000000 meta-edc-demo-0.0.2/meta_subject/migrations/0014_auto_20200120_1622.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      786 2020-04-08 01:09:11.000000 meta-edc-demo-0.0.2/meta_subject/migrations/0015_auto_20200120_1943.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     2036 2020-04-08 01:09:11.000000 meta-edc-demo-0.0.2/meta_subject/migrations/0016_auto_20200123_1508.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     7292 2022-09-30 02:18:01.000000 meta-edc-demo-0.0.2/meta_subject/migrations/0017_auto_20200325_0901.py
+-rw-r--r--   0 estellaye   (501) staff       (20)    59622 2022-08-22 17:23:22.000000 meta-edc-demo-0.0.2/meta_subject/migrations/0018_coronakap_historicalcoronakap.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     1561 2021-07-05 19:24:26.000000 meta-edc-demo-0.0.2/meta_subject/migrations/0019_auto_20200417_0315.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     7014 2021-07-05 19:24:26.000000 meta-edc-demo-0.0.2/meta_subject/migrations/0020_auto_20200417_0329.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     1178 2021-07-05 19:24:26.000000 meta-edc-demo-0.0.2/meta_subject/migrations/0021_auto_20200417_0332.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     5513 2021-08-09 19:25:30.000000 meta-edc-demo-0.0.2/meta_subject/migrations/0022_auto_20200419_2223.py
+-rw-r--r--   0 estellaye   (501) staff       (20)    25416 2020-05-15 02:40:42.000000 meta-edc-demo-0.0.2/meta_subject/migrations/0023_auto_20200419_2305.py
+-rw-r--r--   0 estellaye   (501) staff       (20)    14716 2020-05-15 02:40:42.000000 meta-edc-demo-0.0.2/meta_subject/migrations/0024_auto_20200419_2331.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     7348 2020-05-15 02:40:42.000000 meta-edc-demo-0.0.2/meta_subject/migrations/0025_auto_20200420_1455.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     1092 2020-05-15 02:40:42.000000 meta-edc-demo-0.0.2/meta_subject/migrations/0026_auto_20200420_1524.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     4756 2020-05-15 02:40:42.000000 meta-edc-demo-0.0.2/meta_subject/migrations/0027_auto_20200420_1645.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     6450 2021-07-05 19:24:26.000000 meta-edc-demo-0.0.2/meta_subject/migrations/0028_auto_20200420_1732.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     6004 2020-05-15 02:40:42.000000 meta-edc-demo-0.0.2/meta_subject/migrations/0029_auto_20200420_1751.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     5046 2020-05-15 02:40:42.000000 meta-edc-demo-0.0.2/meta_subject/migrations/0030_auto_20200420_1816.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     4610 2021-07-05 19:24:26.000000 meta-edc-demo-0.0.2/meta_subject/migrations/0031_auto_20200422_2039.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     7736 2021-07-05 19:24:26.000000 meta-edc-demo-0.0.2/meta_subject/migrations/0032_auto_20200515_0307.py
+-rw-r--r--   0 estellaye   (501) staff       (20)    18673 2021-08-09 19:25:30.000000 meta-edc-demo-0.0.2/meta_subject/migrations/0033_auto_20200516_2356.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     1005 2020-05-20 04:57:20.000000 meta-edc-demo-0.0.2/meta_subject/migrations/0034_auto_20200517_0125.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     1317 2021-08-09 19:25:30.000000 meta-edc-demo-0.0.2/meta_subject/migrations/0035_auto_20200517_0128.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     2988 2021-07-05 19:24:26.000000 meta-edc-demo-0.0.2/meta_subject/migrations/0036_auto_20200517_0150.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      588 2020-05-20 04:57:20.000000 meta-edc-demo-0.0.2/meta_subject/migrations/0037_auto_20200517_0207.py
+-rw-r--r--   0 estellaye   (501) staff       (20)    26377 2021-07-05 19:24:26.000000 meta-edc-demo-0.0.2/meta_subject/migrations/0038_auto_20200520_0020.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     6636 2020-06-18 19:11:34.000000 meta-edc-demo-0.0.2/meta_subject/migrations/0039_auto_20200524_1944.py
+-rw-r--r--   0 estellaye   (501) staff       (20)    18300 2021-07-05 19:24:26.000000 meta-edc-demo-0.0.2/meta_subject/migrations/0040_auto_20200527_2155.py
+-rw-r--r--   0 estellaye   (501) staff       (20)    12474 2021-07-05 19:24:26.000000 meta-edc-demo-0.0.2/meta_subject/migrations/0041_auto_20200528_0242.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      224 2020-06-18 19:11:34.000000 meta-edc-demo-0.0.2/meta_subject/migrations/0042_auto_20200528_0252.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     1510 2020-06-18 19:11:34.000000 meta-edc-demo-0.0.2/meta_subject/migrations/0043_auto_20200528_1555.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     2846 2020-06-18 19:11:34.000000 meta-edc-demo-0.0.2/meta_subject/migrations/0044_auto_20200528_1853.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     1245 2021-07-05 19:24:26.000000 meta-edc-demo-0.0.2/meta_subject/migrations/0045_auto_20200530_1801.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     3314 2021-07-05 19:24:26.000000 meta-edc-demo-0.0.2/meta_subject/migrations/0046_auto_20200530_1804.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      590 2022-09-30 02:18:01.000000 meta-edc-demo-0.0.2/meta_subject/migrations/0047_auto_20200530_1819.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      432 2020-06-18 19:11:34.000000 meta-edc-demo-0.0.2/meta_subject/migrations/0048_auto_20200530_1819.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      266 2021-07-05 19:24:26.000000 meta-edc-demo-0.0.2/meta_subject/migrations/0049_auto_20200613_2041.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      877 2021-08-09 19:25:30.000000 meta-edc-demo-0.0.2/meta_subject/migrations/0050_auto_20200614_1934.py
+-rw-r--r--   0 estellaye   (501) staff       (20)    20317 2021-07-05 19:24:26.000000 meta-edc-demo-0.0.2/meta_subject/migrations/0051_auto_20200617_2117.py
+-rw-r--r--   0 estellaye   (501) staff       (20)    40852 2021-07-05 19:24:26.000000 meta-edc-demo-0.0.2/meta_subject/migrations/0052_auto_20210624_0225.py
+-rw-r--r--   0 estellaye   (501) staff       (20)    27485 2022-08-22 17:23:22.000000 meta-edc-demo-0.0.2/meta_subject/migrations/0053_auto_20210628_2105.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     3376 2021-07-05 19:24:26.000000 meta-edc-demo-0.0.2/meta_subject/migrations/0054_auto_20210628_2314.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     2932 2021-07-05 19:24:26.000000 meta-edc-demo-0.0.2/meta_subject/migrations/0055_auto_20210628_2331.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     3544 2021-07-02 03:53:00.000000 meta-edc-demo-0.0.2/meta_subject/migrations/0056_auto_20210702_0426.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     2828 2021-07-05 19:24:26.000000 meta-edc-demo-0.0.2/meta_subject/migrations/0057_auto_20210702_0458.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     1982 2021-07-05 19:24:26.000000 meta-edc-demo-0.0.2/meta_subject/migrations/0058_auto_20210702_0533.py
+-rw-r--r--   0 estellaye   (501) staff       (20)    14818 2022-04-11 18:27:09.000000 meta-edc-demo-0.0.2/meta_subject/migrations/0059_auto_20210709_2056.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     1312 2022-04-11 18:27:09.000000 meta-edc-demo-0.0.2/meta_subject/migrations/0060_auto_20210709_2241.py
+-rw-r--r--   0 estellaye   (501) staff       (20)    36062 2022-04-11 18:27:09.000000 meta-edc-demo-0.0.2/meta_subject/migrations/0061_auto_20210710_1929.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     1008 2022-04-11 18:27:09.000000 meta-edc-demo-0.0.2/meta_subject/migrations/0062_auto_20210713_0616.py
+-rw-r--r--   0 estellaye   (501) staff       (20)    20741 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.2/meta_subject/migrations/0063_auto_20210715_0337.py
+-rw-r--r--   0 estellaye   (501) staff       (20)    31934 2021-08-09 19:25:30.000000 meta-edc-demo-0.0.2/meta_subject/migrations/0064_auto_20210715_2336.py
+-rw-r--r--   0 estellaye   (501) staff       (20)    10394 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.2/meta_subject/migrations/0065_auto_20210716_0813.py
+-rw-r--r--   0 estellaye   (501) staff       (20)    27933 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.2/meta_subject/migrations/0066_auto_20210721_0335.py
+-rw-r--r--   0 estellaye   (501) staff       (20)    47360 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.2/meta_subject/migrations/0067_auto_20210726_0340.py
+-rw-r--r--   0 estellaye   (501) staff       (20)    41023 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.2/meta_subject/migrations/0068_auto_20210728_1809.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     2084 2022-04-11 18:27:09.000000 meta-edc-demo-0.0.2/meta_subject/migrations/0069_auto_20210801_2021.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     2866 2021-08-09 19:25:30.000000 meta-edc-demo-0.0.2/meta_subject/migrations/0070_auto_20210804_0438.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      996 2022-04-11 18:27:09.000000 meta-edc-demo-0.0.2/meta_subject/migrations/0071_auto_20210804_0715.py
+-rw-r--r--   0 estellaye   (501) staff       (20)    25833 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.2/meta_subject/migrations/0072_auto_20210805_1545.py
+-rw-r--r--   0 estellaye   (501) staff       (20)    41645 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.2/meta_subject/migrations/0073_auto_20210809_0055.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      290 2022-04-11 18:27:09.000000 meta-edc-demo-0.0.2/meta_subject/migrations/0074_auto_20210809_1744.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     1997 2021-08-09 19:33:52.000000 meta-edc-demo-0.0.2/meta_subject/migrations/0075_auto_20210809_1744.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      974 2022-04-11 18:27:09.000000 meta-edc-demo-0.0.2/meta_subject/migrations/0076_auto_20210809_1854.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     8021 2022-04-11 18:27:09.000000 meta-edc-demo-0.0.2/meta_subject/migrations/0077_auto_20210809_2323.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     1195 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.2/meta_subject/migrations/0078_auto_20210810_0857.py
+-rw-r--r--   0 estellaye   (501) staff       (20)    35484 2022-04-11 18:27:09.000000 meta-edc-demo-0.0.2/meta_subject/migrations/0079_auto_20210812_0335.py
+-rw-r--r--   0 estellaye   (501) staff       (20)    17308 2022-04-11 18:27:09.000000 meta-edc-demo-0.0.2/meta_subject/migrations/0080_auto_20210812_0400.py
+-rw-r--r--   0 estellaye   (501) staff       (20)    27696 2022-04-11 18:27:09.000000 meta-edc-demo-0.0.2/meta_subject/migrations/0081_auto_20210817_2306.py
+-rw-r--r--   0 estellaye   (501) staff       (20)    12294 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.2/meta_subject/migrations/0082_auto_20210823_1612.py
+-rw-r--r--   0 estellaye   (501) staff       (20)    14439 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.2/meta_subject/migrations/0083_auto_20210823_1620.py
+-rw-r--r--   0 estellaye   (501) staff       (20)    15219 2022-04-11 18:27:09.000000 meta-edc-demo-0.0.2/meta_subject/migrations/0084_auto_20210910_0234.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     2962 2022-04-11 18:27:09.000000 meta-edc-demo-0.0.2/meta_subject/migrations/0085_auto_20210911_2036.py
+-rw-r--r--   0 estellaye   (501) staff       (20)    15645 2022-04-11 18:27:09.000000 meta-edc-demo-0.0.2/meta_subject/migrations/0086_auto_20210920_0229.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     2918 2022-04-11 18:27:09.000000 meta-edc-demo-0.0.2/meta_subject/migrations/0087_auto_20210922_2058.py
+-rw-r--r--   0 estellaye   (501) staff       (20)    28869 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.2/meta_subject/migrations/0088_auto_20210924_0027.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     6594 2022-04-11 18:27:09.000000 meta-edc-demo-0.0.2/meta_subject/migrations/0089_auto_20210924_0121.py
+-rw-r--r--   0 estellaye   (501) staff       (20)    15972 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.2/meta_subject/migrations/0090_auto_20210924_0424.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     1876 2022-06-24 08:50:42.000000 meta-edc-demo-0.0.2/meta_subject/migrations/0091_auto_20210929_2324.py
+-rw-r--r--   0 estellaye   (501) staff       (20)    16400 2022-06-24 08:50:40.000000 meta-edc-demo-0.0.2/meta_subject/migrations/0092_auto_20211013_0447.py
+-rw-r--r--   0 estellaye   (501) staff       (20)    33888 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.2/meta_subject/migrations/0093_auto_20211117_0352.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     4812 2022-06-24 08:50:38.000000 meta-edc-demo-0.0.2/meta_subject/migrations/0094_auto_20211123_1645.py
+-rw-r--r--   0 estellaye   (501) staff       (20)    22479 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.2/meta_subject/migrations/0095_auto_20220128_1719.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     3419 2022-04-11 18:27:09.000000 meta-edc-demo-0.0.2/meta_subject/migrations/0096_auto_20220304_0501.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     2100 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.2/meta_subject/migrations/0097_auto_20220304_2233.py
+-rw-r--r--   0 estellaye   (501) staff       (20)    21283 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.2/meta_subject/migrations/0098_auto_20220309_2106.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     1909 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.2/meta_subject/migrations/0099_auto_20220309_2218.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     1091 2022-06-24 08:50:29.000000 meta-edc-demo-0.0.2/meta_subject/migrations/0100_auto_20220309_2238.py
+-rw-r--r--   0 estellaye   (501) staff       (20)    61584 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.2/meta_subject/migrations/0101_auto_20220316_2147.py
+-rw-r--r--   0 estellaye   (501) staff       (20)    15291 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.2/meta_subject/migrations/0102_auto_20220324_0304.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      869 2022-06-24 08:50:27.000000 meta-edc-demo-0.0.2/meta_subject/migrations/0103_auto_20220324_0326.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      967 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.2/meta_subject/migrations/0104_auto_20220412_2151.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     1291 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.2/meta_subject/migrations/0105_auto_20220412_2310.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      773 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.2/meta_subject/migrations/0106_auto_20220414_1741.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     1493 2022-10-11 02:21:31.000000 meta-edc-demo-0.0.2/meta_subject/migrations/0107_auto_20220415_0043.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      689 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.2/meta_subject/migrations/0108_auto_20220415_1747.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      557 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.2/meta_subject/migrations/0109_auto_20220415_1758.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     2517 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.2/meta_subject/migrations/0110_auto_20220512_1811.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     3011 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.2/meta_subject/migrations/0111_alter_followupvitals_severe_htn_and_more.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     1036 2022-08-22 17:23:22.000000 meta-edc-demo-0.0.2/meta_subject/migrations/0112_historicalsubjectvisit_document_status_comments_and_more.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      720 2022-08-22 17:23:22.000000 meta-edc-demo-0.0.2/meta_subject/migrations/0113_bloodresultsrft_egfr_percent_change_and_more.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      992 2022-08-22 17:23:22.000000 meta-edc-demo-0.0.2/meta_subject/migrations/0114_alter_bloodresultsrft_egfr_percent_change_and_more.py
+-rw-r--r--   0 estellaye   (501) staff       (20)    18447 2022-08-22 17:23:22.000000 meta-edc-demo-0.0.2/meta_subject/migrations/0115_historicalegfrnotification_egfrnotification.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     1177 2022-08-22 17:23:22.000000 meta-edc-demo-0.0.2/meta_subject/migrations/0116_egfrnotification_report_status_and_more.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     3279 2022-08-22 17:23:22.000000 meta-edc-demo-0.0.2/meta_subject/migrations/0117_alter_egfrnotification_managers_and_more.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     2050 2022-08-22 17:23:22.000000 meta-edc-demo-0.0.2/meta_subject/migrations/0118_delivery_crf_status_delivery_crf_status_comments_and_more.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      635 2022-08-22 17:23:22.000000 meta-edc-demo-0.0.2/meta_subject/migrations/0119_historicalstudymedication_roundup_divisible_by_and_more.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     2888 2022-08-22 17:23:22.000000 meta-edc-demo-0.0.2/meta_subject/migrations/0120_alter_birthoutcomes_managers_and_more.py
+-rw-r--r--   0 estellaye   (501) staff       (20)    21741 2022-08-22 17:23:22.000000 meta-edc-demo-0.0.2/meta_subject/migrations/0121_auto_20220704_1841.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      813 2022-07-14 12:01:13.000000 meta-edc-demo-0.0.2/meta_subject/migrations/0122_auto_20220708_2144.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     8263 2022-08-22 17:23:22.000000 meta-edc-demo-0.0.2/meta_subject/migrations/0123_auto_20220714_2136.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     1207 2022-07-19 13:21:21.000000 meta-edc-demo-0.0.2/meta_subject/migrations/0124_auto_20220714_2303.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     1569 2022-08-22 17:23:22.000000 meta-edc-demo-0.0.2/meta_subject/migrations/0125_auto_20220719_2134.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      777 2022-08-22 17:23:22.000000 meta-edc-demo-0.0.2/meta_subject/migrations/0126_auto_20220719_2142.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     5489 2022-08-22 17:23:22.000000 meta-edc-demo-0.0.2/meta_subject/migrations/0127_auto_20220720_0053.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      779 2022-08-22 17:23:22.000000 meta-edc-demo-0.0.2/meta_subject/migrations/0128_auto_20220720_0055.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      491 2022-08-22 17:23:22.000000 meta-edc-demo-0.0.2/meta_subject/migrations/0129_auto_20220720_0108.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      684 2022-08-22 17:23:22.000000 meta-edc-demo-0.0.2/meta_subject/migrations/0130_auto_20220720_0216.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     1933 2022-08-22 17:23:22.000000 meta-edc-demo-0.0.2/meta_subject/migrations/0131_auto_20220722_0411.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      844 2022-08-22 17:23:22.000000 meta-edc-demo-0.0.2/meta_subject/migrations/0132_auto_20220722_1825.py
+-rw-r--r--   0 estellaye   (501) staff       (20)    28131 2022-08-22 17:23:22.000000 meta-edc-demo-0.0.2/meta_subject/migrations/0133_auto_20220722_2140.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     1807 2022-08-22 17:23:22.000000 meta-edc-demo-0.0.2/meta_subject/migrations/0134_auto_20220722_2211.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     2264 2022-08-23 13:24:02.000000 meta-edc-demo-0.0.2/meta_subject/migrations/0135_auto_20220722_2212.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     8661 2022-08-22 17:23:22.000000 meta-edc-demo-0.0.2/meta_subject/migrations/0136_egfrdropnotification_creatinine_quantifier_and_more.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     1139 2022-08-22 17:23:22.000000 meta-edc-demo-0.0.2/meta_subject/migrations/0137_alter_egfrdropnotification_egfr_percent_change_and_more.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     3532 2022-08-22 17:23:22.000000 meta-edc-demo-0.0.2/meta_subject/migrations/0138_alter_glucose_fbg_datetime_and_more.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      939 2022-08-23 13:24:02.000000 meta-edc-demo-0.0.2/meta_subject/migrations/0139_alter_bloodresultsins_ins_units_and_more.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     4342 2022-08-23 13:31:01.000000 meta-edc-demo-0.0.2/meta_subject/migrations/0140_alter_bloodresultsfbc_action_identifier_and_more.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     4571 2022-08-26 02:59:33.000000 meta-edc-demo-0.0.2/meta_subject/migrations/0141_auto_20220826_0258.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     5197 2022-08-26 02:59:33.000000 meta-edc-demo-0.0.2/meta_subject/migrations/0142_auto_20220826_0322.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     3811 2022-08-26 02:59:33.000000 meta-edc-demo-0.0.2/meta_subject/migrations/0143_auto_20220826_0406.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      965 2022-09-08 15:51:35.000000 meta-edc-demo-0.0.2/meta_subject/migrations/0144_auto_20220907_0157.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     1786 2022-09-08 15:51:35.000000 meta-edc-demo-0.0.2/meta_subject/migrations/0145_auto_20220907_0202.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      619 2022-09-08 15:51:35.000000 meta-edc-demo-0.0.2/meta_subject/migrations/0146_auto_20220907_0207.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     1907 2022-09-08 21:41:58.000000 meta-edc-demo-0.0.2/meta_subject/migrations/0147_auto_20220907_1505.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     1815 2022-09-08 15:51:35.000000 meta-edc-demo-0.0.2/meta_subject/migrations/0148_auto_20220908_1826.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     1001 2022-09-15 02:57:38.000000 meta-edc-demo-0.0.2/meta_subject/migrations/0149_auto_20220913_2139.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     1224 2022-09-15 02:57:38.000000 meta-edc-demo-0.0.2/meta_subject/migrations/0150_auto_20220914_0039.py
+-rw-r--r--   0 estellaye   (501) staff       (20)    52999 2022-09-26 19:37:19.000000 meta-edc-demo-0.0.2/meta_subject/migrations/0151_auto_20220918_0508.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      739 2022-09-26 19:37:19.000000 meta-edc-demo-0.0.2/meta_subject/migrations/0152_auto_20220925_0509.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     1173 2022-09-28 03:19:11.000000 meta-edc-demo-0.0.2/meta_subject/migrations/0153_auto_20220928_0250.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     1011 2022-09-28 03:19:11.000000 meta-edc-demo-0.0.2/meta_subject/migrations/0154_auto_20220928_0419.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     9272 2022-09-30 02:18:01.000000 meta-edc-demo-0.0.2/meta_subject/migrations/0155_auto_20220929_1742.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     5445 2022-10-05 21:55:17.000000 meta-edc-demo-0.0.2/meta_subject/migrations/0156_alter_bloodresultsfbc_assay_datetime_and_more.py
+-rw-r--r--   0 estellaye   (501) staff       (20)        0 2020-03-15 03:34:20.000000 meta-edc-demo-0.0.2/meta_subject/migrations/__init__.py
+drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-06-27 06:22:40.360629 meta-edc-demo-0.0.2/meta_subject/model_mixins/
+-rw-r--r--   0 estellaye   (501) staff       (20)      286 2022-09-26 19:37:19.000000 meta-edc-demo-0.0.2/meta_subject/model_mixins/__init__.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     2904 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.2/meta_subject/model_mixins/arv_history_model_mixin.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      248 2022-09-26 19:37:19.000000 meta-edc-demo-0.0.2/meta_subject/model_mixins/crf_model_mixin.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      298 2022-09-26 19:37:19.000000 meta-edc-demo-0.0.2/meta_subject/model_mixins/crf_with_action_model_mixin.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      296 2022-06-24 08:52:03.000000 meta-edc-demo-0.0.2/meta_subject/model_mixins/search_slug_model_mixin.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     1161 2022-06-24 08:49:55.000000 meta-edc-demo-0.0.2/meta_subject/model_mixins/vitals_fields_model_mixin.py
+drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-06-27 06:22:40.366856 meta-edc-demo-0.0.2/meta_subject/models/
+-rw-r--r--   0 estellaye   (501) staff       (20)     1643 2022-08-23 01:10:14.000000 meta-edc-demo-0.0.2/meta_subject/models/__init__.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     2879 2022-09-30 02:18:01.000000 meta-edc-demo-0.0.2/meta_subject/models/birth_outcomes.py
+drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-06-27 06:22:40.368201 meta-edc-demo-0.0.2/meta_subject/models/blood_results/
+-rw-r--r--   0 estellaye   (501) staff       (20)      337 2021-08-09 19:25:30.000000 meta-edc-demo-0.0.2/meta_subject/models/blood_results/__init__.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     1068 2022-09-26 19:37:19.000000 meta-edc-demo-0.0.2/meta_subject/models/blood_results/blood_results_fbc.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      818 2022-09-26 19:37:19.000000 meta-edc-demo-0.0.2/meta_subject/models/blood_results/blood_results_glu.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      776 2022-09-26 19:37:19.000000 meta-edc-demo-0.0.2/meta_subject/models/blood_results/blood_results_hba1c.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      790 2022-09-26 19:37:19.000000 meta-edc-demo-0.0.2/meta_subject/models/blood_results/blood_results_ins.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      977 2022-09-26 19:37:19.000000 meta-edc-demo-0.0.2/meta_subject/models/blood_results/blood_results_lft.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      907 2022-09-26 19:37:19.000000 meta-edc-demo-0.0.2/meta_subject/models/blood_results/blood_results_lipid.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     1417 2022-09-26 19:37:19.000000 meta-edc-demo-0.0.2/meta_subject/models/blood_results/blood_results_rft.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     1952 2022-08-22 17:23:22.000000 meta-edc-demo-0.0.2/meta_subject/models/complications.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     6079 2022-06-24 08:51:45.000000 meta-edc-demo-0.0.2/meta_subject/models/complications_glycemia.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      369 2022-09-26 19:37:19.000000 meta-edc-demo-0.0.2/meta_subject/models/concomitant_medication.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     5100 2022-09-29 13:40:10.000000 meta-edc-demo-0.0.2/meta_subject/models/delivery.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     1085 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.2/meta_subject/models/diet_and_lifestyle.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      558 2022-09-26 19:37:19.000000 meta-edc-demo-0.0.2/meta_subject/models/egfr_drop_notification.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      291 2022-09-26 19:37:19.000000 meta-edc-demo-0.0.2/meta_subject/models/eq5d3l.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     8075 2022-09-26 19:37:19.000000 meta-edc-demo-0.0.2/meta_subject/models/followup_examination.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      926 2022-06-24 08:51:51.000000 meta-edc-demo-0.0.2/meta_subject/models/followup_vitals.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     1314 2022-08-23 01:10:08.000000 meta-edc-demo-0.0.2/meta_subject/models/glucose.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     9736 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.2/meta_subject/models/health_economics.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      741 2022-09-26 19:37:19.000000 meta-edc-demo-0.0.2/meta_subject/models/health_economics_simple.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     1851 2022-08-22 17:23:22.000000 meta-edc-demo-0.0.2/meta_subject/models/hepatitis_test.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     1038 2022-09-26 19:37:19.000000 meta-edc-demo-0.0.2/meta_subject/models/malaria_test.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      399 2022-09-26 19:37:19.000000 meta-edc-demo-0.0.2/meta_subject/models/medication_adherence.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      284 2022-09-26 19:37:19.000000 meta-edc-demo-0.0.2/meta_subject/models/mnsi.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      707 2022-09-26 19:37:19.000000 meta-edc-demo-0.0.2/meta_subject/models/off_study_drug.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      607 2022-10-05 23:57:35.000000 meta-edc-demo-0.0.2/meta_subject/models/other_arv_regimens.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     1828 2022-09-26 19:37:19.000000 meta-edc-demo-0.0.2/meta_subject/models/other_arv_regimens_detail.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     4511 2022-09-26 19:37:19.000000 meta-edc-demo-0.0.2/meta_subject/models/patient_history.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     1994 2022-08-22 17:23:22.000000 meta-edc-demo-0.0.2/meta_subject/models/physical_exam.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      950 2022-09-26 19:37:19.000000 meta-edc-demo-0.0.2/meta_subject/models/pregnancy_update.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      345 2022-09-26 19:37:19.000000 meta-edc-demo-0.0.2/meta_subject/models/sf12.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     3989 2022-07-08 07:31:04.000000 meta-edc-demo-0.0.2/meta_subject/models/signals.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      462 2022-09-26 19:37:19.000000 meta-edc-demo-0.0.2/meta_subject/models/study_medication.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      422 2022-09-26 19:37:19.000000 meta-edc-demo-0.0.2/meta_subject/models/subject_requisition.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     2324 2022-10-13 03:34:11.000000 meta-edc-demo-0.0.2/meta_subject/models/subject_visit.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      748 2022-09-26 19:37:19.000000 meta-edc-demo-0.0.2/meta_subject/models/subject_visit_missed.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     1179 2022-06-24 08:49:07.000000 meta-edc-demo-0.0.2/meta_subject/models/urine_dipstick_test.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     1337 2022-09-26 19:37:19.000000 meta-edc-demo-0.0.2/meta_subject/models/urine_pregnancy.py
+drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-06-27 06:22:40.368496 meta-edc-demo-0.0.2/meta_subject/tests/
+-rw-r--r--   0 estellaye   (501) staff       (20)        0 2020-03-15 03:34:20.000000 meta-edc-demo-0.0.2/meta_subject/tests/__init__.py
+drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-06-27 06:22:40.370395 meta-edc-demo-0.0.2/meta_subject/tests/tests/
+-rw-r--r--   0 estellaye   (501) staff       (20)        0 2021-08-09 19:25:30.000000 meta-edc-demo-0.0.2/meta_subject/tests/tests/__init__.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     9294 2022-09-27 03:17:01.000000 meta-edc-demo-0.0.2/meta_subject/tests/tests/test_egfr.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     1760 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.2/meta_subject/tests/tests/test_followup.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     1376 2022-10-04 03:17:15.000000 meta-edc-demo-0.0.2/meta_subject/tests/tests/test_manager_order.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     2383 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.2/meta_subject/tests/tests/test_medication_adherence.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     4445 2022-08-22 17:23:22.000000 meta-edc-demo-0.0.2/meta_subject/tests/tests/test_metadata_rules.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     9809 2022-06-24 08:51:22.000000 meta-edc-demo-0.0.2/meta_subject/tests/tests/test_mnsi.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     2690 2022-09-26 19:37:19.000000 meta-edc-demo-0.0.2/meta_subject/tests/tests/test_patient_history_form.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     2810 2022-09-26 19:37:19.000000 meta-edc-demo-0.0.2/meta_subject/tests/tests/test_physical_exam.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     6926 2022-09-26 19:37:19.000000 meta-edc-demo-0.0.2/meta_subject/tests/tests/test_sf12.py
+-rw-r--r--   0 estellaye   (501) staff       (20)    10161 2022-09-28 03:19:11.000000 meta-edc-demo-0.0.2/meta_subject/tests/tests/test_study_medication.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     1168 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.2/meta_subject/tests/urls.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      206 2022-06-24 09:02:28.000000 meta-edc-demo-0.0.2/meta_subject/urls.py
+drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-06-27 06:22:40.371141 meta-edc-demo-0.0.2/meta_visit_schedule/
+-rw-r--r--   0 estellaye   (501) staff       (20)        0 2021-07-07 23:18:25.000000 meta-edc-demo-0.0.2/meta_visit_schedule/__init__.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      164 2021-07-02 03:53:00.000000 meta-edc-demo-0.0.2/meta_visit_schedule/apps.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      423 2022-04-11 18:27:09.000000 meta-edc-demo-0.0.2/meta_visit_schedule/constants.py
+drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-06-27 06:22:40.371282 meta-edc-demo-0.0.2/meta_visit_schedule/migrations/
+-rw-r--r--   0 estellaye   (501) staff       (20)        0 2020-03-15 03:34:20.000000 meta-edc-demo-0.0.2/meta_visit_schedule/migrations/__init__.py
+-rw-r--r--   0 estellaye   (501) staff       (20)        0 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.2/meta_visit_schedule/models.py
+drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-06-27 06:22:40.371552 meta-edc-demo-0.0.2/meta_visit_schedule/tests/
+-rw-r--r--   0 estellaye   (501) staff       (20)        0 2020-03-15 03:34:20.000000 meta-edc-demo-0.0.2/meta_visit_schedule/tests/__init__.py
+drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-06-27 06:22:40.371879 meta-edc-demo-0.0.2/meta_visit_schedule/tests/tests/
+-rw-r--r--   0 estellaye   (501) staff       (20)        0 2021-08-09 19:25:30.000000 meta-edc-demo-0.0.2/meta_visit_schedule/tests/tests/__init__.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     7206 2022-07-08 07:31:04.000000 meta-edc-demo-0.0.2/meta_visit_schedule/tests/tests/test_schedule.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      111 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.2/meta_visit_schedule/tests/urls.py
+drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-06-27 06:22:40.372066 meta-edc-demo-0.0.2/meta_visit_schedule/visit_schedules/
+-rw-r--r--   0 estellaye   (501) staff       (20)      318 2022-04-11 18:27:09.000000 meta-edc-demo-0.0.2/meta_visit_schedule/visit_schedules/__init__.py
+drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-06-27 06:22:40.373337 meta-edc-demo-0.0.2/meta_visit_schedule/visit_schedules/phase_three/
+-rw-r--r--   0 estellaye   (501) staff       (20)       74 2022-04-11 18:27:09.000000 meta-edc-demo-0.0.2/meta_visit_schedule/visit_schedules/phase_three/__init__.py
+-rw-r--r--   0 estellaye   (501) staff       (20)    11160 2022-08-23 01:12:29.000000 meta-edc-demo-0.0.2/meta_visit_schedule/visit_schedules/phase_three/crfs.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      167 2022-06-24 08:46:02.000000 meta-edc-demo-0.0.2/meta_visit_schedule/visit_schedules/phase_three/crfs_pregnancy.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     5400 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.2/meta_visit_schedule/visit_schedules/phase_three/requisitions.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     6831 2022-09-26 19:37:19.000000 meta-edc-demo-0.0.2/meta_visit_schedule/visit_schedules/phase_three/schedule.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     1043 2022-08-22 17:23:22.000000 meta-edc-demo-0.0.2/meta_visit_schedule/visit_schedules/phase_three/schedule_pregnancy.py
+-rw-r--r--   0 estellaye   (501) staff       (20)      522 2022-07-08 07:31:04.000000 meta-edc-demo-0.0.2/meta_visit_schedule/visit_schedules/phase_three/visit_schedule.py
+-rw-r--r--   0 estellaye   (501) staff       (20)     1990 2022-06-29 19:36:30.000000 meta-edc-demo-0.0.2/pyproject.toml
+-rw-r--r--   0 estellaye   (501) staff       (20)     1213 2023-06-27 06:22:40.374225 meta-edc-demo-0.0.2/setup.cfg
+-rw-r--r--   0 estellaye   (501) staff       (20)      642 2023-06-27 06:22:29.000000 meta-edc-demo-0.0.2/setup.py
+drwxr-xr-x   0 estellaye   (501) staff       (20)        0 2023-06-27 06:22:40.373494 meta-edc-demo-0.0.2/tests/
+-rw-r--r--   0 estellaye   (501) staff       (20)        0 2020-03-15 03:34:20.000000 meta-edc-demo-0.0.2/tests/__init__.py
```

### Comparing `meta-edc-demo-0.0.1/CHANGES` & `meta-edc-demo-0.0.2/CHANGES`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/LICENSE` & `meta-edc-demo-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/PKG-INFO` & `meta-edc-demo-0.0.2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meta-edc-demo
-Version: 0.0.1
+Version: 0.0.2
 Summary: Testing META Trial EDC (http://www.isrctn.com/ISRCTN76157257)
 Home-page: https://github.com/meta-trial/meta-edc
 Author: Erik van Widenfelt
 Author-email: ew2789@gmail.com
 License: GPL license, see LICENSE
 Keywords: django edc META EDC,clinicedc,clinical trials
 Classifier: Programming Language :: Python :: 3
```

### Comparing `meta-edc-demo-0.0.1/README.rst` & `meta-edc-demo-0.0.2/README.rst`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/TODO.txt` & `meta-edc-demo-0.0.2/TODO.txt`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/label_templates/2.25x1.25in/aliquot.lbl` & `meta-edc-demo-0.0.2/label_templates/2.25x1.25in/aliquot.lbl`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/label_templates/2.25x1.25in/requisition.lbl` & `meta-edc-demo-0.0.2/label_templates/2.25x1.25in/requisition.lbl`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_ae/action_items.py` & `meta-edc-demo-0.0.2/meta_ae/action_items.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_ae/admin/ae_initial_admin.py` & `meta-edc-demo-0.0.2/meta_ae/admin/ae_initial_admin.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_ae/admin/death_report_admin.py` & `meta-edc-demo-0.0.2/meta_ae/admin/death_report_admin.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_ae/admin/modeladmin_mixins.py` & `meta-edc-demo-0.0.2/meta_ae/admin/modeladmin_mixins.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_ae/baker_recipes.py` & `meta-edc-demo-0.0.2/meta_ae/baker_recipes.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_ae/choices.py` & `meta-edc-demo-0.0.2/meta_ae/choices.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_ae/forms/death_report_form.py` & `meta-edc-demo-0.0.2/meta_ae/forms/death_report_form.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_ae/forms/modelform_mixins.py` & `meta-edc-demo-0.0.2/meta_ae/forms/modelform_mixins.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_ae/list_data.py` & `meta-edc-demo-0.0.2/meta_ae/list_data.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_ae/migrations/0001_initial.py` & `meta-edc-demo-0.0.2/meta_ae/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_ae/migrations/0002_auto_20191024_1000.py` & `meta-edc-demo-0.0.2/meta_ae/migrations/0002_auto_20191024_1000.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_ae/migrations/0003_auto_20191102_0033.py` & `meta-edc-demo-0.0.2/meta_ae/migrations/0003_auto_20191102_0033.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_ae/migrations/0004_auto_20191114_0821.py` & `meta-edc-demo-0.0.2/meta_ae/migrations/0004_auto_20191114_0821.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_ae/migrations/0005_auto_20210624_0225.py` & `meta-edc-demo-0.0.2/meta_ae/migrations/0005_auto_20210624_0225.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_ae/migrations/0006_aelocalreview_aesponsorreview.py` & `meta-edc-demo-0.0.2/meta_ae/migrations/0006_aelocalreview_aesponsorreview.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_ae/migrations/0007_auto_20210911_2036.py` & `meta-edc-demo-0.0.2/meta_ae/migrations/0007_auto_20210911_2036.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_ae/migrations/0008_auto_20211011_1657.py` & `meta-edc-demo-0.0.2/meta_ae/migrations/0008_auto_20211011_1657.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_ae/migrations/0009_auto_20220307_1929.py` & `meta-edc-demo-0.0.2/meta_ae/migrations/0009_auto_20220307_1929.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_ae/migrations/0010_auto_20220704_1841.py` & `meta-edc-demo-0.0.2/meta_ae/migrations/0010_auto_20220704_1841.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_ae/migrations/0011_alter_aefollowup_action_identifier_and_more.py` & `meta-edc-demo-0.0.2/meta_ae/migrations/0011_alter_aefollowup_action_identifier_and_more.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_ae/migrations/0012_auto_20220826_0258.py` & `meta-edc-demo-0.0.2/meta_ae/migrations/0012_auto_20220826_0258.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_ae/migrations/0013_auto_20220826_0322.py` & `meta-edc-demo-0.0.2/meta_ae/migrations/0013_auto_20220826_0322.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_ae/migrations/0014_auto_20220826_0406.py` & `meta-edc-demo-0.0.2/meta_ae/migrations/0014_auto_20220826_0406.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_ae/migrations/0015_auto_20220907_0157.py` & `meta-edc-demo-0.0.2/meta_ae/migrations/0015_auto_20220907_0157.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_ae/model_mixins/ae_review_model_mixin.py` & `meta-edc-demo-0.0.2/meta_ae/model_mixins/ae_review_model_mixin.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_ae/model_mixins/death_report_model_mixin.py` & `meta-edc-demo-0.0.2/meta_ae/model_mixins/death_report_model_mixin.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_ae/models/death_report_tmg_second.py` & `meta-edc-demo-0.0.2/meta_ae/models/death_report_tmg_second.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_ae/models/managers.py` & `meta-edc-demo-0.0.2/meta_ae/models/managers.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_ae/pdf_reports/meta_pdf_report_mixin.py` & `meta-edc-demo-0.0.2/meta_ae/pdf_reports/meta_pdf_report_mixin.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_ae/templatetags/meta_ae_extras.py` & `meta-edc-demo-0.0.2/meta_ae/templatetags/meta_ae_extras.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_ae/tests/tests/test_actions.py` & `meta-edc-demo-0.0.2/meta_ae/tests/tests/test_actions.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_auth/auth_objects.py` & `meta-edc-demo-0.0.2/meta_auth/auth_objects.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_auth/auths.py` & `meta-edc-demo-0.0.2/meta_auth/auths.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_consent/action_items.py` & `meta-edc-demo-0.0.2/meta_consent/action_items.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_consent/admin/actions/create_missing_prescriptions.py` & `meta-edc-demo-0.0.2/meta_consent/admin/actions/create_missing_prescriptions.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_consent/admin/subject_consent_admin.py` & `meta-edc-demo-0.0.2/meta_consent/admin/subject_consent_admin.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_consent/admin/subject_reconsent_admin.py` & `meta-edc-demo-0.0.2/meta_consent/admin/subject_reconsent_admin.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_consent/baker_recipes.py` & `meta-edc-demo-0.0.2/meta_consent/baker_recipes.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_consent/forms/subject_consent_form.py` & `meta-edc-demo-0.0.2/meta_consent/forms/subject_consent_form.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_consent/forms/subject_reconsent_form.py` & `meta-edc-demo-0.0.2/meta_consent/forms/subject_reconsent_form.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_consent/management/commands/create_missing_prescriptions.py` & `meta-edc-demo-0.0.2/meta_consent/management/commands/create_missing_prescriptions.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_consent/migrations/0001_initial.py` & `meta-edc-demo-0.0.2/meta_consent/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_consent/migrations/0002_auto_20191024_1000.py` & `meta-edc-demo-0.0.2/meta_consent/migrations/0002_auto_20191024_1000.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_consent/migrations/0003_auto_20200325_0901.py` & `meta-edc-demo-0.0.2/meta_consent/migrations/0003_auto_20200325_0901.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_consent/migrations/0004_auto_20210624_0225.py` & `meta-edc-demo-0.0.2/meta_consent/migrations/0004_auto_20210624_0225.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_consent/migrations/0005_alter_subjectconsent_options.py` & `meta-edc-demo-0.0.2/meta_consent/migrations/0005_alter_subjectconsent_options.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_consent/migrations/0006_auto_20210911_2036.py` & `meta-edc-demo-0.0.2/meta_consent/migrations/0006_auto_20210911_2036.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_consent/migrations/0007_auto_20220128_1719.py` & `meta-edc-demo-0.0.2/meta_consent/migrations/0007_auto_20220128_1719.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_consent/migrations/0008_auto_20220412_2151.py` & `meta-edc-demo-0.0.2/meta_consent/migrations/0008_auto_20220412_2151.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_consent/migrations/0009_auto_20220704_1841.py` & `meta-edc-demo-0.0.2/meta_consent/migrations/0009_auto_20220704_1841.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_consent/migrations/0010_alter_historicalsubjectreconsent_action_identifier_and_more.py` & `meta-edc-demo-0.0.2/meta_consent/migrations/0010_alter_historicalsubjectreconsent_action_identifier_and_more.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_consent/migrations/0011_auto_20220826_0258.py` & `meta-edc-demo-0.0.2/meta_consent/migrations/0011_auto_20220826_0258.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_consent/migrations/0012_auto_20220826_0322.py` & `meta-edc-demo-0.0.2/meta_consent/migrations/0012_auto_20220826_0322.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_consent/migrations/0014_alter_subjectconsent_managers.py` & `meta-edc-demo-0.0.2/meta_consent/migrations/0014_alter_subjectconsent_managers.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_consent/migrations/0015_auto_20220914_0542.py` & `meta-edc-demo-0.0.2/meta_consent/migrations/0015_auto_20220914_0542.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_consent/migrations/0016_auto_20220914_0547.py` & `meta-edc-demo-0.0.2/meta_consent/migrations/0016_auto_20220914_0547.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_consent/migrations/0017_auto_20220929_1742.py` & `meta-edc-demo-0.0.2/meta_consent/migrations/0017_auto_20220929_1742.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_consent/models/signals.py` & `meta-edc-demo-0.0.2/meta_consent/models/signals.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_consent/models/subject_consent.py` & `meta-edc-demo-0.0.2/meta_consent/models/subject_consent.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_consent/models/subject_reconsent.py` & `meta-edc-demo-0.0.2/meta_consent/models/subject_reconsent.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_consent/tests/tests/test_form_validators.py` & `meta-edc-demo-0.0.2/meta_consent/tests/tests/test_form_validators.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_consent/tests/urls.py` & `meta-edc-demo-0.0.2/meta_consent/tests/urls.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_dashboard/apps.py` & `meta-edc-demo-0.0.2/meta_dashboard/apps.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_dashboard/model_wrappers/subject_screening_model_wrapper.py` & `meta-edc-demo-0.0.2/meta_dashboard/model_wrappers/subject_screening_model_wrapper.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_dashboard/navbars.py` & `meta-edc-demo-0.0.2/meta_dashboard/navbars.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_dashboard/templatetags/meta_dashboard_extras.py` & `meta-edc-demo-0.0.2/meta_dashboard/templatetags/meta_dashboard_extras.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_dashboard/tests/admin.py` & `meta-edc-demo-0.0.2/meta_dashboard/tests/admin.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_dashboard/tests/tests/test_model_wrappers.py` & `meta-edc-demo-0.0.2/meta_dashboard/tests/tests/test_model_wrappers.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_dashboard/tests/urls.py` & `meta-edc-demo-0.0.2/meta_dashboard/tests/urls.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_dashboard/urls.py` & `meta-edc-demo-0.0.2/meta_dashboard/urls.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_dashboard/views/screening/listboard_view.py` & `meta-edc-demo-0.0.2/meta_dashboard/views/screening/listboard_view.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_dashboard/views/subject/listboard/listboard_view.py` & `meta-edc-demo-0.0.2/meta_dashboard/views/subject/listboard/listboard_view.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_data_manager/handlers.py` & `meta-edc-demo-0.0.2/meta_data_manager/handlers.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_edc/admin.py` & `meta-edc-demo-0.0.2/meta_edc/admin.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_edc/celery.py` & `meta-edc-demo-0.0.2/meta_edc/celery.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_edc/management/commands/update_forms_reference.py` & `meta-edc-demo-0.0.2/meta_edc/management/commands/update_forms_reference.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_edc/model_callers.py` & `meta-edc-demo-0.0.2/meta_edc/model_callers.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_edc/navbars.py` & `meta-edc-demo-0.0.2/meta_edc/navbars.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_edc/settings/debug.py` & `meta-edc-demo-0.0.2/meta_edc/settings/debug.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,24 +5,23 @@
 from .defaults import *  # noqa
 
 print(f"Settings file {__file__}")  # noqa
 
 SITE_ID = SiteID(default=30)
 EDC_SITES_UAT_DOMAIN = False
 DEBUG = True
-#ALLOWED_HOSTS = [
-#    "localhost",
-#    "mnazi-moja.tz.meta3.clinicedc.org",
-#    "mbagala.tz.meta3.clinicedc.org",
-#    "mwananyamala.tz.meta3.clinicedc.org",
-#    "hindu-mandal.tz.meta3.clinicedc.org",
-#    "temeke.tz.meta3.clinicedc.org",
-#    "amana.tz.meta3.clinicedc.org",
-#]
-ALLOWED_HOSTS = ["*"]
+ALLOWED_HOSTS = [
+    "localhost",
+    "mnazi-moja.tz.meta3.clinicedc.org",
+    "mbagala.tz.meta3.clinicedc.org",
+    "mwananyamala.tz.meta3.clinicedc.org",
+    "hindu-mandal.tz.meta3.clinicedc.org",
+    "temeke.tz.meta3.clinicedc.org",
+    "amana.tz.meta3.clinicedc.org",
+]
 
 SECURE_SSL_REDIRECT = False
 EDC_MODEL_ADMIN_CSS_THEME = "edc_purple"
 
 if os.path.exists(BASE_DIR) and not os.path.exists(KEY_PATH):  # noqa
     os.makedirs(KEY_PATH)  # noqa
     AUTO_CREATE_KEYS = True
```

### Comparing `meta-edc-demo-0.0.1/meta_edc/settings/defaults.py` & `meta-edc-demo-0.0.2/meta_edc/settings/defaults.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_edc/settings/live.py` & `meta-edc-demo-0.0.2/meta_edc/settings/uat.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,19 +2,21 @@
 
 from .defaults import *  # noqa
 
 print(f"Settings file {__file__}")  # noqa
 
 
 SITE_ID = SiteID(default=1)
-EDC_SITES_UAT_DOMAIN = False
-ALLOWED_HOSTS = ["*"]
-#ALLOWED_HOSTS = [
-#    "amana.tz.meta3.clinicedc.org",
-#    "hindu-mandal.tz.meta3.clinicedc.org",
-#    "mbagala.tz.meta3.clinicedc.org",
-#    "mnazi-moja.tz.meta3.clinicedc.org",
-#    "mwananyamala.tz.meta3.clinicedc.org",
-#    "temeke.tz.meta3.clinicedc.org",
-#]
-EDC_MODEL_ADMIN_CSS_THEME = "edc_indigo"
-LIVE_SYSTEM = True
+EDC_SITES_UAT_DOMAIN = True
+EDC_CONSENT_BYPASS_CONSENT_DATETIME_VALIDATION = True
+ALLOWED_HOSTS = [
+    "amana.uat.tz.meta3.clinicedc.org",
+    "hindu-mandal.uat.tz.meta3.clinicedc.org",
+    "mbagala.uat.tz.meta3.clinicedc.org",
+    "mnazi-moja.uat.tz.meta3.clinicedc.org",
+    "mwananyamala.uat.tz.meta3.clinicedc.org",
+    "temeke.uat.tz.meta3.clinicedc.org",
+]
+
+# edc_model_admin
+EDC_MODEL_ADMIN_CSS_THEME = "edc_purple"
+LIVE_SYSTEM = False
```

### Comparing `meta-edc-demo-0.0.1/meta_edc/settings/logging.py` & `meta-edc-demo-0.0.2/meta_edc/settings/logging.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_edc/settings/minimal.py` & `meta-edc-demo-0.0.2/meta_edc/settings/minimal.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_edc/templates/meta_edc/bootstrap3/home.html` & `meta-edc-demo-0.0.2/meta_edc/templates/meta_edc/bootstrap3/home.html`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_edc/tests/tests/test_endpoints.py` & `meta-edc-demo-0.0.2/meta_edc/tests/tests/test_endpoints.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_edc/urls.py` & `meta-edc-demo-0.0.2/meta_edc/urls.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_edc/views/home_view.py` & `meta-edc-demo-0.0.2/meta_edc/views/home_view.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_edc_demo.egg-info/PKG-INFO` & `meta-edc-demo-0.0.2/meta_edc_demo.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meta-edc-demo
-Version: 0.0.1
+Version: 0.0.2
 Summary: Testing META Trial EDC (http://www.isrctn.com/ISRCTN76157257)
 Home-page: https://github.com/meta-trial/meta-edc
 Author: Erik van Widenfelt
 Author-email: ew2789@gmail.com
 License: GPL license, see LICENSE
 Keywords: django edc META EDC,clinicedc,clinical trials
 Classifier: Programming Language :: Python :: 3
```

### Comparing `meta-edc-demo-0.0.1/meta_edc_demo.egg-info/SOURCES.txt` & `meta-edc-demo-0.0.2/meta_edc_demo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_labs/lab_profiles.py` & `meta-edc-demo-0.0.2/meta_labs/lab_profiles.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_labs/reportables.py` & `meta-edc-demo-0.0.2/meta_labs/reportables.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_labs/tests/test_labs.py` & `meta-edc-demo-0.0.2/meta_labs/tests/test_labs.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_labs/tests/test_reportables.py` & `meta-edc-demo-0.0.2/meta_labs/tests/test_reportables.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_lists/admin.py` & `meta-edc-demo-0.0.2/meta_lists/admin.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_lists/list_data.py` & `meta-edc-demo-0.0.2/meta_lists/list_data.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_lists/migrations/0001_initial.py` & `meta-edc-demo-0.0.2/meta_lists/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_lists/migrations/0002_auto_20191026_2231.py` & `meta-edc-demo-0.0.2/meta_lists/migrations/0002_auto_20191026_2231.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_lists/migrations/0003_auto_20191102_0033.py` & `meta-edc-demo-0.0.2/meta_lists/migrations/0003_auto_20191102_0033.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_lists/migrations/0004_auto_20191102_1859.py` & `meta-edc-demo-0.0.2/meta_lists/migrations/0004_auto_20191102_1859.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_lists/migrations/0005_auto_20191104_0930.py` & `meta-edc-demo-0.0.2/meta_lists/migrations/0005_auto_20191104_0930.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_lists/migrations/0006_auto_20200514_1959.py` & `meta-edc-demo-0.0.2/meta_lists/migrations/0006_auto_20200514_1959.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_lists/migrations/0007_auto_20200516_2356.py` & `meta-edc-demo-0.0.2/meta_lists/migrations/0007_auto_20200516_2356.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_lists/migrations/0008_auto_20200528_1517.py` & `meta-edc-demo-0.0.2/meta_lists/migrations/0008_auto_20200528_1517.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_lists/migrations/0010_auto_20200617_1738.py` & `meta-edc-demo-0.0.2/meta_lists/migrations/0010_auto_20200617_1738.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_lists/migrations/0011_auto_20210624_0225.py` & `meta-edc-demo-0.0.2/meta_lists/migrations/0011_auto_20210624_0225.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_lists/migrations/0012_auto_20210728_1809.py` & `meta-edc-demo-0.0.2/meta_lists/migrations/0012_auto_20210728_1809.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_lists/migrations/0013_transferreasons_and_more.py` & `meta-edc-demo-0.0.2/meta_lists/migrations/0013_transferreasons_and_more.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_lists/migrations/0014_auto_20220913_2139.py` & `meta-edc-demo-0.0.2/meta_lists/migrations/0014_auto_20220913_2139.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_lists/models.py` & `meta-edc-demo-0.0.2/meta_lists/models.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_pharmacy/apps.py` & `meta-edc-demo-0.0.2/meta_pharmacy/apps.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_pharmacy/prepare_meta_pharmacy.py` & `meta-edc-demo-0.0.2/meta_pharmacy/prepare_meta_pharmacy.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_prn/action_items.py` & `meta-edc-demo-0.0.2/meta_prn/action_items.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_prn/admin/__init__.py` & `meta-edc-demo-0.0.2/meta_prn/admin/__init__.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_prn/admin/end_of_study_admin.py` & `meta-edc-demo-0.0.2/meta_prn/admin/end_of_study_admin.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_prn/admin/loss_to_followup_admin.py` & `meta-edc-demo-0.0.2/meta_prn/admin/loss_to_followup_admin.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_prn/admin/off_study_medication_admin.py` & `meta-edc-demo-0.0.2/meta_prn/admin/off_study_medication_admin.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_prn/admin/offschedule_admin.py` & `meta-edc-demo-0.0.2/meta_prn/admin/offschedule_admin.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_prn/admin/offschedule_postnatal_admin.py` & `meta-edc-demo-0.0.2/meta_prn/admin/offschedule_postnatal_admin.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_prn/admin/offschedule_pregnancy_admin.py` & `meta-edc-demo-0.0.2/meta_prn/admin/offschedule_pregnancy_admin.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_prn/admin/onschedule_admin.py` & `meta-edc-demo-0.0.2/meta_prn/admin/onschedule_admin.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_prn/admin/pregnancy_notification_admin.py` & `meta-edc-demo-0.0.2/meta_prn/admin/pregnancy_notification_admin.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_prn/admin/protocol_incident_admin.py` & `meta-edc-demo-0.0.2/meta_prn/admin/protocol_incident_admin.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_prn/admin/subject_transfer_admin.py` & `meta-edc-demo-0.0.2/meta_prn/admin/subject_transfer_admin.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_prn/baker_recipes.py` & `meta-edc-demo-0.0.2/meta_prn/baker_recipes.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_prn/choices.py` & `meta-edc-demo-0.0.2/meta_prn/choices.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_prn/constants.py` & `meta-edc-demo-0.0.2/meta_prn/constants.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_prn/form_validators/end_of_study.py` & `meta-edc-demo-0.0.2/meta_prn/form_validators/end_of_study.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_prn/form_validators/protocol_incident.py` & `meta-edc-demo-0.0.2/meta_prn/form_validators/protocol_incident.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_prn/forms/end_of_study_form.py` & `meta-edc-demo-0.0.2/meta_prn/forms/end_of_study_form.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_prn/forms/loss_to_followup_form.py` & `meta-edc-demo-0.0.2/meta_prn/forms/loss_to_followup_form.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_prn/forms/off_study_medication_form.py` & `meta-edc-demo-0.0.2/meta_prn/forms/off_study_medication_form.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_prn/forms/offschedule_form.py` & `meta-edc-demo-0.0.2/meta_prn/forms/offschedule_form.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_prn/forms/offschedule_pregnancy_form.py` & `meta-edc-demo-0.0.2/meta_prn/forms/offschedule_pregnancy_form.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_prn/forms/pregnancy_notification_form.py` & `meta-edc-demo-0.0.2/meta_prn/forms/pregnancy_notification_form.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_prn/forms/subject_transfer_form.py` & `meta-edc-demo-0.0.2/meta_prn/forms/subject_transfer_form.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_prn/list_data.py` & `meta-edc-demo-0.0.2/meta_prn/list_data.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_prn/migrations/0001_initial.py` & `meta-edc-demo-0.0.2/meta_prn/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_prn/migrations/0002_auto_20191024_1000.py` & `meta-edc-demo-0.0.2/meta_prn/migrations/0002_auto_20191024_1000.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_prn/migrations/0003_auto_20200120_2020.py` & `meta-edc-demo-0.0.2/meta_prn/migrations/0003_auto_20200120_2020.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_prn/migrations/0004_auto_20200403_0332.py` & `meta-edc-demo-0.0.2/meta_prn/migrations/0004_auto_20200403_0332.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_prn/migrations/0005_auto_20200524_1944.py` & `meta-edc-demo-0.0.2/meta_prn/migrations/0005_auto_20200524_1944.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_prn/migrations/0006_auto_20210624_0225.py` & `meta-edc-demo-0.0.2/meta_prn/migrations/0006_auto_20210624_0225.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_prn/migrations/0007_auto_20210721_0335.py` & `meta-edc-demo-0.0.2/meta_prn/migrations/0007_auto_20210721_0335.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_prn/migrations/0008_auto_20210910_0238.py` & `meta-edc-demo-0.0.2/meta_prn/migrations/0008_auto_20210910_0238.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_prn/migrations/0009_auto_20210910_0239.py` & `meta-edc-demo-0.0.2/meta_prn/migrations/0009_auto_20210910_0239.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_prn/migrations/0010_auto_20210910_1906.py` & `meta-edc-demo-0.0.2/meta_prn/migrations/0010_auto_20210910_1906.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_prn/migrations/0011_auto_20210910_1911.py` & `meta-edc-demo-0.0.2/meta_prn/migrations/0011_auto_20210910_1911.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_prn/migrations/0012_auto_20210911_0004.py` & `meta-edc-demo-0.0.2/meta_prn/migrations/0012_auto_20210911_0004.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_prn/migrations/0013_auto_20210911_2036.py` & `meta-edc-demo-0.0.2/meta_prn/migrations/0013_auto_20210911_2036.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_prn/migrations/0014_auto_20211003_1709.py` & `meta-edc-demo-0.0.2/meta_prn/migrations/0014_auto_20211003_1709.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_prn/migrations/0015_auto_20211104_1447.py` & `meta-edc-demo-0.0.2/meta_prn/migrations/0015_auto_20211104_1447.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_prn/migrations/0016_auto_20220128_1719.py` & `meta-edc-demo-0.0.2/meta_prn/migrations/0016_auto_20220128_1719.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_prn/migrations/0017_auto_20220307_1929.py` & `meta-edc-demo-0.0.2/meta_prn/migrations/0017_auto_20220307_1929.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_prn/migrations/0018_auto_20220309_2106.py` & `meta-edc-demo-0.0.2/meta_prn/migrations/0018_auto_20220309_2106.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_prn/migrations/0019_auto_20220309_2230.py` & `meta-edc-demo-0.0.2/meta_prn/migrations/0019_auto_20220309_2230.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_prn/migrations/0020_auto_20220310_0439.py` & `meta-edc-demo-0.0.2/meta_prn/migrations/0020_auto_20220310_0439.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_prn/migrations/0021_auto_20220316_2147.py` & `meta-edc-demo-0.0.2/meta_prn/migrations/0021_auto_20220316_2147.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_prn/migrations/0022_auto_20220318_0133.py` & `meta-edc-demo-0.0.2/meta_prn/migrations/0022_auto_20220318_0133.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_prn/migrations/0023_auto_20220415_1747.py` & `meta-edc-demo-0.0.2/meta_prn/migrations/0023_auto_20220415_1747.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_prn/migrations/0024_alter_protocoldeviationviolation_violation.py` & `meta-edc-demo-0.0.2/meta_prn/migrations/0024_alter_protocoldeviationviolation_violation.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_prn/migrations/0025_alter_historicalprotocoldeviationviolation_options_and_more.py` & `meta-edc-demo-0.0.2/meta_prn/migrations/0025_alter_historicalprotocoldeviationviolation_options_and_more.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_prn/migrations/0026_remove_historicalprotocoldeviationviolation_violation_type_and_more.py` & `meta-edc-demo-0.0.2/meta_prn/migrations/0026_remove_historicalprotocoldeviationviolation_violation_type_and_more.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_prn/migrations/0027_rename_historicalprotocoldeviationviolation_historicalprotocolincident_and_more.py` & `meta-edc-demo-0.0.2/meta_prn/migrations/0027_rename_historicalprotocoldeviationviolation_historicalprotocolincident_and_more.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_prn/migrations/0028_historicalpregnancynotification_bhcg_date_and_more.py` & `meta-edc-demo-0.0.2/meta_prn/migrations/0028_historicalpregnancynotification_bhcg_date_and_more.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_prn/migrations/0029_alter_historicalpregnancynotification_edd_and_more.py` & `meta-edc-demo-0.0.2/meta_prn/migrations/0029_alter_historicalpregnancynotification_edd_and_more.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_prn/migrations/0030_auto_20220627_1119.py` & `meta-edc-demo-0.0.2/meta_prn/migrations/0030_auto_20220627_1119.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_prn/migrations/0031_alter_historicaloffschedule_options_and_more.py` & `meta-edc-demo-0.0.2/meta_prn/migrations/0031_alter_historicaloffschedule_options_and_more.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_prn/migrations/0032_historicalegfrnotification_egfrnotification.py` & `meta-edc-demo-0.0.2/meta_prn/migrations/0032_historicalegfrnotification_egfrnotification.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_prn/migrations/0033_remove_historicalegfrnotification_action_item_and_more.py` & `meta-edc-demo-0.0.2/meta_prn/migrations/0033_remove_historicalegfrnotification_action_item_and_more.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_prn/migrations/0034_auto_20220630_1110.py` & `meta-edc-demo-0.0.2/meta_prn/migrations/0034_auto_20220630_1110.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_prn/migrations/0035_auto_20220630_1140.py` & `meta-edc-demo-0.0.2/meta_prn/migrations/0035_auto_20220630_1140.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_prn/migrations/0036_remove_endofstudy_meta_prn_en_id_a50384_idx_and_more.py` & `meta-edc-demo-0.0.2/meta_prn/migrations/0036_remove_endofstudy_meta_prn_en_id_a50384_idx_and_more.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_prn/migrations/0037_endofstudy_delivery_date_endofstudy_pregnancy_date_and_more.py` & `meta-edc-demo-0.0.2/meta_prn/migrations/0037_endofstudy_delivery_date_endofstudy_pregnancy_date_and_more.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_prn/migrations/0038_alter_endofstudy_delivery_date_and_more.py` & `meta-edc-demo-0.0.2/meta_prn/migrations/0038_alter_endofstudy_delivery_date_and_more.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_prn/migrations/0039_historicaloffstudymedication_reason_other_and_more.py` & `meta-edc-demo-0.0.2/meta_prn/migrations/0039_historicaloffstudymedication_reason_other_and_more.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_prn/migrations/0040_remove_historicaloffstudymedication_expected_restart_date_and_more.py` & `meta-edc-demo-0.0.2/meta_prn/migrations/0040_remove_historicaloffstudymedication_expected_restart_date_and_more.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_prn/migrations/0041_endofstudy_transfer_date_and_more.py` & `meta-edc-demo-0.0.2/meta_prn/migrations/0041_endofstudy_transfer_date_and_more.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_prn/migrations/0042_remove_endofstudy_investigator_decision_and_more.py` & `meta-edc-demo-0.0.2/meta_prn/migrations/0042_remove_endofstudy_investigator_decision_and_more.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_prn/migrations/0043_auto_20220704_1841.py` & `meta-edc-demo-0.0.2/meta_prn/migrations/0043_auto_20220704_1841.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_prn/migrations/0044_alter_endofstudy_action_identifier_and_more.py` & `meta-edc-demo-0.0.2/meta_prn/migrations/0044_alter_endofstudy_action_identifier_and_more.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_prn/migrations/0045_auto_20220826_0258.py` & `meta-edc-demo-0.0.2/meta_prn/migrations/0045_auto_20220826_0258.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_prn/migrations/0046_auto_20220826_0322.py` & `meta-edc-demo-0.0.2/meta_prn/migrations/0046_auto_20220826_0322.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_prn/migrations/0047_auto_20220826_0406.py` & `meta-edc-demo-0.0.2/meta_prn/migrations/0047_auto_20220826_0406.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_prn/migrations/0048_auto_20220922_2236.py` & `meta-edc-demo-0.0.2/meta_prn/migrations/0048_auto_20220922_2236.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_prn/migrations/0049_auto_20220929_1742.py` & `meta-edc-demo-0.0.2/meta_prn/migrations/0049_auto_20220929_1742.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_prn/migrations/0050_auto_20221004_0629.py` & `meta-edc-demo-0.0.2/meta_prn/migrations/0050_auto_20221004_0629.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_prn/models/__init__.py` & `meta-edc-demo-0.0.2/meta_prn/models/__init__.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_prn/models/end_of_study.py` & `meta-edc-demo-0.0.2/meta_prn/models/end_of_study.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_prn/models/loss_to_followup.py` & `meta-edc-demo-0.0.2/meta_prn/models/loss_to_followup.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_prn/models/off_study_medication.py` & `meta-edc-demo-0.0.2/meta_prn/models/off_study_medication.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_prn/models/offschedule.py` & `meta-edc-demo-0.0.2/meta_prn/models/offschedule.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_prn/models/onschedule.py` & `meta-edc-demo-0.0.2/meta_prn/models/onschedule.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_prn/models/pregnancy_notification.py` & `meta-edc-demo-0.0.2/meta_prn/models/pregnancy_notification.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_prn/models/protocol_incident.py` & `meta-edc-demo-0.0.2/meta_prn/models/protocol_incident.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_prn/models/signals.py` & `meta-edc-demo-0.0.2/meta_prn/models/signals.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_prn/pregnancy_action_item_mixin.py` & `meta-edc-demo-0.0.2/meta_prn/pregnancy_action_item_mixin.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_prn/tests/tests/test_actions.py` & `meta-edc-demo-0.0.2/meta_prn/tests/tests/test_actions.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_prn/tests/tests/test_manager_order.py` & `meta-edc-demo-0.0.2/meta_prn/tests/tests/test_manager_order.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_prn/tests/tests/test_pregnancy_notification.py` & `meta-edc-demo-0.0.2/meta_prn/tests/tests/test_pregnancy_notification.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_rando/migrations/0001_initial.py` & `meta-edc-demo-0.0.2/meta_rando/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_rando/migrations/0002_auto_20220704_1841.py` & `meta-edc-demo-0.0.2/meta_rando/migrations/0002_auto_20220704_1841.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_rando/migrations/0003_auto_20220826_1640.py` & `meta-edc-demo-0.0.2/meta_rando/migrations/0003_auto_20220826_1640.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_rando/models.py` & `meta-edc-demo-0.0.2/meta_rando/models.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_rando/randomizers.py` & `meta-edc-demo-0.0.2/meta_rando/randomizers.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_rando/tests/tests/test_randomizers.py` & `meta-edc-demo-0.0.2/meta_rando/tests/tests/test_randomizers.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_reports/apps.py` & `meta-edc-demo-0.0.2/meta_reports/apps.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_reports/death_report.py` & `meta-edc-demo-0.0.2/meta_reports/death_report.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_reports/pdf_report.py` & `meta-edc-demo-0.0.2/meta_reports/pdf_report.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_reports/tests/test_reports.py` & `meta-edc-demo-0.0.2/meta_reports/tests/test_reports.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_screening/admin/fieldsets.py` & `meta-edc-demo-0.0.2/meta_screening/admin/fieldsets.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_screening/admin/list_filters.py` & `meta-edc-demo-0.0.2/meta_screening/admin/list_filters.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_screening/admin/screening_part_one_admin.py` & `meta-edc-demo-0.0.2/meta_screening/admin/screening_part_one_admin.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_screening/admin/screening_part_three_admin.py` & `meta-edc-demo-0.0.2/meta_screening/admin/screening_part_three_admin.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_screening/admin/screening_part_two_admin.py` & `meta-edc-demo-0.0.2/meta_screening/admin/screening_part_two_admin.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_screening/admin/subject_refusal_admin.py` & `meta-edc-demo-0.0.2/meta_screening/admin/subject_refusal_admin.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_screening/admin/subject_screening_admin.py` & `meta-edc-demo-0.0.2/meta_screening/admin/subject_screening_admin.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_screening/apps.py` & `meta-edc-demo-0.0.2/meta_screening/apps.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_screening/baker_recipes.py` & `meta-edc-demo-0.0.2/meta_screening/baker_recipes.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_screening/calculators.py` & `meta-edc-demo-0.0.2/meta_screening/calculators.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_screening/choices.py` & `meta-edc-demo-0.0.2/meta_screening/choices.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_screening/constants.py` & `meta-edc-demo-0.0.2/meta_screening/constants.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_screening/eligibility/eligibility.py` & `meta-edc-demo-0.0.2/meta_screening/eligibility/eligibility.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_screening/eligibility/eligibility_part_one.py` & `meta-edc-demo-0.0.2/meta_screening/eligibility/eligibility_part_one.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_screening/eligibility/eligibility_part_three/base_eligibility_part_three.py` & `meta-edc-demo-0.0.2/meta_screening/eligibility/eligibility_part_three/base_eligibility_part_three.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_screening/eligibility/eligibility_part_three/eligibility_part_three_phase_three.py` & `meta-edc-demo-0.0.2/meta_screening/eligibility/eligibility_part_three/eligibility_part_three_phase_three.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_screening/eligibility/eligibility_part_two.py` & `meta-edc-demo-0.0.2/meta_screening/eligibility/eligibility_part_two.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_screening/form_validators/screening_part_one.py` & `meta-edc-demo-0.0.2/meta_screening/form_validators/screening_part_one.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_screening/form_validators/screening_part_three.py` & `meta-edc-demo-0.0.2/meta_screening/form_validators/screening_part_three.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_screening/form_validators/screening_part_two.py` & `meta-edc-demo-0.0.2/meta_screening/form_validators/screening_part_two.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_screening/forms/__init__.py` & `meta-edc-demo-0.0.2/meta_screening/forms/__init__.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_screening/forms/field_lists.py` & `meta-edc-demo-0.0.2/meta_screening/forms/field_lists.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_screening/forms/screening_part_one_form.py` & `meta-edc-demo-0.0.2/meta_screening/forms/screening_part_one_form.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_screening/forms/screening_part_three_form.py` & `meta-edc-demo-0.0.2/meta_screening/forms/screening_part_three_form.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_screening/forms/screening_part_two_form.py` & `meta-edc-demo-0.0.2/meta_screening/forms/screening_part_two_form.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_screening/forms/subject_refusal_form.py` & `meta-edc-demo-0.0.2/meta_screening/forms/subject_refusal_form.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_screening/forms/subject_screening_form.py` & `meta-edc-demo-0.0.2/meta_screening/forms/subject_screening_form.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_screening/migrations/0001_initial.py` & `meta-edc-demo-0.0.2/meta_screening/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_screening/migrations/0002_auto_20191020_0612.py` & `meta-edc-demo-0.0.2/meta_screening/migrations/0002_auto_20191020_0612.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_screening/migrations/0003_auto_20191020_0627.py` & `meta-edc-demo-0.0.2/meta_screening/migrations/0003_auto_20191020_0627.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_screening/migrations/0004_auto_20191020_0738.py` & `meta-edc-demo-0.0.2/meta_screening/migrations/0004_auto_20191020_0738.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_screening/migrations/0005_auto_20191021_0353.py` & `meta-edc-demo-0.0.2/meta_screening/migrations/0005_auto_20191021_0353.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_screening/migrations/0006_auto_20191022_0134.py` & `meta-edc-demo-0.0.2/meta_screening/migrations/0006_auto_20191022_0134.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_screening/migrations/0007_auto_20191024_1000.py` & `meta-edc-demo-0.0.2/meta_screening/migrations/0007_auto_20191024_1000.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_screening/migrations/0008_auto_20191031_0745.py` & `meta-edc-demo-0.0.2/meta_screening/migrations/0008_auto_20191031_0745.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_screening/migrations/0009_auto_20191105_0122.py` & `meta-edc-demo-0.0.2/meta_screening/migrations/0009_auto_20191105_0122.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_screening/migrations/0010_auto_20191106_0828.py` & `meta-edc-demo-0.0.2/meta_screening/migrations/0010_auto_20191106_0828.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_screening/migrations/0011_auto_20191107_0342.py` & `meta-edc-demo-0.0.2/meta_screening/migrations/0011_auto_20191107_0342.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_screening/migrations/0012_auto_20191107_0427.py` & `meta-edc-demo-0.0.2/meta_screening/migrations/0012_auto_20191107_0427.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_screening/migrations/0013_auto_20191107_0442.py` & `meta-edc-demo-0.0.2/meta_screening/migrations/0013_auto_20191107_0442.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_screening/migrations/0014_auto_20191107_0528.py` & `meta-edc-demo-0.0.2/meta_screening/migrations/0014_auto_20191107_0528.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_screening/migrations/0015_auto_20191107_2249.py` & `meta-edc-demo-0.0.2/meta_screening/migrations/0015_auto_20191107_2249.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_screening/migrations/0016_auto_20191119_2331.py` & `meta-edc-demo-0.0.2/meta_screening/migrations/0016_auto_20191119_2331.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_screening/migrations/0017_auto_20191213_0314.py` & `meta-edc-demo-0.0.2/meta_screening/migrations/0017_auto_20191213_0314.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_screening/migrations/0018_auto_20200118_1854.py` & `meta-edc-demo-0.0.2/meta_screening/migrations/0018_auto_20200118_1854.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_screening/migrations/0019_auto_20200120_2256.py` & `meta-edc-demo-0.0.2/meta_screening/migrations/0019_auto_20200120_2256.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_screening/migrations/0020_auto_20200524_1944.py` & `meta-edc-demo-0.0.2/meta_screening/migrations/0020_auto_20200524_1944.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_screening/migrations/0021_auto_20210628_2105.py` & `meta-edc-demo-0.0.2/meta_screening/migrations/0021_auto_20210628_2105.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_screening/migrations/0022_auto_20210702_0426.py` & `meta-edc-demo-0.0.2/meta_screening/migrations/0022_auto_20210702_0426.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_screening/migrations/0023_auto_20210702_0533.py` & `meta-edc-demo-0.0.2/meta_screening/migrations/0023_auto_20210702_0533.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_screening/migrations/0024_auto_20210710_1929.py` & `meta-edc-demo-0.0.2/meta_screening/migrations/0024_auto_20210710_1929.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_screening/migrations/0025_auto_20210710_2247.py` & `meta-edc-demo-0.0.2/meta_screening/migrations/0025_auto_20210710_2247.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_screening/migrations/0026_auto_20210712_0433.py` & `meta-edc-demo-0.0.2/meta_screening/migrations/0026_auto_20210712_0433.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_screening/migrations/0028_auto_20210823_2353.py` & `meta-edc-demo-0.0.2/meta_screening/migrations/0028_auto_20210823_2353.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_screening/migrations/0029_auto_20211123_1645.py` & `meta-edc-demo-0.0.2/meta_screening/migrations/0029_auto_20211123_1645.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_screening/migrations/0030_auto_20220128_1719.py` & `meta-edc-demo-0.0.2/meta_screening/migrations/0030_auto_20220128_1719.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_screening/migrations/0031_auto_20220304_0448.py` & `meta-edc-demo-0.0.2/meta_screening/migrations/0031_auto_20220304_0448.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_screening/migrations/0032_auto_20220304_0501.py` & `meta-edc-demo-0.0.2/meta_screening/migrations/0032_auto_20220304_0501.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_screening/migrations/0033_auto_20220304_0504.py` & `meta-edc-demo-0.0.2/meta_screening/migrations/0033_auto_20220304_0504.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_screening/migrations/0034_auto_20220304_0508.py` & `meta-edc-demo-0.0.2/meta_screening/migrations/0034_auto_20220304_0508.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_screening/migrations/0035_auto_20220304_2233.py` & `meta-edc-demo-0.0.2/meta_screening/migrations/0035_auto_20220304_2233.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_screening/migrations/0036_auto_20220304_2307.py` & `meta-edc-demo-0.0.2/meta_screening/migrations/0036_auto_20220304_2307.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_screening/migrations/0037_auto_20220312_0339.py` & `meta-edc-demo-0.0.2/meta_screening/migrations/0037_auto_20220312_0339.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_screening/migrations/0038_auto_20220312_1929.py` & `meta-edc-demo-0.0.2/meta_screening/migrations/0038_auto_20220312_1929.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_screening/migrations/0039_auto_20220312_1938.py` & `meta-edc-demo-0.0.2/meta_screening/migrations/0039_auto_20220312_1938.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_screening/migrations/0040_auto_20220316_2147.py` & `meta-edc-demo-0.0.2/meta_screening/migrations/0040_auto_20220316_2147.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_screening/migrations/0041_auto_20220403_1227.py` & `meta-edc-demo-0.0.2/meta_screening/migrations/0041_auto_20220403_1227.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_screening/migrations/0042_auto_20220403_1402.py` & `meta-edc-demo-0.0.2/meta_screening/migrations/0042_auto_20220403_1402.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_screening/migrations/0043_auto_20220407_1713.py` & `meta-edc-demo-0.0.2/meta_screening/migrations/0043_auto_20220407_1713.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_screening/migrations/0044_alter_historicalscreeningpartone_severe_htn_and_more.py` & `meta-edc-demo-0.0.2/meta_screening/migrations/0044_alter_historicalscreeningpartone_severe_htn_and_more.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_screening/migrations/0045_historicalscreeningpartone_contact_number_and_more.py` & `meta-edc-demo-0.0.2/meta_screening/migrations/0045_historicalscreeningpartone_contact_number_and_more.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_screening/migrations/0046_historicalscreeningpartone_hba1c_datetime_and_more.py` & `meta-edc-demo-0.0.2/meta_screening/migrations/0046_historicalscreeningpartone_hba1c_datetime_and_more.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_screening/migrations/0047_historicalscreeningpartone_appt_datetime_repeat_and_more.py` & `meta-edc-demo-0.0.2/meta_screening/migrations/0047_historicalscreeningpartone_appt_datetime_repeat_and_more.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_screening/migrations/0048_rename_appt_datetime_repeat_historicalscreeningpartone_repeat_appt_datetime_and_more.py` & `meta-edc-demo-0.0.2/meta_screening/migrations/0048_rename_appt_datetime_repeat_historicalscreeningpartone_repeat_appt_datetime_and_more.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_screening/migrations/0049_historicalscreeningpartone_p3_ltfu_and_more.py` & `meta-edc-demo-0.0.2/meta_screening/migrations/0049_historicalscreeningpartone_p3_ltfu_and_more.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_screening/migrations/0050_historicalscreeningpartone_agree_to_p3_and_more.py` & `meta-edc-demo-0.0.2/meta_screening/migrations/0050_historicalscreeningpartone_agree_to_p3_and_more.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_screening/migrations/0051_alter_historicalscreeningpartone_advised_to_fast_and_more.py` & `meta-edc-demo-0.0.2/meta_screening/migrations/0051_alter_historicalscreeningpartone_advised_to_fast_and_more.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_screening/migrations/0052_alter_historicalscreeningpartone_p3_ltfu_and_more.py` & `meta-edc-demo-0.0.2/meta_screening/migrations/0052_alter_historicalscreeningpartone_p3_ltfu_and_more.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_screening/migrations/0053_auto_20220704_1841.py` & `meta-edc-demo-0.0.2/meta_screening/migrations/0053_auto_20220704_1841.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_screening/migrations/0054_auto_20220722_2130.py` & `meta-edc-demo-0.0.2/meta_screening/migrations/0054_auto_20220722_2130.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_screening/migrations/0055_alter_historicalscreeningpartone_creatinine_value_and_more.py` & `meta-edc-demo-0.0.2/meta_screening/migrations/0055_alter_historicalscreeningpartone_creatinine_value_and_more.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_screening/migrations/0056_alter_historicalscreeningpartone_agree_to_p3_and_more.py` & `meta-edc-demo-0.0.2/meta_screening/migrations/0056_alter_historicalscreeningpartone_agree_to_p3_and_more.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_screening/migrations/0057_alter_historicalscreeningpartone_calculated_egfr_value_and_more.py` & `meta-edc-demo-0.0.2/meta_screening/migrations/0057_alter_historicalscreeningpartone_calculated_egfr_value_and_more.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_screening/model_mixins/calculated_model_mixin.py` & `meta-edc-demo-0.0.2/meta_screening/model_mixins/calculated_model_mixin.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_screening/model_mixins/creatinine_fields_model_mixin.py` & `meta-edc-demo-0.0.2/meta_screening/model_mixins/creatinine_fields_model_mixin.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_screening/model_mixins/eligibility_model_mixin.py` & `meta-edc-demo-0.0.2/meta_screening/model_mixins/eligibility_model_mixin.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_screening/model_mixins/part_one_fields_model_mixin.py` & `meta-edc-demo-0.0.2/meta_screening/model_mixins/part_one_fields_model_mixin.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_screening/model_mixins/part_three_fields_model_mixin.py` & `meta-edc-demo-0.0.2/meta_screening/model_mixins/part_three_fields_model_mixin.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_screening/model_mixins/part_two_fields_model_mixin.py` & `meta-edc-demo-0.0.2/meta_screening/model_mixins/part_two_fields_model_mixin.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_screening/models/icp_referral.py` & `meta-edc-demo-0.0.2/meta_screening/models/icp_referral.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_screening/models/proxy_models.py` & `meta-edc-demo-0.0.2/meta_screening/models/proxy_models.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_screening/models/signals.py` & `meta-edc-demo-0.0.2/meta_screening/models/signals.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_screening/models/subject_refusal.py` & `meta-edc-demo-0.0.2/meta_screening/models/subject_refusal.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_screening/models/subject_screening.py` & `meta-edc-demo-0.0.2/meta_screening/models/subject_screening.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_screening/tests/meta_test_case_mixin.py` & `meta-edc-demo-0.0.2/meta_screening/tests/meta_test_case_mixin.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_screening/tests/options.py` & `meta-edc-demo-0.0.2/meta_screening/tests/options.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_screening/tests/tests/test_forms.py` & `meta-edc-demo-0.0.2/meta_screening/tests/tests/test_forms.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_screening/tests/tests/test_screening_part_one.py` & `meta-edc-demo-0.0.2/meta_screening/tests/tests/test_screening_part_one.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_screening/tests/tests/test_screening_part_three.py` & `meta-edc-demo-0.0.2/meta_screening/tests/tests/test_screening_part_three.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_screening/tests/tests/test_screening_part_two.py` & `meta-edc-demo-0.0.2/meta_screening/tests/tests/test_screening_part_two.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_sites/apps.py` & `meta-edc-demo-0.0.2/meta_sites/apps.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_sites/sites.py` & `meta-edc-demo-0.0.2/meta_sites/sites.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/action_items.py` & `meta-edc-demo-0.0.2/meta_subject/action_items.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/admin/__init__.py` & `meta-edc-demo-0.0.2/meta_subject/admin/__init__.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/admin/autocomplete_admin.py` & `meta-edc-demo-0.0.2/meta_subject/admin/autocomplete_admin.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/admin/birth_outcome_admin.py` & `meta-edc-demo-0.0.2/meta_subject/admin/birth_outcome_admin.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/admin/blood_results/blood_results_fbc_admin.py` & `meta-edc-demo-0.0.2/meta_subject/admin/blood_results/blood_results_fbc_admin.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/admin/blood_results/blood_results_glu_admin.py` & `meta-edc-demo-0.0.2/meta_subject/admin/blood_results/blood_results_glu_admin.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/admin/blood_results/blood_results_hba1c_admin.py` & `meta-edc-demo-0.0.2/meta_subject/admin/blood_results/blood_results_hba1c_admin.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/admin/blood_results/blood_results_ins_admin.py` & `meta-edc-demo-0.0.2/meta_subject/admin/blood_results/blood_results_ins_admin.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/admin/blood_results/blood_results_lft_admin.py` & `meta-edc-demo-0.0.2/meta_subject/admin/blood_results/blood_results_lft_admin.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/admin/blood_results/blood_results_lipid_admin.py` & `meta-edc-demo-0.0.2/meta_subject/admin/blood_results/blood_results_lipid_admin.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/admin/blood_results/blood_results_rft_admin.py` & `meta-edc-demo-0.0.2/meta_subject/admin/blood_results/blood_results_rft_admin.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/admin/complications_admin.py` & `meta-edc-demo-0.0.2/meta_subject/admin/complications_admin.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/admin/complications_glycemia_admin.py` & `meta-edc-demo-0.0.2/meta_subject/admin/complications_glycemia_admin.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/admin/concomitant_medication_admin.py` & `meta-edc-demo-0.0.2/meta_subject/admin/concomitant_medication_admin.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/admin/delivery_admin.py` & `meta-edc-demo-0.0.2/meta_subject/admin/delivery_admin.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/admin/egfr_drop_notification_admin.py` & `meta-edc-demo-0.0.2/meta_subject/admin/egfr_drop_notification_admin.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/admin/eq5d3l_admin.py` & `meta-edc-demo-0.0.2/meta_subject/admin/eq5d3l_admin.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/admin/fieldsets.py` & `meta-edc-demo-0.0.2/meta_subject/admin/fieldsets.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/admin/followup_examination_admin.py` & `meta-edc-demo-0.0.2/meta_subject/admin/followup_examination_admin.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/admin/followup_vitals_admin.py` & `meta-edc-demo-0.0.2/meta_subject/admin/followup_vitals_admin.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/admin/glucose_admin.py` & `meta-edc-demo-0.0.2/meta_subject/admin/glucose_admin.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/admin/health_economics_simple_admin.py` & `meta-edc-demo-0.0.2/meta_subject/admin/health_economics_simple_admin.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/admin/hepatitis_test_admin.py` & `meta-edc-demo-0.0.2/meta_subject/admin/hepatitis_test_admin.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/admin/malaria_test_admin.py` & `meta-edc-demo-0.0.2/meta_subject/admin/malaria_test_admin.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/admin/medication_adherence_admin.py` & `meta-edc-demo-0.0.2/meta_subject/admin/medication_adherence_admin.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/admin/mnsi_admin.py` & `meta-edc-demo-0.0.2/meta_subject/admin/mnsi_admin.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/admin/other_arv_regimens_admin.py` & `meta-edc-demo-0.0.2/meta_subject/admin/other_arv_regimens_admin.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/admin/patient_history_admin.py` & `meta-edc-demo-0.0.2/meta_subject/admin/patient_history_admin.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/admin/physical_exam_admin.py` & `meta-edc-demo-0.0.2/meta_subject/admin/physical_exam_admin.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/admin/pregnancy_update_admin.py` & `meta-edc-demo-0.0.2/meta_subject/admin/pregnancy_update_admin.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/admin/sf12_admin.py` & `meta-edc-demo-0.0.2/meta_subject/admin/sf12_admin.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/admin/study_medication_admin.py` & `meta-edc-demo-0.0.2/meta_subject/admin/study_medication_admin.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/admin/subject_requisition_admin.py` & `meta-edc-demo-0.0.2/meta_subject/admin/subject_requisition_admin.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/admin/subject_visit_admin.py` & `meta-edc-demo-0.0.2/meta_subject/admin/subject_visit_admin.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/admin/subject_visit_missed_admin.py` & `meta-edc-demo-0.0.2/meta_subject/admin/subject_visit_missed_admin.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/admin/urine_dipstick_test_admin.py` & `meta-edc-demo-0.0.2/meta_subject/admin/urine_dipstick_test_admin.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/admin/urine_pregnancy_admin.py` & `meta-edc-demo-0.0.2/meta_subject/admin/urine_pregnancy_admin.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/baker_recipes.py` & `meta-edc-demo-0.0.2/meta_subject/baker_recipes.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/choices.py` & `meta-edc-demo-0.0.2/meta_subject/choices.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/constants.py` & `meta-edc-demo-0.0.2/meta_subject/constants.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/forms/__init__.py` & `meta-edc-demo-0.0.2/meta_subject/forms/__init__.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/forms/birth_outcomes_form.py` & `meta-edc-demo-0.0.2/meta_subject/forms/birth_outcomes_form.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/forms/blood_results/blood_results_fbc_form.py` & `meta-edc-demo-0.0.2/meta_subject/forms/blood_results/blood_results_fbc_form.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/forms/blood_results/blood_results_glu_form.py` & `meta-edc-demo-0.0.2/meta_subject/forms/blood_results/blood_results_glu_form.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/forms/blood_results/blood_results_hba1c_form.py` & `meta-edc-demo-0.0.2/meta_subject/forms/blood_results/blood_results_hba1c_form.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/forms/blood_results/blood_results_ins_form.py` & `meta-edc-demo-0.0.2/meta_subject/forms/blood_results/blood_results_ins_form.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/forms/blood_results/blood_results_lft_form.py` & `meta-edc-demo-0.0.2/meta_subject/forms/blood_results/blood_results_lft_form.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/forms/blood_results/blood_results_lipid_form.py` & `meta-edc-demo-0.0.2/meta_subject/forms/blood_results/blood_results_lipid_form.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/forms/blood_results/blood_results_rft_form.py` & `meta-edc-demo-0.0.2/meta_subject/forms/blood_results/blood_results_rft_form.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/forms/delivery_form.py` & `meta-edc-demo-0.0.2/meta_subject/forms/delivery_form.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/forms/egfr_drop_notification_form.py` & `meta-edc-demo-0.0.2/meta_subject/forms/egfr_drop_notification_form.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/forms/eq53d3l_form.py` & `meta-edc-demo-0.0.2/meta_subject/forms/eq53d3l_form.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/forms/followup_examination_form.py` & `meta-edc-demo-0.0.2/meta_subject/forms/followup_examination_form.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/forms/glucose_form.py` & `meta-edc-demo-0.0.2/meta_subject/forms/glucose_form.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/forms/health_economics_simple_form.py` & `meta-edc-demo-0.0.2/meta_subject/forms/health_economics_simple_form.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/forms/hepatitis_test_form.py` & `meta-edc-demo-0.0.2/meta_subject/forms/hepatitis_test_form.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/forms/malaria_test_form.py` & `meta-edc-demo-0.0.2/meta_subject/forms/malaria_test_form.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/forms/medication_adherence_form.py` & `meta-edc-demo-0.0.2/meta_subject/forms/medication_adherence_form.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/forms/mixins.py` & `meta-edc-demo-0.0.2/meta_subject/forms/mixins.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/forms/other_arv_regimens_detail_form.py` & `meta-edc-demo-0.0.2/meta_subject/forms/other_arv_regimens_detail_form.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/forms/other_arv_regimens_form.py` & `meta-edc-demo-0.0.2/meta_subject/forms/other_arv_regimens_form.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/forms/patient_history_form.py` & `meta-edc-demo-0.0.2/meta_subject/forms/patient_history_form.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/forms/physical_exam_form.py` & `meta-edc-demo-0.0.2/meta_subject/forms/physical_exam_form.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/forms/pregnancy_update_form.py` & `meta-edc-demo-0.0.2/meta_subject/forms/pregnancy_update_form.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/forms/slider_widget.py` & `meta-edc-demo-0.0.2/meta_subject/forms/slider_widget.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/forms/study_medication_form.py` & `meta-edc-demo-0.0.2/meta_subject/forms/study_medication_form.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/forms/subject_requisition_form.py` & `meta-edc-demo-0.0.2/meta_subject/forms/subject_requisition_form.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/forms/subject_visit_form.py` & `meta-edc-demo-0.0.2/meta_subject/forms/subject_visit_form.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/forms/subject_visit_missed_form.py` & `meta-edc-demo-0.0.2/meta_subject/forms/subject_visit_missed_form.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/forms/urine_dipstick_test_form.py` & `meta-edc-demo-0.0.2/meta_subject/forms/urine_dipstick_test_form.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/forms/urine_pregnancy_form.py` & `meta-edc-demo-0.0.2/meta_subject/forms/urine_pregnancy_form.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/metadata_rules/metadata_rules.py` & `meta-edc-demo-0.0.2/meta_subject/metadata_rules/metadata_rules.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/metadata_rules/predicates.py` & `meta-edc-demo-0.0.2/meta_subject/metadata_rules/predicates.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/migrations/0001_initial.py` & `meta-edc-demo-0.0.2/meta_subject/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/migrations/0002_auto_20191021_0353.py` & `meta-edc-demo-0.0.2/meta_subject/migrations/0002_auto_20191021_0353.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/migrations/0003_auto_20191021_0534.py` & `meta-edc-demo-0.0.2/meta_subject/migrations/0003_auto_20191021_0534.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/migrations/0004_auto_20191022_0134.py` & `meta-edc-demo-0.0.2/meta_subject/migrations/0004_auto_20191022_0134.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/migrations/0005_auto_20191024_1000.py` & `meta-edc-demo-0.0.2/meta_subject/migrations/0005_auto_20191024_1000.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/migrations/0006_auto_20191104_0756.py` & `meta-edc-demo-0.0.2/meta_subject/migrations/0006_auto_20191104_0756.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/migrations/0007_auto_20191107_2249.py` & `meta-edc-demo-0.0.2/meta_subject/migrations/0007_auto_20191107_2249.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/migrations/0008_auto_20191115_0132.py` & `meta-edc-demo-0.0.2/meta_subject/migrations/0008_auto_20191115_0132.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/migrations/0009_auto_20191119_2331.py` & `meta-edc-demo-0.0.2/meta_subject/migrations/0009_auto_20191119_2331.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/migrations/0010_auto_20191213_0314.py` & `meta-edc-demo-0.0.2/meta_subject/migrations/0010_auto_20191213_0314.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/migrations/0011_auto_20200118_1854.py` & `meta-edc-demo-0.0.2/meta_subject/migrations/0011_auto_20200118_1854.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/migrations/0012_auto_20200118_2334.py` & `meta-edc-demo-0.0.2/meta_subject/migrations/0012_auto_20200118_2334.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/migrations/0013_auto_20200119_0013.py` & `meta-edc-demo-0.0.2/meta_subject/migrations/0013_auto_20200119_0013.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/migrations/0014_auto_20200120_1622.py` & `meta-edc-demo-0.0.2/meta_subject/migrations/0014_auto_20200120_1622.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/migrations/0015_auto_20200120_1943.py` & `meta-edc-demo-0.0.2/meta_subject/migrations/0015_auto_20200120_1943.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/migrations/0016_auto_20200123_1508.py` & `meta-edc-demo-0.0.2/meta_subject/migrations/0016_auto_20200123_1508.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/migrations/0017_auto_20200325_0901.py` & `meta-edc-demo-0.0.2/meta_subject/migrations/0017_auto_20200325_0901.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/migrations/0018_coronakap_historicalcoronakap.py` & `meta-edc-demo-0.0.2/meta_subject/migrations/0018_coronakap_historicalcoronakap.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/migrations/0019_auto_20200417_0315.py` & `meta-edc-demo-0.0.2/meta_subject/migrations/0019_auto_20200417_0315.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/migrations/0020_auto_20200417_0329.py` & `meta-edc-demo-0.0.2/meta_subject/migrations/0020_auto_20200417_0329.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/migrations/0021_auto_20200417_0332.py` & `meta-edc-demo-0.0.2/meta_subject/migrations/0021_auto_20200417_0332.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/migrations/0022_auto_20200419_2223.py` & `meta-edc-demo-0.0.2/meta_subject/migrations/0022_auto_20200419_2223.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/migrations/0023_auto_20200419_2305.py` & `meta-edc-demo-0.0.2/meta_subject/migrations/0023_auto_20200419_2305.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/migrations/0024_auto_20200419_2331.py` & `meta-edc-demo-0.0.2/meta_subject/migrations/0024_auto_20200419_2331.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/migrations/0025_auto_20200420_1455.py` & `meta-edc-demo-0.0.2/meta_subject/migrations/0025_auto_20200420_1455.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/migrations/0026_auto_20200420_1524.py` & `meta-edc-demo-0.0.2/meta_subject/migrations/0026_auto_20200420_1524.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/migrations/0027_auto_20200420_1645.py` & `meta-edc-demo-0.0.2/meta_subject/migrations/0027_auto_20200420_1645.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/migrations/0028_auto_20200420_1732.py` & `meta-edc-demo-0.0.2/meta_subject/migrations/0028_auto_20200420_1732.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/migrations/0029_auto_20200420_1751.py` & `meta-edc-demo-0.0.2/meta_subject/migrations/0029_auto_20200420_1751.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/migrations/0030_auto_20200420_1816.py` & `meta-edc-demo-0.0.2/meta_subject/migrations/0030_auto_20200420_1816.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/migrations/0031_auto_20200422_2039.py` & `meta-edc-demo-0.0.2/meta_subject/migrations/0031_auto_20200422_2039.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/migrations/0032_auto_20200515_0307.py` & `meta-edc-demo-0.0.2/meta_subject/migrations/0032_auto_20200515_0307.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/migrations/0033_auto_20200516_2356.py` & `meta-edc-demo-0.0.2/meta_subject/migrations/0033_auto_20200516_2356.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/migrations/0034_auto_20200517_0125.py` & `meta-edc-demo-0.0.2/meta_subject/migrations/0034_auto_20200517_0125.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/migrations/0035_auto_20200517_0128.py` & `meta-edc-demo-0.0.2/meta_subject/migrations/0035_auto_20200517_0128.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/migrations/0036_auto_20200517_0150.py` & `meta-edc-demo-0.0.2/meta_subject/migrations/0036_auto_20200517_0150.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/migrations/0037_auto_20200517_0207.py` & `meta-edc-demo-0.0.2/meta_subject/migrations/0037_auto_20200517_0207.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/migrations/0038_auto_20200520_0020.py` & `meta-edc-demo-0.0.2/meta_subject/migrations/0038_auto_20200520_0020.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/migrations/0039_auto_20200524_1944.py` & `meta-edc-demo-0.0.2/meta_subject/migrations/0039_auto_20200524_1944.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/migrations/0040_auto_20200527_2155.py` & `meta-edc-demo-0.0.2/meta_subject/migrations/0040_auto_20200527_2155.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/migrations/0041_auto_20200528_0242.py` & `meta-edc-demo-0.0.2/meta_subject/migrations/0041_auto_20200528_0242.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/migrations/0043_auto_20200528_1555.py` & `meta-edc-demo-0.0.2/meta_subject/migrations/0043_auto_20200528_1555.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/migrations/0044_auto_20200528_1853.py` & `meta-edc-demo-0.0.2/meta_subject/migrations/0044_auto_20200528_1853.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/migrations/0045_auto_20200530_1801.py` & `meta-edc-demo-0.0.2/meta_subject/migrations/0045_auto_20200530_1801.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/migrations/0046_auto_20200530_1804.py` & `meta-edc-demo-0.0.2/meta_subject/migrations/0046_auto_20200530_1804.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/migrations/0047_auto_20200530_1819.py` & `meta-edc-demo-0.0.2/meta_subject/migrations/0047_auto_20200530_1819.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/migrations/0050_auto_20200614_1934.py` & `meta-edc-demo-0.0.2/meta_subject/migrations/0050_auto_20200614_1934.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/migrations/0051_auto_20200617_2117.py` & `meta-edc-demo-0.0.2/meta_subject/migrations/0051_auto_20200617_2117.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/migrations/0052_auto_20210624_0225.py` & `meta-edc-demo-0.0.2/meta_subject/migrations/0052_auto_20210624_0225.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/migrations/0053_auto_20210628_2105.py` & `meta-edc-demo-0.0.2/meta_subject/migrations/0053_auto_20210628_2105.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/migrations/0054_auto_20210628_2314.py` & `meta-edc-demo-0.0.2/meta_subject/migrations/0054_auto_20210628_2314.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/migrations/0055_auto_20210628_2331.py` & `meta-edc-demo-0.0.2/meta_subject/migrations/0055_auto_20210628_2331.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/migrations/0056_auto_20210702_0426.py` & `meta-edc-demo-0.0.2/meta_subject/migrations/0056_auto_20210702_0426.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/migrations/0057_auto_20210702_0458.py` & `meta-edc-demo-0.0.2/meta_subject/migrations/0057_auto_20210702_0458.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/migrations/0058_auto_20210702_0533.py` & `meta-edc-demo-0.0.2/meta_subject/migrations/0058_auto_20210702_0533.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/migrations/0059_auto_20210709_2056.py` & `meta-edc-demo-0.0.2/meta_subject/migrations/0059_auto_20210709_2056.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/migrations/0060_auto_20210709_2241.py` & `meta-edc-demo-0.0.2/meta_subject/migrations/0060_auto_20210709_2241.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/migrations/0061_auto_20210710_1929.py` & `meta-edc-demo-0.0.2/meta_subject/migrations/0061_auto_20210710_1929.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/migrations/0062_auto_20210713_0616.py` & `meta-edc-demo-0.0.2/meta_subject/migrations/0062_auto_20210713_0616.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/migrations/0063_auto_20210715_0337.py` & `meta-edc-demo-0.0.2/meta_subject/migrations/0063_auto_20210715_0337.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/migrations/0064_auto_20210715_2336.py` & `meta-edc-demo-0.0.2/meta_subject/migrations/0064_auto_20210715_2336.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/migrations/0065_auto_20210716_0813.py` & `meta-edc-demo-0.0.2/meta_subject/migrations/0065_auto_20210716_0813.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/migrations/0066_auto_20210721_0335.py` & `meta-edc-demo-0.0.2/meta_subject/migrations/0066_auto_20210721_0335.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/migrations/0067_auto_20210726_0340.py` & `meta-edc-demo-0.0.2/meta_subject/migrations/0067_auto_20210726_0340.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/migrations/0068_auto_20210728_1809.py` & `meta-edc-demo-0.0.2/meta_subject/migrations/0068_auto_20210728_1809.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/migrations/0069_auto_20210801_2021.py` & `meta-edc-demo-0.0.2/meta_subject/migrations/0069_auto_20210801_2021.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/migrations/0070_auto_20210804_0438.py` & `meta-edc-demo-0.0.2/meta_subject/migrations/0070_auto_20210804_0438.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/migrations/0071_auto_20210804_0715.py` & `meta-edc-demo-0.0.2/meta_subject/migrations/0071_auto_20210804_0715.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/migrations/0072_auto_20210805_1545.py` & `meta-edc-demo-0.0.2/meta_subject/migrations/0072_auto_20210805_1545.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/migrations/0073_auto_20210809_0055.py` & `meta-edc-demo-0.0.2/meta_subject/migrations/0073_auto_20210809_0055.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/migrations/0075_auto_20210809_1744.py` & `meta-edc-demo-0.0.2/meta_subject/migrations/0075_auto_20210809_1744.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/migrations/0076_auto_20210809_1854.py` & `meta-edc-demo-0.0.2/meta_subject/migrations/0076_auto_20210809_1854.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/migrations/0077_auto_20210809_2323.py` & `meta-edc-demo-0.0.2/meta_subject/migrations/0077_auto_20210809_2323.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/migrations/0078_auto_20210810_0857.py` & `meta-edc-demo-0.0.2/meta_subject/migrations/0078_auto_20210810_0857.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/migrations/0079_auto_20210812_0335.py` & `meta-edc-demo-0.0.2/meta_subject/migrations/0079_auto_20210812_0335.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/migrations/0080_auto_20210812_0400.py` & `meta-edc-demo-0.0.2/meta_subject/migrations/0080_auto_20210812_0400.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/migrations/0081_auto_20210817_2306.py` & `meta-edc-demo-0.0.2/meta_subject/migrations/0081_auto_20210817_2306.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/migrations/0082_auto_20210823_1612.py` & `meta-edc-demo-0.0.2/meta_subject/migrations/0082_auto_20210823_1612.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/migrations/0083_auto_20210823_1620.py` & `meta-edc-demo-0.0.2/meta_subject/migrations/0083_auto_20210823_1620.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/migrations/0084_auto_20210910_0234.py` & `meta-edc-demo-0.0.2/meta_subject/migrations/0084_auto_20210910_0234.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/migrations/0085_auto_20210911_2036.py` & `meta-edc-demo-0.0.2/meta_subject/migrations/0085_auto_20210911_2036.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/migrations/0086_auto_20210920_0229.py` & `meta-edc-demo-0.0.2/meta_subject/migrations/0086_auto_20210920_0229.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/migrations/0087_auto_20210922_2058.py` & `meta-edc-demo-0.0.2/meta_subject/migrations/0087_auto_20210922_2058.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/migrations/0088_auto_20210924_0027.py` & `meta-edc-demo-0.0.2/meta_subject/migrations/0088_auto_20210924_0027.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/migrations/0089_auto_20210924_0121.py` & `meta-edc-demo-0.0.2/meta_subject/migrations/0089_auto_20210924_0121.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/migrations/0090_auto_20210924_0424.py` & `meta-edc-demo-0.0.2/meta_subject/migrations/0090_auto_20210924_0424.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/migrations/0091_auto_20210929_2324.py` & `meta-edc-demo-0.0.2/meta_subject/migrations/0091_auto_20210929_2324.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/migrations/0092_auto_20211013_0447.py` & `meta-edc-demo-0.0.2/meta_subject/migrations/0092_auto_20211013_0447.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/migrations/0093_auto_20211117_0352.py` & `meta-edc-demo-0.0.2/meta_subject/migrations/0093_auto_20211117_0352.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/migrations/0094_auto_20211123_1645.py` & `meta-edc-demo-0.0.2/meta_subject/migrations/0094_auto_20211123_1645.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/migrations/0095_auto_20220128_1719.py` & `meta-edc-demo-0.0.2/meta_subject/migrations/0095_auto_20220128_1719.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/migrations/0096_auto_20220304_0501.py` & `meta-edc-demo-0.0.2/meta_subject/migrations/0096_auto_20220304_0501.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/migrations/0097_auto_20220304_2233.py` & `meta-edc-demo-0.0.2/meta_subject/migrations/0097_auto_20220304_2233.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/migrations/0098_auto_20220309_2106.py` & `meta-edc-demo-0.0.2/meta_subject/migrations/0098_auto_20220309_2106.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/migrations/0099_auto_20220309_2218.py` & `meta-edc-demo-0.0.2/meta_subject/migrations/0099_auto_20220309_2218.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/migrations/0100_auto_20220309_2238.py` & `meta-edc-demo-0.0.2/meta_subject/migrations/0100_auto_20220309_2238.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/migrations/0101_auto_20220316_2147.py` & `meta-edc-demo-0.0.2/meta_subject/migrations/0101_auto_20220316_2147.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/migrations/0102_auto_20220324_0304.py` & `meta-edc-demo-0.0.2/meta_subject/migrations/0102_auto_20220324_0304.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/migrations/0103_auto_20220324_0326.py` & `meta-edc-demo-0.0.2/meta_subject/migrations/0103_auto_20220324_0326.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/migrations/0104_auto_20220412_2151.py` & `meta-edc-demo-0.0.2/meta_subject/migrations/0104_auto_20220412_2151.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/migrations/0105_auto_20220412_2310.py` & `meta-edc-demo-0.0.2/meta_subject/migrations/0105_auto_20220412_2310.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/migrations/0106_auto_20220414_1741.py` & `meta-edc-demo-0.0.2/meta_subject/migrations/0106_auto_20220414_1741.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/migrations/0107_auto_20220415_0043.py` & `meta-edc-demo-0.0.2/meta_subject/migrations/0107_auto_20220415_0043.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/migrations/0108_auto_20220415_1747.py` & `meta-edc-demo-0.0.2/meta_subject/migrations/0108_auto_20220415_1747.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/migrations/0109_auto_20220415_1758.py` & `meta-edc-demo-0.0.2/meta_subject/migrations/0109_auto_20220415_1758.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/migrations/0110_auto_20220512_1811.py` & `meta-edc-demo-0.0.2/meta_subject/migrations/0110_auto_20220512_1811.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/migrations/0111_alter_followupvitals_severe_htn_and_more.py` & `meta-edc-demo-0.0.2/meta_subject/migrations/0111_alter_followupvitals_severe_htn_and_more.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/migrations/0112_historicalsubjectvisit_document_status_comments_and_more.py` & `meta-edc-demo-0.0.2/meta_subject/migrations/0112_historicalsubjectvisit_document_status_comments_and_more.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/migrations/0113_bloodresultsrft_egfr_percent_change_and_more.py` & `meta-edc-demo-0.0.2/meta_subject/migrations/0113_bloodresultsrft_egfr_percent_change_and_more.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/migrations/0114_alter_bloodresultsrft_egfr_percent_change_and_more.py` & `meta-edc-demo-0.0.2/meta_subject/migrations/0114_alter_bloodresultsrft_egfr_percent_change_and_more.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/migrations/0115_historicalegfrnotification_egfrnotification.py` & `meta-edc-demo-0.0.2/meta_subject/migrations/0115_historicalegfrnotification_egfrnotification.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/migrations/0116_egfrnotification_report_status_and_more.py` & `meta-edc-demo-0.0.2/meta_subject/migrations/0116_egfrnotification_report_status_and_more.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/migrations/0117_alter_egfrnotification_managers_and_more.py` & `meta-edc-demo-0.0.2/meta_subject/migrations/0117_alter_egfrnotification_managers_and_more.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/migrations/0118_delivery_crf_status_delivery_crf_status_comments_and_more.py` & `meta-edc-demo-0.0.2/meta_subject/migrations/0118_delivery_crf_status_delivery_crf_status_comments_and_more.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/migrations/0119_historicalstudymedication_roundup_divisible_by_and_more.py` & `meta-edc-demo-0.0.2/meta_subject/migrations/0119_historicalstudymedication_roundup_divisible_by_and_more.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/migrations/0120_alter_birthoutcomes_managers_and_more.py` & `meta-edc-demo-0.0.2/meta_subject/migrations/0120_alter_birthoutcomes_managers_and_more.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/migrations/0121_auto_20220704_1841.py` & `meta-edc-demo-0.0.2/meta_subject/migrations/0121_auto_20220704_1841.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/migrations/0122_auto_20220708_2144.py` & `meta-edc-demo-0.0.2/meta_subject/migrations/0122_auto_20220708_2144.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/migrations/0123_auto_20220714_2136.py` & `meta-edc-demo-0.0.2/meta_subject/migrations/0123_auto_20220714_2136.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/migrations/0124_auto_20220714_2303.py` & `meta-edc-demo-0.0.2/meta_subject/migrations/0124_auto_20220714_2303.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/migrations/0125_auto_20220719_2134.py` & `meta-edc-demo-0.0.2/meta_subject/migrations/0125_auto_20220719_2134.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/migrations/0126_auto_20220719_2142.py` & `meta-edc-demo-0.0.2/meta_subject/migrations/0126_auto_20220719_2142.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/migrations/0127_auto_20220720_0053.py` & `meta-edc-demo-0.0.2/meta_subject/migrations/0127_auto_20220720_0053.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/migrations/0128_auto_20220720_0055.py` & `meta-edc-demo-0.0.2/meta_subject/migrations/0128_auto_20220720_0055.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/migrations/0130_auto_20220720_0216.py` & `meta-edc-demo-0.0.2/meta_subject/migrations/0130_auto_20220720_0216.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/migrations/0131_auto_20220722_0411.py` & `meta-edc-demo-0.0.2/meta_subject/migrations/0131_auto_20220722_0411.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/migrations/0132_auto_20220722_1825.py` & `meta-edc-demo-0.0.2/meta_subject/migrations/0132_auto_20220722_1825.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/migrations/0133_auto_20220722_2140.py` & `meta-edc-demo-0.0.2/meta_subject/migrations/0133_auto_20220722_2140.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/migrations/0134_auto_20220722_2211.py` & `meta-edc-demo-0.0.2/meta_subject/migrations/0134_auto_20220722_2211.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/migrations/0135_auto_20220722_2212.py` & `meta-edc-demo-0.0.2/meta_subject/migrations/0135_auto_20220722_2212.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/migrations/0136_egfrdropnotification_creatinine_quantifier_and_more.py` & `meta-edc-demo-0.0.2/meta_subject/migrations/0136_egfrdropnotification_creatinine_quantifier_and_more.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/migrations/0137_alter_egfrdropnotification_egfr_percent_change_and_more.py` & `meta-edc-demo-0.0.2/meta_subject/migrations/0137_alter_egfrdropnotification_egfr_percent_change_and_more.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/migrations/0138_alter_glucose_fbg_datetime_and_more.py` & `meta-edc-demo-0.0.2/meta_subject/migrations/0138_alter_glucose_fbg_datetime_and_more.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/migrations/0139_alter_bloodresultsins_ins_units_and_more.py` & `meta-edc-demo-0.0.2/meta_subject/migrations/0139_alter_bloodresultsins_ins_units_and_more.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/migrations/0140_alter_bloodresultsfbc_action_identifier_and_more.py` & `meta-edc-demo-0.0.2/meta_subject/migrations/0140_alter_bloodresultsfbc_action_identifier_and_more.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/migrations/0141_auto_20220826_0258.py` & `meta-edc-demo-0.0.2/meta_subject/migrations/0141_auto_20220826_0258.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/migrations/0142_auto_20220826_0322.py` & `meta-edc-demo-0.0.2/meta_subject/migrations/0142_auto_20220826_0322.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/migrations/0143_auto_20220826_0406.py` & `meta-edc-demo-0.0.2/meta_subject/migrations/0143_auto_20220826_0406.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/migrations/0144_auto_20220907_0157.py` & `meta-edc-demo-0.0.2/meta_subject/migrations/0144_auto_20220907_0157.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/migrations/0145_auto_20220907_0202.py` & `meta-edc-demo-0.0.2/meta_subject/migrations/0145_auto_20220907_0202.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/migrations/0146_auto_20220907_0207.py` & `meta-edc-demo-0.0.2/meta_subject/migrations/0146_auto_20220907_0207.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/migrations/0147_auto_20220907_1505.py` & `meta-edc-demo-0.0.2/meta_subject/migrations/0147_auto_20220907_1505.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/migrations/0148_auto_20220908_1826.py` & `meta-edc-demo-0.0.2/meta_subject/migrations/0148_auto_20220908_1826.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/migrations/0149_auto_20220913_2139.py` & `meta-edc-demo-0.0.2/meta_subject/migrations/0149_auto_20220913_2139.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/migrations/0150_auto_20220914_0039.py` & `meta-edc-demo-0.0.2/meta_subject/migrations/0150_auto_20220914_0039.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/migrations/0151_auto_20220918_0508.py` & `meta-edc-demo-0.0.2/meta_subject/migrations/0151_auto_20220918_0508.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/migrations/0152_auto_20220925_0509.py` & `meta-edc-demo-0.0.2/meta_subject/migrations/0152_auto_20220925_0509.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/migrations/0153_auto_20220928_0250.py` & `meta-edc-demo-0.0.2/meta_subject/migrations/0153_auto_20220928_0250.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/migrations/0154_auto_20220928_0419.py` & `meta-edc-demo-0.0.2/meta_subject/migrations/0154_auto_20220928_0419.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/migrations/0155_auto_20220929_1742.py` & `meta-edc-demo-0.0.2/meta_subject/migrations/0155_auto_20220929_1742.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/migrations/0156_alter_bloodresultsfbc_assay_datetime_and_more.py` & `meta-edc-demo-0.0.2/meta_subject/migrations/0156_alter_bloodresultsfbc_assay_datetime_and_more.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/model_mixins/arv_history_model_mixin.py` & `meta-edc-demo-0.0.2/meta_subject/model_mixins/arv_history_model_mixin.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/model_mixins/vitals_fields_model_mixin.py` & `meta-edc-demo-0.0.2/meta_subject/model_mixins/vitals_fields_model_mixin.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/models/__init__.py` & `meta-edc-demo-0.0.2/meta_subject/models/__init__.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/models/birth_outcomes.py` & `meta-edc-demo-0.0.2/meta_subject/models/birth_outcomes.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/models/blood_results/blood_results_fbc.py` & `meta-edc-demo-0.0.2/meta_subject/models/blood_results/blood_results_fbc.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/models/blood_results/blood_results_glu.py` & `meta-edc-demo-0.0.2/meta_subject/models/blood_results/blood_results_glu.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/models/blood_results/blood_results_hba1c.py` & `meta-edc-demo-0.0.2/meta_subject/models/blood_results/blood_results_hba1c.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/models/blood_results/blood_results_ins.py` & `meta-edc-demo-0.0.2/meta_subject/models/blood_results/blood_results_ins.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/models/blood_results/blood_results_lft.py` & `meta-edc-demo-0.0.2/meta_subject/models/blood_results/blood_results_lft.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/models/blood_results/blood_results_lipid.py` & `meta-edc-demo-0.0.2/meta_subject/models/blood_results/blood_results_lipid.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/models/blood_results/blood_results_rft.py` & `meta-edc-demo-0.0.2/meta_subject/models/blood_results/blood_results_rft.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/models/complications.py` & `meta-edc-demo-0.0.2/meta_subject/models/complications.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/models/complications_glycemia.py` & `meta-edc-demo-0.0.2/meta_subject/models/complications_glycemia.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/models/delivery.py` & `meta-edc-demo-0.0.2/meta_subject/models/delivery.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/models/diet_and_lifestyle.py` & `meta-edc-demo-0.0.2/meta_subject/models/diet_and_lifestyle.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/models/egfr_drop_notification.py` & `meta-edc-demo-0.0.2/meta_subject/models/egfr_drop_notification.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/models/followup_examination.py` & `meta-edc-demo-0.0.2/meta_subject/models/followup_examination.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/models/followup_vitals.py` & `meta-edc-demo-0.0.2/meta_subject/models/followup_vitals.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/models/glucose.py` & `meta-edc-demo-0.0.2/meta_subject/models/glucose.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/models/health_economics.py` & `meta-edc-demo-0.0.2/meta_subject/models/health_economics.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/models/health_economics_simple.py` & `meta-edc-demo-0.0.2/meta_subject/models/health_economics_simple.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/models/hepatitis_test.py` & `meta-edc-demo-0.0.2/meta_subject/models/hepatitis_test.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/models/malaria_test.py` & `meta-edc-demo-0.0.2/meta_subject/models/malaria_test.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/models/off_study_drug.py` & `meta-edc-demo-0.0.2/meta_subject/models/off_study_drug.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/models/other_arv_regimens.py` & `meta-edc-demo-0.0.2/meta_subject/models/other_arv_regimens.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/models/other_arv_regimens_detail.py` & `meta-edc-demo-0.0.2/meta_subject/models/other_arv_regimens_detail.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/models/patient_history.py` & `meta-edc-demo-0.0.2/meta_subject/models/patient_history.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/models/physical_exam.py` & `meta-edc-demo-0.0.2/meta_subject/models/physical_exam.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/models/pregnancy_update.py` & `meta-edc-demo-0.0.2/meta_subject/models/pregnancy_update.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/models/signals.py` & `meta-edc-demo-0.0.2/meta_subject/models/signals.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/models/subject_visit.py` & `meta-edc-demo-0.0.2/meta_subject/models/subject_visit.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/models/subject_visit_missed.py` & `meta-edc-demo-0.0.2/meta_subject/models/subject_visit_missed.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/models/urine_dipstick_test.py` & `meta-edc-demo-0.0.2/meta_subject/models/urine_dipstick_test.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/models/urine_pregnancy.py` & `meta-edc-demo-0.0.2/meta_subject/models/urine_pregnancy.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/tests/tests/test_egfr.py` & `meta-edc-demo-0.0.2/meta_subject/tests/tests/test_egfr.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/tests/tests/test_followup.py` & `meta-edc-demo-0.0.2/meta_subject/tests/tests/test_followup.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/tests/tests/test_manager_order.py` & `meta-edc-demo-0.0.2/meta_subject/tests/tests/test_manager_order.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/tests/tests/test_medication_adherence.py` & `meta-edc-demo-0.0.2/meta_subject/tests/tests/test_medication_adherence.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/tests/tests/test_metadata_rules.py` & `meta-edc-demo-0.0.2/meta_subject/tests/tests/test_metadata_rules.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/tests/tests/test_mnsi.py` & `meta-edc-demo-0.0.2/meta_subject/tests/tests/test_mnsi.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/tests/tests/test_patient_history_form.py` & `meta-edc-demo-0.0.2/meta_subject/tests/tests/test_patient_history_form.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/tests/tests/test_physical_exam.py` & `meta-edc-demo-0.0.2/meta_subject/tests/tests/test_physical_exam.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/tests/tests/test_sf12.py` & `meta-edc-demo-0.0.2/meta_subject/tests/tests/test_sf12.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/tests/tests/test_study_medication.py` & `meta-edc-demo-0.0.2/meta_subject/tests/tests/test_study_medication.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_subject/tests/urls.py` & `meta-edc-demo-0.0.2/meta_subject/tests/urls.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_visit_schedule/tests/tests/test_schedule.py` & `meta-edc-demo-0.0.2/meta_visit_schedule/tests/tests/test_schedule.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_visit_schedule/visit_schedules/phase_three/crfs.py` & `meta-edc-demo-0.0.2/meta_visit_schedule/visit_schedules/phase_three/crfs.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_visit_schedule/visit_schedules/phase_three/requisitions.py` & `meta-edc-demo-0.0.2/meta_visit_schedule/visit_schedules/phase_three/requisitions.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_visit_schedule/visit_schedules/phase_three/schedule.py` & `meta-edc-demo-0.0.2/meta_visit_schedule/visit_schedules/phase_three/schedule.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_visit_schedule/visit_schedules/phase_three/schedule_pregnancy.py` & `meta-edc-demo-0.0.2/meta_visit_schedule/visit_schedules/phase_three/schedule_pregnancy.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/meta_visit_schedule/visit_schedules/phase_three/visit_schedule.py` & `meta-edc-demo-0.0.2/meta_visit_schedule/visit_schedules/phase_three/visit_schedule.py`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/pyproject.toml` & `meta-edc-demo-0.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `meta-edc-demo-0.0.1/setup.cfg` & `meta-edc-demo-0.0.2/setup.cfg`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [metadata]
-name = meta-edc-demo
+name = meta-edc
 version = attr: _version
 author = Erik van Widenfelt
 author_email = ew2789@gmail.com
 url = https://github.com/meta-trial/meta-edc
 license = GPL license, see LICENSE
 description = META Trial EDC (http://www.isrctn.com/ISRCTN76157257)
 long_description = file: README.rst
```

### Comparing `meta-edc-demo-0.0.1/setup.py` & `meta-edc-demo-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import setuptools
 
 long_description = '123'
 
 setuptools.setup(
     name="meta-edc-demo",
-    version="0.0.1",
+    version="0.0.2",
     author="Erik van Widenfelt",
     author_email="ew2789@gmail.com",
     description="Testing META Trial EDC (http://www.isrctn.com/ISRCTN76157257)",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/meta-trial/meta-edc",
     classifiers=[
```

