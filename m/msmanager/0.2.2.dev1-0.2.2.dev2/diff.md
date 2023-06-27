# Comparing `tmp/msmanager-0.2.2.dev1.tar.gz` & `tmp/msmanager-0.2.2.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "msmanager-0.2.2.dev1.tar", max compression
+gzip compressed data, was "msmanager-0.2.2.dev2.tar", max compression
```

## Comparing `msmanager-0.2.2.dev1.tar` & `msmanager-0.2.2.dev2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1111 2023-05-14 16:04:08.180554 msmanager-0.2.2.dev1/LICENSE
--rw-r--r--   0        0        0      267 2023-05-15 20:57:42.797028 msmanager-0.2.2.dev1/msmanager/__init__.py
--rw-r--r--   0        0        0       67 2023-05-15 21:27:48.138274 msmanager-0.2.2.dev1/msmanager/__main__.py
--rw-r--r--   0        0        0     6826 2023-06-26 19:31:40.068583 msmanager-0.2.2.dev1/msmanager/cli.py
--rw-r--r--   0        0        0     2488 2023-05-15 19:04:10.101041 msmanager-0.2.2.dev1/msmanager/config.py
--rw-r--r--   0        0        0     2793 2023-05-15 20:31:27.149266 msmanager-0.2.2.dev1/msmanager/exceptions.py
--rw-r--r--   0        0        0     4002 2023-06-26 19:34:27.030856 msmanager-0.2.2.dev1/msmanager/functions.py
--rw-r--r--   0        0        0      384 2023-05-16 16:36:36.800666 msmanager-0.2.2.dev1/msmanager/models.py
--rw-r--r--   0        0        0     2983 2023-06-13 10:18:25.381658 msmanager-0.2.2.dev1/msmanager/msm.py
--rw-r--r--   0        0        0      143 2023-05-15 19:04:10.113824 msmanager-0.2.2.dev1/msmanager/types.py
--rw-r--r--   0        0        0      591 2023-06-26 19:34:43.467905 msmanager-0.2.2.dev1/msmanager/units.py
--rw-r--r--   0        0        0      552 2023-06-26 19:34:38.000477 msmanager-0.2.2.dev1/pyproject.toml
--rw-r--r--   0        0        0      704 2023-06-21 22:49:16.590585 msmanager-0.2.2.dev1/README.md
--rw-r--r--   0        0        0     1505 1970-01-01 00:00:00.000000 msmanager-0.2.2.dev1/PKG-INFO
+-rw-r--r--   0        0        0     1111 2023-05-14 16:04:08.180554 msmanager-0.2.2.dev2/LICENSE
+-rw-r--r--   0        0        0      267 2023-05-15 20:57:42.797028 msmanager-0.2.2.dev2/msmanager/__init__.py
+-rw-r--r--   0        0        0       67 2023-05-15 21:27:48.138274 msmanager-0.2.2.dev2/msmanager/__main__.py
+-rw-r--r--   0        0        0     7494 2023-06-27 12:06:21.095814 msmanager-0.2.2.dev2/msmanager/cli.py
+-rw-r--r--   0        0        0     2488 2023-05-15 19:04:10.101041 msmanager-0.2.2.dev2/msmanager/config.py
+-rw-r--r--   0        0        0     3231 2023-06-26 19:57:01.709315 msmanager-0.2.2.dev2/msmanager/exceptions.py
+-rw-r--r--   0        0        0     4001 2023-06-26 20:02:25.396576 msmanager-0.2.2.dev2/msmanager/functions.py
+-rw-r--r--   0        0        0      384 2023-05-16 16:36:36.800666 msmanager-0.2.2.dev2/msmanager/models.py
+-rw-r--r--   0        0        0     2983 2023-06-13 10:18:25.381658 msmanager-0.2.2.dev2/msmanager/msm.py
+-rw-r--r--   0        0        0      143 2023-05-15 19:04:10.113824 msmanager-0.2.2.dev2/msmanager/types.py
+-rw-r--r--   0        0        0      591 2023-06-27 12:07:16.435517 msmanager-0.2.2.dev2/msmanager/units.py
+-rw-r--r--   0        0        0      552 2023-06-27 12:07:11.616511 msmanager-0.2.2.dev2/pyproject.toml
+-rw-r--r--   0        0        0      704 2023-06-21 22:49:16.590585 msmanager-0.2.2.dev2/README.md
+-rw-r--r--   0        0        0     1505 1970-01-01 00:00:00.000000 msmanager-0.2.2.dev2/PKG-INFO
```

### Comparing `msmanager-0.2.2.dev1/LICENSE` & `msmanager-0.2.2.dev2/LICENSE`

 * *Files identical despite different names*

### Comparing `msmanager-0.2.2.dev1/msmanager/cli.py` & `msmanager-0.2.2.dev2/msmanager/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,19 +11,30 @@
 from .models import MindustryServerConfig
 from .functions import (
     rich_exception,
     is_server_connect_correct,
     wait_start_server,
     ping, endicext, parse_connect_data
 )
