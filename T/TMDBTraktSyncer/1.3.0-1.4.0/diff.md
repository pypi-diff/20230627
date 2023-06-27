# Comparing `tmp/TMDBTraktSyncer-1.3.0.tar.gz` & `tmp/TMDBTraktSyncer-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TMDBTraktSyncer-1.3.0.tar", last modified: Thu Jun 15 16:56:06 2023, max compression
+gzip compressed data, was "TMDBTraktSyncer-1.4.0.tar", last modified: Tue Jun 27 07:51:49 2023, max compression
```

## Comparing `TMDBTraktSyncer-1.3.0.tar` & `TMDBTraktSyncer-1.4.0.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-06-15 16:56:06.226338 TMDBTraktSyncer-1.3.0/
--rw-rw-rw-   0        0        0     1079 2023-05-21 01:51:26.000000 TMDBTraktSyncer-1.3.0/LICENSE
--rw-rw-rw-   0        0        0    10774 2023-06-15 16:56:06.225338 TMDBTraktSyncer-1.3.0/PKG-INFO
--rw-rw-rw-   0        0        0    10026 2023-06-15 16:29:12.000000 TMDBTraktSyncer-1.3.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-15 16:56:06.194354 TMDBTraktSyncer-1.3.0/TMDBTraktSyncer/
--rw-rw-rw-   0        0        0    16789 2023-06-15 16:10:43.000000 TMDBTraktSyncer-1.3.0/TMDBTraktSyncer/TMDBTraktSyncer.py
--rw-rw-rw-   0        0        0        0 2023-05-21 01:51:26.000000 TMDBTraktSyncer-1.3.0/TMDBTraktSyncer/__init__.py
--rw-rw-rw-   0        0        0     4440 2023-05-28 13:31:50.000000 TMDBTraktSyncer-1.3.0/TMDBTraktSyncer/authTrakt.py
--rw-rw-rw-   0        0        0     9033 2023-06-15 14:40:44.000000 TMDBTraktSyncer-1.3.0/TMDBTraktSyncer/errorHandling.py
--rw-rw-rw-   0        0        0     3977 2023-06-15 14:30:16.000000 TMDBTraktSyncer-1.3.0/TMDBTraktSyncer/tmdbData.py
--rw-rw-rw-   0        0        0     7039 2023-06-15 15:19:15.000000 TMDBTraktSyncer-1.3.0/TMDBTraktSyncer/traktData.py
--rw-rw-rw-   0        0        0     7315 2023-06-15 16:15:40.000000 TMDBTraktSyncer-1.3.0/TMDBTraktSyncer/verifyCredentials.py
-drwxrwxrwx   0        0        0        0 2023-06-15 16:56:06.223338 TMDBTraktSyncer-1.3.0/TMDBTraktSyncer.egg-info/
--rw-rw-rw-   0        0        0    10774 2023-06-15 16:56:06.000000 TMDBTraktSyncer-1.3.0/TMDBTraktSyncer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      481 2023-06-15 16:56:06.000000 TMDBTraktSyncer-1.3.0/TMDBTraktSyncer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-15 16:56:06.000000 TMDBTraktSyncer-1.3.0/TMDBTraktSyncer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       73 2023-06-15 16:56:06.000000 TMDBTraktSyncer-1.3.0/TMDBTraktSyncer.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        9 2023-06-15 16:56:06.000000 TMDBTraktSyncer-1.3.0/TMDBTraktSyncer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-06-15 16:56:06.000000 TMDBTraktSyncer-1.3.0/TMDBTraktSyncer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-15 16:56:06.226338 TMDBTraktSyncer-1.3.0/setup.cfg
--rw-rw-rw-   0        0        0     1341 2023-06-15 16:55:45.000000 TMDBTraktSyncer-1.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-27 07:51:49.837658 TMDBTraktSyncer-1.4.0/
+-rw-rw-rw-   0        0        0     1079 2023-05-21 01:51:26.000000 TMDBTraktSyncer-1.4.0/LICENSE
+-rw-rw-rw-   0        0        0    10839 2023-06-27 07:51:49.836658 TMDBTraktSyncer-1.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0    10091 2023-06-27 07:51:15.000000 TMDBTraktSyncer-1.4.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-27 07:51:49.802660 TMDBTraktSyncer-1.4.0/TMDBTraktSyncer/
+-rw-rw-rw-   0        0        0    18069 2023-06-27 07:32:36.000000 TMDBTraktSyncer-1.4.0/TMDBTraktSyncer/TMDBTraktSyncer.py
+-rw-rw-rw-   0        0        0        0 2023-05-21 01:51:26.000000 TMDBTraktSyncer-1.4.0/TMDBTraktSyncer/__init__.py
+-rw-rw-rw-   0        0        0     4548 2023-06-27 07:34:14.000000 TMDBTraktSyncer-1.4.0/TMDBTraktSyncer/authTrakt.py
+-rw-rw-rw-   0        0        0    10181 2023-06-27 07:45:31.000000 TMDBTraktSyncer-1.4.0/TMDBTraktSyncer/errorHandling.py
+-rw-rw-rw-   0        0        0     1669 2023-06-27 07:34:28.000000 TMDBTraktSyncer-1.4.0/TMDBTraktSyncer/errorLogger.py
+-rw-rw-rw-   0        0        0     4058 2023-06-27 07:33:19.000000 TMDBTraktSyncer-1.4.0/TMDBTraktSyncer/tmdbData.py
+-rw-rw-rw-   0        0        0     7120 2023-06-27 07:33:10.000000 TMDBTraktSyncer-1.4.0/TMDBTraktSyncer/traktData.py
+-rw-rw-rw-   0        0        0     8014 2023-06-27 07:36:59.000000 TMDBTraktSyncer-1.4.0/TMDBTraktSyncer/verifyCredentials.py
+drwxrwxrwx   0        0        0        0 2023-06-27 07:51:49.835658 TMDBTraktSyncer-1.4.0/TMDBTraktSyncer.egg-info/
+-rw-rw-rw-   0        0        0    10839 2023-06-27 07:51:49.000000 TMDBTraktSyncer-1.4.0/TMDBTraktSyncer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      512 2023-06-27 07:51:49.000000 TMDBTraktSyncer-1.4.0/TMDBTraktSyncer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-27 07:51:49.000000 TMDBTraktSyncer-1.4.0/TMDBTraktSyncer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       73 2023-06-27 07:51:49.000000 TMDBTraktSyncer-1.4.0/TMDBTraktSyncer.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        9 2023-06-27 07:51:49.000000 TMDBTraktSyncer-1.4.0/TMDBTraktSyncer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-06-27 07:51:49.000000 TMDBTraktSyncer-1.4.0/TMDBTraktSyncer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-27 07:51:49.838659 TMDBTraktSyncer-1.4.0/setup.cfg
+-rw-rw-rw-   0        0        0     1341 2023-06-27 07:50:17.000000 TMDBTraktSyncer-1.4.0/setup.py
```

### Comparing `TMDBTraktSyncer-1.3.0/LICENSE` & `TMDBTraktSyncer-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `TMDBTraktSyncer-1.3.0/PKG-INFO` & `TMDBTraktSyncer-1.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TMDBTraktSyncer
-Version: 1.3.0
+Version: 1.4.0
 Summary: A python script that syncs user watchlist and ratings for Movies, TV Shows and Episodes both ways between Trakt and TMDB.
 Home-page: https://github.com/RileyXX/TMDB-Trakt-Syncer
 Author: RileyXX
 Keywords: python,video,trakt,tmdb,ratings,sync,movies,tv shows
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Programming Language :: Python :: 3
@@ -79,15 +79,14 @@
 - Setup Automation for:
    - [Windows](https://github.com/RileyXX/TMDB-Trakt-Syncer/wiki/Setting-Up-Automation-on-Windows)
    - [Linux](https://github.com/RileyXX/TMDB-Trakt-Syncer/wiki/Setting-Up-Automation-on-Linux)
    - [macOS](https://github.com/RileyXX/TMDB-Trakt-Syncer/wiki/Setting-Up-Automation-on-macOS)
 - Python Script to Update all Packages with Pip (Windows, Linux, Mac, ChromeOS, etc.) [Link #1](https://github.com/RileyXX/TMDB-Trakt-Syncer/wiki/Python-Script-to-Update-all-Packages-with-Pip-\(Windows,-Linux,-Mac,-ChromeOS,-etc\))
 
 ## Troubleshooting, Known Issues, Workarounds & Future Outlook:
-* Add optional setting to remove watched items from watchlists [Issue #15](https://github.com/RileyXX/TMDB-Trakt-Syncer/issues/15)
 * Add support for review/comment sync [Issue #1](https://github.com/RileyXX/TMDB-Trakt-Syncer/issues/1)
 * If any of your details change (passwords, logins, API keys, etc.), simply open `credentials.txt`, modify your details, save it and then run the script again. Alternatively, delete `credentials.txt` to reset the script and it will prompt you to enter your new details on the next run.
 
 ## Screenshot:
 ![Demo](https://i.imgur.com/5LI04O2.png)
 
 ## Sponsorships, Donations, and Custom Projects:
@@ -112,14 +111,15 @@
 | Project Name | Description |
 |--------------|-------------|
 | [PlexTraktSync](https://github.com/Taxel/PlexTraktSync) | A script that syncs user watch history and ratings between Trakt and Plex (without needing a PlexPass or Trakt VIP subscription). |
 | [IMDB-Trakt-Syncer](https://github.com/RileyXX/IMDB-Trakt-Syncer) | A script that syncs user watchlist, ratings, and comments both ways between Trakt and IMDB. |
 | [TMDB-Trakt-Syncer](https://github.com/RileyXX/TMDB-Trakt-Syncer) | A script that syncs user watchlist and ratings both ways between Trakt and TMDB. |
 | [PlexPreferNonForcedSubs](https://github.com/RileyXX/PlexPreferNonForcedSubs) | A script that sets all movies and shows in your local Plex library to English non-forced subtitles by default. |
 | [Casvt / PlexAutoDelete](https://github.com/Casvt/Plex-scripts/blob/main/changing_settings/plex_auto_delete.py) | A script for automatically deleting watched content from Plex. |
+| [universal-trakt-scrobbler](https://github.com/trakt-tools/universal-trakt-scrobbler) | An extension that automatically scrobbles TV shows and Movies from several streaming services to Trakt. |
 | [Netflix-to-Trakt-Import](https://github.com/jensb89/Netflix-to-Trakt-Import) | A tool to import your Netflix viewing history into Trakt. |
 | [trakt-tv-backup](https://darekkay.com/blog/trakt-tv-backup/) | A command-line tool for backing up your Trakt.tv data. |
 | [blacktwin / JBOPS](https://github.com/blacktwin/JBOPS) | A collection of scripts and tools for enhancing and automating tasks in Plex. |
 | [Casvt / Plex-scripts](https://github.com/Casvt/Plex-scripts) | A collection of useful scripts for Plex automation and management. |
 | [trakt---letterboxd-import](https://github.com/jensb89/trakt---letterboxd-import) | A tool to import your Letterboxd ratings and watchlist into Trakt. |
 | [TraktRater](https://github.com/damienhaynes/TraktRater/) | A tool to help users transfer user episode, show, and movie user ratings and watchlists from multiple media database sites around the web. |
 | [TvTimeToTrakt](https://github.com/lukearran/TvTimeToTrakt) | A tool to sync your TV Time watch history with Trakt.tv. |
```

