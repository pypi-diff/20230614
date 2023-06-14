# Comparing `tmp/python-rtmidi-1.5.1.tar.gz` & `tmp/python-rtmidi-1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-rtmidi-1.5.1.tar", last modified: Mon Jun 12 14:09:30 2023, max compression
+gzip compressed data, was "python-rtmidi-1.5.2.tar", last modified: Wed Jun 14 06:50:52 2023, max compression
```

## Comparing `python-rtmidi-1.5.1.tar` & `python-rtmidi-1.5.2.tar`

### file list

```diff
@@ -1,177 +1,178 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:09:25.630277 python-rtmidi-1.5.1/
--rw-rw-r--   0 runner    (1001) docker     (123)       94 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/.flake8
-drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/.github/
-drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/.github/workflows/
--rw-rw-r--   0 runner    (1001) docker     (123)     2384 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/.github/workflows/development.yml
--rw-rw-r--   0 runner    (1001) docker     (123)     2276 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/.github/workflows/production.yml
--rw-rw-r--   0 runner    (1001) docker     (123)     1707 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/.github/workflows/tests.yml
--rw-rw-r--   0 runner    (1001) docker     (123)      571 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/.gitignore
--rw-rw-r--   0 runner    (1001) docker     (123)      118 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/.gitmodules
--rw-rw-r--   0 runner    (1001) docker     (123)      246 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/AUTHORS.md
--rw-rw-r--   0 runner    (1001) docker     (123)    21032 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/CHANGELOG.md
--rw-rw-r--   0 runner    (1001) docker     (123)     3849 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/INSTALL-windows.md
--rw-rw-r--   0 runner    (1001) docker     (123)     8352 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/INSTALL.md
--rw-rw-r--   0 runner    (1001) docker     (123)     2771 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/LICENSE.md
--rw-rw-r--   0 runner    (1001) docker     (123)      393 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/MANIFEST.in
--rw-rw-r--   0 runner    (1001) docker     (123)     2497 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/Makefile
--rw-rw-r--   0 runner    (1001) docker     (123)     2778 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/README.md
-drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/docs/
--rw-rw-r--   0 runner    (1001) docker     (123)     6778 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/docs/Makefile
--rw-rw-r--   0 runner    (1001) docker     (123)      759 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/docs/api.rst.inc
--rw-rw-r--   0 runner    (1001) docker     (123)       31 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/docs/authors.md
--rwxrwxr-x   0 runner    (1001) docker     (123)     8521 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/docs/conf.py
--rw-rw-r--   0 runner    (1001) docker     (123)     3257 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/docs/contributing.rst
--rw-rw-r--   0 runner    (1001) docker     (123)       33 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/docs/history.md
--rw-rw-r--   0 runner    (1001) docker     (123)      478 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/docs/index.rst
--rw-rw-r--   0 runner    (1001) docker     (123)       39 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/docs/install-windows.md
--rw-rw-r--   0 runner    (1001) docker     (123)       31 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/docs/installation.md
--rw-rw-r--   0 runner    (1001) docker     (123)       31 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/docs/license.md
--rw-rw-r--   0 runner    (1001) docker     (123)     6467 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/docs/make.bat
--rw-rw-r--   0 runner    (1001) docker     (123)       55 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/docs/modules.rst
--rw-rw-r--   0 runner    (1001) docker     (123)       30 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/docs/readme.md
--rw-rw-r--   0 runner    (1001) docker     (123)     1337 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/docs/rtmidi.rst
--rw-rw-r--   0 runner    (1001) docker     (123)     1129 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/docs/usage.rst
-drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/examples/
-drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/examples/advanced/
--rw-rw-r--   0 runner    (1001) docker     (123)     1687 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/examples/advanced/ccstore.py
--rw-rw-r--   0 runner    (1001) docker     (123)     2398 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/examples/advanced/midiclock.py
--rw-rw-r--   0 runner    (1001) docker     (123)     8741 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/examples/advanced/midioutwrapper.py
--rw-rw-r--   0 runner    (1001) docker     (123)     2585 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/examples/advanced/recvrpn.py
-drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/examples/basic/
--rw-rw-r--   0 runner    (1001) docker     (123)      545 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/examples/basic/contextmanager.py
--rwxrwxr-x   0 runner    (1001) docker     (123)     1359 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/examples/basic/midiin_callback.py
--rwxrwxr-x   0 runner    (1001) docker     (123)     1050 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/examples/basic/midiin_poll.py
--rwxrwxr-x   0 runner    (1001) docker     (123)      991 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/examples/basic/midiout.py
--rw-rw-r--   0 runner    (1001) docker     (123)     1012 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/examples/basic/noteon2osc.py
--rw-rw-r--   0 runner    (1001) docker     (123)      765 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/examples/basic/panic.py
--rwxrwxr-x   0 runner    (1001) docker     (123)     1571 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/examples/basic/probe_ports.py
-drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/examples/drumseq/
--rw-rw-r--   0 runner    (1001) docker     (123)     2195 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/examples/drumseq/README.rst
--rw-rw-r--   0 runner    (1001) docker     (123)      275 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/examples/drumseq/break-on-through.txt
--rwxrwxr-x   0 runner    (1001) docker     (123)     6485 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/examples/drumseq/drumseq.py
--rw-rw-r--   0 runner    (1001) docker     (123)      303 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/examples/drumseq/example_01.txt
--rw-rw-r--   0 runner    (1001) docker     (123)      303 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/examples/drumseq/example_02.txt
--rw-rw-r--   0 runner    (1001) docker     (123)      255 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/examples/drumseq/example_03.txt
--rw-rw-r--   0 runner    (1001) docker     (123)      206 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/examples/drumseq/example_04.txt
--rw-rw-r--   0 runner    (1001) docker     (123)      294 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/examples/drumseq/example_05.txt
--rw-rw-r--   0 runner    (1001) docker     (123)      303 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/examples/drumseq/example_06.txt
--rw-rw-r--   0 runner    (1001) docker     (123)      302 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/examples/drumseq/example_07.txt
--rw-rw-r--   0 runner    (1001) docker     (123)      302 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/examples/drumseq/example_08.txt
--rw-rw-r--   0 runner    (1001) docker     (123)      434 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/examples/drumseq/example_09.txt
--rw-rw-r--   0 runner    (1001) docker     (123)      435 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/examples/drumseq/example_10.txt
--rw-rw-r--   0 runner    (1001) docker     (123)      299 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/examples/drumseq/example_11.txt
--rw-rw-r--   0 runner    (1001) docker     (123)      347 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/examples/drumseq/example_12.txt
--rw-rw-r--   0 runner    (1001) docker     (123)      157 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/examples/drumseq/funkydrummer.txt
--rw-rw-r--   0 runner    (1001) docker     (123)      205 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/examples/drumseq/rosanna-shuffle.txt
--rw-rw-r--   0 runner    (1001) docker     (123)      477 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/examples/drumseq/template.txt
-drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/examples/midi2command/
--rw-rw-r--   0 runner    (1001) docker     (123)    45974 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/examples/midi2command/000-playback.mp3
--rw-rw-r--   0 runner    (1001) docker     (123)     2506 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/examples/midi2command/000-sheet.pdf
--rw-rw-r--   0 runner    (1001) docker     (123)     5624 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/examples/midi2command/README.rst
--rw-rw-r--   0 runner    (1001) docker     (123)      522 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/examples/midi2command/example.cfg
--rw-rw-r--   0 runner    (1001) docker     (123)     7132 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/examples/midi2command/midi2command.py
-drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/examples/midifilter/
--rw-rw-r--   0 runner    (1001) docker     (123)        0 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/examples/midifilter/__init__.py
--rw-rw-r--   0 runner    (1001) docker     (123)     3667 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/examples/midifilter/__main__.py
--rw-rw-r--   0 runner    (1001) docker     (123)     3119 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/examples/midifilter/filters.py
--rwxrwxr-x   0 runner    (1001) docker     (123)     5328 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/examples/sendsysex.py
-drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/examples/sequencer/
--rw-rw-r--   0 runner    (1001) docker     (123)     7155 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/examples/sequencer/sequencer.py
-drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/examples/sysex/
--rwxrwxr-x   0 runner    (1001) docker     (123)      745 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/examples/sysex/send_sysex.py
--rwxrwxr-x   0 runner    (1001) docker     (123)     1067 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/examples/sysex/send_sysex_file.py
-drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/examples/sysexsaver/
--rw-rw-r--   0 runner    (1001) docker     (123)        0 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/examples/sysexsaver/__init__.py
--rw-rw-r--   0 runner    (1001) docker     (123)     7022 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/examples/sysexsaver/__main__.py
--rw-rw-r--   0 runner    (1001) docker     (123)    11493 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/examples/sysexsaver/manufacturers.csv
--rw-rw-r--   0 runner    (1001) docker     (123)    12337 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/examples/sysexsaver/manufacturers.py
--rw-rw-r--   0 runner    (1001) docker     (123)    12147 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/examples/sysexsaver/models.py
--rw-rw-r--   0 runner    (1001) docker     (123)     3247 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/examples/wavetablemodstep.py
--rw-rw-r--   0 runner    (1001) docker     (123)     3018 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/meson.build
--rw-rw-r--   0 runner    (1001) docker     (123)      801 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/meson_options.txt
--rwxrwxr-x   0 runner    (1001) docker     (123)      405 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/meson_postinstall.py
--rw-rw-r--   0 runner    (1001) docker     (123)     3122 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/pyproject.toml
--rw-rw-r--   0 runner    (1001) docker     (123)       91 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/requirements-dev.in
--rw-rw-r--   0 runner    (1001) docker     (123)     2845 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/requirements-dev.txt
-drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/rtmidi/
--rw-rw-r--   0 runner    (1001) docker     (123)      165 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/rtmidi/__init__.py
--rw-rw-r--   0 runner    (1001) docker     (123)     1881 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/rtmidi/meson.build
--rw-rw-r--   0 runner    (1001) docker     (123)     7533 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/rtmidi/midiconstants.py
--rw-rw-r--   0 runner    (1001) docker     (123)     9261 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/rtmidi/midiutil.py
--rw-rw-r--   0 runner    (1001) docker     (123)       30 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/rtmidi/version.py.in
-drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:09:26.274290 python-rtmidi-1.5.1/src/
--rw-r--r--   0 runner    (1001) docker     (123)   737320 2023-06-12 14:09:26.274290 python-rtmidi-1.5.1/src/_rtmidi.cpp
--rw-rw-r--   0 runner    (1001) docker     (123)    39588 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/src/_rtmidi.pyx
--rw-rw-r--   0 runner    (1001) docker     (123)      857 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/src/meson.build
--rwxrwxr-x   0 runner    (1001) docker     (123)     1261 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/src/meson_dist_cython.py
-drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-06-06 16:06:52.000000 python-rtmidi-1.5.1/src/rtmidi/
--rw-rw-r--   0 runner    (1001) docker     (123)     9589 2023-06-06 16:06:52.000000 python-rtmidi-1.5.1/src/rtmidi/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (123)     1349 2023-06-06 16:06:52.000000 python-rtmidi-1.5.1/src/rtmidi/LICENSE
--rw-rw-r--   0 runner    (1001) docker     (123)      533 2023-06-06 16:06:52.000000 python-rtmidi-1.5.1/src/rtmidi/Makefile.am
--rw-rw-r--   0 runner    (1001) docker     (123)     2396 2023-06-06 16:06:52.000000 python-rtmidi-1.5.1/src/rtmidi/README.md
--rw-rw-r--   0 runner    (1001) docker     (123)   126832 2023-06-06 16:06:52.000000 python-rtmidi-1.5.1/src/rtmidi/RtMidi.cpp
--rw-rw-r--   0 runner    (1001) docker     (123)    27069 2023-06-06 16:06:52.000000 python-rtmidi-1.5.1/src/rtmidi/RtMidi.h
--rwxrwxr-x   0 runner    (1001) docker     (123)     2884 2023-06-06 16:06:52.000000 python-rtmidi-1.5.1/src/rtmidi/autogen.sh
-drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-06-06 16:06:52.000000 python-rtmidi-1.5.1/src/rtmidi/cmake/
--rw-rw-r--   0 runner    (1001) docker     (123)      252 2023-06-06 16:06:52.000000 python-rtmidi-1.5.1/src/rtmidi/cmake/RtMidi-config.cmake.in
--rw-rw-r--   0 runner    (1001) docker     (123)      940 2023-06-06 16:06:52.000000 python-rtmidi-1.5.1/src/rtmidi/cmake/RtMidiConfigUninstall.cmake.in
--rw-rw-r--   0 runner    (1001) docker     (123)     9307 2023-06-06 16:06:52.000000 python-rtmidi-1.5.1/src/rtmidi/configure.ac
-drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-06-06 16:06:52.000000 python-rtmidi-1.5.1/src/rtmidi/contrib/
-drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-06-06 16:06:52.000000 python-rtmidi-1.5.1/src/rtmidi/contrib/go/
-drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-06-06 16:06:52.000000 python-rtmidi-1.5.1/src/rtmidi/contrib/go/rtmidi/
--rw-rw-r--   0 runner    (1001) docker     (123)     8909 2023-06-06 16:06:52.000000 python-rtmidi-1.5.1/src/rtmidi/contrib/go/rtmidi/rtmidi.go
--rw-rw-r--   0 runner    (1001) docker     (123)       94 2023-06-06 16:06:52.000000 python-rtmidi-1.5.1/src/rtmidi/contrib/go/rtmidi/rtmidi_stub.cpp
--rw-rw-r--   0 runner    (1001) docker     (123)       31 2023-06-06 16:06:52.000000 python-rtmidi-1.5.1/src/rtmidi/contrib/go/rtmidi/rtmidi_stub.h
--rw-rw-r--   0 runner    (1001) docker     (123)      758 2023-06-06 16:06:52.000000 python-rtmidi-1.5.1/src/rtmidi/contrib/go/rtmidi/rtmidi_test.go
-drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-06-06 16:06:52.000000 python-rtmidi-1.5.1/src/rtmidi/doc/
--rw-rw-r--   0 runner    (1001) docker     (123)      682 2023-06-06 16:06:52.000000 python-rtmidi-1.5.1/src/rtmidi/doc/Makefile.am
-drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-06-06 16:06:52.000000 python-rtmidi-1.5.1/src/rtmidi/doc/doxygen/
--rw-rw-r--   0 runner    (1001) docker     (123)    81155 2023-06-06 16:06:52.000000 python-rtmidi-1.5.1/src/rtmidi/doc/doxygen/Doxyfile.in
--rw-rw-r--   0 runner    (1001) docker     (123)      254 2023-06-06 16:06:52.000000 python-rtmidi-1.5.1/src/rtmidi/doc/doxygen/footer.html
--rw-rw-r--   0 runner    (1001) docker     (123)      494 2023-06-06 16:06:52.000000 python-rtmidi-1.5.1/src/rtmidi/doc/doxygen/header.html
-drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-06-06 16:06:52.000000 python-rtmidi-1.5.1/src/rtmidi/doc/doxygen/samples/
--rw-rw-r--   0 runner    (1001) docker     (123)      173 2023-06-06 16:06:52.000000 python-rtmidi-1.5.1/src/rtmidi/doc/doxygen/samples/getting_started.cpp
--rw-rw-r--   0 runner    (1001) docker     (123)    21717 2023-06-06 16:06:52.000000 python-rtmidi-1.5.1/src/rtmidi/doc/doxygen/tutorial.txt
-drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-06-06 16:06:52.000000 python-rtmidi-1.5.1/src/rtmidi/doc/images/
--rw-rw-r--   0 runner    (1001) docker     (123)     3527 2023-06-06 16:06:52.000000 python-rtmidi-1.5.1/src/rtmidi/doc/images/ccrma.gif
--rw-rw-r--   0 runner    (1001) docker     (123)     4614 2023-06-06 16:06:52.000000 python-rtmidi-1.5.1/src/rtmidi/doc/images/mcgill.gif
--rw-rw-r--   0 runner    (1001) docker     (123)     7130 2023-06-06 16:06:52.000000 python-rtmidi-1.5.1/src/rtmidi/doc/release.txt
-drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-06-06 16:06:52.000000 python-rtmidi-1.5.1/src/rtmidi/m4/
--rw-rw-r--   0 runner    (1001) docker     (123)    19367 2023-06-06 16:06:52.000000 python-rtmidi-1.5.1/src/rtmidi/m4/ax_cxx_compile_stdcxx.m4
-drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-06-06 16:06:52.000000 python-rtmidi-1.5.1/src/rtmidi/msw/
--rw-rw-r--   0 runner    (1001) docker     (123)      171 2023-06-06 16:06:52.000000 python-rtmidi-1.5.1/src/rtmidi/msw/readme
--rwxrwxr-x   0 runner    (1001) docker     (123)      883 2023-06-06 16:06:52.000000 python-rtmidi-1.5.1/src/rtmidi/msw/rtmidilib.sln
--rwxrwxr-x   0 runner    (1001) docker     (123)     3734 2023-06-06 16:06:52.000000 python-rtmidi-1.5.1/src/rtmidi/msw/rtmidilib.vcproj
--rw-rw-r--   0 runner    (1001) docker     (123)      388 2023-06-06 16:06:52.000000 python-rtmidi-1.5.1/src/rtmidi/rtmidi-config.in
--rw-rw-r--   0 runner    (1001) docker     (123)      369 2023-06-06 16:06:52.000000 python-rtmidi-1.5.1/src/rtmidi/rtmidi.pc.in
--rw-rw-r--   0 runner    (1001) docker     (123)    10208 2023-06-06 16:06:52.000000 python-rtmidi-1.5.1/src/rtmidi/rtmidi_c.cpp
--rw-rw-r--   0 runner    (1001) docker     (123)     9525 2023-06-06 16:06:52.000000 python-rtmidi-1.5.1/src/rtmidi/rtmidi_c.h
-drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-06-06 16:06:52.000000 python-rtmidi-1.5.1/src/rtmidi/tests/
-drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-06-06 16:06:52.000000 python-rtmidi-1.5.1/src/rtmidi/tests/Debug/
--rw-rw-r--   0 runner    (1001) docker     (123)        0 2023-06-06 16:06:52.000000 python-rtmidi-1.5.1/src/rtmidi/tests/Debug/.placeholder
--rw-rw-r--   0 runner    (1001) docker     (123)     1018 2023-06-06 16:06:52.000000 python-rtmidi-1.5.1/src/rtmidi/tests/Makefile.am
-drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-06-06 16:06:52.000000 python-rtmidi-1.5.1/src/rtmidi/tests/Release/
--rw-rw-r--   0 runner    (1001) docker     (123)        0 2023-06-06 16:06:52.000000 python-rtmidi-1.5.1/src/rtmidi/tests/Release/.placeholder
--rw-rw-r--   0 runner    (1001) docker     (123)     1311 2023-06-06 16:06:52.000000 python-rtmidi-1.5.1/src/rtmidi/tests/RtMidi.dsw
--rw-rw-r--   0 runner    (1001) docker     (123)     5284 2023-06-06 16:06:52.000000 python-rtmidi-1.5.1/src/rtmidi/tests/apinames.cpp
--rw-rw-r--   0 runner    (1001) docker     (123)     2873 2023-06-06 16:06:52.000000 python-rtmidi-1.5.1/src/rtmidi/tests/cmidiin.cpp
--rw-rw-r--   0 runner    (1001) docker     (123)     4320 2023-06-06 16:06:52.000000 python-rtmidi-1.5.1/src/rtmidi/tests/cmidiin.dsp
--rw-rw-r--   0 runner    (1001) docker     (123)     5541 2023-06-06 16:06:52.000000 python-rtmidi-1.5.1/src/rtmidi/tests/midiclock.cpp
--rw-rw-r--   0 runner    (1001) docker     (123)     3147 2023-06-06 16:06:52.000000 python-rtmidi-1.5.1/src/rtmidi/tests/midiout.cpp
--rw-rw-r--   0 runner    (1001) docker     (123)     4320 2023-06-06 16:06:52.000000 python-rtmidi-1.5.1/src/rtmidi/tests/midiout.dsp
--rw-rw-r--   0 runner    (1001) docker     (123)     2138 2023-06-06 16:06:52.000000 python-rtmidi-1.5.1/src/rtmidi/tests/midiprobe.cpp
--rw-rw-r--   0 runner    (1001) docker     (123)     4356 2023-06-06 16:06:52.000000 python-rtmidi-1.5.1/src/rtmidi/tests/midiprobe.dsp
--rw-rw-r--   0 runner    (1001) docker     (123)     2361 2023-06-06 16:06:52.000000 python-rtmidi-1.5.1/src/rtmidi/tests/qmidiin.cpp
--rw-rw-r--   0 runner    (1001) docker     (123)     4320 2023-06-06 16:06:52.000000 python-rtmidi-1.5.1/src/rtmidi/tests/qmidiin.dsp
--rw-rw-r--   0 runner    (1001) docker     (123)     3926 2023-06-06 16:06:52.000000 python-rtmidi-1.5.1/src/rtmidi/tests/sysextest.cpp
--rw-rw-r--   0 runner    (1001) docker     (123)     4360 2023-06-06 16:06:52.000000 python-rtmidi-1.5.1/src/rtmidi/tests/sysextest.dsp
--rw-rw-r--   0 runner    (1001) docker     (123)      667 2023-06-06 16:06:52.000000 python-rtmidi-1.5.1/src/rtmidi/tests/testcapi.c
-drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/tests/
--rw-rw-r--   0 runner    (1001) docker     (123)     2922 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/tests/test_basic.py
--rw-rw-r--   0 runner    (1001) docker     (123)     2484 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/tests/test_delete.py
--rw-rw-r--   0 runner    (1001) docker     (123)     2100 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/tests/test_errorcallback.py
--rw-rw-r--   0 runner    (1001) docker     (123)     2299 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/tests/test_errors.py
--rw-rw-r--   0 runner    (1001) docker     (123)     9256 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/tests/test_rtmidi.py
--rw-rw-r--   0 runner    (1001) docker     (123)      298 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/tox.ini
--rwxrwxr-x   0 runner    (1001) docker     (123)      346 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/update-docs.sh
--rw-r--r--   0 runner    (1001) docker     (123)     7540 2023-06-12 14:09:30.826380 python-rtmidi-1.5.1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:47.066178 python-rtmidi-1.5.2/
+-rw-rw-r--   0 runner    (1001) docker     (123)       94 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/.flake8
+drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/.github/
+drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/.github/workflows/
+-rw-rw-r--   0 runner    (1001) docker     (123)     1393 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/.github/workflows/pr_to_master.yml
+-rw-rw-r--   0 runner    (1001) docker     (123)     2338 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/.github/workflows/push_to_master.yml
+-rw-rw-r--   0 runner    (1001) docker     (123)     2277 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/.github/workflows/release.yml
+-rw-rw-r--   0 runner    (1001) docker     (123)      571 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/.gitignore
+-rw-rw-r--   0 runner    (1001) docker     (123)      118 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/.gitmodules
+-rw-rw-r--   0 runner    (1001) docker     (123)      300 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/AUTHORS.md
+-rw-rw-r--   0 runner    (1001) docker     (123)    21704 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/CHANGELOG.md
+-rw-rw-r--   0 runner    (1001) docker     (123)     3849 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/INSTALL-windows.md
+-rw-rw-r--   0 runner    (1001) docker     (123)     8352 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/INSTALL.md
+-rw-rw-r--   0 runner    (1001) docker     (123)     2771 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/LICENSE.md
+-rw-rw-r--   0 runner    (1001) docker     (123)      393 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/MANIFEST.in
+-rw-rw-r--   0 runner    (1001) docker     (123)     2497 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/Makefile
+-rw-rw-r--   0 runner    (1001) docker     (123)     2802 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/README.md
+drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/docs/
+-rw-rw-r--   0 runner    (1001) docker     (123)     6778 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/docs/Makefile
+-rw-rw-r--   0 runner    (1001) docker     (123)      759 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/docs/api.rst.inc
+-rw-rw-r--   0 runner    (1001) docker     (123)       31 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/docs/authors.md
+-rwxrwxr-x   0 runner    (1001) docker     (123)     8521 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/docs/conf.py
+-rw-rw-r--   0 runner    (1001) docker     (123)     3257 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/docs/contributing.rst
+-rw-rw-r--   0 runner    (1001) docker     (123)       33 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/docs/history.md
+-rw-rw-r--   0 runner    (1001) docker     (123)      478 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/docs/index.rst
+-rw-rw-r--   0 runner    (1001) docker     (123)       39 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/docs/install-windows.md
+-rw-rw-r--   0 runner    (1001) docker     (123)       31 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/docs/installation.md
+-rw-rw-r--   0 runner    (1001) docker     (123)       31 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/docs/license.md
+-rw-rw-r--   0 runner    (1001) docker     (123)     6467 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/docs/make.bat
+-rw-rw-r--   0 runner    (1001) docker     (123)       55 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/docs/modules.rst
+-rw-rw-r--   0 runner    (1001) docker     (123)       30 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/docs/readme.md
+-rw-rw-r--   0 runner    (1001) docker     (123)     1337 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/docs/rtmidi.rst
+-rw-rw-r--   0 runner    (1001) docker     (123)     1129 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/docs/usage.rst
+drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/examples/
+drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/examples/advanced/
+-rw-rw-r--   0 runner    (1001) docker     (123)     1687 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/examples/advanced/ccstore.py
+-rw-rw-r--   0 runner    (1001) docker     (123)     2398 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/examples/advanced/midiclock.py
+-rw-rw-r--   0 runner    (1001) docker     (123)     8741 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/examples/advanced/midioutwrapper.py
+-rw-rw-r--   0 runner    (1001) docker     (123)     2585 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/examples/advanced/recvrpn.py
+drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/examples/basic/
+-rw-rw-r--   0 runner    (1001) docker     (123)      545 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/examples/basic/contextmanager.py
+-rwxrwxr-x   0 runner    (1001) docker     (123)     1359 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/examples/basic/midiin_callback.py
+-rwxrwxr-x   0 runner    (1001) docker     (123)     1050 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/examples/basic/midiin_poll.py
+-rwxrwxr-x   0 runner    (1001) docker     (123)      991 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/examples/basic/midiout.py
+-rw-rw-r--   0 runner    (1001) docker     (123)     1012 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/examples/basic/noteon2osc.py
+-rw-rw-r--   0 runner    (1001) docker     (123)      765 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/examples/basic/panic.py
+-rwxrwxr-x   0 runner    (1001) docker     (123)     1571 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/examples/basic/probe_ports.py
+drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/examples/drumseq/
+-rw-rw-r--   0 runner    (1001) docker     (123)     2195 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/examples/drumseq/README.rst
+-rw-rw-r--   0 runner    (1001) docker     (123)      275 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/examples/drumseq/break-on-through.txt
+-rwxrwxr-x   0 runner    (1001) docker     (123)     6485 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/examples/drumseq/drumseq.py
+-rw-rw-r--   0 runner    (1001) docker     (123)      303 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/examples/drumseq/example_01.txt
+-rw-rw-r--   0 runner    (1001) docker     (123)      303 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/examples/drumseq/example_02.txt
+-rw-rw-r--   0 runner    (1001) docker     (123)      255 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/examples/drumseq/example_03.txt
+-rw-rw-r--   0 runner    (1001) docker     (123)      206 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/examples/drumseq/example_04.txt
+-rw-rw-r--   0 runner    (1001) docker     (123)      294 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/examples/drumseq/example_05.txt
+-rw-rw-r--   0 runner    (1001) docker     (123)      303 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/examples/drumseq/example_06.txt
+-rw-rw-r--   0 runner    (1001) docker     (123)      302 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/examples/drumseq/example_07.txt
+-rw-rw-r--   0 runner    (1001) docker     (123)      302 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/examples/drumseq/example_08.txt
+-rw-rw-r--   0 runner    (1001) docker     (123)      434 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/examples/drumseq/example_09.txt
+-rw-rw-r--   0 runner    (1001) docker     (123)      435 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/examples/drumseq/example_10.txt
+-rw-rw-r--   0 runner    (1001) docker     (123)      299 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/examples/drumseq/example_11.txt
+-rw-rw-r--   0 runner    (1001) docker     (123)      347 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/examples/drumseq/example_12.txt
+-rw-rw-r--   0 runner    (1001) docker     (123)      157 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/examples/drumseq/funkydrummer.txt
+-rw-rw-r--   0 runner    (1001) docker     (123)      205 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/examples/drumseq/rosanna-shuffle.txt
+-rw-rw-r--   0 runner    (1001) docker     (123)      477 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/examples/drumseq/template.txt
+drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/examples/midi2command/
+-rw-rw-r--   0 runner    (1001) docker     (123)    45974 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/examples/midi2command/000-playback.mp3
+-rw-rw-r--   0 runner    (1001) docker     (123)     2506 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/examples/midi2command/000-sheet.pdf
+-rw-rw-r--   0 runner    (1001) docker     (123)     5624 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/examples/midi2command/README.rst
+-rw-rw-r--   0 runner    (1001) docker     (123)      522 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/examples/midi2command/example.cfg
+-rw-rw-r--   0 runner    (1001) docker     (123)     7132 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/examples/midi2command/midi2command.py
+drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/examples/midifilter/
+-rw-rw-r--   0 runner    (1001) docker     (123)        0 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/examples/midifilter/__init__.py
+-rw-rw-r--   0 runner    (1001) docker     (123)     3667 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/examples/midifilter/__main__.py
+-rw-rw-r--   0 runner    (1001) docker     (123)     3119 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/examples/midifilter/filters.py
+-rwxrwxr-x   0 runner    (1001) docker     (123)     5328 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/examples/sendsysex.py
+drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/examples/sequencer/
+-rw-rw-r--   0 runner    (1001) docker     (123)     7155 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/examples/sequencer/sequencer.py
+drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/examples/sysex/
+-rwxrwxr-x   0 runner    (1001) docker     (123)      745 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/examples/sysex/send_sysex.py
+-rwxrwxr-x   0 runner    (1001) docker     (123)     1067 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/examples/sysex/send_sysex_file.py
+drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/examples/sysexsaver/
+-rw-rw-r--   0 runner    (1001) docker     (123)        0 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/examples/sysexsaver/__init__.py
+-rw-rw-r--   0 runner    (1001) docker     (123)     7022 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/examples/sysexsaver/__main__.py
+-rw-rw-r--   0 runner    (1001) docker     (123)    11493 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/examples/sysexsaver/manufacturers.csv
+-rw-rw-r--   0 runner    (1001) docker     (123)    12337 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/examples/sysexsaver/manufacturers.py
+-rw-rw-r--   0 runner    (1001) docker     (123)    12147 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/examples/sysexsaver/models.py
+-rw-rw-r--   0 runner    (1001) docker     (123)     3247 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/examples/wavetablemodstep.py
+-rw-rw-r--   0 runner    (1001) docker     (123)     3224 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (123)      801 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/meson_options.txt
+-rwxrwxr-x   0 runner    (1001) docker     (123)      462 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/meson_postinstall.py
+-rw-rw-r--   0 runner    (1001) docker     (123)     3109 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/pyproject.toml
+-rw-rw-r--   0 runner    (1001) docker     (123)       91 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/requirements-dev.in
+-rw-rw-r--   0 runner    (1001) docker     (123)     2686 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/requirements-dev.txt
+drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/rtmidi/
+-rw-rw-r--   0 runner    (1001) docker     (123)      165 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/rtmidi/__init__.py
+-rw-rw-r--   0 runner    (1001) docker     (123)     1744 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/rtmidi/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (123)     7533 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/rtmidi/midiconstants.py
+-rw-rw-r--   0 runner    (1001) docker     (123)     9261 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/rtmidi/midiutil.py
+-rw-rw-r--   0 runner    (1001) docker     (123)       30 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/rtmidi/version.py.in
+drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:47.706187 python-rtmidi-1.5.2/src/
+-rw-r--r--   0 runner    (1001) docker     (123)   737312 2023-06-14 06:50:47.706187 python-rtmidi-1.5.2/src/_rtmidi.cpp
+-rw-rw-r--   0 runner    (1001) docker     (123)    39588 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/src/_rtmidi.pyx
+-rw-rw-r--   0 runner    (1001) docker     (123)      857 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/src/meson.build
+-rwxrwxr-x   0 runner    (1001) docker     (123)     1261 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/src/meson_dist_cython.py
+drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:56:07.000000 python-rtmidi-1.5.2/src/rtmidi/
+-rw-rw-r--   0 runner    (1001) docker     (123)     9806 2023-06-12 20:56:07.000000 python-rtmidi-1.5.2/src/rtmidi/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (123)     1349 2023-06-12 20:56:07.000000 python-rtmidi-1.5.2/src/rtmidi/LICENSE
+-rw-rw-r--   0 runner    (1001) docker     (123)      533 2023-06-12 20:56:07.000000 python-rtmidi-1.5.2/src/rtmidi/Makefile.am
+-rw-rw-r--   0 runner    (1001) docker     (123)     2396 2023-06-12 20:56:07.000000 python-rtmidi-1.5.2/src/rtmidi/README.md
+-rw-rw-r--   0 runner    (1001) docker     (123)   126845 2023-06-12 20:56:07.000000 python-rtmidi-1.5.2/src/rtmidi/RtMidi.cpp
+-rw-rw-r--   0 runner    (1001) docker     (123)    27079 2023-06-12 20:56:07.000000 python-rtmidi-1.5.2/src/rtmidi/RtMidi.h
+-rwxrwxr-x   0 runner    (1001) docker     (123)     2884 2023-06-12 20:56:07.000000 python-rtmidi-1.5.2/src/rtmidi/autogen.sh
+drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:56:07.000000 python-rtmidi-1.5.2/src/rtmidi/cmake/
+-rw-rw-r--   0 runner    (1001) docker     (123)      940 2023-06-12 20:56:07.000000 python-rtmidi-1.5.2/src/rtmidi/cmake/RtMidiConfigUninstall.cmake.in
+-rw-rw-r--   0 runner    (1001) docker     (123)      277 2023-06-12 20:56:07.000000 python-rtmidi-1.5.2/src/rtmidi/cmake/rtmidi-config.cmake.in
+-rw-rw-r--   0 runner    (1001) docker     (123)     9307 2023-06-12 20:56:07.000000 python-rtmidi-1.5.2/src/rtmidi/configure.ac
+drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:56:07.000000 python-rtmidi-1.5.2/src/rtmidi/contrib/
+drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:56:07.000000 python-rtmidi-1.5.2/src/rtmidi/contrib/go/
+drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:56:07.000000 python-rtmidi-1.5.2/src/rtmidi/contrib/go/rtmidi/
+-rw-rw-r--   0 runner    (1001) docker     (123)       59 2023-06-12 20:56:07.000000 python-rtmidi-1.5.2/src/rtmidi/contrib/go/rtmidi/go.mod
+-rw-rw-r--   0 runner    (1001) docker     (123)    10504 2023-06-12 20:56:07.000000 python-rtmidi-1.5.2/src/rtmidi/contrib/go/rtmidi/rtmidi.go
+-rw-rw-r--   0 runner    (1001) docker     (123)      125 2023-06-12 20:56:07.000000 python-rtmidi-1.5.2/src/rtmidi/contrib/go/rtmidi/rtmidi_stub.cpp
+-rw-rw-r--   0 runner    (1001) docker     (123)       31 2023-06-12 20:56:07.000000 python-rtmidi-1.5.2/src/rtmidi/contrib/go/rtmidi/rtmidi_stub.h
+-rw-rw-r--   0 runner    (1001) docker     (123)      758 2023-06-12 20:56:07.000000 python-rtmidi-1.5.2/src/rtmidi/contrib/go/rtmidi/rtmidi_test.go
+drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:56:07.000000 python-rtmidi-1.5.2/src/rtmidi/doc/
+-rw-rw-r--   0 runner    (1001) docker     (123)      682 2023-06-12 20:56:07.000000 python-rtmidi-1.5.2/src/rtmidi/doc/Makefile.am
+drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:56:07.000000 python-rtmidi-1.5.2/src/rtmidi/doc/doxygen/
+-rw-rw-r--   0 runner    (1001) docker     (123)    81155 2023-06-12 20:56:07.000000 python-rtmidi-1.5.2/src/rtmidi/doc/doxygen/Doxyfile.in
+-rw-rw-r--   0 runner    (1001) docker     (123)      254 2023-06-12 20:56:07.000000 python-rtmidi-1.5.2/src/rtmidi/doc/doxygen/footer.html
+-rw-rw-r--   0 runner    (1001) docker     (123)      494 2023-06-12 20:56:07.000000 python-rtmidi-1.5.2/src/rtmidi/doc/doxygen/header.html
+drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:56:07.000000 python-rtmidi-1.5.2/src/rtmidi/doc/doxygen/samples/
+-rw-rw-r--   0 runner    (1001) docker     (123)      173 2023-06-12 20:56:07.000000 python-rtmidi-1.5.2/src/rtmidi/doc/doxygen/samples/getting_started.cpp
+-rw-rw-r--   0 runner    (1001) docker     (123)    21717 2023-06-12 20:56:07.000000 python-rtmidi-1.5.2/src/rtmidi/doc/doxygen/tutorial.txt
+drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:56:07.000000 python-rtmidi-1.5.2/src/rtmidi/doc/images/
+-rw-rw-r--   0 runner    (1001) docker     (123)     3527 2023-06-12 20:56:07.000000 python-rtmidi-1.5.2/src/rtmidi/doc/images/ccrma.gif
+-rw-rw-r--   0 runner    (1001) docker     (123)     4614 2023-06-12 20:56:07.000000 python-rtmidi-1.5.2/src/rtmidi/doc/images/mcgill.gif
+-rw-rw-r--   0 runner    (1001) docker     (123)     7130 2023-06-12 20:56:07.000000 python-rtmidi-1.5.2/src/rtmidi/doc/release.txt
+drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:56:07.000000 python-rtmidi-1.5.2/src/rtmidi/m4/
+-rw-rw-r--   0 runner    (1001) docker     (123)    19367 2023-06-12 20:56:07.000000 python-rtmidi-1.5.2/src/rtmidi/m4/ax_cxx_compile_stdcxx.m4
+drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:56:07.000000 python-rtmidi-1.5.2/src/rtmidi/msw/
+-rw-rw-r--   0 runner    (1001) docker     (123)      171 2023-06-12 20:56:07.000000 python-rtmidi-1.5.2/src/rtmidi/msw/readme
+-rwxrwxr-x   0 runner    (1001) docker     (123)      883 2023-06-12 20:56:07.000000 python-rtmidi-1.5.2/src/rtmidi/msw/rtmidilib.sln
+-rwxrwxr-x   0 runner    (1001) docker     (123)     3734 2023-06-12 20:56:07.000000 python-rtmidi-1.5.2/src/rtmidi/msw/rtmidilib.vcproj
+-rw-rw-r--   0 runner    (1001) docker     (123)      388 2023-06-12 20:56:07.000000 python-rtmidi-1.5.2/src/rtmidi/rtmidi-config.in
+-rw-rw-r--   0 runner    (1001) docker     (123)      369 2023-06-12 20:56:07.000000 python-rtmidi-1.5.2/src/rtmidi/rtmidi.pc.in
+-rw-rw-r--   0 runner    (1001) docker     (123)    10218 2023-06-12 20:56:07.000000 python-rtmidi-1.5.2/src/rtmidi/rtmidi_c.cpp
+-rw-rw-r--   0 runner    (1001) docker     (123)     9532 2023-06-12 20:56:07.000000 python-rtmidi-1.5.2/src/rtmidi/rtmidi_c.h
+drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:56:07.000000 python-rtmidi-1.5.2/src/rtmidi/tests/
+drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:56:07.000000 python-rtmidi-1.5.2/src/rtmidi/tests/Debug/
+-rw-rw-r--   0 runner    (1001) docker     (123)        0 2023-06-12 20:56:07.000000 python-rtmidi-1.5.2/src/rtmidi/tests/Debug/.placeholder
+-rw-rw-r--   0 runner    (1001) docker     (123)     1018 2023-06-12 20:56:07.000000 python-rtmidi-1.5.2/src/rtmidi/tests/Makefile.am
+drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:56:07.000000 python-rtmidi-1.5.2/src/rtmidi/tests/Release/
+-rw-rw-r--   0 runner    (1001) docker     (123)        0 2023-06-12 20:56:07.000000 python-rtmidi-1.5.2/src/rtmidi/tests/Release/.placeholder
+-rw-rw-r--   0 runner    (1001) docker     (123)     1311 2023-06-12 20:56:07.000000 python-rtmidi-1.5.2/src/rtmidi/tests/RtMidi.dsw
+-rw-rw-r--   0 runner    (1001) docker     (123)     5284 2023-06-12 20:56:07.000000 python-rtmidi-1.5.2/src/rtmidi/tests/apinames.cpp
+-rw-rw-r--   0 runner    (1001) docker     (123)     2873 2023-06-12 20:56:07.000000 python-rtmidi-1.5.2/src/rtmidi/tests/cmidiin.cpp
+-rw-rw-r--   0 runner    (1001) docker     (123)     4320 2023-06-12 20:56:07.000000 python-rtmidi-1.5.2/src/rtmidi/tests/cmidiin.dsp
+-rw-rw-r--   0 runner    (1001) docker     (123)     5541 2023-06-12 20:56:07.000000 python-rtmidi-1.5.2/src/rtmidi/tests/midiclock.cpp
+-rw-rw-r--   0 runner    (1001) docker     (123)     3147 2023-06-12 20:56:07.000000 python-rtmidi-1.5.2/src/rtmidi/tests/midiout.cpp
+-rw-rw-r--   0 runner    (1001) docker     (123)     4320 2023-06-12 20:56:07.000000 python-rtmidi-1.5.2/src/rtmidi/tests/midiout.dsp
+-rw-rw-r--   0 runner    (1001) docker     (123)     2138 2023-06-12 20:56:07.000000 python-rtmidi-1.5.2/src/rtmidi/tests/midiprobe.cpp
+-rw-rw-r--   0 runner    (1001) docker     (123)     4356 2023-06-12 20:56:07.000000 python-rtmidi-1.5.2/src/rtmidi/tests/midiprobe.dsp
+-rw-rw-r--   0 runner    (1001) docker     (123)     2361 2023-06-12 20:56:07.000000 python-rtmidi-1.5.2/src/rtmidi/tests/qmidiin.cpp
+-rw-rw-r--   0 runner    (1001) docker     (123)     4320 2023-06-12 20:56:07.000000 python-rtmidi-1.5.2/src/rtmidi/tests/qmidiin.dsp
+-rw-rw-r--   0 runner    (1001) docker     (123)     3926 2023-06-12 20:56:07.000000 python-rtmidi-1.5.2/src/rtmidi/tests/sysextest.cpp
+-rw-rw-r--   0 runner    (1001) docker     (123)     4360 2023-06-12 20:56:07.000000 python-rtmidi-1.5.2/src/rtmidi/tests/sysextest.dsp
+-rw-rw-r--   0 runner    (1001) docker     (123)      667 2023-06-12 20:56:07.000000 python-rtmidi-1.5.2/src/rtmidi/tests/testcapi.c
+drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/tests/
+-rw-rw-r--   0 runner    (1001) docker     (123)     2922 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/tests/test_basic.py
+-rw-rw-r--   0 runner    (1001) docker     (123)     2484 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/tests/test_delete.py
+-rw-rw-r--   0 runner    (1001) docker     (123)     2100 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/tests/test_errorcallback.py
+-rw-rw-r--   0 runner    (1001) docker     (123)     2299 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/tests/test_errors.py
+-rw-rw-r--   0 runner    (1001) docker     (123)     9256 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/tests/test_rtmidi.py
+-rw-rw-r--   0 runner    (1001) docker     (123)      298 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/tox.ini
+-rwxrwxr-x   0 runner    (1001) docker     (123)      346 2023-06-14 06:47:56.000000 python-rtmidi-1.5.2/update-docs.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     7564 2023-06-14 06:50:52.266248 python-rtmidi-1.5.2/PKG-INFO
```

### Comparing `python-rtmidi-1.5.1/.github/workflows/development.yml` & `python-rtmidi-1.5.2/.github/workflows/release.yml`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,17 @@
-name: Build sdist and wheel and publish to TestPyPI
+name: Build sdist and wheels and publish to PyPI
 
 on:
-  push:
-    branches:
-      - develop
-  pull_request:
-    branches:
-      - develop
+  release:
+    types:
+      - published
+  workflow_dispatch:
+
+permissions:
+  id-token: write # This is required for requesting the JWT
 
 jobs:
   build_sdist:
    name: Build sdist
    runs-on: ubuntu-latest
    steps:
 
@@ -34,15 +35,14 @@
      with:
        path: dist/*.tar.gz
 
   build_wheels:
     name: Build wheels on ${{ matrix.os }}
     runs-on: ${{ matrix.os }}
     strategy:
-      fail-fast: true
       matrix:
         os: [ubuntu-latest, windows-latest, macos-latest]
     steps:
 
     - uses: actions/checkout@v3
       with:
         submodules: true
@@ -86,25 +86,21 @@
      with:
        path: wheelhouse/*.whl
 
   upload_pypi:
    needs: [build_arch_wheels, build_wheels, build_sdist]
    runs-on: ubuntu-latest
    environment: PyPI release
-   if: github.ref == 'refs/heads/develop'
    steps:
    - uses: actions/download-artifact@v3
      with:
        # unpacks default artifact into dist/
        # if `name: artifact` is omitted, the action will create extra parent dir
        name: artifact
        path: dist
 
-   - name: Publish distribution to Test PyPI
+   - name: Publish distribution to PyPI
      uses: pypa/gh-action-pypi-publish@v1.8.6
      with:
-       skip_existing: true
        user: __token__
-       password: ${{ secrets.TEST_PYPI_API_TOKEN }}
-       repository_url: https://test.pypi.org/legacy/
+       password: ${{ secrets.PYPI_API_TOKEN }}
        verify-metadata: false
-
```

