# Comparing `tmp/wagtail-katex-0.0.3.tar.gz` & `tmp/wagtail-katex-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wagtail-katex-0.0.3.tar", last modified: Sat May 28 08:12:42 2022, max compression
+gzip compressed data, was "wagtail-katex-0.0.4.tar", last modified: Wed Jun 14 14:56:31 2023, max compression
```

## Comparing `wagtail-katex-0.0.3.tar` & `wagtail-katex-0.0.4.tar`

### file list

```diff
@@ -1,86 +1,89 @@
-drwxr-xr-x   0 chii       (501) staff       (20)        0 2022-05-28 08:12:42.503686 wagtail-katex-0.0.3/
--rw-r--r--   0 chii       (501) staff       (20)    11357 2022-03-05 02:43:30.000000 wagtail-katex-0.0.3/LICENSE
--rw-r--r--   0 chii       (501) staff       (20)       40 2022-03-05 01:58:29.000000 wagtail-katex-0.0.3/MANIFEST.in
--rw-r--r--   0 chii       (501) staff       (20)     1972 2022-05-28 08:12:42.503543 wagtail-katex-0.0.3/PKG-INFO
--rw-r--r--   0 chii       (501) staff       (20)      918 2022-05-28 08:01:07.000000 wagtail-katex-0.0.3/README.md
--rw-r--r--   0 chii       (501) staff       (20)       38 2022-05-28 08:12:42.503733 wagtail-katex-0.0.3/setup.cfg
--rw-r--r--   0 chii       (501) staff       (20)     1400 2022-05-28 07:00:50.000000 wagtail-katex-0.0.3/setup.py
-drwxr-xr-x   0 chii       (501) staff       (20)        0 2022-05-28 08:12:42.483144 wagtail-katex-0.0.3/wagtail_katex.egg-info/
--rw-r--r--   0 chii       (501) staff       (20)     1972 2022-05-28 08:12:42.000000 wagtail-katex-0.0.3/wagtail_katex.egg-info/PKG-INFO
--rw-r--r--   0 chii       (501) staff       (20)     4786 2022-05-28 08:12:42.000000 wagtail-katex-0.0.3/wagtail_katex.egg-info/SOURCES.txt
--rw-r--r--   0 chii       (501) staff       (20)        1 2022-05-28 08:12:42.000000 wagtail-katex-0.0.3/wagtail_katex.egg-info/dependency_links.txt
--rw-r--r--   0 chii       (501) staff       (20)       13 2022-05-28 08:12:42.000000 wagtail-katex-0.0.3/wagtail_katex.egg-info/requires.txt
--rw-r--r--   0 chii       (501) staff       (20)       13 2022-05-28 08:12:42.000000 wagtail-katex-0.0.3/wagtail_katex.egg-info/top_level.txt
-drwxr-xr-x   0 chii       (501) staff       (20)        0 2022-05-28 08:12:42.483805 wagtail-katex-0.0.3/wagtailkatex/
--rw-r--r--   0 chii       (501) staff       (20)       22 2022-05-28 07:42:31.000000 wagtail-katex-0.0.3/wagtailkatex/__init__.py
--rwxr-xr-x   0 chii       (501) staff       (20)      814 2022-05-28 07:20:48.000000 wagtail-katex-0.0.3/wagtailkatex/richtext.py
-drwxr-xr-x   0 chii       (501) staff       (20)        0 2022-05-28 08:12:42.484053 wagtail-katex-0.0.3/wagtailkatex/static/
--rw-r--r--   0 chii       (501) staff       (20)     6148 2021-03-04 07:31:57.000000 wagtail-katex-0.0.3/wagtailkatex/static/.DS_Store
-drwxr-xr-x   0 chii       (501) staff       (20)        0 2022-05-28 08:12:42.484319 wagtail-katex-0.0.3/wagtailkatex/static/wagtailkatex/
-drwxr-xr-x   0 chii       (501) staff       (20)        0 2022-05-28 08:12:42.485241 wagtail-katex-0.0.3/wagtailkatex/static/wagtailkatex/katex/
--rw-r--r--   0 chii       (501) staff       (20)     7119 2022-01-12 17:36:05.000000 wagtail-katex-0.0.3/wagtailkatex/static/wagtailkatex/katex/README.md
-drwxr-xr-x   0 chii       (501) staff       (20)        0 2022-05-28 08:12:42.503269 wagtail-katex-0.0.3/wagtailkatex/static/wagtailkatex/katex/fonts/
--rw-r--r--   0 chii       (501) staff       (20)    63632 2022-01-12 17:36:05.000000 wagtail-katex-0.0.3/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_AMS-Regular.ttf
--rw-r--r--   0 chii       (501) staff       (20)    33516 2022-01-12 17:36:05.000000 wagtail-katex-0.0.3/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_AMS-Regular.woff
--rw-r--r--   0 chii       (501) staff       (20)    28076 2022-01-12 17:36:05.000000 wagtail-katex-0.0.3/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_AMS-Regular.woff2
--rw-r--r--   0 chii       (501) staff       (20)    12368 2022-01-12 17:36:05.000000 wagtail-katex-0.0.3/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Caligraphic-Bold.ttf
--rw-r--r--   0 chii       (501) staff       (20)     7716 2022-01-12 17:36:05.000000 wagtail-katex-0.0.3/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Caligraphic-Bold.woff
--rw-r--r--   0 chii       (501) staff       (20)     6912 2022-01-12 17:36:05.000000 wagtail-katex-0.0.3/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Caligraphic-Bold.woff2
--rw-r--r--   0 chii       (501) staff       (20)    12344 2022-01-12 17:36:05.000000 wagtail-katex-0.0.3/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Caligraphic-Regular.ttf
--rw-r--r--   0 chii       (501) staff       (20)     7656 2022-01-12 17:36:05.000000 wagtail-katex-0.0.3/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Caligraphic-Regular.woff
--rw-r--r--   0 chii       (501) staff       (20)     6908 2022-01-12 17:36:05.000000 wagtail-katex-0.0.3/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Caligraphic-Regular.woff2
--rw-r--r--   0 chii       (501) staff       (20)    19584 2022-01-12 17:36:05.000000 wagtail-katex-0.0.3/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Fraktur-Bold.ttf
--rw-r--r--   0 chii       (501) staff       (20)    13296 2022-01-12 17:36:05.000000 wagtail-katex-0.0.3/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Fraktur-Bold.woff
--rw-r--r--   0 chii       (501) staff       (20)    11348 2022-01-12 17:36:05.000000 wagtail-katex-0.0.3/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Fraktur-Bold.woff2
--rw-r--r--   0 chii       (501) staff       (20)    19572 2022-01-12 17:36:05.000000 wagtail-katex-0.0.3/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Fraktur-Regular.ttf
--rw-r--r--   0 chii       (501) staff       (20)    13208 2022-01-12 17:36:05.000000 wagtail-katex-0.0.3/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Fraktur-Regular.woff
--rw-r--r--   0 chii       (501) staff       (20)    11316 2022-01-12 17:36:05.000000 wagtail-katex-0.0.3/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Fraktur-Regular.woff2
--rw-r--r--   0 chii       (501) staff       (20)    51336 2022-01-12 17:36:05.000000 wagtail-katex-0.0.3/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Main-Bold.ttf
--rw-r--r--   0 chii       (501) staff       (20)    29912 2022-01-12 17:36:05.000000 wagtail-katex-0.0.3/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Main-Bold.woff
--rw-r--r--   0 chii       (501) staff       (20)    25324 2022-01-12 17:36:05.000000 wagtail-katex-0.0.3/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Main-Bold.woff2
--rw-r--r--   0 chii       (501) staff       (20)    32968 2022-01-12 17:36:05.000000 wagtail-katex-0.0.3/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Main-BoldItalic.ttf
--rw-r--r--   0 chii       (501) staff       (20)    19412 2022-01-12 17:36:05.000000 wagtail-katex-0.0.3/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Main-BoldItalic.woff
--rw-r--r--   0 chii       (501) staff       (20)    16780 2022-01-12 17:36:05.000000 wagtail-katex-0.0.3/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Main-BoldItalic.woff2
--rw-r--r--   0 chii       (501) staff       (20)    33580 2022-01-12 17:36:05.000000 wagtail-katex-0.0.3/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Main-Italic.ttf
--rw-r--r--   0 chii       (501) staff       (20)    19676 2022-01-12 17:36:05.000000 wagtail-katex-0.0.3/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Main-Italic.woff
--rw-r--r--   0 chii       (501) staff       (20)    16988 2022-01-12 17:36:05.000000 wagtail-katex-0.0.3/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Main-Italic.woff2
--rw-r--r--   0 chii       (501) staff       (20)    53580 2022-01-12 17:36:05.000000 wagtail-katex-0.0.3/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Main-Regular.ttf
--rw-r--r--   0 chii       (501) staff       (20)    30772 2022-01-12 17:36:05.000000 wagtail-katex-0.0.3/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Main-Regular.woff
--rw-r--r--   0 chii       (501) staff       (20)    26272 2022-01-12 17:36:05.000000 wagtail-katex-0.0.3/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Main-Regular.woff2
--rw-r--r--   0 chii       (501) staff       (20)    31196 2022-01-12 17:36:05.000000 wagtail-katex-0.0.3/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Math-BoldItalic.ttf
--rw-r--r--   0 chii       (501) staff       (20)    18668 2022-01-12 17:36:05.000000 wagtail-katex-0.0.3/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Math-BoldItalic.woff
--rw-r--r--   0 chii       (501) staff       (20)    16400 2022-01-12 17:36:05.000000 wagtail-katex-0.0.3/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Math-BoldItalic.woff2
--rw-r--r--   0 chii       (501) staff       (20)    31308 2022-01-12 17:36:05.000000 wagtail-katex-0.0.3/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Math-Italic.ttf
--rw-r--r--   0 chii       (501) staff       (20)    18748 2022-01-12 17:36:05.000000 wagtail-katex-0.0.3/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Math-Italic.woff
--rw-r--r--   0 chii       (501) staff       (20)    16440 2022-01-12 17:36:05.000000 wagtail-katex-0.0.3/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Math-Italic.woff2
--rw-r--r--   0 chii       (501) staff       (20)    24504 2022-01-12 17:36:05.000000 wagtail-katex-0.0.3/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_SansSerif-Bold.ttf
--rw-r--r--   0 chii       (501) staff       (20)    14408 2022-01-12 17:36:05.000000 wagtail-katex-0.0.3/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_SansSerif-Bold.woff
--rw-r--r--   0 chii       (501) staff       (20)    12216 2022-01-12 17:36:05.000000 wagtail-katex-0.0.3/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_SansSerif-Bold.woff2
--rw-r--r--   0 chii       (501) staff       (20)    22364 2022-01-12 17:36:05.000000 wagtail-katex-0.0.3/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_SansSerif-Italic.ttf
--rw-r--r--   0 chii       (501) staff       (20)    14112 2022-01-12 17:36:05.000000 wagtail-katex-0.0.3/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_SansSerif-Italic.woff
--rw-r--r--   0 chii       (501) staff       (20)    12028 2022-01-12 17:36:05.000000 wagtail-katex-0.0.3/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_SansSerif-Italic.woff2
--rw-r--r--   0 chii       (501) staff       (20)    19436 2022-01-12 17:36:05.000000 wagtail-katex-0.0.3/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_SansSerif-Regular.ttf
--rw-r--r--   0 chii       (501) staff       (20)    12316 2022-01-12 17:36:05.000000 wagtail-katex-0.0.3/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_SansSerif-Regular.woff
--rw-r--r--   0 chii       (501) staff       (20)    10344 2022-01-12 17:36:05.000000 wagtail-katex-0.0.3/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_SansSerif-Regular.woff2
--rw-r--r--   0 chii       (501) staff       (20)    16648 2022-01-12 17:36:05.000000 wagtail-katex-0.0.3/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Script-Regular.ttf
--rw-r--r--   0 chii       (501) staff       (20)    10588 2022-01-12 17:36:05.000000 wagtail-katex-0.0.3/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Script-Regular.woff
--rw-r--r--   0 chii       (501) staff       (20)     9644 2022-01-12 17:36:05.000000 wagtail-katex-0.0.3/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Script-Regular.woff2
--rw-r--r--   0 chii       (501) staff       (20)    12228 2022-01-12 17:36:05.000000 wagtail-katex-0.0.3/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Size1-Regular.ttf
--rw-r--r--   0 chii       (501) staff       (20)     6496 2022-01-12 17:36:05.000000 wagtail-katex-0.0.3/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Size1-Regular.woff
--rw-r--r--   0 chii       (501) staff       (20)     5468 2022-01-12 17:36:05.000000 wagtail-katex-0.0.3/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Size1-Regular.woff2
--rw-r--r--   0 chii       (501) staff       (20)    11508 2022-01-12 17:36:05.000000 wagtail-katex-0.0.3/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Size2-Regular.ttf
--rw-r--r--   0 chii       (501) staff       (20)     6188 2022-01-12 17:36:05.000000 wagtail-katex-0.0.3/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Size2-Regular.woff
--rw-r--r--   0 chii       (501) staff       (20)     5208 2022-01-12 17:36:05.000000 wagtail-katex-0.0.3/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Size2-Regular.woff2
--rw-r--r--   0 chii       (501) staff       (20)     7588 2022-01-12 17:36:05.000000 wagtail-katex-0.0.3/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Size3-Regular.ttf
--rw-r--r--   0 chii       (501) staff       (20)     4420 2022-01-12 17:36:05.000000 wagtail-katex-0.0.3/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Size3-Regular.woff
--rw-r--r--   0 chii       (501) staff       (20)     3624 2022-01-12 17:36:05.000000 wagtail-katex-0.0.3/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Size3-Regular.woff2
--rw-r--r--   0 chii       (501) staff       (20)    10364 2022-01-12 17:36:05.000000 wagtail-katex-0.0.3/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Size4-Regular.ttf
--rw-r--r--   0 chii       (501) staff       (20)     5980 2022-01-12 17:36:05.000000 wagtail-katex-0.0.3/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Size4-Regular.woff
--rw-r--r--   0 chii       (501) staff       (20)     4928 2022-01-12 17:36:05.000000 wagtail-katex-0.0.3/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Size4-Regular.woff2
--rw-r--r--   0 chii       (501) staff       (20)    27556 2022-01-12 17:36:05.000000 wagtail-katex-0.0.3/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Typewriter-Regular.ttf
--rw-r--r--   0 chii       (501) staff       (20)    16028 2022-01-12 17:36:05.000000 wagtail-katex-0.0.3/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Typewriter-Regular.woff
--rw-r--r--   0 chii       (501) staff       (20)    13568 2022-01-12 17:36:05.000000 wagtail-katex-0.0.3/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Typewriter-Regular.woff2
--rw-r--r--   0 chii       (501) staff       (20)    23112 2022-01-12 17:36:05.000000 wagtail-katex-0.0.3/wagtailkatex/static/wagtailkatex/katex/katex.min.css
--rw-r--r--   0 chii       (501) staff       (20)   270375 2022-01-12 17:36:05.000000 wagtail-katex-0.0.3/wagtailkatex/static/wagtailkatex/katex/katex.min.js
--rwxr-xr-x   0 chii       (501) staff       (20)     3868 2022-05-28 07:44:46.000000 wagtail-katex-0.0.3/wagtailkatex/static/wagtailkatex/wagtailkatex.js
--rwxr-xr-x   0 chii       (501) staff       (20)     1420 2022-05-28 07:41:48.000000 wagtail-katex-0.0.3/wagtailkatex/wagtail_hooks.py
+drwxr-xr-x   0 chii       (501) staff       (20)        0 2023-06-14 14:56:31.178448 wagtail-katex-0.0.4/
+-rw-r--r--   0 chii       (501) staff       (20)    11357 2022-03-05 02:43:30.000000 wagtail-katex-0.0.4/LICENSE
+-rw-r--r--   0 chii       (501) staff       (20)      100 2023-06-14 14:55:14.000000 wagtail-katex-0.0.4/MANIFEST.in
+-rw-r--r--   0 chii       (501) staff       (20)     2011 2023-06-14 14:56:31.178270 wagtail-katex-0.0.4/PKG-INFO
+-rw-r--r--   0 chii       (501) staff       (20)      918 2022-05-28 08:01:07.000000 wagtail-katex-0.0.4/README.md
+-rw-r--r--   0 chii       (501) staff       (20)       38 2023-06-14 14:56:31.178501 wagtail-katex-0.0.4/setup.cfg
+-rw-r--r--   0 chii       (501) staff       (20)     1436 2023-06-14 14:44:59.000000 wagtail-katex-0.0.4/setup.py
+drwxr-xr-x   0 chii       (501) staff       (20)        0 2023-06-14 14:56:31.164939 wagtail-katex-0.0.4/wagtail_katex.egg-info/
+-rw-r--r--   0 chii       (501) staff       (20)     2011 2023-06-14 14:56:31.000000 wagtail-katex-0.0.4/wagtail_katex.egg-info/PKG-INFO
+-rw-r--r--   0 chii       (501) staff       (20)     4847 2023-06-14 14:56:31.000000 wagtail-katex-0.0.4/wagtail_katex.egg-info/SOURCES.txt
+-rw-r--r--   0 chii       (501) staff       (20)        1 2023-06-14 14:56:31.000000 wagtail-katex-0.0.4/wagtail_katex.egg-info/dependency_links.txt
+-rw-r--r--   0 chii       (501) staff       (20)       11 2023-06-14 14:56:31.000000 wagtail-katex-0.0.4/wagtail_katex.egg-info/requires.txt
+-rw-r--r--   0 chii       (501) staff       (20)       13 2023-06-14 14:56:31.000000 wagtail-katex-0.0.4/wagtail_katex.egg-info/top_level.txt
+drwxr-xr-x   0 chii       (501) staff       (20)        0 2023-06-14 14:56:31.165453 wagtail-katex-0.0.4/wagtailkatex/
+-rw-r--r--   0 chii       (501) staff       (20)       22 2023-06-13 00:40:46.000000 wagtail-katex-0.0.4/wagtailkatex/__init__.py
+-rwxr-xr-x   0 chii       (501) staff       (20)      860 2023-06-13 00:40:46.000000 wagtail-katex-0.0.4/wagtailkatex/richtext.py
+drwxr-xr-x   0 chii       (501) staff       (20)        0 2023-06-14 14:56:31.165614 wagtail-katex-0.0.4/wagtailkatex/static/
+-rw-r--r--   0 chii       (501) staff       (20)     6148 2021-03-04 07:31:57.000000 wagtail-katex-0.0.4/wagtailkatex/static/.DS_Store
+drwxr-xr-x   0 chii       (501) staff       (20)        0 2023-06-14 14:56:31.165776 wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/
+drwxr-xr-x   0 chii       (501) staff       (20)        0 2023-06-14 14:56:31.166319 wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/
+-rw-r--r--   0 chii       (501) staff       (20)     7119 2022-01-12 17:36:05.000000 wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/README.md
+drwxr-xr-x   0 chii       (501) staff       (20)        0 2023-06-14 14:56:31.177824 wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/
+-rw-r--r--   0 chii       (501) staff       (20)    63632 2022-01-12 17:36:05.000000 wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_AMS-Regular.ttf
+-rw-r--r--   0 chii       (501) staff       (20)    33516 2022-01-12 17:36:05.000000 wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_AMS-Regular.woff
+-rw-r--r--   0 chii       (501) staff       (20)    28076 2022-01-12 17:36:05.000000 wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_AMS-Regular.woff2
+-rw-r--r--   0 chii       (501) staff       (20)    12368 2022-01-12 17:36:05.000000 wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Caligraphic-Bold.ttf
+-rw-r--r--   0 chii       (501) staff       (20)     7716 2022-01-12 17:36:05.000000 wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Caligraphic-Bold.woff
+-rw-r--r--   0 chii       (501) staff       (20)     6912 2022-01-12 17:36:05.000000 wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Caligraphic-Bold.woff2
+-rw-r--r--   0 chii       (501) staff       (20)    12344 2022-01-12 17:36:05.000000 wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Caligraphic-Regular.ttf
+-rw-r--r--   0 chii       (501) staff       (20)     7656 2022-01-12 17:36:05.000000 wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Caligraphic-Regular.woff
+-rw-r--r--   0 chii       (501) staff       (20)     6908 2022-01-12 17:36:05.000000 wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Caligraphic-Regular.woff2
+-rw-r--r--   0 chii       (501) staff       (20)    19584 2022-01-12 17:36:05.000000 wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Fraktur-Bold.ttf
+-rw-r--r--   0 chii       (501) staff       (20)    13296 2022-01-12 17:36:05.000000 wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Fraktur-Bold.woff
+-rw-r--r--   0 chii       (501) staff       (20)    11348 2022-01-12 17:36:05.000000 wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Fraktur-Bold.woff2
+-rw-r--r--   0 chii       (501) staff       (20)    19572 2022-01-12 17:36:05.000000 wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Fraktur-Regular.ttf
+-rw-r--r--   0 chii       (501) staff       (20)    13208 2022-01-12 17:36:05.000000 wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Fraktur-Regular.woff
+-rw-r--r--   0 chii       (501) staff       (20)    11316 2022-01-12 17:36:05.000000 wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Fraktur-Regular.woff2
+-rw-r--r--   0 chii       (501) staff       (20)    51336 2022-01-12 17:36:05.000000 wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Main-Bold.ttf
+-rw-r--r--   0 chii       (501) staff       (20)    29912 2022-01-12 17:36:05.000000 wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Main-Bold.woff
+-rw-r--r--   0 chii       (501) staff       (20)    25324 2022-01-12 17:36:05.000000 wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Main-Bold.woff2
+-rw-r--r--   0 chii       (501) staff       (20)    32968 2022-01-12 17:36:05.000000 wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Main-BoldItalic.ttf
+-rw-r--r--   0 chii       (501) staff       (20)    19412 2022-01-12 17:36:05.000000 wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Main-BoldItalic.woff
+-rw-r--r--   0 chii       (501) staff       (20)    16780 2022-01-12 17:36:05.000000 wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Main-BoldItalic.woff2
+-rw-r--r--   0 chii       (501) staff       (20)    33580 2022-01-12 17:36:05.000000 wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Main-Italic.ttf
+-rw-r--r--   0 chii       (501) staff       (20)    19676 2022-01-12 17:36:05.000000 wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Main-Italic.woff
+-rw-r--r--   0 chii       (501) staff       (20)    16988 2022-01-12 17:36:05.000000 wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Main-Italic.woff2
+-rw-r--r--   0 chii       (501) staff       (20)    53580 2022-01-12 17:36:05.000000 wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Main-Regular.ttf
+-rw-r--r--   0 chii       (501) staff       (20)    30772 2022-01-12 17:36:05.000000 wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Main-Regular.woff
+-rw-r--r--   0 chii       (501) staff       (20)    26272 2022-01-12 17:36:05.000000 wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Main-Regular.woff2
+-rw-r--r--   0 chii       (501) staff       (20)    31196 2022-01-12 17:36:05.000000 wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Math-BoldItalic.ttf
+-rw-r--r--   0 chii       (501) staff       (20)    18668 2022-01-12 17:36:05.000000 wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Math-BoldItalic.woff
+-rw-r--r--   0 chii       (501) staff       (20)    16400 2022-01-12 17:36:05.000000 wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Math-BoldItalic.woff2
+-rw-r--r--   0 chii       (501) staff       (20)    31308 2022-01-12 17:36:05.000000 wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Math-Italic.ttf
+-rw-r--r--   0 chii       (501) staff       (20)    18748 2022-01-12 17:36:05.000000 wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Math-Italic.woff
+-rw-r--r--   0 chii       (501) staff       (20)    16440 2022-01-12 17:36:05.000000 wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Math-Italic.woff2
+-rw-r--r--   0 chii       (501) staff       (20)    24504 2022-01-12 17:36:05.000000 wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_SansSerif-Bold.ttf
+-rw-r--r--   0 chii       (501) staff       (20)    14408 2022-01-12 17:36:05.000000 wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_SansSerif-Bold.woff
+-rw-r--r--   0 chii       (501) staff       (20)    12216 2022-01-12 17:36:05.000000 wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_SansSerif-Bold.woff2
+-rw-r--r--   0 chii       (501) staff       (20)    22364 2022-01-12 17:36:05.000000 wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_SansSerif-Italic.ttf
+-rw-r--r--   0 chii       (501) staff       (20)    14112 2022-01-12 17:36:05.000000 wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_SansSerif-Italic.woff
+-rw-r--r--   0 chii       (501) staff       (20)    12028 2022-01-12 17:36:05.000000 wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_SansSerif-Italic.woff2
+-rw-r--r--   0 chii       (501) staff       (20)    19436 2022-01-12 17:36:05.000000 wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_SansSerif-Regular.ttf
+-rw-r--r--   0 chii       (501) staff       (20)    12316 2022-01-12 17:36:05.000000 wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_SansSerif-Regular.woff
+-rw-r--r--   0 chii       (501) staff       (20)    10344 2022-01-12 17:36:05.000000 wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_SansSerif-Regular.woff2
+-rw-r--r--   0 chii       (501) staff       (20)    16648 2022-01-12 17:36:05.000000 wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Script-Regular.ttf
+-rw-r--r--   0 chii       (501) staff       (20)    10588 2022-01-12 17:36:05.000000 wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Script-Regular.woff
+-rw-r--r--   0 chii       (501) staff       (20)     9644 2022-01-12 17:36:05.000000 wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Script-Regular.woff2
+-rw-r--r--   0 chii       (501) staff       (20)    12228 2022-01-12 17:36:05.000000 wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Size1-Regular.ttf
+-rw-r--r--   0 chii       (501) staff       (20)     6496 2022-01-12 17:36:05.000000 wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Size1-Regular.woff
+-rw-r--r--   0 chii       (501) staff       (20)     5468 2022-01-12 17:36:05.000000 wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Size1-Regular.woff2
+-rw-r--r--   0 chii       (501) staff       (20)    11508 2022-01-12 17:36:05.000000 wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Size2-Regular.ttf
+-rw-r--r--   0 chii       (501) staff       (20)     6188 2022-01-12 17:36:05.000000 wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Size2-Regular.woff
+-rw-r--r--   0 chii       (501) staff       (20)     5208 2022-01-12 17:36:05.000000 wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Size2-Regular.woff2
+-rw-r--r--   0 chii       (501) staff       (20)     7588 2022-01-12 17:36:05.000000 wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Size3-Regular.ttf
+-rw-r--r--   0 chii       (501) staff       (20)     4420 2022-01-12 17:36:05.000000 wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Size3-Regular.woff
+-rw-r--r--   0 chii       (501) staff       (20)     3624 2022-01-12 17:36:05.000000 wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Size3-Regular.woff2
+-rw-r--r--   0 chii       (501) staff       (20)    10364 2022-01-12 17:36:05.000000 wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Size4-Regular.ttf
+-rw-r--r--   0 chii       (501) staff       (20)     5980 2022-01-12 17:36:05.000000 wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Size4-Regular.woff
+-rw-r--r--   0 chii       (501) staff       (20)     4928 2022-01-12 17:36:05.000000 wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Size4-Regular.woff2
+-rw-r--r--   0 chii       (501) staff       (20)    27556 2022-01-12 17:36:05.000000 wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Typewriter-Regular.ttf
+-rw-r--r--   0 chii       (501) staff       (20)    16028 2022-01-12 17:36:05.000000 wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Typewriter-Regular.woff
+-rw-r--r--   0 chii       (501) staff       (20)    13568 2022-01-12 17:36:05.000000 wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Typewriter-Regular.woff2
+-rw-r--r--   0 chii       (501) staff       (20)    23112 2022-01-12 17:36:05.000000 wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/katex.min.css
+-rw-r--r--   0 chii       (501) staff       (20)   270375 2022-01-12 17:36:05.000000 wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/katex.min.js
+-rwxr-xr-x   0 chii       (501) staff       (20)     3868 2022-05-28 07:44:46.000000 wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/wagtailkatex.js
+drwxr-xr-x   0 chii       (501) staff       (20)        0 2023-06-14 14:56:31.163401 wagtail-katex-0.0.4/wagtailkatex/templates/
+drwxr-xr-x   0 chii       (501) staff       (20)        0 2023-06-14 14:56:31.178011 wagtail-katex-0.0.4/wagtailkatex/templates/wagtailkatex/
+-rw-r--r--   0 chii       (501) staff       (20)      875 2023-06-14 14:42:43.000000 wagtail-katex-0.0.4/wagtailkatex/templates/wagtailkatex/square-root-variable.svg
+-rwxr-xr-x   0 chii       (501) staff       (20)     1562 2023-06-14 14:42:58.000000 wagtail-katex-0.0.4/wagtailkatex/wagtail_hooks.py
```

### Comparing `wagtail-katex-0.0.3/LICENSE` & `wagtail-katex-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `wagtail-katex-0.0.3/PKG-INFO` & `wagtail-katex-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 Metadata-Version: 2.1
 Name: wagtail-katex
-Version: 0.0.3
+Version: 0.0.4
 Summary: KaTex for Wagtail CMS Draftail editor
 Home-page: https://github.com/ongchi/wagtail-katex
 Author: ongchi
 Author-email: ongchi@users.noreply.github.com
 Project-URL: Bug Tracker, https://github.com/ongchi/wagtail-katex/issues
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Framework :: Django
 Classifier: Framework :: Wagtail
-Classifier: Framework :: Wagtail :: 2
 Classifier: Framework :: Wagtail :: 3
+Classifier: Framework :: Wagtail :: 4
+Classifier: Framework :: Wagtail :: 5
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # wagtail-katex ![Wagtail 2.x](https://img.shields.io/badge/wagtail-2.x-g.svg) ![Wagtail 3.x](https://img.shields.io/badge/wagtail-3.x-g.svg)
 
 > This package is modified from [gatensj/wagtail-draftail-katex](https://github.com/gatensj/wagtail-draftail-katex)
```

