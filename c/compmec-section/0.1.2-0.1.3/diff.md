# Comparing `tmp/compmec_section-0.1.2.tar.gz` & `tmp/compmec_section-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "compmec_section-0.1.2.tar", max compression
+gzip compressed data, was "compmec_section-0.1.3.tar", max compression
```

## Comparing `compmec_section-0.1.2.tar` & `compmec_section-0.1.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1079 2023-06-26 09:35:56.600163 compmec_section-0.1.2/LICENSE.md
--rw-r--r--   0        0        0      680 2023-06-26 18:11:41.074743 compmec_section-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     1778 2023-06-26 18:11:41.075736 compmec_section-0.1.2/README.md
--rw-r--r--   0        0        0      295 2023-06-26 17:14:35.445886 compmec_section-0.1.2/src/compmec/section/__init__.py
--rw-r--r--   0        0        0     3049 2023-06-26 18:11:41.076737 compmec_section-0.1.2/src/compmec/section/material.py
--rw-r--r--   0        0        0        0 2023-06-26 17:14:35.431349 compmec_section-0.1.2/src/compmec/section/profile.py
--rw-r--r--   0        0        0     5339 2023-06-26 17:14:35.453481 compmec_section-0.1.2/src/compmec/section/shape.py
--rw-r--r--   0        0        0     2339 1970-01-01 00:00:00.000000 compmec_section-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1079 2023-06-27 14:32:41.371667 compmec_section-0.1.3/LICENSE.md
+-rw-r--r--   0        0        0     2183 2023-06-27 14:32:41.371667 compmec_section-0.1.3/README.md
+-rw-r--r--   0        0        0      680 2023-06-27 14:32:41.371667 compmec_section-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      287 2023-06-27 14:32:41.371667 compmec_section-0.1.3/src/compmec/section/__init__.py
+-rw-r--r--   0        0        0     2957 2023-06-27 14:32:41.371667 compmec_section-0.1.3/src/compmec/section/material.py
+-rw-r--r--   0        0        0        0 2023-06-27 14:32:41.371667 compmec_section-0.1.3/src/compmec/section/profile.py
+-rw-r--r--   0        0        0     6663 2023-06-27 14:32:41.371667 compmec_section-0.1.3/src/compmec/section/shape.py
+-rw-r--r--   0        0        0     2785 1970-01-01 00:00:00.000000 compmec_section-0.1.3/PKG-INFO
```

### Comparing `compmec_section-0.1.2/LICENSE.md` & `compmec_section-0.1.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `compmec_section-0.1.2/pyproject.toml` & `compmec_section-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "compmec-section"
-version = "0.1.2"
+version = "0.1.3"
 description = "Compute characteristics of an arbitrary cross-section in python"
 authors = ["Carlos Adir <carlos.adir.leite@gmail.com>"]
 readme = "README.md"
 packages = [{ include = "compmec/section", from = "src" }]
 
 [tool.poetry.dependencies]
 numpy = "^1.0.0"
```

