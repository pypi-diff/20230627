# Comparing `tmp/deepsecrets-1.0.5.tar.gz` & `tmp/deepsecrets-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deepsecrets-1.0.5.tar", max compression
+gzip compressed data, was "deepsecrets-1.0.6.tar", max compression
```

## Comparing `deepsecrets-1.0.5.tar` & `deepsecrets-1.0.6.tar`

### file list

```diff
@@ -1,146 +1,146 @@
--rw-r--r--   0        0        0     1061 2023-03-27 10:35:08.129343 deepsecrets-1.0.5/LICENSE
--rw-r--r--   0        0        0     5013 2023-04-28 10:40:14.241731 deepsecrets-1.0.5/README.md
--rw-r--r--   0        0        0     8196 2023-03-28 08:59:04.340095 deepsecrets-1.0.5/deepsecrets/.DS_Store
--rw-r--r--   0        0        0      674 2023-04-27 13:31:17.046975 deepsecrets-1.0.5/deepsecrets/__init__.py
--rw-r--r--   0        0        0      107 2023-04-27 13:10:21.769450 deepsecrets-1.0.5/deepsecrets/__main__.py
--rw-r--r--   0        0        0     6429 2023-04-28 06:49:11.562918 deepsecrets-1.0.5/deepsecrets/cli.py
--rw-r--r--   0        0        0     1675 2023-04-17 13:19:49.920625 deepsecrets-1.0.5/deepsecrets/config.py
--rw-r--r--   0        0        0     8196 2023-02-26 15:19:47.000000 deepsecrets-1.0.5/deepsecrets/core/.DS_Store
--rw-r--r--   0        0        0        0 2022-05-17 09:51:36.000000 deepsecrets-1.0.5/deepsecrets/core/engines/__init__.py
--rw-r--r--   0        0        0      150 2023-01-28 13:47:04.000000 deepsecrets-1.0.5/deepsecrets/core/engines/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     2696 2023-04-17 12:40:25.353990 deepsecrets-1.0.5/deepsecrets/core/engines/__pycache__/hashed_secret.cpython-311.pyc
--rw-r--r--   0        0        0     2660 2023-04-17 13:34:38.819504 deepsecrets-1.0.5/deepsecrets/core/engines/__pycache__/iengine.cpython-311.pyc
--rw-r--r--   0        0        0     1992 2023-06-26 12:35:59.459732 deepsecrets-1.0.5/deepsecrets/core/engines/__pycache__/regex.cpython-311.pyc
--rw-r--r--   0        0        0     6192 2023-06-21 09:26:58.841320 deepsecrets-1.0.5/deepsecrets/core/engines/__pycache__/semantic.cpython-311.pyc
--rw-r--r--   0        0        0     1611 2023-04-17 12:40:24.547637 deepsecrets-1.0.5/deepsecrets/core/engines/hashed_secret.py
--rw-r--r--   0        0        0     1200 2023-04-17 13:34:38.199667 deepsecrets-1.0.5/deepsecrets/core/engines/iengine.py
--rw-r--r--   0        0        0     1196 2023-06-26 12:35:58.745163 deepsecrets-1.0.5/deepsecrets/core/engines/regex.py
--rw-r--r--   0        0        0     4341 2023-06-21 09:26:58.182165 deepsecrets-1.0.5/deepsecrets/core/engines/semantic.py
--rw-r--r--   0        0        0     2561 2023-02-28 16:49:26.000000 deepsecrets-1.0.5/deepsecrets/core/helpers/__pycache__/content_analyzer.cpython-311.pyc
--rw-r--r--   0        0        0     1495 2022-09-15 09:37:41.000000 deepsecrets-1.0.5/deepsecrets/core/helpers/__pycache__/content_analyzer.cpython-39.pyc
--rw-r--r--   0        0        0     2971 2023-04-14 12:50:22.603515 deepsecrets-1.0.5/deepsecrets/core/helpers/__pycache__/entropy.cpython-311.pyc
--rw-r--r--   0        0        0     1686 2022-09-15 09:36:08.000000 deepsecrets-1.0.5/deepsecrets/core/helpers/__pycache__/entropy.cpython-39.pyc
--rw-r--r--   0        0        0     1145 2023-02-28 16:18:28.000000 deepsecrets-1.0.5/deepsecrets/core/helpers/content_analyzer.py
--rw-r--r--   0        0        0     1831 2023-04-14 12:50:21.979920 deepsecrets-1.0.5/deepsecrets/core/helpers/entropy.py
--rw-r--r--   0        0        0     6148 2023-02-26 15:19:47.000000 deepsecrets-1.0.5/deepsecrets/core/model/.DS_Store
--rw-r--r--   0        0        0       82 2023-02-23 12:04:19.000000 deepsecrets-1.0.5/deepsecrets/core/model/__init__.py
--rw-r--r--   0        0        0      292 2023-02-23 12:04:20.000000 deepsecrets-1.0.5/deepsecrets/core/model/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     7459 2023-06-26 13:33:19.902788 deepsecrets-1.0.5/deepsecrets/core/model/__pycache__/file.cpython-311.pyc
--rw-r--r--   0        0        0     8418 2023-03-27 20:52:52.004543 deepsecrets-1.0.5/deepsecrets/core/model/__pycache__/finding.cpython-311.pyc
--rw-r--r--   0        0        0      695 2023-02-28 15:59:52.000000 deepsecrets-1.0.5/deepsecrets/core/model/__pycache__/semantic.cpython-311.pyc
--rw-r--r--   0        0        0     3926 2023-04-17 12:50:07.084349 deepsecrets-1.0.5/deepsecrets/core/model/__pycache__/token.cpython-311.pyc
--rw-r--r--   0        0        0     4034 2023-06-26 13:33:19.226359 deepsecrets-1.0.5/deepsecrets/core/model/file.py
--rw-r--r--   0        0        0     4374 2023-03-27 20:52:51.349485 deepsecrets-1.0.5/deepsecrets/core/model/finding.py
--rw-r--r--   0        0        0        0 2023-01-27 16:18:29.000000 deepsecrets-1.0.5/deepsecrets/core/model/rules/__init__.py
--rw-r--r--   0        0        0      154 2023-01-28 13:47:51.000000 deepsecrets-1.0.5/deepsecrets/core/model/rules/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      954 2023-02-23 12:04:24.000000 deepsecrets-1.0.5/deepsecrets/core/model/rules/__pycache__/exlcuded_path.cpython-311.pyc
--rw-r--r--   0        0        0      488 2023-04-17 13:45:18.933981 deepsecrets-1.0.5/deepsecrets/core/model/rules/__pycache__/false_finding.cpython-311.pyc
--rw-r--r--   0        0        0     2589 2023-04-17 13:06:29.025295 deepsecrets-1.0.5/deepsecrets/core/model/rules/__pycache__/hashed_secret.cpython-311.pyc
--rw-r--r--   0        0        0      510 2023-04-17 12:50:07.086386 deepsecrets-1.0.5/deepsecrets/core/model/rules/__pycache__/hashing.cpython-311.pyc
--rw-r--r--   0        0        0     5588 2023-04-14 12:57:25.499628 deepsecrets-1.0.5/deepsecrets/core/model/rules/__pycache__/regex.cpython-311.pyc
--rw-r--r--   0        0        0     2295 2023-04-14 12:57:56.098733 deepsecrets-1.0.5/deepsecrets/core/model/rules/__pycache__/rule.cpython-311.pyc
--rw-r--r--   0        0        0      269 2023-02-23 11:55:43.000000 deepsecrets-1.0.5/deepsecrets/core/model/rules/exlcuded_path.py
--rw-r--r--   0        0        0      121 2023-04-17 13:44:30.761705 deepsecrets-1.0.5/deepsecrets/core/model/rules/false_finding.py
--rw-r--r--   0        0        0     1438 2023-04-17 13:06:28.309253 deepsecrets-1.0.5/deepsecrets/core/model/rules/hashed_secret.py
--rw-r--r--   0        0        0      119 2023-04-17 12:41:47.443006 deepsecrets-1.0.5/deepsecrets/core/model/rules/hashing.py
--rw-r--r--   0        0        0     2971 2023-04-14 12:57:24.773737 deepsecrets-1.0.5/deepsecrets/core/model/rules/regex.py
--rw-r--r--   0        0        0      871 2023-04-14 12:57:55.404355 deepsecrets-1.0.5/deepsecrets/core/model/rules/rule.py
--rw-r--r--   0        0        0       88 2023-02-23 11:55:43.000000 deepsecrets-1.0.5/deepsecrets/core/model/rules/semantic.py
--rw-r--r--   0        0        0      237 2023-02-28 15:59:50.000000 deepsecrets-1.0.5/deepsecrets/core/model/semantic.py
--rw-r--r--   0        0        0     2007 2023-04-17 12:50:06.475278 deepsecrets-1.0.5/deepsecrets/core/model/token.py
--rw-r--r--   0        0        0     6148 2023-02-26 15:19:47.000000 deepsecrets-1.0.5/deepsecrets/core/modes/.DS_Store
--rw-r--r--   0        0        0     8425 2023-06-13 10:12:51.339833 deepsecrets-1.0.5/deepsecrets/core/modes/__pycache__/iscan_mode.cpython-311.pyc
--rw-r--r--   0        0        0     5157 2023-06-13 10:12:50.784613 deepsecrets-1.0.5/deepsecrets/core/modes/iscan_mode.py
--rw-r--r--   0        0        0      214 2023-01-25 14:00:27.000000 deepsecrets-1.0.5/deepsecrets/core/rulesets/__pycache__/confidence.cpython-311.pyc
--rw-r--r--   0        0        0      184 2022-09-13 14:18:23.000000 deepsecrets-1.0.5/deepsecrets/core/rulesets/__pycache__/confidence.cpython-39.pyc
--rw-r--r--   0        0        0      648 2023-02-28 15:59:52.000000 deepsecrets-1.0.5/deepsecrets/core/rulesets/__pycache__/excluded_paths.cpython-311.pyc
--rw-r--r--   0        0        0      649 2023-04-17 13:45:18.931553 deepsecrets-1.0.5/deepsecrets/core/rulesets/__pycache__/false_findings.cpython-311.pyc
--rw-r--r--   0        0        0     1424 2022-11-24 10:59:56.000000 deepsecrets-1.0.5/deepsecrets/core/rulesets/__pycache__/false_tokens.cpython-311.pyc
--rw-r--r--   0        0        0     1796 2022-01-29 06:07:43.000000 deepsecrets-1.0.5/deepsecrets/core/rulesets/__pycache__/false_tokens.cpython-38.pyc
--rw-r--r--   0        0        0     1059 2022-05-17 09:51:38.000000 deepsecrets-1.0.5/deepsecrets/core/rulesets/__pycache__/false_tokens.cpython-39.pyc
--rw-r--r--   0        0        0     2551 2023-04-17 13:11:28.556085 deepsecrets-1.0.5/deepsecrets/core/rulesets/__pycache__/hashed_secrets.cpython-311.pyc
--rw-r--r--   0        0        0     1515 2022-10-14 09:00:28.000000 deepsecrets-1.0.5/deepsecrets/core/rulesets/__pycache__/hashed_secrets.cpython-39.pyc
--rw-r--r--   0        0        0     2281 2023-02-28 16:49:26.000000 deepsecrets-1.0.5/deepsecrets/core/rulesets/__pycache__/ibuilder.cpython-311.pyc
--rw-r--r--   0        0        0     4653 2022-11-24 10:59:56.000000 deepsecrets-1.0.5/deepsecrets/core/rulesets/__pycache__/ldap_detector.cpython-311.pyc
--rw-r--r--   0        0        0     2752 2022-05-17 09:51:38.000000 deepsecrets-1.0.5/deepsecrets/core/rulesets/__pycache__/ldap_detector.cpython-39.pyc
--rw-r--r--   0        0        0      682 2023-01-28 14:26:39.000000 deepsecrets-1.0.5/deepsecrets/core/rulesets/__pycache__/path_exclusions.cpython-311.pyc
--rw-r--r--   0        0        0      821 2022-01-29 06:16:36.000000 deepsecrets-1.0.5/deepsecrets/core/rulesets/__pycache__/path_exclusions.cpython-38.pyc
--rw-r--r--   0        0        0      855 2022-10-13 11:40:21.000000 deepsecrets-1.0.5/deepsecrets/core/rulesets/__pycache__/path_exclusions.cpython-39.pyc
--rw-r--r--   0        0        0      783 2022-01-28 15:38:18.000000 deepsecrets-1.0.5/deepsecrets/core/rulesets/__pycache__/plaintext.cpython-38.pyc
--rw-r--r--   0        0        0     1661 2022-02-02 13:16:29.000000 deepsecrets-1.0.5/deepsecrets/core/rulesets/__pycache__/plaintext.cpython-39.pyc
--rw-r--r--   0        0        0      615 2023-02-28 15:59:52.000000 deepsecrets-1.0.5/deepsecrets/core/rulesets/__pycache__/regex.cpython-311.pyc
--rw-r--r--   0        0        0     2903 2022-10-13 11:43:01.000000 deepsecrets-1.0.5/deepsecrets/core/rulesets/__pycache__/regex.cpython-39.pyc
--rw-r--r--   0        0        0      250 2023-02-28 15:59:51.000000 deepsecrets-1.0.5/deepsecrets/core/rulesets/excluded_paths.py
--rw-r--r--   0        0        0      252 2023-04-17 13:45:18.253008 deepsecrets-1.0.5/deepsecrets/core/rulesets/false_findings.py
--rw-r--r--   0        0        0     1434 2023-04-17 13:11:27.888766 deepsecrets-1.0.5/deepsecrets/core/rulesets/hashed_secrets.py
--rw-r--r--   0        0        0      627 2023-02-28 16:35:44.000000 deepsecrets-1.0.5/deepsecrets/core/rulesets/ibuilder.py
--rw-r--r--   0        0        0      220 2023-02-28 15:59:51.000000 deepsecrets-1.0.5/deepsecrets/core/rulesets/regex.py
--rw-r--r--   0        0        0     6148 2023-02-26 15:19:47.000000 deepsecrets-1.0.5/deepsecrets/core/tokenizers/.DS_Store
--rw-r--r--   0        0        0      181 2023-02-23 11:55:44.000000 deepsecrets-1.0.5/deepsecrets/core/tokenizers/__init__.py
--rw-r--r--   0        0        0      366 2023-02-23 11:55:45.000000 deepsecrets-1.0.5/deepsecrets/core/tokenizers/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      129 2022-09-12 09:34:48.000000 deepsecrets-1.0.5/deepsecrets/core/tokenizers/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     1059 2023-02-15 14:21:01.000000 deepsecrets-1.0.5/deepsecrets/core/tokenizers/__pycache__/full_content.cpython-311.pyc
--rw-r--r--   0        0        0      649 2022-01-28 16:00:02.000000 deepsecrets-1.0.5/deepsecrets/core/tokenizers/__pycache__/full_content.cpython-38.pyc
--rw-r--r--   0        0        0      732 2022-10-13 14:47:47.000000 deepsecrets-1.0.5/deepsecrets/core/tokenizers/__pycache__/full_content.cpython-39.pyc
--rw-r--r--   0        0        0     1948 2023-02-28 15:59:52.000000 deepsecrets-1.0.5/deepsecrets/core/tokenizers/__pycache__/itokenizer.cpython-311.pyc
--rw-r--r--   0        0        0      520 2022-01-28 13:54:30.000000 deepsecrets-1.0.5/deepsecrets/core/tokenizers/__pycache__/itokenizer.cpython-38.pyc
--rw-r--r--   0        0        0     1549 2022-10-13 14:13:37.000000 deepsecrets-1.0.5/deepsecrets/core/tokenizers/__pycache__/itokenizer.cpython-39.pyc
--rw-r--r--   0        0        0     2569 2022-04-25 16:49:33.000000 deepsecrets-1.0.5/deepsecrets/core/tokenizers/__pycache__/lex_utils.cpython-39.pyc
--rw-r--r--   0        0        0    10200 2023-06-26 13:42:04.228723 deepsecrets-1.0.5/deepsecrets/core/tokenizers/__pycache__/lexer.cpython-311.pyc
--rw-r--r--   0        0        0     4195 2022-05-27 10:40:16.000000 deepsecrets-1.0.5/deepsecrets/core/tokenizers/__pycache__/lexer.cpython-39.pyc
--rw-r--r--   0        0        0     1482 2023-04-14 12:50:35.476023 deepsecrets-1.0.5/deepsecrets/core/tokenizers/__pycache__/per_line.cpython-311.pyc
--rw-r--r--   0        0        0      852 2022-01-28 17:43:01.000000 deepsecrets-1.0.5/deepsecrets/core/tokenizers/__pycache__/per_line.cpython-38.pyc
--rw-r--r--   0        0        0      899 2022-09-12 09:34:48.000000 deepsecrets-1.0.5/deepsecrets/core/tokenizers/__pycache__/per_line.cpython-39.pyc
--rw-r--r--   0        0        0     1723 2023-01-25 14:00:28.000000 deepsecrets-1.0.5/deepsecrets/core/tokenizers/__pycache__/per_word.cpython-311.pyc
--rw-r--r--   0        0        0      977 2022-01-28 18:09:20.000000 deepsecrets-1.0.5/deepsecrets/core/tokenizers/__pycache__/per_word.cpython-38.pyc
--rw-r--r--   0        0        0     1010 2022-09-12 09:34:48.000000 deepsecrets-1.0.5/deepsecrets/core/tokenizers/__pycache__/per_word.cpython-39.pyc
--rw-r--r--   0        0        0      349 2023-02-15 13:58:04.000000 deepsecrets-1.0.5/deepsecrets/core/tokenizers/full_content.py
--rw-r--r--   0        0        0     6148 2023-02-26 15:19:47.000000 deepsecrets-1.0.5/deepsecrets/core/tokenizers/helpers/.DS_Store
--rw-r--r--   0        0        0        0 2023-01-25 14:00:23.000000 deepsecrets-1.0.5/deepsecrets/core/tokenizers/helpers/__init__.py
--rw-r--r--   0        0        0      153 2023-01-25 14:00:28.000000 deepsecrets-1.0.5/deepsecrets/core/tokenizers/helpers/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      135 2022-09-12 09:34:48.000000 deepsecrets-1.0.5/deepsecrets/core/tokenizers/helpers/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     9952 2023-02-10 11:22:52.000000 deepsecrets-1.0.5/deepsecrets/core/tokenizers/helpers/__pycache__/lexer.cpython-311.pyc
--rw-r--r--   0        0        0     6003 2022-10-13 14:25:20.000000 deepsecrets-1.0.5/deepsecrets/core/tokenizers/helpers/__pycache__/lexer.cpython-39.pyc
--rw-r--r--   0        0        0     3663 2023-06-26 16:51:54.572701 deepsecrets-1.0.5/deepsecrets/core/tokenizers/helpers/__pycache__/spot_improvements.cpython-311.pyc
--rw-r--r--   0        0        0     2799 2023-04-21 14:40:38.036123 deepsecrets-1.0.5/deepsecrets/core/tokenizers/helpers/__pycache__/type_stream.cpython-311.pyc
--rw-r--r--   0        0        0     6148 2023-02-26 15:19:47.000000 deepsecrets-1.0.5/deepsecrets/core/tokenizers/helpers/semantic/.DS_Store
--rw-r--r--   0        0        0        0 2023-01-25 14:00:23.000000 deepsecrets-1.0.5/deepsecrets/core/tokenizers/helpers/semantic/__init__.py
--rw-r--r--   0        0        0      162 2023-01-25 14:00:28.000000 deepsecrets-1.0.5/deepsecrets/core/tokenizers/helpers/semantic/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      144 2022-09-12 10:58:48.000000 deepsecrets-1.0.5/deepsecrets/core/tokenizers/helpers/semantic/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     1353 2023-04-13 12:42:45.606082 deepsecrets-1.0.5/deepsecrets/core/tokenizers/helpers/semantic/__pycache__/language.cpython-311.pyc
--rw-r--r--   0        0        0     2684 2022-06-08 15:19:48.000000 deepsecrets-1.0.5/deepsecrets/core/tokenizers/helpers/semantic/__pycache__/python.cpython-39.pyc
--rw-r--r--   0        0        0    10645 2023-02-10 11:00:04.000000 deepsecrets-1.0.5/deepsecrets/core/tokenizers/helpers/semantic/__pycache__/variable_detection.cpython-311.pyc
--rw-r--r--   0        0        0     4836 2022-10-13 14:38:14.000000 deepsecrets-1.0.5/deepsecrets/core/tokenizers/helpers/semantic/__pycache__/variable_detection.cpython-39.pyc
--rw-r--r--   0        0        0      529 2023-04-13 12:42:44.862774 deepsecrets-1.0.5/deepsecrets/core/tokenizers/helpers/semantic/language.py
--rw-r--r--   0        0        0        0 2023-02-10 15:56:26.000000 deepsecrets-1.0.5/deepsecrets/core/tokenizers/helpers/semantic/var_detection/__init__.py
--rw-r--r--   0        0        0      184 2023-02-10 15:56:27.000000 deepsecrets-1.0.5/deepsecrets/core/tokenizers/helpers/semantic/var_detection/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     5347 2023-04-14 13:00:04.497720 deepsecrets-1.0.5/deepsecrets/core/tokenizers/helpers/semantic/var_detection/__pycache__/detector.cpython-311.pyc
--rw-r--r--   0        0        0     6476 2023-04-14 13:10:20.748746 deepsecrets-1.0.5/deepsecrets/core/tokenizers/helpers/semantic/var_detection/__pycache__/rules.cpython-311.pyc
--rw-r--r--   0        0        0     2711 2023-04-14 13:00:03.807886 deepsecrets-1.0.5/deepsecrets/core/tokenizers/helpers/semantic/var_detection/detector.py
--rw-r--r--   0        0        0     5781 2023-04-14 13:10:20.026707 deepsecrets-1.0.5/deepsecrets/core/tokenizers/helpers/semantic/var_detection/rules.py
--rw-r--r--   0        0        0     2115 2023-06-26 16:51:53.987615 deepsecrets-1.0.5/deepsecrets/core/tokenizers/helpers/spot_improvements.py
--rw-r--r--   0        0        0     1801 2023-04-21 14:40:37.153608 deepsecrets-1.0.5/deepsecrets/core/tokenizers/helpers/type_stream.py
--rw-r--r--   0        0        0      735 2023-02-28 15:59:51.000000 deepsecrets-1.0.5/deepsecrets/core/tokenizers/itokenizer.py
--rw-r--r--   0        0        0     6481 2023-06-26 13:42:02.632935 deepsecrets-1.0.5/deepsecrets/core/tokenizers/lexer.py
--rw-r--r--   0        0        0      600 2023-04-14 12:50:34.810801 deepsecrets-1.0.5/deepsecrets/core/tokenizers/per_line.py
--rw-r--r--   0        0        0     1022 2023-04-14 12:50:38.878506 deepsecrets-1.0.5/deepsecrets/core/tokenizers/per_word.py
--rw-r--r--   0        0        0     6148 2023-02-26 15:19:47.000000 deepsecrets-1.0.5/deepsecrets/core/utils/.DS_Store
--rw-r--r--   0        0        0        0 2019-08-30 09:25:52.000000 deepsecrets-1.0.5/deepsecrets/core/utils/__init__.py
--rw-r--r--   0        0        0      148 2023-02-10 10:44:34.000000 deepsecrets-1.0.5/deepsecrets/core/utils/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      586 2023-02-28 15:32:35.000000 deepsecrets-1.0.5/deepsecrets/core/utils/__pycache__/exceptions.cpython-311.pyc
--rw-r--r--   0        0        0     5469 2023-03-27 20:23:09.183623 deepsecrets-1.0.5/deepsecrets/core/utils/__pycache__/file_analyzer.cpython-311.pyc
--rw-r--r--   0        0        0     1415 2023-02-28 16:49:26.000000 deepsecrets-1.0.5/deepsecrets/core/utils/__pycache__/fs.cpython-311.pyc
--rw-r--r--   0        0        0     1841 2023-06-26 16:37:09.047505 deepsecrets-1.0.5/deepsecrets/core/utils/__pycache__/guess_filetype.cpython-311.pyc
--rw-r--r--   0        0        0     1774 2023-04-17 12:50:07.088140 deepsecrets-1.0.5/deepsecrets/core/utils/__pycache__/hashing.cpython-311.pyc
--rw-r--r--   0        0        0      100 2023-02-28 15:32:34.000000 deepsecrets-1.0.5/deepsecrets/core/utils/exceptions.py
--rw-r--r--   0        0        0     3018 2023-03-27 20:23:08.288214 deepsecrets-1.0.5/deepsecrets/core/utils/file_analyzer.py
--rw-r--r--   0        0        0      517 2023-02-28 16:47:36.000000 deepsecrets-1.0.5/deepsecrets/core/utils/fs.py
--rw-r--r--   0        0        0     1060 2023-06-26 16:37:08.518447 deepsecrets-1.0.5/deepsecrets/core/utils/guess_filetype.py
--rw-r--r--   0        0        0      771 2023-04-17 12:49:00.602766 deepsecrets-1.0.5/deepsecrets/core/utils/hashing.py
--rw-r--r--   0        0        0     2562 2023-01-29 12:25:02.000000 deepsecrets-1.0.5/deepsecrets/rules/excluded_paths.json
--rw-r--r--   0        0        0     3993 2023-06-26 12:38:43.101327 deepsecrets-1.0.5/deepsecrets/rules/regexes.json
--rw-r--r--   0        0        0     6148 2023-02-26 15:19:47.000000 deepsecrets-1.0.5/deepsecrets/scan_modes/.DS_Store
--rw-r--r--   0        0        0     5698 2023-04-17 13:42:10.557066 deepsecrets-1.0.5/deepsecrets/scan_modes/__pycache__/cli.cpython-311.pyc
--rw-r--r--   0        0        0     3268 2023-04-17 13:42:09.893195 deepsecrets-1.0.5/deepsecrets/scan_modes/cli.py
--rw-r--r--   0        0        0     1646 2023-06-26 16:56:53.909334 deepsecrets-1.0.5/pyproject.toml
--rw-r--r--   0        0        0     6148 1970-01-01 00:00:00.000000 deepsecrets-1.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1061 2023-03-27 10:35:08.129343 deepsecrets-1.0.6/LICENSE
+-rw-r--r--   0        0        0     5013 2023-04-28 10:40:14.241731 deepsecrets-1.0.6/README.md
+-rw-r--r--   0        0        0     8196 2023-03-28 08:59:04.340095 deepsecrets-1.0.6/deepsecrets/.DS_Store
+-rw-r--r--   0        0        0      674 2023-04-27 13:31:17.046975 deepsecrets-1.0.6/deepsecrets/__init__.py
+-rw-r--r--   0        0        0      107 2023-04-27 13:10:21.769450 deepsecrets-1.0.6/deepsecrets/__main__.py
+-rw-r--r--   0        0        0     6429 2023-04-28 06:49:11.562918 deepsecrets-1.0.6/deepsecrets/cli.py
+-rw-r--r--   0        0        0     1675 2023-04-17 13:19:49.920625 deepsecrets-1.0.6/deepsecrets/config.py
+-rw-r--r--   0        0        0     8196 2023-02-26 15:19:47.000000 deepsecrets-1.0.6/deepsecrets/core/.DS_Store
+-rw-r--r--   0        0        0        0 2022-05-17 09:51:36.000000 deepsecrets-1.0.6/deepsecrets/core/engines/__init__.py
+-rw-r--r--   0        0        0      150 2023-01-28 13:47:04.000000 deepsecrets-1.0.6/deepsecrets/core/engines/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     2696 2023-04-17 12:40:25.353990 deepsecrets-1.0.6/deepsecrets/core/engines/__pycache__/hashed_secret.cpython-311.pyc
+-rw-r--r--   0        0        0     2660 2023-04-17 13:34:38.819504 deepsecrets-1.0.6/deepsecrets/core/engines/__pycache__/iengine.cpython-311.pyc
+-rw-r--r--   0        0        0     1992 2023-06-26 12:35:59.459732 deepsecrets-1.0.6/deepsecrets/core/engines/__pycache__/regex.cpython-311.pyc
+-rw-r--r--   0        0        0     6192 2023-06-27 14:07:40.467355 deepsecrets-1.0.6/deepsecrets/core/engines/__pycache__/semantic.cpython-311.pyc
+-rw-r--r--   0        0        0     1611 2023-04-17 12:40:24.547637 deepsecrets-1.0.6/deepsecrets/core/engines/hashed_secret.py
+-rw-r--r--   0        0        0     1200 2023-04-17 13:34:38.199667 deepsecrets-1.0.6/deepsecrets/core/engines/iengine.py
+-rw-r--r--   0        0        0     1196 2023-06-26 12:35:58.745163 deepsecrets-1.0.6/deepsecrets/core/engines/regex.py
+-rw-r--r--   0        0        0     4341 2023-06-27 14:07:39.916706 deepsecrets-1.0.6/deepsecrets/core/engines/semantic.py
+-rw-r--r--   0        0        0     2561 2023-02-28 16:49:26.000000 deepsecrets-1.0.6/deepsecrets/core/helpers/__pycache__/content_analyzer.cpython-311.pyc
+-rw-r--r--   0        0        0     1495 2022-09-15 09:37:41.000000 deepsecrets-1.0.6/deepsecrets/core/helpers/__pycache__/content_analyzer.cpython-39.pyc
+-rw-r--r--   0        0        0     2971 2023-04-14 12:50:22.603515 deepsecrets-1.0.6/deepsecrets/core/helpers/__pycache__/entropy.cpython-311.pyc
+-rw-r--r--   0        0        0     1686 2022-09-15 09:36:08.000000 deepsecrets-1.0.6/deepsecrets/core/helpers/__pycache__/entropy.cpython-39.pyc
+-rw-r--r--   0        0        0     1145 2023-02-28 16:18:28.000000 deepsecrets-1.0.6/deepsecrets/core/helpers/content_analyzer.py
+-rw-r--r--   0        0        0     1831 2023-04-14 12:50:21.979920 deepsecrets-1.0.6/deepsecrets/core/helpers/entropy.py
+-rw-r--r--   0        0        0     6148 2023-02-26 15:19:47.000000 deepsecrets-1.0.6/deepsecrets/core/model/.DS_Store
+-rw-r--r--   0        0        0       82 2023-02-23 12:04:19.000000 deepsecrets-1.0.6/deepsecrets/core/model/__init__.py
+-rw-r--r--   0        0        0      292 2023-02-23 12:04:20.000000 deepsecrets-1.0.6/deepsecrets/core/model/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     7459 2023-06-26 13:33:19.902788 deepsecrets-1.0.6/deepsecrets/core/model/__pycache__/file.cpython-311.pyc
+-rw-r--r--   0        0        0     8418 2023-03-27 20:52:52.004543 deepsecrets-1.0.6/deepsecrets/core/model/__pycache__/finding.cpython-311.pyc
+-rw-r--r--   0        0        0      695 2023-02-28 15:59:52.000000 deepsecrets-1.0.6/deepsecrets/core/model/__pycache__/semantic.cpython-311.pyc
+-rw-r--r--   0        0        0     3926 2023-04-17 12:50:07.084349 deepsecrets-1.0.6/deepsecrets/core/model/__pycache__/token.cpython-311.pyc
+-rw-r--r--   0        0        0     4034 2023-06-26 13:33:19.226359 deepsecrets-1.0.6/deepsecrets/core/model/file.py
+-rw-r--r--   0        0        0     4374 2023-03-27 20:52:51.349485 deepsecrets-1.0.6/deepsecrets/core/model/finding.py
+-rw-r--r--   0        0        0        0 2023-01-27 16:18:29.000000 deepsecrets-1.0.6/deepsecrets/core/model/rules/__init__.py
+-rw-r--r--   0        0        0      154 2023-01-28 13:47:51.000000 deepsecrets-1.0.6/deepsecrets/core/model/rules/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      954 2023-02-23 12:04:24.000000 deepsecrets-1.0.6/deepsecrets/core/model/rules/__pycache__/exlcuded_path.cpython-311.pyc
+-rw-r--r--   0        0        0      488 2023-04-17 13:45:18.933981 deepsecrets-1.0.6/deepsecrets/core/model/rules/__pycache__/false_finding.cpython-311.pyc
+-rw-r--r--   0        0        0     2589 2023-04-17 13:06:29.025295 deepsecrets-1.0.6/deepsecrets/core/model/rules/__pycache__/hashed_secret.cpython-311.pyc
+-rw-r--r--   0        0        0      510 2023-04-17 12:50:07.086386 deepsecrets-1.0.6/deepsecrets/core/model/rules/__pycache__/hashing.cpython-311.pyc
+-rw-r--r--   0        0        0     5588 2023-04-14 12:57:25.499628 deepsecrets-1.0.6/deepsecrets/core/model/rules/__pycache__/regex.cpython-311.pyc
+-rw-r--r--   0        0        0     2295 2023-04-14 12:57:56.098733 deepsecrets-1.0.6/deepsecrets/core/model/rules/__pycache__/rule.cpython-311.pyc
+-rw-r--r--   0        0        0      269 2023-02-23 11:55:43.000000 deepsecrets-1.0.6/deepsecrets/core/model/rules/exlcuded_path.py
+-rw-r--r--   0        0        0      121 2023-04-17 13:44:30.761705 deepsecrets-1.0.6/deepsecrets/core/model/rules/false_finding.py
+-rw-r--r--   0        0        0     1438 2023-04-17 13:06:28.309253 deepsecrets-1.0.6/deepsecrets/core/model/rules/hashed_secret.py
+-rw-r--r--   0        0        0      119 2023-04-17 12:41:47.443006 deepsecrets-1.0.6/deepsecrets/core/model/rules/hashing.py
+-rw-r--r--   0        0        0     2971 2023-04-14 12:57:24.773737 deepsecrets-1.0.6/deepsecrets/core/model/rules/regex.py
+-rw-r--r--   0        0        0      871 2023-04-14 12:57:55.404355 deepsecrets-1.0.6/deepsecrets/core/model/rules/rule.py
+-rw-r--r--   0        0        0       88 2023-02-23 11:55:43.000000 deepsecrets-1.0.6/deepsecrets/core/model/rules/semantic.py
+-rw-r--r--   0        0        0      237 2023-02-28 15:59:50.000000 deepsecrets-1.0.6/deepsecrets/core/model/semantic.py
+-rw-r--r--   0        0        0     2007 2023-04-17 12:50:06.475278 deepsecrets-1.0.6/deepsecrets/core/model/token.py
+-rw-r--r--   0        0        0     6148 2023-02-26 15:19:47.000000 deepsecrets-1.0.6/deepsecrets/core/modes/.DS_Store
+-rw-r--r--   0        0        0     8425 2023-06-13 10:12:51.339833 deepsecrets-1.0.6/deepsecrets/core/modes/__pycache__/iscan_mode.cpython-311.pyc
+-rw-r--r--   0        0        0     5157 2023-06-13 10:12:50.784613 deepsecrets-1.0.6/deepsecrets/core/modes/iscan_mode.py
+-rw-r--r--   0        0        0      214 2023-01-25 14:00:27.000000 deepsecrets-1.0.6/deepsecrets/core/rulesets/__pycache__/confidence.cpython-311.pyc
+-rw-r--r--   0        0        0      184 2022-09-13 14:18:23.000000 deepsecrets-1.0.6/deepsecrets/core/rulesets/__pycache__/confidence.cpython-39.pyc
+-rw-r--r--   0        0        0      648 2023-02-28 15:59:52.000000 deepsecrets-1.0.6/deepsecrets/core/rulesets/__pycache__/excluded_paths.cpython-311.pyc
+-rw-r--r--   0        0        0      649 2023-04-17 13:45:18.931553 deepsecrets-1.0.6/deepsecrets/core/rulesets/__pycache__/false_findings.cpython-311.pyc
+-rw-r--r--   0        0        0     1424 2022-11-24 10:59:56.000000 deepsecrets-1.0.6/deepsecrets/core/rulesets/__pycache__/false_tokens.cpython-311.pyc
+-rw-r--r--   0        0        0     1796 2022-01-29 06:07:43.000000 deepsecrets-1.0.6/deepsecrets/core/rulesets/__pycache__/false_tokens.cpython-38.pyc
+-rw-r--r--   0        0        0     1059 2022-05-17 09:51:38.000000 deepsecrets-1.0.6/deepsecrets/core/rulesets/__pycache__/false_tokens.cpython-39.pyc
+-rw-r--r--   0        0        0     2551 2023-04-17 13:11:28.556085 deepsecrets-1.0.6/deepsecrets/core/rulesets/__pycache__/hashed_secrets.cpython-311.pyc
+-rw-r--r--   0        0        0     1515 2022-10-14 09:00:28.000000 deepsecrets-1.0.6/deepsecrets/core/rulesets/__pycache__/hashed_secrets.cpython-39.pyc
+-rw-r--r--   0        0        0     2281 2023-02-28 16:49:26.000000 deepsecrets-1.0.6/deepsecrets/core/rulesets/__pycache__/ibuilder.cpython-311.pyc
+-rw-r--r--   0        0        0     4653 2022-11-24 10:59:56.000000 deepsecrets-1.0.6/deepsecrets/core/rulesets/__pycache__/ldap_detector.cpython-311.pyc
+-rw-r--r--   0        0        0     2752 2022-05-17 09:51:38.000000 deepsecrets-1.0.6/deepsecrets/core/rulesets/__pycache__/ldap_detector.cpython-39.pyc
+-rw-r--r--   0        0        0      682 2023-01-28 14:26:39.000000 deepsecrets-1.0.6/deepsecrets/core/rulesets/__pycache__/path_exclusions.cpython-311.pyc
+-rw-r--r--   0        0        0      821 2022-01-29 06:16:36.000000 deepsecrets-1.0.6/deepsecrets/core/rulesets/__pycache__/path_exclusions.cpython-38.pyc
+-rw-r--r--   0        0        0      855 2022-10-13 11:40:21.000000 deepsecrets-1.0.6/deepsecrets/core/rulesets/__pycache__/path_exclusions.cpython-39.pyc
+-rw-r--r--   0        0        0      783 2022-01-28 15:38:18.000000 deepsecrets-1.0.6/deepsecrets/core/rulesets/__pycache__/plaintext.cpython-38.pyc
+-rw-r--r--   0        0        0     1661 2022-02-02 13:16:29.000000 deepsecrets-1.0.6/deepsecrets/core/rulesets/__pycache__/plaintext.cpython-39.pyc
+-rw-r--r--   0        0        0      615 2023-02-28 15:59:52.000000 deepsecrets-1.0.6/deepsecrets/core/rulesets/__pycache__/regex.cpython-311.pyc
+-rw-r--r--   0        0        0     2903 2022-10-13 11:43:01.000000 deepsecrets-1.0.6/deepsecrets/core/rulesets/__pycache__/regex.cpython-39.pyc
+-rw-r--r--   0        0        0      250 2023-02-28 15:59:51.000000 deepsecrets-1.0.6/deepsecrets/core/rulesets/excluded_paths.py
+-rw-r--r--   0        0        0      252 2023-04-17 13:45:18.253008 deepsecrets-1.0.6/deepsecrets/core/rulesets/false_findings.py
+-rw-r--r--   0        0        0     1434 2023-04-17 13:11:27.888766 deepsecrets-1.0.6/deepsecrets/core/rulesets/hashed_secrets.py
+-rw-r--r--   0        0        0      627 2023-02-28 16:35:44.000000 deepsecrets-1.0.6/deepsecrets/core/rulesets/ibuilder.py
+-rw-r--r--   0        0        0      220 2023-02-28 15:59:51.000000 deepsecrets-1.0.6/deepsecrets/core/rulesets/regex.py
+-rw-r--r--   0        0        0     6148 2023-02-26 15:19:47.000000 deepsecrets-1.0.6/deepsecrets/core/tokenizers/.DS_Store
+-rw-r--r--   0        0        0      181 2023-02-23 11:55:44.000000 deepsecrets-1.0.6/deepsecrets/core/tokenizers/__init__.py
+-rw-r--r--   0        0        0      366 2023-02-23 11:55:45.000000 deepsecrets-1.0.6/deepsecrets/core/tokenizers/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      129 2022-09-12 09:34:48.000000 deepsecrets-1.0.6/deepsecrets/core/tokenizers/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     1059 2023-02-15 14:21:01.000000 deepsecrets-1.0.6/deepsecrets/core/tokenizers/__pycache__/full_content.cpython-311.pyc
+-rw-r--r--   0        0        0      649 2022-01-28 16:00:02.000000 deepsecrets-1.0.6/deepsecrets/core/tokenizers/__pycache__/full_content.cpython-38.pyc
+-rw-r--r--   0        0        0      732 2022-10-13 14:47:47.000000 deepsecrets-1.0.6/deepsecrets/core/tokenizers/__pycache__/full_content.cpython-39.pyc
+-rw-r--r--   0        0        0     1948 2023-02-28 15:59:52.000000 deepsecrets-1.0.6/deepsecrets/core/tokenizers/__pycache__/itokenizer.cpython-311.pyc
+-rw-r--r--   0        0        0      520 2022-01-28 13:54:30.000000 deepsecrets-1.0.6/deepsecrets/core/tokenizers/__pycache__/itokenizer.cpython-38.pyc
+-rw-r--r--   0        0        0     1549 2022-10-13 14:13:37.000000 deepsecrets-1.0.6/deepsecrets/core/tokenizers/__pycache__/itokenizer.cpython-39.pyc
+-rw-r--r--   0        0        0     2569 2022-04-25 16:49:33.000000 deepsecrets-1.0.6/deepsecrets/core/tokenizers/__pycache__/lex_utils.cpython-39.pyc
+-rw-r--r--   0        0        0    10200 2023-06-26 13:42:04.228723 deepsecrets-1.0.6/deepsecrets/core/tokenizers/__pycache__/lexer.cpython-311.pyc
+-rw-r--r--   0        0        0     4195 2022-05-27 10:40:16.000000 deepsecrets-1.0.6/deepsecrets/core/tokenizers/__pycache__/lexer.cpython-39.pyc
+-rw-r--r--   0        0        0     1482 2023-04-14 12:50:35.476023 deepsecrets-1.0.6/deepsecrets/core/tokenizers/__pycache__/per_line.cpython-311.pyc
+-rw-r--r--   0        0        0      852 2022-01-28 17:43:01.000000 deepsecrets-1.0.6/deepsecrets/core/tokenizers/__pycache__/per_line.cpython-38.pyc
+-rw-r--r--   0        0        0      899 2022-09-12 09:34:48.000000 deepsecrets-1.0.6/deepsecrets/core/tokenizers/__pycache__/per_line.cpython-39.pyc
+-rw-r--r--   0        0        0     1723 2023-01-25 14:00:28.000000 deepsecrets-1.0.6/deepsecrets/core/tokenizers/__pycache__/per_word.cpython-311.pyc
+-rw-r--r--   0        0        0      977 2022-01-28 18:09:20.000000 deepsecrets-1.0.6/deepsecrets/core/tokenizers/__pycache__/per_word.cpython-38.pyc
+-rw-r--r--   0        0        0     1010 2022-09-12 09:34:48.000000 deepsecrets-1.0.6/deepsecrets/core/tokenizers/__pycache__/per_word.cpython-39.pyc
+-rw-r--r--   0        0        0      349 2023-02-15 13:58:04.000000 deepsecrets-1.0.6/deepsecrets/core/tokenizers/full_content.py
+-rw-r--r--   0        0        0     6148 2023-02-26 15:19:47.000000 deepsecrets-1.0.6/deepsecrets/core/tokenizers/helpers/.DS_Store
+-rw-r--r--   0        0        0        0 2023-01-25 14:00:23.000000 deepsecrets-1.0.6/deepsecrets/core/tokenizers/helpers/__init__.py
+-rw-r--r--   0        0        0      153 2023-01-25 14:00:28.000000 deepsecrets-1.0.6/deepsecrets/core/tokenizers/helpers/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      135 2022-09-12 09:34:48.000000 deepsecrets-1.0.6/deepsecrets/core/tokenizers/helpers/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     9952 2023-02-10 11:22:52.000000 deepsecrets-1.0.6/deepsecrets/core/tokenizers/helpers/__pycache__/lexer.cpython-311.pyc
+-rw-r--r--   0        0        0     6003 2022-10-13 14:25:20.000000 deepsecrets-1.0.6/deepsecrets/core/tokenizers/helpers/__pycache__/lexer.cpython-39.pyc
+-rw-r--r--   0        0        0     3663 2023-06-26 16:51:54.572701 deepsecrets-1.0.6/deepsecrets/core/tokenizers/helpers/__pycache__/spot_improvements.cpython-311.pyc
+-rw-r--r--   0        0        0     2799 2023-04-21 14:40:38.036123 deepsecrets-1.0.6/deepsecrets/core/tokenizers/helpers/__pycache__/type_stream.cpython-311.pyc
+-rw-r--r--   0        0        0     6148 2023-02-26 15:19:47.000000 deepsecrets-1.0.6/deepsecrets/core/tokenizers/helpers/semantic/.DS_Store
+-rw-r--r--   0        0        0        0 2023-01-25 14:00:23.000000 deepsecrets-1.0.6/deepsecrets/core/tokenizers/helpers/semantic/__init__.py
+-rw-r--r--   0        0        0      162 2023-01-25 14:00:28.000000 deepsecrets-1.0.6/deepsecrets/core/tokenizers/helpers/semantic/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      144 2022-09-12 10:58:48.000000 deepsecrets-1.0.6/deepsecrets/core/tokenizers/helpers/semantic/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     1353 2023-04-13 12:42:45.606082 deepsecrets-1.0.6/deepsecrets/core/tokenizers/helpers/semantic/__pycache__/language.cpython-311.pyc
+-rw-r--r--   0        0        0     2684 2022-06-08 15:19:48.000000 deepsecrets-1.0.6/deepsecrets/core/tokenizers/helpers/semantic/__pycache__/python.cpython-39.pyc
+-rw-r--r--   0        0        0    10645 2023-02-10 11:00:04.000000 deepsecrets-1.0.6/deepsecrets/core/tokenizers/helpers/semantic/__pycache__/variable_detection.cpython-311.pyc
+-rw-r--r--   0        0        0     4836 2022-10-13 14:38:14.000000 deepsecrets-1.0.6/deepsecrets/core/tokenizers/helpers/semantic/__pycache__/variable_detection.cpython-39.pyc
+-rw-r--r--   0        0        0      529 2023-04-13 12:42:44.862774 deepsecrets-1.0.6/deepsecrets/core/tokenizers/helpers/semantic/language.py
+-rw-r--r--   0        0        0        0 2023-02-10 15:56:26.000000 deepsecrets-1.0.6/deepsecrets/core/tokenizers/helpers/semantic/var_detection/__init__.py
+-rw-r--r--   0        0        0      184 2023-02-10 15:56:27.000000 deepsecrets-1.0.6/deepsecrets/core/tokenizers/helpers/semantic/var_detection/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     5347 2023-04-14 13:00:04.497720 deepsecrets-1.0.6/deepsecrets/core/tokenizers/helpers/semantic/var_detection/__pycache__/detector.cpython-311.pyc
+-rw-r--r--   0        0        0     6581 2023-06-27 14:19:02.007570 deepsecrets-1.0.6/deepsecrets/core/tokenizers/helpers/semantic/var_detection/__pycache__/rules.cpython-311.pyc
+-rw-r--r--   0        0        0     2711 2023-04-14 13:00:03.807886 deepsecrets-1.0.6/deepsecrets/core/tokenizers/helpers/semantic/var_detection/detector.py
+-rw-r--r--   0        0        0     5885 2023-06-27 14:19:01.181294 deepsecrets-1.0.6/deepsecrets/core/tokenizers/helpers/semantic/var_detection/rules.py
+-rw-r--r--   0        0        0     2115 2023-06-26 16:51:53.987615 deepsecrets-1.0.6/deepsecrets/core/tokenizers/helpers/spot_improvements.py
+-rw-r--r--   0        0        0     1801 2023-04-21 14:40:37.153608 deepsecrets-1.0.6/deepsecrets/core/tokenizers/helpers/type_stream.py
+-rw-r--r--   0        0        0      735 2023-02-28 15:59:51.000000 deepsecrets-1.0.6/deepsecrets/core/tokenizers/itokenizer.py
+-rw-r--r--   0        0        0     6481 2023-06-26 13:42:02.632935 deepsecrets-1.0.6/deepsecrets/core/tokenizers/lexer.py
+-rw-r--r--   0        0        0      600 2023-04-14 12:50:34.810801 deepsecrets-1.0.6/deepsecrets/core/tokenizers/per_line.py
+-rw-r--r--   0        0        0     1022 2023-04-14 12:50:38.878506 deepsecrets-1.0.6/deepsecrets/core/tokenizers/per_word.py
+-rw-r--r--   0        0        0     6148 2023-02-26 15:19:47.000000 deepsecrets-1.0.6/deepsecrets/core/utils/.DS_Store
+-rw-r--r--   0        0        0        0 2019-08-30 09:25:52.000000 deepsecrets-1.0.6/deepsecrets/core/utils/__init__.py
+-rw-r--r--   0        0        0      148 2023-02-10 10:44:34.000000 deepsecrets-1.0.6/deepsecrets/core/utils/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      586 2023-02-28 15:32:35.000000 deepsecrets-1.0.6/deepsecrets/core/utils/__pycache__/exceptions.cpython-311.pyc
+-rw-r--r--   0        0        0     5469 2023-03-27 20:23:09.183623 deepsecrets-1.0.6/deepsecrets/core/utils/__pycache__/file_analyzer.cpython-311.pyc
+-rw-r--r--   0        0        0     1415 2023-02-28 16:49:26.000000 deepsecrets-1.0.6/deepsecrets/core/utils/__pycache__/fs.cpython-311.pyc
+-rw-r--r--   0        0        0     1841 2023-06-26 16:37:09.047505 deepsecrets-1.0.6/deepsecrets/core/utils/__pycache__/guess_filetype.cpython-311.pyc
+-rw-r--r--   0        0        0     1774 2023-04-17 12:50:07.088140 deepsecrets-1.0.6/deepsecrets/core/utils/__pycache__/hashing.cpython-311.pyc
+-rw-r--r--   0        0        0      100 2023-02-28 15:32:34.000000 deepsecrets-1.0.6/deepsecrets/core/utils/exceptions.py
+-rw-r--r--   0        0        0     3018 2023-03-27 20:23:08.288214 deepsecrets-1.0.6/deepsecrets/core/utils/file_analyzer.py
+-rw-r--r--   0        0        0      517 2023-02-28 16:47:36.000000 deepsecrets-1.0.6/deepsecrets/core/utils/fs.py
+-rw-r--r--   0        0        0     1060 2023-06-26 16:37:08.518447 deepsecrets-1.0.6/deepsecrets/core/utils/guess_filetype.py
+-rw-r--r--   0        0        0      771 2023-04-17 12:49:00.602766 deepsecrets-1.0.6/deepsecrets/core/utils/hashing.py
+-rw-r--r--   0        0        0     2562 2023-01-29 12:25:02.000000 deepsecrets-1.0.6/deepsecrets/rules/excluded_paths.json
+-rw-r--r--   0        0        0     3993 2023-06-26 12:38:43.101327 deepsecrets-1.0.6/deepsecrets/rules/regexes.json
+-rw-r--r--   0        0        0     6148 2023-02-26 15:19:47.000000 deepsecrets-1.0.6/deepsecrets/scan_modes/.DS_Store
+-rw-r--r--   0        0        0     5698 2023-04-17 13:42:10.557066 deepsecrets-1.0.6/deepsecrets/scan_modes/__pycache__/cli.cpython-311.pyc
+-rw-r--r--   0        0        0     3268 2023-04-17 13:42:09.893195 deepsecrets-1.0.6/deepsecrets/scan_modes/cli.py
+-rw-r--r--   0        0        0     1646 2023-06-27 14:19:34.187662 deepsecrets-1.0.6/pyproject.toml
+-rw-r--r--   0        0        0     6148 1970-01-01 00:00:00.000000 deepsecrets-1.0.6/PKG-INFO
```

### Comparing `deepsecrets-1.0.5/LICENSE` & `deepsecrets-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.5/README.md` & `deepsecrets-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.5/deepsecrets/.DS_Store` & `deepsecrets-1.0.6/deepsecrets/.DS_Store`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.5/deepsecrets/__init__.py` & `deepsecrets-1.0.6/deepsecrets/__init__.py`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.5/deepsecrets/cli.py` & `deepsecrets-1.0.6/deepsecrets/cli.py`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.5/deepsecrets/config.py` & `deepsecrets-1.0.6/deepsecrets/config.py`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.5/deepsecrets/core/.DS_Store` & `deepsecrets-1.0.6/deepsecrets/core/.DS_Store`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.5/deepsecrets/core/engines/__pycache__/hashed_secret.cpython-311.pyc` & `deepsecrets-1.0.6/deepsecrets/core/engines/__pycache__/hashed_secret.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.5/deepsecrets/core/engines/__pycache__/iengine.cpython-311.pyc` & `deepsecrets-1.0.6/deepsecrets/core/engines/__pycache__/iengine.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.5/deepsecrets/core/engines/__pycache__/regex.cpython-311.pyc` & `deepsecrets-1.0.6/deepsecrets/core/engines/__pycache__/regex.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.5/deepsecrets/core/engines/__pycache__/semantic.cpython-311.pyc` & `deepsecrets-1.0.6/deepsecrets/core/engines/__pycache__/semantic.cpython-311.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x62c29264 (Wed Jun 21 09:26:58 2023 UTC)
+moddate:  0x2bed9a64 (Tue Jun 27 14:07:39 2023 UTC)
 files sz: 4341
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
```

