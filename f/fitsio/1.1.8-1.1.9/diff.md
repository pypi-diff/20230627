# Comparing `tmp/fitsio-1.1.8.tar.gz` & `tmp/fitsio-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fitsio-1.1.8.tar", last modified: Tue Sep 27 14:14:39 2022, max compression
+gzip compressed data, was "fitsio-1.1.9.tar", last modified: Fri May 26 13:06:55 2023, max compression
```

## Comparing `fitsio-1.1.8.tar` & `fitsio-1.1.9.tar`

### file list

```diff
@@ -1,211 +1,228 @@
-drwxrwxr-x   0 esheldon  (1000) esheldon  (1000)        0 2022-09-27 14:14:39.099974 fitsio-1.1.8/
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)    18011 2021-03-26 15:14:38.000000 fitsio-1.1.8/LICENSE.txt
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)      131 2021-03-26 15:14:38.000000 fitsio-1.1.8/MANIFEST.in
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)    15660 2022-09-27 14:14:39.099974 fitsio-1.1.8/PKG-INFO
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)    15059 2021-03-26 15:14:38.000000 fitsio-1.1.8/README.md
-drwxrwxr-x   0 esheldon  (1000) esheldon  (1000)        0 2022-09-27 14:14:39.067974 fitsio-1.1.8/cfitsio3490/
--rwxrwxr-x   0 esheldon  (1000) esheldon  (1000)     6405 2021-03-26 15:14:38.000000 fitsio-1.1.8/cfitsio3490/CMakeLists.txt
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)     3209 2021-03-26 15:14:38.000000 fitsio-1.1.8/cfitsio3490/FindPthreads.cmake
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)     1410 2021-03-26 15:14:38.000000 fitsio-1.1.8/cfitsio3490/License.txt
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)     6236 2021-03-26 15:14:38.000000 fitsio-1.1.8/cfitsio3490/Makefile.in
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)     4528 2021-03-26 15:14:38.000000 fitsio-1.1.8/cfitsio3490/README
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)     2493 2021-03-26 15:14:38.000000 fitsio-1.1.8/cfitsio3490/README.MacOS
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)     6134 2021-03-26 15:14:38.000000 fitsio-1.1.8/cfitsio3490/README.win
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)     3534 2021-03-26 15:14:38.000000 fitsio-1.1.8/cfitsio3490/README_OLD.win
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)    53229 2021-03-26 15:14:38.000000 fitsio-1.1.8/cfitsio3490/buffers.c
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)   263595 2021-03-26 15:14:38.000000 fitsio-1.1.8/cfitsio3490/cfileio.c
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)      342 2021-03-26 15:14:38.000000 fitsio-1.1.8/cfitsio3490/cfitsio.pc.cmake
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)      300 2021-03-26 15:14:38.000000 fitsio-1.1.8/cfitsio3490/cfitsio.pc.in
-drwxrwxr-x   0 esheldon  (1000) esheldon  (1000)        0 2022-09-27 14:14:39.067974 fitsio-1.1.8/cfitsio3490/cfitsio.xcodeproj/
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)     3233 2021-03-26 15:14:38.000000 fitsio-1.1.8/cfitsio3490/cfitsio.xcodeproj/project.pbxproj
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)    23366 2021-03-26 15:14:38.000000 fitsio-1.1.8/cfitsio3490/cfitsio_mac.sit.hqx
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)   135706 2021-03-26 15:14:38.000000 fitsio-1.1.8/cfitsio3490/cfortran.h
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)    17601 2021-03-26 15:14:38.000000 fitsio-1.1.8/cfitsio3490/checksum.c
--rwxrwxr-x   0 esheldon  (1000) esheldon  (1000)    44283 2021-03-26 15:14:38.000000 fitsio-1.1.8/cfitsio3490/config.guess
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)    23466 2021-09-07 13:51:31.000000 fitsio-1.1.8/cfitsio3490/config.log
--rwxrwxr-x   0 esheldon  (1000) esheldon  (1000)    36136 2021-03-26 15:14:38.000000 fitsio-1.1.8/cfitsio3490/config.sub
--rwxrwxr-x   0 esheldon  (1000) esheldon  (1000)   219087 2021-03-26 15:14:38.000000 fitsio-1.1.8/cfitsio3490/configure
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)    20705 2021-03-26 15:14:38.000000 fitsio-1.1.8/cfitsio3490/configure.in
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)    21858 2021-03-26 15:14:38.000000 fitsio-1.1.8/cfitsio3490/cookbook.c
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)    30203 2021-03-26 15:14:38.000000 fitsio-1.1.8/cfitsio3490/cookbook.f
-drwxrwxr-x   0 esheldon  (1000) esheldon  (1000)        0 2022-09-27 14:14:39.087974 fitsio-1.1.8/cfitsio3490/docs/
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)  1074054 2021-03-26 15:14:38.000000 fitsio-1.1.8/cfitsio3490/docs/cfitsio.pdf
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)  1412279 2021-03-26 15:14:38.000000 fitsio-1.1.8/cfitsio3490/docs/cfitsio.ps
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)   507182 2021-03-26 15:14:38.000000 fitsio-1.1.8/cfitsio3490/docs/cfitsio.tex
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)    11521 2021-03-26 15:14:38.000000 fitsio-1.1.8/cfitsio3490/docs/cfitsio.toc
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)    95483 2021-03-26 15:14:38.000000 fitsio-1.1.8/cfitsio3490/docs/cfortran.doc
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)   213622 2021-03-26 15:14:38.000000 fitsio-1.1.8/cfitsio3490/docs/changes.txt
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)   326397 2021-03-26 15:14:38.000000 fitsio-1.1.8/cfitsio3490/docs/fitsio.doc
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)   697014 2021-03-26 15:14:38.000000 fitsio-1.1.8/cfitsio3490/docs/fitsio.pdf
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)   958163 2021-03-26 15:14:38.000000 fitsio-1.1.8/cfitsio3490/docs/fitsio.ps
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)   346564 2021-03-26 15:14:38.000000 fitsio-1.1.8/cfitsio3490/docs/fitsio.tex
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)     8707 2021-03-26 15:14:38.000000 fitsio-1.1.8/cfitsio3490/docs/fitsio.toc
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)   588666 2021-03-26 15:14:38.000000 fitsio-1.1.8/cfitsio3490/docs/fpackguide.pdf
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)   232878 2021-03-26 15:14:38.000000 fitsio-1.1.8/cfitsio3490/docs/quick.pdf
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)   312357 2021-03-26 15:14:38.000000 fitsio-1.1.8/cfitsio3490/docs/quick.ps
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)   101448 2021-03-26 15:14:38.000000 fitsio-1.1.8/cfitsio3490/docs/quick.tex
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)     1795 2021-03-26 15:14:38.000000 fitsio-1.1.8/cfitsio3490/docs/quick.toc
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)    28508 2021-03-26 15:14:38.000000 fitsio-1.1.8/cfitsio3490/drvrfile.c
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)    13960 2021-03-26 15:14:38.000000 fitsio-1.1.8/cfitsio3490/drvrgsiftp.c
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)      787 2021-03-26 15:14:38.000000 fitsio-1.1.8/cfitsio3490/drvrgsiftp.h
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)    39553 2021-03-26 15:14:38.000000 fitsio-1.1.8/cfitsio3490/drvrmem.c
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)   125780 2021-03-26 15:14:38.000000 fitsio-1.1.8/cfitsio3490/drvrnet.c
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)    38489 2021-03-26 15:14:38.000000 fitsio-1.1.8/cfitsio3490/drvrsmem.c
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)     6536 2021-03-26 15:14:38.000000 fitsio-1.1.8/cfitsio3490/drvrsmem.h
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)   101807 2021-03-26 15:14:38.000000 fitsio-1.1.8/cfitsio3490/editcol.c
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)    32727 2021-03-26 15:14:38.000000 fitsio-1.1.8/cfitsio3490/edithdu.c
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)    16188 2021-03-26 15:14:38.000000 fitsio-1.1.8/cfitsio3490/eval.l
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)   177512 2021-03-26 15:14:38.000000 fitsio-1.1.8/cfitsio3490/eval.y
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)     4254 2021-03-26 15:14:38.000000 fitsio-1.1.8/cfitsio3490/eval_defs.h
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)    98802 2021-03-26 15:14:38.000000 fitsio-1.1.8/cfitsio3490/eval_f.c
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)    69666 2021-03-26 15:14:38.000000 fitsio-1.1.8/cfitsio3490/eval_l.c
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)     3564 2021-03-26 15:14:38.000000 fitsio-1.1.8/cfitsio3490/eval_tab.h
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)   275403 2021-03-26 15:14:38.000000 fitsio-1.1.8/cfitsio3490/eval_y.c
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)      853 2021-03-26 15:14:38.000000 fitsio-1.1.8/cfitsio3490/f77.inc
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)    10430 2021-03-26 15:14:38.000000 fitsio-1.1.8/cfitsio3490/f77_wrap.h
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)    12779 2021-03-26 15:14:38.000000 fitsio-1.1.8/cfitsio3490/f77_wrap1.c
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)    32385 2021-03-26 15:14:38.000000 fitsio-1.1.8/cfitsio3490/f77_wrap2.c
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)    33790 2021-03-26 15:14:38.000000 fitsio-1.1.8/cfitsio3490/f77_wrap3.c
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)    19467 2021-03-26 15:14:38.000000 fitsio-1.1.8/cfitsio3490/f77_wrap4.c
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)    47082 2021-03-26 15:14:38.000000 fitsio-1.1.8/cfitsio3490/fits_hcompress.c
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)    63312 2021-03-26 15:14:38.000000 fitsio-1.1.8/cfitsio3490/fits_hdecompress.c
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)     2642 2021-03-26 15:14:38.000000 fitsio-1.1.8/cfitsio3490/fitscopy.c
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)   318473 2021-03-26 15:14:38.000000 fitsio-1.1.8/cfitsio3490/fitscore.c
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)   119295 2021-03-26 15:14:38.000000 fitsio-1.1.8/cfitsio3490/fitsio.h
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)    63131 2021-03-26 15:14:38.000000 fitsio-1.1.8/cfitsio3490/fitsio2.h
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)    16825 2021-03-26 15:14:38.000000 fitsio-1.1.8/cfitsio3490/fpack.c
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)     7155 2021-03-26 15:14:38.000000 fitsio-1.1.8/cfitsio3490/fpack.h
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)    78403 2021-03-26 15:14:38.000000 fitsio-1.1.8/cfitsio3490/fpackutil.c
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)     4664 2021-03-26 15:14:38.000000 fitsio-1.1.8/cfitsio3490/funpack.c
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)    41542 2021-03-26 15:14:38.000000 fitsio-1.1.8/cfitsio3490/getcol.c
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)    78585 2021-03-26 15:14:38.000000 fitsio-1.1.8/cfitsio3490/getcolb.c
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)    68830 2021-03-26 15:14:38.000000 fitsio-1.1.8/cfitsio3490/getcold.c
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)    68940 2021-03-26 15:14:38.000000 fitsio-1.1.8/cfitsio3490/getcole.c
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)    74885 2021-03-26 15:14:38.000000 fitsio-1.1.8/cfitsio3490/getcoli.c
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)   148225 2021-03-26 15:14:38.000000 fitsio-1.1.8/cfitsio3490/getcolj.c
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)    74751 2021-03-26 15:14:38.000000 fitsio-1.1.8/cfitsio3490/getcolk.c
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)    23298 2021-03-26 15:14:38.000000 fitsio-1.1.8/cfitsio3490/getcoll.c
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)    33907 2021-03-26 15:14:38.000000 fitsio-1.1.8/cfitsio3490/getcols.c
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)    77347 2021-03-26 15:14:38.000000 fitsio-1.1.8/cfitsio3490/getcolsb.c
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)    75282 2021-03-26 15:14:38.000000 fitsio-1.1.8/cfitsio3490/getcolui.c
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)   148281 2021-03-26 15:14:38.000000 fitsio-1.1.8/cfitsio3490/getcoluj.c
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)    75493 2021-03-26 15:14:38.000000 fitsio-1.1.8/cfitsio3490/getcoluk.c
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)   125729 2021-03-26 15:14:38.000000 fitsio-1.1.8/cfitsio3490/getkey.c
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)   185566 2021-03-26 15:14:38.000000 fitsio-1.1.8/cfitsio3490/group.c
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)     2097 2021-03-26 15:14:38.000000 fitsio-1.1.8/cfitsio3490/group.h
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)    46325 2021-03-26 15:14:38.000000 fitsio-1.1.8/cfitsio3490/grparser.c
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)     5725 2021-03-26 15:14:38.000000 fitsio-1.1.8/cfitsio3490/grparser.h
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)    86820 2021-03-26 15:14:38.000000 fitsio-1.1.8/cfitsio3490/histo.c
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)   380829 2021-03-26 15:14:38.000000 fitsio-1.1.8/cfitsio3490/imcompress.c
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)     9368 2021-03-26 15:14:38.000000 fitsio-1.1.8/cfitsio3490/imcopy.c
--rwxrwxr-x   0 esheldon  (1000) esheldon  (1000)    14799 2021-03-26 15:14:38.000000 fitsio-1.1.8/cfitsio3490/install-sh
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)    57777 2021-03-26 15:14:38.000000 fitsio-1.1.8/cfitsio3490/iraffits.c
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)     5253 2021-03-26 15:14:38.000000 fitsio-1.1.8/cfitsio3490/iter_a.c
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)     6874 2021-03-26 15:14:38.000000 fitsio-1.1.8/cfitsio3490/iter_a.f
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)   129600 2021-03-26 15:14:38.000000 fitsio-1.1.8/cfitsio3490/iter_a.fit
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)     3702 2021-03-26 15:14:38.000000 fitsio-1.1.8/cfitsio3490/iter_b.c
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)     5679 2021-03-26 15:14:38.000000 fitsio-1.1.8/cfitsio3490/iter_b.f
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)   408960 2021-03-26 15:14:38.000000 fitsio-1.1.8/cfitsio3490/iter_b.fit
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)     6007 2021-03-26 15:14:38.000000 fitsio-1.1.8/cfitsio3490/iter_c.c
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)    10525 2021-03-26 15:14:38.000000 fitsio-1.1.8/cfitsio3490/iter_c.f
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)    92160 2021-03-26 15:14:38.000000 fitsio-1.1.8/cfitsio3490/iter_c.fit
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)     3076 2021-03-26 15:14:38.000000 fitsio-1.1.8/cfitsio3490/iter_image.c
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)     3319 2021-03-26 15:14:38.000000 fitsio-1.1.8/cfitsio3490/iter_var.c
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)    21784 2021-03-26 15:14:38.000000 fitsio-1.1.8/cfitsio3490/longnam.h
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)    12754 2021-03-26 15:14:38.000000 fitsio-1.1.8/cfitsio3490/makefile.bc
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)    18040 2021-03-26 15:14:38.000000 fitsio-1.1.8/cfitsio3490/makefile.vcc
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)     2307 2021-03-26 15:14:38.000000 fitsio-1.1.8/cfitsio3490/makepc.bat
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)    67233 2021-03-26 15:14:38.000000 fitsio-1.1.8/cfitsio3490/modkey.c
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)     7067 2021-03-26 15:14:38.000000 fitsio-1.1.8/cfitsio3490/pliocomp.c
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)    67801 2021-03-26 15:14:38.000000 fitsio-1.1.8/cfitsio3490/putcol.c
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)    37199 2021-03-26 15:14:38.000000 fitsio-1.1.8/cfitsio3490/putcolb.c
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)    38722 2021-03-26 15:14:38.000000 fitsio-1.1.8/cfitsio3490/putcold.c
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)    39292 2021-03-26 15:14:38.000000 fitsio-1.1.8/cfitsio3490/putcole.c
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)    35439 2021-03-26 15:14:38.000000 fitsio-1.1.8/cfitsio3490/putcoli.c
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)    71429 2021-03-26 15:14:38.000000 fitsio-1.1.8/cfitsio3490/putcolj.c
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)    36390 2021-03-26 15:14:38.000000 fitsio-1.1.8/cfitsio3490/putcolk.c
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)    13933 2021-03-26 15:14:38.000000 fitsio-1.1.8/cfitsio3490/putcoll.c
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)    10944 2021-03-26 15:14:38.000000 fitsio-1.1.8/cfitsio3490/putcols.c
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)    35466 2021-03-26 15:14:38.000000 fitsio-1.1.8/cfitsio3490/putcolsb.c
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)    21555 2021-03-26 15:14:38.000000 fitsio-1.1.8/cfitsio3490/putcolu.c
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)    34837 2021-03-26 15:14:38.000000 fitsio-1.1.8/cfitsio3490/putcolui.c
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)    69378 2021-03-26 15:14:38.000000 fitsio-1.1.8/cfitsio3490/putcoluj.c
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)    35653 2021-03-26 15:14:38.000000 fitsio-1.1.8/cfitsio3490/putcoluk.c
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)   115057 2021-03-26 15:14:38.000000 fitsio-1.1.8/cfitsio3490/putkey.c
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)   118985 2021-03-26 15:14:38.000000 fitsio-1.1.8/cfitsio3490/quantize.c
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)    55811 2021-03-26 15:14:38.000000 fitsio-1.1.8/cfitsio3490/region.c
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)     2157 2021-03-26 15:14:38.000000 fitsio-1.1.8/cfitsio3490/region.h
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)    35605 2021-03-26 15:14:38.000000 fitsio-1.1.8/cfitsio3490/ricecomp.c
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)     3581 2021-03-26 15:14:38.000000 fitsio-1.1.8/cfitsio3490/sample.tpl
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)     8973 2021-03-26 15:14:38.000000 fitsio-1.1.8/cfitsio3490/scalnull.c
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)    13925 2021-03-26 15:14:38.000000 fitsio-1.1.8/cfitsio3490/simplerng.c
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)     1078 2021-03-26 15:14:38.000000 fitsio-1.1.8/cfitsio3490/simplerng.h
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)     2564 2021-03-26 15:14:38.000000 fitsio-1.1.8/cfitsio3490/smem.c
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)    15459 2021-03-26 15:14:38.000000 fitsio-1.1.8/cfitsio3490/speed.c
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)     7703 2021-03-26 15:14:38.000000 fitsio-1.1.8/cfitsio3490/swapproc.c
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)    80140 2021-03-26 15:14:38.000000 fitsio-1.1.8/cfitsio3490/testf77.f
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)    33427 2021-03-26 15:14:38.000000 fitsio-1.1.8/cfitsio3490/testf77.out
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)    66240 2021-03-26 15:14:38.000000 fitsio-1.1.8/cfitsio3490/testf77.std
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)    85934 2021-03-26 15:14:38.000000 fitsio-1.1.8/cfitsio3490/testprog.c
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)    32223 2021-03-26 15:14:38.000000 fitsio-1.1.8/cfitsio3490/testprog.out
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)    69120 2021-03-26 15:14:38.000000 fitsio-1.1.8/cfitsio3490/testprog.std
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)      396 2021-03-26 15:14:38.000000 fitsio-1.1.8/cfitsio3490/testprog.tpt
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)     3782 2021-03-26 15:14:38.000000 fitsio-1.1.8/cfitsio3490/vmsieee.c
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)    35267 2021-03-26 15:14:38.000000 fitsio-1.1.8/cfitsio3490/wcssub.c
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)    16769 2021-03-26 15:14:38.000000 fitsio-1.1.8/cfitsio3490/wcsutil.c
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)     4257 2021-03-26 15:14:38.000000 fitsio-1.1.8/cfitsio3490/winDumpExts.mak
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)    13037 2021-03-26 15:14:38.000000 fitsio-1.1.8/cfitsio3490/windumpexts.c
-drwxrwxr-x   0 esheldon  (1000) esheldon  (1000)        0 2022-09-27 14:14:39.095974 fitsio-1.1.8/cfitsio3490/zlib/
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)     5031 2021-03-26 15:14:38.000000 fitsio-1.1.8/cfitsio3490/zlib/adler32.c
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)    13664 2021-03-26 15:14:38.000000 fitsio-1.1.8/cfitsio3490/zlib/crc32.c
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)    30568 2021-03-26 15:14:38.000000 fitsio-1.1.8/cfitsio3490/zlib/crc32.h
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)    67975 2021-03-26 15:14:38.000000 fitsio-1.1.8/cfitsio3490/zlib/deflate.c
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)    12655 2021-03-26 15:14:38.000000 fitsio-1.1.8/cfitsio3490/zlib/deflate.h
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)    22622 2021-03-26 15:14:38.000000 fitsio-1.1.8/cfitsio3490/zlib/infback.c
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)    13439 2021-03-26 15:14:38.000000 fitsio-1.1.8/cfitsio3490/zlib/inffast.c
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)      427 2021-03-26 15:14:38.000000 fitsio-1.1.8/cfitsio3490/zlib/inffast.h
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)     6343 2021-03-26 15:14:38.000000 fitsio-1.1.8/cfitsio3490/zlib/inffixed.h
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)    52623 2021-03-26 15:14:38.000000 fitsio-1.1.8/cfitsio3490/zlib/inflate.c
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)     6399 2021-03-26 15:14:38.000000 fitsio-1.1.8/cfitsio3490/zlib/inflate.h
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)    13769 2021-03-26 15:14:38.000000 fitsio-1.1.8/cfitsio3490/zlib/inftrees.c
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)     2928 2021-03-26 15:14:38.000000 fitsio-1.1.8/cfitsio3490/zlib/inftrees.h
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)    45225 2021-03-26 15:14:38.000000 fitsio-1.1.8/cfitsio3490/zlib/trees.c
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)     8472 2021-03-26 15:14:38.000000 fitsio-1.1.8/cfitsio3490/zlib/trees.h
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)     1977 2021-03-26 15:14:38.000000 fitsio-1.1.8/cfitsio3490/zlib/uncompr.c
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)    18946 2021-03-26 15:14:38.000000 fitsio-1.1.8/cfitsio3490/zlib/zcompress.c
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)    13353 2021-03-26 15:14:38.000000 fitsio-1.1.8/cfitsio3490/zlib/zconf.h
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)    79564 2021-03-26 15:14:38.000000 fitsio-1.1.8/cfitsio3490/zlib/zlib.h
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)    16425 2021-03-26 15:14:38.000000 fitsio-1.1.8/cfitsio3490/zlib/zuncompress.c
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)     7296 2021-03-26 15:14:38.000000 fitsio-1.1.8/cfitsio3490/zlib/zutil.c
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)     7136 2021-03-26 15:14:38.000000 fitsio-1.1.8/cfitsio3490/zlib/zutil.h
-drwxrwxr-x   0 esheldon  (1000) esheldon  (1000)        0 2022-09-27 14:14:39.095974 fitsio-1.1.8/fitsio/
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)      677 2022-09-26 18:17:11.000000 fitsio-1.1.8/fitsio/__init__.py
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)   141655 2022-06-23 13:51:45.000000 fitsio-1.1.8/fitsio/fitsio_pywrap.c
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)    64242 2022-09-26 18:00:17.000000 fitsio-1.1.8/fitsio/fitslib.py
-drwxrwxr-x   0 esheldon  (1000) esheldon  (1000)        0 2022-09-27 14:14:39.099974 fitsio-1.1.8/fitsio/hdu/
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)      231 2021-03-26 15:14:38.000000 fitsio-1.1.8/fitsio/hdu/__init__.py
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)    12577 2022-01-04 20:03:22.000000 fitsio-1.1.8/fitsio/hdu/base.py
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)    13716 2021-03-26 15:14:38.000000 fitsio-1.1.8/fitsio/hdu/image.py
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)    87747 2022-01-04 20:03:22.000000 fitsio-1.1.8/fitsio/hdu/table.py
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)    22366 2022-06-23 13:51:45.000000 fitsio-1.1.8/fitsio/header.py
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)   122971 2022-06-23 13:51:45.000000 fitsio-1.1.8/fitsio/test.py
-drwxrwxr-x   0 esheldon  (1000) esheldon  (1000)        0 2022-09-27 14:14:39.099974 fitsio-1.1.8/fitsio/test_images/
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)     8640 2021-03-26 15:14:38.000000 fitsio-1.1.8/fitsio/test_images/test_gzip_compressed_image.fits.fz
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)     3453 2021-03-26 15:14:38.000000 fitsio-1.1.8/fitsio/util.py
-drwxrwxr-x   0 esheldon  (1000) esheldon  (1000)        0 2022-09-27 14:14:39.095974 fitsio-1.1.8/fitsio.egg-info/
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)    15660 2022-09-27 14:14:38.000000 fitsio-1.1.8/fitsio.egg-info/PKG-INFO
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)     4738 2022-09-27 14:14:39.000000 fitsio-1.1.8/fitsio.egg-info/SOURCES.txt
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)        1 2022-09-27 14:14:38.000000 fitsio-1.1.8/fitsio.egg-info/dependency_links.txt
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)        6 2022-09-27 14:14:38.000000 fitsio-1.1.8/fitsio.egg-info/requires.txt
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)        7 2022-09-27 14:14:38.000000 fitsio-1.1.8/fitsio.egg-info/top_level.txt
-drwxrwxr-x   0 esheldon  (1000) esheldon  (1000)        0 2022-09-27 14:14:39.099974 fitsio-1.1.8/patches/
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)      893 2021-03-26 15:14:38.000000 fitsio-1.1.8/patches/README.md
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)     1013 2021-03-26 15:14:38.000000 fitsio-1.1.8/patches/build_cfitsio_patches.py
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)     1196 2021-03-26 15:14:38.000000 fitsio-1.1.8/patches/configure.in.patch
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)     1559 2021-03-26 15:14:38.000000 fitsio-1.1.8/patches/configure.patch
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)      360 2021-03-26 15:14:38.000000 fitsio-1.1.8/patches/drvrnet.c.patch
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)      636 2021-03-26 15:14:38.000000 fitsio-1.1.8/patches/fitscore.c.patch
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)      423 2021-03-26 15:14:38.000000 fitsio-1.1.8/patches/fitsio.h.patch
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)      602 2021-03-26 15:14:38.000000 fitsio-1.1.8/patches/putcols.c.patch
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)       38 2022-09-27 14:14:39.099974 fitsio-1.1.8/setup.cfg
--rw-rw-r--   0 esheldon  (1000) esheldon  (1000)     9873 2022-09-26 18:17:11.000000 fitsio-1.1.8/setup.py
+drwxrwxr-x   0 esheldon  (1000) esheldon  (1000)        0 2023-05-26 13:06:55.380537 fitsio-1.1.9/
+drwxrwxr-x   0 esheldon  (1000) esheldon  (1000)        0 2023-05-26 13:06:55.292539 fitsio-1.1.9/.github/
+drwxrwxr-x   0 esheldon  (1000) esheldon  (1000)        0 2023-05-26 13:06:55.296539 fitsio-1.1.9/.github/workflows/
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)     2162 2023-05-24 20:40:55.000000 fitsio-1.1.9/.github/workflows/tests.yml
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)     1306 2021-03-26 15:14:38.000000 fitsio-1.1.9/.gitignore
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)     2350 2021-03-26 15:14:38.000000 fitsio-1.1.9/.travis.yml
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)    26374 2023-05-26 13:05:13.000000 fitsio-1.1.9/CHANGES.md
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)    18011 2021-03-26 15:14:38.000000 fitsio-1.1.9/LICENSE.txt
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)      131 2021-03-26 15:14:38.000000 fitsio-1.1.9/MANIFEST.in
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)    15431 2023-05-26 13:06:55.380537 fitsio-1.1.9/PKG-INFO
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)    14850 2023-05-26 13:05:13.000000 fitsio-1.1.9/README.md
+drwxrwxr-x   0 esheldon  (1000) esheldon  (1000)        0 2023-05-26 13:06:55.340538 fitsio-1.1.9/cfitsio3490/
+-rwxrwxr-x   0 esheldon  (1000) esheldon  (1000)     6405 2021-03-26 15:14:38.000000 fitsio-1.1.9/cfitsio3490/CMakeLists.txt
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)     3209 2021-03-26 15:14:38.000000 fitsio-1.1.9/cfitsio3490/FindPthreads.cmake
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)     1410 2021-03-26 15:14:38.000000 fitsio-1.1.9/cfitsio3490/License.txt
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)     6236 2021-03-26 15:14:38.000000 fitsio-1.1.9/cfitsio3490/Makefile.in
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)     4528 2021-03-26 15:14:38.000000 fitsio-1.1.9/cfitsio3490/README
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)     2493 2021-03-26 15:14:38.000000 fitsio-1.1.9/cfitsio3490/README.MacOS
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)     6134 2021-03-26 15:14:38.000000 fitsio-1.1.9/cfitsio3490/README.win
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)     3534 2021-03-26 15:14:38.000000 fitsio-1.1.9/cfitsio3490/README_OLD.win
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)    53229 2021-03-26 15:14:38.000000 fitsio-1.1.9/cfitsio3490/buffers.c
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)   263595 2021-03-26 15:14:38.000000 fitsio-1.1.9/cfitsio3490/cfileio.c
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)      342 2021-03-26 15:14:38.000000 fitsio-1.1.9/cfitsio3490/cfitsio.pc.cmake
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)      300 2021-03-26 15:14:38.000000 fitsio-1.1.9/cfitsio3490/cfitsio.pc.in
+drwxrwxr-x   0 esheldon  (1000) esheldon  (1000)        0 2023-05-26 13:06:55.340538 fitsio-1.1.9/cfitsio3490/cfitsio.xcodeproj/
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)     3233 2021-03-26 15:14:38.000000 fitsio-1.1.9/cfitsio3490/cfitsio.xcodeproj/project.pbxproj
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)    23366 2021-03-26 15:14:38.000000 fitsio-1.1.9/cfitsio3490/cfitsio_mac.sit.hqx
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)   135706 2021-03-26 15:14:38.000000 fitsio-1.1.9/cfitsio3490/cfortran.h
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)    17601 2021-03-26 15:14:38.000000 fitsio-1.1.9/cfitsio3490/checksum.c
+-rwxrwxr-x   0 esheldon  (1000) esheldon  (1000)    44283 2021-03-26 15:14:38.000000 fitsio-1.1.9/cfitsio3490/config.guess
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)    23466 2021-09-07 13:51:31.000000 fitsio-1.1.9/cfitsio3490/config.log
+-rwxrwxr-x   0 esheldon  (1000) esheldon  (1000)    36136 2021-03-26 15:14:38.000000 fitsio-1.1.9/cfitsio3490/config.sub
+-rwxrwxr-x   0 esheldon  (1000) esheldon  (1000)   219087 2021-03-26 15:14:38.000000 fitsio-1.1.9/cfitsio3490/configure
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)    20705 2021-03-26 15:14:38.000000 fitsio-1.1.9/cfitsio3490/configure.in
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)    21858 2021-03-26 15:14:38.000000 fitsio-1.1.9/cfitsio3490/cookbook.c
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)    30203 2021-03-26 15:14:38.000000 fitsio-1.1.9/cfitsio3490/cookbook.f
+drwxrwxr-x   0 esheldon  (1000) esheldon  (1000)        0 2023-05-26 13:06:55.360538 fitsio-1.1.9/cfitsio3490/docs/
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)  1074054 2021-03-26 15:14:38.000000 fitsio-1.1.9/cfitsio3490/docs/cfitsio.pdf
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)  1412279 2021-03-26 15:14:38.000000 fitsio-1.1.9/cfitsio3490/docs/cfitsio.ps
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)   507182 2021-03-26 15:14:38.000000 fitsio-1.1.9/cfitsio3490/docs/cfitsio.tex
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)    11521 2021-03-26 15:14:38.000000 fitsio-1.1.9/cfitsio3490/docs/cfitsio.toc
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)    95483 2021-03-26 15:14:38.000000 fitsio-1.1.9/cfitsio3490/docs/cfortran.doc
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)   213622 2021-03-26 15:14:38.000000 fitsio-1.1.9/cfitsio3490/docs/changes.txt
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)   326397 2021-03-26 15:14:38.000000 fitsio-1.1.9/cfitsio3490/docs/fitsio.doc
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)   697014 2021-03-26 15:14:38.000000 fitsio-1.1.9/cfitsio3490/docs/fitsio.pdf
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)   958163 2021-03-26 15:14:38.000000 fitsio-1.1.9/cfitsio3490/docs/fitsio.ps
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)   346564 2021-03-26 15:14:38.000000 fitsio-1.1.9/cfitsio3490/docs/fitsio.tex
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)     8707 2021-03-26 15:14:38.000000 fitsio-1.1.9/cfitsio3490/docs/fitsio.toc
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)   588666 2021-03-26 15:14:38.000000 fitsio-1.1.9/cfitsio3490/docs/fpackguide.pdf
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)   232878 2021-03-26 15:14:38.000000 fitsio-1.1.9/cfitsio3490/docs/quick.pdf
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)   312357 2021-03-26 15:14:38.000000 fitsio-1.1.9/cfitsio3490/docs/quick.ps
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)   101448 2021-03-26 15:14:38.000000 fitsio-1.1.9/cfitsio3490/docs/quick.tex
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)     1795 2021-03-26 15:14:38.000000 fitsio-1.1.9/cfitsio3490/docs/quick.toc
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)    28508 2021-03-26 15:14:38.000000 fitsio-1.1.9/cfitsio3490/drvrfile.c
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)    13960 2021-03-26 15:14:38.000000 fitsio-1.1.9/cfitsio3490/drvrgsiftp.c
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)      787 2021-03-26 15:14:38.000000 fitsio-1.1.9/cfitsio3490/drvrgsiftp.h
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)    39553 2021-03-26 15:14:38.000000 fitsio-1.1.9/cfitsio3490/drvrmem.c
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)   125780 2021-03-26 15:14:38.000000 fitsio-1.1.9/cfitsio3490/drvrnet.c
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)    38489 2021-03-26 15:14:38.000000 fitsio-1.1.9/cfitsio3490/drvrsmem.c
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)     6536 2021-03-26 15:14:38.000000 fitsio-1.1.9/cfitsio3490/drvrsmem.h
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)   101807 2021-03-26 15:14:38.000000 fitsio-1.1.9/cfitsio3490/editcol.c
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)    32727 2021-03-26 15:14:38.000000 fitsio-1.1.9/cfitsio3490/edithdu.c
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)    16188 2021-03-26 15:14:38.000000 fitsio-1.1.9/cfitsio3490/eval.l
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)   177512 2021-03-26 15:14:38.000000 fitsio-1.1.9/cfitsio3490/eval.y
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)     4254 2021-03-26 15:14:38.000000 fitsio-1.1.9/cfitsio3490/eval_defs.h
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)    98802 2021-03-26 15:14:38.000000 fitsio-1.1.9/cfitsio3490/eval_f.c
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)    69666 2021-03-26 15:14:38.000000 fitsio-1.1.9/cfitsio3490/eval_l.c
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)     3564 2021-03-26 15:14:38.000000 fitsio-1.1.9/cfitsio3490/eval_tab.h
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)   275403 2021-03-26 15:14:38.000000 fitsio-1.1.9/cfitsio3490/eval_y.c
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)      853 2021-03-26 15:14:38.000000 fitsio-1.1.9/cfitsio3490/f77.inc
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)    10430 2021-03-26 15:14:38.000000 fitsio-1.1.9/cfitsio3490/f77_wrap.h
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)    12779 2021-03-26 15:14:38.000000 fitsio-1.1.9/cfitsio3490/f77_wrap1.c
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)    32385 2021-03-26 15:14:38.000000 fitsio-1.1.9/cfitsio3490/f77_wrap2.c
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)    33790 2021-03-26 15:14:38.000000 fitsio-1.1.9/cfitsio3490/f77_wrap3.c
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)    19467 2021-03-26 15:14:38.000000 fitsio-1.1.9/cfitsio3490/f77_wrap4.c
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)    47082 2021-03-26 15:14:38.000000 fitsio-1.1.9/cfitsio3490/fits_hcompress.c
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)    63312 2021-03-26 15:14:38.000000 fitsio-1.1.9/cfitsio3490/fits_hdecompress.c
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)     2642 2021-03-26 15:14:38.000000 fitsio-1.1.9/cfitsio3490/fitscopy.c
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)   318473 2021-03-26 15:14:38.000000 fitsio-1.1.9/cfitsio3490/fitscore.c
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)   119295 2021-03-26 15:14:38.000000 fitsio-1.1.9/cfitsio3490/fitsio.h
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)    63131 2021-03-26 15:14:38.000000 fitsio-1.1.9/cfitsio3490/fitsio2.h
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)    16825 2021-03-26 15:14:38.000000 fitsio-1.1.9/cfitsio3490/fpack.c
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)     7155 2021-03-26 15:14:38.000000 fitsio-1.1.9/cfitsio3490/fpack.h
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)    78403 2021-03-26 15:14:38.000000 fitsio-1.1.9/cfitsio3490/fpackutil.c
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)     4664 2021-03-26 15:14:38.000000 fitsio-1.1.9/cfitsio3490/funpack.c
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)    41542 2021-03-26 15:14:38.000000 fitsio-1.1.9/cfitsio3490/getcol.c
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)    78585 2021-03-26 15:14:38.000000 fitsio-1.1.9/cfitsio3490/getcolb.c
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)    68830 2021-03-26 15:14:38.000000 fitsio-1.1.9/cfitsio3490/getcold.c
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)    68940 2021-03-26 15:14:38.000000 fitsio-1.1.9/cfitsio3490/getcole.c
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)    74885 2021-03-26 15:14:38.000000 fitsio-1.1.9/cfitsio3490/getcoli.c
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)   148225 2021-03-26 15:14:38.000000 fitsio-1.1.9/cfitsio3490/getcolj.c
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)    74751 2021-03-26 15:14:38.000000 fitsio-1.1.9/cfitsio3490/getcolk.c
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)    23298 2021-03-26 15:14:38.000000 fitsio-1.1.9/cfitsio3490/getcoll.c
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)    33907 2021-03-26 15:14:38.000000 fitsio-1.1.9/cfitsio3490/getcols.c
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)    77347 2021-03-26 15:14:38.000000 fitsio-1.1.9/cfitsio3490/getcolsb.c
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)    75282 2021-03-26 15:14:38.000000 fitsio-1.1.9/cfitsio3490/getcolui.c
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)   148281 2021-03-26 15:14:38.000000 fitsio-1.1.9/cfitsio3490/getcoluj.c
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)    75493 2021-03-26 15:14:38.000000 fitsio-1.1.9/cfitsio3490/getcoluk.c
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)   125729 2021-03-26 15:14:38.000000 fitsio-1.1.9/cfitsio3490/getkey.c
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)   185566 2021-03-26 15:14:38.000000 fitsio-1.1.9/cfitsio3490/group.c
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)     2097 2021-03-26 15:14:38.000000 fitsio-1.1.9/cfitsio3490/group.h
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)    46325 2021-03-26 15:14:38.000000 fitsio-1.1.9/cfitsio3490/grparser.c
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)     5725 2021-03-26 15:14:38.000000 fitsio-1.1.9/cfitsio3490/grparser.h
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)    86820 2021-03-26 15:14:38.000000 fitsio-1.1.9/cfitsio3490/histo.c
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)   380829 2021-03-26 15:14:38.000000 fitsio-1.1.9/cfitsio3490/imcompress.c
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)     9368 2021-03-26 15:14:38.000000 fitsio-1.1.9/cfitsio3490/imcopy.c
+-rwxrwxr-x   0 esheldon  (1000) esheldon  (1000)    14799 2021-03-26 15:14:38.000000 fitsio-1.1.9/cfitsio3490/install-sh
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)    57777 2021-03-26 15:14:38.000000 fitsio-1.1.9/cfitsio3490/iraffits.c
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)     5253 2021-03-26 15:14:38.000000 fitsio-1.1.9/cfitsio3490/iter_a.c
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)     6874 2021-03-26 15:14:38.000000 fitsio-1.1.9/cfitsio3490/iter_a.f
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)   129600 2021-03-26 15:14:38.000000 fitsio-1.1.9/cfitsio3490/iter_a.fit
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)     3702 2021-03-26 15:14:38.000000 fitsio-1.1.9/cfitsio3490/iter_b.c
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)     5679 2021-03-26 15:14:38.000000 fitsio-1.1.9/cfitsio3490/iter_b.f
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)   408960 2021-03-26 15:14:38.000000 fitsio-1.1.9/cfitsio3490/iter_b.fit
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)     6007 2021-03-26 15:14:38.000000 fitsio-1.1.9/cfitsio3490/iter_c.c
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)    10525 2021-03-26 15:14:38.000000 fitsio-1.1.9/cfitsio3490/iter_c.f
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)    92160 2021-03-26 15:14:38.000000 fitsio-1.1.9/cfitsio3490/iter_c.fit
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)     3076 2021-03-26 15:14:38.000000 fitsio-1.1.9/cfitsio3490/iter_image.c
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)     3319 2021-03-26 15:14:38.000000 fitsio-1.1.9/cfitsio3490/iter_var.c
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)    21784 2021-03-26 15:14:38.000000 fitsio-1.1.9/cfitsio3490/longnam.h
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)    12754 2021-03-26 15:14:38.000000 fitsio-1.1.9/cfitsio3490/makefile.bc
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)    18040 2021-03-26 15:14:38.000000 fitsio-1.1.9/cfitsio3490/makefile.vcc
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)     2307 2021-03-26 15:14:38.000000 fitsio-1.1.9/cfitsio3490/makepc.bat
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)    67233 2021-03-26 15:14:38.000000 fitsio-1.1.9/cfitsio3490/modkey.c
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)     7067 2021-03-26 15:14:38.000000 fitsio-1.1.9/cfitsio3490/pliocomp.c
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)    67801 2021-03-26 15:14:38.000000 fitsio-1.1.9/cfitsio3490/putcol.c
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)    37199 2021-03-26 15:14:38.000000 fitsio-1.1.9/cfitsio3490/putcolb.c
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)    38722 2021-03-26 15:14:38.000000 fitsio-1.1.9/cfitsio3490/putcold.c
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)    39292 2021-03-26 15:14:38.000000 fitsio-1.1.9/cfitsio3490/putcole.c
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)    35439 2021-03-26 15:14:38.000000 fitsio-1.1.9/cfitsio3490/putcoli.c
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)    71429 2021-03-26 15:14:38.000000 fitsio-1.1.9/cfitsio3490/putcolj.c
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)    36390 2021-03-26 15:14:38.000000 fitsio-1.1.9/cfitsio3490/putcolk.c
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)    13933 2021-03-26 15:14:38.000000 fitsio-1.1.9/cfitsio3490/putcoll.c
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)    10944 2021-03-26 15:14:38.000000 fitsio-1.1.9/cfitsio3490/putcols.c
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)    35466 2021-03-26 15:14:38.000000 fitsio-1.1.9/cfitsio3490/putcolsb.c
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)    21555 2021-03-26 15:14:38.000000 fitsio-1.1.9/cfitsio3490/putcolu.c
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)    34837 2021-03-26 15:14:38.000000 fitsio-1.1.9/cfitsio3490/putcolui.c
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)    69378 2021-03-26 15:14:38.000000 fitsio-1.1.9/cfitsio3490/putcoluj.c
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)    35653 2021-03-26 15:14:38.000000 fitsio-1.1.9/cfitsio3490/putcoluk.c
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)   115057 2021-03-26 15:14:38.000000 fitsio-1.1.9/cfitsio3490/putkey.c
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)   118985 2021-03-26 15:14:38.000000 fitsio-1.1.9/cfitsio3490/quantize.c
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)    55811 2021-03-26 15:14:38.000000 fitsio-1.1.9/cfitsio3490/region.c
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)     2157 2021-03-26 15:14:38.000000 fitsio-1.1.9/cfitsio3490/region.h
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)    35605 2021-03-26 15:14:38.000000 fitsio-1.1.9/cfitsio3490/ricecomp.c
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)     3581 2021-03-26 15:14:38.000000 fitsio-1.1.9/cfitsio3490/sample.tpl
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)     8973 2021-03-26 15:14:38.000000 fitsio-1.1.9/cfitsio3490/scalnull.c
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)    13925 2021-03-26 15:14:38.000000 fitsio-1.1.9/cfitsio3490/simplerng.c
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)     1078 2021-03-26 15:14:38.000000 fitsio-1.1.9/cfitsio3490/simplerng.h
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)     2564 2021-03-26 15:14:38.000000 fitsio-1.1.9/cfitsio3490/smem.c
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)    15459 2021-03-26 15:14:38.000000 fitsio-1.1.9/cfitsio3490/speed.c
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)     7703 2021-03-26 15:14:38.000000 fitsio-1.1.9/cfitsio3490/swapproc.c
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)    80140 2021-03-26 15:14:38.000000 fitsio-1.1.9/cfitsio3490/testf77.f
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)    33427 2021-03-26 15:14:38.000000 fitsio-1.1.9/cfitsio3490/testf77.out
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)    66240 2021-03-26 15:14:38.000000 fitsio-1.1.9/cfitsio3490/testf77.std
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)    85934 2021-03-26 15:14:38.000000 fitsio-1.1.9/cfitsio3490/testprog.c
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)    32223 2021-03-26 15:14:38.000000 fitsio-1.1.9/cfitsio3490/testprog.out
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)    69120 2021-03-26 15:14:38.000000 fitsio-1.1.9/cfitsio3490/testprog.std
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)      396 2021-03-26 15:14:38.000000 fitsio-1.1.9/cfitsio3490/testprog.tpt
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)     3782 2021-03-26 15:14:38.000000 fitsio-1.1.9/cfitsio3490/vmsieee.c
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)    35267 2021-03-26 15:14:38.000000 fitsio-1.1.9/cfitsio3490/wcssub.c
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)    16769 2021-03-26 15:14:38.000000 fitsio-1.1.9/cfitsio3490/wcsutil.c
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)     4257 2021-03-26 15:14:38.000000 fitsio-1.1.9/cfitsio3490/winDumpExts.mak
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)    13037 2021-03-26 15:14:38.000000 fitsio-1.1.9/cfitsio3490/windumpexts.c
+drwxrwxr-x   0 esheldon  (1000) esheldon  (1000)        0 2023-05-26 13:06:55.368538 fitsio-1.1.9/cfitsio3490/zlib/
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)     5031 2021-03-26 15:14:38.000000 fitsio-1.1.9/cfitsio3490/zlib/adler32.c
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)    13664 2021-03-26 15:14:38.000000 fitsio-1.1.9/cfitsio3490/zlib/crc32.c
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)    30568 2021-03-26 15:14:38.000000 fitsio-1.1.9/cfitsio3490/zlib/crc32.h
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)    67975 2021-03-26 15:14:38.000000 fitsio-1.1.9/cfitsio3490/zlib/deflate.c
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)    12655 2021-03-26 15:14:38.000000 fitsio-1.1.9/cfitsio3490/zlib/deflate.h
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)    22622 2021-03-26 15:14:38.000000 fitsio-1.1.9/cfitsio3490/zlib/infback.c
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)    13439 2021-03-26 15:14:38.000000 fitsio-1.1.9/cfitsio3490/zlib/inffast.c
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)      427 2021-03-26 15:14:38.000000 fitsio-1.1.9/cfitsio3490/zlib/inffast.h
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)     6343 2021-03-26 15:14:38.000000 fitsio-1.1.9/cfitsio3490/zlib/inffixed.h
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)    52623 2021-03-26 15:14:38.000000 fitsio-1.1.9/cfitsio3490/zlib/inflate.c
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)     6399 2021-03-26 15:14:38.000000 fitsio-1.1.9/cfitsio3490/zlib/inflate.h
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)    13769 2021-03-26 15:14:38.000000 fitsio-1.1.9/cfitsio3490/zlib/inftrees.c
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)     2928 2021-03-26 15:14:38.000000 fitsio-1.1.9/cfitsio3490/zlib/inftrees.h
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)    45225 2021-03-26 15:14:38.000000 fitsio-1.1.9/cfitsio3490/zlib/trees.c
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)     8472 2021-03-26 15:14:38.000000 fitsio-1.1.9/cfitsio3490/zlib/trees.h
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)     1977 2021-03-26 15:14:38.000000 fitsio-1.1.9/cfitsio3490/zlib/uncompr.c
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)    18946 2021-03-26 15:14:38.000000 fitsio-1.1.9/cfitsio3490/zlib/zcompress.c
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)    13353 2021-03-26 15:14:38.000000 fitsio-1.1.9/cfitsio3490/zlib/zconf.h
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)    79564 2021-03-26 15:14:38.000000 fitsio-1.1.9/cfitsio3490/zlib/zlib.h
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)    16425 2021-03-26 15:14:38.000000 fitsio-1.1.9/cfitsio3490/zlib/zuncompress.c
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)     7296 2021-03-26 15:14:38.000000 fitsio-1.1.9/cfitsio3490/zlib/zutil.c
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)     7136 2021-03-26 15:14:38.000000 fitsio-1.1.9/cfitsio3490/zlib/zutil.h
+drwxrwxr-x   0 esheldon  (1000) esheldon  (1000)        0 2023-05-26 13:06:55.372537 fitsio-1.1.9/fitsio/
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)      657 2023-05-24 20:40:55.000000 fitsio-1.1.9/fitsio/__init__.py
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)   143281 2023-05-26 13:05:13.000000 fitsio-1.1.9/fitsio/fitsio_pywrap.c
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)    64242 2022-09-26 18:00:17.000000 fitsio-1.1.9/fitsio/fitslib.py
+drwxrwxr-x   0 esheldon  (1000) esheldon  (1000)        0 2023-05-26 13:06:55.372537 fitsio-1.1.9/fitsio/hdu/
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)      231 2021-03-26 15:14:38.000000 fitsio-1.1.9/fitsio/hdu/__init__.py
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)    12577 2022-01-04 20:03:22.000000 fitsio-1.1.9/fitsio/hdu/base.py
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)    13716 2021-03-26 15:14:38.000000 fitsio-1.1.9/fitsio/hdu/image.py
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)    89144 2023-05-26 13:05:13.000000 fitsio-1.1.9/fitsio/hdu/table.py
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)    22366 2022-06-23 13:51:45.000000 fitsio-1.1.9/fitsio/header.py
+drwxrwxr-x   0 esheldon  (1000) esheldon  (1000)        0 2023-05-26 13:06:55.372537 fitsio-1.1.9/fitsio/test_images/
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)     8640 2021-03-26 15:14:38.000000 fitsio-1.1.9/fitsio/test_images/test_gzip_compressed_image.fits.fz
+drwxrwxr-x   0 esheldon  (1000) esheldon  (1000)        0 2023-05-26 13:06:55.376537 fitsio-1.1.9/fitsio/tests/
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)        0 2023-05-24 20:40:55.000000 fitsio-1.1.9/fitsio/tests/__init__.py
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)     6155 2023-05-25 01:08:32.000000 fitsio-1.1.9/fitsio/tests/checks.py
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)    11820 2023-05-24 20:40:55.000000 fitsio-1.1.9/fitsio/tests/makedata.py
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)    18789 2023-05-24 20:40:55.000000 fitsio-1.1.9/fitsio/tests/test_header.py
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)     7248 2023-05-24 20:40:55.000000 fitsio-1.1.9/fitsio/tests/test_header_junk.py
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)     8768 2023-05-24 20:40:55.000000 fitsio-1.1.9/fitsio/tests/test_image.py
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)     4220 2023-05-24 20:40:55.000000 fitsio-1.1.9/fitsio/tests/test_image_compression.py
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)     3638 2023-05-24 20:40:55.000000 fitsio-1.1.9/fitsio/tests/test_lib.py
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)    42339 2023-05-26 13:05:13.000000 fitsio-1.1.9/fitsio/tests/test_table.py
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)     1234 2023-05-24 20:40:55.000000 fitsio-1.1.9/fitsio/tests/test_warnings.py
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)     3453 2023-05-23 19:28:37.000000 fitsio-1.1.9/fitsio/util.py
+drwxrwxr-x   0 esheldon  (1000) esheldon  (1000)        0 2023-05-26 13:06:55.372537 fitsio-1.1.9/fitsio.egg-info/
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)    15431 2023-05-26 13:06:55.000000 fitsio-1.1.9/fitsio.egg-info/PKG-INFO
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)     5101 2023-05-26 13:06:55.000000 fitsio-1.1.9/fitsio.egg-info/SOURCES.txt
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)        1 2023-05-26 13:06:55.000000 fitsio-1.1.9/fitsio.egg-info/dependency_links.txt
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)        6 2023-05-26 13:06:55.000000 fitsio-1.1.9/fitsio.egg-info/requires.txt
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)        7 2023-05-26 13:06:55.000000 fitsio-1.1.9/fitsio.egg-info/top_level.txt
+drwxrwxr-x   0 esheldon  (1000) esheldon  (1000)        0 2023-05-26 13:06:55.376537 fitsio-1.1.9/patches/
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)      893 2021-03-26 15:14:38.000000 fitsio-1.1.9/patches/README.md
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)      984 2023-05-24 20:40:55.000000 fitsio-1.1.9/patches/build_cfitsio_patches.py
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)     1013 2021-03-26 15:14:38.000000 fitsio-1.1.9/patches/build_cfitsio_patches.py~
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)     1196 2021-03-26 15:14:38.000000 fitsio-1.1.9/patches/configure.in.patch
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)     1559 2021-03-26 15:14:38.000000 fitsio-1.1.9/patches/configure.patch
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)      360 2021-03-26 15:14:38.000000 fitsio-1.1.9/patches/drvrnet.c.patch
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)      636 2021-03-26 15:14:38.000000 fitsio-1.1.9/patches/fitscore.c.patch
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)      423 2021-03-26 15:14:38.000000 fitsio-1.1.9/patches/fitsio.h.patch
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)      602 2021-03-26 15:14:38.000000 fitsio-1.1.9/patches/putcols.c.patch
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)       38 2023-05-26 13:06:55.380537 fitsio-1.1.9/setup.cfg
+-rw-rw-r--   0 esheldon  (1000) esheldon  (1000)     9873 2023-05-24 20:40:55.000000 fitsio-1.1.9/setup.py
```

### Comparing `fitsio-1.1.8/LICENSE.txt` & `fitsio-1.1.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fitsio-1.1.8/PKG-INFO` & `fitsio-1.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: fitsio
-Version: 1.1.8
+Version: 1.1.9
 Summary: A full featured python library to read from and write to FITS files.
 Home-page: https://github.com/esheldon/fitsio
 Author: Erin Scott Sheldon
 Author-email: erin.sheldon@gmail.com
 License: GPL
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: Intended Audience :: Science/Research
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 License-File: LICENSE.txt
 
