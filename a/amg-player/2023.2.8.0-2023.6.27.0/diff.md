# Comparing `tmp/amg-player-2023.2.8.0.tar.gz` & `tmp/amg-player-2023.6.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amg-player-2023.2.8.0.tar", last modified: Wed Feb  8 22:25:46 2023, max compression
+gzip compressed data, was "amg-player-2023.6.27.0.tar", last modified: Tue Jun 27 21:00:05 2023, max compression
```

## Comparing `amg-player-2023.2.8.0.tar` & `amg-player-2023.6.27.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 maxime    (1000) maxime    (1000)        0 2023-02-08 22:25:46.035610 amg-player-2023.2.8.0/
--rw-rw-r--   0 maxime    (1000) maxime    (1000)    35147 2017-08-27 13:04:32.000000 amg-player-2023.2.8.0/LICENSE
--rw-r--r--   0 maxime    (1000) maxime    (1000)       43 2019-04-14 00:02:10.000000 amg-player-2023.2.8.0/MANIFEST.in
--rw-r--r--   0 maxime    (1000) maxime    (1000)     4355 2023-02-08 22:25:46.035610 amg-player-2023.2.8.0/PKG-INFO
--rw-r--r--   0 maxime    (1000) maxime    (1000)     3317 2021-03-06 00:23:11.000000 amg-player-2023.2.8.0/README.md
-drwxr-xr-x   0 maxime    (1000) maxime    (1000)        0 2023-02-08 22:25:46.035610 amg-player-2023.2.8.0/amg/
--rwxr-xr-x   0 maxime    (1000) maxime    (1000)    31835 2023-02-08 22:25:44.000000 amg-player-2023.2.8.0/amg/__init__.py
--rwxrwxr-x   0 maxime    (1000) maxime    (1000)      123 2021-03-06 17:06:13.000000 amg-player-2023.2.8.0/amg/__main__.py
--rw-rw-r--   0 maxime    (1000) maxime    (1000)     1040 2021-08-08 17:01:47.000000 amg-player-2023.2.8.0/amg/colored_logging.py
--rw-r--r--   0 maxime    (1000) maxime    (1000)     4559 2021-08-08 17:01:47.000000 amg-player-2023.2.8.0/amg/menu.py
--rw-r--r--   0 maxime    (1000) maxime    (1000)      487 2021-03-06 16:51:07.000000 amg-player-2023.2.8.0/amg/mkstemp_ctx.py
--rw-r--r--   0 maxime    (1000) maxime    (1000)     3428 2021-11-22 18:58:44.000000 amg-player-2023.2.8.0/amg/sanitize.py
--rw-r--r--   0 maxime    (1000) maxime    (1000)    26992 2023-02-08 22:25:40.000000 amg-player-2023.2.8.0/amg/tag.py
--rw-r--r--   0 maxime    (1000) maxime    (1000)     2942 2022-05-17 14:22:25.000000 amg-player-2023.2.8.0/amg/ytdl_tqdm.py
-drwxr-xr-x   0 maxime    (1000) maxime    (1000)        0 2023-02-08 22:25:46.035610 amg-player-2023.2.8.0/amg_player.egg-info/
--rw-rw-r--   0 maxime    (1000) maxime    (1000)     4355 2023-02-08 22:25:46.000000 amg-player-2023.2.8.0/amg_player.egg-info/PKG-INFO
--rw-rw-r--   0 maxime    (1000) maxime    (1000)      409 2023-02-08 22:25:46.000000 amg-player-2023.2.8.0/amg_player.egg-info/SOURCES.txt
--rw-rw-r--   0 maxime    (1000) maxime    (1000)        1 2023-02-08 22:25:46.000000 amg-player-2023.2.8.0/amg_player.egg-info/dependency_links.txt
--rw-rw-r--   0 maxime    (1000) maxime    (1000)       37 2023-02-08 22:25:46.000000 amg-player-2023.2.8.0/amg_player.egg-info/entry_points.txt
--rw-rw-r--   0 maxime    (1000) maxime    (1000)      215 2023-02-08 22:25:46.000000 amg-player-2023.2.8.0/amg_player.egg-info/requires.txt
--rw-rw-r--   0 maxime    (1000) maxime    (1000)        4 2023-02-08 22:25:46.000000 amg-player-2023.2.8.0/amg_player.egg-info/top_level.txt
--rw-r--r--   0 maxime    (1000) maxime    (1000)      216 2023-02-08 22:25:44.000000 amg-player-2023.2.8.0/requirements.txt
--rw-r--r--   0 maxime    (1000) maxime    (1000)       38 2023-02-08 22:25:46.035610 amg-player-2023.2.8.0/setup.cfg
--rwxr-xr-x   0 maxime    (1000) maxime    (1000)     1871 2021-03-06 17:11:29.000000 amg-player-2023.2.8.0/setup.py
-drwxr-xr-x   0 maxime    (1000) maxime    (1000)        0 2023-02-08 22:25:46.035610 amg-player-2023.2.8.0/tests/
--rwxr-xr-x   0 maxime    (1000) maxime    (1000)     4244 2023-02-07 16:44:12.000000 amg-player-2023.2.8.0/tests/__init__.py
+drwxr-xr-x   0 maxime    (1000) maxime    (1000)        0 2023-06-27 21:00:05.667998 amg-player-2023.6.27.0/
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)    35147 2017-08-27 13:04:32.000000 amg-player-2023.6.27.0/LICENSE
+-rw-r--r--   0 maxime    (1000) maxime    (1000)       43 2019-04-14 00:02:10.000000 amg-player-2023.6.27.0/MANIFEST.in
+-rw-r--r--   0 maxime    (1000) maxime    (1000)     4320 2023-06-27 21:00:05.667998 amg-player-2023.6.27.0/PKG-INFO
+-rw-r--r--   0 maxime    (1000) maxime    (1000)     3317 2021-03-06 00:23:11.000000 amg-player-2023.6.27.0/README.md
+drwxr-xr-x   0 maxime    (1000) maxime    (1000)        0 2023-06-27 21:00:05.667998 amg-player-2023.6.27.0/amg/
+-rwxr-xr-x   0 maxime    (1000) maxime    (1000)    31785 2023-06-27 21:00:03.000000 amg-player-2023.6.27.0/amg/__init__.py
+-rwxrwxr-x   0 maxime    (1000) maxime    (1000)      123 2021-03-06 17:06:13.000000 amg-player-2023.6.27.0/amg/__main__.py
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)     1040 2021-08-08 17:01:47.000000 amg-player-2023.6.27.0/amg/colored_logging.py
+-rw-r--r--   0 maxime    (1000) maxime    (1000)     4559 2021-08-08 17:01:47.000000 amg-player-2023.6.27.0/amg/menu.py
+-rw-r--r--   0 maxime    (1000) maxime    (1000)      487 2021-03-06 16:51:07.000000 amg-player-2023.6.27.0/amg/mkstemp_ctx.py
+-rw-r--r--   0 maxime    (1000) maxime    (1000)     3429 2023-04-16 20:55:50.000000 amg-player-2023.6.27.0/amg/sanitize.py
+-rw-r--r--   0 maxime    (1000) maxime    (1000)    27017 2023-06-27 21:00:05.000000 amg-player-2023.6.27.0/amg/tag.py
+-rw-r--r--   0 maxime    (1000) maxime    (1000)     2942 2022-05-17 14:22:25.000000 amg-player-2023.6.27.0/amg/ytdl_tqdm.py
+drwxr-xr-x   0 maxime    (1000) maxime    (1000)        0 2023-06-27 21:00:05.667998 amg-player-2023.6.27.0/amg_player.egg-info/
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)     4320 2023-06-27 21:00:05.000000 amg-player-2023.6.27.0/amg_player.egg-info/PKG-INFO
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)      409 2023-06-27 21:00:05.000000 amg-player-2023.6.27.0/amg_player.egg-info/SOURCES.txt
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)        1 2023-06-27 21:00:05.000000 amg-player-2023.6.27.0/amg_player.egg-info/dependency_links.txt
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)       36 2023-06-27 21:00:05.000000 amg-player-2023.6.27.0/amg_player.egg-info/entry_points.txt
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)      215 2023-06-27 21:00:05.000000 amg-player-2023.6.27.0/amg_player.egg-info/requires.txt
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)        4 2023-06-27 21:00:05.000000 amg-player-2023.6.27.0/amg_player.egg-info/top_level.txt
+-rw-r--r--   0 maxime    (1000) maxime    (1000)      216 2023-06-27 21:00:03.000000 amg-player-2023.6.27.0/requirements.txt
+-rw-r--r--   0 maxime    (1000) maxime    (1000)       38 2023-06-27 21:00:05.667998 amg-player-2023.6.27.0/setup.cfg
+-rwxr-xr-x   0 maxime    (1000) maxime    (1000)     1871 2021-03-06 17:11:29.000000 amg-player-2023.6.27.0/setup.py
+drwxr-xr-x   0 maxime    (1000) maxime    (1000)        0 2023-06-27 21:00:05.667998 amg-player-2023.6.27.0/tests/
+-rwxr-xr-x   0 maxime    (1000) maxime    (1000)     4244 2023-04-16 21:14:06.000000 amg-player-2023.6.27.0/tests/__init__.py
```

### Comparing `amg-player-2023.2.8.0/LICENSE` & `amg-player-2023.6.27.0/LICENSE`

 * *Files identical despite different names*

### Comparing `amg-player-2023.2.8.0/PKG-INFO` & `amg-player-2023.6.27.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: amg-player
-Version: 2023.2.8.0
+Version: 2023.6.27.0
 Summary: Browse & play embedded tracks from Angry Metal Guy music reviews
 Home-page: https://github.com/desbma/amg-player
