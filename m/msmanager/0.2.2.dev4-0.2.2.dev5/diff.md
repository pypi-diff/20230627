# Comparing `tmp/msmanager-0.2.2.dev4.tar.gz` & `tmp/msmanager-0.2.2.dev5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "msmanager-0.2.2.dev4.tar", max compression
+gzip compressed data, was "msmanager-0.2.2.dev5.tar", max compression
```

## Comparing `msmanager-0.2.2.dev4.tar` & `msmanager-0.2.2.dev5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1111 2023-05-14 16:04:08.180554 msmanager-0.2.2.dev4/LICENSE
--rw-r--r--   0        0        0      267 2023-05-15 20:57:42.797028 msmanager-0.2.2.dev4/msmanager/__init__.py
--rw-r--r--   0        0        0       67 2023-05-15 21:27:48.138274 msmanager-0.2.2.dev4/msmanager/__main__.py
--rw-r--r--   0        0        0     7494 2023-06-27 12:26:03.594529 msmanager-0.2.2.dev4/msmanager/cli.py
--rw-r--r--   0        0        0     2488 2023-05-15 19:04:10.101041 msmanager-0.2.2.dev4/msmanager/config.py
--rw-r--r--   0        0        0     3231 2023-06-26 19:57:01.709315 msmanager-0.2.2.dev4/msmanager/exceptions.py
--rw-r--r--   0        0        0     3995 2023-06-27 12:16:45.380300 msmanager-0.2.2.dev4/msmanager/functions.py
--rw-r--r--   0        0        0      384 2023-05-16 16:36:36.800666 msmanager-0.2.2.dev4/msmanager/models.py
--rw-r--r--   0        0        0     2983 2023-06-13 10:18:25.381658 msmanager-0.2.2.dev4/msmanager/msm.py
--rw-r--r--   0        0        0      143 2023-05-15 19:04:10.113824 msmanager-0.2.2.dev4/msmanager/types.py
--rw-r--r--   0        0        0      591 2023-06-27 12:26:12.585541 msmanager-0.2.2.dev4/msmanager/units.py
--rw-r--r--   0        0        0      552 2023-06-27 12:26:09.464418 msmanager-0.2.2.dev4/pyproject.toml
--rw-r--r--   0        0        0      704 2023-06-21 22:49:16.590585 msmanager-0.2.2.dev4/README.md
--rw-r--r--   0        0        0     1505 1970-01-01 00:00:00.000000 msmanager-0.2.2.dev4/PKG-INFO
+-rw-r--r--   0        0        0     1111 2023-05-14 16:04:08.180554 msmanager-0.2.2.dev5/LICENSE
+-rw-r--r--   0        0        0      267 2023-05-15 20:57:42.797028 msmanager-0.2.2.dev5/msmanager/__init__.py
+-rw-r--r--   0        0        0       67 2023-05-15 21:27:48.138274 msmanager-0.2.2.dev5/msmanager/__main__.py
+-rw-r--r--   0        0        0     7516 2023-06-27 13:08:18.129893 msmanager-0.2.2.dev5/msmanager/cli.py
+-rw-r--r--   0        0        0     2488 2023-05-15 19:04:10.101041 msmanager-0.2.2.dev5/msmanager/config.py
+-rw-r--r--   0        0        0     3231 2023-06-26 19:57:01.709315 msmanager-0.2.2.dev5/msmanager/exceptions.py
+-rw-r--r--   0        0        0     3995 2023-06-27 12:16:45.380300 msmanager-0.2.2.dev5/msmanager/functions.py
+-rw-r--r--   0        0        0      384 2023-05-16 16:36:36.800666 msmanager-0.2.2.dev5/msmanager/models.py
+-rw-r--r--   0        0        0     2983 2023-06-13 10:18:25.381658 msmanager-0.2.2.dev5/msmanager/msm.py
+-rw-r--r--   0        0        0      143 2023-05-15 19:04:10.113824 msmanager-0.2.2.dev5/msmanager/types.py
+-rw-r--r--   0        0        0      591 2023-06-27 13:08:46.386897 msmanager-0.2.2.dev5/msmanager/units.py
+-rw-r--r--   0        0        0      552 2023-06-27 12:57:20.099377 msmanager-0.2.2.dev5/pyproject.toml
+-rw-r--r--   0        0        0      704 2023-06-21 22:49:16.590585 msmanager-0.2.2.dev5/README.md
+-rw-r--r--   0        0        0     1505 1970-01-01 00:00:00.000000 msmanager-0.2.2.dev5/PKG-INFO
```

### Comparing `msmanager-0.2.2.dev4/LICENSE` & `msmanager-0.2.2.dev5/LICENSE`

 * *Files identical despite different names*

### Comparing `msmanager-0.2.2.dev4/msmanager/cli.py` & `msmanager-0.2.2.dev5/msmanager/cli.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 import click
 from rich.console import Console
-from typing import Iterable, Optional
+from typing import Iterable, Optional, Callable, Any
 # > Local Imports
 from .units import (
     __version__ as prog_version,
     __title__ as prog_name
 )
 from .msm import MSManager
 from .models import MindustryServerConfig
