# Comparing `tmp/pyastgrep-1.2.1.tar.gz` & `tmp/pyastgrep-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyastgrep-1.2.1.tar", last modified: Thu Jun 22 10:05:01 2023, max compression
+gzip compressed data, was "pyastgrep-1.2.2.tar", last modified: Tue Jun 27 15:41:42 2023, max compression
```

## Comparing `pyastgrep-1.2.1.tar` & `pyastgrep-1.2.2.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxrwx   0 luke      (1000) luke      (1000)        0 2023-06-22 10:05:01.003704 pyastgrep-1.2.1/
--rw-r--r--   0 luke      (1000) luke      (1000)      378 2022-10-17 13:09:58.000000 pyastgrep-1.2.1/.gitattributes
--rw-r--r--   0 luke      (1000) luke      (1000)     1771 2022-11-07 12:01:43.000000 pyastgrep-1.2.1/.gitignore
--rw-rw-rw-   0 luke      (1000) luke      (1000)    15393 2023-06-22 10:05:01.003704 pyastgrep-1.2.1/PKG-INFO
--rw-r--r--   0 luke      (1000) luke      (1000)    14571 2023-06-21 20:21:15.000000 pyastgrep-1.2.1/README.rst
--rw-r--r--   0 luke      (1000) luke      (1000)      755 2023-04-17 15:02:16.000000 pyastgrep-1.2.1/pyproject.toml
--rw-r--r--   0 luke      (1000) luke      (1000)     1120 2023-06-22 10:05:01.003704 pyastgrep-1.2.1/setup.cfg
--rw-r--r--   0 luke      (1000) luke      (1000)       38 2022-10-21 16:01:47.000000 pyastgrep-1.2.1/setup.py
-drwxrwxrwx   0 luke      (1000) luke      (1000)        0 2023-06-22 10:05:00.995704 pyastgrep-1.2.1/src/
-drwxrwxrwx   0 luke      (1000) luke      (1000)        0 2023-06-22 10:05:00.999704 pyastgrep-1.2.1/src/pyastgrep/
--rw-r--r--   0 luke      (1000) luke      (1000)       22 2023-06-22 09:55:35.000000 pyastgrep-1.2.1/src/pyastgrep/__init__.py
--rw-r--r--   0 luke      (1000) luke      (1000)     1854 2023-06-22 08:42:51.000000 pyastgrep-1.2.1/src/pyastgrep/ast_utils.py
--rw-r--r--   0 luke      (1000) luke      (1000)     3158 2022-11-18 11:57:27.000000 pyastgrep-1.2.1/src/pyastgrep/asts.py
--rw-r--r--   0 luke      (1000) luke      (1000)     6631 2023-06-22 09:20:15.000000 pyastgrep-1.2.1/src/pyastgrep/cli.py
--rw-r--r--   0 luke      (1000) luke      (1000)     1273 2023-06-22 09:46:09.000000 pyastgrep-1.2.1/src/pyastgrep/context.py
--rw-r--r--   0 luke      (1000) luke      (1000)      890 2022-11-25 07:36:32.000000 pyastgrep-1.2.1/src/pyastgrep/dump.py
--rw-r--r--   0 luke      (1000) luke      (1000)     4097 2023-06-21 12:33:14.000000 pyastgrep-1.2.1/src/pyastgrep/files.py
--rw-r--r--   0 luke      (1000) luke      (1000)    10840 2023-06-21 10:04:58.000000 pyastgrep-1.2.1/src/pyastgrep/ignores.py
--rw-r--r--   0 luke      (1000) luke      (1000)    10566 2023-06-22 09:21:14.000000 pyastgrep-1.2.1/src/pyastgrep/printer.py
--rw-r--r--   0 luke      (1000) luke      (1000)     4801 2023-06-21 18:07:13.000000 pyastgrep-1.2.1/src/pyastgrep/search.py
--rw-r--r--   0 luke      (1000) luke      (1000)      696 2022-11-14 14:54:35.000000 pyastgrep-1.2.1/src/pyastgrep/xml.py
--rw-r--r--   0 luke      (1000) luke      (1000)      366 2022-11-06 20:21:35.000000 pyastgrep-1.2.1/src/pyastgrep/xpath2.py
-drwxrwxrwx   0 luke      (1000) luke      (1000)        0 2023-06-22 10:05:00.999704 pyastgrep-1.2.1/src/pyastgrep.egg-info/
--rw-r-----   0 luke      (1000) luke      (1000)    15393 2023-06-22 10:05:00.000000 pyastgrep-1.2.1/src/pyastgrep.egg-info/PKG-INFO
--rw-r-----   0 luke      (1000) luke      (1000)      750 2023-06-22 10:05:00.000000 pyastgrep-1.2.1/src/pyastgrep.egg-info/SOURCES.txt
--rw-r-----   0 luke      (1000) luke      (1000)        1 2023-06-22 10:05:00.000000 pyastgrep-1.2.1/src/pyastgrep.egg-info/dependency_links.txt
--rw-r-----   0 luke      (1000) luke      (1000)       81 2023-06-22 10:05:00.000000 pyastgrep-1.2.1/src/pyastgrep.egg-info/entry_points.txt
--rw-r-----   0 luke      (1000) luke      (1000)       58 2023-06-22 10:05:00.000000 pyastgrep-1.2.1/src/pyastgrep.egg-info/requires.txt
--rw-r-----   0 luke      (1000) luke      (1000)       10 2023-06-22 10:05:00.000000 pyastgrep-1.2.1/src/pyastgrep.egg-info/top_level.txt
-drwxrwxrwx   0 luke      (1000) luke      (1000)        0 2023-06-22 10:05:01.003704 pyastgrep-1.2.1/tests/
--rw-r--r--   0 luke      (1000) luke      (1000)     6529 2023-06-21 08:40:28.000000 pyastgrep-1.2.1/tests/test_cli.py
--rw-r--r--   0 luke      (1000) luke      (1000)      733 2022-11-06 19:59:49.000000 pyastgrep-1.2.1/tests/test_encodings.py
--rw-r--r--   0 luke      (1000) luke      (1000)      648 2022-11-07 12:52:05.000000 pyastgrep-1.2.1/tests/test_errors.py
--rw-r--r--   0 luke      (1000) luke      (1000)     5325 2023-06-21 09:44:46.000000 pyastgrep-1.2.1/tests/test_ignores.py
--rw-r--r--   0 luke      (1000) luke      (1000)      449 2022-11-25 08:08:17.000000 pyastgrep-1.2.1/tests/test_parsing.py
--rw-r--r--   0 luke      (1000) luke      (1000)     7058 2023-06-22 09:50:58.000000 pyastgrep-1.2.1/tests/test_printing.py
--rw-r--r--   0 luke      (1000) luke      (1000)      410 2023-02-20 15:45:50.000000 pyastgrep-1.2.1/tests/test_symlinks.py
--rw-r--r--   0 luke      (1000) luke      (1000)     1560 2023-06-21 09:04:52.000000 pyastgrep-1.2.1/tests/test_xml.py
+drwxrwxrwx   0 luke      (1000) luke      (1000)        0 2023-06-27 15:41:42.811281 pyastgrep-1.2.2/
+-rw-r--r--   0 luke      (1000) luke      (1000)      378 2022-10-17 13:09:58.000000 pyastgrep-1.2.2/.gitattributes
+-rw-r--r--   0 luke      (1000) luke      (1000)     1771 2022-11-07 12:01:43.000000 pyastgrep-1.2.2/.gitignore
+-rw-rw-rw-   0 luke      (1000) luke      (1000)    15748 2023-06-27 15:41:42.811281 pyastgrep-1.2.2/PKG-INFO
+-rw-r--r--   0 luke      (1000) luke      (1000)    14926 2023-06-22 18:47:11.000000 pyastgrep-1.2.2/README.rst
+-rw-r--r--   0 luke      (1000) luke      (1000)      755 2023-04-17 15:02:16.000000 pyastgrep-1.2.2/pyproject.toml
+-rw-r--r--   0 luke      (1000) luke      (1000)     1120 2023-06-27 15:41:42.815281 pyastgrep-1.2.2/setup.cfg
+-rw-r--r--   0 luke      (1000) luke      (1000)       38 2022-10-21 16:01:47.000000 pyastgrep-1.2.2/setup.py
+drwxrwxrwx   0 luke      (1000) luke      (1000)        0 2023-06-27 15:41:42.803281 pyastgrep-1.2.2/src/
+drwxrwxrwx   0 luke      (1000) luke      (1000)        0 2023-06-27 15:41:42.807281 pyastgrep-1.2.2/src/pyastgrep/
+-rw-r--r--   0 luke      (1000) luke      (1000)       22 2023-06-27 15:38:08.000000 pyastgrep-1.2.2/src/pyastgrep/__init__.py
+-rw-r--r--   0 luke      (1000) luke      (1000)     1854 2023-06-22 08:42:51.000000 pyastgrep-1.2.2/src/pyastgrep/ast_utils.py
+-rw-r--r--   0 luke      (1000) luke      (1000)     3851 2023-06-27 07:16:37.000000 pyastgrep-1.2.2/src/pyastgrep/asts.py
+-rw-r--r--   0 luke      (1000) luke      (1000)     6555 2023-06-26 13:47:54.000000 pyastgrep-1.2.2/src/pyastgrep/cli.py
+-rw-r--r--   0 luke      (1000) luke      (1000)     1273 2023-06-22 09:46:09.000000 pyastgrep-1.2.2/src/pyastgrep/context.py
+-rw-r--r--   0 luke      (1000) luke      (1000)      890 2022-11-25 07:36:32.000000 pyastgrep-1.2.2/src/pyastgrep/dump.py
+-rw-r--r--   0 luke      (1000) luke      (1000)     4037 2023-06-26 13:47:54.000000 pyastgrep-1.2.2/src/pyastgrep/files.py
+-rw-r--r--   0 luke      (1000) luke      (1000)    10840 2023-06-21 10:04:58.000000 pyastgrep-1.2.2/src/pyastgrep/ignores.py
+-rw-r--r--   0 luke      (1000) luke      (1000)    10566 2023-06-22 09:21:14.000000 pyastgrep-1.2.2/src/pyastgrep/printer.py
+-rw-r--r--   0 luke      (1000) luke      (1000)     4563 2023-06-26 14:10:33.000000 pyastgrep-1.2.2/src/pyastgrep/search.py
+-rw-r--r--   0 luke      (1000) luke      (1000)      696 2022-11-14 14:54:35.000000 pyastgrep-1.2.2/src/pyastgrep/xml.py
+-rw-r--r--   0 luke      (1000) luke      (1000)      366 2022-11-06 20:21:35.000000 pyastgrep-1.2.2/src/pyastgrep/xpath2.py
+drwxrwxrwx   0 luke      (1000) luke      (1000)        0 2023-06-27 15:41:42.807281 pyastgrep-1.2.2/src/pyastgrep.egg-info/
+-rw-r-----   0 luke      (1000) luke      (1000)    15748 2023-06-27 15:41:42.000000 pyastgrep-1.2.2/src/pyastgrep.egg-info/PKG-INFO
+-rw-r-----   0 luke      (1000) luke      (1000)      750 2023-06-27 15:41:42.000000 pyastgrep-1.2.2/src/pyastgrep.egg-info/SOURCES.txt
+-rw-r-----   0 luke      (1000) luke      (1000)        1 2023-06-27 15:41:42.000000 pyastgrep-1.2.2/src/pyastgrep.egg-info/dependency_links.txt
+-rw-r-----   0 luke      (1000) luke      (1000)       81 2023-06-27 15:41:42.000000 pyastgrep-1.2.2/src/pyastgrep.egg-info/entry_points.txt
+-rw-r-----   0 luke      (1000) luke      (1000)       58 2023-06-27 15:41:42.000000 pyastgrep-1.2.2/src/pyastgrep.egg-info/requires.txt
+-rw-r-----   0 luke      (1000) luke      (1000)       10 2023-06-27 15:41:42.000000 pyastgrep-1.2.2/src/pyastgrep.egg-info/top_level.txt
+drwxrwxrwx   0 luke      (1000) luke      (1000)        0 2023-06-27 15:41:42.811281 pyastgrep-1.2.2/tests/
+-rw-r--r--   0 luke      (1000) luke      (1000)     6529 2023-06-21 08:40:28.000000 pyastgrep-1.2.2/tests/test_cli.py
+-rw-r--r--   0 luke      (1000) luke      (1000)     1558 2023-06-26 19:56:42.000000 pyastgrep-1.2.2/tests/test_encodings.py
+-rw-r--r--   0 luke      (1000) luke      (1000)      648 2022-11-07 12:52:05.000000 pyastgrep-1.2.2/tests/test_errors.py
+-rw-r--r--   0 luke      (1000) luke      (1000)     5325 2023-06-21 09:44:46.000000 pyastgrep-1.2.2/tests/test_ignores.py
+-rw-r--r--   0 luke      (1000) luke      (1000)      449 2022-11-25 08:08:17.000000 pyastgrep-1.2.2/tests/test_parsing.py
+-rw-r--r--   0 luke      (1000) luke      (1000)     7058 2023-06-22 09:50:58.000000 pyastgrep-1.2.2/tests/test_printing.py
+-rw-r--r--   0 luke      (1000) luke      (1000)      410 2023-02-20 15:45:50.000000 pyastgrep-1.2.2/tests/test_symlinks.py
+-rw-r--r--   0 luke      (1000) luke      (1000)    12211 2023-06-27 07:05:06.000000 pyastgrep-1.2.2/tests/test_xml.py
```

### Comparing `pyastgrep-1.2.1/.gitignore` & `pyastgrep-1.2.2/.gitignore`

 * *Files identical despite different names*

### Comparing `pyastgrep-1.2.1/PKG-INFO` & `pyastgrep-1.2.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyastgrep
-Version: 1.2.1
+Version: 1.2.2
 Summary: A query tool for Python abstract syntax trees
 Home-page: https://github.com/spookylukey/pyastgrep
 Author: Luke Plant
 License: MIT
 Keywords: xpath xml ast asts syntax query css grep
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
@@ -142,15 +142,15 @@
 Usages of a function called ``open``:
 
 .. code:: bash
 
    $ pyastgrep './/Call/func/Name[@id="open"]'
    src/pyastgrep/search.py:88:18:            with open(path) as f:
 
