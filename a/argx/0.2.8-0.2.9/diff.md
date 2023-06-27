# Comparing `tmp/argx-0.2.8.tar.gz` & `tmp/argx-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "argx-0.2.8.tar", max compression
+gzip compressed data, was "argx-0.2.9.tar", max compression
```

## Comparing `argx-0.2.8.tar` & `argx-0.2.9.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1063 2023-06-19 19:02:21.857186 argx-0.2.8/LICENSE
--rw-r--r--   0        0        0    14316 2023-06-19 19:02:21.857186 argx-0.2.8/README.md
--rw-r--r--   0        0        0      151 2023-06-19 19:02:21.857186 argx-0.2.8/argx/__init__.py
--rw-r--r--   0        0        0     6571 2023-06-19 19:02:21.857186 argx-0.2.8/argx/action.py
--rw-r--r--   0        0        0     3956 2023-06-19 19:02:21.857186 argx-0.2.8/argx/formatter.py
--rw-r--r--   0        0        0    20522 2023-06-19 19:02:21.857186 argx-0.2.8/argx/parser.py
--rw-r--r--   0        0        0      717 2023-06-19 19:02:21.857186 argx-0.2.8/argx/type_.py
--rw-r--r--   0        0        0     2610 2023-06-19 19:02:21.857186 argx-0.2.8/argx/utils.py
--rw-r--r--   0        0        0     1021 2023-06-19 19:02:21.857186 argx-0.2.8/pyproject.toml
--rw-r--r--   0        0        0    15496 1970-01-01 00:00:00.000000 argx-0.2.8/setup.py
--rw-r--r--   0        0        0    14938 1970-01-01 00:00:00.000000 argx-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-06-27 02:34:40.921715 argx-0.2.9/LICENSE
+-rw-r--r--   0        0        0    14316 2023-06-27 02:34:40.921715 argx-0.2.9/README.md
+-rw-r--r--   0        0        0      151 2023-06-27 02:34:40.921715 argx-0.2.9/argx/__init__.py
+-rw-r--r--   0        0        0     6571 2023-06-27 02:34:40.921715 argx-0.2.9/argx/action.py
+-rw-r--r--   0        0        0     3956 2023-06-27 02:34:40.921715 argx-0.2.9/argx/formatter.py
+-rw-r--r--   0        0        0    20522 2023-06-27 02:34:40.921715 argx-0.2.9/argx/parser.py
+-rw-r--r--   0        0        0      717 2023-06-27 02:34:40.921715 argx-0.2.9/argx/type_.py
+-rw-r--r--   0        0        0     2610 2023-06-27 02:34:40.921715 argx-0.2.9/argx/utils.py
+-rw-r--r--   0        0        0     1017 2023-06-27 02:34:40.921715 argx-0.2.9/pyproject.toml
+-rw-r--r--   0        0        0    15492 1970-01-01 00:00:00.000000 argx-0.2.9/setup.py
+-rw-r--r--   0        0        0    14934 1970-01-01 00:00:00.000000 argx-0.2.9/PKG-INFO
```

### Comparing `argx-0.2.8/LICENSE` & `argx-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `argx-0.2.8/README.md` & `argx-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `argx-0.2.8/argx/action.py` & `argx-0.2.9/argx/action.py`

 * *Files identical despite different names*

### Comparing `argx-0.2.8/argx/formatter.py` & `argx-0.2.9/argx/formatter.py`

 * *Files identical despite different names*

### Comparing `argx-0.2.8/argx/parser.py` & `argx-0.2.9/argx/parser.py`

 * *Files identical despite different names*

### Comparing `argx-0.2.8/argx/type_.py` & `argx-0.2.9/argx/type_.py`

 * *Files identical despite different names*

### Comparing `argx-0.2.8/argx/utils.py` & `argx-0.2.9/argx/utils.py`

 * *Files identical despite different names*

### Comparing `argx-0.2.8/pyproject.toml` & `argx-0.2.9/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 [tool.poetry]
 name = "argx"
-version = "0.2.8"
+version = "0.2.9"
 description = "Super-charged argparse for python"
 authors = ["pwwang <pwwang@pwwang.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.build]
 generate-setup-file = true
 
 [tool.poetry.dependencies]
 python = "^3.7"
-python-simpleconf = "^0.5.7"
+python-simpleconf = "^0.6"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7"
 pytest-cov = "^4"
-python-simpleconf = {version = "^0.5.7", extras = ["toml"]}
+python-simpleconf = {version = "^0.6", extras = ["toml"]}
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.mypy]
 ignore_missing_imports = true
