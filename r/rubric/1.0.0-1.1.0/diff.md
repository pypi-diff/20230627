# Comparing `tmp/rubric-1.0.0.tar.gz` & `tmp/rubric-1.1.0.tar.gz`

## Comparing `rubric-1.0.0.tar` & `rubric-1.1.0.tar`

### file list

```diff
@@ -1,20 +1,18 @@
--rw-r--r--   0        0        0     7399 2020-02-02 00:00:00.000000 rubric-1.0.0/rubric/__init__.py
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 rubric-1.0.0/rubric/files/.editorconfig
--rw-r--r--   0        0        0     2035 2020-02-02 00:00:00.000000 rubric-1.0.0/rubric/files/.gitignore
--rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 rubric-1.0.0/rubric/files/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 rubric-1.0.0/rubric/files/Makefile
--rw-r--r--   0        0        0     2569 2020-02-02 00:00:00.000000 rubric-1.0.0/rubric/files/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rubric-1.0.0/rubric/files/__init__.py
--rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 rubric-1.0.0/rubric/files/pyproject.toml
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 rubric-1.0.0/rubric/files/requirements-dev.in
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rubric-1.0.0/rubric/files/requirements-dev.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rubric-1.0.0/rubric/files/requirements.in
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 rubric-1.0.0/rubric/files/requirements.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rubric-1.0.0/tests/__init__.py
--rw-r--r--   0        0        0     5653 2020-02-02 00:00:00.000000 rubric-1.0.0/tests/test_api.py
--rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 rubric-1.0.0/tests/test_cli.py
--rw-r--r--   0        0        0     2050 2020-02-02 00:00:00.000000 rubric-1.0.0/.gitignore
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 rubric-1.0.0/LICENSE
--rw-r--r--   0        0        0     6065 2020-02-02 00:00:00.000000 rubric-1.0.0/README.md
--rw-r--r--   0        0        0     2232 2020-02-02 00:00:00.000000 rubric-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     8646 2020-02-02 00:00:00.000000 rubric-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     7345 2020-02-02 00:00:00.000000 rubric-1.1.0/rubric/__init__.py
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 rubric-1.1.0/rubric/files/.editorconfig
+-rw-r--r--   0        0        0     2035 2020-02-02 00:00:00.000000 rubric-1.1.0/rubric/files/.gitignore
+-rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 rubric-1.1.0/rubric/files/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 rubric-1.1.0/rubric/files/Makefile
+-rw-r--r--   0        0        0     2569 2020-02-02 00:00:00.000000 rubric-1.1.0/rubric/files/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rubric-1.1.0/rubric/files/__init__.py
+-rw-r--r--   0        0        0      921 2020-02-02 00:00:00.000000 rubric-1.1.0/rubric/files/pyproject.toml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rubric-1.1.0/rubric/files/requirements-dev.txt
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 rubric-1.1.0/rubric/files/requirements.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rubric-1.1.0/tests/__init__.py
+-rw-r--r--   0        0        0     5496 2020-02-02 00:00:00.000000 rubric-1.1.0/tests/test_api.py
+-rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 rubric-1.1.0/tests/test_cli.py
+-rw-r--r--   0        0        0     2050 2020-02-02 00:00:00.000000 rubric-1.1.0/.gitignore
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 rubric-1.1.0/LICENSE
+-rw-r--r--   0        0        0     5946 2020-02-02 00:00:00.000000 rubric-1.1.0/README.md
+-rw-r--r--   0        0        0     2232 2020-02-02 00:00:00.000000 rubric-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     8527 2020-02-02 00:00:00.000000 rubric-1.1.0/PKG-INFO
```

### Comparing `rubric-1.0.0/rubric/__init__.py` & `rubric-1.1.0/rubric/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,30 +11,27 @@
 FILENAMES = (
     ".editorconfig",
     ".gitignore",
     ".pre-commit-config.yaml",
     "README.md",
     "Makefile",
     "pyproject.toml",
-    "requirements-dev.in",
     "requirements-dev.txt",
-    "requirements.in",
     "requirements.txt",
 )
 
 TERMINAL_COLUMN_SIZE: int = shutil.get_terminal_size().columns
 
 
 def copy_over(
     src_filename: str,
     dst_dirname: str = ".",
     overwrite: bool = False,
     append: bool = False,
 ) -> None:
-
     """
     This function takes 'src_filename' and 'dst_dirname' where they mean
     source file name and destination directory name respectively.
 
     First, it searches in the 'rubric' directory to check if there is
     a file that exists with the same name as the 'src_filename'. If the file
     exists, it creates another file named 'src_filename' in the 'dst_dirname'
@@ -57,15 +54,14 @@
         open_mode = "a+"
 
     # We use importlib here so that we don't have to deal with making
     # sure Python can find the `rubric` directory when this is installed
     # as a CLI.
     with importlib.resources.open_text("rubric.files", src_filename) as src_file:
         with open(dst_filepath, open_mode) as dst_file:
-
             if open_mode == "w+":
                 if overwrite:
                     print(f"Overwriting {src_filename}...")
                 else:
                     print(f"Creating {src_filename}...")
             else:
                 print(f"Appending to {src_filename}...")
@@ -138,15 +134,14 @@
 def orchestrator(
     dst_dirname: str,
     filenames: Iterable[str] = FILENAMES,  # Infra filenames.
     overwrite: bool = False,
     append: bool = False,
     show: bool = False,
 ) -> None:
-
     """
     Display / Create / Overwrite / Append to the files listed
     in the 'FILENAMES' iterable.
     """
 
     if show:
         for filename in filenames:
@@ -232,15 +227,14 @@
     dirname: str,
     filename: str,
     create: bool,
     overwrite: bool,
     append: bool,
     show: bool,
 ) -> None:
-
     # Display help text when there's no flag.
     if not any((list, create, overwrite, append, show)):
         display_help(ctx, None, True)
 
     if create and any((show, overwrite, append)):
         if show:
             raise click.UsageError(
```

### Comparing `rubric-1.0.0/rubric/files/.gitignore` & `rubric-1.1.0/rubric/files/.gitignore`

 * *Files identical despite different names*

### Comparing `rubric-1.0.0/rubric/files/Makefile` & `rubric-1.1.0/rubric/files/Makefile`

 * *Files identical despite different names*

### Comparing `rubric-1.0.0/rubric/files/README.md` & `rubric-1.1.0/rubric/files/README.md`

 * *Files identical despite different names*

### Comparing `rubric-1.0.0/rubric/files/pyproject.toml` & `rubric-1.1.0/rubric/files/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,26 @@
+[project]
+requires-python = ">=3.8"
+name = "foo"
+version = "0.1.0"
+
+dependencies = []
+
+[project.optional-dependencies]
+dev = [
+    "hatch",
+    "black",
+    "mypy",
+    "pip-tools",
+    "pytest",
+    "pytest-cov",
+    "ruff"
+]
+
+
 [tool.mypy]
 follow_imports = "skip"
 ignore_missing_imports = true
 warn_no_return = false
 warn_unused_ignores = true
 allow_untyped_globals = true
 allow_redefinition = true
```

### Comparing `rubric-1.0.0/tests/test_api.py` & `rubric-1.1.0/tests/test_api.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,17 +17,15 @@
     expected_filenames = (
         ".editorconfig",
         ".gitignore",
         ".pre-commit-config.yaml",
         "README.md",
         "Makefile",
         "pyproject.toml",
-        "requirements-dev.in",
         "requirements-dev.txt",
-        "requirements.in",
         "requirements.txt",
     )
 
     current_filenames = rubric.FILENAMES
 
     assert current_filenames == expected_filenames
 
@@ -82,19 +80,17 @@
     rubric.copy_over("pyproject.toml", dst_dirname=str(directory), append=True)
     assert len(list(directory.iterdir())) == 1
 
     assert "Lorem ipsum!" in file.read_text()
     assert "tool.ruff" in file.read_text()
 
 
+@pytest.mark.parametrize("filename", ["pyproject.toml", "README.md"])
 @pytest.mark.parametrize(
-    "filename", ["pyproject.toml", "README.md", "requirements-dev.in"]
-)
-@pytest.mark.parametrize(
-    "overwrite, append",
+    ("overwrite", "append"),
     [(False, False), (True, False), (False, True), (True, True)],
 )
 def test_orcherstrator(create_file, overwrite, append):
     file = create_file
     directory = file.parent
 
     # This should copy all the files from rubric/ to the temporary directory.
@@ -110,24 +106,21 @@
             for term in ("tool.ruff", "center", "pip-tools")
             if term in file.read_text()
         )
         is True
     )
 
 
-@pytest.mark.parametrize(
-    "filename", ["pyproject.toml", "README.md", "requirements-dev.in"]
-)
-@pytest.mark.parametrize("overwrite, append", [(True, False)])
+@pytest.mark.parametrize("filename", ["pyproject.toml", "README.md"])
+@pytest.mark.parametrize(("overwrite", "append"), [(True, False)])
 def test_orcherstrator_overwrite(
     create_file,
     overwrite,
     append,
 ):
-
     file = create_file
     directory = file.parent
     file.write_text("Lorem ipsum!")
 
     assert "Lorem ipsum!" in file.read_text()
 
     # This should copy all the files from rubric/ to the temporary directory.
@@ -149,18 +142,16 @@
         )
         is True
     )
 
     assert "Lorem ipsum!" not in file.read_text()
 
 
-@pytest.mark.parametrize(
-    "filename", ["pyproject.toml", "README.md", "requirements-dev.in"]
-)
-@pytest.mark.parametrize("overwrite, append", [(False, True)])
+@pytest.mark.parametrize("filename", ["pyproject.toml", "README.md"])
+@pytest.mark.parametrize(("overwrite", "append"), [(False, True)])
 def test_orcherstrator_append(create_file, overwrite, append):
     file = create_file
     directory = file.parent
 
     file.write_text("Lorem ipsum!")
 
     assert "Lorem ipsum!" in file.read_text()
@@ -185,15 +176,15 @@
         is True
     )
 
     assert "Lorem ipsum!" in file.read_text()
 
 
 def test_display(capsys):
-    for filename in ("pyproject.toml", "README.md", "requirements-dev.in"):
+    for filename in ("pyproject.toml", "README.md"):
         rubric.display_content(filename)
 
     capture = capsys.readouterr()
     out = capture.out
 
     for tool in ("ruff", "mypy", "black"):
         assert tool in out
```

### Comparing `rubric-1.0.0/.gitignore` & `rubric-1.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `rubric-1.0.0/LICENSE` & `rubric-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rubric-1.0.0/README.md` & `rubric-1.1.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -10,41 +10,39 @@
 
 ![logo]
 
 
 ## Preface
 
 Rubric initializes the configuration files of a few Python linters and formatters. Also,
-it adds a README.md boilerplace and a simple Makefile with the commands to apply the
+it adds a README.md boilerplate and a simple Makefile with the commands to apply the
 tools. This helps you maintain an isomorphic workflow across multiple projects. It
 assumes that, in all of your Python projects, you'll use—
 
 * [Black][black] as the primary code formatter.
-* [EditorConfig][editor-config] to enforce consistent coding styles for multiple
-developers.
+* [EditorConfig][editor-config] to enforce consistent style across different editors.
 * [Ruff][ruff] to ensure style guide conformance and sort the imports.
 * [Mypy][mypy] to check the type hints.
 * [Pip-tools][pip-tools] to manage the dependencies.
+* [Hatch][hatch] to generate build artifacts for reusable libraries.
 * [Pre-commit][pre-commit] for managing and maintaining the pre-commit hooks.
 
 
 Following is a list of config files that Rubric is going to add to your target
 directory:
 
 ```
 root
 ├── .editorconfig           # Config file for Editorconfig
 ├── .gitignore              # Python specific .gitignore file
 ├── .pre-commit-config.yaml # Config to manage pre-commit hooks.
 ├── Makefile                # Makefile containing the commands to lint your code
 ├── pyproject.toml          # Toml file to with the configs for black, ruff, and mypy
 ├── README.md               # A readme boilerplate
-├── requirements-dev.in     # File to specify the top level dev requirements
 ├── requirements-dev.txt    # File to specify the dev requirements
-├── requirements.in         # File to specify the top level app requirements
 └── requirements.txt        # File to specify the pinned app requirements
 ```
 
 The files will contain minimal but sensible default configurations for the respective
 tools. You're free to change them as you like.
 
 ## Installation
@@ -102,38 +100,38 @@
 
     => .editorconfig
     => .gitignore
     => .pre-commit-config.yaml
     => README.md
     => Makefile
     => pyproject.toml
-    => requirements-dev.in
     => requirements-dev.txt
-    => requirements.in
     => requirements.txt
     ```
 
 * Take a peek into the content of any config file(s):
-    ```
+
+    ```sh
     rubric --show -f requirements.txt -f .editorconfig
     ```
 
     This will print:
 
-    ```
-    ========================== requirements.txt ==========================
+    ```txt
+
+    ============================ requirements.txt ============================
 
     #
     # This file is autogenerated by pip-compile with python 3.11
     # To update, run:
     #
     #    pip-compile --output-file=requirements.txt requirements.in
     #
 
-    ========================== .editorconfig ==========================
+    ============================ .editorconfig ============================
 
     # https://editorconfig.org
 
     root = true
 
     [*]
     indent_style = space
@@ -149,50 +147,50 @@
     [Makefile]
     indent_size = 4
     indent_style = tab
     ```
 
 * Initialize a project with the following command:
 
-    ```
+    ```sh
     rubric --create
     ```
 
     This will run the tool in a non-destructive way—that means it won't overwrite any of
-    the configuration files that you might have in the directory.
+    the configuration files that you might already have in the directory.
 
 * If you only want to create a selected list of config files, then run:
 
-    ```
+    ```sh
     rubric --create -f requirements.txt -f requirements-dev.txt
     ```
 
 * If you want to overwrite any of the existing config files that you might have in the
 directory, then run:
 
-    ```
+    ```sh
     rubric --overwrite -f filename1 -f filename2
     ```
 
 * If you want to append the configs to an existing file, then run:
 
-    ```
+    ```sh
     rubric --append -f filename1 -f filename2
     ```
 
 * You can also point Rubric to a directory.
 
-    ```
+    ```sh
     rubric --create --directory "some/custom/directory"
     ```
 
 * If you want to check and update the configs across multiple repositories in a single
 sweep, use the following command:
 
-    ```
+    ```sh
     s="dir1 dir2 dir3"; echo $s | xargs -n 1 -P $(echo $s | wc -w) rubric -c -d
     ```
 
     This command will spawn 3 processes to create the config files in `dir1`, `dir2`,
     and `dir3` in parallel.
 
 * You can run the entire linter suite with this command:
```

### Comparing `rubric-1.0.0/pyproject.toml` & `rubric-1.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "rubric"
-version = "1.0.0"
+version = "1.1.0"
 authors = [
   { name="rednafi", email="redowan.nafi@gmail.com" },
 ]
 description = ">> Linter Config Initialization for Python <<"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.8"
```

### Comparing `rubric-1.0.0/PKG-INFO` & `rubric-1.1.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rubric
-Version: 1.0.0
+Version: 1.1.0
 Summary: >> Linter Config Initialization for Python <<
 Project-URL: Homepage, https://github.com/rednafi/rubric
 Project-URL: Issue Tracker, https://github.com/pypa/rubric/issues
 Author-email: rednafi <redowan.nafi@gmail.com>
 License: MIT License
         
         Copyright (c) 2021 Redowan Delowar
@@ -64,41 +64,39 @@
 
 ![logo]
 
 
 ## Preface
 
 Rubric initializes the configuration files of a few Python linters and formatters. Also,
-it adds a README.md boilerplace and a simple Makefile with the commands to apply the
+it adds a README.md boilerplate and a simple Makefile with the commands to apply the
 tools. This helps you maintain an isomorphic workflow across multiple projects. It
 assumes that, in all of your Python projects, you'll use—
 
 * [Black][black] as the primary code formatter.
-* [EditorConfig][editor-config] to enforce consistent coding styles for multiple
-developers.
+* [EditorConfig][editor-config] to enforce consistent style across different editors.
 * [Ruff][ruff] to ensure style guide conformance and sort the imports.
 * [Mypy][mypy] to check the type hints.
 * [Pip-tools][pip-tools] to manage the dependencies.
+* [Hatch][hatch] to generate build artifacts for reusable libraries.
 * [Pre-commit][pre-commit] for managing and maintaining the pre-commit hooks.
 
 
 Following is a list of config files that Rubric is going to add to your target
 directory:
 
 ```
 root
 ├── .editorconfig           # Config file for Editorconfig
 ├── .gitignore              # Python specific .gitignore file
 ├── .pre-commit-config.yaml # Config to manage pre-commit hooks.
 ├── Makefile                # Makefile containing the commands to lint your code
 ├── pyproject.toml          # Toml file to with the configs for black, ruff, and mypy
 ├── README.md               # A readme boilerplate
-├── requirements-dev.in     # File to specify the top level dev requirements
 ├── requirements-dev.txt    # File to specify the dev requirements
-├── requirements.in         # File to specify the top level app requirements
 └── requirements.txt        # File to specify the pinned app requirements
 ```
 
 The files will contain minimal but sensible default configurations for the respective
 tools. You're free to change them as you like.
 
 ## Installation
@@ -156,38 +154,38 @@
 
     => .editorconfig
     => .gitignore
     => .pre-commit-config.yaml
     => README.md
     => Makefile
     => pyproject.toml
-    => requirements-dev.in
     => requirements-dev.txt
-    => requirements.in
     => requirements.txt
     ```
 
 * Take a peek into the content of any config file(s):
-    ```
+
+    ```sh
     rubric --show -f requirements.txt -f .editorconfig
     ```
 
     This will print:
 
-    ```
-    ========================== requirements.txt ==========================
+    ```txt
+
+    ============================ requirements.txt ============================
 
     #
     # This file is autogenerated by pip-compile with python 3.11
     # To update, run:
     #
     #    pip-compile --output-file=requirements.txt requirements.in
     #
 
-    ========================== .editorconfig ==========================
+    ============================ .editorconfig ============================
 
     # https://editorconfig.org
 
     root = true
 
     [*]
     indent_style = space
@@ -203,50 +201,50 @@
     [Makefile]
     indent_size = 4
     indent_style = tab
     ```
 
 * Initialize a project with the following command:
 
-    ```
+    ```sh
     rubric --create
     ```
 
     This will run the tool in a non-destructive way—that means it won't overwrite any of
-    the configuration files that you might have in the directory.
+    the configuration files that you might already have in the directory.
 
 * If you only want to create a selected list of config files, then run:
 
-    ```
+    ```sh
     rubric --create -f requirements.txt -f requirements-dev.txt
     ```
 
 * If you want to overwrite any of the existing config files that you might have in the
 directory, then run:
 
-    ```
+    ```sh
     rubric --overwrite -f filename1 -f filename2
     ```
 
 * If you want to append the configs to an existing file, then run:
 
-    ```
+    ```sh
     rubric --append -f filename1 -f filename2
     ```
 
 * You can also point Rubric to a directory.
 
-    ```
+    ```sh
     rubric --create --directory "some/custom/directory"
     ```
 
 * If you want to check and update the configs across multiple repositories in a single
 sweep, use the following command:
 
-    ```
+    ```sh
     s="dir1 dir2 dir3"; echo $s | xargs -n 1 -P $(echo $s | wc -w) rubric -c -d
     ```
 
     This command will spawn 3 processes to create the config files in `dir1`, `dir2`,
     and `dir3` in parallel.
 
 * You can run the entire linter suite with this command:
```

