# Comparing `tmp/xklb-2.2.3.tar.gz` & `tmp/xklb-2.2.4.tar.gz`

## Comparing `xklb-2.2.3.tar` & `xklb-2.2.4.tar`

### file list

```diff
@@ -1,72 +1,72 @@
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 xklb-2.2.3/.gitattributes
--rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 xklb-2.2.3/TODO
--rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 xklb-2.2.3/Windows.md
--rw-r--r--   0        0        0   529514 2020-02-02 00:00:00.000000 xklb-2.2.3/pdm.lock
--rw-r--r--   0        0        0    13927 2020-02-02 00:00:00.000000 xklb-2.2.3/readme.py
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 xklb-2.2.3/.github/FUNDING.yml
--rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 xklb-2.2.3/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 xklb-2.2.3/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 xklb-2.2.3/.github/workflows/green.yaml
--rw-r--r--   0        0        0     1597 2020-02-02 00:00:00.000000 xklb-2.2.3/.github/workflows/push.yaml
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 xklb-2.2.3/xklb/__init__.py
--rw-r--r--   0        0        0     8679 2020-02-02 00:00:00.000000 xklb-2.2.3/xklb/av.py
--rw-r--r--   0        0        0     6921 2020-02-02 00:00:00.000000 xklb-2.2.3/xklb/books.py
--rw-r--r--   0        0        0     9417 2020-02-02 00:00:00.000000 xklb-2.2.3/xklb/consts.py
--rw-r--r--   0        0        0     8460 2020-02-02 00:00:00.000000 xklb-2.2.3/xklb/db.py
--rw-r--r--   0        0        0     7095 2020-02-02 00:00:00.000000 xklb-2.2.3/xklb/dl_config.py
--rw-r--r--   0        0        0    11059 2020-02-02 00:00:00.000000 xklb-2.2.3/xklb/dl_extract.py
--rw-r--r--   0        0        0    13784 2020-02-02 00:00:00.000000 xklb-2.2.3/xklb/fs_extract.py
--rw-r--r--   0        0        0     7481 2020-02-02 00:00:00.000000 xklb-2.2.3/xklb/gdl_backend.py
--rw-r--r--   0        0        0     3987 2020-02-02 00:00:00.000000 xklb-2.2.3/xklb/gdl_extract.py
--rw-r--r--   0        0        0     6212 2020-02-02 00:00:00.000000 xklb-2.2.3/xklb/gui.py
--rw-r--r--   0        0        0      808 2020-02-02 00:00:00.000000 xklb-2.2.3/xklb/history.py
--rw-r--r--   0        0        0     5712 2020-02-02 00:00:00.000000 xklb-2.2.3/xklb/hn_extract.py
--rw-r--r--   0        0        0    12585 2020-02-02 00:00:00.000000 xklb-2.2.3/xklb/lb.py
--rw-r--r--   0        0        0     7599 2020-02-02 00:00:00.000000 xklb-2.2.3/xklb/media.py
--rw-r--r--   0        0        0    26986 2020-02-02 00:00:00.000000 xklb-2.2.3/xklb/play_actions.py
--rw-r--r--   0        0        0    36936 2020-02-02 00:00:00.000000 xklb-2.2.3/xklb/player.py
--rw-r--r--   0        0        0     5232 2020-02-02 00:00:00.000000 xklb-2.2.3/xklb/playlists.py
--rw-r--r--   0        0        0    13481 2020-02-02 00:00:00.000000 xklb-2.2.3/xklb/praw_extract.py
--rw-r--r--   0        0        0     7997 2020-02-02 00:00:00.000000 xklb-2.2.3/xklb/search.py
--rw-r--r--   0        0        0     4639 2020-02-02 00:00:00.000000 xklb-2.2.3/xklb/subtitle.py
--rw-r--r--   0        0        0     6511 2020-02-02 00:00:00.000000 xklb-2.2.3/xklb/tabs_actions.py
--rw-r--r--   0        0        0     2789 2020-02-02 00:00:00.000000 xklb-2.2.3/xklb/tabs_extract.py
--rw-r--r--   0        0        0    15676 2020-02-02 00:00:00.000000 xklb-2.2.3/xklb/tube_backend.py
--rw-r--r--   0        0        0     4954 2020-02-02 00:00:00.000000 xklb-2.2.3/xklb/tube_extract.py
--rw-r--r--   0        0        0    85450 2020-02-02 00:00:00.000000 xklb-2.2.3/xklb/usage.py
--rw-r--r--   0        0        0    41694 2020-02-02 00:00:00.000000 xklb-2.2.3/xklb/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.2.3/xklb/scripts/__init__.py
--rw-r--r--   0        0        0     6087 2020-02-02 00:00:00.000000 xklb-2.2.3/xklb/scripts/bigdirs.py
--rw-r--r--   0        0        0     7257 2020-02-02 00:00:00.000000 xklb-2.2.3/xklb/scripts/block.py
--rw-r--r--   0        0        0     2437 2020-02-02 00:00:00.000000 xklb-2.2.3/xklb/scripts/christen.py
--rw-r--r--   0        0        0     3975 2020-02-02 00:00:00.000000 xklb-2.2.3/xklb/scripts/cluster_sort.py
--rw-r--r--   0        0        0     3215 2020-02-02 00:00:00.000000 xklb-2.2.3/xklb/scripts/copy_play_counts.py
--rw-r--r--   0        0        0     8198 2020-02-02 00:00:00.000000 xklb-2.2.3/xklb/scripts/dedupe.py
--rw-r--r--   0        0        0     4077 2020-02-02 00:00:00.000000 xklb-2.2.3/xklb/scripts/dedupe_db.py
--rw-r--r--   0        0        0     6891 2020-02-02 00:00:00.000000 xklb-2.2.3/xklb/scripts/disk_usage.py
--rw-r--r--   0        0        0     5454 2020-02-02 00:00:00.000000 xklb-2.2.3/xklb/scripts/download_status.py
--rw-r--r--   0        0        0     6411 2020-02-02 00:00:00.000000 xklb-2.2.3/xklb/scripts/history.py
--rw-r--r--   0        0        0     2686 2020-02-02 00:00:00.000000 xklb-2.2.3/xklb/scripts/merge_dbs.py
--rw-r--r--   0        0        0     3807 2020-02-02 00:00:00.000000 xklb-2.2.3/xklb/scripts/merge_online_local.py
--rw-r--r--   0        0        0     7066 2020-02-02 00:00:00.000000 xklb-2.2.3/xklb/scripts/move_list.py
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 xklb-2.2.3/xklb/scripts/optimize_db.py
--rw-r--r--   0        0        0     1945 2020-02-02 00:00:00.000000 xklb-2.2.3/xklb/scripts/places_import.py
--rw-r--r--   0        0        0     4560 2020-02-02 00:00:00.000000 xklb-2.2.3/xklb/scripts/playback_control.py
--rw-r--r--   0        0        0     5668 2020-02-02 00:00:00.000000 xklb-2.2.3/xklb/scripts/playlists.py
--rw-r--r--   0        0        0     6003 2020-02-02 00:00:00.000000 xklb-2.2.3/xklb/scripts/redownload.py
--rw-r--r--   0        0        0     2224 2020-02-02 00:00:00.000000 xklb-2.2.3/xklb/scripts/relmv.py
--rw-r--r--   0        0        0    10044 2020-02-02 00:00:00.000000 xklb-2.2.3/xklb/scripts/scatter.py
--rw-r--r--   0        0        0     2340 2020-02-02 00:00:00.000000 xklb-2.2.3/xklb/scripts/streaming_tab_loader.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.2.3/xklb/scripts/mining/__init__.py
--rw-r--r--   0        0        0    17101 2020-02-02 00:00:00.000000 xklb-2.2.3/xklb/scripts/mining/data.py
--rw-r--r--   0        0        0     3024 2020-02-02 00:00:00.000000 xklb-2.2.3/xklb/scripts/mining/extract_links.py
--rw-r--r--   0        0        0     1812 2020-02-02 00:00:00.000000 xklb-2.2.3/xklb/scripts/mining/mpv_watchlater.py
--rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 xklb-2.2.3/xklb/scripts/mining/nouns.py
--rw-r--r--   0        0        0     2159 2020-02-02 00:00:00.000000 xklb-2.2.3/xklb/scripts/mining/pushshift.py
--rw-r--r--   0        0        0     2163 2020-02-02 00:00:00.000000 xklb-2.2.3/xklb/scripts/mining/reddit_selftext.py
--rw-r--r--   0        0        0     8385 2020-02-02 00:00:00.000000 xklb-2.2.3/xklb/assets/kotobago.png
--rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 xklb-2.2.3/.gitignore
--rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 xklb-2.2.3/LICENSE
--rw-r--r--   0        0        0    97135 2020-02-02 00:00:00.000000 xklb-2.2.3/README.md
--rw-r--r--   0        0        0     2749 2020-02-02 00:00:00.000000 xklb-2.2.3/pyproject.toml
--rw-r--r--   0        0        0   100770 2020-02-02 00:00:00.000000 xklb-2.2.3/PKG-INFO
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 xklb-2.2.4/.gitattributes
+-rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 xklb-2.2.4/TODO
+-rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 xklb-2.2.4/Windows.md
+-rw-r--r--   0        0        0   529514 2020-02-02 00:00:00.000000 xklb-2.2.4/pdm.lock
+-rw-r--r--   0        0        0    13927 2020-02-02 00:00:00.000000 xklb-2.2.4/readme.py
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 xklb-2.2.4/.github/FUNDING.yml
+-rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 xklb-2.2.4/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 xklb-2.2.4/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 xklb-2.2.4/.github/workflows/green.yaml
+-rw-r--r--   0        0        0     1597 2020-02-02 00:00:00.000000 xklb-2.2.4/.github/workflows/push.yaml
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 xklb-2.2.4/xklb/__init__.py
+-rw-r--r--   0        0        0     8679 2020-02-02 00:00:00.000000 xklb-2.2.4/xklb/av.py
+-rw-r--r--   0        0        0     6921 2020-02-02 00:00:00.000000 xklb-2.2.4/xklb/books.py
+-rw-r--r--   0        0        0     9417 2020-02-02 00:00:00.000000 xklb-2.2.4/xklb/consts.py
+-rw-r--r--   0        0        0     8460 2020-02-02 00:00:00.000000 xklb-2.2.4/xklb/db.py
+-rw-r--r--   0        0        0     7095 2020-02-02 00:00:00.000000 xklb-2.2.4/xklb/dl_config.py
+-rw-r--r--   0        0        0    11059 2020-02-02 00:00:00.000000 xklb-2.2.4/xklb/dl_extract.py
+-rw-r--r--   0        0        0    13784 2020-02-02 00:00:00.000000 xklb-2.2.4/xklb/fs_extract.py
+-rw-r--r--   0        0        0     7481 2020-02-02 00:00:00.000000 xklb-2.2.4/xklb/gdl_backend.py
+-rw-r--r--   0        0        0     3987 2020-02-02 00:00:00.000000 xklb-2.2.4/xklb/gdl_extract.py
+-rw-r--r--   0        0        0     6212 2020-02-02 00:00:00.000000 xklb-2.2.4/xklb/gui.py
+-rw-r--r--   0        0        0      808 2020-02-02 00:00:00.000000 xklb-2.2.4/xklb/history.py
+-rw-r--r--   0        0        0     5712 2020-02-02 00:00:00.000000 xklb-2.2.4/xklb/hn_extract.py
+-rw-r--r--   0        0        0    12585 2020-02-02 00:00:00.000000 xklb-2.2.4/xklb/lb.py
+-rw-r--r--   0        0        0     7599 2020-02-02 00:00:00.000000 xklb-2.2.4/xklb/media.py
+-rw-r--r--   0        0        0    26986 2020-02-02 00:00:00.000000 xklb-2.2.4/xklb/play_actions.py
+-rw-r--r--   0        0        0    36936 2020-02-02 00:00:00.000000 xklb-2.2.4/xklb/player.py
+-rw-r--r--   0        0        0     5232 2020-02-02 00:00:00.000000 xklb-2.2.4/xklb/playlists.py
+-rw-r--r--   0        0        0    13481 2020-02-02 00:00:00.000000 xklb-2.2.4/xklb/praw_extract.py
+-rw-r--r--   0        0        0     7997 2020-02-02 00:00:00.000000 xklb-2.2.4/xklb/search.py
+-rw-r--r--   0        0        0     4639 2020-02-02 00:00:00.000000 xklb-2.2.4/xklb/subtitle.py
+-rw-r--r--   0        0        0     6511 2020-02-02 00:00:00.000000 xklb-2.2.4/xklb/tabs_actions.py
+-rw-r--r--   0        0        0     2789 2020-02-02 00:00:00.000000 xklb-2.2.4/xklb/tabs_extract.py
+-rw-r--r--   0        0        0    15676 2020-02-02 00:00:00.000000 xklb-2.2.4/xklb/tube_backend.py
+-rw-r--r--   0        0        0     4954 2020-02-02 00:00:00.000000 xklb-2.2.4/xklb/tube_extract.py
+-rw-r--r--   0        0        0    85452 2020-02-02 00:00:00.000000 xklb-2.2.4/xklb/usage.py
+-rw-r--r--   0        0        0    41680 2020-02-02 00:00:00.000000 xklb-2.2.4/xklb/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.2.4/xklb/scripts/__init__.py
+-rw-r--r--   0        0        0     6087 2020-02-02 00:00:00.000000 xklb-2.2.4/xklb/scripts/bigdirs.py
+-rw-r--r--   0        0        0     7257 2020-02-02 00:00:00.000000 xklb-2.2.4/xklb/scripts/block.py
+-rw-r--r--   0        0        0     2437 2020-02-02 00:00:00.000000 xklb-2.2.4/xklb/scripts/christen.py
+-rw-r--r--   0        0        0     3975 2020-02-02 00:00:00.000000 xklb-2.2.4/xklb/scripts/cluster_sort.py
+-rw-r--r--   0        0        0     3215 2020-02-02 00:00:00.000000 xklb-2.2.4/xklb/scripts/copy_play_counts.py
+-rw-r--r--   0        0        0     8198 2020-02-02 00:00:00.000000 xklb-2.2.4/xklb/scripts/dedupe.py
+-rw-r--r--   0        0        0     4077 2020-02-02 00:00:00.000000 xklb-2.2.4/xklb/scripts/dedupe_db.py
+-rw-r--r--   0        0        0     6891 2020-02-02 00:00:00.000000 xklb-2.2.4/xklb/scripts/disk_usage.py
+-rw-r--r--   0        0        0     5483 2020-02-02 00:00:00.000000 xklb-2.2.4/xklb/scripts/download_status.py
+-rw-r--r--   0        0        0     6411 2020-02-02 00:00:00.000000 xklb-2.2.4/xklb/scripts/history.py
+-rw-r--r--   0        0        0     2686 2020-02-02 00:00:00.000000 xklb-2.2.4/xklb/scripts/merge_dbs.py
+-rw-r--r--   0        0        0     3807 2020-02-02 00:00:00.000000 xklb-2.2.4/xklb/scripts/merge_online_local.py
+-rw-r--r--   0        0        0     7066 2020-02-02 00:00:00.000000 xklb-2.2.4/xklb/scripts/move_list.py
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 xklb-2.2.4/xklb/scripts/optimize_db.py
+-rw-r--r--   0        0        0     1945 2020-02-02 00:00:00.000000 xklb-2.2.4/xklb/scripts/places_import.py
+-rw-r--r--   0        0        0     4560 2020-02-02 00:00:00.000000 xklb-2.2.4/xklb/scripts/playback_control.py
+-rw-r--r--   0        0        0     5668 2020-02-02 00:00:00.000000 xklb-2.2.4/xklb/scripts/playlists.py
+-rw-r--r--   0        0        0     6003 2020-02-02 00:00:00.000000 xklb-2.2.4/xklb/scripts/redownload.py
+-rw-r--r--   0        0        0     2224 2020-02-02 00:00:00.000000 xklb-2.2.4/xklb/scripts/relmv.py
+-rw-r--r--   0        0        0    10044 2020-02-02 00:00:00.000000 xklb-2.2.4/xklb/scripts/scatter.py
+-rw-r--r--   0        0        0     2340 2020-02-02 00:00:00.000000 xklb-2.2.4/xklb/scripts/streaming_tab_loader.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.2.4/xklb/scripts/mining/__init__.py
+-rw-r--r--   0        0        0    17101 2020-02-02 00:00:00.000000 xklb-2.2.4/xklb/scripts/mining/data.py
+-rw-r--r--   0        0        0     3024 2020-02-02 00:00:00.000000 xklb-2.2.4/xklb/scripts/mining/extract_links.py
+-rw-r--r--   0        0        0     1812 2020-02-02 00:00:00.000000 xklb-2.2.4/xklb/scripts/mining/mpv_watchlater.py
+-rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 xklb-2.2.4/xklb/scripts/mining/nouns.py
+-rw-r--r--   0        0        0     2159 2020-02-02 00:00:00.000000 xklb-2.2.4/xklb/scripts/mining/pushshift.py
+-rw-r--r--   0        0        0     2163 2020-02-02 00:00:00.000000 xklb-2.2.4/xklb/scripts/mining/reddit_selftext.py
+-rw-r--r--   0        0        0     8385 2020-02-02 00:00:00.000000 xklb-2.2.4/xklb/assets/kotobago.png
+-rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 xklb-2.2.4/.gitignore
+-rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 xklb-2.2.4/LICENSE
+-rw-r--r--   0        0        0    97135 2020-02-02 00:00:00.000000 xklb-2.2.4/README.md
+-rw-r--r--   0        0        0     2749 2020-02-02 00:00:00.000000 xklb-2.2.4/pyproject.toml
+-rw-r--r--   0        0        0   100770 2020-02-02 00:00:00.000000 xklb-2.2.4/PKG-INFO
```

