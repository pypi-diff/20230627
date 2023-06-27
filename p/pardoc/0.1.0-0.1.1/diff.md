# Comparing `tmp/pardoc-0.1.0.tar.gz` & `tmp/pardoc-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pardoc-0.1.0.tar", max compression
+gzip compressed data, was "pardoc-0.1.1.tar", max compression
```

## Comparing `pardoc-0.1.0.tar` & `pardoc-0.1.1.tar`

### file list

```diff
@@ -1,11 +1,10 @@
--rw-r--r--   0        0        0     1063 2022-09-19 22:07:16.670332 pardoc-0.1.0/LICENSE
--rw-r--r--   0        0        0     7061 2022-09-19 22:07:16.670332 pardoc-0.1.0/README.md
--rw-r--r--   0        0        0      856 2022-09-19 22:07:16.670332 pardoc-0.1.0/pardoc/__init__.py
--rw-r--r--   0        0        0    16574 2022-09-19 22:07:16.670332 pardoc-0.1.0/pardoc/default.py
--rw-r--r--   0        0        0     3875 2022-09-19 22:07:16.670332 pardoc-0.1.0/pardoc/google.py
--rw-r--r--   0        0        0     5662 2022-09-19 22:07:16.670332 pardoc-0.1.0/pardoc/liquidpy.py
--rw-r--r--   0        0        0     4758 2022-09-19 22:07:16.670332 pardoc-0.1.0/pardoc/numpy.py
--rw-r--r--   0        0        0     3037 2022-09-19 22:07:16.670332 pardoc-0.1.0/pardoc/parsed.py
--rw-r--r--   0        0        0      870 2022-09-19 22:07:16.670332 pardoc-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     8007 1970-01-01 00:00:00.000000 pardoc-0.1.0/setup.py
--rw-r--r--   0        0        0     7771 1970-01-01 00:00:00.000000 pardoc-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-06-27 01:26:20.776112 pardoc-0.1.1/LICENSE
+-rw-r--r--   0        0        0     7061 2023-06-27 01:26:20.776112 pardoc-0.1.1/README.md
+-rw-r--r--   0        0        0      856 2023-06-27 01:26:20.776112 pardoc-0.1.1/pardoc/__init__.py
+-rw-r--r--   0        0        0    16574 2023-06-27 01:26:20.776112 pardoc-0.1.1/pardoc/default.py
+-rw-r--r--   0        0        0     3875 2023-06-27 01:26:20.776112 pardoc-0.1.1/pardoc/google.py
+-rw-r--r--   0        0        0     5662 2023-06-27 01:26:20.776112 pardoc-0.1.1/pardoc/liquidpy.py
+-rw-r--r--   0        0        0     4758 2023-06-27 01:26:20.776112 pardoc-0.1.1/pardoc/numpy.py
+-rw-r--r--   0        0        0     3037 2023-06-27 01:26:20.776112 pardoc-0.1.1/pardoc/parsed.py
+-rw-r--r--   0        0        0      868 2023-06-27 01:26:20.776112 pardoc-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     7818 1970-01-01 00:00:00.000000 pardoc-0.1.1/PKG-INFO
```

### Comparing `pardoc-0.1.0/LICENSE` & `pardoc-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pardoc-0.1.0/README.md` & `pardoc-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `pardoc-0.1.0/pardoc/__init__.py` & `pardoc-0.1.1/pardoc/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Yet another docstring parser"""
 from lark.exceptions import LarkError
 from .google import google_parser
 from .liquidpy import liquidpy_parser
 from .numpy import numpy_parser
 from .parsed import pretty
 
-__version__ = "0.1.0"
+__version__ = "0.1.1"
 
 
 def auto_parser(docstring):
     """Try to get a proper parser for the given docstring
 
     Args:
         docstring (str): The docstring to test for parser
```

### Comparing `pardoc-0.1.0/pardoc/default.py` & `pardoc-0.1.1/pardoc/default.py`

 * *Files identical despite different names*

### Comparing `pardoc-0.1.0/pardoc/google.py` & `pardoc-0.1.1/pardoc/google.py`

 * *Files identical despite different names*

### Comparing `pardoc-0.1.0/pardoc/liquidpy.py` & `pardoc-0.1.1/pardoc/liquidpy.py`

 * *Files identical despite different names*

### Comparing `pardoc-0.1.0/pardoc/numpy.py` & `pardoc-0.1.1/pardoc/numpy.py`

 * *Files identical despite different names*

