# Comparing `tmp/pylibCZIrw-3.4.0.tar.gz` & `tmp/pylibCZIrw-3.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylibCZIrw-3.4.0.tar", last modified: Mon Apr 24 09:26:13 2023, max compression
+gzip compressed data, was "pylibCZIrw-3.4.1.tar", last modified: Tue Jun 27 11:40:23 2023, max compression
```

## Comparing `pylibCZIrw-3.4.0.tar` & `pylibCZIrw-3.4.1.tar`

### file list

```diff
@@ -1,551 +1,551 @@
-drwxrwxrwx   0        0        0        0 2023-04-24 09:26:13.671386 pylibCZIrw-3.4.0/
--rw-rw-rw-   0        0        0     4031 2023-04-24 09:24:54.000000 pylibCZIrw-3.4.0/CMakeLists.txt
--rw-rw-rw-   0        0        0      787 2023-04-24 09:24:54.000000 pylibCZIrw-3.4.0/CMakeSettings.json
--rw-rw-rw-   0        0        0     7815 2023-04-24 09:24:54.000000 pylibCZIrw-3.4.0/COPYING.LESSER.txt
--rw-rw-rw-   0        0        0    35821 2023-04-24 09:24:54.000000 pylibCZIrw-3.4.0/COPYING.txt
--rw-rw-rw-   0        0        0     2060 2023-04-24 09:24:54.000000 pylibCZIrw-3.4.0/INFO.md
--rw-rw-rw-   0        0        0      344 2023-04-24 09:24:54.000000 pylibCZIrw-3.4.0/MANIFEST.in
--rw-rw-rw-   0        0        0      191 2023-04-24 09:24:54.000000 pylibCZIrw-3.4.0/NOTICE.txt
--rw-rw-rw-   0        0        0     3026 2023-04-24 09:26:13.671386 pylibCZIrw-3.4.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-24 09:26:12.999511 pylibCZIrw-3.4.0/_pylibCZIrw/
-drwxrwxrwx   0        0        0        0 2023-04-24 09:26:12.999511 pylibCZIrw-3.4.0/_pylibCZIrw/src/
-drwxrwxrwx   0        0        0        0 2023-04-24 09:26:13.030737 pylibCZIrw-3.4.0/_pylibCZIrw/src/api/
--rw-rw-rw-   0        0        0     2292 2023-04-24 09:24:54.000000 pylibCZIrw-3.4.0/_pylibCZIrw/src/api/CZIreadAPI.cpp
--rw-rw-rw-   0        0        0     1996 2023-04-24 09:24:54.000000 pylibCZIrw-3.4.0/_pylibCZIrw/src/api/CZIreadAPI.h
--rw-rw-rw-   0        0        0    10601 2023-04-24 09:24:54.000000 pylibCZIrw-3.4.0/_pylibCZIrw/src/api/CZIwriteAPI.cpp
--rw-rw-rw-   0        0        0     6496 2023-04-24 09:24:54.000000 pylibCZIrw-3.4.0/_pylibCZIrw/src/api/CZIwriteAPI.h
--rw-rw-rw-   0        0        0      865 2023-04-24 09:24:54.000000 pylibCZIrw-3.4.0/_pylibCZIrw/src/api/DllMain.cpp
--rw-rw-rw-   0        0        0     1232 2023-04-24 09:24:54.000000 pylibCZIrw-3.4.0/_pylibCZIrw/src/api/PImage.cpp
--rw-rw-rw-   0        0        0     1740 2023-04-24 09:24:54.000000 pylibCZIrw-3.4.0/_pylibCZIrw/src/api/PImage.h
--rw-rw-rw-   0        0        0       64 2023-04-24 09:24:54.000000 pylibCZIrw-3.4.0/_pylibCZIrw/src/api/inc_libCzi.h
-drwxrwxrwx   0        0        0        0 2023-04-24 09:26:13.030737 pylibCZIrw-3.4.0/_pylibCZIrw/src/bindings/
--rw-rw-rw-   0        0        0     7998 2023-04-24 09:24:54.000000 pylibCZIrw-3.4.0/_pylibCZIrw/src/bindings/CZIrw.cpp
--rw-rw-rw-   0        0        0     1400 2023-04-24 09:24:54.000000 pylibCZIrw-3.4.0/_pylibCZIrw/src/bindings/PbHelper.cpp
--rw-rw-rw-   0        0        0     1736 2023-04-24 09:24:54.000000 pylibCZIrw-3.4.0/_pylibCZIrw/src/bindings/PbHelper.h
-drwxrwxrwx   0        0        0        0 2023-04-24 09:26:13.030737 pylibCZIrw-3.4.0/_pylibCZIrw/tests/
--rw-rw-rw-   0        0        0     1486 2023-04-24 09:24:54.000000 pylibCZIrw-3.4.0/_pylibCZIrw/tests/main.cpp
-drwxrwxrwx   0        0        0        0 2023-04-24 09:26:13.015117 pylibCZIrw-3.4.0/libs/
-drwxrwxrwx   0        0        0        0 2023-04-24 09:26:13.046375 pylibCZIrw-3.4.0/libs/libCZIrw/
--rw-rw-rw-   0        0        0     3111 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/.editorconfig
--rw-rw-rw-   0        0        0       41 2023-04-24 09:25:00.000000 pylibCZIrw-3.4.0/libs/libCZIrw/.git
-drwxrwxrwx   0        0        0        0 2023-04-24 09:26:13.046375 pylibCZIrw-3.4.0/libs/libCZIrw/.github/
-drwxrwxrwx   0        0        0        0 2023-04-24 09:26:13.046375 pylibCZIrw-3.4.0/libs/libCZIrw/.github/ISSUE_TEMPLATE/
--rw-rw-rw-   0        0        0      872 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/.github/ISSUE_TEMPLATE/bug_report.md
--rw-rw-rw-   0        0        0      615 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/.github/ISSUE_TEMPLATE/feature_request.md
--rw-rw-rw-   0        0        0     1409 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/.github/PULL_REQUEST_TEMPLATE.md
--rw-rw-rw-   0        0        0      469 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/.github/codecov.yml
-drwxrwxrwx   0        0        0        0 2023-04-24 09:26:13.046375 pylibCZIrw-3.4.0/libs/libCZIrw/.github/workflows/
--rw-rw-rw-   0        0        0      858 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/.github/workflows/cla.yml
--rw-rw-rw-   0        0        0     4038 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/.github/workflows/cmake.yml
--rw-rw-rw-   0        0        0     2129 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/.github/workflows/codeql.yml
--rw-rw-rw-   0        0        0     1193 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/.github/workflows/mega-linter.yml
--rw-rw-rw-   0        0        0     1374 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/.github/workflows/pages.yml
--rw-rw-rw-   0        0        0      296 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/.github/workflows/reuse.yml
--rw-rw-rw-   0        0        0     5464 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/.gitignore
--rw-rw-rw-   0        0        0      735 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/.mega-linter.yml
-drwxrwxrwx   0        0        0        0 2023-04-24 09:26:13.046375 pylibCZIrw-3.4.0/libs/libCZIrw/.reuse/
--rw-rw-rw-   0        0        0      712 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/.reuse/dep5
--rw-rw-rw-   0        0        0     4357 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/CMakeLists.txt
--rw-rw-rw-   0        0        0     5501 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/CODE_OF_CONDUCT.md
--rw-rw-rw-   0        0        0     2687 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/CONTRIBUTING.md
--rw-rw-rw-   0        0        0    35819 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/COPYING
--rw-rw-rw-   0        0        0     7815 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/COPYING.LESSER
--rw-rw-rw-   0        0        0      973 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/CPPLINT.cfg
-drwxrwxrwx   0        0        0        0 2023-04-24 09:26:13.077633 pylibCZIrw-3.4.0/libs/libCZIrw/LICENSES/
--rw-rw-rw-   0        0        0     1471 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/LICENSES/BSD-3-Clause.txt
--rw-rw-rw-   0        0        0     7169 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/LICENSES/CC0-1.0.txt
--rw-rw-rw-   0        0        0    42402 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/LICENSES/LGPL-3.0-or-later.txt
--rw-rw-rw-   0        0        0     1087 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/LICENSES/MIT.txt
--rw-rw-rw-   0        0        0      878 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/LICENSES/RSA-MD.txt
--rw-rw-rw-   0        0        0     4249 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/README.md
--rw-rw-rw-   0        0        0      587 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/SECURITY.md
-drwxrwxrwx   0        0        0        0 2023-04-24 09:26:13.077633 pylibCZIrw-3.4.0/libs/libCZIrw/Src/
--rw-rw-rw-   0        0        0      491 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/Src/CMakeLists.txt
--rw-rw-rw-   0        0        0   127198 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/Src/Doxyfile
-drwxrwxrwx   0        0        0        0 2023-04-24 09:26:13.077633 pylibCZIrw-3.4.0/libs/libCZIrw/Src/JxrDecode/
--rw-rw-rw-   0        0        0     2137 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/Src/JxrDecode/CMakeLists.txt
-drwxrwxrwx   0        0        0        0 2023-04-24 09:26:13.140122 pylibCZIrw-3.4.0/libs/libCZIrw/Src/JxrDecode/Jxr/
--rw-rw-rw-   0        0        0    32942 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/Src/JxrDecode/Jxr/JXRGlue.c
--rw-rw-rw-   0        0        0    30331 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/Src/JxrDecode/Jxr/JXRGlue.h
--rw-rw-rw-   0        0        0    82146 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/Src/JxrDecode/Jxr/JXRGlueJxr.c
--rw-rw-rw-   0        0        0    71573 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/Src/JxrDecode/Jxr/JXRGluePFC.c
--rw-rw-rw-   0        0        0    29194 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/Src/JxrDecode/Jxr/JXRMeta.c
--rw-rw-rw-   0        0        0     9173 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/Src/JxrDecode/Jxr/JXRMeta.h
--rw-rw-rw-   0        0        0     9805 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/Src/JxrDecode/Jxr/JXRTest.c
--rw-rw-rw-   0        0        0     5731 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/Src/JxrDecode/Jxr/JXRTest.h
--rw-rw-rw-   0        0        0    12746 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/Src/JxrDecode/Jxr/JXRTestBmp.c
--rw-rw-rw-   0        0        0     7415 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/Src/JxrDecode/Jxr/JXRTestHdr.c
--rw-rw-rw-   0        0        0     9754 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/Src/JxrDecode/Jxr/JXRTestPnm.c
--rw-rw-rw-   0        0        0    28100 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/Src/JxrDecode/Jxr/JXRTestTif.c
--rw-rw-rw-   0        0        0     1208 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/Src/JxrDecode/Jxr/JXRTestWrapper.c
--rw-rw-rw-   0        0        0      392 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/Src/JxrDecode/Jxr/JXRTestWrapper.h
--rw-rw-rw-   0        0        0    15650 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/Src/JxrDecode/Jxr/JXRTestYUV.c
--rw-rw-rw-   0        0        0    46751 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/Src/JxrDecode/Jxr/JXRTranscode.c
-drwxrwxrwx   0        0        0        0 2023-04-24 09:26:13.140122 pylibCZIrw-3.4.0/libs/libCZIrw/Src/JxrDecode/Jxr/_x86/
--rw-rw-rw-   0        0        0     2257 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/Src/JxrDecode/Jxr/_x86/_x86.h
--rw-rw-rw-   0        0        0    13119 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/Src/JxrDecode/Jxr/adapthuff.c
--rw-rw-rw-   0        0        0     2308 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/Src/JxrDecode/Jxr/ansi.h
--rw-rw-rw-   0        0        0     4875 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/Src/JxrDecode/Jxr/common.h
--rw-rw-rw-   0        0        0     6826 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/Src/JxrDecode/Jxr/decode.c
--rw-rw-rw-   0        0        0     5183 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/Src/JxrDecode/Jxr/decode.h
--rw-rw-rw-   0        0        0     5517 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/Src/JxrDecode/Jxr/encode.c
--rw-rw-rw-   0        0        0     4300 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/Src/JxrDecode/Jxr/encode.h
--rw-rw-rw-   0        0        0     6285 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/Src/JxrDecode/Jxr/image.c
--rw-rw-rw-   0        0        0       54 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/Src/JxrDecode/Jxr/jxr_defines.h
--rw-rw-rw-   0        0        0     5274 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/Src/JxrDecode/Jxr/perfTimer.h
--rw-rw-rw-   0        0        0     7657 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/Src/JxrDecode/Jxr/perfTimerANSI.c
--rw-rw-rw-   0        0        0    10556 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/Src/JxrDecode/Jxr/postprocess.c
--rw-rw-rw-   0        0        0     6484 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/Src/JxrDecode/Jxr/priv_guiddef.h
--rw-rw-rw-   0        0        0    44116 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/Src/JxrDecode/Jxr/segdec.c
--rw-rw-rw-   0        0        0    44265 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/Src/JxrDecode/Jxr/segenc.c
--rw-rw-rw-   0        0        0    38303 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/Src/JxrDecode/Jxr/strFwdTransform.c
--rw-rw-rw-   0        0        0    68724 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/Src/JxrDecode/Jxr/strInvTransform.c
--rw-rw-rw-   0        0        0    10644 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/Src/JxrDecode/Jxr/strPredQuant.c
--rw-rw-rw-   0        0        0    18412 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/Src/JxrDecode/Jxr/strPredQuantDec.c
--rw-rw-rw-   0        0        0    18645 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/Src/JxrDecode/Jxr/strPredQuantEnc.c
--rw-rw-rw-   0        0        0     2629 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/Src/JxrDecode/Jxr/strTransform.c
--rw-rw-rw-   0        0        0     2387 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/Src/JxrDecode/Jxr/strTransform.h
--rw-rw-rw-   0        0        0    39625 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/Src/JxrDecode/Jxr/strcodec.c
--rw-rw-rw-   0        0        0    23294 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/Src/JxrDecode/Jxr/strcodec.h
--rw-rw-rw-   0        0        0   151177 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/Src/JxrDecode/Jxr/strdec.c
--rw-rw-rw-   0        0        0    51843 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/Src/JxrDecode/Jxr/strdec_x86.c
--rw-rw-rw-   0        0        0    98067 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/Src/JxrDecode/Jxr/strenc.c
--rw-rw-rw-   0        0        0    12654 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/Src/JxrDecode/Jxr/strenc_x86.c
--rw-rw-rw-   0        0        0    16567 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/Src/JxrDecode/Jxr/windowsmediaphoto.h
--rw-rw-rw-   0        0        0    45861 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/Src/JxrDecode/Jxr/wmsal.h
--rw-rw-rw-   0        0        0    23441 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/Src/JxrDecode/Jxr/wmspecstring.h
--rw-rw-rw-   0        0        0     3295 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/Src/JxrDecode/Jxr/wmspecstrings_adt.h
--rw-rw-rw-   0        0        0    57847 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/Src/JxrDecode/Jxr/wmspecstrings_strict.h
--rw-rw-rw-   0        0        0    12055 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/Src/JxrDecode/Jxr/wmspecstrings_undef.h
--rw-rw-rw-   0        0        0    20032 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/Src/JxrDecode/JxrDecode.cpp
--rw-rw-rw-   0        0        0     4710 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/Src/JxrDecode/JxrDecode.h
--rw-rw-rw-   0        0        0      414 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/Src/JxrDecode/stdafx.cpp
--rw-rw-rw-   0        0        0      489 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/Src/JxrDecode/stdafx.h
--rw-rw-rw-   0        0        0      478 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/Src/JxrDecode/targetver.h
-drwxrwxrwx   0        0        0        0 2023-04-24 09:26:13.218258 pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/
--rw-rw-rw-   0        0        0    16162 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/BitmapOperations.cpp
--rw-rw-rw-   0        0        0     4290 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/BitmapOperations.h
--rw-rw-rw-   0        0        0    22586 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/BitmapOperations.hpp
--rw-rw-rw-   0        0        0    11504 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/CMakeLists.txt
--rw-rw-rw-   0        0        0    12124 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/CZIReader.cpp
--rw-rw-rw-   0        0        0     2892 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/CZIReader.h
--rw-rw-rw-   0        0        0     3460 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/CreateBitmap.cpp
--rw-rw-rw-   0        0        0     1074 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/CziAttachment.cpp
--rw-rw-rw-   0        0        0      804 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/CziAttachment.h
--rw-rw-rw-   0        0        0     5295 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/CziAttachmentsDirectory.cpp
--rw-rw-rw-   0        0        0     2614 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/CziAttachmentsDirectory.h
--rw-rw-rw-   0        0        0     6292 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/CziDimensionInfo.cpp
--rw-rw-rw-   0        0        0     3447 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/CziDimensionInfo.h
--rw-rw-rw-   0        0        0    14592 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/CziDisplaySettings.cpp
--rw-rw-rw-   0        0        0     1867 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/CziDisplaySettings.h
--rw-rw-rw-   0        0        0     7046 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/CziMetadata.cpp
--rw-rw-rw-   0        0        0     1720 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/CziMetadata.h
--rw-rw-rw-   0        0        0    37291 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/CziMetadataBuilder.cpp
--rw-rw-rw-   0        0        0     4939 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/CziMetadataBuilder.h
--rw-rw-rw-   0        0        0    16544 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/CziMetadataDocumentInfo.cpp
--rw-rw-rw-   0        0        0     1522 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/CziMetadataDocumentInfo.h
--rw-rw-rw-   0        0        0    71850 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/CziMetadataDocumentInfo2.cpp
--rw-rw-rw-   0        0        0    41047 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/CziMetadataDocumentInfo2.h
--rw-rw-rw-   0        0        0     1689 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/CziMetadataSegment.cpp
--rw-rw-rw-   0        0        0      773 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/CziMetadataSegment.h
--rw-rw-rw-   0        0        0    32912 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/CziParse.cpp
--rw-rw-rw-   0        0        0     4854 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/CziParse.h
--rw-rw-rw-   0        0        0    37315 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/CziReaderWriter.cpp
--rw-rw-rw-   0        0        0     7881 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/CziReaderWriter.h
--rw-rw-rw-   0        0        0     7183 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/CziStructs.cpp
--rw-rw-rw-   0        0        0     9361 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/CziStructs.h
--rw-rw-rw-   0        0        0     2279 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/CziSubBlock.cpp
--rw-rw-rw-   0        0        0     1001 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/CziSubBlock.h
--rw-rw-rw-   0        0        0    22081 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/CziSubBlockDirectory.cpp
--rw-rw-rw-   0        0        0     6513 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/CziSubBlockDirectory.h
--rw-rw-rw-   0        0        0     6163 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/CziUtils.cpp
--rw-rw-rw-   0        0        0     2342 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/CziUtils.h
--rw-rw-rw-   0        0        0    59642 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/CziWriter.cpp
--rw-rw-rw-   0        0        0    16511 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/CziWriter.h
--rw-rw-rw-   0        0        0     8038 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/DimCoordinate.cpp
-drwxrwxrwx   0        0        0        0 2023-04-24 09:26:13.233888 pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/Doc/
--rw-rw-rw-   0        0        0    25621 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/Doc/CZICmd_usage.markdown
-drwxrwxrwx   0        0        0        0 2023-04-24 09:26:13.280743 pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/Doc/Images/
--rw-rw-rw-   0        0        0    15042 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/Doc/Images/CZI_1.PNG
--rw-rw-rw-   0        0        0    11631 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/Doc/Images/CZI_2.PNG
--rw-rw-rw-   0        0        0   629984 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/Doc/Images/ScalingSingleChannelTileAccessor1.png
--rw-rw-rw-   0        0        0    15606 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/Doc/Images/SingleChannelTileAccessor_1.PNG
--rw-rw-rw-   0        0        0     6597 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/Doc/Images/SingleChannelTileAccessor_2.PNG
--rw-rw-rw-   0        0        0   508732 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/Doc/Images/SingleChannelTileAccessor_3.PNG
--rw-rw-rw-   0        0        0   435548 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/Doc/Images/SingleChannelTileAccessor_4.PNG
--rw-rw-rw-   0        0        0    22752 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/Doc/Images/Tinting-LUT.png
--rw-rw-rw-   0        0        0    95014 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/Doc/Images/VisualStudio_cmake1.png
--rw-rw-rw-   0        0        0   947057 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/Doc/Images/ZEN_screenshot_1.PNG
--rw-rw-rw-   0        0        0   149904 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/Doc/Images/ZEN_screenshot_2.PNG
--rw-rw-rw-   0        0        0   242149 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/Doc/Images/cmake_1_raspi.PNG
--rw-rw-rw-   0        0        0    32954 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/Doc/Images/cmake_1_raspi_help_freetype.PNG
--rw-rw-rw-   0        0        0   270106 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/Doc/Images/cmake_install_raspi1.PNG
--rw-rw-rw-   0        0        0    59883 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/Doc/Images/cmake_raspi_unittests_1.PNG
--rw-rw-rw-   0        0        0    14602 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/Doc/Images/compositors_1.png
--rw-rw-rw-   0        0        0     4107 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/Doc/Images/compositors_2.png
-drwxrwxrwx   0        0        0        0 2023-04-24 09:26:13.280743 pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/Doc/Images/drawings/
--rw-rw-rw-   0        0        0   100864 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/Doc/Images/drawings/VS-project.pub
--rw-rw-rw-   0        0        0   108032 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/Doc/Images/drawings/VS-project_2.pub
--rw-rw-rw-   0        0        0    10567 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/Doc/Images/gradationcurve_1.PNG
--rw-rw-rw-   0        0        0     8316 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/Doc/Images/gradationcurve_2.PNG
--rw-rw-rw-   0        0        0     7632 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/Doc/Images/image_document_concept1.PNG
--rw-rw-rw-   0        0        0    20658 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/Doc/Images/image_document_concept2.PNG
--rw-rw-rw-   0        0        0    14836 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/Doc/Images/image_document_concept3.PNG
--rw-rw-rw-   0        0        0    29100 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/Doc/Images/image_document_concept4.PNG
--rw-rw-rw-   0        0        0     1966 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/Doc/Todos.markdown
--rw-rw-rw-   0        0        0     2964 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/Doc/accessors.markdown
--rw-rw-rw-   0        0        0     3020 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/Doc/building_libCZI.markdown
--rw-rw-rw-   0        0        0    92375 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/Doc/drawings.docx
--rw-rw-rw-   0        0        0     3983 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/Doc/image_document_concept.markdown
--rw-rw-rw-   0        0        0     5655 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/Doc/mainpage.markdown
--rw-rw-rw-   0        0        0     2275 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/Doc/multichannelcomposition.markdown
--rw-rw-rw-   0        0        0    11134 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/Doc/using_libCZI.markdown
--rw-rw-rw-   0        0        0     5534 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/Doc/write_czi.markdown
--rw-rw-rw-   0        0        0     2521 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/FileHeaderSegmentData.h
--rw-rw-rw-   0        0        0      631 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/ImportExport.h
--rw-rw-rw-   0        0        0     5323 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/IndexSet.cpp
--rw-rw-rw-   0        0        0      992 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/IndexSet.h
--rw-rw-rw-   0        0        0     8801 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/MD5Sum.cpp
--rw-rw-rw-   0        0        0     5296 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/MD5Sum.h
--rw-rw-rw-   0        0        0    56461 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/MultiChannelCompositor.cpp
--rw-rw-rw-   0        0        0      166 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/MultiChannelCompositor.h
--rw-rw-rw-   0        0        0     3716 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/SingleChannelAccessorBase.cpp
--rw-rw-rw-   0        0        0      739 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/SingleChannelAccessorBase.h
--rw-rw-rw-   0        0        0    10906 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/SingleChannelPyramidLevelTileAccessor.cpp
--rw-rw-rw-   0        0        0     2835 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/SingleChannelPyramidLevelTileAccessor.h
--rw-rw-rw-   0        0        0    17451 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/SingleChannelScalingTileAccessor.cpp
--rw-rw-rw-   0        0        0     3176 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/SingleChannelScalingTileAccessor.h
--rw-rw-rw-   0        0        0     5437 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/SingleChannelTileAccessor.cpp
--rw-rw-rw-   0        0        0     2132 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/SingleChannelTileAccessor.h
--rw-rw-rw-   0        0        0     2084 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/SingleChannelTileCompositor.cpp
--rw-rw-rw-   0        0        0      333 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/SingleChannelTileCompositor.h
--rw-rw-rw-   0        0        0      187 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/Site.h
--rw-rw-rw-   0        0        0    20334 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/StreamImpl.cpp
--rw-rw-rw-   0        0        0     6093 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/StreamImpl.h
--rw-rw-rw-   0        0        0    10313 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/XmlNodeWrapper.h
--rw-rw-rw-   0        0        0     5713 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/bitmapData.h
--rw-rw-rw-   0        0        0     8206 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/decoder.cpp
--rw-rw-rw-   0        0        0      672 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/decoder.h
--rw-rw-rw-   0        0        0    17042 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/decoder_wic.cpp
--rw-rw-rw-   0        0        0      774 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/decoder_wic.h
--rw-rw-rw-   0        0        0     7689 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/decoder_zstd.cpp
--rw-rw-rw-   0        0        0      773 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/decoder_zstd.h
--rw-rw-rw-   0        0        0      264 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/inc_libCZI_Config.h
--rw-rw-rw-   0        0        0    35455 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/libCZI.h
--rw-rw-rw-   0        0        0    30887 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/libCZI_Compositor.h
--rw-rw-rw-   0        0        0     1997 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/libCZI_Config.h.in
--rw-rw-rw-   0        0        0    17832 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/libCZI_DimCoordinate.h
--rw-rw-rw-   0        0        0     9636 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/libCZI_Helpers.h
--rw-rw-rw-   0        0        0     4403 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/libCZI_Lib.cpp
--rw-rw-rw-   0        0        0    70229 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/libCZI_Metadata.h
--rw-rw-rw-   0        0        0    63505 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/libCZI_Metadata2.h
--rw-rw-rw-   0        0        0    13615 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/libCZI_Pixels.h
--rw-rw-rw-   0        0        0     9656 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/libCZI_ReadWrite.h
--rw-rw-rw-   0        0        0     5061 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/libCZI_Site.cpp
--rw-rw-rw-   0        0        0     6262 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/libCZI_Site.h
--rw-rw-rw-   0        0        0    24080 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/libCZI_Utilities.cpp
--rw-rw-rw-   0        0        0    19595 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/libCZI_Utilities.h
--rw-rw-rw-   0        0        0    32800 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/libCZI_Write.h
--rw-rw-rw-   0        0        0    40830 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/libCZI_compress.h
--rw-rw-rw-   0        0        0    14343 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/libCZI_exceptions.h
--rw-rw-rw-   0        0        0     6566 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/priv_guiddef.h
--rw-rw-rw-   0        0        0     3060 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/pugiconfig.hpp
--rw-rw-rw-   0        0        0   407937 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/pugixml.cpp
--rw-rw-rw-   0        0        0    60454 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/pugixml.hpp
--rw-rw-rw-   0        0        0     3364 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/splines.cpp
--rw-rw-rw-   0        0        0      554 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/splines.h
--rw-rw-rw-   0        0        0     1291 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/stdAllocator.cpp
--rw-rw-rw-   0        0        0      593 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/stdAllocator.h
--rw-rw-rw-   0        0        0      411 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/stdafx.cpp
--rw-rw-rw-   0        0        0      739 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/stdafx.h
--rw-rw-rw-   0        0        0      478 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/targetver.h
--rw-rw-rw-   0        0        0    12984 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/utilities.cpp
--rw-rw-rw-   0        0        0     5866 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/utilities.h
--rw-rw-rw-   0        0        0    12120 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/utilities_simd.cpp
--rw-rw-rw-   0        0        0    18595 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/zstdCompress.cpp
--rw-rw-rw-   0        0        0     6291 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/THIRD_PARTY_LICENSES.txt
--rw-rw-rw-   0        0        0     6882 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/cla_corporate.txt
--rw-rw-rw-   0        0        0     6571 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/cla_individual.txt
-drwxrwxrwx   0        0        0        0 2023-04-24 09:26:13.280743 pylibCZIrw-3.4.0/libs/libCZIrw/cmake/
--rw-rw-rw-   0        0        0      836 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/cmake/ExternalEIGEN3.cmake
--rw-rw-rw-   0        0        0     4609 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/cmake/TestLargeFile.cmake
--rw-rw-rw-   0        0        0     1842 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/cmake/check_can_use_neon_intrinsics.cmake
--rw-rw-rw-   0        0        0     2656 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/cmake/check_unaligned_access.cmake
--rw-rw-rw-   0        0        0      150 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/libCZIrw/opencppcoverage.txt
-drwxrwxrwx   0        0        0        0 2023-04-24 09:26:13.280743 pylibCZIrw-3.4.0/libs/pybind11/
--rw-rw-rw-   0        0        0     1341 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/.appveyor.yml
--rw-rw-rw-   0        0        0     1034 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/.clang-format
--rw-rw-rw-   0        0        0     2282 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/.clang-tidy
--rw-rw-rw-   0        0        0     2269 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/.cmake-format.yaml
--rw-rw-rw-   0        0        0       41 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/.git
-drwxrwxrwx   0        0        0        0 2023-04-24 09:26:13.296390 pylibCZIrw-3.4.0/libs/pybind11/.github/
--rw-rw-rw-   0        0        0      191 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/.github/CODEOWNERS
--rw-rw-rw-   0        0        0    15646 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/.github/CONTRIBUTING.md
-drwxrwxrwx   0        0        0        0 2023-04-24 09:26:13.296390 pylibCZIrw-3.4.0/libs/pybind11/.github/ISSUE_TEMPLATE/
--rw-rw-rw-   0        0        0     2061 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/.github/ISSUE_TEMPLATE/bug-report.yml
--rw-rw-rw-   0        0        0      336 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/.github/ISSUE_TEMPLATE/config.yml
--rw-rw-rw-   0        0        0      575 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/.github/dependabot.yml
--rw-rw-rw-   0        0        0      124 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/.github/labeler.yml
--rw-rw-rw-   0        0        0       53 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/.github/labeler_merged.yml
--rw-rw-rw-   0        0        0      664 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/.github/pull_request_template.md
-drwxrwxrwx   0        0        0        0 2023-04-24 09:26:13.296390 pylibCZIrw-3.4.0/libs/pybind11/.github/workflows/
--rw-rw-rw-   0        0        0    29190 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/.github/workflows/ci.yml
--rw-rw-rw-   0        0        0     2204 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/.github/workflows/configure.yml
--rw-rw-rw-   0        0        0     1262 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/.github/workflows/format.yml
--rw-rw-rw-   0        0        0      349 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/.github/workflows/labeler.yml
--rw-rw-rw-   0        0        0     2624 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/.github/workflows/pip.yml
--rw-rw-rw-   0        0        0     2936 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/.github/workflows/upstream.yml
--rw-rw-rw-   0        0        0      532 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/.gitignore
--rw-rw-rw-   0        0        0     3624 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/.pre-commit-config.yaml
--rw-rw-rw-   0        0        0       65 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/.readthedocs.yml
--rw-rw-rw-   0        0        0    11298 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/CMakeLists.txt
--rw-rw-rw-   0        0        0     1713 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/LICENSE
--rw-rw-rw-   0        0        0      262 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/MANIFEST.in
--rw-rw-rw-   0        0        0     7836 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/README.rst
-drwxrwxrwx   0        0        0        0 2023-04-24 09:26:13.314372 pylibCZIrw-3.4.0/libs/pybind11/docs/
--rw-rw-rw-   0        0        0      675 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/docs/Doxyfile
--rw-rw-rw-   0        0        0     7609 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/docs/Makefile
-drwxrwxrwx   0        0        0        0 2023-04-24 09:26:13.314372 pylibCZIrw-3.4.0/libs/pybind11/docs/_static/
--rw-rw-rw-   0        0        0      265 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/docs/_static/theme_overrides.css
-drwxrwxrwx   0        0        0        0 2023-04-24 09:26:13.314372 pylibCZIrw-3.4.0/libs/pybind11/docs/advanced/
-drwxrwxrwx   0        0        0        0 2023-04-24 09:26:13.327649 pylibCZIrw-3.4.0/libs/pybind11/docs/advanced/cast/
--rw-rw-rw-   0        0        0     4018 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/docs/advanced/cast/chrono.rst
--rw-rw-rw-   0        0        0     3502 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/docs/advanced/cast/custom.rst
--rw-rw-rw-   0        0        0    14593 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/docs/advanced/cast/eigen.rst
--rw-rw-rw-   0        0        0     3998 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/docs/advanced/cast/functional.rst
--rw-rw-rw-   0        0        0     1599 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/docs/advanced/cast/index.rst
--rw-rw-rw-   0        0        0    12604 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/docs/advanced/cast/overview.rst
--rw-rw-rw-   0        0        0     9954 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/docs/advanced/cast/stl.rst
--rw-rw-rw-   0        0        0     9668 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/docs/advanced/cast/strings.rst
--rw-rw-rw-   0        0        0    49668 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/docs/advanced/classes.rst
--rw-rw-rw-   0        0        0     8715 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/docs/advanced/embedding.rst
--rw-rw-rw-   0        0        0    18204 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/docs/advanced/exceptions.rst
--rw-rw-rw-   0        0        0    27442 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/docs/advanced/functions.rst
--rw-rw-rw-   0        0        0    12783 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/docs/advanced/misc.rst
-drwxrwxrwx   0        0        0        0 2023-04-24 09:26:13.327649 pylibCZIrw-3.4.0/libs/pybind11/docs/advanced/pycpp/
--rw-rw-rw-   0        0        0      291 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/docs/advanced/pycpp/index.rst
--rw-rw-rw-   0        0        0    17910 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/docs/advanced/pycpp/numpy.rst
--rw-rw-rw-   0        0        0     9316 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/docs/advanced/pycpp/object.rst
--rw-rw-rw-   0        0        0     5865 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/docs/advanced/pycpp/utilities.rst
--rw-rw-rw-   0        0        0     6541 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/docs/advanced/smart_ptrs.rst
--rw-rw-rw-   0        0        0     9676 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/docs/basics.rst
--rw-rw-rw-   0        0        0     3053 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/docs/benchmark.py
--rw-rw-rw-   0        0        0     3263 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/docs/benchmark.rst
--rw-rw-rw-   0        0        0   101394 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/docs/changelog.rst
--rw-rw-rw-   0        0        0    16993 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/docs/classes.rst
-drwxrwxrwx   0        0        0        0 2023-04-24 09:26:13.327649 pylibCZIrw-3.4.0/libs/pybind11/docs/cmake/
--rw-rw-rw-   0        0        0      281 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/docs/cmake/index.rst
--rw-rw-rw-   0        0        0    26915 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/docs/compiling.rst
--rw-rw-rw-   0        0        0    12463 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/docs/conf.py
--rw-rw-rw-   0        0        0    14942 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/docs/faq.rst
--rw-rw-rw-   0        0        0      661 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/docs/index.rst
--rw-rw-rw-   0        0        0     3382 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/docs/installing.rst
--rw-rw-rw-   0        0        0     3151 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/docs/limitations.rst
--rw-rw-rw-   0        0        0    58510 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/docs/pybind11-logo.png
--rw-rw-rw-   0        0        0    44653 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/docs/pybind11_vs_boost_python1.png
--rw-rw-rw-   0        0        0    88135 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/docs/pybind11_vs_boost_python1.svg
--rw-rw-rw-   0        0        0    41121 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/docs/pybind11_vs_boost_python2.png
--rw-rw-rw-   0        0        0    86280 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/docs/pybind11_vs_boost_python2.svg
--rw-rw-rw-   0        0        0     2777 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/docs/reference.rst
--rw-rw-rw-   0        0        0     4511 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/docs/release.rst
--rw-rw-rw-   0        0        0      135 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/docs/requirements.txt
--rw-rw-rw-   0        0        0    24043 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/docs/upgrade.rst
-drwxrwxrwx   0        0        0        0 2023-04-24 09:26:13.015117 pylibCZIrw-3.4.0/libs/pybind11/include/
-drwxrwxrwx   0        0        0        0 2023-04-24 09:26:13.343938 pylibCZIrw-3.4.0/libs/pybind11/include/pybind11/
--rw-rw-rw-   0        0        0    24595 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/include/pybind11/attr.h
--rw-rw-rw-   0        0        0     7262 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/include/pybind11/buffer_info.h
--rw-rw-rw-   0        0        0    66456 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/include/pybind11/cast.h
--rw-rw-rw-   0        0        0     9143 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/include/pybind11/chrono.h
--rw-rw-rw-   0        0        0      122 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/include/pybind11/common.h
--rw-rw-rw-   0        0        0     2170 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/include/pybind11/complex.h
-drwxrwxrwx   0        0        0        0 2023-04-24 09:26:13.358881 pylibCZIrw-3.4.0/libs/pybind11/include/pybind11/detail/
--rw-rw-rw-   0        0        0    29274 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/include/pybind11/detail/class.h
--rw-rw-rw-   0        0        0    52865 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/include/pybind11/detail/common.h
--rw-rw-rw-   0        0        0     5649 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/include/pybind11/detail/descr.h
--rw-rw-rw-   0        0        0    18399 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/include/pybind11/detail/init.h
--rw-rw-rw-   0        0        0    24768 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/include/pybind11/detail/internals.h
--rw-rw-rw-   0        0        0    45497 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/include/pybind11/detail/type_caster_base.h
--rw-rw-rw-   0        0        0     1572 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/include/pybind11/detail/typeid.h
--rw-rw-rw-   0        0        0    32140 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/include/pybind11/eigen.h
--rw-rw-rw-   0        0        0    12477 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/include/pybind11/embed.h
--rw-rw-rw-   0        0        0     5767 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/include/pybind11/eval.h
--rw-rw-rw-   0        0        0     4886 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/include/pybind11/functional.h
--rw-rw-rw-   0        0        0     7050 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/include/pybind11/gil.h
--rw-rw-rw-   0        0        0     9116 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/include/pybind11/iostream.h
--rw-rw-rw-   0        0        0    79994 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/include/pybind11/numpy.h
--rw-rw-rw-   0        0        0    10001 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/include/pybind11/operators.h
--rw-rw-rw-   0        0        0     2257 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/include/pybind11/options.h
--rw-rw-rw-   0        0        0   128798 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/include/pybind11/pybind11.h
--rw-rw-rw-   0        0        0    83054 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/include/pybind11/pytypes.h
-drwxrwxrwx   0        0        0        0 2023-04-24 09:26:13.358881 pylibCZIrw-3.4.0/libs/pybind11/include/pybind11/stl/
--rw-rw-rw-   0        0        0     3654 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/include/pybind11/stl/filesystem.h
--rw-rw-rw-   0        0        0    14860 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/include/pybind11/stl.h
--rw-rw-rw-   0        0        0    27777 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/include/pybind11/stl_bind.h
--rw-rw-rw-   0        0        0     2667 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/noxfile.py
-drwxrwxrwx   0        0        0        0 2023-04-24 09:26:13.358881 pylibCZIrw-3.4.0/libs/pybind11/pybind11/
--rw-rw-rw-   0        0        0      227 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/pybind11/__init__.py
--rw-rw-rw-   0        0        0     1210 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/pybind11/__main__.py
--rw-rw-rw-   0        0        0      214 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/pybind11/_version.py
--rw-rw-rw-   0        0        0      143 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/pybind11/_version.pyi
--rw-rw-rw-   0        0        0      683 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/pybind11/commands.py
--rw-rw-rw-   0        0        0        0 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/pybind11/py.typed
--rw-rw-rw-   0        0        0    17977 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/pybind11/setup_helpers.py
--rw-rw-rw-   0        0        0     2101 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/pybind11/setup_helpers.pyi
--rw-rw-rw-   0        0        0      998 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/pyproject.toml
--rw-rw-rw-   0        0        0     1973 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/setup.cfg
--rw-rw-rw-   0        0        0     5222 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-24 09:26:13.640135 pylibCZIrw-3.4.0/libs/pybind11/tests/
--rw-rw-rw-   0        0        0    21668 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/tests/CMakeLists.txt
--rw-rw-rw-   0        0        0     5049 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/tests/conftest.py
--rw-rw-rw-   0        0        0    12056 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/tests/constructor_stats.h
--rw-rw-rw-   0        0        0     1845 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/tests/cross_module_gil_utils.cpp
--rw-rw-rw-   0        0        0     1055 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/tests/env.py
-drwxrwxrwx   0        0        0        0 2023-04-24 09:26:13.640135 pylibCZIrw-3.4.0/libs/pybind11/tests/extra_python_package/
--rw-rw-rw-   0        0        0        0 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/tests/extra_python_package/pytest.ini
--rw-rw-rw-   0        0        0     7857 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/tests/extra_python_package/test_files.py
-drwxrwxrwx   0        0        0        0 2023-04-24 09:26:13.640135 pylibCZIrw-3.4.0/libs/pybind11/tests/extra_setuptools/
--rw-rw-rw-   0        0        0        0 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/tests/extra_setuptools/pytest.ini
--rw-rw-rw-   0        0        0     4372 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/tests/extra_setuptools/test_setuphelper.py
--rw-rw-rw-   0        0        0     2939 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/tests/local_bindings.h
--rw-rw-rw-   0        0        0     5948 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/tests/object.h
--rw-rw-rw-   0        0        0     6413 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/tests/pybind11_cross_module_tests.cpp
--rw-rw-rw-   0        0        0     3778 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/tests/pybind11_tests.cpp
--rw-rw-rw-   0        0        0     3109 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/tests/pybind11_tests.h
--rw-rw-rw-   0        0        0      712 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/tests/pytest.ini
--rw-rw-rw-   0        0        0      889 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/tests/requirements.txt
--rw-rw-rw-   0        0        0      880 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/tests/test_async.cpp
--rw-rw-rw-   0        0        0      583 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/tests/test_async.py
--rw-rw-rw-   0        0        0     8791 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/tests/test_buffers.cpp
--rw-rw-rw-   0        0        0     5222 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/tests/test_buffers.py
--rw-rw-rw-   0        0        0    16257 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/tests/test_builtin_casters.cpp
--rw-rw-rw-   0        0        0    18922 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/tests/test_builtin_casters.py
--rw-rw-rw-   0        0        0     4233 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/tests/test_call_policies.cpp
--rw-rw-rw-   0        0        0     6821 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/tests/test_call_policies.py
--rw-rw-rw-   0        0        0     9486 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/tests/test_callbacks.cpp
--rw-rw-rw-   0        0        0     6246 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/tests/test_callbacks.py
--rw-rw-rw-   0        0        0     3451 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/tests/test_chrono.cpp
--rw-rw-rw-   0        0        0     5937 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/tests/test_chrono.py
--rw-rw-rw-   0        0        0    24441 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/tests/test_class.cpp
--rw-rw-rw-   0        0        0    14981 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/tests/test_class.py
-drwxrwxrwx   0        0        0        0 2023-04-24 09:26:13.640135 pylibCZIrw-3.4.0/libs/pybind11/tests/test_cmake_build/
--rw-rw-rw-   0        0        0     2723 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/tests/test_cmake_build/CMakeLists.txt
--rw-rw-rw-   0        0        0      696 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/tests/test_cmake_build/embed.cpp
-drwxrwxrwx   0        0        0        0 2023-04-24 09:26:13.640135 pylibCZIrw-3.4.0/libs/pybind11/tests/test_cmake_build/installed_embed/
--rw-rw-rw-   0        0        0     1199 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/tests/test_cmake_build/installed_embed/CMakeLists.txt
-drwxrwxrwx   0        0        0        0 2023-04-24 09:26:13.640135 pylibCZIrw-3.4.0/libs/pybind11/tests/test_cmake_build/installed_function/
--rw-rw-rw-   0        0        0     1332 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/tests/test_cmake_build/installed_function/CMakeLists.txt
-drwxrwxrwx   0        0        0        0 2023-04-24 09:26:13.640135 pylibCZIrw-3.4.0/libs/pybind11/tests/test_cmake_build/installed_target/
--rw-rw-rw-   0        0        0     1731 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/tests/test_cmake_build/installed_target/CMakeLists.txt
--rw-rw-rw-   0        0        0      158 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/tests/test_cmake_build/main.cpp
-drwxrwxrwx   0        0        0        0 2023-04-24 09:26:13.640135 pylibCZIrw-3.4.0/libs/pybind11/tests/test_cmake_build/subdirectory_embed/
--rw-rw-rw-   0        0        0     1394 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/tests/test_cmake_build/subdirectory_embed/CMakeLists.txt
-drwxrwxrwx   0        0        0        0 2023-04-24 09:26:13.640135 pylibCZIrw-3.4.0/libs/pybind11/tests/test_cmake_build/subdirectory_function/
--rw-rw-rw-   0        0        0     1198 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/tests/test_cmake_build/subdirectory_function/CMakeLists.txt
-drwxrwxrwx   0        0        0        0 2023-04-24 09:26:13.640135 pylibCZIrw-3.4.0/libs/pybind11/tests/test_cmake_build/subdirectory_target/
--rw-rw-rw-   0        0        0     1409 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/tests/test_cmake_build/subdirectory_target/CMakeLists.txt
--rw-rw-rw-   0        0        0      283 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/tests/test_cmake_build/test.py
--rw-rw-rw-   0        0        0     4324 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/tests/test_const_name.cpp
--rw-rw-rw-   0        0        0      681 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/tests/test_const_name.py
--rw-rw-rw-   0        0        0     6096 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/tests/test_constants_and_functions.cpp
--rw-rw-rw-   0        0        0     1575 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/tests/test_constants_and_functions.py
--rw-rw-rw-   0        0        0    11010 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/tests/test_copy_move.cpp
--rw-rw-rw-   0        0        0     4772 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/tests/test_copy_move.py
--rw-rw-rw-   0        0        0     7419 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/tests/test_custom_type_casters.cpp
--rw-rw-rw-   0        0        0     4209 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/tests/test_custom_type_casters.py
--rw-rw-rw-   0        0        0     1300 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/tests/test_custom_type_setup.cpp
--rw-rw-rw-   0        0        0     1164 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/tests/test_custom_type_setup.py
--rw-rw-rw-   0        0        0     2904 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/tests/test_docstring_options.cpp
--rw-rw-rw-   0        0        0     1672 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/tests/test_docstring_options.py
--rw-rw-rw-   0        0        0    18570 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/tests/test_eigen.cpp
--rw-rw-rw-   0        0        0    29054 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/tests/test_eigen.py
-drwxrwxrwx   0        0        0        0 2023-04-24 09:26:13.655751 pylibCZIrw-3.4.0/libs/pybind11/tests/test_embed/
--rw-rw-rw-   0        0        0     1845 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/tests/test_embed/CMakeLists.txt
--rw-rw-rw-   0        0        0      760 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/tests/test_embed/catch.cpp
--rw-rw-rw-   0        0        0      563 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/tests/test_embed/external_module.cpp
--rw-rw-rw-   0        0        0    14573 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/tests/test_embed/test_interpreter.cpp
--rw-rw-rw-   0        0        0      295 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/tests/test_embed/test_interpreter.py
--rw-rw-rw-   0        0        0      318 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/tests/test_embed/test_trampoline.py
--rw-rw-rw-   0        0        0     5855 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/tests/test_enum.cpp
--rw-rw-rw-   0        0        0     9404 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/tests/test_enum.py
--rw-rw-rw-   0        0        0     3286 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/tests/test_eval.cpp
--rw-rw-rw-   0        0        0     1234 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/tests/test_eval.py
--rw-rw-rw-   0        0        0      148 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/tests/test_eval_call.py
--rw-rw-rw-   0        0        0    10502 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/tests/test_exceptions.cpp
--rw-rw-rw-   0        0        0      412 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/tests/test_exceptions.h
--rw-rw-rw-   0        0        0     9313 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/tests/test_exceptions.py
--rw-rw-rw-   0        0        0    18856 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/tests/test_factory_constructors.cpp
--rw-rw-rw-   0        0        0    17251 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/tests/test_factory_constructors.py
--rw-rw-rw-   0        0        0     1720 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/tests/test_gil_scoped.cpp
--rw-rw-rw-   0        0        0     3222 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/tests/test_gil_scoped.py
--rw-rw-rw-   0        0        0     4252 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/tests/test_iostream.cpp
--rw-rw-rw-   0        0        0     8289 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/tests/test_iostream.py
--rw-rw-rw-   0        0        0     9509 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/tests/test_kwargs_and_defaults.cpp
--rw-rw-rw-   0        0        0    14391 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/tests/test_kwargs_and_defaults.py
--rw-rw-rw-   0        0        0     4507 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/tests/test_local_bindings.cpp
--rw-rw-rw-   0        0        0     8358 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/tests/test_local_bindings.py
--rw-rw-rw-   0        0        0    21786 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/tests/test_methods_and_attributes.cpp
--rw-rw-rw-   0        0        0    18329 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/tests/test_methods_and_attributes.py
--rw-rw-rw-   0        0        0     4144 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/tests/test_modules.cpp
--rw-rw-rw-   0        0        0     2935 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/tests/test_modules.py
--rw-rw-rw-   0        0        0    12646 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/tests/test_multiple_inheritance.cpp
--rw-rw-rw-   0        0        0    12530 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/tests/test_multiple_inheritance.py
--rw-rw-rw-   0        0        0    20298 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/tests/test_numpy_array.cpp
--rw-rw-rw-   0        0        0    20932 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/tests/test_numpy_array.py
--rw-rw-rw-   0        0        0    20739 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/tests/test_numpy_dtypes.cpp
--rw-rw-rw-   0        0        0    14477 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/tests/test_numpy_dtypes.py
--rw-rw-rw-   0        0        0     4568 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/tests/test_numpy_vectorize.cpp
--rw-rw-rw-   0        0        0     9977 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/tests/test_numpy_vectorize.py
--rw-rw-rw-   0        0        0     2854 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/tests/test_opaque_types.cpp
--rw-rw-rw-   0        0        0     1966 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/tests/test_opaque_types.py
--rw-rw-rw-   0        0        0     9751 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/tests/test_operator_overloading.cpp
--rw-rw-rw-   0        0        0     4547 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/tests/test_operator_overloading.py
--rw-rw-rw-   0        0        0     6841 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/tests/test_pickling.cpp
--rw-rw-rw-   0        0        0     2368 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/tests/test_pickling.py
--rw-rw-rw-   0        0        0    21430 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/tests/test_pytypes.cpp
--rw-rw-rw-   0        0        0    19669 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/tests/test_pytypes.py
--rw-rw-rw-   0        0        0    21142 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/tests/test_sequences_and_iterators.cpp
--rw-rw-rw-   0        0        0     8312 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/tests/test_sequences_and_iterators.py
--rw-rw-rw-   0        0        0    19514 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/tests/test_smart_ptr.cpp
--rw-rw-rw-   0        0        0     9938 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/tests/test_smart_ptr.py
--rw-rw-rw-   0        0        0    21250 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/tests/test_stl.cpp
--rw-rw-rw-   0        0        0    12020 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/tests/test_stl.py
--rw-rw-rw-   0        0        0     4774 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/tests/test_stl_binders.cpp
--rw-rw-rw-   0        0        0     8389 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/tests/test_stl_binders.py
--rw-rw-rw-   0        0        0     4744 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/tests/test_tagbased_polymorphic.cpp
--rw-rw-rw-   0        0        0      794 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/tests/test_tagbased_polymorphic.py
--rw-rw-rw-   0        0        0     1921 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/tests/test_thread.cpp
--rw-rw-rw-   0        0        0      919 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/tests/test_thread.py
--rw-rw-rw-   0        0        0      625 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/tests/test_union.cpp
--rw-rw-rw-   0        0        0      181 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/tests/test_union.py
--rw-rw-rw-   0        0        0    23695 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/tests/test_virtual_functions.cpp
--rw-rw-rw-   0        0        0    13606 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/tests/test_virtual_functions.py
--rw-rw-rw-   0        0        0     3366 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/tests/valgrind-numpy-scipy.supp
--rw-rw-rw-   0        0        0     2774 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/tests/valgrind-python.supp
-drwxrwxrwx   0        0        0        0 2023-04-24 09:26:13.671386 pylibCZIrw-3.4.0/libs/pybind11/tools/
--rw-rw-rw-   0        0        0     2422 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/tools/FindCatch.cmake
--rw-rw-rw-   0        0        0     3191 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/tools/FindEigen3.cmake
--rw-rw-rw-   0        0        0    10648 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/tools/FindPythonLibsNew.cmake
--rw-rw-rw-   0        0        0     1467 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/tools/check-style.sh
--rw-rw-rw-   0        0        0      975 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/tools/cmake_uninstall.cmake.in
--rw-rw-rw-   0        0        0     1161 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/tools/libsize.py
--rw-rw-rw-   0        0        0     1370 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/tools/make_changelog.py
--rw-rw-rw-   0        0        0    14990 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/tools/pybind11Common.cmake
--rw-rw-rw-   0        0        0     7296 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/tools/pybind11Config.cmake.in
--rw-rw-rw-   0        0        0     9951 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/tools/pybind11NewTools.cmake
--rw-rw-rw-   0        0        0     7666 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/tools/pybind11Tools.cmake
--rw-rw-rw-   0        0        0       97 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/tools/pyproject.toml
--rw-rw-rw-   0        0        0     2016 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/tools/setup_global.py.in
--rw-rw-rw-   0        0        0     1130 2023-04-24 09:25:03.000000 pylibCZIrw-3.4.0/libs/pybind11/tools/setup_main.py.in
-drwxrwxrwx   0        0        0        0 2023-04-24 09:26:13.671386 pylibCZIrw-3.4.0/pylibCZIrw/
--rw-rw-rw-   0        0        0      896 2023-04-24 09:24:55.000000 pylibCZIrw-3.4.0/pylibCZIrw/__init__.py
--rw-rw-rw-   0        0        0    44330 2023-04-24 09:24:55.000000 pylibCZIrw-3.4.0/pylibCZIrw/czi.py
--rw-rw-rw-   0        0        0   578662 2023-04-24 09:24:55.000000 pylibCZIrw-3.4.0/pylibCZIrw-documentation.html
-drwxrwxrwx   0        0        0        0 2023-04-24 09:26:13.671386 pylibCZIrw-3.4.0/pylibCZIrw.egg-info/
--rw-rw-rw-   0        0        0     3026 2023-04-24 09:26:12.000000 pylibCZIrw-3.4.0/pylibCZIrw.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    20816 2023-04-24 09:26:12.000000 pylibCZIrw-3.4.0/pylibCZIrw.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-24 09:26:12.000000 pylibCZIrw-3.4.0/pylibCZIrw.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-04-24 09:26:12.000000 pylibCZIrw-3.4.0/pylibCZIrw.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       22 2023-04-24 09:26:12.000000 pylibCZIrw-3.4.0/pylibCZIrw.egg-info/requires.txt
--rw-rw-rw-   0        0        0       23 2023-04-24 09:26:12.000000 pylibCZIrw-3.4.0/pylibCZIrw.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1631 2023-04-24 09:26:13.671386 pylibCZIrw-3.4.0/setup.cfg
--rw-rw-rw-   0        0        0     4599 2023-04-24 09:24:55.000000 pylibCZIrw-3.4.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-27 11:40:23.712123 pylibCZIrw-3.4.1/
+-rw-rw-rw-   0        0        0     4031 2023-06-27 11:39:32.000000 pylibCZIrw-3.4.1/CMakeLists.txt
+-rw-rw-rw-   0        0        0      787 2023-06-27 11:39:32.000000 pylibCZIrw-3.4.1/CMakeSettings.json
+-rw-rw-rw-   0        0        0     7815 2023-06-27 11:39:32.000000 pylibCZIrw-3.4.1/COPYING.LESSER.txt
+-rw-rw-rw-   0        0        0    35821 2023-06-27 11:39:32.000000 pylibCZIrw-3.4.1/COPYING.txt
+-rw-rw-rw-   0        0        0     2060 2023-06-27 11:39:32.000000 pylibCZIrw-3.4.1/INFO.md
+-rw-rw-rw-   0        0        0      344 2023-06-27 11:39:32.000000 pylibCZIrw-3.4.1/MANIFEST.in
+-rw-rw-rw-   0        0        0      191 2023-06-27 11:39:32.000000 pylibCZIrw-3.4.1/NOTICE.txt
+-rw-rw-rw-   0        0        0     3026 2023-06-27 11:40:23.712123 pylibCZIrw-3.4.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-27 11:40:23.446492 pylibCZIrw-3.4.1/_pylibCZIrw/
+drwxrwxrwx   0        0        0        0 2023-06-27 11:40:23.446492 pylibCZIrw-3.4.1/_pylibCZIrw/src/
+drwxrwxrwx   0        0        0        0 2023-06-27 11:40:23.462119 pylibCZIrw-3.4.1/_pylibCZIrw/src/api/
+-rw-rw-rw-   0        0        0     2292 2023-06-27 11:39:32.000000 pylibCZIrw-3.4.1/_pylibCZIrw/src/api/CZIreadAPI.cpp
+-rw-rw-rw-   0        0        0     1996 2023-06-27 11:39:32.000000 pylibCZIrw-3.4.1/_pylibCZIrw/src/api/CZIreadAPI.h
+-rw-rw-rw-   0        0        0    10754 2023-06-27 11:39:32.000000 pylibCZIrw-3.4.1/_pylibCZIrw/src/api/CZIwriteAPI.cpp
+-rw-rw-rw-   0        0        0     6496 2023-06-27 11:39:32.000000 pylibCZIrw-3.4.1/_pylibCZIrw/src/api/CZIwriteAPI.h
+-rw-rw-rw-   0        0        0      865 2023-06-27 11:39:32.000000 pylibCZIrw-3.4.1/_pylibCZIrw/src/api/DllMain.cpp
+-rw-rw-rw-   0        0        0     1232 2023-06-27 11:39:32.000000 pylibCZIrw-3.4.1/_pylibCZIrw/src/api/PImage.cpp
+-rw-rw-rw-   0        0        0     1740 2023-06-27 11:39:32.000000 pylibCZIrw-3.4.1/_pylibCZIrw/src/api/PImage.h
+-rw-rw-rw-   0        0        0       64 2023-06-27 11:39:32.000000 pylibCZIrw-3.4.1/_pylibCZIrw/src/api/inc_libCzi.h
+drwxrwxrwx   0        0        0        0 2023-06-27 11:40:23.462119 pylibCZIrw-3.4.1/_pylibCZIrw/src/bindings/
+-rw-rw-rw-   0        0        0     7998 2023-06-27 11:39:32.000000 pylibCZIrw-3.4.1/_pylibCZIrw/src/bindings/CZIrw.cpp
+-rw-rw-rw-   0        0        0     1400 2023-06-27 11:39:32.000000 pylibCZIrw-3.4.1/_pylibCZIrw/src/bindings/PbHelper.cpp
+-rw-rw-rw-   0        0        0     1736 2023-06-27 11:39:32.000000 pylibCZIrw-3.4.1/_pylibCZIrw/src/bindings/PbHelper.h
+drwxrwxrwx   0        0        0        0 2023-06-27 11:40:23.462119 pylibCZIrw-3.4.1/_pylibCZIrw/tests/
+-rw-rw-rw-   0        0        0     1486 2023-06-27 11:39:32.000000 pylibCZIrw-3.4.1/_pylibCZIrw/tests/main.cpp
+drwxrwxrwx   0        0        0        0 2023-06-27 11:40:23.446492 pylibCZIrw-3.4.1/libs/
+drwxrwxrwx   0        0        0        0 2023-06-27 11:40:23.462119 pylibCZIrw-3.4.1/libs/libCZIrw/
+-rw-rw-rw-   0        0        0     3111 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/.editorconfig
+-rw-rw-rw-   0        0        0       41 2023-06-27 11:39:38.000000 pylibCZIrw-3.4.1/libs/libCZIrw/.git
+drwxrwxrwx   0        0        0        0 2023-06-27 11:40:23.462119 pylibCZIrw-3.4.1/libs/libCZIrw/.github/
+drwxrwxrwx   0        0        0        0 2023-06-27 11:40:23.462119 pylibCZIrw-3.4.1/libs/libCZIrw/.github/ISSUE_TEMPLATE/
+-rw-rw-rw-   0        0        0      872 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-rw-rw-   0        0        0      615 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-rw-rw-   0        0        0     1409 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/.github/PULL_REQUEST_TEMPLATE.md
+-rw-rw-rw-   0        0        0      469 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/.github/codecov.yml
+drwxrwxrwx   0        0        0        0 2023-06-27 11:40:23.477745 pylibCZIrw-3.4.1/libs/libCZIrw/.github/workflows/
+-rw-rw-rw-   0        0        0      858 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/.github/workflows/cla.yml
+-rw-rw-rw-   0        0        0     4038 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/.github/workflows/cmake.yml
+-rw-rw-rw-   0        0        0     2129 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/.github/workflows/codeql.yml
+-rw-rw-rw-   0        0        0     1193 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/.github/workflows/mega-linter.yml
+-rw-rw-rw-   0        0        0     1374 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/.github/workflows/pages.yml
+-rw-rw-rw-   0        0        0      296 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/.github/workflows/reuse.yml
+-rw-rw-rw-   0        0        0     5464 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/.gitignore
+-rw-rw-rw-   0        0        0      735 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/.mega-linter.yml
+drwxrwxrwx   0        0        0        0 2023-06-27 11:40:23.477745 pylibCZIrw-3.4.1/libs/libCZIrw/.reuse/
+-rw-rw-rw-   0        0        0      712 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/.reuse/dep5
+-rw-rw-rw-   0        0        0     4377 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/CMakeLists.txt
+-rw-rw-rw-   0        0        0     5501 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/CODE_OF_CONDUCT.md
+-rw-rw-rw-   0        0        0     2687 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/CONTRIBUTING.md
+-rw-rw-rw-   0        0        0    35819 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/COPYING
+-rw-rw-rw-   0        0        0     7815 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/COPYING.LESSER
+-rw-rw-rw-   0        0        0      973 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/CPPLINT.cfg
+drwxrwxrwx   0        0        0        0 2023-06-27 11:40:23.477745 pylibCZIrw-3.4.1/libs/libCZIrw/LICENSES/
+-rw-rw-rw-   0        0        0     1471 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/LICENSES/BSD-3-Clause.txt
+-rw-rw-rw-   0        0        0     7169 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/LICENSES/CC0-1.0.txt
+-rw-rw-rw-   0        0        0    42402 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/LICENSES/LGPL-3.0-or-later.txt
+-rw-rw-rw-   0        0        0     1087 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/LICENSES/MIT.txt
+-rw-rw-rw-   0        0        0      878 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/LICENSES/RSA-MD.txt
+-rw-rw-rw-   0        0        0     4249 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/README.md
+-rw-rw-rw-   0        0        0      587 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/SECURITY.md
+drwxrwxrwx   0        0        0        0 2023-06-27 11:40:23.477745 pylibCZIrw-3.4.1/libs/libCZIrw/Src/
+-rw-rw-rw-   0        0        0      491 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/Src/CMakeLists.txt
+-rw-rw-rw-   0        0        0   127198 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/Src/Doxyfile
+drwxrwxrwx   0        0        0        0 2023-06-27 11:40:23.477745 pylibCZIrw-3.4.1/libs/libCZIrw/Src/JxrDecode/
+-rw-rw-rw-   0        0        0     2137 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/Src/JxrDecode/CMakeLists.txt
+drwxrwxrwx   0        0        0        0 2023-06-27 11:40:23.508994 pylibCZIrw-3.4.1/libs/libCZIrw/Src/JxrDecode/Jxr/
+-rw-rw-rw-   0        0        0    32942 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/Src/JxrDecode/Jxr/JXRGlue.c
+-rw-rw-rw-   0        0        0    30331 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/Src/JxrDecode/Jxr/JXRGlue.h
+-rw-rw-rw-   0        0        0    82146 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/Src/JxrDecode/Jxr/JXRGlueJxr.c
+-rw-rw-rw-   0        0        0    71573 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/Src/JxrDecode/Jxr/JXRGluePFC.c
+-rw-rw-rw-   0        0        0    29194 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/Src/JxrDecode/Jxr/JXRMeta.c
+-rw-rw-rw-   0        0        0     9173 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/Src/JxrDecode/Jxr/JXRMeta.h
+-rw-rw-rw-   0        0        0     9805 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/Src/JxrDecode/Jxr/JXRTest.c
+-rw-rw-rw-   0        0        0     5731 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/Src/JxrDecode/Jxr/JXRTest.h
+-rw-rw-rw-   0        0        0    12746 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/Src/JxrDecode/Jxr/JXRTestBmp.c
+-rw-rw-rw-   0        0        0     7415 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/Src/JxrDecode/Jxr/JXRTestHdr.c
+-rw-rw-rw-   0        0        0     9754 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/Src/JxrDecode/Jxr/JXRTestPnm.c
+-rw-rw-rw-   0        0        0    28100 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/Src/JxrDecode/Jxr/JXRTestTif.c
+-rw-rw-rw-   0        0        0     1208 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/Src/JxrDecode/Jxr/JXRTestWrapper.c
+-rw-rw-rw-   0        0        0      392 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/Src/JxrDecode/Jxr/JXRTestWrapper.h
+-rw-rw-rw-   0        0        0    15650 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/Src/JxrDecode/Jxr/JXRTestYUV.c
+-rw-rw-rw-   0        0        0    46751 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/Src/JxrDecode/Jxr/JXRTranscode.c
+drwxrwxrwx   0        0        0        0 2023-06-27 11:40:23.508994 pylibCZIrw-3.4.1/libs/libCZIrw/Src/JxrDecode/Jxr/_x86/
+-rw-rw-rw-   0        0        0     2257 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/Src/JxrDecode/Jxr/_x86/_x86.h
+-rw-rw-rw-   0        0        0    13119 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/Src/JxrDecode/Jxr/adapthuff.c
+-rw-rw-rw-   0        0        0     2308 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/Src/JxrDecode/Jxr/ansi.h
+-rw-rw-rw-   0        0        0     4875 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/Src/JxrDecode/Jxr/common.h
+-rw-rw-rw-   0        0        0     6826 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/Src/JxrDecode/Jxr/decode.c
+-rw-rw-rw-   0        0        0     5183 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/Src/JxrDecode/Jxr/decode.h
+-rw-rw-rw-   0        0        0     5517 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/Src/JxrDecode/Jxr/encode.c
+-rw-rw-rw-   0        0        0     4300 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/Src/JxrDecode/Jxr/encode.h
+-rw-rw-rw-   0        0        0     6285 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/Src/JxrDecode/Jxr/image.c
+-rw-rw-rw-   0        0        0       54 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/Src/JxrDecode/Jxr/jxr_defines.h
+-rw-rw-rw-   0        0        0     5274 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/Src/JxrDecode/Jxr/perfTimer.h
+-rw-rw-rw-   0        0        0     7657 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/Src/JxrDecode/Jxr/perfTimerANSI.c
+-rw-rw-rw-   0        0        0    10556 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/Src/JxrDecode/Jxr/postprocess.c
+-rw-rw-rw-   0        0        0     6484 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/Src/JxrDecode/Jxr/priv_guiddef.h
+-rw-rw-rw-   0        0        0    44116 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/Src/JxrDecode/Jxr/segdec.c
+-rw-rw-rw-   0        0        0    44265 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/Src/JxrDecode/Jxr/segenc.c
+-rw-rw-rw-   0        0        0    38303 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/Src/JxrDecode/Jxr/strFwdTransform.c
+-rw-rw-rw-   0        0        0    68724 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/Src/JxrDecode/Jxr/strInvTransform.c
+-rw-rw-rw-   0        0        0    10644 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/Src/JxrDecode/Jxr/strPredQuant.c
+-rw-rw-rw-   0        0        0    18412 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/Src/JxrDecode/Jxr/strPredQuantDec.c
+-rw-rw-rw-   0        0        0    18645 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/Src/JxrDecode/Jxr/strPredQuantEnc.c
+-rw-rw-rw-   0        0        0     2629 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/Src/JxrDecode/Jxr/strTransform.c
+-rw-rw-rw-   0        0        0     2387 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/Src/JxrDecode/Jxr/strTransform.h
+-rw-rw-rw-   0        0        0    39625 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/Src/JxrDecode/Jxr/strcodec.c
+-rw-rw-rw-   0        0        0    23294 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/Src/JxrDecode/Jxr/strcodec.h
+-rw-rw-rw-   0        0        0   151177 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/Src/JxrDecode/Jxr/strdec.c
+-rw-rw-rw-   0        0        0    51843 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/Src/JxrDecode/Jxr/strdec_x86.c
+-rw-rw-rw-   0        0        0    98067 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/Src/JxrDecode/Jxr/strenc.c
+-rw-rw-rw-   0        0        0    12654 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/Src/JxrDecode/Jxr/strenc_x86.c
+-rw-rw-rw-   0        0        0    16567 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/Src/JxrDecode/Jxr/windowsmediaphoto.h
+-rw-rw-rw-   0        0        0    45861 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/Src/JxrDecode/Jxr/wmsal.h
+-rw-rw-rw-   0        0        0    23441 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/Src/JxrDecode/Jxr/wmspecstring.h
+-rw-rw-rw-   0        0        0     3295 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/Src/JxrDecode/Jxr/wmspecstrings_adt.h
+-rw-rw-rw-   0        0        0    57847 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/Src/JxrDecode/Jxr/wmspecstrings_strict.h
+-rw-rw-rw-   0        0        0    12055 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/Src/JxrDecode/Jxr/wmspecstrings_undef.h
+-rw-rw-rw-   0        0        0    20032 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/Src/JxrDecode/JxrDecode.cpp
+-rw-rw-rw-   0        0        0     4710 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/Src/JxrDecode/JxrDecode.h
+-rw-rw-rw-   0        0        0      414 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/Src/JxrDecode/stdafx.cpp
+-rw-rw-rw-   0        0        0      489 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/Src/JxrDecode/stdafx.h
+-rw-rw-rw-   0        0        0      478 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/Src/JxrDecode/targetver.h
+drwxrwxrwx   0        0        0        0 2023-06-27 11:40:23.555871 pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/
+-rw-rw-rw-   0        0        0    17295 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/BitmapOperations.cpp
+-rw-rw-rw-   0        0        0     5407 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/BitmapOperations.h
+-rw-rw-rw-   0        0        0    25758 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/BitmapOperations.hpp
+-rw-rw-rw-   0        0        0    11614 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/CMakeLists.txt
+-rw-rw-rw-   0        0        0    12124 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/CZIReader.cpp
+-rw-rw-rw-   0        0        0     2892 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/CZIReader.h
+-rw-rw-rw-   0        0        0     3460 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/CreateBitmap.cpp
+-rw-rw-rw-   0        0        0     1074 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/CziAttachment.cpp
+-rw-rw-rw-   0        0        0      804 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/CziAttachment.h
+-rw-rw-rw-   0        0        0     5295 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/CziAttachmentsDirectory.cpp
+-rw-rw-rw-   0        0        0     2614 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/CziAttachmentsDirectory.h
+-rw-rw-rw-   0        0        0     6292 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/CziDimensionInfo.cpp
+-rw-rw-rw-   0        0        0     3447 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/CziDimensionInfo.h
+-rw-rw-rw-   0        0        0    14592 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/CziDisplaySettings.cpp
+-rw-rw-rw-   0        0        0     1867 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/CziDisplaySettings.h
+-rw-rw-rw-   0        0        0     7059 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/CziMetadata.cpp
+-rw-rw-rw-   0        0        0     1733 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/CziMetadata.h
+-rw-rw-rw-   0        0        0    37203 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/CziMetadataBuilder.cpp
+-rw-rw-rw-   0        0        0     4798 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/CziMetadataBuilder.h
+-rw-rw-rw-   0        0        0    16544 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/CziMetadataDocumentInfo.cpp
+-rw-rw-rw-   0        0        0     1522 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/CziMetadataDocumentInfo.h
+-rw-rw-rw-   0        0        0    71850 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/CziMetadataDocumentInfo2.cpp
+-rw-rw-rw-   0        0        0    41047 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/CziMetadataDocumentInfo2.h
+-rw-rw-rw-   0        0        0     1689 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/CziMetadataSegment.cpp
+-rw-rw-rw-   0        0        0      773 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/CziMetadataSegment.h
+-rw-rw-rw-   0        0        0    32912 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/CziParse.cpp
+-rw-rw-rw-   0        0        0     4854 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/CziParse.h
+-rw-rw-rw-   0        0        0    37315 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/CziReaderWriter.cpp
+-rw-rw-rw-   0        0        0     7881 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/CziReaderWriter.h
+-rw-rw-rw-   0        0        0     7183 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/CziStructs.cpp
+-rw-rw-rw-   0        0        0     9361 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/CziStructs.h
+-rw-rw-rw-   0        0        0     2279 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/CziSubBlock.cpp
+-rw-rw-rw-   0        0        0     1001 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/CziSubBlock.h
+-rw-rw-rw-   0        0        0    22081 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/CziSubBlockDirectory.cpp
+-rw-rw-rw-   0        0        0     6513 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/CziSubBlockDirectory.h
+-rw-rw-rw-   0        0        0     6163 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/CziUtils.cpp
+-rw-rw-rw-   0        0        0     2342 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/CziUtils.h
+-rw-rw-rw-   0        0        0    59642 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/CziWriter.cpp
+-rw-rw-rw-   0        0        0    16511 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/CziWriter.h
+-rw-rw-rw-   0        0        0     8038 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/DimCoordinate.cpp
+drwxrwxrwx   0        0        0        0 2023-06-27 11:40:23.571494 pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/Doc/
+-rw-rw-rw-   0        0        0    25621 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/Doc/CZICmd_usage.markdown
+drwxrwxrwx   0        0        0        0 2023-06-27 11:40:23.587121 pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/Doc/Images/
+-rw-rw-rw-   0        0        0    15042 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/Doc/Images/CZI_1.PNG
+-rw-rw-rw-   0        0        0    11631 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/Doc/Images/CZI_2.PNG
+-rw-rw-rw-   0        0        0   629984 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/Doc/Images/ScalingSingleChannelTileAccessor1.png
+-rw-rw-rw-   0        0        0    15606 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/Doc/Images/SingleChannelTileAccessor_1.PNG
+-rw-rw-rw-   0        0        0     6597 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/Doc/Images/SingleChannelTileAccessor_2.PNG
+-rw-rw-rw-   0        0        0   508732 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/Doc/Images/SingleChannelTileAccessor_3.PNG
+-rw-rw-rw-   0        0        0   435548 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/Doc/Images/SingleChannelTileAccessor_4.PNG
+-rw-rw-rw-   0        0        0    22752 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/Doc/Images/Tinting-LUT.png
+-rw-rw-rw-   0        0        0    95014 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/Doc/Images/VisualStudio_cmake1.png
+-rw-rw-rw-   0        0        0   947057 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/Doc/Images/ZEN_screenshot_1.PNG
+-rw-rw-rw-   0        0        0   149904 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/Doc/Images/ZEN_screenshot_2.PNG
+-rw-rw-rw-   0        0        0   242149 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/Doc/Images/cmake_1_raspi.PNG
+-rw-rw-rw-   0        0        0    32954 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/Doc/Images/cmake_1_raspi_help_freetype.PNG
+-rw-rw-rw-   0        0        0   270106 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/Doc/Images/cmake_install_raspi1.PNG
+-rw-rw-rw-   0        0        0    59883 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/Doc/Images/cmake_raspi_unittests_1.PNG
+-rw-rw-rw-   0        0        0    14602 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/Doc/Images/compositors_1.png
+-rw-rw-rw-   0        0        0     4107 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/Doc/Images/compositors_2.png
+drwxrwxrwx   0        0        0        0 2023-06-27 11:40:23.587121 pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/Doc/Images/drawings/
+-rw-rw-rw-   0        0        0   100864 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/Doc/Images/drawings/VS-project.pub
+-rw-rw-rw-   0        0        0   108032 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/Doc/Images/drawings/VS-project_2.pub
+-rw-rw-rw-   0        0        0    10567 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/Doc/Images/gradationcurve_1.PNG
+-rw-rw-rw-   0        0        0     8316 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/Doc/Images/gradationcurve_2.PNG
+-rw-rw-rw-   0        0        0     7632 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/Doc/Images/image_document_concept1.PNG
+-rw-rw-rw-   0        0        0    20658 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/Doc/Images/image_document_concept2.PNG
+-rw-rw-rw-   0        0        0    14836 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/Doc/Images/image_document_concept3.PNG
+-rw-rw-rw-   0        0        0    29100 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/Doc/Images/image_document_concept4.PNG
+-rw-rw-rw-   0        0        0     1966 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/Doc/Todos.markdown
+-rw-rw-rw-   0        0        0     2964 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/Doc/accessors.markdown
+-rw-rw-rw-   0        0        0     3020 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/Doc/building_libCZI.markdown
+-rw-rw-rw-   0        0        0    92375 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/Doc/drawings.docx
+-rw-rw-rw-   0        0        0     3983 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/Doc/image_document_concept.markdown
+-rw-rw-rw-   0        0        0     5655 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/Doc/mainpage.markdown
+-rw-rw-rw-   0        0        0     2275 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/Doc/multichannelcomposition.markdown
+-rw-rw-rw-   0        0        0    11134 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/Doc/using_libCZI.markdown
+-rw-rw-rw-   0        0        0     5534 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/Doc/write_czi.markdown
+-rw-rw-rw-   0        0        0     2521 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/FileHeaderSegmentData.h
+-rw-rw-rw-   0        0        0      631 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/ImportExport.h
+-rw-rw-rw-   0        0        0     5323 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/IndexSet.cpp
+-rw-rw-rw-   0        0        0      992 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/IndexSet.h
+-rw-rw-rw-   0        0        0     8801 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/MD5Sum.cpp
+-rw-rw-rw-   0        0        0     5296 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/MD5Sum.h
+-rw-rw-rw-   0        0        0    56461 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/MultiChannelCompositor.cpp
+-rw-rw-rw-   0        0        0      166 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/MultiChannelCompositor.h
+-rw-rw-rw-   0        0        0     3716 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/SingleChannelAccessorBase.cpp
+-rw-rw-rw-   0        0        0      739 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/SingleChannelAccessorBase.h
+-rw-rw-rw-   0        0        0    10906 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/SingleChannelPyramidLevelTileAccessor.cpp
+-rw-rw-rw-   0        0        0     2835 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/SingleChannelPyramidLevelTileAccessor.h
+-rw-rw-rw-   0        0        0    18704 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/SingleChannelScalingTileAccessor.cpp
+-rw-rw-rw-   0        0        0     3176 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/SingleChannelScalingTileAccessor.h
+-rw-rw-rw-   0        0        0     5437 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/SingleChannelTileAccessor.cpp
+-rw-rw-rw-   0        0        0     2132 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/SingleChannelTileAccessor.h
+-rw-rw-rw-   0        0        0     2088 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/SingleChannelTileCompositor.cpp
+-rw-rw-rw-   0        0        0      333 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/SingleChannelTileCompositor.h
+-rw-rw-rw-   0        0        0      187 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/Site.h
+-rw-rw-rw-   0        0        0    20334 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/StreamImpl.cpp
+-rw-rw-rw-   0        0        0     6093 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/StreamImpl.h
+-rw-rw-rw-   0        0        0    13988 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/XmlNodeWrapper.h
+-rw-rw-rw-   0        0        0     5713 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/bitmapData.h
+-rw-rw-rw-   0        0        0     8206 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/decoder.cpp
+-rw-rw-rw-   0        0        0      672 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/decoder.h
+-rw-rw-rw-   0        0        0    17042 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/decoder_wic.cpp
+-rw-rw-rw-   0        0        0      774 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/decoder_wic.h
+-rw-rw-rw-   0        0        0     7689 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/decoder_zstd.cpp
+-rw-rw-rw-   0        0        0      773 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/decoder_zstd.h
+-rw-rw-rw-   0        0        0      264 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/inc_libCZI_Config.h
+-rw-rw-rw-   0        0        0    35455 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/libCZI.h
+-rw-rw-rw-   0        0        0    30893 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/libCZI_Compositor.h
+-rw-rw-rw-   0        0        0     1997 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/libCZI_Config.h.in
+-rw-rw-rw-   0        0        0    17832 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/libCZI_DimCoordinate.h
+-rw-rw-rw-   0        0        0     9636 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/libCZI_Helpers.h
+-rw-rw-rw-   0        0        0     4403 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/libCZI_Lib.cpp
+-rw-rw-rw-   0        0        0    71325 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/libCZI_Metadata.h
+-rw-rw-rw-   0        0        0    63505 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/libCZI_Metadata2.h
+-rw-rw-rw-   0        0        0    13615 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/libCZI_Pixels.h
+-rw-rw-rw-   0        0        0     9656 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/libCZI_ReadWrite.h
+-rw-rw-rw-   0        0        0     5061 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/libCZI_Site.cpp
+-rw-rw-rw-   0        0        0     6262 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/libCZI_Site.h
+-rw-rw-rw-   0        0        0    24080 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/libCZI_Utilities.cpp
+-rw-rw-rw-   0        0        0    19595 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/libCZI_Utilities.h
+-rw-rw-rw-   0        0        0    32800 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/libCZI_Write.h
+-rw-rw-rw-   0        0        0    40830 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/libCZI_compress.h
+-rw-rw-rw-   0        0        0    14343 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/libCZI_exceptions.h
+-rw-rw-rw-   0        0        0     6566 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/priv_guiddef.h
+-rw-rw-rw-   0        0        0     3060 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/pugiconfig.hpp
+-rw-rw-rw-   0        0        0   407937 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/pugixml.cpp
+-rw-rw-rw-   0        0        0    60454 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/pugixml.hpp
+-rw-rw-rw-   0        0        0     3364 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/splines.cpp
+-rw-rw-rw-   0        0        0      554 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/splines.h
+-rw-rw-rw-   0        0        0     1291 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/stdAllocator.cpp
+-rw-rw-rw-   0        0        0      593 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/stdAllocator.h
+-rw-rw-rw-   0        0        0      411 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/stdafx.cpp
+-rw-rw-rw-   0        0        0      739 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/stdafx.h
+-rw-rw-rw-   0        0        0      478 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/targetver.h
+-rw-rw-rw-   0        0        0    12984 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/utilities.cpp
+-rw-rw-rw-   0        0        0     5866 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/utilities.h
+-rw-rw-rw-   0        0        0    12120 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/utilities_simd.cpp
+-rw-rw-rw-   0        0        0    18595 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/zstdCompress.cpp
+-rw-rw-rw-   0        0        0     6291 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/THIRD_PARTY_LICENSES.txt
+-rw-rw-rw-   0        0        0     6882 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/cla_corporate.txt
+-rw-rw-rw-   0        0        0     6571 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/cla_individual.txt
+drwxrwxrwx   0        0        0        0 2023-06-27 11:40:23.587121 pylibCZIrw-3.4.1/libs/libCZIrw/cmake/
+-rw-rw-rw-   0        0        0      836 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/cmake/ExternalEIGEN3.cmake
+-rw-rw-rw-   0        0        0     4609 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/cmake/TestLargeFile.cmake
+-rw-rw-rw-   0        0        0     1842 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/cmake/check_can_use_neon_intrinsics.cmake
+-rw-rw-rw-   0        0        0     2656 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/cmake/check_unaligned_access.cmake
+-rw-rw-rw-   0        0        0      150 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/libCZIrw/opencppcoverage.txt
+drwxrwxrwx   0        0        0        0 2023-06-27 11:40:23.587121 pylibCZIrw-3.4.1/libs/pybind11/
+-rw-rw-rw-   0        0        0     1341 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/.appveyor.yml
+-rw-rw-rw-   0        0        0     1034 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/.clang-format
+-rw-rw-rw-   0        0        0     2282 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/.clang-tidy
+-rw-rw-rw-   0        0        0     2269 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/.cmake-format.yaml
+-rw-rw-rw-   0        0        0       41 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/.git
+drwxrwxrwx   0        0        0        0 2023-06-27 11:40:23.587121 pylibCZIrw-3.4.1/libs/pybind11/.github/
+-rw-rw-rw-   0        0        0      191 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/.github/CODEOWNERS
+-rw-rw-rw-   0        0        0    15646 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/.github/CONTRIBUTING.md
+drwxrwxrwx   0        0        0        0 2023-06-27 11:40:23.602745 pylibCZIrw-3.4.1/libs/pybind11/.github/ISSUE_TEMPLATE/
+-rw-rw-rw-   0        0        0     2061 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/.github/ISSUE_TEMPLATE/bug-report.yml
+-rw-rw-rw-   0        0        0      336 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/.github/ISSUE_TEMPLATE/config.yml
+-rw-rw-rw-   0        0        0      575 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/.github/dependabot.yml
+-rw-rw-rw-   0        0        0      124 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/.github/labeler.yml
+-rw-rw-rw-   0        0        0       53 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/.github/labeler_merged.yml
+-rw-rw-rw-   0        0        0      664 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/.github/pull_request_template.md
+drwxrwxrwx   0        0        0        0 2023-06-27 11:40:23.602745 pylibCZIrw-3.4.1/libs/pybind11/.github/workflows/
+-rw-rw-rw-   0        0        0    29190 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/.github/workflows/ci.yml
+-rw-rw-rw-   0        0        0     2204 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/.github/workflows/configure.yml
+-rw-rw-rw-   0        0        0     1262 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/.github/workflows/format.yml
+-rw-rw-rw-   0        0        0      349 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/.github/workflows/labeler.yml
+-rw-rw-rw-   0        0        0     2624 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/.github/workflows/pip.yml
+-rw-rw-rw-   0        0        0     2936 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/.github/workflows/upstream.yml
+-rw-rw-rw-   0        0        0      532 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/.gitignore
+-rw-rw-rw-   0        0        0     3624 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/.pre-commit-config.yaml
+-rw-rw-rw-   0        0        0       65 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/.readthedocs.yml
+-rw-rw-rw-   0        0        0    11298 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/CMakeLists.txt
+-rw-rw-rw-   0        0        0     1713 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/LICENSE
+-rw-rw-rw-   0        0        0      262 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/MANIFEST.in
+-rw-rw-rw-   0        0        0     7836 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/README.rst
+drwxrwxrwx   0        0        0        0 2023-06-27 11:40:23.602745 pylibCZIrw-3.4.1/libs/pybind11/docs/
+-rw-rw-rw-   0        0        0      675 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/docs/Doxyfile
+-rw-rw-rw-   0        0        0     7609 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/docs/Makefile
+drwxrwxrwx   0        0        0        0 2023-06-27 11:40:23.618371 pylibCZIrw-3.4.1/libs/pybind11/docs/_static/
+-rw-rw-rw-   0        0        0      265 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/docs/_static/theme_overrides.css
+drwxrwxrwx   0        0        0        0 2023-06-27 11:40:23.618371 pylibCZIrw-3.4.1/libs/pybind11/docs/advanced/
+drwxrwxrwx   0        0        0        0 2023-06-27 11:40:23.618371 pylibCZIrw-3.4.1/libs/pybind11/docs/advanced/cast/
+-rw-rw-rw-   0        0        0     4018 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/docs/advanced/cast/chrono.rst
+-rw-rw-rw-   0        0        0     3502 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/docs/advanced/cast/custom.rst
+-rw-rw-rw-   0        0        0    14593 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/docs/advanced/cast/eigen.rst
+-rw-rw-rw-   0        0        0     3998 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/docs/advanced/cast/functional.rst
+-rw-rw-rw-   0        0        0     1599 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/docs/advanced/cast/index.rst
+-rw-rw-rw-   0        0        0    12604 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/docs/advanced/cast/overview.rst
+-rw-rw-rw-   0        0        0     9954 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/docs/advanced/cast/stl.rst
+-rw-rw-rw-   0        0        0     9668 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/docs/advanced/cast/strings.rst
+-rw-rw-rw-   0        0        0    49668 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/docs/advanced/classes.rst
+-rw-rw-rw-   0        0        0     8715 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/docs/advanced/embedding.rst
+-rw-rw-rw-   0        0        0    18204 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/docs/advanced/exceptions.rst
+-rw-rw-rw-   0        0        0    27442 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/docs/advanced/functions.rst
+-rw-rw-rw-   0        0        0    12783 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/docs/advanced/misc.rst
+drwxrwxrwx   0        0        0        0 2023-06-27 11:40:23.618371 pylibCZIrw-3.4.1/libs/pybind11/docs/advanced/pycpp/
+-rw-rw-rw-   0        0        0      291 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/docs/advanced/pycpp/index.rst
+-rw-rw-rw-   0        0        0    17910 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/docs/advanced/pycpp/numpy.rst
+-rw-rw-rw-   0        0        0     9316 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/docs/advanced/pycpp/object.rst
+-rw-rw-rw-   0        0        0     5865 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/docs/advanced/pycpp/utilities.rst
+-rw-rw-rw-   0        0        0     6541 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/docs/advanced/smart_ptrs.rst
+-rw-rw-rw-   0        0        0     9676 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/docs/basics.rst
+-rw-rw-rw-   0        0        0     3053 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/docs/benchmark.py
+-rw-rw-rw-   0        0        0     3263 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/docs/benchmark.rst
+-rw-rw-rw-   0        0        0   101394 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/docs/changelog.rst
+-rw-rw-rw-   0        0        0    16993 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/docs/classes.rst
+drwxrwxrwx   0        0        0        0 2023-06-27 11:40:23.618371 pylibCZIrw-3.4.1/libs/pybind11/docs/cmake/
+-rw-rw-rw-   0        0        0      281 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/docs/cmake/index.rst
+-rw-rw-rw-   0        0        0    26915 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/docs/compiling.rst
+-rw-rw-rw-   0        0        0    12463 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/docs/conf.py
+-rw-rw-rw-   0        0        0    14942 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/docs/faq.rst
+-rw-rw-rw-   0        0        0      661 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/docs/index.rst
+-rw-rw-rw-   0        0        0     3382 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/docs/installing.rst
+-rw-rw-rw-   0        0        0     3151 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/docs/limitations.rst
+-rw-rw-rw-   0        0        0    58510 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/docs/pybind11-logo.png
+-rw-rw-rw-   0        0        0    44653 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/docs/pybind11_vs_boost_python1.png
+-rw-rw-rw-   0        0        0    88135 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/docs/pybind11_vs_boost_python1.svg
+-rw-rw-rw-   0        0        0    41121 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/docs/pybind11_vs_boost_python2.png
+-rw-rw-rw-   0        0        0    86280 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/docs/pybind11_vs_boost_python2.svg
+-rw-rw-rw-   0        0        0     2777 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/docs/reference.rst
+-rw-rw-rw-   0        0        0     4511 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/docs/release.rst
+-rw-rw-rw-   0        0        0      135 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/docs/requirements.txt
+-rw-rw-rw-   0        0        0    24043 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/docs/upgrade.rst
+drwxrwxrwx   0        0        0        0 2023-06-27 11:40:23.446492 pylibCZIrw-3.4.1/libs/pybind11/include/
+drwxrwxrwx   0        0        0        0 2023-06-27 11:40:23.633998 pylibCZIrw-3.4.1/libs/pybind11/include/pybind11/
+-rw-rw-rw-   0        0        0    24595 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/include/pybind11/attr.h
+-rw-rw-rw-   0        0        0     7262 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/include/pybind11/buffer_info.h
+-rw-rw-rw-   0        0        0    66456 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/include/pybind11/cast.h
+-rw-rw-rw-   0        0        0     9143 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/include/pybind11/chrono.h
+-rw-rw-rw-   0        0        0      122 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/include/pybind11/common.h
+-rw-rw-rw-   0        0        0     2170 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/include/pybind11/complex.h
+drwxrwxrwx   0        0        0        0 2023-06-27 11:40:23.633998 pylibCZIrw-3.4.1/libs/pybind11/include/pybind11/detail/
+-rw-rw-rw-   0        0        0    29274 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/include/pybind11/detail/class.h
+-rw-rw-rw-   0        0        0    52865 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/include/pybind11/detail/common.h
+-rw-rw-rw-   0        0        0     5649 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/include/pybind11/detail/descr.h
+-rw-rw-rw-   0        0        0    18399 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/include/pybind11/detail/init.h
+-rw-rw-rw-   0        0        0    24768 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/include/pybind11/detail/internals.h
+-rw-rw-rw-   0        0        0    45497 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/include/pybind11/detail/type_caster_base.h
+-rw-rw-rw-   0        0        0     1572 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/include/pybind11/detail/typeid.h
+-rw-rw-rw-   0        0        0    32140 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/include/pybind11/eigen.h
+-rw-rw-rw-   0        0        0    12477 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/include/pybind11/embed.h
+-rw-rw-rw-   0        0        0     5767 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/include/pybind11/eval.h
+-rw-rw-rw-   0        0        0     4886 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/include/pybind11/functional.h
+-rw-rw-rw-   0        0        0     7050 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/include/pybind11/gil.h
+-rw-rw-rw-   0        0        0     9116 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/include/pybind11/iostream.h
+-rw-rw-rw-   0        0        0    79994 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/include/pybind11/numpy.h
+-rw-rw-rw-   0        0        0    10001 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/include/pybind11/operators.h
+-rw-rw-rw-   0        0        0     2257 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/include/pybind11/options.h
+-rw-rw-rw-   0        0        0   128798 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/include/pybind11/pybind11.h
+-rw-rw-rw-   0        0        0    83054 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/include/pybind11/pytypes.h
+drwxrwxrwx   0        0        0        0 2023-06-27 11:40:23.633998 pylibCZIrw-3.4.1/libs/pybind11/include/pybind11/stl/
+-rw-rw-rw-   0        0        0     3654 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/include/pybind11/stl/filesystem.h
+-rw-rw-rw-   0        0        0    14860 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/include/pybind11/stl.h
+-rw-rw-rw-   0        0        0    27777 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/include/pybind11/stl_bind.h
+-rw-rw-rw-   0        0        0     2667 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/noxfile.py
+drwxrwxrwx   0        0        0        0 2023-06-27 11:40:23.633998 pylibCZIrw-3.4.1/libs/pybind11/pybind11/
+-rw-rw-rw-   0        0        0      227 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/pybind11/__init__.py
+-rw-rw-rw-   0        0        0     1210 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/pybind11/__main__.py
+-rw-rw-rw-   0        0        0      214 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/pybind11/_version.py
+-rw-rw-rw-   0        0        0      143 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/pybind11/_version.pyi
+-rw-rw-rw-   0        0        0      683 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/pybind11/commands.py
+-rw-rw-rw-   0        0        0        0 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/pybind11/py.typed
+-rw-rw-rw-   0        0        0    17977 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/pybind11/setup_helpers.py
+-rw-rw-rw-   0        0        0     2101 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/pybind11/setup_helpers.pyi
+-rw-rw-rw-   0        0        0      998 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/pyproject.toml
+-rw-rw-rw-   0        0        0     1973 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/setup.cfg
+-rw-rw-rw-   0        0        0     5222 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-27 11:40:23.696498 pylibCZIrw-3.4.1/libs/pybind11/tests/
+-rw-rw-rw-   0        0        0    21668 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/tests/CMakeLists.txt
+-rw-rw-rw-   0        0        0     5049 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/tests/conftest.py
+-rw-rw-rw-   0        0        0    12056 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/tests/constructor_stats.h
+-rw-rw-rw-   0        0        0     1845 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/tests/cross_module_gil_utils.cpp
+-rw-rw-rw-   0        0        0     1055 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/tests/env.py
+drwxrwxrwx   0        0        0        0 2023-06-27 11:40:23.696498 pylibCZIrw-3.4.1/libs/pybind11/tests/extra_python_package/
+-rw-rw-rw-   0        0        0        0 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/tests/extra_python_package/pytest.ini
+-rw-rw-rw-   0        0        0     7857 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/tests/extra_python_package/test_files.py
+drwxrwxrwx   0        0        0        0 2023-06-27 11:40:23.696498 pylibCZIrw-3.4.1/libs/pybind11/tests/extra_setuptools/
+-rw-rw-rw-   0        0        0        0 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/tests/extra_setuptools/pytest.ini
+-rw-rw-rw-   0        0        0     4372 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/tests/extra_setuptools/test_setuphelper.py
+-rw-rw-rw-   0        0        0     2939 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/tests/local_bindings.h
+-rw-rw-rw-   0        0        0     5948 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/tests/object.h
+-rw-rw-rw-   0        0        0     6413 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/tests/pybind11_cross_module_tests.cpp
+-rw-rw-rw-   0        0        0     3778 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/tests/pybind11_tests.cpp
+-rw-rw-rw-   0        0        0     3109 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/tests/pybind11_tests.h
+-rw-rw-rw-   0        0        0      712 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/tests/pytest.ini
+-rw-rw-rw-   0        0        0      889 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/tests/requirements.txt
+-rw-rw-rw-   0        0        0      880 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/tests/test_async.cpp
+-rw-rw-rw-   0        0        0      583 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/tests/test_async.py
+-rw-rw-rw-   0        0        0     8791 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/tests/test_buffers.cpp
+-rw-rw-rw-   0        0        0     5222 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/tests/test_buffers.py
+-rw-rw-rw-   0        0        0    16257 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/tests/test_builtin_casters.cpp
+-rw-rw-rw-   0        0        0    18922 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/tests/test_builtin_casters.py
+-rw-rw-rw-   0        0        0     4233 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/tests/test_call_policies.cpp
+-rw-rw-rw-   0        0        0     6821 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/tests/test_call_policies.py
+-rw-rw-rw-   0        0        0     9486 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/tests/test_callbacks.cpp
+-rw-rw-rw-   0        0        0     6246 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/tests/test_callbacks.py
+-rw-rw-rw-   0        0        0     3451 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/tests/test_chrono.cpp
+-rw-rw-rw-   0        0        0     5937 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/tests/test_chrono.py
+-rw-rw-rw-   0        0        0    24441 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/tests/test_class.cpp
+-rw-rw-rw-   0        0        0    14981 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/tests/test_class.py
+drwxrwxrwx   0        0        0        0 2023-06-27 11:40:23.696498 pylibCZIrw-3.4.1/libs/pybind11/tests/test_cmake_build/
+-rw-rw-rw-   0        0        0     2723 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/tests/test_cmake_build/CMakeLists.txt
+-rw-rw-rw-   0        0        0      696 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/tests/test_cmake_build/embed.cpp
+drwxrwxrwx   0        0        0        0 2023-06-27 11:40:23.696498 pylibCZIrw-3.4.1/libs/pybind11/tests/test_cmake_build/installed_embed/
+-rw-rw-rw-   0        0        0     1199 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/tests/test_cmake_build/installed_embed/CMakeLists.txt
+drwxrwxrwx   0        0        0        0 2023-06-27 11:40:23.696498 pylibCZIrw-3.4.1/libs/pybind11/tests/test_cmake_build/installed_function/
+-rw-rw-rw-   0        0        0     1332 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/tests/test_cmake_build/installed_function/CMakeLists.txt
+drwxrwxrwx   0        0        0        0 2023-06-27 11:40:23.696498 pylibCZIrw-3.4.1/libs/pybind11/tests/test_cmake_build/installed_target/
+-rw-rw-rw-   0        0        0     1731 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/tests/test_cmake_build/installed_target/CMakeLists.txt
+-rw-rw-rw-   0        0        0      158 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/tests/test_cmake_build/main.cpp
+drwxrwxrwx   0        0        0        0 2023-06-27 11:40:23.696498 pylibCZIrw-3.4.1/libs/pybind11/tests/test_cmake_build/subdirectory_embed/
+-rw-rw-rw-   0        0        0     1394 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/tests/test_cmake_build/subdirectory_embed/CMakeLists.txt
+drwxrwxrwx   0        0        0        0 2023-06-27 11:40:23.696498 pylibCZIrw-3.4.1/libs/pybind11/tests/test_cmake_build/subdirectory_function/
+-rw-rw-rw-   0        0        0     1198 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/tests/test_cmake_build/subdirectory_function/CMakeLists.txt
+drwxrwxrwx   0        0        0        0 2023-06-27 11:40:23.696498 pylibCZIrw-3.4.1/libs/pybind11/tests/test_cmake_build/subdirectory_target/
+-rw-rw-rw-   0        0        0     1409 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/tests/test_cmake_build/subdirectory_target/CMakeLists.txt
+-rw-rw-rw-   0        0        0      283 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/tests/test_cmake_build/test.py
+-rw-rw-rw-   0        0        0     4324 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/tests/test_const_name.cpp
+-rw-rw-rw-   0        0        0      681 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/tests/test_const_name.py
+-rw-rw-rw-   0        0        0     6096 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/tests/test_constants_and_functions.cpp
+-rw-rw-rw-   0        0        0     1575 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/tests/test_constants_and_functions.py
+-rw-rw-rw-   0        0        0    11010 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/tests/test_copy_move.cpp
+-rw-rw-rw-   0        0        0     4772 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/tests/test_copy_move.py
+-rw-rw-rw-   0        0        0     7419 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/tests/test_custom_type_casters.cpp
+-rw-rw-rw-   0        0        0     4209 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/tests/test_custom_type_casters.py
+-rw-rw-rw-   0        0        0     1300 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/tests/test_custom_type_setup.cpp
+-rw-rw-rw-   0        0        0     1164 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/tests/test_custom_type_setup.py
+-rw-rw-rw-   0        0        0     2904 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/tests/test_docstring_options.cpp
+-rw-rw-rw-   0        0        0     1672 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/tests/test_docstring_options.py
+-rw-rw-rw-   0        0        0    18570 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/tests/test_eigen.cpp
+-rw-rw-rw-   0        0        0    29054 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/tests/test_eigen.py
+drwxrwxrwx   0        0        0        0 2023-06-27 11:40:23.696498 pylibCZIrw-3.4.1/libs/pybind11/tests/test_embed/
+-rw-rw-rw-   0        0        0     1845 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/tests/test_embed/CMakeLists.txt
+-rw-rw-rw-   0        0        0      760 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/tests/test_embed/catch.cpp
+-rw-rw-rw-   0        0        0      563 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/tests/test_embed/external_module.cpp
+-rw-rw-rw-   0        0        0    14573 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/tests/test_embed/test_interpreter.cpp
+-rw-rw-rw-   0        0        0      295 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/tests/test_embed/test_interpreter.py
+-rw-rw-rw-   0        0        0      318 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/tests/test_embed/test_trampoline.py
+-rw-rw-rw-   0        0        0     5855 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/tests/test_enum.cpp
+-rw-rw-rw-   0        0        0     9404 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/tests/test_enum.py
+-rw-rw-rw-   0        0        0     3286 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/tests/test_eval.cpp
+-rw-rw-rw-   0        0        0     1234 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/tests/test_eval.py
+-rw-rw-rw-   0        0        0      148 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/tests/test_eval_call.py
+-rw-rw-rw-   0        0        0    10502 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/tests/test_exceptions.cpp
+-rw-rw-rw-   0        0        0      412 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/tests/test_exceptions.h
+-rw-rw-rw-   0        0        0     9313 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/tests/test_exceptions.py
+-rw-rw-rw-   0        0        0    18856 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/tests/test_factory_constructors.cpp
+-rw-rw-rw-   0        0        0    17251 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/tests/test_factory_constructors.py
+-rw-rw-rw-   0        0        0     1720 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/tests/test_gil_scoped.cpp
+-rw-rw-rw-   0        0        0     3222 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/tests/test_gil_scoped.py
+-rw-rw-rw-   0        0        0     4252 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/tests/test_iostream.cpp
+-rw-rw-rw-   0        0        0     8289 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/tests/test_iostream.py
+-rw-rw-rw-   0        0        0     9509 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/tests/test_kwargs_and_defaults.cpp
+-rw-rw-rw-   0        0        0    14391 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/tests/test_kwargs_and_defaults.py
+-rw-rw-rw-   0        0        0     4507 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/tests/test_local_bindings.cpp
+-rw-rw-rw-   0        0        0     8358 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/tests/test_local_bindings.py
+-rw-rw-rw-   0        0        0    21786 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/tests/test_methods_and_attributes.cpp
+-rw-rw-rw-   0        0        0    18329 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/tests/test_methods_and_attributes.py
+-rw-rw-rw-   0        0        0     4144 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/tests/test_modules.cpp
+-rw-rw-rw-   0        0        0     2935 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/tests/test_modules.py
+-rw-rw-rw-   0        0        0    12646 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/tests/test_multiple_inheritance.cpp
+-rw-rw-rw-   0        0        0    12530 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/tests/test_multiple_inheritance.py
+-rw-rw-rw-   0        0        0    20298 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/tests/test_numpy_array.cpp
+-rw-rw-rw-   0        0        0    20932 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/tests/test_numpy_array.py
+-rw-rw-rw-   0        0        0    20739 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/tests/test_numpy_dtypes.cpp
+-rw-rw-rw-   0        0        0    14477 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/tests/test_numpy_dtypes.py
+-rw-rw-rw-   0        0        0     4568 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/tests/test_numpy_vectorize.cpp
+-rw-rw-rw-   0        0        0     9977 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/tests/test_numpy_vectorize.py
+-rw-rw-rw-   0        0        0     2854 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/tests/test_opaque_types.cpp
+-rw-rw-rw-   0        0        0     1966 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/tests/test_opaque_types.py
+-rw-rw-rw-   0        0        0     9751 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/tests/test_operator_overloading.cpp
+-rw-rw-rw-   0        0        0     4547 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/tests/test_operator_overloading.py
+-rw-rw-rw-   0        0        0     6841 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/tests/test_pickling.cpp
+-rw-rw-rw-   0        0        0     2368 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/tests/test_pickling.py
+-rw-rw-rw-   0        0        0    21430 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/tests/test_pytypes.cpp
+-rw-rw-rw-   0        0        0    19669 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/tests/test_pytypes.py
+-rw-rw-rw-   0        0        0    21142 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/tests/test_sequences_and_iterators.cpp
+-rw-rw-rw-   0        0        0     8312 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/tests/test_sequences_and_iterators.py
+-rw-rw-rw-   0        0        0    19514 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/tests/test_smart_ptr.cpp
+-rw-rw-rw-   0        0        0     9938 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/tests/test_smart_ptr.py
+-rw-rw-rw-   0        0        0    21250 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/tests/test_stl.cpp
+-rw-rw-rw-   0        0        0    12020 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/tests/test_stl.py
+-rw-rw-rw-   0        0        0     4774 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/tests/test_stl_binders.cpp
+-rw-rw-rw-   0        0        0     8389 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/tests/test_stl_binders.py
+-rw-rw-rw-   0        0        0     4744 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/tests/test_tagbased_polymorphic.cpp
+-rw-rw-rw-   0        0        0      794 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/tests/test_tagbased_polymorphic.py
+-rw-rw-rw-   0        0        0     1921 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/tests/test_thread.cpp
+-rw-rw-rw-   0        0        0      919 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/tests/test_thread.py
+-rw-rw-rw-   0        0        0      625 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/tests/test_union.cpp
+-rw-rw-rw-   0        0        0      181 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/tests/test_union.py
+-rw-rw-rw-   0        0        0    23695 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/tests/test_virtual_functions.cpp
+-rw-rw-rw-   0        0        0    13606 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/tests/test_virtual_functions.py
+-rw-rw-rw-   0        0        0     3366 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/tests/valgrind-numpy-scipy.supp
+-rw-rw-rw-   0        0        0     2774 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/tests/valgrind-python.supp
+drwxrwxrwx   0        0        0        0 2023-06-27 11:40:23.712123 pylibCZIrw-3.4.1/libs/pybind11/tools/
+-rw-rw-rw-   0        0        0     2422 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/tools/FindCatch.cmake
+-rw-rw-rw-   0        0        0     3191 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/tools/FindEigen3.cmake
+-rw-rw-rw-   0        0        0    10648 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/tools/FindPythonLibsNew.cmake
+-rw-rw-rw-   0        0        0     1467 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/tools/check-style.sh
+-rw-rw-rw-   0        0        0      975 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/tools/cmake_uninstall.cmake.in
+-rw-rw-rw-   0        0        0     1161 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/tools/libsize.py
+-rw-rw-rw-   0        0        0     1370 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/tools/make_changelog.py
+-rw-rw-rw-   0        0        0    14990 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/tools/pybind11Common.cmake
+-rw-rw-rw-   0        0        0     7296 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/tools/pybind11Config.cmake.in
+-rw-rw-rw-   0        0        0     9951 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/tools/pybind11NewTools.cmake
+-rw-rw-rw-   0        0        0     7666 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/tools/pybind11Tools.cmake
+-rw-rw-rw-   0        0        0       97 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/tools/pyproject.toml
+-rw-rw-rw-   0        0        0     2016 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/tools/setup_global.py.in
+-rw-rw-rw-   0        0        0     1130 2023-06-27 11:39:40.000000 pylibCZIrw-3.4.1/libs/pybind11/tools/setup_main.py.in
+drwxrwxrwx   0        0        0        0 2023-06-27 11:40:23.712123 pylibCZIrw-3.4.1/pylibCZIrw/
+-rw-rw-rw-   0        0        0      896 2023-06-27 11:39:34.000000 pylibCZIrw-3.4.1/pylibCZIrw/__init__.py
+-rw-rw-rw-   0        0        0    44330 2023-06-27 11:39:34.000000 pylibCZIrw-3.4.1/pylibCZIrw/czi.py
+-rw-rw-rw-   0        0        0   578662 2023-06-27 11:39:34.000000 pylibCZIrw-3.4.1/pylibCZIrw-documentation.html
+drwxrwxrwx   0        0        0        0 2023-06-27 11:40:23.712123 pylibCZIrw-3.4.1/pylibCZIrw.egg-info/
+-rw-rw-rw-   0        0        0     3026 2023-06-27 11:40:23.000000 pylibCZIrw-3.4.1/pylibCZIrw.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    20816 2023-06-27 11:40:23.000000 pylibCZIrw-3.4.1/pylibCZIrw.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-27 11:40:23.000000 pylibCZIrw-3.4.1/pylibCZIrw.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-06-27 11:40:23.000000 pylibCZIrw-3.4.1/pylibCZIrw.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       22 2023-06-27 11:40:23.000000 pylibCZIrw-3.4.1/pylibCZIrw.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       23 2023-06-27 11:40:23.000000 pylibCZIrw-3.4.1/pylibCZIrw.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1631 2023-06-27 11:40:23.712123 pylibCZIrw-3.4.1/setup.cfg
+-rw-rw-rw-   0        0        0     4599 2023-06-27 11:39:34.000000 pylibCZIrw-3.4.1/setup.py
```

### Comparing `pylibCZIrw-3.4.0/CMakeLists.txt` & `pylibCZIrw-3.4.1/CMakeLists.txt`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 set(CMAKE_MACOSX_RPATH 1)
 
 IF (APPLE)
     set(CMAKE_OSX_DEPLOYMENT_TARGET "10.9" CACHE STRING "Minimum OS X deployment version" FORCE)
 ENDIF(APPLE)
 
-project(_pylibCZIrw VERSION 3.4.0)
+project(_pylibCZIrw VERSION 3.4.1)
 
 set(CMAKE_CXX_STANDARD 17)
 set(CMAKE_CXX_STANDARD_REQUIRED ON)
 
 IF (WIN32)
     set(PYBIND11_CPP_STANDARD /std:c++17)
 ELSE()
```

