# Comparing `tmp/flake8_django_migrations-0.3.0.tar.gz` & `tmp/flake8_django_migrations-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flake8_django_migrations-0.3.0.tar", max compression
+gzip compressed data, was "flake8_django_migrations-1.0.0.tar", max compression
```

## Comparing `flake8_django_migrations-0.3.0.tar` & `flake8_django_migrations-1.0.0.tar`

### file list

```diff
@@ -1,10 +1,9 @@
--rw-r--r--   0        0        0     3769 2022-11-20 18:59:33.618824 flake8_django_migrations-0.3.0/README.md
--rw-r--r--   0        0        0     1559 2022-11-20 18:59:34.394816 flake8_django_migrations-0.3.0/pyproject.toml
--rw-r--r--   0        0        0       72 2022-11-20 18:59:34.370817 flake8_django_migrations-0.3.0/src/flake8_django_migrations/__init__.py
--rw-r--r--   0        0        0       53 2022-11-20 18:59:33.618824 flake8_django_migrations-0.3.0/src/flake8_django_migrations/checkers/__init__.py
--rw-r--r--   0        0        0      369 2022-11-20 18:59:33.618824 flake8_django_migrations-0.3.0/src/flake8_django_migrations/checkers/base.py
--rw-r--r--   0        0        0       73 2022-11-20 18:59:33.618824 flake8_django_migrations-0.3.0/src/flake8_django_migrations/checkers/issue.py
--rw-r--r--   0        0        0      703 2022-11-20 18:59:33.618824 flake8_django_migrations-0.3.0/src/flake8_django_migrations/checkers/remove_field.py
--rw-r--r--   0        0        0     1126 2022-11-20 18:59:33.618824 flake8_django_migrations-0.3.0/src/flake8_django_migrations/plugin.py
--rw-r--r--   0        0        0     4933 1970-01-01 00:00:00.000000 flake8_django_migrations-0.3.0/setup.py
--rw-r--r--   0        0        0     5030 1970-01-01 00:00:00.000000 flake8_django_migrations-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     3810 2023-06-27 12:25:24.539003 flake8_django_migrations-1.0.0/README.md
+-rw-r--r--   0        0        0     1559 2023-06-27 12:25:25.379027 flake8_django_migrations-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0       72 2023-06-27 12:25:25.343026 flake8_django_migrations-1.0.0/src/flake8_django_migrations/__init__.py
+-rw-r--r--   0        0        0       53 2023-06-27 12:25:24.539003 flake8_django_migrations-1.0.0/src/flake8_django_migrations/checkers/__init__.py
+-rw-r--r--   0        0        0      369 2023-06-27 12:25:24.539003 flake8_django_migrations-1.0.0/src/flake8_django_migrations/checkers/base.py
+-rw-r--r--   0        0        0       73 2023-06-27 12:25:24.539003 flake8_django_migrations-1.0.0/src/flake8_django_migrations/checkers/issue.py
+-rw-r--r--   0        0        0      703 2023-06-27 12:25:24.539003 flake8_django_migrations-1.0.0/src/flake8_django_migrations/checkers/remove_field.py
+-rw-r--r--   0        0        0      951 2023-06-27 12:25:24.539003 flake8_django_migrations-1.0.0/src/flake8_django_migrations/plugin.py
+-rw-r--r--   0        0        0     5022 1970-01-01 00:00:00.000000 flake8_django_migrations-1.0.0/PKG-INFO
```

### Comparing `flake8_django_migrations-0.3.0/README.md` & `flake8_django_migrations-1.0.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # flake8-django-migrations
 
 <p align="center">
-  <a href="https://github.com/browniebroke/flake8-django-migrations/actions?query=workflow%3ACI">
-    <img alt="CI Status" src="https://img.shields.io/github/workflow/status/browniebroke/flake8-django-migrations/CI?label=CI&logo=github&style=flat-square">
+  <a href="https://github.com/browniebroke/flake8-django-migrations/actions/workflows/ci.yml?query=branch%3Amain">
+    <img alt="CI Status" src="https://img.shields.io/github/actions/workflow/status/browniebroke/flake8-django-migrations/ci.yml?branch=main&label=CI&logo=github&style=flat-square">
   </a>
   <a href="https://codecov.io/gh/browniebroke/flake8-django-migrations">
     <img src="https://img.shields.io/codecov/c/github/browniebroke/flake8-django-migrations.svg?logo=codecov&style=flat-square" alt="Test coverage percentage">
   </a>
 </p>
 <p align="center">
   <a href="https://python-poetry.org/">
```

### Comparing `flake8_django_migrations-0.3.0/pyproject.toml` & `flake8_django_migrations-1.0.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "flake8-django-migrations"
-version = "0.3.0"
+version = "1.0.0"
 description = "Flake8 plugin to lint for backwards incompatible database migrations"
 authors = ["Bruno Alla <bruno.alla@festicket.com>"]
 license = "MIT"
 readme = "README.md"
 keywords = ["flake8", "lint", "django", "migrations"]
 repository = "https://github.com/browniebroke/flake8-django-migrations"
 classifiers = [
@@ -14,15 +14,15 @@
     "Operating System :: OS Independent",
     "Environment :: Console",
     "Framework :: Flake8",
     "Topic :: Software Development :: Quality Assurance"
 ]
 
 [tool.poetry.dependencies]
-python = "^3.7"
+python = "^3.8"
 flake8 = ">=3.7"
 astor = ">=0.1"
 importlib-metadata = {version = ">=0.9", python = "<3.8"}
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.0"
 pytest-cov = "^4.0"
```

### Comparing `flake8_django_migrations-0.3.0/src/flake8_django_migrations/checkers/remove_field.py` & `flake8_django_migrations-1.0.0/src/flake8_django_migrations/checkers/remove_field.py`

 * *Files identical despite different names*

### Comparing `flake8_django_migrations-0.3.0/src/flake8_django_migrations/plugin.py` & `flake8_django_migrations-1.0.0/src/flake8_django_migrations/plugin.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,21 +1,14 @@
 import ast
-import sys
+import importlib.metadata as importlib_metadata
 from typing import Any, Generator, List, Tuple, Type
 
 from .checkers.issue import Issue
 from .checkers.remove_field import RemoveFieldChecker
 
-if sys.version_info < (3, 8):  # pragma: no cover (<PY38)
-    # Third party
-    import importlib_metadata
-else:  # pragma: no cover (PY38+)
-    # Core Library
-    import importlib.metadata as importlib_metadata
-
 
 class Visitor(ast.NodeVisitor):
     checkers = [RemoveFieldChecker()]
 
     def __init__(self) -> None:
         self.issues: List[Issue] = []
