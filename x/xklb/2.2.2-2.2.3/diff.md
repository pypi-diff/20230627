# Comparing `tmp/xklb-2.2.2.tar.gz` & `tmp/xklb-2.2.3.tar.gz`

## Comparing `xklb-2.2.2.tar` & `xklb-2.2.3.tar`

### file list

```diff
@@ -1,72 +1,72 @@
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 xklb-2.2.2/.gitattributes
--rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 xklb-2.2.2/TODO
--rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 xklb-2.2.2/Windows.md
--rw-r--r--   0        0        0   529514 2020-02-02 00:00:00.000000 xklb-2.2.2/pdm.lock
--rw-r--r--   0        0        0    13927 2020-02-02 00:00:00.000000 xklb-2.2.2/readme.py
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 xklb-2.2.2/.github/FUNDING.yml
--rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 xklb-2.2.2/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 xklb-2.2.2/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 xklb-2.2.2/.github/workflows/green.yaml
--rw-r--r--   0        0        0     1597 2020-02-02 00:00:00.000000 xklb-2.2.2/.github/workflows/push.yaml
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 xklb-2.2.2/xklb/__init__.py
--rw-r--r--   0        0        0     8679 2020-02-02 00:00:00.000000 xklb-2.2.2/xklb/av.py
--rw-r--r--   0        0        0     6921 2020-02-02 00:00:00.000000 xklb-2.2.2/xklb/books.py
--rw-r--r--   0        0        0     9417 2020-02-02 00:00:00.000000 xklb-2.2.2/xklb/consts.py
--rw-r--r--   0        0        0     8460 2020-02-02 00:00:00.000000 xklb-2.2.2/xklb/db.py
--rw-r--r--   0        0        0     7095 2020-02-02 00:00:00.000000 xklb-2.2.2/xklb/dl_config.py
--rw-r--r--   0        0        0    11051 2020-02-02 00:00:00.000000 xklb-2.2.2/xklb/dl_extract.py
--rw-r--r--   0        0        0    13784 2020-02-02 00:00:00.000000 xklb-2.2.2/xklb/fs_extract.py
--rw-r--r--   0        0        0     7481 2020-02-02 00:00:00.000000 xklb-2.2.2/xklb/gdl_backend.py
--rw-r--r--   0        0        0     4041 2020-02-02 00:00:00.000000 xklb-2.2.2/xklb/gdl_extract.py
--rw-r--r--   0        0        0     6212 2020-02-02 00:00:00.000000 xklb-2.2.2/xklb/gui.py
--rw-r--r--   0        0        0      808 2020-02-02 00:00:00.000000 xklb-2.2.2/xklb/history.py
--rw-r--r--   0        0        0     5712 2020-02-02 00:00:00.000000 xklb-2.2.2/xklb/hn_extract.py
--rw-r--r--   0        0        0    12585 2020-02-02 00:00:00.000000 xklb-2.2.2/xklb/lb.py
--rw-r--r--   0        0        0     7599 2020-02-02 00:00:00.000000 xklb-2.2.2/xklb/media.py
--rw-r--r--   0        0        0    26986 2020-02-02 00:00:00.000000 xklb-2.2.2/xklb/play_actions.py
--rw-r--r--   0        0        0    36936 2020-02-02 00:00:00.000000 xklb-2.2.2/xklb/player.py
--rw-r--r--   0        0        0     5232 2020-02-02 00:00:00.000000 xklb-2.2.2/xklb/playlists.py
--rw-r--r--   0        0        0    13549 2020-02-02 00:00:00.000000 xklb-2.2.2/xklb/praw_extract.py
--rw-r--r--   0        0        0     7997 2020-02-02 00:00:00.000000 xklb-2.2.2/xklb/search.py
--rw-r--r--   0        0        0     4639 2020-02-02 00:00:00.000000 xklb-2.2.2/xklb/subtitle.py
--rw-r--r--   0        0        0     6511 2020-02-02 00:00:00.000000 xklb-2.2.2/xklb/tabs_actions.py
--rw-r--r--   0        0        0     2789 2020-02-02 00:00:00.000000 xklb-2.2.2/xklb/tabs_extract.py
--rw-r--r--   0        0        0    15676 2020-02-02 00:00:00.000000 xklb-2.2.2/xklb/tube_backend.py
--rw-r--r--   0        0        0     4944 2020-02-02 00:00:00.000000 xklb-2.2.2/xklb/tube_extract.py
--rw-r--r--   0        0        0    85450 2020-02-02 00:00:00.000000 xklb-2.2.2/xklb/usage.py
--rw-r--r--   0        0        0    41694 2020-02-02 00:00:00.000000 xklb-2.2.2/xklb/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.2.2/xklb/scripts/__init__.py
--rw-r--r--   0        0        0     6087 2020-02-02 00:00:00.000000 xklb-2.2.2/xklb/scripts/bigdirs.py
--rw-r--r--   0        0        0     7257 2020-02-02 00:00:00.000000 xklb-2.2.2/xklb/scripts/block.py
--rw-r--r--   0        0        0     2437 2020-02-02 00:00:00.000000 xklb-2.2.2/xklb/scripts/christen.py
--rw-r--r--   0        0        0     3975 2020-02-02 00:00:00.000000 xklb-2.2.2/xklb/scripts/cluster_sort.py
--rw-r--r--   0        0        0     3215 2020-02-02 00:00:00.000000 xklb-2.2.2/xklb/scripts/copy_play_counts.py
--rw-r--r--   0        0        0     8198 2020-02-02 00:00:00.000000 xklb-2.2.2/xklb/scripts/dedupe.py
--rw-r--r--   0        0        0     4077 2020-02-02 00:00:00.000000 xklb-2.2.2/xklb/scripts/dedupe_db.py
--rw-r--r--   0        0        0     6891 2020-02-02 00:00:00.000000 xklb-2.2.2/xklb/scripts/disk_usage.py
--rw-r--r--   0        0        0     5415 2020-02-02 00:00:00.000000 xklb-2.2.2/xklb/scripts/download_status.py
--rw-r--r--   0        0        0     6411 2020-02-02 00:00:00.000000 xklb-2.2.2/xklb/scripts/history.py
--rw-r--r--   0        0        0     2686 2020-02-02 00:00:00.000000 xklb-2.2.2/xklb/scripts/merge_dbs.py
--rw-r--r--   0        0        0     3807 2020-02-02 00:00:00.000000 xklb-2.2.2/xklb/scripts/merge_online_local.py
--rw-r--r--   0        0        0     7066 2020-02-02 00:00:00.000000 xklb-2.2.2/xklb/scripts/move_list.py
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 xklb-2.2.2/xklb/scripts/optimize_db.py
--rw-r--r--   0        0        0     1945 2020-02-02 00:00:00.000000 xklb-2.2.2/xklb/scripts/places_import.py
--rw-r--r--   0        0        0     4560 2020-02-02 00:00:00.000000 xklb-2.2.2/xklb/scripts/playback_control.py
--rw-r--r--   0        0        0     5668 2020-02-02 00:00:00.000000 xklb-2.2.2/xklb/scripts/playlists.py
--rw-r--r--   0        0        0     6003 2020-02-02 00:00:00.000000 xklb-2.2.2/xklb/scripts/redownload.py
--rw-r--r--   0        0        0     2224 2020-02-02 00:00:00.000000 xklb-2.2.2/xklb/scripts/relmv.py
--rw-r--r--   0        0        0    10044 2020-02-02 00:00:00.000000 xklb-2.2.2/xklb/scripts/scatter.py
--rw-r--r--   0        0        0     2340 2020-02-02 00:00:00.000000 xklb-2.2.2/xklb/scripts/streaming_tab_loader.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.2.2/xklb/scripts/mining/__init__.py
--rw-r--r--   0        0        0    17101 2020-02-02 00:00:00.000000 xklb-2.2.2/xklb/scripts/mining/data.py
--rw-r--r--   0        0        0     3024 2020-02-02 00:00:00.000000 xklb-2.2.2/xklb/scripts/mining/extract_links.py
--rw-r--r--   0        0        0     1812 2020-02-02 00:00:00.000000 xklb-2.2.2/xklb/scripts/mining/mpv_watchlater.py
--rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 xklb-2.2.2/xklb/scripts/mining/nouns.py
--rw-r--r--   0        0        0     2159 2020-02-02 00:00:00.000000 xklb-2.2.2/xklb/scripts/mining/pushshift.py
--rw-r--r--   0        0        0     2163 2020-02-02 00:00:00.000000 xklb-2.2.2/xklb/scripts/mining/reddit_selftext.py
--rw-r--r--   0        0        0     8385 2020-02-02 00:00:00.000000 xklb-2.2.2/xklb/assets/kotobago.png
--rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 xklb-2.2.2/.gitignore
--rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 xklb-2.2.2/LICENSE
--rw-r--r--   0        0        0    97135 2020-02-02 00:00:00.000000 xklb-2.2.2/README.md
--rw-r--r--   0        0        0     2749 2020-02-02 00:00:00.000000 xklb-2.2.2/pyproject.toml
--rw-r--r--   0        0        0   100770 2020-02-02 00:00:00.000000 xklb-2.2.2/PKG-INFO
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 xklb-2.2.3/.gitattributes
+-rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 xklb-2.2.3/TODO
+-rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 xklb-2.2.3/Windows.md
+-rw-r--r--   0        0        0   529514 2020-02-02 00:00:00.000000 xklb-2.2.3/pdm.lock
+-rw-r--r--   0        0        0    13927 2020-02-02 00:00:00.000000 xklb-2.2.3/readme.py
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 xklb-2.2.3/.github/FUNDING.yml
+-rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 xklb-2.2.3/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 xklb-2.2.3/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 xklb-2.2.3/.github/workflows/green.yaml
+-rw-r--r--   0        0        0     1597 2020-02-02 00:00:00.000000 xklb-2.2.3/.github/workflows/push.yaml
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 xklb-2.2.3/xklb/__init__.py
+-rw-r--r--   0        0        0     8679 2020-02-02 00:00:00.000000 xklb-2.2.3/xklb/av.py
+-rw-r--r--   0        0        0     6921 2020-02-02 00:00:00.000000 xklb-2.2.3/xklb/books.py
+-rw-r--r--   0        0        0     9417 2020-02-02 00:00:00.000000 xklb-2.2.3/xklb/consts.py
+-rw-r--r--   0        0        0     8460 2020-02-02 00:00:00.000000 xklb-2.2.3/xklb/db.py
+-rw-r--r--   0        0        0     7095 2020-02-02 00:00:00.000000 xklb-2.2.3/xklb/dl_config.py
+-rw-r--r--   0        0        0    11059 2020-02-02 00:00:00.000000 xklb-2.2.3/xklb/dl_extract.py
+-rw-r--r--   0        0        0    13784 2020-02-02 00:00:00.000000 xklb-2.2.3/xklb/fs_extract.py
+-rw-r--r--   0        0        0     7481 2020-02-02 00:00:00.000000 xklb-2.2.3/xklb/gdl_backend.py
+-rw-r--r--   0        0        0     3987 2020-02-02 00:00:00.000000 xklb-2.2.3/xklb/gdl_extract.py
+-rw-r--r--   0        0        0     6212 2020-02-02 00:00:00.000000 xklb-2.2.3/xklb/gui.py
+-rw-r--r--   0        0        0      808 2020-02-02 00:00:00.000000 xklb-2.2.3/xklb/history.py
+-rw-r--r--   0        0        0     5712 2020-02-02 00:00:00.000000 xklb-2.2.3/xklb/hn_extract.py
+-rw-r--r--   0        0        0    12585 2020-02-02 00:00:00.000000 xklb-2.2.3/xklb/lb.py
+-rw-r--r--   0        0        0     7599 2020-02-02 00:00:00.000000 xklb-2.2.3/xklb/media.py
+-rw-r--r--   0        0        0    26986 2020-02-02 00:00:00.000000 xklb-2.2.3/xklb/play_actions.py
+-rw-r--r--   0        0        0    36936 2020-02-02 00:00:00.000000 xklb-2.2.3/xklb/player.py
+-rw-r--r--   0        0        0     5232 2020-02-02 00:00:00.000000 xklb-2.2.3/xklb/playlists.py
+-rw-r--r--   0        0        0    13481 2020-02-02 00:00:00.000000 xklb-2.2.3/xklb/praw_extract.py
+-rw-r--r--   0        0        0     7997 2020-02-02 00:00:00.000000 xklb-2.2.3/xklb/search.py
+-rw-r--r--   0        0        0     4639 2020-02-02 00:00:00.000000 xklb-2.2.3/xklb/subtitle.py
+-rw-r--r--   0        0        0     6511 2020-02-02 00:00:00.000000 xklb-2.2.3/xklb/tabs_actions.py
+-rw-r--r--   0        0        0     2789 2020-02-02 00:00:00.000000 xklb-2.2.3/xklb/tabs_extract.py
+-rw-r--r--   0        0        0    15676 2020-02-02 00:00:00.000000 xklb-2.2.3/xklb/tube_backend.py
+-rw-r--r--   0        0        0     4954 2020-02-02 00:00:00.000000 xklb-2.2.3/xklb/tube_extract.py
+-rw-r--r--   0        0        0    85450 2020-02-02 00:00:00.000000 xklb-2.2.3/xklb/usage.py
+-rw-r--r--   0        0        0    41694 2020-02-02 00:00:00.000000 xklb-2.2.3/xklb/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.2.3/xklb/scripts/__init__.py
+-rw-r--r--   0        0        0     6087 2020-02-02 00:00:00.000000 xklb-2.2.3/xklb/scripts/bigdirs.py
+-rw-r--r--   0        0        0     7257 2020-02-02 00:00:00.000000 xklb-2.2.3/xklb/scripts/block.py
+-rw-r--r--   0        0        0     2437 2020-02-02 00:00:00.000000 xklb-2.2.3/xklb/scripts/christen.py
+-rw-r--r--   0        0        0     3975 2020-02-02 00:00:00.000000 xklb-2.2.3/xklb/scripts/cluster_sort.py
+-rw-r--r--   0        0        0     3215 2020-02-02 00:00:00.000000 xklb-2.2.3/xklb/scripts/copy_play_counts.py
+-rw-r--r--   0        0        0     8198 2020-02-02 00:00:00.000000 xklb-2.2.3/xklb/scripts/dedupe.py
+-rw-r--r--   0        0        0     4077 2020-02-02 00:00:00.000000 xklb-2.2.3/xklb/scripts/dedupe_db.py
+-rw-r--r--   0        0        0     6891 2020-02-02 00:00:00.000000 xklb-2.2.3/xklb/scripts/disk_usage.py
+-rw-r--r--   0        0        0     5454 2020-02-02 00:00:00.000000 xklb-2.2.3/xklb/scripts/download_status.py
+-rw-r--r--   0        0        0     6411 2020-02-02 00:00:00.000000 xklb-2.2.3/xklb/scripts/history.py
+-rw-r--r--   0        0        0     2686 2020-02-02 00:00:00.000000 xklb-2.2.3/xklb/scripts/merge_dbs.py
+-rw-r--r--   0        0        0     3807 2020-02-02 00:00:00.000000 xklb-2.2.3/xklb/scripts/merge_online_local.py
+-rw-r--r--   0        0        0     7066 2020-02-02 00:00:00.000000 xklb-2.2.3/xklb/scripts/move_list.py
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 xklb-2.2.3/xklb/scripts/optimize_db.py
+-rw-r--r--   0        0        0     1945 2020-02-02 00:00:00.000000 xklb-2.2.3/xklb/scripts/places_import.py
+-rw-r--r--   0        0        0     4560 2020-02-02 00:00:00.000000 xklb-2.2.3/xklb/scripts/playback_control.py
+-rw-r--r--   0        0        0     5668 2020-02-02 00:00:00.000000 xklb-2.2.3/xklb/scripts/playlists.py
+-rw-r--r--   0        0        0     6003 2020-02-02 00:00:00.000000 xklb-2.2.3/xklb/scripts/redownload.py
+-rw-r--r--   0        0        0     2224 2020-02-02 00:00:00.000000 xklb-2.2.3/xklb/scripts/relmv.py
+-rw-r--r--   0        0        0    10044 2020-02-02 00:00:00.000000 xklb-2.2.3/xklb/scripts/scatter.py
+-rw-r--r--   0        0        0     2340 2020-02-02 00:00:00.000000 xklb-2.2.3/xklb/scripts/streaming_tab_loader.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.2.3/xklb/scripts/mining/__init__.py
+-rw-r--r--   0        0        0    17101 2020-02-02 00:00:00.000000 xklb-2.2.3/xklb/scripts/mining/data.py
+-rw-r--r--   0        0        0     3024 2020-02-02 00:00:00.000000 xklb-2.2.3/xklb/scripts/mining/extract_links.py
+-rw-r--r--   0        0        0     1812 2020-02-02 00:00:00.000000 xklb-2.2.3/xklb/scripts/mining/mpv_watchlater.py
+-rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 xklb-2.2.3/xklb/scripts/mining/nouns.py
+-rw-r--r--   0        0        0     2159 2020-02-02 00:00:00.000000 xklb-2.2.3/xklb/scripts/mining/pushshift.py
+-rw-r--r--   0        0        0     2163 2020-02-02 00:00:00.000000 xklb-2.2.3/xklb/scripts/mining/reddit_selftext.py
+-rw-r--r--   0        0        0     8385 2020-02-02 00:00:00.000000 xklb-2.2.3/xklb/assets/kotobago.png
+-rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 xklb-2.2.3/.gitignore
+-rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 xklb-2.2.3/LICENSE
+-rw-r--r--   0        0        0    97135 2020-02-02 00:00:00.000000 xklb-2.2.3/README.md
+-rw-r--r--   0        0        0     2749 2020-02-02 00:00:00.000000 xklb-2.2.3/pyproject.toml
+-rw-r--r--   0        0        0   100770 2020-02-02 00:00:00.000000 xklb-2.2.3/PKG-INFO
```

