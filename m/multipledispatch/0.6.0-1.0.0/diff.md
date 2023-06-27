# Comparing `tmp/multipledispatch-0.6.0.tar.gz` & `tmp/multipledispatch-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/multipledispatch-0.6.0.tar", last modified: Wed Aug  8 17:56:54 2018, max compression
+gzip compressed data, was "multipledispatch-1.0.0.tar", last modified: Tue Jun 27 16:29:25 2023, max compression
```

## Comparing `multipledispatch-0.6.0.tar` & `multipledispatch-1.0.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 phillip   (1000) phillip   (1001)        0 2018-08-08 17:56:54.000000 multipledispatch-0.6.0/
--rw-r--r--   0 phillip   (1000) phillip   (1001)       38 2018-08-08 17:56:54.000000 multipledispatch-0.6.0/setup.cfg
-drwxr-xr-x   0 phillip   (1000) phillip   (1001)        0 2018-08-08 17:56:54.000000 multipledispatch-0.6.0/multipledispatch/
--rw-r--r--   0 phillip   (1000) phillip   (1001)     3630 2018-08-08 16:21:20.000000 multipledispatch-0.6.0/multipledispatch/utils.py
--rw-r--r--   0 phillip   (1000) phillip   (1001)     2752 2018-08-08 16:21:20.000000 multipledispatch-0.6.0/multipledispatch/variadic.py
--rw-r--r--   0 phillip   (1000) phillip   (1001)     3912 2018-08-08 16:21:20.000000 multipledispatch-0.6.0/multipledispatch/conflict.py
--rw-r--r--   0 phillip   (1000) phillip   (1001)     2148 2018-08-08 16:21:20.000000 multipledispatch-0.6.0/multipledispatch/core.py
--rw-r--r--   0 phillip   (1000) phillip   (1001)    13562 2018-08-08 16:21:20.000000 multipledispatch-0.6.0/multipledispatch/dispatcher.py
--rw-r--r--   0 phillip   (1000) phillip   (1001)      147 2018-08-08 17:53:22.000000 multipledispatch-0.6.0/multipledispatch/__init__.py
--rw-r--r--   0 phillip   (1000) phillip   (1001)     3734 2018-08-08 16:21:20.000000 multipledispatch-0.6.0/README.rst
--rwxr-xr-x   0 phillip   (1000) phillip   (1001)      596 2018-08-08 16:21:20.000000 multipledispatch-0.6.0/setup.py
--rw-r--r--   0 phillip   (1000) phillip   (1001)     5126 2018-08-08 17:56:54.000000 multipledispatch-0.6.0/PKG-INFO
-drwxr-xr-x   0 phillip   (1000) phillip   (1001)        0 2018-08-08 17:56:54.000000 multipledispatch-0.6.0/multipledispatch.egg-info/
--rw-r--r--   0 phillip   (1000) phillip   (1001)       17 2018-08-08 17:56:54.000000 multipledispatch-0.6.0/multipledispatch.egg-info/top_level.txt
--rw-r--r--   0 phillip   (1000) phillip   (1001)      426 2018-08-08 17:56:54.000000 multipledispatch-0.6.0/multipledispatch.egg-info/SOURCES.txt
--rw-r--r--   0 phillip   (1000) phillip   (1001)        4 2018-08-08 17:56:54.000000 multipledispatch-0.6.0/multipledispatch.egg-info/requires.txt
--rw-r--r--   0 phillip   (1000) phillip   (1001)     5126 2018-08-08 17:56:54.000000 multipledispatch-0.6.0/multipledispatch.egg-info/PKG-INFO
--rw-r--r--   0 phillip   (1000) phillip   (1001)        1 2018-08-08 17:56:54.000000 multipledispatch-0.6.0/multipledispatch.egg-info/dependency_links.txt
--rw-r--r--   0 phillip   (1000) phillip   (1001)        1 2018-08-08 17:56:54.000000 multipledispatch-0.6.0/multipledispatch.egg-info/not-zip-safe
+drwxr-xr-x   0 mrocklin   (502) staff       (20)        0 2023-06-27 16:29:25.667105 multipledispatch-1.0.0/
+-rw-r--r--   0 mrocklin   (502) staff       (20)     1503 2023-06-27 15:26:33.000000 multipledispatch-1.0.0/LICENSE.txt
+-rw-r--r--   0 mrocklin   (502) staff       (20)     3798 2023-06-27 16:29:25.667170 multipledispatch-1.0.0/PKG-INFO
+-rw-r--r--   0 mrocklin   (502) staff       (20)     3539 2023-06-27 16:20:43.000000 multipledispatch-1.0.0/README.rst
+drwxr-xr-x   0 mrocklin   (502) staff       (20)        0 2023-06-27 16:29:25.666208 multipledispatch-1.0.0/multipledispatch/
+-rw-r--r--   0 mrocklin   (502) staff       (20)      162 2023-06-27 15:30:08.000000 multipledispatch-1.0.0/multipledispatch/__init__.py
+-rw-r--r--   0 mrocklin   (502) staff       (20)     3833 2023-06-27 15:30:08.000000 multipledispatch-1.0.0/multipledispatch/conflict.py
+-rw-r--r--   0 mrocklin   (502) staff       (20)     2267 2023-06-27 15:30:08.000000 multipledispatch-1.0.0/multipledispatch/core.py
+-rw-r--r--   0 mrocklin   (502) staff       (20)    13492 2023-06-27 15:30:08.000000 multipledispatch-1.0.0/multipledispatch/dispatcher.py
+-rw-r--r--   0 mrocklin   (502) staff       (20)     3594 2023-06-27 15:30:08.000000 multipledispatch-1.0.0/multipledispatch/utils.py
+-rw-r--r--   0 mrocklin   (502) staff       (20)     2725 2023-06-27 16:20:43.000000 multipledispatch-1.0.0/multipledispatch/variadic.py
+drwxr-xr-x   0 mrocklin   (502) staff       (20)        0 2023-06-27 16:29:25.667009 multipledispatch-1.0.0/multipledispatch.egg-info/
+-rw-r--r--   0 mrocklin   (502) staff       (20)     3798 2023-06-27 16:29:25.000000 multipledispatch-1.0.0/multipledispatch.egg-info/PKG-INFO
+-rw-r--r--   0 mrocklin   (502) staff       (20)      409 2023-06-27 16:29:25.000000 multipledispatch-1.0.0/multipledispatch.egg-info/SOURCES.txt
+-rw-r--r--   0 mrocklin   (502) staff       (20)        1 2023-06-27 16:29:25.000000 multipledispatch-1.0.0/multipledispatch.egg-info/dependency_links.txt
+-rw-r--r--   0 mrocklin   (502) staff       (20)        1 2023-06-27 16:29:25.000000 multipledispatch-1.0.0/multipledispatch.egg-info/not-zip-safe
+-rw-r--r--   0 mrocklin   (502) staff       (20)       17 2023-06-27 16:29:25.000000 multipledispatch-1.0.0/multipledispatch.egg-info/top_level.txt
+-rw-r--r--   0 mrocklin   (502) staff       (20)       84 2023-06-27 16:29:25.667498 multipledispatch-1.0.0/setup.cfg
+-rwxr-xr-x   0 mrocklin   (502) staff       (20)      483 2023-06-27 16:28:26.000000 multipledispatch-1.0.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `multipledispatch-0.6.0/multipledispatch/utils.py` & `multipledispatch-1.0.0/multipledispatch/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
         rest = expand_tuples(L[1:])
         return [(item,) + t for t in rest for item in L[0]]
 
 
 # Taken from theano/theano/gof/sched.py
 # Avoids licensing issues because this was written by Matthew Rocklin
 def _toposort(edges):
-    """ Topological sort algorithm by Kahn [1] - O(nodes + vertices)
+    """Topological sort algorithm by Kahn [1] - O(nodes + vertices)
 
     inputs:
         edges - a dict of the form {a: {b, c}} where b and c depend on a
     outputs:
         L - an ordered list of nodes that satisfy the dependencies of edges
 
     >>> _toposort({1: (2, 3), 2: (3, )})
@@ -44,16 +44,15 @@
     Closely follows the wikipedia page [2]
 
     [1] Kahn, Arthur B. (1962), "Topological sorting of large networks",
     Communications of the ACM
     [2] http://en.wikipedia.org/wiki/Toposort#Algorithms
     """
     incoming_edges = reverse_dict(edges)
-    incoming_edges = OrderedDict((k, set(val))
-                                 for k, val in incoming_edges.items())
+    incoming_edges = OrderedDict((k, set(val)) for k, val in incoming_edges.items())
     S = OrderedDict.fromkeys(v for v in edges if v not in incoming_edges)
     L = []
 
     while S:
         n, _ = S.popitem()
         L.append(n)
         for m in edges.get(n, ()):
@@ -78,22 +77,22 @@
         dict order. So this function output order should be considered
         as undeterministic.
 
     """
     result = OrderedDict()
     for key in d:
         for val in d[key]:
-            result[val] = result.get(val, tuple()) + (key, )
+            result[val] = result.get(val, tuple()) + (key,)
     return result
 
 
 # Taken from toolz
 # Avoids licensing issues because this version was authored by Matthew Rocklin
 def groupby(func, seq):
-    """ Group a collection by a key function
+    """Group a collection by a key function
 
     >>> names = ['Alice', 'Bob', 'Charlie', 'Dan', 'Edith', 'Frank']
     >>> groupby(len, names)  # doctest: +SKIP
     {3: ['Bob', 'Dan'], 5: ['Alice', 'Edith', 'Frank'], 7: ['Charlie']}
 
     >>> iseven = lambda x: x % 2 == 0
     >>> groupby(iseven, [1, 2, 3, 4, 5, 6, 7, 8])  # doctest: +SKIP
@@ -132,8 +131,8 @@
     '(int, float)'
     """
     try:
         return type.__name__
     except AttributeError:
         if len(type) == 1:
             return typename(*type)
-        return '(%s)' % ', '.join(map(typename, type))
+        return "(%s)" % ", ".join(map(typename, type))
```

