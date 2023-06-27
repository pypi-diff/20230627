# Comparing `tmp/xklb-2.1.9.tar.gz` & `tmp/xklb-2.2.2.tar.gz`

## Comparing `xklb-2.1.9.tar` & `xklb-2.2.2.tar`

### file list

```diff
@@ -1,70 +1,72 @@
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 xklb-2.1.9/.gitattributes
--rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 xklb-2.1.9/TODO
--rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 xklb-2.1.9/Windows.md
--rw-r--r--   0        0        0   490400 2020-02-02 00:00:00.000000 xklb-2.1.9/pdm.lock
--rw-r--r--   0        0        0    13120 2020-02-02 00:00:00.000000 xklb-2.1.9/readme.py
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 xklb-2.1.9/.github/FUNDING.yml
--rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 xklb-2.1.9/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 xklb-2.1.9/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 xklb-2.1.9/.github/workflows/green.yaml
--rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 xklb-2.1.9/.github/workflows/push.yaml
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 xklb-2.1.9/xklb/__init__.py
--rw-r--r--   0        0        0     8679 2020-02-02 00:00:00.000000 xklb-2.1.9/xklb/av.py
--rw-r--r--   0        0        0     6921 2020-02-02 00:00:00.000000 xklb-2.1.9/xklb/books.py
--rw-r--r--   0        0        0     9402 2020-02-02 00:00:00.000000 xklb-2.1.9/xklb/consts.py
--rw-r--r--   0        0        0     8342 2020-02-02 00:00:00.000000 xklb-2.1.9/xklb/db.py
--rw-r--r--   0        0        0     7095 2020-02-02 00:00:00.000000 xklb-2.1.9/xklb/dl_config.py
--rw-r--r--   0        0        0    11943 2020-02-02 00:00:00.000000 xklb-2.1.9/xklb/dl_extract.py
--rw-r--r--   0        0        0    13784 2020-02-02 00:00:00.000000 xklb-2.1.9/xklb/fs_extract.py
--rw-r--r--   0        0        0     7481 2020-02-02 00:00:00.000000 xklb-2.1.9/xklb/gdl_backend.py
--rw-r--r--   0        0        0     3809 2020-02-02 00:00:00.000000 xklb-2.1.9/xklb/gdl_extract.py
--rw-r--r--   0        0        0     6212 2020-02-02 00:00:00.000000 xklb-2.1.9/xklb/gui.py
--rw-r--r--   0        0        0      808 2020-02-02 00:00:00.000000 xklb-2.1.9/xklb/history.py
--rw-r--r--   0        0        0     5712 2020-02-02 00:00:00.000000 xklb-2.1.9/xklb/hn_extract.py
--rw-r--r--   0        0        0    12072 2020-02-02 00:00:00.000000 xklb-2.1.9/xklb/lb.py
--rw-r--r--   0        0        0     7597 2020-02-02 00:00:00.000000 xklb-2.1.9/xklb/media.py
--rw-r--r--   0        0        0    25566 2020-02-02 00:00:00.000000 xklb-2.1.9/xklb/play_actions.py
--rw-r--r--   0        0        0    36352 2020-02-02 00:00:00.000000 xklb-2.1.9/xklb/player.py
--rw-r--r--   0        0        0     5232 2020-02-02 00:00:00.000000 xklb-2.1.9/xklb/playlists.py
--rw-r--r--   0        0        0    13549 2020-02-02 00:00:00.000000 xklb-2.1.9/xklb/praw_extract.py
--rw-r--r--   0        0        0     7988 2020-02-02 00:00:00.000000 xklb-2.1.9/xklb/search.py
--rw-r--r--   0        0        0     4639 2020-02-02 00:00:00.000000 xklb-2.1.9/xklb/subtitle.py
--rw-r--r--   0        0        0     6511 2020-02-02 00:00:00.000000 xklb-2.1.9/xklb/tabs_actions.py
--rw-r--r--   0        0        0     2789 2020-02-02 00:00:00.000000 xklb-2.1.9/xklb/tabs_extract.py
--rw-r--r--   0        0        0    15676 2020-02-02 00:00:00.000000 xklb-2.1.9/xklb/tube_backend.py
--rw-r--r--   0        0        0     4725 2020-02-02 00:00:00.000000 xklb-2.1.9/xklb/tube_extract.py
--rw-r--r--   0        0        0    83354 2020-02-02 00:00:00.000000 xklb-2.1.9/xklb/usage.py
--rw-r--r--   0        0        0    41329 2020-02-02 00:00:00.000000 xklb-2.1.9/xklb/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.1.9/xklb/scripts/__init__.py
--rw-r--r--   0        0        0     6051 2020-02-02 00:00:00.000000 xklb-2.1.9/xklb/scripts/bigdirs.py
--rw-r--r--   0        0        0     7248 2020-02-02 00:00:00.000000 xklb-2.1.9/xklb/scripts/block.py
--rw-r--r--   0        0        0     2437 2020-02-02 00:00:00.000000 xklb-2.1.9/xklb/scripts/christen.py
--rw-r--r--   0        0        0     3975 2020-02-02 00:00:00.000000 xklb-2.1.9/xklb/scripts/cluster_sort.py
--rw-r--r--   0        0        0     3074 2020-02-02 00:00:00.000000 xklb-2.1.9/xklb/scripts/copy_play_counts.py
--rw-r--r--   0        0        0     8181 2020-02-02 00:00:00.000000 xklb-2.1.9/xklb/scripts/dedupe.py
--rw-r--r--   0        0        0     4077 2020-02-02 00:00:00.000000 xklb-2.1.9/xklb/scripts/dedupe_db.py
--rw-r--r--   0        0        0     5397 2020-02-02 00:00:00.000000 xklb-2.1.9/xklb/scripts/download_status.py
--rw-r--r--   0        0        0     6474 2020-02-02 00:00:00.000000 xklb-2.1.9/xklb/scripts/history.py
--rw-r--r--   0        0        0     2686 2020-02-02 00:00:00.000000 xklb-2.1.9/xklb/scripts/merge_dbs.py
--rw-r--r--   0        0        0     3795 2020-02-02 00:00:00.000000 xklb-2.1.9/xklb/scripts/merge_online_local.py
--rw-r--r--   0        0        0     7049 2020-02-02 00:00:00.000000 xklb-2.1.9/xklb/scripts/move_list.py
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 xklb-2.1.9/xklb/scripts/optimize_db.py
--rw-r--r--   0        0        0     4560 2020-02-02 00:00:00.000000 xklb-2.1.9/xklb/scripts/playback_control.py
--rw-r--r--   0        0        0     5659 2020-02-02 00:00:00.000000 xklb-2.1.9/xklb/scripts/playlists.py
--rw-r--r--   0        0        0     5985 2020-02-02 00:00:00.000000 xklb-2.1.9/xklb/scripts/redownload.py
--rw-r--r--   0        0        0     2224 2020-02-02 00:00:00.000000 xklb-2.1.9/xklb/scripts/relmv.py
--rw-r--r--   0        0        0    10026 2020-02-02 00:00:00.000000 xklb-2.1.9/xklb/scripts/scatter.py
--rw-r--r--   0        0        0     2340 2020-02-02 00:00:00.000000 xklb-2.1.9/xklb/scripts/streaming_tab_loader.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.1.9/xklb/scripts/mining/__init__.py
--rw-r--r--   0        0        0    17101 2020-02-02 00:00:00.000000 xklb-2.1.9/xklb/scripts/mining/data.py
--rw-r--r--   0        0        0     3024 2020-02-02 00:00:00.000000 xklb-2.1.9/xklb/scripts/mining/extract_links.py
--rw-r--r--   0        0        0     1812 2020-02-02 00:00:00.000000 xklb-2.1.9/xklb/scripts/mining/mpv_watchlater.py
--rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 xklb-2.1.9/xklb/scripts/mining/nouns.py
--rw-r--r--   0        0        0     2159 2020-02-02 00:00:00.000000 xklb-2.1.9/xklb/scripts/mining/pushshift.py
--rw-r--r--   0        0        0     2163 2020-02-02 00:00:00.000000 xklb-2.1.9/xklb/scripts/mining/reddit_selftext.py
--rw-r--r--   0        0        0     8385 2020-02-02 00:00:00.000000 xklb-2.1.9/xklb/assets/kotobago.png
--rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 xklb-2.1.9/.gitignore
--rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 xklb-2.1.9/LICENSE
--rw-r--r--   0        0        0    94114 2020-02-02 00:00:00.000000 xklb-2.1.9/README.md
--rw-r--r--   0        0        0     2740 2020-02-02 00:00:00.000000 xklb-2.1.9/pyproject.toml
--rw-r--r--   0        0        0    97740 2020-02-02 00:00:00.000000 xklb-2.1.9/PKG-INFO
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 xklb-2.2.2/.gitattributes
+-rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 xklb-2.2.2/TODO
+-rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 xklb-2.2.2/Windows.md
+-rw-r--r--   0        0        0   529514 2020-02-02 00:00:00.000000 xklb-2.2.2/pdm.lock
+-rw-r--r--   0        0        0    13927 2020-02-02 00:00:00.000000 xklb-2.2.2/readme.py
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 xklb-2.2.2/.github/FUNDING.yml
+-rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 xklb-2.2.2/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 xklb-2.2.2/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 xklb-2.2.2/.github/workflows/green.yaml
+-rw-r--r--   0        0        0     1597 2020-02-02 00:00:00.000000 xklb-2.2.2/.github/workflows/push.yaml
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 xklb-2.2.2/xklb/__init__.py
+-rw-r--r--   0        0        0     8679 2020-02-02 00:00:00.000000 xklb-2.2.2/xklb/av.py
+-rw-r--r--   0        0        0     6921 2020-02-02 00:00:00.000000 xklb-2.2.2/xklb/books.py
+-rw-r--r--   0        0        0     9417 2020-02-02 00:00:00.000000 xklb-2.2.2/xklb/consts.py
+-rw-r--r--   0        0        0     8460 2020-02-02 00:00:00.000000 xklb-2.2.2/xklb/db.py
+-rw-r--r--   0        0        0     7095 2020-02-02 00:00:00.000000 xklb-2.2.2/xklb/dl_config.py
+-rw-r--r--   0        0        0    11051 2020-02-02 00:00:00.000000 xklb-2.2.2/xklb/dl_extract.py
+-rw-r--r--   0        0        0    13784 2020-02-02 00:00:00.000000 xklb-2.2.2/xklb/fs_extract.py
+-rw-r--r--   0        0        0     7481 2020-02-02 00:00:00.000000 xklb-2.2.2/xklb/gdl_backend.py
+-rw-r--r--   0        0        0     4041 2020-02-02 00:00:00.000000 xklb-2.2.2/xklb/gdl_extract.py
+-rw-r--r--   0        0        0     6212 2020-02-02 00:00:00.000000 xklb-2.2.2/xklb/gui.py
+-rw-r--r--   0        0        0      808 2020-02-02 00:00:00.000000 xklb-2.2.2/xklb/history.py
+-rw-r--r--   0        0        0     5712 2020-02-02 00:00:00.000000 xklb-2.2.2/xklb/hn_extract.py
+-rw-r--r--   0        0        0    12585 2020-02-02 00:00:00.000000 xklb-2.2.2/xklb/lb.py
+-rw-r--r--   0        0        0     7599 2020-02-02 00:00:00.000000 xklb-2.2.2/xklb/media.py
+-rw-r--r--   0        0        0    26986 2020-02-02 00:00:00.000000 xklb-2.2.2/xklb/play_actions.py
+-rw-r--r--   0        0        0    36936 2020-02-02 00:00:00.000000 xklb-2.2.2/xklb/player.py
+-rw-r--r--   0        0        0     5232 2020-02-02 00:00:00.000000 xklb-2.2.2/xklb/playlists.py
+-rw-r--r--   0        0        0    13549 2020-02-02 00:00:00.000000 xklb-2.2.2/xklb/praw_extract.py
+-rw-r--r--   0        0        0     7997 2020-02-02 00:00:00.000000 xklb-2.2.2/xklb/search.py
+-rw-r--r--   0        0        0     4639 2020-02-02 00:00:00.000000 xklb-2.2.2/xklb/subtitle.py
+-rw-r--r--   0        0        0     6511 2020-02-02 00:00:00.000000 xklb-2.2.2/xklb/tabs_actions.py
+-rw-r--r--   0        0        0     2789 2020-02-02 00:00:00.000000 xklb-2.2.2/xklb/tabs_extract.py
+-rw-r--r--   0        0        0    15676 2020-02-02 00:00:00.000000 xklb-2.2.2/xklb/tube_backend.py
+-rw-r--r--   0        0        0     4944 2020-02-02 00:00:00.000000 xklb-2.2.2/xklb/tube_extract.py
+-rw-r--r--   0        0        0    85450 2020-02-02 00:00:00.000000 xklb-2.2.2/xklb/usage.py
+-rw-r--r--   0        0        0    41694 2020-02-02 00:00:00.000000 xklb-2.2.2/xklb/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.2.2/xklb/scripts/__init__.py
+-rw-r--r--   0        0        0     6087 2020-02-02 00:00:00.000000 xklb-2.2.2/xklb/scripts/bigdirs.py
+-rw-r--r--   0        0        0     7257 2020-02-02 00:00:00.000000 xklb-2.2.2/xklb/scripts/block.py
+-rw-r--r--   0        0        0     2437 2020-02-02 00:00:00.000000 xklb-2.2.2/xklb/scripts/christen.py
+-rw-r--r--   0        0        0     3975 2020-02-02 00:00:00.000000 xklb-2.2.2/xklb/scripts/cluster_sort.py
+-rw-r--r--   0        0        0     3215 2020-02-02 00:00:00.000000 xklb-2.2.2/xklb/scripts/copy_play_counts.py
+-rw-r--r--   0        0        0     8198 2020-02-02 00:00:00.000000 xklb-2.2.2/xklb/scripts/dedupe.py
+-rw-r--r--   0        0        0     4077 2020-02-02 00:00:00.000000 xklb-2.2.2/xklb/scripts/dedupe_db.py
+-rw-r--r--   0        0        0     6891 2020-02-02 00:00:00.000000 xklb-2.2.2/xklb/scripts/disk_usage.py
+-rw-r--r--   0        0        0     5415 2020-02-02 00:00:00.000000 xklb-2.2.2/xklb/scripts/download_status.py
+-rw-r--r--   0        0        0     6411 2020-02-02 00:00:00.000000 xklb-2.2.2/xklb/scripts/history.py
+-rw-r--r--   0        0        0     2686 2020-02-02 00:00:00.000000 xklb-2.2.2/xklb/scripts/merge_dbs.py
+-rw-r--r--   0        0        0     3807 2020-02-02 00:00:00.000000 xklb-2.2.2/xklb/scripts/merge_online_local.py
+-rw-r--r--   0        0        0     7066 2020-02-02 00:00:00.000000 xklb-2.2.2/xklb/scripts/move_list.py
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 xklb-2.2.2/xklb/scripts/optimize_db.py
+-rw-r--r--   0        0        0     1945 2020-02-02 00:00:00.000000 xklb-2.2.2/xklb/scripts/places_import.py
+-rw-r--r--   0        0        0     4560 2020-02-02 00:00:00.000000 xklb-2.2.2/xklb/scripts/playback_control.py
+-rw-r--r--   0        0        0     5668 2020-02-02 00:00:00.000000 xklb-2.2.2/xklb/scripts/playlists.py
+-rw-r--r--   0        0        0     6003 2020-02-02 00:00:00.000000 xklb-2.2.2/xklb/scripts/redownload.py
+-rw-r--r--   0        0        0     2224 2020-02-02 00:00:00.000000 xklb-2.2.2/xklb/scripts/relmv.py
+-rw-r--r--   0        0        0    10044 2020-02-02 00:00:00.000000 xklb-2.2.2/xklb/scripts/scatter.py
+-rw-r--r--   0        0        0     2340 2020-02-02 00:00:00.000000 xklb-2.2.2/xklb/scripts/streaming_tab_loader.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.2.2/xklb/scripts/mining/__init__.py
+-rw-r--r--   0        0        0    17101 2020-02-02 00:00:00.000000 xklb-2.2.2/xklb/scripts/mining/data.py
+-rw-r--r--   0        0        0     3024 2020-02-02 00:00:00.000000 xklb-2.2.2/xklb/scripts/mining/extract_links.py
+-rw-r--r--   0        0        0     1812 2020-02-02 00:00:00.000000 xklb-2.2.2/xklb/scripts/mining/mpv_watchlater.py
+-rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 xklb-2.2.2/xklb/scripts/mining/nouns.py
+-rw-r--r--   0        0        0     2159 2020-02-02 00:00:00.000000 xklb-2.2.2/xklb/scripts/mining/pushshift.py
+-rw-r--r--   0        0        0     2163 2020-02-02 00:00:00.000000 xklb-2.2.2/xklb/scripts/mining/reddit_selftext.py
+-rw-r--r--   0        0        0     8385 2020-02-02 00:00:00.000000 xklb-2.2.2/xklb/assets/kotobago.png
+-rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 xklb-2.2.2/.gitignore
+-rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 xklb-2.2.2/LICENSE
+-rw-r--r--   0        0        0    97135 2020-02-02 00:00:00.000000 xklb-2.2.2/README.md
+-rw-r--r--   0        0        0     2749 2020-02-02 00:00:00.000000 xklb-2.2.2/pyproject.toml
+-rw-r--r--   0        0        0   100770 2020-02-02 00:00:00.000000 xklb-2.2.2/PKG-INFO
```

### Comparing `xklb-2.1.9/Windows.md` & `xklb-2.2.2/Windows.md`

 * *Files identical despite different names*

### Comparing `xklb-2.1.9/pdm.lock` & `xklb-2.2.2/pdm.lock`

 * *Files 2% similar despite different names*