### Comparing `compmec_section-0.1.2/README.md` & `compmec_section-0.1.3/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,112 +1,137 @@
-00000000: 5b21 5b50 7950 4920 5665 7273 696f 6e5d  [![PyPI Version]
-00000010: 5b70 7970 692d 696d 6167 655d 5d5b 7079  [pypi-image]][py
-00000020: 7069 2d75 726c 5d0d 0a5b 215b 4275 696c  pi-url]..[![Buil
-00000030: 6420 5374 6174 7573 5d5b 6275 696c 642d  d Status][build-
-00000040: 696d 6167 655d 5d5b 6275 696c 642d 7572  image]][build-ur
-00000050: 6c5d 0d0a 5b21 5b43 6f64 6520 436f 7665  l]..[![Code Cove
-00000060: 7261 6765 5d5b 636f 7665 7261 6765 2d69  rage][coverage-i
-00000070: 6d61 6765 5d5d 5b63 6f76 6572 6167 652d  mage]][coverage-
-00000080: 7572 6c5d 0d0a 5b21 5b5d 5b76 6572 7369  url]..[![][versi
-00000090: 6f6e 732d 696d 6167 655d 5d5b 7665 7273  ons-image]][vers
-000000a0: 696f 6e73 2d75 726c 5d0d 0a3c 6120 6872  ions-url]..<a hr
-000000b0: 6566 3d22 6874 7470 733a 2f2f 6769 7468  ef="https://gith
-000000c0: 7562 2e63 6f6d 2f63 6f6d 706d 6563 2f73  ub.com/compmec/s
-000000d0: 6563 7469 6f6e 2d70 726f 7065 7274 6965  ection-propertie
-000000e0: 7322 3e3c 696d 6720 616c 743d 2243 6f64  s"><img alt="Cod
-000000f0: 6520 7374 796c 653a 2062 6c61 636b 2220  e style: black" 
-00000100: 7372 633d 2268 7474 7073 3a2f 2f69 6d67  src="https://img
-00000110: 2e73 6869 656c 6473 2e69 6f2f 6261 6467  .shields.io/badg
-00000120: 652f 636f 6465 2532 3073 7479 6c65 2d62  e/code%20style-b
-00000130: 6c61 636b 2d30 3030 3030 302e 7376 6722  lack-000000.svg"
-00000140: 3e3c 2f61 3e0d 0a3c 6120 6872 6566 3d22  ></a>..<a href="
-00000150: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00000160: 6f6d 2f63 6f6d 706d 6563 2f73 6563 7469  om/compmec/secti
-00000170: 6f6e 2d70 726f 7065 7274 6965 732f 626c  on-properties/bl
-00000180: 6f62 2f6d 6169 6e2f 4c49 4345 4e53 452e  ob/main/LICENSE.
-00000190: 6d64 223e 3c69 6d67 2061 6c74 3d22 4c69  md"><img alt="Li
-000001a0: 6365 6e73 653a 204d 4954 2220 7372 633d  cense: MIT" src=
-000001b0: 2268 7474 7073 3a2f 2f62 6c61 636b 2e72  "https://black.r
-000001c0: 6561 6474 6865 646f 6373 2e69 6f2f 656e  eadthedocs.io/en
-000001d0: 2f73 7461 626c 652f 5f73 7461 7469 632f  /stable/_static/
-000001e0: 6c69 6365 6e73 652e 7376 6722 3e3c 2f61  license.svg"></a
-000001f0: 3e0d 0a0d 0a0d 0a41 2070 7974 686f 6e20  >......A python 
-00000200: 7061 636b 6167 6520 666f 7220 616e 616c  package for anal
-00000210: 7973 6973 206f 6620 6172 6269 7472 6172  ysis of arbitrar
-00000220: 7920 6265 616d 2063 726f 7373 2073 6563  y beam cross sec
-00000230: 7469 6f6e 2075 7369 6e67 2062 6f75 6e64  tion using bound
-00000240: 6172 7920 656c 656d 656e 7420 6d65 7468  ary element meth
-00000250: 6f64 2e0d 0a0d 0a54 6869 7320 7061 636b  od.....This pack
-00000260: 6167 6520 6361 6e20 6265 2075 7365 6420  age can be used 
-00000270: 696e 2073 7472 7563 7475 7261 6c20 6465  in structural de
-00000280: 7369 676e 2061 6e64 2076 6973 7561 6c69  sign and visuali
-00000290: 7365 2064 6566 6f72 6d65 6420 7072 6f66  se deformed prof
-000002a0: 696c 652c 2073 7472 6573 7320 6475 6520  ile, stress due 
-000002b0: 746f 2061 7070 6c69 6564 2066 6f72 6365  to applied force
-000002c0: 7320 616e 6420 6d6f 6d65 6e74 756d 730d  s and momentums.
-000002d0: 0a0d 0a23 2323 2049 6e73 7461 6c6c 6174  ...### Installat
-000002e0: 696f 6e3a 0d0a 0d0a 5468 6973 206c 6962  ion:....This lib
-000002f0: 7261 7279 2069 7320 6176 6169 6c61 626c  rary is availabl
-00000300: 6520 696e 205b 5079 5049 5d5b 7079 7069  e in [PyPI][pypi
-00000310: 6c69 6e6b 5d2e 2054 6f20 696e 7374 616c  link]. To instal
-00000320: 6c20 6974 0d0a 0d0a 6060 600d 0a24 2070  l it....```..$ p
-00000330: 6970 2069 6e73 7461 6c6c 2063 6f6d 706d  ip install compm
-00000340: 6563 2d73 6563 7469 6f6e 0d0a 6060 600d  ec-section..```.
-00000350: 0a0d 0a23 2323 2044 6f63 756d 656e 7461  ...### Documenta
-00000360: 7469 6f6e 0d0a 0d0a 496e 2070 726f 6772  tion....In progr
-00000370: 6573 730d 0a0d 0a0d 0a23 2323 2043 6f6e  ess......### Con
-00000380: 7472 6962 7574 650d 0a0d 0a50 6c65 6173  tribute....Pleas
-00000390: 6520 7573 6520 7468 6520 5b49 7373 7565  e use the [Issue
-000003a0: 735d 5b69 7373 7565 736c 696e 6b5d 206f  s][issueslink] o
-000003b0: 7220 7265 6665 7220 746f 2074 6865 2065  r refer to the e
-000003c0: 6d61 696c 2060 6060 636f 6d70 6d65 6367  mail ```compmecg
-000003d0: 6974 4067 6d61 696c 2e63 6f6d 6060 600d  it@gmail.com```.
-000003e0: 0a0d 0a3c 212d 2d20 4261 6467 6573 3a20  ...<!-- Badges: 
-000003f0: 2d2d 3e0d 0a0d 0a5b 7079 7069 2d69 6d61  -->....[pypi-ima
-00000400: 6765 5d3a 2068 7474 7073 3a2f 2f69 6d67  ge]: https://img
-00000410: 2e73 6869 656c 6473 2e69 6f2f 7079 7069  .shields.io/pypi
-00000420: 2f76 2f63 6f6d 706d 6563 2d73 6563 7469  /v/compmec-secti
-00000430: 6f6e 0d0a 5b70 7970 692d 7572 6c5d 3a20  on..[pypi-url]: 
-00000440: 6874 7470 733a 2f2f 7079 7069 2e6f 7267  https://pypi.org
-00000450: 2f70 726f 6a65 6374 2f63 6f6d 706d 6563  /project/compmec
-00000460: 2d73 6563 7469 6f6e 2f0d 0a5b 6275 696c  -section/..[buil
-00000470: 642d 696d 6167 655d 3a20 6874 7470 733a  d-image]: https:
-00000480: 2f2f 6769 7468 7562 2e63 6f6d 2f63 6f6d  //github.com/com
-00000490: 706d 6563 2f73 6563 7469 6f6e 2d70 726f  pmec/section-pro
-000004a0: 7065 7274 6965 732f 6163 7469 6f6e 732f  perties/actions/
-000004b0: 776f 726b 666c 6f77 732f 6275 696c 642e  workflows/build.
-000004c0: 7961 6d6c 2f62 6164 6765 2e73 7667 0d0a  yaml/badge.svg..
-000004d0: 5b62 7569 6c64 2d75 726c 5d3a 2068 7474  [build-url]: htt
-000004e0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-000004f0: 636f 6d70 6d65 632f 7365 6374 696f 6e2d  compmec/section-
-00000500: 7072 6f70 6572 7469 6573 2f61 6374 696f  properties/actio
-00000510: 6e73 2f77 6f72 6b66 6c6f 7773 2f62 7569  ns/workflows/bui
-00000520: 6c64 2e79 616d 6c0d 0a5b 636f 7665 7261  ld.yaml..[covera
-00000530: 6765 2d69 6d61 6765 5d3a 2068 7474 7073  ge-image]: https
-00000540: 3a2f 2f63 6f64 6563 6f76 2e69 6f2f 6768  ://codecov.io/gh
-00000550: 2f63 6f6d 706d 6563 2f73 6563 7469 6f6e  /compmec/section
-00000560: 2d70 726f 7065 7274 6965 732f 6272 616e  -properties/bran
-00000570: 6368 2f6d 6169 6e2f 6772 6170 682f 6261  ch/main/graph/ba
-00000580: 6467 652e 7376 673f 746f 6b65 6e3d 7666  dge.svg?token=vf
-00000590: 474d 5065 3957 3349 0d0a 5b63 6f76 6572  GMPe9W3I..[cover
-000005a0: 6167 652d 7572 6c5d 3a20 6874 7470 733a  age-url]: https:
-000005b0: 2f2f 636f 6465 636f 762e 696f 2f67 682f  //codecov.io/gh/
-000005c0: 636f 6d70 6d65 632f 7365 6374 696f 6e2d  compmec/section-
-000005d0: 7072 6f70 6572 7469 6573 0d0a 5b76 6572  properties..[ver
-000005e0: 7369 6f6e 732d 696d 6167 655d 3a20 6874  sions-image]: ht
-000005f0: 7470 733a 2f2f 696d 672e 7368 6965 6c64  tps://img.shield
-00000600: 732e 696f 2f70 7970 692f 7079 7665 7273  s.io/pypi/pyvers
-00000610: 696f 6e73 2f63 6f6d 706d 6563 2d73 6563  ions/compmec-sec
-00000620: 7469 6f6e 2e73 7667 3f73 7479 6c65 3d66  tion.svg?style=f
-00000630: 6c61 742d 7371 7561 7265 0d0a 5b76 6572  lat-square..[ver
-00000640: 7369 6f6e 732d 7572 6c5d 3a20 6874 7470  sions-url]: http
-00000650: 733a 2f2f 7079 7069 2e6f 7267 2f70 726f  s://pypi.org/pro
-00000660: 6a65 6374 2f63 6f6d 706d 6563 2d73 6563  ject/compmec-sec
-00000670: 7469 6f6e 2f0d 0a5b 7079 7069 6c69 6e6b  tion/..[pypilink
-00000680: 5d3a 2068 7474 7073 3a2f 2f70 7970 692e  ]: https://pypi.
-00000690: 6f72 672f 7072 6f6a 6563 742f 636f 6d70  org/project/comp
-000006a0: 6d65 632d 7365 6374 696f 6e2f 0d0a 5b69  mec-section/..[i
-000006b0: 7373 7565 736c 696e 6b5d 3a20 6874 7470  ssueslink]: http
-000006c0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f63  s://github.com/c
-000006d0: 6f6d 706d 6563 2f73 6563 7469 6f6e 2d70  ompmec/section-p
-000006e0: 726f 7065 7274 6965 732f 6973 7375 6573  roperties/issues
-000006f0: 0d0a                                     ..
+00000000: 5b21 5b44 6f63 756d 656e 7461 7469 6f6e  [![Documentation
+00000010: 2053 7461 7475 735d 5b64 6f63 732d 696d   Status][docs-im
+00000020: 675d 5d5b 646f 6373 2d75 726c 5d0a 5b21  g]][docs-url].[!
+00000030: 5b42 7569 6c64 2053 7461 7475 735d 5b62  [Build Status][b
+00000040: 7569 6c64 2d69 6d67 5d5d 5b62 7569 6c64  uild-img]][build
+00000050: 2d75 726c 5d0a 5b21 5b4c 696e 7420 7769  -url].[![Lint wi
+00000060: 7468 2042 6c61 636b 5d5b 6c69 6e74 626c  th Black][lintbl
+00000070: 6163 6b2d 696d 675d 5d5b 6c69 6e74 626c  ack-img]][lintbl
+00000080: 6163 6b2d 7572 6c5d 0a5b 215b 436f 6465  ack-url].[![Code
+00000090: 2043 6f76 6572 6167 655d 5b63 6f76 6572   Coverage][cover
+000000a0: 6167 652d 696d 675d 5d5b 636f 7665 7261  age-img]][covera
+000000b0: 6765 2d75 726c 5d0a 0a5b 215b 5079 5049  ge-url]..[![PyPI
+000000c0: 2056 6572 7369 6f6e 5d5b 7079 7069 2d69   Version][pypi-i
+000000d0: 6d67 5d5d 5b70 7970 692d 7572 6c5d 0a5b  mg]][pypi-url].[
+000000e0: 215b 5079 7468 6f6e 2056 6572 7369 6f6e  ![Python Version
+000000f0: 735d 5b70 7976 6572 7369 6f6e 732d 696d  s][pyversions-im
+00000100: 675d 5d5b 7079 7665 7273 696f 6e73 2d75  g]][pyversions-u
+00000110: 726c 5d0a 5b21 5b4c 6963 656e 7365 3a20  rl].[![License: 
+00000120: 4d49 545d 5b6c 6963 656e 7365 2d69 6d67  MIT][license-img
+00000130: 5d5d 5b6c 6963 656e 7365 2d75 726c 5d0a  ]][license-url].
+00000140: 0a0a 4120 7079 7468 6f6e 2070 6163 6b61  ..A python packa
+00000150: 6765 2066 6f72 2061 6e61 6c79 7369 7320  ge for analysis 
+00000160: 6f66 2061 7262 6974 7261 7279 2062 6561  of arbitrary bea
+00000170: 6d20 6372 6f73 7320 7365 6374 696f 6e20  m cross section 
+00000180: 7573 696e 6720 626f 756e 6461 7279 2065  using boundary e
+00000190: 6c65 6d65 6e74 206d 6574 686f 642e 0a0a  lement method...
+000001a0: 5468 6973 2070 6163 6b61 6765 2063 616e  This package can
+000001b0: 2062 6520 7573 6564 2069 6e20 7374 7275   be used in stru
+000001c0: 6374 7572 616c 2064 6573 6967 6e20 616e  ctural design an
+000001d0: 6420 7669 7375 616c 6973 6520 6465 666f  d visualise defo
+000001e0: 726d 6564 2070 726f 6669 6c65 2c20 7374  rmed profile, st
+000001f0: 7265 7373 2064 7565 2074 6f20 6170 706c  ress due to appl
+00000200: 6965 6420 666f 7263 6573 2061 6e64 206d  ied forces and m
+00000210: 6f6d 656e 7475 6d73 0a0a 2323 2320 496e  omentums..### In
+00000220: 7374 616c 6c61 7469 6f6e 3a0a 0a54 6869  stallation:..Thi
+00000230: 7320 6c69 6272 6172 7920 6973 2061 7661  s library is ava
+00000240: 696c 6162 6c65 2069 6e20 5b50 7950 495d  ilable in [PyPI]
+00000250: 5b70 7970 692d 7572 6c5d 2e20 546f 2069  [pypi-url]. To i
+00000260: 6e73 7461 6c6c 2069 740a 0a60 6060 0a24  nstall it..```.$
+00000270: 2070 6970 2069 6e73 7461 6c6c 2063 6f6d   pip install com
+00000280: 706d 6563 2d73 6563 7469 6f6e 0a60 6060  pmec-section.```
+00000290: 0a0a 466f 7220 6d6f 7265 2064 6574 6169  ..For more detai
+000002a0: 6c73 2c20 7265 6665 7220 746f 2074 6865  ls, refer to the
+000002b0: 205b 646f 6375 6d65 6e74 6174 696f 6e5d   [documentation]
+000002c0: 5b64 6f63 732d 6c69 6e6b 5d2e 0a0a 2323  [docs-link]...##
+000002d0: 2320 446f 6375 6d65 6e74 6174 696f 6e0a  # Documentation.
+000002e0: 0a54 6865 2064 6f63 756d 656e 7461 7469  .The documentati
+000002f0: 6f6e 2063 616e 2062 6520 666f 756e 6420  on can be found 
+00000300: 6174 205b 636f 6d70 6d65 632d 7365 6374  at [compmec-sect
+00000310: 696f 6e2e 7265 6164 7468 6564 6f63 732e  ion.readthedocs.
+00000320: 696f 5d5b 646f 6373 2d6c 696e 6b5d 0a0a  io][docs-link]..
+00000330: 0a23 2323 2043 6f6e 7472 6962 7574 650a  .### Contribute.
+00000340: 0a50 6c65 6173 6520 7573 6520 7468 6520  .Please use the 
+00000350: 5b49 7373 7565 735d 5b69 7373 7565 732d  [Issues][issues-
+00000360: 7572 6b5d 206f 7220 7265 6665 7220 746f  urk] or refer to
+00000370: 2074 6865 2065 6d61 696c 2060 6060 636f   the email ```co
+00000380: 6d70 6d65 6367 6974 4067 6d61 696c 2e63  mpmecgit@gmail.c
+00000390: 6f6d 6060 600a 0a3c 212d 2d20 4261 6467  om```..<!-- Badg
+000003a0: 6573 3a20 2d2d 3e0a 0a5b 6c69 6e74 626c  es: -->..[lintbl
+000003b0: 6163 6b2d 696d 675d 3a20 6874 7470 733a  ack-img]: https:
+000003c0: 2f2f 6769 7468 7562 2e63 6f6d 2f63 6f6d  //github.com/com
+000003d0: 706d 6563 2f73 6563 7469 6f6e 2d70 726f  pmec/section-pro
+000003e0: 7065 7274 6965 732f 6163 7469 6f6e 732f  perties/actions/
+000003f0: 776f 726b 666c 6f77 732f 626c 6163 6b2e  workflows/black.
+00000400: 7961 6d6c 2f62 6164 6765 2e73 7667 0a5b  yaml/badge.svg.[
+00000410: 6c69 6e74 626c 6163 6b2d 7572 6c5d 3a20  lintblack-url]: 
+00000420: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00000430: 6f6d 2f63 6f6d 706d 6563 2f73 6563 7469  om/compmec/secti
+00000440: 6f6e 2d70 726f 7065 7274 6965 732f 6163  on-properties/ac
+00000450: 7469 6f6e 732f 776f 726b 666c 6f77 732f  tions/workflows/
+00000460: 626c 6163 6b2e 7961 6d6c 0a5b 646f 6373  black.yaml.[docs
+00000470: 2d69 6d67 5d3a 2068 7474 7073 3a2f 2f72  -img]: https://r
+00000480: 6561 6474 6865 646f 6373 2e6f 7267 2f70  eadthedocs.org/p
+00000490: 726f 6a65 6374 732f 636f 6d70 6d65 632d  rojects/compmec-
+000004a0: 7365 6374 696f 6e2f 6261 6467 652f 3f76  section/badge/?v
+000004b0: 6572 7369 6f6e 3d6c 6174 6573 740a 5b64  ersion=latest.[d
+000004c0: 6f63 732d 7572 6c5d 3a20 6874 7470 733a  ocs-url]: https:
+000004d0: 2f2f 636f 6d70 6d65 632d 7365 6374 696f  //compmec-sectio
+000004e0: 6e2e 7265 6164 7468 6564 6f63 732e 696f  n.readthedocs.io
+000004f0: 2f65 6e2f 6c61 7465 7374 2f3f 6261 6467  /en/latest/?badg
+00000500: 653d 6c61 7465 7374 0a5b 7079 7069 2d69  e=latest.[pypi-i
+00000510: 6d67 5d3a 2068 7474 7073 3a2f 2f69 6d67  mg]: https://img
+00000520: 2e73 6869 656c 6473 2e69 6f2f 7079 7069  .shields.io/pypi
+00000530: 2f76 2f63 6f6d 706d 6563 2d73 6563 7469  /v/compmec-secti
+00000540: 6f6e 0a5b 7079 7069 2d75 726c 5d3a 2068  on.[pypi-url]: h
+00000550: 7474 7073 3a2f 2f70 7970 692e 6f72 672f  ttps://pypi.org/
+00000560: 7072 6f6a 6563 742f 636f 6d70 6d65 632d  project/compmec-
+00000570: 7365 6374 696f 6e2f 0a5b 6275 696c 642d  section/.[build-
+00000580: 696d 675d 3a20 6874 7470 733a 2f2f 6769  img]: https://gi
+00000590: 7468 7562 2e63 6f6d 2f63 6f6d 706d 6563  thub.com/compmec
+000005a0: 2f73 6563 7469 6f6e 2d70 726f 7065 7274  /section-propert
+000005b0: 6965 732f 6163 7469 6f6e 732f 776f 726b  ies/actions/work
+000005c0: 666c 6f77 732f 6275 696c 642e 7961 6d6c  flows/build.yaml
+000005d0: 2f62 6164 6765 2e73 7667 0a5b 6275 696c  /badge.svg.[buil
+000005e0: 642d 7572 6c5d 3a20 6874 7470 733a 2f2f  d-url]: https://
+000005f0: 6769 7468 7562 2e63 6f6d 2f63 6f6d 706d  github.com/compm
+00000600: 6563 2f73 6563 7469 6f6e 2d70 726f 7065  ec/section-prope
+00000610: 7274 6965 732f 6163 7469 6f6e 732f 776f  rties/actions/wo
+00000620: 726b 666c 6f77 732f 6275 696c 642e 7961  rkflows/build.ya
+00000630: 6d6c 0a5b 636f 7665 7261 6765 2d69 6d67  ml.[coverage-img
+00000640: 5d3a 2068 7474 7073 3a2f 2f63 6f64 6563  ]: https://codec
+00000650: 6f76 2e69 6f2f 6768 2f63 6f6d 706d 6563  ov.io/gh/compmec
+00000660: 2f73 6563 7469 6f6e 2d70 726f 7065 7274  /section-propert
+00000670: 6965 732f 6272 616e 6368 2f6d 6169 6e2f  ies/branch/main/
+00000680: 6772 6170 682f 6261 6467 652e 7376 673f  graph/badge.svg?
+00000690: 746f 6b65 6e3d 7666 474d 5065 3957 3349  token=vfGMPe9W3I
+000006a0: 0a5b 636f 7665 7261 6765 2d75 726c 5d3a  .[coverage-url]:
+000006b0: 2068 7474 7073 3a2f 2f63 6f64 6563 6f76   https://codecov
+000006c0: 2e69 6f2f 6768 2f63 6f6d 706d 6563 2f73  .io/gh/compmec/s
+000006d0: 6563 7469 6f6e 2d70 726f 7065 7274 6965  ection-propertie
+000006e0: 730a 5b70 7976 6572 7369 6f6e 732d 696d  s.[pyversions-im
+000006f0: 675d 3a20 6874 7470 733a 2f2f 696d 672e  g]: https://img.
+00000700: 7368 6965 6c64 732e 696f 2f70 7970 692f  shields.io/pypi/
+00000710: 7079 7665 7273 696f 6e73 2f63 6f6d 706d  pyversions/compm
+00000720: 6563 2d73 6563 7469 6f6e 2e73 7667 3f73  ec-section.svg?s
+00000730: 7479 6c65 3d66 6c61 742d 7371 7561 7265  tyle=flat-square
+00000740: 0a5b 7079 7665 7273 696f 6e73 2d75 726c  .[pyversions-url
+00000750: 5d3a 2068 7474 7073 3a2f 2f70 7970 692e  ]: https://pypi.
+00000760: 6f72 672f 7072 6f6a 6563 742f 636f 6d70  org/project/comp
+00000770: 6d65 632d 7365 6374 696f 6e2f 0a5b 6c69  mec-section/.[li
+00000780: 6365 6e73 652d 696d 675d 3a20 6874 7470  cense-img]: http
+00000790: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
+000007a0: 696f 2f70 7970 692f 6c2f 616e 7369 636f  io/pypi/l/ansico
+000007b0: 6c6f 7274 6167 732e 7376 670a 5b6c 6963  lortags.svg.[lic
+000007c0: 656e 7365 2d75 726c 5d3a 2068 7474 7073  ense-url]: https
+000007d0: 3a2f 2f67 6974 6875 622e 636f 6d2f 636f  ://github.com/co
+000007e0: 6d70 6d65 632f 7365 6374 696f 6e2d 7072  mpmec/section-pr
+000007f0: 6f70 6572 7469 6573 2f62 6c6f 622f 6d61  operties/blob/ma
+00000800: 696e 2f4c 4943 454e 5345 2e6d 640a 5b70  in/LICENSE.md.[p
+00000810: 7970 692d 7572 6c5d 3a20 6874 7470 733a  ypi-url]: https:
+00000820: 2f2f 7079 7069 2e6f 7267 2f70 726f 6a65  //pypi.org/proje
+00000830: 6374 2f63 6f6d 706d 6563 2d73 6563 7469  ct/compmec-secti
+00000840: 6f6e 2f0a 5b69 7373 7565 732d 7572 6c5d  on/.[issues-url]
+00000850: 3a20 6874 7470 733a 2f2f 6769 7468 7562  : https://github
+00000860: 2e63 6f6d 2f63 6f6d 706d 6563 2f73 6563  .com/compmec/sec
+00000870: 7469 6f6e 2d70 726f 7065 7274 6965 732f  tion-properties/
+00000880: 6973 7375 6573 0a                        issues.
```

### Comparing `compmec_section-0.1.2/src/compmec/section/material.py` & `compmec_section-0.1.3/src/compmec/section/material.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,92 +1,92 @@
-"""
-This module contains the class 'Isotropic' to store and convert values
-"""
-
-
-class Isotropic:
-    """
-    Isotropic materials are materials whose properties remain
-    the same when tested in different directions.
-    Wikipedia link of isotropy:
-    https://en.wikipedia.org/wiki/Isotropy
-    """
-
-    def __init__(self):
-        pass
-
-    @property
-    def young_modulus(self):
-        """
-        Young modulus (E) is a mechanical property that measures
-        the tensile or compressive stiffness of a solid material
-        when the force is applied lengthwise
-        https://en.wikipedia.org/wiki/Young%27s_modulus
-        """
-        return self._young_modulus
-
-    @property
-    def poissons_ratio(self):
-        """
-        Poisson's ratio (nu) is a measure of the Poisson effect,
-        the deformation (expansion or contraction) of a material
-        in directions perpendicular to the specific direction of loading
-        https://en.wikipedia.org/wiki/Poisson%27s_ratio
-        """
-        return self._poissons_ratio
-
-    @property
-    def bulk_modulus(self):
-        """
-        The bulk modulus (K) of a substance is a measure
-        of the resistance of a substance to compression.
-        https://en.wikipedia.org/wiki/Bulk_modulus
-        """
-        return self.young_modulus / (3 * (1 - 2 * self.poissons_ratio))
-
-    @property
-    def shear_modulus(self):
-        """
-        Shear modulus (G), is a measure of the elastic shear
-        stiffness of a material and is defined as the ratio
-        of shear stress to the shear strain.
-        https://en.wikipedia.org/wiki/Shear_modulus
-        """
-        return self.young_modulus / (2 * (1 + self.poissons_ratio))
-
-    @property
-    def lames_parameter_1(self):
-        """
-        Lamé parameters (also called the Lamé coefficients)
-        are two material-dependent quantities denoted by lambda
-        and mu that arise in strain-stress relationships.
-        https://en.wikipedia.org/wiki/Lam%C3%A9_parameters
-        """
-        shear = self.shear_modulus
-        poisson = self.poissons_ratio
-        return 2 * shear * poisson / (1 - 2 * poisson)
-
-    @property
-    def lames_parameter_2(self):
-        """
-        Lamé parameters (also called the Lamé coefficients)
-        are two material-dependent quantities denoted by lambda
-        and mu that arise in strain-stress relationships.
-        https://en.wikipedia.org/wiki/Lam%C3%A9_parameters
-        """
-        return self.shear_modulus
-
-    @young_modulus.setter
-    def young_modulus(self, value: float):
-        if value <= 0:
-            raise ValueError
-        self._young_modulus = value
-
-    @poissons_ratio.setter
-    def poissons_ratio(self, value: float):
-        if value < 0.49:
-            pass
-        elif value < 0.50:
-            raise ValueError("Material is incompressible")
-        else:
-            raise ValueError("Cannot have poisson >= 0.50 ")
-        self._poissons_ratio = value
+"""
+This module contains the class 'Isotropic' to store and convert values
+"""
+
+
+class Isotropic:
+    """
+    Isotropic materials are materials whose properties remain
+    the same when tested in different directions.
+    Wikipedia link of isotropy:
+    https://en.wikipedia.org/wiki/Isotropy
+    """
+
+    def __init__(self):
+        pass
+
+    @property
+    def young_modulus(self):
+        """
+        Young modulus (E) is a mechanical property that measures
+        the tensile or compressive stiffness of a solid material
+        when the force is applied lengthwise
+        https://en.wikipedia.org/wiki/Young%27s_modulus
+        """
+        return self._young_modulus
+
+    @property
+    def poissons_ratio(self):
+        """
+        Poisson's ratio (nu) is a measure of the Poisson effect,
+        the deformation (expansion or contraction) of a material
+        in directions perpendicular to the specific direction of loading
+        https://en.wikipedia.org/wiki/Poisson%27s_ratio
+        """
+        return self._poissons_ratio
+
+    @property
+    def bulk_modulus(self):
+        """
+        The bulk modulus (K) of a substance is a measure
+        of the resistance of a substance to compression.
+        https://en.wikipedia.org/wiki/Bulk_modulus
+        """
+        return self.young_modulus / (3 * (1 - 2 * self.poissons_ratio))
+
+    @property
+    def shear_modulus(self):
+        """
+        Shear modulus (G), is a measure of the elastic shear
+        stiffness of a material and is defined as the ratio
+        of shear stress to the shear strain.
+        https://en.wikipedia.org/wiki/Shear_modulus
+        """
+        return self.young_modulus / (2 * (1 + self.poissons_ratio))
+
+    @property
+    def lames_parameter_1(self):
+        """
+        Lamé parameters (also called the Lamé coefficients)
+        are two material-dependent quantities denoted by lambda
+        and mu that arise in strain-stress relationships.
+        https://en.wikipedia.org/wiki/Lam%C3%A9_parameters
+        """
+        shear = self.shear_modulus
+        poisson = self.poissons_ratio
+        return 2 * shear * poisson / (1 - 2 * poisson)
+
+    @property
+    def lames_parameter_2(self):
+        """
+        Lamé parameters (also called the Lamé coefficients)
+        are two material-dependent quantities denoted by lambda
+        and mu that arise in strain-stress relationships.
+        https://en.wikipedia.org/wiki/Lam%C3%A9_parameters
+        """
+        return self.shear_modulus
+
+    @young_modulus.setter
+    def young_modulus(self, value: float):
+        if value <= 0:
+            raise ValueError
+        self._young_modulus = value
+
+    @poissons_ratio.setter
+    def poissons_ratio(self, value: float):
+        if value < 0.49:
+            pass
+        elif value < 0.50:
+            raise ValueError("Material is incompressible")
+        else:
+            raise ValueError("Cannot have poisson >= 0.50 ")
+        self._poissons_ratio = value
```

### Comparing `compmec_section-0.1.2/PKG-INFO` & `compmec_section-0.1.3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 636f 6d70  : 2.1.Name: comp
 00000020: 6d65 632d 7365 6374 696f 6e0a 5665 7273  mec-section.Vers