### Comparing `xklb-2.2.2/TODO` & `xklb-2.2.3/TODO`

 * *Files identical despite different names*

### Comparing `xklb-2.2.2/Windows.md` & `xklb-2.2.3/Windows.md`

 * *Files identical despite different names*

### Comparing `xklb-2.2.2/pdm.lock` & `xklb-2.2.3/pdm.lock`

 * *Files identical despite different names*

### Comparing `xklb-2.2.2/readme.py` & `xklb-2.2.3/readme.py`

 * *Files identical despite different names*

### Comparing `xklb-2.2.2/.github/ISSUE_TEMPLATE/bug_report.md` & `xklb-2.2.3/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `xklb-2.2.2/.github/ISSUE_TEMPLATE/feature_request.md` & `xklb-2.2.3/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `xklb-2.2.2/.github/workflows/push.yaml` & `xklb-2.2.3/.github/workflows/push.yaml`

 * *Files identical despite different names*

### Comparing `xklb-2.2.2/xklb/av.py` & `xklb-2.2.3/xklb/av.py`

 * *Files identical despite different names*

### Comparing `xklb-2.2.2/xklb/books.py` & `xklb-2.2.3/xklb/books.py`

 * *Files identical despite different names*

### Comparing `xklb-2.2.2/xklb/consts.py` & `xklb-2.2.3/xklb/consts.py`

 * *Files identical despite different names*

