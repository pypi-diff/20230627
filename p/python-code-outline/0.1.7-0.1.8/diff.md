# Comparing `tmp/python_code_outline-0.1.7.tar.gz` & `tmp/python_code_outline-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_code_outline-0.1.7.tar", max compression
+gzip compressed data, was "python_code_outline-0.1.8.tar", max compression
```

## Comparing `python_code_outline-0.1.7.tar` & `python_code_outline-0.1.8.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1061 2023-04-12 06:31:17.603547 python_code_outline-0.1.7/LICENSE
--rw-r--r--   0        0        0     5862 2023-06-08 08:42:20.090459 python_code_outline-0.1.7/README.md
--rw-r--r--   0        0        0      581 2023-06-10 07:50:28.984205 python_code_outline-0.1.7/pyproject.toml
--rw-r--r--   0        0        0      155 2023-06-10 07:46:56.328447 python_code_outline-0.1.7/python_code_outline/__init__.py
--rw-r--r--   0        0        0        0 2023-06-10 07:50:00.560611 python_code_outline-0.1.7/python_code_outline/py.typed
--rw-r--r--   0        0        0     5505 2023-06-08 08:35:39.928287 python_code_outline-0.1.7/python_code_outline/python_report_generator.py
--rw-r--r--   0        0        0     6149 1970-01-01 00:00:00.000000 python_code_outline-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     1061 2023-04-12 06:31:17.603547 python_code_outline-0.1.8/LICENSE
+-rw-r--r--   0        0        0     6153 2023-06-27 06:59:29.615431 python_code_outline-0.1.8/README.md
+-rw-r--r--   0        0        0      583 2023-06-27 06:58:29.576160 python_code_outline-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0      155 2023-06-10 07:46:56.328447 python_code_outline-0.1.8/python_code_outline/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-10 07:50:00.560611 python_code_outline-0.1.8/python_code_outline/py.typed
+-rw-r--r--   0        0        0     6064 2023-06-27 07:10:27.920727 python_code_outline-0.1.8/python_code_outline/python_report_generator.py
+-rw-r--r--   0        0        0     6592 1970-01-01 00:00:00.000000 python_code_outline-0.1.8/PKG-INFO
```

### Comparing `python_code_outline-0.1.7/LICENSE` & `python_code_outline-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `python_code_outline-0.1.7/README.md` & `python_code_outline-0.1.8/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,153 +1,163 @@
-# Python Code Structure Report Generator
-
-[![PyPI version](https://badge.fury.io/py/python-code-outline.svg)](https://badge.fury.io/py/python-code-outline)
-
-![Test](https://github.com/seandearnaley/python-code-outline/workflows/Run%20pytest/badge.svg)
-
-This Python script generates a text-based report of the code structure for all Python files in a given folder. It's useful for getting a quick overview of the code structure of a Python project. This can be particularly helpful for ChatGPT/Large Language Model (LLM) applications where you need to ask high-level questions about your codebase.
-
-[Example Report](example_report.txt?raw=true)
-
-## Usage
-
-To use this script, run the `python_report_generator.py` file and provide the path to the folder containing the Python files you want to analyze. You can also optionally specify a name for the report file, which defaults to `report.txt` if not provided, and a path to the ignore file. The ignore file should be a `.gitignore` file or a file with the same format as a `.gitignore` file. If provided, the script will parse the ignore patterns from the file and exclude the matching files and folders from the report.
-
-```bash
-python python_code_outline/python_report_generator.py /path/to/folder --report_file_path custom_report.txt --ignore_file_path /path/to/folder/.gitignore
-```
-
-If the `--report_file_path` option is not specified, the report will be written to `report.txt` by default.
-
-```bash
-python python_report_generator.py /path/to/folder
-```
-
-## Usage as a pip module
-
-After installing the package via pip, you can import and use the functionality in your own code as well. For example:
-
-```python
-""" Generate a report of the python code outline of a folder. """
-from python_code_outline import get_report
-
-# Define the root folder
-ROOT_FOLDER = "/path/to/folder"
-
-# Specify the report and ignore file paths (optional)
-REPORT_FILE_PATH = "custom_report.txt"
-IGNORE_FILE_PATH = "/path/to/folder/.gitignore"
-
-# Generate the report
-REPORT = python_report_generator.get_report(ROOT_FOLDER, IGNORE_FILE_PATH)
-
-# Write the report to a file
-with open(REPORT_FILE_PATH, "w", encoding="utf-8") as file:
-    file.write(REPORT)
-
-print(f"Report generated successfully to {REPORT_FILE_PATH}.")
-```
-
-Please replace "/path/to/folder" with the path to the folder you want to analyze, and update the report and ignore file paths as necessary.
-
-## Output
-
-The script will generate a text-based report of the code structure for each Python file in the specified folder. The report includes information about imports, classes, functions, and variables in each file.
-
-## Optional Parameters
-
-- `--report_file_path`: The name of the report file. Defaults to `report.txt` if not provided.
-- `--ignore_file_path`: The path to the ignore file. If provided, the script will parse the ignore patterns from the file and exclude the matching files and folders from the report.
-
-## Requirements
-
-This script requires Python 3.x to run.
-
-## Installation
-
-This project uses [Poetry](https://python-poetry.org/) for dependency management. To install the dependencies, first install Poetry by following the [official installation guide](https://python-poetry.org/docs/#installation), and then run the following command in the project directory:
-
-```bash
-poetry install
-```
-
-This will create a virtual environment and install the required dependencies.
-
-You can install this module using pip:
-
-```bash
-pip install python-code-outline
-```
-
-or with poetry
-
-```bash
-poetry add python-code-outline
-```
-
-This command will download the package from PyPI and install it in your current Python environment.
-
-## Running Tests
-
-This project uses `pytest` for testing. To run the tests, first activate the virtual environment created by Poetry:
-
-```bash
-poetry shell
-```
-
-Then, run the tests using the following command:
-
-```bash
-pytest
-```
-
-## Checking Test Coverage
-
-This project uses the `coverage` package to generate test coverage reports. Here's how to use it:
-
-1. First, you need to install the `coverage` package if it's not already installed.
-
-```bash
-pip install coverage
-```
-
-or
-
-```bash
-poetry add coverage
-```
-
-If you're using Poetry, you can also add `coverage` to your `pyproject.toml` file and run `poetry install` to install it.
-
-2. After installing `coverage`, you can use it to run your tests and collect coverage data. If you're using `pytest` for testing, you can use the following command:
-
-```bash
-coverage run -m pytest
-```
-
-This command tells `coverage` to run `pytest` as a module (hence the `-m` flag), and `coverage` collects data about which parts of your code were executed during the test run.
-
-3. Once you've collected coverage data, you can generate a report by running:
-
-```bash
-coverage report
-```
-
-This will print a coverage report to the terminal, showing the code coverage for each module in your project.
-
-4. If you want a more detailed view, you can generate an HTML report using:
-
-```bash
-coverage html
-```
-
-This will generate an `htmlcov` directory in your project directory. Inside this directory, you'll find an `index.html` file. You can open this file in a web browser to view a detailed coverage report that shows which lines of each file were covered by the tests.
-
-5. If you're finished checking coverage and want to clear the collected data, you can use the command:
-
-```bash
-coverage erase
-```
-
-This will delete the `.coverage` data file, clearing the collected coverage data.
-
-Remember that code coverage is a useful tool for finding untested parts of your code, but achieving 100% code coverage doesn't necessarily mean your testing is perfect. It's important to write meaningful tests and not just strive for high coverage percentages.
+# Python Code Structure Report Generator
+
+[![PyPI version](https://badge.fury.io/py/python-code-outline.svg)](https://badge.fury.io/py/python-code-outline)
+
+![Test](https://github.com/seandearnaley/python-code-outline/workflows/Run%20pytest/badge.svg)
+
+[![codecov](https://codecov.io/gh/seandearnaley/python-code-outline/branch/main/graph/badge.svg?token=ZTO7T0J6TZ)](https://codecov.io/gh/seandearnaley/python-code-outline)
+
+This Python script generates a text-based report of the code structure for all Python files in a given folder. It's useful for getting a quick overview of the code structure of a Python project. This can be particularly helpful for ChatGPT/Large Language Model (LLM) applications where you need to ask high-level questions about your codebase.
+
+[Example Report](example_report.txt?raw=true)
+
+## Usage
+
+To use this script, run the `python_report_generator.py` file and provide the path to the folder containing the Python files you want to analyze. You can also optionally specify a name for the report file, which defaults to `report.txt` if not provided, and a path to the ignore file. The ignore file should be a `.gitignore` file or a file with the same format as a `.gitignore` file. If provided, the script will parse the ignore patterns from the file and exclude the matching files and folders from the report.
+
+```bash
+python python_code_outline/python_report_generator.py /path/to/folder --report_file_path custom_report.txt --ignore_file_path /path/to/folder/.gitignore
+```
+
+If the `--report_file_path` option is not specified, the report will be written to `report.txt` by default.
+
+```bash
+python python_code_outline/python_report_generator.py /path/to/folder
+```
+
+## Usage as a pip module
+
+After installing the package via pip, you can import and use the functionality in your own code as well. For example:
+
+```python
+""" Generate a report of the python code outline of a folder. """
+from python_code_outline import get_report
+
+# Define the root folder
+ROOT_FOLDER = "/path/to/folder"
+
+# Specify the report and ignore file paths (optional)
+REPORT_FILE_PATH = "custom_report.txt"
+IGNORE_FILE_PATH = "/path/to/folder/.gitignore"
+
+# Generate the report
+REPORT = python_report_generator.get_report(ROOT_FOLDER, IGNORE_FILE_PATH)
+
+# Write the report to a file
+with open(REPORT_FILE_PATH, "w", encoding="utf-8") as file:
+    file.write(REPORT)
+
+print(f"Report generated successfully to {REPORT_FILE_PATH}.")
+```
+
+Please replace "/path/to/folder" with the path to the folder you want to analyze, and update the report and ignore file paths as necessary.
+
+## Output
+
+The script will generate a text-based report of the code structure for each Python file in the specified folder. The report includes information about imports, classes, functions, and variables in each file.
+
+## Optional Parameters
+
+- `--report_file_path`: The name of the report file. Defaults to `report.txt` if not provided.
+- `--ignore_file_path`: The path to the ignore file. If provided, the script will parse the ignore patterns from the file and exclude the matching files and folders from the report.
+
+## Requirements
+
+This script requires Python 3.x to run.
+
+## Installation
+
+This project uses [Poetry](https://python-poetry.org/) for dependency management. To install the dependencies, first install Poetry by following the [official installation guide](https://python-poetry.org/docs/#installation), and then run the following command in the project directory:
+
+```bash
+poetry install
+```
+
+This will create a virtual environment and install the required dependencies.
+
+You can install this module using pip:
+
+```bash
+pip install python-code-outline
+```
+
+or with poetry
+
+```bash
+poetry add python-code-outline
+```
+
+This command will download the package from PyPI and install it in your current Python environment.
+
+## Running Tests
+
+This project uses `pytest` for testing. To run the tests, first activate the virtual environment created by Poetry:
+
+```bash
+poetry shell
+```
+
+Then, run the tests using the following command:
+
+```bash
+pytest
+```
+
+## Checking Test Coverage
+
+This project uses the `pytest-cov` package to generate test coverage reports. Here's how to use it:
+
+1. First, you need to install the `pytest-cov` package if it's not already installed.
+
+```bash
+pip install pytest-cov
+```
+
+or
+
+```bash
+poetry add pytest-cov
+```
+
+If you're using Poetry, you can also add `pytest-cov` to your `pyproject.toml` file and run `poetry install` to install it.
+
+2. After installing `pytest-cov`, you can use it to run your tests and collect coverage data. If you're using `pytest` for testing, you can use the following command:
+
+```bash
+pytest --cov=python_code_outline
+```
+
+This command tells `pytest` to collect coverage data for the `python_code_outline` module during the test run.
+
+3. Once you've collected coverage data, you can generate a report by running:
+
+```bash
+coverage report
+```
+
+This will print a coverage report to the terminal, showing the code coverage for each module in your project.
+
+4. If you want a more detailed view, you can generate an HTML report using:
+
+```bash
+coverage html
+```
+
+This will generate an `htmlcov` directory in your project directory. Inside this directory, you'll find an `index.html` file. You can open this file in a web browser to view a detailed coverage report that shows which lines of each file were covered by the tests.
+
+5. If you're finished checking coverage and want to clear the collected data, you can use the command:
+
+```bash
+coverage erase
+```
+
+This will delete the `.coverage` data file, clearing the collected coverage data.
+
+Remember that code coverage is a useful tool for finding untested parts of your code, but achieving 100% code coverage doesn't necessarily mean your testing is perfect. It's important to write meaningful tests and not just strive for high coverage percentages.
+
+## Contributing
+
+Contributions are welcome! Please feel free to submit a pull request or open an issue on the [GitHub repository](https://github.com/seandearnaley/python-code-outline).
+
+## License
+
+This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
```

