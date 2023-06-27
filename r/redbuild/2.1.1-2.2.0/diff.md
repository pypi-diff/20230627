# Comparing `tmp/redbuild-2.1.1.tar.gz` & `tmp/redbuild-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redbuild-2.1.1.tar", max compression
+gzip compressed data, was "redbuild-2.2.0.tar", max compression
```

## Comparing `redbuild-2.1.1.tar` & `redbuild-2.2.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1066 2023-04-15 16:57:41.337879 redbuild-2.1.1/LICENSE
--rw-r--r--   0        0        0     2475 2023-04-17 07:13:34.753986 redbuild-2.1.1/README.md
--rw-r--r--   0        0        0      604 2023-05-14 19:29:53.086874 redbuild-2.1.1/pyproject.toml
--rw-r--r--   0        0        0      162 2023-04-17 00:47:12.554903 redbuild-2.1.1/redbuild/__init__.py
--rw-r--r--   0        0        0       60 2023-04-07 18:52:09.664386 redbuild-2.1.1/redbuild/__main__.py
--rw-r--r--   0        0        0    11456 2023-05-14 19:30:28.813537 redbuild-2.1.1/redbuild/cli.py
--rw-r--r--   0        0        0     1445 2023-04-17 01:41:29.902707 redbuild-2.1.1/redbuild/composer.py
--rw-r--r--   0        0        0      856 2023-05-05 00:02:51.112733 redbuild-2.1.1/redbuild/engine.py
--rw-r--r--   0        0        0      366 2023-04-17 01:15:37.329254 redbuild-2.1.1/redbuild/res.py
--rw-r--r--   0        0        0      836 2023-04-17 00:40:30.278667 redbuild-2.1.1/redbuild/util.py
--rw-r--r--   0        0        0     3208 1970-01-01 00:00:00.000000 redbuild-2.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-04-15 16:57:41.337879 redbuild-2.2.0/LICENSE
+-rw-r--r--   0        0        0     2480 2023-06-24 18:42:33.826672 redbuild-2.2.0/README.md
+-rw-r--r--   0        0        0      604 2023-06-27 01:37:14.190588 redbuild-2.2.0/pyproject.toml
+-rw-r--r--   0        0        0      162 2023-04-17 00:47:12.554903 redbuild-2.2.0/redbuild/__init__.py
+-rw-r--r--   0        0        0       60 2023-04-07 18:52:09.664386 redbuild-2.2.0/redbuild/__main__.py
+-rw-r--r--   0        0        0    12301 2023-06-27 01:37:14.190588 redbuild-2.2.0/redbuild/cli.py
+-rw-r--r--   0        0        0     1445 2023-04-17 01:41:29.902707 redbuild-2.2.0/redbuild/composer.py
+-rw-r--r--   0        0        0      856 2023-05-05 00:02:51.112733 redbuild-2.2.0/redbuild/engine.py
+-rw-r--r--   0        0        0      366 2023-04-17 01:15:37.329254 redbuild-2.2.0/redbuild/res.py
+-rw-r--r--   0        0        0      836 2023-04-17 00:40:30.278667 redbuild-2.2.0/redbuild/util.py
+-rw-r--r--   0        0        0     3213 1970-01-01 00:00:00.000000 redbuild-2.2.0/PKG-INFO
```

### Comparing `redbuild-2.1.1/LICENSE` & `redbuild-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `redbuild-2.1.1/README.md` & `redbuild-2.2.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 # redbuild
 
 magic containerized builds
 
 ## overview
 
-redbuild is a super simple drop-in script enabling software to be built in pre-defined containers. with `podman` installed, any supported project can be built with a single command. projects provide a `build.docker` and `build.sh` for defining the build environment and build steps.
+redbuild enables software to be built in pre-defined environments using the power of containerization. with `podman` installed, any supported project can be built with a single command. projects provide a `build.docker` and `build.sh` for defining the build environment and build steps.
 
 `redbuild`: just add water!
 
 ## install stable version from pypi
 
 ```sh
 # with pipx (recommended)