### Comparing `xklb-2.2.2/xklb/db.py` & `xklb-2.2.3/xklb/db.py`

 * *Files identical despite different names*

### Comparing `xklb-2.2.2/xklb/dl_config.py` & `xklb-2.2.3/xklb/dl_config.py`

 * *Files identical despite different names*

### Comparing `xklb-2.2.2/xklb/dl_extract.py` & `xklb-2.2.3/xklb/dl_extract.py`

 * *Files 0% similar despite different names*

```diff
@@ -160,15 +160,15 @@
                 and COALESCE(m.time_downloaded,0) = 0
                 and COALESCE(m.time_deleted,0) = 0
                 {'and COALESCE(p.time_deleted, 0) = 0' if 'time_deleted' in pl_columns else ''}
                 and m.path like "http%"
                 {'AND (score IS NULL OR score > 7)' if 'score' in m_columns else ''}
                 {'AND (upvote_ratio IS NULL OR upvote_ratio > 0.73)' if 'upvote_ratio' in m_columns else ''}
                 {" ".join(args.filter_sql)}
-            GROUP BY m.playlist_id
+            GROUP BY m.playlist_id, m.path
             ORDER BY 1=1
                 , COALESCE(m.time_modified, 0) = 0 DESC
                 , m.time_modified
                 {', ' + args.sort if args.sort else ''}
                 , random()
             {LIMIT}
         """
```

