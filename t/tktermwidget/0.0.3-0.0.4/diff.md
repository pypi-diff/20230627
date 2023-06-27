# Comparing `tmp/tktermwidget-0.0.3.tar.gz` & `tmp/tktermwidget-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tktermwidget-0.0.3.tar", last modified: Sun Jun 11 03:02:26 2023, max compression
+gzip compressed data, was "tktermwidget-0.0.4.tar", last modified: Tue Jun 27 06:24:21 2023, max compression
```

## Comparing `tktermwidget-0.0.3.tar` & `tktermwidget-0.0.4.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 03:02:26.074513 tktermwidget-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-06-11 03:02:07.000000 tktermwidget-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-06-11 03:02:26.074513 tktermwidget-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-06-11 03:02:07.000000 tktermwidget-0.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-11 03:02:07.000000 tktermwidget-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-11 03:02:26.074513 tktermwidget-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-06-11 03:02:07.000000 tktermwidget-0.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 03:02:26.074513 tktermwidget-0.0.3/tktermwidget/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-11 03:02:07.000000 tktermwidget-0.0.3/tktermwidget/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9099 2023-06-11 03:02:07.000000 tktermwidget-0.0.3/tktermwidget/tkterm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 03:02:26.074513 tktermwidget-0.0.3/tktermwidget.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-06-11 03:02:26.000000 tktermwidget-0.0.3/tktermwidget.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-06-11 03:02:26.000000 tktermwidget-0.0.3/tktermwidget.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 03:02:26.000000 tktermwidget-0.0.3/tktermwidget.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-11 03:02:26.000000 tktermwidget-0.0.3/tktermwidget.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 06:24:21.981208 tktermwidget-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-06-27 06:24:02.000000 tktermwidget-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-06-27 06:24:21.981208 tktermwidget-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-06-27 06:24:02.000000 tktermwidget-0.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-27 06:24:02.000000 tktermwidget-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 06:24:21.981208 tktermwidget-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-06-27 06:24:02.000000 tktermwidget-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 06:24:21.981208 tktermwidget-0.0.4/tktermwidget/
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-27 06:24:02.000000 tktermwidget-0.0.4/tktermwidget/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-06-27 06:24:02.000000 tktermwidget-0.0.4/tktermwidget/style.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11270 2023-06-27 06:24:02.000000 tktermwidget-0.0.4/tktermwidget/tkterm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 06:24:21.981208 tktermwidget-0.0.4/tktermwidget.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-06-27 06:24:21.000000 tktermwidget-0.0.4/tktermwidget.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-06-27 06:24:21.000000 tktermwidget-0.0.4/tktermwidget.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 06:24:21.000000 tktermwidget-0.0.4/tktermwidget.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-27 06:24:21.000000 tktermwidget-0.0.4/tktermwidget.egg-info/top_level.txt
```

### Comparing `tktermwidget-0.0.3/LICENSE` & `tktermwidget-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `tktermwidget-0.0.3/PKG-INFO` & `tktermwidget-0.0.4/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,26 +1,41 @@
-Metadata-Version: 2.1
-Name: tktermwidget
-Version: 0.0.3
-Summary: A terminal emulator for Tkinter
-Home-page: https://github.com/littlewhitecloud/TkTerminal
-Author: littlewhitecloud
-Description-Content-Type: text/markdown
-License-File: LICENSE
+<h1 align="center"> TkTerminal </h1>
 
-# TkTerminal
-A terminal emulator written in Python using tkinter
+[![PyPI](https://img.shields.io/pypi/v/tktermwidget)](https://pypi.org/project/tktermwidget)
+![Platform](https://img.shields.io/powershellgallery/p/Pester?color=blue)
 
-## Views:
+### 🌏 [简体中文](README_CH.md)
+
+```TkTerminal``` is a terminal emulator written in Python using tkinter. It is quite easy to use.
 ### Windows
-<img src="images/windows.png" width="85%" align="center">
+<img src="images/windows.png" width="75%" align="center">
 
 ### MacOS
 <img src="images/macos.png" width="85%" align="center">
 
+## Features
+- User can set the terminal widget with their own options
+- Use \ to make new lines (On Windows it is &&)
+- Command history recorder
+- Styles
+- And some on
+
+## Future ideas
+- Highlight
+
+## Styles
+```tkterminalwidget``` also have some styles to use such as ```Powershell``` ```Command```:
+![image](https://github.com/littlewhitecloud/TkTerminal/assets/71159641/3affd018-0408-4e91-96de-4775937e0ab8)
+
+
+## Installation:
+```batch
+pip install tktermwidget
+```
+
 ## Example:
 ```python
 from tkinter import Tk
 
 from tkterm import Terminal
 
 # Create root window