```diff
@@ -197,14 +197,31 @@
 version = "1.2.2"
 summary = "Extends click.Group to invoke a command without explicit subcommand name (packaged as a wheel)"
 dependencies = [
     "click",
 ]
 
 [[package]]
+name = "click-plugins"
+version = "1.1.1"
+summary = "An extension module for click to enable registering CLI commands via setuptools entry-points."
+dependencies = [
+    "click>=4.0",
+]
+
+[[package]]
+name = "cligj"
+version = "0.7.2"
+requires_python = ">=2.7, !=3.0.*, !=3.1.*, !=3.2.*, <4"
+summary = "Click params for commmand line interfaces to GeoJSON"
+dependencies = [
+    "click>=4.0",
+]
+
+[[package]]
 name = "cloudpickle"
 version = "2.2.1"
 requires_python = ">=3.6"
 summary = "Extended pickling support for Python objects"
 
 [[package]]
 name = "colorama"
@@ -297,14 +314,29 @@
 version = "0.2.0"
 summary = "Python bindings for FFmpeg - with complex filtering support"
 dependencies = [
     "future",
 ]
 
 [[package]]
+name = "fiona"
+version = "1.9.4.post1"
+requires_python = ">=3.7"
+summary = "Fiona reads and writes spatial data files"
+dependencies = [
+    "attrs>=19.2.0",
+    "certifi",
+    "click-plugins>=1.0",
+    "click~=8.0",
+    "cligj>=0.5",
+    "importlib-metadata; python_version < \"3.10\"",
+    "six",
+]
+
+[[package]]
 name = "flask"
 version = "2.0.2"
 requires_python = ">=3.6"
 summary = "A simple framework for building complex web applications."
 dependencies = [
     "Jinja2>=3.0",
     "Werkzeug>=2.0",
@@ -339,14 +371,27 @@
 requires_python = ">=3.4"
 summary = "Command-line program to download image galleries and collections from several image hosting sites"
 dependencies = [
     "requests>=2.11.0",
 ]
 
 [[package]]
+name = "geopandas"
+version = "0.13.2"
+requires_python = ">=3.8"
+summary = "Geographic pandas extensions"
+dependencies = [
+    "fiona>=1.8.19",
+    "packaging",
+    "pandas>=1.1.0",
+    "pyproj>=3.0.1",
+    "shapely>=1.7.1",
+]
+
+[[package]]
 name = "guessit"
 version = "3.7.1"
 summary = "GuessIt - a library for guessing information from video filenames."
 dependencies = [
     "babelfish>=0.6.0",
     "importlib-resources; python_version < \"3.9\"",
     "python-dateutil",
@@ -463,14 +508,20 @@
 requires_python = ">=3.7"
 summary = "A very fast and expressive template engine."
 dependencies = [
     "MarkupSafe>=2.0",
 ]
 
 [[package]]
+name = "joblib"
+version = "1.2.0"
+requires_python = ">=3.7"
+summary = "Lightweight pipelining with Python functions"
+
+[[package]]
 name = "langcodes"
 version = "3.3.0"
 requires_python = ">=3.6"
 summary = "Tools for labeling human languages with IETF language tags"
 
 [[package]]
 name = "lxml"
@@ -545,15 +596,15 @@
 name = "natsort"
 version = "8.4.0"
 requires_python = ">=3.7"
 summary = "Simple yet flexible natural sorting in Python."
 
 [[package]]
 name = "numpy"
-version = "1.24.3"
+version = "1.24.4"
 requires_python = ">=3.8"
 summary = "Fundamental package for array computing in Python"
 
 [[package]]
 name = "olefile"
 version = "0.46"
 requires_python = ">=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*"
@@ -641,22 +692,22 @@
 name = "pillow"
 version = "9.5.0"
 requires_python = ">=3.7"
 summary = "Python Imaging Library (Fork)"
 
 [[package]]
 name = "platformdirs"
-version = "3.7.0"
+version = "3.8.0"
 requires_python = ">=3.7"
 summary = "A small Python package for determining appropriate platform-specific dirs, e.g. a \"user data dir\"."
 
 [[package]]
 name = "pluggy"
-version = "1.0.0"
-requires_python = ">=3.6"
+version = "1.2.0"
+requires_python = ">=3.7"
 summary = "plugin and hook calling mechanisms for python"
 
 [[package]]
 name = "praw"
 version = "7.7.0"
 requires_python = "~=3.7"
 summary = "PRAW, an acronym for \"Python Reddit API Wrapper\", is a python package that allows for simple access to  Reddit's API."
@@ -783,14 +834,23 @@
 requires_python = ">=3.7"
 summary = "Wrappers for the Cocoa frameworks on macOS"
 dependencies = [
     "pyobjc-core>=9.2",
 ]
 
 [[package]]
+name = "pyproj"
+version = "3.5.0"
+requires_python = ">=3.8"
+summary = "Python interface to PROJ (cartographic projections and coordinate transformations library)"
+dependencies = [
+    "certifi",
+]
+
+[[package]]
 name = "pysrt"
 version = "1.1.2"
 summary = "SubRip (.srt) subtitle parser and writer"
 dependencies = [
     "chardet",
 ]
 
@@ -798,15 +858,15 @@
 name = "pysubs2"
 version = "1.6.1"
 requires_python = ">=3.7"
 summary = "A library for editing subtitle files"
 
 [[package]]
 name = "pytest"
-version = "7.3.2"
+version = "7.4.0"
 requires_python = ">=3.7"
 summary = "pytest: simple powerful testing with Python"
 dependencies = [
     "colorama; sys_platform == \"win32\"",
     "exceptiongroup>=1.0.0rc8; python_version < \"3.11\"",
     "iniconfig",
     "packaging",
@@ -881,15 +941,15 @@
     "markdown-it-py>=2.2.0",
     "pygments<3.0.0,>=2.13.0",
     "typing-extensions<5.0,>=4.0.0; python_version < \"3.9\"",
 ]
 
 [[package]]
 name = "ruff"
-version = "0.0.274"
+version = "0.0.275"
 requires_python = ">=3.7"
 summary = "An extremely fast Python linter, written in Rust."
 
 [[package]]
 name = "scalene"
 version = "1.5.19"
 requires_python = ">=3.8"
@@ -899,14 +959,35 @@
     "cloudpickle>=1.5.0",
     "pynvml>=11.0.0",
     "rich>=10.7.0",
     "wheel>=0.36.1",
 ]
 
 [[package]]
+name = "scikit-learn"
+version = "1.2.2"
+requires_python = ">=3.8"
+summary = "A set of python modules for machine learning and data mining"
+dependencies = [
+    "joblib>=1.1.1",
+    "numpy>=1.17.3",
+    "scipy>=1.3.2",
+    "threadpoolctl>=2.0.0",
+]
+
+[[package]]
+name = "scipy"
+version = "1.9.3"
+requires_python = ">=3.8"
+summary = "Fundamental algorithms for scientific computing in Python"
+dependencies = [
+    "numpy<1.26.0,>=1.18.5",
+]
+
+[[package]]
 name = "screeninfo"
 version = "0.8.1"
 requires_python = ">=3.6.2,<4.0.0"
 summary = "Fetch location and size of physical screens."
 dependencies = [
     "Cython; sys_platform == \"darwin\"",
     "pyobjc-framework-Cocoa; sys_platform == \"darwin\"",
@@ -915,25 +996,29 @@
 [[package]]
 name = "setuptools"
 version = "68.0.0"
 requires_python = ">=3.7"
 summary = "Easily download, build, install, upgrade, and uninstall Python packages"
 
 [[package]]
+name = "shapely"
+version = "2.0.1"
+requires_python = ">=3.7"
+summary = "Manipulation and analysis of geometric objects"
+dependencies = [
+    "numpy>=1.14",
+]
+
+[[package]]
 name = "six"
 version = "1.12.0"
 requires_python = ">=2.6, !=3.0.*, !=3.1.*"
 summary = "Python 2 and 3 compatibility utilities"
 
 [[package]]
-name = "sklearn"
-version = "0.0.post5"
-summary = "deprecated sklearn package, use scikit-learn instead"
-
-[[package]]
 name = "smart-open"
 version = "6.3.0"
 requires_python = ">=3.6,<4.0"
 summary = "Utils for streaming large files (S3, HDFS, GCS, Azure Blob Storage, gzip, bz2...)"
 
 [[package]]
 name = "sortedcontainers"
@@ -994,15 +1079,15 @@
 [[package]]
 name = "sqlite-fts4"
 version = "1.0.3"
 summary = "Python functions for working with SQLite FTS4 search"
 
 [[package]]
 name = "sqlite-utils"
-version = "3.32.1"
+version = "3.33"
 requires_python = ">=3.7"
 summary = "CLI tool and Python library for manipulating SQLite databases"
 dependencies = [
     "click",
     "click-default-group-wheel",
     "python-dateutil",
     "sqlite-fts4",
@@ -1107,14 +1192,20 @@
     "pydantic!=1.8,!=1.8.1,<1.11.0,>=1.7.4",
     "setuptools",
     "srsly<3.0.0,>=2.4.0",
     "wasabi<1.2.0,>=0.8.1",
 ]
 
 [[package]]
+name = "threadpoolctl"
+version = "3.1.0"
+requires_python = ">=3.6"
+summary = "threadpoolctl"
+
+[[package]]
 name = "tinytag"
 version = "1.9.0"
 requires_python = ">=2.7"
 summary = "Read music meta data and length of MP3, OGG, OPUS, MP4, M4A, FLAC, WMA and Wave files"
 
 [[package]]
 name = "tomli"
@@ -1194,15 +1285,15 @@
 [[package]]
 name = "wcwidth"
 version = "0.2.6"
 summary = "Measures the displayed width of unicode strings in a terminal"
 
 [[package]]
 name = "websocket-client"
-version = "1.6.0"
+version = "1.6.1"
 requires_python = ">=3.7"
 summary = "WebSocket client for Python with low level API options"
 
 [[package]]
 name = "websockets"
 version = "11.0.3"
 requires_python = ">=3.7"
@@ -1243,15 +1334,15 @@
 dependencies = [
     "idna>=2.0",
     "multidict>=4.0",
 ]
 
 [[package]]
 name = "yt-dlp"
-version = "2023.6.21"
+version = "2023.6.22"
 requires_python = ">=3.7"
 summary = "A youtube-dl fork with additional features and patches"
 dependencies = [
     "brotli; platform_python_implementation == \"CPython\"",
     "brotlicffi; platform_python_implementation != \"CPython\"",
     "certifi",
     "mutagen",
@@ -1275,15 +1366,15 @@
 requires_python = ">=3.7"
 summary = "Backport of pathlib-compatible object wrapper for zip files"
 
 [metadata]
 lock_version = "4.2"
 cross_platform = true
 groups = ["default", "all", "deluxe", "dev", "test"]
-content_hash = "sha256:def5380a32e603b2ddeeeea22583e403c33051d6f6e517afab5e71d22e69bda9"
+content_hash = "sha256:aa42aafc020e86d43a66a11c7df64ffc69b73f931d34593da3b5938ac26e6a2d"
 
 [metadata.files]
 "aiohttp 3.8.4" = [
     {url = "https://files.pythonhosted.org/packages/03/e7/84b65e341b1f45753fea51158d8a9522e57a5ae804acbc6dc34edf07cea0/aiohttp-3.8.4-cp39-cp39-musllinux_1_1_aarch64.whl", hash = "sha256:bca5f24726e2919de94f047739d0a4fc01372801a3672708260546aa2601bf57"},
     {url = "https://files.pythonhosted.org/packages/04/03/3ce412b191aba5961b4ada3ee7a93498623e218fb4d50ac6d357da61dc26/aiohttp-3.8.4-cp38-cp38-musllinux_1_1_x86_64.whl", hash = "sha256:8189c56eb0ddbb95bfadb8f60ea1b22fcfa659396ea36f6adcc521213cd7b44d"},
     {url = "https://files.pythonhosted.org/packages/05/ee/77b3dc08f41a1bce842e30134233c58b3bbe8c0fa7be121295aa2fad885d/aiohttp-3.8.4-cp39-cp39-musllinux_1_1_x86_64.whl", hash = "sha256:17b79c2963db82086229012cff93ea55196ed31f6493bb1ccd2c62f1724324e4"},
     {url = "https://files.pythonhosted.org/packages/07/3c/04c65b5873524a415509cbcf21787be32c31f4e729840fab9866dd197030/aiohttp-3.8.4-cp36-cp36m-musllinux_1_1_i686.whl", hash = "sha256:7c7837fe8037e96b6dd5cfcf47263c1620a9d332a87ec06a6ca4564e56bd0f36"},
@@ -1774,14 +1865,22 @@
     {url = "https://files.pythonhosted.org/packages/59/87/84326af34517fca8c58418d148f2403df25303e02736832403587318e9e8/click-8.1.3.tar.gz", hash = "sha256:7682dc8afb30297001674575ea00d1814d808d6a36af415a82bd481d37ba7b8e"},
     {url = "https://files.pythonhosted.org/packages/c2/f1/df59e28c642d583f7dacffb1e0965d0e00b218e0186d7858ac5233dce840/click-8.1.3-py3-none-any.whl", hash = "sha256:bb4d8133cb15a609f44e8213d9b391b0809795062913b383c62be0ee95b1db48"},
 ]
 "click-default-group-wheel 1.2.2" = [
     {url = "https://files.pythonhosted.org/packages/0b/77/dbf4952b05efe08ab0ef4be14b6137717c00d0504f5a56ee6e80c010e6d0/click_default_group_wheel-1.2.2-py3-none-any.whl", hash = "sha256:1599b0b6e0ff63ee806c2cb76593cb8cc73e723cd53532c92bc496dc6fc90e5c"},
     {url = "https://files.pythonhosted.org/packages/3d/da/f3bbf30f7e71d881585d598f67f4424b2cc4c68f39849542e81183218017/click-default-group-wheel-1.2.2.tar.gz", hash = "sha256:e90da42d92c03e88a12ed0c0b69c8a29afb5d36e3dc8d29c423ba4219e6d7747"},
 ]
+"click-plugins 1.1.1" = [
+    {url = "https://files.pythonhosted.org/packages/5f/1d/45434f64ed749540af821fd7e42b8e4d23ac04b1eda7c26613288d6cd8a8/click-plugins-1.1.1.tar.gz", hash = "sha256:46ab999744a9d831159c3411bb0c79346d94a444df9a3a3742e9ed63645f264b"},
+    {url = "https://files.pythonhosted.org/packages/e9/da/824b92d9942f4e472702488857914bdd50f73021efea15b4cad9aca8ecef/click_plugins-1.1.1-py2.py3-none-any.whl", hash = "sha256:5d262006d3222f5057fd81e1623d4443e41dcda5dc815c06b442aa3c02889fc8"},
+]
+"cligj 0.7.2" = [
+    {url = "https://files.pythonhosted.org/packages/73/86/43fa9f15c5b9fb6e82620428827cd3c284aa933431405d1bcf5231ae3d3e/cligj-0.7.2-py3-none-any.whl", hash = "sha256:c1ca117dbce1fe20a5809dc96f01e1c2840f6dcc939b3ddbb1111bf330ba82df"},
+    {url = "https://files.pythonhosted.org/packages/ea/0d/837dbd5d8430fd0f01ed72c4cfb2f548180f4c68c635df84ce87956cff32/cligj-0.7.2.tar.gz", hash = "sha256:a4bc13d623356b373c2c27c53dbd9c68cae5d526270bfa71f6c6fa69669c6b27"},
+]
 "cloudpickle 2.2.1" = [
     {url = "https://files.pythonhosted.org/packages/15/80/44286939ca215e88fa827b2aeb6fa3fd2b4a7af322485c7170d6f9fd96e0/cloudpickle-2.2.1-py3-none-any.whl", hash = "sha256:61f594d1f4c295fa5cd9014ceb3a1fc4a70b0de1164b94fbc2d854ccba056f9f"},
     {url = "https://files.pythonhosted.org/packages/5f/51/913ecca3970a2227cf4d5e8937df52cc28f465ac442216110b8e3323262d/cloudpickle-2.2.1.tar.gz", hash = "sha256:d89684b8de9e34a2a43b3460fbca07d09d6e25ce858df4d5a44240403b6178f5"},
 ]
 "colorama 0.4.6" = [
     {url = "https://files.pythonhosted.org/packages/d1/d6/3965ed04c63042e047cb6a3e6ed1a63a35087b6a609aa3a15ed8ac56c221/colorama-0.4.6-py2.py3-none-any.whl", hash = "sha256:4f1d9991f5acc0ca119f9d443620b77f9d6b33703e51011c16baf57afb285fc6"},
     {url = "https://files.pythonhosted.org/packages/d8/53/6f443c9a4a8358a93a6792e2acffb9d9d5cb0a5cfd8802644b7b1c9a02e4/colorama-0.4.6.tar.gz", hash = "sha256:08695f5cb7ed6e0531a20572697297273c47b8cae5a63ffc6d6ed5c201be6e44"},
@@ -1895,14 +1994,36 @@
     {url = "https://files.pythonhosted.org/packages/27/58/601c8b2fc30f648ebb19d67a59a07ff382f8ce2571eb7f172706c8b437fa/extract_msg-0.28.7-py2.py3-none-any.whl", hash = "sha256:6ad2702bef86e6c1b8505e2993c7f3d37a1f3d140903138ee2df4a299dd2a29c"},
     {url = "https://files.pythonhosted.org/packages/67/fb/ed86f4fa53e58e90598f635bba9b4140a20992bd968aaaf8ae1fbacd6e57/extract_msg-0.28.7.tar.gz", hash = "sha256:7ebdbd7863a3699080a69f71ec0cd30ed9bfee70bad9acc6a8e6abe9523c78c0"},
 ]
 "ffmpeg-python 0.2.0" = [
     {url = "https://files.pythonhosted.org/packages/d7/0c/56be52741f75bad4dc6555991fabd2e07b432d333da82c11ad701123888a/ffmpeg_python-0.2.0-py3-none-any.whl", hash = "sha256:ac441a0404e053f8b6a1113a77c0f452f1cfc62f6344a769475ffdc0f56c23c5"},
     {url = "https://files.pythonhosted.org/packages/dd/5e/d5f9105d59c1325759d838af4e973695081fbbc97182baf73afc78dec266/ffmpeg-python-0.2.0.tar.gz", hash = "sha256:65225db34627c578ef0e11c8b1eb528bb35e024752f6f10b78c011f6f64c4127"},
 ]
+"fiona 1.9.4.post1" = [
+    {url = "https://files.pythonhosted.org/packages/16/95/a0b93a97013fb0b5ddd4be7e4844f9524b82bec5fe167314c4a2dce0cf5e/Fiona-1.9.4.post1-cp310-cp310-macosx_11_0_arm64.whl", hash = "sha256:dbe158947099a83ad16f9acd3a21f50ff01114c64e2de67805e382e6b6e0083a"},
+    {url = "https://files.pythonhosted.org/packages/2b/ea/6f581dbc322f9bd7eeb397ca81444dcd0ba1c2aead5113f017be61de8919/Fiona-1.9.4.post1-cp38-cp38-win_amd64.whl", hash = "sha256:a670ea4262cb9140445bcfc97cbfd2f508a058be342f4a97e966b8ce7696601f"},
+    {url = "https://files.pythonhosted.org/packages/3b/c0/1f49b9026e706304a5f214c0758c022cb91367b9b13d0d2cae19847d3c35/Fiona-1.9.4.post1.tar.gz", hash = "sha256:5679d3f7e0d513035eb72e59527bb90486859af4405755dfc739138633106120"},
+    {url = "https://files.pythonhosted.org/packages/43/56/915f3e4c0016f5917d65f70097e1080f1f5341f3cd2d48d9738c2465fffa/Fiona-1.9.4.post1-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:c1faa625d5202b8403471bbc9f9c96b1bf9099cfcb0ee02a80a3641d3d02383e"},
+    {url = "https://files.pythonhosted.org/packages/44/80/64200180c8dacdeadc8192aa6349b3fe2d4051591427149cea97c0a5e744/Fiona-1.9.4.post1-cp38-cp38-macosx_10_15_x86_64.whl", hash = "sha256:71b023ef5248ebfa5524e7a875033f7db3bbfaf634b1b5c1ae36958d1eb82083"},
+    {url = "https://files.pythonhosted.org/packages/57/b9/c3821af48b949f8db275dc5bf0d66fd4cb6a492cd96d3f427bced20945ae/Fiona-1.9.4.post1-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:2c2c7b09eecee3bb074ef8aa518cd6ab30eb663c6fdd0eff3c88d454a9746eaa"},
+    {url = "https://files.pythonhosted.org/packages/62/b6/ca195c42996dd7acb7557cdc8b2487d4889f74e853ef94332c88c2418d74/Fiona-1.9.4.post1-cp37-cp37m-win_amd64.whl", hash = "sha256:450561d308d3ce7c7e30294822b1de3f4f942033b703ddd4a91a7f7f5f506ca0"},
+    {url = "https://files.pythonhosted.org/packages/6e/40/b2830d90c80254dc6fefeb066bd4cbcd305a5058e79cf3fade5706184ea2/Fiona-1.9.4.post1-cp311-cp311-macosx_10_15_x86_64.whl", hash = "sha256:c671d8832287cda397621d79c5a635d52e4631f33a8f0e6fdc732a79a93cb96c"},
+    {url = "https://files.pythonhosted.org/packages/81/04/616d37d4750bd52d606461095a53e55b206be927ac270e497e3bf0962546/Fiona-1.9.4.post1-cp310-cp310-macosx_10_15_x86_64.whl", hash = "sha256:d6483a20037db2209c8e9a0c6f1e552f807d03c8f42ed0c865ab500945a37c4d"},
+    {url = "https://files.pythonhosted.org/packages/8a/61/623b99b4738c27f4e4f5e5f255216a646e7e6e9cd5e22b108dfca8095dfc/Fiona-1.9.4.post1-cp310-cp310-win_amd64.whl", hash = "sha256:1da8b954f6f222c3c782bc285586ea8dd9d7e55e1bc7861da9cd772bca671660"},
+    {url = "https://files.pythonhosted.org/packages/92/da/8dd3d9e9061e90ebe7d173d47547e937a282a8a8d4a4a10c4e7193011536/Fiona-1.9.4.post1-cp39-cp39-win_amd64.whl", hash = "sha256:f5da66b723a876142937e683431bbaa5c3d81bb2ed3ec98941271bc99b7f8cd0"},
+    {url = "https://files.pythonhosted.org/packages/aa/0d/0e13fe2104f5b248ec47eda7345afff763e25c724bb6705a43f4aa28ed96/Fiona-1.9.4.post1-cp37-cp37m-manylinux2014_x86_64.whl", hash = "sha256:b0387cae39e27f338fd948b3b50b6e6ce198cc4cec257fc91660849697c69dc3"},
+    {url = "https://files.pythonhosted.org/packages/ab/51/4353865344a6ac32f7b8ed3f2363a4b1286d5c9e2b53ce3bb61982e3aaa8/Fiona-1.9.4.post1-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:1a585002a6385cc8ab0f66ddf3caf18711f531901906abd011a67a0cc89ab7b0"},
+    {url = "https://files.pythonhosted.org/packages/ae/ab/b6a89cde242f7333c9bdaa314ac73e2ecd9248bc5b1c014323d700289a91/Fiona-1.9.4.post1-cp311-cp311-macosx_11_0_arm64.whl", hash = "sha256:b633a2e550e083805c638d2ab8059c283ca112aaea8241e170c012d2ee0aa905"},
+    {url = "https://files.pythonhosted.org/packages/b0/7f/2de46a2630f609b7520d74ffc7692d4969b1fa1dd3c82f62c7967183d365/Fiona-1.9.4.post1-cp311-cp311-win_amd64.whl", hash = "sha256:39baf11ff0e4318397e2b2197de427b4eebdc49d4a9a7c1366f8a7ed682978a4"},
+    {url = "https://files.pythonhosted.org/packages/b1/dc/a1b2e2dc1278bc2cbdfd5a041a4882c6403e54adaebd95e76f3be4367703/Fiona-1.9.4.post1-cp39-cp39-macosx_11_0_arm64.whl", hash = "sha256:7bfb1f49e0e53f6cd7ad64ae809d72646266b37a7b9881205977408b443a8d79"},
+    {url = "https://files.pythonhosted.org/packages/c0/8e/9be7f11921d7e2f5dcfa748683094e17b5eef38701c5dd2916afd745da8c/Fiona-1.9.4.post1-cp38-cp38-macosx_11_0_arm64.whl", hash = "sha256:74511d3755695d75cea0f4ff6f5e0c6c5d5be8e0d46dafff124c6a219e99b1eb"},
+    {url = "https://files.pythonhosted.org/packages/c7/b3/6de5b6f5f01ee4c7951700a28eaed8c5ee5cc3516c12b1c258f927c0ad5e/Fiona-1.9.4.post1-cp39-cp39-macosx_10_15_x86_64.whl", hash = "sha256:ea7c44c15b3a653452b9b3173181490b7afc5f153b0473c145c43c0fbf90448b"},
+    {url = "https://files.pythonhosted.org/packages/cf/d2/01dc88bef47c0966c2749e35a4ee554583c9c8eebd6e72c0ac9493b116c9/Fiona-1.9.4.post1-cp38-cp38-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:285f3dd4f96aa0a3955ed469f0543375b20989731b2dddc85124453f11ac62bc"},
+    {url = "https://files.pythonhosted.org/packages/db/87/7d5cf9c6c848745f7b4477eb32e6cd629d378ab7f104789d40b37e83a85a/Fiona-1.9.4.post1-cp37-cp37m-macosx_10_15_x86_64.whl", hash = "sha256:d93c993265f6378b23f47708c83bddb3377ca6814a1f0b5a0ae0bee9c8d72cf8"},
+]
 "flask 2.0.2" = [
     {url = "https://files.pythonhosted.org/packages/8f/b6/b4fdcb6d01ee20f9cfe81dcf9d3cd6c2f874b996f186f1c0b898c4a59c04/Flask-2.0.2-py3-none-any.whl", hash = "sha256:cb90f62f1d8e4dc4621f52106613488b5ba826b2e1e10a33eac92f723093ab6a"},
     {url = "https://files.pythonhosted.org/packages/95/40/b976286b5e7ba01794a7e7588e7e7fa27fb16c6168fa849234840bf0f61d/Flask-2.0.2.tar.gz", hash = "sha256:7b2fb8e934ddd50731893bdcdb00fc8c0315916f9fcd50d22c7cc1a95ab634e2"},
 ]
 "frozenlist 1.3.3" = [
     {url = "https://files.pythonhosted.org/packages/01/a3/a3c18bfd7bd2a56831b985140f98eb6dda684a2d8b2a54b1077b45c7f9d9/frozenlist-1.3.3-cp311-cp311-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:23d16d9f477bb55b6154654e0e74557040575d9d19fe78a161bd33d7d76808e8"},
     {url = "https://files.pythonhosted.org/packages/03/00/febbfd2ec244a0f91707bd879afe6aa278e337dc41cd9d0d25260e6da38e/frozenlist-1.3.3-cp38-cp38-win_amd64.whl", hash = "sha256:7f44e24fa70f6fbc74aeec3e971f60a14dde85da364aa87f15d1be94ae75aeef"},
@@ -1986,14 +2107,18 @@
 "future 0.18.3" = [
     {url = "https://files.pythonhosted.org/packages/8f/2e/cf6accf7415237d6faeeebdc7832023c90e0282aa16fd3263db0eb4715ec/future-0.18.3.tar.gz", hash = "sha256:34a17436ed1e96697a86f9de3d15a3b0be01d8bc8de9c1dffd59fb8234ed5307"},
 ]
 "gallery-dl 1.25.6" = [
     {url = "https://files.pythonhosted.org/packages/45/f6/e87f5b13503dff408c202d79d1bdd1c0ff348d92fc463452c02b9f1ae1a3/gallery_dl-1.25.6-py3-none-any.whl", hash = "sha256:a2ae6a06610d905dc86f9ebd091a3619586b9671c70b0c5d3ac9536e4b4cdd80"},
     {url = "https://files.pythonhosted.org/packages/60/78/176e7c4310a6c200372871a005da8ee5447c0e62cd3533172e009b71a94a/gallery_dl-1.25.6.tar.gz", hash = "sha256:0824ceff5b7a9482b69d02adaa05aad07026efad2de6d3a183cbfdf7352463f5"},
 ]
+"geopandas 0.13.2" = [
+    {url = "https://files.pythonhosted.org/packages/cb/7b/2fb6ab376c78d2e60812ad0bf4b24889309d2aeb543f54efcd586c69907f/geopandas-0.13.2-py3-none-any.whl", hash = "sha256:101cfd0de54bcf9e287a55b5ea17ebe0db53a5e25a28bacf100143d0507cabd9"},
+    {url = "https://files.pythonhosted.org/packages/e8/b1/f567b9a2d4e849e8b52b861827c69f53ef5b71bf123546a4f21f3799959a/geopandas-0.13.2.tar.gz", hash = "sha256:e5b56d9c20800c77bcc0c914db3f27447a37b23b2cd892be543f5001a694a968"},
+]
 "guessit 3.7.1" = [
     {url = "https://files.pythonhosted.org/packages/96/5f/64304acee35bac703cee51656a5caf37bd18c9490561fbff225922f41d39/guessit-3.7.1.tar.gz", hash = "sha256:2c18d982ee6db30db5d59557add0324a2b49bf3940a752947510632a2b58a3c1"},
     {url = "https://files.pythonhosted.org/packages/db/5e/eec6416047845a745b1d2aee181244b380e59158e29d814021d2e511b267/guessit-3.7.1-py3-none-any.whl", hash = "sha256:c3be280ee8ec581a45ca6a654a92e317bf89567fdc55e7167452226f4f5b8b38"},
 ]
 "humanize 4.6.0" = [
     {url = "https://files.pythonhosted.org/packages/06/b1/9e491df2ee1c919d67ee328d8bc9f17b7a9af68e4077f3f5fac83a4488c9/humanize-4.6.0.tar.gz", hash = "sha256:5f1f22bc65911eb1a6ffe7659bd6598e33dcfeeb904eb16ee1e705a09bf75916"},
     {url = "https://files.pythonhosted.org/packages/22/2b/30e8725481b071ca53984742a443f944f9c74fb72f509a40b746912645e1/humanize-4.6.0-py3-none-any.whl", hash = "sha256:401201aca462749773f02920139f302450cb548b70489b9b4b92be39fe3c3c50"},
@@ -2042,14 +2167,18 @@
     {url = "https://files.pythonhosted.org/packages/15/02/afd43c5066de05f6b3188f3aa74136a3289e6c30e7a45f351546cab0928c/jedi-0.18.2.tar.gz", hash = "sha256:bae794c30d07f6d910d32a7048af09b5a39ed740918da923c6b780790ebac612"},
     {url = "https://files.pythonhosted.org/packages/6d/60/4acda63286ef6023515eb914543ba36496b8929cb7af49ecce63afde09c6/jedi-0.18.2-py2.py3-none-any.whl", hash = "sha256:203c1fd9d969ab8f2119ec0a3342e0b49910045abe6af0a3ae83a5764d54639e"},
 ]
 "jinja2 3.1.2" = [
     {url = "https://files.pythonhosted.org/packages/7a/ff/75c28576a1d900e87eb6335b063fab47a8ef3c8b4d88524c4bf78f670cce/Jinja2-3.1.2.tar.gz", hash = "sha256:31351a702a408a9e7595a8fc6150fc3f43bb6bf7e319770cbc0db9df9437e852"},
     {url = "https://files.pythonhosted.org/packages/bc/c3/f068337a370801f372f2f8f6bad74a5c140f6fda3d9de154052708dd3c65/Jinja2-3.1.2-py3-none-any.whl", hash = "sha256:6088930bfe239f0e6710546ab9c19c9ef35e29792895fed6e6e31a023a182a61"},
 ]
+"joblib 1.2.0" = [
+    {url = "https://files.pythonhosted.org/packages/45/dd/a5435a6902d6315241c48a5343e6e6675b007e05d3738ed97a7a47864e53/joblib-1.2.0.tar.gz", hash = "sha256:e1cee4a79e4af22881164f218d4311f60074197fb707e082e803b61f6d137018"},
+    {url = "https://files.pythonhosted.org/packages/91/d4/3b4c8e5a30604df4c7518c562d4bf0502f2fa29221459226e140cf846512/joblib-1.2.0-py3-none-any.whl", hash = "sha256:091138ed78f800342968c523bdde947e7a305b8594b910a0fea2ab83c3c6d385"},
+]
 "langcodes 3.3.0" = [
     {url = "https://files.pythonhosted.org/packages/5f/ec/9955d772ecac0bdfb5d706d64f185ac68bd0d4092acdc2c5a1882c824369/langcodes-3.3.0.tar.gz", hash = "sha256:794d07d5a28781231ac335a1561b8442f8648ca07cd518310aeb45d6f0807ef6"},
     {url = "https://files.pythonhosted.org/packages/fe/c3/0d04d248624a181e57c2870127dfa8d371973561caf54333c85e8f9133a2/langcodes-3.3.0-py3-none-any.whl", hash = "sha256:4d89fc9acb6e9c8fdef70bcdf376113a3db09b67285d9e1d534de6d8818e7e69"},
 ]
 "lxml 4.9.2" = [
     {url = "https://files.pythonhosted.org/packages/00/d9/d2ae5c7032157798df585321fc190b51062eb9970edb017ef15127ac899b/lxml-4.9.2-cp38-cp38-musllinux_1_1_x86_64.whl", hash = "sha256:5344a43228767f53a9df6e5b253f8cdca7dfc7b7aeae52551958192f56d98457"},
     {url = "https://files.pythonhosted.org/packages/06/5a/e11cad7b79f2cf3dd2ff8f81fa8ca667e7591d3d8451768589996b65dec1/lxml-4.9.2.tar.gz", hash = "sha256:2455cfaeb7ac70338b3257f41e21f0724f4b5b0c0e7702da67ee6c3640835b67"},
@@ -2311,43 +2440,43 @@
     {url = "https://files.pythonhosted.org/packages/2a/e2/5d3f6ada4297caebe1a2add3b126fe800c96f56dbe5d1988a2cbe0b267aa/mypy_extensions-1.0.0-py3-none-any.whl", hash = "sha256:4392f6c0eb8a5668a69e23d168ffa70f0be9ccfd32b5cc2d26a34ae5b844552d"},
     {url = "https://files.pythonhosted.org/packages/98/a4/1ab47638b92648243faf97a5aeb6ea83059cc3624972ab6b8d2316078d3f/mypy_extensions-1.0.0.tar.gz", hash = "sha256:75dbf8955dc00442a438fc4d0666508a9a97b6bd41aa2f0ffe9d2f2725af0782"},
 ]
 "natsort 8.4.0" = [
     {url = "https://files.pythonhosted.org/packages/e2/a9/a0c57aee75f77794adaf35322f8b6404cbd0f89ad45c87197a937764b7d0/natsort-8.4.0.tar.gz", hash = "sha256:45312c4a0e5507593da193dedd04abb1469253b601ecaf63445ad80f0a1ea581"},
     {url = "https://files.pythonhosted.org/packages/ef/82/7a9d0550484a62c6da82858ee9419f3dd1ccc9aa1c26a1e43da3ecd20b0d/natsort-8.4.0-py3-none-any.whl", hash = "sha256:4732914fb471f56b5cce04d7bae6f164a592c7712e1c85f9ef585e197299521c"},
 ]
-"numpy 1.24.3" = [
-    {url = "https://files.pythonhosted.org/packages/0d/43/643629a4a278b4815541c7d69856c07ddb0e99bdc62b43538d3751eae2d8/numpy-1.24.3-cp39-cp39-macosx_10_9_x86_64.whl", hash = "sha256:4719d5aefb5189f50887773699eaf94e7d1e02bf36c1a9d353d9f46703758ca4"},
-    {url = "https://files.pythonhosted.org/packages/15/b8/cbe1750b9ec78062e5a00ef39ff8bdf189ce753b411b6b35931ababaee47/numpy-1.24.3-pp38-pypy38_pp73-win_amd64.whl", hash = "sha256:35400e6a8d102fd07c71ed7dcadd9eb62ee9a6e84ec159bd48c28235bbb0f8e4"},
-    {url = "https://files.pythonhosted.org/packages/1a/62/af7e78a12207608b23e3b2e248fc823fbef75f17d5defc8a127c5661daca/numpy-1.24.3-cp38-cp38-win_amd64.whl", hash = "sha256:56e48aec79ae238f6e4395886b5eaed058abb7231fb3361ddd7bfdf4eed54289"},
-    {url = "https://files.pythonhosted.org/packages/2c/d4/590ae7df5044465cc9fa2db152ae12468694d62d952b1528ecff328ef7fc/numpy-1.24.3.tar.gz", hash = "sha256:ab344f1bf21f140adab8e47fdbc7c35a477dc01408791f8ba00d018dd0bc5155"},
-    {url = "https://files.pythonhosted.org/packages/53/f7/bf6e2b973c6d6a4c60f722dd95322d4997b4999347d67c5c74a4042a07b7/numpy-1.24.3-cp38-cp38-win32.whl", hash = "sha256:d933fabd8f6a319e8530d0de4fcc2e6a61917e0b0c271fded460032db42a0fe4"},
-    {url = "https://files.pythonhosted.org/packages/54/41/fb17c1d48a574c50422ff3f1b17ed979b755adc6ed291c4a44a76e226c67/numpy-1.24.3-cp39-cp39-macosx_11_0_arm64.whl", hash = "sha256:0ec87a7084caa559c36e0a2309e4ecb1baa03b687201d0a847c8b0ed476a7187"},
-    {url = "https://files.pythonhosted.org/packages/5a/ab/d0eff89e0c05cc86fa7955c5e54e8ed0957a8a97a2516384b9ffd82008cc/numpy-1.24.3-pp38-pypy38_pp73-macosx_10_9_x86_64.whl", hash = "sha256:352ee00c7f8387b44d19f4cada524586f07379c0d49270f87233983bc5087ca0"},
-    {url = "https://files.pythonhosted.org/packages/62/e4/cd77d5f3d02c30d9ca8f2995df3cb3974c75cf1cc777fad445753475c4e4/numpy-1.24.3-cp310-cp310-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:8535303847b89aa6b0f00aa1dc62867b5a32923e4d1681a35b5eef2d9591a463"},
-    {url = "https://files.pythonhosted.org/packages/65/5d/46da284b0bf6cfbf04082c3c5e84399664d69e41c11a33587ad49b0c64e5/numpy-1.24.3-cp310-cp310-win_amd64.whl", hash = "sha256:ab5f23af8c16022663a652d3b25dcdc272ac3f83c3af4c02eb8b824e6b3ab9d7"},
-    {url = "https://files.pythonhosted.org/packages/6f/72/38f9a536bdb5bfb1682f2520f133ec6e08dde8bcca1f632e347641d90763/numpy-1.24.3-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:2d926b52ba1367f9acb76b0df6ed21f0b16a1ad87c6720a1121674e5cf63e2b6"},
-    {url = "https://files.pythonhosted.org/packages/72/eb/9c77bbc4d2b4ca17ef253621794a2d42897d896f86cd493db3eabe1a7d25/numpy-1.24.3-cp311-cp311-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:76e3f4e85fc5d4fd311f6e9b794d0c00e7002ec122be271f2019d63376f1d385"},
-    {url = "https://files.pythonhosted.org/packages/76/7c/cfb8ac4925defbe222aec15ac6b42b2a3d9bab7c9d13a2e767f534b35c2e/numpy-1.24.3-cp39-cp39-win_amd64.whl", hash = "sha256:d5036197ecae68d7f491fcdb4df90082b0d4960ca6599ba2659957aafced7c17"},
-    {url = "https://files.pythonhosted.org/packages/79/4a/63a79242763edde0b5025d104cc2b78c44d89310b1bbc9b0f64a96b72ea0/numpy-1.24.3-cp38-cp38-macosx_10_9_x86_64.whl", hash = "sha256:7776ea65423ca6a15255ba1872d82d207bd1e09f6d0894ee4a64678dd2204078"},
-    {url = "https://files.pythonhosted.org/packages/82/19/321d369ede7458500f59151101470129d14f3b6768bb9b99bb7156f526b5/numpy-1.24.3-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:a1d3c026f57ceaad42f8231305d4653d5f05dc6332a730ae5c0bea3513de0950"},
-    {url = "https://files.pythonhosted.org/packages/83/be/de078ac5e4ff572b1bdac1808b77cea2013b2c6286282f89b1de3e951273/numpy-1.24.3-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:210461d87fb02a84ef243cac5e814aad2b7f4be953b32cb53327bb49fd77fbb4"},
-    {url = "https://files.pythonhosted.org/packages/89/e3/e2f478b2ff131e7c3171044a87e74df61db4b67fbcb90be479c07a44d0a7/numpy-1.24.3-cp310-cp310-win32.whl", hash = "sha256:f21c442fdd2805e91799fbe044a7b999b8571bb0ab0f7850d0cb9641a687092b"},
-    {url = "https://files.pythonhosted.org/packages/8b/d9/814a619ab84d8eb0d95e08d4c723e665f1e694b5a6068ca505a61bdc3745/numpy-1.24.3-cp38-cp38-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:4749e053a29364d3452c034827102ee100986903263e89884922ef01a0a6fd2f"},
-    {url = "https://files.pythonhosted.org/packages/94/84/ed45416c8319c02348a5812d5647796a0833e3fb5576d01758f2a72e9200/numpy-1.24.3-cp311-cp311-win32.whl", hash = "sha256:c91c4afd8abc3908e00a44b2672718905b8611503f7ff87390cc0ac3423fb096"},
-    {url = "https://files.pythonhosted.org/packages/96/92/2a8c1356e226311cf885e04eff576df8c357b2626c47c9283024bc24e01e/numpy-1.24.3-cp39-cp39-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:ea8282b9bcfe2b5e7d491d0bf7f3e2da29700cec05b49e64d6246923329f2b02"},
-    {url = "https://files.pythonhosted.org/packages/a7/fe/72493149c65dcd39d8c8dc09870e242bd689d1db2bde3ec479807bf0d414/numpy-1.24.3-cp38-cp38-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:ecde0f8adef7dfdec993fd54b0f78183051b6580f606111a6d789cd14c61ea0c"},
-    {url = "https://files.pythonhosted.org/packages/ca/13/c5bc0100b425f007412c3ba5d71e5ae9c08260fecbffd620764a9df1f4de/numpy-1.24.3-cp38-cp38-macosx_11_0_arm64.whl", hash = "sha256:ae8d0be48d1b6ed82588934aaaa179875e7dc4f3d84da18d7eae6eb3f06c242c"},
-    {url = "https://files.pythonhosted.org/packages/d5/d6/07b37e7fecad7d158aabb4782a1b941e10afe8b80ec24cd64285a5bbb81b/numpy-1.24.3-cp39-cp39-win32.whl", hash = "sha256:784c6da1a07818491b0ffd63c6bbe5a33deaa0e25a20e1b3ea20cf0e43f8046c"},
-    {url = "https://files.pythonhosted.org/packages/eb/10/2c3c672034d860bcca50b65d656e24c4e2ace9fb452fdd81da78cb7418a1/numpy-1.24.3-pp38-pypy38_pp73-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:1a7d6acc2e7524c9955e5c903160aa4ea083736fde7e91276b0e5d98e6332812"},
-    {url = "https://files.pythonhosted.org/packages/ec/7d/f69c47ea3db0cd8ca444aec241a80b538eb176ae756820489a9d2946ec8c/numpy-1.24.3-cp311-cp311-macosx_10_9_x86_64.whl", hash = "sha256:9a7721ec204d3a237225db3e194c25268faf92e19338a35f3a224469cb6039a3"},
-    {url = "https://files.pythonhosted.org/packages/ee/6c/7217a8844dfe22e349bccbecd35571fa72c5d7fe8b33d8c5540e8cc2535c/numpy-1.24.3-cp311-cp311-macosx_11_0_arm64.whl", hash = "sha256:d6cc757de514c00b24ae8cf5c876af2a7c3df189028d68c0cb4eaa9cd5afc2bf"},
-    {url = "https://files.pythonhosted.org/packages/f0/e8/1ea9adebdccaadfc208c7517e09f5145ed5a73069779ff436393085d47a2/numpy-1.24.3-cp311-cp311-win_amd64.whl", hash = "sha256:5342cf6aad47943286afa6f1609cad9b4266a05e7f2ec408e2cf7aea7ff69d80"},
-    {url = "https://files.pythonhosted.org/packages/f3/23/7cc851bae09cf4db90d42a701dfe525780883ada86bece45e3da7a07e76b/numpy-1.24.3-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:3c1104d3c036fb81ab923f507536daedc718d0ad5a8707c6061cdfd6d184e570"},
-    {url = "https://files.pythonhosted.org/packages/fa/7d/8dfb40eecbb6bc83ca00ef979f5cdeca5909a250cb8b642dcf1fbd34c078/numpy-1.24.3-cp310-cp310-macosx_11_0_arm64.whl", hash = "sha256:202de8f38fc4a45a3eea4b63e2f376e5f2dc64ef0fa692838e31a808520efaf7"},
+"numpy 1.24.4" = [
+    {url = "https://files.pythonhosted.org/packages/10/be/ae5bf4737cb79ba437879915791f6f26d92583c738d7d960ad94e5c36adf/numpy-1.24.4-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:7ffe43c74893dbf38c2b0a1f5428760a1a9c98285553c89e12d70a96a7f3a4d6"},
+    {url = "https://files.pythonhosted.org/packages/11/10/943cfb579f1a02909ff96464c69893b1d25be3731b5d3652c2e0cf1281ea/numpy-1.24.4-cp38-cp38-macosx_10_9_x86_64.whl", hash = "sha256:1452241c290f3e2a312c137a9999cdbf63f78864d63c79039bda65ee86943f61"},
+    {url = "https://files.pythonhosted.org/packages/14/27/638aaa446f39113a3ed38b37a66243e21b38110d021bfcb940c383e120f2/numpy-1.24.4-cp39-cp39-macosx_11_0_arm64.whl", hash = "sha256:9667575fb6d13c95f1b36aca12c5ee3356bf001b714fc354eb5465ce1609e62f"},
+    {url = "https://files.pythonhosted.org/packages/18/9d/e02ace5d7dfccee796c37b995c63322674daf88ae2f4a4724c5dd0afcc91/numpy-1.24.4-cp39-cp39-win32.whl", hash = "sha256:6620c0acd41dbcb368610bb2f4d83145674040025e5536954782467100aa8835"},
+    {url = "https://files.pythonhosted.org/packages/22/55/3d5a7c1142e0d9329ad27cece17933b0e2ab4e54ddc5c1861fbfeb3f7693/numpy-1.24.4-cp310-cp310-win_amd64.whl", hash = "sha256:b4bea75e47d9586d31e892a7401f76e909712a0fd510f58f5337bea9572c571e"},
+    {url = "https://files.pythonhosted.org/packages/22/97/dfb1a31bb46686f09e68ea6ac5c63fdee0d22d7b23b8f3f7ea07712869ef/numpy-1.24.4-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:7215847ce88a85ce39baf9e89070cb860c98fdddacbaa6c0da3ffb31b3350bd5"},
+    {url = "https://files.pythonhosted.org/packages/25/6f/2586a50ad72e8dbb1d8381f837008a0321a3516dfd7cb57fc8cf7e4bb06b/numpy-1.24.4-cp38-cp38-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:a5425b114831d1e77e4b5d812b69d11d962e104095a5b9c3b641a218abcc050e"},
+    {url = "https://files.pythonhosted.org/packages/35/e2/76a11e54139654a324d107da1d98f99e7aa2a7ef97cfd7c631fba7dbde71/numpy-1.24.4-cp311-cp311-win32.whl", hash = "sha256:4979217d7de511a8d57f4b4b5b2b965f707768440c17cb70fbf254c4b225238d"},
+    {url = "https://files.pythonhosted.org/packages/42/e7/4bf953c6e05df90c6d351af69966384fed8e988d0e8c54dad7103b59f3ba/numpy-1.24.4-pp38-pypy38_pp73-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:95f7ac6540e95bc440ad77f56e520da5bf877f87dca58bd095288dce8940532a"},
+    {url = "https://files.pythonhosted.org/packages/5a/b3/2f9c21d799fa07053ffa151faccdceeb69beec5a010576b8991f614021f7/numpy-1.24.4-cp310-cp310-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:79fc682a374c4a8ed08b331bef9c5f582585d1048fa6d80bc6c35bc384eee9b4"},
+    {url = "https://files.pythonhosted.org/packages/63/38/6cc19d6b8bfa1d1a459daf2b3fe325453153ca7019976274b6f33d8b5663/numpy-1.24.4-cp39-cp39-win_amd64.whl", hash = "sha256:befe2bf740fd8373cf56149a5c23a0f601e82869598d41f8e188a0e9869926f8"},
+    {url = "https://files.pythonhosted.org/packages/64/5f/3f01d753e2175cfade1013eea08db99ba1ee4bdb147ebcf3623b75d12aa7/numpy-1.24.4-cp310-cp310-macosx_11_0_arm64.whl", hash = "sha256:ed094d4f0c177b1b8e7aa9cba7d6ceed51c0e569a5318ac0ca9a090680a6a1b1"},
+    {url = "https://files.pythonhosted.org/packages/69/65/0d47953afa0ad569d12de5f65d964321c208492064c38fe3b0b9744f8d44/numpy-1.24.4-cp38-cp38-win_amd64.whl", hash = "sha256:692f2e0f55794943c5bfff12b3f56f99af76f902fc47487bdfe97856de51a706"},
+    {url = "https://files.pythonhosted.org/packages/6b/80/6cdfb3e275d95155a34659163b83c09e3a3ff9f1456880bec6cc63d71083/numpy-1.24.4-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:c0bfb52d2169d58c1cdb8cc1f16989101639b34c7d3ce60ed70b19c63eba0b64"},
+    {url = "https://files.pythonhosted.org/packages/7a/7c/d7b2a0417af6428440c0ad7cb9799073e507b1a465f827d058b826236964/numpy-1.24.4-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:d11efb4dbecbdf22508d55e48d9c8384db795e1b7b51ea735289ff96613ff74d"},
+    {url = "https://files.pythonhosted.org/packages/8f/27/91894916e50627476cff1a4e4363ab6179d01077d71b9afed41d9e1f18bf/numpy-1.24.4-cp39-cp39-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:f3a86ed21e4f87050382c7bc96571755193c4c1392490744ac73d660e8f564a9"},
+    {url = "https://files.pythonhosted.org/packages/98/5d/5738903efe0ecb73e51eb44feafba32bdba2081263d40c5043568ff60faf/numpy-1.24.4-cp38-cp38-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:dd80e219fd4c71fc3699fc1dadac5dcf4fd882bfc6f7ec53d30fa197b8ee22dc"},
+    {url = "https://files.pythonhosted.org/packages/9a/cd/d5b0402b801c8a8b56b04c1e85c6165efab298d2f0ab741c2406516ede3a/numpy-1.24.4-cp39-cp39-macosx_10_9_x86_64.whl", hash = "sha256:2541312fbf09977f3b3ad449c4e5f4bb55d0dbf79226d7724211acc905049400"},
+    {url = "https://files.pythonhosted.org/packages/a4/9b/027bec52c633f6556dba6b722d9a0befb40498b9ceddd29cbe67a45a127c/numpy-1.24.4.tar.gz", hash = "sha256:80f5e3a4e498641401868df4208b74581206afbee7cf7b8329daae82676d9463"},
+    {url = "https://files.pythonhosted.org/packages/a4/fd/8dff40e25e937c94257455c237b9b6bf5a30d42dd1cc11555533be099492/numpy-1.24.4-pp38-pypy38_pp73-macosx_10_9_x86_64.whl", hash = "sha256:31f13e25b4e304632a4619d0e0777662c2ffea99fcae2029556b17d8ff958aef"},
+    {url = "https://files.pythonhosted.org/packages/a7/4c/96cdaa34f54c05e97c1c50f39f98d608f96f0677a6589e64e53104e22904/numpy-1.24.4-cp311-cp311-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:222e40d0e2548690405b0b3c7b21d1169117391c2e82c378467ef9ab4c8f0da7"},
+    {url = "https://files.pythonhosted.org/packages/a7/ae/f53b7b265fdc701e663fbb322a8e9d4b14d9cb7b2385f45ddfabfc4327e4/numpy-1.24.4-cp38-cp38-macosx_11_0_arm64.whl", hash = "sha256:04640dab83f7c6c85abf9cd729c5b65f1ebd0ccf9de90b270cd61935eef0197f"},
+    {url = "https://files.pythonhosted.org/packages/a9/cc/5ed2280a27e5dab12994c884f1f4d8c3bd4d885d02ae9e52a9d213a6a5e2/numpy-1.24.4-cp311-cp311-macosx_10_9_x86_64.whl", hash = "sha256:f136bab9c2cfd8da131132c2cf6cc27331dd6fae65f95f69dcd4ae3c3639c810"},
+    {url = "https://files.pythonhosted.org/packages/c0/64/908c1087be6285f40e4b3e79454552a701664a079321cff519d8c7051d06/numpy-1.24.4-cp310-cp310-win32.whl", hash = "sha256:4c21decb6ea94057331e111a5bed9a79d335658c27ce2adb580fb4d54f2ad9bc"},
+    {url = "https://files.pythonhosted.org/packages/c0/bc/77635c657a3668cf652806210b8662e1aff84b818a55ba88257abf6637a8/numpy-1.24.4-cp311-cp311-macosx_11_0_arm64.whl", hash = "sha256:e2926dac25b313635e4d6cf4dc4e51c8c0ebfed60b801c799ffc4c32bf3d1254"},
+    {url = "https://files.pythonhosted.org/packages/d1/57/8d328f0b91c733aa9aa7ee540dbc49b58796c862b4fbcb1146c701e888da/numpy-1.24.4-cp38-cp38-win32.whl", hash = "sha256:4602244f345453db537be5314d3983dbf5834a9701b7723ec28923e2889e0bb2"},
+    {url = "https://files.pythonhosted.org/packages/d8/ec/ebef2f7d7c28503f958f0f8b992e7ce606fb74f9e891199329d5f5f87404/numpy-1.24.4-cp311-cp311-win_amd64.whl", hash = "sha256:b7b1fc9864d7d39e28f41d089bfd6353cb5f27ecd9905348c24187a768c79694"},
+    {url = "https://files.pythonhosted.org/packages/fc/dd/9106005eb477d022b60b3817ed5937a43dad8fd1f20b0610ea8a32fcb407/numpy-1.24.4-pp38-pypy38_pp73-win_amd64.whl", hash = "sha256:e98f220aa76ca2a977fe435f5b04d7b3470c0a2e6312907b37ba6068f26787f2"},
 ]
 "olefile 0.46" = [
     {url = "https://files.pythonhosted.org/packages/34/81/e1ac43c6b45b4c5f8d9352396a14144bba52c8fec72a80f425f6a4d653ad/olefile-0.46.zip", hash = "sha256:133b031eaf8fd2c9399b78b8bc5b8fcbe4c31e85295749bb17a87cba8f3c3964"},
 ]
 "orjson 3.9.1" = [
     {url = "https://files.pythonhosted.org/packages/0a/9d/19dd0d6cedcfec3355f2808dc3927b04c629e9d2eca5914a0360f1b2ada5/orjson-3.9.1-cp37-cp37m-macosx_10_15_x86_64.macosx_11_0_arm64.macosx_10_15_universal2.whl", hash = "sha256:d4b68d01a506242316a07f1d2f29fb0a8b36cee30a7c35076f1ef59dce0890c1"},
     {url = "https://files.pythonhosted.org/packages/15/c4/3a97924d8768fa982042f1b5b7a1c8dbb161815b8545a4af9faa73b0a4d7/orjson-3.9.1-cp37-cp37m-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:06f6ab4697fab090517f295915318763a97a12ee8186054adf21c1e6f6abbd3d"},
@@ -2519,21 +2648,21 @@
     {url = "https://files.pythonhosted.org/packages/d9/0e/7c6f054022235830dc2c37ec83e947d9ca09b0b0361e1e5e29983da92294/Pillow-9.5.0-pp38-pypy38_pp73-win_amd64.whl", hash = "sha256:cb841572862f629b99725ebaec3287fc6d275be9b14443ea746c1dd325053cbd"},
     {url = "https://files.pythonhosted.org/packages/db/5c/ba9e291850f594f89436cdca93d36c6f8610d4fb7833a6c257f4481d4174/Pillow-9.5.0-cp38-cp38-musllinux_1_1_x86_64.whl", hash = "sha256:662da1f3f89a302cc22faa9f14a262c2e3951f9dbc9617609a47521c69dd9f8f"},
     {url = "https://files.pythonhosted.org/packages/e7/2a/f3ed578595f8486ee2cc07434460097d89aedd406a3db849b890ca8ec416/Pillow-9.5.0-cp39-cp39-musllinux_1_1_aarch64.whl", hash = "sha256:a127ae76092974abfbfa38ca2d12cbeddcdeac0fb71f9627cc1135bedaf9d51a"},
     {url = "https://files.pythonhosted.org/packages/ec/7d/01404982db598f271ac7c0d0207860f60ab9288cfacce9872eb567cfbfe3/Pillow-9.5.0-cp37-cp37m-macosx_10_10_x86_64.whl", hash = "sha256:5d4ebf8e1db4441a55c509c4baa7a0587a0210f7cd25fcfe74dbbce7a4bd1906"},
     {url = "https://files.pythonhosted.org/packages/f2/43/0892913d499c8df2c88dee69d59e77de19e0c51754a9be82023880641c09/Pillow-9.5.0-cp39-cp39-manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:8aca1152d93dcc27dc55395604dcfc55bed5f25ef4c98716a928bacba90d33a3"},
     {url = "https://files.pythonhosted.org/packages/ff/fc/48a51c0fe2a00d5def57b9981a1e0f8339b516351da7a51500383d833bc8/Pillow-9.5.0-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:608488bdcbdb4ba7837461442b90ea6f3079397ddc968c31265c1e056964f1ef"},
 ]
-"platformdirs 3.7.0" = [
-    {url = "https://files.pythonhosted.org/packages/14/62/d8277379c30fc6b0347aaf8ff63e5c9e013e0da95f40ba957c5e098b06c2/platformdirs-3.7.0-py3-none-any.whl", hash = "sha256:cfd065ba43133ff103ab3bd10aecb095c2a0035fcd1f07217c9376900d94ba07"},
-    {url = "https://files.pythonhosted.org/packages/a1/45/ff5224bbf1a9f23d95f70890659a7c2639a25d594adfe4a5ca9221f6cae5/platformdirs-3.7.0.tar.gz", hash = "sha256:87fbf6473e87c078d536980ba970a472422e94f17b752cfad17024c18876d481"},
-]
-"pluggy 1.0.0" = [
-    {url = "https://files.pythonhosted.org/packages/9e/01/f38e2ff29715251cf25532b9082a1589ab7e4f571ced434f98d0139336dc/pluggy-1.0.0-py2.py3-none-any.whl", hash = "sha256:74134bbf457f031a36d68416e1509f34bd5ccc019f0bcc952c7b909d06b37bd3"},
-    {url = "https://files.pythonhosted.org/packages/a1/16/db2d7de3474b6e37cbb9c008965ee63835bba517e22cdb8c35b5116b5ce1/pluggy-1.0.0.tar.gz", hash = "sha256:4224373bacce55f955a878bf9cfa763c1e360858e330072059e10bad68531159"},
+"platformdirs 3.8.0" = [
+    {url = "https://files.pythonhosted.org/packages/cb/10/e5478cc0c3ee5563f91ab7b9da15d16e21f3737b6286ed3fd9a8fb1a99dd/platformdirs-3.8.0.tar.gz", hash = "sha256:b0cabcb11063d21a0b261d557acb0a9d2126350e63b70cdf7db6347baea456dc"},
+    {url = "https://files.pythonhosted.org/packages/e7/61/7fde5beff25a0dae6c2056203696169bd29188b6cedefff8ba6e7b54417b/platformdirs-3.8.0-py3-none-any.whl", hash = "sha256:ca9ed98ce73076ba72e092b23d3c93ea6c4e186b3f1c3dad6edd98ff6ffcca2e"},
+]
+"pluggy 1.2.0" = [
+    {url = "https://files.pythonhosted.org/packages/51/32/4a79112b8b87b21450b066e102d6608907f4c885ed7b04c3fdb085d4d6ae/pluggy-1.2.0-py3-none-any.whl", hash = "sha256:c2fd55a7d7a3863cba1a013e4e2414658b1d07b6bc57b3919e0c63c9abb99849"},
+    {url = "https://files.pythonhosted.org/packages/8a/42/8f2833655a29c4e9cb52ee8a2be04ceac61bcff4a680fb338cbd3d1e322d/pluggy-1.2.0.tar.gz", hash = "sha256:d12f0c4b579b15f5e054301bb226ee85eeeba08ffec228092f8defbaa3a4c4b3"},
 ]
 "praw 7.7.0" = [
     {url = "https://files.pythonhosted.org/packages/b3/93/55ae62910b94b46ecdd0ee8765289304f8df8deeaa1df7a96b0831c637ff/praw-7.7.0-py3-none-any.whl", hash = "sha256:22155c4b3006733a5ab0754136cf2226917747b61ec037ee335246fe0db5420e"},
     {url = "https://files.pythonhosted.org/packages/e5/f2/b784acf53cbb554dd7dd024f9095e1c89e74b294bba2fa187930f22f44cf/praw-7.7.0.tar.gz", hash = "sha256:090d209b35f79dfa36082ed1cdaa0f9a753b9277a69cfe8f9f32fa1827411a5a"},
 ]
 "prawcore 2.3.0" = [
     {url = "https://files.pythonhosted.org/packages/d6/36/55cc2cab22aafbebd52ddac4ccb670b920b54eb6ddbdb8573c79ca870d8a/prawcore-2.3.0-py3-none-any.whl", hash = "sha256:48c17db447fa06a13ca3e722201f443031437708daa736c05a1df895fbcceff5"},
@@ -2768,24 +2897,61 @@
     {url = "https://files.pythonhosted.org/packages/38/91/c54fdffda6d7cfad67ff617f19001163658d50bc72376d1584e691cf4895/pyobjc-framework-Cocoa-9.2.tar.gz", hash = "sha256:efd78080872d8c8de6c2b97e0e4eac99d6203a5d1637aa135d071d464eb2db53"},
     {url = "https://files.pythonhosted.org/packages/64/09/d0eb252549b3009f008c8415c9739a9c726ddfec9adc1aa92b6a8dec0efe/pyobjc_framework_Cocoa-9.2-cp39-cp39-macosx_10_9_universal2.whl", hash = "sha256:b236bb965e41aeb2e215d4e98a5a230d4b63252c6d26e00924ea2e69540a59d6"},
     {url = "https://files.pythonhosted.org/packages/9b/e2/49ea296127184f8b578838ba0d3d170abb75c23760d940f952df0fe0e132/pyobjc_framework_Cocoa-9.2-cp38-cp38-macosx_10_9_x86_64.whl", hash = "sha256:739a421e14382a46cbeb9a883f192dceff368ad28ec34d895c48c0ad34cf2c1d"},
     {url = "https://files.pythonhosted.org/packages/d7/b3/e9c6d3e8d53453567805ca461cf52a08807ca2c860c1364c27dc10cdc67e/pyobjc_framework_Cocoa-9.2-cp310-cp310-macosx_10_9_universal2.whl", hash = "sha256:9e02d8a7cc4eb7685377c50ba4f17345701acf4c05b1e7480d421bff9e2f62a4"},
     {url = "https://files.pythonhosted.org/packages/e0/f6/ecbc6323aa12df79acdaf8a75f7bb93d273b6dcd0c5b65658c2505bbc977/pyobjc_framework_Cocoa-9.2-cp312-cp312-macosx_10_9_universal2.whl", hash = "sha256:312977ce2e3989073c6b324c69ba24283de206fe7acd6dbbbaf3e29238a22537"},
     {url = "https://files.pythonhosted.org/packages/fa/f1/d3d3528d1d62d3e21211bcb8bd6bfe1b8c2815d700eb986fdb1f37de9c7d/pyobjc_framework_Cocoa-9.2-cp37-cp37m-macosx_10_9_x86_64.whl", hash = "sha256:aae7841cf40c26dd915f4dd828f91c6616e6b7998630b72e704750c09e00f334"},
 ]
+"pyproj 3.5.0" = [
+    {url = "https://files.pythonhosted.org/packages/09/92/3e89e4bab0a6f0bc2ede2f56197eaf8cf8b7eb3dc88a6302c563e947501d/pyproj-3.5.0-cp38-cp38-macosx_10_9_x86_64.whl", hash = "sha256:2b708fd43453b985642b737d4a6e7f1d6a0ab1677ffa4e14cc258537b49224b0"},
+    {url = "https://files.pythonhosted.org/packages/0a/0d/5feef9b2e2e447f23c3289db4dc100e6e28510b87c6cfbd14ad338bdfd49/pyproj-3.5.0-cp38-cp38-manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:71b65f2a38cd9e16883dbb0f8ae82bdf8f6b79b1b02975c78483ab8428dbbf2f"},
+    {url = "https://files.pythonhosted.org/packages/0c/8a/1febafc7bdeeede1f0bf76411ff55db266d25ce5ad713050973b7c3e29b7/pyproj-3.5.0-cp311-cp311-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:621d78a9d8bf4d06e08bef2471021fbcb1a65aa629ad4a20c22e521ce729cc20"},
+    {url = "https://files.pythonhosted.org/packages/11/3a/c49b3dd5fad200ab0f061540f574b12638cf4c5a3e9d167f2a9e2d5dd5a0/pyproj-3.5.0-pp39-pypy39_pp73-macosx_10_9_x86_64.whl", hash = "sha256:fde5ece4d2436b5a57c8f5f97b49b5de06a856d03959f836c957d3e609f2de7e"},
+    {url = "https://files.pythonhosted.org/packages/12/e3/3c158c05a43f3ec53091e284100b49733f69dbff359bce64ef749fc2751c/pyproj-3.5.0-cp39-cp39-manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:385b0341861d3ebc8cad98337a738821dcb548d465576527399f4955ca24b6ed"},
+    {url = "https://files.pythonhosted.org/packages/16/d1/683c6264931ff8ecf11b63f7a5d2c705cb5aa91f50bbd3e08a5e5a1e3aee/pyproj-3.5.0-cp38-cp38-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:38862fe07316ae12b79d82d298e390973a4f00b684f3c2d037238e20e00610ba"},
+    {url = "https://files.pythonhosted.org/packages/1b/01/6df17f3b802b2d49480c102516dff30d294c4d300dbc3dfa9a9867b83609/pyproj-3.5.0-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:1b7c2113c4d11184a238077ec85e31eda1dcc58ffeb9a4429830e0a7036e787d"},
+    {url = "https://files.pythonhosted.org/packages/43/62/f157de7f1946c075325f67d82e81ab3e424fbac516a8df968b96312494c6/pyproj-3.5.0-cp38-cp38-win32.whl", hash = "sha256:b937215bfbaf404ec8f03ca741fc3f9f2c4c2c5590a02ccddddd820ae3c71331"},
+    {url = "https://files.pythonhosted.org/packages/44/b9/c278d17300f931e96dd8cc26a7afb46dc08ec82d74e1515ba355c1df17f1/pyproj-3.5.0-cp310-cp310-macosx_11_0_arm64.whl", hash = "sha256:61e4ad57d89b03a7b173793b31bca8ee110112cde1937ef0f42a70b9120c827d"},
+    {url = "https://files.pythonhosted.org/packages/47/05/0fafb80be2f90c00d5f5d659919259ba5a051079cf826dc668df5a938dae/pyproj-3.5.0-pp38-pypy38_pp73-manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:788a5dadb532644a64efe0f5f01bf508c821eb7e984f13a677d56002f1e8a67a"},
+    {url = "https://files.pythonhosted.org/packages/54/9e/3aabbd3e521eab15040348e66d7571d6514c528b18532c3e0dbd6268e799/pyproj-3.5.0-cp310-cp310-win32.whl", hash = "sha256:6f316a66031a14e9c5a88c91f8b77aa97f5454895674541ed6ab630b682be35d"},
+    {url = "https://files.pythonhosted.org/packages/65/76/4ab2d022d0978ecd1f598c1b0a464a78885070dc41c03ce362f26e513d8b/pyproj-3.5.0-cp310-cp310-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:7bdd2021bb6f7f346bfe1d2a358aa109da017d22c4704af2d994e7c7ee0a7a53"},
+    {url = "https://files.pythonhosted.org/packages/75/b4/f1f70c33519f223ecd4c1227ca840d8501e405e07d38b9f783969c41f9c8/pyproj-3.5.0-cp311-cp311-manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:d9a024370e917c899bff9171f03ea6079deecdc7482a146a2c565f3b9df134ea"},
+    {url = "https://files.pythonhosted.org/packages/77/77/cbdb48696e33abfab7a342184d9a37274bf67bd7a442b6ab74418b5e6e20/pyproj-3.5.0-pp38-pypy38_pp73-macosx_10_9_x86_64.whl", hash = "sha256:d711517a8487ef3245b08dc82f781a906df9abb3b6cb0ce0486f0eeb823ca570"},
+    {url = "https://files.pythonhosted.org/packages/7d/dc/fc51814f1a1038a344f596aed3e1c5da33893f2965a398ea0c932dfe93f4/pyproj-3.5.0-cp311-cp311-macosx_10_9_x86_64.whl", hash = "sha256:7572983134e310e0ca809c63f1722557a040fe9443df5f247bf11ba887eb1229"},
+    {url = "https://files.pythonhosted.org/packages/81/ba/ff6015d09cd8510367114fd1602051043c7847ad8fea077308feca9904d7/pyproj-3.5.0-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:cd5e2b6aa255023c4acd0b977590f1f7cc801ba21b4d806fcf6dfac3474ebb83"},
+    {url = "https://files.pythonhosted.org/packages/8d/b0/4de0af66387a6a8ffa2309c92c994872a8e6c49a29a45ed90da4935963a2/pyproj-3.5.0-cp38-cp38-macosx_11_0_arm64.whl", hash = "sha256:b60d93a200639e8367c6542a964fd0aa2dbd152f256c1831dc18cd5aa470fb8a"},
+    {url = "https://files.pythonhosted.org/packages/8e/29/9e37087c94128aff0892080bf6aff9375a3c7d491780ed670cd57ea63dce/pyproj-3.5.0-cp311-cp311-macosx_11_0_arm64.whl", hash = "sha256:eccb417b91d0be27805dfc97550bfb8b7db94e9fe1db5ebedb98f5b88d601323"},
+    {url = "https://files.pythonhosted.org/packages/94/d1/657cff06d9c539b7646b1deea97c1880cbfcf2099e54f49a589682d4b99a/pyproj-3.5.0-cp310-cp310-manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:5674923351e76222e2c10c58b5e1ac119d7a46b270d822c463035971b06f724b"},
+    {url = "https://files.pythonhosted.org/packages/99/d7/de65c65e430f603a51d405ff681fd8ac8ba5d2a2702a1eb896b8482f4f40/pyproj-3.5.0-pp39-pypy39_pp73-manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:e08db25b61cf024648d55973cc3d1c3f1d0818fabf594d5f5a8e2318103d2aa0"},
+    {url = "https://files.pythonhosted.org/packages/9a/49/dc0b35684ef1e4a95b11e38be29baa3a298be74fb2149eae3c2b3ed55d1d/pyproj-3.5.0-cp39-cp39-macosx_10_9_x86_64.whl", hash = "sha256:052c49fce8b5d55943a35c36ccecb87350c68b48ba95bc02a789770c374ef819"},
+    {url = "https://files.pythonhosted.org/packages/9c/0c/7e5d4d965fb9eebda44084737b113847134815208f21b967f3a2879f1427/pyproj-3.5.0-cp39-cp39-win32.whl", hash = "sha256:5c4b85ac10d733c42d73a2e6261c8d6745bf52433a31848dd1b6561c9a382da3"},
+    {url = "https://files.pythonhosted.org/packages/9c/f5/cd9371194d3c939dffddff9e118a018bb7c2f560549bea4c6bc21b24eadd/pyproj-3.5.0.tar.gz", hash = "sha256:9859d1591c1863414d875ae0759e72c2cffc01ab989dc64137fbac572cc81bf6"},
+    {url = "https://files.pythonhosted.org/packages/b8/ab/92a809e5bfe8bb00a7288426de5b1de7bbfd337fce09069cd7caffca1a3d/pyproj-3.5.0-pp38-pypy38_pp73-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:73f7960a97225812f9b1d7aeda5fb83812f38de9441e3476fcc8abb3e2b2f4de"},
+    {url = "https://files.pythonhosted.org/packages/cc/2d/05a84266790936fc9f65731a1a49f0fd6e4e7c994a2c56948aad5583e5ae/pyproj-3.5.0-cp38-cp38-win_amd64.whl", hash = "sha256:97ed199033c2c770e7eea2ef80ff5e6413426ec2d7ec985b869792f04ab95d05"},
+    {url = "https://files.pythonhosted.org/packages/d1/af/fb75eb28ef9a5cddbd0c6352c3defc44235f8afe7feddeb06f8ba17ef51b/pyproj-3.5.0-cp39-cp39-win_amd64.whl", hash = "sha256:1798ff7d65d9057ebb2d017ffe8403268b8452f24d0428b2140018c25c7fa1bc"},
+    {url = "https://files.pythonhosted.org/packages/d3/89/0bf944d2e50500eaceab030454af748bf0fdb90a00b1fcdca3e1464850e4/pyproj-3.5.0-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:6475ce653880938468a1a1b7321267243909e34b972ba9e53d5982c41d555918"},
+    {url = "https://files.pythonhosted.org/packages/da/01/b69528f2137e35665bf0fa60bb4ead2d06e35ca13e8683ca2b192c0306eb/pyproj-3.5.0-cp310-cp310-win_amd64.whl", hash = "sha256:f7c2f4d9681e810cf40239caaca00079930a6d9ee6591139b88d592d36051d82"},
+    {url = "https://files.pythonhosted.org/packages/e0/07/fbc65db1c4c9b387b0c8bf9ed4d26d6544026c40ebe930e645bb22f20ee1/pyproj-3.5.0-cp311-cp311-win_amd64.whl", hash = "sha256:e97573de0ab3bbbcb4c7748bc41f4ceb6da10b45d35b1a294b5820701e7c25f0"},
+    {url = "https://files.pythonhosted.org/packages/e1/63/07781eb5463b1aeb255962ad5106a1ccce986aee804d2ac5f8d61796a03b/pyproj-3.5.0-cp39-cp39-macosx_11_0_arm64.whl", hash = "sha256:1507138ea28bf2134d31797675380791cc1a7156a3aeda484e65a78a4aba9b62"},
+    {url = "https://files.pythonhosted.org/packages/e6/ca/cb70a26fcc6d760be897331d9a7c3c3916b31d20074070401a22d7c90db9/pyproj-3.5.0-cp39-cp39-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:c02742ef3d846401861a878a61ef7ad911ea7539d6cc4619ddb52dbdf7b45aee"},
+    {url = "https://files.pythonhosted.org/packages/e9/41/dd2cc950ce31f27983e8eb8ce5d371e367d5a7ccb53f2fbc3c7cead273fb/pyproj-3.5.0-pp39-pypy39_pp73-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:6a87b419a2a352413fbf759ecb66da9da50bd19861c8f26db6a25439125b27b9"},
+    {url = "https://files.pythonhosted.org/packages/f9/77/930b8168355d3ffb483e9fc7974621ff6a54767fc26cb6927741e99b50a1/pyproj-3.5.0-cp311-cp311-win32.whl", hash = "sha256:a730f5b4c98c8a0f312437873e6e34dbd4cc6dc23d5afd91a6691c62724b1f68"},
+    {url = "https://files.pythonhosted.org/packages/fa/5b/0637f05785e5f6e11c875dd22ab6bdb59e276f2418fbf64c8471fe189be3/pyproj-3.5.0-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:8fe6bb1b68a35d07378d38be77b5b2f8dd2bea5910c957bfcc7bee55988d3910"},
+    {url = "https://files.pythonhosted.org/packages/fc/90/ae0b79da1bea66ac85d6ff0c433214a1f6e028e64b9fd17d26038954cef8/pyproj-3.5.0-cp38-cp38-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:b752b7d9c4b08181c7e8c0d9c7f277cbefff42227f34d3310696a87c863d9dd3"},
+]
 "pysrt 1.1.2" = [
     {url = "https://files.pythonhosted.org/packages/31/1a/0d858da1c6622dcf16011235a2639b0a01a49cecf812f8ab03308ab4de37/pysrt-1.1.2.tar.gz", hash = "sha256:b4f844ba33e4e7743e9db746492f3a193dc0bc112b153914698e7c1cdeb9b0b9"},
 ]
 "pysubs2 1.6.1" = [
     {url = "https://files.pythonhosted.org/packages/22/3e/fb1b08a06144ba63f19cc4758dd72e2eb8c7fc95c6c8364faccfc570c7bf/pysubs2-1.6.1.tar.gz", hash = "sha256:0261611e71735ff7763972c519c72593c8063efcb9039c54af65f31b81cec116"},
     {url = "https://files.pythonhosted.org/packages/4f/dc/dc1763a3abab92af2253b1abb3dd48e07b2a3613d7ae64a3ab5c27da3019/pysubs2-1.6.1-py3-none-any.whl", hash = "sha256:1f96d9dfb5f859a54a00e04621beb20ff21ea1d788821b2f4935c5c0ef8dc68e"},
 ]
-"pytest 7.3.2" = [
-    {url = "https://files.pythonhosted.org/packages/58/2a/07c65fdc40846ecb8a9dcda2c38fcb5a06a3e39d08d4a4960916431951cb/pytest-7.3.2.tar.gz", hash = "sha256:ee990a3cc55ba808b80795a79944756f315c67c12b56abd3ac993a7b8c17030b"},
-    {url = "https://files.pythonhosted.org/packages/7a/d0/de969198293cdea22b3a6fb99a99aeeddb7b3827f0823b33c5dc0734bbe5/pytest-7.3.2-py3-none-any.whl", hash = "sha256:cdcbd012c9312258922f8cd3f1b62a6580fdced17db6014896053d47cddf9295"},
+"pytest 7.4.0" = [
+    {url = "https://files.pythonhosted.org/packages/33/b2/741130cbcf2bbfa852ed95a60dc311c9e232c7ed25bac3d9b8880a8df4ae/pytest-7.4.0-py3-none-any.whl", hash = "sha256:78bf16451a2eb8c7a2ea98e32dc119fd2aa758f1d5d66dbf0a59d69a3969df32"},
+    {url = "https://files.pythonhosted.org/packages/a7/f3/dadfbdbf6b6c8b5bd02adb1e08bc9fbb45ba51c68b0893fa536378cdf485/pytest-7.4.0.tar.gz", hash = "sha256:b4bf8c45bd59934ed84001ad51e11b4ee40d40a1229d2c79f9c592b0a3f6bd8a"},
 ]
 "python-dateutil 2.8.2" = [
     {url = "https://files.pythonhosted.org/packages/36/7a/87837f39d0296e723bb9b62bbb257d0355c7f6128853c78955f57342a56d/python_dateutil-2.8.2-py2.py3-none-any.whl", hash = "sha256:961d03dc3453ebbc59dbdea9e4e11c5651520a876d0f4db161e8674aae935da9"},
     {url = "https://files.pythonhosted.org/packages/4c/c4/13b4776ea2d76c115c1d1b84579f3764ee6d57204f6be27119f13a61d0a9/python-dateutil-2.8.2.tar.gz", hash = "sha256:0123cacc1627ae19ddf3c27a5de5bd67ee4586fbdd6440d9748f8abb483d3e86"},
 ]
 "python-mpv-jsonipc 1.2.0" = [
     {url = "https://files.pythonhosted.org/packages/6f/65/232563752a049831fdd6ae7b4caf8a557529d2f3c72ecbc40fb8b69e372c/python-mpv-jsonipc-1.2.0.tar.gz", hash = "sha256:2199beefa6643d16483dda17c976bf2bbbf5dfedb1a5ca8d7d4611527ae6ad7a"},
@@ -2900,32 +3066,32 @@
     {url = "https://files.pythonhosted.org/packages/45/1e/0c169c6a5381e241ba7404532c16a21d86ab872c9bed8bdcd4c423954103/requests-2.24.0-py2.py3-none-any.whl", hash = "sha256:fe75cc94a9443b9246fc7049224f75604b113c36acb93f87b80ed42c44cbb898"},
     {url = "https://files.pythonhosted.org/packages/da/67/672b422d9daf07365259958912ba533a0ecab839d4084c487a5fe9a5405f/requests-2.24.0.tar.gz", hash = "sha256:b3559a131db72c33ee969480840fff4bb6dd111de7dd27c8ee1f820f4f00231b"},
 ]
 "rich 13.4.2" = [
     {url = "https://files.pythonhosted.org/packages/e3/12/67d0098eb77005f5e068de639e6f4cfb8f24e6fcb0fd2037df0e1d538fee/rich-13.4.2.tar.gz", hash = "sha256:d653d6bccede5844304c605d5aac802c7cf9621efd700b46c7ec2b51ea914898"},
     {url = "https://files.pythonhosted.org/packages/fc/1e/482e5eec0b89b593e81d78f819a9412849814e22225842b598908e7ac560/rich-13.4.2-py3-none-any.whl", hash = "sha256:8f87bc7ee54675732fa66a05ebfe489e27264caeeff3728c945d25971b6485ec"},
 ]
-"ruff 0.0.274" = [
-    {url = "https://files.pythonhosted.org/packages/07/59/7b043efe280a7f6815c87fda4bf1e43e51c87b181f3b461bd761e29377f7/ruff-0.0.274-py3-none-macosx_10_9_x86_64.macosx_11_0_arm64.macosx_10_9_universal2.whl", hash = "sha256:fa9ad8776cb92f2739b8eee316cde841d6012d0eafbf06bae09166203ddf9bb8"},
-    {url = "https://files.pythonhosted.org/packages/18/26/3ee1c9717fa206318be9eb892b8326ac415f1a57952aa996fd7b88435126/ruff-0.0.274-py3-none-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:044084f039a679e557240fefcf521e057941b163014cf969ac6d04620861e04a"},
-    {url = "https://files.pythonhosted.org/packages/30/ad/9dc28c29b8fbb390f2f08c5e2e961c9b2adf2d71549f78ac4f310f392b30/ruff-0.0.274-py3-none-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:dca36d651f88b4b24f17df5db54487057ce0ccd3599cbf38d237cf4d9f0d63c2"},
-    {url = "https://files.pythonhosted.org/packages/36/a2/7b226d7586607e3991646961b29a15d1f923fa8459f0015114c80394e82c/ruff-0.0.274-py3-none-manylinux_2_17_armv7l.manylinux2014_armv7l.whl", hash = "sha256:023cdc5e64b3f34244e12bd236ab412c6056061a2415d50fb862cab333b4ab7c"},
-    {url = "https://files.pythonhosted.org/packages/39/24/e60dfe0b610a13a716bb4fb574c6e4365c7404a16d8352b27edf6d6b1ee9/ruff-0.0.274-py3-none-macosx_10_7_x86_64.whl", hash = "sha256:6d7069157a5674be8090c7d89fa69dbb2478f333a80b1312d20ade2a870cca3e"},
-    {url = "https://files.pythonhosted.org/packages/73/31/3cc256943d29025793279244fd6837240382edd3c585f3b562a62b66deb6/ruff-0.0.274.tar.gz", hash = "sha256:c7e5f9deffbd02d8054f90b565a1106faee64e16cedf50f3aa05c14b59ff8727"},
-    {url = "https://files.pythonhosted.org/packages/7b/d1/029f18d1ad0456c01e23ec40c99c817be7593ce345711ec02683ff8092bf/ruff-0.0.274-py3-none-musllinux_1_2_armv7l.whl", hash = "sha256:86d943107f20fec924f56dc4933cefb0efbc1ec8b729e0a1afabac598c5586ca"},
-    {url = "https://files.pythonhosted.org/packages/7f/60/f8d4966112555805366ec2df37e3653d4d80adbc1b00bf4254dbbd9e340d/ruff-0.0.274-py3-none-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:587130943110e9536018ce139158e2962d46623f379a4486aabfd525e9714b0e"},
-    {url = "https://files.pythonhosted.org/packages/84/7c/21841a330cd8e162ccc848d99e84a3cb27416cd7eb983cc17b082a6469ec/ruff-0.0.274-py3-none-musllinux_1_2_i686.whl", hash = "sha256:b13e765b64487143f05e6ad6f624388b9ac5a6ff8657ff801091c9282de3ca52"},
-    {url = "https://files.pythonhosted.org/packages/b5/da/694e37da2604444f0c5a4dc5eb5cf23af02622d9b4638dc343997a84d3fd/ruff-0.0.274-py3-none-manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:34e71a06a4e27554ca2f1c2b1749a802e3e76cac41481cfc2cb86936c1e37d3c"},
-    {url = "https://files.pythonhosted.org/packages/b9/4b/25f1f00393db9a4d018039b7a39fca5164c6cb5b251caba7abd8ccd8f957/ruff-0.0.274-py3-none-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:6133fa856b230a0281197aeba3e89ce9595f9d8a7265113520ad259d416c9f4b"},
-    {url = "https://files.pythonhosted.org/packages/b9/d9/2dd3f535a211a73754c764212a52d7db70e9d55f9263a963b9b95e779dfe/ruff-0.0.274-py3-none-musllinux_1_2_x86_64.whl", hash = "sha256:461bda8c3a4c1591fd7a09960b86e2ffc9a59a1c42cf14d725077314c12b60b0"},
-    {url = "https://files.pythonhosted.org/packages/bd/7d/57ccbca1428cd4876bf68decfc465b2725ce5234da91fb4c4910443de0f5/ruff-0.0.274-py3-none-manylinux_2_17_ppc64.manylinux2014_ppc64.whl", hash = "sha256:5137f853fffa7352901038a1b5e36a97058380a554763e534aae9f6c0734fdab"},
-    {url = "https://files.pythonhosted.org/packages/c6/ec/fdd733bddd74cee9293cf235505f7e865d435306e24543ca590910f1260c/ruff-0.0.274-py3-none-win_amd64.whl", hash = "sha256:e80aa0c7e1347a96db846287695971925eb56760c019a7d66312fbca389a6800"},
-    {url = "https://files.pythonhosted.org/packages/cf/0b/bf76ae7566952fb0675537ea8730a567c416ba35cd23c95e70b3ea07139f/ruff-0.0.274-py3-none-win_arm64.whl", hash = "sha256:8b99ce776fc60fb938791f558b297e53ed634adeef1a7b84a33455924948c9af"},
-    {url = "https://files.pythonhosted.org/packages/e1/95/1debc53b970c97a991f15c01e6650e76b7e35c8cd4945b0a9a33ec2c53cc/ruff-0.0.274-py3-none-musllinux_1_2_aarch64.whl", hash = "sha256:39b80156ef57b33ab7bfc454b7c2678eaae07f43a7dcf2e7c058f72d87b49538"},
-    {url = "https://files.pythonhosted.org/packages/e6/4a/c09cde430f6aa48e98f0384d49e9612e4f22e2429f745e3e9eca30075f53/ruff-0.0.274-py3-none-win32.whl", hash = "sha256:09c87fa2c4f53bd63c1d8a35150683794b022f4f2fbd6ef2fe383ce21ab53fec"},
+"ruff 0.0.275" = [
+    {url = "https://files.pythonhosted.org/packages/04/27/41dc218102670ea7849dadf3bb0e7861105caac2e498171e1890dbfbf7b7/ruff-0.0.275-py3-none-musllinux_1_2_aarch64.whl", hash = "sha256:c8ace4d40a57b5ea3c16555f25a6b16bc5d8b2779ae1912ce2633543d4e9b1da"},
+    {url = "https://files.pythonhosted.org/packages/0e/ae/9960d8cc311eafb6e0d7ac7b775ee739d1f1361d3e5fea1ba49e61e7e424/ruff-0.0.275-py3-none-macosx_10_7_x86_64.whl", hash = "sha256:5e6554a072e7ce81eb6f0bec1cebd3dcb0e358652c0f4900d7d630d61691e914"},
+    {url = "https://files.pythonhosted.org/packages/21/cf/1b0a4d7f7700c6195f4a54406eb98b7a2f6b56c66a6f9ceeb5da345390bb/ruff-0.0.275-py3-none-musllinux_1_2_armv7l.whl", hash = "sha256:8347fc16aa185aae275906c4ac5b770e00c896b6a0acd5ba521f158801911998"},
+    {url = "https://files.pythonhosted.org/packages/2a/e3/d50caf74e65fbf46ff446929c17fb4d9da3c747817548af81a858f29edca/ruff-0.0.275.tar.gz", hash = "sha256:a63a0b645da699ae5c758fce19188e901b3033ec54d862d93fcd042addf7f38d"},
+    {url = "https://files.pythonhosted.org/packages/2b/9b/3ca65497a21371c276898a0e2e26c2fd1673bf59476bb1c9bea23983ff6b/ruff-0.0.275-py3-none-musllinux_1_2_i686.whl", hash = "sha256:ec43658c64bfda44fd84bbea9da8c7a3b34f65448192d1c4dd63e9f4e7abfdd4"},
+    {url = "https://files.pythonhosted.org/packages/36/12/825b1cdbe5044b4ab92e5e25f60650a7bc726a8acc5df1a3d13b9c443d8c/ruff-0.0.275-py3-none-manylinux_2_17_ppc64.manylinux2014_ppc64.whl", hash = "sha256:22efd9f41af27ef8fb9779462c46c35c89134d33e326c889971e10b2eaf50c63"},
+    {url = "https://files.pythonhosted.org/packages/38/88/fb7fe795721d7af456789db6d2a4eb53b70d59213c3df1cfbafd265199a7/ruff-0.0.275-py3-none-manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:0dbdea02942131dbc15dd45f431d152224f15e1dd1859fcd0c0487b658f60f1a"},
+    {url = "https://files.pythonhosted.org/packages/3c/7d/ce7293a3354d19a438cda962f88025a08bed108d3692b1a9631e035e46c4/ruff-0.0.275-py3-none-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:80043726662144876a381efaab88841c88e8df8baa69559f96b22d4fa216bef1"},
+    {url = "https://files.pythonhosted.org/packages/3d/d6/34859533f225fe0a312d7565782c52773f0ac4d721c3519abde2c9250b8d/ruff-0.0.275-py3-none-macosx_10_9_x86_64.macosx_11_0_arm64.macosx_10_9_universal2.whl", hash = "sha256:1cc599022fe5ffb143a965b8d659eb64161ab8ab4433d208777eab018a1aab67"},
+    {url = "https://files.pythonhosted.org/packages/43/f1/bf25f0b5f426b25006241985d0c407a156f3e56d876a2eed1be076107c21/ruff-0.0.275-py3-none-manylinux_2_17_armv7l.manylinux2014_armv7l.whl", hash = "sha256:0c4e6468da26f77b90cae35319d310999f471a8c352998e9b39937a23750149e"},
+    {url = "https://files.pythonhosted.org/packages/55/cb/aa2ca6cd503b5bb179e6d5f0e8d567fea63e09468c249ef42e8ffb1ecb40/ruff-0.0.275-py3-none-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:2c09662112cfa22d7467a19252a546291fd0eae4f423e52b75a7a2000a1894db"},
+    {url = "https://files.pythonhosted.org/packages/87/30/369db86b101f917ef32e5fedc2a3528ddfd9c258a903a072960e3a00c261/ruff-0.0.275-py3-none-win32.whl", hash = "sha256:6afb1c4422f24f361e877937e2a44b3f8176774a476f5e33845ebfe887dd5ec2"},
+    {url = "https://files.pythonhosted.org/packages/af/fb/2c9d1af4e54d77a9b510ec48fd13f0c40cc7c3b43d7ca261e0a2ac4c0b91/ruff-0.0.275-py3-none-win_arm64.whl", hash = "sha256:a19ce3bea71023eee5f0f089dde4a4272d088d5ac0b675867e074983238ccc65"},
+    {url = "https://files.pythonhosted.org/packages/cf/6e/6d5af3c16541ad4342d81e3e38eecb0593aa9da314686144796d2c0a1a48/ruff-0.0.275-py3-none-win_amd64.whl", hash = "sha256:d9b264d78621bf7b698b6755d4913ab52c19bd28bee1a16001f954d64c1a1220"},
+    {url = "https://files.pythonhosted.org/packages/d7/33/68753ff8b0981edd0978daaf0bff874b8c369e26bf2da06512a17ab9a581/ruff-0.0.275-py3-none-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:5206fc1cd8c1c1deadd2e6360c0dbcd690f1c845da588ca9d32e4a764a402c60"},
+    {url = "https://files.pythonhosted.org/packages/e4/77/f81ec6f3100f6d14638194e877a8928faa70a60b1d176f557642ee2c410d/ruff-0.0.275-py3-none-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:5859ee543b01b7eb67835dfd505faa8bb7cc1550f0295c92c1401b45b42be399"},
+    {url = "https://files.pythonhosted.org/packages/f5/f6/26955e33a3aad236b7e2774c13be1fe505f31bfc6071254fe0d22044cf26/ruff-0.0.275-py3-none-musllinux_1_2_x86_64.whl", hash = "sha256:508b13f7ca37274cceaba4fb3ea5da6ca192356323d92acf39462337c33ad14e"},
 ]
 "scalene 1.5.19" = [
     {url = "https://files.pythonhosted.org/packages/11/19/c973ecc43b18076df6c7efff7bec280d02d48d8245f46d94b7e90cf306f2/scalene-1.5.19-cp39-cp39-win_amd64.whl", hash = "sha256:d1fd5d83f3c022ddc46049f29823351b8dbdb8590f5803358fa6034784601f24"},
     {url = "https://files.pythonhosted.org/packages/19/54/d89426ab970f1cb3850b0374967ae22d831d0091efeb2c1d8e8d02ac2a19/scalene-1.5.19-cp39-cp39-macosx_11_7_universal2.whl", hash = "sha256:6c08f3bc0b6355db3c34f0e9aea1b291e64675bb832e19758ee751918787cac0"},
     {url = "https://files.pythonhosted.org/packages/49/11/5a2fa4567eee217609e0a627534f5fb60d0c1f768b43a93145a2ea24e39b/scalene-1.5.19-cp38-cp38-manylinux_2_24_x86_64.whl", hash = "sha256:f67f39321548c06de440319bdd70c41c14b6c50d4748226a101402995677cade"},
     {url = "https://files.pythonhosted.org/packages/5e/3c/b1f159a11f0949f3f27b18af1cc68ee301088a7337efc7d961684bdd3f46/scalene-1.5.19-cp37-cp37m-macosx_10_15_universal2.whl", hash = "sha256:58fb40d031081a55e813f292b2d85b64d7558a372832d8e456f7fe2113adf182"},
     {url = "https://files.pythonhosted.org/packages/65/c3/ebaf00eef807b8da6c5b0c4eb6627f0a67538a25ac7e3858347e15c55d22/scalene-1.5.19-cp38-cp38-win_amd64.whl", hash = "sha256:7a1d452ad4d32cf8adb8b86cae4e5b9c7bff866fff1c43618f9ad114b9ecac32"},
@@ -2936,29 +3102,112 @@
     {url = "https://files.pythonhosted.org/packages/91/09/947aa7fac9de4cd6d866eddd3711be8a4a2ae273a6467e3aa764c476c121/scalene-1.5.19-cp311-cp311-win_amd64.whl", hash = "sha256:eeef31408df35972e54a39ae2d2f1aeab111f2d53d0a78061e45dcf024c6e01d"},
     {url = "https://files.pythonhosted.org/packages/a4/6b/dce5e2d258b10208b7b0590d4ffdf01e19a72d743f0e5f237fcf86550006/scalene-1.5.19-cp311-cp311-manylinux_2_24_x86_64.whl", hash = "sha256:2dac52555518c7159d2fd9c8c7c31ffa8b6a74f21d1b40a9d315a77f4a7f97ed"},
     {url = "https://files.pythonhosted.org/packages/b7/55/69071e44208c77dccb9b57929e9ddcd507c52e58980b1d6257915bb1d213/scalene-1.5.19-cp310-cp310-manylinux_2_24_x86_64.whl", hash = "sha256:1da57151f00c70446309c9b52843ce7b437bbf32d336a7c309d4fe0b8deda2a2"},
     {url = "https://files.pythonhosted.org/packages/d3/c3/caf694aa795e45bb0fbaa17fdc945a36f36a9ef9291e536cab22418f354a/scalene-1.5.19-cp38-cp38-macosx_10_15_universal2.whl", hash = "sha256:0997b1f1ec90e079a73349d702b18df60e6b24c31c255d3e8d6ec6a8b03493c8"},
     {url = "https://files.pythonhosted.org/packages/f1/95/dae88019fcff89cc1cc3b6fc85b9fc3a25a264b21b67000a665dd3ae372a/scalene-1.5.19-cp310-cp310-win_amd64.whl", hash = "sha256:cdb9be734cfb6b42eef1105fee1876a5c465eb72e109c0d0ceea6e6bdbce21c6"},
     {url = "https://files.pythonhosted.org/packages/fb/08/ed0d55f81bc2bc261c922a2d4171360b1a3a5d6a4e57ccc640fb09a02706/scalene-1.5.19-cp39-cp39-manylinux_2_24_x86_64.whl", hash = "sha256:d8bc53334b13e486ed6ba03fe4b7595ad4038d05537793eed9999952ba1b34c6"},
 ]
+"scikit-learn 1.2.2" = [
+    {url = "https://files.pythonhosted.org/packages/17/13/d4142c9105507ba363d9f3602941b7baf79763cc17e73fa9be826ba3aa89/scikit_learn-1.2.2-cp38-cp38-macosx_10_9_x86_64.whl", hash = "sha256:9c710ff9f9936ba8a3b74a455ccf0dcf59b230caa1e9ba0223773c490cab1e51"},
+    {url = "https://files.pythonhosted.org/packages/27/4a/1afe473760b07663710a75437b795ef37362aebb8bf513ff3bbf78fbd0c6/scikit_learn-1.2.2-cp311-cp311-macosx_10_9_x86_64.whl", hash = "sha256:dfeaf8be72117eb61a164ea6fc8afb6dfe08c6f90365bde2dc16456e4bc8e45f"},
+    {url = "https://files.pythonhosted.org/packages/2f/fd/9fcbe7fe94150e72d87120cbc462bde1971c3674e726b81f4a4c4fdfa8e1/scikit_learn-1.2.2-cp311-cp311-macosx_12_0_arm64.whl", hash = "sha256:fe0aa1a7029ed3e1dcbf4a5bc675aa3b1bc468d9012ecf6c6f081251ca47f590"},
+    {url = "https://files.pythonhosted.org/packages/39/85/95298f12ec1ed756938edafe9f15498109ec8dbfc833ae492ae1cc333933/scikit_learn-1.2.2-cp39-cp39-macosx_12_0_arm64.whl", hash = "sha256:fe175ee1dab589d2e1033657c5b6bec92a8a3b69103e3dd361b58014729975c3"},
+    {url = "https://files.pythonhosted.org/packages/3a/9c/7e26446b45192186c63bf6e9fc50a4834b8c9d85a719e06d60a244ded6f3/scikit_learn-1.2.2-cp38-cp38-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:44b47a305190c28dd8dd73fc9445f802b6ea716669cfc22ab1eb97b335d238b1"},
+    {url = "https://files.pythonhosted.org/packages/3c/21/ee21352f69a980614cb4193d68a64a83aa2c0f80183c9485d6d61821a922/scikit_learn-1.2.2-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:99cc01184e347de485bf253d19fcb3b1a3fb0ee4cea5ee3c43ec0cc429b6d29f"},
+    {url = "https://files.pythonhosted.org/packages/48/92/a39d1c9e0a6cb5ed4112899ecca590138484356ba8c4274dde6c3893ff14/scikit_learn-1.2.2-cp310-cp310-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:6fe83b676f407f00afa388dd1fdd49e5c6612e551ed84f3b1b182858f09e987d"},
+    {url = "https://files.pythonhosted.org/packages/4c/64/a1e6e92b850b39200c82e3bc54d556b2c634b3904c39ac5cdb10b1c5765f/scikit_learn-1.2.2-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:bf036ea7ef66115e0d49655f16febfa547886deba20149555a41d28f56fd6d3c"},
+    {url = "https://files.pythonhosted.org/packages/4f/6b/a204ee49e2d4dec62b38394adbdc7672e9a9df9f359a80705a07a46cace6/scikit_learn-1.2.2-cp39-cp39-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:7d5312d9674bed14f73773d2acf15a3272639b981e60b72c9b190a0cffed5bad"},
+    {url = "https://files.pythonhosted.org/packages/51/b6/d9a414b6579c4ec5703cebc0fe7b7b6821344190bffa3d46a1a23efd173a/scikit_learn-1.2.2-cp39-cp39-win_amd64.whl", hash = "sha256:6477eed40dbce190f9f9e9d0d37e020815825b300121307942ec2110302b66a3"},
+    {url = "https://files.pythonhosted.org/packages/51/d1/58faa69e97ee60e99dcdde5df43f17f0887eda5de9eafb6534a51b63d791/scikit_learn-1.2.2-cp38-cp38-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:953236889928d104c2ef14027539f5f2609a47ebf716b8cbe4437e85dce42744"},
+    {url = "https://files.pythonhosted.org/packages/5a/43/5c4d21217df6a033999ee531fdfd52809263727b4afb26f7196a8ec709ae/scikit_learn-1.2.2-cp310-cp310-macosx_12_0_arm64.whl", hash = "sha256:e6e574db9914afcb4e11ade84fab084536a895ca60aadea3041e85b8ac963edb"},
+    {url = "https://files.pythonhosted.org/packages/5b/fb/478a0460ae2843dd2fc7a7f9ddcd8bb033ae21eb968df6a8cbe8094a28bc/scikit_learn-1.2.2-cp38-cp38-win_amd64.whl", hash = "sha256:7f69313884e8eb311460cc2f28676d5e400bd929841a2c8eb8742ae78ebf7c20"},
+    {url = "https://files.pythonhosted.org/packages/72/aa/a97b6ae8fc4ce0e1b3837b3613b0563ce843eb34cf4089fb41d613dee957/scikit_learn-1.2.2-cp39-cp39-macosx_10_9_x86_64.whl", hash = "sha256:8156db41e1c39c69aa2d8599ab7577af53e9e5e7a57b0504e116cc73c39138dd"},
+    {url = "https://files.pythonhosted.org/packages/81/84/756be2b975959a5f94124d5584ead75d7ca99184f2d16664a0157b274b9a/scikit_learn-1.2.2-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:ea061bf0283bf9a9f36ea3c5d3231ba2176221bbd430abd2603b1c3b2ed85c89"},
+    {url = "https://files.pythonhosted.org/packages/ae/a8/829ef05dbeb9aa4436190ea00c8db6d59a39751b45e17932221d27fe9e51/scikit_learn-1.2.2-cp38-cp38-macosx_12_0_arm64.whl", hash = "sha256:2dd3ffd3950e3d6c0c0ef9033a9b9b32d910c61bd06cb8206303fb4514b88a49"},
+    {url = "https://files.pythonhosted.org/packages/c9/fa/8e158d81e3602da1e7bafbd4987938bc003fe4b0f44d65681e7f8face95a/scikit-learn-1.2.2.tar.gz", hash = "sha256:8429aea30ec24e7a8c7ed8a3fa6213adf3814a6efbea09e16e0a0c71e1a1a3d7"},
+    {url = "https://files.pythonhosted.org/packages/d7/8a/301594a8bb1cfeeb95dd86aa7dfedd31e93211940105429abddf0933cfff/scikit_learn-1.2.2-cp311-cp311-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:065e9673e24e0dc5113e2dd2b4ca30c9d8aa2fa90f4c0597241c93b63130d233"},
+    {url = "https://files.pythonhosted.org/packages/db/98/169b46a84b48f92df2b5e163fce75d471f4df933f8b3d925a61133210776/scikit_learn-1.2.2-cp311-cp311-win_amd64.whl", hash = "sha256:8b0670d4224a3c2d596fd572fb4fa673b2a0ccfb07152688ebd2ea0b8c61025c"},
+    {url = "https://files.pythonhosted.org/packages/f4/4d/fe3b35e18407da4b386be58616bd0f941ea1762a6c6798267f3aa64ef5d5/scikit_learn-1.2.2-cp310-cp310-win_amd64.whl", hash = "sha256:ad66c3848c0a1ec13464b2a95d0a484fd5b02ce74268eaa7e0c697b904f31d6c"},
+    {url = "https://files.pythonhosted.org/packages/fa/1e/36d7609e84b50d4a2e5bc43cd5013d9ea885799e5813a1e9cf5bb1afd3f4/scikit_learn-1.2.2-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:2e2642baa0ad1e8f8188917423dd73994bf25429f8893ddbe115be3ca3183584"},
+]
+"scipy 1.9.3" = [
+    {url = "https://files.pythonhosted.org/packages/0a/2e/44795c6398e24e45fa0bb61c3e98de1cfea567b1b51efd3751e2f7ff9720/scipy-1.9.3.tar.gz", hash = "sha256:fbc5c05c85c1a02be77b1ff591087c83bc44579c6d2bd9fb798bb64ea5e1a027"},
+    {url = "https://files.pythonhosted.org/packages/40/0e/3ff193b6ba6a0a6f13f8d367e8976370232e769bd609c8c11d86e0353adf/scipy-1.9.3-cp310-cp310-macosx_12_0_arm64.whl", hash = "sha256:83b89e9586c62e787f5012e8475fbb12185bafb996a03257e9675cd73d3736dd"},
+    {url = "https://files.pythonhosted.org/packages/42/14/d2500818b7bb7b862d70c1ae97e646a4795b068583c67720553764095024/scipy-1.9.3-cp38-cp38-win_amd64.whl", hash = "sha256:2318bef588acc7a574f5bfdff9c172d0b1bf2c8143d9582e05f878e580a3781e"},
+    {url = "https://files.pythonhosted.org/packages/42/81/0a64d2204c3b261380ac96c6d61f018528108b62c0e21e6153a58cebf4f6/scipy-1.9.3-cp311-cp311-win_amd64.whl", hash = "sha256:06d2e1b4c491dc7d8eacea139a1b0b295f74e1a1a0f704c375028f8320d16e31"},
+    {url = "https://files.pythonhosted.org/packages/44/8a/bae77e624391b27aeea2d33a02f2ce4a8019f1378ce92faf5780f1521f2e/scipy-1.9.3-cp38-cp38-macosx_12_0_arm64.whl", hash = "sha256:545c83ffb518094d8c9d83cce216c0c32f8c04aaf28b92cc8283eda0685162d5"},
+    {url = "https://files.pythonhosted.org/packages/56/af/6a2b90fe280e89466d84747054667f74b84a8304f75931a173090919991f/scipy-1.9.3-cp38-cp38-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:cff3a5295234037e39500d35316a4c5794739433528310e117b8a9a0c76d20fc"},
+    {url = "https://files.pythonhosted.org/packages/59/0b/8a9acfc5c36bbf6e18d02f3a08db5b83bebba510be2df3230f53852c74a4/scipy-1.9.3-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:d01e1dd7b15bd2449c8bfc6b7cc67d630700ed655654f0dfcf121600bad205c9"},
+    {url = "https://files.pythonhosted.org/packages/59/ef/d54d17c36b46a9b8f6e1d4bf039b7f7ad236504cfb13cf1872caec9cbeaa/scipy-1.9.3-cp39-cp39-macosx_10_9_x86_64.whl", hash = "sha256:d644a64e174c16cb4b2e41dfea6af722053e83d066da7343f333a54dae9bc31c"},
+    {url = "https://files.pythonhosted.org/packages/84/86/4f38fa30c112c3590954420f85d95b8cd23811ecc5cfc4bfd4d988d4db44/scipy-1.9.3-cp38-cp38-macosx_10_9_x86_64.whl", hash = "sha256:5a04cd7d0d3eff6ea4719371cbc44df31411862b9646db617c99718ff68d4840"},
+    {url = "https://files.pythonhosted.org/packages/92/f9/7ae2c1ae200212bc84b5a8369a10d644aa8b588140fe292d59db3b4a2545/scipy-1.9.3-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:abaf921531b5aeaafced90157db505e10345e45038c39e5d9b6c7922d68085cb"},
+    {url = "https://files.pythonhosted.org/packages/b5/67/c5451465ec94e654e6315cd5136961d267ae94a0f799b85d26eb9efe4c9f/scipy-1.9.3-cp39-cp39-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:4db5b30849606a95dcf519763dd3ab6fe9bd91df49eba517359e450a7d80ce2e"},
+    {url = "https://files.pythonhosted.org/packages/bb/b7/380c9e4cd71263f03d16f8a92c0e44c9bdef38777e1a7dde1f47ba996bac/scipy-1.9.3-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:c68db6b290cbd4049012990d7fe71a2abd9ffbe82c0056ebe0f01df8be5436b0"},
+    {url = "https://files.pythonhosted.org/packages/c3/3e/e40c52775a5d19abd43b1c245fbc5dee283a29acc45c830bc73bfad9468b/scipy-1.9.3-cp311-cp311-macosx_12_0_arm64.whl", hash = "sha256:90453d2b93ea82a9f434e4e1cba043e779ff67b92f7a0e85d05d286a3625df3c"},
+    {url = "https://files.pythonhosted.org/packages/c8/0f/d9f8c50be8670b7ba6f002679e84cd18f46a23faf62c1590f4d1bbec0c8c/scipy-1.9.3-cp39-cp39-macosx_12_0_arm64.whl", hash = "sha256:da8245491d73ed0a994ed9c2e380fd058ce2fa8a18da204681f2fe1f57f98f95"},
+    {url = "https://files.pythonhosted.org/packages/ce/28/635391e72e24bd3f4a91e374f4a186a5e4ecc95f23d8a55c9b0d25777cf7/scipy-1.9.3-cp310-cp310-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:1a72d885fa44247f92743fc20732ae55564ff2a519e8302fb7e18717c5355a8b"},
+    {url = "https://files.pythonhosted.org/packages/cf/0e/3f1685c1fcb5dfe35ec027a5fc7a29e8818c61b2cc7fa207b4fc7b959f52/scipy-1.9.3-cp310-cp310-win_amd64.whl", hash = "sha256:68239b6aa6f9c593da8be1509a05cb7f9efe98b80f43a5861cd24c7557e98523"},
+    {url = "https://files.pythonhosted.org/packages/d0/96/4f6eac3fea18f836a0e403539556b1684e6f3361fa39aa5d5797dedecd75/scipy-1.9.3-cp39-cp39-win_amd64.whl", hash = "sha256:5b88e6d91ad9d59478fafe92a7c757d00c59e3bdc3331be8ada76a4f8d683f58"},
+    {url = "https://files.pythonhosted.org/packages/df/75/c0254dc58d1f1b00f9d3dbda029743b71b815dd512461ed20d9b7f459e37/scipy-1.9.3-cp311-cp311-macosx_10_9_x86_64.whl", hash = "sha256:b41bc822679ad1c9a5f023bc93f6d0543129ca0f37c1ce294dd9d386f0a21096"},
+    {url = "https://files.pythonhosted.org/packages/f4/9d/882134b1e774a9227ab855c71a39612194e1106185595417ce92f0f1e78c/scipy-1.9.3-cp38-cp38-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:0d54222d7a3ba6022fdf5773931b5d7c56efe41ede7f7128c7b1637700409108"},
+    {url = "https://files.pythonhosted.org/packages/f9/37/5cd44af74d7178a44452b17ea162bc93996d5555b4a978877d2efd56fe84/scipy-1.9.3-cp311-cp311-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:83c06e62a390a9167da60bedd4575a14c1f58ca9dfde59830fc42e5197283dab"},
+    {url = "https://files.pythonhosted.org/packages/fb/ba/1733dbbc19f2aa07d100cfa220bcc83a3977bc5c9f0a5ad262dae1f3ab90/scipy-1.9.3-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:1884b66a54887e21addf9c16fb588720a8309a57b2e258ae1c7986d4444d3bc0"},
+]
 "screeninfo 0.8.1" = [
     {url = "https://files.pythonhosted.org/packages/6e/bf/c5205d480307bef660e56544b9e3d7ff687da776abb30c9cb3f330887570/screeninfo-0.8.1-py3-none-any.whl", hash = "sha256:e97d6b173856edcfa3bd282f81deb528188aff14b11ec3e195584e7641be733c"},
     {url = "https://files.pythonhosted.org/packages/ec/bb/e69e5e628d43f118e0af4fc063c20058faa8635c95a1296764acc8167e27/screeninfo-0.8.1.tar.gz", hash = "sha256:9983076bcc7e34402a1a9e4d7dabf3729411fd2abb3f3b4be7eba73519cd2ed1"},
 ]
 "setuptools 68.0.0" = [
     {url = "https://files.pythonhosted.org/packages/c7/42/be1c7bbdd83e1bfb160c94b9cafd8e25efc7400346cf7ccdbdb452c467fa/setuptools-68.0.0-py3-none-any.whl", hash = "sha256:11e52c67415a381d10d6b462ced9cfb97066179f0e871399e006c4ab101fc85f"},
     {url = "https://files.pythonhosted.org/packages/dc/98/5f896af066c128669229ff1aa81553ac14cfb3e5e74b6b44594132b8540e/setuptools-68.0.0.tar.gz", hash = "sha256:baf1fdb41c6da4cd2eae722e135500da913332ab3f2f5c7d33af9b492acb5235"},
 ]
+"shapely 2.0.1" = [
+    {url = "https://files.pythonhosted.org/packages/04/67/05e96af1c4ee130e12ac228da1ab86f7581809d8f008aa3a9ec19ea22eb2/shapely-2.0.1-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:70a18fc7d6418e5aea76ac55dce33f98e75bd413c6eb39cfed6a1ba36469d7d4"},
+    {url = "https://files.pythonhosted.org/packages/0e/da/055d5b854a9a702fed0965d37754b79967ecfd67fe8377264e6a00b521ea/shapely-2.0.1-cp39-cp39-manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:c43755d2c46b75a7b74ac6226d2cc9fa2a76c3263c5ae70c195c6fb4e7b08e79"},
+    {url = "https://files.pythonhosted.org/packages/10/a7/de139da3ce303101c357a9ba801328cba85cf6ace157da31a4007bca85e4/shapely-2.0.1.tar.gz", hash = "sha256:66a6b1a3e72ece97fc85536a281476f9b7794de2e646ca8a4517e2e3c1446893"},
+    {url = "https://files.pythonhosted.org/packages/18/a6/2e1761f21605e3562b223be7ad82f2edb5c9babdaa8b2d90979112be70f3/shapely-2.0.1-cp311-cp311-macosx_11_0_arm64.whl", hash = "sha256:f470a130d6ddb05b810fc1776d918659407f8d025b7f56d2742a596b6dffa6c7"},
+    {url = "https://files.pythonhosted.org/packages/1d/a4/931d0780f31f3ea8c4f9ef6464a2825137c5241e6707a5fb03bef760a7eb/shapely-2.0.1-cp37-cp37m-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:c8b0d834b11be97d5ab2b4dceada20ae8e07bcccbc0f55d71df6729965f406ad"},
+    {url = "https://files.pythonhosted.org/packages/1f/2a/dc3353c2431cf53e8d04bb8fba27e584410ca3435c9c85f76d71bf0c0e80/shapely-2.0.1-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:9a6ac34c16f4d5d3c174c76c9d7614ec8fe735f8f82b6cc97a46b54f386a86bf"},
+    {url = "https://files.pythonhosted.org/packages/28/81/0239107ccd32eb30085c99fbf22da686aa72278afcc2c8fdf06fa0fa6320/shapely-2.0.1-cp311-cp311-win_amd64.whl", hash = "sha256:d8f55f355be7821dade839df785a49dc9f16d1af363134d07eb11e9207e0b189"},
+    {url = "https://files.pythonhosted.org/packages/2b/cf/c0315a82849de40897ebb09ef441fea4b995570443e4b596b9bc7c8a7fa4/shapely-2.0.1-cp38-cp38-win_amd64.whl", hash = "sha256:c7eed1fb3008a8a4a56425334b7eb82651a51f9e9a9c2f72844a2fb394f38a6c"},
+    {url = "https://files.pythonhosted.org/packages/2d/f2/8ec281d357e8bb7d08dc8d727f0e4c8ef3dae7d3fa75c69c8e452bb82d50/shapely-2.0.1-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:3ad81f292fffbd568ae71828e6c387da7eb5384a79db9b4fde14dd9fdeffca9a"},
+    {url = "https://files.pythonhosted.org/packages/31/05/cbdfaf562ce7a0e0e89b47b3000d3445967c9fca6f906f833faba371053c/shapely-2.0.1-cp38-cp38-macosx_11_0_arm64.whl", hash = "sha256:e55698e0ed95a70fe9ff9a23c763acfe0bf335b02df12142f74e4543095e9a9b"},
+    {url = "https://files.pythonhosted.org/packages/35/da/00737e3cd038d489c257a00829c27b3ff2d3ec264c78540a5d168a06922f/shapely-2.0.1-cp310-cp310-macosx_10_9_universal2.whl", hash = "sha256:b06d031bc64149e340448fea25eee01360a58936c89985cf584134171e05863f"},
+    {url = "https://files.pythonhosted.org/packages/36/a4/7e542a209f862f967d7cb8e939eff155f4294a27d17e16441fb8bdd51a2c/shapely-2.0.1-cp39-cp39-macosx_10_9_x86_64.whl", hash = "sha256:33403b8896e1d98aaa3a52110d828b18985d740cc9f34f198922018b1e0f8afe"},
+    {url = "https://files.pythonhosted.org/packages/41/63/088ea482b1f2a046ec0576b173125a6485d0cc7e3868d50e74f4a89039f5/shapely-2.0.1-cp39-cp39-win32.whl", hash = "sha256:b50c401b64883e61556a90b89948297f1714dbac29243d17ed9284a47e6dd731"},
+    {url = "https://files.pythonhosted.org/packages/49/85/ee3d63f3a4affd146ddb01094c69ae74719c4462285e8aad4d3c6ec70a7b/shapely-2.0.1-cp38-cp38-win32.whl", hash = "sha256:3cb256ae0c01b17f7bc68ee2ffdd45aebf42af8992484ea55c29a6151abe4386"},
+    {url = "https://files.pythonhosted.org/packages/69/2e/29633eca429c9e7eca1264df1764a7f179ec9ec186ba25d874342dcb1a47/shapely-2.0.1-cp310-cp310-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:45b4833235b90bc87ee26c6537438fa77559d994d2d3be5190dd2e54d31b2820"},
+    {url = "https://files.pythonhosted.org/packages/70/21/39c2afae46154f824564d6b5b7213a84d083e243b42b5a1e76de481f91bb/shapely-2.0.1-cp311-cp311-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:4641325e065fd3e07d55677849c9ddfd0cf3ee98f96475126942e746d55b17c8"},
+    {url = "https://files.pythonhosted.org/packages/74/c6/2099380d719a7e38cf0643df562b50d458f4960c2c7bb493e2fbe850753a/shapely-2.0.1-cp38-cp38-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:f32a748703e7bf6e92dfa3d2936b2fbfe76f8ce5f756e24f49ef72d17d26ad02"},
+    {url = "https://files.pythonhosted.org/packages/7b/e3/92ec80d72de8b881c52e47db1fd2f0519d49b6ad65c4c2a3fcbb9f88a91f/shapely-2.0.1-cp311-cp311-macosx_10_9_x86_64.whl", hash = "sha256:7d3bbeefd8a6a1a1017265d2d36f8ff2d79d0162d8c141aa0d37a87063525656"},
+    {url = "https://files.pythonhosted.org/packages/81/8a/7ac076a86b2632f1872284c5e60ed5f2fc26094875a85b35d9fa17b52504/shapely-2.0.1-cp310-cp310-win_amd64.whl", hash = "sha256:da71de5bf552d83dcc21b78cc0020e86f8d0feea43e202110973987ffa781c21"},
+    {url = "https://files.pythonhosted.org/packages/82/12/ed1087cd4b9a6bc6f1f77b35078a49991672fbfa7302ea480322615cd909/shapely-2.0.1-cp38-cp38-manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:1a34a23d6266ca162499e4a22b79159dc0052f4973d16f16f990baa4d29e58b6"},
+    {url = "https://files.pythonhosted.org/packages/8a/31/ad4881727b700a9320a4139ac3483972901a9fdd17bb6a599aca810dbd85/shapely-2.0.1-cp311-cp311-macosx_10_9_universal2.whl", hash = "sha256:502e0a607f1dcc6dee0125aeee886379be5242c854500ea5fd2e7ac076b9ce6d"},
+    {url = "https://files.pythonhosted.org/packages/91/d3/1f7c41508d42b81b4f454ad20a7f17a73225949805ea638125ac09188d33/shapely-2.0.1-cp37-cp37m-win32.whl", hash = "sha256:b4f0711cc83734c6fad94fc8d4ec30f3d52c1787b17d9dca261dc841d4731c64"},
+    {url = "https://files.pythonhosted.org/packages/94/0f/09e51e71c3a35818abe1ba75f2d2516a5c90b3596989920a0b116768fe32/shapely-2.0.1-cp38-cp38-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:d173d24e85e51510e658fb108513d5bc11e3fd2820db6b1bd0522266ddd11f51"},
+    {url = "https://files.pythonhosted.org/packages/98/e4/2d5b48e13cbcc976f468b995bb8bcfa8e758a8b73fe307af54184989158e/shapely-2.0.1-cp39-cp39-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:a70a614791ff65f5e283feed747e1cc3d9e6c6ba91556e640636bbb0a1e32a71"},
+    {url = "https://files.pythonhosted.org/packages/a7/ae/eab645c4075093584b7a65ab71cb8ff4563a015bd935c9b55dba14b2c1eb/shapely-2.0.1-cp39-cp39-win_amd64.whl", hash = "sha256:bca57b683e3d94d0919e2f31e4d70fdfbb7059650ef1b431d9f4e045690edcd5"},
+    {url = "https://files.pythonhosted.org/packages/a8/a5/403728b5614b28083f6424dfdefec5fcf58068495fb03bb08532671c642f/shapely-2.0.1-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:ce88ec79df55430e37178a191ad8df45cae90b0f6972d46d867bf6ebbb58cc4d"},
+    {url = "https://files.pythonhosted.org/packages/b0/b4/b0cedcc974f5d3fba51850f81961f48a1246b4c4ddf4cd3faef6829e4173/shapely-2.0.1-cp39-cp39-macosx_10_9_universal2.whl", hash = "sha256:ac1dfc397475d1de485e76de0c3c91cc9d79bd39012a84bb0f5e8a199fc17bef"},
+    {url = "https://files.pythonhosted.org/packages/b4/6f/08bb91f043854ec9e73b8d970437b6dca7323e44c63b53d2af6e80a9edba/shapely-2.0.1-cp38-cp38-macosx_10_9_x86_64.whl", hash = "sha256:193a398d81c97a62fc3634a1a33798a58fd1dcf4aead254d080b273efbb7e3ff"},
+    {url = "https://files.pythonhosted.org/packages/bb/9b/c9dc1b43cd4364a247f7e82959f77b7ba63e6fe0b98435e3c98b08ba01d6/shapely-2.0.1-cp38-cp38-macosx_10_9_universal2.whl", hash = "sha256:b519cf3726ddb6c67f6a951d1bb1d29691111eaa67ea19ddca4d454fbe35949c"},
+    {url = "https://files.pythonhosted.org/packages/bc/f1/c9db479170a7288d6bd2adcd1892785a3206b7a6f7972e7478714cb39e3c/shapely-2.0.1-cp311-cp311-win32.whl", hash = "sha256:09d6c7763b1bee0d0a2b84bb32a4c25c6359ad1ac582a62d8b211e89de986154"},
+    {url = "https://files.pythonhosted.org/packages/cf/0f/c0456b1382d2a6815727cbd9c0713deca11653b330ba14b2cc165f0b9565/shapely-2.0.1-cp310-cp310-win32.whl", hash = "sha256:01224899ff692a62929ef1a3f5fe389043e262698a708ab7569f43a99a48ae82"},
+    {url = "https://files.pythonhosted.org/packages/e2/87/b8b8d8d57b429b01aa56b7d723075c09f33c988b8091bb6f790c83436909/shapely-2.0.1-cp37-cp37m-win_amd64.whl", hash = "sha256:05c51a29336e604c084fb43ae5dbbfa2c0ef9bd6fedeae0a0d02c7b57a56ba46"},
+    {url = "https://files.pythonhosted.org/packages/e6/7d/4923f27c340339e1c896c77cafc8ed672c8d381a025bbab6c6ddcba27e8f/shapely-2.0.1-cp37-cp37m-macosx_10_9_x86_64.whl", hash = "sha256:83a8ec0ee0192b6e3feee9f6a499d1377e9c295af74d7f81ecba5a42a6b195b7"},
+    {url = "https://files.pythonhosted.org/packages/e9/7c/76e54fa615a20ceb876e4de6b9f01a56926184bcc2076186c51c27ce39ad/shapely-2.0.1-cp311-cp311-manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:90cfa4144ff189a3c3de62e2f3669283c98fb760cfa2e82ff70df40f11cadb39"},
+    {url = "https://files.pythonhosted.org/packages/ea/aa/45fbd031edf3149cb767d8b9f9db45d5faf0324d743c6b8fb0298cc022d0/shapely-2.0.1-cp39-cp39-macosx_11_0_arm64.whl", hash = "sha256:2569a4b91caeef54dd5ae9091ae6f63526d8ca0b376b5bb9fd1a3195d047d7d4"},
+    {url = "https://files.pythonhosted.org/packages/ec/41/d59208743e737184e1b403e95a937aebb022b8459e99efbcd5208fc8be46/shapely-2.0.1-cp310-cp310-macosx_11_0_arm64.whl", hash = "sha256:865bc3d7cc0ea63189d11a0b1120d1307ed7a64720a8bfa5be2fde5fc6d0d33f"},
+    {url = "https://files.pythonhosted.org/packages/f7/17/8bb86d26173982b81675cf6bcb0941ca144ea569a966d67774460121ba55/shapely-2.0.1-cp37-cp37m-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:a529218e72a3dbdc83676198e610485fdfa31178f4be5b519a8ae12ea688db14"},
+    {url = "https://files.pythonhosted.org/packages/fa/fb/7ce0aff96d317916ec75889068c9c6bd92268b20839efd270e3d4e7107ab/shapely-2.0.1-cp37-cp37m-manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:91575d97fd67391b85686573d758896ed2fc7476321c9d2e2b0c398b628b961c"},
+]
 "six 1.12.0" = [
     {url = "https://files.pythonhosted.org/packages/73/fb/00a976f728d0d1fecfe898238ce23f502a721c0ac0ecfedb80e0d88c64e9/six-1.12.0-py2.py3-none-any.whl", hash = "sha256:3350809f0555b11f552448330d0b52d5f24c91a322ea4a15ef22629740f3761c"},
     {url = "https://files.pythonhosted.org/packages/dd/bf/4138e7bfb757de47d1f4b6994648ec67a51efe58fa907c1e11e350cddfca/six-1.12.0.tar.gz", hash = "sha256:d16a0141ec1a18405cd4ce8b4613101da75da0e9a7aec5bdd4fa804d0e0eba73"},
 ]
-"sklearn 0.0.post5" = [
-    {url = "https://files.pythonhosted.org/packages/7a/93/e0e1b1e98f39dfca7ec9795cb46f6e09e88a2fd5d4a28e4b3d1f618a2aec/sklearn-0.0.post5.tar.gz", hash = "sha256:7377c714a03a79bbe9196f435db931fd2a6fa8c68514da7ed3a251fd08c52e2c"},
-]
 "smart-open 6.3.0" = [
     {url = "https://files.pythonhosted.org/packages/47/80/c2d1bdd36c6b64ae566d9a29724291510e4f3796ce99639d3c2999286284/smart_open-6.3.0-py3-none-any.whl", hash = "sha256:b4c9ae193ad6d3e7add50944b86afa0d150bd821ab8ec21edb26d9a06b66f6a8"},
     {url = "https://files.pythonhosted.org/packages/b0/2b/ebc6d835bb354eb6d7f5f560be53dc746dab84d0958c363a082bfdf1e862/smart_open-6.3.0.tar.gz", hash = "sha256:d5238825fe9a9340645fac3d75b287c08fbb99fb2b422477de781c9f5f09e019"},
 ]
 "sortedcontainers 2.4.0" = [
     {url = "https://files.pythonhosted.org/packages/32/46/9cb0e58b2deb7f82b84065f37f3bffeb12413f947f9388e4cac22c4621ce/sortedcontainers-2.4.0-py2.py3-none-any.whl", hash = "sha256:a163dcaede0f1c021485e957a39245190e74249897e2ae4b2aa38595db237ee0"},
     {url = "https://files.pythonhosted.org/packages/e8/c4/ba2f8066cceb6f23394729afe52f3bf7adec04bf9ed2c820b39e19299111/sortedcontainers-2.4.0.tar.gz", hash = "sha256:25caa5a06cc30b6b83d11423433f65d1f9d76c4c6a0c90e3379eaa43b9bfdb88"},
@@ -3008,17 +3257,17 @@
 "speechrecognition 3.8.1" = [
     {url = "https://files.pythonhosted.org/packages/26/e1/7f5678cd94ec1234269d23756dbdaa4c8cfaed973412f88ae8adf7893a50/SpeechRecognition-3.8.1-py2.py3-none-any.whl", hash = "sha256:4d8f73a0c05ec70331c3bacaa89ecc06dfa8d9aba0899276664cda06ab597e8e"},
 ]
 "sqlite-fts4 1.0.3" = [
     {url = "https://files.pythonhosted.org/packages/51/29/0096e8b1811aaa78cfb296996f621f41120c21c2f5cd448ae1d54979d9fc/sqlite_fts4-1.0.3-py3-none-any.whl", hash = "sha256:0359edd8dea6fd73c848989e1e2b1f31a50fe5f9d7272299ff0e8dbaa62d035f"},
     {url = "https://files.pythonhosted.org/packages/c2/6d/9dad6c3b433ab8912ace969c66abd595f8e0a2ccccdb73602b1291dbda29/sqlite-fts4-1.0.3.tar.gz", hash = "sha256:78b05eeaf6680e9dbed8986bde011e9c086a06cb0c931b3cf7da94c214e8930c"},
 ]
-"sqlite-utils 3.32.1" = [
-    {url = "https://files.pythonhosted.org/packages/1a/95/b6fe852980c9494bf8a5e99d017cc6b864f9807a3e082c7837c267302217/sqlite-utils-3.32.1.tar.gz", hash = "sha256:6c28fe32fcebd658a1691dedfa4d111499ad302cc0139c5a5893a590d461848a"},
-    {url = "https://files.pythonhosted.org/packages/9e/eb/144eb61fd739b78d412d84d2d79148a4c5f3160c766317e9a19cd4ce3160/sqlite_utils-3.32.1-py3-none-any.whl", hash = "sha256:dfa124c4f752d67b2a36aa41929c51c699d81364b7b076218885a5ea714610d0"},
+"sqlite-utils 3.33" = [
+    {url = "https://files.pythonhosted.org/packages/6f/66/bde379930f356e157b880e9a55058c44e0846f18d1839104fc947b13cb93/sqlite_utils-3.33-py3-none-any.whl", hash = "sha256:a5260d0797606650847b3367547e9e3c4cba51ca88d55a1da0cef9aa2f13dfd5"},
+    {url = "https://files.pythonhosted.org/packages/99/48/b974a270fd710e62c5ab863dc216cf3ffe26b5108ffb5d64ddeba1786bce/sqlite-utils-3.33.tar.gz", hash = "sha256:be779936dadb9decef511a46f280bd94683d385625f69a65730fb6e00e5f2656"},
 ]
 "srsly 2.4.6" = [
     {url = "https://files.pythonhosted.org/packages/03/46/bfa8823b635ca9867c130d6a52506d132249293063a5cb0fee0358014d84/srsly-2.4.6-cp39-cp39-macosx_10_9_x86_64.whl", hash = "sha256:0522d9aeaf58c6d58ee0cec247653a460545422d3266b2d970df7af1530f3dcc"},
     {url = "https://files.pythonhosted.org/packages/20/25/4dba38f470b4683b68ee741b85d852248074ce90eee503490a543c279c1f/srsly-2.4.6-cp311-cp311-macosx_11_0_arm64.whl", hash = "sha256:99131465fea74aa5e80dbba6effad10ae661bee2c3fbc1fd6da8a1e954e031d0"},
     {url = "https://files.pythonhosted.org/packages/29/19/c9af82aca65180b187f335bfbfa52719e2056367956ebbf32fcabff46b37/srsly-2.4.6-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:2261ef76f6b8d4029b9d2fc4a65ac505a760d2ea1de0132fc4b423883f7df52e"},
     {url = "https://files.pythonhosted.org/packages/29/ab/e819adf93bee080c594d3207cc96e0263f5094967246cfd6b09356093cd5/srsly-2.4.6-cp38-cp38-macosx_11_0_arm64.whl", hash = "sha256:720715be0efb9646ab64850185ecd22fe6ace93027d02f6367bdc8842450b369"},
     {url = "https://files.pythonhosted.org/packages/38/1c/66e7908dd223eb6e0befee2056ae1ccc64451a589380ea8e841ddbea976b/srsly-2.4.6-cp38-cp38-macosx_10_9_x86_64.whl", hash = "sha256:02b0708878f6a1e344284ae7c65b36a9ad8178eeff71583cd212d2d379f0e2ce"},
@@ -3096,14 +3345,18 @@
     {url = "https://files.pythonhosted.org/packages/a6/0b/fafa1853bf5db8403a1ff2499b9a6b811b7d4228fc044a1f03345017cf4c/thinc-8.1.10-cp36-cp36m-win_amd64.whl", hash = "sha256:bc321d0fbb8e146de4c152d36ea6000de0669fe081fd9777c8768ad9b4478839"},
     {url = "https://files.pythonhosted.org/packages/b0/c3/c3f124964f216e728acb7205f41609f9799177f13380298adf1ecfd7d8f7/thinc-8.1.10-cp311-cp311-macosx_10_9_x86_64.whl", hash = "sha256:575b7dbe3a5d773c12f5dd6e366d942ad3c3ef7a5381332ba842bdbaf4d3e820"},
     {url = "https://files.pythonhosted.org/packages/ba/dd/174a128d0e84814b0f05ec5de9ecf65e3a9b3c4882823610736385df21ab/thinc-8.1.10-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:dbd1dc4394352d80af22131e1a238238eded59de19b55f77e6237436f4865b2c"},
     {url = "https://files.pythonhosted.org/packages/d3/60/c82a50fdde18d4544719c88d8e8adc0ba9ea23bb444b03e7296982f93a58/thinc-8.1.10-cp37-cp37m-macosx_10_9_x86_64.whl", hash = "sha256:bd9b678bcbf3f3a21260b2f55a65742aeeb7f5442c3ceb475378d95e0e99dc44"},
     {url = "https://files.pythonhosted.org/packages/f3/5c/4e8671aa258dbefce508aa0236fae572bf7bbd9784fad3637d76a858ff6f/thinc-8.1.10-cp38-cp38-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:d31f6834f1b1c428718a9668b7a06b74854a9217ba1d8186b41e48146d487fa3"},
     {url = "https://files.pythonhosted.org/packages/fb/aa/daaff7c5c5878cad416b906bb8b573b5a4023e11a138ad082f1fb089eab8/thinc-8.1.10.tar.gz", hash = "sha256:6c4a48d7da07e044e84a68cbb9b22f32f8490995a2bab0bfc60e412d14afb991"},
 ]
+"threadpoolctl 3.1.0" = [
+    {url = "https://files.pythonhosted.org/packages/1b/c7/3d85f8b3894ba7228d0c74e16e97a36a72b2cd2b0e0f8f89b5d435d11f71/threadpoolctl-3.1.0.tar.gz", hash = "sha256:a335baacfaa4400ae1f0d8e3a58d6674d2f8828e3716bb2802c44955ad391380"},
+    {url = "https://files.pythonhosted.org/packages/61/cf/6e354304bcb9c6413c4e02a747b600061c21d38ba51e7e544ac7bc66aecc/threadpoolctl-3.1.0-py3-none-any.whl", hash = "sha256:8b99adda265feb6773280df41eece7b2e6561b772d21ffd52e372f999024907b"},
+]
 "tinytag 1.9.0" = [
     {url = "https://files.pythonhosted.org/packages/33/58/ff5f7a345b6448b6ad3cb8dd3c9a6cb4100e3359468e5f984aaca2634213/tinytag-1.9.0.tar.gz", hash = "sha256:f8d71110e1e680a33d99202e00a5a698481d25d20173b81ba3e863423979e014"},
 ]
 "tomli 2.0.1" = [
     {url = "https://files.pythonhosted.org/packages/97/75/10a9ebee3fd790d20926a90a2547f0bf78f371b2f13aa822c759680ca7b9/tomli-2.0.1-py3-none-any.whl", hash = "sha256:939de3e7a6161af0c887ef91b7d41a53e7c5a1ca976325f429cb46ea9bc30ecc"},
     {url = "https://files.pythonhosted.org/packages/c0/3f/d7af728f075fb08564c5949a9c95e44352e23dee646869fa104a3b2060a3/tomli-2.0.1.tar.gz", hash = "sha256:de526c12914f0c550d15924c62d72abc48d6fe7364aa87328337a31007fe8a4f"},
 ]
@@ -3143,17 +3396,17 @@
     {url = "https://files.pythonhosted.org/packages/3e/09/bbd7e880b56e825d5859a58adb1bd1feb45b604218706057ca1e3278fa62/wasabi-1.1.2.tar.gz", hash = "sha256:1aaef3aceaa32edb9c91330d29d3936c0c39fdb965743549c173cb54b16c30b5"},
     {url = "https://files.pythonhosted.org/packages/8f/69/26cbf0bad11703241cb84d5324d868097f7a8faf2f1888354dac8883f3fc/wasabi-1.1.2-py3-none-any.whl", hash = "sha256:0a3f933c4bf0ed3f93071132c1b87549733256d6c8de6473c5f7ed2e171b5cf9"},
 ]
 "wcwidth 0.2.6" = [
     {url = "https://files.pythonhosted.org/packages/20/f4/c0584a25144ce20bfcf1aecd041768b8c762c1eb0aa77502a3f0baa83f11/wcwidth-0.2.6-py2.py3-none-any.whl", hash = "sha256:795b138f6875577cd91bba52baf9e445cd5118fd32723b460e30a0af30ea230e"},
     {url = "https://files.pythonhosted.org/packages/5e/5f/1e4bd82a9cc1f17b2c2361a2d876d4c38973a997003ba5eb400e8a932b6c/wcwidth-0.2.6.tar.gz", hash = "sha256:a5220780a404dbe3353789870978e472cfe477761f06ee55077256e509b156d0"},
 ]
-"websocket-client 1.6.0" = [
-    {url = "https://files.pythonhosted.org/packages/31/4e/aa6ab8f8812b5766350ed2beb5bc6f3a007c448dd9c178ef5db2d163dac3/websocket-client-1.6.0.tar.gz", hash = "sha256:e84c7eafc66aade6d1967a51dfd219aabdf81d15b9705196e11fd81f48666b78"},
-    {url = "https://files.pythonhosted.org/packages/cd/b9/cf588fc9e8cdfe2cdb22360c608a9337918ee63ded9b232fe9c1c46e1d8a/websocket_client-1.6.0-py3-none-any.whl", hash = "sha256:72d7802608745b0a212f79b478642473bd825777d8637b6c8c421bf167790d4f"},
+"websocket-client 1.6.1" = [
+    {url = "https://files.pythonhosted.org/packages/b1/34/3a5cae1e07d9566ad073fa6d169bf22c03a3ba7b31b3c3422ec88d039108/websocket-client-1.6.1.tar.gz", hash = "sha256:c951af98631d24f8df89ab1019fc365f2227c0892f12fd150e935607c79dd0dd"},
+    {url = "https://files.pythonhosted.org/packages/d3/a3/63e9329c8cc9be6153e919e17d0ef5b60d537fed78564872951b95bcc17c/websocket_client-1.6.1-py3-none-any.whl", hash = "sha256:f1f9f2ad5291f0225a49efad77abf9e700b6fef553900623060dad6e26503b9d"},
 ]
 "websockets 11.0.3" = [
     {url = "https://files.pythonhosted.org/packages/03/28/3a51ffcf51ac45746639f83128908bbb1cd212aa631e42d15a7acebce5cb/websockets-11.0.3-pp37-pypy37_pp73-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:e052b8467dd07d4943936009f46ae5ce7b908ddcac3fda581656b1b19c083d9b"},
     {url = "https://files.pythonhosted.org/packages/0a/84/68b848a373493b58615d6c10e9e8ccbaadfd540f84905421739a807704f8/websockets-11.0.3-cp311-cp311-macosx_10_9_x86_64.whl", hash = "sha256:aa5003845cdd21ac0dc6c9bf661c5beddd01116f6eb9eb3c8e272353d45b3288"},
     {url = "https://files.pythonhosted.org/packages/0f/d8/a997d3546aef9cc995a1126f7d7ade96c0e16c1a0efb9d2d430aee57c925/websockets-11.0.3-cp311-cp311-musllinux_1_1_i686.whl", hash = "sha256:619d9f06372b3a42bc29d0cd0354c9bb9fb39c2cbc1a9c5025b4538738dbffaf"},
     {url = "https://files.pythonhosted.org/packages/14/fc/5cbbf439c925e1e184a0392ec477a30cee2fabc0e63807c1d4b6d570fb52/websockets-11.0.3-cp311-cp311-musllinux_1_1_aarch64.whl", hash = "sha256:b30c6590146e53149f04e85a6e4fcae068df4289e31e4aee1fdf56a0dead8f97"},
     {url = "https://files.pythonhosted.org/packages/16/49/ae616bd221efba84a3d78737b417f704af1ffa36f40dcaba5eb954dd4753/websockets-11.0.3-cp311-cp311-macosx_10_9_universal2.whl", hash = "sha256:e848f46a58b9fcf3d06061d17be388caf70ea5b8cc3466251963c8345e13f7eb"},
@@ -3311,17 +3564,17 @@
     {url = "https://files.pythonhosted.org/packages/f0/cc/cf416dff5bd88899a567fea556a5f68ab94cdf525ebe122e0bdba478f2c4/yarl-1.9.2-cp37-cp37m-musllinux_1_1_i686.whl", hash = "sha256:52a25809fcbecfc63ac9ba0c0fb586f90837f5425edfd1ec9f3372b119585e45"},
     {url = "https://files.pythonhosted.org/packages/f1/0c/c2e07b3a37c4363078a1c7d586b251eec191594a2d24d6e09dae33c1368f/yarl-1.9.2-cp37-cp37m-musllinux_1_1_s390x.whl", hash = "sha256:1b1bba902cba32cdec51fca038fd53f8beee88b77efc373968d1ed021024cc04"},
     {url = "https://files.pythonhosted.org/packages/f2/b1/9a6eeba1a3f35188eac6b7b535f20c06df0f48e78705405d86a0407e75f1/yarl-1.9.2-cp38-cp38-win32.whl", hash = "sha256:f7a3d8146575e08c29ed1cd287068e6d02f1c7bdff8970db96683b9591b86ee7"},
     {url = "https://files.pythonhosted.org/packages/f2/ea/6fd350376ed2581d0cdb11018bad0215cf987817dba69ea9a4bf8adbac6e/yarl-1.9.2-cp39-cp39-musllinux_1_1_x86_64.whl", hash = "sha256:8288d7cd28f8119b07dd49b7230d6b4562f9b61ee9a4ab02221060d21136be80"},
     {url = "https://files.pythonhosted.org/packages/fb/2d/060ab740f64ea6ea2088e375c3046839faaf4bbba2b65a5364668bd765e7/yarl-1.9.2-cp38-cp38-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:84e0b1599334b1e1478db01b756e55937d4614f8654311eb26012091be109d59"},
     {url = "https://files.pythonhosted.org/packages/fe/7d/9d85f658b6f7c041ca3ba371d133040c4dc41eb922aef0a6ba917291d187/yarl-1.9.2-cp311-cp311-macosx_10_9_x86_64.whl", hash = "sha256:aff634b15beff8902d1f918012fc2a42e0dbae6f469fce134c8a0dc51ca423bb"},
 ]
-"yt-dlp 2023.6.21" = [
-    {url = "https://files.pythonhosted.org/packages/36/9a/13eee74e6a621ab42d2b8c7fd7daf6e943af1a8269aa966718fae177a64b/yt-dlp-2023.6.21.tar.gz", hash = "sha256:56c35d1ad3ecfb828c3b89ffe07b235b354eddd82e1a31ddc3d16eb8c3e71e8e"},
-    {url = "https://files.pythonhosted.org/packages/45/27/02df242aba3ccb6b02457c4063113add4c7b06af46f1cd5bc75b9856656f/yt_dlp-2023.6.21-py2.py3-none-any.whl", hash = "sha256:e4117b1ee07878c7dade2a64e6102fb7840fa1e3f19365cca42ce291754f35cf"},
+"yt-dlp 2023.6.22" = [
+    {url = "https://files.pythonhosted.org/packages/57/86/b5fb11442d96a7a438ec6ad27d04c546f4f7e64c3d551259f886adeddb8e/yt-dlp-2023.6.22.tar.gz", hash = "sha256:ed6a8b8e0ad08a4540d4afa0fd08a7f980022c79b9081bd9e63ddc00aeeee5a8"},
+    {url = "https://files.pythonhosted.org/packages/65/9b/21628ca5bcf40f58c33f0fbb4927a1bb91e12f3c33a3cf8e29e03f6bc1d1/yt_dlp-2023.6.22-py2.py3-none-any.whl", hash = "sha256:c559885322f7f492c1e7fc8f5a59e2a72e47719b59575599cf8b0e69ea70d0a8"},
 ]
 "zeroconf 0.69.0" = [
     {url = "https://files.pythonhosted.org/packages/04/f9/b89ba913563eca7ad5cf80d066d14df68c8a1614731b07a5cc238c7680cb/zeroconf-0.69.0-pp39-pypy39_pp73-manylinux_2_17_i686.manylinux_2_5_i686.manylinux1_i686.manylinux2014_i686.whl", hash = "sha256:9e2cfe4baa6540e21cbb74d820a1bf8f3258449bee92be1cba289033fe77f0c9"},
     {url = "https://files.pythonhosted.org/packages/0b/30/0d5cb2bf0a29e844748c039d7ceb13008a376e2af95c6b51f4a8754ed494/zeroconf-0.69.0-cp39-cp39-macosx_11_0_x86_64.whl", hash = "sha256:ff92c07ff69156cb496d001700afd06959c37b80731c78c5ce896f4f3aebfe21"},
     {url = "https://files.pythonhosted.org/packages/0b/31/516fd6b8512190e94896ece6c37f9be244611ea2c64877a3ea0227ef532d/zeroconf-0.69.0-cp311-cp311-macosx_11_0_x86_64.whl", hash = "sha256:1dea30128d618a46d489809a55a932a5797c353b5d9a3dc5ed63d5d5887a7e97"},
     {url = "https://files.pythonhosted.org/packages/0b/5a/03a16379942dd478099eddc92316e4b1be37928797fa12ed592353360482/zeroconf-0.69.0-cp39-cp39-manylinux_2_17_i686.manylinux_2_5_i686.manylinux1_i686.manylinux2014_i686.whl", hash = "sha256:0a7a34989a88eacd4948e8a04c5b9ed5757df8684a09fb85e8f3d374b57903e5"},
     {url = "https://files.pythonhosted.org/packages/15/72/34dbc01948cf279175f4d042405caefeb90e720cfcb9988b370ca8dee052/zeroconf-0.69.0-cp37-cp37m-manylinux_2_17_i686.manylinux_2_5_i686.manylinux1_i686.manylinux2014_i686.whl", hash = "sha256:d1d543bc558e526ae217848c508c737d74be678712ebd226fc3d8335762b807f"},
```