### Comparing `pylibCZIrw-3.4.0/CMakeSettings.json` & `pylibCZIrw-3.4.1/CMakeSettings.json`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/COPYING.LESSER.txt` & `pylibCZIrw-3.4.1/COPYING.LESSER.txt`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/COPYING.txt` & `pylibCZIrw-3.4.1/COPYING.txt`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/INFO.md` & `pylibCZIrw-3.4.1/INFO.md`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/PKG-INFO` & `pylibCZIrw-3.4.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pylibCZIrw
-Version: 3.4.0
+Version: 3.4.1
 Summary: A python wrapper around the libCZI C++ library with reading and writing functionality.
 Home-page: UNKNOWN
 Author: Felix Scheffler
 Author-email: felix.scheffler@zeiss.com
 License: UNKNOWN
 Keywords: czi,imaging
 Platform: UNKNOWN
```

### Comparing `pylibCZIrw-3.4.0/_pylibCZIrw/src/api/CZIreadAPI.cpp` & `pylibCZIrw-3.4.1/_pylibCZIrw/src/api/CZIreadAPI.cpp`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/_pylibCZIrw/src/api/CZIreadAPI.h` & `pylibCZIrw-3.4.1/_pylibCZIrw/src/api/CZIreadAPI.h`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/_pylibCZIrw/src/api/CZIwriteAPI.cpp` & `pylibCZIrw-3.4.1/_pylibCZIrw/src/api/CZIwriteAPI.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -125,54 +125,56 @@
         scaleInfo.scaleZ = scaleZ.value();
     }
 
     MetadataUtils::WriteScalingInfo(mdBldr.get(), scaleInfo);
 
     // Add DisplaySettings
     // see test_DisplaySettings.cpp -> TEST(DisplaySettings, WriteDisplaySettingsToDocumentAndReadFromThereAndCompare) for an explanation on this process)