### Comparing `xklb-2.2.2/xklb/fs_extract.py` & `xklb-2.2.3/xklb/fs_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-2.2.2/xklb/gdl_backend.py` & `xklb-2.2.3/xklb/gdl_backend.py`

 * *Files identical despite different names*

### Comparing `xklb-2.2.2/xklb/gdl_extract.py` & `xklb-2.2.3/xklb/gdl_extract.py`

 * *Files 5% similar despite different names*

```diff
@@ -69,37 +69,35 @@
 
 def gallery_add(args=None) -> None:
     if args:
         sys.argv = ["galleryadd", *args]
 
     args = parse_args(SC.galleryadd, usage=usage.galleryadd)
 
-    known_playlists = set()
-    if not args.force and len(args.playlists) > 9:
-        known_playlists = media.get_paths(args)
-
-    added_media_count = len(args.playlists)
-    for path in args.playlists:
-        if path in known_playlists:
-            log.info("[%s]: Already added. Skipping!", path)
-            continue
-
-        if args.safe and not gdl_backend.is_supported(args, path):
-            log.info("[%s]: Skipping unsupported playlist (safe_mode)", path)
-            continue
-
-        if args.insert_only:
-            args.db["media"].insert({"path": path}, alter=True, ignore=True, pk="path")
-        elif args.insert_only_playlists:
-            args.db["playlists"].insert({"path": path}, alter=True, ignore=True, pk="path")
-        else:
-            added_media_count += gdl_backend.get_playlist_metadata(args, path)
+    if args.insert_only:
+        args.db["media"].insert_all([{"path": p} for p in args.playlists], alter=True, ignore=True, pk="path")
+    elif args.insert_only_playlists:
+        args.db["playlists"].insert_all([{"path": p} for p in args.playlists], alter=True, ignore=True, pk="path")
+    else:
+        known_playlists = set()
+        if not args.force and len(args.playlists) > 9:
+            known_playlists = media.get_paths(args)
+
+        for path in args.playlists:
+            if path in known_playlists:
+                log.info("[%s]: Already added. Skipping!", path)
+                continue
+
+            if args.safe and not gdl_backend.is_supported(args, path):
+                log.info("[%s]: Skipping unsupported playlist (safe_mode)", path)
+                continue
 
-    LARGE_NUMBER = 100_000
-    if not args.db["media"].detect_fts() or added_media_count > LARGE_NUMBER:
+            gdl_backend.get_playlist_metadata(args, path)
+
+    if not args.db["media"].detect_fts():
         db.optimize(args)
 
 
 def gallery_update(args=None) -> None:
     if args:
         sys.argv = ["galleryupdate", *args]
```