@@ -83,19 +82,14 @@
 
 # Write an image to the same file. By default a new extension is
 # added to the file.  use clobber=True to overwrite an existing file
 # instead.  To append rows to an existing table, see below.
 
 fitsio.write(filename, image)
 
-# NOTE when reading row subsets, the data must still be read from disk.
-# This is most efficient if the data are read in the order they appear in
-# the file.  For this reason, the rows are always returned in row-sorted
-# order.
-
 #
 # the FITS class gives the you the ability to explore the data, and gives
 # more control
 #
 
 # open a FITS file for reading and explore
 fits=fitsio.FITS('data.fits')
@@ -190,18 +184,22 @@
 # all rows of column 'x'
 data = fits[1]['x'][:]
 
 # Read a few columns at once. This is more efficient than separate read for
 # each column
 data = fits[1]['x','y'][:]
 
-# General column and row subsets.  As noted above, the data are returned
-# in row sorted order for efficiency reasons.
+# General column and row subsets.
 columns=['index','x','y']
-rows=[1,5]
+rows = [1, 5]
+data = fits[1][columns][rows]
+
+# data are returned in the order requested by the user
+# and duplicates are preserved
+rows = [2, 2, 5]
 data = fits[1][columns][rows]
 
 # iterate over rows in a table hdu
 # faster if we buffer some rows, let's buffer 1000 at a time
 fits=fitsio.FITS(filename,iter_row_buffer=1000)
 for row in fits[1]:
     print(row)