-    DisplaySettingsPOD display_settings;
-    ChannelDisplaySettingsPOD channel_display_setting;
-    for (const auto& entry : displaySettings)
+    if (displaySettings.size())
     {
-        channel_display_setting.Clear();
-        channel_display_setting.isEnabled = entry.second.isEnabled;
-        channel_display_setting.tintingColor = entry.second.tintingColor;
-        channel_display_setting.blackPoint = entry.second.blackPoint;
-        channel_display_setting.whitePoint = entry.second.whitePoint;
-        switch (entry.second.tintingMode)
+        DisplaySettingsPOD display_settings;
+        ChannelDisplaySettingsPOD channel_display_setting;
+        for (const auto& entry : displaySettings)
         {
-        case TintingModeEnum::Color:
-            channel_display_setting.tintingMode = libCZI::IDisplaySettings::TintingMode::Color;
-            break;
-            case TintingModeEnum::LookUpTableExplicit:
-            channel_display_setting.tintingMode = libCZI::IDisplaySettings::TintingMode::LookUpTableExplicit;
-            break;
-        case TintingModeEnum::LookUpTableWellKnown:
-            channel_display_setting.tintingMode = libCZI::IDisplaySettings::TintingMode::LookUpTableWellKnown;
-            break;
-        default:
-            channel_display_setting.tintingMode = libCZI::IDisplaySettings::TintingMode::None;
-            break;
+            channel_display_setting.Clear();
+            channel_display_setting.isEnabled = entry.second.isEnabled;
+            channel_display_setting.tintingColor = entry.second.tintingColor;
+            channel_display_setting.blackPoint = entry.second.blackPoint;
+            channel_display_setting.whitePoint = entry.second.whitePoint;
+            switch (entry.second.tintingMode)
+            {
+            case TintingModeEnum::Color:
+                channel_display_setting.tintingMode = libCZI::IDisplaySettings::TintingMode::Color;
+                break;
+                case TintingModeEnum::LookUpTableExplicit:
+                channel_display_setting.tintingMode = libCZI::IDisplaySettings::TintingMode::LookUpTableExplicit;
+                break;
+            case TintingModeEnum::LookUpTableWellKnown:
+                channel_display_setting.tintingMode = libCZI::IDisplaySettings::TintingMode::LookUpTableWellKnown;
+                break;
+            default:
+                channel_display_setting.tintingMode = libCZI::IDisplaySettings::TintingMode::None;
+                break;
+            }
+            display_settings.channelDisplaySettings[entry.first] = (channel_display_setting);
         }
 
-        display_settings.channelDisplaySettings[entry.first] = (channel_display_setting);
+        MetadataUtils::WriteDisplaySettings(mdBldr.get(), DisplaySettingsPOD::CreateIDisplaySettingSp(display_settings).get());
     }
 