### Comparing `xklb-2.2.2/xklb/gui.py` & `xklb-2.2.3/xklb/gui.py`

 * *Files identical despite different names*

### Comparing `xklb-2.2.2/xklb/history.py` & `xklb-2.2.3/xklb/history.py`

 * *Files identical despite different names*

### Comparing `xklb-2.2.2/xklb/hn_extract.py` & `xklb-2.2.3/xklb/hn_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-2.2.2/xklb/lb.py` & `xklb-2.2.3/xklb/lb.py`

 * *Files identical despite different names*

### Comparing `xklb-2.2.2/xklb/media.py` & `xklb-2.2.3/xklb/media.py`

 * *Files identical despite different names*

### Comparing `xklb-2.2.2/xklb/play_actions.py` & `xklb-2.2.3/xklb/play_actions.py`

 * *Files identical despite different names*

### Comparing `xklb-2.2.2/xklb/player.py` & `xklb-2.2.3/xklb/player.py`

 * *Files identical despite different names*

### Comparing `xklb-2.2.2/xklb/playlists.py` & `xklb-2.2.3/xklb/playlists.py`

 * *Files identical despite different names*

### Comparing `xklb-2.2.2/xklb/praw_extract.py` & `xklb-2.2.3/xklb/praw_extract.py`

 * *Files 1% similar despite different names*