### Comparing `xklb-2.2.3/TODO` & `xklb-2.2.4/TODO`

 * *Files identical despite different names*

### Comparing `xklb-2.2.3/Windows.md` & `xklb-2.2.4/Windows.md`

 * *Files identical despite different names*

### Comparing `xklb-2.2.3/pdm.lock` & `xklb-2.2.4/pdm.lock`

 * *Files identical despite different names*

### Comparing `xklb-2.2.3/readme.py` & `xklb-2.2.4/readme.py`

 * *Files identical despite different names*

### Comparing `xklb-2.2.3/.github/ISSUE_TEMPLATE/bug_report.md` & `xklb-2.2.4/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `xklb-2.2.3/.github/ISSUE_TEMPLATE/feature_request.md` & `xklb-2.2.4/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `xklb-2.2.3/.github/workflows/push.yaml` & `xklb-2.2.4/.github/workflows/push.yaml`

 * *Files identical despite different names*

### Comparing `xklb-2.2.3/xklb/av.py` & `xklb-2.2.4/xklb/av.py`

 * *Files identical despite different names*

### Comparing `xklb-2.2.3/xklb/books.py` & `xklb-2.2.4/xklb/books.py`

 * *Files identical despite different names*

### Comparing `xklb-2.2.3/xklb/consts.py` & `xklb-2.2.4/xklb/consts.py`

 * *Files identical despite different names*