### Comparing `multipledispatch-0.6.0/multipledispatch/variadic.py` & `multipledispatch-1.0.0/multipledispatch/variadic.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,14 @@
-import six
-
-from .utils import typename
+from multipledispatch.utils import typename
 
 
 class VariadicSignatureType(type):
     # checking if subclass is a subclass of self
     def __subclasscheck__(self, subclass):
-        other_type = (subclass.variadic_type if isvariadic(subclass)
-                      else (subclass,))
+        other_type = subclass.variadic_type if isvariadic(subclass) else (subclass,)
         return subclass is self or all(
             issubclass(other, self.variadic_type) for other in other_type
         )
 
     def __eq__(self, other):
         """
         Return True if other has the same variadic type
@@ -22,16 +19,15 @@
             The object (type) to check
 
         Returns
         -------
         bool
             Whether or not `other` is equal to `self`
         """
-        return (isvariadic(other) and
-                set(self.variadic_type) == set(other.variadic_type))
+        return isvariadic(other) and set(self.variadic_type) == set(other.variadic_type)
 
     def __hash__(self):
         return hash((type(self), frozenset(self.variadic_type)))
 
 
 def isvariadic(obj):
     """Check whether the type `obj` is variadic.
@@ -57,29 +53,32 @@
 
 
 class VariadicSignatureMeta(type):
     """A metaclass that overrides ``__getitem__`` on the class. This is used to
     generate a new type for Variadic signatures. See the Variadic class for
     examples of how this behaves.
     """
+
     def __getitem__(self, variadic_type):
         if not (isinstance(variadic_type, (type, tuple)) or type(variadic_type)):
-            raise ValueError("Variadic types must be type or tuple of types"
-                             " (Variadic[int] or Variadic[(int, float)]")
+            raise ValueError(
+                "Variadic types must be type or tuple of types"
+                " (Variadic[int] or Variadic[(int, float)]"
+            )
 
         if not isinstance(variadic_type, tuple):
-            variadic_type = variadic_type,
+            variadic_type = (variadic_type,)
         return VariadicSignatureType(
-            'Variadic[%s]' % typename(variadic_type),
+            "Variadic[%s]" % typename(variadic_type),
             (),
-            dict(variadic_type=variadic_type, __slots__=())
+            dict(variadic_type=variadic_type, __slots__=()),
         )
 
 
-class Variadic(six.with_metaclass(VariadicSignatureMeta)):
+class Variadic(metaclass=VariadicSignatureMeta):
     """A class whose getitem method can be used to generate a new type
     representing a specific variadic signature.
 
     Examples
     --------
     >>> Variadic[int]  # any number of int arguments
     <class 'multipledispatch.variadic.Variadic[int]'>