### Comparing `wagtail-katex-0.0.3/README.md` & `wagtail-katex-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `wagtail-katex-0.0.3/setup.py` & `wagtail-katex-0.0.4/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,29 +13,30 @@
     description='KaTex for Wagtail CMS Draftail editor',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/ongchi/wagtail-katex',
     project_urls={
         "Bug Tracker": "https://github.com/ongchi/wagtail-katex/issues",
     },
-    install_requires=['wagtail>=2.3'],
+    install_requires=['wagtail>=3'],
     classifiers=[
         'Environment :: Web Environment',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: Apache Software License',
         "Operating System :: OS Independent",
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.5',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
         'Framework :: Django',
         'Framework :: Wagtail',
-        'Framework :: Wagtail :: 2',
         'Framework :: Wagtail :: 3',
+        'Framework :: Wagtail :: 4',
+        'Framework :: Wagtail :: 5',
     ],
     packages=find_packages(),
     include_package_data=True,
     python_requires=">=3.6",
 )
```

### Comparing `wagtail-katex-0.0.3/wagtail_katex.egg-info/PKG-INFO` & `wagtail-katex-0.0.4/wagtail_katex.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 Metadata-Version: 2.1
 Name: wagtail-katex
-Version: 0.0.3
+Version: 0.0.4
 Summary: KaTex for Wagtail CMS Draftail editor
 Home-page: https://github.com/ongchi/wagtail-katex
 Author: ongchi
 Author-email: ongchi@users.noreply.github.com
 Project-URL: Bug Tracker, https://github.com/ongchi/wagtail-katex/issues
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Framework :: Django
 Classifier: Framework :: Wagtail