### Comparing `pardoc-0.1.0/pardoc/parsed.py` & `pardoc-0.1.1/pardoc/parsed.py`

 * *Files identical despite different names*

### Comparing `pardoc-0.1.0/pyproject.toml` & `pardoc-0.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [build-system]
 requires = [ "poetry>=0.12",]
 build-backend = "poetry.masonry.api"
 
 [tool.poetry]
 name = "pardoc"
-version = "0.1.0"
+version = "0.1.1"
 description = "Yet another docstring parser for python"
 authors = [ "pwwang <pwwang@pwwang.com>",]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/pwwang/pardoc"
 repository = "https://github.com/pwwang/pardoc"
 
 [tool.poetry.dependencies]
 python = "^3.7"
 lark-parser = "^0.12"
-diot = "^0.1.6"
+diot = "^0.2"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7"
 pytest-cov = "^3"
 flake8 = "^4"
 
 [tool.pytest.ini_options]
```

### Comparing `pardoc-0.1.0/setup.py` & `pardoc-0.1.1/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,30 +1,253 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: pardoc
+Version: 0.1.1
+Summary: Yet another docstring parser for python
+Home-page: https://github.com/pwwang/pardoc
+License: MIT
+Author: pwwang
+Author-email: pwwang@pwwang.com
+Requires-Python: >=3.7,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: diot (>=0.2,<0.3)
+Requires-Dist: lark-parser (>=0.12,<0.13)
+Project-URL: Repository, https://github.com/pwwang/pardoc
+Description-Content-Type: text/markdown
+
+# pardoc
+
+[![pypi][3]][4] [![tag][5]][6] ![pyver][12] [![build][7]][8] [![codacy quality][9]][10] [![codacy quality][11]][10]
+
+Yet another docstring parser for python, using [`lark-parser`][1]
+
+## Installation
+
+```python
+pip install pardoc
+```
+
+## A quick look
+
+```python console
+>>> from pardoc import google_parser, pretty
+
+>>> docstring = """This is an example of a module level function.
+
+Function parameters should be documented in the ``Args`` section. The name
+of each parameter is required. The type and description of each parameter
+is optional, but should be included if not obvious.
+
+If \*args or \*\*kwargs are accepted,
+they should be listed as ``*args`` and ``**kwargs``.
+
+The format for a parameter is::
+
+    name (type): description
+        The description may span multiple lines. Following
+        lines should be indented. The "(type)" is optional.
+
+        Multiple paragraphs are supported in parameter
+        descriptions.
+
+Args:
+    param1 (int): The first parameter.
+    param2 (:obj:`str`, optional): The second parameter. Defaults to None.
+        Second line of description should be indented.
+    *args: Variable length argument list.
+    **kwargs: Arbitrary keyword arguments.
+
+Returns:
+    bool: True if successful, False otherwise.
+
+    The return type is optional and may be specified at the beginning of
+    the ``Returns`` section followed by a colon.
+
+    The ``Returns`` section may span multiple lines and paragraphs.
+    Following lines should be indented to match the first line.
+
+    The ``Returns`` section supports any reStructuredText formatting,
+    including literal blocks::
+
+        {
+            'param1': param1,
+            'param2': param2
+        }
+
+Raises:
+    AttributeError: The ``Raises`` section is a list of all exceptions
+        that are relevant to the interface.
+    ValueError: If `param2` is equal to `param1`.
+
+"""
+
+>>> parsed = google_parser.parse(docstring)
+>>> pretty(parsed, print_=True)
+
+ParsedSection(title=SUMMARY)
+   ParsedPara(lines=1)
+      This is an example of a module level function.
+   ParsedPara(lines=3)
+      Function parameters should be documented in the ``Args`` section. The name
+      of each parameter is required. The type and description of each parameter
+      is optional, but should be included if not obvious.
+   ParsedPara(lines=2)
+      If \*args or \*\*kwargs are accepted,
+      they should be listed as ``*args`` and ``**kwargs``.
+   ParsedPara(lines=1)
+      The format for a parameter is::
+   ParsedPara(lines=2)
+      ParsedPara(lines=1)
+         name (type): description
+      ParsedPara(lines=2)
+         ParsedPara(lines=2)
+            The description may span multiple lines. Following
+            lines should be indented. The "(type)" is optional.
+         ParsedPara(lines=2)
+            Multiple paragraphs are supported in parameter
+            descriptions.
+
+ParsedSection(title=Args)
+   ParsedItem(name=param1, type=int, desc=The first parameter.)
+   ParsedItem(name=param2, type=:obj:`str`, optional, desc=The second parameter. Defaults to None.)
+      ParsedPara(lines=1)
+         Second line of description should be indented.
+   ParsedItem(name=*args, type=None, desc=Variable length argument list.)
+   ParsedItem(name=**kwargs, type=None, desc=Arbitrary keyword arguments.)
+
+ParsedSection(title=Returns)
+   ParsedItem(name=bool, type=None, desc=True if successful, False otherwise.)
+   ParsedPara(lines=2)
+      The return type is optional and may be specified at the beginning of
+      the ``Returns`` section followed by a colon.
+   ParsedPara(lines=2)
+      The ``Returns`` section may span multiple lines and paragraphs.
+      Following lines should be indented to match the first line.
+   ParsedPara(lines=2)
+      The ``Returns`` section supports any reStructuredText formatting,
+      including literal blocks::
+   ParsedPara(lines=2)
+      ParsedPara(lines=1)
+         {
+      ParsedPara(lines=1)
+         ParsedPara(lines=2)
+            'param1': param1,
+            'param2': param2
+   ParsedPara(lines=1)
+      ParsedPara(lines=1)
+         }
+
+ParsedSection(title=Raises)
+   ParsedItem(name=AttributeError, type=None, desc=The ``Raises`` section is a list of all exceptions)
+      ParsedPara(lines=1)
+         that are relevant to the interface.
+   ParsedItem(name=ValueError, type=None, desc=If `param2` is equal to `param1`.)
+
+```
+
+## Usage
+
+### Parsing a known style docstring
+
+```python
+from pardoc import google_parser, numpy_parser
+parsed = google_parser(docstring)
+# or
+parsed = numpy_parser(docstring)
+```
+
+### Parsing an unknown style docstring
+
+```python
+from pardoc import auto_parser
+
+parser = auto_parser(docstring)
+# parsing results from auto_parser is cached and reused.
+parsed = parser.parse(docstring)
+```
+
+### Parsed object
+
+There are 6 types of parsed objects, include the final `Parsed` object that
+attaches all sections
+
+The first 5 are all `namedtuple`s:
+
+```python
+ParsedItem = namedtuple('ParsedItem',
+                        ['name', 'type', 'desc', 'more'])
+ParsedTodo = namedtuple('ParsedTodo', ['todo', 'more'])
+ParsedSection = namedtuple('ParsedSection', ['title', 'section'])
+ParsedPara = namedtuple('ParsedPara', ['lines'])
+ParsedCode = namedtuple('ParsedCode', ['lang', 'codes'])
+
+```
+
+The `Parsed` is an ordered dictionary (`OrderedDiot`) from [`diot`][2], which
+allows dot access to keys:
+
+```python
+from diot import OrderedDiot
+
+class Parsed(OrderedDiot):
+    """Parsed object"""
+```
+
+### Formatting a parsed object to the original style
+
+```python console
+>>> from pardoc import google_parser
+>>> docstring = """Example function with types documented in the docstring.
+
+
+Args:
+
+
+    param0: No type
+
+    param1 (int): The first parameter.
+    param2 (str): The second parameter.
+
+Returns:
+
+
+    bool: The return value. True for success, False otherwise.
+
+"""
+>>> # note the arbitrary empty lines
+>>> reformatted = google_parser.format(docstring)
+>>> # or
+>>> reformatted = google_parser.format(google_parser.parse(docstring))
+>>> print(reformatted)
+Example function with types documented in the docstring.
+
+Args:
+    param0: No type
+    param1 (int): The first parameter.
+    param2 (str): The second parameter.
+
+Returns:
+    bool: The return value. True for success, False otherwise.
+```
+
+### Pretty printing the parsed objects
+
+See `A quick look`
+
+[1]: https://github.com/lark-parser/lark
+[2]: https://github.com/pwwang/diot
+[3]: https://img.shields.io/pypi/v/pardoc?style=flat-square
+[4]: https://pypi.org/project/pardoc/
+[5]: https://img.shields.io/github/tag/pwwang/pardoc?style=flat-square
+[6]: https://github.com/pwwang/pardoc
+[7]: https://img.shields.io/github/workflow/status/pwwang/pardoc/Build%20and%20Deploy?style=flat-square
+[8]: https://github.com/pwwang/pardoc
+[9]: https://img.shields.io/codacy/grade/a1ba6573a5fa4fc589ce3cf7daa5ddea?style=flat-square
+[10]: https://app.codacy.com/project/pwwang/pardoc/dashboard
+[11]: https://img.shields.io/codacy/coverage/a1ba6573a5fa4fc589ce3cf7daa5ddea?style=flat-square
+[12]: https://img.shields.io/pypi/pyversions/pardoc?style=flat-square
 
