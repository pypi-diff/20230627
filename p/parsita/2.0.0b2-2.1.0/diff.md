# Comparing `tmp/parsita-2.0.0b2.tar.gz` & `tmp/parsita-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "parsita-2.0.0b2.tar", max compression
+gzip compressed data, was "parsita-2.1.0.tar", max compression
```

## Comparing `parsita-2.0.0b2.tar` & `parsita-2.1.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0     1062 2023-05-10 01:19:05.730334 parsita-2.0.0b2/LICENSE
--rw-r--r--   0        0        0     2649 2023-06-19 18:30:55.314799 parsita-2.0.0b2/README.md
--rw-r--r--   0        0        0     2115 2023-06-19 20:53:20.299938 parsita-2.0.0b2/pyproject.toml
--rw-r--r--   0        0        0      363 2023-06-19 18:30:55.314799 parsita-2.0.0b2/src/parsita/__init__.py
--rw-r--r--   0        0        0     5488 2023-06-19 18:30:55.314799 parsita-2.0.0b2/src/parsita/metaclasses.py
--rw-r--r--   0        0        0      165 2023-06-19 18:30:55.314799 parsita-2.0.0b2/src/parsita/options.py
--rw-r--r--   0        0        0      833 2023-06-19 18:30:55.318799 parsita-2.0.0b2/src/parsita/parsers/__init__.py
--rw-r--r--   0        0        0     3845 2023-06-19 18:30:55.318799 parsita-2.0.0b2/src/parsita/parsers/_alternative.py
--rw-r--r--   0        0        0      940 2023-06-19 18:30:55.318799 parsita-2.0.0b2/src/parsita/parsers/_any.py
--rw-r--r--   0        0        0     7859 2023-06-19 18:30:55.318799 parsita-2.0.0b2/src/parsita/parsers/_base.py
--rw-r--r--   0        0        0     1532 2023-06-19 18:30:55.318799 parsita-2.0.0b2/src/parsita/parsers/_conversion.py
--rw-r--r--   0        0        0     2345 2023-06-19 18:30:55.318799 parsita-2.0.0b2/src/parsita/parsers/_debug.py
--rw-r--r--   0        0        0      640 2023-06-19 18:30:55.318799 parsita-2.0.0b2/src/parsita/parsers/_end_of_source.py
--rw-r--r--   0        0        0     2576 2023-06-19 18:30:55.318799 parsita-2.0.0b2/src/parsita/parsers/_literal.py
--rw-r--r--   0        0        0     1266 2023-06-19 18:30:55.318799 parsita-2.0.0b2/src/parsita/parsers/_optional.py
--rw-r--r--   0        0        0     1489 2023-06-19 18:58:14.007247 parsita-2.0.0b2/src/parsita/parsers/_predicate.py
--rw-r--r--   0        0        0     1809 2023-06-19 18:30:55.318799 parsita-2.0.0b2/src/parsita/parsers/_regex.py
--rw-r--r--   0        0        0     3863 2023-06-19 18:30:55.318799 parsita-2.0.0b2/src/parsita/parsers/_repeated.py
--rw-r--r--   0        0        0     6112 2023-06-19 18:30:55.318799 parsita-2.0.0b2/src/parsita/parsers/_repeated_seperated.py
--rw-r--r--   0        0        0     2512 2023-06-19 18:30:55.318799 parsita-2.0.0b2/src/parsita/parsers/_sequential.py
--rw-r--r--   0        0        0     1817 2023-06-19 18:30:55.318799 parsita-2.0.0b2/src/parsita/parsers/_success.py
--rw-r--r--   0        0        0     1298 2023-06-19 18:30:55.318799 parsita-2.0.0b2/src/parsita/parsers/_until.py
--rw-r--r--   0        0        0      207 2023-06-19 18:30:55.318799 parsita-2.0.0b2/src/parsita/state/__init__.py
--rw-r--r--   0        0        0      807 2023-06-19 18:30:55.318799 parsita-2.0.0b2/src/parsita/state/_exceptions.py
--rw-r--r--   0        0        0     8450 2023-06-19 20:34:31.867158 parsita-2.0.0b2/src/parsita/state/_reader.py
--rw-r--r--   0        0        0      500 2023-06-19 18:30:55.318799 parsita-2.0.0b2/src/parsita/state/_result.py
--rw-r--r--   0        0        0     1050 2023-06-19 18:30:55.318799 parsita-2.0.0b2/src/parsita/state/_state.py
--rw-r--r--   0        0        0     1688 2023-06-19 18:30:55.318799 parsita-2.0.0b2/src/parsita/util.py
--rw-r--r--   0        0        0     3653 1970-01-01 00:00:00.000000 parsita-2.0.0b2/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-05-10 01:19:05.730334 parsita-2.1.0/LICENSE
+-rw-r--r--   0        0        0     2649 2023-06-24 14:10:57.618930 parsita-2.1.0/README.md
+-rw-r--r--   0        0        0     2111 2023-06-26 23:56:16.483050 parsita-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0      400 2023-06-24 14:10:57.622930 parsita-2.1.0/src/parsita/__init__.py
+-rw-r--r--   0        0        0     5572 2023-06-24 14:10:57.622930 parsita-2.1.0/src/parsita/metaclasses.py
+-rw-r--r--   0        0        0      165 2023-06-24 14:10:57.622930 parsita-2.1.0/src/parsita/options.py
+-rw-r--r--   0        0        0      868 2023-06-26 13:02:50.667350 parsita-2.1.0/src/parsita/parsers/__init__.py
+-rw-r--r--   0        0        0     3823 2023-06-26 13:02:50.743350 parsita-2.1.0/src/parsita/parsers/_alternative.py
+-rw-r--r--   0        0        0      955 2023-06-26 13:02:50.743350 parsita-2.1.0/src/parsita/parsers/_any.py
+-rw-r--r--   0        0        0     7841 2023-06-26 13:02:50.743350 parsita-2.1.0/src/parsita/parsers/_base.py
+-rw-r--r--   0        0        0     1572 2023-06-26 13:02:50.743350 parsita-2.1.0/src/parsita/parsers/_conversion.py
+-rw-r--r--   0        0        0     2290 2023-06-26 13:02:50.743350 parsita-2.1.0/src/parsita/parsers/_debug.py
+-rw-r--r--   0        0        0      655 2023-06-26 13:02:50.743350 parsita-2.1.0/src/parsita/parsers/_end_of_source.py
+-rw-r--r--   0        0        0     2563 2023-06-26 13:02:50.743350 parsita-2.1.0/src/parsita/parsers/_literal.py
+-rw-r--r--   0        0        0     1201 2023-06-26 13:02:50.743350 parsita-2.1.0/src/parsita/parsers/_optional.py
+-rw-r--r--   0        0        0     1527 2023-06-26 13:02:50.743350 parsita-2.1.0/src/parsita/parsers/_predicate.py
+-rw-r--r--   0        0        0     1796 2023-06-26 13:02:50.743350 parsita-2.1.0/src/parsita/parsers/_regex.py
+-rw-r--r--   0        0        0     3768 2023-06-26 13:02:50.743350 parsita-2.1.0/src/parsita/parsers/_repeated.py
+-rw-r--r--   0        0        0     6007 2023-06-26 13:02:50.743350 parsita-2.1.0/src/parsita/parsers/_repeated_seperated.py
+-rw-r--r--   0        0        0     2527 2023-06-26 13:02:50.743350 parsita-2.1.0/src/parsita/parsers/_sequential.py
+-rw-r--r--   0        0        0     1819 2023-06-26 13:02:50.743350 parsita-2.1.0/src/parsita/parsers/_success.py
+-rw-r--r--   0        0        0     1233 2023-06-26 13:02:50.743350 parsita-2.1.0/src/parsita/parsers/_until.py
+-rw-r--r--   0        0        0      207 2023-06-24 14:10:57.622930 parsita-2.1.0/src/parsita/state/__init__.py
+-rw-r--r--   0        0        0      807 2023-06-24 14:10:57.622930 parsita-2.1.0/src/parsita/state/_exceptions.py
+-rw-r--r--   0        0        0     8522 2023-06-26 10:31:34.277910 parsita-2.1.0/src/parsita/state/_reader.py
+-rw-r--r--   0        0        0      500 2023-06-24 14:10:57.622930 parsita-2.1.0/src/parsita/state/_result.py
+-rw-r--r--   0        0        0     1050 2023-06-24 14:10:57.622930 parsita-2.1.0/src/parsita/state/_state.py
+-rw-r--r--   0        0        0     1680 2023-06-24 14:10:57.622930 parsita-2.1.0/src/parsita/util.py
+-rw-r--r--   0        0        0     3651 1970-01-01 00:00:00.000000 parsita-2.1.0/PKG-INFO
```

### Comparing `parsita-2.0.0b2/LICENSE` & `parsita-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `parsita-2.0.0b2/README.md` & `parsita-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `parsita-2.0.0b2/pyproject.toml` & `parsita-2.1.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "parsita"
-version = "2.0.0b2"
+version = "2.1.0"
 description = "Parser combinator library for Python"
 authors = ["David Hagen <david@drhagen.com>"]
 license = "MIT"
 readme = "README.md"
 documentation = "https://parsita.drhagen.com"
 repository = "https://github.com/drhagen/parsita"
 keywords = ["text", "parsing", "parser",  "combinator"]