-Literal numbers (Python 3.8+):
+Literal numbers:
 
 .. code:: bash
 
    $ pyastgrep './/Constant[@type="int" or @type="float"]'
    tests/examples/test_xml/everything.py:5:20:    assigned_int = 123
    tests/examples/test_xml/everything.py:6:22:    assigned_float = 3.14
 
@@ -373,39 +373,48 @@
 a ``target`` node that is a parent of a ``Name`` node with attribute ``id``
 equal to ``"foo"``:
 
 .. code:: bash
 
    $ pyastgrep './/Assign[./targets//Name[@id="foo"]]' --xml
 
-Limitations
------------
+Limitations and other tools
+---------------------------
 
 pyastgrep is useful for grepping Python code at a fairly low level. It can be
 used for various refactoring or linting tasks. Some linting tasks require higher
 level understanding of a code base. For example, to detect use of a certain
 function, you need to cope with various ways that the function may be imported
 and used, and avoid detecting a function with the same name but from a different
 module. For these kinds of tasks, you might be interested in:
 
 * `Semgrep <https://semgrep.dev/>`_
 * `Fixit <https://github.com/Instagram/Fixit>`_
 
+
+If you are looking for something simpler, try:
+
+* Simon Willison’s `symbex <https://github.com/simonw/symbex/>`_ which can
+  extract functions/methods/classes.
+
 If you are using this as a library, you should note that while AST works well
 for linting, it’s not as good for rewriting code, because AST does not contain
 or preserve things like formatting and comments. For a better approach, have a
 look at `libCST <https://github.com/Instagram/LibCST>`_.
 
 
 Use as a library
 ----------------
 
