# Comparing `tmp/kraken_wrapper-0.26.1.tar.gz` & `tmp/kraken_wrapper-0.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kraken_wrapper-0.26.1.tar", max compression
+gzip compressed data, was "kraken_wrapper-0.27.0.tar", max compression
```

## Comparing `kraken_wrapper-0.26.1.tar` & `kraken_wrapper-0.27.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0      988 2023-05-15 12:38:11.992918 kraken_wrapper-0.26.1/LICENSE
--rw-r--r--   0        0        0      378 2023-06-19 22:14:09.973885 kraken_wrapper-0.26.1/README.md
--rw-r--r--   0        0        0     2174 2023-06-20 14:42:33.722681 kraken_wrapper-0.26.1/pyproject.toml
--rw-r--r--   0        0        0      134 2023-06-20 14:42:33.726681 kraken_wrapper-0.26.1/src/kraken/wrapper/__init__.py
--rw-r--r--   0        0        0     7660 2023-06-19 22:14:09.973885 kraken_wrapper-0.26.1/src/kraken/wrapper/_buildend_venv.py
--rw-r--r--   0        0        0     3478 2023-06-19 22:14:09.973885 kraken_wrapper-0.26.1/src/kraken/wrapper/_buildenv.py
--rw-r--r--   0        0        0     5311 2023-05-15 12:38:11.992918 kraken_wrapper-0.26.1/src/kraken/wrapper/_buildenv_manager.py
--rw-r--r--   0        0        0     3674 2023-05-15 12:38:11.992918 kraken_wrapper-0.26.1/src/kraken/wrapper/_buildenv_pex.py
--rw-r--r--   0        0        0     3250 2023-06-19 15:38:25.250142 kraken_wrapper-0.26.1/src/kraken/wrapper/_config.py
--rw-r--r--   0        0        0     4605 2023-05-15 12:38:11.992918 kraken_wrapper-0.26.1/src/kraken/wrapper/_lockfile.py
--rw-r--r--   0        0        0     3564 2023-05-15 12:38:11.992918 kraken_wrapper-0.26.1/src/kraken/wrapper/_option_sets.py
--rw-r--r--   0        0        0     4222 2023-05-15 12:38:11.992918 kraken_wrapper-0.26.1/src/kraken/wrapper/_pex.py
--rw-r--r--   0        0        0    15814 2023-06-19 22:14:09.973885 kraken_wrapper-0.26.1/src/kraken/wrapper/main.py
--rw-r--r--   0        0        0        0 2023-05-15 12:38:11.992918 kraken_wrapper-0.26.1/src/kraken/wrapper/py.typed
--rw-r--r--   0        0        0     1451 1970-01-01 00:00:00.000000 kraken_wrapper-0.26.1/PKG-INFO
+-rw-r--r--   0        0        0      998 2023-06-26 11:46:09.748133 kraken_wrapper-0.27.0/LICENSE
+-rw-r--r--   0        0        0      378 2023-06-26 11:13:42.662140 kraken_wrapper-0.27.0/README.md
+-rw-r--r--   0        0        0     2196 2023-06-27 00:25:10.711064 kraken_wrapper-0.27.0/pyproject.toml
+-rw-r--r--   0        0        0      134 2023-06-27 00:25:10.711236 kraken_wrapper-0.27.0/src/kraken/wrapper/__init__.py
+-rw-r--r--   0        0        0     7660 2023-06-26 11:13:42.663936 kraken_wrapper-0.27.0/src/kraken/wrapper/_buildend_venv.py
+-rw-r--r--   0        0        0     3478 2023-06-26 11:13:42.664260 kraken_wrapper-0.27.0/src/kraken/wrapper/_buildenv.py
+-rw-r--r--   0        0        0     5311 2023-06-20 12:31:06.105651 kraken_wrapper-0.27.0/src/kraken/wrapper/_buildenv_manager.py
+-rw-r--r--   0        0        0     3674 2023-06-20 12:31:06.105769 kraken_wrapper-0.27.0/src/kraken/wrapper/_buildenv_pex.py
+-rw-r--r--   0        0        0     3250 2023-06-26 11:13:42.664763 kraken_wrapper-0.27.0/src/kraken/wrapper/_config.py
+-rw-r--r--   0        0        0     4605 2023-06-20 12:31:06.106048 kraken_wrapper-0.27.0/src/kraken/wrapper/_lockfile.py
+-rw-r--r--   0        0        0     3564 2023-06-20 12:31:06.106187 kraken_wrapper-0.27.0/src/kraken/wrapper/_option_sets.py
+-rw-r--r--   0        0        0     4222 2023-06-20 12:31:06.106313 kraken_wrapper-0.27.0/src/kraken/wrapper/_pex.py
+-rw-r--r--   0        0        0    15982 2023-06-27 00:17:45.123581 kraken_wrapper-0.27.0/src/kraken/wrapper/main.py
+-rw-r--r--   0        0        0        0 2023-06-20 12:31:06.106556 kraken_wrapper-0.27.0/src/kraken/wrapper/py.typed
+-rw-r--r--   0        0        0     1473 1970-01-01 00:00:00.000000 kraken_wrapper-0.27.0/PKG-INFO
```

### Comparing `kraken_wrapper-0.26.1/LICENSE` & `kraken_wrapper-0.27.0/LICENSE`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2022 Unknown
+Copyright (c) 2022 Niklas Rosenstein
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 this software and associated documentation files (the "Software"), to deal in
 Software without restriction, including without limitation the rights to use,
 modify, merge, publish, distribute, sublicense, and/or sell copies of the
 and to permit persons to whom the Software is furnished to do so, subject to
 following conditions:
```