-00000030: 696f 6e3a 2030 2e31 2e32 0a53 756d 6d61  ion: 0.1.2.Summa
+00000030: 696f 6e3a 2030 2e31 2e33 0a53 756d 6d61  ion: 0.1.3.Summa
 00000040: 7279 3a20 436f 6d70 7574 6520 6368 6172  ry: Compute char
 00000050: 6163 7465 7269 7374 6963 7320 6f66 2061  acteristics of a
 00000060: 6e20 6172 6269 7472 6172 7920 6372 6f73  n arbitrary cros
 00000070: 732d 7365 6374 696f 6e20 696e 2070 7974  s-section in pyt
 00000080: 686f 6e0a 4175 7468 6f72 3a20 4361 726c  hon.Author: Carl
 00000090: 6f73 2041 6469 720a 4175 7468 6f72 2d65  os Adir.Author-e
 000000a0: 6d61 696c 3a20 6361 726c 6f73 2e61 6469  mail: carlos.adi
@@ -31,117 +31,145 @@
 000001e0: 723a 2050 726f 6772 616d 6d69 6e67 204c  r: Programming L
 000001f0: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
 00000200: 6e20 3a3a 2033 2e31 310a 5265 7175 6972  n :: 3.11.Requir
 00000210: 6573 2d44 6973 743a 206e 756d 7079 2028  es-Dist: numpy (
 00000220: 3e3d 312e 302e 302c 3c32 2e30 2e30 290a  >=1.0.0,<2.0.0).
 00000230: 4465 7363 7269 7074 696f 6e2d 436f 6e74  Description-Cont
 00000240: 656e 742d 5479 7065 3a20 7465 7874 2f6d  ent-Type: text/m