```

### Comparing `multipledispatch-0.6.0/multipledispatch/conflict.py` & `multipledispatch-1.0.0/multipledispatch/conflict.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 
 class AmbiguityWarning(Warning):
     pass
 
 
 def supercedes(a, b):
-    """ A is consistent and strictly more specific than B """
+    """A is consistent and strictly more specific than B"""
     if len(a) < len(b):
         # only case is if a is empty and b is variadic
         return not a and len(b) == 1 and isvariadic(b[-1])
     elif len(a) == len(b):
         return all(map(issubclass, a, b))
     else:
         # len(a) > len(b)
@@ -33,26 +33,25 @@
                 if not issubclass(cur_a, cur_b):
                     return False
                 p1 += 1
         return p2 == len(b) - 1 and p1 == len(a)
 
 
 def consistent(a, b):
-    """ It is possible for an argument list to satisfy both A and B """
+    """It is possible for an argument list to satisfy both A and B"""
 
     # Need to check for empty args
     if not a:
         return not b or isvariadic(b[0])
     if not b:
         return not a or isvariadic(a[0])
 
     # Non-empty args check for mutual subclasses
     if len(a) == len(b):
-        return all(issubclass(aa, bb) or issubclass(bb, aa)
-                   for aa, bb in zip(a, b))
+        return all(issubclass(aa, bb) or issubclass(bb, aa) for aa, bb in zip(a, b))
     else:
         p1 = 0
         p2 = 0
         while p1 < len(a) and p2 < len(b):
             cur_a = a[p1]
             cur_b = b[p2]
             if not issubclass(cur_b, cur_a) and not issubclass(cur_a, cur_b):
