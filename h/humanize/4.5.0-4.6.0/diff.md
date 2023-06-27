# Comparing `tmp/humanize-4.5.0.tar.gz` & `tmp/humanize-4.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "humanize-4.5.0.tar", last modified: Sun Jan 29 14:11:55 2023, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `humanize-4.5.0.tar` & `humanize-4.6.0.tar`

### file list

```diff
@@ -1,176 +1,102 @@
-drwxr-xr-x   0 huvankem (692055019) wheel        (0)        0 2023-01-29 14:11:55.183731 humanize-4.5.0/
--rw-r--r--   0 huvankem (692055019) wheel        (0)       30 2023-01-29 14:07:51.000000 humanize-4.5.0/.flake8
-drwxr-xr-x   0 huvankem (692055019) wheel        (0)        0 2023-01-29 14:11:55.156942 humanize-4.5.0/.github/
--rw-r--r--   0 huvankem (692055019) wheel        (0)      514 2023-01-29 14:07:51.000000 humanize-4.5.0/.github/CONTRIBUTING.md
--rw-r--r--   0 huvankem (692055019) wheel        (0)       41 2023-01-29 14:07:51.000000 humanize-4.5.0/.github/FUNDING.yml
--rw-r--r--   0 huvankem (692055019) wheel        (0)      442 2023-01-29 14:07:51.000000 humanize-4.5.0/.github/ISSUE_TEMPLATE.md
--rw-r--r--   0 huvankem (692055019) wheel        (0)       58 2023-01-29 14:07:51.000000 humanize-4.5.0/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 huvankem (692055019) wheel        (0)      144 2023-01-29 14:07:51.000000 humanize-4.5.0/.github/SECURITY.md
--rw-r--r--   0 huvankem (692055019) wheel        (0)     1950 2023-01-29 14:07:51.000000 humanize-4.5.0/.github/labels.yml
--rw-r--r--   0 huvankem (692055019) wheel        (0)      797 2023-01-29 14:07:51.000000 humanize-4.5.0/.github/release-drafter.yml
--rw-r--r--   0 huvankem (692055019) wheel        (0)      453 2023-01-29 14:07:51.000000 humanize-4.5.0/.github/renovate.json
-drwxr-xr-x   0 huvankem (692055019) wheel        (0)        0 2023-01-29 14:11:55.158581 humanize-4.5.0/.github/workflows/
--rw-r--r--   0 huvankem (692055019) wheel        (0)      494 2023-01-29 14:07:51.000000 humanize-4.5.0/.github/workflows/docs.yml
--rw-r--r--   0 huvankem (692055019) wheel        (0)      351 2023-01-29 14:07:51.000000 humanize-4.5.0/.github/workflows/labels.yml
--rw-r--r--   0 huvankem (692055019) wheel        (0)      273 2023-01-29 14:07:51.000000 humanize-4.5.0/.github/workflows/lint.yml
--rw-r--r--   0 huvankem (692055019) wheel        (0)      465 2023-01-29 14:07:51.000000 humanize-4.5.0/.github/workflows/release-drafter.yml
--rw-r--r--   0 huvankem (692055019) wheel        (0)      452 2023-01-29 14:07:51.000000 humanize-4.5.0/.github/workflows/require-pr-label.yml
--rw-r--r--   0 huvankem (692055019) wheel        (0)     1542 2023-01-29 14:07:51.000000 humanize-4.5.0/.github/workflows/test.yml
--rw-r--r--   0 huvankem (692055019) wheel        (0)     3078 2023-01-29 14:07:51.000000 humanize-4.5.0/.gitignore
--rw-r--r--   0 huvankem (692055019) wheel        (0)     1922 2023-01-29 14:07:51.000000 humanize-4.5.0/.pre-commit-config.yaml
--rw-r--r--   0 huvankem (692055019) wheel        (0)       30 2023-01-29 14:07:51.000000 humanize-4.5.0/.readthedocs.yml
--rw-r--r--   0 huvankem (692055019) wheel        (0)     1078 2023-01-29 14:07:51.000000 humanize-4.5.0/LICENCE
--rw-r--r--   0 huvankem (692055019) wheel        (0)       43 2023-01-29 14:07:51.000000 humanize-4.5.0/MANIFEST.in
--rw-r--r--   0 huvankem (692055019) wheel        (0)     7701 2023-01-29 14:11:55.183559 humanize-4.5.0/PKG-INFO
--rw-r--r--   0 huvankem (692055019) wheel        (0)     6087 2023-01-29 14:07:51.000000 humanize-4.5.0/README.md
--rw-r--r--   0 huvankem (692055019) wheel        (0)     1690 2023-01-29 14:07:51.000000 humanize-4.5.0/RELEASING.md
-drwxr-xr-x   0 huvankem (692055019) wheel        (0)        0 2023-01-29 14:11:55.160198 humanize-4.5.0/docs/
-drwxr-xr-x   0 huvankem (692055019) wheel        (0)        0 2023-01-29 14:11:55.160468 humanize-4.5.0/docs/css/
--rw-r--r--   0 huvankem (692055019) wheel        (0)      253 2023-01-29 14:07:51.000000 humanize-4.5.0/docs/css/code_select.css
--rw-r--r--   0 huvankem (692055019) wheel        (0)       34 2023-01-29 14:07:51.000000 humanize-4.5.0/docs/filesize.md
--rw-r--r--   0 huvankem (692055019) wheel        (0)       42 2023-01-29 14:07:51.000000 humanize-4.5.0/docs/i18n.md
--rw-r--r--   0 huvankem (692055019) wheel        (0)      244 2023-01-29 14:07:51.000000 humanize-4.5.0/docs/index.md
--rw-r--r--   0 huvankem (692055019) wheel        (0)       30 2023-01-29 14:07:51.000000 humanize-4.5.0/docs/number.md
--rw-r--r--   0 huvankem (692055019) wheel        (0)      123 2023-01-29 14:07:51.000000 humanize-4.5.0/docs/requirements.txt
--rw-r--r--   0 huvankem (692055019) wheel        (0)       26 2023-01-29 14:07:51.000000 humanize-4.5.0/docs/time.md
--rw-r--r--   0 huvankem (692055019) wheel        (0)      857 2023-01-29 14:07:51.000000 humanize-4.5.0/mkdocs.yml
--rw-r--r--   0 huvankem (692055019) wheel        (0)     2121 2023-01-29 14:07:51.000000 humanize-4.5.0/pyproject.toml
-drwxr-xr-x   0 huvankem (692055019) wheel        (0)        0 2023-01-29 14:11:55.161203 humanize-4.5.0/scripts/
--rwxr-xr-x   0 huvankem (692055019) wheel        (0)      204 2023-01-29 14:07:51.000000 humanize-4.5.0/scripts/generate-translation-binaries.sh
--rwxr-xr-x   0 huvankem (692055019) wheel        (0)      528 2023-01-29 14:07:51.000000 humanize-4.5.0/scripts/update-translations.sh
--rw-r--r--   0 huvankem (692055019) wheel        (0)       38 2023-01-29 14:11:55.183769 humanize-4.5.0/setup.cfg
--rw-r--r--   0 huvankem (692055019) wheel        (0)       78 2023-01-29 14:07:51.000000 humanize-4.5.0/setup.py
-drwxr-xr-x   0 huvankem (692055019) wheel        (0)        0 2023-01-29 14:11:55.142430 humanize-4.5.0/src/
-drwxr-xr-x   0 huvankem (692055019) wheel        (0)        0 2023-01-29 14:11:55.163426 humanize-4.5.0/src/humanize/
--rw-r--r--   0 huvankem (692055019) wheel        (0)     1003 2023-01-29 14:07:51.000000 humanize-4.5.0/src/humanize/__init__.py
--rw-r--r--   0 huvankem (692055019) wheel        (0)     2169 2023-01-29 14:07:51.000000 humanize-4.5.0/src/humanize/filesize.py
--rw-r--r--   0 huvankem (692055019) wheel        (0)     5091 2023-01-29 14:07:51.000000 humanize-4.5.0/src/humanize/i18n.py
-drwxr-xr-x   0 huvankem (692055019) wheel        (0)        0 2023-01-29 14:11:55.150903 humanize-4.5.0/src/humanize/locale/
-drwxr-xr-x   0 huvankem (692055019) wheel        (0)        0 2023-01-29 14:11:55.142748 humanize-4.5.0/src/humanize/locale/ar/
-drwxr-xr-x   0 huvankem (692055019) wheel        (0)        0 2023-01-29 14:11:55.165395 humanize-4.5.0/src/humanize/locale/ar/LC_MESSAGES/
--rw-r--r--   0 huvankem (692055019) wheel        (0)     3856 2023-01-29 14:07:51.000000 humanize-4.5.0/src/humanize/locale/ar/LC_MESSAGES/humanize.mo
--rw-r--r--   0 huvankem (692055019) wheel        (0)     6933 2023-01-29 14:07:51.000000 humanize-4.5.0/src/humanize/locale/ar/LC_MESSAGES/humanize.po
-drwxr-xr-x   0 huvankem (692055019) wheel        (0)        0 2023-01-29 14:11:55.142978 humanize-4.5.0/src/humanize/locale/bn_BD/
-drwxr-xr-x   0 huvankem (692055019) wheel        (0)        0 2023-01-29 14:11:55.166084 humanize-4.5.0/src/humanize/locale/bn_BD/LC_MESSAGES/
--rw-r--r--   0 huvankem (692055019) wheel        (0)     2399 2023-01-29 14:07:51.000000 humanize-4.5.0/src/humanize/locale/bn_BD/LC_MESSAGES/humanize.mo
--rw-r--r--   0 huvankem (692055019) wheel        (0)     5554 2023-01-29 14:07:51.000000 humanize-4.5.0/src/humanize/locale/bn_BD/LC_MESSAGES/humanize.po
-drwxr-xr-x   0 huvankem (692055019) wheel        (0)        0 2023-01-29 14:11:55.143610 humanize-4.5.0/src/humanize/locale/ca_ES/
-drwxr-xr-x   0 huvankem (692055019) wheel        (0)        0 2023-01-29 14:11:55.166692 humanize-4.5.0/src/humanize/locale/ca_ES/LC_MESSAGES/
--rw-r--r--   0 huvankem (692055019) wheel        (0)     3345 2023-01-29 14:07:51.000000 humanize-4.5.0/src/humanize/locale/ca_ES/LC_MESSAGES/humanize.mo
--rw-r--r--   0 huvankem (692055019) wheel        (0)     6489 2023-01-29 14:07:51.000000 humanize-4.5.0/src/humanize/locale/ca_ES/LC_MESSAGES/humanize.po
-drwxr-xr-x   0 huvankem (692055019) wheel        (0)        0 2023-01-29 14:11:55.143961 humanize-4.5.0/src/humanize/locale/da_DK/
-drwxr-xr-x   0 huvankem (692055019) wheel        (0)        0 2023-01-29 14:11:55.167301 humanize-4.5.0/src/humanize/locale/da_DK/LC_MESSAGES/
--rw-r--r--   0 huvankem (692055019) wheel        (0)     3524 2023-01-29 14:07:51.000000 humanize-4.5.0/src/humanize/locale/da_DK/LC_MESSAGES/humanize.mo
--rw-r--r--   0 huvankem (692055019) wheel        (0)     6619 2023-01-29 14:07:51.000000 humanize-4.5.0/src/humanize/locale/da_DK/LC_MESSAGES/humanize.po
-drwxr-xr-x   0 huvankem (692055019) wheel        (0)        0 2023-01-29 14:11:55.144178 humanize-4.5.0/src/humanize/locale/de_DE/
-drwxr-xr-x   0 huvankem (692055019) wheel        (0)        0 2023-01-29 14:11:55.167955 humanize-4.5.0/src/humanize/locale/de_DE/LC_MESSAGES/
--rw-r--r--   0 huvankem (692055019) wheel        (0)     3356 2023-01-29 14:07:51.000000 humanize-4.5.0/src/humanize/locale/de_DE/LC_MESSAGES/humanize.mo
--rw-r--r--   0 huvankem (692055019) wheel        (0)     6676 2023-01-29 14:07:51.000000 humanize-4.5.0/src/humanize/locale/de_DE/LC_MESSAGES/humanize.po
-drwxr-xr-x   0 huvankem (692055019) wheel        (0)        0 2023-01-29 14:11:55.144393 humanize-4.5.0/src/humanize/locale/el_GR/
-drwxr-xr-x   0 huvankem (692055019) wheel        (0)        0 2023-01-29 14:11:55.168717 humanize-4.5.0/src/humanize/locale/el_GR/LC_MESSAGES/
--rw-r--r--   0 huvankem (692055019) wheel        (0)     4311 2023-01-29 14:07:51.000000 humanize-4.5.0/src/humanize/locale/el_GR/LC_MESSAGES/humanize.mo
--rw-r--r--   0 huvankem (692055019) wheel        (0)     7816 2023-01-29 14:07:51.000000 humanize-4.5.0/src/humanize/locale/el_GR/LC_MESSAGES/humanize.po
-drwxr-xr-x   0 huvankem (692055019) wheel        (0)        0 2023-01-29 14:11:55.144602 humanize-4.5.0/src/humanize/locale/es_ES/
-drwxr-xr-x   0 huvankem (692055019) wheel        (0)        0 2023-01-29 14:11:55.169349 humanize-4.5.0/src/humanize/locale/es_ES/LC_MESSAGES/
--rw-r--r--   0 huvankem (692055019) wheel        (0)     3466 2023-01-29 14:07:51.000000 humanize-4.5.0/src/humanize/locale/es_ES/LC_MESSAGES/humanize.mo
--rw-r--r--   0 huvankem (692055019) wheel        (0)     6594 2023-01-29 14:07:51.000000 humanize-4.5.0/src/humanize/locale/es_ES/LC_MESSAGES/humanize.po
-drwxr-xr-x   0 huvankem (692055019) wheel        (0)        0 2023-01-29 14:11:55.144815 humanize-4.5.0/src/humanize/locale/eu/
-drwxr-xr-x   0 huvankem (692055019) wheel        (0)        0 2023-01-29 14:11:55.169992 humanize-4.5.0/src/humanize/locale/eu/LC_MESSAGES/
--rw-r--r--   0 huvankem (692055019) wheel        (0)     3098 2023-01-29 14:07:51.000000 humanize-4.5.0/src/humanize/locale/eu/LC_MESSAGES/humanize.mo
--rw-r--r--   0 huvankem (692055019) wheel        (0)     6522 2023-01-29 14:07:51.000000 humanize-4.5.0/src/humanize/locale/eu/LC_MESSAGES/humanize.po
-drwxr-xr-x   0 huvankem (692055019) wheel        (0)        0 2023-01-29 14:11:55.145031 humanize-4.5.0/src/humanize/locale/fa_IR/
-drwxr-xr-x   0 huvankem (692055019) wheel        (0)        0 2023-01-29 14:11:55.170582 humanize-4.5.0/src/humanize/locale/fa_IR/LC_MESSAGES/
--rw-r--r--   0 huvankem (692055019) wheel        (0)     4010 2023-01-29 14:07:51.000000 humanize-4.5.0/src/humanize/locale/fa_IR/LC_MESSAGES/humanize.mo
--rw-r--r--   0 huvankem (692055019) wheel        (0)     7124 2023-01-29 14:07:51.000000 humanize-4.5.0/src/humanize/locale/fa_IR/LC_MESSAGES/humanize.po
-drwxr-xr-x   0 huvankem (692055019) wheel        (0)        0 2023-01-29 14:11:55.145236 humanize-4.5.0/src/humanize/locale/fi_FI/
-drwxr-xr-x   0 huvankem (692055019) wheel        (0)        0 2023-01-29 14:11:55.171181 humanize-4.5.0/src/humanize/locale/fi_FI/LC_MESSAGES/
--rw-r--r--   0 huvankem (692055019) wheel        (0)     3369 2023-01-29 14:07:51.000000 humanize-4.5.0/src/humanize/locale/fi_FI/LC_MESSAGES/humanize.mo
--rw-r--r--   0 huvankem (692055019) wheel        (0)     6697 2023-01-29 14:07:51.000000 humanize-4.5.0/src/humanize/locale/fi_FI/LC_MESSAGES/humanize.po
-drwxr-xr-x   0 huvankem (692055019) wheel        (0)        0 2023-01-29 14:11:55.145448 humanize-4.5.0/src/humanize/locale/fr_FR/
-drwxr-xr-x   0 huvankem (692055019) wheel        (0)        0 2023-01-29 14:11:55.171781 humanize-4.5.0/src/humanize/locale/fr_FR/LC_MESSAGES/
--rw-r--r--   0 huvankem (692055019) wheel        (0)     2645 2023-01-29 14:07:51.000000 humanize-4.5.0/src/humanize/locale/fr_FR/LC_MESSAGES/humanize.mo
--rw-r--r--   0 huvankem (692055019) wheel        (0)     6905 2023-01-29 14:07:51.000000 humanize-4.5.0/src/humanize/locale/fr_FR/LC_MESSAGES/humanize.po
-drwxr-xr-x   0 huvankem (692055019) wheel        (0)        0 2023-01-29 14:11:55.145755 humanize-4.5.0/src/humanize/locale/id_ID/
-drwxr-xr-x   0 huvankem (692055019) wheel        (0)        0 2023-01-29 14:11:55.172491 humanize-4.5.0/src/humanize/locale/id_ID/LC_MESSAGES/
--rw-r--r--   0 huvankem (692055019) wheel        (0)     3005 2023-01-29 14:07:51.000000 humanize-4.5.0/src/humanize/locale/id_ID/LC_MESSAGES/humanize.mo
--rw-r--r--   0 huvankem (692055019) wheel        (0)     6057 2023-01-29 14:07:51.000000 humanize-4.5.0/src/humanize/locale/id_ID/LC_MESSAGES/humanize.po
-drwxr-xr-x   0 huvankem (692055019) wheel        (0)        0 2023-01-29 14:11:55.146001 humanize-4.5.0/src/humanize/locale/it_IT/
-drwxr-xr-x   0 huvankem (692055019) wheel        (0)        0 2023-01-29 14:11:55.173072 humanize-4.5.0/src/humanize/locale/it_IT/LC_MESSAGES/
--rw-r--r--   0 huvankem (692055019) wheel        (0)     3188 2023-01-29 14:07:51.000000 humanize-4.5.0/src/humanize/locale/it_IT/LC_MESSAGES/humanize.mo
--rw-r--r--   0 huvankem (692055019) wheel        (0)     6565 2023-01-29 14:07:51.000000 humanize-4.5.0/src/humanize/locale/it_IT/LC_MESSAGES/humanize.po
-drwxr-xr-x   0 huvankem (692055019) wheel        (0)        0 2023-01-29 14:11:55.146237 humanize-4.5.0/src/humanize/locale/ja_JP/
-drwxr-xr-x   0 huvankem (692055019) wheel        (0)        0 2023-01-29 14:11:55.173672 humanize-4.5.0/src/humanize/locale/ja_JP/LC_MESSAGES/
--rw-r--r--   0 huvankem (692055019) wheel        (0)     2457 2023-01-29 14:07:51.000000 humanize-4.5.0/src/humanize/locale/ja_JP/LC_MESSAGES/humanize.mo
--rw-r--r--   0 huvankem (692055019) wheel        (0)     6107 2023-01-29 14:07:51.000000 humanize-4.5.0/src/humanize/locale/ja_JP/LC_MESSAGES/humanize.po
-drwxr-xr-x   0 huvankem (692055019) wheel        (0)        0 2023-01-29 14:11:55.148321 humanize-4.5.0/src/humanize/locale/ko_KR/
-drwxr-xr-x   0 huvankem (692055019) wheel        (0)        0 2023-01-29 14:11:55.174260 humanize-4.5.0/src/humanize/locale/ko_KR/LC_MESSAGES/
--rw-r--r--   0 huvankem (692055019) wheel        (0)     2016 2023-01-29 14:07:51.000000 humanize-4.5.0/src/humanize/locale/ko_KR/LC_MESSAGES/humanize.mo
--rw-r--r--   0 huvankem (692055019) wheel        (0)     7019 2023-01-29 14:07:51.000000 humanize-4.5.0/src/humanize/locale/ko_KR/LC_MESSAGES/humanize.po
-drwxr-xr-x   0 huvankem (692055019) wheel        (0)        0 2023-01-29 14:11:55.148724 humanize-4.5.0/src/humanize/locale/nl_NL/
-drwxr-xr-x   0 huvankem (692055019) wheel        (0)        0 2023-01-29 14:11:55.174855 humanize-4.5.0/src/humanize/locale/nl_NL/LC_MESSAGES/
--rw-r--r--   0 huvankem (692055019) wheel        (0)     3258 2023-01-29 14:07:51.000000 humanize-4.5.0/src/humanize/locale/nl_NL/LC_MESSAGES/humanize.mo
--rw-r--r--   0 huvankem (692055019) wheel        (0)     6604 2023-01-29 14:07:51.000000 humanize-4.5.0/src/humanize/locale/nl_NL/LC_MESSAGES/humanize.po
-drwxr-xr-x   0 huvankem (692055019) wheel        (0)        0 2023-01-29 14:11:55.148962 humanize-4.5.0/src/humanize/locale/pl_PL/
-drwxr-xr-x   0 huvankem (692055019) wheel        (0)        0 2023-01-29 14:11:55.175459 humanize-4.5.0/src/humanize/locale/pl_PL/LC_MESSAGES/
--rw-r--r--   0 huvankem (692055019) wheel        (0)     3753 2023-01-29 14:07:51.000000 humanize-4.5.0/src/humanize/locale/pl_PL/LC_MESSAGES/humanize.mo
--rw-r--r--   0 huvankem (692055019) wheel        (0)     7291 2023-01-29 14:07:51.000000 humanize-4.5.0/src/humanize/locale/pl_PL/LC_MESSAGES/humanize.po
-drwxr-xr-x   0 huvankem (692055019) wheel        (0)        0 2023-01-29 14:11:55.149153 humanize-4.5.0/src/humanize/locale/pt_BR/
-drwxr-xr-x   0 huvankem (692055019) wheel        (0)        0 2023-01-29 14:11:55.176061 humanize-4.5.0/src/humanize/locale/pt_BR/LC_MESSAGES/
--rw-r--r--   0 huvankem (692055019) wheel        (0)     3184 2023-01-29 14:07:51.000000 humanize-4.5.0/src/humanize/locale/pt_BR/LC_MESSAGES/humanize.mo
--rw-r--r--   0 huvankem (692055019) wheel        (0)     6524 2023-01-29 14:07:51.000000 humanize-4.5.0/src/humanize/locale/pt_BR/LC_MESSAGES/humanize.po
-drwxr-xr-x   0 huvankem (692055019) wheel        (0)        0 2023-01-29 14:11:55.149336 humanize-4.5.0/src/humanize/locale/pt_PT/
-drwxr-xr-x   0 huvankem (692055019) wheel        (0)        0 2023-01-29 14:11:55.176661 humanize-4.5.0/src/humanize/locale/pt_PT/LC_MESSAGES/
--rw-r--r--   0 huvankem (692055019) wheel        (0)     3403 2023-01-29 14:07:51.000000 humanize-4.5.0/src/humanize/locale/pt_PT/LC_MESSAGES/humanize.mo
--rw-r--r--   0 huvankem (692055019) wheel        (0)     6567 2023-01-29 14:07:51.000000 humanize-4.5.0/src/humanize/locale/pt_PT/LC_MESSAGES/humanize.po
-drwxr-xr-x   0 huvankem (692055019) wheel        (0)        0 2023-01-29 14:11:55.149516 humanize-4.5.0/src/humanize/locale/ru_RU/
-drwxr-xr-x   0 huvankem (692055019) wheel        (0)        0 2023-01-29 14:11:55.177319 humanize-4.5.0/src/humanize/locale/ru_RU/LC_MESSAGES/
--rw-r--r--   0 huvankem (692055019) wheel        (0)     4538 2023-01-29 14:07:51.000000 humanize-4.5.0/src/humanize/locale/ru_RU/LC_MESSAGES/humanize.mo
--rw-r--r--   0 huvankem (692055019) wheel        (0)     7906 2023-01-29 14:07:51.000000 humanize-4.5.0/src/humanize/locale/ru_RU/LC_MESSAGES/humanize.po
-drwxr-xr-x   0 huvankem (692055019) wheel        (0)        0 2023-01-29 14:11:55.149684 humanize-4.5.0/src/humanize/locale/sk_SK/
-drwxr-xr-x   0 huvankem (692055019) wheel        (0)        0 2023-01-29 14:11:55.177910 humanize-4.5.0/src/humanize/locale/sk_SK/LC_MESSAGES/
--rw-r--r--   0 huvankem (692055019) wheel        (0)     3540 2023-01-29 14:07:51.000000 humanize-4.5.0/src/humanize/locale/sk_SK/LC_MESSAGES/humanize.mo
--rw-r--r--   0 huvankem (692055019) wheel        (0)     7180 2023-01-29 14:07:51.000000 humanize-4.5.0/src/humanize/locale/sk_SK/LC_MESSAGES/humanize.po
-drwxr-xr-x   0 huvankem (692055019) wheel        (0)        0 2023-01-29 14:11:55.149844 humanize-4.5.0/src/humanize/locale/sl_SI/
-drwxr-xr-x   0 huvankem (692055019) wheel        (0)        0 2023-01-29 14:11:55.178479 humanize-4.5.0/src/humanize/locale/sl_SI/LC_MESSAGES/
--rw-r--r--   0 huvankem (692055019) wheel        (0)     3979 2023-01-29 14:07:51.000000 humanize-4.5.0/src/humanize/locale/sl_SI/LC_MESSAGES/humanize.mo
--rw-r--r--   0 huvankem (692055019) wheel        (0)     7618 2023-01-29 14:07:51.000000 humanize-4.5.0/src/humanize/locale/sl_SI/LC_MESSAGES/humanize.po
-drwxr-xr-x   0 huvankem (692055019) wheel        (0)        0 2023-01-29 14:11:55.150003 humanize-4.5.0/src/humanize/locale/sv_SE/
-drwxr-xr-x   0 huvankem (692055019) wheel        (0)        0 2023-01-29 14:11:55.179076 humanize-4.5.0/src/humanize/locale/sv_SE/LC_MESSAGES/
--rw-r--r--   0 huvankem (692055019) wheel        (0)     3498 2023-01-29 14:07:51.000000 humanize-4.5.0/src/humanize/locale/sv_SE/LC_MESSAGES/humanize.mo
--rw-r--r--   0 huvankem (692055019) wheel        (0)     6596 2023-01-29 14:07:51.000000 humanize-4.5.0/src/humanize/locale/sv_SE/LC_MESSAGES/humanize.po
-drwxr-xr-x   0 huvankem (692055019) wheel        (0)        0 2023-01-29 14:11:55.150235 humanize-4.5.0/src/humanize/locale/tr_TR/
-drwxr-xr-x   0 huvankem (692055019) wheel        (0)        0 2023-01-29 14:11:55.179776 humanize-4.5.0/src/humanize/locale/tr_TR/LC_MESSAGES/
--rw-r--r--   0 huvankem (692055019) wheel        (0)     3151 2023-01-29 14:07:51.000000 humanize-4.5.0/src/humanize/locale/tr_TR/LC_MESSAGES/humanize.mo
--rw-r--r--   0 huvankem (692055019) wheel        (0)     6479 2023-01-29 14:07:51.000000 humanize-4.5.0/src/humanize/locale/tr_TR/LC_MESSAGES/humanize.po
-drwxr-xr-x   0 huvankem (692055019) wheel        (0)        0 2023-01-29 14:11:55.150391 humanize-4.5.0/src/humanize/locale/uk_UA/
-drwxr-xr-x   0 huvankem (692055019) wheel        (0)        0 2023-01-29 14:11:55.180394 humanize-4.5.0/src/humanize/locale/uk_UA/LC_MESSAGES/
--rw-r--r--   0 huvankem (692055019) wheel        (0)     4188 2023-01-29 14:07:51.000000 humanize-4.5.0/src/humanize/locale/uk_UA/LC_MESSAGES/humanize.mo
--rw-r--r--   0 huvankem (692055019) wheel        (0)     7661 2023-01-29 14:07:51.000000 humanize-4.5.0/src/humanize/locale/uk_UA/LC_MESSAGES/humanize.po
-drwxr-xr-x   0 huvankem (692055019) wheel        (0)        0 2023-01-29 14:11:55.150588 humanize-4.5.0/src/humanize/locale/vi_VN/
-drwxr-xr-x   0 huvankem (692055019) wheel        (0)        0 2023-01-29 14:11:55.180990 humanize-4.5.0/src/humanize/locale/vi_VN/LC_MESSAGES/
--rw-r--r--   0 huvankem (692055019) wheel        (0)     3164 2023-01-29 14:07:51.000000 humanize-4.5.0/src/humanize/locale/vi_VN/LC_MESSAGES/humanize.mo
--rw-r--r--   0 huvankem (692055019) wheel        (0)     6920 2023-01-29 14:07:51.000000 humanize-4.5.0/src/humanize/locale/vi_VN/LC_MESSAGES/humanize.po
-drwxr-xr-x   0 huvankem (692055019) wheel        (0)        0 2023-01-29 14:11:55.150805 humanize-4.5.0/src/humanize/locale/zh_CN/
-drwxr-xr-x   0 huvankem (692055019) wheel        (0)        0 2023-01-29 14:11:55.181593 humanize-4.5.0/src/humanize/locale/zh_CN/LC_MESSAGES/
--rw-r--r--   0 huvankem (692055019) wheel        (0)     3011 2023-01-29 14:07:51.000000 humanize-4.5.0/src/humanize/locale/zh_CN/LC_MESSAGES/humanize.mo
--rw-r--r--   0 huvankem (692055019) wheel        (0)     6359 2023-01-29 14:07:51.000000 humanize-4.5.0/src/humanize/locale/zh_CN/LC_MESSAGES/humanize.po
-drwxr-xr-x   0 huvankem (692055019) wheel        (0)        0 2023-01-29 14:11:55.151004 humanize-4.5.0/src/humanize/locale/zh_HK/
-drwxr-xr-x   0 huvankem (692055019) wheel        (0)        0 2023-01-29 14:11:55.182197 humanize-4.5.0/src/humanize/locale/zh_HK/LC_MESSAGES/
--rw-r--r--   0 huvankem (692055019) wheel        (0)     3323 2023-01-29 14:07:51.000000 humanize-4.5.0/src/humanize/locale/zh_HK/LC_MESSAGES/humanize.mo
--rw-r--r--   0 huvankem (692055019) wheel        (0)     6495 2023-01-29 14:07:51.000000 humanize-4.5.0/src/humanize/locale/zh_HK/LC_MESSAGES/humanize.po
--rw-r--r--   0 huvankem (692055019) wheel        (0)    16249 2023-01-29 14:07:51.000000 humanize-4.5.0/src/humanize/number.py
--rw-r--r--   0 huvankem (692055019) wheel        (0)        0 2023-01-29 14:07:51.000000 humanize-4.5.0/src/humanize/py.typed
--rw-r--r--   0 huvankem (692055019) wheel        (0)    18259 2023-01-29 14:07:51.000000 humanize-4.5.0/src/humanize/time.py
-drwxr-xr-x   0 huvankem (692055019) wheel        (0)        0 2023-01-29 14:11:55.164711 humanize-4.5.0/src/humanize.egg-info/
--rw-r--r--   0 huvankem (692055019) wheel        (0)     7701 2023-01-29 14:11:55.000000 humanize-4.5.0/src/humanize.egg-info/PKG-INFO
--rw-r--r--   0 huvankem (692055019) wheel        (0)     3919 2023-01-29 14:11:55.000000 humanize-4.5.0/src/humanize.egg-info/SOURCES.txt
--rw-r--r--   0 huvankem (692055019) wheel        (0)        1 2023-01-29 14:11:55.000000 humanize-4.5.0/src/humanize.egg-info/dependency_links.txt
--rw-r--r--   0 huvankem (692055019) wheel        (0)       83 2023-01-29 14:11:55.000000 humanize-4.5.0/src/humanize.egg-info/requires.txt
--rw-r--r--   0 huvankem (692055019) wheel        (0)        9 2023-01-29 14:11:55.000000 humanize-4.5.0/src/humanize.egg-info/top_level.txt
-drwxr-xr-x   0 huvankem (692055019) wheel        (0)        0 2023-01-29 14:11:55.183259 humanize-4.5.0/tests/
--rw-r--r--   0 huvankem (692055019) wheel        (0)        0 2023-01-29 14:07:51.000000 humanize-4.5.0/tests/__init__.py
--rw-r--r--   0 huvankem (692055019) wheel        (0)     1292 2023-01-29 14:07:51.000000 humanize-4.5.0/tests/test_filesize.py
--rw-r--r--   0 huvankem (692055019) wheel        (0)     6113 2023-01-29 14:07:51.000000 humanize-4.5.0/tests/test_i18n.py
--rw-r--r--   0 huvankem (692055019) wheel        (0)     8401 2023-01-29 14:07:51.000000 humanize-4.5.0/tests/test_number.py
--rw-r--r--   0 huvankem (692055019) wheel        (0)    23833 2023-01-29 14:07:51.000000 humanize-4.5.0/tests/test_time.py
--rw-r--r--   0 huvankem (692055019) wheel        (0)      503 2023-01-29 14:07:51.000000 humanize-4.5.0/tox.ini
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 humanize-4.6.0/.flake8
+-rw-r--r--   0        0        0     1923 2020-02-02 00:00:00.000000 humanize-4.6.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 humanize-4.6.0/.readthedocs.yml
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 humanize-4.6.0/MANIFEST.in
+-rw-r--r--   0        0        0     1690 2020-02-02 00:00:00.000000 humanize-4.6.0/RELEASING.md
+-rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 humanize-4.6.0/mkdocs.yml
+-rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 humanize-4.6.0/tox.ini
+-rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 humanize-4.6.0/.github/CONTRIBUTING.md
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 humanize-4.6.0/.github/FUNDING.yml
+-rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 humanize-4.6.0/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 humanize-4.6.0/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 humanize-4.6.0/.github/SECURITY.md
+-rw-r--r--   0        0        0     1950 2020-02-02 00:00:00.000000 humanize-4.6.0/.github/labels.yml
+-rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 humanize-4.6.0/.github/release-drafter.yml
+-rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 humanize-4.6.0/.github/renovate.json
+-rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 humanize-4.6.0/.github/workflows/docs.yml
+-rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 humanize-4.6.0/.github/workflows/labels.yml
+-rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 humanize-4.6.0/.github/workflows/lint.yml
+-rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 humanize-4.6.0/.github/workflows/release-drafter.yml
+-rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 humanize-4.6.0/.github/workflows/require-pr-label.yml
+-rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 humanize-4.6.0/.github/workflows/test.yml
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 humanize-4.6.0/docs/filesize.md
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 humanize-4.6.0/docs/i18n.md
+-rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 humanize-4.6.0/docs/index.md
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 humanize-4.6.0/docs/number.md
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 humanize-4.6.0/docs/requirements.txt
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 humanize-4.6.0/docs/time.md
+-rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 humanize-4.6.0/docs/css/code_select.css
+-rwxr-xr-x   0        0        0      204 2020-02-02 00:00:00.000000 humanize-4.6.0/scripts/generate-translation-binaries.sh
+-rwxr-xr-x   0        0        0      465 2020-02-02 00:00:00.000000 humanize-4.6.0/scripts/update-translations.sh
+-rw-r--r--   0        0        0     1003 2020-02-02 00:00:00.000000 humanize-4.6.0/src/humanize/__init__.py
+-rw-r--r--   0        0        0     2169 2020-02-02 00:00:00.000000 humanize-4.6.0/src/humanize/filesize.py
+-rw-r--r--   0        0        0     5127 2020-02-02 00:00:00.000000 humanize-4.6.0/src/humanize/i18n.py
+-rw-r--r--   0        0        0    16249 2020-02-02 00:00:00.000000 humanize-4.6.0/src/humanize/number.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 humanize-4.6.0/src/humanize/py.typed
+-rw-r--r--   0        0        0    18259 2020-02-02 00:00:00.000000 humanize-4.6.0/src/humanize/time.py
+-rw-r--r--   0        0        0     3856 2020-02-02 00:00:00.000000 humanize-4.6.0/src/humanize/locale/ar/LC_MESSAGES/humanize.mo
+-rw-r--r--   0        0        0     7034 2020-02-02 00:00:00.000000 humanize-4.6.0/src/humanize/locale/ar/LC_MESSAGES/humanize.po
+-rw-r--r--   0        0        0     2399 2020-02-02 00:00:00.000000 humanize-4.6.0/src/humanize/locale/bn_BD/LC_MESSAGES/humanize.mo
+-rw-r--r--   0        0        0     6905 2020-02-02 00:00:00.000000 humanize-4.6.0/src/humanize/locale/bn_BD/LC_MESSAGES/humanize.po
+-rw-r--r--   0        0        0     3345 2020-02-02 00:00:00.000000 humanize-4.6.0/src/humanize/locale/ca_ES/LC_MESSAGES/humanize.mo
+-rw-r--r--   0        0        0     6496 2020-02-02 00:00:00.000000 humanize-4.6.0/src/humanize/locale/ca_ES/LC_MESSAGES/humanize.po
+-rw-r--r--   0        0        0     3474 2020-02-02 00:00:00.000000 humanize-4.6.0/src/humanize/locale/da_DK/LC_MESSAGES/humanize.mo
+-rw-r--r--   0        0        0     6576 2020-02-02 00:00:00.000000 humanize-4.6.0/src/humanize/locale/da_DK/LC_MESSAGES/humanize.po
+-rw-r--r--   0        0        0     3356 2020-02-02 00:00:00.000000 humanize-4.6.0/src/humanize/locale/de_DE/LC_MESSAGES/humanize.mo
+-rw-r--r--   0        0        0     6683 2020-02-02 00:00:00.000000 humanize-4.6.0/src/humanize/locale/de_DE/LC_MESSAGES/humanize.po
+-rw-r--r--   0        0        0     3559 2020-02-02 00:00:00.000000 humanize-4.6.0/src/humanize/locale/el_GR/LC_MESSAGES/humanize.mo
+-rw-r--r--   0        0        0     8843 2020-02-02 00:00:00.000000 humanize-4.6.0/src/humanize/locale/el_GR/LC_MESSAGES/humanize.po
+-rw-r--r--   0        0        0     3466 2020-02-02 00:00:00.000000 humanize-4.6.0/src/humanize/locale/es_ES/LC_MESSAGES/humanize.mo
+-rw-r--r--   0        0        0     6601 2020-02-02 00:00:00.000000 humanize-4.6.0/src/humanize/locale/es_ES/LC_MESSAGES/humanize.po
+-rw-r--r--   0        0        0     3098 2020-02-02 00:00:00.000000 humanize-4.6.0/src/humanize/locale/eu/LC_MESSAGES/humanize.mo
+-rw-r--r--   0        0        0     6522 2020-02-02 00:00:00.000000 humanize-4.6.0/src/humanize/locale/eu/LC_MESSAGES/humanize.po
+-rw-r--r--   0        0        0     4010 2020-02-02 00:00:00.000000 humanize-4.6.0/src/humanize/locale/fa_IR/LC_MESSAGES/humanize.mo
+-rw-r--r--   0        0        0     7131 2020-02-02 00:00:00.000000 humanize-4.6.0/src/humanize/locale/fa_IR/LC_MESSAGES/humanize.po
+-rw-r--r--   0        0        0     3369 2020-02-02 00:00:00.000000 humanize-4.6.0/src/humanize/locale/fi_FI/LC_MESSAGES/humanize.mo
+-rw-r--r--   0        0        0     6704 2020-02-02 00:00:00.000000 humanize-4.6.0/src/humanize/locale/fi_FI/LC_MESSAGES/humanize.po
+-rw-r--r--   0        0        0     2645 2020-02-02 00:00:00.000000 humanize-4.6.0/src/humanize/locale/fr_FR/LC_MESSAGES/humanize.mo
+-rw-r--r--   0        0        0     6912 2020-02-02 00:00:00.000000 humanize-4.6.0/src/humanize/locale/fr_FR/LC_MESSAGES/humanize.po
+-rw-r--r--   0        0        0     3005 2020-02-02 00:00:00.000000 humanize-4.6.0/src/humanize/locale/id_ID/LC_MESSAGES/humanize.mo
+-rw-r--r--   0        0        0     6064 2020-02-02 00:00:00.000000 humanize-4.6.0/src/humanize/locale/id_ID/LC_MESSAGES/humanize.po
+-rw-r--r--   0        0        0     3274 2020-02-02 00:00:00.000000 humanize-4.6.0/src/humanize/locale/it_IT/LC_MESSAGES/humanize.mo
+-rw-r--r--   0        0        0     6595 2020-02-02 00:00:00.000000 humanize-4.6.0/src/humanize/locale/it_IT/LC_MESSAGES/humanize.po
+-rw-r--r--   0        0        0     2457 2020-02-02 00:00:00.000000 humanize-4.6.0/src/humanize/locale/ja_JP/LC_MESSAGES/humanize.mo
+-rw-r--r--   0        0        0     6114 2020-02-02 00:00:00.000000 humanize-4.6.0/src/humanize/locale/ja_JP/LC_MESSAGES/humanize.po
+-rw-r--r--   0        0        0     2016 2020-02-02 00:00:00.000000 humanize-4.6.0/src/humanize/locale/ko_KR/LC_MESSAGES/humanize.mo
+-rw-r--r--   0        0        0     7026 2020-02-02 00:00:00.000000 humanize-4.6.0/src/humanize/locale/ko_KR/LC_MESSAGES/humanize.po
+-rw-r--r--   0        0        0     3258 2020-02-02 00:00:00.000000 humanize-4.6.0/src/humanize/locale/nl_NL/LC_MESSAGES/humanize.mo
+-rw-r--r--   0        0        0     6611 2020-02-02 00:00:00.000000 humanize-4.6.0/src/humanize/locale/nl_NL/LC_MESSAGES/humanize.po
+-rw-r--r--   0        0        0     3753 2020-02-02 00:00:00.000000 humanize-4.6.0/src/humanize/locale/pl_PL/LC_MESSAGES/humanize.mo
+-rw-r--r--   0        0        0     7298 2020-02-02 00:00:00.000000 humanize-4.6.0/src/humanize/locale/pl_PL/LC_MESSAGES/humanize.po
+-rw-r--r--   0        0        0     3184 2020-02-02 00:00:00.000000 humanize-4.6.0/src/humanize/locale/pt_BR/LC_MESSAGES/humanize.mo
+-rw-r--r--   0        0        0     6531 2020-02-02 00:00:00.000000 humanize-4.6.0/src/humanize/locale/pt_BR/LC_MESSAGES/humanize.po
+-rw-r--r--   0        0        0     3403 2020-02-02 00:00:00.000000 humanize-4.6.0/src/humanize/locale/pt_PT/LC_MESSAGES/humanize.mo
+-rw-r--r--   0        0        0     6574 2020-02-02 00:00:00.000000 humanize-4.6.0/src/humanize/locale/pt_PT/LC_MESSAGES/humanize.po
+-rw-r--r--   0        0        0     4538 2020-02-02 00:00:00.000000 humanize-4.6.0/src/humanize/locale/ru_RU/LC_MESSAGES/humanize.mo
+-rw-r--r--   0        0        0     7913 2020-02-02 00:00:00.000000 humanize-4.6.0/src/humanize/locale/ru_RU/LC_MESSAGES/humanize.po
+-rw-r--r--   0        0        0     3540 2020-02-02 00:00:00.000000 humanize-4.6.0/src/humanize/locale/sk_SK/LC_MESSAGES/humanize.mo
+-rw-r--r--   0        0        0     7187 2020-02-02 00:00:00.000000 humanize-4.6.0/src/humanize/locale/sk_SK/LC_MESSAGES/humanize.po
+-rw-r--r--   0        0        0     3979 2020-02-02 00:00:00.000000 humanize-4.6.0/src/humanize/locale/sl_SI/LC_MESSAGES/humanize.mo
+-rw-r--r--   0        0        0     7625 2020-02-02 00:00:00.000000 humanize-4.6.0/src/humanize/locale/sl_SI/LC_MESSAGES/humanize.po
+-rw-r--r--   0        0        0     3448 2020-02-02 00:00:00.000000 humanize-4.6.0/src/humanize/locale/sv_SE/LC_MESSAGES/humanize.mo
+-rw-r--r--   0        0        0     6553 2020-02-02 00:00:00.000000 humanize-4.6.0/src/humanize/locale/sv_SE/LC_MESSAGES/humanize.po
+-rw-r--r--   0        0        0     3151 2020-02-02 00:00:00.000000 humanize-4.6.0/src/humanize/locale/tr_TR/LC_MESSAGES/humanize.mo
+-rw-r--r--   0        0        0     6486 2020-02-02 00:00:00.000000 humanize-4.6.0/src/humanize/locale/tr_TR/LC_MESSAGES/humanize.po
+-rw-r--r--   0        0        0     4188 2020-02-02 00:00:00.000000 humanize-4.6.0/src/humanize/locale/uk_UA/LC_MESSAGES/humanize.mo
+-rw-r--r--   0        0        0     7668 2020-02-02 00:00:00.000000 humanize-4.6.0/src/humanize/locale/uk_UA/LC_MESSAGES/humanize.po
+-rw-r--r--   0        0        0     3164 2020-02-02 00:00:00.000000 humanize-4.6.0/src/humanize/locale/vi_VN/LC_MESSAGES/humanize.mo
+-rw-r--r--   0        0        0     6927 2020-02-02 00:00:00.000000 humanize-4.6.0/src/humanize/locale/vi_VN/LC_MESSAGES/humanize.po
+-rw-r--r--   0        0        0     3011 2020-02-02 00:00:00.000000 humanize-4.6.0/src/humanize/locale/zh_CN/LC_MESSAGES/humanize.mo
+-rw-r--r--   0        0        0     6366 2020-02-02 00:00:00.000000 humanize-4.6.0/src/humanize/locale/zh_CN/LC_MESSAGES/humanize.po
+-rw-r--r--   0        0        0     3323 2020-02-02 00:00:00.000000 humanize-4.6.0/src/humanize/locale/zh_HK/LC_MESSAGES/humanize.mo
+-rw-r--r--   0        0        0     6502 2020-02-02 00:00:00.000000 humanize-4.6.0/src/humanize/locale/zh_HK/LC_MESSAGES/humanize.po
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 humanize-4.6.0/tests/__init__.py
+-rw-r--r--   0        0        0     1292 2020-02-02 00:00:00.000000 humanize-4.6.0/tests/test_filesize.py
+-rw-r--r--   0        0        0     6113 2020-02-02 00:00:00.000000 humanize-4.6.0/tests/test_i18n.py
+-rw-r--r--   0        0        0     8401 2020-02-02 00:00:00.000000 humanize-4.6.0/tests/test_number.py
+-rw-r--r--   0        0        0    23833 2020-02-02 00:00:00.000000 humanize-4.6.0/tests/test_time.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 humanize-4.6.0/.gitignore
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 humanize-4.6.0/LICENCE
+-rw-r--r--   0        0        0     6117 2020-02-02 00:00:00.000000 humanize-4.6.0/README.md
+-rw-r--r--   0        0        0     2081 2020-02-02 00:00:00.000000 humanize-4.6.0/pyproject.toml
+-rw-r--r--   0        0        0     7916 2020-02-02 00:00:00.000000 humanize-4.6.0/PKG-INFO
```

### Comparing `humanize-4.5.0/.github/CONTRIBUTING.md` & `humanize-4.6.0/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `humanize-4.5.0/.github/labels.yml` & `humanize-4.6.0/.github/labels.yml`

 * *Files identical despite different names*

### Comparing `humanize-4.5.0/.github/release-drafter.yml` & `humanize-4.6.0/.github/release-drafter.yml`

 * *Files identical despite different names*

### Comparing `humanize-4.5.0/.github/workflows/test.yml` & `humanize-4.6.0/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `humanize-4.5.0/.gitignore` & `humanize-4.6.0/.gitignore`

 * *Files identical despite different names*

### Comparing `humanize-4.5.0/.pre-commit-config.yaml` & `humanize-4.6.0/.pre-commit-config.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
   - repo: https://github.com/psf/black
     rev: 22.12.0
     hooks:
       - id: black
         args: [--target-version=py37]
 
   - repo: https://github.com/PyCQA/isort
-    rev: 5.11.4
+    rev: 5.12.0
     hooks:
       - id: isort
 
   - repo: https://github.com/PyCQA/autoflake
     rev: v2.0.0
     hooks:
       - id: autoflake
@@ -33,52 +33,52 @@
   - repo: https://github.com/PyCQA/flake8
     rev: 6.0.0
     hooks:
       - id: flake8
         additional_dependencies: [flake8-2020, flake8-errmsg, flake8-implicit-str-concat]
 
   - repo: https://github.com/pre-commit/pygrep-hooks
-    rev: v1.9.0
+    rev: v1.10.0
     hooks:
       - id: python-check-blanket-noqa
       - id: python-no-log-warn
 
   - repo: https://github.com/pre-commit/pre-commit-hooks
     rev: v4.4.0
     hooks:
       - id: check-json
       - id: check-merge-conflict
       - id: check-toml
       - id: check-yaml
       - id: end-of-file-fixer
 
   - repo: https://github.com/PyCQA/pydocstyle
-    rev: 6.2.0
+    rev: 6.3.0
     hooks:
       - id: pydocstyle
         args: ["--convention", "google"]
         files: "src/"
 
   - repo: https://github.com/pre-commit/mirrors-mypy
     rev: v0.991
     hooks:
       - id: mypy
         additional_dependencies: [pytest, types-freezegun, types-setuptools]
         args: [--strict]
 
   - repo: https://github.com/tox-dev/pyproject-fmt
-    rev: 0.4.1
+    rev: 0.5.0
     hooks:
       - id: pyproject-fmt
 
   - repo: https://github.com/abravalheri/validate-pyproject
-    rev: v0.10.1
+    rev: v0.12.1
     hooks:
       - id: validate-pyproject
 
   - repo: https://github.com/tox-dev/tox-ini-fmt
-    rev: 0.5.2
+    rev: 0.6.1
     hooks:
       - id: tox-ini-fmt
 
 ci:
   autoupdate_schedule: quarterly
```

### Comparing `humanize-4.5.0/LICENCE` & `humanize-4.6.0/LICENCE`

 * *Files identical despite different names*

### Comparing `humanize-4.5.0/PKG-INFO` & `humanize-4.6.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: humanize
-Version: 4.5.0
+Version: 4.6.0
 Summary: Python humanize utilities
-Author-email: Jason Moiron <jmoiron@jmoiron.net>
-Maintainer: Hugo van Kemenade
-License: MIT
 Project-URL: Documentation, https://python-humanize.readthedocs.io/
 Project-URL: Funding, https://tidelift.com/subscription/pkg/pypi-humanize?utm_source=pypi-humanize&utm_medium=pypi
 Project-URL: Homepage, https://github.com/python-humanize/humanize
 Project-URL: Issue tracker, https://github.com/python-humanize/humanize/issues
 Project-URL: Release notes, https://github.com/python-humanize/humanize/releases
 Project-URL: Source, https://github.com/python-humanize/humanize
+Author-email: Jason Moiron <jmoiron@jmoiron.net>
+Maintainer: Hugo van Kemenade
+License: MIT
+License-File: LICENCE
 Keywords: humanize time size
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -25,17 +26,20 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Text Processing
 Classifier: Topic :: Text Processing :: General
 Requires-Python: >=3.7
-Description-Content-Type: text/markdown
+Requires-Dist: importlib-metadata; python_version < '3.8'
 Provides-Extra: tests
-License-File: LICENCE
+Requires-Dist: freezegun; extra == 'tests'
+Requires-Dist: pytest; extra == 'tests'
+Requires-Dist: pytest-cov; extra == 'tests'
+Description-Content-Type: text/markdown
 
 # humanize
 
 [![PyPI version](https://img.shields.io/pypi/v/humanize.svg?logo=pypi&logoColor=FFE873)](https://pypi.org/project/humanize/)
 [![Supported Python versions](https://img.shields.io/pypi/pyversions/humanize.svg?logo=python&logoColor=FFE873)](https://pypi.org/project/humanize/)
 [![Documentation Status](https://readthedocs.org/projects/python-humanize/badge/?version=latest)](https://python-humanize.readthedocs.io/en/latest/?badge=latest)
 [![PyPI downloads](https://img.shields.io/pypi/dm/humanize.svg)](https://pypistats.org/packages/humanize)
@@ -257,15 +261,15 @@
 ```
 
 <!-- usage-end -->
 
 How to add new phrases to existing locale files:
 
 ```sh
-xgettext --from-code=UTF-8 -o humanize.pot -k'_' -k'N_' -k'P_:1c,2' -l python src/humanize/*.py  # extract new phrases
+xgettext --from-code=UTF-8 -o humanize.pot -k'_' -k'N_' -k'P_:1c,2' -k'NS_:1,2' -k'_ngettext:1,2' -l python src/humanize/*.py  # extract new phrases
 msgmerge -U src/humanize/locale/ru_RU/LC_MESSAGES/humanize.po humanize.pot # add them to locale files
 ```
 
 How to add a new locale:
 
 ```sh
 msginit -i humanize.pot -o humanize/locale/<locale name>/LC_MESSAGES/humanize.po --locale <locale name>
```

### Comparing `humanize-4.5.0/README.md` & `humanize-4.6.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -222,15 +222,15 @@
 ```
 
 <!-- usage-end -->
 
 How to add new phrases to existing locale files:
 
 ```sh
-xgettext --from-code=UTF-8 -o humanize.pot -k'_' -k'N_' -k'P_:1c,2' -l python src/humanize/*.py  # extract new phrases
+xgettext --from-code=UTF-8 -o humanize.pot -k'_' -k'N_' -k'P_:1c,2' -k'NS_:1,2' -k'_ngettext:1,2' -l python src/humanize/*.py  # extract new phrases
 msgmerge -U src/humanize/locale/ru_RU/LC_MESSAGES/humanize.po humanize.pot # add them to locale files
 ```
 
 How to add a new locale:
 
 ```sh
 msginit -i humanize.pot -o humanize/locale/<locale name>/LC_MESSAGES/humanize.po --locale <locale name>
```

### Comparing `humanize-4.5.0/RELEASING.md` & `humanize-4.6.0/RELEASING.md`

 * *Files identical despite different names*

### Comparing `humanize-4.5.0/mkdocs.yml` & `humanize-4.6.0/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `humanize-4.5.0/pyproject.toml` & `humanize-4.6.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [build-system]
-build-backend = "setuptools.build_meta"
+build-backend = "hatchling.build"
 requires = [
-  "setuptools>=61.2",
-  "setuptools_scm[toml]>=6.2",
+  "hatch-vcs",
+  "hatchling",
 ]
 
 [project]
 name = "humanize"
 description = "Python humanize utilities"
 readme = "README.md"
 keywords = [
@@ -58,22 +58,23 @@
 
 [tool.black]
 target_version = ["py37"]
 
 [tool.hatch]
 version.source = "vcs"
 
+[tool.hatch.build]
+artifacts = [
+  "*.mo",
+]
+
+[tool.hatch.version.raw-options]
+local_scheme = "no-local-version"
+
 [tool.isort]
 profile = "black"
 
 [tool.pydocstyle]
 convention = "google"
 
 [tool.pytest.ini_options]
 addopts = "--color=yes"
-
-[tool.setuptools.packages.find]
-where = ["src"]
-namespaces = false
-
-[tool.setuptools_scm]
-local_scheme = "no-local-version"
```

### Comparing `humanize-4.5.0/src/humanize/__init__.py` & `humanize-4.6.0/src/humanize/__init__.py`

 * *Files identical despite different names*

### Comparing `humanize-4.5.0/src/humanize/filesize.py` & `humanize-4.6.0/src/humanize/filesize.py`

 * *Files identical despite different names*

### Comparing `humanize-4.5.0/src/humanize/i18n.py` & `humanize-4.6.0/src/humanize/i18n.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,20 +13,22 @@
 _CURRENT = local()
 
 
 # Mapping of locale to thousands separator
 _THOUSANDS_SEPARATOR = {
     "de_DE": ".",
     "fr_FR": " ",
+    "it_IT": ".",
     "pt_BR": ".",
 }
 
 # Mapping of locale to decimal separator
 _DECIMAL_SEPARATOR = {
     "de_DE": ",",
+    "it_IT": ",",
     "pt_BR": ",",
 }
 
 
 def _get_default_locale_path() -> str | None:
     try:
         if __file__ is None:
```

### Comparing `humanize-4.5.0/src/humanize/locale/ar/LC_MESSAGES/humanize.mo` & `humanize-4.6.0/src/humanize/locale/ar/LC_MESSAGES/humanize.mo`

 * *Files identical despite different names*

### Comparing `humanize-4.5.0/src/humanize/locale/ar/LC_MESSAGES/humanize.po` & `humanize-4.6.0/src/humanize/locale/ar/LC_MESSAGES/humanize.po`

 * *Files 7% similar despite different names*

```diff
@@ -3,355 +3,361 @@
 # This file is distributed under the same license as the humanize package.
 # AYMEN Mohammed <let.me.code.safe@gmail.com>, 2022.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: humanize\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-04-13 17:27+0300\n"
+"POT-Creation-Date: 2023-01-08 19:22+0200\n"
 "PO-Revision-Date: 2022-04-13 17:28+0300\n"
 "Last-Translator: AYMEN Mohammed <let.me.code.safe@gmail.com>\n"
 "Language-Team: Arabic <let.me.code.safe@gmail.com>\n"
 "Language: Arabic (عربي)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
-#: src/humanize/number.py:58
+#: src/humanize/number.py:84
 msgctxt "0 (male)"
 msgid "th"
 msgstr "صفر"
 
-#: src/humanize/number.py:59
+#: src/humanize/number.py:85
 msgctxt "1 (male)"
 msgid "st"
 msgstr "اول"
 
-#: src/humanize/number.py:60
+#: src/humanize/number.py:86
 msgctxt "2 (male)"
 msgid "nd"
 msgstr "ثاني"
 
-#: src/humanize/number.py:61
+#: src/humanize/number.py:87
 msgctxt "3 (male)"
 msgid "rd"
 msgstr "ثالث"
 
-#: src/humanize/number.py:62
+#: src/humanize/number.py:88
 msgctxt "4 (male)"
 msgid "th"
 msgstr "رابع"
 
-#: src/humanize/number.py:63
+#: src/humanize/number.py:89
 msgctxt "5 (male)"
 msgid "th"
 msgstr "خامس"
 
-#: src/humanize/number.py:64
+#: src/humanize/number.py:90
 msgctxt "6 (male)"
 msgid "th"
 msgstr "سادس"
 
-#: src/humanize/number.py:65
+#: src/humanize/number.py:91
 msgctxt "7 (male)"
 msgid "th"
 msgstr "سابع"
 
-#: src/humanize/number.py:66
+#: src/humanize/number.py:92
 msgctxt "8 (male)"
 msgid "th"
 msgstr "ثامن"
 
-#: src/humanize/number.py:67
+#: src/humanize/number.py:93
 msgctxt "9 (male)"
 msgid "th"
 msgstr "تاسع"
 
-#: src/humanize/number.py:71
+#: src/humanize/number.py:97
 msgctxt "0 (female)"
 msgid "th"
 msgstr "صفر"
 
-#: src/humanize/number.py:72
+#: src/humanize/number.py:98
 msgctxt "1 (female)"
 msgid "st"
 msgstr "اول"
 
-#: src/humanize/number.py:73
+#: src/humanize/number.py:99
 msgctxt "2 (female)"
 msgid "nd"
 msgstr "ثاني"
 
-#: src/humanize/number.py:74
+#: src/humanize/number.py:100
 msgctxt "3 (female)"
 msgid "rd"
 msgstr "ثالث"
 
-#: src/humanize/number.py:75
+#: src/humanize/number.py:101
 msgctxt "4 (female)"
 msgid "th"
 msgstr "رابع"
 
-#: src/humanize/number.py:76
+#: src/humanize/number.py:102
 msgctxt "5 (female)"
 msgid "th"
 msgstr "خامس"
 
-#: src/humanize/number.py:77
+#: src/humanize/number.py:103
 msgctxt "6 (female)"
 msgid "th"
 msgstr "سادس"
 
-#: src/humanize/number.py:78
+#: src/humanize/number.py:104
 msgctxt "7 (female)"
 msgid "th"
 msgstr "سابع"
 
-#: src/humanize/number.py:79
+#: src/humanize/number.py:105
 msgctxt "8 (female)"
 msgid "th"
 msgstr "ثامن"
 
-#: src/humanize/number.py:80
+#: src/humanize/number.py:106
 msgctxt "9 (female)"
 msgid "th"
 msgstr "تاسع"
 
-#: src/humanize/number.py:140
+#: src/humanize/number.py:178
 msgid "thousand"
 msgid_plural "thousand"
 msgstr[0] "الف"
 msgstr[1] "الاف"
 
-#: src/humanize/number.py:141
+#: src/humanize/number.py:179
 msgid "million"
 msgid_plural "million"
 msgstr[0] "مليون"
 msgstr[1] "ملايين"
 
-#: src/humanize/number.py:142
+#: src/humanize/number.py:180
 msgid "billion"
 msgid_plural "billion"
 msgstr[0] "مليار"
 msgstr[1] "مليارات"
 
-#: src/humanize/number.py:143
+#: src/humanize/number.py:181
 msgid "trillion"
 msgid_plural "trillion"
 msgstr[0] "تريليون"
 msgstr[1] "تريليونات"
 
-#: src/humanize/number.py:144
+#: src/humanize/number.py:182
 msgid "quadrillion"
 msgid_plural "quadrillion"
 msgstr[0] "كوادريليون"
 msgstr[1] "كوادريليون"
 
-#: src/humanize/number.py:145
+#: src/humanize/number.py:183
 msgid "quintillion"
 msgid_plural "quintillion"
 msgstr[0] "كوينتيليون"
 msgstr[1] "كوينتيليون"
 
-#: src/humanize/number.py:146
+#: src/humanize/number.py:184
 msgid "sextillion"
 msgid_plural "sextillion"
 msgstr[0] "سكستليون"
 msgstr[1] "سكستليون"
 
-#: src/humanize/number.py:147
+#: src/humanize/number.py:185
 msgid "septillion"
 msgid_plural "septillion"
 msgstr[0] "سبتيليون"
 msgstr[1] "سبتيليون"
 
-#: src/humanize/number.py:148
+#: src/humanize/number.py:186
 msgid "octillion"
 msgid_plural "octillion"
 msgstr[0] "اوكتيليون"
 msgstr[1] "اوكتيليون"
 
-#: src/humanize/number.py:149
+#: src/humanize/number.py:187
 msgid "nonillion"
 msgid_plural "nonillion"
 msgstr[0] "نونليون"
 msgstr[1] "نونليون"
 
-#: src/humanize/number.py:150
+#: src/humanize/number.py:188
 msgid "decillion"
 msgid_plural "decillion"
 msgstr[0] "ديليون"
 msgstr[1] "ديليون"
 
-#: src/humanize/number.py:247
+#: src/humanize/number.py:189
+msgid "googol"
+msgid_plural "googol"
+msgstr[0] ""
+msgstr[1] ""
+
+#: src/humanize/number.py:301
 msgid "zero"
 msgstr "صفر"
 
-#: src/humanize/number.py:248
+#: src/humanize/number.py:302
 msgid "one"
 msgstr "واحد"
 
-#: src/humanize/number.py:249
+#: src/humanize/number.py:303
 msgid "two"
 msgstr "اثنين"
 
-#: src/humanize/number.py:250
+#: src/humanize/number.py:304
 msgid "three"
 msgstr "ثلاثه"
 
-#: src/humanize/number.py:251
+#: src/humanize/number.py:305
 msgid "four"
 msgstr "اربعه"
 
-#: src/humanize/number.py:252
+#: src/humanize/number.py:306
 msgid "five"
 msgstr "خمسه"
 
-#: src/humanize/number.py:253
+#: src/humanize/number.py:307
 msgid "six"
 msgstr "سته"
 
-#: src/humanize/number.py:254
+#: src/humanize/number.py:308
 msgid "seven"
 msgstr "سبعه"
 
-#: src/humanize/number.py:255
+#: src/humanize/number.py:309
 msgid "eight"
 msgstr "ثمانيه"
 
-#: src/humanize/number.py:256
+#: src/humanize/number.py:310
 msgid "nine"
 msgstr "تسعه"
 
-#: src/humanize/time.py:133
+#: src/humanize/time.py:152
 #, python-format
 msgid "%d microsecond"
 msgid_plural "%d microseconds"
 msgstr[0] "%d ميكرو من الثانية"
 msgstr[1] "%d ميكرو من الثانية"
 
-#: src/humanize/time.py:142
+#: src/humanize/time.py:161
 #, python-format
 msgid "%d millisecond"
 msgid_plural "%d milliseconds"
 msgstr[0] "%d جزء من الثانية"
 msgstr[1] "%d اجزاء من الثانية"
 
-#: src/humanize/time.py:145 src/humanize/time.py:220
+#: src/humanize/time.py:164 src/humanize/time.py:259
 msgid "a moment"
 msgstr "لحظة"
 
-#: src/humanize/time.py:147
+#: src/humanize/time.py:167
 msgid "a second"
 msgstr "ثانية"
 
-#: src/humanize/time.py:149
+#: src/humanize/time.py:170
 #, python-format
 msgid "%d second"
 msgid_plural "%d seconds"
 msgstr[0] "%d ثانية"
 msgstr[1] "%d ثواني"
 
-#: src/humanize/time.py:151
+#: src/humanize/time.py:173
 msgid "a minute"
 msgstr "دقيقة"
 
-#: src/humanize/time.py:154
+#: src/humanize/time.py:177
 #, python-format
 msgid "%d minute"
 msgid_plural "%d minutes"
 msgstr[0] "%d دقيقة"
 msgstr[1] "%d دقائق"
 
-#: src/humanize/time.py:156
+#: src/humanize/time.py:180
 msgid "an hour"
 msgstr "ساعة"
 
-#: src/humanize/time.py:159
+#: src/humanize/time.py:184
 #, python-format
 msgid "%d hour"
 msgid_plural "%d hours"
 msgstr[0] "%d ساعة"
 msgstr[1] "%d ساعات"
 
-#: src/humanize/time.py:162
+#: src/humanize/time.py:188
 msgid "a day"
 msgstr "يوم"
 
-#: src/humanize/time.py:164 src/humanize/time.py:167
+#: src/humanize/time.py:191 src/humanize/time.py:194
 #, python-format
 msgid "%d day"
 msgid_plural "%d days"
 msgstr[0] "%d يوم"
 msgstr[1] "%d أيام"
 
-#: src/humanize/time.py:169
+#: src/humanize/time.py:197
 msgid "a month"
 msgstr "شهر"
 
-#: src/humanize/time.py:171
+#: src/humanize/time.py:199
 #, python-format
 msgid "%d month"
 msgid_plural "%d months"
 msgstr[0] "%d شهر"
 msgstr[1] "%d أشهر"
 
-#: src/humanize/time.py:174
+#: src/humanize/time.py:203
 msgid "a year"
 msgstr "سنة"
 
-#: src/humanize/time.py:176 src/humanize/time.py:185
+#: src/humanize/time.py:206 src/humanize/time.py:217
 #, python-format
 msgid "1 year, %d day"
 msgid_plural "1 year, %d days"
 msgstr[0] "1 سنة ، %d يوم"
 msgstr[1] "1 سنة ، %d ايام"
 
-#: src/humanize/time.py:179
+#: src/humanize/time.py:210
 msgid "1 year, 1 month"
 msgstr "سنة وشهر"
 
-#: src/humanize/time.py:182
+#: src/humanize/time.py:213
 #, python-format
 msgid "1 year, %d month"
 msgid_plural "1 year, %d months"
 msgstr[0] "1 سنة ، %d شهر"
 msgstr[1] "1 سنة ، %d اشهر"
 
-#: src/humanize/time.py:187
+#: src/humanize/time.py:219
 #, python-format
 msgid "%d year"
 msgid_plural "%d years"
 msgstr[0] "%d سنة"
 msgstr[1] "%d سنين"
 
-#: src/humanize/time.py:217
+#: src/humanize/time.py:256
 #, python-format
 msgid "%s from now"
 msgstr "%s من الان"
 
-#: src/humanize/time.py:217
+#: src/humanize/time.py:256
 #, python-format
 msgid "%s ago"
 msgstr "قبل %s"
 
-#: src/humanize/time.py:221
+#: src/humanize/time.py:260
 msgid "now"
 msgstr "الان"
 
-#: src/humanize/time.py:244
+#: src/humanize/time.py:284
 msgid "today"
 msgstr "اليوم"
 
-#: src/humanize/time.py:246
+#: src/humanize/time.py:287
 msgid "tomorrow"
 msgstr "بكرة"
 
-#: src/humanize/time.py:248
+#: src/humanize/time.py:290
 msgid "yesterday"
 msgstr "أمس"
 
-#: src/humanize/time.py:534
+#: src/humanize/time.py:600
 #, python-format
 msgid "%s and %s"
 msgstr "%s و %s"
```

### Comparing `humanize-4.5.0/src/humanize/locale/bn_BD/LC_MESSAGES/humanize.mo` & `humanize-4.6.0/src/humanize/locale/bn_BD/LC_MESSAGES/humanize.mo`

 * *Files identical despite different names*

### Comparing `humanize-4.5.0/src/humanize/locale/bn_BD/LC_MESSAGES/humanize.po` & `humanize-4.6.0/src/humanize/locale/bn_BD/LC_MESSAGES/humanize.po`

 * *Files 17% similar despite different names*

```diff
@@ -3,289 +3,363 @@
 # This file is distributed under the same license as the humanize package.
 # Wasi Master <arianmollik323@gmail.com>, 2021.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: humanize\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2021-07-29 21:59+0600\n"
+"POT-Creation-Date: 2023-01-08 19:22+0200\n"
 "PO-Revision-Date: 2021-07-29 22:07+0600\n"
 "Last-Translator: U-WASI-PC\\Wasi Master <arianmollik323@gmail.com>\n"
 "Language-Team: Bengali\n"
 "Language: bn_BD\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
-#: src/humanize/number.py:58
+#: src/humanize/number.py:84
 msgctxt "0 (male)"
 msgid "th"
 msgstr ""
 
-#: src/humanize/number.py:59
+#: src/humanize/number.py:85
 msgctxt "1 (male)"
 msgid "st"
 msgstr ""
 
-#: src/humanize/number.py:60
+#: src/humanize/number.py:86
 msgctxt "2 (male)"
 msgid "nd"
 msgstr ""
 
-#: src/humanize/number.py:61
+#: src/humanize/number.py:87
 msgctxt "3 (male)"
 msgid "rd"
 msgstr ""
 
-#: src/humanize/number.py:62
+#: src/humanize/number.py:88
 msgctxt "4 (male)"
 msgid "th"
 msgstr ""
 
-#: src/humanize/number.py:63
+#: src/humanize/number.py:89
 msgctxt "5 (male)"
 msgid "th"
 msgstr ""
 
-#: src/humanize/number.py:64
+#: src/humanize/number.py:90
 msgctxt "6 (male)"
 msgid "th"
 msgstr ""
 
-#: src/humanize/number.py:65
+#: src/humanize/number.py:91
 msgctxt "7 (male)"
 msgid "th"
 msgstr ""
 
-#: src/humanize/number.py:66
+#: src/humanize/number.py:92
 msgctxt "8 (male)"
 msgid "th"
 msgstr ""
 
-#: src/humanize/number.py:67
+#: src/humanize/number.py:93
 msgctxt "9 (male)"
 msgid "th"
 msgstr ""
 
-#: src/humanize/number.py:71
+#: src/humanize/number.py:97
 msgctxt "0 (female)"
 msgid "th"
 msgstr ""
 
-#: src/humanize/number.py:72
+#: src/humanize/number.py:98
 msgctxt "1 (female)"
 msgid "st"
 msgstr ""
 
-#: src/humanize/number.py:73
+#: src/humanize/number.py:99
 msgctxt "2 (female)"
 msgid "nd"
 msgstr ""
 
-#: src/humanize/number.py:74
+#: src/humanize/number.py:100
 msgctxt "3 (female)"
 msgid "rd"
 msgstr ""
 
-#: src/humanize/number.py:75
+#: src/humanize/number.py:101
 msgctxt "4 (female)"
 msgid "th"
 msgstr ""
 
-#: src/humanize/number.py:76
+#: src/humanize/number.py:102
 msgctxt "5 (female)"
 msgid "th"
 msgstr ""
 
-#: src/humanize/number.py:77
+#: src/humanize/number.py:103
 msgctxt "6 (female)"
 msgid "th"
 msgstr ""
 
-#: src/humanize/number.py:78
+#: src/humanize/number.py:104
 msgctxt "7 (female)"
 msgid "th"
 msgstr ""
 
-#: src/humanize/number.py:79
+#: src/humanize/number.py:105
 msgctxt "8 (female)"
 msgid "th"
 msgstr ""
 
-#: src/humanize/number.py:80
+#: src/humanize/number.py:106
 msgctxt "9 (female)"
 msgid "th"
 msgstr ""
 
-#: src/humanize/number.py:247
+#: src/humanize/number.py:178
+msgid "thousand"
+msgid_plural "thousand"
+msgstr[0] ""
+msgstr[1] ""
+
+#: src/humanize/number.py:179
+#, fuzzy
+msgid "million"
+msgid_plural "million"
+msgstr[0] "%d মিলিসেকন্ড"
+msgstr[1] "%d মিলিসেকন্ড"
+
+#: src/humanize/number.py:180
+msgid "billion"
+msgid_plural "billion"
+msgstr[0] ""
+msgstr[1] ""
+
+#: src/humanize/number.py:181
+msgid "trillion"
+msgid_plural "trillion"
+msgstr[0] ""
+msgstr[1] ""
+
+#: src/humanize/number.py:182
+msgid "quadrillion"
+msgid_plural "quadrillion"
+msgstr[0] ""
+msgstr[1] ""
+
+#: src/humanize/number.py:183
+msgid "quintillion"
+msgid_plural "quintillion"
+msgstr[0] ""
+msgstr[1] ""
+
+#: src/humanize/number.py:184
+msgid "sextillion"
+msgid_plural "sextillion"
+msgstr[0] ""
+msgstr[1] ""
+
+#: src/humanize/number.py:185
+msgid "septillion"
+msgid_plural "septillion"
+msgstr[0] ""
+msgstr[1] ""
+
+#: src/humanize/number.py:186
+msgid "octillion"
+msgid_plural "octillion"
+msgstr[0] ""
+msgstr[1] ""
+
+#: src/humanize/number.py:187
+msgid "nonillion"
+msgid_plural "nonillion"
+msgstr[0] ""
+msgstr[1] ""
+
+#: src/humanize/number.py:188
+#, fuzzy
+msgid "decillion"
+msgid_plural "decillion"
+msgstr[0] "%d মিলিসেকন্ড"
+msgstr[1] "%d মিলিসেকন্ড"
+
+#: src/humanize/number.py:189
+msgid "googol"
+msgid_plural "googol"
+msgstr[0] ""
+msgstr[1] ""
+
+#: src/humanize/number.py:301
 msgid "zero"
 msgstr "শুন্য"
 
-#: src/humanize/number.py:248
+#: src/humanize/number.py:302
 msgid "one"
 msgstr "এক"
 
-#: src/humanize/number.py:249
+#: src/humanize/number.py:303
 msgid "two"
 msgstr "দুই"
 
-#: src/humanize/number.py:250
+#: src/humanize/number.py:304
 msgid "three"
 msgstr "তিন"
 
-#: src/humanize/number.py:251
+#: src/humanize/number.py:305
 msgid "four"
 msgstr "চার"
 
-#: src/humanize/number.py:252
+#: src/humanize/number.py:306
 msgid "five"
 msgstr "পাচ"
 
-#: src/humanize/number.py:253
+#: src/humanize/number.py:307
 msgid "six"
 msgstr "ছয়"
 
-#: src/humanize/number.py:254
+#: src/humanize/number.py:308
 msgid "seven"
 msgstr "সাত"
 
-#: src/humanize/number.py:255
+#: src/humanize/number.py:309
 msgid "eight"
 msgstr "আট"
 
-#: src/humanize/number.py:256
+#: src/humanize/number.py:310
 msgid "nine"
 msgstr "নয়"
 
-#: src/humanize/time.py:138
+#: src/humanize/time.py:152
 #, python-format
 msgid "%d microsecond"
 msgid_plural "%d microseconds"
 msgstr[0] "%d মাইক্রোসেকন্ড"
 msgstr[1] "%d মাইক্রোসেকন্ড"
 
-#: src/humanize/time.py:147
+#: src/humanize/time.py:161
 #, python-format
 msgid "%d millisecond"
 msgid_plural "%d milliseconds"
 msgstr[0] "%d মিলিসেকন্ড"
 msgstr[1] "%d মিলিসেকন্ড"
 
-#: src/humanize/time.py:150 src/humanize/time.py:231
+#: src/humanize/time.py:164 src/humanize/time.py:259
 msgid "a moment"
 msgstr "এক মুহুর্ত"
 
-#: src/humanize/time.py:152
+#: src/humanize/time.py:167
 msgid "a second"
 msgstr "এক সেকন্ড"
 
-#: src/humanize/time.py:154
+#: src/humanize/time.py:170
 #, python-format
 msgid "%d second"
 msgid_plural "%d seconds"
 msgstr[0] "%d সেকন্ড"
 msgstr[1] "%d সেকন্ড"
 
-#: src/humanize/time.py:156
+#: src/humanize/time.py:173
 msgid "a minute"
 msgstr "এক মিনিট"
 
-#: src/humanize/time.py:159
+#: src/humanize/time.py:177
 #, python-format
 msgid "%d minute"
 msgid_plural "%d minutes"
 msgstr[0] "%d মিনিট"
 msgstr[1] "%d মিনিট"
 
-#: src/humanize/time.py:161
+#: src/humanize/time.py:180
 msgid "an hour"
 msgstr "এক ঘন্টা"
 
-#: src/humanize/time.py:164
+#: src/humanize/time.py:184
 #, python-format
 msgid "%d hour"
 msgid_plural "%d hours"
 msgstr[0] "%d ঘন্টা"
 msgstr[1] "%d ঘন্টা"
 
-#: src/humanize/time.py:167
+#: src/humanize/time.py:188
 msgid "a day"
 msgstr "এক দিন"
 
-#: src/humanize/time.py:169 src/humanize/time.py:172
+#: src/humanize/time.py:191 src/humanize/time.py:194
 #, python-format
 msgid "%d day"
 msgid_plural "%d days"
 msgstr[0] "%d দিন"
 msgstr[1] "%d দিন"
 
-#: src/humanize/time.py:174
+#: src/humanize/time.py:197
 msgid "a month"
 msgstr "এক মাস"
 
-#: src/humanize/time.py:176
+#: src/humanize/time.py:199
 #, python-format
 msgid "%d month"
 msgid_plural "%d months"
 msgstr[0] "%d মাস"
 msgstr[1] "%d মাস"
 
-#: src/humanize/time.py:179
+#: src/humanize/time.py:203
 msgid "a year"
 msgstr "এক বছর"
 
-#: src/humanize/time.py:181 src/humanize/time.py:190
+#: src/humanize/time.py:206 src/humanize/time.py:217
 #, python-format
 msgid "1 year, %d day"
 msgid_plural "1 year, %d days"
 msgstr[0] "%d বছর"
 msgstr[1] "%d বছর"
 
-#: src/humanize/time.py:184
+#: src/humanize/time.py:210
 msgid "1 year, 1 month"
 msgstr "১ বছর, ১ মাস"
 
-#: src/humanize/time.py:187
+#: src/humanize/time.py:213
 #, python-format
 msgid "1 year, %d month"
 msgid_plural "1 year, %d months"
 msgstr[0] "১ বছর, %d মাস"
 msgstr[1] "১ বছর, %d মাস"
 
-#: src/humanize/time.py:192
+#: src/humanize/time.py:219
 #, python-format
 msgid "%d year"
 msgid_plural "%d years"
 msgstr[0] "%d বছর"
 msgstr[1] "%d বছর"
 
-#: src/humanize/time.py:228
+#: src/humanize/time.py:256
 #, python-format
 msgid "%s from now"
 msgstr "আজ থেকে %s পরে"
 
-#: src/humanize/time.py:228
+#: src/humanize/time.py:256
 #, python-format
 msgid "%s ago"
 msgstr "%s আগে"
 
-#: src/humanize/time.py:232
+#: src/humanize/time.py:260
 msgid "now"
 msgstr "এখন"
 
-#: src/humanize/time.py:255
+#: src/humanize/time.py:284
 msgid "today"
 msgstr "আজকে"
 
-#: src/humanize/time.py:257
+#: src/humanize/time.py:287
 msgid "tomorrow"
 msgstr "আগামীকাল"
 
-#: src/humanize/time.py:259
+#: src/humanize/time.py:290
 msgid "yesterday"
 msgstr "গতকাল"
 
-#: src/humanize/time.py:545
+#: src/humanize/time.py:600
 #, python-format
 msgid "%s and %s"
 msgstr "%s আর  %s"
```

### Comparing `humanize-4.5.0/src/humanize/locale/ca_ES/LC_MESSAGES/humanize.mo` & `humanize-4.6.0/src/humanize/locale/ca_ES/LC_MESSAGES/humanize.mo`

 * *Files identical despite different names*

### Comparing `humanize-4.5.0/src/humanize/locale/ca_ES/LC_MESSAGES/humanize.po` & `humanize-4.6.0/src/humanize/locale/fi_FI/LC_MESSAGES/humanize.po`

 * *Files 7% similar despite different names*

```diff
@@ -1,363 +1,364 @@
-# Catalan translations for PACKAGE package
-# This file is distributed under the same license as the PACKAGE package.
-# Jordi Mas i Hernàndez <jmas@softcatala.org>, 2021
+# Finnish translations for humanize package
+# Copyright (C) 2017 THE PACKAGE'S COPYRIGHT HOLDER
+# This file is distributed under the same license as the humanize package.
+# Ville Skyttä <ville.skytta@iki.fi>, 2017.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: humanize\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2021-05-04 23:15+0200\n"
-"PO-Revision-Date: 2021-04-09 19:57+0200\n"
-"Last-Translator: Jordi Mas i Hernàndez <jmas@softcatala.org>\n"
-"Language-Team: Catalan\n"
-"Language: ca\n"
+"POT-Creation-Date: 2023-01-08 19:22+0200\n"
+"PO-Revision-Date: 2017-03-02 11:26+0200\n"
+"Last-Translator: Ville Skyttä <ville.skytta@iki.fi>\n"
+"Language-Team: Finnish\n"
+"Language: fi\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=n!=1;\n"
-"X-Generator: Poedit 2.4.1\n"
+"Plural-Forms: nplurals=2; plural=(n != 1);\n"
+"X-Generator: Poedit 1.8.12\n"
 
-#: src/humanize/number.py:57
+#: src/humanize/number.py:84
 msgctxt "0 (male)"
 msgid "th"
-msgstr "º"
+msgstr "."
 
-#: src/humanize/number.py:58
+#: src/humanize/number.py:85
 msgctxt "1 (male)"
 msgid "st"
-msgstr "º"
+msgstr "."
 
-#: src/humanize/number.py:59
+#: src/humanize/number.py:86
 msgctxt "2 (male)"
 msgid "nd"
-msgstr "º"
+msgstr "."
 
-#: src/humanize/number.py:60
+#: src/humanize/number.py:87
 msgctxt "3 (male)"
 msgid "rd"
-msgstr "º"
+msgstr "."
 
-#: src/humanize/number.py:61
+#: src/humanize/number.py:88
 msgctxt "4 (male)"
 msgid "th"
-msgstr "º"
+msgstr "."
 
-#: src/humanize/number.py:62
+#: src/humanize/number.py:89
 msgctxt "5 (male)"
 msgid "th"
-msgstr "º"
+msgstr "."
 
-#: src/humanize/number.py:63
+#: src/humanize/number.py:90
 msgctxt "6 (male)"
 msgid "th"
-msgstr "º"
+msgstr "."
 
-#: src/humanize/number.py:64
+#: src/humanize/number.py:91
 msgctxt "7 (male)"
 msgid "th"
-msgstr "º"
+msgstr "."
 
-#: src/humanize/number.py:65
+#: src/humanize/number.py:92
 msgctxt "8 (male)"
 msgid "th"
-msgstr "º"
+msgstr "."
 
-#: src/humanize/number.py:66
+#: src/humanize/number.py:93
 msgctxt "9 (male)"
 msgid "th"
-msgstr "º"
+msgstr "."
 
-#: src/humanize/number.py:70
+#: src/humanize/number.py:97
 msgctxt "0 (female)"
 msgid "th"
-msgstr "º"
+msgstr "."
 
-#: src/humanize/number.py:71
+#: src/humanize/number.py:98
 msgctxt "1 (female)"
 msgid "st"
-msgstr "º"
+msgstr "."
 
-#: src/humanize/number.py:72
+#: src/humanize/number.py:99
 msgctxt "2 (female)"
 msgid "nd"
-msgstr "º"
+msgstr "."
 
-#: src/humanize/number.py:73
+#: src/humanize/number.py:100
 msgctxt "3 (female)"
 msgid "rd"
-msgstr "º"
+msgstr "."
 
-#: src/humanize/number.py:74
+#: src/humanize/number.py:101
 msgctxt "4 (female)"
 msgid "th"
-msgstr "º"
+msgstr "."
 
-#: src/humanize/number.py:75
+#: src/humanize/number.py:102
 msgctxt "5 (female)"
 msgid "th"
-msgstr "º"
+msgstr "."
 
-#: src/humanize/number.py:76
+#: src/humanize/number.py:103
 msgctxt "6 (female)"
 msgid "th"
-msgstr "º"
+msgstr "."
 
-#: src/humanize/number.py:77
+#: src/humanize/number.py:104
 msgctxt "7 (female)"
 msgid "th"
-msgstr "º"
+msgstr "."
 
-#: src/humanize/number.py:78
+#: src/humanize/number.py:105
 msgctxt "8 (female)"
 msgid "th"
-msgstr "º"
+msgstr "."
 
-#: src/humanize/number.py:79
+#: src/humanize/number.py:106
 msgctxt "9 (female)"
 msgid "th"
-msgstr "º"
+msgstr "."
 
-#: src/humanize/number.py:140
+#: src/humanize/number.py:178
 msgid "thousand"
 msgid_plural "thousand"
-msgstr[0] ""
-msgstr[1] ""
+msgstr[0] "tuhatta"
+msgstr[1] "tuhatta"
 
-#: src/humanize/number.py:141
+#: src/humanize/number.py:179
 msgid "million"
 msgid_plural "million"
-msgstr[0] "milió"
-msgstr[1] "milió"
+msgstr[0] "miljoonaa"
+msgstr[1] "miljoonaa"
 
-#: src/humanize/number.py:142
+#: src/humanize/number.py:180
 msgid "billion"
 msgid_plural "billion"
-msgstr[0] "mil milions"
-msgstr[1] "mil milions"
+msgstr[0] "miljardia"
+msgstr[1] "miljardia"
 
-#: src/humanize/number.py:143
+#: src/humanize/number.py:181
 msgid "trillion"
 msgid_plural "trillion"
-msgstr[0] "bilions"
-msgstr[1] "bilions"
+msgstr[0] "biljoonaa"
+msgstr[1] "biljoonaa"
 
-#: src/humanize/number.py:144
+#: src/humanize/number.py:182
 msgid "quadrillion"
 msgid_plural "quadrillion"
-msgstr[0] "quadrilió"
-msgstr[1] "quadrilió"
+msgstr[0] "kvadriljoonaa"
+msgstr[1] "kvadriljoonaa"
 
-#: src/humanize/number.py:145
+#: src/humanize/number.py:183
 msgid "quintillion"
 msgid_plural "quintillion"
-msgstr[0] "quintillió"
-msgstr[1] "quintillió"
+msgstr[0] "kvintiljoonaa"
+msgstr[1] "kvintiljoonaa"
 
-#: src/humanize/number.py:146
+#: src/humanize/number.py:184
 msgid "sextillion"
 msgid_plural "sextillion"
-msgstr[0] "sextilió"
-msgstr[1] "sextilió"
+msgstr[0] "sekstiljoonaa"
+msgstr[1] "sekstiljoonaa"
 
-#: src/humanize/number.py:147
+#: src/humanize/number.py:185
 msgid "septillion"
 msgid_plural "septillion"
-msgstr[0] "septilió"
-msgstr[1] "septilió"
+msgstr[0] "septiljoonaa"
+msgstr[1] "septiljoonaa"
 
-#: src/humanize/number.py:148
+#: src/humanize/number.py:186
 msgid "octillion"
 msgid_plural "octillion"
-msgstr[0] "octilió"
-msgstr[1] "octilió"
+msgstr[0] "oktiljoonaa"
+msgstr[1] "oktiljoonaa"
 
-#: src/humanize/number.py:149
+#: src/humanize/number.py:187
 msgid "nonillion"
 msgid_plural "nonillion"
-msgstr[0] "nonilió"
-msgstr[1] "nonilió"
+msgstr[0] "noniljoonaa"
+msgstr[1] "noniljoonaa"
 
-#: src/humanize/number.py:150
+#: src/humanize/number.py:188
 msgid "decillion"
 msgid_plural "decillion"
-msgstr[0] "decilió"
-msgstr[1] "decilió"
+msgstr[0] "dekiljoonaa"
+msgstr[1] "dekiljoonaa"
 
-#: src/humanize/number.py:151
+#: src/humanize/number.py:189
 msgid "googol"
 msgid_plural "googol"
 msgstr[0] "googol"
 msgstr[1] "googol"
 
-#: src/humanize/number.py:246
+#: src/humanize/number.py:301
 msgid "zero"
-msgstr "zero"
+msgstr "nolla"
 
-#: src/humanize/number.py:247
+#: src/humanize/number.py:302
 msgid "one"
-msgstr "un"
+msgstr "yksi"
 
-#: src/humanize/number.py:248
+#: src/humanize/number.py:303
 msgid "two"
-msgstr "dos"
+msgstr "kaksi"
 
-#: src/humanize/number.py:249
+#: src/humanize/number.py:304
 msgid "three"
-msgstr "tres"
+msgstr "kolme"
 
-#: src/humanize/number.py:250
+#: src/humanize/number.py:305
 msgid "four"
-msgstr "quatre"
+msgstr "neljä"
 
-#: src/humanize/number.py:251
+#: src/humanize/number.py:306
 msgid "five"
-msgstr "cinc"
+msgstr "viisi"
 
-#: src/humanize/number.py:252
+#: src/humanize/number.py:307
 msgid "six"
-msgstr "sis"
+msgstr "kuusi"
 
-#: src/humanize/number.py:253
+#: src/humanize/number.py:308
 msgid "seven"
-msgstr "set"
+msgstr "seitsemän"
 
-#: src/humanize/number.py:254
+#: src/humanize/number.py:309
 msgid "eight"
-msgstr "vuit"
+msgstr "kahdeksan"
 
-#: src/humanize/number.py:255
+#: src/humanize/number.py:310
 msgid "nine"
-msgstr "nou"
+msgstr "yhdeksän"
 
-#: src/humanize/time.py:133
-#, python-format
+#: src/humanize/time.py:152
+#, fuzzy, python-format
 msgid "%d microsecond"
 msgid_plural "%d microseconds"
-msgstr[0] "%d microsegon"
-msgstr[1] "%d microsegons"
+msgstr[0] "%d mikrosekunti"
+msgstr[1] "%d mikrosekuntia"
 
-#: src/humanize/time.py:142
-#, python-format
+#: src/humanize/time.py:161
+#, fuzzy, python-format
 msgid "%d millisecond"
 msgid_plural "%d milliseconds"
-msgstr[0] "%d mil·lisegons"
-msgstr[1] "%d mil·lisegons"
+msgstr[0] "%d millisekunti"
+msgstr[1] "%d millisekuntia"
 
-#: src/humanize/time.py:145 src/humanize/time.py:220
+#: src/humanize/time.py:164 src/humanize/time.py:259
 msgid "a moment"
-msgstr "un moment"
+msgstr "hetki"
 
-#: src/humanize/time.py:147
+#: src/humanize/time.py:167
 msgid "a second"
-msgstr "un segon"
+msgstr "sekunti"
 
-#: src/humanize/time.py:149
+#: src/humanize/time.py:170
 #, python-format
 msgid "%d second"
 msgid_plural "%d seconds"
-msgstr[0] "%d segon"
-msgstr[1] "%d segons"
+msgstr[0] "%d sekunti"
+msgstr[1] "%d sekuntia"
 
-#: src/humanize/time.py:151
+#: src/humanize/time.py:173
 msgid "a minute"
-msgstr "un minut"
+msgstr "minuutti"
 
-#: src/humanize/time.py:154
+#: src/humanize/time.py:177
 #, python-format
 msgid "%d minute"
 msgid_plural "%d minutes"
-msgstr[0] "%d minut"
-msgstr[1] "%d minuts"
+msgstr[0] "%d minuutti"
+msgstr[1] "%d minuuttia"
 
-#: src/humanize/time.py:156
+#: src/humanize/time.py:180
 msgid "an hour"
-msgstr "una hora"
+msgstr "tunti"
 
-#: src/humanize/time.py:159
+#: src/humanize/time.py:184
 #, python-format
 msgid "%d hour"
 msgid_plural "%d hours"
-msgstr[0] "%d hora"
-msgstr[1] "%d hores"
+msgstr[0] "%d tunti"
+msgstr[1] "%d tuntia"
 
-#: src/humanize/time.py:162
+#: src/humanize/time.py:188
 msgid "a day"
-msgstr "un dia"
+msgstr "päivä"
 
-#: src/humanize/time.py:164 src/humanize/time.py:167
+#: src/humanize/time.py:191 src/humanize/time.py:194
 #, python-format
 msgid "%d day"
 msgid_plural "%d days"
-msgstr[0] "%d dia"
-msgstr[1] "%d dies"
+msgstr[0] "%d päivä"
+msgstr[1] "%d päivää"
 
-#: src/humanize/time.py:169
+#: src/humanize/time.py:197
 msgid "a month"
-msgstr "un mes"
+msgstr "kuukausi"
 
-#: src/humanize/time.py:171
+#: src/humanize/time.py:199
 #, python-format
 msgid "%d month"
 msgid_plural "%d months"
-msgstr[0] "%d mes"
-msgstr[1] "%d mesos"
+msgstr[0] "%d kuukausi"
+msgstr[1] "%d kuukautta"
 
-#: src/humanize/time.py:174
+#: src/humanize/time.py:203
 msgid "a year"
-msgstr "un any"
+msgstr "vuosi"
 
-#: src/humanize/time.py:176 src/humanize/time.py:185
+#: src/humanize/time.py:206 src/humanize/time.py:217
 #, python-format
 msgid "1 year, %d day"
 msgid_plural "1 year, %d days"
-msgstr[0] "1 any, %d dia"
-msgstr[1] "1 any, %d dies"
+msgstr[0] "1 vuosi, %d päivä"
+msgstr[1] "1 vuosi, %d päivää"
 
-#: src/humanize/time.py:179
+#: src/humanize/time.py:210
 msgid "1 year, 1 month"
-msgstr "1 any, 1 mes"
+msgstr "1 vuosi, 1 kuukausi"
 
-#: src/humanize/time.py:182
+#: src/humanize/time.py:213
 #, python-format
 msgid "1 year, %d month"
 msgid_plural "1 year, %d months"
-msgstr[0] "1 any, %d mes"
-msgstr[1] "1 any, %d mesos"
+msgstr[0] "1 vuosi, %d kuukausi"
+msgstr[1] "1 vuosi, %d kuukautta"
 
-#: src/humanize/time.py:187
+#: src/humanize/time.py:219
 #, python-format
 msgid "%d year"
 msgid_plural "%d years"
-msgstr[0] "%d any"
-msgstr[1] "%d anys"
+msgstr[0] "%d vuosi"
+msgstr[1] "%d vuotta"
 
-#: src/humanize/time.py:217
+#: src/humanize/time.py:256
 #, python-format
 msgid "%s from now"
-msgstr "en %s"
+msgstr "%s tästä"
 
-#: src/humanize/time.py:217
+#: src/humanize/time.py:256
 #, python-format
 msgid "%s ago"
-msgstr "fa %s"
+msgstr "%s sitten"
 
-#: src/humanize/time.py:221
+#: src/humanize/time.py:260
 msgid "now"
-msgstr "ara"
+msgstr "nyt"
 
-#: src/humanize/time.py:244
+#: src/humanize/time.py:284
 msgid "today"
-msgstr "avui"
+msgstr "tänään"
 
-#: src/humanize/time.py:246
+#: src/humanize/time.py:287
 msgid "tomorrow"
-msgstr "demà"
+msgstr "huomenna"
 
-#: src/humanize/time.py:248
+#: src/humanize/time.py:290
 msgid "yesterday"
-msgstr "ahir"
+msgstr "eilen"
 
-#: src/humanize/time.py:534
+#: src/humanize/time.py:600
 #, python-format
 msgid "%s and %s"
-msgstr "%s i %s"
+msgstr "%s ja %s"
```

### Comparing `humanize-4.5.0/src/humanize/locale/da_DK/LC_MESSAGES/humanize.mo` & `humanize-4.6.0/src/humanize/locale/da_DK/LC_MESSAGES/humanize.mo`

 * *Files 17% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,11 +1,11 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: humanize\n"
-"Report-Msgid-Bugs-To: https://github.com/python-humanize/humanize/issues\n"
+"Report-Msgid-Bugs-To: \n"
 "PO-Revision-Date: 2021-11-24 22:25+0200\n"
 "Last-Translator: YURII DEREVYCH <gkhelloworld@gmail.com>\n"
 "Language-Team: Da\n"
 "Language: da\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
```

### Comparing `humanize-4.5.0/src/humanize/locale/da_DK/LC_MESSAGES/humanize.po` & `humanize-4.6.0/src/humanize/locale/da_DK/LC_MESSAGES/humanize.po`

 * *Files 5% similar despite different names*

```diff
@@ -2,363 +2,363 @@
 # Copyright (C) 2021
 # This file is distributed under the same license as the humanize project.
 # YURII DEREVYCH <gkhelloworld@gmail.com>, 2021.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: humanize\n"
-"Report-Msgid-Bugs-To: https://github.com/python-humanize/humanize/issues\n"
-"POT-Creation-Date: 2021-07-05 09:49+0200\n"
+"Report-Msgid-Bugs-To: \n"
+"POT-Creation-Date: 2023-01-08 19:22+0200\n"
 "PO-Revision-Date: 2021-11-24 22:25+0200\n"
 "Last-Translator: YURII DEREVYCH <gkhelloworld@gmail.com>\n"
 "Language-Team: Da\n"
 "Language: da\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "X-Generator: Poedit 3.0\n"
 
-#: src/humanize/number.py:58
+#: src/humanize/number.py:84
 msgctxt "0 (male)"
 msgid "th"
 msgstr ":e"
 
-#: src/humanize/number.py:59
+#: src/humanize/number.py:85
 msgctxt "1 (male)"
 msgid "st"
 msgstr ":e"
 
-#: src/humanize/number.py:60
+#: src/humanize/number.py:86
 msgctxt "2 (male)"
 msgid "nd"
 msgstr ":t"
 
-#: src/humanize/number.py:61
+#: src/humanize/number.py:87
 msgctxt "3 (male)"
 msgid "rd"
 msgstr ":e"
 
-#: src/humanize/number.py:62
+#: src/humanize/number.py:88
 msgctxt "4 (male)"
 msgid "th"
 msgstr ":e"
 
-#: src/humanize/number.py:63
+#: src/humanize/number.py:89
 msgctxt "5 (male)"
 msgid "th"
 msgstr ":e"
 
-#: src/humanize/number.py:64
+#: src/humanize/number.py:90
 msgctxt "6 (male)"
 msgid "th"
 msgstr ":e"
 
-#: src/humanize/number.py:65
+#: src/humanize/number.py:91
 msgctxt "7 (male)"
 msgid "th"
 msgstr ":e"
 
-#: src/humanize/number.py:66
+#: src/humanize/number.py:92
 msgctxt "8 (male)"
 msgid "th"
 msgstr ":e"
 
-#: src/humanize/number.py:67
+#: src/humanize/number.py:93
 msgctxt "9 (male)"
 msgid "th"
 msgstr ":e"
 
-#: src/humanize/number.py:71
+#: src/humanize/number.py:97
 msgctxt "0 (female)"
 msgid "th"
 msgstr ":e"
 
-#: src/humanize/number.py:72
+#: src/humanize/number.py:98
 msgctxt "1 (female)"
 msgid "st"
 msgstr ":e"
 
-#: src/humanize/number.py:73
+#: src/humanize/number.py:99
 msgctxt "2 (female)"
 msgid "nd"
 msgstr ":t"
 
-#: src/humanize/number.py:74
+#: src/humanize/number.py:100
 msgctxt "3 (female)"
 msgid "rd"
 msgstr ":e"
 
-#: src/humanize/number.py:75
+#: src/humanize/number.py:101
 msgctxt "4 (female)"
 msgid "th"
 msgstr ":e"
 
-#: src/humanize/number.py:76
+#: src/humanize/number.py:102
 msgctxt "5 (female)"
 msgid "th"
 msgstr ":e"
 
-#: src/humanize/number.py:77
+#: src/humanize/number.py:103
 msgctxt "6 (female)"
 msgid "th"
 msgstr ":e"
 
-#: src/humanize/number.py:78
+#: src/humanize/number.py:104
 msgctxt "7 (female)"
 msgid "th"
 msgstr ":e"
 
-#: src/humanize/number.py:79
+#: src/humanize/number.py:105
 msgctxt "8 (female)"
 msgid "th"
 msgstr ":e"
 
-#: src/humanize/number.py:80
+#: src/humanize/number.py:106
 msgctxt "9 (female)"
 msgid "th"
 msgstr ":e"
 
-#: src/humanize/number.py:141
+#: src/humanize/number.py:178
 msgid "thousand"
 msgid_plural "thousand"
 msgstr[0] "tusind"
 msgstr[1] "thousand"
 
-#: src/humanize/number.py:142
+#: src/humanize/number.py:179
 msgid "million"
 msgid_plural "million"
 msgstr[0] "million"
 msgstr[1] "millioner"
 
-#: src/humanize/number.py:143
+#: src/humanize/number.py:180
 msgid "billion"
 msgid_plural "billion"
 msgstr[0] "billion"
 msgstr[1] "billioner"
 
-#: src/humanize/number.py:144
+#: src/humanize/number.py:181
 msgid "trillion"
 msgid_plural "trillion"
 msgstr[0] "billion"
 msgstr[1] "billioner"
 
-#: src/humanize/number.py:145
+#: src/humanize/number.py:182
 msgid "quadrillion"
 msgid_plural "quadrillion"
 msgstr[0] "quadrillion"
 msgstr[1] "quadrillioner"
 
-#: src/humanize/number.py:146
+#: src/humanize/number.py:183
 msgid "quintillion"
 msgid_plural "quintillion"
 msgstr[0] "quintillion"
 msgstr[1] "quintillioner"
 
-#: src/humanize/number.py:147
+#: src/humanize/number.py:184
 msgid "sextillion"
 msgid_plural "sextillion"
 msgstr[0] "sextillion"
 msgstr[1] "sextillioner"
 
-#: src/humanize/number.py:148
+#: src/humanize/number.py:185
 msgid "septillion"
 msgid_plural "septillion"
 msgstr[0] "septillion"
 msgstr[1] "septillioner"
 
-#: src/humanize/number.py:149
+#: src/humanize/number.py:186
 msgid "octillion"
 msgid_plural "octillion"
 msgstr[0] "octillion"
 msgstr[1] "octillioner"
 
-#: src/humanize/number.py:150
+#: src/humanize/number.py:187
 msgid "nonillion"
 msgid_plural "nonillion"
 msgstr[0] "nonillion"
 msgstr[1] "nonillioner"
 
-#: src/humanize/number.py:151
+#: src/humanize/number.py:188
 msgid "decillion"
 msgid_plural "decillion"
 msgstr[0] "decillion"
 msgstr[1] "decillioner"
 
-#: src/humanize/number.py:152
+#: src/humanize/number.py:189
 msgid "googol"
 msgid_plural "googol"
 msgstr[0] "googol"
 msgstr[1] "googol"
 
-#: src/humanize/number.py:247
+#: src/humanize/number.py:301
 msgid "zero"
 msgstr "nul"
 
-#: src/humanize/number.py:248
+#: src/humanize/number.py:302
 msgid "one"
 msgstr "en"
 
-#: src/humanize/number.py:249
+#: src/humanize/number.py:303
 msgid "two"
 msgstr "to"
 
-#: src/humanize/number.py:250
+#: src/humanize/number.py:304
 msgid "three"
 msgstr "tre"
 
-#: src/humanize/number.py:251
+#: src/humanize/number.py:305
 msgid "four"
 msgstr "fire"
 
-#: src/humanize/number.py:252
+#: src/humanize/number.py:306
 msgid "five"
 msgstr "fem"
 
-#: src/humanize/number.py:253
+#: src/humanize/number.py:307
 msgid "six"
 msgstr "seks"
 
-#: src/humanize/number.py:254
+#: src/humanize/number.py:308
 msgid "seven"
 msgstr "syv"
 
-#: src/humanize/number.py:255
+#: src/humanize/number.py:309
 msgid "eight"
 msgstr "otte"
 
-#: src/humanize/number.py:256
+#: src/humanize/number.py:310
 msgid "nine"
 msgstr "ni"
 
-#: src/humanize/time.py:138
+#: src/humanize/time.py:152
 #, python-format
 msgid "%d microsecond"
 msgid_plural "%d microseconds"
 msgstr[0] "%d mikrosekund"
 msgstr[1] "%d mikrosekunder"
 
-#: src/humanize/time.py:147
+#: src/humanize/time.py:161
 #, python-format
 msgid "%d millisecond"
 msgid_plural "%d milliseconds"
 msgstr[0] "%d millsekund"
 msgstr[1] "%d millsekunder"
 
-#: src/humanize/time.py:150 src/humanize/time.py:231
+#: src/humanize/time.py:164 src/humanize/time.py:259
 msgid "a moment"
 msgstr "et øjeblik"
 
-#: src/humanize/time.py:152
+#: src/humanize/time.py:167
 msgid "a second"
 msgstr "en anden"
 
-#: src/humanize/time.py:154
+#: src/humanize/time.py:170
 #, python-format
 msgid "%d second"
 msgid_plural "%d seconds"
 msgstr[0] "%d sekund"
 msgstr[1] "%d sekunder"
 
-#: src/humanize/time.py:156
+#: src/humanize/time.py:173
 msgid "a minute"
 msgstr "en minut"
 
-#: src/humanize/time.py:159
+#: src/humanize/time.py:177
 #, python-format
 msgid "%d minute"
 msgid_plural "%d minutes"
 msgstr[0] "%d minut"
 msgstr[1] "%d minutter"
 
-#: src/humanize/time.py:161
+#: src/humanize/time.py:180
 msgid "an hour"
 msgstr "en time"
 
-#: src/humanize/time.py:164
+#: src/humanize/time.py:184
 #, python-format
 msgid "%d hour"
 msgid_plural "%d hours"
 msgstr[0] "%d time"
 msgstr[1] "%d timer"
 
-#: src/humanize/time.py:167
+#: src/humanize/time.py:188
 msgid "a day"
 msgstr "en dag"
 
-#: src/humanize/time.py:169 src/humanize/time.py:172
+#: src/humanize/time.py:191 src/humanize/time.py:194
 #, python-format
 msgid "%d day"
 msgid_plural "%d days"
 msgstr[0] "%d dag"
 msgstr[1] "%d dage"
 
-#: src/humanize/time.py:174
+#: src/humanize/time.py:197
 msgid "a month"
 msgstr "en måned"
 
-#: src/humanize/time.py:176
+#: src/humanize/time.py:199
 #, python-format
 msgid "%d month"
 msgid_plural "%d months"
 msgstr[0] "%d måned"
 msgstr[1] "%d måneder"
 
-#: src/humanize/time.py:179
+#: src/humanize/time.py:203
 msgid "a year"
 msgstr "et år"
 
-#: src/humanize/time.py:181 src/humanize/time.py:190
+#: src/humanize/time.py:206 src/humanize/time.py:217
 #, python-format
 msgid "1 year, %d day"
 msgid_plural "1 year, %d days"
 msgstr[0] "1 år, %d dag"
 msgstr[1] "1 år, %d dage"
 
-#: src/humanize/time.py:184
+#: src/humanize/time.py:210
 msgid "1 year, 1 month"
 msgstr "1 år, 1 måned"
 
-#: src/humanize/time.py:187
+#: src/humanize/time.py:213
 #, python-format
 msgid "1 year, %d month"
 msgid_plural "1 year, %d months"
 msgstr[0] "1 år, %d måned"
 msgstr[1] "1 år, %d måneder"
 
-#: src/humanize/time.py:192
+#: src/humanize/time.py:219
 #, python-format
 msgid "%d year"
 msgid_plural "%d years"
 msgstr[0] "%d år"
 msgstr[1] "%d år"
 
-#: src/humanize/time.py:228
+#: src/humanize/time.py:256
 #, python-format
 msgid "%s from now"
 msgstr "%s fra nu"
 
-#: src/humanize/time.py:228
+#: src/humanize/time.py:256
 #, python-format
 msgid "%s ago"
 msgstr "%s siden"
 
-#: src/humanize/time.py:232
+#: src/humanize/time.py:260
 msgid "now"
 msgstr "nu"
 
-#: src/humanize/time.py:255
+#: src/humanize/time.py:284
 msgid "today"
 msgstr "i dag"
 
-#: src/humanize/time.py:257
+#: src/humanize/time.py:287
 msgid "tomorrow"
 msgstr "i morgen"
 
-#: src/humanize/time.py:259
+#: src/humanize/time.py:290
 msgid "yesterday"
 msgstr "i går"
 
-#: src/humanize/time.py:545
+#: src/humanize/time.py:600
 #, python-format
 msgid "%s and %s"
 msgstr "%s og %s"
```

### Comparing `humanize-4.5.0/src/humanize/locale/de_DE/LC_MESSAGES/humanize.mo` & `humanize-4.6.0/src/humanize/locale/de_DE/LC_MESSAGES/humanize.mo`

 * *Files identical despite different names*

### Comparing `humanize-4.5.0/src/humanize/locale/de_DE/LC_MESSAGES/humanize.po` & `humanize-4.6.0/src/humanize/locale/de_DE/LC_MESSAGES/humanize.po`

 * *Files 7% similar despite different names*

```diff
@@ -3,363 +3,363 @@
 # This file is distributed under the same license as the humanize package.
 # Christian Klein <chris@5711.org>, 2016.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: humanize\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2021-05-04 23:15+0200\n"
+"POT-Creation-Date: 2023-01-08 19:22+0200\n"
 "PO-Revision-Date: 2016-12-18 11:50+0100\n"
 "Last-Translator: Christian Klein <chris@5711.org>\n"
 "Language-Team: German\n"
 "Language: de\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "Generated-By: Christian Klein\n"
 "X-Generator: Sublime Text 3\n"
 
-#: src/humanize/number.py:57
+#: src/humanize/number.py:84
 msgctxt "0 (male)"
 msgid "th"
 msgstr "."
 
-#: src/humanize/number.py:58
+#: src/humanize/number.py:85
 msgctxt "1 (male)"
 msgid "st"
 msgstr "."
 
-#: src/humanize/number.py:59
+#: src/humanize/number.py:86
 msgctxt "2 (male)"
 msgid "nd"
 msgstr "."
 
-#: src/humanize/number.py:60
+#: src/humanize/number.py:87
 msgctxt "3 (male)"
 msgid "rd"
 msgstr "."
 
-#: src/humanize/number.py:61
+#: src/humanize/number.py:88
 msgctxt "4 (male)"
 msgid "th"
 msgstr "."
 
-#: src/humanize/number.py:62
+#: src/humanize/number.py:89
 msgctxt "5 (male)"
 msgid "th"
 msgstr "."
 
-#: src/humanize/number.py:63
+#: src/humanize/number.py:90
 msgctxt "6 (male)"
 msgid "th"
 msgstr "."
 
-#: src/humanize/number.py:64
+#: src/humanize/number.py:91
 msgctxt "7 (male)"
 msgid "th"
 msgstr "."
 
-#: src/humanize/number.py:65
+#: src/humanize/number.py:92
 msgctxt "8 (male)"
 msgid "th"
 msgstr "."
 
-#: src/humanize/number.py:66
+#: src/humanize/number.py:93
 msgctxt "9 (male)"
 msgid "th"
 msgstr "."
 
-#: src/humanize/number.py:70
+#: src/humanize/number.py:97
 msgctxt "0 (female)"
 msgid "th"
 msgstr "."
 
-#: src/humanize/number.py:71
+#: src/humanize/number.py:98
 msgctxt "1 (female)"
 msgid "st"
 msgstr "."
 
-#: src/humanize/number.py:72
+#: src/humanize/number.py:99
 msgctxt "2 (female)"
 msgid "nd"
 msgstr "."
 
-#: src/humanize/number.py:73
+#: src/humanize/number.py:100
 msgctxt "3 (female)"
 msgid "rd"
 msgstr "."
 
-#: src/humanize/number.py:74
+#: src/humanize/number.py:101
 msgctxt "4 (female)"
 msgid "th"
 msgstr "."
 
-#: src/humanize/number.py:75
+#: src/humanize/number.py:102
 msgctxt "5 (female)"
 msgid "th"
 msgstr "."
 
-#: src/humanize/number.py:76
+#: src/humanize/number.py:103
 msgctxt "6 (female)"
 msgid "th"
 msgstr "."
 
-#: src/humanize/number.py:77
+#: src/humanize/number.py:104
 msgctxt "7 (female)"
 msgid "th"
 msgstr "."
 
-#: src/humanize/number.py:78
+#: src/humanize/number.py:105
 msgctxt "8 (female)"
 msgid "th"
 msgstr "."
 
-#: src/humanize/number.py:79
+#: src/humanize/number.py:106
 msgctxt "9 (female)"
 msgid "th"
 msgstr "."
 
-#: src/humanize/number.py:140
+#: src/humanize/number.py:178
 msgid "thousand"
 msgid_plural "thousand"
 msgstr[0] "Tausend"
 msgstr[1] "Tausend"
 
-#: src/humanize/number.py:141
+#: src/humanize/number.py:179
 msgid "million"
 msgid_plural "million"
 msgstr[0] "Million"
 msgstr[1] "Millionen"
 
-#: src/humanize/number.py:142
+#: src/humanize/number.py:180
 msgid "billion"
 msgid_plural "billion"
 msgstr[0] "Milliarde"
 msgstr[1] "Milliarden"
 
-#: src/humanize/number.py:143
+#: src/humanize/number.py:181
 msgid "trillion"
 msgid_plural "trillion"
 msgstr[0] "Billion"
 msgstr[1] "Billionen"
 
-#: src/humanize/number.py:144
+#: src/humanize/number.py:182
 msgid "quadrillion"
 msgid_plural "quadrillion"
 msgstr[0] "Billiarde"
 msgstr[1] "Billiarden"
 
-#: src/humanize/number.py:145
+#: src/humanize/number.py:183
 msgid "quintillion"
 msgid_plural "quintillion"
 msgstr[0] "Trillion"
 msgstr[1] "Trillionen"
 
-#: src/humanize/number.py:146
+#: src/humanize/number.py:184
 msgid "sextillion"
 msgid_plural "sextillion"
 msgstr[0] "Trilliarde"
 msgstr[1] "Trilliarden"
 
-#: src/humanize/number.py:147
+#: src/humanize/number.py:185
 msgid "septillion"
 msgid_plural "septillion"
 msgstr[0] "Quadrillion"
 msgstr[1] "Quadrillionen"
 
-#: src/humanize/number.py:148
+#: src/humanize/number.py:186
 msgid "octillion"
 msgid_plural "octillion"
 msgstr[0] "Quadrillarde"
 msgstr[1] "Quadrillarden"
 
-#: src/humanize/number.py:149
+#: src/humanize/number.py:187
 msgid "nonillion"
 msgid_plural "nonillion"
 msgstr[0] "Quintillion"
 msgstr[1] "Quintillionen"
 
-#: src/humanize/number.py:150
+#: src/humanize/number.py:188
 msgid "decillion"
 msgid_plural "decillion"
 msgstr[0] "Quintilliarde"
 msgstr[1] "Quintilliarden"
 
-#: src/humanize/number.py:151
+#: src/humanize/number.py:189
 msgid "googol"
 msgid_plural "googol"
 msgstr[0] "Googol"
 msgstr[1] "Googol"
 
-#: src/humanize/number.py:246
+#: src/humanize/number.py:301
 msgid "zero"
 msgstr "null"
 
-#: src/humanize/number.py:247
+#: src/humanize/number.py:302
 msgid "one"
 msgstr "eins"
 
-#: src/humanize/number.py:248
+#: src/humanize/number.py:303
 msgid "two"
 msgstr "zwei"
 
-#: src/humanize/number.py:249
+#: src/humanize/number.py:304
 msgid "three"
 msgstr "drei"
 
-#: src/humanize/number.py:250
+#: src/humanize/number.py:305
 msgid "four"
 msgstr "vier"
 
-#: src/humanize/number.py:251
+#: src/humanize/number.py:306
 msgid "five"
 msgstr "fünf"
 
-#: src/humanize/number.py:252
+#: src/humanize/number.py:307
 msgid "six"
 msgstr "sechs"
 
-#: src/humanize/number.py:253
+#: src/humanize/number.py:308
 msgid "seven"
 msgstr "sieben"
 
-#: src/humanize/number.py:254
+#: src/humanize/number.py:309
 msgid "eight"
 msgstr "acht"
 
-#: src/humanize/number.py:255
+#: src/humanize/number.py:310
 msgid "nine"
 msgstr "neun"
 
-#: src/humanize/time.py:133
+#: src/humanize/time.py:152
 #, fuzzy, python-format
 msgid "%d microsecond"
 msgid_plural "%d microseconds"
 msgstr[0] "%d Mikrosekunde"
 msgstr[1] "%d Mikrosekunden"
 
-#: src/humanize/time.py:142
+#: src/humanize/time.py:161
 #, fuzzy, python-format
 msgid "%d millisecond"
 msgid_plural "%d milliseconds"
 msgstr[0] "%d Millisekunde"
 msgstr[1] "%d Millisekunden"
 
-#: src/humanize/time.py:145 src/humanize/time.py:220
+#: src/humanize/time.py:164 src/humanize/time.py:259
 msgid "a moment"
 msgstr "ein Moment"
 
-#: src/humanize/time.py:147
+#: src/humanize/time.py:167
 msgid "a second"
 msgstr "eine Sekunde"
 
-#: src/humanize/time.py:149
+#: src/humanize/time.py:170
 #, python-format
 msgid "%d second"
 msgid_plural "%d seconds"
 msgstr[0] "%d Sekunde"
 msgstr[1] "%d Sekunden"
 
-#: src/humanize/time.py:151
+#: src/humanize/time.py:173
 msgid "a minute"
 msgstr "eine Minute"
 
-#: src/humanize/time.py:154
+#: src/humanize/time.py:177
 #, python-format
 msgid "%d minute"
 msgid_plural "%d minutes"
 msgstr[0] "%d Minute"
 msgstr[1] "%d Minuten"
 
-#: src/humanize/time.py:156
+#: src/humanize/time.py:180
 msgid "an hour"
 msgstr "eine Stunde"
 
-#: src/humanize/time.py:159
+#: src/humanize/time.py:184
 #, python-format
 msgid "%d hour"
 msgid_plural "%d hours"
 msgstr[0] "%d Stunde"
 msgstr[1] "%d Stunden"
 
-#: src/humanize/time.py:162
+#: src/humanize/time.py:188
 msgid "a day"
 msgstr "ein Tag"
 
-#: src/humanize/time.py:164 src/humanize/time.py:167
+#: src/humanize/time.py:191 src/humanize/time.py:194
 #, python-format
 msgid "%d day"
 msgid_plural "%d days"
 msgstr[0] "%d Tag"
 msgstr[1] "%d Tage"
 
-#: src/humanize/time.py:169
+#: src/humanize/time.py:197
 msgid "a month"
 msgstr "ein Monat"
 
-#: src/humanize/time.py:171
+#: src/humanize/time.py:199
 #, python-format
 msgid "%d month"
 msgid_plural "%d months"
 msgstr[0] "%d Monat"
 msgstr[1] "%d Monate"
 
-#: src/humanize/time.py:174
+#: src/humanize/time.py:203
 msgid "a year"
 msgstr "ein Jahr"
 
-#: src/humanize/time.py:176 src/humanize/time.py:185
+#: src/humanize/time.py:206 src/humanize/time.py:217
 #, python-format
 msgid "1 year, %d day"
 msgid_plural "1 year, %d days"
 msgstr[0] "ein Jahr und %d Tag"
 msgstr[1] "ein Jahr und %d Tage"
 
-#: src/humanize/time.py:179
+#: src/humanize/time.py:210
 msgid "1 year, 1 month"
 msgstr "ein Monat"
 
-#: src/humanize/time.py:182
+#: src/humanize/time.py:213
 #, python-format
 msgid "1 year, %d month"
 msgid_plural "1 year, %d months"
 msgstr[0] "ein Jahr und %d Monat"
 msgstr[1] "ein Jahr und %d Monate"
 
-#: src/humanize/time.py:187
+#: src/humanize/time.py:219
 #, python-format
 msgid "%d year"
 msgid_plural "%d years"
 msgstr[0] "%d Jahr"
 msgstr[1] "%d Jahre"
 
-#: src/humanize/time.py:217
+#: src/humanize/time.py:256
 #, python-format
 msgid "%s from now"
 msgstr "%s ab jetzt"
 
-#: src/humanize/time.py:217
+#: src/humanize/time.py:256
 #, python-format
 msgid "%s ago"
 msgstr "vor %s"
 
-#: src/humanize/time.py:221
+#: src/humanize/time.py:260
 msgid "now"
 msgstr "jetzt"
 
-#: src/humanize/time.py:244
+#: src/humanize/time.py:284
 msgid "today"
 msgstr "heute"
 
-#: src/humanize/time.py:246
+#: src/humanize/time.py:287
 msgid "tomorrow"
 msgstr "morgen"
 
-#: src/humanize/time.py:248
+#: src/humanize/time.py:290
 msgid "yesterday"
 msgstr "gestern"
 
-#: src/humanize/time.py:534
+#: src/humanize/time.py:600
 #, python-format
 msgid "%s and %s"
 msgstr "%s und %s"
```

### Comparing `humanize-4.5.0/src/humanize/locale/el_GR/LC_MESSAGES/humanize.po` & `humanize-4.6.0/src/humanize/locale/el_GR/LC_MESSAGES/humanize.po`

 * *Files 18% similar despite different names*

```diff
@@ -3,363 +3,443 @@
 # This file is distributed under the same license as the PACKAGE package.
 # Isaak Tsalicoglou <isaak@waseigo.com>, 2022.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: humanize\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-08-05 01:06+0300\n"
+"POT-Creation-Date: 2023-01-08 19:22+0200\n"
 "PO-Revision-Date: 2022-08-05 01:09+0300\n"
 "Last-Translator: Isaak Tsalicoglou <isaak@waseigo.com>\n"
 "Language-Team: Greek <team@lists.gnome.gr>\n"
 "Language: el\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "Generated-By: Isaak Tsalicoglou\n"
 "X-Generator: Mousepad 0.5.9\n"
 
-#: src/humanize/number.py:71
+#: src/humanize/number.py:84
 msgctxt "0 (male)"
-msgid "ος"
-msgstr "."
+msgid "th"
+msgstr ""
 
-#: src/humanize/number.py:72
+#: src/humanize/number.py:85
 msgctxt "1 (male)"
-msgid "ος"
-msgstr "."
+msgid "st"
+msgstr ""
 
-#: src/humanize/number.py:73
+#: src/humanize/number.py:86
 msgctxt "2 (male)"
-msgid "ος"
-msgstr "."
+msgid "nd"
+msgstr ""
 
-#: src/humanize/number.py:74
+#: src/humanize/number.py:87
 msgctxt "3 (male)"
-msgid "ος"
-msgstr "."
+msgid "rd"
+msgstr ""
 
-#: src/humanize/number.py:75
+#: src/humanize/number.py:88
 msgctxt "4 (male)"
-msgid "ος"
-msgstr "."
+msgid "th"
+msgstr ""
 
-#: src/humanize/number.py:76
+#: src/humanize/number.py:89
 msgctxt "5 (male)"
-msgid "ος"
-msgstr "."
+msgid "th"
+msgstr ""
 
-#: src/humanize/number.py:77
+#: src/humanize/number.py:90
 msgctxt "6 (male)"
-msgid "ος"
-msgstr "."
+msgid "th"
+msgstr ""
 
-#: src/humanize/number.py:78
+#: src/humanize/number.py:91
 msgctxt "7 (male)"
-msgid "ος"
-msgstr "."
+msgid "th"
+msgstr ""
 
-#: src/humanize/number.py:79
+#: src/humanize/number.py:92
 msgctxt "8 (male)"
-msgid "ος"
-msgstr "."
+msgid "th"
+msgstr ""
 
-#: src/humanize/number.py:80
+#: src/humanize/number.py:93
 msgctxt "9 (male)"
-msgid "ος"
-msgstr "."
+msgid "th"
+msgstr ""
 
-#: src/humanize/number.py:84
+#: src/humanize/number.py:97
 msgctxt "0 (female)"
-msgid "η"
-msgstr "."
+msgid "th"
+msgstr ""
 
-#: src/humanize/number.py:85
+#: src/humanize/number.py:98
 msgctxt "1 (female)"
-msgid "η"
-msgstr "."
+msgid "st"
+msgstr ""
 
-#: src/humanize/number.py:86
+#: src/humanize/number.py:99
 msgctxt "2 (female)"
-msgid "η"
-msgstr "."
+msgid "nd"
+msgstr ""
 
-#: src/humanize/number.py:87
+#: src/humanize/number.py:100
 msgctxt "3 (female)"
-msgid "η"
-msgstr "."
+msgid "rd"
+msgstr ""
 
-#: src/humanize/number.py:88
+#: src/humanize/number.py:101
 msgctxt "4 (female)"
-msgid "η"
-msgstr "."
+msgid "th"
+msgstr ""
 
-#: src/humanize/number.py:89
+#: src/humanize/number.py:102
 msgctxt "5 (female)"
-msgid "η"
-msgstr "."
+msgid "th"
+msgstr ""
 
-#: src/humanize/number.py:90
+#: src/humanize/number.py:103
 msgctxt "6 (female)"
-msgid "η"
-msgstr "."
+msgid "th"
+msgstr ""
 
-#: src/humanize/number.py:91
+#: src/humanize/number.py:104
 msgctxt "7 (female)"
-msgid "η"
-msgstr "."
+msgid "th"
+msgstr ""
 
-#: src/humanize/number.py:92
+#: src/humanize/number.py:105
 msgctxt "8 (female)"
-msgid "η"
-msgstr "."
+msgid "th"
+msgstr ""
 
-#: src/humanize/number.py:93
+#: src/humanize/number.py:106
 msgctxt "9 (female)"
-msgid "η"
-msgstr "."
+msgid "th"
+msgstr ""
 
-#: src/humanize/number.py:140
+#: src/humanize/number.py:178
 msgid "thousand"
 msgid_plural "thousand"
 msgstr[0] "χιλιάδα"
 msgstr[1] "χιλιάδες"
 
-#: src/humanize/number.py:141
+#: src/humanize/number.py:179
 msgid "million"
 msgid_plural "million"
 msgstr[0] "εκατομμύριο"
 msgstr[1] "εκατομμύρια"
 
-#: src/humanize/number.py:142
+#: src/humanize/number.py:180
 msgid "billion"
 msgid_plural "billion"
 msgstr[0] "δισεκατομμύριο"
 msgstr[1] "δισεκατομμύρια"
 
-#: src/humanize/number.py:143
+#: src/humanize/number.py:181
 msgid "trillion"
 msgid_plural "trillion"
 msgstr[0] "τρισεκατομμύριο"
 msgstr[1] "τρισεκατομμύρια"
 
-#: src/humanize/number.py:144
+#: src/humanize/number.py:182
 msgid "quadrillion"
 msgid_plural "quadrillion"
 msgstr[0] "τετράκις εκατομμύριο"
 msgstr[1] "τετράκις εκατομμύρια"
 
-#: src/humanize/number.py:145
+#: src/humanize/number.py:183
 msgid "quintillion"
 msgid_plural "quintillion"
 msgstr[0] "πεντάκις εκατομμύριο"
 msgstr[1] "πεντάκις εκατομμύρια"
 
-#: src/humanize/number.py:146
+#: src/humanize/number.py:184
 msgid "sextillion"
 msgid_plural "sextillion"
 msgstr[0] "εξάκις εκατομμύριο"
 msgstr[1] "εξάκις εκατομμύρια"
 
-#: src/humanize/number.py:147
+#: src/humanize/number.py:185
 msgid "septillion"
 msgid_plural "septillion"
 msgstr[0] "επτάκις εκατομμύριο"
 msgstr[1] "επτάκις εκατομμύρια"
 
-#: src/humanize/number.py:148
+#: src/humanize/number.py:186
 msgid "octillion"
 msgid_plural "octillion"
 msgstr[0] "οκτάκις εκατομμύριο"
 msgstr[1] "οκτάκις εκατομμύρια"
 
-#: src/humanize/number.py:149
+#: src/humanize/number.py:187
 msgid "nonillion"
 msgid_plural "nonillion"
 msgstr[0] "εννεάκις εκατομμύριο"
 msgstr[1] "εννεάκις εκατομμύρια"
 
-#: src/humanize/number.py:150
+#: src/humanize/number.py:188
 msgid "decillion"
 msgid_plural "decillion"
 msgstr[0] "δεκάκις εκατομμύριο"
 msgstr[1] "δεκάκις εκατομμύρια"
 
-#: src/humanize/number.py:151
+#: src/humanize/number.py:189
 msgid "googol"
 msgid_plural "googol"
 msgstr[0] "δέκα τριακονταδυάκις εκατομμύριο"
 msgstr[1] "δέκα τριακονταδυάκις εκατομμύρια"
 
-#: src/humanize/number.py:246
+#: src/humanize/number.py:301
 msgid "zero"
 msgstr "μηδέν"
 
-#: src/humanize/number.py:275
+#: src/humanize/number.py:302
 msgid "one"
 msgstr "ένα"
 
-#: src/humanize/number.py:276
+#: src/humanize/number.py:303
 msgid "two"
 msgstr "δύο"
 
-#: src/humanize/number.py:277
+#: src/humanize/number.py:304
 msgid "three"
 msgstr "τρία"
 
-#: src/humanize/number.py:278
+#: src/humanize/number.py:305
 msgid "four"
 msgstr "τέσσερα"
 
-#: src/humanize/number.py:279
+#: src/humanize/number.py:306
 msgid "five"
 msgstr "πέντε"
 
-#: src/humanize/number.py:280
+#: src/humanize/number.py:307
 msgid "six"
 msgstr "έξι"
 
-#: src/humanize/number.py:281
+#: src/humanize/number.py:308
 msgid "seven"
 msgstr "επτά"
 
-#: src/humanize/number.py:254
+#: src/humanize/number.py:309
 msgid "eight"
 msgstr "οκτώ"
 
-#: src/humanize/number.py:255
+#: src/humanize/number.py:310
 msgid "nine"
 msgstr "εννέα"
 
-#: src/humanize/time.py:133
+#: src/humanize/time.py:152
 #, fuzzy, python-format
 msgid "%d microsecond"
 msgid_plural "%d microseconds"
 msgstr[0] "%d εκατομμυριοστό του δευτερολέπτου"
 msgstr[1] "%d εκατομμυριοστά του δευτερολέπτου"
 
-#: src/humanize/time.py:142
+#: src/humanize/time.py:161
 #, fuzzy, python-format
 msgid "%d millisecond"
 msgid_plural "%d milliseconds"
 msgstr[0] "%d χιλιοστό του δευτερολέπτου"
 msgstr[1] "%d χιλιοστά του δευτερολέπτου"
 
-#: src/humanize/time.py:145 src/humanize/time.py:220
+#: src/humanize/time.py:164 src/humanize/time.py:259
 msgid "a moment"
 msgstr "μια στιγμή"
 
-#: src/humanize/time.py:147
+#: src/humanize/time.py:167
 msgid "a second"
 msgstr "ένα δευτερόλεπτο"
 
-#: src/humanize/time.py:149
+#: src/humanize/time.py:170
 #, python-format
 msgid "%d second"
 msgid_plural "%d seconds"
 msgstr[0] "%d δευτερόλεπτο"
 msgstr[1] "%d δευτερόλεπτα"
 
-#: src/humanize/time.py:151
+#: src/humanize/time.py:173
 msgid "a minute"
 msgstr "ένα λεπτό"
 
-#: src/humanize/time.py:154
+#: src/humanize/time.py:177
 #, python-format
 msgid "%d minute"
 msgid_plural "%d minutes"
 msgstr[0] "%d λεπτό"
 msgstr[1] "%d λεπτά"
 
-#: src/humanize/time.py:156
+#: src/humanize/time.py:180
 msgid "an hour"
 msgstr "μία ώρα"
 
-#: src/humanize/time.py:159
+#: src/humanize/time.py:184
 #, python-format
 msgid "%d hour"
 msgid_plural "%d hours"
 msgstr[0] "%d ώρα"
 msgstr[1] "%d ώρες"
 
-#: src/humanize/time.py:162
+#: src/humanize/time.py:188
 msgid "a day"
 msgstr "μία ημέρα"
 
-#: src/humanize/time.py:164 src/humanize/time.py:167
+#: src/humanize/time.py:191 src/humanize/time.py:194
 #, python-format
 msgid "%d day"
 msgid_plural "%d days"
 msgstr[0] "%d ημέρα"
 msgstr[1] "%d ημέρες"
 
-#: src/humanize/time.py:169
+#: src/humanize/time.py:197
 msgid "a month"
 msgstr "ένα μήνα"
 
-#: src/humanize/time.py:171
+#: src/humanize/time.py:199
 #, python-format
 msgid "%d month"
 msgid_plural "%d months"
 msgstr[0] "%d μήνα"
 msgstr[1] "%d μήνες"
 
-#: src/humanize/time.py:174
+#: src/humanize/time.py:203
 msgid "a year"
 msgstr "ένα έτος"
 
-#: src/humanize/time.py:176 src/humanize/time.py:185
+#: src/humanize/time.py:206 src/humanize/time.py:217
 #, python-format
 msgid "1 year, %d day"
 msgid_plural "1 year, %d days"
 msgstr[0] "ένα έτος και %d ημέρα"
 msgstr[1] "ένα έτος και %d ημέρες"
 
-#: src/humanize/time.py:179
+#: src/humanize/time.py:210
 msgid "1 year, 1 month"
 msgstr "ένα έτος και ένα μήνα"
 
-#: src/humanize/time.py:182
+#: src/humanize/time.py:213
 #, python-format
 msgid "1 year, %d month"
 msgid_plural "1 year, %d months"
 msgstr[0] "ένα έτος και %d μήνα"
 msgstr[1] "ένα έτος και %d μήνες"
 
-#: src/humanize/time.py:187
+#: src/humanize/time.py:219
 #, python-format
 msgid "%d year"
 msgid_plural "%d years"
 msgstr[0] "%d έτος"
 msgstr[1] "%d έτη"
 
-#: src/humanize/time.py:217
+#: src/humanize/time.py:256
 #, python-format
 msgid "%s from now"
 msgstr "σε %s από τώρα"
 
-#: src/humanize/time.py:242
+#: src/humanize/time.py:256
 #, python-format
 msgid "%s ago"
 msgstr "πριν από %s"
 
-#: src/humanize/time.py:246
+#: src/humanize/time.py:260
 msgid "now"
 msgstr "τώρα"
 
-#: src/humanize/time.py:269
+#: src/humanize/time.py:284
 msgid "today"
 msgstr "σήμερα"
 
-#: src/humanize/time.py:271
+#: src/humanize/time.py:287
 msgid "tomorrow"
 msgstr "αύριο"
 
-#: src/humanize/time.py:273
+#: src/humanize/time.py:290
 msgid "yesterday"
 msgstr "χθες"
 
-#: src/humanize/time.py:581
+#: src/humanize/time.py:600
 #, python-format
 msgid "%s and %s"
 msgstr "%s και %s"
+
+#~ msgctxt "0 (male)"
+#~ msgid "ος"
+#~ msgstr "."
+
+#~ msgctxt "1 (male)"
+#~ msgid "ος"
+#~ msgstr "."
+
+#~ msgctxt "2 (male)"
+#~ msgid "ος"
+#~ msgstr "."
+
+#~ msgctxt "3 (male)"
+#~ msgid "ος"
+#~ msgstr "."
+
+#~ msgctxt "4 (male)"
+#~ msgid "ος"
+#~ msgstr "."
+
+#~ msgctxt "5 (male)"
+#~ msgid "ος"
+#~ msgstr "."
+
+#~ msgctxt "6 (male)"
+#~ msgid "ος"
+#~ msgstr "."
+
+#~ msgctxt "7 (male)"
+#~ msgid "ος"
+#~ msgstr "."
+
+#~ msgctxt "8 (male)"
+#~ msgid "ος"
+#~ msgstr "."
+
+#~ msgctxt "9 (male)"
+#~ msgid "ος"
+#~ msgstr "."
+
+#~ msgctxt "0 (female)"
+#~ msgid "η"
+#~ msgstr "."
+
+#~ msgctxt "1 (female)"
+#~ msgid "η"
+#~ msgstr "."
+
+#~ msgctxt "2 (female)"
+#~ msgid "η"
+#~ msgstr "."
+
+#~ msgctxt "3 (female)"
+#~ msgid "η"
+#~ msgstr "."
+
+#~ msgctxt "4 (female)"
+#~ msgid "η"
+#~ msgstr "."
+
+#~ msgctxt "5 (female)"
+#~ msgid "η"
+#~ msgstr "."
+
+#~ msgctxt "6 (female)"
+#~ msgid "η"
+#~ msgstr "."
+
+#~ msgctxt "7 (female)"
+#~ msgid "η"
+#~ msgstr "."
+
+#~ msgctxt "8 (female)"
+#~ msgid "η"
+#~ msgstr "."
+
+#~ msgctxt "9 (female)"
+#~ msgid "η"
+#~ msgstr "."
```

### Comparing `humanize-4.5.0/src/humanize/locale/es_ES/LC_MESSAGES/humanize.mo` & `humanize-4.6.0/src/humanize/locale/es_ES/LC_MESSAGES/humanize.mo`

 * *Files identical despite different names*

### Comparing `humanize-4.5.0/src/humanize/locale/es_ES/LC_MESSAGES/humanize.po` & `humanize-4.6.0/src/humanize/locale/es_ES/LC_MESSAGES/humanize.po`

 * *Files 5% similar despite different names*

```diff
@@ -3,362 +3,362 @@
 # This file is distributed under the same license as the PACKAGE package.
 # Álvaro Mondéjar <mondejar1994@gmail.com>, 2020.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: \n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2021-05-04 23:15+0200\n"
+"POT-Creation-Date: 2023-01-08 19:22+0200\n"
 "PO-Revision-Date: 2020-03-31 21:08+0200\n"
 "Last-Translator: Álvaro Mondéjar <mondejar1994@gmail.com>\n"
 "Language-Team: \n"
 "Language: es_ES\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "X-Generator: Poedit 2.3\n"
 
-#: src/humanize/number.py:57
+#: src/humanize/number.py:84
 msgctxt "0 (male)"
 msgid "th"
 msgstr "º"
 
-#: src/humanize/number.py:58
+#: src/humanize/number.py:85
 msgctxt "1 (male)"
 msgid "st"
 msgstr "º"
 
-#: src/humanize/number.py:59
+#: src/humanize/number.py:86
 msgctxt "2 (male)"
 msgid "nd"
 msgstr "º"
 
-#: src/humanize/number.py:60
+#: src/humanize/number.py:87
 msgctxt "3 (male)"
 msgid "rd"
 msgstr "º"
 
-#: src/humanize/number.py:61
+#: src/humanize/number.py:88
 msgctxt "4 (male)"
 msgid "th"
 msgstr "º"
 
-#: src/humanize/number.py:62
+#: src/humanize/number.py:89
 msgctxt "5 (male)"
 msgid "th"
 msgstr "º"
 
-#: src/humanize/number.py:63
+#: src/humanize/number.py:90
 msgctxt "6 (male)"
 msgid "th"
 msgstr "º"
 
-#: src/humanize/number.py:64
+#: src/humanize/number.py:91
 msgctxt "7 (male)"
 msgid "th"
 msgstr "º"
 
-#: src/humanize/number.py:65
+#: src/humanize/number.py:92
 msgctxt "8 (male)"
 msgid "th"
 msgstr "º"
 
-#: src/humanize/number.py:66
+#: src/humanize/number.py:93
 msgctxt "9 (male)"
 msgid "th"
 msgstr "º"
 
-#: src/humanize/number.py:70
+#: src/humanize/number.py:97
 msgctxt "0 (female)"
 msgid "th"
 msgstr "ª"
 
-#: src/humanize/number.py:71
+#: src/humanize/number.py:98
 msgctxt "1 (female)"
 msgid "st"
 msgstr "ª"
 
-#: src/humanize/number.py:72
+#: src/humanize/number.py:99
 msgctxt "2 (female)"
 msgid "nd"
 msgstr "ª"
 
-#: src/humanize/number.py:73
+#: src/humanize/number.py:100
 msgctxt "3 (female)"
 msgid "rd"
 msgstr "ª"
 
-#: src/humanize/number.py:74
+#: src/humanize/number.py:101
 msgctxt "4 (female)"
 msgid "th"
 msgstr "ª"
 
-#: src/humanize/number.py:75
+#: src/humanize/number.py:102
 msgctxt "5 (female)"
 msgid "th"
 msgstr "ª"
 
-#: src/humanize/number.py:76
+#: src/humanize/number.py:103
 msgctxt "6 (female)"
 msgid "th"
 msgstr "ª"
 
-#: src/humanize/number.py:77
+#: src/humanize/number.py:104
 msgctxt "7 (female)"
 msgid "th"
 msgstr "ª"
 
-#: src/humanize/number.py:78
+#: src/humanize/number.py:105
 msgctxt "8 (female)"
 msgid "th"
 msgstr "ª"
 
-#: src/humanize/number.py:79
+#: src/humanize/number.py:106
 msgctxt "9 (female)"
 msgid "th"
 msgstr "ª"
 
-#: src/humanize/number.py:140
+#: src/humanize/number.py:178
 msgid "thousand"
 msgid_plural "thousand"
 msgstr[0] "mil"
 msgstr[1] "mil"
 
-#: src/humanize/number.py:141
+#: src/humanize/number.py:179
 msgid "million"
 msgid_plural "million"
 msgstr[0] "millón"
 msgstr[1] "millones"
 
-#: src/humanize/number.py:142
+#: src/humanize/number.py:180
 msgid "billion"
 msgid_plural "billion"
 msgstr[0] "billón"
 msgstr[1] "billones"
 
-#: src/humanize/number.py:143
+#: src/humanize/number.py:181
 msgid "trillion"
 msgid_plural "trillion"
 msgstr[0] "trillón"
 msgstr[1] "trillones"
 
-#: src/humanize/number.py:144
+#: src/humanize/number.py:182
 msgid "quadrillion"
 msgid_plural "quadrillion"
 msgstr[0] "quatrillón"
 msgstr[1] "quatrillones"
 
-#: src/humanize/number.py:145
+#: src/humanize/number.py:183
 msgid "quintillion"
 msgid_plural "quintillion"
 msgstr[0] "quintillón"
 msgstr[1] "quintillones"
 
-#: src/humanize/number.py:146
+#: src/humanize/number.py:184
 msgid "sextillion"
 msgid_plural "sextillion"
 msgstr[0] "sextillón"
 msgstr[1] "sextillones"
 
-#: src/humanize/number.py:147
+#: src/humanize/number.py:185
 msgid "septillion"
 msgid_plural "septillion"
 msgstr[0] "septillón"
 msgstr[1] "septillones"
 
-#: src/humanize/number.py:148
+#: src/humanize/number.py:186
 msgid "octillion"
 msgid_plural "octillion"
 msgstr[0] "octillón"
 msgstr[1] "octillones"
 
-#: src/humanize/number.py:149
+#: src/humanize/number.py:187
 msgid "nonillion"
 msgid_plural "nonillion"
 msgstr[0] "nonillón"
 msgstr[1] "nonillones"
 
-#: src/humanize/number.py:150
+#: src/humanize/number.py:188
 msgid "decillion"
 msgid_plural "decillion"
 msgstr[0] "decillón"
 msgstr[1] "decillones"
 
-#: src/humanize/number.py:151
+#: src/humanize/number.py:189
 msgid "googol"
 msgid_plural "googol"
 msgstr[0] "gúgol"
 msgstr[1] "gúgol"
 
-#: src/humanize/number.py:246
+#: src/humanize/number.py:301
 msgid "zero"
 msgstr "cero"
 
-#: src/humanize/number.py:247
+#: src/humanize/number.py:302
 msgid "one"
 msgstr "uno"
 
-#: src/humanize/number.py:248
+#: src/humanize/number.py:303
 msgid "two"
 msgstr "dos"
 
-#: src/humanize/number.py:249
+#: src/humanize/number.py:304
 msgid "three"
 msgstr "tres"
 
-#: src/humanize/number.py:250
+#: src/humanize/number.py:305
 msgid "four"
 msgstr "cuatro"
 
-#: src/humanize/number.py:251
+#: src/humanize/number.py:306
 msgid "five"
 msgstr "cinco"
 
-#: src/humanize/number.py:252
+#: src/humanize/number.py:307
 msgid "six"
 msgstr "seis"
 
-#: src/humanize/number.py:253
+#: src/humanize/number.py:308
 msgid "seven"
 msgstr "siete"
 
-#: src/humanize/number.py:254
+#: src/humanize/number.py:309
 msgid "eight"
 msgstr "ocho"
 
-#: src/humanize/number.py:255
+#: src/humanize/number.py:310
 msgid "nine"
 msgstr "nueve"
 
-#: src/humanize/time.py:133
+#: src/humanize/time.py:152
 #, python-format
 msgid "%d microsecond"
 msgid_plural "%d microseconds"
 msgstr[0] "%d microsegundo"
 msgstr[1] "%d microsegundos"
 
-#: src/humanize/time.py:142
+#: src/humanize/time.py:161
 #, python-format
 msgid "%d millisecond"
 msgid_plural "%d milliseconds"
 msgstr[0] "%d milisegundo"
 msgstr[1] "%d milisegundos"
 
-#: src/humanize/time.py:145 src/humanize/time.py:220
+#: src/humanize/time.py:164 src/humanize/time.py:259
 msgid "a moment"
 msgstr "un momento"
 
-#: src/humanize/time.py:147
+#: src/humanize/time.py:167
 msgid "a second"
 msgstr "un segundo"
 
-#: src/humanize/time.py:149
+#: src/humanize/time.py:170
 #, python-format
 msgid "%d second"
 msgid_plural "%d seconds"
 msgstr[0] "%d segundo"
 msgstr[1] "%d segundos"
 
-#: src/humanize/time.py:151
+#: src/humanize/time.py:173
 msgid "a minute"
 msgstr "un minuto"
 
-#: src/humanize/time.py:154
+#: src/humanize/time.py:177
 #, python-format
 msgid "%d minute"
 msgid_plural "%d minutes"
 msgstr[0] "%d minuto"
 msgstr[1] "%d minutos"
 
-#: src/humanize/time.py:156
+#: src/humanize/time.py:180
 msgid "an hour"
 msgstr "una hora"
 
-#: src/humanize/time.py:159
+#: src/humanize/time.py:184
 #, python-format
 msgid "%d hour"
 msgid_plural "%d hours"
 msgstr[0] "%d hora"
 msgstr[1] "%d horas"
 
-#: src/humanize/time.py:162
+#: src/humanize/time.py:188
 msgid "a day"
 msgstr "un día"
 
-#: src/humanize/time.py:164 src/humanize/time.py:167
+#: src/humanize/time.py:191 src/humanize/time.py:194
 #, python-format
 msgid "%d day"
 msgid_plural "%d days"
 msgstr[0] "%d día"
 msgstr[1] "%d días"
 
-#: src/humanize/time.py:169
+#: src/humanize/time.py:197
 msgid "a month"
 msgstr "un mes"
 
-#: src/humanize/time.py:171
+#: src/humanize/time.py:199
 #, python-format
 msgid "%d month"
 msgid_plural "%d months"
 msgstr[0] "%d mes"
 msgstr[1] "%d meses"
 
-#: src/humanize/time.py:174
+#: src/humanize/time.py:203
 msgid "a year"
 msgstr "un año"
 
-#: src/humanize/time.py:176 src/humanize/time.py:185
+#: src/humanize/time.py:206 src/humanize/time.py:217
 #, python-format
 msgid "1 year, %d day"
 msgid_plural "1 year, %d days"
 msgstr[0] "1 año y %d día"
 msgstr[1] "1 año y %d días"
 
-#: src/humanize/time.py:179
+#: src/humanize/time.py:210
 msgid "1 year, 1 month"
 msgstr "1 año y 1 mes"
 
-#: src/humanize/time.py:182
+#: src/humanize/time.py:213
 #, python-format
 msgid "1 year, %d month"
 msgid_plural "1 year, %d months"
 msgstr[0] "1 año y %d mes"
 msgstr[1] "1 año y %d meses"
 
-#: src/humanize/time.py:187
+#: src/humanize/time.py:219
 #, python-format
 msgid "%d year"
 msgid_plural "%d years"
 msgstr[0] "%d año"
 msgstr[1] "%d años"
 
-#: src/humanize/time.py:217
+#: src/humanize/time.py:256
 #, python-format
 msgid "%s from now"
 msgstr "en %s"
 
-#: src/humanize/time.py:217
+#: src/humanize/time.py:256
 #, python-format
 msgid "%s ago"
 msgstr "hace %s"
 
-#: src/humanize/time.py:221
+#: src/humanize/time.py:260
 msgid "now"
 msgstr "ahora"
 
-#: src/humanize/time.py:244
+#: src/humanize/time.py:284
 msgid "today"
 msgstr "hoy"
 
-#: src/humanize/time.py:246
+#: src/humanize/time.py:287
 msgid "tomorrow"
 msgstr "mañana"
 
-#: src/humanize/time.py:248
+#: src/humanize/time.py:290
 msgid "yesterday"
 msgstr "ayer"
 
-#: src/humanize/time.py:534
+#: src/humanize/time.py:600
 #, python-format
 msgid "%s and %s"
 msgstr "%s y %s"
```

### Comparing `humanize-4.5.0/src/humanize/locale/eu/LC_MESSAGES/humanize.mo` & `humanize-4.6.0/src/humanize/locale/eu/LC_MESSAGES/humanize.mo`

 * *Files identical despite different names*

### Comparing `humanize-4.5.0/src/humanize/locale/eu/LC_MESSAGES/humanize.po` & `humanize-4.6.0/src/humanize/locale/eu/LC_MESSAGES/humanize.po`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # This file is distributed under the same license as the PACKAGE package.
 # Mikel Olasagasti <mikel@olasagasti.info>, 2023.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: \n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-01-02 20:23+0100\n"
+"POT-Creation-Date: 2023-01-08 19:22+0200\n"
 "PO-Revision-Date: 2023-01-02 20:35+0100\n"
 "Last-Translator: Mikel Olasagasti <mikel@olasagasti.info>\n"
 "Language-Team: Basque <translation-team-eu@googlegroups.com>\n"
 "Language: eu\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=ASCII\n"
 "Content-Transfer-Encoding: 8bit\n"
@@ -226,139 +226,139 @@
 msgid "eight"
 msgstr "zortzi"
 
 #: src/humanize/number.py:310
 msgid "nine"
 msgstr "bederatzi"
 
-#: src/humanize/time.py:151
+#: src/humanize/time.py:152
 #, python-format
 msgid "%d microsecond"
 msgid_plural "%d microseconds"
 msgstr[0] "mikrosegundo %d"
 msgstr[1] "%d mikrosegundo"
 
-#: src/humanize/time.py:160
+#: src/humanize/time.py:161
 #, python-format
 msgid "%d millisecond"
 msgid_plural "%d milliseconds"
 msgstr[0] "milisegundo %d"
 msgstr[1] "%d milisegundo"
 
-#: src/humanize/time.py:163 src/humanize/time.py:258
+#: src/humanize/time.py:164 src/humanize/time.py:259
 msgid "a moment"
 msgstr "une bat"
 
-#: src/humanize/time.py:166
+#: src/humanize/time.py:167
 msgid "a second"
 msgstr "segundo bat"
 
-#: src/humanize/time.py:169
+#: src/humanize/time.py:170
 #, python-format
 msgid "%d second"
 msgid_plural "%d seconds"
 msgstr[0] "segundo %d"
 msgstr[1] "%d segundo"
 
-#: src/humanize/time.py:172
+#: src/humanize/time.py:173
 msgid "a minute"
 msgstr "minutu bat"
 
-#: src/humanize/time.py:176
+#: src/humanize/time.py:177
 #, python-format
 msgid "%d minute"
 msgid_plural "%d minutes"
 msgstr[0] "minutu %d"
 msgstr[1] "%d minutu"
 
-#: src/humanize/time.py:179
+#: src/humanize/time.py:180
 msgid "an hour"
 msgstr "ordu bat"
 
-#: src/humanize/time.py:183
+#: src/humanize/time.py:184
 #, python-format
 msgid "%d hour"
 msgid_plural "%d hours"
 msgstr[0] "ordu %d"
 msgstr[1] "%d ordu"
 
-#: src/humanize/time.py:187
+#: src/humanize/time.py:188
 msgid "a day"
 msgstr "egun bat"
 
-#: src/humanize/time.py:190 src/humanize/time.py:193
+#: src/humanize/time.py:191 src/humanize/time.py:194
 #, python-format
 msgid "%d day"
 msgid_plural "%d days"
 msgstr[0] "egun %d"
 msgstr[1] "%d egun"
 
-#: src/humanize/time.py:196
+#: src/humanize/time.py:197
 msgid "a month"
 msgstr "hilabete bat"
 
-#: src/humanize/time.py:198
+#: src/humanize/time.py:199
 #, python-format
 msgid "%d month"
 msgid_plural "%d months"
 msgstr[0] "hilabete %d"
 msgstr[1] "%d hilabete"
 
-#: src/humanize/time.py:202
+#: src/humanize/time.py:203
 msgid "a year"
 msgstr "urte bat"
 
-#: src/humanize/time.py:205 src/humanize/time.py:216
+#: src/humanize/time.py:206 src/humanize/time.py:217
 #, python-format
 msgid "1 year, %d day"
 msgid_plural "1 year, %d days"
 msgstr[0] "urte 1, egun %d"
 msgstr[1] "urte 1, %d egun"
 
-#: src/humanize/time.py:209
+#: src/humanize/time.py:210
 msgid "1 year, 1 month"
 msgstr "urte 1, hilabete 1"
 
-#: src/humanize/time.py:212
+#: src/humanize/time.py:213
 #, python-format
 msgid "1 year, %d month"
 msgid_plural "1 year, %d months"
 msgstr[0] "urte 1, hilabete %d"
 msgstr[1] "urte 1, %d hilabete"
 
-#: src/humanize/time.py:218
+#: src/humanize/time.py:219
 #, python-format
 msgid "%d year"
 msgid_plural "%d years"
 msgstr[0] "urte %d"
 msgstr[1] "%d urte"
 
-#: src/humanize/time.py:255
+#: src/humanize/time.py:256
 #, python-format
 msgid "%s from now"
 msgstr "hemendik %s-(e)ra"
 
-#: src/humanize/time.py:255
+#: src/humanize/time.py:256
 #, python-format
 msgid "%s ago"
 msgstr "orain dela %s"
 
-#: src/humanize/time.py:259
+#: src/humanize/time.py:260
 msgid "now"
 msgstr "orain"
 
-#: src/humanize/time.py:283
+#: src/humanize/time.py:284
 msgid "today"
 msgstr "gaur"
 
-#: src/humanize/time.py:286
+#: src/humanize/time.py:287
 msgid "tomorrow"
 msgstr "bihar"
 
-#: src/humanize/time.py:289
+#: src/humanize/time.py:290
 msgid "yesterday"
 msgstr "atzo"
 
 #: src/humanize/time.py:600
 #, python-format
 msgid "%s and %s"
 msgstr "%s eta %s"
```

### Comparing `humanize-4.5.0/src/humanize/locale/fa_IR/LC_MESSAGES/humanize.mo` & `humanize-4.6.0/src/humanize/locale/fa_IR/LC_MESSAGES/humanize.mo`

 * *Files identical despite different names*

### Comparing `humanize-4.5.0/src/humanize/locale/fa_IR/LC_MESSAGES/humanize.po` & `humanize-4.6.0/src/humanize/locale/fa_IR/LC_MESSAGES/humanize.po`

 * *Files 5% similar despite different names*

```diff
@@ -3,363 +3,363 @@
 # This file is distributed under the same license as the humanize package.
 # Christian Klein <chris@5711.org>, 2016.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: humanize\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2021-05-04 23:15+0200\n"
+"POT-Creation-Date: 2023-01-08 19:22+0200\n"
 "PO-Revision-Date: 2017-01-10 02:44+0330\n"
 "Last-Translator: Christian Klein <chris@5711.org>\n"
 "Language-Team: German\n"
 "Language: de\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "Generated-By: Christian Klein\n"
 "X-Generator: Poedit 1.5.4\n"
 
-#: src/humanize/number.py:57
+#: src/humanize/number.py:84
 msgctxt "0 (male)"
 msgid "th"
 msgstr "صفرمین"
 
-#: src/humanize/number.py:58
+#: src/humanize/number.py:85
 msgctxt "1 (male)"
 msgid "st"
 msgstr "اولین"
 
-#: src/humanize/number.py:59
+#: src/humanize/number.py:86
 msgctxt "2 (male)"
 msgid "nd"
 msgstr "دومین"
 
-#: src/humanize/number.py:60
+#: src/humanize/number.py:87
 msgctxt "3 (male)"
 msgid "rd"
 msgstr "سومین"
 
-#: src/humanize/number.py:61
+#: src/humanize/number.py:88
 msgctxt "4 (male)"
 msgid "th"
 msgstr "چهارمین"
 
-#: src/humanize/number.py:62
+#: src/humanize/number.py:89
 msgctxt "5 (male)"
 msgid "th"
 msgstr "پنجمین"
 
-#: src/humanize/number.py:63
+#: src/humanize/number.py:90
 msgctxt "6 (male)"
 msgid "th"
 msgstr "ششمین"
 
-#: src/humanize/number.py:64
+#: src/humanize/number.py:91
 msgctxt "7 (male)"
 msgid "th"
 msgstr "هفتمین"
 
-#: src/humanize/number.py:65
+#: src/humanize/number.py:92
 msgctxt "8 (male)"
 msgid "th"
 msgstr "هشتمین"
 
-#: src/humanize/number.py:66
+#: src/humanize/number.py:93
 msgctxt "9 (male)"
 msgid "th"
 msgstr "نهمین"
 
-#: src/humanize/number.py:70
+#: src/humanize/number.py:97
 msgctxt "0 (female)"
 msgid "th"
 msgstr "صفرمین"
 
-#: src/humanize/number.py:71
+#: src/humanize/number.py:98
 msgctxt "1 (female)"
 msgid "st"
 msgstr "اولین"
 
-#: src/humanize/number.py:72
+#: src/humanize/number.py:99
 msgctxt "2 (female)"
 msgid "nd"
 msgstr "دومین"
 
-#: src/humanize/number.py:73
+#: src/humanize/number.py:100
 msgctxt "3 (female)"
 msgid "rd"
 msgstr "سومین"
 
-#: src/humanize/number.py:74
+#: src/humanize/number.py:101
 msgctxt "4 (female)"
 msgid "th"
 msgstr "چهارمین"
 
-#: src/humanize/number.py:75
+#: src/humanize/number.py:102
 msgctxt "5 (female)"
 msgid "th"
 msgstr "پنجمین"
 
-#: src/humanize/number.py:76
+#: src/humanize/number.py:103
 msgctxt "6 (female)"
 msgid "th"
 msgstr "ششمین"
 
-#: src/humanize/number.py:77
+#: src/humanize/number.py:104
 msgctxt "7 (female)"
 msgid "th"
 msgstr "هفتمین"
 
-#: src/humanize/number.py:78
+#: src/humanize/number.py:105
 msgctxt "8 (female)"
 msgid "th"
 msgstr "هشتمین"
 
-#: src/humanize/number.py:79
+#: src/humanize/number.py:106
 msgctxt "9 (female)"
 msgid "th"
 msgstr "نهمین"
 
-#: src/humanize/number.py:140
+#: src/humanize/number.py:178
 msgid "thousand"
 msgid_plural "thousand"
 msgstr[0] "هزار"
 msgstr[1] "هزار"
 
-#: src/humanize/number.py:141
+#: src/humanize/number.py:179
 msgid "million"
 msgid_plural "million"
 msgstr[0] "میلیون"
 msgstr[1] "میلیون"
 
-#: src/humanize/number.py:142
+#: src/humanize/number.py:180
 msgid "billion"
 msgid_plural "billion"
 msgstr[0] "میلیارد"
 msgstr[1] "میلیارد"
 
-#: src/humanize/number.py:143
+#: src/humanize/number.py:181
 msgid "trillion"
 msgid_plural "trillion"
 msgstr[0] "ترلیون"
 msgstr[1] "ترلیون"
 
-#: src/humanize/number.py:144
+#: src/humanize/number.py:182
 msgid "quadrillion"
 msgid_plural "quadrillion"
 msgstr[0] "کوادریلیون"
 msgstr[1] "کوادریلیون"
 
-#: src/humanize/number.py:145
+#: src/humanize/number.py:183
 msgid "quintillion"
 msgid_plural "quintillion"
 msgstr[0] "کوانتیلیون"
 msgstr[1] "کوانتیلیون"
 
-#: src/humanize/number.py:146
+#: src/humanize/number.py:184
 msgid "sextillion"
 msgid_plural "sextillion"
 msgstr[0] "سکستیلیون"
 msgstr[1] "سکستیلیون"
 
-#: src/humanize/number.py:147
+#: src/humanize/number.py:185
 msgid "septillion"
 msgid_plural "septillion"
 msgstr[0] "سپتیلیون"
 msgstr[1] "سپتیلیون"
 
-#: src/humanize/number.py:148
+#: src/humanize/number.py:186
 msgid "octillion"
 msgid_plural "octillion"
 msgstr[0] "اوکتیلیون"
 msgstr[1] "اوکتیلیون"
 
-#: src/humanize/number.py:149
+#: src/humanize/number.py:187
 msgid "nonillion"
 msgid_plural "nonillion"
 msgstr[0] "نونیلیون"
 msgstr[1] "نونیلیون"
 
-#: src/humanize/number.py:150
+#: src/humanize/number.py:188
 msgid "decillion"
 msgid_plural "decillion"
 msgstr[0] "دسیلیون"
 msgstr[1] "دسیلیون"
 
-#: src/humanize/number.py:151
+#: src/humanize/number.py:189
 msgid "googol"
 msgid_plural "googol"
 msgstr[0] "گوگول"
 msgstr[1] "گوگول"
 
-#: src/humanize/number.py:246
+#: src/humanize/number.py:301
 msgid "zero"
 msgstr "صفر"
 
-#: src/humanize/number.py:247
+#: src/humanize/number.py:302
 msgid "one"
 msgstr "یک"
 
-#: src/humanize/number.py:248
+#: src/humanize/number.py:303
 msgid "two"
 msgstr "دو"
 
-#: src/humanize/number.py:249
+#: src/humanize/number.py:304
 msgid "three"
 msgstr "سه"
 
-#: src/humanize/number.py:250
+#: src/humanize/number.py:305
 msgid "four"
 msgstr "چهار"
 
-#: src/humanize/number.py:251
+#: src/humanize/number.py:306
 msgid "five"
 msgstr "پنج"
 
-#: src/humanize/number.py:252
+#: src/humanize/number.py:307
 msgid "six"
 msgstr "شش"
 
-#: src/humanize/number.py:253
+#: src/humanize/number.py:308
 msgid "seven"
 msgstr "هفت"
 
-#: src/humanize/number.py:254
+#: src/humanize/number.py:309
 msgid "eight"
 msgstr "هشت"
 
-#: src/humanize/number.py:255
+#: src/humanize/number.py:310
 msgid "nine"
 msgstr "نه"
 
-#: src/humanize/time.py:133
+#: src/humanize/time.py:152
 #, python-format
 msgid "%d microsecond"
 msgid_plural "%d microseconds"
 msgstr[0] "%d میکرو‌ثانیه"
 msgstr[1] "%d میکرو‌ثانیه"
 
-#: src/humanize/time.py:142
+#: src/humanize/time.py:161
 #, python-format
 msgid "%d millisecond"
 msgid_plural "%d milliseconds"
 msgstr[0] "%d میلی‌ثانیه"
 msgstr[1] "%d میلی‌ثانیه"
 
-#: src/humanize/time.py:145 src/humanize/time.py:220
+#: src/humanize/time.py:164 src/humanize/time.py:259
 msgid "a moment"
 msgstr "یک لحظه"
 
-#: src/humanize/time.py:147
+#: src/humanize/time.py:167
 msgid "a second"
 msgstr "یک ثانیه"
 
-#: src/humanize/time.py:149
+#: src/humanize/time.py:170
 #, python-format
 msgid "%d second"
 msgid_plural "%d seconds"
 msgstr[0] "%d ثانیه"
 msgstr[1] "%d ثانیه"
 
-#: src/humanize/time.py:151
+#: src/humanize/time.py:173
 msgid "a minute"
 msgstr "یک دقیقه"
 
-#: src/humanize/time.py:154
+#: src/humanize/time.py:177
 #, python-format
 msgid "%d minute"
 msgid_plural "%d minutes"
 msgstr[0] "%d دقیقه"
 msgstr[1] "%d دقیقه"
 
-#: src/humanize/time.py:156
+#: src/humanize/time.py:180
 msgid "an hour"
 msgstr "یک ساعت"
 
-#: src/humanize/time.py:159
+#: src/humanize/time.py:184
 #, python-format
 msgid "%d hour"
 msgid_plural "%d hours"
 msgstr[0] "%d ساعت"
 msgstr[1] "%d ساعت"
 
-#: src/humanize/time.py:162
+#: src/humanize/time.py:188
 msgid "a day"
 msgstr "یک روز"
 
-#: src/humanize/time.py:164 src/humanize/time.py:167
+#: src/humanize/time.py:191 src/humanize/time.py:194
 #, python-format
 msgid "%d day"
 msgid_plural "%d days"
 msgstr[0] "%d روز"
 msgstr[1] "%d روز"
 
-#: src/humanize/time.py:169
+#: src/humanize/time.py:197
 msgid "a month"
 msgstr "یک ماه"
 
-#: src/humanize/time.py:171
+#: src/humanize/time.py:199
 #, python-format
 msgid "%d month"
 msgid_plural "%d months"
 msgstr[0] "%d ماه"
 msgstr[1] "%d ماه"
 
-#: src/humanize/time.py:174
+#: src/humanize/time.py:203
 msgid "a year"
 msgstr "یک سال"
 
-#: src/humanize/time.py:176 src/humanize/time.py:185
+#: src/humanize/time.py:206 src/humanize/time.py:217
 #, python-format
 msgid "1 year, %d day"
 msgid_plural "1 year, %d days"
 msgstr[0] "۱ سال و %d روز"
 msgstr[1] "۱ سال و %d روز"
 
-#: src/humanize/time.py:179
+#: src/humanize/time.py:210
 msgid "1 year, 1 month"
 msgstr "۱ سال و ۱ ماه"
 
-#: src/humanize/time.py:182
+#: src/humanize/time.py:213
 #, python-format
 msgid "1 year, %d month"
 msgid_plural "1 year, %d months"
 msgstr[0] "۱ سال و %d ماه"
 msgstr[1] "۱ سال و %d ماه"
 
-#: src/humanize/time.py:187
+#: src/humanize/time.py:219
 #, python-format
 msgid "%d year"
 msgid_plural "%d years"
 msgstr[0] "%d سال"
 msgstr[1] "%d سال"
 
-#: src/humanize/time.py:217
+#: src/humanize/time.py:256
 #, python-format
 msgid "%s from now"
 msgstr "%s تا به اکنون"
 
-#: src/humanize/time.py:217
+#: src/humanize/time.py:256
 #, python-format
 msgid "%s ago"
 msgstr "%s پیش"
 
-#: src/humanize/time.py:221
+#: src/humanize/time.py:260
 msgid "now"
 msgstr "اکنون"
 
-#: src/humanize/time.py:244
+#: src/humanize/time.py:284
 msgid "today"
 msgstr "امروز"
 
-#: src/humanize/time.py:246
+#: src/humanize/time.py:287
 msgid "tomorrow"
 msgstr "فردا"
 
-#: src/humanize/time.py:248
+#: src/humanize/time.py:290
 msgid "yesterday"
 msgstr "دیروز"
 
-#: src/humanize/time.py:534
+#: src/humanize/time.py:600
 #, python-format
 msgid "%s and %s"
 msgstr "%s و %s"
```

### Comparing `humanize-4.5.0/src/humanize/locale/fi_FI/LC_MESSAGES/humanize.mo` & `humanize-4.6.0/src/humanize/locale/fi_FI/LC_MESSAGES/humanize.mo`

 * *Files identical despite different names*

### Comparing `humanize-4.5.0/src/humanize/locale/fi_FI/LC_MESSAGES/humanize.po` & `humanize-4.6.0/src/humanize/locale/pl_PL/LC_MESSAGES/humanize.po`

 * *Files 11% similar despite different names*

```diff
@@ -1,364 +1,388 @@
-# Finnish translations for humanize package
-# Copyright (C) 2017 THE PACKAGE'S COPYRIGHT HOLDER
-# This file is distributed under the same license as the humanize package.
-# Ville Skyttä <ville.skytta@iki.fi>, 2017.
+# Polish translations for PACKAGE package.
+# Copyright (C) 2020 THE PACKAGE'S COPYRIGHT HOLDER
+# This file is distributed under the same license as the PACKAGE package.
+# Bartosz Bubak <bartosz.bubak@gmail.com>, 2020.
+# Added missing strings by Krystian Postek <krystian postek eu>, 2020.
+# Replace short scale with long scale by Maciej J. Mikulski (mjmikulski), 2022.
 #
 msgid ""
 msgstr ""
-"Project-Id-Version: humanize\n"
+"Project-Id-Version: 0.0.1\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2021-05-04 23:15+0200\n"
-"PO-Revision-Date: 2017-03-02 11:26+0200\n"
-"Last-Translator: Ville Skyttä <ville.skytta@iki.fi>\n"
-"Language-Team: Finnish\n"
-"Language: fi\n"
+"POT-Creation-Date: 2023-01-08 19:22+0200\n"
+"PO-Revision-Date: 2020-04-22 10:02+0200\n"
+"Last-Translator: Bartosz Bubak <bartosz.bubak gmail com>\n"
+"Language-Team: Polish\n"
+"Language: pl\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=(n != 1);\n"
-"X-Generator: Poedit 1.8.12\n"
+"Plural-Forms: nplurals=3; plural=(n==1 ? 0 : n%10>=2 && n%10<=4 && (n%100<10 "
+"|| n%100>=20) ? 1 : 2);\n"
 
-#: src/humanize/number.py:57
+#: src/humanize/number.py:84
 msgctxt "0 (male)"
 msgid "th"
 msgstr "."
 
-#: src/humanize/number.py:58
+#: src/humanize/number.py:85
 msgctxt "1 (male)"
 msgid "st"
 msgstr "."
 
-#: src/humanize/number.py:59
+#: src/humanize/number.py:86
 msgctxt "2 (male)"
 msgid "nd"
 msgstr "."
 
-#: src/humanize/number.py:60
+#: src/humanize/number.py:87
 msgctxt "3 (male)"
 msgid "rd"
 msgstr "."
 
-#: src/humanize/number.py:61
+#: src/humanize/number.py:88
 msgctxt "4 (male)"
 msgid "th"
 msgstr "."
 
-#: src/humanize/number.py:62
+#: src/humanize/number.py:89
 msgctxt "5 (male)"
 msgid "th"
 msgstr "."
 
-#: src/humanize/number.py:63
+#: src/humanize/number.py:90
 msgctxt "6 (male)"
 msgid "th"
 msgstr "."
 
-#: src/humanize/number.py:64
+#: src/humanize/number.py:91
 msgctxt "7 (male)"
 msgid "th"
 msgstr "."
 
-#: src/humanize/number.py:65
+#: src/humanize/number.py:92
 msgctxt "8 (male)"
 msgid "th"
 msgstr "."
 
-#: src/humanize/number.py:66
+#: src/humanize/number.py:93
 msgctxt "9 (male)"
 msgid "th"
 msgstr "."
 
-#: src/humanize/number.py:70
+#: src/humanize/number.py:97
 msgctxt "0 (female)"
 msgid "th"
 msgstr "."
 
-#: src/humanize/number.py:71
+#: src/humanize/number.py:98
 msgctxt "1 (female)"
 msgid "st"
 msgstr "."
 
-#: src/humanize/number.py:72
+#: src/humanize/number.py:99
 msgctxt "2 (female)"
 msgid "nd"
 msgstr "."
 
-#: src/humanize/number.py:73
+#: src/humanize/number.py:100
 msgctxt "3 (female)"
 msgid "rd"
 msgstr "."
 
-#: src/humanize/number.py:74
+#: src/humanize/number.py:101
 msgctxt "4 (female)"
 msgid "th"
 msgstr "."
 
-#: src/humanize/number.py:75
+#: src/humanize/number.py:102
 msgctxt "5 (female)"
 msgid "th"
 msgstr "."
 
-#: src/humanize/number.py:76
+#: src/humanize/number.py:103
 msgctxt "6 (female)"
 msgid "th"
 msgstr "."
 
-#: src/humanize/number.py:77
+#: src/humanize/number.py:104
 msgctxt "7 (female)"
 msgid "th"
 msgstr "."
 
-#: src/humanize/number.py:78
+#: src/humanize/number.py:105
 msgctxt "8 (female)"
 msgid "th"
 msgstr "."
 
-#: src/humanize/number.py:79
+#: src/humanize/number.py:106
 msgctxt "9 (female)"
 msgid "th"
 msgstr "."
 
-#: src/humanize/number.py:140
+#: src/humanize/number.py:178
 msgid "thousand"
 msgid_plural "thousand"
-msgstr[0] "tuhatta"
-msgstr[1] "tuhatta"
+msgstr[0] "tysiąc"
+msgstr[1] "tysiąc"
+msgstr[2] "tysięcy"
 
-#: src/humanize/number.py:141
+#: src/humanize/number.py:179
 msgid "million"
 msgid_plural "million"
-msgstr[0] "miljoonaa"
-msgstr[1] "miljoonaa"
+msgstr[0] "milion"
+msgstr[1] "miliony"
+msgstr[2] "milionów"
 
-#: src/humanize/number.py:142
+#: src/humanize/number.py:180
 msgid "billion"
 msgid_plural "billion"
-msgstr[0] "miljardia"
-msgstr[1] "miljardia"
+msgstr[0] "miliard"
+msgstr[1] "miliardy"
+msgstr[2] "miliardów"
 
-#: src/humanize/number.py:143
+#: src/humanize/number.py:181
 msgid "trillion"
 msgid_plural "trillion"
-msgstr[0] "biljoonaa"
-msgstr[1] "biljoonaa"
+msgstr[0] "bilion"
+msgstr[1] "biliony"
+msgstr[2] "bilionów"
 
-#: src/humanize/number.py:144
+#: src/humanize/number.py:182
 msgid "quadrillion"
 msgid_plural "quadrillion"
-msgstr[0] "kvadriljoonaa"
-msgstr[1] "kvadriljoonaa"
+msgstr[0] "biliard"
+msgstr[1] "biliardy"
+msgstr[2] "biliardów"
 
-#: src/humanize/number.py:145
+#: src/humanize/number.py:183
 msgid "quintillion"
 msgid_plural "quintillion"
-msgstr[0] "kvintiljoonaa"
-msgstr[1] "kvintiljoonaa"
+msgstr[0] "trylion"
+msgstr[1] "tryliony"
+msgstr[2] "trylionów"
 
-#: src/humanize/number.py:146
+#: src/humanize/number.py:184
 msgid "sextillion"
 msgid_plural "sextillion"
-msgstr[0] "sekstiljoonaa"
-msgstr[1] "sekstiljoonaa"
+msgstr[0] "tryliard"
+msgstr[1] "tryliard"
+msgstr[2] "tryliard"
 
-#: src/humanize/number.py:147
+#: src/humanize/number.py:185
 msgid "septillion"
 msgid_plural "septillion"
-msgstr[0] "septiljoonaa"
-msgstr[1] "septiljoonaa"
+msgstr[0] "kwadrylion"
+msgstr[1] "kwadryliony"
+msgstr[2] "kwadrylionów"
 
-#: src/humanize/number.py:148
+#: src/humanize/number.py:186
 msgid "octillion"
 msgid_plural "octillion"
-msgstr[0] "oktiljoonaa"
-msgstr[1] "oktiljoonaa"
+msgstr[0] "kwadryliard"
+msgstr[1] "kwadryliardy"
+msgstr[2] "kwadryliardów"
 
-#: src/humanize/number.py:149
+#: src/humanize/number.py:187
 msgid "nonillion"
 msgid_plural "nonillion"
-msgstr[0] "noniljoonaa"
-msgstr[1] "noniljoonaa"
+msgstr[0] "kwintylion"
+msgstr[1] "kwintyliony"
+msgstr[2] "kwintylionów"
 
-#: src/humanize/number.py:150
+#: src/humanize/number.py:188
 msgid "decillion"
 msgid_plural "decillion"
-msgstr[0] "dekiljoonaa"
-msgstr[1] "dekiljoonaa"
+msgstr[0] "kwintyliard"
+msgstr[1] "kwintyliardy"
+msgstr[2] "kwintyliardów"
 
-#: src/humanize/number.py:151
+#: src/humanize/number.py:189
 msgid "googol"
 msgid_plural "googol"
 msgstr[0] "googol"
-msgstr[1] "googol"
+msgstr[1] "googole"
+msgstr[2] "googoli"
 
-#: src/humanize/number.py:246
+#: src/humanize/number.py:301
 msgid "zero"
-msgstr "nolla"
+msgstr "zero"
 
-#: src/humanize/number.py:247
+#: src/humanize/number.py:302
 msgid "one"
-msgstr "yksi"
+msgstr "jeden"
 
-#: src/humanize/number.py:248
+#: src/humanize/number.py:303
 msgid "two"
-msgstr "kaksi"
+msgstr "dwa"
 
-#: src/humanize/number.py:249
+#: src/humanize/number.py:304
 msgid "three"
-msgstr "kolme"
+msgstr "trzy"
 
-#: src/humanize/number.py:250
+#: src/humanize/number.py:305
 msgid "four"
-msgstr "neljä"
+msgstr "cztery"
 
-#: src/humanize/number.py:251
+#: src/humanize/number.py:306
 msgid "five"
-msgstr "viisi"
+msgstr "pięć"
 
-#: src/humanize/number.py:252
+#: src/humanize/number.py:307
 msgid "six"
-msgstr "kuusi"
+msgstr "sześć"
 
-#: src/humanize/number.py:253
+#: src/humanize/number.py:308
 msgid "seven"
-msgstr "seitsemän"
+msgstr "siedem"
 
-#: src/humanize/number.py:254
+#: src/humanize/number.py:309
 msgid "eight"
-msgstr "kahdeksan"
+msgstr "osiem"
 
-#: src/humanize/number.py:255
+#: src/humanize/number.py:310
 msgid "nine"
-msgstr "yhdeksän"
+msgstr "dziewięć"
 
-#: src/humanize/time.py:133
-#, fuzzy, python-format
+#: src/humanize/time.py:152
+#, python-format
 msgid "%d microsecond"
 msgid_plural "%d microseconds"
-msgstr[0] "%d mikrosekunti"
-msgstr[1] "%d mikrosekuntia"
+msgstr[0] "%d mikrosekunda"
+msgstr[1] "%d mikrosekundy"
+msgstr[2] "%d mikrosekund"
 
-#: src/humanize/time.py:142
-#, fuzzy, python-format
+#: src/humanize/time.py:161
+#, python-format
 msgid "%d millisecond"
 msgid_plural "%d milliseconds"
-msgstr[0] "%d millisekunti"
-msgstr[1] "%d millisekuntia"
+msgstr[0] "%d milisekunda"
+msgstr[1] "%d milisekundy"
+msgstr[2] "%d milisekund"
 
-#: src/humanize/time.py:145 src/humanize/time.py:220
+#: src/humanize/time.py:164 src/humanize/time.py:259
 msgid "a moment"
-msgstr "hetki"
+msgstr "chwila"
 
-#: src/humanize/time.py:147
+#: src/humanize/time.py:167
 msgid "a second"
-msgstr "sekunti"
+msgstr "sekunda"
 
-#: src/humanize/time.py:149
+#: src/humanize/time.py:170
 #, python-format
 msgid "%d second"
 msgid_plural "%d seconds"
-msgstr[0] "%d sekunti"
-msgstr[1] "%d sekuntia"
+msgstr[0] "%d sekunda"
+msgstr[1] "%d sekundy"
+msgstr[2] "%d sekund"
 
-#: src/humanize/time.py:151
+#: src/humanize/time.py:173
 msgid "a minute"
-msgstr "minuutti"
+msgstr "minuta"
 
-#: src/humanize/time.py:154
+#: src/humanize/time.py:177
 #, python-format
 msgid "%d minute"
 msgid_plural "%d minutes"
-msgstr[0] "%d minuutti"
-msgstr[1] "%d minuuttia"
+msgstr[0] "%d minuta"
+msgstr[1] "%d minuty"
+msgstr[2] "%d minut"
 
-#: src/humanize/time.py:156
+#: src/humanize/time.py:180
 msgid "an hour"
-msgstr "tunti"
+msgstr "godzina"
 
-#: src/humanize/time.py:159
+#: src/humanize/time.py:184
 #, python-format
 msgid "%d hour"
 msgid_plural "%d hours"
-msgstr[0] "%d tunti"
-msgstr[1] "%d tuntia"
+msgstr[0] "%d godzina"
+msgstr[1] "%d godziny"
+msgstr[2] "%d godzin"
 
-#: src/humanize/time.py:162
+#: src/humanize/time.py:188
 msgid "a day"
-msgstr "päivä"
+msgstr "dzień"
 
-#: src/humanize/time.py:164 src/humanize/time.py:167
+#: src/humanize/time.py:191 src/humanize/time.py:194
 #, python-format
 msgid "%d day"
 msgid_plural "%d days"
-msgstr[0] "%d päivä"
-msgstr[1] "%d päivää"
+msgstr[0] "%d dzień"
+msgstr[1] "%d dni"
+msgstr[2] "%d dni"
 
-#: src/humanize/time.py:169
+#: src/humanize/time.py:197
 msgid "a month"
-msgstr "kuukausi"
+msgstr "miesiąc"
 
-#: src/humanize/time.py:171
+#: src/humanize/time.py:199
 #, python-format
 msgid "%d month"
 msgid_plural "%d months"
-msgstr[0] "%d kuukausi"
-msgstr[1] "%d kuukautta"
+msgstr[0] "%d miesiąc"
+msgstr[1] "%d miesiące"
+msgstr[2] "%d miesięcy"
 
-#: src/humanize/time.py:174
+#: src/humanize/time.py:203
 msgid "a year"
-msgstr "vuosi"
+msgstr "rok"
 
-#: src/humanize/time.py:176 src/humanize/time.py:185
+#: src/humanize/time.py:206 src/humanize/time.py:217
 #, python-format
 msgid "1 year, %d day"
 msgid_plural "1 year, %d days"
-msgstr[0] "1 vuosi, %d päivä"
-msgstr[1] "1 vuosi, %d päivää"
+msgstr[0] "1 rok, %d dzień"
+msgstr[1] "1 rok, %d dni"
+msgstr[2] "1 rok, %d dni"
 
-#: src/humanize/time.py:179
+#: src/humanize/time.py:210
 msgid "1 year, 1 month"
-msgstr "1 vuosi, 1 kuukausi"
+msgstr "1 rok, 1 miesiąc"
 
-#: src/humanize/time.py:182
+#: src/humanize/time.py:213
 #, python-format
 msgid "1 year, %d month"
 msgid_plural "1 year, %d months"
-msgstr[0] "1 vuosi, %d kuukausi"
-msgstr[1] "1 vuosi, %d kuukautta"
+msgstr[0] "1 rok, %d miesiąc"
+msgstr[1] "1 rok, %d miesiące"
+msgstr[2] "1 rok, %d miesięcy"
 
-#: src/humanize/time.py:187
+#: src/humanize/time.py:219
 #, python-format
 msgid "%d year"
 msgid_plural "%d years"
-msgstr[0] "%d vuosi"
-msgstr[1] "%d vuotta"
+msgstr[0] "%d rok"
+msgstr[1] "%d lata"
+msgstr[2] "%d lat"
 
-#: src/humanize/time.py:217
+#: src/humanize/time.py:256
 #, python-format
 msgid "%s from now"
-msgstr "%s tästä"
+msgstr "%s od teraz"
 
-#: src/humanize/time.py:217
+#: src/humanize/time.py:256
 #, python-format
 msgid "%s ago"
-msgstr "%s sitten"
+msgstr "%s temu"
 
-#: src/humanize/time.py:221
+#: src/humanize/time.py:260
 msgid "now"
-msgstr "nyt"
+msgstr "teraz"
 
-#: src/humanize/time.py:244
+#: src/humanize/time.py:284
 msgid "today"
-msgstr "tänään"
+msgstr "dziś"
 
-#: src/humanize/time.py:246
+#: src/humanize/time.py:287
 msgid "tomorrow"
-msgstr "huomenna"
+msgstr "jutro"
 
-#: src/humanize/time.py:248
+#: src/humanize/time.py:290
 msgid "yesterday"
-msgstr "eilen"
+msgstr "wczoraj"
 
-#: src/humanize/time.py:534
+#: src/humanize/time.py:600
 #, python-format
 msgid "%s and %s"
-msgstr "%s ja %s"
+msgstr "%s i %s"
```

### Comparing `humanize-4.5.0/src/humanize/locale/fr_FR/LC_MESSAGES/humanize.mo` & `humanize-4.6.0/src/humanize/locale/fr_FR/LC_MESSAGES/humanize.mo`

 * *Files identical despite different names*

### Comparing `humanize-4.5.0/src/humanize/locale/fr_FR/LC_MESSAGES/humanize.po` & `humanize-4.6.0/src/humanize/locale/vi_VN/LC_MESSAGES/humanize.po`

 * *Files 6% similar despite different names*

```diff
@@ -1,375 +1,372 @@
-# French (France) translations for PROJECT.
+# Vietnamese (Vietnam) translations for PROJECT.
 # Copyright (C) 2013 ORGANIZATION
 # This file is distributed under the same license as the PROJECT project.
 # FIRST AUTHOR <EMAIL@ADDRESS>, 2013.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2021-05-04 23:15+0200\n"
-"PO-Revision-Date: 2013-06-22 08:52+0100\n"
+"POT-Creation-Date: 2023-01-08 19:22+0200\n"
+"PO-Revision-Date: 2017-05-30 11:51+0700\n"
 "Last-Translator: Olivier Cortès <oc@1flow.io>\n"
-"Language-Team: fr_FR <LL@li.org>\n"
-"Language: fr\n"
+"Language-Team: vi_VI <sapd@vccloud.vn>\n"
+"Language: vi_VN\n"
 "MIME-Version: 1.0\n"
-"Content-Type: text/plain; charset=utf-8\n"
+"Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n > 1);\n"
 "Generated-By: Babel 0.9.6\n"
-"X-Generator: Poedit 1.5.5\n"
+"X-Generator: Poedit 1.8.7.1\n"
 
-#: src/humanize/number.py:57
+#: src/humanize/number.py:84
 msgctxt "0 (male)"
 msgid "th"
-msgstr "e"
+msgstr "."
 
-#: src/humanize/number.py:58
+#: src/humanize/number.py:85
 msgctxt "1 (male)"
 msgid "st"
-msgstr "er"
+msgstr "."
 
-#: src/humanize/number.py:59
+#: src/humanize/number.py:86
 msgctxt "2 (male)"
 msgid "nd"
-msgstr "e"
+msgstr "."
 
-#: src/humanize/number.py:60
+#: src/humanize/number.py:87
 msgctxt "3 (male)"
 msgid "rd"
-msgstr "e"
+msgstr "."
 
-#: src/humanize/number.py:61
+#: src/humanize/number.py:88
 msgctxt "4 (male)"
 msgid "th"
-msgstr "e"
+msgstr "."
 
-#: src/humanize/number.py:62
+#: src/humanize/number.py:89
 msgctxt "5 (male)"
 msgid "th"
-msgstr "e"
+msgstr "."
 
-#: src/humanize/number.py:63
+#: src/humanize/number.py:90
 msgctxt "6 (male)"
 msgid "th"
-msgstr "e"
+msgstr "."
 
-#: src/humanize/number.py:64
+#: src/humanize/number.py:91
 msgctxt "7 (male)"
 msgid "th"
-msgstr "e"
+msgstr "."
 
-#: src/humanize/number.py:65
+#: src/humanize/number.py:92
 msgctxt "8 (male)"
 msgid "th"
-msgstr "e"
+msgstr "."
 
-#: src/humanize/number.py:66
+#: src/humanize/number.py:93
 msgctxt "9 (male)"
 msgid "th"
-msgstr "e"
+msgstr "."
 
-#: src/humanize/number.py:70
+#: src/humanize/number.py:97
 msgctxt "0 (female)"
 msgid "th"
-msgstr "e"
+msgstr "."
 
-#: src/humanize/number.py:71
+#: src/humanize/number.py:98
 msgctxt "1 (female)"
 msgid "st"
-msgstr "ère"
+msgstr "."
 
-#: src/humanize/number.py:72
+#: src/humanize/number.py:99
 msgctxt "2 (female)"
 msgid "nd"
-msgstr "e"
+msgstr "."
 
-#: src/humanize/number.py:73
+#: src/humanize/number.py:100
 msgctxt "3 (female)"
 msgid "rd"
-msgstr "e"
+msgstr "."
 
-#: src/humanize/number.py:74
+#: src/humanize/number.py:101
 msgctxt "4 (female)"
 msgid "th"
-msgstr "e"
+msgstr "."
 
-#: src/humanize/number.py:75
+#: src/humanize/number.py:102
 msgctxt "5 (female)"
 msgid "th"
-msgstr "e"
+msgstr "."
 
-#: src/humanize/number.py:76
+#: src/humanize/number.py:103
 msgctxt "6 (female)"
 msgid "th"
-msgstr "e"
+msgstr "."
 
-#: src/humanize/number.py:77
+#: src/humanize/number.py:104
 msgctxt "7 (female)"
 msgid "th"
-msgstr "e"
+msgstr "."
 
-#: src/humanize/number.py:78
+#: src/humanize/number.py:105
 msgctxt "8 (female)"
 msgid "th"
-msgstr "e"
+msgstr "."
 
-#: src/humanize/number.py:79
+#: src/humanize/number.py:106
 msgctxt "9 (female)"
 msgid "th"
-msgstr "e"
+msgstr "."
 
-#: src/humanize/number.py:140
+#: src/humanize/number.py:178
 msgid "thousand"
 msgid_plural "thousand"
-msgstr[0] ""
-msgstr[1] ""
+msgstr[0] "nghìn"
+msgstr[1] "nghìn"
 
-#: src/humanize/number.py:141
-#, fuzzy
+#: src/humanize/number.py:179
 msgid "million"
 msgid_plural "million"
-msgstr[0] "%(value)s million"
-msgstr[1] "%(value)s million"
+msgstr[0] "%(value)s triệu"
+msgstr[1] "%(value)s triệu"
 
-#: src/humanize/number.py:142
+#: src/humanize/number.py:180
 msgid "billion"
 msgid_plural "billion"
-msgstr[0] "milliard"
-msgstr[1] "milliard"
+msgstr[0] "tỷ"
+msgstr[1] "tỷ"
 
-#: src/humanize/number.py:143
-#, fuzzy
+#: src/humanize/number.py:181
 msgid "trillion"
 msgid_plural "trillion"
-msgstr[0] "%(value)s billion"
-msgstr[1] "%(value)s billion"
+msgstr[0] "%(value)s nghìn tỷ"
+msgstr[1] "%(value)s nghìn tỷ"
 
-#: src/humanize/number.py:144
-#, fuzzy
+#: src/humanize/number.py:182
 msgid "quadrillion"
 msgid_plural "quadrillion"
-msgstr[0] "%(value)s billiard"
-msgstr[1] "%(value)s billiard"
+msgstr[0] "%(value)s triệu tỷ"
+msgstr[1] "%(value)s triệu tỷ"
 
-#: src/humanize/number.py:145
+#: src/humanize/number.py:183
 #, fuzzy
 msgid "quintillion"
 msgid_plural "quintillion"
-msgstr[0] "%(value)s trillion"
-msgstr[1] "%(value)s trillion"
+msgstr[0] "%(value)s tỷ tỷ"
+msgstr[1] "%(value)s tỷ tỷ"
 
-#: src/humanize/number.py:146
+#: src/humanize/number.py:184
 #, fuzzy
 msgid "sextillion"
 msgid_plural "sextillion"
-msgstr[0] "%(value)s trilliard"
-msgstr[1] "%(value)s trilliard"
+msgstr[0] "%(value)s sextillion"
+msgstr[1] "%(value)s sextillion"
 
-#: src/humanize/number.py:147
+#: src/humanize/number.py:185
 #, fuzzy
 msgid "septillion"
 msgid_plural "septillion"
-msgstr[0] "%(value)s quatrillion"
-msgstr[1] "%(value)s quatrillion"
+msgstr[0] "%(value)s septillion"
+msgstr[1] "%(value)s septillion"
 
-#: src/humanize/number.py:148
+#: src/humanize/number.py:186
 #, fuzzy
 msgid "octillion"
 msgid_plural "octillion"
-msgstr[0] "%(value)s quadrilliard"
-msgstr[1] "%(value)s quadrilliard"
+msgstr[0] "%(value)s octillion"
+msgstr[1] "%(value)s octillion"
 
-#: src/humanize/number.py:149
+#: src/humanize/number.py:187
 #, fuzzy
 msgid "nonillion"
 msgid_plural "nonillion"
-msgstr[0] "%(value)s quintillion"
-msgstr[1] "%(value)s quintillion"
+msgstr[0] "%(value)s nonillion"
+msgstr[1] "%(value)s nonillion"
 
-#: src/humanize/number.py:150
+#: src/humanize/number.py:188
 #, fuzzy
 msgid "decillion"
 msgid_plural "decillion"
-msgstr[0] "%(value)s quintilliard"
-msgstr[1] "%(value)s quintilliard"
+msgstr[0] "%(value)s décillion"
+msgstr[1] "%(value)s décillion"
 
-#: src/humanize/number.py:151
+#: src/humanize/number.py:189
 #, fuzzy
 msgid "googol"
 msgid_plural "googol"
 msgstr[0] "%(value)s gogol"
 msgstr[1] "%(value)s gogol"
 
-#: src/humanize/number.py:246
+#: src/humanize/number.py:301
 msgid "zero"
-msgstr "zéro"
+msgstr "không"
 
-#: src/humanize/number.py:247
+#: src/humanize/number.py:302
 msgid "one"
-msgstr "un"
+msgstr "một"
 
-#: src/humanize/number.py:248
+#: src/humanize/number.py:303
 msgid "two"
-msgstr "deux"
+msgstr "hai"
 
-#: src/humanize/number.py:249
+#: src/humanize/number.py:304
 msgid "three"
-msgstr "trois"
+msgstr "ba"
 
-#: src/humanize/number.py:250
+#: src/humanize/number.py:305
 msgid "four"
-msgstr "quatre"
+msgstr "bốn"
 
-#: src/humanize/number.py:251
+#: src/humanize/number.py:306
 msgid "five"
-msgstr "cinq"
+msgstr "năm"
 
-#: src/humanize/number.py:252
+#: src/humanize/number.py:307
 msgid "six"
-msgstr "six"
+msgstr "sáu"
 
-#: src/humanize/number.py:253
+#: src/humanize/number.py:308
 msgid "seven"
-msgstr "sept"
+msgstr "bảy"
 
-#: src/humanize/number.py:254
+#: src/humanize/number.py:309
 msgid "eight"
-msgstr "huit"
+msgstr "tám"
 
-#: src/humanize/number.py:255
+#: src/humanize/number.py:310
 msgid "nine"
-msgstr "neuf"
+msgstr "chín"
 
-#: src/humanize/time.py:133
-#, fuzzy, python-format
+#: src/humanize/time.py:152
+#, python-format
 msgid "%d microsecond"
 msgid_plural "%d microseconds"
-msgstr[0] "%d microseconde"
-msgstr[1] "%d microsecondes"
+msgstr[0] "%d micro giây"
+msgstr[1] "%d micro giây"
 
-#: src/humanize/time.py:142
-#, fuzzy, python-format
+#: src/humanize/time.py:161
+#, python-format
 msgid "%d millisecond"
 msgid_plural "%d milliseconds"
-msgstr[0] "%d milliseconde"
-msgstr[1] "%d millisecondes"
+msgstr[0] "%d mili giây"
+msgstr[1] "%d mili giây"
 
-#: src/humanize/time.py:145 src/humanize/time.py:220
+#: src/humanize/time.py:164 src/humanize/time.py:259
 msgid "a moment"
-msgstr "un moment"
+msgstr "ngay lúc này"
 
-#: src/humanize/time.py:147
+#: src/humanize/time.py:167
 msgid "a second"
-msgstr "une seconde"
+msgstr "một giây"
 
-#: src/humanize/time.py:149
+#: src/humanize/time.py:170
 #, python-format
 msgid "%d second"
 msgid_plural "%d seconds"
-msgstr[0] "%d seconde"
-msgstr[1] "%d secondes"
+msgstr[0] "%d giây"
+msgstr[1] "%d giây"
 
-#: src/humanize/time.py:151
+#: src/humanize/time.py:173
 msgid "a minute"
-msgstr "une minute"
+msgstr "một phút"
 
-#: src/humanize/time.py:154
+#: src/humanize/time.py:177
 #, python-format
 msgid "%d minute"
 msgid_plural "%d minutes"
-msgstr[0] "%d minute"
-msgstr[1] "%d minutes"
+msgstr[0] "%d phút"
+msgstr[1] "%d phút"
 
-#: src/humanize/time.py:156
+#: src/humanize/time.py:180
 msgid "an hour"
-msgstr "une heure"
+msgstr "một giờ"
 
-#: src/humanize/time.py:159
+#: src/humanize/time.py:184
 #, python-format
 msgid "%d hour"
 msgid_plural "%d hours"
-msgstr[0] "%d heure"
-msgstr[1] "%d heures"
+msgstr[0] "%d giờ"
+msgstr[1] "%d giờ"
 
-#: src/humanize/time.py:162
+#: src/humanize/time.py:188
 msgid "a day"
-msgstr "un jour"
+msgstr "một ngày"
 
-#: src/humanize/time.py:164 src/humanize/time.py:167
+#: src/humanize/time.py:191 src/humanize/time.py:194
 #, python-format
 msgid "%d day"
 msgid_plural "%d days"
-msgstr[0] "%d jour"
-msgstr[1] "%d jours"
+msgstr[0] "%d ngày"
+msgstr[1] "%d ngày"
 
-#: src/humanize/time.py:169
+#: src/humanize/time.py:197
 msgid "a month"
-msgstr "un mois"
+msgstr "một tháng"
 
-#: src/humanize/time.py:171
+#: src/humanize/time.py:199
 #, python-format
 msgid "%d month"
 msgid_plural "%d months"
-msgstr[0] "%d mois"
-msgstr[1] "%d mois"
+msgstr[0] "%d tháng"
+msgstr[1] "%d tháng"
 
-#: src/humanize/time.py:174
+#: src/humanize/time.py:203
 msgid "a year"
-msgstr "un an"
+msgstr "một năm"
 
-#: src/humanize/time.py:176 src/humanize/time.py:185
+#: src/humanize/time.py:206 src/humanize/time.py:217
 #, python-format
 msgid "1 year, %d day"
 msgid_plural "1 year, %d days"
-msgstr[0] "un an et %d jour"
-msgstr[1] "un an et %d jours"
+msgstr[0] "1 năm %d ngày"
+msgstr[1] "1 năm %d ngày"
 
-#: src/humanize/time.py:179
+#: src/humanize/time.py:210
 msgid "1 year, 1 month"
-msgstr "un an et un mois"
+msgstr "1 năm 1 tháng"
 
-#: src/humanize/time.py:182
+#: src/humanize/time.py:213
 #, python-format
 msgid "1 year, %d month"
 msgid_plural "1 year, %d months"
-msgstr[0] "un an et %d mois"
+msgstr[0] "1 năm %d tháng"
 msgstr[1] "un an et %d mois"
 
-#: src/humanize/time.py:187
+#: src/humanize/time.py:219
 #, python-format
 msgid "%d year"
 msgid_plural "%d years"
-msgstr[0] "%d an"
-msgstr[1] "%d ans"
+msgstr[0] "%d năm"
+msgstr[1] "%d năm"
 
-#: src/humanize/time.py:217
+#: src/humanize/time.py:256
 #, python-format
 msgid "%s from now"
-msgstr "dans %s"
+msgstr "%s ngày tới"
 
-#: src/humanize/time.py:217
+#: src/humanize/time.py:256
 #, python-format
 msgid "%s ago"
-msgstr "il y a %s"
+msgstr "%s trước"
 
-#: src/humanize/time.py:221
+#: src/humanize/time.py:260
 msgid "now"
-msgstr "maintenant"
+msgstr "ngay bây giờ"
 
-#: src/humanize/time.py:244
+#: src/humanize/time.py:284
 msgid "today"
-msgstr "aujourd'hui"
+msgstr "hôm nay"
 
-#: src/humanize/time.py:246
+#: src/humanize/time.py:287
 msgid "tomorrow"
-msgstr "demain"
+msgstr "ngày mai"
 
-#: src/humanize/time.py:248
+#: src/humanize/time.py:290
 msgid "yesterday"
-msgstr "hier"
+msgstr "ngày hôm qua"
 
-#: src/humanize/time.py:534
+#: src/humanize/time.py:600
 #, python-format
 msgid "%s and %s"
-msgstr "%s et %s"
+msgstr "%s và %s"
```

### Comparing `humanize-4.5.0/src/humanize/locale/id_ID/LC_MESSAGES/humanize.mo` & `humanize-4.6.0/src/humanize/locale/id_ID/LC_MESSAGES/humanize.mo`

 * *Files identical despite different names*

### Comparing `humanize-4.5.0/src/humanize/locale/id_ID/LC_MESSAGES/humanize.po` & `humanize-4.6.0/src/humanize/locale/id_ID/LC_MESSAGES/humanize.po`

 * *Files 5% similar despite different names*

```diff
@@ -3,340 +3,340 @@
 # This file is distributed under the same license as the PACKAGE package.
 #  <adie.rebel@gmail.com>, 2017.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: \n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2021-05-04 23:15+0200\n"
+"POT-Creation-Date: 2023-01-08 19:22+0200\n"
 "PO-Revision-Date: 2017-03-18 15:41+0700\n"
 "Last-Translator: adie.rebel@gmail.com\n"
 "Language-Team: Indonesian\n"
 "Language: id\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=ASCII\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 "X-Generator: Poedit 1.8.11\n"
 
-#: src/humanize/number.py:57
+#: src/humanize/number.py:84
 msgctxt "0 (male)"
 msgid "th"
 msgstr "."
 
-#: src/humanize/number.py:58
+#: src/humanize/number.py:85
 msgctxt "1 (male)"
 msgid "st"
 msgstr "."
 
-#: src/humanize/number.py:59
+#: src/humanize/number.py:86
 msgctxt "2 (male)"
 msgid "nd"
 msgstr "."
 
-#: src/humanize/number.py:60
+#: src/humanize/number.py:87
 msgctxt "3 (male)"
 msgid "rd"
 msgstr "."
 
-#: src/humanize/number.py:61
+#: src/humanize/number.py:88
 msgctxt "4 (male)"
 msgid "th"
 msgstr "."
 
-#: src/humanize/number.py:62
+#: src/humanize/number.py:89
 msgctxt "5 (male)"
 msgid "th"
 msgstr "."
 
-#: src/humanize/number.py:63
+#: src/humanize/number.py:90
 msgctxt "6 (male)"
 msgid "th"
 msgstr "."
 
-#: src/humanize/number.py:64
+#: src/humanize/number.py:91
 msgctxt "7 (male)"
 msgid "th"
 msgstr "."
 
-#: src/humanize/number.py:65
+#: src/humanize/number.py:92
 msgctxt "8 (male)"
 msgid "th"
 msgstr "."
 
-#: src/humanize/number.py:66
+#: src/humanize/number.py:93
 msgctxt "9 (male)"
 msgid "th"
 msgstr "."
 
-#: src/humanize/number.py:70
+#: src/humanize/number.py:97
 msgctxt "0 (female)"
 msgid "th"
 msgstr "."
 
-#: src/humanize/number.py:71
+#: src/humanize/number.py:98
 msgctxt "1 (female)"
 msgid "st"
 msgstr "."
 
-#: src/humanize/number.py:72
+#: src/humanize/number.py:99
 msgctxt "2 (female)"
 msgid "nd"
 msgstr "."
 
-#: src/humanize/number.py:73
+#: src/humanize/number.py:100
 msgctxt "3 (female)"
 msgid "rd"
 msgstr "."
 
-#: src/humanize/number.py:74
+#: src/humanize/number.py:101
 msgctxt "4 (female)"
 msgid "th"
 msgstr "."
 
-#: src/humanize/number.py:75
+#: src/humanize/number.py:102
 msgctxt "5 (female)"
 msgid "th"
 msgstr "."
 
-#: src/humanize/number.py:76
+#: src/humanize/number.py:103
 msgctxt "6 (female)"
 msgid "th"
 msgstr "."
 
-#: src/humanize/number.py:77
+#: src/humanize/number.py:104
 msgctxt "7 (female)"
 msgid "th"
 msgstr "."
 
-#: src/humanize/number.py:78
+#: src/humanize/number.py:105
 msgctxt "8 (female)"
 msgid "th"
 msgstr "."
 
-#: src/humanize/number.py:79
+#: src/humanize/number.py:106
 msgctxt "9 (female)"
 msgid "th"
 msgstr "."
 
-#: src/humanize/number.py:140
+#: src/humanize/number.py:178
 msgid "thousand"
 msgid_plural "thousand"
 msgstr[0] ""
 
-#: src/humanize/number.py:141
+#: src/humanize/number.py:179
 msgid "million"
 msgid_plural "million"
 msgstr[0] "juta"
 
-#: src/humanize/number.py:142
+#: src/humanize/number.py:180
 msgid "billion"
 msgid_plural "billion"
 msgstr[0] "miliar"
 
-#: src/humanize/number.py:143
+#: src/humanize/number.py:181
 msgid "trillion"
 msgid_plural "trillion"
 msgstr[0] "triliun"
 
-#: src/humanize/number.py:144
+#: src/humanize/number.py:182
 msgid "quadrillion"
 msgid_plural "quadrillion"
 msgstr[0] "kuadriliun"
 
-#: src/humanize/number.py:145
+#: src/humanize/number.py:183
 msgid "quintillion"
 msgid_plural "quintillion"
 msgstr[0] "quintillion"
 
-#: src/humanize/number.py:146
+#: src/humanize/number.py:184
 msgid "sextillion"
 msgid_plural "sextillion"
 msgstr[0] "sextillion"
 
-#: src/humanize/number.py:147
+#: src/humanize/number.py:185
 msgid "septillion"
 msgid_plural "septillion"
 msgstr[0] "septillion"
 
-#: src/humanize/number.py:148
+#: src/humanize/number.py:186
 msgid "octillion"
 msgid_plural "octillion"
 msgstr[0] "octillion"
 
-#: src/humanize/number.py:149
+#: src/humanize/number.py:187
 msgid "nonillion"
 msgid_plural "nonillion"
 msgstr[0] "nonillion"
 
-#: src/humanize/number.py:150
+#: src/humanize/number.py:188
 msgid "decillion"
 msgid_plural "decillion"
 msgstr[0] "decillion"
 
-#: src/humanize/number.py:151
+#: src/humanize/number.py:189
 msgid "googol"
 msgid_plural "googol"
 msgstr[0] "googol"
 
-#: src/humanize/number.py:246
+#: src/humanize/number.py:301
 msgid "zero"
 msgstr "nol"
 
-#: src/humanize/number.py:247
+#: src/humanize/number.py:302
 msgid "one"
 msgstr "satu"
 
-#: src/humanize/number.py:248
+#: src/humanize/number.py:303
 msgid "two"
 msgstr "dua"
 
-#: src/humanize/number.py:249
+#: src/humanize/number.py:304
 msgid "three"
 msgstr "tiga"
 
-#: src/humanize/number.py:250
+#: src/humanize/number.py:305
 msgid "four"
 msgstr "empat"
 
-#: src/humanize/number.py:251
+#: src/humanize/number.py:306
 msgid "five"
 msgstr "lima"
 
-#: src/humanize/number.py:252
+#: src/humanize/number.py:307
 msgid "six"
 msgstr "enam"
 
-#: src/humanize/number.py:253
+#: src/humanize/number.py:308
 msgid "seven"
 msgstr "tujuh"
 
-#: src/humanize/number.py:254
+#: src/humanize/number.py:309
 msgid "eight"
 msgstr "delapan"
 
-#: src/humanize/number.py:255
+#: src/humanize/number.py:310
 msgid "nine"
 msgstr "sembilan"
 
-#: src/humanize/time.py:133
+#: src/humanize/time.py:152
 #, fuzzy, python-format
 msgid "%d microsecond"
 msgid_plural "%d microseconds"
 msgstr[0] "%d mikro detik"
 
-#: src/humanize/time.py:142
+#: src/humanize/time.py:161
 #, fuzzy, python-format
 msgid "%d millisecond"
 msgid_plural "%d milliseconds"
 msgstr[0] "%d mili detik"
 
-#: src/humanize/time.py:145 src/humanize/time.py:220
+#: src/humanize/time.py:164 src/humanize/time.py:259
 msgid "a moment"
 msgstr "beberapa saat"
 
-#: src/humanize/time.py:147
+#: src/humanize/time.py:167
 msgid "a second"
 msgstr "sedetik"
 
-#: src/humanize/time.py:149
+#: src/humanize/time.py:170
 #, python-format
 msgid "%d second"
 msgid_plural "%d seconds"
 msgstr[0] "%d detik"
 
-#: src/humanize/time.py:151
+#: src/humanize/time.py:173
 msgid "a minute"
 msgstr "semenit"
 
-#: src/humanize/time.py:154
+#: src/humanize/time.py:177
 #, python-format
 msgid "%d minute"
 msgid_plural "%d minutes"
 msgstr[0] "%d menit"
 
-#: src/humanize/time.py:156
+#: src/humanize/time.py:180
 msgid "an hour"
 msgstr "sejam"
 
-#: src/humanize/time.py:159
+#: src/humanize/time.py:184
 #, python-format
 msgid "%d hour"
 msgid_plural "%d hours"
 msgstr[0] "%d jam"
 
-#: src/humanize/time.py:162
+#: src/humanize/time.py:188
 msgid "a day"
 msgstr "sehari"
 
-#: src/humanize/time.py:164 src/humanize/time.py:167
+#: src/humanize/time.py:191 src/humanize/time.py:194
 #, python-format
 msgid "%d day"
 msgid_plural "%d days"
 msgstr[0] "%d hari"
 
-#: src/humanize/time.py:169
+#: src/humanize/time.py:197
 msgid "a month"
 msgstr "sebulan"
 
-#: src/humanize/time.py:171
+#: src/humanize/time.py:199
 #, python-format
 msgid "%d month"
 msgid_plural "%d months"
 msgstr[0] "%d bulan"
 
-#: src/humanize/time.py:174
+#: src/humanize/time.py:203
 msgid "a year"
 msgstr "setahun"
 
-#: src/humanize/time.py:176 src/humanize/time.py:185
+#: src/humanize/time.py:206 src/humanize/time.py:217
 #, python-format
 msgid "1 year, %d day"
 msgid_plural "1 year, %d days"
 msgstr[0] "1 tahun, %d hari"
 
-#: src/humanize/time.py:179
+#: src/humanize/time.py:210
 msgid "1 year, 1 month"
 msgstr "1 tahun, 1 bulan"
 
-#: src/humanize/time.py:182
+#: src/humanize/time.py:213
 #, python-format
 msgid "1 year, %d month"
 msgid_plural "1 year, %d months"
 msgstr[0] "1 tahun, %d bulan"
 
-#: src/humanize/time.py:187
+#: src/humanize/time.py:219
 #, python-format
 msgid "%d year"
 msgid_plural "%d years"
 msgstr[0] "%d tahun"
 
-#: src/humanize/time.py:217
+#: src/humanize/time.py:256
 #, python-format
 msgid "%s from now"
 msgstr "%s dari sekarang"
 
-#: src/humanize/time.py:217
+#: src/humanize/time.py:256
 #, python-format
 msgid "%s ago"
 msgstr "%s yang lalu"
 
-#: src/humanize/time.py:221
+#: src/humanize/time.py:260
 msgid "now"
 msgstr "sekarang"
 
-#: src/humanize/time.py:244
+#: src/humanize/time.py:284
 msgid "today"
 msgstr "hari ini"
 
-#: src/humanize/time.py:246
+#: src/humanize/time.py:287
 msgid "tomorrow"
 msgstr "besok"
 
-#: src/humanize/time.py:248
+#: src/humanize/time.py:290
 msgid "yesterday"
 msgstr "kemarin"
 
-#: src/humanize/time.py:534
+#: src/humanize/time.py:600
 #, python-format
 msgid "%s and %s"
 msgstr "%s dan %s"
```

### Comparing `humanize-4.5.0/src/humanize/locale/it_IT/LC_MESSAGES/humanize.po` & `humanize-4.6.0/src/humanize/locale/pt_PT/LC_MESSAGES/humanize.po`

 * *Files 7% similar despite different names*

```diff
@@ -1,364 +1,364 @@
-# Italian translations for PACKAGE package.
-# Copyright (C) 2018 THE PACKAGE'S COPYRIGHT HOLDER
+# SOME DESCRIPTIVE TITLE.
+# Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
-# derfel <code@derfel.net>, 2018.
+# FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: \n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2021-05-04 23:15+0200\n"
-"PO-Revision-Date: 2018-10-27 22:52+0200\n"
-"Last-Translator: derfel <code@derfel.net>\n"
-"Language-Team: Italian\n"
-"Language: it\n"
+"POT-Creation-Date: 2023-01-08 19:22+0200\n"
+"PO-Revision-Date: 2020-07-05 18:17+0100\n"
+"Last-Translator: \n"
+"Language-Team: \n"
+"Language: pt_PT\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=(n != 1);\n"
-"X-Generator: Poedit 2.2\n"
+"Plural-Forms: nplurals=2; plural=(n > 1);\n"
+"X-Generator: Poedit 2.3.1\n"
 
-#: src/humanize/number.py:57
+#: src/humanize/number.py:84
 msgctxt "0 (male)"
 msgid "th"
 msgstr "º"
 
-#: src/humanize/number.py:58
+#: src/humanize/number.py:85
 msgctxt "1 (male)"
 msgid "st"
 msgstr "º"
 
-#: src/humanize/number.py:59
+#: src/humanize/number.py:86
 msgctxt "2 (male)"
 msgid "nd"
 msgstr "º"
 
-#: src/humanize/number.py:60
+#: src/humanize/number.py:87
 msgctxt "3 (male)"
 msgid "rd"
 msgstr "º"
 
-#: src/humanize/number.py:61
+#: src/humanize/number.py:88
 msgctxt "4 (male)"
 msgid "th"
 msgstr "º"
 
-#: src/humanize/number.py:62
+#: src/humanize/number.py:89
 msgctxt "5 (male)"
 msgid "th"
 msgstr "º"
 
-#: src/humanize/number.py:63
+#: src/humanize/number.py:90
 msgctxt "6 (male)"
 msgid "th"
 msgstr "º"
 
-#: src/humanize/number.py:64
+#: src/humanize/number.py:91
 msgctxt "7 (male)"
 msgid "th"
 msgstr "º"
 
-#: src/humanize/number.py:65
+#: src/humanize/number.py:92
 msgctxt "8 (male)"
 msgid "th"
 msgstr "º"
 
-#: src/humanize/number.py:66
+#: src/humanize/number.py:93
 msgctxt "9 (male)"
 msgid "th"
 msgstr "º"
 
-#: src/humanize/number.py:70
+#: src/humanize/number.py:97
 msgctxt "0 (female)"
 msgid "th"
 msgstr "ª"
 
-#: src/humanize/number.py:71
+#: src/humanize/number.py:98
 msgctxt "1 (female)"
 msgid "st"
 msgstr "ª"
 
-#: src/humanize/number.py:72
+#: src/humanize/number.py:99
 msgctxt "2 (female)"
 msgid "nd"
 msgstr "ª"
 
-#: src/humanize/number.py:73
+#: src/humanize/number.py:100
 msgctxt "3 (female)"
 msgid "rd"
 msgstr "ª"
 
-#: src/humanize/number.py:74
+#: src/humanize/number.py:101
 msgctxt "4 (female)"
 msgid "th"
 msgstr "ª"
 
-#: src/humanize/number.py:75
+#: src/humanize/number.py:102
 msgctxt "5 (female)"
 msgid "th"
 msgstr "ª"
 
-#: src/humanize/number.py:76
+#: src/humanize/number.py:103
 msgctxt "6 (female)"
 msgid "th"
 msgstr "ª"
 
-#: src/humanize/number.py:77
+#: src/humanize/number.py:104
 msgctxt "7 (female)"
 msgid "th"
 msgstr "ª"
 
-#: src/humanize/number.py:78
+#: src/humanize/number.py:105
 msgctxt "8 (female)"
 msgid "th"
 msgstr "ª"
 
-#: src/humanize/number.py:79
+#: src/humanize/number.py:106
 msgctxt "9 (female)"
 msgid "th"
 msgstr "ª"
 
-#: src/humanize/number.py:140
+#: src/humanize/number.py:178
 msgid "thousand"
 msgid_plural "thousand"
 msgstr[0] ""
 msgstr[1] ""
 
-#: src/humanize/number.py:141
+#: src/humanize/number.py:179
 msgid "million"
 msgid_plural "million"
-msgstr[0] "milioni"
-msgstr[1] "milioni"
+msgstr[0] "milhão"
+msgstr[1] "milhão"
 
-#: src/humanize/number.py:142
+#: src/humanize/number.py:180
 msgid "billion"
 msgid_plural "billion"
-msgstr[0] "miliardi"
-msgstr[1] "miliardi"
+msgstr[0] "milhar de milhão"
+msgstr[1] "milhar de milhão"
 
-#: src/humanize/number.py:143
+#: src/humanize/number.py:181
 msgid "trillion"
 msgid_plural "trillion"
-msgstr[0] "bilioni"
-msgstr[1] "bilioni"
+msgstr[0] "bilião"
+msgstr[1] "bilião"
 
-#: src/humanize/number.py:144
+#: src/humanize/number.py:182
 msgid "quadrillion"
 msgid_plural "quadrillion"
-msgstr[0] "biliardi"
-msgstr[1] "biliardi"
+msgstr[0] "mil biliões"
+msgstr[1] "mil biliões"
 
-#: src/humanize/number.py:145
+#: src/humanize/number.py:183
 msgid "quintillion"
 msgid_plural "quintillion"
-msgstr[0] "trilioni"
-msgstr[1] "trilioni"
+msgstr[0] "trilião"
+msgstr[1] "trilião"
 
-#: src/humanize/number.py:146
+#: src/humanize/number.py:184
 msgid "sextillion"
 msgid_plural "sextillion"
-msgstr[0] "triliardi"
-msgstr[1] "triliardi"
+msgstr[0] "mil triliões"
+msgstr[1] "mil triliões"
 
-#: src/humanize/number.py:147
+#: src/humanize/number.py:185
 msgid "septillion"
 msgid_plural "septillion"
-msgstr[0] "quadrilioni"
-msgstr[1] "quadrilioni"
+msgstr[0] "quatrilião"
+msgstr[1] "quatrilião"
 
-#: src/humanize/number.py:148
+#: src/humanize/number.py:186
 msgid "octillion"
 msgid_plural "octillion"
-msgstr[0] "quadriliardi"
-msgstr[1] "quadriliardi"
+msgstr[0] "mil quatriliões"
+msgstr[1] "mil quatriliões"
 
-#: src/humanize/number.py:149
+#: src/humanize/number.py:187
 msgid "nonillion"
 msgid_plural "nonillion"
-msgstr[0] "quintilioni"
-msgstr[1] "quintilioni"
+msgstr[0] "quintilhão"
+msgstr[1] "quintilhão"
 
-#: src/humanize/number.py:150
+#: src/humanize/number.py:188
 msgid "decillion"
 msgid_plural "decillion"
-msgstr[0] "quintiliardi"
-msgstr[1] "quintiliardi"
+msgstr[0] "mil quintilhões"
+msgstr[1] "mil quintilhões"
 
-#: src/humanize/number.py:151
+#: src/humanize/number.py:189
 msgid "googol"
 msgid_plural "googol"
-msgstr[0] "googol"
-msgstr[1] "googol"
+msgstr[0] "sextilhão"
+msgstr[1] "sextilhão"
 
-#: src/humanize/number.py:246
+#: src/humanize/number.py:301
 msgid "zero"
 msgstr "zero"
 
-#: src/humanize/number.py:247
+#: src/humanize/number.py:302
 msgid "one"
-msgstr "uno"
+msgstr "um"
 
-#: src/humanize/number.py:248
+#: src/humanize/number.py:303
 msgid "two"
-msgstr "due"
+msgstr "dois"
 
-#: src/humanize/number.py:249
+#: src/humanize/number.py:304
 msgid "three"
-msgstr "tre"
+msgstr "três"
 
-#: src/humanize/number.py:250
+#: src/humanize/number.py:305
 msgid "four"
-msgstr "quattro"
+msgstr "quatro"
 
-#: src/humanize/number.py:251
+#: src/humanize/number.py:306
 msgid "five"
-msgstr "cinque"
+msgstr "cinco"
 
-#: src/humanize/number.py:252
+#: src/humanize/number.py:307
 msgid "six"
-msgstr "sei"
+msgstr "seis"
 
-#: src/humanize/number.py:253
+#: src/humanize/number.py:308
 msgid "seven"
-msgstr "sette"
+msgstr "sete"
 
-#: src/humanize/number.py:254
+#: src/humanize/number.py:309
 msgid "eight"
-msgstr "otto"
+msgstr "oito"
 
-#: src/humanize/number.py:255
+#: src/humanize/number.py:310
 msgid "nine"
 msgstr "nove"
 
-#: src/humanize/time.py:133
-#, fuzzy, python-format
+#: src/humanize/time.py:152
+#, python-format
 msgid "%d microsecond"
 msgid_plural "%d microseconds"
-msgstr[0] "%d microsecondo"
-msgstr[1] "%d microsecondi"
+msgstr[0] "%d microssegundo"
+msgstr[1] "%d microssegundos"
 
-#: src/humanize/time.py:142
-#, fuzzy, python-format
+#: src/humanize/time.py:161
+#, python-format
 msgid "%d millisecond"
 msgid_plural "%d milliseconds"
-msgstr[0] "%d millisecondo"
-msgstr[1] "%d millisecondi"
+msgstr[0] "%d milissegundo"
+msgstr[1] "%d milissegundos"
 
-#: src/humanize/time.py:145 src/humanize/time.py:220
+#: src/humanize/time.py:164 src/humanize/time.py:259
 msgid "a moment"
-msgstr "un momento"
+msgstr "um momento"
 
-#: src/humanize/time.py:147
+#: src/humanize/time.py:167
 msgid "a second"
-msgstr "un secondo"
+msgstr "um segundo"
 
-#: src/humanize/time.py:149
+#: src/humanize/time.py:170
 #, python-format
 msgid "%d second"
 msgid_plural "%d seconds"
-msgstr[0] "%d secondo"
-msgstr[1] "%d secondi"
+msgstr[0] "%d segundo"
+msgstr[1] "%d segundos"
 
-#: src/humanize/time.py:151
+#: src/humanize/time.py:173
 msgid "a minute"
-msgstr "un minuto"
+msgstr "um minuto"
 
-#: src/humanize/time.py:154
+#: src/humanize/time.py:177
 #, python-format
 msgid "%d minute"
 msgid_plural "%d minutes"
 msgstr[0] "%d minuto"
-msgstr[1] "%d minuti"
+msgstr[1] "%d minutos"
 
-#: src/humanize/time.py:156
+#: src/humanize/time.py:180
 msgid "an hour"
-msgstr "un'ora"
+msgstr "uma hora"
 
-#: src/humanize/time.py:159
+#: src/humanize/time.py:184
 #, python-format
 msgid "%d hour"
 msgid_plural "%d hours"
-msgstr[0] "%d ora"
-msgstr[1] "%d ore"
+msgstr[0] "%d hora"
+msgstr[1] "%d horas"
 
-#: src/humanize/time.py:162
+#: src/humanize/time.py:188
 msgid "a day"
-msgstr "un giorno"
+msgstr "um dia"
 
-#: src/humanize/time.py:164 src/humanize/time.py:167
+#: src/humanize/time.py:191 src/humanize/time.py:194
 #, python-format
 msgid "%d day"
 msgid_plural "%d days"
-msgstr[0] "%d giorno"
-msgstr[1] "%d giorni"
+msgstr[0] "%d dia"
+msgstr[1] "%d dias"
 
-#: src/humanize/time.py:169
+#: src/humanize/time.py:197
 msgid "a month"
-msgstr "un mese"
+msgstr "um mês"
 
-#: src/humanize/time.py:171
+#: src/humanize/time.py:199
 #, python-format
 msgid "%d month"
 msgid_plural "%d months"
-msgstr[0] "%d mese"
-msgstr[1] "%d mesi"
+msgstr[0] "%d mês"
+msgstr[1] "%d meses"
 
-#: src/humanize/time.py:174
+#: src/humanize/time.py:203
 msgid "a year"
-msgstr "un anno"
+msgstr "um ano"
 
-#: src/humanize/time.py:176 src/humanize/time.py:185
+#: src/humanize/time.py:206 src/humanize/time.py:217
 #, python-format
 msgid "1 year, %d day"
 msgid_plural "1 year, %d days"
-msgstr[0] "un anno e %d giorno"
-msgstr[1] "un anno e %d giorni"
+msgstr[0] "1 ano e %d dia"
+msgstr[1] "1 ano e %d dias"
 
-#: src/humanize/time.py:179
+#: src/humanize/time.py:210
 msgid "1 year, 1 month"
-msgstr "un anno ed un mese"
+msgstr "1 ano e 1 mês"
 
-#: src/humanize/time.py:182
+#: src/humanize/time.py:213
 #, python-format
 msgid "1 year, %d month"
 msgid_plural "1 year, %d months"
-msgstr[0] "un anno e %d mese"
-msgstr[1] "un anno e %d mesi"
+msgstr[0] "1 ano e %d mês"
+msgstr[1] "1 ano e %d meses"
 
-#: src/humanize/time.py:187
+#: src/humanize/time.py:219
 #, python-format
 msgid "%d year"
 msgid_plural "%d years"
-msgstr[0] "%d anno"
-msgstr[1] "%d anni"
+msgstr[0] "%d ano"
+msgstr[1] "%d anos"
 
-#: src/humanize/time.py:217
+#: src/humanize/time.py:256
 #, python-format
 msgid "%s from now"
-msgstr "fra %s"
+msgstr "daqui a %s"
 
-#: src/humanize/time.py:217
+#: src/humanize/time.py:256
 #, python-format
 msgid "%s ago"
-msgstr "%s fa"
+msgstr "há %s"
 
-#: src/humanize/time.py:221
+#: src/humanize/time.py:260
 msgid "now"
-msgstr "adesso"
+msgstr "agora"
 
-#: src/humanize/time.py:244
+#: src/humanize/time.py:284
 msgid "today"
-msgstr "oggi"
+msgstr "hoje"
 
-#: src/humanize/time.py:246
+#: src/humanize/time.py:287
 msgid "tomorrow"
-msgstr "domani"
+msgstr "amanhã"
 
-#: src/humanize/time.py:248
+#: src/humanize/time.py:290
 msgid "yesterday"
-msgstr "ieri"
+msgstr "ontem"
 
-#: src/humanize/time.py:534
+#: src/humanize/time.py:600
 #, python-format
 msgid "%s and %s"
-msgstr ""
+msgstr "%s e %s"
```

### Comparing `humanize-4.5.0/src/humanize/locale/ja_JP/LC_MESSAGES/humanize.mo` & `humanize-4.6.0/src/humanize/locale/ja_JP/LC_MESSAGES/humanize.mo`

 * *Files identical despite different names*

### Comparing `humanize-4.5.0/src/humanize/locale/ja_JP/LC_MESSAGES/humanize.po` & `humanize-4.6.0/src/humanize/locale/ja_JP/LC_MESSAGES/humanize.po`

 * *Files 6% similar despite different names*

```diff
@@ -3,352 +3,352 @@
 # This file is distributed under the same license as the humanize project.
 # @qoolloop, 2018.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: humanize\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2021-05-04 23:15+0200\n"
+"POT-Creation-Date: 2023-01-08 19:22+0200\n"
 "PO-Revision-Date: 2018-01-22 10:48+0900\n"
 "Last-Translator: Kan Torii <oss@qoolloop.com>\n"
 "Language-Team: Japanese\n"
 "Language: ja\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 "Generated-By: Babel 0.9.6\n"
 "X-Generator: Poedit 2.0.6\n"
 
-#: src/humanize/number.py:57
+#: src/humanize/number.py:84
 msgctxt "0 (male)"
 msgid "th"
 msgstr "番目"
 
-#: src/humanize/number.py:58
+#: src/humanize/number.py:85
 msgctxt "1 (male)"
 msgid "st"
 msgstr "番目"
 
-#: src/humanize/number.py:59
+#: src/humanize/number.py:86
 msgctxt "2 (male)"
 msgid "nd"
 msgstr "番目"
 
-#: src/humanize/number.py:60
+#: src/humanize/number.py:87
 msgctxt "3 (male)"
 msgid "rd"
 msgstr "番目"
 
-#: src/humanize/number.py:61
+#: src/humanize/number.py:88
 msgctxt "4 (male)"
 msgid "th"
 msgstr "番目"
 
-#: src/humanize/number.py:62
+#: src/humanize/number.py:89
 msgctxt "5 (male)"
 msgid "th"
 msgstr "番目"
 
-#: src/humanize/number.py:63
+#: src/humanize/number.py:90
 msgctxt "6 (male)"
 msgid "th"
 msgstr "番目"
 
-#: src/humanize/number.py:64
+#: src/humanize/number.py:91
 msgctxt "7 (male)"
 msgid "th"
 msgstr "番目"
 
-#: src/humanize/number.py:65
+#: src/humanize/number.py:92
 msgctxt "8 (male)"
 msgid "th"
 msgstr "番目"
 
-#: src/humanize/number.py:66
+#: src/humanize/number.py:93
 msgctxt "9 (male)"
 msgid "th"
 msgstr "番目"
 
-#: src/humanize/number.py:70
+#: src/humanize/number.py:97
 msgctxt "0 (female)"
 msgid "th"
 msgstr "番目"
 
-#: src/humanize/number.py:71
+#: src/humanize/number.py:98
 msgctxt "1 (female)"
 msgid "st"
 msgstr "番目"
 
-#: src/humanize/number.py:72
+#: src/humanize/number.py:99
 msgctxt "2 (female)"
 msgid "nd"
 msgstr "番目"
 
-#: src/humanize/number.py:73
+#: src/humanize/number.py:100
 msgctxt "3 (female)"
 msgid "rd"
 msgstr "番目"
 
-#: src/humanize/number.py:74
+#: src/humanize/number.py:101
 msgctxt "4 (female)"
 msgid "th"
 msgstr "番目"
 
-#: src/humanize/number.py:75
+#: src/humanize/number.py:102
 msgctxt "5 (female)"
 msgid "th"
 msgstr "番目"
 
-#: src/humanize/number.py:76
+#: src/humanize/number.py:103
 msgctxt "6 (female)"
 msgid "th"
 msgstr "番目"
 
-#: src/humanize/number.py:77
+#: src/humanize/number.py:104
 msgctxt "7 (female)"
 msgid "th"
 msgstr "番目"
 
-#: src/humanize/number.py:78
+#: src/humanize/number.py:105
 msgctxt "8 (female)"
 msgid "th"
 msgstr "番目"
 
-#: src/humanize/number.py:79
+#: src/humanize/number.py:106
 msgctxt "9 (female)"
 msgid "th"
 msgstr "番目"
 
-#: src/humanize/number.py:140
+#: src/humanize/number.py:178
 msgid "thousand"
 msgid_plural "thousand"
 msgstr[0] ""
 
-#: src/humanize/number.py:141
+#: src/humanize/number.py:179
 msgid "million"
 msgid_plural "million"
 msgstr[0] "百万"
 
-#: src/humanize/number.py:142
+#: src/humanize/number.py:180
 #, fuzzy
 msgid "billion"
 msgid_plural "billion"
 msgstr[0] "十億"
 
-#: src/humanize/number.py:143
+#: src/humanize/number.py:181
 msgid "trillion"
 msgid_plural "trillion"
 msgstr[0] "兆"
 
-#: src/humanize/number.py:144
+#: src/humanize/number.py:182
 #, fuzzy
 msgid "quadrillion"
 msgid_plural "quadrillion"
 msgstr[0] "千兆"
 
-#: src/humanize/number.py:145
+#: src/humanize/number.py:183
 #, fuzzy
 msgid "quintillion"
 msgid_plural "quintillion"
 msgstr[0] "百京"
 
-#: src/humanize/number.py:146
+#: src/humanize/number.py:184
 #, fuzzy
 msgid "sextillion"
 msgid_plural "sextillion"
 msgstr[0] "十垓"
 
-#: src/humanize/number.py:147
+#: src/humanize/number.py:185
 #, fuzzy
 msgid "septillion"
 msgid_plural "septillion"
 msgstr[0] "じょ"
 
-#: src/humanize/number.py:148
+#: src/humanize/number.py:186
 #, fuzzy
 msgid "octillion"
 msgid_plural "octillion"
 msgstr[0] "千じょ"
 
-#: src/humanize/number.py:149
+#: src/humanize/number.py:187
 #, fuzzy
 msgid "nonillion"
 msgid_plural "nonillion"
 msgstr[0] "百穣"
 
-#: src/humanize/number.py:150
+#: src/humanize/number.py:188
 #, fuzzy
 msgid "decillion"
 msgid_plural "decillion"
 msgstr[0] "十溝"
 
-#: src/humanize/number.py:151
+#: src/humanize/number.py:189
 #, fuzzy
 msgid "googol"
 msgid_plural "googol"
 msgstr[0] "溝無量大数"
 
-#: src/humanize/number.py:246
+#: src/humanize/number.py:301
 msgid "zero"
 msgstr ""
 
-#: src/humanize/number.py:247
+#: src/humanize/number.py:302
 msgid "one"
 msgstr "一"
 
-#: src/humanize/number.py:248
+#: src/humanize/number.py:303
 msgid "two"
 msgstr "二"
 
-#: src/humanize/number.py:249
+#: src/humanize/number.py:304
 msgid "three"
 msgstr "三"
 
-#: src/humanize/number.py:250
+#: src/humanize/number.py:305
 msgid "four"
 msgstr "四"
 
-#: src/humanize/number.py:251
+#: src/humanize/number.py:306
 msgid "five"
 msgstr "五"
 
-#: src/humanize/number.py:252
+#: src/humanize/number.py:307
 msgid "six"
 msgstr "六"
 
-#: src/humanize/number.py:253
+#: src/humanize/number.py:308
 msgid "seven"
 msgstr "七"
 
-#: src/humanize/number.py:254
+#: src/humanize/number.py:309
 msgid "eight"
 msgstr "八"
 
-#: src/humanize/number.py:255
+#: src/humanize/number.py:310
 msgid "nine"
 msgstr "九"
 
-#: src/humanize/time.py:133
+#: src/humanize/time.py:152
 #, python-format
 msgid "%d microsecond"
 msgid_plural "%d microseconds"
 msgstr[0] ""
 
-#: src/humanize/time.py:142
+#: src/humanize/time.py:161
 #, python-format
 msgid "%d millisecond"
 msgid_plural "%d milliseconds"
 msgstr[0] ""
 
-#: src/humanize/time.py:145 src/humanize/time.py:220
+#: src/humanize/time.py:164 src/humanize/time.py:259
 #, fuzzy
 msgid "a moment"
 msgstr "短時間"
 
-#: src/humanize/time.py:147
+#: src/humanize/time.py:167
 msgid "a second"
 msgstr "1秒"
 
-#: src/humanize/time.py:149
+#: src/humanize/time.py:170
 #, python-format
 msgid "%d second"
 msgid_plural "%d seconds"
 msgstr[0] "%d秒"
 
-#: src/humanize/time.py:151
+#: src/humanize/time.py:173
 msgid "a minute"
 msgstr "1分"
 
-#: src/humanize/time.py:154
+#: src/humanize/time.py:177
 #, python-format
 msgid "%d minute"
 msgid_plural "%d minutes"
 msgstr[0] "%d分"
 
-#: src/humanize/time.py:156
+#: src/humanize/time.py:180
 msgid "an hour"
 msgstr "1時間"
 
-#: src/humanize/time.py:159
+#: src/humanize/time.py:184
 #, python-format
 msgid "%d hour"
 msgid_plural "%d hours"
 msgstr[0] "%d時間"
 
-#: src/humanize/time.py:162
+#: src/humanize/time.py:188
 msgid "a day"
 msgstr "1日"
 
-#: src/humanize/time.py:164 src/humanize/time.py:167
+#: src/humanize/time.py:191 src/humanize/time.py:194
 #, python-format
 msgid "%d day"
 msgid_plural "%d days"
 msgstr[0] "%d日"
 
-#: src/humanize/time.py:169
+#: src/humanize/time.py:197
 msgid "a month"
 msgstr "1ヶ月"
 
-#: src/humanize/time.py:171
+#: src/humanize/time.py:199
 #, python-format
 msgid "%d month"
 msgid_plural "%d months"
 msgstr[0] "%dヶ月"
 
-#: src/humanize/time.py:174
+#: src/humanize/time.py:203
 msgid "a year"
 msgstr "1年"
 
-#: src/humanize/time.py:176 src/humanize/time.py:185
+#: src/humanize/time.py:206 src/humanize/time.py:217
 #, python-format
 msgid "1 year, %d day"
 msgid_plural "1 year, %d days"
 msgstr[0] "1年 %d日"
 
-#: src/humanize/time.py:179
+#: src/humanize/time.py:210
 msgid "1 year, 1 month"
 msgstr "1年 1ヶ月"
 
-#: src/humanize/time.py:182
+#: src/humanize/time.py:213
 #, python-format
 msgid "1 year, %d month"
 msgid_plural "1 year, %d months"
 msgstr[0] "1年 %dヶ月"
 
-#: src/humanize/time.py:187
+#: src/humanize/time.py:219
 #, python-format
 msgid "%d year"
 msgid_plural "%d years"
 msgstr[0] "%d年"
 
-#: src/humanize/time.py:217
+#: src/humanize/time.py:256
 #, python-format
 msgid "%s from now"
 msgstr "%s後"
 
-#: src/humanize/time.py:217
+#: src/humanize/time.py:256
 #, python-format
 msgid "%s ago"
 msgstr "%s前"
 
-#: src/humanize/time.py:221
+#: src/humanize/time.py:260
 #, fuzzy
 msgid "now"
 msgstr "今"
 
-#: src/humanize/time.py:244
+#: src/humanize/time.py:284
 msgid "today"
 msgstr "本日"
 
-#: src/humanize/time.py:246
+#: src/humanize/time.py:287
 msgid "tomorrow"
 msgstr "明日"
 
-#: src/humanize/time.py:248
+#: src/humanize/time.py:290
 msgid "yesterday"
 msgstr "昨日"
 
-#: src/humanize/time.py:534
+#: src/humanize/time.py:600
 #, python-format
 msgid "%s and %s"
 msgstr ""
```

### Comparing `humanize-4.5.0/src/humanize/locale/ko_KR/LC_MESSAGES/humanize.mo` & `humanize-4.6.0/src/humanize/locale/ko_KR/LC_MESSAGES/humanize.mo`

 * *Files identical despite different names*

### Comparing `humanize-4.5.0/src/humanize/locale/ko_KR/LC_MESSAGES/humanize.po` & `humanize-4.6.0/src/humanize/locale/zh_HK/LC_MESSAGES/humanize.po`

 * *Files 9% similar despite different names*

```diff
@@ -1,394 +1,365 @@
-# Korean (Korea) translations for humanize.
-# Copyright (C) 2013
-# This file is distributed under the same license as the humanize project.
-# @youngrok, 2013.
+# Traditional Chinese (China) translation for the project
+# Copyright (C) 2021
+# This file is distributed under the same license as the PACKAGE package.
+# AZLisme <helloazl@icloud.com>, 2016.
+# Liwen SUN <sunliwen@gmail.com>, 2019.
+# Edward Ho <edward@edward.is>, 2021.
 #
 msgid ""
 msgstr ""
-"Project-Id-Version: PROJECT VERSION\n"
+"Project-Id-Version: 1.0\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2021-05-04 23:15+0200\n"
-"PO-Revision-Date: 2013-07-10 11:38+0900\n"
-"Last-Translator: @youngrok\n"
-"Language-Team: ko_KR <LL@li.org>\n"
-"Language: ko\n"
+"POT-Creation-Date: 2023-01-08 19:22+0200\n"
+"PO-Revision-Date: 2016-11-14 23:02+0000\n"
+"Last-Translator: Edward Ho <edward@edward.is>\n"
+"Language-Team: Chinese (traditional)\n"
+"Language: zh_HK\n"
 "MIME-Version: 1.0\n"
-"Content-Type: text/plain; charset=utf-8\n"
+"Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n > 1);\n"
-"Generated-By: Babel 0.9.6\n"
-"X-Generator: Poedit 1.5.7\n"
 
-#: src/humanize/number.py:57
-#, fuzzy
+#: src/humanize/number.py:84
 msgctxt "0 (male)"
 msgid "th"
-msgstr "번째"
+msgstr "第"
 
-#: src/humanize/number.py:58
-#, fuzzy
+#: src/humanize/number.py:85
 msgctxt "1 (male)"
 msgid "st"
-msgstr "번째"
+msgstr "第"
 
-#: src/humanize/number.py:59
-#, fuzzy
+#: src/humanize/number.py:86
 msgctxt "2 (male)"
 msgid "nd"
-msgstr "번째"
+msgstr "第"
 
-#: src/humanize/number.py:60
-#, fuzzy
+#: src/humanize/number.py:87
 msgctxt "3 (male)"
 msgid "rd"
-msgstr "번째"
+msgstr "第"
 
-#: src/humanize/number.py:61
-#, fuzzy
+#: src/humanize/number.py:88
 msgctxt "4 (male)"
 msgid "th"
-msgstr "번째"
+msgstr "第"
 
-#: src/humanize/number.py:62
-#, fuzzy
+#: src/humanize/number.py:89
 msgctxt "5 (male)"
 msgid "th"
-msgstr "번째"
+msgstr "第"
 
-#: src/humanize/number.py:63
-#, fuzzy
+#: src/humanize/number.py:90
 msgctxt "6 (male)"
 msgid "th"
-msgstr "번째"
+msgstr "第"
 
-#: src/humanize/number.py:64
-#, fuzzy
+#: src/humanize/number.py:91
 msgctxt "7 (male)"
 msgid "th"
-msgstr "번째"
+msgstr "第"
 
-#: src/humanize/number.py:65
-#, fuzzy
+#: src/humanize/number.py:92
 msgctxt "8 (male)"
 msgid "th"
-msgstr "번째"
+msgstr "第"
 
-#: src/humanize/number.py:66
-#, fuzzy
+#: src/humanize/number.py:93
 msgctxt "9 (male)"
 msgid "th"
-msgstr "번째"
+msgstr "第"
 
-#: src/humanize/number.py:70
-#, fuzzy
+#: src/humanize/number.py:97
 msgctxt "0 (female)"
 msgid "th"
-msgstr "번째"
+msgstr "第"
 
-#: src/humanize/number.py:71
-#, fuzzy
+#: src/humanize/number.py:98
 msgctxt "1 (female)"
 msgid "st"
-msgstr "번째"
+msgstr "第"
 
-#: src/humanize/number.py:72
-#, fuzzy
+#: src/humanize/number.py:99
 msgctxt "2 (female)"
 msgid "nd"
-msgstr "번째"
+msgstr "第"
 
-#: src/humanize/number.py:73
-#, fuzzy
+#: src/humanize/number.py:100
 msgctxt "3 (female)"
 msgid "rd"
-msgstr "번째"
+msgstr "第"
 
-#: src/humanize/number.py:74
-#, fuzzy
+#: src/humanize/number.py:101
 msgctxt "4 (female)"
 msgid "th"
-msgstr "번째"
+msgstr "第"
 
-#: src/humanize/number.py:75
-#, fuzzy
+#: src/humanize/number.py:102
 msgctxt "5 (female)"
 msgid "th"
-msgstr "번째"
+msgstr "第"
 
-#: src/humanize/number.py:76
-#, fuzzy
+#: src/humanize/number.py:103
 msgctxt "6 (female)"
 msgid "th"
-msgstr "번째"
+msgstr "第"
 
-#: src/humanize/number.py:77
-#, fuzzy
+#: src/humanize/number.py:104
 msgctxt "7 (female)"
 msgid "th"
-msgstr "번째"
+msgstr "第"
 
-#: src/humanize/number.py:78
-#, fuzzy
+#: src/humanize/number.py:105
 msgctxt "8 (female)"
 msgid "th"
-msgstr "번째"
+msgstr "第"
 
-#: src/humanize/number.py:79
-#, fuzzy
+#: src/humanize/number.py:106
 msgctxt "9 (female)"
 msgid "th"
-msgstr "번째"
+msgstr "第"
 
-#: src/humanize/number.py:140
+#: src/humanize/number.py:178
 msgid "thousand"
 msgid_plural "thousand"
-msgstr[0] ""
-msgstr[1] ""
+msgstr[0] "千"
+msgstr[1] "千"
 
-#: src/humanize/number.py:141
+#: src/humanize/number.py:179
 msgid "million"
 msgid_plural "million"
-msgstr[0] "%(value)s million"
-msgstr[1] "%(value)s million"
+msgstr[0] "百萬"
+msgstr[1] "百萬"
 
-#: src/humanize/number.py:142
+#: src/humanize/number.py:180
 msgid "billion"
 msgid_plural "billion"
-msgstr[0] "milliard"
-msgstr[1] "milliard"
+msgstr[0] "十億"
+msgstr[1] "十億"
 
-#: src/humanize/number.py:143
-#, fuzzy
+#: src/humanize/number.py:181
 msgid "trillion"
 msgid_plural "trillion"
-msgstr[0] "%(value)s billion"
-msgstr[1] "%(value)s billion"
+msgstr[0] "兆"
+msgstr[1] "兆"
 
-#: src/humanize/number.py:144
-#, fuzzy
+#: src/humanize/number.py:182
 msgid "quadrillion"
 msgid_plural "quadrillion"
-msgstr[0] "%(value)s quadrillion"
-msgstr[1] "%(value)s quadrillion"
+msgstr[0] "萬億"
+msgstr[1] "萬億"
 
-#: src/humanize/number.py:145
-#, fuzzy
+#: src/humanize/number.py:183
 msgid "quintillion"
 msgid_plural "quintillion"
-msgstr[0] "%(value)s quintillion"
-msgstr[1] "%(value)s quintillion"
+msgstr[0] "百京"
+msgstr[1] "百京"
 
-#: src/humanize/number.py:146
-#, fuzzy
+#: src/humanize/number.py:184
 msgid "sextillion"
 msgid_plural "sextillion"
-msgstr[0] "%(value)s sextillion"
-msgstr[1] "%(value)s sextillion"
+msgstr[0] "十垓"
+msgstr[1] "十垓"
 
-#: src/humanize/number.py:147
-#, fuzzy
+#: src/humanize/number.py:185
 msgid "septillion"
 msgid_plural "septillion"
-msgstr[0] "%(value)s septillion"
-msgstr[1] "%(value)s septillion"
+msgstr[0] "秭"
+msgstr[1] "秭"
 
-#: src/humanize/number.py:148
-#, fuzzy
+#: src/humanize/number.py:186
 msgid "octillion"
 msgid_plural "octillion"
-msgstr[0] "%(value)s octillion"
-msgstr[1] "%(value)s octillion"
+msgstr[0] "千秭"
+msgstr[1] "千秭"
 
-#: src/humanize/number.py:149
-#, fuzzy
+#: src/humanize/number.py:187
 msgid "nonillion"
 msgid_plural "nonillion"
-msgstr[0] "%(value)s nonillion"
-msgstr[1] "%(value)s nonillion"
+msgstr[0] "百穰"
+msgstr[1] "百穰"
 
-#: src/humanize/number.py:150
-#, fuzzy
+#: src/humanize/number.py:188
 msgid "decillion"
 msgid_plural "decillion"
-msgstr[0] "%(value)s décillion"
-msgstr[1] "%(value)s décillion"
+msgstr[0] "十溝"
+msgstr[1] "十溝"
 
-#: src/humanize/number.py:151
-#, fuzzy
+#: src/humanize/number.py:189
 msgid "googol"
 msgid_plural "googol"
-msgstr[0] "%(value)s gogol"
-msgstr[1] "%(value)s gogol"
+msgstr[0] "古高爾"
+msgstr[1] "古高爾"
 
-#: src/humanize/number.py:246
+#: src/humanize/number.py:301
 msgid "zero"
-msgstr ""
+msgstr "零"
 
-#: src/humanize/number.py:247
+#: src/humanize/number.py:302
 msgid "one"
-msgstr "하나"
+msgstr "一"
 
-#: src/humanize/number.py:248
+#: src/humanize/number.py:303
 msgid "two"
-msgstr "둘"
+msgstr "二"
 
-#: src/humanize/number.py:249
+#: src/humanize/number.py:304
 msgid "three"
-msgstr "셋"
+msgstr "三"
 
-#: src/humanize/number.py:250
+#: src/humanize/number.py:305
 msgid "four"
-msgstr "넷"
+msgstr "四"
 
-#: src/humanize/number.py:251
+#: src/humanize/number.py:306
 msgid "five"
-msgstr "다섯"
+msgstr "五"
 
-#: src/humanize/number.py:252
+#: src/humanize/number.py:307
 msgid "six"
-msgstr "여섯"
+msgstr "六"
 
-#: src/humanize/number.py:253
+#: src/humanize/number.py:308
 msgid "seven"
-msgstr "일곱"
+msgstr "七"
 
-#: src/humanize/number.py:254
+#: src/humanize/number.py:309
 msgid "eight"
-msgstr "여덟"
+msgstr "八"
 
-#: src/humanize/number.py:255
+#: src/humanize/number.py:310
 msgid "nine"
-msgstr "아홉"
+msgstr "九"
 
-#: src/humanize/time.py:133
+#: src/humanize/time.py:152
 #, python-format
 msgid "%d microsecond"
 msgid_plural "%d microseconds"
-msgstr[0] "%d마이크로초"
-msgstr[1] "%d마이크로초"
+msgstr[0] "%d 微秒"
+msgstr[1] "%d 微秒"
 
-#: src/humanize/time.py:142
+#: src/humanize/time.py:161
 #, python-format
 msgid "%d millisecond"
 msgid_plural "%d milliseconds"
-msgstr[0] "%d밀리초"
-msgstr[1] "%d밀리초"
+msgstr[0] "%d 毫秒"
+msgstr[1] "%d 毫秒"
 
-#: src/humanize/time.py:145 src/humanize/time.py:220
+#: src/humanize/time.py:164 src/humanize/time.py:259
 msgid "a moment"
-msgstr "잠깐"
+msgstr "一會"
 
-#: src/humanize/time.py:147
+#: src/humanize/time.py:167
 msgid "a second"
-msgstr "1초"
+msgstr "1 秒"
 
-#: src/humanize/time.py:149
+#: src/humanize/time.py:170
 #, python-format
 msgid "%d second"
 msgid_plural "%d seconds"
-msgstr[0] "%d초"
-msgstr[1] "%d초"
+msgstr[0] "%d 秒"
+msgstr[1] "%d 秒"
 
-#: src/humanize/time.py:151
+#: src/humanize/time.py:173
 msgid "a minute"
-msgstr "1분"
+msgstr "1 分鐘"
 
-#: src/humanize/time.py:154
+#: src/humanize/time.py:177
 #, python-format
 msgid "%d minute"
 msgid_plural "%d minutes"
-msgstr[0] "%d분"
-msgstr[1] "%d분"
+msgstr[0] "%d 分鐘"
+msgstr[1] "%d 分鐘"
 
-#: src/humanize/time.py:156
+#: src/humanize/time.py:180
 msgid "an hour"
-msgstr "1시간"
+msgstr "1 小時"
 
-#: src/humanize/time.py:159
+#: src/humanize/time.py:184
 #, python-format
 msgid "%d hour"
 msgid_plural "%d hours"
-msgstr[0] "%d시간"
-msgstr[1] "%d시간"
+msgstr[0] "%d 小時"
+msgstr[1] "%d 小時"
 
-#: src/humanize/time.py:162
+#: src/humanize/time.py:188
 msgid "a day"
-msgstr "하루"
+msgstr "1 天"
 
-#: src/humanize/time.py:164 src/humanize/time.py:167
+#: src/humanize/time.py:191 src/humanize/time.py:194
 #, python-format
 msgid "%d day"
 msgid_plural "%d days"
-msgstr[0] "%d일"
-msgstr[1] "%d일"
+msgstr[0] "%d 天"
+msgstr[1] "%d 天"
 
-#: src/humanize/time.py:169
+#: src/humanize/time.py:197
 msgid "a month"
-msgstr "1개월"
+msgstr "1 月"
 
-#: src/humanize/time.py:171
+#: src/humanize/time.py:199
 #, python-format
 msgid "%d month"
 msgid_plural "%d months"
-msgstr[0] "%d개월"
-msgstr[1] "%d개월"
+msgstr[0] "%d 月"
+msgstr[1] "%d 月"
 
-#: src/humanize/time.py:174
+#: src/humanize/time.py:203
 msgid "a year"
-msgstr "1년"
+msgstr "1 年"
 
-#: src/humanize/time.py:176 src/humanize/time.py:185
+#: src/humanize/time.py:206 src/humanize/time.py:217
 #, python-format
 msgid "1 year, %d day"
 msgid_plural "1 year, %d days"
-msgstr[0] "1년, %d일"
-msgstr[1] "1년, %d일"
+msgstr[0] "%d 年"
+msgstr[1] "%d 年"
 
-#: src/humanize/time.py:179
+#: src/humanize/time.py:210
 msgid "1 year, 1 month"
-msgstr "1년, 1개월"
+msgstr "1 年又 1 個月"
 
-#: src/humanize/time.py:182
+#: src/humanize/time.py:213
 #, python-format
 msgid "1 year, %d month"
 msgid_plural "1 year, %d months"
-msgstr[0] "1년, %d개월"
-msgstr[1] "1년, %d개월"
+msgstr[0] "1 年又 %d 個月"
+msgstr[1] "1 年又 %d 個月"
 
-#: src/humanize/time.py:187
+#: src/humanize/time.py:219
 #, python-format
 msgid "%d year"
 msgid_plural "%d years"
-msgstr[0] "%d년"
-msgstr[1] "%d년"
+msgstr[0] "%d年"
+msgstr[1] "%d年"
 
-#: src/humanize/time.py:217
+#: src/humanize/time.py:256
 #, python-format
 msgid "%s from now"
-msgstr "%s 후"
+msgstr "%s 之後"
 
-#: src/humanize/time.py:217
+#: src/humanize/time.py:256
 #, python-format
 msgid "%s ago"
-msgstr "%s 전"
+msgstr "%s 之前"
 
-#: src/humanize/time.py:221
+#: src/humanize/time.py:260
 msgid "now"
-msgstr "방금"
+msgstr "現在"
 
-#: src/humanize/time.py:244
+#: src/humanize/time.py:284
 msgid "today"
-msgstr "오늘"
+msgstr "今天"
 
-#: src/humanize/time.py:246
+#: src/humanize/time.py:287
 msgid "tomorrow"
-msgstr "내일"
+msgstr "明天"
 
-#: src/humanize/time.py:248
+#: src/humanize/time.py:290
 msgid "yesterday"
-msgstr "어제"
+msgstr "昨天"
 
-#: src/humanize/time.py:534
+#: src/humanize/time.py:600
 #, python-format
 msgid "%s and %s"
-msgstr ""
+msgstr "%s 與 %s"
```

### Comparing `humanize-4.5.0/src/humanize/locale/nl_NL/LC_MESSAGES/humanize.mo` & `humanize-4.6.0/src/humanize/locale/nl_NL/LC_MESSAGES/humanize.mo`

 * *Files identical despite different names*

### Comparing `humanize-4.5.0/src/humanize/locale/nl_NL/LC_MESSAGES/humanize.po` & `humanize-4.6.0/src/humanize/locale/nl_NL/LC_MESSAGES/humanize.po`

 * *Files 4% similar despite different names*

```diff
@@ -3,363 +3,363 @@
 # This file is distributed under the same license as the PROJECT project.
 # FIRST AUTHOR <EMAIL@ADDRESS>, 2013.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2021-05-04 23:15+0200\n"
+"POT-Creation-Date: 2023-01-08 19:22+0200\n"
 "PO-Revision-Date: 2015-03-25 21:08+0100\n"
 "Last-Translator: Martin van Wingerden\n"
 "Language-Team: nl_NL\n"
 "Language: nl_NL\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "Generated-By: Babel 0.9.6\n"
 "X-Generator: Poedit 1.7.5\n"
 
-#: src/humanize/number.py:57
+#: src/humanize/number.py:84
 msgctxt "0 (male)"
 msgid "th"
 msgstr "de"
 
-#: src/humanize/number.py:58
+#: src/humanize/number.py:85
 msgctxt "1 (male)"
 msgid "st"
 msgstr "ste"
 
-#: src/humanize/number.py:59
+#: src/humanize/number.py:86
 msgctxt "2 (male)"
 msgid "nd"
 msgstr "de"
 
-#: src/humanize/number.py:60
+#: src/humanize/number.py:87
 msgctxt "3 (male)"
 msgid "rd"
 msgstr "de"
 
-#: src/humanize/number.py:61
+#: src/humanize/number.py:88
 msgctxt "4 (male)"
 msgid "th"
 msgstr "de"
 
-#: src/humanize/number.py:62
+#: src/humanize/number.py:89
 msgctxt "5 (male)"
 msgid "th"
 msgstr "de"
 
-#: src/humanize/number.py:63
+#: src/humanize/number.py:90
 msgctxt "6 (male)"
 msgid "th"
 msgstr "de"
 
-#: src/humanize/number.py:64
+#: src/humanize/number.py:91
 msgctxt "7 (male)"
 msgid "th"
 msgstr "de"
 
-#: src/humanize/number.py:65
+#: src/humanize/number.py:92
 msgctxt "8 (male)"
 msgid "th"
 msgstr "de"
 
-#: src/humanize/number.py:66
+#: src/humanize/number.py:93
 msgctxt "9 (male)"
 msgid "th"
 msgstr "de"
 
-#: src/humanize/number.py:70
+#: src/humanize/number.py:97
 msgctxt "0 (female)"
 msgid "th"
 msgstr "de"
 
-#: src/humanize/number.py:71
+#: src/humanize/number.py:98
 msgctxt "1 (female)"
 msgid "st"
 msgstr "ste"
 
-#: src/humanize/number.py:72
+#: src/humanize/number.py:99
 msgctxt "2 (female)"
 msgid "nd"
 msgstr "de"
 
-#: src/humanize/number.py:73
+#: src/humanize/number.py:100
 msgctxt "3 (female)"
 msgid "rd"
 msgstr "de"
 
-#: src/humanize/number.py:74
+#: src/humanize/number.py:101
 msgctxt "4 (female)"
 msgid "th"
 msgstr "de"
 
-#: src/humanize/number.py:75
+#: src/humanize/number.py:102
 msgctxt "5 (female)"
 msgid "th"
 msgstr "de"
 
-#: src/humanize/number.py:76
+#: src/humanize/number.py:103
 msgctxt "6 (female)"
 msgid "th"
 msgstr "de"
 
-#: src/humanize/number.py:77
+#: src/humanize/number.py:104
 msgctxt "7 (female)"
 msgid "th"
 msgstr "de"
 
-#: src/humanize/number.py:78
+#: src/humanize/number.py:105
 msgctxt "8 (female)"
 msgid "th"
 msgstr "de"
 
-#: src/humanize/number.py:79
+#: src/humanize/number.py:106
 msgctxt "9 (female)"
 msgid "th"
 msgstr "de"
 
-#: src/humanize/number.py:140
+#: src/humanize/number.py:178
 msgid "thousand"
 msgid_plural "thousand"
 msgstr[0] ""
 msgstr[1] ""
 
-#: src/humanize/number.py:141
+#: src/humanize/number.py:179
 msgid "million"
 msgid_plural "million"
 msgstr[0] "miljoen"
 msgstr[1] "miljoen"
 
-#: src/humanize/number.py:142
+#: src/humanize/number.py:180
 msgid "billion"
 msgid_plural "billion"
 msgstr[0] "miljard"
 msgstr[1] "miljard"
 
-#: src/humanize/number.py:143
+#: src/humanize/number.py:181
 msgid "trillion"
 msgid_plural "trillion"
 msgstr[0] "biljoen"
 msgstr[1] "biljoen"
 
-#: src/humanize/number.py:144
+#: src/humanize/number.py:182
 msgid "quadrillion"
 msgid_plural "quadrillion"
 msgstr[0] "biljard"
 msgstr[1] "biljard"
 
-#: src/humanize/number.py:145
+#: src/humanize/number.py:183
 msgid "quintillion"
 msgid_plural "quintillion"
 msgstr[0] "triljoen"
 msgstr[1] "triljoen"
 
-#: src/humanize/number.py:146
+#: src/humanize/number.py:184
 msgid "sextillion"
 msgid_plural "sextillion"
 msgstr[0] "triljard"
 msgstr[1] "triljard"
 
-#: src/humanize/number.py:147
+#: src/humanize/number.py:185
 msgid "septillion"
 msgid_plural "septillion"
 msgstr[0] "quadriljoen"
 msgstr[1] "quadriljoen"
 
-#: src/humanize/number.py:148
+#: src/humanize/number.py:186
 msgid "octillion"
 msgid_plural "octillion"
 msgstr[0] "quadriljard"
 msgstr[1] "quadriljard"
 
-#: src/humanize/number.py:149
+#: src/humanize/number.py:187
 msgid "nonillion"
 msgid_plural "nonillion"
 msgstr[0] "quintiljoen"
 msgstr[1] "quintiljoen"
 
-#: src/humanize/number.py:150
+#: src/humanize/number.py:188
 msgid "decillion"
 msgid_plural "decillion"
 msgstr[0] "quintiljard"
 msgstr[1] "quintiljard"
 
-#: src/humanize/number.py:151
+#: src/humanize/number.py:189
 msgid "googol"
 msgid_plural "googol"
 msgstr[0] "googol"
 msgstr[1] "googol"
 
-#: src/humanize/number.py:246
+#: src/humanize/number.py:301
 msgid "zero"
 msgstr "nul"
 
-#: src/humanize/number.py:247
+#: src/humanize/number.py:302
 msgid "one"
 msgstr "één"
 
-#: src/humanize/number.py:248
+#: src/humanize/number.py:303
 msgid "two"
 msgstr "twee"
 
-#: src/humanize/number.py:249
+#: src/humanize/number.py:304
 msgid "three"
 msgstr "drie"
 
-#: src/humanize/number.py:250
+#: src/humanize/number.py:305
 msgid "four"
 msgstr "vier"
 
-#: src/humanize/number.py:251
+#: src/humanize/number.py:306
 msgid "five"
 msgstr "vijf"
 
-#: src/humanize/number.py:252
+#: src/humanize/number.py:307
 msgid "six"
 msgstr "zes"
 
-#: src/humanize/number.py:253
+#: src/humanize/number.py:308
 msgid "seven"
 msgstr "zeven"
 
-#: src/humanize/number.py:254
+#: src/humanize/number.py:309
 msgid "eight"
 msgstr "acht"
 
-#: src/humanize/number.py:255
+#: src/humanize/number.py:310
 msgid "nine"
 msgstr "negen"
 
-#: src/humanize/time.py:133
+#: src/humanize/time.py:152
 #, fuzzy, python-format
 msgid "%d microsecond"
 msgid_plural "%d microseconds"
 msgstr[0] "%d microseconde"
 msgstr[1] "%d microseconden"
 
-#: src/humanize/time.py:142
+#: src/humanize/time.py:161
 #, fuzzy, python-format
 msgid "%d millisecond"
 msgid_plural "%d milliseconds"
 msgstr[0] "%d milliseconde"
 msgstr[1] "%d milliseconden"
 
-#: src/humanize/time.py:145 src/humanize/time.py:220
+#: src/humanize/time.py:164 src/humanize/time.py:259
 msgid "a moment"
 msgstr "een moment"
 
-#: src/humanize/time.py:147
+#: src/humanize/time.py:167
 msgid "a second"
 msgstr "een seconde"
 
-#: src/humanize/time.py:149
+#: src/humanize/time.py:170
 #, python-format
 msgid "%d second"
 msgid_plural "%d seconds"
 msgstr[0] "%d seconde"
 msgstr[1] "%d seconden"
 
-#: src/humanize/time.py:151
+#: src/humanize/time.py:173
 msgid "a minute"
 msgstr "een minuut"
 
-#: src/humanize/time.py:154
+#: src/humanize/time.py:177
 #, python-format
 msgid "%d minute"
 msgid_plural "%d minutes"
 msgstr[0] "%d minuut"
 msgstr[1] "%d minuten"
 
-#: src/humanize/time.py:156
+#: src/humanize/time.py:180
 msgid "an hour"
 msgstr "een uur"
 
-#: src/humanize/time.py:159
+#: src/humanize/time.py:184
 #, python-format
 msgid "%d hour"
 msgid_plural "%d hours"
 msgstr[0] "%d uur"
 msgstr[1] "%d uur"
 
-#: src/humanize/time.py:162
+#: src/humanize/time.py:188
 msgid "a day"
 msgstr "een dag"
 
-#: src/humanize/time.py:164 src/humanize/time.py:167
+#: src/humanize/time.py:191 src/humanize/time.py:194
 #, python-format
 msgid "%d day"
 msgid_plural "%d days"
 msgstr[0] "%d dag"
 msgstr[1] "%d dagen"
 
-#: src/humanize/time.py:169
+#: src/humanize/time.py:197
 msgid "a month"
 msgstr "een maand"
 
-#: src/humanize/time.py:171
+#: src/humanize/time.py:199
 #, python-format
 msgid "%d month"
 msgid_plural "%d months"
 msgstr[0] "%d maand"
 msgstr[1] "%d maanden"
 
-#: src/humanize/time.py:174
+#: src/humanize/time.py:203
 msgid "a year"
 msgstr "een jaar"
 
-#: src/humanize/time.py:176 src/humanize/time.py:185
+#: src/humanize/time.py:206 src/humanize/time.py:217
 #, python-format
 msgid "1 year, %d day"
 msgid_plural "1 year, %d days"
 msgstr[0] "1 jaar, %d dag"
 msgstr[1] "1 jaar, %d dagen"
 
-#: src/humanize/time.py:179
+#: src/humanize/time.py:210
 msgid "1 year, 1 month"
 msgstr "1 jaar, 1 maand"
 
-#: src/humanize/time.py:182
+#: src/humanize/time.py:213
 #, python-format
 msgid "1 year, %d month"
 msgid_plural "1 year, %d months"
 msgstr[0] "1 jaar, %d maand"
 msgstr[1] "1 jaar, %d maanden"
 
-#: src/humanize/time.py:187
+#: src/humanize/time.py:219
 #, python-format
 msgid "%d year"
 msgid_plural "%d years"
 msgstr[0] "%d jaar"
 msgstr[1] "%d jaar"
 
-#: src/humanize/time.py:217
+#: src/humanize/time.py:256
 #, python-format
 msgid "%s from now"
 msgstr "over %s"
 
-#: src/humanize/time.py:217
+#: src/humanize/time.py:256
 #, python-format
 msgid "%s ago"
 msgstr "%s geleden"
 
-#: src/humanize/time.py:221
+#: src/humanize/time.py:260
 msgid "now"
 msgstr "nu"
 
-#: src/humanize/time.py:244
+#: src/humanize/time.py:284
 msgid "today"
 msgstr "vandaag"
 
-#: src/humanize/time.py:246
+#: src/humanize/time.py:287
 msgid "tomorrow"
 msgstr "morgen"
 
-#: src/humanize/time.py:248
+#: src/humanize/time.py:290
 msgid "yesterday"
 msgstr "gisteren"
 
-#: src/humanize/time.py:534
+#: src/humanize/time.py:600
 #, python-format
 msgid "%s and %s"
 msgstr "%s en %s"
```

### Comparing `humanize-4.5.0/src/humanize/locale/pl_PL/LC_MESSAGES/humanize.mo` & `humanize-4.6.0/src/humanize/locale/pl_PL/LC_MESSAGES/humanize.mo`

 * *Files identical despite different names*

### Comparing `humanize-4.5.0/src/humanize/locale/pl_PL/LC_MESSAGES/humanize.po` & `humanize-4.6.0/src/humanize/locale/sk_SK/LC_MESSAGES/humanize.po`

 * *Files 6% similar despite different names*

```diff
@@ -1,388 +1,386 @@
-# Polish translations for PACKAGE package.
-# Copyright (C) 2020 THE PACKAGE'S COPYRIGHT HOLDER
+# Slovak translation of humanize
+# Copyright (C) 2016
 # This file is distributed under the same license as the PACKAGE package.
-# Bartosz Bubak <bartosz.bubak@gmail.com>, 2020.
-# Added missing strings by Krystian Postek <krystian postek eu>, 2020.
-# Replace short scale with long scale by Maciej J. Mikulski (mjmikulski), 2022.
+# Jose Riha <jose1711 gmail com>, 2016.
 #
+#, fuzzy
 msgid ""
 msgstr ""
-"Project-Id-Version: 0.0.1\n"
+"Project-Id-Version: humanize\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2021-05-04 23:15+0200\n"
-"PO-Revision-Date: 2020-04-22 10:02+0200\n"
-"Last-Translator: Bartosz Bubak <bartosz.bubak gmail com>\n"
-"Language-Team: Polish\n"
-"Language: pl\n"
+"POT-Creation-Date: 2023-01-08 19:22+0200\n"
+"PO-Revision-Date: 2020-09-29 22:43+0300\n"
+"Last-Translator: Jose Riha <jose1711 gmail com>\n"
+"Language-Team: sk <LL@li.org>\n"
+"Language: Slovak\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=3; plural=(n==1 ? 0 : n%10>=2 && n%10<=4 && (n%100<10 "
-"|| n%100>=20) ? 1 : 2);\n"
+"Plural-Forms: nplurals=3; plural=(n==1) ? 0 : (n>=2 && n<=4) ? 1 : 2;\n"
 
-#: src/humanize/number.py:57
+#: src/humanize/number.py:84
 msgctxt "0 (male)"
 msgid "th"
 msgstr "."
 
-#: src/humanize/number.py:58
+#: src/humanize/number.py:85
 msgctxt "1 (male)"
 msgid "st"
 msgstr "."
 
-#: src/humanize/number.py:59
+#: src/humanize/number.py:86
 msgctxt "2 (male)"
 msgid "nd"
 msgstr "."
 
-#: src/humanize/number.py:60
+#: src/humanize/number.py:87
 msgctxt "3 (male)"
 msgid "rd"
 msgstr "."
 
-#: src/humanize/number.py:61
+#: src/humanize/number.py:88
 msgctxt "4 (male)"
 msgid "th"
 msgstr "."
 
-#: src/humanize/number.py:62
+#: src/humanize/number.py:89
 msgctxt "5 (male)"
 msgid "th"
 msgstr "."
 
-#: src/humanize/number.py:63
+#: src/humanize/number.py:90
 msgctxt "6 (male)"
 msgid "th"
 msgstr "."
 
-#: src/humanize/number.py:64
+#: src/humanize/number.py:91
 msgctxt "7 (male)"
 msgid "th"
 msgstr "."
 
-#: src/humanize/number.py:65
+#: src/humanize/number.py:92
 msgctxt "8 (male)"
 msgid "th"
 msgstr "."
 
-#: src/humanize/number.py:66
+#: src/humanize/number.py:93
 msgctxt "9 (male)"
 msgid "th"
 msgstr "."
 
-#: src/humanize/number.py:70
+#: src/humanize/number.py:97
 msgctxt "0 (female)"
 msgid "th"
 msgstr "."
 
-#: src/humanize/number.py:71
+#: src/humanize/number.py:98
 msgctxt "1 (female)"
 msgid "st"
 msgstr "."
 
-#: src/humanize/number.py:72
+#: src/humanize/number.py:99
 msgctxt "2 (female)"
 msgid "nd"
 msgstr "."
 
-#: src/humanize/number.py:73
+#: src/humanize/number.py:100
 msgctxt "3 (female)"
 msgid "rd"
 msgstr "."
 
-#: src/humanize/number.py:74
+#: src/humanize/number.py:101
 msgctxt "4 (female)"
 msgid "th"
 msgstr "."
 
-#: src/humanize/number.py:75
+#: src/humanize/number.py:102
 msgctxt "5 (female)"
 msgid "th"
 msgstr "."
 
-#: src/humanize/number.py:76
+#: src/humanize/number.py:103
 msgctxt "6 (female)"
 msgid "th"
 msgstr "."
 
-#: src/humanize/number.py:77
+#: src/humanize/number.py:104
 msgctxt "7 (female)"
 msgid "th"
 msgstr "."
 
-#: src/humanize/number.py:78
+#: src/humanize/number.py:105
 msgctxt "8 (female)"
 msgid "th"
 msgstr "."
 
-#: src/humanize/number.py:79
+#: src/humanize/number.py:106
 msgctxt "9 (female)"
 msgid "th"
 msgstr "."
 
-#: src/humanize/number.py:140
+#: src/humanize/number.py:178
 msgid "thousand"
 msgid_plural "thousand"
-msgstr[0] "tysiąc"
-msgstr[1] "tysiąc"
-msgstr[2] "tysięcy"
+msgstr[0] ""
+msgstr[1] ""
+msgstr[2] ""
 
-#: src/humanize/number.py:141
+#: src/humanize/number.py:179
 msgid "million"
 msgid_plural "million"
-msgstr[0] "milion"
-msgstr[1] "miliony"
-msgstr[2] "milionów"
+msgstr[0] "milióna/ov"
+msgstr[1] "milióna/ov"
+msgstr[2] "milióna/ov"
 
-#: src/humanize/number.py:142
+#: src/humanize/number.py:180
 msgid "billion"
 msgid_plural "billion"
-msgstr[0] "miliard"
-msgstr[1] "miliardy"
-msgstr[2] "miliardów"
+msgstr[0] "miliardy/árd"
+msgstr[1] "miliardy/árd"
+msgstr[2] "miliardy/árd"
 
-#: src/humanize/number.py:143
+#: src/humanize/number.py:181
 msgid "trillion"
 msgid_plural "trillion"
-msgstr[0] "bilion"
-msgstr[1] "biliony"
-msgstr[2] "bilionów"
+msgstr[0] "bilióna/ov"
+msgstr[1] "bilióna/ov"
+msgstr[2] "bilióna/ov"
 
-#: src/humanize/number.py:144
+#: src/humanize/number.py:182
 msgid "quadrillion"
 msgid_plural "quadrillion"
-msgstr[0] "biliard"
-msgstr[1] "biliardy"
-msgstr[2] "biliardów"
+msgstr[0] "biliardy/árd"
+msgstr[1] "biliardy/árd"
+msgstr[2] "biliardy/árd"
 
-#: src/humanize/number.py:145
+#: src/humanize/number.py:183
 msgid "quintillion"
 msgid_plural "quintillion"
-msgstr[0] "trylion"
-msgstr[1] "tryliony"
-msgstr[2] "trylionów"
+msgstr[0] "trilióna/árd"
+msgstr[1] "trilióna/árd"
+msgstr[2] "trilióna/árd"
 
-#: src/humanize/number.py:146
+#: src/humanize/number.py:184
 msgid "sextillion"
 msgid_plural "sextillion"
-msgstr[0] "tryliard"
-msgstr[1] "tryliard"
-msgstr[2] "tryliard"
+msgstr[0] "triliardy/árd"
+msgstr[1] "triliardy/árd"
+msgstr[2] "triliardy/árd"
 
-#: src/humanize/number.py:147
+#: src/humanize/number.py:185
 msgid "septillion"
 msgid_plural "septillion"
-msgstr[0] "kwadrylion"
-msgstr[1] "kwadryliony"
-msgstr[2] "kwadrylionów"
+msgstr[0] "kvadrilióna/ov"
+msgstr[1] "kvadrilióna/ov"
+msgstr[2] "kvadrilióna/ov"
 
-#: src/humanize/number.py:148
+#: src/humanize/number.py:186
 msgid "octillion"
 msgid_plural "octillion"
-msgstr[0] "kwadryliard"
-msgstr[1] "kwadryliardy"
-msgstr[2] "kwadryliardów"
+msgstr[0] "kvadriliardy/árd"
+msgstr[1] "kvadriliardy/árd"
+msgstr[2] "kvadriliardy/árd"
 
-#: src/humanize/number.py:149
+#: src/humanize/number.py:187
 msgid "nonillion"
 msgid_plural "nonillion"
-msgstr[0] "kwintylion"
-msgstr[1] "kwintyliony"
-msgstr[2] "kwintylionów"
+msgstr[0] "kvintilióna/ov"
+msgstr[1] "kvintilióna/ov"
+msgstr[2] "kvintilióna/ov"
 
-#: src/humanize/number.py:150
+#: src/humanize/number.py:188
 msgid "decillion"
 msgid_plural "decillion"
-msgstr[0] "kwintyliard"
-msgstr[1] "kwintyliardy"
-msgstr[2] "kwintyliardów"
+msgstr[0] "kvintiliardy/árd"
+msgstr[1] "kvintiliardy/árd"
+msgstr[2] "kvintiliardy/árd"
 
-#: src/humanize/number.py:151
+#: src/humanize/number.py:189
 msgid "googol"
 msgid_plural "googol"
-msgstr[0] "googol"
-msgstr[1] "googole"
-msgstr[2] "googoli"
+msgstr[0] "googola/ov"
+msgstr[1] "googola/ov"
+msgstr[2] "googola/ov"
 
-#: src/humanize/number.py:246
+#: src/humanize/number.py:301
 msgid "zero"
-msgstr "zero"
+msgstr "nula"
 
-#: src/humanize/number.py:247
+#: src/humanize/number.py:302
 msgid "one"
-msgstr "jeden"
+msgstr "jedna"
 
-#: src/humanize/number.py:248
+#: src/humanize/number.py:303
 msgid "two"
-msgstr "dwa"
+msgstr "dve"
 
-#: src/humanize/number.py:249
+#: src/humanize/number.py:304
 msgid "three"
-msgstr "trzy"
+msgstr "tri"
 
-#: src/humanize/number.py:250
+#: src/humanize/number.py:305
 msgid "four"
-msgstr "cztery"
+msgstr "štyri"
 
-#: src/humanize/number.py:251
+#: src/humanize/number.py:306
 msgid "five"
-msgstr "pięć"
+msgstr "päť"
 
-#: src/humanize/number.py:252
+#: src/humanize/number.py:307
 msgid "six"
-msgstr "sześć"
+msgstr "šesť"
 
-#: src/humanize/number.py:253
+#: src/humanize/number.py:308
 msgid "seven"
-msgstr "siedem"
+msgstr "sedem"
 
-#: src/humanize/number.py:254
+#: src/humanize/number.py:309
 msgid "eight"
-msgstr "osiem"
+msgstr "osem"
 
-#: src/humanize/number.py:255
+#: src/humanize/number.py:310
 msgid "nine"
-msgstr "dziewięć"
+msgstr "deväť"
 
-#: src/humanize/time.py:133
-#, python-format
+#: src/humanize/time.py:152
+#, fuzzy, python-format
 msgid "%d microsecond"
 msgid_plural "%d microseconds"
-msgstr[0] "%d mikrosekunda"
+msgstr[0] "%d mikrosekundu"
 msgstr[1] "%d mikrosekundy"
-msgstr[2] "%d mikrosekund"
+msgstr[2] "%d mikrosekúnd"
 
-#: src/humanize/time.py:142
-#, python-format
+#: src/humanize/time.py:161
+#, fuzzy, python-format
 msgid "%d millisecond"
 msgid_plural "%d milliseconds"
-msgstr[0] "%d milisekunda"
+msgstr[0] "%d milisekundu"
 msgstr[1] "%d milisekundy"
-msgstr[2] "%d milisekund"
+msgstr[2] "%d milisekúnd"
 
-#: src/humanize/time.py:145 src/humanize/time.py:220
+#: src/humanize/time.py:164 src/humanize/time.py:259
 msgid "a moment"
-msgstr "chwila"
+msgstr "chvíľku"
 
-#: src/humanize/time.py:147
+#: src/humanize/time.py:167
 msgid "a second"
-msgstr "sekunda"
+msgstr "sekundu"
 
-#: src/humanize/time.py:149
+#: src/humanize/time.py:170
 #, python-format
 msgid "%d second"
 msgid_plural "%d seconds"
-msgstr[0] "%d sekunda"
+msgstr[0] "%d sekundu"
 msgstr[1] "%d sekundy"
-msgstr[2] "%d sekund"
+msgstr[2] "%d sekúnd"
 
-#: src/humanize/time.py:151
+#: src/humanize/time.py:173
 msgid "a minute"
-msgstr "minuta"
+msgstr "minútu"
 
-#: src/humanize/time.py:154
+#: src/humanize/time.py:177
 #, python-format
 msgid "%d minute"
 msgid_plural "%d minutes"
-msgstr[0] "%d minuta"
-msgstr[1] "%d minuty"
-msgstr[2] "%d minut"
+msgstr[0] "%d minútu"
+msgstr[1] "%d minúty"
+msgstr[2] "%d minút"
 
-#: src/humanize/time.py:156
+#: src/humanize/time.py:180
 msgid "an hour"
-msgstr "godzina"
+msgstr "hodinu"
 
-#: src/humanize/time.py:159
+#: src/humanize/time.py:184
 #, python-format
 msgid "%d hour"
 msgid_plural "%d hours"
-msgstr[0] "%d godzina"
-msgstr[1] "%d godziny"
-msgstr[2] "%d godzin"
+msgstr[0] "%d hodina"
+msgstr[1] "%d hodiny"
+msgstr[2] "%d hodín"
 
-#: src/humanize/time.py:162
+#: src/humanize/time.py:188
 msgid "a day"
-msgstr "dzień"
+msgstr "deň"
 
-#: src/humanize/time.py:164 src/humanize/time.py:167
+#: src/humanize/time.py:191 src/humanize/time.py:194
 #, python-format
 msgid "%d day"
 msgid_plural "%d days"
-msgstr[0] "%d dzień"
+msgstr[0] "%d deň"
 msgstr[1] "%d dni"
-msgstr[2] "%d dni"
+msgstr[2] "%d dní"
 
-#: src/humanize/time.py:169
+#: src/humanize/time.py:197
 msgid "a month"
-msgstr "miesiąc"
+msgstr "mesiac"
 
-#: src/humanize/time.py:171
+#: src/humanize/time.py:199
 #, python-format
 msgid "%d month"
 msgid_plural "%d months"
-msgstr[0] "%d miesiąc"
-msgstr[1] "%d miesiące"
-msgstr[2] "%d miesięcy"
+msgstr[0] "%d mesiac"
+msgstr[1] "%d mesiace"
+msgstr[2] "%d mesiacov"
 
-#: src/humanize/time.py:174
+#: src/humanize/time.py:203
 msgid "a year"
 msgstr "rok"
 
-#: src/humanize/time.py:176 src/humanize/time.py:185
+#: src/humanize/time.py:206 src/humanize/time.py:217
 #, python-format
 msgid "1 year, %d day"
 msgid_plural "1 year, %d days"
-msgstr[0] "1 rok, %d dzień"
+msgstr[0] "1 rok, %d deň"
 msgstr[1] "1 rok, %d dni"
-msgstr[2] "1 rok, %d dni"
+msgstr[2] "1 rok, %d dní"
 
-#: src/humanize/time.py:179
+#: src/humanize/time.py:210
 msgid "1 year, 1 month"
-msgstr "1 rok, 1 miesiąc"
+msgstr "1 rok, 1 mesiac"
 
-#: src/humanize/time.py:182
+#: src/humanize/time.py:213
 #, python-format
 msgid "1 year, %d month"
 msgid_plural "1 year, %d months"
-msgstr[0] "1 rok, %d miesiąc"
-msgstr[1] "1 rok, %d miesiące"
-msgstr[2] "1 rok, %d miesięcy"
+msgstr[0] "1 rok, %d mesiac"
+msgstr[1] "1 rok, %d mesiace"
+msgstr[2] "1 rok, %d mesiacov"
 
-#: src/humanize/time.py:187
+#: src/humanize/time.py:219
 #, python-format
 msgid "%d year"
 msgid_plural "%d years"
 msgstr[0] "%d rok"
-msgstr[1] "%d lata"
-msgstr[2] "%d lat"
+msgstr[1] "%d roky"
+msgstr[2] "%d rokov"
 
-#: src/humanize/time.py:217
+#: src/humanize/time.py:256
 #, python-format
 msgid "%s from now"
-msgstr "%s od teraz"
+msgstr "o %s"
 
-#: src/humanize/time.py:217
+#: src/humanize/time.py:256
 #, python-format
 msgid "%s ago"
-msgstr "%s temu"
+msgstr "%s naspäť"
 
-#: src/humanize/time.py:221
+#: src/humanize/time.py:260
 msgid "now"
 msgstr "teraz"
 
-#: src/humanize/time.py:244
+#: src/humanize/time.py:284
 msgid "today"
-msgstr "dziś"
+msgstr "dnes"
 
-#: src/humanize/time.py:246
+#: src/humanize/time.py:287
 msgid "tomorrow"
-msgstr "jutro"
+msgstr "zajtra"
 
-#: src/humanize/time.py:248
+#: src/humanize/time.py:290
 msgid "yesterday"
-msgstr "wczoraj"
+msgstr "včera"
 
-#: src/humanize/time.py:534
+#: src/humanize/time.py:600
 #, python-format
 msgid "%s and %s"
-msgstr "%s i %s"
+msgstr ""
```

### Comparing `humanize-4.5.0/src/humanize/locale/pt_BR/LC_MESSAGES/humanize.mo` & `humanize-4.6.0/src/humanize/locale/pt_BR/LC_MESSAGES/humanize.mo`

 * *Files identical despite different names*

### Comparing `humanize-4.5.0/src/humanize/locale/pt_BR/LC_MESSAGES/humanize.po` & `humanize-4.6.0/src/humanize/locale/ko_KR/LC_MESSAGES/humanize.po`

 * *Files 15% similar despite different names*

```diff
@@ -1,364 +1,394 @@
-# SOME DESCRIPTIVE TITLE.
-# Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
-# This file is distributed under the same license as the PACKAGE package.
-# FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
+# Korean (Korea) translations for humanize.
+# Copyright (C) 2013
+# This file is distributed under the same license as the humanize project.
+# @youngrok, 2013.
 #
 msgid ""
 msgstr ""
-"Project-Id-Version: \n"
+"Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2021-05-04 23:15+0200\n"
-"PO-Revision-Date: 2016-06-15 15:58-0300\n"
-"Last-Translator: \n"
-"Language-Team: \n"
-"Language: pt_BR\n"
+"POT-Creation-Date: 2023-01-08 19:22+0200\n"
+"PO-Revision-Date: 2013-07-10 11:38+0900\n"
+"Last-Translator: @youngrok\n"
+"Language-Team: ko_KR <LL@li.org>\n"
+"Language: ko\n"
 "MIME-Version: 1.0\n"
-"Content-Type: text/plain; charset=UTF-8\n"
+"Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n > 1);\n"
-"X-Generator: Poedit 1.8.5\n"
+"Generated-By: Babel 0.9.6\n"
+"X-Generator: Poedit 1.5.7\n"
 
-#: src/humanize/number.py:57
+#: src/humanize/number.py:84
+#, fuzzy
 msgctxt "0 (male)"
 msgid "th"
-msgstr "º"
+msgstr "번째"
 
-#: src/humanize/number.py:58
+#: src/humanize/number.py:85
+#, fuzzy
 msgctxt "1 (male)"
 msgid "st"
-msgstr "º"
+msgstr "번째"
 
-#: src/humanize/number.py:59
+#: src/humanize/number.py:86
+#, fuzzy
 msgctxt "2 (male)"
 msgid "nd"
-msgstr "º"
+msgstr "번째"
 
-#: src/humanize/number.py:60
+#: src/humanize/number.py:87
+#, fuzzy
 msgctxt "3 (male)"
 msgid "rd"
-msgstr "º"
+msgstr "번째"
 
-#: src/humanize/number.py:61
+#: src/humanize/number.py:88
+#, fuzzy
 msgctxt "4 (male)"
 msgid "th"
-msgstr "º"
+msgstr "번째"
 
-#: src/humanize/number.py:62
+#: src/humanize/number.py:89
+#, fuzzy
 msgctxt "5 (male)"
 msgid "th"
-msgstr "º"
+msgstr "번째"
 
-#: src/humanize/number.py:63
+#: src/humanize/number.py:90
+#, fuzzy
 msgctxt "6 (male)"
 msgid "th"
-msgstr "º"
+msgstr "번째"
 
-#: src/humanize/number.py:64
+#: src/humanize/number.py:91
+#, fuzzy
 msgctxt "7 (male)"
 msgid "th"
-msgstr "º"
+msgstr "번째"
 
-#: src/humanize/number.py:65
+#: src/humanize/number.py:92
+#, fuzzy
 msgctxt "8 (male)"
 msgid "th"
-msgstr "º"
+msgstr "번째"
 
-#: src/humanize/number.py:66
+#: src/humanize/number.py:93
+#, fuzzy
 msgctxt "9 (male)"
 msgid "th"
-msgstr "º"
+msgstr "번째"
 
-#: src/humanize/number.py:70
+#: src/humanize/number.py:97
+#, fuzzy
 msgctxt "0 (female)"
 msgid "th"
-msgstr "ª"
+msgstr "번째"
 
-#: src/humanize/number.py:71
+#: src/humanize/number.py:98
+#, fuzzy
 msgctxt "1 (female)"
 msgid "st"
-msgstr "ª"
+msgstr "번째"
 
-#: src/humanize/number.py:72
+#: src/humanize/number.py:99
+#, fuzzy
 msgctxt "2 (female)"
 msgid "nd"
-msgstr "ª"
+msgstr "번째"
 
-#: src/humanize/number.py:73
+#: src/humanize/number.py:100
+#, fuzzy
 msgctxt "3 (female)"
 msgid "rd"
-msgstr "ª"
+msgstr "번째"
 
-#: src/humanize/number.py:74
+#: src/humanize/number.py:101
+#, fuzzy
 msgctxt "4 (female)"
 msgid "th"
-msgstr "ª"
+msgstr "번째"
 
-#: src/humanize/number.py:75
+#: src/humanize/number.py:102
+#, fuzzy
 msgctxt "5 (female)"
 msgid "th"
-msgstr "ª"
+msgstr "번째"
 
-#: src/humanize/number.py:76
+#: src/humanize/number.py:103
+#, fuzzy
 msgctxt "6 (female)"
 msgid "th"
-msgstr "ª"
+msgstr "번째"
 
-#: src/humanize/number.py:77
+#: src/humanize/number.py:104
+#, fuzzy
 msgctxt "7 (female)"
 msgid "th"
-msgstr "ª"
+msgstr "번째"
 
-#: src/humanize/number.py:78
+#: src/humanize/number.py:105
+#, fuzzy
 msgctxt "8 (female)"
 msgid "th"
-msgstr "ª"
+msgstr "번째"
 
-#: src/humanize/number.py:79
+#: src/humanize/number.py:106
+#, fuzzy
 msgctxt "9 (female)"
 msgid "th"
-msgstr "ª"
+msgstr "번째"
 
-#: src/humanize/number.py:140
+#: src/humanize/number.py:178
 msgid "thousand"
 msgid_plural "thousand"
 msgstr[0] ""
 msgstr[1] ""
 
-#: src/humanize/number.py:141
+#: src/humanize/number.py:179
 msgid "million"
 msgid_plural "million"
-msgstr[0] "milhão"
-msgstr[1] "milhão"
+msgstr[0] "%(value)s million"
+msgstr[1] "%(value)s million"
 
-#: src/humanize/number.py:142
+#: src/humanize/number.py:180
 msgid "billion"
 msgid_plural "billion"
-msgstr[0] "bilhão"
-msgstr[1] "bilhão"
+msgstr[0] "milliard"
+msgstr[1] "milliard"
 
-#: src/humanize/number.py:143
+#: src/humanize/number.py:181
+#, fuzzy
 msgid "trillion"
 msgid_plural "trillion"
-msgstr[0] "trilhão"
-msgstr[1] "trilhão"
+msgstr[0] "%(value)s billion"
+msgstr[1] "%(value)s billion"
 
-#: src/humanize/number.py:144
+#: src/humanize/number.py:182
+#, fuzzy
 msgid "quadrillion"
 msgid_plural "quadrillion"
-msgstr[0] "quatrilhão"
-msgstr[1] "quatrilhão"
+msgstr[0] "%(value)s quadrillion"
+msgstr[1] "%(value)s quadrillion"
 
-#: src/humanize/number.py:145
+#: src/humanize/number.py:183
+#, fuzzy
 msgid "quintillion"
 msgid_plural "quintillion"
-msgstr[0] "quintilhão"
-msgstr[1] "quintilhão"
+msgstr[0] "%(value)s quintillion"
+msgstr[1] "%(value)s quintillion"
 
-#: src/humanize/number.py:146
+#: src/humanize/number.py:184
+#, fuzzy
 msgid "sextillion"
 msgid_plural "sextillion"
-msgstr[0] "sextilhão"
-msgstr[1] "sextilhão"
+msgstr[0] "%(value)s sextillion"
+msgstr[1] "%(value)s sextillion"
 
-#: src/humanize/number.py:147
+#: src/humanize/number.py:185
+#, fuzzy
 msgid "septillion"
 msgid_plural "septillion"
-msgstr[0] "septilhão"
-msgstr[1] "septilhão"
+msgstr[0] "%(value)s septillion"
+msgstr[1] "%(value)s septillion"
 
-#: src/humanize/number.py:148
+#: src/humanize/number.py:186
+#, fuzzy
 msgid "octillion"
 msgid_plural "octillion"
-msgstr[0] "octilhão"
-msgstr[1] "octilhão"
+msgstr[0] "%(value)s octillion"
+msgstr[1] "%(value)s octillion"
 
-#: src/humanize/number.py:149
+#: src/humanize/number.py:187
+#, fuzzy
 msgid "nonillion"
 msgid_plural "nonillion"
-msgstr[0] "nonilhão"
-msgstr[1] "nonilhão"
+msgstr[0] "%(value)s nonillion"
+msgstr[1] "%(value)s nonillion"
 
-#: src/humanize/number.py:150
+#: src/humanize/number.py:188
+#, fuzzy
 msgid "decillion"
 msgid_plural "decillion"
-msgstr[0] "decilhão"
-msgstr[1] "decilhão"
+msgstr[0] "%(value)s décillion"
+msgstr[1] "%(value)s décillion"
 
-#: src/humanize/number.py:151
+#: src/humanize/number.py:189
+#, fuzzy
 msgid "googol"
 msgid_plural "googol"
-msgstr[0] "undecilhão"
-msgstr[1] "undecilhão"
+msgstr[0] "%(value)s gogol"
+msgstr[1] "%(value)s gogol"
 
-#: src/humanize/number.py:246
+#: src/humanize/number.py:301
 msgid "zero"
-msgstr "zero"
+msgstr ""
 
-#: src/humanize/number.py:247
+#: src/humanize/number.py:302
 msgid "one"
-msgstr "um"
+msgstr "하나"
 
-#: src/humanize/number.py:248
+#: src/humanize/number.py:303
 msgid "two"
-msgstr "dois"
+msgstr "둘"
 
-#: src/humanize/number.py:249
+#: src/humanize/number.py:304
 msgid "three"
-msgstr "três"
+msgstr "셋"
 
-#: src/humanize/number.py:250
+#: src/humanize/number.py:305
 msgid "four"
-msgstr "quatro"
+msgstr "넷"
 
-#: src/humanize/number.py:251
+#: src/humanize/number.py:306
 msgid "five"
-msgstr "cinco"
+msgstr "다섯"
 
-#: src/humanize/number.py:252
+#: src/humanize/number.py:307
 msgid "six"
-msgstr "seis"
+msgstr "여섯"
 
-#: src/humanize/number.py:253
+#: src/humanize/number.py:308
 msgid "seven"
-msgstr "sete"
+msgstr "일곱"
 
-#: src/humanize/number.py:254
+#: src/humanize/number.py:309
 msgid "eight"
-msgstr "oito"
+msgstr "여덟"
 
-#: src/humanize/number.py:255
+#: src/humanize/number.py:310
 msgid "nine"
-msgstr "nove"
+msgstr "아홉"
 
-#: src/humanize/time.py:133
-#, fuzzy, python-format
+#: src/humanize/time.py:152
+#, python-format
 msgid "%d microsecond"
 msgid_plural "%d microseconds"
-msgstr[0] "%d microssegundo"
-msgstr[1] "%d microssegundos"
+msgstr[0] "%d마이크로초"
+msgstr[1] "%d마이크로초"
 
-#: src/humanize/time.py:142
-#, fuzzy, python-format
+#: src/humanize/time.py:161
+#, python-format
 msgid "%d millisecond"
 msgid_plural "%d milliseconds"
-msgstr[0] "%d milissegundo"
-msgstr[1] "%d milissegundos"
+msgstr[0] "%d밀리초"
+msgstr[1] "%d밀리초"
 
-#: src/humanize/time.py:145 src/humanize/time.py:220
+#: src/humanize/time.py:164 src/humanize/time.py:259
 msgid "a moment"
-msgstr "um momento"
+msgstr "잠깐"
 
-#: src/humanize/time.py:147
+#: src/humanize/time.py:167
 msgid "a second"
-msgstr "um segundo"
+msgstr "1초"
 
-#: src/humanize/time.py:149
+#: src/humanize/time.py:170
 #, python-format
 msgid "%d second"
 msgid_plural "%d seconds"
-msgstr[0] "%d segundo"
-msgstr[1] "%d segundos"
+msgstr[0] "%d초"
+msgstr[1] "%d초"
 
-#: src/humanize/time.py:151
+#: src/humanize/time.py:173
 msgid "a minute"
-msgstr "um minuto"
+msgstr "1분"
 
-#: src/humanize/time.py:154
+#: src/humanize/time.py:177
 #, python-format
 msgid "%d minute"
 msgid_plural "%d minutes"
-msgstr[0] "%d minuto"
-msgstr[1] "%d minutos"
+msgstr[0] "%d분"
+msgstr[1] "%d분"
 
-#: src/humanize/time.py:156
+#: src/humanize/time.py:180
 msgid "an hour"
-msgstr "uma hora"
+msgstr "1시간"
 
-#: src/humanize/time.py:159
+#: src/humanize/time.py:184
 #, python-format
 msgid "%d hour"
 msgid_plural "%d hours"
-msgstr[0] "%d hora"
-msgstr[1] "%d horas"
+msgstr[0] "%d시간"
+msgstr[1] "%d시간"
 
-#: src/humanize/time.py:162
+#: src/humanize/time.py:188
 msgid "a day"
-msgstr "um dia"
+msgstr "하루"
 
-#: src/humanize/time.py:164 src/humanize/time.py:167
+#: src/humanize/time.py:191 src/humanize/time.py:194
 #, python-format
 msgid "%d day"
 msgid_plural "%d days"
-msgstr[0] "%d dia"
-msgstr[1] "%d dias"
+msgstr[0] "%d일"
+msgstr[1] "%d일"
 
-#: src/humanize/time.py:169
+#: src/humanize/time.py:197
 msgid "a month"
-msgstr "um mês"
+msgstr "1개월"
 
-#: src/humanize/time.py:171
+#: src/humanize/time.py:199
 #, python-format
 msgid "%d month"
 msgid_plural "%d months"
-msgstr[0] "%d mês"
-msgstr[1] "%d meses"
+msgstr[0] "%d개월"
+msgstr[1] "%d개월"
 
-#: src/humanize/time.py:174
+#: src/humanize/time.py:203
 msgid "a year"
-msgstr "um ano"
+msgstr "1년"
 
-#: src/humanize/time.py:176 src/humanize/time.py:185
+#: src/humanize/time.py:206 src/humanize/time.py:217
 #, python-format
 msgid "1 year, %d day"
 msgid_plural "1 year, %d days"
-msgstr[0] "1 ano e %d dia"
-msgstr[1] "1 ano e %d dias"
+msgstr[0] "1년, %d일"
+msgstr[1] "1년, %d일"
 
-#: src/humanize/time.py:179
+#: src/humanize/time.py:210
 msgid "1 year, 1 month"
-msgstr "1 ano e 1 mês"
+msgstr "1년, 1개월"
 
-#: src/humanize/time.py:182
+#: src/humanize/time.py:213
 #, python-format
 msgid "1 year, %d month"
 msgid_plural "1 year, %d months"
-msgstr[0] "1 ano e %d mês"
-msgstr[1] "1 ano e %d meses"
+msgstr[0] "1년, %d개월"
+msgstr[1] "1년, %d개월"
 
-#: src/humanize/time.py:187
+#: src/humanize/time.py:219
 #, python-format
 msgid "%d year"
 msgid_plural "%d years"
-msgstr[0] "%d ano"
-msgstr[1] "%d anos"
+msgstr[0] "%d년"
+msgstr[1] "%d년"
 
-#: src/humanize/time.py:217
+#: src/humanize/time.py:256
 #, python-format
 msgid "%s from now"
-msgstr "em %s"
+msgstr "%s 후"
 
-#: src/humanize/time.py:217
+#: src/humanize/time.py:256
 #, python-format
 msgid "%s ago"
-msgstr "há %s"
+msgstr "%s 전"
 
-#: src/humanize/time.py:221
+#: src/humanize/time.py:260
 msgid "now"
-msgstr "agora"
+msgstr "방금"
 
-#: src/humanize/time.py:244
+#: src/humanize/time.py:284
 msgid "today"
-msgstr "hoje"
+msgstr "오늘"
 
-#: src/humanize/time.py:246
+#: src/humanize/time.py:287
 msgid "tomorrow"
-msgstr "amanhã"
+msgstr "내일"
 
-#: src/humanize/time.py:248
+#: src/humanize/time.py:290
 msgid "yesterday"
-msgstr "ontem"
+msgstr "어제"
 
-#: src/humanize/time.py:534
+#: src/humanize/time.py:600
 #, python-format
 msgid "%s and %s"
-msgstr "%s e %s"
+msgstr ""
```

### Comparing `humanize-4.5.0/src/humanize/locale/pt_PT/LC_MESSAGES/humanize.mo` & `humanize-4.6.0/src/humanize/locale/pt_PT/LC_MESSAGES/humanize.mo`

 * *Files identical despite different names*

### Comparing `humanize-4.5.0/src/humanize/locale/pt_PT/LC_MESSAGES/humanize.po` & `humanize-4.6.0/src/humanize/locale/fr_FR/LC_MESSAGES/humanize.po`

 * *Files 12% similar despite different names*

```diff
@@ -1,364 +1,375 @@
-# SOME DESCRIPTIVE TITLE.
-# Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
-# This file is distributed under the same license as the PACKAGE package.
-# FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
+# French (France) translations for PROJECT.
+# Copyright (C) 2013 ORGANIZATION
+# This file is distributed under the same license as the PROJECT project.
+# FIRST AUTHOR <EMAIL@ADDRESS>, 2013.
 #
 msgid ""
 msgstr ""
-"Project-Id-Version: \n"
+"Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2021-05-04 23:15+0200\n"
-"PO-Revision-Date: 2020-07-05 18:17+0100\n"
-"Last-Translator: \n"
-"Language-Team: \n"
-"Language: pt_PT\n"
+"POT-Creation-Date: 2023-01-08 19:22+0200\n"
+"PO-Revision-Date: 2013-06-22 08:52+0100\n"
+"Last-Translator: Olivier Cortès <oc@1flow.io>\n"
+"Language-Team: fr_FR <LL@li.org>\n"
+"Language: fr\n"
 "MIME-Version: 1.0\n"
-"Content-Type: text/plain; charset=UTF-8\n"
+"Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n > 1);\n"
-"X-Generator: Poedit 2.3.1\n"
+"Generated-By: Babel 0.9.6\n"
+"X-Generator: Poedit 1.5.5\n"
 
-#: src/humanize/number.py:57
+#: src/humanize/number.py:84
 msgctxt "0 (male)"
 msgid "th"
-msgstr "º"
+msgstr "e"
 
-#: src/humanize/number.py:58
+#: src/humanize/number.py:85
 msgctxt "1 (male)"
 msgid "st"
-msgstr "º"
+msgstr "er"
 
-#: src/humanize/number.py:59
+#: src/humanize/number.py:86
 msgctxt "2 (male)"
 msgid "nd"
-msgstr "º"
+msgstr "e"
 
-#: src/humanize/number.py:60
+#: src/humanize/number.py:87
 msgctxt "3 (male)"
 msgid "rd"
-msgstr "º"
+msgstr "e"
 
-#: src/humanize/number.py:61
+#: src/humanize/number.py:88
 msgctxt "4 (male)"
 msgid "th"
-msgstr "º"
+msgstr "e"
 
-#: src/humanize/number.py:62
+#: src/humanize/number.py:89
 msgctxt "5 (male)"
 msgid "th"
-msgstr "º"
+msgstr "e"
 
-#: src/humanize/number.py:63
+#: src/humanize/number.py:90
 msgctxt "6 (male)"
 msgid "th"
-msgstr "º"
+msgstr "e"
 
-#: src/humanize/number.py:64
+#: src/humanize/number.py:91
 msgctxt "7 (male)"
 msgid "th"
-msgstr "º"
+msgstr "e"
 
-#: src/humanize/number.py:65
+#: src/humanize/number.py:92
 msgctxt "8 (male)"
 msgid "th"
-msgstr "º"
+msgstr "e"
 
-#: src/humanize/number.py:66
+#: src/humanize/number.py:93
 msgctxt "9 (male)"
 msgid "th"
-msgstr "º"
+msgstr "e"
 
-#: src/humanize/number.py:70
+#: src/humanize/number.py:97
 msgctxt "0 (female)"
 msgid "th"
-msgstr "ª"
+msgstr "e"
 
-#: src/humanize/number.py:71
+#: src/humanize/number.py:98
 msgctxt "1 (female)"
 msgid "st"
-msgstr "ª"
+msgstr "ère"
 
-#: src/humanize/number.py:72
+#: src/humanize/number.py:99
 msgctxt "2 (female)"
 msgid "nd"
-msgstr "ª"
+msgstr "e"
 
-#: src/humanize/number.py:73
+#: src/humanize/number.py:100
 msgctxt "3 (female)"
 msgid "rd"
-msgstr "ª"
+msgstr "e"
 
-#: src/humanize/number.py:74
+#: src/humanize/number.py:101
 msgctxt "4 (female)"
 msgid "th"
-msgstr "ª"
+msgstr "e"
 
-#: src/humanize/number.py:75
+#: src/humanize/number.py:102
 msgctxt "5 (female)"
 msgid "th"
-msgstr "ª"
+msgstr "e"
 
-#: src/humanize/number.py:76
+#: src/humanize/number.py:103
 msgctxt "6 (female)"
 msgid "th"
-msgstr "ª"
+msgstr "e"
 
-#: src/humanize/number.py:77
+#: src/humanize/number.py:104
 msgctxt "7 (female)"
 msgid "th"
-msgstr "ª"
+msgstr "e"
 
-#: src/humanize/number.py:78
+#: src/humanize/number.py:105
 msgctxt "8 (female)"
 msgid "th"
-msgstr "ª"
+msgstr "e"
 
-#: src/humanize/number.py:79
+#: src/humanize/number.py:106
 msgctxt "9 (female)"
 msgid "th"
-msgstr "ª"
+msgstr "e"
 
-#: src/humanize/number.py:140
+#: src/humanize/number.py:178
 msgid "thousand"
 msgid_plural "thousand"
 msgstr[0] ""
 msgstr[1] ""
 
-#: src/humanize/number.py:141
+#: src/humanize/number.py:179
+#, fuzzy
 msgid "million"
 msgid_plural "million"
-msgstr[0] "milhão"
-msgstr[1] "milhão"
+msgstr[0] "%(value)s million"
+msgstr[1] "%(value)s million"
 
-#: src/humanize/number.py:142
+#: src/humanize/number.py:180
 msgid "billion"
 msgid_plural "billion"
-msgstr[0] "milhar de milhão"
-msgstr[1] "milhar de milhão"
+msgstr[0] "milliard"
+msgstr[1] "milliard"
 
-#: src/humanize/number.py:143
+#: src/humanize/number.py:181
+#, fuzzy
 msgid "trillion"
 msgid_plural "trillion"
-msgstr[0] "bilião"
-msgstr[1] "bilião"
+msgstr[0] "%(value)s billion"
+msgstr[1] "%(value)s billion"
 
-#: src/humanize/number.py:144
+#: src/humanize/number.py:182
+#, fuzzy
 msgid "quadrillion"
 msgid_plural "quadrillion"
-msgstr[0] "mil biliões"
-msgstr[1] "mil biliões"
+msgstr[0] "%(value)s billiard"
+msgstr[1] "%(value)s billiard"
 
-#: src/humanize/number.py:145
+#: src/humanize/number.py:183
+#, fuzzy
 msgid "quintillion"
 msgid_plural "quintillion"
-msgstr[0] "trilião"
-msgstr[1] "trilião"
+msgstr[0] "%(value)s trillion"
+msgstr[1] "%(value)s trillion"
 
-#: src/humanize/number.py:146
+#: src/humanize/number.py:184
+#, fuzzy
 msgid "sextillion"
 msgid_plural "sextillion"
-msgstr[0] "mil triliões"
-msgstr[1] "mil triliões"
+msgstr[0] "%(value)s trilliard"
+msgstr[1] "%(value)s trilliard"
 
-#: src/humanize/number.py:147
+#: src/humanize/number.py:185
+#, fuzzy
 msgid "septillion"
 msgid_plural "septillion"
-msgstr[0] "quatrilião"
-msgstr[1] "quatrilião"
+msgstr[0] "%(value)s quatrillion"
+msgstr[1] "%(value)s quatrillion"
 
-#: src/humanize/number.py:148
+#: src/humanize/number.py:186
+#, fuzzy
 msgid "octillion"
 msgid_plural "octillion"
-msgstr[0] "mil quatriliões"
-msgstr[1] "mil quatriliões"
+msgstr[0] "%(value)s quadrilliard"
+msgstr[1] "%(value)s quadrilliard"
 
-#: src/humanize/number.py:149
+#: src/humanize/number.py:187
+#, fuzzy
 msgid "nonillion"
 msgid_plural "nonillion"
-msgstr[0] "quintilhão"
-msgstr[1] "quintilhão"
+msgstr[0] "%(value)s quintillion"
+msgstr[1] "%(value)s quintillion"
 
-#: src/humanize/number.py:150
+#: src/humanize/number.py:188
+#, fuzzy
 msgid "decillion"
 msgid_plural "decillion"
-msgstr[0] "mil quintilhões"
-msgstr[1] "mil quintilhões"
+msgstr[0] "%(value)s quintilliard"
+msgstr[1] "%(value)s quintilliard"
 
-#: src/humanize/number.py:151
+#: src/humanize/number.py:189
+#, fuzzy
 msgid "googol"
 msgid_plural "googol"
-msgstr[0] "sextilhão"
-msgstr[1] "sextilhão"
+msgstr[0] "%(value)s gogol"
+msgstr[1] "%(value)s gogol"
 
-#: src/humanize/number.py:246
+#: src/humanize/number.py:301
 msgid "zero"
-msgstr "zero"
+msgstr "zéro"
 
-#: src/humanize/number.py:247
+#: src/humanize/number.py:302
 msgid "one"
-msgstr "um"
+msgstr "un"
 
-#: src/humanize/number.py:248
+#: src/humanize/number.py:303
 msgid "two"
-msgstr "dois"
+msgstr "deux"
 
-#: src/humanize/number.py:249
+#: src/humanize/number.py:304
 msgid "three"
-msgstr "três"
+msgstr "trois"
 
-#: src/humanize/number.py:250
+#: src/humanize/number.py:305
 msgid "four"
-msgstr "quatro"
+msgstr "quatre"
 
-#: src/humanize/number.py:251
+#: src/humanize/number.py:306
 msgid "five"
-msgstr "cinco"
+msgstr "cinq"
 
-#: src/humanize/number.py:252
+#: src/humanize/number.py:307
 msgid "six"
-msgstr "seis"
+msgstr "six"
 
-#: src/humanize/number.py:253
+#: src/humanize/number.py:308
 msgid "seven"
-msgstr "sete"
+msgstr "sept"
 
-#: src/humanize/number.py:254
+#: src/humanize/number.py:309
 msgid "eight"
-msgstr "oito"
+msgstr "huit"
 
-#: src/humanize/number.py:255
+#: src/humanize/number.py:310
 msgid "nine"
-msgstr "nove"
+msgstr "neuf"
 
-#: src/humanize/time.py:133
-#, python-format
+#: src/humanize/time.py:152
+#, fuzzy, python-format
 msgid "%d microsecond"
 msgid_plural "%d microseconds"
-msgstr[0] "%d microssegundo"
-msgstr[1] "%d microssegundos"
+msgstr[0] "%d microseconde"
+msgstr[1] "%d microsecondes"
 
-#: src/humanize/time.py:142
-#, python-format
+#: src/humanize/time.py:161
+#, fuzzy, python-format
 msgid "%d millisecond"
 msgid_plural "%d milliseconds"
-msgstr[0] "%d milissegundo"
-msgstr[1] "%d milissegundos"
+msgstr[0] "%d milliseconde"
+msgstr[1] "%d millisecondes"
 
-#: src/humanize/time.py:145 src/humanize/time.py:220
+#: src/humanize/time.py:164 src/humanize/time.py:259
 msgid "a moment"
-msgstr "um momento"
+msgstr "un moment"
 
-#: src/humanize/time.py:147
+#: src/humanize/time.py:167
 msgid "a second"
-msgstr "um segundo"
+msgstr "une seconde"
 
-#: src/humanize/time.py:149
+#: src/humanize/time.py:170
 #, python-format
 msgid "%d second"
 msgid_plural "%d seconds"
-msgstr[0] "%d segundo"
-msgstr[1] "%d segundos"
+msgstr[0] "%d seconde"
+msgstr[1] "%d secondes"
 
-#: src/humanize/time.py:151
+#: src/humanize/time.py:173
 msgid "a minute"
-msgstr "um minuto"
+msgstr "une minute"
 
-#: src/humanize/time.py:154
+#: src/humanize/time.py:177
 #, python-format
 msgid "%d minute"
 msgid_plural "%d minutes"
-msgstr[0] "%d minuto"
-msgstr[1] "%d minutos"
+msgstr[0] "%d minute"
+msgstr[1] "%d minutes"
 
-#: src/humanize/time.py:156
+#: src/humanize/time.py:180
 msgid "an hour"
-msgstr "uma hora"
+msgstr "une heure"
 
-#: src/humanize/time.py:159
+#: src/humanize/time.py:184
 #, python-format
 msgid "%d hour"
 msgid_plural "%d hours"
-msgstr[0] "%d hora"
-msgstr[1] "%d horas"
+msgstr[0] "%d heure"
+msgstr[1] "%d heures"
 
-#: src/humanize/time.py:162
+#: src/humanize/time.py:188
 msgid "a day"
-msgstr "um dia"
+msgstr "un jour"
 
-#: src/humanize/time.py:164 src/humanize/time.py:167
+#: src/humanize/time.py:191 src/humanize/time.py:194
 #, python-format
 msgid "%d day"
 msgid_plural "%d days"
-msgstr[0] "%d dia"
-msgstr[1] "%d dias"
+msgstr[0] "%d jour"
+msgstr[1] "%d jours"
 
-#: src/humanize/time.py:169
+#: src/humanize/time.py:197
 msgid "a month"
-msgstr "um mês"
+msgstr "un mois"
 
-#: src/humanize/time.py:171
+#: src/humanize/time.py:199
 #, python-format
 msgid "%d month"
 msgid_plural "%d months"
-msgstr[0] "%d mês"
-msgstr[1] "%d meses"
+msgstr[0] "%d mois"
+msgstr[1] "%d mois"
 
-#: src/humanize/time.py:174
+#: src/humanize/time.py:203
 msgid "a year"
-msgstr "um ano"
+msgstr "un an"
 
-#: src/humanize/time.py:176 src/humanize/time.py:185
+#: src/humanize/time.py:206 src/humanize/time.py:217
 #, python-format
 msgid "1 year, %d day"
 msgid_plural "1 year, %d days"
-msgstr[0] "1 ano e %d dia"
-msgstr[1] "1 ano e %d dias"
+msgstr[0] "un an et %d jour"
+msgstr[1] "un an et %d jours"
 
-#: src/humanize/time.py:179
+#: src/humanize/time.py:210
 msgid "1 year, 1 month"
-msgstr "1 ano e 1 mês"
+msgstr "un an et un mois"
 
-#: src/humanize/time.py:182
+#: src/humanize/time.py:213
 #, python-format
 msgid "1 year, %d month"
 msgid_plural "1 year, %d months"
-msgstr[0] "1 ano e %d mês"
-msgstr[1] "1 ano e %d meses"
+msgstr[0] "un an et %d mois"
+msgstr[1] "un an et %d mois"
 
-#: src/humanize/time.py:187
+#: src/humanize/time.py:219
 #, python-format
 msgid "%d year"
 msgid_plural "%d years"
-msgstr[0] "%d ano"
-msgstr[1] "%d anos"
+msgstr[0] "%d an"
+msgstr[1] "%d ans"
 
-#: src/humanize/time.py:217
+#: src/humanize/time.py:256
 #, python-format
 msgid "%s from now"
-msgstr "daqui a %s"
+msgstr "dans %s"
 
-#: src/humanize/time.py:217
+#: src/humanize/time.py:256
 #, python-format
 msgid "%s ago"
-msgstr "há %s"
+msgstr "il y a %s"
 
-#: src/humanize/time.py:221
+#: src/humanize/time.py:260
 msgid "now"
-msgstr "agora"
+msgstr "maintenant"
 
-#: src/humanize/time.py:244
+#: src/humanize/time.py:284
 msgid "today"
-msgstr "hoje"
+msgstr "aujourd'hui"
 
-#: src/humanize/time.py:246
+#: src/humanize/time.py:287
 msgid "tomorrow"
-msgstr "amanhã"
+msgstr "demain"
 
-#: src/humanize/time.py:248
+#: src/humanize/time.py:290
 msgid "yesterday"
-msgstr "ontem"
+msgstr "hier"
 
-#: src/humanize/time.py:534
+#: src/humanize/time.py:600
 #, python-format
 msgid "%s and %s"
-msgstr "%s e %s"
+msgstr "%s et %s"
```

### Comparing `humanize-4.5.0/src/humanize/locale/ru_RU/LC_MESSAGES/humanize.mo` & `humanize-4.6.0/src/humanize/locale/ru_RU/LC_MESSAGES/humanize.mo`

 * *Files identical despite different names*

### Comparing `humanize-4.5.0/src/humanize/locale/ru_RU/LC_MESSAGES/humanize.po` & `humanize-4.6.0/src/humanize/locale/ru_RU/LC_MESSAGES/humanize.po`

 * *Files 4% similar despite different names*

```diff
@@ -3,386 +3,386 @@
 # This file is distributed under the same license as the PROJECT project.
 # FIRST AUTHOR <EMAIL@ADDRESS>, 2013.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2021-05-04 23:15+0200\n"
+"POT-Creation-Date: 2023-01-08 19:22+0200\n"
 "PO-Revision-Date: 2014-03-24 20:32+0300\n"
 "Last-Translator: Sergey Prokhorov <me@seriyps.ru>\n"
 "Language-Team: ru_RU <LL@li.org>\n"
 "Language: ru\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=3; plural=(n%10==1 && n%100!=11 ? 0 : n%10>=2 && n"
-"%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2);\n"
+"Plural-Forms: nplurals=3; plural=(n%10==1 && n%100!=11 ? 0 : n%10>=2 && "
+"n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2);\n"
 "Generated-By: Babel 0.9.6\n"
 "X-Generator: Poedit 1.5.4\n"
 
-#: src/humanize/number.py:57
+#: src/humanize/number.py:84
 msgctxt "0 (male)"
 msgid "th"
 msgstr "ой"
 
-#: src/humanize/number.py:58
+#: src/humanize/number.py:85
 msgctxt "1 (male)"
 msgid "st"
 msgstr "ый"
 
-#: src/humanize/number.py:59
+#: src/humanize/number.py:86
 msgctxt "2 (male)"
 msgid "nd"
 msgstr "ой"
 
-#: src/humanize/number.py:60
+#: src/humanize/number.py:87
 msgctxt "3 (male)"
 msgid "rd"
 msgstr "ий"
 
-#: src/humanize/number.py:61
+#: src/humanize/number.py:88
 msgctxt "4 (male)"
 msgid "th"
 msgstr "ый"
 
-#: src/humanize/number.py:62
+#: src/humanize/number.py:89
 msgctxt "5 (male)"
 msgid "th"
 msgstr "ый"
 
-#: src/humanize/number.py:63
+#: src/humanize/number.py:90
 msgctxt "6 (male)"
 msgid "th"
 msgstr "ой"
 
-#: src/humanize/number.py:64
+#: src/humanize/number.py:91
 msgctxt "7 (male)"
 msgid "th"
 msgstr "ой"
 
-#: src/humanize/number.py:65
+#: src/humanize/number.py:92
 msgctxt "8 (male)"
 msgid "th"
 msgstr "ой"
 
-#: src/humanize/number.py:66
+#: src/humanize/number.py:93
 msgctxt "9 (male)"
 msgid "th"
 msgstr "ый"
 
-#: src/humanize/number.py:70
+#: src/humanize/number.py:97
 msgctxt "0 (female)"
 msgid "th"
 msgstr "ой"
 
-#: src/humanize/number.py:71
+#: src/humanize/number.py:98
 msgctxt "1 (female)"
 msgid "st"
 msgstr "ый"
 
-#: src/humanize/number.py:72
+#: src/humanize/number.py:99
 msgctxt "2 (female)"
 msgid "nd"
 msgstr "ой"
 
-#: src/humanize/number.py:73
+#: src/humanize/number.py:100
 msgctxt "3 (female)"
 msgid "rd"
 msgstr "ий"
 
-#: src/humanize/number.py:74
+#: src/humanize/number.py:101
 msgctxt "4 (female)"
 msgid "th"
 msgstr "ый"
 
-#: src/humanize/number.py:75
+#: src/humanize/number.py:102
 msgctxt "5 (female)"
 msgid "th"
 msgstr "ый"
 
-#: src/humanize/number.py:76
+#: src/humanize/number.py:103
 msgctxt "6 (female)"
 msgid "th"
 msgstr "ой"
 
-#: src/humanize/number.py:77
+#: src/humanize/number.py:104
 msgctxt "7 (female)"
 msgid "th"
 msgstr "ой"
 
-#: src/humanize/number.py:78
+#: src/humanize/number.py:105
 msgctxt "8 (female)"
 msgid "th"
 msgstr "ой"
 
-#: src/humanize/number.py:79
+#: src/humanize/number.py:106
 msgctxt "9 (female)"
 msgid "th"
 msgstr "ый"
 
-#: src/humanize/number.py:140
+#: src/humanize/number.py:178
 msgid "thousand"
 msgid_plural "thousand"
 msgstr[0] "тысяча"
 msgstr[1] "тысячи"
 msgstr[2] "тысяч"
 
-#: src/humanize/number.py:141
+#: src/humanize/number.py:179
 msgid "million"
 msgid_plural "million"
 msgstr[0] "миллион"
 msgstr[1] "миллиона"
 msgstr[2] "миллионов"
 
-#: src/humanize/number.py:142
+#: src/humanize/number.py:180
 msgid "billion"
 msgid_plural "billion"
 msgstr[0] "миллиард"
 msgstr[1] "миллиарда"
 msgstr[2] "миллиардов"
 
-#: src/humanize/number.py:143
+#: src/humanize/number.py:181
 msgid "trillion"
 msgid_plural "trillion"
 msgstr[0] "триллион"
 msgstr[1] "триллиона"
 msgstr[2] "триллионов"
 
-#: src/humanize/number.py:144
+#: src/humanize/number.py:182
 msgid "quadrillion"
 msgid_plural "quadrillion"
 msgstr[0] "квадриллион"
 msgstr[1] "квадриллиона"
 msgstr[2] "квадриллионов"
 
-#: src/humanize/number.py:145
+#: src/humanize/number.py:183
 msgid "quintillion"
 msgid_plural "quintillion"
 msgstr[0] "квинтиллион"
 msgstr[1] "квинтиллиона"
 msgstr[2] "квинтиллионов"
 
-#: src/humanize/number.py:146
+#: src/humanize/number.py:184
 msgid "sextillion"
 msgid_plural "sextillion"
 msgstr[0] "сикстиллион"
 msgstr[1] "сикстиллиона"
 msgstr[2] "сикстиллионов"
 
-#: src/humanize/number.py:147
+#: src/humanize/number.py:185
 msgid "septillion"
 msgid_plural "septillion"
 msgstr[0] "септиллион"
 msgstr[1] "септиллиона"
 msgstr[2] "септиллионов"
 
-#: src/humanize/number.py:148
+#: src/humanize/number.py:186
 msgid "octillion"
 msgid_plural "octillion"
 msgstr[0] "октиллион"
 msgstr[1] "октиллиона"
 msgstr[2] "октиллионов"
 
-#: src/humanize/number.py:149
+#: src/humanize/number.py:187
 msgid "nonillion"
 msgid_plural "nonillion"
 msgstr[0] "нониллион"
 msgstr[1] "нониллиона"
 msgstr[2] "нониллионов"
 
-#: src/humanize/number.py:150
+#: src/humanize/number.py:188
 msgid "decillion"
 msgid_plural "decillion"
 msgstr[0] "децилион"
 msgstr[1] "децилиона"
 msgstr[2] "децилионов"
 
-#: src/humanize/number.py:151
+#: src/humanize/number.py:189
 msgid "googol"
 msgid_plural "googol"
 msgstr[0] "гогол"
 msgstr[1] "гогола"
 msgstr[2] "гоголов"
 
-#: src/humanize/number.py:246
+#: src/humanize/number.py:301
 msgid "zero"
 msgstr "ноль"
 
-#: src/humanize/number.py:247
+#: src/humanize/number.py:302
 msgid "one"
 msgstr "один"
 
-#: src/humanize/number.py:248
+#: src/humanize/number.py:303
 msgid "two"
 msgstr "два"
 
-#: src/humanize/number.py:249
+#: src/humanize/number.py:304
 msgid "three"
 msgstr "три"
 
-#: src/humanize/number.py:250
+#: src/humanize/number.py:305
 msgid "four"
 msgstr "четыре"
 
-#: src/humanize/number.py:251
+#: src/humanize/number.py:306
 msgid "five"
 msgstr "пять"
 
-#: src/humanize/number.py:252
+#: src/humanize/number.py:307
 msgid "six"
 msgstr "шесть"
 
-#: src/humanize/number.py:253
+#: src/humanize/number.py:308
 msgid "seven"
 msgstr "семь"
 
-#: src/humanize/number.py:254
+#: src/humanize/number.py:309
 msgid "eight"
 msgstr "восемь"
 
-#: src/humanize/number.py:255
+#: src/humanize/number.py:310
 msgid "nine"
 msgstr "девять"
 
-#: src/humanize/time.py:133
+#: src/humanize/time.py:152
 #, python-format
 msgid "%d microsecond"
 msgid_plural "%d microseconds"
 msgstr[0] "%d микросекунда"
 msgstr[1] "%d микросекунды"
 msgstr[2] "%d микросекунд"
 
-#: src/humanize/time.py:142
+#: src/humanize/time.py:161
 #, python-format
 msgid "%d millisecond"
 msgid_plural "%d milliseconds"
 msgstr[0] "%d миллисекунда"
 msgstr[1] "%d миллисекунды"
 msgstr[2] "%d миллисекунд"
 
-#: src/humanize/time.py:145 src/humanize/time.py:220
+#: src/humanize/time.py:164 src/humanize/time.py:259
 msgid "a moment"
 msgstr "только что"
 
-#: src/humanize/time.py:147
+#: src/humanize/time.py:167
 msgid "a second"
 msgstr "секунду"
 
-#: src/humanize/time.py:149
+#: src/humanize/time.py:170
 #, python-format
 msgid "%d second"
 msgid_plural "%d seconds"
 msgstr[0] "%d секунда"
 msgstr[1] "%d секунды"
 msgstr[2] "%d секунд"
 
-#: src/humanize/time.py:151
+#: src/humanize/time.py:173
 msgid "a minute"
 msgstr "минуту"
 
-#: src/humanize/time.py:154
+#: src/humanize/time.py:177
 #, python-format
 msgid "%d minute"
 msgid_plural "%d minutes"
 msgstr[0] "%d минута"
 msgstr[1] "%d минуты"
 msgstr[2] "%d минут"
 
-#: src/humanize/time.py:156
+#: src/humanize/time.py:180
 msgid "an hour"
 msgstr "час"
 
-#: src/humanize/time.py:159
+#: src/humanize/time.py:184
 #, python-format
 msgid "%d hour"
 msgid_plural "%d hours"
 msgstr[0] "%d час"
 msgstr[1] "%d часа"
 msgstr[2] "%d часов"
 
-#: src/humanize/time.py:162
+#: src/humanize/time.py:188
 msgid "a day"
 msgstr "день"
 
-#: src/humanize/time.py:164 src/humanize/time.py:167
+#: src/humanize/time.py:191 src/humanize/time.py:194
 #, python-format
 msgid "%d day"
 msgid_plural "%d days"
 msgstr[0] "%d день"
 msgstr[1] "%d дня"
 msgstr[2] "%d дней"
 
-#: src/humanize/time.py:169
+#: src/humanize/time.py:197
 msgid "a month"
 msgstr "месяц"
 
-#: src/humanize/time.py:171
+#: src/humanize/time.py:199
 #, python-format
 msgid "%d month"
 msgid_plural "%d months"
 msgstr[0] "%d месяц"
 msgstr[1] "%d месяца"
 msgstr[2] "%d месяцев"
 
-#: src/humanize/time.py:174
+#: src/humanize/time.py:203
 msgid "a year"
 msgstr "год"
 
-#: src/humanize/time.py:176 src/humanize/time.py:185
+#: src/humanize/time.py:206 src/humanize/time.py:217
 #, python-format
 msgid "1 year, %d day"
 msgid_plural "1 year, %d days"
 msgstr[0] "1 год, %d день"
 msgstr[1] "1 год, %d дня"
 msgstr[2] "1 год, %d дней"
 
-#: src/humanize/time.py:179
+#: src/humanize/time.py:210
 msgid "1 year, 1 month"
 msgstr "1 год, 1 месяц"
 
-#: src/humanize/time.py:182
+#: src/humanize/time.py:213
 #, python-format
 msgid "1 year, %d month"
 msgid_plural "1 year, %d months"
 msgstr[0] "1 год, %d месяц"
 msgstr[1] "1 год, %d месяца"
 msgstr[2] "1 год, %d месяцев"
 
-#: src/humanize/time.py:187
+#: src/humanize/time.py:219
 #, python-format
 msgid "%d year"
 msgid_plural "%d years"
 msgstr[0] "%d год"
 msgstr[1] "%d года"
 msgstr[2] "%d лет"
 
-#: src/humanize/time.py:217
+#: src/humanize/time.py:256
 #, python-format
 msgid "%s from now"
 msgstr "через %s"
 
-#: src/humanize/time.py:217
+#: src/humanize/time.py:256
 #, python-format
 msgid "%s ago"
 msgstr "%s назад"
 
-#: src/humanize/time.py:221
+#: src/humanize/time.py:260
 msgid "now"
 msgstr "сейчас"
 
-#: src/humanize/time.py:244
+#: src/humanize/time.py:284
 msgid "today"
 msgstr "сегодня"
 
-#: src/humanize/time.py:246
+#: src/humanize/time.py:287
 msgid "tomorrow"
 msgstr "завтра"
 
-#: src/humanize/time.py:248
+#: src/humanize/time.py:290
 msgid "yesterday"
 msgstr "вчера"
 
-#: src/humanize/time.py:534
+#: src/humanize/time.py:600
 #, python-format
 msgid "%s and %s"
 msgstr "%s и %s"
```

### Comparing `humanize-4.5.0/src/humanize/locale/sk_SK/LC_MESSAGES/humanize.mo` & `humanize-4.6.0/src/humanize/locale/sk_SK/LC_MESSAGES/humanize.mo`

 * *Files identical despite different names*

### Comparing `humanize-4.5.0/src/humanize/locale/sk_SK/LC_MESSAGES/humanize.po` & `humanize-4.6.0/src/humanize/locale/uk_UA/LC_MESSAGES/humanize.po`

 * *Files 11% similar despite different names*

```diff
@@ -1,386 +1,383 @@
-# Slovak translation of humanize
-# Copyright (C) 2016
-# This file is distributed under the same license as the PACKAGE package.
-# Jose Riha <jose1711 gmail com>, 2016.
-#
-#, fuzzy
 msgid ""
 msgstr ""
-"Project-Id-Version: humanize\n"
+"Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2021-05-04 23:15+0200\n"
-"PO-Revision-Date: 2020-09-29 22:43+0300\n"
-"Last-Translator: Jose Riha <jose1711 gmail com>\n"
-"Language-Team: sk <LL@li.org>\n"
-"Language: Slovak\n"
+"POT-Creation-Date: 2023-01-08 19:22+0200\n"
+"PO-Revision-Date: \n"
+"Last-Translator: TL\n"
+"Language-Team: uk_UA\n"
+"Language: uk\n"
 "MIME-Version: 1.0\n"
-"Content-Type: text/plain; charset=UTF-8\n"
+"Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=3; plural=(n==1) ? 0 : (n>=2 && n<=4) ? 1 : 2;\n"
+"Plural-Forms: nplurals=3; plural=(n%10==1 && n%100!=11 ? 0 : n%10>=2 && "
+"n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2);\n"
+"Generated-By:\n"
+"X-Generator: \n"
 
-#: src/humanize/number.py:57
+#: src/humanize/number.py:84
 msgctxt "0 (male)"
 msgid "th"
-msgstr "."
+msgstr "ий"
 
-#: src/humanize/number.py:58
+#: src/humanize/number.py:85
 msgctxt "1 (male)"
 msgid "st"
-msgstr "."
+msgstr "ий"
 
-#: src/humanize/number.py:59
+#: src/humanize/number.py:86
 msgctxt "2 (male)"
 msgid "nd"
-msgstr "."
+msgstr "ий"
 
-#: src/humanize/number.py:60
+#: src/humanize/number.py:87
 msgctxt "3 (male)"
 msgid "rd"
-msgstr "."
+msgstr "ій"
 
-#: src/humanize/number.py:61
+#: src/humanize/number.py:88
 msgctxt "4 (male)"
 msgid "th"
-msgstr "."
+msgstr "ий"
 
-#: src/humanize/number.py:62
+#: src/humanize/number.py:89
 msgctxt "5 (male)"
 msgid "th"
-msgstr "."
+msgstr "ий"
 
-#: src/humanize/number.py:63
+#: src/humanize/number.py:90
 msgctxt "6 (male)"
 msgid "th"
-msgstr "."
+msgstr "ий"
 
-#: src/humanize/number.py:64
+#: src/humanize/number.py:91
 msgctxt "7 (male)"
 msgid "th"
-msgstr "."
+msgstr "ий"
 
-#: src/humanize/number.py:65
+#: src/humanize/number.py:92
 msgctxt "8 (male)"
 msgid "th"
-msgstr "."
+msgstr "ий"
 
-#: src/humanize/number.py:66
+#: src/humanize/number.py:93
 msgctxt "9 (male)"
 msgid "th"
-msgstr "."
+msgstr "ий"
 
-#: src/humanize/number.py:70
+#: src/humanize/number.py:97
 msgctxt "0 (female)"
 msgid "th"
-msgstr "."
+msgstr "ий"
 
-#: src/humanize/number.py:71
+#: src/humanize/number.py:98
 msgctxt "1 (female)"
 msgid "st"
-msgstr "."
+msgstr "ий"
 
-#: src/humanize/number.py:72
+#: src/humanize/number.py:99
 msgctxt "2 (female)"
 msgid "nd"
-msgstr "."
+msgstr "ий"
 
-#: src/humanize/number.py:73
+#: src/humanize/number.py:100
 msgctxt "3 (female)"
 msgid "rd"
-msgstr "."
+msgstr "ій"
 
-#: src/humanize/number.py:74
+#: src/humanize/number.py:101
 msgctxt "4 (female)"
 msgid "th"
-msgstr "."
+msgstr "ий"
 
-#: src/humanize/number.py:75
+#: src/humanize/number.py:102
 msgctxt "5 (female)"
 msgid "th"
-msgstr "."
+msgstr "ий"
 
-#: src/humanize/number.py:76
+#: src/humanize/number.py:103
 msgctxt "6 (female)"
 msgid "th"
-msgstr "."
+msgstr "ий"
 
-#: src/humanize/number.py:77
+#: src/humanize/number.py:104
 msgctxt "7 (female)"
 msgid "th"
-msgstr "."
+msgstr "ий"
 
-#: src/humanize/number.py:78
+#: src/humanize/number.py:105
 msgctxt "8 (female)"
 msgid "th"
-msgstr "."
+msgstr "ий"
 
-#: src/humanize/number.py:79
+#: src/humanize/number.py:106
 msgctxt "9 (female)"
 msgid "th"
-msgstr "."
+msgstr "ий"
 
-#: src/humanize/number.py:140
+#: src/humanize/number.py:178
 msgid "thousand"
 msgid_plural "thousand"
-msgstr[0] ""
-msgstr[1] ""
-msgstr[2] ""
+msgstr[0] "тисяча"
+msgstr[1] "тисячі"
+msgstr[2] "тисяч"
 
-#: src/humanize/number.py:141
+#: src/humanize/number.py:179
 msgid "million"
 msgid_plural "million"
-msgstr[0] "milióna/ov"
-msgstr[1] "milióna/ov"
-msgstr[2] "milióna/ov"
+msgstr[0] "мільйон"
+msgstr[1] "мільйона"
+msgstr[2] "мільйонів"
 
-#: src/humanize/number.py:142
+#: src/humanize/number.py:180
 msgid "billion"
 msgid_plural "billion"
-msgstr[0] "miliardy/árd"
-msgstr[1] "miliardy/árd"
-msgstr[2] "miliardy/árd"
+msgstr[0] "мільярд"
+msgstr[1] "мільярда"
+msgstr[2] "мільярдів"
 
-#: src/humanize/number.py:143
+#: src/humanize/number.py:181
 msgid "trillion"
 msgid_plural "trillion"
-msgstr[0] "bilióna/ov"
-msgstr[1] "bilióna/ov"
-msgstr[2] "bilióna/ov"
+msgstr[0] "трильйон"
+msgstr[1] "трильйона"
+msgstr[2] "трильйонів"
 
-#: src/humanize/number.py:144
+#: src/humanize/number.py:182
 msgid "quadrillion"
 msgid_plural "quadrillion"
-msgstr[0] "biliardy/árd"
-msgstr[1] "biliardy/árd"
-msgstr[2] "biliardy/árd"
+msgstr[0] "квадрильйон"
+msgstr[1] "квадрильйона"
+msgstr[2] "квадрильйонів"
 
-#: src/humanize/number.py:145
+#: src/humanize/number.py:183
 msgid "quintillion"
 msgid_plural "quintillion"
-msgstr[0] "trilióna/árd"
-msgstr[1] "trilióna/árd"
-msgstr[2] "trilióna/árd"
+msgstr[0] "квинтиліон"
+msgstr[1] "квинтиліона"
+msgstr[2] "квинтиліонів"
 
-#: src/humanize/number.py:146
+#: src/humanize/number.py:184
 msgid "sextillion"
 msgid_plural "sextillion"
-msgstr[0] "triliardy/árd"
-msgstr[1] "triliardy/árd"
-msgstr[2] "triliardy/árd"
+msgstr[0] "сикстильйон"
+msgstr[1] "сикстильйона"
+msgstr[2] "сикстильйонів"
 
-#: src/humanize/number.py:147
+#: src/humanize/number.py:185
 msgid "septillion"
 msgid_plural "septillion"
-msgstr[0] "kvadrilióna/ov"
-msgstr[1] "kvadrilióna/ov"
-msgstr[2] "kvadrilióna/ov"
+msgstr[0] "септильйон"
+msgstr[1] "септильйона"
+msgstr[2] "септильйонів"
 
-#: src/humanize/number.py:148
+#: src/humanize/number.py:186
 msgid "octillion"
 msgid_plural "octillion"
-msgstr[0] "kvadriliardy/árd"
-msgstr[1] "kvadriliardy/árd"
-msgstr[2] "kvadriliardy/árd"
+msgstr[0] "октильйон"
+msgstr[1] "октильйона"
+msgstr[2] "октильйонів"
 
-#: src/humanize/number.py:149
+#: src/humanize/number.py:187
 msgid "nonillion"
 msgid_plural "nonillion"
-msgstr[0] "kvintilióna/ov"
-msgstr[1] "kvintilióna/ov"
-msgstr[2] "kvintilióna/ov"
+msgstr[0] "нонильйон"
+msgstr[1] "нонильйона"
+msgstr[2] "нонильйонів"
 
-#: src/humanize/number.py:150
+#: src/humanize/number.py:188
 msgid "decillion"
 msgid_plural "decillion"
-msgstr[0] "kvintiliardy/árd"
-msgstr[1] "kvintiliardy/árd"
-msgstr[2] "kvintiliardy/árd"
+msgstr[0] "децильйон"
+msgstr[1] "децильйона"
+msgstr[2] "децильйонів"
 
-#: src/humanize/number.py:151
+#: src/humanize/number.py:189
 msgid "googol"
 msgid_plural "googol"
-msgstr[0] "googola/ov"
-msgstr[1] "googola/ov"
-msgstr[2] "googola/ov"
+msgstr[0] "гугол"
+msgstr[1] "гугла"
+msgstr[2] "гуглів"
 
-#: src/humanize/number.py:246
+#: src/humanize/number.py:301
 msgid "zero"
-msgstr "nula"
+msgstr "нуль"
 
-#: src/humanize/number.py:247
+#: src/humanize/number.py:302
 msgid "one"
-msgstr "jedna"
+msgstr "один"
 
-#: src/humanize/number.py:248
+#: src/humanize/number.py:303
 msgid "two"
-msgstr "dve"
+msgstr "два"
 
-#: src/humanize/number.py:249
+#: src/humanize/number.py:304
 msgid "three"
-msgstr "tri"
+msgstr "три"
 
-#: src/humanize/number.py:250
+#: src/humanize/number.py:305
 msgid "four"
-msgstr "štyri"
+msgstr "чотири"
 
-#: src/humanize/number.py:251
+#: src/humanize/number.py:306
 msgid "five"
-msgstr "päť"
+msgstr "п'ять"
 
-#: src/humanize/number.py:252
+#: src/humanize/number.py:307
 msgid "six"
-msgstr "šesť"
+msgstr "шість"
 
-#: src/humanize/number.py:253
+#: src/humanize/number.py:308
 msgid "seven"
-msgstr "sedem"
+msgstr "сім"
 
-#: src/humanize/number.py:254
+#: src/humanize/number.py:309
 msgid "eight"
-msgstr "osem"
+msgstr "вісім"
 
-#: src/humanize/number.py:255
+#: src/humanize/number.py:310
 msgid "nine"
-msgstr "deväť"
+msgstr "дев'ять"
 
-#: src/humanize/time.py:133
+#: src/humanize/time.py:152
 #, fuzzy, python-format
 msgid "%d microsecond"
 msgid_plural "%d microseconds"
-msgstr[0] "%d mikrosekundu"
-msgstr[1] "%d mikrosekundy"
-msgstr[2] "%d mikrosekúnd"
+msgstr[0] "%d мікросекунда"
+msgstr[1] "%d мікросекунди"
+msgstr[2] "%d мікросекунд"
 
-#: src/humanize/time.py:142
+#: src/humanize/time.py:161
 #, fuzzy, python-format
 msgid "%d millisecond"
 msgid_plural "%d milliseconds"
-msgstr[0] "%d milisekundu"
-msgstr[1] "%d milisekundy"
-msgstr[2] "%d milisekúnd"
+msgstr[0] "%d мілісекунда"
+msgstr[1] "%d мілісекунди"
+msgstr[2] "%d мілісекунд"
 
-#: src/humanize/time.py:145 src/humanize/time.py:220
+#: src/humanize/time.py:164 src/humanize/time.py:259
 msgid "a moment"
-msgstr "chvíľku"
+msgstr "у цей момент"
 
-#: src/humanize/time.py:147
+#: src/humanize/time.py:167
 msgid "a second"
-msgstr "sekundu"
+msgstr "секунда"
 
-#: src/humanize/time.py:149
+#: src/humanize/time.py:170
 #, python-format
 msgid "%d second"
 msgid_plural "%d seconds"
-msgstr[0] "%d sekundu"
-msgstr[1] "%d sekundy"
-msgstr[2] "%d sekúnd"
+msgstr[0] "%d секунда"
+msgstr[1] "%d секунди"
+msgstr[2] "%d секунд"
 
-#: src/humanize/time.py:151
+#: src/humanize/time.py:173
 msgid "a minute"
-msgstr "minútu"
+msgstr "хвилина"
 
-#: src/humanize/time.py:154
+#: src/humanize/time.py:177
 #, python-format
 msgid "%d minute"
 msgid_plural "%d minutes"
-msgstr[0] "%d minútu"
-msgstr[1] "%d minúty"
-msgstr[2] "%d minút"
+msgstr[0] "%d хвилина"
+msgstr[1] "%d хвилини"
+msgstr[2] "%d хвилин"
 
-#: src/humanize/time.py:156
+#: src/humanize/time.py:180
 msgid "an hour"
-msgstr "hodinu"
+msgstr "година"
 
-#: src/humanize/time.py:159
+#: src/humanize/time.py:184
 #, python-format
 msgid "%d hour"
 msgid_plural "%d hours"
-msgstr[0] "%d hodina"
-msgstr[1] "%d hodiny"
-msgstr[2] "%d hodín"
+msgstr[0] "%d година"
+msgstr[1] "%d години"
+msgstr[2] "%d годин"
 
-#: src/humanize/time.py:162
+#: src/humanize/time.py:188
 msgid "a day"
-msgstr "deň"
+msgstr "день"
 
-#: src/humanize/time.py:164 src/humanize/time.py:167
+#: src/humanize/time.py:191 src/humanize/time.py:194
 #, python-format
 msgid "%d day"
 msgid_plural "%d days"
-msgstr[0] "%d deň"
-msgstr[1] "%d dni"
-msgstr[2] "%d dní"
+msgstr[0] "%d день"
+msgstr[1] "%d дня"
+msgstr[2] "%d днів"
 
-#: src/humanize/time.py:169
+#: src/humanize/time.py:197
 msgid "a month"
-msgstr "mesiac"
+msgstr "місяць"
 
-#: src/humanize/time.py:171
+#: src/humanize/time.py:199
 #, python-format
 msgid "%d month"
 msgid_plural "%d months"
-msgstr[0] "%d mesiac"
-msgstr[1] "%d mesiace"
-msgstr[2] "%d mesiacov"
+msgstr[0] "%d місяць"
+msgstr[1] "%d місяця"
+msgstr[2] "%d місяців"
 
-#: src/humanize/time.py:174
+#: src/humanize/time.py:203
 msgid "a year"
-msgstr "rok"
+msgstr "рік"
 
-#: src/humanize/time.py:176 src/humanize/time.py:185
+#: src/humanize/time.py:206 src/humanize/time.py:217
 #, python-format
 msgid "1 year, %d day"
 msgid_plural "1 year, %d days"
-msgstr[0] "1 rok, %d deň"
-msgstr[1] "1 rok, %d dni"
-msgstr[2] "1 rok, %d dní"
+msgstr[0] "1 рік, %d день"
+msgstr[1] "1 рік, %d дня"
+msgstr[2] "1 рік, %d днів"
 
-#: src/humanize/time.py:179
+#: src/humanize/time.py:210
 msgid "1 year, 1 month"
-msgstr "1 rok, 1 mesiac"
+msgstr "1 рік, 1 місяць"
 
-#: src/humanize/time.py:182
+#: src/humanize/time.py:213
 #, python-format
 msgid "1 year, %d month"
 msgid_plural "1 year, %d months"
-msgstr[0] "1 rok, %d mesiac"
-msgstr[1] "1 rok, %d mesiace"
-msgstr[2] "1 rok, %d mesiacov"
+msgstr[0] "1 рік, %d місяць"
+msgstr[1] "1 рік, %d місяця"
+msgstr[2] "1 рік, %d місяців"
 
-#: src/humanize/time.py:187
+#: src/humanize/time.py:219
 #, python-format
 msgid "%d year"
 msgid_plural "%d years"
-msgstr[0] "%d rok"
-msgstr[1] "%d roky"
-msgstr[2] "%d rokov"
+msgstr[0] "%d рік"
+msgstr[1] "%d роки"
+msgstr[2] "%d років"
 
-#: src/humanize/time.py:217
+#: src/humanize/time.py:256
 #, python-format
 msgid "%s from now"
-msgstr "o %s"
+msgstr "через %s"
 
-#: src/humanize/time.py:217
+#: src/humanize/time.py:256
 #, python-format
 msgid "%s ago"
-msgstr "%s naspäť"
+msgstr "%s назад"
 
-#: src/humanize/time.py:221
+#: src/humanize/time.py:260
 msgid "now"
-msgstr "teraz"
+msgstr "зараз"
 
-#: src/humanize/time.py:244
+#: src/humanize/time.py:284
 msgid "today"
-msgstr "dnes"
+msgstr "сьогодні"
 
-#: src/humanize/time.py:246
+#: src/humanize/time.py:287
 msgid "tomorrow"
-msgstr "zajtra"
+msgstr "завтра"
 
-#: src/humanize/time.py:248
+#: src/humanize/time.py:290
 msgid "yesterday"
-msgstr "včera"
+msgstr "вчора"
 
-#: src/humanize/time.py:534
+#: src/humanize/time.py:600
 #, python-format
 msgid "%s and %s"
-msgstr ""
+msgstr "%s й %s"
```

### Comparing `humanize-4.5.0/src/humanize/locale/sl_SI/LC_MESSAGES/humanize.mo` & `humanize-4.6.0/src/humanize/locale/sl_SI/LC_MESSAGES/humanize.mo`

 * *Files identical despite different names*

### Comparing `humanize-4.5.0/src/humanize/locale/sl_SI/LC_MESSAGES/humanize.po` & `humanize-4.6.0/src/humanize/locale/sl_SI/LC_MESSAGES/humanize.po`

 * *Files 13% similar despite different names*

```diff
@@ -3,407 +3,407 @@
 # This file is distributed under the same license as the PACKAGE package.
 # vlin <vlin@vlin-vb1>, 2021.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: humanize\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2021-06-11 22:52+0200\n"
+"POT-Creation-Date: 2023-01-08 19:22+0200\n"
 "PO-Revision-Date: 2021-06-11 23:39+0200\n"
 "Last-Translator: dkrat7 <dkrat7 @github.com>\n"
 "Language-Team: Slovenian\n"
 "Language: sl\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=4; plural=(n%100==1 ? 0 : n%100==2 ? 1 : n%100==3 || n"
-"%100==4 ? 2 : 3);\n"
+"Plural-Forms: nplurals=4; plural=(n%100==1 ? 0 : n%100==2 ? 1 : n%100==3 || "
+"n%100==4 ? 2 : 3);\n"
 "X-Generator: Poedit 2.3\n"
 
-#: src/humanize/number.py:58
+#: src/humanize/number.py:84
 msgctxt "0 (male)"
 msgid "th"
 msgstr "."
 
-#: src/humanize/number.py:59
+#: src/humanize/number.py:85
 msgctxt "1 (male)"
 msgid "st"
 msgstr "."
 
-#: src/humanize/number.py:60
+#: src/humanize/number.py:86
 msgctxt "2 (male)"
 msgid "nd"
 msgstr "."
 
-#: src/humanize/number.py:61
+#: src/humanize/number.py:87
 msgctxt "3 (male)"
 msgid "rd"
 msgstr "."
 
-#: src/humanize/number.py:62
+#: src/humanize/number.py:88
 msgctxt "4 (male)"
 msgid "th"
 msgstr "."
 
-#: src/humanize/number.py:63
+#: src/humanize/number.py:89
 msgctxt "5 (male)"
 msgid "th"
 msgstr "."
 
-#: src/humanize/number.py:64
+#: src/humanize/number.py:90
 msgctxt "6 (male)"
 msgid "th"
 msgstr "."
 
-#: src/humanize/number.py:65
+#: src/humanize/number.py:91
 msgctxt "7 (male)"
 msgid "th"
 msgstr "."
 
-#: src/humanize/number.py:66
+#: src/humanize/number.py:92
 msgctxt "8 (male)"
 msgid "th"
 msgstr "."
 
-#: src/humanize/number.py:67
+#: src/humanize/number.py:93
 msgctxt "9 (male)"
 msgid "th"
 msgstr "."
 
-#: src/humanize/number.py:71
+#: src/humanize/number.py:97
 msgctxt "0 (female)"
 msgid "th"
 msgstr "."
 
-#: src/humanize/number.py:72
+#: src/humanize/number.py:98
 msgctxt "1 (female)"
 msgid "st"
 msgstr "."
 
-#: src/humanize/number.py:73
+#: src/humanize/number.py:99
 msgctxt "2 (female)"
 msgid "nd"
 msgstr "."
 
-#: src/humanize/number.py:74
+#: src/humanize/number.py:100
 msgctxt "3 (female)"
 msgid "rd"
 msgstr "."
 
-#: src/humanize/number.py:75
+#: src/humanize/number.py:101
 msgctxt "4 (female)"
 msgid "th"
 msgstr "."
 
-#: src/humanize/number.py:76
+#: src/humanize/number.py:102
 msgctxt "5 (female)"
 msgid "th"
 msgstr "."
 
-#: src/humanize/number.py:77
+#: src/humanize/number.py:103
 msgctxt "6 (female)"
 msgid "th"
 msgstr "."
 
-#: src/humanize/number.py:78
+#: src/humanize/number.py:104
 msgctxt "7 (female)"
 msgid "th"
 msgstr "."
 
-#: src/humanize/number.py:79
+#: src/humanize/number.py:105
 msgctxt "8 (female)"
 msgid "th"
 msgstr "."
 
-#: src/humanize/number.py:80
+#: src/humanize/number.py:106
 msgctxt "9 (female)"
 msgid "th"
 msgstr "."
 
-#: src/humanize/number.py:140
+#: src/humanize/number.py:178
 msgid "thousand"
 msgid_plural "thousand"
 msgstr[0] "tisoč"
 msgstr[1] "tisoč"
 msgstr[2] "tisoč"
 msgstr[3] "tisoč"
 
-#: src/humanize/number.py:141
+#: src/humanize/number.py:179
 msgid "million"
 msgid_plural "million"
 msgstr[0] "milijon"
 msgstr[1] "milijona"
 msgstr[2] "milijoni"
 msgstr[3] "milijonov"
 
-#: src/humanize/number.py:142
+#: src/humanize/number.py:180
 msgid "billion"
 msgid_plural "billion"
 msgstr[0] "milijarda"
 msgstr[1] "milijardi"
 msgstr[2] "milijarde"
 msgstr[3] "milijard"
 
-#: src/humanize/number.py:143
+#: src/humanize/number.py:181
 msgid "trillion"
 msgid_plural "trillion"
 msgstr[0] "bilijon"
 msgstr[1] "bilijona"
 msgstr[2] "bilijoni"
 msgstr[3] "bilijonov"
 
-#: src/humanize/number.py:144
+#: src/humanize/number.py:182
 msgid "quadrillion"
 msgid_plural "quadrillion"
 msgstr[0] "bilijarda"
 msgstr[1] "bilijardi"
 msgstr[2] "bilijarde"
 msgstr[3] "bilijard"
 
-#: src/humanize/number.py:145
+#: src/humanize/number.py:183
 msgid "quintillion"
 msgid_plural "quintillion"
 msgstr[0] "trilijon"
 msgstr[1] "trilijona"
 msgstr[2] "trilijoni"
 msgstr[3] "trilijonov"
 
-#: src/humanize/number.py:146
+#: src/humanize/number.py:184
 msgid "sextillion"
 msgid_plural "sextillion"
 msgstr[0] "trilijarda"
 msgstr[1] "trilijardi"
 msgstr[2] "trilijarde"
 msgstr[3] "trilijard"
 
-#: src/humanize/number.py:147
+#: src/humanize/number.py:185
 msgid "septillion"
 msgid_plural "septillion"
 msgstr[0] "kvadrilijon"
 msgstr[1] "kvadrilijona"
 msgstr[2] "kvadrilijoni"
 msgstr[3] "kvadrilijonov"
 
-#: src/humanize/number.py:148
+#: src/humanize/number.py:186
 msgid "octillion"
 msgid_plural "octillion"
 msgstr[0] "kvadrilijarda"
 msgstr[1] "kvadrilijardi"
 msgstr[2] "kvadrilijarde"
 msgstr[3] "kvadrilijard"
 
-#: src/humanize/number.py:149
+#: src/humanize/number.py:187
 msgid "nonillion"
 msgid_plural "nonillion"
 msgstr[0] "kvintilijon"
 msgstr[1] "kvintilijona"
 msgstr[2] "kvintilijoni"
 msgstr[3] "kvintilijonov"
 
-#: src/humanize/number.py:150
+#: src/humanize/number.py:188
 msgid "decillion"
 msgid_plural "decillion"
 msgstr[0] "kvintilijarda"
 msgstr[1] "kvintilijardi"
 msgstr[2] "kvintilijarde"
 msgstr[3] "kvintilijard"
 
-#: src/humanize/number.py:151
+#: src/humanize/number.py:189
 msgid "googol"
 msgid_plural "googol"
 msgstr[0] "gugol"
 msgstr[1] "gugola"
 msgstr[2] "gugoli"
 msgstr[3] "gugolov"
 
-#: src/humanize/number.py:247
+#: src/humanize/number.py:301
 msgid "zero"
 msgstr "nič"
 
-#: src/humanize/number.py:248
+#: src/humanize/number.py:302
 msgid "one"
 msgstr "ena"
 
-#: src/humanize/number.py:249
+#: src/humanize/number.py:303
 msgid "two"
 msgstr "dve"
 
-#: src/humanize/number.py:250
+#: src/humanize/number.py:304
 msgid "three"
 msgstr "tri"
 
-#: src/humanize/number.py:251
+#: src/humanize/number.py:305
 msgid "four"
 msgstr "štiri"
 
-#: src/humanize/number.py:252
+#: src/humanize/number.py:306
 msgid "five"
 msgstr "pet"
 
-#: src/humanize/number.py:253
+#: src/humanize/number.py:307
 msgid "six"
 msgstr "šest"
 
-#: src/humanize/number.py:254
+#: src/humanize/number.py:308
 msgid "seven"
 msgstr "sedem"
 
-#: src/humanize/number.py:255
+#: src/humanize/number.py:309
 msgid "eight"
 msgstr "osem"
 
-#: src/humanize/number.py:256
+#: src/humanize/number.py:310
 msgid "nine"
 msgstr "devet"
 
-#: src/humanize/time.py:138
+#: src/humanize/time.py:152
 #, python-format
 msgid "%d microsecond"
 msgid_plural "%d microseconds"
 msgstr[0] "%d mikrosekunda"
 msgstr[1] "%d mikrosekundi"
 msgstr[2] "%d mikrosekunde"
 msgstr[3] "%d mikrosekund"
 
-#: src/humanize/time.py:147
+#: src/humanize/time.py:161
 #, python-format
 msgid "%d millisecond"
 msgid_plural "%d milliseconds"
 msgstr[0] "%d milisekunda"
 msgstr[1] "%d milisekundi"
 msgstr[2] "%d milisekunde"
 msgstr[3] "%d milisekund"
 
-#: src/humanize/time.py:150 src/humanize/time.py:231
+#: src/humanize/time.py:164 src/humanize/time.py:259
 msgid "a moment"
 msgstr "trenutek"
 
-#: src/humanize/time.py:152
+#: src/humanize/time.py:167
 msgid "a second"
 msgstr "sekunda"
 
-#: src/humanize/time.py:154
+#: src/humanize/time.py:170
 #, python-format
 msgid "%d second"
 msgid_plural "%d seconds"
 msgstr[0] "%d sekunda"
 msgstr[1] "%d sekundi"
 msgstr[2] "%d sekunde"
 msgstr[3] "%d sekund"
 
-#: src/humanize/time.py:156
+#: src/humanize/time.py:173
 msgid "a minute"
 msgstr "minuta"
 
-#: src/humanize/time.py:159
+#: src/humanize/time.py:177
 #, python-format
 msgid "%d minute"
 msgid_plural "%d minutes"
 msgstr[0] "%d minuta"
 msgstr[1] "%d minuti"
 msgstr[2] "%d minute"
 msgstr[3] "%d minut"
 
-#: src/humanize/time.py:161
+#: src/humanize/time.py:180
 msgid "an hour"
 msgstr "ura"
 
-#: src/humanize/time.py:164
+#: src/humanize/time.py:184
 #, python-format
 msgid "%d hour"
 msgid_plural "%d hours"
 msgstr[0] "%d ura"
 msgstr[1] "%d uri"
 msgstr[2] "%d ure"
 msgstr[3] "%d ur"
 
-#: src/humanize/time.py:167
+#: src/humanize/time.py:188
 msgid "a day"
 msgstr "dan"
 
-#: src/humanize/time.py:169 src/humanize/time.py:172
+#: src/humanize/time.py:191 src/humanize/time.py:194
 #, python-format
 msgid "%d day"
 msgid_plural "%d days"
 msgstr[0] "%d dan"
 msgstr[1] "%d dneva"
 msgstr[2] "%d dnevi"
 msgstr[3] "%d dni"
 
-#: src/humanize/time.py:174
+#: src/humanize/time.py:197
 msgid "a month"
 msgstr "mesec"
 
-#: src/humanize/time.py:176
+#: src/humanize/time.py:199
 #, python-format
 msgid "%d month"
 msgid_plural "%d months"
 msgstr[0] "%d mesec"
 msgstr[1] "%d meseca"
 msgstr[2] "%d meseci"
 msgstr[3] "%d mesecev"
 
-#: src/humanize/time.py:179
+#: src/humanize/time.py:203
 msgid "a year"
 msgstr "leto"
 
-#: src/humanize/time.py:181 src/humanize/time.py:190
+#: src/humanize/time.py:206 src/humanize/time.py:217
 #, python-format
 msgid "1 year, %d day"
 msgid_plural "1 year, %d days"
 msgstr[0] "1 leto, %d dan"
 msgstr[1] "1 leto, %d dneva"
 msgstr[2] "1 leto, %d dnevi"
 msgstr[3] "1 leto, %d dni"
 
-#: src/humanize/time.py:184
+#: src/humanize/time.py:210
 msgid "1 year, 1 month"
 msgstr "1 leto, 1 mesec"
 
-#: src/humanize/time.py:187
+#: src/humanize/time.py:213
 #, python-format
 msgid "1 year, %d month"
 msgid_plural "1 year, %d months"
 msgstr[0] "1 leto, %d mesec"
 msgstr[1] "1 leto, %d meseca"
 msgstr[2] "1 leto, %d meseci"
 msgstr[3] "1 leto, %d mesecev"
 
-#: src/humanize/time.py:192
+#: src/humanize/time.py:219
 #, python-format
 msgid "%d year"
 msgid_plural "%d years"
 msgstr[0] "%d leto"
 msgstr[1] "%d leti"
 msgstr[2] "%d leta"
 msgstr[3] "%d let"
 
-#: src/humanize/time.py:228
+#: src/humanize/time.py:256
 #, python-format
 msgid "%s from now"
 msgstr "%s od zdaj"
 
-#: src/humanize/time.py:228
+#: src/humanize/time.py:256
 #, python-format
 msgid "%s ago"
 msgstr "%s nazaj"
 
-#: src/humanize/time.py:232
+#: src/humanize/time.py:260
 msgid "now"
 msgstr "zdaj"
 
-#: src/humanize/time.py:255
+#: src/humanize/time.py:284
 msgid "today"
 msgstr "danes"
 
-#: src/humanize/time.py:257
+#: src/humanize/time.py:287
 msgid "tomorrow"
 msgstr "jutri"
 
-#: src/humanize/time.py:259
+#: src/humanize/time.py:290
 msgid "yesterday"
 msgstr "včeraj"
 
-#: src/humanize/time.py:545
+#: src/humanize/time.py:600
 #, python-format
 msgid "%s and %s"
 msgstr "%s in %s"
```

### Comparing `humanize-4.5.0/src/humanize/locale/sv_SE/LC_MESSAGES/humanize.mo` & `humanize-4.6.0/src/humanize/locale/sv_SE/LC_MESSAGES/humanize.mo`

 * *Files 5% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,11 +1,11 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: humanize\n"
-"Report-Msgid-Bugs-To: https://github.com/python-humanize/humanize/issues\n"
+"Report-Msgid-Bugs-To: \n"
 "PO-Revision-Date: 2021-07-05 10:30+0200\n"
 "Last-Translator: Kess Vargavind <vargavind@gmail.com>\n"
 "Language-Team: Swedish\n"
 "Language: sv\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
```

### Comparing `humanize-4.5.0/src/humanize/locale/sv_SE/LC_MESSAGES/humanize.po` & `humanize-4.6.0/src/humanize/locale/zh_CN/LC_MESSAGES/humanize.po`

 * *Files 14% similar despite different names*

```diff
@@ -1,363 +1,364 @@
-# Swedish (Sweden) translations for humanize package.
-# Copyright (C) 2021
-# This file is distributed under the same license as the humanize project.
-# Kess Vargavind <vargavind@gmail.com>, 2021.
+# Simplified Chinese (China) translation for the project
+# Copyright (C) 2016
+# This file is distributed under the same license as the PACKAGE package.
+# AZLisme <helloazl@icloud.com>, 2016.
+# Liwen SUN <sunliwen@gmail.com>, 2019.
 #
 msgid ""
 msgstr ""
-"Project-Id-Version: humanize\n"
-"Report-Msgid-Bugs-To: https://github.com/python-humanize/humanize/issues\n"
-"POT-Creation-Date: 2021-07-05 09:49+0200\n"
-"PO-Revision-Date: 2021-07-05 10:30+0200\n"
-"Last-Translator: Kess Vargavind <vargavind@gmail.com>\n"
-"Language-Team: Swedish\n"
-"Language: sv\n"
+"Project-Id-Version: 1.0\n"
+"Report-Msgid-Bugs-To: \n"
+"POT-Creation-Date: 2023-01-08 19:22+0200\n"
+"PO-Revision-Date: 2016-11-14 23:02+0000\n"
+"Last-Translator: Liwen SUN <sunliwen@gmail.com>\n"
+"Language-Team: Chinese (simplified)\n"
+"Language: zh_CN\n"
 "MIME-Version: 1.0\n"
-"Content-Type: text/plain; charset=utf-8\n"
+"Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=(n != 1);\n"
+"Plural-Forms: nplurals=2; plural=(n > 1);\n"
 
-#: src/humanize/number.py:58
+#: src/humanize/number.py:84
 msgctxt "0 (male)"
 msgid "th"
-msgstr ":e"
+msgstr "第"
 
-#: src/humanize/number.py:59
+#: src/humanize/number.py:85
 msgctxt "1 (male)"
 msgid "st"
-msgstr ":a"
+msgstr "第"
 
-#: src/humanize/number.py:60
+#: src/humanize/number.py:86
 msgctxt "2 (male)"
 msgid "nd"
-msgstr ":a"
+msgstr "第"
 
-#: src/humanize/number.py:61
+#: src/humanize/number.py:87
 msgctxt "3 (male)"
 msgid "rd"
-msgstr ":e"
+msgstr "第"
 
-#: src/humanize/number.py:62
+#: src/humanize/number.py:88
 msgctxt "4 (male)"
 msgid "th"
-msgstr ":e"
+msgstr "第"
 
-#: src/humanize/number.py:63
+#: src/humanize/number.py:89
 msgctxt "5 (male)"
 msgid "th"
-msgstr ":e"
+msgstr "第"
 
-#: src/humanize/number.py:64
+#: src/humanize/number.py:90
 msgctxt "6 (male)"
 msgid "th"
-msgstr ":e"
+msgstr "第"
 
-#: src/humanize/number.py:65
+#: src/humanize/number.py:91
 msgctxt "7 (male)"
 msgid "th"
-msgstr ":e"
+msgstr "第"
 
-#: src/humanize/number.py:66
+#: src/humanize/number.py:92
 msgctxt "8 (male)"
 msgid "th"
-msgstr ":e"
+msgstr "第"
 
-#: src/humanize/number.py:67
+#: src/humanize/number.py:93
 msgctxt "9 (male)"
 msgid "th"
-msgstr ":e"
+msgstr "第"
 
-#: src/humanize/number.py:71
+#: src/humanize/number.py:97
 msgctxt "0 (female)"
 msgid "th"
-msgstr ":e"
+msgstr "第"
 
-#: src/humanize/number.py:72
+#: src/humanize/number.py:98
 msgctxt "1 (female)"
 msgid "st"
-msgstr ":a"
+msgstr "第"
 
-#: src/humanize/number.py:73
+#: src/humanize/number.py:99
 msgctxt "2 (female)"
 msgid "nd"
-msgstr ":a"
+msgstr "第"
 
-#: src/humanize/number.py:74
+#: src/humanize/number.py:100
 msgctxt "3 (female)"
 msgid "rd"
-msgstr ":e"
+msgstr "第"
 
-#: src/humanize/number.py:75
+#: src/humanize/number.py:101
 msgctxt "4 (female)"
 msgid "th"
-msgstr ":e"
+msgstr "第"
 
-#: src/humanize/number.py:76
+#: src/humanize/number.py:102
 msgctxt "5 (female)"
 msgid "th"
-msgstr ":e"
+msgstr "第"
 
-#: src/humanize/number.py:77
+#: src/humanize/number.py:103
 msgctxt "6 (female)"
 msgid "th"
-msgstr ":e"
+msgstr "第"
 
-#: src/humanize/number.py:78
+#: src/humanize/number.py:104
 msgctxt "7 (female)"
 msgid "th"
-msgstr ":e"
+msgstr "第"
 
-#: src/humanize/number.py:79
+#: src/humanize/number.py:105
 msgctxt "8 (female)"
 msgid "th"
-msgstr ":e"
+msgstr "第"
 
-#: src/humanize/number.py:80
+#: src/humanize/number.py:106
 msgctxt "9 (female)"
 msgid "th"
-msgstr ":e"
+msgstr "第"
 
-#: src/humanize/number.py:141
+#: src/humanize/number.py:178
 msgid "thousand"
 msgid_plural "thousand"
-msgstr[0] "tusen"
-msgstr[1] "tusen"
+msgstr[0] ""
+msgstr[1] ""
 
-#: src/humanize/number.py:142
+#: src/humanize/number.py:179
 msgid "million"
 msgid_plural "million"
-msgstr[0] "miljon"
-msgstr[1] "miljoner"
+msgstr[0] "百万"
+msgstr[1] "百万"
 
-#: src/humanize/number.py:143
+#: src/humanize/number.py:180
 msgid "billion"
 msgid_plural "billion"
-msgstr[0] "miljard"
-msgstr[1] "miljarder"
+msgstr[0] "十亿"
+msgstr[1] "十亿"
 
-#: src/humanize/number.py:144
+#: src/humanize/number.py:181
 msgid "trillion"
 msgid_plural "trillion"
-msgstr[0] "biljon"
-msgstr[1] "biljoner"
+msgstr[0] "兆"
+msgstr[1] "兆"
 
-#: src/humanize/number.py:145
+#: src/humanize/number.py:182
 msgid "quadrillion"
 msgid_plural "quadrillion"
-msgstr[0] "biljard"
-msgstr[1] "biljarder"
+msgstr[0] "万亿"
+msgstr[1] "万亿"
 
-#: src/humanize/number.py:146
+#: src/humanize/number.py:183
 msgid "quintillion"
 msgid_plural "quintillion"
-msgstr[0] "triljon"
-msgstr[1] "triljoner"
+msgstr[0] "百京"
+msgstr[1] "百京"
 
-#: src/humanize/number.py:147
+#: src/humanize/number.py:184
 msgid "sextillion"
 msgid_plural "sextillion"
-msgstr[0] "triljard"
-msgstr[1] "triljarder"
+msgstr[0] "十垓"
+msgstr[1] "十垓"
 
-#: src/humanize/number.py:148
+#: src/humanize/number.py:185
 msgid "septillion"
 msgid_plural "septillion"
-msgstr[0] "kvadriljon"
-msgstr[1] "kvadriljoner"
+msgstr[0] "秭"
+msgstr[1] "秭"
 
-#: src/humanize/number.py:149
+#: src/humanize/number.py:186
 msgid "octillion"
 msgid_plural "octillion"
-msgstr[0] "kvadriljard"
-msgstr[1] "kvadriljarder"
+msgstr[0] "千秭"
+msgstr[1] "千秭"
 
-#: src/humanize/number.py:150
+#: src/humanize/number.py:187
 msgid "nonillion"
 msgid_plural "nonillion"
-msgstr[0] "kvintiljon"
-msgstr[1] "kvintiljoner"
+msgstr[0] "百穰"
+msgstr[1] "百穰"
 
-#: src/humanize/number.py:151
+#: src/humanize/number.py:188
 msgid "decillion"
 msgid_plural "decillion"
-msgstr[0] "kvintiljard"
-msgstr[1] "kvintiljarder"
+msgstr[0] "十沟"
+msgstr[1] "十沟"
 
-#: src/humanize/number.py:152
+#: src/humanize/number.py:189
 msgid "googol"
 msgid_plural "googol"
-msgstr[0] "googol"
-msgstr[1] "googol"
+msgstr[0] "古高尔"
+msgstr[1] "古高尔"
 
-#: src/humanize/number.py:247
+#: src/humanize/number.py:301
 msgid "zero"
-msgstr "noll"
+msgstr ""
 
-#: src/humanize/number.py:248
+#: src/humanize/number.py:302
 msgid "one"
-msgstr "ett"
+msgstr "一"
 
-#: src/humanize/number.py:249
+#: src/humanize/number.py:303
 msgid "two"
-msgstr "två"
+msgstr "二"
 
-#: src/humanize/number.py:250
+#: src/humanize/number.py:304
 msgid "three"
-msgstr "tre"
+msgstr "三"
 
-#: src/humanize/number.py:251
+#: src/humanize/number.py:305
 msgid "four"
-msgstr "fyra"
+msgstr "四"
 
-#: src/humanize/number.py:252
+#: src/humanize/number.py:306
 msgid "five"
-msgstr "fem"
+msgstr "五"
 
-#: src/humanize/number.py:253
+#: src/humanize/number.py:307
 msgid "six"
-msgstr "sex"
+msgstr "六"
 
-#: src/humanize/number.py:254
+#: src/humanize/number.py:308
 msgid "seven"
-msgstr "sju"
+msgstr "七"
 
-#: src/humanize/number.py:255
+#: src/humanize/number.py:309
 msgid "eight"
-msgstr "åtta"
+msgstr "八"
 
-#: src/humanize/number.py:256
+#: src/humanize/number.py:310
 msgid "nine"
-msgstr "nio"
+msgstr "九"
 
-#: src/humanize/time.py:138
+#: src/humanize/time.py:152
 #, python-format
 msgid "%d microsecond"
 msgid_plural "%d microseconds"
-msgstr[0] "%d mikrosekund"
-msgstr[1] "%d mikrosekunder"
+msgstr[0] ""
+msgstr[1] ""
 
-#: src/humanize/time.py:147
+#: src/humanize/time.py:161
 #, python-format
 msgid "%d millisecond"
 msgid_plural "%d milliseconds"
-msgstr[0] "%d millsekund"
-msgstr[1] "%d millsekunder"
+msgstr[0] ""
+msgstr[1] ""
 
-#: src/humanize/time.py:150 src/humanize/time.py:231
+#: src/humanize/time.py:164 src/humanize/time.py:259
 msgid "a moment"
-msgstr "en liten stund"
+msgstr "一会儿"
 
-#: src/humanize/time.py:152
+#: src/humanize/time.py:167
 msgid "a second"
-msgstr "en sekund"
+msgstr "1秒"
 
-#: src/humanize/time.py:154
+#: src/humanize/time.py:170
 #, python-format
 msgid "%d second"
 msgid_plural "%d seconds"
-msgstr[0] "%d sekund"
-msgstr[1] "%d sekunder"
+msgstr[0] "%d秒"
+msgstr[1] "%d秒"
 
-#: src/humanize/time.py:156
+#: src/humanize/time.py:173
 msgid "a minute"
-msgstr "en minut"
+msgstr "1分"
 
-#: src/humanize/time.py:159
+#: src/humanize/time.py:177
 #, python-format
 msgid "%d minute"
 msgid_plural "%d minutes"
-msgstr[0] "%d minut"
-msgstr[1] "%d minuter"
+msgstr[0] "%d分"
+msgstr[1] "%d分"
 
-#: src/humanize/time.py:161
+#: src/humanize/time.py:180
 msgid "an hour"
-msgstr "en timme"
+msgstr "1小时"
 
-#: src/humanize/time.py:164
+#: src/humanize/time.py:184
 #, python-format
 msgid "%d hour"
 msgid_plural "%d hours"
-msgstr[0] "%d timme"
-msgstr[1] "%d timmar"
+msgstr[0] "%d小时"
+msgstr[1] "%d小时"
 
-#: src/humanize/time.py:167
+#: src/humanize/time.py:188
 msgid "a day"
-msgstr "en dag"
+msgstr "1天"
 
-#: src/humanize/time.py:169 src/humanize/time.py:172
+#: src/humanize/time.py:191 src/humanize/time.py:194
 #, python-format
 msgid "%d day"
 msgid_plural "%d days"
-msgstr[0] "%d dag"
-msgstr[1] "%d dagar"
+msgstr[0] "%d天"
+msgstr[1] "%d天"
 
-#: src/humanize/time.py:174
+#: src/humanize/time.py:197
 msgid "a month"
-msgstr "en månad"
+msgstr "1月"
 
-#: src/humanize/time.py:176
+#: src/humanize/time.py:199
 #, python-format
 msgid "%d month"
 msgid_plural "%d months"
-msgstr[0] "%d månad"
-msgstr[1] "%d månader"
+msgstr[0] "%d月"
+msgstr[1] "%d月"
 
-#: src/humanize/time.py:179
+#: src/humanize/time.py:203
 msgid "a year"
-msgstr "ett år"
+msgstr "1年"
 
-#: src/humanize/time.py:181 src/humanize/time.py:190
+#: src/humanize/time.py:206 src/humanize/time.py:217
 #, python-format
 msgid "1 year, %d day"
 msgid_plural "1 year, %d days"
-msgstr[0] "1 år, %d dag"
-msgstr[1] "1 år, %d dagar"
+msgstr[0] "%d年"
+msgstr[1] "%d年"
 
-#: src/humanize/time.py:184
+#: src/humanize/time.py:210
 msgid "1 year, 1 month"
-msgstr "1 år, 1 månad"
+msgstr "1年又1月"
 
-#: src/humanize/time.py:187
+#: src/humanize/time.py:213
 #, python-format
 msgid "1 year, %d month"
 msgid_plural "1 year, %d months"
-msgstr[0] "1 år, %d månad"
-msgstr[1] "1 år, %d månader"
+msgstr[0] "1年又%d月"
+msgstr[1] "1年又%d月"
 
-#: src/humanize/time.py:192
+#: src/humanize/time.py:219
 #, python-format
 msgid "%d year"
 msgid_plural "%d years"
-msgstr[0] "%d år"
-msgstr[1] "%d år"
+msgstr[0] "%d年"
+msgstr[1] "%d年"
 
-#: src/humanize/time.py:228
+#: src/humanize/time.py:256
 #, python-format
 msgid "%s from now"
-msgstr "%s från nu"
+msgstr "%s之后"
 
-#: src/humanize/time.py:228
+#: src/humanize/time.py:256
 #, python-format
 msgid "%s ago"
-msgstr "%s sedan"
+msgstr "%s之前"
 
-#: src/humanize/time.py:232
+#: src/humanize/time.py:260
 msgid "now"
-msgstr "nu"
+msgstr "现在"
 
-#: src/humanize/time.py:255
+#: src/humanize/time.py:284
 msgid "today"
-msgstr "idag"
+msgstr "今天"
 
-#: src/humanize/time.py:257
+#: src/humanize/time.py:287
 msgid "tomorrow"
-msgstr "imorgon"
+msgstr "明天"
 
-#: src/humanize/time.py:259
+#: src/humanize/time.py:290
 msgid "yesterday"
-msgstr "igår"
+msgstr "昨天"
 
-#: src/humanize/time.py:545
+#: src/humanize/time.py:600
 #, python-format
 msgid "%s and %s"
-msgstr "%s och %s"
+msgstr ""
```

### Comparing `humanize-4.5.0/src/humanize/locale/tr_TR/LC_MESSAGES/humanize.mo` & `humanize-4.6.0/src/humanize/locale/tr_TR/LC_MESSAGES/humanize.mo`

 * *Files identical despite different names*

### Comparing `humanize-4.5.0/src/humanize/locale/tr_TR/LC_MESSAGES/humanize.po` & `humanize-4.6.0/src/humanize/locale/tr_TR/LC_MESSAGES/humanize.po`

 * *Files 5% similar despite different names*

```diff
@@ -3,363 +3,363 @@
 # This file is distributed under the same license as the humanize package.
 # Emre Çintay <emre@cintay.com>, 2017.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: humanize\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2021-05-04 23:15+0200\n"
+"POT-Creation-Date: 2023-01-08 19:22+0200\n"
 "PO-Revision-Date: 2017-02-23 20:00+0300\n"
 "Last-Translator: Emre Çintay <emre@cintay.com>\n"
 "Language-Team: Turkish\n"
 "Language: tr_TR\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "X-Generator: Poedit 1.8.7.1\n"
 "Generated-By: Emre Çintay\n"
 
-#: src/humanize/number.py:57
+#: src/humanize/number.py:84
 msgctxt "0 (male)"
 msgid "th"
 msgstr "."
 
-#: src/humanize/number.py:58
+#: src/humanize/number.py:85
 msgctxt "1 (male)"
 msgid "st"
 msgstr "."
 
-#: src/humanize/number.py:59
+#: src/humanize/number.py:86
 msgctxt "2 (male)"
 msgid "nd"
 msgstr "."
 
-#: src/humanize/number.py:60
+#: src/humanize/number.py:87
 msgctxt "3 (male)"
 msgid "rd"
 msgstr "."
 
-#: src/humanize/number.py:61
+#: src/humanize/number.py:88
 msgctxt "4 (male)"
 msgid "th"
 msgstr "."
 
-#: src/humanize/number.py:62
+#: src/humanize/number.py:89
 msgctxt "5 (male)"
 msgid "th"
 msgstr "."
 
-#: src/humanize/number.py:63
+#: src/humanize/number.py:90
 msgctxt "6 (male)"
 msgid "th"
 msgstr "."
 
-#: src/humanize/number.py:64
+#: src/humanize/number.py:91
 msgctxt "7 (male)"
 msgid "th"
 msgstr "."
 
-#: src/humanize/number.py:65
+#: src/humanize/number.py:92
 msgctxt "8 (male)"
 msgid "th"
 msgstr "."
 
-#: src/humanize/number.py:66
+#: src/humanize/number.py:93
 msgctxt "9 (male)"
 msgid "th"
 msgstr "."
 
-#: src/humanize/number.py:70
+#: src/humanize/number.py:97
 msgctxt "0 (female)"
 msgid "th"
 msgstr "."
 
-#: src/humanize/number.py:71
+#: src/humanize/number.py:98
 msgctxt "1 (female)"
 msgid "st"
 msgstr "."
 
-#: src/humanize/number.py:72
+#: src/humanize/number.py:99
 msgctxt "2 (female)"
 msgid "nd"
 msgstr "."
 
-#: src/humanize/number.py:73
+#: src/humanize/number.py:100
 msgctxt "3 (female)"
 msgid "rd"
 msgstr "."
 
-#: src/humanize/number.py:74
+#: src/humanize/number.py:101
 msgctxt "4 (female)"
 msgid "th"
 msgstr "."
 
-#: src/humanize/number.py:75
+#: src/humanize/number.py:102
 msgctxt "5 (female)"
 msgid "th"
 msgstr "."
 
-#: src/humanize/number.py:76
+#: src/humanize/number.py:103
 msgctxt "6 (female)"
 msgid "th"
 msgstr "."
 
-#: src/humanize/number.py:77
+#: src/humanize/number.py:104
 msgctxt "7 (female)"
 msgid "th"
 msgstr "."
 
-#: src/humanize/number.py:78
+#: src/humanize/number.py:105
 msgctxt "8 (female)"
 msgid "th"
 msgstr "."
 
-#: src/humanize/number.py:79
+#: src/humanize/number.py:106
 msgctxt "9 (female)"
 msgid "th"
 msgstr "."
 
-#: src/humanize/number.py:140
+#: src/humanize/number.py:178
 msgid "thousand"
 msgid_plural "thousand"
 msgstr[0] ""
 msgstr[1] ""
 
-#: src/humanize/number.py:141
+#: src/humanize/number.py:179
 msgid "million"
 msgid_plural "million"
 msgstr[0] "milyon"
 msgstr[1] "milyon"
 
-#: src/humanize/number.py:142
+#: src/humanize/number.py:180
 msgid "billion"
 msgid_plural "billion"
 msgstr[0] "milyar"
 msgstr[1] "milyar"
 
-#: src/humanize/number.py:143
+#: src/humanize/number.py:181
 msgid "trillion"
 msgid_plural "trillion"
 msgstr[0] "trilyon"
 msgstr[1] "trilyon"
 
-#: src/humanize/number.py:144
+#: src/humanize/number.py:182
 msgid "quadrillion"
 msgid_plural "quadrillion"
 msgstr[0] "katrilyon"
 msgstr[1] "katrilyon"
 
-#: src/humanize/number.py:145
+#: src/humanize/number.py:183
 msgid "quintillion"
 msgid_plural "quintillion"
 msgstr[0] "kentilyon"
 msgstr[1] "kentilyon"
 
-#: src/humanize/number.py:146
+#: src/humanize/number.py:184
 msgid "sextillion"
 msgid_plural "sextillion"
 msgstr[0] "sekstilyon"
 msgstr[1] "sekstilyon"
 
-#: src/humanize/number.py:147
+#: src/humanize/number.py:185
 msgid "septillion"
 msgid_plural "septillion"
 msgstr[0] "septilyon"
 msgstr[1] "septilyon"
 
-#: src/humanize/number.py:148
+#: src/humanize/number.py:186
 msgid "octillion"
 msgid_plural "octillion"
 msgstr[0] "oktilyon"
 msgstr[1] "oktilyon"
 
-#: src/humanize/number.py:149
+#: src/humanize/number.py:187
 msgid "nonillion"
 msgid_plural "nonillion"
 msgstr[0] "nonilyon"
 msgstr[1] "nonilyon"
 
-#: src/humanize/number.py:150
+#: src/humanize/number.py:188
 msgid "decillion"
 msgid_plural "decillion"
 msgstr[0] "desilyon"
 msgstr[1] "desilyon"
 
-#: src/humanize/number.py:151
+#: src/humanize/number.py:189
 msgid "googol"
 msgid_plural "googol"
 msgstr[0] "googol"
 msgstr[1] "googol"
 
-#: src/humanize/number.py:246
+#: src/humanize/number.py:301
 msgid "zero"
 msgstr ""
 
-#: src/humanize/number.py:247
+#: src/humanize/number.py:302
 msgid "one"
 msgstr "bir"
 
-#: src/humanize/number.py:248
+#: src/humanize/number.py:303
 msgid "two"
 msgstr "iki"
 
-#: src/humanize/number.py:249
+#: src/humanize/number.py:304
 msgid "three"
 msgstr "üç"
 
-#: src/humanize/number.py:250
+#: src/humanize/number.py:305
 msgid "four"
 msgstr "dört"
 
-#: src/humanize/number.py:251
+#: src/humanize/number.py:306
 msgid "five"
 msgstr "beş"
 
-#: src/humanize/number.py:252
+#: src/humanize/number.py:307
 msgid "six"
 msgstr "altı"
 
-#: src/humanize/number.py:253
+#: src/humanize/number.py:308
 msgid "seven"
 msgstr "yedi"
 
-#: src/humanize/number.py:254
+#: src/humanize/number.py:309
 msgid "eight"
 msgstr "sekiz"
 
-#: src/humanize/number.py:255
+#: src/humanize/number.py:310
 msgid "nine"
 msgstr "dokuz"
 
-#: src/humanize/time.py:133
+#: src/humanize/time.py:152
 #, python-format
 msgid "%d microsecond"
 msgid_plural "%d microseconds"
 msgstr[0] ""
 msgstr[1] ""
 
-#: src/humanize/time.py:142
+#: src/humanize/time.py:161
 #, python-format
 msgid "%d millisecond"
 msgid_plural "%d milliseconds"
 msgstr[0] ""
 msgstr[1] ""
 
-#: src/humanize/time.py:145 src/humanize/time.py:220
+#: src/humanize/time.py:164 src/humanize/time.py:259
 msgid "a moment"
 msgstr "biraz"
 
-#: src/humanize/time.py:147
+#: src/humanize/time.py:167
 msgid "a second"
 msgstr "bir saniye"
 
-#: src/humanize/time.py:149
+#: src/humanize/time.py:170
 #, python-format
 msgid "%d second"
 msgid_plural "%d seconds"
 msgstr[0] "%d saniye"
 msgstr[1] "%d saniye"
 
-#: src/humanize/time.py:151
+#: src/humanize/time.py:173
 msgid "a minute"
 msgstr "bir dakika"
 
-#: src/humanize/time.py:154
+#: src/humanize/time.py:177
 #, python-format
 msgid "%d minute"
 msgid_plural "%d minutes"
 msgstr[0] "%d dakika"
 msgstr[1] "%d dakika"
 
-#: src/humanize/time.py:156
+#: src/humanize/time.py:180
 msgid "an hour"
 msgstr "bir saat"
 
-#: src/humanize/time.py:159
+#: src/humanize/time.py:184
 #, python-format
 msgid "%d hour"
 msgid_plural "%d hours"
 msgstr[0] "%d saat"
 msgstr[1] "%d saat"
 
-#: src/humanize/time.py:162
+#: src/humanize/time.py:188
 msgid "a day"
 msgstr "bir gün"
 
-#: src/humanize/time.py:164 src/humanize/time.py:167
+#: src/humanize/time.py:191 src/humanize/time.py:194
 #, python-format
 msgid "%d day"
 msgid_plural "%d days"
 msgstr[0] "%d gün"
 msgstr[1] "%d gün"
 
-#: src/humanize/time.py:169
+#: src/humanize/time.py:197
 msgid "a month"
 msgstr "bir ay"
 
-#: src/humanize/time.py:171
+#: src/humanize/time.py:199
 #, python-format
 msgid "%d month"
 msgid_plural "%d months"
 msgstr[0] "%d ay"
 msgstr[1] "%d ay"
 
-#: src/humanize/time.py:174
+#: src/humanize/time.py:203
 msgid "a year"
 msgstr "bir yıl"
 
-#: src/humanize/time.py:176 src/humanize/time.py:185
+#: src/humanize/time.py:206 src/humanize/time.py:217
 #, python-format
 msgid "1 year, %d day"
 msgid_plural "1 year, %d days"
 msgstr[0] "1 yıl, %d gün"
 msgstr[1] "1 yıl, %d gün"
 
-#: src/humanize/time.py:179
+#: src/humanize/time.py:210
 msgid "1 year, 1 month"
 msgstr "1 yıl, 1 ay"
 
-#: src/humanize/time.py:182
+#: src/humanize/time.py:213
 #, python-format
 msgid "1 year, %d month"
 msgid_plural "1 year, %d months"
 msgstr[0] "1 yıl, %d ay"
 msgstr[1] "1 yıl, %d ay"
 
-#: src/humanize/time.py:187
+#: src/humanize/time.py:219
 #, python-format
 msgid "%d year"
 msgid_plural "%d years"
 msgstr[0] "%d yıl"
 msgstr[1] "%d yıl"
 
-#: src/humanize/time.py:217
+#: src/humanize/time.py:256
 #, python-format
 msgid "%s from now"
 msgstr "şu andan itibaren %s"
 
-#: src/humanize/time.py:217
+#: src/humanize/time.py:256
 #, python-format
 msgid "%s ago"
 msgstr "%s önce"
 
-#: src/humanize/time.py:221
+#: src/humanize/time.py:260
 msgid "now"
 msgstr "şimdi"
 
-#: src/humanize/time.py:244
+#: src/humanize/time.py:284
 msgid "today"
 msgstr "bugün"
 
-#: src/humanize/time.py:246
+#: src/humanize/time.py:287
 msgid "tomorrow"
 msgstr "yarın"
 
-#: src/humanize/time.py:248
+#: src/humanize/time.py:290
 msgid "yesterday"
 msgstr "dün"
 
-#: src/humanize/time.py:534
+#: src/humanize/time.py:600
 #, python-format
 msgid "%s and %s"
 msgstr ""
```

### Comparing `humanize-4.5.0/src/humanize/locale/uk_UA/LC_MESSAGES/humanize.mo` & `humanize-4.6.0/src/humanize/locale/uk_UA/LC_MESSAGES/humanize.mo`

 * *Files identical despite different names*

### Comparing `humanize-4.5.0/src/humanize/locale/vi_VN/LC_MESSAGES/humanize.mo` & `humanize-4.6.0/src/humanize/locale/vi_VN/LC_MESSAGES/humanize.mo`

 * *Files identical despite different names*

### Comparing `humanize-4.5.0/src/humanize/locale/vi_VN/LC_MESSAGES/humanize.po` & `humanize-4.6.0/src/humanize/locale/ca_ES/LC_MESSAGES/humanize.po`

 * *Files 17% similar despite different names*

```diff
@@ -1,372 +1,363 @@
-# Vietnamese (Vietnam) translations for PROJECT.
-# Copyright (C) 2013 ORGANIZATION
-# This file is distributed under the same license as the PROJECT project.
-# FIRST AUTHOR <EMAIL@ADDRESS>, 2013.
+# Catalan translations for PACKAGE package
+# This file is distributed under the same license as the PACKAGE package.
+# Jordi Mas i Hernàndez <jmas@softcatala.org>, 2021
 #
 msgid ""
 msgstr ""
-"Project-Id-Version: PROJECT VERSION\n"
+"Project-Id-Version: humanize\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2021-05-04 23:15+0200\n"
-"PO-Revision-Date: 2017-05-30 11:51+0700\n"
-"Last-Translator: Olivier Cortès <oc@1flow.io>\n"
-"Language-Team: vi_VI <sapd@vccloud.vn>\n"
-"Language: vi_VN\n"
+"POT-Creation-Date: 2023-01-08 19:22+0200\n"
+"PO-Revision-Date: 2021-04-09 19:57+0200\n"
+"Last-Translator: Jordi Mas i Hernàndez <jmas@softcatala.org>\n"
+"Language-Team: Catalan\n"
+"Language: ca\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=(n > 1);\n"
-"Generated-By: Babel 0.9.6\n"
-"X-Generator: Poedit 1.8.7.1\n"
+"Plural-Forms: nplurals=2; plural=n!=1;\n"
+"X-Generator: Poedit 2.4.1\n"
 
-#: src/humanize/number.py:57
+#: src/humanize/number.py:84
 msgctxt "0 (male)"
 msgid "th"
-msgstr "."
+msgstr "º"
 
-#: src/humanize/number.py:58
+#: src/humanize/number.py:85
 msgctxt "1 (male)"
 msgid "st"
-msgstr "."
+msgstr "º"
 
-#: src/humanize/number.py:59
+#: src/humanize/number.py:86
 msgctxt "2 (male)"
 msgid "nd"
-msgstr "."
+msgstr "º"
 
-#: src/humanize/number.py:60
+#: src/humanize/number.py:87
 msgctxt "3 (male)"
 msgid "rd"
-msgstr "."
+msgstr "º"
 
-#: src/humanize/number.py:61
+#: src/humanize/number.py:88
 msgctxt "4 (male)"
 msgid "th"
-msgstr "."
+msgstr "º"
 
-#: src/humanize/number.py:62
+#: src/humanize/number.py:89
 msgctxt "5 (male)"
 msgid "th"
-msgstr "."
+msgstr "º"
 
-#: src/humanize/number.py:63
+#: src/humanize/number.py:90
 msgctxt "6 (male)"
 msgid "th"
-msgstr "."
+msgstr "º"
 
-#: src/humanize/number.py:64
+#: src/humanize/number.py:91
 msgctxt "7 (male)"
 msgid "th"
-msgstr "."
+msgstr "º"
 
-#: src/humanize/number.py:65
+#: src/humanize/number.py:92
 msgctxt "8 (male)"
 msgid "th"
-msgstr "."
+msgstr "º"
 
-#: src/humanize/number.py:66
+#: src/humanize/number.py:93
 msgctxt "9 (male)"
 msgid "th"
-msgstr "."
+msgstr "º"
 
-#: src/humanize/number.py:70
+#: src/humanize/number.py:97
 msgctxt "0 (female)"
 msgid "th"
-msgstr "."
+msgstr "º"
 
-#: src/humanize/number.py:71
+#: src/humanize/number.py:98
 msgctxt "1 (female)"
 msgid "st"
-msgstr "."
+msgstr "º"
 
-#: src/humanize/number.py:72
+#: src/humanize/number.py:99
 msgctxt "2 (female)"
 msgid "nd"
-msgstr "."
+msgstr "º"
 
-#: src/humanize/number.py:73
+#: src/humanize/number.py:100
 msgctxt "3 (female)"
 msgid "rd"
-msgstr "."
+msgstr "º"
 
-#: src/humanize/number.py:74
+#: src/humanize/number.py:101
 msgctxt "4 (female)"
 msgid "th"
-msgstr "."
+msgstr "º"
 
-#: src/humanize/number.py:75
+#: src/humanize/number.py:102
 msgctxt "5 (female)"
 msgid "th"
-msgstr "."
+msgstr "º"
 
-#: src/humanize/number.py:76
+#: src/humanize/number.py:103
 msgctxt "6 (female)"
 msgid "th"
-msgstr "."
+msgstr "º"
 
-#: src/humanize/number.py:77
+#: src/humanize/number.py:104
 msgctxt "7 (female)"
 msgid "th"
-msgstr "."
+msgstr "º"
 
-#: src/humanize/number.py:78
+#: src/humanize/number.py:105
 msgctxt "8 (female)"
 msgid "th"
-msgstr "."
+msgstr "º"
 
-#: src/humanize/number.py:79
+#: src/humanize/number.py:106
 msgctxt "9 (female)"
 msgid "th"
-msgstr "."
+msgstr "º"
 
-#: src/humanize/number.py:140
+#: src/humanize/number.py:178
 msgid "thousand"
 msgid_plural "thousand"
-msgstr[0] "nghìn"
-msgstr[1] "nghìn"
+msgstr[0] ""
+msgstr[1] ""
 
-#: src/humanize/number.py:141
+#: src/humanize/number.py:179
 msgid "million"
 msgid_plural "million"
-msgstr[0] "%(value)s triệu"
-msgstr[1] "%(value)s triệu"
+msgstr[0] "milió"
+msgstr[1] "milió"
 
-#: src/humanize/number.py:142
+#: src/humanize/number.py:180
 msgid "billion"
 msgid_plural "billion"
-msgstr[0] "tỷ"
-msgstr[1] "tỷ"
+msgstr[0] "mil milions"
+msgstr[1] "mil milions"
 
-#: src/humanize/number.py:143
+#: src/humanize/number.py:181
 msgid "trillion"
 msgid_plural "trillion"
-msgstr[0] "%(value)s nghìn tỷ"
-msgstr[1] "%(value)s nghìn tỷ"
+msgstr[0] "bilions"
+msgstr[1] "bilions"
 
-#: src/humanize/number.py:144
+#: src/humanize/number.py:182
 msgid "quadrillion"
 msgid_plural "quadrillion"
-msgstr[0] "%(value)s triệu tỷ"
-msgstr[1] "%(value)s triệu tỷ"
+msgstr[0] "quadrilió"
+msgstr[1] "quadrilió"
 
-#: src/humanize/number.py:145
-#, fuzzy
+#: src/humanize/number.py:183
 msgid "quintillion"
 msgid_plural "quintillion"
-msgstr[0] "%(value)s tỷ tỷ"
-msgstr[1] "%(value)s tỷ tỷ"
+msgstr[0] "quintillió"
+msgstr[1] "quintillió"
 
-#: src/humanize/number.py:146
-#, fuzzy
+#: src/humanize/number.py:184
 msgid "sextillion"
 msgid_plural "sextillion"
-msgstr[0] "%(value)s sextillion"
-msgstr[1] "%(value)s sextillion"
+msgstr[0] "sextilió"
+msgstr[1] "sextilió"
 
-#: src/humanize/number.py:147
-#, fuzzy
+#: src/humanize/number.py:185
 msgid "septillion"
 msgid_plural "septillion"
-msgstr[0] "%(value)s septillion"
-msgstr[1] "%(value)s septillion"
+msgstr[0] "septilió"
+msgstr[1] "septilió"
 
-#: src/humanize/number.py:148
-#, fuzzy
+#: src/humanize/number.py:186
 msgid "octillion"
 msgid_plural "octillion"
-msgstr[0] "%(value)s octillion"
-msgstr[1] "%(value)s octillion"
+msgstr[0] "octilió"
+msgstr[1] "octilió"
 
-#: src/humanize/number.py:149
-#, fuzzy
+#: src/humanize/number.py:187
 msgid "nonillion"
 msgid_plural "nonillion"
-msgstr[0] "%(value)s nonillion"
-msgstr[1] "%(value)s nonillion"
+msgstr[0] "nonilió"
+msgstr[1] "nonilió"
 
-#: src/humanize/number.py:150
-#, fuzzy
+#: src/humanize/number.py:188
 msgid "decillion"
 msgid_plural "decillion"
-msgstr[0] "%(value)s décillion"
-msgstr[1] "%(value)s décillion"
+msgstr[0] "decilió"
+msgstr[1] "decilió"
 
-#: src/humanize/number.py:151
-#, fuzzy
+#: src/humanize/number.py:189
 msgid "googol"
 msgid_plural "googol"
-msgstr[0] "%(value)s gogol"
-msgstr[1] "%(value)s gogol"
+msgstr[0] "googol"
+msgstr[1] "googol"
 
-#: src/humanize/number.py:246
+#: src/humanize/number.py:301
 msgid "zero"
-msgstr "không"
+msgstr "zero"
 
-#: src/humanize/number.py:247
+#: src/humanize/number.py:302
 msgid "one"
-msgstr "một"
+msgstr "un"
 
-#: src/humanize/number.py:248
+#: src/humanize/number.py:303
 msgid "two"
-msgstr "hai"
+msgstr "dos"
 
-#: src/humanize/number.py:249
+#: src/humanize/number.py:304
 msgid "three"
-msgstr "ba"
+msgstr "tres"
 
-#: src/humanize/number.py:250
+#: src/humanize/number.py:305
 msgid "four"
-msgstr "bốn"
+msgstr "quatre"
 
-#: src/humanize/number.py:251
+#: src/humanize/number.py:306
 msgid "five"
-msgstr "năm"
+msgstr "cinc"
 
-#: src/humanize/number.py:252
+#: src/humanize/number.py:307
 msgid "six"
-msgstr "sáu"
+msgstr "sis"
 
-#: src/humanize/number.py:253
+#: src/humanize/number.py:308
 msgid "seven"
-msgstr "bảy"
+msgstr "set"
 
-#: src/humanize/number.py:254
+#: src/humanize/number.py:309
 msgid "eight"
-msgstr "tám"
+msgstr "vuit"
 
-#: src/humanize/number.py:255
+#: src/humanize/number.py:310
 msgid "nine"
-msgstr "chín"
+msgstr "nou"
 
-#: src/humanize/time.py:133
+#: src/humanize/time.py:152
 #, python-format
 msgid "%d microsecond"
 msgid_plural "%d microseconds"
-msgstr[0] "%d micro giây"
-msgstr[1] "%d micro giây"
+msgstr[0] "%d microsegon"
+msgstr[1] "%d microsegons"
 
-#: src/humanize/time.py:142
+#: src/humanize/time.py:161
 #, python-format
 msgid "%d millisecond"
 msgid_plural "%d milliseconds"
-msgstr[0] "%d mili giây"
-msgstr[1] "%d mili giây"
+msgstr[0] "%d mil·lisegons"
+msgstr[1] "%d mil·lisegons"
 
-#: src/humanize/time.py:145 src/humanize/time.py:220
+#: src/humanize/time.py:164 src/humanize/time.py:259
 msgid "a moment"
-msgstr "ngay lúc này"
+msgstr "un moment"
 
-#: src/humanize/time.py:147
+#: src/humanize/time.py:167
 msgid "a second"
-msgstr "một giây"
+msgstr "un segon"
 
-#: src/humanize/time.py:149
+#: src/humanize/time.py:170
 #, python-format
 msgid "%d second"
 msgid_plural "%d seconds"
-msgstr[0] "%d giây"
-msgstr[1] "%d giây"
+msgstr[0] "%d segon"
+msgstr[1] "%d segons"
 
-#: src/humanize/time.py:151
+#: src/humanize/time.py:173
 msgid "a minute"
-msgstr "một phút"
+msgstr "un minut"
 
-#: src/humanize/time.py:154
+#: src/humanize/time.py:177
 #, python-format
 msgid "%d minute"
 msgid_plural "%d minutes"
-msgstr[0] "%d phút"
-msgstr[1] "%d phút"
+msgstr[0] "%d minut"
+msgstr[1] "%d minuts"
 
-#: src/humanize/time.py:156
+#: src/humanize/time.py:180
 msgid "an hour"
-msgstr "một giờ"
+msgstr "una hora"
 
-#: src/humanize/time.py:159
+#: src/humanize/time.py:184
 #, python-format
 msgid "%d hour"
 msgid_plural "%d hours"
-msgstr[0] "%d giờ"
-msgstr[1] "%d giờ"
+msgstr[0] "%d hora"
+msgstr[1] "%d hores"
 
-#: src/humanize/time.py:162
+#: src/humanize/time.py:188
 msgid "a day"
-msgstr "một ngày"
+msgstr "un dia"
 
-#: src/humanize/time.py:164 src/humanize/time.py:167
+#: src/humanize/time.py:191 src/humanize/time.py:194
 #, python-format
 msgid "%d day"
 msgid_plural "%d days"
-msgstr[0] "%d ngày"
-msgstr[1] "%d ngày"
+msgstr[0] "%d dia"
+msgstr[1] "%d dies"
 
-#: src/humanize/time.py:169
+#: src/humanize/time.py:197
 msgid "a month"
-msgstr "một tháng"
+msgstr "un mes"
 
-#: src/humanize/time.py:171
+#: src/humanize/time.py:199
 #, python-format
 msgid "%d month"
 msgid_plural "%d months"
-msgstr[0] "%d tháng"
-msgstr[1] "%d tháng"
+msgstr[0] "%d mes"
+msgstr[1] "%d mesos"
 
-#: src/humanize/time.py:174
+#: src/humanize/time.py:203
 msgid "a year"
-msgstr "một năm"
+msgstr "un any"
 
-#: src/humanize/time.py:176 src/humanize/time.py:185
+#: src/humanize/time.py:206 src/humanize/time.py:217
 #, python-format
 msgid "1 year, %d day"
 msgid_plural "1 year, %d days"
-msgstr[0] "1 năm %d ngày"
-msgstr[1] "1 năm %d ngày"
+msgstr[0] "1 any, %d dia"
+msgstr[1] "1 any, %d dies"
 
-#: src/humanize/time.py:179
+#: src/humanize/time.py:210
 msgid "1 year, 1 month"
-msgstr "1 năm 1 tháng"
+msgstr "1 any, 1 mes"
 
-#: src/humanize/time.py:182
+#: src/humanize/time.py:213
 #, python-format
 msgid "1 year, %d month"
 msgid_plural "1 year, %d months"
-msgstr[0] "1 năm %d tháng"
-msgstr[1] "un an et %d mois"
+msgstr[0] "1 any, %d mes"
+msgstr[1] "1 any, %d mesos"
 
-#: src/humanize/time.py:187
+#: src/humanize/time.py:219
 #, python-format
 msgid "%d year"
 msgid_plural "%d years"
-msgstr[0] "%d năm"
-msgstr[1] "%d năm"
+msgstr[0] "%d any"
+msgstr[1] "%d anys"
 
-#: src/humanize/time.py:217
+#: src/humanize/time.py:256
 #, python-format
 msgid "%s from now"
-msgstr "%s ngày tới"
+msgstr "en %s"
 
-#: src/humanize/time.py:217
+#: src/humanize/time.py:256
 #, python-format
 msgid "%s ago"
-msgstr "%s trước"
+msgstr "fa %s"
 
-#: src/humanize/time.py:221
+#: src/humanize/time.py:260
 msgid "now"
-msgstr "ngay bây giờ"
+msgstr "ara"
 
-#: src/humanize/time.py:244
+#: src/humanize/time.py:284
 msgid "today"
-msgstr "hôm nay"
+msgstr "avui"
 
-#: src/humanize/time.py:246
+#: src/humanize/time.py:287
 msgid "tomorrow"
-msgstr "ngày mai"
+msgstr "demà"
 
-#: src/humanize/time.py:248
+#: src/humanize/time.py:290
 msgid "yesterday"
-msgstr "ngày hôm qua"
+msgstr "ahir"
 
-#: src/humanize/time.py:534
+#: src/humanize/time.py:600
 #, python-format
 msgid "%s and %s"
-msgstr "%s và %s"
+msgstr "%s i %s"
```

### Comparing `humanize-4.5.0/src/humanize/locale/zh_CN/LC_MESSAGES/humanize.mo` & `humanize-4.6.0/src/humanize/locale/zh_CN/LC_MESSAGES/humanize.mo`

 * *Files identical despite different names*

### Comparing `humanize-4.5.0/src/humanize/locale/zh_CN/LC_MESSAGES/humanize.po` & `humanize-4.6.0/src/humanize/locale/pt_BR/LC_MESSAGES/humanize.po`

 * *Files 7% similar despite different names*

```diff
@@ -1,364 +1,364 @@
-# Simplified Chinese (China) translation for the project
-# Copyright (C) 2016
+# SOME DESCRIPTIVE TITLE.
+# Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
-# AZLisme <helloazl@icloud.com>, 2016.
-# Liwen SUN <sunliwen@gmail.com>, 2019.
+# FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
-"Project-Id-Version: 1.0\n"
+"Project-Id-Version: \n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2021-05-04 23:15+0200\n"
-"PO-Revision-Date: 2016-11-14 23:02+0000\n"
-"Last-Translator: Liwen SUN <sunliwen@gmail.com>\n"
-"Language-Team: Chinese (simplified)\n"
-"Language: zh_CN\n"
+"POT-Creation-Date: 2023-01-08 19:22+0200\n"
+"PO-Revision-Date: 2016-06-15 15:58-0300\n"
+"Last-Translator: \n"
+"Language-Team: \n"
+"Language: pt_BR\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n > 1);\n"
+"X-Generator: Poedit 1.8.5\n"
 
-#: src/humanize/number.py:57
+#: src/humanize/number.py:84
 msgctxt "0 (male)"
 msgid "th"
-msgstr "第"
+msgstr "º"
 
-#: src/humanize/number.py:58
+#: src/humanize/number.py:85
 msgctxt "1 (male)"
 msgid "st"
-msgstr "第"
+msgstr "º"
 
-#: src/humanize/number.py:59
+#: src/humanize/number.py:86
 msgctxt "2 (male)"
 msgid "nd"
-msgstr "第"
+msgstr "º"
 
-#: src/humanize/number.py:60
+#: src/humanize/number.py:87
 msgctxt "3 (male)"
 msgid "rd"
-msgstr "第"
+msgstr "º"
 
-#: src/humanize/number.py:61
+#: src/humanize/number.py:88
 msgctxt "4 (male)"
 msgid "th"
-msgstr "第"
+msgstr "º"
 
-#: src/humanize/number.py:62
+#: src/humanize/number.py:89
 msgctxt "5 (male)"
 msgid "th"
-msgstr "第"
+msgstr "º"
 
-#: src/humanize/number.py:63
+#: src/humanize/number.py:90
 msgctxt "6 (male)"
 msgid "th"
-msgstr "第"
+msgstr "º"
 
-#: src/humanize/number.py:64
+#: src/humanize/number.py:91
 msgctxt "7 (male)"
 msgid "th"
-msgstr "第"
+msgstr "º"
 
-#: src/humanize/number.py:65
+#: src/humanize/number.py:92
 msgctxt "8 (male)"
 msgid "th"
-msgstr "第"
+msgstr "º"
 
-#: src/humanize/number.py:66
+#: src/humanize/number.py:93
 msgctxt "9 (male)"
 msgid "th"
-msgstr "第"
+msgstr "º"
 
-#: src/humanize/number.py:70
+#: src/humanize/number.py:97
 msgctxt "0 (female)"
 msgid "th"
-msgstr "第"
+msgstr "ª"
 
-#: src/humanize/number.py:71
+#: src/humanize/number.py:98
 msgctxt "1 (female)"
 msgid "st"
-msgstr "第"
+msgstr "ª"
 
-#: src/humanize/number.py:72
+#: src/humanize/number.py:99
 msgctxt "2 (female)"
 msgid "nd"
-msgstr "第"
+msgstr "ª"
 
-#: src/humanize/number.py:73
+#: src/humanize/number.py:100
 msgctxt "3 (female)"
 msgid "rd"
-msgstr "第"
+msgstr "ª"
 
-#: src/humanize/number.py:74
+#: src/humanize/number.py:101
 msgctxt "4 (female)"
 msgid "th"
-msgstr "第"
+msgstr "ª"
 
-#: src/humanize/number.py:75
+#: src/humanize/number.py:102
 msgctxt "5 (female)"
 msgid "th"
-msgstr "第"
+msgstr "ª"
 
-#: src/humanize/number.py:76
+#: src/humanize/number.py:103
 msgctxt "6 (female)"
 msgid "th"
-msgstr "第"
+msgstr "ª"
 
-#: src/humanize/number.py:77
+#: src/humanize/number.py:104
 msgctxt "7 (female)"
 msgid "th"
-msgstr "第"
+msgstr "ª"
 
-#: src/humanize/number.py:78
+#: src/humanize/number.py:105
 msgctxt "8 (female)"
 msgid "th"
-msgstr "第"
+msgstr "ª"
 
-#: src/humanize/number.py:79
+#: src/humanize/number.py:106
 msgctxt "9 (female)"
 msgid "th"
-msgstr "第"
+msgstr "ª"
 
-#: src/humanize/number.py:140
+#: src/humanize/number.py:178
 msgid "thousand"
 msgid_plural "thousand"
 msgstr[0] ""
 msgstr[1] ""
 
-#: src/humanize/number.py:141
+#: src/humanize/number.py:179
 msgid "million"
 msgid_plural "million"
-msgstr[0] "百万"
-msgstr[1] "百万"
+msgstr[0] "milhão"
+msgstr[1] "milhão"
 
-#: src/humanize/number.py:142
+#: src/humanize/number.py:180
 msgid "billion"
 msgid_plural "billion"
-msgstr[0] "十亿"
-msgstr[1] "十亿"
+msgstr[0] "bilhão"
+msgstr[1] "bilhão"
 
-#: src/humanize/number.py:143
+#: src/humanize/number.py:181
 msgid "trillion"
 msgid_plural "trillion"
-msgstr[0] "兆"
-msgstr[1] "兆"
+msgstr[0] "trilhão"
+msgstr[1] "trilhão"
 
-#: src/humanize/number.py:144
+#: src/humanize/number.py:182
 msgid "quadrillion"
 msgid_plural "quadrillion"
-msgstr[0] "万亿"
-msgstr[1] "万亿"
+msgstr[0] "quatrilhão"
+msgstr[1] "quatrilhão"
 
-#: src/humanize/number.py:145
+#: src/humanize/number.py:183
 msgid "quintillion"
 msgid_plural "quintillion"
-msgstr[0] "百京"
-msgstr[1] "百京"
+msgstr[0] "quintilhão"
+msgstr[1] "quintilhão"
 
-#: src/humanize/number.py:146
+#: src/humanize/number.py:184
 msgid "sextillion"
 msgid_plural "sextillion"
-msgstr[0] "十垓"
-msgstr[1] "十垓"
+msgstr[0] "sextilhão"
+msgstr[1] "sextilhão"
 
-#: src/humanize/number.py:147
+#: src/humanize/number.py:185
 msgid "septillion"
 msgid_plural "septillion"
-msgstr[0] "秭"
-msgstr[1] "秭"
+msgstr[0] "septilhão"
+msgstr[1] "septilhão"
 
-#: src/humanize/number.py:148
+#: src/humanize/number.py:186
 msgid "octillion"
 msgid_plural "octillion"
-msgstr[0] "千秭"
-msgstr[1] "千秭"
+msgstr[0] "octilhão"
+msgstr[1] "octilhão"
 
-#: src/humanize/number.py:149
+#: src/humanize/number.py:187
 msgid "nonillion"
 msgid_plural "nonillion"
-msgstr[0] "百穰"
-msgstr[1] "百穰"
+msgstr[0] "nonilhão"
+msgstr[1] "nonilhão"
 
-#: src/humanize/number.py:150
+#: src/humanize/number.py:188
 msgid "decillion"
 msgid_plural "decillion"
-msgstr[0] "十沟"
-msgstr[1] "十沟"
+msgstr[0] "decilhão"
+msgstr[1] "decilhão"
 
-#: src/humanize/number.py:151
+#: src/humanize/number.py:189
 msgid "googol"
 msgid_plural "googol"
-msgstr[0] "古高尔"
-msgstr[1] "古高尔"
+msgstr[0] "undecilhão"
+msgstr[1] "undecilhão"
 
-#: src/humanize/number.py:246
+#: src/humanize/number.py:301
 msgid "zero"
-msgstr ""
+msgstr "zero"
 
-#: src/humanize/number.py:247
+#: src/humanize/number.py:302
 msgid "one"
-msgstr "一"
+msgstr "um"
 
-#: src/humanize/number.py:248
+#: src/humanize/number.py:303
 msgid "two"
-msgstr "二"
+msgstr "dois"
 
-#: src/humanize/number.py:249
+#: src/humanize/number.py:304
 msgid "three"
-msgstr "三"
+msgstr "três"
 
-#: src/humanize/number.py:250
+#: src/humanize/number.py:305
 msgid "four"
-msgstr "四"
+msgstr "quatro"
 
-#: src/humanize/number.py:251
+#: src/humanize/number.py:306
 msgid "five"
-msgstr "五"
+msgstr "cinco"
 
-#: src/humanize/number.py:252
+#: src/humanize/number.py:307
 msgid "six"
-msgstr "六"
+msgstr "seis"
 
-#: src/humanize/number.py:253
+#: src/humanize/number.py:308
 msgid "seven"
-msgstr "七"
+msgstr "sete"
 
-#: src/humanize/number.py:254
+#: src/humanize/number.py:309
 msgid "eight"
-msgstr "八"
+msgstr "oito"
 
-#: src/humanize/number.py:255
+#: src/humanize/number.py:310
 msgid "nine"
-msgstr "九"
+msgstr "nove"
 
-#: src/humanize/time.py:133
-#, python-format
+#: src/humanize/time.py:152
+#, fuzzy, python-format
 msgid "%d microsecond"
 msgid_plural "%d microseconds"
-msgstr[0] ""
-msgstr[1] ""
+msgstr[0] "%d microssegundo"
+msgstr[1] "%d microssegundos"
 
-#: src/humanize/time.py:142
-#, python-format
+#: src/humanize/time.py:161
+#, fuzzy, python-format
 msgid "%d millisecond"
 msgid_plural "%d milliseconds"
-msgstr[0] ""
-msgstr[1] ""
+msgstr[0] "%d milissegundo"
+msgstr[1] "%d milissegundos"
 
-#: src/humanize/time.py:145 src/humanize/time.py:220
+#: src/humanize/time.py:164 src/humanize/time.py:259
 msgid "a moment"
-msgstr "一会儿"
+msgstr "um momento"
 
-#: src/humanize/time.py:147
+#: src/humanize/time.py:167
 msgid "a second"
-msgstr "1秒"
+msgstr "um segundo"
 
-#: src/humanize/time.py:149
+#: src/humanize/time.py:170
 #, python-format
 msgid "%d second"
 msgid_plural "%d seconds"
-msgstr[0] "%d秒"
-msgstr[1] "%d秒"
+msgstr[0] "%d segundo"
+msgstr[1] "%d segundos"
 
-#: src/humanize/time.py:151
+#: src/humanize/time.py:173
 msgid "a minute"
-msgstr "1分"
+msgstr "um minuto"
 
-#: src/humanize/time.py:154
+#: src/humanize/time.py:177
 #, python-format
 msgid "%d minute"
 msgid_plural "%d minutes"
-msgstr[0] "%d分"
-msgstr[1] "%d分"
+msgstr[0] "%d minuto"
+msgstr[1] "%d minutos"
 
-#: src/humanize/time.py:156
+#: src/humanize/time.py:180
 msgid "an hour"
-msgstr "1小时"
+msgstr "uma hora"
 
-#: src/humanize/time.py:159
+#: src/humanize/time.py:184
 #, python-format
 msgid "%d hour"
 msgid_plural "%d hours"
-msgstr[0] "%d小时"
-msgstr[1] "%d小时"
+msgstr[0] "%d hora"
+msgstr[1] "%d horas"
 
-#: src/humanize/time.py:162
+#: src/humanize/time.py:188
 msgid "a day"
-msgstr "1天"
+msgstr "um dia"
 
-#: src/humanize/time.py:164 src/humanize/time.py:167
+#: src/humanize/time.py:191 src/humanize/time.py:194
 #, python-format
 msgid "%d day"
 msgid_plural "%d days"
-msgstr[0] "%d天"
-msgstr[1] "%d天"
+msgstr[0] "%d dia"
+msgstr[1] "%d dias"
 
-#: src/humanize/time.py:169
+#: src/humanize/time.py:197
 msgid "a month"
-msgstr "1月"
+msgstr "um mês"
 
-#: src/humanize/time.py:171
+#: src/humanize/time.py:199
 #, python-format
 msgid "%d month"
 msgid_plural "%d months"
-msgstr[0] "%d月"
-msgstr[1] "%d月"
+msgstr[0] "%d mês"
+msgstr[1] "%d meses"
 
-#: src/humanize/time.py:174
+#: src/humanize/time.py:203
 msgid "a year"
-msgstr "1年"
+msgstr "um ano"
 
-#: src/humanize/time.py:176 src/humanize/time.py:185
+#: src/humanize/time.py:206 src/humanize/time.py:217
 #, python-format
 msgid "1 year, %d day"
 msgid_plural "1 year, %d days"
-msgstr[0] "%d年"
-msgstr[1] "%d年"
+msgstr[0] "1 ano e %d dia"
+msgstr[1] "1 ano e %d dias"
 
-#: src/humanize/time.py:179
+#: src/humanize/time.py:210
 msgid "1 year, 1 month"
-msgstr "1年又1月"
+msgstr "1 ano e 1 mês"
 
-#: src/humanize/time.py:182
+#: src/humanize/time.py:213
 #, python-format
 msgid "1 year, %d month"
 msgid_plural "1 year, %d months"
-msgstr[0] "1年又%d月"
-msgstr[1] "1年又%d月"
+msgstr[0] "1 ano e %d mês"
+msgstr[1] "1 ano e %d meses"
 
-#: src/humanize/time.py:187
+#: src/humanize/time.py:219
 #, python-format
 msgid "%d year"
 msgid_plural "%d years"
-msgstr[0] "%d年"
-msgstr[1] "%d年"
+msgstr[0] "%d ano"
+msgstr[1] "%d anos"
 
-#: src/humanize/time.py:217
+#: src/humanize/time.py:256
 #, python-format
 msgid "%s from now"
-msgstr "%s之后"
+msgstr "em %s"
 
-#: src/humanize/time.py:217
+#: src/humanize/time.py:256
 #, python-format
 msgid "%s ago"
-msgstr "%s之前"
+msgstr "há %s"
 
-#: src/humanize/time.py:221
+#: src/humanize/time.py:260
 msgid "now"
-msgstr "现在"
+msgstr "agora"
 
-#: src/humanize/time.py:244
+#: src/humanize/time.py:284
 msgid "today"
-msgstr "今天"
+msgstr "hoje"
 
-#: src/humanize/time.py:246
+#: src/humanize/time.py:287
 msgid "tomorrow"
-msgstr "明天"
+msgstr "amanhã"
 
-#: src/humanize/time.py:248
+#: src/humanize/time.py:290
 msgid "yesterday"
-msgstr "昨天"
+msgstr "ontem"
 
-#: src/humanize/time.py:534
+#: src/humanize/time.py:600
 #, python-format
 msgid "%s and %s"
-msgstr ""
+msgstr "%s e %s"
```

### Comparing `humanize-4.5.0/src/humanize/locale/zh_HK/LC_MESSAGES/humanize.mo` & `humanize-4.6.0/src/humanize/locale/zh_HK/LC_MESSAGES/humanize.mo`

 * *Files identical despite different names*

### Comparing `humanize-4.5.0/src/humanize/locale/zh_HK/LC_MESSAGES/humanize.po` & `humanize-4.6.0/src/humanize/locale/sv_SE/LC_MESSAGES/humanize.po`

 * *Files 12% similar despite different names*

```diff
@@ -1,365 +1,363 @@
-# Traditional Chinese (China) translation for the project
+# Swedish (Sweden) translations for humanize package.
 # Copyright (C) 2021
-# This file is distributed under the same license as the PACKAGE package.
-# AZLisme <helloazl@icloud.com>, 2016.
-# Liwen SUN <sunliwen@gmail.com>, 2019.
-# Edward Ho <edward@edward.is>, 2021.
+# This file is distributed under the same license as the humanize project.
+# Kess Vargavind <vargavind@gmail.com>, 2021.
 #
 msgid ""
 msgstr ""
-"Project-Id-Version: 1.0\n"
+"Project-Id-Version: humanize\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2021-05-04 23:15+0200\n"
-"PO-Revision-Date: 2016-11-14 23:02+0000\n"
-"Last-Translator: Edward Ho <edward@edward.is>\n"
-"Language-Team: Chinese (traditional)\n"
-"Language: zh_HK\n"
+"POT-Creation-Date: 2023-01-08 19:22+0200\n"
+"PO-Revision-Date: 2021-07-05 10:30+0200\n"
+"Last-Translator: Kess Vargavind <vargavind@gmail.com>\n"
+"Language-Team: Swedish\n"
+"Language: sv\n"
 "MIME-Version: 1.0\n"
-"Content-Type: text/plain; charset=UTF-8\n"
+"Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=(n > 1);\n"
+"Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
-#: src/humanize/number.py:57
+#: src/humanize/number.py:84
 msgctxt "0 (male)"
 msgid "th"
-msgstr "第"
+msgstr ":e"
 
-#: src/humanize/number.py:58
+#: src/humanize/number.py:85
 msgctxt "1 (male)"
 msgid "st"
-msgstr "第"
+msgstr ":a"
 
-#: src/humanize/number.py:59
+#: src/humanize/number.py:86
 msgctxt "2 (male)"
 msgid "nd"
-msgstr "第"
+msgstr ":a"
 
-#: src/humanize/number.py:60
+#: src/humanize/number.py:87
 msgctxt "3 (male)"
 msgid "rd"
-msgstr "第"
+msgstr ":e"
 
-#: src/humanize/number.py:61
+#: src/humanize/number.py:88
 msgctxt "4 (male)"
 msgid "th"
-msgstr "第"
+msgstr ":e"
 
-#: src/humanize/number.py:62
+#: src/humanize/number.py:89
 msgctxt "5 (male)"
 msgid "th"
-msgstr "第"
+msgstr ":e"
 
-#: src/humanize/number.py:63
+#: src/humanize/number.py:90
 msgctxt "6 (male)"
 msgid "th"
-msgstr "第"
+msgstr ":e"
 
-#: src/humanize/number.py:64
+#: src/humanize/number.py:91
 msgctxt "7 (male)"
 msgid "th"
-msgstr "第"
+msgstr ":e"
 
-#: src/humanize/number.py:65
+#: src/humanize/number.py:92
 msgctxt "8 (male)"
 msgid "th"
-msgstr "第"
+msgstr ":e"
 
-#: src/humanize/number.py:66
+#: src/humanize/number.py:93
 msgctxt "9 (male)"
 msgid "th"
-msgstr "第"
+msgstr ":e"
 
-#: src/humanize/number.py:70
+#: src/humanize/number.py:97
 msgctxt "0 (female)"
 msgid "th"
-msgstr "第"
+msgstr ":e"
 
-#: src/humanize/number.py:71
+#: src/humanize/number.py:98
 msgctxt "1 (female)"
 msgid "st"
-msgstr "第"
+msgstr ":a"
 
-#: src/humanize/number.py:72
+#: src/humanize/number.py:99
 msgctxt "2 (female)"
 msgid "nd"
-msgstr "第"
+msgstr ":a"
 
-#: src/humanize/number.py:73
+#: src/humanize/number.py:100
 msgctxt "3 (female)"
 msgid "rd"
-msgstr "第"
+msgstr ":e"
 
-#: src/humanize/number.py:74
+#: src/humanize/number.py:101
 msgctxt "4 (female)"
 msgid "th"
-msgstr "第"
+msgstr ":e"
 
-#: src/humanize/number.py:75
+#: src/humanize/number.py:102
 msgctxt "5 (female)"
 msgid "th"
-msgstr "第"
+msgstr ":e"
 
-#: src/humanize/number.py:76
+#: src/humanize/number.py:103
 msgctxt "6 (female)"
 msgid "th"
-msgstr "第"
+msgstr ":e"
 
-#: src/humanize/number.py:77
+#: src/humanize/number.py:104
 msgctxt "7 (female)"
 msgid "th"
-msgstr "第"
+msgstr ":e"
 
-#: src/humanize/number.py:78
+#: src/humanize/number.py:105
 msgctxt "8 (female)"
 msgid "th"
-msgstr "第"
+msgstr ":e"
 
-#: src/humanize/number.py:79
+#: src/humanize/number.py:106
 msgctxt "9 (female)"
 msgid "th"
-msgstr "第"
+msgstr ":e"
 
-#: src/humanize/number.py:140
+#: src/humanize/number.py:178
 msgid "thousand"
 msgid_plural "thousand"
-msgstr[0] "千"
-msgstr[1] "千"
+msgstr[0] "tusen"
+msgstr[1] "tusen"
 
-#: src/humanize/number.py:141
+#: src/humanize/number.py:179
 msgid "million"
 msgid_plural "million"
-msgstr[0] "百萬"
-msgstr[1] "百萬"
+msgstr[0] "miljon"
+msgstr[1] "miljoner"
 
-#: src/humanize/number.py:142
+#: src/humanize/number.py:180
 msgid "billion"
 msgid_plural "billion"
-msgstr[0] "十億"
-msgstr[1] "十億"
+msgstr[0] "miljard"
+msgstr[1] "miljarder"
 
-#: src/humanize/number.py:143
+#: src/humanize/number.py:181
 msgid "trillion"
 msgid_plural "trillion"
-msgstr[0] "兆"
-msgstr[1] "兆"
+msgstr[0] "biljon"
+msgstr[1] "biljoner"
 
-#: src/humanize/number.py:144
+#: src/humanize/number.py:182
 msgid "quadrillion"
 msgid_plural "quadrillion"
-msgstr[0] "萬億"
-msgstr[1] "萬億"
+msgstr[0] "biljard"
+msgstr[1] "biljarder"
 
-#: src/humanize/number.py:145
+#: src/humanize/number.py:183
 msgid "quintillion"
 msgid_plural "quintillion"
-msgstr[0] "百京"
-msgstr[1] "百京"
+msgstr[0] "triljon"
+msgstr[1] "triljoner"
 
-#: src/humanize/number.py:146
+#: src/humanize/number.py:184
 msgid "sextillion"
 msgid_plural "sextillion"
-msgstr[0] "十垓"
-msgstr[1] "十垓"
+msgstr[0] "triljard"
+msgstr[1] "triljarder"
 
-#: src/humanize/number.py:147
+#: src/humanize/number.py:185
 msgid "septillion"
 msgid_plural "septillion"
-msgstr[0] "秭"
-msgstr[1] "秭"
+msgstr[0] "kvadriljon"
+msgstr[1] "kvadriljoner"
 
-#: src/humanize/number.py:148
+#: src/humanize/number.py:186
 msgid "octillion"
 msgid_plural "octillion"
-msgstr[0] "千秭"
-msgstr[1] "千秭"
+msgstr[0] "kvadriljard"
+msgstr[1] "kvadriljarder"
 
-#: src/humanize/number.py:149
+#: src/humanize/number.py:187
 msgid "nonillion"
 msgid_plural "nonillion"
-msgstr[0] "百穰"
-msgstr[1] "百穰"
+msgstr[0] "kvintiljon"
+msgstr[1] "kvintiljoner"
 
-#: src/humanize/number.py:150
+#: src/humanize/number.py:188
 msgid "decillion"
 msgid_plural "decillion"
-msgstr[0] "十溝"
-msgstr[1] "十溝"
+msgstr[0] "kvintiljard"
+msgstr[1] "kvintiljarder"
 
-#: src/humanize/number.py:151
+#: src/humanize/number.py:189
 msgid "googol"
 msgid_plural "googol"
-msgstr[0] "古高爾"
-msgstr[1] "古高爾"
+msgstr[0] "googol"
+msgstr[1] "googol"
 
-#: src/humanize/number.py:246
+#: src/humanize/number.py:301
 msgid "zero"
-msgstr "零"
+msgstr "noll"
 
-#: src/humanize/number.py:247
+#: src/humanize/number.py:302
 msgid "one"
-msgstr "一"
+msgstr "ett"
 
-#: src/humanize/number.py:248
+#: src/humanize/number.py:303
 msgid "two"
-msgstr "二"
+msgstr "två"
 
-#: src/humanize/number.py:249
+#: src/humanize/number.py:304
 msgid "three"
-msgstr "三"
+msgstr "tre"
 
-#: src/humanize/number.py:250
+#: src/humanize/number.py:305
 msgid "four"
-msgstr "四"
+msgstr "fyra"
 
-#: src/humanize/number.py:251
+#: src/humanize/number.py:306
 msgid "five"
-msgstr "五"
+msgstr "fem"
 
-#: src/humanize/number.py:252
+#: src/humanize/number.py:307
 msgid "six"
-msgstr "六"
+msgstr "sex"
 
-#: src/humanize/number.py:253
+#: src/humanize/number.py:308
 msgid "seven"
-msgstr "七"
+msgstr "sju"
 
-#: src/humanize/number.py:254
+#: src/humanize/number.py:309
 msgid "eight"
-msgstr "八"
+msgstr "åtta"
 
-#: src/humanize/number.py:255
+#: src/humanize/number.py:310
 msgid "nine"
-msgstr "九"
+msgstr "nio"
 
-#: src/humanize/time.py:133
+#: src/humanize/time.py:152
 #, python-format
 msgid "%d microsecond"
 msgid_plural "%d microseconds"
-msgstr[0] "%d 微秒"
-msgstr[1] "%d 微秒"
+msgstr[0] "%d mikrosekund"
+msgstr[1] "%d mikrosekunder"
 
-#: src/humanize/time.py:142
+#: src/humanize/time.py:161
 #, python-format
 msgid "%d millisecond"
 msgid_plural "%d milliseconds"
-msgstr[0] "%d 毫秒"
-msgstr[1] "%d 毫秒"
+msgstr[0] "%d millsekund"
+msgstr[1] "%d millsekunder"
 
-#: src/humanize/time.py:145 src/humanize/time.py:220
+#: src/humanize/time.py:164 src/humanize/time.py:259
 msgid "a moment"
-msgstr "一會"
+msgstr "en liten stund"
 
-#: src/humanize/time.py:147
+#: src/humanize/time.py:167
 msgid "a second"
-msgstr "1 秒"
+msgstr "en sekund"
 
-#: src/humanize/time.py:149
+#: src/humanize/time.py:170
 #, python-format
 msgid "%d second"
 msgid_plural "%d seconds"
-msgstr[0] "%d 秒"
-msgstr[1] "%d 秒"
+msgstr[0] "%d sekund"
+msgstr[1] "%d sekunder"
 
-#: src/humanize/time.py:151
+#: src/humanize/time.py:173
 msgid "a minute"
-msgstr "1 分鐘"
+msgstr "en minut"
 
-#: src/humanize/time.py:154
+#: src/humanize/time.py:177
 #, python-format
 msgid "%d minute"
 msgid_plural "%d minutes"
-msgstr[0] "%d 分鐘"
-msgstr[1] "%d 分鐘"
+msgstr[0] "%d minut"
+msgstr[1] "%d minuter"
 
-#: src/humanize/time.py:156
+#: src/humanize/time.py:180
 msgid "an hour"
-msgstr "1 小時"
+msgstr "en timme"
 
-#: src/humanize/time.py:159
+#: src/humanize/time.py:184
 #, python-format
 msgid "%d hour"
 msgid_plural "%d hours"
-msgstr[0] "%d 小時"
-msgstr[1] "%d 小時"
+msgstr[0] "%d timme"
+msgstr[1] "%d timmar"
 
-#: src/humanize/time.py:162
+#: src/humanize/time.py:188
 msgid "a day"
-msgstr "1 天"
+msgstr "en dag"
 
-#: src/humanize/time.py:164 src/humanize/time.py:167
+#: src/humanize/time.py:191 src/humanize/time.py:194
 #, python-format
 msgid "%d day"
 msgid_plural "%d days"
-msgstr[0] "%d 天"
-msgstr[1] "%d 天"
+msgstr[0] "%d dag"
+msgstr[1] "%d dagar"
 
-#: src/humanize/time.py:169
+#: src/humanize/time.py:197
 msgid "a month"
-msgstr "1 月"
+msgstr "en månad"
 
-#: src/humanize/time.py:171
+#: src/humanize/time.py:199
 #, python-format
 msgid "%d month"
 msgid_plural "%d months"
-msgstr[0] "%d 月"
-msgstr[1] "%d 月"
+msgstr[0] "%d månad"
+msgstr[1] "%d månader"
 
-#: src/humanize/time.py:174
+#: src/humanize/time.py:203
 msgid "a year"
-msgstr "1 年"
+msgstr "ett år"
 
-#: src/humanize/time.py:176 src/humanize/time.py:185
+#: src/humanize/time.py:206 src/humanize/time.py:217
 #, python-format
 msgid "1 year, %d day"
 msgid_plural "1 year, %d days"
-msgstr[0] "%d 年"
-msgstr[1] "%d 年"
+msgstr[0] "1 år, %d dag"
+msgstr[1] "1 år, %d dagar"
 
-#: src/humanize/time.py:179
+#: src/humanize/time.py:210
 msgid "1 year, 1 month"
-msgstr "1 年又 1 個月"
+msgstr "1 år, 1 månad"
 
-#: src/humanize/time.py:182
+#: src/humanize/time.py:213
 #, python-format
 msgid "1 year, %d month"
 msgid_plural "1 year, %d months"
-msgstr[0] "1 年又 %d 個月"
-msgstr[1] "1 年又 %d 個月"
+msgstr[0] "1 år, %d månad"
+msgstr[1] "1 år, %d månader"
 
-#: src/humanize/time.py:187
+#: src/humanize/time.py:219
 #, python-format
 msgid "%d year"
 msgid_plural "%d years"
-msgstr[0] "%d年"
-msgstr[1] "%d年"
+msgstr[0] "%d år"
+msgstr[1] "%d år"
 
-#: src/humanize/time.py:217
+#: src/humanize/time.py:256
 #, python-format
 msgid "%s from now"
-msgstr "%s 之後"
+msgstr "%s från nu"
 
-#: src/humanize/time.py:217
+#: src/humanize/time.py:256
 #, python-format
 msgid "%s ago"
-msgstr "%s 之前"
+msgstr "%s sedan"
 
-#: src/humanize/time.py:221
+#: src/humanize/time.py:260
 msgid "now"
-msgstr "現在"
+msgstr "nu"
 
-#: src/humanize/time.py:244
+#: src/humanize/time.py:284
 msgid "today"
-msgstr "今天"
+msgstr "idag"
 
-#: src/humanize/time.py:246
+#: src/humanize/time.py:287
 msgid "tomorrow"
-msgstr "明天"
+msgstr "imorgon"
 
-#: src/humanize/time.py:248
+#: src/humanize/time.py:290
 msgid "yesterday"
-msgstr "昨天"
+msgstr "igår"
 
-#: src/humanize/time.py:534
+#: src/humanize/time.py:600
 #, python-format
 msgid "%s and %s"
-msgstr "%s 與 %s"
+msgstr "%s och %s"
```

### Comparing `humanize-4.5.0/src/humanize/number.py` & `humanize-4.6.0/src/humanize/number.py`

 * *Files identical despite different names*

### Comparing `humanize-4.5.0/src/humanize/time.py` & `humanize-4.6.0/src/humanize/time.py`

 * *Files identical despite different names*

### Comparing `humanize-4.5.0/tests/test_filesize.py` & `humanize-4.6.0/tests/test_filesize.py`

 * *Files identical despite different names*

### Comparing `humanize-4.5.0/tests/test_i18n.py` & `humanize-4.6.0/tests/test_i18n.py`

 * *Files identical despite different names*

### Comparing `humanize-4.5.0/tests/test_number.py` & `humanize-4.6.0/tests/test_number.py`

 * *Files identical despite different names*

### Comparing `humanize-4.5.0/tests/test_time.py` & `humanize-4.6.0/tests/test_time.py`

 * *Files identical despite different names*

