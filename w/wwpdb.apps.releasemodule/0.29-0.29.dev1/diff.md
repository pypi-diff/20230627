# Comparing `tmp/wwpdb.apps.releasemodule-0.29.tar.gz` & `tmp/wwpdb.apps.releasemodule-0.29.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wwpdb.apps.releasemodule-0.29.tar", last modified: Tue Jun 27 12:52:37 2023, max compression
+gzip compressed data, was "wwpdb.apps.releasemodule-0.29.dev1.tar", last modified: Tue May 30 10:29:44 2023, max compression
```

## Comparing `wwpdb.apps.releasemodule-0.29.tar` & `wwpdb.apps.releasemodule-0.29.dev1.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-27 12:52:37.005140 wwpdb.apps.releasemodule-0.29/
--rw-r--r--   0 vsts      (1001) docker     (123)      728 2023-06-27 12:52:37.005140 wwpdb.apps.releasemodule-0.29/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)       52 2023-06-27 12:50:40.000000 wwpdb.apps.releasemodule-0.29/README.md
--rw-r--r--   0 vsts      (1001) docker     (123)      531 2023-06-27 12:52:37.005140 wwpdb.apps.releasemodule-0.29/setup.cfg
--rwxr-xr-x   0 vsts      (1001) docker     (123)     2509 2023-06-27 12:50:40.000000 wwpdb.apps.releasemodule-0.29/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-27 12:52:36.997140 wwpdb.apps.releasemodule-0.29/wwpdb/
--rw-r--r--   0 vsts      (1001) docker     (123)       65 2023-06-27 12:50:40.000000 wwpdb.apps.releasemodule-0.29/wwpdb/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-27 12:52:36.997140 wwpdb.apps.releasemodule-0.29/wwpdb/apps/
--rw-r--r--   0 vsts      (1001) docker     (123)       65 2023-06-27 12:50:40.000000 wwpdb.apps.releasemodule-0.29/wwpdb/apps/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-27 12:52:36.997140 wwpdb.apps.releasemodule-0.29/wwpdb/apps/releasemodule/
--rw-r--r--   0 vsts      (1001) docker     (123)      150 2023-06-27 12:50:40.000000 wwpdb.apps.releasemodule-0.29/wwpdb/apps/releasemodule/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-27 12:52:36.997140 wwpdb.apps.releasemodule-0.29/wwpdb/apps/releasemodule/citation/
--rw-r--r--   0 vsts      (1001) docker     (123)    10466 2023-06-27 12:50:40.000000 wwpdb.apps.releasemodule-0.29/wwpdb/apps/releasemodule/citation/Analysis.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2661 2023-06-27 12:50:40.000000 wwpdb.apps.releasemodule-0.29/wwpdb/apps/releasemodule/citation/CheckResult.py
--rw-r--r--   0 vsts      (1001) docker     (123)    15685 2023-06-27 12:50:40.000000 wwpdb.apps.releasemodule-0.29/wwpdb/apps/releasemodule/citation/CitationFinder.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5284 2023-06-27 12:50:40.000000 wwpdb.apps.releasemodule-0.29/wwpdb/apps/releasemodule/citation/FetchMP.py
--rw-r--r--   0 vsts      (1001) docker     (123)    35269 2023-06-27 12:50:40.000000 wwpdb.apps.releasemodule-0.29/wwpdb/apps/releasemodule/citation/FetchResultParser.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4490 2023-06-27 12:50:40.000000 wwpdb.apps.releasemodule-0.29/wwpdb/apps/releasemodule/citation/FetchUtil.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3611 2023-06-27 12:50:40.000000 wwpdb.apps.releasemodule-0.29/wwpdb/apps/releasemodule/citation/MatchMP.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2569 2023-06-27 12:50:40.000000 wwpdb.apps.releasemodule-0.29/wwpdb/apps/releasemodule/citation/MatchUtil.py
--rw-r--r--   0 vsts      (1001) docker     (123)     8181 2023-06-27 12:50:40.000000 wwpdb.apps.releasemodule-0.29/wwpdb/apps/releasemodule/citation/MonitorCitationUpdate.py
--rw-r--r--   0 vsts      (1001) docker     (123)    14457 2023-06-27 12:50:40.000000 wwpdb.apps.releasemodule-0.29/wwpdb/apps/releasemodule/citation/ReadCitationFinderResult_v2.py
--rw-r--r--   0 vsts      (1001) docker     (123)     6962 2023-06-27 12:50:40.000000 wwpdb.apps.releasemodule-0.29/wwpdb/apps/releasemodule/citation/RisCitationParser.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4999 2023-06-27 12:50:40.000000 wwpdb.apps.releasemodule-0.29/wwpdb/apps/releasemodule/citation/SearchMP.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1635 2023-06-27 12:50:40.000000 wwpdb.apps.releasemodule-0.29/wwpdb/apps/releasemodule/citation/SearchResultParser.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3194 2023-06-27 12:50:40.000000 wwpdb.apps.releasemodule-0.29/wwpdb/apps/releasemodule/citation/SearchUtil.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2505 2023-06-27 12:50:40.000000 wwpdb.apps.releasemodule-0.29/wwpdb/apps/releasemodule/citation/StringUtil.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-27 12:50:40.000000 wwpdb.apps.releasemodule-0.29/wwpdb/apps/releasemodule/citation/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-27 12:52:37.001140 wwpdb.apps.releasemodule-0.29/wwpdb/apps/releasemodule/depict/
--rw-r--r--   0 vsts      (1001) docker     (123)     2904 2023-06-27 12:50:40.000000 wwpdb.apps.releasemodule-0.29/wwpdb/apps/releasemodule/depict/DepictAnnotatorHistory.py
--rw-r--r--   0 vsts      (1001) docker     (123)    19491 2023-06-27 12:50:40.000000 wwpdb.apps.releasemodule-0.29/wwpdb/apps/releasemodule/depict/DepictBase.py
--rw-r--r--   0 vsts      (1001) docker     (123)     7724 2023-06-27 12:50:40.000000 wwpdb.apps.releasemodule-0.29/wwpdb/apps/releasemodule/depict/DepictCitationForm_v2.py
--rw-r--r--   0 vsts      (1001) docker     (123)    19597 2023-06-27 12:50:40.000000 wwpdb.apps.releasemodule-0.29/wwpdb/apps/releasemodule/depict/DepictCitation_v2.py
--rw-r--r--   0 vsts      (1001) docker     (123)     7582 2023-06-27 12:50:40.000000 wwpdb.apps.releasemodule-0.29/wwpdb/apps/releasemodule/depict/DepictEntryHistory.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4158 2023-06-27 12:50:40.000000 wwpdb.apps.releasemodule-0.29/wwpdb/apps/releasemodule/depict/DepictReleaseInfo.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4437 2023-06-27 12:50:40.000000 wwpdb.apps.releasemodule-0.29/wwpdb/apps/releasemodule/depict/DepictRemovalMark.py
--rw-r--r--   0 vsts      (1001) docker     (123)     6428 2023-06-27 12:50:40.000000 wwpdb.apps.releasemodule-0.29/wwpdb/apps/releasemodule/depict/DepictRequest.py
--rw-r--r--   0 vsts      (1001) docker     (123)    14638 2023-06-27 12:50:40.000000 wwpdb.apps.releasemodule-0.29/wwpdb/apps/releasemodule/depict/ReleaseOption_v2.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-27 12:50:40.000000 wwpdb.apps.releasemodule-0.29/wwpdb/apps/releasemodule/depict/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)      894 2023-06-27 12:50:40.000000 wwpdb.apps.releasemodule-0.29/wwpdb/apps/releasemodule/depict/test_DepictCitation.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-27 12:52:37.001140 wwpdb.apps.releasemodule-0.29/wwpdb/apps/releasemodule/update/
--rw-r--r--   0 vsts      (1001) docker     (123)    12660 2023-06-27 12:50:40.000000 wwpdb.apps.releasemodule-0.29/wwpdb/apps/releasemodule/update/AutoReRelease.py
--rw-r--r--   0 vsts      (1001) docker     (123)    12851 2023-06-27 12:50:40.000000 wwpdb.apps.releasemodule-0.29/wwpdb/apps/releasemodule/update/CitationFormParser_v2.py
--rw-r--r--   0 vsts      (1001) docker     (123)    12694 2023-06-27 12:50:40.000000 wwpdb.apps.releasemodule-0.29/wwpdb/apps/releasemodule/update/EmReleaseUtil.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3069 2023-06-27 12:50:40.000000 wwpdb.apps.releasemodule-0.29/wwpdb/apps/releasemodule/update/EntryFormParser_v2.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2600 2023-06-27 12:50:40.000000 wwpdb.apps.releasemodule-0.29/wwpdb/apps/releasemodule/update/EntryPullProcess.py
--rw-r--r--   0 vsts      (1001) docker     (123)    25384 2023-06-27 12:50:40.000000 wwpdb.apps.releasemodule-0.29/wwpdb/apps/releasemodule/update/EntryUpdateBase.py
--rw-r--r--   0 vsts      (1001) docker     (123)    25079 2023-06-27 12:50:40.000000 wwpdb.apps.releasemodule-0.29/wwpdb/apps/releasemodule/update/EntryUpdateProcess.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3537 2023-06-27 12:50:40.000000 wwpdb.apps.releasemodule-0.29/wwpdb/apps/releasemodule/update/InputFormParser_v2.py
--rw-r--r--   0 vsts      (1001) docker     (123)    17268 2023-06-27 12:50:40.000000 wwpdb.apps.releasemodule-0.29/wwpdb/apps/releasemodule/update/MultiUpdateProcess.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4828 2023-06-27 12:50:40.000000 wwpdb.apps.releasemodule-0.29/wwpdb/apps/releasemodule/update/NmrDataGenerator.py
--rw-r--r--   0 vsts      (1001) docker     (123)    21726 2023-06-27 12:50:40.000000 wwpdb.apps.releasemodule-0.29/wwpdb/apps/releasemodule/update/ReleaseDpUtil.py
--rw-r--r--   0 vsts      (1001) docker     (123)    23667 2023-06-27 12:50:40.000000 wwpdb.apps.releasemodule-0.29/wwpdb/apps/releasemodule/update/ReleaseUtil.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3479 2023-06-27 12:50:40.000000 wwpdb.apps.releasemodule-0.29/wwpdb/apps/releasemodule/update/RunAutoReReleaseProcess.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3774 2023-06-27 12:50:40.000000 wwpdb.apps.releasemodule-0.29/wwpdb/apps/releasemodule/update/UpdateBase.py
--rw-r--r--   0 vsts      (1001) docker     (123)    22156 2023-06-27 12:50:40.000000 wwpdb.apps.releasemodule-0.29/wwpdb/apps/releasemodule/update/UpdateFormParser.py
--rw-r--r--   0 vsts      (1001) docker     (123)    13024 2023-06-27 12:50:40.000000 wwpdb.apps.releasemodule-0.29/wwpdb/apps/releasemodule/update/UpdateUtil_v2.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-27 12:50:40.000000 wwpdb.apps.releasemodule-0.29/wwpdb/apps/releasemodule/update/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-27 12:52:37.005140 wwpdb.apps.releasemodule-0.29/wwpdb/apps/releasemodule/utils/
--rw-r--r--   0 vsts      (1001) docker     (123)    23712 2023-06-27 12:50:40.000000 wwpdb.apps.releasemodule-0.29/wwpdb/apps/releasemodule/utils/CombineDbApi.py
--rw-r--r--   0 vsts      (1001) docker     (123)    22302 2023-06-27 12:50:40.000000 wwpdb.apps.releasemodule-0.29/wwpdb/apps/releasemodule/utils/ContentDbApi.py
--rw-r--r--   0 vsts      (1001) docker     (123)     7405 2023-06-27 12:50:40.000000 wwpdb.apps.releasemodule-0.29/wwpdb/apps/releasemodule/utils/DbApiUtil.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4439 2023-06-27 12:50:40.000000 wwpdb.apps.releasemodule-0.29/wwpdb/apps/releasemodule/utils/JournalAbbrev.py
--rw-r--r--   0 vsts      (1001) docker     (123)     6429 2023-06-27 12:50:40.000000 wwpdb.apps.releasemodule-0.29/wwpdb/apps/releasemodule/utils/MessageBaseClass.py
--rw-r--r--   0 vsts      (1001) docker     (123)     9479 2023-06-27 12:50:40.000000 wwpdb.apps.releasemodule-0.29/wwpdb/apps/releasemodule/utils/ModuleBaseClass.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1574 2023-06-27 12:50:40.000000 wwpdb.apps.releasemodule-0.29/wwpdb/apps/releasemodule/utils/MultiProcLimit.py
--rw-r--r--   0 vsts      (1001) docker     (123)     6170 2023-06-27 12:50:40.000000 wwpdb.apps.releasemodule-0.29/wwpdb/apps/releasemodule/utils/StatusDbApi_v2.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3456 2023-06-27 12:50:40.000000 wwpdb.apps.releasemodule-0.29/wwpdb/apps/releasemodule/utils/TimeUtil.py
--rw-r--r--   0 vsts      (1001) docker     (123)    12748 2023-06-27 12:50:40.000000 wwpdb.apps.releasemodule-0.29/wwpdb/apps/releasemodule/utils/Utility.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-27 12:50:40.000000 wwpdb.apps.releasemodule-0.29/wwpdb/apps/releasemodule/utils/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-27 12:52:37.005140 wwpdb.apps.releasemodule-0.29/wwpdb/apps/releasemodule/webapp/
--rw-r--r--   0 vsts      (1001) docker     (123)    46743 2023-06-27 12:50:40.000000 wwpdb.apps.releasemodule-0.29/wwpdb/apps/releasemodule/webapp/ReleaseWebApp_v2.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-27 12:50:40.000000 wwpdb.apps.releasemodule-0.29/wwpdb/apps/releasemodule/webapp/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-27 12:52:36.997140 wwpdb.apps.releasemodule-0.29/wwpdb.apps.releasemodule.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (123)      728 2023-06-27 12:52:36.000000 wwpdb.apps.releasemodule-0.29/wwpdb.apps.releasemodule.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)     3256 2023-06-27 12:52:36.000000 wwpdb.apps.releasemodule-0.29/wwpdb.apps.releasemodule.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-06-27 12:52:36.000000 wwpdb.apps.releasemodule-0.29/wwpdb.apps.releasemodule.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-06-27 12:52:19.000000 wwpdb.apps.releasemodule-0.29/wwpdb.apps.releasemodule.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (123)      246 2023-06-27 12:52:36.000000 wwpdb.apps.releasemodule-0.29/wwpdb.apps.releasemodule.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        6 2023-06-27 12:52:36.000000 wwpdb.apps.releasemodule-0.29/wwpdb.apps.releasemodule.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-30 10:29:44.117573 wwpdb.apps.releasemodule-0.29.dev1/
+-rw-r--r--   0 vsts      (1001) docker     (123)      733 2023-05-30 10:29:44.117573 wwpdb.apps.releasemodule-0.29.dev1/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)       52 2023-05-30 10:27:52.000000 wwpdb.apps.releasemodule-0.29.dev1/README.md
+-rw-r--r--   0 vsts      (1001) docker     (123)      531 2023-05-30 10:29:44.117573 wwpdb.apps.releasemodule-0.29.dev1/setup.cfg
+-rwxr-xr-x   0 vsts      (1001) docker     (123)     2509 2023-05-30 10:27:52.000000 wwpdb.apps.releasemodule-0.29.dev1/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-30 10:29:44.105573 wwpdb.apps.releasemodule-0.29.dev1/wwpdb/
+-rw-r--r--   0 vsts      (1001) docker     (123)       65 2023-05-30 10:27:52.000000 wwpdb.apps.releasemodule-0.29.dev1/wwpdb/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-30 10:29:44.105573 wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/
+-rw-r--r--   0 vsts      (1001) docker     (123)       65 2023-05-30 10:27:52.000000 wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-30 10:29:44.105573 wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/
+-rw-r--r--   0 vsts      (1001) docker     (123)      155 2023-05-30 10:27:52.000000 wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-30 10:29:44.109573 wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/citation/
+-rw-r--r--   0 vsts      (1001) docker     (123)    10466 2023-05-30 10:27:52.000000 wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/citation/Analysis.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2661 2023-05-30 10:27:52.000000 wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/citation/CheckResult.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    15685 2023-05-30 10:27:52.000000 wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/citation/CitationFinder.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5284 2023-05-30 10:27:52.000000 wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/citation/FetchMP.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    35269 2023-05-30 10:27:52.000000 wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/citation/FetchResultParser.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4490 2023-05-30 10:27:52.000000 wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/citation/FetchUtil.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3611 2023-05-30 10:27:52.000000 wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/citation/MatchMP.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2569 2023-05-30 10:27:52.000000 wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/citation/MatchUtil.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     8181 2023-05-30 10:27:52.000000 wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/citation/MonitorCitationUpdate.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    14457 2023-05-30 10:27:52.000000 wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/citation/ReadCitationFinderResult_v2.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     6962 2023-05-30 10:27:52.000000 wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/citation/RisCitationParser.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4999 2023-05-30 10:27:52.000000 wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/citation/SearchMP.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1635 2023-05-30 10:27:52.000000 wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/citation/SearchResultParser.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3194 2023-05-30 10:27:52.000000 wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/citation/SearchUtil.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2505 2023-05-30 10:27:52.000000 wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/citation/StringUtil.py
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-05-30 10:27:52.000000 wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/citation/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-30 10:29:44.109573 wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/depict/
+-rw-r--r--   0 vsts      (1001) docker     (123)     2904 2023-05-30 10:27:52.000000 wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/depict/DepictAnnotatorHistory.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    19491 2023-05-30 10:27:52.000000 wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/depict/DepictBase.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     7724 2023-05-30 10:27:52.000000 wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/depict/DepictCitationForm_v2.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    19597 2023-05-30 10:27:52.000000 wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/depict/DepictCitation_v2.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     7582 2023-05-30 10:27:52.000000 wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/depict/DepictEntryHistory.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4158 2023-05-30 10:27:52.000000 wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/depict/DepictReleaseInfo.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4437 2023-05-30 10:27:52.000000 wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/depict/DepictRemovalMark.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     6428 2023-05-30 10:27:52.000000 wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/depict/DepictRequest.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    14638 2023-05-30 10:27:52.000000 wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/depict/ReleaseOption_v2.py
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-05-30 10:27:52.000000 wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/depict/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      894 2023-05-30 10:27:52.000000 wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/depict/test_DepictCitation.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-30 10:29:44.113573 wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/update/
+-rw-r--r--   0 vsts      (1001) docker     (123)    12660 2023-05-30 10:27:52.000000 wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/update/AutoReRelease.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    12851 2023-05-30 10:27:52.000000 wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/update/CitationFormParser_v2.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    12694 2023-05-30 10:27:52.000000 wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/update/EmReleaseUtil.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3069 2023-05-30 10:27:52.000000 wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/update/EntryFormParser_v2.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2600 2023-05-30 10:27:52.000000 wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/update/EntryPullProcess.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    25384 2023-05-30 10:27:52.000000 wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/update/EntryUpdateBase.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    25079 2023-05-30 10:27:52.000000 wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/update/EntryUpdateProcess.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3537 2023-05-30 10:27:52.000000 wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/update/InputFormParser_v2.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    17268 2023-05-30 10:27:52.000000 wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/update/MultiUpdateProcess.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4828 2023-05-30 10:27:52.000000 wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/update/NmrDataGenerator.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    21726 2023-05-30 10:27:52.000000 wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/update/ReleaseDpUtil.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    23667 2023-05-30 10:27:52.000000 wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/update/ReleaseUtil.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3479 2023-05-30 10:27:52.000000 wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/update/RunAutoReReleaseProcess.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3774 2023-05-30 10:27:52.000000 wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/update/UpdateBase.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    22156 2023-05-30 10:27:52.000000 wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/update/UpdateFormParser.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    13024 2023-05-30 10:27:52.000000 wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/update/UpdateUtil_v2.py
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-05-30 10:27:52.000000 wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/update/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-30 10:29:44.117573 wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/utils/
+-rw-r--r--   0 vsts      (1001) docker     (123)    23712 2023-05-30 10:27:52.000000 wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/utils/CombineDbApi.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    22302 2023-05-30 10:27:52.000000 wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/utils/ContentDbApi.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     7405 2023-05-30 10:27:52.000000 wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/utils/DbApiUtil.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4439 2023-05-30 10:27:52.000000 wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/utils/JournalAbbrev.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     6429 2023-05-30 10:27:52.000000 wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/utils/MessageBaseClass.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     9479 2023-05-30 10:27:52.000000 wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/utils/ModuleBaseClass.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1574 2023-05-30 10:27:52.000000 wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/utils/MultiProcLimit.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     6170 2023-05-30 10:27:52.000000 wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/utils/StatusDbApi_v2.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3456 2023-05-30 10:27:52.000000 wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/utils/TimeUtil.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    12748 2023-05-30 10:27:52.000000 wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/utils/Utility.py
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-05-30 10:27:52.000000 wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/utils/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-30 10:29:44.117573 wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/webapp/
+-rw-r--r--   0 vsts      (1001) docker     (123)    46743 2023-05-30 10:27:52.000000 wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/webapp/ReleaseWebApp_v2.py
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-05-30 10:27:52.000000 wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/webapp/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-30 10:29:44.105573 wwpdb.apps.releasemodule-0.29.dev1/wwpdb.apps.releasemodule.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (123)      733 2023-05-30 10:29:44.000000 wwpdb.apps.releasemodule-0.29.dev1/wwpdb.apps.releasemodule.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)     3256 2023-05-30 10:29:44.000000 wwpdb.apps.releasemodule-0.29.dev1/wwpdb.apps.releasemodule.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-05-30 10:29:44.000000 wwpdb.apps.releasemodule-0.29.dev1/wwpdb.apps.releasemodule.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-05-30 10:29:26.000000 wwpdb.apps.releasemodule-0.29.dev1/wwpdb.apps.releasemodule.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (123)      246 2023-05-30 10:29:44.000000 wwpdb.apps.releasemodule-0.29.dev1/wwpdb.apps.releasemodule.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        6 2023-05-30 10:29:44.000000 wwpdb.apps.releasemodule-0.29.dev1/wwpdb.apps.releasemodule.egg-info/top_level.txt
```

### Comparing `wwpdb.apps.releasemodule-0.29/PKG-INFO` & `wwpdb.apps.releasemodule-0.29.dev1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wwpdb.apps.releasemodule
-Version: 0.29
+Version: 0.29.dev1
 Summary: wwPDB sequence module
 Home-page: https://github.com/rcsb/py-wwpdb_apps_releasemodule
 Author: Ezra Peisach
 Author-email: ezra.peisach@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `wwpdb.apps.releasemodule-0.29/setup.cfg` & `wwpdb.apps.releasemodule-0.29.dev1/setup.cfg`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.releasemodule-0.29/setup.py` & `wwpdb.apps.releasemodule-0.29.dev1/setup.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.releasemodule-0.29/wwpdb/apps/releasemodule/citation/Analysis.py` & `wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/citation/Analysis.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.releasemodule-0.29/wwpdb/apps/releasemodule/citation/CheckResult.py` & `wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/citation/CheckResult.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.releasemodule-0.29/wwpdb/apps/releasemodule/citation/CitationFinder.py` & `wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/citation/CitationFinder.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.releasemodule-0.29/wwpdb/apps/releasemodule/citation/FetchMP.py` & `wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/citation/FetchMP.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.releasemodule-0.29/wwpdb/apps/releasemodule/citation/FetchResultParser.py` & `wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/citation/FetchResultParser.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.releasemodule-0.29/wwpdb/apps/releasemodule/citation/FetchUtil.py` & `wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/citation/FetchUtil.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.releasemodule-0.29/wwpdb/apps/releasemodule/citation/MatchMP.py` & `wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/citation/MatchMP.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.releasemodule-0.29/wwpdb/apps/releasemodule/citation/MatchUtil.py` & `wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/citation/MatchUtil.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.releasemodule-0.29/wwpdb/apps/releasemodule/citation/MonitorCitationUpdate.py` & `wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/citation/MonitorCitationUpdate.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.releasemodule-0.29/wwpdb/apps/releasemodule/citation/ReadCitationFinderResult_v2.py` & `wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/citation/ReadCitationFinderResult_v2.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.releasemodule-0.29/wwpdb/apps/releasemodule/citation/RisCitationParser.py` & `wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/citation/RisCitationParser.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.releasemodule-0.29/wwpdb/apps/releasemodule/citation/SearchMP.py` & `wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/citation/SearchMP.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.releasemodule-0.29/wwpdb/apps/releasemodule/citation/SearchResultParser.py` & `wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/citation/SearchResultParser.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.releasemodule-0.29/wwpdb/apps/releasemodule/citation/SearchUtil.py` & `wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/citation/SearchUtil.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.releasemodule-0.29/wwpdb/apps/releasemodule/citation/StringUtil.py` & `wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/citation/StringUtil.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.releasemodule-0.29/wwpdb/apps/releasemodule/depict/DepictAnnotatorHistory.py` & `wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/depict/DepictAnnotatorHistory.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.releasemodule-0.29/wwpdb/apps/releasemodule/depict/DepictBase.py` & `wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/depict/DepictBase.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.releasemodule-0.29/wwpdb/apps/releasemodule/depict/DepictCitationForm_v2.py` & `wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/depict/DepictCitationForm_v2.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.releasemodule-0.29/wwpdb/apps/releasemodule/depict/DepictCitation_v2.py` & `wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/depict/DepictCitation_v2.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.releasemodule-0.29/wwpdb/apps/releasemodule/depict/DepictEntryHistory.py` & `wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/depict/DepictEntryHistory.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.releasemodule-0.29/wwpdb/apps/releasemodule/depict/DepictReleaseInfo.py` & `wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/depict/DepictReleaseInfo.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.releasemodule-0.29/wwpdb/apps/releasemodule/depict/DepictRemovalMark.py` & `wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/depict/DepictRemovalMark.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.releasemodule-0.29/wwpdb/apps/releasemodule/depict/DepictRequest.py` & `wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/depict/DepictRequest.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.releasemodule-0.29/wwpdb/apps/releasemodule/depict/ReleaseOption_v2.py` & `wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/depict/ReleaseOption_v2.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.releasemodule-0.29/wwpdb/apps/releasemodule/depict/test_DepictCitation.py` & `wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/depict/test_DepictCitation.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.releasemodule-0.29/wwpdb/apps/releasemodule/update/AutoReRelease.py` & `wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/update/AutoReRelease.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.releasemodule-0.29/wwpdb/apps/releasemodule/update/CitationFormParser_v2.py` & `wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/update/CitationFormParser_v2.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.releasemodule-0.29/wwpdb/apps/releasemodule/update/EmReleaseUtil.py` & `wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/update/EmReleaseUtil.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.releasemodule-0.29/wwpdb/apps/releasemodule/update/EntryFormParser_v2.py` & `wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/update/EntryFormParser_v2.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.releasemodule-0.29/wwpdb/apps/releasemodule/update/EntryPullProcess.py` & `wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/update/EntryPullProcess.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.releasemodule-0.29/wwpdb/apps/releasemodule/update/EntryUpdateBase.py` & `wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/update/EntryUpdateBase.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.releasemodule-0.29/wwpdb/apps/releasemodule/update/EntryUpdateProcess.py` & `wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/update/EntryUpdateProcess.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.releasemodule-0.29/wwpdb/apps/releasemodule/update/InputFormParser_v2.py` & `wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/update/InputFormParser_v2.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.releasemodule-0.29/wwpdb/apps/releasemodule/update/MultiUpdateProcess.py` & `wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/update/MultiUpdateProcess.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.releasemodule-0.29/wwpdb/apps/releasemodule/update/NmrDataGenerator.py` & `wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/update/NmrDataGenerator.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.releasemodule-0.29/wwpdb/apps/releasemodule/update/ReleaseDpUtil.py` & `wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/update/ReleaseDpUtil.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.releasemodule-0.29/wwpdb/apps/releasemodule/update/ReleaseUtil.py` & `wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/update/ReleaseUtil.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.releasemodule-0.29/wwpdb/apps/releasemodule/update/RunAutoReReleaseProcess.py` & `wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/update/RunAutoReReleaseProcess.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.releasemodule-0.29/wwpdb/apps/releasemodule/update/UpdateBase.py` & `wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/update/UpdateBase.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.releasemodule-0.29/wwpdb/apps/releasemodule/update/UpdateFormParser.py` & `wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/update/UpdateFormParser.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.releasemodule-0.29/wwpdb/apps/releasemodule/update/UpdateUtil_v2.py` & `wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/update/UpdateUtil_v2.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.releasemodule-0.29/wwpdb/apps/releasemodule/utils/CombineDbApi.py` & `wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/utils/CombineDbApi.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.releasemodule-0.29/wwpdb/apps/releasemodule/utils/ContentDbApi.py` & `wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/utils/ContentDbApi.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.releasemodule-0.29/wwpdb/apps/releasemodule/utils/DbApiUtil.py` & `wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/utils/DbApiUtil.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.releasemodule-0.29/wwpdb/apps/releasemodule/utils/JournalAbbrev.py` & `wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/utils/JournalAbbrev.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.releasemodule-0.29/wwpdb/apps/releasemodule/utils/MessageBaseClass.py` & `wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/utils/MessageBaseClass.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.releasemodule-0.29/wwpdb/apps/releasemodule/utils/ModuleBaseClass.py` & `wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/utils/ModuleBaseClass.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.releasemodule-0.29/wwpdb/apps/releasemodule/utils/MultiProcLimit.py` & `wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/utils/MultiProcLimit.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.releasemodule-0.29/wwpdb/apps/releasemodule/utils/StatusDbApi_v2.py` & `wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/utils/StatusDbApi_v2.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.releasemodule-0.29/wwpdb/apps/releasemodule/utils/TimeUtil.py` & `wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/utils/TimeUtil.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.releasemodule-0.29/wwpdb/apps/releasemodule/utils/Utility.py` & `wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/utils/Utility.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.releasemodule-0.29/wwpdb/apps/releasemodule/webapp/ReleaseWebApp_v2.py` & `wwpdb.apps.releasemodule-0.29.dev1/wwpdb/apps/releasemodule/webapp/ReleaseWebApp_v2.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.releasemodule-0.29/wwpdb.apps.releasemodule.egg-info/PKG-INFO` & `wwpdb.apps.releasemodule-0.29.dev1/wwpdb.apps.releasemodule.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wwpdb.apps.releasemodule
-Version: 0.29
+Version: 0.29.dev1
 Summary: wwPDB sequence module
 Home-page: https://github.com/rcsb/py-wwpdb_apps_releasemodule
 Author: Ezra Peisach
 Author-email: ezra.peisach@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `wwpdb.apps.releasemodule-0.29/wwpdb.apps.releasemodule.egg-info/SOURCES.txt` & `wwpdb.apps.releasemodule-0.29.dev1/wwpdb.apps.releasemodule.egg-info/SOURCES.txt`

 * *Files identical despite different names*