### Comparing `python-rtmidi-1.5.1/.github/workflows/production.yml` & `python-rtmidi-1.5.2/.github/workflows/push_to_master.yml`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,13 @@
-name: Build sdist and wheel and publish to PyPI
+name: Build sdist and wheels and publish to TestPyPI
 
 on:
-  release:
-    types:
-      - published
-  workflow_dispatch:
-
-permissions:
-  id-token: write # This is required for requesting the JWT
+  push:
+    branches:
+      - master
 
 jobs:
   build_sdist:
    name: Build sdist
    runs-on: ubuntu-latest
    steps:
 
@@ -35,14 +31,15 @@
      with:
        path: dist/*.tar.gz
 
   build_wheels:
     name: Build wheels on ${{ matrix.os }}
     runs-on: ${{ matrix.os }}
     strategy:
+      fail-fast: true
       matrix:
         os: [ubuntu-latest, windows-latest, macos-latest]
     steps:
 
     - uses: actions/checkout@v3
       with:
         submodules: true
@@ -86,21 +83,25 @@
      with:
        path: wheelhouse/*.whl
 
   upload_pypi:
    needs: [build_arch_wheels, build_wheels, build_sdist]
    runs-on: ubuntu-latest
    environment: PyPI release
+   if: github.ref == 'refs/heads/develop'
    steps:
    - uses: actions/download-artifact@v3
      with:
        # unpacks default artifact into dist/
        # if `name: artifact` is omitted, the action will create extra parent dir
        name: artifact
        path: dist
 
-   - name: Publish distribution to PyPI
+   - name: Publish distribution to Test PyPI
      uses: pypa/gh-action-pypi-publish@v1.8.6
      with:
+       skip_existing: true
        user: __token__
-       password: ${{ secrets.PYPI_API_TOKEN }}
+       password: ${{ secrets.TEST_PYPI_API_TOKEN }}
+       repository_url: https://test.pypi.org/legacy/
        verify-metadata: false
+
```

### Comparing `python-rtmidi-1.5.1/.github/workflows/tests.yml` & `python-rtmidi-1.5.2/.github/workflows/pr_to_master.yml`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,13 @@
-name: Build sdist and wheel for testing purposes
+name: Build sdist and wheels for testing purposes
 
 on:
-  push:
-    branches:
-      - improve-build
   pull_request:
     branches:
-      - improve-build
+      - master
 
 jobs:
   build_sdist:
    name: Build sdist
    runs-on: ubuntu-latest
    steps:
 
@@ -26,18 +23,14 @@
 
    - name: Build sdist
      run: pipx run build --sdist
 
    - name: Check metadata
      run: pipx run twine check --strict dist/*
 
-   - uses: actions/upload-artifact@v3
-     with:
-       path: dist/*.tar.gz
-
   build_wheels:
     name: Build wheels on ${{ matrix.os }}
     runs-on: ${{ matrix.os }}
     strategy:
       fail-fast: true
       matrix:
         os: [ubuntu-latest, windows-latest, macos-latest]
@@ -49,18 +42,14 @@
 
     - uses: ilammy/msvc-dev-cmd@v1
       if: matrix.os == 'windows-latest'
 
     - name: Build wheels
       uses: pypa/cibuildwheel@v2.12.3
 
-    - uses: actions/upload-artifact@v3
-      with:
-        path: wheelhouse/*.whl
-
   build_arch_wheels:
    name: Build wheels on Linux ${{ matrix.arch }}
    runs-on: ubuntu-20.04
    strategy:
      matrix:
        arch: [aarch64]
    steps:
@@ -77,11 +66,7 @@
      env:
        CIBW_ARCHS: ${{ matrix.arch }}
 
    - name: Verify clean directory
      run: git diff --exit-code
      shell: bash
 
-   - name: Upload wheels
-     uses: actions/upload-artifact@v3
-     with:
-       path: wheelhouse/*.whl
```

### Comparing `python-rtmidi-1.5.1/.gitignore` & `python-rtmidi-1.5.2/.gitignore`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.1/CHANGELOG.md` & `python-rtmidi-1.5.2/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,54 @@
 # Changelog
 
 For details and minor changes, please see the [version control log
 messages](https://github.com/SpotlightKid/python-rtmidi/commits/master).
 
 
+## 1.5.1 (2023-06-12)
+
+Project infrastructure:
+
+-   Fixed broken windows binary wheels built by CI.
+
+
+## 1.5.0 (2023-05-23)
+
+Fixes:
+
+-   Fixed memleak in `midiutils.list_{in,out}put_ports` function (#103).
+-   Fixed compilation with PyPy3.
+
+Documentation:
+
+-   Clarified return types in docstrings.
+-   Converted readme, changelog, authors, and install docs to Markdown.
+
+Examples:
+
+-   Fixed `basic/panic.py` to actually use channel number loop var.
+
+Project infrastructure:
+
+-   Modernized project structure and build system (now used `meson` and `mesonpep517`) (#119).
+-   Added working cibuildwheel github action (#121).
+-   Removed redundant Github action (#140).
+
+
 ## 1.4.9 (2021-04-26)
 
 Fixes:
 
 -   Fixed Windows build for 64-bit Python 3.9 on AppVeyor CI.
 
 Changes:
 
 -   The SysEx reception buffer size for the Windows MM backend was
     changed from 8096 to 8196.
--   Synced with upstream [RtMidi](https://github.com/thestk/rtmidi)
+s-   Synced with upstream [RtMidi](https://github.com/thestk/rtmidi)
     (3dc525baf3cac345cdd3511316571c20b47f30b5, fixes #89).
 
 
 ## 1.4.8 (2021-04-26)
 
 Fixes:
```

### Comparing `python-rtmidi-1.5.1/INSTALL-windows.md` & `python-rtmidi-1.5.2/INSTALL-windows.md`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.1/INSTALL.md` & `python-rtmidi-1.5.2/INSTALL.md`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.1/LICENSE.md` & `python-rtmidi-1.5.2/LICENSE.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Copyright & License
 ===================
 
-python-rtmidi was written by Christopher Arndt, 2012 - 2021.
+python-rtmidi was written by Christopher Arndt, 2012 - 2023.
 
 The software is released unter the MIT License:
 
-Copyright (c) 2012 - 2022 Christopher Arndt
+Copyright (c) 2012 - 2023 Christopher Arndt
 
     Permission is hereby granted, free of charge, to any person obtaining a
     copy of this software and associated documentation files (the "Software"),
     to deal in the Software without restriction, including without limitation
     the rights to use, copy, modify, merge, publish, distribute, sublicense,
     and/or sell copies of the Software, and to permit persons to whom the
     Software is furnished to do so, subject to the following conditions:
```

### Comparing `python-rtmidi-1.5.1/Makefile` & `python-rtmidi-1.5.2/Makefile`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.1/README.md` & `python-rtmidi-1.5.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 A Python binding for the RtMidi C++ library implemented using Cython.
 
 [![Latest version](https://shields.io/pypi/v/python-rtmidi)](https://pypi.org/project/python-rtmidi)
 ![Project status](https://shields.io/pypi/status/python-rtmidi)
 [![MIT License](https://shields.io/pypi/l/python-rtmidi)](LICENSE.md)
 ![Python versions](https://shields.io/pypi/pyversions/python-rtmidi)
 [![Distribution format](https://shields.io/pypi/format/python-rtmidi)](https://pypi.org/project/python-rtmidi/#files)
-[![Travis CI status](https://travis-ci.org/SpotlightKid/python-rtmidi.svg?branch=master)](https://travis-ci.org/SpotlightKid/python-rtmidi)
+[![CI status](https://github.com/SpotlightKid/python-rtmidi/actions/workflows/push_to_master.yml/badge.svg)](https://github.com/SpotlightKid/python-rtmidi/actions)
 
 # Overview
 
 [RtMidi] is a set of C++ classes which provides a concise and simple,
 cross-platform API (Application Programming Interface) for realtime MIDI
 input / output across Linux (ALSA & JACK), macOS / OS X (CoreMIDI & JACK), and
 Windows (MultiMedia System) operating systems.
```

### Comparing `python-rtmidi-1.5.1/docs/Makefile` & `python-rtmidi-1.5.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.1/docs/api.rst.inc` & `python-rtmidi-1.5.2/docs/api.rst.inc`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.1/docs/conf.py` & `python-rtmidi-1.5.2/docs/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -56,15 +56,15 @@
 
 # The master toctree document.
 master_doc = 'index'
 
 # General information about the project.
 project = 'python-rtmidi'
 author = 'Christopher Arndt'
-copyright = f'2012 - 2022, {author}'
+copyright = f'2012 - 2023, {author}'
 
 # The version info for the project you're documenting, acts as replacement
 # for |version| and |release|, also used in various other places throughout
 # the built documents.
 #
 # The short X.Y version.
 version = meta['version']
```

### Comparing `python-rtmidi-1.5.1/docs/contributing.rst` & `python-rtmidi-1.5.2/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.1/docs/make.bat` & `python-rtmidi-1.5.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.1/docs/rtmidi.rst` & `python-rtmidi-1.5.2/docs/rtmidi.rst`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.1/docs/usage.rst` & `python-rtmidi-1.5.2/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.1/examples/advanced/ccstore.py` & `python-rtmidi-1.5.2/examples/advanced/ccstore.py`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.1/examples/advanced/midiclock.py` & `python-rtmidi-1.5.2/examples/advanced/midiclock.py`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.1/examples/advanced/midioutwrapper.py` & `python-rtmidi-1.5.2/examples/advanced/midioutwrapper.py`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.1/examples/advanced/recvrpn.py` & `python-rtmidi-1.5.2/examples/advanced/recvrpn.py`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.1/examples/basic/contextmanager.py` & `python-rtmidi-1.5.2/examples/basic/contextmanager.py`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.1/examples/basic/midiin_callback.py` & `python-rtmidi-1.5.2/examples/basic/midiin_callback.py`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.1/examples/basic/midiin_poll.py` & `python-rtmidi-1.5.2/examples/basic/midiin_poll.py`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.1/examples/basic/midiout.py` & `python-rtmidi-1.5.2/examples/basic/midiout.py`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.1/examples/basic/noteon2osc.py` & `python-rtmidi-1.5.2/examples/basic/noteon2osc.py`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.1/examples/basic/panic.py` & `python-rtmidi-1.5.2/examples/basic/panic.py`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.1/examples/basic/probe_ports.py` & `python-rtmidi-1.5.2/examples/basic/probe_ports.py`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.1/examples/drumseq/README.rst` & `python-rtmidi-1.5.2/examples/drumseq/README.rst`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.1/examples/drumseq/drumseq.py` & `python-rtmidi-1.5.2/examples/drumseq/drumseq.py`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.1/examples/midi2command/000-playback.mp3` & `python-rtmidi-1.5.2/examples/midi2command/000-playback.mp3`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.1/examples/midi2command/000-sheet.pdf` & `python-rtmidi-1.5.2/examples/midi2command/000-sheet.pdf`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.1/examples/midi2command/README.rst` & `python-rtmidi-1.5.2/examples/midi2command/README.rst`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.1/examples/midi2command/example.cfg` & `python-rtmidi-1.5.2/examples/midi2command/example.cfg`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.1/examples/midi2command/midi2command.py` & `python-rtmidi-1.5.2/examples/midi2command/midi2command.py`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.1/examples/midifilter/__main__.py` & `python-rtmidi-1.5.2/examples/midifilter/__main__.py`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.1/examples/midifilter/filters.py` & `python-rtmidi-1.5.2/examples/midifilter/filters.py`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.1/examples/sendsysex.py` & `python-rtmidi-1.5.2/examples/sendsysex.py`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.1/examples/sequencer/sequencer.py` & `python-rtmidi-1.5.2/examples/sequencer/sequencer.py`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.1/examples/sysex/send_sysex.py` & `python-rtmidi-1.5.2/examples/sysex/send_sysex.py`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.1/examples/sysex/send_sysex_file.py` & `python-rtmidi-1.5.2/examples/sysex/send_sysex_file.py`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.1/examples/sysexsaver/__main__.py` & `python-rtmidi-1.5.2/examples/sysexsaver/__main__.py`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.1/examples/sysexsaver/manufacturers.csv` & `python-rtmidi-1.5.2/examples/sysexsaver/manufacturers.csv`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.1/examples/sysexsaver/manufacturers.py` & `python-rtmidi-1.5.2/examples/sysexsaver/manufacturers.py`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.1/examples/sysexsaver/models.py` & `python-rtmidi-1.5.2/examples/sysexsaver/models.py`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.1/examples/wavetablemodstep.py` & `python-rtmidi-1.5.2/examples/wavetablemodstep.py`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.1/meson.build` & `python-rtmidi-1.5.2/meson.build`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 project(
     'python-rtmidi',
     'cpp',
-    version: '1.5.1',
+    version: '1.5.2',
     license: 'MIT',
     default_options: [
         'warning_level=2'
     ],
     meson_version: '>=0.63.0'
 )
 
@@ -20,15 +20,14 @@
 elif jack2_dep.found()
     jack_dep = jack2_dep
 else
     warning('No version of JACK found, which is recent enough (jack2>=1.9.11 or jack1>=0.125.0)')
     jack_dep = disabler()
 endif
 
-
 jack_not_found = jack_dep.found() ? false : true
 
 ## From https://github.com/numpy/numpy/blob/main/numpy/meson.build
 # Platform dependent config
 if host_machine.system() == 'windows'
     # WINDOWS
     if cpp.get_id() == 'gcc'
@@ -61,17 +60,24 @@
         required: jack_not_found
     )
 else
     # LINUX
 
     # API
     alsa_dep = dependency('alsa', required: jack_not_found)
-    threads_dep = dependency('threads')
 endif # Platform detection
 
+jack_support = jack_dep.found() and get_option('jack')
+alsa_support = host_machine.system() == 'linux' and alsa_dep.found() and get_option('alsa')
+coremidi_support = host_machine.system() == 'darwin' and coremidi_dep.found() and get_option('coremidi')
+winmm_support = host_machine.system() == 'windows' and winmm_dep.found() and get_option('winmm')
+
+threads_dep = dependency('threads', required: alsa_support or jack_support)
+have_semaphore = cpp.has_header('semaphore.h')
+
 pymod = import('python')
 python = pymod.find_installation(get_option('python'), required: true)
 
 # Generate _rtmidi extension source
 subdir('src')
 
 # Build & install C++ extension module and Python package
@@ -81,13 +87,13 @@
     postinstall_script = files('meson_postinstall.py')
     meson.add_install_script(python, postinstall_script)
 endif
 
 summary({
     'Debug messages (verbose)': get_option('verbose'),
     'Build for wheel': get_option('wheel'),
-    'JACK support': jack_dep.found() and get_option('jack'),
-    'ALSA support': host_machine.system() == 'linux' and alsa_dep.found() and get_option('alsa'),
-    'CoreMIDI support': host_machine.system() == 'darwin' and coremidi_dep.found() and get_option('coremidi'),
-    'Window MM support': host_machine.system() == 'windows' and winmm_dep.found() and get_option('winmm'),
+    'JACK support': jack_support,
+    'ALSA support': alsa_support,
+    'CoreMIDI support': coremidi_support,
+    'Window MM support': winmm_support,
 }, section: 'Configuration')
```

### Comparing `python-rtmidi-1.5.1/meson_options.txt` & `python-rtmidi-1.5.2/meson_options.txt`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.1/pyproject.toml` & `python-rtmidi-1.5.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     "multimedia",
     "music",
     "rtmidi",
 ]
 meson-python-option-name = "python"
 meson-options = [
     "-Dwheel=true",
-    "-Dverbose=true",
+    "-Dverbose=false",
     "--buildtype=plain"
 ]
 
 [project.license]
 file = "LICENSE.md"
 
 [project.urls]
@@ -102,17 +102,17 @@
     "python3 waf configure --prefix=/usr --autostart=none --classic",
     "python3 waf build",
     "python3 waf install",
 ]
 
 [tool.cibuildwheel.macos]
 build = "cp3{8,9,10,11}-macosx*"
-archs = ["universal2"]
+archs = ["x86_64", "arm64"]
 environment = { MACOSX_DEPLOYMENT_TARGET = "10.14" }
 before-all = [
     "pipx install ninja",
 ]
 
 [tool.cibuildwheel.windows]
 build = "cp3{8,9,10,11}-win*"
 archs = ["AMD64"]
-build-verbosity = 1
+
```

### Comparing `python-rtmidi-1.5.1/requirements-dev.txt` & `python-rtmidi-1.5.2/requirements-dev.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,150 +1,138 @@
 #
-# This file is autogenerated by pip-compile with Python 3.10
+# This file is autogenerated by pip-compile with Python 3.11
 # by the following command:
 #
 #    pip-compile --no-emit-index-url --resolver=backtracking requirements-dev.in
 #
-alabaster==0.7.12
+alabaster==0.7.13
     # via sphinx
-attrs==22.1.0
-    # via pytest
-babel==2.11.0
+babel==2.12.1
     # via sphinx
-build==0.9.0
+build==0.10.0
     # via pip-tools
-cachetools==5.2.0
+cachetools==5.3.1
     # via tox
-certifi==2022.12.7
+certifi==2023.5.7
     # via requests
 chardet==5.1.0
     # via tox
-charset-normalizer==2.1.1
+charset-normalizer==3.1.0
     # via requests
 click==8.1.3
     # via pip-tools
 colorama==0.4.6
     # via tox
-coverage==6.5.0
+coverage==7.2.7
     # via -r requirements-dev.in
-cython==0.29.32
+cython==0.29.35
     # via -r requirements-dev.in
 distlib==0.3.6
     # via virtualenv
-docutils==0.17.1
+docutils==0.18.1
     # via
     #   myst-parser
     #   sphinx
     #   sphinx-rtd-theme
-exceptiongroup==1.0.4
-    # via pytest
-filelock==3.8.2
+filelock==3.12.1
     # via
     #   tox
     #   virtualenv
 flake8==6.0.0
     # via -r requirements-dev.in
 idna==3.4
     # via requests
 imagesize==1.4.1
     # via sphinx
-iniconfig==1.1.1
+iniconfig==2.0.0
     # via pytest
 jinja2==3.1.2
     # via
     #   myst-parser
     #   sphinx
-markdown-it-py==2.1.0
+markdown-it-py==2.2.0
     # via
     #   mdit-py-plugins
     #   myst-parser
-markupsafe==2.1.1
+markupsafe==2.1.3
     # via jinja2
 mccabe==0.7.0
     # via flake8
-mdit-py-plugins==0.3.3
+mdit-py-plugins==0.3.5
     # via myst-parser
 mdurl==0.1.2
     # via markdown-it-py
-myst-parser==0.18.1
+myst-parser==1.0.0
     # via -r requirements-dev.in
-packaging==22.0
+packaging==23.1
     # via
     #   build
     #   pyproject-api
     #   pytest
     #   sphinx
     #   tox
-pep517==0.13.0
-    # via build
-pip-tools==6.12.0
+pip-tools==6.13.0
     # via -r requirements-dev.in
-platformdirs==2.6.0
+platformdirs==3.5.3
     # via
     #   tox
     #   virtualenv
 pluggy==1.0.0
     # via
     #   pytest
     #   tox
 pycodestyle==2.10.0
     # via flake8
-pydocstyle==6.1.1
+pydocstyle==6.3.0
     # via -r requirements-dev.in
 pyflakes==3.0.1
     # via flake8
-pygments==2.13.0
+pygments==2.15.1
     # via sphinx
-pyproject-api==1.2.1
+pyproject-api==1.5.1
     # via tox
-pytest==7.2.0
+pyproject-hooks==1.0.0
+    # via build
+pytest==7.3.2
     # via -r requirements-dev.in
-pytz==2022.6
-    # via babel
 pyyaml==6.0
     # via myst-parser
-requests==2.28.1
+requests==2.31.0
     # via sphinx
 snowballstemmer==2.2.0
     # via
     #   pydocstyle
     #   sphinx
-sphinx==5.3.0
+sphinx==6.2.1
     # via
     #   -r requirements-dev.in
     #   myst-parser
     #   sphinx-rtd-theme
-sphinx-rtd-theme==1.1.1
+    #   sphinxcontrib-jquery
+sphinx-rtd-theme==1.2.2
     # via -r requirements-dev.in
-sphinxcontrib-applehelp==1.0.2
+sphinxcontrib-applehelp==1.0.4
     # via sphinx
 sphinxcontrib-devhelp==1.0.2
     # via sphinx
-sphinxcontrib-htmlhelp==2.0.0
+sphinxcontrib-htmlhelp==2.0.1
     # via sphinx
+sphinxcontrib-jquery==4.1
+    # via sphinx-rtd-theme
 sphinxcontrib-jsmath==1.0.1
     # via sphinx
 sphinxcontrib-qthelp==1.0.3
     # via sphinx
 sphinxcontrib-serializinghtml==1.1.5
     # via sphinx
-tomli==2.0.1
-    # via
-    #   build
-    #   pep517
-    #   pyproject-api
-    #   pytest
-    #   tox
-tox==4.0.9
+tox==4.6.0
     # via -r requirements-dev.in
-typing-extensions==4.4.0
-    # via myst-parser
-urllib3==1.26.13
+urllib3==2.0.3
     # via requests
-virtualenv==20.17.1
+virtualenv==20.23.0
     # via tox
-wheel==0.38.4
+wheel==0.40.0
     # via pip-tools
 
 # The following packages are considered to be unsafe in a requirements file:
 # pip
 # setuptools
```

### Comparing `python-rtmidi-1.5.1/rtmidi/meson.build` & `python-rtmidi-1.5.2/rtmidi/meson.build`

 * *Files 13% similar despite different names*

```diff
@@ -1,43 +1,46 @@
 # https://mesonbuild.com/Python-module.html
 
 defines = []
 dependencies = [python.dependency()]
 link_args = []
 
-if host_machine.system() == 'darwin' and coremidi_dep.found() and get_option('coremidi')
+if coremidi_support
     defines += ['-D__MACOSX_CORE__']
     #defines += ['-frtti']
     dependencies += [coremidi_dep]
     link_args += [
         '-framework', 'CoreAudio',
         '-framework', 'CoreMIDI',
         '-framework', 'CoreFoundation'
     ]
 endif
 
-if host_machine.system() == 'linux'
+if alsa_support or jack_support
     dependencies += [threads_dep]
 endif
 
-if host_machine.system() == 'linux' and alsa_dep.found() and get_option('alsa')
+if alsa_support
     defines += ['-D__LINUX_ALSA__']
     dependencies += [alsa_dep]
 endif
 
-if host_machine.system() == 'windows' and get_option('winmm')
+if winmm_support
     defines += ['-D__WINDOWS_MM__']
     if meson.get_compiler('cpp').get_id() != 'gcc'
         defines += ['/EHsc']
     endif
     dependencies += [winmm_dep]
 endif
 
-if jack_dep.found() and get_option('jack')
+if jack_support
     defines += ['-D__UNIX_JACK__', '-DJACK_HAS_PORT_RENAME']
+    if have_semaphore
+        defines += ['-DHAVE_SEMAPHORE']
+    endif
     dependencies += [jack_dep]
 endif
 
 if get_option('verbose')
     defines += ['-D__RTMIDI_DEBUG__']
 else
     defines += ['-D__RTMIDI_SILENCE_WARNINGS__']
```

### Comparing `python-rtmidi-1.5.1/rtmidi/midiconstants.py` & `python-rtmidi-1.5.2/rtmidi/midiconstants.py`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.1/rtmidi/midiutil.py` & `python-rtmidi-1.5.2/rtmidi/midiutil.py`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.1/src/_rtmidi.cpp` & `python-rtmidi-1.5.2/src/_rtmidi.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -12038,55 +12038,55 @@
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "_rtmidi.pyx":248
  * API_MACOSX_CORE = MACOSX_CORE
  * API_LINUX_ALSA = LINUX_ALSA
  * API_UNIX_JACK = UNIX_JACK             # <<<<<<<<<<<<<<
  * API_WINDOWS_MM = WINDOWS_MM
- * API_RTMIDI_DUMMY = RTMIDI_DUMMY
+ * API_WEB_MIDI = WEB_MIDI
  */
   __pyx_t_1 = __Pyx_PyInt_From_enum__RtMidi_3a__3a_Api(RtMidi::UNIX_JACK); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 248, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_API_UNIX_JACK, __pyx_t_1) < 0) __PYX_ERR(0, 248, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "_rtmidi.pyx":249
  * API_LINUX_ALSA = LINUX_ALSA
  * API_UNIX_JACK = UNIX_JACK
  * API_WINDOWS_MM = WINDOWS_MM             # <<<<<<<<<<<<<<
- * API_RTMIDI_DUMMY = RTMIDI_DUMMY
  * API_WEB_MIDI = WEB_MIDI
+ * API_RTMIDI_DUMMY = RTMIDI_DUMMY
  */
   __pyx_t_1 = __Pyx_PyInt_From_enum__RtMidi_3a__3a_Api(RtMidi::WINDOWS_MM); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 249, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_API_WINDOWS_MM, __pyx_t_1) < 0) __PYX_ERR(0, 249, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "_rtmidi.pyx":250
  * API_UNIX_JACK = UNIX_JACK
  * API_WINDOWS_MM = WINDOWS_MM
- * API_RTMIDI_DUMMY = RTMIDI_DUMMY             # <<<<<<<<<<<<<<
- * API_WEB_MIDI = WEB_MIDI
+ * API_WEB_MIDI = WEB_MIDI             # <<<<<<<<<<<<<<
+ * API_RTMIDI_DUMMY = RTMIDI_DUMMY
  * 
  */
-  __pyx_t_1 = __Pyx_PyInt_From_enum__RtMidi_3a__3a_Api(RtMidi::RTMIDI_DUMMY); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 250, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_enum__RtMidi_3a__3a_Api(RtMidi::WEB_MIDI_API); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 250, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_API_RTMIDI_DUMMY, __pyx_t_1) < 0) __PYX_ERR(0, 250, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_API_WEB_MIDI, __pyx_t_1) < 0) __PYX_ERR(0, 250, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "_rtmidi.pyx":251
  * API_WINDOWS_MM = WINDOWS_MM
- * API_RTMIDI_DUMMY = RTMIDI_DUMMY
- * API_WEB_MIDI = WEB_MIDI             # <<<<<<<<<<<<<<
+ * API_WEB_MIDI = WEB_MIDI
+ * API_RTMIDI_DUMMY = RTMIDI_DUMMY             # <<<<<<<<<<<<<<
  * 
  * # export error values to Python
  */
-  __pyx_t_1 = __Pyx_PyInt_From_enum__RtMidi_3a__3a_Api(RtMidi::WEB_MIDI_API); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 251, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_enum__RtMidi_3a__3a_Api(RtMidi::RTMIDI_DUMMY); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 251, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_API_WEB_MIDI, __pyx_t_1) < 0) __PYX_ERR(0, 251, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_API_RTMIDI_DUMMY, __pyx_t_1) < 0) __PYX_ERR(0, 251, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "_rtmidi.pyx":255
  * # export error values to Python
  * 
  * ERRORTYPE_WARNING = ERR_WARNING             # <<<<<<<<<<<<<<
  * ERRORTYPE_DEBUG_WARNING = ERR_DEBUG_WARNING
```

### Comparing `python-rtmidi-1.5.1/src/_rtmidi.pyx` & `python-rtmidi-1.5.2/src/_rtmidi.pyx`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -146,16 +146,16 @@
     # https://groups.google.com/d/msg/cython-users/monwJxJCb-g/k_h1rcU-3TgJ
     cdef enum Api "RtMidi::Api":
         UNSPECIFIED  "RtMidi::UNSPECIFIED"
         MACOSX_CORE  "RtMidi::MACOSX_CORE"
         LINUX_ALSA   "RtMidi::LINUX_ALSA"
         UNIX_JACK    "RtMidi::UNIX_JACK"
         WINDOWS_MM   "RtMidi::WINDOWS_MM"
-        RTMIDI_DUMMY "RtMidi::RTMIDI_DUMMY"
         WEB_MIDI     "RtMidi::WEB_MIDI_API"
+        RTMIDI_DUMMY "RtMidi::RTMIDI_DUMMY"
 
     cdef enum ErrorType "RtMidiError::Type":
         ERR_WARNING           "RtMidiError::WARNING"
         ERR_DEBUG_WARNING     "RtMidiError::DEBUG_WARNING"
         ERR_UNSPECIFIED       "RtMidiError::UNSPECIFIED"
         ERR_NO_DEVICES_FOUND  "RtMidiError::NO_DEVICES_FOUND"
         ERR_INVALID_DEVICE    "RtMidiError::INVALID_DEVICE"
@@ -243,16 +243,16 @@
 # export Api enum values to Python
 
 API_UNSPECIFIED = UNSPECIFIED
 API_MACOSX_CORE = MACOSX_CORE
 API_LINUX_ALSA = LINUX_ALSA
 API_UNIX_JACK = UNIX_JACK
 API_WINDOWS_MM = WINDOWS_MM
-API_RTMIDI_DUMMY = RTMIDI_DUMMY
 API_WEB_MIDI = WEB_MIDI
+API_RTMIDI_DUMMY = RTMIDI_DUMMY
 
 # export error values to Python
 
 ERRORTYPE_WARNING = ERR_WARNING
 ERRORTYPE_DEBUG_WARNING = ERR_DEBUG_WARNING
 ERRORTYPE_UNSPECIFIED = ERR_UNSPECIFIED
 ERRORTYPE_NO_DEVICES_FOUND = ERR_NO_DEVICES_FOUND
```

### Comparing `python-rtmidi-1.5.1/src/meson.build` & `python-rtmidi-1.5.2/src/meson.build`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.1/src/meson_dist_cython.py` & `python-rtmidi-1.5.2/src/meson_dist_cython.py`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.1/src/rtmidi/CMakeLists.txt` & `python-rtmidi-1.5.2/src/rtmidi/CMakeLists.txt`

 * *Files 3% similar despite different names*

```diff
@@ -66,15 +66,15 @@
 foreach(_S ${CONFIGAC})
   string(REGEX REPLACE ${R} "\\1" k ${_S})
   string(REGEX REPLACE ${R} "\\2" v ${_S})
   set(SO_${k} ${v})
 endforeach()
 math(EXPR SO_current_minus_age "${SO_current} - ${SO_age}")
 set(SO_VER "${SO_current_minus_age}")
-set(FULL_VER "${SO_current_minus_age}.${SO_revision}.${SO_age}")
+set(FULL_VER "${SO_current_minus_age}.${SO_age}.${SO_revision}")
 
 # Read package version info from configure.ac
 set(R "AC_INIT\\(RtMidi, ([0-9\\.]+),.*\\)")
 file(STRINGS "${CMAKE_CURRENT_SOURCE_DIR}/configure.ac" CONFIGAC
   REGEX ${R})
 string(REGEX REPLACE ${R} "\\1" PACKAGE_VERSION ${CONFIGAC})
 
@@ -83,14 +83,15 @@
 set(LINKLIBS)
 set(PUBLICLINKLIBS)
 set(INCDIRS)
 set(PKGCONFIG_REQUIRES)
 set(LIBS_REQUIRES)
 set(API_DEFS)
 set(API_LIST)
+set(PACKAGE_DEPENDENCIES)
 
 # Tweak API-specific configuration.
 
 # Jack
 if(RTMIDI_API_JACK)
   if (NOT HAVE_JACK)
     message(FATAL_ERROR "Jack API requested but no Jack dev libraries found")
@@ -121,18 +122,19 @@
 if(RTMIDI_API_ALSA)
   set(NEED_PTHREAD ON)
   find_package(ALSA)
   if (NOT ALSA_FOUND)
     message(FATAL_ERROR "ALSA API requested but no ALSA dev libraries found")
   endif()
   list(APPEND INCDIRS ${ALSA_INCLUDE_DIR})
-  list(APPEND LINKLIBS ${ALSA_LIBRARY})
+  list(APPEND LINKLIBS ALSA::ALSA)
   list(APPEND PKGCONFIG_REQUIRES "alsa")
   list(APPEND API_DEFS "-D__LINUX_ALSA__")
   list(APPEND API_LIST "alsa")
+  list(APPEND PACKAGE_DEPENDENCIES "find_dependency(ALSA)")
 endif()
 
 # WinMM
 if(RTMIDI_API_WINMM)
   list(APPEND API_DEFS "-D__WINDOWS_MM__")
   list(APPEND API_LIST "winmm")
   list(APPEND LINKLIBS winmm)
@@ -153,14 +155,15 @@
 
 # pthread
 if (NEED_PTHREAD)
   find_package(Threads REQUIRED
     CMAKE_THREAD_PREFER_PTHREAD
     THREADS_PREFER_PTHREAD_FLAG)
   list(APPEND PUBLICLINKLIBS Threads::Threads)
+  list(APPEND PACKAGE_DEPENDENCIES "find_dependency(Threads)")
 endif()
 
 # Create library targets.
 set(LIB_TARGETS)
 
 # Use RTMIDI_BUILD_SHARED_LIBS / RTMIDI_BUILD_STATIC_LIBS if they
 # are defined, otherwise default to standard BUILD_SHARED_LIBS.
@@ -183,29 +186,29 @@
 
 # Add headers destination for install rule.
 set_property(TARGET rtmidi PROPERTY PUBLIC_HEADER RtMidi.h rtmidi_c.h)
 set_target_properties(rtmidi PROPERTIES
   SOVERSION ${SO_VER}
   VERSION ${FULL_VER})
 
+# Set standard installation directories.
+include(GNUInstallDirs)
+
 # Set include paths, populate target interface.
 target_include_directories(rtmidi PRIVATE ${INCDIRS}
                                   PUBLIC
                                     $<BUILD_INTERFACE:${CMAKE_CURRENT_SOURCE_DIR}>
                                     $<INSTALL_INTERFACE:${CMAKE_INSTALL_INCLUDEDIR}>)
 
 # Set compile-time definitions
 target_compile_definitions(rtmidi PRIVATE ${API_DEFS})
 target_compile_definitions(rtmidi PRIVATE RTMIDI_EXPORT)
 target_link_libraries(rtmidi PUBLIC ${PUBLICLINKLIBS} 
                              PRIVATE ${LINKLIBS})
 
-# Set standard installation directories.
-include(GNUInstallDirs)
-
 # Add tests if requested.
 option(RTMIDI_BUILD_TESTING "Build test programs" ON)
 if (NOT DEFINED RTMIDI_BUILD_TESTING OR RTMIDI_BUILD_TESTING STREQUAL "")
   set(RTMIDI_BUILD_TESTING ${BUILD_TESTING})
 endif()
 if (RTMIDI_BUILD_TESTING)
   include(CTest)
@@ -276,27 +279,29 @@
     DESTINATION ${CMAKE_INSTALL_LIBDIR}/pkgconfig)
 
 # Set up CMake package
 include(CMakePackageConfigHelpers)
 
 # Write cmake package version file
 write_basic_package_version_file(
-    RtMidi-config-version.cmake
+    rtmidi-config-version.cmake
     VERSION ${FULL_VER}
     COMPATIBILITY SameMajorVersion
 )
 
+string(REPLACE ";" "\n" package_dependencies "${PACKAGE_DEPENDENCIES}")
+
 # Write cmake package config file
 configure_package_config_file (
-    cmake/RtMidi-config.cmake.in
-    RtMidi-config.cmake
+    cmake/rtmidi-config.cmake.in
+    rtmidi-config.cmake
     INSTALL_DESTINATION "${RTMIDI_CMAKE_DESTINATION}"
 )
 
 # Install package files
 install (
     FILES
-        "${CMAKE_CURRENT_BINARY_DIR}/RtMidi-config.cmake"
-        "${CMAKE_CURRENT_BINARY_DIR}/RtMidi-config-version.cmake"
+        "${CMAKE_CURRENT_BINARY_DIR}/rtmidi-config.cmake"
+        "${CMAKE_CURRENT_BINARY_DIR}/rtmidi-config-version.cmake"
     DESTINATION
         "${RTMIDI_CMAKE_DESTINATION}"
 )
```

### Comparing `python-rtmidi-1.5.1/src/rtmidi/LICENSE` & `python-rtmidi-1.5.2/src/rtmidi/LICENSE`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.1/src/rtmidi/Makefile.am` & `python-rtmidi-1.5.2/src/rtmidi/Makefile.am`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.1/src/rtmidi/README.md` & `python-rtmidi-1.5.2/src/rtmidi/README.md`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.1/src/rtmidi/RtMidi.cpp` & `python-rtmidi-1.5.2/src/rtmidi/RtMidi.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -35,14 +35,17 @@
     CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION
     WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 */
 /**********************************************************************/
 
 #include "RtMidi.h"
 #include <sstream>
+#if defined(__APPLE__)
+#include <TargetConditionals.h>
+#endif
 
 #if (TARGET_OS_IPHONE == 1)
 
     #define AudioGetCurrentHostTime CAHostTimeBase::GetCurrentTime
     #define AudioConvertHostTimeToNanos CAHostTimeBase::ConvertToNanos
 
     #include <mach/mach_time.h>
@@ -374,16 +377,16 @@
 extern "C" {
 const char* rtmidi_api_names[][2] = {
   { "unspecified" , "Unknown" },
   { "core"        , "CoreMidi" },
   { "alsa"        , "ALSA" },
   { "jack"        , "Jack" },
   { "winmm"       , "Windows MultiMedia" },
-  { "dummy"       , "Dummy" },
   { "web"         , "Web MIDI API" },
+  { "dummy"       , "Dummy" },
 };
 const unsigned int rtmidi_num_api_names =
   sizeof(rtmidi_api_names)/sizeof(rtmidi_api_names[0]);
 
 // The order here will control the order of RtMidi's API search in
 // the constructor.
 extern "C" const RtMidi::Api rtmidi_compiled_apis[] = {
@@ -1174,91 +1177,87 @@
 {
   CFRunLoopRunInMode( kCFRunLoopDefaultMode, 0, false );
   return MIDIGetNumberOfSources();
 }
 
 // This function was submitted by Douglas Casey Tucker and apparently
 // derived largely from PortMidi.
-CFStringRef EndpointName( MIDIEndpointRef endpoint, bool isExternal )
+CFStringRef CreateEndpointName( MIDIEndpointRef endpoint, bool isExternal )
 {
   CFMutableStringRef result = CFStringCreateMutable( NULL, 0 );
   CFStringRef str;
 
   // Begin with the endpoint's name.
   str = NULL;
   MIDIObjectGetStringProperty( endpoint, kMIDIPropertyName, &str );
   if ( str != NULL ) {
     CFStringAppend( result, str );
-    CFRelease( str );
   }
 
   // some MIDI devices have a leading space in endpoint name. trim
-  CFStringRef space = CFStringCreateWithCString(NULL, " ", kCFStringEncodingUTF8);
-  CFStringTrim(result, space);
-  CFRelease(space);
+  CFStringTrim(result, CFSTR(" "));
 
   MIDIEntityRef entity = 0;
   MIDIEndpointGetEntity( endpoint, &entity );
   if ( entity == 0 )
     // probably virtual
     return result;
 
   if ( CFStringGetLength( result ) == 0 ) {
     // endpoint name has zero length -- try the entity
     str = NULL;
     MIDIObjectGetStringProperty( entity, kMIDIPropertyName, &str );
     if ( str != NULL ) {
       CFStringAppend( result, str );
-      CFRelease( str );
     }
   }
   // now consider the device's name
   MIDIDeviceRef device = 0;
   MIDIEntityGetDevice( entity, &device );
   if ( device == 0 )
     return result;
 
   str = NULL;
   MIDIObjectGetStringProperty( device, kMIDIPropertyName, &str );
   if ( CFStringGetLength( result ) == 0 ) {
       CFRelease( result );
+      CFRetain( str );
       return str;
   }
   if ( str != NULL ) {
     // if an external device has only one entity, throw away
     // the endpoint name and just use the device name
     if ( isExternal && MIDIDeviceGetNumberOfEntities( device ) < 2 ) {
       CFRelease( result );
+      CFRetain( str );
       return str;
     } else {
       if ( CFStringGetLength( str ) == 0 ) {
-        CFRelease( str );
         return result;
       }
       // does the entity name already start with the device name?
       // (some drivers do this though they shouldn't)
       // if so, do not prepend
       if ( CFStringCompareWithOptions( result, /* endpoint name */
                                        str /* device name */,
                                        CFRangeMake(0, CFStringGetLength( str ) ), 0 ) != kCFCompareEqualTo ) {
         // prepend the device name to the entity name
         if ( CFStringGetLength( result ) > 0 )
           CFStringInsert( result, 0, CFSTR(" ") );
 
         CFStringInsert( result, 0, str );
       }
-      CFRelease( str );
     }
   }
   return result;
 }
 
 // This function was submitted by Douglas Casey Tucker and apparently
 // derived largely from PortMidi.
-static CFStringRef ConnectedEndpointName( MIDIEndpointRef endpoint )
+static CFStringRef CreateConnectedEndpointName( MIDIEndpointRef endpoint )
 {
   CFMutableStringRef result = CFStringCreateMutable( NULL, 0 );
   CFStringRef str;
   OSStatus err;
   int i;
 
   // Does the endpoint have connections?
@@ -1277,19 +1276,20 @@
         MIDIObjectRef connObject;
         MIDIObjectType connObjectType;
         err = MIDIObjectFindByUniqueID( id, &connObject, &connObjectType );
         if ( err == noErr ) {
           if ( connObjectType == kMIDIObjectType_ExternalSource  ||
                connObjectType == kMIDIObjectType_ExternalDestination ) {
             // Connected to an external device's endpoint (10.3 and later).
-            str = EndpointName( (MIDIEndpointRef)(connObject), true );
+            str = CreateEndpointName( (MIDIEndpointRef)(connObject), true );
           } else {
             // Connected to an external device (10.2) (or something else, catch-
             str = NULL;
             MIDIObjectGetStringProperty( connObject, kMIDIPropertyName, &str );
+            if ( str ) CFRetain ( str );
           }
           if ( str != NULL ) {
             if ( anyStrings )
               CFStringAppend( result, CFSTR(", ") );
             else
               anyStrings = true;
             CFStringAppend( result, str );
@@ -1302,15 +1302,15 @@
   }
   if ( anyStrings )
     return result;
 
   CFRelease( result );
 
   // Here, either the endpoint had no connections, or we failed to obtain names
-  return EndpointName( endpoint, false );
+  return CreateEndpointName( endpoint, false );
 }
 
 std::string MidiInCore :: getPortName( unsigned int portNumber )
 {
   CFStringRef nameRef;
   MIDIEndpointRef portRef;
   char name[128];
@@ -1322,15 +1322,15 @@
     ost << "MidiInCore::getPortName: the 'portNumber' argument (" << portNumber << ") is invalid.";
     errorString_ = ost.str();
     error( RtMidiError::WARNING, errorString_ );
     return stringName;
   }
 
   portRef = MIDIGetSource( portNumber );
-  nameRef = ConnectedEndpointName( portRef );
+  nameRef = CreateConnectedEndpointName( portRef );
   CFStringGetCString( nameRef, name, sizeof(name), kCFStringEncodingUTF8 );
   CFRelease( nameRef );
 
   return stringName = name;
 }
 
 //*********************************************************************//
@@ -1409,15 +1409,15 @@
     ost << "MidiOutCore::getPortName: the 'portNumber' argument (" << portNumber << ") is invalid.";
     errorString_ = ost.str();
     error( RtMidiError::WARNING, errorString_ );
     return stringName;
   }
 
   portRef = MIDIGetDestination( portNumber );
-  nameRef = ConnectedEndpointName(portRef);
+  nameRef = CreateConnectedEndpointName(portRef);
   CFStringGetCString( nameRef, name, sizeof(name), kCFStringEncodingUTF8 );
   CFRelease( nameRef );
 
   return stringName = name;
 }
 
 void MidiOutCore :: openPort( unsigned int portNumber, const std::string &portName )
@@ -2729,15 +2729,15 @@
     errorString_ = "MidiInWinMM::openPort: error creating Windows MM MIDI input port.";
     error( RtMidiError::DRIVER_ERROR, errorString_ );
     return;
   }
 
   // Allocate and init the sysex buffers.
   data->sysexBuffer.resize( inputData_.bufferCount );
