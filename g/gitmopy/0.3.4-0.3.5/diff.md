# Comparing `tmp/gitmopy-0.3.4.tar.gz` & `tmp/gitmopy-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gitmopy-0.3.4.tar", max compression
+gzip compressed data, was "gitmopy-0.3.5.tar", max compression
```

## Comparing `gitmopy-0.3.4.tar` & `gitmopy-0.3.5.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1070 2023-06-16 22:59:50.534602 gitmopy-0.3.4/LICENSE
--rw-r--r--   0        0        0     7683 2023-06-19 21:42:16.941940 gitmopy-0.3.4/README.md
--rw-r--r--   0        0        0      112 2023-06-16 19:39:04.304895 gitmopy-0.3.4/gitmopy/__init__.py
--rw-r--r--   0        0        0    14906 2023-06-20 20:50:48.838374 gitmopy-0.3.4/gitmopy/cli.py
--rw-r--r--   0        0        0     6979 2023-06-20 20:54:35.068310 gitmopy-0.3.4/gitmopy/git.py
--rw-r--r--   0        0        0     2972 2023-06-20 20:35:09.442753 gitmopy-0.3.4/gitmopy/history.py
--rw-r--r--   0        0        0     8106 2023-06-19 23:04:51.808559 gitmopy-0.3.4/gitmopy/prompt.py
--rw-r--r--   0        0        0    21278 2023-06-20 20:34:34.169023 gitmopy-0.3.4/gitmopy/utils.py
--rw-r--r--   0        0        0      578 2023-06-20 20:26:39.943844 gitmopy-0.3.4/pyproject.toml
--rw-r--r--   0        0        0     8664 1970-01-01 00:00:00.000000 gitmopy-0.3.4/setup.py
--rw-r--r--   0        0        0     8311 1970-01-01 00:00:00.000000 gitmopy-0.3.4/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-06-16 22:59:50.534602 gitmopy-0.3.5/LICENSE
+-rw-r--r--   0        0        0     7683 2023-06-27 14:21:04.752927 gitmopy-0.3.5/README.md
+-rw-r--r--   0        0        0      112 2023-06-16 19:39:04.304895 gitmopy-0.3.5/gitmopy/__init__.py
+-rw-r--r--   0        0        0    14951 2023-06-27 14:20:26.669404 gitmopy-0.3.5/gitmopy/cli.py
+-rw-r--r--   0        0        0     6871 2023-06-27 14:20:26.669816 gitmopy-0.3.5/gitmopy/git.py
+-rw-r--r--   0        0        0     2972 2023-06-27 13:10:13.038440 gitmopy-0.3.5/gitmopy/history.py
+-rw-r--r--   0        0        0     8761 2023-06-27 14:20:26.670390 gitmopy-0.3.5/gitmopy/prompt.py
+-rw-r--r--   0        0        0    21278 2023-06-27 13:10:13.040862 gitmopy-0.3.5/gitmopy/utils.py
+-rw-r--r--   0        0        0      578 2023-06-27 14:20:39.116461 gitmopy-0.3.5/pyproject.toml
+-rw-r--r--   0        0        0     8664 1970-01-01 00:00:00.000000 gitmopy-0.3.5/setup.py
+-rw-r--r--   0        0        0     8311 1970-01-01 00:00:00.000000 gitmopy-0.3.5/PKG-INFO
```

### Comparing `gitmopy-0.3.4/LICENSE` & `gitmopy-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `gitmopy-0.3.4/README.md` & `gitmopy-0.3.5/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -82,15 +82,15 @@
 
 ## User guide
 
 ```text
 $ gitmopy info
 
 gitmopy info:
-  version : 0.1.0
+  version : 0.3.5
   app path: /Users/victor/.gitmopy
   history : /Users/victor/.gitmopy/history.json
   config  : /Users/victor/.gitmopy/config.yaml
 
 Current configuration:
   skip_scope      : False
   skip_message    : False