-    MetadataUtils::WriteDisplaySettings(mdBldr.get(), DisplaySettingsPOD::CreateIDisplaySettingSp(display_settings).get());
-
     // Add custom attributes
     for (const auto& it : customAttributes)
     {
         const auto& key = it.first;
         const auto& value = it.second;
         MetadataUtils::SetOrAddCustomKeyValuePair(mdBldr.get(), key, value);
     }
 
    mdBldr->GetRootNode()->GetOrCreateChildNode("Metadata/Information/Application/Name")->SetValue("pylibCZIrw");
-   mdBldr->GetRootNode()->GetOrCreateChildNode("Metadata/Information/Application/Version")->SetValue("3.4.0");
+   mdBldr->GetRootNode()->GetOrCreateChildNode("Metadata/Information/Application/Version")->SetValue("3.4.1");
 
     // the resulting metadata-information is written to the CZI here
     auto xml = mdBldr->GetXml();
     WriteMetadataInfo writerMdInfo;
     writerMdInfo.Clear();
     writerMdInfo.szMetadata = xml.c_str();
     writerMdInfo.szMetadataSize = xml.size();
```

### Comparing `pylibCZIrw-3.4.0/_pylibCZIrw/src/api/CZIwriteAPI.h` & `pylibCZIrw-3.4.1/_pylibCZIrw/src/api/CZIwriteAPI.h`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/_pylibCZIrw/src/api/DllMain.cpp` & `pylibCZIrw-3.4.1/_pylibCZIrw/src/api/DllMain.cpp`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/_pylibCZIrw/src/api/PImage.cpp` & `pylibCZIrw-3.4.1/_pylibCZIrw/src/api/PImage.cpp`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/_pylibCZIrw/src/api/PImage.h` & `pylibCZIrw-3.4.1/_pylibCZIrw/src/api/PImage.h`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/_pylibCZIrw/src/bindings/CZIrw.cpp` & `pylibCZIrw-3.4.1/_pylibCZIrw/src/bindings/CZIrw.cpp`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/_pylibCZIrw/src/bindings/PbHelper.cpp` & `pylibCZIrw-3.4.1/_pylibCZIrw/src/bindings/PbHelper.cpp`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/_pylibCZIrw/src/bindings/PbHelper.h` & `pylibCZIrw-3.4.1/_pylibCZIrw/src/bindings/PbHelper.h`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/_pylibCZIrw/tests/main.cpp` & `pylibCZIrw-3.4.1/_pylibCZIrw/tests/main.cpp`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/libCZIrw/.editorconfig` & `pylibCZIrw-3.4.1/libs/libCZIrw/.editorconfig`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/libCZIrw/.github/ISSUE_TEMPLATE/bug_report.md` & `pylibCZIrw-3.4.1/libs/libCZIrw/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/libCZIrw/.github/ISSUE_TEMPLATE/feature_request.md` & `pylibCZIrw-3.4.1/libs/libCZIrw/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/libCZIrw/.github/PULL_REQUEST_TEMPLATE.md` & `pylibCZIrw-3.4.1/libs/libCZIrw/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/libCZIrw/.github/workflows/cla.yml` & `pylibCZIrw-3.4.1/libs/libCZIrw/.github/workflows/cla.yml`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/libCZIrw/.github/workflows/cmake.yml` & `pylibCZIrw-3.4.1/libs/libCZIrw/.github/workflows/cmake.yml`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/libCZIrw/.github/workflows/codeql.yml` & `pylibCZIrw-3.4.1/libs/libCZIrw/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/libCZIrw/.github/workflows/mega-linter.yml` & `pylibCZIrw-3.4.1/libs/libCZIrw/.github/workflows/mega-linter.yml`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/libCZIrw/.github/workflows/pages.yml` & `pylibCZIrw-3.4.1/libs/libCZIrw/.github/workflows/pages.yml`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/libCZIrw/.gitignore` & `pylibCZIrw-3.4.1/libs/libCZIrw/.gitignore`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/libCZIrw/.mega-linter.yml` & `pylibCZIrw-3.4.1/libs/libCZIrw/.mega-linter.yml`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/libCZIrw/.reuse/dep5` & `pylibCZIrw-3.4.1/libs/libCZIrw/.reuse/dep5`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/libCZIrw/CMakeLists.txt` & `pylibCZIrw-3.4.1/libs/libCZIrw/CMakeLists.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 cmake_minimum_required(VERSION 3.15)
 
 cmake_policy(SET CMP0091 NEW) # enable new "MSVC runtime library selection" (https://cmake.org/cmake/help/latest/variable/CMAKE_MSVC_RUNTIME_LIBRARY.html)
 
 project(libCZI 
-      VERSION 0.48.0
+      VERSION 0.49.0
       HOMEPAGE_URL "https://github.com/ZEISS/libczi"
       DESCRIPTION "libCZI is an Open Source Cross-Platform C++ library to read and write CZI")
 
 list (APPEND CMAKE_MODULE_PATH "${CMAKE_CURRENT_SOURCE_DIR}/cmake")
 
 include(GNUInstallDirs)
 
@@ -92,13 +92,14 @@
 option(LIBCZI_BUILD_PREFER_EXTERNALPACKAGE_EIGEN3 "Prefer an Eigen3-package present on the system" OFF)
 
 # With this option, we try to use an existing zstd-library. Note: this seems to work with vcpkg, but
 #  on Debian it seems that the package "libzstd-dev" does not have the required CMake-config-file.
 #  See here: https://discourse.cmake.org/t/findzstd/3506
 option(LIBCZI_BUILD_PREFER_EXTERNALPACKAGE_ZSTD "Prefer a ZSTD-package present on the system" OFF)
 
-
 if (LIBCZI_BUILD_UNITTESTS)
+ include (CTest)
  enable_testing()
 endif()
 