@@ -441,15 +439,15 @@
 
 
 ## Tests
 
 The unit tests should all pass for full support.
 
 ```bash
-python -c "import fitsio; fitsio.test.test()"
+pytest fitsio
 ```
 
 Some tests may fail if certain libraries are not available, such
 as bzip2.  This failure only implies that bzipped files cannot
 be read, without affecting other functionality.
 
 ## Notes on Usage and Features
@@ -485,9 +483,7 @@
 in Python 3 will now come back as a string and not a byte string. Note that this
 support is not the same as full unicode support. Internally, fitsio only supports
 the ASCII character set.
 
 ## TODO
 
 - HDU groups: does anyone use these? If so open an issue!
-
-
```

### Comparing `fitsio-1.1.8/README.md` & `fitsio-1.1.9/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -67,19 +67,14 @@
 
 # Write an image to the same file. By default a new extension is
 # added to the file.  use clobber=True to overwrite an existing file
 # instead.  To append rows to an existing table, see below.
 
 fitsio.write(filename, image)
 
-# NOTE when reading row subsets, the data must still be read from disk.
-# This is most efficient if the data are read in the order they appear in
-# the file.  For this reason, the rows are always returned in row-sorted
-# order.
-
 #
 # the FITS class gives the you the ability to explore the data, and gives
 # more control
 #
 
 # open a FITS file for reading and explore
 fits=fitsio.FITS('data.fits')