-Classifier: Framework :: Wagtail :: 2
 Classifier: Framework :: Wagtail :: 3
+Classifier: Framework :: Wagtail :: 4
+Classifier: Framework :: Wagtail :: 5
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # wagtail-katex ![Wagtail 2.x](https://img.shields.io/badge/wagtail-2.x-g.svg) ![Wagtail 3.x](https://img.shields.io/badge/wagtail-3.x-g.svg)
 
 > This package is modified from [gatensj/wagtail-draftail-katex](https://github.com/gatensj/wagtail-draftail-katex)
```

### Comparing `wagtail-katex-0.0.3/wagtail_katex.egg-info/SOURCES.txt` & `wagtail-katex-0.0.4/wagtail_katex.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -70,8 +70,9 @@
 wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Size3-Regular.woff
 wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Size3-Regular.woff2
 wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Size4-Regular.ttf
 wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Size4-Regular.woff
 wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Size4-Regular.woff2
 wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Typewriter-Regular.ttf
 wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Typewriter-Regular.woff
-wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Typewriter-Regular.woff2
+wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Typewriter-Regular.woff2
+wagtailkatex/templates/wagtailkatex/square-root-variable.svg
```

### Comparing `wagtail-katex-0.0.3/wagtailkatex/richtext.py` & `wagtail-katex-0.0.4/wagtailkatex/richtext.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,31 @@
 from draftjs_exporter.dom import DOM
 from wagtail.admin.rich_text.converters.contentstate_models import Entity
-from wagtail.admin.rich_text.converters.html_to_contentstate import AtomicBlockEntityElementHandler
+from wagtail.admin.rich_text.converters.html_to_contentstate import (
+    AtomicBlockEntityElementHandler,
+)
 
 
 def katex_entity_decorator(props):
     """
-    Takes Draft.js ContentState and converts it to HTML for saving in the Database.
+    Takes Draft.js ContentState and converts it to HTML for saving in the database.
     """
-    return DOM.create_element('div', {
-        'data-katex-embed': props['text'],
-    })
+    return DOM.create_element(
+        "div",
+        {"data-katex-embed": props["text"]},
+    )
 
 
 class KaTeXEntityElementHandler(AtomicBlockEntityElementHandler):
     """
-    Takes Database HTML and converts it to Draft.js ContentState for display in the editor.
+    Takes Database HTML and converts it to Draft.js ContentState for display in the
+    editor.
     """
-    mutability = 'MUTABLE'
+
+    mutability = "MUTABLE"
 
     def create_entity(self, name, attrs, state, contentstate):
-        return Entity('KATEX-EMBED', 'IMMUTABLE', {
-            'text': attrs['data-katex-embed'],
-        })
+        return Entity(
+            "KATEX-EMBED",
+            "IMMUTABLE",
+            {"text": attrs["data-katex-embed"]},
+        )
```

### Comparing `wagtail-katex-0.0.3/wagtailkatex/static/.DS_Store` & `wagtail-katex-0.0.4/wagtailkatex/static/.DS_Store`

 * *Files identical despite different names*

### Comparing `wagtail-katex-0.0.3/wagtailkatex/static/wagtailkatex/katex/README.md` & `wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/README.md`

 * *Files identical despite different names*

### Comparing `wagtail-katex-0.0.3/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_AMS-Regular.ttf` & `wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_AMS-Regular.ttf`

 * *Files identical despite different names*

### Comparing `wagtail-katex-0.0.3/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_AMS-Regular.woff` & `wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_AMS-Regular.woff`

 * *Files identical despite different names*

### Comparing `wagtail-katex-0.0.3/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_AMS-Regular.woff2` & `wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_AMS-Regular.woff2`

 * *Files identical despite different names*

### Comparing `wagtail-katex-0.0.3/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Caligraphic-Bold.ttf` & `wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Caligraphic-Bold.ttf`

 * *Files identical despite different names*

### Comparing `wagtail-katex-0.0.3/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Caligraphic-Bold.woff` & `wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Caligraphic-Bold.woff`

 * *Files identical despite different names*

### Comparing `wagtail-katex-0.0.3/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Caligraphic-Bold.woff2` & `wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Caligraphic-Bold.woff2`

 * *Files identical despite different names*

### Comparing `wagtail-katex-0.0.3/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Caligraphic-Regular.ttf` & `wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Caligraphic-Regular.ttf`

 * *Files identical despite different names*

### Comparing `wagtail-katex-0.0.3/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Caligraphic-Regular.woff` & `wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Caligraphic-Regular.woff`

 * *Files identical despite different names*

### Comparing `wagtail-katex-0.0.3/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Caligraphic-Regular.woff2` & `wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Caligraphic-Regular.woff2`

 * *Files identical despite different names*

### Comparing `wagtail-katex-0.0.3/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Fraktur-Bold.ttf` & `wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Fraktur-Bold.ttf`

 * *Files identical despite different names*

### Comparing `wagtail-katex-0.0.3/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Fraktur-Bold.woff` & `wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Fraktur-Bold.woff`

 * *Files identical despite different names*

### Comparing `wagtail-katex-0.0.3/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Fraktur-Bold.woff2` & `wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Fraktur-Bold.woff2`

 * *Files identical despite different names*

### Comparing `wagtail-katex-0.0.3/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Fraktur-Regular.ttf` & `wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Fraktur-Regular.ttf`

 * *Files identical despite different names*

### Comparing `wagtail-katex-0.0.3/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Fraktur-Regular.woff` & `wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Fraktur-Regular.woff`

 * *Files identical despite different names*

### Comparing `wagtail-katex-0.0.3/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Fraktur-Regular.woff2` & `wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Fraktur-Regular.woff2`

 * *Files identical despite different names*

### Comparing `wagtail-katex-0.0.3/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Main-Bold.ttf` & `wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Main-Bold.ttf`

 * *Files identical despite different names*

### Comparing `wagtail-katex-0.0.3/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Main-Bold.woff` & `wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Main-Bold.woff`

 * *Files identical despite different names*

### Comparing `wagtail-katex-0.0.3/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Main-Bold.woff2` & `wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Main-Bold.woff2`

 * *Files identical despite different names*

### Comparing `wagtail-katex-0.0.3/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Main-BoldItalic.ttf` & `wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Main-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `wagtail-katex-0.0.3/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Main-BoldItalic.woff` & `wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Main-BoldItalic.woff`

 * *Files identical despite different names*

### Comparing `wagtail-katex-0.0.3/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Main-BoldItalic.woff2` & `wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Main-BoldItalic.woff2`

 * *Files identical despite different names*

### Comparing `wagtail-katex-0.0.3/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Main-Italic.ttf` & `wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Main-Italic.ttf`

 * *Files identical despite different names*

### Comparing `wagtail-katex-0.0.3/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Main-Italic.woff` & `wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Main-Italic.woff`

 * *Files identical despite different names*

### Comparing `wagtail-katex-0.0.3/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Main-Italic.woff2` & `wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Main-Italic.woff2`

 * *Files identical despite different names*

### Comparing `wagtail-katex-0.0.3/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Main-Regular.ttf` & `wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Main-Regular.ttf`

 * *Files identical despite different names*

### Comparing `wagtail-katex-0.0.3/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Main-Regular.woff` & `wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Main-Regular.woff`

 * *Files identical despite different names*

### Comparing `wagtail-katex-0.0.3/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Main-Regular.woff2` & `wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Main-Regular.woff2`

 * *Files identical despite different names*

### Comparing `wagtail-katex-0.0.3/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Math-BoldItalic.ttf` & `wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Math-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `wagtail-katex-0.0.3/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Math-BoldItalic.woff` & `wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Math-BoldItalic.woff`

 * *Files identical despite different names*

### Comparing `wagtail-katex-0.0.3/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Math-BoldItalic.woff2` & `wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Math-BoldItalic.woff2`

 * *Files identical despite different names*

### Comparing `wagtail-katex-0.0.3/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Math-Italic.ttf` & `wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Math-Italic.ttf`

 * *Files identical despite different names*

### Comparing `wagtail-katex-0.0.3/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Math-Italic.woff` & `wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Math-Italic.woff`

 * *Files identical despite different names*

### Comparing `wagtail-katex-0.0.3/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Math-Italic.woff2` & `wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Math-Italic.woff2`

 * *Files identical despite different names*

### Comparing `wagtail-katex-0.0.3/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_SansSerif-Bold.ttf` & `wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_SansSerif-Bold.ttf`

 * *Files identical despite different names*

### Comparing `wagtail-katex-0.0.3/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_SansSerif-Bold.woff` & `wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_SansSerif-Bold.woff`

 * *Files identical despite different names*

### Comparing `wagtail-katex-0.0.3/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_SansSerif-Bold.woff2` & `wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_SansSerif-Bold.woff2`

 * *Files identical despite different names*

### Comparing `wagtail-katex-0.0.3/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_SansSerif-Italic.ttf` & `wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_SansSerif-Italic.ttf`

 * *Files identical despite different names*

### Comparing `wagtail-katex-0.0.3/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_SansSerif-Italic.woff` & `wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_SansSerif-Italic.woff`

 * *Files identical despite different names*

### Comparing `wagtail-katex-0.0.3/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_SansSerif-Italic.woff2` & `wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_SansSerif-Italic.woff2`

 * *Files identical despite different names*

### Comparing `wagtail-katex-0.0.3/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_SansSerif-Regular.ttf` & `wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_SansSerif-Regular.ttf`

 * *Files identical despite different names*

### Comparing `wagtail-katex-0.0.3/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_SansSerif-Regular.woff` & `wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_SansSerif-Regular.woff`

 * *Files identical despite different names*

### Comparing `wagtail-katex-0.0.3/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_SansSerif-Regular.woff2` & `wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_SansSerif-Regular.woff2`

 * *Files identical despite different names*

### Comparing `wagtail-katex-0.0.3/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Script-Regular.ttf` & `wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Script-Regular.ttf`

 * *Files identical despite different names*

### Comparing `wagtail-katex-0.0.3/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Script-Regular.woff` & `wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Script-Regular.woff`

 * *Files identical despite different names*

### Comparing `wagtail-katex-0.0.3/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Script-Regular.woff2` & `wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Script-Regular.woff2`

 * *Files identical despite different names*

### Comparing `wagtail-katex-0.0.3/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Size1-Regular.ttf` & `wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Size1-Regular.ttf`

 * *Files identical despite different names*

### Comparing `wagtail-katex-0.0.3/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Size1-Regular.woff` & `wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Size1-Regular.woff`

 * *Files identical despite different names*

### Comparing `wagtail-katex-0.0.3/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Size1-Regular.woff2` & `wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Size1-Regular.woff2`

 * *Files identical despite different names*

### Comparing `wagtail-katex-0.0.3/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Size2-Regular.ttf` & `wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Size2-Regular.ttf`

 * *Files identical despite different names*

### Comparing `wagtail-katex-0.0.3/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Size2-Regular.woff` & `wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Size2-Regular.woff`

 * *Files identical despite different names*

### Comparing `wagtail-katex-0.0.3/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Size2-Regular.woff2` & `wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Size2-Regular.woff2`

 * *Files identical despite different names*

### Comparing `wagtail-katex-0.0.3/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Size3-Regular.ttf` & `wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Size3-Regular.ttf`

 * *Files identical despite different names*

### Comparing `wagtail-katex-0.0.3/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Size3-Regular.woff` & `wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Size3-Regular.woff`

 * *Files identical despite different names*

### Comparing `wagtail-katex-0.0.3/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Size3-Regular.woff2` & `wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Size3-Regular.woff2`

 * *Files identical despite different names*

### Comparing `wagtail-katex-0.0.3/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Size4-Regular.ttf` & `wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Size4-Regular.ttf`

 * *Files identical despite different names*

### Comparing `wagtail-katex-0.0.3/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Size4-Regular.woff` & `wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Size4-Regular.woff`

 * *Files identical despite different names*

### Comparing `wagtail-katex-0.0.3/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Size4-Regular.woff2` & `wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Size4-Regular.woff2`

 * *Files identical despite different names*

### Comparing `wagtail-katex-0.0.3/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Typewriter-Regular.ttf` & `wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Typewriter-Regular.ttf`

 * *Files identical despite different names*

### Comparing `wagtail-katex-0.0.3/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Typewriter-Regular.woff` & `wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Typewriter-Regular.woff`

 * *Files identical despite different names*

### Comparing `wagtail-katex-0.0.3/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Typewriter-Regular.woff2` & `wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Typewriter-Regular.woff2`

 * *Files identical despite different names*

### Comparing `wagtail-katex-0.0.3/wagtailkatex/static/wagtailkatex/katex/katex.min.css` & `wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/katex.min.css`

 * *Files identical despite different names*

### Comparing `wagtail-katex-0.0.3/wagtailkatex/static/wagtailkatex/katex/katex.min.js` & `wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/katex.min.js`

 * *Files identical despite different names*

### Comparing `wagtail-katex-0.0.3/wagtailkatex/static/wagtailkatex/wagtailkatex.js` & `wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/wagtailkatex.js`

 * *Files identical despite different names*

### Comparing `wagtail-katex-0.0.3/wagtailkatex/wagtail_hooks.py` & `wagtail-katex-0.0.4/wagtailkatex/wagtail_hooks.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 from django.utils.translation import gettext
 
 from wagtail.admin.rich_text.editors.draftail import features as draftail_features
-from wagtail.core import hooks
+from wagtail import hooks
 
 from .richtext import KaTeXEntityElementHandler, katex_entity_decorator
 
 
 @hooks.register('register_rich_text_features')
 def register_katex_features(features):
     features.default_features.append('katex')
     """
     Registering the `katex` feature, which uses the `KATEX` Draft.js entity type,
-    and is stored as HTML with a `<div data-katex-embed="c = \\pm\\sqrt{a^2 + b^2}">` tag.
+    and is stored as HTML with a `<div data-katex-embed="c = \\pm\\sqrt{a^2 + b^2}">`
+    tag.
     """
     feature_name = 'katex-embed'
     type_ = 'KATEX-EMBED'
 
     features.register_editor_plugin(
         'draftail',
         feature_name,
         draftail_features.EntityFeature(
             {
                 'type': type_,
-                'icon': 'square-root-alt',
+                'icon': 'square-root-variable',
                 'description': gettext('Equation'),
             },
             js=[
                 'wagtailkatex/katex/katex.min.js',
                 'wagtailkatex/wagtailkatex.js',
             ],
             css={
@@ -37,7 +38,14 @@
         )
     )
 
     features.register_converter_rule('contentstate', feature_name, {
         'from_database_format': {'div[data-katex-embed]': KaTeXEntityElementHandler()},
         'to_database_format': {'entity_decorators': {type_: katex_entity_decorator}},
     })
+
+
+@hooks.register('register_icons')
+def register_icons(icons):
+    return icons + [
+        "wagtailkatex/square-root-variable.svg"
+    ]
```