@@ -27,14 +27,24 @@
 # ! Functions
 def printexcept(e: Exception):
     if debag_mode:
         console.print_exception(word_wrap=True, show_locals=True)
     else:
         console.print(rich_exception(e))
 
+def hand_exception():
+    def hand_exception_wrapper(func: Callable[..., Any]):
+        def hand_exception_wrapped(*args, **kwargs):
+            try:
+                return func(*args, **kwargs)
+            except Exception as e:
+                printexcept(e)
+        return hand_exception_wrapped
+    return hand_exception_wrapper
+
 # ! Commands
 # ? Add Command
 @click.command("add", help="Add a server to the config.")
 @click.argument("screen_name", type=str)
 @click.argument("executable_filepath", type=click.Path(exists=True))
 @click.option(
     "-a", "--arg", "arguments",
@@ -53,86 +63,79 @@
     type=int, default=None, show_default=True
 )
 @click.option(
     "-i", "--input-port", "input_port",
     help="Server input port for telnet connection.",
     type=int, default=None, show_default=True
 )
+@hand_exception()
 def adder(
     screen_name: str,
     executable_filepath: str,
     arguments: Iterable[str],
     host: Optional[str],
     port: Optional[int],
     input_port: Optional[int]
 ):
-    try:
-        msmanager.add_server_config(
-            MindustryServerConfig(
-                screen_name=screen_name,
-                work_dirpath=os.path.dirname(os.path.abspath(executable_filepath)),
-                executable_filepath=os.path.abspath(executable_filepath),
-                arguments=list(arguments),
-                host=host, port=port, input_port=input_port
-            )
+    msmanager.add_server_config(
+        MindustryServerConfig(
+            screen_name=screen_name,
+            work_dirpath=os.path.dirname(os.path.abspath(executable_filepath)),
+            executable_filepath=os.path.abspath(executable_filepath),
+            arguments=list(arguments),
+            host=host, port=port, input_port=input_port
         )
-        console.print("[green]>[/] Server [bold yellow]added[/]!")
-    except Exception as e:
-        printexcept(e)
+    )
+    console.print("[green]>[/] Server [bold yellow]added[/]!")
 
 # ? Remove Command
 @click.command("remove", help="Remove the server from the config.")
 @click.argument("screen_name", type=str)
+@hand_exception()
 def remover(screen_name: str):
-    try:
-        msmanager.remove_server_config(screen_name)
-        console.print("[green]>[/] Server [bold yellow]removed[/]!")
-    except Exception as e:
-        printexcept(e)
+    msmanager.remove_server_config(screen_name)
+    console.print("[green]>[/] Server [bold yellow]removed[/]!")
 
 # ? Start Command
 @click.command("start", help="Run the server.")
 @click.argument("screen_name", type=str)
 @click.option(
     "-w", "--wait", "wait",
     help="Waiting for the server to start up.",
     is_flag=True
 )
+@hand_exception()
 def starter(screen_name: str, wait: bool):
-    try:
-        msmanager.start_server(screen_name)
-        if (server_config:=msmanager.get_server_config(screen_name)) is not None:
-            if is_server_connect_correct(server_config.host, server_config.port, server_config.input_port) and wait:
-                wait_start_server(server_config.host, server_config.port, server_config.input_port)
-        console.print("[green]>[/] Server [bold yellow]started[/]!")
-    except Exception as e:
-        printexcept(e)
+    msmanager.start_server(screen_name)
+    if (server_config:=msmanager.get_server_config(screen_name)) is not None:
+        if is_server_connect_correct(server_config.host, server_config.port, server_config.input_port) and wait:
+            wait_start_server(server_config.host, server_config.port, server_config.input_port)
+    console.print("[green]>[/] Server [bold yellow]started[/]!")
 
 # ? Stop Command
 @click.command("stop", help="Stop the server.")
 @click.argument("screen_name", type=str)
+@hand_exception()
 def stoper(screen_name: str):
-    try:
-        msmanager.stop_server(screen_name)
-        console.print("[green]>[/] Server [bold yellow]stoped[/]!")
-    except Exception as e:
-        printexcept(e)
+    msmanager.stop_server(screen_name)
+    console.print("[green]>[/] Server [bold yellow]stoped[/]!")
 
 # ? List Command
 @click.command("list", help="List of servers in the config.")
 @click.option(
     "--pinging", "pinging",
     help="Whether to do a ping to check.",
     is_flag=True, default=False
 )
 @click.option(
     "-t", "--timeout", "timeout",
     help="Maximum response waiting time (in seconds).",
     type=int, default=10, show_default=True
 )
+@hand_exception()
 def lister(pinging: bool, timeout: int):
     try:
         if len(msmanager.config.config.servers) != 0:
             for idx, server in enumerate(msmanager.config.config.servers):
                 lines = [
                     f"({idx}) Server {repr(server.screen_name)}:",
                     f"[magenta]Executable Filepath[/] : {repr(server.executable_filepath)}",
@@ -157,39 +160,37 @@
 @click.command("ping", help="Server status check.")
 @click.argument("connect", type=str)
 @click.option(
     "-t", "--timeout", "timeout",
     help="Maximum response waiting time (in seconds).",
     type=int, default=10, show_default=True
 )
+@hand_exception()
 def pinger(connect: str, timeout: int):
-    try:
-        if (server_config:=msmanager.get_server_config(connect)) is not None:
-            connect_data = {"host": server_config.host, "port": server_config.port}
-        else:
-            try:
-                connect_data = parse_connect_data(connect)
-            except VBMLParseError:
-                raise IncorrectConnectionDataError(connect)
-        status = ping(connect_data["host"], connect_data["port"], timeout)
-        console.print(
-            "\n\t".join(
-                [
-                    f"[green]>[/] Server {endicext(status.name)}:",
-                    f"- [magenta]Players[/] : {status.players} players",
-                    f"- [magenta]Map[/]     : {repr(status.map)}",
-                    f"- [magenta]Wave[/]    : {status.wave} wave",
-                    f"- [magenta]Ping[/]    : {round(status.ping)} ms",
-                    f"- [magenta]Version[/] : {repr(status.version)}",
-                    f"- [magenta]Vertype[/] : {repr(status.vertype)}"
-                ]
-            )
+    if (server_config:=msmanager.get_server_config(connect)) is not None:
+        connect_data = {"host": server_config.host, "port": server_config.port}
+    else:
+        try:
+            connect_data = parse_connect_data(connect)
+        except VBMLParseError:
+            raise IncorrectConnectionDataError(connect)
+    status = ping(connect_data["host"], connect_data["port"], timeout)
+    console.print(
+        "\n\t".join(
+            [
+                f"[green]>[/] Server {endicext(status.name)}:",
+                f"- [magenta]Players[/] : {status.players} players",
+                f"- [magenta]Map[/]     : {repr(status.map)}",
+                f"- [magenta]Wave[/]    : {status.wave} wave",
+                f"- [magenta]Ping[/]    : {round(status.ping)} ms",
+                f"- [magenta]Version[/] : {repr(status.version)}",
+                f"- [magenta]Vertype[/] : {repr(status.vertype)}"
+            ]
         )
-    except Exception as e:
-        printexcept(e)
+    )
 
 # ! Main Group
 @click.group()
 @click.option(
     "-nce", "--not-check-environment", "not_check_environment",
     help="Disables checks for GNU Screen, Java and system support.",
     is_flag=True
@@ -199,14 +200,15 @@
     help="Enables debug mode of operation.",
     is_flag=True
 )
 @click.version_option(
     version=prog_version,
     prog_name=prog_name
 )
+@hand_exception()
 def main(not_check_environment: bool, debug: bool):
     global msmanager, debag_mode
     
     msmanager = MSManager(check_environment=(not not_check_environment))
     debag_mode = debug
 
 # ! Add in Group
```

### Comparing `msmanager-0.2.2.dev4/msmanager/config.py` & `msmanager-0.2.2.dev5/msmanager/config.py`

 * *Files identical despite different names*

### Comparing `msmanager-0.2.2.dev4/msmanager/exceptions.py` & `msmanager-0.2.2.dev5/msmanager/exceptions.py`

 * *Files identical despite different names*

### Comparing `msmanager-0.2.2.dev4/msmanager/functions.py` & `msmanager-0.2.2.dev5/msmanager/functions.py`

 * *Files identical despite different names*

### Comparing `msmanager-0.2.2.dev4/msmanager/msm.py` & `msmanager-0.2.2.dev5/msmanager/msm.py`

 * *Files identical despite different names*

### Comparing `msmanager-0.2.2.dev4/msmanager/units.py` & `msmanager-0.2.2.dev5/msmanager/units.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 from platformdirs import user_config_dir
 
 # ! Metadata
 __name__ = "msmanager"
 __title__ = "MSManager (Mindustry Servers Manager)"
-__version__ = "0.2.2.dev4"
+__version__ = "0.2.2.dev5"
 __author__ = "RCR"
 __email__ = "semina054@gmail.com"
 __url__ = "https://github.com/RCR-OOP/msmanager"
 
 # ! Constants
 SUPPORT_PLATFORMS = [
     "windows-amd64", "windows-x86_64", "linux-x86_64"
```

### Comparing `msmanager-0.2.2.dev4/pyproject.toml` & `msmanager-0.2.2.dev5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "msmanager"
-version = "0.2.2.dev4"
+version = "0.2.2.dev5"
 description = "Manager for managing Mindustry servers."
 authors = ["Romanin <semina054@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "msmanager"}]
 
 [tool.poetry.dependencies]
```

### Comparing `msmanager-0.2.2.dev4/README.md` & `msmanager-0.2.2.dev5/README.md`

 * *Files identical despite different names*

### Comparing `msmanager-0.2.2.dev4/PKG-INFO` & `msmanager-0.2.2.dev5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: msmanager
-Version: 0.2.2.dev4
+Version: 0.2.2.dev5
 Summary: Manager for managing Mindustry servers.
 License: MIT
 Author: Romanin
 Author-email: semina054@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