@@ -62,56 +61,57 @@
                 p2 += 1
             elif isvariadic(cur_a):
                 p2 += 1
             elif isvariadic(cur_b):
                 p1 += 1
         # We only need to check for variadic ends
         # Variadic types are guaranteed to be the last element
-        return (isvariadic(cur_a) and p2 == len(b) or
-                isvariadic(cur_b) and p1 == len(a))
+        return isvariadic(cur_a) and p2 == len(b) or isvariadic(cur_b) and p1 == len(a)
 
 
 def ambiguous(a, b):
-    """ A is consistent with B but neither is strictly more specific """
+    """A is consistent with B but neither is strictly more specific"""
     return consistent(a, b) and not (supercedes(a, b) or supercedes(b, a))
 
 
 def ambiguities(signatures):
-    """ All signature pairs such that A is ambiguous with B """
+    """All signature pairs such that A is ambiguous with B"""
     signatures = list(map(tuple, signatures))
-    return set((a, b) for a in signatures for b in signatures
-               if hash(a) < hash(b)
-               and ambiguous(a, b)
-               and not any(supercedes(c, a) and supercedes(c, b)
-                           for c in signatures))
+    return set(
+        (a, b)
+        for a in signatures
+        for b in signatures
+        if hash(a) < hash(b)
+        and ambiguous(a, b)
+        and not any(supercedes(c, a) and supercedes(c, b) for c in signatures)
+    )
 
 
 def super_signature(signatures):
-    """ A signature that would break ambiguities """
+    """A signature that would break ambiguities"""
     n = len(signatures[0])
     assert all(len(s) == n for s in signatures)
 
-    return [max([type.mro(sig[i]) for sig in signatures], key=len)[0]
-            for i in range(n)]
+    return [max([type.mro(sig[i]) for sig in signatures], key=len)[0] for i in range(n)]
 
 
 def edge(a, b, tie_breaker=hash):
-    """ A should be checked before B
+    """A should be checked before B
 
     Tie broken by tie_breaker, defaults to ``hash``
     """
     # A either supercedes B and B does not supercede A or if B does then call
     # tie_breaker
     return supercedes(a, b) and (
         not supercedes(b, a) or tie_breaker(a) > tie_breaker(b)
     )
 
 
 def ordering(signatures):
-    """ A sane ordering of signatures to check, first to last
+    """A sane ordering of signatures to check, first to last
 
     Topoological sort of edges as given by ``edge`` and ``supercedes``
     """
     signatures = list(map(tuple, signatures))
     edges = [(a, b) for a in signatures for b in signatures if edge(a, b)]
     edges = groupby(lambda x: x[0], edges)
     for s in signatures:
```

### Comparing `multipledispatch-0.6.0/multipledispatch/core.py` & `multipledispatch-1.0.0/multipledispatch/core.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import inspect
+import sys
 
 from .dispatcher import Dispatcher, MethodDispatcher, ambiguity_warn
 
 global_namespace = dict()
 
 
 def dispatch(*types, **kwargs):