-add_subdirectory(Src)
+add_subdirectory(Src)
+
```

### Comparing `pylibCZIrw-3.4.0/libs/libCZIrw/CODE_OF_CONDUCT.md` & `pylibCZIrw-3.4.1/libs/libCZIrw/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/libCZIrw/CONTRIBUTING.md` & `pylibCZIrw-3.4.1/libs/libCZIrw/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/libCZIrw/COPYING` & `pylibCZIrw-3.4.1/libs/libCZIrw/COPYING`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/libCZIrw/COPYING.LESSER` & `pylibCZIrw-3.4.1/libs/libCZIrw/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/libCZIrw/CPPLINT.cfg` & `pylibCZIrw-3.4.1/libs/libCZIrw/CPPLINT.cfg`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/libCZIrw/LICENSES/BSD-3-Clause.txt` & `pylibCZIrw-3.4.1/libs/libCZIrw/LICENSES/BSD-3-Clause.txt`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/libCZIrw/LICENSES/CC0-1.0.txt` & `pylibCZIrw-3.4.1/libs/libCZIrw/LICENSES/CC0-1.0.txt`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/libCZIrw/LICENSES/LGPL-3.0-or-later.txt` & `pylibCZIrw-3.4.1/libs/libCZIrw/LICENSES/LGPL-3.0-or-later.txt`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/libCZIrw/LICENSES/MIT.txt` & `pylibCZIrw-3.4.1/libs/libCZIrw/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/libCZIrw/LICENSES/RSA-MD.txt` & `pylibCZIrw-3.4.1/libs/libCZIrw/LICENSES/RSA-MD.txt`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/libCZIrw/README.md` & `pylibCZIrw-3.4.1/libs/libCZIrw/README.md`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/libCZIrw/SECURITY.md` & `pylibCZIrw-3.4.1/libs/libCZIrw/SECURITY.md`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/libCZIrw/Src/Doxyfile` & `pylibCZIrw-3.4.1/libs/libCZIrw/Src/Doxyfile`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/libCZIrw/Src/JxrDecode/CMakeLists.txt` & `pylibCZIrw-3.4.1/libs/libCZIrw/Src/JxrDecode/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/libCZIrw/Src/JxrDecode/Jxr/JXRGlue.c` & `pylibCZIrw-3.4.1/libs/libCZIrw/Src/JxrDecode/Jxr/JXRGlue.c`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/libCZIrw/Src/JxrDecode/Jxr/JXRGlue.h` & `pylibCZIrw-3.4.1/libs/libCZIrw/Src/JxrDecode/Jxr/JXRGlue.h`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/libCZIrw/Src/JxrDecode/Jxr/JXRGlueJxr.c` & `pylibCZIrw-3.4.1/libs/libCZIrw/Src/JxrDecode/Jxr/JXRGlueJxr.c`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/libCZIrw/Src/JxrDecode/Jxr/JXRGluePFC.c` & `pylibCZIrw-3.4.1/libs/libCZIrw/Src/JxrDecode/Jxr/JXRGluePFC.c`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/libCZIrw/Src/JxrDecode/Jxr/JXRMeta.c` & `pylibCZIrw-3.4.1/libs/libCZIrw/Src/JxrDecode/Jxr/JXRMeta.c`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/libCZIrw/Src/JxrDecode/Jxr/JXRMeta.h` & `pylibCZIrw-3.4.1/libs/libCZIrw/Src/JxrDecode/Jxr/JXRMeta.h`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/libCZIrw/Src/JxrDecode/Jxr/JXRTest.c` & `pylibCZIrw-3.4.1/libs/libCZIrw/Src/JxrDecode/Jxr/JXRTest.c`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/libCZIrw/Src/JxrDecode/Jxr/JXRTest.h` & `pylibCZIrw-3.4.1/libs/libCZIrw/Src/JxrDecode/Jxr/JXRTest.h`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/libCZIrw/Src/JxrDecode/Jxr/JXRTestBmp.c` & `pylibCZIrw-3.4.1/libs/libCZIrw/Src/JxrDecode/Jxr/JXRTestBmp.c`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/libCZIrw/Src/JxrDecode/Jxr/JXRTestHdr.c` & `pylibCZIrw-3.4.1/libs/libCZIrw/Src/JxrDecode/Jxr/JXRTestHdr.c`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/libCZIrw/Src/JxrDecode/Jxr/JXRTestPnm.c` & `pylibCZIrw-3.4.1/libs/libCZIrw/Src/JxrDecode/Jxr/JXRTestPnm.c`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/libCZIrw/Src/JxrDecode/Jxr/JXRTestTif.c` & `pylibCZIrw-3.4.1/libs/libCZIrw/Src/JxrDecode/Jxr/JXRTestTif.c`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/libCZIrw/Src/JxrDecode/Jxr/JXRTestWrapper.c` & `pylibCZIrw-3.4.1/libs/libCZIrw/Src/JxrDecode/Jxr/JXRTestWrapper.c`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/libCZIrw/Src/JxrDecode/Jxr/JXRTestYUV.c` & `pylibCZIrw-3.4.1/libs/libCZIrw/Src/JxrDecode/Jxr/JXRTestYUV.c`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/libCZIrw/Src/JxrDecode/Jxr/JXRTranscode.c` & `pylibCZIrw-3.4.1/libs/libCZIrw/Src/JxrDecode/Jxr/JXRTranscode.c`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/libCZIrw/Src/JxrDecode/Jxr/_x86/_x86.h` & `pylibCZIrw-3.4.1/libs/libCZIrw/Src/JxrDecode/Jxr/_x86/_x86.h`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/libCZIrw/Src/JxrDecode/Jxr/adapthuff.c` & `pylibCZIrw-3.4.1/libs/libCZIrw/Src/JxrDecode/Jxr/adapthuff.c`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/libCZIrw/Src/JxrDecode/Jxr/ansi.h` & `pylibCZIrw-3.4.1/libs/libCZIrw/Src/JxrDecode/Jxr/ansi.h`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/libCZIrw/Src/JxrDecode/Jxr/common.h` & `pylibCZIrw-3.4.1/libs/libCZIrw/Src/JxrDecode/Jxr/common.h`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/libCZIrw/Src/JxrDecode/Jxr/decode.c` & `pylibCZIrw-3.4.1/libs/libCZIrw/Src/JxrDecode/Jxr/decode.c`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/libCZIrw/Src/JxrDecode/Jxr/decode.h` & `pylibCZIrw-3.4.1/libs/libCZIrw/Src/JxrDecode/Jxr/decode.h`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/libCZIrw/Src/JxrDecode/Jxr/encode.c` & `pylibCZIrw-3.4.1/libs/libCZIrw/Src/JxrDecode/Jxr/encode.c`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/libCZIrw/Src/JxrDecode/Jxr/encode.h` & `pylibCZIrw-3.4.1/libs/libCZIrw/Src/JxrDecode/Jxr/encode.h`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/libCZIrw/Src/JxrDecode/Jxr/image.c` & `pylibCZIrw-3.4.1/libs/libCZIrw/Src/JxrDecode/Jxr/image.c`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/libCZIrw/Src/JxrDecode/Jxr/perfTimer.h` & `pylibCZIrw-3.4.1/libs/libCZIrw/Src/JxrDecode/Jxr/perfTimer.h`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/libCZIrw/Src/JxrDecode/Jxr/perfTimerANSI.c` & `pylibCZIrw-3.4.1/libs/libCZIrw/Src/JxrDecode/Jxr/perfTimerANSI.c`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/libCZIrw/Src/JxrDecode/Jxr/postprocess.c` & `pylibCZIrw-3.4.1/libs/libCZIrw/Src/JxrDecode/Jxr/postprocess.c`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/libCZIrw/Src/JxrDecode/Jxr/priv_guiddef.h` & `pylibCZIrw-3.4.1/libs/libCZIrw/Src/JxrDecode/Jxr/priv_guiddef.h`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/libCZIrw/Src/JxrDecode/Jxr/segdec.c` & `pylibCZIrw-3.4.1/libs/libCZIrw/Src/JxrDecode/Jxr/segdec.c`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/libCZIrw/Src/JxrDecode/Jxr/segenc.c` & `pylibCZIrw-3.4.1/libs/libCZIrw/Src/JxrDecode/Jxr/segenc.c`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/libCZIrw/Src/JxrDecode/Jxr/strFwdTransform.c` & `pylibCZIrw-3.4.1/libs/libCZIrw/Src/JxrDecode/Jxr/strFwdTransform.c`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/libCZIrw/Src/JxrDecode/Jxr/strInvTransform.c` & `pylibCZIrw-3.4.1/libs/libCZIrw/Src/JxrDecode/Jxr/strInvTransform.c`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/libCZIrw/Src/JxrDecode/Jxr/strPredQuant.c` & `pylibCZIrw-3.4.1/libs/libCZIrw/Src/JxrDecode/Jxr/strPredQuant.c`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/libCZIrw/Src/JxrDecode/Jxr/strPredQuantDec.c` & `pylibCZIrw-3.4.1/libs/libCZIrw/Src/JxrDecode/Jxr/strPredQuantDec.c`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/libCZIrw/Src/JxrDecode/Jxr/strPredQuantEnc.c` & `pylibCZIrw-3.4.1/libs/libCZIrw/Src/JxrDecode/Jxr/strPredQuantEnc.c`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/libCZIrw/Src/JxrDecode/Jxr/strTransform.c` & `pylibCZIrw-3.4.1/libs/libCZIrw/Src/JxrDecode/Jxr/strTransform.c`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/libCZIrw/Src/JxrDecode/Jxr/strTransform.h` & `pylibCZIrw-3.4.1/libs/libCZIrw/Src/JxrDecode/Jxr/strTransform.h`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/libCZIrw/Src/JxrDecode/Jxr/strcodec.c` & `pylibCZIrw-3.4.1/libs/libCZIrw/Src/JxrDecode/Jxr/strcodec.c`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/libCZIrw/Src/JxrDecode/Jxr/strcodec.h` & `pylibCZIrw-3.4.1/libs/libCZIrw/Src/JxrDecode/Jxr/strcodec.h`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/libCZIrw/Src/JxrDecode/Jxr/strdec.c` & `pylibCZIrw-3.4.1/libs/libCZIrw/Src/JxrDecode/Jxr/strdec.c`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/libCZIrw/Src/JxrDecode/Jxr/strdec_x86.c` & `pylibCZIrw-3.4.1/libs/libCZIrw/Src/JxrDecode/Jxr/strdec_x86.c`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/libCZIrw/Src/JxrDecode/Jxr/strenc.c` & `pylibCZIrw-3.4.1/libs/libCZIrw/Src/JxrDecode/Jxr/strenc.c`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/libCZIrw/Src/JxrDecode/Jxr/strenc_x86.c` & `pylibCZIrw-3.4.1/libs/libCZIrw/Src/JxrDecode/Jxr/strenc_x86.c`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/libCZIrw/Src/JxrDecode/Jxr/windowsmediaphoto.h` & `pylibCZIrw-3.4.1/libs/libCZIrw/Src/JxrDecode/Jxr/windowsmediaphoto.h`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/libCZIrw/Src/JxrDecode/Jxr/wmsal.h` & `pylibCZIrw-3.4.1/libs/libCZIrw/Src/JxrDecode/Jxr/wmsal.h`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/libCZIrw/Src/JxrDecode/Jxr/wmspecstring.h` & `pylibCZIrw-3.4.1/libs/libCZIrw/Src/JxrDecode/Jxr/wmspecstring.h`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/libCZIrw/Src/JxrDecode/Jxr/wmspecstrings_adt.h` & `pylibCZIrw-3.4.1/libs/libCZIrw/Src/JxrDecode/Jxr/wmspecstrings_adt.h`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/libCZIrw/Src/JxrDecode/Jxr/wmspecstrings_strict.h` & `pylibCZIrw-3.4.1/libs/libCZIrw/Src/JxrDecode/Jxr/wmspecstrings_strict.h`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/libCZIrw/Src/JxrDecode/Jxr/wmspecstrings_undef.h` & `pylibCZIrw-3.4.1/libs/libCZIrw/Src/JxrDecode/Jxr/wmspecstrings_undef.h`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/libCZIrw/Src/JxrDecode/JxrDecode.cpp` & `pylibCZIrw-3.4.1/libs/libCZIrw/Src/JxrDecode/JxrDecode.cpp`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/libCZIrw/Src/JxrDecode/JxrDecode.h` & `pylibCZIrw-3.4.1/libs/libCZIrw/Src/JxrDecode/JxrDecode.h`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/BitmapOperations.cpp` & `pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/BitmapOperations.cpp`

 * *Files 16% similar despite different names*

```diff
@@ -85,21 +85,29 @@
         default:break;
         }
         break;
 
     case PixelType::Gray16:
         switch (dstPixelType)
         {
-        case PixelType::Gray8:break;
+        case PixelType::Gray8:
+            Copy<PixelType::Gray16, PixelType::Gray8>(srcPtr, srcStride, dstPtr, dstStride, width, height, drawTileBorder);
+            return;
         case PixelType::Gray16:
             Copy<PixelType::Gray16, PixelType::Gray16>(srcPtr, srcStride, dstPtr, dstStride, width, height, drawTileBorder);
             return;
-        case PixelType::Gray32Float:break;
-        case PixelType::Bgr24:break;
-        case PixelType::Bgr48:break;
+        case PixelType::Gray32Float:
+            Copy<PixelType::Gray16, PixelType::Gray32Float>(srcPtr, srcStride, dstPtr, dstStride, width, height, drawTileBorder);
+            return;
+        case PixelType::Bgr24:
+            Copy<PixelType::Gray16, PixelType::Bgr24>(srcPtr, srcStride, dstPtr, dstStride, width, height, drawTileBorder);
+            return;
+        case PixelType::Bgr48:
+            Copy<PixelType::Gray16, PixelType::Bgr48>(srcPtr, srcStride, dstPtr, dstStride, width, height, drawTileBorder);
+            return;
         default:break;
         }
         break;
 
     case PixelType::Gray32Float:
         switch (dstPixelType)
         {
@@ -135,32 +143,40 @@
         default:break;
         }
         break;
 
     case PixelType::Bgr48:
         switch (dstPixelType)
         {
-        case PixelType::Gray8:break;
-        case PixelType::Gray16:break;
-        case PixelType::Gray32Float:break;
-        case PixelType::Bgr24:break;
+        case PixelType::Gray8:
+            Copy<PixelType::Bgr48, PixelType::Gray8>(srcPtr, srcStride, dstPtr, dstStride, width, height, drawTileBorder);
+            return;
+        case PixelType::Gray16:
+            Copy<PixelType::Bgr48, PixelType::Gray16>(srcPtr, srcStride, dstPtr, dstStride, width, height, drawTileBorder);
+            return;
+        case PixelType::Gray32Float:
+            Copy<PixelType::Bgr48, PixelType::Gray32Float>(srcPtr, srcStride, dstPtr, dstStride, width, height, drawTileBorder);
+            return;
+        case PixelType::Bgr24:
+            Copy<PixelType::Bgr48, PixelType::Bgr24>(srcPtr, srcStride, dstPtr, dstStride, width, height, drawTileBorder);
+            return;
         case PixelType::Bgr48:
             Copy<PixelType::Bgr48, PixelType::Bgr48>(srcPtr, srcStride, dstPtr, dstStride, width, height, drawTileBorder);
             return;
         default:break;
         }
         break;
 
     default:break;
     }
 
     throw std::logic_error("It seems that this conversion is not implemented...");
 }
 
-/*static*/void CBitmapOperations::CopyOffseted(const CopyOffsetedInfo& info)
+/*static*/void CBitmapOperations::CopyWithOffset(const CopyWithOffsetInfo& info)
 {
     const IntRect srcRect = IntRect{ info.xOffset,info.yOffset,info.srcWidth,info.srcHeight };
     const IntRect dstRect = IntRect{ 0,0,info.dstWidth,info.dstHeight };
     const IntRect intersection = Utilities::Intersect(srcRect, dstRect);
 
     if (intersection.w == 0 || intersection.h == 0)
     {
```

### Comparing `pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/BitmapOperations.hpp` & `pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/BitmapOperations.hpp`

 * *Files 13% similar despite different names*

```diff
@@ -359,14 +359,54 @@
     Copy<libCZI::PixelType::Bgr24, libCZI::PixelType::Gray16, CConvBgr24ToGray16>(CConvBgr24ToGray16(), srcPtr, srcStride, dstPtr, dstStride, width, height, drawTileBorder);
 }
 template <>
 inline void CBitmapOperations::Copy<libCZI::PixelType::Bgr24, libCZI::PixelType::Bgr48>(const void* srcPtr, int srcStride, void* dstPtr, int dstStride, int width, int height, bool drawTileBorder)
 {
     Copy<libCZI::PixelType::Bgr24, libCZI::PixelType::Bgr48, CConvBgr24ToBgr48>(CConvBgr24ToBgr48(), srcPtr, srcStride, dstPtr, dstStride, width, height, drawTileBorder);
 }
+template <>
+inline void CBitmapOperations::Copy<libCZI::PixelType::Gray16, libCZI::PixelType::Gray8>(const void* srcPtr, int srcStride, void* dstPtr, int dstStride, int width, int height, bool drawTileBorder)
+{
+    Copy<libCZI::PixelType::Gray16, libCZI::PixelType::Gray8, CConvGray16ToGray8>(CConvGray16ToGray8(), srcPtr, srcStride, dstPtr, dstStride, width, height, drawTileBorder);
+}
+template <>
+inline void CBitmapOperations::Copy<libCZI::PixelType::Gray16, libCZI::PixelType::Gray32Float>(const void* srcPtr, int srcStride, void* dstPtr, int dstStride, int width, int height, bool drawTileBorder)
+{
+    Copy<libCZI::PixelType::Gray16, libCZI::PixelType::Gray32Float, CConvGray16ToGray32Float>(CConvGray16ToGray32Float(), srcPtr, srcStride, dstPtr, dstStride, width, height, drawTileBorder);
+}
+template <>
+inline void CBitmapOperations::Copy<libCZI::PixelType::Gray16, libCZI::PixelType::Bgr24>(const void* srcPtr, int srcStride, void* dstPtr, int dstStride, int width, int height, bool drawTileBorder)
+{
+    Copy<libCZI::PixelType::Gray16, libCZI::PixelType::Bgr24, CConvGray16ToBgr24>(CConvGray16ToBgr24(), srcPtr, srcStride, dstPtr, dstStride, width, height, drawTileBorder);
+}
+template <>
+inline void CBitmapOperations::Copy<libCZI::PixelType::Gray16, libCZI::PixelType::Bgr48>(const void* srcPtr, int srcStride, void* dstPtr, int dstStride, int width, int height, bool drawTileBorder)
+{
+    Copy<libCZI::PixelType::Gray16, libCZI::PixelType::Bgr48, CConvGray16ToBgr48>(CConvGray16ToBgr48(), srcPtr, srcStride, dstPtr, dstStride, width, height, drawTileBorder);
+}
+template <>
+inline void CBitmapOperations::Copy<libCZI::PixelType::Bgr48, libCZI::PixelType::Gray8>(const void* srcPtr, int srcStride, void* dstPtr, int dstStride, int width, int height, bool drawTileBorder)
+{
+    Copy<libCZI::PixelType::Bgr48, libCZI::PixelType::Gray8, CConvBgr48ToGray8>(CConvBgr48ToGray8(), srcPtr, srcStride, dstPtr, dstStride, width, height, drawTileBorder);
+}
+template <>
+inline void CBitmapOperations::Copy<libCZI::PixelType::Bgr48, libCZI::PixelType::Gray16>(const void* srcPtr, int srcStride, void* dstPtr, int dstStride, int width, int height, bool drawTileBorder)
+{
+    Copy<libCZI::PixelType::Bgr48, libCZI::PixelType::Gray16, CConvBgr48ToGray16>(CConvBgr48ToGray16(), srcPtr, srcStride, dstPtr, dstStride, width, height, drawTileBorder);
+}
+template <>
+inline void CBitmapOperations::Copy<libCZI::PixelType::Bgr48, libCZI::PixelType::Gray32Float>(const void* srcPtr, int srcStride, void* dstPtr, int dstStride, int width, int height, bool drawTileBorder)
+{
+    Copy<libCZI::PixelType::Bgr48, libCZI::PixelType::Gray32Float, CConvBgr48ToGray32Float>(CConvBgr48ToGray32Float(), srcPtr, srcStride, dstPtr, dstStride, width, height, drawTileBorder);
+}
+template <>
+inline void CBitmapOperations::Copy<libCZI::PixelType::Bgr48, libCZI::PixelType::Bgr24>(const void* srcPtr, int srcStride, void* dstPtr, int dstStride, int width, int height, bool drawTileBorder)
+{
+    Copy<libCZI::PixelType::Bgr48, libCZI::PixelType::Bgr24, CConvBgr48ToBgr24>(CConvBgr48ToBgr24(), srcPtr, srcStride, dstPtr, dstStride, width, height, drawTileBorder);
+}
 
 //------------------------------------------------------------------------------------------------------------
 
 template <libCZI::PixelType tSrcPixelType, libCZI::PixelType tDstPixelType, typename tPixelConverter, typename tFlt>
 inline void CBitmapOperations::InternalNNScale2(const tPixelConverter& conv, const NNResizeInfo2<tFlt>& resizeInfo)
 {
     constexpr uint8_t bytesPerPelSrc = CziUtils::BytesPerPel<tSrcPixelType>();
```

### Comparing `pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/CMakeLists.txt` & `pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/CMakeLists.txt`

 * *Files 1% similar despite different names*

```diff
@@ -211,21 +211,23 @@
 
 if (LIBCZI_BUILD_PREFER_EXTERNALPACKAGE_ZSTD)
   find_package(zstd CONFIG REQUIRED)
 else()
   FetchContent_Declare(
     zstd
     GIT_REPOSITORY https://github.com/facebook/zstd.git
-    GIT_TAG "v1.5.4"
+    GIT_TAG "v1.5.5"
   )
 
   if(NOT zstd_POPULATED)
     message(STATUS "Fetching zstd...")
     set(ZSTD_BUILD_PROGRAMS  OFF CACHE BOOL "" FORCE)
     set(ZSTD_BUILD_SHARED    OFF CACHE BOOL "" FORCE)
+    set(ZSTD_BUILD_TESTS     OFF CACHE BOOL "" FORCE)
+    set(ZSTD_BUILD_CONTRIB   OFF CACHE BOOL "" FORCE)
 
     FetchContent_Populate(zstd)
 
     add_subdirectory(${zstd_SOURCE_DIR}/build/cmake ${zstd_BINARY_DIR})
   endif()
 endif()
```

### Comparing `pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/CZIReader.cpp` & `pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/CZIReader.cpp`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/CZIReader.h` & `pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/CZIReader.h`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/CreateBitmap.cpp` & `pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/CreateBitmap.cpp`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/CziAttachment.cpp` & `pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/CziAttachment.cpp`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/CziAttachment.h` & `pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/CziAttachment.h`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/CziAttachmentsDirectory.cpp` & `pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/CziAttachmentsDirectory.cpp`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/CziAttachmentsDirectory.h` & `pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/CziAttachmentsDirectory.h`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/CziDimensionInfo.cpp` & `pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/CziDimensionInfo.cpp`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/CziDimensionInfo.h` & `pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/CziDimensionInfo.h`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/CziDisplaySettings.cpp` & `pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/CziDisplaySettings.cpp`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/CziDisplaySettings.h` & `pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/CziDisplaySettings.h`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/CziMetadata.cpp` & `pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/CziMetadata.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -182,15 +182,15 @@
             //  therefore we have this work-around
             uint64_t v = stoull(s, idx);
             if (v > (numeric_limits<uint32_t>::max)())
             {
                 throw out_of_range("value was out-of-range");
             }
 
-            return (uint32_t)v;
+            return static_cast<uint32_t>(v);
         }
     };
 
     return TryConvert<conv>(this, p);
 }
 
 bool IXmlNodeRead::TryGetValueAsInt32(std::int32_t* p)
```

### Comparing `pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/CziMetadata.h` & `pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/CziMetadata.h`

 * *Files 5% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 #include "XmlNodeWrapper.h"
 
 class CCziMetadata : public libCZI::ICziMetadata, public std::enable_shared_from_this<CCziMetadata>
 {
 private:
     struct XmlNodeWrapperThrowExcp
     {
-        static void ThrowInvalidPath()
+        [[noreturn]] static void ThrowInvalidPath()
         {
             throw libCZI::LibCZIMetadataException("invalid path", libCZI::LibCZIMetadataException::ErrorType::InvalidPath);
         }
     };
 
     pugi::xml_parse_result   parseResult;
     pugi::xml_document doc;
```

### Comparing `pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/CziMetadataBuilder.cpp` & `pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/CziMetadataBuilder.cpp`

 * *Files 7% similar despite different names*

```diff
@@ -70,55 +70,66 @@
 
         return true;
     }
 
     return false;
 }
 
-/*virtual*/std::shared_ptr<IXmlNodeRead> CNodeWrapper::GetChildNodeReadonly(const char* path)
+pugi::xml_node CNodeWrapper::GetChildNodePathMustExist(const char* path)
 {
     auto p = Utilities::convertUtf8ToWchar_t(path);
     vector<std::wstring> tokens;
     Utilities::Tokenize(p, tokens, L"/");
     if (tokens.empty())
     {
         throw LibCZIMetadataBuilderException("invalid path", LibCZIMetadataBuilderException::ErrorType::InvalidPath);
     }
 
     if (any_of(tokens.cbegin(), tokens.cend(), [](const wstring& str) {return str.empty(); }))
     {
         throw LibCZIMetadataBuilderException("invalid path", LibCZIMetadataBuilderException::ErrorType::InvalidPath);
     }
 
-    auto node = this->GetOrCreateChildElementNodeWithAttributes(tokens[0], false);
+    auto node = XmlPathSpecifierUtilities<MetadataBuilderXmlNodeWrapperThrowExcp>::GetChildElementNodeWithAttributes(this->node, tokens[0]);
     if (!node)
     {
-        return nullptr;
+        return {};
     }
 
     for (size_t i = 1; i < tokens.size(); ++i)
     {
-        node = CNodeWrapper::GetOrCreateChildElementNodeWithAttributes(node, tokens[i].c_str(), false);
+        node = XmlPathSpecifierUtilities<MetadataBuilderXmlNodeWrapperThrowExcp>::GetChildElementNodeWithAttributes(node, tokens[i]);
         if (!node)
         {
-            return nullptr;
+            return {};
         }
     }
 
-    return std::make_shared<XmlNodeWrapperReadonly<CCZiMetadataBuilder, MetadataBuilderXmlNodeWrapperThrowExcp> >(this->builderRef, node.internal_object());
+    return node;
+}
+
+/*virtual*/std::shared_ptr<IXmlNodeRead> CNodeWrapper::GetChildNodeReadonly(const char* path)
+{
+    const auto child_node = this->GetChildNodePathMustExist(path);
+    if (!child_node)
+    {
+        return nullptr;
+    }
+
+    return std::make_shared<XmlNodeWrapperReadonly<CCZiMetadataBuilder, MetadataBuilderXmlNodeWrapperThrowExcp>>(this->builderRef, child_node.internal_object());
 }
 
 /*virtual*/void CNodeWrapper::EnumChildren(const std::function<bool(std::shared_ptr<IXmlNodeRead>)>& enumChildren)
 {
-    for (pugi::xml_node childNode = this->node.first_child(); childNode; childNode = childNode.next_sibling())
+    for (pugi::xml_node child_node = this->node.first_child(); child_node; child_node = child_node.next_sibling())
     {
-        if (childNode.type() == pugi::xml_node_type::node_element)
+        if (child_node.type() == pugi::xml_node_type::node_element)
         {
-            bool b = enumChildren(
-                std::make_shared<XmlNodeWrapperReadonly<CCZiMetadataBuilder, MetadataBuilderXmlNodeWrapperThrowExcp> >(this->builderRef, childNode.internal_object()));
+            const bool b = enumChildren(
+                std::make_shared<XmlNodeWrapperReadonly<CCZiMetadataBuilder, MetadataBuilderXmlNodeWrapperThrowExcp>>(this->builderRef, child_node.internal_object()));
             if (!b)
             {
                 break;
             }
         }
     }
 }
@@ -126,20 +137,26 @@
 /*virtual*/std::wstring CNodeWrapper::Name() const
 {
     return this->node.name();
 }
 
 /*virtual*/std::shared_ptr<IXmlNodeRw> CNodeWrapper::GetOrCreateChildNode(const char* path)
 {
-    return this->GetOrCreateChildNode(path, true);
+    return this->GetOrCreateChildNodeInternal(path);
 }
 
 /*virtual*/std::shared_ptr<IXmlNodeRw> CNodeWrapper::GetChildNode(const char* path)
 {
-    return this->GetOrCreateChildNode(path, false);
+    const auto child_node = this->GetChildNodePathMustExist(path);
+    if (!child_node)
+    {
+        return nullptr;
+    }
+
+    return std::make_shared<CNodeWrapper>(this->builderRef, child_node.internal_object());
 }
 
 /*virtual*/void CNodeWrapper::SetValue(const char* str)
 {
     this->ThrowIfCannotSetValue();
     auto pcdata = this->GetOrCreatePcDataChild();
     pcdata.set_value(Utilities::convertUtf8ToWchar_t(str).c_str());
@@ -213,15 +230,15 @@
 /*virtual*/bool CNodeWrapper::RemoveAttribute(const char* name)
 {
     return this->node.remove_attribute(Utilities::convertUtf8ToWchar_t(name).c_str());
 }
 
 //--------------------------------------------------------------------------------------
 
-std::shared_ptr<IXmlNodeRw> CNodeWrapper::GetOrCreateChildNode(const char* path, bool allowCreation)
+std::shared_ptr<IXmlNodeRw> CNodeWrapper::GetOrCreateChildNodeInternal(const char* path)
 {
     auto p = Utilities::convertUtf8ToWchar_t(path);
 
     vector<std::wstring> tokens;
     Utilities::Tokenize(p, tokens, L"/");
     if (tokens.empty())
     {
@@ -229,23 +246,23 @@
     }
 
     if (any_of(tokens.cbegin(), tokens.cend(), [](const wstring& str) {return str.empty(); }))
     {
         throw LibCZIMetadataBuilderException("invalid path", LibCZIMetadataBuilderException::ErrorType::InvalidPath);
     }
 
-    auto node = this->GetOrCreateChildElementNodeWithAttributes(tokens[0], allowCreation);
+    auto node = this->GetOrCreateChildElementNodeWithAttributes(this->node, tokens[0]);
     if (!node)
     {
         return nullptr;
     }
 
     for (size_t i = 1; i < tokens.size(); ++i)
     {
-        node = CNodeWrapper::GetOrCreateChildElementNodeWithAttributes(node, tokens[i].c_str(), allowCreation);
+        node = CNodeWrapper::GetOrCreateChildElementNodeWithAttributes(node, tokens[i]);
         if (!node)
         {
             return nullptr;
         }
     }
 
     return std::make_shared<CNodeWrapper>(this->builderRef, node.internal_object());
@@ -284,54 +301,49 @@
         // otherwise, we add a new attribute
         attribute = this->node.append_attribute(Utilities::convertUtf8ToWchar_t(name).c_str());
     }
 
     attribute.set_value(Utilities::convertUtf8ToWchar_t(value).c_str());
 }
 
-pugi::xml_node CNodeWrapper::GetOrCreateChildElementNodeWithAttributes(const std::wstring& str, bool allowCreation)
-{
-    return CNodeWrapper::GetOrCreateChildElementNodeWithAttributes(this->node, str, allowCreation);
-}
-
-/*static*/pugi::xml_node CNodeWrapper::GetOrCreateChildElementNodeWithAttributes(pugi::xml_node& node, const std::wstring& str, bool allowCreation)
+/*static*/pugi::xml_node CNodeWrapper::GetOrCreateChildElementNodeWithAttributes(pugi::xml_node& node, const std::wstring& str)
 {
     std::wregex nodenameWihtAttribregex(LR"(([^\[\]]+)(\[([^\[\]]*)\])?)");
     std::wsmatch pieces_match;
 
     if (std::regex_match(str, pieces_match, nodenameWihtAttribregex))
     {
         if (pieces_match.size() == 4)
         {
             if (pieces_match[0].matched == true && pieces_match[1].matched == true)
             {
                 wstring nodeName = pieces_match[1];
                 if (pieces_match[2].matched == false && pieces_match[3].matched == false)
                 {
                     // we only got a name ( not followed by [Id=abc] )
-                    return GetOrCreateChildElementNode(node, nodeName.c_str(), allowCreation);
+                    return GetOrCreateChildElementNode(node, nodeName.c_str());
                 }
                 else if (pieces_match[2].matched == true && pieces_match[3].matched == true)
                 {
                     const auto attribValuePairs = CNodeWrapper::ParseAttributes(pieces_match[3]);
-                    return GetOrCreateChildElementNodeWithAttributes(node, nodeName, attribValuePairs, allowCreation);
+                    return GetOrCreateChildElementNodeWithAttributes(node, nodeName, attribValuePairs);
                 }
             }
         }
     }
 
     throw LibCZIMetadataBuilderException("invalid path", LibCZIMetadataBuilderException::ErrorType::InvalidPath);
 }
 
-pugi::xml_node CNodeWrapper::GetOrCreateChildElementNode(const wchar_t* sz, bool allowCreation)
+pugi::xml_node CNodeWrapper::GetOrCreateChildElementNode(const wchar_t* sz)
 {
-    return CNodeWrapper::GetOrCreateChildElementNode(this->node, sz, allowCreation);
+    return CNodeWrapper::GetOrCreateChildElementNode(this->node, sz);
 }
 
-/*static*/pugi::xml_node CNodeWrapper::GetOrCreateChildElementNodeWithAttributes(pugi::xml_node& node, const std::wstring& str, const std::map<std::wstring, std::wstring>& attribs, bool allowCreation)
+/*static*/pugi::xml_node CNodeWrapper::GetOrCreateChildElementNodeWithAttributes(pugi::xml_node& node, const std::wstring& str, const std::map<std::wstring, std::wstring>& attribs)
 {
     struct find_element_node_and_attributes
     {
         const wchar_t* nodeName;
         const std::map<std::wstring, std::wstring>& attribs;
 
         bool operator()(pugi::xml_node node) const
@@ -367,32 +379,27 @@
             return true;
         }
     };
 
     auto c = node.find_child(find_element_node_and_attributes{ str.c_str(), attribs });
     if (!c)
     {
-        if (!allowCreation)
-        {
-            return xml_node();
-        }
-
         auto newNode = node.append_child(str.c_str());
         for (auto it = attribs.cbegin(); it != attribs.cend(); ++it)
         {
             newNode.append_attribute(it->first.c_str()).set_value(it->second.c_str());
         }
 
         return newNode;
     }
 
     return c;
 }
 
