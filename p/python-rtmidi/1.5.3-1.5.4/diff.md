# Comparing `tmp/python_rtmidi-1.5.3.tar.gz` & `tmp/python_rtmidi-1.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_rtmidi-1.5.3.tar", last modified: Fri Jun 23 06:48:00 2023, max compression
+gzip compressed data, was "python_rtmidi-1.5.4.tar", last modified: Tue Jun 27 11:23:47 2023, max compression
```

## Comparing `python_rtmidi-1.5.3.tar` & `python_rtmidi-1.5.4.tar`

### file list

```diff
@@ -1,149 +1,150 @@
--rw-r--r--   0        0        0       94 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/.flake8
--rw-r--r--   0        0        0     1903 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/.github/workflows/pr_to_master.yml
--rw-r--r--   0        0        0     2603 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/.github/workflows/push_to_master.yml
--rw-r--r--   0        0        0     2539 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/.github/workflows/release.yml
--rw-r--r--   0        0        0      571 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/.gitignore
--rw-r--r--   0        0        0      118 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/.gitmodules
--rw-r--r--   0        0        0      295 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/AUTHORS.md
--rw-r--r--   0        0        0    22683 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/CHANGELOG.md
--rw-r--r--   0        0        0     3849 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/INSTALL-windows.md
--rw-r--r--   0        0        0     8891 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/INSTALL.md
--rw-r--r--   0        0        0     2771 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/LICENSE.md
--rw-r--r--   0        0        0      393 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/MANIFEST.in
--rw-r--r--   0        0        0     2647 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/Makefile
--rw-r--r--   0        0        0     2802 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/README.md
--rw-r--r--   0        0        0     6778 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/docs/Makefile
--rw-r--r--   0        0        0      759 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/docs/api.rst.inc
--rw-r--r--   0        0        0       31 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/docs/authors.md
--rwxr-xr-x   0        0        0     8521 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/docs/conf.py
--rw-r--r--   0        0        0     3436 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/docs/contributing.rst
--rw-r--r--   0        0        0       33 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/docs/history.md
--rw-r--r--   0        0        0      257 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/docs/index.rst
--rw-r--r--   0        0        0       39 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/docs/install-windows.md
--rw-r--r--   0        0        0       31 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/docs/installation.md
--rw-r--r--   0        0        0       31 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/docs/license.md
--rw-r--r--   0        0        0     6467 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/docs/make.bat
--rw-r--r--   0        0        0       55 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/docs/modules.rst
--rw-r--r--   0        0        0       30 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/docs/readme.md
--rw-r--r--   0        0        0     1337 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/docs/rtmidi.rst
--rw-r--r--   0        0        0     1129 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/docs/usage.rst
--rw-r--r--   0        0        0     1687 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/examples/advanced/ccstore.py
--rw-r--r--   0        0        0     2398 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/examples/advanced/midiclock.py
--rw-r--r--   0        0        0     8741 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/examples/advanced/midioutwrapper.py
--rw-r--r--   0        0        0     2585 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/examples/advanced/recvrpn.py
--rw-r--r--   0        0        0      545 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/examples/basic/contextmanager.py
--rwxr-xr-x   0        0        0     1359 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/examples/basic/midiin_callback.py
--rwxr-xr-x   0        0        0     1050 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/examples/basic/midiin_poll.py
--rwxr-xr-x   0        0        0      991 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/examples/basic/midiout.py
--rw-r--r--   0        0        0     1012 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/examples/basic/noteon2osc.py
--rw-r--r--   0        0        0      765 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/examples/basic/panic.py
--rwxr-xr-x   0        0        0     1571 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/examples/basic/probe_ports.py
--rw-r--r--   0        0        0     2195 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/examples/drumseq/README.rst
--rw-r--r--   0        0        0      275 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/examples/drumseq/break-on-through.txt
--rwxr-xr-x   0        0        0     6485 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/examples/drumseq/drumseq.py
--rw-r--r--   0        0        0      303 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/examples/drumseq/example_01.txt
--rw-r--r--   0        0        0      303 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/examples/drumseq/example_02.txt
--rw-r--r--   0        0        0      255 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/examples/drumseq/example_03.txt
--rw-r--r--   0        0        0      206 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/examples/drumseq/example_04.txt
--rw-r--r--   0        0        0      294 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/examples/drumseq/example_05.txt
--rw-r--r--   0        0        0      303 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/examples/drumseq/example_06.txt
--rw-r--r--   0        0        0      302 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/examples/drumseq/example_07.txt
--rw-r--r--   0        0        0      302 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/examples/drumseq/example_08.txt
--rw-r--r--   0        0        0      434 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/examples/drumseq/example_09.txt
--rw-r--r--   0        0        0      435 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/examples/drumseq/example_10.txt
--rw-r--r--   0        0        0      299 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/examples/drumseq/example_11.txt
--rw-r--r--   0        0        0      347 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/examples/drumseq/example_12.txt
--rw-r--r--   0        0        0      157 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/examples/drumseq/funkydrummer.txt
--rw-r--r--   0        0        0      205 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/examples/drumseq/rosanna-shuffle.txt
--rw-r--r--   0        0        0      477 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/examples/drumseq/template.txt
--rw-r--r--   0        0        0    45974 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/examples/midi2command/000-playback.mp3
--rw-r--r--   0        0        0     2506 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/examples/midi2command/000-sheet.pdf
--rw-r--r--   0        0        0     5624 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/examples/midi2command/README.rst
--rw-r--r--   0        0        0      522 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/examples/midi2command/example.cfg
--rw-r--r--   0        0        0     7132 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/examples/midi2command/midi2command.py
--rw-r--r--   0        0        0        0 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/examples/midifilter/__init__.py
--rw-r--r--   0        0        0     3667 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/examples/midifilter/__main__.py
--rw-r--r--   0        0        0     3119 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/examples/midifilter/filters.py
--rwxr-xr-x   0        0        0     5328 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/examples/sendsysex.py
--rw-r--r--   0        0        0     7155 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/examples/sequencer/sequencer.py
--rwxr-xr-x   0        0        0      745 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/examples/sysex/send_sysex.py
--rwxr-xr-x   0        0        0     1067 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/examples/sysex/send_sysex_file.py
--rw-r--r--   0        0        0        0 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/examples/sysexsaver/__init__.py
--rw-r--r--   0        0        0     7022 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/examples/sysexsaver/__main__.py
--rw-r--r--   0        0        0    11493 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/examples/sysexsaver/manufacturers.csv
--rw-r--r--   0        0        0    12337 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/examples/sysexsaver/manufacturers.py
--rw-r--r--   0        0        0    12147 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/examples/sysexsaver/models.py
--rw-r--r--   0        0        0     3247 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/examples/wavetablemodstep.py
--rw-r--r--   0        0        0     3305 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/meson.build
--rw-r--r--   0        0        0      801 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/meson_options.txt
--rwxr-xr-x   0        0        0      462 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/meson_postinstall.py
--rw-r--r--   0        0        0     3110 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/pyproject.toml
--rw-r--r--   0        0        0       91 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/requirements-dev.in
--rw-r--r--   0        0        0     2686 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/requirements-dev.txt
--rw-r--r--   0        0        0      165 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/rtmidi/__init__.py
--rw-r--r--   0        0        0     1728 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/rtmidi/meson.build
--rw-r--r--   0        0        0     7533 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/rtmidi/midiconstants.py
--rw-r--r--   0        0        0     9261 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/rtmidi/midiutil.py
--rw-r--r--   0        0        0       30 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/rtmidi/version.py.in
--rw-r--r--   0 runner    (1001) docker     (123)   737312 2023-06-23 06:48:00.492697 python_rtmidi-1.5.3/src/_rtmidi.cpp
--rw-r--r--   0        0        0    39588 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/src/_rtmidi.pyx
--rw-r--r--   0        0        0      857 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/src/meson.build
--rwxr-xr-x   0        0        0     1261 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/src/meson_dist_cython.py
--rw-r--r--   0        0        0     9806 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/src/rtmidi/CMakeLists.txt
--rw-r--r--   0        0        0     1349 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/src/rtmidi/LICENSE
--rw-r--r--   0        0        0      533 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/src/rtmidi/Makefile.am
--rw-r--r--   0        0        0     2396 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/src/rtmidi/README.md
--rw-r--r--   0        0        0   126845 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/src/rtmidi/RtMidi.cpp
--rw-r--r--   0        0        0    27079 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/src/rtmidi/RtMidi.h
--rwxr-xr-x   0        0        0     2884 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/src/rtmidi/autogen.sh
--rw-r--r--   0        0        0      940 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/src/rtmidi/cmake/RtMidiConfigUninstall.cmake.in
--rw-r--r--   0        0        0      277 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/src/rtmidi/cmake/rtmidi-config.cmake.in
--rw-r--r--   0        0        0     9307 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/src/rtmidi/configure.ac
--rw-r--r--   0        0        0       59 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/src/rtmidi/contrib/go/rtmidi/go.mod
--rw-r--r--   0        0        0    10504 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/src/rtmidi/contrib/go/rtmidi/rtmidi.go
--rw-r--r--   0        0        0      125 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/src/rtmidi/contrib/go/rtmidi/rtmidi_stub.cpp
--rw-r--r--   0        0        0       31 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/src/rtmidi/contrib/go/rtmidi/rtmidi_stub.h
--rw-r--r--   0        0        0      758 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/src/rtmidi/contrib/go/rtmidi/rtmidi_test.go
--rw-r--r--   0        0        0      682 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/src/rtmidi/doc/Makefile.am
--rw-r--r--   0        0        0    81155 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/src/rtmidi/doc/doxygen/Doxyfile.in
--rw-r--r--   0        0        0      254 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/src/rtmidi/doc/doxygen/footer.html
--rw-r--r--   0        0        0      494 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/src/rtmidi/doc/doxygen/header.html
--rw-r--r--   0        0        0      173 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/src/rtmidi/doc/doxygen/samples/getting_started.cpp
--rw-r--r--   0        0        0    21717 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/src/rtmidi/doc/doxygen/tutorial.txt
--rw-r--r--   0        0        0     3527 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/src/rtmidi/doc/images/ccrma.gif
--rw-r--r--   0        0        0     4614 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/src/rtmidi/doc/images/mcgill.gif
--rw-r--r--   0        0        0     7130 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/src/rtmidi/doc/release.txt
--rw-r--r--   0        0        0    19367 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/src/rtmidi/m4/ax_cxx_compile_stdcxx.m4
--rw-r--r--   0        0        0      171 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/src/rtmidi/msw/readme
--rwxr-xr-x   0        0        0      883 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/src/rtmidi/msw/rtmidilib.sln
--rwxr-xr-x   0        0        0     3734 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/src/rtmidi/msw/rtmidilib.vcproj
--rw-r--r--   0        0        0      388 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/src/rtmidi/rtmidi-config.in
--rw-r--r--   0        0        0      369 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/src/rtmidi/rtmidi.pc.in
--rw-r--r--   0        0        0    10218 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/src/rtmidi/rtmidi_c.cpp
--rw-r--r--   0        0        0     9532 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/src/rtmidi/rtmidi_c.h
--rw-r--r--   0        0        0        0 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/src/rtmidi/tests/Debug/.placeholder
--rw-r--r--   0        0        0     1018 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/src/rtmidi/tests/Makefile.am
--rw-r--r--   0        0        0        0 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/src/rtmidi/tests/Release/.placeholder
--rw-r--r--   0        0        0     1311 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/src/rtmidi/tests/RtMidi.dsw
--rw-r--r--   0        0        0     5284 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/src/rtmidi/tests/apinames.cpp
--rw-r--r--   0        0        0     2873 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/src/rtmidi/tests/cmidiin.cpp
--rw-r--r--   0        0        0     4320 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/src/rtmidi/tests/cmidiin.dsp
--rw-r--r--   0        0        0     5541 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/src/rtmidi/tests/midiclock.cpp
--rw-r--r--   0        0        0     3147 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/src/rtmidi/tests/midiout.cpp
--rw-r--r--   0        0        0     4320 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/src/rtmidi/tests/midiout.dsp
--rw-r--r--   0        0        0     2138 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/src/rtmidi/tests/midiprobe.cpp
--rw-r--r--   0        0        0     4356 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/src/rtmidi/tests/midiprobe.dsp
--rw-r--r--   0        0        0     2361 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/src/rtmidi/tests/qmidiin.cpp
--rw-r--r--   0        0        0     4320 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/src/rtmidi/tests/qmidiin.dsp
--rw-r--r--   0        0        0     3926 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/src/rtmidi/tests/sysextest.cpp
--rw-r--r--   0        0        0     4360 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/src/rtmidi/tests/sysextest.dsp
--rw-r--r--   0        0        0      667 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/src/rtmidi/tests/testcapi.c
--rw-r--r--   0        0        0     2823 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/tests/test_basic.py
--rw-r--r--   0        0        0      907 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/tests/test_ci_wheels.py
--rw-r--r--   0        0        0     2460 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/tests/test_delete.py
--rw-r--r--   0        0        0     2055 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/tests/test_errorcallback.py
--rw-r--r--   0        0        0     2276 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/tests/test_errors.py
--rw-r--r--   0        0        0     7000 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/tests/test_rtmidi.py
--rw-r--r--   0        0        0      298 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/tox.ini
--rwxr-xr-x   0        0        0      346 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/update-docs.sh
--rw-r--r--   0        0        0     7498 1970-01-01 00:00:00.000000 python_rtmidi-1.5.3/PKG-INFO
+-rw-r--r--   0        0        0       94 1970-01-01 00:00:00.000000 python_rtmidi-1.5.4/.flake8
+-rw-r--r--   0        0        0     1903 1970-01-01 00:00:00.000000 python_rtmidi-1.5.4/.github/workflows/pr_to_master.yml
+-rw-r--r--   0        0        0     2603 1970-01-01 00:00:00.000000 python_rtmidi-1.5.4/.github/workflows/push_to_master.yml
+-rw-r--r--   0        0        0     2539 1970-01-01 00:00:00.000000 python_rtmidi-1.5.4/.github/workflows/release.yml
+-rw-r--r--   0        0        0      571 1970-01-01 00:00:00.000000 python_rtmidi-1.5.4/.gitignore
+-rw-r--r--   0        0        0      118 1970-01-01 00:00:00.000000 python_rtmidi-1.5.4/.gitmodules
+-rw-r--r--   0        0        0      295 1970-01-01 00:00:00.000000 python_rtmidi-1.5.4/AUTHORS.md
+-rw-r--r--   0        0        0    22884 1970-01-01 00:00:00.000000 python_rtmidi-1.5.4/CHANGELOG.md
+-rw-r--r--   0        0        0     3849 1970-01-01 00:00:00.000000 python_rtmidi-1.5.4/INSTALL-windows.md
+-rw-r--r--   0        0        0     8891 1970-01-01 00:00:00.000000 python_rtmidi-1.5.4/INSTALL.md
+-rw-r--r--   0        0        0     2771 1970-01-01 00:00:00.000000 python_rtmidi-1.5.4/LICENSE.md
+-rw-r--r--   0        0        0      393 1970-01-01 00:00:00.000000 python_rtmidi-1.5.4/MANIFEST.in
+-rw-r--r--   0        0        0     2647 1970-01-01 00:00:00.000000 python_rtmidi-1.5.4/Makefile
+-rw-r--r--   0        0        0     2802 1970-01-01 00:00:00.000000 python_rtmidi-1.5.4/README.md
+-rw-r--r--   0        0        0     6778 1970-01-01 00:00:00.000000 python_rtmidi-1.5.4/docs/Makefile
+-rw-r--r--   0        0        0      759 1970-01-01 00:00:00.000000 python_rtmidi-1.5.4/docs/api.rst.inc
+-rw-r--r--   0        0        0       31 1970-01-01 00:00:00.000000 python_rtmidi-1.5.4/docs/authors.md
+-rwxr-xr-x   0        0        0     8521 1970-01-01 00:00:00.000000 python_rtmidi-1.5.4/docs/conf.py
+-rw-r--r--   0        0        0     3436 1970-01-01 00:00:00.000000 python_rtmidi-1.5.4/docs/contributing.rst
+-rw-r--r--   0        0        0       33 1970-01-01 00:00:00.000000 python_rtmidi-1.5.4/docs/history.md
+-rw-r--r--   0        0        0      257 1970-01-01 00:00:00.000000 python_rtmidi-1.5.4/docs/index.rst
+-rw-r--r--   0        0        0       39 1970-01-01 00:00:00.000000 python_rtmidi-1.5.4/docs/install-windows.md
+-rw-r--r--   0        0        0       31 1970-01-01 00:00:00.000000 python_rtmidi-1.5.4/docs/installation.md
+-rw-r--r--   0        0        0       31 1970-01-01 00:00:00.000000 python_rtmidi-1.5.4/docs/license.md
+-rw-r--r--   0        0        0     6467 1970-01-01 00:00:00.000000 python_rtmidi-1.5.4/docs/make.bat
+-rw-r--r--   0        0        0       55 1970-01-01 00:00:00.000000 python_rtmidi-1.5.4/docs/modules.rst
+-rw-r--r--   0        0        0       30 1970-01-01 00:00:00.000000 python_rtmidi-1.5.4/docs/readme.md
+-rw-r--r--   0        0        0     1337 1970-01-01 00:00:00.000000 python_rtmidi-1.5.4/docs/rtmidi.rst
+-rw-r--r--   0        0        0     1129 1970-01-01 00:00:00.000000 python_rtmidi-1.5.4/docs/usage.rst
+-rw-r--r--   0        0        0     1687 1970-01-01 00:00:00.000000 python_rtmidi-1.5.4/examples/advanced/ccstore.py
+-rw-r--r--   0        0        0     2398 1970-01-01 00:00:00.000000 python_rtmidi-1.5.4/examples/advanced/midiclock.py
+-rw-r--r--   0        0        0     8741 1970-01-01 00:00:00.000000 python_rtmidi-1.5.4/examples/advanced/midioutwrapper.py
+-rw-r--r--   0        0        0     2585 1970-01-01 00:00:00.000000 python_rtmidi-1.5.4/examples/advanced/recvrpn.py
+-rw-r--r--   0        0        0     2447 1970-01-01 00:00:00.000000 python_rtmidi-1.5.4/examples/advanced/send_all.py
+-rw-r--r--   0        0        0      545 1970-01-01 00:00:00.000000 python_rtmidi-1.5.4/examples/basic/contextmanager.py
+-rwxr-xr-x   0        0        0     1359 1970-01-01 00:00:00.000000 python_rtmidi-1.5.4/examples/basic/midiin_callback.py
+-rwxr-xr-x   0        0        0     1050 1970-01-01 00:00:00.000000 python_rtmidi-1.5.4/examples/basic/midiin_poll.py
+-rwxr-xr-x   0        0        0      991 1970-01-01 00:00:00.000000 python_rtmidi-1.5.4/examples/basic/midiout.py
+-rw-r--r--   0        0        0     1012 1970-01-01 00:00:00.000000 python_rtmidi-1.5.4/examples/basic/noteon2osc.py
+-rw-r--r--   0        0        0      765 1970-01-01 00:00:00.000000 python_rtmidi-1.5.4/examples/basic/panic.py
+-rwxr-xr-x   0        0        0     1571 1970-01-01 00:00:00.000000 python_rtmidi-1.5.4/examples/basic/probe_ports.py
+-rw-r--r--   0        0        0     2195 1970-01-01 00:00:00.000000 python_rtmidi-1.5.4/examples/drumseq/README.rst
+-rw-r--r--   0        0        0      275 1970-01-01 00:00:00.000000 python_rtmidi-1.5.4/examples/drumseq/break-on-through.txt
+-rwxr-xr-x   0        0        0     6485 1970-01-01 00:00:00.000000 python_rtmidi-1.5.4/examples/drumseq/drumseq.py
+-rw-r--r--   0        0        0      303 1970-01-01 00:00:00.000000 python_rtmidi-1.5.4/examples/drumseq/example_01.txt
+-rw-r--r--   0        0        0      303 1970-01-01 00:00:00.000000 python_rtmidi-1.5.4/examples/drumseq/example_02.txt
+-rw-r--r--   0        0        0      255 1970-01-01 00:00:00.000000 python_rtmidi-1.5.4/examples/drumseq/example_03.txt
+-rw-r--r--   0        0        0      206 1970-01-01 00:00:00.000000 python_rtmidi-1.5.4/examples/drumseq/example_04.txt
+-rw-r--r--   0        0        0      294 1970-01-01 00:00:00.000000 python_rtmidi-1.5.4/examples/drumseq/example_05.txt
+-rw-r--r--   0        0        0      303 1970-01-01 00:00:00.000000 python_rtmidi-1.5.4/examples/drumseq/example_06.txt
+-rw-r--r--   0        0        0      302 1970-01-01 00:00:00.000000 python_rtmidi-1.5.4/examples/drumseq/example_07.txt
+-rw-r--r--   0        0        0      302 1970-01-01 00:00:00.000000 python_rtmidi-1.5.4/examples/drumseq/example_08.txt
+-rw-r--r--   0        0        0      434 1970-01-01 00:00:00.000000 python_rtmidi-1.5.4/examples/drumseq/example_09.txt
+-rw-r--r--   0        0        0      435 1970-01-01 00:00:00.000000 python_rtmidi-1.5.4/examples/drumseq/example_10.txt
+-rw-r--r--   0        0        0      299 1970-01-01 00:00:00.000000 python_rtmidi-1.5.4/examples/drumseq/example_11.txt
+-rw-r--r--   0        0        0      347 1970-01-01 00:00:00.000000 python_rtmidi-1.5.4/examples/drumseq/example_12.txt
+-rw-r--r--   0        0        0      157 1970-01-01 00:00:00.000000 python_rtmidi-1.5.4/examples/drumseq/funkydrummer.txt
+-rw-r--r--   0        0        0      205 1970-01-01 00:00:00.000000 python_rtmidi-1.5.4/examples/drumseq/rosanna-shuffle.txt
+-rw-r--r--   0        0        0      477 1970-01-01 00:00:00.000000 python_rtmidi-1.5.4/examples/drumseq/template.txt
+-rw-r--r--   0        0        0    45974 1970-01-01 00:00:00.000000 python_rtmidi-1.5.4/examples/midi2command/000-playback.mp3
+-rw-r--r--   0        0        0     2506 1970-01-01 00:00:00.000000 python_rtmidi-1.5.4/examples/midi2command/000-sheet.pdf
+-rw-r--r--   0        0        0     5624 1970-01-01 00:00:00.000000 python_rtmidi-1.5.4/examples/midi2command/README.rst
+-rw-r--r--   0        0        0      522 1970-01-01 00:00:00.000000 python_rtmidi-1.5.4/examples/midi2command/example.cfg
+-rw-r--r--   0        0        0     7132 1970-01-01 00:00:00.000000 python_rtmidi-1.5.4/examples/midi2command/midi2command.py
+-rw-r--r--   0        0        0        0 1970-01-01 00:00:00.000000 python_rtmidi-1.5.4/examples/midifilter/__init__.py
+-rw-r--r--   0        0        0     3667 1970-01-01 00:00:00.000000 python_rtmidi-1.5.4/examples/midifilter/__main__.py
+-rw-r--r--   0        0        0     3119 1970-01-01 00:00:00.000000 python_rtmidi-1.5.4/examples/midifilter/filters.py
+-rwxr-xr-x   0        0        0     5328 1970-01-01 00:00:00.000000 python_rtmidi-1.5.4/examples/sendsysex.py
+-rw-r--r--   0        0        0     7155 1970-01-01 00:00:00.000000 python_rtmidi-1.5.4/examples/sequencer/sequencer.py
+-rwxr-xr-x   0        0        0      745 1970-01-01 00:00:00.000000 python_rtmidi-1.5.4/examples/sysex/send_sysex.py
+-rwxr-xr-x   0        0        0     1067 1970-01-01 00:00:00.000000 python_rtmidi-1.5.4/examples/sysex/send_sysex_file.py
+-rw-r--r--   0        0        0        0 1970-01-01 00:00:00.000000 python_rtmidi-1.5.4/examples/sysexsaver/__init__.py
+-rw-r--r--   0        0        0     7022 1970-01-01 00:00:00.000000 python_rtmidi-1.5.4/examples/sysexsaver/__main__.py
+-rw-r--r--   0        0        0    11493 1970-01-01 00:00:00.000000 python_rtmidi-1.5.4/examples/sysexsaver/manufacturers.csv
+-rw-r--r--   0        0        0    12337 1970-01-01 00:00:00.000000 python_rtmidi-1.5.4/examples/sysexsaver/manufacturers.py
+-rw-r--r--   0        0        0    12147 1970-01-01 00:00:00.000000 python_rtmidi-1.5.4/examples/sysexsaver/models.py
+-rw-r--r--   0        0        0     3247 1970-01-01 00:00:00.000000 python_rtmidi-1.5.4/examples/wavetablemodstep.py
+-rw-r--r--   0        0        0     3380 1970-01-01 00:00:00.000000 python_rtmidi-1.5.4/meson.build
+-rw-r--r--   0        0        0      801 1970-01-01 00:00:00.000000 python_rtmidi-1.5.4/meson_options.txt
+-rwxr-xr-x   0        0        0      462 1970-01-01 00:00:00.000000 python_rtmidi-1.5.4/meson_postinstall.py
+-rw-r--r--   0        0        0     3110 1970-01-01 00:00:00.000000 python_rtmidi-1.5.4/pyproject.toml
+-rw-r--r--   0        0        0       91 1970-01-01 00:00:00.000000 python_rtmidi-1.5.4/requirements-dev.in
+-rw-r--r--   0        0        0     2686 1970-01-01 00:00:00.000000 python_rtmidi-1.5.4/requirements-dev.txt
+-rw-r--r--   0        0        0      165 1970-01-01 00:00:00.000000 python_rtmidi-1.5.4/rtmidi/__init__.py
+-rw-r--r--   0        0        0     1728 1970-01-01 00:00:00.000000 python_rtmidi-1.5.4/rtmidi/meson.build
+-rw-r--r--   0        0        0     7533 1970-01-01 00:00:00.000000 python_rtmidi-1.5.4/rtmidi/midiconstants.py
+-rw-r--r--   0        0        0     9261 1970-01-01 00:00:00.000000 python_rtmidi-1.5.4/rtmidi/midiutil.py
+-rw-r--r--   0        0        0       30 1970-01-01 00:00:00.000000 python_rtmidi-1.5.4/rtmidi/version.py.in
+-rw-r--r--   0 runner    (1001) docker     (123)   737312 2023-06-27 11:23:46.926165 python_rtmidi-1.5.4/src/_rtmidi.cpp
+-rw-r--r--   0        0        0    39588 1970-01-01 00:00:00.000000 python_rtmidi-1.5.4/src/_rtmidi.pyx
+-rw-r--r--   0        0        0      857 1970-01-01 00:00:00.000000 python_rtmidi-1.5.4/src/meson.build
+-rwxr-xr-x   0        0        0     1261 1970-01-01 00:00:00.000000 python_rtmidi-1.5.4/src/meson_dist_cython.py
+-rw-r--r--   0        0        0     9806 1970-01-01 00:00:00.000000 python_rtmidi-1.5.4/src/rtmidi/CMakeLists.txt
+-rw-r--r--   0        0        0     1349 1970-01-01 00:00:00.000000 python_rtmidi-1.5.4/src/rtmidi/LICENSE
+-rw-r--r--   0        0        0      533 1970-01-01 00:00:00.000000 python_rtmidi-1.5.4/src/rtmidi/Makefile.am
+-rw-r--r--   0        0        0     2396 1970-01-01 00:00:00.000000 python_rtmidi-1.5.4/src/rtmidi/README.md
+-rw-r--r--   0        0        0   126845 1970-01-01 00:00:00.000000 python_rtmidi-1.5.4/src/rtmidi/RtMidi.cpp
+-rw-r--r--   0        0        0    27079 1970-01-01 00:00:00.000000 python_rtmidi-1.5.4/src/rtmidi/RtMidi.h
+-rwxr-xr-x   0        0        0     2884 1970-01-01 00:00:00.000000 python_rtmidi-1.5.4/src/rtmidi/autogen.sh
+-rw-r--r--   0        0        0      940 1970-01-01 00:00:00.000000 python_rtmidi-1.5.4/src/rtmidi/cmake/RtMidiConfigUninstall.cmake.in
+-rw-r--r--   0        0        0      277 1970-01-01 00:00:00.000000 python_rtmidi-1.5.4/src/rtmidi/cmake/rtmidi-config.cmake.in
+-rw-r--r--   0        0        0     9307 1970-01-01 00:00:00.000000 python_rtmidi-1.5.4/src/rtmidi/configure.ac
+-rw-r--r--   0        0        0       59 1970-01-01 00:00:00.000000 python_rtmidi-1.5.4/src/rtmidi/contrib/go/rtmidi/go.mod
+-rw-r--r--   0        0        0    10504 1970-01-01 00:00:00.000000 python_rtmidi-1.5.4/src/rtmidi/contrib/go/rtmidi/rtmidi.go
+-rw-r--r--   0        0        0      125 1970-01-01 00:00:00.000000 python_rtmidi-1.5.4/src/rtmidi/contrib/go/rtmidi/rtmidi_stub.cpp
+-rw-r--r--   0        0        0       31 1970-01-01 00:00:00.000000 python_rtmidi-1.5.4/src/rtmidi/contrib/go/rtmidi/rtmidi_stub.h
+-rw-r--r--   0        0        0      758 1970-01-01 00:00:00.000000 python_rtmidi-1.5.4/src/rtmidi/contrib/go/rtmidi/rtmidi_test.go
+-rw-r--r--   0        0        0      682 1970-01-01 00:00:00.000000 python_rtmidi-1.5.4/src/rtmidi/doc/Makefile.am
+-rw-r--r--   0        0        0    81155 1970-01-01 00:00:00.000000 python_rtmidi-1.5.4/src/rtmidi/doc/doxygen/Doxyfile.in
+-rw-r--r--   0        0        0      254 1970-01-01 00:00:00.000000 python_rtmidi-1.5.4/src/rtmidi/doc/doxygen/footer.html
+-rw-r--r--   0        0        0      494 1970-01-01 00:00:00.000000 python_rtmidi-1.5.4/src/rtmidi/doc/doxygen/header.html
+-rw-r--r--   0        0        0      173 1970-01-01 00:00:00.000000 python_rtmidi-1.5.4/src/rtmidi/doc/doxygen/samples/getting_started.cpp
+-rw-r--r--   0        0        0    21717 1970-01-01 00:00:00.000000 python_rtmidi-1.5.4/src/rtmidi/doc/doxygen/tutorial.txt
+-rw-r--r--   0        0        0     3527 1970-01-01 00:00:00.000000 python_rtmidi-1.5.4/src/rtmidi/doc/images/ccrma.gif
+-rw-r--r--   0        0        0     4614 1970-01-01 00:00:00.000000 python_rtmidi-1.5.4/src/rtmidi/doc/images/mcgill.gif
+-rw-r--r--   0        0        0     7130 1970-01-01 00:00:00.000000 python_rtmidi-1.5.4/src/rtmidi/doc/release.txt
+-rw-r--r--   0        0        0    19367 1970-01-01 00:00:00.000000 python_rtmidi-1.5.4/src/rtmidi/m4/ax_cxx_compile_stdcxx.m4
+-rw-r--r--   0        0        0      171 1970-01-01 00:00:00.000000 python_rtmidi-1.5.4/src/rtmidi/msw/readme
+-rwxr-xr-x   0        0        0      883 1970-01-01 00:00:00.000000 python_rtmidi-1.5.4/src/rtmidi/msw/rtmidilib.sln
+-rwxr-xr-x   0        0        0     3734 1970-01-01 00:00:00.000000 python_rtmidi-1.5.4/src/rtmidi/msw/rtmidilib.vcproj
+-rw-r--r--   0        0        0      388 1970-01-01 00:00:00.000000 python_rtmidi-1.5.4/src/rtmidi/rtmidi-config.in
+-rw-r--r--   0        0        0      369 1970-01-01 00:00:00.000000 python_rtmidi-1.5.4/src/rtmidi/rtmidi.pc.in
+-rw-r--r--   0        0        0    10218 1970-01-01 00:00:00.000000 python_rtmidi-1.5.4/src/rtmidi/rtmidi_c.cpp
+-rw-r--r--   0        0        0     9532 1970-01-01 00:00:00.000000 python_rtmidi-1.5.4/src/rtmidi/rtmidi_c.h
+-rw-r--r--   0        0        0        0 1970-01-01 00:00:00.000000 python_rtmidi-1.5.4/src/rtmidi/tests/Debug/.placeholder
+-rw-r--r--   0        0        0     1018 1970-01-01 00:00:00.000000 python_rtmidi-1.5.4/src/rtmidi/tests/Makefile.am
+-rw-r--r--   0        0        0        0 1970-01-01 00:00:00.000000 python_rtmidi-1.5.4/src/rtmidi/tests/Release/.placeholder
+-rw-r--r--   0        0        0     1311 1970-01-01 00:00:00.000000 python_rtmidi-1.5.4/src/rtmidi/tests/RtMidi.dsw
+-rw-r--r--   0        0        0     5284 1970-01-01 00:00:00.000000 python_rtmidi-1.5.4/src/rtmidi/tests/apinames.cpp
+-rw-r--r--   0        0        0     2873 1970-01-01 00:00:00.000000 python_rtmidi-1.5.4/src/rtmidi/tests/cmidiin.cpp
+-rw-r--r--   0        0        0     4320 1970-01-01 00:00:00.000000 python_rtmidi-1.5.4/src/rtmidi/tests/cmidiin.dsp
+-rw-r--r--   0        0        0     5541 1970-01-01 00:00:00.000000 python_rtmidi-1.5.4/src/rtmidi/tests/midiclock.cpp
+-rw-r--r--   0        0        0     3147 1970-01-01 00:00:00.000000 python_rtmidi-1.5.4/src/rtmidi/tests/midiout.cpp
+-rw-r--r--   0        0        0     4320 1970-01-01 00:00:00.000000 python_rtmidi-1.5.4/src/rtmidi/tests/midiout.dsp
+-rw-r--r--   0        0        0     2138 1970-01-01 00:00:00.000000 python_rtmidi-1.5.4/src/rtmidi/tests/midiprobe.cpp
+-rw-r--r--   0        0        0     4356 1970-01-01 00:00:00.000000 python_rtmidi-1.5.4/src/rtmidi/tests/midiprobe.dsp
+-rw-r--r--   0        0        0     2361 1970-01-01 00:00:00.000000 python_rtmidi-1.5.4/src/rtmidi/tests/qmidiin.cpp
+-rw-r--r--   0        0        0     4320 1970-01-01 00:00:00.000000 python_rtmidi-1.5.4/src/rtmidi/tests/qmidiin.dsp
+-rw-r--r--   0        0        0     3926 1970-01-01 00:00:00.000000 python_rtmidi-1.5.4/src/rtmidi/tests/sysextest.cpp
+-rw-r--r--   0        0        0     4360 1970-01-01 00:00:00.000000 python_rtmidi-1.5.4/src/rtmidi/tests/sysextest.dsp
+-rw-r--r--   0        0        0      667 1970-01-01 00:00:00.000000 python_rtmidi-1.5.4/src/rtmidi/tests/testcapi.c
+-rw-r--r--   0        0        0     2823 1970-01-01 00:00:00.000000 python_rtmidi-1.5.4/tests/test_basic.py
+-rw-r--r--   0        0        0      907 1970-01-01 00:00:00.000000 python_rtmidi-1.5.4/tests/test_ci_wheels.py
+-rw-r--r--   0        0        0     2460 1970-01-01 00:00:00.000000 python_rtmidi-1.5.4/tests/test_delete.py
+-rw-r--r--   0        0        0     2055 1970-01-01 00:00:00.000000 python_rtmidi-1.5.4/tests/test_errorcallback.py
+-rw-r--r--   0        0        0     2276 1970-01-01 00:00:00.000000 python_rtmidi-1.5.4/tests/test_errors.py
+-rw-r--r--   0        0        0     7000 1970-01-01 00:00:00.000000 python_rtmidi-1.5.4/tests/test_rtmidi.py
+-rw-r--r--   0        0        0      298 1970-01-01 00:00:00.000000 python_rtmidi-1.5.4/tox.ini
+-rwxr-xr-x   0        0        0      346 1970-01-01 00:00:00.000000 python_rtmidi-1.5.4/update-docs.sh
+-rw-r--r--   0        0        0     7498 1970-01-01 00:00:00.000000 python_rtmidi-1.5.4/PKG-INFO
```

### Comparing `python_rtmidi-1.5.3/.github/workflows/pr_to_master.yml` & `python_rtmidi-1.5.4/.github/workflows/pr_to_master.yml`

 * *Files identical despite different names*

### Comparing `python_rtmidi-1.5.3/.github/workflows/push_to_master.yml` & `python_rtmidi-1.5.4/.github/workflows/push_to_master.yml`

 * *Files identical despite different names*

### Comparing `python_rtmidi-1.5.3/.github/workflows/release.yml` & `python_rtmidi-1.5.4/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `python_rtmidi-1.5.3/.gitignore` & `python_rtmidi-1.5.4/.gitignore`

 * *Files identical despite different names*