-packages = \
-['pardoc']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['diot>=0.1.6,<0.2.0', 'lark-parser>=0.12,<0.13']
-
-setup_kwargs = {
-    'name': 'pardoc',
-    'version': '0.1.0',
-    'description': 'Yet another docstring parser for python',
-    'long_description': '# pardoc\n\n[![pypi][3]][4] [![tag][5]][6] ![pyver][12] [![build][7]][8] [![codacy quality][9]][10] [![codacy quality][11]][10]\n\nYet another docstring parser for python, using [`lark-parser`][1]\n\n## Installation\n\n```python\npip install pardoc\n```\n\n## A quick look\n\n```python console\n>>> from pardoc import google_parser, pretty\n\n>>> docstring = """This is an example of a module level function.\n\nFunction parameters should be documented in the ``Args`` section. The name\nof each parameter is required. The type and description of each parameter\nis optional, but should be included if not obvious.\n\nIf \\*args or \\*\\*kwargs are accepted,\nthey should be listed as ``*args`` and ``**kwargs``.\n\nThe format for a parameter is::\n\n    name (type): description\n        The description may span multiple lines. Following\n        lines should be indented. The "(type)" is optional.\n\n        Multiple paragraphs are supported in parameter\n        descriptions.\n\nArgs:\n    param1 (int): The first parameter.\n    param2 (:obj:`str`, optional): The second parameter. Defaults to None.\n        Second line of description should be indented.\n    *args: Variable length argument list.\n    **kwargs: Arbitrary keyword arguments.\n\nReturns:\n    bool: True if successful, False otherwise.\n\n    The return type is optional and may be specified at the beginning of\n    the ``Returns`` section followed by a colon.\n\n    The ``Returns`` section may span multiple lines and paragraphs.\n    Following lines should be indented to match the first line.\n\n    The ``Returns`` section supports any reStructuredText formatting,\n    including literal blocks::\n\n        {\n            \'param1\': param1,\n            \'param2\': param2\n        }\n\nRaises:\n    AttributeError: The ``Raises`` section is a list of all exceptions\n        that are relevant to the interface.\n    ValueError: If `param2` is equal to `param1`.\n\n"""\n\n>>> parsed = google_parser.parse(docstring)\n>>> pretty(parsed, print_=True)\n\nParsedSection(title=SUMMARY)\n   ParsedPara(lines=1)\n      This is an example of a module level function.\n   ParsedPara(lines=3)\n      Function parameters should be documented in the ``Args`` section. The name\n      of each parameter is required. The type and description of each parameter\n      is optional, but should be included if not obvious.\n   ParsedPara(lines=2)\n      If \\*args or \\*\\*kwargs are accepted,\n      they should be listed as ``*args`` and ``**kwargs``.\n   ParsedPara(lines=1)\n      The format for a parameter is::\n   ParsedPara(lines=2)\n      ParsedPara(lines=1)\n         name (type): description\n      ParsedPara(lines=2)\n         ParsedPara(lines=2)\n            The description may span multiple lines. Following\n            lines should be indented. The "(type)" is optional.\n         ParsedPara(lines=2)\n            Multiple paragraphs are supported in parameter\n            descriptions.\n\nParsedSection(title=Args)\n   ParsedItem(name=param1, type=int, desc=The first parameter.)\n   ParsedItem(name=param2, type=:obj:`str`, optional, desc=The second parameter. Defaults to None.)\n      ParsedPara(lines=1)\n         Second line of description should be indented.\n   ParsedItem(name=*args, type=None, desc=Variable length argument list.)\n   ParsedItem(name=**kwargs, type=None, desc=Arbitrary keyword arguments.)\n\nParsedSection(title=Returns)\n   ParsedItem(name=bool, type=None, desc=True if successful, False otherwise.)\n   ParsedPara(lines=2)\n      The return type is optional and may be specified at the beginning of\n      the ``Returns`` section followed by a colon.\n   ParsedPara(lines=2)\n      The ``Returns`` section may span multiple lines and paragraphs.\n      Following lines should be indented to match the first line.\n   ParsedPara(lines=2)\n      The ``Returns`` section supports any reStructuredText formatting,\n      including literal blocks::\n   ParsedPara(lines=2)\n      ParsedPara(lines=1)\n         {\n      ParsedPara(lines=1)\n         ParsedPara(lines=2)\n            \'param1\': param1,\n            \'param2\': param2\n   ParsedPara(lines=1)\n      ParsedPara(lines=1)\n         }\n\nParsedSection(title=Raises)\n   ParsedItem(name=AttributeError, type=None, desc=The ``Raises`` section is a list of all exceptions)\n      ParsedPara(lines=1)\n         that are relevant to the interface.\n   ParsedItem(name=ValueError, type=None, desc=If `param2` is equal to `param1`.)\n\n```\n\n## Usage\n\n### Parsing a known style docstring\n\n```python\nfrom pardoc import google_parser, numpy_parser\nparsed = google_parser(docstring)\n# or\nparsed = numpy_parser(docstring)\n```\n\n### Parsing an unknown style docstring\n\n```python\nfrom pardoc import auto_parser\n\nparser = auto_parser(docstring)\n# parsing results from auto_parser is cached and reused.\nparsed = parser.parse(docstring)\n```\n\n### Parsed object\n\nThere are 6 types of parsed objects, include the final `Parsed` object that\nattaches all sections\n\nThe first 5 are all `namedtuple`s:\n\n```python\nParsedItem = namedtuple(\'ParsedItem\',\n                        [\'name\', \'type\', \'desc\', \'more\'])\nParsedTodo = namedtuple(\'ParsedTodo\', [\'todo\', \'more\'])\nParsedSection = namedtuple(\'ParsedSection\', [\'title\', \'section\'])\nParsedPara = namedtuple(\'ParsedPara\', [\'lines\'])\nParsedCode = namedtuple(\'ParsedCode\', [\'lang\', \'codes\'])\n\n```\n\nThe `Parsed` is an ordered dictionary (`OrderedDiot`) from [`diot`][2], which\nallows dot access to keys:\n\n```python\nfrom diot import OrderedDiot\n\nclass Parsed(OrderedDiot):\n    """Parsed object"""\n```\n\n### Formatting a parsed object to the original style\n\n```python console\n>>> from pardoc import google_parser\n>>> docstring = """Example function with types documented in the docstring.\n\n\nArgs:\n\n\n    param0: No type\n\n    param1 (int): The first parameter.\n    param2 (str): The second parameter.\n\nReturns:\n\n\n    bool: The return value. True for success, False otherwise.\n\n"""\n>>> # note the arbitrary empty lines\n>>> reformatted = google_parser.format(docstring)\n>>> # or\n>>> reformatted = google_parser.format(google_parser.parse(docstring))\n>>> print(reformatted)\nExample function with types documented in the docstring.\n\nArgs:\n    param0: No type\n    param1 (int): The first parameter.\n    param2 (str): The second parameter.\n\nReturns:\n    bool: The return value. True for success, False otherwise.\n```\n\n### Pretty printing the parsed objects\n\nSee `A quick look`\n\n[1]: https://github.com/lark-parser/lark\n[2]: https://github.com/pwwang/diot\n[3]: https://img.shields.io/pypi/v/pardoc?style=flat-square\n[4]: https://pypi.org/project/pardoc/\n[5]: https://img.shields.io/github/tag/pwwang/pardoc?style=flat-square\n[6]: https://github.com/pwwang/pardoc\n[7]: https://img.shields.io/github/workflow/status/pwwang/pardoc/Build%20and%20Deploy?style=flat-square\n[8]: https://github.com/pwwang/pardoc\n[9]: https://img.shields.io/codacy/grade/a1ba6573a5fa4fc589ce3cf7daa5ddea?style=flat-square\n[10]: https://app.codacy.com/project/pwwang/pardoc/dashboard\n[11]: https://img.shields.io/codacy/coverage/a1ba6573a5fa4fc589ce3cf7daa5ddea?style=flat-square\n[12]: https://img.shields.io/pypi/pyversions/pardoc?style=flat-square\n',
-    'author': 'pwwang',
-    'author_email': 'pwwang@pwwang.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/pwwang/pardoc',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.7,<4.0',
-}
-
-
-setup(**setup_kwargs)
```