@@ -174,18 +169,22 @@
 # all rows of column 'x'
 data = fits[1]['x'][:]
 
 # Read a few columns at once. This is more efficient than separate read for
 # each column
 data = fits[1]['x','y'][:]
 
-# General column and row subsets.  As noted above, the data are returned
-# in row sorted order for efficiency reasons.
+# General column and row subsets.
 columns=['index','x','y']
-rows=[1,5]
+rows = [1, 5]
+data = fits[1][columns][rows]
+
+# data are returned in the order requested by the user
+# and duplicates are preserved
+rows = [2, 2, 5]
 data = fits[1][columns][rows]
 
 # iterate over rows in a table hdu
 # faster if we buffer some rows, let's buffer 1000 at a time
 fits=fitsio.FITS(filename,iter_row_buffer=1000)
 for row in fits[1]:
     print(row)
@@ -425,15 +424,15 @@
 
 
 ## Tests
 
 The unit tests should all pass for full support.
 
 ```bash
-python -c "import fitsio; fitsio.test.test()"
+pytest fitsio
 ```
 
 Some tests may fail if certain libraries are not available, such
 as bzip2.  This failure only implies that bzipped files cannot
 be read, without affecting other functionality.
 
 ## Notes on Usage and Features
```

### Comparing `fitsio-1.1.8/cfitsio3490/CMakeLists.txt` & `fitsio-1.1.9/cfitsio3490/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `fitsio-1.1.8/cfitsio3490/FindPthreads.cmake` & `fitsio-1.1.9/cfitsio3490/FindPthreads.cmake`

 * *Files identical despite different names*

### Comparing `fitsio-1.1.8/cfitsio3490/License.txt` & `fitsio-1.1.9/cfitsio3490/License.txt`

 * *Files identical despite different names*

### Comparing `fitsio-1.1.8/cfitsio3490/Makefile.in` & `fitsio-1.1.9/cfitsio3490/Makefile.in`

 * *Files identical despite different names*

### Comparing `fitsio-1.1.8/cfitsio3490/README` & `fitsio-1.1.9/cfitsio3490/README`

 * *Files identical despite different names*

### Comparing `fitsio-1.1.8/cfitsio3490/README.MacOS` & `fitsio-1.1.9/cfitsio3490/README.MacOS`

 * *Files identical despite different names*

### Comparing `fitsio-1.1.8/cfitsio3490/README.win` & `fitsio-1.1.9/cfitsio3490/README.win`

 * *Files identical despite different names*

### Comparing `fitsio-1.1.8/cfitsio3490/README_OLD.win` & `fitsio-1.1.9/cfitsio3490/README_OLD.win`

 * *Files identical despite different names*

### Comparing `fitsio-1.1.8/cfitsio3490/buffers.c` & `fitsio-1.1.9/cfitsio3490/buffers.c`

 * *Files identical despite different names*

### Comparing `fitsio-1.1.8/cfitsio3490/cfileio.c` & `fitsio-1.1.9/cfitsio3490/cfileio.c`

 * *Files identical despite different names*

### Comparing `fitsio-1.1.8/cfitsio3490/cfitsio.xcodeproj/project.pbxproj` & `fitsio-1.1.9/cfitsio3490/cfitsio.xcodeproj/project.pbxproj`

 * *Files identical despite different names*

### Comparing `fitsio-1.1.8/cfitsio3490/cfitsio_mac.sit.hqx` & `fitsio-1.1.9/cfitsio3490/cfitsio_mac.sit.hqx`

 * *Files identical despite different names*

### Comparing `fitsio-1.1.8/cfitsio3490/cfortran.h` & `fitsio-1.1.9/cfitsio3490/cfortran.h`

 * *Files identical despite different names*

### Comparing `fitsio-1.1.8/cfitsio3490/checksum.c` & `fitsio-1.1.9/cfitsio3490/checksum.c`

 * *Files identical despite different names*

### Comparing `fitsio-1.1.8/cfitsio3490/config.guess` & `fitsio-1.1.9/cfitsio3490/config.guess`

 * *Files identical despite different names*

### Comparing `fitsio-1.1.8/cfitsio3490/config.log` & `fitsio-1.1.9/cfitsio3490/config.log`

 * *Files identical despite different names*

### Comparing `fitsio-1.1.8/cfitsio3490/config.sub` & `fitsio-1.1.9/cfitsio3490/config.sub`

 * *Files identical despite different names*

### Comparing `fitsio-1.1.8/cfitsio3490/configure` & `fitsio-1.1.9/cfitsio3490/configure`

 * *Files identical despite different names*

### Comparing `fitsio-1.1.8/cfitsio3490/configure.in` & `fitsio-1.1.9/cfitsio3490/configure.in`

 * *Files identical despite different names*

### Comparing `fitsio-1.1.8/cfitsio3490/cookbook.c` & `fitsio-1.1.9/cfitsio3490/cookbook.c`

 * *Files identical despite different names*

### Comparing `fitsio-1.1.8/cfitsio3490/cookbook.f` & `fitsio-1.1.9/cfitsio3490/cookbook.f`

 * *Files identical despite different names*

### Comparing `fitsio-1.1.8/cfitsio3490/docs/cfitsio.pdf` & `fitsio-1.1.9/cfitsio3490/docs/cfitsio.pdf`

 * *Files identical despite different names*

### Comparing `fitsio-1.1.8/cfitsio3490/docs/cfitsio.ps` & `fitsio-1.1.9/cfitsio3490/docs/cfitsio.ps`

 * *Files identical despite different names*

### Comparing `fitsio-1.1.8/cfitsio3490/docs/cfitsio.tex` & `fitsio-1.1.9/cfitsio3490/docs/cfitsio.tex`

 * *Files identical despite different names*

### Comparing `fitsio-1.1.8/cfitsio3490/docs/cfitsio.toc` & `fitsio-1.1.9/cfitsio3490/docs/cfitsio.toc`

 * *Files identical despite different names*

### Comparing `fitsio-1.1.8/cfitsio3490/docs/cfortran.doc` & `fitsio-1.1.9/cfitsio3490/docs/cfortran.doc`

 * *Files identical despite different names*

### Comparing `fitsio-1.1.8/cfitsio3490/docs/changes.txt` & `fitsio-1.1.9/cfitsio3490/docs/changes.txt`

 * *Files identical despite different names*

### Comparing `fitsio-1.1.8/cfitsio3490/docs/fitsio.doc` & `fitsio-1.1.9/cfitsio3490/docs/fitsio.doc`

 * *Files identical despite different names*

### Comparing `fitsio-1.1.8/cfitsio3490/docs/fitsio.pdf` & `fitsio-1.1.9/cfitsio3490/docs/fitsio.pdf`

 * *Files identical despite different names*

### Comparing `fitsio-1.1.8/cfitsio3490/docs/fitsio.ps` & `fitsio-1.1.9/cfitsio3490/docs/fitsio.ps`

 * *Files identical despite different names*

### Comparing `fitsio-1.1.8/cfitsio3490/docs/fitsio.tex` & `fitsio-1.1.9/cfitsio3490/docs/fitsio.tex`

 * *Files identical despite different names*

### Comparing `fitsio-1.1.8/cfitsio3490/docs/fitsio.toc` & `fitsio-1.1.9/cfitsio3490/docs/fitsio.toc`

 * *Files identical despite different names*

### Comparing `fitsio-1.1.8/cfitsio3490/docs/fpackguide.pdf` & `fitsio-1.1.9/cfitsio3490/docs/fpackguide.pdf`

 * *Files identical despite different names*

### Comparing `fitsio-1.1.8/cfitsio3490/docs/quick.pdf` & `fitsio-1.1.9/cfitsio3490/docs/quick.pdf`

 * *Files identical despite different names*

### Comparing `fitsio-1.1.8/cfitsio3490/docs/quick.ps` & `fitsio-1.1.9/cfitsio3490/docs/quick.ps`

 * *Files identical despite different names*

### Comparing `fitsio-1.1.8/cfitsio3490/docs/quick.tex` & `fitsio-1.1.9/cfitsio3490/docs/quick.tex`

 * *Files identical despite different names*

### Comparing `fitsio-1.1.8/cfitsio3490/docs/quick.toc` & `fitsio-1.1.9/cfitsio3490/docs/quick.toc`

 * *Files identical despite different names*

### Comparing `fitsio-1.1.8/cfitsio3490/drvrfile.c` & `fitsio-1.1.9/cfitsio3490/drvrfile.c`

 * *Files identical despite different names*

### Comparing `fitsio-1.1.8/cfitsio3490/drvrgsiftp.c` & `fitsio-1.1.9/cfitsio3490/drvrgsiftp.c`

 * *Files identical despite different names*

### Comparing `fitsio-1.1.8/cfitsio3490/drvrgsiftp.h` & `fitsio-1.1.9/cfitsio3490/drvrgsiftp.h`

 * *Files identical despite different names*

### Comparing `fitsio-1.1.8/cfitsio3490/drvrmem.c` & `fitsio-1.1.9/cfitsio3490/drvrmem.c`

 * *Files identical despite different names*

### Comparing `fitsio-1.1.8/cfitsio3490/drvrnet.c` & `fitsio-1.1.9/cfitsio3490/drvrnet.c`

 * *Files identical despite different names*

### Comparing `fitsio-1.1.8/cfitsio3490/drvrsmem.c` & `fitsio-1.1.9/cfitsio3490/drvrsmem.c`

 * *Files identical despite different names*

### Comparing `fitsio-1.1.8/cfitsio3490/drvrsmem.h` & `fitsio-1.1.9/cfitsio3490/drvrsmem.h`

 * *Files identical despite different names*

### Comparing `fitsio-1.1.8/cfitsio3490/editcol.c` & `fitsio-1.1.9/cfitsio3490/editcol.c`

 * *Files identical despite different names*

### Comparing `fitsio-1.1.8/cfitsio3490/edithdu.c` & `fitsio-1.1.9/cfitsio3490/edithdu.c`

 * *Files identical despite different names*

### Comparing `fitsio-1.1.8/cfitsio3490/eval.l` & `fitsio-1.1.9/cfitsio3490/eval.l`

 * *Files identical despite different names*

### Comparing `fitsio-1.1.8/cfitsio3490/eval.y` & `fitsio-1.1.9/cfitsio3490/eval.y`

 * *Files identical despite different names*

### Comparing `fitsio-1.1.8/cfitsio3490/eval_defs.h` & `fitsio-1.1.9/cfitsio3490/eval_defs.h`

 * *Files identical despite different names*

### Comparing `fitsio-1.1.8/cfitsio3490/eval_f.c` & `fitsio-1.1.9/cfitsio3490/eval_f.c`

 * *Files identical despite different names*

### Comparing `fitsio-1.1.8/cfitsio3490/eval_l.c` & `fitsio-1.1.9/cfitsio3490/eval_l.c`

 * *Files identical despite different names*

### Comparing `fitsio-1.1.8/cfitsio3490/eval_tab.h` & `fitsio-1.1.9/cfitsio3490/eval_tab.h`

 * *Files identical despite different names*

### Comparing `fitsio-1.1.8/cfitsio3490/eval_y.c` & `fitsio-1.1.9/cfitsio3490/eval_y.c`

 * *Files identical despite different names*

### Comparing `fitsio-1.1.8/cfitsio3490/f77.inc` & `fitsio-1.1.9/cfitsio3490/f77.inc`

 * *Files identical despite different names*

### Comparing `fitsio-1.1.8/cfitsio3490/f77_wrap.h` & `fitsio-1.1.9/cfitsio3490/f77_wrap.h`

 * *Files identical despite different names*

### Comparing `fitsio-1.1.8/cfitsio3490/f77_wrap1.c` & `fitsio-1.1.9/cfitsio3490/f77_wrap1.c`

 * *Files identical despite different names*

### Comparing `fitsio-1.1.8/cfitsio3490/f77_wrap2.c` & `fitsio-1.1.9/cfitsio3490/f77_wrap2.c`

 * *Files identical despite different names*

### Comparing `fitsio-1.1.8/cfitsio3490/f77_wrap3.c` & `fitsio-1.1.9/cfitsio3490/f77_wrap3.c`

 * *Files identical despite different names*

### Comparing `fitsio-1.1.8/cfitsio3490/f77_wrap4.c` & `fitsio-1.1.9/cfitsio3490/f77_wrap4.c`

 * *Files identical despite different names*

### Comparing `fitsio-1.1.8/cfitsio3490/fits_hcompress.c` & `fitsio-1.1.9/cfitsio3490/fits_hcompress.c`

 * *Files identical despite different names*

### Comparing `fitsio-1.1.8/cfitsio3490/fits_hdecompress.c` & `fitsio-1.1.9/cfitsio3490/fits_hdecompress.c`

 * *Files identical despite different names*

### Comparing `fitsio-1.1.8/cfitsio3490/fitscopy.c` & `fitsio-1.1.9/cfitsio3490/fitscopy.c`

 * *Files identical despite different names*

### Comparing `fitsio-1.1.8/cfitsio3490/fitscore.c` & `fitsio-1.1.9/cfitsio3490/fitscore.c`

 * *Files identical despite different names*

### Comparing `fitsio-1.1.8/cfitsio3490/fitsio.h` & `fitsio-1.1.9/cfitsio3490/fitsio.h`

 * *Files identical despite different names*

### Comparing `fitsio-1.1.8/cfitsio3490/fitsio2.h` & `fitsio-1.1.9/cfitsio3490/fitsio2.h`

 * *Files identical despite different names*

### Comparing `fitsio-1.1.8/cfitsio3490/fpack.c` & `fitsio-1.1.9/cfitsio3490/fpack.c`

 * *Files identical despite different names*

### Comparing `fitsio-1.1.8/cfitsio3490/fpack.h` & `fitsio-1.1.9/cfitsio3490/fpack.h`

 * *Files identical despite different names*

### Comparing `fitsio-1.1.8/cfitsio3490/fpackutil.c` & `fitsio-1.1.9/cfitsio3490/fpackutil.c`

 * *Files identical despite different names*

### Comparing `fitsio-1.1.8/cfitsio3490/funpack.c` & `fitsio-1.1.9/cfitsio3490/funpack.c`

 * *Files identical despite different names*

### Comparing `fitsio-1.1.8/cfitsio3490/getcol.c` & `fitsio-1.1.9/cfitsio3490/getcol.c`

 * *Files identical despite different names*

### Comparing `fitsio-1.1.8/cfitsio3490/getcolb.c` & `fitsio-1.1.9/cfitsio3490/getcolb.c`

 * *Files identical despite different names*

### Comparing `fitsio-1.1.8/cfitsio3490/getcold.c` & `fitsio-1.1.9/cfitsio3490/getcold.c`

 * *Files identical despite different names*

### Comparing `fitsio-1.1.8/cfitsio3490/getcole.c` & `fitsio-1.1.9/cfitsio3490/getcole.c`

 * *Files identical despite different names*

### Comparing `fitsio-1.1.8/cfitsio3490/getcoli.c` & `fitsio-1.1.9/cfitsio3490/getcoli.c`

 * *Files identical despite different names*

### Comparing `fitsio-1.1.8/cfitsio3490/getcolj.c` & `fitsio-1.1.9/cfitsio3490/getcolj.c`

 * *Files identical despite different names*

### Comparing `fitsio-1.1.8/cfitsio3490/getcolk.c` & `fitsio-1.1.9/cfitsio3490/getcolk.c`

 * *Files identical despite different names*

### Comparing `fitsio-1.1.8/cfitsio3490/getcoll.c` & `fitsio-1.1.9/cfitsio3490/getcoll.c`

 * *Files identical despite different names*

### Comparing `fitsio-1.1.8/cfitsio3490/getcols.c` & `fitsio-1.1.9/cfitsio3490/getcols.c`

 * *Files identical despite different names*

### Comparing `fitsio-1.1.8/cfitsio3490/getcolsb.c` & `fitsio-1.1.9/cfitsio3490/getcolsb.c`

 * *Files identical despite different names*

### Comparing `fitsio-1.1.8/cfitsio3490/getcolui.c` & `fitsio-1.1.9/cfitsio3490/getcolui.c`

 * *Files identical despite different names*