@@ -63,20 +63,20 @@
     "src/",
     ".nox/test*/lib/python*/site-packages/",
     ".nox/test*/Lib/site-packages/",
 ]
 
 
 [tool.black]
-line-length = 120
+line-length = 99
 
 
 [tool.ruff]
 src = ["src"]
-line-length = 120
+line-length = 99
 extend-select = [
     "I", # isort
     "N", # pep8-naming
     "RUF", # ruff
     "B", # flake8-bugbear
     "N", # flake8-broken-line
     "C4", # flake8-comprehensions
```

### Comparing `parsita-2.0.0b2/src/parsita/metaclasses.py` & `parsita-2.1.0/src/parsita/metaclasses.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,15 +18,16 @@
         super().__init__()
         self.old_options = old_options  # Holds state of options at start of definition
         self.forward_declarations = {}  # Stores forward declarations as they are discovered
 
     def __missing__(self, key):
         frame = inspect.currentframe()  # Should be the frame of __missing__
         while frame.f_code.co_name != "__missing__":  # pragma: no cover
-            # But sometimes debuggers add frames on top of the stack; get back to `__missing__`'s frame
+            # But sometimes debuggers add frames on top of the stack;
+            # get back to `__missing__`'s frame
             frame = frame.f_back
 
         class_body_frame = frame.f_back.f_back  # Frame of parser context is two frames back
         class_body_locals = class_body_frame.f_locals
         class_body_globals = class_body_frame.f_globals
 
         if key in self.forward_declarations:
@@ -40,16 +41,19 @@
         else:
             new_forward_declaration = ForwardDeclaration()
             self.forward_declarations[key] = new_forward_declaration
             return new_forward_declaration
 
     def __setitem__(self, key, value):
         if isinstance(value, Parser):
-            value.protected = True  # Protects against accidental concatenation of sequential parsers
-            value.name = key  # Used for better error messages
+            # Protects against accidental concatenation of sequential parsers
+            value.protected = True
+
+            # Used for better error messages
+            value.name = key
 
         super().__setitem__(key, value)
 
 
 class ForwardDeclaration(Parser):
     def __init__(self):
         self._definition = None
@@ -75,15 +79,19 @@
 
 
 class ParserContextMeta(type):
     default_whitespace: Union[Parser[Input, Any], Pattern, str, None] = None
 
     @classmethod
     def __prepare__(
-        mcs, name, bases, *, whitespace: Union[Parser[Input, Any], Pattern, str, None] = missing  # noqa: N804
+        mcs,  # noqa: N804
+        name,
+        bases,
+        *,
+        whitespace: Union[Parser[Input, Any], Pattern, str, None] = missing
     ):
         if whitespace is missing:
             whitespace = mcs.default_whitespace
 
         if isinstance(whitespace, (str, bytes)):
             whitespace = re.compile(whitespace)
 
@@ -115,16 +123,17 @@
             setattr(options, key, value)
 
     def __new__(mcs, name, bases, dct, **_):  # noqa: N804
         return super().__new__(mcs, name, bases, dct)
 
     def __call__(cls, *args, **kwargs):
         raise TypeError(
-            "Parsers cannot be instantiated. They use class bodies purely as contexts for managing defaults and "
-            "allowing forward declarations. Access the individual parsers as static attributes."
+            "Parsers cannot be instantiated. They use class bodies purely as contexts for "
+            "managing defaults and allowing forward declarations. Access the individual parsers "
+            "as static attributes."
         )
 
 
 class ParserContext(metaclass=ParserContextMeta):
     """Context for parsing.
 
     This is not a real class. Don't instantiate it. This is used by inheriting
```

### Comparing `parsita-2.0.0b2/src/parsita/parsers/__init__.py` & `parsita-2.1.0/src/parsita/parsers/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,20 @@
 from ._alternative import FirstAlternativeParser, LongestAlternativeParser, first, longest
 from ._any import AnyParser, any1
-from ._base import Parser
+from ._base import Parser, wrap_literal
 from ._conversion import ConversionParser, TransformationParser
 from ._debug import DebugParser, debug
 from ._end_of_source import EndOfSourceParser, eof
 from ._literal import LiteralParser, lit
 from ._optional import OptionalParser, opt
 from ._predicate import PredicateParser, pred
 from ._regex import RegexParser, reg
 from ._repeated import RepeatedOnceParser, RepeatedParser, rep, rep1
-from ._repeated_seperated import RepeatedOnceSeparatedParser, RepeatedSeparatedParser, rep1sep, repsep
+from ._repeated_seperated import (
+    RepeatedOnceSeparatedParser,
+    RepeatedSeparatedParser,
+    rep1sep,
+    repsep,
+)
 from ._sequential import DiscardLeftParser, DiscardRightParser, SequentialParser
 from ._success import FailureParser, SuccessParser, failure, success
 from ._until import UntilParser, until
```

### Comparing `parsita-2.0.0b2/src/parsita/parsers/_alternative.py` & `parsita-2.1.0/src/parsita/parsers/_alternative.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 __all__ = ["FirstAlternativeParser", "first", "LongestAlternativeParser", "longest"]
 
 from typing import Generic, Optional, Sequence, Union
 
 from ..state import Continue, Input, Output, Reader, State
-from ._base import Parser
-from ._literal import lit
+from ._base import Parser, wrap_literal
 
 
 class FirstAlternativeParser(Generic[Input, Output], Parser[Input, Output]):
     def __init__(self, parser: Parser[Input, Output], *parsers: Parser[Input, Output]):
         super().__init__()
         self.parsers = (parser, *parsers)
 
-    def consume(self, state: State[Input], reader: Reader[Input]):
+    def _consume(self, state: State[Input], reader: Reader[Input]):
         for parser in self.parsers:
-            status = parser.cached_consume(state, reader)
+            status = parser.consume(state, reader)
             if isinstance(status, Continue):
                 return status
 
         return None
 
     def __repr__(self):
         names = []
         for parser in self.parsers:
             names.append(parser.name_or_repr())
 
         return self.name_or_nothing() + f"first({', '.join(names)})"
 
 
 def first(
-    parser: Union[Parser[Input, Output], Sequence[Input]], *parsers: Union[Parser[Input, Output], Sequence[Input]]
+    parser: Union[Parser[Input, Output], Sequence[Input]],
+    *parsers: Union[Parser[Input, Output], Sequence[Input]],
 ) -> FirstAlternativeParser[Input, Output]:
     """Match the first of several alternative parsers.
 
     A ``AlternativeParser`` attempts to match each supplied parser. If a parser
     succeeds, its result is immediately returned and later parsers are not
     attempted. If all parsers fail, a failure is returned.
 
@@ -41,43 +41,47 @@
     behavior of always returning the first parser to succeed is desired, this
     function should be used instead, because a future release of Parsita will
     change the behavior of `|` to use `longest` instead.
 
     Args:
         *parsers: Non-empty list of ``Parser``s or literals to try
     """
-    cleaned_parsers = [lit(parser_i) if isinstance(parser_i, str) else parser_i for parser_i in [parser, *parsers]]
+    cleaned_parsers = [wrap_literal(parser_i) for parser_i in [parser, *parsers]]
     return FirstAlternativeParser(*cleaned_parsers)
 
 
 class LongestAlternativeParser(Generic[Input, Output], Parser[Input, Output]):
     def __init__(self, parser: Parser[Input, Output], *parsers: Parser[Input, Output]):
         super().__init__()
         self.parsers = (parser, *parsers)
 
-    def consume(self, state: State[Input], reader: Reader[Input]):
+    def _consume(self, state: State[Input], reader: Reader[Input]):
         longest_success: Optional[Continue] = None
         for parser in self.parsers:
-            status = parser.cached_consume(state, reader)
+            status = parser.consume(state, reader)
             if isinstance(status, Continue):
-                if longest_success is None or status.remainder.position > longest_success.remainder.position:
+                if (
+                    longest_success is None
+                    or status.remainder.position > longest_success.remainder.position
+                ):
                     longest_success = status
 
         return longest_success
 
     def __repr__(self):
         names = []
         for parser in self.parsers:
             names.append(parser.name_or_repr())
 
         return self.name_or_nothing() + " | ".join(names)
 
 
 def longest(
-    parser: Union[Parser[Input, Output], Sequence[Input]], *parsers: Union[Parser[Input, Output], Sequence[Input]]
+    parser: Union[Parser[Input, Output], Sequence[Input]],
+    *parsers: Union[Parser[Input, Output], Sequence[Input]],
 ) -> LongestAlternativeParser[Input, Output]:
     """Match the longest of several alternative parsers.
 
     A ``LongestAlternativeParser`` attempts to match all supplied parsers. If
     multiple parsers succeed, the result of the one that makes the farthest
     successful progress is returned. If all parsers fail, a failure is returned.
     If multiple alternatives succeed with the same progress, the first one is
@@ -86,9 +90,9 @@
     Currently, the behavior of `|` matches `first`. If you desired returning the
     longest match instead of the first, use this function instead. A future
     release of Parsita will change the behavior of `|` to use `longest`.
 
     Args:
         *parsers: Non-empty list of ``Parser``s or literals to try
     """
-    cleaned_parsers = [lit(parser_i) if isinstance(parser_i, str) else parser_i for parser_i in [parser, *parsers]]
+    cleaned_parsers = [wrap_literal(parser_i) for parser_i in [parser, *parsers]]
     return LongestAlternativeParser(*cleaned_parsers)
```

### Comparing `parsita-2.0.0b2/src/parsita/parsers/_any.py` & `parsita-2.1.0/src/parsita/parsers/_any.py`

 * *Files 13% similar despite different names*

```diff
@@ -14,15 +14,17 @@
     later step, such as with the ``pred`` parser. This parser can only fail at
     the end of the stream.
     """
 
     def __init__(self):
         super().__init__()
 
-    def consume(self, state: State[Input], reader: Reader[Input]) -> Optional[Continue[Input, Input]]:
+    def _consume(
+        self, state: State[Input], reader: Reader[Input]
+    ) -> Optional[Continue[Input, Input]]:
         if reader.finished:
             state.register_failure("anything", reader)
             return None
         else:
             return Continue(reader.rest, reader.first)
 
     def __repr__(self):
```

### Comparing `parsita-2.0.0b2/src/parsita/parsers/_base.py` & `parsita-2.1.0/src/parsita/parsers/_base.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from __future__ import annotations
 
-__all__ = ["Parser"]
+__all__ = ["Parser", "wrap_literal"]
 
+from abc import abstractmethod
 from typing import Any, Generic, List, Optional, Sequence, Union
 
 from .. import options
 from ..state import (
     Continue,
     Failure,
     Input,
@@ -19,23 +20,30 @@
     Success,
 )
 
 # Singleton indicating that no result is yet in the memo
 missing = object()
 
 
+def wrap_literal(obj: Any) -> Parser:
+    from ._literal import LiteralParser
+
+    if isinstance(obj, Parser):
+        return obj
+    else:
+        return LiteralParser(obj, options.whitespace)
+
+
 class Parser(Generic[Input, Output]):
     """Abstract base class for all parser combinators.
 
     Inheritors of this class must:
 
-    1. Implement the ``consume`` method
+    1. Implement the ``_consume`` method
     2. Implement the ``__repr__`` method
-    3. Call super().__init__() in their constructor to get the parse method from
-       the context.
 
     Attributes:
         protected (bool): The metaclasses set this flag to true whenever a
             parser is assigned to a name. Operators that flatten the parsers
             they receive (``__or__`` and ``__and__``) will not flatten parsers
             with a ``True`` value here. This is most important for ``__and__``
             because there is no other way to tell that these two should be
@@ -53,30 +61,32 @@
             lists well or have unpacking that would let one unpack abc as
             [temp, c].
         name (Optional[str]): A name used by ``__str__`` and ``__repr__``.
             It is set by the context classes when a parser is assigned to a
             name.
     """
 
-    def cached_consume(self, state: State[Input], reader: Reader[Input]) -> Optional[Continue[Input, Output]]:
+    def consume(
+        self, state: State[Input], reader: Reader[Input]
+    ) -> Optional[Continue[Input, Output]]:
         """Match this parser at the given location.
 
         This is a concrete wrapper around ``consume``. This method implements
         the left-recursive packrat algorithm:
 
         1. Check the memo if this parser has already operated at this location
             a. Return the result immediately if it is there
         2. Put a ``None`` in the memo for this parser at this position
         3. Invoke ``consume``
         4. Put the result in the memo for this parser at this position
         5. Return the result
 
-        Individual parsers need to implement ``consume``, but not
-        ``cached_consume``. But all combinations should invoke
-        ``cached_consume`` instead of ``consume`` on their member parsers.
+        Individual parsers need to implement ``_consume``, but not ``consume``.
+        But all combinations should invoke ``consume`` instead of ``_consume``
+        on their member parsers.
 
         Args:
             state: The mutable state of the parse
             reader: The current state of the input
 
         Returns:
             If the pattern matches, a ``Continue`` is returned. If the pattern
@@ -86,21 +96,24 @@
         value = state.memo.get(key, missing)
 
         if value is not missing:
             return value
 
         state.memo[key] = None
 
-        result = self.consume(state, reader)
+        result = self._consume(state, reader)
 
         state.memo[key] = result
 
         return result
 
-    def consume(self, state: State[Input], reader: Reader[Input]) -> Optional[Continue[Input, Output]]:
+    @abstractmethod
+    def _consume(
+        self, state: State[Input], reader: Reader[Input]
+    ) -> Optional[Continue[Input, Output]]:
         """Abstract method for matching this parser at the given location.
 
         This is the central method of every parser combinator.
 
         Args:
             state: The mutable state of the parse
             reader: The current state of the input
@@ -108,26 +121,27 @@
         Returns:
             If the pattern matches, a ``Continue`` is returned. If the pattern
             does not match, a ``None`` is returned.
         """
         raise NotImplementedError()
 
     def parse(self, source: Union[Sequence[Input], Reader]) -> Result[Output]:
-        """Abstract method for completely parsing a source.
+        """Completely parse a source.
 
         Args:
             source: What will be parsed.
 
         Returns:
             If the parser succeeded in matching and consumed the entire output,
             the value from ``Continue`` is copied to make a ``Success``. If the
-            parser failed in matching, the error message is copied to a
-            ``Failure``. If the parser succeeded but the source was not
-            completely consumed, a ``Failure`` with a message indicating this
-            is returned.
+            parser failed in matching, the expected patterns at the farthest
+            point in the source are used to construct a ``ParseError`, which is
+            then used to contruct a ``Failure``. If the parser succeeded but the
+            source was not completely consumed, it returns a ``Failure`` with a
+            ``ParseError` indicating this.
 
         If a ``Reader`` is passed in, it is used directly. Otherwise, the source
         is converted to an appropriate ``Reader``. If the source is ``str`, a
         ``StringReader`` is used. Otherwise, a ``SequenceReader`` is used.
         """
         from ._end_of_source import eof
 
@@ -136,15 +150,15 @@
         elif isinstance(source, str):
             reader = StringReader(source, 0)
         else:
             reader = SequenceReader(source)
 
         state: State[Input] = State()
 
-        status = (self << eof).cached_consume(state, reader)
+        status = (self << eof).consume(state, reader)
 
         if isinstance(status, Continue):
             return Success(status.value)
         else:
             used = set()
             unique_expected = []
             for expected in state.expected:
@@ -166,73 +180,64 @@
 
     def name_or_nothing(self) -> Optional[str]:
         if self.name is None:
             return ""
         else:
             return self.name + " = "
 
-    @staticmethod
-    def handle_other(obj: Any) -> Parser:
-        from ._literal import LiteralParser
-
-        if isinstance(obj, Parser):
-            return obj
-        else:
-            return LiteralParser(obj, options.whitespace)
-
     def __or__(self, other) -> Parser:
         from ._alternative import LongestAlternativeParser
 
-        other = self.handle_other(other)
+        other = wrap_literal(other)
         parsers: List[Parser] = []
         if isinstance(self, LongestAlternativeParser) and not self.protected:
             parsers.extend(self.parsers)
         else:
             parsers.append(self)
         if isinstance(other, LongestAlternativeParser) and not other.protected:
             parsers.extend(other.parsers)
         else:
             parsers.append(other)
         return LongestAlternativeParser(*parsers)
 
     def __ror__(self, other) -> Parser:
-        other = self.handle_other(other)
+        other = wrap_literal(other)
         return other.__or__(self)
 
     def __and__(self, other) -> Parser:
         from ._sequential import SequentialParser
 
-        other = self.handle_other(other)
+        other = wrap_literal(other)
         if isinstance(self, SequentialParser) and not self.protected:
             return SequentialParser(*self.parsers, other)
         else:
             return SequentialParser(self, other)
 
     def __rand__(self, other) -> Parser:
-        other = self.handle_other(other)
+        other = wrap_literal(other)
         return other.__and__(self)
 
     def __rshift__(self, other) -> Parser:
         from ._sequential import DiscardLeftParser
 
-        other = self.handle_other(other)
+        other = wrap_literal(other)
         return DiscardLeftParser(self, other)
 
     def __rrshift__(self, other) -> Parser:
-        other = self.handle_other(other)
+        other = wrap_literal(other)
         return other.__rshift__(self)
 
     def __lshift__(self, other) -> Parser:
         from ._sequential import DiscardRightParser
 
-        other = self.handle_other(other)
+        other = wrap_literal(other)
         return DiscardRightParser(self, other)
 
     def __rlshift__(self, other) -> Parser:
-        other = self.handle_other(other)
+        other = wrap_literal(other)
         return other.__lshift__(self)
 
     def __gt__(self, other) -> Parser:
         from ._conversion import ConversionParser
 
         return ConversionParser(self, other)
```

### Comparing `parsita-2.0.0b2/src/parsita/parsers/_conversion.py` & `parsita-2.1.0/src/parsita/parsers/_conversion.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,32 +10,40 @@
 
 class ConversionParser(Generic[Input, Output, Convert], Parser[Input, Convert]):
     def __init__(self, parser: Parser[Input, Output], converter: Callable[[Output], Convert]):
         super().__init__()
         self.parser = parser
         self.converter = converter
 
-    def consume(self, state: State[Input], reader: Reader[Input]) -> Optional[Continue[Input, Convert]]:
-        status = self.parser.cached_consume(state, reader)
+    def _consume(
+        self, state: State[Input], reader: Reader[Input]
+    ) -> Optional[Continue[Input, Convert]]:
+        status = self.parser.consume(state, reader)
 
         if isinstance(status, Continue):
             return Continue(status.remainder, self.converter(status.value))
         else:
             return None
 
     def __repr__(self):
         return self.name_or_nothing() + repr(self.parser)
 
 
 class TransformationParser(Generic[Input, Output, Convert], Parser[Input, Convert]):
-    def __init__(self, parser: Parser[Input, Output], transformer: Callable[[Output], Parser[Input, Convert]]):
+    def __init__(
+        self,
+        parser: Parser[Input, Output],
+        transformer: Callable[[Output], Parser[Input, Convert]],
+    ):
         super().__init__()
         self.parser = parser
         self.transformer = transformer
 
-    def consume(self, state: State[Input], reader: Reader[Input]) -> Optional[Continue[Input, Convert]]:
-        status = self.parser.cached_consume(state, reader)
+    def _consume(
+        self, state: State[Input], reader: Reader[Input]
+    ) -> Optional[Continue[Input, Convert]]:
+        status = self.parser.consume(state, reader)
 
         if isinstance(status, Continue):
-            return self.transformer(status.value).cached_consume(state, status.remainder)
+            return self.transformer(status.value).consume(state, status.remainder)
         else:
             return status
```

### Comparing `parsita-2.0.0b2/src/parsita/parsers/_debug.py` & `parsita-2.1.0/src/parsita/parsers/_debug.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,37 +1,36 @@
 __all__ = ["DebugParser", "debug"]
 
 from typing import Callable, Generic, Optional
 
 from ..state import Input, Output, Reader, State
-from ._base import Parser
-from ._literal import lit
+from ._base import Parser, wrap_literal
 
 
 class DebugParser(Generic[Input, Output], Parser[Input, Output]):
     def __init__(
         self,
         parser: Parser[Input, Output],
         verbose: bool = False,
-        callback: Callable[[Parser[Input, Output], Reader[Input]], None] = None,
+        callback: Optional[Callable[[Parser[Input, Output], Reader[Input]], None]] = None,
     ):
         super().__init__()
         self.parser = parser
         self.verbose = verbose
         self.callback = callback
         self._parser_string = repr(parser)
 
-    def consume(self, state: State[Input], reader: Reader[Input]):
+    def _consume(self, state: State[Input], reader: Reader[Input]):
         if self.verbose:
             print(f"""Evaluating token {reader.next_token()} using parser {self._parser_string}""")
 
         if self.callback:
             self.callback(self.parser, reader)
 
-        result = self.parser.cached_consume(state, reader)
+        result = self.parser.consume(state, reader)
 
         if self.verbose:
             print(f"""Result {result!r}""")
 
         return result
 
     def __repr__(self):
@@ -58,10 +57,8 @@
             representation of ``parser`` and the next token before the
             invocation of ``parser``. After ``parser`` returns, the
             ``ParseResult`` returned is printed.
         callback: If not ``None``, is invoked immediately before ``parser`` is
             invoked. This allows the use to inspect the state of the input or
             add breakpoints before the possibly troublesome parser is invoked.
     """
-    if isinstance(parser, str):
-        parser = lit(parser)
-    return DebugParser(parser, verbose, callback)
+    return DebugParser(wrap_literal(parser), verbose, callback)
```

### Comparing `parsita-2.0.0b2/src/parsita/parsers/_end_of_source.py` & `parsita-2.1.0/src/parsita/parsers/_end_of_source.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,15 +6,17 @@
 from ._base import Parser
 
 
 class EndOfSourceParser(Generic[Input], Parser[Input, None]):
     def __init__(self):
         super().__init__()
 
-    def consume(self, state: State[Input], reader: Reader[Input]) -> Optional[Continue[Input, None]]:
+    def _consume(
+        self, state: State[Input], reader: Reader[Input]
+    ) -> Optional[Continue[Input, None]]:
         if reader.finished:
             return Continue(reader, None)
         else:
             state.register_failure("end of source", reader)
             return None
 
     def __repr__(self):
```

### Comparing `parsita-2.0.0b2/src/parsita/parsers/_literal.py` & `parsita-2.1.0/src/parsita/parsers/_literal.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,17 +9,17 @@
 
 class LiteralParser(Parser[Input, Input]):
     def __init__(self, pattern: Sequence[Input], whitespace: Optional[Parser[Input, Any]] = None):
         super().__init__()
         self.pattern = pattern
         self.whitespace = whitespace
 
-    def consume(self, state: State[Input], reader: Reader[Input]):
+    def _consume(self, state: State[Input], reader: Reader[Input]):
         if self.whitespace is not None:
-            status = self.whitespace.cached_consume(state, reader)
+            status = self.whitespace.consume(state, reader)
             reader = status.remainder
 
         if isinstance(reader, StringReader):
             if reader.source.startswith(self.pattern, reader.position):
                 reader = reader.drop(len(self.pattern))
             else:
                 state.register_failure(repr(self.pattern), reader)
@@ -32,15 +32,15 @@
                 elif elem == reader.first:
                     reader = reader.rest
                 else:
                     state.register_failure(str(elem), reader)
                     return None
 
         if self.whitespace is not None:
-            status = self.whitespace.cached_consume(state, reader)
+            status = self.whitespace.consume(state, reader)
             reader = status.remainder
 
         return Continue(reader, self.pattern)
 
     def __repr__(self):
         return self.name_or_nothing() + repr(self.pattern)
```

### Comparing `parsita-2.0.0b2/src/parsita/parsers/_optional.py` & `parsita-2.1.0/src/parsita/parsers/_optional.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 __all__ = ["OptionalParser", "opt"]
 
 from typing import Generic, List, Sequence, Union
 
 from ..state import Continue, Input, Output, Reader, State
-from ._base import Parser
-from ._literal import lit
+from ._base import Parser, wrap_literal
 
 
 class OptionalParser(Generic[Input, Output], Parser[Input, List[Output]]):
     def __init__(self, parser: Parser[Input, Output]):
         super().__init__()
         self.parser = parser
 
-    def consume(self, state: State[Input], reader: Reader[Input]):
-        status = self.parser.cached_consume(state, reader)
+    def _consume(self, state: State[Input], reader: Reader[Input]):
+        status = self.parser.consume(state, reader)
 
         if isinstance(status, Continue):
             return Continue(status.remainder, [status.value])
         else:
             return Continue(reader, [])
 
     def __repr__(self):
@@ -30,10 +29,8 @@
     An ``OptionalParser`` attempts to match ``parser``. If it succeeds, it
     returns a list of length one with the value returned by the parser as the
     only element. If it fails, it returns an empty list.
 
     Args:
         parser: Parser or literal
     """
-    if isinstance(parser, str):
-        parser = lit(parser)
-    return OptionalParser(parser)
+    return OptionalParser(wrap_literal(parser))
```

### Comparing `parsita-2.0.0b2/src/parsita/parsers/_predicate.py` & `parsita-2.1.0/src/parsita/parsers/_predicate.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 __all__ = ["PredicateParser", "pred"]
 
 from typing import Callable, Generic
 
 from ..state import Continue, Input, Output, Reader, State
-from ._base import Parser
+from ._base import Parser, wrap_literal
 
 
 class PredicateParser(Generic[Input, Output], Parser[Input, Input]):
-    def __init__(self, parser: Parser[Input, Output], predicate: Callable[[Output], bool], description: str):
+    def __init__(
+        self, parser: Parser[Input, Output], predicate: Callable[[Output], bool], description: str
+    ):
         super().__init__()
         self.parser = parser
         self.predicate = predicate
         self.description = description
 
-    def consume(self, state: State[Input], reader: Reader[Input]):
-        status = self.parser.cached_consume(state, reader)
+    def _consume(self, state: State[Input], reader: Reader[Input]):
+        status = self.parser.consume(state, reader)
         if isinstance(status, Continue):
             if self.predicate(status.value):
                 return status
             else:
                 state.register_failure(self.description, status.remainder)
                 return None
         else:
@@ -30,15 +32,15 @@
 
 def pred(
     parser: Parser[Input, Output], predicate: Callable[[Output], bool], description: str
 ) -> PredicateParser[Input, Output]:
     """Match ``parser``'s result if it satisfies the predicate.
 
     Args:
-        parser: Provides the result
+        parser: ``Parser`` or literal
         predicate: A predicate for the result to satisfy
         description: Name for the predicate, to use in error reporting
 
     Returns:
         A ``PredicateParser``.
     """
-    return PredicateParser(parser, predicate, description)
+    return PredicateParser(wrap_literal(parser), predicate, description)
```

### Comparing `parsita-2.0.0b2/src/parsita/parsers/_regex.py` & `parsita-2.1.0/src/parsita/parsers/_regex.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,30 +12,30 @@
 
 class RegexParser(Generic[StringType], Parser[StringType, StringType]):
     def __init__(self, pattern: re.Pattern, whitespace: Optional[Parser[StringType, Any]] = None):
         super().__init__()
         self.pattern = pattern
         self.whitespace = whitespace
 
-    def consume(self, state: State[StringType], reader: Reader[StringType]):
+    def _consume(self, state: State[StringType], reader: Reader[StringType]):
         if self.whitespace is not None:
-            status = self.whitespace.cached_consume(state, reader)
+            status = self.whitespace.consume(state, reader)
             reader = status.remainder
 
         match = self.pattern.match(reader.source, reader.position)
 
         if match is None:
             state.register_failure(f"r'{self.pattern.pattern}'", reader)
             return None
         else:
             value = reader.source[match.start() : match.end()]
             reader = reader.drop(len(value))
 
             if self.whitespace is not None:
-                status = self.whitespace.cached_consume(state, reader)
+                status = self.whitespace.consume(state, reader)
                 reader = status.remainder
 
             return Continue(reader, value)
 
     def __repr__(self):
         return self.name_or_nothing() + f"reg(r'{self.pattern.pattern}')"
```

### Comparing `parsita-2.0.0b2/src/parsita/parsers/_repeated.py` & `parsita-2.1.0/src/parsita/parsers/_repeated.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,73 +1,72 @@
 __all__ = ["RepeatedOnceParser", "rep1", "RepeatedParser", "rep"]
 
 from typing import Generic, List, Optional, Sequence, Union
 
 from ..state import Continue, Input, Output, Reader, RecursionError, State
-from ._base import Parser
-from ._literal import lit
+from ._base import Parser, wrap_literal
 
 
 class RepeatedOnceParser(Generic[Input, Output], Parser[Input, Sequence[Output]]):
     def __init__(self, parser: Parser[Input, Output]):
         super().__init__()
         self.parser = parser
 
-    def consume(self, state: State[Input], reader: Reader[Input]):
-        status = self.parser.cached_consume(state, reader)
+    def _consume(self, state: State[Input], reader: Reader[Input]):
+        status = self.parser.consume(state, reader)
 
         if status is None:
             return None
         else:
             output = [status.value]
             remainder = status.remainder
             while True:
-                status = self.parser.cached_consume(state, remainder)
+                status = self.parser.consume(state, remainder)
                 if isinstance(status, Continue):
                     if remainder.position == status.remainder.position:
                         raise RecursionError(self, remainder)
 
                     remainder = status.remainder
                     output.append(status.value)
                 else:
                     return Continue(remainder, output)
 
     def __repr__(self):
         return self.name_or_nothing() + f"rep1({self.parser.name_or_repr()})"
 
 
-def rep1(parser: Union[Parser[Input, Output], Sequence[Input]]) -> RepeatedOnceParser[Input, Output]:
+def rep1(
+    parser: Union[Parser[Input, Output], Sequence[Input]]
+) -> RepeatedOnceParser[Input, Output]:
     """Match a parser one or more times repeatedly.
 
     This matches ``parser`` multiple times in a row. If it matches as least
     once, it returns a list of values from each time ``parser`` matched. If it
     does not match ``parser`` at all, it fails. This parser is shorthand for
     ``rep(parser, min=1)``.
 
     Args:
         parser: Parser or literal
     """
-    if isinstance(parser, str):
-        parser = lit(parser)
-    return RepeatedOnceParser(parser)
+    return RepeatedOnceParser(wrap_literal(parser))
 
 
 class RepeatedParser(Generic[Input, Output], Parser[Input, Sequence[Output]]):
     def __init__(self, parser: Parser[Input, Output], *, min: int = 0, max: Optional[int] = None):
         super().__init__()
         self.parser = parser
         self.min = min
         self.max = max
 
-    def consume(self, state: State[Input], reader: Reader[Input]):
+    def _consume(self, state: State[Input], reader: Reader[Input]):
         output: List[Output] = []
         remainder = reader
 
         while self.max is None or len(output) < self.max:
-            status = self.parser.cached_consume(state, remainder)
+            status = self.parser.consume(state, remainder)
             if isinstance(status, Continue):
                 if remainder.position == status.remainder.position:
                     raise RecursionError(self, remainder)
 
                 remainder = status.remainder
                 output.append(status.value)
             else:
@@ -77,15 +76,16 @@
             return Continue(remainder, output)
         else:
             return None
 
     def __repr__(self):
         min_string = f", min={self.min}" if self.min > 0 else ""
         max_string = f", max={self.max}" if self.max is not None else ""
-        return self.name_or_nothing() + f"rep({self.parser.name_or_repr()}{min_string}{max_string})"
+        string = f"rep({self.parser.name_or_repr()}{min_string}{max_string})"
+        return self.name_or_nothing() + string
 
 
 def rep(
     parser: Union[Parser, Sequence[Input]], *, min: int = 0, max: Optional[int] = None
 ) -> RepeatedParser[Input, Output]:
     """Match a parser zero or more times repeatedly.
 
@@ -96,10 +96,8 @@
     Args:
         parser: Parser or literal
         min: Nonnegative integer defining the minimum number of entries matched
             before the parser can succeed
         max: Nonnegative integer defining the maximum number of entries that
             will be matched or ``None``, meaning that there is no limit
     """
-    if isinstance(parser, str):
-        parser = lit(parser)
-    return RepeatedParser(parser, min=min, max=max)
+    return RepeatedParser(wrap_literal(parser), min=min, max=max)
```

### Comparing `parsita-2.0.0b2/src/parsita/parsers/_repeated_seperated.py` & `parsita-2.1.0/src/parsita/parsers/_repeated_seperated.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 __all__ = ["RepeatedSeparatedParser", "repsep", "RepeatedOnceSeparatedParser", "rep1sep"]
 
 from typing import Any, Generic, Optional, Sequence, Union
 
 from ..state import Continue, Input, Output, Reader, RecursionError, State
-from ._base import Parser
-from ._literal import lit
+from ._base import Parser, wrap_literal
 
 
 class RepeatedSeparatedParser(Generic[Input, Output], Parser[Input, Sequence[Output]]):
     def __init__(
         self,
         parser: Parser[Input, Output],
         separator: Parser[Input, Any],
@@ -18,30 +17,32 @@
     ):
         super().__init__()
         self.parser = parser
         self.separator = separator
         self.min = min
         self.max = max
 
-    def consume(self, state: State[Input], reader: Reader[Input]):
-        status = self.parser.cached_consume(state, reader)
+    def _consume(self, state: State[Input], reader: Reader[Input]):
+        status = self.parser.consume(state, reader)
 
         if not isinstance(status, Continue):
             output = []
             remainder = reader
         else:
             output = [status.value]
             remainder = status.remainder
             while self.max is None or len(output) < self.max:
-                # If the separator matches, but the parser does not, the remainder from the last successful parser step
-                # must be used, not the remainder from any separator. That is why the parser starts from the remainder
-                # on the status, but remainder is not updated until after the parser succeeds.
-                status = self.separator.cached_consume(state, remainder)
+                # If the separator matches, but the parser does not, the
+                # remainder from the last successful parser step must be used,
+                # not the remainder from any separator. That is why the parser
+                # starts from the remainder on the status, but remainder is not
+                # updated until after the parser succeeds.
+                status = self.separator.consume(state, remainder)
                 if isinstance(status, Continue):
-                    status = self.parser.cached_consume(state, status.remainder)
+                    status = self.parser.consume(state, status.remainder)
                     if isinstance(status, Continue):
                         if remainder.position == status.remainder.position:
                             raise RecursionError(self, remainder)
 
                         remainder = status.remainder
                         output.append(status.value)
                     else:
@@ -51,20 +52,20 @@
 
         if len(output) >= self.min:
             return Continue(remainder, output)
         else:
             return None
 
     def __repr__(self):
+        rep_string = self.parser.name_or_repr()
+        sep_string = self.separator.name_or_repr()
         min_string = f", min={self.min}" if self.min > 0 else ""
         max_string = f", max={self.max}" if self.max is not None else ""
-        return (
-            self.name_or_nothing()
-            + f"repsep({self.parser.name_or_repr()}, {self.separator.name_or_repr()}{min_string}{max_string})"
-        )
+        string = f"repsep({rep_string}, {sep_string}{min_string}{max_string})"
+        return self.name_or_nothing() + string
 
 
 def repsep(
     parser: Union[Parser[Input, Output], Sequence[Input]],
     separator: Union[Parser[Input, Any], Sequence[Input]],
     *,
     min: int = 0,
@@ -81,69 +82,65 @@
         parser: Parser or literal
         separator: Parser or literal
         min: Nonnegative integer defining the minimum number of entries matched
             before the parser can succeed
         max: Nonnegative integer defining the maximum number of entries that
             will be matched or ``None``, meaning that there is no limit
     """
-    if isinstance(parser, str):
-        parser = lit(parser)
-    if isinstance(separator, str):
-        separator = lit(separator)
-    return RepeatedSeparatedParser(parser, separator, min=min, max=max)
+    return RepeatedSeparatedParser(wrap_literal(parser), wrap_literal(separator), min=min, max=max)
 
 
 class RepeatedOnceSeparatedParser(Generic[Input, Output], Parser[Input, Sequence[Output]]):
     def __init__(self, parser: Parser[Input, Output], separator: Parser[Input, Any]):
         super().__init__()
         self.parser = parser
         self.separator = separator
 
-    def consume(self, state: State[Input], reader: Reader[Input]):
-        status = self.parser.cached_consume(state, reader)
+    def _consume(self, state: State[Input], reader: Reader[Input]):
+        status = self.parser.consume(state, reader)
 
         if status is None:
             return None
         else:
             output = [status.value]
             remainder = status.remainder
             while True:
-                # If the separator matches, but the parser does not, the remainder from the last successful parser step
-                # must be used, not the remainder from any separator. That is why the parser starts from the remainder
-                # on the status, but remainder is not updated until after the parser succeeds.
-                status = self.separator.cached_consume(state, remainder)
+                # If the separator matches, but the parser does not, the
+                # remainder from the last successful parser step must be used,
+                # not the remainder from any separator. That is why the parser
+                # starts from the remainder on the status, but remainder is not
+                # updated until after the parser succeeds.
+                status = self.separator.consume(state, remainder)
                 if isinstance(status, Continue):
-                    status = self.parser.cached_consume(state, status.remainder)
+                    status = self.parser.consume(state, status.remainder)
                     if isinstance(status, Continue):
                         if remainder.position == status.remainder.position:
                             raise RecursionError(self, remainder)
 
                         remainder = status.remainder
                         output.append(status.value)
                     else:
                         return Continue(remainder, output)
                 else:
                     return Continue(remainder, output)
 
     def __repr__(self):
-        return self.name_or_nothing() + f"rep1sep({self.parser.name_or_repr()}, {self.separator.name_or_repr()})"
+        string = f"rep1sep({self.parser.name_or_repr()}, {self.separator.name_or_repr()})"
+        return self.name_or_nothing() + string
 
 
 def rep1sep(
-    parser: Union[Parser[Input, Output], Sequence[Input]], separator: Union[Parser[Input, Any], Sequence[Input]]
+    parser: Union[Parser[Input, Output], Sequence[Input]],
+    separator: Union[Parser[Input, Any], Sequence[Input]],
 ) -> RepeatedOnceSeparatedParser[Input, Output]:
     """Match a parser one or more times separated by another parser.
 
     This matches repeated sequences of ``parser`` separated by ``separator``.
     If there is at least one match, a list containing the values of the
     ``parser`` matches is returned. The values from ``separator`` are discarded.
     If it does not match ``parser`` at all, it fails.
 
     Args:
         parser: Parser or literal
         separator: Parser or literal
     """
-    if isinstance(parser, str):
-        parser = lit(parser)
-    if isinstance(separator, str):
-        separator = lit(separator)
-    return RepeatedOnceSeparatedParser(parser, separator)
+    return RepeatedOnceSeparatedParser(wrap_literal(parser), wrap_literal(separator))
```

### Comparing `parsita-2.0.0b2/src/parsita/parsers/_sequential.py` & `parsita-2.1.0/src/parsita/parsers/_sequential.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,25 +2,26 @@
 
 from typing import Any, Generic, List
 
 from ..state import Continue, Input, Output, Reader, State
 from ._base import Parser
 
 
-class SequentialParser(Generic[Input], Parser[Input, List[Any]]):  # Type of this class is inexpressible
+# Type of this class is inexpressible
+class SequentialParser(Generic[Input], Parser[Input, List[Any]]):
     def __init__(self, parser: Parser[Input, Any], *parsers: Parser[Input, Any]):
         super().__init__()
         self.parsers = (parser, *parsers)
 
-    def consume(self, state: State[Input], reader: Reader[Input]):
+    def _consume(self, state: State[Input], reader: Reader[Input]):
         output = []
         remainder = reader
 
         for parser in self.parsers:
-            status = parser.cached_consume(state, remainder)
+            status = parser.consume(state, remainder)
             if isinstance(status, Continue):
                 output.append(status.value)
                 remainder = status.remainder
             else:
                 return None
 
         return Continue(remainder, output)
@@ -35,37 +36,39 @@
 
 class DiscardLeftParser(Generic[Input, Output], Parser[Input, Output]):
     def __init__(self, left: Parser[Input, Any], right: Parser[Input, Output]):
         super().__init__()
         self.left = left
         self.right = right
 
-    def consume(self, state: State[Input], reader: Reader[Input]):
-        status = self.left.cached_consume(state, reader)
+    def _consume(self, state: State[Input], reader: Reader[Input]):
+        status = self.left.consume(state, reader)
         if isinstance(status, Continue):
-            return self.right.cached_consume(state, status.remainder)
+            return self.right.consume(state, status.remainder)
         else:
             return None
 
     def __repr__(self):
-        return self.name_or_nothing() + f"{self.left.name_or_repr()} >> {self.right.name_or_repr()}"
+        string = f"{self.left.name_or_repr()} >> {self.right.name_or_repr()}"
+        return self.name_or_nothing() + string
 
 
 class DiscardRightParser(Generic[Input, Output], Parser[Input, Output]):
     def __init__(self, left: Parser[Input, Output], right: Parser[Input, Any]):
         super().__init__()
         self.left = left
         self.right = right
 
-    def consume(self, state: State[Input], reader: Reader[Input]):
-        status1 = self.left.cached_consume(state, reader)
+    def _consume(self, state: State[Input], reader: Reader[Input]):
+        status1 = self.left.consume(state, reader)
         if isinstance(status1, Continue):
-            status2 = self.right.cached_consume(state, status1.remainder)
+            status2 = self.right.consume(state, status1.remainder)
             if isinstance(status2, Continue):
                 return Continue(status2.remainder, status1.value)
             else:
                 return None
         else:
             return None
 
     def __repr__(self):
-        return self.name_or_nothing() + f"{self.left.name_or_repr()} << {self.right.name_or_repr()}"
+        string = f"{self.left.name_or_repr()} << {self.right.name_or_repr()}"
+        return self.name_or_nothing() + string
```

### Comparing `parsita-2.0.0b2/src/parsita/parsers/_success.py` & `parsita-2.1.0/src/parsita/parsers/_success.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 
 class SuccessParser(Generic[Input, Output], Parser[Any, Output]):
     def __init__(self, value: Output):
         super().__init__()
         self.value = value
 
-    def consume(self, state: State[Input], reader: Reader[Input]) -> Continue[Input, Output]:
+    def _consume(self, state: State[Input], reader: Reader[Input]) -> Continue[Input, Output]:
         return Continue(reader, self.value)
 
     def __repr__(self):
         return self.name_or_nothing() + f"success({self.value!r})"
 
 
 def success(value: Output) -> SuccessParser[Input, Output]:
@@ -32,15 +32,15 @@
 
 
 class FailureParser(Generic[Input], Parser[Input, NoReturn]):
     def __init__(self, expected: str):
         super().__init__()
         self.expected = expected
 
-    def consume(self, state: State[Input], reader: Reader[Input]) -> None:
+    def _consume(self, state: State[Input], reader: Reader[Input]) -> None:
         state.register_failure(self.expected, reader)
         return None
 
     def __repr__(self):
         return self.name_or_nothing() + f"failure({self.expected!r})"
```

### Comparing `parsita-2.0.0b2/src/parsita/parsers/_until.py` & `parsita-2.1.0/src/parsita/parsers/_until.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 __all__ = ["UntilParser", "until"]
 
 from typing import Any, Generic
 
 from ..state import Continue, Input, Output, Reader, State
-from ._base import Parser
-from ._literal import lit
+from ._base import Parser, wrap_literal
 
 
 class UntilParser(Generic[Input], Parser[Input, Input]):
     def __init__(self, parser: Parser[Input, Any]):
         super().__init__()
         self.parser = parser
 
-    def consume(self, state: State[Input], reader: Reader[Input]):
+    def _consume(self, state: State[Input], reader: Reader[Input]):
         start_position = reader.position
         while True:
-            status = self.parser.cached_consume(state, reader)
+            status = self.parser.consume(state, reader)
 
             if isinstance(status, Continue):
                 break
             elif reader.finished:
                 return status
             else:
                 reader = reader.rest
@@ -35,10 +34,8 @@
 
     This parser matches all input until it encounters a position in the input
     where the given ``parser`` succeeds.
 
     Args:
         parser: Parser or literal
     """
-    if isinstance(parser, str):
-        parser = lit(parser)
-    return UntilParser(parser)
+    return UntilParser(wrap_literal(parser))
```

### Comparing `parsita-2.0.0b2/src/parsita/state/_exceptions.py` & `parsita-2.1.0/src/parsita/state/_exceptions.py`

 * *Files identical despite different names*

### Comparing `parsita-2.0.0b2/src/parsita/state/_reader.py` & `parsita-2.1.0/src/parsita/state/_reader.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,15 +62,18 @@
             A full error message
         """
         expected_string = " or ".join(expected)
 
         if self.finished:
             return f"Expected {expected_string} but found end of source"
         else:
-            return f"Expected {expected_string} but found {self.next_token()} at index {self.position}"
+            return (
+                f"Expected {expected_string} but found {self.next_token()} "
+                f"at index {self.position}"
+            )
 
     def recursion_error(self, repeated_parser: str):
         """Generate an error to indicate that infinite recursion was encountered.
 
         A parser can supply a representation of itself to this method and the
         reader will supply the context, including the location where the
         parser stalled.
@@ -80,21 +83,21 @@
 
         Returns:
             A full error message
         """
 
         if self.finished:
             return (
-                f"Infinite recursion detected in {repeated_parser}; empty string was matched and will be matched "
-                "forever at end of source"
+                f"Infinite recursion detected in {repeated_parser}; "
+                "empty string was matched and will be matched forever at end of source"
             )
         else:
             return (
-                f"Infinite recursion detected in {repeated_parser}; empty string was matched and will be matched "
-                f"forever at index {self.position} before {self.next_token()}"
+                f"Infinite recursion detected in {repeated_parser}; empty string was matched "
+                f"and will be matched forever at index {self.position} before {self.next_token()}"
             )
 
 
 @dataclass(frozen=True)
 class SequenceReader(Reader[Input]):
     """A reader for sequences that should not be sliced.
 
@@ -123,15 +126,16 @@
     def finished(self) -> bool:
         return self.position >= len(self.source)
 
     def drop(self, count: int) -> SequenceReader[Input]:
         return SequenceReader(self.source, self.position + count)
 
 
-# Python lacks character type, so "str" will be used for both the sequence and the elements
+# Python lacks character type, so "str" will be used for both the sequence and
+# the elements
 @dataclass(frozen=True)
 class StringReader(Reader[str]):
     """A reader for strings.
 
     Python's regular expressions and string operations only work on strings,
     not abstract "readers". This class defines the source as a string so that
     regular expressions (and string literals) can safely and efficiently work
@@ -165,15 +169,15 @@
     def next_token(self) -> str:
         match = self.next_token_regex.match(self.source, self.position)
         if match is None:
             return self.source[self.position]
         else:
             return self.source[match.start() : match.end()]
 
-    def current_line(self):
+    def _current_line(self):
         # StringIO is not consistent in how it treats empty strings
         # and other strings not ending in newlines. Ensure that the
         # source always ends in a newline.
         # This also ensures that the loop below runs at least once
         # and that `line` always ends with a newline.
         if not self.source.endswith("\n"):
             source = self.source + "\n"
@@ -215,15 +219,15 @@
         expected_string = " or ".join(expected)
 
         if self.finished:
             next_string = "end of source"
         else:
             next_string = repr(self.next_token())
 
-        line_index, character_index, line, pointer = self.current_line()
+        line_index, character_index, line, pointer = self._current_line()
 
         return (
             f"Expected {expected_string} but found {next_string}\n"
             f"Line {line_index}, character {character_index}\n\n{line}{pointer}"
         )
 
     def recursion_error(self, repeated_parser: str):
@@ -235,13 +239,14 @@
 
         Args:
             repeated_parser: A representation of the repeated parser
 
         Returns:
             A full error message
         """
-        line_index, character_index, line, pointer = self.current_line()
+        line_index, character_index, line, pointer = self._current_line()
 
         return (
-            f"Infinite recursion detected in {repeated_parser}; empty string was matched and will be matched "
-            f"forever\nLine {line_index}, character {character_index}\n\n{line}{pointer}"
+            f"Infinite recursion detected in {repeated_parser}; "
+            "empty string was matched and will be matched forever\n"
+            f"Line {line_index}, character {character_index}\n\n{line}{pointer}"
         )
```

### Comparing `parsita-2.0.0b2/src/parsita/state/_state.py` & `parsita-2.1.0/src/parsita/state/_state.py`

 * *Files identical despite different names*

### Comparing `parsita-2.0.0b2/src/parsita/util.py` & `parsita-2.1.0/src/parsita/util.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,32 +8,33 @@
 def constant(x: A) -> Callable[..., A]:
     """Produce a function that always returns a supplied value.
 
     Args:
         x: Any object.
 
     Returns:
-        A function that accepts any number of positional and keyword arguments, discards them, and returns ``x``.
+        A function that accepts any number of positional and keyword arguments,
+        discards them, and returns ``x``.
     """
 
     def constanted(*args, **kwargs):
         return x
 
     return constanted
 
 
 def splat(f: Callable[..., A]) -> Callable[[Iterable], A]:
-    """Convert a function taking multiple arguments into a function taking a single iterable argument.
+    """Convert a function of multiple arguments into a function of a single iterable argument.
 
     Args:
         f: Any function
 
     Returns:
-        A function that accepts a single iterable argument. Each element of this iterable argument is passed as an
-        argument to ``f``.
+        A function that accepts a single iterable argument. Each element of this
+        iterable argument is passed as an argument to ``f``.
 
     Example:
         $ def f(a, b, c):
         $     return a + b + c
         $
         $ f(1, 2, 3)  # 6
         $ g = splat(f)
@@ -43,22 +44,22 @@
     def splatted(args):
         return f(*args)
 
     return splatted
 
 
 def unsplat(f: Callable[[Iterable], A]) -> Callable[..., A]:
-    """Convert a function taking a single iterable argument into a function taking multiple arguments.
+    """Convert a function of a single iterable argument into a function of multiple arguments.
 
     Args:
         f: Any function taking a single iterable argument
 
     Returns:
-        A function that accepts multiple arguments. Each argument of this function is passed as an element of an
-        iterable to ``f``.
+        A function that accepts multiple arguments. Each argument of this
+        function is passed as an element of an iterable to ``f``.
 
     Example:
         $ def f(a):
         $     return a[0] + a[1] + a[2]
         $
         $ f([1, 2, 3])  # 6
         $ g = unsplat(f)
```

### Comparing `parsita-2.0.0b2/PKG-INFO` & `parsita-2.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: parsita
-Version: 2.0.0b2
+Version: 2.1.0
 Summary: Parser combinator library for Python
 Home-page: https://github.com/drhagen/parsita
 License: MIT
 Keywords: text,parsing,parser,combinator
 Author: David Hagen
 Author-email: david@drhagen.com
 Requires-Python: >=3.8.0,<4.0.0
```

