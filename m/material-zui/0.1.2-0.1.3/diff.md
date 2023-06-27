# Comparing `tmp/material_zui-0.1.2.tar.gz` & `tmp/material_zui-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "material_zui-0.1.2.tar", max compression
+gzip compressed data, was "material_zui-0.1.3.tar", max compression
```

## Comparing `material_zui-0.1.2.tar` & `material_zui-0.1.3.tar`

### file list

```diff
@@ -1,102 +1,99 @@
--rw-r--r--   0        0        0     1091 2023-06-23 08:06:01.615959 material_zui-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      260 2023-05-01 15:33:57.972869 material_zui-0.1.2/src/material_zui/.pypirc
--rw-r--r--   0        0        0      555 2023-03-21 08:40:33.421115 material_zui-0.1.2/src/material_zui/ResizeImage.py
--rw-r--r--   0        0        0     2405 2023-05-20 11:57:06.283965 material_zui-0.1.2/src/material_zui/automation/Constant.py
--rw-r--r--   0        0        0       44 2023-05-21 02:36:24.004618 material_zui-0.1.2/src/material_zui/automation/__init__.py
--rw-r--r--   0        0        0      175 2023-06-18 12:07:30.298939 material_zui-0.1.2/src/material_zui/automation/data.py
--rw-r--r--   0        0        0      110 2023-05-21 04:26:37.532312 material_zui-0.1.2/src/material_zui/automation/index.py
--rw-r--r--   0        0        0        0 2023-05-21 02:38:12.347239 material_zui-0.1.2/src/material_zui/automation/pinterest.py
--rw-r--r--   0        0        0    10600 2023-06-19 01:47:01.519677 material_zui-0.1.2/src/material_zui/automation/tiktok.py
--rw-r--r--   0        0        0      310 2023-05-21 14:22:10.812226 material_zui-0.1.2/src/material_zui/automation/type.py
--rw-r--r--   0        0        0    13957 2023-06-23 02:26:53.960600 material_zui-0.1.2/src/material_zui/automation/youtube.py
--rw-r--r--   0        0        0       38 2023-05-25 02:02:05.757233 material_zui-0.1.2/src/material_zui/bard/__init__.py
--rw-r--r--   0        0        0      543 2023-05-25 02:04:14.001207 material_zui-0.1.2/src/material_zui/bard/google_bard.py
--rw-r--r--   0        0        0       77 2023-05-25 02:02:05.757233 material_zui-0.1.2/src/material_zui/bard/index.py
--rw-r--r--   0        0        0       41 2023-06-09 09:12:08.062573 material_zui-0.1.2/src/material_zui/bing_ai/__init__.py
--rw-r--r--   0        0        0     2572 2023-06-14 10:38:43.733788 material_zui-0.1.2/src/material_zui/bing_ai/bing_ai.py
--rw-r--r--   0        0        0       51 2023-06-09 09:12:20.262575 material_zui-0.1.2/src/material_zui/bing_ai/index.py
--rw-r--r--   0        0        0      868 2023-06-14 08:51:22.816844 material_zui-0.1.2/src/material_zui/bing_ai/result.py
--rw-r--r--   0        0        0       42 2023-05-07 05:09:56.400820 material_zui-0.1.2/src/material_zui/compress/__init__.py
--rw-r--r--   0        0        0       74 2023-05-07 05:16:12.115224 material_zui-0.1.2/src/material_zui/compress/index.py
--rw-r--r--   0        0        0     2131 2023-05-07 05:22:45.101162 material_zui-0.1.2/src/material_zui/compress/text.py
--rw-r--r--   0        0        0       39 2023-05-22 10:20:44.145129 material_zui-0.1.2/src/material_zui/crawl/__init__.py
--rw-r--r--   0        0        0     3282 2023-05-28 04:29:31.650227 material_zui-0.1.2/src/material_zui/crawl/image.py
--rw-r--r--   0        0        0      171 2023-05-28 04:26:35.259642 material_zui-0.1.2/src/material_zui/crawl/index.py
--rw-r--r--   0        0        0       41 2023-05-11 04:24:47.172982 material_zui-0.1.2/src/material_zui/crontab/__init__.py
--rw-r--r--   0        0        0      638 2023-05-11 04:23:06.569200 material_zui-0.1.2/src/material_zui/crontab/index.py
--rw-r--r--   0        0        0       21 2023-06-12 02:21:47.920504 material_zui-0.1.2/src/material_zui/date_time/__init__.py
--rw-r--r--   0        0        0      219 2023-06-12 02:56:34.237482 material_zui-0.1.2/src/material_zui/date_time/__init__.pyc
--rw-r--r--   0        0        0      491 2023-06-18 06:24:16.415897 material_zui-0.1.2/src/material_zui/date_time/date_time.py
--rw-r--r--   0        0        0       73 2023-06-13 08:55:03.914876 material_zui-0.1.2/src/material_zui/date_time/index.py
--rw-r--r--   0        0        0      180 2023-06-12 02:58:53.334820 material_zui-0.1.2/src/material_zui/date_time/index.pyc
--rw-r--r--   0        0        0      692 2023-05-07 14:16:10.888166 material_zui-0.1.2/src/material_zui/date_time/time.py
--rw-r--r--   0        0        0       36 2023-05-21 13:41:44.819759 material_zui-0.1.2/src/material_zui/dict/__init__.py
--rw-r--r--   0        0        0        0 2023-05-21 13:45:02.045051 material_zui-0.1.2/src/material_zui/dict/common.py
--rw-r--r--   0        0        0        0 2023-05-21 13:41:44.819759 material_zui-0.1.2/src/material_zui/dict/index.py
--rw-r--r--   0        0        0       37 2023-05-15 08:36:55.132989 material_zui-0.1.2/src/material_zui/env/__init__.py
--rw-r--r--   0        0        0      183 2023-05-15 09:09:28.356336 material_zui-0.1.2/src/material_zui/env/env.py
--rw-r--r--   0        0        0       52 2023-05-15 08:46:26.760087 material_zui-0.1.2/src/material_zui/env/index.py
--rw-r--r--   0        0        0       38 2023-05-19 02:12:30.886319 material_zui-0.1.2/src/material_zui/fake/__init__.py
--rw-r--r--   0        0        0       62 2023-05-19 02:24:23.295278 material_zui-0.1.2/src/material_zui/fake/index.py
--rw-r--r--   0        0        0      254 2023-05-21 05:39:54.079978 material_zui-0.1.2/src/material_zui/fake/number.py
--rw-r--r--   0        0        0       38 2023-05-21 03:57:08.912678 material_zui-0.1.2/src/material_zui/file/__init__.py
--rw-r--r--   0        0        0      551 2023-06-23 07:37:11.257875 material_zui-0.1.2/src/material_zui/file/check.py
--rw-r--r--   0        0        0     2115 2023-06-15 03:25:12.103320 material_zui-0.1.2/src/material_zui/file/common.py
--rw-r--r--   0        0        0      304 2023-06-15 03:25:12.271318 material_zui-0.1.2/src/material_zui/file/download.py
--rw-r--r--   0        0        0      326 2023-06-23 08:03:00.554832 material_zui-0.1.2/src/material_zui/file/index.py
--rw-r--r--   0        0        0     1042 2023-06-15 03:25:12.027320 material_zui-0.1.2/src/material_zui/file/read.py
--rw-r--r--   0        0        0       77 2023-06-10 05:42:45.080334 material_zui-0.1.2/src/material_zui/file/type.py
--rw-r--r--   0        0        0      992 2023-06-23 08:03:07.838708 material_zui-0.1.2/src/material_zui/file/write.py
--rw-r--r--   0        0        0       37 2023-05-25 02:02:05.757233 material_zui-0.1.2/src/material_zui/gpt/__init__.py
--rw-r--r--   0        0        0     1048 2023-05-25 02:22:20.028251 material_zui-0.1.2/src/material_zui/gpt/gpt_vietnam.py
--rw-r--r--   0        0        0       63 2023-05-25 02:22:19.960250 material_zui-0.1.2/src/material_zui/gpt/index.py
--rw-r--r--   0        0        0      216 2023-05-11 09:54:07.451440 material_zui-0.1.2/src/material_zui/image/__init__.py
--rw-r--r--   0        0        0     2199 2023-05-05 09:48:58.874264 material_zui-0.1.2/src/material_zui/image/colorization.py
--rw-r--r--   0        0        0     2921 2023-05-11 09:52:23.138728 material_zui-0.1.2/src/material_zui/image/combine.py
--rw-r--r--   0        0        0     7057 2023-05-28 04:11:03.932782 material_zui-0.1.2/src/material_zui/image/common.py
--rw-r--r--   0        0        0     2808 2023-05-11 10:13:26.444992 material_zui-0.1.2/src/material_zui/image/convert.py
--rw-r--r--   0        0        0       78 2023-05-06 06:26:57.697131 material_zui-0.1.2/src/material_zui/image/data.py
--rw-r--r--   0        0        0      490 2023-05-28 04:11:04.028780 material_zui-0.1.2/src/material_zui/image/index.py
--rw-r--r--   0        0        0     9945 2023-05-05 03:49:43.138352 material_zui-0.1.2/src/material_zui/image/model/colorization_deploy_v2.prototxt
--rw-r--r--   0        0        0     5088 2023-05-05 03:49:53.225773 material_zui-0.1.2/src/material_zui/image/model/pts_in_hull.npy
--rw-r--r--   0        0        0      782 2023-05-11 04:50:18.808963 material_zui-0.1.2/src/material_zui/image/remove_background.py
--rw-r--r--   0        0        0     6445 2023-05-06 08:59:41.215230 material_zui-0.1.2/src/material_zui/image/to_svg.py
--rw-r--r--   0        0        0      520 2023-05-11 09:48:54.829117 material_zui-0.1.2/src/material_zui/image/transparent_background.py
--rw-r--r--   0        0        0      249 2023-04-28 09:24:02.020353 material_zui-0.1.2/src/material_zui/image/type.py
--rw-r--r--   0        0        0     4779 2023-05-11 10:15:27.410813 material_zui-0.1.2/src/material_zui/image/upscale.py
--rw-r--r--   0        0        0       38 2023-05-22 04:09:03.922071 material_zui-0.1.2/src/material_zui/list/__init__.py
--rw-r--r--   0        0        0     2916 2023-06-18 14:13:03.127264 material_zui-0.1.2/src/material_zui/list/common.py
--rw-r--r--   0        0        0       92 2023-06-13 09:15:39.330734 material_zui-0.1.2/src/material_zui/list/index.py
--rw-r--r--   0        0        0       37 2023-04-30 11:48:06.179161 material_zui-0.1.2/src/material_zui/log/__init__.py
--rw-r--r--   0        0        0       83 2023-05-11 10:20:42.114888 material_zui-0.1.2/src/material_zui/log/index.py
--rw-r--r--   0        0        0      559 2023-05-11 10:19:34.415566 material_zui-0.1.2/src/material_zui/log/log.py
--rw-r--r--   0        0        0       21 2023-06-13 09:33:05.320819 material_zui-0.1.2/src/material_zui/number/__init__.py
--rw-r--r--   0        0        0      364 2023-06-13 10:11:32.006838 material_zui-0.1.2/src/material_zui/number/common.py
--rw-r--r--   0        0        0       47 2023-06-13 09:40:32.023908 material_zui-0.1.2/src/material_zui/number/index.py
--rw-r--r--   0        0        0       36 2023-05-20 14:09:01.119097 material_zui-0.1.2/src/material_zui/os/__init__.py
--rw-r--r--   0        0        0       83 2023-06-16 02:02:57.672095 material_zui-0.1.2/src/material_zui/os/index.py
--rw-r--r--   0        0        0      840 2023-06-15 03:40:00.119319 material_zui-0.1.2/src/material_zui/os/os.py
--rw-r--r--   0        0        0     1213 2023-06-23 08:04:27.953396 material_zui-0.1.2/src/material_zui/readme.md
--rw-r--r--   0        0        0       39 2023-05-02 05:15:13.799596 material_zui-0.1.2/src/material_zui/regex/__init__.py
--rw-r--r--   0        0        0     5344 2023-05-02 05:18:47.668155 material_zui-0.1.2/src/material_zui/regex/index.py
--rw-r--r--   0        0        0       43 2023-04-30 11:47:27.662335 material_zui-0.1.2/src/material_zui/replicate/__init__.py
--rw-r--r--   0        0        0     2481 2023-05-01 15:33:18.205379 material_zui-0.1.2/src/material_zui/replicate/index.py
--rw-r--r--   0        0        0       42 2023-05-18 03:46:44.861073 material_zui-0.1.2/src/material_zui/selenium/__init__.py
--rw-r--r--   0        0        0     5939 2023-06-18 11:54:12.858507 material_zui-0.1.2/src/material_zui/selenium/chrome.py
--rw-r--r--   0        0        0      257 2023-05-22 02:03:22.582766 material_zui-0.1.2/src/material_zui/selenium/common.py
--rw-r--r--   0        0        0      120 2023-05-22 02:03:54.393486 material_zui-0.1.2/src/material_zui/selenium/index.py
--rw-r--r--   0        0        0      895 2023-05-11 10:31:29.010961 material_zui-0.1.2/src/material_zui/setup.py
--rw-r--r--   0        0        0       40 2023-06-10 10:50:13.743103 material_zui-0.1.2/src/material_zui/string/__init__.py
--rw-r--r--   0        0        0     2802 2023-06-18 14:03:40.774857 material_zui-0.1.2/src/material_zui/string/common.py
--rw-r--r--   0        0        0      135 2023-06-14 08:12:20.153192 material_zui-0.1.2/src/material_zui/string/index.py
--rw-r--r--   0        0        0       46 2023-05-02 13:44:38.645684 material_zui-0.1.2/src/material_zui/telegram_bot/__init__.py
--rw-r--r--   0        0        0      432 2023-05-07 05:43:32.880583 material_zui-0.1.2/src/material_zui/telegram_bot/index.py
--rw-r--r--   0        0        0       23 2023-06-12 02:21:47.852520 material_zui-0.1.2/src/material_zui/tmp/__init__.py
--rw-r--r--   0        0        0       24 2023-06-12 02:21:47.776537 material_zui-0.1.2/src/material_zui/tmp/index.py
--rw-r--r--   0        0        0       41 2023-06-11 03:35:54.474267 material_zui-0.1.2/src/material_zui/utility/__init__.py
--rw-r--r--   0        0        0      888 2023-06-11 04:23:19.200816 material_zui-0.1.2/src/material_zui/utility/common.py
--rw-r--r--   0        0        0       56 2023-06-11 04:21:30.408379 material_zui-0.1.2/src/material_zui/utility/index.py
--rw-r--r--   0        0        0       42 2023-05-25 02:32:34.010325 material_zui-0.1.2/src/material_zui/validate/__init__.py
--rw-r--r--   0        0        0      308 2023-05-28 04:05:43.248601 material_zui-0.1.2/src/material_zui/validate/common.py
--rw-r--r--   0        0        0       65 2023-05-27 14:15:24.849747 material_zui-0.1.2/src/material_zui/validate/index.py
--rw-r--r--   0        0        0     2631 1970-01-01 00:00:00.000000 material_zui-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1224 2023-06-27 07:46:19.598737 material_zui-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      260 2023-05-01 15:33:57.972869 material_zui-0.1.3/src/material_zui/.pypirc
+-rw-r--r--   0        0        0      555 2023-03-21 08:40:33.421115 material_zui-0.1.3/src/material_zui/ResizeImage.py
+-rw-r--r--   0        0        0       38 2023-05-25 02:02:05.757233 material_zui-0.1.3/src/material_zui/bard/__init__.py
+-rw-r--r--   0        0        0      543 2023-05-25 02:04:14.001207 material_zui-0.1.3/src/material_zui/bard/google_bard.py
+-rw-r--r--   0        0        0       77 2023-05-25 02:02:05.757233 material_zui-0.1.3/src/material_zui/bard/index.py
+-rw-r--r--   0        0        0       41 2023-06-09 09:12:08.062573 material_zui-0.1.3/src/material_zui/bing_ai/__init__.py
+-rw-r--r--   0        0        0     3531 2023-06-27 03:27:48.335228 material_zui-0.1.3/src/material_zui/bing_ai/bing_ai.py
+-rw-r--r--   0        0        0       51 2023-06-09 09:12:20.262575 material_zui-0.1.3/src/material_zui/bing_ai/index.py
+-rw-r--r--   0        0        0      955 2023-06-24 04:25:16.261811 material_zui-0.1.3/src/material_zui/bing_ai/result.py
+-rw-r--r--   0        0        0      132 2023-06-24 05:06:49.316509 material_zui-0.1.3/src/material_zui/bing_ai/type.py
+-rw-r--r--   0        0        0       42 2023-05-07 05:09:56.400820 material_zui-0.1.3/src/material_zui/compress/__init__.py
+-rw-r--r--   0        0        0       74 2023-05-07 05:16:12.115224 material_zui-0.1.3/src/material_zui/compress/index.py
+-rw-r--r--   0        0        0     2131 2023-05-07 05:22:45.101162 material_zui-0.1.3/src/material_zui/compress/text.py
+-rw-r--r--   0        0        0       39 2023-05-22 10:20:44.145129 material_zui-0.1.3/src/material_zui/crawl/__init__.py
+-rw-r--r--   0        0        0     3282 2023-05-28 04:29:31.650227 material_zui-0.1.3/src/material_zui/crawl/image.py
+-rw-r--r--   0        0        0      171 2023-05-28 04:26:35.259642 material_zui-0.1.3/src/material_zui/crawl/index.py
+-rw-r--r--   0        0        0       41 2023-05-11 04:24:47.172982 material_zui-0.1.3/src/material_zui/crontab/__init__.py
+-rw-r--r--   0        0        0      638 2023-05-11 04:23:06.569200 material_zui-0.1.3/src/material_zui/crontab/index.py
+-rw-r--r--   0        0        0       21 2023-06-12 02:21:47.920504 material_zui-0.1.3/src/material_zui/date_time/__init__.py
+-rw-r--r--   0        0        0      219 2023-06-12 02:56:34.237482 material_zui-0.1.3/src/material_zui/date_time/__init__.pyc
+-rw-r--r--   0        0        0      491 2023-06-18 06:24:16.415897 material_zui-0.1.3/src/material_zui/date_time/date_time.py
+-rw-r--r--   0        0        0       73 2023-06-13 08:55:03.914876 material_zui-0.1.3/src/material_zui/date_time/index.py
+-rw-r--r--   0        0        0      180 2023-06-12 02:58:53.334820 material_zui-0.1.3/src/material_zui/date_time/index.pyc
+-rw-r--r--   0        0        0      692 2023-05-07 14:16:10.888166 material_zui-0.1.3/src/material_zui/date_time/time.py
+-rw-r--r--   0        0        0       36 2023-05-21 13:41:44.819759 material_zui-0.1.3/src/material_zui/dict/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-21 13:45:02.045051 material_zui-0.1.3/src/material_zui/dict/common.py
+-rw-r--r--   0        0        0        0 2023-05-21 13:41:44.819759 material_zui-0.1.3/src/material_zui/dict/index.py
+-rw-r--r--   0        0        0       37 2023-05-15 08:36:55.132989 material_zui-0.1.3/src/material_zui/env/__init__.py
+-rw-r--r--   0        0        0      183 2023-05-15 09:09:28.356336 material_zui-0.1.3/src/material_zui/env/env.py
+-rw-r--r--   0        0        0       52 2023-05-15 08:46:26.760087 material_zui-0.1.3/src/material_zui/env/index.py
+-rw-r--r--   0        0        0       38 2023-05-19 02:12:30.886319 material_zui-0.1.3/src/material_zui/fake/__init__.py
+-rw-r--r--   0        0        0       62 2023-05-19 02:24:23.295278 material_zui-0.1.3/src/material_zui/fake/index.py
+-rw-r--r--   0        0        0      254 2023-05-21 05:39:54.079978 material_zui-0.1.3/src/material_zui/fake/number.py
+-rw-r--r--   0        0        0       21 2023-06-24 01:47:34.605558 material_zui-0.1.3/src/material_zui/file/__init__.py
+-rw-r--r--   0        0        0      551 2023-06-23 07:37:11.257875 material_zui-0.1.3/src/material_zui/file/check.py
+-rw-r--r--   0        0        0     2115 2023-06-15 03:25:12.103320 material_zui-0.1.3/src/material_zui/file/common.py
+-rw-r--r--   0        0        0      304 2023-06-15 03:25:12.271318 material_zui-0.1.3/src/material_zui/file/download.py
+-rw-r--r--   0        0        0     2051 2023-06-24 03:27:30.253159 material_zui-0.1.3/src/material_zui/file/excel.py
+-rw-r--r--   0        0        0      353 2023-06-25 14:02:51.225505 material_zui-0.1.3/src/material_zui/file/index.py
+-rw-r--r--   0        0        0     1757 2023-06-27 02:48:30.793448 material_zui-0.1.3/src/material_zui/file/read.py
+-rw-r--r--   0        0        0      430 2023-06-24 05:09:30.541040 material_zui-0.1.3/src/material_zui/file/type.py
+-rw-r--r--   0        0        0      992 2023-06-23 08:03:07.838708 material_zui-0.1.3/src/material_zui/file/write.py
+-rw-r--r--   0        0        0       21 2023-06-27 03:03:29.674154 material_zui-0.1.3/src/material_zui/generate/__init__.py
+-rw-r--r--   0        0        0     2103 2023-06-27 07:23:41.480905 material_zui-0.1.3/src/material_zui/generate/common.py
+-rw-r--r--   0        0        0       22 2023-06-27 03:05:13.513527 material_zui-0.1.3/src/material_zui/generate/index.py
+-rw-r--r--   0        0        0       37 2023-05-25 02:02:05.757233 material_zui-0.1.3/src/material_zui/gpt/__init__.py
+-rw-r--r--   0        0        0     1048 2023-05-25 02:22:20.028251 material_zui-0.1.3/src/material_zui/gpt/gpt_vietnam.py
+-rw-r--r--   0        0        0       63 2023-05-25 02:22:19.960250 material_zui-0.1.3/src/material_zui/gpt/index.py
+-rw-r--r--   0        0        0      216 2023-05-11 09:54:07.451440 material_zui-0.1.3/src/material_zui/image/__init__.py
+-rw-r--r--   0        0        0     2199 2023-05-05 09:48:58.874264 material_zui-0.1.3/src/material_zui/image/colorization.py
+-rw-r--r--   0        0        0     2921 2023-05-11 09:52:23.138728 material_zui-0.1.3/src/material_zui/image/combine.py
+-rw-r--r--   0        0        0     7057 2023-05-28 04:11:03.932782 material_zui-0.1.3/src/material_zui/image/common.py
+-rw-r--r--   0        0        0     2808 2023-05-11 10:13:26.444992 material_zui-0.1.3/src/material_zui/image/convert.py
+-rw-r--r--   0        0        0       78 2023-05-06 06:26:57.697131 material_zui-0.1.3/src/material_zui/image/data.py
+-rw-r--r--   0        0        0      490 2023-05-28 04:11:04.028780 material_zui-0.1.3/src/material_zui/image/index.py
+-rw-r--r--   0        0        0     9945 2023-05-05 03:49:43.138352 material_zui-0.1.3/src/material_zui/image/model/colorization_deploy_v2.prototxt
+-rw-r--r--   0        0        0     5088 2023-05-05 03:49:53.225773 material_zui-0.1.3/src/material_zui/image/model/pts_in_hull.npy
+-rw-r--r--   0        0        0      782 2023-05-11 04:50:18.808963 material_zui-0.1.3/src/material_zui/image/remove_background.py
+-rw-r--r--   0        0        0     6445 2023-05-06 08:59:41.215230 material_zui-0.1.3/src/material_zui/image/to_svg.py
+-rw-r--r--   0        0        0      520 2023-05-11 09:48:54.829117 material_zui-0.1.3/src/material_zui/image/transparent_background.py
+-rw-r--r--   0        0        0      249 2023-04-28 09:24:02.020353 material_zui-0.1.3/src/material_zui/image/type.py
+-rw-r--r--   0        0        0     4779 2023-05-11 10:15:27.410813 material_zui-0.1.3/src/material_zui/image/upscale.py
+-rw-r--r--   0        0        0       38 2023-05-22 04:09:03.922071 material_zui-0.1.3/src/material_zui/list/__init__.py
+-rw-r--r--   0        0        0     2916 2023-06-18 14:13:03.127264 material_zui-0.1.3/src/material_zui/list/common.py
+-rw-r--r--   0        0        0       92 2023-06-13 09:15:39.330734 material_zui-0.1.3/src/material_zui/list/index.py
+-rw-r--r--   0        0        0       37 2023-04-30 11:48:06.179161 material_zui-0.1.3/src/material_zui/log/__init__.py
+-rw-r--r--   0        0        0       83 2023-05-11 10:20:42.114888 material_zui-0.1.3/src/material_zui/log/index.py
+-rw-r--r--   0        0        0      559 2023-05-11 10:19:34.415566 material_zui-0.1.3/src/material_zui/log/log.py
+-rw-r--r--   0        0        0       21 2023-06-13 09:33:05.320819 material_zui-0.1.3/src/material_zui/number/__init__.py
+-rw-r--r--   0        0        0      364 2023-06-13 10:11:32.006838 material_zui-0.1.3/src/material_zui/number/common.py
+-rw-r--r--   0        0        0       47 2023-06-13 09:40:32.023908 material_zui-0.1.3/src/material_zui/number/index.py
+-rw-r--r--   0        0        0       36 2023-05-20 14:09:01.119097 material_zui-0.1.3/src/material_zui/os/__init__.py
+-rw-r--r--   0        0        0       83 2023-06-16 02:02:57.672095 material_zui-0.1.3/src/material_zui/os/index.py
+-rw-r--r--   0        0        0      840 2023-06-15 03:40:00.119319 material_zui-0.1.3/src/material_zui/os/os.py
+-rw-r--r--   0        0        0     1213 2023-06-23 08:04:27.953396 material_zui-0.1.3/src/material_zui/readme.md
+-rw-r--r--   0        0        0       39 2023-05-02 05:15:13.799596 material_zui-0.1.3/src/material_zui/regex/__init__.py
+-rw-r--r--   0        0        0     5344 2023-05-02 05:18:47.668155 material_zui-0.1.3/src/material_zui/regex/index.py
+-rw-r--r--   0        0        0       43 2023-04-30 11:47:27.662335 material_zui-0.1.3/src/material_zui/replicate/__init__.py
+-rw-r--r--   0        0        0     2481 2023-05-01 15:33:18.205379 material_zui-0.1.3/src/material_zui/replicate/index.py
+-rw-r--r--   0        0        0       42 2023-05-18 03:46:44.861073 material_zui-0.1.3/src/material_zui/selenium/__init__.py
+-rw-r--r--   0        0        0     6709 2023-06-25 13:43:29.275206 material_zui-0.1.3/src/material_zui/selenium/chrome.py
+-rw-r--r--   0        0        0      257 2023-05-22 02:03:22.582766 material_zui-0.1.3/src/material_zui/selenium/common.py
+-rw-r--r--   0        0        0      120 2023-05-22 02:03:54.393486 material_zui-0.1.3/src/material_zui/selenium/index.py
+-rw-r--r--   0        0        0      895 2023-05-11 10:31:29.010961 material_zui-0.1.3/src/material_zui/setup.py
+-rw-r--r--   0        0        0       40 2023-06-10 10:50:13.743103 material_zui-0.1.3/src/material_zui/string/__init__.py
+-rw-r--r--   0        0        0     2802 2023-06-18 14:03:40.774857 material_zui-0.1.3/src/material_zui/string/common.py
+-rw-r--r--   0        0        0      135 2023-06-14 08:12:20.153192 material_zui-0.1.3/src/material_zui/string/index.py
+-rw-r--r--   0        0        0       46 2023-05-02 13:44:38.645684 material_zui-0.1.3/src/material_zui/telegram_bot/__init__.py
+-rw-r--r--   0        0        0      432 2023-05-07 05:43:32.880583 material_zui-0.1.3/src/material_zui/telegram_bot/index.py
+-rw-r--r--   0        0        0       23 2023-06-12 02:21:47.852520 material_zui-0.1.3/src/material_zui/tmp/__init__.py
+-rw-r--r--   0        0        0       24 2023-06-12 02:21:47.776537 material_zui-0.1.3/src/material_zui/tmp/index.py
+-rw-r--r--   0        0        0       41 2023-06-11 03:35:54.474267 material_zui-0.1.3/src/material_zui/utility/__init__.py
+-rw-r--r--   0        0        0      888 2023-06-11 04:23:19.200816 material_zui-0.1.3/src/material_zui/utility/common.py
+-rw-r--r--   0        0        0       56 2023-06-11 04:21:30.408379 material_zui-0.1.3/src/material_zui/utility/index.py
+-rw-r--r--   0        0        0       42 2023-05-25 02:32:34.010325 material_zui-0.1.3/src/material_zui/validate/__init__.py
+-rw-r--r--   0        0        0      308 2023-05-28 04:05:43.248601 material_zui-0.1.3/src/material_zui/validate/common.py
+-rw-r--r--   0        0        0       65 2023-05-27 14:15:24.849747 material_zui-0.1.3/src/material_zui/validate/index.py
+-rw-r--r--   0        0        0     2821 1970-01-01 00:00:00.000000 material_zui-0.1.3/PKG-INFO
```

### Comparing `material_zui-0.1.2/pyproject.toml` & `material_zui-0.1.3/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [tool.poetry]
 name = "material_zui"