### Comparing `kraken_wrapper-0.26.1/pyproject.toml` & `kraken_wrapper-0.27.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "kraken-wrapper"
-version = "0.26.1"
+version = "0.27.0"
 description = ""
-authors = ["Unknown <me@unknown.org>"]
+authors = ["Niklas Rosenstein <rosensteinniklas@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "kraken/wrapper", from = "src" }]
 classifiers = []
 keywords = []
 
 [tool.poetry.urls]
@@ -18,15 +18,15 @@
 Documentation = "https://kraken-build.github.io/kraken-build/"
 Homepage = "https://kraken-build.github.io/kraken-build/"
 Repository = "https://github.com/kraken-build/kraken-build/"
 
 [tool.poetry.dependencies]
 python = ">=3.7,<3.11"
 keyring = "^23.8.2"
-kraken-common = "^0.26.1"
+kraken-common = "^0.27.0"
 pex = "^2.1.103"
 setuptools = ">=33.0.0"  # For pkg_resources
 termcolor = "^1.1.0"
 rich = "^13.4.2"
 
 # NOTE(@NiklasRosenstein): Need to pin transitive dependency markdown-it under 3.0 because it dropped Python 3.9
 #       support after that version. Technically this shouldn't be a big issue for runtime, but Mypy checks site
```

### Comparing `kraken_wrapper-0.26.1/src/kraken/wrapper/_buildend_venv.py` & `kraken_wrapper-0.27.0/src/kraken/wrapper/_buildend_venv.py`

 * *Files identical despite different names*

### Comparing `kraken_wrapper-0.26.1/src/kraken/wrapper/_buildenv.py` & `kraken_wrapper-0.27.0/src/kraken/wrapper/_buildenv.py`

 * *Files identical despite different names*

### Comparing `kraken_wrapper-0.26.1/src/kraken/wrapper/_buildenv_manager.py` & `kraken_wrapper-0.27.0/src/kraken/wrapper/_buildenv_manager.py`

 * *Files identical despite different names*

### Comparing `kraken_wrapper-0.26.1/src/kraken/wrapper/_buildenv_pex.py` & `kraken_wrapper-0.27.0/src/kraken/wrapper/_buildenv_pex.py`

 * *Files identical despite different names*

### Comparing `kraken_wrapper-0.26.1/src/kraken/wrapper/_config.py` & `kraken_wrapper-0.27.0/src/kraken/wrapper/_config.py`

 * *Files identical despite different names*

### Comparing `kraken_wrapper-0.26.1/src/kraken/wrapper/_lockfile.py` & `kraken_wrapper-0.27.0/src/kraken/wrapper/_lockfile.py`

 * *Files identical despite different names*

### Comparing `kraken_wrapper-0.26.1/src/kraken/wrapper/_option_sets.py` & `kraken_wrapper-0.27.0/src/kraken/wrapper/_option_sets.py`

 * *Files identical despite different names*

### Comparing `kraken_wrapper-0.26.1/src/kraken/wrapper/_pex.py` & `kraken_wrapper-0.27.0/src/kraken/wrapper/_pex.py`

 * *Files identical despite different names*

### Comparing `kraken_wrapper-0.26.1/src/kraken/wrapper/main.py` & `kraken_wrapper-0.27.0/src/kraken/wrapper/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,15 +61,15 @@
                 "This is kraken-wrapper's help. To show kraken's help instead, run krakenw -- --help",
                 "yellow",
                 attrs=["bold"],
             )
         ),
     )
     parser.add_argument("-V", "--version", version=__version__, action="version")