### Comparing `fitsio-1.1.8/cfitsio3490/getcoluj.c` & `fitsio-1.1.9/cfitsio3490/getcoluj.c`

 * *Files identical despite different names*

### Comparing `fitsio-1.1.8/cfitsio3490/getcoluk.c` & `fitsio-1.1.9/cfitsio3490/getcoluk.c`

 * *Files identical despite different names*

### Comparing `fitsio-1.1.8/cfitsio3490/getkey.c` & `fitsio-1.1.9/cfitsio3490/getkey.c`

 * *Files identical despite different names*

### Comparing `fitsio-1.1.8/cfitsio3490/group.c` & `fitsio-1.1.9/cfitsio3490/group.c`

 * *Files identical despite different names*

### Comparing `fitsio-1.1.8/cfitsio3490/group.h` & `fitsio-1.1.9/cfitsio3490/group.h`

 * *Files identical despite different names*

### Comparing `fitsio-1.1.8/cfitsio3490/grparser.c` & `fitsio-1.1.9/cfitsio3490/grparser.c`

 * *Files identical despite different names*

### Comparing `fitsio-1.1.8/cfitsio3490/grparser.h` & `fitsio-1.1.9/cfitsio3490/grparser.h`

 * *Files identical despite different names*

### Comparing `fitsio-1.1.8/cfitsio3490/histo.c` & `fitsio-1.1.9/cfitsio3490/histo.c`

 * *Files identical despite different names*

### Comparing `fitsio-1.1.8/cfitsio3490/imcompress.c` & `fitsio-1.1.9/cfitsio3490/imcompress.c`

 * *Files identical despite different names*

### Comparing `fitsio-1.1.8/cfitsio3490/imcopy.c` & `fitsio-1.1.9/cfitsio3490/imcopy.c`

 * *Files identical despite different names*

### Comparing `fitsio-1.1.8/cfitsio3490/install-sh` & `fitsio-1.1.9/cfitsio3490/install-sh`

 * *Files identical despite different names*

### Comparing `fitsio-1.1.8/cfitsio3490/iraffits.c` & `fitsio-1.1.9/cfitsio3490/iraffits.c`

 * *Files identical despite different names*

### Comparing `fitsio-1.1.8/cfitsio3490/iter_a.c` & `fitsio-1.1.9/cfitsio3490/iter_a.c`

 * *Files identical despite different names*

### Comparing `fitsio-1.1.8/cfitsio3490/iter_a.f` & `fitsio-1.1.9/cfitsio3490/iter_a.f`

 * *Files identical despite different names*

### Comparing `fitsio-1.1.8/cfitsio3490/iter_a.fit` & `fitsio-1.1.9/cfitsio3490/iter_a.fit`

 * *Files identical despite different names*

### Comparing `fitsio-1.1.8/cfitsio3490/iter_b.c` & `fitsio-1.1.9/cfitsio3490/iter_b.c`

 * *Files identical despite different names*

### Comparing `fitsio-1.1.8/cfitsio3490/iter_b.f` & `fitsio-1.1.9/cfitsio3490/iter_b.f`

 * *Files identical despite different names*

### Comparing `fitsio-1.1.8/cfitsio3490/iter_b.fit` & `fitsio-1.1.9/cfitsio3490/iter_b.fit`

 * *Files identical despite different names*

### Comparing `fitsio-1.1.8/cfitsio3490/iter_c.c` & `fitsio-1.1.9/cfitsio3490/iter_c.c`

 * *Files identical despite different names*

### Comparing `fitsio-1.1.8/cfitsio3490/iter_c.f` & `fitsio-1.1.9/cfitsio3490/iter_c.f`

 * *Files identical despite different names*

### Comparing `fitsio-1.1.8/cfitsio3490/iter_c.fit` & `fitsio-1.1.9/cfitsio3490/iter_c.fit`

 * *Files identical despite different names*

### Comparing `fitsio-1.1.8/cfitsio3490/iter_image.c` & `fitsio-1.1.9/cfitsio3490/iter_image.c`

 * *Files identical despite different names*

### Comparing `fitsio-1.1.8/cfitsio3490/iter_var.c` & `fitsio-1.1.9/cfitsio3490/iter_var.c`

 * *Files identical despite different names*

### Comparing `fitsio-1.1.8/cfitsio3490/longnam.h` & `fitsio-1.1.9/cfitsio3490/longnam.h`

 * *Files identical despite different names*

### Comparing `fitsio-1.1.8/cfitsio3490/makefile.bc` & `fitsio-1.1.9/cfitsio3490/makefile.bc`

 * *Files identical despite different names*

### Comparing `fitsio-1.1.8/cfitsio3490/makefile.vcc` & `fitsio-1.1.9/cfitsio3490/makefile.vcc`

 * *Files identical despite different names*

### Comparing `fitsio-1.1.8/cfitsio3490/makepc.bat` & `fitsio-1.1.9/cfitsio3490/makepc.bat`

 * *Files identical despite different names*

### Comparing `fitsio-1.1.8/cfitsio3490/modkey.c` & `fitsio-1.1.9/cfitsio3490/modkey.c`

 * *Files identical despite different names*

### Comparing `fitsio-1.1.8/cfitsio3490/pliocomp.c` & `fitsio-1.1.9/cfitsio3490/pliocomp.c`

 * *Files identical despite different names*

### Comparing `fitsio-1.1.8/cfitsio3490/putcol.c` & `fitsio-1.1.9/cfitsio3490/putcol.c`

 * *Files identical despite different names*

### Comparing `fitsio-1.1.8/cfitsio3490/putcolb.c` & `fitsio-1.1.9/cfitsio3490/putcolb.c`

 * *Files identical despite different names*

### Comparing `fitsio-1.1.8/cfitsio3490/putcold.c` & `fitsio-1.1.9/cfitsio3490/putcold.c`

 * *Files identical despite different names*

### Comparing `fitsio-1.1.8/cfitsio3490/putcole.c` & `fitsio-1.1.9/cfitsio3490/putcole.c`

 * *Files identical despite different names*

### Comparing `fitsio-1.1.8/cfitsio3490/putcoli.c` & `fitsio-1.1.9/cfitsio3490/putcoli.c`

 * *Files identical despite different names*

### Comparing `fitsio-1.1.8/cfitsio3490/putcolj.c` & `fitsio-1.1.9/cfitsio3490/putcolj.c`

 * *Files identical despite different names*

### Comparing `fitsio-1.1.8/cfitsio3490/putcolk.c` & `fitsio-1.1.9/cfitsio3490/putcolk.c`

 * *Files identical despite different names*

### Comparing `fitsio-1.1.8/cfitsio3490/putcoll.c` & `fitsio-1.1.9/cfitsio3490/putcoll.c`

 * *Files identical despite different names*

### Comparing `fitsio-1.1.8/cfitsio3490/putcols.c` & `fitsio-1.1.9/cfitsio3490/putcols.c`

 * *Files identical despite different names*

### Comparing `fitsio-1.1.8/cfitsio3490/putcolsb.c` & `fitsio-1.1.9/cfitsio3490/putcolsb.c`

 * *Files identical despite different names*

### Comparing `fitsio-1.1.8/cfitsio3490/putcolu.c` & `fitsio-1.1.9/cfitsio3490/putcolu.c`

 * *Files identical despite different names*

### Comparing `fitsio-1.1.8/cfitsio3490/putcolui.c` & `fitsio-1.1.9/cfitsio3490/putcolui.c`

 * *Files identical despite different names*

### Comparing `fitsio-1.1.8/cfitsio3490/putcoluj.c` & `fitsio-1.1.9/cfitsio3490/putcoluj.c`

 * *Files identical despite different names*

### Comparing `fitsio-1.1.8/cfitsio3490/putcoluk.c` & `fitsio-1.1.9/cfitsio3490/putcoluk.c`

 * *Files identical despite different names*

### Comparing `fitsio-1.1.8/cfitsio3490/putkey.c` & `fitsio-1.1.9/cfitsio3490/putkey.c`

 * *Files identical despite different names*

### Comparing `fitsio-1.1.8/cfitsio3490/quantize.c` & `fitsio-1.1.9/cfitsio3490/quantize.c`

 * *Files identical despite different names*

### Comparing `fitsio-1.1.8/cfitsio3490/region.c` & `fitsio-1.1.9/cfitsio3490/region.c`

 * *Files identical despite different names*

### Comparing `fitsio-1.1.8/cfitsio3490/region.h` & `fitsio-1.1.9/cfitsio3490/region.h`

 * *Files identical despite different names*

### Comparing `fitsio-1.1.8/cfitsio3490/ricecomp.c` & `fitsio-1.1.9/cfitsio3490/ricecomp.c`

 * *Files identical despite different names*

### Comparing `fitsio-1.1.8/cfitsio3490/sample.tpl` & `fitsio-1.1.9/cfitsio3490/sample.tpl`

 * *Files identical despite different names*

### Comparing `fitsio-1.1.8/cfitsio3490/scalnull.c` & `fitsio-1.1.9/cfitsio3490/scalnull.c`

 * *Files identical despite different names*

### Comparing `fitsio-1.1.8/cfitsio3490/simplerng.c` & `fitsio-1.1.9/cfitsio3490/simplerng.c`

 * *Files identical despite different names*

### Comparing `fitsio-1.1.8/cfitsio3490/simplerng.h` & `fitsio-1.1.9/cfitsio3490/simplerng.h`

 * *Files identical despite different names*

### Comparing `fitsio-1.1.8/cfitsio3490/smem.c` & `fitsio-1.1.9/cfitsio3490/smem.c`

 * *Files identical despite different names*

### Comparing `fitsio-1.1.8/cfitsio3490/speed.c` & `fitsio-1.1.9/cfitsio3490/speed.c`

 * *Files identical despite different names*

### Comparing `fitsio-1.1.8/cfitsio3490/swapproc.c` & `fitsio-1.1.9/cfitsio3490/swapproc.c`

 * *Files identical despite different names*

### Comparing `fitsio-1.1.8/cfitsio3490/testf77.f` & `fitsio-1.1.9/cfitsio3490/testf77.f`

 * *Files identical despite different names*

### Comparing `fitsio-1.1.8/cfitsio3490/testf77.out` & `fitsio-1.1.9/cfitsio3490/testf77.out`

 * *Files identical despite different names*

### Comparing `fitsio-1.1.8/cfitsio3490/testf77.std` & `fitsio-1.1.9/cfitsio3490/testf77.std`

 * *Files identical despite different names*

### Comparing `fitsio-1.1.8/cfitsio3490/testprog.c` & `fitsio-1.1.9/cfitsio3490/testprog.c`

 * *Files identical despite different names*

### Comparing `fitsio-1.1.8/cfitsio3490/testprog.out` & `fitsio-1.1.9/cfitsio3490/testprog.out`

 * *Files identical despite different names*

### Comparing `fitsio-1.1.8/cfitsio3490/testprog.std` & `fitsio-1.1.9/cfitsio3490/testprog.std`

 * *Files identical despite different names*

### Comparing `fitsio-1.1.8/cfitsio3490/vmsieee.c` & `fitsio-1.1.9/cfitsio3490/vmsieee.c`

 * *Files identical despite different names*

### Comparing `fitsio-1.1.8/cfitsio3490/wcssub.c` & `fitsio-1.1.9/cfitsio3490/wcssub.c`

 * *Files identical despite different names*

### Comparing `fitsio-1.1.8/cfitsio3490/wcsutil.c` & `fitsio-1.1.9/cfitsio3490/wcsutil.c`

 * *Files identical despite different names*

### Comparing `fitsio-1.1.8/cfitsio3490/winDumpExts.mak` & `fitsio-1.1.9/cfitsio3490/winDumpExts.mak`

 * *Files identical despite different names*

### Comparing `fitsio-1.1.8/cfitsio3490/windumpexts.c` & `fitsio-1.1.9/cfitsio3490/windumpexts.c`

 * *Files identical despite different names*

### Comparing `fitsio-1.1.8/cfitsio3490/zlib/adler32.c` & `fitsio-1.1.9/cfitsio3490/zlib/adler32.c`

 * *Files identical despite different names*

### Comparing `fitsio-1.1.8/cfitsio3490/zlib/crc32.c` & `fitsio-1.1.9/cfitsio3490/zlib/crc32.c`

 * *Files identical despite different names*

### Comparing `fitsio-1.1.8/cfitsio3490/zlib/crc32.h` & `fitsio-1.1.9/cfitsio3490/zlib/crc32.h`

 * *Files identical despite different names*

### Comparing `fitsio-1.1.8/cfitsio3490/zlib/deflate.c` & `fitsio-1.1.9/cfitsio3490/zlib/deflate.c`

 * *Files identical despite different names*

### Comparing `fitsio-1.1.8/cfitsio3490/zlib/deflate.h` & `fitsio-1.1.9/cfitsio3490/zlib/deflate.h`

 * *Files identical despite different names*

### Comparing `fitsio-1.1.8/cfitsio3490/zlib/infback.c` & `fitsio-1.1.9/cfitsio3490/zlib/infback.c`

 * *Files identical despite different names*

### Comparing `fitsio-1.1.8/cfitsio3490/zlib/inffast.c` & `fitsio-1.1.9/cfitsio3490/zlib/inffast.c`

 * *Files identical despite different names*

### Comparing `fitsio-1.1.8/cfitsio3490/zlib/inffixed.h` & `fitsio-1.1.9/cfitsio3490/zlib/inffixed.h`

 * *Files identical despite different names*

### Comparing `fitsio-1.1.8/cfitsio3490/zlib/inflate.c` & `fitsio-1.1.9/cfitsio3490/zlib/inflate.c`

 * *Files identical despite different names*

### Comparing `fitsio-1.1.8/cfitsio3490/zlib/inflate.h` & `fitsio-1.1.9/cfitsio3490/zlib/inflate.h`

 * *Files identical despite different names*

### Comparing `fitsio-1.1.8/cfitsio3490/zlib/inftrees.c` & `fitsio-1.1.9/cfitsio3490/zlib/inftrees.c`

 * *Files identical despite different names*

### Comparing `fitsio-1.1.8/cfitsio3490/zlib/inftrees.h` & `fitsio-1.1.9/cfitsio3490/zlib/inftrees.h`

 * *Files identical despite different names*

### Comparing `fitsio-1.1.8/cfitsio3490/zlib/trees.c` & `fitsio-1.1.9/cfitsio3490/zlib/trees.c`

 * *Files identical despite different names*

### Comparing `fitsio-1.1.8/cfitsio3490/zlib/trees.h` & `fitsio-1.1.9/cfitsio3490/zlib/trees.h`

 * *Files identical despite different names*

### Comparing `fitsio-1.1.8/cfitsio3490/zlib/uncompr.c` & `fitsio-1.1.9/cfitsio3490/zlib/uncompr.c`

 * *Files identical despite different names*

### Comparing `fitsio-1.1.8/cfitsio3490/zlib/zcompress.c` & `fitsio-1.1.9/cfitsio3490/zlib/zcompress.c`

 * *Files identical despite different names*

### Comparing `fitsio-1.1.8/cfitsio3490/zlib/zconf.h` & `fitsio-1.1.9/cfitsio3490/zlib/zconf.h`

 * *Files identical despite different names*

### Comparing `fitsio-1.1.8/cfitsio3490/zlib/zlib.h` & `fitsio-1.1.9/cfitsio3490/zlib/zlib.h`

 * *Files identical despite different names*

### Comparing `fitsio-1.1.8/cfitsio3490/zlib/zuncompress.c` & `fitsio-1.1.9/cfitsio3490/zlib/zuncompress.c`

 * *Files identical despite different names*

### Comparing `fitsio-1.1.8/cfitsio3490/zlib/zutil.c` & `fitsio-1.1.9/cfitsio3490/zlib/zutil.c`

 * *Files identical despite different names*

### Comparing `fitsio-1.1.8/cfitsio3490/zlib/zutil.h` & `fitsio-1.1.9/cfitsio3490/zlib/zutil.h`

 * *Files identical despite different names*

### Comparing `fitsio-1.1.8/fitsio/__init__.py` & `fitsio-1.1.9/fitsio/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # flake8: noqa
 """
 A python library to read and write data to FITS files using cfitsio.
 See the docs at https://github.com/esheldon/fitsio for example
 usage.
 """
 
-__version__ = '1.1.8'
+__version__ = '1.1.9'
 
 from . import fitslib
 
 from .fitslib import (
     FITS,
     read,
     read_header,
@@ -31,9 +31,7 @@
 )
 
 from .header import FITSHDR, FITSRecord, FITSCard
 from .hdu import BINARY_TBL, ASCII_TBL, IMAGE_HDU
 
 from . import util
 from .util import cfitsio_version, FITSRuntimeWarning