-    """ Dispatch function on the types of the inputs
+    """Dispatch function on the types of the inputs
 
     Supports dispatch on all non-keyword arguments.
 
     Collects implementations based on the function name.  Ignores namespaces.
 
     If ambiguous type signatures occur a warning is raised when the function is
     defined suggesting the additional method to break the ambiguity.
@@ -44,41 +45,45 @@
     ...     @dispatch(list)
     ...     def __init__(self, data):
     ...         self.data = data
     ...     @dispatch(int)
     ...     def __init__(self, datum):
     ...         self.data = [datum]
     """
-    namespace = kwargs.get('namespace', global_namespace)
+    namespace = kwargs.get("namespace", global_namespace)
 
     types = tuple(types)
 
-    def _(func):
+    def _df(func):
         name = func.__name__
 
         if ismethod(func):
             dispatcher = inspect.currentframe().f_back.f_locals.get(
                 name,
                 MethodDispatcher(name),
             )
         else:
             if name not in namespace:
                 namespace[name] = Dispatcher(name)
             dispatcher = namespace[name]
 
         dispatcher.add(types, func)
         return dispatcher
-    return _
+
+    return _df
 
 
 def ismethod(func):
-    """ Is func a method?
+    """Is func a method?
 
     Note that this has to work as the method is defined but before the class is
     defined.  At this stage methods look like functions.
     """
     if hasattr(inspect, "signature"):
         signature = inspect.signature(func)
-        return signature.parameters.get('self', None) is not None
+        return signature.parameters.get("self", None) is not None
     else:
-        spec = inspect.getargspec(func)
-        return spec and spec.args and spec.args[0] == 'self'
+        if sys.version_info.major < 3:
+            spec = inspect.getargspec(func)
+        else:
+            spec = inspect.getfullargspec(func)
+        return spec and spec.args and spec.args[0] == "self"
```

### Comparing `multipledispatch-0.6.0/multipledispatch/dispatcher.py` & `multipledispatch-1.0.0/multipledispatch/dispatcher.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,19 +3,19 @@
 from .conflict import ordering, ambiguities, super_signature, AmbiguityWarning
 from .utils import expand_tuples
 from .variadic import Variadic, isvariadic
 import itertools as itl
 
 
 class MDNotImplementedError(NotImplementedError):
-    """ A NotImplementedError for multiple dispatch """
+    """A NotImplementedError for multiple dispatch"""
 
 
 def ambiguity_warn(dispatcher, ambiguities):
-    """ Raise warning when ambiguity is detected
+    """Raise warning when ambiguity is detected
 
     Parameters
     ----------
     dispatcher : Dispatcher
         The dispatcher on which the ambiguity was detected
     ambiguities : set
         Set of type signature pairs that are ambiguous within this dispatcher
@@ -24,29 +24,27 @@
         Dispatcher.add
         warning_text
     """
     warn(warning_text(dispatcher.name, ambiguities), AmbiguityWarning)
 
 
 def halt_ordering():
-    """Deprecated interface to temporarily disable ordering.
-    """
+    """Deprecated interface to temporarily disable ordering."""
     warn(
-        'halt_ordering is deprecated, you can safely remove this call.',
+        "halt_ordering is deprecated, you can safely remove this call.",
         DeprecationWarning,
     )
 
 
 def restart_ordering(on_ambiguity=ambiguity_warn):
-    """Deprecated interface to temporarily resume ordering.
-    """
+    """Deprecated interface to temporarily resume ordering."""
     warn(
-        'restart_ordering is deprecated, if you would like to eagerly order'
-        'the dispatchers, you should call the ``reorder()`` method on each'
-        ' dispatcher.',
+        "restart_ordering is deprecated, if you would like to eagerly order"
+        "the dispatchers, you should call the ``reorder()`` method on each"
+        " dispatcher.",
         DeprecationWarning,
     )
 
 
 def variadic_signature_matches_iter(types, full_signature):
     """Check if a set of input types matches a variadic signature.
 
@@ -92,15 +90,15 @@
 def variadic_signature_matches(types, full_signature):
     # No arguments always matches a variadic signature
     assert full_signature
     return all(variadic_signature_matches_iter(types, full_signature))
 
 
 class Dispatcher(object):
-    """ Dispatch methods based on type signature
+    """Dispatch methods based on type signature
 
     Use ``dispatch`` to add implementations
 
     Examples
     --------
 
     >>> from multipledispatch import dispatch