-version = "0.1.2"
+version = "0.1.3"
 description = "Material Zui"
 authors = ["chauhmnguyen <chauhoangminhnguyen@gmail.com>"]
 readme = "src/material_zui/readme.md"
 keywords = [
 	"material",
 	"zui",
 	"material zui",
 	"zui material"
 ]
 include = ["src/material_zui/*"]
-exclude = ["src/material_zui/image/model/colorization_release_v2.caffemodel"]
+exclude = ["src/material_zui/automation/*", "src/material_zui/image/model/colorization_release_v2.caffemodel"]
 
 [tool.poetry.dependencies]
 python = "~3.10"
 opencv-python = "^4.7.0.72"
 pillow = "^9.5.0"
 matplotlib = "^3.7.1"
 flask = "^2.3.2"
@@ -33,16 +33,20 @@
 selenium = "^4.9.1"
 selenium-browser = "^0.0.15"
 webdriver-manager = "^3.8.6"
 beautifulsoup4 = "^4.12.2"
 pytube = "^15.0.0"
 newspaper3k = "^0.2.8"
 validators = "^0.20.0"
-edgegpt = "^0.10.7"
+edgegpt = "^0.11.6"
 setuptools = "^67.8.0"
+xlsxwriter = "^3.1.2"
+youtube-dl = "^2021.12.17"
+langchain = "^0.0.216"
+huggingface-hub = "^0.15.1"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.3.2"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `material_zui-0.1.2/src/material_zui/ResizeImage.py` & `material_zui-0.1.3/src/material_zui/ResizeImage.py`

 * *Files identical despite different names*

