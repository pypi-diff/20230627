# Comparing `tmp/frogmouth-0.6.0.tar.gz` & `tmp/frogmouth-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "frogmouth-0.6.0.tar", max compression
+gzip compressed data, was "frogmouth-0.7.0.tar", max compression
```

## Comparing `frogmouth-0.6.0.tar` & `frogmouth-0.7.0.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0     1072 2023-04-27 14:46:52.801782 frogmouth-0.6.0/LICENSE
--rw-r--r--   0        0        0     2752 2023-04-30 07:26:36.700670 frogmouth-0.6.0/README.md
--rw-r--r--   0        0        0      283 2023-05-24 09:22:14.385143 frogmouth-0.6.0/frogmouth/__init__.py
--rw-r--r--   0        0        0      112 2023-04-27 14:46:52.802125 frogmouth-0.6.0/frogmouth/__main__.py
--rw-r--r--   0        0        0       74 2023-04-27 14:46:52.802222 frogmouth-0.6.0/frogmouth/app/__init__.py
--rw-r--r--   0        0        0     2070 2023-04-30 11:10:42.375933 frogmouth-0.6.0/frogmouth/app/app.py
--rw-r--r--   0        0        0      395 2023-04-27 14:46:52.802403 frogmouth-0.6.0/frogmouth/data/__init__.py
--rw-r--r--   0        0        0     1639 2023-04-27 14:46:52.802497 frogmouth-0.6.0/frogmouth/data/bookmarks.py
--rw-r--r--   0        0        0     2270 2023-05-09 08:04:58.867587 frogmouth-0.6.0/frogmouth/data/config.py
--rw-r--r--   0        0        0      582 2023-04-27 14:46:52.802650 frogmouth-0.6.0/frogmouth/data/data_directory.py
--rw-r--r--   0        0        0     1370 2023-04-27 14:46:52.802714 frogmouth-0.6.0/frogmouth/data/history.py
--rw-r--r--   0        0        0      354 2023-04-27 14:46:52.802828 frogmouth-0.6.0/frogmouth/dialogs/__init__.py
--rw-r--r--   0        0        0      565 2023-04-28 13:52:42.406602 frogmouth-0.6.0/frogmouth/dialogs/error.py
--rw-r--r--   0        0        0     4616 2023-05-18 13:41:34.483482 frogmouth-0.6.0/frogmouth/dialogs/help_dialog.py
--rw-r--r--   0        0        0      269 2023-04-27 14:55:30.387330 frogmouth-0.6.0/frogmouth/dialogs/information.py
--rw-r--r--   0        0        0     2544 2023-05-09 08:04:58.868437 frogmouth-0.6.0/frogmouth/dialogs/input_dialog.py
--rw-r--r--   0        0        0     2168 2023-04-29 20:35:07.295162 frogmouth-0.6.0/frogmouth/dialogs/text_dialog.py
--rw-r--r--   0        0        0     3602 2023-05-03 09:31:33.036152 frogmouth-0.6.0/frogmouth/dialogs/yes_no_dialog.py
--rw-r--r--   0        0        0       83 2023-04-27 14:46:52.803485 frogmouth-0.6.0/frogmouth/screens/__init__.py
--rw-r--r--   0        0        0    18949 2023-05-18 13:41:34.483651 frogmouth-0.6.0/frogmouth/screens/main.py
--rw-r--r--   0        0        0      402 2023-05-18 13:41:34.484301 frogmouth-0.6.0/frogmouth/utility/__init__.py
--rw-r--r--   0        0        0      894 2023-04-28 13:00:47.734733 frogmouth-0.6.0/frogmouth/utility/advertising.py
--rw-r--r--   0        0        0     5135 2023-05-18 13:41:34.484397 frogmouth-0.6.0/frogmouth/utility/forge.py
--rw-r--r--   0        0        0     1206 2023-05-09 08:04:58.868785 frogmouth-0.6.0/frogmouth/utility/type_tests.py
--rw-r--r--   0        0        0      184 2023-04-27 14:46:52.804110 frogmouth-0.6.0/frogmouth/widgets/__init__.py
--rw-r--r--   0        0        0     6015 2023-05-09 08:04:58.868929 frogmouth-0.6.0/frogmouth/widgets/navigation.py
--rw-r--r--   0        0        0      298 2023-04-27 14:46:52.804311 frogmouth-0.6.0/frogmouth/widgets/navigation_panes/__init__.py
--rw-r--r--   0        0        0     5633 2023-05-03 09:31:33.037203 frogmouth-0.6.0/frogmouth/widgets/navigation_panes/bookmarks.py
--rw-r--r--   0        0        0     5685 2023-05-09 08:04:58.869061 frogmouth-0.6.0/frogmouth/widgets/navigation_panes/history.py
--rw-r--r--   0        0        0     3071 2023-05-09 08:04:58.869180 frogmouth-0.6.0/frogmouth/widgets/navigation_panes/local_files.py
--rw-r--r--   0        0        0      665 2023-05-03 09:31:33.037312 frogmouth-0.6.0/frogmouth/widgets/navigation_panes/navigation_pane.py
--rw-r--r--   0        0        0     2341 2023-05-09 08:04:58.869286 frogmouth-0.6.0/frogmouth/widgets/navigation_panes/table_of_contents.py
--rw-r--r--   0        0        0    12260 2023-05-18 13:41:34.484532 frogmouth-0.6.0/frogmouth/widgets/omnibox.py
--rw-r--r--   0        0        0    10750 2023-05-09 08:04:58.872361 frogmouth-0.6.0/frogmouth/widgets/viewer.py
--rw-r--r--   0        0        0     1470 2023-05-24 09:22:14.385940 frogmouth-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     4323 1970-01-01 00:00:00.000000 frogmouth-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-04-27 14:46:52.801782 frogmouth-0.7.0/LICENSE
+-rw-r--r--   0        0        0     2752 2023-04-30 07:26:36.700670 frogmouth-0.7.0/README.md
+-rw-r--r--   0        0        0      283 2023-06-27 08:26:21.273197 frogmouth-0.7.0/frogmouth/__init__.py
+-rw-r--r--   0        0        0      112 2023-04-27 14:46:52.802125 frogmouth-0.7.0/frogmouth/__main__.py
+-rw-r--r--   0        0        0       74 2023-04-27 14:46:52.802222 frogmouth-0.7.0/frogmouth/app/__init__.py
+-rw-r--r--   0        0        0     2070 2023-04-30 11:10:42.375933 frogmouth-0.7.0/frogmouth/app/app.py
+-rw-r--r--   0        0        0      395 2023-04-27 14:46:52.802403 frogmouth-0.7.0/frogmouth/data/__init__.py
+-rw-r--r--   0        0        0     1639 2023-04-27 14:46:52.802497 frogmouth-0.7.0/frogmouth/data/bookmarks.py
+-rw-r--r--   0        0        0     2270 2023-05-09 08:04:58.867587 frogmouth-0.7.0/frogmouth/data/config.py
+-rw-r--r--   0        0        0      582 2023-04-27 14:46:52.802650 frogmouth-0.7.0/frogmouth/data/data_directory.py
+-rw-r--r--   0        0        0     1370 2023-04-27 14:46:52.802714 frogmouth-0.7.0/frogmouth/data/history.py
+-rw-r--r--   0        0        0      354 2023-04-27 14:46:52.802828 frogmouth-0.7.0/frogmouth/dialogs/__init__.py
+-rw-r--r--   0        0        0      565 2023-04-28 13:52:42.406602 frogmouth-0.7.0/frogmouth/dialogs/error.py
+-rw-r--r--   0        0        0     4658 2023-05-30 09:10:09.565607 frogmouth-0.7.0/frogmouth/dialogs/help_dialog.py
+-rw-r--r--   0        0        0      269 2023-04-27 14:55:30.387330 frogmouth-0.7.0/frogmouth/dialogs/information.py
+-rw-r--r--   0        0        0     2544 2023-05-09 08:04:58.868437 frogmouth-0.7.0/frogmouth/dialogs/input_dialog.py
+-rw-r--r--   0        0        0     2168 2023-04-29 20:35:07.295162 frogmouth-0.7.0/frogmouth/dialogs/text_dialog.py
+-rw-r--r--   0        0        0     3602 2023-05-03 09:31:33.036152 frogmouth-0.7.0/frogmouth/dialogs/yes_no_dialog.py
+-rw-r--r--   0        0        0       83 2023-04-27 14:46:52.803485 frogmouth-0.7.0/frogmouth/screens/__init__.py
+-rw-r--r--   0        0        0    20103 2023-05-30 09:10:09.565826 frogmouth-0.7.0/frogmouth/screens/main.py
+-rw-r--r--   0        0        0      402 2023-05-18 13:41:34.484301 frogmouth-0.7.0/frogmouth/utility/__init__.py
+-rw-r--r--   0        0        0      894 2023-04-28 13:00:47.734733 frogmouth-0.7.0/frogmouth/utility/advertising.py
+-rw-r--r--   0        0        0     5373 2023-05-30 09:10:09.565984 frogmouth-0.7.0/frogmouth/utility/forge.py
+-rw-r--r--   0        0        0     1206 2023-05-09 08:04:58.868785 frogmouth-0.7.0/frogmouth/utility/type_tests.py
+-rw-r--r--   0        0        0      184 2023-04-27 14:46:52.804110 frogmouth-0.7.0/frogmouth/widgets/__init__.py
+-rw-r--r--   0        0        0     6015 2023-05-09 08:04:58.868929 frogmouth-0.7.0/frogmouth/widgets/navigation.py
+-rw-r--r--   0        0        0      298 2023-04-27 14:46:52.804311 frogmouth-0.7.0/frogmouth/widgets/navigation_panes/__init__.py
+-rw-r--r--   0        0        0     5633 2023-05-03 09:31:33.037203 frogmouth-0.7.0/frogmouth/widgets/navigation_panes/bookmarks.py
+-rw-r--r--   0        0        0     5685 2023-05-09 08:04:58.869061 frogmouth-0.7.0/frogmouth/widgets/navigation_panes/history.py
+-rw-r--r--   0        0        0     3071 2023-05-09 08:04:58.869180 frogmouth-0.7.0/frogmouth/widgets/navigation_panes/local_files.py
+-rw-r--r--   0        0        0      665 2023-05-03 09:31:33.037312 frogmouth-0.7.0/frogmouth/widgets/navigation_panes/navigation_pane.py
+-rw-r--r--   0        0        0     2341 2023-05-09 08:04:58.869286 frogmouth-0.7.0/frogmouth/widgets/navigation_panes/table_of_contents.py
+-rw-r--r--   0        0        0    12260 2023-05-18 13:41:34.484532 frogmouth-0.7.0/frogmouth/widgets/omnibox.py
+-rw-r--r--   0        0        0    10907 2023-05-30 09:10:09.566549 frogmouth-0.7.0/frogmouth/widgets/viewer.py
+-rw-r--r--   0        0        0     1470 2023-06-27 08:28:04.508561 frogmouth-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0     4323 1970-01-01 00:00:00.000000 frogmouth-0.7.0/PKG-INFO
```

### Comparing `frogmouth-0.6.0/LICENSE` & `frogmouth-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `frogmouth-0.6.0/README.md` & `frogmouth-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `frogmouth-0.6.0/frogmouth/app/app.py` & `frogmouth-0.7.0/frogmouth/app/app.py`

 * *Files identical despite different names*

### Comparing `frogmouth-0.6.0/frogmouth/data/bookmarks.py` & `frogmouth-0.7.0/frogmouth/data/bookmarks.py`

 * *Files identical despite different names*

### Comparing `frogmouth-0.6.0/frogmouth/data/config.py` & `frogmouth-0.7.0/frogmouth/data/config.py`

 * *Files identical despite different names*

### Comparing `frogmouth-0.6.0/frogmouth/data/data_directory.py` & `frogmouth-0.7.0/frogmouth/data/data_directory.py`

 * *Files identical despite different names*

### Comparing `frogmouth-0.6.0/frogmouth/data/history.py` & `frogmouth-0.7.0/frogmouth/data/history.py`

 * *Files identical despite different names*

### Comparing `frogmouth-0.6.0/frogmouth/dialogs/error.py` & `frogmouth-0.7.0/frogmouth/dialogs/error.py`

 * *Files identical despite different names*

### Comparing `frogmouth-0.6.0/frogmouth/dialogs/help_dialog.py` & `frogmouth-0.7.0/frogmouth/dialogs/help_dialog.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,29 +37,30 @@
 | `Ctrl+right` | Go forward in history |
 
 ## General keys
 
 | Key | Command |
 | -- | -- |
 | `Ctrl+d` | Add the current document to the bookmarks |
