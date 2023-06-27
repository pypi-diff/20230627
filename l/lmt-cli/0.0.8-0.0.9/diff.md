# Comparing `tmp/lmt-cli-0.0.8.tar.gz` & `tmp/lmt-cli-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lmt-cli-0.0.8.tar", last modified: Sat Jun 24 01:57:07 2023, max compression
+gzip compressed data, was "lmt-cli-0.0.9.tar", last modified: Tue Jun 27 00:42:41 2023, max compression
```

## Comparing `lmt-cli-0.0.8.tar` & `lmt-cli-0.0.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-06-24 01:57:07.796952 lmt-cli-0.0.8/
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)    11357 2023-06-18 17:13:45.000000 lmt-cli-0.0.8/LICENSE
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)     9059 2023-06-24 01:57:07.796952 lmt-cli-0.0.8/PKG-INFO
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)     8416 2023-06-24 00:13:18.000000 lmt-cli-0.0.8/README.md
-drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-06-24 01:57:07.796952 lmt-cli-0.0.8/lmt_cli/
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)        0 2023-06-18 20:39:32.000000 lmt-cli-0.0.8/lmt_cli/__init__.py
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)     7666 2023-06-23 19:35:04.000000 lmt-cli-0.0.8/lmt_cli/cli.py
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)     4828 2023-06-22 23:46:33.000000 lmt-cli-0.0.8/lmt_cli/gpt_integration.py
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)     9216 2023-06-24 01:55:28.000000 lmt-cli-0.0.8/lmt_cli/lib.py
-drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-06-24 01:57:07.796952 lmt-cli-0.0.8/lmt_cli.egg-info/
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)     9059 2023-06-24 01:57:07.000000 lmt-cli-0.0.8/lmt_cli.egg-info/PKG-INFO
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      291 2023-06-24 01:57:07.000000 lmt-cli-0.0.8/lmt_cli.egg-info/SOURCES.txt
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)        1 2023-06-24 01:57:07.000000 lmt-cli-0.0.8/lmt_cli.egg-info/dependency_links.txt
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)       40 2023-06-24 01:57:07.000000 lmt-cli-0.0.8/lmt_cli.egg-info/entry_points.txt
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)       34 2023-06-24 01:57:07.000000 lmt-cli-0.0.8/lmt_cli.egg-info/requires.txt
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)        8 2023-06-24 01:57:07.000000 lmt-cli-0.0.8/lmt_cli.egg-info/top_level.txt
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)       38 2023-06-24 01:57:07.796952 lmt-cli-0.0.8/setup.cfg
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)     1174 2023-06-24 01:55:39.000000 lmt-cli-0.0.8/setup.py
+drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-06-27 00:42:41.710826 lmt-cli-0.0.9/
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)    11357 2023-06-18 17:13:45.000000 lmt-cli-0.0.9/LICENSE
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)     9059 2023-06-27 00:42:41.710826 lmt-cli-0.0.9/PKG-INFO
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)     8416 2023-06-24 00:13:18.000000 lmt-cli-0.0.9/README.md
+drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-06-27 00:42:41.700826 lmt-cli-0.0.9/lmt_cli/
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)        0 2023-06-18 20:39:32.000000 lmt-cli-0.0.9/lmt_cli/__init__.py
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)     7669 2023-06-24 03:27:10.000000 lmt-cli-0.0.9/lmt_cli/cli.py
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)     4828 2023-06-22 23:46:33.000000 lmt-cli-0.0.9/lmt_cli/gpt_integration.py
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)     9242 2023-06-27 00:40:24.000000 lmt-cli-0.0.9/lmt_cli/lib.py
+drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-06-27 00:42:41.710826 lmt-cli-0.0.9/lmt_cli.egg-info/
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)     9059 2023-06-27 00:42:41.000000 lmt-cli-0.0.9/lmt_cli.egg-info/PKG-INFO
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      291 2023-06-27 00:42:41.000000 lmt-cli-0.0.9/lmt_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)        1 2023-06-27 00:42:41.000000 lmt-cli-0.0.9/lmt_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)       40 2023-06-27 00:42:41.000000 lmt-cli-0.0.9/lmt_cli.egg-info/entry_points.txt
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)       34 2023-06-27 00:42:41.000000 lmt-cli-0.0.9/lmt_cli.egg-info/requires.txt
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)        8 2023-06-27 00:42:41.000000 lmt-cli-0.0.9/lmt_cli.egg-info/top_level.txt
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)       38 2023-06-27 00:42:41.710826 lmt-cli-0.0.9/setup.cfg
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)     1174 2023-06-27 00:42:03.000000 lmt-cli-0.0.9/setup.py
```

### Comparing `lmt-cli-0.0.8/LICENSE` & `lmt-cli-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `lmt-cli-0.0.8/PKG-INFO` & `lmt-cli-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lmt-cli
-Version: 0.0.8
+Version: 0.0.9
 Summary: The main CLI tool within the LLM-Toolbox, designed to enable seamless communication with ChatGPT from your terminal. You can customize your experience by creating templates and using them to generate messages.
 Home-page: https://github.com/sderev/lmt
 Author: Sébastien De Revière
 License: Apache Licence, Version 2.0
 Project-URL: Documentation, https://github.com/sderev/lmt
 Project-URL: Issues, http://github.com/sderev/lmt/issues
 Project-URL: Changelog, https://github.com/sderev/lmt/releases
```