### Comparing `deepsecrets-1.0.5/deepsecrets/core/engines/hashed_secret.py` & `deepsecrets-1.0.6/deepsecrets/core/engines/hashed_secret.py`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.5/deepsecrets/core/engines/iengine.py` & `deepsecrets-1.0.6/deepsecrets/core/engines/iengine.py`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.5/deepsecrets/core/engines/regex.py` & `deepsecrets-1.0.6/deepsecrets/core/engines/regex.py`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.5/deepsecrets/core/engines/semantic.py` & `deepsecrets-1.0.6/deepsecrets/core/engines/semantic.py`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.5/deepsecrets/core/helpers/__pycache__/content_analyzer.cpython-311.pyc` & `deepsecrets-1.0.6/deepsecrets/core/helpers/__pycache__/content_analyzer.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.5/deepsecrets/core/helpers/__pycache__/content_analyzer.cpython-39.pyc` & `deepsecrets-1.0.6/deepsecrets/core/helpers/__pycache__/content_analyzer.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.5/deepsecrets/core/helpers/__pycache__/entropy.cpython-311.pyc` & `deepsecrets-1.0.6/deepsecrets/core/helpers/__pycache__/entropy.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.5/deepsecrets/core/helpers/__pycache__/entropy.cpython-39.pyc` & `deepsecrets-1.0.6/deepsecrets/core/helpers/__pycache__/entropy.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.5/deepsecrets/core/helpers/content_analyzer.py` & `deepsecrets-1.0.6/deepsecrets/core/helpers/content_analyzer.py`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.5/deepsecrets/core/helpers/entropy.py` & `deepsecrets-1.0.6/deepsecrets/core/helpers/entropy.py`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.5/deepsecrets/core/model/.DS_Store` & `deepsecrets-1.0.6/deepsecrets/core/model/.DS_Store`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.5/deepsecrets/core/model/__pycache__/file.cpython-311.pyc` & `deepsecrets-1.0.6/deepsecrets/core/model/__pycache__/file.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.5/deepsecrets/core/model/__pycache__/finding.cpython-311.pyc` & `deepsecrets-1.0.6/deepsecrets/core/model/__pycache__/finding.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.5/deepsecrets/core/model/__pycache__/semantic.cpython-311.pyc` & `deepsecrets-1.0.6/deepsecrets/core/model/__pycache__/semantic.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.5/deepsecrets/core/model/__pycache__/token.cpython-311.pyc` & `deepsecrets-1.0.6/deepsecrets/core/model/__pycache__/token.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.5/deepsecrets/core/model/file.py` & `deepsecrets-1.0.6/deepsecrets/core/model/file.py`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.5/deepsecrets/core/model/finding.py` & `deepsecrets-1.0.6/deepsecrets/core/model/finding.py`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.5/deepsecrets/core/model/rules/__pycache__/exlcuded_path.cpython-311.pyc` & `deepsecrets-1.0.6/deepsecrets/core/model/rules/__pycache__/exlcuded_path.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.5/deepsecrets/core/model/rules/__pycache__/hashed_secret.cpython-311.pyc` & `deepsecrets-1.0.6/deepsecrets/core/model/rules/__pycache__/hashed_secret.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.5/deepsecrets/core/model/rules/__pycache__/regex.cpython-311.pyc` & `deepsecrets-1.0.6/deepsecrets/core/model/rules/__pycache__/regex.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.5/deepsecrets/core/model/rules/__pycache__/rule.cpython-311.pyc` & `deepsecrets-1.0.6/deepsecrets/core/model/rules/__pycache__/rule.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.5/deepsecrets/core/model/rules/hashed_secret.py` & `deepsecrets-1.0.6/deepsecrets/core/model/rules/hashed_secret.py`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.5/deepsecrets/core/model/rules/regex.py` & `deepsecrets-1.0.6/deepsecrets/core/model/rules/regex.py`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.5/deepsecrets/core/model/rules/rule.py` & `deepsecrets-1.0.6/deepsecrets/core/model/rules/rule.py`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.5/deepsecrets/core/model/token.py` & `deepsecrets-1.0.6/deepsecrets/core/model/token.py`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.5/deepsecrets/core/modes/.DS_Store` & `deepsecrets-1.0.6/deepsecrets/core/modes/.DS_Store`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.5/deepsecrets/core/modes/__pycache__/iscan_mode.cpython-311.pyc` & `deepsecrets-1.0.6/deepsecrets/core/modes/__pycache__/iscan_mode.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.5/deepsecrets/core/modes/iscan_mode.py` & `deepsecrets-1.0.6/deepsecrets/core/modes/iscan_mode.py`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.5/deepsecrets/core/rulesets/__pycache__/excluded_paths.cpython-311.pyc` & `deepsecrets-1.0.6/deepsecrets/core/rulesets/__pycache__/excluded_paths.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.5/deepsecrets/core/rulesets/__pycache__/false_findings.cpython-311.pyc` & `deepsecrets-1.0.6/deepsecrets/core/rulesets/__pycache__/false_findings.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.5/deepsecrets/core/rulesets/__pycache__/false_tokens.cpython-311.pyc` & `deepsecrets-1.0.6/deepsecrets/core/rulesets/__pycache__/false_tokens.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.5/deepsecrets/core/rulesets/__pycache__/false_tokens.cpython-38.pyc` & `deepsecrets-1.0.6/deepsecrets/core/rulesets/__pycache__/false_tokens.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.5/deepsecrets/core/rulesets/__pycache__/false_tokens.cpython-39.pyc` & `deepsecrets-1.0.6/deepsecrets/core/rulesets/__pycache__/false_tokens.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.5/deepsecrets/core/rulesets/__pycache__/hashed_secrets.cpython-311.pyc` & `deepsecrets-1.0.6/deepsecrets/core/rulesets/__pycache__/hashed_secrets.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.5/deepsecrets/core/rulesets/__pycache__/hashed_secrets.cpython-39.pyc` & `deepsecrets-1.0.6/deepsecrets/core/rulesets/__pycache__/hashed_secrets.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.5/deepsecrets/core/rulesets/__pycache__/ibuilder.cpython-311.pyc` & `deepsecrets-1.0.6/deepsecrets/core/rulesets/__pycache__/ibuilder.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.5/deepsecrets/core/rulesets/__pycache__/ldap_detector.cpython-311.pyc` & `deepsecrets-1.0.6/deepsecrets/core/rulesets/__pycache__/ldap_detector.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.5/deepsecrets/core/rulesets/__pycache__/ldap_detector.cpython-39.pyc` & `deepsecrets-1.0.6/deepsecrets/core/rulesets/__pycache__/ldap_detector.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.5/deepsecrets/core/rulesets/__pycache__/path_exclusions.cpython-311.pyc` & `deepsecrets-1.0.6/deepsecrets/core/rulesets/__pycache__/path_exclusions.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.5/deepsecrets/core/rulesets/__pycache__/path_exclusions.cpython-38.pyc` & `deepsecrets-1.0.6/deepsecrets/core/rulesets/__pycache__/path_exclusions.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.5/deepsecrets/core/rulesets/__pycache__/path_exclusions.cpython-39.pyc` & `deepsecrets-1.0.6/deepsecrets/core/rulesets/__pycache__/path_exclusions.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.5/deepsecrets/core/rulesets/__pycache__/plaintext.cpython-38.pyc` & `deepsecrets-1.0.6/deepsecrets/core/rulesets/__pycache__/plaintext.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.5/deepsecrets/core/rulesets/__pycache__/plaintext.cpython-39.pyc` & `deepsecrets-1.0.6/deepsecrets/core/rulesets/__pycache__/plaintext.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.5/deepsecrets/core/rulesets/__pycache__/regex.cpython-311.pyc` & `deepsecrets-1.0.6/deepsecrets/core/rulesets/__pycache__/regex.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.5/deepsecrets/core/rulesets/__pycache__/regex.cpython-39.pyc` & `deepsecrets-1.0.6/deepsecrets/core/rulesets/__pycache__/regex.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.5/deepsecrets/core/rulesets/hashed_secrets.py` & `deepsecrets-1.0.6/deepsecrets/core/rulesets/hashed_secrets.py`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.5/deepsecrets/core/rulesets/ibuilder.py` & `deepsecrets-1.0.6/deepsecrets/core/rulesets/ibuilder.py`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.5/deepsecrets/core/tokenizers/.DS_Store` & `deepsecrets-1.0.6/deepsecrets/core/tokenizers/.DS_Store`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.5/deepsecrets/core/tokenizers/__pycache__/full_content.cpython-311.pyc` & `deepsecrets-1.0.6/deepsecrets/core/tokenizers/__pycache__/full_content.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.5/deepsecrets/core/tokenizers/__pycache__/full_content.cpython-38.pyc` & `deepsecrets-1.0.6/deepsecrets/core/tokenizers/__pycache__/full_content.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.5/deepsecrets/core/tokenizers/__pycache__/full_content.cpython-39.pyc` & `deepsecrets-1.0.6/deepsecrets/core/tokenizers/__pycache__/full_content.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.5/deepsecrets/core/tokenizers/__pycache__/itokenizer.cpython-311.pyc` & `deepsecrets-1.0.6/deepsecrets/core/tokenizers/__pycache__/itokenizer.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.5/deepsecrets/core/tokenizers/__pycache__/itokenizer.cpython-38.pyc` & `deepsecrets-1.0.6/deepsecrets/core/tokenizers/__pycache__/itokenizer.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.5/deepsecrets/core/tokenizers/__pycache__/itokenizer.cpython-39.pyc` & `deepsecrets-1.0.6/deepsecrets/core/tokenizers/__pycache__/itokenizer.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.5/deepsecrets/core/tokenizers/__pycache__/lex_utils.cpython-39.pyc` & `deepsecrets-1.0.6/deepsecrets/core/tokenizers/__pycache__/lex_utils.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.5/deepsecrets/core/tokenizers/__pycache__/lexer.cpython-311.pyc` & `deepsecrets-1.0.6/deepsecrets/core/tokenizers/__pycache__/lexer.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.5/deepsecrets/core/tokenizers/__pycache__/lexer.cpython-39.pyc` & `deepsecrets-1.0.6/deepsecrets/core/tokenizers/__pycache__/lexer.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.5/deepsecrets/core/tokenizers/__pycache__/per_line.cpython-311.pyc` & `deepsecrets-1.0.6/deepsecrets/core/tokenizers/__pycache__/per_line.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.5/deepsecrets/core/tokenizers/__pycache__/per_line.cpython-38.pyc` & `deepsecrets-1.0.6/deepsecrets/core/tokenizers/__pycache__/per_line.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.5/deepsecrets/core/tokenizers/__pycache__/per_line.cpython-39.pyc` & `deepsecrets-1.0.6/deepsecrets/core/tokenizers/__pycache__/per_line.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.5/deepsecrets/core/tokenizers/__pycache__/per_word.cpython-311.pyc` & `deepsecrets-1.0.6/deepsecrets/core/tokenizers/__pycache__/per_word.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.5/deepsecrets/core/tokenizers/__pycache__/per_word.cpython-38.pyc` & `deepsecrets-1.0.6/deepsecrets/core/tokenizers/__pycache__/per_word.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.5/deepsecrets/core/tokenizers/__pycache__/per_word.cpython-39.pyc` & `deepsecrets-1.0.6/deepsecrets/core/tokenizers/__pycache__/per_word.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.5/deepsecrets/core/tokenizers/helpers/.DS_Store` & `deepsecrets-1.0.6/deepsecrets/core/tokenizers/helpers/.DS_Store`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.5/deepsecrets/core/tokenizers/helpers/__pycache__/lexer.cpython-311.pyc` & `deepsecrets-1.0.6/deepsecrets/core/tokenizers/helpers/__pycache__/lexer.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.5/deepsecrets/core/tokenizers/helpers/__pycache__/lexer.cpython-39.pyc` & `deepsecrets-1.0.6/deepsecrets/core/tokenizers/helpers/__pycache__/lexer.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.5/deepsecrets/core/tokenizers/helpers/__pycache__/spot_improvements.cpython-311.pyc` & `deepsecrets-1.0.6/deepsecrets/core/tokenizers/helpers/__pycache__/spot_improvements.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.5/deepsecrets/core/tokenizers/helpers/__pycache__/type_stream.cpython-311.pyc` & `deepsecrets-1.0.6/deepsecrets/core/tokenizers/helpers/__pycache__/type_stream.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.5/deepsecrets/core/tokenizers/helpers/semantic/.DS_Store` & `deepsecrets-1.0.6/deepsecrets/core/tokenizers/helpers/semantic/.DS_Store`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.5/deepsecrets/core/tokenizers/helpers/semantic/__pycache__/language.cpython-311.pyc` & `deepsecrets-1.0.6/deepsecrets/core/tokenizers/helpers/semantic/__pycache__/language.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.5/deepsecrets/core/tokenizers/helpers/semantic/__pycache__/python.cpython-39.pyc` & `deepsecrets-1.0.6/deepsecrets/core/tokenizers/helpers/semantic/__pycache__/python.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.5/deepsecrets/core/tokenizers/helpers/semantic/__pycache__/variable_detection.cpython-311.pyc` & `deepsecrets-1.0.6/deepsecrets/core/tokenizers/helpers/semantic/__pycache__/variable_detection.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.5/deepsecrets/core/tokenizers/helpers/semantic/__pycache__/variable_detection.cpython-39.pyc` & `deepsecrets-1.0.6/deepsecrets/core/tokenizers/helpers/semantic/__pycache__/variable_detection.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.5/deepsecrets/core/tokenizers/helpers/semantic/language.py` & `deepsecrets-1.0.6/deepsecrets/core/tokenizers/helpers/semantic/language.py`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.5/deepsecrets/core/tokenizers/helpers/semantic/var_detection/__pycache__/detector.cpython-311.pyc` & `deepsecrets-1.0.6/deepsecrets/core/tokenizers/helpers/semantic/var_detection/__pycache__/detector.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.5/deepsecrets/core/tokenizers/helpers/semantic/var_detection/__pycache__/rules.cpython-311.pyc` & `deepsecrets-1.0.6/deepsecrets/core/tokenizers/helpers/semantic/var_detection/__pycache__/rules.cpython-311.pyc`

 * *Files 4% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0xbc503964 (Fri Apr 14 13:10:20 2023 UTC)
