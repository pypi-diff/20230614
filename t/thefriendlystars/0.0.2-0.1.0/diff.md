# Comparing `tmp/thefriendlystars-0.0.2.tar.gz` & `tmp/thefriendlystars-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/thefriendlystars-0.0.2.tar", last modified: Thu Oct  4 14:52:45 2018, max compression
+gzip compressed data, was "thefriendlystars-0.1.0.tar", last modified: Wed Jun 14 03:20:23 2023, max compression
```

## Comparing `thefriendlystars-0.0.2.tar` & `thefriendlystars-0.1.0.tar`

### file list

```diff
@@ -1,25 +1,18 @@
-drwxr-xr-x   0 zkbt       (502) staff       (20)        0 2018-10-04 14:52:45.000000 thefriendlystars-0.0.2/
--rw-r--r--   0 zkbt       (502) staff       (20)     2643 2018-10-04 14:52:45.000000 thefriendlystars-0.0.2/PKG-INFO
--rw-r--r--   0 zkbt       (502) staff       (20)     1592 2018-10-04 14:50:49.000000 thefriendlystars-0.0.2/setup.py
--rw-r--r--   0 zkbt       (502) staff       (20)     1894 2018-06-29 15:47:02.000000 thefriendlystars-0.0.2/README.md
--rw-r--r--   0 zkbt       (502) staff       (20)       38 2018-10-04 14:52:45.000000 thefriendlystars-0.0.2/setup.cfg
-drwxr-xr-x   0 zkbt       (502) staff       (20)        0 2018-10-04 14:52:45.000000 thefriendlystars-0.0.2/thefriendlystars.egg-info/
--rw-r--r--   0 zkbt       (502) staff       (20)        1 2018-06-22 16:02:41.000000 thefriendlystars-0.0.2/thefriendlystars.egg-info/not-zip-safe
--rw-r--r--   0 zkbt       (502) staff       (20)     2643 2018-10-04 14:52:45.000000 thefriendlystars-0.0.2/thefriendlystars.egg-info/PKG-INFO
--rw-r--r--   0 zkbt       (502) staff       (20)       42 2018-10-04 14:52:45.000000 thefriendlystars-0.0.2/thefriendlystars.egg-info/requires.txt
--rw-r--r--   0 zkbt       (502) staff       (20)       17 2018-10-04 14:52:45.000000 thefriendlystars-0.0.2/thefriendlystars.egg-info/top_level.txt
--rw-r--r--   0 zkbt       (502) staff       (20)      638 2018-10-04 14:52:45.000000 thefriendlystars-0.0.2/thefriendlystars.egg-info/SOURCES.txt
--rw-r--r--   0 zkbt       (502) staff       (20)        1 2018-10-04 14:52:45.000000 thefriendlystars-0.0.2/thefriendlystars.egg-info/dependency_links.txt
-drwxr-xr-x   0 zkbt       (502) staff       (20)        0 2018-10-04 14:52:45.000000 thefriendlystars-0.0.2/thefriendlystars/
--rw-r--r--   0 zkbt       (502) staff       (20)     2818 2018-03-15 03:08:30.000000 thefriendlystars-0.0.2/thefriendlystars/talker.py
-drwxr-xr-x   0 zkbt       (502) staff       (20)        0 2018-10-04 14:52:45.000000 thefriendlystars-0.0.2/thefriendlystars/constellations/
--rw-r--r--   0 zkbt       (502) staff       (20)    14955 2018-09-07 23:20:59.000000 thefriendlystars-0.0.2/thefriendlystars/constellations/constellation.py
--rw-r--r--   0 zkbt       (502) staff       (20)       69 2018-08-04 21:27:28.000000 thefriendlystars-0.0.2/thefriendlystars/constellations/__init__.py
--rw-r--r--   0 zkbt       (502) staff       (20)     6583 2018-07-05 16:07:34.000000 thefriendlystars-0.0.2/thefriendlystars/constellations/gaia.py
--rw-r--r--   0 zkbt       (502) staff       (20)     3401 2018-06-22 20:25:37.000000 thefriendlystars-0.0.2/thefriendlystars/constellations/others.py
--rw-r--r--   0 zkbt       (502) staff       (20)     4979 2018-07-05 16:17:39.000000 thefriendlystars-0.0.2/thefriendlystars/constellations/lspm.py
--rw-r--r--   0 zkbt       (502) staff       (20)       22 2018-10-04 14:51:12.000000 thefriendlystars-0.0.2/thefriendlystars/version.py
--rw-r--r--   0 zkbt       (502) staff       (20)     2235 2018-06-09 05:28:19.000000 thefriendlystars-0.0.2/thefriendlystars/finders.py
--rw-r--r--   0 zkbt       (502) staff       (20)      199 2018-10-04 14:48:44.000000 thefriendlystars-0.0.2/thefriendlystars/__init__.py
--rw-r--r--   0 zkbt       (502) staff       (20)      656 2018-07-06 01:34:11.000000 thefriendlystars-0.0.2/thefriendlystars/imports.py
--rw-r--r--   0 zkbt       (502) staff       (20)     1083 2018-05-08 19:27:28.000000 thefriendlystars-0.0.2/thefriendlystars/panels.py
+drwxr-xr-x   0 zach       (502) staff       (20)        0 2023-06-14 03:20:23.841244 thefriendlystars-0.1.0/
+-rw-r--r--   0 zach       (502) staff       (20)     1076 2023-06-14 03:17:18.000000 thefriendlystars-0.1.0/LICENSE
+-rw-r--r--   0 zach       (502) staff       (20)      616 2023-06-14 03:20:23.840994 thefriendlystars-0.1.0/PKG-INFO
+-rw-r--r--   0 zach       (502) staff       (20)     2299 2023-06-14 03:19:01.000000 thefriendlystars-0.1.0/README.md
+-rw-r--r--   0 zach       (502) staff       (20)       38 2023-06-14 03:20:23.841312 thefriendlystars-0.1.0/setup.cfg
+-rw-r--r--   0 zach       (502) staff       (20)     3882 2023-06-14 03:18:21.000000 thefriendlystars-0.1.0/setup.py
+drwxr-xr-x   0 zach       (502) staff       (20)        0 2023-06-14 03:20:23.839170 thefriendlystars-0.1.0/thefriendlystars/
+-rw-r--r--   0 zach       (502) staff       (20)       19 2023-06-14 03:17:18.000000 thefriendlystars-0.1.0/thefriendlystars/__init__.py
+-rw-r--r--   0 zach       (502) staff       (20)     7860 2023-06-14 03:17:18.000000 thefriendlystars-0.1.0/thefriendlystars/gaia.py
+-rw-r--r--   0 zach       (502) staff       (20)      306 2023-06-14 03:17:18.000000 thefriendlystars-0.1.0/thefriendlystars/imports.py
+-rwxr-xr-x   0 zach       (502) staff       (20)       62 2023-06-14 03:17:18.000000 thefriendlystars-0.1.0/thefriendlystars/version.py
+drwxr-xr-x   0 zach       (502) staff       (20)        0 2023-06-14 03:20:23.840679 thefriendlystars-0.1.0/thefriendlystars.egg-info/
+-rw-r--r--   0 zach       (502) staff       (20)      616 2023-06-14 03:20:23.000000 thefriendlystars-0.1.0/thefriendlystars.egg-info/PKG-INFO
+-rw-r--r--   0 zach       (502) staff       (20)      374 2023-06-14 03:20:23.000000 thefriendlystars-0.1.0/thefriendlystars.egg-info/SOURCES.txt
+-rw-r--r--   0 zach       (502) staff       (20)        1 2023-06-14 03:20:23.000000 thefriendlystars-0.1.0/thefriendlystars.egg-info/dependency_links.txt
+-rw-r--r--   0 zach       (502) staff       (20)        1 2023-06-14 03:19:56.000000 thefriendlystars-0.1.0/thefriendlystars.egg-info/not-zip-safe
+-rw-r--r--   0 zach       (502) staff       (20)      204 2023-06-14 03:20:23.000000 thefriendlystars-0.1.0/thefriendlystars.egg-info/requires.txt
+-rw-r--r--   0 zach       (502) staff       (20)       17 2023-06-14 03:20:23.000000 thefriendlystars-0.1.0/thefriendlystars.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `thefriendlystars-0.0.2/README.md` & `thefriendlystars-0.1.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,31 +1,30 @@
-# the-friendly-stars
-`the-friendly-stars` is a Python toolkit for interacting with catalogs of stars and images of the sky. It can be used to make custom finder charts, as well as do a tiny bit of cross-matching across catalogs.
+# thefriendlystars
+`thefriendlystars` is a Python toolkit for interacting with catalogs of stars and images of the sky. It can be used to make custom finder charts, and it may soon include additional visualizations. Read the (very basic) [documentation](https://zkbt.github.io/thefriendlystars/).
 
-Following [The Friendly Stars](https://play.google.com/books/reader?id=xa8RAAAAYAAJ&printsec=frontcover&output=reader&hl=en&pg=GBS.PP1) by Martha Evans Martin (1925), "the chief aim of this [package] is to share with others the pleasure which the writer has had in what may be called a relation of personal friendship with the stars." It is still a *work in progress*.
+Following [The Friendly Stars](https://books.google.com/books?id=uUYJAAAAIAAJ&printsec=frontcover&source=gbs_ge_summary_r&cad=0#v=onepage&q&f=false) by Martha Evans Martin (1925), "the chief aim of this [package] is to share with others the pleasure which the writer has had in what may be called a relation of personal friendship with the stars." It is still very much so a *work in progress*.
 
-## Usage
+*(If there's any chance you had been using a pre-2023 version of `thefriendlystars`, please note it has moved to [`the-earlier-version-of-the-friendly-stars`](https://github.com/zkbt/the-earlier-version-of-the-friendly-stars). We're starting from scratch here!)*
+
+## Installation
+You should be able to install this simply by running
 
-Please feel free to peruse the few examples of how `thefriendlystars` works in `notebooks/`, as well as the tests in the `tests/`. One simple usage would be to run
 ```