-pyastgrep is structured internally to make it easy to use a library as well as
-a CLI. However, while we will try not to break things without good reason, at this
-point we are not documenting or guaranteeing API stability for these functions.
+pyastgrep is structured internally to make it easy to use as a library as well
+as a CLI, with a clear separation of the different layers. However, while we
+will try not to break things without good reason, at this point we are not
+documenting or guaranteeing API stability for these functions. Please contribute
+to `the discussion <https://github.com/spookylukey/pyastgrep/discussions/18>`_
+if you have needs here.
 
 Editor integration
 ------------------
 
 Emacs
 ~~~~~
```

### Comparing `pyastgrep-1.2.1/README.rst` & `pyastgrep-1.2.2/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -120,15 +120,15 @@
 Usages of a function called ``open``:
 
 .. code:: bash
 
    $ pyastgrep './/Call/func/Name[@id="open"]'
    src/pyastgrep/search.py:88:18:            with open(path) as f:
 
-Literal numbers (Python 3.8+):
+Literal numbers:
 
 .. code:: bash
 
    $ pyastgrep './/Constant[@type="int" or @type="float"]'
    tests/examples/test_xml/everything.py:5:20:    assigned_int = 123
    tests/examples/test_xml/everything.py:6:22:    assigned_float = 3.14
 
