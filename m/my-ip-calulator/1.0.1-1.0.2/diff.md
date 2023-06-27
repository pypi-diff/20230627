# Comparing `tmp/my_ip_calulator-1.0.1.tar.gz` & `tmp/my_ip_calulator-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "my_ip_calulator-1.0.1.tar", max compression
+gzip compressed data, was "my_ip_calulator-1.0.2.tar", max compression
```

## Comparing `my_ip_calulator-1.0.1.tar` & `my_ip_calulator-1.0.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1070 2023-05-31 20:27:54.398428 my_ip_calulator-1.0.1/LICENSE
--rw-r--r--   0        0        0    31699 2023-05-31 20:27:54.399437 my_ip_calulator-1.0.1/README.md
--rw-r--r--   0        0        0     7769 2023-06-26 23:45:55.270762 my_ip_calulator-1.0.1/pyproject.toml
--rw-r--r--   0        0        0       38 2023-05-31 20:27:54.412856 my_ip_calulator-1.0.1/src/app/__init__.py
--rw-r--r--   0        0        0    18576 2023-05-31 20:27:54.413148 my_ip_calulator-1.0.1/src/app/calc.py
--rw-r--r--   0        0        0    11259 2023-06-27 00:01:22.032257 my_ip_calulator-1.0.1/src/app/cmd.py
--rw-r--r--   0        0        0    32605 1970-01-01 00:00:00.000000 my_ip_calulator-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-05-31 20:27:54.398428 my_ip_calulator-1.0.2/LICENSE
+-rw-r--r--   0        0        0    31693 2023-06-27 00:12:20.052695 my_ip_calulator-1.0.2/README.md
+-rw-r--r--   0        0        0     7769 2023-06-27 00:22:05.358113 my_ip_calulator-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0       38 2023-05-31 20:27:54.412856 my_ip_calulator-1.0.2/src/app/__init__.py
+-rw-r--r--   0        0        0    18576 2023-05-31 20:27:54.413148 my_ip_calulator-1.0.2/src/app/calc.py
+-rw-r--r--   0        0        0    11278 2023-06-27 00:21:59.053001 my_ip_calulator-1.0.2/src/app/cmd.py
+-rw-r--r--   0        0        0    32599 1970-01-01 00:00:00.000000 my_ip_calulator-1.0.2/PKG-INFO
```

### Comparing `my_ip_calulator-1.0.1/LICENSE` & `my_ip_calulator-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `my_ip_calulator-1.0.1/README.md` & `my_ip_calulator-1.0.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 ## Install
 You can use this tool in many ways:
 
 ### Install from Repository
 With this command, you PC will download the app from https://pypi.org/project/my-ip-calulator/0.4.0/:
 ````
-pip install my-ip-calculator
+pip install my-ip-calc
 ````
 
 [![asciicast](https://asciinema.org/a/585935.svg)](https://asciinema.org/a/585935)
 
 ### Run in Container
 With this commands:
 ````
```

### Comparing `my_ip_calulator-1.0.1/pyproject.toml` & `my_ip_calulator-1.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "my-ip-calulator"
-version = "1.0.1"
+version = "1.0.2"
 license = "MIT"
 description = "This is an IPv4 and IPv6 calculator. It can validate IP address, convert then and also do net and subnet calculations."
 authors = ["Bruno Botelho <bruno.botelho.br@gmail.com>"]
 maintainers = ["Bruno Botelho <bruno.botelho.br@gmail.com>"]
 readme = "README.md"
 packages = [{include = "app", from = "src"}]
 repository = "https://github.com/brunobotelhobr/My-IP-Calculator"
```

### Comparing `my_ip_calulator-1.0.1/src/app/calc.py` & `my_ip_calulator-1.0.2/src/app/calc.py`

 * *Files identical despite different names*

### Comparing `my_ip_calulator-1.0.1/src/app/cmd.py` & `my_ip_calulator-1.0.2/src/app/cmd.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 cmd = typer.Typer(no_args_is_help=True)
 
 
 @cmd.command()
 def version() -> str:
     """Show version."""
-    app_version: str = "1.0.1"
+    app_version: str = "1.0.2"
     typer.echo(app_version)
     return app_version
 
 
 @cmd.command()
 def val(
     address: Annotated[str, typer.Argument(..., help="IP address, it supports IPv4 and IPv6")],
@@ -92,16 +92,15 @@
     mask: Annotated[
         Optional[str], typer.Argument(help="IP address mask, if not provided an auto generated one will be assigned.")
     ] = None,
 ) -> bool:
     """Calculate the network address from an IP address and a subnet mask, output the address in the desired format."""
     # Split the address and the mask
     if "/" in address:
-        Printer().error(name="address", value=address, message="Address field can not contain a mask")
-        exit()
+        address, mask = address.split("/")
     # Identify the address type
     address_version: int = discover_version(address=address)
     # Return False if the address is invalid
     if address_version not in [4, 6]:
         Printer().error(name="address", value=address, message="Invalid address")
         return False
     # Set default output format
@@ -183,16 +182,20 @@
             case_sensitive=False,
             show_choices=True,
         ),
     ] = None,
 ) -> bool:
     """Split an IP address into network and host parts, output the address in the desired format."""
     if "/" in address:
-        Printer().error(name="address", value=address, message="Address field can not contain a mask")
-        exit()
+        Printer().error(
+            name="address",
+            value=address,
+            message="Address field can not contain a " + "mask, check --help, for more information",
+        )
+        return False
     # Identify the address type
     address_version: int = discover_version(address=address)
     # Return False if the address is invalid
     if address_version not in [4, 6]:
         Printer().error(name="address", value=address, message="Invalid address")
         return False
     # Set default output format
```

### Comparing `my_ip_calulator-1.0.1/PKG-INFO` & `my_ip_calulator-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: my-ip-calulator
-Version: 1.0.1
+Version: 1.0.2
 Summary: This is an IPv4 and IPv6 calculator. It can validate IP address, convert then and also do net and subnet calculations.
 Home-page: https://brunobotelhobr.github.io/My-IP-Calculator
 License: MIT
 Keywords: ip,calculator,ipv4,ipv6,net,subnet,cidr,mask,address,convert,validate
 Author: Bruno Botelho
 Author-email: bruno.botelho.br@gmail.com
 Maintainer: Bruno Botelho
@@ -45,15 +45,15 @@
 
 ## Install
 You can use this tool in many ways:
 
 ### Install from Repository
 With this command, you PC will download the app from https://pypi.org/project/my-ip-calulator/0.4.0/:
 ````
-pip install my-ip-calculator
+pip install my-ip-calc
 ````
 
 [![asciicast](https://asciinema.org/a/585935.svg)](https://asciinema.org/a/585935)
 
 ### Run in Container
 With this commands:
 ````
```

