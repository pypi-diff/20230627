# Comparing `tmp/ptyx-23.3.tar.gz` & `tmp/ptyx-24.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ptyx-23.3.tar", max compression
+gzip compressed data, was "ptyx-24.0.1.tar", max compression
```

## Comparing `ptyx-23.3.tar` & `ptyx-24.0.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0    35150 2020-10-30 21:31:21.000000 ptyx-23.3/LICENSE
--rw-r--r--   0        0        0     2103 2022-06-30 22:01:37.570132 ptyx-23.3/README.md
--rw-r--r--   0        0        0      502 2022-06-30 18:12:51.329772 ptyx-23.3/ptyx/__init__.py
--rw-r--r--   0        0        0     1281 2023-02-25 22:04:21.525422 ptyx-23.3/ptyx/asynctools.py
--rw-r--r--   0        0        0    17379 2023-04-05 08:16:06.526131 ptyx-23.3/ptyx/compilation.py
--rw-r--r--   0        0        0     1414 2023-03-07 21:39:04.864606 ptyx-23.3/ptyx/config.py
--rw-r--r--   0        0        0     2166 2023-04-03 14:57:01.344552 ptyx-23.3/ptyx/context.py
--rw-r--r--   0        0        0        0 2020-10-30 21:31:21.000000 ptyx-23.3/ptyx/extensions/__init__.py
--rw-r--r--   0        0        0     3331 2023-02-28 08:48:01.754776 ptyx-23.3/ptyx/extensions/extended_python/__init__.py
--rw-r--r--   0        0        0     1236 2021-10-24 11:22:17.366687 ptyx-23.3/ptyx/extensions/extended_python/tests/test_extended_python.py
--rwxr-xr-x   0        0        0     3843 2023-03-07 21:46:27.398091 ptyx-23.3/ptyx/extensions/geophyx/__init__.py
--rw-r--r--   0        0        0     1045 2022-06-28 21:14:42.142582 ptyx-23.3/ptyx/extensions/geophyx/tests/test_geophyx.py
--rw-r--r--   0        0        0     6451 2022-01-14 17:03:08.268277 ptyx-23.3/ptyx/extensions/questions/__init__.py
--rw-r--r--   0        0        0      882 2020-05-16 15:27:00.754047 ptyx-23.3/ptyx/extensions/questions/tests/in.txt
--rw-r--r--   0        0        0      610 2020-05-16 15:28:17.000000 ptyx-23.3/ptyx/extensions/questions/tests/out.ptyx
--rw-r--r--   0        0        0      347 2021-12-14 21:39:11.968415 ptyx-23.3/ptyx/extensions/questions/tests/test_questions.py
--rw-r--r--   0        0        0    44449 2023-04-03 15:38:53.378669 ptyx-23.3/ptyx/latex_generator.py
--rw-r--r--   0        0        0     7276 2023-03-07 22:23:52.242156 ptyx-23.3/ptyx/printers.py
--rw-r--r--   0        0        0        0 2022-07-02 20:31:53.563621 ptyx-23.3/ptyx/py.typed
--rw-r--r--   0        0        0    11024 2023-03-07 22:21:42.328539 ptyx-23.3/ptyx/randfunc.py
--rwxr-xr-x   0        0        0     9833 2023-04-05 08:39:33.150238 ptyx-23.3/ptyx/script.py
--rw-r--r--   0        0        0    21141 2023-04-03 15:32:55.653998 ptyx-23.3/ptyx/syntax_tree.py
--rw-r--r--   0        0        0     8160 2023-04-03 14:57:01.464554 ptyx-23.3/ptyx/utilities.py
--rw-r--r--   0        0        0     1282 2023-04-05 06:14:35.139917 ptyx-23.3/pyproject.toml
--rw-r--r--   0        0        0     2904 1970-01-01 00:00:00.000000 ptyx-23.3/PKG-INFO
+-rw-r--r--   0        0        0    35150 2020-10-30 21:31:21.000000 ptyx-24.0.1/LICENSE
+-rw-r--r--   0        0        0     2103 2022-06-30 22:01:37.000000 ptyx-24.0.1/README.md
+-rw-r--r--   0        0        0      212 2023-06-27 17:36:42.418224 ptyx-24.0.1/ptyx/__init__.py
+-rw-r--r--   0        0        0     1281 2023-02-25 22:04:21.525422 ptyx-24.0.1/ptyx/asynctools.py
+-rw-r--r--   0        0        0    17389 2023-06-27 17:21:00.184250 ptyx-24.0.1/ptyx/compilation.py
+-rw-r--r--   0        0        0     1414 2023-03-07 21:39:04.864606 ptyx-24.0.1/ptyx/config.py
+-rw-r--r--   0        0        0     2166 2023-04-03 14:57:01.344552 ptyx-24.0.1/ptyx/context.py
+-rw-r--r--   0        0        0      258 2023-06-27 17:21:15.380475 ptyx-24.0.1/ptyx/extensions/__init__.py
+-rw-r--r--   0        0        0     3331 2023-02-28 08:48:01.754776 ptyx-24.0.1/ptyx/extensions/extended_python/__init__.py
+-rw-r--r--   0        0        0     1236 2021-10-24 11:22:17.366687 ptyx-24.0.1/ptyx/extensions/extended_python/tests/test_extended_python.py
+-rwxr-xr-x   0        0        0     4080 2023-06-27 17:21:15.380475 ptyx-24.0.1/ptyx/extensions/geophyx/__init__.py
+-rw-r--r--   0        0        0     1045 2022-06-28 21:14:42.142582 ptyx-24.0.1/ptyx/extensions/geophyx/tests/test_geophyx.py
+-rw-r--r--   0        0        0     6451 2022-01-14 17:03:08.268277 ptyx-24.0.1/ptyx/extensions/questions/__init__.py
+-rw-r--r--   0        0        0      882 2020-05-16 15:27:00.754047 ptyx-24.0.1/ptyx/extensions/questions/tests/in.txt
+-rw-r--r--   0        0        0      610 2020-05-16 15:28:17.000000 ptyx-24.0.1/ptyx/extensions/questions/tests/out.ptyx
+-rw-r--r--   0        0        0      347 2021-12-14 21:39:11.968415 ptyx-24.0.1/ptyx/extensions/questions/tests/test_questions.py
+-rw-r--r--   0        0        0    44476 2023-06-27 17:21:15.384475 ptyx-24.0.1/ptyx/latex_generator.py
+-rw-r--r--   0        0        0     7212 2023-06-27 17:20:50.352104 ptyx-24.0.1/ptyx/printers.py
+-rw-r--r--   0        0        0        0 2022-07-02 20:31:53.563621 ptyx-24.0.1/ptyx/py.typed
+-rw-r--r--   0        0        0    11024 2023-03-07 22:21:42.328539 ptyx-24.0.1/ptyx/randfunc.py
+-rwxr-xr-x   0        0        0     9998 2023-06-27 17:21:15.396475 ptyx-24.0.1/ptyx/script.py
+-rw-r--r--   0        0        0    21142 2023-06-27 17:21:15.388475 ptyx-24.0.1/ptyx/syntax_tree.py
+-rw-r--r--   0        0        0     8160 2023-04-03 14:57:01.464554 ptyx-24.0.1/ptyx/utilities.py
+-rw-r--r--   0        0        0     1394 2023-06-27 17:38:53.492137 ptyx-24.0.1/pyproject.toml
+-rw-r--r--   0        0        0     2906 1970-01-01 00:00:00.000000 ptyx-24.0.1/PKG-INFO
```

### Comparing `ptyx-23.3/LICENSE` & `ptyx-24.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ptyx-23.3/README.md` & `ptyx-24.0.1/README.md`

 * *Files identical despite different names*

### Comparing `ptyx-23.3/ptyx/asynctools.py` & `ptyx-24.0.1/ptyx/asynctools.py`

 * *Files identical despite different names*

### Comparing `ptyx-23.3/ptyx/compilation.py` & `ptyx-24.0.1/ptyx/compilation.py`

 * *Files 0% similar despite different names*

```diff
@@ -236,17 +236,17 @@
         assert ext[0] != "."
         ext = f".{ext}"
         name = output_basename.with_suffix(ext)
         if name.is_file():
             # There is only one file (only one document was generated,
             # or they were several documents, but they were joined into a single document).
             shutil.copy(name, input_name.parent)