@@ -351,39 +351,48 @@
 a ``target`` node that is a parent of a ``Name`` node with attribute ``id``
 equal to ``"foo"``:
 
 .. code:: bash
 
    $ pyastgrep './/Assign[./targets//Name[@id="foo"]]' --xml
 
-Limitations
------------
+Limitations and other tools
+---------------------------
 
 pyastgrep is useful for grepping Python code at a fairly low level. It can be
 used for various refactoring or linting tasks. Some linting tasks require higher
 level understanding of a code base. For example, to detect use of a certain
 function, you need to cope with various ways that the function may be imported
 and used, and avoid detecting a function with the same name but from a different
 module. For these kinds of tasks, you might be interested in:
 
 * `Semgrep <https://semgrep.dev/>`_
 * `Fixit <https://github.com/Instagram/Fixit>`_
 
+
+If you are looking for something simpler, try:
+
+* Simon Willison’s `symbex <https://github.com/simonw/symbex/>`_ which can
+  extract functions/methods/classes.
+
 If you are using this as a library, you should note that while AST works well
 for linting, it’s not as good for rewriting code, because AST does not contain
 or preserve things like formatting and comments. For a better approach, have a
 look at `libCST <https://github.com/Instagram/LibCST>`_.
 
 
 Use as a library
 ----------------
 