-/*static*/pugi::xml_node CNodeWrapper::GetOrCreateChildElementNode(pugi::xml_node& node, const wchar_t* sz, bool allowCreation)
+/*static*/pugi::xml_node CNodeWrapper::GetOrCreateChildElementNode(pugi::xml_node& node, const wchar_t* sz)
 {
     struct find_element_node
     {
         const wchar_t* nodeName;
 
         bool operator()(pugi::xml_node node) const
         {
@@ -404,19 +411,14 @@
             return wcscmp(node.name(), this->nodeName) == 0;
         }
     };
 
     auto c = node.find_child(find_element_node{ sz });
     if (!c)
     {
-        if (!allowCreation)
-        {
-            return xml_node();
-        }
-
         return node.append_child(sz);
     }
 
     return c;
 }
 
 /*static*/std::map<wstring, wstring> CNodeWrapper::ParseAttributes(const std::wstring& str)
@@ -538,15 +540,15 @@
         {
             s.append(",Name=");
             s.append(get<1>(get<1>(idAndOptionalName)));
         }
 
         s.append("]");
 
-        auto channelNode = root->GetOrCreateChildNode(s.c_str());
+        const auto channelNode = root->GetOrCreateChildNode(s.c_str());
 
         auto pxlTypeIterator = pixelTypeForChannel.GetChannelIndexPixelTypeMap().find(ch);
         if (pxlTypeIterator != pixelTypeForChannel.GetChannelIndexPixelTypeMap().end())
         {
             int pxlTypeInt = pxlTypeIterator->second;
             string pixelTypeString;;
             PixelType pxlType = CziUtils::PixelTypeFromInt(pxlTypeInt);
@@ -607,15 +609,15 @@
         str = "Gray64ComplexFloat";
         break;
     case PixelType::Bgr192ComplexFloat:
         str = "Bgr192ComplexFloat";
         break;
     default:
         return false;
-    };
+    }
 
     return true;
 }
 
 //**************************************************************************************************
 
 std::string libCZI::XmlDateTime::ToXmlString() const
@@ -663,15 +665,14 @@
     std::wstring_convert<std::codecvt_utf8<wchar_t>> utf8_conv;
     return XmlDateTime::TryParse(utf8_conv.to_bytes(szw).c_str(), ptrDateTime);
 }
 
 /*static*/bool libCZI::XmlDateTime::TryParse(const char* sz, libCZI::XmlDateTime* ptrDateTime)
 {
     // cf. https://www.oreilly.com/library/view/regular-expressions-cookbook/9781449327453/ch04s07.html
-    //static const char* regexStr = "^(?<year>-?(?:[1-9][0-9]*)?[0-9]{4})-(?<month>1[0-2]|0[1-9])-(?<day>3[01]|0[1-9]|[12][0-9])T(?<hour>2[0-3]|[01][0-9]):(?<minute>[0-5][0-9]):(?<second>[0-5][0-9])(?<ms>\.[0-9]+)?(?<timezone>Z|[+-](?:2[0-3]|[01][0-9]):[0-5][0-9])?$";
     static const char* regexStr = R"((-?(?:[1-9][0-9]*)?[0-9]{4})-(1[0-2]|0[1-9])-(3[01]|0[1-9]|[12][0-9])T(2[0-3]|[01][0-9]):([0-5][0-9]):([0-5][0-9])(\.[0-9]+)?(Z|[+-](?:2[0-3]|[01][0-9]):[0-5][0-9])?)";
 
     auto str = Utilities::Trim(sz);
     regex dateTimeRegex(regexStr);
     smatch pieces_match;
     if (regex_match(str, pieces_match, dateTimeRegex) && pieces_match.size() == 9)
     {
@@ -763,15 +764,15 @@
 /*static*/void libCZI::MetadataUtils::WriteFillWithSubBlockStatistics(libCZI::ICziMetadataBuilder* builder, const libCZI::SubBlockStatistics& statistics)
 {
     MetadataUtils::WriteImageSizeInformation(builder, statistics.boundingBox.w, statistics.boundingBox.h);
     statistics.dimBounds.EnumValidDimensions(
         [&](libCZI::DimensionIndex dim, int start, int size)->bool
         {
             MetadataUtils::WriteDimensionSize(builder, dim, size);
-    return true;
+            return true;
         });
 
     if (statistics.IsMIndexValid())
     {
         MetadataUtils::WriteMIndexSizeInformation(builder, statistics.maxMindex - statistics.minMindex + 1);
     }
 }
@@ -944,28 +945,33 @@
         [&](int channel_index)->bool
         {
             if (channel_index > max_channel_index_in_display_settings)
             {
                 max_channel_index_in_display_settings = channel_index;
             }
 
-    return true;
+            return true;
         });
 
     MetadataUtils::WriteDisplaySettings(builder, display_settings, 1 + max_channel_index_in_display_settings);
 }
 
 static void WriteChannelDisplaySettings(const IChannelDisplaySetting* channel_display_setting, IXmlNodeRw* node)
 {
     node->GetOrCreateChildNode("IsSelected")->SetValueBool(channel_display_setting->GetIsEnabled());
 
     Rgb8Color tinting_color;
     if (channel_display_setting->TryGetTintingColorRgb8(&tinting_color))
     {
         node->GetOrCreateChildNode("Color")->SetValue(Utilities::Rgb8ColorToString(tinting_color));
+        node->GetOrCreateChildNode("ColorMode")->SetValue("Color"); // instruct to use 'tinting'
+    }
+    else
+    {
+        node->GetOrCreateChildNode("ColorMode")->SetValue("None"); // instruct to 'disable tinting'
     }
 
     float black_point, white_point;
     channel_display_setting->GetBlackWhitePoint(&black_point, &white_point);
     node->GetOrCreateChildNode("Low")->SetValueFlt(black_point);
     node->GetOrCreateChildNode("High")->SetValueFlt(white_point);
```

### Comparing `pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/CziMetadataBuilder.h` & `pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/CziMetadataBuilder.h`

 * *Files 8% similar despite different names*

```diff
@@ -69,23 +69,20 @@
     void SetValueI64(long long value) override;
     void SetValueUI64(unsigned long long value) override;
     void RemoveChildren() override;
     void RemoveAttributes() override;
     bool RemoveChild(const char* name) override;
     bool RemoveAttribute(const char* name) override;
 private:
-    std::shared_ptr<IXmlNodeRw> GetOrCreateChildNode(const char* path, bool allowCreation);
-    pugi::xml_node GetOrCreateChildElementNode(const wchar_t* sz, bool allowCreation);
-    static pugi::xml_node GetOrCreateChildElementNode(pugi::xml_node& node, const wchar_t* sz, bool allowCreation);
-
-    pugi::xml_node GetOrCreateChildElementNodeWithAttributes(const std::wstring& str, bool allowCreation);
-    static pugi::xml_node GetOrCreateChildElementNodeWithAttributes(pugi::xml_node& node, const std::wstring& str, bool allowCreation);
-
-    static pugi::xml_node GetOrCreateChildElementNodeWithAttributes(pugi::xml_node& node, const std::wstring& str, const std::map<std::wstring, std::wstring>& attribs, bool allowCreation);
-
+    pugi::xml_node GetChildNodePathMustExist(const char* path);
+    std::shared_ptr<IXmlNodeRw> GetOrCreateChildNodeInternal(const char* path);
+    pugi::xml_node GetOrCreateChildElementNode(const wchar_t* sz);
+    static pugi::xml_node GetOrCreateChildElementNode(pugi::xml_node& node, const wchar_t* sz);
+    static pugi::xml_node GetOrCreateChildElementNodeWithAttributes(pugi::xml_node& node, const std::wstring& str);
+    static pugi::xml_node GetOrCreateChildElementNodeWithAttributes(pugi::xml_node& node, const std::wstring& str, const std::map<std::wstring, std::wstring>& attribs);
     static std::map<std::wstring, std::wstring> ParseAttributes(const std::wstring& str);
 
     void ThrowIfCannotSetValue();
     pugi::xml_node GetOrCreatePcDataChild();
 
     template <typename t> void SetValueT(t v)
     {
```

### Comparing `pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/CziMetadataDocumentInfo.cpp` & `pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/CziMetadataDocumentInfo.cpp`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/CziMetadataDocumentInfo.h` & `pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/CziMetadataDocumentInfo.h`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/CziMetadataDocumentInfo2.cpp` & `pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/CziMetadataDocumentInfo2.cpp`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/CziMetadataDocumentInfo2.h` & `pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/CziMetadataDocumentInfo2.h`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/CziMetadataSegment.cpp` & `pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/CziMetadataSegment.cpp`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/CziMetadataSegment.h` & `pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/CziMetadataSegment.h`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/CziParse.cpp` & `pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/CziParse.cpp`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/CziParse.h` & `pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/CziParse.h`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/CziReaderWriter.cpp` & `pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/CziReaderWriter.cpp`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/CziReaderWriter.h` & `pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/CziReaderWriter.h`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/CziStructs.cpp` & `pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/CziStructs.cpp`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/CziStructs.h` & `pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/CziStructs.h`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/CziSubBlock.cpp` & `pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/CziSubBlock.cpp`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/CziSubBlock.h` & `pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/CziSubBlock.h`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/CziSubBlockDirectory.cpp` & `pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/CziSubBlockDirectory.cpp`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/CziSubBlockDirectory.h` & `pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/CziSubBlockDirectory.h`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/CziUtils.cpp` & `pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/CziUtils.cpp`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/CziUtils.h` & `pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/CziUtils.h`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/CziWriter.cpp` & `pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/CziWriter.cpp`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/CziWriter.h` & `pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/CziWriter.h`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/DimCoordinate.cpp` & `pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/DimCoordinate.cpp`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/Doc/CZICmd_usage.markdown` & `pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/Doc/CZICmd_usage.markdown`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/Doc/Images/CZI_1.PNG` & `pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/Doc/Images/CZI_1.PNG`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/Doc/Images/CZI_2.PNG` & `pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/Doc/Images/CZI_2.PNG`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/Doc/Images/ScalingSingleChannelTileAccessor1.png` & `pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/Doc/Images/ScalingSingleChannelTileAccessor1.png`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/Doc/Images/SingleChannelTileAccessor_1.PNG` & `pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/Doc/Images/SingleChannelTileAccessor_1.PNG`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/Doc/Images/SingleChannelTileAccessor_2.PNG` & `pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/Doc/Images/SingleChannelTileAccessor_2.PNG`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/Doc/Images/SingleChannelTileAccessor_3.PNG` & `pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/Doc/Images/SingleChannelTileAccessor_3.PNG`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/Doc/Images/SingleChannelTileAccessor_4.PNG` & `pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/Doc/Images/SingleChannelTileAccessor_4.PNG`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/Doc/Images/Tinting-LUT.png` & `pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/Doc/Images/Tinting-LUT.png`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/Doc/Images/VisualStudio_cmake1.png` & `pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/Doc/Images/VisualStudio_cmake1.png`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/Doc/Images/ZEN_screenshot_1.PNG` & `pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/Doc/Images/ZEN_screenshot_1.PNG`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/Doc/Images/ZEN_screenshot_2.PNG` & `pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/Doc/Images/ZEN_screenshot_2.PNG`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/Doc/Images/cmake_1_raspi.PNG` & `pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/Doc/Images/cmake_1_raspi.PNG`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/Doc/Images/cmake_1_raspi_help_freetype.PNG` & `pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/Doc/Images/cmake_1_raspi_help_freetype.PNG`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/Doc/Images/cmake_install_raspi1.PNG` & `pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/Doc/Images/cmake_install_raspi1.PNG`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/Doc/Images/cmake_raspi_unittests_1.PNG` & `pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/Doc/Images/cmake_raspi_unittests_1.PNG`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/Doc/Images/compositors_1.png` & `pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/Doc/Images/compositors_1.png`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/Doc/Images/compositors_2.png` & `pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/Doc/Images/compositors_2.png`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/Doc/Images/drawings/VS-project.pub` & `pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/Doc/Images/drawings/VS-project.pub`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/Doc/Images/drawings/VS-project_2.pub` & `pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/Doc/Images/drawings/VS-project_2.pub`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/Doc/Images/gradationcurve_1.PNG` & `pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/Doc/Images/gradationcurve_1.PNG`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/Doc/Images/gradationcurve_2.PNG` & `pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/Doc/Images/gradationcurve_2.PNG`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/Doc/Images/image_document_concept1.PNG` & `pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/Doc/Images/image_document_concept1.PNG`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/Doc/Images/image_document_concept2.PNG` & `pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/Doc/Images/image_document_concept2.PNG`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/Doc/Images/image_document_concept3.PNG` & `pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/Doc/Images/image_document_concept3.PNG`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/Doc/Images/image_document_concept4.PNG` & `pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/Doc/Images/image_document_concept4.PNG`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/Doc/Todos.markdown` & `pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/Doc/Todos.markdown`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/Doc/accessors.markdown` & `pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/Doc/accessors.markdown`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/Doc/building_libCZI.markdown` & `pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/Doc/building_libCZI.markdown`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/Doc/drawings.docx` & `pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/Doc/drawings.docx`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/Doc/image_document_concept.markdown` & `pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/Doc/image_document_concept.markdown`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/Doc/mainpage.markdown` & `pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/Doc/mainpage.markdown`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/Doc/multichannelcomposition.markdown` & `pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/Doc/multichannelcomposition.markdown`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/Doc/using_libCZI.markdown` & `pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/Doc/using_libCZI.markdown`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/Doc/write_czi.markdown` & `pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/Doc/write_czi.markdown`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/FileHeaderSegmentData.h` & `pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/FileHeaderSegmentData.h`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/ImportExport.h` & `pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/ImportExport.h`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/IndexSet.cpp` & `pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/IndexSet.cpp`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/IndexSet.h` & `pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/IndexSet.h`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/MD5Sum.cpp` & `pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/MD5Sum.cpp`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/MD5Sum.h` & `pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/MD5Sum.h`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/MultiChannelCompositor.cpp` & `pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/MultiChannelCompositor.cpp`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/SingleChannelAccessorBase.cpp` & `pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/SingleChannelAccessorBase.cpp`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/SingleChannelAccessorBase.h` & `pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/SingleChannelAccessorBase.h`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/SingleChannelPyramidLevelTileAccessor.cpp` & `pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/SingleChannelPyramidLevelTileAccessor.cpp`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/SingleChannelPyramidLevelTileAccessor.h` & `pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/SingleChannelPyramidLevelTileAccessor.h`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/SingleChannelScalingTileAccessor.cpp` & `pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/SingleChannelScalingTileAccessor.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -63,51 +63,77 @@
 /*static*/libCZI::IntSize CSingleChannelScalingTileAccessor::InternalCalcSize(const libCZI::IntRect& roi, float zoom)
 {
     return IntSize{ static_cast<uint32_t>(roi.w * zoom),static_cast<uint32_t>(roi.h * zoom) };
 }
 
 void CSingleChannelScalingTileAccessor::ScaleBlt(libCZI::IBitmapData* bmDest, float zoom, const libCZI::IntRect& roi, const SbInfo& sbInfo)
 {
-    // calculate the intersection of the with the subblock (logical rect) and the destination
-    const auto intersect = Utilities::Intersect(sbInfo.logicalRect, roi);
-
-    const double roiSrcTopLeftX = double(intersect.x - sbInfo.logicalRect.x) / sbInfo.logicalRect.w;
-    const double roiSrcTopLeftY = double(intersect.y - sbInfo.logicalRect.y) / sbInfo.logicalRect.h;
-    const double roiSrcBttmRightX = double(intersect.x + intersect.w - sbInfo.logicalRect.x) / sbInfo.logicalRect.w;
-    const double roiSrcBttmRightY = double(intersect.y + intersect.h - sbInfo.logicalRect.y) / sbInfo.logicalRect.h;
-
-    const double destTopLeftX = double(intersect.x - roi.x) / roi.w;
-    const double destTopLeftY = double(intersect.y - roi.y) / roi.h;
-    const double destBttmRightX = double(intersect.x + intersect.w - roi.x) / roi.w;
-    const double destBttmRightY = double(intersect.y + intersect.h - roi.y) / roi.h;
-
-    DblRect srcRoi{ roiSrcTopLeftX ,roiSrcTopLeftY,roiSrcBttmRightX - roiSrcTopLeftX ,roiSrcBttmRightY - roiSrcTopLeftY };
-    DblRect dstRoi{ destTopLeftX ,destTopLeftY,destBttmRightX - destTopLeftX ,destBttmRightY - destTopLeftY };
-
-    srcRoi.x *= sbInfo.physicalSize.w;
-    srcRoi.y *= sbInfo.physicalSize.h;
-    srcRoi.w *= sbInfo.physicalSize.w;
-    srcRoi.h *= sbInfo.physicalSize.h;
-
-    dstRoi.x *= bmDest->GetWidth();
-    dstRoi.y *= bmDest->GetHeight();
-    dstRoi.w *= bmDest->GetWidth();
-    dstRoi.h *= bmDest->GetHeight();
-
     const auto sb = this->sbBlkRepository->ReadSubBlock(sbInfo.index);
     if (GetSite()->IsEnabled(LOGLEVEL_CHATTYINFORMATION))
     {
         stringstream ss;
         ss << "   bounds: " << Utils::DimCoordinateToString(&sb->GetSubBlockInfo().coordinate);
         GetSite()->Log(LOGLEVEL_CHATTYINFORMATION, ss);
     }
 
-    const auto spBm = sb->CreateBitmap();
+    const auto source = sb->CreateBitmap();
+
+    // In order not to run into trouble with floating point precision, if the scale is exactly 1, we refrain from using the scaling operation
+    //  and do instead a simple copy operation. This should ensure a pixel-accurate result if zoom is exactly 1.
+    if (zoom == 1)
+    {
+        ScopedBitmapLockerSP srcLck{ source };
+        ScopedBitmapLockerP dstLck{ bmDest };
+        CBitmapOperations::CopyWithOffsetInfo info;
+        info.xOffset = sbInfo.logicalRect.x - roi.x;
+        info.yOffset = sbInfo.logicalRect.y - roi.y;
+        info.srcPixelType = source->GetPixelType();
+        info.srcPtr = srcLck.ptrDataRoi;
+        info.srcStride = srcLck.stride;
+        info.srcWidth = source->GetWidth();
+        info.srcHeight = source->GetHeight();
+        info.dstPixelType = bmDest->GetPixelType();
+        info.dstPtr = dstLck.ptrDataRoi;
+        info.dstStride = dstLck.stride;
+        info.dstWidth = bmDest->GetWidth();
+        info.dstHeight = bmDest->GetHeight();
+        info.drawTileBorder = false;
+
+        CBitmapOperations::CopyWithOffset(info);
+    }
+    else
+    {
+        // calculate the intersection of the subblock (logical rect) and the destination
+        const auto intersect = Utilities::Intersect(sbInfo.logicalRect, roi);
+    
+        const double roiSrcTopLeftX = double(intersect.x - sbInfo.logicalRect.x) / sbInfo.logicalRect.w;
+        const double roiSrcTopLeftY = double(intersect.y - sbInfo.logicalRect.y) / sbInfo.logicalRect.h;
+        const double roiSrcBttmRightX = double(intersect.x + intersect.w - sbInfo.logicalRect.x) / sbInfo.logicalRect.w;
+        const double roiSrcBttmRightY = double(intersect.y + intersect.h - sbInfo.logicalRect.y) / sbInfo.logicalRect.h;
+
+        const double destTopLeftX = double(intersect.x - roi.x) / roi.w;
+        const double destTopLeftY = double(intersect.y - roi.y) / roi.h;
+        const double destBttmRightX = double(intersect.x + intersect.w - roi.x) / roi.w;
+        const double destBttmRightY = double(intersect.y + intersect.h - roi.y) / roi.h;
+
+        DblRect srcRoi{ roiSrcTopLeftX ,roiSrcTopLeftY,roiSrcBttmRightX - roiSrcTopLeftX ,roiSrcBttmRightY - roiSrcTopLeftY };
+        DblRect dstRoi{ destTopLeftX ,destTopLeftY,destBttmRightX - destTopLeftX ,destBttmRightY - destTopLeftY };
+
+        srcRoi.x *= sbInfo.physicalSize.w;
+        srcRoi.y *= sbInfo.physicalSize.h;
+        srcRoi.w *= sbInfo.physicalSize.w;
+        srcRoi.h *= sbInfo.physicalSize.h;
+
+        dstRoi.x *= bmDest->GetWidth();
+        dstRoi.y *= bmDest->GetHeight();
+        dstRoi.w *= bmDest->GetWidth();
+        dstRoi.h *= bmDest->GetHeight();
 
-    CBitmapOperations::NNResize(spBm.get(), bmDest, srcRoi, dstRoi);
+        CBitmapOperations::NNResize(source.get(), bmDest, srcRoi, dstRoi);
+    }
 }
 
 int CSingleChannelScalingTileAccessor::GetIdxOf1stSubBlockWithZoomGreater(const std::vector<SbInfo>& sbBlks, const std::vector<int>& byZoom, float zoom)
 {
     // now, skip until the zoom of the subBlock is greater than the specified zoom
     for (size_t i = 0; i < byZoom.size(); ++i)
     {
@@ -191,21 +217,21 @@
                         // if there is a set of "allowedScenes" given, and the subblock has a valid S-index, and it is not found in the
                         //  set of allowed scenes, then we need to discard this subblock (need to return true in order to continue the enumeration)
                         return true;
                     }
                 }
             }
 
-    SbInfo sbinfo;
-    sbinfo.logicalRect = info.logicalRect;
-    sbinfo.physicalSize = info.physicalSize;
-    sbinfo.mIndex = info.mIndex;
-    sbinfo.index = idx;
-    sblks.push_back(sbinfo);
-    return true;
+            SbInfo sbinfo;
+            sbinfo.logicalRect = info.logicalRect;
+            sbinfo.physicalSize = info.physicalSize;
+            sbinfo.mIndex = info.mIndex;
+            sbinfo.index = idx;
+            sblks.push_back(sbinfo);
+            return true;
         });
 
     return sblks;
 }
 
 void CSingleChannelScalingTileAccessor::InternalGet(libCZI::IBitmapData* bmDest, const libCZI::IntRect& roi, const libCZI::IDimCoordinate* planeCoordinate, float zoom, const libCZI::ISingleChannelScalingTileAccessor::Options& options)
 {
@@ -258,27 +284,27 @@
             this->Paint(bmDest, roi, get<1>(it), zoom);
         }
     }
 }
 
 void CSingleChannelScalingTileAccessor::Paint(libCZI::IBitmapData* bmDest, const libCZI::IntRect& roi, const SubSetSortedByZoom& sbSetSortedByZoom, float zoom)
 {
-    const int idxOf1stSSubBlockOfZoomGreater = this->GetIdxOf1stSubBlockWithZoomGreater(sbSetSortedByZoom.subBlocks, sbSetSortedByZoom.sortedByZoom, zoom);
-    if (idxOf1stSSubBlockOfZoomGreater < 0)
+    const int idxOf1stSubBlockOfZoomGreater = this->GetIdxOf1stSubBlockWithZoomGreater(sbSetSortedByZoom.subBlocks, sbSetSortedByZoom.sortedByZoom, zoom);
+    if (idxOf1stSubBlockOfZoomGreater < 0)
     {
         // this means that we would need to overzoom (i.e. the requested zoom is less than the lowest level we find in the subblock-repository)
         // TODO: this requires special consideration, for the time being -> bail out
         // ...we end up here e. g. when lowest level does not cover all the range, so - this is not
         //    something where we want to throw an excpetion
         //throw LibCZIAccessorException("Overzoom not supported", LibCZIAccessorException::ErrorType::Unspecified);
         return;
     }
 
     std::vector<int>::const_iterator it = sbSetSortedByZoom.sortedByZoom.cbegin();
-    std::advance(it, idxOf1stSSubBlockOfZoomGreater);
+    std::advance(it, idxOf1stSubBlockOfZoomGreater);
 
     const float startZoom = sbSetSortedByZoom.subBlocks.at(*it).GetZoom();
 
     for (; it != sbSetSortedByZoom.sortedByZoom.cend(); ++it)
     {
         const SbInfo& sbInfo = sbSetSortedByZoom.subBlocks.at(*it);
```

### Comparing `pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/SingleChannelScalingTileAccessor.h` & `pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/SingleChannelScalingTileAccessor.h`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/SingleChannelTileAccessor.cpp` & `pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/SingleChannelTileAccessor.cpp`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/SingleChannelTileAccessor.h` & `pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/SingleChannelTileAccessor.h`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/SingleChannelTileCompositor.cpp` & `pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/SingleChannelTileCompositor.cpp`

 * *Files 6% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 using namespace libCZI;
 
 /*static*/void CSingleChannelTileCompositor::Compose(libCZI::IBitmapData* dest, libCZI::IBitmapData* source, int x, int y, bool drawTileBorder)
 {
     ScopedBitmapLockerP srcLck{ source };
     ScopedBitmapLockerP dstLck{ dest };
-    CBitmapOperations::CopyOffsetedInfo info;
+    CBitmapOperations::CopyWithOffsetInfo info;
     info.xOffset = x;
     info.yOffset = y;
     info.srcPixelType = source->GetPixelType();
     info.srcPtr = srcLck.ptrDataRoi;
     info.srcStride = srcLck.stride;
     info.srcWidth = source->GetWidth();
     info.srcHeight = source->GetHeight();
@@ -26,15 +26,15 @@
     info.dstPtr = dstLck.ptrDataRoi;
     info.dstStride = dstLck.stride;
     info.dstWidth = dest->GetWidth();
     info.dstHeight = dest->GetHeight();
 
     info.drawTileBorder = drawTileBorder;
 
-    CBitmapOperations::CopyOffseted(info);
+    CBitmapOperations::CopyWithOffset(info);
 }
 
 /*-----------------------------------------------------------------------------------------------*/
 
 /*static*/void libCZI::Compositors::ComposeSingleChannelTiles(
     std::function<bool(int, std::shared_ptr<libCZI::IBitmapData>&, int&, int&)> getTiles,
     libCZI::IBitmapData* dest,
```

### Comparing `pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/StreamImpl.cpp` & `pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/StreamImpl.cpp`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/StreamImpl.h` & `pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/StreamImpl.h`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/XmlNodeWrapper.h` & `pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/XmlNodeWrapper.h`

 * *Files 16% similar despite different names*

```diff
@@ -12,178 +12,115 @@
 #include "libCZI_Metadata.h"
 #include <regex>
 #include <exception>
 #include "utilities.h"
 #include "pugixml.hpp"
 #include "libCZI_exceptions.h"
 
-/// This implements a wrapper around a pugi-node struct (implementing the IXmlNodeRead-interface). It is initialized
-/// with a raw pointer (to the pugi-xml-node-structure), and we rely on that pointer being valid for the lifetime
-/// of this object. In order to achieve this, we take another shared_ptr and keep a reference to it, and this
-/// object is assumed to be the (sole) owner of the pugi-xml-document.
-/// We provide two constructors, where one takes the mentioned shared_ptr and the other doesn't. If using the one without
-/// the shared_ptr, then it must be ensured that the lifetime of this object is the same as the underlying pugi-xml-document
-/// (e.g. if this class is a member of the class owning the pugi-xml-document, in which case we would create a circular
-/// reference). In that case, you need to use only the "GetChildNodeReadonly"-overload which takes an additional shared_ptr
-/// (which is to be owner of the pugi-xml-document).
-/// \tparam t Generic type parameter (of the object owning the pugi-xml-document).
-template<typename t, typename tExcp>
-class XmlNodeWrapperReadonly : public libCZI::IXmlNodeRead
+/// A utility for parsing an "XML path specifier" (as used with IXmlNodeRead).
+///
+/// \tparam tExcp   Generic type used for throwing the appropriate exception in case of an error while parsing.
+template<typename tExcp>
+class XmlPathSpecifierUtilities
 {
-private:
-    pugi::xml_node node;
-    std::shared_ptr<t> parentRef;
 public:
-    XmlNodeWrapperReadonly(std::shared_ptr<t> parentRef, pugi::xml_node_struct* node_struct) :node(node_struct), parentRef(std::move(parentRef)) {}
-    explicit XmlNodeWrapperReadonly(pugi::xml_node_struct* node_struct) :node(node_struct) {}
-public: // interface IXmlNodeRead
-    std::wstring Name() const override
-    {
-        return this->node.name();
-    }
 
-    bool TryGetAttribute(const wchar_t* attributeName, std::wstring* attribValue) const override
+    /// Gets the child element node specified by the given path. This method supports node specifiers in the form of
+    /// "list of attributes" (e.g. "[Id=abc][Name=def]") and "index" (e.g. "[2]").
+    /// \param [in]     node    The node where the path is to be evaluated for.
+    /// \param          str     The path.
+    ///
+    /// \returns    The child element identified by the path.
+    static pugi::xml_node GetChildElementNodeWithAttributes(pugi::xml_node& node, const std::wstring& str)
     {
-        auto attrib = this->node.find_attribute([&](const pugi::xml_attribute& a)
-            {
-                return wcscmp(a.name(), attributeName) == 0;
-            });
-
-        if (!attrib)
-        {
-            return false;
-        }
+        // this matches one or more characters that are not square brackets, followed by an optional group that starts with a '[', 
+        // followed by zero or more of any characters that are not square brackets, and ends with a ']'
+        std::wregex node_name_with_attributes_regex(LR"(([^\[\]]+)(\[([^\[\]]*)\])?)");
+        std::wsmatch pieces_match;
 
-        if (attribValue != nullptr)
+        if (std::regex_match(str, pieces_match, node_name_with_attributes_regex))
         {
-            *attribValue = attrib.value();
+            if (pieces_match.size() == 4)
+            {
+                if (pieces_match[0].matched == true && pieces_match[1].matched == true)
+                {
+                    const std::wstring nodeName = pieces_match[1];
+                    if (pieces_match[2].matched == false && pieces_match[3].matched == false)
+                    {
+                        // we only got a name ( not followed by [Id=abc] )
+                        return GetChildElementNode(node, nodeName.c_str());
+                    }
+                    else if (pieces_match[2].matched == true && pieces_match[3].matched == true)
+                    {
+                        return GetChildElementWithSpecifier(node, nodeName, pieces_match[3]);
+                    }
+                }
+            }
         }
 
-        return true;
+        tExcp::ThrowInvalidPath();
+        throw std::logic_error("Must not get here.");
     }
-
-    void EnumAttributes(const std::function<bool(const std::wstring& attribName, const std::wstring& attribValue)>& enumFunc) const override
+private:
+    static pugi::xml_node GetChildElementWithSpecifier(pugi::xml_node& node, const std::wstring& nodeName, const std::wstring& specifier)
     {
-        for (pugi::xml_attribute_iterator ait = this->node.attributes_begin(); ait != this->node.attributes_end(); ++ait)
-        {
-            if (!enumFunc(std::wstring(ait->name()), std::wstring(ait->value())))
+        // if the specifier contains only digits, then it is an index - otherwise it is (or has to be) a list of key-value pairs giving attributes
+        const std::wregex regex_contains_only_a_number(L"^\\s*\\d+\\s*$");
+        if (std::regex_match(specifier, regex_contains_only_a_number))
+        {
+            // we then expect the specifier to be a number
+            unsigned long num = 0;
+            try
             {
-                break;
+                num = std::stoul(specifier);
             }
-        }
-    }
-
-    bool TryGetValue(std::wstring* value) const override
-    {
-        if (this->node.first_child().type() == pugi::xml_node_type::node_pcdata)
-        {
-            if (value != nullptr)
+            catch (const std::exception&)
             {
-                *value = this->node.child_value();
+                tExcp::ThrowInvalidPath();
             }
 
-            return true;
-        }
-
-        return false;
-    }
+            if (num > (std::numeric_limits<std::uint32_t>::max)())
+            {
+                tExcp::ThrowInvalidPath();
+            }
 
-    std::shared_ptr<IXmlNodeRead> GetChildNodeReadonly(const char* path) override
-    {
-        if (!this->parentRef)
-        {
-            // we must never get here
-            throw std::logic_error("there is no valid object which is the owner of the xml-dom");
+            return GetChildElementNodeWithIndex(node, nodeName, static_cast<std::uint32_t>(num));
         }
-
-        return this->GetChildNodeReadonly(path, this->parentRef);
-    }
-
-    void EnumChildren(const std::function<bool(std::shared_ptr<IXmlNodeRead>)>& enumChildren) override
-    {
-        if (!this->parentRef)
+        else
         {
-            // we must never get here
-            throw std::logic_error("there is no valid object which is the owner of the xml-dom");
+            const auto attribute_value_pairs = ParseAttributes(specifier);
+            return GetChildElementNodeWithAttributes(node, nodeName, attribute_value_pairs);
         }
-
-        return this->EnumChildren(enumChildren, this->parentRef);
     }
 
-    std::shared_ptr<IXmlNodeRead> GetChildNodeReadonly(const char* path, std::shared_ptr<t> parentRef)
+    /// Gets the n-th child node with name 'node_name' from the specified node. The index is zero-based.
+    /// If this node does not exist, an exception is thrown.
+    /// \param [in]     node        The node (to get the n-th child node).
+    /// \param          node_name   Name of the child node to search for.
+    /// \param          index       Zero-based index of the child node (with the specified name) to search for.
+    /// \returns    The child node with the specified index.
+    static pugi::xml_node GetChildElementNodeWithIndex(pugi::xml_node& node, const std::wstring& node_name, std::uint32_t index)
     {
-        const auto p = Utilities::convertUtf8ToWchar_t(path);
-        std::vector<std::wstring> tokens;
-        Utilities::Tokenize(p, tokens, L"/");
-        if (tokens.empty())
+        auto child_node = node.child(node_name.c_str());
+        if (!child_node)
         {
             tExcp::ThrowInvalidPath();
         }
 
-        if (any_of(tokens.cbegin(), tokens.cend(), [](const std::wstring& str) {return str.empty(); }))
-        {
-            tExcp::ThrowInvalidPath();
-        }
-
-        auto node = GetChildElementNodeWithAttributes(this->node, tokens[0]);
-        if (!node)
-        {
-            return nullptr;
-        }
-
-        for (size_t i = 1; i < tokens.size(); ++i)
-        {
-            node = GetChildElementNodeWithAttributes(node, tokens[i].c_str());
-            if (!node)
-            {
-                return nullptr;
-            }
-        }
-
-        return std::make_shared<XmlNodeWrapperReadonly>(parentRef, node.internal_object());
-    }
-
-    void EnumChildren(std::function<bool(std::shared_ptr<IXmlNodeRead>)> enumChildren, std::shared_ptr<t> parentRef)
-    {
-        for (pugi::xml_node childNode = this->node.first_child(); childNode; childNode = childNode.next_sibling())
+        for (std::uint32_t i = 0; i <= index; ++i)
         {
-            if (childNode.type() == pugi::xml_node_type::node_element)
+            if (i == index)
             {
-                const bool b = enumChildren(std::make_shared<XmlNodeWrapperReadonly>(parentRef, childNode.internal_object()));
-                if (!b)
-                {
-                    break;
-                }
+                return child_node;
             }
-        }
-    }
-private:
-    static pugi::xml_node GetChildElementNodeWithAttributes(pugi::xml_node& node, const std::wstring& str)
-    {
-        std::wregex nodenameWihtAttribregex(LR"(([^\[\]]+)(\[([^\[\]]*)\])?)");
-        std::wsmatch pieces_match;
 
-        if (std::regex_match(str, pieces_match, nodenameWihtAttribregex))
-        {
-            if (pieces_match.size() == 4)
+            child_node = child_node.next_sibling(node_name.c_str());
+            if (!child_node)
             {
-                if (pieces_match[0].matched == true && pieces_match[1].matched == true)
-                {
-                    const std::wstring nodeName = pieces_match[1];
-                    if (pieces_match[2].matched == false && pieces_match[3].matched == false)
-                    {
-                        // we only got a name ( not followed by [Id=abc] )
-                        return GetChildElementNode(node, nodeName.c_str());
-                    }
-                    else if (pieces_match[2].matched == true && pieces_match[3].matched == true)
-                    {
-                        const auto attribValuePairs = ParseAttributes(pieces_match[3]);
-                        return GetChildElementNodeWithAttributes(node, nodeName, attribValuePairs);
-                    }
-                }
+                tExcp::ThrowInvalidPath();
             }
         }
 
         tExcp::ThrowInvalidPath();
         throw std::logic_error("Must not get here.");
     }
 
@@ -227,15 +164,15 @@
                 return true;
             }
         };
 
         auto c = node.find_child(find_element_node_and_attributes{ str.c_str(), attribs });
         if (!c)
         {
-            return pugi::xml_node();
+            return {};
         }
 
         return c;
     }
 
     static pugi::xml_node GetChildElementNode(pugi::xml_node& node, const wchar_t* sz)
     {
@@ -253,20 +190,23 @@
                 return wcscmp(node.name(), this->nodeName) == 0;
             }
         };
 
         auto c = node.find_child(find_element_node{ sz });
         if (!c)
         {
-            return pugi::xml_node();
+            return {};
         }
 
         return c;
     }
 