+from .exceptions import (
+    VBMLParseError, IncorrectConnectionDataError
+)
 
 # ! Vars
 console = Console()
+debag_mode = False
 msmanager: MSManager = ...
 
+# ! Functions
+def printexcept(e: Exception):
+    if debag_mode:
+        console.print_exception(word_wrap=True, show_locals=True)
+    else:
+        console.print(rich_exception(e))
+
 # ! Commands
 # ? Add Command
 @click.command("add", help="Add a server to the config.")
 @click.argument("screen_name", type=str)
 @click.argument("executable_filepath", type=click.Path(exists=True))
 @click.option(
     "-a", "--arg", "arguments",
@@ -62,25 +73,25 @@
                 executable_filepath=os.path.abspath(executable_filepath),
                 arguments=list(arguments),
                 host=host, port=port, input_port=input_port
             )
         )
         console.print("[green]>[/] Server [bold yellow]added[/]!")
     except Exception as e:
-        console.print(rich_exception(e))
+        printexcept(e)
 
 # ? Remove Command
 @click.command("remove", help="Remove the server from the config.")
 @click.argument("screen_name", type=str)
 def remover(screen_name: str):
     try:
         msmanager.remove_server_config(screen_name)
         console.print("[green]>[/] Server [bold yellow]removed[/]!")
     except Exception as e:
-        console.print(rich_exception(e))
+        printexcept(e)
 
 # ? Start Command
 @click.command("start", help="Run the server.")
 @click.argument("screen_name", type=str)
 @click.option(
     "-w", "--wait", "wait",
     help="Waiting for the server to start up.",
@@ -90,25 +101,25 @@
     try:
         msmanager.start_server(screen_name)
         if (server_config:=msmanager.get_server_config(screen_name)) is not None:
             if is_server_connect_correct(server_config.host, server_config.port, server_config.input_port) and wait:
                 wait_start_server(server_config.host, server_config.port, server_config.input_port)
         console.print("[green]>[/] Server [bold yellow]started[/]!")
     except Exception as e:
-        console.print(rich_exception(e))
+        printexcept(e)
 
 # ? Stop Command
 @click.command("stop", help="Stop the server.")
 @click.argument("screen_name", type=str)
 def stoper(screen_name: str):
     try:
         msmanager.stop_server(screen_name)
         console.print("[green]>[/] Server [bold yellow]stoped[/]!")
     except Exception as e:
-        console.print(rich_exception(e))
+        printexcept(e)
 
 # ? List Command
 @click.command("list", help="List of servers in the config.")
 @click.option(
     "--pinging", "pinging",
     help="Whether to do a ping to check.",
     is_flag=True, default=False
@@ -148,46 +159,59 @@
 @click.option(
     "-t", "--timeout", "timeout",
     help="Maximum response waiting time (in seconds).",
     type=int, default=10, show_default=True
 )
 def pinger(connect: str, timeout: int):
     try:
-        connect_data = parse_connect_data(connect)
+        try:
+            connect_data = parse_connect_data(connect)
+        except VBMLParseError:
+            if (server_config:=msmanager.get_server_config(connect)) is not None:
+                connect_data = {"host": server_config.host, "port": server_config.port}
+            else:
+                raise IncorrectConnectionDataError(connect)
         status = ping(connect_data["host"], connect_data["port"], timeout)
         console.print(
             "\n\t".join(
                 [
-                    f"[green]>[/] Server '{endicext(status.name)}':",
+                    f"[green]>[/] Server {endicext(status.name)}:",
                     f"- [magenta]Players[/] : {status.players} players",
                     f"- [magenta]Map[/]     : {repr(status.map)}",
                     f"- [magenta]Wave[/]    : {status.wave} wave",
                     f"- [magenta]Ping[/]    : {round(status.ping)} ms",
                     f"- [magenta]Version[/] : {repr(status.version)}",
                     f"- [magenta]Vertype[/] : {repr(status.vertype)}"
                 ]
             )
         )
     except Exception as e:
-        console.print(rich_exception(e))
+        printexcept(e)
 
 # ! Main Group
 @click.group()
 @click.option(
     "-nce", "--not-check-environment", "not_check_environment",
-    is_flag=True,
-    help="Disables checks for GNU Screen, Java and system support."
+    help="Disables checks for GNU Screen, Java and system support.",
+    is_flag=True
+)
+@click.option(
+    "--debug", "-d", "debug",
+    help="Enables debug mode of operation.",
+    is_flag=True
 )
 @click.version_option(
     version=prog_version,
     prog_name=prog_name
 )
-def main(not_check_environment: bool):
-    global msmanager
+def main(not_check_environment: bool, debug: bool):
+    global msmanager, debag_mode
+    
     msmanager = MSManager(check_environment=(not not_check_environment))
+    debag_mode = debug
 
 # ! Add in Group
 main.add_command(adder)
 main.add_command(remover)
 main.add_command(starter)
 main.add_command(stoper)
 main.add_command(lister)
```

### Comparing `msmanager-0.2.2.dev1/msmanager/config.py` & `msmanager-0.2.2.dev2/msmanager/config.py`

 * *Files identical despite different names*

### Comparing `msmanager-0.2.2.dev1/msmanager/exceptions.py` & `msmanager-0.2.2.dev2/msmanager/exceptions.py`

 * *Files 6% similar despite different names*

```diff
@@ -54,13 +54,22 @@
     def __init__(self, name: str) -> None:
         """Called when attempting to start an already running server."""
         self.args = (
             f"A server named {repr(name)} is already up and running."
         )
 
 class ServerIsStoppedError(Exception):
-    """..."""
+    """Indicates that the server is already stopped."""
     def __init__(self, name: str) -> None:
-        """..."""
+        """Called if the server is already stopped."""
         self.args = (
             f"The {repr(name)} server is stopped as it is."
+        )
+
+# ! CLI Exception
+class IncorrectConnectionDataError(Exception):
+    """Indicates incorrect data to connect to the server."""
+    def __init__(self, connect_data: str) -> None:
+        """Called if the connection data is incorrect."""
+        self.args = (
+            f"The data to connect to the server is not correct ({connect_data})."
         )
```

### Comparing `msmanager-0.2.2.dev1/msmanager/functions.py` & `msmanager-0.2.2.dev2/msmanager/functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,15 +51,16 @@
     return pydustry.Server(host, port).get_status(timeout)
 
 # ! Subproccess Functions
 def runner(*args: str) -> Tuple[int, str]:
     return getstatusoutput(" ".join([*args]))
 
 def exists_screen() -> bool:
-    return (runner("screen", "-v")[0] == 0) or (runner("screen", "-v")[0] == 1)
+    out = runner("screen", "-v")[0]
+    return (out[0] == 0) or (out[0] == 1)
 
 def exists_java() -> bool:
     return runner("java", "--version")[0] == 0
 
 # ! Parse Functions
 def remove_color(text: str) -> str:
     return replaces(text, COLORS_STRINGS_REPLACEBLE)
```

### Comparing `msmanager-0.2.2.dev1/msmanager/msm.py` & `msmanager-0.2.2.dev2/msmanager/msm.py`

 * *Files identical despite different names*

### Comparing `msmanager-0.2.2.dev1/msmanager/units.py` & `msmanager-0.2.2.dev2/msmanager/units.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 from platformdirs import user_config_dir
 
 # ! Metadata
 __name__ = "msmanager"
 __title__ = "MSManager (Mindustry Servers Manager)"
-__version__ = "0.2.2.dev1"
+__version__ = "0.2.2.dev2"
 __author__ = "RCR"
 __email__ = "semina054@gmail.com"
 __url__ = "https://github.com/RCR-OOP/msmanager"
 
 # ! Constants
 SUPPORT_PLATFORMS = [
     "windows-amd64", "windows-x86_64", "linux-x86_64"
```

### Comparing `msmanager-0.2.2.dev1/pyproject.toml` & `msmanager-0.2.2.dev2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "msmanager"
-version = "0.2.2.dev1"
+version = "0.2.2.dev2"
 description = "Manager for managing Mindustry servers."
 authors = ["Romanin <semina054@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "msmanager"}]
 
 [tool.poetry.dependencies]
```

### Comparing `msmanager-0.2.2.dev1/README.md` & `msmanager-0.2.2.dev2/README.md`

 * *Files identical despite different names*

### Comparing `msmanager-0.2.2.dev1/PKG-INFO` & `msmanager-0.2.2.dev2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: msmanager
-Version: 0.2.2.dev1
+Version: 0.2.2.dev2
 Summary: Manager for managing Mindustry servers.
 License: MIT
 Author: Romanin
 Author-email: semina054@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