```

### Comparing `gitmopy-0.3.4/gitmopy/cli.py` & `gitmopy-0.3.5/gitmopy/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,19 +17,21 @@
 from gitmopy.history import gitmojis_setup, save_to_history
 from gitmopy.prompt import (
     choose_remote_prompt,
     commit_prompt,
     config_prompt,
     git_add_prompt,
     set_upstream_prompt,
+    what_now_prompt,
 )
 from gitmopy.utils import (
     APP_PATH,
     CONFIG_PATH,
     HISTORY_PATH,
+    COLORS,
     _sentinels,
     col,
     console,
     load_config,
     message_from_commit_dict,
     print,
     print_staged_files,
@@ -106,44 +108,37 @@
 
     Returns:
         bool: Whether the user wants to continue or not.
     """
     gitmojis_setup()
     print()
     print(terminal_separator())
-    prompt_txt = (
-        f"🔄 [u]Ready to commit again[/u]. Press {col('enter', 'g', True)} "
-        + "to commit again"
-    )
+    print("\n🔄 [u]Ready to commit again[/u].")
+    choices = {"c": "Commit again"}
 
     print()
     remotes_diff = format_remotes_diff(repo)
     if remotes_diff:
         print(remotes_diff)
-        prompt_txt += f", {col('p', 'b', True)} to push and commit again,"
+        choices["p"] = "Push and commit again"
         if "does not have a branch" not in remotes_diff:
-            prompt_txt += (
-                f" {col('s', 'b', True)} to sync (pull then pull)"
-                + " and commit again,"
-            )
+            choices["s"] = "Sync (pull then push) and commit again"
 
-    print(prompt_txt + f" or {col('q', 'r', True)} to quit.", end="")
+    choices["q"] = "Quit gitmopy"
+    choice = what_now_prompt(choices)
 
-    commit_again = typer.prompt(
-        "", default="enter", show_default=False, prompt_suffix=""
-    )
     if remotes_diff:
-        if commit_again in {"p", "s"}:
+        if choice in {"p", "s"}:
             print()
-            if commit_again == "s":
+            if choice == "s":
                 pull_cli(repo, remote)
             push_cli(repo, remote)
             return should_commit_again(repo, remote)
 
-    commit_again = commit_again != "q"
+    commit_again = choice != "q"
 
     if commit_again:
         print()
 
     return commit_again
 
 
@@ -165,39 +160,44 @@
                 selected_remotes = choose_remote_prompt(repo.remotes)
             if not selected_remotes:
                 # stop if no remote selected
                 print(col("No remote selected. Aborting.", "y"))
                 raise typer.Abort()
             selected_remotes = set(selected_remotes)
 
-        with console.status(col("Fetching remotes...", "o")):
+        with console.status(col("Fetching remotes...", "o"), spinner_style=COLORS["o"]):
             remote_upstreams = has_upstreams(
                 repo, selected_remotes, repo.active_branch.name
             )
 
         # there is at least one remote to push to at this point
         for remote in repo.remotes:
             if remote.name in selected_remotes:
                 wait = col(f"Pushing to remote {remote.name}...", "o")
                 done = col(f"Pushed to remote {remote.name}", "b", True)
+                set_upstream = False
+                if not remote_upstreams[remote.name]:
+                    set_upstream = set_upstream_prompt(remote.name)
+                    if not set_upstream:
+                        print(col(f"Skipping remote {remote.name}.", "y"))
+                        continue
                 with console.status(wait):
                     # push to remote, catch exception if it fails to be able to
                     # 1. continue pushing to other remotes
                     # 2. potentially set the upstream branch
-                    set_upstream = False
-                    if not remote_upstreams[remote.name]:
-                        set_upstream = set_upstream_prompt(remote.name)
                     cre = None
                     if set_upstream:
                         with CatchRemoteException(remote.name) as cre:
                             repo.git.push(
                                 "--set-upstream",
                                 remote.name,
                                 repo.active_branch.name,
                             )
+                        if not cre.error:
+                            done += col(" (upstream branch created)", "b", True)
                     else:
                         with CatchRemoteException(remote.name) as cre:
                             repo.git.push(remote.name, repo.active_branch.name)
                     if cre and not cre.error:
                         print(done)
```

### Comparing `gitmopy-0.3.4/gitmopy/git.py` & `gitmopy-0.3.5/gitmopy/git.py`

 * *Files 6% similar despite different names*

```diff
@@ -83,28 +83,24 @@
     Returns:
         Dict[str, bool]: Dictionnary of booleans indicating if each remote has the
             branch.
     """
 
     fetch_all(repo)
     remote_has_upstream = {
-        r.name if isinstance(r, Remote) else r: None for r in remotes
+        r.name if isinstance(r, Remote) else r: False for r in remotes
     }
-    for r in remotes:
-        if isinstance(r, Remote):
-            r = r.name
-        assert isinstance(r, str)
-        try:
-            repo.git.branch("--list", f"{r}/{branch_name}")
-            remote_has_upstream[r] = True
-        except GitCommandError as e:
-            if "fatal: not a valid revision" in str(e):
-                remote_has_upstream[r] = False
-            else:
-                raise e
+    remote_refs = {
+        ref.remote_name: True
+        for ref in repo.refs
+        if ref.is_remote()
+        and ref.name.removeprefix(ref.remote_name + "/") == branch_name
+    }
+    remote_has_upstream.update(remote_refs)
+
     return remote_has_upstream
 
 
 def get_staged(repo: Repo) -> List[str]:
     """
     Get staged files from a GitPython repository.
 
@@ -244,12 +240,16 @@
     s = f"[u]{col('Remotes diff:', 'g')}[/u]\n"
     for r in repo.remotes:
         if behind[r.name]:
             if behind[r.name] is _sentinels["no-branch"]:
                 b = repo.active_branch
                 s += col(f"remote {r.name} does not have a branch {b}\n", "y")
                 continue
-            s += col(f"local is behind {r.name} by {behind[r.name]} commit(s)\n", "o")
+            s += col(
+                f"  ↵ local is behind {r.name} by {behind[r.name]} commit(s)\n", "o"
+            )
         if ahead[r.name]:
-            s += col(f"local is ahead of {r.name} by {ahead[r.name]} commit(s)\n", "p")
+            s += col(
+                f"  ↳ local is ahead of {r.name} by {ahead[r.name]} commit(s)\n", "p"
+            )
 
     return s
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `gitmopy-0.3.4/gitmopy/history.py` & `gitmopy-0.3.5/gitmopy/history.py`

 * *Files identical despite different names*

### Comparing `gitmopy-0.3.4/gitmopy/prompt.py` & `gitmopy-0.3.5/gitmopy/prompt.py`

 * *Files 6% similar despite different names*

```diff
@@ -264,23 +264,47 @@
         amark="✓",
         transformer=lambda result: "Pushing to " + ", ".join(result),
     ).execute()
 
     return selected
 
 
-def set_upstream_prompt(remote_name: str) -> bool:
+def set_upstream_prompt(branch_name: str, remote_name: str) -> bool:
     """
     Prompt the user to set the upstream branch for a remote.
 
     Args:
+        branch_name (str): Branch name to set on the remote.
         remote_name (str): Remote name.
 
     Returns:
         bool: Whether or not to set the upstream branch.
     """
     return inquirer.confirm(
-        f"Do you want to set the upstream branch for '{remote_name}' now?",
+        f"'{remote_name}' does not have a branch named '{branch_name}'."
+        + " Create upstream branch?",
         qmark="❓",
         amark="✓",
         default=True,
     ).execute()
+
+
+def what_now_prompt(choices: Dict[str, str]) -> str:
+    """
+    Prompt the user to select what to do next. Choices must be a
+    dict like `{value: name}`
+
+    Args:
+        choices (Dict[str, str]): Available choices.
+
+    Returns:
+        str: User's choice.
+    """
+    choices = [Choice(k, v, True) for k, v in choices.items()]
+    return inquirer.select(
+        message="What do you want to do now?",
+        choices=choices,
+        qmark="❓",
+        amark="✓",
+        default=choices[0],
+        cycle=True,
+    ).execute()
```

### Comparing `gitmopy-0.3.4/gitmopy/utils.py` & `gitmopy-0.3.5/gitmopy/utils.py`

 * *Files identical despite different names*

### Comparing `gitmopy-0.3.4/pyproject.toml` & `gitmopy-0.3.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gitmopy"
-version = "0.3.4"
+version = "0.3.5"
 description = "A python command-line for gitmoji"
 authors = ["vict0rsch <vsch@pm.me>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `gitmopy-0.3.4/setup.py` & `gitmopy-0.3.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,17 +14,17 @@
  'typer[all]>=0.8.0']
 
 entry_points = \
 {'console_scripts': ['gitmopy = gitmopy.cli:app']}
 
 setup_kwargs = {
     'name': 'gitmopy',
-    'version': '0.3.4',
+    'version': '0.3.5',
     'description': 'A python command-line for gitmoji',
-    'long_description': '# `gitmopy`\n\nAn interactive Python implementation of the Gitmoji standard: https://gitmoji.dev/\n\n```text\npip install gitmopy\n```\n\n![demo-gitmopy](./assets/demo-gitmopy.gif)\n\n## How to use\n\n* I typically use `$ gitmopy commit --add --keep-alive`\n* Navigate through options with ⬆️ and ⬇️\n* Select option with **`space`**\n* Validate selection with **`enter`**\n* Press **`tab`** to auto-complete\n  * Press `tab` on an empty line to see history\n* Restart commit with **`crtl+c`**\n  * The keyboard interruption will be caught once, then press `enter` to restart\n\n## Suggested shortcuts\n\n```bash\nalias gpy="gitmopy"\nalias gpyc="gitmopy commit"\nalias gpya="gitmopy commit --add"\nalias gpyk="gitmopy commit --add --keep-alive"\n```\n\n![gpyk depo](assets/gpyk.png)\n\n## Examples\n\n```bash\n# Typical daily use-case\n# ----------------------\n\n# continuously commit, interactively select files to stage\n$ gitmopy commit --add --keep-alive\n\n# same using an alias, + push after every commit (could be dangerous)\n$ gpyk --push\n\n\n# Specific usage\n# --------------\n\n# commit currently staged files. Will fail if no file is staged.\n$ gitmopy commit\n\n# Enable interactive file selection if no file is currently staged. Ignored if\n# there are staged files.\n$ gitmopy commit --add\n\n# Commit continuously: don\'t leave the CLI after the first commit but restart\n# the commit procedure.\n$ gitmopy commit --keep-alive\n\n# Push to remote repositories after commit.\n# Interactively select remotes to push to if there are more than 1.\n$ gitmopy commit --push\n\n# Push to specific remotes\n$ gitmopy commit --push --remote origin --remote upstream\n\n# Make and display a commit message without staging/committing/pushing\n$ gitmopy commit --dry\n\n# configure gitmopy\n$ gitmopy config\n\n# print version, data paths and current configuration\n$ gitmopy info\n\n# print helps\n$ gitmopy --help\n$ gitmopy commit --help\n```\n\n⚠️ The sync feature is still experimental. It will `pull` then `push` but in the case of several remotes and the branch not existing on one of them, I recommend you deal with it with `git` manually.\n\n## User guide\n\n```text\n$ gitmopy info\n\ngitmopy info:\n  version : 0.1.0\n  app path: /Users/victor/.gitmopy\n  history : /Users/victor/.gitmopy/history.json\n  config  : /Users/victor/.gitmopy/config.yaml\n\nCurrent configuration:\n  skip_scope      : False\n  skip_message    : False\n  capitalize_title: True\n  enable_history  : True\n```\n\nUpdate configuration with\n\n```text\n$ gitmopy config\n$ gitmopy config\n❓ Configure gitmopy locally. Use \'space\' to (de-)select, \'enter\' to validate.\n❯ ○ Skip commit scope\n  ○ Skip commit message\n  ◉ Capitalize commit title\n  ◉ Remember commit history for auto-complete and emoji sorting\n\nConfig will be saved in /Users/victor/.gitmopy/config.yaml.\n```\n\nGet help with\n\n```text\n$ gitmopy --help\n\n Usage: gitmopy [OPTIONS] COMMAND [ARGS]...\n\n╭─ Options ───────────────────────────────────────────────────────────────────────────╮\n│ --install-completion          Install completion for the current shell.             │\n│ --show-completion             Show completion for the current shell, to copy it or  │\n│                               customize the installation.                           │\n│ --help                        Show this message and exit.                           │\n╰─────────────────────────────────────────────────────────────────────────────────────╯\n╭─ Commands ──────────────────────────────────────────────────────────────────────────╮\n│ commit  Commit staged files. Use --add to interactively select files to stage if    │\n│         none is already staged                                                      │\n│ config  Configure gitmopy                                                           │\n│ info    Print gitmopy info                                                          │\n╰─────────────────────────────────────────────────────────────────────────────────────╯\n\n$ gitmopy commit --help\n\n Usage: gitmopy commit [OPTIONS]\n\n Commit staged files. Use --add to interactively select files to stage if none is\n already staged\n\n╭─ Options ───────────────────────────────────────────────────────────────────────────╮\n│ --repo                             TEXT  Path to the git repository [default: .]    │\n│ --add           --no-add                 Whether or not to interactively select     │\n│                                          files to stage if none is already staged   │\n│                                          [default: no-add]                          │\n│ --push          --no-push                Whether to `git push` after commit. If     │\n│                                          multiple remotes exist, you will be asked  │\n│                                          to interactively choose the ones to push   │\n│                                          to. Use --remote to skip interactive       │\n│                                          selection. Disabled by default.            │\n│                                          [default: no-push]                         │\n│ --dry           --no-dry                 Whether or not to actually commit.         │\n│                                          [default: no-dry]                          │\n│ --remote                           TEXT  Remote to push to after commit. Use to     │\n│                                          skip interactive remote selection when     │\n│                                          several exist. Use several \'--remote       │\n│                                          {remote name}\' to push to multiple remotes │\n│ --keep-alive    --no-keep-alive          Whether or not to keep the app alive after │\n│                                          commit, to be ready for another one.       │\n│                                          [default: no-keep-alive]                   │\n│ --help                                   Show this message and exit.                │\n╰─────────────────────────────────────────────────────────────────────────────────────╯\n```\n\n## To Do\n\n* Features\n  * *If requested:*\n    * Install hook\n    * `git commit` flags (like `-S`)\n    * max history length (if loading the json becomes slow)\n* Tests\n  * https://typer.tiangolo.com/tutorial/testing/\n  * 👋 **Help wanted**\n* Docs\n  * Not critical\n\n## Resources\n\n`gitmopy` is inspired by [`gitmoji-cli`](https://github.com/carloscuesta/gitmoji-cli).\n\nIt is built thanks to:\n\n* [`typer`](https://github.com/tiangolo/typer)\n* [`InquirePy`](https://github.com/kazhala/InquirerPy)\n* [`GitPython`](https://github.com/gitpython-developers/GitPython)\n',
+    'long_description': '# `gitmopy`\n\nAn interactive Python implementation of the Gitmoji standard: https://gitmoji.dev/\n\n```text\npip install gitmopy\n```\n\n![demo-gitmopy](./assets/demo-gitmopy.gif)\n\n## How to use\n\n* I typically use `$ gitmopy commit --add --keep-alive`\n* Navigate through options with ⬆️ and ⬇️\n* Select option with **`space`**\n* Validate selection with **`enter`**\n* Press **`tab`** to auto-complete\n  * Press `tab` on an empty line to see history\n* Restart commit with **`crtl+c`**\n  * The keyboard interruption will be caught once, then press `enter` to restart\n\n## Suggested shortcuts\n\n```bash\nalias gpy="gitmopy"\nalias gpyc="gitmopy commit"\nalias gpya="gitmopy commit --add"\nalias gpyk="gitmopy commit --add --keep-alive"\n```\n\n![gpyk depo](assets/gpyk.png)\n\n## Examples\n\n```bash\n# Typical daily use-case\n# ----------------------\n\n# continuously commit, interactively select files to stage\n$ gitmopy commit --add --keep-alive\n\n# same using an alias, + push after every commit (could be dangerous)\n$ gpyk --push\n\n\n# Specific usage\n# --------------\n\n# commit currently staged files. Will fail if no file is staged.\n$ gitmopy commit\n\n# Enable interactive file selection if no file is currently staged. Ignored if\n# there are staged files.\n$ gitmopy commit --add\n\n# Commit continuously: don\'t leave the CLI after the first commit but restart\n# the commit procedure.\n$ gitmopy commit --keep-alive\n\n# Push to remote repositories after commit.\n# Interactively select remotes to push to if there are more than 1.\n$ gitmopy commit --push\n\n# Push to specific remotes\n$ gitmopy commit --push --remote origin --remote upstream\n\n# Make and display a commit message without staging/committing/pushing\n$ gitmopy commit --dry\n\n# configure gitmopy\n$ gitmopy config\n\n# print version, data paths and current configuration\n$ gitmopy info\n\n# print helps\n$ gitmopy --help\n$ gitmopy commit --help\n```\n\n⚠️ The sync feature is still experimental. It will `pull` then `push` but in the case of several remotes and the branch not existing on one of them, I recommend you deal with it with `git` manually.\n\n## User guide\n\n```text\n$ gitmopy info\n\ngitmopy info:\n  version : 0.3.5\n  app path: /Users/victor/.gitmopy\n  history : /Users/victor/.gitmopy/history.json\n  config  : /Users/victor/.gitmopy/config.yaml\n\nCurrent configuration:\n  skip_scope      : False\n  skip_message    : False\n  capitalize_title: True\n  enable_history  : True\n```\n\nUpdate configuration with\n\n```text\n$ gitmopy config\n$ gitmopy config\n❓ Configure gitmopy locally. Use \'space\' to (de-)select, \'enter\' to validate.\n❯ ○ Skip commit scope\n  ○ Skip commit message\n  ◉ Capitalize commit title\n  ◉ Remember commit history for auto-complete and emoji sorting\n\nConfig will be saved in /Users/victor/.gitmopy/config.yaml.\n```\n\nGet help with\n\n```text\n$ gitmopy --help\n\n Usage: gitmopy [OPTIONS] COMMAND [ARGS]...\n\n╭─ Options ───────────────────────────────────────────────────────────────────────────╮\n│ --install-completion          Install completion for the current shell.             │\n│ --show-completion             Show completion for the current shell, to copy it or  │\n│                               customize the installation.                           │\n│ --help                        Show this message and exit.                           │\n╰─────────────────────────────────────────────────────────────────────────────────────╯\n╭─ Commands ──────────────────────────────────────────────────────────────────────────╮\n│ commit  Commit staged files. Use --add to interactively select files to stage if    │\n│         none is already staged                                                      │\n│ config  Configure gitmopy                                                           │\n│ info    Print gitmopy info                                                          │\n╰─────────────────────────────────────────────────────────────────────────────────────╯\n\n$ gitmopy commit --help\n\n Usage: gitmopy commit [OPTIONS]\n\n Commit staged files. Use --add to interactively select files to stage if none is\n already staged\n\n╭─ Options ───────────────────────────────────────────────────────────────────────────╮\n│ --repo                             TEXT  Path to the git repository [default: .]    │\n│ --add           --no-add                 Whether or not to interactively select     │\n│                                          files to stage if none is already staged   │\n│                                          [default: no-add]                          │\n│ --push          --no-push                Whether to `git push` after commit. If     │\n│                                          multiple remotes exist, you will be asked  │\n│                                          to interactively choose the ones to push   │\n│                                          to. Use --remote to skip interactive       │\n│                                          selection. Disabled by default.            │\n│                                          [default: no-push]                         │\n│ --dry           --no-dry                 Whether or not to actually commit.         │\n│                                          [default: no-dry]                          │\n│ --remote                           TEXT  Remote to push to after commit. Use to     │\n│                                          skip interactive remote selection when     │\n│                                          several exist. Use several \'--remote       │\n│                                          {remote name}\' to push to multiple remotes │\n│ --keep-alive    --no-keep-alive          Whether or not to keep the app alive after │\n│                                          commit, to be ready for another one.       │\n│                                          [default: no-keep-alive]                   │\n│ --help                                   Show this message and exit.                │\n╰─────────────────────────────────────────────────────────────────────────────────────╯\n```\n\n## To Do\n\n* Features\n  * *If requested:*\n    * Install hook\n    * `git commit` flags (like `-S`)\n    * max history length (if loading the json becomes slow)\n* Tests\n  * https://typer.tiangolo.com/tutorial/testing/\n  * 👋 **Help wanted**\n* Docs\n  * Not critical\n\n## Resources\n\n`gitmopy` is inspired by [`gitmoji-cli`](https://github.com/carloscuesta/gitmoji-cli).\n\nIt is built thanks to:\n\n* [`typer`](https://github.com/tiangolo/typer)\n* [`InquirePy`](https://github.com/kazhala/InquirerPy)\n* [`GitPython`](https://github.com/gitpython-developers/GitPython)\n',
     'author': 'vict0rsch',
     'author_email': 'vsch@pm.me',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `gitmopy-0.3.4/PKG-INFO` & `gitmopy-0.3.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gitmopy
-Version: 0.3.4
+Version: 0.3.5
 Summary: A python command-line for gitmoji
 License: MIT
 Author: vict0rsch
 Author-email: vsch@pm.me
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -101,15 +101,15 @@
 
 ## User guide
 
 ```text
 $ gitmopy info
 
 gitmopy info:
-  version : 0.1.0
+  version : 0.3.5
   app path: /Users/victor/.gitmopy
   history : /Users/victor/.gitmopy/history.json
   config  : /Users/victor/.gitmopy/config.yaml
 
 Current configuration:
   skip_scope      : False
   skip_message    : False
```