-files sz: 5781
+moddate:  0xd5ef9a64 (Tue Jun 27 14:19:01 2023 UTC)
+files sz: 5885
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 4
    flags     : 0
    code
       0x9700640064016c005a01640064026c026d035a030100640064036c046d
@@ -107,48 +107,49 @@
             0065066a0700000000000000006425a6010000ab01000000000000000064
             020200650864036701ac05a6010000ab0100000000000000006901640664
             0764089c02ac09a6040000ab0400000000000000000200650365046a0e00
             00000000000000020065066a0700000000000000006426a6010000ab0100
             00000000000000640202006508641e64036702ac05a6010000ab01000000
             000000000069016406640764089c02ac09a6040000ab0400000000000000
             000200650365046a0f0000000000000000020065066a0700000000000000
-            006427a6010000ab010000000000000000640202006508640464036702ac
-            05a6010000ab01000000000000000069016406640764089c02ac09a60400
-            00ab0400000000000000000200650365046a100000000000000000020065
-            066a0700000000000000006428a6010000ab010000000000000000020065
-            08020065066a0700000000000000006429a6010000ab0100000000000000
-            006701ac05a6010000ab01000000000000000002006508020065066a0700
-            00000000000000642aa6010000ab0100000000000000006701ac05a60100
-            00ab01000000000000000002006508020065066a07000000000000000064
-            2ba6010000ab0100000000000000006701ac19a6010000ab010000000000
-            000000642c9c036406640764159c02642dac2ea6050000ab050000000000
-            0000000200650365046a110000000000000000020065066a070000000000
-            000000642fa6010000ab01000000000000000002006508020065066a0700
-            000000000000006430a6010000ab0100000000000000006701ac05a60100
-            00ab01000000000000000002006508020065066a07000000000000000064
-            31a6010000ab0100000000000000006701ac19a6010000ab010000000000
-            000000640e9c0264066407640d9c02ac09a6040000ab0400000000000000
-            000200650365046a110000000000000000020065066a0700000000000000
-            006432a6010000ab01000000000000000002006508020065066a07000000
-            00000000006433a6010000ab0100000000000000006701ac05a6010000ab
-            01000000000000000002006508020065066a0700000000000000006434a6
-            010000ab0100000000000000006701ac05a6010000ab0100000000000000
-            0002006508020065066a0700000000000000006431a6010000ab01000000
-            00000000006701ac05a6010000ab01000000000000000064359c03640664
-            0764369c02ac09a6040000ab0400000000000000000200650365046a1200
-            00000000000000020065066a0700000000000000006437a6010000ab0100
-            0000000000000002006508020065066a0700000000000000006438a60100
-            00ab0100000000000000006701ac05a6010000ab01000000000000000002
-            006508020065066a0700000000000000006439a6010000ab010000000000
-            0000006701ac05a6010000ab01000000000000000002006508020065066a
-            0700000000000000006434a6010000ab0100000000000000006701ac05a6
-            010000ab010000000000000000642c9c0364066407643a9c02ac09a60400
-            00ab04000000000000000067125a136514643b6504643c65156503190000
-            000000000000006604643d8404a6000000ab0000000000000000005a1664
-            3e5300
+            006427a6010000ab010000000000000000640202006508020065066a0700
+            000000000000006428a6010000ab010000000000000000020065066a0700
+            000000000000006429a6010000ab0100000000000000006702ac05a60100
+            00ab01000000000000000069016406640764089c02ac09a6040000ab0400
+            000000000000000200650365046a100000000000000000020065066a0700
+            00000000000000642aa6010000ab01000000000000000002006508020065
+            066a070000000000000000642ba6010000ab0100000000000000006701ac
+            05a6010000ab01000000000000000002006508020065066a070000000000
+            000000642ca6010000ab0100000000000000006701ac05a6010000ab0100
+            0000000000000002006508020065066a070000000000000000642da60100
+            00ab0100000000000000006701ac19a6010000ab01000000000000000064
+            2e9c036406640764159c02642fac30a6050000ab05000000000000000002
+            00650365046a110000000000000000020065066a07000000000000000064
+            31a6010000ab01000000000000000002006508020065066a070000000000
+            0000006432a6010000ab0100000000000000006701ac05a6010000ab0100
+            0000000000000002006508020065066a0700000000000000006433a60100
+            00ab0100000000000000006701ac19a6010000ab01000000000000000064
+            0e9c0264066407640d9c02ac09a6040000ab040000000000000000020065
+            0365046a110000000000000000020065066a0700000000000000006434a6
+            010000ab01000000000000000002006508020065066a0700000000000000
+            006435a6010000ab0100000000000000006701ac05a6010000ab01000000
+            000000000002006508020065066a0700000000000000006436a6010000ab
+            0100000000000000006701ac05a6010000ab010000000000000000020065
+            08020065066a0700000000000000006433a6010000ab0100000000000000
+            006701ac05a6010000ab01000000000000000064379c036406640764389c
+            02ac09a6040000ab0400000000000000000200650365046a120000000000
+            000000020065066a0700000000000000006439a6010000ab010000000000
+            00000002006508020065066a070000000000000000643aa6010000ab0100
+            000000000000006701ac05a6010000ab0100000000000000000200650802
+            0065066a070000000000000000643ba6010000ab01000000000000000067
+            01ac05a6010000ab01000000000000000002006508020065066a07000000
+            00000000006436a6010000ab0100000000000000006701ac05a6010000ab
+            010000000000000000642e9c0364066407643c9c02ac09a6040000ab0400
+            0000000000000067125a136514643d6504643e6515650319000000000000
+            0000006604643f8404a6000000ab0000000000000000005a1664405300
            8           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('VariableDetectionRules')
                        8 STORE_NAME               2 (__qualname__)
          
           10          10 PUSH_NULL