-00000250: 6172 6b64 6f77 6e0a 0a5b 215b 5079 5049  arkdown..[![PyPI
-00000260: 2056 6572 7369 6f6e 5d5b 7079 7069 2d69   Version][pypi-i
-00000270: 6d61 6765 5d5d 5b70 7970 692d 7572 6c5d  mage]][pypi-url]
-00000280: 0a5b 215b 4275 696c 6420 5374 6174 7573  .[![Build Status
-00000290: 5d5b 6275 696c 642d 696d 6167 655d 5d5b  ][build-image]][
-000002a0: 6275 696c 642d 7572 6c5d 0a5b 215b 436f  build-url].[![Co
-000002b0: 6465 2043 6f76 6572 6167 655d 5b63 6f76  de Coverage][cov
-000002c0: 6572 6167 652d 696d 6167 655d 5d5b 636f  erage-image]][co
-000002d0: 7665 7261 6765 2d75 726c 5d0a 5b21 5b5d  verage-url].[![]
-000002e0: 5b76 6572 7369 6f6e 732d 696d 6167 655d  [versions-image]
-000002f0: 5d5b 7665 7273 696f 6e73 2d75 726c 5d0a  ][versions-url].
-00000300: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
-00000310: 2f67 6974 6875 622e 636f 6d2f 636f 6d70  /github.com/comp
-00000320: 6d65 632f 7365 6374 696f 6e2d 7072 6f70  mec/section-prop
-00000330: 6572 7469 6573 223e 3c69 6d67 2061 6c74  erties"><img alt
-00000340: 3d22 436f 6465 2073 7479 6c65 3a20 626c  ="Code style: bl
-00000350: 6163 6b22 2073 7263 3d22 6874 7470 733a  ack" src="https:
-00000360: 2f2f 696d 672e 7368 6965 6c64 732e 696f  //img.shields.io
-00000370: 2f62 6164 6765 2f63 6f64 6525 3230 7374  /badge/code%20st
-00000380: 796c 652d 626c 6163 6b2d 3030 3030 3030  yle-black-000000
-00000390: 2e73 7667 223e 3c2f 613e 0a3c 6120 6872  .svg"></a>.<a hr
-000003a0: 6566 3d22 6874 7470 733a 2f2f 6769 7468  ef="https://gith
-000003b0: 7562 2e63 6f6d 2f63 6f6d 706d 6563 2f73  ub.com/compmec/s
-000003c0: 6563 7469 6f6e 2d70 726f 7065 7274 6965  ection-propertie
-000003d0: 732f 626c 6f62 2f6d 6169 6e2f 4c49 4345  s/blob/main/LICE
-000003e0: 4e53 452e 6d64 223e 3c69 6d67 2061 6c74  NSE.md"><img alt
-000003f0: 3d22 4c69 6365 6e73 653a 204d 4954 2220  ="License: MIT" 
-00000400: 7372 633d 2268 7474 7073 3a2f 2f62 6c61  src="https://bla
-00000410: 636b 2e72 6561 6474 6865 646f 6373 2e69  ck.readthedocs.i
-00000420: 6f2f 656e 2f73 7461 626c 652f 5f73 7461  o/en/stable/_sta
-00000430: 7469 632f 6c69 6365 6e73 652e 7376 6722  tic/license.svg"
-00000440: 3e3c 2f61 3e0a 0a0a 4120 7079 7468 6f6e  ></a>...A python
-00000450: 2070 6163 6b61 6765 2066 6f72 2061 6e61   package for ana
-00000460: 6c79 7369 7320 6f66 2061 7262 6974 7261  lysis of arbitra
-00000470: 7279 2062 6561 6d20 6372 6f73 7320 7365  ry beam cross se
-00000480: 6374 696f 6e20 7573 696e 6720 626f 756e  ction using boun
-00000490: 6461 7279 2065 6c65 6d65 6e74 206d 6574  dary element met
-000004a0: 686f 642e 0a0a 5468 6973 2070 6163 6b61  hod...This packa
-000004b0: 6765 2063 616e 2062 6520 7573 6564 2069  ge can be used i
-000004c0: 6e20 7374 7275 6374 7572 616c 2064 6573  n structural des
-000004d0: 6967 6e20 616e 6420 7669 7375 616c 6973  ign and visualis
-000004e0: 6520 6465 666f 726d 6564 2070 726f 6669  e deformed profi
-000004f0: 6c65 2c20 7374 7265 7373 2064 7565 2074  le, stress due t
-00000500: 6f20 6170 706c 6965 6420 666f 7263 6573  o applied forces
-00000510: 2061 6e64 206d 6f6d 656e 7475 6d73 0a0a   and momentums..
-00000520: 2323 2320 496e 7374 616c 6c61 7469 6f6e  ### Installation
-00000530: 3a0a 0a54 6869 7320 6c69 6272 6172 7920  :..This library 
-00000540: 6973 2061 7661 696c 6162 6c65 2069 6e20  is available in 
-00000550: 5b50 7950 495d 5b70 7970 696c 696e 6b5d  [PyPI][pypilink]
-00000560: 2e20 546f 2069 6e73 7461 6c6c 2069 740a  . To install it.
-00000570: 0a60 6060 0a24 2070 6970 2069 6e73 7461  .```.$ pip insta
-00000580: 6c6c 2063 6f6d 706d 6563 2d73 6563 7469  ll compmec-secti
-00000590: 6f6e 0a60 6060 0a0a 2323 2320 446f 6375  on.```..### Docu
-000005a0: 6d65 6e74 6174 696f 6e0a 0a49 6e20 7072  mentation..In pr
-000005b0: 6f67 7265 7373 0a0a 0a23 2323 2043 6f6e  ogress...### Con
-000005c0: 7472 6962 7574 650a 0a50 6c65 6173 6520  tribute..Please 
-000005d0: 7573 6520 7468 6520 5b49 7373 7565 735d  use the [Issues]
-000005e0: 5b69 7373 7565 736c 696e 6b5d 206f 7220  [issueslink] or 
-000005f0: 7265 6665 7220 746f 2074 6865 2065 6d61  refer to the ema
-00000600: 696c 2060 6060 636f 6d70 6d65 6367 6974  il ```compmecgit
-00000610: 4067 6d61 696c 2e63 6f6d 6060 600a 0a3c  @gmail.com```..<
-00000620: 212d 2d20 4261 6467 6573 3a20 2d2d 3e0a  !-- Badges: -->.
-00000630: 0a5b 7079 7069 2d69 6d61 6765 5d3a 2068  .[pypi-image]: h
-00000640: 7474 7073 3a2f 2f69 6d67 2e73 6869 656c  ttps://img.shiel
-00000650: 6473 2e69 6f2f 7079 7069 2f76 2f63 6f6d  ds.io/pypi/v/com
-00000660: 706d 6563 2d73 6563 7469 6f6e 0a5b 7079  pmec-section.[py
-00000670: 7069 2d75 726c 5d3a 2068 7474 7073 3a2f  pi-url]: https:/
-00000680: 2f70 7970 692e 6f72 672f 7072 6f6a 6563  /pypi.org/projec
-00000690: 742f 636f 6d70 6d65 632d 7365 6374 696f  t/compmec-sectio
-000006a0: 6e2f 0a5b 6275 696c 642d 696d 6167 655d  n/.[build-image]
-000006b0: 3a20 6874 7470 733a 2f2f 6769 7468 7562  : https://github
-000006c0: 2e63 6f6d 2f63 6f6d 706d 6563 2f73 6563  .com/compmec/sec
-000006d0: 7469 6f6e 2d70 726f 7065 7274 6965 732f  tion-properties/
-000006e0: 6163 7469 6f6e 732f 776f 726b 666c 6f77  actions/workflow
-000006f0: 732f 6275 696c 642e 7961 6d6c 2f62 6164  s/build.yaml/bad
-00000700: 6765 2e73 7667 0a5b 6275 696c 642d 7572  ge.svg.[build-ur
-00000710: 6c5d 3a20 6874 7470 733a 2f2f 6769 7468  l]: https://gith
-00000720: 7562 2e63 6f6d 2f63 6f6d 706d 6563 2f73  ub.com/compmec/s
-00000730: 6563 7469 6f6e 2d70 726f 7065 7274 6965  ection-propertie
-00000740: 732f 6163 7469 6f6e 732f 776f 726b 666c  s/actions/workfl
-00000750: 6f77 732f 6275 696c 642e 7961 6d6c 0a5b  ows/build.yaml.[
-00000760: 636f 7665 7261 6765 2d69 6d61 6765 5d3a  coverage-image]:
-00000770: 2068 7474 7073 3a2f 2f63 6f64 6563 6f76   https://codecov
-00000780: 2e69 6f2f 6768 2f63 6f6d 706d 6563 2f73  .io/gh/compmec/s
-00000790: 6563 7469 6f6e 2d70 726f 7065 7274 6965  ection-propertie
-000007a0: 732f 6272 616e 6368 2f6d 6169 6e2f 6772  s/branch/main/gr
-000007b0: 6170 682f 6261 6467 652e 7376 673f 746f  aph/badge.svg?to
-000007c0: 6b65 6e3d 7666 474d 5065 3957 3349 0a5b  ken=vfGMPe9W3I.[
-000007d0: 636f 7665 7261 6765 2d75 726c 5d3a 2068  coverage-url]: h
-000007e0: 7474 7073 3a2f 2f63 6f64 6563 6f76 2e69  ttps://codecov.i
-000007f0: 6f2f 6768 2f63 6f6d 706d 6563 2f73 6563  o/gh/compmec/sec
-00000800: 7469 6f6e 2d70 726f 7065 7274 6965 730a  tion-properties.
-00000810: 5b76 6572 7369 6f6e 732d 696d 6167 655d  [versions-image]
-00000820: 3a20 6874 7470 733a 2f2f 696d 672e 7368  : https://img.sh
-00000830: 6965 6c64 732e 696f 2f70 7970 692f 7079  ields.io/pypi/py
-00000840: 7665 7273 696f 6e73 2f63 6f6d 706d 6563  versions/compmec
-00000850: 2d73 6563 7469 6f6e 2e73 7667 3f73 7479  -section.svg?sty
-00000860: 6c65 3d66 6c61 742d 7371 7561 7265 0a5b  le=flat-square.[
-00000870: 7665 7273 696f 6e73 2d75 726c 5d3a 2068  versions-url]: h
-00000880: 7474 7073 3a2f 2f70 7970 692e 6f72 672f  ttps://pypi.org/
-00000890: 7072 6f6a 6563 742f 636f 6d70 6d65 632d  project/compmec-
-000008a0: 7365 6374 696f 6e2f 0a5b 7079 7069 6c69  section/.[pypili
-000008b0: 6e6b 5d3a 2068 7474 7073 3a2f 2f70 7970  nk]: https://pyp
-000008c0: 692e 6f72 672f 7072 6f6a 6563 742f 636f  i.org/project/co
-000008d0: 6d70 6d65 632d 7365 6374 696f 6e2f 0a5b  mpmec-section/.[
-000008e0: 6973 7375 6573 6c69 6e6b 5d3a 2068 7474  issueslink]: htt
-000008f0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00000900: 636f 6d70 6d65 632f 7365 6374 696f 6e2d  compmec/section-
-00000910: 7072 6f70 6572 7469 6573 2f69 7373 7565  properties/issue
-00000920: 730a 0a                                  s..
+00000250: 6172 6b64 6f77 6e0a 0a5b 215b 446f 6375  arkdown..[![Docu
+00000260: 6d65 6e74 6174 696f 6e20 5374 6174 7573  mentation Status
+00000270: 5d5b 646f 6373 2d69 6d67 5d5d 5b64 6f63  ][docs-img]][doc
+00000280: 732d 7572 6c5d 0a5b 215b 4275 696c 6420  s-url].[![Build 
+00000290: 5374 6174 7573 5d5b 6275 696c 642d 696d  Status][build-im
+000002a0: 675d 5d5b 6275 696c 642d 7572 6c5d 0a5b  g]][build-url].[
+000002b0: 215b 4c69 6e74 2077 6974 6820 426c 6163  ![Lint with Blac
+000002c0: 6b5d 5b6c 696e 7462 6c61 636b 2d69 6d67  k][lintblack-img
+000002d0: 5d5d 5b6c 696e 7462 6c61 636b 2d75 726c  ]][lintblack-url
+000002e0: 5d0a 5b21 5b43 6f64 6520 436f 7665 7261  ].[![Code Covera
+000002f0: 6765 5d5b 636f 7665 7261 6765 2d69 6d67  ge][coverage-img
+00000300: 5d5d 5b63 6f76 6572 6167 652d 7572 6c5d  ]][coverage-url]
+00000310: 0a0a 5b21 5b50 7950 4920 5665 7273 696f  ..[![PyPI Versio
+00000320: 6e5d 5b70 7970 692d 696d 675d 5d5b 7079  n][pypi-img]][py
+00000330: 7069 2d75 726c 5d0a 5b21 5b50 7974 686f  pi-url].[![Pytho
+00000340: 6e20 5665 7273 696f 6e73 5d5b 7079 7665  n Versions][pyve
+00000350: 7273 696f 6e73 2d69 6d67 5d5d 5b70 7976  rsions-img]][pyv
+00000360: 6572 7369 6f6e 732d 7572 6c5d 0a5b 215b  ersions-url].[![
+00000370: 4c69 6365 6e73 653a 204d 4954 5d5b 6c69  License: MIT][li
+00000380: 6365 6e73 652d 696d 675d 5d5b 6c69 6365  cense-img]][lice
+00000390: 6e73 652d 7572 6c5d 0a0a 0a41 2070 7974  nse-url]...A pyt
+000003a0: 686f 6e20 7061 636b 6167 6520 666f 7220  hon package for 
+000003b0: 616e 616c 7973 6973 206f 6620 6172 6269  analysis of arbi
+000003c0: 7472 6172 7920 6265 616d 2063 726f 7373  trary beam cross
+000003d0: 2073 6563 7469 6f6e 2075 7369 6e67 2062   section using b
+000003e0: 6f75 6e64 6172 7920 656c 656d 656e 7420  oundary element 
+000003f0: 6d65 7468 6f64 2e0a 0a54 6869 7320 7061  method...This pa
+00000400: 636b 6167 6520 6361 6e20 6265 2075 7365  ckage can be use
+00000410: 6420 696e 2073 7472 7563 7475 7261 6c20  d in structural 
+00000420: 6465 7369 676e 2061 6e64 2076 6973 7561  design and visua
+00000430: 6c69 7365 2064 6566 6f72 6d65 6420 7072  lise deformed pr
+00000440: 6f66 696c 652c 2073 7472 6573 7320 6475  ofile, stress du
+00000450: 6520 746f 2061 7070 6c69 6564 2066 6f72  e to applied for
+00000460: 6365 7320 616e 6420 6d6f 6d65 6e74 756d  ces and momentum
+00000470: 730a 0a23 2323 2049 6e73 7461 6c6c 6174  s..### Installat
+00000480: 696f 6e3a 0a0a 5468 6973 206c 6962 7261  ion:..This libra
+00000490: 7279 2069 7320 6176 6169 6c61 626c 6520  ry is available 
+000004a0: 696e 205b 5079 5049 5d5b 7079 7069 2d75  in [PyPI][pypi-u
+000004b0: 726c 5d2e 2054 6f20 696e 7374 616c 6c20  rl]. To install 
+000004c0: 6974 0a0a 6060 600a 2420 7069 7020 696e  it..```.$ pip in
+000004d0: 7374 616c 6c20 636f 6d70 6d65 632d 7365  stall compmec-se
+000004e0: 6374 696f 6e0a 6060 600a 0a46 6f72 206d  ction.```..For m
+000004f0: 6f72 6520 6465 7461 696c 732c 2072 6566  ore details, ref
+00000500: 6572 2074 6f20 7468 6520 5b64 6f63 756d  er to the [docum
+00000510: 656e 7461 7469 6f6e 5d5b 646f 6373 2d6c  entation][docs-l
+00000520: 696e 6b5d 2e0a 0a23 2323 2044 6f63 756d  ink]...### Docum
+00000530: 656e 7461 7469 6f6e 0a0a 5468 6520 646f  entation..The do
+00000540: 6375 6d65 6e74 6174 696f 6e20 6361 6e20  cumentation can 
+00000550: 6265 2066 6f75 6e64 2061 7420 5b63 6f6d  be found at [com
+00000560: 706d 6563 2d73 6563 7469 6f6e 2e72 6561  pmec-section.rea
+00000570: 6474 6865 646f 6373 2e69 6f5d 5b64 6f63  dthedocs.io][doc
+00000580: 732d 6c69 6e6b 5d0a 0a0a 2323 2320 436f  s-link]...### Co
+00000590: 6e74 7269 6275 7465 0a0a 506c 6561 7365  ntribute..Please
+000005a0: 2075 7365 2074 6865 205b 4973 7375 6573   use the [Issues
+000005b0: 5d5b 6973 7375 6573 2d75 726b 5d20 6f72  ][issues-urk] or
+000005c0: 2072 6566 6572 2074 6f20 7468 6520 656d   refer to the em
+000005d0: 6169 6c20 6060 6063 6f6d 706d 6563 6769  ail ```compmecgi
+000005e0: 7440 676d 6169 6c2e 636f 6d60 6060 0a0a  t@gmail.com```..
+000005f0: 3c21 2d2d 2042 6164 6765 733a 202d 2d3e  <!-- Badges: -->
+00000600: 0a0a 5b6c 696e 7462 6c61 636b 2d69 6d67  ..[lintblack-img
+00000610: 5d3a 2068 7474 7073 3a2f 2f67 6974 6875  ]: https://githu
+00000620: 622e 636f 6d2f 636f 6d70 6d65 632f 7365  b.com/compmec/se
+00000630: 6374 696f 6e2d 7072 6f70 6572 7469 6573  ction-properties
+00000640: 2f61 6374 696f 6e73 2f77 6f72 6b66 6c6f  /actions/workflo
+00000650: 7773 2f62 6c61 636b 2e79 616d 6c2f 6261  ws/black.yaml/ba
+00000660: 6467 652e 7376 670a 5b6c 696e 7462 6c61  dge.svg.[lintbla
+00000670: 636b 2d75 726c 5d3a 2068 7474 7073 3a2f  ck-url]: https:/
+00000680: 2f67 6974 6875 622e 636f 6d2f 636f 6d70  /github.com/comp
+00000690: 6d65 632f 7365 6374 696f 6e2d 7072 6f70  mec/section-prop
+000006a0: 6572 7469 6573 2f61 6374 696f 6e73 2f77  erties/actions/w
+000006b0: 6f72 6b66 6c6f 7773 2f62 6c61 636b 2e79  orkflows/black.y
+000006c0: 616d 6c0a 5b64 6f63 732d 696d 675d 3a20  aml.[docs-img]: 
+000006d0: 6874 7470 733a 2f2f 7265 6164 7468 6564  https://readthed
+000006e0: 6f63 732e 6f72 672f 7072 6f6a 6563 7473  ocs.org/projects
+000006f0: 2f63 6f6d 706d 6563 2d73 6563 7469 6f6e  /compmec-section
+00000700: 2f62 6164 6765 2f3f 7665 7273 696f 6e3d  /badge/?version=
+00000710: 6c61 7465 7374 0a5b 646f 6373 2d75 726c  latest.[docs-url
+00000720: 5d3a 2068 7474 7073 3a2f 2f63 6f6d 706d  ]: https://compm
+00000730: 6563 2d73 6563 7469 6f6e 2e72 6561 6474  ec-section.readt
+00000740: 6865 646f 6373 2e69 6f2f 656e 2f6c 6174  hedocs.io/en/lat
+00000750: 6573 742f 3f62 6164 6765 3d6c 6174 6573  est/?badge=lates
+00000760: 740a 5b70 7970 692d 696d 675d 3a20 6874  t.[pypi-img]: ht
+00000770: 7470 733a 2f2f 696d 672e 7368 6965 6c64  tps://img.shield
+00000780: 732e 696f 2f70 7970 692f 762f 636f 6d70  s.io/pypi/v/comp
+00000790: 6d65 632d 7365 6374 696f 6e0a 5b70 7970  mec-section.[pyp
+000007a0: 692d 7572 6c5d 3a20 6874 7470 733a 2f2f  i-url]: https://
+000007b0: 7079 7069 2e6f 7267 2f70 726f 6a65 6374  pypi.org/project
+000007c0: 2f63 6f6d 706d 6563 2d73 6563 7469 6f6e  /compmec-section
+000007d0: 2f0a 5b62 7569 6c64 2d69 6d67 5d3a 2068  /.[build-img]: h
+000007e0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+000007f0: 6d2f 636f 6d70 6d65 632f 7365 6374 696f  m/compmec/sectio
+00000800: 6e2d 7072 6f70 6572 7469 6573 2f61 6374  n-properties/act
+00000810: 696f 6e73 2f77 6f72 6b66 6c6f 7773 2f62  ions/workflows/b
+00000820: 7569 6c64 2e79 616d 6c2f 6261 6467 652e  uild.yaml/badge.
+00000830: 7376 670a 5b62 7569 6c64 2d75 726c 5d3a  svg.[build-url]:
+00000840: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
+00000850: 636f 6d2f 636f 6d70 6d65 632f 7365 6374  com/compmec/sect
+00000860: 696f 6e2d 7072 6f70 6572 7469 6573 2f61  ion-properties/a
+00000870: 6374 696f 6e73 2f77 6f72 6b66 6c6f 7773  ctions/workflows
+00000880: 2f62 7569 6c64 2e79 616d 6c0a 5b63 6f76  /build.yaml.[cov
+00000890: 6572 6167 652d 696d 675d 3a20 6874 7470  erage-img]: http
+000008a0: 733a 2f2f 636f 6465 636f 762e 696f 2f67  s://codecov.io/g
+000008b0: 682f 636f 6d70 6d65 632f 7365 6374 696f  h/compmec/sectio
+000008c0: 6e2d 7072 6f70 6572 7469 6573 2f62 7261  n-properties/bra
+000008d0: 6e63 682f 6d61 696e 2f67 7261 7068 2f62  nch/main/graph/b
+000008e0: 6164 6765 2e73 7667 3f74 6f6b 656e 3d76  adge.svg?token=v
+000008f0: 6647 4d50 6539 5733 490a 5b63 6f76 6572  fGMPe9W3I.[cover
+00000900: 6167 652d 7572 6c5d 3a20 6874 7470 733a  age-url]: https:
+00000910: 2f2f 636f 6465 636f 762e 696f 2f67 682f  //codecov.io/gh/
+00000920: 636f 6d70 6d65 632f 7365 6374 696f 6e2d  compmec/section-
+00000930: 7072 6f70 6572 7469 6573 0a5b 7079 7665  properties.[pyve
+00000940: 7273 696f 6e73 2d69 6d67 5d3a 2068 7474  rsions-img]: htt
+00000950: 7073 3a2f 2f69 6d67 2e73 6869 656c 6473  ps://img.shields
+00000960: 2e69 6f2f 7079 7069 2f70 7976 6572 7369  .io/pypi/pyversi
+00000970: 6f6e 732f 636f 6d70 6d65 632d 7365 6374  ons/compmec-sect
+00000980: 696f 6e2e 7376 673f 7374 796c 653d 666c  ion.svg?style=fl
+00000990: 6174 2d73 7175 6172 650a 5b70 7976 6572  at-square.[pyver
+000009a0: 7369 6f6e 732d 7572 6c5d 3a20 6874 7470  sions-url]: http
+000009b0: 733a 2f2f 7079 7069 2e6f 7267 2f70 726f  s://pypi.org/pro
+000009c0: 6a65 6374 2f63 6f6d 706d 6563 2d73 6563  ject/compmec-sec
+000009d0: 7469 6f6e 2f0a 5b6c 6963 656e 7365 2d69  tion/.[license-i
+000009e0: 6d67 5d3a 2068 7474 7073 3a2f 2f69 6d67  mg]: https://img
+000009f0: 2e73 6869 656c 6473 2e69 6f2f 7079 7069  .shields.io/pypi
+00000a00: 2f6c 2f61 6e73 6963 6f6c 6f72 7461 6773  /l/ansicolortags
+00000a10: 2e73 7667 0a5b 6c69 6365 6e73 652d 7572  .svg.[license-ur
+00000a20: 6c5d 3a20 6874 7470 733a 2f2f 6769 7468  l]: https://gith
+00000a30: 7562 2e63 6f6d 2f63 6f6d 706d 6563 2f73  ub.com/compmec/s
+00000a40: 6563 7469 6f6e 2d70 726f 7065 7274 6965  ection-propertie
+00000a50: 732f 626c 6f62 2f6d 6169 6e2f 4c49 4345  s/blob/main/LICE
+00000a60: 4e53 452e 6d64 0a5b 7079 7069 2d75 726c  NSE.md.[pypi-url
+00000a70: 5d3a 2068 7474 7073 3a2f 2f70 7970 692e  ]: https://pypi.
+00000a80: 6f72 672f 7072 6f6a 6563 742f 636f 6d70  org/project/comp
+00000a90: 6d65 632d 7365 6374 696f 6e2f 0a5b 6973  mec-section/.[is
+00000aa0: 7375 6573 2d75 726c 5d3a 2068 7474 7073  sues-url]: https
+00000ab0: 3a2f 2f67 6974 6875 622e 636f 6d2f 636f  ://github.com/co
+00000ac0: 6d70 6d65 632f 7365 6374 696f 6e2d 7072  mpmec/section-pr
+00000ad0: 6f70 6572 7469 6573 2f69 7373 7565 730a  operties/issues.
+00000ae0: 0a                                       .
```