+| `Ctrl+r` | Reload the current document |
 | `Ctrl+q` | Quit the application |
 | `F1` | This help |
 | `F2` | Details about {APPLICATION_TITLE} |
 | `F10` | Toggle dark/light theme |
 
 ## Commands
 
 Press `/` or click the address bar, then enter any of the following commands:
 
 | Command | Aliases | Arguments | Command |
 | -- | -- | -- | -- |
 | `about` | `a` | | Show details about the application |
 | `bookmarks` | `b`, `bm` | | Show the bookmarks list |
 | `bitbucket` | `bb` | `<repo-info>` | View a file on BitBucket (see below) |
-| `codeberg` | `cb` | `<repo-info>` | View a file on Codceberg (see below) |
+| `codeberg` | `cb` | `<repo-info>` | View a file on Codeberg (see below) |
 | `changelog` | `cl` | | View the Frogmouth ChangeLog |
 | `chdir` | `cd` | `<dir>` | Switch the local file browser to a new directory |
 | `contents` | `c`, `toc` | | Show the table of contents for the document |
 | `discord` | | | Visit the Textualize Discord server |
 | `github` | `gh` | `<repo-info>` | View a file on GitHub (see below) |
 | `gitlab` | `gl` | `<repo-info>` | View a file on GitLab (see below) |
 | `help` | `?` | | Show this document |