```

### Comparing `flake8_django_migrations-0.3.0/setup.py` & `flake8_django_migrations-1.0.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,309 +1,314 @@
-00000000: 2320 2d2a 2d20 636f 6469 6e67 3a20 7574  # -*- coding: ut
-00000010: 662d 3820 2d2a 2d0a 6672 6f6d 2073 6574  f-8 -*-.from set
-00000020: 7570 746f 6f6c 7320 696d 706f 7274 2073  uptools import s
-00000030: 6574 7570 0a0a 7061 636b 6167 655f 6469  etup..package_di
-00000040: 7220 3d20 5c0a 7b27 273a 2027 7372 6327  r = \.{'': 'src'
-00000050: 7d0a 0a70 6163 6b61 6765 7320 3d20 5c0a  }..packages = \.
-00000060: 5b27 666c 616b 6538 5f64 6a61 6e67 6f5f  ['flake8_django_
-00000070: 6d69 6772 6174 696f 6e73 272c 2027 666c  migrations', 'fl
-00000080: 616b 6538 5f64 6a61 6e67 6f5f 6d69 6772  ake8_django_migr
-00000090: 6174 696f 6e73 2e63 6865 636b 6572 7327  ations.checkers'
-000000a0: 5d0a 0a70 6163 6b61 6765 5f64 6174 6120  ]..package_data 
-000000b0: 3d20 5c0a 7b27 273a 205b 272a 275d 7d0a  = \.{'': ['*']}.
-000000c0: 0a69 6e73 7461 6c6c 5f72 6571 7569 7265  .install_require
-000000d0: 7320 3d20 5c0a 5b27 6173 746f 723e 3d30  s = \.['astor>=0
-000000e0: 2e31 272c 2027 666c 616b 6538 3e3d 332e  .1', 'flake8>=3.
-000000f0: 3727 5d0a 0a65 7874 7261 735f 7265 7175  7']..extras_requ
-00000100: 6972 6520 3d20 5c0a 7b27 3a70 7974 686f  ire = \.{':pytho
-00000110: 6e5f 7665 7273 696f 6e20 3c20 2233 2e38  n_version < "3.8
-00000120: 2227 3a20 5b27 696d 706f 7274 6c69 622d  "': ['importlib-
-00000130: 6d65 7461 6461 7461 3e3d 302e 3927 5d7d  metadata>=0.9']}
-00000140: 0a0a 656e 7472 795f 706f 696e 7473 203d  ..entry_points =
-00000150: 205c 0a7b 2766 6c61 6b65 382e 6578 7465   \.{'flake8.exte
-00000160: 6e73 696f 6e27 3a20 5b27 444d 203d 2066  nsion': ['DM = f
-00000170: 6c61 6b65 385f 646a 616e 676f 5f6d 6967  lake8_django_mig
-00000180: 7261 7469 6f6e 733a 506c 7567 696e 275d  rations:Plugin']
-00000190: 7d0a 0a73 6574 7570 5f6b 7761 7267 7320  }..setup_kwargs 
-000001a0: 3d20 7b0a 2020 2020 276e 616d 6527 3a20  = {.    'name': 
-000001b0: 2766 6c61 6b65 382d 646a 616e 676f 2d6d  'flake8-django-m
-000001c0: 6967 7261 7469 6f6e 7327 2c0a 2020 2020  igrations',.    
-000001d0: 2776 6572 7369 6f6e 273a 2027 302e 332e  'version': '0.3.
-000001e0: 3027 2c0a 2020 2020 2764 6573 6372 6970  0',.    'descrip
-000001f0: 7469 6f6e 273a 2027 466c 616b 6538 2070  tion': 'Flake8 p
-00000200: 6c75 6769 6e20 746f 206c 696e 7420 666f  lugin to lint fo
-00000210: 7220 6261 636b 7761 7264 7320 696e 636f  r backwards inco
-00000220: 6d70 6174 6962 6c65 2064 6174 6162 6173  mpatible databas
-00000230: 6520 6d69 6772 6174 696f 6e73 272c 0a20  e migrations',. 
-00000240: 2020 2027 6c6f 6e67 5f64 6573 6372 6970     'long_descrip
-00000250: 7469 6f6e 273a 2027 2320 666c 616b 6538  tion': '# flake8
-00000260: 2d64 6a61 6e67 6f2d 6d69 6772 6174 696f  -django-migratio
-00000270: 6e73 5c6e 5c6e 3c70 2061 6c69 676e 3d22  ns\n\n<p align="
-00000280: 6365 6e74 6572 223e 5c6e 2020 3c61 2068  center">\n  <a h
-00000290: 7265 663d 2268 7474 7073 3a2f 2f67 6974  ref="https://git
-000002a0: 6875 622e 636f 6d2f 6272 6f77 6e69 6562  hub.com/brownieb
-000002b0: 726f 6b65 2f66 6c61 6b65 382d 646a 616e  roke/flake8-djan
-000002c0: 676f 2d6d 6967 7261 7469 6f6e 732f 6163  go-migrations/ac
-000002d0: 7469 6f6e 733f 7175 6572 793d 776f 726b  tions?query=work
-000002e0: 666c 6f77 2533 4143 4922 3e5c 6e20 2020  flow%3ACI">\n   
-000002f0: 203c 696d 6720 616c 743d 2243 4920 5374   <img alt="CI St
-00000300: 6174 7573 2220 7372 633d 2268 7474 7073  atus" src="https
-00000310: 3a2f 2f69 6d67 2e73 6869 656c 6473 2e69  ://img.shields.i
-00000320: 6f2f 6769 7468 7562 2f77 6f72 6b66 6c6f  o/github/workflo
-00000330: 772f 7374 6174 7573 2f62 726f 776e 6965  w/status/brownie
-00000340: 6272 6f6b 652f 666c 616b 6538 2d64 6a61  broke/flake8-dja
-00000350: 6e67 6f2d 6d69 6772 6174 696f 6e73 2f43  ngo-migrations/C
-00000360: 493f 6c61 6265 6c3d 4349 266c 6f67 6f3d  I?label=CI&logo=
-00000370: 6769 7468 7562 2673 7479 6c65 3d66 6c61  github&style=fla
-00000380: 742d 7371 7561 7265 223e 5c6e 2020 3c2f  t-square">\n  </
-00000390: 613e 5c6e 2020 3c61 2068 7265 663d 2268  a>\n  <a href="h
-000003a0: 7474 7073 3a2f 2f63 6f64 6563 6f76 2e69  ttps://codecov.i
-000003b0: 6f2f 6768 2f62 726f 776e 6965 6272 6f6b  o/gh/browniebrok
-000003c0: 652f 666c 616b 6538 2d64 6a61 6e67 6f2d  e/flake8-django-
-000003d0: 6d69 6772 6174 696f 6e73 223e 5c6e 2020  migrations">\n  
-000003e0: 2020 3c69 6d67 2073 7263 3d22 6874 7470    <img src="http
-000003f0: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
-00000400: 696f 2f63 6f64 6563 6f76 2f63 2f67 6974  io/codecov/c/git
-00000410: 6875 622f 6272 6f77 6e69 6562 726f 6b65  hub/browniebroke
-00000420: 2f66 6c61 6b65 382d 646a 616e 676f 2d6d  /flake8-django-m
-00000430: 6967 7261 7469 6f6e 732e 7376 673f 6c6f  igrations.svg?lo
-00000440: 676f 3d63 6f64 6563 6f76 2673 7479 6c65  go=codecov&style
-00000450: 3d66 6c61 742d 7371 7561 7265 2220 616c  =flat-square" al
-00000460: 743d 2254 6573 7420 636f 7665 7261 6765  t="Test coverage
-00000470: 2070 6572 6365 6e74 6167 6522 3e5c 6e20   percentage">\n 
-00000480: 203c 2f61 3e5c 6e3c 2f70 3e5c 6e3c 7020   </a>\n</p>\n<p 
-00000490: 616c 6967 6e3d 2263 656e 7465 7222 3e5c  align="center">\
-000004a0: 6e20 203c 6120 6872 6566 3d22 6874 7470  n  <a href="http
-000004b0: 733a 2f2f 7079 7468 6f6e 2d70 6f65 7472  s://python-poetr
-000004c0: 792e 6f72 672f 223e 5c6e 2020 2020 3c69  y.org/">\n    <i
-000004d0: 6d67 2073 7263 3d22 6874 7470 733a 2f2f  mg src="https://
-000004e0: 696d 672e 7368 6965 6c64 732e 696f 2f62  img.shields.io/b
-000004f0: 6164 6765 2f70 6163 6b61 6769 6e67 2d70  adge/packaging-p
-00000500: 6f65 7472 792d 3239 3962 6437 3f73 7479  oetry-299bd7?sty
-00000510: 6c65 3d66 6c61 742d 7371 7561 7265 266c  le=flat-square&l
-00000520: 6f67 6f3d 6461 7461 3a69 6d61 6765 2f70  ogo=data:image/p
-00000530: 6e67 3b62 6173 6536 342c 6956 424f 5277  ng;base64,iVBORw
-00000540: 304b 4767 6f41 4141 414e 5355 6845 5567  0KGgoAAAANSUhEUg
-00000550: 4141 4141 3441 4141 4153 4341 5941 4141  AAAA4AAAASCAYAAA
-00000560: 4272 584f 3878 4141 4141 4358 4249 5758  BrXO8xAAAACXBIWX
-00000570: 4d41 4141 7354 4141 414c 4577 4541 6d70  MAAAsTAAALEwEAmp
-00000580: 7759 4141 4141 4158 4e53 5230 4941 7273  wYAAAAAXNSR0IArs
-00000590: 3463 3651 4141 4141 526e 5155 3142 4141  4c6QAAAARnQU1BAA
-000005a0: 4378 6a77 7638 5951 5541 4141 4a4a 5355  Cxjwv8YQUAAAJJSU
-000005b0: 5242 5648 6742 665a 4c50 6131 4e42 454d  RBVHgBfZLPa1NBEM
-000005c0: 652f 7337 744e 586f 7857 314b 4a51 4b61  e/s7tNXoxW1KJQKa
-000005d0: 5548 6b58 6851 7648 6757 3655 4851 5130  UHkXhQvHgW6UHQQ0
-000005e0: 3943 4253 2f36 5633 684b 632f 4150 3843  9CBS/6V3hKc/AP8C
-000005f0: 7143 7255 6370 6d6f 7033 4378 3438 6544  qCrUcpmop3Cx48eD
-00000600: 4234 7945 4543 6a56 5172 6c5a 6238 3043  B4yEECjVQrlZb80C
-00000610: 524e 3874 364f 4d2f 7465 6167 5678 595a  RN8t6OM/teagVxYZ
-00000620: 6933 382b 597a 3835 3364 4a62 7a6f 4d56  i38+Yz853dJbzoMV
-00000630: 334d 4d38 634a 5563 4c4d 5355 4b49 4538  3MM8cJUcLMSUKIE8
-00000640: 417a 5132 5069 655a 7a46 7845 4a4f 484d  AzQ2PieZzFxEJOHM
-00000650: 4f67 4d51 512b 6455 6753 4163 6b4e 5868  OgMQQ+dUgSAckNXh
-00000660: 6170 552f 4e4d 6844 5357 4c73 3142 3234  apU/NMhDSWLs1B24
-00000670: 4138 734f 3178 724e 344e 4543 6b63 4143  A8sO1xrN4NECkcAC
-00000680: 3941 536b 6949 4a63 366b 3554 5269 5544  9ASkiIJc6k5TRiUD
-00000690: 5068 6e79 4d4d 6468 4b63 2b5a 7831 396c  PhnyMMdhKc+Zx19l
-000006a0: 3653 6779 6557 3736 4245 4f4e 5939 6578  6SgyeW76BEONY9ex
-000006b0: 5651 4d7a 4b45 7847 4b77 7750 7343 7a7a  VQMzKExGKwwPsCzz
-000006c0: 6137 4b47 5353 5752 5745 5168 7945 6144  a7KGSSWRWEQhyEaD
-000006d0: 5870 365a 4845 7234 3136 7967 6269 4b59  Xp6ZHEr416ygbiKY
-000006e0: 4f64 3754 4557 7676 6351 4965 7573 4859  Od7TEWvvcQIeusHY
-000006f0: 4d4a 4768 5477 4639 7937 7347 6e53 7761  MJGhTwF9y7sGnSwa
-00000700: 5779 4641 6979 6f78 7a71 5730 504d 2f52  WyFAiyoxzqW0PM/R
-00000710: 6a67 6850 7846 3270 5752 6541 6f77 5445  jghPxF2pWReAowTE
-00000720: 586e 4468 3078 6763 4c73 386c 3259 516d  XnDh0xgcLs8l2YQm
-00000730: 4f72 6a33 4e37 4279 6971 456f 4830 6341  Orj3N7ByiqEoH0cA
-00000740: 5273 3475 3738 5767 4156 6b6f 4544 4944  Rs4u78WgAVkoEDID
-00000750: 6f4f 6933 416b 634c 4f48 5536 3052 4967  oOi3AkcLOHU60RIg
-00000760: 3577 4334 5a75 5443 3746 6148 4b51 6d38  5wC4ZuTC7FaHKQm8
-00000770: 4871 3166 5175 534f 4276 582f 736f 646d  Hq1fQuSOBvX/sodm
-00000780: 4e4a 5342 3567 6561 4635 4350 496b 5565  NJSB5geaF5CPIkUe
-00000790: 6563 644d 7869 656f 524f 356a 7a39 6268  ecdMxieoRO5jz9bh
-000007a0: 654c 362f 7458 6a72 7743 7958 2f55 5942  eL6/tXjrwCyX/UYB
-000007b0: 5563 6a43 6157 486c 6a78 3178 6958 367a  UcjCaWHljx1xiX6z
-000007c0: 3978 456a 6b59 417a 6247 566e 4238 7076  9xEjkYAzbGVnB8pv
-000007d0: 4c6d 7958 6d39 6570 2b57 3843 6d73 5348  LmyXm9ep+W8CmsSH
-000007e0: 5151 5937 375a 7831 7a62 6f78 4156 3077  QQY77Zx1zboxAV0w
-000007f0: 3779 624d 6851 6d66 7164 6d6d 7733 6e45  7ybMhQmfqdmmw3nE
-00000800: 7031 4930 5a2b 4647 4f36 4d38 4c5a 646f  p1I0Z+FGO6M8LZdo
-00000810: 795a 6e75 7a7a 4264 6a49 5369 634b 526e  yZnuzzBdjISicKRn
-00000820: 7078 7a49 3966 5062 2b30 6f59 5873 4e64  pxzI9fPb+0oYXsNd
-00000830: 7969 2b64 3368 3962 6d39 4d57 5948 4674  yi+d3h9bm9MWYHFt
-00000840: 5065 495a 664c 777a 6d46 444b 7931 6169  PeIZfLwzmFDKy1ai
-00000850: 3370 2b50 446c 7331 4c6c 7a34 7979 4670  3p+PDls1Llz4yyFp
-00000860: 6665 7278 6a6e 796a 4a44 5345 7939 4361  ferxjnyjJDSEy9Ca
-00000870: 4378 356d 3263 4a50 6572 7136 586d 3334  Cx5m2cJPerq6Xm34
-00000880: 6554 725a 7433 5071 7859 4f31 584f 7744  eTrZt3PqxYO1XOwD
-00000890: 595a 7246 6c48 3166 576e 7055 3338 5939  YZrFlH1fWnpU38Y9
-000008a0: 4852 7a65 336c 6a30 764f 756a 5a63 584b  HRze3lj0vOujZcXK
-000008b0: 7575 586d 336a 502b 7333 4b62 5a56 7261  uuXm3jP+s3KbZVra
-000008c0: 3779 3245 4141 4141 4141 5355 564f 524b  7y2EAAAAAASUVORK
-000008d0: 3543 5949 493d 2220 616c 743d 2250 6f65  5CYII=" alt="Poe
-000008e0: 7472 7922 3e5c 6e20 203c 2f61 3e5c 6e20  try">\n  </a>\n 
-000008f0: 203c 6120 6872 6566 3d22 6874 7470 733a   <a href="https:
-00000900: 2f2f 6769 7468 7562 2e63 6f6d 2f61 6d62  //github.com/amb
-00000910: 762f 626c 6163 6b22 3e5c 6e20 2020 203c  v/black">\n    <
-00000920: 696d 6720 7372 633d 2268 7474 7073 3a2f  img src="https:/
-00000930: 2f69 6d67 2e73 6869 656c 6473 2e69 6f2f  /img.shields.io/
-00000940: 6261 6467 652f 636f 6465 2532 3073 7479  badge/code%20sty
-00000950: 6c65 2d62 6c61 636b 2d30 3030 3030 302e  le-black-000000.
-00000960: 7376 673f 7374 796c 653d 666c 6174 2d73  svg?style=flat-s
-00000970: 7175 6172 6522 2061 6c74 3d22 626c 6163  quare" alt="blac
-00000980: 6b22 3e5c 6e20 203c 2f61 3e5c 6e20 203c  k">\n  </a>\n  <
-00000990: 6120 6872 6566 3d22 6874 7470 733a 2f2f  a href="https://
-000009a0: 6769 7468 7562 2e63 6f6d 2f70 7265 2d63  github.com/pre-c
-000009b0: 6f6d 6d69 742f 7072 652d 636f 6d6d 6974  ommit/pre-commit
-000009c0: 223e 5c6e 2020 2020 3c69 6d67 2073 7263  ">\n    <img src
-000009d0: 3d22 6874 7470 733a 2f2f 696d 672e 7368  ="https://img.sh
-000009e0: 6965 6c64 732e 696f 2f62 6164 6765 2f70  ields.io/badge/p
-000009f0: 7265 2d2d 636f 6d6d 6974 2d65 6e61 626c  re--commit-enabl
-00000a00: 6564 2d62 7269 6768 7467 7265 656e 3f6c  ed-brightgreen?l
-00000a10: 6f67 6f3d 7072 652d 636f 6d6d 6974 266c  ogo=pre-commit&l
-00000a20: 6f67 6f43 6f6c 6f72 3d77 6869 7465 2673  ogoColor=white&s
-00000a30: 7479 6c65 3d66 6c61 742d 7371 7561 7265  tyle=flat-square
-00000a40: 2220 616c 743d 2270 7265 2d63 6f6d 6d69  " alt="pre-commi
-00000a50: 7422 3e5c 6e20 203c 2f61 3e5c 6e3c 2f70  t">\n  </a>\n</p
-00000a60: 3e5c 6e3c 7020 616c 6967 6e3d 2263 656e  >\n<p align="cen
-00000a70: 7465 7222 3e5c 6e20 203c 6120 6872 6566  ter">\n  <a href
-00000a80: 3d22 6874 7470 733a 2f2f 7079 7069 2e6f  ="https://pypi.o
-00000a90: 7267 2f70 726f 6a65 6374 2f66 6c61 6b65  rg/project/flake
-00000aa0: 382d 646a 616e 676f 2d6d 6967 7261 7469  8-django-migrati
-00000ab0: 6f6e 732f 223e 5c6e 2020 2020 3c69 6d67  ons/">\n    <img
-00000ac0: 2073 7263 3d22 6874 7470 733a 2f2f 696d   src="https://im
-00000ad0: 672e 7368 6965 6c64 732e 696f 2f70 7970  g.shields.io/pyp
-00000ae0: 692f 762f 666c 616b 6538 2d64 6a61 6e67  i/v/flake8-djang
-00000af0: 6f2d 6d69 6772 6174 696f 6e73 2e73 7667  o-migrations.svg
-00000b00: 3f6c 6f67 6f3d 7079 7468 6f6e 2661 6d70  ?logo=python&amp
-00000b10: 3b6c 6f67 6f43 6f6c 6f72 3d66 6666 2661  ;logoColor=fff&a
-00000b20: 6d70 3b73 7479 6c65 3d66 6c61 742d 7371  mp;style=flat-sq
-00000b30: 7561 7265 2220 616c 743d 2250 7950 6920  uare" alt="PyPi 
-00000b40: 5374 6174 7573 223e 5c6e 2020 3c2f 613e  Status">\n  </a>
-00000b50: 5c6e 2020 3c69 6d67 2073 7263 3d22 6874  \n  <img src="ht
-00000b60: 7470 733a 2f2f 696d 672e 7368 6965 6c64  tps://img.shield
-00000b70: 732e 696f 2f70 7970 692f 7079 7665 7273  s.io/pypi/pyvers
-00000b80: 696f 6e73 2f66 6c61 6b65 382d 646a 616e  ions/flake8-djan
-00000b90: 676f 2d6d 6967 7261 7469 6f6e 732e 7376  go-migrations.sv
-00000ba0: 673f 7374 796c 653d 666c 6174 2d73 7175  g?style=flat-squ
-00000bb0: 6172 6522 2061 6c74 3d22 7079 7665 7273  are" alt="pyvers
-00000bc0: 696f 6e73 223e 5c6e 2020 3c69 6d67 2073  ions">\n  <img s
-00000bd0: 7263 3d22 6874 7470 733a 2f2f 696d 672e  rc="https://img.
-00000be0: 7368 6965 6c64 732e 696f 2f70 7970 692f  shields.io/pypi/
-00000bf0: 6c2f 666c 616b 6538 2d64 6a61 6e67 6f2d  l/flake8-django-
-00000c00: 6d69 6772 6174 696f 6e73 2e73 7667 3f73  migrations.svg?s
-00000c10: 7479 6c65 3d66 6c61 742d 7371 7561 7265  tyle=flat-square
-00000c20: 2220 616c 743d 226c 6963 656e 7365 223e  " alt="license">
-00000c30: 5c6e 3c2f 703e 5c6e 5c6e 466c 616b 6538  \n</p>\n\nFlake8
-00000c40: 2070 6c75 6769 6e20 746f 206c 696e 7420   plugin to lint 
-00000c50: 666f 7220 6261 636b 7761 7264 7320 696e  for backwards in
-00000c60: 636f 6d70 6174 6962 6c65 2064 6174 6162  compatible datab
-00000c70: 6173 6520 6d69 6772 6174 696f 6e73 2e5c  ase migrations.\
-00000c80: 6e5c 6e23 2320 496e 7374 616c 6c61 7469  n\n## Installati
-00000c90: 6f6e 5c6e 5c6e 496e 7374 616c 6c20 7573  on\n\nInstall us
-00000ca0: 696e 6720 6070 6970 6020 286f 7220 796f  ing `pip` (or yo
-00000cb0: 7572 2066 6176 6f75 7269 7465 2070 6163  ur favourite pac
-00000cc0: 6b61 6765 206d 616e 6167 6572 293a 5c6e  kage manager):\n
-00000cd0: 5c6e 6060 6073 685c 6e70 6970 2069 6e73  \n```sh\npip ins
-00000ce0: 7461 6c6c 2066 6c61 6b65 382d 646a 616e  tall flake8-djan
-00000cf0: 676f 2d6d 6967 7261 7469 6f6e 735c 6e60  go-migrations\n`
-00000d00: 6060 5c6e 5c6e 2323 2055 7361 6765 5c6e  ``\n\n## Usage\n
-00000d10: 5c6e 5468 6973 2070 6c75 6769 6e20 7368  \nThis plugin sh
-00000d20: 6f75 6c64 2062 6520 7573 6564 2061 7574  ould be used aut
-00000d30: 6f6d 6174 6963 616c 6c79 2077 6865 6e20  omatically when 
-00000d40: 7275 6e6e 696e 6720 666c 616b 6538 3a5c  running flake8:\
-00000d50: 6e5c 6e60 6060 7368 5c6e 666c 616b 6538  n\n```sh\nflake8
-00000d60: 5c6e 6060 605c 6e5c 6e23 2320 4368 6563  \n```\n\n## Chec
-00000d70: 6b73 5c6e 5c6e 5468 6973 2069 7320 7468  ks\n\nThis is th
-00000d80: 6520 6c69 7374 206f 6620 6368 6563 6b73  e list of checks
-00000d90: 2063 7572 7265 6e74 6c79 2069 6d70 6c65   currently imple
-00000da0: 6d65 6e74 6564 2062 7920 7468 6973 2070  mented by this p
-00000db0: 6c75 6769 6e2e 5c6e 5c6e 2323 2320 444d  lugin.\n\n### DM
-00000dc0: 3030 315c 6e5c 6e60 5265 6d6f 7665 4669  001\n\n`RemoveFi
-00000dd0: 656c 6460 206f 7065 7261 7469 6f6e 2073  eld` operation s
-00000de0: 686f 756c 6420 6265 2077 7261 7070 6564  hould be wrapped
-00000df0: 2069 6e20 6053 6570 6172 6174 6544 6174   in `SeparateDat
-00000e00: 6162 6173 6541 6e64 5374 6174 6560 2e5c  abaseAndState`.\
-00000e10: 6e5c 6e53 7563 6820 616e 206f 7065 7261  n\nSuch an opera
-00000e20: 7469 6f6e 2073 686f 756c 6420 6265 2072  tion should be r
-00000e30: 756e 2069 6e20 7477 6f20 7365 7061 7261  un in two separa
-00000e40: 7465 2073 7465 7073 2c20 7573 696e 6720  te steps, using 
-00000e50: 6053 6570 6172 6174 6544 6174 6162 6173  `SeparateDatabas
-00000e60: 6541 6e64 5374 6174 6560 2c20 6f74 6865  eAndState`, othe
-00000e70: 7277 6973 6520 6974 2069 7320 6e6f 7420  rwise it is not 
-00000e80: 6261 636b 7761 7264 7320 636f 6d70 6174  backwards compat
-00000e90: 6962 6c65 2e5c 6e5c 6e2d 2053 7465 7020  ible.\n\n- Step 
-00000ea0: 313a 2072 656d 6f76 6520 7468 6520 6669  1: remove the fi
-00000eb0: 656c 6420 6672 6f6d 2074 6865 206d 6f64  eld from the mod
-00000ec0: 656c 2061 6e64 2063 6f64 652e 2046 6f72  el and code. For
-00000ed0: 2066 6f72 6569 676e 206b 6579 2066 6965   foreign key fie
-00000ee0: 6c64 732c 2074 6865 2066 6f72 6569 676e  lds, the foreign
-00000ef0: 206b 6579 2063 6f6e 7374 7261 696e 7420   key constraint 
-00000f00: 7368 6f75 6c64 2061 6c73 6f20 6265 2064  should also be d
-00000f10: 726f 7070 6564 2e5c 6e2d 2053 7465 7020  ropped.\n- Step 
-00000f20: 323a 2072 656d 6f76 6520 7468 6520 636f  2: remove the co
-00000f30: 6c75 6d6e 2066 726f 6d20 7468 6520 6461  lumn from the da
-00000f40: 7461 6261 7365 2e5c 6e5c 6e23 2323 2320  tabase.\n\n#### 
-00000f50: 4261 645c 6e5c 6e60 6060 7079 7468 6f6e  Bad\n\n```python
-00000f60: 5c6e 636c 6173 7320 4d69 6772 6174 696f  \nclass Migratio
-00000f70: 6e28 6d69 6772 6174 696f 6e73 2e4d 6967  n(migrations.Mig
-00000f80: 7261 7469 6f6e 293a 5c6e 2020 2020 6f70  ration):\n    op
-00000f90: 6572 6174 696f 6e73 203d 205b 5c6e 2020  erations = [\n  
-00000fa0: 2020 2020 2020 6d69 6772 6174 696f 6e73        migrations
-00000fb0: 2e52 656d 6f76 6546 6965 6c64 285c 6e20  .RemoveField(\n 
-00000fc0: 2020 2020 2020 2020 2020 206d 6f64 656c             model
-00000fd0: 5f6e 616d 653d 226f 7264 6572 222c 5c6e  _name="order",\n
-00000fe0: 2020 2020 2020 2020 2020 2020 6e61 6d65              name
-00000ff0: 3d22 746f 7461 6c22 2c5c 6e20 2020 2020  ="total",\n     
-00001000: 2020 2029 2c5c 6e20 2020 205d 5c6e 6060     ),\n    ]\n``
-00001010: 605c 6e5c 6e23 2323 2320 476f 6f64 5c6e  `\n\n#### Good\n
-00001020: 5c6e 6060 6070 7974 686f 6e5c 6e63 6c61  \n```python\ncla
-00001030: 7373 204d 6967 7261 7469 6f6e 286d 6967  ss Migration(mig
-00001040: 7261 7469 6f6e 732e 4d69 6772 6174 696f  rations.Migratio
-00001050: 6e29 3a5c 6e20 2020 206f 7065 7261 7469  n):\n    operati
-00001060: 6f6e 7320 3d20 5b5c 6e20 2020 2020 2020  ons = [\n       
-00001070: 206d 6967 7261 7469 6f6e 732e 5365 7061   migrations.Sepa
-00001080: 7261 7465 4461 7461 6261 7365 416e 6453  rateDatabaseAndS
-00001090: 7461 7465 285c 6e20 2020 2020 2020 2020  tate(\n         
-000010a0: 2020 2073 7461 7465 5f6f 7065 7261 7469     state_operati
-000010b0: 6f6e 733d 5b5c 6e20 2020 2020 2020 2020  ons=[\n         
-000010c0: 2020 2020 2020 206d 6967 7261 7469 6f6e         migration
-000010d0: 732e 5265 6d6f 7665 4669 656c 6428 5c6e  s.RemoveField(\n
-000010e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000010f0: 2020 2020 6d6f 6465 6c5f 6e61 6d65 3d22      model_name="
-00001100: 6f72 6465 7222 2c5c 6e20 2020 2020 2020  order",\n       
-00001110: 2020 2020 2020 2020 2020 2020 206e 616d               nam
-00001120: 653d 2274 6f74 616c 222c 5c6e 2020 2020  e="total",\n    
-00001130: 2020 2020 2020 2020 2020 2020 292c 5c6e              ),\n
-00001140: 2020 2020 2020 2020 2020 2020 5d2c 5c6e              ],\n
-00001150: 2020 2020 2020 2020 292c 5c6e 2020 2020          ),\n    
-00001160: 5d5c 6e60 6060 5c6e 272c 0a20 2020 2027  ]\n```\n',.    '
-00001170: 6175 7468 6f72 273a 2027 4272 756e 6f20  author': 'Bruno 
-00001180: 416c 6c61 272c 0a20 2020 2027 6175 7468  Alla',.    'auth
-00001190: 6f72 5f65 6d61 696c 273a 2027 6272 756e  or_email': 'brun
-000011a0: 6f2e 616c 6c61 4066 6573 7469 636b 6574  o.alla@festicket
-000011b0: 2e63 6f6d 272c 0a20 2020 2027 6d61 696e  .com',.    'main
-000011c0: 7461 696e 6572 273a 2027 4e6f 6e65 272c  tainer': 'None',
-000011d0: 0a20 2020 2027 6d61 696e 7461 696e 6572  .    'maintainer
-000011e0: 5f65 6d61 696c 273a 2027 4e6f 6e65 272c  _email': 'None',
-000011f0: 0a20 2020 2027 7572 6c27 3a20 2768 7474  .    'url': 'htt
-00001200: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00001210: 6272 6f77 6e69 6562 726f 6b65 2f66 6c61  browniebroke/fla
-00001220: 6b65 382d 646a 616e 676f 2d6d 6967 7261  ke8-django-migra
-00001230: 7469 6f6e 7327 2c0a 2020 2020 2770 6163  tions',.    'pac
-00001240: 6b61 6765 5f64 6972 273a 2070 6163 6b61  kage_dir': packa
-00001250: 6765 5f64 6972 2c0a 2020 2020 2770 6163  ge_dir,.    'pac
-00001260: 6b61 6765 7327 3a20 7061 636b 6167 6573  kages': packages
-00001270: 2c0a 2020 2020 2770 6163 6b61 6765 5f64  ,.    'package_d
-00001280: 6174 6127 3a20 7061 636b 6167 655f 6461  ata': package_da
-00001290: 7461 2c0a 2020 2020 2769 6e73 7461 6c6c  ta,.    'install
-000012a0: 5f72 6571 7569 7265 7327 3a20 696e 7374  _requires': inst
-000012b0: 616c 6c5f 7265 7175 6972 6573 2c0a 2020  all_requires,.  
-000012c0: 2020 2765 7874 7261 735f 7265 7175 6972    'extras_requir
-000012d0: 6527 3a20 6578 7472 6173 5f72 6571 7569  e': extras_requi
-000012e0: 7265 2c0a 2020 2020 2765 6e74 7279 5f70  re,.    'entry_p
-000012f0: 6f69 6e74 7327 3a20 656e 7472 795f 706f  oints': entry_po
-00001300: 696e 7473 2c0a 2020 2020 2770 7974 686f  ints,.    'pytho
-00001310: 6e5f 7265 7175 6972 6573 273a 2027 3e3d  n_requires': '>=
-00001320: 332e 372c 3c34 2e30 272c 0a7d 0a0a 0a73  3.7,<4.0',.}...s
-00001330: 6574 7570 282a 2a73 6574 7570 5f6b 7761  etup(**setup_kwa
-00001340: 7267 7329 0a                             rgs).
+00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
+00000010: 3a20 322e 310a 4e61 6d65 3a20 666c 616b  : 2.1.Name: flak
+00000020: 6538 2d64 6a61 6e67 6f2d 6d69 6772 6174  e8-django-migrat
+00000030: 696f 6e73 0a56 6572 7369 6f6e 3a20 312e  ions.Version: 1.
+00000040: 302e 300a 5375 6d6d 6172 793a 2046 6c61  0.0.Summary: Fla
+00000050: 6b65 3820 706c 7567 696e 2074 6f20 6c69  ke8 plugin to li
+00000060: 6e74 2066 6f72 2062 6163 6b77 6172 6473  nt for backwards
+00000070: 2069 6e63 6f6d 7061 7469 626c 6520 6461   incompatible da
+00000080: 7461 6261 7365 206d 6967 7261 7469 6f6e  tabase migration
+00000090: 730a 486f 6d65 2d70 6167 653a 2068 7474  s.Home-page: htt
+000000a0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+000000b0: 6272 6f77 6e69 6562 726f 6b65 2f66 6c61  browniebroke/fla
+000000c0: 6b65 382d 646a 616e 676f 2d6d 6967 7261  ke8-django-migra
+000000d0: 7469 6f6e 730a 4c69 6365 6e73 653a 204d  tions.License: M
+000000e0: 4954 0a4b 6579 776f 7264 733a 2066 6c61  IT.Keywords: fla
+000000f0: 6b65 382c 6c69 6e74 2c64 6a61 6e67 6f2c  ke8,lint,django,
+00000100: 6d69 6772 6174 696f 6e73 0a41 7574 686f  migrations.Autho
+00000110: 723a 2042 7275 6e6f 2041 6c6c 610a 4175  r: Bruno Alla.Au
+00000120: 7468 6f72 2d65 6d61 696c 3a20 6272 756e  thor-email: brun
+00000130: 6f2e 616c 6c61 4066 6573 7469 636b 6574  o.alla@festicket
+00000140: 2e63 6f6d 0a52 6571 7569 7265 732d 5079  .com.Requires-Py
+00000150: 7468 6f6e 3a20 3e3d 332e 382c 3c34 2e30  thon: >=3.8,<4.0
+00000160: 0a43 6c61 7373 6966 6965 723a 2044 6576  .Classifier: Dev
+00000170: 656c 6f70 6d65 6e74 2053 7461 7475 7320  elopment Status 
+00000180: 3a3a 2031 202d 2050 6c61 6e6e 696e 670a  :: 1 - Planning.
+00000190: 436c 6173 7369 6669 6572 3a20 456e 7669  Classifier: Envi
+000001a0: 726f 6e6d 656e 7420 3a3a 2043 6f6e 736f  ronment :: Conso
+000001b0: 6c65 0a43 6c61 7373 6966 6965 723a 2046  le.Classifier: F
+000001c0: 7261 6d65 776f 726b 203a 3a20 466c 616b  ramework :: Flak
+000001d0: 6538 0a43 6c61 7373 6966 6965 723a 2049  e8.Classifier: I
+000001e0: 6e74 656e 6465 6420 4175 6469 656e 6365  ntended Audience
+000001f0: 203a 3a20 4465 7665 6c6f 7065 7273 0a43   :: Developers.C
+00000200: 6c61 7373 6966 6965 723a 204c 6963 656e  lassifier: Licen
+00000210: 7365 203a 3a20 4f53 4920 4170 7072 6f76  se :: OSI Approv
+00000220: 6564 203a 3a20 4d49 5420 4c69 6365 6e73  ed :: MIT Licens
+00000230: 650a 436c 6173 7369 6669 6572 3a20 4e61  e.Classifier: Na
+00000240: 7475 7261 6c20 4c61 6e67 7561 6765 203a  tural Language :
+00000250: 3a20 456e 676c 6973 680a 436c 6173 7369  : English.Classi
+00000260: 6669 6572 3a20 4f70 6572 6174 696e 6720  fier: Operating 
+00000270: 5379 7374 656d 203a 3a20 4f53 2049 6e64  System :: OS Ind
+00000280: 6570 656e 6465 6e74 0a43 6c61 7373 6966  ependent.Classif
+00000290: 6965 723a 2050 726f 6772 616d 6d69 6e67  ier: Programming
+000002a0: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
+000002b0: 686f 6e20 3a3a 2033 0a43 6c61 7373 6966  hon :: 3.Classif
+000002c0: 6965 723a 2050 726f 6772 616d 6d69 6e67  ier: Programming
+000002d0: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
+000002e0: 686f 6e20 3a3a 2033 2e38 0a43 6c61 7373  hon :: 3.8.Class
+000002f0: 6966 6965 723a 2050 726f 6772 616d 6d69  ifier: Programmi
+00000300: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
+00000310: 7974 686f 6e20 3a3a 2033 2e39 0a43 6c61  ython :: 3.9.Cla
+00000320: 7373 6966 6965 723a 2050 726f 6772 616d  ssifier: Program
+00000330: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
+00000340: 2050 7974 686f 6e20 3a3a 2033 2e31 300a   Python :: 3.10.
+00000350: 436c 6173 7369 6669 6572 3a20 5072 6f67  Classifier: Prog
+00000360: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
+00000370: 203a 3a20 5079 7468 6f6e 203a 3a20 332e   :: Python :: 3.
+00000380: 3131 0a43 6c61 7373 6966 6965 723a 2054  11.Classifier: T
+00000390: 6f70 6963 203a 3a20 536f 6674 7761 7265  opic :: Software
+000003a0: 2044 6576 656c 6f70 6d65 6e74 203a 3a20   Development :: 
+000003b0: 5175 616c 6974 7920 4173 7375 7261 6e63  Quality Assuranc
+000003c0: 650a 5265 7175 6972 6573 2d44 6973 743a  e.Requires-Dist:
+000003d0: 2061 7374 6f72 2028 3e3d 302e 3129 0a52   astor (>=0.1).R
+000003e0: 6571 7569 7265 732d 4469 7374 3a20 666c  equires-Dist: fl
+000003f0: 616b 6538 2028 3e3d 332e 3729 0a52 6571  ake8 (>=3.7).Req
+00000400: 7569 7265 732d 4469 7374 3a20 696d 706f  uires-Dist: impo
+00000410: 7274 6c69 622d 6d65 7461 6461 7461 2028  rtlib-metadata (
+00000420: 3e3d 302e 3929 203b 2070 7974 686f 6e5f  >=0.9) ; python_
+00000430: 7665 7273 696f 6e20 3c20 2233 2e38 220a  version < "3.8".
+00000440: 5072 6f6a 6563 742d 5552 4c3a 2052 6570  Project-URL: Rep
+00000450: 6f73 6974 6f72 792c 2068 7474 7073 3a2f  ository, https:/
+00000460: 2f67 6974 6875 622e 636f 6d2f 6272 6f77  /github.com/brow
+00000470: 6e69 6562 726f 6b65 2f66 6c61 6b65 382d  niebroke/flake8-
+00000480: 646a 616e 676f 2d6d 6967 7261 7469 6f6e  django-migration
+00000490: 730a 4465 7363 7269 7074 696f 6e2d 436f  s.Description-Co
+000004a0: 6e74 656e 742d 5479 7065 3a20 7465 7874  ntent-Type: text
+000004b0: 2f6d 6172 6b64 6f77 6e0a 0a23 2066 6c61  /markdown..# fla
+000004c0: 6b65 382d 646a 616e 676f 2d6d 6967 7261  ke8-django-migra
+000004d0: 7469 6f6e 730a 0a3c 7020 616c 6967 6e3d  tions..<p align=
+000004e0: 2263 656e 7465 7222 3e0a 2020 3c61 2068  "center">.  <a h
+000004f0: 7265 663d 2268 7474 7073 3a2f 2f67 6974  ref="https://git
+00000500: 6875 622e 636f 6d2f 6272 6f77 6e69 6562  hub.com/brownieb
+00000510: 726f 6b65 2f66 6c61 6b65 382d 646a 616e  roke/flake8-djan
+00000520: 676f 2d6d 6967 7261 7469 6f6e 732f 6163  go-migrations/ac
+00000530: 7469 6f6e 732f 776f 726b 666c 6f77 732f  tions/workflows/
+00000540: 6369 2e79 6d6c 3f71 7565 7279 3d62 7261  ci.yml?query=bra
+00000550: 6e63 6825 3341 6d61 696e 223e 0a20 2020  nch%3Amain">.   
+00000560: 203c 696d 6720 616c 743d 2243 4920 5374   <img alt="CI St
+00000570: 6174 7573 2220 7372 633d 2268 7474 7073  atus" src="https
+00000580: 3a2f 2f69 6d67 2e73 6869 656c 6473 2e69  ://img.shields.i
+00000590: 6f2f 6769 7468 7562 2f61 6374 696f 6e73  o/github/actions
+000005a0: 2f77 6f72 6b66 6c6f 772f 7374 6174 7573  /workflow/status
+000005b0: 2f62 726f 776e 6965 6272 6f6b 652f 666c  /browniebroke/fl
+000005c0: 616b 6538 2d64 6a61 6e67 6f2d 6d69 6772  ake8-django-migr
+000005d0: 6174 696f 6e73 2f63 692e 796d 6c3f 6272  ations/ci.yml?br
+000005e0: 616e 6368 3d6d 6169 6e26 6c61 6265 6c3d  anch=main&label=
+000005f0: 4349 266c 6f67 6f3d 6769 7468 7562 2673  CI&logo=github&s
+00000600: 7479 6c65 3d66 6c61 742d 7371 7561 7265  tyle=flat-square
+00000610: 223e 0a20 203c 2f61 3e0a 2020 3c61 2068  ">.  </a>.  <a h
+00000620: 7265 663d 2268 7474 7073 3a2f 2f63 6f64  ref="https://cod
+00000630: 6563 6f76 2e69 6f2f 6768 2f62 726f 776e  ecov.io/gh/brown
+00000640: 6965 6272 6f6b 652f 666c 616b 6538 2d64  iebroke/flake8-d
+00000650: 6a61 6e67 6f2d 6d69 6772 6174 696f 6e73  jango-migrations
+00000660: 223e 0a20 2020 203c 696d 6720 7372 633d  ">.    <img src=
+00000670: 2268 7474 7073 3a2f 2f69 6d67 2e73 6869  "https://img.shi
+00000680: 656c 6473 2e69 6f2f 636f 6465 636f 762f  elds.io/codecov/
+00000690: 632f 6769 7468 7562 2f62 726f 776e 6965  c/github/brownie
+000006a0: 6272 6f6b 652f 666c 616b 6538 2d64 6a61  broke/flake8-dja
+000006b0: 6e67 6f2d 6d69 6772 6174 696f 6e73 2e73  ngo-migrations.s
+000006c0: 7667 3f6c 6f67 6f3d 636f 6465 636f 7626  vg?logo=codecov&
+000006d0: 7374 796c 653d 666c 6174 2d73 7175 6172  style=flat-squar
+000006e0: 6522 2061 6c74 3d22 5465 7374 2063 6f76  e" alt="Test cov
+000006f0: 6572 6167 6520 7065 7263 656e 7461 6765  erage percentage
+00000700: 223e 0a20 203c 2f61 3e0a 3c2f 703e 0a3c  ">.  </a>.</p>.<
+00000710: 7020 616c 6967 6e3d 2263 656e 7465 7222  p align="center"
+00000720: 3e0a 2020 3c61 2068 7265 663d 2268 7474  >.  <a href="htt
+00000730: 7073 3a2f 2f70 7974 686f 6e2d 706f 6574  ps://python-poet
+00000740: 7279 2e6f 7267 2f22 3e0a 2020 2020 3c69  ry.org/">.    <i
+00000750: 6d67 2073 7263 3d22 6874 7470 733a 2f2f  mg src="https://
+00000760: 696d 672e 7368 6965 6c64 732e 696f 2f62  img.shields.io/b
+00000770: 6164 6765 2f70 6163 6b61 6769 6e67 2d70  adge/packaging-p
+00000780: 6f65 7472 792d 3239 3962 6437 3f73 7479  oetry-299bd7?sty
+00000790: 6c65 3d66 6c61 742d 7371 7561 7265 266c  le=flat-square&l
+000007a0: 6f67 6f3d 6461 7461 3a69 6d61 6765 2f70  ogo=data:image/p
+000007b0: 6e67 3b62 6173 6536 342c 6956 424f 5277  ng;base64,iVBORw
+000007c0: 304b 4767 6f41 4141 414e 5355 6845 5567  0KGgoAAAANSUhEUg
+000007d0: 4141 4141 3441 4141 4153 4341 5941 4141  AAAA4AAAASCAYAAA
+000007e0: 4272 584f 3878 4141 4141 4358 4249 5758  BrXO8xAAAACXBIWX
+000007f0: 4d41 4141 7354 4141 414c 4577 4541 6d70  MAAAsTAAALEwEAmp
+00000800: 7759 4141 4141 4158 4e53 5230 4941 7273  wYAAAAAXNSR0IArs
+00000810: 3463 3651 4141 4141 526e 5155 3142 4141  4c6QAAAARnQU1BAA
+00000820: 4378 6a77 7638 5951 5541 4141 4a4a 5355  Cxjwv8YQUAAAJJSU
+00000830: 5242 5648 6742 665a 4c50 6131 4e42 454d  RBVHgBfZLPa1NBEM
+00000840: 652f 7337 744e 586f 7857 314b 4a51 4b61  e/s7tNXoxW1KJQKa
+00000850: 5548 6b58 6851 7648 6757 3655 4851 5130  UHkXhQvHgW6UHQQ0
+00000860: 3943 4253 2f36 5633 684b 632f 4150 3843  9CBS/6V3hKc/AP8C
+00000870: 7143 7255 6370 6d6f 7033 4378 3438 6544  qCrUcpmop3Cx48eD
+00000880: 4234 7945 4543 6a56 5172 6c5a 6238 3043  B4yEECjVQrlZb80C
+00000890: 524e 3874 364f 4d2f 7465 6167 5678 595a  RN8t6OM/teagVxYZ
+000008a0: 6933 382b 597a 3835 3364 4a62 7a6f 4d56  i38+Yz853dJbzoMV
+000008b0: 334d 4d38 634a 5563 4c4d 5355 4b49 4538  3MM8cJUcLMSUKIE8
+000008c0: 417a 5132 5069 655a 7a46 7845 4a4f 484d  AzQ2PieZzFxEJOHM
+000008d0: 4f67 4d51 512b 6455 6753 4163 6b4e 5868  OgMQQ+dUgSAckNXh
+000008e0: 6170 552f 4e4d 6844 5357 4c73 3142 3234  apU/NMhDSWLs1B24
+000008f0: 4138 734f 3178 724e 344e 4543 6b63 4143  A8sO1xrN4NECkcAC
+00000900: 3941 536b 6949 4a63 366b 3554 5269 5544  9ASkiIJc6k5TRiUD
+00000910: 5068 6e79 4d4d 6468 4b63 2b5a 7831 396c  PhnyMMdhKc+Zx19l
+00000920: 3653 6779 6557 3736 4245 4f4e 5939 6578  6SgyeW76BEONY9ex
+00000930: 5651 4d7a 4b45 7847 4b77 7750 7343 7a7a  VQMzKExGKwwPsCzz
+00000940: 6137 4b47 5353 5752 5745 5168 7945 6144  a7KGSSWRWEQhyEaD
+00000950: 5870 365a 4845 7234 3136 7967 6269 4b59  Xp6ZHEr416ygbiKY
+00000960: 4f64 3754 4557 7676 6351 4965 7573 4859  Od7TEWvvcQIeusHY
+00000970: 4d4a 4768 5477 4639 7937 7347 6e53 7761  MJGhTwF9y7sGnSwa
+00000980: 5779 4641 6979 6f78 7a71 5730 504d 2f52  WyFAiyoxzqW0PM/R
+00000990: 6a67 6850 7846 3270 5752 6541 6f77 5445  jghPxF2pWReAowTE
+000009a0: 586e 4468 3078 6763 4c73 386c 3259 516d  XnDh0xgcLs8l2YQm
+000009b0: 4f72 6a33 4e37 4279 6971 456f 4830 6341  Orj3N7ByiqEoH0cA
+000009c0: 5273 3475 3738 5767 4156 6b6f 4544 4944  Rs4u78WgAVkoEDID
+000009d0: 6f4f 6933 416b 634c 4f48 5536 3052 4967  oOi3AkcLOHU60RIg
+000009e0: 3577 4334 5a75 5443 3746 6148 4b51 6d38  5wC4ZuTC7FaHKQm8
+000009f0: 4871 3166 5175 534f 4276 582f 736f 646d  Hq1fQuSOBvX/sodm
+00000a00: 4e4a 5342 3567 6561 4635 4350 496b 5565  NJSB5geaF5CPIkUe
+00000a10: 6563 644d 7869 656f 524f 356a 7a39 6268  ecdMxieoRO5jz9bh
+00000a20: 654c 362f 7458 6a72 7743 7958 2f55 5942  eL6/tXjrwCyX/UYB
+00000a30: 5563 6a43 6157 486c 6a78 3178 6958 367a  UcjCaWHljx1xiX6z
+00000a40: 3978 456a 6b59 417a 6247 566e 4238 7076  9xEjkYAzbGVnB8pv
+00000a50: 4c6d 7958 6d39 6570 2b57 3843 6d73 5348  LmyXm9ep+W8CmsSH
+00000a60: 5151 5937 375a 7831 7a62 6f78 4156 3077  QQY77Zx1zboxAV0w
+00000a70: 3779 624d 6851 6d66 7164 6d6d 7733 6e45  7ybMhQmfqdmmw3nE
+00000a80: 7031 4930 5a2b 4647 4f36 4d38 4c5a 646f  p1I0Z+FGO6M8LZdo
+00000a90: 795a 6e75 7a7a 4264 6a49 5369 634b 526e  yZnuzzBdjISicKRn
+00000aa0: 7078 7a49 3966 5062 2b30 6f59 5873 4e64  pxzI9fPb+0oYXsNd
+00000ab0: 7969 2b64 3368 3962 6d39 4d57 5948 4674  yi+d3h9bm9MWYHFt
+00000ac0: 5065 495a 664c 777a 6d46 444b 7931 6169  PeIZfLwzmFDKy1ai
+00000ad0: 3370 2b50 446c 7331 4c6c 7a34 7979 4670  3p+PDls1Llz4yyFp
+00000ae0: 6665 7278 6a6e 796a 4a44 5345 7939 4361  ferxjnyjJDSEy9Ca
+00000af0: 4378 356d 3263 4a50 6572 7136 586d 3334  Cx5m2cJPerq6Xm34
+00000b00: 6554 725a 7433 5071 7859 4f31 584f 7744  eTrZt3PqxYO1XOwD
+00000b10: 595a 7246 6c48 3166 576e 7055 3338 5939  YZrFlH1fWnpU38Y9
+00000b20: 4852 7a65 336c 6a30 764f 756a 5a63 584b  HRze3lj0vOujZcXK
+00000b30: 7575 586d 336a 502b 7333 4b62 5a56 7261  uuXm3jP+s3KbZVra
+00000b40: 3779 3245 4141 4141 4141 5355 564f 524b  7y2EAAAAAASUVORK
+00000b50: 3543 5949 493d 2220 616c 743d 2250 6f65  5CYII=" alt="Poe
+00000b60: 7472 7922 3e0a 2020 3c2f 613e 0a20 203c  try">.  </a>.  <
+00000b70: 6120 6872 6566 3d22 6874 7470 733a 2f2f  a href="https://
+00000b80: 6769 7468 7562 2e63 6f6d 2f61 6d62 762f  github.com/ambv/
+00000b90: 626c 6163 6b22 3e0a 2020 2020 3c69 6d67  black">.    <img
+00000ba0: 2073 7263 3d22 6874 7470 733a 2f2f 696d   src="https://im
+00000bb0: 672e 7368 6965 6c64 732e 696f 2f62 6164  g.shields.io/bad
+00000bc0: 6765 2f63 6f64 6525 3230 7374 796c 652d  ge/code%20style-
+00000bd0: 626c 6163 6b2d 3030 3030 3030 2e73 7667  black-000000.svg
+00000be0: 3f73 7479 6c65 3d66 6c61 742d 7371 7561  ?style=flat-squa
+00000bf0: 7265 2220 616c 743d 2262 6c61 636b 223e  re" alt="black">
+00000c00: 0a20 203c 2f61 3e0a 2020 3c61 2068 7265  .  </a>.  <a hre
+00000c10: 663d 2268 7474 7073 3a2f 2f67 6974 6875  f="https://githu
+00000c20: 622e 636f 6d2f 7072 652d 636f 6d6d 6974  b.com/pre-commit
+00000c30: 2f70 7265 2d63 6f6d 6d69 7422 3e0a 2020  /pre-commit">.  
+00000c40: 2020 3c69 6d67 2073 7263 3d22 6874 7470    <img src="http
+00000c50: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
+00000c60: 696f 2f62 6164 6765 2f70 7265 2d2d 636f  io/badge/pre--co
+00000c70: 6d6d 6974 2d65 6e61 626c 6564 2d62 7269  mmit-enabled-bri
+00000c80: 6768 7467 7265 656e 3f6c 6f67 6f3d 7072  ghtgreen?logo=pr
+00000c90: 652d 636f 6d6d 6974 266c 6f67 6f43 6f6c  e-commit&logoCol
+00000ca0: 6f72 3d77 6869 7465 2673 7479 6c65 3d66  or=white&style=f
+00000cb0: 6c61 742d 7371 7561 7265 2220 616c 743d  lat-square" alt=
+00000cc0: 2270 7265 2d63 6f6d 6d69 7422 3e0a 2020  "pre-commit">.  
+00000cd0: 3c2f 613e 0a3c 2f70 3e0a 3c70 2061 6c69  </a>.</p>.<p ali
+00000ce0: 676e 3d22 6365 6e74 6572 223e 0a20 203c  gn="center">.  <
+00000cf0: 6120 6872 6566 3d22 6874 7470 733a 2f2f  a href="https://
+00000d00: 7079 7069 2e6f 7267 2f70 726f 6a65 6374  pypi.org/project
+00000d10: 2f66 6c61 6b65 382d 646a 616e 676f 2d6d  /flake8-django-m
+00000d20: 6967 7261 7469 6f6e 732f 223e 0a20 2020  igrations/">.   
+00000d30: 203c 696d 6720 7372 633d 2268 7474 7073   <img src="https
+00000d40: 3a2f 2f69 6d67 2e73 6869 656c 6473 2e69  ://img.shields.i
+00000d50: 6f2f 7079 7069 2f76 2f66 6c61 6b65 382d  o/pypi/v/flake8-
+00000d60: 646a 616e 676f 2d6d 6967 7261 7469 6f6e  django-migration
+00000d70: 732e 7376 673f 6c6f 676f 3d70 7974 686f  s.svg?logo=pytho
+00000d80: 6e26 616d 703b 6c6f 676f 436f 6c6f 723d  n&amp;logoColor=
+00000d90: 6666 6626 616d 703b 7374 796c 653d 666c  fff&amp;style=fl
+00000da0: 6174 2d73 7175 6172 6522 2061 6c74 3d22  at-square" alt="
+00000db0: 5079 5069 2053 7461 7475 7322 3e0a 2020  PyPi Status">.  
+00000dc0: 3c2f 613e 0a20 203c 696d 6720 7372 633d  </a>.  <img src=
+00000dd0: 2268 7474 7073 3a2f 2f69 6d67 2e73 6869  "https://img.shi
+00000de0: 656c 6473 2e69 6f2f 7079 7069 2f70 7976  elds.io/pypi/pyv
+00000df0: 6572 7369 6f6e 732f 666c 616b 6538 2d64  ersions/flake8-d
+00000e00: 6a61 6e67 6f2d 6d69 6772 6174 696f 6e73  jango-migrations
+00000e10: 2e73 7667 3f73 7479 6c65 3d66 6c61 742d  .svg?style=flat-
+00000e20: 7371 7561 7265 2220 616c 743d 2270 7976  square" alt="pyv
+00000e30: 6572 7369 6f6e 7322 3e0a 2020 3c69 6d67  ersions">.  <img
+00000e40: 2073 7263 3d22 6874 7470 733a 2f2f 696d   src="https://im
+00000e50: 672e 7368 6965 6c64 732e 696f 2f70 7970  g.shields.io/pyp
+00000e60: 692f 6c2f 666c 616b 6538 2d64 6a61 6e67  i/l/flake8-djang
+00000e70: 6f2d 6d69 6772 6174 696f 6e73 2e73 7667  o-migrations.svg
+00000e80: 3f73 7479 6c65 3d66 6c61 742d 7371 7561  ?style=flat-squa
+00000e90: 7265 2220 616c 743d 226c 6963 656e 7365  re" alt="license
+00000ea0: 223e 0a3c 2f70 3e0a 0a46 6c61 6b65 3820  ">.</p>..Flake8 
+00000eb0: 706c 7567 696e 2074 6f20 6c69 6e74 2066  plugin to lint f
+00000ec0: 6f72 2062 6163 6b77 6172 6473 2069 6e63  or backwards inc
+00000ed0: 6f6d 7061 7469 626c 6520 6461 7461 6261  ompatible databa
+00000ee0: 7365 206d 6967 7261 7469 6f6e 732e 0a0a  se migrations...
+00000ef0: 2323 2049 6e73 7461 6c6c 6174 696f 6e0a  ## Installation.
+00000f00: 0a49 6e73 7461 6c6c 2075 7369 6e67 2060  .Install using `
+00000f10: 7069 7060 2028 6f72 2079 6f75 7220 6661  pip` (or your fa
+00000f20: 766f 7572 6974 6520 7061 636b 6167 6520  vourite package 
+00000f30: 6d61 6e61 6765 7229 3a0a 0a60 6060 7368  manager):..```sh
+00000f40: 0a70 6970 2069 6e73 7461 6c6c 2066 6c61  .pip install fla
+00000f50: 6b65 382d 646a 616e 676f 2d6d 6967 7261  ke8-django-migra
+00000f60: 7469 6f6e 730a 6060 600a 0a23 2320 5573  tions.```..## Us
+00000f70: 6167 650a 0a54 6869 7320 706c 7567 696e  age..This plugin
+00000f80: 2073 686f 756c 6420 6265 2075 7365 6420   should be used 
+00000f90: 6175 746f 6d61 7469 6361 6c6c 7920 7768  automatically wh
+00000fa0: 656e 2072 756e 6e69 6e67 2066 6c61 6b65  en running flake
+00000fb0: 383a 0a0a 6060 6073 680a 666c 616b 6538  8:..```sh.flake8
+00000fc0: 0a60 6060 0a0a 2323 2043 6865 636b 730a  .```..## Checks.
+00000fd0: 0a54 6869 7320 6973 2074 6865 206c 6973  .This is the lis
+00000fe0: 7420 6f66 2063 6865 636b 7320 6375 7272  t of checks curr
+00000ff0: 656e 746c 7920 696d 706c 656d 656e 7465  ently implemente
+00001000: 6420 6279 2074 6869 7320 706c 7567 696e  d by this plugin
+00001010: 2e0a 0a23 2323 2044 4d30 3031 0a0a 6052  ...### DM001..`R
+00001020: 656d 6f76 6546 6965 6c64 6020 6f70 6572  emoveField` oper
+00001030: 6174 696f 6e20 7368 6f75 6c64 2062 6520  ation should be 
+00001040: 7772 6170 7065 6420 696e 2060 5365 7061  wrapped in `Sepa
+00001050: 7261 7465 4461 7461 6261 7365 416e 6453  rateDatabaseAndS
+00001060: 7461 7465 602e 0a0a 5375 6368 2061 6e20  tate`...Such an 
+00001070: 6f70 6572 6174 696f 6e20 7368 6f75 6c64  operation should
+00001080: 2062 6520 7275 6e20 696e 2074 776f 2073   be run in two s
+00001090: 6570 6172 6174 6520 7374 6570 732c 2075  eparate steps, u
+000010a0: 7369 6e67 2060 5365 7061 7261 7465 4461  sing `SeparateDa
+000010b0: 7461 6261 7365 416e 6453 7461 7465 602c  tabaseAndState`,
+000010c0: 206f 7468 6572 7769 7365 2069 7420 6973   otherwise it is
+000010d0: 206e 6f74 2062 6163 6b77 6172 6473 2063   not backwards c
+000010e0: 6f6d 7061 7469 626c 652e 0a0a 2d20 5374  ompatible...- St
+000010f0: 6570 2031 3a20 7265 6d6f 7665 2074 6865  ep 1: remove the
+00001100: 2066 6965 6c64 2066 726f 6d20 7468 6520   field from the 
+00001110: 6d6f 6465 6c20 616e 6420 636f 6465 2e20  model and code. 
+00001120: 466f 7220 666f 7265 6967 6e20 6b65 7920  For foreign key 
+00001130: 6669 656c 6473 2c20 7468 6520 666f 7265  fields, the fore
+00001140: 6967 6e20 6b65 7920 636f 6e73 7472 6169  ign key constrai
+00001150: 6e74 2073 686f 756c 6420 616c 736f 2062  nt should also b
+00001160: 6520 6472 6f70 7065 642e 0a2d 2053 7465  e dropped..- Ste
+00001170: 7020 323a 2072 656d 6f76 6520 7468 6520  p 2: remove the 
+00001180: 636f 6c75 6d6e 2066 726f 6d20 7468 6520  column from the 
+00001190: 6461 7461 6261 7365 2e0a 0a23 2323 2320  database...#### 
+000011a0: 4261 640a 0a60 6060 7079 7468 6f6e 0a63  Bad..```python.c
+000011b0: 6c61 7373 204d 6967 7261 7469 6f6e 286d  lass Migration(m
+000011c0: 6967 7261 7469 6f6e 732e 4d69 6772 6174  igrations.Migrat
+000011d0: 696f 6e29 3a0a 2020 2020 6f70 6572 6174  ion):.    operat
+000011e0: 696f 6e73 203d 205b 0a20 2020 2020 2020  ions = [.       
+000011f0: 206d 6967 7261 7469 6f6e 732e 5265 6d6f   migrations.Remo
+00001200: 7665 4669 656c 6428 0a20 2020 2020 2020  veField(.       
+00001210: 2020 2020 206d 6f64 656c 5f6e 616d 653d       model_name=
+00001220: 226f 7264 6572 222c 0a20 2020 2020 2020  "order",.       
+00001230: 2020 2020 206e 616d 653d 2274 6f74 616c       name="total
+00001240: 222c 0a20 2020 2020 2020 2029 2c0a 2020  ",.        ),.  
+00001250: 2020 5d0a 6060 600a 0a23 2323 2320 476f    ].```..#### Go
+00001260: 6f64 0a0a 6060 6070 7974 686f 6e0a 636c  od..```python.cl
+00001270: 6173 7320 4d69 6772 6174 696f 6e28 6d69  ass Migration(mi
+00001280: 6772 6174 696f 6e73 2e4d 6967 7261 7469  grations.Migrati
+00001290: 6f6e 293a 0a20 2020 206f 7065 7261 7469  on):.    operati
+000012a0: 6f6e 7320 3d20 5b0a 2020 2020 2020 2020  ons = [.        
+000012b0: 6d69 6772 6174 696f 6e73 2e53 6570 6172  migrations.Separ
+000012c0: 6174 6544 6174 6162 6173 6541 6e64 5374  ateDatabaseAndSt
+000012d0: 6174 6528 0a20 2020 2020 2020 2020 2020  ate(.           
+000012e0: 2073 7461 7465 5f6f 7065 7261 7469 6f6e   state_operation
+000012f0: 733d 5b0a 2020 2020 2020 2020 2020 2020  s=[.            
+00001300: 2020 2020 6d69 6772 6174 696f 6e73 2e52      migrations.R
+00001310: 656d 6f76 6546 6965 6c64 280a 2020 2020  emoveField(.    
+00001320: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001330: 6d6f 6465 6c5f 6e61 6d65 3d22 6f72 6465  model_name="orde
+00001340: 7222 2c0a 2020 2020 2020 2020 2020 2020  r",.            
+00001350: 2020 2020 2020 2020 6e61 6d65 3d22 746f          name="to
+00001360: 7461 6c22 2c0a 2020 2020 2020 2020 2020  tal",.          
+00001370: 2020 2020 2020 292c 0a20 2020 2020 2020        ),.       
+00001380: 2020 2020 205d 2c0a 2020 2020 2020 2020       ],.        
+00001390: 292c 0a20 2020 205d 0a60 6060 0a0a       ),.    ].```..
```

