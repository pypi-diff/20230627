# Comparing `tmp/gitmopy-0.3.5.1.tar.gz` & `tmp/gitmopy-0.3.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gitmopy-0.3.5.1.tar", max compression
+gzip compressed data, was "gitmopy-0.3.5.2.tar", max compression
```

## Comparing `gitmopy-0.3.5.1.tar` & `gitmopy-0.3.5.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1070 2023-06-16 22:59:50.534602 gitmopy-0.3.5.1/LICENSE
--rw-r--r--   0        0        0     7758 2023-06-27 19:10:12.417496 gitmopy-0.3.5.1/README.md
--rw-r--r--   0        0        0      112 2023-06-16 19:39:04.304895 gitmopy-0.3.5.1/gitmopy/__init__.py
--rw-r--r--   0        0        0    15022 2023-06-27 19:06:35.770663 gitmopy-0.3.5.1/gitmopy/cli.py
--rw-r--r--   0        0        0     6871 2023-06-27 14:20:26.669816 gitmopy-0.3.5.1/gitmopy/git.py
--rw-r--r--   0        0        0     2972 2023-06-27 13:10:13.038440 gitmopy-0.3.5.1/gitmopy/history.py
--rw-r--r--   0        0        0     8761 2023-06-27 14:20:26.670390 gitmopy-0.3.5.1/gitmopy/prompt.py
--rw-r--r--   0        0        0    21278 2023-06-27 13:10:13.040862 gitmopy-0.3.5.1/gitmopy/utils.py
--rw-r--r--   0        0        0      580 2023-06-27 19:08:19.470248 gitmopy-0.3.5.1/pyproject.toml
--rw-r--r--   0        0        0     8743 1970-01-01 00:00:00.000000 gitmopy-0.3.5.1/setup.py
--rw-r--r--   0        0        0     8388 1970-01-01 00:00:00.000000 gitmopy-0.3.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-06-16 22:59:50.534602 gitmopy-0.3.5.2/LICENSE
+-rw-r--r--   0        0        0     7758 2023-06-27 19:13:53.503733 gitmopy-0.3.5.2/README.md
+-rw-r--r--   0        0        0      112 2023-06-16 19:39:04.304895 gitmopy-0.3.5.2/gitmopy/__init__.py
+-rw-r--r--   0        0        0    15076 2023-06-27 19:13:12.371022 gitmopy-0.3.5.2/gitmopy/cli.py
+-rw-r--r--   0        0        0     6871 2023-06-27 14:20:26.669816 gitmopy-0.3.5.2/gitmopy/git.py
+-rw-r--r--   0        0        0     2972 2023-06-27 13:10:13.038440 gitmopy-0.3.5.2/gitmopy/history.py
+-rw-r--r--   0        0        0     8761 2023-06-27 14:20:26.670390 gitmopy-0.3.5.2/gitmopy/prompt.py
+-rw-r--r--   0        0        0    21278 2023-06-27 13:10:13.040862 gitmopy-0.3.5.2/gitmopy/utils.py
+-rw-r--r--   0        0        0      580 2023-06-27 19:13:44.007974 gitmopy-0.3.5.2/pyproject.toml
+-rw-r--r--   0        0        0     8743 1970-01-01 00:00:00.000000 gitmopy-0.3.5.2/setup.py
+-rw-r--r--   0        0        0     8388 1970-01-01 00:00:00.000000 gitmopy-0.3.5.2/PKG-INFO
```

### Comparing `gitmopy-0.3.5.1/LICENSE` & `gitmopy-0.3.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `gitmopy-0.3.5.1/README.md` & `gitmopy-0.3.5.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -84,15 +84,15 @@
 
 ## User guide
 
 ```text
 $ gitmopy info
 
 gitmopy info:
-  version : 0.3.5.1
+  version : 0.3.5.2
   app path: /Users/victor/.gitmopy
   history : /Users/victor/.gitmopy/history.json
   config  : /Users/victor/.gitmopy/config.yaml
 
 Current configuration:
   skip_scope      : False
   skip_message    : False