### Comparing `xklb-2.2.3/xklb/db.py` & `xklb-2.2.4/xklb/db.py`

 * *Files identical despite different names*

### Comparing `xklb-2.2.3/xklb/dl_config.py` & `xklb-2.2.4/xklb/dl_config.py`

 * *Files identical despite different names*

### Comparing `xklb-2.2.3/xklb/dl_extract.py` & `xklb-2.2.4/xklb/dl_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-2.2.3/xklb/fs_extract.py` & `xklb-2.2.4/xklb/fs_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-2.2.3/xklb/gdl_backend.py` & `xklb-2.2.4/xklb/gdl_backend.py`

 * *Files identical despite different names*

### Comparing `xklb-2.2.3/xklb/gdl_extract.py` & `xklb-2.2.4/xklb/gdl_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-2.2.3/xklb/gui.py` & `xklb-2.2.4/xklb/gui.py`

 * *Files identical despite different names*

### Comparing `xklb-2.2.3/xklb/history.py` & `xklb-2.2.4/xklb/history.py`

 * *Files identical despite different names*

### Comparing `xklb-2.2.3/xklb/hn_extract.py` & `xklb-2.2.4/xklb/hn_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-2.2.3/xklb/lb.py` & `xklb-2.2.4/xklb/lb.py`

 * *Files identical despite different names*