### Comparing `material_zui-0.1.2/src/material_zui/bard/google_bard.py` & `material_zui-0.1.3/src/material_zui/bard/google_bard.py`

 * *Files identical despite different names*

### Comparing `material_zui-0.1.2/src/material_zui/bing_ai/result.py` & `material_zui-0.1.3/src/material_zui/bing_ai/result.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import Any
 
 from material_zui.list import map_to, filter_to
 from material_zui.string import not_empty
 
 
 class ZuiBingAiResult():
-    def __init__(self, response: dict[Any, Any]):
+    def __init__(self, response: dict[Any, Any]) -> None:
         self.response = response
 
     def get_valid_message(self, messages: list[str]) -> list[str]:
         return filter_to(messages, lambda text, _: not_empty(text))
 
     @property
     def full_texts(self) -> list[str]:
@@ -18,7 +18,11 @@
         return self.get_valid_message(texts)
 
     @property
     def texts(self) -> list[str]:
         texts: list[str] = map_to(self.response["item"]["messages"],
                                   lambda message, _: message.get('text'))
         return self.get_valid_message(texts)
+
+    @property
+    def last_text(self) -> str:
+        return self.texts.pop()
```

### Comparing `material_zui-0.1.2/src/material_zui/compress/text.py` & `material_zui-0.1.3/src/material_zui/compress/text.py`

 * *Files identical despite different names*

### Comparing `material_zui-0.1.2/src/material_zui/crawl/image.py` & `material_zui-0.1.3/src/material_zui/crawl/image.py`

 * *Files identical despite different names*

### Comparing `material_zui-0.1.2/src/material_zui/crontab/index.py` & `material_zui-0.1.3/src/material_zui/crontab/index.py`

 * *Files identical despite different names*

### Comparing `material_zui-0.1.2/src/material_zui/date_time/time.py` & `material_zui-0.1.3/src/material_zui/date_time/time.py`

 * *Files identical despite different names*

### Comparing `material_zui-0.1.2/src/material_zui/file/check.py` & `material_zui-0.1.3/src/material_zui/file/check.py`

 * *Files identical despite different names*

### Comparing `material_zui-0.1.2/src/material_zui/file/common.py` & `material_zui-0.1.3/src/material_zui/file/common.py`

 * *Files identical despite different names*

### Comparing `material_zui-0.1.2/src/material_zui/file/read.py` & `material_zui-0.1.3/src/material_zui/file/read.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 from collections import defaultdict
 import json
 from typing import DefaultDict
 from pyparsing import Any
 