```

### Comparing `gitmopy-0.3.5.1/gitmopy/cli.py` & `gitmopy-0.3.5.2/gitmopy/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -178,15 +178,15 @@
                 if not remote_upstreams[remote.name]:
                     set_upstream = set_upstream_prompt(
                         repo.active_branch.name, remote.name
                     )
                     if not set_upstream:
                         print(col(f"Skipping remote {remote.name}.", "y"))
                         continue
-                with console.status(wait):
+                with console.status(wait, spinner_style=COLORS["o"]):
                     # push to remote, catch exception if it fails to be able to
                     # 1. continue pushing to other remotes
                     # 2. potentially set the upstream branch
                     cre = None
                     if set_upstream:
                         with CatchRemoteException(remote.name) as cre:
                             repo.git.push(
@@ -226,15 +226,15 @@
         print()
 
         # there is at least one remote to push to at this point
         for remote in repo.remotes:
             if remote.name in selected_remotes:
                 wait = col(f"Pulling from remote {remote.name}...", "o")
                 done = col(f"Pulled from remote {remote.name}", "b", True)
-                with console.status(wait):
+                with console.status(wait, spinner_style=COLORS["o"]):
                     cre = None
                     with CatchRemoteException(remote.name) as cre:
                         repo.git.pull(remote.name, repo.active_branch.name)
                     if cre and not cre.error:
                         print(done)
```

### Comparing `gitmopy-0.3.5.1/gitmopy/git.py` & `gitmopy-0.3.5.2/gitmopy/git.py`

 * *Files identical despite different names*

### Comparing `gitmopy-0.3.5.1/gitmopy/history.py` & `gitmopy-0.3.5.2/gitmopy/history.py`

 * *Files identical despite different names*

### Comparing `gitmopy-0.3.5.1/gitmopy/prompt.py` & `gitmopy-0.3.5.2/gitmopy/prompt.py`

 * *Files identical despite different names*

### Comparing `gitmopy-0.3.5.1/gitmopy/utils.py` & `gitmopy-0.3.5.2/gitmopy/utils.py`

 * *Files identical despite different names*

### Comparing `gitmopy-0.3.5.1/pyproject.toml` & `gitmopy-0.3.5.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gitmopy"
-version = "0.3.5.1"
+version = "0.3.5.2"
 description = "A python command-line for gitmoji"
 authors = ["vict0rsch <vsch@pm.me>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `gitmopy-0.3.5.1/setup.py` & `gitmopy-0.3.5.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,17 +14,17 @@
  'typer[all]>=0.8.0']
 
 entry_points = \
 {'console_scripts': ['gitmopy = gitmopy.cli:app']}
 
 setup_kwargs = {
     'name': 'gitmopy',
-    'version': '0.3.5.1',
+    'version': '0.3.5.2',
     'description': 'A python command-line for gitmoji',
-    'long_description': '# `gitmopy`\n\nAn interactive Python implementation of the Gitmoji standard: https://gitmoji.dev/\n\n```text\npip install gitmopy\n```\n\n![demo-gitmopy](./assets/demo-gitmopy.gif)\n\n## How to use\n\n* I typically use `$ gitmopy commit --add --keep-alive`\n* Navigate through options with ⬆️ and ⬇️\n* **Select** option with **`space`**\n* **Validate** selection with **`enter`**\n* Press **`tab`** to **auto-complete**\n  * Press `tab` on an empty line to see history\n* **Restart commit** with **`crtl+c`**\n  * The keyboard interruption will be caught once, then press `enter` to restart\n* Push (and set upstream if need be)\n* Commit again 🔄\n\n## Suggested shortcuts\n\n```bash\nalias gpy="gitmopy"\nalias gpyc="gitmopy commit"\nalias gpya="gitmopy commit --add"\nalias gpyk="gitmopy commit --add --keep-alive"\n```\n\n![gpyk depo](assets/gpyk.png)\n\n## Examples\n\n```bash\n# Typical daily use-case\n# ----------------------\n\n# continuously commit, interactively select files to stage\n$ gitmopy commit --add --keep-alive\n\n# same using an alias, + push after every commit (could be dangerous)\n$ gpyk --push\n\n\n# Specific usage\n# --------------\n\n# commit currently staged files. Will fail if no file is staged.\n$ gitmopy commit\n\n# Enable interactive file selection if no file is currently staged. Ignored if\n# there are staged files.\n$ gitmopy commit --add\n\n# Commit continuously: don\'t leave the CLI after the first commit but restart\n# the commit procedure.\n$ gitmopy commit --keep-alive\n\n# Push to remote repositories after commit.\n# Interactively select remotes to push to if there are more than 1.\n$ gitmopy commit --push\n\n# Push to specific remotes\n$ gitmopy commit --push --remote origin --remote upstream\n\n# Make and display a commit message without staging/committing/pushing\n$ gitmopy commit --dry\n\n# configure gitmopy\n$ gitmopy config\n\n# print version, data paths and current configuration\n$ gitmopy info\n\n# print helps\n$ gitmopy --help\n$ gitmopy commit --help\n```\n\n⚠️ The sync feature is still experimental. It will `pull` then `push` but in the case of several remotes and the branch not existing on one of them, I recommend you deal with it with `git` manually.\n\n## User guide\n\n```text\n$ gitmopy info\n\ngitmopy info:\n  version : 0.3.5.1\n  app path: /Users/victor/.gitmopy\n  history : /Users/victor/.gitmopy/history.json\n  config  : /Users/victor/.gitmopy/config.yaml\n\nCurrent configuration:\n  skip_scope      : False\n  skip_message    : False\n  capitalize_title: True\n  enable_history  : True\n```\n\nUpdate configuration with\n\n```text\n$ gitmopy config\n$ gitmopy config\n❓ Configure gitmopy locally. Use \'space\' to (de-)select, \'enter\' to validate.\n❯ ○ Skip commit scope\n  ○ Skip commit message\n  ◉ Capitalize commit title\n  ◉ Remember commit history for auto-complete and emoji sorting\n\nConfig will be saved in /Users/victor/.gitmopy/config.yaml.\n```\n\nGet help with\n\n```text\n$ gitmopy --help\n\n Usage: gitmopy [OPTIONS] COMMAND [ARGS]...\n\n╭─ Options ───────────────────────────────────────────────────────────────────────────╮\n│ --install-completion          Install completion for the current shell.             │\n│ --show-completion             Show completion for the current shell, to copy it or  │\n│                               customize the installation.                           │\n│ --help                        Show this message and exit.                           │\n╰─────────────────────────────────────────────────────────────────────────────────────╯\n╭─ Commands ──────────────────────────────────────────────────────────────────────────╮\n│ commit  Commit staged files. Use --add to interactively select files to stage if    │\n│         none is already staged                                                      │\n│ config  Configure gitmopy                                                           │\n│ info    Print gitmopy info                                                          │\n╰─────────────────────────────────────────────────────────────────────────────────────╯\n\n$ gitmopy commit --help\n\n Usage: gitmopy commit [OPTIONS]\n\n Commit staged files. Use --add to interactively select files to stage if none is\n already staged\n\n╭─ Options ───────────────────────────────────────────────────────────────────────────╮\n│ --repo                             TEXT  Path to the git repository [default: .]    │\n│ --add           --no-add                 Whether or not to interactively select     │\n│                                          files to stage if none is already staged   │\n│                                          [default: no-add]                          │\n│ --push          --no-push                Whether to `git push` after commit. If     │\n│                                          multiple remotes exist, you will be asked  │\n│                                          to interactively choose the ones to push   │\n│                                          to. Use --remote to skip interactive       │\n│                                          selection. Disabled by default.            │\n│                                          [default: no-push]                         │\n│ --dry           --no-dry                 Whether or not to actually commit.         │\n│                                          [default: no-dry]                          │\n│ --remote                           TEXT  Remote to push to after commit. Use to     │\n│                                          skip interactive remote selection when     │\n│                                          several exist. Use several \'--remote       │\n│                                          {remote name}\' to push to multiple remotes │\n│ --keep-alive    --no-keep-alive          Whether or not to keep the app alive after │\n│                                          commit, to be ready for another one.       │\n│                                          [default: no-keep-alive]                   │\n│ --help                                   Show this message and exit.                │\n╰─────────────────────────────────────────────────────────────────────────────────────╯\n```\n\n## To Do\n\n* Features\n  * *If requested:*\n    * Install hook\n    * `git commit` flags (like `-S`)\n    * max history length (if loading the json becomes slow)\n* Tests\n  * https://typer.tiangolo.com/tutorial/testing/\n  * 👋 **Help wanted**\n* Docs\n  * Not critical\n\n## Resources\n\n`gitmopy` is inspired by [`gitmoji-cli`](https://github.com/carloscuesta/gitmoji-cli).\n\nIt is built thanks to:\n\n* [`typer`](https://github.com/tiangolo/typer)\n* [`InquirePy`](https://github.com/kazhala/InquirerPy)\n* [`GitPython`](https://github.com/gitpython-developers/GitPython)\n',
+    'long_description': '# `gitmopy`\n\nAn interactive Python implementation of the Gitmoji standard: https://gitmoji.dev/\n\n```text\npip install gitmopy\n```\n\n![demo-gitmopy](./assets/demo-gitmopy.gif)\n\n## How to use\n\n* I typically use `$ gitmopy commit --add --keep-alive`\n* Navigate through options with ⬆️ and ⬇️\n* **Select** option with **`space`**\n* **Validate** selection with **`enter`**\n* Press **`tab`** to **auto-complete**\n  * Press `tab` on an empty line to see history\n* **Restart commit** with **`crtl+c`**\n  * The keyboard interruption will be caught once, then press `enter` to restart\n* Push (and set upstream if need be)\n* Commit again 🔄\n\n## Suggested shortcuts\n\n```bash\nalias gpy="gitmopy"\nalias gpyc="gitmopy commit"\nalias gpya="gitmopy commit --add"\nalias gpyk="gitmopy commit --add --keep-alive"\n```\n\n![gpyk depo](assets/gpyk.png)\n\n## Examples\n\n```bash\n# Typical daily use-case\n# ----------------------\n\n# continuously commit, interactively select files to stage\n$ gitmopy commit --add --keep-alive\n\n# same using an alias, + push after every commit (could be dangerous)\n$ gpyk --push\n\n\n# Specific usage\n# --------------\n\n# commit currently staged files. Will fail if no file is staged.\n$ gitmopy commit\n\n# Enable interactive file selection if no file is currently staged. Ignored if\n# there are staged files.\n$ gitmopy commit --add\n\n# Commit continuously: don\'t leave the CLI after the first commit but restart\n# the commit procedure.\n$ gitmopy commit --keep-alive\n\n# Push to remote repositories after commit.\n# Interactively select remotes to push to if there are more than 1.\n$ gitmopy commit --push\n\n# Push to specific remotes\n$ gitmopy commit --push --remote origin --remote upstream\n\n# Make and display a commit message without staging/committing/pushing\n$ gitmopy commit --dry\n\n# configure gitmopy\n$ gitmopy config\n\n# print version, data paths and current configuration\n$ gitmopy info\n\n# print helps\n$ gitmopy --help\n$ gitmopy commit --help\n```\n\n⚠️ The sync feature is still experimental. It will `pull` then `push` but in the case of several remotes and the branch not existing on one of them, I recommend you deal with it with `git` manually.\n\n## User guide\n\n```text\n$ gitmopy info\n\ngitmopy info:\n  version : 0.3.5.2\n  app path: /Users/victor/.gitmopy\n  history : /Users/victor/.gitmopy/history.json\n  config  : /Users/victor/.gitmopy/config.yaml\n\nCurrent configuration:\n  skip_scope      : False\n  skip_message    : False\n  capitalize_title: True\n  enable_history  : True\n```\n\nUpdate configuration with\n\n```text\n$ gitmopy config\n$ gitmopy config\n❓ Configure gitmopy locally. Use \'space\' to (de-)select, \'enter\' to validate.\n❯ ○ Skip commit scope\n  ○ Skip commit message\n  ◉ Capitalize commit title\n  ◉ Remember commit history for auto-complete and emoji sorting\n\nConfig will be saved in /Users/victor/.gitmopy/config.yaml.\n```\n\nGet help with\n\n```text\n$ gitmopy --help\n\n Usage: gitmopy [OPTIONS] COMMAND [ARGS]...\n\n╭─ Options ───────────────────────────────────────────────────────────────────────────╮\n│ --install-completion          Install completion for the current shell.             │\n│ --show-completion             Show completion for the current shell, to copy it or  │\n│                               customize the installation.                           │\n│ --help                        Show this message and exit.                           │\n╰─────────────────────────────────────────────────────────────────────────────────────╯\n╭─ Commands ──────────────────────────────────────────────────────────────────────────╮\n│ commit  Commit staged files. Use --add to interactively select files to stage if    │\n│         none is already staged                                                      │\n│ config  Configure gitmopy                                                           │\n│ info    Print gitmopy info                                                          │\n╰─────────────────────────────────────────────────────────────────────────────────────╯\n\n$ gitmopy commit --help\n\n Usage: gitmopy commit [OPTIONS]\n\n Commit staged files. Use --add to interactively select files to stage if none is\n already staged\n\n╭─ Options ───────────────────────────────────────────────────────────────────────────╮\n│ --repo                             TEXT  Path to the git repository [default: .]    │\n│ --add           --no-add                 Whether or not to interactively select     │\n│                                          files to stage if none is already staged   │\n│                                          [default: no-add]                          │\n│ --push          --no-push                Whether to `git push` after commit. If     │\n│                                          multiple remotes exist, you will be asked  │\n│                                          to interactively choose the ones to push   │\n│                                          to. Use --remote to skip interactive       │\n│                                          selection. Disabled by default.            │\n│                                          [default: no-push]                         │\n│ --dry           --no-dry                 Whether or not to actually commit.         │\n│                                          [default: no-dry]                          │\n│ --remote                           TEXT  Remote to push to after commit. Use to     │\n│                                          skip interactive remote selection when     │\n│                                          several exist. Use several \'--remote       │\n│                                          {remote name}\' to push to multiple remotes │\n│ --keep-alive    --no-keep-alive          Whether or not to keep the app alive after │\n│                                          commit, to be ready for another one.       │\n│                                          [default: no-keep-alive]                   │\n│ --help                                   Show this message and exit.                │\n╰─────────────────────────────────────────────────────────────────────────────────────╯\n```\n\n## To Do\n\n* Features\n  * *If requested:*\n    * Install hook\n    * `git commit` flags (like `-S`)\n    * max history length (if loading the json becomes slow)\n* Tests\n  * https://typer.tiangolo.com/tutorial/testing/\n  * 👋 **Help wanted**\n* Docs\n  * Not critical\n\n## Resources\n\n`gitmopy` is inspired by [`gitmoji-cli`](https://github.com/carloscuesta/gitmoji-cli).\n\nIt is built thanks to:\n\n* [`typer`](https://github.com/tiangolo/typer)\n* [`InquirePy`](https://github.com/kazhala/InquirerPy)\n* [`GitPython`](https://github.com/gitpython-developers/GitPython)\n',
     'author': 'vict0rsch',
     'author_email': 'vsch@pm.me',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `gitmopy-0.3.5.1/PKG-INFO` & `gitmopy-0.3.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gitmopy
-Version: 0.3.5.1
+Version: 0.3.5.2
 Summary: A python command-line for gitmoji
 License: MIT
 Author: vict0rsch
 Author-email: vsch@pm.me
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -103,15 +103,15 @@
 
 ## User guide
 
 ```text
 $ gitmopy info
 
 gitmopy info:
-  version : 0.3.5.1
+  version : 0.3.5.2
   app path: /Users/victor/.gitmopy
   history : /Users/victor/.gitmopy/history.json
   config  : /Users/victor/.gitmopy/config.yaml
 
 Current configuration:
   skip_scope      : False
   skip_message    : False
```

