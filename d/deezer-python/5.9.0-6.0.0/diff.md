# Comparing `tmp/deezer_python-5.9.0.tar.gz` & `tmp/deezer_python-6.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deezer_python-5.9.0.tar", max compression
+gzip compressed data, was "deezer_python-6.0.0.tar", max compression
```

## Comparing `deezer_python-5.9.0.tar` & `deezer_python-6.0.0.tar`

### file list

```diff
@@ -1,22 +1,23 @@
--rw-r--r--   0        0        0     1054 2023-04-13 09:24:49.202700 deezer_python-5.9.0/LICENSE.txt
--rw-r--r--   0        0        0    13246 2023-04-13 09:24:49.202700 deezer_python-5.9.0/README.md
--rw-r--r--   0        0        0     2244 2023-04-13 09:24:50.086698 deezer_python-5.9.0/pyproject.toml
--rw-r--r--   0        0        0      556 2023-04-13 09:24:50.046698 deezer_python-5.9.0/src/deezer/__init__.py
--rw-r--r--   0        0        0    23250 2023-04-13 09:24:49.210701 deezer_python-5.9.0/src/deezer/client.py
--rw-r--r--   0        0        0      530 2023-04-13 09:24:49.210701 deezer_python-5.9.0/src/deezer/dates.py
--rw-r--r--   0        0        0     1864 2023-04-13 09:24:49.210701 deezer_python-5.9.0/src/deezer/exceptions.py
--rw-r--r--   0        0        0     3745 2023-04-13 09:24:49.210701 deezer_python-5.9.0/src/deezer/pagination.py
--rw-r--r--   0        0        0      549 2023-04-13 09:24:49.210701 deezer_python-5.9.0/src/deezer/resources/__init__.py
--rw-r--r--   0        0        0     1734 2023-04-13 09:24:49.210701 deezer_python-5.9.0/src/deezer/resources/album.py
--rw-r--r--   0        0        0     2150 2023-04-13 09:24:49.210701 deezer_python-5.9.0/src/deezer/resources/artist.py
--rw-r--r--   0        0        0     2047 2023-04-13 09:24:49.210701 deezer_python-5.9.0/src/deezer/resources/chart.py
--rw-r--r--   0        0        0     1413 2023-04-13 09:24:49.210701 deezer_python-5.9.0/src/deezer/resources/editorial.py
--rw-r--r--   0        0        0     1043 2023-04-13 09:24:49.210701 deezer_python-5.9.0/src/deezer/resources/episode.py
--rw-r--r--   0        0        0     1355 2023-04-13 09:24:49.210701 deezer_python-5.9.0/src/deezer/resources/genre.py
--rw-r--r--   0        0        0     1400 2023-04-13 09:24:49.210701 deezer_python-5.9.0/src/deezer/resources/playlist.py
--rw-r--r--   0        0        0      914 2023-04-13 09:24:49.210701 deezer_python-5.9.0/src/deezer/resources/podcast.py
--rw-r--r--   0        0        0      805 2023-04-13 09:24:49.210701 deezer_python-5.9.0/src/deezer/resources/radio.py
--rw-r--r--   0        0        0     4006 2023-04-13 09:24:49.210701 deezer_python-5.9.0/src/deezer/resources/resource.py
--rw-r--r--   0        0        0     1546 2023-04-13 09:24:49.210701 deezer_python-5.9.0/src/deezer/resources/track.py
--rw-r--r--   0        0        0     2984 2023-04-13 09:24:49.210701 deezer_python-5.9.0/src/deezer/resources/user.py
--rw-r--r--   0        0        0    14647 1970-01-01 00:00:00.000000 deezer_python-5.9.0/PKG-INFO
+-rw-r--r--   0        0        0     1054 2023-06-27 12:38:33.897315 deezer_python-6.0.0/LICENSE.txt
+-rw-r--r--   0        0        0    13246 2023-06-27 12:38:33.897315 deezer_python-6.0.0/README.md
+-rw-r--r--   0        0        0     2248 2023-06-27 12:38:34.849318 deezer_python-6.0.0/pyproject.toml
+-rw-r--r--   0        0        0      556 2023-06-27 12:38:34.817318 deezer_python-6.0.0/src/deezer/__init__.py
+-rw-r--r--   0        0        0    24840 2023-06-27 12:38:33.897315 deezer_python-6.0.0/src/deezer/client.py
+-rw-r--r--   0        0        0      530 2023-06-27 12:38:33.897315 deezer_python-6.0.0/src/deezer/dates.py
+-rw-r--r--   0        0        0     1864 2023-06-27 12:38:33.897315 deezer_python-6.0.0/src/deezer/exceptions.py
+-rw-r--r--   0        0        0     3745 2023-06-27 12:38:33.897315 deezer_python-6.0.0/src/deezer/pagination.py
+-rw-r--r--   0        0        0      549 2023-06-27 12:38:33.897315 deezer_python-6.0.0/src/deezer/resources/__init__.py
+-rw-r--r--   0        0        0     1734 2023-06-27 12:38:33.897315 deezer_python-6.0.0/src/deezer/resources/album.py
+-rw-r--r--   0        0        0     2150 2023-06-27 12:38:33.897315 deezer_python-6.0.0/src/deezer/resources/artist.py
+-rw-r--r--   0        0        0     2047 2023-06-27 12:38:33.897315 deezer_python-6.0.0/src/deezer/resources/chart.py
+-rw-r--r--   0        0        0     1413 2023-06-27 12:38:33.897315 deezer_python-6.0.0/src/deezer/resources/editorial.py
+-rw-r--r--   0        0        0     1761 2023-06-27 12:38:33.897315 deezer_python-6.0.0/src/deezer/resources/episode.py
+-rw-r--r--   0        0        0     1355 2023-06-27 12:38:33.897315 deezer_python-6.0.0/src/deezer/resources/genre.py
+-rw-r--r--   0        0        0     3325 2023-06-27 12:38:33.897315 deezer_python-6.0.0/src/deezer/resources/playlist.py
+-rw-r--r--   0        0        0      914 2023-06-27 12:38:33.897315 deezer_python-6.0.0/src/deezer/resources/podcast.py
+-rw-r--r--   0        0        0      805 2023-06-27 12:38:33.897315 deezer_python-6.0.0/src/deezer/resources/radio.py
+-rw-r--r--   0        0        0     4826 2023-06-27 12:38:33.897315 deezer_python-6.0.0/src/deezer/resources/resource.py
+-rw-r--r--   0        0        0     1546 2023-06-27 12:38:33.897315 deezer_python-6.0.0/src/deezer/resources/track.py
+-rw-r--r--   0        0        0     6752 2023-06-27 12:38:33.897315 deezer_python-6.0.0/src/deezer/resources/user.py
+-rw-r--r--   0        0        0      583 2023-06-27 12:38:33.897315 deezer_python-6.0.0/src/deezer/utils.py
+-rw-r--r--   0        0        0    14597 1970-01-01 00:00:00.000000 deezer_python-6.0.0/PKG-INFO
```

### Comparing `deezer_python-5.9.0/LICENSE.txt` & `deezer_python-6.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `deezer_python-5.9.0/README.md` & `deezer_python-6.0.0/README.md`

 * *Files identical despite different names*