@@ -632,300 +633,314 @@
          104        1456 PUSH_NULL
                     1458 LOAD_NAME                6 (re)
                     1460 LOAD_ATTR                7 (compile)
                     1470 LOAD_CONST              39 ('(v|n)(p|o)(L)')
                     1472 PRECALL                  1
                     1476 CALL                     1
          
-         105        1486 LOAD_CONST               2 (2)
+         106        1486 LOAD_CONST               2 (2)
                     1488 PUSH_NULL
                     1490 LOAD_NAME                8 (Match)
-                    1492 LOAD_CONST               4 (':')
-                    1494 LOAD_CONST               3 ('=')
-                    1496 BUILD_LIST               2
-                    1498 KW_NAMES                 5
-                    1500 PRECALL                  1
-                    1504 CALL                     1
-                    1514 BUILD_MAP                1
-         
-         106        1516 LOAD_CONST               6 ('name')
-                    1518 LOAD_CONST               7 ('value')
-                    1520 LOAD_CONST               8 ((1, 3))
-                    1522 BUILD_CONST_KEY_MAP      2
-         
-         102        1524 KW_NAMES                 9
-                    1526 PRECALL                  4
-                    1530 CALL                     4
-         
-         108        1540 PUSH_NULL
-                    1542 LOAD_NAME                3 (VaribleDetector)
-         
-         109        1544 LOAD_NAME                4 (Language)
-                    1546 LOAD_ATTR               16 (SHELL)
-         
-         110        1556 PUSH_NULL
-                    1558 LOAD_NAME                6 (re)
-                    1560 LOAD_ATTR                7 (compile)
-                    1570 LOAD_CONST              40 ('(L)(L)(L)(L)')
-                    1572 PRECALL                  1
-                    1576 CALL                     1
-         
-         112        1586 PUSH_NULL
-                    1588 LOAD_NAME                8 (Match)
-                    1590 PUSH_NULL
-                    1592 LOAD_NAME                6 (re)
-                    1594 LOAD_ATTR                7 (compile)
-                    1604 LOAD_CONST              41 ('^curl$')
-                    1606 PRECALL                  1
-                    1610 CALL                     1
-                    1620 BUILD_LIST               1
-                    1622 KW_NAMES                 5
-                    1624 PRECALL                  1
-                    1628 CALL                     1
-         
-         113        1638 PUSH_NULL
-                    1640 LOAD_NAME                8 (Match)
-                    1642 PUSH_NULL
-                    1644 LOAD_NAME                6 (re)
-                    1646 LOAD_ATTR                7 (compile)
-                    1656 LOAD_CONST              42 ('^-u$')
-                    1658 PRECALL                  1
-                    1662 CALL                     1
-                    1672 BUILD_LIST               1
-                    1674 KW_NAMES                 5
-                    1676 PRECALL                  1
-                    1680 CALL                     1
-         
-         114        1690 PUSH_NULL
-                    1692 LOAD_NAME                8 (Match)
-                    1694 PUSH_NULL
-                    1696 LOAD_NAME                6 (re)
-                    1698 LOAD_ATTR                7 (compile)
-                    1708 LOAD_CONST              43 ('^\\$')
-                    1710 PRECALL                  1
-                    1714 CALL                     1
-                    1724 BUILD_LIST               1
-                    1726 KW_NAMES                25
-                    1728 PRECALL                  1
-                    1732 CALL                     1
-         
-         111        1742 LOAD_CONST              44 ((1, 2, 4))
-                    1744 BUILD_CONST_KEY_MAP      3
-         
-         116        1746 LOAD_CONST               6 ('name')
-                    1748 LOAD_CONST               7 ('value')
-                    1750 LOAD_CONST              21 ((3, 4))
-                    1752 BUILD_CONST_KEY_MAP      2
-         
-         117        1754 LOAD_CONST              45 (9)
-         
-         108        1756 KW_NAMES                46
-                    1758 PRECALL                  5
-                    1762 CALL                     5
-         
-         120        1772 PUSH_NULL
-                    1774 LOAD_NAME                3 (VaribleDetector)
-         
-         121        1776 LOAD_NAME                4 (Language)
-                    1778 LOAD_ATTR               17 (CSHARP)
-         
-         122        1788 PUSH_NULL
-                    1790 LOAD_NAME                6 (re)
-                    1792 LOAD_ATTR                7 (compile)
-                    1802 LOAD_CONST              47 ('(n).{0,6}(u|L)p(L)(p)')
-                    1804 PRECALL                  1
-                    1808 CALL                     1
-         
-         124        1818 PUSH_NULL
-                    1820 LOAD_NAME                8 (Match)
-                    1822 PUSH_NULL
-                    1824 LOAD_NAME                6 (re)
-                    1826 LOAD_ATTR                7 (compile)
-                    1836 LOAD_CONST              48 ('^KeyValuePair$')
-                    1838 PRECALL                  1
-                    1842 CALL                     1
-                    1852 BUILD_LIST               1
-                    1854 KW_NAMES                 5
-                    1856 PRECALL                  1
-                    1860 CALL                     1
-         
-         125        1870 PUSH_NULL
-                    1872 LOAD_NAME                8 (Match)
-                    1874 PUSH_NULL
-                    1876 LOAD_NAME                6 (re)
-                    1878 LOAD_ATTR                7 (compile)
-                    1888 LOAD_CONST              49 ('^}$')
-                    1890 PRECALL                  1
-                    1894 CALL                     1
-                    1904 BUILD_LIST               1
-                    1906 KW_NAMES                25
-                    1908 PRECALL                  1
-                    1912 CALL                     1
-         
-         123        1922 LOAD_CONST              14 ((1, 4))
-                    1924 BUILD_CONST_KEY_MAP      2
-         
-         127        1926 LOAD_CONST               6 ('name')
-                    1928 LOAD_CONST               7 ('value')
-                    1930 LOAD_CONST              13 ((2, 3))
-                    1932 BUILD_CONST_KEY_MAP      2
-         
-         120        1934 KW_NAMES                 9
-                    1936 PRECALL                  4
-                    1940 CALL                     4
-         
-         130        1950 PUSH_NULL
-                    1952 LOAD_NAME                3 (VaribleDetector)
-         
-         131        1954 LOAD_NAME                4 (Language)
-                    1956 LOAD_ATTR               17 (CSHARP)
-         
-         132        1966 PUSH_NULL
-                    1968 LOAD_NAME                6 (re)
-                    1970 LOAD_ATTR                7 (compile)
-                    1980 LOAD_CONST              50 ('(p)(.)(p)(L)(p)')
-                    1982 PRECALL                  1
-                    1986 CALL                     1
-         
-         134        1996 PUSH_NULL
-                    1998 LOAD_NAME                8 (Match)
-                    2000 PUSH_NULL
-                    2002 LOAD_NAME                6 (re)
-                    2004 LOAD_ATTR                7 (compile)
-                    2014 LOAD_CONST              51 ('^{$')
-                    2016 PRECALL                  1
-                    2020 CALL                     1
-                    2030 BUILD_LIST               1
-                    2032 KW_NAMES                 5
-                    2034 PRECALL                  1
-                    2038 CALL                     1
-         
-         135        2048 PUSH_NULL
-                    2050 LOAD_NAME                8 (Match)
-                    2052 PUSH_NULL
-                    2054 LOAD_NAME                6 (re)
-                    2056 LOAD_ATTR                7 (compile)
-                    2066 LOAD_CONST              52 ('^,$')
-                    2068 PRECALL                  1
-                    2072 CALL                     1
-                    2082 BUILD_LIST               1
-                    2084 KW_NAMES                 5
-                    2086 PRECALL                  1
-                    2090 CALL                     1
-         
-         136        2100 PUSH_NULL
-                    2102 LOAD_NAME                8 (Match)
-                    2104 PUSH_NULL
-                    2106 LOAD_NAME                6 (re)
-                    2108 LOAD_ATTR                7 (compile)
-                    2118 LOAD_CONST              49 ('^}$')
-                    2120 PRECALL                  1
-                    2124 CALL                     1
-                    2134 BUILD_LIST               1
-                    2136 KW_NAMES                 5
-                    2138 PRECALL                  1
-                    2142 CALL                     1
-         
-         133        2152 LOAD_CONST              53 ((1, 3, 5))
-                    2154 BUILD_CONST_KEY_MAP      3
-         
-         138        2156 LOAD_CONST               6 ('name')
-                    2158 LOAD_CONST               7 ('value')
-                    2160 LOAD_CONST              54 ((2, 4))
-                    2162 BUILD_CONST_KEY_MAP      2
-         
-         130        2164 KW_NAMES                 9
-                    2166 PRECALL                  4
-                    2170 CALL                     4
-         
-         141        2180 PUSH_NULL
-                    2182 LOAD_NAME                3 (VaribleDetector)
-         
-         142        2184 LOAD_NAME                4 (Language)
-                    2186 LOAD_ATTR               18 (JAVA)
-         
-         143        2196 PUSH_NULL
-                    2198 LOAD_NAME                6 (re)
-                    2200 LOAD_ATTR                7 (compile)
-                    2210 LOAD_CONST              55 ('(n)(p)(.)(p)(L)')
-                    2212 PRECALL                  1
-                    2216 CALL                     1
-         
-         145        2226 PUSH_NULL
-                    2228 LOAD_NAME                8 (Match)
-                    2230 PUSH_NULL
-                    2232 LOAD_NAME                6 (re)
-                    2234 LOAD_ATTR                7 (compile)
-                    2244 LOAD_CONST              56 ('^put$')
-                    2246 PRECALL                  1
-                    2250 CALL                     1
-                    2260 BUILD_LIST               1
-                    2262 KW_NAMES                 5
-                    2264 PRECALL                  1
-                    2268 CALL                     1
-         
-         146        2278 PUSH_NULL
-                    2280 LOAD_NAME                8 (Match)
-                    2282 PUSH_NULL
-                    2284 LOAD_NAME                6 (re)
-                    2286 LOAD_ATTR                7 (compile)
-                    2296 LOAD_CONST              57 ('^\\($')
-                    2298 PRECALL                  1
-                    2302 CALL                     1
-                    2312 BUILD_LIST               1
-                    2314 KW_NAMES                 5
-                    2316 PRECALL                  1
-                    2320 CALL                     1
-         
-         147        2330 PUSH_NULL
-                    2332 LOAD_NAME                8 (Match)
-                    2334 PUSH_NULL
-                    2336 LOAD_NAME                6 (re)
-                    2338 LOAD_ATTR                7 (compile)
-                    2348 LOAD_CONST              52 ('^,$')
-                    2350 PRECALL                  1
-                    2354 CALL                     1
-                    2364 BUILD_LIST               1
-                    2366 KW_NAMES                 5
-                    2368 PRECALL                  1
-                    2372 CALL                     1
-         
-         144        2382 LOAD_CONST              44 ((1, 2, 4))
-                    2384 BUILD_CONST_KEY_MAP      3
-         
-         149        2386 LOAD_CONST               6 ('name')
-                    2388 LOAD_CONST               7 ('value')
-                    2390 LOAD_CONST              58 ((3, 5))
-                    2392 BUILD_CONST_KEY_MAP      2
-         
-         141        2394 KW_NAMES                 9
-                    2396 PRECALL                  4
-                    2400 CALL                     4
-         
-           9        2410 BUILD_LIST              18
-                    2412 STORE_NAME              19 (rules)
-         
-         154        2414 LOAD_NAME               20 (classmethod)
-         
-         155        2416 LOAD_CONST              59 ('language')
-                    2418 LOAD_NAME                4 (Language)
-                    2420 LOAD_CONST              60 ('return')
-                    2422 LOAD_NAME               21 (List)
-                    2424 LOAD_NAME                3 (VaribleDetector)
-                    2426 BINARY_SUBSCR
-                    2436 BUILD_TUPLE              4
-                    2438 LOAD_CONST              61 (<code object for_language, file "/app/deepsecrets/core/tokenizers/helpers/semantic/var_detection/rules.py", line 154>)
-                    2440 MAKE_FUNCTION            4 (annotations)
-         
-         154        2442 PRECALL                  0
-                    2446 CALL                     0
-         
-         155        2456 STORE_NAME              22 (for_language)
-                    2458 LOAD_CONST              62 (None)
-                    2460 RETURN_VALUE
+         
+         107        1492 PUSH_NULL
+                    1494 LOAD_NAME                6 (re)
+                    1496 LOAD_ATTR                7 (compile)
+                    1506 LOAD_CONST              40 ('^:$')
+                    1508 PRECALL                  1
+                    1512 CALL                     1
+         
+         108        1522 PUSH_NULL
+                    1524 LOAD_NAME                6 (re)
+                    1526 LOAD_ATTR                7 (compile)
+                    1536 LOAD_CONST              41 ('^=$')
+                    1538 PRECALL                  1
+                    1542 CALL                     1
+         
+         106        1552 BUILD_LIST               2
+                    1554 KW_NAMES                 5
+                    1556 PRECALL                  1
+                    1560 CALL                     1
+         
+         105        1570 BUILD_MAP                1
+         
+         110        1572 LOAD_CONST               6 ('name')
+                    1574 LOAD_CONST               7 ('value')
+                    1576 LOAD_CONST               8 ((1, 3))
+                    1578 BUILD_CONST_KEY_MAP      2
+         
+         102        1580 KW_NAMES                 9
+                    1582 PRECALL                  4
+                    1586 CALL                     4
+         
+         112        1596 PUSH_NULL
+                    1598 LOAD_NAME                3 (VaribleDetector)
+         
+         113        1600 LOAD_NAME                4 (Language)
+                    1602 LOAD_ATTR               16 (SHELL)
+         
+         114        1612 PUSH_NULL
+                    1614 LOAD_NAME                6 (re)
+                    1616 LOAD_ATTR                7 (compile)
+                    1626 LOAD_CONST              42 ('(L)(L)(L)(L)')
+                    1628 PRECALL                  1
+                    1632 CALL                     1
+         
+         116        1642 PUSH_NULL
+                    1644 LOAD_NAME                8 (Match)
+                    1646 PUSH_NULL
+                    1648 LOAD_NAME                6 (re)
+                    1650 LOAD_ATTR                7 (compile)
+                    1660 LOAD_CONST              43 ('^curl$')
+                    1662 PRECALL                  1
+                    1666 CALL                     1
+                    1676 BUILD_LIST               1
+                    1678 KW_NAMES                 5
+                    1680 PRECALL                  1
+                    1684 CALL                     1
+         
+         117        1694 PUSH_NULL
+                    1696 LOAD_NAME                8 (Match)
+                    1698 PUSH_NULL
+                    1700 LOAD_NAME                6 (re)
+                    1702 LOAD_ATTR                7 (compile)
+                    1712 LOAD_CONST              44 ('^-u$')
+                    1714 PRECALL                  1
+                    1718 CALL                     1
+                    1728 BUILD_LIST               1
+                    1730 KW_NAMES                 5
+                    1732 PRECALL                  1
+                    1736 CALL                     1
+         
+         118        1746 PUSH_NULL
+                    1748 LOAD_NAME                8 (Match)
+                    1750 PUSH_NULL
+                    1752 LOAD_NAME                6 (re)
+                    1754 LOAD_ATTR                7 (compile)
+                    1764 LOAD_CONST              45 ('^\\$')
+                    1766 PRECALL                  1
+                    1770 CALL                     1
+                    1780 BUILD_LIST               1
+                    1782 KW_NAMES                25
+                    1784 PRECALL                  1
+                    1788 CALL                     1
+         
+         115        1798 LOAD_CONST              46 ((1, 2, 4))
+                    1800 BUILD_CONST_KEY_MAP      3
+         
+         120        1802 LOAD_CONST               6 ('name')
+                    1804 LOAD_CONST               7 ('value')
+                    1806 LOAD_CONST              21 ((3, 4))
+                    1808 BUILD_CONST_KEY_MAP      2
+         
+         121        1810 LOAD_CONST              47 (9)
+         
+         112        1812 KW_NAMES                48
+                    1814 PRECALL                  5
+                    1818 CALL                     5
+         
+         124        1828 PUSH_NULL
+                    1830 LOAD_NAME                3 (VaribleDetector)
+         
+         125        1832 LOAD_NAME                4 (Language)
+                    1834 LOAD_ATTR               17 (CSHARP)
+         
+         126        1844 PUSH_NULL
+                    1846 LOAD_NAME                6 (re)
+                    1848 LOAD_ATTR                7 (compile)
+                    1858 LOAD_CONST              49 ('(n).{0,6}(u|L)p(L)(p)')
+                    1860 PRECALL                  1
+                    1864 CALL                     1
+         
+         128        1874 PUSH_NULL
+                    1876 LOAD_NAME                8 (Match)
+                    1878 PUSH_NULL
+                    1880 LOAD_NAME                6 (re)
+                    1882 LOAD_ATTR                7 (compile)
+                    1892 LOAD_CONST              50 ('^KeyValuePair$')
+                    1894 PRECALL                  1
+                    1898 CALL                     1
+                    1908 BUILD_LIST               1
+                    1910 KW_NAMES                 5
+                    1912 PRECALL                  1
+                    1916 CALL                     1
+         
+         129        1926 PUSH_NULL
+                    1928 LOAD_NAME                8 (Match)
+                    1930 PUSH_NULL
+                    1932 LOAD_NAME                6 (re)
+                    1934 LOAD_ATTR                7 (compile)
+                    1944 LOAD_CONST              51 ('^}$')
+                    1946 PRECALL                  1
+                    1950 CALL                     1
+                    1960 BUILD_LIST               1
+                    1962 KW_NAMES                25
+                    1964 PRECALL                  1
+                    1968 CALL                     1
+         
+         127        1978 LOAD_CONST              14 ((1, 4))
+                    1980 BUILD_CONST_KEY_MAP      2
+         
+         131        1982 LOAD_CONST               6 ('name')
+                    1984 LOAD_CONST               7 ('value')
+                    1986 LOAD_CONST              13 ((2, 3))
+                    1988 BUILD_CONST_KEY_MAP      2
+         
+         124        1990 KW_NAMES                 9
+                    1992 PRECALL                  4
+                    1996 CALL                     4
+         
+         134        2006 PUSH_NULL
+                    2008 LOAD_NAME                3 (VaribleDetector)
+         
+         135        2010 LOAD_NAME                4 (Language)
+                    2012 LOAD_ATTR               17 (CSHARP)
+         
+         136        2022 PUSH_NULL
+                    2024 LOAD_NAME                6 (re)
+                    2026 LOAD_ATTR                7 (compile)
+                    2036 LOAD_CONST              52 ('(p)(.)(p)(L)(p)')
+                    2038 PRECALL                  1
+                    2042 CALL                     1
+         
+         138        2052 PUSH_NULL
+                    2054 LOAD_NAME                8 (Match)
+                    2056 PUSH_NULL
+                    2058 LOAD_NAME                6 (re)
+                    2060 LOAD_ATTR                7 (compile)
+                    2070 LOAD_CONST              53 ('^{$')
+                    2072 PRECALL                  1
+                    2076 CALL                     1
+                    2086 BUILD_LIST               1
+                    2088 KW_NAMES                 5
+                    2090 PRECALL                  1
+                    2094 CALL                     1
+         
+         139        2104 PUSH_NULL
+                    2106 LOAD_NAME                8 (Match)
+                    2108 PUSH_NULL
+                    2110 LOAD_NAME                6 (re)
+                    2112 LOAD_ATTR                7 (compile)
+                    2122 LOAD_CONST              54 ('^,$')
+                    2124 PRECALL                  1
+                    2128 CALL                     1
+                    2138 BUILD_LIST               1
+                    2140 KW_NAMES                 5
+                    2142 PRECALL                  1
+                    2146 CALL                     1
+         
+         140        2156 PUSH_NULL
+                    2158 LOAD_NAME                8 (Match)
+                    2160 PUSH_NULL
+                    2162 LOAD_NAME                6 (re)
+                    2164 LOAD_ATTR                7 (compile)
+                    2174 LOAD_CONST              51 ('^}$')
+                    2176 PRECALL                  1
+                    2180 CALL                     1
+                    2190 BUILD_LIST               1
+                    2192 KW_NAMES                 5
+                    2194 PRECALL                  1
+                    2198 CALL                     1
+         
+         137        2208 LOAD_CONST              55 ((1, 3, 5))
+                    2210 BUILD_CONST_KEY_MAP      3
+         
+         142        2212 LOAD_CONST               6 ('name')
+                    2214 LOAD_CONST               7 ('value')
+                    2216 LOAD_CONST              56 ((2, 4))
+                    2218 BUILD_CONST_KEY_MAP      2
+         
+         134        2220 KW_NAMES                 9
+                    2222 PRECALL                  4
+                    2226 CALL                     4
+         
+         145        2236 PUSH_NULL
+                    2238 LOAD_NAME                3 (VaribleDetector)
+         
+         146        2240 LOAD_NAME                4 (Language)
+                    2242 LOAD_ATTR               18 (JAVA)
+         
+         147        2252 PUSH_NULL
+                    2254 LOAD_NAME                6 (re)
+                    2256 LOAD_ATTR                7 (compile)
+                    2266 LOAD_CONST              57 ('(n)(p)(.)(p)(L)')
+                    2268 PRECALL                  1
+                    2272 CALL                     1
+         
+         149        2282 PUSH_NULL
+                    2284 LOAD_NAME                8 (Match)
+                    2286 PUSH_NULL
+                    2288 LOAD_NAME                6 (re)
+                    2290 LOAD_ATTR                7 (compile)
+                    2300 LOAD_CONST              58 ('^put$')
+                    2302 PRECALL                  1
+                    2306 CALL                     1
+                    2316 BUILD_LIST               1
+                    2318 KW_NAMES                 5
+                    2320 PRECALL                  1
+                    2324 CALL                     1
+         
+         150        2334 PUSH_NULL
+                    2336 LOAD_NAME                8 (Match)
+                    2338 PUSH_NULL
+                    2340 LOAD_NAME                6 (re)
+                    2342 LOAD_ATTR                7 (compile)
+                    2352 LOAD_CONST              59 ('^\\($')
+                    2354 PRECALL                  1
+                    2358 CALL                     1
+                    2368 BUILD_LIST               1
+                    2370 KW_NAMES                 5
+                    2372 PRECALL                  1
+                    2376 CALL                     1
+         
+         151        2386 PUSH_NULL
+                    2388 LOAD_NAME                8 (Match)
+                    2390 PUSH_NULL
+                    2392 LOAD_NAME                6 (re)
+                    2394 LOAD_ATTR                7 (compile)
+                    2404 LOAD_CONST              54 ('^,$')
+                    2406 PRECALL                  1
+                    2410 CALL                     1
+                    2420 BUILD_LIST               1
+                    2422 KW_NAMES                 5
+                    2424 PRECALL                  1
+                    2428 CALL                     1
+         
+         148        2438 LOAD_CONST              46 ((1, 2, 4))
+                    2440 BUILD_CONST_KEY_MAP      3
+         
+         153        2442 LOAD_CONST               6 ('name')
+                    2444 LOAD_CONST               7 ('value')
+                    2446 LOAD_CONST              60 ((3, 5))
+                    2448 BUILD_CONST_KEY_MAP      2
+         
+         145        2450 KW_NAMES                 9
+                    2452 PRECALL                  4
+                    2456 CALL                     4
+         
+           9        2466 BUILD_LIST              18
+                    2468 STORE_NAME              19 (rules)
+         
+         158        2470 LOAD_NAME               20 (classmethod)
+         
+         159        2472 LOAD_CONST              61 ('language')
+                    2474 LOAD_NAME                4 (Language)
+                    2476 LOAD_CONST              62 ('return')
+                    2478 LOAD_NAME               21 (List)
+                    2480 LOAD_NAME                3 (VaribleDetector)
+                    2482 BINARY_SUBSCR
+                    2492 BUILD_TUPLE              4
+                    2494 LOAD_CONST              63 (<code object for_language, file "/app/deepsecrets/core/tokenizers/helpers/semantic/var_detection/rules.py", line 158>)
+                    2496 MAKE_FUNCTION            4 (annotations)
+         
+         158        2498 PRECALL                  0
+                    2502 CALL                     0
+         
+         159        2512 STORE_NAME              22 (for_language)
+                    2514 LOAD_CONST              64 (None)
+                    2516 RETURN_VALUE
          consts
             'VariableDetectionRules'
             '(n)(o|p)(?:\n?)(L)(?:\n|p|\\?)'
             2
             '='
             ':'
             ('values',)