+from .write import write_to_last
+from material_zui.list import get_diff
 from material_zui.string import remove_all
 from material_zui.utility import pipe_list
 
 
 def read_file_to_list(filename: str) -> list[str]:
     with open(filename, "r") as f:
         lines = f.readlines()
@@ -31,8 +33,24 @@
     '''
     with open(json_file_path, "r") as f:
         data = json.load(f)
     return list(data)
 
 
 def read_json(json_file_path: str):
+    '''
+    Read json file and return content value
+    @return: `dict` for json object, otherwise `list dict` for json array
+    - ex: using: `data[0]` or `data['field_value']`
+    '''
     return json.loads(open(json_file_path, encoding="utf-8").read())
+
+
+def load_diff_line(file_urls_path: str, input_urls: list[str], is_write_file: bool = False) -> list[str]:
+    saved_urls = read_file_to_list(file_urls_path)
+    diff_urls = get_diff(input_urls, saved_urls)
+    print("New lines", len(diff_urls))
+    print("Duplicate lines", len(input_urls)-len(diff_urls))
+    if is_write_file:
+        write_to_last(file_urls_path, '\n---New lines---\n' +
+                      "\n".join(diff_urls))
+    return diff_urls
```

### Comparing `material_zui-0.1.2/src/material_zui/file/write.py` & `material_zui-0.1.3/src/material_zui/file/write.py`

 * *Files identical despite different names*

### Comparing `material_zui-0.1.2/src/material_zui/gpt/gpt_vietnam.py` & `material_zui-0.1.3/src/material_zui/gpt/gpt_vietnam.py`

 * *Files identical despite different names*

### Comparing `material_zui-0.1.2/src/material_zui/image/colorization.py` & `material_zui-0.1.3/src/material_zui/image/colorization.py`

 * *Files identical despite different names*

### Comparing `material_zui-0.1.2/src/material_zui/image/combine.py` & `material_zui-0.1.3/src/material_zui/image/combine.py`

 * *Files identical despite different names*

### Comparing `material_zui-0.1.2/src/material_zui/image/common.py` & `material_zui-0.1.3/src/material_zui/image/common.py`

 * *Files identical despite different names*

### Comparing `material_zui-0.1.2/src/material_zui/image/convert.py` & `material_zui-0.1.3/src/material_zui/image/convert.py`

 * *Files identical despite different names*

### Comparing `material_zui-0.1.2/src/material_zui/image/model/colorization_deploy_v2.prototxt` & `material_zui-0.1.3/src/material_zui/image/model/colorization_deploy_v2.prototxt`

 * *Files identical despite different names*

### Comparing `material_zui-0.1.2/src/material_zui/image/model/pts_in_hull.npy` & `material_zui-0.1.3/src/material_zui/image/model/pts_in_hull.npy`

 * *Files identical despite different names*

### Comparing `material_zui-0.1.2/src/material_zui/image/remove_background.py` & `material_zui-0.1.3/src/material_zui/image/remove_background.py`

 * *Files identical despite different names*

### Comparing `material_zui-0.1.2/src/material_zui/image/to_svg.py` & `material_zui-0.1.3/src/material_zui/image/to_svg.py`

 * *Files identical despite different names*

### Comparing `material_zui-0.1.2/src/material_zui/image/transparent_background.py` & `material_zui-0.1.3/src/material_zui/image/transparent_background.py`

 * *Files identical despite different names*

### Comparing `material_zui-0.1.2/src/material_zui/image/upscale.py` & `material_zui-0.1.3/src/material_zui/image/upscale.py`

 * *Files identical despite different names*

### Comparing `material_zui-0.1.2/src/material_zui/list/common.py` & `material_zui-0.1.3/src/material_zui/list/common.py`

 * *Files identical despite different names*

### Comparing `material_zui-0.1.2/src/material_zui/log/log.py` & `material_zui-0.1.3/src/material_zui/log/log.py`

 * *Files identical despite different names*

### Comparing `material_zui-0.1.2/src/material_zui/os/os.py` & `material_zui-0.1.3/src/material_zui/os/os.py`

 * *Files identical despite different names*

### Comparing `material_zui-0.1.2/src/material_zui/readme.md` & `material_zui-0.1.3/src/material_zui/readme.md`

 * *Files identical despite different names*

### Comparing `material_zui-0.1.2/src/material_zui/regex/index.py` & `material_zui-0.1.3/src/material_zui/regex/index.py`

 * *Files identical despite different names*

### Comparing `material_zui-0.1.2/src/material_zui/replicate/index.py` & `material_zui-0.1.3/src/material_zui/replicate/index.py`

 * *Files identical despite different names*

### Comparing `material_zui-0.1.2/src/material_zui/selenium/chrome.py` & `material_zui-0.1.3/src/material_zui/selenium/chrome.py`

 * *Files 8% similar despite different names*

```diff
@@ -62,42 +62,48 @@
 
     def safe_find_element(
             self, by: str = By.ID,
             value: str | None = None,
             parent: Any = None) -> WebElement | None:
         '''
         This is safe find element method