### Comparing `deezer_python-5.9.0/pyproject.toml` & `deezer_python-6.0.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "deezer-python"
-version = "5.9.0"
+version = "6.0.0"
 description = "A friendly wrapper library for the Deezer API"
 authors = ["Bruno Alla <alla.brunoo@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 keywords = ["deezer", "sdk", "client", "requests"]
 repository = "https://github.com/browniebroke/deezer-python"
 documentation = "https://deezer-python.readthedocs.io"
@@ -22,15 +22,15 @@
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/browniebroke/deezer-python/issues"
 "Changelog" = "https://deezer-python.readthedocs.io/en/latest/changelog.html"
 "Twitter" = "https://twitter.com/_BrunoAlla"
 "Mastodon" = "https://fosstodon.org/@browniebroke"
 
 [tool.poetry.dependencies]
-python = "^3.7"
+python = "^3.8"
 requests = ">=2.18"
 
 [tool.poetry.group.docs]
 optional = true
 
 [tool.poetry.group.docs.dependencies]
 myst-parser = ">=0.16"
@@ -41,16 +41,16 @@
 [tool.poetry.group.dev.dependencies]
 coverage = "^7.0"
 environs = "^9.3"
 pytest = "^7.0"
 pytest-cov = "^4.0"
 pytest-mock = "^3.6"
 pytest-vcr = "^1.0"
-vcrpy = "^4.1"
-deezer-oauth-cli = "^0.4"
+vcrpy = "^5.0.0"
+deezer-oauth-cli = "^1.0.0"
 
 [tool.semantic_release]
 version_toml = "pyproject.toml:tool.poetry.version"
 version_variable = "src/deezer/__init__.py:__version__"
 branch = "main"
 build_command = "pip install poetry && poetry build"
```

### Comparing `deezer_python-5.9.0/src/deezer/__init__.py` & `deezer_python-6.0.0/src/deezer/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     Podcast,
     Radio,
     Resource,
     Track,
     User,
 )
 