@@ -959,14 +974,16 @@
             (2, 3, 4)
             (1, 5)
             '(n)(o)(L)\n'
             '(L)(p)(L)'
             '(n)(o)(L)'
             '(v|n)(o)(L)'
             '(v|n)(p|o)(L)'
+            '^:$'
+            '^=$'
             '(L)(L)(L)(L)'
             '^curl$'
             '^-u$'
             '^\\$'
             (1, 2, 4)
             9
             ('language', 'stream_pattern', 'match_rules', 'match_semantics', 'creds_probability')
@@ -991,21 +1008,21 @@
                flags     : 3
                code
                   0x8701970074010000000000000000000074030000000000000000000088
                   016601640184087c006a020000000000000000a6020000ab020000000000
                   000000a6010000ab0100000000000000005300
                              0 MAKE_CELL                1 (language)
                
-               154           2 RESUME                   0
+               158           2 RESUME                   0
                
-               156           4 LOAD_GLOBAL              1 (NULL + list)
+               160           4 LOAD_GLOBAL              1 (NULL + list)
                             16 LOAD_GLOBAL              3 (NULL + filter)
                             28 LOAD_CLOSURE             1 (language)
                             30 BUILD_TUPLE              1
-                            32 LOAD_CONST               1 (<code object <lambda>, file "/app/deepsecrets/core/tokenizers/helpers/semantic/var_detection/rules.py", line 156>)
+                            32 LOAD_CONST               1 (<code object <lambda>, file "/app/deepsecrets/core/tokenizers/helpers/semantic/var_detection/rules.py", line 160>)
                             34 MAKE_FUNCTION            8 (closure)
                             36 LOAD_FAST                0 (cls)
                             38 LOAD_ATTR                2 (rules)
                             48 PRECALL                  2
                             52 CALL                     2
                             62 PRECALL                  1
                             66 CALL                     1