### Comparing `TMDBTraktSyncer-1.3.0/README.md` & `TMDBTraktSyncer-1.4.0/TMDBTraktSyncer.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,118 +1,134 @@
-# TMDB-Trakt-Syncer
-
-This Python script syncs user watchlist and ratings for Movies, TV Shows, and Episodes both ways between [Trakt](https://trakt.tv/) and [TMDB](https://www.themoviedb.org/). Data already set will not be overwritten. Ratings and watchlist sync are both optional. The user will be prompted to enter their settings and api keys on first run.
-
-The script is compatible on any operating system that supports Python v3.6 or later, including Windows, Linux, Mac, and ChromeOS. If you're interested in syncing ratings between Trakt, Plex, IMDB, and TMDB, I recommend the following projects: [PlexTraktSync](https://github.com/Taxel/PlexTraktSync), [IMDB-Trakt-Syncer](https://github.com/RileyXX/IMDB-Trakt-Syncer), and [TMDB-Trakt-Syncer](https://github.com/RileyXX/TMDB-Trakt-Syncer). See below for my other [recommended projects](https://github.com/RileyXX/TMDB-Trakt-Syncer#other-recommended-projects).
-
-## Installation Instructions:
-1. Install [Python](https://www.python.org/downloads/) (v3.6 or later).
-2. Install the script by running `python -m pip install TMDBTraktSyncer` in command line.
-3. Login to [Trakt](https://trakt.tv/oauth/applications) and create a new API application named `TMDbTraktSyncer`. In the "Redirect uri" field, enter `urn:ietf:wg:oauth:2.0:oob`, then save the application.
-4. Login to [TMDB](https://www.themoviedb.org/settings/api/) and create a new API application. Choose "Developer" and accept the terms. Fill out the application form as follows: 
-   - Type of use: `Personal`
-   - Application name: `TMDB-Trakt-Sync`
-   - Application URL: `https://github.com/RileyXX/TMDB-Trakt-Syncer`
-   - Application summary: `Use TMDB API and Trakt API to sync user ratings between platforms.`
-   - Fill in the rest of the fields as desired and submit the form. Your API keys will be generated instantly.
-5. Run the script by running `TMDBTraktSyncer` in the command line.
-6. Follow the prompts during the first run. You will need to enter your Trakt `client ID` and `client secret` from step 3, as well as your `tmdb_v4_token` from step 4. Please note that these details are saved insecurely as `credentials.txt` in the same folder as the script.
-7. Setup is complete. The script will continue running and syncing your ratings. You can monitor its progress in the command line.
-
-## Installing the Script:
-```
-python -m pip install TMDBTraktSyncer
-```
-_Run in your operating system's native command line._
-## Running the Script:
-```
-TMDBTraktSyncer
-```
-_Run in your operating system's native command line._
-## Updating the Script:
-```
-python -m pip install TMDBTraktSyncer --upgrade
-```
-_Run in your operating system's native command line._
-## Uninstalling the Script:
-```
-python -m pip uninstall TMDBTraktSyncer
-```
-_Run in your operating system's native command line._
-
-## Installing a Specific Version:
-```
-python -m pip install TMDBTraktSyncer==VERSION_NUMBER
-```
-_Replace `VERSION_NUMBER` with your [desired version](https://github.com/RileyXX/TMDB-Trakt-Syncer/releases) (e.g. 1.0.1) and run in your operating system's native command line._
-
-## Alternative Manual Installation Method (without pip install):
-1. Install [Python](https://www.python.org/downloads/) (v3.6 or later).
-2. Download the latest .zip from the [releases page](https://github.com/RileyXX/TMDB-Trakt-Syncer/releases) and extract it to the desired directory.
-3. Login to [Trakt](https://trakt.tv/oauth/applications) and create a new API application named `TMDBTraktSyncer`. In the "Redirect uri" field, enter `urn:ietf:wg:oauth:2.0:oob`, then save the application.
-4. Login to [TMDB](https://www.themoviedb.org/settings/api/) and create a new API application. Choose "Developer" and accept the terms. Fill out the application form as follows: 
-   - Type of use: `Personal`
-   - Application name: `TMDB-Trakt-Sync`
-   - Application URL: `https://github.com/RileyXX/TMDB-Trakt-Syncer`
-   - Application summary: `Use TMDB API and Trakt API to sync user ratings between platforms.`
-   - Fill in the rest of the fields as desired and submit the form. Your API keys will be generated instantly.
-5. Run `TMDBTraktSyncer.py` or open the terminal and navigate to the folder where `TMDBTraktSyncer.py` is located, then run `TMDBTraktSyncer.py` in the terminal.
-6. Follow the prompts during the first run. You will need to enter your Trakt `client ID` and `client secret` from step 3, as well as your `tmdb_v4_token` from step 4. Please note that these details are saved insecurely as `credentials.txt` in the same folder as the script.
-7. Setup is complete. The script will continue running and syncing your ratings. You can monitor its progress in the command line.
-
-## For Setting Up Automation See the Following Wiki Pages:
-- Setup Automation for:
-   - [Windows](https://github.com/RileyXX/TMDB-Trakt-Syncer/wiki/Setting-Up-Automation-on-Windows)
-   - [Linux](https://github.com/RileyXX/TMDB-Trakt-Syncer/wiki/Setting-Up-Automation-on-Linux)
-   - [macOS](https://github.com/RileyXX/TMDB-Trakt-Syncer/wiki/Setting-Up-Automation-on-macOS)
-- Python Script to Update all Packages with Pip (Windows, Linux, Mac, ChromeOS, etc.) [Link #1](https://github.com/RileyXX/TMDB-Trakt-Syncer/wiki/Python-Script-to-Update-all-Packages-with-Pip-\(Windows,-Linux,-Mac,-ChromeOS,-etc\))
-
-## Troubleshooting, Known Issues, Workarounds & Future Outlook:
-* Add optional setting to remove watched items from watchlists [Issue #15](https://github.com/RileyXX/TMDB-Trakt-Syncer/issues/15)
-* Add support for review/comment sync [Issue #1](https://github.com/RileyXX/TMDB-Trakt-Syncer/issues/1)
-* If any of your details change (passwords, logins, API keys, etc.), simply open `credentials.txt`, modify your details, save it and then run the script again. Alternatively, delete `credentials.txt` to reset the script and it will prompt you to enter your new details on the next run.
-
-## Screenshot:
-![Demo](https://i.imgur.com/5LI04O2.png)
-
-## Sponsorships, Donations, and Custom Projects:
-If you find my scripts helpful, you can become a [sponsor](https://github.com/sponsors/RileyXX) and support my projects! If you need help with a project, open an issue, and I'll do my best to assist you. For other inquiries and custom projects, you can contact me on [Twitter](https://twitter.com/RileyxBell).
-
-#### More Donation Options:
-- Cashapp: `$rileyxx`
-- Venmo: `@rileyxx`
-- Bitcoin: `bc1qrjevwqv49z8y77len3azqfghxrjmrjvhy5zqau`
-- Amazon Wishlist: [Link ↗](https://www.amazon.com/hz/wishlist/ls/WURF5NWZ843U)
-
-## Also Posted on:
-* [PyPi](https://pypi.org/project/TMDBTraktSyncer/)
-* [Reddit](https://www.reddit.com/r/trakt/comments/13jlu4r/tmdb_trakt_rating_syncer_tool_2_way_sync/)
-
-<br>
-
-[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
-
-## Other Recommended Projects:
-
-| Project Name | Description |
-|--------------|-------------|
-| [PlexTraktSync](https://github.com/Taxel/PlexTraktSync) | A script that syncs user watch history and ratings between Trakt and Plex (without needing a PlexPass or Trakt VIP subscription). |
-| [IMDB-Trakt-Syncer](https://github.com/RileyXX/IMDB-Trakt-Syncer) | A script that syncs user watchlist, ratings, and comments both ways between Trakt and IMDB. |
-| [TMDB-Trakt-Syncer](https://github.com/RileyXX/TMDB-Trakt-Syncer) | A script that syncs user watchlist and ratings both ways between Trakt and TMDB. |
-| [PlexPreferNonForcedSubs](https://github.com/RileyXX/PlexPreferNonForcedSubs) | A script that sets all movies and shows in your local Plex library to English non-forced subtitles by default. |
-| [Casvt / PlexAutoDelete](https://github.com/Casvt/Plex-scripts/blob/main/changing_settings/plex_auto_delete.py) | A script for automatically deleting watched content from Plex. |
-| [Netflix-to-Trakt-Import](https://github.com/jensb89/Netflix-to-Trakt-Import) | A tool to import your Netflix viewing history into Trakt. |
-| [trakt-tv-backup](https://darekkay.com/blog/trakt-tv-backup/) | A command-line tool for backing up your Trakt.tv data. |
-| [blacktwin / JBOPS](https://github.com/blacktwin/JBOPS) | A collection of scripts and tools for enhancing and automating tasks in Plex. |
-| [Casvt / Plex-scripts](https://github.com/Casvt/Plex-scripts) | A collection of useful scripts for Plex automation and management. |
-| [trakt---letterboxd-import](https://github.com/jensb89/trakt---letterboxd-import) | A tool to import your Letterboxd ratings and watchlist into Trakt. |
-| [TraktRater](https://github.com/damienhaynes/TraktRater/) | A tool to help users transfer user episode, show, and movie user ratings and watchlists from multiple media database sites around the web. |
-| [TvTimeToTrakt](https://github.com/lukearran/TvTimeToTrakt) | A tool to sync your TV Time watch history with Trakt.tv. |
-| [Plex Media Server](https://www.plex.tv/media-server-downloads/#plex-app) | A media server software to organize and stream your personal media collection. |
-| [Radarr](https://github.com/Radarr/Radarr) | A movie collection manager and downloader for various platforms. |
-| [Sonarr](https://github.com/Sonarr/Sonarr) | A TV show collection manager and downloader for various platforms. |
-| [Jackett](https://github.com/Jackett/Jackett) | A proxy server that provides API support for various torrent trackers commonly used with Radarr and Sonarr. |
-| [qBittorrent](https://github.com/qbittorrent/qBittorrent) | A free and open-source BitTorrent client. |
-| [Mullvad VPN](https://github.com/mullvad/mullvadvpn-app) | An open-source VPN client for Mullvad VPN service with port forwarding support. Great VPN for torrents. |
-| [Overseerr](https://github.com/sct/overseerr) | A request management and media discovery tool for your home media server. |
-| [FlareSolverr](https://github.com/FlareSolverr/FlareSolverr) | A reverse proxy solution to bypass Cloudflare protection and access websites commonly used with Jackett. |
-| [youtube-dl](https://github.com/ytdl-org/youtube-dl) | A command-line program to download videos from YouTube and other sites. |
+Metadata-Version: 2.1
+Name: TMDBTraktSyncer
+Version: 1.4.0
+Summary: A python script that syncs user watchlist and ratings for Movies, TV Shows and Episodes both ways between Trakt and TMDB.
+Home-page: https://github.com/RileyXX/TMDB-Trakt-Syncer
+Author: RileyXX
+Keywords: python,video,trakt,tmdb,ratings,sync,movies,tv shows
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: End Users/Desktop
+Classifier: Programming Language :: Python :: 3
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+
+# TMDB-Trakt-Syncer
+
+This Python script syncs user watchlist and ratings for Movies, TV Shows, and Episodes both ways between [Trakt](https://trakt.tv/) and [TMDB](https://www.themoviedb.org/). Data already set will not be overwritten. Ratings and watchlist sync are both optional. The user will be prompted to enter their settings and api keys on first run.
+
+The script is compatible on any operating system that supports Python v3.6 or later, including Windows, Linux, Mac, and ChromeOS. If you're interested in syncing ratings between Trakt, Plex, IMDB, and TMDB, I recommend the following projects: [PlexTraktSync](https://github.com/Taxel/PlexTraktSync), [IMDB-Trakt-Syncer](https://github.com/RileyXX/IMDB-Trakt-Syncer), and [TMDB-Trakt-Syncer](https://github.com/RileyXX/TMDB-Trakt-Syncer). See below for my other [recommended projects](https://github.com/RileyXX/TMDB-Trakt-Syncer#other-recommended-projects).
+
+## Installation Instructions:
+1. Install [Python](https://www.python.org/downloads/) (v3.6 or later).
+2. Install the script by running `python -m pip install TMDBTraktSyncer` in command line.
+3. Login to [Trakt](https://trakt.tv/oauth/applications) and create a new API application named `TMDbTraktSyncer`. In the "Redirect uri" field, enter `urn:ietf:wg:oauth:2.0:oob`, then save the application.
+4. Login to [TMDB](https://www.themoviedb.org/settings/api/) and create a new API application. Choose "Developer" and accept the terms. Fill out the application form as follows: 
+   - Type of use: `Personal`
+   - Application name: `TMDB-Trakt-Sync`
+   - Application URL: `https://github.com/RileyXX/TMDB-Trakt-Syncer`
+   - Application summary: `Use TMDB API and Trakt API to sync user ratings between platforms.`
+   - Fill in the rest of the fields as desired and submit the form. Your API keys will be generated instantly.
+5. Run the script by running `TMDBTraktSyncer` in the command line.
+6. Follow the prompts during the first run. You will need to enter your Trakt `client ID` and `client secret` from step 3, as well as your `tmdb_v4_token` from step 4. Please note that these details are saved insecurely as `credentials.txt` in the same folder as the script.
+7. Setup is complete. The script will continue running and syncing your ratings. You can monitor its progress in the command line.
+
+## Installing the Script:
+```
+python -m pip install TMDBTraktSyncer
+```
+_Run in your operating system's native command line._
+## Running the Script:
+```
+TMDBTraktSyncer
+```
+_Run in your operating system's native command line._
+## Updating the Script:
+```
+python -m pip install TMDBTraktSyncer --upgrade
+```
+_Run in your operating system's native command line._
+## Uninstalling the Script:
+```
+python -m pip uninstall TMDBTraktSyncer
+```
+_Run in your operating system's native command line._
+
+## Installing a Specific Version:
+```
+python -m pip install TMDBTraktSyncer==VERSION_NUMBER
+```
+_Replace `VERSION_NUMBER` with your [desired version](https://github.com/RileyXX/TMDB-Trakt-Syncer/releases) (e.g. 1.0.1) and run in your operating system's native command line._
+
+## Alternative Manual Installation Method (without pip install):
+1. Install [Python](https://www.python.org/downloads/) (v3.6 or later).
+2. Download the latest .zip from the [releases page](https://github.com/RileyXX/TMDB-Trakt-Syncer/releases) and extract it to the desired directory.
+3. Login to [Trakt](https://trakt.tv/oauth/applications) and create a new API application named `TMDBTraktSyncer`. In the "Redirect uri" field, enter `urn:ietf:wg:oauth:2.0:oob`, then save the application.
+4. Login to [TMDB](https://www.themoviedb.org/settings/api/) and create a new API application. Choose "Developer" and accept the terms. Fill out the application form as follows: 
+   - Type of use: `Personal`
+   - Application name: `TMDB-Trakt-Sync`
+   - Application URL: `https://github.com/RileyXX/TMDB-Trakt-Syncer`
+   - Application summary: `Use TMDB API and Trakt API to sync user ratings between platforms.`
+   - Fill in the rest of the fields as desired and submit the form. Your API keys will be generated instantly.
+5. Run `TMDBTraktSyncer.py` or open the terminal and navigate to the folder where `TMDBTraktSyncer.py` is located, then run `TMDBTraktSyncer.py` in the terminal.
+6. Follow the prompts during the first run. You will need to enter your Trakt `client ID` and `client secret` from step 3, as well as your `tmdb_v4_token` from step 4. Please note that these details are saved insecurely as `credentials.txt` in the same folder as the script.
+7. Setup is complete. The script will continue running and syncing your ratings. You can monitor its progress in the command line.
+
+## For Setting Up Automation See the Following Wiki Pages:
+- Setup Automation for:
+   - [Windows](https://github.com/RileyXX/TMDB-Trakt-Syncer/wiki/Setting-Up-Automation-on-Windows)
+   - [Linux](https://github.com/RileyXX/TMDB-Trakt-Syncer/wiki/Setting-Up-Automation-on-Linux)
+   - [macOS](https://github.com/RileyXX/TMDB-Trakt-Syncer/wiki/Setting-Up-Automation-on-macOS)
+- Python Script to Update all Packages with Pip (Windows, Linux, Mac, ChromeOS, etc.) [Link #1](https://github.com/RileyXX/TMDB-Trakt-Syncer/wiki/Python-Script-to-Update-all-Packages-with-Pip-\(Windows,-Linux,-Mac,-ChromeOS,-etc\))
+
+## Troubleshooting, Known Issues, Workarounds & Future Outlook:
+* Add support for review/comment sync [Issue #1](https://github.com/RileyXX/TMDB-Trakt-Syncer/issues/1)
+* If any of your details change (passwords, logins, API keys, etc.), simply open `credentials.txt`, modify your details, save it and then run the script again. Alternatively, delete `credentials.txt` to reset the script and it will prompt you to enter your new details on the next run.
+
+## Screenshot:
+![Demo](https://i.imgur.com/5LI04O2.png)
+
+## Sponsorships, Donations, and Custom Projects:
+If you find my scripts helpful, you can become a [sponsor](https://github.com/sponsors/RileyXX) and support my projects! If you need help with a project, open an issue, and I'll do my best to assist you. For other inquiries and custom projects, you can contact me on [Twitter](https://twitter.com/RileyxBell).
+
+#### More Donation Options:
+- Cashapp: `$rileyxx`
+- Venmo: `@rileyxx`
+- Bitcoin: `bc1qrjevwqv49z8y77len3azqfghxrjmrjvhy5zqau`
+- Amazon Wishlist: [Link ↗](https://www.amazon.com/hz/wishlist/ls/WURF5NWZ843U)
+
+## Also Posted on:
+* [PyPi](https://pypi.org/project/TMDBTraktSyncer/)
+* [Reddit](https://www.reddit.com/r/trakt/comments/13jlu4r/tmdb_trakt_rating_syncer_tool_2_way_sync/)
+
+<br>
+
+[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
+
+## Other Recommended Projects:
+
+| Project Name | Description |
+|--------------|-------------|
+| [PlexTraktSync](https://github.com/Taxel/PlexTraktSync) | A script that syncs user watch history and ratings between Trakt and Plex (without needing a PlexPass or Trakt VIP subscription). |
+| [IMDB-Trakt-Syncer](https://github.com/RileyXX/IMDB-Trakt-Syncer) | A script that syncs user watchlist, ratings, and comments both ways between Trakt and IMDB. |
+| [TMDB-Trakt-Syncer](https://github.com/RileyXX/TMDB-Trakt-Syncer) | A script that syncs user watchlist and ratings both ways between Trakt and TMDB. |
+| [PlexPreferNonForcedSubs](https://github.com/RileyXX/PlexPreferNonForcedSubs) | A script that sets all movies and shows in your local Plex library to English non-forced subtitles by default. |
+| [Casvt / PlexAutoDelete](https://github.com/Casvt/Plex-scripts/blob/main/changing_settings/plex_auto_delete.py) | A script for automatically deleting watched content from Plex. |
+| [universal-trakt-scrobbler](https://github.com/trakt-tools/universal-trakt-scrobbler) | An extension that automatically scrobbles TV shows and Movies from several streaming services to Trakt. |
+| [Netflix-to-Trakt-Import](https://github.com/jensb89/Netflix-to-Trakt-Import) | A tool to import your Netflix viewing history into Trakt. |
+| [trakt-tv-backup](https://darekkay.com/blog/trakt-tv-backup/) | A command-line tool for backing up your Trakt.tv data. |
+| [blacktwin / JBOPS](https://github.com/blacktwin/JBOPS) | A collection of scripts and tools for enhancing and automating tasks in Plex. |
+| [Casvt / Plex-scripts](https://github.com/Casvt/Plex-scripts) | A collection of useful scripts for Plex automation and management. |
+| [trakt---letterboxd-import](https://github.com/jensb89/trakt---letterboxd-import) | A tool to import your Letterboxd ratings and watchlist into Trakt. |
+| [TraktRater](https://github.com/damienhaynes/TraktRater/) | A tool to help users transfer user episode, show, and movie user ratings and watchlists from multiple media database sites around the web. |
+| [TvTimeToTrakt](https://github.com/lukearran/TvTimeToTrakt) | A tool to sync your TV Time watch history with Trakt.tv. |
+| [Plex Media Server](https://www.plex.tv/media-server-downloads/#plex-app) | A media server software to organize and stream your personal media collection. |
+| [Radarr](https://github.com/Radarr/Radarr) | A movie collection manager and downloader for various platforms. |
+| [Sonarr](https://github.com/Sonarr/Sonarr) | A TV show collection manager and downloader for various platforms. |
+| [Jackett](https://github.com/Jackett/Jackett) | A proxy server that provides API support for various torrent trackers commonly used with Radarr and Sonarr. |
+| [qBittorrent](https://github.com/qbittorrent/qBittorrent) | A free and open-source BitTorrent client. |
+| [Mullvad VPN](https://github.com/mullvad/mullvadvpn-app) | An open-source VPN client for Mullvad VPN service with port forwarding support. Great VPN for torrents. |
+| [Overseerr](https://github.com/sct/overseerr) | A request management and media discovery tool for your home media server. |
+| [FlareSolverr](https://github.com/FlareSolverr/FlareSolverr) | A reverse proxy solution to bypass Cloudflare protection and access websites commonly used with Jackett. |
+| [youtube-dl](https://github.com/ytdl-org/youtube-dl) | A command-line program to download videos from YouTube and other sites. |
```

### Comparing `TMDBTraktSyncer-1.3.0/TMDBTraktSyncer/TMDBTraktSyncer.py` & `TMDBTraktSyncer-1.4.0/TMDBTraktSyncer/TMDBTraktSyncer.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,19 +2,21 @@
 import requests
 import time
 try:
     from TMDBTraktSyncer import verifyCredentials as VC
     from TMDBTraktSyncer import traktData
     from TMDBTraktSyncer import tmdbData
     from TMDBTraktSyncer import errorHandling as EH
+    from TMDBTraktSyncer import errorLogger as EL
 except ImportError:
     import verifyCredentials as VC
     import traktData
     import tmdbData
     import errorHandling as EH
+    import errorLogger as EL
 
 
 def main():
     try:
             
         trakt_watchlist, trakt_ratings, watched_content = traktData.getTraktData()
         tmdb_watchlist, tmdb_ratings = tmdbData.getTMDBRatings()
@@ -59,32 +61,34 @@
                 
                 # Count the total number of items
                 num_items = len(tmdb_watchlist_to_set)
                 item_count = 0
                 
                 for item in tmdb_watchlist_to_set:
                     item_count += 1
+                    print(f" - Adding item ({item_count} of {num_items}): {item['Title']} ({item['Year']}) to TMDB Watchlist")
                     payload = {}  # Add any additional payload parameters if required
                     if item['Type'] == 'movie':
                         url = f"https://api.themoviedb.org/3/account/{account_id}/watchlist"
                         payload['media_type'] = "movie"
                         payload['media_id'] = item['TMDB_ID']
                         payload['watchlist'] = True
                         response = EH.make_tmdb_request(url, payload=payload)
 
                     elif item['Type'] == 'show':
                         url = f"https://api.themoviedb.org/3/account/{account_id}/watchlist"
                         payload['media_type'] = "tv"
                         payload['media_id'] = item['TMDB_ID']
                         payload['watchlist'] = True
                         response = EH.make_tmdb_request(url, payload=payload)
-                    if response:
-                        print(f"Adding item ({item_count} of {num_items}): {item['Title']} ({item['Year']}) to TMDB Watchlist")
-                    else:
-                        print(f"Failed to add item ({item_count} of {num_items}): {item['Title']} ({item['Year']}) to TMDB Watchlist (TMDB ID: {item['TMDB_ID']})")
+                    
+                    if response is None:
+                        error_message = f"Failed to add item ({item_count} of {num_items}): {item['Title']} ({item['Year']}) to TMDB Watchlist (TMDB ID: {item['TMDB_ID']})"
+                        print(f"   - {error_message}")
+                        EL.logger.error(error_message)
                 
                 print('Setting TMDB Watchlist Items Complete')
             else:
                 print('No TMDB Watchlist Items To Set')
 
             # Set Trakt Watchlist Items
             if trakt_watchlist_to_set:
@@ -92,14 +96,15 @@
 
                 # Count the total number of items
                 num_items = len(trakt_watchlist_to_set)
                 item_count = 0
 
                 for item in trakt_watchlist_to_set:
                     item_count += 1
+                    print(f" - Adding item ({item_count} of {num_items}): {item['Title']} ({item['Year']}) to Trakt Watchlist")
                     tmdb_id = item['TMDB_ID']
                     media_type = item['Type']  # 'movie', 'show', or 'episode'
 
                     url = f"https://api.trakt.tv/sync/watchlist"
 
                     data = {
                         "movies": [],
@@ -123,19 +128,19 @@
                         data['episodes'].append({
                             "ids": {
                                 "tmdb": tmdb_id
                             }
                         })
 
                     response = EH.make_trakt_request(url, payload=data)
-                    if response:
-                        print(f"Adding item ({item_count} of {num_items}): {item['Title']} ({item['Year']}) to Trakt Watchlist")
-                    else:
-                        print(f"Failed to add item ({item_count} of {num_items}): {item['Title']} ({item['Year']}) to Trakt Watchlist (TMDB ID: {item['TMDB_ID']})")
-                        print("Error Response:", response.content, response.status_code)
+                    
+                    if response is None:
+                        error_message = f"Failed to add item ({item_count} of {num_items}): {item['Title']} ({item['Year']}) to Trakt Watchlist (TMDB ID: {item['TMDB_ID']})"
+                        print(f"   - {error_message}")
+                        EL.logger.error(error_message)
 
                 print('Setting Trakt Watchlist Items Complete')
             else:
                 print('No Trakt Watchlist Items To Set')
 
         # If sync_ratings_value is true
         if VC.sync_ratings_value:
@@ -153,31 +158,36 @@
                     item_count += 1
 
                     if item['Type'] == 'movie':
                         payload = {
                             'value': item['Rating']
                         }
                         url = f"https://api.themoviedb.org/3/movie/{item['TMDB_ID']}/rating"
-                        print(f"Rating movie ({item_count} of {num_items}): {item['Title']} ({item['Year']}): {item['Rating']}/10 on TMDB")
+                        print(f" - Rating movie ({item_count} of {num_items}): {item['Title']} ({item['Year']}): {item['Rating']}/10 on TMDB")
 
                     elif item['Type'] == 'show':
                         payload = {
                             'value': item['Rating']
                         }
                         url = f"https://api.themoviedb.org/3/tv/{item['TMDB_ID']}/rating"
-                        print(f"Rating TV show ({item_count} of {num_items}): {item['Title']} ({item['Year']}): {item['Rating']}/10 on TMDB")
+                        print(f" - Rating TV show ({item_count} of {num_items}): {item['Title']} ({item['Year']}): {item['Rating']}/10 on TMDB")
 
                     elif item['Type'] == 'episode':
                         payload = {
                             'value': item['Rating']
                         }
                         url = f"https://api.themoviedb.org/3/tv/{item['TMDB_ShowID']}/season/{item['Season']}/episode/{item['Episode']}/rating"
-                        print(f"Rating episode ({item_count} of {num_items}): {item['Title']} ({item['Year']}) [S{item['Season']:02d}E{item['Episode']:02d}]: {item['Rating']}/10 on TMDB")
+                        print(f" - Rating episode ({item_count} of {num_items}): {item['Title']} ({item['Year']}) [S{item['Season']:02d}E{item['Episode']:02d}]: {item['Rating']}/10 on TMDB")
 
                     response = EH.make_tmdb_request(url, payload=payload)
+                    
+                    if response is None:
+                        error_message = f"Failed rating item ({item_count} of {num_items}): {item['Title']} ({item['Year']}): {item['Rating']}/10 on TMDB"
+                        print(f"   - {error_message}")
+                        EL.logger.error(error_message)
 
                 print('Setting TMDB Ratings Complete')
             else:
                 print('No TMDB Ratings To Set')
 
             # Set Trakt Ratings
             if trakt_ratings_to_set:
@@ -199,40 +209,45 @@
                             "shows": [{
                                 "ids": {
                                     "tmdb": item["TMDB_ID"]
                                 },
                                 "rating": item["Rating"]
                             }]
                         }
-                        print(f"Rating TV show ({item_count} of {num_items}): {item['Title']} ({item['Year']}): {item['Rating']}/10 on Trakt")
+                        print(f" - Rating TV show ({item_count} of {num_items}): {item['Title']} ({item['Year']}): {item['Rating']}/10 on Trakt")
                     elif item["Type"] == "movie":
                         # This is a movie
                         data = {
                             "movies": [{
                                 "ids": {
                                     "tmdb": item["TMDB_ID"]
                                 },
                                 "rating": item["Rating"]
                             }]
                         }
-                        print(f"Rating movie ({item_count} of {num_items}): {item['Title']} ({item['Year']}): {item['Rating']}/10 on Trakt")
+                        print(f" - Rating movie ({item_count} of {num_items}): {item['Title']} ({item['Year']}): {item['Rating']}/10 on Trakt")
                     elif item["Type"] == "episode":
                         # This is an episode
                         data = {
                             "episodes": [{
                                 "ids": {
                                     "tmdb": item["TMDB_ID"]
                                 },
                                 "rating": item["Rating"]
                             }]
                         }
-                        print(f"Rating episode ({item_count} of {num_items}): {item['Title']} ({item['Year']}) [S{item['Season']:02d}E{item['Episode']:02d}]: {item['Rating']}/10 on Trakt")
+                        print(f" - Rating episode ({item_count} of {num_items}): {item['Title']} ({item['Year']}) [S{item['Season']:02d}E{item['Episode']:02d}]: {item['Rating']}/10 on Trakt")
 
                     # Make the API call to rate the item
                     response = EH.make_trakt_request(rate_url, payload=data)
+                    
+                    if response is None:
+                        error_message = f"Failed rating item ({item_count} of {num_items}): {item['Title']} ({item['Year']}): {item['Rating']}/10 on Trakt"
+                        print(f"   - {error_message}")
+                        EL.logger.error(error_message)
 
                 print('Setting Trakt Ratings Complete')
             else:
                 print('No Trakt Ratings To Set')
         
         # If remove_watched_from_watchlists_value is true
         if VC.remove_watched_from_watchlists_value:
@@ -256,41 +271,43 @@
                         data = {
                             "shows": [{
                                 "ids": {
                                     "trakt": item["TraktID"]
                                 }
                             }]
                         }
-                        print(f"Removing TV show ({item_count} of {num_items}): {item['Title']} ({item['Year']}) from Trakt Watchlist")
+                        print(f" - Removing TV show ({item_count} of {num_items}): {item['Title']} ({item['Year']}) from Trakt Watchlist")
                     elif item["Type"] == "movie":
                         # This is a movie
                         data = {
                             "movies": [{
                                 "ids": {
                                     "trakt": item["TraktID"]
                                 }
                             }]
                         }
-                        print(f"Removing movie ({item_count} of {num_items}): {item['Title']} ({item['Year']}) from Trakt Watchlist")
+                        print(f" - Removing movie ({item_count} of {num_items}): {item['Title']} ({item['Year']}) from Trakt Watchlist")
                     elif item["Type"] == "episode":
                         # This is an episode
                         data = {
                             "episodes": [{
                                 "ids": {
                                     "trakt": item["TraktID"]
                                 }
                             }]
                         }
-                        print(f"Removing episode ({item_count} of {num_items}): {item['Title']} ({item['Year']}) from Trakt Watchlist")
+                        print(f" - Removing episode ({item_count} of {num_items}): {item['Title']} ({item['Year']}) from Trakt Watchlist")
 
                     # Make the API call to remove the item from the watchlist
                     response = EH.make_trakt_request(remove_url, payload=data)
 
                     if response is None:
-                        print(f"Error removing {item}: {response.content}")
+                        error_message = f"Failed removing {item['Type']} ({item_count} of {num_items}): {item['Title']} ({item['Year']}) from Trakt Watchlist"
+                        print(f"   - {error_message}")
+                        EL.logger.error(error_message)
 
                 print('Removing Watched Items From Trakt Watchlist Complete')
             else:
                 print('No Watched Items To Remove From Trakt Watchlist')
 
             # Remove Watched Items TMDB Watchlist
             if tmdb_watchlist_items_to_remove:
@@ -302,14 +319,15 @@
                 account_id = json_data['id']
                 
                 # Count the total number of items
                 num_items = len(tmdb_watchlist_items_to_remove)
                 item_count = 0
                 
                 for item in tmdb_watchlist_items_to_remove:
+                    print(f" - Removing item ({item_count} of {num_items}): {item['Title']} ({item['Year']}) from TMDB Watchlist")
                     item_count += 1
                     payload = {}  # Add any additional payload parameters if required
                     if item['Type'] == 'movie':
                         url = f"https://api.themoviedb.org/3/account/{account_id}/watchlist"
                         payload['media_type'] = "movie"
                         payload['media_id'] = item['TMDB_ID']
                         payload['watchlist'] = False  # Set watchlist to False to remove the item
@@ -318,23 +336,24 @@
                     elif item['Type'] == 'show':
                         url = f"https://api.themoviedb.org/3/account/{account_id}/watchlist"
                         payload['media_type'] = "tv"
                         payload['media_id'] = item['TMDB_ID']
                         payload['watchlist'] = False  # Set watchlist to False to remove the item
                         response = EH.make_tmdb_request(url, payload=payload)
                     
-                    if response:
-                        print(f"Removing item ({item_count} of {num_items}): {item['Title']} ({item['Year']}) from TMDB Watchlist")
-                    else:
-                        print(f"Failed to remove item ({item_count} of {num_items}): {item['Title']} ({item['Year']}) from TMDB Watchlist (TMDB ID: {item['TMDB_ID']})")
+                    if response is None:
+                        error_message = f"Failed to remove item ({item_count} of {num_items}): {item['Title']} ({item['Year']}) from TMDB Watchlist (TMDB ID: {item['TMDB_ID']})"
+                        print(f"   - {error_message}")
+                        EL.logger.error(error_message)
 
                 
                 print('Removing Watched Items From TMDB Watchlist Complete')
             else:
                 print('No Watched Items To Remove From TMDB Watchlist')
         
     except Exception as e:
         error_message = "An error occurred while running the script."
         EH.report_error(error_message)
+        EL.logger.error(error_message, exc_info=True)
 
 if __name__ == '__main__':
     main()
```

### Comparing `TMDBTraktSyncer-1.3.0/TMDBTraktSyncer/authTrakt.py` & `TMDBTraktSyncer-1.4.0/TMDBTraktSyncer/authTrakt.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 import requests
 import time
+try:
+    from TMDBTraktSyncer import errorLogger as EL
+except ImportError:
+    import errorLogger as EL
 
 def make_trakt_request(url, headers=None, params=None, payload=None, max_retries=3):
     retry_delay = 5  # seconds between retries
     retry_attempts = 0
 
     while retry_attempts < max_retries:
         response = None
```

### Comparing `TMDBTraktSyncer-1.3.0/TMDBTraktSyncer/errorHandling.py` & `TMDBTraktSyncer-1.4.0/TMDBTraktSyncer/errorHandling.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import traceback
 import requests
 import time
 try:
     from TMDBTraktSyncer import verifyCredentials as VC
+    from TMDBTraktSyncer import errorLogger as EL
 except ImportError:
     import verifyCredentials as VC
+    import errorLogger as EL
 
 def report_error(error_message):
     github_issue_url = "https://github.com/RileyXX/TMDB-Trakt-Syncer/issues/new?template=bug_report.yml"
     traceback_info = traceback.format_exc()
 
     print("\n--- ERROR ---")
     print(error_message)
@@ -47,23 +49,29 @@
             elif response.status_code in [429, 500, 502, 503, 504, 520, 521, 522]:
                 # Server overloaded or rate limit exceeded, retry after delay
                 retry_attempts += 1
                 time.sleep(retry_delay)
                 retry_delay *= 2  # Exponential backoff for retries
             else:
                 # Handle other status codes as needed
-                error_message = get_trakt_message(response.status_code)
-                print(f"Request failed with status code {response.status_code}: {error_message}")
+                status_message = get_trakt_message(response.status_code)
+                error_message = f"Request failed with status code {response.status_code}: {status_message}"
+                print(f"   - {error_message}")
+                EL.logger.error(f"{error_message}. URL: {url}")
                 return None
 
         except requests.exceptions.RequestException as e:
-            print(f"Request failed with exception: {e}")
+            error_message = f"Request failed with exception: {e}"
+            print(f"   - {error_message}")
+            EL.logger.error(error_message, exc_info=True)
             return None
 
-    print("Max retry attempts reached with Trakt API, request failed.")
+    error_message = "Max retry attempts reached with Trakt API, request failed."
+    print(f"   - {error_message}")
+    EL.logger.error(error_message)
     return None
 
 def get_trakt_message(status_code):
     error_messages = {
         200: "Success",
         201: "Success - new resource created (POST)",
         204: "Success - no content to return (DELETE)",
@@ -105,39 +113,53 @@
         try:
             if payload is None:
                 response = requests.get(url, headers=headers)
             else:
                 response = requests.post(url, headers=headers, json=payload)
 
             status_code = response.status_code
+            
             if status_code in [200, 201]:
                 return response  # Request succeeded, return response
             elif status_code in [504, 429, 502, 503]:
                 # Rate limit exceeded, retry after delay
                 retry_attempts += 1
                 time.sleep(retry_delay)
                 retry_delay *= 2  # Exponential backoff for retries
+                # Handle specific status codes as needed
+                status_message = get_tmdb_message(status_code)
+                error_message = f"Request failed with status code {status_code}: {status_message}. Retrying..."
+                print(f"   - {error_message}")
+                EL.logger.error(error_message)
             elif status_code in [501, 401, 405, 422, 404, 403, 409, 503, 500, 504, 429, 400, 406,
                                  422, 504, 429, 400, 400, 400, 401, 401, 401, 500, 401, 401, 401,
                                  404, 401, 401, 404, 401, 401, 404, 401, 200, 422, 405, 502, 500,
                                  403, 503, 400]:
                 # Handle specific status codes as needed
-                error_message = get_tmdb_message(status_code)
-                print(f"Request failed with status code {status_code}: {error_message}")
+                status_message = get_tmdb_message(status_code)
+                error_message = f"Request failed with status code {status_code}: {status_message}"
+                print(f"   - {error_message}")
+                EL.logger.error(error_message)
                 return None
             else:
                 # Request failed with an unknown status code
-                print(f"Request failed with unknown status code: {status_code}")
+                error_message = f"Request failed with unknown status code: {status_code}"
+                print(f"   - {error_message}")
+                EL.logger.error(error_message)
                 return None
 
         except requests.exceptions.RequestException as e:
-            print(f"Request failed with exception: {e}")
+            error_message = f"Request failed with exception: {e}"
+            print(f"   - {error_message}")
+            EL.logger.error(error_message, exc_info=True)
             return None
 
-    print("Max retry attempts reached with TMDB API, request failed.")
+    error_message = "Max retry attempts reached with TMDB API, request failed."
+    print(f"   - {error_message}")
+    EL.logger.error(error_message)
     return None
 
 def get_tmdb_message(status_code):
     error_messages = {
         200: "Success",
         501: "Invalid service: this service does not exist",
         401: "Authentication failed: You do not have permissions to access the service",
```

### Comparing `TMDBTraktSyncer-1.3.0/TMDBTraktSyncer/tmdbData.py` & `TMDBTraktSyncer-1.4.0/TMDBTraktSyncer/tmdbData.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import requests
 import json
 import time
 try:
     from TMDBTraktSyncer import errorHandling as EH
+    from TMDBTraktSyncer import errorLogger as EL
 except ImportError:
     import errorHandling as EH
+    import errorLogger as EL
 
 def fetch_data(url):
     response = EH.make_tmdb_request(url)
     json_data = json.loads(response.text)
     results = json_data['results']
     total_pages = json_data['total_pages']
     current_page = json_data['page']
```

### Comparing `TMDBTraktSyncer-1.3.0/TMDBTraktSyncer/traktData.py` & `TMDBTraktSyncer-1.4.0/TMDBTraktSyncer/traktData.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 import json
 import requests
 import urllib.parse
 import datetime
 try:
     from TMDBTraktSyncer import errorHandling as EH
+    from TMDBTraktSyncer import errorLogger as EL
 except ImportError:
     import errorHandling as EH
+    import errorLogger as EL
 
 def getTraktData():
     # Process Trakt Ratings and Comments
     print('Processing Trakt Data')
 
     response = EH.make_trakt_request('https://api.trakt.tv/users/me')
     json_data = json.loads(response.text)
```

### Comparing `TMDBTraktSyncer-1.3.0/TMDBTraktSyncer/verifyCredentials.py` & `TMDBTraktSyncer-1.4.0/TMDBTraktSyncer/verifyCredentials.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import os
 import json
 try:
     from TMDBTraktSyncer import authTrakt
+    from TMDBTraktSyncer import errorLogger as EL
 except ImportError:
     import authTrakt
+    import errorLogger as EL
 
 def prompt_get_credentials():
     # Define the file path
     here = os.path.abspath(os.path.dirname(__file__))
     file_path = os.path.join(here, 'credentials.txt')
 
     # Check if the file exists
@@ -61,14 +63,16 @@
     try:
         with open(file_path, 'r', encoding='utf-8') as file:
             credentials = json.load(file)
             sync_ratings_value = credentials.get('sync_ratings')
             if sync_ratings_value is not None:
                 return sync_ratings_value
     except FileNotFoundError:
+        error_message = "File not found error"
+        EL.logger.error(error_message, exc_info=True)
         pass
 
     while True:
         # Prompt the user for input
         print("Do you want to sync ratings? (y/n)")
         user_input = input("Enter your choice: ")
 
@@ -85,14 +89,16 @@
 
     # Update the value in the JSON file
     credentials = {}
     try:
         with open(file_path, 'r', encoding='utf-8') as file:
             credentials = json.load(file)
     except FileNotFoundError:
+        error_message = "File not found error"
+        EL.logger.error(error_message, exc_info=True)
         pass
 
     credentials['sync_ratings'] = sync_ratings_value
 
     with open(file_path, 'w', encoding='utf-8') as file:
         json.dump(credentials, file)
 
@@ -108,14 +114,16 @@
     try:
         with open(file_path, 'r', encoding='utf-8') as file:
             credentials = json.load(file)
             sync_watchlist_value = credentials.get('sync_watchlist')
             if sync_watchlist_value is not None:
                 return sync_watchlist_value
     except FileNotFoundError:
+        error_message = "File not found error"
+        EL.logger.error(error_message, exc_info=True)
         pass
 
     while True:
         # Prompt the user for input
         print("Do you want to sync watchlists? (y/n)")
         user_input = input("Enter your choice: ")
 
@@ -132,14 +140,16 @@
 
     # Update the value in the JSON file
     credentials = {}
     try:
         with open(file_path, 'r', encoding='utf-8') as file:
             credentials = json.load(file)
     except FileNotFoundError:
+        error_message = "File not found error"
+        EL.logger.error(error_message, exc_info=True)
         pass
 
     credentials['sync_watchlist'] = sync_watchlist_value
 
     with open(file_path, 'w', encoding='utf-8') as file:
         json.dump(credentials, file)
 
@@ -155,14 +165,16 @@
     try:
         with open(file_path, 'r', encoding='utf-8') as file:
             credentials = json.load(file)
             remove_watched_from_watchlists_value = credentials.get('remove_watched_from_watchlists')
             if remove_watched_from_watchlists_value is not None:
                 return remove_watched_from_watchlists_value
     except FileNotFoundError:
+        error_message = "File not found error"
+        EL.logger.error(error_message, exc_info=True)
         pass
 
     while True:
         # Prompt the user for input
         print("Movies and Episodes are removed from watchlists after 1 play.")
         print("Shows are removed when atleast 80% of the episodes are watched AND the series is marked as ended or cancelled.")
         print("Do you want to remove watched items from watchlists? (y/n)")
@@ -181,14 +193,16 @@
 
     # Update the value in the JSON file
     credentials = {}
     try:
         with open(file_path, 'r', encoding='utf-8') as file:
             credentials = json.load(file)
     except FileNotFoundError:
+        error_message = "File not found error"
+        EL.logger.error(error_message, exc_info=True)
         pass
 
     credentials['remove_watched_from_watchlists'] = remove_watched_from_watchlists_value
 
     with open(file_path, 'w', encoding='utf-8') as file:
         json.dump(credentials, file)
```

### Comparing `TMDBTraktSyncer-1.3.0/TMDBTraktSyncer.egg-info/PKG-INFO` & `TMDBTraktSyncer-1.4.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,134 +1,118 @@
-Metadata-Version: 2.1
-Name: TMDBTraktSyncer
-Version: 1.3.0
-Summary: A python script that syncs user watchlist and ratings for Movies, TV Shows and Episodes both ways between Trakt and TMDB.
-Home-page: https://github.com/RileyXX/TMDB-Trakt-Syncer
-Author: RileyXX
-Keywords: python,video,trakt,tmdb,ratings,sync,movies,tv shows
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: End Users/Desktop
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-
-# TMDB-Trakt-Syncer
-
-This Python script syncs user watchlist and ratings for Movies, TV Shows, and Episodes both ways between [Trakt](https://trakt.tv/) and [TMDB](https://www.themoviedb.org/). Data already set will not be overwritten. Ratings and watchlist sync are both optional. The user will be prompted to enter their settings and api keys on first run.
-
-The script is compatible on any operating system that supports Python v3.6 or later, including Windows, Linux, Mac, and ChromeOS. If you're interested in syncing ratings between Trakt, Plex, IMDB, and TMDB, I recommend the following projects: [PlexTraktSync](https://github.com/Taxel/PlexTraktSync), [IMDB-Trakt-Syncer](https://github.com/RileyXX/IMDB-Trakt-Syncer), and [TMDB-Trakt-Syncer](https://github.com/RileyXX/TMDB-Trakt-Syncer). See below for my other [recommended projects](https://github.com/RileyXX/TMDB-Trakt-Syncer#other-recommended-projects).
-
-## Installation Instructions:
-1. Install [Python](https://www.python.org/downloads/) (v3.6 or later).
-2. Install the script by running `python -m pip install TMDBTraktSyncer` in command line.
-3. Login to [Trakt](https://trakt.tv/oauth/applications) and create a new API application named `TMDbTraktSyncer`. In the "Redirect uri" field, enter `urn:ietf:wg:oauth:2.0:oob`, then save the application.
-4. Login to [TMDB](https://www.themoviedb.org/settings/api/) and create a new API application. Choose "Developer" and accept the terms. Fill out the application form as follows: 
-   - Type of use: `Personal`
-   - Application name: `TMDB-Trakt-Sync`
-   - Application URL: `https://github.com/RileyXX/TMDB-Trakt-Syncer`
-   - Application summary: `Use TMDB API and Trakt API to sync user ratings between platforms.`
-   - Fill in the rest of the fields as desired and submit the form. Your API keys will be generated instantly.
-5. Run the script by running `TMDBTraktSyncer` in the command line.
-6. Follow the prompts during the first run. You will need to enter your Trakt `client ID` and `client secret` from step 3, as well as your `tmdb_v4_token` from step 4. Please note that these details are saved insecurely as `credentials.txt` in the same folder as the script.
-7. Setup is complete. The script will continue running and syncing your ratings. You can monitor its progress in the command line.
-
-## Installing the Script:
-```
-python -m pip install TMDBTraktSyncer
-```
-_Run in your operating system's native command line._
-## Running the Script:
-```
-TMDBTraktSyncer
-```
-_Run in your operating system's native command line._
-## Updating the Script:
-```
-python -m pip install TMDBTraktSyncer --upgrade
-```
-_Run in your operating system's native command line._
-## Uninstalling the Script:
-```
-python -m pip uninstall TMDBTraktSyncer
-```
-_Run in your operating system's native command line._
-
-## Installing a Specific Version:
-```
-python -m pip install TMDBTraktSyncer==VERSION_NUMBER
-```
-_Replace `VERSION_NUMBER` with your [desired version](https://github.com/RileyXX/TMDB-Trakt-Syncer/releases) (e.g. 1.0.1) and run in your operating system's native command line._
-
-## Alternative Manual Installation Method (without pip install):
-1. Install [Python](https://www.python.org/downloads/) (v3.6 or later).
-2. Download the latest .zip from the [releases page](https://github.com/RileyXX/TMDB-Trakt-Syncer/releases) and extract it to the desired directory.
-3. Login to [Trakt](https://trakt.tv/oauth/applications) and create a new API application named `TMDBTraktSyncer`. In the "Redirect uri" field, enter `urn:ietf:wg:oauth:2.0:oob`, then save the application.
-4. Login to [TMDB](https://www.themoviedb.org/settings/api/) and create a new API application. Choose "Developer" and accept the terms. Fill out the application form as follows: 
-   - Type of use: `Personal`
-   - Application name: `TMDB-Trakt-Sync`
-   - Application URL: `https://github.com/RileyXX/TMDB-Trakt-Syncer`
-   - Application summary: `Use TMDB API and Trakt API to sync user ratings between platforms.`
-   - Fill in the rest of the fields as desired and submit the form. Your API keys will be generated instantly.
-5. Run `TMDBTraktSyncer.py` or open the terminal and navigate to the folder where `TMDBTraktSyncer.py` is located, then run `TMDBTraktSyncer.py` in the terminal.
-6. Follow the prompts during the first run. You will need to enter your Trakt `client ID` and `client secret` from step 3, as well as your `tmdb_v4_token` from step 4. Please note that these details are saved insecurely as `credentials.txt` in the same folder as the script.
-7. Setup is complete. The script will continue running and syncing your ratings. You can monitor its progress in the command line.
-
-## For Setting Up Automation See the Following Wiki Pages:
-- Setup Automation for:
-   - [Windows](https://github.com/RileyXX/TMDB-Trakt-Syncer/wiki/Setting-Up-Automation-on-Windows)
-   - [Linux](https://github.com/RileyXX/TMDB-Trakt-Syncer/wiki/Setting-Up-Automation-on-Linux)
-   - [macOS](https://github.com/RileyXX/TMDB-Trakt-Syncer/wiki/Setting-Up-Automation-on-macOS)
-- Python Script to Update all Packages with Pip (Windows, Linux, Mac, ChromeOS, etc.) [Link #1](https://github.com/RileyXX/TMDB-Trakt-Syncer/wiki/Python-Script-to-Update-all-Packages-with-Pip-\(Windows,-Linux,-Mac,-ChromeOS,-etc\))
-
-## Troubleshooting, Known Issues, Workarounds & Future Outlook:
-* Add optional setting to remove watched items from watchlists [Issue #15](https://github.com/RileyXX/TMDB-Trakt-Syncer/issues/15)
-* Add support for review/comment sync [Issue #1](https://github.com/RileyXX/TMDB-Trakt-Syncer/issues/1)
-* If any of your details change (passwords, logins, API keys, etc.), simply open `credentials.txt`, modify your details, save it and then run the script again. Alternatively, delete `credentials.txt` to reset the script and it will prompt you to enter your new details on the next run.
-
-## Screenshot:
-![Demo](https://i.imgur.com/5LI04O2.png)
-
-## Sponsorships, Donations, and Custom Projects:
-If you find my scripts helpful, you can become a [sponsor](https://github.com/sponsors/RileyXX) and support my projects! If you need help with a project, open an issue, and I'll do my best to assist you. For other inquiries and custom projects, you can contact me on [Twitter](https://twitter.com/RileyxBell).
-
-#### More Donation Options:
-- Cashapp: `$rileyxx`
-- Venmo: `@rileyxx`
-- Bitcoin: `bc1qrjevwqv49z8y77len3azqfghxrjmrjvhy5zqau`
-- Amazon Wishlist: [Link ↗](https://www.amazon.com/hz/wishlist/ls/WURF5NWZ843U)
-
-## Also Posted on:
-* [PyPi](https://pypi.org/project/TMDBTraktSyncer/)
-* [Reddit](https://www.reddit.com/r/trakt/comments/13jlu4r/tmdb_trakt_rating_syncer_tool_2_way_sync/)
-
-<br>
-
-[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
-
-## Other Recommended Projects:
-
-| Project Name | Description |
-|--------------|-------------|
-| [PlexTraktSync](https://github.com/Taxel/PlexTraktSync) | A script that syncs user watch history and ratings between Trakt and Plex (without needing a PlexPass or Trakt VIP subscription). |
-| [IMDB-Trakt-Syncer](https://github.com/RileyXX/IMDB-Trakt-Syncer) | A script that syncs user watchlist, ratings, and comments both ways between Trakt and IMDB. |
-| [TMDB-Trakt-Syncer](https://github.com/RileyXX/TMDB-Trakt-Syncer) | A script that syncs user watchlist and ratings both ways between Trakt and TMDB. |
-| [PlexPreferNonForcedSubs](https://github.com/RileyXX/PlexPreferNonForcedSubs) | A script that sets all movies and shows in your local Plex library to English non-forced subtitles by default. |
-| [Casvt / PlexAutoDelete](https://github.com/Casvt/Plex-scripts/blob/main/changing_settings/plex_auto_delete.py) | A script for automatically deleting watched content from Plex. |
-| [Netflix-to-Trakt-Import](https://github.com/jensb89/Netflix-to-Trakt-Import) | A tool to import your Netflix viewing history into Trakt. |
-| [trakt-tv-backup](https://darekkay.com/blog/trakt-tv-backup/) | A command-line tool for backing up your Trakt.tv data. |
-| [blacktwin / JBOPS](https://github.com/blacktwin/JBOPS) | A collection of scripts and tools for enhancing and automating tasks in Plex. |
-| [Casvt / Plex-scripts](https://github.com/Casvt/Plex-scripts) | A collection of useful scripts for Plex automation and management. |
-| [trakt---letterboxd-import](https://github.com/jensb89/trakt---letterboxd-import) | A tool to import your Letterboxd ratings and watchlist into Trakt. |
-| [TraktRater](https://github.com/damienhaynes/TraktRater/) | A tool to help users transfer user episode, show, and movie user ratings and watchlists from multiple media database sites around the web. |
-| [TvTimeToTrakt](https://github.com/lukearran/TvTimeToTrakt) | A tool to sync your TV Time watch history with Trakt.tv. |
-| [Plex Media Server](https://www.plex.tv/media-server-downloads/#plex-app) | A media server software to organize and stream your personal media collection. |
-| [Radarr](https://github.com/Radarr/Radarr) | A movie collection manager and downloader for various platforms. |
-| [Sonarr](https://github.com/Sonarr/Sonarr) | A TV show collection manager and downloader for various platforms. |
-| [Jackett](https://github.com/Jackett/Jackett) | A proxy server that provides API support for various torrent trackers commonly used with Radarr and Sonarr. |
-| [qBittorrent](https://github.com/qbittorrent/qBittorrent) | A free and open-source BitTorrent client. |
-| [Mullvad VPN](https://github.com/mullvad/mullvadvpn-app) | An open-source VPN client for Mullvad VPN service with port forwarding support. Great VPN for torrents. |
-| [Overseerr](https://github.com/sct/overseerr) | A request management and media discovery tool for your home media server. |
-| [FlareSolverr](https://github.com/FlareSolverr/FlareSolverr) | A reverse proxy solution to bypass Cloudflare protection and access websites commonly used with Jackett. |
-| [youtube-dl](https://github.com/ytdl-org/youtube-dl) | A command-line program to download videos from YouTube and other sites. |
+# TMDB-Trakt-Syncer
+
+This Python script syncs user watchlist and ratings for Movies, TV Shows, and Episodes both ways between [Trakt](https://trakt.tv/) and [TMDB](https://www.themoviedb.org/). Data already set will not be overwritten. Ratings and watchlist sync are both optional. The user will be prompted to enter their settings and api keys on first run.
+
+The script is compatible on any operating system that supports Python v3.6 or later, including Windows, Linux, Mac, and ChromeOS. If you're interested in syncing ratings between Trakt, Plex, IMDB, and TMDB, I recommend the following projects: [PlexTraktSync](https://github.com/Taxel/PlexTraktSync), [IMDB-Trakt-Syncer](https://github.com/RileyXX/IMDB-Trakt-Syncer), and [TMDB-Trakt-Syncer](https://github.com/RileyXX/TMDB-Trakt-Syncer). See below for my other [recommended projects](https://github.com/RileyXX/TMDB-Trakt-Syncer#other-recommended-projects).
+
+## Installation Instructions:
+1. Install [Python](https://www.python.org/downloads/) (v3.6 or later).
+2. Install the script by running `python -m pip install TMDBTraktSyncer` in command line.
+3. Login to [Trakt](https://trakt.tv/oauth/applications) and create a new API application named `TMDbTraktSyncer`. In the "Redirect uri" field, enter `urn:ietf:wg:oauth:2.0:oob`, then save the application.
+4. Login to [TMDB](https://www.themoviedb.org/settings/api/) and create a new API application. Choose "Developer" and accept the terms. Fill out the application form as follows: 
+   - Type of use: `Personal`
+   - Application name: `TMDB-Trakt-Sync`
+   - Application URL: `https://github.com/RileyXX/TMDB-Trakt-Syncer`
+   - Application summary: `Use TMDB API and Trakt API to sync user ratings between platforms.`
+   - Fill in the rest of the fields as desired and submit the form. Your API keys will be generated instantly.
+5. Run the script by running `TMDBTraktSyncer` in the command line.
+6. Follow the prompts during the first run. You will need to enter your Trakt `client ID` and `client secret` from step 3, as well as your `tmdb_v4_token` from step 4. Please note that these details are saved insecurely as `credentials.txt` in the same folder as the script.
+7. Setup is complete. The script will continue running and syncing your ratings. You can monitor its progress in the command line.
+
+## Installing the Script:
+```
+python -m pip install TMDBTraktSyncer
+```
+_Run in your operating system's native command line._
+## Running the Script:
+```
+TMDBTraktSyncer
+```
+_Run in your operating system's native command line._
+## Updating the Script:
+```
+python -m pip install TMDBTraktSyncer --upgrade
+```
+_Run in your operating system's native command line._
+## Uninstalling the Script:
+```
+python -m pip uninstall TMDBTraktSyncer
+```
+_Run in your operating system's native command line._
+
+## Installing a Specific Version:
+```
+python -m pip install TMDBTraktSyncer==VERSION_NUMBER
+```
+_Replace `VERSION_NUMBER` with your [desired version](https://github.com/RileyXX/TMDB-Trakt-Syncer/releases) (e.g. 1.0.1) and run in your operating system's native command line._
+
+## Alternative Manual Installation Method (without pip install):
+1. Install [Python](https://www.python.org/downloads/) (v3.6 or later).
+2. Download the latest .zip from the [releases page](https://github.com/RileyXX/TMDB-Trakt-Syncer/releases) and extract it to the desired directory.
+3. Login to [Trakt](https://trakt.tv/oauth/applications) and create a new API application named `TMDBTraktSyncer`. In the "Redirect uri" field, enter `urn:ietf:wg:oauth:2.0:oob`, then save the application.
+4. Login to [TMDB](https://www.themoviedb.org/settings/api/) and create a new API application. Choose "Developer" and accept the terms. Fill out the application form as follows: 
+   - Type of use: `Personal`
+   - Application name: `TMDB-Trakt-Sync`
+   - Application URL: `https://github.com/RileyXX/TMDB-Trakt-Syncer`
+   - Application summary: `Use TMDB API and Trakt API to sync user ratings between platforms.`
+   - Fill in the rest of the fields as desired and submit the form. Your API keys will be generated instantly.
+5. Run `TMDBTraktSyncer.py` or open the terminal and navigate to the folder where `TMDBTraktSyncer.py` is located, then run `TMDBTraktSyncer.py` in the terminal.
+6. Follow the prompts during the first run. You will need to enter your Trakt `client ID` and `client secret` from step 3, as well as your `tmdb_v4_token` from step 4. Please note that these details are saved insecurely as `credentials.txt` in the same folder as the script.
+7. Setup is complete. The script will continue running and syncing your ratings. You can monitor its progress in the command line.
+
+## For Setting Up Automation See the Following Wiki Pages:
+- Setup Automation for:
+   - [Windows](https://github.com/RileyXX/TMDB-Trakt-Syncer/wiki/Setting-Up-Automation-on-Windows)
+   - [Linux](https://github.com/RileyXX/TMDB-Trakt-Syncer/wiki/Setting-Up-Automation-on-Linux)
+   - [macOS](https://github.com/RileyXX/TMDB-Trakt-Syncer/wiki/Setting-Up-Automation-on-macOS)
+- Python Script to Update all Packages with Pip (Windows, Linux, Mac, ChromeOS, etc.) [Link #1](https://github.com/RileyXX/TMDB-Trakt-Syncer/wiki/Python-Script-to-Update-all-Packages-with-Pip-\(Windows,-Linux,-Mac,-ChromeOS,-etc\))
+
+## Troubleshooting, Known Issues, Workarounds & Future Outlook:
+* Add support for review/comment sync [Issue #1](https://github.com/RileyXX/TMDB-Trakt-Syncer/issues/1)
+* If any of your details change (passwords, logins, API keys, etc.), simply open `credentials.txt`, modify your details, save it and then run the script again. Alternatively, delete `credentials.txt` to reset the script and it will prompt you to enter your new details on the next run.
+
+## Screenshot:
+![Demo](https://i.imgur.com/5LI04O2.png)
+
+## Sponsorships, Donations, and Custom Projects:
+If you find my scripts helpful, you can become a [sponsor](https://github.com/sponsors/RileyXX) and support my projects! If you need help with a project, open an issue, and I'll do my best to assist you. For other inquiries and custom projects, you can contact me on [Twitter](https://twitter.com/RileyxBell).
+
+#### More Donation Options:
+- Cashapp: `$rileyxx`
+- Venmo: `@rileyxx`
+- Bitcoin: `bc1qrjevwqv49z8y77len3azqfghxrjmrjvhy5zqau`
+- Amazon Wishlist: [Link ↗](https://www.amazon.com/hz/wishlist/ls/WURF5NWZ843U)
+
+## Also Posted on:
+* [PyPi](https://pypi.org/project/TMDBTraktSyncer/)
+* [Reddit](https://www.reddit.com/r/trakt/comments/13jlu4r/tmdb_trakt_rating_syncer_tool_2_way_sync/)
+
+<br>
+
+[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
+
+## Other Recommended Projects:
+
+| Project Name | Description |
+|--------------|-------------|
+| [PlexTraktSync](https://github.com/Taxel/PlexTraktSync) | A script that syncs user watch history and ratings between Trakt and Plex (without needing a PlexPass or Trakt VIP subscription). |
+| [IMDB-Trakt-Syncer](https://github.com/RileyXX/IMDB-Trakt-Syncer) | A script that syncs user watchlist, ratings, and comments both ways between Trakt and IMDB. |
+| [TMDB-Trakt-Syncer](https://github.com/RileyXX/TMDB-Trakt-Syncer) | A script that syncs user watchlist and ratings both ways between Trakt and TMDB. |
+| [PlexPreferNonForcedSubs](https://github.com/RileyXX/PlexPreferNonForcedSubs) | A script that sets all movies and shows in your local Plex library to English non-forced subtitles by default. |
+| [Casvt / PlexAutoDelete](https://github.com/Casvt/Plex-scripts/blob/main/changing_settings/plex_auto_delete.py) | A script for automatically deleting watched content from Plex. |
+| [universal-trakt-scrobbler](https://github.com/trakt-tools/universal-trakt-scrobbler) | An extension that automatically scrobbles TV shows and Movies from several streaming services to Trakt. |
+| [Netflix-to-Trakt-Import](https://github.com/jensb89/Netflix-to-Trakt-Import) | A tool to import your Netflix viewing history into Trakt. |
+| [trakt-tv-backup](https://darekkay.com/blog/trakt-tv-backup/) | A command-line tool for backing up your Trakt.tv data. |
+| [blacktwin / JBOPS](https://github.com/blacktwin/JBOPS) | A collection of scripts and tools for enhancing and automating tasks in Plex. |
+| [Casvt / Plex-scripts](https://github.com/Casvt/Plex-scripts) | A collection of useful scripts for Plex automation and management. |
+| [trakt---letterboxd-import](https://github.com/jensb89/trakt---letterboxd-import) | A tool to import your Letterboxd ratings and watchlist into Trakt. |
+| [TraktRater](https://github.com/damienhaynes/TraktRater/) | A tool to help users transfer user episode, show, and movie user ratings and watchlists from multiple media database sites around the web. |
+| [TvTimeToTrakt](https://github.com/lukearran/TvTimeToTrakt) | A tool to sync your TV Time watch history with Trakt.tv. |
+| [Plex Media Server](https://www.plex.tv/media-server-downloads/#plex-app) | A media server software to organize and stream your personal media collection. |
+| [Radarr](https://github.com/Radarr/Radarr) | A movie collection manager and downloader for various platforms. |
+| [Sonarr](https://github.com/Sonarr/Sonarr) | A TV show collection manager and downloader for various platforms. |
+| [Jackett](https://github.com/Jackett/Jackett) | A proxy server that provides API support for various torrent trackers commonly used with Radarr and Sonarr. |
+| [qBittorrent](https://github.com/qbittorrent/qBittorrent) | A free and open-source BitTorrent client. |
+| [Mullvad VPN](https://github.com/mullvad/mullvadvpn-app) | An open-source VPN client for Mullvad VPN service with port forwarding support. Great VPN for torrents. |
+| [Overseerr](https://github.com/sct/overseerr) | A request management and media discovery tool for your home media server. |
+| [FlareSolverr](https://github.com/FlareSolverr/FlareSolverr) | A reverse proxy solution to bypass Cloudflare protection and access websites commonly used with Jackett. |
+| [youtube-dl](https://github.com/ytdl-org/youtube-dl) | A command-line program to download videos from YouTube and other sites. |
```

### Comparing `TMDBTraktSyncer-1.3.0/setup.py` & `TMDBTraktSyncer-1.4.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #To upload package: twine upload dist/*
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), 'r', encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '1.3.0'
+VERSION = '1.4.0'
 DESCRIPTION = 'A python script that syncs user watchlist and ratings for Movies, TV Shows and Episodes both ways between Trakt and TMDB.'
 
 # Setting up
 setup(
     name="TMDBTraktSyncer",
     version=VERSION,
     author="RileyXX",
```

