# Comparing `tmp/rvtools-0.1.0.tar.gz` & `tmp/rvtools-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rvtools-0.1.0.tar", max compression
+gzip compressed data, was "rvtools-0.1.1.tar", max compression
```

## Comparing `rvtools-0.1.0.tar` & `rvtools-0.1.1.tar`

### file list

```diff
@@ -1,24 +1,31 @@
--rw-r--r--   0        0        0     1696 2023-06-25 23:16:15.989291 rvtools-0.1.0/README.md
--rw-r--r--   0        0        0      852 2023-06-25 23:16:15.989431 rvtools-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      299 2023-06-25 22:44:46.565852 rvtools-0.1.0/rvtools/__init__.py
--rw-r--r--   0        0        0      188 2023-06-25 21:11:58.261298 rvtools-0.1.0/rvtools/_constructors/__init__.py
--rw-r--r--   0        0        0      459 2023-06-25 21:11:59.187336 rvtools-0.1.0/rvtools/_constructors/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     2573 2023-06-25 22:21:36.090266 rvtools-0.1.0/rvtools/_constructors/__pycache__/_helpers.cpython-311.pyc
--rw-r--r--   0        0        0     2776 2023-06-25 22:16:58.773929 rvtools-0.1.0/rvtools/_constructors/__pycache__/beta.cpython-311.pyc
--rw-r--r--   0        0        0     3810 2023-06-25 22:44:47.103090 rvtools-0.1.0/rvtools/_constructors/__pycache__/lognorm.cpython-311.pyc
--rw-r--r--   0        0        0     2772 2023-06-25 22:44:47.103766 rvtools-0.1.0/rvtools/_constructors/__pycache__/norm.cpython-311.pyc
--rw-r--r--   0        0        0     2649 2023-06-25 22:44:47.104215 rvtools-0.1.0/rvtools/_constructors/__pycache__/uniform.cpython-311.pyc
--rw-r--r--   0        0        0     1535 2023-06-25 22:20:41.612198 rvtools-0.1.0/rvtools/_constructors/_helpers.py
--rw-r--r--   0        0        0     1481 2023-06-25 22:16:58.269024 rvtools-0.1.0/rvtools/_constructors/beta.py
--rw-r--r--   0        0        0     2135 2023-06-25 22:32:32.135227 rvtools-0.1.0/rvtools/_constructors/lognorm.py
--rw-r--r--   0        0        0     1262 2023-06-25 22:32:32.143293 rvtools-0.1.0/rvtools/_constructors/norm.py
--rw-r--r--   0        0        0     1441 2023-06-25 22:32:32.138670 rvtools-0.1.0/rvtools/_constructors/uniform.py
--rw-r--r--   0        0        0      613 2023-06-25 21:11:58.260296 rvtools-0.1.0/rvtools/distributions.py
--rw-r--r--   0        0        0      560 2023-06-25 21:13:58.682207 rvtools-0.1.0/rvtools/types.py
--rw-r--r--   0        0        0        0 2023-06-25 18:12:13.995575 rvtools-0.1.0/tests/__init__.py
--rw-r--r--   0        0        0      339 2023-06-25 21:11:58.259220 rvtools-0.1.0/tests/test_certainty.py
--rw-r--r--   0        0        0     5379 2023-06-25 22:21:35.569427 rvtools-0.1.0/tests/test_constructors.py
--rw-r--r--   0        0        0      274 2023-06-25 23:03:01.270501 rvtools-0.1.0/tests/test_docs_do_not_raise.py
--rw-r--r--   0        0        0     2163 2023-06-25 22:20:41.629042 rvtools-0.1.0/tests/test_parse_spec.py
--rw-r--r--   0        0        0      521 2023-06-25 20:54:28.571779 rvtools-0.1.0/tests/test_types.py
--rw-r--r--   0        0        0     2345 1970-01-01 00:00:00.000000 rvtools-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     4152 2023-06-26 22:59:09.399091 rvtools-0.1.1/README.md
+-rw-r--r--   0        0        0      852 2023-06-26 23:19:50.728717 rvtools-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      264 2023-06-26 22:42:35.971751 rvtools-0.1.1/rvtools/__init__.py
+-rw-r--r--   0        0        0      172 2023-06-26 22:48:01.905065 rvtools-0.1.1/rvtools/construct/__init__.py
+-rw-r--r--   0        0        0      439 2023-06-26 22:48:02.435189 rvtools-0.1.1/rvtools/construct/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     2573 2023-06-25 22:21:36.090266 rvtools-0.1.1/rvtools/construct/__pycache__/_helpers.cpython-311.pyc
+-rw-r--r--   0        0        0     2768 2023-06-26 22:48:02.435671 rvtools-0.1.1/rvtools/construct/__pycache__/beta.cpython-311.pyc
+-rw-r--r--   0        0        0     3798 2023-06-26 22:48:02.436259 rvtools-0.1.1/rvtools/construct/__pycache__/lognorm.cpython-311.pyc
+-rw-r--r--   0        0        0     2764 2023-06-26 22:48:02.436685 rvtools-0.1.1/rvtools/construct/__pycache__/norm.cpython-311.pyc
+-rw-r--r--   0        0        0     2641 2023-06-26 22:48:02.437087 rvtools-0.1.1/rvtools/construct/__pycache__/uniform.cpython-311.pyc
+-rw-r--r--   0        0        0     1535 2023-06-25 22:20:41.612198 rvtools-0.1.1/rvtools/construct/_helpers.py
+-rw-r--r--   0        0        0     1477 2023-06-26 22:48:01.909872 rvtools-0.1.1/rvtools/construct/beta.py
+-rw-r--r--   0        0        0     2127 2023-06-26 22:48:01.906834 rvtools-0.1.1/rvtools/construct/lognorm.py
+-rw-r--r--   0        0        0     1258 2023-06-26 22:48:01.911084 rvtools-0.1.1/rvtools/construct/norm.py
+-rw-r--r--   0        0        0     1437 2023-06-26 22:48:01.914585 rvtools-0.1.1/rvtools/construct/uniform.py
+-rw-r--r--   0        0        0      126 2023-06-26 20:21:17.331337 rvtools-0.1.1/rvtools/distributions/__init__.py
+-rw-r--r--   0        0        0      358 2023-06-26 20:21:36.589514 rvtools-0.1.1/rvtools/distributions/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     1726 2023-06-26 18:36:15.269055 rvtools-0.1.1/rvtools/distributions/__pycache__/certainty.cpython-311.pyc
+-rw-r--r--   0        0        0     8408 2023-06-26 20:16:33.256135 rvtools-0.1.1/rvtools/distributions/__pycache__/tp_uniform.cpython-311.pyc
+-rw-r--r--   0        0        0      854 2023-06-26 18:23:58.213480 rvtools-0.1.1/rvtools/distributions/certainty.py
+-rw-r--r--   0        0        0     5151 2023-06-26 20:16:32.712477 rvtools-0.1.1/rvtools/distributions/tp_uniform.py
+-rw-r--r--   0        0        0      556 2023-06-26 21:58:51.980313 rvtools-0.1.1/rvtools/types.py
+-rw-r--r--   0        0        0        0 2023-06-25 18:12:13.995575 rvtools-0.1.1/tests/__init__.py
+-rw-r--r--   0        0        0      507 2023-06-26 20:21:17.339335 rvtools-0.1.1/tests/conftest.py
+-rw-r--r--   0        0        0      339 2023-06-25 21:11:58.259220 rvtools-0.1.1/tests/test_certainty.py
+-rw-r--r--   0        0        0     5084 2023-06-26 22:48:01.916512 rvtools-0.1.1/tests/test_constructors.py
+-rw-r--r--   0        0        0      274 2023-06-25 23:03:01.270501 rvtools-0.1.1/tests/test_docs_do_not_raise.py
+-rw-r--r--   0        0        0     2159 2023-06-26 22:48:01.912458 rvtools-0.1.1/tests/test_parse_spec.py
+-rw-r--r--   0        0        0     4264 2023-06-26 22:48:01.908527 rvtools-0.1.1/tests/test_tp_uniform.py
+-rw-r--r--   0        0        0      513 2023-06-26 21:58:51.980481 rvtools-0.1.1/tests/test_types.py
+-rw-r--r--   0        0        0     4801 1970-01-01 00:00:00.000000 rvtools-0.1.1/PKG-INFO
```

### Comparing `rvtools-0.1.0/pyproject.toml` & `rvtools-0.1.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool]
 [tool.poetry]
 name = "rvtools"