-        elif options.get("names"):
+        elif options.get("names_list"):
             # Rename files according to the given names' list.
-            names = options["names"]
+            names = options["names_list"]
             assert len(names) == len(filenames)
             for filename, stem in zip(filenames, names):
                 new_name = filename.with_stem(stem).name
                 shutil.copy(filename.with_suffix(ext), input_name.parent / new_name)
         else:
             # Copy files without changing names.
             for filename in filenames:
```

### Comparing `ptyx-23.3/ptyx/config.py` & `ptyx-24.0.1/ptyx/config.py`

 * *Files identical despite different names*

### Comparing `ptyx-23.3/ptyx/context.py` & `ptyx-24.0.1/ptyx/context.py`

 * *Files identical despite different names*

### Comparing `ptyx-23.3/ptyx/extensions/extended_python/__init__.py` & `ptyx-24.0.1/ptyx/extensions/extended_python/__init__.py`

 * *Files identical despite different names*

### Comparing `ptyx-23.3/ptyx/extensions/extended_python/tests/test_extended_python.py` & `ptyx-24.0.1/ptyx/extensions/extended_python/tests/test_extended_python.py`

 * *Files identical despite different names*

### Comparing `ptyx-23.3/ptyx/extensions/geophyx/__init__.py` & `ptyx-24.0.1/ptyx/extensions/geophyx/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 
 """
 
 # mypy: ignore-errors
 
 import random
 
+from ptyx.extensions import CompilerExtension
 from wxgeometrie.modules.tablatex import tabval, tabvar, tabsign
 from wxgeometrie.mathlib.parsers import traduire_formule
 from wxgeometrie.mathlib.interprete import Interprete
 from wxgeometrie.geolib import Feuille
 
 import sympy
 from ptyx.latex_generator import LatexGenerator
@@ -115,21 +116,23 @@
         args, kw = self._parse_options(node)
         for key in kw:
             kw[key] = eval(kw[key])
         self._parse_children(node.children, function=tabsign, **kw)
         random.setstate(state)
 
 
-__latex_generator_extension__ = GeophyxLatexGenerator
-__tags__ = {
-    "CALC": (1, 0, None),
-    "GCALC": (0, 0, ["@END_GCALC", "@END"]),
-    "GEO": (0, 0, ["@END_GEO", "@END"]),
-    "TABSIGN": (0, 0, ["@END_TABSIGN", "@END"]),
-    "TABVAL": (0, 0, ["@END_TABVAL", "@END"]),
-    "TABVAR": (0, 0, ["@END_TABVAR", "@END"]),
-}
+def extend_compiler() -> CompilerExtension:
+    """Function called by the compiler when loading this extension, to add ability to parse new tags."""
+    tags = {
+        "CALC": (1, 0, None),
+        "GCALC": (0, 0, ["@END_GCALC", "@END"]),
+        "GEO": (0, 0, ["@END_GEO", "@END"]),
+        "TABSIGN": (0, 0, ["@END_TABSIGN", "@END"]),
+        "TABVAL": (0, 0, ["@END_TABVAL", "@END"]),
+        "TABVAR": (0, 0, ["@END_TABVAR", "@END"]),
+    }
+    return {"latex_generator": GeophyxLatexGenerator, "tags": tags}
 
 
 def main(code, compiler):
     # Code is left untouched, this extension only adds new commands.
     return code
```

### Comparing `ptyx-23.3/ptyx/extensions/geophyx/tests/test_geophyx.py` & `ptyx-24.0.1/ptyx/extensions/geophyx/tests/test_geophyx.py`

 * *Files identical despite different names*

### Comparing `ptyx-23.3/ptyx/extensions/questions/__init__.py` & `ptyx-24.0.1/ptyx/extensions/questions/__init__.py`

 * *Files identical despite different names*

### Comparing `ptyx-23.3/ptyx/extensions/questions/tests/in.txt` & `ptyx-24.0.1/ptyx/extensions/questions/tests/in.txt`

 * *Files identical despite different names*

### Comparing `ptyx-23.3/ptyx/extensions/questions/tests/out.ptyx` & `ptyx-24.0.1/ptyx/extensions/questions/tests/out.ptyx`

 * *Files identical despite different names*

### Comparing `ptyx-23.3/ptyx/latex_generator.py` & `ptyx-24.0.1/ptyx/latex_generator.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,16 +3,18 @@
 import traceback
 from importlib import import_module, metadata
 from os.path import dirname, basename, join
 from pathlib import Path
 from types import ModuleType
 from typing import Optional, Union, Callable, Iterable, Dict, Tuple, List, TypedDict
 
+from ptyx.extensions import CompilerExtension
+
 import ptyx.randfunc as randfunc
-from ptyx import __version__, __api__
+from ptyx import __version__
 from ptyx.config import param, SYMPY_AVAILABLE
 from ptyx.context import GLOBAL_CONTEXT
 
 # from ptyx.printers import sympy2latex
 from ptyx.syntax_tree import Node, SyntaxTreeGenerator, Tag, TagSyntax
 from ptyx.utilities import advanced_split, numbers_to_floats, _float_me_if_you_can, latex_verbatim
 
@@ -267,30 +269,24 @@
         context_backup = self.context
         self.set_new_context()
         # Interprete code
         self._parse_children(node.children)
         # Restore local variables and update generated LaTeX code.
         self.set_new_context(context_backup)
 
-    def _parse_API_VERSION_tag(self, node: Node):
-        def version_tuple(version: str):
-            return version.split(".")
+    def _parse_PTYX_VERSION_tag(self, node: Node):
+        def version_tuple(version_: str):
+            return version_.split(".")
 
         assert isinstance(node.children[0], Node), repr(node)
         assert isinstance(node.children[0].children[0], str), repr(node)
         version = version_tuple(node.children[0].children[0])
         if version_tuple(__version__) < version:
             print("Warning: pTyX engine is too old (v%s required)." % version)
-        if version < version_tuple(__api__):
-            print(
-                "Warning: pTyX file uses an old API. You may have to update "
-                "your pTyX file code before compiling it."
-            )
-        # TODO: display a short list of API changes which broke compatibility.
-        self.context["API_VERSION"] = version
+        self.context["PTYX_VERSION"] = version
 
     def _parse_ASK_tag(self, node: Node):
         self._parse_children(node.children, function=self.context.get("format_ask"))
 
     def _parse_ASK_ONLY_tag(self, node: Node):
         if not self.WITH_ANSWERS:
             self._parse_children(node.children, function=self.context.get("format_ask_only"))
@@ -918,30 +914,34 @@
                 for entry_point in metadata.entry_points(group="ptyx.extensions"):
                     if entry_point.name == extension_name:
                         extensions[extension_name] = import_module(entry_point.value)
                         break
                 else:
                     traceback.print_exc()
                     raise ImportError(f"Extension {extension_name} not found.")
-            # Test if extension defines new tags.
-            ext_tags = getattr(extensions[extension_name], "__tags__", {})
-            for tag, syntax in ext_tags.items():
-                # Test for conflict between extensions.
-                if tag in tags_source:
-                    raise NameError(
-                        f"Extension {extension_name} tries to define tag {tag}, "
-                        f"which was already defined by extension {tags_source[tag]}."
-                    )
-                # Tag not already declared, everything seems OK.
-                tags_source[tag] = extension_name
-                tags_syntax[tag] = syntax
-            # Extension may subclass LatexGenerator class, notably to handle new tags.
-            subclass = getattr(extensions[extension_name], "__latex_generator_extension__", None)
-            if subclass is not None:
-                latex_generator_extensions.append(subclass)
+            try:
+                # This extension may define a function `extend_compiler()` to customize the compiler.
+                extensions_dict: CompilerExtension = getattr(extensions[extension_name], "extend_compiler")()
+                # This extension may subclass LatexGenerator class, notably to handle new tags.
+                if "latex_generator" in extensions_dict:
+                    latex_generator_extensions.append(extensions_dict["latex_generator"])
+                # Test if this extension defines new tags.
+                ext_tags = extensions_dict.get("tags", {})
+                for tag, syntax in ext_tags.items():
+                    # Test for conflict between extensions.
+                    if tag in tags_source:
+                        raise NameError(
+                            f"Extension {extension_name} tries to define tag {tag}, "
+                            f"which was already defined by extension {tags_source[tag]}."
+                        )
+                    # Tag not already declared, everything seems OK.
+                    tags_source[tag] = extension_name
+                    tags_syntax[tag] = syntax
+            except AttributeError:
+                pass
         # Load new tags.
         self.add_new_tags(*tags_syntax.items())
         # Update LatexGenerator.
         if latex_generator_extensions:
             # TODO: Test for conflicting methods ?
             class CustomLatexGenerator(*reversed(latex_generator_extensions)):  # type: ignore
                 pass
```

### Comparing `ptyx-23.3/ptyx/printers.py` & `ptyx-24.0.1/ptyx/printers.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 #     from sympy.printing.latex import LatexPrinter
 # except ImportError:
 #     print("Warning: `sympy` library not found !")
 #     sympy = None  # type: ignore
 
 import sympy
 from sympy import Basic, Symbol, Integer, Float, I, Mul
-from sympy.core.core import BasicMeta
 from sympy.printing.latex import LatexPrinter
 
 from ptyx.config import param
 
 
 class CustomLatexPrinter(LatexPrinter):
     def __init__(self, settings):
@@ -55,30 +54,30 @@
                 printmethod = "_print_" + cls.__name__
                 if hasattr(self, printmethod):
                     return getattr(self, printmethod)(expr, *args, **kwargs)
 
             # If the printer defines a name for a printing method
             # (Printer.printmethod) and the object knows for itself how it
             # should be printed, use that method.
-            if self.printmethod and hasattr(expr, self.printmethod) and not isinstance(expr, BasicMeta):
+            if self.printmethod and hasattr(expr, self.printmethod):
                 return getattr(expr, self.printmethod)(self, *args, **kwargs)
 
             # Avoid new (strange) behaviour of sympy 1.7+
             if isinstance(expr, str):
                 return expr
             # Unknown object, fall back to the emptyPrinter.
             return self.emptyPrinter(expr)
         finally:
             self._print_level -= 1
 
     def _print_exp(self, expr, exp=None):
         tex = r"\mathrm{e}^{%s}" % self._print(expr.args[0])
         return self._do_exponent(tex, exp)
 
-    def _print_Exp1(self, expr):
+    def _print_Exp1(self, expr, exp=None):
         return r"\mathrm{e}"
 
     def _print_Abs(self, *args, **kw):
         res = LatexPrinter._print_Abs(self, *args, **kw)
         return res.replace(r"\lvert", r"|").replace(r"\rvert", r"|")
 
     def _print_Pi(self, *args, **kw):
```

### Comparing `ptyx-23.3/ptyx/randfunc.py` & `ptyx-24.0.1/ptyx/randfunc.py`

 * *Files identical despite different names*

### Comparing `ptyx-23.3/ptyx/script.py` & `ptyx-24.0.1/ptyx/script.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,27 +20,25 @@
 #
 #    You should have received a copy of the GNU General Public License
 #    along with this program; if not, write to the Free Software
 #    Foundation, Inc., 51 Franklin St, Fifth Floor, Boston, MA  02110-1301  USA
 
 
 import argparse
-import csv
 import sys
+import csv
 from ast import literal_eval
 from pathlib import Path
 
 from ptyx import __version__
-from ptyx.compilation import make_files
 from ptyx.config import param
-from ptyx.latex_generator import compiler
 
 
 if sys.version_info.major == 2:
-    raise RuntimeError("Python version 3.8+ is needed !")
+    raise RuntimeError("Python version 3.10+ is needed !")
 
 
 class PtyxArgumentParser(argparse.ArgumentParser):
     """Parse pTyX command line interface options."""
 
     def __init__(self):
         super().__init__(
@@ -56,14 +54,15 @@
             type=int,
             help="Number of pdf files to generate. Default is %s.\n \
                        Ex: ptyx -n 5 my_file.ptyx"
             % param["total"],
         )
         group.add_argument(
             "--names",
+            type=str,
             metavar="CSV_FILE",
             help="Name of a CSV file containing a column of names \
                                (and optionally a second column with forenames). \n \
                                The names will be used to generate the #NAME tag \
                                replacement value.\n \
                                Additionally, if `-n` option is not specified, \
                                default value will be the number of names in the CSV file.",
@@ -103,15 +102,15 @@
             help="Cat all generated pdf files inside a single one.",
         )
         self.add_argument(
             "-C",
             "--compress",
             action="store_true",
             help="Like --cat, but compress final pdf file using pdf2ps and ps2pdf. "
-                 "Ghostscript must be present (on Linux, it is probably already installed).",
+            "Ghostscript must be present (on Linux, it is probably already installed).",
         )
         self.add_argument(
             "--reorder-pages",
             choices=["brochure", "brochure-reversed"],
             help="Reorder pages for printing.\n\
                 Currently, only 'brochure' and 'brochure-reversed' mode are supported.\
                 The `pdftk` command must be installed.\n\
@@ -173,31 +172,39 @@
             # pdftk and ghostscript must be installed.
             if "pdf" not in options.formats:
                 raise RuntimeError("--cat or --compress option invalid unless pdf output is selected.")
         if options.debug:
             param["debug"] = True
         if options.names:
             with open(Path(options.names).expanduser().resolve()) as f:
-                options.names = [" ".join(line) for line in csv.reader(f)]
+                options.names_list = [" ".join(line) for line in csv.reader(f)]
                 print("Names extracted from CSV file:")
-                print(options.names)
+                print(options.names_list)
             options.number_of_documents = len(options.names)
         else:
-            options.names = []
+            options.names_list = []
         if options.number_of_documents is None:
             options.number_of_documents = param["total"]
         return options
 
 
 def ptyx(parser=PtyxArgumentParser()):
     """Main pTyX procedure."""
+
     # First, parse all arguments (filenames, options...)
     # --------------------------------------------------
     options = parser.parse_args()
 
+    if not options.filenames:
+        # Exit quickly before main imports, so that `ptyx --help` is fast.
+        exit(0)
+
+    from ptyx.compilation import make_files
+    from ptyx.latex_generator import compiler
+
     # TODO: remove kwargs and explicitly pass arguments, to verify types.
     kwargs = vars(options)
     if "fixed_number_of_pages" in kwargs:
         kwargs["pages"] = kwargs["fixed_number_of_pages"]
         kwargs["fixed_number_of_pages"] = True
     else:
         kwargs["fixed_number_of_pages"] = False
```

### Comparing `ptyx-23.3/ptyx/syntax_tree.py` & `ptyx-24.0.1/ptyx/syntax_tree.py`

 * *Files 0% similar despite different names*

```diff
@@ -134,15 +134,14 @@
     # By contrast, in code arguments, inner strings should be detected:
     # in {val=="}"}, the bracket closing the tag is the second `}`, not the first one !
 
     tags: Dict[Tag, TagSyntax] = {
         "ANS": (0, 0, ["@END"]),
         "ANSWER": (0, 1, None),
         "APART": (0, 0, ["@END", "@END_APART"]),
-        "API_VERSION": (0, 1, None),
         "ASK": (0, 0, ["@END"]),
         "ASK_ONLY": (0, 0, ["@END"]),
         "ASSERT": (1, 0, None),
         # Do *NOT* consume #END tag, which must be used to end #CONDITIONAL_BLOCK.
         "CASE": (1, 0, ["CASE", "ELSE", "END", "END_CASE"]),
         "COMMENT": (0, 0, ["@END"]),
         # CONDITIONAL_BLOCK isn't a real tag, but is used to enclose
@@ -164,14 +163,15 @@
         "FREEZE_RANDOM_STATE": (0, 0, []),
         "IFNUM": (1, 1, None),
         "INCLUDE": (1, 0, None),
         "CALL": (0, 1, None),
         "MACRO": (0, 1, ["@END", "@END_MACRO"]),
         "PICK": (0, 0, ["@END", "@END_PICK"]),
         "PRINT": (1, 0, None),
+        "PTYX_VERSION": (0, 1, None),
         "PYTHON": (0, 0, ["@END"]),
         "QUESTION": (0, 1, None),
         # ROOT isn't a real tag, and is never closed.
         "ROOT": (0, 0, []),
         "SEED": (1, 0, None),
         "SHUFFLE": (0, 0, ["@END", "@END_SHUFFLE"]),
         # Do *NOT* consume #END tag, which must be used to end #SHUFFLE block.
```

### Comparing `ptyx-23.3/ptyx/utilities.py` & `ptyx-24.0.1/ptyx/utilities.py`

 * *Files identical despite different names*

### Comparing `ptyx-23.3/pyproject.toml` & `ptyx-24.0.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,39 +1,43 @@
 [tool.poetry]
 name = "ptyx"
-version = "23.3"
+version = "24.0.1"
 description = "pTyX is a python precompiler for LaTeX."
 authors = ["Nicolas Pourcelot <nicolas.pourcelot@gmail.com>"]
 repository = "https://github.com/wxgeo/ptyx"
 license = "GPL-3.0-or-later"
 readme = "README.md"
 keywords = ["python", "tikz", "latex", "pdf", "exam", "mcq", "student"]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 numpy = "^1.23.0"
 sympy = "^1.10.1"
 psutil = "^5.9.4"
 pymupdf = "^1.21.1"
 
-[tool.poetry.dev-dependencies]
+[tool.poetry.group.dev.dependencies]
 pytest = "^7.2.1"
 mypy = "^1.0.1"
 flake8 = "^6"
 black = "^22.1.0"
 tox = "^4.3.5"
 sphinx-autodoc-typehints = "^1.19.5"
 sphinx-rtd-theme = "^1.0.0"
 myst-parser = "^0.18.0"
+python-semantic-release = "7.28.1"
 
 [tool.poetry.scripts]
 ptyx = 'ptyx.script:ptyx'
 scan = 'ptyx.extensions.autoqcm.cli:scan'
 autoqcm = 'ptyx.extensions.autoqcm.cli:main'
 
+[tool.semantic_release]
+version_variable = "pyproject.toml:version"
+
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.mypy]
 ignore_missing_imports = true
 implicit_optional = true
```

### Comparing `ptyx-23.3/PKG-INFO` & `ptyx-24.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ptyx
-Version: 23.3
+Version: 24.0.1
 Summary: pTyX is a python precompiler for LaTeX.
 Home-page: https://github.com/wxgeo/ptyx
 License: GPL-3.0-or-later
 Keywords: python,tikz,latex,pdf,exam,mcq,student
 Author: Nicolas Pourcelot
 Author-email: nicolas.pourcelot@gmail.com
 Requires-Python: >=3.10,<4.0
```