```

### Comparing `argx-0.2.8/setup.py` & `argx-0.2.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 packages = \
 ['argx']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['python-simpleconf>=0.5.7,<0.6.0']
+['python-simpleconf>=0.6,<0.7']
 
 setup_kwargs = {
     'name': 'argx',
-    'version': '0.2.8',
+    'version': '0.2.9',
     'description': 'Super-charged argparse for python',
     'long_description': '# argx\n\n[![pypi][1]][2] [![tag][3]][2] [![codacy quality][4]][5] [![codacy quality][6]][5] ![github action][7] ![pyver][8]\n\nSupercharged argparse for Python\n\n## Installation\n\n```bash\npip install -U argx\n```\n\n## Features enhanced or added\n\n- [Option `exit_on_void`](#option-exit_on_void): Exit with error if no arguments are provided\n- [Subcommand shortcut](#subcommand-shortcut): Adding subcommands directly, without `parser.add_subparsers()`\n- [Namespace arguments](#namespace-arguments): Access arguments like `--foo.bar` as `args.foo.bar`\n- [Brief help message for massive arguments](#brief-help-message-for-massive-arguments): Show only the most important arguments in the help message\n- [Default value in argument help](#default-value-in-argument-help): Show the default value in the help message of arguments\n- [Newlines kept in help](#newlines-kept-in-help): Newlines are kept in argument help if any\n- [Defaults from file](#defaults-from-files): Read default values from a configuration file by API or from command line\n- [Clear-append/extend action](#clear_appendextend-action): Store a list of values. Different from `append` and `extend`, the initial value is cleared.\n- [Grouping required arguments by default](#grouping-required-arguments-by-default): Put required arguments in \'required arguments\' group, instead of \'optional arguments\' group\n- [Order of groups in help message](#order-of-groups-in-help-message): Allow to add an `order` attribute to groups to change the order of groups in help message\n- [Addtional types](#additional-types): Some additional types to convert the values of arguments\n- [Configuration file to create the parser](#configuration-file-to-create-the-parser): Instead of creating the parser by code, you can also create it by a configuration file\n- [Pre-parse hook](#pre-parse-hook): A hook to modify the arguments before parsing\n- [Backward compatibility](#backward-compatibility): All features are optional. You can use `argx` as a drop-in replacement for `argparse`.\n\n### Option `exit_on_void`\n\nIf all arguments are optional, `argparse` will not raise an error if no arguments are provided. This is not always desirable. `argx` provides the option `exit_on_void` to change this behavior. If `exit_on_void` is set to `True` and no arguments are provided, `argx` will exit with an error (No arguments provided).\n\n```python\nimport argx as argparse\n\nparser = argparse.ArgumentParser(exit_on_void=True)\nparser.add_argument(\'--foo\', action=\'store_true\')\n\nargs = parser.parse_args([])\n# No arguments provided\n# standard argparse produces: Namespace(foo=False)\n```\n\n### Subcommand shortcut\n\n`argparse` requires to create subparsers first and then add the subcommands to the subparsers.\n`argx` allows to add subcommands directly to the main parser.\n\n```python\n# standard argparse\nparser = argparse.ArgumentParser()\nsubparsers = parser.add_subparsers(title=\'subcommands\')\nparser_a = subparsers.add_parser(\'a\')\nparser_b = subparsers.add_parser(\'b\')\n\n# argx\nparser = argparse.ArgumentParser()\nparser.add_command(\'a\')  # or parser.add_subparser(\'a\')\nparser.add_command(\'b\')\n# args = parser.parse_args([\'a\'])\n# Namespace(COMMAND=\'a\')\n```\n\nThe `subparsers` is added automatically with the title `subcommands` and the `dest` is set to `COMMAND`. You can add subcommands to subcommands directly, then the `dest` is set to `COMMAND2`, `COMMAND3`, etc. If you want to change the behavior, you can always fall back to the standard `argparse` way.\n\n### Namespace arguments\n\nThe values of arguments like `--foo.bar` can be accessed as `vars(args)[\'foo.bar\']`. With `argx` you can access them as `args.foo.bar`.\n\nThe arguments `--foo.bar`, `--foo.baz` and `--foo.qux` are automatically grouped in a namespace `foo`.\n\n```python\nimport argx as argparse\n\nparser = argparse.ArgumentParser()\nparser.add_argument(\'--foo.bar\', type=int)\nparser.add_argument(\'--foo.baz\', type=int)\nparser.add_argument(\'--foo.qux\', type=int)\n\nparser.print_help()\n```\n\n```shell\nUsage: test.py [-h] [--foo.bar BAR] [--foo.baz BAZ] [--foo.qux QUX]\n\nOptional arguments:\n  -h, --help            show this help message and exit\n\nNamespace <foo>:\n  --foo.bar BAR\n  --foo.baz BAZ\n  --foo.qux QUX\n```\n\nYou can modify the namespace by adding the namespace manually before adding the arguments.\n\n```python\nimport argx as argparse\n\nparser = argparse.ArgumentParser()\nparser.add_namespace(\'foo\', title="Foo\'s options")\nparser.add_argument(\'--foo.bar\', type=int)\nparser.add_argument(\'--foo.baz\', type=int)\nparser.add_argument(\'--foo.qux\', type=int)\n\nparser.print_help()\n```\n\n```shell\nUsage: test.py [-h] [--foo.bar BAR] [--foo.baz BAZ] [--foo.qux QUX]\n\nOptional Arguments:\n  -h, --help            show this help message and exit\n\nFoo\'s Options:\n    --foo.bar BAR\n    --foo.baz BAZ\n    --foo.qux QUX\n```\n\nYou can also add a namespace action argument to take a json that can be parsed as a dict:\n\n```python\nimport argx as argparse\n\nparser = argparse.ArgumentParser()\nparser.add_argument(\'--foo\', action="namespace") # or action="ns"\nparser.add_argument(\'--foo.bar\', type=int)\nparser.add_argument(\'--foo.baz\', type=int)\nparser.add_argument(\'--foo.qux\', type=int)\n\nparser.parse_args([\'--foo\', \'{"bar": 1, "baz": 2, "qux": 3}\', \'--foo.qux\', \'4\'])\n# Namespace(foo=Namespace(bar=1, baz=2, qux=4))\n```\n\n### Brief help message for massive arguments\n\nIf you have a lot of arguments, the help message can be very long. `argx` allows to show only the most important arguments in the help message.\n\n```python\nimport argx as argparse\n\n# Advanced help options to show the brief help message or the full help message\nparser = argparse.ArgumentParser(add_help=\'+\')\nparser.add_argument(\'--foo\', type=int)\nparser.add_argument(\'--bar\', type=int, show=False)\nparser.parse_args([\'--help\'])\n```\n\n```shell\nUsage: test.py [-h] [--foo FOO]\n\nOptional Arguments:\n  -h, --help, -h+, --help+\n                        show help message (with + to show more options) and exit\n  --foo FOO\n```\n\nWith `parser.parse_args([\'--help+\'])` you can show the full help message.\n\n```shell\nUsage: test.py [-h] [--foo FOO] [--bar BAR]\n\nOptional Arguments:\n  -h, --help, -h+, --help+\n                        show help message (with + to show more options) and exit\n  --foo FOO\n  --bar BAR\n```\n\nYou can also set `show=False` for argument groups.\n\n### Default value in argument help\n\nWith `argparse`, the default value is not shown in the help message. With `argx`, the default value is added to the help message automatically.\n\n```python\nimport argx as argparse\n\nparser = argparse.ArgumentParser()\nparser.add_argument(\'--foo\', type=int, default=1)\nparser.add_argument(\'--bar\', type=int, default=2, help=\'bar [default: two]\')\nparser.add_argument(\'--baz\', type=int, default=3, help=\'baz [nodefault]\')\nparser.print_help()\n```\n\n```shell\nUsage: test.py [-h] [--foo FOO]\n\nOptional Arguments:\n  -h, --help            show help message and exit\n  --foo FOO             [default: 1]\n  --bar BAR             bar [default: two]\n  --baz BAZ             baz\n```\n\n### Newlines kept in help\n\nBy default, `argparse` replaces the newlines with spaces in the argument help message. However, sometimes you want to keep the newlines. With `argx`, if there is not newline, it is handled as the default behavior. If there is a newline, the newlines and spaces are kept.\n\n```python\nimport argx as argparse\n\nparser = argparse.ArgumentParser()\nparser.add_argument(\'--foo\', help=\'foo\\n- bar\\n  indent also kept\')\nparser.print_help()\n```\n\n```shell\nUsage: test.py [-h] [--foo FOO]\n\nOptional Arguments:\n  -h, --help            show this help message and exit\n  --foo FOO             foo\n                        - bar\n                          indent also kept\n```\n\n### Defaults from files\n\nWith standard `argparse`, when `fromfile_prefix_chars` is set, the arguments can be read from a file. The file can be specified with `@filename`. The arguments in the file are separated by newlines by default.\n\nWith `argx`, Other than a text file to provide command line arguments, you can also provide other types of configuration files. The extension of the file can be `.json`, `.yaml`, `.ini`, `.env` or `.toml`.\n\n```python\nimport argx as argparse\n\nparser = argparse.ArgumentParser()\nparser.add_argument(\'--foo\', type=int)\nparser.add_argument(\'--bar\', type=int)\nparser.add_argument(\'--baz\', type=int)\n\n# config.json\n# { "foo": 1, "bar": 2, "baz": 3 }\nargs = parser.parse_args([\'@config.json\'])\n# Namespace(foo=1, bar=2, baz=3)\n```\n\nYou can also use `set_defaults_from_configs` method:\n\n```python\nparser.set_defaults_from_configs(\'config.json\')\n```\n\n### Clear_append/extend action\n\nThe `clear_append`/`clear_extend` action is similar to `append` and `extend`, but the initial value is cleared.\n\nThis is useful when you want to accept a new list of values from the command line, instead of append/extend to the existing list or default.\n\n```python\nimport argx as argparse\n\nparser = argparse.ArgumentParser()\nparser.add_argument(\'--foo\', action=\'clear_append\', default=[1, 2, 3], type=int)\nparser.add_argument(\'--bar\', action=\'append\', default=[1, 2, 3], type=int)\n\nargs = parser.parse_args(\'--foo 4 --foo 5 --bar 4 --bar 5\'.split())\n# Namespace(foo=[4, 5], bar=[1, 2, 3, 4, 5])\n```\n\n### Grouping required arguments by default\n\nBy default, `argparse` puts both `required=True` and `required=False` arguments in the same group (optional arguments), which is sometimes confusing. `argx` groups `required=True` arguments in a separate group (required arguments).\n\n```python\nimport argx as argparse\n\nparser = argparse.ArgumentParser()\nparser.add_argument(\'--foo\')\nparser.add_argument(\'--bar\', required=True)\n\nparser.print_help()\n```\n\n```shell\nUsage: test.py [-h] [--foo FOO] --bar BAR\n\nRequired Arguments:\n  --bar BAR\n\nOptional Arguments:\n  -h, --help            show help message and exit\n  --foo FOO\n```\n\n### Order of groups in help message\n\nAllow to add an `order` attribute to groups to change the order of groups in help message\n\n```python\nimport argx as argparse\n\nparser = argparse.ArgumentParser()\ngroup1 = parser.add_argument_group(\'group1\', order=2)\ngroup1.add_argument(\'--foo\')\ngroup2 = parser.add_argument_group(\'group2\', order=1)\ngroup2.add_argument(\'--bar\')\n\nparser.print_help()\n```\n\n```shell\nUsage: test.py [-h] [--bar BAR] [--foo FOO]\n\nOptional arguments:\n  -h, --help            show help message and exit\n\nGroup2:\n  --bar BAR\n\nGroup1:\n  --foo FOO\n```\n\nThe order by default is 0. The groups with the same order are sorted by title. Groups with small numbers are displayed first. `required arguments` has a `order` of -1.\n\n### Additional types\n\n`parser.add_argument()` accepts `type` as a function to convert the argument value. It has to be a callable that accepts a single string argument and returns the converted value. While `argx` supports string for `type` so it can be configured in the configuration file. Builtin functions and types can also be specified by its name.\n\nWe also have additional types:\n\n```python\nimport argx as argparse\n\nparser = argparse.ArgumentParser()\nparser.add_argument(\'--foo\', type=\'py\')\nparser.add_argument(\'--bar\', type=\'json\')\nparser.add_argument(\'--baz\', type=\'path\')\nparser.add_argument(\'--qux\', type=\'auto\')\n\nargs = parser.parse_args(\n    \'--foo 1 --bar {"a":1} --baz path/to/file --qux true\'.split()\n)\n# Namespace(foo=1, bar={\'a\': 1}, baz=PosixPath(\'path/to/file\'), qux=True)\n```\n\n- `py`: Python expression. The string is evaluated by `ast.literal_eval`.\n- `json`: JSON string. The string is loaded by `json.loads`.\n- `path`: Path string. The string is converted by `pathlib.Path`.\n- `auto`: Automatic type conversion.\n  - `True` if the string is `True/TRUE/true`\n  - `False` if the string is `False/FALSE/false`\n  - `None` if the string is `None/NONE/none`\n  - An integer if the string can be converted to an integer\n  - A float if the string can be converted to a float\n  - A dict if the string is a JSON string\n  - The string itself otherwise\n\n### Configuration file to create the parser\n\nYou can create the parser from a configuration file.\n\n```python\nimport argx as argparse\n\n# config.json\n# {\n#   "prog": "myprog",\n#   "arguments": [ {"flags": ["-a", "--abc"], "help": "Optiona a help"} ]\n# }\nparser = argparse.ArgumentParser.from_configs(\'config.json\')\nparser.print_help()\n```\n\n```shell\nUsage: myprog [-h] [-a ABC]\n\nOptional Arguments:\n  -h, --help            show help message and exit\n  -a ABC, --abc ABC     Optiona a help\n```\n\n### Pre-parse hook\n\nYou can add a pre-parse hook to the parser. The hook is called before parsing the arguments. It can be used to modify the arguments before parsing.\n\n```python\nimport argx as argparse\n\ndef pre_parse(parser, args, namespace):\n    """We can modify the parser (i.e. add arguments)\n    the arguments to be parsed, and even manipulate the namespace.\n    """\n    parser.add_argument(\'--foo\', type=int)\n    parser.add_argument(\'--bar\', type=int)\n    namespace.baz = 2\n    return args + ["--bar", "3"]\n\nparser = argparse.ArgumentParser()\nparser.add_command(\'command1\', pre_parse=pre_parse)\nparsed = parser.parse_args(\'command1 --foo 1\'.split())\n# Namespace(COMMAND=\'command1\', baz=2, foo=1, bar=3)\n```\n\nThis is especially useful when you have a lot of subcommands and each has a lot of arguments, when it takes time to add these arguments, for example, some of the values need to be parsed from a file. Using this hook, you can add the arguments only when the subcommand is called, instead of adding them all at the beginning.\n\n### Backward compatibility\n\nAll features are optional. You can use `argx` as a drop-in replacement for `argparse`.\n\n`argx` supports python `3.7+`. Some of the later-introduced features are also supported in python 3.7. For example, `extend` action is added in python 3.8, `argx` supports in python 3.7.\n\n[1]: https://img.shields.io/pypi/v/argx.svg?style=flat-square\n[2]: https://pypi.org/project/argx/\n[3]: https://img.shields.io/github/tag/pwwang/argx.svg?style=flat-square\n[4]: https://img.shields.io/codacy/grade/c5eaafcde482437b901b1acd2b70420e.svg?style=flat-square\n[5]: https://app.codacy.com/gh/pwwang/argx/dashboard\n[6]: https://img.shields.io/codacy/coverage/c5eaafcde482437b901b1acd2b70420e.svg?style=flat-square\n[7]: https://img.shields.io/github/actions/workflow/status/pwwang/argx/build.yml?style=flat-square\n[8]: https://img.shields.io/pypi/pyversions/argx.svg?style=flat-square\n',
     'author': 'pwwang',
     'author_email': 'pwwang@pwwang.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `argx-0.2.8/PKG-INFO` & `argx-0.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: argx
-Version: 0.2.8
+Version: 0.2.9
 Summary: Super-charged argparse for python
 License: MIT
 Author: pwwang
 Author-email: pwwang@pwwang.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: python-simpleconf (>=0.5.7,<0.6.0)
+Requires-Dist: python-simpleconf (>=0.6,<0.7)
 Description-Content-Type: text/markdown
 
 # argx
 
 [![pypi][1]][2] [![tag][3]][2] [![codacy quality][4]][5] [![codacy quality][6]][5] ![github action][7] ![pyver][8]
 
 Supercharged argparse for Python
```