@@ -1018,15 +1035,15 @@
                      stacksize : 3
                      flags     : 19
                      code
                         0x950197007c006a00000000000000000089017402000000000000000000
                         006a020000000000000000660276005300
                                    0 COPY_FREE_VARS           1
                      
-                     156           2 RESUME                   0
+                     160           2 RESUME                   0
                                    4 LOAD_FAST                0 (x)
                                    6 LOAD_ATTR                0 (language)
                                   16 LOAD_DEREF               1 (language)
                                   18 LOAD_GLOBAL              2 (Language)
                                   30 LOAD_ATTR                2 (ANY)
                                   40 BUILD_TUPLE              2
                                   42 CONTAINS_OP              0
@@ -1035,23 +1052,23 @@
                         None
                      names      ('language', 'Language', 'ANY')
                      varnames   ('x',)
                      freevars   ('language',)
                      cellvars   ()
                      filename   '/app/deepsecrets/core/tokenizers/helpers/semantic/var_detection/rules.py'
                      name       '<lambda>'
-                     firstlineno 156
+                     firstlineno 160
                      lnotab 0x
                names      ('list', 'filter', 'rules')
                varnames   ('cls', 'language')
                freevars   ()
                cellvars   ('language',)
                filename   '/app/deepsecrets/core/tokenizers/helpers/semantic/var_detection/rules.py'
                name       'for_language'
