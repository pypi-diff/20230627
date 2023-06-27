# Comparing `tmp/xcoll-0.2.2.tar.gz` & `tmp/xcoll-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xcoll-0.2.2.tar", max compression
+gzip compressed data, was "xcoll-0.2.3.tar", max compression
```

## Comparing `xcoll-0.2.2.tar` & `xcoll-0.2.3.tar`

### file list

```diff
@@ -1,31 +1,103 @@
--rw-r--r--   0        0        0    11357 2023-01-26 20:47:21.412402 xcoll-0.2.2/LICENSE
--rw-r--r--   0        0        0       74 2023-01-26 20:47:21.413402 xcoll-0.2.2/NOTICE
--rw-r--r--   0        0        0     1713 2023-06-15 15:54:59.927458 xcoll-0.2.2/README.md
--rw-r--r--   0        0        0     1008 2023-06-15 15:54:59.927458 xcoll-0.2.2/pyproject.toml
--rw-r--r--   0        0        0      392 2023-06-15 15:54:59.928458 xcoll-0.2.2/xcoll/__init__.py
--rw-r--r--   0        0        0      224 2023-06-13 14:41:23.114175 xcoll-0.2.2/xcoll/beam_elements/__init__.py
--rw-r--r--   0        0        0     1248 2023-06-13 14:41:23.114175 xcoll-0.2.2/xcoll/beam_elements/absorber.py
--rw-r--r--   0        0        0    14594 2023-06-13 14:41:23.115175 xcoll-0.2.2/xcoll/beam_elements/base_collimator.py
--rw-r--r--   0        0        0     8600 2023-06-15 15:54:59.928458 xcoll-0.2.2/xcoll/beam_elements/collimators_src/absorber.h
--rw-r--r--   0        0        0      413 2023-06-13 14:41:23.115175 xcoll-0.2.2/xcoll/beam_elements/collimators_src/base_collimator.h
--rw-r--r--   0        0        0     3774 2023-06-15 15:54:59.928458 xcoll-0.2.2/xcoll/beam_elements/collimators_src/everest_collimator.h
--rw-r--r--   0        0        0     4672 2023-06-15 15:54:59.928458 xcoll-0.2.2/xcoll/beam_elements/collimators_src/everest_crystal.h
--rw-r--r--   0        0        0      433 2023-06-13 14:41:23.115175 xcoll-0.2.2/xcoll/beam_elements/collimators_src/invalid_collimator.h
--rw-r--r--   0        0        0     6559 2023-06-13 14:41:23.115175 xcoll-0.2.2/xcoll/beam_elements/everest_collimator.py
--rw-r--r--   0        0        0    39298 2023-06-13 14:41:23.115175 xcoll-0.2.2/xcoll/colldb.py
--rw-r--r--   0        0        0    17015 2023-06-13 14:41:23.116175 xcoll-0.2.2/xcoll/collimator_settings.py
--rw-r--r--   0        0        0       71 2023-04-01 09:07:08.962808 xcoll-0.2.2/xcoll/general.py
--rw-r--r--   0        0        0      639 2023-06-13 14:41:23.116175 xcoll-0.2.2/xcoll/headers/particle_states.h
--rw-r--r--   0        0        0    43926 2023-06-13 14:41:23.116175 xcoll-0.2.2/xcoll/manager.py
--rw-r--r--   0        0        0       84 2023-06-15 14:24:13.343504 xcoll-0.2.2/xcoll/scattering_routines/everest/__init__.py
--rw-r--r--   0        0        0    53426 2023-06-13 14:41:23.116175 xcoll-0.2.2/xcoll/scattering_routines/everest/crystal.h
--rw-r--r--   0        0        0     1059 2023-06-13 14:41:23.117175 xcoll-0.2.2/xcoll/scattering_routines/everest/everest.h
--rw-r--r--   0        0        0      970 2023-06-15 14:24:13.343504 xcoll-0.2.2/xcoll/scattering_routines/everest/everest.py
--rw-r--r--   0        0        0    12414 2023-06-13 14:41:23.117175 xcoll-0.2.2/xcoll/scattering_routines/everest/jaw.h
--rw-r--r--   0        0        0     8742 2023-06-13 14:41:23.117175 xcoll-0.2.2/xcoll/scattering_routines/everest/materials.py
--rw-r--r--   0        0        0    10362 2023-06-13 14:41:23.117175 xcoll-0.2.2/xcoll/scattering_routines/everest/scatter.h
--rw-r--r--   0        0        0     9368 2023-06-13 14:41:23.117175 xcoll-0.2.2/xcoll/scattering_routines/everest/scatter_crystal.h
--rw-r--r--   0        0        0     2863 2023-06-13 14:41:23.117175 xcoll-0.2.2/xcoll/scattering_routines/everest/scatter_init.h
--rw-r--r--   0        0        0     1919 2023-04-01 09:07:08.965808 xcoll-0.2.2/xcoll/tables.py
--rw-r--r--   0        0        0     2807 1970-01-01 00:00:00.000000 xcoll-0.2.2/setup.py
--rw-r--r--   0        0        0     2733 1970-01-01 00:00:00.000000 xcoll-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-01-26 20:47:21.412402 xcoll-0.2.3/LICENSE
+-rw-r--r--   0        0        0       74 2023-01-26 20:47:21.413402 xcoll-0.2.3/NOTICE
+-rw-r--r--   0        0        0     1713 2023-06-16 17:31:39.044273 xcoll-0.2.3/README.md
+-rw-r--r--   0        0        0      996 2023-06-27 18:36:04.026456 xcoll-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0      325 2023-06-27 18:36:04.026456 xcoll-0.2.3/xcoll/__init__.py
+-rw-r--r--   0        0        0      224 2023-06-13 14:41:23.114175 xcoll-0.2.3/xcoll/beam_elements/__init__.py
+-rw-r--r--   0        0        0     1248 2023-06-13 14:41:23.114175 xcoll-0.2.3/xcoll/beam_elements/absorber.py
+-rw-r--r--   0        0        0    14594 2023-06-13 14:41:23.115175 xcoll-0.2.3/xcoll/beam_elements/base_collimator.py
+-rw-r--r--   0        0        0     8600 2023-06-16 17:31:39.046273 xcoll-0.2.3/xcoll/beam_elements/collimators_src/absorber.h
+-rw-r--r--   0        0        0      413 2023-06-13 14:41:23.115175 xcoll-0.2.3/xcoll/beam_elements/collimators_src/base_collimator.h
+-rw-r--r--   0        0        0     4026 2023-06-27 18:36:04.026456 xcoll-0.2.3/xcoll/beam_elements/collimators_src/everest_collimator.h
+-rw-r--r--   0        0        0     5177 2023-06-27 18:36:04.026456 xcoll-0.2.3/xcoll/beam_elements/collimators_src/everest_crystal.h
+-rw-r--r--   0        0        0      433 2023-06-13 14:41:23.115175 xcoll-0.2.3/xcoll/beam_elements/collimators_src/invalid_collimator.h
+-rw-r--r--   0        0        0     6986 2023-06-27 18:36:04.027456 xcoll-0.2.3/xcoll/beam_elements/everest_collimator.py
+-rw-r--r--   0        0        0    39298 2023-06-13 14:41:23.115175 xcoll-0.2.3/xcoll/colldb.py
+-rw-r--r--   0        0        0    17015 2023-06-13 14:41:23.116175 xcoll-0.2.3/xcoll/collimator_settings.py
+-rw-r--r--   0        0        0       71 2023-04-01 09:07:08.962808 xcoll-0.2.3/xcoll/general.py
+-rw-r--r--   0        0        0      639 2023-06-13 14:41:23.116175 xcoll-0.2.3/xcoll/headers/particle_states.h
+-rw-r--r--   0        0        0    43926 2023-06-13 14:41:23.116175 xcoll-0.2.3/xcoll/manager.py
+-rw-r--r--   0        0        0      101 2023-06-27 18:36:04.027456 xcoll-0.2.3/xcoll/scattering_routines/everest/__init__.py
+-rw-r--r--   0        0        0    54119 2023-06-27 18:36:04.027456 xcoll-0.2.3/xcoll/scattering_routines/everest/crystal.h
+-rw-r--r--   0        0        0     1059 2023-06-13 14:41:23.117175 xcoll-0.2.3/xcoll/scattering_routines/everest/everest.h
+-rw-r--r--   0        0        0      970 2023-06-26 15:53:03.238534 xcoll-0.2.3/xcoll/scattering_routines/everest/everest.py
+-rw-r--r--   0        0        0    12673 2023-06-27 18:36:04.027456 xcoll-0.2.3/xcoll/scattering_routines/everest/jaw.h
+-rw-r--r--   0        0        0     8742 2023-06-13 14:41:23.117175 xcoll-0.2.3/xcoll/scattering_routines/everest/materials.py
+-rw-r--r--   0        0        0    10392 2023-06-27 18:36:04.027456 xcoll-0.2.3/xcoll/scattering_routines/everest/scatter.h
+-rw-r--r--   0        0        0     9455 2023-06-27 18:36:04.027456 xcoll-0.2.3/xcoll/scattering_routines/everest/scatter_crystal.h
+-rw-r--r--   0        0        0     2863 2023-06-13 14:41:23.117175 xcoll-0.2.3/xcoll/scattering_routines/everest/scatter_init.h
+-rw-r--r--   0        0        0       73 2023-06-16 17:47:08.025919 xcoll-0.2.3/xcoll/scattering_routines/fluka/flukaio/.git
+-rw-r--r--   0        0        0       12 2023-06-16 17:47:08.027918 xcoll-0.2.3/xcoll/scattering_routines/fluka/flukaio/.gitignore
+-rw-r--r--   0        0        0      591 2023-06-16 17:47:08.027918 xcoll-0.2.3/xcoll/scattering_routines/fluka/flukaio/CMakeLists.txt
+-rw-r--r--   0        0        0     5951 2023-06-16 17:47:08.027918 xcoll-0.2.3/xcoll/scattering_routines/fluka/flukaio/ComponentMakefile
+-rw-r--r--   0        0        0     3404 2023-06-16 17:47:08.027918 xcoll-0.2.3/xcoll/scattering_routines/fluka/flukaio/Makefile
+-rw-r--r--   0        0        0      611 2023-06-16 17:47:08.027918 xcoll-0.2.3/xcoll/scattering_routines/fluka/flukaio/README
+-rw-r--r--   0        0        0    65455 2023-06-16 17:47:08.028919 xcoll-0.2.3/xcoll/scattering_routines/fluka/flukaio/doc/Doxyfile
+-rw-r--r--   0        0        0    45517 2023-06-16 17:47:08.028919 xcoll-0.2.3/xcoll/scattering_routines/fluka/flukaio/doc/FlukaIO.asciidoc
+-rw-r--r--   0        0        0   138089 2023-06-16 17:47:08.028919 xcoll-0.2.3/xcoll/scattering_routines/fluka/flukaio/doc/FlukaIO.epub
+-rw-r--r--   0        0        0    74567 2023-06-16 17:47:08.028919 xcoll-0.2.3/xcoll/scattering_routines/fluka/flukaio/doc/FlukaIO.html
+-rw-r--r--   0        0        0   233955 2023-06-16 17:47:08.029919 xcoll-0.2.3/xcoll/scattering_routines/fluka/flukaio/doc/FlukaIO.pdf
+-rw-r--r--   0        0        0    36021 2023-06-16 17:47:08.029919 xcoll-0.2.3/xcoll/scattering_routines/fluka/flukaio/doc/FlukaIO__1.png
+-rw-r--r--   0        0        0     2904 2023-06-16 17:47:08.030918 xcoll-0.2.3/xcoll/scattering_routines/fluka/flukaio/doc/FlukaIO__2.png
+-rw-r--r--   0        0        0    23826 2023-06-16 17:47:08.030918 xcoll-0.2.3/xcoll/scattering_routines/fluka/flukaio/doc/FlukaIO__3.png
+-rw-r--r--   0        0        0     3956 2023-06-16 17:47:08.030918 xcoll-0.2.3/xcoll/scattering_routines/fluka/flukaio/doc/FlukaIO__4.png
+-rw-r--r--   0        0        0     7017 2023-06-16 17:47:08.030918 xcoll-0.2.3/xcoll/scattering_routines/fluka/flukaio/doc/FlukaIO__5.png
+-rw-r--r--   0        0        0    33614 2023-06-16 17:47:08.030918 xcoll-0.2.3/xcoll/scattering_routines/fluka/flukaio/doc/FlukaIO__6.png
+-rw-r--r--   0        0        0    51182 2023-06-16 17:47:08.030918 xcoll-0.2.3/xcoll/scattering_routines/fluka/flukaio/doc/FlukaIO__7.png
+-rw-r--r--   0        0        0      146 2023-06-16 17:47:08.030918 xcoll-0.2.3/xcoll/scattering_routines/fluka/flukaio/doc/Makefile
+-rw-r--r--   0        0        0    74068 2023-06-16 17:47:08.030918 xcoll-0.2.3/xcoll/scattering_routines/fluka/flukaio/doc/docbook.xsl
+-rw-r--r--   0        0        0     2793 2023-06-16 17:47:08.030918 xcoll-0.2.3/xcoll/scattering_routines/fluka/flukaio/include/Connection.h
+-rw-r--r--   0        0        0     1976 2023-06-16 17:47:08.030918 xcoll-0.2.3/xcoll/scattering_routines/fluka/flukaio/include/FlukaIO.h
+-rw-r--r--   0        0        0      757 2023-06-16 17:47:08.031918 xcoll-0.2.3/xcoll/scattering_routines/fluka/flukaio/include/FlukaIOServer.h
+-rw-r--r--   0        0        0     5954 2023-06-16 17:47:08.031918 xcoll-0.2.3/xcoll/scattering_routines/fluka/flukaio/include/FortranFlukaIO.h
+-rw-r--r--   0        0        0     1731 2023-06-16 17:47:08.031918 xcoll-0.2.3/xcoll/scattering_routines/fluka/flukaio/include/Message.h
+-rw-r--r--   0        0        0     1328 2023-06-16 17:47:08.031918 xcoll-0.2.3/xcoll/scattering_routines/fluka/flukaio/include/ParticleInfo.h
+-rw-r--r--   0        0        0    98764 2023-06-16 17:50:44.547202 xcoll-0.2.3/xcoll/scattering_routines/fluka/flukaio/lib/libFlukaIO64.a
+-rwxr-xr-x   0        0        0    64288 2023-06-16 17:50:44.566202 xcoll-0.2.3/xcoll/scattering_routines/fluka/flukaio/lib/libFlukaIO64.so
+-rw-r--r--   0        0        0     2907 2023-06-16 17:47:08.031918 xcoll-0.2.3/xcoll/scattering_routines/fluka/flukaio/samples/ClientTest.c
+-rw-r--r--   0        0        0     2330 2023-06-16 17:47:08.031918 xcoll-0.2.3/xcoll/scattering_routines/fluka/flukaio/samples/ServerTest.c
+-rw-r--r--   0        0        0     3629 2023-06-16 17:47:08.031918 xcoll-0.2.3/xcoll/scattering_routines/fluka/flukaio/samples/fclient.f
+-rw-r--r--   0        0        0     2995 2023-06-16 17:47:08.031918 xcoll-0.2.3/xcoll/scattering_routines/fluka/flukaio/samples/fserver.f
+-rw-r--r--   0        0        0     5769 2023-06-16 17:47:08.031918 xcoll-0.2.3/xcoll/scattering_routines/fluka/flukaio/src/Connection.c
+-rw-r--r--   0        0        0     3078 2023-06-16 17:50:44.253205 xcoll-0.2.3/xcoll/scattering_routines/fluka/flukaio/src/Connection.d
+-rw-r--r--   0        0        0    15432 2023-06-16 17:50:44.291205 xcoll-0.2.3/xcoll/scattering_routines/fluka/flukaio/src/Connection.o
+-rw-r--r--   0        0        0     4804 2023-06-16 17:47:08.031918 xcoll-0.2.3/xcoll/scattering_routines/fluka/flukaio/src/FlukaIO.c
+-rw-r--r--   0        0        0     2308 2023-06-16 17:50:44.307204 xcoll-0.2.3/xcoll/scattering_routines/fluka/flukaio/src/FlukaIO.d
+-rw-r--r--   0        0        0    14808 2023-06-16 17:50:44.337204 xcoll-0.2.3/xcoll/scattering_routines/fluka/flukaio/src/FlukaIO.o
+-rw-r--r--   0        0        0     1541 2023-06-16 17:47:08.031918 xcoll-0.2.3/xcoll/scattering_routines/fluka/flukaio/src/FlukaIOHandshake.c
+-rw-r--r--   0        0        0     1598 2023-06-16 17:50:44.351204 xcoll-0.2.3/xcoll/scattering_routines/fluka/flukaio/src/FlukaIOHandshake.d
+-rw-r--r--   0        0        0      288 2023-06-16 17:47:08.031918 xcoll-0.2.3/xcoll/scattering_routines/fluka/flukaio/src/FlukaIOHandshake.h
+-rw-r--r--   0        0        0     9064 2023-06-16 17:50:44.372204 xcoll-0.2.3/xcoll/scattering_routines/fluka/flukaio/src/FlukaIOHandshake.o
+-rw-r--r--   0        0        0     1925 2023-06-16 17:47:08.031918 xcoll-0.2.3/xcoll/scattering_routines/fluka/flukaio/src/FlukaIOServer.c
+-rw-r--r--   0        0        0     3159 2023-06-16 17:50:44.391204 xcoll-0.2.3/xcoll/scattering_routines/fluka/flukaio/src/FlukaIOServer.d
+-rw-r--r--   0        0        0     8416 2023-06-16 17:50:44.422204 xcoll-0.2.3/xcoll/scattering_routines/fluka/flukaio/src/FlukaIOServer.o
+-rw-r--r--   0        0        0      396 2023-06-16 17:47:08.031918 xcoll-0.2.3/xcoll/scattering_routines/fluka/flukaio/src/FlukaIOServer_private.h
+-rw-r--r--   0        0        0      421 2023-06-16 17:47:08.031918 xcoll-0.2.3/xcoll/scattering_routines/fluka/flukaio/src/FlukaIO_private.h
+-rw-r--r--   0        0        0    11512 2023-06-16 17:47:08.031918 xcoll-0.2.3/xcoll/scattering_routines/fluka/flukaio/src/FortranFlukaIO.c
+-rw-r--r--   0        0        0     2134 2023-06-16 17:50:44.437204 xcoll-0.2.3/xcoll/scattering_routines/fluka/flukaio/src/FortranFlukaIO.d
+-rw-r--r--   0        0        0    29088 2023-06-16 17:50:44.480203 xcoll-0.2.3/xcoll/scattering_routines/fluka/flukaio/src/FortranFlukaIO.o
+-rw-r--r--   0        0        0     6361 2023-06-16 17:47:08.031918 xcoll-0.2.3/xcoll/scattering_routines/fluka/flukaio/src/NetIO.c
+-rw-r--r--   0        0        0     2973 2023-06-16 17:50:44.500203 xcoll-0.2.3/xcoll/scattering_routines/fluka/flukaio/src/NetIO.d
+-rw-r--r--   0        0        0      902 2023-06-16 17:47:08.031918 xcoll-0.2.3/xcoll/scattering_routines/fluka/flukaio/src/NetIO.h
+-rw-r--r--   0        0        0    19936 2023-06-16 17:50:44.538203 xcoll-0.2.3/xcoll/scattering_routines/fluka/flukaio/src/NetIO.o
+-rw-r--r--   0        0        0    14484 2023-06-16 17:47:08.031918 xcoll-0.2.3/xcoll/scattering_routines/fluka/flukaio/src/tags
+-rw-r--r--   0        0        0      166 2023-06-16 17:47:08.031918 xcoll-0.2.3/xcoll/scattering_routines/fluka/flukaio/tests/AllTests.cpp
+-rw-r--r--   0        0        0      152 2023-06-16 17:47:08.031918 xcoll-0.2.3/xcoll/scattering_routines/fluka/flukaio/tests/CommonTest.h
+-rw-r--r--   0        0        0     2464 2023-06-16 17:47:08.031918 xcoll-0.2.3/xcoll/scattering_routines/fluka/flukaio/tests/ConnectionTest.cpp
+-rw-r--r--   0        0        0     1851 2023-06-16 17:47:08.031918 xcoll-0.2.3/xcoll/scattering_routines/fluka/flukaio/tests/FlukaIOServerTest.cpp
+-rw-r--r--   0        0        0    11293 2023-06-16 17:47:08.031918 xcoll-0.2.3/xcoll/scattering_routines/fluka/flukaio/tests/FlukaIOTest.cpp
+-rw-r--r--   0        0        0    14331 2023-06-16 17:47:08.031918 xcoll-0.2.3/xcoll/scattering_routines/fluka/flukaio/tests/FortranFlukaIOTest.cpp
+-rw-r--r--   0        0        0      526 2023-06-16 17:47:08.032919 xcoll-0.2.3/xcoll/scattering_routines/fluka/flukaio/tests/fakes/FakeConnection.c
+-rw-r--r--   0        0        0      226 2023-06-16 17:47:08.032919 xcoll-0.2.3/xcoll/scattering_routines/fluka/flukaio/tests/fakes/FakeConnection.h
+-rw-r--r--   0        0        0     2244 2023-06-16 17:47:08.032919 xcoll-0.2.3/xcoll/scattering_routines/fluka/flukaio/tests/fakes/FakeFlukaIO.c
+-rw-r--r--   0        0        0     1660 2023-06-16 17:47:08.032919 xcoll-0.2.3/xcoll/scattering_routines/fluka/flukaio/tests/fakes/FakeFlukaIO.h
+-rw-r--r--   0        0        0      549 2023-06-16 17:47:08.032919 xcoll-0.2.3/xcoll/scattering_routines/fluka/flukaio/tests/fakes/FakeFlukaIOHandshake.c
+-rw-r--r--   0        0        0      395 2023-06-16 17:47:08.032919 xcoll-0.2.3/xcoll/scattering_routines/fluka/flukaio/tests/fakes/FakeFlukaIOHandshake.h
+-rw-r--r--   0        0        0      360 2023-06-16 17:47:08.032919 xcoll-0.2.3/xcoll/scattering_routines/fluka/flukaio/tests/fakes/FakeFlukaIOServer.c
+-rw-r--r--   0        0        0      280 2023-06-16 17:47:08.032919 xcoll-0.2.3/xcoll/scattering_routines/fluka/flukaio/tests/fakes/FakeFlukaIOServer.h
+-rw-r--r--   0        0        0      330 2023-06-16 17:47:08.032919 xcoll-0.2.3/xcoll/scattering_routines/fluka/flukaio/tests/fakes/FakeFortranFlukaIO.h
+-rw-r--r--   0        0        0     1452 2023-06-16 17:47:08.032919 xcoll-0.2.3/xcoll/scattering_routines/fluka/flukaio/tests/fakes/FakeNetIO.c
+-rw-r--r--   0        0        0      906 2023-06-16 17:47:08.032919 xcoll-0.2.3/xcoll/scattering_routines/fluka/flukaio/tests/fakes/FakeNetIO.h
+-rw-r--r--   0        0        0     1919 2023-04-01 09:07:08.965808 xcoll-0.2.3/xcoll/tables.py
+-rw-r--r--   0        0        0     3191 1970-01-01 00:00:00.000000 xcoll-0.2.3/setup.py
+-rw-r--r--   0        0        0     2657 1970-01-01 00:00:00.000000 xcoll-0.2.3/PKG-INFO
```

### Comparing `xcoll-0.2.2/LICENSE` & `xcoll-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `xcoll-0.2.2/README.md` & `xcoll-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `xcoll-0.2.2/pyproject.toml` & `xcoll-0.2.3/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "xcoll"
-version = "0.2.2"
+version = "0.2.3"
 description = "Xsuite collimation package"
 homepage = "https://github.com/xsuite/xcoll"
 repository = "https://github.com/xsuite/xcoll"
 authors = [
            "Frederik F. Van der Veken <frederik@cern.ch>",
            "Despina Demetriadou <despina.demetriadou@cern.ch>",
            "Andrey Abramov <andrey.abramov@cern.ch>",
@@ -16,20 +16,19 @@
 
 
 [tool.poetry.dependencies]
 python = ">=3.8"
 ruamel-yaml = { version = "^0.17.31", optional = true }
 numpy = ">=1.0"
 pandas = ">=1.4"
-xobjects = "^0.2.6"
-xdeps = "^0.1.1"
-xpart = "^0.15.0"
-xtrack = "^0.36.5"
-xfields = "^0.12.1"
-xcoll = "^0.2.1"
+xobjects = ">=0.2.6"
+xdeps = ">=0.1.1"
+xpart = ">=0.15.0"
+xtrack = ">=0.36.5"
+xfields = ">=0.12.1"
 
 [tool.poetry.dev-dependencies]
 pytest = ">=7.3"
 
 [tool.poetry.extras]
 tests = ["pytest", "ruamel-yaml"]
```

### Comparing `xcoll-0.2.2/xcoll/beam_elements/absorber.py` & `xcoll-0.2.3/xcoll/beam_elements/absorber.py`

 * *Files identical despite different names*

### Comparing `xcoll-0.2.2/xcoll/beam_elements/base_collimator.py` & `xcoll-0.2.3/xcoll/beam_elements/base_collimator.py`

 * *Files identical despite different names*

### Comparing `xcoll-0.2.2/xcoll/beam_elements/collimators_src/absorber.h` & `xcoll-0.2.3/xcoll/beam_elements/collimators_src/absorber.h`

 * *Files identical despite different names*

### Comparing `xcoll-0.2.2/xcoll/beam_elements/collimators_src/everest_collimator.h` & `xcoll-0.2.3/xcoll/beam_elements/collimators_src/everest_collimator.h`

 * *Files 6% similar despite different names*

```diff
@@ -4,26 +4,31 @@
 // ######################################### #
 
 #ifndef XCOLL_EVEREST_H
 #define XCOLL_EVEREST_H
 #include <math.h>
 #include <stdio.h>
 
+/*gpufun*/
+void EverestCollimator_set_material(EverestCollimatorData el, LocalParticle* part0){
+    MaterialData material = EverestCollimatorData_getp__material(el);
+    RandomRutherfordData rng = EverestCollimatorData_getp_rutherford_rng(el);
+    RandomRutherford_set_by_xcoll_material(rng, (GeneralMaterialData) material);
+}
 
 /*gpufun*/
 void EverestCollimator_track_local_particle(EverestCollimatorData el, LocalParticle* part0) {
     int8_t active = EverestCollimatorData_get_active(el);
     active       *= EverestCollimatorData_get__tracking(el);
     double const inactive_front = EverestCollimatorData_get_inactive_front(el);
     double const active_length  = EverestCollimatorData_get_active_length(el);
     double const inactive_back  = EverestCollimatorData_get_inactive_back(el);
 
     MaterialData material = EverestCollimatorData_getp__material(el);
     RandomRutherfordData rng = EverestCollimatorData_getp_rutherford_rng(el);
-    RandomRutherford_set_by_xcoll_material(rng, (GeneralMaterialData) material);
 
     // Collimator properties
     double const length     = EverestCollimatorData_get_active_length(el);
     double const co_x       = EverestCollimatorData_get_ref_x(el);
     double const co_y       = EverestCollimatorData_get_ref_y(el);
     // TODO: use xtrack C-code for rotation element
     // TODO: we are ignoring the angle of the right jaw
@@ -44,18 +49,18 @@
         if (!active){
             // Drift full length
             Drift_single_particle(part, inactive_front+active_length+inactive_back);
 
         } else {
             // Check collimator initialisation
             int8_t is_tracking = assert_tracking(part, XC_ERR_INVALID_TRACK);
-            int8_t rng_set     = assert_rng_set(part, RNG_ERR_SEEDS_NOT_SET);
-            int8_t ruth_set    = assert_rutherford_set(rng, part, RNG_ERR_RUTH_NOT_SET);
+            int8_t rng_is_set  = assert_rng_set(part, RNG_ERR_SEEDS_NOT_SET);
+            int8_t ruth_is_set = assert_rutherford_set(rng, part, RNG_ERR_RUTH_NOT_SET);
 
-            if (is_tracking && rng_set && ruth_set) {
+            if (is_tracking && rng_is_set && ruth_is_set) {
                 // Drift inactive front
                 Drift_single_particle(part, inactive_front);
 
                 // Scattering parameters
                 double const energy0 = LocalParticle_get_energy0(part) / 1e9; // Reference energy in GeV
                 struct ScatteringParameters scat = calculate_scattering(energy0, material);
```

### Comparing `xcoll-0.2.2/xcoll/beam_elements/collimators_src/everest_crystal.h` & `xcoll-0.2.3/xcoll/beam_elements/collimators_src/everest_crystal.h`

 * *Files 5% similar despite different names*

```diff
@@ -5,25 +5,32 @@
 
 #ifndef XCOLL_EVEREST_CRYSTAL_H
 #define XCOLL_EVEREST_CRYSTAL_H
 #include <math.h>
 #include <stdio.h>
 
 
+
+/*gpufun*/
+void EverestCrystal_set_material(EverestCrystalData el, LocalParticle* part0){
+    CrystalMaterialData material = EverestCrystalData_getp__material(el);
+    RandomRutherfordData rng = EverestCrystalData_getp_rutherford_rng(el);
+    RandomRutherford_set_by_xcoll_material(rng, (GeneralMaterialData) material);
+}
+
 /*gpufun*/
 void EverestCrystal_track_local_particle(EverestCrystalData el, LocalParticle* part0) {
     int8_t active      = EverestCrystalData_get_active(el);
     active            *= EverestCrystalData_get__tracking(el);
     double const inactive_front = EverestCrystalData_get_inactive_front(el);
     double const active_length  = EverestCrystalData_get_active_length(el);
     double const inactive_back  = EverestCrystalData_get_inactive_back(el);
 
     CrystalMaterialData material = EverestCrystalData_getp__material(el);
     RandomRutherfordData rng = EverestCrystalData_getp_rutherford_rng(el);
-    RandomRutherford_set_by_xcoll_material(rng, (GeneralMaterialData) material);
 
     // Crystal properties
     double length  = EverestCrystalData_get_active_length(el);
     double const co_x       = EverestCrystalData_get_ref_x(el);
     double const co_y       = EverestCrystalData_get_ref_y(el);
     // TODO: use xtrack C-code for rotation element
     // TODO: we are ignoring the angle of the right jaw
@@ -56,38 +63,45 @@
     double const cry_bend   = length/cry_rcurv; //final value (with corrected length) 
     double const cry_alayer = EverestCrystalData_get_thick(el);
     double const cry_xmax   = EverestCrystalData_get_xdim(el);
     double const cry_ymax   = EverestCrystalData_get_ydim(el);
     double const cry_orient = EverestCrystalData_get__orient(el);
     double const cry_miscut = EverestCrystalData_get_miscut(el);
 
+    // Impact table
+    CollimatorImpactsData record = EverestCrystalData_getp_internal_record(el, part0);
+    RecordIndex record_index = NULL;
+    if (record){
+        record_index = CollimatorImpactsData_getp__index(record);
+    }
+
     //start_per_particle_block (part0->part)
         if (!active){
             // Drift full length
             Drift_single_particle(part, inactive_front+active_length+inactive_back);
 
         } else {
             // Check collimator initialisation
             int8_t is_tracking = assert_tracking(part, XC_ERR_INVALID_TRACK);
-            int8_t rng_set     = assert_rng_set(part, RNG_ERR_SEEDS_NOT_SET);
-            int8_t ruth_set    = assert_rutherford_set(rng, part, RNG_ERR_RUTH_NOT_SET);
+            int8_t rng_is_set  = assert_rng_set(part, RNG_ERR_SEEDS_NOT_SET);
+            int8_t ruth_is_set = assert_rutherford_set(rng, part, RNG_ERR_RUTH_NOT_SET);
 
-            if (is_tracking && rng_set && ruth_set) {
+            if (is_tracking && rng_is_set && ruth_is_set) {
                 // Drift inactive front
                 Drift_single_particle(part, inactive_front);
 
                 // Scatter
 
                 // Move to closed orbit
                 LocalParticle_add_to_x(part, -co_x);
                 LocalParticle_add_to_y(part, -co_y);
 
                 scatter_cry(part, length, material, rng, cos_zL, sin_zL, c_aperture, c_offset,
                             side, cry_tilt, cry_rcurv, cry_bend, cry_alayer, cry_xmax, cry_ymax, cry_orient, 
-                            cry_miscut);
+                            cry_miscut, record, record_index);
 
                 // Return from closed orbit
                 LocalParticle_add_to_x(part, co_x);
                 LocalParticle_add_to_y(part, co_y);
 
                 // Drift inactive back (only surviving particles)
                 if (LocalParticle_get_state(part) > 0){
```

### Comparing `xcoll-0.2.2/xcoll/beam_elements/everest_collimator.py` & `xcoll-0.2.3/xcoll/beam_elements/everest_collimator.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,26 +4,28 @@
 # ######################################### #
 
 import xobjects as xo
 import xpart as xp
 import xtrack as xt
 
 from .base_collimator import BaseCollimator, InvalidCollimator
-from ..scattering_routines.everest import Material, CrystalMaterial, EverestEngine
+from ..scattering_routines.everest import GeneralMaterial, Material, CrystalMaterial, EverestEngine
 from ..general import _pkg_root
 
 
 
 # TODO: 
 #      We want these elements to behave as if 'iscollective = True' when doing twiss etc (because they would ruin the CO),
 #      but as if 'iscollective = False' for normal tracking as it is natively in C...
 #      Currently this is achieved with the hack '_tracking' which defaults to False after installation in the line, and is
 #      only activated around the track command. Furthermore, because of 'iscollective = False' we need to specify 
 #      get_backtrack_element. We want it nicer..
 
+# TODO: _per_particle_kernels should be a normal kernel (such that we don't need to pass a dummy Particles() )
+
 class EverestCollimator(BaseCollimator):
     _xofields = { **BaseCollimator._xofields,
         '_material':        Material,
         'rutherford_rng':   xt.RandomRutherford,
         '_tracking':        xo.Int8
     }
 
@@ -37,41 +39,48 @@
 
     _depends_on = [BaseCollimator, EverestEngine]
 
     _extra_c_sources = [
         _pkg_root.joinpath('beam_elements','collimators_src','everest_collimator.h')
     ]
 
+    _per_particle_kernels = {
+        '_EverestCollimator_set_material': xo.Kernel(
+                c_name='EverestCollimator_set_material',
+                args=[]
+            )
+        }
+
 
     def __init__(self, **kwargs):
         if '_xobject' not in kwargs:
             if kwargs.get('material') is None:
                 raise ValueError("Need to provide a material to the collimator!")
             if not isinstance(kwargs['material'], Material):
                 if not isinstance(kwargs['material'], dict) \
                 or kwargs['material']['__class__'] != "Material":
                     raise ValueError("Invalid material!")
             kwargs['_material'] = kwargs.pop('material')
             kwargs.setdefault('rutherford_rng', xt.RandomRutherford())
             kwargs.setdefault('_tracking', True)
         super().__init__(**kwargs)
-#         if '_xobject' not in kwargs:
-#             self.random_generator.set_rutherford_by_xcoll_material(self.material)
+        if '_xobject' not in kwargs:
+            self._EverestCollimator_set_material(xp.Particles())
 
     @property
     def material(self):
         return self._material
 
     @material.setter
     def material(self, material):
         if not isinstance(material, Material):
             if not isinstance('material', dict) or material['__class__'] != "Material":
                 raise ValueError("Invalid material!")
         self._material = material
-#         self.random_generator.set_rutherford_by_xcoll_material(material)
+        self._EverestCollimator_set_material(xp.Particles())
 
     def get_backtrack_element(self, _context=None, _buffer=None, _offset=None):
         # TODO: this should be an InvalidCollimator
         return xt.Drift(length=-self.length, _context=_context, _buffer=_buffer, _offset=_offset)
 
 
 
@@ -99,14 +108,21 @@
 
     _depends_on = [BaseCollimator, EverestEngine]
 
     _extra_c_sources = [
         _pkg_root.joinpath('beam_elements','collimators_src','everest_crystal.h')
     ]
 
+    _per_particle_kernels = {
+        '_EverestCrystal_set_material': xo.Kernel(
+                c_name='EverestCrystal_set_material',
+                args=[]
+            )
+        }
+
 
     def __init__(self, **kwargs):
         if '_xobject' not in kwargs:
             if kwargs.get('material') is None:
                 raise ValueError("Need to provide a material to the collimator!")
             if not isinstance(kwargs['material'], CrystalMaterial):
                 if not isinstance(kwargs['material'], dict) \
@@ -118,16 +134,16 @@
             kwargs.setdefault('ydim', 0)
             kwargs.setdefault('thick', 0)
             kwargs.setdefault('miscut', 0)
             kwargs['_orient'] = _lattice_setter(kwargs.pop('lattice', 'strip'))
             kwargs.setdefault('rutherford_rng', xt.RandomRutherford())
             kwargs.setdefault('_tracking', True)
         super().__init__(**kwargs)
-#         if '_xobject' not in kwargs:
-#             self.random_generator.set_rutherford_by_xcoll_material(self.material)
+        if '_xobject' not in kwargs:
+            self._EverestCrystal_set_material(xp.Particles())
 
     @property
     def lattice(self):
         if self._orient == 1:
             return 'strip'
         elif self._orient == 2:
             return 'quasi-mosaic'
@@ -144,15 +160,15 @@
 
     @material.setter
     def material(self, material):
         if not isinstance(material, CrystalMaterial):
             if not isinstance(material, dict) or material['__class__'] != "CrystalMaterial":
                 raise ValueError("Invalid material!")
         self._material = material
-#         self.random_generator.set_rutherford_by_xcoll_material(material)
+        self._EverestCrystal_set_material(xp.Particles())
 
     def get_backtrack_element(self, _context=None, _buffer=None, _offset=None):
         # TODO: this should be an InvalidCollimator
         return xt.Drift(length=-self.length, _context=_context, _buffer=_buffer, _offset=_offset)
 
 
 def _lattice_setter(lattice):
```

### Comparing `xcoll-0.2.2/xcoll/colldb.py` & `xcoll-0.2.3/xcoll/colldb.py`

 * *Files identical despite different names*

### Comparing `xcoll-0.2.2/xcoll/collimator_settings.py` & `xcoll-0.2.3/xcoll/collimator_settings.py`

 * *Files identical despite different names*

### Comparing `xcoll-0.2.2/xcoll/headers/particle_states.h` & `xcoll-0.2.3/xcoll/headers/particle_states.h`

 * *Files identical despite different names*

### Comparing `xcoll-0.2.2/xcoll/manager.py` & `xcoll-0.2.3/xcoll/manager.py`

 * *Files identical despite different names*

### Comparing `xcoll-0.2.2/xcoll/scattering_routines/everest/crystal.h` & `xcoll-0.2.3/xcoll/scattering_routines/everest/crystal.h`

 * *Files 3% similar despite different names*

```diff
@@ -5,51 +5,49 @@
 
 #ifndef XCOLL_EVEREST_CRYSTAL_INTERACT_H
 #define XCOLL_EVEREST_CRYSTAL_INTERACT_H
 #include <math.h>
 #include <stdio.h>
 #include <stdlib.h>
 
-double tlcut_cry = 0.0009982;
+double const tlcut_cry = 0.0009982;
 
-double aTF = 0.194e-10; // Screening function [m]
-double dP  = 1.920e-10; // Distance between planes (110) [m]
-double u1  = 0.075e-10; // Thermal vibrations amplitude
+double const aTF = 0.194e-10; // Screening function [m]
+double const dP  = 1.920e-10; // Distance between planes (110) [m]
+double const u1  = 0.075e-10; // Thermal vibrations amplitude
 
 // pp cross-sections and parameters for energy dependence
-double pptref_cry = 0.040;
-double freeco_cry = 1.618;
+double const pptref_cry = 0.040;
+double const freeco_cry = 1.618;
 
 // Processes
-int proc_out         =  -1;     // Crystal not hit
-int proc_AM          =   1;     // Amorphous
-int proc_VR          =   2;     // Volume reflection
-int proc_CH          =   3;     // Channeling
-int proc_VC          =   4;     // Volume capture
-int proc_absorbed    =   5;     // Absorption
-int proc_DC          =   6;     // Dechanneling
-int proc_pne         =   7;     // Proton-neutron elastic interaction
-int proc_ppe         =   8;     // Proton-proton elastic interaction
-int proc_diff        =   9;     // Single diffractive
-int proc_ruth        =  10;     // Rutherford scattering
-int proc_ch_absorbed =  15;     // Channeling followed by absorption
-int proc_ch_pne      =  17;     // Channeling followed by proton-neutron elastic interaction
-int proc_ch_ppe      =  18;     // Channeling followed by proton-proton elastic interaction
-int proc_ch_diff     =  19;     // Channeling followed by single diffractive
-int proc_ch_ruth     =  20;     // Channeling followed by Rutherford scattering
-int proc_TRVR        = 100;     // Volume reflection in VR-AM transition region
-int proc_TRAM        = 101;     // Amorphous in VR-AM transition region
-
-int temp = 0;
+int const proc_out         =  -1;     // Crystal not hit
+int const proc_AM          =   1;     // Amorphous
+int const proc_VR          =   2;     // Volume reflection
+int const proc_CH          =   3;     // Channeling
+int const proc_VC          =   4;     // Volume capture
+int const proc_absorbed    =   5;     // Absorption
+int const proc_DC          =   6;     // Dechanneling
+int const proc_pne         =   7;     // Proton-neutron elastic interaction
+int const proc_ppe         =   8;     // Proton-proton elastic interaction
+int const proc_diff        =   9;     // Single diffractive
+int const proc_ruth        =  10;     // Rutherford scattering
+int const proc_ch_absorbed =  15;     // Channeling followed by absorption
+int const proc_ch_pne      =  17;     // Channeling followed by proton-neutron elastic interaction
+int const proc_ch_ppe      =  18;     // Channeling followed by proton-proton elastic interaction
+int const proc_ch_diff     =  19;     // Channeling followed by single diffractive
+int const proc_ch_ruth     =  20;     // Channeling followed by Rutherford scattering
+int const proc_TRVR        = 100;     // Volume reflection in VR-AM transition region
+int const proc_TRAM        = 101;     // Amorphous in VR-AM transition region
 
 
 /*gpufun*/
 double* movech(RandomRutherfordData rng, LocalParticle* part, double nam, double dz, double x, double xp, double yp, double pc, double r, double rc, double rho, double anuc, double zatom, double emr, double hcut, double bnref, double csref0, double csref1, double csref5, double eUm, double collnt, double iProc) {
 
-    static double result[5];
+    double* result = (double*)malloc(5 * sizeof(double));
 
 //     // Material properties
 //     double const exenergy = CrystalMaterialData_get_excitation_energy(material);
 //     double const rho      = CrystalMaterialData_get_density(material);
 //     double const anuc     = CrystalMaterialData_get_A(material);
 //     double const zatom    = CrystalMaterialData_get_Z(material);
 //     double const emr      = CrystalMaterialData_get_nuclear_radius(material);
@@ -270,15 +268,15 @@
     return result;
 }
 
 
 /*gpufun*/
 double* moveam(RandomRutherfordData rng, LocalParticle* part, double nam, double dz, double dei, double dlr, double xp, double yp, double pc, double anuc, double zatom, double emr, double hcut, double bnref, double csref0, double csref1, double csref5, double collnt, double iProc) {
 
-    static double result[4];
+    double* result = (double*)malloc(4 * sizeof(double));
 
 //     // Material properties
 //     double const exenergy = CrystalMaterialData_get_excitation_energy(material);
 //     double const rho      = CrystalMaterialData_get_density(material);
 //     double const anuc     = CrystalMaterialData_get_A(material);
 //     double const zatom    = CrystalMaterialData_get_Z(material);
 //     double const emr      = CrystalMaterialData_get_nuclear_radius(material);
@@ -489,15 +487,15 @@
 
 /*gpufun*/
 double* interact(RandomRutherfordData rng, LocalParticle* part, double x, double xp, double y, double yp, double pc, double length, double s_P, double x_P, double exenergy, double rho, double anuc, double zatom, double emr, double dlri, double dlyi, 
                 double ai, double eUm, double collnt, double hcut, double csref0, double csref1, double csref5, double bnref,
                  double cry_tilt, double cry_rcurv, double cry_alayer, double cry_xmax, 
                 double cry_ymax, double cry_orient, double cry_miscut, double cry_bend, double cry_cBend, double cry_sBend, double cry_cpTilt, double cry_spTilt, double cry_cnTilt, double cry_snTilt, double iProc) {
 
-    static double result[6];
+    double* result = (double*)malloc(6 * sizeof(double));
 
 //     // Material properties
 //     double const exenergy = CrystalMaterialData_get_excitation_energy(material);
 //     double const rho      = CrystalMaterialData_get_density(material);
 //     double const anuc     = CrystalMaterialData_get_A(material);
 //     double const zatom    = CrystalMaterialData_get_Z(material);
 //     double const emr      = CrystalMaterialData_get_nuclear_radius(material);
@@ -508,17 +506,14 @@
 //     double const collnt   = CrystalMaterialData_get_nuclear_collision_length(material);
 //     double const hcut     = CrystalMaterialData_get_hcut(material);
 //     double const bnref    = CrystalMaterialData_get_nuclear_elastic_slope(material);
 //     double const csref0   = CrystalMaterialData_get_cross_section(material, 0);
 //     double const csref1   = CrystalMaterialData_get_cross_section(material, 1);
 //     double const csref5   = CrystalMaterialData_get_cross_section(material, 5);
 
-    double* result_am;
-    double* result_ch;
-
     double dest = 0.;
     double pmap = 938.271998;
     double pmae = 0.51099890;
     double crade = 2.817940285e-15;
 
     double c_v1 =  1.7;   // Fitting coefficient
     double c_v2 = -1.5;   // Fitting coefficient
@@ -650,20 +645,21 @@
         x  = x0 + xp*s;
         y     = y0 + yp*s;
         iProc = proc_AM;
 
         dest = calcionloss_cry(part,s_length,dest,betar,bgr,gammar,tmax,plen,
                             exenergy,zatom,rho,anuc);
 
-        result_am = moveam(rng, part,nam,am_len,dest,dlri,xp,yp,pc,anuc,zatom,emr,hcut,
+        double* result_am = moveam(rng, part,nam,am_len,dest,dlri,xp,yp,pc,anuc,zatom,emr,hcut,
                             bnref,csref0,csref1,csref5,collnt,iProc);
         xp = result_am[0];
         yp = result_am[1];
         pc = result_am[2];
         iProc = result_am[3];
+        free(result_am);
 
         x = x + xp*(s_length-s);
         y = y + yp*(s_length-s);
 
         result[0] = x;
         result[1] = xp;
         result[2] = y;
@@ -674,20 +670,21 @@
 
     } else if (x > cry_xmax-cry_alayer && x < cry_xmax) {
         iProc = proc_AM;
         
         dest = calcionloss_cry(part,s_length,dest,betar,bgr,gammar,tmax,plen,
                             exenergy,zatom,rho,anuc);
 
-        result_am = moveam(rng, part,nam,s_length,dest,dlri,xp,yp,pc,anuc,zatom,emr,hcut,bnref,csref0,
+        double* result_am = moveam(rng, part,nam,s_length,dest,dlri,xp,yp,pc,anuc,zatom,emr,hcut,bnref,csref0,
                         csref1,csref5,collnt,iProc);
         xp = result_am[0];
         yp = result_am[1];
         pc = result_am[2];
         iProc = result_am[3];
+        free(result_am);
 
         result[0] = x;
         result[1] = xp;
         result[2] = y;
         result[3] = yp;
         result[4] = pc;
         result[5] = iProc;
@@ -755,35 +752,37 @@
                                     exenergy,zatom,rho,anuc);
                 pc = pc - 0.5*dest*Ldech; //Energy loss to ionization while in CH [GeV]
                 x  = x  + (0.5*(s_length-Sdech))*xp;
                 y  = y  + (0.5*(s_length-Sdech))*yp;
 
                 dest = calcionloss_cry(part,s_length-Sdech,dest,betar,bgr,gammar,tmax,plen,exenergy,zatom,rho,anuc);
 
-                result_am = moveam(rng,part,nam,s_length-Sdech,dest,dlri,xp,yp,pc,anuc,zatom,emr,hcut,bnref,csref0,csref1,csref5,collnt,iProc);
+                double* result_am = moveam(rng,part,nam,s_length-Sdech,dest,dlri,xp,yp,pc,anuc,zatom,emr,hcut,bnref,csref0,csref1,csref5,collnt,iProc);
                 xp = result_am[0];
                 yp = result_am[1];
                 pc = result_am[2];
                 iProc = result_am[3];
+                free(result_am);
 
                 x = x + (0.5*(s_length-Sdech))*xp;
                 y = y + (0.5*(s_length-Sdech))*yp;
             } else {
                 iProc = proc_CH;
                 double xpin  = xp;
                 double ypin  = yp;
 
                 //check if a nuclear interaction happen while in CH
-                result_ch = movech(rng,part,nam,L_chan,x,xp,yp,pc,cry_rcurv,Rcrit,rho,anuc,zatom,emr,hcut,bnref,
+                double* result_ch = movech(rng,part,nam,L_chan,x,xp,yp,pc,cry_rcurv,Rcrit,rho,anuc,zatom,emr,hcut,bnref,
                                 csref0,csref1,csref5,eUm,collnt,iProc);
                 x = result_ch[0];
                 xp = result_ch[1];
                 yp = result_ch[2];
                 pc = result_ch[3];
                 iProc = result_ch[4];
+                free(result_ch);
 
                 if (iProc != proc_CH) {
                     //if an nuclear interaction happened, move until the middle with initial xp,yp:
                     //propagate until the "crystal exit" with the new xp,yp accordingly with the rest
                     //of the code in "thin lens approx"
                     x = x + (0.5*L_chan)*xpin;
                     y = y + (0.5*L_chan)*ypin;
@@ -809,19 +808,20 @@
             iProc = proc_VR;
 
             xp = xp + (0.45*(xp_rel/xpcrit + 1))*Ang_avr;
             x  = x  + (0.5*s_length)*xp;
             y  = y  + (0.5*s_length)*yp;
 
             dest = calcionloss_cry(part,s_length,dest,betar,bgr,gammar,tmax,plen,exenergy,zatom,rho,anuc);
-            result_am = moveam(rng, part,nam,s_length,dest,dlri,xp,yp,pc,anuc,zatom,emr,hcut,bnref,csref0,csref1,csref5,collnt,iProc);
+            double* result_am = moveam(rng, part,nam,s_length,dest,dlri,xp,yp,pc,anuc,zatom,emr,hcut,bnref,csref0,csref1,csref5,collnt,iProc);
             xp = result_am[0];
             yp = result_am[1];
             pc = result_am[2];
             iProc = result_am[3];
+            free(result_am);
 
             x = x + (0.5*s_length)*xp;
             y = y + (0.5*s_length)*yp;  
         }
     } else { //case 3-2: no good for channeling. check if the  can VR
         double Lrefl = xp_rel*r; //Distance of refl. point [m]
         double Srefl = sin(xp_rel/2. + cry_miscut)*Lrefl;
@@ -836,19 +836,20 @@
                 y     = y + yp*Srefl;
                 double Dxp   = Ang_avr;
                 xp    = xp + Dxp + Ang_rms*RandomNormal_generate(part);
                 x  = x  + (0.5*xp)*(s_length - Srefl);
                 y     = y  + (0.5*yp)*(s_length - Srefl);
 
                 dest = calcionloss_cry(part,s_length-Srefl,dest,betar,bgr,gammar,tmax,plen,exenergy,zatom,rho,anuc);
-                result_am = moveam(rng,part,nam,s_length-Srefl,dest,dlri,xp,yp,pc,anuc,zatom,emr,hcut,bnref,csref0,csref1,csref5,collnt,iProc);
+                double* result_am = moveam(rng,part,nam,s_length-Srefl,dest,dlri,xp,yp,pc,anuc,zatom,emr,hcut,bnref,csref0,csref1,csref5,collnt,iProc);
                 xp = result_am[0];
                 yp = result_am[1];
                 pc = result_am[2];
                 iProc = result_am[3];
+                free(result_am);
 
                 x = x + (0.5*xp)*(s_length - Srefl);
                 y = y + (0.5*yp)*(s_length - Srefl);
             } else { //Option 2: VC
                 x = x + xp*Srefl;
                 y = y + yp*Srefl;
 
@@ -874,20 +875,21 @@
 
                     dest = calcionloss_cry(part,Sdech,dest,betar,bgr,gammar,tmax,plen,
                                         exenergy,zatom,rho,anuc);
                     pc = pc - (0.5*dest)*Sdech; //"added" energy loss while captured
 
                     dest = calcionloss_cry(part,Red_S,dest,betar,bgr,gammar,tmax,plen,
                                         exenergy,zatom,rho,anuc);
-                    result_am = moveam(rng,part,nam,Red_S,dest,dlri,xp,yp,pc,anuc,zatom,emr,hcut,bnref,csref0,
+                    double* result_am = moveam(rng,part,nam,Red_S,dest,dlri,xp,yp,pc,anuc,zatom,emr,hcut,bnref,csref0,
                         csref1,csref5,collnt,iProc);
                     xp = result_am[0];
                     yp = result_am[1];
                     pc = result_am[2];
                     iProc = result_am[3];
+                    free(result_am);
                     
                     x = x + (0.5*xp)*Red_S;
                     y = y + (0.5*yp)*Red_S;
                 } else {
                     iProc   = proc_VC;
                     double Rlength = length - Lrefl;
                     double tchan   = Rlength/cry_rcurv;
@@ -896,21 +898,22 @@
                     dest = calcionloss_cry(part,Lrefl,dest,betar,bgr,gammar,tmax,plen,
                                         exenergy,zatom,rho,anuc);
                     pc   = pc - dest*Lrefl; //"added" energy loss before capture
                     double xpin = xp;
                     double ypin = yp;
 
                     //Check if a nuclear interaction happen while in ch
-                    result_ch = movech(rng,part,nam,Rlength,x,xp,yp,pc,cry_rcurv,Rcrit,rho,anuc,zatom,emr,hcut,bnref,
+                    double* result_ch = movech(rng,part,nam,Rlength,x,xp,yp,pc,cry_rcurv,Rcrit,rho,anuc,zatom,emr,hcut,bnref,
                                     csref0,csref1,csref5,eUm,collnt,iProc);
                     x = result_ch[0];
                     xp = result_ch[1];
                     yp = result_ch[2];
                     pc = result_ch[3];
                     iProc = result_ch[4];
+                    free(result_ch);
                                     
                     if (iProc != proc_VC) {
                         //if an nuclear interaction happened, move until the middle with initial xp,yp: propagate until
                         //the "crystal exit" with the new xp,yp aciordingly with the rest of the code in "thin lens approx"
                         x = x + (0.5*Rlength)*xpin;
                         y = y + (0.5*Rlength)*ypin;
                         x = x + (0.5*Rlength)*xp;
@@ -937,20 +940,21 @@
             if (xp_rel > tdefl-cry_miscut + 2*xpcrit || xp_rel < -xpcrit) {
                 iProc = proc_AM;
                 x  = x + (0.5*s_length)*xp;
                 y     = y + (0.5*s_length)*yp;
                 if(zn > 0) {
                     dest = calcionloss_cry(part,s_length,dest,betar,bgr,gammar,tmax,plen,
                                         exenergy,zatom,rho,anuc);
-                    result_am = moveam(rng,part,nam,s_length,dest,dlri,xp,yp,pc,anuc,zatom,emr,hcut,bnref,csref0,
+                    double* result_am = moveam(rng,part,nam,s_length,dest,dlri,xp,yp,pc,anuc,zatom,emr,hcut,bnref,csref0,
                         csref1,csref5,collnt,iProc);
                     xp = result_am[0];
                     yp = result_am[1];
                     pc = result_am[2];
                     iProc = result_am[3];
+                    free(result_am);
                 }
             
                 x = x + (0.5*s_length)*xp;
                 y = y + (0.5*s_length)*yp;
             } else {
                 double Pvr = (xp_rel-(tdefl-cry_miscut))/(2.*xpcrit);
                 if(RandomUniform_generate(part) > Pvr) {
@@ -962,40 +966,42 @@
                     double Dxp = (((-3.*Ang_rms)*xp_rel)/(2.*xpcrit) + Ang_avr) + ((3.*Ang_rms)*(tdefl-cry_miscut))/(2.*xpcrit);
                     xp  = xp + Dxp;
                     x = x + (0.5*xp)*(s_length-Srefl);
                     y   = y + (0.5*yp)*(s_length-Srefl);
 
                     dest = calcionloss_cry(part,s_length-Srefl,dest,betar,bgr,gammar,tmax,plen,
                                         exenergy,zatom,rho,anuc);
-                    result_am = moveam(rng,part,nam,s_length-Srefl,dest,dlri,xp,yp,pc,anuc,zatom,emr,hcut,bnref,csref0,
+                    double* result_am = moveam(rng,part,nam,s_length-Srefl,dest,dlri,xp,yp,pc,anuc,zatom,emr,hcut,bnref,csref0,
                         csref1,csref5,collnt,iProc);
                     xp = result_am[0];
                     yp = result_am[1];
                     pc = result_am[2];
                     iProc = result_am[3];
+                    free(result_am);
 
                     x = x + (0.5*xp)*(s_length - Srefl);
                     y = y + (0.5*yp)*(s_length - Srefl);
                 } else {
                     iProc = proc_TRAM;
                     x = x + xp*Srefl;
                     y = y + yp*Srefl;
                     double Dxp = ((((-1.*(13.6/pc))*sqrt(s_length/dlri))*1.0e-3)*xp_rel)/(2.*xpcrit) + (((13.6/pc)*sqrt(s_length/dlri))*1.0e-3)*(1.+(tdefl-cry_miscut)/(2.*xpcrit));
                     xp = xp+Dxp;
                     x  = x + (0.5*xp)*(s_length-Srefl);
                     y  = y + (0.5*yp)*(s_length-Srefl);
 
                     dest = calcionloss_cry(part,s_length-Srefl,dest,betar,bgr,gammar,tmax,plen,
                                         exenergy,zatom,rho,anuc);
-                    result_am = moveam(rng,part,nam,s_length-Srefl,dest,dlri,xp,yp,pc,anuc,zatom,emr,hcut,bnref,csref0,
+                    double* result_am = moveam(rng,part,nam,s_length-Srefl,dest,dlri,xp,yp,pc,anuc,zatom,emr,hcut,bnref,csref0,
                         csref1,csref5,collnt,iProc);
                     xp = result_am[0];
                     yp = result_am[1];
                     pc = result_am[2];
                     iProc = result_am[3];
+                    free(result_am);
 
                     x = x + (0.5*xp)*(s_length - Srefl);
                     y = y + (0.5*yp)*(s_length - Srefl);
                 }
             }
         }            
     }
@@ -1054,16 +1060,15 @@
     double b_eq       = 0.;
     double c_eq       = 0.;
     double cry_length  = c_length;
 
     s_imp  = 0.;
     iProc  = proc_out;
 
-    static double crystal_result[21];
-    double* result;
+    double* crystal_result = (double*)malloc(21 * sizeof(double));
 
     double const cry_cBend  = cos(cry_bend);
     double const cry_sBend  = sin(cry_bend);
 
     // Transform in the crystal reference system
     // 1st transformation: shift of the center of the reference frame
     double const cry_cpTilt = cos(cry_tilt);
@@ -1096,25 +1101,26 @@
   
     // Check that particle hit the crystal
     if (x >= 0. && x < cry_xmax) {
         // MISCUT first step: P coordinates (center of curvature of crystalline planes)
         double s_P = (cry_rcurv-cry_xmax)*sin(-cry_miscut);
         double x_P = cry_xmax + (cry_rcurv-cry_xmax)*cos(-cry_miscut);
 
-        result = interact(rng,part,x,xp,z,zp,p,cry_length,s_P,x_P,exenergy,rho,anuc,zatom,emr,dlri,dlyi,
+        double* result = interact(rng,part,x,xp,z,zp,p,cry_length,s_P,x_P,exenergy,rho,anuc,zatom,emr,dlri,dlyi,
                         ai,eum,collnt,hcut,csref0,csref1,csref5,bnref,cry_tilt,
                         cry_rcurv,cry_alayer,cry_xmax,cry_ymax,cry_orient,cry_miscut,cry_bend,cry_cBend,
                         cry_sBend,cry_cpTilt,cry_spTilt,cry_cnTilt,cry_snTilt,iProc);
 
         x = result[0];
         xp = result[1];
         z = result[2];
         zp = result[3];
         p = result[4];
         iProc = result[5];
+        free(result);
 
         s   = cry_rcurv*cry_sBend;
         zlm = cry_rcurv*cry_sBend;
 
         if (iProc != proc_out) {
             isimp    = 1;
             nhit     = nhit + 1.;
@@ -1161,25 +1167,26 @@
                 // Translation
                 s_P_tmp = s_P_tmp - s_int;
                 x_P_tmp = x_P_tmp - x_int;
                 // Rotation
                 double s_P = s_P_tmp*cos(tilt_int) + x_P_tmp*sin(tilt_int);
                 double x_P = -s_P_tmp*sin(tilt_int) + x_P_tmp*cos(tilt_int);
 
-                result = interact(rng,part,x,xp,z,zp,p,cry_length-(tilt_int*cry_rcurv),s_P,x_P,exenergy,rho,anuc,
+                double* result = interact(rng,part,x,xp,z,zp,p,cry_length-(tilt_int*cry_rcurv),s_P,x_P,exenergy,rho,anuc,
                                 zatom,emr,dlri,dlyi,ai,eum,collnt,hcut,csref0,csref1,csref5,bnref,
                                 cry_tilt,cry_rcurv,cry_alayer,cry_xmax,cry_ymax,cry_orient,cry_miscut,
                                 cry_bend,cry_cBend,cry_sBend,cry_cpTilt,cry_spTilt,cry_cnTilt,cry_snTilt,iProc);
 
                 x = result[0];
                 xp = result[1];
                 z = result[2];
                 zp = result[3];
                 p = result[4];
                 iProc = result[5];
+                free(result);
 
                 s   = cry_rcurv*sin(cry_bend - tilt_int);
                 zlm = cry_rcurv*sin(cry_bend - tilt_int);
                 
                 if (iProc != proc_out) {
                     x_rot    = x_int;
                     s_rot    = s_int;
@@ -1263,15 +1270,15 @@
     } else if (iProc == proc_CH) {
         n_chan = n_chan + 1;
     } else if (iProc == proc_absorbed) {
         nabs = 1;   // TODO: do we need to set part_abs_pos etc?
     } else if (iProc == proc_ch_absorbed) {
         nabs = 1;
     }
-    
+
     crystal_result[0] = val_part_hit;
     crystal_result[1] = val_part_abs;
     crystal_result[2] = val_part_impact;
     crystal_result[3] = val_part_indiv;
     crystal_result[4] = nhit;
     crystal_result[5] = nabs;
     crystal_result[6] = s_imp;
```

### Comparing `xcoll-0.2.2/xcoll/scattering_routines/everest/everest.h` & `xcoll-0.2.3/xcoll/scattering_routines/everest/everest.h`

 * *Files identical despite different names*

### Comparing `xcoll-0.2.2/xcoll/scattering_routines/everest/everest.py` & `xcoll-0.2.3/xcoll/scattering_routines/everest/everest.py`

 * *Files identical despite different names*

### Comparing `xcoll-0.2.2/xcoll/scattering_routines/everest/jaw.h` & `xcoll-0.2.3/xcoll/scattering_routines/everest/jaw.h`

 * *Files 3% similar despite different names*

```diff
@@ -80,15 +80,15 @@
 /*gpufun*/
 double* scamcs(LocalParticle* part, double x0, double xp0, double s) {
     // double x0  = *xx;
     // double xp0 = *xxp;
     double r2 = 0;
     double v1 = 0;
     double v2 = 0;
-    static double result[2];
+    double* result = (double*)malloc(2 * sizeof(double));
 
     while (1) {
         v1 = 2*RandomUniform_generate(part) - 1;
         v2 = 2*RandomUniform_generate(part) - 1;
         r2 = pow(v1,2) + pow(v2,2);
 
         if(r2 < 1) {
@@ -115,15 +115,15 @@
     double s;
     double theta = 13.6e-3/p;
     double h   = 0.001;
     double dh  = 0.0001;
     double bn0 = 0.4330127019;
     double rlen0 = zlm1/radl;
     double rlen  = rlen0;
-    static double result[5];
+    double* result = (double*)malloc(5 * sizeof(double));
 
     x     = (x/theta)/radl;
     xp    = xp/theta;
     z     = (z/theta)/radl;
     zp    = zp/theta;
 
     while (1) {
@@ -139,14 +139,15 @@
         s = soln3(ae,be,dh,rlen);
         if (s < h) {
             s = h;
         }
         double* res = scamcs(part, x,xp,s);
         x  = res[0];
         xp = res[1];
+        free(res);
         if (x <= 0) {
             s = (rlen0-rlen)+ s;
             break; // go to 20
         }
         if ((s + dh) >= rlen) {
             s = rlen0;
             break; // go to 20
@@ -154,14 +155,15 @@
         // go to 10
         rlen = rlen - s;
     }
 
     double* res = scamcs(part, z,zp,s);
     z  = res[0];
     zp = res[1];
+    free(res);
 
     result[0]  = s*radl;
     result[1]  = (x*theta)*radl;
     result[2]  = xp*theta;
     result[3]  = (z*theta)*radl;
     result[4]  = zp*theta;
     return result;
@@ -172,15 +174,15 @@
 double* tetat(LocalParticle* part, double t, double p) {
     double teta = sqrt(t)/p;
     double va = 0;
     double vb  = 0;
     double va2 = 0;
     double vb2 = 0;
     double r2  = 0;
-    static double result[2];
+    double* result = (double*)malloc(2 * sizeof(double));
     
     while (1) {
         va  = 2*RandomUniform_generate(part) - 1;
         vb  = RandomUniform_generate(part);
         va2 = pow(va,2);
         vb2 = pow(vb,2);
         r2  = va2 + vb2;
@@ -194,15 +196,16 @@
     return result;
 }
 
 
 /*gpufun*/
 double* gettran(RandomRutherfordData rng, LocalParticle* part, double inter, double p, struct ScatteringParameters scat) {
 
-    static double res[2];
+    double* res = (double*)malloc(2 * sizeof(double));
+
     // Neither if-statements below have an else, so defaulting function return to zero.
     double result = 0;
 
     if (inter==2) { // Nuclear Elastic
         result = RandomExponential_generate(part)/scat.bn;
     } else if (inter==3) { // pp Elastic
         result = RandomExponential_generate(part)/scat.bpp;
@@ -303,16 +306,16 @@
     return i;
 }
 
 
 /*gpufun*/
 double* jaw(LocalParticle* part, MaterialData material, RandomRutherfordData rng, struct ScatteringParameters scat,
             double p, double zlm, double x, double xp, double z, double zp) {
-    
-    static double result[7];
+
+    double* result = (double*)malloc(7 * sizeof(double));
     double s;
     double nabs = 0;
     double rlen = zlm;
     double m_dpodx = 0.;
     double t;
     double tx; 
     double tz;
@@ -330,28 +333,30 @@
             zlm1 = rlen;
             double* res = mcs(part, material, zlm1, p, x, xp, z, zp);
             s = res[0];
             x = res[1];
             xp = res[2];
             z = res[3];
             zp = res[4];
+            free(res);
 
             s = (zlm-rlen)+s;
             m_dpodx = calcionloss(part, p, rlen, material);  // DM routine to include tail
             p = p-m_dpodx*s;
             break;
         }
         // Otherwise do multi-coulomb scattering.
         // REGULAR STEP IN ITERATION LOOP
         double* res1 = mcs(part, material, zlm1, p, x, xp, z, zp);
         s = res1[0];
         x = res1[1];
         xp = res1[2];
         z = res1[3];
         zp = res1[4];
+        free(res1);
 
         // Check if particle is outside of collimator (X.LT.0) after
         // MCS. If yes, calculate output longitudinal position (s),
         // reduce momentum (output as dpop) and return.
         // PARTICLE LEFT COLLIMATOR BEFORE ITS END.
 
         if(x <= 0) {
@@ -384,22 +389,24 @@
         // Coulomb:                  inter = 5
 
         // Gettran returns some monte carlo number, that, as I believe, gives the rms transverse momentum transfer.
 
         double* res2 = gettran(rng, part, inter, p, scat);
         t = res2[0];
         p = res2[1];
+        free(res2);
 
         // Tetat calculates from the rms transverse momentum transfer in
         // monte-carlo fashion the angle changes for x and z planes. The
         // angle change is proportional to SQRT(t) and 1/p, as expected.
 
         double* res3 = tetat(part,t,p);
         tx = res3[0]; 
         tz = res3[1];
+        free(res3);
 
         // Apply angle changes
         xp = xp + tx;
         zp = zp + tz;
 
         // Treat single-diffractive scattering.
         if(inter == 4) {
```

### Comparing `xcoll-0.2.2/xcoll/scattering_routines/everest/materials.py` & `xcoll-0.2.3/xcoll/scattering_routines/everest/materials.py`

 * *Files identical despite different names*

### Comparing `xcoll-0.2.2/xcoll/scattering_routines/everest/scatter.h` & `xcoll-0.2.3/xcoll/scattering_routines/everest/scatter.h`

 * *Files 0% similar despite different names*

```diff
@@ -163,14 +163,15 @@
             p_out = jaw_result[0];
             nabs = jaw_result[1];
             s_out = jaw_result[2];
             x = jaw_result[3];
             xp = jaw_result[4];
             z = jaw_result[5];
             zp = jaw_result[6];
+            free(jaw_result);
 
             // val_nabs_type = nabs;
             val_part_hit  = 1;
 
             // Writeout should be done for both inelastic and single diffractive. doing all transformations
             // in x_flk and making the set to 99.99 mm conditional for nabs=1
             if (nabs == 1 || nabs == 4) {
```

### Comparing `xcoll-0.2.2/xcoll/scattering_routines/everest/scatter_crystal.h` & `xcoll-0.2.3/xcoll/scattering_routines/everest/scatter_crystal.h`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 #include <stdio.h>
 
 
 /*gpufun*/
 void scatter_cry(LocalParticle* part, double length, CrystalMaterialData material, RandomRutherfordData rng,
                  double cRot, double sRot, double c_aperture, double c_offset, int side, double cry_tilt,
                  double cry_rcurv, double cry_bend, double cry_alayer, double cry_xmax, double cry_ymax, 
-                 double cry_orient, double cry_miscut){
+                 double cry_orient, double cry_miscut, CollimatorImpactsData record, RecordIndex record_index){
 
     // Store initial coordinates for updating later
     double const rpp_in  = LocalParticle_get_rpp(part);
     double const rvv_in  = LocalParticle_get_rvv(part);
     double const e0      = LocalParticle_get_energy0(part) / 1e9; // Reference energy in GeV
     double const beta0   = LocalParticle_get_beta0(part);
     double const ptau_in = LocalParticle_get_ptau(part);
@@ -167,14 +167,16 @@
         zp = crystal_result[15];
         p = crystal_result[16];
         iProc = crystal_result[17];
         n_chan = crystal_result[18];
         n_VR = crystal_result[19];
         n_amorphous = crystal_result[20];
 
+        free(crystal_result);
+
         if (nabs != 0.) {
             val_part_abs = 1.;
             // val_part_linteract = zlm;
         }
         s_imp  = (s - length) + s_imp;
 
         // Transform back to particle coordinates with opening and offset
```

### Comparing `xcoll-0.2.2/xcoll/scattering_routines/everest/scatter_init.h` & `xcoll-0.2.3/xcoll/scattering_routines/everest/scatter_init.h`

 * *Files identical despite different names*

### Comparing `xcoll-0.2.2/xcoll/tables.py` & `xcoll-0.2.3/xcoll/tables.py`

 * *Files identical despite different names*

### Comparing `xcoll-0.2.2/setup.py` & `xcoll-0.2.3/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,33 +2,40 @@
 from setuptools import setup
 
 packages = \
 ['xcoll', 'xcoll.beam_elements', 'xcoll.scattering_routines.everest']
 
 package_data = \
 {'': ['*'],
- 'xcoll': ['headers/*'],
+ 'xcoll': ['headers/*',
+           'scattering_routines/fluka/flukaio/*',
+           'scattering_routines/fluka/flukaio/doc/*',
+           'scattering_routines/fluka/flukaio/include/*',
+           'scattering_routines/fluka/flukaio/lib/*',
+           'scattering_routines/fluka/flukaio/samples/*',
+           'scattering_routines/fluka/flukaio/src/*',
+           'scattering_routines/fluka/flukaio/tests/*',
+           'scattering_routines/fluka/flukaio/tests/fakes/*'],
  'xcoll.beam_elements': ['collimators_src/*']}
 
 install_requires = \
 ['numpy>=1.0',
  'pandas>=1.4',
- 'xcoll>=0.2.1,<0.3.0',
- 'xdeps>=0.1.1,<0.2.0',
- 'xfields>=0.12.1,<0.13.0',
- 'xobjects>=0.2.6,<0.3.0',
- 'xpart>=0.15.0,<0.16.0',
- 'xtrack>=0.36.5,<0.37.0']
+ 'xdeps>=0.1.1',
+ 'xfields>=0.12.1',
+ 'xobjects>=0.2.6',
+ 'xpart>=0.15.0',
+ 'xtrack>=0.36.5']
 
 extras_require = \
 {'tests': ['ruamel-yaml>=0.17.31,<0.18.0']}
 
 setup_kwargs = {
     'name': 'xcoll',
-    'version': '0.2.2',
+    'version': '0.2.3',
     'description': 'Xsuite collimation package',
     'long_description': '# xcoll\n\n<!---![PyPI - Python Version](https://img.shields.io/pypi/pyversions/xcoll?logo=PyPI?style=plastic) ![PyPI - Wheel](https://img.shields.io/pypi/wheel/xcoll?logo=PyPI?style=plastic)-->\n\n![GitHub release (latest by date)](https://img.shields.io/github/v/release/xsuite/xcoll?style=plastic)\n![GitHub](https://img.shields.io/github/license/xsuite/xcoll?style=plastic)\n![PyPi](https://img.shields.io/pypi/dm/xcoll?logo=PyPI&style=plastic)\n![GitHub all releases](https://img.shields.io/github/downloads/xsuite/xcoll/total?logo=GitHub&style=plastic)\n\n![GitHub pull requests](https://img.shields.io/github/issues-pr/xsuite/xcoll?logo=GitHub&style=plastic)\n![GitHub issues](https://img.shields.io/github/issues/xsuite/xcoll?logo=GitHub&style=plastic)\n![GitHub repo size](https://img.shields.io/github/repo-size/xsuite/xcoll?logo=GitHub&style=plastic)\n\nCollimation in xtrack simulations\n\n## Description\n\n## Getting Started\n\n### Dependencies\n\n* python >= 3.8\n    * numpy\n    * pandas\n    * xsuite (in particular xobjects, xdeps, xtrack, xpart)\n\n### Installing\n`xcoll` is packaged using `poetry`, and can be easily installed with `pip`:\n```bash\npip install xcoll\n```\nFor a local installation, clone and install in editable mode (need to have `pip` >22):\n```bash\ngit clone git@github.com:xsuite/xcoll.git\npip install -e xcoll\n```\n\n### Example\n\n## Features\n\n## Authors\n\n* [Frederik Van der Veken](https://github.com/freddieknets) (frederik@cern.ch)\n* [Despina Demetriadou](https://github.com/ddemetriadou)\n* [Andrey Abramov](https://github.com/anabramo)\n* [Giovanni Iadarola](https://github.com/giadarol)\n\n\n## Version History\n\n* 0.1\n    * Initial Release\n\n## License\n\nThis project is [Apache 2.0 licensed](./LICENSE).\n',
     'author': 'Frederik F. Van der Veken',
     'author_email': 'frederik@cern.ch',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/xsuite/xcoll',
```

### Comparing `xcoll-0.2.2/PKG-INFO` & `xcoll-0.2.3/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xcoll
-Version: 0.2.2
+Version: 0.2.3
 Summary: Xsuite collimation package
 Home-page: https://github.com/xsuite/xcoll
 License: Apache 2.0
 Author: Frederik F. Van der Veken
 Author-email: frederik@cern.ch
 Requires-Python: >=3.8
 Classifier: License :: Other/Proprietary License
@@ -13,20 +13,19 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: tests
 Requires-Dist: numpy (>=1.0)
 Requires-Dist: pandas (>=1.4)
 Requires-Dist: ruamel-yaml (>=0.17.31,<0.18.0); extra == "tests"
-Requires-Dist: xcoll (>=0.2.1,<0.3.0)
-Requires-Dist: xdeps (>=0.1.1,<0.2.0)
-Requires-Dist: xfields (>=0.12.1,<0.13.0)
-Requires-Dist: xobjects (>=0.2.6,<0.3.0)
-Requires-Dist: xpart (>=0.15.0,<0.16.0)
-Requires-Dist: xtrack (>=0.36.5,<0.37.0)
+Requires-Dist: xdeps (>=0.1.1)
+Requires-Dist: xfields (>=0.12.1)
+Requires-Dist: xobjects (>=0.2.6)
+Requires-Dist: xpart (>=0.15.0)
+Requires-Dist: xtrack (>=0.36.5)
 Project-URL: Repository, https://github.com/xsuite/xcoll
 Description-Content-Type: text/markdown
 
 # xcoll
 
 <!---![PyPI - Python Version](https://img.shields.io/pypi/pyversions/xcoll?logo=PyPI?style=plastic) ![PyPI - Wheel](https://img.shields.io/pypi/wheel/xcoll?logo=PyPI?style=plastic)-->
```