```

### Comparing `frogmouth-0.6.0/frogmouth/dialogs/input_dialog.py` & `frogmouth-0.7.0/frogmouth/dialogs/input_dialog.py`

 * *Files identical despite different names*

### Comparing `frogmouth-0.6.0/frogmouth/dialogs/text_dialog.py` & `frogmouth-0.7.0/frogmouth/dialogs/text_dialog.py`

 * *Files identical despite different names*

### Comparing `frogmouth-0.6.0/frogmouth/dialogs/yes_no_dialog.py` & `frogmouth-0.7.0/frogmouth/dialogs/yes_no_dialog.py`

 * *Files identical despite different names*

### Comparing `frogmouth-0.6.0/frogmouth/screens/main.py` & `frogmouth-0.7.0/frogmouth/screens/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,14 +74,15 @@
     BINDINGS = [
         Binding("/,:", "omnibox", "Omnibox", show=False),
         Binding("ctrl+b", "bookmarks", "", show=False),
         Binding("ctrl+d", "bookmark_this", "", show=False),
         Binding("ctrl+l", "local_files", "", show=False),
         Binding("ctrl+left", "backward", "", show=False),
         Binding("ctrl+right", "forward", "", show=False),
+        Binding("ctrl+r", "reload", "", show=False),
         Binding("ctrl+t", "table_of_contents", "", show=False),
         Binding("ctrl+y", "history", "", show=False),
         Binding("escape", "escape", "", show=False),
         Binding("f1", "help", "Help"),
         Binding("f2", "about", "About"),
         Binding("ctrl+n", "navigation", "Navigation"),
         Binding("ctrl+q", "app.quit", "Quit"),
@@ -123,15 +124,15 @@
             # ...attempt to visit it in the viewer.
             self.query_one(Viewer).visit(location, remember)
         elif isinstance(location, Path):
             # So, it's not Markdown, but it *is* a Path of some sort. If the
             # resource seems to exist...
             if location.exists():
                 # ...ask the OS to open it.
-                open_url(str(location))
+                open_url(f"file:///{location.absolute()}")
             else:
                 # It's a Path but it doesn't exist, there's not much else we
                 # can do with it.
                 self.app.push_screen(
                     ErrorDialog(
                         "Does not exist",
                         f"Unable to open {location} because it does not exist.",
@@ -381,27 +382,48 @@
 
     def on_markdown_link_clicked(self, event: Markdown.LinkClicked) -> None:
         """Handle a link being clicked in the Markdown document.
 
         Args:
             event: The Markdown link click event to handle.
         """
+        # We'll be using the current location to help work out some relative
+        # things.
+        current_location = self.query_one(Viewer).location
         # If the link we're to handle obviously looks like URL...
         if is_likely_url(event.href):
-            # ...handle it as such. No point in truing trying to do anything
-            # else.
+            # ...handle it as such. No point in trying to do anything else.
             self.visit(URL(event.href))
-        elif isinstance(current_location := self.query_one(Viewer).location, URL):
+        elif isinstance(current_location, URL):
             # Seems we're currently visiting a remote location, and the href
             # looks like a simple file path, so let's make a best effort to
             # visit the file at the remote location.
             self.visit(current_location.copy_with().join(event.href))
+        elif (local_file := Path(event.href)).exists():
+            # It looks like a local file and it exists...
+            self.visit(local_file)
+        elif (
+            isinstance(current_location, Path)
+            and (local_file := (current_location.parent / Path(event.href)))
+            .absolute()
+            .exists()
+        ):
+            # It looks like a local file, and tested relative to the
+            # document we found it exists in the local filesystem, so let's
+            # assume that's what we're supposed to handle.
+            self.visit(local_file)
         else:
-            # Final option is that it's a local path.
-            self.visit(Path(event.href))
+            # Yeah, not sure *what* this link is. Rather than silently fail,
+            # let's let the user know we don't know how to process this.
+            self.app.push_screen(
+                ErrorDialog(
+                    "Unable to handle link",
+                    f"Unable to work out how to handle this link:\n\n{event.href}",
+                )
+            )
 
     def on_paste(self, event: Paste) -> None:
         """Handle a paste event.
 
         Args:
             event: The paste event.
 
@@ -516,7 +538,11 @@
     def action_toggle_theme(self) -> None:
         """Toggle the light/dark mode theme."""
         config = load_config()
         config.light_mode = not config.light_mode
         save_config(config)
         # pylint:disable=attribute-defined-outside-init
         self.app.dark = not config.light_mode
+
+    def action_reload(self) -> None:
+        """Reload the current document."""
+        self.query_one(Viewer).reload()
```

### Comparing `frogmouth-0.6.0/frogmouth/utility/advertising.py` & `frogmouth-0.7.0/frogmouth/utility/advertising.py`

 * *Files identical despite different names*

### Comparing `frogmouth-0.6.0/frogmouth/utility/forge.py` & `frogmouth-0.7.0/frogmouth/utility/forge.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Code for getting files from a forge."""
 
 from __future__ import annotations
 
-from httpx import URL, AsyncClient, HTTPStatusError
+from httpx import URL, AsyncClient, HTTPStatusError, RequestError
 
 from .advertising import USER_AGENT
 
 
 async def build_raw_forge_url(
     url_format: str,
     owner: str,
@@ -35,19 +35,24 @@
         for test_branch in (branch,) if branch else ("main", "master"):
             url = url_format.format(
                 owner=owner,
                 repository=repository,
                 branch=test_branch,
                 file=desired_file,
             )
-            response = await client.head(
-                url,
-                follow_redirects=True,
-                headers={"user-agent": USER_AGENT},
-            )
+            try:
+                response = await client.head(
+                    url,
+                    follow_redirects=True,
+                    headers={"user-agent": USER_AGENT},
+                )
+            except RequestError:
+                # We've failed to even make the request, there's no point in
+                # trying to build anything here.
+                return None
             try:
                 response.raise_for_status()
                 return URL(url)
             except HTTPStatusError:
                 pass
     return None
```

### Comparing `frogmouth-0.6.0/frogmouth/utility/type_tests.py` & `frogmouth-0.7.0/frogmouth/utility/type_tests.py`

 * *Files identical despite different names*

### Comparing `frogmouth-0.6.0/frogmouth/widgets/navigation.py` & `frogmouth-0.7.0/frogmouth/widgets/navigation.py`

 * *Files identical despite different names*

### Comparing `frogmouth-0.6.0/frogmouth/widgets/navigation_panes/bookmarks.py` & `frogmouth-0.7.0/frogmouth/widgets/navigation_panes/bookmarks.py`

 * *Files identical despite different names*

### Comparing `frogmouth-0.6.0/frogmouth/widgets/navigation_panes/history.py` & `frogmouth-0.7.0/frogmouth/widgets/navigation_panes/history.py`

 * *Files identical despite different names*

### Comparing `frogmouth-0.6.0/frogmouth/widgets/navigation_panes/local_files.py` & `frogmouth-0.7.0/frogmouth/widgets/navigation_panes/local_files.py`

 * *Files identical despite different names*

### Comparing `frogmouth-0.6.0/frogmouth/widgets/navigation_panes/navigation_pane.py` & `frogmouth-0.7.0/frogmouth/widgets/navigation_panes/navigation_pane.py`

 * *Files identical despite different names*

### Comparing `frogmouth-0.6.0/frogmouth/widgets/navigation_panes/table_of_contents.py` & `frogmouth-0.7.0/frogmouth/widgets/navigation_panes/table_of_contents.py`

 * *Files identical despite different names*

### Comparing `frogmouth-0.6.0/frogmouth/widgets/omnibox.py` & `frogmouth-0.7.0/frogmouth/widgets/omnibox.py`

 * *Files identical despite different names*

### Comparing `frogmouth-0.6.0/frogmouth/widgets/viewer.py` & `frogmouth-0.7.0/frogmouth/widgets/viewer.py`

 * *Files 1% similar despite different names*

```diff
@@ -260,14 +260,19 @@
         if isinstance(location, Path):
             self._local_load(location.expanduser().resolve(), remember)
         elif isinstance(location, URL):
             self._remote_load(location, remember)
         else:
             raise ValueError("Unknown location type passed to the Markdown viewer")
 
+    def reload(self) -> None:
+        """Reload the current location."""
+        if self.location is not None:
+            self.visit(self.location, False)
+
     def show(self, content: str) -> None:
         """Show some direct text in the viewer.
 
         Args:
             content: The text to show.
         """
         self.viewing_location = False
```

### Comparing `frogmouth-0.6.0/pyproject.toml` & `frogmouth-0.7.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "frogmouth"
 homepage = "https://github.com/Textualize/frogmouth"
-version = "0.6.0"
+version = "0.7.0"
 description = "A Markdown document viewer for the terminal"
 authors = ["Dave Pearson <dave@textualize.io>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "frogmouth"}]
 classifiers = [
     "Development Status :: 4 - Beta",
@@ -24,22 +24,22 @@
     "Programming Language :: Python :: 3.9",
     "Topic :: Software Development :: Documentation",
     "Topic :: Text Processing :: Markup :: Markdown",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
-textual = {version = ">=0.24.0"}
+textual = {version = ">=0.28.1"}
 typing-extensions = "^4.5.0"
-httpx = "^0.23.3"
+httpx = "^0.24.1"
 xdg = "^6.0.0"
 
 
 [tool.poetry.group.dev.dependencies]
-textual = {extras = ["dev"], version = ">=0.24.0"}
+textual = {extras = ["dev"], version = ">=0.28.1"}
 mypy = "^1.1.1"
 pylint = "^2.17.1"
 pre-commit = "^3.2.1"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `frogmouth-0.6.0/PKG-INFO` & `frogmouth-0.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: frogmouth
-Version: 0.6.0
+Version: 0.7.0
 Summary: A Markdown document viewer for the terminal
 Home-page: https://github.com/Textualize/frogmouth
 License: MIT
 Author: Dave Pearson
 Author-email: dave@textualize.io
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 4 - Beta
@@ -25,16 +25,16 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Documentation
 Classifier: Topic :: Text Processing :: Markup :: Markdown
-Requires-Dist: httpx (>=0.23.3,<0.24.0)
-Requires-Dist: textual (>=0.24.0)
+Requires-Dist: httpx (>=0.24.1,<0.25.0)
+Requires-Dist: textual (>=0.28.1)
 Requires-Dist: typing-extensions (>=4.5.0,<5.0.0)
 Requires-Dist: xdg (>=6.0.0,<7.0.0)
 Description-Content-Type: text/markdown
 
 
 <p align="center">
   <img src="https://user-images.githubusercontent.com/554369/234892488-856f9da7-7b82-4429-ac35-0d0545bf0d24.png"  width="300" align="center"/>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: frogmouth Version: 0.6.0 Summary: A Markdown
+Metadata-Version: 2.1 Name: frogmouth Version: 0.7.0 Summary: A Markdown
 document viewer for the terminal Home-page: https://github.com/Textualize/
 frogmouth License: MIT Author: Dave Pearson Author-email: dave@textualize.io
 Requires-Python: >=3.8,<4.0 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: End Users/Desktop Classifier: Intended
 Audience :: Information Technology Classifier: Intended Audience :: Other
 Audience Classifier: License :: OSI Approved :: MIT License Classifier:
@@ -12,16 +12,16 @@
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Topic :: Software
 Development :: Documentation Classifier: Topic :: Text Processing :: Markup ::
-Markdown Requires-Dist: httpx (>=0.23.3,<0.24.0) Requires-Dist: textual
-(>=0.24.0) Requires-Dist: typing-extensions (>=4.5.0,<5.0.0) Requires-Dist: xdg
+Markdown Requires-Dist: httpx (>=0.24.1,<0.25.0) Requires-Dist: textual
+(>=0.28.1) Requires-Dist: typing-extensions (>=4.5.0,<5.0.0) Requires-Dist: xdg
 (>=6.0.0,<7.0.0) Description-Content-Type: text/markdown
 [https://user-images.githubusercontent.com/554369/234892488-856f9da7-7b82-4429-
                             ac35-0d0545bf0d24.png]
 [![Discord](https://img.shields.io/discord/1026214085173461072)](https://
 discord.gg/Enf6Z3qhVr) # Frogmouth Frogmouth is a Markdown viewer / browser for
 your terminal, built with [Textual](https://github.com/Textualize/textual).
 Frogmouth can open `*.md` files locally or via a URL. There is a familiar
```