-               firstlineno 154
+               firstlineno 158
                lnotab 0x0402
             None
          names      ('__name__', '__module__', '__qualname__', 'VaribleDetector', 'Language', 'PYTHON', 're', 'compile', 'Match', 'GOLANG', 'PHP', 'TOML', 'YAML', 'INI', 'PUPPET', 'ANY', 'SHELL', 'CSHARP', 'JAVA', 'rules', 'classmethod', 'List', 'for_language')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/app/deepsecrets/core/tokenizers/helpers/semantic/var_detection/rules.py'
@@ -1060,18 +1077,18 @@
          lnotab
             0x0a0204010c011e011e0108fc100604010c011e011c0108fc100604010c
             011e01340108fc100704010c011e011e0108fc100604010c011e02180118
             0118fd040508f8100a04010c011e0218011afe040408f9100904010c011e
             011e0108fc100704010c011e011e0108fc100604010c011e021801180118
             fd040508f8100b04010c011e011c0108fc100604010c011e011c0108fc10
             0604010c011e011c0108fc100604010c011e011e0108fc100604010c011e
-            011e0108fc100604010c011e023401340134fd0405080102f7100c04010c
-            011e02340134fe040408f9100a04010c011e023401340134fd040508f810
-            0b04010c011e023401340134fd040508f8108000fc047f001202011aff0e
-            01
+            0206011e011efe12ff020508f8100a04010c011e023401340134fd040508
+            0102f7100c04010c011e02340134fe040408f9100a04010c011e02340134
+            0134fd040508f8100b04010c011e023401340134fd040508f8108000f804
+            7f001602011aff0e01
       'VariableDetectionRules'
    names      ('regex', 're', 'typing', 'List', 'deepsecrets.core.tokenizers.helpers.semantic.language', 'Language', 'deepsecrets.core.tokenizers.helpers.semantic.var_detection.detector', 'Match', 'VaribleDetector', 'VariableDetectionRules')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/app/deepsecrets/core/tokenizers/helpers/semantic/var_detection/rules.py'
    name       '<module>'