### Comparing `xklb-2.2.3/xklb/media.py` & `xklb-2.2.4/xklb/media.py`

 * *Files identical despite different names*

### Comparing `xklb-2.2.3/xklb/play_actions.py` & `xklb-2.2.4/xklb/play_actions.py`

 * *Files identical despite different names*

### Comparing `xklb-2.2.3/xklb/player.py` & `xklb-2.2.4/xklb/player.py`

 * *Files identical despite different names*

### Comparing `xklb-2.2.3/xklb/playlists.py` & `xklb-2.2.4/xklb/playlists.py`

 * *Files identical despite different names*

### Comparing `xklb-2.2.3/xklb/praw_extract.py` & `xklb-2.2.4/xklb/praw_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-2.2.3/xklb/search.py` & `xklb-2.2.4/xklb/search.py`

 * *Files identical despite different names*

### Comparing `xklb-2.2.3/xklb/subtitle.py` & `xklb-2.2.4/xklb/subtitle.py`

 * *Files identical despite different names*

### Comparing `xklb-2.2.3/xklb/tabs_actions.py` & `xklb-2.2.4/xklb/tabs_actions.py`

 * *Files identical despite different names*

### Comparing `xklb-2.2.3/xklb/tabs_extract.py` & `xklb-2.2.4/xklb/tabs_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-2.2.3/xklb/tube_backend.py` & `xklb-2.2.4/xklb/tube_backend.py`

 * *Files identical despite different names*