-from thefriendlystars.constellations import Gaia
-g = Gaia.from_cone('GJ1132')
-g.animate('GJ1132-weeeeeeee.gif')
+pip install thefriendlystars
 ```
-to make a finder chart that would work for past, present, and future astronomers.
-
-![example finder chart of GJ1132](images/GJ1132-weeeeeeee.gif)
-
-## Installation
-You should be able to install this simply by running `pip install git+https://github.com/zkbt/the-friendly-stars.git`.
 
 If you want to be able to modify the code yourself, please also feel free to fork/clone this repository onto your own computer and install directly from that editable package. For example, this might look like:
 ```
-git clone https://github.com/zkbt/the-friendly-stars.git
-cd craftroom/
-pip install -e .
+git clone git@github.com:zkbt/thefriendlystars.git
+cd thefriendlystars/
+pip install -e '.[develop]'
 ```
-This will link the installed version of the `thefriendlystars` package to your local repository. Changes you make to the code in the repository should be reflected in the version Python sees when it tries to `import thefriendlystars`.
+This will link the installed version of the `thefriendlystars` package to your local repository. Changes you make to the code in the repository should be reflected in the version Python sees when it tries to `import thefriendlystars`. The `-e` means "we can edit the code in its local director"y; the `.` means "install from this current directory"; and the `[develop]` means "install the development dependencies for testing and documentation".
 
 ## Contributors
 
-This package was written mostly by [Zach Berta-Thompson](https://github.com/zkbt), with contributions from [Luci Ibarra Perez](https://github.com/luib0557).
+Code or conceptual contributions were made by:
+- [Zach Berta-Thompson](https://github.com/zkbt)
+- [Luci Ibarra Perez](https://github.com/luib0557)
+- (maybe you soon!)
+
+The [ESA Gaia mission](https://gea.esac.esa.int/archive/) provides the data that sits at the core of `thefriendlystars`. Any work that makes use of this tiny package should acknowledge the incredible work of the thousands of people who make Gaia possible and cite the Gaia archive.
```