-pyastgrep is structured internally to make it easy to use a library as well as
-a CLI. However, while we will try not to break things without good reason, at this
-point we are not documenting or guaranteeing API stability for these functions.
+pyastgrep is structured internally to make it easy to use as a library as well
+as a CLI, with a clear separation of the different layers. However, while we
+will try not to break things without good reason, at this point we are not
+documenting or guaranteeing API stability for these functions. Please contribute
+to `the discussion <https://github.com/spookylukey/pyastgrep/discussions/18>`_
+if you have needs here.
 
 Editor integration
 ------------------
 
 Emacs
 ~~~~~
```

### Comparing `pyastgrep-1.2.1/pyproject.toml` & `pyastgrep-1.2.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyastgrep-1.2.1/setup.cfg` & `pyastgrep-1.2.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `pyastgrep-1.2.1/src/pyastgrep/ast_utils.py` & `pyastgrep-1.2.2/src/pyastgrep/ast_utils.py`

 * *Files identical despite different names*

### Comparing `pyastgrep-1.2.1/src/pyastgrep/cli.py` & `pyastgrep-1.2.2/src/pyastgrep/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -191,15 +191,14 @@
             search_python_files(
                 paths,
                 expr,
                 xpath2=args.xpath2,
                 include_hidden=args.hidden,
                 respect_global_ignores=not args.no_ignore_global,
                 respect_vcs_ignores=not args.no_ignore_vcs,
-                add_ast_parent_nodes=isinstance(context, StatementContext),
             ),
             print_xml=args.xml,
             print_ast=args.ast,
             quiet=args.quiet,
             context=context,
             heading=args.heading,
         )