### Comparing `xklb-2.2.3/xklb/tube_extract.py` & `xklb-2.2.4/xklb/tube_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-2.2.3/xklb/usage.py` & `xklb-2.2.4/xklb/usage.py`

 * *Files 0% similar despite different names*

```diff
@@ -754,15 +754,15 @@
 
 galleryadd = """library galleryadd DATABASE URLS
 
 Add gallery_dl URLs to download later or periodically update
 
 If you have many URLs use stdin
 
-    cat ./my-favorite-manhwa.txt | library galleryadd my.db --insert-only
+    cat ./my-favorite-manhwa.txt | library galleryadd my.db --insert-only -
 """
 
 galleryupdate = """library galleryupdate DATABASE URLS
 
 Check previously saved gallery_dl URLs for new content
 """
```

### Comparing `xklb-2.2.3/xklb/utils.py` & `xklb-2.2.4/xklb/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -775,15 +775,15 @@
             msg = f'Could not parse argument "{values}" as k1=1 k2=2 format {ex}'
             raise argparse.ArgumentError(self, msg) from ex
         setattr(args, self.dest, d)
 
 
 class ArgparseArgsOrStdin(argparse.Action):
     def __call__(self, parser, namespace, values, option_string=None):
-        if values == ["-"] or not values:
+        if values == ["-"]:
             lines = sys.stdin.readlines()
         else:
             lines = values
         setattr(namespace, self.dest, lines)
 
 
 def filter_namespace(args, config_opts) -> Optional[Dict]:
```

### Comparing `xklb-2.2.3/xklb/scripts/bigdirs.py` & `xklb-2.2.4/xklb/scripts/bigdirs.py`

 * *Files identical despite different names*

### Comparing `xklb-2.2.3/xklb/scripts/block.py` & `xklb-2.2.4/xklb/scripts/block.py`

 * *Files identical despite different names*

### Comparing `xklb-2.2.3/xklb/scripts/christen.py` & `xklb-2.2.4/xklb/scripts/christen.py`

 * *Files identical despite different names*

### Comparing `xklb-2.2.3/xklb/scripts/cluster_sort.py` & `xklb-2.2.4/xklb/scripts/cluster_sort.py`

 * *Files identical despite different names*

### Comparing `xklb-2.2.3/xklb/scripts/copy_play_counts.py` & `xklb-2.2.4/xklb/scripts/copy_play_counts.py`

 * *Files identical despite different names*

### Comparing `xklb-2.2.3/xklb/scripts/dedupe.py` & `xklb-2.2.4/xklb/scripts/dedupe.py`

 * *Files identical despite different names*

### Comparing `xklb-2.2.3/xklb/scripts/dedupe_db.py` & `xklb-2.2.4/xklb/scripts/dedupe_db.py`

 * *Files identical despite different names*

### Comparing `xklb-2.2.3/xklb/scripts/disk_usage.py` & `xklb-2.2.4/xklb/scripts/disk_usage.py`

 * *Files identical despite different names*

### Comparing `xklb-2.2.3/xklb/scripts/download_status.py` & `xklb-2.2.4/xklb/scripts/download_status.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,14 +33,15 @@
     )
 
     parser.add_argument("-v", "--verbose", action="count", default=0)
     parser.add_argument("--db", "-db", help=argparse.SUPPRESS)
 
     parser.add_argument("database")
     args = parser.parse_args()