+    /// Parse an "attributes definition string" of the form "Id=abc,Name=abc" into a map of name/value pairs.
+    /// \param  str The string to be parsed.
+    /// \returns    A std::map&lt;std::wstring,std::wstring&gt; containing the key-value pairs.
     static std::map<std::wstring, std::wstring> ParseAttributes(const std::wstring& str)
     {
         std::map<std::wstring, std::wstring> attribMap;
 
         std::wsmatch pieces_match;
 
         // now we have string of the form Id=abc,Name=abc
@@ -291,7 +231,150 @@
                 tExcp::ThrowInvalidPath();
             }
         }
 
         return attribMap;
     }
 };
+
+/// This implements a wrapper around a pugi-node struct (implementing the IXmlNodeRead-interface). It is initialized
+/// with a raw pointer (to the pugi-xml-node-structure), and we rely on that pointer being valid for the lifetime
+/// of this object. In order to achieve this, we take another shared_ptr and keep a reference to it, and this
+/// object is assumed to be the (sole) owner of the pugi-xml-document.
+/// We provide two constructors, where one takes the mentioned shared_ptr and the other doesn't. If using the one without
+/// the shared_ptr, then it must be ensured that the lifetime of this object is the same as the underlying pugi-xml-document
+/// (e.g. if this class is a member of the class owning the pugi-xml-document, in which case we would create a circular
+/// reference). In that case, you need to use only the "GetChildNodeReadonly"-overload which takes an additional shared_ptr
+/// (which is to be owner of the pugi-xml-document).
+/// \tparam t Generic type parameter (of the object owning the pugi-xml-document).
+template<typename t, typename tExcp>
+class XmlNodeWrapperReadonly : public libCZI::IXmlNodeRead
+{
+private:
+    pugi::xml_node node;
+    std::shared_ptr<t> parentRef;
+public:
+    XmlNodeWrapperReadonly(std::shared_ptr<t> parentRef, pugi::xml_node_struct* node_struct) :node(node_struct), parentRef(std::move(parentRef)) {}
+    explicit XmlNodeWrapperReadonly(pugi::xml_node_struct* node_struct) :node(node_struct) {}
+public: // interface IXmlNodeRead
+    std::wstring Name() const override
+    {
+        return this->node.name();
+    }
+
+    bool TryGetAttribute(const wchar_t* attributeName, std::wstring* attribValue) const override
+    {
+        auto attrib = this->node.find_attribute([&](const pugi::xml_attribute& a)
+            {
+                return wcscmp(a.name(), attributeName) == 0;
+            });
+
+        if (!attrib)
+        {
+            return false;
+        }
+
+        if (attribValue != nullptr)
+        {
+            *attribValue = attrib.value();
+        }
+
+        return true;
+    }
+
+    void EnumAttributes(const std::function<bool(const std::wstring& attribName, const std::wstring& attribValue)>& enumFunc) const override
+    {
+        for (pugi::xml_attribute_iterator ait = this->node.attributes_begin(); ait != this->node.attributes_end(); ++ait)
+        {
+            if (!enumFunc(std::wstring(ait->name()), std::wstring(ait->value())))
+            {
+                break;
+            }
+        }
+    }
+
+    bool TryGetValue(std::wstring* value) const override
+    {
+        if (this->node.first_child().type() == pugi::xml_node_type::node_pcdata)
+        {
+            if (value != nullptr)
+            {
+                *value = this->node.child_value();
+            }
+
+            return true;
+        }
+
+        return false;
+    }
+
+    std::shared_ptr<IXmlNodeRead> GetChildNodeReadonly(const char* path) override
+    {
+        if (!this->parentRef)
+        {
+            // we must never get here
+            throw std::logic_error("there is no valid object which is the owner of the xml-dom");
+        }
+
+        return this->GetChildNodeReadonly(path, this->parentRef);
+    }
+
+    void EnumChildren(const std::function<bool(std::shared_ptr<IXmlNodeRead>)>& enumChildren) override
+    {
+        if (!this->parentRef)
+        {
+            // we must never get here
+            throw std::logic_error("there is no valid object which is the owner of the xml-dom");
+        }
+
+        return this->EnumChildren(enumChildren, this->parentRef);
+    }
+
+    std::shared_ptr<IXmlNodeRead> GetChildNodeReadonly(const char* path, std::shared_ptr<t> parentRef)
+    {
+        const auto p = Utilities::convertUtf8ToWchar_t(path);
+        std::vector<std::wstring> tokens;
+        Utilities::Tokenize(p, tokens, L"/");
+        if (tokens.empty())
+        {
+            tExcp::ThrowInvalidPath();
+        }
+
+        // if any of the tokens is empty, then we have a path like "/a//b", which is invalid
+        if (any_of(tokens.cbegin(), tokens.cend(), [](const std::wstring& str) {return str.empty(); }))
+        {
+            tExcp::ThrowInvalidPath();
+        }
+
+        auto node = XmlPathSpecifierUtilities<tExcp>::GetChildElementNodeWithAttributes(this->node, tokens[0]);
+        if (!node)
+        {
+            return nullptr;
+        }
+
+        for (size_t i = 1; i < tokens.size(); ++i)
+        {
+            node = XmlPathSpecifierUtilities<tExcp>::GetChildElementNodeWithAttributes(node, tokens[i]);
+            if (!node)
+            {
+                return nullptr;
+            }
+        }
+
+        return std::make_shared<XmlNodeWrapperReadonly>(parentRef, node.internal_object());
+    }
+
+    void EnumChildren(const std::function<bool(std::shared_ptr<IXmlNodeRead>)>& enumChildren, std::shared_ptr<t> parentRef)
+    {
+        for (pugi::xml_node childNode = this->node.first_child(); childNode; childNode = childNode.next_sibling())
+        {
+            if (childNode.type() == pugi::xml_node_type::node_element)
+            {
+                const bool b = enumChildren(std::make_shared<XmlNodeWrapperReadonly>(parentRef, childNode.internal_object()));
+                if (!b)
+                {
+                    break;
+                }
+            }
+        }
+    }
+};
```

### Comparing `pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/bitmapData.h` & `pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/bitmapData.h`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/decoder.cpp` & `pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/decoder.cpp`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/decoder.h` & `pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/decoder.h`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/decoder_wic.cpp` & `pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/decoder_wic.cpp`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/decoder_wic.h` & `pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/decoder_wic.h`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/decoder_zstd.cpp` & `pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/decoder_zstd.cpp`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/decoder_zstd.h` & `pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/decoder_zstd.h`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/libCZI.h` & `pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/libCZI.h`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/libCZI_Compositor.h` & `pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/libCZI_Compositor.h`

 * *Files 0% similar despite different names*

```diff
@@ -187,15 +187,15 @@
         struct PyramidLayerInfo
         {
             std::uint8_t minificationFactor;    ///< Factor by which adjacent pyramid-layers are shrunk. Commonly used in CZI are 2 or 3.
             std::uint8_t pyramidLayerNo;        ///< The pyramid layer number.
         };
 
         /// Gets the tile composite of the specified plane and the specified ROI and the specified pyramid-layer.
-        /// The pixeltype is determined by examing the first subblock found in the
+        /// The pixeltype is determined by examining the first subblock found in the
         /// specified plane (which is an arbitrary subblock). A newly allocated
         /// bitmap is returned.
         /// \param roi             The ROI.
         /// \param planeCoordinate The plane coordinate.
         /// \param pyramidInfo     Information describing the pyramid-layer.
         /// \param pOptions        Options for controlling the operation.
         /// \return A std::shared_ptr&lt;libCZI::IBitmapData&gt;
@@ -263,26 +263,26 @@
         /// Since the exact size if subject to rounding errors, one should always use this method if the exact size must be known beforehand.
         /// The Get-method which operates on a pre-allocated bitmap will only work if the size (of the bitmap passed in) exactly matches.
         /// \param roi  The ROI.
         /// \param zoom The zoom factor.
         /// \return The size of the composite created by this accessor (for these parameters).
         virtual libCZI::IntSize CalcSize(const libCZI::IntRect& roi, float zoom) const = 0;
 
-        /// Gets the scaled tile composite of the specified plane and the specified ROI with the specifed zoom factor.\n
-        /// The pixeltype is determined by examing the first subblock found in the
+        /// Gets the scaled tile composite of the specified plane and the specified ROI with the specified zoom factor.\n
+        /// The pixeltype is determined by examining the first subblock found in the
         /// specified plane (which is an arbitrary subblock). A newly allocated
         /// bitmap is returned.
         /// \param roi             The ROI.
         /// \param planeCoordinate The plane coordinate.
         /// \param zoom            The zoom.
         /// \param pOptions        Options for controlling the operation (may be nullptr).
         /// \return A std::shared_ptr&lt;libCZI::IBitmapData&gt;
         virtual std::shared_ptr<libCZI::IBitmapData> Get(const libCZI::IntRect& roi, const libCZI::IDimCoordinate* planeCoordinate, float zoom, const libCZI::ISingleChannelScalingTileAccessor::Options* pOptions) = 0;
 
-        /// Gets the scaled tile composite of the specified plane and the specified ROI with the specifed zoom factor.
+        /// Gets the scaled tile composite of the specified plane and the specified ROI with the specified zoom factor.
         /// \param pixeltype       The pixeltype (of the destination bitmap).
         /// \param roi             The ROI.
         /// \param planeCoordinate The plane coordinate.
         /// \param zoom            The zoom factor.
         /// \param pOptions        Options for controlling the operation (may be nullptr).
         /// \return A std::shared_ptr&lt;libCZI::IBitmapData&gt;
         virtual std::shared_ptr<libCZI::IBitmapData> Get(libCZI::PixelType pixeltype, const libCZI::IntRect& roi, const libCZI::IDimCoordinate* planeCoordinate, float zoom, const libCZI::ISingleChannelScalingTileAccessor::Options* pOptions) = 0;
```

### Comparing `pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/libCZI_Config.h.in` & `pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/libCZI_Config.h.in`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/libCZI_DimCoordinate.h` & `pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/libCZI_DimCoordinate.h`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/libCZI_Helpers.h` & `pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/libCZI_Helpers.h`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/libCZI_Lib.cpp` & `pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/libCZI_Lib.cpp`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/libCZI_Metadata.h` & `pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/libCZI_Metadata.h`

 * *Files 1% similar despite different names*

```diff
@@ -579,15 +579,15 @@
         virtual IDisplaySettings::GradationCurveMode GetGradationCurveMode() const = 0;
 
         /// Attempts to get the gamma - this will only be available if gradation curve mode is <tt>Gamma</tt>.
         ///
         /// \param [out] gamma If non-null and applicable, the gamma will be returned.
         ///
         /// \return True if the corresponding channel uses gradation curve mode <tt>Gamma</tt> (and a value for gamma is available), false otherwise.
-        virtual bool    TryGetGamma(float* gamma)const = 0;
+        virtual bool    TryGetGamma(float* gamma) const = 0;
 
         /// Attempts to get spline control points - this will only be available if gradation curve mode is <tt>Spline</tt>.
         /// \remark
         /// We make no promises that both the control-points and the spline-data are always available. It might be plausible that
         /// the spline is defined in a different way (different than control-points), so in that case only the "spline-data" would
         /// be available. So - be careful is using this interface in a context different thant "CZI-metadata" where it might be
         /// the case the 'TryGetSplineControlPoints' will fail but 'TryGetSplineData' might succeed.
@@ -739,15 +739,15 @@
 
         /// Gets the display settings.
         /// \remark
         /// This method may return an empty shared_ptr in case that display-settings are not present in the metadata.
         /// \return The display settings object.
         virtual std::shared_ptr<IDisplaySettings> GetDisplaySettings() const = 0;
 