### Comparing `python_code_outline-0.1.7/python_code_outline/python_report_generator.py` & `python_code_outline-0.1.8/python_code_outline/python_report_generator.py`

 * *Files 4% similar despite different names*

```diff
@@ -75,17 +75,14 @@
             output.extend(process_function_def(item))
         elif isinstance(item, ast.ClassDef):
             output.extend(process_class_def(item))
 
     return "\n".join(output)
 
 
-# ...
-
-
 def generate_report(
     root: str, root_folder: str, ignored_patterns: Optional[List[str]] = None
 ) -> str:
     """
     Generate a report of the code structure for all Python
     files in a given folder."""
 
@@ -106,14 +103,25 @@
             subdir_report = generate_report(str(entry), root_folder, ignored_patterns)
             if subdir_report:
                 report.append(subdir_report)
 
     return "\n\n".join(report)
 
 
+def expand_user_path(path: Optional[str]) -> Optional[str]:
+    """Expand the user home directory symbol '~' if it's part of the path."""
+    if path is not None:
+        path_obj = Path(path)
+        if "~" in path:
+            return str(path_obj.expanduser().resolve())
+
+        return str(path_obj)
+    return None
+
+
 def parse_arguments() -> argparse.Namespace:
     """Parse the command-line arguments."""
     parser = argparse.ArgumentParser(
         description=(
             "Generate a text-based report of the code structure for all Python files in"
             " a given folder."
         )
@@ -130,24 +138,30 @@
         type=str,
         default=None,
         help="Path to the ignore file",
     )
 
     args = parser.parse_args()
 
-    root_folder: str = args.root_folder
-
-    if not Path(root_folder).is_dir():
-        raise ValueError(f"{root_folder} is not a valid directory")
+    args.root_folder = expand_user_path(args.root_folder)
+    args.ignore_file_path = expand_user_path(args.ignore_file_path)
 
     return args
 
 
 def get_report(root_folder: str, ignore_file_path: Optional[str] = None) -> str:
     """Get the report of the code structure for all Python files in a given folder."""
+
+    if not Path(root_folder).is_dir():
+        raise ValueError(f"{root_folder} is not a valid directory")
+
+    if ignore_file_path is not None:
+        if not Path(ignore_file_path).is_file():
+            raise ValueError(f"{ignore_file_path} is not a valid file")
+
     ignored_patterns = (
         parse_ignore_patterns(ignore_file_path)
         if ignore_file_path and Path(ignore_file_path).exists()
         else []
     )
 
     return generate_report(root_folder, root_folder, ignored_patterns)
```