```

### Comparing `deepsecrets-1.0.5/deepsecrets/core/tokenizers/helpers/semantic/var_detection/detector.py` & `deepsecrets-1.0.6/deepsecrets/core/tokenizers/helpers/semantic/var_detection/detector.py`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.5/deepsecrets/core/tokenizers/helpers/semantic/var_detection/rules.py` & `deepsecrets-1.0.6/deepsecrets/core/tokenizers/helpers/semantic/var_detection/rules.py`

 * *Files 4% similar despite different names*

```diff
@@ -98,15 +98,19 @@
             stream_pattern=re.compile('(v|n)(o)(L)'),
             match_rules={2: Match(values=['=>', '='])},
             match_semantics={1: 'name', 3: 'value'},
         ),
         VaribleDetector(
             language=Language.ANY,
             stream_pattern=re.compile('(v|n)(p|o)(L)'),
-            match_rules={2: Match(values=[':', '='])},
+            match_rules={
+                2: Match(values=[
+                    re.compile('^:$'),
+                    re.compile('^=$'),
+                ])},
             match_semantics={1: 'name', 3: 'value'},
         ),
         VaribleDetector(
             language=Language.SHELL,
             stream_pattern=re.compile('(L)(L)(L)(L)'),
             match_rules={
                 1: Match(values=[re.compile('^curl$')]),
```

### Comparing `deepsecrets-1.0.5/deepsecrets/core/tokenizers/helpers/spot_improvements.py` & `deepsecrets-1.0.6/deepsecrets/core/tokenizers/helpers/spot_improvements.py`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.5/deepsecrets/core/tokenizers/helpers/type_stream.py` & `deepsecrets-1.0.6/deepsecrets/core/tokenizers/helpers/type_stream.py`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.5/deepsecrets/core/tokenizers/itokenizer.py` & `deepsecrets-1.0.6/deepsecrets/core/tokenizers/itokenizer.py`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.5/deepsecrets/core/tokenizers/lexer.py` & `deepsecrets-1.0.6/deepsecrets/core/tokenizers/lexer.py`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.5/deepsecrets/core/tokenizers/per_line.py` & `deepsecrets-1.0.6/deepsecrets/core/tokenizers/per_line.py`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.5/deepsecrets/core/tokenizers/per_word.py` & `deepsecrets-1.0.6/deepsecrets/core/tokenizers/per_word.py`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.5/deepsecrets/core/utils/.DS_Store` & `deepsecrets-1.0.6/deepsecrets/core/utils/.DS_Store`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.5/deepsecrets/core/utils/__pycache__/exceptions.cpython-311.pyc` & `deepsecrets-1.0.6/deepsecrets/core/utils/__pycache__/exceptions.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.5/deepsecrets/core/utils/__pycache__/file_analyzer.cpython-311.pyc` & `deepsecrets-1.0.6/deepsecrets/core/utils/__pycache__/file_analyzer.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.5/deepsecrets/core/utils/__pycache__/fs.cpython-311.pyc` & `deepsecrets-1.0.6/deepsecrets/core/utils/__pycache__/fs.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.5/deepsecrets/core/utils/__pycache__/guess_filetype.cpython-311.pyc` & `deepsecrets-1.0.6/deepsecrets/core/utils/__pycache__/guess_filetype.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.5/deepsecrets/core/utils/__pycache__/hashing.cpython-311.pyc` & `deepsecrets-1.0.6/deepsecrets/core/utils/__pycache__/hashing.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.5/deepsecrets/core/utils/file_analyzer.py` & `deepsecrets-1.0.6/deepsecrets/core/utils/file_analyzer.py`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.5/deepsecrets/core/utils/fs.py` & `deepsecrets-1.0.6/deepsecrets/core/utils/fs.py`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.5/deepsecrets/core/utils/guess_filetype.py` & `deepsecrets-1.0.6/deepsecrets/core/utils/guess_filetype.py`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.5/deepsecrets/core/utils/hashing.py` & `deepsecrets-1.0.6/deepsecrets/core/utils/hashing.py`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.5/deepsecrets/rules/excluded_paths.json` & `deepsecrets-1.0.6/deepsecrets/rules/excluded_paths.json`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.5/deepsecrets/rules/regexes.json` & `deepsecrets-1.0.6/deepsecrets/rules/regexes.json`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.5/deepsecrets/scan_modes/.DS_Store` & `deepsecrets-1.0.6/deepsecrets/scan_modes/.DS_Store`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.5/deepsecrets/scan_modes/__pycache__/cli.cpython-311.pyc` & `deepsecrets-1.0.6/deepsecrets/scan_modes/__pycache__/cli.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.5/deepsecrets/scan_modes/cli.py` & `deepsecrets-1.0.6/deepsecrets/scan_modes/cli.py`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.5/pyproject.toml` & `deepsecrets-1.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "deepsecrets"
-version = "1.0.5"
+version = "1.0.6"
 description = "A better tool for secrets search"
 license = "MIT"
 authors = [
   "Nikolai Khechumov <khechumov@gmail.com>",
 ]
 keywords = ["security", "secrets", "credentials", "scanning", "appsec"]
 packages = [{include = "deepsecrets"}]
```

### Comparing `deepsecrets-1.0.5/PKG-INFO` & `deepsecrets-1.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deepsecrets
-Version: 1.0.5
+Version: 1.0.6
 Summary: A better tool for secrets search
 License: MIT
 Keywords: security,secrets,credentials,scanning,appsec
 Author: Nikolai Khechumov
 Author-email: khechumov@gmail.com
 Requires-Python: >=3.9,<3.12
 Classifier: Environment :: Console
```