```diff
@@ -371,16 +371,15 @@
                     "time_deleted": 0,
                 },
             ),
         )
 
     process_subreddits(args, subreddits)
     process_redditors(args, redditors)
-    LARGE_NUMBER = 75
-    if not args.db["media"].detect_fts() or len(subreddits + redditors) > LARGE_NUMBER:
+    if not args.db["media"].detect_fts():
         db.optimize(args)
 
 
 def reddit_update(args=None) -> None:
     if args:
         sys.argv = ["lb", *args]
```

### Comparing `xklb-2.2.2/xklb/search.py` & `xklb-2.2.3/xklb/search.py`

 * *Files identical despite different names*

### Comparing `xklb-2.2.2/xklb/subtitle.py` & `xklb-2.2.3/xklb/subtitle.py`

 * *Files identical despite different names*

### Comparing `xklb-2.2.2/xklb/tabs_actions.py` & `xklb-2.2.3/xklb/tabs_actions.py`

 * *Files identical despite different names*

### Comparing `xklb-2.2.2/xklb/tabs_extract.py` & `xklb-2.2.3/xklb/tabs_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-2.2.2/xklb/tube_backend.py` & `xklb-2.2.3/xklb/tube_backend.py`

 * *Files identical despite different names*

### Comparing `xklb-2.2.2/xklb/tube_extract.py` & `xklb-2.2.3/xklb/tube_extract.py`

 * *Files 6% similar despite different names*

```diff
@@ -74,40 +74,39 @@
 
 def tube_add(args=None) -> None:
     if args:
         sys.argv = ["tubeadd", *args]
 
     args = parse_args(SC.tubeadd, usage=usage.tubeadd)
 
-    known_playlists = set()
-    if not args.force and len(args.playlists) > 9:
-        known_playlists = media.get_paths(args)
-
-    for path in args.playlists:
-        if args.safe and not tube_backend.is_supported(path):
-            log.info("[%s]: Skipping unsupported playlist (safe_mode)", path)
-            continue
-
-        if path in known_playlists:
-            log.info("[%s]: Already added. Skipping!", path)
-            continue
-
-        if args.insert_only:
-            args.db["media"].insert({"path": path}, alter=True, ignore=True, pk="path")
-        elif args.insert_only_playlists:
-            args.db["playlists"].insert({"path": path}, alter=True, ignore=True, pk="path")
-        else:
+    if args.insert_only:
+        args.db["media"].insert_all([{"path": p} for p in args.playlists], alter=True, ignore=True, pk="path")
+    elif args.insert_only_playlists:
+        args.db["playlists"].insert_all([{"path": p} for p in args.playlists], alter=True, ignore=True, pk="path")
+    else:
+        known_playlists = set()
+        if not args.force and len(args.playlists) > 9:
+            known_playlists = media.get_paths(args)
+
+        for path in args.playlists:
+            if args.safe and not tube_backend.is_supported(path):
+                log.info("[%s]: Skipping unsupported playlist (safe_mode)", path)
+                continue
+
+            if path in known_playlists:
+                log.info("[%s]: Already added. Skipping!", path)
+                continue
+
             tube_backend.get_playlist_metadata(args, path, tube_backend.tube_opts(args))
 
-        if args.extra:
-            log.warning("[%s]: Getting extra metadata", path)
-            tube_backend.get_extra_metadata(args, path)
+            if args.extra:
+                log.warning("[%s]: Getting extra metadata", path)
+                tube_backend.get_extra_metadata(args, path)
 
-    LARGE_NUMBER = 100_000
-    if not args.db["media"].detect_fts() or tube_backend.added_media_count > LARGE_NUMBER:
+    if not args.db["media"].detect_fts():
         db.optimize(args)
 
 
 def tube_update(args=None) -> None:
     if args:
         sys.argv = ["tubeupdate", *args]
```