### Comparing `python_code_outline-0.1.7/PKG-INFO` & `python_code_outline-0.1.8/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-code-outline
-Version: 0.1.7
+Version: 0.1.8
 Summary: Takes a folder path and outputs a text outline of the code, supports ignore files.
 Author: Sean Dearnaley
 Author-email: SeanDearnaley@outlook.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -12,14 +12,16 @@
 
 # Python Code Structure Report Generator
 
 [![PyPI version](https://badge.fury.io/py/python-code-outline.svg)](https://badge.fury.io/py/python-code-outline)
 
 ![Test](https://github.com/seandearnaley/python-code-outline/workflows/Run%20pytest/badge.svg)
 
+[![codecov](https://codecov.io/gh/seandearnaley/python-code-outline/branch/main/graph/badge.svg?token=ZTO7T0J6TZ)](https://codecov.io/gh/seandearnaley/python-code-outline)
+
 This Python script generates a text-based report of the code structure for all Python files in a given folder. It's useful for getting a quick overview of the code structure of a Python project. This can be particularly helpful for ChatGPT/Large Language Model (LLM) applications where you need to ask high-level questions about your codebase.
 
 [Example Report](example_report.txt?raw=true)
 
 ## Usage
 
 To use this script, run the `python_report_generator.py` file and provide the path to the folder containing the Python files you want to analyze. You can also optionally specify a name for the report file, which defaults to `report.txt` if not provided, and a path to the ignore file. The ignore file should be a `.gitignore` file or a file with the same format as a `.gitignore` file. If provided, the script will parse the ignore patterns from the file and exclude the matching files and folders from the report.
@@ -27,15 +29,15 @@
 ```bash
 python python_code_outline/python_report_generator.py /path/to/folder --report_file_path custom_report.txt --ignore_file_path /path/to/folder/.gitignore
 ```
 
 If the `--report_file_path` option is not specified, the report will be written to `report.txt` by default.
 
 ```bash
-python python_report_generator.py /path/to/folder
+python python_code_outline/python_report_generator.py /path/to/folder
 ```
 
 ## Usage as a pip module
 
 After installing the package via pip, you can import and use the functionality in your own code as well. For example:
 
 ```python
@@ -110,37 +112,37 @@
 
 ```bash
 pytest
 ```
 
 ## Checking Test Coverage
 
-This project uses the `coverage` package to generate test coverage reports. Here's how to use it:
+This project uses the `pytest-cov` package to generate test coverage reports. Here's how to use it:
 
-1. First, you need to install the `coverage` package if it's not already installed.
+1. First, you need to install the `pytest-cov` package if it's not already installed.
 
 ```bash
-pip install coverage
+pip install pytest-cov
 ```
 
 or
 
 ```bash
-poetry add coverage
+poetry add pytest-cov
 ```
 
-If you're using Poetry, you can also add `coverage` to your `pyproject.toml` file and run `poetry install` to install it.
+If you're using Poetry, you can also add `pytest-cov` to your `pyproject.toml` file and run `poetry install` to install it.
 
-2. After installing `coverage`, you can use it to run your tests and collect coverage data. If you're using `pytest` for testing, you can use the following command:
+2. After installing `pytest-cov`, you can use it to run your tests and collect coverage data. If you're using `pytest` for testing, you can use the following command:
 
 ```bash
-coverage run -m pytest
+pytest --cov=python_code_outline
 ```
 
-This command tells `coverage` to run `pytest` as a module (hence the `-m` flag), and `coverage` collects data about which parts of your code were executed during the test run.
+This command tells `pytest` to collect coverage data for the `python_code_outline` module during the test run.
 
 3. Once you've collected coverage data, you can generate a report by running:
 
 ```bash
 coverage report
 ```
 
@@ -159,7 +161,16 @@
 ```bash
 coverage erase
 ```
 
 This will delete the `.coverage` data file, clearing the collected coverage data.
 
 Remember that code coverage is a useful tool for finding untested parts of your code, but achieving 100% code coverage doesn't necessarily mean your testing is perfect. It's important to write meaningful tests and not just strive for high coverage percentages.
+
+## Contributing
+
+Contributions are welcome! Please feel free to submit a pull request or open an issue on the [GitHub repository](https://github.com/seandearnaley/python-code-outline).
+
+## License
+
+This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
+
```