@@ -78,8 +78,8 @@
     `build.sh`:
 
     ```sh
     #!/bin/bash
     dub build --compiler ldc2 -B release
     ```
 
-that's it! now you can build the project with `redbuild build`, copy it into the project root, and run it. you can also open an interactive shell in the build environment with `redbuild shell`.
+that's it! now you can build the project with `redbuild build`, copy it into the project root, and run it. you can also open an interactive shell in the build environment with `redbuild shell`.
```

### Comparing `redbuild-2.1.1/pyproject.toml` & `redbuild-2.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "redbuild"
-version = "2.1.1"
+version = "2.2.0"
 description = "magic containerized builds"
 authors = ["redthing1 <redthing1@alt.icu>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<4.0"
 typer = {extras = ["rich"], version = "^0.7.0"}
```

### Comparing `redbuild-2.1.1/redbuild/cli.py` & `redbuild-2.2.0/redbuild/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,16 +31,30 @@
     no_args_is_help=True,
     context_settings=CONTEXT_SETTINGS,
 )
 
 DEFAULT_DOCKERFILE = (
     "build.docker"  # filename of default dockerfile for build environment
 )
-VOLUME_OPTS = ":z"  # bind mount volume options
 
+# VOLUME_OPTS = ":z"  # bind mount volume options
+# detect volume options based on OS
+if sys.platform == "linux":
+    # selinux may be present
+    VOLUME_OPTS = ":z"
+elif sys.platform == "darwin":
+    # macos
+    VOLUME_OPTS = ""
+elif sys.platform == "win32":
+    # windows
+    VOLUME_OPTS = ""
+else:
+    # unknown
+    logger.warning(f"Unknown platform [{sys.platform}], assuming no volume options")
+    VOLUME_OPTS = ""
 
 @app.command()
 def info():
     app_info_logo = f"{APP_NAME} v{__version__}"
     print(app_info_logo)
     print("- " * (len(app_info_logo) // 2 + 1))
 
@@ -162,14 +176,15 @@
             f"Build script [{buildscript_path}] not found. Create it or pass a specific path with -s."
         )
         raise typer.Exit(1)
     # $CONTAINER_ENGINE run --rm -it -v $(pwd):/prj $CRUN_ARGS $BUILDER_TAG /bin/bash -l -c "cd /prj && $BUILDSCRIPT $ARGS" | sed 's/^/  /'
     print(
         f"Running build in [{builder_image_name}] with buildscript [{buildscript}] in context [{cwd}]:"
     )
+    cwd_absolute = os.path.abspath(cwd)
 
     cache_volume_mount_args = []
     for cache_mount in cache_mounts:
         cache_mount_source, cache_mount_target = cache_mount.split(":")
         # cache_volume_mount_args.extend(["-v", f"{cache_mount}"])
         # create source directory if it doesn't exist
         os.makedirs(cache_mount_source, exist_ok=True)
@@ -180,37 +195,40 @@
     run_cmd_args = [
         "run",
         # podman run args
         "--rm",
         # "-it",
         # mount project directory
         "-v",
-        f"{cwd}:/prj{VOLUME_OPTS}",
+        f"{cwd_absolute}:/prj{VOLUME_OPTS}",
         *cache_volume_mount_args,
         *parse_secondary_args(crun_args),
     ]
     run_cmd = ctr_engine.bake(
         *run_cmd_args,
         # _fg=True,
         # output formatting
         _out=lambda line: print(f"  {line}", end=""),
         _err=lambda line: print(f"  {line}", end=""),
     )
 
-    relative_buildscript = f"./{buildscript}"
-    logger.debug(f"Running command: {run_cmd}")
+    relative_buildscript = os.path.join(".", buildscript)
+    # logger.debug(f"Running command: {run_cmd}")
 
+    bash_command = f"cd /prj && {relative_buildscript} {build_args}"
     try:
-        run_proc = run_cmd(
+        run_cmd = run_cmd.bake(
             builder_image_name,
             "/bin/bash",
             "-l",
             "-c",
-            f"cd /prj && {relative_buildscript} {build_args}",
+            bash_command,
         )
+        logger.debug(f"Running command: {run_cmd}")
+        run_proc = run_cmd()
     except sh.ErrorReturnCode as e:
         print(f"Build failed with error code {e.exit_code}")
         raise typer.Exit(1)
 
 
 @app.command(help="Run a shell in the build environment")
 def shell(
@@ -225,14 +243,20 @@
     ),
     crun_args=typer.Option(
         "",
         "--crun-args",
         "-R",
         help="Additional arguments to pass to container engine",
     ),
+    login_shell: str = typer.Option(
+        "/bin/bash",
+        "--login-shell",
+        "-s",
+        help="Login shell to use in the container",
+    ),
     shell_args=typer.Option(
         "",
         "--shell-args",
         "-A",
         help="Additional arguments to pass to shell",
     ),
 ):
@@ -243,37 +267,40 @@
     builder_image_name = get_builder_image_name(cwd)
 
     # 2. build builder image
     image(dockerfile=dockerfile, cwd=cwd)
 
     # 3. run an interactive shell with the build environment
     print(f"Running interactive shell in [{builder_image_name}] in context [{cwd}]:")
+    cwd_absolute = os.path.abspath(cwd)
     run_cmd_args = [
         "run",
         # podman run args
         "--rm",
         "-it",
         "-v",
-        f"{cwd}:/prj{VOLUME_OPTS}",
+        f"{cwd_absolute}:/prj{VOLUME_OPTS}",
         *parse_secondary_args(crun_args),
     ]
     run_cmd = ctr_engine.bake(
         *run_cmd_args,
     )
 
-    logger.debug(f"Running command: {run_cmd}")
+    # logger.debug(f"Running command: {run_cmd}")
 
     try:
-        run_proc = run_cmd(
+        run_cmd = run_cmd.bake(
             builder_image_name,
-            "/bin/bash",
+            login_shell,
             "-l",
             *parse_secondary_args(shell_args),
             _fg=True,
         )
+        logger.debug(f"Running command: {run_cmd}")
+        run_proc = run_cmd()
     except sh.ErrorReturnCode as e:
         print(f"Shell failed with error code {e.exit_code}")
         raise typer.Exit(1)
 
 
 @app.command(help="Initialize a build environment")
 def init(
```

### Comparing `redbuild-2.1.1/redbuild/composer.py` & `redbuild-2.2.0/redbuild/composer.py`

 * *Files identical despite different names*

### Comparing `redbuild-2.1.1/redbuild/engine.py` & `redbuild-2.2.0/redbuild/engine.py`

 * *Files identical despite different names*

### Comparing `redbuild-2.1.1/redbuild/util.py` & `redbuild-2.2.0/redbuild/util.py`

 * *Files identical despite different names*

### Comparing `redbuild-2.1.1/PKG-INFO` & `redbuild-2.2.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redbuild
-Version: 2.1.1
+Version: 2.2.0
 Summary: magic containerized builds
 Author: redthing1
 Author-email: redthing1@alt.icu
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -22,15 +22,15 @@
 
 # redbuild
 
 magic containerized builds
 
 ## overview
 
-redbuild is a super simple drop-in script enabling software to be built in pre-defined containers. with `podman` installed, any supported project can be built with a single command. projects provide a `build.docker` and `build.sh` for defining the build environment and build steps.
+redbuild enables software to be built in pre-defined environments using the power of containerization. with `podman` installed, any supported project can be built with a single command. projects provide a `build.docker` and `build.sh` for defining the build environment and build steps.
 
 `redbuild`: just add water!
 
 ## install stable version from pypi
 
 ```sh
 # with pipx (recommended)
@@ -100,7 +100,8 @@
 
     ```sh
     #!/bin/bash
     dub build --compiler ldc2 -B release
     ```
 
 that's it! now you can build the project with `redbuild build`, copy it into the project root, and run it. you can also open an interactive shell in the build environment with `redbuild shell`.
+
```