### Comparing `xklb-2.2.2/xklb/usage.py` & `xklb-2.2.3/xklb/usage.py`

 * *Files identical despite different names*

### Comparing `xklb-2.2.2/xklb/utils.py` & `xklb-2.2.3/xklb/utils.py`

 * *Files identical despite different names*

### Comparing `xklb-2.2.2/xklb/scripts/bigdirs.py` & `xklb-2.2.3/xklb/scripts/bigdirs.py`

 * *Files identical despite different names*

### Comparing `xklb-2.2.2/xklb/scripts/block.py` & `xklb-2.2.3/xklb/scripts/block.py`

 * *Files identical despite different names*

### Comparing `xklb-2.2.2/xklb/scripts/christen.py` & `xklb-2.2.3/xklb/scripts/christen.py`

 * *Files identical despite different names*

### Comparing `xklb-2.2.2/xklb/scripts/cluster_sort.py` & `xklb-2.2.3/xklb/scripts/cluster_sort.py`

 * *Files identical despite different names*

### Comparing `xklb-2.2.2/xklb/scripts/copy_play_counts.py` & `xklb-2.2.3/xklb/scripts/copy_play_counts.py`

 * *Files identical despite different names*

### Comparing `xklb-2.2.2/xklb/scripts/dedupe.py` & `xklb-2.2.3/xklb/scripts/dedupe.py`

 * *Files identical despite different names*

### Comparing `xklb-2.2.2/xklb/scripts/dedupe_db.py` & `xklb-2.2.3/xklb/scripts/dedupe_db.py`

 * *Files identical despite different names*

### Comparing `xklb-2.2.2/xklb/scripts/disk_usage.py` & `xklb-2.2.3/xklb/scripts/disk_usage.py`

 * *Files identical despite different names*

### Comparing `xklb-2.2.2/xklb/scripts/download_status.py` & `xklb-2.2.3/xklb/scripts/download_status.py`

 * *Files 2% similar despite different names*

```diff
@@ -99,24 +99,24 @@
             args.db.register_function(tube_backend.is_supported, deterministic=True)
             count_paths = "count(*) FILTER(WHERE COALESCE(time_modified,0) = 0 and is_supported(path)) never_downloaded"
         else:
             count_paths = "count(*) FILTER(WHERE COALESCE(time_modified,0) = 0) never_downloaded"
 
     query = f"""select
         {count_paths}
-        , extractor_key
+        , COALESCE(extractor_key, 'Unknown') extractor_key
         {', sum(duration) duration' if 'duration' in query else ''}
         {', count(*) FILTER(WHERE COALESCE(time_modified,0) > 0 AND error IS NOT NULL) errors' if 'error' in query else ''}
         {', group_concat(distinct error) error_descriptions' if 'error' in query and args.verbose >= 1 else ''}
     from ({query})
     where 1=1
         and COALESCE(time_downloaded,0) = 0
         and COALESCE(time_deleted,0) = 0
     group by extractor_key
-    order by never_downloaded"""
+    order by never_downloaded DESC"""
 
     printer(args, query, bindings)
 
     if "error" in db.columns(args, "media"):
         query = """
         select error, count(*) count
         from media
@@ -125,15 +125,15 @@
         order by 2
         """
         errors = list(args.db.query(query))
 
         common_errors = []
         other_errors = []
         for error in errors:
-            if error["count"] == 1:
+            if error["count"] < 5:
                 other_errors.append(error)
             else:
                 common_errors.append(error)
 
         common_errors.append({"error": "Other", "count": len(other_errors)})
         common_errors.append({"error": "Total", "count": sum(d["count"] for d in errors)})
         print(tabulate(common_errors, tablefmt=consts.TABULATE_STYLE, headers="keys", showindex=False))
```

### Comparing `xklb-2.2.2/xklb/scripts/history.py` & `xklb-2.2.3/xklb/scripts/history.py`

 * *Files identical despite different names*

### Comparing `xklb-2.2.2/xklb/scripts/merge_dbs.py` & `xklb-2.2.3/xklb/scripts/merge_dbs.py`

 * *Files identical despite different names*

### Comparing `xklb-2.2.2/xklb/scripts/merge_online_local.py` & `xklb-2.2.3/xklb/scripts/merge_online_local.py`

 * *Files identical despite different names*

### Comparing `xklb-2.2.2/xklb/scripts/move_list.py` & `xklb-2.2.3/xklb/scripts/move_list.py`

 * *Files identical despite different names*