```

### Comparing `pyastgrep-1.2.1/src/pyastgrep/context.py` & `pyastgrep-1.2.2/src/pyastgrep/context.py`

 * *Files identical despite different names*

### Comparing `pyastgrep-1.2.1/src/pyastgrep/dump.py` & `pyastgrep-1.2.2/src/pyastgrep/dump.py`

 * *Files identical despite different names*

### Comparing `pyastgrep-1.2.1/src/pyastgrep/files.py` & `pyastgrep-1.2.2/src/pyastgrep/files.py`

 * *Files 3% similar despite different names*

```diff
@@ -72,26 +72,23 @@
         if linebreak_idx < 0:
             break
         else:
             current_idx = linebreak_idx + 1
     return "utf-8"
 
 
-def parse_python_file(
-    contents: bytes, filename: str | Path, *, auto_dedent: bool, add_ast_parent_nodes: bool = False
-) -> tuple[str, ast.AST]:
+def parse_python_file(contents: bytes, filename: str | Path, *, auto_dedent: bool) -> tuple[str, ast.AST]:
     if auto_dedent:
         contents = auto_dedent_code(contents)
 
     parsed_ast: ast.AST = ast.parse(contents, str(filename))
-    if add_ast_parent_nodes:
-        # Needed for StatementContext
-        for node in ast.walk(parsed_ast):
-            for child in ast.iter_child_nodes(node):
-                child.parent = node  # type: ignore
+    # Needed for StatementContext and for position_from_node
+    for node in ast.walk(parsed_ast):
+        for child in ast.iter_child_nodes(node):
+            child.parent = node  # type: ignore
 
     # ast.parse does it's own encoding detection, which we have to replicate
     # here since we can't assume utf-8
     encoding = get_encoding(contents)
     str_contents = contents.decode(encoding)
     return str_contents, parsed_ast
```

### Comparing `pyastgrep-1.2.1/src/pyastgrep/ignores.py` & `pyastgrep-1.2.2/src/pyastgrep/ignores.py`

 * *Files identical despite different names*

### Comparing `pyastgrep-1.2.1/src/pyastgrep/printer.py` & `pyastgrep-1.2.2/src/pyastgrep/printer.py`

 * *Files identical despite different names*

### Comparing `pyastgrep-1.2.1/src/pyastgrep/search.py` & `pyastgrep-1.2.2/src/pyastgrep/search.py`

 * *Files 18% similar despite different names*

```diff
@@ -53,30 +53,24 @@
 
 @dataclass(frozen=True)
 class FileFinished:
     """
     Sentinel used for flushing output
     """
 
-    path: Pathlike
+    source: Path | BinaryIO
 
 
-def position_from_xml(element: _Element, node_mappings: dict[_Element, ast.AST] | None = None) -> Position | None:
-    if not hasattr(element, "xpath"):
-        # Most likely an _ElementUnicodeResult, the result of a query that terminated in
-        # an attribute rather than a node. We have no way of getting from here to
-        # something representing an AST node.
-        raise NonElementReturned(element)
-    try:
-        linenos = xml.lxml_query(element, "./ancestor-or-self::*[@lineno][1]/@lineno")
-        col_offsets = xml.lxml_query(element, "./ancestor-or-self::*[@col_offset][1]/@col_offset")
-    except AttributeError:
-        raise AttributeError("Element has no ancestor with line number/col offset")
-    if linenos and col_offsets:
-        return Position(int(linenos[0]), int(col_offsets[0]))
+def position_from_node(node: ast.AST) -> Position | None:
+    lineno = getattr(node, "lineno", None)
+    col_offset = getattr(node, "col_offset", None)
+    if lineno is not None and col_offset is not None:
+        return Position(int(lineno), int(col_offset))
+    if (parent := getattr(node, "parent", None)) is not None:
+        return position_from_node(parent)
     return None
 
 
 def get_query_func(*, xpath2: bool) -> Callable[[_Element, str], Iterable[_Element]]:
     if xpath2:
         from .xpath2 import elementpath_query
 