### Comparing `xklb-2.1.9/readme.py` & `xklb-2.2.2/readme.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,14 +22,15 @@
     ("Re-optimize database", "optimize"),
     ("Re-download media", "redownload"),
     ("Merge online and local data", "merge-online-local"),
     ("Convert selftext links to media table", "reddit-selftext"),
     ("Merge SQLITE databases", "merge-dbs"),
     ("Dedupe SQLITE tables", "dedupe-db"),
     ("Show large folders", "bigdirs"),
+    ("Disk Usage", "disk-usage"),
     ("Copy play history", "copy-play-counts"),
     ("Import mpv watchlater files", "mpv-watchlater"),
     ("Sort data by similarity", "cluster-sort"),
     ("Scatter files between folders or disks", "scatter"),
     ("Move files preserving parent folder hierarchy", "relmv"),
     ("Clean filenames", "christen"),
     ("Dedupe music", "dedupe"),
@@ -371,13 +372,40 @@
     pip install datasette
     datasette tv.db
 
 ## Usage
 
 {''.join(usage_details)}
 
+<details><summary>Chicken mode</summary>
+
+just kidding :-)
+
+           ////////////////////////
+          ////////////////////////|
+         //////////////////////// |
+        ////////////////////////| |
+        |    _\/_   |   _\/_    | |
+        |     )o(>  |  <)o(     | |
+        |   _/ <\   |   /> \_   | |
+        |  (_____)  |  (_____)  | |_
+        | ~~~oOo~~~ | ~~~0oO~~~ |/__|
+       _|====\_=====|=====_/====|_ ||
+      |_|\_________ O _________/|_|||
+       ||//////////|_|\\\\\\\\\\|| ||
+       || ||       |\_\\        || ||
+       ||/||        \\_\\       ||/||
+       ||/||         \)_\)      ||/||
+       || ||         \  O /     || ||
+       ||             \  /      || LGB
+
+                   \________/======
+                   / ( || ) \\
+
+</details>
+
 You can expand all by running this in your browser console:
 
 {expand_all_js}
 
 """,
 )
```

### Comparing `xklb-2.1.9/.github/ISSUE_TEMPLATE/bug_report.md` & `xklb-2.2.2/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `xklb-2.1.9/.github/ISSUE_TEMPLATE/feature_request.md` & `xklb-2.2.2/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `xklb-2.1.9/.github/workflows/push.yaml` & `xklb-2.2.2/.github/workflows/push.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
           python-version: ${{ matrix.nv.py }}
 
       - uses: FedericoCarboni/setup-ffmpeg@v2
 
       - name: Install Dependencies
         run: |
           python -m pip install pdm 'requests<2.30.0'
-          pdm install --no-editable -G test
+          pdm install --no-editable -G deluxe -G test
 
       - name: Run pytest
         run: pdm run pytest
 
   publish:
     needs: test
     runs-on: ubuntu-latest
```

### Comparing `xklb-2.1.9/xklb/av.py` & `xklb-2.2.2/xklb/av.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.9/xklb/books.py` & `xklb-2.2.2/xklb/books.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.9/xklb/consts.py` & `xklb-2.2.2/xklb/consts.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,14 +48,15 @@
             r".*redd\.it/user/(.*?)/.*",
         ],
     ),
 )
 REGEX_V_REDD_IT = re.compile("https?://v.redd.it/(?:[^/?#&]+)")
 APPLICATION_START = now()
 TERMINAL_SIZE = shutil.get_terminal_size(fallback=(80, 60))
+TABULATE_STYLE = "simple"
 
 TIME_COLUMNS = (
     "time_scanned",
     "time_downloaded",
     "time_deleted",
     "time_modified",
     "time_created",
@@ -180,22 +181,15 @@
     "created",
     "modified",
     "downloaded",
 ]
 
 frequency = ["daily", "weekly", "monthly", "quarterly", "yearly"]
 
-PLAYLIST_KNOWN_KEYS = (
-    "description",
-    "url",
-    "duration",
-    "view_count",
-    "webpage_url",
-    "original_url",
-)
+PLAYLIST_KNOWN_KEYS = ("description", "url", "duration", "view_count", "webpage_url", "original_url", "time_deleted")
 
 MEDIA_KNOWN_KEYS = (
     "photoset_layout",
     "asks_allow_media",
     "submission_page_title",
     "post_author_is_adult",
     "is_submission",
```

### Comparing `xklb-2.1.9/xklb/db.py` & `xklb-2.2.2/xklb/db.py`

 * *Files 1% similar despite different names*

```diff
@@ -134,16 +134,18 @@
         table_config = config.get(table) or {}
         ignore_columns = table_config.get("ignore_columns") or []
         search_columns = table_config.get("search_columns") or []
 
         fts_columns = [c for c in search_columns if c in table_columns]
         int_columns = [k for k, v in table_columns.items() if v == int and k not in search_columns + ignore_columns]
         str_columns = [k for k, v in table_columns.items() if v == str and k not in search_columns + ignore_columns]
+        if "path" in table_columns:
+            str_columns = list(set(str_columns + ["path"]))
 
-        optimized_column_order = [*int_columns, *(table_config.get("column_order") or [])]
+        optimized_column_order = list(utils.order_set([*int_columns, *(table_config.get("column_order") or [])]))
         compare_order = zip(table_columns, optimized_column_order)
         was_transformed = False
         if not all(x == y for x, y in compare_order):
             log.info("Transforming column order: %s", optimized_column_order)
             db[table].transform(column_order=optimized_column_order)  # type: ignore
             was_transformed = True
 
@@ -190,15 +192,14 @@
     if args.exclude:
         fts_query += " NOT " + " NOT ".join(fts_quote(args.exclude))
     args.filter_bindings["query"] = fts_query
     table = "(" + args.db[table].search_sql(include_rank=True) + ")"
     return table
 
 
-
 def fts_flexible_search(args, table="media") -> str:
     args.filter_bindings["query"] = " OR ".join(fts_quote(args.include))
     if args.exclude:
         args.filter_bindings["query"] += " NOT " + " NOT ".join(fts_quote(args.exclude))
     table = "(" + args.db[table].search_sql(include_rank=True) + ")"
     return table
```

### Comparing `xklb-2.1.9/xklb/dl_config.py` & `xklb-2.2.2/xklb/dl_config.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.9/xklb/dl_extract.py` & `xklb-2.2.2/xklb/dl_extract.py`

 * *Files 5% similar despite different names*

```diff
@@ -53,15 +53,14 @@
         metavar="KEY=VALUE",
         help="Add key/value pairs to override or extend downloader configuration",
     )
     parser.add_argument("--download-archive")
     parser.add_argument("--extra-media-data", default={}, nargs=1, action=utils.ArgparseDict, metavar="KEY=VALUE")
     parser.add_argument("--extra-playlist-data", default={}, nargs=1, action=utils.ArgparseDict, metavar="KEY=VALUE")
     parser.add_argument("--safe", "-safe", action="store_true", help="Skip generic URLs")
-    parser.add_argument("--playlist-files", action="store_true", help="Read playlists from text files")
 
     parser.add_argument("--subs", action="store_true")
     parser.add_argument("--auto-subs", "--autosubs", action="store_true")
     parser.add_argument("--subtitle-languages", "--subtitle-language", "--sl", action=utils.ArgparseList)
 
     parser.add_argument("--prefix", default=os.getcwd(), help=argparse.SUPPRESS)
     parser.add_argument("--ext", default="DEFAULT")
@@ -90,15 +89,15 @@
 
     parser.add_argument("--force", "-f", action="store_true", help=argparse.SUPPRESS)
     parser.add_argument("--ignore-errors", "--ignoreerrors", "-i", action="store_true", help=argparse.SUPPRESS)
     parser.add_argument("--db", "-db", help=argparse.SUPPRESS)
     parser.add_argument("--verbose", "-v", action="count", default=0)
 
     parser.add_argument("database", help=argparse.SUPPRESS)
-    parser.add_argument("playlists", nargs="*", help=argparse.SUPPRESS)
+    parser.add_argument("playlists", nargs="*", action=utils.ArgparseArgsOrStdin, help=argparse.SUPPRESS)
     args = parser.parse_intermixed_args()
 
     if args.duration:
         args.duration = utils.parse_human_to_sql(utils.human_to_seconds, "duration", args.duration)
 
     if not args.profile and not args.print:
         log.error("Download profile must be specified. Use one of: --video OR --audio OR --image")
@@ -201,42 +200,19 @@
         {LIMIT}
         """
 
     return query, args.filter_bindings
 
 
 def process_downloadqueue(args) -> List[dict]:
-    if args.playlist_files:
-        Path(args.database).touch()
-        playlist_files_data = set(utils.flatten(Path(p).read_text().splitlines() for p in args.playlists))
-
-        known_playlists = set()
-        if not args.force and len(playlist_files_data) > 9:
-            known_playlists = get_paths(args)
-        playlists = list(playlist_files_data - known_playlists)
-        log.warning(
-            "%s new - %s known = %s to download",
-            len(playlist_files_data),
-            len(known_playlists),
-            len(playlists),
-        )
-        random.shuffle(playlists)
-
-        media = []
-        for i, path in enumerate(playlists):
-            media.append({"path": path})
-            if args.limit and i >= int(args.limit):
-                break
-        playlists = []
-    else:
-        query, bindings = construct_query(args)
-        if args.print:
-            player.printer(args, query, bindings)
-            return []
-        media = list(args.db.query(query, bindings))
+    query, bindings = construct_query(args)
+    if args.print:
+        player.printer(args, query, bindings)
+        return []
+    media = list(args.db.query(query, bindings))
 
     if media and "blocklist" in args.db.table_names():
         media = utils.block_dicts_like_sql(media, [{d["key"]: d["value"]} for d in args.db["blocklist"].rows])
     if not media:
         utils.no_media_found()
 
     return media