### Comparing `xklb-2.2.2/xklb/scripts/optimize_db.py` & `xklb-2.2.3/xklb/scripts/optimize_db.py`

 * *Files identical despite different names*

### Comparing `xklb-2.2.2/xklb/scripts/places_import.py` & `xklb-2.2.3/xklb/scripts/places_import.py`

 * *Files identical despite different names*

### Comparing `xklb-2.2.2/xklb/scripts/playback_control.py` & `xklb-2.2.3/xklb/scripts/playback_control.py`

 * *Files identical despite different names*

### Comparing `xklb-2.2.2/xklb/scripts/playlists.py` & `xklb-2.2.3/xklb/scripts/playlists.py`

 * *Files identical despite different names*

### Comparing `xklb-2.2.2/xklb/scripts/redownload.py` & `xklb-2.2.3/xklb/scripts/redownload.py`

 * *Files identical despite different names*

### Comparing `xklb-2.2.2/xklb/scripts/relmv.py` & `xklb-2.2.3/xklb/scripts/relmv.py`

 * *Files identical despite different names*

### Comparing `xklb-2.2.2/xklb/scripts/scatter.py` & `xklb-2.2.3/xklb/scripts/scatter.py`

 * *Files identical despite different names*

### Comparing `xklb-2.2.2/xklb/scripts/streaming_tab_loader.py` & `xklb-2.2.3/xklb/scripts/streaming_tab_loader.py`

 * *Files identical despite different names*

### Comparing `xklb-2.2.2/xklb/scripts/mining/data.py` & `xklb-2.2.3/xklb/scripts/mining/data.py`

 * *Files identical despite different names*

### Comparing `xklb-2.2.2/xklb/scripts/mining/extract_links.py` & `xklb-2.2.3/xklb/scripts/mining/extract_links.py`

 * *Files identical despite different names*

### Comparing `xklb-2.2.2/xklb/scripts/mining/mpv_watchlater.py` & `xklb-2.2.3/xklb/scripts/mining/mpv_watchlater.py`

 * *Files identical despite different names*

### Comparing `xklb-2.2.2/xklb/scripts/mining/nouns.py` & `xklb-2.2.3/xklb/scripts/mining/nouns.py`

 * *Files identical despite different names*

### Comparing `xklb-2.2.2/xklb/scripts/mining/pushshift.py` & `xklb-2.2.3/xklb/scripts/mining/pushshift.py`

 * *Files identical despite different names*

### Comparing `xklb-2.2.2/xklb/scripts/mining/reddit_selftext.py` & `xklb-2.2.3/xklb/scripts/mining/reddit_selftext.py`

 * *Files identical despite different names*

### Comparing `xklb-2.2.2/xklb/assets/kotobago.png` & `xklb-2.2.3/xklb/assets/kotobago.png`

 * *Files identical despite different names*

### Comparing `xklb-2.2.2/.gitignore` & `xklb-2.2.3/.gitignore`

 * *Files identical despite different names*

### Comparing `xklb-2.2.2/LICENSE` & `xklb-2.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `xklb-2.2.2/README.md` & `xklb-2.2.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -139,15 +139,15 @@
 Incremental surfing. 📈🏄 totally rad!
 
 </details>
 
 <details><summary>List all subcommands</summary>
 
     $ library
-    xk media library subcommands (v2.2.002)
+    xk media library subcommands (v2.2.003)
 
     local media:
       lb fsadd                 Create a local media database; Add folders
       lb fsupdate              Refresh database: add new files, mark deleted
 
       lb listen                Listen to local and online media
       lb watch                 Watch local and online media
```

### Comparing `xklb-2.2.2/pyproject.toml` & `xklb-2.2.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `xklb-2.2.2/PKG-INFO` & `xklb-2.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xklb
-Version: 2.2.2
+Version: 2.2.3
 Summary: xk library
 Project-URL: documentation, https://github.com/chapmanjacobd/library#usage
 Project-URL: homepage, https://github.com/chapmanjacobd/library#readme
 Project-URL: repository, https://github.com/chapmanjacobd/library/
 Author-email: Jacob Chapman <7908073+chapmanjacobd@users.noreply.github.com>
 License: BSD 3-Clause No Nuclear License
         
@@ -224,15 +224,15 @@
 Incremental surfing. 📈🏄 totally rad!
 
 </details>
 
 <details><summary>List all subcommands</summary>
 
     $ library
-    xk media library subcommands (v2.2.002)
+    xk media library subcommands (v2.2.003)
 
     local media:
       lb fsadd                 Create a local media database; Add folders
       lb fsupdate              Refresh database: add new files, mark deleted
 
       lb listen                Listen to local and online media
       lb watch                 Watch local and online media
```