-
-from . import test
```

### Comparing `fitsio-1.1.8/fitsio/fitsio_pywrap.c` & `fitsio-1.1.9/fitsio/fitsio_pywrap.c`

 * *Files 2% similar despite different names*

```diff
@@ -1476,16 +1476,18 @@
         // if (comptype >= 0) {
         if (comptype > 0) {
             // exception strings are set internally
             if (set_compression(self->fits, comptype, tile_dims_obj, &status)) {
                 goto create_image_hdu_cleanup;
             }
 
-            if (fits_set_quantize_level(self->fits, qlevel, &status)) {
-                goto create_image_hdu_cleanup;
+            if (qlevel > 0) {
+                if (fits_set_quantize_level(self->fits, qlevel, &status)) {
+                    goto create_image_hdu_cleanup;
+                }
             }
 
             if (fits_set_quantize_method(self->fits, qmethod, &status)) {
                 goto create_image_hdu_cleanup;
             }
 
             if (comptype == HCOMPRESS_1) {
@@ -2521,15 +2523,15 @@
         return NULL;
     }
 
     if (strlen(comment_in) > 0) {
         comment=comment_in;
     }
 
-    if (fits_write_key_longstr(self->fits, keyname, value, comment, &status)) {
+    if (fits_update_key_longstr(self->fits, keyname, value, comment, &status)) {
         set_ioerr_string_from_status(status);
         return NULL;
     }
 
     // this does not close and reopen
     if (fits_flush_buffer(self->fits, 0, &status)) {
         set_ioerr_string_from_status(status);
@@ -3087,22 +3089,28 @@
         }
     }
 
     return 0;
 
 }
 static int read_ascii_column_byrow(
-        fitsfile* fits, int colnum, PyObject* array, PyObject* rowsObj, int* status) {
+        fitsfile* fits, int colnum, PyObject* array,
+        PyObject* rowsObj,
+        PyObject* sortindObj,
+        int* status
+)
+{
 
     int npy_dtype=0;
     int fits_dtype=0;
 
     npy_intp nelem=0;
     LONGLONG firstelem=1;
     LONGLONG rownum=0;
+    npy_int64 si=0;
     npy_intp nrows=-1;
 
     int* anynul=NULL;
     void* nulval=0;
     char* nulstr=" ";
     void* data=NULL;
     char* cdata=NULL;
@@ -3123,24 +3131,25 @@
         if (nrows != nelem) {
             PyErr_Format(PyExc_ValueError,
                     "input array[%ld] and rows[%ld] have different size", nelem,nrows);
             return 1;
         }
     }
 
-    data = PyArray_GETPTR1(array, i);
     for (i=0; i<nrows; i++) {
         if (dorows) {
-            rownum = (LONGLONG) (1 + *(npy_int64*) PyArray_GETPTR1(rowsObj, i));
+            si = *(npy_int64*) PyArray_GETPTR1(sortindObj, i);
+            rownum = (LONGLONG)( *(npy_int64*) PyArray_GETPTR1(rowsObj, si) );
+            rownum += 1;
         } else {
             rownum = (LONGLONG) (1+i);
         }
         // assuming 1-D
-        data = PyArray_GETPTR1(array, i);
-        if (fits_dtype==TSTRING) {
+        data = PyArray_GETPTR1(array, si);
+        if (fits_dtype == TSTRING) {
             cdata = (char* ) data;
             if (fits_read_col_str(fits,colnum,rownum,firstelem,1,nulstr,&cdata,anynul,status) > 0) {
                 return 1;
             }
         } else {
             if (fits_read_col(fits,fits_dtype,colnum,rownum,firstelem,1,nulval,data,anynul,status) > 0) {
                 return 1;
@@ -3148,19 +3157,27 @@
         }
     }
 
     return 0;
 }
 
 
-static int read_ascii_column(fitsfile* fits, int colnum, PyObject* array, PyObject* rowsObj, int* status) {
+static int read_ascii_column(
+    fitsfile* fits, int colnum, PyObject* array,
+    PyObject* rowsObj,
+    PyObject* sortindObj,
+    int* status
+)
+{
 
     int ret=0;
     if (rowsObj != Py_None || !PyArray_ISCONTIGUOUS(array)) {
-        ret = read_ascii_column_byrow(fits, colnum, array, rowsObj, status);
+        ret = read_ascii_column_byrow(
+            fits, colnum, array, rowsObj, sortindObj, status
+        );
     } else {
         ret = read_ascii_column_all(fits, colnum, array, status);
     }
 
     return ret;
 }
 
@@ -3171,54 +3188,59 @@
 // read a subset of rows for the input column
 // the row array is assumed to be unique and sorted.
 static int read_binary_column(
         fitsfile* fits,
         int colnum,
         npy_intp nrows,
         npy_int64* rows,
-        void* data,
+        npy_int64* sortind,
+        void* vdata,
         npy_intp stride,
         int* status) {
 
     FITSfile* hdu=NULL;
     tcolumn* colptr=NULL;
     LONGLONG file_pos=0, irow=0;
-    npy_int64 row=0;
+    npy_int64 row=0, si=0;
 
     LONGLONG repeat=0;
     LONGLONG width=0;
 
     int rows_sent=0;
 
     // use char for pointer arith.  It's actually ok to use void as char but
     // this is just in case.
-    char* ptr=NULL;
+    char *data=NULL, *ptr=NULL;
+
+    data = (char *) vdata;
 
     // using struct defs here, could cause problems
     hdu = fits->Fptr;
     colptr = hdu->tableptr + (colnum-1);
 
     repeat = colptr->trepeat;
     width = colptr->tdatatype == TSTRING ? 1 : colptr->twidth;
 
     rows_sent = nrows == hdu->numrows ? 0 : 1;
 
-    ptr = (char*) data;
     for (irow=0; irow<nrows; irow++) {
         if (rows_sent) {
-            row = rows[irow];
+            si = sortind[irow];
+            row = rows[si];
         } else {
             row = irow;
         }
+
+        ptr = data + si * stride;
+
         file_pos = hdu->datastart + row*hdu->rowlength + colptr->tbcol;
         ffmbyt(fits, file_pos, REPORT_EOF, status);
         if (ffgbytoff(fits, width, repeat, 0, (void*)ptr, status)) {
             return 1;
         }
-        ptr += stride;
     }
 
     return 0;
 }
 
 
 
@@ -3234,16 +3256,18 @@
 
     FITSfile* hdu=NULL;
     int status=0;
 
     PyObject* array=NULL;
 
     PyObject* rowsObj;
+    PyObject* sortindObj;
 
-    if (!PyArg_ParseTuple(args, (char*)"iiOO", &hdunum, &colnum, &array, &rowsObj)) {
+    if (!PyArg_ParseTuple(args, (char*)"iiOOO",
+            &hdunum, &colnum, &array, &rowsObj, &sortindObj)) {
         return NULL;
     }
 
     if (self->fits == NULL) {
         PyErr_SetString(PyExc_RuntimeError, "FITS file is NULL");
         return NULL;
     }
@@ -3261,30 +3285,31 @@
     if (colnum < 1 || colnum > hdu->tfield) {
         PyErr_SetString(PyExc_RuntimeError, "requested column is out of bounds");
         return NULL;
     }
 
 
     if (hdutype == ASCII_TBL) {
-        if (read_ascii_column(self->fits, colnum, array, rowsObj, &status)) {
+        if (read_ascii_column(self->fits, colnum, array, rowsObj, sortindObj, &status)) {
             set_ioerr_string_from_status(status);
             return NULL;
         }
     } else {
         void* data=PyArray_DATA(array);
-        npy_intp nrows=0;
-        npy_int64* rows=NULL;
+        npy_intp nrows=0, nsortind=0;
+        npy_int64* rows=NULL, *sortind=NULL;
         npy_intp stride=PyArray_STRIDE(array,0);
         if (rowsObj == Py_None) {
             nrows = hdu->numrows;
         } else {
             rows = get_int64_from_array(rowsObj, &nrows);
+            sortind = get_int64_from_array(sortindObj, &nsortind);
         }
 
-        if (read_binary_column(self->fits, colnum, nrows, rows, data, stride, &status)) {
+        if (read_binary_column(self->fits, colnum, nrows, rows, sortind, data, stride, &status)) {
             set_ioerr_string_from_status(status);
             return NULL;
         }
     }
     Py_RETURN_NONE;
 }
 
@@ -3373,36 +3398,38 @@
  * what about strings?
  */
 static PyObject *
 PyFITSObject_read_var_column_as_list(struct PyFITSObject* self, PyObject* args) {
     int hdunum=0;
     int colnum=0;
     PyObject* rowsObj=NULL;
+    PyObject* sortindObj=NULL;
 
     int hdutype=0;
     int ncols=0;
-    const npy_int64* rows=NULL;
+    const npy_int64* rows=NULL, *sortind=NULL;
     LONGLONG nrows=0;
     int get_all_rows=0;
 
     int status=0, tstatus=0;
 
     int fits_dtype=0;
     int npy_dtype=0;
     int isvariable=0;
     LONGLONG repeat=0;
     LONGLONG width=0;
     LONGLONG offset=0;
     LONGLONG i=0;
     LONGLONG row=0;
+    npy_int64 si = 0;
 
     PyObject* listObj=NULL;
     PyObject* tempObj=NULL;
 
-    if (!PyArg_ParseTuple(args, (char*)"iiO", &hdunum, &colnum, &rowsObj)) {
+    if (!PyArg_ParseTuple(args, (char*)"iiOO", &hdunum, &colnum, &rowsObj, &sortindObj)) {
         return NULL;
     }
 
     if (self->fits == NULL) {
         PyErr_SetString(PyExc_RuntimeError, "FITS file is NULL");
         return NULL;
     }
@@ -3436,29 +3463,31 @@
         return NULL;
     }
 
     if (rowsObj == Py_None) {
         fits_get_num_rowsll(self->fits, &nrows, &tstatus);
         get_all_rows=1;
     } else {
-        npy_intp tnrows=0;
+        npy_intp tnrows=0, nsortind=0;
         rows = (const npy_int64*) get_int64_from_array(rowsObj, &tnrows);
-        nrows=(LONGLONG) tnrows;
-        get_all_rows=0;
+        sortind = (const npy_int64*) get_int64_from_array(sortindObj, &nsortind);
+        nrows = (LONGLONG) tnrows;
+        get_all_rows = 0;
     }
 
     listObj = PyList_New(0);
 
     for (i=0; i<nrows; i++) {
         tempObj=NULL;
 
         if (get_all_rows) {
             row = i+1;
         } else {
-            row = (LONGLONG) (rows[i]+1);
+            si = sortind[i];
+            row = (LONGLONG) (rows[si]+1);
         }
 
         // repeat holds how many elements are in this row
         if (fits_read_descriptll(self->fits, colnum, row, &repeat, &offset, &status) > 0) {
             goto read_var_column_cleanup;
         }
 
@@ -3491,70 +3520,77 @@
     return listObj;
 }
 
 
 // read specified columns and rows
 static int read_binary_rec_columns(
         fitsfile* fits,
-        npy_intp ncols, npy_int64* colnums,
-        npy_intp nrows, npy_int64* rows,
-        void* data, int* status) {
+        npy_intp ncols,
+        npy_int64* colnums,
+        npy_intp nrows,
+        npy_int64* rows,
+        npy_int64* sortind,
+        PyObject *array,
+        int* status
+) {
     FITSfile* hdu=NULL;
     tcolumn* colptr=NULL;
     LONGLONG file_pos=0;
     npy_intp col=0;
     npy_int64 colnum=0;
+    char* ptr=NULL;
 
     int rows_sent=0;
     npy_intp irow=0;
-    npy_int64 row=0;
-
-    // use char for pointer arith.  It's actually ok to use void as char but
-    // this is just in case.
-    char* ptr;
+    npy_int64 row=0, si=0;
 
     LONGLONG gsize=0; // number of bytes in column
     LONGLONG repeat=0;
     LONGLONG width=0;
 
     // using struct defs here, could cause problems
     hdu = fits->Fptr;
 
-    rows_sent = nrows == hdu->numrows ? 0 : 1;
+    rows_sent = (nrows == hdu->numrows) ? 0 : 1;
 
-    ptr = (char*) data;
-    for (irow=0; irow<nrows; irow++) {
+    for (irow=0; irow < nrows; irow++) {
         if (rows_sent) {
-            row = rows[irow];
+            si = sortind[irow];
+            row = rows[si];
         } else {
+            si = irow;
             row = irow;
         }
+
+        ptr = (char *) PyArray_GETPTR1(array, si);
         for (col=0; col < ncols; col++) {
 
             colnum = colnums[col];
             colptr = hdu->tableptr + (colnum-1);
 
             repeat = colptr->trepeat;
             width = colptr->tdatatype == TSTRING ? 1 : colptr->twidth;
-            gsize = repeat*width;
 
             file_pos = hdu->datastart + row*hdu->rowlength + colptr->tbcol;
 
             if (colptr->tdatatype == TBIT) {
-                if (fits_read_col_bit(fits, colnum, row+1, 1, repeat, (char*)ptr, status)) {
+                if (fits_read_col_bit(fits, colnum, row+1, 1, repeat, ptr, status)) {
                     return 1;
                 }
             } else {
                 // can just do one status check, since status are inherited.
                 ffmbyt(fits, file_pos, REPORT_EOF, status);
                 if (ffgbytoff(fits, width, repeat, 0, (void*)ptr, status)) {
                     return 1;
                 }
             }
+
+            gsize = repeat * width;
             ptr += gsize;
+
         }
     }
 
     return 0;
 }
 
 
@@ -3568,19 +3604,23 @@
     npy_int64* colnums=NULL;
     FITSfile* hdu=NULL;
 
     int status=0;
 
     PyObject* columnsobj=NULL;
     PyObject* array=NULL;
-    void* data=NULL;
 
-    PyObject* rowsobj=NULL;
+    PyObject* rowsObj=NULL;
+    PyObject* sortindObj=NULL;
+
+    npy_intp nrows, nsortind;
+    npy_int64* rows=NULL, *sortind=NULL;
 
-    if (!PyArg_ParseTuple(args, (char*)"iOOO", &hdunum, &columnsobj, &array, &rowsobj)) {
+    if (!PyArg_ParseTuple(args, (char*)"iOOOO",
+                          &hdunum, &columnsobj, &array, &rowsObj, &sortindObj)) {
         return NULL;
     }
 
     if (self->fits == NULL) {
         PyErr_SetString(PyExc_RuntimeError, "FITS file is NULL");
         return NULL;
     }
@@ -3595,23 +3635,24 @@
 
     colnums = get_int64_from_array(columnsobj, &ncols);
     if (colnums == NULL) {
         return NULL;
     }
 
     hdu = self->fits->Fptr;
-    data = PyArray_DATA(array);
-    npy_intp nrows;
-    npy_int64* rows=NULL;
-    if (rowsobj == Py_None) {
+
+    if (rowsObj == Py_None) {
         nrows = hdu->numrows;
     } else {
-        rows = get_int64_from_array(rowsobj, &nrows);
+        rows = get_int64_from_array(rowsObj, &nrows);
+        sortind = get_int64_from_array(sortindObj, &nsortind);
     }
-    if (read_binary_rec_columns(self->fits, ncols, colnums, nrows, rows, data, &status)) {
+    if (read_binary_rec_columns(
+            self->fits, ncols, colnums,
+            nrows, rows, sortind, array, &status)) {
         goto recread_columns_cleanup;
     }
 
 recread_columns_cleanup:
 
     if (status != 0) {
         set_ioerr_string_from_status(status);
@@ -3635,50 +3676,53 @@
 static int read_columns_as_rec_byoffset(
         fitsfile* fits,
         npy_intp ncols,
         const npy_int64* colnums,         // columns to read from file
         const npy_int64* field_offsets,   // offsets of corresponding fields within array
         npy_intp nrows,
         const npy_int64* rows,
+        const npy_int64* sortind,
         char* data,
         npy_intp recsize,
         int* status) {
 
     FITSfile* hdu=NULL;
     tcolumn* colptr=NULL;
     LONGLONG file_pos=0;
     npy_intp col=0;
     npy_int64 colnum=0;
 
     char* ptr=NULL;
 
     int get_all_rows=1;
     npy_intp irow=0;
-    npy_int64 row=0;
+    npy_int64 row=0, si=0;
 
     long groupsize=0; // number of bytes in column
     long ngroups=1; // number to read, one for row-by-row reading
     long group_gap=0; // gap between groups, zero since we aren't using it
 
     if (rows != NULL) {
         get_all_rows=0;
     }
 
     // using struct defs here, could cause problems
     hdu = fits->Fptr;
-    for (irow=0; irow<nrows; irow++) {
+    for (irow=0; irow < nrows; irow++) {
         if (get_all_rows) {
-            row=irow;
+            row = irow;
+            si = irow;
         } else {
-            row = rows[irow];
+            si = sortind[irow];
+            row = rows[si];
         }
         for (col=0; col < ncols; col++) {
 
             // point to this field in the array, allows for skipping
-            ptr = data + irow*recsize + field_offsets[col];
+            ptr = data + si*recsize + field_offsets[col];
 
             colnum = colnums[col];
             colptr = hdu->tableptr + (colnum-1);
 
             groupsize = get_groupsize(colptr);
 
             file_pos = hdu->datastart + row*hdu->rowlength + colptr->tbcol;
@@ -3710,28 +3754,30 @@
 PyFITSObject_read_columns_as_rec_byoffset(struct PyFITSObject* self, PyObject* args) {
     int status=0;
     int hdunum=0;
     int hdutype=0;
 
     npy_intp ncols=0;
     npy_intp noffsets=0;
-    npy_intp nrows=0;
+    npy_intp nrows=0, nsortind=0;
     const npy_int64* colnums=NULL;
     const npy_int64* offsets=NULL;
-    const npy_int64* rows=NULL;
+    const npy_int64* rows=NULL, *sortind=NULL;
 
     PyObject* columnsObj=NULL;
     PyObject* offsetsObj=NULL;
     PyObject* rowsObj=NULL;
+    PyObject* sortindObj=NULL;
 
     PyObject* array=NULL;
     void* data=NULL;
     npy_intp recsize=0;
 
-    if (!PyArg_ParseTuple(args, (char*)"iOOOO", &hdunum, &columnsObj, &offsetsObj, &array, &rowsObj)) {
+    if (!PyArg_ParseTuple(args, (char*)"iOOOOO",
+            &hdunum, &columnsObj, &offsetsObj, &array, &rowsObj, &sortindObj)) {
         return NULL;
     }
 
     if (self->fits == NULL) {
         PyErr_SetString(PyExc_RuntimeError, "FITS file is NULL");
         return NULL;
     }
@@ -3757,25 +3803,27 @@
                      "%ld columns requested but got %ld offsets",
                      ncols, noffsets);
         return NULL;
     }
 
     if (rowsObj != Py_None) {
         rows = (const npy_int64*) get_int64_from_array(rowsObj, &nrows);
+        sortind = (const npy_int64*) get_int64_from_array(sortindObj, &nsortind);
     } else {
         nrows = PyArray_SIZE(array);
     }
 
     data = PyArray_DATA(array);
     recsize = PyArray_ITEMSIZE(array);
     if (read_columns_as_rec_byoffset(
                 self->fits,
                 ncols, colnums, offsets,
                 nrows,
                 rows,
+                sortind,
                 (char*) data,
                 recsize,
                 &status) > 0) {
         goto recread_columns_byoffset_cleanup;
     }
 
 recread_columns_byoffset_cleanup:
@@ -3788,40 +3836,46 @@
 }
 
 
 
 // read specified rows, all columns
 static int read_rec_bytes_byrow(
         fitsfile* fits,
-        npy_intp nrows, npy_int64* rows,
-        void* data, int* status) {
+        npy_intp nrows, npy_int64* rows, npy_int64* sortind,
+        void* vdata, int* status) {
 
     FITSfile* hdu=NULL;
 
-    npy_intp irow=0;
+    npy_intp irow=0, si=0;
     LONGLONG firstrow=1;
     LONGLONG firstchar=1;
 
     // use char for pointer arith.  It's actually ok to use void as char but
     // this is just in case.
-    unsigned char* ptr;
+    unsigned char* ptr, *data;
 
     // using struct defs here, could cause problems
     hdu = fits->Fptr;
-    ptr = (unsigned char*) data;
+    // ptr = (unsigned char*) data;
+    data = (unsigned char*) vdata;
+
+    for (irow=0; irow < nrows; irow++) {
+
+        si = sortind[irow];
 
-    for (irow=0; irow<nrows; irow++) {
         // Input is zero-offset
-        firstrow = 1 + (LONGLONG) rows[irow];
+        firstrow = 1 + (LONGLONG) rows[si];
+
+        ptr = data + si * hdu->rowlength;
 
         if (fits_read_tblbytes(fits, firstrow, firstchar, hdu->rowlength, ptr, status)) {
             return 1;
         }
 
-        ptr += hdu->rowlength;
+        // ptr += hdu->rowlength;
     }
 
     return 0;
 }
 // read specified rows, all columns
 /*
 static int read_rec_bytes_byrowold(
@@ -3869,18 +3923,20 @@
     int hdutype=0;
 
     int status=0;
     PyObject* array=NULL;
     void* data=NULL;
 
     PyObject* rowsObj=NULL;
-    npy_intp nrows=0;
+    PyObject* sortindObj=NULL;
+    npy_intp nrows=0, nsortind=0;
     npy_int64* rows=NULL;
+    npy_int64* sortind=NULL;
 
-    if (!PyArg_ParseTuple(args, (char*)"iOO", &hdunum, &array, &rowsObj)) {
+    if (!PyArg_ParseTuple(args, (char*)"iOOO", &hdunum, &array, &rowsObj, &sortindObj)) {
         return NULL;
     }
 
     if (self->fits == NULL) {
         PyErr_SetString(PyExc_RuntimeError, "FITS file is NULL");
         return NULL;
     }
@@ -3895,16 +3951,20 @@
 
     data = PyArray_DATA(array);
 
     rows = get_int64_from_array(rowsObj, &nrows);
     if (rows == NULL) {
         return NULL;
     }
+    sortind = get_int64_from_array(sortindObj, &nsortind);
+    if (sortind == NULL) {
+        return NULL;
+    }
 
-    if (read_rec_bytes_byrow(self->fits, nrows, rows, data, &status)) {
+    if (read_rec_bytes_byrow(self->fits, nrows, rows, sortind, data, &status)) {
         goto recread_byrow_cleanup;
     }
 
 recread_byrow_cleanup:
 
     if (status != 0) {
         set_ioerr_string_from_status(status);
@@ -4538,50 +4598,51 @@
 static PyObject *
 PyFITSObject_where(struct PyFITSObject* self, PyObject* args) {
     int status=0;
     int hdunum=0;
     int hdutype=0;
     char* expression=NULL;
 
-    LONGLONG nrows=0;
-
-    long firstrow=1;
+    long firstrow;
+    long nrows;
     long ngood=0;
     char* row_status=NULL;
 
 
     // Indices of rows for which expression is true
     PyObject* indicesObj=NULL;
     int ndim=1;
     npy_intp dims[1];
     npy_intp* data=NULL;
     long i=0;
 
 
-    if (!PyArg_ParseTuple(args, (char*)"is", &hdunum, &expression)) {
+    if (!PyArg_ParseTuple(args, (char*)"isll", &hdunum, &expression,
+                          &firstrow, &nrows)) {
         return NULL;
     }
 
-    if (fits_movabs_hdu(self->fits, hdunum, &hdutype, &status)) {
-        set_ioerr_string_from_status(status);
+    if (firstrow < 1 || nrows < 1) {
+        PyErr_SetString(PyExc_ValueError,
+                        "firstrow and nrows must be positive integers");
         return NULL;
     }
 
-    if (fits_get_num_rowsll(self->fits, &nrows, &status)) {
+    if (fits_movabs_hdu(self->fits, hdunum, &hdutype, &status)) {
         set_ioerr_string_from_status(status);
         return NULL;
     }
 
     row_status = malloc(nrows*sizeof(char));
     if (row_status==NULL) {
         PyErr_SetString(PyExc_MemoryError, "Could not allocate row_status array");
         return NULL;
     }
 
-    if (fits_find_rows(self->fits, expression, firstrow, (long) nrows, &ngood, row_status, &status)) {
+    if (fits_find_rows(self->fits, expression, firstrow, nrows, &ngood, row_status, &status)) {
         set_ioerr_string_from_status(status);
         goto where_function_cleanup;
     }
 
     dims[0] = ngood;
     indicesObj = PyArray_EMPTY(ndim, dims, NPY_INTP, 0);
     if (indicesObj == NULL) {
```

### Comparing `fitsio-1.1.8/fitsio/fitslib.py` & `fitsio-1.1.9/fitsio/fitslib.py`

 * *Files identical despite different names*

### Comparing `fitsio-1.1.8/fitsio/hdu/base.py` & `fitsio-1.1.9/fitsio/hdu/base.py`

 * *Files identical despite different names*

### Comparing `fitsio-1.1.8/fitsio/hdu/image.py` & `fitsio-1.1.9/fitsio/hdu/image.py`

 * *Files identical despite different names*

### Comparing `fitsio-1.1.8/fitsio/hdu/table.py` & `fitsio-1.1.9/fitsio/hdu/table.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 """
 from __future__ import with_statement, print_function
 import copy
 import warnings
 from functools import reduce
 
-import numpy
+import numpy as np
 
 from ..util import (
     IS_PY3,
     isstring,
     isinteger,
     is_object,
     fields_are_object,
@@ -148,25 +148,39 @@
         Check that the row count is not zero
         """
         if self._info['nrows'] > 0:
             return True
         else:
             return False
 
-    def where(self, expression):
+    def where(self, expression, firstrow=None, lastrow=None):
         """
         Return the indices where the expression evaluates to true.
 
         parameters
         ----------
         expression: string
             A fits row selection expression.  E.g.
             "x > 3 && y < 5"
-        """
-        return self._FITS.where(self._ext+1, expression)
+        firstrow, lastrow : int
+            Range of rows for evaluation.  This follows the Python list
+            slice convention that the last element is not included.
+        """
+        if firstrow is None:
+            firstrow = 0
+        elif firstrow < 0:
+            raise ValueError('firstrow cannot be negative')
+        if lastrow is None:
+            lastrow = self._info['nrows']
+        elif lastrow < firstrow:
+            raise ValueError('lastrow cannot be less than firstrow')
+        elif lastrow > self._info['nrows']:
+            raise ValueError('lastrow cannot be greater than nrows')
+        nrows = lastrow - firstrow
+        return self._FITS.where(self._ext+1, expression, firstrow+1, nrows)
 
     def write(self, data, firstrow=0, columns=None, names=None, slow=False,
               **keys):
         """
         Write data into this HDU
 
         parameters
@@ -216,15 +230,15 @@
             else:
                 columns_all = list(data.keys())
                 data_list = [data[n] for n in columns_all]
 
             colnums_all = [self._extract_colnum(c) for c in columns_all]
             names = [self.get_colname(c) for c in colnums_all]
 
-            isobj = numpy.zeros(len(data_list), dtype=bool)
+            isobj = np.zeros(len(data_list), dtype=bool)
             for i in xrange(len(data_list)):
                 isobj[i] = is_object(data_list[i])
 
         else:
             if data.dtype.fields is None:
                 raise ValueError("You are writing to a table, so I expected "
                                  "an array with fields as input. If you want "
@@ -317,15 +331,15 @@
         colnum = self._extract_colnum(column)
 
         # need it to be contiguous and native byte order.  For now, make a
         # copy.  but we may be able to avoid this with some care.
 
         if not data.flags['C_CONTIGUOUS']:
             # this always makes a copy
-            data_send = numpy.ascontiguousarray(data)
+            data_send = np.ascontiguousarray(data)
             # this is a copy, we can make sure it is native
             # and modify in place if needed
             array_to_native(data_send, inplace=True)
         else:
             # we can avoid the copy with a try-finally block and
             # some logic
             data_send = array_to_native(data, inplace=False)
@@ -377,25 +391,14 @@
         if col_shape is None:
             if this_shape == ():
                 this_shape = None
 
         if col_shape is not None and not isinstance(col_shape, tuple):
             col_shape = (col_shape,)
 
-        """
-        print('column name:',col_name)
-        print(data.shape)
-        print('col tdim', info['tdim'])
-        print('column dtype:',npy_type)
-        print('input dtype:',this_npy_type)
-        print('column shape:',col_shape)
-        print('input shape:',this_shape)
-        print()
-        """
-
         # this mismatch is OK
         if npy_type == 'i1' and this_npy_type == 'b1':
             this_npy_type = 'i1'
 
         if isinstance(self, AsciiTableHDU):
             # we don't enforce types exact for ascii
             if npy_type == 'i8' and this_npy_type in ['i2', 'i4']:
@@ -486,15 +489,15 @@
 
         if IS_PY3 and data.dtype.char == 'U':
             # fast dtype conversion using an empty array
             # we could hack at the actual text description, but using
             # the numpy API is probably safer
             # this also avoids doing a dtype conversion on every array
             # element which could b expensive
-            descr = numpy.empty(1).astype(data.dtype).astype('S').dtype.descr
+            descr = np.empty(1).astype(data.dtype).astype('S').dtype.descr
         else:
             descr = data.dtype.descr
 
         if len(descr) > 1:
             raise ValueError("you can only insert a single column, "
                              "requested: %s" % descr)
 
@@ -577,24 +580,24 @@
         if rows is None:
             return
 
         # extract and convert to 1-offset for C routine
         if isinstance(rows, slice):
             rows = self._process_slice(rows)
             if rows.step is not None and rows.step != 1:
-                rows = numpy.arange(
+                rows = np.arange(
                     rows.start+1,
                     rows.stop+1,
                     rows.step,
                 )
             else:
                 # rows must be 1-offset
                 rows = slice(rows.start+1, rows.stop+1)
         else:
-            rows = self._extract_rows(rows)
+            rows, sortind = self._extract_rows(rows, sort=True)
             # rows must be 1-offset
             rows += 1
 
         if isinstance(rows, slice):
             self._FITS.delete_row_range(self._ext+1, rows.start, rows.stop)
         else:
             if rows.size == 0:
@@ -747,38 +750,41 @@
                 "The keyword arguments '%s' are being ignored! This warning "
                 "will be an error in a future version of `fitsio`!" % keys,
                 DeprecationWarning, stacklevel=2)
 
         dtype, offsets, isvar = self.get_rec_dtype(
             colnums=colnums, vstorage=vstorage)
 
-        w, = numpy.where(isvar == True)  # noqa
+        w, = np.where(isvar == True)  # noqa
         has_tbit = self._check_tbit()
 
         if w.size > 0:
             if vstorage is None:
                 _vstorage = self._vstorage
             else:
                 _vstorage = vstorage
             colnums = self._extract_colnums()
             rows = None
-            array = self._read_rec_with_var(colnums, rows, dtype,
-                                            offsets, isvar, _vstorage)
+            sortind = None
+            array = self._read_rec_with_var(
+                colnums, rows, sortind, dtype,
+                offsets, isvar, _vstorage,
+            )
         elif has_tbit:
             # drop down to read_columns since we can't stuff into a
             # contiguous array
             colnums = self._extract_colnums()
             array = self.read_columns(
                 colnums,
                 rows=None, vstorage=vstorage,
                 upper=upper, lower=lower, trim_strings=trim_strings)
         else:
             firstrow = 1  # noqa - not used?
             nrows = self._info['nrows']
-            array = numpy.zeros(nrows, dtype=dtype)
+            array = np.zeros(nrows, dtype=dtype)
 
             self._FITS.read_as_rec(self._ext+1, 1, nrows, array)
 
             array = self._maybe_decode_fits_ascii_strings_to_unicode_py3(array)
 
             for colnum, name in enumerate(array.dtype.names):
                 self._rescale_and_convert_field_inplace(
@@ -881,29 +887,30 @@
             return self._read_all()
 
         if self._info['hdutype'] == ASCII_TBL:
             return self.read(
                 rows=rows, vstorage=vstorage,
                 upper=upper, lower=lower, trim_strings=trim_strings)
 
-        rows = self._extract_rows(rows)
+        rows, sortind = self._extract_rows(rows)
         dtype, offsets, isvar = self.get_rec_dtype(vstorage=vstorage)
 
-        w, = numpy.where(isvar == True)  # noqa
+        w, = np.where(isvar == True)  # noqa
         if w.size > 0:
             if vstorage is None:
                 _vstorage = self._vstorage
             else:
                 _vstorage = vstorage
             colnums = self._extract_colnums()
             return self._read_rec_with_var(
-                colnums, rows, dtype, offsets, isvar, _vstorage)
+                colnums, rows, sortind, dtype, offsets, isvar, _vstorage,
+            )
         else:
-            array = numpy.zeros(rows.size, dtype=dtype)
-            self._FITS.read_rows_as_rec(self._ext+1, array, rows)
+            array = np.zeros(rows.size, dtype=dtype)
+            self._FITS.read_rows_as_rec(self._ext+1, array, rows, sortind)
 
             array = self._maybe_decode_fits_ascii_strings_to_unicode_py3(array)
 
             for colnum, name in enumerate(array.dtype.names):
                 self._rescale_and_convert_field_inplace(
                     array,
                     name,
@@ -966,43 +973,48 @@
         # if columns is None, returns all.  Guaranteed to be unique and sorted
         colnums = self._extract_colnums(columns)
         if isinstance(colnums, int):
             # scalar sent, don't read as a recarray
             return self.read_column(
                 columns,
                 rows=rows, vstorage=vstorage,
-                upper=upper, lower=lower, trim_strings=trim_strings)
+                upper=upper, lower=lower, trim_strings=trim_strings,
+            )
 
         # if rows is None still returns None, and is correctly interpreted
         # by the reader to mean all
-        rows = self._extract_rows(rows)
+        rows, sortind = self._extract_rows(rows)
 
         # this is the full dtype for all columns
         dtype, offsets, isvar = self.get_rec_dtype(
             colnums=colnums, vstorage=vstorage)
 
-        w, = numpy.where(isvar == True)  # noqa
+        w, = np.where(isvar == True)  # noqa
         if w.size > 0:
             if vstorage is None:
                 _vstorage = self._vstorage
             else:
                 _vstorage = vstorage
             array = self._read_rec_with_var(
-                colnums, rows, dtype, offsets, isvar, _vstorage)
+                colnums, rows, sortind, dtype, offsets, isvar, _vstorage,
+            )
         else:
 
             if rows is None:
                 nrows = self._info['nrows']
             else:
                 nrows = rows.size
-            array = numpy.zeros(nrows, dtype=dtype)
+
+            array = np.zeros(nrows, dtype=dtype)
 
             colnumsp = colnums[:].copy()
             colnumsp[:] += 1
-            self._FITS.read_columns_as_rec(self._ext+1, colnumsp, array, rows)
+            self._FITS.read_columns_as_rec(
+                self._ext+1, colnumsp, array, rows, sortind
+            )
 
             array = self._maybe_decode_fits_ascii_strings_to_unicode_py3(array)
 
             for i in xrange(colnums.size):
                 colnum = int(colnums[i])
                 name = array.dtype.names[i]
                 self._rescale_and_convert_field_inplace(
@@ -1061,47 +1073,48 @@
             import warnings
             warnings.warn(
                 "The keyword arguments '%s' are being ignored! This warning "
                 "will be an error in a future version of `fitsio`!" % keys,
                 DeprecationWarning, stacklevel=2)
 
         if self._info['hdutype'] == ASCII_TBL:
-            rows = numpy.arange(firstrow, lastrow, step, dtype='i8')
+            rows = np.arange(firstrow, lastrow, step, dtype='i8')
             return self.read_ascii(
                 rows=rows, vstorage=vstorage,
                 upper=upper, lower=lower, trim_strings=trim_strings)
 
         if self._info['hdutype'] == IMAGE_HDU:
             raise ValueError("slices currently only supported for tables")
 
         maxrow = self._info['nrows']
         if firstrow < 0 or lastrow > maxrow:
             raise ValueError(
                 "slice must specify a sub-range of [%d,%d]" % (0, maxrow))
 
         dtype, offsets, isvar = self.get_rec_dtype(vstorage=vstorage)
 
-        w, = numpy.where(isvar == True)  # noqa
+        w, = np.where(isvar == True)  # noqa
         if w.size > 0:
             if vstorage is None:
                 _vstorage = self._vstorage
             else:
                 _vstorage = vstorage
-            rows = numpy.arange(firstrow, lastrow, step, dtype='i8')
+            rows = np.arange(firstrow, lastrow, step, dtype='i8')
+            sortind = np.arange(rows.size)
             colnums = self._extract_colnums()
             array = self._read_rec_with_var(
-                colnums, rows, dtype, offsets, isvar, _vstorage)
+                colnums, rows, sortind, dtype, offsets, isvar, _vstorage)
         else:
             if step != 1:
-                rows = numpy.arange(firstrow, lastrow, step, dtype='i8')
+                rows = np.arange(firstrow, lastrow, step, dtype='i8')
                 array = self.read(rows=rows)
             else:
                 # no +1 because lastrow is non-inclusive
                 nrows = lastrow - firstrow
-                array = numpy.zeros(nrows, dtype=dtype)
+                array = np.zeros(nrows, dtype=dtype)
 
                 # only first needs to be +1.  This is becuase the c code is
                 # inclusive
                 self._FITS.read_as_rec(self._ext+1, firstrow+1, lastrow, array)
 
                 array = self._maybe_decode_fits_ascii_strings_to_unicode_py3(
                     array)
@@ -1145,22 +1158,22 @@
         else:
             _vstorage = vstorage
 
         if colnums is None:
             colnums = self._extract_colnums()
 
         descr = []
-        isvararray = numpy.zeros(len(colnums), dtype=bool)
+        isvararray = np.zeros(len(colnums), dtype=bool)
         for i, colnum in enumerate(colnums):
             dt, isvar = self.get_rec_column_descr(colnum, _vstorage)
             descr.append(dt)
             isvararray[i] = isvar
-        dtype = numpy.dtype(descr)
+        dtype = np.dtype(descr)
 
-        offsets = numpy.zeros(len(colnums), dtype='i8')
+        offsets = np.zeros(len(colnums), dtype='i8')
         for i, n in enumerate(dtype.names):
             offsets[i] = dtype.fields[n][1]
         return dtype, offsets, isvararray
 
     def _check_tbit(self, colnums=None, **keys):
         """
         Check if one of the columns is a TBIT column
@@ -1302,15 +1315,15 @@
             if shape is not None:
                 descr = (name, npy_type, shape)
             else:
                 descr = (name, npy_type)
         return descr, isvar
 
     def _read_rec_with_var(
-            self, colnums, rows, dtype, offsets, isvar, vstorage):
+            self, colnums, rows, sortind, dtype, offsets, isvar, vstorage):
         """
         Read columns from a table into a rec array, including variable length
         columns.  This is special because, for efficiency, it involves reading
         from the main table as normal but skipping the columns in the array
         that are variable.  Then reading the variable length columns, with
         accounting for strides appropriately.
 
@@ -1318,66 +1331,75 @@
         """
 
         colnumsp = colnums+1
         if rows is None:
             nrows = self._info['nrows']
         else:
             nrows = rows.size
-        array = numpy.zeros(nrows, dtype=dtype)
+        array = np.zeros(nrows, dtype=dtype)
 
         # read from the main table first
-        wnotvar, = numpy.where(isvar == False)  # noqa
+        wnotvar, = np.where(isvar == False)  # noqa
         if wnotvar.size > 0:
             # this will be contiguous (not true for slices)
             thesecol = colnumsp[wnotvar]
             theseoff = offsets[wnotvar]
-            self._FITS.read_columns_as_rec_byoffset(self._ext+1,
-                                                    thesecol,
-                                                    theseoff,
-                                                    array,
-                                                    rows)
+            self._FITS.read_columns_as_rec_byoffset(
+                self._ext+1,
+                thesecol,
+                theseoff,
+                array,
+                rows,
+                sortind,
+            )
             for i in xrange(thesecol.size):
 
                 name = array.dtype.names[wnotvar[i]]
                 colnum = thesecol[i]-1
                 self._rescale_and_convert_field_inplace(
                     array,
                     name,
                     self._info['colinfo'][colnum]['tscale'],
-                    self._info['colinfo'][colnum]['tzero'])
+                    self._info['colinfo'][colnum]['tzero'],
+                )
 
         array = self._maybe_decode_fits_ascii_strings_to_unicode_py3(array)
 
         # now read the variable length arrays we may be able to speed this up
         # by storing directly instead of reading first into a list
-        wvar, = numpy.where(isvar == True)  # noqa
+        wvar, = np.where(isvar == True)  # noqa
         if wvar.size > 0:
             # this will be contiguous (not true for slices)
             thesecol = colnumsp[wvar]
             for i in xrange(thesecol.size):
                 colnump = thesecol[i]
                 name = array.dtype.names[wvar[i]]
                 dlist = self._FITS.read_var_column_as_list(
-                    self._ext+1, colnump, rows)
+                    self._ext+1, colnump, rows, sortind,
+                )
 
                 if (isinstance(dlist[0], str) or
                         (IS_PY3 and isinstance(dlist[0], bytes))):
                     is_string = True
                 else:
                     is_string = False
 
                 if array[name].dtype.descr[0][1][1] == 'O':
                     # storing in object array
                     # get references to each, no copy made
                     for irow, item in enumerate(dlist):
+                        if sortind is not None:
+                            irow = sortind[irow]
                         if IS_PY3 and isinstance(item, bytes):
                             item = item.decode('ascii')
                         array[name][irow] = item
                 else:
                     for irow, item in enumerate(dlist):
+                        if sortind is not None:
+                            irow = sortind[irow]
                         if IS_PY3 and isinstance(item, bytes):
                             item = item.decode('ascii')
 
                         if is_string:
                             array[name][irow] = item
                         else:
                             ncopy = len(item)
@@ -1389,27 +1411,38 @@
                                 else:
                                     array[name][irow] = item
                             else:
                                 array[name][irow][0:ncopy] = item[:]
 
         return array
 
-    def _extract_rows(self, rows):
+    def _extract_rows(self, rows, sort=False):
         """
         Extract an array of rows from an input scalar or sequence
         """
         if rows is not None:
-            rows = numpy.array(rows, ndmin=1, copy=False, dtype='i8')
+            rows = np.array(rows, ndmin=1, copy=False, dtype='i8')
+            if sort:
+                rows = np.unique(rows)
+                return rows, None
+
             # returns unique, sorted
-            rows = numpy.unique(rows)
+            sortind = rows.argsort()
 
             maxrow = self._info['nrows']-1
-            if len(rows) > 0 and (rows[0] < 0 or rows[-1] > maxrow):
-                raise ValueError("rows must be in [%d,%d]" % (0, maxrow))
-        return rows
+            if rows.size > 0:
+                firstrow = rows[sortind[0]]
+                lastrow = rows[sortind[-1]]
+
+                if len(rows) > 0 and (firstrow < 0 or lastrow > maxrow):
+                    raise ValueError("rows must be in [%d,%d]" % (0, maxrow))
+        else:
+            sortind = None
+
+        return rows, sortind
 
     def _process_slice(self, arg):
         """
         process the input slice for use calling the C code
         """
         start = arg.start
         stop = arg.stop
@@ -1455,15 +1488,15 @@
         tstop = self._fix_range(stop)
         if tstart == 0 and tstop == nrows and step is None:
             # this is faster: if all fields are also requested, then a
             # single fread will be done
             return None
         if stop < start:
             raise ValueError("start is greater than stop in slice")
-        return numpy.arange(tstart, tstop, step, dtype='i8')
+        return np.arange(tstart, tstop, step, dtype='i8')
 
     def _fix_range(self, num, isslice=True):
         """
         Ensure the input is within range.
 
         If el=True, then don't treat as a slice element
         """
@@ -1506,18 +1539,18 @@
         return array
 
     def _rescale_array(self, array, scale, zero):
         """
         Scale the input array
         """
         if scale != 1.0:
-            sval = numpy.array(scale, dtype=array.dtype)
+            sval = np.array(scale, dtype=array.dtype)
             array *= sval
         if zero != 0.0:
-            zval = numpy.array(zero, dtype=array.dtype)
+            zval = np.array(zero, dtype=array.dtype)
             array += zval
 
     def _maybe_trim_strings(self, array, trim_strings=False, **keys):
         """
         if requested, trim trailing white space from
         all string fields in the input array
         """
@@ -1555,15 +1588,15 @@
 
     def _convert_bool_array(self, array):
         """
         cfitsio reads as characters 'T' and 'F' -- convert to real boolean
         If input is a fits bool, convert to numpy boolean
         """
 
-        output = (array.view(numpy.int8) == ord('T')).astype(bool)
+        output = (array.view(np.int8) == ord('T')).astype(bool)
         return output
 
     def _get_tbl_numpy_dtype(self, colnum, include_endianness=True):
         """
         Get numpy type for the input column
         """
         table_type = self._info['hdutype']
@@ -1616,15 +1649,15 @@
             [35,55,86]
             ['f1',f2',...]
         Can also be tuples or arrays.
         """
 
         flags = set()
         #
-        if isinstance(arg, (tuple, list, numpy.ndarray)):
+        if isinstance(arg, (tuple, list, np.ndarray)):
             # a sequence was entered
             if isstring(arg[0]):
                 result = arg
             else:
                 result = arg
                 flags.add('isrows')
         elif isstring(arg):
@@ -1639,33 +1672,35 @@
                 flags.add('isslice')
                 result = self._process_slice(arg)
         else:
             # a single object was entered.
             # Probably should apply some more checking on this
             result = arg
             flags.add('isrows')
-            if numpy.ndim(arg) == 0:
+            if np.ndim(arg) == 0:
                 flags.add('isscalar')
 
         return result, flags
 
-    def _read_var_column(self, colnum, rows, vstorage):
+    def _read_var_column(self, colnum, rows, sortind, vstorage):
         """
 
         first read as a list of arrays, then copy into either a fixed length
         array or an array of objects, depending on vstorage.
 
         """
 
         if IS_PY3:
             stype = bytes
         else:
             stype = str
 
-        dlist = self._FITS.read_var_column_as_list(self._ext+1, colnum+1, rows)
+        dlist = self._FITS.read_var_column_as_list(
+            self._ext+1, colnum+1, rows, sortind,
+        )
 
         if vstorage == 'fixed':
             tform = self._info['colinfo'][colnum]['tform']
             max_size = _extract_vararray_max(tform)
 
             if max_size <= 0:
                 name = self._info['colinfo'][colnum]['name']
@@ -1680,50 +1715,55 @@
                     warnings.warn(mess, FITSRuntimeWarning)
 
                 # we are forced to read this as an object array
                 return self._read_var_column(colnum, rows, 'object')
 
             if isinstance(dlist[0], stype):
                 descr = 'S%d' % max_size
-                array = numpy.fromiter(dlist, descr)
+                array = np.fromiter(dlist, descr)
                 if IS_PY3:
                     array = array.astype('U', copy=False)
             else:
                 descr = dlist[0].dtype.str
-                array = numpy.zeros((len(dlist), max_size), dtype=descr)
+                array = np.zeros((len(dlist), max_size), dtype=descr)
 
                 for irow, item in enumerate(dlist):
+                    if sortind is not None:
+                        irow = sortind[irow]
                     ncopy = len(item)
                     array[irow, 0:ncopy] = item[:]
         else:
-            array = numpy.zeros(len(dlist), dtype='O')
+            array = np.zeros(len(dlist), dtype='O')
             for irow, item in enumerate(dlist):
+                if sortind is not None:
+                    irow = sortind[irow]
+
                 if IS_PY3 and isinstance(item, bytes):
                     item = item.decode('ascii')
                 array[irow] = item
 
         return array
 
     def _extract_colnums(self, columns=None):
         """
         Extract an array of columns from the input
         """
         if columns is None:
-            return numpy.arange(self._ncol, dtype='i8')
+            return np.arange(self._ncol, dtype='i8')
 
-        if not isinstance(columns, (tuple, list, numpy.ndarray)):
+        if not isinstance(columns, (tuple, list, np.ndarray)):
             # is a scalar
             return self._extract_colnum(columns)
 
-        colnums = numpy.zeros(len(columns), dtype='i8')
+        colnums = np.zeros(len(columns), dtype='i8')
         for i in xrange(colnums.size):
             colnums[i] = self._extract_colnum(columns[i])
 
         # returns unique sorted
-        colnums = numpy.unique(colnums)
+        colnums = np.unique(colnums)
         return colnums
 
     def _extract_colnum(self, col):
         """
         Get the column number for the input column
         """
         if isinteger(col):
@@ -1965,64 +2005,69 @@
         colnums = self._extract_colnums(columns)
         if isinstance(colnums, int):
             # scalar sent, don't read as a recarray
             return self.read_column(
                 columns, rows=rows, vstorage=vstorage,
                 upper=upper, lower=lower, trim_strings=trim_strings)
 
-        rows = self._extract_rows(rows)
+        rows, sortind = self._extract_rows(rows)
         if rows is None:
             nrows = self._info['nrows']
         else:
             nrows = rows.size
 
         # if rows is None still returns None, and is correctly interpreted
         # by the reader to mean all
-        rows = self._extract_rows(rows)
+        rows, sortind = self._extract_rows(rows)
 
         # this is the full dtype for all columns
         dtype, offsets, isvar = self.get_rec_dtype(
             colnums=colnums, vstorage=vstorage)
-        array = numpy.zeros(nrows, dtype=dtype)
+        array = np.zeros(nrows, dtype=dtype)
 
         # note reading into existing data
-        wnotvar, = numpy.where(isvar == False)  # noqa
+        wnotvar, = np.where(isvar == False)  # noqa
         if wnotvar.size > 0:
             for i in wnotvar:
                 colnum = colnums[i]
                 name = array.dtype.names[i]
                 a = array[name].copy()
-                self._FITS.read_column(self._ext+1, colnum+1, a, rows)
+                self._FITS.read_column(self._ext+1, colnum+1, a, rows, sortind)
                 array[name] = a
                 del a
 
         array = self._maybe_decode_fits_ascii_strings_to_unicode_py3(array)
 
-        wvar, = numpy.where(isvar == True)  # noqa
+        wvar, = np.where(isvar == True)  # noqa
         if wvar.size > 0:
             for i in wvar:
                 colnum = colnums[i]
                 name = array.dtype.names[i]
                 dlist = self._FITS.read_var_column_as_list(
-                    self._ext+1, colnum+1, rows)
+                    self._ext+1, colnum+1, rows, sortind,
+                )
                 if (isinstance(dlist[0], str) or
                         (IS_PY3 and isinstance(dlist[0], bytes))):
                     is_string = True
                 else:
                     is_string = False
 
                 if array[name].dtype.descr[0][1][1] == 'O':
                     # storing in object array
                     # get references to each, no copy made
                     for irow, item in enumerate(dlist):
+                        if sortind is not None:
+                            irow = sortind[irow]
                         if IS_PY3 and isinstance(item, bytes):
                             item = item.decode('ascii')
                         array[name][irow] = item
                 else:
                     for irow, item in enumerate(dlist):
+                        if sortind is not None:
+                            irow = sortind[irow]
                         if IS_PY3 and isinstance(item, bytes):
                             item = item.decode('ascii')
                         if is_string:
                             array[name][irow] = item
                         else:
                             ncopy = len(item)
                             array[name][irow][0:ncopy] = item[:]
@@ -2248,18 +2293,18 @@
 
 def _trim_strings(data):
     names = data.dtype.names
     if names is not None:
         # run through each field separately
         for n in names:
             if data[n].dtype.descr[0][1][1] in ['S', 'U']:
-                data[n] = numpy.char.rstrip(data[n])
+                data[n] = np.char.rstrip(data[n])
     else:
         if data.dtype.descr[0][1][1] in ['S', 'U']:
-            data[:] = numpy.char.rstrip(data[:])
+            data[:] = np.char.rstrip(data[:])
 
 
 def _extract_vararray_max(tform):
     """
     Extract number from PX(number)
     """
     first = tform.find('(')
```

### Comparing `fitsio-1.1.8/fitsio/header.py` & `fitsio-1.1.9/fitsio/header.py`

 * *Files identical despite different names*

### Comparing `fitsio-1.1.8/fitsio/test_images/test_gzip_compressed_image.fits.fz` & `fitsio-1.1.9/fitsio/test_images/test_gzip_compressed_image.fits.fz`

 * *Files identical despite different names*

### Comparing `fitsio-1.1.8/fitsio/util.py` & `fitsio-1.1.9/fitsio/util.py`

 * *Files identical despite different names*

### Comparing `fitsio-1.1.8/fitsio.egg-info/PKG-INFO` & `fitsio-1.1.9/fitsio.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: fitsio
-Version: 1.1.8
+Version: 1.1.9
 Summary: A full featured python library to read from and write to FITS files.
 Home-page: https://github.com/esheldon/fitsio
 Author: Erin Scott Sheldon
 Author-email: erin.sheldon@gmail.com
 License: GPL
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: Intended Audience :: Science/Research
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 License-File: LICENSE.txt
 
@@ -83,19 +82,14 @@
 
 # Write an image to the same file. By default a new extension is
 # added to the file.  use clobber=True to overwrite an existing file
 # instead.  To append rows to an existing table, see below.
 
 fitsio.write(filename, image)
 
-# NOTE when reading row subsets, the data must still be read from disk.
-# This is most efficient if the data are read in the order they appear in
-# the file.  For this reason, the rows are always returned in row-sorted
-# order.
-
 #
 # the FITS class gives the you the ability to explore the data, and gives
 # more control
 #
 
 # open a FITS file for reading and explore
 fits=fitsio.FITS('data.fits')
@@ -190,18 +184,22 @@
 # all rows of column 'x'
 data = fits[1]['x'][:]
 
 # Read a few columns at once. This is more efficient than separate read for
 # each column
 data = fits[1]['x','y'][:]
 
-# General column and row subsets.  As noted above, the data are returned
-# in row sorted order for efficiency reasons.
+# General column and row subsets.
 columns=['index','x','y']
-rows=[1,5]
+rows = [1, 5]
+data = fits[1][columns][rows]
+
+# data are returned in the order requested by the user
+# and duplicates are preserved
+rows = [2, 2, 5]
 data = fits[1][columns][rows]
 
 # iterate over rows in a table hdu
 # faster if we buffer some rows, let's buffer 1000 at a time
 fits=fitsio.FITS(filename,iter_row_buffer=1000)
 for row in fits[1]:
     print(row)
@@ -441,15 +439,15 @@
 
 
 ## Tests
 
 The unit tests should all pass for full support.
 
 ```bash
-python -c "import fitsio; fitsio.test.test()"
+pytest fitsio
 ```
 
 Some tests may fail if certain libraries are not available, such
 as bzip2.  This failure only implies that bzipped files cannot
 be read, without affecting other functionality.
 
 ## Notes on Usage and Features
@@ -485,9 +483,7 @@
 in Python 3 will now come back as a string and not a byte string. Note that this
 support is not the same as full unicode support. Internally, fitsio only supports
 the ASCII character set.
 
 ## TODO
 
 - HDU groups: does anyone use these? If so open an issue!
-
-
```

### Comparing `fitsio-1.1.8/patches/README.md` & `fitsio-1.1.9/patches/README.md`

 * *Files identical despite different names*

### Comparing `fitsio-1.1.8/patches/build_cfitsio_patches.py` & `fitsio-1.1.9/patches/build_cfitsio_patches.py~`

 * *Files identical despite different names*

### Comparing `fitsio-1.1.8/patches/configure.in.patch` & `fitsio-1.1.9/patches/configure.in.patch`

 * *Files identical despite different names*

### Comparing `fitsio-1.1.8/patches/configure.patch` & `fitsio-1.1.9/patches/configure.patch`

 * *Files identical despite different names*

### Comparing `fitsio-1.1.8/patches/fitscore.c.patch` & `fitsio-1.1.9/patches/fitscore.c.patch`

 * *Files identical despite different names*

### Comparing `fitsio-1.1.8/patches/putcols.c.patch` & `fitsio-1.1.9/patches/putcols.c.patch`

 * *Files identical despite different names*

### Comparing `fitsio-1.1.8/setup.py` & `fitsio-1.1.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -263,15 +263,15 @@
     "License :: OSI Approved :: GNU General Public License (GPL)",
     "Topic :: Scientific/Engineering :: Astronomy",
     "Intended Audience :: Science/Research",
 ]
 
 setup(
     name="fitsio",
-    version="1.1.8",
+    version="1.1.9",
     description=description,
     long_description=long_description,
     long_description_content_type='text/markdown; charset=UTF-8; variant=GFM',
     license="GPL",
     classifiers=classifiers,
     url="https://github.com/esheldon/fitsio",
     author="Erin Scott Sheldon",
```

