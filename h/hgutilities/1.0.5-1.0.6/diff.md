# Comparing `tmp/hgutilities-1.0.5.tar.gz` & `tmp/hgutilities-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hgutilities-1.0.5.tar", last modified: Tue Jun  6 10:31:56 2023, max compression
+gzip compressed data, was "hgutilities-1.0.6.tar", last modified: Wed Jun 14 09:11:27 2023, max compression
```

## Comparing `hgutilities-1.0.5.tar` & `hgutilities-1.0.6.tar`

### file list

```diff
@@ -1,228 +1,106 @@
-drwxrwxr-x   0 henry     (1000) henry     (1000)        0 2023-06-06 10:31:56.725046 hgutilities-1.0.5/
-drwxrwxr-x   0 henry     (1000) henry     (1000)        0 2023-06-06 10:31:56.693046 hgutilities-1.0.5/.github/
-drwxrwxr-x   0 henry     (1000) henry     (1000)        0 2023-06-06 10:31:56.697046 hgutilities-1.0.5/.github/workflows/
--rw-rw-r--   0 henry     (1000) henry     (1000)     1084 2023-06-06 07:09:05.000000 hgutilities-1.0.5/.github/workflows/python-publish.yml
--rw-rw-r--   0 henry     (1000) henry     (1000)    35149 2023-06-06 07:09:05.000000 hgutilities-1.0.5/LICENSE.md
--rw-rw-r--   0 henry     (1000) henry     (1000)     7866 2023-06-06 10:31:56.725046 hgutilities-1.0.5/PKG-INFO
--rw-rw-r--   0 henry     (1000) henry     (1000)     7148 2023-06-06 08:09:48.000000 hgutilities-1.0.5/README.md
-drwxrwxr-x   0 henry     (1000) henry     (1000)        0 2023-06-06 10:31:56.697046 hgutilities-1.0.5/hgutilities/
-drwxrwxr-x   0 henry     (1000) henry     (1000)        0 2023-06-06 10:31:56.697046 hgutilities-1.0.5/hgutilities/Documentation/
--rw-rw-r--   0 henry     (1000) henry     (1000)        0 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/Documentation/__init__.py
--rw-rw-r--   0 henry     (1000) henry     (1000)     2483 2023-06-06 10:29:51.000000 hgutilities-1.0.5/hgutilities/Documentation/hgutilities.txt
--rw-rw-r--   0 henry     (1000) henry     (1000)      154 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/__init__.py
-drwxrwxr-x   0 henry     (1000) henry     (1000)        0 2023-06-06 10:31:56.701046 hgutilities-1.0.5/hgutilities/__pycache__/
--rw-rw-r--   0 henry     (1000) henry     (1000)      541 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/__pycache__/TesterProgram2.cpython-310.pyc
--rw-rw-r--   0 henry     (1000) henry     (1000)      730 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/__pycache__/TesterProgram2.cpython-311.pyc
--rw-rw-r--   0 henry     (1000) henry     (1000)      352 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/__pycache__/__init__.cpython-310.pyc
-drwxrwxr-x   0 henry     (1000) henry     (1000)        0 2023-06-06 10:31:56.701046 hgutilities-1.0.5/hgutilities/defaults/
-drwxrwxr-x   0 henry     (1000) henry     (1000)        0 2023-06-06 10:31:56.701046 hgutilities-1.0.5/hgutilities/defaults/Documentation/
--rw-rw-r--   0 henry     (1000) henry     (1000)        0 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/defaults/Documentation/__init__.py
--rw-rw-r--   0 henry     (1000) henry     (1000)      614 2023-06-06 08:19:26.000000 hgutilities-1.0.5/hgutilities/defaults/Documentation/defaults.txt
--rw-rw-r--   0 henry     (1000) henry     (1000)      701 2023-06-06 08:19:23.000000 hgutilities-1.0.5/hgutilities/defaults/Documentation/docs.txt
--rw-rw-r--   0 henry     (1000) henry     (1000)      353 2023-06-06 08:19:42.000000 hgutilities-1.0.5/hgutilities/defaults/Documentation/inherit.txt
--rw-rw-r--   0 henry     (1000) henry     (1000)      608 2023-06-06 08:19:38.000000 hgutilities-1.0.5/hgutilities/defaults/Documentation/loaddefaults.txt
--rw-rw-r--   0 henry     (1000) henry     (1000)      524 2023-06-06 08:19:31.000000 hgutilities-1.0.5/hgutilities/defaults/Documentation/processkwargs.txt
--rw-rw-r--   0 henry     (1000) henry     (1000)      229 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/defaults/__init__.py
-drwxrwxr-x   0 henry     (1000) henry     (1000)        0 2023-06-06 10:31:56.701046 hgutilities-1.0.5/hgutilities/defaults/__pycache__/
--rw-rw-r--   0 henry     (1000) henry     (1000)   154356 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/defaults/__pycache__/DefaultsHelpText.cpython-311.pyc
--rw-rw-r--   0 henry     (1000) henry     (1000)     1923 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/defaults/__pycache__/DoDocs.cpython-310.pyc
--rw-rw-r--   0 henry     (1000) henry     (1000)     3774 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/defaults/__pycache__/Docs.cpython-310.pyc
--rw-rw-r--   0 henry     (1000) henry     (1000)      728 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/defaults/__pycache__/Inherit.cpython-310.pyc
--rw-rw-r--   0 henry     (1000) henry     (1000)     2262 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/defaults/__pycache__/LoadDefaults.cpython-310.pyc
--rw-rw-r--   0 henry     (1000) henry     (1000)     3782 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/defaults/__pycache__/LoadDefaults.cpython-311.pyc
--rw-rw-r--   0 henry     (1000) henry     (1000)     3165 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/defaults/__pycache__/ProcessKwargs.cpython-310.pyc
--rw-rw-r--   0 henry     (1000) henry     (1000)     4611 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/defaults/__pycache__/ProcessKwargs.cpython-311.pyc
--rw-rw-r--   0 henry     (1000) henry     (1000)     1019 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/defaults/__pycache__/SetDocs.cpython-310.pyc
--rw-rw-r--   0 henry     (1000) henry     (1000)      432 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/defaults/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 henry     (1000) henry     (1000)     1065 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/defaults/__pycache__/__init__.cpython-311.pyc
--rw-rw-r--   0 henry     (1000) henry     (1000)     3805 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/defaults/__pycache__/docs.cpython-310.pyc
--rw-rw-r--   0 henry     (1000) henry     (1000)      749 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/defaults/__pycache__/inherit.cpython-310.pyc
--rw-rw-r--   0 henry     (1000) henry     (1000)     2265 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/defaults/__pycache__/loaddefaults.cpython-310.pyc
--rw-rw-r--   0 henry     (1000) henry     (1000)     3186 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/defaults/__pycache__/processkwargs.cpython-310.pyc
--rw-rw-r--   0 henry     (1000) henry     (1000)     2881 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/defaults/docs.py
--rw-rw-r--   0 henry     (1000) henry     (1000)      656 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/defaults/inherit.py
--rw-rw-r--   0 henry     (1000) henry     (1000)     1518 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/defaults/loaddefaults.py
--rw-rw-r--   0 henry     (1000) henry     (1000)     2502 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/defaults/processkwargs.py
-drwxrwxr-x   0 henry     (1000) henry     (1000)        0 2023-06-06 10:31:56.705046 hgutilities-1.0.5/hgutilities/plotting/
-drwxrwxr-x   0 henry     (1000) henry     (1000)        0 2023-06-06 10:31:56.705046 hgutilities-1.0.5/hgutilities/plotting/Default Settings/
--rw-rw-r--   0 henry     (1000) henry     (1000)      181 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/Default Settings/Animate.txt
--rw-rw-r--   0 henry     (1000) henry     (1000)      580 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/Default Settings/Figure.txt
--rw-rw-r--   0 henry     (1000) henry     (1000)      314 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/Default Settings/Figures.txt
--rw-rw-r--   0 henry     (1000) henry     (1000)        0 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/Default Settings/__init__.py
-drwxrwxr-x   0 henry     (1000) henry     (1000)        0 2023-06-06 10:31:56.705046 hgutilities-1.0.5/hgutilities/plotting/Documentation/
--rw-rw-r--   0 henry     (1000) henry     (1000)      581 2023-06-06 08:18:45.000000 hgutilities-1.0.5/hgutilities/plotting/Documentation/Animate.txt
--rw-rw-r--   0 henry     (1000) henry     (1000)      414 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/Documentation/Figure.txt
--rw-rw-r--   0 henry     (1000) henry     (1000)      564 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/Documentation/Figures.txt
--rw-rw-r--   0 henry     (1000) henry     (1000)        0 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/Documentation/__init__.py
--rw-rw-r--   0 henry     (1000) henry     (1000)      791 2023-06-06 08:18:42.000000 hgutilities-1.0.5/hgutilities/plotting/Documentation/create_animations.txt
--rw-rw-r--   0 henry     (1000) henry     (1000)      612 2023-06-06 08:18:39.000000 hgutilities-1.0.5/hgutilities/plotting/Documentation/create_figures.txt
--rw-rw-r--   0 henry     (1000) henry     (1000)     1155 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/Documentation/plotting.txt
--rw-rw-r--   0 henry     (1000) henry     (1000)    10839 2023-06-06 08:05:19.000000 hgutilities-1.0.5/hgutilities/plotting/README.md
--rw-rw-r--   0 henry     (1000) henry     (1000)     1098 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/__init__.py
-drwxrwxr-x   0 henry     (1000) henry     (1000)        0 2023-06-06 10:31:56.709046 hgutilities-1.0.5/hgutilities/plotting/__pycache__/
--rw-rw-r--   0 henry     (1000) henry     (1000)     3616 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/__pycache__/Animate.cpython-310.pyc
--rw-rw-r--   0 henry     (1000) henry     (1000)     5849 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/__pycache__/Animate.cpython-311.pyc
--rw-rw-r--   0 henry     (1000) henry     (1000)     7105 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/__pycache__/Figure.cpython-310.pyc
--rw-rw-r--   0 henry     (1000) henry     (1000)    12637 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/__pycache__/Figure.cpython-311.pyc
--rw-rw-r--   0 henry     (1000) henry     (1000)     3492 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/__pycache__/Figures.cpython-310.pyc
--rw-rw-r--   0 henry     (1000) henry     (1000)     4308 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/__pycache__/Figures.cpython-311.pyc
--rw-rw-r--   0 henry     (1000) henry     (1000)      584 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/__pycache__/Line.cpython-310.pyc
--rw-rw-r--   0 henry     (1000) henry     (1000)      795 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/__pycache__/Line.cpython-311.pyc
--rw-rw-r--   0 henry     (1000) henry     (1000)      970 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/__pycache__/Line.cpython-38.pyc
--rw-rw-r--   0 henry     (1000) henry     (1000)     1245 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/__pycache__/Lines.cpython-310.pyc
--rw-rw-r--   0 henry     (1000) henry     (1000)     2083 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/__pycache__/Lines.cpython-311.pyc
--rw-rw-r--   0 henry     (1000) henry     (1000)     2773 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/__pycache__/Lines.cpython-38.pyc
--rw-rw-r--   0 henry     (1000) henry     (1000)     6113 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/__pycache__/Plot.cpython-310.pyc
--rw-rw-r--   0 henry     (1000) henry     (1000)    10132 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/__pycache__/Plot.cpython-311.pyc
--rw-rw-r--   0 henry     (1000) henry     (1000)    11426 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/__pycache__/Plot.cpython-38.pyc
--rw-rw-r--   0 henry     (1000) henry     (1000)    11376 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/__pycache__/PlotAxes.cpython-311.pyc
--rw-rw-r--   0 henry     (1000) henry     (1000)     7542 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/__pycache__/PlotAxes.cpython-38.pyc
--rw-rw-r--   0 henry     (1000) henry     (1000)      519 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/__pycache__/PlotFunctions.cpython-310.pyc
--rw-rw-r--   0 henry     (1000) henry     (1000)      822 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/__pycache__/PlotFunctions.cpython-311.pyc
--rw-rw-r--   0 henry     (1000) henry     (1000)     5102 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/__pycache__/PlotShape.cpython-310.pyc
--rw-rw-r--   0 henry     (1000) henry     (1000)     8252 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/__pycache__/PlotShape.cpython-311.pyc
--rw-rw-r--   0 henry     (1000) henry     (1000)     5135 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/__pycache__/PlotShape.cpython-38.pyc
--rw-rw-r--   0 henry     (1000) henry     (1000)     4366 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/__pycache__/PlotUtils.cpython-311.pyc
--rw-rw-r--   0 henry     (1000) henry     (1000)     4172 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/__pycache__/PlotUtils.cpython-38.pyc
--rw-rw-r--   0 henry     (1000) henry     (1000)     2928 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/__pycache__/Plots.cpython-310.pyc
--rw-rw-r--   0 henry     (1000) henry     (1000)     4497 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/__pycache__/Plots.cpython-311.pyc
--rw-rw-r--   0 henry     (1000) henry     (1000)     3439 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/__pycache__/Plots.cpython-38.pyc
--rw-rw-r--   0 henry     (1000) henry     (1000)     1121 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 henry     (1000) henry     (1000)     1990 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/__pycache__/__init__.cpython-311.pyc
--rw-rw-r--   0 henry     (1000) henry     (1000)     3641 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/__pycache__/animate.cpython-310.pyc
--rw-rw-r--   0 henry     (1000) henry     (1000)     7154 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/__pycache__/figure.cpython-310.pyc
--rw-rw-r--   0 henry     (1000) henry     (1000)     3548 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/__pycache__/figures.cpython-310.pyc
--rw-rw-r--   0 henry     (1000) henry     (1000)      558 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/__pycache__/plotfunctions.cpython-310.pyc
--rw-rw-r--   0 henry     (1000) henry     (1000)     2595 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/animate.py
-drwxrwxr-x   0 henry     (1000) henry     (1000)        0 2023-06-06 10:31:56.713046 hgutilities-1.0.5/hgutilities/plotting/datatypes/
-drwxrwxr-x   0 henry     (1000) henry     (1000)        0 2023-06-06 10:31:56.713046 hgutilities-1.0.5/hgutilities/plotting/datatypes/Default Settings/
--rw-rw-r--   0 henry     (1000) henry     (1000)      267 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/datatypes/Default Settings/Bar.txt
--rw-rw-r--   0 henry     (1000) henry     (1000)      173 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/datatypes/Default Settings/Bars.txt
--rw-rw-r--   0 henry     (1000) henry     (1000)      699 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/datatypes/Default Settings/Colorplot.txt
--rw-rw-r--   0 henry     (1000) henry     (1000)      421 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/datatypes/Default Settings/Data.txt
--rw-rw-r--   0 henry     (1000) henry     (1000)     1081 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/datatypes/Default Settings/Line.txt
--rw-rw-r--   0 henry     (1000) henry     (1000)      180 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/datatypes/Default Settings/Lines.txt
--rw-rw-r--   0 henry     (1000) henry     (1000)      334 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/datatypes/Default Settings/Pie.txt
--rw-rw-r--   0 henry     (1000) henry     (1000)      553 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/datatypes/Default Settings/Surface.txt
--rw-rw-r--   0 henry     (1000) henry     (1000)        0 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/datatypes/Default Settings/__init__.py
-drwxrwxr-x   0 henry     (1000) henry     (1000)        0 2023-06-06 10:31:56.713046 hgutilities-1.0.5/hgutilities/plotting/datatypes/Documentation/
--rw-rw-r--   0 henry     (1000) henry     (1000)      664 2023-06-06 08:18:34.000000 hgutilities-1.0.5/hgutilities/plotting/datatypes/Documentation/Bar.txt
--rw-rw-r--   0 henry     (1000) henry     (1000)      869 2023-06-06 08:18:26.000000 hgutilities-1.0.5/hgutilities/plotting/datatypes/Documentation/Bars.txt
--rw-rw-r--   0 henry     (1000) henry     (1000)      365 2023-06-06 08:18:23.000000 hgutilities-1.0.5/hgutilities/plotting/datatypes/Documentation/Colormap.txt
--rw-rw-r--   0 henry     (1000) henry     (1000)      762 2023-06-06 08:18:19.000000 hgutilities-1.0.5/hgutilities/plotting/datatypes/Documentation/Data.txt
--rw-rw-r--   0 henry     (1000) henry     (1000)      659 2023-06-06 08:18:14.000000 hgutilities-1.0.5/hgutilities/plotting/datatypes/Documentation/Line.txt
--rw-rw-r--   0 henry     (1000) henry     (1000)     1210 2023-06-06 08:18:11.000000 hgutilities-1.0.5/hgutilities/plotting/datatypes/Documentation/Lines.txt
--rw-rw-r--   0 henry     (1000) henry     (1000)      656 2023-06-06 08:18:07.000000 hgutilities-1.0.5/hgutilities/plotting/datatypes/Documentation/Pie.txt
--rw-rw-r--   0 henry     (1000) henry     (1000)      859 2023-06-06 08:18:04.000000 hgutilities-1.0.5/hgutilities/plotting/datatypes/Documentation/Surface.txt
--rw-rw-r--   0 henry     (1000) henry     (1000)        0 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/datatypes/Documentation/__init__.py
--rw-rw-r--   0 henry     (1000) henry     (1000)        0 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/datatypes/__init__.py
-drwxrwxr-x   0 henry     (1000) henry     (1000)        0 2023-06-06 10:31:56.717046 hgutilities-1.0.5/hgutilities/plotting/datatypes/__pycache__/
--rw-rw-r--   0 henry     (1000) henry     (1000)      541 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/datatypes/__pycache__/Bar.cpython-310.pyc
--rw-rw-r--   0 henry     (1000) henry     (1000)      883 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/datatypes/__pycache__/Bar.cpython-311.pyc
--rw-rw-r--   0 henry     (1000) henry     (1000)     1552 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/datatypes/__pycache__/Bars.cpython-310.pyc
--rw-rw-r--   0 henry     (1000) henry     (1000)      886 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/datatypes/__pycache__/Bars.cpython-311.pyc
--rw-rw-r--   0 henry     (1000) henry     (1000)      855 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/datatypes/__pycache__/Colormap.cpython-310.pyc
--rw-rw-r--   0 henry     (1000) henry     (1000)      898 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/datatypes/__pycache__/Colormap.cpython-311.pyc
--rw-rw-r--   0 henry     (1000) henry     (1000)     1273 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/datatypes/__pycache__/Colorplot.cpython-310.pyc
--rw-rw-r--   0 henry     (1000) henry     (1000)      691 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/datatypes/__pycache__/Data.cpython-310.pyc
--rw-rw-r--   0 henry     (1000) henry     (1000)      966 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/datatypes/__pycache__/Data.cpython-311.pyc
--rw-rw-r--   0 henry     (1000) henry     (1000)      550 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/datatypes/__pycache__/Line.cpython-310.pyc
--rw-rw-r--   0 henry     (1000) henry     (1000)      785 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/datatypes/__pycache__/Line.cpython-311.pyc
--rw-rw-r--   0 henry     (1000) henry     (1000)     2248 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/datatypes/__pycache__/Lines.cpython-310.pyc
--rw-rw-r--   0 henry     (1000) henry     (1000)     2215 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/datatypes/__pycache__/Lines.cpython-311.pyc
--rw-rw-r--   0 henry     (1000) henry     (1000)      782 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/datatypes/__pycache__/Pie.cpython-310.pyc
--rw-rw-r--   0 henry     (1000) henry     (1000)      883 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/datatypes/__pycache__/Pie.cpython-311.pyc
--rw-rw-r--   0 henry     (1000) henry     (1000)     1626 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/datatypes/__pycache__/Surface.cpython-310.pyc
--rw-rw-r--   0 henry     (1000) henry     (1000)     2413 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/datatypes/__pycache__/Surface.cpython-311.pyc
--rw-rw-r--   0 henry     (1000) henry     (1000)      565 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/datatypes/__pycache__/bar.cpython-310.pyc
--rw-rw-r--   0 henry     (1000) henry     (1000)     1548 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/datatypes/__pycache__/bars.cpython-310.pyc
--rw-rw-r--   0 henry     (1000) henry     (1000)     1288 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/datatypes/__pycache__/colorplot.cpython-310.pyc
--rw-rw-r--   0 henry     (1000) henry     (1000)      715 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/datatypes/__pycache__/data.cpython-310.pyc
--rw-rw-r--   0 henry     (1000) henry     (1000)      574 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/datatypes/__pycache__/line.cpython-310.pyc
--rw-rw-r--   0 henry     (1000) henry     (1000)     2244 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/datatypes/__pycache__/lines.cpython-310.pyc
--rw-rw-r--   0 henry     (1000) henry     (1000)      797 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/datatypes/__pycache__/pie.cpython-310.pyc
--rw-rw-r--   0 henry     (1000) henry     (1000)     1641 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/datatypes/__pycache__/surface.cpython-310.pyc
--rw-rw-r--   0 henry     (1000) henry     (1000)      219 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/datatypes/bar.py
--rw-rw-r--   0 henry     (1000) henry     (1000)      992 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/datatypes/bars.py
--rw-rw-r--   0 henry     (1000) henry     (1000)      845 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/datatypes/colorplot.py
--rw-rw-r--   0 henry     (1000) henry     (1000)      244 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/datatypes/data.py
--rw-rw-r--   0 henry     (1000) henry     (1000)      222 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/datatypes/line.py
--rw-rw-r--   0 henry     (1000) henry     (1000)     1630 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/datatypes/lines.py
--rw-rw-r--   0 henry     (1000) henry     (1000)      370 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/datatypes/pie.py
--rw-rw-r--   0 henry     (1000) henry     (1000)      979 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/datatypes/surface.py
--rw-rw-r--   0 henry     (1000) henry     (1000)     5255 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/figure.py
--rw-rw-r--   0 henry     (1000) henry     (1000)     2538 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/figures.py
--rw-rw-r--   0 henry     (1000) henry     (1000)      386 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/plotfunctions.py
-drwxrwxr-x   0 henry     (1000) henry     (1000)        0 2023-06-06 10:31:56.721046 hgutilities-1.0.5/hgutilities/plotting/plottypes/
-drwxrwxr-x   0 henry     (1000) henry     (1000)        0 2023-06-06 10:31:56.721046 hgutilities-1.0.5/hgutilities/plotting/plottypes/Documentation/
--rw-rw-r--   0 henry     (1000) henry     (1000)      497 2023-06-06 08:18:00.000000 hgutilities-1.0.5/hgutilities/plotting/plottypes/Documentation/Plot.txt
--rw-rw-r--   0 henry     (1000) henry     (1000)        0 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/plottypes/Documentation/__init__.py
--rw-rw-r--   0 henry     (1000) henry     (1000)        0 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/plottypes/__init__.py
-drwxrwxr-x   0 henry     (1000) henry     (1000)        0 2023-06-06 10:31:56.721046 hgutilities-1.0.5/hgutilities/plotting/plottypes/__pycache__/
--rw-rw-r--   0 henry     (1000) henry     (1000)     3690 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/plottypes/__pycache__/Plot.cpython-310.pyc
--rw-rw-r--   0 henry     (1000) henry     (1000)     1879 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/plottypes/__pycache__/Plot.cpython-311.pyc
--rw-rw-r--   0 henry     (1000) henry     (1000)     3777 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/plottypes/__pycache__/PlotBars.cpython-310.pyc
--rw-rw-r--   0 henry     (1000) henry     (1000)     1327 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/plottypes/__pycache__/PlotBars.cpython-311.pyc
--rw-rw-r--   0 henry     (1000) henry     (1000)     1135 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/plottypes/__pycache__/PlotColormap.cpython-310.pyc
--rw-rw-r--   0 henry     (1000) henry     (1000)     1350 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/plottypes/__pycache__/PlotColormap.cpython-311.pyc
--rw-rw-r--   0 henry     (1000) henry     (1000)     2003 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/plottypes/__pycache__/PlotColorplot.cpython-310.pyc
--rw-rw-r--   0 henry     (1000) henry     (1000)     4552 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/plottypes/__pycache__/PlotLines.cpython-310.pyc
--rw-rw-r--   0 henry     (1000) henry     (1000)     7970 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/plottypes/__pycache__/PlotLines.cpython-311.pyc
--rw-rw-r--   0 henry     (1000) henry     (1000)     1350 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/plottypes/__pycache__/PlotPie.cpython-310.pyc
--rw-rw-r--   0 henry     (1000) henry     (1000)     1322 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/plottypes/__pycache__/PlotPie.cpython-311.pyc
--rw-rw-r--   0 henry     (1000) henry     (1000)     3219 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/plottypes/__pycache__/PlotSurface.cpython-310.pyc
--rw-rw-r--   0 henry     (1000) henry     (1000)     3141 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/plottypes/__pycache__/PlotSurface.cpython-311.pyc
--rw-rw-r--   0 henry     (1000) henry     (1000)     3657 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/plottypes/__pycache__/plot.cpython-310.pyc
--rw-rw-r--   0 henry     (1000) henry     (1000)     3788 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/plottypes/__pycache__/plotbars.cpython-310.pyc
--rw-rw-r--   0 henry     (1000) henry     (1000)     2014 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/plottypes/__pycache__/plotcolorplot.cpython-310.pyc
--rw-rw-r--   0 henry     (1000) henry     (1000)     4573 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/plottypes/__pycache__/plotlines.cpython-310.pyc
--rw-rw-r--   0 henry     (1000) henry     (1000)     1361 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/plottypes/__pycache__/plotpie.cpython-310.pyc
--rw-rw-r--   0 henry     (1000) henry     (1000)     3230 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/plottypes/__pycache__/plotsurface.cpython-310.pyc
--rw-rw-r--   0 henry     (1000) henry     (1000)     3209 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/plottypes/plot.py
--rw-rw-r--   0 henry     (1000) henry     (1000)     3354 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/plottypes/plotbars.py
--rw-rw-r--   0 henry     (1000) henry     (1000)     2613 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/plottypes/plotcolorplot.py
--rw-rw-r--   0 henry     (1000) henry     (1000)     6683 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/plottypes/plotlines.py
--rw-rw-r--   0 henry     (1000) henry     (1000)     1249 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/plottypes/plotpie.py
--rw-rw-r--   0 henry     (1000) henry     (1000)     3691 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/plottypes/plotsurface.py
-drwxrwxr-x   0 henry     (1000) henry     (1000)        0 2023-06-06 10:31:56.721046 hgutilities-1.0.5/hgutilities/plotting/plotutils/
--rw-rw-r--   0 henry     (1000) henry     (1000)        0 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/plotutils/__init__.py
-drwxrwxr-x   0 henry     (1000) henry     (1000)        0 2023-06-06 10:31:56.725046 hgutilities-1.0.5/hgutilities/plotting/plotutils/__pycache__/
--rw-rw-r--   0 henry     (1000) henry     (1000)     1138 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/plotutils/__pycache__/FigureSize.cpython-310.pyc
--rw-rw-r--   0 henry     (1000) henry     (1000)     1838 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/plotutils/__pycache__/FigureSize.cpython-311.pyc
--rw-rw-r--   0 henry     (1000) henry     (1000)     5357 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/plotutils/__pycache__/GridDimensions.cpython-310.pyc
--rw-rw-r--   0 henry     (1000) henry     (1000)     8558 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/plotutils/__pycache__/GridDimensions.cpython-311.pyc
--rw-rw-r--   0 henry     (1000) henry     (1000)     5262 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/plotutils/__pycache__/PlotShape.cpython-310.pyc
--rw-rw-r--   0 henry     (1000) henry     (1000)     1453 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/plotutils/__pycache__/SaveFigure.cpython-310.pyc
--rw-rw-r--   0 henry     (1000) henry     (1000)     2325 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/plotutils/__pycache__/SaveFigure.cpython-311.pyc
--rw-rw-r--   0 henry     (1000) henry     (1000)     1159 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/plotutils/__pycache__/figuresize.cpython-310.pyc
--rw-rw-r--   0 henry     (1000) henry     (1000)     5378 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/plotutils/__pycache__/griddimensions.cpython-310.pyc
--rw-rw-r--   0 henry     (1000) henry     (1000)     1474 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/plotutils/__pycache__/savefigure.cpython-310.pyc
--rw-rw-r--   0 henry     (1000) henry     (1000)      690 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/plotutils/figuresize.py
--rw-rw-r--   0 henry     (1000) henry     (1000)     4445 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/plotutils/griddimensions.py
--rw-rw-r--   0 henry     (1000) henry     (1000)     4425 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/plotutils/plotshape.py
--rw-rw-r--   0 henry     (1000) henry     (1000)     1287 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/plotting/plotutils/savefigure.py
-drwxrwxr-x   0 henry     (1000) henry     (1000)        0 2023-06-06 10:31:56.725046 hgutilities-1.0.5/hgutilities/utils/
--rw-rw-r--   0 henry     (1000) henry     (1000)        0 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/utils/__init__.py
-drwxrwxr-x   0 henry     (1000) henry     (1000)        0 2023-06-06 10:31:56.725046 hgutilities-1.0.5/hgutilities/utils/__pycache__/
--rw-rw-r--   0 henry     (1000) henry     (1000)      474 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/utils/__pycache__/Dicts.cpython-310.pyc
--rw-rw-r--   0 henry     (1000) henry     (1000)     1546 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/utils/__pycache__/Groups.cpython-310.pyc
--rw-rw-r--   0 henry     (1000) henry     (1000)     2364 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/utils/__pycache__/Groups.cpython-311.pyc
--rw-rw-r--   0 henry     (1000) henry     (1000)     1385 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/utils/__pycache__/Paths.cpython-310.pyc
--rw-rw-r--   0 henry     (1000) henry     (1000)     2695 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/utils/__pycache__/Paths.cpython-311.pyc
--rw-rw-r--   0 henry     (1000) henry     (1000)      311 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/utils/__pycache__/Strings.cpython-310.pyc
--rw-rw-r--   0 henry     (1000) henry     (1000)      168 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/utils/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 henry     (1000) henry     (1000)      495 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/utils/__pycache__/dicts.cpython-310.pyc
--rw-rw-r--   0 henry     (1000) henry     (1000)     1567 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/utils/__pycache__/groups.cpython-310.pyc
--rw-rw-r--   0 henry     (1000) henry     (1000)     1406 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/utils/__pycache__/paths.cpython-310.pyc
--rw-rw-r--   0 henry     (1000) henry     (1000)      191 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/utils/dicts.py
--rw-rw-r--   0 henry     (1000) henry     (1000)     1419 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/utils/groups.py
--rw-rw-r--   0 henry     (1000) henry     (1000)      927 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/utils/paths.py
--rw-rw-r--   0 henry     (1000) henry     (1000)      668 2023-06-06 07:09:05.000000 hgutilities-1.0.5/hgutilities/utils/plots.py
-drwxrwxr-x   0 henry     (1000) henry     (1000)        0 2023-06-06 10:31:56.697046 hgutilities-1.0.5/hgutilities.egg-info/
--rw-rw-r--   0 henry     (1000) henry     (1000)     7866 2023-06-06 10:31:56.000000 hgutilities-1.0.5/hgutilities.egg-info/PKG-INFO
--rw-rw-r--   0 henry     (1000) henry     (1000)    10801 2023-06-06 10:31:56.000000 hgutilities-1.0.5/hgutilities.egg-info/SOURCES.txt
--rw-rw-r--   0 henry     (1000) henry     (1000)        1 2023-06-06 10:31:56.000000 hgutilities-1.0.5/hgutilities.egg-info/dependency_links.txt
--rw-rw-r--   0 henry     (1000) henry     (1000)       35 2023-06-06 10:31:56.000000 hgutilities-1.0.5/hgutilities.egg-info/requires.txt
--rw-rw-r--   0 henry     (1000) henry     (1000)        1 2023-06-06 10:31:56.000000 hgutilities-1.0.5/hgutilities.egg-info/top_level.txt
--rw-rw-r--   0 henry     (1000) henry     (1000)       38 2023-06-06 10:31:56.725046 hgutilities-1.0.5/setup.cfg
--rw-rw-r--   0 henry     (1000) henry     (1000)     1453 2023-06-06 10:28:34.000000 hgutilities-1.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-14 09:11:27.709352 hgutilities-1.0.6/
+drwxrwxrwx   0        0        0        0 2023-06-14 09:11:27.581107 hgutilities-1.0.6/.github/
+drwxrwxrwx   0        0        0        0 2023-06-14 09:11:27.592109 hgutilities-1.0.6/.github/workflows/
+-rw-rw-rw-   0        0        0     1123 2023-06-14 09:06:29.000000 hgutilities-1.0.6/.github/workflows/python-publish.yml
+-rw-rw-rw-   0        0        0    35823 2023-06-14 09:06:29.000000 hgutilities-1.0.6/LICENSE.md
+-rw-rw-rw-   0        0        0     7982 2023-06-14 09:11:27.709352 hgutilities-1.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     7224 2023-06-14 09:06:29.000000 hgutilities-1.0.6/README.md
+drwxrwxrwx   0        0        0        0 2023-06-14 09:11:27.593108 hgutilities-1.0.6/hgutilities/
+drwxrwxrwx   0        0        0        0 2023-06-14 09:11:27.609334 hgutilities-1.0.6/hgutilities/Documentation/
+-rw-rw-rw-   0        0        0        0 2023-06-14 09:06:29.000000 hgutilities-1.0.6/hgutilities/Documentation/__init__.py
+-rw-rw-rw-   0        0        0     2505 2023-06-14 09:06:29.000000 hgutilities-1.0.6/hgutilities/Documentation/hgutilities.txt
+-rw-rw-rw-   0        0        0      163 2023-06-14 09:06:29.000000 hgutilities-1.0.6/hgutilities/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-14 09:11:27.612334 hgutilities-1.0.6/hgutilities/defaults/
+drwxrwxrwx   0        0        0        0 2023-06-14 09:11:27.623333 hgutilities-1.0.6/hgutilities/defaults/Documentation/
+-rw-rw-rw-   0        0        0        0 2023-06-14 09:06:29.000000 hgutilities-1.0.6/hgutilities/defaults/Documentation/__init__.py
+-rw-rw-rw-   0        0        0      633 2023-06-14 09:06:29.000000 hgutilities-1.0.6/hgutilities/defaults/Documentation/defaults.txt
+-rw-rw-rw-   0        0        0      715 2023-06-14 09:06:29.000000 hgutilities-1.0.6/hgutilities/defaults/Documentation/docs.txt
+-rw-rw-rw-   0        0        0      361 2023-06-14 09:06:29.000000 hgutilities-1.0.6/hgutilities/defaults/Documentation/inherit.txt
+-rw-rw-rw-   0        0        0      625 2023-06-14 09:06:29.000000 hgutilities-1.0.6/hgutilities/defaults/Documentation/loaddefaults.txt
+-rw-rw-rw-   0        0        0      537 2023-06-14 09:06:29.000000 hgutilities-1.0.6/hgutilities/defaults/Documentation/processkwargs.txt
+-rw-rw-rw-   0        0        0      239 2023-06-14 09:06:29.000000 hgutilities-1.0.6/hgutilities/defaults/__init__.py
+-rw-rw-rw-   0        0        0     2962 2023-06-14 09:06:29.000000 hgutilities-1.0.6/hgutilities/defaults/docs.py
+-rw-rw-rw-   0        0        0      671 2023-06-14 09:06:29.000000 hgutilities-1.0.6/hgutilities/defaults/inherit.py
+-rw-rw-rw-   0        0        0     1562 2023-06-14 09:06:29.000000 hgutilities-1.0.6/hgutilities/defaults/loaddefaults.py
+-rw-rw-rw-   0        0        0     2571 2023-06-14 09:06:29.000000 hgutilities-1.0.6/hgutilities/defaults/processkwargs.py
+drwxrwxrwx   0        0        0        0 2023-06-14 09:11:27.630146 hgutilities-1.0.6/hgutilities/plotting/
+drwxrwxrwx   0        0        0        0 2023-06-14 09:11:27.636146 hgutilities-1.0.6/hgutilities/plotting/Default Settings/
+-rw-rw-rw-   0        0        0      193 2023-06-14 09:06:29.000000 hgutilities-1.0.6/hgutilities/plotting/Default Settings/Animate.txt
+-rw-rw-rw-   0        0        0      608 2023-06-14 09:06:29.000000 hgutilities-1.0.6/hgutilities/plotting/Default Settings/Figure.txt
+-rw-rw-rw-   0        0        0      330 2023-06-14 09:06:29.000000 hgutilities-1.0.6/hgutilities/plotting/Default Settings/Figures.txt
+-rw-rw-rw-   0        0        0        0 2023-06-14 09:06:29.000000 hgutilities-1.0.6/hgutilities/plotting/Default Settings/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-14 09:11:27.652907 hgutilities-1.0.6/hgutilities/plotting/Documentation/
+-rw-rw-rw-   0        0        0      598 2023-06-14 09:06:29.000000 hgutilities-1.0.6/hgutilities/plotting/Documentation/Animate.txt
+-rw-rw-rw-   0        0        0      424 2023-06-14 09:06:29.000000 hgutilities-1.0.6/hgutilities/plotting/Documentation/Figure.txt
+-rw-rw-rw-   0        0        0      579 2023-06-14 09:06:29.000000 hgutilities-1.0.6/hgutilities/plotting/Documentation/Figures.txt
+-rw-rw-rw-   0        0        0        0 2023-06-14 09:06:29.000000 hgutilities-1.0.6/hgutilities/plotting/Documentation/__init__.py
+-rw-rw-rw-   0        0        0      811 2023-06-14 09:06:29.000000 hgutilities-1.0.6/hgutilities/plotting/Documentation/create_animations.txt
+-rw-rw-rw-   0        0        0      628 2023-06-14 09:06:29.000000 hgutilities-1.0.6/hgutilities/plotting/Documentation/create_figures.txt
+-rw-rw-rw-   0        0        0     1180 2023-06-14 09:06:29.000000 hgutilities-1.0.6/hgutilities/plotting/Documentation/plotting.txt
+-rw-rw-rw-   0        0        0    11039 2023-06-14 09:06:29.000000 hgutilities-1.0.6/hgutilities/plotting/README.md
+-rw-rw-rw-   0        0        0     1132 2023-06-14 09:06:29.000000 hgutilities-1.0.6/hgutilities/plotting/__init__.py
+-rw-rw-rw-   0        0        0     2673 2023-06-14 09:06:29.000000 hgutilities-1.0.6/hgutilities/plotting/animate.py
+drwxrwxrwx   0        0        0        0 2023-06-14 09:11:27.655905 hgutilities-1.0.6/hgutilities/plotting/datatypes/
+drwxrwxrwx   0        0        0        0 2023-06-14 09:11:27.674744 hgutilities-1.0.6/hgutilities/plotting/datatypes/Default Settings/
+-rw-rw-rw-   0        0        0      283 2023-06-14 09:06:29.000000 hgutilities-1.0.6/hgutilities/plotting/datatypes/Default Settings/Bar.txt
+-rw-rw-rw-   0        0        0      183 2023-06-14 09:06:29.000000 hgutilities-1.0.6/hgutilities/plotting/datatypes/Default Settings/Bars.txt
+-rw-rw-rw-   0        0        0      738 2023-06-14 09:06:29.000000 hgutilities-1.0.6/hgutilities/plotting/datatypes/Default Settings/Colorplot.txt
+-rw-rw-rw-   0        0        0      441 2023-06-14 09:06:29.000000 hgutilities-1.0.6/hgutilities/plotting/datatypes/Default Settings/Data.txt
+-rw-rw-rw-   0        0        0     1135 2023-06-14 09:06:29.000000 hgutilities-1.0.6/hgutilities/plotting/datatypes/Default Settings/Line.txt
+-rw-rw-rw-   0        0        0      191 2023-06-14 09:06:29.000000 hgutilities-1.0.6/hgutilities/plotting/datatypes/Default Settings/Lines.txt
+-rw-rw-rw-   0        0        0      355 2023-06-14 09:06:29.000000 hgutilities-1.0.6/hgutilities/plotting/datatypes/Default Settings/Pie.txt
+-rw-rw-rw-   0        0        0      582 2023-06-14 09:06:29.000000 hgutilities-1.0.6/hgutilities/plotting/datatypes/Default Settings/Surface.txt
+-rw-rw-rw-   0        0        0        0 2023-06-14 09:06:29.000000 hgutilities-1.0.6/hgutilities/plotting/datatypes/Default Settings/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-14 09:11:27.697356 hgutilities-1.0.6/hgutilities/plotting/datatypes/Documentation/
+-rw-rw-rw-   0        0        0      677 2023-06-14 09:06:29.000000 hgutilities-1.0.6/hgutilities/plotting/datatypes/Documentation/Bar.txt
+-rw-rw-rw-   0        0        0      887 2023-06-14 09:06:29.000000 hgutilities-1.0.6/hgutilities/plotting/datatypes/Documentation/Bars.txt
+-rw-rw-rw-   0        0        0      374 2023-06-14 09:06:29.000000 hgutilities-1.0.6/hgutilities/plotting/datatypes/Documentation/Colormap.txt
+-rw-rw-rw-   0        0        0      782 2023-06-14 09:06:29.000000 hgutilities-1.0.6/hgutilities/plotting/datatypes/Documentation/Data.txt
+-rw-rw-rw-   0        0        0      674 2023-06-14 09:06:29.000000 hgutilities-1.0.6/hgutilities/plotting/datatypes/Documentation/Line.txt
+-rw-rw-rw-   0        0        0     1232 2023-06-14 09:06:29.000000 hgutilities-1.0.6/hgutilities/plotting/datatypes/Documentation/Lines.txt
+-rw-rw-rw-   0        0        0      670 2023-06-14 09:06:29.000000 hgutilities-1.0.6/hgutilities/plotting/datatypes/Documentation/Pie.txt
+-rw-rw-rw-   0        0        0      872 2023-06-14 09:06:29.000000 hgutilities-1.0.6/hgutilities/plotting/datatypes/Documentation/Surface.txt
+-rw-rw-rw-   0        0        0        0 2023-06-14 09:06:29.000000 hgutilities-1.0.6/hgutilities/plotting/datatypes/Documentation/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-06-14 09:06:29.000000 hgutilities-1.0.6/hgutilities/plotting/datatypes/__init__.py
+-rw-rw-rw-   0        0        0      229 2023-06-14 09:06:29.000000 hgutilities-1.0.6/hgutilities/plotting/datatypes/bar.py
+-rw-rw-rw-   0        0        0     1025 2023-06-14 09:06:29.000000 hgutilities-1.0.6/hgutilities/plotting/datatypes/bars.py
+-rw-rw-rw-   0        0        0      872 2023-06-14 09:06:29.000000 hgutilities-1.0.6/hgutilities/plotting/datatypes/colorplot.py
+-rw-rw-rw-   0        0        0      255 2023-06-14 09:06:29.000000 hgutilities-1.0.6/hgutilities/plotting/datatypes/data.py
+-rw-rw-rw-   0        0        0      232 2023-06-14 09:06:29.000000 hgutilities-1.0.6/hgutilities/plotting/datatypes/line.py
+-rw-rw-rw-   0        0        0     1677 2023-06-14 09:06:29.000000 hgutilities-1.0.6/hgutilities/plotting/datatypes/lines.py
+-rw-rw-rw-   0        0        0      387 2023-06-14 09:06:29.000000 hgutilities-1.0.6/hgutilities/plotting/datatypes/pie.py
+-rw-rw-rw-   0        0        0     1014 2023-06-14 09:06:29.000000 hgutilities-1.0.6/hgutilities/plotting/datatypes/surface.py
+-rw-rw-rw-   0        0        0     5536 2023-06-14 09:00:42.000000 hgutilities-1.0.6/hgutilities/plotting/figure.py
+-rw-rw-rw-   0        0        0     2609 2023-06-14 09:06:29.000000 hgutilities-1.0.6/hgutilities/plotting/figures.py
+-rw-rw-rw-   0        0        0      398 2023-06-14 09:06:29.000000 hgutilities-1.0.6/hgutilities/plotting/plotfunctions.py
+drwxrwxrwx   0        0        0        0 2023-06-14 09:11:27.700353 hgutilities-1.0.6/hgutilities/plotting/plottypes/
+drwxrwxrwx   0        0        0        0 2023-06-14 09:11:27.701352 hgutilities-1.0.6/hgutilities/plotting/plottypes/Documentation/
+-rw-rw-rw-   0        0        0      508 2023-06-14 09:06:29.000000 hgutilities-1.0.6/hgutilities/plotting/plottypes/Documentation/Plot.txt
+-rw-rw-rw-   0        0        0        0 2023-06-14 09:06:29.000000 hgutilities-1.0.6/hgutilities/plotting/plottypes/Documentation/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-06-14 09:06:29.000000 hgutilities-1.0.6/hgutilities/plotting/plottypes/__init__.py
+-rw-rw-rw-   0        0        0     3301 2023-06-14 09:06:29.000000 hgutilities-1.0.6/hgutilities/plotting/plottypes/plot.py
+-rw-rw-rw-   0        0        0     3444 2023-06-14 09:06:29.000000 hgutilities-1.0.6/hgutilities/plotting/plottypes/plotbars.py
+-rw-rw-rw-   0        0        0     2671 2023-06-14 09:06:29.000000 hgutilities-1.0.6/hgutilities/plotting/plottypes/plotcolorplot.py
+-rw-rw-rw-   0        0        0     6829 2023-06-14 09:06:29.000000 hgutilities-1.0.6/hgutilities/plotting/plottypes/plotlines.py
+-rw-rw-rw-   0        0        0     1284 2023-06-14 09:06:29.000000 hgutilities-1.0.6/hgutilities/plotting/plottypes/plotpie.py
+-rw-rw-rw-   0        0        0     3786 2023-06-14 09:06:29.000000 hgutilities-1.0.6/hgutilities/plotting/plottypes/plotsurface.py
+drwxrwxrwx   0        0        0        0 2023-06-14 09:11:27.706352 hgutilities-1.0.6/hgutilities/plotting/plotutils/
+-rw-rw-rw-   0        0        0        0 2023-06-14 09:06:29.000000 hgutilities-1.0.6/hgutilities/plotting/plotutils/__init__.py
+-rw-rw-rw-   0        0        0      719 2023-06-14 09:00:40.000000 hgutilities-1.0.6/hgutilities/plotting/plotutils/figuresize.py
+-rw-rw-rw-   0        0        0     4561 2023-06-14 09:06:29.000000 hgutilities-1.0.6/hgutilities/plotting/plotutils/griddimensions.py
+-rw-rw-rw-   0        0        0     4541 2023-06-14 09:06:29.000000 hgutilities-1.0.6/hgutilities/plotting/plotutils/plotshape.py
+-rw-rw-rw-   0        0        0     1330 2023-06-14 09:06:29.000000 hgutilities-1.0.6/hgutilities/plotting/plotutils/savefigure.py
+drwxrwxrwx   0        0        0        0 2023-06-14 09:11:27.709352 hgutilities-1.0.6/hgutilities/utils/
+-rw-rw-rw-   0        0        0        0 2023-06-14 09:06:29.000000 hgutilities-1.0.6/hgutilities/utils/__init__.py
+-rw-rw-rw-   0        0        0      195 2023-06-14 09:06:29.000000 hgutilities-1.0.6/hgutilities/utils/dicts.py
+-rw-rw-rw-   0        0        0     1456 2023-06-14 09:06:29.000000 hgutilities-1.0.6/hgutilities/utils/groups.py
+-rw-rw-rw-   0        0        0      961 2023-06-14 09:06:29.000000 hgutilities-1.0.6/hgutilities/utils/paths.py
+-rw-rw-rw-   0        0        0      697 2023-06-14 09:06:29.000000 hgutilities-1.0.6/hgutilities/utils/plots.py
+drwxrwxrwx   0        0        0        0 2023-06-14 09:11:27.605673 hgutilities-1.0.6/hgutilities.egg-info/
+-rw-rw-rw-   0        0        0     7982 2023-06-14 09:11:27.000000 hgutilities-1.0.6/hgutilities.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3707 2023-06-14 09:11:27.000000 hgutilities-1.0.6/hgutilities.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-14 09:11:27.000000 hgutilities-1.0.6/hgutilities.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       35 2023-06-14 09:11:27.000000 hgutilities-1.0.6/hgutilities.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-06-14 09:11:27.000000 hgutilities-1.0.6/hgutilities.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-14 09:11:27.709352 hgutilities-1.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     1491 2023-06-14 09:09:51.000000 hgutilities-1.0.6/setup.py
```

### Comparing `hgutilities-1.0.5/LICENSE.md` & `hgutilities-1.0.6/LICENSE.md`

 * *Ordering differences only*

 * *Files 7% similar despite different names*

```diff
@@ -1,674 +1,674 @@
-                    GNU GENERAL PUBLIC LICENSE
-                       Version 3, 29 June 2007
-
- Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
- Everyone is permitted to copy and distribute verbatim copies
- of this license document, but changing it is not allowed.
-
-                            Preamble
-
-  The GNU General Public License is a free, copyleft license for
-software and other kinds of works.
-
-  The licenses for most software and other practical works are designed
-to take away your freedom to share and change the works.  By contrast,
-the GNU General Public License is intended to guarantee your freedom to
-share and change all versions of a program--to make sure it remains free
-software for all its users.  We, the Free Software Foundation, use the
-GNU General Public License for most of our software; it applies also to
-any other work released this way by its authors.  You can apply it to
-your programs, too.
-
-  When we speak of free software, we are referring to freedom, not
-price.  Our General Public Licenses are designed to make sure that you
-have the freedom to distribute copies of free software (and charge for
-them if you wish), that you receive source code or can get it if you
-want it, that you can change the software or use pieces of it in new
-free programs, and that you know you can do these things.
-
-  To protect your rights, we need to prevent others from denying you
-these rights or asking you to surrender the rights.  Therefore, you have
-certain responsibilities if you distribute copies of the software, or if
-you modify it: responsibilities to respect the freedom of others.
-
-  For example, if you distribute copies of such a program, whether
-gratis or for a fee, you must pass on to the recipients the same
-freedoms that you received.  You must make sure that they, too, receive
-or can get the source code.  And you must show them these terms so they
-know their rights.
-
-  Developers that use the GNU GPL protect your rights with two steps:
-(1) assert copyright on the software, and (2) offer you this License
-giving you legal permission to copy, distribute and/or modify it.
-
-  For the developers' and authors' protection, the GPL clearly explains
-that there is no warranty for this free software.  For both users' and
-authors' sake, the GPL requires that modified versions be marked as
-changed, so that their problems will not be attributed erroneously to
-authors of previous versions.
-
-  Some devices are designed to deny users access to install or run
-modified versions of the software inside them, although the manufacturer
-can do so.  This is fundamentally incompatible with the aim of
-protecting users' freedom to change the software.  The systematic
-pattern of such abuse occurs in the area of products for individuals to
-use, which is precisely where it is most unacceptable.  Therefore, we
-have designed this version of the GPL to prohibit the practice for those
-products.  If such problems arise substantially in other domains, we
-stand ready to extend this provision to those domains in future versions
-of the GPL, as needed to protect the freedom of users.
-
-  Finally, every program is threatened constantly by software patents.
-States should not allow patents to restrict development and use of
-software on general-purpose computers, but in those that do, we wish to
-avoid the special danger that patents applied to a free program could
-make it effectively proprietary.  To prevent this, the GPL assures that
-patents cannot be used to render the program non-free.
-
-  The precise terms and conditions for copying, distribution and
-modification follow.
-
-                       TERMS AND CONDITIONS
-
-  0. Definitions.
-
-  "This License" refers to version 3 of the GNU General Public License.
-
-  "Copyright" also means copyright-like laws that apply to other kinds of
-works, such as semiconductor masks.
-
-  "The Program" refers to any copyrightable work licensed under this
-License.  Each licensee is addressed as "you".  "Licensees" and
-"recipients" may be individuals or organizations.
-
-  To "modify" a work means to copy from or adapt all or part of the work
-in a fashion requiring copyright permission, other than the making of an
-exact copy.  The resulting work is called a "modified version" of the
-earlier work or a work "based on" the earlier work.
-
-  A "covered work" means either the unmodified Program or a work based
-on the Program.
-
-  To "propagate" a work means to do anything with it that, without
-permission, would make you directly or secondarily liable for
-infringement under applicable copyright law, except executing it on a
-computer or modifying a private copy.  Propagation includes copying,
-distribution (with or without modification), making available to the
-public, and in some countries other activities as well.
-
-  To "convey" a work means any kind of propagation that enables other
-parties to make or receive copies.  Mere interaction with a user through
-a computer network, with no transfer of a copy, is not conveying.
-
-  An interactive user interface displays "Appropriate Legal Notices"
-to the extent that it includes a convenient and prominently visible
-feature that (1) displays an appropriate copyright notice, and (2)
-tells the user that there is no warranty for the work (except to the
-extent that warranties are provided), that licensees may convey the
-work under this License, and how to view a copy of this License.  If
-the interface presents a list of user commands or options, such as a
-menu, a prominent item in the list meets this criterion.
-
-  1. Source Code.
-
-  The "source code" for a work means the preferred form of the work
-for making modifications to it.  "Object code" means any non-source
-form of a work.
-
-  A "Standard Interface" means an interface that either is an official
-standard defined by a recognized standards body, or, in the case of
-interfaces specified for a particular programming language, one that
-is widely used among developers working in that language.
-
-  The "System Libraries" of an executable work include anything, other
-than the work as a whole, that (a) is included in the normal form of
-packaging a Major Component, but which is not part of that Major
-Component, and (b) serves only to enable use of the work with that
-Major Component, or to implement a Standard Interface for which an
-implementation is available to the public in source code form.  A
-"Major Component", in this context, means a major essential component
-(kernel, window system, and so on) of the specific operating system
-(if any) on which the executable work runs, or a compiler used to
-produce the work, or an object code interpreter used to run it.
-
-  The "Corresponding Source" for a work in object code form means all
-the source code needed to generate, install, and (for an executable
-work) run the object code and to modify the work, including scripts to
-control those activities.  However, it does not include the work's
-System Libraries, or general-purpose tools or generally available free
-programs which are used unmodified in performing those activities but
-which are not part of the work.  For example, Corresponding Source
-includes interface definition files associated with source files for
-the work, and the source code for shared libraries and dynamically
-linked subprograms that the work is specifically designed to require,
-such as by intimate data communication or control flow between those
-subprograms and other parts of the work.
-
-  The Corresponding Source need not include anything that users
-can regenerate automatically from other parts of the Corresponding
-Source.
-
-  The Corresponding Source for a work in source code form is that
-same work.
-
-  2. Basic Permissions.
-
-  All rights granted under this License are granted for the term of
-copyright on the Program, and are irrevocable provided the stated
-conditions are met.  This License explicitly affirms your unlimited
-permission to run the unmodified Program.  The output from running a
-covered work is covered by this License only if the output, given its
-content, constitutes a covered work.  This License acknowledges your
-rights of fair use or other equivalent, as provided by copyright law.
-
-  You may make, run and propagate covered works that you do not
-convey, without conditions so long as your license otherwise remains
-in force.  You may convey covered works to others for the sole purpose
-of having them make modifications exclusively for you, or provide you
-with facilities for running those works, provided that you comply with
-the terms of this License in conveying all material for which you do
-not control copyright.  Those thus making or running the covered works
-for you must do so exclusively on your behalf, under your direction
-and control, on terms that prohibit them from making any copies of
-your copyrighted material outside their relationship with you.
-
-  Conveying under any other circumstances is permitted solely under
-the conditions stated below.  Sublicensing is not allowed; section 10
-makes it unnecessary.
-
-  3. Protecting Users' Legal Rights From Anti-Circumvention Law.
-
-  No covered work shall be deemed part of an effective technological
-measure under any applicable law fulfilling obligations under article
-11 of the WIPO copyright treaty adopted on 20 December 1996, or
-similar laws prohibiting or restricting circumvention of such
-measures.
-
-  When you convey a covered work, you waive any legal power to forbid
-circumvention of technological measures to the extent such circumvention
-is effected by exercising rights under this License with respect to
-the covered work, and you disclaim any intention to limit operation or
-modification of the work as a means of enforcing, against the work's
-users, your or third parties' legal rights to forbid circumvention of
-technological measures.
-
-  4. Conveying Verbatim Copies.
-
-  You may convey verbatim copies of the Program's source code as you
-receive it, in any medium, provided that you conspicuously and
-appropriately publish on each copy an appropriate copyright notice;
-keep intact all notices stating that this License and any
-non-permissive terms added in accord with section 7 apply to the code;
-keep intact all notices of the absence of any warranty; and give all
-recipients a copy of this License along with the Program.
-
-  You may charge any price or no price for each copy that you convey,
-and you may offer support or warranty protection for a fee.
-
-  5. Conveying Modified Source Versions.
-
-  You may convey a work based on the Program, or the modifications to
-produce it from the Program, in the form of source code under the
-terms of section 4, provided that you also meet all of these conditions:
-
-    a) The work must carry prominent notices stating that you modified
-    it, and giving a relevant date.
-
-    b) The work must carry prominent notices stating that it is
-    released under this License and any conditions added under section
-    7.  This requirement modifies the requirement in section 4 to
-    "keep intact all notices".
-
-    c) You must license the entire work, as a whole, under this
-    License to anyone who comes into possession of a copy.  This
-    License will therefore apply, along with any applicable section 7
-    additional terms, to the whole of the work, and all its parts,
-    regardless of how they are packaged.  This License gives no
-    permission to license the work in any other way, but it does not
-    invalidate such permission if you have separately received it.
-
-    d) If the work has interactive user interfaces, each must display
-    Appropriate Legal Notices; however, if the Program has interactive
-    interfaces that do not display Appropriate Legal Notices, your
-    work need not make them do so.
-
-  A compilation of a covered work with other separate and independent
-works, which are not by their nature extensions of the covered work,
-and which are not combined with it such as to form a larger program,
-in or on a volume of a storage or distribution medium, is called an
-"aggregate" if the compilation and its resulting copyright are not
-used to limit the access or legal rights of the compilation's users
-beyond what the individual works permit.  Inclusion of a covered work
-in an aggregate does not cause this License to apply to the other
-parts of the aggregate.
-
-  6. Conveying Non-Source Forms.
-
-  You may convey a covered work in object code form under the terms
-of sections 4 and 5, provided that you also convey the
-machine-readable Corresponding Source under the terms of this License,
-in one of these ways:
-
-    a) Convey the object code in, or embodied in, a physical product
-    (including a physical distribution medium), accompanied by the
-    Corresponding Source fixed on a durable physical medium
-    customarily used for software interchange.
-
-    b) Convey the object code in, or embodied in, a physical product
-    (including a physical distribution medium), accompanied by a
-    written offer, valid for at least three years and valid for as
-    long as you offer spare parts or customer support for that product
-    model, to give anyone who possesses the object code either (1) a
-    copy of the Corresponding Source for all the software in the
-    product that is covered by this License, on a durable physical
-    medium customarily used for software interchange, for a price no
-    more than your reasonable cost of physically performing this
-    conveying of source, or (2) access to copy the
-    Corresponding Source from a network server at no charge.
-
-    c) Convey individual copies of the object code with a copy of the
-    written offer to provide the Corresponding Source.  This
-    alternative is allowed only occasionally and noncommercially, and
-    only if you received the object code with such an offer, in accord
-    with subsection 6b.
-
-    d) Convey the object code by offering access from a designated
-    place (gratis or for a charge), and offer equivalent access to the
-    Corresponding Source in the same way through the same place at no
-    further charge.  You need not require recipients to copy the
-    Corresponding Source along with the object code.  If the place to
-    copy the object code is a network server, the Corresponding Source
-    may be on a different server (operated by you or a third party)
-    that supports equivalent copying facilities, provided you maintain
-    clear directions next to the object code saying where to find the
-    Corresponding Source.  Regardless of what server hosts the
-    Corresponding Source, you remain obligated to ensure that it is
-    available for as long as needed to satisfy these requirements.
-
-    e) Convey the object code using peer-to-peer transmission, provided
-    you inform other peers where the object code and Corresponding
-    Source of the work are being offered to the general public at no
-    charge under subsection 6d.
-
-  A separable portion of the object code, whose source code is excluded
-from the Corresponding Source as a System Library, need not be
-included in conveying the object code work.
-
-  A "User Product" is either (1) a "consumer product", which means any
-tangible personal property which is normally used for personal, family,
-or household purposes, or (2) anything designed or sold for incorporation
-into a dwelling.  In determining whether a product is a consumer product,
-doubtful cases shall be resolved in favor of coverage.  For a particular
-product received by a particular user, "normally used" refers to a
-typical or common use of that class of product, regardless of the status
-of the particular user or of the way in which the particular user
-actually uses, or expects or is expected to use, the product.  A product
-is a consumer product regardless of whether the product has substantial
-commercial, industrial or non-consumer uses, unless such uses represent
-the only significant mode of use of the product.
-
-  "Installation Information" for a User Product means any methods,
-procedures, authorization keys, or other information required to install
-and execute modified versions of a covered work in that User Product from
-a modified version of its Corresponding Source.  The information must
-suffice to ensure that the continued functioning of the modified object
-code is in no case prevented or interfered with solely because
-modification has been made.
-
-  If you convey an object code work under this section in, or with, or
-specifically for use in, a User Product, and the conveying occurs as
-part of a transaction in which the right of possession and use of the
-User Product is transferred to the recipient in perpetuity or for a
-fixed term (regardless of how the transaction is characterized), the
-Corresponding Source conveyed under this section must be accompanied
-by the Installation Information.  But this requirement does not apply
-if neither you nor any third party retains the ability to install
-modified object code on the User Product (for example, the work has
-been installed in ROM).
-
-  The requirement to provide Installation Information does not include a
-requirement to continue to provide support service, warranty, or updates
-for a work that has been modified or installed by the recipient, or for
-the User Product in which it has been modified or installed.  Access to a
-network may be denied when the modification itself materially and
-adversely affects the operation of the network or violates the rules and
-protocols for communication across the network.
-
-  Corresponding Source conveyed, and Installation Information provided,
-in accord with this section must be in a format that is publicly
-documented (and with an implementation available to the public in
-source code form), and must require no special password or key for
-unpacking, reading or copying.
-
-  7. Additional Terms.
-
-  "Additional permissions" are terms that supplement the terms of this
-License by making exceptions from one or more of its conditions.
-Additional permissions that are applicable to the entire Program shall
-be treated as though they were included in this License, to the extent
-that they are valid under applicable law.  If additional permissions
-apply only to part of the Program, that part may be used separately
-under those permissions, but the entire Program remains governed by
-this License without regard to the additional permissions.
-
-  When you convey a copy of a covered work, you may at your option
-remove any additional permissions from that copy, or from any part of
-it.  (Additional permissions may be written to require their own
-removal in certain cases when you modify the work.)  You may place
-additional permissions on material, added by you to a covered work,
-for which you have or can give appropriate copyright permission.
-
-  Notwithstanding any other provision of this License, for material you
-add to a covered work, you may (if authorized by the copyright holders of
-that material) supplement the terms of this License with terms:
-
-    a) Disclaiming warranty or limiting liability differently from the
-    terms of sections 15 and 16 of this License; or
-
-    b) Requiring preservation of specified reasonable legal notices or
-    author attributions in that material or in the Appropriate Legal
-    Notices displayed by works containing it; or
-
-    c) Prohibiting misrepresentation of the origin of that material, or
-    requiring that modified versions of such material be marked in
-    reasonable ways as different from the original version; or
-
-    d) Limiting the use for publicity purposes of names of licensors or
-    authors of the material; or
-
-    e) Declining to grant rights under trademark law for use of some
-    trade names, trademarks, or service marks; or
-
-    f) Requiring indemnification of licensors and authors of that
-    material by anyone who conveys the material (or modified versions of
-    it) with contractual assumptions of liability to the recipient, for
-    any liability that these contractual assumptions directly impose on
-    those licensors and authors.
-
-  All other non-permissive additional terms are considered "further
-restrictions" within the meaning of section 10.  If the Program as you
-received it, or any part of it, contains a notice stating that it is
-governed by this License along with a term that is a further
-restriction, you may remove that term.  If a license document contains
-a further restriction but permits relicensing or conveying under this
-License, you may add to a covered work material governed by the terms
-of that license document, provided that the further restriction does
-not survive such relicensing or conveying.
-
-  If you add terms to a covered work in accord with this section, you
-must place, in the relevant source files, a statement of the
-additional terms that apply to those files, or a notice indicating
-where to find the applicable terms.
-
-  Additional terms, permissive or non-permissive, may be stated in the
-form of a separately written license, or stated as exceptions;
-the above requirements apply either way.
-
-  8. Termination.
-
-  You may not propagate or modify a covered work except as expressly
-provided under this License.  Any attempt otherwise to propagate or
-modify it is void, and will automatically terminate your rights under
-this License (including any patent licenses granted under the third
-paragraph of section 11).
-
-  However, if you cease all violation of this License, then your
-license from a particular copyright holder is reinstated (a)
-provisionally, unless and until the copyright holder explicitly and
-finally terminates your license, and (b) permanently, if the copyright
-holder fails to notify you of the violation by some reasonable means
-prior to 60 days after the cessation.
-
-  Moreover, your license from a particular copyright holder is
-reinstated permanently if the copyright holder notifies you of the
-violation by some reasonable means, this is the first time you have
-received notice of violation of this License (for any work) from that
-copyright holder, and you cure the violation prior to 30 days after
-your receipt of the notice.
-
-  Termination of your rights under this section does not terminate the
-licenses of parties who have received copies or rights from you under
-this License.  If your rights have been terminated and not permanently
-reinstated, you do not qualify to receive new licenses for the same
-material under section 10.
-
-  9. Acceptance Not Required for Having Copies.
-
-  You are not required to accept this License in order to receive or
-run a copy of the Program.  Ancillary propagation of a covered work
-occurring solely as a consequence of using peer-to-peer transmission
-to receive a copy likewise does not require acceptance.  However,
-nothing other than this License grants you permission to propagate or
-modify any covered work.  These actions infringe copyright if you do
-not accept this License.  Therefore, by modifying or propagating a
-covered work, you indicate your acceptance of this License to do so.
-
-  10. Automatic Licensing of Downstream Recipients.
-
-  Each time you convey a covered work, the recipient automatically
-receives a license from the original licensors, to run, modify and
-propagate that work, subject to this License.  You are not responsible
-for enforcing compliance by third parties with this License.
-
-  An "entity transaction" is a transaction transferring control of an
-organization, or substantially all assets of one, or subdividing an
-organization, or merging organizations.  If propagation of a covered
-work results from an entity transaction, each party to that
-transaction who receives a copy of the work also receives whatever
-licenses to the work the party's predecessor in interest had or could
-give under the previous paragraph, plus a right to possession of the
-Corresponding Source of the work from the predecessor in interest, if
-the predecessor has it or can get it with reasonable efforts.
-
-  You may not impose any further restrictions on the exercise of the
-rights granted or affirmed under this License.  For example, you may
-not impose a license fee, royalty, or other charge for exercise of
-rights granted under this License, and you may not initiate litigation
-(including a cross-claim or counterclaim in a lawsuit) alleging that
-any patent claim is infringed by making, using, selling, offering for
-sale, or importing the Program or any portion of it.
-
-  11. Patents.
-
-  A "contributor" is a copyright holder who authorizes use under this
-License of the Program or a work on which the Program is based.  The
-work thus licensed is called the contributor's "contributor version".
-
-  A contributor's "essential patent claims" are all patent claims
-owned or controlled by the contributor, whether already acquired or
-hereafter acquired, that would be infringed by some manner, permitted
-by this License, of making, using, or selling its contributor version,
-but do not include claims that would be infringed only as a
-consequence of further modification of the contributor version.  For
-purposes of this definition, "control" includes the right to grant
-patent sublicenses in a manner consistent with the requirements of
-this License.
-
-  Each contributor grants you a non-exclusive, worldwide, royalty-free
-patent license under the contributor's essential patent claims, to
-make, use, sell, offer for sale, import and otherwise run, modify and
-propagate the contents of its contributor version.
-
-  In the following three paragraphs, a "patent license" is any express
-agreement or commitment, however denominated, not to enforce a patent
-(such as an express permission to practice a patent or covenant not to
-sue for patent infringement).  To "grant" such a patent license to a
-party means to make such an agreement or commitment not to enforce a
-patent against the party.
-
-  If you convey a covered work, knowingly relying on a patent license,
-and the Corresponding Source of the work is not available for anyone
-to copy, free of charge and under the terms of this License, through a
-publicly available network server or other readily accessible means,
-then you must either (1) cause the Corresponding Source to be so
-available, or (2) arrange to deprive yourself of the benefit of the
-patent license for this particular work, or (3) arrange, in a manner
-consistent with the requirements of this License, to extend the patent
-license to downstream recipients.  "Knowingly relying" means you have
-actual knowledge that, but for the patent license, your conveying the
-covered work in a country, or your recipient's use of the covered work
-in a country, would infringe one or more identifiable patents in that
-country that you have reason to believe are valid.
-
-  If, pursuant to or in connection with a single transaction or
-arrangement, you convey, or propagate by procuring conveyance of, a
-covered work, and grant a patent license to some of the parties
-receiving the covered work authorizing them to use, propagate, modify
-or convey a specific copy of the covered work, then the patent license
-you grant is automatically extended to all recipients of the covered
-work and works based on it.
-
-  A patent license is "discriminatory" if it does not include within
-the scope of its coverage, prohibits the exercise of, or is
-conditioned on the non-exercise of one or more of the rights that are
-specifically granted under this License.  You may not convey a covered
-work if you are a party to an arrangement with a third party that is
-in the business of distributing software, under which you make payment
-to the third party based on the extent of your activity of conveying
-the work, and under which the third party grants, to any of the
-parties who would receive the covered work from you, a discriminatory
-patent license (a) in connection with copies of the covered work
-conveyed by you (or copies made from those copies), or (b) primarily
-for and in connection with specific products or compilations that
-contain the covered work, unless you entered into that arrangement,
-or that patent license was granted, prior to 28 March 2007.
-
-  Nothing in this License shall be construed as excluding or limiting
-any implied license or other defenses to infringement that may
-otherwise be available to you under applicable patent law.
-
-  12. No Surrender of Others' Freedom.
-
-  If conditions are imposed on you (whether by court order, agreement or
-otherwise) that contradict the conditions of this License, they do not
-excuse you from the conditions of this License.  If you cannot convey a
-covered work so as to satisfy simultaneously your obligations under this
-License and any other pertinent obligations, then as a consequence you may
-not convey it at all.  For example, if you agree to terms that obligate you
-to collect a royalty for further conveying from those to whom you convey
-the Program, the only way you could satisfy both those terms and this
-License would be to refrain entirely from conveying the Program.
-
-  13. Use with the GNU Affero General Public License.
-
-  Notwithstanding any other provision of this License, you have
-permission to link or combine any covered work with a work licensed
-under version 3 of the GNU Affero General Public License into a single
-combined work, and to convey the resulting work.  The terms of this
-License will continue to apply to the part which is the covered work,
-but the special requirements of the GNU Affero General Public License,
-section 13, concerning interaction through a network will apply to the
-combination as such.
-
-  14. Revised Versions of this License.
-
-  The Free Software Foundation may publish revised and/or new versions of
-the GNU General Public License from time to time.  Such new versions will
-be similar in spirit to the present version, but may differ in detail to
-address new problems or concerns.
-
-  Each version is given a distinguishing version number.  If the
-Program specifies that a certain numbered version of the GNU General
-Public License "or any later version" applies to it, you have the
-option of following the terms and conditions either of that numbered
-version or of any later version published by the Free Software
-Foundation.  If the Program does not specify a version number of the
-GNU General Public License, you may choose any version ever published
-by the Free Software Foundation.
-
-  If the Program specifies that a proxy can decide which future
-versions of the GNU General Public License can be used, that proxy's
-public statement of acceptance of a version permanently authorizes you
-to choose that version for the Program.
-
-  Later license versions may give you additional or different
-permissions.  However, no additional obligations are imposed on any
-author or copyright holder as a result of your choosing to follow a
-later version.
-
-  15. Disclaimer of Warranty.
-
-  THERE IS NO WARRANTY FOR THE PROGRAM, TO THE EXTENT PERMITTED BY
-APPLICABLE LAW.  EXCEPT WHEN OTHERWISE STATED IN WRITING THE COPYRIGHT
-HOLDERS AND/OR OTHER PARTIES PROVIDE THE PROGRAM "AS IS" WITHOUT WARRANTY
-OF ANY KIND, EITHER EXPRESSED OR IMPLIED, INCLUDING, BUT NOT LIMITED TO,
-THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
-PURPOSE.  THE ENTIRE RISK AS TO THE QUALITY AND PERFORMANCE OF THE PROGRAM
-IS WITH YOU.  SHOULD THE PROGRAM PROVE DEFECTIVE, YOU ASSUME THE COST OF
-ALL NECESSARY SERVICING, REPAIR OR CORRECTION.
-
-  16. Limitation of Liability.
-
-  IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN WRITING
-WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MODIFIES AND/OR CONVEYS
-THE PROGRAM AS PERMITTED ABOVE, BE LIABLE TO YOU FOR DAMAGES, INCLUDING ANY
-GENERAL, SPECIAL, INCIDENTAL OR CONSEQUENTIAL DAMAGES ARISING OUT OF THE
-USE OR INABILITY TO USE THE PROGRAM (INCLUDING BUT NOT LIMITED TO LOSS OF
-DATA OR DATA BEING RENDERED INACCURATE OR LOSSES SUSTAINED BY YOU OR THIRD
-PARTIES OR A FAILURE OF THE PROGRAM TO OPERATE WITH ANY OTHER PROGRAMS),
-EVEN IF SUCH HOLDER OR OTHER PARTY HAS BEEN ADVISED OF THE POSSIBILITY OF
-SUCH DAMAGES.
-
-  17. Interpretation of Sections 15 and 16.
-
-  If the disclaimer of warranty and limitation of liability provided
-above cannot be given local legal effect according to their terms,
-reviewing courts shall apply local law that most closely approximates
-an absolute waiver of all civil liability in connection with the
-Program, unless a warranty or assumption of liability accompanies a
-copy of the Program in return for a fee.
-
-                     END OF TERMS AND CONDITIONS
-
-            How to Apply These Terms to Your New Programs
-
-  If you develop a new program, and you want it to be of the greatest
-possible use to the public, the best way to achieve this is to make it
-free software which everyone can redistribute and change under these terms.
-
-  To do so, attach the following notices to the program.  It is safest
-to attach them to the start of each source file to most effectively
-state the exclusion of warranty; and each file should have at least
-the "copyright" line and a pointer to where the full notice is found.
-
-    <one line to give the program's name and a brief idea of what it does.>
-    Copyright (C) <year>  <name of author>
-
-    This program is free software: you can redistribute it and/or modify
-    it under the terms of the GNU General Public License as published by
-    the Free Software Foundation, either version 3 of the License, or
-    (at your option) any later version.
-
-    This program is distributed in the hope that it will be useful,
-    but WITHOUT ANY WARRANTY; without even the implied warranty of
-    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-    GNU General Public License for more details.
-
-    You should have received a copy of the GNU General Public License
-    along with this program.  If not, see <https://www.gnu.org/licenses/>.
-
-Also add information on how to contact you by electronic and paper mail.
-
-  If the program does terminal interaction, make it output a short
-notice like this when it starts in an interactive mode:
-
-    <program>  Copyright (C) <year>  <name of author>
-    This program comes with ABSOLUTELY NO WARRANTY; for details type `show w'.
-    This is free software, and you are welcome to redistribute it
-    under certain conditions; type `show c' for details.
-
-The hypothetical commands `show w' and `show c' should show the appropriate
-parts of the General Public License.  Of course, your program's commands
-might be different; for a GUI interface, you would use an "about box".
-
-  You should also get your employer (if you work as a programmer) or school,
-if any, to sign a "copyright disclaimer" for the program, if necessary.
-For more information on this, and how to apply and follow the GNU GPL, see
-<https://www.gnu.org/licenses/>.
-
-  The GNU General Public License does not permit incorporating your program
-into proprietary programs.  If your program is a subroutine library, you
-may consider it more useful to permit linking proprietary applications with
-the library.  If this is what you want to do, use the GNU Lesser General
-Public License instead of this License.  But first, please read
-<https://www.gnu.org/licenses/why-not-lgpl.html>.
+                    GNU GENERAL PUBLIC LICENSE
+                       Version 3, 29 June 2007
+
+ Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
+ Everyone is permitted to copy and distribute verbatim copies
+ of this license document, but changing it is not allowed.
+
+                            Preamble
+
+  The GNU General Public License is a free, copyleft license for
+software and other kinds of works.
+
+  The licenses for most software and other practical works are designed
+to take away your freedom to share and change the works.  By contrast,
+the GNU General Public License is intended to guarantee your freedom to
+share and change all versions of a program--to make sure it remains free
+software for all its users.  We, the Free Software Foundation, use the
+GNU General Public License for most of our software; it applies also to
+any other work released this way by its authors.  You can apply it to
+your programs, too.
+
+  When we speak of free software, we are referring to freedom, not
+price.  Our General Public Licenses are designed to make sure that you
+have the freedom to distribute copies of free software (and charge for
+them if you wish), that you receive source code or can get it if you
+want it, that you can change the software or use pieces of it in new
+free programs, and that you know you can do these things.
+
+  To protect your rights, we need to prevent others from denying you
+these rights or asking you to surrender the rights.  Therefore, you have
+certain responsibilities if you distribute copies of the software, or if
+you modify it: responsibilities to respect the freedom of others.
+
+  For example, if you distribute copies of such a program, whether
+gratis or for a fee, you must pass on to the recipients the same
+freedoms that you received.  You must make sure that they, too, receive
+or can get the source code.  And you must show them these terms so they
+know their rights.
+
+  Developers that use the GNU GPL protect your rights with two steps:
+(1) assert copyright on the software, and (2) offer you this License
+giving you legal permission to copy, distribute and/or modify it.
+
+  For the developers' and authors' protection, the GPL clearly explains
+that there is no warranty for this free software.  For both users' and
+authors' sake, the GPL requires that modified versions be marked as
+changed, so that their problems will not be attributed erroneously to
+authors of previous versions.
+
+  Some devices are designed to deny users access to install or run
+modified versions of the software inside them, although the manufacturer
+can do so.  This is fundamentally incompatible with the aim of
+protecting users' freedom to change the software.  The systematic
+pattern of such abuse occurs in the area of products for individuals to
+use, which is precisely where it is most unacceptable.  Therefore, we
+have designed this version of the GPL to prohibit the practice for those
+products.  If such problems arise substantially in other domains, we
+stand ready to extend this provision to those domains in future versions
+of the GPL, as needed to protect the freedom of users.
+
+  Finally, every program is threatened constantly by software patents.
+States should not allow patents to restrict development and use of
+software on general-purpose computers, but in those that do, we wish to
+avoid the special danger that patents applied to a free program could
+make it effectively proprietary.  To prevent this, the GPL assures that
+patents cannot be used to render the program non-free.
+
+  The precise terms and conditions for copying, distribution and
+modification follow.
+
+                       TERMS AND CONDITIONS
+
+  0. Definitions.
+
+  "This License" refers to version 3 of the GNU General Public License.
+
+  "Copyright" also means copyright-like laws that apply to other kinds of
+works, such as semiconductor masks.
+
+  "The Program" refers to any copyrightable work licensed under this
+License.  Each licensee is addressed as "you".  "Licensees" and
+"recipients" may be individuals or organizations.
+
+  To "modify" a work means to copy from or adapt all or part of the work
+in a fashion requiring copyright permission, other than the making of an
+exact copy.  The resulting work is called a "modified version" of the
+earlier work or a work "based on" the earlier work.
+
+  A "covered work" means either the unmodified Program or a work based
+on the Program.
+
+  To "propagate" a work means to do anything with it that, without
+permission, would make you directly or secondarily liable for
+infringement under applicable copyright law, except executing it on a
+computer or modifying a private copy.  Propagation includes copying,
+distribution (with or without modification), making available to the
+public, and in some countries other activities as well.
+
+  To "convey" a work means any kind of propagation that enables other
+parties to make or receive copies.  Mere interaction with a user through
+a computer network, with no transfer of a copy, is not conveying.
+
+  An interactive user interface displays "Appropriate Legal Notices"
+to the extent that it includes a convenient and prominently visible
+feature that (1) displays an appropriate copyright notice, and (2)
+tells the user that there is no warranty for the work (except to the
+extent that warranties are provided), that licensees may convey the
+work under this License, and how to view a copy of this License.  If
+the interface presents a list of user commands or options, such as a
+menu, a prominent item in the list meets this criterion.
+
+  1. Source Code.
+
+  The "source code" for a work means the preferred form of the work
+for making modifications to it.  "Object code" means any non-source
+form of a work.
+
+  A "Standard Interface" means an interface that either is an official
+standard defined by a recognized standards body, or, in the case of
+interfaces specified for a particular programming language, one that
+is widely used among developers working in that language.
+
+  The "System Libraries" of an executable work include anything, other
+than the work as a whole, that (a) is included in the normal form of
+packaging a Major Component, but which is not part of that Major
+Component, and (b) serves only to enable use of the work with that
+Major Component, or to implement a Standard Interface for which an
+implementation is available to the public in source code form.  A
+"Major Component", in this context, means a major essential component
+(kernel, window system, and so on) of the specific operating system
+(if any) on which the executable work runs, or a compiler used to
+produce the work, or an object code interpreter used to run it.
+
+  The "Corresponding Source" for a work in object code form means all
+the source code needed to generate, install, and (for an executable
+work) run the object code and to modify the work, including scripts to
+control those activities.  However, it does not include the work's
+System Libraries, or general-purpose tools or generally available free
+programs which are used unmodified in performing those activities but
+which are not part of the work.  For example, Corresponding Source
+includes interface definition files associated with source files for
+the work, and the source code for shared libraries and dynamically
+linked subprograms that the work is specifically designed to require,
+such as by intimate data communication or control flow between those
+subprograms and other parts of the work.
+
+  The Corresponding Source need not include anything that users
+can regenerate automatically from other parts of the Corresponding
+Source.
+
+  The Corresponding Source for a work in source code form is that
+same work.
+
+  2. Basic Permissions.
+
+  All rights granted under this License are granted for the term of
+copyright on the Program, and are irrevocable provided the stated
+conditions are met.  This License explicitly affirms your unlimited
+permission to run the unmodified Program.  The output from running a
+covered work is covered by this License only if the output, given its
+content, constitutes a covered work.  This License acknowledges your
+rights of fair use or other equivalent, as provided by copyright law.
+
+  You may make, run and propagate covered works that you do not
+convey, without conditions so long as your license otherwise remains
+in force.  You may convey covered works to others for the sole purpose
+of having them make modifications exclusively for you, or provide you
+with facilities for running those works, provided that you comply with
+the terms of this License in conveying all material for which you do
+not control copyright.  Those thus making or running the covered works
+for you must do so exclusively on your behalf, under your direction
+and control, on terms that prohibit them from making any copies of
+your copyrighted material outside their relationship with you.
+
+  Conveying under any other circumstances is permitted solely under
+the conditions stated below.  Sublicensing is not allowed; section 10
+makes it unnecessary.
+
+  3. Protecting Users' Legal Rights From Anti-Circumvention Law.
+
+  No covered work shall be deemed part of an effective technological
+measure under any applicable law fulfilling obligations under article
+11 of the WIPO copyright treaty adopted on 20 December 1996, or
+similar laws prohibiting or restricting circumvention of such
+measures.
+
+  When you convey a covered work, you waive any legal power to forbid
+circumvention of technological measures to the extent such circumvention
+is effected by exercising rights under this License with respect to
+the covered work, and you disclaim any intention to limit operation or
+modification of the work as a means of enforcing, against the work's
+users, your or third parties' legal rights to forbid circumvention of
+technological measures.
+
+  4. Conveying Verbatim Copies.
+
+  You may convey verbatim copies of the Program's source code as you
+receive it, in any medium, provided that you conspicuously and
+appropriately publish on each copy an appropriate copyright notice;
+keep intact all notices stating that this License and any
+non-permissive terms added in accord with section 7 apply to the code;
+keep intact all notices of the absence of any warranty; and give all
+recipients a copy of this License along with the Program.
+
+  You may charge any price or no price for each copy that you convey,
+and you may offer support or warranty protection for a fee.
+
+  5. Conveying Modified Source Versions.
+
+  You may convey a work based on the Program, or the modifications to
+produce it from the Program, in the form of source code under the
+terms of section 4, provided that you also meet all of these conditions:
+
+    a) The work must carry prominent notices stating that you modified
+    it, and giving a relevant date.
+
+    b) The work must carry prominent notices stating that it is
+    released under this License and any conditions added under section
+    7.  This requirement modifies the requirement in section 4 to
+    "keep intact all notices".
+
+    c) You must license the entire work, as a whole, under this
+    License to anyone who comes into possession of a copy.  This
+    License will therefore apply, along with any applicable section 7
+    additional terms, to the whole of the work, and all its parts,
+    regardless of how they are packaged.  This License gives no
+    permission to license the work in any other way, but it does not
+    invalidate such permission if you have separately received it.
+
+    d) If the work has interactive user interfaces, each must display
+    Appropriate Legal Notices; however, if the Program has interactive
+    interfaces that do not display Appropriate Legal Notices, your
+    work need not make them do so.
+
+  A compilation of a covered work with other separate and independent
+works, which are not by their nature extensions of the covered work,
+and which are not combined with it such as to form a larger program,
+in or on a volume of a storage or distribution medium, is called an
+"aggregate" if the compilation and its resulting copyright are not
+used to limit the access or legal rights of the compilation's users
+beyond what the individual works permit.  Inclusion of a covered work
+in an aggregate does not cause this License to apply to the other
+parts of the aggregate.
+
+  6. Conveying Non-Source Forms.
+
+  You may convey a covered work in object code form under the terms
+of sections 4 and 5, provided that you also convey the
+machine-readable Corresponding Source under the terms of this License,
+in one of these ways:
+
+    a) Convey the object code in, or embodied in, a physical product
+    (including a physical distribution medium), accompanied by the
+    Corresponding Source fixed on a durable physical medium
+    customarily used for software interchange.
+
+    b) Convey the object code in, or embodied in, a physical product
+    (including a physical distribution medium), accompanied by a
+    written offer, valid for at least three years and valid for as
+    long as you offer spare parts or customer support for that product
+    model, to give anyone who possesses the object code either (1) a
+    copy of the Corresponding Source for all the software in the
+    product that is covered by this License, on a durable physical
+    medium customarily used for software interchange, for a price no
+    more than your reasonable cost of physically performing this
+    conveying of source, or (2) access to copy the
+    Corresponding Source from a network server at no charge.
+
+    c) Convey individual copies of the object code with a copy of the
+    written offer to provide the Corresponding Source.  This
+    alternative is allowed only occasionally and noncommercially, and
+    only if you received the object code with such an offer, in accord
+    with subsection 6b.
+
+    d) Convey the object code by offering access from a designated
+    place (gratis or for a charge), and offer equivalent access to the
+    Corresponding Source in the same way through the same place at no
+    further charge.  You need not require recipients to copy the
+    Corresponding Source along with the object code.  If the place to
+    copy the object code is a network server, the Corresponding Source
+    may be on a different server (operated by you or a third party)
+    that supports equivalent copying facilities, provided you maintain
+    clear directions next to the object code saying where to find the
+    Corresponding Source.  Regardless of what server hosts the
+    Corresponding Source, you remain obligated to ensure that it is
+    available for as long as needed to satisfy these requirements.
+
+    e) Convey the object code using peer-to-peer transmission, provided
+    you inform other peers where the object code and Corresponding
+    Source of the work are being offered to the general public at no
+    charge under subsection 6d.
+
+  A separable portion of the object code, whose source code is excluded
+from the Corresponding Source as a System Library, need not be
+included in conveying the object code work.
+
+  A "User Product" is either (1) a "consumer product", which means any
+tangible personal property which is normally used for personal, family,
+or household purposes, or (2) anything designed or sold for incorporation
+into a dwelling.  In determining whether a product is a consumer product,
+doubtful cases shall be resolved in favor of coverage.  For a particular
+product received by a particular user, "normally used" refers to a
+typical or common use of that class of product, regardless of the status
+of the particular user or of the way in which the particular user
+actually uses, or expects or is expected to use, the product.  A product
+is a consumer product regardless of whether the product has substantial
+commercial, industrial or non-consumer uses, unless such uses represent
+the only significant mode of use of the product.
+
+  "Installation Information" for a User Product means any methods,
+procedures, authorization keys, or other information required to install
+and execute modified versions of a covered work in that User Product from
+a modified version of its Corresponding Source.  The information must
+suffice to ensure that the continued functioning of the modified object
+code is in no case prevented or interfered with solely because
+modification has been made.
+
+  If you convey an object code work under this section in, or with, or
+specifically for use in, a User Product, and the conveying occurs as
+part of a transaction in which the right of possession and use of the
+User Product is transferred to the recipient in perpetuity or for a
+fixed term (regardless of how the transaction is characterized), the
+Corresponding Source conveyed under this section must be accompanied
+by the Installation Information.  But this requirement does not apply
+if neither you nor any third party retains the ability to install
+modified object code on the User Product (for example, the work has
+been installed in ROM).
+
+  The requirement to provide Installation Information does not include a
+requirement to continue to provide support service, warranty, or updates
+for a work that has been modified or installed by the recipient, or for
+the User Product in which it has been modified or installed.  Access to a
+network may be denied when the modification itself materially and
+adversely affects the operation of the network or violates the rules and
+protocols for communication across the network.
+
+  Corresponding Source conveyed, and Installation Information provided,
+in accord with this section must be in a format that is publicly
+documented (and with an implementation available to the public in
+source code form), and must require no special password or key for
+unpacking, reading or copying.
+
+  7. Additional Terms.
+
+  "Additional permissions" are terms that supplement the terms of this
+License by making exceptions from one or more of its conditions.
+Additional permissions that are applicable to the entire Program shall
+be treated as though they were included in this License, to the extent
+that they are valid under applicable law.  If additional permissions
+apply only to part of the Program, that part may be used separately
+under those permissions, but the entire Program remains governed by
+this License without regard to the additional permissions.
+
+  When you convey a copy of a covered work, you may at your option
+remove any additional permissions from that copy, or from any part of
+it.  (Additional permissions may be written to require their own
+removal in certain cases when you modify the work.)  You may place
+additional permissions on material, added by you to a covered work,
+for which you have or can give appropriate copyright permission.
+
+  Notwithstanding any other provision of this License, for material you
+add to a covered work, you may (if authorized by the copyright holders of
+that material) supplement the terms of this License with terms:
+
+    a) Disclaiming warranty or limiting liability differently from the
+    terms of sections 15 and 16 of this License; or
+
+    b) Requiring preservation of specified reasonable legal notices or
+    author attributions in that material or in the Appropriate Legal
+    Notices displayed by works containing it; or
+
+    c) Prohibiting misrepresentation of the origin of that material, or
+    requiring that modified versions of such material be marked in
+    reasonable ways as different from the original version; or
+
+    d) Limiting the use for publicity purposes of names of licensors or
+    authors of the material; or
+
+    e) Declining to grant rights under trademark law for use of some
+    trade names, trademarks, or service marks; or
+
+    f) Requiring indemnification of licensors and authors of that
+    material by anyone who conveys the material (or modified versions of
+    it) with contractual assumptions of liability to the recipient, for
+    any liability that these contractual assumptions directly impose on
+    those licensors and authors.
+
+  All other non-permissive additional terms are considered "further
+restrictions" within the meaning of section 10.  If the Program as you
+received it, or any part of it, contains a notice stating that it is
+governed by this License along with a term that is a further
+restriction, you may remove that term.  If a license document contains
+a further restriction but permits relicensing or conveying under this
+License, you may add to a covered work material governed by the terms
+of that license document, provided that the further restriction does
+not survive such relicensing or conveying.
+
+  If you add terms to a covered work in accord with this section, you
+must place, in the relevant source files, a statement of the
+additional terms that apply to those files, or a notice indicating
+where to find the applicable terms.
+
+  Additional terms, permissive or non-permissive, may be stated in the
+form of a separately written license, or stated as exceptions;
+the above requirements apply either way.
+
+  8. Termination.
+
+  You may not propagate or modify a covered work except as expressly
+provided under this License.  Any attempt otherwise to propagate or
+modify it is void, and will automatically terminate your rights under
+this License (including any patent licenses granted under the third
+paragraph of section 11).
+
+  However, if you cease all violation of this License, then your
+license from a particular copyright holder is reinstated (a)
+provisionally, unless and until the copyright holder explicitly and
+finally terminates your license, and (b) permanently, if the copyright
+holder fails to notify you of the violation by some reasonable means
+prior to 60 days after the cessation.
+
+  Moreover, your license from a particular copyright holder is
+reinstated permanently if the copyright holder notifies you of the
+violation by some reasonable means, this is the first time you have
+received notice of violation of this License (for any work) from that
+copyright holder, and you cure the violation prior to 30 days after
+your receipt of the notice.
+
+  Termination of your rights under this section does not terminate the
+licenses of parties who have received copies or rights from you under
+this License.  If your rights have been terminated and not permanently
+reinstated, you do not qualify to receive new licenses for the same
+material under section 10.
+
+  9. Acceptance Not Required for Having Copies.
+
+  You are not required to accept this License in order to receive or
+run a copy of the Program.  Ancillary propagation of a covered work
+occurring solely as a consequence of using peer-to-peer transmission
+to receive a copy likewise does not require acceptance.  However,
+nothing other than this License grants you permission to propagate or
+modify any covered work.  These actions infringe copyright if you do
+not accept this License.  Therefore, by modifying or propagating a
+covered work, you indicate your acceptance of this License to do so.
+
+  10. Automatic Licensing of Downstream Recipients.
+
+  Each time you convey a covered work, the recipient automatically
+receives a license from the original licensors, to run, modify and
+propagate that work, subject to this License.  You are not responsible
+for enforcing compliance by third parties with this License.
+
+  An "entity transaction" is a transaction transferring control of an
+organization, or substantially all assets of one, or subdividing an
+organization, or merging organizations.  If propagation of a covered
+work results from an entity transaction, each party to that
+transaction who receives a copy of the work also receives whatever
+licenses to the work the party's predecessor in interest had or could
+give under the previous paragraph, plus a right to possession of the
+Corresponding Source of the work from the predecessor in interest, if
+the predecessor has it or can get it with reasonable efforts.
+
+  You may not impose any further restrictions on the exercise of the
+rights granted or affirmed under this License.  For example, you may
+not impose a license fee, royalty, or other charge for exercise of
+rights granted under this License, and you may not initiate litigation
+(including a cross-claim or counterclaim in a lawsuit) alleging that
+any patent claim is infringed by making, using, selling, offering for
+sale, or importing the Program or any portion of it.
+
+  11. Patents.
+
+  A "contributor" is a copyright holder who authorizes use under this
+License of the Program or a work on which the Program is based.  The
+work thus licensed is called the contributor's "contributor version".
+
+  A contributor's "essential patent claims" are all patent claims
+owned or controlled by the contributor, whether already acquired or
+hereafter acquired, that would be infringed by some manner, permitted
+by this License, of making, using, or selling its contributor version,
+but do not include claims that would be infringed only as a
+consequence of further modification of the contributor version.  For
+purposes of this definition, "control" includes the right to grant
+patent sublicenses in a manner consistent with the requirements of
+this License.
+
+  Each contributor grants you a non-exclusive, worldwide, royalty-free
+patent license under the contributor's essential patent claims, to
+make, use, sell, offer for sale, import and otherwise run, modify and
+propagate the contents of its contributor version.
+
+  In the following three paragraphs, a "patent license" is any express
+agreement or commitment, however denominated, not to enforce a patent
+(such as an express permission to practice a patent or covenant not to
+sue for patent infringement).  To "grant" such a patent license to a
+party means to make such an agreement or commitment not to enforce a
+patent against the party.
+
+  If you convey a covered work, knowingly relying on a patent license,
+and the Corresponding Source of the work is not available for anyone
+to copy, free of charge and under the terms of this License, through a
+publicly available network server or other readily accessible means,
+then you must either (1) cause the Corresponding Source to be so
+available, or (2) arrange to deprive yourself of the benefit of the
+patent license for this particular work, or (3) arrange, in a manner
+consistent with the requirements of this License, to extend the patent
+license to downstream recipients.  "Knowingly relying" means you have
+actual knowledge that, but for the patent license, your conveying the
+covered work in a country, or your recipient's use of the covered work
+in a country, would infringe one or more identifiable patents in that
+country that you have reason to believe are valid.
+
+  If, pursuant to or in connection with a single transaction or
+arrangement, you convey, or propagate by procuring conveyance of, a
+covered work, and grant a patent license to some of the parties
+receiving the covered work authorizing them to use, propagate, modify
+or convey a specific copy of the covered work, then the patent license
+you grant is automatically extended to all recipients of the covered
+work and works based on it.
+
+  A patent license is "discriminatory" if it does not include within
+the scope of its coverage, prohibits the exercise of, or is
+conditioned on the non-exercise of one or more of the rights that are
+specifically granted under this License.  You may not convey a covered
+work if you are a party to an arrangement with a third party that is
+in the business of distributing software, under which you make payment
+to the third party based on the extent of your activity of conveying
+the work, and under which the third party grants, to any of the
+parties who would receive the covered work from you, a discriminatory
+patent license (a) in connection with copies of the covered work
+conveyed by you (or copies made from those copies), or (b) primarily
+for and in connection with specific products or compilations that
+contain the covered work, unless you entered into that arrangement,
+or that patent license was granted, prior to 28 March 2007.
+
+  Nothing in this License shall be construed as excluding or limiting
+any implied license or other defenses to infringement that may
+otherwise be available to you under applicable patent law.
+
+  12. No Surrender of Others' Freedom.
+
+  If conditions are imposed on you (whether by court order, agreement or
+otherwise) that contradict the conditions of this License, they do not
+excuse you from the conditions of this License.  If you cannot convey a
+covered work so as to satisfy simultaneously your obligations under this
+License and any other pertinent obligations, then as a consequence you may
+not convey it at all.  For example, if you agree to terms that obligate you
+to collect a royalty for further conveying from those to whom you convey
+the Program, the only way you could satisfy both those terms and this
+License would be to refrain entirely from conveying the Program.
+
+  13. Use with the GNU Affero General Public License.
+
+  Notwithstanding any other provision of this License, you have
+permission to link or combine any covered work with a work licensed
+under version 3 of the GNU Affero General Public License into a single
+combined work, and to convey the resulting work.  The terms of this
+License will continue to apply to the part which is the covered work,
+but the special requirements of the GNU Affero General Public License,
+section 13, concerning interaction through a network will apply to the
+combination as such.
+
+  14. Revised Versions of this License.
+
+  The Free Software Foundation may publish revised and/or new versions of
+the GNU General Public License from time to time.  Such new versions will
+be similar in spirit to the present version, but may differ in detail to
+address new problems or concerns.
+
+  Each version is given a distinguishing version number.  If the
+Program specifies that a certain numbered version of the GNU General
+Public License "or any later version" applies to it, you have the
+option of following the terms and conditions either of that numbered
+version or of any later version published by the Free Software
+Foundation.  If the Program does not specify a version number of the
+GNU General Public License, you may choose any version ever published
+by the Free Software Foundation.
+
+  If the Program specifies that a proxy can decide which future
+versions of the GNU General Public License can be used, that proxy's
+public statement of acceptance of a version permanently authorizes you
+to choose that version for the Program.
+
+  Later license versions may give you additional or different
+permissions.  However, no additional obligations are imposed on any
+author or copyright holder as a result of your choosing to follow a
+later version.
+
+  15. Disclaimer of Warranty.
+
+  THERE IS NO WARRANTY FOR THE PROGRAM, TO THE EXTENT PERMITTED BY
+APPLICABLE LAW.  EXCEPT WHEN OTHERWISE STATED IN WRITING THE COPYRIGHT
+HOLDERS AND/OR OTHER PARTIES PROVIDE THE PROGRAM "AS IS" WITHOUT WARRANTY
+OF ANY KIND, EITHER EXPRESSED OR IMPLIED, INCLUDING, BUT NOT LIMITED TO,
+THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
+PURPOSE.  THE ENTIRE RISK AS TO THE QUALITY AND PERFORMANCE OF THE PROGRAM
+IS WITH YOU.  SHOULD THE PROGRAM PROVE DEFECTIVE, YOU ASSUME THE COST OF
+ALL NECESSARY SERVICING, REPAIR OR CORRECTION.
+
+  16. Limitation of Liability.
+
+  IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN WRITING
+WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MODIFIES AND/OR CONVEYS
+THE PROGRAM AS PERMITTED ABOVE, BE LIABLE TO YOU FOR DAMAGES, INCLUDING ANY
+GENERAL, SPECIAL, INCIDENTAL OR CONSEQUENTIAL DAMAGES ARISING OUT OF THE
+USE OR INABILITY TO USE THE PROGRAM (INCLUDING BUT NOT LIMITED TO LOSS OF
+DATA OR DATA BEING RENDERED INACCURATE OR LOSSES SUSTAINED BY YOU OR THIRD
+PARTIES OR A FAILURE OF THE PROGRAM TO OPERATE WITH ANY OTHER PROGRAMS),
+EVEN IF SUCH HOLDER OR OTHER PARTY HAS BEEN ADVISED OF THE POSSIBILITY OF
+SUCH DAMAGES.
+
+  17. Interpretation of Sections 15 and 16.
+
+  If the disclaimer of warranty and limitation of liability provided
+above cannot be given local legal effect according to their terms,
+reviewing courts shall apply local law that most closely approximates
+an absolute waiver of all civil liability in connection with the
+Program, unless a warranty or assumption of liability accompanies a
+copy of the Program in return for a fee.
+
+                     END OF TERMS AND CONDITIONS
+
+            How to Apply These Terms to Your New Programs
+
+  If you develop a new program, and you want it to be of the greatest
+possible use to the public, the best way to achieve this is to make it
+free software which everyone can redistribute and change under these terms.
+
+  To do so, attach the following notices to the program.  It is safest
+to attach them to the start of each source file to most effectively
+state the exclusion of warranty; and each file should have at least
+the "copyright" line and a pointer to where the full notice is found.
+
+    <one line to give the program's name and a brief idea of what it does.>
+    Copyright (C) <year>  <name of author>
+
+    This program is free software: you can redistribute it and/or modify
+    it under the terms of the GNU General Public License as published by
+    the Free Software Foundation, either version 3 of the License, or
+    (at your option) any later version.
+
+    This program is distributed in the hope that it will be useful,
+    but WITHOUT ANY WARRANTY; without even the implied warranty of
+    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+    GNU General Public License for more details.
+
+    You should have received a copy of the GNU General Public License
+    along with this program.  If not, see <https://www.gnu.org/licenses/>.
+
+Also add information on how to contact you by electronic and paper mail.
+
+  If the program does terminal interaction, make it output a short
+notice like this when it starts in an interactive mode:
+
+    <program>  Copyright (C) <year>  <name of author>
+    This program comes with ABSOLUTELY NO WARRANTY; for details type `show w'.
+    This is free software, and you are welcome to redistribute it
+    under certain conditions; type `show c' for details.
+
+The hypothetical commands `show w' and `show c' should show the appropriate
+parts of the General Public License.  Of course, your program's commands
+might be different; for a GUI interface, you would use an "about box".
+
+  You should also get your employer (if you work as a programmer) or school,
+if any, to sign a "copyright disclaimer" for the program, if necessary.
+For more information on this, and how to apply and follow the GNU GPL, see
+<https://www.gnu.org/licenses/>.
+
+  The GNU General Public License does not permit incorporating your program
+into proprietary programs.  If your program is a subroutine library, you
+may consider it more useful to permit linking proprietary applications with
+the library.  If this is what you want to do, use the GNU Lesser General
+Public License instead of this License.  But first, please read
+<https://www.gnu.org/licenses/why-not-lgpl.html>.
```

### Comparing `hgutilities-1.0.5/PKG-INFO` & `hgutilities-1.0.6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,99 +1,95 @@
-Metadata-Version: 2.1
-Name: hgutilities
-Version: 1.0.5
-Summary: A triple of tools used for plotting, handling key-words, and utilities
-Home-page: UNKNOWN
-Author: Henry Ginn
-Author-email: <henryginn137@gmail.com>
-License: UNKNOWN
-Keywords: python,matplotlib,plotting,default,keywords,utils
-Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Natural Language :: English
-Classifier: Operating System :: Unix
-Classifier: Operating System :: Microsoft :: Windows
-Description-Content-Type: text/markdown
-License-File: LICENSE.md
-
-
-# HGUtilities
-This is a collection of useful tools I use regularly. There are three parts to this package:
-
-- Defaults: manages settings for classes that can be controlled easily from an interface.
-- Plotting: a front end for matplotlib to easily create subplots.
-- Utils: a collection of generally useful functions
-
-## Contents
-
-1. [Defaults](#defaults)
-1. [Plotting](#plotting)
-1. [Utils](#utils)
-1. [Development](#development)
-
-## Defaults
-
-### The Problem
-
-Usually at the beginning of a class there will be a list of class variables with default values set. The aim of this part of the package is to deal with the following issues:
-
-- To view all the defaults you need to go into the script itself
-- It is awkward to change the value of those variables from an interface
-- It is impossible to change the default values without digging into the code itself.
-- Passing in many arguments to functions is messy
-- Mutable default values need to be implemented more carefully
-
-Normally there are two ways of handling keyword arguments with default values.The simpler way is to have the keyword in the function signature being set equal to it's default value. If it's default value is mutable, it will need to be set to None. Code will then need to be implemented to check if it has been changed, and if not, set it to it's default value. Once there are several keyword arguemnts, this becomes messy however, and it would be preferred to pack the keywords together with **kwargs. With this second method, there will need to be code that detects if a keyword is in the **kwargs dict, and if so change it. This means we have a method for every keyword argument a function takes in, and so we can easily end up with dozens of lines of code that clogs up our classes and is a chore to implement every time we change the keyword arguments a function takes in.
-
-In the second case, we cannot see what keyword arguments a function takes in, and can only do so in the first case if the we are calling a function directly unless each function in the middle also has all the keywords in the signature. Modifying the default values would also mean going into the code, finding the method where the keyword is processed, and editing the code directly.
-
-### The Solution
-
-For each class, we store the default values in a json file. After the class definition, we pass the class itself into a function that loads the values from the file, and sets them as class variables. This code is only run once when the file with the class is imported. The class will also have the attribute "defaults" assigned to it with all the default values. This allows the user to read what the defaults are from the interface, but beyond that it serves to purpose after the default values have been loaded in. If the user overwrites it, they will no longer be able to see the defaults for that object (with `my_obj.defaults`), and will need to look at the class attribute itself (with `MyClass.defaults`).
-
-Whenever a method takes in keyword arguments, they can be passed into a function that processes the kwargs, along with a reference to the instance itself. This will automate the process described in the previous section, and if there are any keyword arguments that were not in the list of defaults, the file will be opened and overwritten with the new keyword arguments added. Their default value will be set to `None`. Below is an example of how this is implemented.
-
-    from hgutilities import defaults
-
-    class MyClass():
-
-        def __init__(self, **kwargs):
-            defaults.kwargs(self, **kwargs)
-
-    defaults.load(MyClass)
-
-We note that `defaults.kwargs` can be called from anywhere within the class and not just at initialisation, and that `**kwargs` or `kwargs` can be fed in as the second argument. If there are kwargs that require more complicated processing, they can be processed after the call to `defaults.kwargs`, and the default value of such keyword arguments should be set to `null` in the json file of defaults.
-
-The path to the json file is stored as a class attribute `defaults_path`. In the directory that contains the script with the class, there will be another directory called "Default Settings", and this has the json files for all scripts in the original directory.
-
-## Plotting
-
-For full documentation, see the specific README inside the "plotting" module folder.
-
-When creating a figure with varying characteristics, the user needs to change their code in potentially non-trivial ways in order to get the desired result. For example, if they had 12 subplots on a figure, and they decide that they want two figures with six subplots each instead, a single for loop would need to be split into two different for loops. If one of the subplots needed two lines plotted instead of one, they would either need to add that in manually outside of the loop, or change the whole data structure to make it more general. When the number of subplots is unknown, these problems are even worse. The aim of this part of the package is to make the creation of such figures easier.
-
-The user creates data objects that store the information to be plotted. For example an instance of `Line` would have a list of $x$ values, a list of $y$ values, and optional settings such as a label and linestyle. A `Lines` object would have a collection of `Line` objects, and other information such as a subplot title, axes labels, whether it has a legend, etc. These objects can be passed in to a `Figures` object, and this does the work of deciding how they should be distributed among figures. The purpose of this is to give the user a way to easily specify what data needs to be plotted where, without needing to hardcode in the structure of the subplots.
-
-It also provides other functions such as easily applying a rainbow pattern to the lines, adding a legend that corresponds to multiple subplots, and applying prefixes to the axes. The ability to animate figures is also built in, although this should only be used for short gifs, on the order of a few dozen frames.
-
-## Utils
-
-The aim of this is to improve quality of coding life by implementing some common functions. For example when reading a json file, you cannot simply open the file and load the json, you must first check whether it is empty. Such annoyances are handled by the functions in this part of the package. We split the utilities into several categories to make it easier to organise them. The functions implemented here are tailored to my personal needs, and they may not have the desired functionality for a general use case. Backwards compatibility is not guaranteed.
-
-## Development
-
-### Features and functionality to add in V1.1
-
-- automatic prefixing to axes
-- more control over subplot placement
-- automatic paragraph organisation for documentation
-- better distribution of subplots over multiple figures
-- control over tick labels
-- horizontal bar charts
-- better file extension handling for Defaults package
-- inherit function should be able to take in a single attribute as a non-iterable
-- animations need to be made compatible with more plot types
-- add README to defaults subpackage
-
+Metadata-Version: 2.1
+Name: hgutilities
+Version: 1.0.6
+Summary: A triple of tools used for plotting, handling key-words, and utilities
+Author: Henry Ginn
+Author-email: <henryginn137@gmail.com>
+Keywords: python,matplotlib,plotting,default,keywords,utils
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Natural Language :: English
+Classifier: Operating System :: Unix
+Classifier: Operating System :: Microsoft :: Windows
+Description-Content-Type: text/markdown
+License-File: LICENSE.md
+
+
+# HGUtilities
+This is a collection of useful tools I use regularly. There are three parts to this package:
+
+- Defaults: manages settings for classes that can be controlled easily from an interface.
+- Plotting: a front end for matplotlib to easily create subplots.
+- Utils: a collection of generally useful functions
+
+## Contents
+
+1. [Defaults](#defaults)
+1. [Plotting](#plotting)
+1. [Utils](#utils)
+1. [Development](#development)
+
+## Defaults
+
+### The Problem
+
+Usually at the beginning of a class there will be a list of class variables with default values set. The aim of this part of the package is to deal with the following issues:
+
+- To view all the defaults you need to go into the script itself
+- It is awkward to change the value of those variables from an interface
+- It is impossible to change the default values without digging into the code itself.
+- Passing in many arguments to functions is messy
+- Mutable default values need to be implemented more carefully
+
+Normally there are two ways of handling keyword arguments with default values.The simpler way is to have the keyword in the function signature being set equal to it's default value. If it's default value is mutable, it will need to be set to None. Code will then need to be implemented to check if it has been changed, and if not, set it to it's default value. Once there are several keyword arguemnts, this becomes messy however, and it would be preferred to pack the keywords together with **kwargs. With this second method, there will need to be code that detects if a keyword is in the **kwargs dict, and if so change it. This means we have a method for every keyword argument a function takes in, and so we can easily end up with dozens of lines of code that clogs up our classes and is a chore to implement every time we change the keyword arguments a function takes in.
+
+In the second case, we cannot see what keyword arguments a function takes in, and can only do so in the first case if the we are calling a function directly unless each function in the middle also has all the keywords in the signature. Modifying the default values would also mean going into the code, finding the method where the keyword is processed, and editing the code directly.
+
+### The Solution
+
+For each class, we store the default values in a json file. After the class definition, we pass the class itself into a function that loads the values from the file, and sets them as class variables. This code is only run once when the file with the class is imported. The class will also have the attribute "defaults" assigned to it with all the default values. This allows the user to read what the defaults are from the interface, but beyond that it serves to purpose after the default values have been loaded in. If the user overwrites it, they will no longer be able to see the defaults for that object (with `my_obj.defaults`), and will need to look at the class attribute itself (with `MyClass.defaults`).
+
+Whenever a method takes in keyword arguments, they can be passed into a function that processes the kwargs, along with a reference to the instance itself. This will automate the process described in the previous section, and if there are any keyword arguments that were not in the list of defaults, the file will be opened and overwritten with the new keyword arguments added. Their default value will be set to `None`. Below is an example of how this is implemented.
+
+    from hgutilities import defaults
+
+    class MyClass():
+
+        def __init__(self, **kwargs):
+            defaults.kwargs(self, **kwargs)
+
+    defaults.load(MyClass)
+
+We note that `defaults.kwargs` can be called from anywhere within the class and not just at initialisation, and that `**kwargs` or `kwargs` can be fed in as the second argument. If there are kwargs that require more complicated processing, they can be processed after the call to `defaults.kwargs`, and the default value of such keyword arguments should be set to `null` in the json file of defaults.
+
+The path to the json file is stored as a class attribute `defaults_path`. In the directory that contains the script with the class, there will be another directory called "Default Settings", and this has the json files for all scripts in the original directory.
+
+## Plotting
+
+For full documentation, see the specific README inside the "plotting" module folder.
+
+When creating a figure with varying characteristics, the user needs to change their code in potentially non-trivial ways in order to get the desired result. For example, if they had 12 subplots on a figure, and they decide that they want two figures with six subplots each instead, a single for loop would need to be split into two different for loops. If one of the subplots needed two lines plotted instead of one, they would either need to add that in manually outside of the loop, or change the whole data structure to make it more general. When the number of subplots is unknown, these problems are even worse. The aim of this part of the package is to make the creation of such figures easier.
+
+The user creates data objects that store the information to be plotted. For example an instance of `Line` would have a list of $x$ values, a list of $y$ values, and optional settings such as a label and linestyle. A `Lines` object would have a collection of `Line` objects, and other information such as a subplot title, axes labels, whether it has a legend, etc. These objects can be passed in to a `Figures` object, and this does the work of deciding how they should be distributed among figures. The purpose of this is to give the user a way to easily specify what data needs to be plotted where, without needing to hardcode in the structure of the subplots.
+
+It also provides other functions such as easily applying a rainbow pattern to the lines, adding a legend that corresponds to multiple subplots, and applying prefixes to the axes. The ability to animate figures is also built in, although this should only be used for short gifs, on the order of a few dozen frames.
+
+## Utils
+
+The aim of this is to improve quality of coding life by implementing some common functions. For example when reading a json file, you cannot simply open the file and load the json, you must first check whether it is empty. Such annoyances are handled by the functions in this part of the package. We split the utilities into several categories to make it easier to organise them. The functions implemented here are tailored to my personal needs, and they may not have the desired functionality for a general use case. Backwards compatibility is not guaranteed.
+
+## Development
+
+### Features and functionality to add in V1.1
+
+- automatic prefixing to axes
+- more control over subplot placement
+- automatic paragraph organisation for documentation
+- better distribution of subplots over multiple figures
+- control over tick labels
+- horizontal bar charts
+- better file extension handling for Defaults package
+- inherit function should be able to take in a single attribute as a non-iterable
+- animations need to be made compatible with more plot types
+- add README to defaults subpackage
```

### Comparing `hgutilities-1.0.5/README.md` & `hgutilities-1.0.6/README.md`

 * *Ordering differences only*

 * *Files 7% similar despite different names*

```diff
@@ -1,77 +1,77 @@
-# HGUtilities
-This is a collection of useful tools I use regularly. There are three parts to this package:
-
-- Defaults: manages settings for classes that can be controlled easily from an interface.
-- Plotting: a front end for matplotlib to easily create subplots.
-- Utils: a collection of generally useful functions
-
-## Contents
-
-1. [Defaults](#defaults)
-1. [Plotting](#plotting)
-1. [Utils](#utils)
-1. [Development](#development)
-
-## Defaults
-
-### The Problem
-
-Usually at the beginning of a class there will be a list of class variables with default values set. The aim of this part of the package is to deal with the following issues:
-
-- To view all the defaults you need to go into the script itself
-- It is awkward to change the value of those variables from an interface
-- It is impossible to change the default values without digging into the code itself.
-- Passing in many arguments to functions is messy
-- Mutable default values need to be implemented more carefully
-
-Normally there are two ways of handling keyword arguments with default values.The simpler way is to have the keyword in the function signature being set equal to it's default value. If it's default value is mutable, it will need to be set to None. Code will then need to be implemented to check if it has been changed, and if not, set it to it's default value. Once there are several keyword arguemnts, this becomes messy however, and it would be preferred to pack the keywords together with **kwargs. With this second method, there will need to be code that detects if a keyword is in the **kwargs dict, and if so change it. This means we have a method for every keyword argument a function takes in, and so we can easily end up with dozens of lines of code that clogs up our classes and is a chore to implement every time we change the keyword arguments a function takes in.
-
-In the second case, we cannot see what keyword arguments a function takes in, and can only do so in the first case if the we are calling a function directly unless each function in the middle also has all the keywords in the signature. Modifying the default values would also mean going into the code, finding the method where the keyword is processed, and editing the code directly.
-
-### The Solution
-
-For each class, we store the default values in a json file. After the class definition, we pass the class itself into a function that loads the values from the file, and sets them as class variables. This code is only run once when the file with the class is imported. The class will also have the attribute "defaults" assigned to it with all the default values. This allows the user to read what the defaults are from the interface, but beyond that it serves to purpose after the default values have been loaded in. If the user overwrites it, they will no longer be able to see the defaults for that object (with `my_obj.defaults`), and will need to look at the class attribute itself (with `MyClass.defaults`).
-
-Whenever a method takes in keyword arguments, they can be passed into a function that processes the kwargs, along with a reference to the instance itself. This will automate the process described in the previous section, and if there are any keyword arguments that were not in the list of defaults, the file will be opened and overwritten with the new keyword arguments added. Their default value will be set to `None`. Below is an example of how this is implemented.
-
-    from hgutilities import defaults
-
-    class MyClass():
-
-        def __init__(self, **kwargs):
-            defaults.kwargs(self, **kwargs)
-
-    defaults.load(MyClass)
-
-We note that `defaults.kwargs` can be called from anywhere within the class and not just at initialisation, and that `**kwargs` or `kwargs` can be fed in as the second argument. If there are kwargs that require more complicated processing, they can be processed after the call to `defaults.kwargs`, and the default value of such keyword arguments should be set to `null` in the json file of defaults.
-
-The path to the json file is stored as a class attribute `defaults_path`. In the directory that contains the script with the class, there will be another directory called "Default Settings", and this has the json files for all scripts in the original directory.
-
-## Plotting
-
-For full documentation, see the specific README inside the "plotting" module folder.
-
-When creating a figure with varying characteristics, the user needs to change their code in potentially non-trivial ways in order to get the desired result. For example, if they had 12 subplots on a figure, and they decide that they want two figures with six subplots each instead, a single for loop would need to be split into two different for loops. If one of the subplots needed two lines plotted instead of one, they would either need to add that in manually outside of the loop, or change the whole data structure to make it more general. When the number of subplots is unknown, these problems are even worse. The aim of this part of the package is to make the creation of such figures easier.
-
-The user creates data objects that store the information to be plotted. For example an instance of `Line` would have a list of $x$ values, a list of $y$ values, and optional settings such as a label and linestyle. A `Lines` object would have a collection of `Line` objects, and other information such as a subplot title, axes labels, whether it has a legend, etc. These objects can be passed in to a `Figures` object, and this does the work of deciding how they should be distributed among figures. The purpose of this is to give the user a way to easily specify what data needs to be plotted where, without needing to hardcode in the structure of the subplots.
-
-It also provides other functions such as easily applying a rainbow pattern to the lines, adding a legend that corresponds to multiple subplots, and applying prefixes to the axes. The ability to animate figures is also built in, although this should only be used for short gifs, on the order of a few dozen frames.
-
-## Utils
-
-The aim of this is to improve quality of coding life by implementing some common functions. For example when reading a json file, you cannot simply open the file and load the json, you must first check whether it is empty. Such annoyances are handled by the functions in this part of the package. We split the utilities into several categories to make it easier to organise them. The functions implemented here are tailored to my personal needs, and they may not have the desired functionality for a general use case. Backwards compatibility is not guaranteed.
-
-## Development
-
-### Features and functionality to add in V1.1
-
-- automatic prefixing to axes
-- more control over subplot placement
-- automatic paragraph organisation for documentation
-- better distribution of subplots over multiple figures
-- control over tick labels
-- horizontal bar charts
-- better file extension handling for Defaults package
-- inherit function should be able to take in a single attribute as a non-iterable
-- animations need to be made compatible with more plot types
+# HGUtilities
+This is a collection of useful tools I use regularly. There are three parts to this package:
+
+- Defaults: manages settings for classes that can be controlled easily from an interface.
+- Plotting: a front end for matplotlib to easily create subplots.
+- Utils: a collection of generally useful functions
+
+## Contents
+
+1. [Defaults](#defaults)
+1. [Plotting](#plotting)
+1. [Utils](#utils)
+1. [Development](#development)
+
+## Defaults
+
+### The Problem
+
+Usually at the beginning of a class there will be a list of class variables with default values set. The aim of this part of the package is to deal with the following issues:
+
+- To view all the defaults you need to go into the script itself
+- It is awkward to change the value of those variables from an interface
+- It is impossible to change the default values without digging into the code itself.
+- Passing in many arguments to functions is messy
+- Mutable default values need to be implemented more carefully
+
+Normally there are two ways of handling keyword arguments with default values.The simpler way is to have the keyword in the function signature being set equal to it's default value. If it's default value is mutable, it will need to be set to None. Code will then need to be implemented to check if it has been changed, and if not, set it to it's default value. Once there are several keyword arguemnts, this becomes messy however, and it would be preferred to pack the keywords together with **kwargs. With this second method, there will need to be code that detects if a keyword is in the **kwargs dict, and if so change it. This means we have a method for every keyword argument a function takes in, and so we can easily end up with dozens of lines of code that clogs up our classes and is a chore to implement every time we change the keyword arguments a function takes in.
+
+In the second case, we cannot see what keyword arguments a function takes in, and can only do so in the first case if the we are calling a function directly unless each function in the middle also has all the keywords in the signature. Modifying the default values would also mean going into the code, finding the method where the keyword is processed, and editing the code directly.
+
+### The Solution
+
+For each class, we store the default values in a json file. After the class definition, we pass the class itself into a function that loads the values from the file, and sets them as class variables. This code is only run once when the file with the class is imported. The class will also have the attribute "defaults" assigned to it with all the default values. This allows the user to read what the defaults are from the interface, but beyond that it serves to purpose after the default values have been loaded in. If the user overwrites it, they will no longer be able to see the defaults for that object (with `my_obj.defaults`), and will need to look at the class attribute itself (with `MyClass.defaults`).
+
+Whenever a method takes in keyword arguments, they can be passed into a function that processes the kwargs, along with a reference to the instance itself. This will automate the process described in the previous section, and if there are any keyword arguments that were not in the list of defaults, the file will be opened and overwritten with the new keyword arguments added. Their default value will be set to `None`. Below is an example of how this is implemented.
+
+    from hgutilities import defaults
+
+    class MyClass():
+
+        def __init__(self, **kwargs):
+            defaults.kwargs(self, **kwargs)
+
+    defaults.load(MyClass)
+
+We note that `defaults.kwargs` can be called from anywhere within the class and not just at initialisation, and that `**kwargs` or `kwargs` can be fed in as the second argument. If there are kwargs that require more complicated processing, they can be processed after the call to `defaults.kwargs`, and the default value of such keyword arguments should be set to `null` in the json file of defaults.
+
+The path to the json file is stored as a class attribute `defaults_path`. In the directory that contains the script with the class, there will be another directory called "Default Settings", and this has the json files for all scripts in the original directory.
+
+## Plotting
+
+For full documentation, see the specific README inside the "plotting" module folder.
+
+When creating a figure with varying characteristics, the user needs to change their code in potentially non-trivial ways in order to get the desired result. For example, if they had 12 subplots on a figure, and they decide that they want two figures with six subplots each instead, a single for loop would need to be split into two different for loops. If one of the subplots needed two lines plotted instead of one, they would either need to add that in manually outside of the loop, or change the whole data structure to make it more general. When the number of subplots is unknown, these problems are even worse. The aim of this part of the package is to make the creation of such figures easier.
+
+The user creates data objects that store the information to be plotted. For example an instance of `Line` would have a list of $x$ values, a list of $y$ values, and optional settings such as a label and linestyle. A `Lines` object would have a collection of `Line` objects, and other information such as a subplot title, axes labels, whether it has a legend, etc. These objects can be passed in to a `Figures` object, and this does the work of deciding how they should be distributed among figures. The purpose of this is to give the user a way to easily specify what data needs to be plotted where, without needing to hardcode in the structure of the subplots.
+
+It also provides other functions such as easily applying a rainbow pattern to the lines, adding a legend that corresponds to multiple subplots, and applying prefixes to the axes. The ability to animate figures is also built in, although this should only be used for short gifs, on the order of a few dozen frames.
+
+## Utils
+
+The aim of this is to improve quality of coding life by implementing some common functions. For example when reading a json file, you cannot simply open the file and load the json, you must first check whether it is empty. Such annoyances are handled by the functions in this part of the package. We split the utilities into several categories to make it easier to organise them. The functions implemented here are tailored to my personal needs, and they may not have the desired functionality for a general use case. Backwards compatibility is not guaranteed.
+
+## Development
+
+### Features and functionality to add in V1.1
+
+- automatic prefixing to axes
+- more control over subplot placement
+- automatic paragraph organisation for documentation
+- better distribution of subplots over multiple figures
+- control over tick labels
+- horizontal bar charts
+- better file extension handling for Defaults package
+- inherit function should be able to take in a single attribute as a non-iterable
+- animations need to be made compatible with more plot types
 - add README to defaults subpackage
```

### Comparing `hgutilities-1.0.5/hgutilities/Documentation/hgutilities.txt` & `hgutilities-1.0.6/hgutilities/Documentation/hgutilities.txt`

 * *Ordering differences only*

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-This is a collection of useful tools I use regularly.
-
-There are three parts to this package:
-
-- Defaults: manages settings for classes that can be controlled easily from an interface.
-- Plotting: a front end for matplotlib to easily create subplots.
-- Utils: a collection of generally useful functions
-
-Defaults:
-This part of the package aims to make passing in keyword value pairs into classes easier. A list of keywords with their default values are stored in files and are loaded in upon creation of the class. When keywords are passed into a class, they can be fed into this sub-package along with the object instance where they are processed. Classes also inherit default values from parent classes. Tools for documentation and inheriting attributes from one object to another are also included.
-
-Plotting:
-When creating a figure with varying characteristics, the user needs to change their code in potentially non-trivial ways in order to get the desired result. For example, if they had 12 subplots on a figure, and they decide that they want two figures with six subplots each instead, a single for loop would need to be split into two different for loops. If one of the subplots needed two lines plotted instead of one, they would either need to add that in manually outside of the loop, or change the whole data structure to make it more general. When the number of subplots is unknown, these problems are even worse. The aim of the plotting part of the package is to make the creation of such figures easier.
-
-Utils:
-The aim of the utils part of this package is to improve quality of coding life by implementing some common functions. For example when reading a json file, you cannot simply open the file and load the json, you must first check whether it is empty. Such annoyances are handled by the functions in this part of the package. We split the utilities into several categories to make it easier to organise them. The functions implemented here are tailored to my personal needs, and they may not have the desired functionality for a general use case. Backwards compatibility is not guaranteed and it has been left undocumented. Where suitable spellings and names are consistent with matplotlib.
-
-For further documentation see the following:
-hgutils.defaults, hgutils.plotting
-https://github.com/HenryGinn/hgutilities
-https://github.com/HenryGinn/hgutilities/tree/main/hgutilities/defaults
-https://github.com/HenryGinn/hgutilities/tree/main/hgutilities/plotting
+This is a collection of useful tools I use regularly.
+
+There are three parts to this package:
+
+- Defaults: manages settings for classes that can be controlled easily from an interface.
+- Plotting: a front end for matplotlib to easily create subplots.
+- Utils: a collection of generally useful functions
+
+Defaults:
+This part of the package aims to make passing in keyword value pairs into classes easier. A list of keywords with their default values are stored in files and are loaded in upon creation of the class. When keywords are passed into a class, they can be fed into this sub-package along with the object instance where they are processed. Classes also inherit default values from parent classes. Tools for documentation and inheriting attributes from one object to another are also included.
+
+Plotting:
+When creating a figure with varying characteristics, the user needs to change their code in potentially non-trivial ways in order to get the desired result. For example, if they had 12 subplots on a figure, and they decide that they want two figures with six subplots each instead, a single for loop would need to be split into two different for loops. If one of the subplots needed two lines plotted instead of one, they would either need to add that in manually outside of the loop, or change the whole data structure to make it more general. When the number of subplots is unknown, these problems are even worse. The aim of the plotting part of the package is to make the creation of such figures easier.
+
+Utils:
+The aim of the utils part of this package is to improve quality of coding life by implementing some common functions. For example when reading a json file, you cannot simply open the file and load the json, you must first check whether it is empty. Such annoyances are handled by the functions in this part of the package. We split the utilities into several categories to make it easier to organise them. The functions implemented here are tailored to my personal needs, and they may not have the desired functionality for a general use case. Backwards compatibility is not guaranteed and it has been left undocumented. Where suitable spellings and names are consistent with matplotlib.
+
+For further documentation see the following:
+hgutils.defaults, hgutils.plotting
+https://github.com/HenryGinn/hgutilities
+https://github.com/HenryGinn/hgutilities/tree/main/hgutilities/defaults
+https://github.com/HenryGinn/hgutilities/tree/main/hgutilities/plotting
```

### Comparing `hgutilities-1.0.5/hgutilities/defaults/Documentation/docs.txt` & `hgutilities-1.0.6/hgutilities/defaults/Documentation/docs.txt`

 * *Ordering differences only*

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-The purpose of this function is to prevent bloated doc strings
-at the start of modules, classes, and functions by storing the
-doc strings in text files.
-
-By placing "defaults.docs()" in a package __init__.py file, all the
-modules, classes, and functions that were imported within that file
-that are part of the package will have their doc strings set. The
-doc strings are set from text files stored in folders called
-"Documentation", and these folders are in the same directory as
-the script for the corresponding module, class, or function.
-
-For further documentation see the following:
-https://github.com/HenryGinn/hgutilities
-https://github.com/HenryGinn/hgutilities/tree/main/hgutilities/defaults
+The purpose of this function is to prevent bloated doc strings
+at the start of modules, classes, and functions by storing the
+doc strings in text files.
+
+By placing "defaults.docs()" in a package __init__.py file, all the
+modules, classes, and functions that were imported within that file
+that are part of the package will have their doc strings set. The
+doc strings are set from text files stored in folders called
+"Documentation", and these folders are in the same directory as
+the script for the corresponding module, class, or function.
+
+For further documentation see the following:
+https://github.com/HenryGinn/hgutilities
+https://github.com/HenryGinn/hgutilities/tree/main/hgutilities/defaults
```

### Comparing `hgutilities-1.0.5/hgutilities/defaults/Documentation/loaddefaults.txt` & `hgutilities-1.0.6/hgutilities/defaults/Documentation/loaddefaults.txt`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-Load
-
-Takes key-word value pairs in a json file and sets them as
-class attributes. The file will have the same name as the class
-and should be located in a folder called "Default Settings" in
-the same folder as the script where the class is defined.
-
-After a class, (e.g. "MyClass") has been defined, calling
-"Defaults.load(MyClass)" will load from the file if it exists.
-
-Any keyword-value pairs defined in parent classes will be
-inherited.
-
-For further documentation see the following:
-kwargs
-https://github.com/HenryGinn/hgutilities
-https://github.com/HenryGinn/hgutilities/tree/main/hgutilities/defaults
+Load
+
+Takes key-word value pairs in a json file and sets them as
+class attributes. The file will have the same name as the class
+and should be located in a folder called "Default Settings" in
+the same folder as the script where the class is defined.
+
+After a class, (e.g. "MyClass") has been defined, calling
+"Defaults.load(MyClass)" will load from the file if it exists.
+
+Any keyword-value pairs defined in parent classes will be
+inherited.
+
+For further documentation see the following:
+kwargs
+https://github.com/HenryGinn/hgutilities
+https://github.com/HenryGinn/hgutilities/tree/main/hgutilities/defaults
```

### Comparing `hgutilities-1.0.5/hgutilities/defaults/Documentation/processkwargs.txt` & `hgutilities-1.0.6/hgutilities/defaults/Documentation/processkwargs.txt`

 * *Ordering differences only*

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-Allows the user to easily set the key-words passed in to classes
-as object attributes.
-
-Calling "defaults.kwargs(self, **kwargs)" or
-"defaults.kwargs(self, kwargs)" will take any key-word value pairs
-in the kwargs dict and assign them as object variables. If these
-key-words had default values set, they will be overruled by the new
-values passed in.
-
-For further documentation see the following:
-load, inherit
-https://github.com/HenryGinn/hgutilities
-https://github.com/HenryGinn/hgutilities/tree/main/hgutilities/defaults
+Allows the user to easily set the key-words passed in to classes
+as object attributes.
+
+Calling "defaults.kwargs(self, **kwargs)" or
+"defaults.kwargs(self, kwargs)" will take any key-word value pairs
+in the kwargs dict and assign them as object variables. If these
+key-words had default values set, they will be overruled by the new
+values passed in.
+
+For further documentation see the following:
+load, inherit
+https://github.com/HenryGinn/hgutilities
+https://github.com/HenryGinn/hgutilities/tree/main/hgutilities/defaults
```

### Comparing `hgutilities-1.0.5/hgutilities/defaults/docs.py` & `hgutilities-1.0.6/hgutilities/defaults/docs.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,81 +1,81 @@
-import os
-import traceback
-import inspect
-import sys
-
-class Docs():
-
-    def __init__(self):
-        self.extract_package()
-        self.process_package_directory()
-        self.add_package_docs()
-
-    def extract_package(self):
-        frame = inspect.stack()[3]
-        module = inspect.getmodule(frame[0])
-        self.package_path = os.path.split(module.__file__)[0]
-        self.package_name = module.__name__
-        self.package = sys.modules[self.package_name]
-
-    def process_package_directory(self):
-        for name, obj in inspect.getmembers(self.package):
-            if not inspect.ismodule(obj):
-                if hasattr(obj, "__module__"):
-                    self.filter_non_module_objects(obj)
-
-    def filter_non_module_objects(self, obj):
-        object_module = inspect.getmodule(obj)
-        common_path = self.get_common_path(object_module)
-        if common_path == self.package_path:
-            self.set_object_docs(obj)
-
-    def get_common_path(self, object_module):
-        object_module_path = object_module.__file__
-        common_path = os.path.commonpath((self.package_path, object_module_path))
-        return common_path
-
-    def set_object_docs(self, obj):
-        doc_path = self.get_doc_path(obj)
-        doc_string = self.get_doc_string_from_path(doc_path)
-        obj.__doc__ = doc_string
-
-    def get_doc_path(self, obj):
-        module = sys.modules[obj.__module__]
-        folder_path = os.path.split(module.__file__)[0]
-        name = os.path.splitext(obj.__name__)[0]
-        doc_path = self.get_doc_path_from_path_data(folder_path, name)
-        return doc_path
-
-    def get_doc_path_from_path_data(self, folder_path, name):
-        doc_file_name = f"{name}.txt"
-        doc_path = os.path.join(folder_path, "Documentation", doc_file_name)
-        return doc_path
-
-    def get_doc_string_from_path(self, doc_path):
-        if os.path.exists(doc_path):
-            return self.get_doc_string_from_existing_path(doc_path)
-        else:
-            return self.get_doc_string_from_non_existing_path(doc_path)
-
-    def get_doc_string_from_existing_path(self, doc_path):
-        with open(doc_path, "r") as file:
-            doc_string = "".join([line for line in file])
-        return doc_string
-
-    def get_doc_string_from_non_existing_path(self, doc_path):
-        return ("No documentation exists for this object.\n"
-                "It was expected to be found at the following location:\n"
-                f"{doc_path}\n")
-
-    def add_package_docs(self):
-        doc_path = self.get_package_doc_path()
-        doc_string = self.get_doc_string_from_path(doc_path)
-        self.package.__doc__ = doc_string
-
-    def get_package_doc_path(self):
-        name = self.package.__name__.split(".")[-1]
-        doc_path = self.get_doc_path_from_path_data(self.package_path, name)
-        return doc_path
-
-def docs():
-    docs_obj = Docs()
+import os
+import traceback
+import inspect
+import sys
+
+class Docs():
+
+    def __init__(self):
+        self.extract_package()
+        self.process_package_directory()
+        self.add_package_docs()
+
+    def extract_package(self):
+        frame = inspect.stack()[3]
+        module = inspect.getmodule(frame[0])
+        self.package_path = os.path.split(module.__file__)[0]
+        self.package_name = module.__name__
+        self.package = sys.modules[self.package_name]
+
+    def process_package_directory(self):
+        for name, obj in inspect.getmembers(self.package):
+            if not inspect.ismodule(obj):
+                if hasattr(obj, "__module__"):
+                    self.filter_non_module_objects(obj)
+
+    def filter_non_module_objects(self, obj):
+        object_module = inspect.getmodule(obj)
+        common_path = self.get_common_path(object_module)
+        if common_path == self.package_path:
+            self.set_object_docs(obj)
+
+    def get_common_path(self, object_module):
+        object_module_path = object_module.__file__
+        common_path = os.path.commonpath((self.package_path, object_module_path))
+        return common_path
+
+    def set_object_docs(self, obj):
+        doc_path = self.get_doc_path(obj)
+        doc_string = self.get_doc_string_from_path(doc_path)
+        obj.__doc__ = doc_string
+
+    def get_doc_path(self, obj):
+        module = sys.modules[obj.__module__]
+        folder_path = os.path.split(module.__file__)[0]
+        name = os.path.splitext(obj.__name__)[0]
+        doc_path = self.get_doc_path_from_path_data(folder_path, name)
+        return doc_path
+
+    def get_doc_path_from_path_data(self, folder_path, name):
+        doc_file_name = f"{name}.txt"
+        doc_path = os.path.join(folder_path, "Documentation", doc_file_name)
+        return doc_path
+
+    def get_doc_string_from_path(self, doc_path):
+        if os.path.exists(doc_path):
+            return self.get_doc_string_from_existing_path(doc_path)
+        else:
+            return self.get_doc_string_from_non_existing_path(doc_path)
+
+    def get_doc_string_from_existing_path(self, doc_path):
+        with open(doc_path, "r") as file:
+            doc_string = "".join([line for line in file])
+        return doc_string
+
+    def get_doc_string_from_non_existing_path(self, doc_path):
+        return ("No documentation exists for this object.\n"
+                "It was expected to be found at the following location:\n"
+                f"{doc_path}\n")
+
+    def add_package_docs(self):
+        doc_path = self.get_package_doc_path()
+        doc_string = self.get_doc_string_from_path(doc_path)
+        self.package.__doc__ = doc_string
+
+    def get_package_doc_path(self):
+        name = self.package.__name__.split(".")[-1]
+        doc_path = self.get_doc_path_from_path_data(self.package_path, name)
+        return doc_path
+
+def docs():
+    docs_obj = Docs()
```

### Comparing `hgutilities-1.0.5/hgutilities/defaults/inherit.py` & `hgutilities-1.0.6/hgutilities/defaults/inherit.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-def inherit(child_obj, parent_obj, attributes):
-    for attribute in attributes:
-        if hasattr(parent_obj, attribute):
-            parent_value = getattr(parent_obj, attribute)
-            attempt_attribute_inheritance(child_obj, parent_value, attribute)
-
-def attempt_attribute_inheritance(child_obj, parent_value, attribute):
-    if hasattr(child_obj, attribute):
-        child_has_attribute(child_obj, parent_value, attribute)
-    else:
-        setattr(child_obj, attribute, parent_value)
-
-def child_has_attribute(child_obj, parent_value, attribute):
-    if getattr(child_obj, attribute) is None:
-        setattr(child_obj, attribute, parent_value)
+def inherit(child_obj, parent_obj, attributes):
+    for attribute in attributes:
+        if hasattr(parent_obj, attribute):
+            parent_value = getattr(parent_obj, attribute)
+            attempt_attribute_inheritance(child_obj, parent_value, attribute)
+
+def attempt_attribute_inheritance(child_obj, parent_value, attribute):
+    if hasattr(child_obj, attribute):
+        child_has_attribute(child_obj, parent_value, attribute)
+    else:
+        setattr(child_obj, attribute, parent_value)
+
+def child_has_attribute(child_obj, parent_value, attribute):
+    if getattr(child_obj, attribute) is None:
+        setattr(child_obj, attribute, parent_value)
```

### Comparing `hgutilities-1.0.5/hgutilities/defaults/processkwargs.py` & `hgutilities-1.0.6/hgutilities/defaults/processkwargs.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,69 +1,69 @@
-import json
-
-from ..utils.paths import load_json
-from ..utils.paths import make_folder_path
-
-class ProcessKwargs():
-
-    def __init__(self, obj, *args, **kwargs):
-        self.set_obj(obj)
-        self.set_kwargs(args, kwargs)
-        self.try_process_kwargs()
-
-    def set_obj(self, obj):
-        if isinstance(obj, dict):
-            raise Exception("You need to pass the object instance into 'kwargs' function")
-        else:
-            self.obj = obj
-
-    def set_kwargs(self, args, kwargs):
-        if len(args) > 0 and isinstance(args[0], dict):
-            self.kwargs = args[0]
-        else:
-            self.kwargs = kwargs
-
-    def try_process_kwargs(self):
-        if hasattr(self.obj, "defaults_path"):
-            self.process_kwargs()
-
-    def process_kwargs(self):
-        self.key_words_to_add = []
-        self.process_key_words()
-        self.add_key_words_to_defaults()
-
-    def process_key_words(self):
-        for key_word, value in self.kwargs.items():
-            self.process_key_word(key_word, value)
-
-    def process_key_word(self, key_word, value):
-        setattr(self.obj, key_word, value)
-        if key_word not in self.obj.defaults:
-            self.key_words_to_add.append(key_word)
-
-    def add_key_words_to_defaults(self):
-        if self.add_extra_defaults_to_file():
-            self.do_add_key_words_to_defaults()
-
-    def add_extra_defaults_to_file(self):
-        if "add_input_kwargs_to_file" in self.obj.defaults:
-            return self.obj.defaults["add_input_kwargs_to_file"]
-        else:
-            return False
-
-    def do_add_key_words_to_defaults(self):
-        original_file_contents = load_json(self.obj.defaults_path, ignore_empty_or_none=True)
-        new_file_contents = self.add_key_words_to_file_contents(original_file_contents)
-        self.save_file_contents(original_file_contents, new_file_contents)
-
-    def add_key_words_to_file_contents(self, original_file_contents):
-        new_file_contents = dict(original_file_contents)
-        for key_word in self.key_words_to_add:
-            if key_word not in original_file_contents:
-                new_file_contents.update({key_word: None})
-        return new_file_contents
-
-    def save_file_contents(self, original_file_contents, new_file_contents):
-        if len(original_file_contents) != len(new_file_contents):
-            make_folder_path(self.obj.defaults_path)
-            with open(self.obj.defaults_path, "w") as file:
-                json.dump(new_file_contents, file, indent=2)
+import json
+
+from ..utils.paths import load_json
+from ..utils.paths import make_folder_path
+
+class ProcessKwargs():
+
+    def __init__(self, obj, *args, **kwargs):
+        self.set_obj(obj)
+        self.set_kwargs(args, kwargs)
+        self.try_process_kwargs()
+
+    def set_obj(self, obj):
+        if isinstance(obj, dict):
+            raise Exception("You need to pass the object instance into 'kwargs' function")
+        else:
+            self.obj = obj
+
+    def set_kwargs(self, args, kwargs):
+        if len(args) > 0 and isinstance(args[0], dict):
+            self.kwargs = args[0]
+        else:
+            self.kwargs = kwargs
+
+    def try_process_kwargs(self):
+        if hasattr(self.obj, "defaults_path"):
+            self.process_kwargs()
+
+    def process_kwargs(self):
+        self.key_words_to_add = []
+        self.process_key_words()
+        self.add_key_words_to_defaults()
+
+    def process_key_words(self):
+        for key_word, value in self.kwargs.items():
+            self.process_key_word(key_word, value)
+
+    def process_key_word(self, key_word, value):
+        setattr(self.obj, key_word, value)
+        if key_word not in self.obj.defaults:
+            self.key_words_to_add.append(key_word)
+
+    def add_key_words_to_defaults(self):
+        if self.add_extra_defaults_to_file():
+            self.do_add_key_words_to_defaults()
+
+    def add_extra_defaults_to_file(self):
+        if "add_input_kwargs_to_file" in self.obj.defaults:
+            return self.obj.defaults["add_input_kwargs_to_file"]
+        else:
+            return False
+
+    def do_add_key_words_to_defaults(self):
+        original_file_contents = load_json(self.obj.defaults_path, ignore_empty_or_none=True)
+        new_file_contents = self.add_key_words_to_file_contents(original_file_contents)
+        self.save_file_contents(original_file_contents, new_file_contents)
+
+    def add_key_words_to_file_contents(self, original_file_contents):
+        new_file_contents = dict(original_file_contents)
+        for key_word in self.key_words_to_add:
+            if key_word not in original_file_contents:
+                new_file_contents.update({key_word: None})
+        return new_file_contents
+
+    def save_file_contents(self, original_file_contents, new_file_contents):
+        if len(original_file_contents) != len(new_file_contents):
+            make_folder_path(self.obj.defaults_path)
+            with open(self.obj.defaults_path, "w") as file:
+                json.dump(new_file_contents, file, indent=2)
```

### Comparing `hgutilities-1.0.5/hgutilities/plotting/Default Settings/Figure.txt` & `hgutilities-1.0.6/hgutilities/plotting/Default Settings/Figure.txt`

 * *Format-specific differences are supported for JSON files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JSON text data*

 * *Files 22% similar despite different names*

```diff
@@ -1,37 +1,38 @@
-00000000: 7b0a 2020 2274 6974 6c65 223a 206e 756c  {.  "title": nul
-00000010: 6c2c 0a20 2022 6461 726b 223a 2066 616c  l,.  "dark": fal
-00000020: 7365 2c0a 2020 226d 6178 696d 6973 6522  se,.  "maximise"
-00000030: 3a20 7472 7565 2c0a 2020 2264 7069 223a  : true,.  "dpi":
-00000040: 206e 756c 6c2c 0a20 2022 6669 6775 7265   null,.  "figure
-00000050: 5f73 697a 6522 3a20 6e75 6c6c 2c0a 2020  _size": null,.  
-00000060: 2273 7562 706c 6f74 7322 3a20 6e75 6c6c  "subplots": null
-00000070: 2c0a 2020 2277 5f70 6164 223a 2030 2e33  ,.  "w_pad": 0.3
-00000080: 2c0a 2020 2268 5f70 6164 223a 2030 2e33  ,.  "h_pad": 0.3
-00000090: 2c0a 2020 2268 7370 6163 6522 3a20 6e75  ,.  "hspace": nu
-000000a0: 6c6c 2c0a 2020 2277 7370 6163 6522 3a20  ll,.  "wspace": 
-000000b0: 6e75 6c6c 2c0a 2020 2274 6974 6c65 5f66  null,.  "title_f
-000000c0: 6f6e 746e 616d 6522 3a20 6e75 6c6c 2c0a  ontname": null,.
-000000d0: 2020 2274 6974 6c65 5f66 6f6e 7473 697a    "title_fontsiz
-000000e0: 6522 3a20 6e75 6c6c 2c0a 2020 2274 6974  e": null,.  "tit
-000000f0: 6c65 5f63 6f6c 6f72 223a 206e 756c 6c2c  le_color": null,
-00000100: 0a20 2022 7469 746c 655f 7665 7274 6963  .  "title_vertic
-00000110: 616c 616c 6967 6e6d 656e 7422 3a20 6e75  alalignment": nu
-00000120: 6c6c 2c0a 2020 2274 6974 6c65 5f68 6f72  ll,.  "title_hor
-00000130: 697a 6f6e 7461 6c61 6c69 676e 6d65 6e74  izontalalignment
-00000140: 223a 206e 756c 6c2c 0a20 2022 7469 746c  ": null,.  "titl
-00000150: 655f 7922 3a20 6e75 6c6c 2c0a 2020 2274  e_y": null,.  "t
-00000160: 6974 6c65 5f70 6164 223a 206e 756c 6c2c  itle_pad": null,
-00000170: 0a20 2022 7469 746c 655f 6c6f 6322 3a20  .  "title_loc": 
-00000180: 6e75 6c6c 2c0a 2020 2261 7869 735f 666f  null,.  "axis_fo
-00000190: 6e74 6e61 6d65 223a 206e 756c 6c2c 0a20  ntname": null,. 
-000001a0: 2022 6178 6973 5f66 6f6e 7473 697a 6522   "axis_fontsize"
-000001b0: 3a20 6e75 6c6c 2c0a 2020 2261 7869 735f  : null,.  "axis_
-000001c0: 636f 6c6f 7222 3a20 6e75 6c6c 2c0a 2020  color": null,.  
-000001d0: 2261 7869 735f 6c61 6265 6c70 6164 223a  "axis_labelpad":
-000001e0: 206e 756c 6c2c 0a20 2022 6178 6973 5f6c   null,.  "axis_l
-000001f0: 6f63 223a 206e 756c 6c2c 0a20 2022 785f  oc": null,.  "x_
-00000200: 6178 6973 5f72 6f74 6174 696f 6e22 3a20  axis_rotation": 
-00000210: 302c 0a20 2022 795f 6178 6973 5f72 6f74  0,.  "y_axis_rot
-00000220: 6174 696f 6e22 3a20 302c 0a20 2022 7a5f  ation": 0,.  "z_
-00000230: 6178 6973 5f72 6f74 6174 696f 6e22 3a20  axis_rotation": 
-00000240: 300a 7d0a                                0.}.
+00000000: 7b0d 0a20 2022 7469 746c 6522 3a20 6e75  {..  "title": nu
+00000010: 6c6c 2c0d 0a20 2022 6461 726b 223a 2066  ll,..  "dark": f
+00000020: 616c 7365 2c0d 0a20 2022 6d61 7869 6d69  alse,..  "maximi
+00000030: 7365 223a 2074 7275 652c 0d0a 2020 2264  se": true,..  "d
+00000040: 7069 223a 206e 756c 6c2c 0d0a 2020 2266  pi": null,..  "f
+00000050: 6967 7572 655f 7369 7a65 223a 206e 756c  igure_size": nul
+00000060: 6c2c 0d0a 2020 2273 7562 706c 6f74 7322  l,..  "subplots"
+00000070: 3a20 6e75 6c6c 2c0d 0a20 2022 775f 7061  : null,..  "w_pa
+00000080: 6422 3a20 302e 332c 0d0a 2020 2268 5f70  d": 0.3,..  "h_p
+00000090: 6164 223a 2030 2e33 2c0d 0a20 2022 6873  ad": 0.3,..  "hs
+000000a0: 7061 6365 223a 206e 756c 6c2c 0d0a 2020  pace": null,..  
+000000b0: 2277 7370 6163 6522 3a20 6e75 6c6c 2c0d  "wspace": null,.
+000000c0: 0a20 2022 7469 746c 655f 666f 6e74 6e61  .  "title_fontna
+000000d0: 6d65 223a 206e 756c 6c2c 0d0a 2020 2274  me": null,..  "t
+000000e0: 6974 6c65 5f66 6f6e 7473 697a 6522 3a20  itle_fontsize": 
+000000f0: 6e75 6c6c 2c0d 0a20 2022 7469 746c 655f  null,..  "title_
+00000100: 636f 6c6f 7222 3a20 6e75 6c6c 2c0d 0a20  color": null,.. 
+00000110: 2022 7469 746c 655f 7665 7274 6963 616c   "title_vertical
+00000120: 616c 6967 6e6d 656e 7422 3a20 6e75 6c6c  alignment": null
+00000130: 2c0d 0a20 2022 7469 746c 655f 686f 7269  ,..  "title_hori
+00000140: 7a6f 6e74 616c 616c 6967 6e6d 656e 7422  zontalalignment"
+00000150: 3a20 6e75 6c6c 2c0d 0a20 2022 7469 746c  : null,..  "titl
+00000160: 655f 7922 3a20 6e75 6c6c 2c0d 0a20 2022  e_y": null,..  "
+00000170: 7469 746c 655f 7061 6422 3a20 6e75 6c6c  title_pad": null
+00000180: 2c0d 0a20 2022 7469 746c 655f 6c6f 6322  ,..  "title_loc"
+00000190: 3a20 6e75 6c6c 2c0d 0a20 2022 6178 6973  : null,..  "axis
+000001a0: 5f66 6f6e 746e 616d 6522 3a20 6e75 6c6c  _fontname": null
+000001b0: 2c0d 0a20 2022 6178 6973 5f66 6f6e 7473  ,..  "axis_fonts
+000001c0: 697a 6522 3a20 6e75 6c6c 2c0d 0a20 2022  ize": null,..  "
+000001d0: 6178 6973 5f63 6f6c 6f72 223a 206e 756c  axis_color": nul
+000001e0: 6c2c 0d0a 2020 2261 7869 735f 6c61 6265  l,..  "axis_labe
+000001f0: 6c70 6164 223a 206e 756c 6c2c 0d0a 2020  lpad": null,..  
+00000200: 2261 7869 735f 6c6f 6322 3a20 6e75 6c6c  "axis_loc": null
+00000210: 2c0d 0a20 2022 785f 6178 6973 5f72 6f74  ,..  "x_axis_rot
+00000220: 6174 696f 6e22 3a20 302c 0d0a 2020 2279  ation": 0,..  "y
+00000230: 5f61 7869 735f 726f 7461 7469 6f6e 223a  _axis_rotation":
+00000240: 2030 2c0d 0a20 2022 7a5f 6178 6973 5f72   0,..  "z_axis_r
+00000250: 6f74 6174 696f 6e22 3a20 300d 0a7d 0d0a  otation": 0..}..
```

### Comparing `hgutilities-1.0.5/hgutilities/plotting/Documentation/Animate.txt` & `hgutilities-1.0.6/hgutilities/plotting/Documentation/Animate.txt`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-A subclass of Figures, this is responsible for creating
-short animations.
-
-create_animations is an interface for this class.
-
-Takes in a list of Data objects. These are just like
-regular Data objects, but the dependent variable should
-instead be an iterable where each element gives the values
-for a single frame.
-
-Currently this is only implemented for Surface objects.
-
-Animate.defaults shows a list of optional kwargs.
-
-For further documentation see the following:
-https://github.com/HenryGinn/hgutilities
-https://github.com/HenryGinn/hgutilities/tree/main/hgutilities/plotting
+A subclass of Figures, this is responsible for creating
+short animations.
+
+create_animations is an interface for this class.
+
+Takes in a list of Data objects. These are just like
+regular Data objects, but the dependent variable should
+instead be an iterable where each element gives the values
+for a single frame.
+
+Currently this is only implemented for Surface objects.
+
+Animate.defaults shows a list of optional kwargs.
+
+For further documentation see the following:
+https://github.com/HenryGinn/hgutilities
+https://github.com/HenryGinn/hgutilities/tree/main/hgutilities/plotting
```

### Comparing `hgutilities-1.0.5/hgutilities/plotting/Documentation/create_animations.txt` & `hgutilities-1.0.6/hgutilities/plotting/Documentation/create_animations.txt`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-This function will take in a list of data objects
-and produce an animation. These Data objects are just
-like regular Data objects, but the dependent variable
-should instead be an iterable where each element gives
-the values for a single frame.
-
-This is an interface for the Animate class, and to
-see a list of optional key-word arguments you can
-look at Animate.defaults, Figures.defaults and
-Figure.defaults.
-
-This also returns the Figures object produced if
-the user wants to work with it directly, but this
-is not encouraged, and should only be necessary if
-a feature has not been implemented.
-
-For further documentation see the following:
-Animate, Figures, and Data classes
-https://github.com/HenryGinn/hgutilities
-https://github.com/HenryGinn/hgutilities/tree/main/hgutilities/plotting
+This function will take in a list of data objects
+and produce an animation. These Data objects are just
+like regular Data objects, but the dependent variable
+should instead be an iterable where each element gives
+the values for a single frame.
+
+This is an interface for the Animate class, and to
+see a list of optional key-word arguments you can
+look at Animate.defaults, Figures.defaults and
+Figure.defaults.
+
+This also returns the Figures object produced if
+the user wants to work with it directly, but this
+is not encouraged, and should only be necessary if
+a feature has not been implemented.
+
+For further documentation see the following:
+Animate, Figures, and Data classes
+https://github.com/HenryGinn/hgutilities
+https://github.com/HenryGinn/hgutilities/tree/main/hgutilities/plotting
```

### Comparing `hgutilities-1.0.5/hgutilities/plotting/Documentation/create_figures.txt` & `hgutilities-1.0.6/hgutilities/plotting/Documentation/create_figures.txt`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-This function will take in a list of data objects
-and produce a set of figures showing them.
-
-This is an interface for the Figures class, and to
-see a list of optional key-word arguments you can
-look at Figures.defaults and Figure.defaults.
-
-This also returns the Figures object produced if
-the user wants to work with it directly, but this
-is not encouraged, and should only be necessary if
-a feature has not been implemented.
-
-For further documentation see the following:
-Figures and Data classes
-https://github.com/HenryGinn/hgutilities
-https://github.com/HenryGinn/hgutilities/tree/main/hgutilities/plotting
+This function will take in a list of data objects
+and produce a set of figures showing them.
+
+This is an interface for the Figures class, and to
+see a list of optional key-word arguments you can
+look at Figures.defaults and Figure.defaults.
+
+This also returns the Figures object produced if
+the user wants to work with it directly, but this
+is not encouraged, and should only be necessary if
+a feature has not been implemented.
+
+For further documentation see the following:
+Figures and Data classes
+https://github.com/HenryGinn/hgutilities
+https://github.com/HenryGinn/hgutilities/tree/main/hgutilities/plotting
```

### Comparing `hgutilities-1.0.5/hgutilities/plotting/Documentation/plotting.txt` & `hgutilities-1.0.6/hgutilities/plotting/Documentation/plotting.txt`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-This package is an interface for matplotlib and is designed to make
-creation and processing of figures with subplots easier. The data and
-settings are specified, and they are arranged on figures where the user
-can control the maximum number of subplots on each figure and prescribe
-a target aspect ratio. If the subplots do not fit on one figure, they
-will be spread over multiple figures. The number of figures is no more
-than the ceiling of the total number of plots divided by the maximum
-number of plots per figure.
-
-While this package offers a lot of flexibility, it is mainly intended for
-convenient production of figures. For publication quality plots, it is
-recommended that the full flexibility of matplotlib or other plotting
-packages should be used instead. This package performs best for purposes
-such as analysing data and making powerpoints to be shared among
-colleages and students.
-
-Functions defined here:
-
-create_figures
-create_animations
-
-For further documentation see the following:
-Data and Figures classes and functions from the above list
-https://github.com/HenryGinn/HGUtils
-https://github.com/HenryGinn/HGUtils/tree/main/Plotting
+This package is an interface for matplotlib and is designed to make
+creation and processing of figures with subplots easier. The data and
+settings are specified, and they are arranged on figures where the user
+can control the maximum number of subplots on each figure and prescribe
+a target aspect ratio. If the subplots do not fit on one figure, they
+will be spread over multiple figures. The number of figures is no more
+than the ceiling of the total number of plots divided by the maximum
+number of plots per figure.
+
+While this package offers a lot of flexibility, it is mainly intended for
+convenient production of figures. For publication quality plots, it is
+recommended that the full flexibility of matplotlib or other plotting
+packages should be used instead. This package performs best for purposes
+such as analysing data and making powerpoints to be shared among
+colleages and students.
+
+Functions defined here:
+
+create_figures
+create_animations
+
+For further documentation see the following:
+Data and Figures classes and functions from the above list
+https://github.com/HenryGinn/HGUtils
+https://github.com/HenryGinn/HGUtils/tree/main/Plotting
```

### Comparing `hgutilities-1.0.5/hgutilities/plotting/README.md` & `hgutilities-1.0.6/hgutilities/plotting/README.md`

 * *Ordering differences only*

 * *Files 9% similar despite different names*

```diff
@@ -1,201 +1,201 @@
-# Plotting
-
-## Contents
-
-1. [Overview and Structure](#overview-and-structure)
-    1. [Figures](#figures)
-    1. [Animate](#animate)
-    1. [Figure](#figure)
-    1. [Plot](#plot)
-    1. [Data](#data)
-1. [Usage](#usage)
-1. [Features](#features)
-    1. [Universal Legend](#universal-legend)
-    1. [Subplot Adjustment](#subplot-adjustment)
-
-## Overview and Structure
-
-This is a tool designed to make creating figures with multiple subplots easier. The data is prescribed, and the creation of the figures is handled by the package.
-
-### Figures
-
-At the top level there is a Figures object. This contains all the information about the figures to be produced. This includes the data to be plotted, the title of the figures, if the figures are going to be shown or saved, the base path to be saved to if needed, the number of subplots per figure, and any appearance settings of the plots. It organises the creation of Figure objects, as if there is too much data for one figure, it will need to be spread over multiple.
-
-### Animate
-
-This is a subclass of Figures, and allows the user to make animations. Creating animations is done through exactly the same process as creating figures, with one difference. The independent variables can't be animated, but the dependent variables will need to be passed in as a list or array where each element of the list or array gives the values of the variable for each frame. See the [usage](#usage) section for more details.
-
-### Figure
-
-The next level down is the Figure object. This arranges how the subplots will be arranged on the figure and organises the creation of the subplots, which are subsequently handled by Plot objects. Adding the title and universal legend happens here. An aspect ratio can be specified, and it will try to arrange the plots in that ratio as closely as it can.
-
-### Plot
-
-A Plot object is responsible for each individual subplot. The subplot title, axis labels, plot legends, and the data to be put on the subplot are handled at this level. There are subclasses of Plot for different types of data object, and these classes follow the naming convention of appending "Plot" to the name of the data object they are associated with.
-
-### Data
-
-This class handles the data to be plotted. The most basic is a Lines object which handles quantititive data on a 2D plot. There is also a Bars object which handles bar charts, and a Pie object that handles pie charts. Colorplot and Surface are also subclasses which work with 3 dimensional data. As a rule of thumb, if two matplotlib plotting functions are sufficiently different, their data will be handled by two distinct subclasses of Data. Here are the subclasses of Data currently implemented.
-
-- Lines. This takes in a collection of Line objects. It also has an optional keyword argument called `plot_type` which controls whether the plot is made using `plot`, `semilogy`, `semilogx`, `loglog`, or `errorbar`. Each Line object corresponds to a single line on a subplot, and has a list of $x$ values and $y$ values. The Line object also has optional attributes that control the appearance of the line and the line label.
-- Bars. This is similar to Lines, but it handles Bar objects which are similar to Line objects. The key distinction here is that the $x$ axis has qualitative data, and that prescribing the appearance of the bars is very different from lines. We note that a Bar object handles an entire series of data, and a Bars object handles a bar chart plot, so a single plot with two data series on it will be handled by one Bars object and two Bar objects.
-- Pie. Pie charts cannot show multiple data series so this subclass does not have a correspondence to Line or Bar. This takes in all the arguments that the matplotlib `pie` function takes in, and also any of the arguments from the parent class, Plot.
-- Colormesh. This shows a single data series with two dimensional input and one dimensional output. It takes in almost all of the arguments that the matplotlib pcolormesh function takes in and uses pcolormesh instead of pcolor.
-- Surface. This shows a single data series with a two dimensional input and a one dimensional output. Different from Colormesh, this produces a plot in three spatial dimensions represented as a surface. Wireframe and 3D contour plotting is also supported by passing in "plot_wireframe" or "contour" as a value of the `plot_type` keyword
-
-### Usage
-
-The first step in creating a figure is specifying the data. Here is an example with plotting a single line on a graph. `lines_obj` is the Data object in this case, and we pass it in to `create_figures`.
-    
-    # Importing
-    import numpy as np
-    from hgutilities import plotting
-
-    # Creation of Line object
-    x_values = np.arange(0, 2*np.pi, 0.1)
-    y_values = np.sin(x_values)
-    line_obj = plotting.line(x_values, y_values)
-
-    # Creation of Lines object
-    lines_obj = plotting.lines(line_obj)
-
-    # Creation of figures
-    plotting.create_figures(lines_obj)
-
-If we want to create multiple lines, we can pass in a list of line objects. We can also give our figure some labels.
-
-
-    # Importing
-    import numpy as np
-    from hgutilities import plotting
-
-    # Creation of Line object
-    def get_line_obj(n):
-        y_values = np.sin(n*x_values)
-        label = f"n = {n}"
-        line_obj = plotting.line(x_values, y_values, label=label)
-        return line_obj
-
-    x_values = np.arange(0, 2*np.pi, 0.01)
-    x_coefficients = [1, 2, 3]
-    line_objects = [get_line_obj(n) for n in x_coefficients]
-
-    # Creation of Lines object
-    title = "Sin(nx)"
-    x_label = "My x axis label"
-    y_label = "My y axis label"
-    lines_obj = plotting.lines(line_objects, title=title, legend=True,
-                                  x_label=x_label, y_label=y_label)
-
-    # Creation of figures
-    plotting.create_figures(lines_obj)
-
-We could have data split across multiple subplots. By default we have `subplots=None` and all subplots will be put on a figure. If subplots is specified and the subplots do not fit on one figure, they will be distributed across multiple. The subplots will be evenly distributed over $\left \lfloor \frac{\text{total subplots}}{\text{subplots per figure}} \right \rfloor$ figures, so the number of subplots per figure is at least as big as the number specified. In future versions this behaviour will change, and the number given by the subplots keyword will be an upper bound on how many subplots there will be on a given figure, and the number of figures will be as small as possible given that constraint.
-
-    # Importing
-    import numpy as np
-    from hgutilities import plotting
-
-    def get_lines_obj(n):
-        line_obj = get_line_obj(n)
-        title = f"Sin({n}x)"
-        x_label = "My x axis label"
-        y_label = "My y axis label"
-        lines_obj = plotting.lines(line_obj, title=title,
-        x_label=x_label, y_label=y_label)
-        return lines_obj
-
-    def get_line_obj(n):
-        y_values = np.sin(n*x_values)
-        line_obj = plotting.line(x_values, y_values)
-        return line_obj
-
-    # Creation of lines objects
-    x_values = np.arange(0, 2*np.pi, 0.01)
-    x_coefficients = list(range(1, 13))
-    lines_objects = [get_lines_obj(n) for n in x_coefficients]
-
-    # Creation of figures
-    plotting.create_figures(lines_objects, subplots=6)
-
-You can mix the types of plot within a figure. Here is an example that shows the other types of plot supported.
-
-    # Importing
-    import numpy as np
-    from hgutilities import plotting
-
-    # Creating bars object
-    x_values_1 = ["Red", "Green", "Blue"]
-    y_values_1 = [4, 2, 7]
-    bar_obj_1 = plotting.bar(x_values_1, y_values_1)
-
-    x_values_2 = ["Green", "Red", "Blue"]
-    y_values_2 = [1, 4, 5]
-    bar_obj_2 = plotting.bar(x_values_2, y_values_2)
-
-    title = "Bar Chart Example"
-    bar_objects = [bar_obj_1, bar_obj_2]
-    bars_obj = plotting.bars(bar_objects, title=title)
-
-    # Creating pie object
-    values = [4, 2, 7]
-    labels = ["Red", "Green", "Blue"]
-    title = "Pie Chart Example"
-    pie_obj = plotting.pie(values, labels, title=title,
-                           colors=labels, test=False)
-
-    # Creating surface object
-    x_values = np.arange(0, 10, 0.01)
-    y_values = np.arange(0, 10, 0.01)
-    x_mesh, y_mesh = np.meshgrid(x_values, y_values)
-    z_mesh = np.cos(x_mesh) + np.cos(y_mesh)
-    title = "Surface Plot Example"
-    surface_obj = plotting.surface(x_mesh, y_mesh, z_mesh,
-                                   title=title)
-
-    # Creating colorplot object
-    title = "Colorplot Example"
-    colormap_obj = plotting.colorplot(x_mesh, y_mesh, z_mesh,
-                                      title=title)
-
-    # Creation of figures
-    data_objects = [bars_obj, pie_obj, surface_obj, colormap_obj]
-    plotting.create_figures(data_objects)
-
-Animations can also be made by adding a dimension to the dependent variable. Currently this is only implemented for Surface objects. We note that all matplotlib figure objects need to be kept open while making the animation, so this is only suitable for short animations.
-
-    # Importing
-    import numpy as np
-    from hgutilities import plotting
-
-    # Set independent variable values
-    x_values = np.arange(0, 10, 0.5)
-    y_values = np.arange(0, 10, 0.5)
-    x_mesh, y_mesh = np.meshgrid(x_values, y_values)
-
-    # Set dependent variable values
-    def get_z_mesh_layer(time_value):
-        time_mesh = np.ones(x_mesh.shape) * time_value
-        z_mesh_layer = (np.sin(x_mesh + time_mesh)
-                        + np.sin(y_mesh + time_mesh))
-        return z_mesh_layer
-
-    time_values = np.arange(0, 2*np.pi, 0.5)
-    z_meshes = [get_z_mesh_layer(time_value)
-                for time_value in time_values]
-    z_meshes = np.stack(z_meshes)
-
-    # Creating animation
-    surface_obj = plotting.surface(x_mesh, y_mesh, z_meshes)
-    surface_objects = [surface_obj]
-    plotting.create_animations(surface_objects)
-
-## Features
-
-### Universal Legend
-
-The universal legend is a tool that can be used if all subplots in a figure have the same legend. An extra blank subplot is created and the space is used to show a legend that corresponds to all plots. This can be activated by passing `universal_legend=True` as a keyword-value pair into the `create_figures` function, and any individual legends will be overruled. Exception handling not implemented, will crash or get unexpected results if not used properly.
-
-### Subplot Adjustment
-
+# Plotting
+
+## Contents
+
+1. [Overview and Structure](#overview-and-structure)
+    1. [Figures](#figures)
+    1. [Animate](#animate)
+    1. [Figure](#figure)
+    1. [Plot](#plot)
+    1. [Data](#data)
+1. [Usage](#usage)
+1. [Features](#features)
+    1. [Universal Legend](#universal-legend)
+    1. [Subplot Adjustment](#subplot-adjustment)
+
+## Overview and Structure
+
+This is a tool designed to make creating figures with multiple subplots easier. The data is prescribed, and the creation of the figures is handled by the package.
+
+### Figures
+
+At the top level there is a Figures object. This contains all the information about the figures to be produced. This includes the data to be plotted, the title of the figures, if the figures are going to be shown or saved, the base path to be saved to if needed, the number of subplots per figure, and any appearance settings of the plots. It organises the creation of Figure objects, as if there is too much data for one figure, it will need to be spread over multiple.
+
+### Animate
+
+This is a subclass of Figures, and allows the user to make animations. Creating animations is done through exactly the same process as creating figures, with one difference. The independent variables can't be animated, but the dependent variables will need to be passed in as a list or array where each element of the list or array gives the values of the variable for each frame. See the [usage](#usage) section for more details.
+
+### Figure
+
+The next level down is the Figure object. This arranges how the subplots will be arranged on the figure and organises the creation of the subplots, which are subsequently handled by Plot objects. Adding the title and universal legend happens here. An aspect ratio can be specified, and it will try to arrange the plots in that ratio as closely as it can.
+
+### Plot
+
+A Plot object is responsible for each individual subplot. The subplot title, axis labels, plot legends, and the data to be put on the subplot are handled at this level. There are subclasses of Plot for different types of data object, and these classes follow the naming convention of appending "Plot" to the name of the data object they are associated with.
+
+### Data
+
+This class handles the data to be plotted. The most basic is a Lines object which handles quantititive data on a 2D plot. There is also a Bars object which handles bar charts, and a Pie object that handles pie charts. Colorplot and Surface are also subclasses which work with 3 dimensional data. As a rule of thumb, if two matplotlib plotting functions are sufficiently different, their data will be handled by two distinct subclasses of Data. Here are the subclasses of Data currently implemented.
+
+- Lines. This takes in a collection of Line objects. It also has an optional keyword argument called `plot_type` which controls whether the plot is made using `plot`, `semilogy`, `semilogx`, `loglog`, or `errorbar`. Each Line object corresponds to a single line on a subplot, and has a list of $x$ values and $y$ values. The Line object also has optional attributes that control the appearance of the line and the line label.
+- Bars. This is similar to Lines, but it handles Bar objects which are similar to Line objects. The key distinction here is that the $x$ axis has qualitative data, and that prescribing the appearance of the bars is very different from lines. We note that a Bar object handles an entire series of data, and a Bars object handles a bar chart plot, so a single plot with two data series on it will be handled by one Bars object and two Bar objects.
+- Pie. Pie charts cannot show multiple data series so this subclass does not have a correspondence to Line or Bar. This takes in all the arguments that the matplotlib `pie` function takes in, and also any of the arguments from the parent class, Plot.
+- Colormesh. This shows a single data series with two dimensional input and one dimensional output. It takes in almost all of the arguments that the matplotlib pcolormesh function takes in and uses pcolormesh instead of pcolor.
+- Surface. This shows a single data series with a two dimensional input and a one dimensional output. Different from Colormesh, this produces a plot in three spatial dimensions represented as a surface. Wireframe and 3D contour plotting is also supported by passing in "plot_wireframe" or "contour" as a value of the `plot_type` keyword
+
+### Usage
+
+The first step in creating a figure is specifying the data. Here is an example with plotting a single line on a graph. `lines_obj` is the Data object in this case, and we pass it in to `create_figures`.
+    
+    # Importing
+    import numpy as np
+    from hgutilities import plotting
+
+    # Creation of Line object
+    x_values = np.arange(0, 2*np.pi, 0.1)
+    y_values = np.sin(x_values)
+    line_obj = plotting.line(x_values, y_values)
+
+    # Creation of Lines object
+    lines_obj = plotting.lines(line_obj)
+
+    # Creation of figures
+    plotting.create_figures(lines_obj)
+
+If we want to create multiple lines, we can pass in a list of line objects. We can also give our figure some labels.
+
+
+    # Importing
+    import numpy as np
+    from hgutilities import plotting
+
+    # Creation of Line object
+    def get_line_obj(n):
+        y_values = np.sin(n*x_values)
+        label = f"n = {n}"
+        line_obj = plotting.line(x_values, y_values, label=label)
+        return line_obj
+
+    x_values = np.arange(0, 2*np.pi, 0.01)
+    x_coefficients = [1, 2, 3]
+    line_objects = [get_line_obj(n) for n in x_coefficients]
+
+    # Creation of Lines object
+    title = "Sin(nx)"
+    x_label = "My x axis label"
+    y_label = "My y axis label"
+    lines_obj = plotting.lines(line_objects, title=title, legend=True,
+                                  x_label=x_label, y_label=y_label)
+
+    # Creation of figures
+    plotting.create_figures(lines_obj)
+
+We could have data split across multiple subplots. By default we have `subplots=None` and all subplots will be put on a figure. If subplots is specified and the subplots do not fit on one figure, they will be distributed across multiple. The subplots will be evenly distributed over $\left \lfloor \frac{\text{total subplots}}{\text{subplots per figure}} \right \rfloor$ figures, so the number of subplots per figure is at least as big as the number specified. In future versions this behaviour will change, and the number given by the subplots keyword will be an upper bound on how many subplots there will be on a given figure, and the number of figures will be as small as possible given that constraint.
+
+    # Importing
+    import numpy as np
+    from hgutilities import plotting
+
+    def get_lines_obj(n):
+        line_obj = get_line_obj(n)
+        title = f"Sin({n}x)"
+        x_label = "My x axis label"
+        y_label = "My y axis label"
+        lines_obj = plotting.lines(line_obj, title=title,
+        x_label=x_label, y_label=y_label)
+        return lines_obj
+
+    def get_line_obj(n):
+        y_values = np.sin(n*x_values)
+        line_obj = plotting.line(x_values, y_values)
+        return line_obj
+
+    # Creation of lines objects
+    x_values = np.arange(0, 2*np.pi, 0.01)
+    x_coefficients = list(range(1, 13))
+    lines_objects = [get_lines_obj(n) for n in x_coefficients]
+
+    # Creation of figures
+    plotting.create_figures(lines_objects, subplots=6)
+
+You can mix the types of plot within a figure. Here is an example that shows the other types of plot supported.
+
+    # Importing
+    import numpy as np
+    from hgutilities import plotting
+
+    # Creating bars object
+    x_values_1 = ["Red", "Green", "Blue"]
+    y_values_1 = [4, 2, 7]
+    bar_obj_1 = plotting.bar(x_values_1, y_values_1)
+
+    x_values_2 = ["Green", "Red", "Blue"]
+    y_values_2 = [1, 4, 5]
+    bar_obj_2 = plotting.bar(x_values_2, y_values_2)
+
+    title = "Bar Chart Example"
+    bar_objects = [bar_obj_1, bar_obj_2]
+    bars_obj = plotting.bars(bar_objects, title=title)
+
+    # Creating pie object
+    values = [4, 2, 7]
+    labels = ["Red", "Green", "Blue"]
+    title = "Pie Chart Example"
+    pie_obj = plotting.pie(values, labels, title=title,
+                           colors=labels, test=False)
+
+    # Creating surface object
+    x_values = np.arange(0, 10, 0.01)
+    y_values = np.arange(0, 10, 0.01)
+    x_mesh, y_mesh = np.meshgrid(x_values, y_values)
+    z_mesh = np.cos(x_mesh) + np.cos(y_mesh)
+    title = "Surface Plot Example"
+    surface_obj = plotting.surface(x_mesh, y_mesh, z_mesh,
+                                   title=title)
+
+    # Creating colorplot object
+    title = "Colorplot Example"
+    colormap_obj = plotting.colorplot(x_mesh, y_mesh, z_mesh,
+                                      title=title)
+
+    # Creation of figures
+    data_objects = [bars_obj, pie_obj, surface_obj, colormap_obj]
+    plotting.create_figures(data_objects)
+
+Animations can also be made by adding a dimension to the dependent variable. Currently this is only implemented for Surface objects. We note that all matplotlib figure objects need to be kept open while making the animation, so this is only suitable for short animations.
+
+    # Importing
+    import numpy as np
+    from hgutilities import plotting
+
+    # Set independent variable values
+    x_values = np.arange(0, 10, 0.5)
+    y_values = np.arange(0, 10, 0.5)
+    x_mesh, y_mesh = np.meshgrid(x_values, y_values)
+
+    # Set dependent variable values
+    def get_z_mesh_layer(time_value):
+        time_mesh = np.ones(x_mesh.shape) * time_value
+        z_mesh_layer = (np.sin(x_mesh + time_mesh)
+                        + np.sin(y_mesh + time_mesh))
+        return z_mesh_layer
+
+    time_values = np.arange(0, 2*np.pi, 0.5)
+    z_meshes = [get_z_mesh_layer(time_value)
+                for time_value in time_values]
+    z_meshes = np.stack(z_meshes)
+
+    # Creating animation
+    surface_obj = plotting.surface(x_mesh, y_mesh, z_meshes)
+    surface_objects = [surface_obj]
+    plotting.create_animations(surface_objects)
+
+## Features
+
+### Universal Legend
+
+The universal legend is a tool that can be used if all subplots in a figure have the same legend. An extra blank subplot is created and the space is used to show a legend that corresponds to all plots. This can be activated by passing `universal_legend=True` as a keyword-value pair into the `create_figures` function, and any individual legends will be overruled. Exception handling not implemented, will crash or get unexpected results if not used properly.
+
+### Subplot Adjustment
+
 Note: this feature has not been implemented yet. If the optional keyword argument, `adjust_subplots=True` is passed in to `create_figures` (or `create_animation`), then the matplotlib subplot adjustment tool will appear when the figures are created. The subplots are usually plotted with using the constrained layout, but in this case that will be turned off and tight layout used instead.
```

### Comparing `hgutilities-1.0.5/hgutilities/plotting/__init__.py` & `hgutilities-1.0.6/hgutilities/plotting/__init__.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,34 +1,34 @@
-from ..defaults import docs
-
-# Functions and classes to be accessed by the user
-from .plotfunctions import create_figures
-from .plotfunctions import create_animations
-from .datatypes.line import Line as line
-from .datatypes.lines import Lines as lines
-from .datatypes.bars import Bars as bars
-from .datatypes.bar import Bar as bar
-from .datatypes.pie import Pie as pie
-from .datatypes.surface import Surface as surface
-from .datatypes.colorplot import Colorplot as colorplot
-
-# Classes that need initialisation
-from .figure import Figure
-from .plottypes.plotlines import PlotLines
-from .plottypes.plotbars import PlotBars
-from .plottypes.plotpie import PlotPie
-from .plottypes.plotsurface import PlotSurface
-from .plottypes.plotcolorplot import PlotColorplot
-
-# Initialising classes
-Figure.set_plot_classes()
-PlotLines.set_function_dict()
-PlotBars.set_function_dict()
-PlotPie.set_function_dict()
-PlotSurface.set_function_dict()
-PlotColorplot.set_function_dict()
-
-# Importing other classes that have documentation
-# files so they can be detected by defaults.doc
-from .animate import Animate
-
-docs()
+from ..defaults import docs
+
+# Functions and classes to be accessed by the user
+from .plotfunctions import create_figures
+from .plotfunctions import create_animations
+from .datatypes.line import Line as line
+from .datatypes.lines import Lines as lines
+from .datatypes.bars import Bars as bars
+from .datatypes.bar import Bar as bar
+from .datatypes.pie import Pie as pie
+from .datatypes.surface import Surface as surface
+from .datatypes.colorplot import Colorplot as colorplot
+
+# Classes that need initialisation
+from .figure import Figure
+from .plottypes.plotlines import PlotLines
+from .plottypes.plotbars import PlotBars
+from .plottypes.plotpie import PlotPie
+from .plottypes.plotsurface import PlotSurface
+from .plottypes.plotcolorplot import PlotColorplot
+
+# Initialising classes
+Figure.set_plot_classes()
+PlotLines.set_function_dict()
+PlotBars.set_function_dict()
+PlotPie.set_function_dict()
+PlotSurface.set_function_dict()
+PlotColorplot.set_function_dict()
+
+# Importing other classes that have documentation
+# files so they can be detected by defaults.doc
+from .animate import Animate
+
+docs()
```

### Comparing `hgutilities-1.0.5/hgutilities/plotting/animate.py` & `hgutilities-1.0.6/hgutilities/plotting/animate.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,78 +1,78 @@
-import PIL
-import io
-
-from matplotlib.pyplot import savefig
-from matplotlib.pyplot import show
-
-from .figures import Figures
-from .. import defaults
-
-class Animate(Figures):
-    
-    def __init__(self, data_objects, **kwargs):
-        Figures.__init__(self, data_objects, **kwargs)
-        defaults.kwargs(self, kwargs)
-    
-    def create_animations(self, **kwargs):
-        self.process_data_objects()
-        self.set_figure_objects(**kwargs)
-        self.prepare_animation_settings()
-        self.animate_data_objects()
-
-    def prepare_animation_settings(self):
-        self.output = None
-        self.set_animation_axis_limits()
-        self.set_figure_animation_settings()
-
-    def set_animation_axis_limits(self):
-        for figure_obj in self.figure_objects:
-            figure_obj.set_animation_axis_limits()
-
-    def set_figure_animation_settings(self):
-        for figure_obj in self.figure_objects:
-            figure_obj.maximise = self.maximise
-            figure_obj.figure_size = self.figure_size
-
-    def animate_data_objects(self):
-        for figure_obj in self.figure_objects:
-            self.animate_figure(figure_obj)
-
-    def animate_figure(self, figure_obj):
-        frame_count = figure_obj.get_frame_count()
-        self.set_all_data_values(figure_obj)
-        frames = self.get_frames(figure_obj, frame_count)
-        self.save_animation(frames)
-
-    def set_all_data_values(self, figure_obj):
-        figure_obj.all_data_values = [data_obj.get_data_values()
-                                      for data_obj in figure_obj.data_objects]
-
-    def get_frames(self, figure_obj, frame_count):
-        frames = [self.get_frame(figure_obj, index)
-                  for index in range(frame_count)]
-        return frames
-
-    def get_frame(self, figure_obj, index):
-        buffer = self.get_buffer(figure_obj, index)
-        image = self.get_image(buffer, figure_obj)
-        return image
-
-    def get_buffer(self, figure_obj, index):
-        figure_obj.set_data_value(index)
-        figure_obj.create_figure()
-        buffer = io.BytesIO()
-        return buffer
-
-    def get_image(self, buffer, figure_obj):
-        savefig(buffer, dpi=figure_obj.fig.dpi)
-        buffer.seek(0)
-        image = PIL.Image.open(buffer)
-        image = image.resize(figure_obj.figure_size_pixels)
-        return image
-
-    def save_animation(self, frames):
-        animation_path = f"{self.animation_name}.{self.format}"
-        frames[0].save(animation_path, loop=self.loop, save_all=True,
-                       append_images=frames[1:], duration=self.duration)
-
-defaults.load(Animate)
+import PIL
+import io
+
+from matplotlib.pyplot import savefig
+from matplotlib.pyplot import show
+
+from .figures import Figures
+from .. import defaults
+
+class Animate(Figures):
+    
+    def __init__(self, data_objects, **kwargs):
+        Figures.__init__(self, data_objects, **kwargs)
+        defaults.kwargs(self, kwargs)
+    
+    def create_animations(self, **kwargs):
+        self.process_data_objects()
+        self.set_figure_objects(**kwargs)
+        self.prepare_animation_settings()
+        self.animate_data_objects()
+
+    def prepare_animation_settings(self):
+        self.output = None
+        self.set_animation_axis_limits()
+        self.set_figure_animation_settings()
+
+    def set_animation_axis_limits(self):
+        for figure_obj in self.figure_objects:
+            figure_obj.set_animation_axis_limits()
+
+    def set_figure_animation_settings(self):
+        for figure_obj in self.figure_objects:
+            figure_obj.maximise = self.maximise
+            figure_obj.figure_size = self.figure_size
+
+    def animate_data_objects(self):
+        for figure_obj in self.figure_objects:
+            self.animate_figure(figure_obj)
+
+    def animate_figure(self, figure_obj):
+        frame_count = figure_obj.get_frame_count()
+        self.set_all_data_values(figure_obj)
+        frames = self.get_frames(figure_obj, frame_count)
+        self.save_animation(frames)
+
+    def set_all_data_values(self, figure_obj):
+        figure_obj.all_data_values = [data_obj.get_data_values()
+                                      for data_obj in figure_obj.data_objects]
+
+    def get_frames(self, figure_obj, frame_count):
+        frames = [self.get_frame(figure_obj, index)
+                  for index in range(frame_count)]
+        return frames
+
+    def get_frame(self, figure_obj, index):
+        buffer = self.get_buffer(figure_obj, index)
+        image = self.get_image(buffer, figure_obj)
+        return image
+
+    def get_buffer(self, figure_obj, index):
+        figure_obj.set_data_value(index)
+        figure_obj.create_figure()
+        buffer = io.BytesIO()
+        return buffer
+
+    def get_image(self, buffer, figure_obj):
+        savefig(buffer, dpi=figure_obj.fig.dpi)
+        buffer.seek(0)
+        image = PIL.Image.open(buffer)
+        image = image.resize(figure_obj.figure_size_pixels)
+        return image
+
+    def save_animation(self, frames):
+        animation_path = f"{self.animation_name}.{self.format}"
+        frames[0].save(animation_path, loop=self.loop, save_all=True,
+                       append_images=frames[1:], duration=self.duration)
+
+defaults.load(Animate)
```

### Comparing `hgutilities-1.0.5/hgutilities/plotting/datatypes/Default Settings/Colorplot.txt` & `hgutilities-1.0.6/hgutilities/plotting/datatypes/Default Settings/Line.txt`

 * *Files 27% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.2753623188405797%*

 * *Differences: {"'barsabove'": 'None',*

 * * "'capsize'": 'None',*

 * * "'capthick'": 'None',*

 * * "'cmap'": 'None',*

 * * "'dash_capstyle'": 'None',*

 * * "'dash_joinstyle'": 'None',*

 * * "'dashes'": '[None, None]',*

 * * "'drawstyle'": 'None',*

 * * "'ecolor'": 'None',*

 * * "'elinewidth'": 'None',*

 * * "'errorever'": 'None',*

 * * "'fillstyle'": 'None',*

 * * "'gapcolor'": 'None',*

 * * "'in_layout'": 'None',*

 * * "'linestyle'": 'None',*

 * * "'linwidths'": 'None',*

 * * "'lolims'": 'None',*

 * * "'marker'": 'None',*

 * * "'markeredgecolor'": 'None',*

 * * "'markeredgewidth'": 'None',*

 * * "'markerfacecolor'": ' […]*

```diff
@@ -1,39 +1,57 @@
 {
     "agg_filter": null,
     "alpha": null,
-    "animated": null,
     "antialiased": null,
-    "capstyle": null,
-    "clip_box": null,
-    "clip_on": null,
-    "clip_path": null,
-    "cmap": "viridis",
+    "barsabove": null,
+    "capsize": null,
+    "capthick": null,
+    "cmap": null,
     "color": null,
-    "colors": null,
-    "edgecolor": null,
+    "dash_capstyle": null,
+    "dash_joinstyle": null,
+    "dashes": [
+        null,
+        null
+    ],
+    "drawstyle": null,
+    "ecolor": null,
     "edgecolors": null,
-    "facecolor": null,
+    "elinewidth": null,
+    "errorever": null,
+    "fillstyle": null,
+    "gapcolor": null,
     "gid": null,
-    "hatch": null,
-    "joinstyle": null,
+    "in_layout": null,
     "label": null,
-    "linestyle": "-",
+    "linestyle": null,
     "linewidth": null,
+    "linwidths": null,
+    "lolims": null,
+    "marker": null,
+    "markeredgecolor": null,
+    "markeredgewidth": null,
+    "markerfacecolor": null,
+    "markerfacecoloralt": null,
+    "markersize": null,
+    "markevery": null,
     "mouseover": null,
     "norm": null,
-    "offsets": null,
     "path_effects": null,
+    "plotnonfinite": null,
     "rasterized": null,
-    "shade": false,
-    "shading": null,
+    "sketch_params": null,
     "snap": null,
+    "solid_capstyle": null,
+    "solid_joinstyle": null,
+    "transform": null,
+    "uplims": null,
     "url": null,
     "visible": true,
     "vmax": null,
     "vmin": null,
-    "x": null,
-    "x_label": null,
-    "y": null,
-    "y_label": null,
+    "xerr": null,
+    "xlolims": null,
+    "xuplims": null,
+    "yerr": null,
     "zorder": null
 }
```

### Comparing `hgutilities-1.0.5/hgutilities/plotting/datatypes/Documentation/Bar.txt` & `hgutilities-1.0.6/hgutilities/plotting/datatypes/Documentation/Bar.txt`

 * *Ordering differences only*

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-Contains information about a single data series on a bar chart.
-Anything that affects the entire chart should be specied upon creation
-of Bars objects. Almost all features of matplotlib bar charts are
-supported, and the key-word arguments are the same. Care must be
-taken to enter the key-word arguments in relevant object (Bars
-properties not entered into Bar properties and vice versa).
-
-Bar.defaults shows a list of optional kwargs.
-
-For further documentation see the following:
-https://github.com/HenryGinn/hgutilities
-https://github.com/HenryGinn/hgutilities/tree/main/hgutilities/plotting
-https://matplotlib.org/stable/api/_as_gen/matplotlib.pyplot.bar.html
+Contains information about a single data series on a bar chart.
+Anything that affects the entire chart should be specied upon creation
+of Bars objects. Almost all features of matplotlib bar charts are
+supported, and the key-word arguments are the same. Care must be
+taken to enter the key-word arguments in relevant object (Bars
+properties not entered into Bar properties and vice versa).
+
+Bar.defaults shows a list of optional kwargs.
+
+For further documentation see the following:
+https://github.com/HenryGinn/hgutilities
+https://github.com/HenryGinn/hgutilities/tree/main/hgutilities/plotting
+https://matplotlib.org/stable/api/_as_gen/matplotlib.pyplot.bar.html
```

### Comparing `hgutilities-1.0.5/hgutilities/plotting/datatypes/Documentation/Bars.txt` & `hgutilities-1.0.6/hgutilities/plotting/datatypes/Documentation/Bars.txt`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-This is a subclass of Data used to create bar charts.
-It takes in a bar object, or an iterable of bar objects,
-and keyword arguments thar are relevant only to the entire
-plot. If you wanted every data series to be the same color,
-you would need to specify that for each bar object, but if
-you wanted a log scale, you would specify that at this level.
-If it does not make sense for two distinct data series to
-have different values for a property, then it should be a
-property of this object. For more detail, look at the
-default values for Bars and Bar objects.
-
-Bars.defaults shows a list of optional kwargs.
-
-For further documentation see the following:
-Bar, Data, and Figures classes
-https://github.com/HenryGinn/hgutilities
-https://github.com/HenryGinn/hgutilities/tree/main/hgutilities/plotting
-https://matplotlib.org/stable/api/_as_gen/matplotlib.pyplot.bar.html
+This is a subclass of Data used to create bar charts.
+It takes in a bar object, or an iterable of bar objects,
+and keyword arguments thar are relevant only to the entire
+plot. If you wanted every data series to be the same color,
+you would need to specify that for each bar object, but if
+you wanted a log scale, you would specify that at this level.
+If it does not make sense for two distinct data series to
+have different values for a property, then it should be a
+property of this object. For more detail, look at the
+default values for Bars and Bar objects.
+
+Bars.defaults shows a list of optional kwargs.
+
+For further documentation see the following:
+Bar, Data, and Figures classes
+https://github.com/HenryGinn/hgutilities
+https://github.com/HenryGinn/hgutilities/tree/main/hgutilities/plotting
+https://matplotlib.org/stable/api/_as_gen/matplotlib.pyplot.bar.html
```

### Comparing `hgutilities-1.0.5/hgutilities/plotting/datatypes/Documentation/Line.txt` & `hgutilities-1.0.6/hgutilities/plotting/datatypes/Documentation/Line.txt`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-Contains information about a single data series
-on a line or scatter graph. Anything that affects
-the entire chart should be specified upon creation
-of Lines objects. Properties such as line color,
-line style, line thickness, and errors in x or y
-should be specified here.If a line is given a label
-then this label will be used in the chart legend.
-
-Line.defaults shows a list of optional kwargs.
-
-For further documentation see the following:
-Lines, Data, and Figures classes
-https://github.com/HenryGinn/hgutilities
-https://github.com/HenryGinn/hgutilities/tree/main/hgutilities/plotting
-https://matplotlib.org/stable/api/_as_gen/matplotlib.pyplot.plot.html
+Contains information about a single data series
+on a line or scatter graph. Anything that affects
+the entire chart should be specified upon creation
+of Lines objects. Properties such as line color,
+line style, line thickness, and errors in x or y
+should be specified here.If a line is given a label
+then this label will be used in the chart legend.
+
+Line.defaults shows a list of optional kwargs.
+
+For further documentation see the following:
+Lines, Data, and Figures classes
+https://github.com/HenryGinn/hgutilities
+https://github.com/HenryGinn/hgutilities/tree/main/hgutilities/plotting
+https://matplotlib.org/stable/api/_as_gen/matplotlib.pyplot.plot.html
```

### Comparing `hgutilities-1.0.5/hgutilities/plotting/datatypes/Documentation/Lines.txt` & `hgutilities-1.0.6/hgutilities/plotting/datatypes/Documentation/Lines.txt`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-This is used to create line and scatter graphs and takes in a Line
-object or an iterable of line objects. The scope of this object is the
-entire plot, and data about individual lines should be specified by
-Line objects. Properties such as whether the plot has a legend, what
-the title and axis labels are, and the plot type are relevant at this
-level. If it does not make sense for two distinct data series to have
-different values for a property, then it should be a property of this
-object. For more detail, look at the default values for Lines and Line objects.
-
-The plot_type key-word controls which matplotlib plotting function is
-used to create the plot. The options are "plot", "semilogx", "semilogy",
-"loglog", "scatter", and "errorbar". If values for xerr and yerr are
-given for any line object, this will not be detected. The keyword
-plot_type="errorbar" needs to be passed in explicitily.
-
-lines.defaults shows a list of optional kwargs.
-
-For further documentation see the following:
-Line, Data, and Figures classes
-https://github.com/HenryGinn/hgutilities
-https://github.com/HenryGinn/hgutilities/tree/main/hgutilities/plotting
-https://matplotlib.org/stable/api/_as_gen/matplotlib.pyplot.plot.html
+This is used to create line and scatter graphs and takes in a Line
+object or an iterable of line objects. The scope of this object is the
+entire plot, and data about individual lines should be specified by
+Line objects. Properties such as whether the plot has a legend, what
+the title and axis labels are, and the plot type are relevant at this
+level. If it does not make sense for two distinct data series to have
+different values for a property, then it should be a property of this
+object. For more detail, look at the default values for Lines and Line objects.
+
+The plot_type key-word controls which matplotlib plotting function is
+used to create the plot. The options are "plot", "semilogx", "semilogy",
+"loglog", "scatter", and "errorbar". If values for xerr and yerr are
+given for any line object, this will not be detected. The keyword
+plot_type="errorbar" needs to be passed in explicitily.
+
+lines.defaults shows a list of optional kwargs.
+
+For further documentation see the following:
+Line, Data, and Figures classes
+https://github.com/HenryGinn/hgutilities
+https://github.com/HenryGinn/hgutilities/tree/main/hgutilities/plotting
+https://matplotlib.org/stable/api/_as_gen/matplotlib.pyplot.plot.html
```

### Comparing `hgutilities-1.0.5/hgutilities/plotting/datatypes/Documentation/Pie.txt` & `hgutilities-1.0.6/hgutilities/plotting/datatypes/Documentation/Pie.txt`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-This is a Data subclass used to create pie charts. A pie chart can only
-display one data series, and so this takes in a list of values and
-labels directly unlike the Lines and Bars classes. Almost all
-matplotlib pie chart keyword arguments are accepted, and information
-about the plot legend should also be passed in, either upon creation
-or set directly.
-
-Pie.defaults shows a list of optional kwargs.
-
-For further documentation see the following:
-Data and Figures classes
-https://github.com/HenryGinn/hgutilities
-https://github.com/HenryGinn/hgutilities/tree/main/hgutilities/plotting
-https://matplotlib.org/stable/api/_as_gen/matplotlib.pyplot.pie.html
+This is a Data subclass used to create pie charts. A pie chart can only
+display one data series, and so this takes in a list of values and
+labels directly unlike the Lines and Bars classes. Almost all
+matplotlib pie chart keyword arguments are accepted, and information
+about the plot legend should also be passed in, either upon creation
+or set directly.
+
+Pie.defaults shows a list of optional kwargs.
+
+For further documentation see the following:
+Data and Figures classes
+https://github.com/HenryGinn/hgutilities
+https://github.com/HenryGinn/hgutilities/tree/main/hgutilities/plotting
+https://matplotlib.org/stable/api/_as_gen/matplotlib.pyplot.pie.html
```

### Comparing `hgutilities-1.0.5/hgutilities/plotting/datatypes/Documentation/Surface.txt` & `hgutilities-1.0.6/hgutilities/plotting/datatypes/Documentation/Surface.txt`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-This is a Data subclass used to create surfaces in 3D. It takes in x, y, and z values, all of which are 2D arrays of the same shape. Only one data series can be shown on each plot. All keyword arguments are the same as the matplotlib keyword arguments. This accepts the following arguments for the plot_type keyword, all of which are the names of the corresponding matplotlib plotting function:
-
-plot_surface: standard surface plotter
-plot_wireframe: shows the surface as a wire frame
-contour: shows the level sets of a function
-
-Surface.defaults shows a list of optional kwargs.
-
-For further documentation see the following:
-Data and Figures classes
-https://github.com/HenryGinn/hgutilities
-https://github.com/HenryGinn/hgutilities/tree/main/hgutilities/plotting
-https://matplotlib.org/stable/api/_as_gen/mpl_toolkits.mplot3d.axes3d.Axes3D.plot_surface.html
+This is a Data subclass used to create surfaces in 3D. It takes in x, y, and z values, all of which are 2D arrays of the same shape. Only one data series can be shown on each plot. All keyword arguments are the same as the matplotlib keyword arguments. This accepts the following arguments for the plot_type keyword, all of which are the names of the corresponding matplotlib plotting function:
+
+plot_surface: standard surface plotter
+plot_wireframe: shows the surface as a wire frame
+contour: shows the level sets of a function
+
+Surface.defaults shows a list of optional kwargs.
+
+For further documentation see the following:
+Data and Figures classes
+https://github.com/HenryGinn/hgutilities
+https://github.com/HenryGinn/hgutilities/tree/main/hgutilities/plotting
+https://matplotlib.org/stable/api/_as_gen/mpl_toolkits.mplot3d.axes3d.Axes3D.plot_surface.html
```

### Comparing `hgutilities-1.0.5/hgutilities/plotting/datatypes/bars.py` & `hgutilities-1.0.6/hgutilities/plotting/datatypes/bars.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,33 +1,33 @@
-import numpy as np
-
-from ... import defaults
-from .data import Data
-from .bar import Bar
-
-class Bars(Data):
-
-    def __init__(self, bar_objects, **kwargs):
-        Data.__init__(self, **kwargs)
-        defaults.kwargs(self, kwargs)
-        self.set_bar_objects(bar_objects)
-
-    def set_bar_objects(self, bar_objects):
-        if isinstance(bar_objects, Bar):
-            self.bar_objects = [bar_objects]
-        else:
-            self.set_bar_objects_multiple(bar_objects)
-
-    def set_bar_objects_multiple(self, bar_objects):
-        if np.all([isinstance(bar_obj, Bar)
-                   for bar_obj in bar_objects]):
-            self.bar_objects = list(bar_objects)
-        else:
-            self.bad_data_objects_exception()
-
-    def bad_data_objects_exception(self):
-        message = ("When creating a bars object you must pass "
-                   "in an instance of bar or an iterable of "
-                   "instances of bar")
-        raise TypeError(message)
-
-defaults.load(Bars)
+import numpy as np
+
+from ... import defaults
+from .data import Data
+from .bar import Bar
+
+class Bars(Data):
+
+    def __init__(self, bar_objects, **kwargs):
+        Data.__init__(self, **kwargs)
+        defaults.kwargs(self, kwargs)
+        self.set_bar_objects(bar_objects)
+
+    def set_bar_objects(self, bar_objects):
+        if isinstance(bar_objects, Bar):
+            self.bar_objects = [bar_objects]
+        else:
+            self.set_bar_objects_multiple(bar_objects)
+
+    def set_bar_objects_multiple(self, bar_objects):
+        if np.all([isinstance(bar_obj, Bar)
+                   for bar_obj in bar_objects]):
+            self.bar_objects = list(bar_objects)
+        else:
+            self.bad_data_objects_exception()
+
+    def bad_data_objects_exception(self):
+        message = ("When creating a bars object you must pass "
+                   "in an instance of bar or an iterable of "
+                   "instances of bar")
+        raise TypeError(message)
+
+defaults.load(Bars)
```

### Comparing `hgutilities-1.0.5/hgutilities/plotting/datatypes/surface.py` & `hgutilities-1.0.6/hgutilities/plotting/datatypes/surface.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,35 +1,35 @@
-import numpy as np
-
-from ... import defaults
-from .data import Data
-
-class Surface(Data):
-
-    def __init__(self, x_values, y_values, z_values, **kwargs):
-        Data.__init__(self, **kwargs)
-        self.set_xyz_values(x_values, y_values, z_values)
-        defaults.kwargs(self, kwargs)
-
-    def set_xyz_values(self, x_values, y_values, z_values):
-        self.x_values = x_values
-        self.y_values = y_values
-        self.z_values = z_values
-
-    def set_animation_axis_limits(self):
-        max_z = np.max(self.z_values)
-        min_z = np.min(self.z_values)
-        self.z_limits = [min_z, max_z]
-
-    def get_frame_count(self):
-        if len(self.z_values.shape) == 3:
-            return self.z_values.shape[0]
-        else:
-            raise ValueError("z_values needs 3 dimensions to animate")
-
-    def get_data_values(self):
-        return np.copy(self.z_values)
-
-    def set_data_value(self, data_value):
-        self.z_values = data_value
-
-defaults.load(Surface)
+import numpy as np
+
+from ... import defaults
+from .data import Data
+
+class Surface(Data):
+
+    def __init__(self, x_values, y_values, z_values, **kwargs):
+        Data.__init__(self, **kwargs)
+        self.set_xyz_values(x_values, y_values, z_values)
+        defaults.kwargs(self, kwargs)
+
+    def set_xyz_values(self, x_values, y_values, z_values):
+        self.x_values = x_values
+        self.y_values = y_values
+        self.z_values = z_values
+
+    def set_animation_axis_limits(self):
+        max_z = np.max(self.z_values)
+        min_z = np.min(self.z_values)
+        self.z_limits = [min_z, max_z]
+
+    def get_frame_count(self):
+        if len(self.z_values.shape) == 3:
+            return self.z_values.shape[0]
+        else:
+            raise ValueError("z_values needs 3 dimensions to animate")
+
+    def get_data_values(self):
+        return np.copy(self.z_values)
+
+    def set_data_value(self, data_value):
+        self.z_values = data_value
+
+defaults.load(Surface)
```

### Comparing `hgutilities-1.0.5/hgutilities/plotting/figure.py` & `hgutilities-1.0.6/hgutilities/plotting/figure.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,156 +1,160 @@
-import os
-import math
-from screeninfo import get_monitors
-
-import matplotlib.pyplot as plt
-import numpy as np
-
-from .. import defaults
-from .plottypes.plotlines import PlotLines
-from .plottypes.plotbars import PlotBars
-from .plottypes.plotpie import PlotPie
-from .plottypes.plotcolorplot import PlotColorplot
-from .plottypes.plotsurface import PlotSurface
-from .plotutils.griddimensions import get_grid_dimensions
-from .plotutils.savefigure import save_figure
-from .plotutils.figuresize import maximise_figure
-
-class Figure():
-    
-    @classmethod
-    def set_plot_classes(cls):
-        cls.plot_classes = {"Lines": PlotLines,
-                            "Bars": PlotBars,
-                            "Pie": PlotPie,
-                            "Colorplot": PlotColorplot,
-                            "Surface": PlotSurface}
-    
-    def __init__(self, figures_obj, data_objects, plot_index, **kwargs):
-        defaults.kwargs(self, kwargs)
-        self.figures_obj = figures_obj
-        self.plot_index = plot_index
-        self.initialise_data_objects(data_objects)
-        self.set_grid_size()
-        self.process_light_or_dark()
-
-    def process_light_or_dark(self):
-        if self.dark:
-            plt.style.use('dark_background')
-
-    def initialise_data_objects(self, data_objects):
-        self.data_objects = data_objects
-        self.count = len(data_objects)
-        if self.figures_obj.universal_legend:
-            self.count += 1
-
-    def set_grid_size(self):
-        aspect_ratio = self.figures_obj.aspect_ratio
-        self.rows, self.columns = get_grid_dimensions(self.count, aspect_ratio)
-
-    def create_figure(self):
-        self.initialise_figure()
-        self.create_plots()
-        self.add_figure_peripherals()
-        self.output_figure()
-
-    def initialise_figure(self):
-        self.set_figure()
-        self.create_axes()
-        self.remove_extra_axes()
-
-    def set_figure(self):
-        self.fig = plt.figure(constrained_layout=True, dpi=self.dpi)
-        self.fig.set_constrained_layout_pads(w_pad=self.w_pad, h_pad=self.h_pad,
-                                             hspace=self.hspace, wspace=self.wspace)
-
-    def create_axes(self):
-        self.axes = [self.get_axis(index, data_obj)
-                     for index, data_obj in enumerate(self.data_objects)]
-
-    def get_axis(self, index, data_obj):
-        axis = self.fig.add_subplot(self.rows, self.columns, index + 1,
-                                    projection=data_obj.projection)
-        return axis
-    
-    def remove_extra_axes(self):
-        extra_axes_count = len(self.axes) - self.count
-        for ax, _ in zip(self.axes[::-1], range(extra_axes_count)):
-            ax.remove()
-
-    def add_figure_peripherals(self):
-        self.set_suptitle()
-        self.set_universal_legend()
-        self.set_figure_size()
-
-    def set_suptitle(self):
-        if self.figures_obj.title is not None:
-            self.fig.suptitle(f"{self.figures_obj.title}")
-
-    def set_universal_legend(self):
-        if self.figures_obj.universal_legend:
-            self.do_universal_legend()
-
-    def do_universal_legend(self):
-        ax = self.axes[-1]
-        for data_obj in self.data_objects[0].data_objects:
-            ax.plot(1, 1, label=data_obj.label, color=data_obj.colour)
-        ax.legend(loc="center", borderpad=2, labelspacing=1)
-        ax.axis("off")
-
-    def set_figure_size(self):
-        self.update_size()
-        self.set_figure_size_pixels()
-
-    def update_size(self):
-        if self.maximise:
-            self.maximise_figure()
-        self.set_figure_inches()
-
-    def maximise_figure(self):
-        maximise_figure()
-        monitor = get_monitors()[0]
-        figure_size = [monitor.width_mm / 25.4, monitor.height_mm / 25.4]
-        self.figure_size = figure_size
-
-    def set_figure_inches(self):
-        if self.figure_size is not None:
-            self.fig.set_size_inches(self.figure_size)
-
-    def set_figure_size_pixels(self):
-        self.figure_size_pixels = self.fig.get_size_inches()*self.fig.dpi
-        self.figure_size_pixels = [int(value) for value in self.figure_size_pixels]
-
-    def create_plots(self):
-        self.plot_objects = [self.create_plot_obj(ax, data_obj)
-                             for ax, data_obj in zip(self.axes, self.data_objects)]
-
-    def create_plot_obj(self, ax, data_obj):
-        plot_class = self.plot_classes[data_obj.__class__.__name__]
-        plot_obj = plot_class(self, ax, data_obj)
-        plot_obj.create_plot()
-        return plot_obj
-    
-    def output_figure(self):
-        if self.figures_obj.output == "Show":
-            self.show_figure()
-        elif self.figures_obj.output == "Save":
-            save_figure(self)
-
-    def show_figure(self):
-        plt.show()
-        plt.close()
-
-    def set_animation_axis_limits(self):
-        for data_obj in self.data_objects:
-            data_obj.set_animation_axis_limits()
-
-    def get_frame_count(self):
-        frame_count = self.data_objects[0].get_frame_count()
-        return frame_count
-
-    def set_data_value(self, index):
-        for data_obj, data_values in zip(self.data_objects, self.all_data_values):
-            data_value = data_values[index]
-            data_obj.set_data_value(data_value)
-
-defaults.load(Figure)
+import os
+import math
+from screeninfo import get_monitors
+
+import matplotlib.pyplot as plt
+import numpy as np
+
+from .. import defaults
+from .plottypes.plotlines import PlotLines
+from .plottypes.plotbars import PlotBars
+from .plottypes.plotpie import PlotPie
+from .plottypes.plotcolorplot import PlotColorplot
+from .plottypes.plotsurface import PlotSurface
+from .plotutils.griddimensions import get_grid_dimensions
+from .plotutils.savefigure import save_figure
+from .plotutils.figuresize import maximise_figure
+
+class Figure():
+    
+    @classmethod
+    def set_plot_classes(cls):
+        cls.plot_classes = {"Lines": PlotLines,
+                            "Bars": PlotBars,
+                            "Pie": PlotPie,
+                            "Colorplot": PlotColorplot,
+                            "Surface": PlotSurface}
+    
+    def __init__(self, figures_obj, data_objects, plot_index, **kwargs):
+        defaults.kwargs(self, kwargs)
+        self.figures_obj = figures_obj
+        self.plot_index = plot_index
+        self.initialise_data_objects(data_objects)
+        self.set_grid_size()
+        self.process_light_or_dark()
+
+    def process_light_or_dark(self):
+        if self.dark:
+            plt.style.use('dark_background')
+
+    def initialise_data_objects(self, data_objects):
+        self.data_objects = data_objects
+        self.count = len(data_objects)
+        if self.figures_obj.universal_legend:
+            self.count += 1
+
+    def set_grid_size(self):
+        aspect_ratio = self.figures_obj.aspect_ratio
+        self.rows, self.columns = get_grid_dimensions(self.count, aspect_ratio)
+
+    def create_figure(self):
+        self.initialise_figure()
+        self.create_plots()
+        self.add_figure_peripherals()
+        self.output_figure()
+
+    def initialise_figure(self):
+        self.set_figure()
+        self.create_axes()
+        self.remove_extra_axes()
+
+    def set_figure(self):
+        self.fig = plt.figure(constrained_layout=True, dpi=self.dpi)
+        self.fig.set_constrained_layout_pads(w_pad=self.w_pad, h_pad=self.h_pad,
+                                             hspace=self.hspace, wspace=self.wspace)
+
+    def create_axes(self):
+        self.axes = [self.get_axis(index, data_obj)
+                     for index, data_obj in enumerate(self.data_objects)]
+
+    def get_axis(self, index, data_obj):
+        axis = self.fig.add_subplot(self.rows, self.columns, index + 1,
+                                    projection=data_obj.projection)
+        return axis
+    
+    def remove_extra_axes(self):
+        extra_axes_count = len(self.axes) - self.count
+        for ax, _ in zip(self.axes[::-1], range(extra_axes_count)):
+            ax.remove()
+
+    def add_figure_peripherals(self):
+        self.set_suptitle()
+        self.set_universal_legend()
+        self.set_figure_size()
+
+    def set_suptitle(self):
+        if self.figures_obj.title is not None:
+            self.fig.suptitle(f"{self.figures_obj.title}")
+
+    def set_universal_legend(self):
+        if self.figures_obj.universal_legend:
+            self.do_universal_legend()
+
+    def do_universal_legend(self):
+        ax = self.axes[-1]
+        for data_obj in self.data_objects[0].data_objects:
+            ax.plot(1, 1, label=data_obj.label, color=data_obj.colour)
+        ax.legend(loc="center", borderpad=2, labelspacing=1)
+        ax.axis("off")
+
+    def set_figure_size(self):
+        self.update_size()
+        self.set_figure_size_pixels()
+
+    def update_size(self):
+        self.set_maximised_figure_size()
+        self.set_figure_inches()
+        self.maximise_figure()
+
+    def set_maximised_figure_size(self):
+        if self.maximise:
+            monitor = get_monitors()[0]
+            figure_size = [monitor.width_mm / 25.4, monitor.height_mm / 25.4]
+            self.figure_size = figure_size
+
+    def maximise_figure(self):
+        if self.maximise:
+            maximise_figure()
+
+    def set_figure_inches(self):
+        if self.figure_size is not None:
+            self.fig.set_size_inches(self.figure_size)
+
+    def set_figure_size_pixels(self):
+        self.figure_size_pixels = self.fig.get_size_inches()*self.fig.dpi
+        self.figure_size_pixels = [int(value) for value in self.figure_size_pixels]
+
+    def create_plots(self):
+        self.plot_objects = [self.create_plot_obj(ax, data_obj)
+                             for ax, data_obj in zip(self.axes, self.data_objects)]
+
+    def create_plot_obj(self, ax, data_obj):
+        plot_class = self.plot_classes[data_obj.__class__.__name__]
+        plot_obj = plot_class(self, ax, data_obj)
+        plot_obj.create_plot()
+        return plot_obj
+    
+    def output_figure(self):
+        if self.figures_obj.output == "Show":
+            self.show_figure()
+        elif self.figures_obj.output == "Save":
+            save_figure(self)
+
+    def show_figure(self):
+        plt.show()
+        plt.close()
+
+    def set_animation_axis_limits(self):
+        for data_obj in self.data_objects:
+            data_obj.set_animation_axis_limits()
+
+    def get_frame_count(self):
+        frame_count = self.data_objects[0].get_frame_count()
+        return frame_count
+
+    def set_data_value(self, index):
+        for data_obj, data_values in zip(self.data_objects, self.all_data_values):
+            data_value = data_values[index]
+            data_obj.set_data_value(data_value)
+
+defaults.load(Figure)
```

### Comparing `hgutilities-1.0.5/hgutilities/plotting/figures.py` & `hgutilities-1.0.6/hgutilities/plotting/figures.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,71 +1,71 @@
-import os
-import __main__
-
-import numpy as np
-
-from .. import defaults
-from .figure import Figure
-from .datatypes.data import Data
-from ..utils.groups import get_group_indexes
-from ..utils.groups import get_group_size
-from ..utils.paths import make_folder
-
-class Figures():
-
-    def __init__(self, data_objects, **kwargs):
-        defaults.kwargs(self, **kwargs)
-        self.set_data_objects(data_objects)
-        self.data_obj_count = self.data_objects.size
-
-    def set_data_objects(self, data_objects):
-        if isinstance(data_objects, Data):
-            self.data_objects = np.array([data_objects])
-        else:
-            self.set_data_objects_multiple(data_objects)
-
-    def set_data_objects_multiple(self, data_objects):
-        if np.all([isinstance(data_obj, Data)
-                   for data_obj in data_objects]):
-            self.data_objects = np.array(data_objects)
-        else:
-            self.bad_data_objects_exception()
-
-    def bad_data_objects_exception(self):
-        message = ("When creating figure objects you must pass "
-                   "in an instance of Data or an iterable of "
-                   "instances of Data. If you are passing in "
-                   "Line/Bar objects, you need to create a "
-                   "Lines/Bars object to pass in instead")
-        raise TypeError(message)
-    
-    def create_figures(self, **kwargs):
-        self.process_data_objects()
-        self.process_output_mode()
-        self.plot_data_objects(**kwargs)
-
-    def process_output_mode(self):
-        if self.output == "Save":
-            self.create_plots_folder()
-
-    def create_plots_folder(self):
-        if self.path is None:
-            self.path = os.path.split(__main__.__file__)[0]
-        make_folder(self.path)
-
-    def process_data_objects(self):
-        self.subplots = get_group_size(self.subplots, self.data_objects)
-        group_indexes = get_group_indexes(self.data_obj_count, self.subplots)
-        self.data_object_groups = [self.data_objects[indexes]
-                                    for indexes in group_indexes]
-
-    def plot_data_objects(self, **kwargs):
-        self.set_figure_objects(**kwargs)
-        for figure_obj in self.figure_objects:
-            figure_obj.create_figure()
-
-    def set_figure_objects(self, **kwargs):
-        data_obj_iterable = enumerate(self.data_object_groups)
-        self.figure_objects = [Figure(self, data_object_group, index, **kwargs)
-                               for index, data_object_group in data_obj_iterable]
-
-defaults.load(Figures)
+import os
+import __main__
+
+import numpy as np
+
+from .. import defaults
+from .figure import Figure
+from .datatypes.data import Data
+from ..utils.groups import get_group_indexes
+from ..utils.groups import get_group_size
+from ..utils.paths import make_folder
+
+class Figures():
+
+    def __init__(self, data_objects, **kwargs):
+        defaults.kwargs(self, **kwargs)
+        self.set_data_objects(data_objects)
+        self.data_obj_count = self.data_objects.size
+
+    def set_data_objects(self, data_objects):
+        if isinstance(data_objects, Data):
+            self.data_objects = np.array([data_objects])
+        else:
+            self.set_data_objects_multiple(data_objects)
+
+    def set_data_objects_multiple(self, data_objects):
+        if np.all([isinstance(data_obj, Data)
+                   for data_obj in data_objects]):
+            self.data_objects = np.array(data_objects)
+        else:
+            self.bad_data_objects_exception()
+
+    def bad_data_objects_exception(self):
+        message = ("When creating figure objects you must pass "
+                   "in an instance of Data or an iterable of "
+                   "instances of Data. If you are passing in "
+                   "Line/Bar objects, you need to create a "
+                   "Lines/Bars object to pass in instead")
+        raise TypeError(message)
+    
+    def create_figures(self, **kwargs):
+        self.process_data_objects()
+        self.process_output_mode()
+        self.plot_data_objects(**kwargs)
+
+    def process_output_mode(self):
+        if self.output == "Save":
+            self.create_plots_folder()
+
+    def create_plots_folder(self):
+        if self.path is None:
+            self.path = os.path.split(__main__.__file__)[0]
+        make_folder(self.path)
+
+    def process_data_objects(self):
+        self.subplots = get_group_size(self.subplots, self.data_objects)
+        group_indexes = get_group_indexes(self.data_obj_count, self.subplots)
+        self.data_object_groups = [self.data_objects[indexes]
+                                    for indexes in group_indexes]
+
+    def plot_data_objects(self, **kwargs):
+        self.set_figure_objects(**kwargs)
+        for figure_obj in self.figure_objects:
+            figure_obj.create_figure()
+
+    def set_figure_objects(self, **kwargs):
+        data_obj_iterable = enumerate(self.data_object_groups)
+        self.figure_objects = [Figure(self, data_object_group, index, **kwargs)
+                               for index, data_object_group in data_obj_iterable]
+
+defaults.load(Figures)
```

### Comparing `hgutilities-1.0.5/hgutilities/plotting/plottypes/plot.py` & `hgutilities-1.0.6/hgutilities/plotting/plottypes/plot.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,92 +1,92 @@
-import matplotlib.pyplot as plt
-import matplotlib.font_manager
-import numpy as np
-
-from ... import defaults
-from ...utils.dicts import remove_none_values
-
-class Plot():
-
-    @classmethod
-    def set_function_dict(cls):
-        pass
-    
-    def __init__(self, figure_obj, ax, data_obj, **kwargs):
-        self.set_figure_obj(figure_obj)
-        self.ax = ax
-        self.data_obj = data_obj
-        defaults.kwargs(self, kwargs)
-        self.set_kwargs()
-
-    def set_kwargs(self):
-        self.inherit_kwargs()
-        self.set_font_kwargs()
-
-    def inherit_kwargs(self):
-        attributes = ["title_fontname", "title_fontsize",
-                      "title_color", "title_verticalalignment",
-                      "title_horizontalalignment", "title_y",
-                      "title_pad", "title_loc",
-                      "axis_fontname", "axis_fontsize",
-                      "axis_color", "axis_labelpad", "axis_loc",
-                      "x_axis_rotation", "y_axis_rotation", "z_axis_rotation"]
-        defaults.inherit(self.data_obj, self.figure_obj, attributes)
-        
-    def set_font_kwargs(self):
-        self.set_title_fontdict()
-        self.set_axis_fontdict()
-
-    def set_title_fontdict(self):
-        kwargs = {"fontname": self.data_obj.title_fontname,
-                  "fontsize": self.data_obj.title_fontsize,
-                  "color": self.data_obj.title_color,
-                  "verticalalignment": self.data_obj.title_verticalalignment,
-                  "horizontalalignment": self.data_obj.title_horizontalalignment}
-        self.title_fontdict = remove_none_values(kwargs)
-
-    def set_axis_fontdict(self):
-        kwargs = {"fontname": self.data_obj.axis_fontname,
-                  "fontsize": self.data_obj.axis_fontsize,
-                  "color": self.data_obj.axis_color}
-        self.axis_fontdict = remove_none_values(kwargs)
-
-    def set_figure_obj(self, figure_obj):
-        self.figure_obj = figure_obj
-        self.figures_obj = figure_obj.figures_obj
-
-    def create_plot(self):
-        self.plot_data()
-        self.set_title()
-        self.add_legend()
-        self.add_axis_labels()
-
-    def set_title(self):
-        if self.data_obj.title is not None:
-            self.ax.set_title(self.data_obj.title, **self.title_fontdict,
-                              loc=self.data_obj.title_loc, y=self.data_obj.title_y,
-                              pad=self.data_obj.title_pad)
-    
-    def add_legend(self):
-        if not self.figures_obj.universal_legend:
-            if self.data_obj.legend:
-                self.ax.legend(loc=self.data_obj.legend_loc)
-
-    def add_axis_labels(self):
-        pass
-
-    def add_x_label(self):
-        if self.data_obj.x_label is not None:
-            self.ax.set_xlabel(self.data_obj.x_label,
-                               **self.axis_fontdict)
-
-    def add_y_label(self):
-        if self.data_obj.y_label is not None:
-            self.ax.set_ylabel(self.data_obj.y_label,
-                               **self.axis_fontdict)
-
-    def add_z_label(self):
-        if self.data_obj.z_label is not None:
-            self.ax.set_zlabel(self.data_obj.z_label,
-                               **self.axis_fontdict)
-
-defaults.load(Plot)
+import matplotlib.pyplot as plt
+import matplotlib.font_manager
+import numpy as np
+
+from ... import defaults
+from ...utils.dicts import remove_none_values
+
+class Plot():
+
+    @classmethod
+    def set_function_dict(cls):
+        pass
+    
+    def __init__(self, figure_obj, ax, data_obj, **kwargs):
+        self.set_figure_obj(figure_obj)
+        self.ax = ax
+        self.data_obj = data_obj
+        defaults.kwargs(self, kwargs)
+        self.set_kwargs()
+
+    def set_kwargs(self):
+        self.inherit_kwargs()
+        self.set_font_kwargs()
+
+    def inherit_kwargs(self):
+        attributes = ["title_fontname", "title_fontsize",
+                      "title_color", "title_verticalalignment",
+                      "title_horizontalalignment", "title_y",
+                      "title_pad", "title_loc",
+                      "axis_fontname", "axis_fontsize",
+                      "axis_color", "axis_labelpad", "axis_loc",
+                      "x_axis_rotation", "y_axis_rotation", "z_axis_rotation"]
+        defaults.inherit(self.data_obj, self.figure_obj, attributes)
+        
+    def set_font_kwargs(self):
+        self.set_title_fontdict()
+        self.set_axis_fontdict()
+
+    def set_title_fontdict(self):
+        kwargs = {"fontname": self.data_obj.title_fontname,
+                  "fontsize": self.data_obj.title_fontsize,
+                  "color": self.data_obj.title_color,
+                  "verticalalignment": self.data_obj.title_verticalalignment,
+                  "horizontalalignment": self.data_obj.title_horizontalalignment}
+        self.title_fontdict = remove_none_values(kwargs)
+
+    def set_axis_fontdict(self):
+        kwargs = {"fontname": self.data_obj.axis_fontname,
+                  "fontsize": self.data_obj.axis_fontsize,
+                  "color": self.data_obj.axis_color}
+        self.axis_fontdict = remove_none_values(kwargs)
+
+    def set_figure_obj(self, figure_obj):
+        self.figure_obj = figure_obj
+        self.figures_obj = figure_obj.figures_obj
+
+    def create_plot(self):
+        self.plot_data()
+        self.set_title()
+        self.add_legend()
+        self.add_axis_labels()
+
+    def set_title(self):
+        if self.data_obj.title is not None:
+            self.ax.set_title(self.data_obj.title, **self.title_fontdict,
+                              loc=self.data_obj.title_loc, y=self.data_obj.title_y,
+                              pad=self.data_obj.title_pad)
+    
+    def add_legend(self):
+        if not self.figures_obj.universal_legend:
+            if self.data_obj.legend:
+                self.ax.legend(loc=self.data_obj.legend_loc)
+
+    def add_axis_labels(self):
+        pass
+
+    def add_x_label(self):
+        if self.data_obj.x_label is not None:
+            self.ax.set_xlabel(self.data_obj.x_label,
+                               **self.axis_fontdict)
+
+    def add_y_label(self):
+        if self.data_obj.y_label is not None:
+            self.ax.set_ylabel(self.data_obj.y_label,
+                               **self.axis_fontdict)
+
+    def add_z_label(self):
+        if self.data_obj.z_label is not None:
+            self.ax.set_zlabel(self.data_obj.z_label,
+                               **self.axis_fontdict)
+
+defaults.load(Plot)
```

### Comparing `hgutilities-1.0.5/hgutilities/plotting/plottypes/plotbars.py` & `hgutilities-1.0.6/hgutilities/plotting/plottypes/plotbars.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,90 +1,90 @@
-import matplotlib.pyplot as plt
-import numpy as np
-
-from ... import defaults
-from ..plottypes.plot import Plot
-
-class PlotBars(Plot):
-
-    def __init__(self, figure_obj, ax, bars_obj, **kwargs):
-        Plot.__init__(self, figure_obj, ax, bars_obj, **kwargs)
-        self.bars_obj = bars_obj
-        self.initialise_from_bars_obj()
-        defaults.kwargs(self, kwargs)
-
-    def initialise_from_bars_obj(self):
-        self.bar_objects = self.bars_obj.bar_objects
-        self.between_group_spacing = self.bars_obj.between_group_spacing
-        self.within_group_spacing = self.bars_obj.within_group_spacing
-
-    def plot_data(self):
-        self.preprocess_bars()
-        for index, bar_obj in enumerate(self.bars_obj.bar_objects):
-            self.plot_bar_obj(index, bar_obj)
-
-    def preprocess_bars(self):
-        self.group_width = 1 - self.between_group_spacing
-        self.set_bar_proportions()
-        self.x_offset = (self.between_group_spacing + self.bar_width - 1) / 2
-        self.set_x_axis_dictionary()
-        
-    def set_bar_proportions(self):
-        if len(self.bar_objects) == 1:
-            self.set_bar_proportions_single()
-        else:
-            self.set_proportions_multiple()
-
-    def set_bar_proportions_single(self):
-        self.bar_width = self.group_width
-        self.bar_space = self.group_width
-
-    def set_proportions_multiple(self):
-        n = len(self.bar_objects)
-        self.bar_width = self.group_width / (n + (n-1) * self.within_group_spacing)
-        self.bar_space = (self.group_width - n * self.bar_width) / (n - 1)
-
-    def set_x_axis_dictionary(self):
-        self.x_axis_dictionary = {}
-        for bar_obj in self.bar_objects:
-            for x_value in bar_obj.x_values:
-                self.add_to_x_axis_dictionary(x_value)
-
-    def add_to_x_axis_dictionary(self, x_value):
-        if x_value not in self.x_axis_dictionary:
-            new_dict_entry = {x_value: len(self.x_axis_dictionary)}
-            self.x_axis_dictionary.update(new_dict_entry)
-
-    def get_x_values(self, index, bar_obj):
-        x_values = np.array([self.x_axis_dictionary[x_value]
-                             for x_value in bar_obj.x_values])
-        x_values = x_values + self.x_offset + (self.bar_width + self.bar_space) * index
-        return x_values
-
-    def plot_bar_obj(self, index, bar_obj):
-        bars_obj = self.bars_obj
-        x_values = self.get_x_values(index, bar_obj)
-        self.ax.bar(x_values,
-                    bar_obj.y_values,
-                    width=self.bar_width,
-                    bottom=bars_obj.bottom,
-                    color=bar_obj.color,
-                    edgecolor=bar_obj.edgecolor,
-                    linewidth=bar_obj.linewidth,
-                    tick_label=bar_obj.tick_label,
-                    label=bar_obj.label,
-                    xerr=bar_obj.xerr,
-                    yerr=bar_obj.yerr,
-                    ecolor=bar_obj.ecolor,
-                    capsize=bar_obj.capsize,
-                    log=bars_obj.log,
-                    agg_filter=bar_obj.agg_filter,
-                    alpha=bar_obj.alpha,
-                    angle=bar_obj.angle,
-                    animated=bars_obj.animated,
-                    antialiased=bar_obj.antialiased)
-
-    def add_axis_labels(self):
-        self.add_x_label()
-        self.add_y_label()
-
-defaults.load(PlotBars)
+import matplotlib.pyplot as plt
+import numpy as np
+
+from ... import defaults
+from ..plottypes.plot import Plot
+
+class PlotBars(Plot):
+
+    def __init__(self, figure_obj, ax, bars_obj, **kwargs):
+        Plot.__init__(self, figure_obj, ax, bars_obj, **kwargs)
+        self.bars_obj = bars_obj
+        self.initialise_from_bars_obj()
+        defaults.kwargs(self, kwargs)
+
+    def initialise_from_bars_obj(self):
+        self.bar_objects = self.bars_obj.bar_objects
+        self.between_group_spacing = self.bars_obj.between_group_spacing
+        self.within_group_spacing = self.bars_obj.within_group_spacing
+
+    def plot_data(self):
+        self.preprocess_bars()
+        for index, bar_obj in enumerate(self.bars_obj.bar_objects):
+            self.plot_bar_obj(index, bar_obj)
+
+    def preprocess_bars(self):
+        self.group_width = 1 - self.between_group_spacing
+        self.set_bar_proportions()
+        self.x_offset = (self.between_group_spacing + self.bar_width - 1) / 2
+        self.set_x_axis_dictionary()
+        
+    def set_bar_proportions(self):
+        if len(self.bar_objects) == 1:
+            self.set_bar_proportions_single()
+        else:
+            self.set_proportions_multiple()
+
+    def set_bar_proportions_single(self):
+        self.bar_width = self.group_width
+        self.bar_space = self.group_width
+
+    def set_proportions_multiple(self):
+        n = len(self.bar_objects)
+        self.bar_width = self.group_width / (n + (n-1) * self.within_group_spacing)
+        self.bar_space = (self.group_width - n * self.bar_width) / (n - 1)
+
+    def set_x_axis_dictionary(self):
+        self.x_axis_dictionary = {}
+        for bar_obj in self.bar_objects:
+            for x_value in bar_obj.x_values:
+                self.add_to_x_axis_dictionary(x_value)
+
+    def add_to_x_axis_dictionary(self, x_value):
+        if x_value not in self.x_axis_dictionary:
+            new_dict_entry = {x_value: len(self.x_axis_dictionary)}
+            self.x_axis_dictionary.update(new_dict_entry)
+
+    def get_x_values(self, index, bar_obj):
+        x_values = np.array([self.x_axis_dictionary[x_value]
+                             for x_value in bar_obj.x_values])
+        x_values = x_values + self.x_offset + (self.bar_width + self.bar_space) * index
+        return x_values
+
+    def plot_bar_obj(self, index, bar_obj):
+        bars_obj = self.bars_obj
+        x_values = self.get_x_values(index, bar_obj)
+        self.ax.bar(x_values,
+                    bar_obj.y_values,
+                    width=self.bar_width,
+                    bottom=bars_obj.bottom,
+                    color=bar_obj.color,
+                    edgecolor=bar_obj.edgecolor,
+                    linewidth=bar_obj.linewidth,
+                    tick_label=bar_obj.tick_label,
+                    label=bar_obj.label,
+                    xerr=bar_obj.xerr,
+                    yerr=bar_obj.yerr,
+                    ecolor=bar_obj.ecolor,
+                    capsize=bar_obj.capsize,
+                    log=bars_obj.log,
+                    agg_filter=bar_obj.agg_filter,
+                    alpha=bar_obj.alpha,
+                    angle=bar_obj.angle,
+                    animated=bars_obj.animated,
+                    antialiased=bar_obj.antialiased)
+
+    def add_axis_labels(self):
+        self.add_x_label()
+        self.add_y_label()
+
+defaults.load(PlotBars)
```

### Comparing `hgutilities-1.0.5/hgutilities/plotting/plottypes/plotcolorplot.py` & `hgutilities-1.0.6/hgutilities/plotting/plottypes/plotcolorplot.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,58 +1,58 @@
-import matplotlib.pyplot as plt
-import matplotlib.font_manager
-import numpy as np
-
-from ... import defaults
-from ..plottypes.plot import Plot
-
-class PlotColorplot(Plot):
-
-    def __init__(self, figure_obj, ax, colorplot_obj, **kwargs):
-        Plot.__init__(self, figure_obj, ax, colorplot_obj, **kwargs)
-        self.colorplot_obj = colorplot_obj
-        defaults.kwargs(self, kwargs)
-
-    def plot_data(self):
-        colorplot_obj = self.colorplot_obj
-        x_and_y = self.get_x_and_y()
-        self.ax.pcolormesh(*x_and_y, colorplot_obj.z_mesh,
-                           cmap=colorplot_obj.cmap,
-                           norm=colorplot_obj.norm,
-                           vmin=colorplot_obj.vmin,
-                           vmax=colorplot_obj.vmax,
-                           edgecolors=colorplot_obj.edgecolors,
-                           alpha=colorplot_obj.alpha,
-                           shading=colorplot_obj.shading,
-                           snap=colorplot_obj.snap,
-                           rasterized=colorplot_obj.rasterized,
-                           agg_filter=colorplot_obj.agg_filter,
-                           animated=colorplot_obj.animated,
-                           antialiased=colorplot_obj.antialiased,
-                           capstyle=colorplot_obj.capstyle,
-                           clip_box=colorplot_obj.clip_box,
-                           clip_on=colorplot_obj.clip_on,
-                           clip_path=colorplot_obj.clip_path,
-                           color=colorplot_obj.color,
-                           edgecolor=colorplot_obj.edgecolor,
-                           facecolor=colorplot_obj.facecolor,
-                           gid=colorplot_obj.gid,
-                           hatch=colorplot_obj.hatch,
-                           joinstyle=colorplot_obj.joinstyle,
-                           label=colorplot_obj.label,
-                           linestyle=colorplot_obj.linestyle,
-                           linewidth=colorplot_obj.linewidth,
-                           mouseover=colorplot_obj.mouseover,
-                           offsets=colorplot_obj.offsets,
-                           path_effects=colorplot_obj.path_effects,
-                           visible=colorplot_obj.visible,
-                           url=colorplot_obj.url,
-                           zorder=colorplot_obj.zorder)
-
-    def get_x_and_y(self):
-        if ((self.colorplot_obj.x is not None) and
-            (self.colorplot_obj.y is not None)):
-            return (self.colorplot_obj.x, self.colorplot_obj.y)
-        else:
-            return ()
-
-defaults.load(PlotColorplot)
+import matplotlib.pyplot as plt
+import matplotlib.font_manager
+import numpy as np
+
+from ... import defaults
+from ..plottypes.plot import Plot
+
+class PlotColorplot(Plot):
+
+    def __init__(self, figure_obj, ax, colorplot_obj, **kwargs):
+        Plot.__init__(self, figure_obj, ax, colorplot_obj, **kwargs)
+        self.colorplot_obj = colorplot_obj
+        defaults.kwargs(self, kwargs)
+
+    def plot_data(self):
+        colorplot_obj = self.colorplot_obj
+        x_and_y = self.get_x_and_y()
+        self.ax.pcolormesh(*x_and_y, colorplot_obj.z_mesh,
+                           cmap=colorplot_obj.cmap,
+                           norm=colorplot_obj.norm,
+                           vmin=colorplot_obj.vmin,
+                           vmax=colorplot_obj.vmax,
+                           edgecolors=colorplot_obj.edgecolors,
+                           alpha=colorplot_obj.alpha,
+                           shading=colorplot_obj.shading,
+                           snap=colorplot_obj.snap,
+                           rasterized=colorplot_obj.rasterized,
+                           agg_filter=colorplot_obj.agg_filter,
+                           animated=colorplot_obj.animated,
+                           antialiased=colorplot_obj.antialiased,
+                           capstyle=colorplot_obj.capstyle,
+                           clip_box=colorplot_obj.clip_box,
+                           clip_on=colorplot_obj.clip_on,
+                           clip_path=colorplot_obj.clip_path,
+                           color=colorplot_obj.color,
+                           edgecolor=colorplot_obj.edgecolor,
+                           facecolor=colorplot_obj.facecolor,
+                           gid=colorplot_obj.gid,
+                           hatch=colorplot_obj.hatch,
+                           joinstyle=colorplot_obj.joinstyle,
+                           label=colorplot_obj.label,
+                           linestyle=colorplot_obj.linestyle,
+                           linewidth=colorplot_obj.linewidth,
+                           mouseover=colorplot_obj.mouseover,
+                           offsets=colorplot_obj.offsets,
+                           path_effects=colorplot_obj.path_effects,
+                           visible=colorplot_obj.visible,
+                           url=colorplot_obj.url,
+                           zorder=colorplot_obj.zorder)
+
+    def get_x_and_y(self):
+        if ((self.colorplot_obj.x is not None) and
+            (self.colorplot_obj.y is not None)):
+            return (self.colorplot_obj.x, self.colorplot_obj.y)
+        else:
+            return ()
+
+defaults.load(PlotColorplot)
```

### Comparing `hgutilities-1.0.5/hgutilities/plotting/plottypes/plotsurface.py` & `hgutilities-1.0.6/hgutilities/plotting/plottypes/plotsurface.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,95 +1,95 @@
-import matplotlib.pyplot as plt
-import numpy as np
-
-from ... import defaults
-from ..plottypes.plot import Plot
-
-class PlotSurface(Plot):
-
-    @classmethod
-    def set_function_dict(cls):
-        cls.function_dict = {"plot_surface": cls.plot_surface,
-                             "plot_wireframe": cls.plot_wireframe,
-                             "contour": cls.plot_contour}
-
-    def __init__(self, figure_obj, ax, data_obj, **kwargs):
-        Plot.__init__(self, figure_obj, ax, data_obj, **kwargs)
-        defaults.kwargs(self, kwargs)
-
-    def plot_data(self):
-        function_type = self.get_plot_function()
-        plot_function = getattr(self.ax, self.data_obj.plot_type)
-        function_type(self, plot_function, self.data_obj)
-        self.set_z_limits()
-        self.set_axes()
-
-    def get_plot_function(self):
-        plot_type = self.data_obj.plot_type
-        plot_function = self.function_dict[plot_type]
-        return plot_function
-
-    def plot_surface(self, plot_function, data_obj):
-        plot_function(data_obj.x_values,
-                      data_obj.y_values,
-                      data_obj.z_values,
-                      color=data_obj.color,
-                      cmap=data_obj.cmap,
-                      facecolors=data_obj.facecolors,
-                      norm=data_obj.norm,
-                      vmin=data_obj.vmin,
-                      vmax=data_obj.vmax,
-                      shade=data_obj.shade,
-                      lightsource=data_obj.lightsource)
-    
-    def plot_wireframe(self, plot_function, data_obj):
-        plot_function(data_obj.x_values,
-                      data_obj.y_values,
-                      data_obj.z_values,
-                      rcount=data_obj.rcount,
-                      ccount=data_obj.ccount,
-                      colors=data_obj.colors,
-                      cmap=data_obj.cmap,
-                      facecolors=data_obj.facecolors,
-                      norm=data_obj.norm,
-                      segments=data_obj.segments,
-                      linewidths=data_obj.linewidths,
-                      antialiased=data_obj.antialiased,
-                      zorder=data_obj.zorder,
-                      edgecolors=data_obj.edgecolors,
-                      linestyles=data_obj.linestyles,
-                      capstyle=data_obj.capstyle,
-                      joinstyle=data_obj.joinstyle,
-                      offsets=data_obj.offsets,
-                      offset_transform=data_obj.offset_transform,
-                      hatch=data_obj.hatch)
-
-    def plot_contour(self, plot_function, data_obj):
-        plot_function(data_obj.x_values,
-                      data_obj.y_values,
-                      data_obj.z_values,
-                      extend3d=data_obj.extend3d,
-                      stride=data_obj.stride,
-                      zdir=data_obj.zdir,
-                      offset=data_obj.offset,
-                      levels=data_obj.levels,
-                      corner_mask=data_obj.corner_mask,
-                      colors=data_obj.colors,
-                      cmap=data_obj.cmap,
-                      norm=data_obj.norm,
-                      vmin=data_obj.vmin,
-                      vmax=data_obj.vmax,
-                      origin=data_obj.origin,
-                      extent=data_obj.extent,
-                      locator=data_obj.locator,
-                      extend=data_obj.extend)
-    
-    def set_z_limits(self):
-        if self.data_obj.z_limits is not None:
-            bottom, top = self.data_obj.z_limits
-            self.ax.set_zlim(bottom=bottom, top=top)
-
-    def set_axes(self):
-        if not self.data_obj.axes:
-            self.ax.axis("off")
-
-defaults.load(PlotSurface)
+import matplotlib.pyplot as plt
+import numpy as np
+
+from ... import defaults
+from ..plottypes.plot import Plot
+
+class PlotSurface(Plot):
+
+    @classmethod
+    def set_function_dict(cls):
+        cls.function_dict = {"plot_surface": cls.plot_surface,
+                             "plot_wireframe": cls.plot_wireframe,
+                             "contour": cls.plot_contour}
+
+    def __init__(self, figure_obj, ax, data_obj, **kwargs):
+        Plot.__init__(self, figure_obj, ax, data_obj, **kwargs)
+        defaults.kwargs(self, kwargs)
+
+    def plot_data(self):
+        function_type = self.get_plot_function()
+        plot_function = getattr(self.ax, self.data_obj.plot_type)
+        function_type(self, plot_function, self.data_obj)
+        self.set_z_limits()
+        self.set_axes()
+
+    def get_plot_function(self):
+        plot_type = self.data_obj.plot_type
+        plot_function = self.function_dict[plot_type]
+        return plot_function
+
+    def plot_surface(self, plot_function, data_obj):
+        plot_function(data_obj.x_values,
+                      data_obj.y_values,
+                      data_obj.z_values,
+                      color=data_obj.color,
+                      cmap=data_obj.cmap,
+                      facecolors=data_obj.facecolors,
+                      norm=data_obj.norm,
+                      vmin=data_obj.vmin,
+                      vmax=data_obj.vmax,
+                      shade=data_obj.shade,
+                      lightsource=data_obj.lightsource)
+    
+    def plot_wireframe(self, plot_function, data_obj):
+        plot_function(data_obj.x_values,
+                      data_obj.y_values,
+                      data_obj.z_values,
+                      rcount=data_obj.rcount,
+                      ccount=data_obj.ccount,
+                      colors=data_obj.colors,
+                      cmap=data_obj.cmap,
+                      facecolors=data_obj.facecolors,
+                      norm=data_obj.norm,
+                      segments=data_obj.segments,
+                      linewidths=data_obj.linewidths,
+                      antialiased=data_obj.antialiased,
+                      zorder=data_obj.zorder,
+                      edgecolors=data_obj.edgecolors,
+                      linestyles=data_obj.linestyles,
+                      capstyle=data_obj.capstyle,
+                      joinstyle=data_obj.joinstyle,
+                      offsets=data_obj.offsets,
+                      offset_transform=data_obj.offset_transform,
+                      hatch=data_obj.hatch)
+
+    def plot_contour(self, plot_function, data_obj):
+        plot_function(data_obj.x_values,
+                      data_obj.y_values,
+                      data_obj.z_values,
+                      extend3d=data_obj.extend3d,
+                      stride=data_obj.stride,
+                      zdir=data_obj.zdir,
+                      offset=data_obj.offset,
+                      levels=data_obj.levels,
+                      corner_mask=data_obj.corner_mask,
+                      colors=data_obj.colors,
+                      cmap=data_obj.cmap,
+                      norm=data_obj.norm,
+                      vmin=data_obj.vmin,
+                      vmax=data_obj.vmax,
+                      origin=data_obj.origin,
+                      extent=data_obj.extent,
+                      locator=data_obj.locator,
+                      extend=data_obj.extend)
+    
+    def set_z_limits(self):
+        if self.data_obj.z_limits is not None:
+            bottom, top = self.data_obj.z_limits
+            self.ax.set_zlim(bottom=bottom, top=top)
+
+    def set_axes(self):
+        if not self.data_obj.axes:
+            self.ax.axis("off")
+
+defaults.load(PlotSurface)
```

### Comparing `hgutilities-1.0.5/hgutilities/plotting/plotutils/figuresize.py` & `hgutilities-1.0.6/hgutilities/utils/plots.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,29 +1,29 @@
-from matplotlib.pyplot import get_current_fig_manager
-
-def maximise_figure():
-    mng = get_current_fig_manager()
-    maximise_figure_attempt_1(mng)
-
-def maximise_figure_attempt_1(mng):
-    try:
-        mng.resize(*mng.window.maxsize())
-    except:
-        maximise_figure_attempt_2(mng)
-
-def maximise_figure_attempt_2(mng):
-    try:
-        mng.window.fullscreen()
-    except:
-        maximise_figure_attempt_3(mng)
-
-def maximise_figure_attempt_3(mng):
-    try:
-        mng.window.state('zoomed')
-    except:
-        maximise_figure_attempt_4(mng)
-
-def maximise_figure_attempt_4(mng):
-    try:
-        mng.full_screen_toggle()
-    except:
-        print("Could not maximise figure window")
+import matplotlib.pyplot as plt
+
+def maximise_figure():
+    mng = plt.get_current_fig_manager()
+    maximise_figure_attempt_1(mng)
+
+def maximise_figure_attempt_1(mng):
+    try:
+        mng.resize(*mng.window.maxsize())
+    except:
+        maximise_figure_attempt_2(mng)
+
+def maximise_figure_attempt_2(mng):
+    try:
+        mng.window.fullscreen()
+    except:
+        maximise_figure_attempt_3(mng)
+
+def maximise_figure_attempt_3(mng):
+    try:
+        mng.window.state('zoomed')
+    except:
+        maximise_figure_attempt_4(mng)
+
+def maximise_figure_attempt_4(mng):
+    try:
+        full_screen_toggle()
+    except:
+        print("Could not maximise figure window")
```

### Comparing `hgutilities-1.0.5/hgutilities/plotting/plotutils/griddimensions.py` & `hgutilities-1.0.6/hgutilities/plotting/plotutils/plotshape.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,116 +1,116 @@
-import math
-
-class GridDimensions():
-
-    def __init__(self, count, aspect_ratio):
-        self.count = count
-        self.aspect_ratio = aspect_ratio
-        self.set_grid_size()
-
-    def set_grid_size(self):
-        self.set_row_and_column_sizes()
-        self.set_row_column_pairs()
-        self.select_row_column_pair()
-        self.dimensions = [self.rows, self.columns]
-
-    def set_row_and_column_sizes(self):
-        self.set_row_sizes()
-        self.set_column_sizes()
-
-    def set_row_sizes(self):
-        row_size = math.sqrt(self.count / self.aspect_ratio)
-        self.row_small = math.floor(row_size)
-        self.row_large = math.ceil(row_size)
-
-    def set_column_sizes(self):
-        column_size = math.sqrt(self.count * self.aspect_ratio)
-        self.column_small = math.floor(column_size)
-        self.column_large = math.ceil(column_size)
-
-    def set_row_column_pairs(self):
-        self.set_pairs()
-        self.row_column_pairs = {pair: {} for pair in self.pairs}
-        self.populate_row_column_pairs()
-
-    def set_pairs(self):
-        self.pairs = [(self.row_small, self.column_small),
-                      (self.row_small, self.column_large),
-                      (self.row_large, self.column_small),
-                      (self.row_large, self.column_large)]
-
-    def populate_row_column_pairs(self):
-        for pair in self.row_column_pairs.keys():
-            self.row_column_pairs[pair] = self.get_row_column_pair_data(pair)
-
-    def get_row_column_pair_data(self, pair):
-        size = pair[0] * pair[1]
-        aspect_ratio = self.get_aspect_ratio(pair)
-        pair_data_dict = {"Size": size, "Aspect Ratio": aspect_ratio}
-        return pair_data_dict
-
-    def get_aspect_ratio(self, pair):
-        if pair[0] != 0 and pair[1] != 0:
-            aspect_ratio = pair[0] / pair[1]
-        else:
-            aspect_ratio = None
-        return aspect_ratio
-
-    def select_row_column_pair(self):
-        if len(self.row_column_pairs) == 1:
-            self.exact_ratio_pair()
-        else:
-            self.non_exact_ratio_pairs()
-
-    def exact_ratio_pair(self):
-        self.rows, self.columns = self.pairs[0]
-
-    def non_exact_ratio_pairs(self):
-        is_grid_big_enough = self.get_is_grid_big_enough()
-        row_column_pair_functions = self.get_row_column_pair_functions()
-        row_column_pair_function, *args = row_column_pair_functions[is_grid_big_enough]
-        row_column_pair_function(*args)
-        self.rows, self.columns = self.best_pair
-
-    def get_is_grid_big_enough(self):
-        is_grid_big_enough = tuple([row_column_pair["Size"] >= self.count
-                                    for row_column_pair in self.row_column_pairs.values()])
-        return is_grid_big_enough
-
-    def get_row_column_pair_functions(self):
-        row_column_pair_functions = {(True, True, True, True): (self.set_best_pair, 0),
-                                     (False, True, True, True): (self.middle_pair_compare,),
-                                     (False, True, False, True): (self.set_best_pair, 1),
-                                     (False, False, True, True): (self.set_best_pair, 2),
-                                     (False, False, False, True): (self.set_best_pair, 3)}
-        return row_column_pair_functions
-
-    def set_best_pair(self, pair_index):
-        self.best_pair = self.pairs[pair_index]
-
-    def middle_pair_compare(self):
-        self.set_aspect_ratio_scores()
-        self.compare_aspect_ratio_scores()
-
-    def set_aspect_ratio_scores(self):
-        aspect_ratio_1 = self.row_column_pairs[self.pairs[1]]["Aspect Ratio"]
-        aspect_ratio_2 = self.row_column_pairs[self.pairs[2]]["Aspect Ratio"]
-        self.aspect_ratio_score_1 = self.get_aspect_ratio_score(aspect_ratio_1)
-        self.aspect_ratio_score_2 = self.get_aspect_ratio_score(aspect_ratio_2)
-
-    def get_aspect_ratio_score(self, aspect_ratio):
-        if aspect_ratio is not None:
-            score = max(aspect_ratio / self.aspect_ratio,
-                        self.aspect_ratio / aspect_ratio)
-        else:
-            score = None
-        return score
-
-    def compare_aspect_ratio_scores(self):
-        if self.aspect_ratio_score_1 < self.aspect_ratio_score_2:
-            self.set_best_pair(1)
-        else:
-            self.set_best_pair(2)
-
-def get_grid_dimensions(count, aspect_ratio):
-    grid_dimensions_obj = GridDimensions(count, aspect_ratio)
-    return grid_dimensions_obj.dimensions
+import math
+
+class PlotShape():
+
+    def __init__(self, count, aspect_ratio):
+        self.count = count
+        self.aspect_ratio = aspect_ratio
+        self.set_grid_size()
+
+    def set_grid_size(self):
+        self.set_row_and_column_sizes()
+        self.set_row_column_pairs()
+        self.select_row_column_pair()
+        self.dimensions = [self.rows, self.columns]
+
+    def set_row_and_column_sizes(self):
+        self.set_row_sizes()
+        self.set_column_sizes()
+
+    def set_row_sizes(self):
+        row_size = math.sqrt(self.count / self.aspect_ratio)
+        self.row_small = math.floor(row_size)
+        self.row_large = math.ceil(row_size)
+
+    def set_column_sizes(self):
+        column_size = math.sqrt(self.count * self.aspect_ratio)
+        self.column_small = math.floor(column_size)
+        self.column_large = math.ceil(column_size)
+
+    def set_row_column_pairs(self):
+        self.set_pairs()
+        self.row_column_pairs = {pair: {} for pair in self.pairs}
+        self.populate_row_column_pairs()
+
+    def set_pairs(self):
+        self.pairs = [(self.row_small, self.column_small),
+                      (self.row_small, self.column_large),
+                      (self.row_large, self.column_small),
+                      (self.row_large, self.column_large)]
+
+    def populate_row_column_pairs(self):
+        for pair in self.row_column_pairs.keys():
+            self.row_column_pairs[pair] = self.get_row_column_pair_data(pair)
+
+    def get_row_column_pair_data(self, pair):
+        size = pair[0] * pair[1]
+        aspect_ratio = self.get_aspect_ratio(pair)
+        pair_data_dict = {"Size": size, "Aspect Ratio": aspect_ratio}
+        return pair_data_dict
+
+    def get_aspect_ratio(self, pair):
+        if pair[0] != 0 and pair[1] != 0:
+            aspect_ratio = pair[0] / pair[1]
+        else:
+            aspect_ratio = None
+        return aspect_ratio
+
+    def select_row_column_pair(self):
+        if len(self.row_column_pairs) == 1:
+            self.exact_ratio_pair()
+        else:
+            self.non_exact_ratio_pairs()
+
+    def exact_ratio_pair(self):
+        self.rows, self.columns = self.pairs[0]
+
+    def non_exact_ratio_pairs(self):
+        is_grid_big_enough = self.get_is_grid_big_enough()
+        row_column_pair_functions = self.get_row_column_pair_functions()
+        row_column_pair_function, *args = row_column_pair_functions[is_grid_big_enough]
+        row_column_pair_function(*args)
+        self.rows, self.columns = self.best_pair
+
+    def get_is_grid_big_enough(self):
+        is_grid_big_enough = tuple([row_column_pair["Size"] >= self.count
+                                    for row_column_pair in self.row_column_pairs.values()])
+        return is_grid_big_enough
+
+    def get_row_column_pair_functions(self):
+        row_column_pair_functions = {(True, True, True, True): (self.set_best_pair, 0),
+                                     (False, True, True, True): (self.middle_pair_compare,),
+                                     (False, True, False, True): (self.set_best_pair, 1),
+                                     (False, False, True, True): (self.set_best_pair, 2),
+                                     (False, False, False, True): (self.set_best_pair, 3)}
+        return row_column_pair_functions
+
+    def set_best_pair(self, pair_index):
+        self.best_pair = self.pairs[pair_index]
+
+    def middle_pair_compare(self):
+        self.set_aspect_ratio_scores()
+        self.compare_aspect_ratio_scores()
+
+    def set_aspect_ratio_scores(self):
+        aspect_ratio_1 = self.row_column_pairs[self.pairs[1]]["Aspect Ratio"]
+        aspect_ratio_2 = self.row_column_pairs[self.pairs[2]]["Aspect Ratio"]
+        self.aspect_ratio_score_1 = self.get_aspect_ratio_score(aspect_ratio_1)
+        self.aspect_ratio_score_2 = self.get_aspect_ratio_score(aspect_ratio_2)
+
+    def get_aspect_ratio_score(self, aspect_ratio):
+        if aspect_ratio is not None:
+            score = max(aspect_ratio / self.aspect_ratio,
+                        self.aspect_ratio / aspect_ratio)
+        else:
+            score = None
+        return score
+
+    def compare_aspect_ratio_scores(self):
+        if self.aspect_ratio_score_1 < self.aspect_ratio_score_2:
+            self.set_best_pair(1)
+        else:
+            self.set_best_pair(2)
+
+def get_grid_dimensions(count, aspect_ratio):
+    plot_shape_obj = PlotShape(count, aspect_ratio)
+    return plot_shape_obj.dimensions
```

### Comparing `hgutilities-1.0.5/hgutilities/plotting/plotutils/plotshape.py` & `hgutilities-1.0.6/hgutilities/plotting/plotutils/griddimensions.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,116 +1,116 @@
-import math
-
-class PlotShape():
-
-    def __init__(self, count, aspect_ratio):
-        self.count = count
-        self.aspect_ratio = aspect_ratio
-        self.set_grid_size()
-
-    def set_grid_size(self):
-        self.set_row_and_column_sizes()
-        self.set_row_column_pairs()
-        self.select_row_column_pair()
-        self.dimensions = [self.rows, self.columns]
-
-    def set_row_and_column_sizes(self):
-        self.set_row_sizes()
-        self.set_column_sizes()
-
-    def set_row_sizes(self):
-        row_size = math.sqrt(self.count / self.aspect_ratio)
-        self.row_small = math.floor(row_size)
-        self.row_large = math.ceil(row_size)
-
-    def set_column_sizes(self):
-        column_size = math.sqrt(self.count * self.aspect_ratio)
-        self.column_small = math.floor(column_size)
-        self.column_large = math.ceil(column_size)
-
-    def set_row_column_pairs(self):
-        self.set_pairs()
-        self.row_column_pairs = {pair: {} for pair in self.pairs}
-        self.populate_row_column_pairs()
-
-    def set_pairs(self):
-        self.pairs = [(self.row_small, self.column_small),
-                      (self.row_small, self.column_large),
-                      (self.row_large, self.column_small),
-                      (self.row_large, self.column_large)]
-
-    def populate_row_column_pairs(self):
-        for pair in self.row_column_pairs.keys():
-            self.row_column_pairs[pair] = self.get_row_column_pair_data(pair)
-
-    def get_row_column_pair_data(self, pair):
-        size = pair[0] * pair[1]
-        aspect_ratio = self.get_aspect_ratio(pair)
-        pair_data_dict = {"Size": size, "Aspect Ratio": aspect_ratio}
-        return pair_data_dict
-
-    def get_aspect_ratio(self, pair):
-        if pair[0] != 0 and pair[1] != 0:
-            aspect_ratio = pair[0] / pair[1]
-        else:
-            aspect_ratio = None
-        return aspect_ratio
-
-    def select_row_column_pair(self):
-        if len(self.row_column_pairs) == 1:
-            self.exact_ratio_pair()
-        else:
-            self.non_exact_ratio_pairs()
-
-    def exact_ratio_pair(self):
-        self.rows, self.columns = self.pairs[0]
-
-    def non_exact_ratio_pairs(self):
-        is_grid_big_enough = self.get_is_grid_big_enough()
-        row_column_pair_functions = self.get_row_column_pair_functions()
-        row_column_pair_function, *args = row_column_pair_functions[is_grid_big_enough]
-        row_column_pair_function(*args)
-        self.rows, self.columns = self.best_pair
-
-    def get_is_grid_big_enough(self):
-        is_grid_big_enough = tuple([row_column_pair["Size"] >= self.count
-                                    for row_column_pair in self.row_column_pairs.values()])
-        return is_grid_big_enough
-
-    def get_row_column_pair_functions(self):
-        row_column_pair_functions = {(True, True, True, True): (self.set_best_pair, 0),
-                                     (False, True, True, True): (self.middle_pair_compare,),
-                                     (False, True, False, True): (self.set_best_pair, 1),
-                                     (False, False, True, True): (self.set_best_pair, 2),
-                                     (False, False, False, True): (self.set_best_pair, 3)}
-        return row_column_pair_functions
-
-    def set_best_pair(self, pair_index):
-        self.best_pair = self.pairs[pair_index]
-
-    def middle_pair_compare(self):
-        self.set_aspect_ratio_scores()
-        self.compare_aspect_ratio_scores()
-
-    def set_aspect_ratio_scores(self):
-        aspect_ratio_1 = self.row_column_pairs[self.pairs[1]]["Aspect Ratio"]
-        aspect_ratio_2 = self.row_column_pairs[self.pairs[2]]["Aspect Ratio"]
-        self.aspect_ratio_score_1 = self.get_aspect_ratio_score(aspect_ratio_1)
-        self.aspect_ratio_score_2 = self.get_aspect_ratio_score(aspect_ratio_2)
-
-    def get_aspect_ratio_score(self, aspect_ratio):
-        if aspect_ratio is not None:
-            score = max(aspect_ratio / self.aspect_ratio,
-                        self.aspect_ratio / aspect_ratio)
-        else:
-            score = None
-        return score
-
-    def compare_aspect_ratio_scores(self):
-        if self.aspect_ratio_score_1 < self.aspect_ratio_score_2:
-            self.set_best_pair(1)
-        else:
-            self.set_best_pair(2)
-
-def get_grid_dimensions(count, aspect_ratio):
-    plot_shape_obj = PlotShape(count, aspect_ratio)
-    return plot_shape_obj.dimensions
+import math
+
+class GridDimensions():
+
+    def __init__(self, count, aspect_ratio):
+        self.count = count
+        self.aspect_ratio = aspect_ratio
+        self.set_grid_size()
+
+    def set_grid_size(self):
+        self.set_row_and_column_sizes()
+        self.set_row_column_pairs()
+        self.select_row_column_pair()
+        self.dimensions = [self.rows, self.columns]
+
+    def set_row_and_column_sizes(self):
+        self.set_row_sizes()
+        self.set_column_sizes()
+
+    def set_row_sizes(self):
+        row_size = math.sqrt(self.count / self.aspect_ratio)
+        self.row_small = math.floor(row_size)
+        self.row_large = math.ceil(row_size)
+
+    def set_column_sizes(self):
+        column_size = math.sqrt(self.count * self.aspect_ratio)
+        self.column_small = math.floor(column_size)
+        self.column_large = math.ceil(column_size)
+
+    def set_row_column_pairs(self):
+        self.set_pairs()
+        self.row_column_pairs = {pair: {} for pair in self.pairs}
+        self.populate_row_column_pairs()
+
+    def set_pairs(self):
+        self.pairs = [(self.row_small, self.column_small),
+                      (self.row_small, self.column_large),
+                      (self.row_large, self.column_small),
+                      (self.row_large, self.column_large)]
+
+    def populate_row_column_pairs(self):
+        for pair in self.row_column_pairs.keys():
+            self.row_column_pairs[pair] = self.get_row_column_pair_data(pair)
+
+    def get_row_column_pair_data(self, pair):
+        size = pair[0] * pair[1]
+        aspect_ratio = self.get_aspect_ratio(pair)
+        pair_data_dict = {"Size": size, "Aspect Ratio": aspect_ratio}
+        return pair_data_dict
+
+    def get_aspect_ratio(self, pair):
+        if pair[0] != 0 and pair[1] != 0:
+            aspect_ratio = pair[0] / pair[1]
+        else:
+            aspect_ratio = None
+        return aspect_ratio
+
+    def select_row_column_pair(self):
+        if len(self.row_column_pairs) == 1:
+            self.exact_ratio_pair()
+        else:
+            self.non_exact_ratio_pairs()
+
+    def exact_ratio_pair(self):
+        self.rows, self.columns = self.pairs[0]
+
+    def non_exact_ratio_pairs(self):
+        is_grid_big_enough = self.get_is_grid_big_enough()
+        row_column_pair_functions = self.get_row_column_pair_functions()
+        row_column_pair_function, *args = row_column_pair_functions[is_grid_big_enough]
+        row_column_pair_function(*args)
+        self.rows, self.columns = self.best_pair
+
+    def get_is_grid_big_enough(self):
+        is_grid_big_enough = tuple([row_column_pair["Size"] >= self.count
+                                    for row_column_pair in self.row_column_pairs.values()])
+        return is_grid_big_enough
+
+    def get_row_column_pair_functions(self):
+        row_column_pair_functions = {(True, True, True, True): (self.set_best_pair, 0),
+                                     (False, True, True, True): (self.middle_pair_compare,),
+                                     (False, True, False, True): (self.set_best_pair, 1),
+                                     (False, False, True, True): (self.set_best_pair, 2),
+                                     (False, False, False, True): (self.set_best_pair, 3)}
+        return row_column_pair_functions
+
+    def set_best_pair(self, pair_index):
+        self.best_pair = self.pairs[pair_index]
+
+    def middle_pair_compare(self):
+        self.set_aspect_ratio_scores()
+        self.compare_aspect_ratio_scores()
+
+    def set_aspect_ratio_scores(self):
+        aspect_ratio_1 = self.row_column_pairs[self.pairs[1]]["Aspect Ratio"]
+        aspect_ratio_2 = self.row_column_pairs[self.pairs[2]]["Aspect Ratio"]
+        self.aspect_ratio_score_1 = self.get_aspect_ratio_score(aspect_ratio_1)
+        self.aspect_ratio_score_2 = self.get_aspect_ratio_score(aspect_ratio_2)
+
+    def get_aspect_ratio_score(self, aspect_ratio):
+        if aspect_ratio is not None:
+            score = max(aspect_ratio / self.aspect_ratio,
+                        self.aspect_ratio / aspect_ratio)
+        else:
+            score = None
+        return score
+
+    def compare_aspect_ratio_scores(self):
+        if self.aspect_ratio_score_1 < self.aspect_ratio_score_2:
+            self.set_best_pair(1)
+        else:
+            self.set_best_pair(2)
+
+def get_grid_dimensions(count, aspect_ratio):
+    grid_dimensions_obj = GridDimensions(count, aspect_ratio)
+    return grid_dimensions_obj.dimensions
```

### Comparing `hgutilities-1.0.5/hgutilities/plotting/plotutils/savefigure.py` & `hgutilities-1.0.6/hgutilities/plotting/plotutils/savefigure.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,43 +1,43 @@
-import os
-
-from matplotlib.pyplot import savefig
-
-def save_figure(plot_obj):
-    path = get_figure_path(plot_obj)
-    plots_obj = plot_obj.plots_obj
-    save_fig(path, plots_obj)
-    plt.close()
-
-def get_figure_path(plot_obj):
-    file_name = get_file_name(plot_obj)
-    file_name = f"{file_name}.{plot_obj.plots_obj.format}"
-    path = os.path.join(plot_obj.plots_obj.path, file_name)
-    return path
-
-def get_file_name(plot_obj):
-    if len(plot_obj.plots_obj.lines_object_groups) == 1:
-        return get_base_file_name(plot_obj.plots_obj)
-    else:
-        return get_numbered_file_name(plot_obj)
-
-def get_base_file_name(plot_objs):
-    if plot_objs.title is None:
-        return "Figure"
-    else:
-        return str(plot_objs.title)
-
-def get_numbered_file_name(plot_obj):
-    file_name = get_base_file_name(plot_obj.plot_objs)
-    file_name = f"{file_name} {plot_obj.plot_index + 1}"
-    return file_name
-
-def save_fig(path, plots_obj):
-    savefig(path,
-            dpi=plots_obj.dpi,
-            format=plots_obj.format,
-            metadata=plots_obj.metadata,
-            bbox_inches=plots_obj.bbox_inches,
-            pad_inches=plots_obj.pad_inches,
-            facecolor=plots_obj.facecolor,
-            edgecolor=plots_obj.edgecolor,
-            backend=plots_obj.backend)
+import os
+
+from matplotlib.pyplot import savefig
+
+def save_figure(plot_obj):
+    path = get_figure_path(plot_obj)
+    plots_obj = plot_obj.plots_obj
+    save_fig(path, plots_obj)
+    plt.close()
+
+def get_figure_path(plot_obj):
+    file_name = get_file_name(plot_obj)
+    file_name = f"{file_name}.{plot_obj.plots_obj.format}"
+    path = os.path.join(plot_obj.plots_obj.path, file_name)
+    return path
+
+def get_file_name(plot_obj):
+    if len(plot_obj.plots_obj.lines_object_groups) == 1:
+        return get_base_file_name(plot_obj.plots_obj)
+    else:
+        return get_numbered_file_name(plot_obj)
+
+def get_base_file_name(plot_objs):
+    if plot_objs.title is None:
+        return "Figure"
+    else:
+        return str(plot_objs.title)
+
+def get_numbered_file_name(plot_obj):
+    file_name = get_base_file_name(plot_obj.plot_objs)
+    file_name = f"{file_name} {plot_obj.plot_index + 1}"
+    return file_name
+
+def save_fig(path, plots_obj):
+    savefig(path,
+            dpi=plots_obj.dpi,
+            format=plots_obj.format,
+            metadata=plots_obj.metadata,
+            bbox_inches=plots_obj.bbox_inches,
+            pad_inches=plots_obj.pad_inches,
+            facecolor=plots_obj.facecolor,
+            edgecolor=plots_obj.edgecolor,
+            backend=plots_obj.backend)
```

### Comparing `hgutilities-1.0.5/hgutilities/utils/groups.py` & `hgutilities-1.0.6/hgutilities/utils/groups.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,37 +1,37 @@
-import math
-
-import numpy as np
-
-def get_group_size(group_size, object_list):
-    if group_size is None:
-        group_size = len(object_list)
-    return group_size
-
-def get_group_indexes(length, group_size):
-    group_size, group_count = get_group_data(length, group_size)
-    end_point_indexes = get_end_point_indexes(length, group_size, group_count)
-    group_indexes = construct_group_indexes(length, group_count, end_point_indexes)
-    return group_indexes
-
-def get_group_data(length, group_size):
-    group_size = get_modified_group_size(length, group_size)
-    group_count = math.floor(length/group_size)
-    return group_size, group_count
-
-def get_modified_group_size(list_size, average_size):
-    if list_size < average_size:
-        average_size = list_size
-    return average_size
-
-def get_end_point_indexes(length, group_size, group_count):
-    real_group_size = length/group_count
-    real_group_end_points = np.arange(0, group_count + 1) * real_group_size
-    real_group_end_points = np.round(real_group_end_points, 5)
-    end_point_indexes = np.ceil(real_group_end_points)
-    return end_point_indexes
-
-def construct_group_indexes(length, group_count, end_point_indexes):
-    group_indexes = [np.arange(end_point_indexes[group_number],
-                               end_point_indexes[group_number + 1]).astype('int')
-                     for group_number in range(group_count)]
-    return group_indexes
+import math
+
+import numpy as np
+
+def get_group_size(group_size, object_list):
+    if group_size is None:
+        group_size = len(object_list)
+    return group_size
+
+def get_group_indexes(length, group_size):
+    group_size, group_count = get_group_data(length, group_size)
+    end_point_indexes = get_end_point_indexes(length, group_size, group_count)
+    group_indexes = construct_group_indexes(length, group_count, end_point_indexes)
+    return group_indexes
+
+def get_group_data(length, group_size):
+    group_size = get_modified_group_size(length, group_size)
+    group_count = math.floor(length/group_size)
+    return group_size, group_count
+
+def get_modified_group_size(list_size, average_size):
+    if list_size < average_size:
+        average_size = list_size
+    return average_size
+
+def get_end_point_indexes(length, group_size, group_count):
+    real_group_size = length/group_count
+    real_group_end_points = np.arange(0, group_count + 1) * real_group_size
+    real_group_end_points = np.round(real_group_end_points, 5)
+    end_point_indexes = np.ceil(real_group_end_points)
+    return end_point_indexes
+
+def construct_group_indexes(length, group_count, end_point_indexes):
+    group_indexes = [np.arange(end_point_indexes[group_number],
+                               end_point_indexes[group_number + 1]).astype('int')
+                     for group_number in range(group_count)]
+    return group_indexes
```

### Comparing `hgutilities-1.0.5/hgutilities/utils/paths.py` & `hgutilities-1.0.6/hgutilities/utils/paths.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,34 +1,34 @@
-import os
-import json
-
-def make_file(file_path):
-    if not os.path.exists(file_path):
-        folder_path = os.path.split(file_path)[0]
-        make_folder(folder_path)
-        make_empty_file(file_path)
-
-def make_empty_file(file_path):
-    with open(file_path, "w") as file:
-        pass
-
-def make_folder(folder_path):
-    if not os.path.exists(folder_path):
-        parent_folder_path = os.path.split(folder_path)[0]
-        make_folder(parent_folder_path)
-        os.mkdir(folder_path)
-
-def make_folder_path(path):
-    if os.path.isfile(path):
-        path = os.path.split(path)[0]
-    make_file(path)
-
-def load_json(path, ignore_empty_or_none=True):
-    if ignore_empty_or_none:
-        if not os.path.exists(path) or os.stat(path).st_size == 0:
-            return {}
-    return do_load_json(path)
-
-def do_load_json(path):
-    with open(path, "r") as file:
-        file_contents = json.load(file)
-    return file_contents
+import os
+import json
+
+def make_file(file_path):
+    if not os.path.exists(file_path):
+        folder_path = os.path.split(file_path)[0]
+        make_folder(folder_path)
+        make_empty_file(file_path)
+
+def make_empty_file(file_path):
+    with open(file_path, "w") as file:
+        pass
+
+def make_folder(folder_path):
+    if not os.path.exists(folder_path):
+        parent_folder_path = os.path.split(folder_path)[0]
+        make_folder(parent_folder_path)
+        os.mkdir(folder_path)
+
+def make_folder_path(path):
+    if os.path.isfile(path):
+        path = os.path.split(path)[0]
+    make_file(path)
+
+def load_json(path, ignore_empty_or_none=True):
+    if ignore_empty_or_none:
+        if not os.path.exists(path) or os.stat(path).st_size == 0:
+            return {}
+    return do_load_json(path)
+
+def do_load_json(path):
+    with open(path, "r") as file:
+        file_contents = json.load(file)
+    return file_contents
```

### Comparing `hgutilities-1.0.5/hgutilities.egg-info/PKG-INFO` & `hgutilities-1.0.6/hgutilities.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,99 +1,95 @@
-Metadata-Version: 2.1
-Name: hgutilities
-Version: 1.0.5
-Summary: A triple of tools used for plotting, handling key-words, and utilities
-Home-page: UNKNOWN
-Author: Henry Ginn
-Author-email: <henryginn137@gmail.com>
-License: UNKNOWN
-Keywords: python,matplotlib,plotting,default,keywords,utils
-Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Natural Language :: English
-Classifier: Operating System :: Unix
-Classifier: Operating System :: Microsoft :: Windows
-Description-Content-Type: text/markdown
-License-File: LICENSE.md
-
-
-# HGUtilities
-This is a collection of useful tools I use regularly. There are three parts to this package:
-
-- Defaults: manages settings for classes that can be controlled easily from an interface.
-- Plotting: a front end for matplotlib to easily create subplots.
-- Utils: a collection of generally useful functions
-
-## Contents
-
-1. [Defaults](#defaults)
-1. [Plotting](#plotting)
-1. [Utils](#utils)
-1. [Development](#development)
-
-## Defaults
-
-### The Problem
-
-Usually at the beginning of a class there will be a list of class variables with default values set. The aim of this part of the package is to deal with the following issues:
-
-- To view all the defaults you need to go into the script itself
-- It is awkward to change the value of those variables from an interface
-- It is impossible to change the default values without digging into the code itself.
-- Passing in many arguments to functions is messy
-- Mutable default values need to be implemented more carefully
-
-Normally there are two ways of handling keyword arguments with default values.The simpler way is to have the keyword in the function signature being set equal to it's default value. If it's default value is mutable, it will need to be set to None. Code will then need to be implemented to check if it has been changed, and if not, set it to it's default value. Once there are several keyword arguemnts, this becomes messy however, and it would be preferred to pack the keywords together with **kwargs. With this second method, there will need to be code that detects if a keyword is in the **kwargs dict, and if so change it. This means we have a method for every keyword argument a function takes in, and so we can easily end up with dozens of lines of code that clogs up our classes and is a chore to implement every time we change the keyword arguments a function takes in.
-
-In the second case, we cannot see what keyword arguments a function takes in, and can only do so in the first case if the we are calling a function directly unless each function in the middle also has all the keywords in the signature. Modifying the default values would also mean going into the code, finding the method where the keyword is processed, and editing the code directly.
-
-### The Solution
-
-For each class, we store the default values in a json file. After the class definition, we pass the class itself into a function that loads the values from the file, and sets them as class variables. This code is only run once when the file with the class is imported. The class will also have the attribute "defaults" assigned to it with all the default values. This allows the user to read what the defaults are from the interface, but beyond that it serves to purpose after the default values have been loaded in. If the user overwrites it, they will no longer be able to see the defaults for that object (with `my_obj.defaults`), and will need to look at the class attribute itself (with `MyClass.defaults`).
-
-Whenever a method takes in keyword arguments, they can be passed into a function that processes the kwargs, along with a reference to the instance itself. This will automate the process described in the previous section, and if there are any keyword arguments that were not in the list of defaults, the file will be opened and overwritten with the new keyword arguments added. Their default value will be set to `None`. Below is an example of how this is implemented.
-
-    from hgutilities import defaults
-
-    class MyClass():
-
-        def __init__(self, **kwargs):
-            defaults.kwargs(self, **kwargs)
-
-    defaults.load(MyClass)
-
-We note that `defaults.kwargs` can be called from anywhere within the class and not just at initialisation, and that `**kwargs` or `kwargs` can be fed in as the second argument. If there are kwargs that require more complicated processing, they can be processed after the call to `defaults.kwargs`, and the default value of such keyword arguments should be set to `null` in the json file of defaults.
-
-The path to the json file is stored as a class attribute `defaults_path`. In the directory that contains the script with the class, there will be another directory called "Default Settings", and this has the json files for all scripts in the original directory.
-
-## Plotting
-
-For full documentation, see the specific README inside the "plotting" module folder.
-
-When creating a figure with varying characteristics, the user needs to change their code in potentially non-trivial ways in order to get the desired result. For example, if they had 12 subplots on a figure, and they decide that they want two figures with six subplots each instead, a single for loop would need to be split into two different for loops. If one of the subplots needed two lines plotted instead of one, they would either need to add that in manually outside of the loop, or change the whole data structure to make it more general. When the number of subplots is unknown, these problems are even worse. The aim of this part of the package is to make the creation of such figures easier.
-
-The user creates data objects that store the information to be plotted. For example an instance of `Line` would have a list of $x$ values, a list of $y$ values, and optional settings such as a label and linestyle. A `Lines` object would have a collection of `Line` objects, and other information such as a subplot title, axes labels, whether it has a legend, etc. These objects can be passed in to a `Figures` object, and this does the work of deciding how they should be distributed among figures. The purpose of this is to give the user a way to easily specify what data needs to be plotted where, without needing to hardcode in the structure of the subplots.
-
-It also provides other functions such as easily applying a rainbow pattern to the lines, adding a legend that corresponds to multiple subplots, and applying prefixes to the axes. The ability to animate figures is also built in, although this should only be used for short gifs, on the order of a few dozen frames.
-
-## Utils
-
-The aim of this is to improve quality of coding life by implementing some common functions. For example when reading a json file, you cannot simply open the file and load the json, you must first check whether it is empty. Such annoyances are handled by the functions in this part of the package. We split the utilities into several categories to make it easier to organise them. The functions implemented here are tailored to my personal needs, and they may not have the desired functionality for a general use case. Backwards compatibility is not guaranteed.
-
-## Development
-
-### Features and functionality to add in V1.1
-
-- automatic prefixing to axes
-- more control over subplot placement
-- automatic paragraph organisation for documentation
-- better distribution of subplots over multiple figures
-- control over tick labels
-- horizontal bar charts
-- better file extension handling for Defaults package
-- inherit function should be able to take in a single attribute as a non-iterable
-- animations need to be made compatible with more plot types
-- add README to defaults subpackage
-
+Metadata-Version: 2.1
+Name: hgutilities
+Version: 1.0.6
+Summary: A triple of tools used for plotting, handling key-words, and utilities
+Author: Henry Ginn
+Author-email: <henryginn137@gmail.com>
+Keywords: python,matplotlib,plotting,default,keywords,utils
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Natural Language :: English
+Classifier: Operating System :: Unix
+Classifier: Operating System :: Microsoft :: Windows
+Description-Content-Type: text/markdown
+License-File: LICENSE.md
+
+
+# HGUtilities
+This is a collection of useful tools I use regularly. There are three parts to this package:
+
+- Defaults: manages settings for classes that can be controlled easily from an interface.
+- Plotting: a front end for matplotlib to easily create subplots.
+- Utils: a collection of generally useful functions
+
+## Contents
+
+1. [Defaults](#defaults)
+1. [Plotting](#plotting)
+1. [Utils](#utils)
+1. [Development](#development)
+
+## Defaults
+
+### The Problem
+
+Usually at the beginning of a class there will be a list of class variables with default values set. The aim of this part of the package is to deal with the following issues:
+
+- To view all the defaults you need to go into the script itself
+- It is awkward to change the value of those variables from an interface
+- It is impossible to change the default values without digging into the code itself.
+- Passing in many arguments to functions is messy
+- Mutable default values need to be implemented more carefully
+
+Normally there are two ways of handling keyword arguments with default values.The simpler way is to have the keyword in the function signature being set equal to it's default value. If it's default value is mutable, it will need to be set to None. Code will then need to be implemented to check if it has been changed, and if not, set it to it's default value. Once there are several keyword arguemnts, this becomes messy however, and it would be preferred to pack the keywords together with **kwargs. With this second method, there will need to be code that detects if a keyword is in the **kwargs dict, and if so change it. This means we have a method for every keyword argument a function takes in, and so we can easily end up with dozens of lines of code that clogs up our classes and is a chore to implement every time we change the keyword arguments a function takes in.
+
+In the second case, we cannot see what keyword arguments a function takes in, and can only do so in the first case if the we are calling a function directly unless each function in the middle also has all the keywords in the signature. Modifying the default values would also mean going into the code, finding the method where the keyword is processed, and editing the code directly.
+
+### The Solution
+
+For each class, we store the default values in a json file. After the class definition, we pass the class itself into a function that loads the values from the file, and sets them as class variables. This code is only run once when the file with the class is imported. The class will also have the attribute "defaults" assigned to it with all the default values. This allows the user to read what the defaults are from the interface, but beyond that it serves to purpose after the default values have been loaded in. If the user overwrites it, they will no longer be able to see the defaults for that object (with `my_obj.defaults`), and will need to look at the class attribute itself (with `MyClass.defaults`).
+
+Whenever a method takes in keyword arguments, they can be passed into a function that processes the kwargs, along with a reference to the instance itself. This will automate the process described in the previous section, and if there are any keyword arguments that were not in the list of defaults, the file will be opened and overwritten with the new keyword arguments added. Their default value will be set to `None`. Below is an example of how this is implemented.
+
+    from hgutilities import defaults
+
+    class MyClass():
+
+        def __init__(self, **kwargs):
+            defaults.kwargs(self, **kwargs)
+
+    defaults.load(MyClass)
+
+We note that `defaults.kwargs` can be called from anywhere within the class and not just at initialisation, and that `**kwargs` or `kwargs` can be fed in as the second argument. If there are kwargs that require more complicated processing, they can be processed after the call to `defaults.kwargs`, and the default value of such keyword arguments should be set to `null` in the json file of defaults.
+
+The path to the json file is stored as a class attribute `defaults_path`. In the directory that contains the script with the class, there will be another directory called "Default Settings", and this has the json files for all scripts in the original directory.
+
+## Plotting
+
+For full documentation, see the specific README inside the "plotting" module folder.
+
+When creating a figure with varying characteristics, the user needs to change their code in potentially non-trivial ways in order to get the desired result. For example, if they had 12 subplots on a figure, and they decide that they want two figures with six subplots each instead, a single for loop would need to be split into two different for loops. If one of the subplots needed two lines plotted instead of one, they would either need to add that in manually outside of the loop, or change the whole data structure to make it more general. When the number of subplots is unknown, these problems are even worse. The aim of this part of the package is to make the creation of such figures easier.
+
+The user creates data objects that store the information to be plotted. For example an instance of `Line` would have a list of $x$ values, a list of $y$ values, and optional settings such as a label and linestyle. A `Lines` object would have a collection of `Line` objects, and other information such as a subplot title, axes labels, whether it has a legend, etc. These objects can be passed in to a `Figures` object, and this does the work of deciding how they should be distributed among figures. The purpose of this is to give the user a way to easily specify what data needs to be plotted where, without needing to hardcode in the structure of the subplots.
+
+It also provides other functions such as easily applying a rainbow pattern to the lines, adding a legend that corresponds to multiple subplots, and applying prefixes to the axes. The ability to animate figures is also built in, although this should only be used for short gifs, on the order of a few dozen frames.
+
+## Utils
+
+The aim of this is to improve quality of coding life by implementing some common functions. For example when reading a json file, you cannot simply open the file and load the json, you must first check whether it is empty. Such annoyances are handled by the functions in this part of the package. We split the utilities into several categories to make it easier to organise them. The functions implemented here are tailored to my personal needs, and they may not have the desired functionality for a general use case. Backwards compatibility is not guaranteed.
+
+## Development
+
+### Features and functionality to add in V1.1
+
+- automatic prefixing to axes
+- more control over subplot placement
+- automatic paragraph organisation for documentation
+- better distribution of subplots over multiple figures
+- control over tick labels
+- horizontal bar charts
+- better file extension handling for Defaults package
+- inherit function should be able to take in a single attribute as a non-iterable
+- animations need to be made compatible with more plot types
+- add README to defaults subpackage
```

### Comparing `hgutilities-1.0.5/setup.py` & `hgutilities-1.0.6/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,38 +1,38 @@
-from setuptools import setup, find_packages
-import codecs
-import os
-
-here = os.path.abspath(os.path.dirname(__file__))
-
-with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
-    long_description = "\n" + fh.read()
-
-VERSION = "1.0.5"
-DESCRIPTION = "A triple of tools used for plotting, handling key-words, and utilities"
-LONG_DESCRIPTION = ("Defaults: manages settings for classes that can be controlled easily from an interface.\n"
-                    "Plotting: a front end for matplotlib to easily create subplots.\n"
-                    "Utils: a collection of generally useful functions")
-
-# Setting up
-setup(
-    name="hgutilities",
-    version=VERSION,
-    author="Henry Ginn",
-    author_email="<henryginn137@gmail.com>",
-    description=DESCRIPTION,
-    long_description_content_type="text/markdown",
-    long_description=long_description,
-    setup_requires=['setuptools_scm'],
-    include_package_data=True,
-    install_requires=["matplotlib", "numpy", "screeninfo", "pillow"],
-    keywords=["python", "matplotlib", "plotting", "default", "keywords", "utils"],
-    classifiers=[
-        "Development Status :: 4 - Beta",
-        "Intended Audience :: Developers",
-        "Programming Language :: Python :: 3",
-        "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
-        "Natural Language :: English",
-        "Operating System :: Unix",
-        "Operating System :: Microsoft :: Windows",
-    ]
-)
+from setuptools import setup, find_packages
+import codecs
+import os
+
+here = os.path.abspath(os.path.dirname(__file__))
+
+with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
+    long_description = "\n" + fh.read()
+
+VERSION = "1.0.6"
+DESCRIPTION = "A triple of tools used for plotting, handling key-words, and utilities"
+LONG_DESCRIPTION = ("Defaults: manages settings for classes that can be controlled easily from an interface.\n"
+                    "Plotting: a front end for matplotlib to easily create subplots.\n"
+                    "Utils: a collection of generally useful functions")
+
+# Setting up
+setup(
+    name="hgutilities",
+    version=VERSION,
+    author="Henry Ginn",
+    author_email="<henryginn137@gmail.com>",
+    description=DESCRIPTION,
+    long_description_content_type="text/markdown",
+    long_description=long_description,
+    setup_requires=['setuptools_scm'],
+    include_package_data=True,
+    install_requires=["matplotlib", "numpy", "screeninfo", "pillow"],
+    keywords=["python", "matplotlib", "plotting", "default", "keywords", "utils"],
+    classifiers=[
+        "Development Status :: 4 - Beta",
+        "Intended Audience :: Developers",
+        "Programming Language :: Python :: 3",
+        "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
+        "Natural Language :: English",
+        "Operating System :: Unix",
+        "Operating System :: Microsoft :: Windows",
+    ]
+)
```