-  for ( int i=0; i < inputData_.bufferCount; ++i ) {
+  for ( unsigned int i=0; i < inputData_.bufferCount; ++i ) {
     data->sysexBuffer[i] = (MIDIHDR*) new char[ sizeof(MIDIHDR) ];
     data->sysexBuffer[i]->lpData = new char[ inputData_.bufferSize ];
     data->sysexBuffer[i]->dwBufferLength = inputData_.bufferSize;
     data->sysexBuffer[i]->dwUser = i; // We use the dwUser parameter as buffer indicator
     data->sysexBuffer[i]->dwFlags = 0;
 
     result = midiInPrepareHeader( data->inHandle, data->sysexBuffer[i], sizeof(MIDIHDR) );
@@ -2783,15 +2783,15 @@
 {
   if ( connected_ ) {
     WinMidiData *data = static_cast<WinMidiData *> (apiData_);
     EnterCriticalSection( &(data->_mutex) );
     midiInReset( data->inHandle );
     midiInStop( data->inHandle );
 
-    for ( int i=0; i < data->sysexBuffer.size(); ++i ) {
+    for ( size_t i=0; i < data->sysexBuffer.size(); ++i ) {
       int result = midiInUnprepareHeader(data->inHandle, data->sysexBuffer[i], sizeof(MIDIHDR));
       delete [] data->sysexBuffer[i]->lpData;
       delete [] data->sysexBuffer[i];
       if ( result != MMSYSERR_NOERROR ) {
         midiInClose( data->inHandle );
         data->inHandle = 0;
         errorString_ = "MidiInWinMM::openPort: error closing Windows MM MIDI input port (midiInUnprepareHeader).";
@@ -3093,14 +3093,15 @@
 #if defined(__UNIX_JACK__)
 
 // JACK header files
 #include <jack/jack.h>
 #include <jack/midiport.h>
 #include <jack/ringbuffer.h>
 #include <pthread.h>
+#include <sched.h>
 #ifdef HAVE_SEMAPHORE
   #include <semaphore.h>
 #endif
 
 #define JACK_RINGBUFFER_SIZE 16384 // Default size for ringbuffer
 
 struct JackMidiData {
@@ -3609,15 +3610,15 @@
   int nBytes = static_cast<int>(size);
   JackMidiData *data = static_cast<JackMidiData *> (apiData_);
 
   if ( size + sizeof(nBytes) > (size_t) data->buffMaxWrite )
       return;
 
   while ( jack_ringbuffer_write_space(data->buff) < sizeof(nBytes) + size )
-      pthread_yield();
+      sched_yield();
 
   // Write full message to buffer
   jack_ringbuffer_write( data->buff, ( char * ) &nBytes, sizeof( nBytes ) );
   jack_ringbuffer_write( data->buff, ( const char * ) message, nBytes );
 }
 
 #endif  // __UNIX_JACK__
@@ -3724,15 +3725,15 @@
     var port = window._rtmidi_internals_get_port_by_number($0, $1);
     if( port == null)
       return null;
     var length = lengthBytesUTF8(port.name) + 1;
     var ret = _malloc(length);
     stringToUTF8(port.name, ret, length);
     return ret;
-  }, portNumber, isInput, &ret );
+  }, portNumber, isInput);
   if (ret == nullptr)
       return "";
   std::string s = ret;
   free(ret);
   return s;
 }
```

### Comparing `python-rtmidi-1.5.1/src/rtmidi/RtMidi.h` & `python-rtmidi-1.5.2/src/rtmidi/RtMidi.h`

 * *Files 1% similar despite different names*

```diff
@@ -82,20 +82,20 @@
   //! Defined RtMidiError types.
   enum Type {
     WARNING,           /*!< A non-critical error. */
     DEBUG_WARNING,     /*!< A non-critical error which might be useful for debugging. */
     UNSPECIFIED,       /*!< The default, unspecified error type. */
     NO_DEVICES_FOUND,  /*!< No devices found on system. */
     INVALID_DEVICE,    /*!< An invalid device ID was specified. */
-    MEMORY_ERROR,      /*!< An error occured during memory allocation. */
+    MEMORY_ERROR,      /*!< An error occurred during memory allocation. */
     INVALID_PARAMETER, /*!< An invalid parameter was specified to a function. */
     INVALID_USE,       /*!< The function was called incorrectly. */
-    DRIVER_ERROR,      /*!< A system driver error occured. */
-    SYSTEM_ERROR,      /*!< A system error occured. */
-    THREAD_ERROR       /*!< A thread error occured. */
+    DRIVER_ERROR,      /*!< A system driver error occurred. */
+    SYSTEM_ERROR,      /*!< A system error occurred. */
+    THREAD_ERROR       /*!< A thread error occurred. */
   };
 
   //! The constructor.
   RtMidiError( const std::string& message, Type type = RtMidiError::UNSPECIFIED ) throw()
     : message_(message), type_(type) {}
 
   //! The destructor.
@@ -138,16 +138,16 @@
   //! MIDI API specifier arguments.
   enum Api {
     UNSPECIFIED,    /*!< Search for a working compiled API. */
     MACOSX_CORE,    /*!< Macintosh OS-X CoreMIDI API. */
     LINUX_ALSA,     /*!< The Advanced Linux Sound Architecture API. */
     UNIX_JACK,      /*!< The JACK Low-Latency MIDI Server API. */
     WINDOWS_MM,     /*!< The Microsoft Multimedia MIDI API. */
-    RTMIDI_DUMMY,   /*!< A compilable but non-functional API. */
     WEB_MIDI_API,   /*!< W3C Web MIDI API. */
+    RTMIDI_DUMMY,   /*!< A compilable but non-functional API. */
     NUM_APIS        /*!< Number of values in this enum. */
   };
 
   //! A static function to determine the current RtMidi version.
   static std::string getVersion( void ) throw();
 
   //! A static function to determine the available compiled MIDI APIs.
@@ -202,17 +202,17 @@
   //! Returns true if a port is open and false if not.
   /*!
       Note that this only applies to connections made with the openPort()
       function, not to virtual ports.
   */
   virtual bool isPortOpen( void ) const = 0;
 
-  //! Set an error callback function to be invoked when an error has occured.
+  //! Set an error callback function to be invoked when an error has occurred.
   /*!
-    The callback function will be called whenever an error has occured. It is best
+    The callback function will be called whenever an error has occurred. It is best
     to set the error callback function before opening a port.
   */
   virtual void setErrorCallback( RtMidiErrorCallback errorCallback = NULL, void *userData = 0 ) = 0;
 
  protected:
   RtMidi();
   virtual ~RtMidi();
@@ -369,17 +369,17 @@
     available or not.  A valid message is indicated by a non-zero
     vector size.  An exception is thrown if an error occurs during
     message retrieval or an input connection was not previously
     established.
   */
   double getMessage( std::vector<unsigned char> *message );
 
-  //! Set an error callback function to be invoked when an error has occured.
+  //! Set an error callback function to be invoked when an error has occurred.
   /*!
-    The callback function will be called whenever an error has occured. It is best
+    The callback function will be called whenever an error has occurred. It is best
     to set the error callback function before opening a port.
   */
   virtual void setErrorCallback( RtMidiErrorCallback errorCallback = NULL, void *userData = 0 );
 
   //! Set maximum expected incoming message size.
   /*!
     For APIs that require manual buffer management, it can be useful to set the buffer
@@ -487,17 +487,17 @@
       output connection was not previously established.
 
       \param message A pointer to the MIDI message as raw bytes
       \param size    Length of the MIDI message in bytes
   */
   void sendMessage( const unsigned char *message, size_t size );
 
-  //! Set an error callback function to be invoked when an error has occured.
+  //! Set an error callback function to be invoked when an error has occurred.
   /*!
-    The callback function will be called whenever an error has occured. It is best
+    The callback function will be called whenever an error has occurred. It is best
     to set the error callback function before opening a port.
   */
   virtual void setErrorCallback( RtMidiErrorCallback errorCallback = NULL, void *userData = 0 );
 
  protected:
   void openMidiApi( RtMidi::Api api, const std::string &clientName );
 };
```

### Comparing `python-rtmidi-1.5.1/src/rtmidi/autogen.sh` & `python-rtmidi-1.5.2/src/rtmidi/autogen.sh`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.1/src/rtmidi/cmake/RtMidiConfigUninstall.cmake.in` & `python-rtmidi-1.5.2/src/rtmidi/cmake/RtMidiConfigUninstall.cmake.in`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.1/src/rtmidi/configure.ac` & `python-rtmidi-1.5.2/src/rtmidi/configure.ac`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.1/src/rtmidi/contrib/go/rtmidi/rtmidi.go` & `python-rtmidi-1.5.2/src/rtmidi/contrib/go/rtmidi/rtmidi.go`

 * *Files 25% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 package rtmidi
 
 /*
-#cgo CXXFLAGS: -g
+#cgo CXXFLAGS: -g -std=c++11
 #cgo LDFLAGS: -g
 
 #cgo linux CXXFLAGS: -D__LINUX_ALSA__
 #cgo linux LDFLAGS: -lasound -pthread
 #cgo windows CXXFLAGS: -D__WINDOWS_MM__
 #cgo windows LDFLAGS: -luuid -lksuser -lwinmm -lole32
 #cgo darwin CXXFLAGS: -D__MACOSX_CORE__
@@ -35,25 +35,26 @@
 // API is an enumeration of possible MIDI API specifiers.
 type API C.enum_RtMidiApi
 
 const (
 	// APIUnspecified searches for a working compiled API.
 	APIUnspecified API = C.RTMIDI_API_UNSPECIFIED
 	// APIMacOSXCore uses Macintosh OS-X CoreMIDI API.
-	APIMacOSXCore = C.RTMIDI_API_MACOSX_CORE
+	APIMacOSXCore API = C.RTMIDI_API_MACOSX_CORE
 	// APILinuxALSA uses the Advanced Linux Sound Architecture API.
-	APILinuxALSA = C.RTMIDI_API_LINUX_ALSA
+	APILinuxALSA API = C.RTMIDI_API_LINUX_ALSA
 	// APIUnixJack uses the JACK Low-Latency MIDI Server API.
-	APIUnixJack = C.RTMIDI_API_UNIX_JACK
+	APIUnixJack API = C.RTMIDI_API_UNIX_JACK
 	// APIWindowsMM uses the Microsoft Multimedia MIDI API.
-	APIWindowsMM = C.RTMIDI_API_WINDOWS_MM
+	APIWindowsMM API = C.RTMIDI_API_WINDOWS_MM
 	// APIDummy is a compilable but non-functional API.
-	APIDummy = C.RTMIDI_API_RTMIDI_DUMMY
+	APIDummy API = C.RTMIDI_API_RTMIDI_DUMMY
 )
 
+// Format an API as a string
 func (api API) String() string {
 	switch api {
 	case APIUnspecified:
 		return "unspecified"
 	case APILinuxALSA:
 		return "alsa"
 	case APIUnixJack:
@@ -117,51 +118,71 @@
 	Destroy()
 }
 
 type midi struct {
 	midi C.RtMidiPtr
 }
 
+// Open a MIDI input connection given by enumeration number.
 func (m *midi) OpenPort(port int, name string) error {
 	p := C.CString(name)
 	defer C.free(unsafe.Pointer(p))
 	C.rtmidi_open_port(m.midi, C.uint(port), p)
 	if !m.midi.ok {
 		return errors.New(C.GoString(m.midi.msg))
 	}
 	return nil
 }
 
+// Create a virtual input port, with optional name, to allow software connections
+// (OS X, JACK and ALSA only).
 func (m *midi) OpenVirtualPort(name string) error {
 	p := C.CString(name)
 	defer C.free(unsafe.Pointer(p))
 	C.rtmidi_open_virtual_port(m.midi, p)
 	if !m.midi.ok {
 		return errors.New(C.GoString(m.midi.msg))
 	}
 	return nil
 }
 
+// Return a string identifier for the specified MIDI input port number.
 func (m *midi) PortName(port int) (string, error) {
-	p := C.rtmidi_get_port_name(m.midi, C.uint(port))
+	bufLen := C.int(0)
+
+	C.rtmidi_get_port_name(m.midi, C.uint(port), nil, &bufLen)
 	if !m.midi.ok {
 		return "", errors.New(C.GoString(m.midi.msg))
 	}
-	defer C.free(unsafe.Pointer(p))
-	return C.GoString(p), nil
+
+	if bufLen < 1 {
+		return "", nil
+	}
+
+	bufOut := make([]byte, int(bufLen))
+	p := (*C.char)(unsafe.Pointer(&bufOut[0]))
+
+	C.rtmidi_get_port_name(m.midi, C.uint(port), p, &bufLen)
+	if !m.midi.ok {
+		return "", errors.New(C.GoString(m.midi.msg))
+	}
+
+	return string(bufOut[0 : bufLen-1]), nil
 }
 
+// Return the number of available MIDI input ports.
 func (m *midi) PortCount() (int, error) {
 	n := C.rtmidi_get_port_count(m.midi)
 	if !m.midi.ok {
 		return 0, errors.New(C.GoString(m.midi.msg))
 	}
 	return int(n), nil
 }
 
+// Close an open MIDI connection.
 func (m *midi) Close() error {
 	C.rtmidi_close_port(C.RtMidiPtr(m.midi))
 	if !m.midi.ok {
 		return errors.New(C.GoString(m.midi.msg))
 	}
 	return nil
 }
@@ -173,54 +194,63 @@
 }
 
 type midiOut struct {
 	midi
 	out C.RtMidiOutPtr
 }
 
-// NewMIDIInDefault opens a default MIDIIn port.
+// Open a default MIDIIn port.
 func NewMIDIInDefault() (MIDIIn, error) {
 	in := C.rtmidi_in_create_default()
 	if !in.ok {
 		defer C.rtmidi_in_free(in)
 		return nil, errors.New(C.GoString(in.msg))
 	}
 	return &midiIn{in: in, midi: midi{midi: C.RtMidiPtr(in)}}, nil
 }
 
-// NewMIDIIn opens a single MIDIIn port using the given API. One can provide a
-// custom port name and a desired queue size for the incomming MIDI messages.
+// Open a single MIDIIn port using the given API. One can provide a
+// custom port name and a desired queue size for the incoming MIDI messages.
 func NewMIDIIn(api API, name string, queueSize int) (MIDIIn, error) {
 	p := C.CString(name)
 	defer C.free(unsafe.Pointer(p))
 	in := C.rtmidi_in_create(C.enum_RtMidiApi(api), p, C.uint(queueSize))
 	if !in.ok {
 		defer C.rtmidi_in_free(in)
 		return nil, errors.New(C.GoString(in.msg))
 	}
 	return &midiIn{in: in, midi: midi{midi: C.RtMidiPtr(in)}}, nil
 }
 
+// Return the MIDI API specifier for the current instance of RtMidiIn.
 func (m *midiIn) API() (API, error) {
 	api := C.rtmidi_in_get_current_api(m.in)
 	if !m.in.ok {
 		return APIUnspecified, errors.New(C.GoString(m.in.msg))
 	}
 	return API(api), nil
 }
 
+// Close an open MIDI connection (if one exists).
 func (m *midiIn) Close() error {
 	unregisterMIDIIn(m)
 	if err := m.midi.Close(); err != nil {
 		return err
 	}
 	C.rtmidi_in_free(m.in)
 	return nil
 }
 
+// Specify whether certain MIDI message types should be queued or ignored during input.
+//
+// By default, MIDI timing and active sensing messages are ignored
+// during message input because of their relative high data rates.
+// MIDI sysex messages are ignored by default as well.  Variable
+// values of "true" imply that the respective message type will be
+// ignored.
 func (m *midiIn) IgnoreTypes(midiSysex bool, midiTime bool, midiSense bool) error {
 	C.rtmidi_in_ignore_types(m.in, C._Bool(midiSysex), C._Bool(midiTime), C._Bool(midiSense))
 	if !m.in.ok {
 		return errors.New(C.GoString(m.in.msg))
 	}
 	return nil
 }
@@ -261,33 +291,39 @@
 //export goMIDIInCallback
 func goMIDIInCallback(ts C.double, msg *C.uchar, msgsz C.size_t, arg unsafe.Pointer) {
 	k := int(uintptr(arg))
 	m := findMIDIIn(k)
 	m.cb(m, C.GoBytes(unsafe.Pointer(msg), C.int(msgsz)), float64(ts))
 }
 
+// Set a callback function to be invoked for incoming MIDI messages.
 func (m *midiIn) SetCallback(cb func(MIDIIn, []byte, float64)) error {
 	k := registerMIDIIn(m)
 	m.cb = cb
 	C.cgoSetCallback(m.in, C.int(k))
 	if !m.in.ok {
 		return errors.New(C.GoString(m.in.msg))
 	}
 	return nil
 }
 
+// Cancel use of the current callback function (if one exists).
 func (m *midiIn) CancelCallback() error {
 	unregisterMIDIIn(m)
 	C.rtmidi_in_cancel_callback(m.in)
 	if !m.in.ok {
 		return errors.New(C.GoString(m.in.msg))
 	}
 	return nil
 }
 
+// Fill a byte buffer with the next available MIDI message in the input queue
+// and return the event delta-time in seconds.
+//
+// This function returns immediately whether a new message is available or not.
 func (m *midiIn) Message() ([]byte, float64, error) {
 	msg := make([]C.uchar, 64*1024, 64*1024)
 	sz := C.size_t(len(msg))
 	r := C.rtmidi_in_get_message(m.in, &msg[0], &sz)
 	if !m.in.ok {
 		return nil, 0, errors.New(C.GoString(m.in.msg))
 	}
@@ -298,52 +334,55 @@
 	return b, float64(r), nil
 }
 
 func (m *midiIn) Destroy() {
 	C.rtmidi_in_free(m.in)
 }
 
-// NewMIDIOutDefault opens a default MIDIOut port.
+// Open a default MIDIOut port.
 func NewMIDIOutDefault() (MIDIOut, error) {
 	out := C.rtmidi_out_create_default()
 	if !out.ok {
 		defer C.rtmidi_out_free(out)
 		return nil, errors.New(C.GoString(out.msg))
 	}
 	return &midiOut{out: out, midi: midi{midi: C.RtMidiPtr(out)}}, nil
 }
 
-// NewMIDIOut opens a single MIDIIn port using the given API with the given port name.
+// Open a single MIDIIn port using the given API with the given port name.
 func NewMIDIOut(api API, name string) (MIDIOut, error) {
 	p := C.CString(name)
 	defer C.free(unsafe.Pointer(p))
 	out := C.rtmidi_out_create(C.enum_RtMidiApi(api), p)
 	if !out.ok {
 		defer C.rtmidi_out_free(out)
 		return nil, errors.New(C.GoString(out.msg))
 	}
 	return &midiOut{out: out, midi: midi{midi: C.RtMidiPtr(out)}}, nil
 }
 
+// Return the MIDI API specifier for the current instance of RtMidiOut.
 func (m *midiOut) API() (API, error) {
 	api := C.rtmidi_out_get_current_api(m.out)
 	if !m.out.ok {
 		return APIUnspecified, errors.New(C.GoString(m.out.msg))
 	}
 	return API(api), nil
 }
 
+// Close an open MIDI connection.
 func (m *midiOut) Close() error {
 	if err := m.midi.Close(); err != nil {
 		return err
 	}
 	C.rtmidi_out_free(m.out)
 	return nil
 }
 
+// Immediately send a single message out an open MIDI output port.
 func (m *midiOut) SendMessage(b []byte) error {
 	p := C.CBytes(b)
 	defer C.free(unsafe.Pointer(p))
 	C.rtmidi_out_send_message(m.out, (*C.uchar)(p), C.int(len(b)))
 	if !m.out.ok {
 		return errors.New(C.GoString(m.out.msg))
 	}
```

### Comparing `python-rtmidi-1.5.1/src/rtmidi/contrib/go/rtmidi/rtmidi_test.go` & `python-rtmidi-1.5.2/src/rtmidi/contrib/go/rtmidi/rtmidi_test.go`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.1/src/rtmidi/doc/Makefile.am` & `python-rtmidi-1.5.2/src/rtmidi/doc/Makefile.am`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.1/src/rtmidi/doc/doxygen/Doxyfile.in` & `python-rtmidi-1.5.2/src/rtmidi/doc/doxygen/Doxyfile.in`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.1/src/rtmidi/doc/doxygen/tutorial.txt` & `python-rtmidi-1.5.2/src/rtmidi/doc/doxygen/tutorial.txt`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.1/src/rtmidi/doc/images/ccrma.gif` & `python-rtmidi-1.5.2/src/rtmidi/doc/images/ccrma.gif`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.1/src/rtmidi/doc/images/mcgill.gif` & `python-rtmidi-1.5.2/src/rtmidi/doc/images/mcgill.gif`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.1/src/rtmidi/doc/release.txt` & `python-rtmidi-1.5.2/src/rtmidi/doc/release.txt`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.1/src/rtmidi/m4/ax_cxx_compile_stdcxx.m4` & `python-rtmidi-1.5.2/src/rtmidi/m4/ax_cxx_compile_stdcxx.m4`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.1/src/rtmidi/msw/rtmidilib.sln` & `python-rtmidi-1.5.2/src/rtmidi/msw/rtmidilib.sln`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.1/src/rtmidi/msw/rtmidilib.vcproj` & `python-rtmidi-1.5.2/src/rtmidi/msw/rtmidilib.vcproj`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.1/src/rtmidi/rtmidi_c.cpp` & `python-rtmidi-1.5.2/src/rtmidi/rtmidi_c.cpp`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 #include <string.h>
 #include <stdlib.h>
 #include "rtmidi_c.h"
 #include "RtMidi.h"
 
 /* Compile-time assertions that will break if the enums are changed in
  * the future without synchronizing them properly.  If you get (g++)
- * "error: ‘StaticAssert<b>::StaticAssert() [with bool b = false]’ is
- * private within this context", it means enums are not aligned. */
-template<bool b> class StaticAssert { private: StaticAssert() {} };
-template<> class StaticAssert<true>{ public: StaticAssert() {} };
-#define ENUM_EQUAL(x,y) StaticAssert<(int)x==(int)y>()
-class StaticAssertions { StaticAssertions() {
+ * "error: ‘StaticEnumAssert<b>::StaticEnumAssert() [with bool b = false]’
+ * is private within this context", it means enums are not aligned. */
+template<bool b> class StaticEnumAssert { private: StaticEnumAssert() {} };
+template<> class StaticEnumAssert<true>{ public: StaticEnumAssert() {} };
+#define ENUM_EQUAL(x,y) StaticEnumAssert<(int)x==(int)y>()
+class StaticEnumAssertions { StaticEnumAssertions() {
     ENUM_EQUAL( RTMIDI_API_UNSPECIFIED,     RtMidi::UNSPECIFIED );
     ENUM_EQUAL( RTMIDI_API_MACOSX_CORE,     RtMidi::MACOSX_CORE );
     ENUM_EQUAL( RTMIDI_API_LINUX_ALSA,      RtMidi::LINUX_ALSA );
     ENUM_EQUAL( RTMIDI_API_UNIX_JACK,       RtMidi::UNIX_JACK );
     ENUM_EQUAL( RTMIDI_API_WINDOWS_MM,      RtMidi::WINDOWS_MM );
     ENUM_EQUAL( RTMIDI_API_RTMIDI_DUMMY,    RtMidi::RTMIDI_DUMMY );
-    ENUM_EQUAL( RTMIDI_API_WEB_MIDI_API,    RtMidi::WEB_MIDI_API );
 
     ENUM_EQUAL( RTMIDI_ERROR_WARNING,            RtMidiError::WARNING );
     ENUM_EQUAL( RTMIDI_ERROR_DEBUG_WARNING,      RtMidiError::DEBUG_WARNING );
     ENUM_EQUAL( RTMIDI_ERROR_UNSPECIFIED,        RtMidiError::UNSPECIFIED );
     ENUM_EQUAL( RTMIDI_ERROR_NO_DEVICES_FOUND,   RtMidiError::NO_DEVICES_FOUND );
     ENUM_EQUAL( RTMIDI_ERROR_INVALID_DEVICE,     RtMidiError::INVALID_DEVICE );
     ENUM_EQUAL( RTMIDI_ERROR_MEMORY_ERROR,       RtMidiError::MEMORY_ERROR );
@@ -39,15 +38,17 @@
     : c_callback (cCallback), user_data (userData)
   {
   }
   RtMidiCCallback c_callback;
   void *user_data;
 };
 
-extern "C" const enum RtMidiApi rtmidi_compiled_apis[]; // casting from RtMidi::Api[]
+#ifndef RTMIDI_SOURCE_INCLUDED
+    extern "C" const enum RtMidiApi rtmidi_compiled_apis[]; // casting from RtMidi::Api[]
+#endif
 extern "C" const unsigned int rtmidi_num_compiled_apis;
 
 /* RtMidi API */
 int rtmidi_get_compiled_api (enum RtMidiApi *apis, unsigned int apis_size)
 {
     unsigned num = rtmidi_num_compiled_apis;
     if (apis) {
```

### Comparing `python-rtmidi-1.5.1/src/rtmidi/rtmidi_c.h` & `python-rtmidi-1.5.2/src/rtmidi/rtmidi_c.h`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     //! The wrapped RtMidi object.
     void* ptr;
     void* data;
 
     //! True when the last function call was OK.
     bool  ok;
 
-    //! If an error occured (ok != true), set to an error message.
+    //! If an error occurred (ok != true), set to an error message.
     const char* msg;
 };
 
 //! \brief Typedef for a generic RtMidi pointer.
 typedef struct RtMidiWrapper* RtMidiPtr;
 
 //! \brief Typedef for a generic RtMidiIn pointer.
@@ -60,32 +60,32 @@
 //! \brief MIDI API specifier arguments.  See \ref RtMidi::Api.
 enum RtMidiApi {
     RTMIDI_API_UNSPECIFIED,    /*!< Search for a working compiled API. */
     RTMIDI_API_MACOSX_CORE,    /*!< Macintosh OS-X CoreMIDI API. */
     RTMIDI_API_LINUX_ALSA,     /*!< The Advanced Linux Sound Architecture API. */
     RTMIDI_API_UNIX_JACK,      /*!< The Jack Low-Latency MIDI Server API. */
     RTMIDI_API_WINDOWS_MM,     /*!< The Microsoft Multimedia MIDI API. */
-    RTMIDI_API_RTMIDI_DUMMY,   /*!< A compilable but non-functional API. */
     RTMIDI_API_WEB_MIDI_API,   /*!< W3C Web MIDI API. */
+    RTMIDI_API_RTMIDI_DUMMY,   /*!< A compilable but non-functional API. */
     RTMIDI_API_NUM             /*!< Number of values in this enum. */
 };
 
 //! \brief Defined RtMidiError types. See \ref RtMidiError::Type.
 enum RtMidiErrorType {
   RTMIDI_ERROR_WARNING,           /*!< A non-critical error. */
   RTMIDI_ERROR_DEBUG_WARNING,     /*!< A non-critical error which might be useful for debugging. */
   RTMIDI_ERROR_UNSPECIFIED,       /*!< The default, unspecified error type. */
   RTMIDI_ERROR_NO_DEVICES_FOUND,  /*!< No devices found on system. */
   RTMIDI_ERROR_INVALID_DEVICE,    /*!< An invalid device ID was specified. */
-  RTMIDI_ERROR_MEMORY_ERROR,      /*!< An error occured during memory allocation. */
+  RTMIDI_ERROR_MEMORY_ERROR,      /*!< An error occurred during memory allocation. */
   RTMIDI_ERROR_INVALID_PARAMETER, /*!< An invalid parameter was specified to a function. */
   RTMIDI_ERROR_INVALID_USE,       /*!< The function was called incorrectly. */
-  RTMIDI_ERROR_DRIVER_ERROR,      /*!< A system driver error occured. */
-  RTMIDI_ERROR_SYSTEM_ERROR,      /*!< A system error occured. */
-  RTMIDI_ERROR_THREAD_ERROR       /*!< A thread error occured. */
+  RTMIDI_ERROR_DRIVER_ERROR,      /*!< A system driver error occurred. */
+  RTMIDI_ERROR_SYSTEM_ERROR,      /*!< A system error occurred. */
+  RTMIDI_ERROR_THREAD_ERROR       /*!< A thread error occurred. */
 };
 
 /*! \brief The type of a RtMidi callback function.
  *
  * \param timeStamp   The time at which the message has been received.
  * \param message     The midi message.
  * \param userData    Additional user data for the callback.
@@ -153,18 +153,18 @@
 
 /*! \brief Return the number of available MIDI ports.
  * See RtMidi::getPortCount().
  */
 RTMIDIAPI unsigned int rtmidi_get_port_count (RtMidiPtr device);
 
 /*! \brief Access a string identifier for the specified MIDI input port number.
- *
+ * 
  * To prevent memory leaks a char buffer must be passed to this function.
  * NULL can be passed as bufOut parameter, and that will write the required buffer length in the bufLen.
- *
+ * 
  * See RtMidi::getPortName().
  */
 RTMIDIAPI int rtmidi_get_port_name (RtMidiPtr device, unsigned int portNumber, char * bufOut, int * bufLen);
 
 /* RtMidiIn API */
 
 //! \brief Create a default RtMidiInPtr value, with no initialization.
```

### Comparing `python-rtmidi-1.5.1/src/rtmidi/tests/Makefile.am` & `python-rtmidi-1.5.2/src/rtmidi/tests/Makefile.am`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.1/src/rtmidi/tests/RtMidi.dsw` & `python-rtmidi-1.5.2/src/rtmidi/tests/RtMidi.dsw`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.1/src/rtmidi/tests/apinames.cpp` & `python-rtmidi-1.5.2/src/rtmidi/tests/apinames.cpp`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.1/src/rtmidi/tests/cmidiin.cpp` & `python-rtmidi-1.5.2/src/rtmidi/tests/cmidiin.cpp`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.1/src/rtmidi/tests/cmidiin.dsp` & `python-rtmidi-1.5.2/src/rtmidi/tests/cmidiin.dsp`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.1/src/rtmidi/tests/midiclock.cpp` & `python-rtmidi-1.5.2/src/rtmidi/tests/midiclock.cpp`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.1/src/rtmidi/tests/midiout.cpp` & `python-rtmidi-1.5.2/src/rtmidi/tests/midiout.cpp`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.1/src/rtmidi/tests/midiout.dsp` & `python-rtmidi-1.5.2/src/rtmidi/tests/midiout.dsp`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.1/src/rtmidi/tests/midiprobe.cpp` & `python-rtmidi-1.5.2/src/rtmidi/tests/midiprobe.cpp`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.1/src/rtmidi/tests/midiprobe.dsp` & `python-rtmidi-1.5.2/src/rtmidi/tests/midiprobe.dsp`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.1/src/rtmidi/tests/qmidiin.cpp` & `python-rtmidi-1.5.2/src/rtmidi/tests/qmidiin.cpp`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.1/src/rtmidi/tests/qmidiin.dsp` & `python-rtmidi-1.5.2/src/rtmidi/tests/qmidiin.dsp`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.1/src/rtmidi/tests/sysextest.cpp` & `python-rtmidi-1.5.2/src/rtmidi/tests/sysextest.cpp`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.1/src/rtmidi/tests/sysextest.dsp` & `python-rtmidi-1.5.2/src/rtmidi/tests/sysextest.dsp`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.1/src/rtmidi/tests/testcapi.c` & `python-rtmidi-1.5.2/src/rtmidi/tests/testcapi.c`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.1/tests/test_basic.py` & `python-rtmidi-1.5.2/tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.1/tests/test_delete.py` & `python-rtmidi-1.5.2/tests/test_delete.py`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.1/tests/test_errorcallback.py` & `python-rtmidi-1.5.2/tests/test_errorcallback.py`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.1/tests/test_errors.py` & `python-rtmidi-1.5.2/tests/test_errors.py`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.1/tests/test_rtmidi.py` & `python-rtmidi-1.5.2/tests/test_rtmidi.py`

 * *Files 0% similar despite different names*

```diff
@@ -53,15 +53,15 @@
                 self.assertEqual(res, api)
             else:
                 self.assertEqual(res, rtmidi.API_UNSPECIFIED)
 
     def test_get_rtmidi_version(self):
         version = rtmidi.get_rtmidi_version()
         self.assertTrue(isinstance(version, string_types))
-        self.assertEqual(version, '4.0.0')
+        self.assertEqual(version, '5.0.0')
 
 
 class BaseTests:
     NOTE_ON = [0x90, 48, 100]
     NOTE_OFF = [0x80, 48, 16]
     IN_CLIENT_NAME = "RtMidiTestCase In"
     OUT_CLIENT_NAME = "RtMidiTestCase Out"
```

### Comparing `python-rtmidi-1.5.1/PKG-INFO` & `python-rtmidi-1.5.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-rtmidi
-Version: 1.5.1
+Version: 1.5.2
 Summary: A Python binding for the RtMidi C++ library implemented using Cython.
 Keywords: MIDI, multimedia, music, rtmidi
 Author: Christopher Arndt
 Author-email: info@chrisarndt.de
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: MacOS X
 Classifier: Environment :: Win32 (MS Windows)
@@ -28,19 +28,19 @@
 Project-URL: Download, https://pypi.python.org/pypi/python-rtmidi
 Project-URL: Homepage, https://github.com/SpotlightKid/python-rtmidi
 Project-URL: Source, https://gitlab.com/SpotlightKid/python-rtmidi/
 License:
        |Copyright & License
        |===================
        |
-       |python-rtmidi was written by Christopher Arndt, 2012 - 2021.
+       |python-rtmidi was written by Christopher Arndt, 2012 - 2023.
        |
        |The software is released unter the MIT License:
        |
-       |Copyright (c) 2012 - 2022 Christopher Arndt
+       |Copyright (c) 2012 - 2023 Christopher Arndt
        |
        |    Permission is hereby granted, free of charge, to any person obtaining a
        |    copy of this software and associated documentation files (the "Software"),
        |    to deal in the Software without restriction, including without limitation
        |    the rights to use, copy, modify, merge, publish, distribute, sublicense,
        |    and/or sell copies of the Software, and to permit persons to whom the
        |    Software is furnished to do so, subject to the following conditions:
@@ -94,15 +94,15 @@
 A Python binding for the RtMidi C++ library implemented using Cython.
 
 [![Latest version](https://shields.io/pypi/v/python-rtmidi)](https://pypi.org/project/python-rtmidi)
 ![Project status](https://shields.io/pypi/status/python-rtmidi)
 [![MIT License](https://shields.io/pypi/l/python-rtmidi)](LICENSE.md)
 ![Python versions](https://shields.io/pypi/pyversions/python-rtmidi)
 [![Distribution format](https://shields.io/pypi/format/python-rtmidi)](https://pypi.org/project/python-rtmidi/#files)
-[![Travis CI status](https://travis-ci.org/SpotlightKid/python-rtmidi.svg?branch=master)](https://travis-ci.org/SpotlightKid/python-rtmidi)
+[![CI status](https://github.com/SpotlightKid/python-rtmidi/actions/workflows/push_to_master.yml/badge.svg)](https://github.com/SpotlightKid/python-rtmidi/actions)
 
 # Overview
 
 [RtMidi] is a set of C++ classes which provides a concise and simple,
 cross-platform API (Application Programming Interface) for realtime MIDI
 input / output across Linux (ALSA & JACK), macOS / OS X (CoreMIDI & JACK), and
 Windows (MultiMedia System) operating systems.
```