-version = "0.1.0"
+version = "0.1.1"
 homepage = "https://github.com/tadamcz/rvtools"
 description = "Top-level package for Probability distribution and random variable tools."
 authors = ["Tom Adamczewski <tadamczewskipublic@gmail.com>"]
 readme = "README.md"
 classifiers=[
     'Natural Language :: English',
     'Programming Language :: Python :: 3',
```

### Comparing `rvtools-0.1.0/rvtools/_constructors/__pycache__/_helpers.cpython-311.pyc` & `rvtools-0.1.1/rvtools/construct/__pycache__/_helpers.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `rvtools-0.1.0/rvtools/_constructors/__pycache__/beta.cpython-311.pyc` & `rvtools-0.1.1/rvtools/construct/__pycache__/beta.cpython-311.pyc`

 * *Files 7% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0xdabc9864 (Sun Jun 25 22:16:58 2023 UTC)
-files sz: 1481
+moddate:  0xa1159a64 (Mon Jun 26 22:48:01 2023 UTC)
+files sz: 1477
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 10
    flags     : 0
    code
       0x9700640064016c006d015a010100640064026c025a03640064026c045a
@@ -28,15 +28,15 @@
      4          22 LOAD_CONST               0 (0)
                 24 LOAD_CONST               2 (None)
                 26 IMPORT_NAME              4 (scipy)
                 28 STORE_NAME               4 (scipy)
    
      6          30 LOAD_CONST               0 (0)
                 32 LOAD_CONST               3 (('parse_spec',))
-                34 IMPORT_NAME              5 (rvtools._constructors._helpers)
+                34 IMPORT_NAME              5 (rvtools.construct._helpers)
                 36 IMPORT_FROM              6 (parse_spec)
                 38 STORE_NAME               6 (parse_spec)
                 40 POP_TOP
    
      9          42 LOAD_CONST              10 ((None, None))
                 44 LOAD_CONST               2 (None)
                 46 LOAD_CONST               4 (('quantiles',))
@@ -48,26 +48,26 @@
                 58 LOAD_CONST               7 ('quantiles')
                 60 LOAD_NAME                7 (dict)
                 62 LOAD_NAME                1 (Real)
                 64 LOAD_NAME                1 (Real)
                 66 BUILD_TUPLE              2
                 68 BINARY_SUBSCR
                 78 BUILD_TUPLE              6
-                80 LOAD_CONST               8 (<code object beta, file "/Users/t/repos/rvtools/rvtools/_constructors/beta.py", line 9>)
+                80 LOAD_CONST               8 (<code object beta, file "/Users/t/repos/rvtools/rvtools/construct/beta.py", line 9>)
                 82 MAKE_FUNCTION            7 (defaults, kwdefaults, annotations)
                 84 STORE_NAME               8 (beta)
    
     19          86 LOAD_CONST               7 ('quantiles')
                 88 LOAD_NAME                7 (dict)
                 90 LOAD_NAME                1 (Real)
                 92 LOAD_NAME                1 (Real)
                 94 BUILD_TUPLE              2
                 96 BINARY_SUBSCR
                106 BUILD_TUPLE              2
-               108 LOAD_CONST               9 (<code object from_quantiles, file "/Users/t/repos/rvtools/rvtools/_constructors/beta.py", line 19>)
+               108 LOAD_CONST               9 (<code object from_quantiles, file "/Users/t/repos/rvtools/rvtools/construct/beta.py", line 19>)
                110 MAKE_FUNCTION            4 (annotations)
                112 STORE_NAME               9 (from_quantiles)
                114 LOAD_CONST               2 (None)
                116 RETURN_VALUE
    consts
       0
       ('Real',)
@@ -156,15 +156,15 @@
             'quantiles'
             "You must specify either 'alpha' and 'beta', or 'quantiles'."
             ()
          names      ('parse_spec', 'keys', 'scipy', 'stats', 'beta', 'from_quantiles', 'ValueError')
          varnames   ('alpha', 'beta', 'quantiles', 'kwargs', 'spec')
          freevars   ()
          cellvars   ()
-         filename   '/Users/t/repos/rvtools/rvtools/_constructors/beta.py'
+         filename   '/Users/t/repos/rvtools/rvtools/construct/beta.py'
          name       'beta'
          firstlineno 9
          lnotab 0x020120013401400132012a02
       code
          argcount  : 1
          nlocals   : 9
          stacksize : 7
@@ -236,15 +236,15 @@
                      242 STORE_FAST               3 (alpha_init)
                      244 STORE_FAST               4 (beta_init)
          
           27         246 LOAD_GLOBAL             10 (scipy)
                      258 LOAD_ATTR                6 (optimize)
                      268 LOAD_METHOD              7 (curve_fit)
          
-          28         290 LOAD_CONST               5 (<code object <lambda>, file "/Users/t/repos/rvtools/rvtools/_constructors/beta.py", line 28>)
+          28         290 LOAD_CONST               5 (<code object <lambda>, file "/Users/t/repos/rvtools/rvtools/construct/beta.py", line 28>)
                      292 MAKE_FUNCTION            0
          
           29         294 LOAD_FAST                2 (qs)
          
           30         296 LOAD_FAST                1 (ps)
          
           31         298 LOAD_FAST                3 (alpha_init)
@@ -337,34 +337,34 @@
                             76 RETURN_VALUE
                consts
                   None
                names      ('scipy', 'stats', 'beta', 'cdf')
                varnames   ('x', 'alpha', 'beta')
                freevars   ()
                cellvars   ()
-               filename   '/Users/t/repos/rvtools/rvtools/_constructors/beta.py'
+               filename   '/Users/t/repos/rvtools/rvtools/construct/beta.py'
                name       '<lambda>'
                firstlineno 28
                lnotab 0x
             ('xdata', 'ydata', 'p0')
             0
             'Could not fit beta distribution to quantiles. Expected probabilities '
             ', got fitted values '
          names      ('len', 'ValueError', 'list', 'keys', 'values', 'scipy', 'optimize', 'curve_fit', 'stats', 'beta', 'cdf', 'np', 'allclose')
          varnames   ('quantiles', 'ps', 'qs', 'alpha_init', 'beta_init', 'fit', 'alpha', 'beta', 'fitted_ps')
          freevars   ()
          cellvars   ()
-         filename   '/Users/t/repos/rvtools/rvtools/_constructors/beta.py'
+         filename   '/Users/t/repos/rvtools/rvtools/construct/beta.py'
          name       'from_quantiles'
          firstlineno 19
          lnotab
             0x020126014002420142020a012c0104010201020106fc120816014c012a
             010c01020102ff040102ff06ff1005
       (None, None)
-   names      ('numbers', 'Real', 'numpy', 'np', 'scipy', 'rvtools._constructors._helpers', 'parse_spec', 'dict', 'beta', 'from_quantiles')
+   names      ('numbers', 'Real', 'numpy', 'np', 'scipy', 'rvtools.construct._helpers', 'parse_spec', 'dict', 'beta', 'from_quantiles')
    varnames   ()
    freevars   ()
    cellvars   ()
-   filename   '/Users/t/repos/rvtools/rvtools/_constructors/beta.py'
+   filename   '/Users/t/repos/rvtools/rvtools/construct/beta.py'
    name       '<module>'
    firstlineno 1
    lnotab 0x00ff02010c02080108020c032c0a
```

### Comparing `rvtools-0.1.0/rvtools/_constructors/__pycache__/lognorm.cpython-311.pyc` & `rvtools-0.1.1/rvtools/construct/__pycache__/lognorm.cpython-311.pyc`

 * *Files 4% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0x80c09864 (Sun Jun 25 22:32:32 2023 UTC)
-files sz: 2135
+moddate:  0xa1159a64 (Mon Jun 26 22:48:01 2023 UTC)
+files sz: 2127
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 14
    flags     : 0
    code
       0x9700640064016c006d015a010100640064026c025a03640064026c045a
@@ -30,22 +30,22 @@
      4          22 LOAD_CONST               0 (0)
                 24 LOAD_CONST               2 (None)
                 26 IMPORT_NAME              4 (scipy)
                 28 STORE_NAME               4 (scipy)
    
      6          30 LOAD_CONST               0 (0)
                 32 LOAD_CONST               3 (('parse_spec',))
-                34 IMPORT_NAME              5 (rvtools._constructors._helpers)
+                34 IMPORT_NAME              5 (rvtools.construct._helpers)
                 36 IMPORT_FROM              6 (parse_spec)
                 38 STORE_NAME               6 (parse_spec)
                 40 POP_TOP
    
      7          42 LOAD_CONST               0 (0)
                 44 LOAD_CONST               4 (('params_from_quantiles',))
-                46 IMPORT_NAME              7 (rvtools._constructors.norm)
+                46 IMPORT_NAME              7 (rvtools.construct.norm)
                 48 IMPORT_FROM              8 (params_from_quantiles)
                 50 STORE_NAME               9 (norm_params_from_quantiles)
                 52 POP_TOP
    
     11          54 NOP
    
     12          56 NOP
@@ -81,43 +81,43 @@
     16          88 LOAD_NAME               10 (dict)
                 90 LOAD_NAME                1 (Real)
                 92 LOAD_NAME                1 (Real)
                 94 BUILD_TUPLE              2
                 96 BINARY_SUBSCR
    
     10         106 BUILD_TUPLE             10
-               108 LOAD_CONST              11 (<code object lognorm, file "/Users/t/repos/rvtools/rvtools/_constructors/lognorm.py", line 10>)
+               108 LOAD_CONST              11 (<code object lognorm, file "/Users/t/repos/rvtools/rvtools/construct/lognorm.py", line 10>)
                110 MAKE_FUNCTION            7 (defaults, kwdefaults, annotations)
                112 STORE_NAME              11 (lognorm)
    
     32         114 LOAD_CONST              10 ('quantiles')
                116 LOAD_NAME               10 (dict)
                118 LOAD_NAME                1 (Real)
                120 LOAD_NAME                1 (Real)
                122 BUILD_TUPLE              2
                124 BINARY_SUBSCR
                134 BUILD_TUPLE              2
-               136 LOAD_CONST              12 (<code object from_quantiles, file "/Users/t/repos/rvtools/rvtools/_constructors/lognorm.py", line 32>)
+               136 LOAD_CONST              12 (<code object from_quantiles, file "/Users/t/repos/rvtools/rvtools/construct/lognorm.py", line 32>)
                138 MAKE_FUNCTION            4 (annotations)
                140 STORE_NAME              12 (from_quantiles)
    
     46         142 LOAD_CONST               6 ('mu')
                144 LOAD_NAME                1 (Real)
                146 LOAD_CONST               7 ('sigma')
                148 LOAD_NAME                1 (Real)
                150 BUILD_TUPLE              4
-               152 LOAD_CONST              13 (<code object from_params, file "/Users/t/repos/rvtools/rvtools/_constructors/lognorm.py", line 46>)
+               152 LOAD_CONST              13 (<code object from_params, file "/Users/t/repos/rvtools/rvtools/construct/lognorm.py", line 46>)
                154 MAKE_FUNCTION            4 (annotations)
                156 STORE_NAME              13 (from_params)
    
-    57         158 LOAD_CONST              14 (<code object from_mean_sd, file "/Users/t/repos/rvtools/rvtools/_constructors/lognorm.py", line 57>)
+    57         158 LOAD_CONST              14 (<code object from_mean_sd, file "/Users/t/repos/rvtools/rvtools/construct/lognorm.py", line 57>)
                160 MAKE_FUNCTION            0
                162 STORE_NAME              14 (from_mean_sd)
    
-    62         164 LOAD_CONST              15 (<code object to_mu_sigma, file "/Users/t/repos/rvtools/rvtools/_constructors/lognorm.py", line 62>)
+    62         164 LOAD_CONST              15 (<code object to_mu_sigma, file "/Users/t/repos/rvtools/rvtools/construct/lognorm.py", line 62>)
                166 MAKE_FUNCTION            0
                168 STORE_NAME              15 (to_mu_sigma)
                170 LOAD_CONST               2 (None)
                172 RETURN_VALUE
    consts
       0
       ('Real',)
@@ -231,15 +231,15 @@
             'quantiles'
             "You must specify either 'mu' and 'sigma', 'mean' and 'sd', or 'quantiles'."
             ()
          names      ('parse_spec', 'keys', 'from_params', 'from_mean_sd', 'from_quantiles', 'ValueError')
          varnames   ('mu', 'sigma', 'mean', 'sd', 'quantiles', 'kwargs', 'spec')
          freevars   ()
          cellvars   ()
-         filename   '/Users/t/repos/rvtools/rvtools/_constructors/lognorm.py'
+         filename   '/Users/t/repos/rvtools/rvtools/construct/lognorm.py'
          name       'lognorm'
          firstlineno 10
          lnotab 0x02092401340120013401200132012a020c0102ff
       code
          argcount  : 1
          nlocals   : 6
          stacksize : 7
@@ -339,15 +339,15 @@
             '.'
             0
             1
          names      ('len', 'ValueError', 'list', 'keys', 'values', 'np', 'log', 'norm_params_from_quantiles', 'from_params')
          varnames   ('quantiles', 'ps', 'qs', 'log_qs', 'mu', 'sigma')
          freevars   ()
          cellvars   ()
-         filename   '/Users/t/repos/rvtools/rvtools/_constructors/lognorm.py'
+         filename   '/Users/t/repos/rvtools/rvtools/construct/lognorm.py'
          name       'from_quantiles'
          firstlineno 32
          lnotab 0x0201260140024201420328015a02
       code
          argcount  : 2
          nlocals   : 2
          stacksize : 5
@@ -375,15 +375,15 @@
          consts
             "\n    SciPy's ``lognorm`` does not take the ``mu`` and ``sigma`` parameters (it takes its own\n    ``scale`` and ``s`` parameters).\n\n    This is a convenience wrapper that allows you to create a (frozen) SciPy log-normal distribution using ``mu`` and\n    ``sigma``.\n    "
             ('scale', 's')
          names      ('scipy', 'stats', 'lognorm', 'np', 'exp')
          varnames   ('mu', 'sigma')
          freevars   ()
          cellvars   ()
-         filename   '/Users/t/repos/rvtools/rvtools/_constructors/lognorm.py'
+         filename   '/Users/t/repos/rvtools/rvtools/construct/lognorm.py'
          name       'from_params'
          firstlineno 46
          lnotab 0x0208
       code
          argcount  : 2
          nlocals   : 4
          stacksize : 4
@@ -411,15 +411,15 @@
                       70 RETURN_VALUE
          consts
             None
          names      ('to_mu_sigma', 'from_params')
          varnames   ('mean', 'sd', 'mu', 'sigma')
          freevars   ()
          cellvars   ()
-         filename   '/Users/t/repos/rvtools/rvtools/_constructors/lognorm.py'
+         filename   '/Users/t/repos/rvtools/rvtools/construct/lognorm.py'
          name       'from_mean_sd'
          firstlineno 57
          lnotab 0x02012601
       code
          argcount  : 2
          nlocals   : 5
          stacksize : 7
@@ -487,22 +487,22 @@
             2
             1
             0.5
          names      ('np', 'sqrt', 'log')
          varnames   ('mean', 'sd', 'var', 'sigma', 'mu')
          freevars   ()
          cellvars   ()
-         filename   '/Users/t/repos/rvtools/rvtools/_constructors/lognorm.py'
+         filename   '/Users/t/repos/rvtools/rvtools/construct/lognorm.py'
          name       'to_mu_sigma'
          firstlineno 62
          lnotab 0x02040a015e026a02
       (None, None)
-   names      ('numbers', 'Real', 'numpy', 'np', 'scipy', 'rvtools._constructors._helpers', 'parse_spec', 'rvtools._constructors.norm', 'params_from_quantiles', 'norm_params_from_quantiles', 'dict', 'lognorm', 'from_quantiles', 'from_params', 'from_mean_sd', 'to_mu_sigma')
+   names      ('numbers', 'Real', 'numpy', 'np', 'scipy', 'rvtools.construct._helpers', 'parse_spec', 'rvtools.construct.norm', 'params_from_quantiles', 'norm_params_from_quantiles', 'dict', 'lognorm', 'from_quantiles', 'from_params', 'from_mean_sd', 'to_mu_sigma')
    varnames   ()
    freevars   ()
    cellvars   ()
-   filename   '/Users/t/repos/rvtools/rvtools/_constructors/lognorm.py'
+   filename   '/Users/t/repos/rvtools/rvtools/construct/lognorm.py'
    name       '<module>'
    firstlineno 1
    lnotab
       0x00ff02010c02080108020c010c04020102fe02040201020102fa060102
       ff020202fe020402fc020502fb020612fa08161c0e100b0605
```

### Comparing `rvtools-0.1.0/rvtools/_constructors/__pycache__/norm.cpython-311.pyc` & `rvtools-0.1.1/rvtools/construct/__pycache__/norm.cpython-311.pyc`

 * *Files 4% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0x80c09864 (Sun Jun 25 22:32:32 2023 UTC)
-files sz: 1262
+moddate:  0xa1159a64 (Mon Jun 26 22:48:01 2023 UTC)
+files sz: 1258
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 10
    flags     : 0
    code
       0x9700640064016c006d015a010100640064026c025a02640064036c036d
@@ -24,15 +24,15 @@
      3          14 LOAD_CONST               0 (0)
                 16 LOAD_CONST               2 (None)
                 18 IMPORT_NAME              2 (scipy)
                 20 STORE_NAME               2 (scipy)
    
      5          22 LOAD_CONST               0 (0)
                 24 LOAD_CONST               3 (('parse_spec',))
-                26 IMPORT_NAME              3 (rvtools._constructors._helpers)
+                26 IMPORT_NAME              3 (rvtools.construct._helpers)
                 28 IMPORT_FROM              4 (parse_spec)
                 30 STORE_NAME               4 (parse_spec)
                 32 POP_TOP
    
      8          34 LOAD_CONST              12 ((None, None))
                 36 LOAD_CONST               2 (None)
                 38 LOAD_CONST               4 (('quantiles',))
@@ -44,37 +44,37 @@
                 50 LOAD_CONST               7 ('quantiles')
                 52 LOAD_NAME                6 (dict)
                 54 LOAD_NAME                1 (Real)
                 56 LOAD_NAME                1 (Real)
                 58 BUILD_TUPLE              2
                 60 BINARY_SUBSCR
                 70 BUILD_TUPLE              6
-                72 LOAD_CONST               8 (<code object norm, file "/Users/t/repos/rvtools/rvtools/_constructors/norm.py", line 8>)
+                72 LOAD_CONST               8 (<code object norm, file "/Users/t/repos/rvtools/rvtools/construct/norm.py", line 8>)
                 74 MAKE_FUNCTION            7 (defaults, kwdefaults, annotations)
                 76 STORE_NAME               7 (norm)
    
     18          78 LOAD_CONST               7 ('quantiles')
                 80 LOAD_NAME                6 (dict)
                 82 LOAD_NAME                1 (Real)
                 84 LOAD_NAME                1 (Real)
                 86 BUILD_TUPLE              2
                 88 BINARY_SUBSCR
                 98 BUILD_TUPLE              2
-               100 LOAD_CONST               9 (<code object from_quantiles, file "/Users/t/repos/rvtools/rvtools/_constructors/norm.py", line 18>)
+               100 LOAD_CONST               9 (<code object from_quantiles, file "/Users/t/repos/rvtools/rvtools/construct/norm.py", line 18>)
                102 MAKE_FUNCTION            4 (annotations)
                104 STORE_NAME               8 (from_quantiles)
    
     30         106 LOAD_CONST              10 ('return')
                108 LOAD_NAME                9 (tuple)
                110 LOAD_NAME                1 (Real)
                112 LOAD_NAME                1 (Real)
                114 BUILD_TUPLE              2
                116 BINARY_SUBSCR
                126 BUILD_TUPLE              2
-               128 LOAD_CONST              11 (<code object params_from_quantiles, file "/Users/t/repos/rvtools/rvtools/_constructors/norm.py", line 30>)
+               128 LOAD_CONST              11 (<code object params_from_quantiles, file "/Users/t/repos/rvtools/rvtools/construct/norm.py", line 30>)
                130 MAKE_FUNCTION            4 (annotations)
                132 STORE_NAME              10 (params_from_quantiles)
                134 LOAD_CONST               2 (None)
                136 RETURN_VALUE
    consts
       0
       ('Real',)
@@ -163,15 +163,15 @@
             'quantiles'
             "You must specify either 'mean' and 'sd', or 'quantiles'."
             ()
          names      ('parse_spec', 'keys', 'scipy', 'stats', 'norm', 'from_quantiles', 'ValueError')
          varnames   ('mean', 'sd', 'quantiles', 'kwargs', 'spec')
          freevars   ()
          cellvars   ()
-         filename   '/Users/t/repos/rvtools/rvtools/_constructors/norm.py'
+         filename   '/Users/t/repos/rvtools/rvtools/construct/norm.py'
          name       'norm'
          firstlineno 8
          lnotab 0x020120013401400132012a02
       code
          argcount  : 1
          nlocals   : 5
          stacksize : 7
@@ -266,15 +266,15 @@
             '.'
             0
             1
          names      ('len', 'ValueError', 'list', 'keys', 'values', 'params_from_quantiles', 'scipy', 'stats', 'norm')
          varnames   ('quantiles', 'ps', 'qs', 'mu', 'sigma')
          freevars   ()
          cellvars   ()
-         filename   '/Users/t/repos/rvtools/rvtools/_constructors/norm.py'
+         filename   '/Users/t/repos/rvtools/rvtools/construct/norm.py'
          name       'from_quantiles'
          firstlineno 18
          lnotab 0x020126014002420142025a02
       'return'
       code
          argcount  : 4
          nlocals   : 7
@@ -348,20 +348,20 @@
                      334 RETURN_VALUE
          consts
             'Find parameters for a normal random variable X so that P(X < x1) = p1 and P(X < x2) = p2.'
          names      ('scipy', 'stats', 'norm', 'ppf')
          varnames   ('p1', 'x1', 'p2', 'x2', 'denom', 'sigma', 'mu')
          freevars   ()
          cellvars   ()
-         filename   '/Users/t/repos/rvtools/rvtools/_constructors/norm.py'
+         filename   '/Users/t/repos/rvtools/rvtools/construct/norm.py'
          name       'params_from_quantiles'
          firstlineno 30
          lnotab 0x020292011001a401
       (None, None)
-   names      ('numbers', 'Real', 'scipy', 'rvtools._constructors._helpers', 'parse_spec', 'float', 'dict', 'norm', 'from_quantiles', 'tuple', 'params_from_quantiles')
+   names      ('numbers', 'Real', 'scipy', 'rvtools.construct._helpers', 'parse_spec', 'float', 'dict', 'norm', 'from_quantiles', 'tuple', 'params_from_quantiles')
    varnames   ()
    freevars   ()
    cellvars   ()
-   filename   '/Users/t/repos/rvtools/rvtools/_constructors/norm.py'
+   filename   '/Users/t/repos/rvtools/rvtools/construct/norm.py'
    name       '<module>'
    firstlineno 1
    lnotab 0x00ff02010c0208020c032c0a1c0c
```

### Comparing `rvtools-0.1.0/rvtools/_constructors/__pycache__/uniform.cpython-311.pyc` & `rvtools-0.1.1/rvtools/construct/__pycache__/uniform.cpython-311.pyc`

 * *Files 12% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0x80c09864 (Sun Jun 25 22:32:32 2023 UTC)
-files sz: 1441
+moddate:  0xa1159a64 (Mon Jun 26 22:48:01 2023 UTC)
+files sz: 1437
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 10
    flags     : 0
    code
       0x9700640064016c006d015a010100640064026c025a02640064036c036d
@@ -31,15 +31,15 @@
                 26 IMPORT_NAME              3 (scipy.interpolate)
                 28 IMPORT_FROM              4 (interp1d)
                 30 STORE_NAME               4 (interp1d)
                 32 POP_TOP
    
      6          34 LOAD_CONST               0 (0)
                 36 LOAD_CONST               4 (('parse_spec',))
-                38 IMPORT_NAME              5 (rvtools._constructors._helpers)
+                38 IMPORT_NAME              5 (rvtools.construct._helpers)
                 40 IMPORT_FROM              6 (parse_spec)
                 42 STORE_NAME               6 (parse_spec)
                 44 POP_TOP
    
      9          46 LOAD_CONST              12 ((None, None))
                 48 LOAD_CONST               2 (None)
                 50 LOAD_CONST               5 (('quantiles',))
@@ -51,30 +51,30 @@
                 62 LOAD_CONST               8 ('quantiles')
                 64 LOAD_NAME                7 (dict)
                 66 LOAD_NAME                1 (Real)
                 68 LOAD_NAME                1 (Real)
                 70 BUILD_TUPLE              2
                 72 BINARY_SUBSCR
                 82 BUILD_TUPLE              6
-                84 LOAD_CONST               9 (<code object uniform, file "/Users/t/repos/rvtools/rvtools/_constructors/uniform.py", line 9>)
+                84 LOAD_CONST               9 (<code object uniform, file "/Users/t/repos/rvtools/rvtools/construct/uniform.py", line 9>)
                 86 MAKE_FUNCTION            7 (defaults, kwdefaults, annotations)
                 88 STORE_NAME               8 (uniform)
    
     19          90 LOAD_CONST               8 ('quantiles')
                 92 LOAD_NAME                7 (dict)
                 94 LOAD_NAME                1 (Real)
                 96 LOAD_NAME                1 (Real)
                 98 BUILD_TUPLE              2
                100 BINARY_SUBSCR
                110 BUILD_TUPLE              2
-               112 LOAD_CONST              10 (<code object from_quantiles, file "/Users/t/repos/rvtools/rvtools/_constructors/uniform.py", line 19>)
+               112 LOAD_CONST              10 (<code object from_quantiles, file "/Users/t/repos/rvtools/rvtools/construct/uniform.py", line 19>)
                114 MAKE_FUNCTION            4 (annotations)
                116 STORE_NAME               9 (from_quantiles)
    
-    34         118 LOAD_CONST              11 (<code object from_extrema, file "/Users/t/repos/rvtools/rvtools/_constructors/uniform.py", line 34>)
+    34         118 LOAD_CONST              11 (<code object from_extrema, file "/Users/t/repos/rvtools/rvtools/construct/uniform.py", line 34>)
                120 MAKE_FUNCTION            0
                122 STORE_NAME              10 (from_extrema)
                124 LOAD_CONST               2 (None)
                126 RETURN_VALUE
    consts
       0
       ('Real',)
@@ -161,15 +161,15 @@
             'quantiles'
             "You must specify either the extrema 'a' and 'b', or 'quantiles'."
             ()
          names      ('parse_spec', 'keys', 'from_extrema', 'from_quantiles', 'ValueError')
          varnames   ('a', 'b', 'quantiles', 'kwargs', 'spec')
          freevars   ()
          cellvars   ()
-         filename   '/Users/t/repos/rvtools/rvtools/_constructors/uniform.py'
+         filename   '/Users/t/repos/rvtools/rvtools/construct/uniform.py'
          name       'uniform'
          firstlineno 9
          lnotab 0x020120013401200132012a02
       code
          argcount  : 1
          nlocals   : 6
          stacksize : 7
@@ -270,15 +270,15 @@
             ('kind', 'fill_value', 'assume_sorted')
             0
             1
          names      ('len', 'ValueError', 'list', 'keys', 'values', 'interp1d', 'uniform')
          varnames   ('quantiles', 'ps', 'qs', 'f', 'min_val', 'max_val')
          freevars   ()
          cellvars   ()
-         filename   '/Users/t/repos/rvtools/rvtools/_constructors/uniform.py'
+         filename   '/Users/t/repos/rvtools/rvtools/construct/uniform.py'
          name       'from_quantiles'
          firstlineno 19
          lnotab 0x02012601400242014203280116011602
       code
          argcount  : 2
          nlocals   : 4
          stacksize : 5
@@ -314,20 +314,20 @@
          consts
             "\n    SciPy's ``uniform`` does not take the extrema of the distribution (it takes its own ``loc`` and ``scale``).\n\n    This is a convenience wrapper that allows you to create a (frozen) SciPy uniform distribution using the extrema\n    ``a`` and ``b``. ``a`` need not be less than ``b``.\n    "
             ('loc', 'scale')
          names      ('sorted', 'scipy', 'stats', 'uniform')
          varnames   ('a', 'b', 'min', 'max')
          freevars   ()
          cellvars   ()
-         filename   '/Users/t/repos/rvtools/rvtools/_constructors/uniform.py'
+         filename   '/Users/t/repos/rvtools/rvtools/construct/uniform.py'
          name       'from_extrema'
          firstlineno 34
          lnotab 0x02072801
       (None, None)
-   names      ('numbers', 'Real', 'scipy', 'scipy.interpolate', 'interp1d', 'rvtools._constructors._helpers', 'parse_spec', 'dict', 'uniform', 'from_quantiles', 'from_extrema')
+   names      ('numbers', 'Real', 'scipy', 'scipy.interpolate', 'interp1d', 'rvtools.construct._helpers', 'parse_spec', 'dict', 'uniform', 'from_quantiles', 'from_extrema')
    varnames   ()
    freevars   ()
    cellvars   ()
-   filename   '/Users/t/repos/rvtools/rvtools/_constructors/uniform.py'
+   filename   '/Users/t/repos/rvtools/rvtools/construct/uniform.py'
    name       '<module>'
    firstlineno 1
    lnotab 0x00ff02010c0208010c020c032c0a1c0f
```

### Comparing `rvtools-0.1.0/rvtools/_constructors/_helpers.py` & `rvtools-0.1.1/rvtools/construct/_helpers.py`

 * *Files identical despite different names*

### Comparing `rvtools-0.1.0/rvtools/_constructors/beta.py` & `rvtools-0.1.1/rvtools/construct/beta.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from numbers import Real
 
 import numpy as np
 import scipy
 
-from rvtools._constructors._helpers import parse_spec
+from rvtools.construct._helpers import parse_spec
 
 
 def beta(alpha: Real = None, beta: Real = None, *, quantiles: dict[Real, Real] = None, **kwargs):
     spec = parse_spec(alpha=alpha, beta=beta, quantiles=quantiles, **kwargs)
     if spec.keys() == {"alpha", "beta"}:
         return scipy.stats.beta(alpha, beta)
     elif spec.keys() == {"quantiles"}:
```

### Comparing `rvtools-0.1.0/rvtools/_constructors/lognorm.py` & `rvtools-0.1.1/rvtools/construct/lognorm.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from numbers import Real
 
 import numpy as np
 import scipy
 
-from rvtools._constructors._helpers import parse_spec
-from rvtools._constructors.norm import params_from_quantiles as norm_params_from_quantiles
+from rvtools.construct._helpers import parse_spec
+from rvtools.construct.norm import params_from_quantiles as norm_params_from_quantiles
 
 
 def lognorm(
     mu: Real = None,
     sigma: Real = None,
     *,
     mean: Real = None,
```

### Comparing `rvtools-0.1.0/rvtools/_constructors/norm.py` & `rvtools-0.1.1/rvtools/construct/norm.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from numbers import Real
 
 import scipy
 
-from rvtools._constructors._helpers import parse_spec
+from rvtools.construct._helpers import parse_spec
 
 
 def norm(mean: float = None, sd: float = None, *, quantiles: dict[Real, Real] = None, **kwargs):
     spec = parse_spec(mean=mean, sd=sd, quantiles=quantiles, **kwargs)
     if spec.keys() == {"mean", "sd"}:
         return scipy.stats.norm(mean, sd)
     elif spec.keys() == {"quantiles"}:
```

### Comparing `rvtools-0.1.0/rvtools/_constructors/uniform.py` & `rvtools-0.1.1/rvtools/construct/uniform.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from numbers import Real
 
 import scipy
 from scipy.interpolate import interp1d
 
-from rvtools._constructors._helpers import parse_spec
+from rvtools.construct._helpers import parse_spec
 
 
 def uniform(a: Real = None, b: Real = None, *, quantiles: dict[Real, Real] = None, **kwargs):
     spec = parse_spec(a=a, b=b, quantiles=quantiles, **kwargs)
     if spec.keys() == {"a", "b"}:
         return from_extrema(a, b)
     elif spec.keys() == {"quantiles"}:
```

### Comparing `rvtools-0.1.0/rvtools/types.py` & `rvtools-0.1.1/rvtools/types.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import scipy
 
 
-def is_frozen_normal(distribution):
+def is_frozen_norm(distribution):
     try:
         return isinstance(distribution.dist, scipy.stats._continuous_distns.norm_gen)
     except AttributeError:
         return False
 
 
-def is_frozen_lognormal(distribution):
+def is_frozen_lognorm(distribution):
     try:
         return isinstance(distribution.dist, scipy.stats._continuous_distns.lognorm_gen)
     except AttributeError:
         return False
 
 
 def is_frozen_beta(distribution):
```

### Comparing `rvtools-0.1.0/tests/test_constructors.py` & `rvtools-0.1.1/tests/test_constructors.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,13 @@
 import numpy as np
 import pytest
 import scipy
 
-import rvtools
-
-
-def assert_same_distribution(d1, d2):
-    """
-    Assert that two (frozen) distributions are the same.
-    """
-    assert d1.support() == d2.support()
-
-    xs = np.linspace(d1.ppf(0.001), d1.ppf(0.999))
-    assert d1.pdf(xs) == pytest.approx(d2.pdf(xs))
-
-    ps = np.linspace(0, 1)
-    assert d1.ppf(ps) == pytest.approx(d2.ppf(ps))
-
-    # ...We could check more things, but is there really any point?
+import rvtools.construct as construct
+from tests.conftest import assert_same_distribution
 
 
 def assert_has_quantiles(d, quantiles):
     """
     Assert that a (frozen) distribution has the given quantiles.
     """
     for p, q in quantiles.items():
@@ -36,33 +22,33 @@
     @pytest.fixture(params=[1, 5], ids=lambda p: f"beta={p}")
     def beta(self, request):
         return request.param
 
     @pytest.mark.parametrize("as_kwargs", [True, False], ids=lambda x: "kwargs" if x else "args")
     def test_from_alpha_beta(self, alpha, beta, as_kwargs):
         if as_kwargs:
-            our_d = rvtools.beta(alpha=alpha, beta=beta)
+            our_d = construct.beta(alpha=alpha, beta=beta)
         else:
-            our_d = rvtools.beta(alpha, beta)
+            our_d = construct.beta(alpha, beta)
         scipy_d = scipy.stats.beta(alpha, beta)
         assert_same_distribution(our_d, scipy_d)
 
     @pytest.fixture(
         params=[{0.1: 0.2, 0.5: 0.85}, {0.1: 0.5, 0.5: 0.99}, {0.001: 0.5, 0.5: 0.99}],  #  #  #
         ids=lambda p: f"quantiles={p}",
     )
     def quantiles(self, request):
         return request.param
 
     def test_from_quantiles(self, quantiles):
-        assert_has_quantiles(rvtools.beta(quantiles=quantiles), quantiles)
+        assert_has_quantiles(construct.beta(quantiles=quantiles), quantiles)
 
     def test_too_many_args(self):
         with pytest.raises(ValueError, match="You must specify"):
-            rvtools.beta(1, 1, quantiles={0.1: 0.1, 0.5: 0.5})
+            construct.beta(1, 1, quantiles={0.1: 0.1, 0.5: 0.5})
 
 
 class TestLognorm:
     @pytest.fixture(params=[0.5, 3], ids=lambda p: f"mean={p}")
     def mean(self, request):
         return request.param
 
@@ -81,40 +67,40 @@
     @pytest.fixture
     def quantiles(self):
         return {0.1: 1, 0.9: 10}
 
     @pytest.mark.parametrize("as_kwargs", [True, False], ids=lambda x: "kwargs" if x else "args")
     def test_from_mu_sigma(self, mu, sigma, as_kwargs):
         if as_kwargs:
-            dist = rvtools.lognorm(mu=mu, sigma=sigma)
+            dist = construct.lognorm(mu=mu, sigma=sigma)
         else:
-            dist = rvtools.lognorm(mu, sigma)
+            dist = construct.lognorm(mu, sigma)
 
         # Check that the log of our distribution is normal
         ps = np.linspace(0, 1)
         got = np.log(dist.ppf(ps))
         want = scipy.stats.norm.ppf(ps, mu, sigma)
         assert got == pytest.approx(want)
 
     def test_from_mean_sd(self, mean, sd):
-        dist = rvtools.lognorm(mean=mean, sd=sd)
+        dist = construct.lognorm(mean=mean, sd=sd)
         got = (dist.mean(), dist.std())
         assert got == pytest.approx((mean, sd))
 
     def test_from_quantiles(self, quantiles):
-        dist = rvtools.lognorm(quantiles=quantiles)
+        dist = construct.lognorm(quantiles=quantiles)
         assert_has_quantiles(dist, quantiles)
 
     def test_inconsistent_spec(self):
         with pytest.raises(ValueError, match="You must specify"):
-            rvtools.lognorm(1, 1, quantiles={0.1: 0.1, 0.5: 0.5})
+            construct.lognorm(1, 1, quantiles={0.1: 0.1, 0.5: 0.5})
         with pytest.raises(ValueError, match="You must specify"):
-            rvtools.lognorm(1, 1, mean=1)
+            construct.lognorm(1, 1, mean=1)
         with pytest.raises(ValueError, match="You must specify"):
-            rvtools.lognorm(mean=1, sd=1, mu=1)
+            construct.lognorm(mean=1, sd=1, mu=1)
 
 
 class TestNorm:
     @pytest.fixture(params=[0.5, 3], ids=lambda p: f"mean={p}")
     def mean(self, request):
         return request.param
 
@@ -123,25 +109,25 @@
         return request.param
 
     @pytest.fixture
     def quantiles(self):
         return {0.1: -1, 0.9: 1}
 
     def test_from_mean_sd(self, mean, sd):
-        our_d = rvtools.norm(mean=mean, sd=sd)
+        our_d = construct.norm(mean=mean, sd=sd)
         scipy_d = scipy.stats.norm(mean, sd)
         assert_same_distribution(our_d, scipy_d)
 
     def test_from_quantiles(self, quantiles):
-        dist = rvtools.norm(quantiles=quantiles)
+        dist = construct.norm(quantiles=quantiles)
         assert_has_quantiles(dist, quantiles)
 
     def test_too_many_args(self):
         with pytest.raises(ValueError, match="You must specify"):
-            rvtools.norm(1, 1, quantiles={0.1: 0.1, 0.5: 0.5})
+            construct.norm(1, 1, quantiles={0.1: 0.1, 0.5: 0.5})
 
 
 class TestUniform:
     @pytest.fixture(
         params=[
             # A simple case
             (1, 2),
@@ -155,18 +141,18 @@
         return request.param
 
     @pytest.fixture(params=[{0.1: 1, 0.9: 2}], ids=lambda p: f"quantiles={p}")
     def quantiles(self, request):
         return request.param
 
     def test_from_pair(self, pair):
-        dist = rvtools.uniform(*pair)
+        dist = construct.uniform(*pair)
         assert dist.ppf(0.5) == pytest.approx(np.mean(pair))
         assert dist.support() == pytest.approx(sorted(pair))
 
     def test_from_quantiles(self, quantiles):
-        dist = rvtools.uniform(quantiles=quantiles)
+        dist = construct.uniform(quantiles=quantiles)
         assert_has_quantiles(dist, quantiles)
 
     def test_degenerate_rvs(self):
-        our_d = rvtools.uniform(1, 1)
+        our_d = construct.uniform(1, 1)
         assert all(our_d.rvs(size=10) == [1] * 10)
```

### Comparing `rvtools-0.1.0/tests/test_parse_spec.py` & `rvtools-0.1.1/tests/test_parse_spec.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import pytest
 
-from rvtools._constructors._helpers import parse_spec, collect_kwarg_quantiles
+from rvtools.construct._helpers import parse_spec, collect_kwarg_quantiles
 
 
 class TestParseSpec:
     def test_no_quantiles(self):
         spec = parse_spec(a=1, b=2)
         assert spec == {"a": 1, "b": 2}
```

### Comparing `rvtools-0.1.0/tests/test_types.py` & `rvtools-0.1.1/tests/test_types.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import scipy
 
 import rvtools.types
 
 
 def test_normal():
-    assert rvtools.types.is_frozen_normal(scipy.stats.norm(1, 1))
-    assert not rvtools.types.is_frozen_normal(scipy.stats.uniform(1, 1))
+    assert rvtools.types.is_frozen_norm(scipy.stats.norm(1, 1))
+    assert not rvtools.types.is_frozen_norm(scipy.stats.uniform(1, 1))
 
 
 def test_lognormal():
-    assert rvtools.types.is_frozen_lognormal(scipy.stats.lognorm(1, 1))
-    assert not rvtools.types.is_frozen_lognormal(scipy.stats.uniform(1, 1))
+    assert rvtools.types.is_frozen_lognorm(scipy.stats.lognorm(1, 1))
+    assert not rvtools.types.is_frozen_lognorm(scipy.stats.uniform(1, 1))
 
 
 def test_beta():
     assert rvtools.types.is_frozen_beta(scipy.stats.beta(1, 1))
     assert not rvtools.types.is_frozen_beta(scipy.stats.uniform(1, 1))
```