```

### Comparing `xklb-2.1.9/xklb/fs_extract.py` & `xklb-2.2.2/xklb/fs_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.9/xklb/gdl_backend.py` & `xklb-2.2.2/xklb/gdl_backend.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.9/xklb/gdl_extract.py` & `xklb-2.2.2/xklb/gdl_extract.py`

 * *Files 14% similar despite different names*

```diff
@@ -37,18 +37,19 @@
 
     parser.add_argument("--timeout", "-T", help="Quit after x minutes")
     parser.add_argument("--verbose", "-v", action="count", default=0)
     parser.add_argument("--db", "-db", help=argparse.SUPPRESS)
 
     parser.add_argument("database")
     if action == SC.galleryadd:
-        parser.add_argument("--playlist-files", action="store_true", help="Read playlists from text files")
-        parser.add_argument("playlists", nargs="+", help=argparse.SUPPRESS)
+        parser.add_argument("--insert-only", action="store_true")
+        parser.add_argument("--insert-only-playlists", action="store_true")
+        parser.add_argument("playlists", nargs="*", action=utils.ArgparseArgsOrStdin, help=argparse.SUPPRESS)
 
-    args = parser.parse_args()
+    args = parser.parse_intermixed_args()
     args.action = action
 
     if args.db:
         args.database = args.db
     if action == SC.galleryadd:
         Path(args.database).touch()
     args.db = db.connect(args)