@@ -113,25 +111,26 @@
     ...     return x - 1
 
     >>> f(3)
     4
     >>> f(3.0)
     2.0
     """
-    __slots__ = '__name__', 'name', 'funcs', '_ordering', '_cache', 'doc'
+
+    __slots__ = "__name__", "name", "funcs", "_ordering", "_cache", "doc"
 
     def __init__(self, name, doc=None):
         self.name = self.__name__ = name
         self.funcs = {}
         self.doc = doc
 
         self._cache = {}
 
     def register(self, *types, **kwargs):
-        """ register dispatcher with new implementation
+        """register dispatcher with new implementation
 
         >>> f = Dispatcher('f')
         >>> @f.register(int)
         ... def inc(x):
         ...     return x + 1
 
         >>> @f.register(float)
@@ -148,47 +147,48 @@
 
         >>> f(1.0)
         0.0
 
         >>> f([1, 2, 3])
         [3, 2, 1]
         """
-        def _(func):
+
+        def _df(func):
             self.add(types, func, **kwargs)
             return func
-        return _
+
+        return _df
 
     @classmethod
     def get_func_params(cls, func):
         if hasattr(inspect, "signature"):
             sig = inspect.signature(func)
             return sig.parameters.values()
 
     @classmethod
     def get_func_annotations(cls, func):
-        """ get annotations of function positional parameters
-        """
+        """get annotations of function positional parameters"""
         params = cls.get_func_params(func)
         if params:
             Parameter = inspect.Parameter
 
-            params = (param for param in params
-                      if param.kind in
-                      (Parameter.POSITIONAL_ONLY,
-                       Parameter.POSITIONAL_OR_KEYWORD))
-
-            annotations = tuple(
-                param.annotation
-                for param in params)
+            params = (
+                param
+                for param in params
+                if param.kind
+                in (Parameter.POSITIONAL_ONLY, Parameter.POSITIONAL_OR_KEYWORD)
+            )
+
+            annotations = tuple(param.annotation for param in params)
 
             if all(ann is not Parameter.empty for ann in annotations):
                 return annotations
 
     def add(self, signature, func):
-        """ Add new types/method pair to dispatcher
+        """Add new types/method pair to dispatcher
 
         >>> D = Dispatcher('add')
         >>> D.add((int, int), lambda x, y: x + y)
         >>> D.add((float, float), lambda x, y: x + y)
 
         >>> D(1, 2)
         3
@@ -213,33 +213,33 @@
                 self.add(typs, func)
             return
 
         new_signature = []
 
         for index, typ in enumerate(signature, start=1):
             if not isinstance(typ, (type, list)):
-                str_sig = ', '.join(c.__name__ if isinstance(c, type)
-                                    else str(c) for c in signature)
-                raise TypeError("Tried to dispatch on non-type: %s\n"
-                                "In signature: <%s>\n"
-                                "In function: %s" %
-                                (typ, str_sig, self.name))
+                str_sig = ", ".join(
+                    c.__name__ if isinstance(c, type) else str(c) for c in signature
+                )
+                raise TypeError(
+                    "Tried to dispatch on non-type: %s\n"
+                    "In signature: <%s>\n"
+                    "In function: %s" % (typ, str_sig, self.name)
+                )
 
             # handle variadic signatures
             if isinstance(typ, list):
                 if index != len(signature):
-                    raise TypeError(
-                        'Variadic signature must be the last element'
-                    )
+                    raise TypeError("Variadic signature must be the last element")
 
                 if len(typ) != 1:
                     raise TypeError(
-                        'Variadic signature must contain exactly one element. '
-                        'To use a variadic union type place the desired types '
-                        'inside of a tuple, e.g., [(int, str)]'
+                        "Variadic signature must contain exactly one element. "
+                        "To use a variadic union type place the desired types "
+                        "inside of a tuple, e.g., [(int, str)]"
                     )
                 new_signature.append(Variadic[typ[0]])
             else:
                 new_signature.append(typ)
 
         self.funcs[tuple(new_signature)] = func
         self._cache.clear()
@@ -267,16 +267,17 @@
         types = tuple([type(arg) for arg in args])
         try:
             func = self._cache[types]
         except KeyError:
             func = self.dispatch(*types)
             if not func:
                 raise NotImplementedError(
-                    'Could not find signature for %s: <%s>' %
-                    (self.name, str_signature(types)))
+                    "Could not find signature for %s: <%s>"
+                    % (self.name, str_signature(types))
+                )
             self._cache[types] = func
         try:
             return func(*args, **kwargs)
 
         except MDNotImplementedError:
             funcs = self.dispatch_iter(*types)
             next(funcs)  # burn first