-        @return `None` incase not found
+        @return `None` in case not found
         '''
         return safe_find_element(parent if parent else self.driver, by, value)
 
     def safe_find_element_by_xpath(self, xpath_value: str) -> WebElement | None:
         return self.safe_find_element(By.XPATH, xpath_value)
 
+    def find_element_by_xpath(self, xpath_value: str): return self.driver.find_element(
+        By.XPATH, xpath_value)
+
+    def find_elements_by_xpath(self, xpath_value: str): return self.driver.find_elements(
+        By.XPATH, xpath_value)
+
+    def find_elements_by_class(self, class_value: str): return self.driver.find_elements(
+        By.CLASS_NAME, class_value)
+
     def scroll_to_end(self) -> None:
         self.driver.execute_script("window.scrollTo(0, {scroll_height});".format(
             scroll_height=self.scroll_height))
 
+    def scroll(self, step_scroll: int) -> None:
+        for index in range(step_scroll):
+            print(index+1, "Scrolling to", self.scroll_height)
+            self.scroll_to_end()
+            self.delay()
+
     def get_urls(self, class_selector: str) -> list[str]:
         '''
         Get video urls by class selector of each video
         '''
         videos = self.document.find_all(
             "div", {"class": class_selector})
         return map_to(videos, lambda video, _: video.a["href"])
 
-    def find_element_by_xpath(self, xpath_value: str): return self.driver.find_element(
-        By.XPATH, xpath_value)
-
-    def find_elements_by_xpath(self, xpath_value: str): return self.driver.find_elements(
-        By.XPATH, xpath_value)
-
-    def find_elements_by_class(self, class_value: str): return self.driver.find_elements(
-        By.CLASS_NAME, class_value)
-
     def switch_to_frame(self, xpath_value: str) -> None:
         '''
         @xpath_value: must be end with `frame/iframe` like `//*[@id="main"]/div[2]/div/iframe`
         '''
         frame_element = self.find_element_by_xpath(xpath_value)
         self.driver.switch_to.frame(frame_element)
 
@@ -126,30 +132,40 @@
             element = self.safe_find_element_by_xpath(xpath_value)
             if element:
                 element.click()
             return element
         except:
             return None
 
-    def send_keys(self, xpath_value: str, key_value: str, clear_before_send_keys: bool = True):
+    def send_keys(self, xpath_value: str, key_value: str, clear_before_send_keys: bool = True, delay_time: int = 10):
         '''
         Send keys then return that element
         @xpath_value: only valid with element selector can input value
         @clear_before_send_keys:
         - True: clear input before send keys
         - False: value will input after existed value
         '''
         # element = self.find_element_by_xpath(xpath_value)
-        element = self.wait_get(xpath_value)
+        element = self.wait_get(xpath_value, delay_time)
         element.click()
         if clear_before_send_keys:
             element.send_keys(Keys.CONTROL + 'a')
             element.send_keys(Keys.BACKSPACE)
         element.send_keys(key_value)
         return element
 
-    def wait_get(self, xpath_value: str, delay_time: int = 10) -> WebElement:
-        element: Any = WebDriverWait(self.driver, delay_time).until(  # using explicit wait for 10 seconds
+    # def wait_get(self, xpath_value: str, delay_time: int = 10) -> WebElement:
+    #     element: Any = WebDriverWait(self.driver, delay_time).until(  # using explicit wait for 10 seconds
+    #         EC.presence_of_element_located(
+    #             (By.XPATH, xpath_value))  # finding the element
+    #     )
+    #     return element
+    def wait_get(self, xpath_value: str, delay_time: int = 10, time_to_try: int = 10) -> WebElement:
+        for _ in range(time_to_try):
+            element = self.safe_find_element_by_xpath(xpath_value)
+            if element:
+                return element
+            self.delay(delay_time)
+        return WebDriverWait(self.driver, delay_time).until(  # using explicit wait for 10 seconds
             EC.presence_of_element_located(
                 (By.XPATH, xpath_value))  # finding the element
         )
-        return element
```

### Comparing `material_zui-0.1.2/src/material_zui/setup.py` & `material_zui-0.1.3/src/material_zui/setup.py`

 * *Files identical despite different names*

### Comparing `material_zui-0.1.2/src/material_zui/string/common.py` & `material_zui-0.1.3/src/material_zui/string/common.py`

 * *Files identical despite different names*

### Comparing `material_zui-0.1.2/src/material_zui/utility/common.py` & `material_zui-0.1.3/src/material_zui/utility/common.py`

 * *Files identical despite different names*

### Comparing `material_zui-0.1.2/PKG-INFO` & `material_zui-0.1.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 Metadata-Version: 2.1
 Name: material-zui
-Version: 0.1.2
+Version: 0.1.3
 Summary: Material Zui
 Keywords: material,zui,material zui,zui material
 Author: chauhmnguyen
 Author-email: chauhoangminhnguyen@gmail.com
 Requires-Python: >=3.10,<3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: bardapi (>=0.1.2,<0.2.0)
 Requires-Dist: beautifulsoup4 (>=4.12.2,<5.0.0)
-Requires-Dist: edgegpt (>=0.10.7,<0.11.0)
+Requires-Dist: edgegpt (>=0.11.6,<0.12.0)
 Requires-Dist: flask (>=2.3.2,<3.0.0)
+Requires-Dist: huggingface-hub (>=0.15.1,<0.16.0)
+Requires-Dist: langchain (>=0.0.216,<0.0.217)
 Requires-Dist: matplotlib (>=3.7.1,<4.0.0)
 Requires-Dist: multipledispatch (>=0.6.0,<0.7.0)
 Requires-Dist: newspaper3k (>=0.2.8,<0.3.0)
 Requires-Dist: numpy (>=1.24.3,<2.0.0)
 Requires-Dist: opencv-python (>=4.7.0.72,<5.0.0.0)
 Requires-Dist: pandas (>=2.0.1,<3.0.0)
 Requires-Dist: pillow (>=9.5.0,<10.0.0)
@@ -28,14 +30,16 @@
 Requires-Dist: replicate (>=0.8.1,<0.9.0)
 Requires-Dist: requests (>=2.30.0,<3.0.0)
 Requires-Dist: selenium (>=4.9.1,<5.0.0)
 Requires-Dist: selenium-browser (>=0.0.15,<0.0.16)
 Requires-Dist: setuptools (>=67.8.0,<68.0.0)
 Requires-Dist: validators (>=0.20.0,<0.21.0)
 Requires-Dist: webdriver-manager (>=3.8.6,<4.0.0)
+Requires-Dist: xlsxwriter (>=3.1.2,<4.0.0)
+Requires-Dist: youtube-dl (>=2021.12.17,<2022.0.0)
 Description-Content-Type: text/markdown
 
 # Modules
 
 <ol>
   <!-- <li>automation</li> -->
   <li>bard</li>
```

#### html2text {}

```diff
@@ -1,27 +1,29 @@
-Metadata-Version: 2.1 Name: material-zui Version: 0.1.2 Summary: Material Zui
+Metadata-Version: 2.1 Name: material-zui Version: 0.1.3 Summary: Material Zui
 Keywords: material,zui,material zui,zui material Author: chauhmnguyen Author-
 email: chauhoangminhnguyen@gmail.com Requires-Python: >=3.10,<3.11 Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.10 Requires-Dist: bardapi (>=0.1.2,<0.2.0) Requires-Dist: beautifulsoup4
-(>=4.12.2,<5.0.0) Requires-Dist: edgegpt (>=0.10.7,<0.11.0) Requires-Dist:
-flask (>=2.3.2,<3.0.0) Requires-Dist: matplotlib (>=3.7.1,<4.0.0) Requires-
-Dist: multipledispatch (>=0.6.0,<0.7.0) Requires-Dist: newspaper3k
-(>=0.2.8,<0.3.0) Requires-Dist: numpy (>=1.24.3,<2.0.0) Requires-Dist: opencv-
-python (>=4.7.0.72,<5.0.0.0) Requires-Dist: pandas (>=2.0.1,<3.0.0) Requires-
-Dist: pillow (>=9.5.0,<10.0.0) Requires-Dist: pytelegrambotapi
-(>=4.11.0,<5.0.0) Requires-Dist: python-crontab (>=2.7.1,<3.0.0) Requires-Dist:
-python-dotenv (>=1.0.0,<2.0.0) Requires-Dist: pythonlangutil (>=0.1,<0.2)
-Requires-Dist: pytube (>=15.0.0,<16.0.0) Requires-Dist: rembg (>=2.0.36,<3.0.0)
-Requires-Dist: replicate (>=0.8.1,<0.9.0) Requires-Dist: requests
-(>=2.30.0,<3.0.0) Requires-Dist: selenium (>=4.9.1,<5.0.0) Requires-Dist:
-selenium-browser (>=0.0.15,<0.0.16) Requires-Dist: setuptools
-(>=67.8.0,<68.0.0) Requires-Dist: validators (>=0.20.0,<0.21.0) Requires-Dist:
-webdriver-manager (>=3.8.6,<4.0.0) Description-Content-Type: text/markdown #
-Modules
+(>=4.12.2,<5.0.0) Requires-Dist: edgegpt (>=0.11.6,<0.12.0) Requires-Dist:
+flask (>=2.3.2,<3.0.0) Requires-Dist: huggingface-hub (>=0.15.1,<0.16.0)
+Requires-Dist: langchain (>=0.0.216,<0.0.217) Requires-Dist: matplotlib
+(>=3.7.1,<4.0.0) Requires-Dist: multipledispatch (>=0.6.0,<0.7.0) Requires-
+Dist: newspaper3k (>=0.2.8,<0.3.0) Requires-Dist: numpy (>=1.24.3,<2.0.0)
+Requires-Dist: opencv-python (>=4.7.0.72,<5.0.0.0) Requires-Dist: pandas
+(>=2.0.1,<3.0.0) Requires-Dist: pillow (>=9.5.0,<10.0.0) Requires-Dist:
+pytelegrambotapi (>=4.11.0,<5.0.0) Requires-Dist: python-crontab
+(>=2.7.1,<3.0.0) Requires-Dist: python-dotenv (>=1.0.0,<2.0.0) Requires-Dist:
+pythonlangutil (>=0.1,<0.2) Requires-Dist: pytube (>=15.0.0,<16.0.0) Requires-
+Dist: rembg (>=2.0.36,<3.0.0) Requires-Dist: replicate (>=0.8.1,<0.9.0)
+Requires-Dist: requests (>=2.30.0,<3.0.0) Requires-Dist: selenium
+(>=4.9.1,<5.0.0) Requires-Dist: selenium-browser (>=0.0.15,<0.0.16) Requires-
+Dist: setuptools (>=67.8.0,<68.0.0) Requires-Dist: validators
+(>=0.20.0,<0.21.0) Requires-Dist: webdriver-manager (>=3.8.6,<4.0.0) Requires-
+Dist: xlsxwriter (>=3.1.2,<4.0.0) Requires-Dist: youtube-dl
+(>=2021.12.17,<2022.0.0) Description-Content-Type: text/markdown # Modules
    1. bard
    2. bing_ai
    3. compress
    4. crawl
    5. crontab
    6. date_time
    7. env
```