@@ -67,32 +68,35 @@
 
 
 def gallery_add(args=None) -> None:
     if args:
         sys.argv = ["galleryadd", *args]
 
     args = parse_args(SC.galleryadd, usage=usage.galleryadd)
-    if args.playlist_files:
-        args.playlists = list(utils.flatten([Path(p).read_text().splitlines() for p in args.playlists]))
 
     known_playlists = set()
     if not args.force and len(args.playlists) > 9:
         known_playlists = media.get_paths(args)
 
-    added_media_count = 0
+    added_media_count = len(args.playlists)
     for path in args.playlists:
         if path in known_playlists:
             log.info("[%s]: Already added. Skipping!", path)
             continue
 
         if args.safe and not gdl_backend.is_supported(args, path):
             log.info("[%s]: Skipping unsupported playlist (safe_mode)", path)
             continue
 
-        added_media_count += gdl_backend.get_playlist_metadata(args, path)
+        if args.insert_only:
+            args.db["media"].insert({"path": path}, alter=True, ignore=True, pk="path")
+        elif args.insert_only_playlists:
+            args.db["playlists"].insert({"path": path}, alter=True, ignore=True, pk="path")
+        else:
+            added_media_count += gdl_backend.get_playlist_metadata(args, path)
 
     LARGE_NUMBER = 100_000
     if not args.db["media"].detect_fts() or added_media_count > LARGE_NUMBER:
         db.optimize(args)
 
 
 def gallery_update(args=None) -> None:
```

### Comparing `xklb-2.1.9/xklb/gui.py` & `xklb-2.2.2/xklb/gui.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.9/xklb/history.py` & `xklb-2.2.2/xklb/history.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.9/xklb/hn_extract.py` & `xklb-2.2.2/xklb/hn_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.9/xklb/lb.py` & `xklb-2.2.2/xklb/lb.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,25 +11,27 @@
 from xklb.scripts.bigdirs import bigdirs
 from xklb.scripts.block import block
 from xklb.scripts.christen import christen
 from xklb.scripts.cluster_sort import cluster_sort
 from xklb.scripts.copy_play_counts import copy_play_counts
 from xklb.scripts.dedupe import dedupe
 from xklb.scripts.dedupe_db import dedupe_db
+from xklb.scripts.disk_usage import disk_usage
 from xklb.scripts.download_status import download_status
 from xklb.scripts.history import history
 from xklb.scripts.merge_dbs import merge_dbs
 from xklb.scripts.merge_online_local import merge_online_local
 from xklb.scripts.mining.extract_links import extract_links
 from xklb.scripts.mining.mpv_watchlater import mpv_watchlater
 from xklb.scripts.mining.nouns import nouns
 from xklb.scripts.mining.pushshift import pushshift_extract
 from xklb.scripts.mining.reddit_selftext import reddit_selftext
 from xklb.scripts.move_list import move_list
 from xklb.scripts.optimize_db import optimize_db
+from xklb.scripts.places_import import places_import
 from xklb.scripts.playback_control import playback_next, playback_now, playback_pause, playback_stop
 from xklb.scripts.playlists import playlists
 from xklb.scripts.redownload import redownload
 from xklb.scripts.relmv import relmv
 from xklb.scripts.scatter import scatter
 from xklb.scripts.streaming_tab_loader import streaming_tab_loader
 from xklb.search import search
@@ -86,21 +88,25 @@
       lb stop                  Stop all playback
       lb pause                 Pause all playback
 
     statistics:
       lb history               Show some playback statistics
       lb playlists             List added playlists
       lb download-status       Show download status
-      lb disk-usage            Print mount usage
+      lb disk-usage            Print disk usage
+      lb mount-stats           Print mount usage
 
     browser tabs:
       lb tabsadd               Create a tabs database; Add URLs
       lb tabs                  Open your tabs for the day
       lb surf                  Load browser tabs in a streaming way (stdin)
 
+    places:
+      lb places-import         Load POIs from Google Maps Google Takeout
+
     mining:
       lb reddit-selftext       db selftext external links -> db media table
       lb pushshift             Convert Pushshift jsonl.zstd -> reddit.db format (stdin)
       lb hnadd                 Create a hackernews database (this takes a few days)
 
       lb extract-links         Extract links from lists of web pages
 
@@ -217,16 +223,18 @@
 
     subp_playlist = add_parser(subparsers, "playlists", ["pl", "folders"])
     subp_playlist.set_defaults(func=playlists)
     subp_history = add_parser(subparsers, "history", ["hi", "log"])
     subp_history.set_defaults(func=history)
     subp_download_status = add_parser(subparsers, "download-status", ["ds", "dlstatus"])
     subp_download_status.set_defaults(func=download_status)
-    subp_usage = add_parser(subparsers, "disk-usage", ["du", "usage", "mount-stats"])
-    subp_usage.set_defaults(func=utils.mount_stats)
+    subp_disk_usage = add_parser(subparsers, "disk-usage", ["du", "usage", "diskusage"])
+    subp_disk_usage.set_defaults(func=disk_usage)
+    subp_mount_stats = add_parser(subparsers, "mount-stats", ["mu", "mount-usage", "mountstats"])
+    subp_mount_stats.set_defaults(func=utils.mount_stats)
 
     subp_playback_now = add_parser(subparsers, "now")
     subp_playback_now.set_defaults(func=playback_now)
     subp_playback_next = add_parser(subparsers, "next")
     subp_playback_next.set_defaults(func=playback_next)
     subp_playback_stop = add_parser(subparsers, "stop")
     subp_playback_stop.set_defaults(func=playback_stop)
@@ -236,14 +244,17 @@
     subp_tabsadd = add_parser(subparsers, "tabsadd")
     subp_tabsadd.set_defaults(func=tabs_add)
     subp_tabs = add_parser(subparsers, "tabs", ["tb"])
     subp_tabs.set_defaults(func=tabs)
     subp_surf = add_parser(subparsers, "surf")
     subp_surf.set_defaults(func=streaming_tab_loader)
 
+    subp_places_import = add_parser(subparsers, "places-import")
+    subp_places_import.set_defaults(func=places_import)
+
     subp_nouns = add_parser(subparsers, "nouns")
     subp_nouns.set_defaults(func=nouns)
     subp_cluster_sort = add_parser(subparsers, "cluster-sort", ["cs", "clustersort", "cluster_sort"])
     subp_cluster_sort.set_defaults(func=cluster_sort)
 
     subp_mpv_watchlater = add_parser(subparsers, "mpv-watchlater")
     subp_mpv_watchlater.set_defaults(func=mpv_watchlater)
```

### Comparing `xklb-2.1.9/xklb/media.py` & `xklb-2.2.2/xklb/media.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
         return False
     if known is None:
         return False
     return True
 
 
 def get(args, path):
-    return args.db.pop_dict("select * from media where path = ?", path)
+    return args.db.pop_dict("select * from media where path = ?", [path])
 
 
 def get_paths(args):
     tables = args.db.table_names()
 
     known_playlists = set()
     if "media" in tables:
```

### Comparing `xklb-2.1.9/xklb/play_actions.py` & `xklb-2.2.2/xklb/play_actions.py`

 * *Files 6% similar despite different names*

```diff
@@ -86,14 +86,16 @@
     parser.add_argument("--created-before", help=argparse.SUPPRESS)
     parser.add_argument("--changed-within", "--modified-within", help=argparse.SUPPRESS)
     parser.add_argument("--changed-before", "--modified-before", help=argparse.SUPPRESS)
     parser.add_argument("--played-within", help=argparse.SUPPRESS)
     parser.add_argument("--played-before", help=argparse.SUPPRESS)
     parser.add_argument("--deleted-within", help=argparse.SUPPRESS)
     parser.add_argument("--deleted-before", help=argparse.SUPPRESS)