+Download-URL: https://github.com/desbma/amg-player/archive/2023.06.27.0.tar.gz
 Author: desbma
-License: UNKNOWN
-Download-URL: https://github.com/desbma/amg-player/archive/2023.02.8.0.tar.gz
 Keywords: music,metal,extreme,angry,guy,player,youtube,bandcamp,soundcloud
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -92,9 +90,7 @@
 - Play last 20 tracks in chronological order, skipping those already played:
 
   `amg -c 20 -m discover`
 
 ## License
 
 [GPLv3](https://www.gnu.org/licenses/gpl-3.0-standalone.html)
-
-
```

### Comparing `amg-player-2023.2.8.0/README.md` & `amg-player-2023.6.27.0/README.md`

 * *Files identical despite different names*

### Comparing `amg-player-2023.2.8.0/amg/__init__.py` & `amg-player-2023.6.27.0/amg/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python3
 
 """ Browse & play embedded tracks from Angry Metal Guy music reviews. """
 
-__version__ = "2023.02.8.0"
+__version__ = "2023.06.27.0"
 __author__ = "desbma"
 __license__ = "GPLv3"
 
 import argparse
 import codecs
 import collections
 import concurrent.futures
@@ -191,28 +191,25 @@
             iframe = PLAYER_IFRAME_SELECTOR(page)[0]
         except IndexError:
             pass
         else:
             iframe_url = iframe.get("src")
             if iframe_url is not None:
                 yt_prefixes = ("https://www.youtube.com/embed/", "https://www.youtube-nocookie.com/embed/")
-                bc_prefix = "https://bandcamp.com/EmbeddedPlayer/"
+                bc_prefixes = ("https://bandcamp.com/EmbeddedPlayer/", "http://bandcamp.com/EmbeddedPlayer/")
                 sc_prefix = "https://w.soundcloud.com/player/"
                 rn_prefix = "https://www.reverbnation.com/widget_code/"
                 if any(map(iframe_url.startswith, yt_prefixes)):
                     yt_id = urllib.parse.urlparse(iframe_url).path.rsplit("/", 1)[-1]
                     urls = (f"https://www.youtube.com/watch?v={yt_id}",)
-                elif iframe_url.startswith(bc_prefix):
+                elif any(map(iframe_url.startswith, bc_prefixes)):
                     iframe_page = fetch_page(iframe_url, http_cache=http_cache)
                     js = BANDCAMP_JS_SELECTOR(iframe_page)[0]
                     js = js.attrib["data-player-data"]
                     js = json.loads(js)
-                    # import pprint
-                    # pprint.pprint(js)
-                    # exit(7)
                     urls = tuple(t["title_link"] for t in js["tracks"] if (t["track_streaming"] and t["file"]))
                     audio_only = True
                 elif iframe_url.startswith(sc_prefix):
                     urls = (iframe_url.split("&", 1)[0],)
                     audio_only = True
                 elif iframe_url.startswith(rn_prefix):
                     iframe_page = fetch_page(iframe_url, http_cache=http_cache)
```

### Comparing `amg-player-2023.2.8.0/amg/colored_logging.py` & `amg-player-2023.6.27.0/amg/colored_logging.py`

 * *Files identical despite different names*

### Comparing `amg-player-2023.2.8.0/amg/menu.py` & `amg-player-2023.6.27.0/amg/menu.py`

 * *Files identical despite different names*

### Comparing `amg-player-2023.2.8.0/amg/sanitize.py` & `amg-player-2023.6.27.0/amg/sanitize.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,15 +76,15 @@
     punct_followed_uppercase = set(string.punctuation)
     punct_followed_uppercase.remove("'")
     for i, old_word in enumerate(old_words):
         if (
             (prev_word is not None) and ((prev_word[-1] in punct_followed_all_uppercase) and old_word[0].isupper())
         ) or ("." in old_word):
             new_word = old_word
-        elif old_word[0] in "[(-":
+        elif old_word[0] in "[(-'":
             new_word = old_word
         elif old_word.find("'") == 1:
             if i > 0:
                 new_word = "'".join((old_word[0].lower(), old_word[2:].capitalize()))
             else:
                 new_word = old_word
         elif (
```

### Comparing `amg-player-2023.2.8.0/amg/tag.py` & `amg-player-2023.6.27.0/amg/tag.py`

 * *Files 0% similar despite different names*

```diff
@@ -228,14 +228,15 @@
                             expressions.add(w3)
         expressions.update(
             (
                 "full ep",
                 "full-length",
                 "hd",
                 "official",
+                "offical",
                 "pre-listening",
                 "pre-order now",
                 "pre-orders available",
                 "prelistening",
                 "preorders available",
                 "s/t",
                 "sw exclusive",
@@ -290,18 +291,16 @@
     def cleanup(self, title: str) -> str:
         """Do the string cleanup by running all cleaners."""
         cur_title = title
         to_del_indexes: Deque[int] = collections.deque()
         start_index = 0
 
         while self.cleaners:
-
             cleaner: TitleCleanerBase
             for i, (cleaner, args) in enumerate(itertools.islice(self.cleaners, start_index, None), start_index):
-
                 remove_cur_cleaner = False
                 restart_loop = False
 
                 if cleaner.doSkip(cur_title, *args):
                     if cleaner.remove_if_skipped and not cleaner.doKeep():
                         remove_cur_cleaner = True
```

### Comparing `amg-player-2023.2.8.0/amg/ytdl_tqdm.py` & `amg-player-2023.6.27.0/amg/ytdl_tqdm.py`

 * *Files identical despite different names*

### Comparing `amg-player-2023.2.8.0/amg_player.egg-info/PKG-INFO` & `amg-player-2023.6.27.0/amg_player.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: amg-player
-Version: 2023.2.8.0
+Version: 2023.6.27.0
 Summary: Browse & play embedded tracks from Angry Metal Guy music reviews
 Home-page: https://github.com/desbma/amg-player
+Download-URL: https://github.com/desbma/amg-player/archive/2023.06.27.0.tar.gz
 Author: desbma
-License: UNKNOWN
-Download-URL: https://github.com/desbma/amg-player/archive/2023.02.8.0.tar.gz
 Keywords: music,metal,extreme,angry,guy,player,youtube,bandcamp,soundcloud
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -92,9 +90,7 @@
 - Play last 20 tracks in chronological order, skipping those already played:
 
   `amg -c 20 -m discover`
 
 ## License
 
 [GPLv3](https://www.gnu.org/licenses/gpl-3.0-standalone.html)
-
-
```

### Comparing `amg-player-2023.2.8.0/setup.py` & `amg-player-2023.6.27.0/setup.py`

 * *Files identical despite different names*

### Comparing `amg-player-2023.2.8.0/tests/__init__.py` & `amg-player-2023.6.27.0/tests/__init__.py`

 * *Files identical despite different names*