### Comparing `lmt-cli-0.0.8/README.md` & `lmt-cli-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `lmt-cli-0.0.8/lmt_cli/cli.py` & `lmt-cli-0.0.9/lmt_cli/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -135,15 +135,15 @@
         elif not sys.stdin.isatty():
             prompt_input = sys.stdin.read()
         elif sys.stdin.isatty():
             click.echo(
                 click.style(
                     (
                         "You can paste your prompt below. Press <Enter> to"
-                        " validate.\nOnce you've done, press Ctrl+D to send it."
+                        " skip a line.\nOnce you've done, press Ctrl+D to send it."
                     ),
                     fg="yellow",
                 )
                 + "\n---"
             )
             prompt_input = sys.stdin.read()
             click.echo()
```

### Comparing `lmt-cli-0.0.8/lmt_cli/gpt_integration.py` & `lmt-cli-0.0.9/lmt_cli/gpt_integration.py`

 * *Files identical despite different names*

### Comparing `lmt-cli-0.0.8/lmt_cli/lib.py` & `lmt-cli-0.0.9/lmt_cli/lib.py`

 * *Files 0% similar despite different names*

```diff
@@ -125,15 +125,15 @@
     """
     markdown_stream = ""
     with Live(Markdown(markdown_stream), refresh_per_second=25) as live:
 
         def update_markdown_stream(chunk: str) -> None:
             nonlocal markdown_stream
             markdown_stream += chunk
-            if raw:
+            if raw or not sys.stdout.isatty():
                 print("".join(chunk), end="")
             else:
                 rich_markdown_stream = Markdown(markdown_stream)
                 live.update(rich_markdown_stream)
 
         try:
             content, response_time, response = openai_utils.chatgpt_request(
@@ -153,15 +153,14 @@
         except Exception as error:
             print(f"{RED}Error: {error}{RESET}")
 
         else:
             return content, response_time, response
 
 
-
 def get_template_content(template):
     """
     Reads the template YAML file and returns a dictionary with its content.
     """
     template_file = TEMPLATES_DIR / f"{template}.yaml"
 
     try:
```

### Comparing `lmt-cli-0.0.8/lmt_cli.egg-info/PKG-INFO` & `lmt-cli-0.0.9/lmt_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lmt-cli
-Version: 0.0.8
+Version: 0.0.9
 Summary: The main CLI tool within the LLM-Toolbox, designed to enable seamless communication with ChatGPT from your terminal. You can customize your experience by creating templates and using them to generate messages.
 Home-page: https://github.com/sderev/lmt
 Author: Sébastien De Revière
 License: Apache Licence, Version 2.0
 Project-URL: Documentation, https://github.com/sderev/lmt
 Project-URL: Issues, http://github.com/sderev/lmt/issues
 Project-URL: Changelog, https://github.com/sderev/lmt/releases
```

### Comparing `lmt-cli-0.0.8/setup.py` & `lmt-cli-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 
 
-VERSION = "0.0.8"
+VERSION = "0.0.9"
 
 
 def read_requirements():
     with open("requirements.txt") as file:
         return list(file)
```