@@ -56,11 +71,7 @@
 # Show root window
 root.deiconify()
 
 # Start mainloop
 root.mainloop()
 ```
 
-## Install:
-```batch
-pip install tktermwidget
-```
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `tktermwidget-0.0.3/tktermwidget/tkterm.py` & `tktermwidget-0.0.4/tktermwidget/tkterm.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,228 +5,299 @@
 from pathlib import Path
 from platform import system
 from subprocess import PIPE, Popen
 from tkinter import Event, Misc, Text
 from tkinter.ttk import Frame, Scrollbar
 
 from platformdirs import user_cache_dir
+from style import Default
 
 # Set constants
-HISTORY_PATH = Path(user_cache_dir("tkterm"))
+HISTORY_PATH = Path(user_cache_dir("tktermwidget"))
+HISTORY_FILE = HISTORY_PATH / "history.txt"
 SYSTEM = system()
-CREATE_NEW_CONSOLE = 0
-DIR = "{command}$ "
 if SYSTEM == "Windows":
     from subprocess import CREATE_NEW_CONSOLE
 
-    DIR = "PS {command}>"
+    SIGN = ">"
+else:
+    CREATE_NEW_CONSOLE = 0
+    SIGN = "$ "
 
 # Check that the history directory exists
 if not HISTORY_PATH.exists():
     HISTORY_PATH.mkdir(parents=True)
     # Also create the history file
-    open(HISTORY_PATH / "history.txt", "w").close()
+    with open(HISTORY_FILE, "w", encoding="utf-8") as f:
+        f.close()
 
 # Check that the history file exists
-if not (HISTORY_PATH / "history.txt").exists():
-    open(HISTORY_PATH / "history.txt", "w").close()
+if not (HISTORY_FILE).exists():
+    with open(HISTORY_FILE, "w", encoding="utf-8") as f:
+        f.close()
+
 
 class AutoHideScrollbar(Scrollbar):
     """Scrollbar that automatically hides when not needed"""
 
     def __init__(self, master=None, **kwargs):
         Scrollbar.__init__(self, master=master, **kwargs)
 
     def set(self, first: int, last: int):
+        """Set the Scrollbar"""
         if float(first) <= 0.0 and float(last) >= 1.0:
             self.grid_remove()
         else:
             self.grid()
         Scrollbar.set(self, first, last)
 
+
 class Terminal(Frame):
     """A terminal widget for tkinter applications
 
     Args:
         master (Misc): The parent widget
-        autohide (bool, optional): Whether to autohide the scrollbars. Defaults to True.
+        autohide (bool, optional): Whether to autohide the scrollbars.
+        (Set true to enable it.)
         *args: Arguments for the text widget
         **kwargs: Keyword arguments for the text widget
 
     Methods for outside use:
         None
 
     Methods for internal use:
         up (Event) -> str: Goes up in the history
-        down (Event) -> str: Goes down in the history 
-        (if the user is at the bottom of the history, it clears the command)
-        left (Event) -> str: Goes left in the command if the index is greater than the length of the directory
-        (so the user can't delete the directory or go left of it)
+        down (Event) -> str: Goes down in the history
+        (If the user is at the bottom of the history, it clears the command)
+        left (Event) -> str: Goes left in the command if the index is greater than the directory
+        (So the user can't delete the directory or go left of it)
         kill (Event) -> str: Kills the current command
         loop (Event) -> str: Runs the command typed"""
 
-    def __init__(self, master: Misc, autohide: bool = True, *args, **kwargs):
+    def __init__(
+        self,
+        master: Misc,
+        style: dict = Default,
+        filehistory: str = None,
+        autohide: bool = False,
+        *args,
+        **kwargs,
+    ):
         Frame.__init__(self, master)
 
         # Set row and column weights
         self.rowconfigure(0, weight=1)
         self.columnconfigure(0, weight=1)
 
         # Create text widget and scrollbars
         scrollbars = Scrollbar if not autohide else AutoHideScrollbar
         self.xscroll = scrollbars(self, orient="horizontal")
         self.yscroll = scrollbars(self)
         self.text = Text(
             self,
             *args,
-            background=kwargs.get("background", "#2B2B2B"),
-            insertbackground=kwargs.get("insertbackground", "#DCDCDC"),
-            selectbackground=kwargs.get("selectbackground", "#b4b3b3"),
+            background=kwargs.get("background", style["background"]),
+            insertbackground=kwargs.get("insertbackground", style["insertbackground"]),
+            selectbackground=kwargs.get("selectbackground", style["selectbackground"]),
+            selectforeground=kwargs.get("selectforeground", style["selectforeground"]),
             relief=kwargs.get("relief", "flat"),
-            foreground=kwargs.get("foreground", "#cccccc"),
+            foreground=kwargs.get("foreground", style["foreground"]),
             xscrollcommand=self.xscroll.set,
             yscrollcommand=self.yscroll.set,
             wrap=kwargs.get("wrap", "char"),
             font=kwargs.get("font", ("Cascadia Code", 9, "normal")),
         )
         self.xscroll.config(command=self.text.xview)
         self.yscroll.config(command=self.text.yview)
 
         # Grid widgets
         self.text.grid(row=0, column=0, sticky="nsew")