### Comparing `python_rtmidi-1.5.3/CHANGELOG.md` & `python_rtmidi-1.5.4/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,25 @@
 # Changelog
 
 For details and minor changes, please see the [version control log
 messages](https://github.com/SpotlightKid/python-rtmidi/commits/master).
 
-## Development
+
+## 1.5.4 (2023-06-27)
+
+Changes:
+
+-   Added `send_all.py` script to examples (#167).
+
+Project infrastructure:
+
+-   Fixed macOS arm64 binary wheels built by CI without CoreMIDI support (#169).
+
+
+## 1.5.3 (2023-06-23)
 
 Changes:
 
 -   Updated `rtmidi` submodule (#156).
 
 Documentation:
```

### Comparing `python_rtmidi-1.5.3/INSTALL-windows.md` & `python_rtmidi-1.5.4/INSTALL-windows.md`

 * *Files identical despite different names*

### Comparing `python_rtmidi-1.5.3/INSTALL.md` & `python_rtmidi-1.5.4/INSTALL.md`

 * *Files identical despite different names*

### Comparing `python_rtmidi-1.5.3/LICENSE.md` & `python_rtmidi-1.5.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `python_rtmidi-1.5.3/Makefile` & `python_rtmidi-1.5.4/Makefile`

 * *Files identical despite different names*

### Comparing `python_rtmidi-1.5.3/README.md` & `python_rtmidi-1.5.4/README.md`

 * *Files identical despite different names*

### Comparing `python_rtmidi-1.5.3/docs/Makefile` & `python_rtmidi-1.5.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `python_rtmidi-1.5.3/docs/api.rst.inc` & `python_rtmidi-1.5.4/docs/api.rst.inc`

 * *Files identical despite different names*

### Comparing `python_rtmidi-1.5.3/docs/conf.py` & `python_rtmidi-1.5.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `python_rtmidi-1.5.3/docs/contributing.rst` & `python_rtmidi-1.5.4/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `python_rtmidi-1.5.3/docs/make.bat` & `python_rtmidi-1.5.4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `python_rtmidi-1.5.3/docs/rtmidi.rst` & `python_rtmidi-1.5.4/docs/rtmidi.rst`

 * *Files identical despite different names*

### Comparing `python_rtmidi-1.5.3/docs/usage.rst` & `python_rtmidi-1.5.4/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `python_rtmidi-1.5.3/examples/advanced/ccstore.py` & `python_rtmidi-1.5.4/examples/advanced/ccstore.py`

 * *Files identical despite different names*

### Comparing `python_rtmidi-1.5.3/examples/advanced/midiclock.py` & `python_rtmidi-1.5.4/examples/advanced/midiclock.py`

 * *Files identical despite different names*

### Comparing `python_rtmidi-1.5.3/examples/advanced/midioutwrapper.py` & `python_rtmidi-1.5.4/examples/advanced/midioutwrapper.py`

 * *Files identical despite different names*

### Comparing `python_rtmidi-1.5.3/examples/advanced/recvrpn.py` & `python_rtmidi-1.5.4/examples/advanced/recvrpn.py`

 * *Files identical despite different names*

### Comparing `python_rtmidi-1.5.3/examples/basic/contextmanager.py` & `python_rtmidi-1.5.4/examples/basic/contextmanager.py`

 * *Files identical despite different names*

### Comparing `python_rtmidi-1.5.3/examples/basic/midiin_callback.py` & `python_rtmidi-1.5.4/examples/basic/midiin_callback.py`

 * *Files identical despite different names*

### Comparing `python_rtmidi-1.5.3/examples/basic/midiin_poll.py` & `python_rtmidi-1.5.4/examples/basic/midiin_poll.py`

 * *Files identical despite different names*

### Comparing `python_rtmidi-1.5.3/examples/basic/midiout.py` & `python_rtmidi-1.5.4/examples/basic/midiout.py`

 * *Files identical despite different names*

### Comparing `python_rtmidi-1.5.3/examples/basic/noteon2osc.py` & `python_rtmidi-1.5.4/examples/basic/noteon2osc.py`

 * *Files identical despite different names*

### Comparing `python_rtmidi-1.5.3/examples/basic/panic.py` & `python_rtmidi-1.5.4/examples/basic/panic.py`

 * *Files identical despite different names*

### Comparing `python_rtmidi-1.5.3/examples/basic/probe_ports.py` & `python_rtmidi-1.5.4/examples/basic/probe_ports.py`

 * *Files identical despite different names*

### Comparing `python_rtmidi-1.5.3/examples/drumseq/README.rst` & `python_rtmidi-1.5.4/examples/drumseq/README.rst`

 * *Files identical despite different names*

### Comparing `python_rtmidi-1.5.3/examples/drumseq/drumseq.py` & `python_rtmidi-1.5.4/examples/drumseq/drumseq.py`

 * *Files identical despite different names*

### Comparing `python_rtmidi-1.5.3/examples/midi2command/000-playback.mp3` & `python_rtmidi-1.5.4/examples/midi2command/000-playback.mp3`

 * *Files identical despite different names*

### Comparing `python_rtmidi-1.5.3/examples/midi2command/000-sheet.pdf` & `python_rtmidi-1.5.4/examples/midi2command/000-sheet.pdf`

 * *Files identical despite different names*

### Comparing `python_rtmidi-1.5.3/examples/midi2command/README.rst` & `python_rtmidi-1.5.4/examples/midi2command/README.rst`

 * *Files identical despite different names*

### Comparing `python_rtmidi-1.5.3/examples/midi2command/example.cfg` & `python_rtmidi-1.5.4/examples/midi2command/example.cfg`

 * *Files identical despite different names*

### Comparing `python_rtmidi-1.5.3/examples/midi2command/midi2command.py` & `python_rtmidi-1.5.4/examples/midi2command/midi2command.py`

 * *Files identical despite different names*

### Comparing `python_rtmidi-1.5.3/examples/midifilter/__main__.py` & `python_rtmidi-1.5.4/examples/midifilter/__main__.py`

 * *Files identical despite different names*

### Comparing `python_rtmidi-1.5.3/examples/midifilter/filters.py` & `python_rtmidi-1.5.4/examples/midifilter/filters.py`

 * *Files identical despite different names*

### Comparing `python_rtmidi-1.5.3/examples/sendsysex.py` & `python_rtmidi-1.5.4/examples/sendsysex.py`

 * *Files identical despite different names*

### Comparing `python_rtmidi-1.5.3/examples/sequencer/sequencer.py` & `python_rtmidi-1.5.4/examples/sequencer/sequencer.py`

 * *Files identical despite different names*

### Comparing `python_rtmidi-1.5.3/examples/sysex/send_sysex.py` & `python_rtmidi-1.5.4/examples/sysex/send_sysex.py`

 * *Files identical despite different names*

### Comparing `python_rtmidi-1.5.3/examples/sysex/send_sysex_file.py` & `python_rtmidi-1.5.4/examples/sysex/send_sysex_file.py`

 * *Files identical despite different names*

### Comparing `python_rtmidi-1.5.3/examples/sysexsaver/__main__.py` & `python_rtmidi-1.5.4/examples/sysexsaver/__main__.py`

 * *Files identical despite different names*

### Comparing `python_rtmidi-1.5.3/examples/sysexsaver/manufacturers.csv` & `python_rtmidi-1.5.4/examples/sysexsaver/manufacturers.csv`

 * *Files identical despite different names*

### Comparing `python_rtmidi-1.5.3/examples/sysexsaver/manufacturers.py` & `python_rtmidi-1.5.4/examples/sysexsaver/manufacturers.py`

 * *Files identical despite different names*

### Comparing `python_rtmidi-1.5.3/examples/sysexsaver/models.py` & `python_rtmidi-1.5.4/examples/sysexsaver/models.py`

 * *Files identical despite different names*

### Comparing `python_rtmidi-1.5.3/examples/wavetablemodstep.py` & `python_rtmidi-1.5.4/examples/wavetablemodstep.py`

 * *Files identical despite different names*

### Comparing `python_rtmidi-1.5.3/meson.build` & `python_rtmidi-1.5.4/meson.build`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 project(
     'python-rtmidi',
     'cpp',
-    version: '1.5.3',
+    version: '1.5.4',
     license: 'MIT',
     default_options: [
         'warning_level=2',
         'cpp_std=c++11'
     ],
     meson_version: '>=0.64.0'
 )
 
-message('Host machine system:', host_machine.system())
-
 cpp = meson.get_compiler('cpp')
 
 # Jack API (portable)
 jack2_dep = dependency('jack', version: '>=1.9.11', required: false)
 jack1_dep = dependency('jack', version: ['>=0.125.0', '<1.0'], required: false)
 
 if not jack2_dep.found() and jack1_dep.found()
@@ -65,17 +63,17 @@
     # LINUX
 
     # API
     alsa_dep = dependency('alsa', required: jack_not_found)
 endif # Platform detection
 
 jack_support = jack_dep.found() and get_option('jack')
-alsa_support = host_machine.system() == 'linux' and alsa_dep.found() and get_option('alsa')
-coremidi_support = host_machine.system() == 'darwin' and coremidi_dep.found() and get_option('coremidi')
-winmm_support = host_machine.system() == 'windows' and winmm_dep.found() and get_option('winmm')
+alsa_support = host_machine.system().to_lower() == 'linux' and alsa_dep.found() and get_option('alsa')
+coremidi_support = host_machine.system().to_lower() == 'darwin' and coremidi_dep.found() and get_option('coremidi')
+winmm_support = host_machine.system().to_lower() == 'windows' and winmm_dep.found() and get_option('winmm')
 
 threads_dep = dependency('threads', required: alsa_support or jack_support)
 have_semaphore = cpp.has_header('semaphore.h')
 
 pymod = import('python')
 python = pymod.find_installation(get_option('python'), required: true, pure: false)
 
@@ -87,15 +85,16 @@
 
 if not get_option('wheel')
     postinstall_script = files('meson_postinstall.py')
     meson.add_install_script(python, postinstall_script)
 endif
 
 summary({
+    'Host machine system': host_machine.system(),
+    'Python version': python.language_version(),
     'Debug messages (verbose)': get_option('verbose'),
     'Build for wheel': get_option('wheel'),
     'JACK support': jack_support,
     'ALSA support': alsa_support,
     'CoreMIDI support': coremidi_support,
     'Window MM support': winmm_support,
 }, section: 'Configuration')
-
```

### Comparing `python_rtmidi-1.5.3/meson_options.txt` & `python_rtmidi-1.5.4/meson_options.txt`

 * *Files identical despite different names*

### Comparing `python_rtmidi-1.5.3/pyproject.toml` & `python_rtmidi-1.5.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `python_rtmidi-1.5.3/requirements-dev.txt` & `python_rtmidi-1.5.4/requirements-dev.txt`

 * *Files identical despite different names*

### Comparing `python_rtmidi-1.5.3/rtmidi/meson.build` & `python_rtmidi-1.5.4/rtmidi/meson.build`

 * *Files identical despite different names*

### Comparing `python_rtmidi-1.5.3/rtmidi/midiconstants.py` & `python_rtmidi-1.5.4/rtmidi/midiconstants.py`

 * *Files identical despite different names*

### Comparing `python_rtmidi-1.5.3/rtmidi/midiutil.py` & `python_rtmidi-1.5.4/rtmidi/midiutil.py`

 * *Files identical despite different names*

### Comparing `python_rtmidi-1.5.3/src/_rtmidi.cpp` & `python_rtmidi-1.5.4/src/_rtmidi.cpp`

 * *Files identical despite different names*

### Comparing `python_rtmidi-1.5.3/src/_rtmidi.pyx` & `python_rtmidi-1.5.4/src/_rtmidi.pyx`

 * *Files identical despite different names*

### Comparing `python_rtmidi-1.5.3/src/meson.build` & `python_rtmidi-1.5.4/src/meson.build`

 * *Files identical despite different names*

### Comparing `python_rtmidi-1.5.3/src/meson_dist_cython.py` & `python_rtmidi-1.5.4/src/meson_dist_cython.py`

 * *Files identical despite different names*

### Comparing `python_rtmidi-1.5.3/src/rtmidi/CMakeLists.txt` & `python_rtmidi-1.5.4/src/rtmidi/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `python_rtmidi-1.5.3/src/rtmidi/LICENSE` & `python_rtmidi-1.5.4/src/rtmidi/LICENSE`

 * *Files identical despite different names*

### Comparing `python_rtmidi-1.5.3/src/rtmidi/Makefile.am` & `python_rtmidi-1.5.4/src/rtmidi/Makefile.am`

 * *Files identical despite different names*

### Comparing `python_rtmidi-1.5.3/src/rtmidi/README.md` & `python_rtmidi-1.5.4/src/rtmidi/README.md`

 * *Files identical despite different names*

### Comparing `python_rtmidi-1.5.3/src/rtmidi/RtMidi.cpp` & `python_rtmidi-1.5.4/src/rtmidi/RtMidi.cpp`

 * *Files identical despite different names*

### Comparing `python_rtmidi-1.5.3/src/rtmidi/RtMidi.h` & `python_rtmidi-1.5.4/src/rtmidi/RtMidi.h`

 * *Files identical despite different names*

### Comparing `python_rtmidi-1.5.3/src/rtmidi/autogen.sh` & `python_rtmidi-1.5.4/src/rtmidi/autogen.sh`

 * *Files identical despite different names*

### Comparing `python_rtmidi-1.5.3/src/rtmidi/cmake/RtMidiConfigUninstall.cmake.in` & `python_rtmidi-1.5.4/src/rtmidi/cmake/RtMidiConfigUninstall.cmake.in`

 * *Files identical despite different names*

### Comparing `python_rtmidi-1.5.3/src/rtmidi/configure.ac` & `python_rtmidi-1.5.4/src/rtmidi/configure.ac`

 * *Files identical despite different names*

### Comparing `python_rtmidi-1.5.3/src/rtmidi/contrib/go/rtmidi/rtmidi.go` & `python_rtmidi-1.5.4/src/rtmidi/contrib/go/rtmidi/rtmidi.go`

 * *Files identical despite different names*

### Comparing `python_rtmidi-1.5.3/src/rtmidi/contrib/go/rtmidi/rtmidi_test.go` & `python_rtmidi-1.5.4/src/rtmidi/contrib/go/rtmidi/rtmidi_test.go`

 * *Files identical despite different names*

### Comparing `python_rtmidi-1.5.3/src/rtmidi/doc/Makefile.am` & `python_rtmidi-1.5.4/src/rtmidi/doc/Makefile.am`

 * *Files identical despite different names*

### Comparing `python_rtmidi-1.5.3/src/rtmidi/doc/doxygen/Doxyfile.in` & `python_rtmidi-1.5.4/src/rtmidi/doc/doxygen/Doxyfile.in`

 * *Files identical despite different names*

### Comparing `python_rtmidi-1.5.3/src/rtmidi/doc/doxygen/tutorial.txt` & `python_rtmidi-1.5.4/src/rtmidi/doc/doxygen/tutorial.txt`

 * *Files identical despite different names*

### Comparing `python_rtmidi-1.5.3/src/rtmidi/doc/images/ccrma.gif` & `python_rtmidi-1.5.4/src/rtmidi/doc/images/ccrma.gif`

 * *Files identical despite different names*

### Comparing `python_rtmidi-1.5.3/src/rtmidi/doc/images/mcgill.gif` & `python_rtmidi-1.5.4/src/rtmidi/doc/images/mcgill.gif`

 * *Files identical despite different names*

### Comparing `python_rtmidi-1.5.3/src/rtmidi/doc/release.txt` & `python_rtmidi-1.5.4/src/rtmidi/doc/release.txt`

 * *Files identical despite different names*

### Comparing `python_rtmidi-1.5.3/src/rtmidi/m4/ax_cxx_compile_stdcxx.m4` & `python_rtmidi-1.5.4/src/rtmidi/m4/ax_cxx_compile_stdcxx.m4`

 * *Files identical despite different names*

### Comparing `python_rtmidi-1.5.3/src/rtmidi/msw/rtmidilib.sln` & `python_rtmidi-1.5.4/src/rtmidi/msw/rtmidilib.sln`

 * *Files identical despite different names*

### Comparing `python_rtmidi-1.5.3/src/rtmidi/msw/rtmidilib.vcproj` & `python_rtmidi-1.5.4/src/rtmidi/msw/rtmidilib.vcproj`

 * *Files identical despite different names*

### Comparing `python_rtmidi-1.5.3/src/rtmidi/rtmidi_c.cpp` & `python_rtmidi-1.5.4/src/rtmidi/rtmidi_c.cpp`

 * *Files identical despite different names*

### Comparing `python_rtmidi-1.5.3/src/rtmidi/rtmidi_c.h` & `python_rtmidi-1.5.4/src/rtmidi/rtmidi_c.h`

 * *Files identical despite different names*

### Comparing `python_rtmidi-1.5.3/src/rtmidi/tests/Makefile.am` & `python_rtmidi-1.5.4/src/rtmidi/tests/Makefile.am`

 * *Files identical despite different names*

### Comparing `python_rtmidi-1.5.3/src/rtmidi/tests/RtMidi.dsw` & `python_rtmidi-1.5.4/src/rtmidi/tests/RtMidi.dsw`

 * *Files identical despite different names*

### Comparing `python_rtmidi-1.5.3/src/rtmidi/tests/apinames.cpp` & `python_rtmidi-1.5.4/src/rtmidi/tests/apinames.cpp`

 * *Files identical despite different names*

### Comparing `python_rtmidi-1.5.3/src/rtmidi/tests/cmidiin.cpp` & `python_rtmidi-1.5.4/src/rtmidi/tests/cmidiin.cpp`

 * *Files identical despite different names*

### Comparing `python_rtmidi-1.5.3/src/rtmidi/tests/cmidiin.dsp` & `python_rtmidi-1.5.4/src/rtmidi/tests/cmidiin.dsp`

 * *Files identical despite different names*

### Comparing `python_rtmidi-1.5.3/src/rtmidi/tests/midiclock.cpp` & `python_rtmidi-1.5.4/src/rtmidi/tests/midiclock.cpp`

 * *Files identical despite different names*

### Comparing `python_rtmidi-1.5.3/src/rtmidi/tests/midiout.cpp` & `python_rtmidi-1.5.4/src/rtmidi/tests/midiout.cpp`

 * *Files identical despite different names*

### Comparing `python_rtmidi-1.5.3/src/rtmidi/tests/midiout.dsp` & `python_rtmidi-1.5.4/src/rtmidi/tests/midiout.dsp`

 * *Files identical despite different names*

### Comparing `python_rtmidi-1.5.3/src/rtmidi/tests/midiprobe.cpp` & `python_rtmidi-1.5.4/src/rtmidi/tests/midiprobe.cpp`

 * *Files identical despite different names*

### Comparing `python_rtmidi-1.5.3/src/rtmidi/tests/midiprobe.dsp` & `python_rtmidi-1.5.4/src/rtmidi/tests/midiprobe.dsp`

 * *Files identical despite different names*

### Comparing `python_rtmidi-1.5.3/src/rtmidi/tests/qmidiin.cpp` & `python_rtmidi-1.5.4/src/rtmidi/tests/qmidiin.cpp`

 * *Files identical despite different names*

### Comparing `python_rtmidi-1.5.3/src/rtmidi/tests/qmidiin.dsp` & `python_rtmidi-1.5.4/src/rtmidi/tests/qmidiin.dsp`

 * *Files identical despite different names*

### Comparing `python_rtmidi-1.5.3/src/rtmidi/tests/sysextest.cpp` & `python_rtmidi-1.5.4/src/rtmidi/tests/sysextest.cpp`

 * *Files identical despite different names*

### Comparing `python_rtmidi-1.5.3/src/rtmidi/tests/sysextest.dsp` & `python_rtmidi-1.5.4/src/rtmidi/tests/sysextest.dsp`

 * *Files identical despite different names*

### Comparing `python_rtmidi-1.5.3/src/rtmidi/tests/testcapi.c` & `python_rtmidi-1.5.4/src/rtmidi/tests/testcapi.c`

 * *Files identical despite different names*

### Comparing `python_rtmidi-1.5.3/tests/test_basic.py` & `python_rtmidi-1.5.4/tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `python_rtmidi-1.5.3/tests/test_ci_wheels.py` & `python_rtmidi-1.5.4/tests/test_ci_wheels.py`

 * *Files identical despite different names*

### Comparing `python_rtmidi-1.5.3/tests/test_delete.py` & `python_rtmidi-1.5.4/tests/test_delete.py`

 * *Files identical despite different names*

### Comparing `python_rtmidi-1.5.3/tests/test_errorcallback.py` & `python_rtmidi-1.5.4/tests/test_errorcallback.py`

 * *Files identical despite different names*

### Comparing `python_rtmidi-1.5.3/tests/test_errors.py` & `python_rtmidi-1.5.4/tests/test_errors.py`

 * *Files identical despite different names*

### Comparing `python_rtmidi-1.5.3/tests/test_rtmidi.py` & `python_rtmidi-1.5.4/tests/test_rtmidi.py`

 * *Files identical despite different names*

### Comparing `python_rtmidi-1.5.3/PKG-INFO` & `python_rtmidi-1.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-rtmidi
-Version: 1.5.3
+Version: 1.5.4
 Summary: A Python binding for the RtMidi C++ library implemented using Cython.
 Keywords: MIDI multimedia music rtmidi
 Author-Email: Christopher Arndt <info@chrisarndt.de>
 License: Copyright & License
         ===================
         
         python-rtmidi was written by Christopher Arndt, 2012 - 2023.
```