-        virtual ~ICziMultiDimensionDocumentInfo() {}
+        virtual ~ICziMultiDimensionDocumentInfo() = default;
 
         /// Gets a vector with all dimensions (found in metadata).
         /// \return The vector containing all dimensions.
         std::vector<DimensionIndex> GetDimensions()
         {
             std::vector<DimensionIndex> vec;
             this->EnumDimensions([&](DimensionIndex i)->bool {vec.push_back(i); return true; });
@@ -783,15 +783,15 @@
         ///
         /// \return True if it succeeds, false if it fails.
         virtual bool TryGetValue(std::wstring* value) const = 0;
 
         /// Gets a child node for the specified path/attribute specification if it
         /// exists. Otherwise, a nullptr is returned. 
         /// The path is specified as node-names separated by slashes.
-        /// At path "A/B/C" selects (or creates) a node-structure like this
+        /// A path "A/B/C" selects a node-structure like this
         /// \code{.unparsed}
         /// <A>
         ///   <B>
         ///     <C/>
         ///   </B>
         /// </A>
         /// \endcode
@@ -801,14 +801,27 @@
         /// \code{.unparsed}
         /// <A>
         ///   <B Id="ab" Name="xy">
         ///     <C/>
         ///   </B>
         /// </A>
         /// \endcode
+        /// It is also possible to specify a number inside the square brackets, which indicates that the
+        /// n-th element is to be selected. This index is zero-based.
+        /// In this example     
+        /// \code{.unparsed}
+        /// <A>
+        ///   <B Id="ab" Name="xy">
+        ///     <C Id="first"></C>
+        ///     <C Id="second"></C>
+        ///     <C Id="third"></C>
+        ///   </B>
+        /// </A>
+        /// \endcode
+        /// the path "A/B/C[1]" will select the second node of name 'C'.        
         /// \param path The path  (in UTF8-encoding).
         /// \return Either the requested node if it exists or nullptr.
         virtual std::shared_ptr<IXmlNodeRead> GetChildNodeReadonly(const char* path) = 0;
 
         /// Enumerate the children of the node. The functor will be called until there are no
         /// more children or if the function return false.
         /// \param enumChildren The function to be called with the children nodes.
@@ -846,15 +859,15 @@
 
         /// Attempts to get value of this node as an unsigned long integer (64-bit). Valid values for true are: "true", "yes" or "1";
         /// valid values for false are "false", "no" or "0" (case insensitive comparison).
         /// \param [in,out] p If non-null, a pointer to a bool to store the result in.
         /// \returns True if it succeeds, false if it fails.
         bool TryGetValueAsBool(bool* p);
 
-        virtual ~IXmlNodeRead() {}
+        virtual ~IXmlNodeRead() = default;
     };
 
     /// Representation of the CZI-metadata.
     class LIBCZI_API ICziMetadata : public IXmlNodeRead
     {
     public:
         /// Query if the CZI's metadata (the XML) is well-formed and parsed correctly.
@@ -870,25 +883,25 @@
         virtual std::string GetXml() = 0;
 
         /// Gets the "document information" part of the metadata.
         ///
         /// \return The "document information".
         virtual std::shared_ptr<libCZI::ICziMultiDimensionDocumentInfo> GetDocumentInfo() = 0;
 
-        virtual ~ICziMetadata() {}
+        virtual ~ICziMetadata() = default;
     };
 
     class IXmlNodeRw;
 
     /// This interface provides write access to an XML-node.
     class LIBCZI_API IXmlNodeWrite
     {
     public:
         /// Gets or create a child node. The path is specified as node-names separated by slashes.
-        /// At path "A/B/C" selects (or creates) a node-structure like this
+        /// A path "A/B/C" selects (or creates) a node-structure like this
         /// \code{.unparsed}
         /// <A>
         ///   <B>
         ///     <C/>
         ///   </B>
         /// </A>
         /// \endcode
@@ -903,15 +916,15 @@
         /// </A>
         /// \endcode
         /// \param path The path  (in UTF8-encoding).
         /// \return Either an existing node or a newly created one.
         virtual std::shared_ptr<IXmlNodeRw> GetOrCreateChildNode(const char* path) = 0;
 
         /// Gets an existing child node. The path is specified as node-names separated by slashes.
-        /// At path "A/B/C" selects (or creates) a node-structure like this
+        /// A path "A/B/C" selects (or creates) a node-structure like this
         /// \code{.unparsed}
         /// <A>
         ///   <B>
         ///     <C/>
         ///   </B>
         /// </A>
         /// \endcode
@@ -921,14 +934,27 @@
         /// \code{.unparsed}
         /// <A>
         ///   <B Id="ab" Name="xy">
         ///     <C/>
         ///   </B>
         /// </A>
         /// \endcode
+        /// It is also possible to specify a number inside the square brackets, which indicates that the
+        /// n-th element is to be selected. This index is zero-based.
+        /// In this example
+        /// \code{.unparsed}
+        /// <A>
+        ///   <B Id="ab" Name="xy">
+        ///     <C Id="first"></C>
+        ///     <C Id="second"></C>
+        ///     <C Id="third"></C>
+        ///   </B>
+        /// </A>
+        /// \endcode
+        /// the path "A/B/C[1]" will select the second node of name 'C'.
         /// \param path The path (in UTF8-encoding).
         /// \return The existing node conforming to the path if it exists, null otherwise.
         virtual std::shared_ptr<IXmlNodeRw> GetChildNode(const char* path) = 0;
 
         /// Appends a child node with the specified name.
         ///
         /// \param name The name of the node to add.
@@ -1061,15 +1087,15 @@
         virtual std::shared_ptr<IXmlNodeRw> GetRootNode() = 0;
 
         /// Gets the metadata as an UTF8-encoded XML-string.
         ///
         /// \return The metadata (UTF8-encoded XML).
         virtual std::string GetXml(bool withIndent = false) = 0;
 
-        virtual ~ICziMetadataBuilder() {}
+        virtual ~ICziMetadataBuilder() = default;
     };
 
     /// Variant for CustomValue.
     struct LIBCZI_API CustomValueVariant
     {
     public:
         /// Values that represent the type represented by this variant.
```

### Comparing `pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/libCZI_Metadata2.h` & `pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/libCZI_Metadata2.h`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/libCZI_Pixels.h` & `pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/libCZI_Pixels.h`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/libCZI_ReadWrite.h` & `pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/libCZI_ReadWrite.h`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/libCZI_Site.cpp` & `pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/libCZI_Site.cpp`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/libCZI_Site.h` & `pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/libCZI_Site.h`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/libCZI_Utilities.cpp` & `pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/libCZI_Utilities.cpp`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/libCZI_Utilities.h` & `pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/libCZI_Utilities.h`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/libCZI_Write.h` & `pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/libCZI_Write.h`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/libCZI_compress.h` & `pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/libCZI_compress.h`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/libCZI_exceptions.h` & `pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/libCZI_exceptions.h`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/priv_guiddef.h` & `pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/priv_guiddef.h`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/pugiconfig.hpp` & `pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/pugiconfig.hpp`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/pugixml.cpp` & `pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/pugixml.cpp`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/pugixml.hpp` & `pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/pugixml.hpp`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/splines.cpp` & `pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/splines.cpp`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/splines.h` & `pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/splines.h`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/stdAllocator.cpp` & `pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/stdAllocator.cpp`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/stdAllocator.h` & `pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/stdAllocator.h`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/stdafx.h` & `pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/stdafx.h`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/utilities.cpp` & `pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/utilities.cpp`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/utilities.h` & `pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/utilities.h`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/utilities_simd.cpp` & `pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/utilities_simd.cpp`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/libCZIrw/Src/libCZI/zstdCompress.cpp` & `pylibCZIrw-3.4.1/libs/libCZIrw/Src/libCZI/zstdCompress.cpp`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/libCZIrw/THIRD_PARTY_LICENSES.txt` & `pylibCZIrw-3.4.1/libs/libCZIrw/THIRD_PARTY_LICENSES.txt`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/libCZIrw/cla_corporate.txt` & `pylibCZIrw-3.4.1/libs/libCZIrw/cla_corporate.txt`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/libCZIrw/cla_individual.txt` & `pylibCZIrw-3.4.1/libs/libCZIrw/cla_individual.txt`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/libCZIrw/cmake/ExternalEIGEN3.cmake` & `pylibCZIrw-3.4.1/libs/libCZIrw/cmake/ExternalEIGEN3.cmake`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/libCZIrw/cmake/TestLargeFile.cmake` & `pylibCZIrw-3.4.1/libs/libCZIrw/cmake/TestLargeFile.cmake`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/libCZIrw/cmake/check_can_use_neon_intrinsics.cmake` & `pylibCZIrw-3.4.1/libs/libCZIrw/cmake/check_can_use_neon_intrinsics.cmake`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/libCZIrw/cmake/check_unaligned_access.cmake` & `pylibCZIrw-3.4.1/libs/libCZIrw/cmake/check_unaligned_access.cmake`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/pybind11/.appveyor.yml` & `pylibCZIrw-3.4.1/libs/pybind11/.appveyor.yml`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/pybind11/.clang-format` & `pylibCZIrw-3.4.1/libs/pybind11/.clang-format`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/pybind11/.clang-tidy` & `pylibCZIrw-3.4.1/libs/pybind11/.clang-tidy`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/pybind11/.cmake-format.yaml` & `pylibCZIrw-3.4.1/libs/pybind11/.cmake-format.yaml`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/pybind11/.github/CONTRIBUTING.md` & `pylibCZIrw-3.4.1/libs/pybind11/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/pybind11/.github/ISSUE_TEMPLATE/bug-report.yml` & `pylibCZIrw-3.4.1/libs/pybind11/.github/ISSUE_TEMPLATE/bug-report.yml`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/pybind11/.github/dependabot.yml` & `pylibCZIrw-3.4.1/libs/pybind11/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/pybind11/.github/pull_request_template.md` & `pylibCZIrw-3.4.1/libs/pybind11/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/pybind11/.github/workflows/ci.yml` & `pylibCZIrw-3.4.1/libs/pybind11/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/pybind11/.github/workflows/configure.yml` & `pylibCZIrw-3.4.1/libs/pybind11/.github/workflows/configure.yml`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/pybind11/.github/workflows/format.yml` & `pylibCZIrw-3.4.1/libs/pybind11/.github/workflows/format.yml`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/pybind11/.github/workflows/pip.yml` & `pylibCZIrw-3.4.1/libs/pybind11/.github/workflows/pip.yml`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/pybind11/.github/workflows/upstream.yml` & `pylibCZIrw-3.4.1/libs/pybind11/.github/workflows/upstream.yml`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/pybind11/.gitignore` & `pylibCZIrw-3.4.1/libs/pybind11/.gitignore`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/pybind11/.pre-commit-config.yaml` & `pylibCZIrw-3.4.1/libs/pybind11/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/pybind11/CMakeLists.txt` & `pylibCZIrw-3.4.1/libs/pybind11/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/pybind11/LICENSE` & `pylibCZIrw-3.4.1/libs/pybind11/LICENSE`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/pybind11/README.rst` & `pylibCZIrw-3.4.1/libs/pybind11/README.rst`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/pybind11/docs/Doxyfile` & `pylibCZIrw-3.4.1/libs/pybind11/docs/Doxyfile`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/pybind11/docs/Makefile` & `pylibCZIrw-3.4.1/libs/pybind11/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/pybind11/docs/advanced/cast/chrono.rst` & `pylibCZIrw-3.4.1/libs/pybind11/docs/advanced/cast/chrono.rst`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/pybind11/docs/advanced/cast/custom.rst` & `pylibCZIrw-3.4.1/libs/pybind11/docs/advanced/cast/custom.rst`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/pybind11/docs/advanced/cast/eigen.rst` & `pylibCZIrw-3.4.1/libs/pybind11/docs/advanced/cast/eigen.rst`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/pybind11/docs/advanced/cast/functional.rst` & `pylibCZIrw-3.4.1/libs/pybind11/docs/advanced/cast/functional.rst`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/pybind11/docs/advanced/cast/index.rst` & `pylibCZIrw-3.4.1/libs/pybind11/docs/advanced/cast/index.rst`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/pybind11/docs/advanced/cast/overview.rst` & `pylibCZIrw-3.4.1/libs/pybind11/docs/advanced/cast/overview.rst`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/pybind11/docs/advanced/cast/stl.rst` & `pylibCZIrw-3.4.1/libs/pybind11/docs/advanced/cast/stl.rst`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/pybind11/docs/advanced/cast/strings.rst` & `pylibCZIrw-3.4.1/libs/pybind11/docs/advanced/cast/strings.rst`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/pybind11/docs/advanced/classes.rst` & `pylibCZIrw-3.4.1/libs/pybind11/docs/advanced/classes.rst`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/pybind11/docs/advanced/embedding.rst` & `pylibCZIrw-3.4.1/libs/pybind11/docs/advanced/embedding.rst`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/pybind11/docs/advanced/exceptions.rst` & `pylibCZIrw-3.4.1/libs/pybind11/docs/advanced/exceptions.rst`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/pybind11/docs/advanced/functions.rst` & `pylibCZIrw-3.4.1/libs/pybind11/docs/advanced/functions.rst`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/pybind11/docs/advanced/misc.rst` & `pylibCZIrw-3.4.1/libs/pybind11/docs/advanced/misc.rst`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/pybind11/docs/advanced/pycpp/numpy.rst` & `pylibCZIrw-3.4.1/libs/pybind11/docs/advanced/pycpp/numpy.rst`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/pybind11/docs/advanced/pycpp/object.rst` & `pylibCZIrw-3.4.1/libs/pybind11/docs/advanced/pycpp/object.rst`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/pybind11/docs/advanced/pycpp/utilities.rst` & `pylibCZIrw-3.4.1/libs/pybind11/docs/advanced/pycpp/utilities.rst`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/pybind11/docs/advanced/smart_ptrs.rst` & `pylibCZIrw-3.4.1/libs/pybind11/docs/advanced/smart_ptrs.rst`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/pybind11/docs/basics.rst` & `pylibCZIrw-3.4.1/libs/pybind11/docs/basics.rst`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/pybind11/docs/benchmark.py` & `pylibCZIrw-3.4.1/libs/pybind11/docs/benchmark.py`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/pybind11/docs/benchmark.rst` & `pylibCZIrw-3.4.1/libs/pybind11/docs/benchmark.rst`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/pybind11/docs/changelog.rst` & `pylibCZIrw-3.4.1/libs/pybind11/docs/changelog.rst`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/pybind11/docs/classes.rst` & `pylibCZIrw-3.4.1/libs/pybind11/docs/classes.rst`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/pybind11/docs/compiling.rst` & `pylibCZIrw-3.4.1/libs/pybind11/docs/compiling.rst`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/pybind11/docs/conf.py` & `pylibCZIrw-3.4.1/libs/pybind11/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/pybind11/docs/faq.rst` & `pylibCZIrw-3.4.1/libs/pybind11/docs/faq.rst`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/pybind11/docs/index.rst` & `pylibCZIrw-3.4.1/libs/pybind11/docs/index.rst`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/pybind11/docs/installing.rst` & `pylibCZIrw-3.4.1/libs/pybind11/docs/installing.rst`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/pybind11/docs/limitations.rst` & `pylibCZIrw-3.4.1/libs/pybind11/docs/limitations.rst`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/pybind11/docs/pybind11-logo.png` & `pylibCZIrw-3.4.1/libs/pybind11/docs/pybind11-logo.png`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/pybind11/docs/pybind11_vs_boost_python1.png` & `pylibCZIrw-3.4.1/libs/pybind11/docs/pybind11_vs_boost_python1.png`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/pybind11/docs/pybind11_vs_boost_python1.svg` & `pylibCZIrw-3.4.1/libs/pybind11/docs/pybind11_vs_boost_python1.svg`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/pybind11/docs/pybind11_vs_boost_python2.png` & `pylibCZIrw-3.4.1/libs/pybind11/docs/pybind11_vs_boost_python2.png`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/pybind11/docs/pybind11_vs_boost_python2.svg` & `pylibCZIrw-3.4.1/libs/pybind11/docs/pybind11_vs_boost_python2.svg`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/pybind11/docs/reference.rst` & `pylibCZIrw-3.4.1/libs/pybind11/docs/reference.rst`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/pybind11/docs/release.rst` & `pylibCZIrw-3.4.1/libs/pybind11/docs/release.rst`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/pybind11/docs/upgrade.rst` & `pylibCZIrw-3.4.1/libs/pybind11/docs/upgrade.rst`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/pybind11/include/pybind11/attr.h` & `pylibCZIrw-3.4.1/libs/pybind11/include/pybind11/attr.h`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/pybind11/include/pybind11/buffer_info.h` & `pylibCZIrw-3.4.1/libs/pybind11/include/pybind11/buffer_info.h`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/pybind11/include/pybind11/cast.h` & `pylibCZIrw-3.4.1/libs/pybind11/include/pybind11/cast.h`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/pybind11/include/pybind11/chrono.h` & `pylibCZIrw-3.4.1/libs/pybind11/include/pybind11/chrono.h`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/pybind11/include/pybind11/complex.h` & `pylibCZIrw-3.4.1/libs/pybind11/include/pybind11/complex.h`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/pybind11/include/pybind11/detail/class.h` & `pylibCZIrw-3.4.1/libs/pybind11/include/pybind11/detail/class.h`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/pybind11/include/pybind11/detail/common.h` & `pylibCZIrw-3.4.1/libs/pybind11/include/pybind11/detail/common.h`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/pybind11/include/pybind11/detail/descr.h` & `pylibCZIrw-3.4.1/libs/pybind11/include/pybind11/detail/descr.h`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/pybind11/include/pybind11/detail/init.h` & `pylibCZIrw-3.4.1/libs/pybind11/include/pybind11/detail/init.h`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/pybind11/include/pybind11/detail/internals.h` & `pylibCZIrw-3.4.1/libs/pybind11/include/pybind11/detail/internals.h`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/pybind11/include/pybind11/detail/type_caster_base.h` & `pylibCZIrw-3.4.1/libs/pybind11/include/pybind11/detail/type_caster_base.h`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/pybind11/include/pybind11/detail/typeid.h` & `pylibCZIrw-3.4.1/libs/pybind11/include/pybind11/detail/typeid.h`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/pybind11/include/pybind11/eigen.h` & `pylibCZIrw-3.4.1/libs/pybind11/include/pybind11/eigen.h`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/pybind11/include/pybind11/embed.h` & `pylibCZIrw-3.4.1/libs/pybind11/include/pybind11/embed.h`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/pybind11/include/pybind11/eval.h` & `pylibCZIrw-3.4.1/libs/pybind11/include/pybind11/eval.h`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/pybind11/include/pybind11/functional.h` & `pylibCZIrw-3.4.1/libs/pybind11/include/pybind11/functional.h`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/pybind11/include/pybind11/gil.h` & `pylibCZIrw-3.4.1/libs/pybind11/include/pybind11/gil.h`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/pybind11/include/pybind11/iostream.h` & `pylibCZIrw-3.4.1/libs/pybind11/include/pybind11/iostream.h`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/pybind11/include/pybind11/numpy.h` & `pylibCZIrw-3.4.1/libs/pybind11/include/pybind11/numpy.h`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/pybind11/include/pybind11/operators.h` & `pylibCZIrw-3.4.1/libs/pybind11/include/pybind11/operators.h`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/pybind11/include/pybind11/options.h` & `pylibCZIrw-3.4.1/libs/pybind11/include/pybind11/options.h`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/pybind11/include/pybind11/pybind11.h` & `pylibCZIrw-3.4.1/libs/pybind11/include/pybind11/pybind11.h`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/pybind11/include/pybind11/pytypes.h` & `pylibCZIrw-3.4.1/libs/pybind11/include/pybind11/pytypes.h`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/pybind11/include/pybind11/stl/filesystem.h` & `pylibCZIrw-3.4.1/libs/pybind11/include/pybind11/stl/filesystem.h`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/pybind11/include/pybind11/stl.h` & `pylibCZIrw-3.4.1/libs/pybind11/include/pybind11/stl.h`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/pybind11/include/pybind11/stl_bind.h` & `pylibCZIrw-3.4.1/libs/pybind11/include/pybind11/stl_bind.h`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/pybind11/noxfile.py` & `pylibCZIrw-3.4.1/libs/pybind11/noxfile.py`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/pybind11/pybind11/__main__.py` & `pylibCZIrw-3.4.1/libs/pybind11/pybind11/__main__.py`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/pybind11/pybind11/commands.py` & `pylibCZIrw-3.4.1/libs/pybind11/pybind11/commands.py`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/pybind11/pybind11/setup_helpers.py` & `pylibCZIrw-3.4.1/libs/pybind11/pybind11/setup_helpers.py`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/pybind11/pybind11/setup_helpers.pyi` & `pylibCZIrw-3.4.1/libs/pybind11/pybind11/setup_helpers.pyi`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/pybind11/pyproject.toml` & `pylibCZIrw-3.4.1/libs/pybind11/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/pybind11/setup.cfg` & `pylibCZIrw-3.4.1/libs/pybind11/setup.cfg`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/pybind11/setup.py` & `pylibCZIrw-3.4.1/libs/pybind11/setup.py`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/pybind11/tests/CMakeLists.txt` & `pylibCZIrw-3.4.1/libs/pybind11/tests/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/pybind11/tests/conftest.py` & `pylibCZIrw-3.4.1/libs/pybind11/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/pybind11/tests/constructor_stats.h` & `pylibCZIrw-3.4.1/libs/pybind11/tests/constructor_stats.h`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/pybind11/tests/cross_module_gil_utils.cpp` & `pylibCZIrw-3.4.1/libs/pybind11/tests/cross_module_gil_utils.cpp`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/pybind11/tests/env.py` & `pylibCZIrw-3.4.1/libs/pybind11/tests/env.py`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/pybind11/tests/extra_python_package/test_files.py` & `pylibCZIrw-3.4.1/libs/pybind11/tests/extra_python_package/test_files.py`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/pybind11/tests/extra_setuptools/test_setuphelper.py` & `pylibCZIrw-3.4.1/libs/pybind11/tests/extra_setuptools/test_setuphelper.py`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/pybind11/tests/local_bindings.h` & `pylibCZIrw-3.4.1/libs/pybind11/tests/local_bindings.h`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/pybind11/tests/object.h` & `pylibCZIrw-3.4.1/libs/pybind11/tests/object.h`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/pybind11/tests/pybind11_cross_module_tests.cpp` & `pylibCZIrw-3.4.1/libs/pybind11/tests/pybind11_cross_module_tests.cpp`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/pybind11/tests/pybind11_tests.cpp` & `pylibCZIrw-3.4.1/libs/pybind11/tests/pybind11_tests.cpp`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/pybind11/tests/pybind11_tests.h` & `pylibCZIrw-3.4.1/libs/pybind11/tests/pybind11_tests.h`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/pybind11/tests/pytest.ini` & `pylibCZIrw-3.4.1/libs/pybind11/tests/pytest.ini`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/pybind11/tests/requirements.txt` & `pylibCZIrw-3.4.1/libs/pybind11/tests/requirements.txt`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/pybind11/tests/test_async.cpp` & `pylibCZIrw-3.4.1/libs/pybind11/tests/test_async.cpp`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/pybind11/tests/test_async.py` & `pylibCZIrw-3.4.1/libs/pybind11/tests/test_async.py`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/pybind11/tests/test_buffers.cpp` & `pylibCZIrw-3.4.1/libs/pybind11/tests/test_buffers.cpp`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/pybind11/tests/test_buffers.py` & `pylibCZIrw-3.4.1/libs/pybind11/tests/test_buffers.py`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/pybind11/tests/test_builtin_casters.cpp` & `pylibCZIrw-3.4.1/libs/pybind11/tests/test_builtin_casters.cpp`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/pybind11/tests/test_builtin_casters.py` & `pylibCZIrw-3.4.1/libs/pybind11/tests/test_builtin_casters.py`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/pybind11/tests/test_call_policies.cpp` & `pylibCZIrw-3.4.1/libs/pybind11/tests/test_call_policies.cpp`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/pybind11/tests/test_call_policies.py` & `pylibCZIrw-3.4.1/libs/pybind11/tests/test_call_policies.py`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/pybind11/tests/test_callbacks.cpp` & `pylibCZIrw-3.4.1/libs/pybind11/tests/test_callbacks.cpp`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/pybind11/tests/test_callbacks.py` & `pylibCZIrw-3.4.1/libs/pybind11/tests/test_callbacks.py`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/pybind11/tests/test_chrono.cpp` & `pylibCZIrw-3.4.1/libs/pybind11/tests/test_chrono.cpp`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/pybind11/tests/test_chrono.py` & `pylibCZIrw-3.4.1/libs/pybind11/tests/test_chrono.py`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/pybind11/tests/test_class.cpp` & `pylibCZIrw-3.4.1/libs/pybind11/tests/test_class.cpp`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/pybind11/tests/test_class.py` & `pylibCZIrw-3.4.1/libs/pybind11/tests/test_class.py`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/pybind11/tests/test_cmake_build/CMakeLists.txt` & `pylibCZIrw-3.4.1/libs/pybind11/tests/test_cmake_build/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/pybind11/tests/test_cmake_build/embed.cpp` & `pylibCZIrw-3.4.1/libs/pybind11/tests/test_cmake_build/embed.cpp`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/pybind11/tests/test_cmake_build/installed_embed/CMakeLists.txt` & `pylibCZIrw-3.4.1/libs/pybind11/tests/test_cmake_build/installed_embed/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/pybind11/tests/test_cmake_build/installed_function/CMakeLists.txt` & `pylibCZIrw-3.4.1/libs/pybind11/tests/test_cmake_build/installed_function/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/pybind11/tests/test_cmake_build/installed_target/CMakeLists.txt` & `pylibCZIrw-3.4.1/libs/pybind11/tests/test_cmake_build/installed_target/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/pybind11/tests/test_cmake_build/subdirectory_embed/CMakeLists.txt` & `pylibCZIrw-3.4.1/libs/pybind11/tests/test_cmake_build/subdirectory_embed/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/pybind11/tests/test_cmake_build/subdirectory_function/CMakeLists.txt` & `pylibCZIrw-3.4.1/libs/pybind11/tests/test_cmake_build/subdirectory_function/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/pybind11/tests/test_cmake_build/subdirectory_target/CMakeLists.txt` & `pylibCZIrw-3.4.1/libs/pybind11/tests/test_cmake_build/subdirectory_target/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/pybind11/tests/test_const_name.cpp` & `pylibCZIrw-3.4.1/libs/pybind11/tests/test_const_name.cpp`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/pybind11/tests/test_const_name.py` & `pylibCZIrw-3.4.1/libs/pybind11/tests/test_const_name.py`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/pybind11/tests/test_constants_and_functions.cpp` & `pylibCZIrw-3.4.1/libs/pybind11/tests/test_constants_and_functions.cpp`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/pybind11/tests/test_constants_and_functions.py` & `pylibCZIrw-3.4.1/libs/pybind11/tests/test_constants_and_functions.py`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/pybind11/tests/test_copy_move.cpp` & `pylibCZIrw-3.4.1/libs/pybind11/tests/test_copy_move.cpp`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/pybind11/tests/test_copy_move.py` & `pylibCZIrw-3.4.1/libs/pybind11/tests/test_copy_move.py`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/pybind11/tests/test_custom_type_casters.cpp` & `pylibCZIrw-3.4.1/libs/pybind11/tests/test_custom_type_casters.cpp`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/pybind11/tests/test_custom_type_casters.py` & `pylibCZIrw-3.4.1/libs/pybind11/tests/test_custom_type_casters.py`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/pybind11/tests/test_custom_type_setup.cpp` & `pylibCZIrw-3.4.1/libs/pybind11/tests/test_custom_type_setup.cpp`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/pybind11/tests/test_custom_type_setup.py` & `pylibCZIrw-3.4.1/libs/pybind11/tests/test_custom_type_setup.py`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/pybind11/tests/test_docstring_options.cpp` & `pylibCZIrw-3.4.1/libs/pybind11/tests/test_docstring_options.cpp`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/pybind11/tests/test_docstring_options.py` & `pylibCZIrw-3.4.1/libs/pybind11/tests/test_docstring_options.py`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/pybind11/tests/test_eigen.cpp` & `pylibCZIrw-3.4.1/libs/pybind11/tests/test_eigen.cpp`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/pybind11/tests/test_eigen.py` & `pylibCZIrw-3.4.1/libs/pybind11/tests/test_eigen.py`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/pybind11/tests/test_embed/CMakeLists.txt` & `pylibCZIrw-3.4.1/libs/pybind11/tests/test_embed/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/pybind11/tests/test_embed/catch.cpp` & `pylibCZIrw-3.4.1/libs/pybind11/tests/test_embed/catch.cpp`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/pybind11/tests/test_embed/external_module.cpp` & `pylibCZIrw-3.4.1/libs/pybind11/tests/test_embed/external_module.cpp`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/pybind11/tests/test_embed/test_interpreter.cpp` & `pylibCZIrw-3.4.1/libs/pybind11/tests/test_embed/test_interpreter.cpp`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/pybind11/tests/test_enum.cpp` & `pylibCZIrw-3.4.1/libs/pybind11/tests/test_enum.cpp`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/pybind11/tests/test_enum.py` & `pylibCZIrw-3.4.1/libs/pybind11/tests/test_enum.py`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/pybind11/tests/test_eval.cpp` & `pylibCZIrw-3.4.1/libs/pybind11/tests/test_eval.cpp`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/pybind11/tests/test_eval.py` & `pylibCZIrw-3.4.1/libs/pybind11/tests/test_eval.py`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/pybind11/tests/test_exceptions.cpp` & `pylibCZIrw-3.4.1/libs/pybind11/tests/test_exceptions.cpp`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/pybind11/tests/test_exceptions.py` & `pylibCZIrw-3.4.1/libs/pybind11/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/pybind11/tests/test_factory_constructors.cpp` & `pylibCZIrw-3.4.1/libs/pybind11/tests/test_factory_constructors.cpp`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/pybind11/tests/test_factory_constructors.py` & `pylibCZIrw-3.4.1/libs/pybind11/tests/test_factory_constructors.py`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/pybind11/tests/test_gil_scoped.cpp` & `pylibCZIrw-3.4.1/libs/pybind11/tests/test_gil_scoped.cpp`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/pybind11/tests/test_gil_scoped.py` & `pylibCZIrw-3.4.1/libs/pybind11/tests/test_gil_scoped.py`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/pybind11/tests/test_iostream.cpp` & `pylibCZIrw-3.4.1/libs/pybind11/tests/test_iostream.cpp`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/pybind11/tests/test_iostream.py` & `pylibCZIrw-3.4.1/libs/pybind11/tests/test_iostream.py`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/pybind11/tests/test_kwargs_and_defaults.cpp` & `pylibCZIrw-3.4.1/libs/pybind11/tests/test_kwargs_and_defaults.cpp`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/pybind11/tests/test_kwargs_and_defaults.py` & `pylibCZIrw-3.4.1/libs/pybind11/tests/test_kwargs_and_defaults.py`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/pybind11/tests/test_local_bindings.cpp` & `pylibCZIrw-3.4.1/libs/pybind11/tests/test_local_bindings.cpp`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/pybind11/tests/test_local_bindings.py` & `pylibCZIrw-3.4.1/libs/pybind11/tests/test_local_bindings.py`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/pybind11/tests/test_methods_and_attributes.cpp` & `pylibCZIrw-3.4.1/libs/pybind11/tests/test_methods_and_attributes.cpp`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/pybind11/tests/test_methods_and_attributes.py` & `pylibCZIrw-3.4.1/libs/pybind11/tests/test_methods_and_attributes.py`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/pybind11/tests/test_modules.cpp` & `pylibCZIrw-3.4.1/libs/pybind11/tests/test_modules.cpp`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/pybind11/tests/test_modules.py` & `pylibCZIrw-3.4.1/libs/pybind11/tests/test_modules.py`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/pybind11/tests/test_multiple_inheritance.cpp` & `pylibCZIrw-3.4.1/libs/pybind11/tests/test_multiple_inheritance.cpp`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/pybind11/tests/test_multiple_inheritance.py` & `pylibCZIrw-3.4.1/libs/pybind11/tests/test_multiple_inheritance.py`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/pybind11/tests/test_numpy_array.cpp` & `pylibCZIrw-3.4.1/libs/pybind11/tests/test_numpy_array.cpp`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/pybind11/tests/test_numpy_array.py` & `pylibCZIrw-3.4.1/libs/pybind11/tests/test_numpy_array.py`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/pybind11/tests/test_numpy_dtypes.cpp` & `pylibCZIrw-3.4.1/libs/pybind11/tests/test_numpy_dtypes.cpp`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/pybind11/tests/test_numpy_dtypes.py` & `pylibCZIrw-3.4.1/libs/pybind11/tests/test_numpy_dtypes.py`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/pybind11/tests/test_numpy_vectorize.cpp` & `pylibCZIrw-3.4.1/libs/pybind11/tests/test_numpy_vectorize.cpp`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/pybind11/tests/test_numpy_vectorize.py` & `pylibCZIrw-3.4.1/libs/pybind11/tests/test_numpy_vectorize.py`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/pybind11/tests/test_opaque_types.cpp` & `pylibCZIrw-3.4.1/libs/pybind11/tests/test_opaque_types.cpp`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/pybind11/tests/test_opaque_types.py` & `pylibCZIrw-3.4.1/libs/pybind11/tests/test_opaque_types.py`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/pybind11/tests/test_operator_overloading.cpp` & `pylibCZIrw-3.4.1/libs/pybind11/tests/test_operator_overloading.cpp`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/pybind11/tests/test_operator_overloading.py` & `pylibCZIrw-3.4.1/libs/pybind11/tests/test_operator_overloading.py`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/pybind11/tests/test_pickling.cpp` & `pylibCZIrw-3.4.1/libs/pybind11/tests/test_pickling.cpp`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/pybind11/tests/test_pickling.py` & `pylibCZIrw-3.4.1/libs/pybind11/tests/test_pickling.py`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/pybind11/tests/test_pytypes.cpp` & `pylibCZIrw-3.4.1/libs/pybind11/tests/test_pytypes.cpp`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/pybind11/tests/test_pytypes.py` & `pylibCZIrw-3.4.1/libs/pybind11/tests/test_pytypes.py`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/pybind11/tests/test_sequences_and_iterators.cpp` & `pylibCZIrw-3.4.1/libs/pybind11/tests/test_sequences_and_iterators.cpp`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/pybind11/tests/test_sequences_and_iterators.py` & `pylibCZIrw-3.4.1/libs/pybind11/tests/test_sequences_and_iterators.py`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/pybind11/tests/test_smart_ptr.cpp` & `pylibCZIrw-3.4.1/libs/pybind11/tests/test_smart_ptr.cpp`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/pybind11/tests/test_smart_ptr.py` & `pylibCZIrw-3.4.1/libs/pybind11/tests/test_smart_ptr.py`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/pybind11/tests/test_stl.cpp` & `pylibCZIrw-3.4.1/libs/pybind11/tests/test_stl.cpp`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/pybind11/tests/test_stl.py` & `pylibCZIrw-3.4.1/libs/pybind11/tests/test_stl.py`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/pybind11/tests/test_stl_binders.cpp` & `pylibCZIrw-3.4.1/libs/pybind11/tests/test_stl_binders.cpp`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/pybind11/tests/test_stl_binders.py` & `pylibCZIrw-3.4.1/libs/pybind11/tests/test_stl_binders.py`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/pybind11/tests/test_tagbased_polymorphic.cpp` & `pylibCZIrw-3.4.1/libs/pybind11/tests/test_tagbased_polymorphic.cpp`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/pybind11/tests/test_tagbased_polymorphic.py` & `pylibCZIrw-3.4.1/libs/pybind11/tests/test_tagbased_polymorphic.py`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/pybind11/tests/test_thread.cpp` & `pylibCZIrw-3.4.1/libs/pybind11/tests/test_thread.cpp`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/pybind11/tests/test_thread.py` & `pylibCZIrw-3.4.1/libs/pybind11/tests/test_thread.py`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/pybind11/tests/test_union.cpp` & `pylibCZIrw-3.4.1/libs/pybind11/tests/test_union.cpp`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/pybind11/tests/test_virtual_functions.cpp` & `pylibCZIrw-3.4.1/libs/pybind11/tests/test_virtual_functions.cpp`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/pybind11/tests/test_virtual_functions.py` & `pylibCZIrw-3.4.1/libs/pybind11/tests/test_virtual_functions.py`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/pybind11/tests/valgrind-numpy-scipy.supp` & `pylibCZIrw-3.4.1/libs/pybind11/tests/valgrind-numpy-scipy.supp`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/pybind11/tests/valgrind-python.supp` & `pylibCZIrw-3.4.1/libs/pybind11/tests/valgrind-python.supp`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/pybind11/tools/FindCatch.cmake` & `pylibCZIrw-3.4.1/libs/pybind11/tools/FindCatch.cmake`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/pybind11/tools/FindEigen3.cmake` & `pylibCZIrw-3.4.1/libs/pybind11/tools/FindEigen3.cmake`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/pybind11/tools/FindPythonLibsNew.cmake` & `pylibCZIrw-3.4.1/libs/pybind11/tools/FindPythonLibsNew.cmake`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/pybind11/tools/check-style.sh` & `pylibCZIrw-3.4.1/libs/pybind11/tools/check-style.sh`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/pybind11/tools/cmake_uninstall.cmake.in` & `pylibCZIrw-3.4.1/libs/pybind11/tools/cmake_uninstall.cmake.in`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/pybind11/tools/libsize.py` & `pylibCZIrw-3.4.1/libs/pybind11/tools/libsize.py`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/pybind11/tools/make_changelog.py` & `pylibCZIrw-3.4.1/libs/pybind11/tools/make_changelog.py`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/pybind11/tools/pybind11Common.cmake` & `pylibCZIrw-3.4.1/libs/pybind11/tools/pybind11Common.cmake`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/pybind11/tools/pybind11Config.cmake.in` & `pylibCZIrw-3.4.1/libs/pybind11/tools/pybind11Config.cmake.in`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/pybind11/tools/pybind11NewTools.cmake` & `pylibCZIrw-3.4.1/libs/pybind11/tools/pybind11NewTools.cmake`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/pybind11/tools/pybind11Tools.cmake` & `pylibCZIrw-3.4.1/libs/pybind11/tools/pybind11Tools.cmake`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/pybind11/tools/setup_global.py.in` & `pylibCZIrw-3.4.1/libs/pybind11/tools/setup_global.py.in`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/libs/pybind11/tools/setup_main.py.in` & `pylibCZIrw-3.4.1/libs/pybind11/tools/setup_main.py.in`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/pylibCZIrw/__init__.py` & `pylibCZIrw-3.4.1/pylibCZIrw/__init__.py`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/pylibCZIrw/czi.py` & `pylibCZIrw-3.4.1/pylibCZIrw/czi.py`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/pylibCZIrw-documentation.html` & `pylibCZIrw-3.4.1/pylibCZIrw-documentation.html`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/pylibCZIrw.egg-info/PKG-INFO` & `pylibCZIrw-3.4.1/pylibCZIrw.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pylibCZIrw
-Version: 3.4.0
+Version: 3.4.1
 Summary: A python wrapper around the libCZI C++ library with reading and writing functionality.
 Home-page: UNKNOWN
 Author: Felix Scheffler
 Author-email: felix.scheffler@zeiss.com
 License: UNKNOWN
 Keywords: czi,imaging
 Platform: UNKNOWN
```

### Comparing `pylibCZIrw-3.4.0/pylibCZIrw.egg-info/SOURCES.txt` & `pylibCZIrw-3.4.1/pylibCZIrw.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/setup.cfg` & `pylibCZIrw-3.4.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `pylibCZIrw-3.4.0/setup.py` & `pylibCZIrw-3.4.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from pathlib import Path
 import platform
 import re
 import subprocess
 import sys
 from distutils.version import LooseVersion
 
-VERSION = "3.4.0"
+VERSION = "3.4.1"
 
 
 with open("INFO.md") as readme_file:
     readme = readme_file.read()
 
 # List any runtime requirements here
 requirements = ["numpy", "cmake", "xmltodict"]
```