@@ -88,15 +82,14 @@
 def search_python_files(
     paths: Sequence[Path | BinaryIO],
     expression: str,
     xpath2: bool = False,
     include_hidden: bool = False,
     respect_global_ignores: bool = True,
     respect_vcs_ignores: bool = True,
-    add_ast_parent_nodes: bool = False,
 ) -> Generator[Match | MissingPath | ReadError | NonElementReturned | FileFinished, None, None]:
     """
     Perform a recursive search through Python files.
 
     Paths may include directories, e.g "." for the current directory.
     .gitignore rules will be applied automatically.
 
@@ -105,58 +98,66 @@
 
     for path in get_files_to_search(
         paths,
         include_hidden=include_hidden,
         respect_global_ignores=respect_global_ignores,
         respect_vcs_ignores=respect_vcs_ignores,
     ):
-        node_mappings: dict[_Element, ast.AST] = {}
-        source: Pathlike
-        auto_dedent = False
         if isinstance(path, MissingPath):
             yield path
-            continue
-        elif isinstance(path, Path):
-            source = path
-            try:
-                contents = path.read_bytes()
-            except OSError as ex:
-                yield ReadError(str(path), ex)
-                continue
         else:
-            source = "<stdin>"
-            contents = path.read()
-            auto_dedent = True
+            yield from search_python_file(path, query_func, expression)
+            yield FileFinished(path)
+
 
+def search_python_file(
+    path: Path | BinaryIO,
+    query_func: Callable[[ast.AST, str], Iterable[_Element]],
+    expression: str,
+) -> Generator[Match | ReadError | NonElementReturned, None, None]:
+    node_mappings: dict[_Element, ast.AST] = {}
+    source: Pathlike
+    auto_dedent = False
+    if isinstance(path, Path):
+        source = path
         try:
-            str_contents, parsed_ast = parse_python_file(
-                contents, source, auto_dedent=auto_dedent, add_ast_parent_nodes=add_ast_parent_nodes
-            )
-        except SyntaxError as ex:
-            yield ReadError(str(source), ex)
-            continue
-
-        file_lines = str_contents.splitlines()
-        xml_ast = ast_to_xml(
-            parsed_ast,
-            node_mappings,
-        )
+            contents = path.read_bytes()
+        except OSError as ex:
+            yield ReadError(str(path), ex)
+            return
+    else:
+        source = "<stdin>"
+        contents = path.read()
+        auto_dedent = True
 
-        matching_elements = query_func(xml_ast, expression)
+    try:
+        str_contents, parsed_ast = parse_python_file(contents, source, auto_dedent=auto_dedent)
+    except SyntaxError as ex:
+        yield ReadError(str(source), ex)
+        return
+
+    file_lines = str_contents.splitlines()
+    xml_ast = ast_to_xml(
+        parsed_ast,
+        node_mappings,
+    )
 
-        try:
-            iterator = iter(matching_elements)
-        except TypeError:
-            yield NonElementReturned(matching_elements)
-            continue
-
-        for element in iterator:
-            ast_node = node_mappings.get(element, None)
-            try:
-                position = position_from_xml(element, node_mappings=node_mappings)
-            except NonElementReturned as ex:
-                position = None
-                yield ex
-            if position is not None and ast_node is not None:
-                yield Match(source, file_lines, element, position, ast_node)
+    matching_elements = query_func(xml_ast, expression)
 
-        yield FileFinished(source)
+    try:
+        iterator = iter(matching_elements)
+    except TypeError:
+        yield NonElementReturned(matching_elements)
+        return
+
+    for element in iterator:
+        if not isinstance(element, _Element):
+            # Most likely an _ElementUnicodeResult, the result of a query that terminated in
+            # an attribute rather than a node. We have no way of getting from here to
+            # something representing an AST node.
+            yield NonElementReturned(element)
+
+        ast_node = node_mappings.get(element, None)
+        if ast_node is not None:
+            position = position_from_node(ast_node)
+            if position is not None:
+                yield Match(source, file_lines, element, position, ast_node)
```

### Comparing `pyastgrep-1.2.1/src/pyastgrep/xml.py` & `pyastgrep-1.2.2/src/pyastgrep/xml.py`

 * *Files identical despite different names*

### Comparing `pyastgrep-1.2.1/src/pyastgrep.egg-info/PKG-INFO` & `pyastgrep-1.2.2/src/pyastgrep.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyastgrep
-Version: 1.2.1
+Version: 1.2.2
 Summary: A query tool for Python abstract syntax trees
 Home-page: https://github.com/spookylukey/pyastgrep
 Author: Luke Plant
 License: MIT
 Keywords: xpath xml ast asts syntax query css grep
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
@@ -142,15 +142,15 @@
 Usages of a function called ``open``:
 
 .. code:: bash
 
    $ pyastgrep './/Call/func/Name[@id="open"]'
    src/pyastgrep/search.py:88:18:            with open(path) as f:
 
-Literal numbers (Python 3.8+):
+Literal numbers:
 
 .. code:: bash
 
    $ pyastgrep './/Constant[@type="int" or @type="float"]'
    tests/examples/test_xml/everything.py:5:20:    assigned_int = 123
    tests/examples/test_xml/everything.py:6:22:    assigned_float = 3.14
 
@@ -373,39 +373,48 @@
 a ``target`` node that is a parent of a ``Name`` node with attribute ``id``
 equal to ``"foo"``:
 
 .. code:: bash
 
    $ pyastgrep './/Assign[./targets//Name[@id="foo"]]' --xml
 
-Limitations
------------
+Limitations and other tools
+---------------------------
 
 pyastgrep is useful for grepping Python code at a fairly low level. It can be
 used for various refactoring or linting tasks. Some linting tasks require higher
 level understanding of a code base. For example, to detect use of a certain
 function, you need to cope with various ways that the function may be imported
 and used, and avoid detecting a function with the same name but from a different
 module. For these kinds of tasks, you might be interested in:
 
 * `Semgrep <https://semgrep.dev/>`_
 * `Fixit <https://github.com/Instagram/Fixit>`_
 
+
+If you are looking for something simpler, try:
+
+* Simon Willison’s `symbex <https://github.com/simonw/symbex/>`_ which can
+  extract functions/methods/classes.
+
 If you are using this as a library, you should note that while AST works well
 for linting, it’s not as good for rewriting code, because AST does not contain
 or preserve things like formatting and comments. For a better approach, have a
 look at `libCST <https://github.com/Instagram/LibCST>`_.
 
 
 Use as a library
 ----------------
 
-pyastgrep is structured internally to make it easy to use a library as well as
-a CLI. However, while we will try not to break things without good reason, at this
-point we are not documenting or guaranteeing API stability for these functions.
+pyastgrep is structured internally to make it easy to use as a library as well
+as a CLI, with a clear separation of the different layers. However, while we
+will try not to break things without good reason, at this point we are not
+documenting or guaranteeing API stability for these functions. Please contribute
+to `the discussion <https://github.com/spookylukey/pyastgrep/discussions/18>`_
+if you have needs here.
 
 Editor integration
 ------------------
 
 Emacs
 ~~~~~
```

### Comparing `pyastgrep-1.2.1/src/pyastgrep.egg-info/SOURCES.txt` & `pyastgrep-1.2.2/src/pyastgrep.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyastgrep-1.2.1/tests/test_cli.py` & `pyastgrep-1.2.2/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `pyastgrep-1.2.1/tests/test_errors.py` & `pyastgrep-1.2.2/tests/test_errors.py`

 * *Files identical despite different names*

### Comparing `pyastgrep-1.2.1/tests/test_ignores.py` & `pyastgrep-1.2.2/tests/test_ignores.py`

 * *Files identical despite different names*

### Comparing `pyastgrep-1.2.1/tests/test_printing.py` & `pyastgrep-1.2.2/tests/test_printing.py`

 * *Files identical despite different names*