+    parser.add_argument("--downloaded-within", help=argparse.SUPPRESS)
+    parser.add_argument("--downloaded-before", help=argparse.SUPPRESS)
 
     parser.add_argument(
         "--chromecast-device",
         "--cast-to",
         "-t",
         default=default_chromecast or "",
         help=argparse.SUPPRESS,
@@ -142,14 +144,18 @@
 
     parser.add_argument("--start", "-vs", help=argparse.SUPPRESS)
     parser.add_argument("--end", "-ve", help=argparse.SUPPRESS)
     parser.add_argument("--mpv-socket", default=consts.DEFAULT_MPV_SOCKET, help=argparse.SUPPRESS)
     parser.add_argument("--watch-later-directory", default=consts.DEFAULT_MPV_WATCH_LATER, help=argparse.SUPPRESS)
     parser.add_argument("--subtitle-mix", default=consts.DEFAULT_SUBTITLE_MIX, help=argparse.SUPPRESS)
 
+    parser.add_argument("--no-video", "-vn", action="store_true", help=argparse.SUPPRESS)
+    parser.add_argument("--no-audio", "-an", action="store_true", help=argparse.SUPPRESS)
+    parser.add_argument("--no-subtitle", "-sn", action="store_true", help=argparse.SUPPRESS)
+
     parser.add_argument("--override-player", "--player", "-player", help=argparse.SUPPRESS)
     parser.add_argument("--player-args-sub", "-player-sub", nargs="*", default=DEFAULT_PLAYER_ARGS_SUB)
     parser.add_argument("--player-args-no-sub", "-player-no-sub", nargs="*", default=DEFAULT_PLAYER_ARGS_NO_SUB)
     parser.add_argument("--transcode", action="store_true", help=argparse.SUPPRESS)
     parser.add_argument("--transcode-audio", action="store_true", help=argparse.SUPPRESS)
 
     parser.add_argument("--post-action", "--action", "-k", default="keep", help=argparse.SUPPRESS)
@@ -262,66 +268,80 @@
     return args
 
 
 def construct_query(args) -> Tuple[str, dict]:
     m_columns = db.columns(args, "media")
 
     args.filter_sql = []
+    args.aggregate_filter_sql = []
     args.filter_bindings = {}
 
     if args.duration:
         args.filter_sql.append(" and duration IS NOT NULL " + args.duration)
     if args.size:
         args.filter_sql.append(" and size IS NOT NULL " + args.size)
     if args.duration_from_size:
         args.filter_sql.append(
-            " and size IS NOT NULL and duration in (select distinct duration from m where 1=1 "
+            " and size IS NOT NULL and duration in (select distinct duration from media where 1=1 "
             + args.duration_from_size
             + ")",
         )
 
-    args.filter_sql.extend([" and " + w for w in args.where])
+    if args.no_video:
+        args.filter_sql.append(" and video_count=0 ")
+    if args.no_audio:
+        args.filter_sql.append(" and audio_count=0 ")
+    if args.no_subtitle:
+        args.filter_sql.append(" and subtitle_count=0 ")
 
     def ii(string):
         if string.isdigit():
             return string + " minutes"
         return string.replace("mins", "minutes").replace("secs", "seconds")
 
     if args.created_within:
-        args.filter_sql.append(
+        args.aggregate_filter_sql.append(
             f"and time_created > cast(STRFTIME('%s', datetime( 'now', '-{ii(args.created_within)}')) as int)",
         )
     if args.created_before:
-        args.filter_sql.append(
+        args.aggregate_filter_sql.append(
             f"and time_created < cast(STRFTIME('%s', datetime( 'now', '-{ii(args.created_before)}')) as int)",
         )
     if args.changed_within:
-        args.filter_sql.append(
+        args.aggregate_filter_sql.append(
             f"and time_modified > cast(STRFTIME('%s', datetime( 'now', '-{ii(args.changed_within)}')) as int)",
         )
     if args.changed_before:
-        args.filter_sql.append(
+        args.aggregate_filter_sql.append(
             f"and time_modified < cast(STRFTIME('%s', datetime( 'now', '-{ii(args.changed_before)}')) as int)",
         )
     if args.played_within:
-        args.filter_sql.append(
+        args.aggregate_filter_sql.append(
             f"and time_last_played > cast(STRFTIME('%s', datetime( 'now', '-{ii(args.played_within)}')) as int)",
         )
     if args.played_before:
-        args.filter_sql.append(
+        args.aggregate_filter_sql.append(
             f"and time_last_played < cast(STRFTIME('%s', datetime( 'now', '-{ii(args.played_before)}')) as int)",
         )
     if args.deleted_within:
-        args.filter_sql.append(
+        args.aggregate_filter_sql.append(
             f"and time_deleted > cast(STRFTIME('%s', datetime( 'now', '-{ii(args.deleted_within)}')) as int)",
         )
     if args.deleted_before:
-        args.filter_sql.append(
+        args.aggregate_filter_sql.append(
             f"and time_deleted < cast(STRFTIME('%s', datetime( 'now', '-{ii(args.deleted_before)}')) as int)",
         )
+    if args.downloaded_within:
+        args.aggregate_filter_sql.append(
+            f"and time_downloaded > cast(STRFTIME('%s', datetime( 'now', '-{ii(args.downloaded_within)}')) as int)",
+        )
+    if args.downloaded_before:
+        args.aggregate_filter_sql.append(
+            f"and time_downloaded < cast(STRFTIME('%s', datetime( 'now', '-{ii(args.downloaded_before)}')) as int)",
+        )
 
     args.table = "media"
     if args.db["media"].detect_fts() and not args.no_fts:
         if args.include:
             args.table = db.fts_search(args)
             m_columns = {**m_columns, "rank": int}
         elif args.exclude:
@@ -350,14 +370,16 @@
             if "time_deleted" in m_columns and "time_deleted" not in " ".join(sys.argv)
             else ""
         )
         args.filter_sql.append(
             f"and m.id in (select id from media {where_not_deleted} order by random() limit {limit})",
         )
 
+    aggregate_filter_columns = ["time_first_played", "time_last_played", "play_count", "playhead"]
+
     cols = args.cols or ["path", "title", "duration", "size", "subtitle_count", "is_dir", "rank"]
     args.select = [c for c in cols if c in m_columns or c in ["*"]]
     if args.action == SC.read and "tags" in m_columns:
         args.select += "cast(length(tags) / 4.2 / 220 * 60 as INT) + 10 duration"
     args.select_sql = "\n        , ".join(args.select)
     args.limit_sql = "LIMIT " + str(args.limit) if args.limit else ""
     args.offset_sql = f"OFFSET {args.skip}" if args.skip and args.limit else ""
@@ -369,33 +391,34 @@
                 , MAX(h.time_played) time_last_played
                 , FIRST_VALUE(h.playhead) OVER (PARTITION BY h.media_id ORDER BY h.time_played DESC) playhead
                 , *
             FROM {args.table} m
             LEFT JOIN history h on h.media_id = m.id
             WHERE 1=1
                 {player.filter_args_sql(args, m_columns)}
+                {" ".join(args.filter_sql)}
+                {" ".join([" and " + w for w in args.where if not any(a in w for a in aggregate_filter_columns)])}
             GROUP BY m.id, m.path
         )
         SELECT
             {args.select_sql}
             , play_count
             , time_first_played
             , time_last_played
             , playhead
         FROM m
         WHERE 1=1
-            {" ".join(args.filter_sql)}
+            {" ".join(args.aggregate_filter_sql)}
+            {" ".join([" and " + w for w in args.where if any(a in w for a in aggregate_filter_columns)])}
         ORDER BY 1=1
             , {args.sort}
         {args.limit_sql} {args.offset_sql}
     """
 
-    args.filter_sql = [
-        s for s in args.filter_sql if "id" not in s
-    ]  # only use random id constraint in first query
+    args.filter_sql = [s for s in args.filter_sql if "id" not in s]  # only use random id constraint in first query
 
     return query, args.filter_bindings
 
 
 def chromecast_play(args, m) -> None:
     if args.action in (SC.watch):
         catt_log = player.watch_chromecast(args, m, subtitles_file=safe_unpack(subtitle.get_subtitle_paths(m["path"])))
@@ -496,30 +519,30 @@
 
     m["now_playing"] = now_playing(m["path"])
 
     return m
 
 
 def save_playhead(args, m, start_time):
-    m_columns = db.columns(args, "media")
-    if "playhead" in m_columns:
-        playhead = utils.get_playhead(
-            args,
-            m["original_path"],
-            start_time,
-            existing_playhead=m.get("playhead"),
-            media_duration=m.get("duration"),
-        )
-        if playhead:
-            history.add(args, [m["original_path"]], playhead=playhead)
+    playhead = utils.get_playhead(
+        args,
+        m["original_path"],
+        start_time,
+        existing_playhead=m.get("playhead"),
+        media_duration=m.get("duration"),
+    )
+    log.debug("save_playhead %s", playhead)
+    if playhead:
+        history.add(args, [m["original_path"]], playhead=playhead)
 
 
 def play(args, m, media_len) -> None:
     t = utils.Timer()
     print(m["now_playing"])
+    log.debug(m)
     log.debug("now_playing: %s", t.elapsed())
 
     args.player = player.parse(args, m)
     log.debug("player.parse: %s", t.elapsed())
 
     if args.interdimensional_cable:
         player.socket_play(args, m)
```

### Comparing `xklb-2.1.9/xklb/player.py` & `xklb-2.2.2/xklb/player.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,19 +35,20 @@
     return player
 
 
 def calculate_duration(args, m) -> Tuple[int, int]:
     start = 0
     end = m.get("duration", 0)
     minimum_duration = 7 * 60
+    playhead = m.get("playhead")
+    if playhead:
+        start = playhead
 
     duration = m.get("duration", 20 * 60)
     if args.start:
-        playhead = m.get("playhead")
-
         if args.start.isnumeric() and int(args.start) > 0:
             start = int(args.start)
         elif "%" in args.start:
             start_percent = int(args.start[:-1])
             start = int(duration * start_percent / 100)
         elif playhead and any([end == 0, end > minimum_duration]):
             start = playhead
@@ -62,14 +63,15 @@
             end_percent = int(args.end[:-1])
             end = int(duration * end_percent / 100)
         elif "+" in args.end:
             end = int(args.start) + int(args.end)
         else:
             end = int(args.end)
 
+    log.debug("calculate_duration: %s -- %s", start, end)
     return start, end
 
 
 def get_browser() -> Optional[str]:
     default_application = cmd("xdg-mime", "query", "default", "text/html").stdout
     return which(default_application.replace(".desktop", ""))
 
@@ -117,15 +119,17 @@
         if getattr(args, "crop", None):
             player.extend(["--panscan=1.0"])
 
         if args.action in (SC.watch, SC.listen, SC.search) and m:
             start, end = calculate_duration(args, m)
             if end != 0:
                 if start != 0:
-                    player.extend([f"--start={start}", "--no-save-position-on-quit"])
+                    player.extend([f"--start={start}"])
+                    if args.start:
+                        player.extend(["--no-save-position-on-quit"])
                 if end != m["duration"]:
                     player.extend([f"--end={end}"])
 
         if args.action == SC.watch and m and m.get("subtitle_count") is not None:
             if m["subtitle_count"] > 0:
                 player.extend(args.player_args_sub)
             elif m["size"] > 500 * 1000000:  # 500 MB
@@ -402,29 +406,28 @@
         candidate = new_candidate
         query = f"""WITH m as (
                 SELECT
                     SUM(CASE WHEN h.done = 1 THEN 1 ELSE 0 END) play_count
                     , MIN(h.time_played) time_first_played
                     , MAX(h.time_played) time_last_played
                     , FIRST_VALUE(h.playhead) OVER (PARTITION BY h.media_id ORDER BY h.time_played DESC) playhead
-                    , *
+                    , {args.select_sql}
                 FROM media m
                 LEFT JOIN history h on h.media_id = m.id
+                WHERE 1=1
+                    and path like :candidate
+                    {'' if args.play_in_order >= consts.SIMILAR_NO_FILTER_NO_FTS else f'and m.id in (select id from {args.table})'}
+                    {filter_args_sql(args, m_columns)}
+                    {'' if args.play_in_order >= consts.SIMILAR_NO_FILTER else (" ".join(args.filter_sql) or '')}
+                    {"and path not in ({})".format(",".join([f":ignore_path{i}" for i in range(len(ignore_paths))])) if len(ignore_paths) > 0 else ''}
                 GROUP BY m.id, m.path
             )
             SELECT
-                {args.select_sql}
-                , play_count
+                *
             FROM m
-            WHERE 1=1
-                and path like :candidate
-                {'' if args.play_in_order >= consts.SIMILAR_NO_FILTER_NO_FTS else f'and m.id in (select id from {args.table})'}
-                {filter_args_sql(args, m_columns)}
-                {'' if args.play_in_order >= consts.SIMILAR_NO_FILTER else (" ".join(args.filter_sql) or '')}
-                {"and path not in ({})".format(",".join([f":ignore_path{i}" for i in range(len(ignore_paths))])) if len(ignore_paths) > 0 else ''}
             ORDER BY play_count, path
             LIMIT 1000
             """
 
         ignore_path_params = {f"ignore_path{i}": value for i, value in enumerate(ignore_paths)}
         bindings = {"candidate": candidate + "%", **ignore_path_params}
         if args.play_in_order >= consts.SIMILAR_NO_FILTER:
@@ -464,28 +467,26 @@
 
     query = f"""WITH m as (
             SELECT
                 SUM(CASE WHEN h.done = 1 THEN 1 ELSE 0 END) play_count
                 , MIN(h.time_played) time_first_played
                 , MAX(h.time_played) time_last_played
                 , FIRST_VALUE(h.playhead) OVER (PARTITION BY h.media_id ORDER BY h.time_played DESC) playhead
-                , *
-            FROM media m
+                , {args.select_sql}
+                , rank
+            FROM {args.table} m
             LEFT JOIN history h on h.media_id = m.id
+            WHERE 1=1
+                and path != :path
+                {filter_args_sql(args, m_columns)}
+                {'' if args.related >= consts.RELATED_NO_FILTER else (" ".join(args.filter_sql) or '')}
             GROUP BY m.id, m.path
         )
-        SELECT
-            {args.select_sql}, rank
-            , play_count
+        SELECT *
         FROM m
-        WHERE 1=1
-            and path != :path
-            and m.id in (select id from {args.table})
-            {filter_args_sql(args, m_columns)}
-            {'' if args.related >= consts.RELATED_NO_FILTER else (" ".join(args.filter_sql) or '')}
         ORDER BY play_count
             , m.path like "http%"
             , {'rank' if 'sort' in args.defaults else f'ntile(1000) over (order by rank), {args.sort}'}
             , path
         {"LIMIT " + str(args.limit - 1) if args.limit else ""} {args.offset_sql}
         """
     bindings = {"path": m["path"]}
@@ -517,28 +518,26 @@
 
     query = f"""WITH m as (
             SELECT
                 SUM(CASE WHEN h.done = 1 THEN 1 ELSE 0 END) play_count
                 , MIN(h.time_played) time_first_played
                 , MAX(h.time_played) time_last_played
                 , FIRST_VALUE(h.playhead) OVER (PARTITION BY h.media_id ORDER BY h.time_played DESC) playhead
-                , *
+                , {args.select_sql}
             FROM media m
             LEFT JOIN history h on h.media_id = m.id
+            WHERE 1=1
+                and m.id in (select id from {args.table})
+                {filter_args_sql(args, m_columns)}
+                {filter_paths}
+                {'' if args.related >= consts.DIRS_NO_FILTER else (" ".join(args.filter_sql) or '')}
             GROUP BY m.id, m.path
         )
-        SELECT
-            {args.select_sql}
-            , play_count
+        SELECT *
         FROM m
-        WHERE 1=1
-            and m.id in (select id from {args.table})
-            {filter_args_sql(args, m_columns)}
-            {filter_paths}
-            {'' if args.related >= consts.DIRS_NO_FILTER else (" ".join(args.filter_sql) or '')}
         ORDER BY play_count
             , m.path LIKE "http%"
             {'' if 'sort' in args.defaults else ', ' + args.sort}
             , path
         {"LIMIT 10000" if 'limit' in args.defaults else str(args.limit)} {args.offset_sql}
     """
     subpath_params = {f"subpath{i}": value + "%" for i, value in enumerate(dirs)}
@@ -907,14 +906,36 @@
         historical_daily = statistics.mean((d["duration_sum"] or 0) for d in historical_usage(args))
     except statistics.StatisticsError:
         return duration
 
     return duration / historical_daily * 86400 * 30.42
 
 
+def filter_deleted(media):
+    http_list = []
+    local_list = []
+    nonexistent_local_paths = []
+
+    for i, m in enumerate(media):
+        path = m["path"]
+        if path.startswith("http"):
+            http_list.append(m)
+            continue
+
+        if len(local_list) == 50 and len(nonexistent_local_paths) <= 2:
+            return local_list + http_list + media[i:], nonexistent_local_paths
+
+        if os.path.exists(path):
+            local_list.append(m)
+        else:
+            nonexistent_local_paths.append(path)
+
+    return local_list + http_list, nonexistent_local_paths
+
+
 def media_printer(args, media) -> None:
     if args.verbose >= consts.LOG_DEBUG and args.cols and "*" in args.cols:
         breakpoint()
 
     if not media:
         utils.no_media_found()
 
@@ -946,56 +967,54 @@
             marked = mark_media_deleted(args, [d["path"] for d in media])
             log.warning(f"Marked {marked} metadata records as deleted")
         if "w" in args.print:
             marked = history.add(args, [d["path"] for d in media])
             log.warning(f"Marked {marked} metadata records as watched")
 
     if "f" in args.print:
-        if args.limit == 1:
-            path = media[0]["path"]
-            if not Path(path).exists():
-                mark_media_deleted(args, path)
+        if len(media) <= 1000:
+            media, deleted_paths = filter_deleted(media)
+            mark_media_deleted(args, deleted_paths)
+            if len(media) == 0:
                 raise FileNotFoundError
-            utils.pipe_print(path)
-            return
-        else:
-            if not args.cols:
-                args.cols = ["path"]
 
-            selected_cols = [{k: d.get(k, None) for k in args.cols} for d in media]
-            virtual_csv = StringIO()
-            wr = csv.writer(virtual_csv, quoting=csv.QUOTE_NONE)
-            wr = csv.DictWriter(virtual_csv, fieldnames=args.cols)
-            wr.writerows(selected_cols)
-
-            virtual_csv.seek(0)
-            for line in virtual_csv.readlines():
-                if args.moved:
-                    utils.pipe_print(line.strip().replace(args.moved[0], "", 1))
-                else:
-                    utils.pipe_print(line.strip())
+        if not args.cols:
+            args.cols = ["path"]
+
+        selected_cols = [{k: d.get(k, None) for k in args.cols} for d in media]
+        virtual_csv = StringIO()
+        wr = csv.writer(virtual_csv, quoting=csv.QUOTE_NONE)
+        wr = csv.DictWriter(virtual_csv, fieldnames=args.cols)
+        wr.writerows(selected_cols)
+
+        virtual_csv.seek(0)
+        for line in virtual_csv.readlines():
             if args.moved:
-                moved_media(args, [d["path"] for d in media], *args.moved)
-                return
+                utils.pipe_print(line.strip().replace(args.moved[0], "", 1))
+            else:
+                utils.pipe_print(line.strip())
+        if args.moved:
+            moved_media(args, [d["path"] for d in media], *args.moved)
             return
+        return
     else:
         tbl = deepcopy(media)
         utils.col_resize(tbl, "path", 22)
         utils.col_resize(tbl, "title", 11)
 
         utils.col_naturalsize(tbl, "size")
         utils.col_naturalsize(tbl, "avg_size")
         utils.col_duration(tbl, "duration")
         utils.col_duration(tbl, "avg_duration")
         utils.col_duration(tbl, "cadence_adj_duration")
 
         for t in consts.TIME_COLUMNS:
             utils.col_naturaldate(tbl, t)
 
-        print(tabulate(tbl, tablefmt="fancy_grid", headers="keys", showindex=False))
+        print(tabulate(tbl, tablefmt=consts.TABULATE_STYLE, headers="keys", showindex=False))
 
         if len(media) > 1:
             print(f"{len(media)} media" + (f" (limited to {args.limit})" if args.limit else ""))
 
         if duration > 0:
             duration = human_time(duration)
             if "a" not in args.print:
```

### Comparing `xklb-2.1.9/xklb/playlists.py` & `xklb-2.2.2/xklb/playlists.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.9/xklb/praw_extract.py` & `xklb-2.2.2/xklb/praw_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.9/xklb/search.py` & `xklb-2.2.2/xklb/search.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,15 +82,15 @@
         print(json.dumps(tbl, indent=3))
     elif args.csv:
         utils.write_csv_to_stdout(tbl)
     elif args.table:
         tbl = utils.col_resize(tbl, "path", 20)
         tbl = utils.col_resize(tbl, "text", 35)
         tbl = utils.list_dict_filter_bool(tbl)
-        print(tabulate(tbl, tablefmt="fancy_grid", headers="keys", showindex=False))
+        print(tabulate(tbl, tablefmt=consts.TABULATE_STYLE, headers="keys", showindex=False))
         print(f"{len(captions)} captions")
     else:
         print(f"{len(captions)} captions")
         for path, path_group in groupby(tbl, key=lambda x: x["path"]):
             path_group = list(path_group)
             title = path_group[0].get("title")
             print(" - ".join(utils.concat(title, path)))
```

### Comparing `xklb-2.1.9/xklb/subtitle.py` & `xklb-2.2.2/xklb/subtitle.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.9/xklb/tabs_actions.py` & `xklb-2.2.2/xklb/tabs_actions.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.9/xklb/tabs_extract.py` & `xklb-2.2.2/xklb/tabs_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.9/xklb/tube_backend.py` & `xklb-2.2.2/xklb/tube_backend.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.9/xklb/tube_extract.py` & `xklb-2.2.2/xklb/tube_extract.py`

 * *Files 14% similar despite different names*

```diff
@@ -22,15 +22,15 @@
         metavar="KEY=VALUE",
         help="Add key/value pairs to override or extend default downloader configuration",
     )
     parser.add_argument("--download-archive", default="~/.local/share/yt_archive.txt")
     parser.add_argument("--safe", "-safe", action="store_true", help="Skip generic URLs")
     parser.add_argument("--no-sanitize", "-s", action="store_true", help="Don't sanitize some common URL parameters")
     parser.add_argument("--extra", "-extra", action="store_true", help="Get full metadata (takes a lot longer)")
-    parser.add_argument("--playlist-files", action="store_true", help="Read playlists from text files")
+
     parser.add_argument(
         "--force",
         "-f",
         action="store_true",
         help="Fetch metadata for paths even if they are already in the media table",
     )
     parser.add_argument("--subs", action="store_true")
@@ -42,17 +42,19 @@
 
     parser.add_argument("--timeout", "-T", help="Quit after x minutes")
     parser.add_argument("--verbose", "-v", action="count", default=0)
     parser.add_argument("--db", "-db", help=argparse.SUPPRESS)
 
     parser.add_argument("database")
     if action == SC.tubeadd:
-        parser.add_argument("playlists", nargs="+", help=argparse.SUPPRESS)
+        parser.add_argument("--insert-only", action="store_true")
+        parser.add_argument("--insert-only-playlists", action="store_true")
+        parser.add_argument("playlists", nargs="*", action=utils.ArgparseArgsOrStdin, help=argparse.SUPPRESS)
 
-    args = parser.parse_args()
+    args = parser.parse_intermixed_args()
     args.action = action
 
     if args.db:
         args.database = args.db
     if action == SC.tubeadd:
         Path(args.database).touch()
     args.db = db.connect(args)
@@ -71,31 +73,34 @@
 
 
 def tube_add(args=None) -> None:
     if args:
         sys.argv = ["tubeadd", *args]
 
     args = parse_args(SC.tubeadd, usage=usage.tubeadd)
-    if args.playlist_files:
-        args.playlists = list(utils.flatten([Path(p).read_text().splitlines() for p in args.playlists]))
 
     known_playlists = set()
     if not args.force and len(args.playlists) > 9:
         known_playlists = media.get_paths(args)
 
     for path in args.playlists:
         if args.safe and not tube_backend.is_supported(path):
             log.info("[%s]: Skipping unsupported playlist (safe_mode)", path)
             continue
 
         if path in known_playlists:
             log.info("[%s]: Already added. Skipping!", path)
             continue
 
-        tube_backend.get_playlist_metadata(args, path, tube_backend.tube_opts(args))
+        if args.insert_only:
+            args.db["media"].insert({"path": path}, alter=True, ignore=True, pk="path")
+        elif args.insert_only_playlists:
+            args.db["playlists"].insert({"path": path}, alter=True, ignore=True, pk="path")
+        else:
+            tube_backend.get_playlist_metadata(args, path, tube_backend.tube_opts(args))
 
         if args.extra:
             log.warning("[%s]: Getting extra metadata", path)
             tube_backend.get_extra_metadata(args, path)
 
     LARGE_NUMBER = 100_000
     if not args.db["media"].detect_fts() or tube_backend.added_media_count > LARGE_NUMBER:
```

### Comparing `xklb-2.1.9/xklb/usage.py` & `xklb-2.2.2/xklb/usage.py`

 * *Files 2% similar despite different names*

```diff
@@ -101,14 +101,20 @@
 fsupdate = """library fsupdate DATABASE
 
     Update each path previously saved:
 
         library fsupdate video.db
 """
 
+places_import = """library places-import DATABASE PATHS ...
+
+Load POIs from Google Maps Google Takeout
+
+"""
+
 hnadd = """library hnadd [--oldest] DATABASE
 
     Fetch latest stories first:
 
         library hnadd hn.db -v
         Fetching 154873 items (33212696 to 33367569)
         Saving comment 33367568
@@ -702,15 +708,15 @@
 
     Create a dl database / add links to an existing database
 
         library tubeadd dl.db https://www.youdl.com/c/BranchEducation/videos
 
     Add links from a line-delimited file
 
-        library tubeadd reddit.db --playlist-file ./my_yt_subscriptions.txt
+        cat ./my_yt_subscriptions.txt | library tubeadd reddit.db -
 
     Add metadata to links already in a database table
 
         library tubeadd --force reddit.db (sqlite-utils --raw-lines reddit.db 'select path from media')
 
     Files will be saved to <download prefix>/<extractor>/
 
@@ -746,17 +752,17 @@
         library tubeupdate educational.db --extra https://www.youtube.com/channel/UCBsEUcR-ezAuxB2WlfeENvA/videos
 """
 
 galleryadd = """library galleryadd DATABASE URLS
 
 Add gallery_dl URLs to download later or periodically update
 
-Passing the `--playlist-files` flag will treat each URL as a local file to read URLs from
+If you have many URLs use stdin
 
-    library galleryadd my.db ./my-favorite-manhwa.txt
+    cat ./my-favorite-manhwa.txt | library galleryadd my.db --insert-only
 """
 
 galleryupdate = """library galleryupdate DATABASE URLS
 
 Check previously saved gallery_dl URLs for new content
 """
 
@@ -770,14 +776,45 @@
 
     lb bigdirs video.db --folder-size=+10G --lower 400 --upper 14000
 
     lb bigdirs video.db --depth 5
     lb bigdirs video.db --depth 7
 """
 
+disk_usage = """library disk-usage DATABASE [--sort-by size | count] [--depth DEPTH] [PATH / SUBSTRING SEARCH]
+
+    Only include files smaller than 1kib
+
+        library disk-usage du.db --size=-1Ki
+        lb du du.db -S-1Ki
+        | path                                  |      size |   count |
+        |---------------------------------------|-----------|---------|
+        | /home/xk/github/xk/lb/__pycache__/    | 620 Bytes |       1 |
+        | /home/xk/github/xk/lb/.github/        |    1.7 kB |       4 |
+        | /home/xk/github/xk/lb/__pypackages__/ |    1.4 MB |    3519 |
+        | /home/xk/github/xk/lb/xklb/           |    4.4 kB |      12 |
+        | /home/xk/github/xk/lb/tests/          |    3.2 kB |       9 |
+        | /home/xk/github/xk/lb/.git/           |  782.4 kB |    2276 |
+        | /home/xk/github/xk/lb/.pytest_cache/  |    1.5 kB |       5 |
+        | /home/xk/github/xk/lb/.ruff_cache/    |   19.5 kB |     100 |
+        | /home/xk/github/xk/lb/.gitattributes  | 119 Bytes |         |
+        | /home/xk/github/xk/lb/.mypy_cache/    | 280 Bytes |       4 |
+        | /home/xk/github/xk/lb/.pdm-python     |  15 Bytes |         |
+
+    Only include files with a specific depth
+
+        library disk-usage du.db --depth 19
+        lb du du.db -d 19
+        | path                                                                                                                                                                |     size |
+        |---------------------------------------------------------------------------------------------------------------------------------------------------------------------|----------|
+        | /home/xk/github/xk/lb/__pypackages__/3.11/lib/jedi/third_party/typeshed/third_party/2and3/requests/packages/urllib3/packages/ssl_match_hostname/__init__.pyi        | 88 Bytes |
+        | /home/xk/github/xk/lb/__pypackages__/3.11/lib/jedi/third_party/typeshed/third_party/2and3/requests/packages/urllib3/packages/ssl_match_hostname/_implementation.pyi | 81 Bytes |
+
+"""
+
 christen = """library christen DATABASE [--run]
 
     Rename files to be somewhat normalized
 
     Default mode is dry-run
 
         library christen fs.db
```

### Comparing `xklb-2.1.9/xklb/utils.py` & `xklb-2.2.2/xklb/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -773,14 +773,23 @@
 
         except ValueError as ex:
             msg = f'Could not parse argument "{values}" as k1=1 k2=2 format {ex}'
             raise argparse.ArgumentError(self, msg) from ex
         setattr(args, self.dest, d)
 
 
+class ArgparseArgsOrStdin(argparse.Action):
+    def __call__(self, parser, namespace, values, option_string=None):
+        if values == ["-"] or not values:
+            lines = sys.stdin.readlines()
+        else:
+            lines = values
+        setattr(namespace, self.dest, lines)
+
+
 def filter_namespace(args, config_opts) -> Optional[Dict]:
     return dict_filter_bool({k: v for k, v in args.__dict__.items() if k in config_opts})
 
 
 def clear_input() -> None:
     if platform.system() == "Linux":
         from termios import TCIFLUSH, tcflush
@@ -1035,15 +1044,17 @@
     md5 = path_to_mpv_watchlater_md5(path)
     metadata_path = Path(args.watch_later_directory, md5)
     try:
         mpv_playhead = safe_int(mpv_watchlater_value(metadata_path, "start"))
     except Exception:
         mpv_playhead = None
 
-    for playhead in sorted([mpv_playhead or 0, python_playhead], reverse=True):
+    log.debug("mpv_playhead %s", mpv_playhead)
+    log.debug("python_playhead %s", python_playhead)
+    for playhead in [mpv_playhead or 0, python_playhead]:
         if playhead > 0 and (media_duration is None or media_duration >= playhead):
             return playhead
     return None
 
 
 class Timer:
     def __init__(self):
```

### Comparing `xklb-2.1.9/xklb/scripts/bigdirs.py` & `xklb-2.2.2/xklb/scripts/bigdirs.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import argparse, os
 from pathlib import Path
 from typing import Dict, List
 
 from tabulate import tabulate
 
-from xklb import db, history, usage, utils
+from xklb import consts, db, history, usage, utils
 from xklb.utils import log
 
 
 def parse_args() -> argparse.Namespace:
     parser = argparse.ArgumentParser(
         prog="library bigdirs",
         usage=usage.bigdirs,
@@ -124,15 +124,15 @@
     media = list(
         args.db.query(
             f"""
         SELECT
             path
             , size
             {', time_deleted' if 'time_deleted' in m_columns else ''}
-            , time_played
+            , MAX(h.time_played) time_played
         FROM media m
         LEFT JOIN history h on h.media_id = m.id
         WHERE 1=1
             {'and time_downloaded > 0' if 'time_downloaded' in m_columns else ''}
             {" ".join(args.filter_sql)}
         GROUP BY m.id
         ORDER BY path
@@ -180,14 +180,14 @@
 
     if args.limit:
         tbl = tbl[-int(args.limit) :]
 
     tbl = utils.list_dict_filter_bool(tbl, keep_0=False)
     tbl = utils.col_resize(tbl, "path", 50)
     tbl = utils.col_naturalsize(tbl, "size")
-    print(tabulate(tbl, tablefmt="fancy_grid", headers="keys", showindex=False))
+    print(tabulate(tbl, tablefmt=consts.TABULATE_STYLE, headers="keys", showindex=False))
     if not args.limit:
         print(f"{len(tbl)} folders found")
 
 
 if __name__ == "__main__":
     bigdirs()
```

### Comparing `xklb-2.1.9/xklb/scripts/block.py` & `xklb-2.2.2/xklb/scripts/block.py`

 * *Files 1% similar despite different names*

```diff
@@ -161,15 +161,15 @@
             }
             for d in tbl
         ]
         tbl = [{k: v for k, v in d.items() if k not in ("title", "path", "webpath")} for d in tbl]
         tbl = utils.col_resize(tbl, "title_path", 40)
         tbl = utils.col_naturalsize(tbl, "size")
         tbl = utils.col_naturaldate(tbl, "time_deleted")
-        print(tabulate(tbl, tablefmt="fancy_grid", headers="keys", showindex=False))
+        print(tabulate(tbl, tablefmt=consts.TABULATE_STYLE, headers="keys", showindex=False))
         if utils.confirm(f"{len(matching_media)} media matching {p}. Add to blocklist?"):
             add_to_blocklist(args, p)
         else:
             continue
 
         paths_to_delete = [
             d["path"] for d in matching_media if d["time_deleted"] == 0 and not d["path"].startswith("http")
```

### Comparing `xklb-2.1.9/xklb/scripts/christen.py` & `xklb-2.2.2/xklb/scripts/christen.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.9/xklb/scripts/cluster_sort.py` & `xklb-2.2.2/xklb/scripts/cluster_sort.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.9/xklb/scripts/copy_play_counts.py` & `xklb-2.2.2/xklb/scripts/copy_play_counts.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import argparse
 from pathlib import Path
 
-from xklb import db, history, usage, utils
+from xklb import consts, db, history, usage, utils
 from xklb.scripts.dedupe_db import dedupe_rows
 from xklb.utils import log
 
 
 def parse_args() -> argparse.Namespace:
     parser = argparse.ArgumentParser(prog="library copy-play-counts", usage=usage.copy_play_counts)
     parser.add_argument("database")
@@ -22,77 +22,81 @@
     args.db = db.connect(args)
     log.info(utils.dict_filter_bool(args.__dict__))
 
     return args
 
 
 def copy_play_count(args, source_db) -> None:
-    args.db.attach("src", Path(source_db).resolve())
+    s_db = db.connect(argparse.Namespace(database=source_db, verbose=args.verbose))
+    m_columns = s_db["media"].columns_dict
 
     copy_counts = []
     try:
         # TODO delete after 2024-06-01
         old_schema = list(
-            args.db.query(
-                """
+            s_db.query(
+                f"""
                 SELECT
-                    path, play_count, time_played, playhead
+                    path
+                    , {', '.join(s for s in ['play_count', 'time_played', 'playhead'] if s in m_columns)}
                 FROM
-                    src.media
+                    media
                 WHERE
-                    src.media.play_count > 0
-                    OR
-                    src.media.playhead > 0
+                    {' OR '.join(f"media.{s} > 0" for s in ['play_count', 'time_played', 'playhead'] if s in m_columns)}
                 """,
             ),
         )
 
         new_schema = []
         for d in old_schema:
-            if d["playhead"] is None or d["playhead"] == 0:
-                new_schema.append(
-                    {"path": d["path"], "time_played": d["time_played"], "playhead": d["playhead"], "done": False},
-                )
+            if (d.get("play_count") or 0) == 0:
+                new_schema.append({**d, "done": False})
             else:
-                for _ in range(d["playhead"]):
-                    new_schema.append(
-                        {"path": d["path"], "time_played": d["time_played"], "playhead": d["playhead"], "done": True},
-                    )
+                n = d.get("time_played") or consts.now()
+                for i in range(d["play_count"]):
+                    new_schema.append({**d, "done": True, "time_played": n + i})
         copy_counts.extend(new_schema)
-    except:
-        log.info("Old schema playhead could not be read")
+    except Exception:
+        log.info("Old schema could not be read")
 
     try:
         copy_counts.extend(
             list(
-                args.db.query(
+                s_db.query(
                     """
                 SELECT
-                    path, time_played, playhead, done
+                    path
+                    , h.time_played
+                    , h.playhead
+                    , done
                 FROM
-                    src.media m
-                JOIN src.history h on h.media_id = m.id
+                    media m
+                JOIN history h on h.media_id = m.id
                 WHERE
                     h.time_played > 0
                     OR
                     h.playhead > 0
                 """,
                 ),
             ),
         )
-    except:
-        log.info("New schema playhead could not be read")
+    except Exception:
+        log.exception("New schema could not be read")
 
+    log.info(len(copy_counts))
     for d in copy_counts:
         renamed_path = d["path"].replace(args.source_prefix, args.target_prefix, 1)
-        history.add(args, [renamed_path], time_played=d["time_played"], playhead=d["playhead"], mark_done=d["done"])
+        history.add(
+            args, [renamed_path], time_played=d.get("time_played"), playhead=d.get("playhead"), mark_done=d["done"]
+        )
 
 
 def copy_play_counts() -> None:
     args = parse_args()
+    history.create(args)
     for s_db in args.source_dbs:
         copy_play_count(args, s_db)
     dedupe_rows(args, "history", ["id"], ["media_id", "time_played"])
 
 
 if __name__ == "__main__":
     copy_play_counts()
```

### Comparing `xklb-2.1.9/xklb/scripts/dedupe.py` & `xklb-2.2.2/xklb/scripts/dedupe.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from copy import deepcopy
 from pathlib import Path
 from typing import List
 
 import humanize
 from tabulate import tabulate
 
-from xklb import db, player, usage, utils
+from xklb import consts, db, player, usage, utils
 from xklb.consts import DBType
 from xklb.utils import log
 
 
 def parse_args() -> argparse.Namespace:
     parser = argparse.ArgumentParser(prog="library dedupe", usage=usage.dedupe)
 
@@ -234,15 +234,15 @@
         return
 
     tbl = deepcopy(duplicates)
     tbl = tbl[: int(args.limit)]
     tbl = utils.col_resize(tbl, "keep_path", 30)
     tbl = utils.col_resize(tbl, "duplicate_path", 30)
     tbl = utils.col_naturalsize(tbl, "duplicate_size")
-    print(tabulate(tbl, tablefmt="fancy_grid", headers="keys", showindex=False))
+    print(tabulate(tbl, tablefmt=consts.TABULATE_STYLE, headers="keys", showindex=False))
 
     duplicates_count = len(duplicates)
     print(f"{duplicates_count} duplicates found (showing first {args.limit})")
 
     try:
         import pandas as pd
```

### Comparing `xklb-2.1.9/xklb/scripts/dedupe_db.py` & `xklb-2.2.2/xklb/scripts/dedupe_db.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.9/xklb/scripts/download_status.py` & `xklb-2.2.2/xklb/scripts/download_status.py`

 * *Files 6% similar despite different names*

```diff
@@ -69,15 +69,15 @@
     else:
         tbl = utils.col_resize(tbl, "path", 30)
         tbl = utils.col_resize(tbl, "title", 20)
         tbl = utils.col_resize(tbl, "uploader_url")
 
         tbl = utils.list_dict_filter_bool(tbl)
 
-        print(tabulate(tbl, tablefmt="fancy_grid", headers="keys", showindex=False))
+        print(tabulate(tbl, tablefmt=consts.TABULATE_STYLE, headers="keys", showindex=False))
 
     print(f"{len(media)} playlists" if len(media) > 1 else "1 playlist")
     duration = sum(m.get("duration") or 0 for m in media)
     if duration > 0:
         duration = utils.human_time(duration)
         if not args.aggregate:
             print("Total duration:", duration)
@@ -132,8 +132,8 @@
             if error["count"] == 1:
                 other_errors.append(error)
             else:
                 common_errors.append(error)
 
         common_errors.append({"error": "Other", "count": len(other_errors)})
         common_errors.append({"error": "Total", "count": sum(d["count"] for d in errors)})
-        print(tabulate(common_errors, tablefmt="fancy_grid", headers="keys", showindex=False))
+        print(tabulate(common_errors, tablefmt=consts.TABULATE_STYLE, headers="keys", showindex=False))
```

### Comparing `xklb-2.1.9/xklb/scripts/history.py` & `xklb-2.2.2/xklb/scripts/history.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,30 +61,30 @@
 
 def print_history(tbl):
     utils.col_duration(tbl, "duration_sum")
     utils.col_duration(tbl, "duration_avg")
     utils.col_naturalsize(tbl, "size_sum")
     utils.col_naturalsize(tbl, "size_avg")
     tbl = utils.list_dict_filter_bool(tbl)
-    print(tabulate(tbl, tablefmt="fancy_grid", headers="keys", showindex=False))
+    print(tabulate(tbl, tablefmt=consts.TABULATE_STYLE, headers="keys", showindex=False))
 
 
 def print_recent(tbl, time_column=None):
     utils.col_duration(tbl, "duration")
     utils.col_duration(tbl, "playhead")
     if time_column:
         utils.col_naturaltime(tbl, time_column)
     tbl = [{"title_path": "\n".join(utils.concat(d["title"], d["path"])), **d} for d in tbl]
     tbl = [{k: v for k, v in d.items() if k not in ("title", "path")} for d in tbl]
 
     tbl = utils.col_resize(tbl, "title_path", 40)
     tbl = utils.col_resize(tbl, "duration", 5)
     tbl = utils.col_resize(tbl, "playhead", 5)
     tbl = utils.list_dict_filter_bool(tbl)
-    print(tabulate(tbl, tablefmt="fancy_grid", headers="keys", showindex=False))
+    print(tabulate(tbl, tablefmt=consts.TABULATE_STYLE, headers="keys", showindex=False))
 
 
 def recent_media(args, time_column):
     m_columns = db.columns(args, "media")
     query = f"""
     SELECT
         path
@@ -112,27 +112,26 @@
         print_history(tbl)
         query = f"""WITH m as (
                 SELECT
                     SUM(CASE WHEN h.done = 1 THEN 1 ELSE 0 END) play_count
                     , MIN(h.time_played) time_first_played
                     , MAX(h.time_played) time_last_played
                     , FIRST_VALUE(h.playhead) OVER (PARTITION BY h.media_id ORDER BY h.time_played DESC) playhead
-                    , *
+                    , path
+                    {', title' if 'title' in m_columns else ''}
+                    {', duration' if 'duration' in m_columns else ''}
+                    {', subtitle_count' if 'subtitle_count' in m_columns else ''}
                 FROM media m
                 LEFT JOIN history h on h.media_id = m.id
+                WHERE coalesce(time_deleted, 0) = 0
                 GROUP BY m.id, m.path
             )
-            SELECT
-                path
-                {', title' if 'title' in m_columns else ''}
-                {', duration' if 'duration' in m_columns else ''}
-                {', subtitle_count' if 'subtitle_count' in m_columns else ''}
-                , time_last_played
+            SELECT *
             FROM m
-            WHERE coalesce(time_deleted, 0) = 0
+            WHERE 1=1
                 and coalesce(playhead, 0) > 60
                 and coalesce(play_count, 0) = 0
             ORDER BY time_last_played desc, playhead desc
             LIMIT {args.limit or 5}
         """
         tbl = list(args.db.query(query))
         print_recent(tbl, "time_last_played")
@@ -143,26 +142,23 @@
         print_history(tbl)
         query = f"""WITH m as (
                 SELECT
                     SUM(CASE WHEN h.done = 1 THEN 1 ELSE 0 END) play_count
                     , MIN(h.time_played) time_first_played
                     , MAX(h.time_played) time_last_played
                     , FIRST_VALUE(h.playhead) OVER (PARTITION BY h.media_id ORDER BY h.time_played DESC) playhead
-                    , *
+                    , path
+                    {', title' if 'title' in m_columns else ''}
+                    {', duration' if 'duration' in m_columns else ''}
+                    {', subtitle_count' if 'subtitle_count' in m_columns else ''}
                 FROM media m
                 LEFT JOIN history h on h.media_id = m.id
                 GROUP BY m.id, m.path
             )
-            SELECT
-                path
-                {', title' if 'title' in m_columns else ''}
-                {', duration' if 'duration' in m_columns else ''}
-                {', subtitle_count' if 'subtitle_count' in m_columns else ''}
-                , time_last_played
-                , play_count
+            SELECT *
             FROM m
             WHERE coalesce(play_count, 0)>0
             ORDER BY time_last_played desc, path
             LIMIT {args.limit or 5}
         """
         tbl = list(args.db.query(query))
         print_recent(tbl, "time_last_played")
```

### Comparing `xklb-2.1.9/xklb/scripts/merge_dbs.py` & `xklb-2.2.2/xklb/scripts/merge_dbs.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.9/xklb/scripts/merge_online_local.py` & `xklb-2.2.2/xklb/scripts/merge_online_local.py`

 * *Files 4% similar despite different names*

```diff
@@ -47,15 +47,15 @@
         FROM
             media
         WHERE 1=1
             and time_deleted = 0
             and extractor_id is null
             and title is null
     ) m2
-    JOIN media_fts on m2.id = media_fts.id
+    JOIN media_fts on m2.id = media_fts.rowid
     JOIN playlists p2 on p2.id = m2.playlist_id
     WHERE p2.extractor_key = 'Local'
         AND media_fts.path MATCH '"'||m1.extractor_id||'"'
         AND m2.PATH LIKE '%['||m1.extractor_id||']%'
     ORDER BY 1=1
         , length(m2.path)-length(REPLACE(m2.path, '/', '')) desc
         , length(m2.path)-length(REPLACE(m2.path, '.', ''))
@@ -76,15 +76,15 @@
     duplicates_count = len(duplicates)
 
     tbl = deepcopy(duplicates)
     tbl = tbl[: int(args.limit)]
     tbl = utils.col_resize(tbl, "keep_path", 30)
     tbl = utils.col_resize(tbl, "duplicate_path", 30)
     tbl = utils.col_naturalsize(tbl, "duplicate_size")
-    print(tabulate(tbl, tablefmt="fancy_grid", headers="keys", showindex=False))
+    print(tabulate(tbl, tablefmt=consts.TABULATE_STYLE, headers="keys", showindex=False))
 
     print(f"{duplicates_count} duplicates found (showing first {args.limit})")
     if duplicates and utils.confirm("Merge duplicates?"):  # type: ignore
         log.info("Merging...")
 
         merged = []
         for d in duplicates:
```

### Comparing `xklb-2.1.9/xklb/scripts/move_list.py` & `xklb-2.2.2/xklb/scripts/move_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from copy import deepcopy
 from pathlib import Path
 from typing import Dict, List, Tuple
 
 import humanize
 from tabulate import tabulate
 
-from xklb import db, player, usage, utils
+from xklb import consts, db, player, usage, utils
 from xklb.utils import log
 
 
 def parse_args() -> argparse.Namespace:
     parser = argparse.ArgumentParser(
         prog="library mv-list",
         usage=usage.mv_list,
@@ -77,15 +77,15 @@
 
 def iterate_and_show_options(args, tbl) -> Tuple[List[Dict], List[Dict]]:
     vew = tbl[-int(args.limit) :] if args.limit else tbl
 
     vew = utils.list_dict_filter_bool(vew, keep_0=False)
     vew = utils.col_resize(vew, "path", 60)
     vew = utils.col_naturalsize(vew, "size")
-    print(tabulate(vew, tablefmt="fancy_grid", headers="keys", showindex=False))
+    print(tabulate(vew, tablefmt=consts.TABULATE_STYLE, headers="keys", showindex=False))
     print(len(tbl) - len(vew), "other folders not shown")
 
     if args.limit:
         return tbl[-int(args.limit) :], tbl[: -int(args.limit)]
     else:
         return tbl, tbl
```

### Comparing `xklb-2.1.9/xklb/scripts/optimize_db.py` & `xklb-2.2.2/xklb/scripts/optimize_db.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.9/xklb/scripts/playback_control.py` & `xklb-2.2.2/xklb/scripts/playback_control.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.9/xklb/scripts/playlists.py` & `xklb-2.2.2/xklb/scripts/playlists.py`

 * *Files 4% similar despite different names*

```diff
@@ -94,15 +94,15 @@
     else:
         tbl = utils.col_resize(tbl, "path", 30)
         tbl = utils.col_resize(tbl, "title", 20)
         tbl = utils.col_resize(tbl, "uploader_url")
 
         tbl = utils.list_dict_filter_bool(tbl)
 
-        print(tabulate(tbl, tablefmt="fancy_grid", headers="keys", showindex=False))
+        print(tabulate(tbl, tablefmt=consts.TABULATE_STYLE, headers="keys", showindex=False))
 
     print(f"{len(media)} playlists" if len(media) > 1 else "1 playlist")
     duration = sum(m.get("duration") or 0 for m in media)
     if duration > 0:
         duration = utils.human_time(duration)
         if not args.aggregate:
             print("Total duration:", duration)
```

### Comparing `xklb-2.1.9/xklb/scripts/redownload.py` & `xklb-2.2.2/xklb/scripts/redownload.py`

 * *Files 1% similar despite different names*

```diff
@@ -104,29 +104,29 @@
         else:
             args.db["media"].upsert(d, pk="id", alter=True)  # type: ignore
 
 
 def print_deletions(args, deletions) -> None:
     print("Deletions:")
     tbl = deepcopy(deletions)
-    print(tabulate(tbl, tablefmt="fancy_grid", headers="keys", showindex=False))
+    print(tabulate(tbl, tablefmt=consts.TABULATE_STYLE, headers="keys", showindex=False))
     print(f"Showing most recent {args.limit} deletions. Use -l to change this limit")
 
 
 def print_deleted(args, deleted_media) -> None:
     tbl = deepcopy(deleted_media)
     tbl = utils.list_dict_filter_bool(tbl, keep_0=False)
     tbl = utils.list_dict_filter_unique(tbl)
     tbl = tbl[: int(args.limit)]
     tbl = utils.col_resize(tbl, "path", 25)
     tbl = utils.col_duration(tbl, "duration")
     tbl = utils.col_naturalsize(tbl, "size")
     for t in consts.TIME_COLUMNS:
         utils.col_naturaldate(tbl, t)
-    print(tabulate(tbl, tablefmt="fancy_grid", headers="keys", showindex=False))
+    print(tabulate(tbl, tablefmt=consts.TABULATE_STYLE, headers="keys", showindex=False))
     print(f"{len(deleted_media)} deleted media found (showing first {args.limit})")
 
 
 def redownload() -> None:
     args = parse_args()
 
     if args.deleted_at:
```

### Comparing `xklb-2.1.9/xklb/scripts/relmv.py` & `xklb-2.2.2/xklb/scripts/relmv.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.9/xklb/scripts/scatter.py` & `xklb-2.2.2/xklb/scripts/scatter.py`

 * *Files 2% similar despite different names*

```diff
@@ -113,15 +113,15 @@
 def print_path_stats(tbl) -> None:
     tbl = utils.list_dict_filter_bool(tbl, keep_0=False)
     tbl = utils.col_naturalsize(tbl, "total_size")
     tbl = utils.col_naturalsize(tbl, "median_size")
     for t in consts.TIME_COLUMNS:
         utils.col_naturaldate(tbl, t)
 
-    print(tabulate(tbl, tablefmt="fancy_grid", headers="keys", showindex=False))
+    print(tabulate(tbl, tablefmt=consts.TABULATE_STYLE, headers="keys", showindex=False))
 
 
 def rebin_files(args, disk_stats, all_files) -> Tuple[List, List]:
     total_size = sum(d["size"] for d in all_files)
 
     untouched = []
     to_rebin = []
@@ -206,15 +206,15 @@
         tbl = []
         for existing_path, new_path in rebinned:
             tbl.append({"existing_path": existing_path, "new_path": new_path})
             if len(tbl) > 10:
                 break
         tbl = utils.col_resize(tbl, "existing_path", 20)
         tbl = utils.col_resize(tbl, "new_path", 20)
-        print(tabulate(tbl, tablefmt="fancy_grid", headers="keys", showindex=False))
+        print(tabulate(tbl, tablefmt=consts.TABULATE_STYLE, headers="keys", showindex=False))
         print(len(rebinned), "files would be moved (only 10 shown)")
         print(len(untouched), "files would not be moved")
 
         if utils.confirm("Move files ?"):
             utils.move_files(rebinned)
         sys.exit(0)
```

### Comparing `xklb-2.1.9/xklb/scripts/streaming_tab_loader.py` & `xklb-2.2.2/xklb/scripts/streaming_tab_loader.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.9/xklb/scripts/mining/data.py` & `xklb-2.2.2/xklb/scripts/mining/data.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.9/xklb/scripts/mining/extract_links.py` & `xklb-2.2.2/xklb/scripts/mining/extract_links.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.9/xklb/scripts/mining/mpv_watchlater.py` & `xklb-2.2.2/xklb/scripts/mining/mpv_watchlater.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.9/xklb/scripts/mining/nouns.py` & `xklb-2.2.2/xklb/scripts/mining/nouns.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.9/xklb/scripts/mining/pushshift.py` & `xklb-2.2.2/xklb/scripts/mining/pushshift.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.9/xklb/scripts/mining/reddit_selftext.py` & `xklb-2.2.2/xklb/scripts/mining/reddit_selftext.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.9/xklb/assets/kotobago.png` & `xklb-2.2.2/xklb/assets/kotobago.png`

 * *Files identical despite different names*

### Comparing `xklb-2.1.9/.gitignore` & `xklb-2.2.2/.gitignore`

 * *Files identical despite different names*

### Comparing `xklb-2.1.9/LICENSE` & `xklb-2.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `xklb-2.1.9/README.md` & `xklb-2.2.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -139,15 +139,15 @@
 Incremental surfing. 📈🏄 totally rad!
 
 </details>
 
 <details><summary>List all subcommands</summary>
 
     $ library
-    xk media library subcommands (v2.1.007)
+    xk media library subcommands (v2.2.002)
 
     local media:
       lb fsadd                 Create a local media database; Add folders
       lb fsupdate              Refresh database: add new files, mark deleted
 
       lb listen                Listen to local and online media
       lb watch                 Watch local and online media
@@ -189,33 +189,37 @@
       lb stop                  Stop all playback
       lb pause                 Pause all playback
 
     statistics:
       lb history               Show some playback statistics
       lb playlists             List added playlists
       lb download-status       Show download status
-      lb disk-usage            Print mount usage
+      lb disk-usage            Print disk usage
+      lb mount-stats           Print mount usage
 
     browser tabs:
       lb tabsadd               Create a tabs database; Add URLs
       lb tabs                  Open your tabs for the day
       lb surf                  Load browser tabs in a streaming way (stdin)
 
+    places:
+      lb places-import         Load POIs from Google Maps Google Takeout
+
     mining:
       lb reddit-selftext       db selftext external links -> db media table
       lb pushshift             Convert Pushshift jsonl.zstd -> reddit.db format (stdin)
       lb hnadd                 Create a hackernews database (this takes a few days)
 
       lb extract-links         Extract links from lists of web pages
 
       lb mpv-watchlater        Import timestamps from mpv watchlater to history table
 
       lb cluster-sort          Lines -> sorted by sentence similarity groups (stdin)
       lb nouns                 Unstructured text -> compound nouns (stdin)
-
+    
 
 </details>
 
 ## Examples
 
 ### Watch online media on your PC
 
@@ -446,15 +450,15 @@
 
     Create a dl database / add links to an existing database
 
         library tubeadd dl.db https://www.youdl.com/c/BranchEducation/videos
 
     Add links from a line-delimited file
 
-        library tubeadd reddit.db --playlist-file ./my_yt_subscriptions.txt
+        cat ./my_yt_subscriptions.txt | library tubeadd reddit.db -
 
     Add metadata to links already in a database table
 
         library tubeadd --force reddit.db (sqlite-utils --raw-lines reddit.db 'select path from media')
 
     Files will be saved to <download prefix>/<extractor>/
 
@@ -1373,14 +1377,50 @@
 
     lb bigdirs video.db --depth 5
     lb bigdirs video.db --depth 7
 
 
 </details>
 
+<details><summary>Disk Usage (disk-usage)</summary>
+
+    $ library disk-usage -h
+    usage: library disk-usage DATABASE [--sort-by size | count] [--depth DEPTH] [PATH / SUBSTRING SEARCH]
+
+    Only include files smaller than 1kib
+
+        library disk-usage du.db --size=-1Ki
+        lb du du.db -S-1Ki
+        | path                                  |      size |   count |
+        |---------------------------------------|-----------|---------|
+        | /home/xk/github/xk/lb/__pycache__/    | 620 Bytes |       1 |
+        | /home/xk/github/xk/lb/.github/        |    1.7 kB |       4 |
+        | /home/xk/github/xk/lb/__pypackages__/ |    1.4 MB |    3519 |
+        | /home/xk/github/xk/lb/xklb/           |    4.4 kB |      12 |
+        | /home/xk/github/xk/lb/tests/          |    3.2 kB |       9 |
+        | /home/xk/github/xk/lb/.git/           |  782.4 kB |    2276 |
+        | /home/xk/github/xk/lb/.pytest_cache/  |    1.5 kB |       5 |
+        | /home/xk/github/xk/lb/.ruff_cache/    |   19.5 kB |     100 |
+        | /home/xk/github/xk/lb/.gitattributes  | 119 Bytes |         |
+        | /home/xk/github/xk/lb/.mypy_cache/    | 280 Bytes |       4 |
+        | /home/xk/github/xk/lb/.pdm-python     |  15 Bytes |         |
+
+    Only include files with a specific depth
+
+        library disk-usage du.db --depth 19
+        lb du du.db -d 19
+        | path                                                                                                                                                                |     size |
+        |---------------------------------------------------------------------------------------------------------------------------------------------------------------------|----------|
+        | /home/xk/github/xk/lb/__pypackages__/3.11/lib/jedi/third_party/typeshed/third_party/2and3/requests/packages/urllib3/packages/ssl_match_hostname/__init__.pyi        | 88 Bytes |
+        | /home/xk/github/xk/lb/__pypackages__/3.11/lib/jedi/third_party/typeshed/third_party/2and3/requests/packages/urllib3/packages/ssl_match_hostname/_implementation.pyi | 81 Bytes |
+
+
+
+</details>
+
 <details><summary>Copy play history (copy-play-counts)</summary>
 
     $ library copy-play-counts -h
     usage: library copy-play-counts DEST_DB SOURCE_DB ... [--source-prefix x] [--target-prefix y]
 
     Copy play count information between databases
 
@@ -1585,14 +1625,41 @@
 
     If you prefer GUI, check out https://unli.xyz/tabsender/
 
 
 </details>
 
 
+<details><summary>Chicken mode</summary>
+
+just kidding :-)
+
+           ////////////////////////
+          ////////////////////////|
+         //////////////////////// |
+        ////////////////////////| |
+        |    _\/_   |   _\/_    | |
+        |     )o(>  |  <)o(     | |
+        |   _/ <\   |   /> \_   | |
+        |  (_____)  |  (_____)  | |_
+        | ~~~oOo~~~ | ~~~0oO~~~ |/__|
+       _|====\_=====|=====_/====|_ ||
+      |_|\_________ O _________/|_|||
+       ||//////////|_|\\\\\\\\\\|| ||
+       || ||       |\_\\        || ||
+       ||/||        \\_\\       ||/||
+       ||/||         \)_\)      ||/||
+       || ||         \  O /     || ||
+       ||             \  /      || LGB
+
+                   \________/======
+                   / ( || ) \\
+
+</details>
+
 You can expand all by running this in your browser console:
 
 ```js
 (() => { const readmeDiv = document.getElementById("readme"); const detailsElements = readmeDiv.getElementsByTagName("details"); for (let i = 0; i < detailsElements.length; i++) { detailsElements[i].setAttribute("open", "true"); } })();
 ```
```

### Comparing `xklb-2.1.9/pyproject.toml` & `xklb-2.2.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -30,21 +30,21 @@
 license = {file = "LICENSE"}
 name = "xklb"
 readme = "README.md"
 requires-python = ">=3.8"
 
 [project.optional-dependencies]
 all = ["xklb[deluxe,dev,test]"]
-deluxe = ["textract", "PyExifTool", "aiohttp", "brotab", "orjson", "pandas", "spacy", "sklearn"]
+deluxe = ["textract", "PyExifTool", "aiohttp", "brotab", "orjson", "geopandas", "spacy", "scikit-learn"]
 dev = ["black", "ipdb", "isort", "scalene", "ssort"]
 test = ["ruff", "pytest"]
 
 [project.urls]
-documentation = "https://github.com/chapmanjacobd/library/wiki/Usage"
-homepage = "https://github.com/chapmanjacobd/library/"
+documentation = "https://github.com/chapmanjacobd/library#usage"
+homepage = "https://github.com/chapmanjacobd/library#readme"
 repository = "https://github.com/chapmanjacobd/library/"
 
 [project.scripts]
 lb = 'xklb.lb:library'
 library = 'xklb.lb:library'
 
 [tool.pdm]
```

### Comparing `xklb-2.1.9/PKG-INFO` & `xklb-2.2.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: xklb
-Version: 2.1.9
+Version: 2.2.2
 Summary: xk library
-Project-URL: documentation, https://github.com/chapmanjacobd/library/wiki/Usage
-Project-URL: homepage, https://github.com/chapmanjacobd/library/
+Project-URL: documentation, https://github.com/chapmanjacobd/library#usage
+Project-URL: homepage, https://github.com/chapmanjacobd/library#readme
 Project-URL: repository, https://github.com/chapmanjacobd/library/
 Author-email: Jacob Chapman <7908073+chapmanjacobd@users.noreply.github.com>
 License: BSD 3-Clause No Nuclear License
         
         Copyright (c) 2021, Jacob Chapman
         All rights reserved.
         
@@ -62,18 +62,18 @@
 Requires-Dist: tinytag
 Requires-Dist: yt-dlp
 Provides-Extra: all
 Requires-Dist: xklb[deluxe,dev,test]; extra == 'all'
 Provides-Extra: deluxe
 Requires-Dist: aiohttp; extra == 'deluxe'
 Requires-Dist: brotab; extra == 'deluxe'
+Requires-Dist: geopandas; extra == 'deluxe'
 Requires-Dist: orjson; extra == 'deluxe'
-Requires-Dist: pandas; extra == 'deluxe'
 Requires-Dist: pyexiftool; extra == 'deluxe'
-Requires-Dist: sklearn; extra == 'deluxe'
+Requires-Dist: scikit-learn; extra == 'deluxe'
 Requires-Dist: spacy; extra == 'deluxe'
 Requires-Dist: textract; extra == 'deluxe'
 Provides-Extra: dev
 Requires-Dist: black; extra == 'dev'
 Requires-Dist: ipdb; extra == 'dev'
 Requires-Dist: isort; extra == 'dev'
 Requires-Dist: scalene; extra == 'dev'
@@ -224,15 +224,15 @@
 Incremental surfing. 📈🏄 totally rad!
 
 </details>
 
 <details><summary>List all subcommands</summary>
 
     $ library
-    xk media library subcommands (v2.1.007)
+    xk media library subcommands (v2.2.002)
 
     local media:
       lb fsadd                 Create a local media database; Add folders
       lb fsupdate              Refresh database: add new files, mark deleted
 
       lb listen                Listen to local and online media
       lb watch                 Watch local and online media
@@ -274,33 +274,37 @@
       lb stop                  Stop all playback
       lb pause                 Pause all playback
 
     statistics:
       lb history               Show some playback statistics
       lb playlists             List added playlists
       lb download-status       Show download status
-      lb disk-usage            Print mount usage
+      lb disk-usage            Print disk usage
+      lb mount-stats           Print mount usage
 
     browser tabs:
       lb tabsadd               Create a tabs database; Add URLs
       lb tabs                  Open your tabs for the day
       lb surf                  Load browser tabs in a streaming way (stdin)
 
+    places:
+      lb places-import         Load POIs from Google Maps Google Takeout
+
     mining:
       lb reddit-selftext       db selftext external links -> db media table
       lb pushshift             Convert Pushshift jsonl.zstd -> reddit.db format (stdin)
       lb hnadd                 Create a hackernews database (this takes a few days)
 
       lb extract-links         Extract links from lists of web pages
 
       lb mpv-watchlater        Import timestamps from mpv watchlater to history table
 
       lb cluster-sort          Lines -> sorted by sentence similarity groups (stdin)
       lb nouns                 Unstructured text -> compound nouns (stdin)
-
+    
 
 </details>
 
 ## Examples
 
 ### Watch online media on your PC
 
@@ -531,15 +535,15 @@
 
     Create a dl database / add links to an existing database
 
         library tubeadd dl.db https://www.youdl.com/c/BranchEducation/videos
 
     Add links from a line-delimited file
 
-        library tubeadd reddit.db --playlist-file ./my_yt_subscriptions.txt
+        cat ./my_yt_subscriptions.txt | library tubeadd reddit.db -
 
     Add metadata to links already in a database table
 
         library tubeadd --force reddit.db (sqlite-utils --raw-lines reddit.db 'select path from media')
 
     Files will be saved to <download prefix>/<extractor>/
 
@@ -1458,14 +1462,50 @@
 
     lb bigdirs video.db --depth 5
     lb bigdirs video.db --depth 7
 
 
 </details>
 
+<details><summary>Disk Usage (disk-usage)</summary>
+
+    $ library disk-usage -h
+    usage: library disk-usage DATABASE [--sort-by size | count] [--depth DEPTH] [PATH / SUBSTRING SEARCH]
+
+    Only include files smaller than 1kib
+
+        library disk-usage du.db --size=-1Ki
+        lb du du.db -S-1Ki
+        | path                                  |      size |   count |
+        |---------------------------------------|-----------|---------|
+        | /home/xk/github/xk/lb/__pycache__/    | 620 Bytes |       1 |
+        | /home/xk/github/xk/lb/.github/        |    1.7 kB |       4 |
+        | /home/xk/github/xk/lb/__pypackages__/ |    1.4 MB |    3519 |
+        | /home/xk/github/xk/lb/xklb/           |    4.4 kB |      12 |
+        | /home/xk/github/xk/lb/tests/          |    3.2 kB |       9 |
+        | /home/xk/github/xk/lb/.git/           |  782.4 kB |    2276 |
+        | /home/xk/github/xk/lb/.pytest_cache/  |    1.5 kB |       5 |
+        | /home/xk/github/xk/lb/.ruff_cache/    |   19.5 kB |     100 |
+        | /home/xk/github/xk/lb/.gitattributes  | 119 Bytes |         |
+        | /home/xk/github/xk/lb/.mypy_cache/    | 280 Bytes |       4 |
+        | /home/xk/github/xk/lb/.pdm-python     |  15 Bytes |         |
+
+    Only include files with a specific depth
+
+        library disk-usage du.db --depth 19
+        lb du du.db -d 19
+        | path                                                                                                                                                                |     size |
+        |---------------------------------------------------------------------------------------------------------------------------------------------------------------------|----------|
+        | /home/xk/github/xk/lb/__pypackages__/3.11/lib/jedi/third_party/typeshed/third_party/2and3/requests/packages/urllib3/packages/ssl_match_hostname/__init__.pyi        | 88 Bytes |
+        | /home/xk/github/xk/lb/__pypackages__/3.11/lib/jedi/third_party/typeshed/third_party/2and3/requests/packages/urllib3/packages/ssl_match_hostname/_implementation.pyi | 81 Bytes |
+
+
+
+</details>
+
 <details><summary>Copy play history (copy-play-counts)</summary>
 
     $ library copy-play-counts -h
     usage: library copy-play-counts DEST_DB SOURCE_DB ... [--source-prefix x] [--target-prefix y]
 
     Copy play count information between databases
 
@@ -1670,14 +1710,41 @@
 
     If you prefer GUI, check out https://unli.xyz/tabsender/
 
 
 </details>
 
 
+<details><summary>Chicken mode</summary>
+
+just kidding :-)
+
+           ////////////////////////
+          ////////////////////////|
+         //////////////////////// |
+        ////////////////////////| |
+        |    _\/_   |   _\/_    | |
+        |     )o(>  |  <)o(     | |
+        |   _/ <\   |   /> \_   | |
+        |  (_____)  |  (_____)  | |_
+        | ~~~oOo~~~ | ~~~0oO~~~ |/__|
+       _|====\_=====|=====_/====|_ ||
+      |_|\_________ O _________/|_|||
+       ||//////////|_|\\\\\\\\\\|| ||
+       || ||       |\_\\        || ||
+       ||/||        \\_\\       ||/||
+       ||/||         \)_\)      ||/||
+       || ||         \  O /     || ||
+       ||             \  /      || LGB
+
+                   \________/======
+                   / ( || ) \\
+
+</details>
+
 You can expand all by running this in your browser console:
 
 ```js
 (() => { const readmeDiv = document.getElementById("readme"); const detailsElements = readmeDiv.getElementsByTagName("details"); for (let i = 0; i < detailsElements.length; i++) { detailsElements[i].setAttribute("open", "true"); } })();
 ```
```