@@ -284,21 +285,24 @@
                 try:
                     return func(*args, **kwargs)
                 except MDNotImplementedError:
                     pass
 
             raise NotImplementedError(
                 "Matching functions for "
-                "%s: <%s> found, but none completed successfully" % (
-                    self.name, str_signature(types),
+                "%s: <%s> found, but none completed successfully"
+                % (
+                    self.name,
+                    str_signature(types),
                 ),
             )
 
     def __str__(self):
         return "<dispatched %s>" % self.name
+
     __repr__ = __str__
 
     def dispatch(self, *types):
         """Deterimine appropriate implementation for this type signature
 
         This method is internal.  Users should call this object as a function.
         Implementation resolution occurs within the ``__call__`` method.
@@ -324,100 +328,98 @@
 
         try:
             return next(self.dispatch_iter(*types))
         except StopIteration:
             return None
 
     def dispatch_iter(self, *types):
-
         n = len(types)
         for signature in self.ordering:
             if len(signature) == n and all(map(issubclass, types, signature)):
                 result = self.funcs[signature]
                 yield result
             elif len(signature) and isvariadic(signature[-1]):
                 if variadic_signature_matches(types, signature):
                     result = self.funcs[signature]
                     yield result
 
     def resolve(self, types):
-        """ Deterimine appropriate implementation for this type signature
+        """Deterimine appropriate implementation for this type signature
 
         .. deprecated:: 0.4.4
             Use ``dispatch(*types)`` instead
         """
-        warn("resolve() is deprecated, use dispatch(*types)",
-             DeprecationWarning)
+        warn("resolve() is deprecated, use dispatch(*types)", DeprecationWarning)
 
         return self.dispatch(*types)
 
     def __getstate__(self):
-        return {'name': self.name,
-                'funcs': self.funcs}
+        return {"name": self.name, "funcs": self.funcs}
 
     def __setstate__(self, d):
-        self.name = d['name']
-        self.funcs = d['funcs']
+        self.name = d["name"]
+        self.funcs = d["funcs"]
         self._ordering = ordering(self.funcs)
         self._cache = dict()
 
     @property
     def __doc__(self):
         docs = ["Multiply dispatched method: %s" % self.name]
 
         if self.doc:
             docs.append(self.doc)
 
         other = []
         for sig in self.ordering[::-1]:
             func = self.funcs[sig]
             if func.__doc__:
-                s = 'Inputs: <%s>\n' % str_signature(sig)
-                s += '-' * len(s) + '\n'
+                s = "Inputs: <%s>\n" % str_signature(sig)
+                s += "-" * len(s) + "\n"
                 s += func.__doc__.strip()
                 docs.append(s)
             else:
                 other.append(str_signature(sig))
 
         if other:
-            docs.append('Other signatures:\n    ' + '\n    '.join(other))
+            docs.append("Other signatures:\n    " + "\n    ".join(other))
 
-        return '\n\n'.join(docs)
+        return "\n\n".join(docs)
 
     def _help(self, *args):
         return self.dispatch(*map(type, args)).__doc__
 
     def help(self, *args, **kwargs):
-        """ Print docstring for the function corresponding to inputs """
+        """Print docstring for the function corresponding to inputs"""
         print(self._help(*args))
 
     def _source(self, *args):
         func = self.dispatch(*map(type, args))
         if not func:
             raise TypeError("No function found")
         return source(func)
 
     def source(self, *args, **kwargs):
-        """ Print source code for the function corresponding to inputs """
+        """Print source code for the function corresponding to inputs"""
         print(self._source(*args))
 
 
 def source(func):
-    s = 'File: %s\n\n' % inspect.getsourcefile(func)
+    s = "File: %s\n\n" % inspect.getsourcefile(func)
     s = s + inspect.getsource(func)
     return s
 
 
 class MethodDispatcher(Dispatcher):
-    """ Dispatch methods based on type signature
+    """Dispatch methods based on type signature
 
     See Also:
         Dispatcher
     """
-    __slots__ = ('obj', 'cls')
+
+    __slots__ = ("obj", "cls")
 
     @classmethod
     def get_func_params(cls, func):
         if hasattr(inspect, "signature"):
             sig = inspect.signature(func)
             return itl.islice(sig.parameters.values(), 1, None)
 
@@ -426,32 +428,37 @@
         self.cls = owner
         return self
 
     def __call__(self, *args, **kwargs):
         types = tuple([type(arg) for arg in args])
         func = self.dispatch(*types)
         if not func:
-            raise NotImplementedError('Could not find signature for %s: <%s>' %
-                                      (self.name, str_signature(types)))
+            raise NotImplementedError(
+                "Could not find signature for %s: <%s>"
+                % (self.name, str_signature(types))
+            )
         return func(self.obj, *args, **kwargs)
 
 
 def str_signature(sig):
-    """ String representation of type signature
+    """String representation of type signature
 
     >>> str_signature((int, float))
     'int, float'
     """
-    return ', '.join(cls.__name__ for cls in sig)
+    return ", ".join(cls.__name__ for cls in sig)
 
 
 def warning_text(name, amb):
-    """ The text for ambiguity warnings """
+    """The text for ambiguity warnings"""
     text = "\nAmbiguities exist in dispatched function %s\n\n" % (name)
     text += "The following signatures may result in ambiguous behavior:\n"
     for pair in amb:
-        text += "\t" + \
-            ', '.join('[' + str_signature(s) + ']' for s in pair) + "\n"
+        text += "\t" + ", ".join("[" + str_signature(s) + "]" for s in pair) + "\n"
     text += "\n\nConsider making the following additions:\n\n"
-    text += '\n\n'.join(['@dispatch(' + str_signature(super_signature(s))
-                         + ')\ndef %s(...)' % name for s in amb])
+    text += "\n\n".join(
+        [
+            "@dispatch(" + str_signature(super_signature(s)) + ")\ndef %s(...)" % name
+            for s in amb
+        ]
+    )
     return text
```

### Comparing `multipledispatch-0.6.0/README.rst` & `multipledispatch-1.0.0/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -78,26 +78,16 @@
 
 ``multipledispatch`` is on the Python Package Index (PyPI):
 
 ::
 
     pip install multipledispatch
 
-or
-
-::
-
-    easy_install multipledispatch
-
-
-``multipledispatch`` supports Python 2.6+ and Python 3.2+ with a common
-codebase.  It is pure Python and requires only the small `six
-<https://pypi.org/project/six/>`_ library as a dependency.
-
-It is, in short, a light weight dependency.
+It is Pure-Python and depends only on the standard library.
+It is a light weight dependency.
 
 
 License
 -------
 
 New BSD. See `License file`_.
 
@@ -120,22 +110,22 @@
 .. _`multimethods package on PyPI`:
   https://pypi.python.org/pypi/multimethods
 .. _`singledispatch in Python 3.4's functools`:
   http://docs.python.org/3.4/library/functools.html#functools.singledispatch
 .. _`Clojure Protocols`:
   http://clojure.org/protocols
 .. _`Julia methods docs`:
-  https://julia.readthedocs.io/en/latest/manual/methods/
+  https://docs.julialang.org/en/v1/manual/methods/
 .. _`Karpinksi notebook: *The Design Impact of Multiple Dispatch*`:
   http://nbviewer.ipython.org/gist/StefanKarpinski/b8fe9dbb36c1427b9f22
 .. _`Wikipedia article`:
   http://en.wikipedia.org/wiki/Multiple_dispatch
 .. _`PEP 3124 - *Overloading, Generic Functions, Interfaces, and Adaptation*`:
   http://legacy.python.org/dev/peps/pep-3124/
 
-.. |Build Status| image:: https://travis-ci.org/mrocklin/multipledispatch.png
+.. |Build Status| image:: https://travis-ci.org/mrocklin/multipledispatch.svg
    :target: https://travis-ci.org/mrocklin/multipledispatch
-.. |Version Status| image:: https://pypip.in/v/multipledispatch/badge.png
+.. |Version Status| image:: https://pypip.in/v/multipledispatch/badge.svg
    :target: https://img.shields.io/pypi/v/multipledispatch.svg
-.. |Coverage Status| image:: https://coveralls.io/repos/mrocklin/multipledispatch/badge.png
+.. |Coverage Status| image:: https://coveralls.io/repos/mrocklin/multipledispatch/badge.svg
    :target: https://coveralls.io/r/mrocklin/multipledispatch
 .. _License file: https://github.com/mrocklin/multipledispatch/blob/master/LICENSE.txt
```