-        self.xscroll.grid(row=1, column=0, sticky="ew")
+
+        if kwargs.get("wrap", "char") == "none":
+            self.xscroll.grid(row=1, column=0, sticky="ew")
         self.yscroll.grid(row=0, column=1, sticky="ns")
 
         # Create command prompt
         self.directory()
 
         # Set variables
-        self.index = 1
+        self.longflag: bool = False
         self.current_process: Popen | None = None
+        self.index: int = 1
+        self.cursor: int = self.text.index("insert")
+        self.longsymbol: str = "\\" if not SYSTEM == "Windows" else "&&"
+        self.longcmd: str = ""
+        self.filehistory: str = HISTORY_FILE if not filehistory else filehistory
 
-        # Bind events & tags
+        self.latest: int = self.cursor
+
+        # Bind events
         self.text.bind("<Up>", self.up, add=True)
         self.text.bind("<Down>", self.down, add=True)
-        self.text.bind("<Left>", self.left, add=True)
         self.text.bind("<Return>", self.loop, add=True)
-        self.text.bind("<BackSpace>", self.left, add=True)
-
-        # TODO: Refactor the way we get output from subprocess
-        self.text.bind("<Control-KeyPress-c>", self.kill, add=True) # Isn't working
+        for bind_str in ("<Left>", "<BackSpace>"):
+            self.text.bind(bind_str, self.left, add=True)
+        for bind_str in ("<Return>", "<ButtonRelease-1>"):
+            self.text.bind(bind_str, self.check, add=True)
+        self.text.bind("<Control-KeyPress-c>", self.kill, add=True)  # Isn't working
 
         # History recorder
-        self.history = open(HISTORY_PATH / "history.txt", "r+")
+        self.history = open(
+            self.filehistory,
+            "r+",
+            encoding="utf-8",
+        )
+
         self.historys = [i.strip() for i in self.history.readlines() if i.strip()]
-        self.hi = len(self.historys) - 1
+        self.historyindex = len(self.historys) - 1
 
+    def check(self, _: Event) -> None:
+        """Update cursor"""
+        self.cursor = self.text.index("insert")
+        if float(self.cursor) < float(self.latest):
+            self.text.bind("<KeyPress>", self.ignore, True)
+            self.text.bind("<KeyPress-BackSpace>", self.ignore, True)
+        elif float(self.cursor) >= float(self.latest):
+            self.text.unbind("<Key>")
+            self.text.unbind("<KeyPress-Backspace>")
 
-    def directory(self):
+    def directory(self) -> None:
         """Insert the directory"""
-        self.text.insert(
-            "insert",
-            f"{DIR.format(command=getcwd())}",
-        )
+        self.text.insert("insert", getcwd() + SIGN)
+
+    def newline(self) -> None:
+        """Insert a newline"""
+        self.text.insert("insert", "\n")
+        self.index += 1
+
+    def ignore(self, _: Event) -> str:
+        """Ignore the event"""
+        return "break"
 
     def up(self, _: Event) -> str:
         """Go up in the history"""
-        if self.hi >= 0:
+        if self.historyindex >= 0:
             self.text.delete(f"{self.index}.0", "end-1c")
-            # Insert the directory
             self.directory()
             # Insert the command
-            self.text.insert("insert", self.historys[self.hi].strip())
-            self.hi -= 1
+            self.text.insert("insert", self.historys[self.historyindex].strip())
+            self.historyindex -= 1
         return "break"
 
     def down(self, _: Event) -> str:
         """Go down in the history"""
-        if self.hi < len(self.historys) - 1:
+        if self.historyindex < len(self.historys) - 1:
             self.text.delete(f"{self.index}.0", "end-1c")
-            # Insert the directory
             self.directory()
             # Insert the command