+
     if args.db:
         args.database = args.db
     args.db = db.connect(args)
     log.info(utils.dict_filter_bool(args.__dict__))
 
     args.action = consts.SC.stats
     return args
@@ -113,27 +114,27 @@
         and COALESCE(time_deleted,0) = 0
     group by extractor_key
     order by never_downloaded DESC"""
 
     printer(args, query, bindings)
 
     if "error" in db.columns(args, "media"):
-        query = """
+        query = f"""
         select error, count(*) count
         from media
         where error is not null
         group by 1
-        order by 2
+        order by 2 DESC
         """
         errors = list(args.db.query(query))
 
         common_errors = []
         other_errors = []
         for error in errors:
-            if error["count"] < 5:
+            if error["count"] < errors[:5][-1]["count"]:
                 other_errors.append(error)
             else:
                 common_errors.append(error)
 
         common_errors.append({"error": "Other", "count": len(other_errors)})
         common_errors.append({"error": "Total", "count": sum(d["count"] for d in errors)})
         print(tabulate(common_errors, tablefmt=consts.TABULATE_STYLE, headers="keys", showindex=False))
```

### Comparing `xklb-2.2.3/xklb/scripts/history.py` & `xklb-2.2.4/xklb/scripts/history.py`

 * *Files identical despite different names*

### Comparing `xklb-2.2.3/xklb/scripts/merge_dbs.py` & `xklb-2.2.4/xklb/scripts/merge_dbs.py`

 * *Files identical despite different names*

### Comparing `xklb-2.2.3/xklb/scripts/merge_online_local.py` & `xklb-2.2.4/xklb/scripts/merge_online_local.py`

 * *Files identical despite different names*

### Comparing `xklb-2.2.3/xklb/scripts/move_list.py` & `xklb-2.2.4/xklb/scripts/move_list.py`

 * *Files identical despite different names*

### Comparing `xklb-2.2.3/xklb/scripts/optimize_db.py` & `xklb-2.2.4/xklb/scripts/optimize_db.py`

 * *Files identical despite different names*

### Comparing `xklb-2.2.3/xklb/scripts/places_import.py` & `xklb-2.2.4/xklb/scripts/places_import.py`

 * *Files identical despite different names*

### Comparing `xklb-2.2.3/xklb/scripts/playback_control.py` & `xklb-2.2.4/xklb/scripts/playback_control.py`

 * *Files identical despite different names*

### Comparing `xklb-2.2.3/xklb/scripts/playlists.py` & `xklb-2.2.4/xklb/scripts/playlists.py`

 * *Files identical despite different names*

### Comparing `xklb-2.2.3/xklb/scripts/redownload.py` & `xklb-2.2.4/xklb/scripts/redownload.py`

 * *Files identical despite different names*

### Comparing `xklb-2.2.3/xklb/scripts/relmv.py` & `xklb-2.2.4/xklb/scripts/relmv.py`

 * *Files identical despite different names*

### Comparing `xklb-2.2.3/xklb/scripts/scatter.py` & `xklb-2.2.4/xklb/scripts/scatter.py`

 * *Files identical despite different names*

### Comparing `xklb-2.2.3/xklb/scripts/streaming_tab_loader.py` & `xklb-2.2.4/xklb/scripts/streaming_tab_loader.py`

 * *Files identical despite different names*

### Comparing `xklb-2.2.3/xklb/scripts/mining/data.py` & `xklb-2.2.4/xklb/scripts/mining/data.py`

 * *Files identical despite different names*

### Comparing `xklb-2.2.3/xklb/scripts/mining/extract_links.py` & `xklb-2.2.4/xklb/scripts/mining/extract_links.py`

 * *Files identical despite different names*

### Comparing `xklb-2.2.3/xklb/scripts/mining/mpv_watchlater.py` & `xklb-2.2.4/xklb/scripts/mining/mpv_watchlater.py`

 * *Files identical despite different names*

### Comparing `xklb-2.2.3/xklb/scripts/mining/nouns.py` & `xklb-2.2.4/xklb/scripts/mining/nouns.py`

 * *Files identical despite different names*

### Comparing `xklb-2.2.3/xklb/scripts/mining/pushshift.py` & `xklb-2.2.4/xklb/scripts/mining/pushshift.py`

 * *Files identical despite different names*

### Comparing `xklb-2.2.3/xklb/scripts/mining/reddit_selftext.py` & `xklb-2.2.4/xklb/scripts/mining/reddit_selftext.py`

 * *Files identical despite different names*

### Comparing `xklb-2.2.3/xklb/assets/kotobago.png` & `xklb-2.2.4/xklb/assets/kotobago.png`

 * *Files identical despite different names*

### Comparing `xklb-2.2.3/.gitignore` & `xklb-2.2.4/.gitignore`

 * *Files identical despite different names*

### Comparing `xklb-2.2.3/LICENSE` & `xklb-2.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `xklb-2.2.3/README.md` & `xklb-2.2.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -139,15 +139,15 @@
 Incremental surfing. 📈🏄 totally rad!
 
 </details>
 
 <details><summary>List all subcommands</summary>
 
     $ library
-    xk media library subcommands (v2.2.003)
+    xk media library subcommands (v2.2.004)
 
     local media:
       lb fsadd                 Create a local media database; Add folders
       lb fsupdate              Refresh database: add new files, mark deleted
 
       lb listen                Listen to local and online media
       lb watch                 Watch local and online media
```

### Comparing `xklb-2.2.3/pyproject.toml` & `xklb-2.2.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `xklb-2.2.3/PKG-INFO` & `xklb-2.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xklb
-Version: 2.2.3
+Version: 2.2.4
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
-    xk media library subcommands (v2.2.003)
+    xk media library subcommands (v2.2.004)
 
     local media:
       lb fsadd                 Create a local media database; Add folders
       lb fsupdate              Refresh database: add new files, mark deleted
 
       lb listen                Listen to local and online media
       lb watch                 Watch local and online media
```