-    LoggingOptions.add_to_parser(parser)
+    LoggingOptions.add_to_parser(parser, default_verbosity=1)
     EnvOptions.add_to_parser(parser)
 
     # NOTE (@NiklasRosenstein): If we combine "+" with remainder, we get options passed after the `cmd`
     #       passed directly into `args` without argparse treating it like an option. This is not the case
     #       when using `nargs=1` for `cmd`.
     parser.add_argument("cmd", nargs="*", metavar="cmd", help="{auth,list-pythons,lock} or a kraken command")
     parser.add_argument("args", nargs=argparse.REMAINDER, help="additional arguments")
@@ -362,14 +362,17 @@
     logging_options.init_logging()
     env_options = EnvOptions.collect(args)
 
     if not args.cmd and not env_options.any():
         parser.print_usage()
         sys.exit(0)
 
+    # When we delegate to the Kraken CLI, we want to make sure it can detect that it has been invoked from the wrapper.
+    os.environ["KRAKENW"] = "1"
+
     # Convert the arguments we defined in the argument parser to the actual subcommand that we want
     # delegated.
     cmd: str | None = args.cmd[0] if args.cmd else None
     argv: list[str] = args.cmd[1:] + args.args
 
     if cmd in ("a", "auth"):
         # The `auth` comand does not require any current project information, it can be used globally.
@@ -415,15 +418,15 @@
         sys.exit(0)
 
     elif cmd in ("l", "lock"):
         lock(f"{parser.prog} lock", argv, manager, project)
 
     else:
         if project.directory.absolute() != Path.cwd():
-            argv = ["-p", str(project.directory)] + argv
+            argv += ["-p", str(project.directory)]
         command = [cmd, *argv]
         logger.info("$ %s", " ".join(map(shlex.quote, ["kraken"] + command)))
         environment = manager.get_environment()
         environment.dispatch_to_kraken_cli(command)
 
 
 if __name__ == "__main__":
```

### Comparing `kraken_wrapper-0.26.1/PKG-INFO` & `kraken_wrapper-0.27.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: kraken-wrapper
-Version: 0.26.1
+Version: 0.27.0
 Summary: 
 License: MIT
-Author: Unknown
-Author-email: me@unknown.org
+Author: Niklas Rosenstein
+Author-email: rosensteinniklas@gmail.com
 Requires-Python: >=3.7,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: keyring (>=23.8.2,<24.0.0)
-Requires-Dist: kraken-common (>=0.26.1,<0.27.0)
+Requires-Dist: kraken-common (>=0.27.0,<0.28.0)
 Requires-Dist: markdown-it-py (<3.0.0)
 Requires-Dist: pex (>=2.1.103,<3.0.0)
 Requires-Dist: rich (>=13.4.2,<14.0.0)
 Requires-Dist: setuptools (>=33.0.0)
 Requires-Dist: termcolor (>=1.1.0,<2.0.0)
 Project-URL: Bug Tracker, https://github.com/kraken-build/kraken-build/issues
 Project-URL: Documentation, https://kraken-build.github.io/kraken-build/
```