-            self.text.insert("insert", self.historys[self.hi].strip())
-            self.hi += 1
+            self.text.insert("insert", self.historys[self.historyindex].strip())
+            self.historyindex += 1
         else:
             # Clear the command
             self.text.delete(f"{self.index}.0", "end-1c")
-            # Insert the directory
             self.directory()
         return "break"
 
     def left(self, _: Event) -> str:
         """Go left in the command if the command is greater than the path"""
         insert_index = self.text.index("insert")
-        dir_index = f"{insert_index.split('.')[0]}.{len(DIR.format(command=getcwd()))}"
+        dir_index = f"{insert_index.split('.')[0]}.{len(getcwd() + SIGN)}"
         if insert_index == dir_index:
             return "break"
 
     def kill(self, _: Event) -> str:
         """Kill the current process"""
         if self.current_process:
             self.current_process.kill()
             self.current_process = None
         return "break"
 
+    def update(self) -> str:
+        """Update or the command has no output"""
+        self.directory()
+        self.check(None)
+        self.latest = self.text.index("insert")
+        self.text.see("end")
+        return "break"
+
     def loop(self, _: Event) -> str:
         """Create an input loop"""
+        # Get the command from the text
         cmd = self.text.get(f"{self.index}.0", "end-1c")
-        # Determine command based on system
-        cmd = cmd.split("$")[-1].strip() if not SYSTEM == "Windows" else cmd.split(">")[-1].strip()
+        cmd = cmd.split(SIGN)[-1].strip()
 
-        # Record the command
-        if cmd != "":
+        if self.longflag:
+            self.longcmd += cmd
+            cmd = self.longcmd
+            self.longcmd = ""
+            self.longflag = False
+
+        if cmd.endswith(self.longsymbol):
+            self.longcmd += cmd.split(self.longsymbol)[0]
+            self.longflag = True
+            self.newline()
+            return "break"
+
+        if cmd:  # Record the command if it isn't empty
             self.history.write(cmd + "\n")
             self.historys.append(cmd)
-            self.hi = len(self.historys) - 1
-        else:
-            self.text.insert("insert", "\n")
-            self.index += 1
+            self.historyindex = len(self.historys) - 1
+        else:  # Leave the loop
+            self.newline()
             self.directory()
+            self.text.see("end")
             return "break"
 
-        # Check that the insert position is at the end
-        if self.text.index("insert") != f"{self.index}.end":
-            self.text.mark_set("insert", f"{self.index}.end")
-            self.text.see("insert")
-
-        # If the command is "clear" or "cls", clear the screen
+        # Check the command if it is a special command
         if cmd in ["clear", "cls"]:
             self.text.delete("1.0", "end")
             self.directory()
             return "break"
+        elif cmd == "exit":
+            self.master.quit()
 
+        # Check that the insert position is at the end
+        if self.text.index("insert") != f"{self.index}.end":
+            self.text.mark_set("insert", f"{self.index}.end")
+            self.text.see("insert")
+
+        # TODO: Refactor the way we get output from subprocess
+        # Run the command
         self.current_process = Popen(
             cmd,
             shell=True,
             stdout=PIPE,
             stderr=PIPE,
             stdin=PIPE,
             text=True,
-            cwd=getcwd(), # Until a solution for changing the working directory is found, this will have to do
+            bufsize=1,
+            universal_newlines=True,
+            cwd=getcwd(),  # TODO: use dynamtic path instead (see #35)
             creationflags=CREATE_NEW_CONSOLE,
         )
-        # The following needs to be put in an after so the kill command works and the program doesn't freeze
+        # The following needs to be put in an after so the kill command works
 
         # Check if the command was successful
-        returnlines, errors, = self.current_process.communicate()
+        output: tuple = self.current_process.communicate()
+        returnlines: str = output[0]
+        errors: str = output[1]
         returncode = self.current_process.returncode
         self.current_process = None
         if returncode != 0:
-            returnlines += errors # If the command was unsuccessful, it doesn't give stdout
-            # TODO: Get the success message from the command (see #16)
-
-        self.text.insert("insert", "\n")
-        self.index += 1
+            returnlines += errors  # If the command was unsuccessful, it doesn't give stdout
+        # TODO: Get the success message from the command (see #16)
+        # Output to the text
+        self.newline()
         for line in returnlines:
             self.text.insert("insert", line)
             if line == "\n":
                 self.index += 1
 
-        self.directory()
+        # Update the text and the index
+        self.update()
         return "break"  # Prevent the default newline character insertion
 
 
 if __name__ == "__main__":
     from tkinter import Tk
 
     # Create root window
```