-__version__ = "5.9.0"
+__version__ = "6.0.0"
 __all__ = [
     "Album",
     "Artist",
     "Chart",
     "Client",
     "Editorial",
     "Episode",
```

### Comparing `deezer_python-5.9.0/src/deezer/client.py` & `deezer_python-6.0.0/src/deezer/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -114,22 +114,23 @@
             result[key] = value
         if parent is not None:
             result[parent.type] = parent
 
         if "id" not in result and resource_id is not None:
             result["id"] = resource_id
 
-        if "type" in result:
-            if result["type"] in self.objects_types:
-                object_class = self.objects_types[result["type"]]
-            else:
-                # in case any new types are introduced by the API
-                object_class = Resource
+        if "type" in result and result["type"] in self.objects_types:
+            object_class = self.objects_types[result["type"]]
+        elif "type" in result or not resource_type and "id" in result:
+            # in case any new types are introduced by the API
+            object_class = Resource
         elif resource_type:
             object_class = resource_type
+        elif item.get("results") is True:
+            return True
         else:
             raise DeezerUnknownResource(f"Unable to find resource type for {result!r}")
         assert object_class is not None  # nosec B101
         return object_class(self, result)
 
     def request(
         self,
@@ -162,15 +163,15 @@
         try:
             response.raise_for_status()
         except requests.HTTPError as exc:
             raise DeezerHTTPError.from_http_error(exc) from exc
         json_data = response.json()
         if not isinstance(json_data, dict):
             return json_data
-        if "error" in json_data:
+        if "error" in json_data and json_data["error"]:
             raise DeezerErrorResponse(json_data)
         return self._process_json(
             json_data,
             parent=parent,
             resource_type=resource_type,
             resource_id=resource_id,
             paginate_list=paginate_list,
@@ -537,14 +538,53 @@
         Remove a track from the user's library
 
         :param track_id: the ID of the track to remove.
         :return: boolean whether the operation succeeded.
         """
         return self.request("DELETE", "user/me/tracks", track_id=track_id)
 
+    def remove_user_playlist(self, playlist_id: int) -> bool:
+        """
+        Remove a playlist from the user's library
+
+        :param playlist_id: the ID of the playlist to remove.
+        :return: boolean whether the operation succeeded.
+        """
+        return self.request("DELETE", "user/me/playlists", playlist_id=playlist_id)
+
+    def add_user_playlist(self, playlist_id: int) -> bool:
+        """
+        Add a playlist to the user's library
+
+        :param playlist_id: the ID of the playlist to add.
+        :return: boolean whether the operation succeeded.
+        """
+        return self.request("POST", "user/me/playlists", playlist_id=playlist_id)
+
+    def create_playlist(self, playlist_name) -> int:
+        """
+        Create a playlist on the user's account
+
+        :param playlist_name: the name of the playlist.
+        :return: the ID of the playlist that was created
+        """
+        result = self.request("POST", "user/me/playlists", title=playlist_name)
+        # Note: the REST API call returns a dict with just the "id" key in it,
+        # so we return that instead of the full Playlist object
+        return result.id
+
+    def delete_playlist(self, playlist_id) -> bool:
+        """
+        Delete a playlist from the user's account
+
+        :param playlist_id: the ID of the playlist to remove.
+        :return: boolean whether the operation succeeded.
+        """
+        return self.request("DELETE", f"playlist/{playlist_id}")
+
     def _search(
         self,
         path: str,
         query: str = "",
         strict: bool | None = None,
         ordering: str | None = None,
         **advanced_params: str | int | None,
```

### Comparing `deezer_python-5.9.0/src/deezer/dates.py` & `deezer_python-6.0.0/src/deezer/dates.py`

 * *Files identical despite different names*

### Comparing `deezer_python-5.9.0/src/deezer/exceptions.py` & `deezer_python-6.0.0/src/deezer/exceptions.py`

 * *Files identical despite different names*

### Comparing `deezer_python-5.9.0/src/deezer/pagination.py` & `deezer_python-6.0.0/src/deezer/pagination.py`

 * *Files identical despite different names*

### Comparing `deezer_python-5.9.0/src/deezer/resources/__init__.py` & `deezer_python-6.0.0/src/deezer/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `deezer_python-5.9.0/src/deezer/resources/album.py` & `deezer_python-6.0.0/src/deezer/resources/album.py`

 * *Files identical despite different names*

### Comparing `deezer_python-5.9.0/src/deezer/resources/artist.py` & `deezer_python-6.0.0/src/deezer/resources/artist.py`

 * *Files identical despite different names*

### Comparing `deezer_python-5.9.0/src/deezer/resources/chart.py` & `deezer_python-6.0.0/src/deezer/resources/chart.py`

 * *Files identical despite different names*

### Comparing `deezer_python-5.9.0/src/deezer/resources/editorial.py` & `deezer_python-6.0.0/src/deezer/resources/editorial.py`

 * *Files identical despite different names*

### Comparing `deezer_python-5.9.0/src/deezer/resources/genre.py` & `deezer_python-6.0.0/src/deezer/resources/genre.py`

 * *Files identical despite different names*

### Comparing `deezer_python-5.9.0/src/deezer/resources/playlist.py` & `deezer_python-6.0.0/src/deezer/resources/podcast.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,57 +2,39 @@
 
 from typing import TYPE_CHECKING
 
 from .resource import Resource
 
 if TYPE_CHECKING:
     from ..pagination import PaginatedList
-    from .track import Track
-    from .user import User
+    from .episode import Episode
 
 
-class Playlist(Resource):
+class Podcast(Resource):
     """
-    To work with Deezer playlist objects.
+    To work with Deezer podcast objects.
 
-    Check the :deezer-api:`Deezer documentation <playlist>`
+    Check the :deezer-api:`Deezer documentation <podcast>`
     for more details about each field.
     """
 
     id: int
     title: str
     description: str
-    duration: int
-    public: bool
-    is_loved_track: bool
-    collaborative: bool
-    nb_tracks: int
-    unseen_track_count: int
+    available: bool
     fans: int
     link: str
     share: str
     picture: str
     picture_small: str
     picture_medium: str
     picture_big: str
     picture_xl: str
-    checksum: str
-    creator: User
-    tracks: list[Track]
 
-    def get_tracks(self, **kwargs) -> PaginatedList[Track]:
+    def get_episodes(self, **kwargs) -> PaginatedList[Episode]:
         """
-        Get tracks from a playlist.
+        Get episodes from a podcast
 
         :returns: a :class:`PaginatedList <deezer.PaginatedList>`
-                  of :class:`Track <deezer.Track>` instances
+                  of :class:`Episode <deezer.Episode>` instances
         """
-        return self.get_paginated_list("tracks", **kwargs)
-
-    def get_fans(self, **kwargs) -> PaginatedList[User]:
-        """
-        Get fans from a playlist.
-
-        :returns: a :class:`PaginatedList <deezer.PaginatedList>`
-                  of :class:`User <deezer.User>` instances
-        """
-        return self.get_paginated_list("fans", **kwargs)
+        return self.get_paginated_list("episodes", **kwargs)
```

### Comparing `deezer_python-5.9.0/src/deezer/resources/radio.py` & `deezer_python-6.0.0/src/deezer/resources/radio.py`

 * *Files identical despite different names*

### Comparing `deezer_python-5.9.0/src/deezer/resources/resource.py` & `deezer_python-6.0.0/src/deezer/resources/resource.py`

 * *Files 15% similar despite different names*

```diff
@@ -67,14 +67,40 @@
         return self.client.request(
             "GET",
             f"{self.type}/{self.id}/{relation}",
             parent=self,
             **kwargs,
         )
 
+    def post_relation(self, relation, **kwargs):
+        """
+        Generic method to make a POST request to a relation from any resource.
+
+        This is not meant to be used directly by a client, it's more
+        a helper method for the child objects.
+        """
+        return self.client.request(
+            "POST",
+            f"{self.type}/{self.id}/{relation}",
+            **kwargs,
+        )
+
+    def delete_relation(self, relation, **kwargs):
+        """
+        Generic method to make a DELETE request to a relation from any resource.
+
+        This is not meant to be used directly by a client, it's more
+        a helper method for the child objects.
+        """
+        return self.client.request(
+            "DELETE",
+            f"{self.type}/{self.id}/{relation}",
+            **kwargs,
+        )
+
     def get_paginated_list(
         self,
         relation: str,
         **kwargs,
     ):
         return PaginatedList(
             client=self.client,
```

### Comparing `deezer_python-5.9.0/src/deezer/resources/track.py` & `deezer_python-6.0.0/src/deezer/resources/track.py`

 * *Files identical despite different names*

### Comparing `deezer_python-5.9.0/PKG-INFO` & `deezer_python-6.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: deezer-python
-Version: 5.9.0
+Version: 6.0.0
 Summary: A friendly wrapper library for the Deezer API
 Home-page: https://github.com/browniebroke/deezer-python
 License: MIT
 Keywords: deezer,sdk,client,requests
 Author: Bruno Alla
 Author-email: alla.brunoo@gmail.com
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: requests (>=2.18)
 Project-URL: Bug Tracker, https://github.com/browniebroke/deezer-python/issues
```

#### html2text {}

```diff
@@ -1,27 +1,26 @@
-Metadata-Version: 2.1 Name: deezer-python Version: 5.9.0 Summary: A friendly
+Metadata-Version: 2.1 Name: deezer-python Version: 6.0.0 Summary: A friendly
 wrapper library for the Deezer API Home-page: https://github.com/browniebroke/
 deezer-python License: MIT Keywords: deezer,sdk,client,requests Author: Bruno
-Alla Author-email: alla.brunoo@gmail.com Requires-Python: >=3.7,<4.0
+Alla Author-email: alla.brunoo@gmail.com Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable Classifier: Intended
 Audience :: Developers Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python :: 3 Classifier:
-Programming Language :: Python :: 3.7 Classifier: Programming Language ::
-Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
-Programming Language :: Python :: 3.10 Classifier: Programming Language ::
-Python :: 3.11 Classifier: Topic :: Software Development :: Libraries :: Python
-Modules Requires-Dist: requests (>=2.18) Project-URL: Bug Tracker, https://
-github.com/browniebroke/deezer-python/issues Project-URL: Changelog, https://
-deezer-python.readthedocs.io/en/latest/changelog.html Project-URL:
-Documentation, https://deezer-python.readthedocs.io Project-URL: Mastodon,
-https://fosstodon.org/@browniebroke Project-URL: Repository, https://
-github.com/browniebroke/deezer-python Project-URL: Twitter, https://
-twitter.com/_BrunoAlla Description-Content-Type: text/markdown # Deezer Python
-Client
+Programming Language :: Python :: 3.8 Classifier: Programming Language ::
+Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
+Programming Language :: Python :: 3.11 Classifier: Topic :: Software
+Development :: Libraries :: Python Modules Requires-Dist: requests (>=2.18)
+Project-URL: Bug Tracker, https://github.com/browniebroke/deezer-python/issues
+Project-URL: Changelog, https://deezer-python.readthedocs.io/en/latest/
+changelog.html Project-URL: Documentation, https://deezer-python.readthedocs.io
+Project-URL: Mastodon, https://fosstodon.org/@browniebroke Project-URL:
+Repository, https://github.com/browniebroke/deezer-python Project-URL: Twitter,
+https://twitter.com/_BrunoAlla Description-Content-Type: text/markdown # Deezer
+Python Client
          [CI_Status] [Documentation_Status] [Test_coverage_percentage]
                          [Poetry] [black] [pre-commit]
       [Launch_demo_on_Binder] [PyPi_Status] [pyversions] [license] [LoC]
 --- **Documentation**: https://deezer-python.readthedocs.io **Source Code**:
 https://github.com/browniebroke/deezer-python --- A friendly Python wrapper
 around the [Deezer API](https://developers.deezer.com/api). ## Installation The
 package is published on [PyPI](https://pypi.org/project/deezer-python/) and can
```

